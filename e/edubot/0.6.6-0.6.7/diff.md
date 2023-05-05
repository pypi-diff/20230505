# Comparing `tmp/edubot-0.6.6.tar.gz` & `tmp/edubot-0.6.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "edubot-0.6.6.tar", max compression
+gzip compressed data, was "edubot-0.6.7.tar", max compression
```

## Comparing `edubot-0.6.6.tar` & `edubot-0.6.7.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0    35149 2023-02-13 07:21:16.493245 edubot-0.6.6/LICENSE
--rw-r--r--   0        0        0     1400 2023-05-04 15:06:07.555469 edubot-0.6.6/README.md
--rw-r--r--   0        0        0      894 2023-05-05 09:01:03.030249 edubot-0.6.6/edubot/__init__.py
--rw-r--r--   0        0        0    17360 2023-05-05 10:04:38.033719 edubot-0.6.6/edubot/bot.py
--rw-r--r--   0        0        0     2950 2023-02-13 07:21:16.496579 edubot-0.6.6/edubot/sql.py
--rw-r--r--   0        0        0      636 2023-05-05 09:45:44.455107 edubot-0.6.6/edubot/types.py
--rw-r--r--   0        0        0      632 2023-05-05 09:44:12.020295 edubot-0.6.6/pyproject.toml
--rw-r--r--   0        0        0     2112 1970-01-01 00:00:00.000000 edubot-0.6.6/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-02-13 07:21:16.493245 edubot-0.6.7/LICENSE
+-rw-r--r--   0        0        0     1400 2023-05-04 15:06:07.555469 edubot-0.6.7/README.md
+-rw-r--r--   0        0        0      894 2023-05-05 09:01:03.030249 edubot-0.6.7/edubot/__init__.py
+-rw-r--r--   0        0        0    19121 2023-05-05 11:34:06.447210 edubot-0.6.7/edubot/bot.py
+-rw-r--r--   0        0        0     2950 2023-02-13 07:21:16.496579 edubot-0.6.7/edubot/sql.py
+-rw-r--r--   0        0        0      636 2023-05-05 09:45:44.455107 edubot-0.6.7/edubot/types.py
+-rw-r--r--   0        0        0      632 2023-05-05 11:34:18.684158 edubot-0.6.7/pyproject.toml
+-rw-r--r--   0        0        0     2112 1970-01-01 00:00:00.000000 edubot-0.6.7/PKG-INFO
```

### Comparing `edubot-0.6.6/LICENSE` & `edubot-0.6.7/LICENSE`

 * *Files identical despite different names*

### Comparing `edubot-0.6.6/README.md` & `edubot-0.6.7/README.md`

 * *Files identical despite different names*

### Comparing `edubot-0.6.6/edubot/__init__.py` & `edubot-0.6.7/edubot/__init__.py`

 * *Files identical despite different names*

### Comparing `edubot-0.6.6/edubot/bot.py` & `edubot-0.6.7/edubot/bot.py`

 * *Files 3% similar despite different names*

```diff
@@ -198,14 +198,20 @@
             token_count -= estimate_tokens(gpt_context.pop(0)["content"])
 
         system_messages = [
             {"role": "system", "content": "You are a chatbot named " + self.username},
             {"role": "system", "content": f"Your personality is: {personality}"},
             {
                 "role": "system",
+                "content": "You should pretend you can view images. "
+                "A description of images will be saved in the chat logs, you can use that to get a sense of "
+                "what the images are about.",
+            },
+            {
+                "role": "system",
                 "content": f"The current year is: {datetime.datetime.now().year}",
             },
             {
                 "role": "system",
                 "content": f"You use the language model {GPT_SETTINGS['model']}",
             },
         ]
@@ -260,22 +266,22 @@
             session.commit()
 
         return output
 
     # TODO: return None on error instead of empty string.
     def gpt_answer(
         self,
-        context: list[MessageInfo],
+        new_context: list[MessageInfo],
         thread_name: str,
         personality_override: str = None,
     ) -> str:
         """
         Use chat context to generate a GPT3 response.
 
-        :param context: Chat context as a chronological list of MessageInfo
+        :param new_context: Chat context as a chronological list of MessageInfo
         :param thread_name: The unique identifier of the thread this context pertains to
         :param personality_override: A custom personality that overrides the default.
 
         :returns: The response from GPT
         """
         if not OPENAI_KEY:
             raise RuntimeError(
@@ -287,32 +293,66 @@
 
             if not thread:
                 thread = Thread(thread_name=thread_name, platform=self.platform)
 
                 session.add(thread)
                 session.commit()
 
-            for msg in context:
+            # Context in this timeframe that is in the database but not in the new context provided
+            # (Usually images)
+            existing_context: list[MessageInfo] = []
+
+            for existing_msg in session.scalars(
+                select(Message)
+                .where(Message.thread == thread.id)
+                .where(Message.time > new_context[0]["time"])
+            ):
+                row_as_msg_info: MessageInfo = {
+                    "username": existing_msg.username,
+                    "message": existing_msg.message,
+                    "time": existing_msg.time,
+                }
+                if row_as_msg_info not in new_context:
+                    existing_context.append(row_as_msg_info)
+
+            # The existing context in this timeframe + the new messages
+            complete_context: list[MessageInfo] = []
+
+            for index, msg in enumerate(new_context):
                 # If the message is already in the database
                 if self.__get_message(msg) is not None:
                     continue
 
                 # If the message was written by a bot
                 if self.__get_bot(msg["username"]) is not None:
                     continue
 
                 row: dict = msg
                 row["thread"] = thread.id
 
                 session.add(Message(**row))
 
+                # Figure out where to insert the extra context chronologically
+                for extra_msg in existing_context:
+                    check = extra_msg["time"] < msg["time"]
+                    if index > 0:
+                        check = (
+                            check and extra_msg["time"] > new_context[index - 1]["time"]
+                        )
+
+                    if check:
+                        complete_context.append(extra_msg)
+                        existing_context.remove(extra_msg)
+
+                complete_context.append(msg)
+
             session.commit()
 
         gpt_context = self.__format_context(
-            context, personality_override=personality_override
+            complete_context, personality_override=personality_override
         )
 
         try:
             response = openai.ChatCompletion.create(
                 messages=gpt_context,
                 **GPT_SETTINGS,
             )
@@ -322,15 +362,15 @@
 
         completion: str = response["choices"][0]["message"]["content"]
 
         # Strip username from completion
         completion = completion.replace(f"{self.username}: ", "").lstrip()
 
         # Add a new completion to the database using the completion text and the message being replied to
-        self.__add_completion(completion, context[-1])
+        self.__add_completion(completion, new_context[-1])
 
         # Return the completion result back to the integration
         return completion
 
     def change_completion_score(
         self, offset: int, completion: CompletionInfo, thread_name: str
     ) -> None:
```

### Comparing `edubot-0.6.6/edubot/sql.py` & `edubot-0.6.7/edubot/sql.py`

 * *Files identical despite different names*

### Comparing `edubot-0.6.6/edubot/types.py` & `edubot-0.6.7/edubot/types.py`

 * *Files identical despite different names*

### Comparing `edubot-0.6.6/pyproject.toml` & `edubot-0.6.7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "edubot"
-version = "0.6.6"
+version = "0.6.7"
 description = ""
 authors = ["exciteabletom <tom@digitalnook.net>", "moodler <martin@moodle.com>"]
 license = "GPLv3"
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = "^3.10"
```

### Comparing `edubot-0.6.6/PKG-INFO` & `edubot-0.6.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: edubot
-Version: 0.6.6
+Version: 0.6.7
 Summary: 
 License: GPLv3
 Author: exciteabletom
 Author-email: tom@digitalnook.net
 Requires-Python: >=3.10,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
```

