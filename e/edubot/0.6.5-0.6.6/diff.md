# Comparing `tmp/edubot-0.6.5.tar.gz` & `tmp/edubot-0.6.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "edubot-0.6.5.tar", max compression
+gzip compressed data, was "edubot-0.6.6.tar", max compression
```

## Comparing `edubot-0.6.5.tar` & `edubot-0.6.6.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0    35149 2022-11-24 18:21:26.784597 edubot-0.6.5/LICENSE
--rw-r--r--   0        0        0     1400 2023-03-29 15:28:01.248879 edubot-0.6.5/README.md
--rw-r--r--   0        0        0      813 2023-02-23 10:23:15.963305 edubot-0.6.5/edubot/__init__.py
--rw-r--r--   0        0        0    15338 2023-03-29 16:09:27.258084 edubot-0.6.5/edubot/bot.py
--rw-r--r--   0        0        0     2950 2023-02-23 10:32:46.665675 edubot-0.6.5/edubot/sql.py
--rw-r--r--   0        0        0      353 2023-01-07 10:48:32.725588 edubot-0.6.5/edubot/types.py
--rw-r--r--   0        0        0      611 2023-03-29 16:16:14.940637 edubot-0.6.5/pyproject.toml
--rw-r--r--   0        0        0     2070 1970-01-01 00:00:00.000000 edubot-0.6.5/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-02-13 07:21:16.493245 edubot-0.6.6/LICENSE
+-rw-r--r--   0        0        0     1400 2023-05-04 15:06:07.555469 edubot-0.6.6/README.md
+-rw-r--r--   0        0        0      894 2023-05-05 09:01:03.030249 edubot-0.6.6/edubot/__init__.py
+-rw-r--r--   0        0        0    17360 2023-05-05 10:04:38.033719 edubot-0.6.6/edubot/bot.py
+-rw-r--r--   0        0        0     2950 2023-02-13 07:21:16.496579 edubot-0.6.6/edubot/sql.py
+-rw-r--r--   0        0        0      636 2023-05-05 09:45:44.455107 edubot-0.6.6/edubot/types.py
+-rw-r--r--   0        0        0      632 2023-05-05 09:44:12.020295 edubot-0.6.6/pyproject.toml
+-rw-r--r--   0        0        0     2112 1970-01-01 00:00:00.000000 edubot-0.6.6/PKG-INFO
```

### Comparing `edubot-0.6.5/LICENSE` & `edubot-0.6.6/LICENSE`

 * *Files identical despite different names*

### Comparing `edubot-0.6.5/README.md` & `edubot-0.6.6/README.md`

 * *Files identical despite different names*

### Comparing `edubot-0.6.5/edubot/__init__.py` & `edubot-0.6.6/edubot/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -20,8 +20,9 @@
     return config
 
 
 CONFIG = _read_cfg()
 
 OPENAI_KEY: str | None = CONFIG.get("edubot", "openai_key", fallback=None)
 DREAMSTUDIO_KEY: str | None = CONFIG.get("edubot", "dreamstudio_key", fallback=None)
+REPLICATE_KEY: str | None = CONFIG.get("edubot", "replicate_key", fallback=None)
 DATABASE: str = CONFIG.get("edubot", "database")
```

### Comparing `edubot-0.6.5/edubot/bot.py` & `edubot-0.6.6/edubot/bot.py`

 * *Files 6% similar despite different names*

```diff
@@ -3,30 +3,34 @@
 """
 import datetime
 import io
 import logging
 
 import openai
 import PIL
+import replicate
 import trafilatura
 from openai import OpenAIError
 from PIL import Image
 from sqlalchemy import desc, select
 from stability_sdk.client import StabilityInference, process_artifacts_from_answers
 from stability_sdk.utils import generation
 
-from edubot import DREAMSTUDIO_KEY, OPENAI_KEY
+from edubot import DREAMSTUDIO_KEY, OPENAI_KEY, REPLICATE_KEY
 from edubot.sql import Bot, Completion, Message, Session, Thread
-from edubot.types import CompletionInfo, MessageInfo
+from edubot.types import CompletionInfo, ImageInfo, MessageInfo
 
 # The maximum number of GPT tokens that chat context can be.
 # The limit for GPT-4 is 8192.
 # We limit to 7800 to allow extra room for the response and the personality.
 MAX_GPT_TOKENS = 7200
 
+# The maximum allowed size of images in megabytes
+MAX_IMAGE_SIZE_MB = 50
+
 # Prompt for GPT to summarise web pages
 WEB_SUMMARY_PROMPT = (
     "Your input is scraped text from a website. Your job is to summarise the text and post it to a chatroom.\n"
     "Long-form text includes pages such as news articles and blog posts.\n"
     "If the page doesn't contain long-form text return the phrase 'NO CONTENT' and nothing else.\n"
     "If the page mentions any variation of 'requiring javascript', or 'enable javascript' you should also return 'NO CONTENT' and nothing else.\n"
     "If the page DOES contain long-form text return a brief 2 sentence summary of the text content. "
@@ -34,14 +38,16 @@
 )
 
 # Settings for GPT completion generation
 GPT_SETTINGS = {"model": "gpt-4", "temperature": 0.3, "max_tokens": 700}
 
 logger = logging.getLogger(__name__)
 
+REPLICATE_CLIENT = replicate.Client(api_token=REPLICATE_KEY)
+
 
 # TODO: use tiktoken for this, the function is currently inaccurate
 def estimate_tokens(text: str) -> int:
     """
     Roughly estimates how many GPT tokens a string is.
     See: https://help.openai.com/en/articles/4936856-what-are-tokens-and-how-to-count-them
 
@@ -202,14 +208,63 @@
                 "role": "system",
                 "content": f"You use the language model {GPT_SETTINGS['model']}",
             },
         ]
 
         return system_messages + gpt_context
 
+    def save_image_to_context(self, image: ImageInfo, thread_name: str) -> str | None:
+        """
+        Saves an AI generated description of an image to the database. This allows GPT to understand what images are
+         and how to describe them. The maximum image size in MB can be read from the MAX_IMAGE_SIZE_MB constant.
+
+        :param image: An ImageInfo object.
+        :param thread_name: A unique identifier for the thread the image was posted in.
+        :returns: The description of the image or None if an error occurred.
+        """
+        if not REPLICATE_KEY:
+            raise RuntimeError(
+                "Replicate key is not defined, make sure to supply it in the config."
+            )
+
+        image_bytes = io.BytesIO()
+        image["image"].save(image_bytes, format="PNG")
+
+        if image_bytes.tell() / 1048576 > MAX_IMAGE_SIZE_MB:
+            logger.info(f"Skipped image in {thread_name} because it was too large.")
+            return
+
+        output: str = REPLICATE_CLIENT.run(
+            "j-min/clip-caption-reward:de37751f75135f7ebbe62548e27d6740d5155dfefdf6447db35c9865253d7e06",
+            input={"image": image_bytes},
+        )
+
+        if not output:
+            logger.error("Replicate returned an empty response.")
+            return
+
+        with Session() as session:
+            thread = self.__get_thread(thread_name)
+            if not thread:
+                thread = Thread(thread_name=thread_name, platform=self.platform)
+                session.add(thread)
+                session.commit()
+
+            message = Message(
+                thread=thread.id,
+                username=image["username"],
+                message=f"*An image of {output}",
+                time=image["time"],
+            )
+
+            session.add(message)
+            session.commit()
+
+        return output
+
     # TODO: return None on error instead of empty string.
     def gpt_answer(
         self,
         context: list[MessageInfo],
         thread_name: str,
         personality_override: str = None,
     ) -> str:
```

### Comparing `edubot-0.6.5/edubot/sql.py` & `edubot-0.6.6/edubot/sql.py`

 * *Files identical despite different names*

### Comparing `edubot-0.6.5/pyproject.toml` & `edubot-0.6.6/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 [tool.poetry]
 name = "edubot"
-version = "0.6.5"
+version = "0.6.6"
 description = ""
 authors = ["exciteabletom <tom@digitalnook.net>", "moodler <martin@moodle.com>"]
 license = "GPLv3"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.10"
 sqlalchemy = {version = ">=1.4.45,<1.5.0", extras = ["mypy"]}
 openai = "^0.27.2"
 stability-sdk = "^0.4.0"
 pillow = "^9.4.0"
 beautifulsoup4 = "^4.11.2"
 trafilatura = "^1.4.1"
+replicate = "^0.8.1"
 
 [tool.poetry.dev-dependencies]
 pre-commit = "^3.2.0"
 mypy = "^1.1.1"
 
 [tool.mypy]
 plugins = "sqlalchemy.ext.mypy.plugin"
```

### Comparing `edubot-0.6.5/PKG-INFO` & `edubot-0.6.6/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 Metadata-Version: 2.1
 Name: edubot
-Version: 0.6.5
+Version: 0.6.6
 Summary: 
 License: GPLv3
 Author: exciteabletom
 Author-email: tom@digitalnook.net
 Requires-Python: >=3.10,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: beautifulsoup4 (>=4.11.2,<5.0.0)
 Requires-Dist: openai (>=0.27.2,<0.28.0)
 Requires-Dist: pillow (>=9.4.0,<10.0.0)
+Requires-Dist: replicate (>=0.8.1,<0.9.0)
 Requires-Dist: sqlalchemy[mypy] (>=1.4.45,<1.5.0)
 Requires-Dist: stability-sdk (>=0.4.0,<0.5.0)
 Requires-Dist: trafilatura (>=1.4.1,<2.0.0)
 Description-Content-Type: text/markdown
 
 # Edubot
```

