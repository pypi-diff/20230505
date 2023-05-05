# Comparing `tmp/hugchat-0.0.5.3.tar.gz` & `tmp/hugchat-0.0.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hugchat-0.0.5.3.tar", last modified: Thu May  4 13:54:51 2023, max compression
+gzip compressed data, was "hugchat-0.0.5.4.tar", last modified: Fri May  5 13:53:29 2023, max compression
```

## Comparing `hugchat-0.0.5.3.tar` & `hugchat-0.0.5.4.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-05-04 13:54:51.791249 hugchat-0.0.5.3/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    34523 2023-05-01 00:33:11.000000 hugchat-0.0.5.3/LICENSE
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2836 2023-05-04 13:54:51.791249 hugchat-0.0.5.3/PKG-INFO
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1816 2023-05-04 13:53:20.000000 hugchat-0.0.5.3/README.md
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)       38 2023-05-04 13:54:51.791249 hugchat-0.0.5.3/setup.cfg
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1407 2023-05-04 13:53:59.000000 hugchat-0.0.5.3/setup.py
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-05-04 13:54:51.783249 hugchat-0.0.5.3/src/
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-05-04 13:54:51.787249 hugchat-0.0.5.3/src/hugchat/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)        0 2023-05-03 15:54:22.000000 hugchat-0.0.5.3/src/hugchat/__init__.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      179 2023-05-03 15:54:22.000000 hugchat-0.0.5.3/src/hugchat/cli.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     6405 2023-05-04 13:53:20.000000 hugchat-0.0.5.3/src/hugchat/hugchat.py
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-05-04 13:54:51.791249 hugchat-0.0.5.3/src/hugchat.egg-info/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2836 2023-05-04 13:54:51.000000 hugchat-0.0.5.3/src/hugchat.egg-info/PKG-INFO
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      266 2023-05-04 13:54:51.000000 hugchat-0.0.5.3/src/hugchat.egg-info/SOURCES.txt
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)        1 2023-05-04 13:54:51.000000 hugchat-0.0.5.3/src/hugchat.egg-info/dependency_links.txt
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)        9 2023-05-04 13:54:51.000000 hugchat-0.0.5.3/src/hugchat.egg-info/requires.txt
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)        8 2023-05-04 13:54:51.000000 hugchat-0.0.5.3/src/hugchat.egg-info/top_level.txt
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-05-05 13:53:29.555837 hugchat-0.0.5.4/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    34523 2023-05-01 00:33:11.000000 hugchat-0.0.5.4/LICENSE
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2874 2023-05-05 13:53:29.555837 hugchat-0.0.5.4/PKG-INFO
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1854 2023-05-05 02:29:43.000000 hugchat-0.0.5.4/README.md
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)       38 2023-05-05 13:53:29.555837 hugchat-0.0.5.4/setup.cfg
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     1407 2023-05-05 13:53:22.000000 hugchat-0.0.5.4/setup.py
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-05-05 13:53:29.543836 hugchat-0.0.5.4/src/
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-05-05 13:53:29.551836 hugchat-0.0.5.4/src/hugchat/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)        0 2023-05-03 15:54:22.000000 hugchat-0.0.5.4/src/hugchat/__init__.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      179 2023-05-03 15:54:22.000000 hugchat-0.0.5.4/src/hugchat/cli.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     8764 2023-05-05 13:53:16.000000 hugchat-0.0.5.4/src/hugchat/hugchat.py
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2023-05-05 13:53:29.555837 hugchat-0.0.5.4/src/hugchat.egg-info/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2874 2023-05-05 13:53:29.000000 hugchat-0.0.5.4/src/hugchat.egg-info/PKG-INFO
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      266 2023-05-05 13:53:29.000000 hugchat-0.0.5.4/src/hugchat.egg-info/SOURCES.txt
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)        1 2023-05-05 13:53:29.000000 hugchat-0.0.5.4/src/hugchat.egg-info/dependency_links.txt
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)        9 2023-05-05 13:53:29.000000 hugchat-0.0.5.4/src/hugchat.egg-info/requires.txt
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)        8 2023-05-05 13:53:29.000000 hugchat-0.0.5.4/src/hugchat.egg-info/top_level.txt
```

### Comparing `hugchat-0.0.5.3/LICENSE` & `hugchat-0.0.5.4/LICENSE`

 * *Files identical despite different names*

### Comparing `hugchat-0.0.5.3/PKG-INFO` & `hugchat-0.0.5.4/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hugchat
-Version: 0.0.5.3
+Version: 0.0.5.4
 Summary: A huggingchat python api.
 Home-page: https://github.com/Soulter/hugging-chat-api
 Author: Soulter
 Author-email: 905617992@qq.com
 License: GNU Affero General Public License v3.0
 Project-URL: Bug Report, https://github.com/Soulter/hugging-chat-api/issues
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
@@ -20,14 +20,16 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # hugging-chat-api
 
+English | [简体中文](README_cn.md)
+
 HuggingChat Python API
 
 [![PyPi](https://img.shields.io/pypi/v/hugchat.svg)](https://pypi.python.org/pypi/hugchat)
 [![Support_Platform](https://img.shields.io/pypi/pyversions/hugchat)](https://pypi.python.org/pypi/hugchat)
 [![Downloads](https://static.pepy.tech/badge/hugchat)](https://pypi.python.org/pypi/hugchat)
 
 Leave a star :)
@@ -49,15 +51,15 @@
 id = chatbot.new_conversation()
 chatbot.change_conversation(id)
 
 # Get conversation list
 conversation_list = chatbot.get_conversation_list()
 ```
 
-The `chat()` function can receive many parameters:
+The `chat()` function receives these parameters:
 
 - `text`: Required[str].
 - `temperature`: Optional[float]. Default is 0.9
 - `top_p`: Optional[float]. Default is 0.95
 - `repetition_penalty`: Optional[float]. Default is 1.2
 - `top_k`: Optional[int]. Default is 50
 - `truncate`: Optional[int]. Default is 1024
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `hugchat-0.0.5.3/README.md` & `hugchat-0.0.5.4/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,11 @@
 # hugging-chat-api
 
+English | [简体中文](README_cn.md)
+
 HuggingChat Python API
 
 [![PyPi](https://img.shields.io/pypi/v/hugchat.svg)](https://pypi.python.org/pypi/hugchat)
 [![Support_Platform](https://img.shields.io/pypi/pyversions/hugchat)](https://pypi.python.org/pypi/hugchat)
 [![Downloads](https://static.pepy.tech/badge/hugchat)](https://pypi.python.org/pypi/hugchat)
 
 Leave a star :)
@@ -25,15 +27,15 @@
 id = chatbot.new_conversation()
 chatbot.change_conversation(id)
 
 # Get conversation list
 conversation_list = chatbot.get_conversation_list()
 ```
 
-The `chat()` function can receive many parameters:
+The `chat()` function receives these parameters:
 
 - `text`: Required[str].
 - `temperature`: Optional[float]. Default is 0.9
 - `top_p`: Optional[float]. Default is 0.95
 - `repetition_penalty`: Optional[float]. Default is 1.2
 - `top_k`: Optional[int]. Default is 50
 - `truncate`: Optional[int]. Default is 1024
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `hugchat-0.0.5.3/setup.py` & `hugchat-0.0.5.4/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import find_namespace_packages
 from setuptools import setup
 
 setup(
     name="hugchat",
-    version="0.0.5.3",
+    version="0.0.5.4",
     description="A huggingchat python api.",
     long_description=open("README.md", "rt", encoding="utf-8").read(),
     long_description_content_type="text/markdown",
     url="https://github.com/Soulter/hugging-chat-api",
     project_urls={
         "Bug Report": "https://github.com/Soulter/hugging-chat-api/issues"
     },
```

### Comparing `hugchat-0.0.5.3/src/hugchat/hugchat.py` & `hugchat-0.0.5.4/src/hugchat/hugchat.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,23 +1,28 @@
+import random
+import string
 from requests import Session
 import json
 import uuid
-
-hf_url = "https://huggingface.co/chat"
-
+from requests_toolbelt import MultipartEncoder
 
 class ChatBot:
     def __init__(self) -> None:
+        self.hf_base_url = "https://huggingface.co"
+        self.json_header = {"Content-Type": "application/json"}
         self.session = self.get_hc_session()
         self.conversation_id_list = []
+        self.active_model = "OpenAssistant/oasst-sft-6-llama-30b-xor"
+        self.accepted_welcome_modal = False # Only when accepted, it can create a new conversation.
         self.current_conversation = self.new_conversation()
 
+
     def get_hc_session(self) -> Session:
         session = Session()
-        session.get(hf_url)
+        session.get(self.hf_base_url + "/chat")
         return session
     
     def change_conversation(self, conversation_id: str) -> bool:
         if conversation_id not in self.conversation_id_list:
             raise Exception("Invalid conversation id. Please check conversation id list.")
         self.current_conversation = conversation_id
         return True
@@ -31,18 +36,47 @@
     #
     # Returns a pointer to this objects list that contains id of conversations.
     def get_conversation_list(self) -> list:
         return list(self.conversation_id_list)
     
     def new_conversation(self) -> str:
         err_count = 0
+
+        # Accept the welcome modal when init.
+        if not self.accepted_welcome_modal:
+            boundary = "----WebKitFormBoundary" + ''.join(random.sample(string.ascii_letters + string.digits, 16))
+            headers = {
+                "Content-Type": f"multipart/form-data; boundary={boundary}",
+                "Origin": self.hf_base_url,
+                "Referer": self.hf_base_url + "/chat/",
+                "Sec-Fetch-Dest": "empty",
+                "Sec-Fetch-Mode": "cors",
+                "Sec-Fetch-Site": "same-origin",
+                "User-Agent": "Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/112.0.0.0 Safari/537.36 Edg/112.0.1722.64",
+                "Accept": "application/json",
+            }
+            welcome_modal_fields = {
+                "ethicsModalAccepted": "true",
+                "shareConversationsWithModelAuthors": "true",
+                "ethicsModalAcceptedAt": "",
+                "activeModel": self.active_model,
+            }
+            m = MultipartEncoder(fields=welcome_modal_fields, boundary=boundary)
+            res = self.session.post(self.hf_base_url + "/chat/settings", headers=headers, data=m)
+            # result_json = json.loads(res.text)
+            # if result_json['type'] == "redirect" and result_json['status'] == 303:
+            self.accepted_welcome_modal = True
+            # print(res.request.body)
+            # print(res.text)
+
+        # Create new conversation and get a conversation id.
         resp = ""
         while True:
             try:
-                resp = self.session.post(hf_url + "/conversation", json={"model": "OpenAssistant/oasst-sft-6-llama-30b-xor"}, headers={"Content-Type": "application/json"})
+                resp = self.session.post(self.hf_base_url + "/chat/conversation", json={"model": self.active_model}, headers=self.json_header)
                 # print(resp.text)
                 cid = json.loads(resp.text)['conversationId']
                 self.conversation_id_list.append(cid)
                 return cid
             except BaseException as e:
                 err_count += 1
                 print(f"[Error] Failed to create new conversation. Retrying... ({err_count})")
@@ -95,26 +129,26 @@
                     "id": str(uuid.uuid4()),
             },
         }
         # print(req_json)
         # print(self.session.cookies.get_dict())
         # print(f"https://huggingface.co/chat/conversation/{self.now_conversation}")
         headers = {
-            "Origin": "https://huggingface.co",
-            "Referer": f"https://huggingface.co/chat/conversation/{self.current_conversation}",
+            **self.json_header,
+            "Origin": self.hf_base_url,
+            "Referer": self.hf_base_url + f"/chat/conversation/{self.current_conversation}",
             "Sec-Fetch-Dest": "empty",
             "Sec-Fetch-Mode": "cors",
             "Sec-Fetch-Site": "same-origin",
             "User-Agent": "Mozilla/5.0 (Windows NT 10.0; Win64; x64) AppleWebKit/537.36 (KHTML, like Gecko) Chrome/112.0.0.0 Safari/537.36 Edg/112.0.1722.64",
-            "Content-Type": "application/json",
             "Accept": "*/*",
         }
 
         while retry_count > 0:
-            resp = self.session.post(hf_url + f"/conversation/{self.current_conversation}", json=req_json, stream=True, headers=headers, cookies=self.session.cookies.get_dict())
+            resp = self.session.post(self.hf_base_url + f"/chat/conversation/{self.current_conversation}", json=req_json, stream=True, headers=headers, cookies=self.session.cookies.get_dict())
             res_text = ""
             if resp.status_code == 200:
                 for line in resp.iter_lines():
                     if line:
                         res = line.decode("utf-8")
                         obj = json.loads(res[1:-1])
                         if "generated_text" in obj:
@@ -124,36 +158,41 @@
                 return res_text
             else:
                 retry_count -= 1
                 if retry_count <= 0:
                     raise Exception(f"Failed to chat. ({resp.status_code})")
 
 def cli():
-    chatbot = ChatBot()
     print("-------HuggingChat-------")
+    print("1. AI is an area of active research with known problems such as biased generation and misinformation. Do not use this application for high-stakes decisions or advice.\n2. Your conversations will be shared with model authors.\nContinuing to use means that you accept the above points")
+    chatbot = ChatBot()
     running = True
     while running:
         question = input("> ")
         if question == "/new":
             cid = chatbot.new_conversation()
             print("The new conversation ID is: " + cid)
             chatbot.change_conversation(cid)
             print("Conversation changed successfully.")
             continue
         
         elif question.startswith("/switch"):
             try:
-                _index = int(question.split(" ")[1])
+                conversations = chatbot.get_conversation_list()
+                conversation_id = str(question.split(" ")[1] if len(question.split(" ")) > 1 else "")
+                if conversation_id not in conversations:
+                    print("# Please enter a valid ID number.")
+                    print(f"# Sessions include: {conversations}")
+                else:
+                    chatbot.change_conversation(conversation_id)
+                    print(f"# Conversation switched successfully to {conversation_id}")
             except ValueError:
                 print("# Please enter a valid ID number\n")
             
-            if len(chatbot.get_conversation_list()) < _index-1:
-                print("# Please enter a valid ID number")
-            else:
-                chatbot.change_conversation(list(chatbot.get_conversation_list())[_index-1])
+            
         
         elif question == "/ids":
             id_list = list(chatbot.get_conversation_list())
             [print(f"{id_list.index(i)+1} : {i}{' <active>' if chatbot.current_conversation == i else ''}") for i in id_list]
         
         elif question in ["/exit", "/quit","/close"]:
             running = False
```

### Comparing `hugchat-0.0.5.3/src/hugchat.egg-info/PKG-INFO` & `hugchat-0.0.5.4/src/hugchat.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hugchat
-Version: 0.0.5.3
+Version: 0.0.5.4
 Summary: A huggingchat python api.
 Home-page: https://github.com/Soulter/hugging-chat-api
 Author: Soulter
 Author-email: 905617992@qq.com
 License: GNU Affero General Public License v3.0
 Project-URL: Bug Report, https://github.com/Soulter/hugging-chat-api/issues
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
@@ -20,14 +20,16 @@
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # hugging-chat-api
 
+English | [简体中文](README_cn.md)
+
 HuggingChat Python API
 
 [![PyPi](https://img.shields.io/pypi/v/hugchat.svg)](https://pypi.python.org/pypi/hugchat)
 [![Support_Platform](https://img.shields.io/pypi/pyversions/hugchat)](https://pypi.python.org/pypi/hugchat)
 [![Downloads](https://static.pepy.tech/badge/hugchat)](https://pypi.python.org/pypi/hugchat)
 
 Leave a star :)
@@ -49,15 +51,15 @@
 id = chatbot.new_conversation()
 chatbot.change_conversation(id)
 
 # Get conversation list
 conversation_list = chatbot.get_conversation_list()
 ```
 
-The `chat()` function can receive many parameters:
+The `chat()` function receives these parameters:
 
 - `text`: Required[str].
 - `temperature`: Optional[float]. Default is 0.9
 - `top_p`: Optional[float]. Default is 0.95
 - `repetition_penalty`: Optional[float]. Default is 1.2
 - `top_k`: Optional[int]. Default is 50
 - `truncate`: Optional[int]. Default is 1024
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

