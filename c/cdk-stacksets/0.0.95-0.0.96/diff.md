# Comparing `tmp/cdk-stacksets-0.0.95.tar.gz` & `tmp/cdk-stacksets-0.0.96.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cdk-stacksets-0.0.95.tar", last modified: Thu May  4 14:56:57 2023, max compression
+gzip compressed data, was "cdk-stacksets-0.0.96.tar", last modified: Fri May  5 00:17:14 2023, max compression
```

## Comparing `cdk-stacksets-0.0.95.tar` & `cdk-stacksets-0.0.96.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 14:56:57.099719 cdk-stacksets-0.0.95/
--rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-05-04 14:56:44.000000 cdk-stacksets-0.0.95/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-04 14:56:44.000000 cdk-stacksets-0.0.95/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    12163 2023-05-04 14:56:57.099719 cdk-stacksets-0.0.95/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    11249 2023-05-04 14:56:44.000000 cdk-stacksets-0.0.95/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-05-04 14:56:44.000000 cdk-stacksets-0.0.95/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-04 14:56:57.099719 cdk-stacksets-0.0.95/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1753 2023-05-04 14:56:44.000000 cdk-stacksets-0.0.95/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 14:56:57.095719 cdk-stacksets-0.0.95/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 14:56:57.095719 cdk-stacksets-0.0.95/src/cdk_stacksets/
--rw-r--r--   0 runner    (1001) docker     (123)    83981 2023-05-04 14:56:44.000000 cdk-stacksets-0.0.95/src/cdk_stacksets/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 14:56:57.095719 cdk-stacksets-0.0.95/src/cdk_stacksets/_jsii/
--rw-r--r--   0 runner    (1001) docker     (123)      395 2023-05-04 14:56:44.000000 cdk-stacksets-0.0.95/src/cdk_stacksets/_jsii/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    71110 2023-05-04 14:56:44.000000 cdk-stacksets-0.0.95/src/cdk_stacksets/_jsii/cdk-stacksets@0.0.95.jsii.tgz
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-04 14:56:44.000000 cdk-stacksets-0.0.95/src/cdk_stacksets/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 14:56:57.095719 cdk-stacksets-0.0.95/src/cdk_stacksets.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    12163 2023-05-04 14:56:57.000000 cdk-stacksets-0.0.95/src/cdk_stacksets.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      404 2023-05-04 14:56:57.000000 cdk-stacksets-0.0.95/src/cdk_stacksets.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-04 14:56:57.000000 cdk-stacksets-0.0.95/src/cdk_stacksets.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-05-04 14:56:57.000000 cdk-stacksets-0.0.95/src/cdk_stacksets.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-04 14:56:57.000000 cdk-stacksets-0.0.95/src/cdk_stacksets.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 00:17:14.896632 cdk-stacksets-0.0.96/
+-rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-05-05 00:16:56.000000 cdk-stacksets-0.0.96/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-05 00:16:56.000000 cdk-stacksets-0.0.96/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    12163 2023-05-05 00:17:14.896632 cdk-stacksets-0.0.96/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    11249 2023-05-05 00:16:56.000000 cdk-stacksets-0.0.96/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-05-05 00:16:56.000000 cdk-stacksets-0.0.96/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-05 00:17:14.896632 cdk-stacksets-0.0.96/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1753 2023-05-05 00:16:56.000000 cdk-stacksets-0.0.96/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 00:17:14.892632 cdk-stacksets-0.0.96/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 00:17:14.896632 cdk-stacksets-0.0.96/src/cdk_stacksets/
+-rw-r--r--   0 runner    (1001) docker     (123)    83981 2023-05-05 00:16:56.000000 cdk-stacksets-0.0.96/src/cdk_stacksets/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 00:17:14.896632 cdk-stacksets-0.0.96/src/cdk_stacksets/_jsii/
+-rw-r--r--   0 runner    (1001) docker     (123)      395 2023-05-05 00:16:56.000000 cdk-stacksets-0.0.96/src/cdk_stacksets/_jsii/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    71110 2023-05-05 00:16:56.000000 cdk-stacksets-0.0.96/src/cdk_stacksets/_jsii/cdk-stacksets@0.0.96.jsii.tgz
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 00:16:56.000000 cdk-stacksets-0.0.96/src/cdk_stacksets/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 00:17:14.896632 cdk-stacksets-0.0.96/src/cdk_stacksets.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    12163 2023-05-05 00:17:14.000000 cdk-stacksets-0.0.96/src/cdk_stacksets.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      404 2023-05-05 00:17:14.000000 cdk-stacksets-0.0.96/src/cdk_stacksets.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 00:17:14.000000 cdk-stacksets-0.0.96/src/cdk_stacksets.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-05-05 00:17:14.000000 cdk-stacksets-0.0.96/src/cdk_stacksets.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-05 00:17:14.000000 cdk-stacksets-0.0.96/src/cdk_stacksets.egg-info/top_level.txt
```

### Comparing `cdk-stacksets-0.0.95/LICENSE` & `cdk-stacksets-0.0.96/LICENSE`

 * *Files identical despite different names*

### Comparing `cdk-stacksets-0.0.95/PKG-INFO` & `cdk-stacksets-0.0.96/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cdk-stacksets
-Version: 0.0.95
+Version: 0.0.96
 Summary: cdk-stacksets
 Home-page: https://github.com/cdklabs/cdk-stacksets.git
 Author: Amazon Web Services<aws-cdk-dev@amazon.com>
 License: Apache-2.0
 Project-URL: Source, https://github.com/cdklabs/cdk-stacksets.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `cdk-stacksets-0.0.95/README.md` & `cdk-stacksets-0.0.96/README.md`

 * *Files identical despite different names*

### Comparing `cdk-stacksets-0.0.95/setup.py` & `cdk-stacksets-0.0.96/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "cdk-stacksets",
-    "version": "0.0.95",
+    "version": "0.0.96",
     "description": "cdk-stacksets",
     "license": "Apache-2.0",
     "url": "https://github.com/cdklabs/cdk-stacksets.git",
     "long_description_content_type": "text/markdown",
     "author": "Amazon Web Services<aws-cdk-dev@amazon.com>",
     "bdist_wheel": {
         "universal": true
@@ -22,15 +22,15 @@
     },
     "packages": [
         "cdk_stacksets",
         "cdk_stacksets._jsii"
     ],
     "package_data": {
         "cdk_stacksets._jsii": [
-            "cdk-stacksets@0.0.95.jsii.tgz"
+            "cdk-stacksets@0.0.96.jsii.tgz"
         ],
         "cdk_stacksets": [
             "py.typed"
         ]
     },
     "python_requires": "~=3.7",
     "install_requires": [
```

### Comparing `cdk-stacksets-0.0.95/src/cdk_stacksets/__init__.py` & `cdk-stacksets-0.0.96/src/cdk_stacksets/__init__.py`

 * *Files identical despite different names*

### Comparing `cdk-stacksets-0.0.95/src/cdk_stacksets.egg-info/PKG-INFO` & `cdk-stacksets-0.0.96/src/cdk_stacksets.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cdk-stacksets
-Version: 0.0.95
+Version: 0.0.96
 Summary: cdk-stacksets
 Home-page: https://github.com/cdklabs/cdk-stacksets.git
 Author: Amazon Web Services<aws-cdk-dev@amazon.com>
 License: Apache-2.0
 Project-URL: Source, https://github.com/cdklabs/cdk-stacksets.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

