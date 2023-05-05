# Comparing `tmp/pyroporn-0.1.5.tar.gz` & `tmp/pyroporn-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyroporn-0.1.5.tar", last modified: Fri May  5 14:30:06 2023, max compression
+gzip compressed data, was "pyroporn-0.1.6.tar", last modified: Fri May  5 14:44:03 2023, max compression
```

## Comparing `pyroporn-0.1.5.tar` & `pyroporn-0.1.6.tar`

### file list

```diff
@@ -1,55 +1,55 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 14:30:06.529828 pyroporn-0.1.5/
--rw-r--r--   0 runner    (1001) docker     (123)      949 2023-05-05 14:30:06.529828 pyroporn-0.1.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-05-05 14:29:49.000000 pyroporn-0.1.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 14:30:06.525828 pyroporn-0.1.5/pyroporn/
--rw-r--r--   0 runner    (1001) docker     (123)       86 2023-05-05 14:29:49.000000 pyroporn-0.1.5/pyroporn/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    20759 2023-05-05 14:29:49.000000 pyroporn-0.1.5/pyroporn/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     6623 2023-05-05 14:29:49.000000 pyroporn-0.1.5/pyroporn/config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 14:30:06.525828 pyroporn-0.1.5/pyroporn/database/
--rw-r--r--   0 runner    (1001) docker     (123)      355 2023-05-05 14:29:49.000000 pyroporn-0.1.5/pyroporn/database/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5622 2023-05-05 14:29:49.000000 pyroporn-0.1.5/pyroporn/database/bdbDatabase.py
--rw-r--r--   0 runner    (1001) docker     (123)     1220 2023-05-05 14:29:49.000000 pyroporn-0.1.5/pyroporn/database/bubDatabase.py
--rw-r--r--   0 runner    (1001) docker     (123)     5839 2023-05-05 14:29:49.000000 pyroporn-0.1.5/pyroporn/database/othDatabase.py
--rw-r--r--   0 runner    (1001) docker     (123)     1612 2023-05-05 14:29:49.000000 pyroporn-0.1.5/pyroporn/database/papDatabase.py
--rw-r--r--   0 runner    (1001) docker     (123)     2838 2023-05-05 14:29:49.000000 pyroporn-0.1.5/pyroporn/database/pmoDatabase.py
--rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-05-05 14:29:49.000000 pyroporn-0.1.5/pyroporn/database/pobDatabase.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 14:30:06.525828 pyroporn-0.1.5/pyroporn/decorators/
--rw-r--r--   0 runner    (1001) docker     (123)      374 2023-05-05 14:29:49.000000 pyroporn-0.1.5/pyroporn/decorators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      406 2023-05-05 14:29:49.000000 pyroporn-0.1.5/pyroporn/decorators/addhandler.py
--rw-r--r--   0 runner    (1001) docker     (123)     2407 2023-05-05 14:29:49.000000 pyroporn-0.1.5/pyroporn/decorators/botcmd.py
--rw-r--r--   0 runner    (1001) docker     (123)     6317 2023-05-05 14:29:49.000000 pyroporn-0.1.5/pyroporn/decorators/forcesub.py
--rw-r--r--   0 runner    (1001) docker     (123)      814 2023-05-05 14:29:49.000000 pyroporn-0.1.5/pyroporn/decorators/genbuttons.py
--rw-r--r--   0 runner    (1001) docker     (123)      503 2023-05-05 14:29:49.000000 pyroporn-0.1.5/pyroporn/decorators/getjson.py
--rw-r--r--   0 runner    (1001) docker     (123)      514 2023-05-05 14:29:49.000000 pyroporn-0.1.5/pyroporn/decorators/getlink.py
--rw-r--r--   0 runner    (1001) docker     (123)     2456 2023-05-05 14:29:49.000000 pyroporn-0.1.5/pyroporn/decorators/oncmd.py
--rw-r--r--   0 runner    (1001) docker     (123)       86 2023-05-05 14:29:49.000000 pyroporn-0.1.5/pyroporn/decorators/task.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 14:30:06.529828 pyroporn-0.1.5/pyroporn/methods/
--rw-r--r--   0 runner    (1001) docker     (123)      184 2023-05-05 14:29:49.000000 pyroporn-0.1.5/pyroporn/methods/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1383 2023-05-05 14:29:49.000000 pyroporn-0.1.5/pyroporn/methods/content.py
--rw-r--r--   0 runner    (1001) docker     (123)     8161 2023-05-05 14:29:49.000000 pyroporn-0.1.5/pyroporn/methods/getfile.py
--rw-r--r--   0 runner    (1001) docker     (123)     7325 2023-05-05 14:29:49.000000 pyroporn-0.1.5/pyroporn/methods/message.py
--rw-r--r--   0 runner    (1001) docker     (123)     9364 2023-05-05 14:29:49.000000 pyroporn-0.1.5/pyroporn/methods/thumbnail.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 14:30:06.529828 pyroporn-0.1.5/pyroporn/types/
--rw-r--r--   0 runner    (1001) docker     (123)      329 2023-05-05 14:29:49.000000 pyroporn-0.1.5/pyroporn/types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10063 2023-05-05 14:29:49.000000 pyroporn-0.1.5/pyroporn/types/inline.py
--rw-r--r--   0 runner    (1001) docker     (123)     3942 2023-05-05 14:29:49.000000 pyroporn-0.1.5/pyroporn/types/inlineBdb.py
--rw-r--r--   0 runner    (1001) docker     (123)     4279 2023-05-05 14:29:49.000000 pyroporn-0.1.5/pyroporn/types/inlineBub.py
--rw-r--r--   0 runner    (1001) docker     (123)     5881 2023-05-05 14:29:49.000000 pyroporn-0.1.5/pyroporn/types/inlinePob.py
--rw-r--r--   0 runner    (1001) docker     (123)     3668 2023-05-05 14:29:49.000000 pyroporn-0.1.5/pyroporn/types/inlineVip.py
--rw-r--r--   0 runner    (1001) docker     (123)      306 2023-05-05 14:29:49.000000 pyroporn-0.1.5/pyroporn/types/style.py
--rw-r--r--   0 runner    (1001) docker     (123)     5255 2023-05-05 14:29:49.000000 pyroporn-0.1.5/pyroporn/types/text.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 14:30:06.529828 pyroporn-0.1.5/pyroporn/utilities/
--rw-r--r--   0 runner    (1001) docker     (123)      189 2023-05-05 14:29:49.000000 pyroporn-0.1.5/pyroporn/utilities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1104 2023-05-05 14:29:49.000000 pyroporn-0.1.5/pyroporn/utilities/formater.py
--rw-r--r--   0 runner    (1001) docker     (123)      572 2023-05-05 14:29:49.000000 pyroporn-0.1.5/pyroporn/utilities/logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     1811 2023-05-05 14:29:49.000000 pyroporn-0.1.5/pyroporn/utilities/mongo.py
--rw-r--r--   0 runner    (1001) docker     (123)     1372 2023-05-05 14:29:49.000000 pyroporn-0.1.5/pyroporn/utilities/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-05-05 14:29:49.000000 pyroporn-0.1.5/pyroporn/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 14:30:06.525828 pyroporn-0.1.5/pyroporn.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      949 2023-05-05 14:30:06.000000 pyroporn-0.1.5/pyroporn.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1266 2023-05-05 14:30:06.000000 pyroporn-0.1.5/pyroporn.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 14:30:06.000000 pyroporn-0.1.5/pyroporn.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      202 2023-05-05 14:30:06.000000 pyroporn-0.1.5/pyroporn.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-05 14:30:06.000000 pyroporn-0.1.5/pyroporn.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-05 14:30:06.529828 pyroporn-0.1.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1618 2023-05-05 14:29:49.000000 pyroporn-0.1.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 14:44:03.479500 pyroporn-0.1.6/
+-rw-r--r--   0 runner    (1001) docker     (123)      949 2023-05-05 14:44:03.479500 pyroporn-0.1.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-05-05 14:43:48.000000 pyroporn-0.1.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 14:44:03.475500 pyroporn-0.1.6/pyroporn/
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-05-05 14:43:48.000000 pyroporn-0.1.6/pyroporn/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20759 2023-05-05 14:43:48.000000 pyroporn-0.1.6/pyroporn/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6623 2023-05-05 14:43:48.000000 pyroporn-0.1.6/pyroporn/config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 14:44:03.475500 pyroporn-0.1.6/pyroporn/database/
+-rw-r--r--   0 runner    (1001) docker     (123)      355 2023-05-05 14:43:48.000000 pyroporn-0.1.6/pyroporn/database/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5622 2023-05-05 14:43:48.000000 pyroporn-0.1.6/pyroporn/database/bdbDatabase.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1220 2023-05-05 14:43:48.000000 pyroporn-0.1.6/pyroporn/database/bubDatabase.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5839 2023-05-05 14:43:48.000000 pyroporn-0.1.6/pyroporn/database/othDatabase.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1612 2023-05-05 14:43:48.000000 pyroporn-0.1.6/pyroporn/database/papDatabase.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2838 2023-05-05 14:43:48.000000 pyroporn-0.1.6/pyroporn/database/pmoDatabase.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-05-05 14:43:48.000000 pyroporn-0.1.6/pyroporn/database/pobDatabase.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 14:44:03.475500 pyroporn-0.1.6/pyroporn/decorators/
+-rw-r--r--   0 runner    (1001) docker     (123)      374 2023-05-05 14:43:48.000000 pyroporn-0.1.6/pyroporn/decorators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      407 2023-05-05 14:43:48.000000 pyroporn-0.1.6/pyroporn/decorators/addhandler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2407 2023-05-05 14:43:48.000000 pyroporn-0.1.6/pyroporn/decorators/botcmd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6317 2023-05-05 14:43:48.000000 pyroporn-0.1.6/pyroporn/decorators/forcesub.py
+-rw-r--r--   0 runner    (1001) docker     (123)      814 2023-05-05 14:43:48.000000 pyroporn-0.1.6/pyroporn/decorators/genbuttons.py
+-rw-r--r--   0 runner    (1001) docker     (123)      503 2023-05-05 14:43:48.000000 pyroporn-0.1.6/pyroporn/decorators/getjson.py
+-rw-r--r--   0 runner    (1001) docker     (123)      514 2023-05-05 14:43:48.000000 pyroporn-0.1.6/pyroporn/decorators/getlink.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2456 2023-05-05 14:43:48.000000 pyroporn-0.1.6/pyroporn/decorators/oncmd.py
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-05-05 14:43:48.000000 pyroporn-0.1.6/pyroporn/decorators/task.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 14:44:03.475500 pyroporn-0.1.6/pyroporn/methods/
+-rw-r--r--   0 runner    (1001) docker     (123)      184 2023-05-05 14:43:48.000000 pyroporn-0.1.6/pyroporn/methods/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1383 2023-05-05 14:43:48.000000 pyroporn-0.1.6/pyroporn/methods/content.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8161 2023-05-05 14:43:48.000000 pyroporn-0.1.6/pyroporn/methods/getfile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7325 2023-05-05 14:43:48.000000 pyroporn-0.1.6/pyroporn/methods/message.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9364 2023-05-05 14:43:48.000000 pyroporn-0.1.6/pyroporn/methods/thumbnail.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 14:44:03.479500 pyroporn-0.1.6/pyroporn/types/
+-rw-r--r--   0 runner    (1001) docker     (123)      329 2023-05-05 14:43:48.000000 pyroporn-0.1.6/pyroporn/types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10063 2023-05-05 14:43:48.000000 pyroporn-0.1.6/pyroporn/types/inline.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3942 2023-05-05 14:43:48.000000 pyroporn-0.1.6/pyroporn/types/inlineBdb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4279 2023-05-05 14:43:48.000000 pyroporn-0.1.6/pyroporn/types/inlineBub.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5881 2023-05-05 14:43:48.000000 pyroporn-0.1.6/pyroporn/types/inlinePob.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3668 2023-05-05 14:43:48.000000 pyroporn-0.1.6/pyroporn/types/inlineVip.py
+-rw-r--r--   0 runner    (1001) docker     (123)      306 2023-05-05 14:43:48.000000 pyroporn-0.1.6/pyroporn/types/style.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5255 2023-05-05 14:43:48.000000 pyroporn-0.1.6/pyroporn/types/text.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 14:44:03.479500 pyroporn-0.1.6/pyroporn/utilities/
+-rw-r--r--   0 runner    (1001) docker     (123)      189 2023-05-05 14:43:48.000000 pyroporn-0.1.6/pyroporn/utilities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1104 2023-05-05 14:43:48.000000 pyroporn-0.1.6/pyroporn/utilities/formater.py
+-rw-r--r--   0 runner    (1001) docker     (123)      572 2023-05-05 14:43:48.000000 pyroporn-0.1.6/pyroporn/utilities/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1811 2023-05-05 14:43:48.000000 pyroporn-0.1.6/pyroporn/utilities/mongo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1372 2023-05-05 14:43:48.000000 pyroporn-0.1.6/pyroporn/utilities/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-05-05 14:43:48.000000 pyroporn-0.1.6/pyroporn/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 14:44:03.475500 pyroporn-0.1.6/pyroporn.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      949 2023-05-05 14:44:03.000000 pyroporn-0.1.6/pyroporn.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1266 2023-05-05 14:44:03.000000 pyroporn-0.1.6/pyroporn.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 14:44:03.000000 pyroporn-0.1.6/pyroporn.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      202 2023-05-05 14:44:03.000000 pyroporn-0.1.6/pyroporn.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-05 14:44:03.000000 pyroporn-0.1.6/pyroporn.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-05 14:44:03.479500 pyroporn-0.1.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1618 2023-05-05 14:43:48.000000 pyroporn-0.1.6/setup.py
```

### Comparing `pyroporn-0.1.5/PKG-INFO` & `pyroporn-0.1.6/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyroporn
-Version: 0.1.5
+Version: 0.1.6
 Summary: Best Porn Code for the Pyrogram Library.
 Home-page: https://github.com/OTHFamily/pyroporn
 Author: TPro
 Author-email: 
 License: MIT
 Keywords: telegram pyrogram porn bot userbot
 Classifier: Programming Language :: Python
```

### Comparing `pyroporn-0.1.5/pyroporn/client.py` & `pyroporn-0.1.6/pyroporn/client.py`

 * *Files identical despite different names*

### Comparing `pyroporn-0.1.5/pyroporn/config.py` & `pyroporn-0.1.6/pyroporn/config.py`

 * *Files identical despite different names*

### Comparing `pyroporn-0.1.5/pyroporn/database/bdbDatabase.py` & `pyroporn-0.1.6/pyroporn/database/bdbDatabase.py`

 * *Files identical despite different names*

### Comparing `pyroporn-0.1.5/pyroporn/database/bubDatabase.py` & `pyroporn-0.1.6/pyroporn/database/bubDatabase.py`

 * *Files identical despite different names*

### Comparing `pyroporn-0.1.5/pyroporn/database/othDatabase.py` & `pyroporn-0.1.6/pyroporn/database/othDatabase.py`

 * *Files identical despite different names*

### Comparing `pyroporn-0.1.5/pyroporn/database/papDatabase.py` & `pyroporn-0.1.6/pyroporn/database/papDatabase.py`

 * *Files identical despite different names*

### Comparing `pyroporn-0.1.5/pyroporn/database/pmoDatabase.py` & `pyroporn-0.1.6/pyroporn/database/pmoDatabase.py`

 * *Files identical despite different names*

### Comparing `pyroporn-0.1.5/pyroporn/database/pobDatabase.py` & `pyroporn-0.1.6/pyroporn/database/pobDatabase.py`

 * *Files identical despite different names*

### Comparing `pyroporn-0.1.5/pyroporn/decorators/botcmd.py` & `pyroporn-0.1.6/pyroporn/decorators/oncmd.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from pyrogram import filters, enums
 
 from pyrogram.errors.exceptions.bad_request_400 import MessageIdInvalid
 
 
-class BotCmd:
-    def bot_cmd(
+class OnCmd:
+    def on_cmd(
         self,
         command: list,
         group: int = 0,
         owner: bool = False,
         private: bool = True
     ):
         """
@@ -18,35 +18,35 @@
 
             ``command``: List of commands
             ``group`` (optional): Handler group (Defaults to 0)
             ``owner`` (optional): True if the command is only for owner (Defaults to False)
             ``private`` (optional): True if the command is only for private chats (Defaults to True)
         """
         if owner:
-            _filter = (filters.user(self.OWNER_ID) & filters.command(command) & ~filters.via_bot & ~filters.forwarded)
+            filterm = (filters.user(self.OWNER_ID) & filters.me & filters.command(command, self.PREFIX) & ~filters.via_bot & ~filters.forwarded)
         else:
-            _filter = (filters.command(command) & ~filters.via_bot & ~filters.forwarded)
+            filterm = (filters.me & filters.command(command, self.PREFIX) & ~filters.via_bot & ~filters.forwarded)
         def decorators(func):
             async def wrapper(client, message):
                 chat_type = message.chat.type
                 if private and chat_type != enums.ChatType.PRIVATE:
                     return await message.reply_text(text="`Yo, perintah ini hanya untuk Pribadi!`")
                 try:
                     await func(client, message)
                 except MessageIdInvalid:
                     self.logs.warning("Jangan hapus pesan saat memproses. Ini dapat merusak bot!")
                 except BaseException as e:
                     self.logs.error(e)
                     
-            self.addhandler(wrapper, _filter, group)
+            self.addhandler(filterm, wrapper, group)
             return wrapper
         return decorators 
     
     
-    def bot_cf(self, custom_filters):
+    def on_cf(self, custom_filters):
         """
         ## Decorator to handle custom filters
 
         ### Arguments:
 
             ``custom_filters``: Custom filters to handle
             ``handler_group`` (optional): Handler group (Defaults to 0)
@@ -56,10 +56,10 @@
                 try:
                     await func(client, message)
                 except MessageIdInvalid:
                     self.logs.warning("Jangan hapus pesan saat memproses. Ini dapat merusak bot!")
                 except BaseException as e:
                     self.logs.error(e)
                 await message.continue_propagation()
-            self.addhandler(wrapper, custom_filters, handler_group)
+            self.addhandler(custom_filters, wrapper, handler_group)
             return wrapper
         return decorators
```

### Comparing `pyroporn-0.1.5/pyroporn/decorators/forcesub.py` & `pyroporn-0.1.6/pyroporn/decorators/forcesub.py`

 * *Files identical despite different names*

### Comparing `pyroporn-0.1.5/pyroporn/decorators/genbuttons.py` & `pyroporn-0.1.6/pyroporn/decorators/genbuttons.py`

 * *Files identical despite different names*

### Comparing `pyroporn-0.1.5/pyroporn/decorators/getlink.py` & `pyroporn-0.1.6/pyroporn/decorators/getlink.py`

 * *Files identical despite different names*

### Comparing `pyroporn-0.1.5/pyroporn/decorators/oncmd.py` & `pyroporn-0.1.6/pyroporn/decorators/botcmd.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from pyrogram import filters, enums
 
 from pyrogram.errors.exceptions.bad_request_400 import MessageIdInvalid
 
 
-class OnCmd:
-    def on_cmd(
+class BotCmd:
+    def bot_cmd(
         self,
         command: list,
         group: int = 0,
         owner: bool = False,
         private: bool = True
     ):
         """
@@ -18,35 +18,35 @@
 
             ``command``: List of commands
             ``group`` (optional): Handler group (Defaults to 0)
             ``owner`` (optional): True if the command is only for owner (Defaults to False)
             ``private`` (optional): True if the command is only for private chats (Defaults to True)
         """
         if owner:
-            _filter = (filters.user(self.OWNER_ID) & filters.me & filters.command(command, self.PREFIX) & ~filters.via_bot & ~filters.forwarded)
+            filterm = (filters.user(self.OWNER_ID) & filters.command(command) & ~filters.via_bot & ~filters.forwarded)
         else:
-            _filter = (filters.me & filters.command(command, self.PREFIX) & ~filters.via_bot & ~filters.forwarded)
+            filterm = (filters.command(command) & ~filters.via_bot & ~filters.forwarded)
         def decorators(func):
             async def wrapper(client, message):
                 chat_type = message.chat.type
                 if private and chat_type != enums.ChatType.PRIVATE:
                     return await message.reply_text(text="`Yo, perintah ini hanya untuk Pribadi!`")
                 try:
                     await func(client, message)
                 except MessageIdInvalid:
                     self.logs.warning("Jangan hapus pesan saat memproses. Ini dapat merusak bot!")
                 except BaseException as e:
                     self.logs.error(e)
                     
-            self.addhandler(wrapper, _filter, group)
+            self.addhandler(filterm, wrapper, group)
             return wrapper
         return decorators 
     
     
-    def on_cf(self, custom_filters):
+    def bot_cf(self, custom_filters):
         """
         ## Decorator to handle custom filters
 
         ### Arguments:
 
             ``custom_filters``: Custom filters to handle
             ``handler_group`` (optional): Handler group (Defaults to 0)
@@ -56,10 +56,10 @@
                 try:
                     await func(client, message)
                 except MessageIdInvalid:
                     self.logs.warning("Jangan hapus pesan saat memproses. Ini dapat merusak bot!")
                 except BaseException as e:
                     self.logs.error(e)
                 await message.continue_propagation()
-            self.addhandler(wrapper, custom_filters, handler_group)
+            self.addhandler(custom_filters, wrapper, handler_group)
             return wrapper
         return decorators
```

### Comparing `pyroporn-0.1.5/pyroporn/methods/content.py` & `pyroporn-0.1.6/pyroporn/methods/content.py`

 * *Files identical despite different names*

### Comparing `pyroporn-0.1.5/pyroporn/methods/getfile.py` & `pyroporn-0.1.6/pyroporn/methods/getfile.py`

 * *Files identical despite different names*

### Comparing `pyroporn-0.1.5/pyroporn/methods/message.py` & `pyroporn-0.1.6/pyroporn/methods/message.py`

 * *Files identical despite different names*

### Comparing `pyroporn-0.1.5/pyroporn/methods/thumbnail.py` & `pyroporn-0.1.6/pyroporn/methods/thumbnail.py`

 * *Files identical despite different names*

### Comparing `pyroporn-0.1.5/pyroporn/types/inline.py` & `pyroporn-0.1.6/pyroporn/types/inline.py`

 * *Files identical despite different names*

### Comparing `pyroporn-0.1.5/pyroporn/types/inlineBdb.py` & `pyroporn-0.1.6/pyroporn/types/inlineBdb.py`

 * *Files identical despite different names*

### Comparing `pyroporn-0.1.5/pyroporn/types/inlineBub.py` & `pyroporn-0.1.6/pyroporn/types/inlineBub.py`

 * *Files identical despite different names*

### Comparing `pyroporn-0.1.5/pyroporn/types/inlinePob.py` & `pyroporn-0.1.6/pyroporn/types/inlinePob.py`

 * *Files identical despite different names*

### Comparing `pyroporn-0.1.5/pyroporn/types/inlineVip.py` & `pyroporn-0.1.6/pyroporn/types/inlineVip.py`

 * *Files identical despite different names*

### Comparing `pyroporn-0.1.5/pyroporn/types/text.py` & `pyroporn-0.1.6/pyroporn/types/text.py`

 * *Files identical despite different names*

### Comparing `pyroporn-0.1.5/pyroporn/utilities/formater.py` & `pyroporn-0.1.6/pyroporn/utilities/formater.py`

 * *Files identical despite different names*

### Comparing `pyroporn-0.1.5/pyroporn/utilities/logger.py` & `pyroporn-0.1.6/pyroporn/utilities/logger.py`

 * *Files identical despite different names*

### Comparing `pyroporn-0.1.5/pyroporn/utilities/mongo.py` & `pyroporn-0.1.6/pyroporn/utilities/mongo.py`

 * *Files identical despite different names*

### Comparing `pyroporn-0.1.5/pyroporn/utilities/utils.py` & `pyroporn-0.1.6/pyroporn/utilities/utils.py`

 * *Files identical despite different names*

### Comparing `pyroporn-0.1.5/pyroporn.egg-info/PKG-INFO` & `pyroporn-0.1.6/pyroporn.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyroporn
-Version: 0.1.5
+Version: 0.1.6
 Summary: Best Porn Code for the Pyrogram Library.
 Home-page: https://github.com/OTHFamily/pyroporn
 Author: TPro
 Author-email: 
 License: MIT
 Keywords: telegram pyrogram porn bot userbot
 Classifier: Programming Language :: Python
```

### Comparing `pyroporn-0.1.5/pyroporn.egg-info/SOURCES.txt` & `pyroporn-0.1.6/pyroporn.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyroporn-0.1.5/setup.py` & `pyroporn-0.1.6/setup.py`

 * *Files identical despite different names*

