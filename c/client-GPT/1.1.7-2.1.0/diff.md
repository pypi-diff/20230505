# Comparing `tmp/client_GPT-1.1.7.tar.gz` & `tmp/client_GPT-2.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "client_GPT-1.1.7.tar", last modified: Mon May  1 16:58:02 2023, max compression
+gzip compressed data, was "client_GPT-2.1.0.tar", last modified: Fri May  5 12:35:26 2023, max compression
```

## Comparing `client_GPT-1.1.7.tar` & `client_GPT-2.1.0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-05-01 16:58:02.515378 client_GPT-1.1.7/
--rw-rw-rw-   0        0        0      419 2023-05-01 16:58:02.514380 client_GPT-1.1.7/PKG-INFO
--rw-rw-rw-   0        0        0      425 2023-04-27 14:12:47.000000 client_GPT-1.1.7/README.md
-drwxrwxrwx   0        0        0        0 2023-05-01 16:58:02.500381 client_GPT-1.1.7/client_GPT.egg-info/
--rw-rw-rw-   0        0        0      419 2023-05-01 16:58:02.000000 client_GPT-1.1.7/client_GPT.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      235 2023-05-01 16:58:02.000000 client_GPT-1.1.7/client_GPT.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-01 16:58:02.000000 client_GPT-1.1.7/client_GPT.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-05-01 16:58:02.000000 client_GPT-1.1.7/client_GPT.egg-info/requires.txt
--rw-rw-rw-   0        0        0       11 2023-05-01 16:58:02.000000 client_GPT-1.1.7/client_GPT.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-05-01 16:58:02.513379 client_GPT-1.1.7/client_gpt/
--rw-rw-rw-   0        0        0        0 2023-04-27 13:20:09.000000 client_GPT-1.1.7/client_gpt/__init__.py
--rw-rw-rw-   0        0        0     4087 2023-05-01 16:57:46.000000 client_GPT-1.1.7/client_gpt/client_gpt.py
--rw-rw-rw-   0        0        0       42 2023-05-01 16:58:02.516380 client_GPT-1.1.7/setup.cfg
--rw-rw-rw-   0        0        0      591 2023-05-01 16:57:55.000000 client_GPT-1.1.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-05 12:35:26.391035 client_GPT-2.1.0/
+-rw-rw-rw-   0        0        0      419 2023-05-05 12:35:26.390081 client_GPT-2.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0      425 2023-04-27 14:12:47.000000 client_GPT-2.1.0/README.md
+drwxrwxrwx   0        0        0        0 2023-05-05 12:35:26.384037 client_GPT-2.1.0/client_GPT.egg-info/
+-rw-rw-rw-   0        0        0      419 2023-05-05 12:35:26.000000 client_GPT-2.1.0/client_GPT.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      235 2023-05-05 12:35:26.000000 client_GPT-2.1.0/client_GPT.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-05 12:35:26.000000 client_GPT-2.1.0/client_GPT.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-05-05 12:35:26.000000 client_GPT-2.1.0/client_GPT.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       11 2023-05-05 12:35:26.000000 client_GPT-2.1.0/client_GPT.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-05 12:35:26.387035 client_GPT-2.1.0/client_gpt/
+-rw-rw-rw-   0        0        0        0 2023-04-27 13:20:09.000000 client_GPT-2.1.0/client_gpt/__init__.py
+-rw-rw-rw-   0        0        0     3974 2023-05-05 12:30:42.000000 client_GPT-2.1.0/client_gpt/client_gpt.py
+-rw-rw-rw-   0        0        0       42 2023-05-05 12:35:26.391035 client_GPT-2.1.0/setup.cfg
+-rw-rw-rw-   0        0        0      591 2023-05-05 12:35:10.000000 client_GPT-2.1.0/setup.py
```

### Comparing `client_GPT-1.1.7/client_gpt/client_gpt.py` & `client_GPT-2.1.0/client_gpt/client_gpt.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,38 +1,38 @@
 import requests
 import json
 import re
 import uuid
 import os
-from typing import Tuple
+from typing import Tuple, Optional
 
 
 class ClientGPT:
     """
     A class for interacting with the OpenAI API.
     Attributes:
         api_key (str): Your OpenAI API key.
         model (str): The ID of the GPT-3 model to use.
         conversation_id (str or None): the unique identifier of the current conversation in the OpenAI. If the value is None, a new conversation ID will be created. If a string is passed, then an existing conversation ID is used.
         session (requests.Session): A session object for making HTTP requests.
     Method:
         ask(prompt, conversation_id=None, previous_convo_id=None): Sends a prompt to the OpenAI API and returns the response.
     """
-    
+
     chat_api_url = "https://api.openai.com/v1/completions"
 
     def __init__(self, api_key: str, model: str):
         self.api_key = api_key
         self.model = model
         self.conversation_id = None
         self.session = requests.Session()
 
     def ask(
         self, prompt: str, conversation_id: str or None, previous_convo_id: str or None
-    ) -> Tuple[str, str or None, str or None]:
+    ) -> Optional[str]:
         """
         Args:
             prompt (str): a string containing text to send to the OpenAI server.
             conversation_id (str or None): The ID of the conversation. If None, a new conversation will be started.
             previous_convo_id (str or None): The ID of the previous conversation. If None, a new conversation will be started.
 
         Return:
@@ -45,14 +45,19 @@
             "OpenAI-Integration-Name": "python",
             "OpenAI-Integration-Version": "0.1",
         }
 
         data = {
             "model": self.model,
             "prompt": prompt,
+            "max_tokens": 150,
+            "temperature": 0.3,
+            "n": 1,
+            "echo": True,
+            "stream": False,
         }
 
         if previous_convo_id is None:
             previous_convo_id = str(uuid.uuid4())
 
         if conversation_id is not None and len(conversation_id) == 0:
             conversation_id = None
@@ -60,25 +65,22 @@
         try:
             response = self.session.post(
                 self.chat_api_url,
                 headers=headers,
                 data=json.dumps(data),
             )
             if response.status_code == 200:
-                response_text = response.text.replace("data: [DONE]", "")
-                data = re.findall(r"data: (.*)", response_text)[-1]
-                as_json = json.loads(data)
-                print(as_json["message"]["content"]["parts"][0],
-                    as_json["message"]["id"],
-                    as_json["conversation_id"],)
-                return (
-                    as_json["message"]["content"]["parts"][0],
-                    as_json["message"]["id"],
-                    as_json["conversation_id"],
-                )
+                response_data = json.loads(response.text)
+                choices = response_data["choices"]
+                print(choices)
+                if len(choices) > 0:
+                    text = choices[0]["text"]
+                    return text
+                else:
+                    return None
             elif response.status_code == 401:
                 if os.path.exists("auth.json"):
                     os.remove("auth.json")
                 return (
                     f"[Status Code] 401 | [Response Text] {response.text}",
                     None,
                     None,
```

### Comparing `client_GPT-1.1.7/setup.py` & `client_GPT-2.1.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import setuptools
 
 setuptools.setup(
     name="client_GPT",
-    version="1.1.7",
+    version="2.1.0",
     author="littleknitsstory",
     description="A package for working with GPT language models.",
     url="https://github.com/littleknitsstory/client-gpt",
     packages=setuptools.find_packages(),
     install_requires=[
         "requests",
     ],
```

