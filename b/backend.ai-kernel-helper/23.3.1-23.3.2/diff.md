# Comparing `tmp/backend.ai-kernel-helper-23.3.1.tar.gz` & `tmp/backend.ai-kernel-helper-23.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "backend.ai-kernel-helper-23.3.1.tar", last modified: Thu May  4 05:10:09 2023, max compression
+gzip compressed data, was "backend.ai-kernel-helper-23.3.2.tar", last modified: Fri May  5 07:08:12 2023, max compression
```

## Comparing `backend.ai-kernel-helper-23.3.1.tar` & `backend.ai-kernel-helper-23.3.2.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 05:10:09.462789 backend.ai-kernel-helper-23.3.1/
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-04 05:10:08.000000 backend.ai-kernel-helper-23.3.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      970 2023-05-04 05:10:09.462789 backend.ai-kernel-helper-23.3.1/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 05:10:09.458789 backend.ai-kernel-helper-23.3.1/ai/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 05:10:09.458789 backend.ai-kernel-helper-23.3.1/ai/backend/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 05:10:09.458789 backend.ai-kernel-helper-23.3.1/ai/backend/helpers/
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-04 05:10:08.000000 backend.ai-kernel-helper-23.3.1/ai/backend/helpers/VERSION
--rw-r--r--   0 runner    (1001) docker     (123)      110 2023-05-04 05:10:08.000000 backend.ai-kernel-helper-23.3.1/ai/backend/helpers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1281 2023-05-04 05:10:08.000000 backend.ai-kernel-helper-23.3.1/ai/backend/helpers/package.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 05:10:09.462789 backend.ai-kernel-helper-23.3.1/backend.ai_kernel_helper.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      970 2023-05-04 05:10:09.000000 backend.ai-kernel-helper-23.3.1/backend.ai_kernel_helper.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      467 2023-05-04 05:10:09.000000 backend.ai-kernel-helper-23.3.1/backend.ai_kernel_helper.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-04 05:10:09.000000 backend.ai-kernel-helper-23.3.1/backend.ai_kernel_helper.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-04 05:10:09.000000 backend.ai-kernel-helper-23.3.1/backend.ai_kernel_helper.egg-info/namespace_packages.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-04 05:10:09.000000 backend.ai-kernel-helper-23.3.1/backend.ai_kernel_helper.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-05-04 05:10:09.000000 backend.ai-kernel-helper-23.3.1/backend.ai_kernel_helper.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        3 2023-05-04 05:10:09.000000 backend.ai-kernel-helper-23.3.1/backend.ai_kernel_helper.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      626 2023-05-04 05:10:08.000000 backend.ai-kernel-helper-23.3.1/backend_shim.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-04 05:10:09.462789 backend.ai-kernel-helper-23.3.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1512 2023-05-04 05:10:08.000000 backend.ai-kernel-helper-23.3.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 07:08:12.046856 backend.ai-kernel-helper-23.3.2/
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-05 07:08:11.000000 backend.ai-kernel-helper-23.3.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      970 2023-05-05 07:08:12.046856 backend.ai-kernel-helper-23.3.2/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 07:08:12.042856 backend.ai-kernel-helper-23.3.2/ai/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 07:08:12.042856 backend.ai-kernel-helper-23.3.2/ai/backend/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 07:08:12.042856 backend.ai-kernel-helper-23.3.2/ai/backend/helpers/
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-05 07:08:11.000000 backend.ai-kernel-helper-23.3.2/ai/backend/helpers/VERSION
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-05-05 07:08:11.000000 backend.ai-kernel-helper-23.3.2/ai/backend/helpers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1281 2023-05-05 07:08:11.000000 backend.ai-kernel-helper-23.3.2/ai/backend/helpers/package.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 07:08:12.042856 backend.ai-kernel-helper-23.3.2/backend.ai_kernel_helper.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      970 2023-05-05 07:08:12.000000 backend.ai-kernel-helper-23.3.2/backend.ai_kernel_helper.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      467 2023-05-05 07:08:12.000000 backend.ai-kernel-helper-23.3.2/backend.ai_kernel_helper.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 07:08:12.000000 backend.ai-kernel-helper-23.3.2/backend.ai_kernel_helper.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 07:08:12.000000 backend.ai-kernel-helper-23.3.2/backend.ai_kernel_helper.egg-info/namespace_packages.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 07:08:11.000000 backend.ai-kernel-helper-23.3.2/backend.ai_kernel_helper.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-05-05 07:08:12.000000 backend.ai-kernel-helper-23.3.2/backend.ai_kernel_helper.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        3 2023-05-05 07:08:12.000000 backend.ai-kernel-helper-23.3.2/backend.ai_kernel_helper.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      626 2023-05-05 07:08:11.000000 backend.ai-kernel-helper-23.3.2/backend_shim.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-05 07:08:12.046856 backend.ai-kernel-helper-23.3.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1512 2023-05-05 07:08:11.000000 backend.ai-kernel-helper-23.3.2/setup.py
```

### Comparing `backend.ai-kernel-helper-23.3.1/PKG-INFO` & `backend.ai-kernel-helper-23.3.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: backend.ai-kernel-helper
-Version: 23.3.1
+Version: 23.3.2
 Summary: Backend.AI Kernel Runner Prebuilt Binaries Package
 Home-page: https://github.com/lablup/backend.ai
 Author: Lablup Inc. and contributors
 License: LGPLv3
 Project-URL: Documentation, https://docs.backend.ai/
 Project-URL: Source, https://github.com/lablup/backend.ai
 Classifier: Intended Audience :: Developers
```

### Comparing `backend.ai-kernel-helper-23.3.1/ai/backend/helpers/package.py` & `backend.ai-kernel-helper-23.3.2/ai/backend/helpers/package.py`

 * *Files identical despite different names*

### Comparing `backend.ai-kernel-helper-23.3.1/backend.ai_kernel_helper.egg-info/PKG-INFO` & `backend.ai-kernel-helper-23.3.2/backend.ai_kernel_helper.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: backend.ai-kernel-helper
-Version: 23.3.1
+Version: 23.3.2
 Summary: Backend.AI Kernel Runner Prebuilt Binaries Package
 Home-page: https://github.com/lablup/backend.ai
 Author: Lablup Inc. and contributors
 License: LGPLv3
 Project-URL: Documentation, https://docs.backend.ai/
 Project-URL: Source, https://github.com/lablup/backend.ai
 Classifier: Intended Audience :: Developers
```

### Comparing `backend.ai-kernel-helper-23.3.1/backend_shim.py` & `backend.ai-kernel-helper-23.3.2/backend_shim.py`

 * *Files identical despite different names*

### Comparing `backend.ai-kernel-helper-23.3.1/setup.py` & `backend.ai-kernel-helper-23.3.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -39,11 +39,11 @@
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

