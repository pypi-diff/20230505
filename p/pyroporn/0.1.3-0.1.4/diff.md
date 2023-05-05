# Comparing `tmp/pyroporn-0.1.3.tar.gz` & `tmp/pyroporn-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyroporn-0.1.3.tar", last modified: Fri May  5 12:22:43 2023, max compression
+gzip compressed data, was "pyroporn-0.1.4.tar", last modified: Fri May  5 12:50:46 2023, max compression
```

## Comparing `pyroporn-0.1.3.tar` & `pyroporn-0.1.4.tar`

### file list

```diff
@@ -1,53 +1,53 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 12:22:43.921963 pyroporn-0.1.3/
--rw-r--r--   0 runner    (1001) docker     (123)      949 2023-05-05 12:22:43.921963 pyroporn-0.1.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-05-05 12:22:32.000000 pyroporn-0.1.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 12:22:43.913963 pyroporn-0.1.3/pyroporn/
--rw-r--r--   0 runner    (1001) docker     (123)       86 2023-05-05 12:22:32.000000 pyroporn-0.1.3/pyroporn/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    20759 2023-05-05 12:22:32.000000 pyroporn-0.1.3/pyroporn/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     6623 2023-05-05 12:22:32.000000 pyroporn-0.1.3/pyroporn/config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 12:22:43.917963 pyroporn-0.1.3/pyroporn/database/
--rw-r--r--   0 runner    (1001) docker     (123)      355 2023-05-05 12:22:32.000000 pyroporn-0.1.3/pyroporn/database/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5622 2023-05-05 12:22:32.000000 pyroporn-0.1.3/pyroporn/database/bdbDatabase.py
--rw-r--r--   0 runner    (1001) docker     (123)     1220 2023-05-05 12:22:32.000000 pyroporn-0.1.3/pyroporn/database/bubDatabase.py
--rw-r--r--   0 runner    (1001) docker     (123)     5839 2023-05-05 12:22:32.000000 pyroporn-0.1.3/pyroporn/database/othDatabase.py
--rw-r--r--   0 runner    (1001) docker     (123)     1612 2023-05-05 12:22:32.000000 pyroporn-0.1.3/pyroporn/database/papDatabase.py
--rw-r--r--   0 runner    (1001) docker     (123)     2838 2023-05-05 12:22:32.000000 pyroporn-0.1.3/pyroporn/database/pmoDatabase.py
--rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-05-05 12:22:32.000000 pyroporn-0.1.3/pyroporn/database/pobDatabase.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 12:22:43.917963 pyroporn-0.1.3/pyroporn/decorators/
--rw-r--r--   0 runner    (1001) docker     (123)      284 2023-05-05 12:22:32.000000 pyroporn-0.1.3/pyroporn/decorators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6317 2023-05-05 12:22:32.000000 pyroporn-0.1.3/pyroporn/decorators/forcesub.py
--rw-r--r--   0 runner    (1001) docker     (123)      814 2023-05-05 12:22:32.000000 pyroporn-0.1.3/pyroporn/decorators/genbuttons.py
--rw-r--r--   0 runner    (1001) docker     (123)      503 2023-05-05 12:22:32.000000 pyroporn-0.1.3/pyroporn/decorators/getjson.py
--rw-r--r--   0 runner    (1001) docker     (123)      514 2023-05-05 12:22:32.000000 pyroporn-0.1.3/pyroporn/decorators/getlink.py
--rw-r--r--   0 runner    (1001) docker     (123)     4326 2023-05-05 12:22:32.000000 pyroporn-0.1.3/pyroporn/decorators/oncmd.py
--rw-r--r--   0 runner    (1001) docker     (123)       86 2023-05-05 12:22:32.000000 pyroporn-0.1.3/pyroporn/decorators/task.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 12:22:43.921963 pyroporn-0.1.3/pyroporn/methods/
--rw-r--r--   0 runner    (1001) docker     (123)      184 2023-05-05 12:22:32.000000 pyroporn-0.1.3/pyroporn/methods/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1383 2023-05-05 12:22:32.000000 pyroporn-0.1.3/pyroporn/methods/content.py
--rw-r--r--   0 runner    (1001) docker     (123)     8161 2023-05-05 12:22:32.000000 pyroporn-0.1.3/pyroporn/methods/getfile.py
--rw-r--r--   0 runner    (1001) docker     (123)     7325 2023-05-05 12:22:32.000000 pyroporn-0.1.3/pyroporn/methods/message.py
--rw-r--r--   0 runner    (1001) docker     (123)     9364 2023-05-05 12:22:32.000000 pyroporn-0.1.3/pyroporn/methods/thumbnail.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 12:22:43.921963 pyroporn-0.1.3/pyroporn/types/
--rw-r--r--   0 runner    (1001) docker     (123)      329 2023-05-05 12:22:32.000000 pyroporn-0.1.3/pyroporn/types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10063 2023-05-05 12:22:32.000000 pyroporn-0.1.3/pyroporn/types/inline.py
--rw-r--r--   0 runner    (1001) docker     (123)     3942 2023-05-05 12:22:32.000000 pyroporn-0.1.3/pyroporn/types/inlineBdb.py
--rw-r--r--   0 runner    (1001) docker     (123)     4279 2023-05-05 12:22:32.000000 pyroporn-0.1.3/pyroporn/types/inlineBub.py
--rw-r--r--   0 runner    (1001) docker     (123)     5881 2023-05-05 12:22:32.000000 pyroporn-0.1.3/pyroporn/types/inlinePob.py
--rw-r--r--   0 runner    (1001) docker     (123)     3668 2023-05-05 12:22:32.000000 pyroporn-0.1.3/pyroporn/types/inlineVip.py
--rw-r--r--   0 runner    (1001) docker     (123)      306 2023-05-05 12:22:32.000000 pyroporn-0.1.3/pyroporn/types/style.py
--rw-r--r--   0 runner    (1001) docker     (123)     5255 2023-05-05 12:22:32.000000 pyroporn-0.1.3/pyroporn/types/text.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 12:22:43.921963 pyroporn-0.1.3/pyroporn/utilities/
--rw-r--r--   0 runner    (1001) docker     (123)      189 2023-05-05 12:22:32.000000 pyroporn-0.1.3/pyroporn/utilities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1104 2023-05-05 12:22:32.000000 pyroporn-0.1.3/pyroporn/utilities/formater.py
--rw-r--r--   0 runner    (1001) docker     (123)      572 2023-05-05 12:22:32.000000 pyroporn-0.1.3/pyroporn/utilities/logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     1811 2023-05-05 12:22:32.000000 pyroporn-0.1.3/pyroporn/utilities/mongo.py
--rw-r--r--   0 runner    (1001) docker     (123)     1372 2023-05-05 12:22:32.000000 pyroporn-0.1.3/pyroporn/utilities/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-05-05 12:22:32.000000 pyroporn-0.1.3/pyroporn/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 12:22:43.913963 pyroporn-0.1.3/pyroporn.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      949 2023-05-05 12:22:43.000000 pyroporn-0.1.3/pyroporn.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1202 2023-05-05 12:22:43.000000 pyroporn-0.1.3/pyroporn.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 12:22:43.000000 pyroporn-0.1.3/pyroporn.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      202 2023-05-05 12:22:43.000000 pyroporn-0.1.3/pyroporn.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-05 12:22:43.000000 pyroporn-0.1.3/pyroporn.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-05 12:22:43.921963 pyroporn-0.1.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1618 2023-05-05 12:22:32.000000 pyroporn-0.1.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 12:50:46.462905 pyroporn-0.1.4/
+-rw-r--r--   0 runner    (1001) docker     (123)      949 2023-05-05 12:50:46.462905 pyroporn-0.1.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-05-05 12:50:31.000000 pyroporn-0.1.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 12:50:46.458905 pyroporn-0.1.4/pyroporn/
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-05-05 12:50:31.000000 pyroporn-0.1.4/pyroporn/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20759 2023-05-05 12:50:31.000000 pyroporn-0.1.4/pyroporn/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6623 2023-05-05 12:50:31.000000 pyroporn-0.1.4/pyroporn/config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 12:50:46.458905 pyroporn-0.1.4/pyroporn/database/
+-rw-r--r--   0 runner    (1001) docker     (123)      355 2023-05-05 12:50:31.000000 pyroporn-0.1.4/pyroporn/database/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5622 2023-05-05 12:50:31.000000 pyroporn-0.1.4/pyroporn/database/bdbDatabase.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1220 2023-05-05 12:50:31.000000 pyroporn-0.1.4/pyroporn/database/bubDatabase.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5839 2023-05-05 12:50:31.000000 pyroporn-0.1.4/pyroporn/database/othDatabase.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1612 2023-05-05 12:50:31.000000 pyroporn-0.1.4/pyroporn/database/papDatabase.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2838 2023-05-05 12:50:31.000000 pyroporn-0.1.4/pyroporn/database/pmoDatabase.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-05-05 12:50:31.000000 pyroporn-0.1.4/pyroporn/database/pobDatabase.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 12:50:46.458905 pyroporn-0.1.4/pyroporn/decorators/
+-rw-r--r--   0 runner    (1001) docker     (123)      284 2023-05-05 12:50:31.000000 pyroporn-0.1.4/pyroporn/decorators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6317 2023-05-05 12:50:31.000000 pyroporn-0.1.4/pyroporn/decorators/forcesub.py
+-rw-r--r--   0 runner    (1001) docker     (123)      814 2023-05-05 12:50:31.000000 pyroporn-0.1.4/pyroporn/decorators/genbuttons.py
+-rw-r--r--   0 runner    (1001) docker     (123)      503 2023-05-05 12:50:31.000000 pyroporn-0.1.4/pyroporn/decorators/getjson.py
+-rw-r--r--   0 runner    (1001) docker     (123)      514 2023-05-05 12:50:31.000000 pyroporn-0.1.4/pyroporn/decorators/getlink.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3162 2023-05-05 12:50:31.000000 pyroporn-0.1.4/pyroporn/decorators/oncmd.py
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-05-05 12:50:31.000000 pyroporn-0.1.4/pyroporn/decorators/task.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 12:50:46.462905 pyroporn-0.1.4/pyroporn/methods/
+-rw-r--r--   0 runner    (1001) docker     (123)      184 2023-05-05 12:50:31.000000 pyroporn-0.1.4/pyroporn/methods/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1383 2023-05-05 12:50:31.000000 pyroporn-0.1.4/pyroporn/methods/content.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8161 2023-05-05 12:50:31.000000 pyroporn-0.1.4/pyroporn/methods/getfile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7325 2023-05-05 12:50:31.000000 pyroporn-0.1.4/pyroporn/methods/message.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9364 2023-05-05 12:50:31.000000 pyroporn-0.1.4/pyroporn/methods/thumbnail.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 12:50:46.462905 pyroporn-0.1.4/pyroporn/types/
+-rw-r--r--   0 runner    (1001) docker     (123)      329 2023-05-05 12:50:31.000000 pyroporn-0.1.4/pyroporn/types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10063 2023-05-05 12:50:31.000000 pyroporn-0.1.4/pyroporn/types/inline.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3942 2023-05-05 12:50:31.000000 pyroporn-0.1.4/pyroporn/types/inlineBdb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4279 2023-05-05 12:50:31.000000 pyroporn-0.1.4/pyroporn/types/inlineBub.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5881 2023-05-05 12:50:31.000000 pyroporn-0.1.4/pyroporn/types/inlinePob.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3668 2023-05-05 12:50:31.000000 pyroporn-0.1.4/pyroporn/types/inlineVip.py
+-rw-r--r--   0 runner    (1001) docker     (123)      306 2023-05-05 12:50:31.000000 pyroporn-0.1.4/pyroporn/types/style.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5255 2023-05-05 12:50:31.000000 pyroporn-0.1.4/pyroporn/types/text.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 12:50:46.462905 pyroporn-0.1.4/pyroporn/utilities/
+-rw-r--r--   0 runner    (1001) docker     (123)      189 2023-05-05 12:50:31.000000 pyroporn-0.1.4/pyroporn/utilities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1104 2023-05-05 12:50:31.000000 pyroporn-0.1.4/pyroporn/utilities/formater.py
+-rw-r--r--   0 runner    (1001) docker     (123)      572 2023-05-05 12:50:31.000000 pyroporn-0.1.4/pyroporn/utilities/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1811 2023-05-05 12:50:31.000000 pyroporn-0.1.4/pyroporn/utilities/mongo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1372 2023-05-05 12:50:31.000000 pyroporn-0.1.4/pyroporn/utilities/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-05-05 12:50:31.000000 pyroporn-0.1.4/pyroporn/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 12:50:46.458905 pyroporn-0.1.4/pyroporn.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      949 2023-05-05 12:50:46.000000 pyroporn-0.1.4/pyroporn.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1202 2023-05-05 12:50:46.000000 pyroporn-0.1.4/pyroporn.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 12:50:46.000000 pyroporn-0.1.4/pyroporn.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      202 2023-05-05 12:50:46.000000 pyroporn-0.1.4/pyroporn.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-05 12:50:46.000000 pyroporn-0.1.4/pyroporn.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-05 12:50:46.462905 pyroporn-0.1.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1618 2023-05-05 12:50:31.000000 pyroporn-0.1.4/setup.py
```

### Comparing `pyroporn-0.1.3/PKG-INFO` & `pyroporn-0.1.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyroporn
-Version: 0.1.3
+Version: 0.1.4
 Summary: Best Porn Code for the Pyrogram Library.
 Home-page: https://github.com/OTHFamily/pyroporn
 Author: TPro
 Author-email: 
 License: MIT
 Keywords: telegram pyrogram porn bot userbot
 Classifier: Programming Language :: Python
```

### Comparing `pyroporn-0.1.3/pyroporn/client.py` & `pyroporn-0.1.4/pyroporn/client.py`

 * *Files identical despite different names*

### Comparing `pyroporn-0.1.3/pyroporn/config.py` & `pyroporn-0.1.4/pyroporn/config.py`

 * *Files identical despite different names*

### Comparing `pyroporn-0.1.3/pyroporn/database/bdbDatabase.py` & `pyroporn-0.1.4/pyroporn/database/bdbDatabase.py`

 * *Files identical despite different names*

### Comparing `pyroporn-0.1.3/pyroporn/database/bubDatabase.py` & `pyroporn-0.1.4/pyroporn/database/bubDatabase.py`

 * *Files identical despite different names*

### Comparing `pyroporn-0.1.3/pyroporn/database/othDatabase.py` & `pyroporn-0.1.4/pyroporn/database/othDatabase.py`

 * *Files identical despite different names*

### Comparing `pyroporn-0.1.3/pyroporn/database/papDatabase.py` & `pyroporn-0.1.4/pyroporn/database/papDatabase.py`

 * *Files identical despite different names*

### Comparing `pyroporn-0.1.3/pyroporn/database/pmoDatabase.py` & `pyroporn-0.1.4/pyroporn/database/pmoDatabase.py`

 * *Files identical despite different names*

### Comparing `pyroporn-0.1.3/pyroporn/database/pobDatabase.py` & `pyroporn-0.1.4/pyroporn/database/pobDatabase.py`

 * *Files identical despite different names*

### Comparing `pyroporn-0.1.3/pyroporn/decorators/forcesub.py` & `pyroporn-0.1.4/pyroporn/decorators/forcesub.py`

 * *Files identical despite different names*

### Comparing `pyroporn-0.1.3/pyroporn/decorators/genbuttons.py` & `pyroporn-0.1.4/pyroporn/decorators/genbuttons.py`

 * *Files identical despite different names*

### Comparing `pyroporn-0.1.3/pyroporn/decorators/getlink.py` & `pyroporn-0.1.4/pyroporn/decorators/getlink.py`

 * *Files identical despite different names*

### Comparing `pyroporn-0.1.3/pyroporn/decorators/oncmd.py` & `pyroporn-0.1.4/pyroporn/decorators/oncmd.py`

 * *Files 24% similar despite different names*

```diff
@@ -20,53 +20,33 @@
 
             ``command``: List of commands
             ``group`` (optional): Handler group (Defaults to 0)
             ``owner`` (optional): True if the command is only for owner (Defaults to False)
             ``private`` (optional): True if the command is only for private chats (Defaults to True)
             ``userbot`` (optional): True if the command is only for userbot (Defaults to False)
         """
-        if userbot:
-            if owner:
-                _filter = (filters.user(self.OWNER_ID) & filters.me & filters.command(command, self.PREFIX) & ~filters.via_bot & ~filters.forwarded)
-            else:
-                _filter = (filters.me & filters.command(command, self.PREFIX) & ~filters.via_bot & ~filters.forwarded)
-            def decorators(func):
-                async def wrapper(client, message):
-                    chat_type = message.chat.type
-                    if private and chat_type != enums.ChatType.PRIVATE:
-                        return await message.reply_text(text="`Yo, perintah ini hanya untuk Pribadi!`")
-                    try:
-                        await func(client, message)
-                    except MessageIdInvalid:
-                        self.logs.warning("Jangan hapus pesan saat memproses. Ini dapat merusak bot!")
-                    except BaseException as e:
-                        self.logs.error(f"\nModule - {func.__module__} | Command: {command[0]} | Traceback: \n{e}")
-                        
-                self.addhandler(wrapper, _filter, group)
-                return wrapper
+        if owner:
+            _filter = (filters.user(self.OWNER_ID) & filters.me & filters.command(command, self.PREFIX) & ~filters.via_bot & ~filters.forwarded)
         else:
-            if owner:
-                _filter = (filters.user(self.OWNER_ID) & filters.command(command) & ~filters.via_bot & ~filters.forwarded)
-            else:
-                _filter = (filters.command(command) & ~filters.via_bot & ~filters.forwarded)
-            def decorators(func):
-                async def wrapper(client, message):
-                    chat_type = message.chat.type
-                    if private and chat_type != enums.ChatType.PRIVATE:
-                        return await message.reply_text(text="`Yo, perintah ini hanya untuk Pribadi!`")
-                    try:
-                        await func(client, message)
-                    except MessageIdInvalid:
-                        self.logs.warning("Jangan hapus pesan saat memproses. Ini dapat merusak bot!")
-                    except BaseException as e:
-                        self.logs.error(f"\nModule - {func.__module__} | Command: {command[0]} | Traceback: \n{e}")
-                        
-                self.addhandler(wrapper, _filter, group)
-                return wrapper
-            return decorators
+            _filter = (filters.me & filters.command(command, self.PREFIX) & ~filters.via_bot & ~filters.forwarded)
+        def decorators(func):
+            async def wrapper(client, message):
+                chat_type = message.chat.type
+                if private and chat_type != enums.ChatType.PRIVATE:
+                    return await message.reply_text(text="`Yo, perintah ini hanya untuk Pribadi!`")
+                try:
+                    await func(client, message)
+                except MessageIdInvalid:
+                    self.logs.warning("Jangan hapus pesan saat memproses. Ini dapat merusak bot!")
+                except BaseException as e:
+                    self.logs.error(f"\nModule - {func.__module__} | Command: {command[0]} | Traceback: \n{e}")
+                    
+            self.addhandler(wrapper, _filter, group)
+            return wrapper
+        return decorators 
     
     
     @classmethod
     def on_cf(self, custom_filters):
         """
         ## Decorator to handle custom filters
 
@@ -95,8 +75,8 @@
 
         ### Arguments:
 
             ``wrapper``: Callback function
             ``_filter``: Filters
             ``cmdgrp``: Command Group
         """
-        self.add_handler(MessageHandler(wrapper, _filter), cmdgrp)
+        self.add_handler(MessageHandler(wrapper, filters=_filter), group=cmdgrp)
```

### Comparing `pyroporn-0.1.3/pyroporn/methods/content.py` & `pyroporn-0.1.4/pyroporn/methods/content.py`

 * *Files identical despite different names*

### Comparing `pyroporn-0.1.3/pyroporn/methods/getfile.py` & `pyroporn-0.1.4/pyroporn/methods/getfile.py`

 * *Files identical despite different names*

### Comparing `pyroporn-0.1.3/pyroporn/methods/message.py` & `pyroporn-0.1.4/pyroporn/methods/message.py`

 * *Files identical despite different names*

### Comparing `pyroporn-0.1.3/pyroporn/methods/thumbnail.py` & `pyroporn-0.1.4/pyroporn/methods/thumbnail.py`

 * *Files identical despite different names*

### Comparing `pyroporn-0.1.3/pyroporn/types/inline.py` & `pyroporn-0.1.4/pyroporn/types/inline.py`

 * *Files identical despite different names*

### Comparing `pyroporn-0.1.3/pyroporn/types/inlineBdb.py` & `pyroporn-0.1.4/pyroporn/types/inlineBdb.py`

 * *Files identical despite different names*

### Comparing `pyroporn-0.1.3/pyroporn/types/inlineBub.py` & `pyroporn-0.1.4/pyroporn/types/inlineBub.py`

 * *Files identical despite different names*

### Comparing `pyroporn-0.1.3/pyroporn/types/inlinePob.py` & `pyroporn-0.1.4/pyroporn/types/inlinePob.py`

 * *Files identical despite different names*

### Comparing `pyroporn-0.1.3/pyroporn/types/inlineVip.py` & `pyroporn-0.1.4/pyroporn/types/inlineVip.py`

 * *Files identical despite different names*

### Comparing `pyroporn-0.1.3/pyroporn/types/text.py` & `pyroporn-0.1.4/pyroporn/types/text.py`

 * *Files identical despite different names*

### Comparing `pyroporn-0.1.3/pyroporn/utilities/formater.py` & `pyroporn-0.1.4/pyroporn/utilities/formater.py`

 * *Files identical despite different names*

### Comparing `pyroporn-0.1.3/pyroporn/utilities/logger.py` & `pyroporn-0.1.4/pyroporn/utilities/logger.py`

 * *Files identical despite different names*

### Comparing `pyroporn-0.1.3/pyroporn/utilities/mongo.py` & `pyroporn-0.1.4/pyroporn/utilities/mongo.py`

 * *Files identical despite different names*

### Comparing `pyroporn-0.1.3/pyroporn/utilities/utils.py` & `pyroporn-0.1.4/pyroporn/utilities/utils.py`

 * *Files identical despite different names*

### Comparing `pyroporn-0.1.3/pyroporn.egg-info/PKG-INFO` & `pyroporn-0.1.4/pyroporn.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyroporn
-Version: 0.1.3
+Version: 0.1.4
 Summary: Best Porn Code for the Pyrogram Library.
 Home-page: https://github.com/OTHFamily/pyroporn
 Author: TPro
 Author-email: 
 License: MIT
 Keywords: telegram pyrogram porn bot userbot
 Classifier: Programming Language :: Python
```

### Comparing `pyroporn-0.1.3/pyroporn.egg-info/SOURCES.txt` & `pyroporn-0.1.4/pyroporn.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyroporn-0.1.3/setup.py` & `pyroporn-0.1.4/setup.py`

 * *Files identical despite different names*

