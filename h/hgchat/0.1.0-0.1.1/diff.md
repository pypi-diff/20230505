# Comparing `tmp/hgchat-0.1.0.tar.gz` & `tmp/hgchat-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hgchat-0.1.0.tar", max compression
+gzip compressed data, was "hgchat-0.1.1.tar", max compression
```

## Comparing `hgchat-0.1.0.tar` & `hgchat-0.1.1.tar`

### file list

```diff
@@ -1,5 +1,4 @@
--rw-r--r--   0        0        0      240 2023-04-29 11:50:06.142215 hgchat-0.1.0/README.md
--rw-r--r--   0        0        0     2343 2023-04-29 12:02:44.236868 hgchat-0.1.0/hgchat/__init__.py
--rw-r--r--   0        0        0      278 2023-04-29 11:50:19.975966 hgchat-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      843 1970-01-01 00:00:00.000000 hgchat-0.1.0/setup.py
--rw-r--r--   0        0        0      609 1970-01-01 00:00:00.000000 hgchat-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0      683 2023-04-30 10:09:45.807393 hgchat-0.1.1/README.md
+-rw-r--r--   0        0        0     2684 2023-05-04 23:28:08.663907 hgchat-0.1.1/hgchat/__init__.py
+-rw-r--r--   0        0        0      409 2023-05-04 23:27:42.726826 hgchat-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     1052 1970-01-01 00:00:00.000000 hgchat-0.1.1/PKG-INFO
```

### Comparing `hgchat-0.1.0/hgchat/__init__.py` & `hgchat-0.1.1/hgchat/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,40 +1,43 @@
 import json 
 import requests
 
+__version__ = "0.1.1"
+
 class Chat:
     def __init__(self, id:int) -> None:
         self.id = id
 
     @property
     def url(self):
         return f"https://huggingface.co/chat/conversation/{self.id}"
 
     
 class HGChat:
-    def __init__(self) -> None:
+    def __init__(self, model:str=None) -> None:
         self.chat = None
         self.session = self.make_session()
+        self.model = "OpenAssistant/oasst-sft-6-llama-30b-xor" if model is None else model
 
     def make_session(self) -> requests.Session:
         session = requests.Session()
         session.get(url="https://huggingface.co/chat/")
         return session
 
     def get_chat(self, id:int=None) -> Chat:
         if self.chat is None:
             self.chat = self.new_chat()
         return self.chat
 
     def new_chat(self) -> Chat:
-        r = self.session.post(url="https://huggingface.co/chat/conversation")
+        r = self.session.post(url="https://huggingface.co/chat/conversation", json={"model": self.model}, headers={"Content-Type": "application/json"})
         if r.status_code != 200:
             raise Exception("Failed to create new conversation")
         else:
-            return Chat(id=r.json()["conversationId"])
+            return Chat(id=json.loads(r.text)['conversationId'])
        
 
     def ask(self, message:str, temperature: float = 0.9, top_p: float = 0.95, repetition_penalty: float = 1.2, top_k: int = 50, truncate: int = 1024, watermark: bool = False, max_new_tokens: int = 1024) -> None:
         self.get_chat()
         r = self.session.post(
             url=self.chat.url, 
             json={
@@ -59,14 +62,20 @@
             },
             stream=True
         )
         if r.status_code != 200:
             raise Exception("Failed to send message")
 
         for chunk in r.iter_content(chunk_size=None):
+            data = chunk.decode("utf-8")
             if chunk:
-                data = json.loads(chunk.decode("utf-8")[5:])
+                data = json.loads(chunk[5:])
                 if "error" not in data:
                     yield data
                 else:
                     print("error: ", data["error"])
                     break
+
+if __name__ == "__main__":
+    chat = HGChat()
+    for data in chat.ask("Hello"):
+        print(data)
```

