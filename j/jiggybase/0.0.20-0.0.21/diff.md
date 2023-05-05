# Comparing `tmp/jiggybase-0.0.20.tar.gz` & `tmp/jiggybase-0.0.21.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jiggybase-0.0.20.tar", last modified: Thu May  4 23:57:52 2023, max compression
+gzip compressed data, was "jiggybase-0.0.21.tar", last modified: Fri May  5 00:02:58 2023, max compression
```

## Comparing `jiggybase-0.0.20.tar` & `jiggybase-0.0.21.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxr-xr-x   0 wsk        (501) staff       (20)        0 2023-05-04 23:57:52.925708 jiggybase-0.0.20/
--rw-r--r--   0 wsk        (501) staff       (20)    11357 2023-04-10 04:07:02.000000 jiggybase-0.0.20/LICENSE
--rw-r--r--   0 wsk        (501) staff       (20)     5826 2023-05-04 23:57:52.925295 jiggybase-0.0.20/PKG-INFO
--rw-r--r--   0 wsk        (501) staff       (20)     5292 2023-05-01 15:45:10.000000 jiggybase-0.0.20/README.md
-drwxr-xr-x   0 wsk        (501) staff       (20)        0 2023-05-04 23:57:52.918666 jiggybase-0.0.20/jiggybase/
--rw-r--r--   0 wsk        (501) staff       (20)       30 2023-04-28 15:28:30.000000 jiggybase-0.0.20/jiggybase/__init__.py
--rw-r--r--   0 wsk        (501) staff       (20)     2044 2023-05-01 01:40:42.000000 jiggybase-0.0.20/jiggybase/client.py
--rw-r--r--   0 wsk        (501) staff       (20)     8508 2023-04-30 00:50:55.000000 jiggybase-0.0.20/jiggybase/collection.py
--rw-r--r--   0 wsk        (501) staff       (20)     4531 2023-04-29 04:12:14.000000 jiggybase-0.0.20/jiggybase/jiggybase_session.py
--rw-r--r--   0 wsk        (501) staff       (20)     1187 2023-03-30 18:09:13.000000 jiggybase-0.0.20/jiggybase/login.py
-drwxr-xr-x   0 wsk        (501) staff       (20)        0 2023-05-04 23:57:52.924250 jiggybase-0.0.20/jiggybase/models/
--rw-r--r--   0 wsk        (501) staff       (20)      273 2023-04-26 01:37:49.000000 jiggybase-0.0.20/jiggybase/models/__init__.py
--rw-r--r--   0 wsk        (501) staff       (20)     1236 2023-04-10 05:17:32.000000 jiggybase-0.0.20/jiggybase/models/auth.py
--rw-r--r--   0 wsk        (501) staff       (20)     1007 2023-04-23 16:10:39.000000 jiggybase-0.0.20/jiggybase/models/chat.py
--rw-r--r--   0 wsk        (501) staff       (20)      188 2023-04-23 04:17:06.000000 jiggybase-0.0.20/jiggybase/models/chatmodel.py
--rw-r--r--   0 wsk        (501) staff       (20)     1322 2023-04-10 16:54:34.000000 jiggybase-0.0.20/jiggybase/models/chunk.py
--rw-r--r--   0 wsk        (501) staff       (20)     4240 2023-04-20 21:45:37.000000 jiggybase-0.0.20/jiggybase/models/collection.py
--rw-r--r--   0 wsk        (501) staff       (20)      454 2023-04-23 05:06:00.000000 jiggybase-0.0.20/jiggybase/models/embedding.py
--rw-r--r--   0 wsk        (501) staff       (20)      696 2023-04-10 04:48:20.000000 jiggybase-0.0.20/jiggybase/models/metadata.py
--rw-r--r--   0 wsk        (501) staff       (20)     2214 2023-04-10 04:58:39.000000 jiggybase-0.0.20/jiggybase/models/org.py
--rw-r--r--   0 wsk        (501) staff       (20)     2777 2023-04-29 00:07:44.000000 jiggybase-0.0.20/jiggybase/models/plugin.py
--rw-r--r--   0 wsk        (501) staff       (20)     3415 2023-05-04 23:56:42.000000 jiggybase-0.0.20/jiggybase/models/plugin_config.py
--rw-r--r--   0 wsk        (501) staff       (20)     2834 2023-04-22 23:44:02.000000 jiggybase-0.0.20/jiggybase/models/prompt.py
--rw-r--r--   0 wsk        (501) staff       (20)     3012 2023-04-11 17:29:49.000000 jiggybase-0.0.20/jiggybase/models/providers.py
--rw-r--r--   0 wsk        (501) staff       (20)     1820 2023-04-17 16:14:19.000000 jiggybase-0.0.20/jiggybase/models/user.py
--rw-r--r--   0 wsk        (501) staff       (20)     4600 2023-04-29 15:22:54.000000 jiggybase-0.0.20/jiggybase/org.py
-drwxr-xr-x   0 wsk        (501) staff       (20)        0 2023-05-04 23:57:52.920036 jiggybase-0.0.20/jiggybase.egg-info/
--rw-r--r--   0 wsk        (501) staff       (20)     5826 2023-05-04 23:57:52.000000 jiggybase-0.0.20/jiggybase.egg-info/PKG-INFO
--rw-r--r--   0 wsk        (501) staff       (20)      734 2023-05-04 23:57:52.000000 jiggybase-0.0.20/jiggybase.egg-info/SOURCES.txt
--rw-r--r--   0 wsk        (501) staff       (20)        1 2023-05-04 23:57:52.000000 jiggybase-0.0.20/jiggybase.egg-info/dependency_links.txt
--rw-r--r--   0 wsk        (501) staff       (20)       32 2023-05-04 23:57:52.000000 jiggybase-0.0.20/jiggybase.egg-info/requires.txt
--rw-r--r--   0 wsk        (501) staff       (20)       10 2023-05-04 23:57:52.000000 jiggybase-0.0.20/jiggybase.egg-info/top_level.txt
--rw-r--r--   0 wsk        (501) staff       (20)      669 2023-05-04 23:56:48.000000 jiggybase-0.0.20/pyproject.toml
--rw-r--r--   0 wsk        (501) staff       (20)       38 2023-05-04 23:57:52.925817 jiggybase-0.0.20/setup.cfg
-drwxr-xr-x   0 wsk        (501) staff       (20)        0 2023-05-04 23:57:52.924742 jiggybase-0.0.20/test/
--rw-r--r--   0 wsk        (501) staff       (20)      830 2023-04-28 15:38:35.000000 jiggybase-0.0.20/test/test.py
+drwxr-xr-x   0 wsk        (501) staff       (20)        0 2023-05-05 00:02:58.657431 jiggybase-0.0.21/
+-rw-r--r--   0 wsk        (501) staff       (20)    11357 2023-04-10 04:07:02.000000 jiggybase-0.0.21/LICENSE
+-rw-r--r--   0 wsk        (501) staff       (20)     5826 2023-05-05 00:02:58.657156 jiggybase-0.0.21/PKG-INFO
+-rw-r--r--   0 wsk        (501) staff       (20)     5292 2023-05-01 15:45:10.000000 jiggybase-0.0.21/README.md
+drwxr-xr-x   0 wsk        (501) staff       (20)        0 2023-05-05 00:02:58.651579 jiggybase-0.0.21/jiggybase/
+-rw-r--r--   0 wsk        (501) staff       (20)       30 2023-04-28 15:28:30.000000 jiggybase-0.0.21/jiggybase/__init__.py
+-rw-r--r--   0 wsk        (501) staff       (20)     2044 2023-05-01 01:40:42.000000 jiggybase-0.0.21/jiggybase/client.py
+-rw-r--r--   0 wsk        (501) staff       (20)     8508 2023-04-30 00:50:55.000000 jiggybase-0.0.21/jiggybase/collection.py
+-rw-r--r--   0 wsk        (501) staff       (20)     4531 2023-04-29 04:12:14.000000 jiggybase-0.0.21/jiggybase/jiggybase_session.py
+-rw-r--r--   0 wsk        (501) staff       (20)     1187 2023-03-30 18:09:13.000000 jiggybase-0.0.21/jiggybase/login.py
+drwxr-xr-x   0 wsk        (501) staff       (20)        0 2023-05-05 00:02:58.656573 jiggybase-0.0.21/jiggybase/models/
+-rw-r--r--   0 wsk        (501) staff       (20)      273 2023-04-26 01:37:49.000000 jiggybase-0.0.21/jiggybase/models/__init__.py
+-rw-r--r--   0 wsk        (501) staff       (20)     1236 2023-04-10 05:17:32.000000 jiggybase-0.0.21/jiggybase/models/auth.py
+-rw-r--r--   0 wsk        (501) staff       (20)     1007 2023-04-23 16:10:39.000000 jiggybase-0.0.21/jiggybase/models/chat.py
+-rw-r--r--   0 wsk        (501) staff       (20)      188 2023-04-23 04:17:06.000000 jiggybase-0.0.21/jiggybase/models/chatmodel.py
+-rw-r--r--   0 wsk        (501) staff       (20)     1322 2023-04-10 16:54:34.000000 jiggybase-0.0.21/jiggybase/models/chunk.py
+-rw-r--r--   0 wsk        (501) staff       (20)     4240 2023-04-20 21:45:37.000000 jiggybase-0.0.21/jiggybase/models/collection.py
+-rw-r--r--   0 wsk        (501) staff       (20)      454 2023-04-23 05:06:00.000000 jiggybase-0.0.21/jiggybase/models/embedding.py
+-rw-r--r--   0 wsk        (501) staff       (20)      696 2023-04-10 04:48:20.000000 jiggybase-0.0.21/jiggybase/models/metadata.py
+-rw-r--r--   0 wsk        (501) staff       (20)     2214 2023-04-10 04:58:39.000000 jiggybase-0.0.21/jiggybase/models/org.py
+-rw-r--r--   0 wsk        (501) staff       (20)     2777 2023-04-29 00:07:44.000000 jiggybase-0.0.21/jiggybase/models/plugin.py
+-rw-r--r--   0 wsk        (501) staff       (20)     3415 2023-05-04 23:56:42.000000 jiggybase-0.0.21/jiggybase/models/plugin_config.py
+-rw-r--r--   0 wsk        (501) staff       (20)     2834 2023-04-22 23:44:02.000000 jiggybase-0.0.21/jiggybase/models/prompt.py
+-rw-r--r--   0 wsk        (501) staff       (20)     3012 2023-04-11 17:29:49.000000 jiggybase-0.0.21/jiggybase/models/providers.py
+-rw-r--r--   0 wsk        (501) staff       (20)     1820 2023-04-17 16:14:19.000000 jiggybase-0.0.21/jiggybase/models/user.py
+-rw-r--r--   0 wsk        (501) staff       (20)     4600 2023-04-29 15:22:54.000000 jiggybase-0.0.21/jiggybase/org.py
+drwxr-xr-x   0 wsk        (501) staff       (20)        0 2023-05-05 00:02:58.652944 jiggybase-0.0.21/jiggybase.egg-info/
+-rw-r--r--   0 wsk        (501) staff       (20)     5826 2023-05-05 00:02:58.000000 jiggybase-0.0.21/jiggybase.egg-info/PKG-INFO
+-rw-r--r--   0 wsk        (501) staff       (20)      734 2023-05-05 00:02:58.000000 jiggybase-0.0.21/jiggybase.egg-info/SOURCES.txt
+-rw-r--r--   0 wsk        (501) staff       (20)        1 2023-05-05 00:02:58.000000 jiggybase-0.0.21/jiggybase.egg-info/dependency_links.txt
+-rw-r--r--   0 wsk        (501) staff       (20)       32 2023-05-05 00:02:58.000000 jiggybase-0.0.21/jiggybase.egg-info/requires.txt
+-rw-r--r--   0 wsk        (501) staff       (20)       10 2023-05-05 00:02:58.000000 jiggybase-0.0.21/jiggybase.egg-info/top_level.txt
+-rw-r--r--   0 wsk        (501) staff       (20)      669 2023-05-05 00:02:26.000000 jiggybase-0.0.21/pyproject.toml
+-rw-r--r--   0 wsk        (501) staff       (20)       38 2023-05-05 00:02:58.657506 jiggybase-0.0.21/setup.cfg
+drwxr-xr-x   0 wsk        (501) staff       (20)        0 2023-05-05 00:02:58.656824 jiggybase-0.0.21/test/
+-rw-r--r--   0 wsk        (501) staff       (20)      830 2023-04-28 15:38:35.000000 jiggybase-0.0.21/test/test.py
```

### Comparing `jiggybase-0.0.20/LICENSE` & `jiggybase-0.0.21/LICENSE`

 * *Files identical despite different names*

### Comparing `jiggybase-0.0.20/PKG-INFO` & `jiggybase-0.0.21/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jiggybase
-Version: 0.0.20
+Version: 0.0.21
 Summary: Client for Jiggy AI JiggyBase, including ChatGPT Retriever Plugins
 Author-email: Bill Kish <bk@jiggy.ai>
 Project-URL: Homepage, https://github.com/jiggy-ai/jiggybase
 Project-URL: Bug Tracker, https://github.com/jiggy-ai/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

### Comparing `jiggybase-0.0.20/README.md` & `jiggybase-0.0.21/README.md`

 * *Files identical despite different names*

### Comparing `jiggybase-0.0.20/jiggybase/client.py` & `jiggybase-0.0.21/jiggybase/client.py`

 * *Files identical despite different names*

### Comparing `jiggybase-0.0.20/jiggybase/collection.py` & `jiggybase-0.0.21/jiggybase/collection.py`

 * *Files identical despite different names*

### Comparing `jiggybase-0.0.20/jiggybase/jiggybase_session.py` & `jiggybase-0.0.21/jiggybase/jiggybase_session.py`

 * *Files identical despite different names*

### Comparing `jiggybase-0.0.20/jiggybase/login.py` & `jiggybase-0.0.21/jiggybase/login.py`

 * *Files identical despite different names*

### Comparing `jiggybase-0.0.20/jiggybase/models/auth.py` & `jiggybase-0.0.21/jiggybase/models/auth.py`

 * *Files identical despite different names*

### Comparing `jiggybase-0.0.20/jiggybase/models/chat.py` & `jiggybase-0.0.21/jiggybase/models/chat.py`

 * *Files identical despite different names*

### Comparing `jiggybase-0.0.20/jiggybase/models/chunk.py` & `jiggybase-0.0.21/jiggybase/models/chunk.py`

 * *Files identical despite different names*

### Comparing `jiggybase-0.0.20/jiggybase/models/collection.py` & `jiggybase-0.0.21/jiggybase/models/collection.py`

 * *Files identical despite different names*

### Comparing `jiggybase-0.0.20/jiggybase/models/metadata.py` & `jiggybase-0.0.21/jiggybase/models/metadata.py`

 * *Files identical despite different names*

### Comparing `jiggybase-0.0.20/jiggybase/models/org.py` & `jiggybase-0.0.21/jiggybase/models/org.py`

 * *Files identical despite different names*

### Comparing `jiggybase-0.0.20/jiggybase/models/plugin.py` & `jiggybase-0.0.21/jiggybase/models/plugin.py`

 * *Files identical despite different names*

### Comparing `jiggybase-0.0.20/jiggybase/models/plugin_config.py` & `jiggybase-0.0.21/jiggybase/models/plugin_config.py`

 * *Files identical despite different names*

### Comparing `jiggybase-0.0.20/jiggybase/models/prompt.py` & `jiggybase-0.0.21/jiggybase/models/prompt.py`

 * *Files identical despite different names*

### Comparing `jiggybase-0.0.20/jiggybase/models/providers.py` & `jiggybase-0.0.21/jiggybase/models/providers.py`

 * *Files identical despite different names*

### Comparing `jiggybase-0.0.20/jiggybase/models/user.py` & `jiggybase-0.0.21/jiggybase/models/user.py`

 * *Files identical despite different names*

### Comparing `jiggybase-0.0.20/jiggybase/org.py` & `jiggybase-0.0.21/jiggybase/org.py`

 * *Files identical despite different names*

### Comparing `jiggybase-0.0.20/jiggybase.egg-info/PKG-INFO` & `jiggybase-0.0.21/jiggybase.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jiggybase
-Version: 0.0.20
+Version: 0.0.21
 Summary: Client for Jiggy AI JiggyBase, including ChatGPT Retriever Plugins
 Author-email: Bill Kish <bk@jiggy.ai>
 Project-URL: Homepage, https://github.com/jiggy-ai/jiggybase
 Project-URL: Bug Tracker, https://github.com/jiggy-ai/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

### Comparing `jiggybase-0.0.20/jiggybase.egg-info/SOURCES.txt` & `jiggybase-0.0.21/jiggybase.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `jiggybase-0.0.20/pyproject.toml` & `jiggybase-0.0.21/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "jiggybase"
-version = "0.0.20"
+version = "0.0.21"
 authors = [
   { name="Bill Kish", email="bk@jiggy.ai" },
 ]
-dependencies=['loguru', 'pedantic[email]', 'requests']
+dependencies=['loguru', 'pydantic[email]', 'requests']
 description = "Client for Jiggy AI JiggyBase, including ChatGPT Retriever Plugins"
 readme = "README.md"
 requires-python = ">=3.9"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: Apache Software License",
     "Operating System :: OS Independent",
```

### Comparing `jiggybase-0.0.20/test/test.py` & `jiggybase-0.0.21/test/test.py`

 * *Files identical despite different names*

