# Comparing `tmp/backend.ai-test-23.3.1.tar.gz` & `tmp/backend.ai-test-23.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "backend.ai-test-23.3.1.tar", last modified: Thu May  4 05:10:09 2023, max compression
+gzip compressed data, was "backend.ai-test-23.3.2.tar", last modified: Fri May  5 07:08:12 2023, max compression
```

## Comparing `backend.ai-test-23.3.1.tar` & `backend.ai-test-23.3.2.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 05:10:09.758785 backend.ai-test-23.3.1/
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-04 05:10:09.000000 backend.ai-test-23.3.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1304 2023-05-04 05:10:09.758785 backend.ai-test-23.3.1/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 05:10:09.758785 backend.ai-test-23.3.1/ai/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 05:10:09.758785 backend.ai-test-23.3.1/ai/backend/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 05:10:09.758785 backend.ai-test-23.3.1/ai/backend/test/
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-04 05:10:09.000000 backend.ai-test-23.3.1/ai/backend/test/VERSION
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-04 05:10:09.000000 backend.ai-test-23.3.1/ai/backend/test/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 05:10:09.758785 backend.ai-test-23.3.1/ai/backend/test/cli/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 05:10:09.000000 backend.ai-test-23.3.1/ai/backend/test/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1607 2023-05-04 05:10:09.000000 backend.ai-test-23.3.1/ai/backend/test/cli/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)       88 2023-05-04 05:10:09.000000 backend.ai-test-23.3.1/ai/backend/test/cli/context.py
--rw-r--r--   0 runner    (1001) docker     (123)      848 2023-05-04 05:10:09.000000 backend.ai-test-23.3.1/ai/backend/test/cli/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-04 05:10:09.000000 backend.ai-test-23.3.1/ai/backend/test/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 05:10:09.758785 backend.ai-test-23.3.1/backend.ai_test.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1304 2023-05-04 05:10:09.000000 backend.ai-test-23.3.1/backend.ai_test.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      559 2023-05-04 05:10:09.000000 backend.ai-test-23.3.1/backend.ai_test.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-04 05:10:09.000000 backend.ai-test-23.3.1/backend.ai_test.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-05-04 05:10:09.000000 backend.ai-test-23.3.1/backend.ai_test.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-04 05:10:09.000000 backend.ai-test-23.3.1/backend.ai_test.egg-info/namespace_packages.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-04 05:10:09.000000 backend.ai-test-23.3.1/backend.ai_test.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-05-04 05:10:09.000000 backend.ai-test-23.3.1/backend.ai_test.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        3 2023-05-04 05:10:09.000000 backend.ai-test-23.3.1/backend.ai_test.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      626 2023-05-04 05:10:09.000000 backend.ai-test-23.3.1/backend_shim.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-04 05:10:09.758785 backend.ai-test-23.3.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2096 2023-05-04 05:10:09.000000 backend.ai-test-23.3.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 07:08:12.438857 backend.ai-test-23.3.2/
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-05 07:08:12.000000 backend.ai-test-23.3.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1304 2023-05-05 07:08:12.438857 backend.ai-test-23.3.2/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 07:08:12.434857 backend.ai-test-23.3.2/ai/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 07:08:12.434857 backend.ai-test-23.3.2/ai/backend/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 07:08:12.434857 backend.ai-test-23.3.2/ai/backend/test/
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-05 07:08:12.000000 backend.ai-test-23.3.2/ai/backend/test/VERSION
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-05 07:08:12.000000 backend.ai-test-23.3.2/ai/backend/test/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 07:08:12.438857 backend.ai-test-23.3.2/ai/backend/test/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 07:08:12.000000 backend.ai-test-23.3.2/ai/backend/test/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1607 2023-05-05 07:08:12.000000 backend.ai-test-23.3.2/ai/backend/test/cli/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-05-05 07:08:12.000000 backend.ai-test-23.3.2/ai/backend/test/cli/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)      848 2023-05-05 07:08:12.000000 backend.ai-test-23.3.2/ai/backend/test/cli/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-05 07:08:12.000000 backend.ai-test-23.3.2/ai/backend/test/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 07:08:12.438857 backend.ai-test-23.3.2/backend.ai_test.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1304 2023-05-05 07:08:12.000000 backend.ai-test-23.3.2/backend.ai_test.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      559 2023-05-05 07:08:12.000000 backend.ai-test-23.3.2/backend.ai_test.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 07:08:12.000000 backend.ai-test-23.3.2/backend.ai_test.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-05-05 07:08:12.000000 backend.ai-test-23.3.2/backend.ai_test.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 07:08:12.000000 backend.ai-test-23.3.2/backend.ai_test.egg-info/namespace_packages.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 07:08:12.000000 backend.ai-test-23.3.2/backend.ai_test.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       64 2023-05-05 07:08:12.000000 backend.ai-test-23.3.2/backend.ai_test.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        3 2023-05-05 07:08:12.000000 backend.ai-test-23.3.2/backend.ai_test.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      626 2023-05-05 07:08:12.000000 backend.ai-test-23.3.2/backend_shim.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-05 07:08:12.438857 backend.ai-test-23.3.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2096 2023-05-05 07:08:12.000000 backend.ai-test-23.3.2/setup.py
```

### Comparing `backend.ai-test-23.3.1/PKG-INFO` & `backend.ai-test-23.3.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: backend.ai-test
-Version: 23.3.1
+Version: 23.3.2
 Summary: Backend.AI Integration Test Suite
 Home-page: https://github.com/lablup/backend.ai
 Author: Lablup Inc. and contributors
 License: MIT
 Project-URL: Documentation, https://docs.backend.ai/
 Project-URL: Source, https://github.com/lablup/backend.ai
 Classifier: Intended Audience :: Developers
```

### Comparing `backend.ai-test-23.3.1/ai/backend/test/cli/__main__.py` & `backend.ai-test-23.3.2/ai/backend/test/cli/__main__.py`

 * *Files identical despite different names*

### Comparing `backend.ai-test-23.3.1/ai/backend/test/cli/utils.py` & `backend.ai-test-23.3.2/ai/backend/test/cli/utils.py`

 * *Files identical despite different names*

### Comparing `backend.ai-test-23.3.1/backend.ai_test.egg-info/PKG-INFO` & `backend.ai-test-23.3.2/backend.ai_test.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: backend.ai-test
-Version: 23.3.1
+Version: 23.3.2
 Summary: Backend.AI Integration Test Suite
 Home-page: https://github.com/lablup/backend.ai
 Author: Lablup Inc. and contributors
 License: MIT
 Project-URL: Documentation, https://docs.backend.ai/
 Project-URL: Source, https://github.com/lablup/backend.ai
 Classifier: Intended Audience :: Developers
```

### Comparing `backend.ai-test-23.3.1/backend.ai_test.egg-info/SOURCES.txt` & `backend.ai-test-23.3.2/backend.ai_test.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `backend.ai-test-23.3.1/backend_shim.py` & `backend.ai-test-23.3.2/backend_shim.py`

 * *Files identical despite different names*

### Comparing `backend.ai-test-23.3.1/setup.py` & `backend.ai-test-23.3.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -63,11 +63,11 @@
     ),
     'project_urls': {
         'Documentation': 'https://docs.backend.ai/',
         'Source': 'https://github.com/lablup/backend.ai',
     },
     'python_requires': '>=3.11,<3.12',
     'url': 'https://github.com/lablup/backend.ai',
-    'version': """23.03.1
+    'version': """23.03.2
 """,
     'zip_safe': False,
 })
```

