# Comparing `tmp/pyTPro-0.0.0.tar.gz` & `tmp/pyTPro-0.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyTPro-0.0.0.tar", last modified: Thu May  4 19:50:35 2023, max compression
+gzip compressed data, was "pyTPro-0.0.1.tar", last modified: Fri May  5 07:06:05 2023, max compression
```

## Comparing `pyTPro-0.0.0.tar` & `pyTPro-0.0.1.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 19:50:35.502832 pyTPro-0.0.0/
--rw-r--r--   0 runner    (1001) docker     (123)      932 2023-05-04 19:50:35.502832 pyTPro-0.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-05-04 19:50:22.000000 pyTPro-0.0.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 19:50:35.498831 pyTPro-0.0.0/Tele/
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-05-04 19:50:22.000000 pyTPro-0.0.0/Tele/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    20624 2023-05-04 19:50:22.000000 pyTPro-0.0.0/Tele/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     6623 2023-05-04 19:50:22.000000 pyTPro-0.0.0/Tele/config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 19:50:35.498831 pyTPro-0.0.0/Tele/database/
--rw-r--r--   0 runner    (1001) docker     (123)      355 2023-05-04 19:50:22.000000 pyTPro-0.0.0/Tele/database/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5622 2023-05-04 19:50:22.000000 pyTPro-0.0.0/Tele/database/bdbDatabase.py
--rw-r--r--   0 runner    (1001) docker     (123)     1220 2023-05-04 19:50:22.000000 pyTPro-0.0.0/Tele/database/bubDatabase.py
--rw-r--r--   0 runner    (1001) docker     (123)     5839 2023-05-04 19:50:22.000000 pyTPro-0.0.0/Tele/database/othDatabase.py
--rw-r--r--   0 runner    (1001) docker     (123)     1612 2023-05-04 19:50:22.000000 pyTPro-0.0.0/Tele/database/papDatabase.py
--rw-r--r--   0 runner    (1001) docker     (123)     2838 2023-05-04 19:50:22.000000 pyTPro-0.0.0/Tele/database/pmoDatabase.py
--rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-05-04 19:50:22.000000 pyTPro-0.0.0/Tele/database/pobDatabase.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 19:50:35.498831 pyTPro-0.0.0/Tele/decorators/
--rw-r--r--   0 runner    (1001) docker     (123)      144 2023-05-04 19:50:22.000000 pyTPro-0.0.0/Tele/decorators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6317 2023-05-04 19:50:22.000000 pyTPro-0.0.0/Tele/decorators/forcesub.py
--rw-r--r--   0 runner    (1001) docker     (123)     3169 2023-05-04 19:50:22.000000 pyTPro-0.0.0/Tele/decorators/oncmd.py
--rw-r--r--   0 runner    (1001) docker     (123)     1891 2023-05-04 19:50:22.000000 pyTPro-0.0.0/Tele/decorators/task.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 19:50:35.498831 pyTPro-0.0.0/Tele/methods/
--rw-r--r--   0 runner    (1001) docker     (123)      200 2023-05-04 19:50:22.000000 pyTPro-0.0.0/Tele/methods/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1383 2023-05-04 19:50:22.000000 pyTPro-0.0.0/Tele/methods/content.py
--rw-r--r--   0 runner    (1001) docker     (123)     8161 2023-05-04 19:50:22.000000 pyTPro-0.0.0/Tele/methods/getfile.py
--rw-r--r--   0 runner    (1001) docker     (123)     8433 2023-05-04 19:50:22.000000 pyTPro-0.0.0/Tele/methods/message.py
--rw-r--r--   0 runner    (1001) docker     (123)     9364 2023-05-04 19:50:22.000000 pyTPro-0.0.0/Tele/methods/thumbnail.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 19:50:35.502832 pyTPro-0.0.0/Tele/types/
--rw-r--r--   0 runner    (1001) docker     (123)      326 2023-05-04 19:50:22.000000 pyTPro-0.0.0/Tele/types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10063 2023-05-04 19:50:22.000000 pyTPro-0.0.0/Tele/types/inline.py
--rw-r--r--   0 runner    (1001) docker     (123)     3942 2023-05-04 19:50:22.000000 pyTPro-0.0.0/Tele/types/inlineBdb.py
--rw-r--r--   0 runner    (1001) docker     (123)     4279 2023-05-04 19:50:22.000000 pyTPro-0.0.0/Tele/types/inlineBub.py
--rw-r--r--   0 runner    (1001) docker     (123)     5881 2023-05-04 19:50:22.000000 pyTPro-0.0.0/Tele/types/inlinePob.py
--rw-r--r--   0 runner    (1001) docker     (123)     3668 2023-05-04 19:50:22.000000 pyTPro-0.0.0/Tele/types/inlineVip.py
--rw-r--r--   0 runner    (1001) docker     (123)      306 2023-05-04 19:50:22.000000 pyTPro-0.0.0/Tele/types/style.py
--rw-r--r--   0 runner    (1001) docker     (123)     5255 2023-05-04 19:50:22.000000 pyTPro-0.0.0/Tele/types/text.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 19:50:35.502832 pyTPro-0.0.0/Tele/utilities/
--rw-r--r--   0 runner    (1001) docker     (123)      124 2023-05-04 19:50:22.000000 pyTPro-0.0.0/Tele/utilities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      568 2023-05-04 19:50:22.000000 pyTPro-0.0.0/Tele/utilities/logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     1807 2023-05-04 19:50:22.000000 pyTPro-0.0.0/Tele/utilities/mongo.py
--rw-r--r--   0 runner    (1001) docker     (123)     1368 2023-05-04 19:50:22.000000 pyTPro-0.0.0/Tele/utilities/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 19:50:35.502832 pyTPro-0.0.0/pyTPro.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      932 2023-05-04 19:50:35.000000 pyTPro-0.0.0/pyTPro.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      921 2023-05-04 19:50:35.000000 pyTPro-0.0.0/pyTPro.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-04 19:50:35.000000 pyTPro-0.0.0/pyTPro.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      202 2023-05-04 19:50:35.000000 pyTPro-0.0.0/pyTPro.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-05-04 19:50:35.000000 pyTPro-0.0.0/pyTPro.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-04 19:50:35.502832 pyTPro-0.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1611 2023-05-04 19:50:22.000000 pyTPro-0.0.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 07:06:05.586779 pyTPro-0.0.1/
+-rw-r--r--   0 runner    (1001) docker     (123)      932 2023-05-05 07:06:05.586779 pyTPro-0.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-05-05 07:05:53.000000 pyTPro-0.0.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 07:06:05.578780 pyTPro-0.0.1/Tele/
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-05-05 07:05:53.000000 pyTPro-0.0.1/Tele/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20623 2023-05-05 07:05:53.000000 pyTPro-0.0.1/Tele/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6623 2023-05-05 07:05:53.000000 pyTPro-0.0.1/Tele/config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 07:06:05.578780 pyTPro-0.0.1/Tele/database/
+-rw-r--r--   0 runner    (1001) docker     (123)      355 2023-05-05 07:05:53.000000 pyTPro-0.0.1/Tele/database/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5622 2023-05-05 07:05:53.000000 pyTPro-0.0.1/Tele/database/bdbDatabase.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1220 2023-05-05 07:05:53.000000 pyTPro-0.0.1/Tele/database/bubDatabase.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5839 2023-05-05 07:05:53.000000 pyTPro-0.0.1/Tele/database/othDatabase.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1612 2023-05-05 07:05:53.000000 pyTPro-0.0.1/Tele/database/papDatabase.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2838 2023-05-05 07:05:53.000000 pyTPro-0.0.1/Tele/database/pmoDatabase.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-05-05 07:05:53.000000 pyTPro-0.0.1/Tele/database/pobDatabase.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 07:06:05.578780 pyTPro-0.0.1/Tele/decorators/
+-rw-r--r--   0 runner    (1001) docker     (123)      144 2023-05-05 07:05:53.000000 pyTPro-0.0.1/Tele/decorators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6317 2023-05-05 07:05:53.000000 pyTPro-0.0.1/Tele/decorators/forcesub.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3169 2023-05-05 07:05:53.000000 pyTPro-0.0.1/Tele/decorators/oncmd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1891 2023-05-05 07:05:53.000000 pyTPro-0.0.1/Tele/decorators/task.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 07:06:05.582780 pyTPro-0.0.1/Tele/methods/
+-rw-r--r--   0 runner    (1001) docker     (123)      200 2023-05-05 07:05:53.000000 pyTPro-0.0.1/Tele/methods/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1383 2023-05-05 07:05:53.000000 pyTPro-0.0.1/Tele/methods/content.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8161 2023-05-05 07:05:53.000000 pyTPro-0.0.1/Tele/methods/getfile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8433 2023-05-05 07:05:53.000000 pyTPro-0.0.1/Tele/methods/message.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9364 2023-05-05 07:05:53.000000 pyTPro-0.0.1/Tele/methods/thumbnail.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 07:06:05.582780 pyTPro-0.0.1/Tele/types/
+-rw-r--r--   0 runner    (1001) docker     (123)      326 2023-05-05 07:05:53.000000 pyTPro-0.0.1/Tele/types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10063 2023-05-05 07:05:53.000000 pyTPro-0.0.1/Tele/types/inline.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3942 2023-05-05 07:05:53.000000 pyTPro-0.0.1/Tele/types/inlineBdb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4279 2023-05-05 07:05:53.000000 pyTPro-0.0.1/Tele/types/inlineBub.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5881 2023-05-05 07:05:53.000000 pyTPro-0.0.1/Tele/types/inlinePob.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3668 2023-05-05 07:05:53.000000 pyTPro-0.0.1/Tele/types/inlineVip.py
+-rw-r--r--   0 runner    (1001) docker     (123)      306 2023-05-05 07:05:53.000000 pyTPro-0.0.1/Tele/types/style.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5255 2023-05-05 07:05:53.000000 pyTPro-0.0.1/Tele/types/text.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 07:06:05.582780 pyTPro-0.0.1/Tele/utilities/
+-rw-r--r--   0 runner    (1001) docker     (123)      124 2023-05-05 07:05:53.000000 pyTPro-0.0.1/Tele/utilities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      568 2023-05-05 07:05:53.000000 pyTPro-0.0.1/Tele/utilities/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1807 2023-05-05 07:05:53.000000 pyTPro-0.0.1/Tele/utilities/mongo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1368 2023-05-05 07:05:53.000000 pyTPro-0.0.1/Tele/utilities/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 07:06:05.586779 pyTPro-0.0.1/pyTPro.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      932 2023-05-05 07:06:05.000000 pyTPro-0.0.1/pyTPro.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      921 2023-05-05 07:06:05.000000 pyTPro-0.0.1/pyTPro.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 07:06:05.000000 pyTPro-0.0.1/pyTPro.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      202 2023-05-05 07:06:05.000000 pyTPro-0.0.1/pyTPro.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-05-05 07:06:05.000000 pyTPro-0.0.1/pyTPro.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-05 07:06:05.586779 pyTPro-0.0.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1611 2023-05-05 07:05:53.000000 pyTPro-0.0.1/setup.py
```

### Comparing `pyTPro-0.0.0/PKG-INFO` & `pyTPro-0.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyTPro
-Version: 0.0.0
+Version: 0.0.1
 Summary: Best Code for the Pyrogram Library.
 Home-page: https://github.com/OTHFamily/pyTele
 Author: TPro
 Author-email: 
 License: MIT
 Keywords: telegram pyrogram keyboard bot userbot
 Classifier: Programming Language :: Python
```

### Comparing `pyTPro-0.0.0/Tele/client.py` & `pyTPro-0.0.1/Tele/client.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,41 +1,40 @@
 import sys
 import pyromod.listen
 
-from pyrogram import Client
+from pyrogram import Client as RawClient
 from pyrogram.errors import (
     AuthKeyDuplicated,
     AuthKeyUnregistered,
     SessionRevoked,
     UserDeactivated,
     UserDeactivatedBan,
     SessionPasswordNeeded,
 )
 from .database import Database
 from .decorators import Decorators
 from .methods import Methods
 from .types import Types
-from .utilities import Utilities 
+from .utilities import Utilities
 
 
 class _Abc(
     Database, Decorators, Methods, Types, Utilities
 ):
     pass
 
 
-class AppCli(Client, _Abc):
-    def __init__(self):
-        super().__init__(
-            "OTHNewBot",
-            api_id=self.API_ID,
-            api_hash=self.API_HASH,
-            bot_token=self.BOT_TOKEN,
-        )
-    
+class Client(RawClient, _Abc):
+    def __init__(
+        self,
+        **kwargs,
+    ):
+        super().__init__(**kwargs)
+        
+        
     async def start(self):
         await super().start()
         await self.Media.ensure_indexes()
         await self.Media2.ensure_indexes()
         string = await self.get_session()
         me = await self.get_me()
         self.id = me.id
@@ -85,23 +84,22 @@
                     await self.del_session(session)
                 self.rawbot.append(bot_)
                 try:
                     mebot = await bot_.get_me()
                     self.logs.info(f"Userbot Started !\nName: {mebot.first_name}\nUserID: {mebot.id}")
                 except BaseException:
                     pass
-
         self.BLCHAT.append(self.id)
         self.logs.info(f"OTH Started !\nName: {self.name}\nUserID: {self.id}")     
     
     async def stop(self, *args):
         await super().stop()
         
-    
-    class VipCli(Client, _Abc):
+        
+    class VipCli(Client, Utils):
         def __init__(self):
             super().__init__(
                 "VipNewUbot",
                 api_id=self.API_ID,
                 api_hash=self.API_HASH,
                 session_string=self.SESSION,
             )
@@ -136,17 +134,17 @@
                 self.logs.warning(e)
                 sys.exit()
       
             self.logs.info(f"Ubot Vip Started !\nName: {self.name}\nUserID: {self.id}")
       
         async def stop(self, *args):
             await super().stop()
-      
-      
-    class InxCli(Client, _Abc):
+            
+            
+    class InxCli(Client, Utils):
         def __init__(self):
             super().__init__(
                 "InxNewBot",
                 api_id=self.API_ID,
                 api_hash=self.API_HASH,
                 bot_token=self.BOT_TOKEN2,
             )
@@ -166,17 +164,17 @@
                 sys.exit()
             
             self.BLCHAT.append(self.id)
             self.logs.info(f"Index Started !\nName: {self.name}\nUserID: {self.id}")
       
         async def stop(self, *args):
             await super().stop()
-
-
-    class PobCli(Client, _Abc):
+            
+            
+    class PobCli(Client, Utils):
         def __init__(self):
             super().__init__(
                 "PobNewBot",
                 api_id=self.API_ID,
                 api_hash=self.API_HASH,
                 bot_token=self.BOT_TOKEN3,
             )
@@ -198,15 +196,15 @@
             self.BLCHAT.append(self.id)
             self.logs.info(f"POB Started !\nName: {self.name}\nUserID: {self.id}")
       
         async def stop(self, *args):
             await super().stop()
       
       
-    class PapCli(Client, _Abc):
+    class PapCli(Client, Utils):
         def __init__(self):
             super().__init__(
                 "PapNewBot",
                 api_id=self.API_ID,
                 api_hash=self.API_HASH,
                 bot_token=self.BOT_TOKEN4,
             )
@@ -220,23 +218,22 @@
       
             try:
                 self.channel_db = await self.get_chat(self.PAP_INDEX)
             except Exception as e:
                 self.logs.warning(e)
                 self.logs.warning(f"Pastikan bot adalah Admin di Channel DB Rate")
                 sys.exit()
-
             self.BLCHAT.append(self.id)
             self.logs.info(f"PAP Started !\nName: {self.name}\nUserID: {self.id}")
             
         async def stop(self, *args):
             await super().stop()
-      
-      
-    class BclCli(Client, _Abc):
+            
+            
+    class BclCli(Client, Utils):
         def __init__(self):
             super().__init__(
                 "BclNewBot",
                 api_id=self.API_ID,
                 api_hash=self.API_HASH,
                 bot_token=self.BOT_TOKEN5,
             )
@@ -250,23 +247,22 @@
       
             try:
                 self.channel_db = await self.get_chat(self.BCL_INDEX)
             except Exception as e:
                 self.logs.warning(e)
                 self.logs.warning(f"Pastikan bot adalah Admin di Channel DB Bocil")
                 sys.exit()
-
             self.BLCHAT.append(self.id)
             self.logs.info(f"BCL Started !\nName: {self.name}\nUserID: {self.id}")
           
         async def stop(self, *args):
             await super().stop()
-      
-      
-    class BdbCli(Client, _Abc):
+            
+            
+    class BdbCli(Client, Utils):
         def __init__(self):
             super().__init__(
                 "BdbNewBot",
                 api_id=self.API_ID,
                 api_hash=self.API_HASH,
                 bot_token=self.BOT_TOKEN6,
             )
@@ -365,15 +361,15 @@
                         mebot = await bot_.get_me()
                         self.logs.info(f"BDB Userbot Started !\nName: {mebot.first_name}\nUserID: {mebot.id}")
                     
         async def stop(self, *args):
             await super().stop()
 
 
-    class PmoCli(Client, _Abc):
+    class PmoCli(Client, Utils):
         def __init__(self):
             super().__init__(
                 "PmoNewBot",
                 api_id=self.API_ID,
                 api_hash=self.API_HASH,
                 bot_token=self.BOT_TOKEN7,
             )
@@ -395,15 +391,15 @@
             self.BLCHAT.append(self.id)
             self.logs.info(f"PMO Started !\nName: {self.name}\nUserID: {self.id}")
             
         async def stop(self, *args):
             await super().stop()
 
 
-    class VipBotCli(Client, _Abc):
+    class VipBotCli(Client, Utils):
         def __init__(self):
             super().__init__(
                 "VipNewBot",
                 api_id=self.API_ID,
                 api_hash=self.API_HASH,
                 bot_token=self.BOT_TOKEN8,
             )
@@ -430,15 +426,15 @@
       
             self.logs.info(f"Bot Vip Started !\nName: {self.name}\nUserID: {self.id}")
       
         async def stop(self, *args):
             await super().stop()
 
 
-    class BubCli(Client, _Abc):
+    class BubCli(Client, Utils):
         def __init__(self):
             super().__init__(
                 "BubNewBot",
                 api_id=self.API_ID,
                 api_hash=self.API_HASH,
                 bot_token=self.BOT_TOKEN9,
             )
```

### Comparing `pyTPro-0.0.0/Tele/config.py` & `pyTPro-0.0.1/Tele/config.py`

 * *Files identical despite different names*

### Comparing `pyTPro-0.0.0/Tele/database/bdbDatabase.py` & `pyTPro-0.0.1/Tele/database/bdbDatabase.py`

 * *Files identical despite different names*

### Comparing `pyTPro-0.0.0/Tele/database/bubDatabase.py` & `pyTPro-0.0.1/Tele/database/bubDatabase.py`

 * *Files identical despite different names*

### Comparing `pyTPro-0.0.0/Tele/database/othDatabase.py` & `pyTPro-0.0.1/Tele/database/othDatabase.py`

 * *Files identical despite different names*

### Comparing `pyTPro-0.0.0/Tele/database/papDatabase.py` & `pyTPro-0.0.1/Tele/database/papDatabase.py`

 * *Files identical despite different names*

### Comparing `pyTPro-0.0.0/Tele/database/pmoDatabase.py` & `pyTPro-0.0.1/Tele/database/pmoDatabase.py`

 * *Files identical despite different names*

### Comparing `pyTPro-0.0.0/Tele/database/pobDatabase.py` & `pyTPro-0.0.1/Tele/database/pobDatabase.py`

 * *Files identical despite different names*

### Comparing `pyTPro-0.0.0/Tele/decorators/forcesub.py` & `pyTPro-0.0.1/Tele/decorators/forcesub.py`

 * *Files identical despite different names*

### Comparing `pyTPro-0.0.0/Tele/decorators/oncmd.py` & `pyTPro-0.0.1/Tele/decorators/oncmd.py`

 * *Files identical despite different names*

### Comparing `pyTPro-0.0.0/Tele/decorators/task.py` & `pyTPro-0.0.1/Tele/decorators/task.py`

 * *Files identical despite different names*

### Comparing `pyTPro-0.0.0/Tele/methods/content.py` & `pyTPro-0.0.1/Tele/methods/content.py`

 * *Files identical despite different names*

### Comparing `pyTPro-0.0.0/Tele/methods/getfile.py` & `pyTPro-0.0.1/Tele/methods/getfile.py`

 * *Files identical despite different names*

### Comparing `pyTPro-0.0.0/Tele/methods/message.py` & `pyTPro-0.0.1/Tele/methods/message.py`

 * *Files identical despite different names*

### Comparing `pyTPro-0.0.0/Tele/methods/thumbnail.py` & `pyTPro-0.0.1/Tele/methods/thumbnail.py`

 * *Files identical despite different names*

### Comparing `pyTPro-0.0.0/Tele/types/inline.py` & `pyTPro-0.0.1/Tele/types/inline.py`

 * *Files identical despite different names*

### Comparing `pyTPro-0.0.0/Tele/types/inlineBdb.py` & `pyTPro-0.0.1/Tele/types/inlineBdb.py`

 * *Files identical despite different names*

### Comparing `pyTPro-0.0.0/Tele/types/inlineBub.py` & `pyTPro-0.0.1/Tele/types/inlineBub.py`

 * *Files identical despite different names*

### Comparing `pyTPro-0.0.0/Tele/types/inlinePob.py` & `pyTPro-0.0.1/Tele/types/inlinePob.py`

 * *Files identical despite different names*

### Comparing `pyTPro-0.0.0/Tele/types/inlineVip.py` & `pyTPro-0.0.1/Tele/types/inlineVip.py`

 * *Files identical despite different names*

### Comparing `pyTPro-0.0.0/Tele/types/text.py` & `pyTPro-0.0.1/Tele/types/text.py`

 * *Files identical despite different names*

### Comparing `pyTPro-0.0.0/Tele/utilities/logger.py` & `pyTPro-0.0.1/Tele/utilities/logger.py`

 * *Files identical despite different names*

### Comparing `pyTPro-0.0.0/Tele/utilities/mongo.py` & `pyTPro-0.0.1/Tele/utilities/mongo.py`

 * *Files identical despite different names*

### Comparing `pyTPro-0.0.0/Tele/utilities/utils.py` & `pyTPro-0.0.1/Tele/utilities/utils.py`

 * *Files identical despite different names*

### Comparing `pyTPro-0.0.0/pyTPro.egg-info/PKG-INFO` & `pyTPro-0.0.1/pyTPro.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyTPro
-Version: 0.0.0
+Version: 0.0.1
 Summary: Best Code for the Pyrogram Library.
 Home-page: https://github.com/OTHFamily/pyTele
 Author: TPro
 Author-email: 
 License: MIT
 Keywords: telegram pyrogram keyboard bot userbot
 Classifier: Programming Language :: Python
```

### Comparing `pyTPro-0.0.0/pyTPro.egg-info/SOURCES.txt` & `pyTPro-0.0.1/pyTPro.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyTPro-0.0.0/setup.py` & `pyTPro-0.0.1/setup.py`

 * *Files identical despite different names*

