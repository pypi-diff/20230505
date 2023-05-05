# Comparing `tmp/backend.ai-plugin-23.3.1.tar.gz` & `tmp/backend.ai-plugin-23.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "backend.ai-plugin-23.3.1.tar", last modified: Thu May  4 05:10:10 2023, max compression
+gzip compressed data, was "backend.ai-plugin-23.3.2.tar", last modified: Fri May  5 07:08:12 2023, max compression
```

## Comparing `backend.ai-plugin-23.3.1.tar` & `backend.ai-plugin-23.3.2.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 05:10:10.042780 backend.ai-plugin-23.3.1/
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-04 05:10:09.000000 backend.ai-plugin-23.3.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1028 2023-05-04 05:10:10.042780 backend.ai-plugin-23.3.1/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 05:10:10.038780 backend.ai-plugin-23.3.1/ai/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 05:10:10.038780 backend.ai-plugin-23.3.1/ai/backend/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 05:10:10.042780 backend.ai-plugin-23.3.1/ai/backend/plugin/
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-04 05:10:09.000000 backend.ai-plugin-23.3.1/ai/backend/plugin/VERSION
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-04 05:10:09.000000 backend.ai-plugin-23.3.1/ai/backend/plugin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8139 2023-05-04 05:10:09.000000 backend.ai-plugin-23.3.1/ai/backend/plugin/entrypoint.py
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-04 05:10:09.000000 backend.ai-plugin-23.3.1/ai/backend/plugin/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 05:10:10.042780 backend.ai-plugin-23.3.1/backend.ai_plugin.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1028 2023-05-04 05:10:10.000000 backend.ai-plugin-23.3.1/backend.ai_plugin.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      405 2023-05-04 05:10:10.000000 backend.ai-plugin-23.3.1/backend.ai_plugin.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-04 05:10:10.000000 backend.ai-plugin-23.3.1/backend.ai_plugin.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-04 05:10:10.000000 backend.ai-plugin-23.3.1/backend.ai_plugin.egg-info/namespace_packages.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-04 05:10:10.000000 backend.ai-plugin-23.3.1/backend.ai_plugin.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)        3 2023-05-04 05:10:10.000000 backend.ai-plugin-23.3.1/backend.ai_plugin.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      626 2023-05-04 05:10:09.000000 backend.ai-plugin-23.3.1/backend_shim.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-04 05:10:10.042780 backend.ai-plugin-23.3.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1560 2023-05-04 05:10:09.000000 backend.ai-plugin-23.3.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 07:08:12.854858 backend.ai-plugin-23.3.2/
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-05 07:08:12.000000 backend.ai-plugin-23.3.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1028 2023-05-05 07:08:12.854858 backend.ai-plugin-23.3.2/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 07:08:12.850859 backend.ai-plugin-23.3.2/ai/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 07:08:12.850859 backend.ai-plugin-23.3.2/ai/backend/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 07:08:12.850859 backend.ai-plugin-23.3.2/ai/backend/plugin/
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-05 07:08:12.000000 backend.ai-plugin-23.3.2/ai/backend/plugin/VERSION
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-05 07:08:12.000000 backend.ai-plugin-23.3.2/ai/backend/plugin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8139 2023-05-05 07:08:12.000000 backend.ai-plugin-23.3.2/ai/backend/plugin/entrypoint.py
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-05 07:08:12.000000 backend.ai-plugin-23.3.2/ai/backend/plugin/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 07:08:12.854858 backend.ai-plugin-23.3.2/backend.ai_plugin.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1028 2023-05-05 07:08:12.000000 backend.ai-plugin-23.3.2/backend.ai_plugin.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      405 2023-05-05 07:08:12.000000 backend.ai-plugin-23.3.2/backend.ai_plugin.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 07:08:12.000000 backend.ai-plugin-23.3.2/backend.ai_plugin.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 07:08:12.000000 backend.ai-plugin-23.3.2/backend.ai_plugin.egg-info/namespace_packages.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 07:08:12.000000 backend.ai-plugin-23.3.2/backend.ai_plugin.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)        3 2023-05-05 07:08:12.000000 backend.ai-plugin-23.3.2/backend.ai_plugin.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      626 2023-05-05 07:08:12.000000 backend.ai-plugin-23.3.2/backend_shim.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-05 07:08:12.854858 backend.ai-plugin-23.3.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1560 2023-05-05 07:08:12.000000 backend.ai-plugin-23.3.2/setup.py
```

### Comparing `backend.ai-plugin-23.3.1/PKG-INFO` & `backend.ai-plugin-23.3.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: backend.ai-plugin
-Version: 23.3.1
+Version: 23.3.2
 Summary: Backend.AI Plugin Subsystem
 Home-page: https://github.com/lablup/backend.ai
 Author: Lablup Inc. and contributors
 License: MIT
 Project-URL: Documentation, https://docs.backend.ai/
 Project-URL: Source, https://github.com/lablup/backend.ai
 Classifier: Intended Audience :: Developers
```

### Comparing `backend.ai-plugin-23.3.1/ai/backend/plugin/entrypoint.py` & `backend.ai-plugin-23.3.2/ai/backend/plugin/entrypoint.py`

 * *Files identical despite different names*

### Comparing `backend.ai-plugin-23.3.1/backend.ai_plugin.egg-info/PKG-INFO` & `backend.ai-plugin-23.3.2/backend.ai_plugin.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: backend.ai-plugin
-Version: 23.3.1
+Version: 23.3.2
 Summary: Backend.AI Plugin Subsystem
 Home-page: https://github.com/lablup/backend.ai
 Author: Lablup Inc. and contributors
 License: MIT
 Project-URL: Documentation, https://docs.backend.ai/
 Project-URL: Source, https://github.com/lablup/backend.ai
 Classifier: Intended Audience :: Developers
```

### Comparing `backend.ai-plugin-23.3.1/backend_shim.py` & `backend.ai-plugin-23.3.2/backend_shim.py`

 * *Files identical despite different names*

### Comparing `backend.ai-plugin-23.3.1/setup.py` & `backend.ai-plugin-23.3.2/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -45,11 +45,11 @@
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

