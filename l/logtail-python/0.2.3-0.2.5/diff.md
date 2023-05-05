# Comparing `tmp/logtail-python-0.2.3.tar.gz` & `tmp/logtail-python-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "logtail-python-0.2.3.tar", last modified: Thu Mar 30 14:06:47 2023, max compression
+gzip compressed data, was "logtail-python-0.2.5.tar", last modified: Fri May  5 17:19:29 2023, max compression
```

## Comparing `logtail-python-0.2.3.tar` & `logtail-python-0.2.5.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-03-30 14:06:47.276946 logtail-python-0.2.3/
--rw-r--r--   0 simon      (501) staff       (20)      737 2023-02-17 20:58:53.000000 logtail-python-0.2.3/LICENSE.md
--rw-r--r--   0 simon      (501) staff       (20)      115 2023-02-17 20:58:53.000000 logtail-python-0.2.3/MANIFEST.in
--rw-r--r--   0 simon      (501) staff       (20)     2107 2023-03-30 14:06:47.276994 logtail-python-0.2.3/PKG-INFO
--rw-r--r--   0 simon      (501) staff       (20)     1065 2023-03-30 09:34:01.000000 logtail-python-0.2.3/README.md
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-03-30 14:06:47.273371 logtail-python-0.2.3/logtail/
--rw-r--r--   0 simon      (501) staff       (20)      252 2023-02-17 20:58:53.000000 logtail-python-0.2.3/logtail/__init__.py
--rw-r--r--   0 simon      (501) staff       (20)      141 2023-02-17 20:58:53.000000 logtail-python-0.2.3/logtail/compat.py
--rw-r--r--   0 simon      (501) staff       (20)     2999 2023-03-30 14:00:59.000000 logtail-python-0.2.3/logtail/flusher.py
--rw-r--r--   0 simon      (501) staff       (20)      968 2023-02-17 20:58:53.000000 logtail-python-0.2.3/logtail/formatter.py
--rw-r--r--   0 simon      (501) staff       (20)     2642 2023-03-30 14:00:59.000000 logtail-python-0.2.3/logtail/frame.py
--rw-r--r--   0 simon      (501) staff       (20)     2617 2023-03-30 09:09:04.000000 logtail-python-0.2.3/logtail/handler.py
--rw-r--r--   0 simon      (501) staff       (20)     1156 2023-02-17 20:58:53.000000 logtail-python-0.2.3/logtail/helpers.py
--rw-r--r--   0 simon      (501) staff       (20)      588 2023-03-30 09:24:28.000000 logtail-python-0.2.3/logtail/uploader.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-03-30 14:06:47.274082 logtail-python-0.2.3/logtail_python.egg-info/
--rw-r--r--   0 simon      (501) staff       (20)     2107 2023-03-30 14:06:47.000000 logtail-python-0.2.3/logtail_python.egg-info/PKG-INFO
--rw-r--r--   0 simon      (501) staff       (20)      909 2023-03-30 14:06:47.000000 logtail-python-0.2.3/logtail_python.egg-info/SOURCES.txt
--rw-r--r--   0 simon      (501) staff       (20)        1 2023-03-30 14:06:47.000000 logtail-python-0.2.3/logtail_python.egg-info/dependency_links.txt
--rw-r--r--   0 simon      (501) staff       (20)       32 2023-03-30 14:06:47.000000 logtail-python-0.2.3/logtail_python.egg-info/requires.txt
--rw-r--r--   0 simon      (501) staff       (20)        8 2023-03-30 14:06:47.000000 logtail-python-0.2.3/logtail_python.egg-info/top_level.txt
--rw-r--r--   0 simon      (501) staff       (20)       32 2023-02-17 20:58:53.000000 logtail-python-0.2.3/requirements.txt
--rw-r--r--   0 simon      (501) staff       (20)       67 2023-03-30 14:06:47.277160 logtail-python-0.2.3/setup.cfg
--rw-r--r--   0 simon      (501) staff       (20)     1551 2023-03-30 14:06:02.000000 logtail-python-0.2.3/setup.py
--rw-r--r--   0 simon      (501) staff       (20)       54 2023-03-30 14:00:59.000000 logtail-python-0.2.3/test-requirements.txt
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-03-30 14:06:47.274884 logtail-python-0.2.3/tests/
--rw-r--r--   0 simon      (501) staff       (20)        0 2023-02-17 20:58:53.000000 logtail-python-0.2.3/tests/__init__.py
-drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-03-30 14:06:47.276818 logtail-python-0.2.3/tests/__pycache__/
--rw-r--r--   0 simon      (501) staff       (20)      158 2023-02-19 13:17:27.000000 logtail-python-0.2.3/tests/__pycache__/__init__.cpython-311.pyc
--rw-r--r--   0 simon      (501) staff       (20)    10312 2023-03-30 12:30:52.000000 logtail-python-0.2.3/tests/__pycache__/test_flusher.cpython-311.pyc
--rw-r--r--   0 simon      (501) staff       (20)    11774 2023-03-30 12:30:52.000000 logtail-python-0.2.3/tests/__pycache__/test_formatter.cpython-311.pyc
--rw-r--r--   0 simon      (501) staff       (20)     3465 2023-03-30 12:30:52.000000 logtail-python-0.2.3/tests/__pycache__/test_frame.cpython-311.pyc
--rw-r--r--   0 simon      (501) staff       (20)     8319 2023-03-30 12:30:52.000000 logtail-python-0.2.3/tests/__pycache__/test_handler.cpython-311.pyc
--rw-r--r--   0 simon      (501) staff       (20)     4559 2023-03-30 12:30:52.000000 logtail-python-0.2.3/tests/__pycache__/test_helpers.cpython-311.pyc
--rw-r--r--   0 simon      (501) staff       (20)     2147 2023-03-30 12:30:52.000000 logtail-python-0.2.3/tests/__pycache__/test_uploader.cpython-311.pyc
--rw-r--r--   0 simon      (501) staff       (20)     5061 2023-03-30 14:00:59.000000 logtail-python-0.2.3/tests/test_flusher.py
--rw-r--r--   0 simon      (501) staff       (20)     5318 2023-03-30 14:00:59.000000 logtail-python-0.2.3/tests/test_formatter.py
--rw-r--r--   0 simon      (501) staff       (20)     1953 2023-03-30 14:00:59.000000 logtail-python-0.2.3/tests/test_frame.py
--rw-r--r--   0 simon      (501) staff       (20)     4565 2023-03-30 14:00:59.000000 logtail-python-0.2.3/tests/test_handler.py
--rw-r--r--   0 simon      (501) staff       (20)     1844 2023-03-30 14:00:59.000000 logtail-python-0.2.3/tests/test_helpers.py
--rw-r--r--   0 simon      (501) staff       (20)     1057 2023-03-30 14:00:59.000000 logtail-python-0.2.3/tests/test_uploader.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-05 17:19:29.126438 logtail-python-0.2.5/
+-rw-r--r--   0 simon      (501) staff       (20)      737 2023-02-17 20:58:53.000000 logtail-python-0.2.5/LICENSE.md
+-rw-r--r--   0 simon      (501) staff       (20)      115 2023-02-17 20:58:53.000000 logtail-python-0.2.5/MANIFEST.in
+-rw-r--r--   0 simon      (501) staff       (20)     2107 2023-05-05 17:19:29.126499 logtail-python-0.2.5/PKG-INFO
+-rw-r--r--   0 simon      (501) staff       (20)     1065 2023-03-30 09:34:01.000000 logtail-python-0.2.5/README.md
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-05 17:19:29.124220 logtail-python-0.2.5/logtail/
+-rw-r--r--   0 simon      (501) staff       (20)      252 2023-05-05 17:09:07.000000 logtail-python-0.2.5/logtail/__init__.py
+-rw-r--r--   0 simon      (501) staff       (20)      141 2023-02-17 20:58:53.000000 logtail-python-0.2.5/logtail/compat.py
+-rw-r--r--   0 simon      (501) staff       (20)     2999 2023-03-30 14:07:44.000000 logtail-python-0.2.5/logtail/flusher.py
+-rw-r--r--   0 simon      (501) staff       (20)      968 2023-02-17 20:58:53.000000 logtail-python-0.2.5/logtail/formatter.py
+-rw-r--r--   0 simon      (501) staff       (20)     2497 2023-05-05 17:05:57.000000 logtail-python-0.2.5/logtail/frame.py
+-rw-r--r--   0 simon      (501) staff       (20)     2617 2023-03-30 09:09:04.000000 logtail-python-0.2.5/logtail/handler.py
+-rw-r--r--   0 simon      (501) staff       (20)     1156 2023-02-17 20:58:53.000000 logtail-python-0.2.5/logtail/helpers.py
+-rw-r--r--   0 simon      (501) staff       (20)      588 2023-03-30 09:24:28.000000 logtail-python-0.2.5/logtail/uploader.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-05 17:19:29.124738 logtail-python-0.2.5/logtail_python.egg-info/
+-rw-r--r--   0 simon      (501) staff       (20)     2107 2023-05-05 17:19:29.000000 logtail-python-0.2.5/logtail_python.egg-info/PKG-INFO
+-rw-r--r--   0 simon      (501) staff       (20)      909 2023-05-05 17:19:29.000000 logtail-python-0.2.5/logtail_python.egg-info/SOURCES.txt
+-rw-r--r--   0 simon      (501) staff       (20)        1 2023-05-05 17:19:29.000000 logtail-python-0.2.5/logtail_python.egg-info/dependency_links.txt
+-rw-r--r--   0 simon      (501) staff       (20)       32 2023-05-05 17:19:29.000000 logtail-python-0.2.5/logtail_python.egg-info/requires.txt
+-rw-r--r--   0 simon      (501) staff       (20)        8 2023-05-05 17:19:29.000000 logtail-python-0.2.5/logtail_python.egg-info/top_level.txt
+-rw-r--r--   0 simon      (501) staff       (20)       32 2023-02-17 20:58:53.000000 logtail-python-0.2.5/requirements.txt
+-rw-r--r--   0 simon      (501) staff       (20)       67 2023-05-05 17:19:29.126717 logtail-python-0.2.5/setup.cfg
+-rw-r--r--   0 simon      (501) staff       (20)     1551 2023-05-05 17:06:09.000000 logtail-python-0.2.5/setup.py
+-rw-r--r--   0 simon      (501) staff       (20)       54 2023-03-30 14:07:44.000000 logtail-python-0.2.5/test-requirements.txt
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-05 17:19:29.125531 logtail-python-0.2.5/tests/
+-rw-r--r--   0 simon      (501) staff       (20)        0 2023-02-17 20:58:53.000000 logtail-python-0.2.5/tests/__init__.py
+drwxr-xr-x   0 simon      (501) staff       (20)        0 2023-05-05 17:19:29.126329 logtail-python-0.2.5/tests/__pycache__/
+-rw-r--r--   0 simon      (501) staff       (20)      158 2023-02-19 13:17:27.000000 logtail-python-0.2.5/tests/__pycache__/__init__.cpython-311.pyc
+-rw-r--r--   0 simon      (501) staff       (20)    10312 2023-03-30 12:30:52.000000 logtail-python-0.2.5/tests/__pycache__/test_flusher.cpython-311.pyc
+-rw-r--r--   0 simon      (501) staff       (20)    11774 2023-03-30 12:30:52.000000 logtail-python-0.2.5/tests/__pycache__/test_formatter.cpython-311.pyc
+-rw-r--r--   0 simon      (501) staff       (20)     3465 2023-03-30 12:30:52.000000 logtail-python-0.2.5/tests/__pycache__/test_frame.cpython-311.pyc
+-rw-r--r--   0 simon      (501) staff       (20)     8319 2023-03-30 12:30:52.000000 logtail-python-0.2.5/tests/__pycache__/test_handler.cpython-311.pyc
+-rw-r--r--   0 simon      (501) staff       (20)     4559 2023-03-30 12:30:52.000000 logtail-python-0.2.5/tests/__pycache__/test_helpers.cpython-311.pyc
+-rw-r--r--   0 simon      (501) staff       (20)     2147 2023-03-30 12:30:52.000000 logtail-python-0.2.5/tests/__pycache__/test_uploader.cpython-311.pyc
+-rw-r--r--   0 simon      (501) staff       (20)     5061 2023-03-30 14:07:44.000000 logtail-python-0.2.5/tests/test_flusher.py
+-rw-r--r--   0 simon      (501) staff       (20)     5318 2023-03-30 14:07:44.000000 logtail-python-0.2.5/tests/test_formatter.py
+-rw-r--r--   0 simon      (501) staff       (20)     1953 2023-03-30 14:07:44.000000 logtail-python-0.2.5/tests/test_frame.py
+-rw-r--r--   0 simon      (501) staff       (20)     4565 2023-03-30 14:07:44.000000 logtail-python-0.2.5/tests/test_handler.py
+-rw-r--r--   0 simon      (501) staff       (20)     1844 2023-03-30 14:07:44.000000 logtail-python-0.2.5/tests/test_helpers.py
+-rw-r--r--   0 simon      (501) staff       (20)     1057 2023-03-30 14:07:44.000000 logtail-python-0.2.5/tests/test_uploader.py
```

### Comparing `logtail-python-0.2.3/LICENSE.md` & `logtail-python-0.2.5/LICENSE.md`

 * *Files identical despite different names*

### Comparing `logtail-python-0.2.3/PKG-INFO` & `logtail-python-0.2.5/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: logtail-python
-Version: 0.2.3
+Version: 0.2.5
 Summary: Logtail.com client library
 Home-page: https://github.com/logtail/logtail-python
-Download-URL: https://github.com/logtail/logtail-python/tarball/0.2.3
+Download-URL: https://github.com/logtail/logtail-python/tarball/0.2.5
 Author: Logtail
 Author-email: hello@logtail.com
 License: ISC
 Keywords: api,logtail,logging,client
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: ISC License (ISCL)
 Classifier: Operating System :: OS Independent
```

### Comparing `logtail-python-0.2.3/README.md` & `logtail-python-0.2.5/README.md`

 * *Files identical despite different names*

### Comparing `logtail-python-0.2.3/logtail/flusher.py` & `logtail-python-0.2.5/logtail/flusher.py`

 * *Files identical despite different names*

### Comparing `logtail-python-0.2.3/logtail/formatter.py` & `logtail-python-0.2.5/logtail/formatter.py`

 * *Files identical despite different names*

### Comparing `logtail-python-0.2.3/logtail/frame.py` & `logtail-python-0.2.5/logtail/frame.py`

 * *Files 6% similar despite different names*

```diff
@@ -58,22 +58,15 @@
         if not include_extra_attributes and not isinstance(val, dict):
             continue
         events[key] = val
     return events
 
 
 def _levelname(level):
-    return {
-        'debug': 'debug',
-        'info': 'info',
-        'warning': 'warn',
-        'error': 'error',
-        'critical': 'critical',
-    }[level.lower()]
-
+    return level.lower()
 
 def _relative_to_main_module_if_possible(pathname):
     has_main_module = hasattr(__main__, '__file__')
     return _relative_to_main_module(pathname) if has_main_module else pathname
 
 def _relative_to_main_module(pathname):
     return path.relpath(pathname, path.dirname(__main__.__file__))
```

### Comparing `logtail-python-0.2.3/logtail/handler.py` & `logtail-python-0.2.5/logtail/handler.py`

 * *Files identical despite different names*

### Comparing `logtail-python-0.2.3/logtail/helpers.py` & `logtail-python-0.2.5/logtail/helpers.py`

 * *Files identical despite different names*

### Comparing `logtail-python-0.2.3/logtail/uploader.py` & `logtail-python-0.2.5/logtail/uploader.py`

 * *Files identical despite different names*

### Comparing `logtail-python-0.2.3/logtail_python.egg-info/PKG-INFO` & `logtail-python-0.2.5/logtail_python.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: logtail-python
-Version: 0.2.3
+Version: 0.2.5
 Summary: Logtail.com client library
 Home-page: https://github.com/logtail/logtail-python
-Download-URL: https://github.com/logtail/logtail-python/tarball/0.2.3
+Download-URL: https://github.com/logtail/logtail-python/tarball/0.2.5
 Author: Logtail
 Author-email: hello@logtail.com
 License: ISC
 Keywords: api,logtail,logging,client
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: ISC License (ISCL)
 Classifier: Operating System :: OS Independent
```

### Comparing `logtail-python-0.2.3/logtail_python.egg-info/SOURCES.txt` & `logtail-python-0.2.5/logtail_python.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `logtail-python-0.2.3/setup.py` & `logtail-python-0.2.5/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # coding: utf-8
 import os
 from setuptools import setup
 
 
-VERSION = '0.2.3'
+VERSION = '0.2.5'
 ROOT_DIR = os.path.dirname(__file__)
 
 REQUIREMENTS = [
     line.strip() for line in
     open(os.path.join(ROOT_DIR, 'requirements.txt')).readlines()
 ]
```

### Comparing `logtail-python-0.2.3/tests/__pycache__/test_flusher.cpython-311.pyc` & `logtail-python-0.2.5/tests/__pycache__/test_flusher.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `logtail-python-0.2.3/tests/__pycache__/test_formatter.cpython-311.pyc` & `logtail-python-0.2.5/tests/__pycache__/test_formatter.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `logtail-python-0.2.3/tests/__pycache__/test_frame.cpython-311.pyc` & `logtail-python-0.2.5/tests/__pycache__/test_frame.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `logtail-python-0.2.3/tests/__pycache__/test_handler.cpython-311.pyc` & `logtail-python-0.2.5/tests/__pycache__/test_handler.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `logtail-python-0.2.3/tests/__pycache__/test_helpers.cpython-311.pyc` & `logtail-python-0.2.5/tests/__pycache__/test_helpers.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `logtail-python-0.2.3/tests/__pycache__/test_uploader.cpython-311.pyc` & `logtail-python-0.2.5/tests/__pycache__/test_uploader.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `logtail-python-0.2.3/tests/test_flusher.py` & `logtail-python-0.2.5/tests/test_flusher.py`

 * *Files identical despite different names*

### Comparing `logtail-python-0.2.3/tests/test_formatter.py` & `logtail-python-0.2.5/tests/test_formatter.py`

 * *Files identical despite different names*

### Comparing `logtail-python-0.2.3/tests/test_frame.py` & `logtail-python-0.2.5/tests/test_frame.py`

 * *Files identical despite different names*

### Comparing `logtail-python-0.2.3/tests/test_handler.py` & `logtail-python-0.2.5/tests/test_handler.py`

 * *Files identical despite different names*

### Comparing `logtail-python-0.2.3/tests/test_helpers.py` & `logtail-python-0.2.5/tests/test_helpers.py`

 * *Files identical despite different names*

### Comparing `logtail-python-0.2.3/tests/test_uploader.py` & `logtail-python-0.2.5/tests/test_uploader.py`

 * *Files identical despite different names*

