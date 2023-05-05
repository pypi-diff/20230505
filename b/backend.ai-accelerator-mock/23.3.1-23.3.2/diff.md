# Comparing `tmp/backend.ai-accelerator-mock-23.3.1.tar.gz` & `tmp/backend.ai-accelerator-mock-23.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "backend.ai-accelerator-mock-23.3.1.tar", last modified: Thu May  4 05:10:17 2023, max compression
+gzip compressed data, was "backend.ai-accelerator-mock-23.3.2.tar", last modified: Fri May  5 07:08:19 2023, max compression
```

## Comparing `backend.ai-accelerator-mock-23.3.1.tar` & `backend.ai-accelerator-mock-23.3.2.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 05:10:17.626670 backend.ai-accelerator-mock-23.3.1/
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-04 05:10:17.000000 backend.ai-accelerator-mock-23.3.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1946 2023-05-04 05:10:17.626670 backend.ai-accelerator-mock-23.3.1/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 05:10:17.626670 backend.ai-accelerator-mock-23.3.1/ai/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 05:10:17.626670 backend.ai-accelerator-mock-23.3.1/ai/backend/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 05:10:17.626670 backend.ai-accelerator-mock-23.3.1/ai/backend/accelerator/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 05:10:17.626670 backend.ai-accelerator-mock-23.3.1/ai/backend/accelerator/mock/
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-04 05:10:17.000000 backend.ai-accelerator-mock-23.3.1/ai/backend/accelerator/mock/VERSION
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-04 05:10:17.000000 backend.ai-accelerator-mock-23.3.1/ai/backend/accelerator/mock/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      109 2023-05-04 05:10:17.000000 backend.ai-accelerator-mock-23.3.1/ai/backend/accelerator/mock/defs.py
--rw-r--r--   0 runner    (1001) docker     (123)    32914 2023-05-04 05:10:17.000000 backend.ai-accelerator-mock-23.3.1/ai/backend/accelerator/mock/plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-04 05:10:17.000000 backend.ai-accelerator-mock-23.3.1/ai/backend/accelerator/mock/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     1972 2023-05-04 05:10:17.000000 backend.ai-accelerator-mock-23.3.1/ai/backend/accelerator/mock/types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 05:10:17.626670 backend.ai-accelerator-mock-23.3.1/backend.ai_accelerator_mock.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1946 2023-05-04 05:10:17.000000 backend.ai-accelerator-mock-23.3.1/backend.ai_accelerator_mock.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      678 2023-05-04 05:10:17.000000 backend.ai-accelerator-mock-23.3.1/backend.ai_accelerator_mock.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-04 05:10:17.000000 backend.ai-accelerator-mock-23.3.1/backend.ai_accelerator_mock.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-05-04 05:10:17.000000 backend.ai-accelerator-mock-23.3.1/backend.ai_accelerator_mock.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-04 05:10:17.000000 backend.ai-accelerator-mock-23.3.1/backend.ai_accelerator_mock.egg-info/namespace_packages.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-04 05:10:17.000000 backend.ai-accelerator-mock-23.3.1/backend.ai_accelerator_mock.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      231 2023-05-04 05:10:17.000000 backend.ai-accelerator-mock-23.3.1/backend.ai_accelerator_mock.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        3 2023-05-04 05:10:17.000000 backend.ai-accelerator-mock-23.3.1/backend.ai_accelerator_mock.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      626 2023-05-04 05:10:17.000000 backend.ai-accelerator-mock-23.3.1/backend_shim.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-04 05:10:17.626670 backend.ai-accelerator-mock-23.3.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3020 2023-05-04 05:10:17.000000 backend.ai-accelerator-mock-23.3.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 07:08:19.866471 backend.ai-accelerator-mock-23.3.2/
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-05 07:08:19.000000 backend.ai-accelerator-mock-23.3.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1946 2023-05-05 07:08:19.866471 backend.ai-accelerator-mock-23.3.2/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 07:08:19.866471 backend.ai-accelerator-mock-23.3.2/ai/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 07:08:19.866471 backend.ai-accelerator-mock-23.3.2/ai/backend/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 07:08:19.866471 backend.ai-accelerator-mock-23.3.2/ai/backend/accelerator/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 07:08:19.866471 backend.ai-accelerator-mock-23.3.2/ai/backend/accelerator/mock/
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-05 07:08:19.000000 backend.ai-accelerator-mock-23.3.2/ai/backend/accelerator/mock/VERSION
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-05 07:08:19.000000 backend.ai-accelerator-mock-23.3.2/ai/backend/accelerator/mock/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      109 2023-05-05 07:08:19.000000 backend.ai-accelerator-mock-23.3.2/ai/backend/accelerator/mock/defs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32914 2023-05-05 07:08:19.000000 backend.ai-accelerator-mock-23.3.2/ai/backend/accelerator/mock/plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-05 07:08:19.000000 backend.ai-accelerator-mock-23.3.2/ai/backend/accelerator/mock/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     1972 2023-05-05 07:08:19.000000 backend.ai-accelerator-mock-23.3.2/ai/backend/accelerator/mock/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 07:08:19.866471 backend.ai-accelerator-mock-23.3.2/backend.ai_accelerator_mock.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1946 2023-05-05 07:08:19.000000 backend.ai-accelerator-mock-23.3.2/backend.ai_accelerator_mock.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      678 2023-05-05 07:08:19.000000 backend.ai-accelerator-mock-23.3.2/backend.ai_accelerator_mock.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 07:08:19.000000 backend.ai-accelerator-mock-23.3.2/backend.ai_accelerator_mock.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-05-05 07:08:19.000000 backend.ai-accelerator-mock-23.3.2/backend.ai_accelerator_mock.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 07:08:19.000000 backend.ai-accelerator-mock-23.3.2/backend.ai_accelerator_mock.egg-info/namespace_packages.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 07:08:19.000000 backend.ai-accelerator-mock-23.3.2/backend.ai_accelerator_mock.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      231 2023-05-05 07:08:19.000000 backend.ai-accelerator-mock-23.3.2/backend.ai_accelerator_mock.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        3 2023-05-05 07:08:19.000000 backend.ai-accelerator-mock-23.3.2/backend.ai_accelerator_mock.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      626 2023-05-05 07:08:19.000000 backend.ai-accelerator-mock-23.3.2/backend_shim.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-05 07:08:19.866471 backend.ai-accelerator-mock-23.3.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3020 2023-05-05 07:08:19.000000 backend.ai-accelerator-mock-23.3.2/setup.py
```

### Comparing `backend.ai-accelerator-mock-23.3.1/PKG-INFO` & `backend.ai-accelerator-mock-23.3.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: backend.ai-accelerator-mock
-Version: 23.3.1
+Version: 23.3.2
 Summary: Backend.AI Mockup Accelerator Plugin
 Home-page: https://github.com/lablup/backend.ai
 Author: Lablup Inc. and contributors
 License: LGPLv3
 Project-URL: Documentation, https://docs.backend.ai/
 Project-URL: Source, https://github.com/lablup/backend.ai
 Classifier: Intended Audience :: Developers
```

### Comparing `backend.ai-accelerator-mock-23.3.1/ai/backend/accelerator/mock/plugin.py` & `backend.ai-accelerator-mock-23.3.2/ai/backend/accelerator/mock/plugin.py`

 * *Files identical despite different names*

### Comparing `backend.ai-accelerator-mock-23.3.1/ai/backend/accelerator/mock/types.py` & `backend.ai-accelerator-mock-23.3.2/ai/backend/accelerator/mock/types.py`

 * *Files identical despite different names*

### Comparing `backend.ai-accelerator-mock-23.3.1/backend.ai_accelerator_mock.egg-info/PKG-INFO` & `backend.ai-accelerator-mock-23.3.2/backend.ai_accelerator_mock.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: backend.ai-accelerator-mock
-Version: 23.3.1
+Version: 23.3.2
 Summary: Backend.AI Mockup Accelerator Plugin
 Home-page: https://github.com/lablup/backend.ai
 Author: Lablup Inc. and contributors
 License: LGPLv3
 Project-URL: Documentation, https://docs.backend.ai/
 Project-URL: Source, https://github.com/lablup/backend.ai
 Classifier: Intended Audience :: Developers
```

### Comparing `backend.ai-accelerator-mock-23.3.1/backend.ai_accelerator_mock.egg-info/SOURCES.txt` & `backend.ai-accelerator-mock-23.3.2/backend.ai_accelerator_mock.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `backend.ai-accelerator-mock-23.3.1/backend_shim.py` & `backend.ai-accelerator-mock-23.3.2/backend_shim.py`

 * *Files identical despite different names*

### Comparing `backend.ai-accelerator-mock-23.3.1/setup.py` & `backend.ai-accelerator-mock-23.3.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,27 +22,27 @@
     'entry_points': {
         'backendai_accelerator_v21': [
             'mock = ai.backend.accelerator.mock.plugin:MockPlugin',
         ],
     },
     'install_requires': (
         'aiodocker~=0.21.0',
-        """backend.ai-agent==23.03.1
+        """backend.ai-agent==23.03.2
 """,
-        """backend.ai-cli==23.03.1
+        """backend.ai-cli==23.03.2
 """,
-        """backend.ai-common==23.03.1
+        """backend.ai-common==23.03.2
 """,
-        """backend.ai-kernel-binary==23.03.1
+        """backend.ai-kernel-binary==23.03.2
 """,
-        """backend.ai-kernel-helper==23.03.1
+        """backend.ai-kernel-helper==23.03.2
 """,
-        """backend.ai-kernel==23.03.1
+        """backend.ai-kernel==23.03.2
 """,
-        """backend.ai-plugin==23.03.1
+        """backend.ai-plugin==23.03.2
 """,
         'trafaret~=2.1',
     ),
     'license': 'LGPLv3',
     'long_description': """# backend.ai-accelerator-mock
 
 A mockup plugin for accelerators
@@ -74,11 +74,11 @@
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

