# Comparing `tmp/pyroporn-0.0.2.tar.gz` & `tmp/pyroporn-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyroporn-0.0.2.tar", last modified: Fri May  5 09:03:04 2023, max compression
+gzip compressed data, was "pyroporn-0.0.3.tar", last modified: Fri May  5 09:14:49 2023, max compression
```

## Comparing `pyroporn-0.0.2.tar` & `pyroporn-0.0.3.tar`

### file list

```diff
@@ -1,53 +1,53 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 09:03:04.177327 pyroporn-0.0.2/
--rw-r--r--   0 runner    (1001) docker     (123)      949 2023-05-05 09:03:04.177327 pyroporn-0.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-05-05 09:02:52.000000 pyroporn-0.0.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 09:03:04.173327 pyroporn-0.0.2/pyroporn/
--rw-r--r--   0 runner    (1001) docker     (123)       86 2023-05-05 09:02:52.000000 pyroporn-0.0.2/pyroporn/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    20659 2023-05-05 09:02:52.000000 pyroporn-0.0.2/pyroporn/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     6623 2023-05-05 09:02:52.000000 pyroporn-0.0.2/pyroporn/config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 09:03:04.173327 pyroporn-0.0.2/pyroporn/database/
--rw-r--r--   0 runner    (1001) docker     (123)      355 2023-05-05 09:02:52.000000 pyroporn-0.0.2/pyroporn/database/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5622 2023-05-05 09:02:52.000000 pyroporn-0.0.2/pyroporn/database/bdbDatabase.py
--rw-r--r--   0 runner    (1001) docker     (123)     1220 2023-05-05 09:02:52.000000 pyroporn-0.0.2/pyroporn/database/bubDatabase.py
--rw-r--r--   0 runner    (1001) docker     (123)     5839 2023-05-05 09:02:52.000000 pyroporn-0.0.2/pyroporn/database/othDatabase.py
--rw-r--r--   0 runner    (1001) docker     (123)     1612 2023-05-05 09:02:52.000000 pyroporn-0.0.2/pyroporn/database/papDatabase.py
--rw-r--r--   0 runner    (1001) docker     (123)     2838 2023-05-05 09:02:52.000000 pyroporn-0.0.2/pyroporn/database/pmoDatabase.py
--rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-05-05 09:02:52.000000 pyroporn-0.0.2/pyroporn/database/pobDatabase.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 09:03:04.173327 pyroporn-0.0.2/pyroporn/decorators/
--rw-r--r--   0 runner    (1001) docker     (123)      284 2023-05-05 09:02:52.000000 pyroporn-0.0.2/pyroporn/decorators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6317 2023-05-05 09:02:52.000000 pyroporn-0.0.2/pyroporn/decorators/forcesub.py
--rw-r--r--   0 runner    (1001) docker     (123)      814 2023-05-05 09:02:52.000000 pyroporn-0.0.2/pyroporn/decorators/genbuttons.py
--rw-r--r--   0 runner    (1001) docker     (123)      503 2023-05-05 09:02:52.000000 pyroporn-0.0.2/pyroporn/decorators/getjson.py
--rw-r--r--   0 runner    (1001) docker     (123)      514 2023-05-05 09:02:52.000000 pyroporn-0.0.2/pyroporn/decorators/getlink.py
--rw-r--r--   0 runner    (1001) docker     (123)     3169 2023-05-05 09:02:52.000000 pyroporn-0.0.2/pyroporn/decorators/oncmd.py
--rw-r--r--   0 runner    (1001) docker     (123)       86 2023-05-05 09:02:52.000000 pyroporn-0.0.2/pyroporn/decorators/task.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 09:03:04.173327 pyroporn-0.0.2/pyroporn/methods/
--rw-r--r--   0 runner    (1001) docker     (123)      184 2023-05-05 09:02:52.000000 pyroporn-0.0.2/pyroporn/methods/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1383 2023-05-05 09:02:52.000000 pyroporn-0.0.2/pyroporn/methods/content.py
--rw-r--r--   0 runner    (1001) docker     (123)     8161 2023-05-05 09:02:52.000000 pyroporn-0.0.2/pyroporn/methods/getfile.py
--rw-r--r--   0 runner    (1001) docker     (123)     7325 2023-05-05 09:02:52.000000 pyroporn-0.0.2/pyroporn/methods/message.py
--rw-r--r--   0 runner    (1001) docker     (123)     9364 2023-05-05 09:02:52.000000 pyroporn-0.0.2/pyroporn/methods/thumbnail.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 09:03:04.177327 pyroporn-0.0.2/pyroporn/types/
--rw-r--r--   0 runner    (1001) docker     (123)      329 2023-05-05 09:02:52.000000 pyroporn-0.0.2/pyroporn/types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10063 2023-05-05 09:02:52.000000 pyroporn-0.0.2/pyroporn/types/inline.py
--rw-r--r--   0 runner    (1001) docker     (123)     3942 2023-05-05 09:02:52.000000 pyroporn-0.0.2/pyroporn/types/inlineBdb.py
--rw-r--r--   0 runner    (1001) docker     (123)     4279 2023-05-05 09:02:52.000000 pyroporn-0.0.2/pyroporn/types/inlineBub.py
--rw-r--r--   0 runner    (1001) docker     (123)     5881 2023-05-05 09:02:52.000000 pyroporn-0.0.2/pyroporn/types/inlinePob.py
--rw-r--r--   0 runner    (1001) docker     (123)     3668 2023-05-05 09:02:52.000000 pyroporn-0.0.2/pyroporn/types/inlineVip.py
--rw-r--r--   0 runner    (1001) docker     (123)      306 2023-05-05 09:02:52.000000 pyroporn-0.0.2/pyroporn/types/style.py
--rw-r--r--   0 runner    (1001) docker     (123)     5255 2023-05-05 09:02:52.000000 pyroporn-0.0.2/pyroporn/types/text.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 09:03:04.177327 pyroporn-0.0.2/pyroporn/utilities/
--rw-r--r--   0 runner    (1001) docker     (123)      189 2023-05-05 09:02:52.000000 pyroporn-0.0.2/pyroporn/utilities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1104 2023-05-05 09:02:52.000000 pyroporn-0.0.2/pyroporn/utilities/formater.py
--rw-r--r--   0 runner    (1001) docker     (123)      572 2023-05-05 09:02:52.000000 pyroporn-0.0.2/pyroporn/utilities/logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     1811 2023-05-05 09:02:52.000000 pyroporn-0.0.2/pyroporn/utilities/mongo.py
--rw-r--r--   0 runner    (1001) docker     (123)     1372 2023-05-05 09:02:52.000000 pyroporn-0.0.2/pyroporn/utilities/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-05-05 09:02:52.000000 pyroporn-0.0.2/pyroporn/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 09:03:04.173327 pyroporn-0.0.2/pyroporn.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      949 2023-05-05 09:03:04.000000 pyroporn-0.0.2/pyroporn.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1202 2023-05-05 09:03:04.000000 pyroporn-0.0.2/pyroporn.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 09:03:04.000000 pyroporn-0.0.2/pyroporn.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      202 2023-05-05 09:03:04.000000 pyroporn-0.0.2/pyroporn.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-05 09:03:04.000000 pyroporn-0.0.2/pyroporn.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-05 09:03:04.177327 pyroporn-0.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1618 2023-05-05 09:02:52.000000 pyroporn-0.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 09:14:49.700020 pyroporn-0.0.3/
+-rw-r--r--   0 runner    (1001) docker     (123)      949 2023-05-05 09:14:49.700020 pyroporn-0.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-05-05 09:14:34.000000 pyroporn-0.0.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 09:14:49.692019 pyroporn-0.0.3/pyroporn/
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-05-05 09:14:34.000000 pyroporn-0.0.3/pyroporn/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20698 2023-05-05 09:14:34.000000 pyroporn-0.0.3/pyroporn/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6623 2023-05-05 09:14:34.000000 pyroporn-0.0.3/pyroporn/config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 09:14:49.692019 pyroporn-0.0.3/pyroporn/database/
+-rw-r--r--   0 runner    (1001) docker     (123)      355 2023-05-05 09:14:34.000000 pyroporn-0.0.3/pyroporn/database/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5622 2023-05-05 09:14:34.000000 pyroporn-0.0.3/pyroporn/database/bdbDatabase.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1220 2023-05-05 09:14:34.000000 pyroporn-0.0.3/pyroporn/database/bubDatabase.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5839 2023-05-05 09:14:34.000000 pyroporn-0.0.3/pyroporn/database/othDatabase.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1612 2023-05-05 09:14:34.000000 pyroporn-0.0.3/pyroporn/database/papDatabase.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2838 2023-05-05 09:14:34.000000 pyroporn-0.0.3/pyroporn/database/pmoDatabase.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-05-05 09:14:34.000000 pyroporn-0.0.3/pyroporn/database/pobDatabase.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 09:14:49.696020 pyroporn-0.0.3/pyroporn/decorators/
+-rw-r--r--   0 runner    (1001) docker     (123)      284 2023-05-05 09:14:34.000000 pyroporn-0.0.3/pyroporn/decorators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6317 2023-05-05 09:14:34.000000 pyroporn-0.0.3/pyroporn/decorators/forcesub.py
+-rw-r--r--   0 runner    (1001) docker     (123)      814 2023-05-05 09:14:34.000000 pyroporn-0.0.3/pyroporn/decorators/genbuttons.py
+-rw-r--r--   0 runner    (1001) docker     (123)      503 2023-05-05 09:14:34.000000 pyroporn-0.0.3/pyroporn/decorators/getjson.py
+-rw-r--r--   0 runner    (1001) docker     (123)      514 2023-05-05 09:14:34.000000 pyroporn-0.0.3/pyroporn/decorators/getlink.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3169 2023-05-05 09:14:34.000000 pyroporn-0.0.3/pyroporn/decorators/oncmd.py
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-05-05 09:14:34.000000 pyroporn-0.0.3/pyroporn/decorators/task.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 09:14:49.696020 pyroporn-0.0.3/pyroporn/methods/
+-rw-r--r--   0 runner    (1001) docker     (123)      184 2023-05-05 09:14:34.000000 pyroporn-0.0.3/pyroporn/methods/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1383 2023-05-05 09:14:34.000000 pyroporn-0.0.3/pyroporn/methods/content.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8161 2023-05-05 09:14:34.000000 pyroporn-0.0.3/pyroporn/methods/getfile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7325 2023-05-05 09:14:34.000000 pyroporn-0.0.3/pyroporn/methods/message.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9364 2023-05-05 09:14:34.000000 pyroporn-0.0.3/pyroporn/methods/thumbnail.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 09:14:49.696020 pyroporn-0.0.3/pyroporn/types/
+-rw-r--r--   0 runner    (1001) docker     (123)      329 2023-05-05 09:14:34.000000 pyroporn-0.0.3/pyroporn/types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10063 2023-05-05 09:14:34.000000 pyroporn-0.0.3/pyroporn/types/inline.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3942 2023-05-05 09:14:34.000000 pyroporn-0.0.3/pyroporn/types/inlineBdb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4279 2023-05-05 09:14:34.000000 pyroporn-0.0.3/pyroporn/types/inlineBub.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5881 2023-05-05 09:14:34.000000 pyroporn-0.0.3/pyroporn/types/inlinePob.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3668 2023-05-05 09:14:34.000000 pyroporn-0.0.3/pyroporn/types/inlineVip.py
+-rw-r--r--   0 runner    (1001) docker     (123)      306 2023-05-05 09:14:34.000000 pyroporn-0.0.3/pyroporn/types/style.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5255 2023-05-05 09:14:34.000000 pyroporn-0.0.3/pyroporn/types/text.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 09:14:49.700020 pyroporn-0.0.3/pyroporn/utilities/
+-rw-r--r--   0 runner    (1001) docker     (123)      189 2023-05-05 09:14:34.000000 pyroporn-0.0.3/pyroporn/utilities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1104 2023-05-05 09:14:34.000000 pyroporn-0.0.3/pyroporn/utilities/formater.py
+-rw-r--r--   0 runner    (1001) docker     (123)      572 2023-05-05 09:14:34.000000 pyroporn-0.0.3/pyroporn/utilities/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1811 2023-05-05 09:14:34.000000 pyroporn-0.0.3/pyroporn/utilities/mongo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1372 2023-05-05 09:14:34.000000 pyroporn-0.0.3/pyroporn/utilities/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-05-05 09:14:34.000000 pyroporn-0.0.3/pyroporn/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 09:14:49.692019 pyroporn-0.0.3/pyroporn.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      949 2023-05-05 09:14:49.000000 pyroporn-0.0.3/pyroporn.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1202 2023-05-05 09:14:49.000000 pyroporn-0.0.3/pyroporn.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 09:14:49.000000 pyroporn-0.0.3/pyroporn.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      202 2023-05-05 09:14:49.000000 pyroporn-0.0.3/pyroporn.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-05 09:14:49.000000 pyroporn-0.0.3/pyroporn.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-05 09:14:49.700020 pyroporn-0.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1618 2023-05-05 09:14:34.000000 pyroporn-0.0.3/setup.py
```

### Comparing `pyroporn-0.0.2/PKG-INFO` & `pyroporn-0.0.3/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyroporn
-Version: 0.0.2
+Version: 0.0.3
 Summary: Best Porn Code for the Pyrogram Library.
 Home-page: https://github.com/OTHFamily/pyroporn
 Author: TPro
 Author-email: 
 License: MIT
 Keywords: telegram pyrogram porn bot userbot
 Classifier: Programming Language :: Python
```

### Comparing `pyroporn-0.0.2/pyroporn/client.py` & `pyroporn-0.0.3/pyroporn/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -23,15 +23,15 @@
     Methods, 
     Types,
     Utilities,
 ):
     pass
 
 
-class Client(RawClient, _AbstractCli):
+class RawClient(RawClient, _AbstractCli):
     def __init__(
         self,
         **kwargs,
     ):
         super().__init__(**kwargs)
         
         
@@ -60,15 +60,15 @@
         except Exception as e:
             self.logs.warning(e)
             self.logs.warning(f"Pastikan bot adalah Admin di OTH Content DB")
             sys.exit()
             
         if string:
             for session in string:
-                bot_ = Client(
+                bot_ = RawClient(
                     "NewUserbot",
                     api_id=self.API_ID,
                     api_hash=self.API_HASH,
                     device_model="@OnTheHerd",
                     session_string=session,
                     plugins={"root": "Tele.userbot"},
                 )
@@ -95,15 +95,15 @@
         self.BLCHAT.append(self.id)
         self.logs.info(f"OTH Started !\nName: {self.name}\nUserID: {self.id}")     
     
     async def stop(self, *args):
         await super().stop()
         
         
-    class VipCli(Client, Utils):
+    class VipCli(RawClient, Utils):
         def __init__(self):
             super().__init__(
                 "VipNewUbot",
                 api_id=self.API_ID,
                 api_hash=self.API_HASH,
                 session_string=self.SESSION,
             )
@@ -140,15 +140,15 @@
       
             self.logs.info(f"Ubot Vip Started !\nName: {self.name}\nUserID: {self.id}")
       
         async def stop(self, *args):
             await super().stop()
             
             
-    class InxCli(Client, Utils):
+    class InxCli(RawClient, Utils):
         def __init__(self):
             super().__init__(
                 "InxNewBot",
                 api_id=self.API_ID,
                 api_hash=self.API_HASH,
                 bot_token=self.BOT_TOKEN2,
             )
@@ -170,15 +170,15 @@
             self.BLCHAT.append(self.id)
             self.logs.info(f"Index Started !\nName: {self.name}\nUserID: {self.id}")
       
         async def stop(self, *args):
             await super().stop()
             
             
-    class PobCli(Client, Utils):
+    class PobCli(RawClient, Utils):
         def __init__(self):
             super().__init__(
                 "PobNewBot",
                 api_id=self.API_ID,
                 api_hash=self.API_HASH,
                 bot_token=self.BOT_TOKEN3,
             )
@@ -200,15 +200,15 @@
             self.BLCHAT.append(self.id)
             self.logs.info(f"POB Started !\nName: {self.name}\nUserID: {self.id}")
       
         async def stop(self, *args):
             await super().stop()
       
       
-    class PapCli(Client, Utils):
+    class PapCli(RawClient, Utils):
         def __init__(self):
             super().__init__(
                 "PapNewBot",
                 api_id=self.API_ID,
                 api_hash=self.API_HASH,
                 bot_token=self.BOT_TOKEN4,
             )
@@ -229,15 +229,15 @@
             self.BLCHAT.append(self.id)
             self.logs.info(f"PAP Started !\nName: {self.name}\nUserID: {self.id}")
             
         async def stop(self, *args):
             await super().stop()
             
             
-    class BclCli(Client, Utils):
+    class BclCli(RawClient, Utils):
         def __init__(self):
             super().__init__(
                 "BclNewBot",
                 api_id=self.API_ID,
                 api_hash=self.API_HASH,
                 bot_token=self.BOT_TOKEN5,
             )
@@ -258,15 +258,15 @@
             self.BLCHAT.append(self.id)
             self.logs.info(f"BCL Started !\nName: {self.name}\nUserID: {self.id}")
           
         async def stop(self, *args):
             await super().stop()
             
             
-    class BdbCli(Client, Utils):
+    class BdbCli(RawClient, Utils):
         def __init__(self):
             super().__init__(
                 "BdbNewBot",
                 api_id=self.API_ID,
                 api_hash=self.API_HASH,
                 bot_token=self.BOT_TOKEN6,
             )
@@ -287,15 +287,15 @@
                     name = prems["name"] 
                     joined = prems["joined"]
                     session = prems["string"]
                     userid = prems["userid"] 
                     status = prems["status"] 
                     expires = prems["expires"] 
                     if session != "":
-                        bot_ = Client(
+                        bot_ = RawClient(
                             "BDBNewUbot",
                             api_id=self.API_ID,
                             api_hash=self.API_HASH,
                             device_model="YourBDB",
                             session_string=session,
                             plugins={"root": "Tele.plugins.bdb"},
                         )
@@ -365,15 +365,15 @@
                         mebot = await bot_.get_me()
                         self.logs.info(f"BDB Userbot Started !\nName: {mebot.first_name}\nUserID: {mebot.id}")
                     
         async def stop(self, *args):
             await super().stop()
 
 
-    class PmoCli(Client, Utils):
+    class PmoCli(RawClient, Utils):
         def __init__(self):
             super().__init__(
                 "PmoNewBot",
                 api_id=self.API_ID,
                 api_hash=self.API_HASH,
                 bot_token=self.BOT_TOKEN7,
             )
@@ -395,15 +395,15 @@
             self.BLCHAT.append(self.id)
             self.logs.info(f"PMO Started !\nName: {self.name}\nUserID: {self.id}")
             
         async def stop(self, *args):
             await super().stop()
 
 
-    class VipBotCli(Client, Utils):
+    class VipBotCli(RawClient, Utils):
         def __init__(self):
             super().__init__(
                 "VipNewBot",
                 api_id=self.API_ID,
                 api_hash=self.API_HASH,
                 bot_token=self.BOT_TOKEN8,
             )
@@ -430,15 +430,15 @@
       
             self.logs.info(f"Bot Vip Started !\nName: {self.name}\nUserID: {self.id}")
       
         async def stop(self, *args):
             await super().stop()
 
 
-    class BubCli(Client, Utils):
+    class BubCli(RawClient, Utils):
         def __init__(self):
             super().__init__(
                 "BubNewBot",
                 api_id=self.API_ID,
                 api_hash=self.API_HASH,
                 bot_token=self.BOT_TOKEN9,
             )
@@ -459,15 +459,15 @@
                     name = u["name"] 
                     userid = u["userid"]
                     string = u["string"]
                     status = u["string"]
                     joined = u["joined"] 
                     expires = u["expires"] 
                     if string != "":
-                        bot_ = Client(
+                        bot_ = RawClient(
                             "BUBNewUbot",
                             api_id=self.API_ID,
                             api_hash=self.API_HASH,
                             device_model="BokepUBot",
                             session_string=string,
                             plugins={"root": "Tele.plugins.bub"},
                         )
```

### Comparing `pyroporn-0.0.2/pyroporn/config.py` & `pyroporn-0.0.3/pyroporn/config.py`

 * *Files identical despite different names*

### Comparing `pyroporn-0.0.2/pyroporn/database/bdbDatabase.py` & `pyroporn-0.0.3/pyroporn/database/bdbDatabase.py`

 * *Files identical despite different names*

### Comparing `pyroporn-0.0.2/pyroporn/database/bubDatabase.py` & `pyroporn-0.0.3/pyroporn/database/bubDatabase.py`

 * *Files identical despite different names*

### Comparing `pyroporn-0.0.2/pyroporn/database/othDatabase.py` & `pyroporn-0.0.3/pyroporn/database/othDatabase.py`

 * *Files identical despite different names*

### Comparing `pyroporn-0.0.2/pyroporn/database/papDatabase.py` & `pyroporn-0.0.3/pyroporn/database/papDatabase.py`

 * *Files identical despite different names*

### Comparing `pyroporn-0.0.2/pyroporn/database/pmoDatabase.py` & `pyroporn-0.0.3/pyroporn/database/pmoDatabase.py`

 * *Files identical despite different names*

### Comparing `pyroporn-0.0.2/pyroporn/database/pobDatabase.py` & `pyroporn-0.0.3/pyroporn/database/pobDatabase.py`

 * *Files identical despite different names*

### Comparing `pyroporn-0.0.2/pyroporn/decorators/forcesub.py` & `pyroporn-0.0.3/pyroporn/decorators/forcesub.py`

 * *Files identical despite different names*

### Comparing `pyroporn-0.0.2/pyroporn/decorators/genbuttons.py` & `pyroporn-0.0.3/pyroporn/decorators/genbuttons.py`

 * *Files identical despite different names*

### Comparing `pyroporn-0.0.2/pyroporn/decorators/getlink.py` & `pyroporn-0.0.3/pyroporn/decorators/getlink.py`

 * *Files identical despite different names*

### Comparing `pyroporn-0.0.2/pyroporn/decorators/oncmd.py` & `pyroporn-0.0.3/pyroporn/decorators/oncmd.py`

 * *Files identical despite different names*

### Comparing `pyroporn-0.0.2/pyroporn/methods/content.py` & `pyroporn-0.0.3/pyroporn/methods/content.py`

 * *Files identical despite different names*

### Comparing `pyroporn-0.0.2/pyroporn/methods/getfile.py` & `pyroporn-0.0.3/pyroporn/methods/getfile.py`

 * *Files identical despite different names*

### Comparing `pyroporn-0.0.2/pyroporn/methods/message.py` & `pyroporn-0.0.3/pyroporn/methods/message.py`

 * *Files identical despite different names*

### Comparing `pyroporn-0.0.2/pyroporn/methods/thumbnail.py` & `pyroporn-0.0.3/pyroporn/methods/thumbnail.py`

 * *Files identical despite different names*

### Comparing `pyroporn-0.0.2/pyroporn/types/inline.py` & `pyroporn-0.0.3/pyroporn/types/inline.py`

 * *Files identical despite different names*

### Comparing `pyroporn-0.0.2/pyroporn/types/inlineBdb.py` & `pyroporn-0.0.3/pyroporn/types/inlineBdb.py`

 * *Files identical despite different names*

### Comparing `pyroporn-0.0.2/pyroporn/types/inlineBub.py` & `pyroporn-0.0.3/pyroporn/types/inlineBub.py`

 * *Files identical despite different names*

### Comparing `pyroporn-0.0.2/pyroporn/types/inlinePob.py` & `pyroporn-0.0.3/pyroporn/types/inlinePob.py`

 * *Files identical despite different names*

### Comparing `pyroporn-0.0.2/pyroporn/types/inlineVip.py` & `pyroporn-0.0.3/pyroporn/types/inlineVip.py`

 * *Files identical despite different names*

### Comparing `pyroporn-0.0.2/pyroporn/types/text.py` & `pyroporn-0.0.3/pyroporn/types/text.py`

 * *Files identical despite different names*

### Comparing `pyroporn-0.0.2/pyroporn/utilities/formater.py` & `pyroporn-0.0.3/pyroporn/utilities/formater.py`

 * *Files identical despite different names*

### Comparing `pyroporn-0.0.2/pyroporn/utilities/logger.py` & `pyroporn-0.0.3/pyroporn/utilities/logger.py`

 * *Files identical despite different names*

### Comparing `pyroporn-0.0.2/pyroporn/utilities/mongo.py` & `pyroporn-0.0.3/pyroporn/utilities/mongo.py`

 * *Files identical despite different names*

### Comparing `pyroporn-0.0.2/pyroporn/utilities/utils.py` & `pyroporn-0.0.3/pyroporn/utilities/utils.py`

 * *Files identical despite different names*

### Comparing `pyroporn-0.0.2/pyroporn.egg-info/PKG-INFO` & `pyroporn-0.0.3/pyroporn.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyroporn
-Version: 0.0.2
+Version: 0.0.3
 Summary: Best Porn Code for the Pyrogram Library.
 Home-page: https://github.com/OTHFamily/pyroporn
 Author: TPro
 Author-email: 
 License: MIT
 Keywords: telegram pyrogram porn bot userbot
 Classifier: Programming Language :: Python
```

### Comparing `pyroporn-0.0.2/pyroporn.egg-info/SOURCES.txt` & `pyroporn-0.0.3/pyroporn.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyroporn-0.0.2/setup.py` & `pyroporn-0.0.3/setup.py`

 * *Files identical despite different names*

