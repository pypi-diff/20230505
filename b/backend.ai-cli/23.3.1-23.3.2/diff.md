# Comparing `tmp/backend.ai-cli-23.3.1.tar.gz` & `tmp/backend.ai-cli-23.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "backend.ai-cli-23.3.1.tar", last modified: Thu May  4 05:10:09 2023, max compression
+gzip compressed data, was "backend.ai-cli-23.3.2.tar", last modified: Fri May  5 07:08:13 2023, max compression
```

## Comparing `backend.ai-cli-23.3.1.tar` & `backend.ai-cli-23.3.2.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 05:10:09.814784 backend.ai-cli-23.3.1/
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-04 05:10:09.000000 backend.ai-cli-23.3.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1554 2023-05-04 05:10:09.814784 backend.ai-cli-23.3.1/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 05:10:09.814784 backend.ai-cli-23.3.1/ai/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 05:10:09.814784 backend.ai-cli-23.3.1/ai/backend/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 05:10:09.814784 backend.ai-cli-23.3.1/ai/backend/cli/
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-04 05:10:09.000000 backend.ai-cli-23.3.1/ai/backend/cli/VERSION
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-04 05:10:09.000000 backend.ai-cli-23.3.1/ai/backend/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      291 2023-05-04 05:10:09.000000 backend.ai-cli-23.3.1/ai/backend/cli/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5125 2023-05-04 05:10:09.000000 backend.ai-cli-23.3.1/ai/backend/cli/extensions.py
--rw-r--r--   0 runner    (1001) docker     (123)     4982 2023-05-04 05:10:09.000000 backend.ai-cli-23.3.1/ai/backend/cli/interaction.py
--rw-r--r--   0 runner    (1001) docker     (123)      985 2023-05-04 05:10:09.000000 backend.ai-cli-23.3.1/ai/backend/cli/loader.py
--rw-r--r--   0 runner    (1001) docker     (123)      707 2023-05-04 05:10:09.000000 backend.ai-cli-23.3.1/ai/backend/cli/main.py
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-04 05:10:09.000000 backend.ai-cli-23.3.1/ai/backend/cli/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)      381 2023-05-04 05:10:09.000000 backend.ai-cli-23.3.1/ai/backend/cli/types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 05:10:09.814784 backend.ai-cli-23.3.1/backend.ai_cli.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1554 2023-05-04 05:10:09.000000 backend.ai-cli-23.3.1/backend.ai_cli.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      582 2023-05-04 05:10:09.000000 backend.ai-cli-23.3.1/backend.ai_cli.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-04 05:10:09.000000 backend.ai-cli-23.3.1/backend.ai_cli.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-05-04 05:10:09.000000 backend.ai-cli-23.3.1/backend.ai_cli.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-04 05:10:09.000000 backend.ai-cli-23.3.1/backend.ai_cli.egg-info/namespace_packages.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-04 05:10:09.000000 backend.ai-cli-23.3.1/backend.ai_cli.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-05-04 05:10:09.000000 backend.ai-cli-23.3.1/backend.ai_cli.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        3 2023-05-04 05:10:09.000000 backend.ai-cli-23.3.1/backend.ai_cli.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      626 2023-05-04 05:10:09.000000 backend.ai-cli-23.3.1/backend_shim.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-04 05:10:09.814784 backend.ai-cli-23.3.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2293 2023-05-04 05:10:09.000000 backend.ai-cli-23.3.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 07:08:13.122859 backend.ai-cli-23.3.2/
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-05 07:08:12.000000 backend.ai-cli-23.3.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1554 2023-05-05 07:08:13.122859 backend.ai-cli-23.3.2/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 07:08:13.118859 backend.ai-cli-23.3.2/ai/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 07:08:13.118859 backend.ai-cli-23.3.2/ai/backend/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 07:08:13.122859 backend.ai-cli-23.3.2/ai/backend/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-05 07:08:12.000000 backend.ai-cli-23.3.2/ai/backend/cli/VERSION
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-05 07:08:12.000000 backend.ai-cli-23.3.2/ai/backend/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      291 2023-05-05 07:08:12.000000 backend.ai-cli-23.3.2/ai/backend/cli/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5125 2023-05-05 07:08:12.000000 backend.ai-cli-23.3.2/ai/backend/cli/extensions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4982 2023-05-05 07:08:12.000000 backend.ai-cli-23.3.2/ai/backend/cli/interaction.py
+-rw-r--r--   0 runner    (1001) docker     (123)      985 2023-05-05 07:08:12.000000 backend.ai-cli-23.3.2/ai/backend/cli/loader.py
+-rw-r--r--   0 runner    (1001) docker     (123)      707 2023-05-05 07:08:12.000000 backend.ai-cli-23.3.2/ai/backend/cli/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-05 07:08:12.000000 backend.ai-cli-23.3.2/ai/backend/cli/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)      381 2023-05-05 07:08:12.000000 backend.ai-cli-23.3.2/ai/backend/cli/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 07:08:13.122859 backend.ai-cli-23.3.2/backend.ai_cli.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1554 2023-05-05 07:08:13.000000 backend.ai-cli-23.3.2/backend.ai_cli.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      582 2023-05-05 07:08:13.000000 backend.ai-cli-23.3.2/backend.ai_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 07:08:13.000000 backend.ai-cli-23.3.2/backend.ai_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-05-05 07:08:13.000000 backend.ai-cli-23.3.2/backend.ai_cli.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 07:08:13.000000 backend.ai-cli-23.3.2/backend.ai_cli.egg-info/namespace_packages.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 07:08:13.000000 backend.ai-cli-23.3.2/backend.ai_cli.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-05-05 07:08:13.000000 backend.ai-cli-23.3.2/backend.ai_cli.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        3 2023-05-05 07:08:13.000000 backend.ai-cli-23.3.2/backend.ai_cli.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      626 2023-05-05 07:08:12.000000 backend.ai-cli-23.3.2/backend_shim.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-05 07:08:13.122859 backend.ai-cli-23.3.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2293 2023-05-05 07:08:12.000000 backend.ai-cli-23.3.2/setup.py
```

### Comparing `backend.ai-cli-23.3.1/PKG-INFO` & `backend.ai-cli-23.3.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: backend.ai-cli
-Version: 23.3.1
+Version: 23.3.2
 Summary: Backend.AI Command Line Interface Helper
 Home-page: https://github.com/lablup/backend.ai
 Author: Lablup Inc. and contributors
 License: MIT
 Project-URL: Documentation, https://docs.backend.ai/
 Project-URL: Source, https://github.com/lablup/backend.ai
 Classifier: Intended Audience :: Developers
```

### Comparing `backend.ai-cli-23.3.1/ai/backend/cli/extensions.py` & `backend.ai-cli-23.3.2/ai/backend/cli/extensions.py`

 * *Files identical despite different names*

### Comparing `backend.ai-cli-23.3.1/ai/backend/cli/interaction.py` & `backend.ai-cli-23.3.2/ai/backend/cli/interaction.py`

 * *Files identical despite different names*

### Comparing `backend.ai-cli-23.3.1/ai/backend/cli/loader.py` & `backend.ai-cli-23.3.2/ai/backend/cli/loader.py`

 * *Files identical despite different names*

### Comparing `backend.ai-cli-23.3.1/ai/backend/cli/main.py` & `backend.ai-cli-23.3.2/ai/backend/cli/main.py`

 * *Files identical despite different names*

### Comparing `backend.ai-cli-23.3.1/backend.ai_cli.egg-info/PKG-INFO` & `backend.ai-cli-23.3.2/backend.ai_cli.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: backend.ai-cli
-Version: 23.3.1
+Version: 23.3.2
 Summary: Backend.AI Command Line Interface Helper
 Home-page: https://github.com/lablup/backend.ai
 Author: Lablup Inc. and contributors
 License: MIT
 Project-URL: Documentation, https://docs.backend.ai/
 Project-URL: Source, https://github.com/lablup/backend.ai
 Classifier: Intended Audience :: Developers
```

### Comparing `backend.ai-cli-23.3.1/backend.ai_cli.egg-info/SOURCES.txt` & `backend.ai-cli-23.3.2/backend.ai_cli.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `backend.ai-cli-23.3.1/backend_shim.py` & `backend.ai-cli-23.3.2/backend_shim.py`

 * *Files identical despite different names*

### Comparing `backend.ai-cli-23.3.1/setup.py` & `backend.ai-cli-23.3.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,15 +22,15 @@
     'entry_points': {
         'console_scripts': [
             'backend.ai = ai.backend.cli.__main__:main',
         ],
     },
     'install_requires': (
         'attrs>=20.3',
-        """backend.ai-plugin==23.03.1
+        """backend.ai-plugin==23.03.2
 """,
         'click>=7.1.2',
     ),
     'license': 'MIT',
     'long_description': """# backend.ai-cli
 
 Unified command-line interface for Backend.AI
@@ -70,11 +70,11 @@
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

