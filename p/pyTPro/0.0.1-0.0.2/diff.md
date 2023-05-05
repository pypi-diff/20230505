# Comparing `tmp/pyTPro-0.0.1.tar.gz` & `tmp/pyTPro-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyTPro-0.0.1.tar", last modified: Fri May  5 07:06:05 2023, max compression
+gzip compressed data, was "pyTPro-0.0.2.tar", last modified: Fri May  5 07:58:38 2023, max compression
```

## Comparing `pyTPro-0.0.1.tar` & `pyTPro-0.0.2.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 07:06:05.586779 pyTPro-0.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)      932 2023-05-05 07:06:05.586779 pyTPro-0.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-05-05 07:05:53.000000 pyTPro-0.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 07:06:05.578780 pyTPro-0.0.1/Tele/
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-05-05 07:05:53.000000 pyTPro-0.0.1/Tele/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    20623 2023-05-05 07:05:53.000000 pyTPro-0.0.1/Tele/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     6623 2023-05-05 07:05:53.000000 pyTPro-0.0.1/Tele/config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 07:06:05.578780 pyTPro-0.0.1/Tele/database/
--rw-r--r--   0 runner    (1001) docker     (123)      355 2023-05-05 07:05:53.000000 pyTPro-0.0.1/Tele/database/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5622 2023-05-05 07:05:53.000000 pyTPro-0.0.1/Tele/database/bdbDatabase.py
--rw-r--r--   0 runner    (1001) docker     (123)     1220 2023-05-05 07:05:53.000000 pyTPro-0.0.1/Tele/database/bubDatabase.py
--rw-r--r--   0 runner    (1001) docker     (123)     5839 2023-05-05 07:05:53.000000 pyTPro-0.0.1/Tele/database/othDatabase.py
--rw-r--r--   0 runner    (1001) docker     (123)     1612 2023-05-05 07:05:53.000000 pyTPro-0.0.1/Tele/database/papDatabase.py
--rw-r--r--   0 runner    (1001) docker     (123)     2838 2023-05-05 07:05:53.000000 pyTPro-0.0.1/Tele/database/pmoDatabase.py
--rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-05-05 07:05:53.000000 pyTPro-0.0.1/Tele/database/pobDatabase.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 07:06:05.578780 pyTPro-0.0.1/Tele/decorators/
--rw-r--r--   0 runner    (1001) docker     (123)      144 2023-05-05 07:05:53.000000 pyTPro-0.0.1/Tele/decorators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6317 2023-05-05 07:05:53.000000 pyTPro-0.0.1/Tele/decorators/forcesub.py
--rw-r--r--   0 runner    (1001) docker     (123)     3169 2023-05-05 07:05:53.000000 pyTPro-0.0.1/Tele/decorators/oncmd.py
--rw-r--r--   0 runner    (1001) docker     (123)     1891 2023-05-05 07:05:53.000000 pyTPro-0.0.1/Tele/decorators/task.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 07:06:05.582780 pyTPro-0.0.1/Tele/methods/
--rw-r--r--   0 runner    (1001) docker     (123)      200 2023-05-05 07:05:53.000000 pyTPro-0.0.1/Tele/methods/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1383 2023-05-05 07:05:53.000000 pyTPro-0.0.1/Tele/methods/content.py
--rw-r--r--   0 runner    (1001) docker     (123)     8161 2023-05-05 07:05:53.000000 pyTPro-0.0.1/Tele/methods/getfile.py
--rw-r--r--   0 runner    (1001) docker     (123)     8433 2023-05-05 07:05:53.000000 pyTPro-0.0.1/Tele/methods/message.py
--rw-r--r--   0 runner    (1001) docker     (123)     9364 2023-05-05 07:05:53.000000 pyTPro-0.0.1/Tele/methods/thumbnail.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 07:06:05.582780 pyTPro-0.0.1/Tele/types/
--rw-r--r--   0 runner    (1001) docker     (123)      326 2023-05-05 07:05:53.000000 pyTPro-0.0.1/Tele/types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10063 2023-05-05 07:05:53.000000 pyTPro-0.0.1/Tele/types/inline.py
--rw-r--r--   0 runner    (1001) docker     (123)     3942 2023-05-05 07:05:53.000000 pyTPro-0.0.1/Tele/types/inlineBdb.py
--rw-r--r--   0 runner    (1001) docker     (123)     4279 2023-05-05 07:05:53.000000 pyTPro-0.0.1/Tele/types/inlineBub.py
--rw-r--r--   0 runner    (1001) docker     (123)     5881 2023-05-05 07:05:53.000000 pyTPro-0.0.1/Tele/types/inlinePob.py
--rw-r--r--   0 runner    (1001) docker     (123)     3668 2023-05-05 07:05:53.000000 pyTPro-0.0.1/Tele/types/inlineVip.py
--rw-r--r--   0 runner    (1001) docker     (123)      306 2023-05-05 07:05:53.000000 pyTPro-0.0.1/Tele/types/style.py
--rw-r--r--   0 runner    (1001) docker     (123)     5255 2023-05-05 07:05:53.000000 pyTPro-0.0.1/Tele/types/text.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 07:06:05.582780 pyTPro-0.0.1/Tele/utilities/
--rw-r--r--   0 runner    (1001) docker     (123)      124 2023-05-05 07:05:53.000000 pyTPro-0.0.1/Tele/utilities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      568 2023-05-05 07:05:53.000000 pyTPro-0.0.1/Tele/utilities/logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     1807 2023-05-05 07:05:53.000000 pyTPro-0.0.1/Tele/utilities/mongo.py
--rw-r--r--   0 runner    (1001) docker     (123)     1368 2023-05-05 07:05:53.000000 pyTPro-0.0.1/Tele/utilities/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 07:06:05.586779 pyTPro-0.0.1/pyTPro.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      932 2023-05-05 07:06:05.000000 pyTPro-0.0.1/pyTPro.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      921 2023-05-05 07:06:05.000000 pyTPro-0.0.1/pyTPro.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 07:06:05.000000 pyTPro-0.0.1/pyTPro.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      202 2023-05-05 07:06:05.000000 pyTPro-0.0.1/pyTPro.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-05-05 07:06:05.000000 pyTPro-0.0.1/pyTPro.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-05 07:06:05.586779 pyTPro-0.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1611 2023-05-05 07:05:53.000000 pyTPro-0.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 07:58:38.374040 pyTPro-0.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)      932 2023-05-05 07:58:38.374040 pyTPro-0.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-05-05 07:58:27.000000 pyTPro-0.0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 07:58:38.366040 pyTPro-0.0.2/Tele/
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-05-05 07:58:27.000000 pyTPro-0.0.2/Tele/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20623 2023-05-05 07:58:27.000000 pyTPro-0.0.2/Tele/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6623 2023-05-05 07:58:27.000000 pyTPro-0.0.2/Tele/config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 07:58:38.366040 pyTPro-0.0.2/Tele/database/
+-rw-r--r--   0 runner    (1001) docker     (123)      355 2023-05-05 07:58:27.000000 pyTPro-0.0.2/Tele/database/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5622 2023-05-05 07:58:27.000000 pyTPro-0.0.2/Tele/database/bdbDatabase.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1220 2023-05-05 07:58:27.000000 pyTPro-0.0.2/Tele/database/bubDatabase.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5839 2023-05-05 07:58:27.000000 pyTPro-0.0.2/Tele/database/othDatabase.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1612 2023-05-05 07:58:27.000000 pyTPro-0.0.2/Tele/database/papDatabase.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2838 2023-05-05 07:58:27.000000 pyTPro-0.0.2/Tele/database/pmoDatabase.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-05-05 07:58:27.000000 pyTPro-0.0.2/Tele/database/pobDatabase.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 07:58:38.370040 pyTPro-0.0.2/Tele/decorators/
+-rw-r--r--   0 runner    (1001) docker     (123)      132 2023-05-05 07:58:27.000000 pyTPro-0.0.2/Tele/decorators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6317 2023-05-05 07:58:27.000000 pyTPro-0.0.2/Tele/decorators/forcesub.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3169 2023-05-05 07:58:27.000000 pyTPro-0.0.2/Tele/decorators/oncmd.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1891 2023-05-05 07:58:27.000000 pyTPro-0.0.2/Tele/decorators/task.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 07:58:38.370040 pyTPro-0.0.2/Tele/methods/
+-rw-r--r--   0 runner    (1001) docker     (123)      184 2023-05-05 07:58:27.000000 pyTPro-0.0.2/Tele/methods/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1383 2023-05-05 07:58:27.000000 pyTPro-0.0.2/Tele/methods/content.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8161 2023-05-05 07:58:27.000000 pyTPro-0.0.2/Tele/methods/getfile.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8433 2023-05-05 07:58:27.000000 pyTPro-0.0.2/Tele/methods/message.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9364 2023-05-05 07:58:27.000000 pyTPro-0.0.2/Tele/methods/thumbnail.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 07:58:38.374040 pyTPro-0.0.2/Tele/types/
+-rw-r--r--   0 runner    (1001) docker     (123)      328 2023-05-05 07:58:27.000000 pyTPro-0.0.2/Tele/types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10063 2023-05-05 07:58:27.000000 pyTPro-0.0.2/Tele/types/inline.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3942 2023-05-05 07:58:27.000000 pyTPro-0.0.2/Tele/types/inlineBdb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4279 2023-05-05 07:58:27.000000 pyTPro-0.0.2/Tele/types/inlineBub.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5881 2023-05-05 07:58:27.000000 pyTPro-0.0.2/Tele/types/inlinePob.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3668 2023-05-05 07:58:27.000000 pyTPro-0.0.2/Tele/types/inlineVip.py
+-rw-r--r--   0 runner    (1001) docker     (123)      306 2023-05-05 07:58:27.000000 pyTPro-0.0.2/Tele/types/style.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5255 2023-05-05 07:58:27.000000 pyTPro-0.0.2/Tele/types/text.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 07:58:38.374040 pyTPro-0.0.2/Tele/utilities/
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-05-05 07:58:27.000000 pyTPro-0.0.2/Tele/utilities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      568 2023-05-05 07:58:27.000000 pyTPro-0.0.2/Tele/utilities/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1807 2023-05-05 07:58:27.000000 pyTPro-0.0.2/Tele/utilities/mongo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1368 2023-05-05 07:58:27.000000 pyTPro-0.0.2/Tele/utilities/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 07:58:38.374040 pyTPro-0.0.2/pyTPro.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      932 2023-05-05 07:58:38.000000 pyTPro-0.0.2/pyTPro.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      921 2023-05-05 07:58:38.000000 pyTPro-0.0.2/pyTPro.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 07:58:38.000000 pyTPro-0.0.2/pyTPro.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      202 2023-05-05 07:58:38.000000 pyTPro-0.0.2/pyTPro.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-05-05 07:58:38.000000 pyTPro-0.0.2/pyTPro.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-05 07:58:38.374040 pyTPro-0.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1611 2023-05-05 07:58:27.000000 pyTPro-0.0.2/setup.py
```

### Comparing `pyTPro-0.0.1/PKG-INFO` & `pyTPro-0.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyTPro
-Version: 0.0.1
+Version: 0.0.2
 Summary: Best Code for the Pyrogram Library.
 Home-page: https://github.com/OTHFamily/pyTele
 Author: TPro
 Author-email: 
 License: MIT
 Keywords: telegram pyrogram keyboard bot userbot
 Classifier: Programming Language :: Python
```

### Comparing `pyTPro-0.0.1/Tele/client.py` & `pyTPro-0.0.2/Tele/client.py`

 * *Files identical despite different names*

### Comparing `pyTPro-0.0.1/Tele/config.py` & `pyTPro-0.0.2/Tele/config.py`

 * *Files identical despite different names*

### Comparing `pyTPro-0.0.1/Tele/database/bdbDatabase.py` & `pyTPro-0.0.2/Tele/database/bdbDatabase.py`

 * *Files identical despite different names*

### Comparing `pyTPro-0.0.1/Tele/database/bubDatabase.py` & `pyTPro-0.0.2/Tele/database/bubDatabase.py`

 * *Files identical despite different names*

### Comparing `pyTPro-0.0.1/Tele/database/othDatabase.py` & `pyTPro-0.0.2/Tele/database/othDatabase.py`

 * *Files identical despite different names*

### Comparing `pyTPro-0.0.1/Tele/database/papDatabase.py` & `pyTPro-0.0.2/Tele/database/papDatabase.py`

 * *Files identical despite different names*

### Comparing `pyTPro-0.0.1/Tele/database/pmoDatabase.py` & `pyTPro-0.0.2/Tele/database/pmoDatabase.py`

 * *Files identical despite different names*

### Comparing `pyTPro-0.0.1/Tele/database/pobDatabase.py` & `pyTPro-0.0.2/Tele/database/pobDatabase.py`

 * *Files identical despite different names*

### Comparing `pyTPro-0.0.1/Tele/decorators/forcesub.py` & `pyTPro-0.0.2/Tele/decorators/forcesub.py`

 * *Files identical despite different names*

### Comparing `pyTPro-0.0.1/Tele/decorators/oncmd.py` & `pyTPro-0.0.2/Tele/decorators/oncmd.py`

 * *Files identical despite different names*

### Comparing `pyTPro-0.0.1/Tele/decorators/task.py` & `pyTPro-0.0.2/Tele/decorators/task.py`

 * *Files identical despite different names*

### Comparing `pyTPro-0.0.1/Tele/methods/content.py` & `pyTPro-0.0.2/Tele/methods/content.py`

 * *Files identical despite different names*

### Comparing `pyTPro-0.0.1/Tele/methods/getfile.py` & `pyTPro-0.0.2/Tele/methods/getfile.py`

 * *Files identical despite different names*

### Comparing `pyTPro-0.0.1/Tele/methods/message.py` & `pyTPro-0.0.2/Tele/methods/message.py`

 * *Files identical despite different names*

### Comparing `pyTPro-0.0.1/Tele/methods/thumbnail.py` & `pyTPro-0.0.2/Tele/methods/thumbnail.py`

 * *Files identical despite different names*

### Comparing `pyTPro-0.0.1/Tele/types/inline.py` & `pyTPro-0.0.2/Tele/types/inline.py`

 * *Files identical despite different names*

### Comparing `pyTPro-0.0.1/Tele/types/inlineBdb.py` & `pyTPro-0.0.2/Tele/types/inlineBdb.py`

 * *Files identical despite different names*

### Comparing `pyTPro-0.0.1/Tele/types/inlineBub.py` & `pyTPro-0.0.2/Tele/types/inlineBub.py`

 * *Files identical despite different names*

### Comparing `pyTPro-0.0.1/Tele/types/inlinePob.py` & `pyTPro-0.0.2/Tele/types/inlinePob.py`

 * *Files identical despite different names*

### Comparing `pyTPro-0.0.1/Tele/types/inlineVip.py` & `pyTPro-0.0.2/Tele/types/inlineVip.py`

 * *Files identical despite different names*

### Comparing `pyTPro-0.0.1/Tele/types/text.py` & `pyTPro-0.0.2/Tele/types/text.py`

 * *Files identical despite different names*

### Comparing `pyTPro-0.0.1/Tele/utilities/logger.py` & `pyTPro-0.0.2/Tele/utilities/logger.py`

 * *Files identical despite different names*

### Comparing `pyTPro-0.0.1/Tele/utilities/mongo.py` & `pyTPro-0.0.2/Tele/utilities/mongo.py`

 * *Files identical despite different names*

### Comparing `pyTPro-0.0.1/Tele/utilities/utils.py` & `pyTPro-0.0.2/Tele/utilities/utils.py`

 * *Files identical despite different names*

### Comparing `pyTPro-0.0.1/pyTPro.egg-info/PKG-INFO` & `pyTPro-0.0.2/pyTPro.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyTPro
-Version: 0.0.1
+Version: 0.0.2
 Summary: Best Code for the Pyrogram Library.
 Home-page: https://github.com/OTHFamily/pyTele
 Author: TPro
 Author-email: 
 License: MIT
 Keywords: telegram pyrogram keyboard bot userbot
 Classifier: Programming Language :: Python
```

### Comparing `pyTPro-0.0.1/pyTPro.egg-info/SOURCES.txt` & `pyTPro-0.0.2/pyTPro.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyTPro-0.0.1/setup.py` & `pyTPro-0.0.2/setup.py`

 * *Files identical despite different names*

