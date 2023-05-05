# Comparing `tmp/pyroporn-0.1.1.tar.gz` & `tmp/pyroporn-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyroporn-0.1.1.tar", last modified: Fri May  5 11:12:56 2023, max compression
+gzip compressed data, was "pyroporn-0.1.2.tar", last modified: Fri May  5 11:57:06 2023, max compression
```

## Comparing `pyroporn-0.1.1.tar` & `pyroporn-0.1.2.tar`

### file list

```diff
@@ -1,53 +1,53 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 11:12:56.555147 pyroporn-0.1.1/
--rw-r--r--   0 runner    (1001) docker     (123)      949 2023-05-05 11:12:56.555147 pyroporn-0.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-05-05 11:12:43.000000 pyroporn-0.1.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 11:12:56.547147 pyroporn-0.1.1/pyroporn/
--rw-r--r--   0 runner    (1001) docker     (123)       86 2023-05-05 11:12:43.000000 pyroporn-0.1.1/pyroporn/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    20759 2023-05-05 11:12:43.000000 pyroporn-0.1.1/pyroporn/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     6623 2023-05-05 11:12:43.000000 pyroporn-0.1.1/pyroporn/config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 11:12:56.551147 pyroporn-0.1.1/pyroporn/database/
--rw-r--r--   0 runner    (1001) docker     (123)      355 2023-05-05 11:12:43.000000 pyroporn-0.1.1/pyroporn/database/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5622 2023-05-05 11:12:43.000000 pyroporn-0.1.1/pyroporn/database/bdbDatabase.py
--rw-r--r--   0 runner    (1001) docker     (123)     1220 2023-05-05 11:12:43.000000 pyroporn-0.1.1/pyroporn/database/bubDatabase.py
--rw-r--r--   0 runner    (1001) docker     (123)     5839 2023-05-05 11:12:43.000000 pyroporn-0.1.1/pyroporn/database/othDatabase.py
--rw-r--r--   0 runner    (1001) docker     (123)     1612 2023-05-05 11:12:43.000000 pyroporn-0.1.1/pyroporn/database/papDatabase.py
--rw-r--r--   0 runner    (1001) docker     (123)     2838 2023-05-05 11:12:43.000000 pyroporn-0.1.1/pyroporn/database/pmoDatabase.py
--rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-05-05 11:12:43.000000 pyroporn-0.1.1/pyroporn/database/pobDatabase.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 11:12:56.551147 pyroporn-0.1.1/pyroporn/decorators/
--rw-r--r--   0 runner    (1001) docker     (123)      284 2023-05-05 11:12:43.000000 pyroporn-0.1.1/pyroporn/decorators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6317 2023-05-05 11:12:43.000000 pyroporn-0.1.1/pyroporn/decorators/forcesub.py
--rw-r--r--   0 runner    (1001) docker     (123)      814 2023-05-05 11:12:43.000000 pyroporn-0.1.1/pyroporn/decorators/genbuttons.py
--rw-r--r--   0 runner    (1001) docker     (123)      503 2023-05-05 11:12:43.000000 pyroporn-0.1.1/pyroporn/decorators/getjson.py
--rw-r--r--   0 runner    (1001) docker     (123)      514 2023-05-05 11:12:43.000000 pyroporn-0.1.1/pyroporn/decorators/getlink.py
--rw-r--r--   0 runner    (1001) docker     (123)     3468 2023-05-05 11:12:43.000000 pyroporn-0.1.1/pyroporn/decorators/oncmd.py
--rw-r--r--   0 runner    (1001) docker     (123)       86 2023-05-05 11:12:43.000000 pyroporn-0.1.1/pyroporn/decorators/task.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 11:12:56.551147 pyroporn-0.1.1/pyroporn/methods/
--rw-r--r--   0 runner    (1001) docker     (123)      184 2023-05-05 11:12:43.000000 pyroporn-0.1.1/pyroporn/methods/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1383 2023-05-05 11:12:43.000000 pyroporn-0.1.1/pyroporn/methods/content.py
--rw-r--r--   0 runner    (1001) docker     (123)     8161 2023-05-05 11:12:43.000000 pyroporn-0.1.1/pyroporn/methods/getfile.py
--rw-r--r--   0 runner    (1001) docker     (123)     7325 2023-05-05 11:12:43.000000 pyroporn-0.1.1/pyroporn/methods/message.py
--rw-r--r--   0 runner    (1001) docker     (123)     9364 2023-05-05 11:12:43.000000 pyroporn-0.1.1/pyroporn/methods/thumbnail.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 11:12:56.551147 pyroporn-0.1.1/pyroporn/types/
--rw-r--r--   0 runner    (1001) docker     (123)      329 2023-05-05 11:12:43.000000 pyroporn-0.1.1/pyroporn/types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10063 2023-05-05 11:12:43.000000 pyroporn-0.1.1/pyroporn/types/inline.py
--rw-r--r--   0 runner    (1001) docker     (123)     3942 2023-05-05 11:12:43.000000 pyroporn-0.1.1/pyroporn/types/inlineBdb.py
--rw-r--r--   0 runner    (1001) docker     (123)     4279 2023-05-05 11:12:43.000000 pyroporn-0.1.1/pyroporn/types/inlineBub.py
--rw-r--r--   0 runner    (1001) docker     (123)     5881 2023-05-05 11:12:43.000000 pyroporn-0.1.1/pyroporn/types/inlinePob.py
--rw-r--r--   0 runner    (1001) docker     (123)     3668 2023-05-05 11:12:43.000000 pyroporn-0.1.1/pyroporn/types/inlineVip.py
--rw-r--r--   0 runner    (1001) docker     (123)      306 2023-05-05 11:12:43.000000 pyroporn-0.1.1/pyroporn/types/style.py
--rw-r--r--   0 runner    (1001) docker     (123)     5255 2023-05-05 11:12:43.000000 pyroporn-0.1.1/pyroporn/types/text.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 11:12:56.555147 pyroporn-0.1.1/pyroporn/utilities/
--rw-r--r--   0 runner    (1001) docker     (123)      189 2023-05-05 11:12:43.000000 pyroporn-0.1.1/pyroporn/utilities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1104 2023-05-05 11:12:43.000000 pyroporn-0.1.1/pyroporn/utilities/formater.py
--rw-r--r--   0 runner    (1001) docker     (123)      572 2023-05-05 11:12:43.000000 pyroporn-0.1.1/pyroporn/utilities/logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     1811 2023-05-05 11:12:43.000000 pyroporn-0.1.1/pyroporn/utilities/mongo.py
--rw-r--r--   0 runner    (1001) docker     (123)     1372 2023-05-05 11:12:43.000000 pyroporn-0.1.1/pyroporn/utilities/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-05-05 11:12:43.000000 pyroporn-0.1.1/pyroporn/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 11:12:56.547147 pyroporn-0.1.1/pyroporn.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      949 2023-05-05 11:12:56.000000 pyroporn-0.1.1/pyroporn.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1202 2023-05-05 11:12:56.000000 pyroporn-0.1.1/pyroporn.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 11:12:56.000000 pyroporn-0.1.1/pyroporn.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      202 2023-05-05 11:12:56.000000 pyroporn-0.1.1/pyroporn.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-05 11:12:56.000000 pyroporn-0.1.1/pyroporn.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-05 11:12:56.555147 pyroporn-0.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1618 2023-05-05 11:12:43.000000 pyroporn-0.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 11:57:06.082633 pyroporn-0.1.2/
+-rw-r--r--   0 runner    (1001) docker     (123)      949 2023-05-05 11:57:06.082633 pyroporn-0.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-05-05 11:56:54.000000 pyroporn-0.1.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 11:57:06.078633 pyroporn-0.1.2/pyroporn/
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-05-05 11:56:54.000000 pyroporn-0.1.2/pyroporn/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20759 2023-05-05 11:56:54.000000 pyroporn-0.1.2/pyroporn/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6623 2023-05-05 11:56:54.000000 pyroporn-0.1.2/pyroporn/config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 11:57:06.078633 pyroporn-0.1.2/pyroporn/database/
+-rw-r--r--   0 runner    (1001) docker     (123)      355 2023-05-05 11:56:54.000000 pyroporn-0.1.2/pyroporn/database/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5622 2023-05-05 11:56:54.000000 pyroporn-0.1.2/pyroporn/database/bdbDatabase.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1220 2023-05-05 11:56:54.000000 pyroporn-0.1.2/pyroporn/database/bubDatabase.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5839 2023-05-05 11:56:54.000000 pyroporn-0.1.2/pyroporn/database/othDatabase.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1612 2023-05-05 11:56:54.000000 pyroporn-0.1.2/pyroporn/database/papDatabase.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2838 2023-05-05 11:56:54.000000 pyroporn-0.1.2/pyroporn/database/pmoDatabase.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-05-05 11:56:54.000000 pyroporn-0.1.2/pyroporn/database/pobDatabase.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 11:57:06.078633 pyroporn-0.1.2/pyroporn/decorators/
+-rw-r--r--   0 runner    (1001) docker     (123)      284 2023-05-05 11:56:54.000000 pyroporn-0.1.2/pyroporn/decorators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6317 2023-05-05 11:56:54.000000 pyroporn-0.1.2/pyroporn/decorators/forcesub.py
+-rw-r--r--   0 runner    (1001) docker     (123)      814 2023-05-05 11:56:54.000000 pyroporn-0.1.2/pyroporn/decorators/genbuttons.py
+-rw-r--r--   0 runner    (1001) docker     (123)      503 2023-05-05 11:56:54.000000 pyroporn-0.1.2/pyroporn/decorators/getjson.py
+-rw-r--r--   0 runner    (1001) docker     (123)      514 2023-05-05 11:56:54.000000 pyroporn-0.1.2/pyroporn/decorators/getlink.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3480 2023-05-05 11:56:54.000000 pyroporn-0.1.2/pyroporn/decorators/oncmd.py
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-05-05 11:56:54.000000 pyroporn-0.1.2/pyroporn/decorators/task.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 11:57:06.078633 pyroporn-0.1.2/pyroporn/methods/
+-rw-r--r--   0 runner    (1001) docker     (123)      184 2023-05-05 11:56:54.000000 pyroporn-0.1.2/pyroporn/methods/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1383 2023-05-05 11:56:54.000000 pyroporn-0.1.2/pyroporn/methods/content.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8161 2023-05-05 11:56:54.000000 pyroporn-0.1.2/pyroporn/methods/getfile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7325 2023-05-05 11:56:54.000000 pyroporn-0.1.2/pyroporn/methods/message.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9364 2023-05-05 11:56:54.000000 pyroporn-0.1.2/pyroporn/methods/thumbnail.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 11:57:06.082633 pyroporn-0.1.2/pyroporn/types/
+-rw-r--r--   0 runner    (1001) docker     (123)      329 2023-05-05 11:56:54.000000 pyroporn-0.1.2/pyroporn/types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10063 2023-05-05 11:56:54.000000 pyroporn-0.1.2/pyroporn/types/inline.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3942 2023-05-05 11:56:54.000000 pyroporn-0.1.2/pyroporn/types/inlineBdb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4279 2023-05-05 11:56:54.000000 pyroporn-0.1.2/pyroporn/types/inlineBub.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5881 2023-05-05 11:56:54.000000 pyroporn-0.1.2/pyroporn/types/inlinePob.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3668 2023-05-05 11:56:54.000000 pyroporn-0.1.2/pyroporn/types/inlineVip.py
+-rw-r--r--   0 runner    (1001) docker     (123)      306 2023-05-05 11:56:54.000000 pyroporn-0.1.2/pyroporn/types/style.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5255 2023-05-05 11:56:54.000000 pyroporn-0.1.2/pyroporn/types/text.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 11:57:06.082633 pyroporn-0.1.2/pyroporn/utilities/
+-rw-r--r--   0 runner    (1001) docker     (123)      189 2023-05-05 11:56:54.000000 pyroporn-0.1.2/pyroporn/utilities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1104 2023-05-05 11:56:54.000000 pyroporn-0.1.2/pyroporn/utilities/formater.py
+-rw-r--r--   0 runner    (1001) docker     (123)      572 2023-05-05 11:56:54.000000 pyroporn-0.1.2/pyroporn/utilities/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1811 2023-05-05 11:56:54.000000 pyroporn-0.1.2/pyroporn/utilities/mongo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1372 2023-05-05 11:56:54.000000 pyroporn-0.1.2/pyroporn/utilities/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-05-05 11:56:54.000000 pyroporn-0.1.2/pyroporn/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 11:57:06.078633 pyroporn-0.1.2/pyroporn.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      949 2023-05-05 11:57:06.000000 pyroporn-0.1.2/pyroporn.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1202 2023-05-05 11:57:06.000000 pyroporn-0.1.2/pyroporn.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 11:57:06.000000 pyroporn-0.1.2/pyroporn.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      202 2023-05-05 11:57:06.000000 pyroporn-0.1.2/pyroporn.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-05 11:57:06.000000 pyroporn-0.1.2/pyroporn.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-05 11:57:06.082633 pyroporn-0.1.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1618 2023-05-05 11:56:54.000000 pyroporn-0.1.2/setup.py
```

### Comparing `pyroporn-0.1.1/PKG-INFO` & `pyroporn-0.1.2/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyroporn
-Version: 0.1.1
+Version: 0.1.2
 Summary: Best Porn Code for the Pyrogram Library.
 Home-page: https://github.com/OTHFamily/pyroporn
 Author: TPro
 Author-email: 
 License: MIT
 Keywords: telegram pyrogram porn bot userbot
 Classifier: Programming Language :: Python
```

### Comparing `pyroporn-0.1.1/pyroporn/client.py` & `pyroporn-0.1.2/pyroporn/client.py`

 * *Files identical despite different names*

### Comparing `pyroporn-0.1.1/pyroporn/config.py` & `pyroporn-0.1.2/pyroporn/config.py`

 * *Files identical despite different names*

### Comparing `pyroporn-0.1.1/pyroporn/database/bdbDatabase.py` & `pyroporn-0.1.2/pyroporn/database/bdbDatabase.py`

 * *Files identical despite different names*

### Comparing `pyroporn-0.1.1/pyroporn/database/bubDatabase.py` & `pyroporn-0.1.2/pyroporn/database/bubDatabase.py`

 * *Files identical despite different names*

### Comparing `pyroporn-0.1.1/pyroporn/database/othDatabase.py` & `pyroporn-0.1.2/pyroporn/database/othDatabase.py`

 * *Files identical despite different names*

### Comparing `pyroporn-0.1.1/pyroporn/database/papDatabase.py` & `pyroporn-0.1.2/pyroporn/database/papDatabase.py`

 * *Files identical despite different names*

### Comparing `pyroporn-0.1.1/pyroporn/database/pmoDatabase.py` & `pyroporn-0.1.2/pyroporn/database/pmoDatabase.py`

 * *Files identical despite different names*

### Comparing `pyroporn-0.1.1/pyroporn/database/pobDatabase.py` & `pyroporn-0.1.2/pyroporn/database/pobDatabase.py`

 * *Files identical despite different names*

### Comparing `pyroporn-0.1.1/pyroporn/decorators/forcesub.py` & `pyroporn-0.1.2/pyroporn/decorators/forcesub.py`

 * *Files identical despite different names*

### Comparing `pyroporn-0.1.1/pyroporn/decorators/genbuttons.py` & `pyroporn-0.1.2/pyroporn/decorators/genbuttons.py`

 * *Files identical despite different names*

### Comparing `pyroporn-0.1.1/pyroporn/decorators/getlink.py` & `pyroporn-0.1.2/pyroporn/decorators/getlink.py`

 * *Files identical despite different names*

### Comparing `pyroporn-0.1.1/pyroporn/decorators/oncmd.py` & `pyroporn-0.1.2/pyroporn/decorators/oncmd.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,10 @@
+import os
+import asyncio
+
 from pyrogram import filters, enums
 from pyrogram.handlers import MessageHandler
 from pyrogram.errors.exceptions.bad_request_400 import MessageIdInvalid
 
 
 class OnCmd:
     @classmethod
@@ -81,8 +84,8 @@
 
         ### Arguments:
 
             ``wrapper``: Callback function
             ``_filter``: Filters
             ``cmdgrp``: Command Group
         """
-        self.add_handler(MessageHandler(wrapper, filters=_filter), group=cmdgrp)
+        self.add_handler(MessageHandler(wrapper, _filter), cmdgrp)
```

### Comparing `pyroporn-0.1.1/pyroporn/methods/content.py` & `pyroporn-0.1.2/pyroporn/methods/content.py`

 * *Files identical despite different names*

### Comparing `pyroporn-0.1.1/pyroporn/methods/getfile.py` & `pyroporn-0.1.2/pyroporn/methods/getfile.py`

 * *Files identical despite different names*

### Comparing `pyroporn-0.1.1/pyroporn/methods/message.py` & `pyroporn-0.1.2/pyroporn/methods/message.py`

 * *Files identical despite different names*

### Comparing `pyroporn-0.1.1/pyroporn/methods/thumbnail.py` & `pyroporn-0.1.2/pyroporn/methods/thumbnail.py`

 * *Files identical despite different names*

### Comparing `pyroporn-0.1.1/pyroporn/types/inline.py` & `pyroporn-0.1.2/pyroporn/types/inline.py`

 * *Files identical despite different names*

### Comparing `pyroporn-0.1.1/pyroporn/types/inlineBdb.py` & `pyroporn-0.1.2/pyroporn/types/inlineBdb.py`

 * *Files identical despite different names*

### Comparing `pyroporn-0.1.1/pyroporn/types/inlineBub.py` & `pyroporn-0.1.2/pyroporn/types/inlineBub.py`

 * *Files identical despite different names*

### Comparing `pyroporn-0.1.1/pyroporn/types/inlinePob.py` & `pyroporn-0.1.2/pyroporn/types/inlinePob.py`

 * *Files identical despite different names*

### Comparing `pyroporn-0.1.1/pyroporn/types/inlineVip.py` & `pyroporn-0.1.2/pyroporn/types/inlineVip.py`

 * *Files identical despite different names*

### Comparing `pyroporn-0.1.1/pyroporn/types/text.py` & `pyroporn-0.1.2/pyroporn/types/text.py`

 * *Files identical despite different names*

### Comparing `pyroporn-0.1.1/pyroporn/utilities/formater.py` & `pyroporn-0.1.2/pyroporn/utilities/formater.py`

 * *Files identical despite different names*

### Comparing `pyroporn-0.1.1/pyroporn/utilities/logger.py` & `pyroporn-0.1.2/pyroporn/utilities/logger.py`

 * *Files identical despite different names*

### Comparing `pyroporn-0.1.1/pyroporn/utilities/mongo.py` & `pyroporn-0.1.2/pyroporn/utilities/mongo.py`

 * *Files identical despite different names*

### Comparing `pyroporn-0.1.1/pyroporn/utilities/utils.py` & `pyroporn-0.1.2/pyroporn/utilities/utils.py`

 * *Files identical despite different names*

### Comparing `pyroporn-0.1.1/pyroporn.egg-info/PKG-INFO` & `pyroporn-0.1.2/pyroporn.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyroporn
-Version: 0.1.1
+Version: 0.1.2
 Summary: Best Porn Code for the Pyrogram Library.
 Home-page: https://github.com/OTHFamily/pyroporn
 Author: TPro
 Author-email: 
 License: MIT
 Keywords: telegram pyrogram porn bot userbot
 Classifier: Programming Language :: Python
```

### Comparing `pyroporn-0.1.1/pyroporn.egg-info/SOURCES.txt` & `pyroporn-0.1.2/pyroporn.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyroporn-0.1.1/setup.py` & `pyroporn-0.1.2/setup.py`

 * *Files identical despite different names*

