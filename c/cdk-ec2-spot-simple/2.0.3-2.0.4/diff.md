# Comparing `tmp/cdk-ec2-spot-simple-2.0.3.tar.gz` & `tmp/cdk-ec2-spot-simple-2.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cdk-ec2-spot-simple-2.0.3.tar", last modified: Sun Feb 12 15:33:51 2023, max compression
+gzip compressed data, was "cdk-ec2-spot-simple-2.0.4.tar", last modified: Fri May  5 15:54:04 2023, max compression
```

## Comparing `cdk-ec2-spot-simple-2.0.3.tar` & `cdk-ec2-spot-simple-2.0.4.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-12 15:33:51.407191 cdk-ec2-spot-simple-2.0.3/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-02-12 15:33:30.000000 cdk-ec2-spot-simple-2.0.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-02-12 15:33:30.000000 cdk-ec2-spot-simple-2.0.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3733 2023-02-12 15:33:51.407191 cdk-ec2-spot-simple-2.0.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2797 2023-02-12 15:33:30.000000 cdk-ec2-spot-simple-2.0.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      236 2023-02-12 15:33:30.000000 cdk-ec2-spot-simple-2.0.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-12 15:33:51.407191 cdk-ec2-spot-simple-2.0.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1785 2023-02-12 15:33:30.000000 cdk-ec2-spot-simple-2.0.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-12 15:33:51.399191 cdk-ec2-spot-simple-2.0.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-12 15:33:51.403190 cdk-ec2-spot-simple-2.0.3/src/cdk_ec2_spot_simple/
--rw-r--r--   0 runner    (1001) docker     (123)    43875 2023-02-12 15:33:30.000000 cdk-ec2-spot-simple-2.0.3/src/cdk_ec2_spot_simple/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-12 15:33:51.407191 cdk-ec2-spot-simple-2.0.3/src/cdk_ec2_spot_simple/_jsii/
--rw-r--r--   0 runner    (1001) docker     (123)      418 2023-02-12 15:33:30.000000 cdk-ec2-spot-simple-2.0.3/src/cdk_ec2_spot_simple/_jsii/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   647872 2023-02-12 15:33:30.000000 cdk-ec2-spot-simple-2.0.3/src/cdk_ec2_spot_simple/_jsii/cdk-ec2-spot-simple@2.0.3.jsii.tgz
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-12 15:33:30.000000 cdk-ec2-spot-simple-2.0.3/src/cdk_ec2_spot_simple/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-12 15:33:51.407191 cdk-ec2-spot-simple-2.0.3/src/cdk_ec2_spot_simple.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3733 2023-02-12 15:33:49.000000 cdk-ec2-spot-simple-2.0.3/src/cdk_ec2_spot_simple.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      463 2023-02-12 15:33:51.000000 cdk-ec2-spot-simple-2.0.3/src/cdk_ec2_spot_simple.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-12 15:33:49.000000 cdk-ec2-spot-simple-2.0.3/src/cdk_ec2_spot_simple.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-02-12 15:33:50.000000 cdk-ec2-spot-simple-2.0.3/src/cdk_ec2_spot_simple.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-02-12 15:33:50.000000 cdk-ec2-spot-simple-2.0.3/src/cdk_ec2_spot_simple.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 15:54:04.141143 cdk-ec2-spot-simple-2.0.4/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-05 15:53:47.000000 cdk-ec2-spot-simple-2.0.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-05 15:53:47.000000 cdk-ec2-spot-simple-2.0.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3764 2023-05-05 15:54:04.141143 cdk-ec2-spot-simple-2.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2797 2023-05-05 15:53:47.000000 cdk-ec2-spot-simple-2.0.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-05-05 15:53:47.000000 cdk-ec2-spot-simple-2.0.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-05 15:54:04.141143 cdk-ec2-spot-simple-2.0.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1835 2023-05-05 15:53:47.000000 cdk-ec2-spot-simple-2.0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 15:54:04.125143 cdk-ec2-spot-simple-2.0.4/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 15:54:04.133143 cdk-ec2-spot-simple-2.0.4/src/cdk_ec2_spot_simple/
+-rw-r--r--   0 runner    (1001) docker     (123)    43875 2023-05-05 15:53:47.000000 cdk-ec2-spot-simple-2.0.4/src/cdk_ec2_spot_simple/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 15:54:04.141143 cdk-ec2-spot-simple-2.0.4/src/cdk_ec2_spot_simple/_jsii/
+-rw-r--r--   0 runner    (1001) docker     (123)      418 2023-05-05 15:53:47.000000 cdk-ec2-spot-simple-2.0.4/src/cdk_ec2_spot_simple/_jsii/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   647867 2023-05-05 15:53:47.000000 cdk-ec2-spot-simple-2.0.4/src/cdk_ec2_spot_simple/_jsii/cdk-ec2-spot-simple@2.0.4.jsii.tgz
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 15:53:47.000000 cdk-ec2-spot-simple-2.0.4/src/cdk_ec2_spot_simple/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 15:54:04.137143 cdk-ec2-spot-simple-2.0.4/src/cdk_ec2_spot_simple.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3764 2023-05-05 15:54:03.000000 cdk-ec2-spot-simple-2.0.4/src/cdk_ec2_spot_simple.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      463 2023-05-05 15:54:04.000000 cdk-ec2-spot-simple-2.0.4/src/cdk_ec2_spot_simple.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 15:54:03.000000 cdk-ec2-spot-simple-2.0.4/src/cdk_ec2_spot_simple.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-05-05 15:54:03.000000 cdk-ec2-spot-simple-2.0.4/src/cdk_ec2_spot_simple.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-05-05 15:54:03.000000 cdk-ec2-spot-simple-2.0.4/src/cdk_ec2_spot_simple.egg-info/top_level.txt
```

### Comparing `cdk-ec2-spot-simple-2.0.3/LICENSE` & `cdk-ec2-spot-simple-2.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `cdk-ec2-spot-simple-2.0.3/PKG-INFO` & `cdk-ec2-spot-simple-2.0.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: cdk-ec2-spot-simple
-Version: 2.0.3
+Version: 2.0.4
 Summary: CDK construct library to create EC2 Spot Instances simply.
 Home-page: https://github.com/tksst/cdk-ec2-spot-simple/
 Author: Takashi Sato<takashi@tks.st>
 License: Apache-2.0
 Project-URL: Source, https://github.com/tksst/cdk-ec2-spot-simple.git
-Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: JavaScript
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Typing :: Typed
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved
 Requires-Python: ~=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
@@ -113,9 +113,7 @@
 ## Background
 
 The `Instance` construct in `aws-cdk-lib/aws-ec2` does not have any spot instance functionality.
 
 This `SpotInstance` construct creates `LaunchTemplate` that is enabled spot request internally and associate with `Instance`.
 
 Also, `SpotInstance` creates a Lambda-backed custom resource if the spot requiest type is PERSISTENT. That resource deletes the spot request when the stack is destroyed.
-
-
```

### Comparing `cdk-ec2-spot-simple-2.0.3/README.md` & `cdk-ec2-spot-simple-2.0.4/README.md`

 * *Files identical despite different names*

### Comparing `cdk-ec2-spot-simple-2.0.3/setup.py` & `cdk-ec2-spot-simple-2.0.4/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "cdk-ec2-spot-simple",
-    "version": "2.0.3",
+    "version": "2.0.4",
     "description": "CDK construct library to create EC2 Spot Instances simply.",
     "license": "Apache-2.0",
     "url": "https://github.com/tksst/cdk-ec2-spot-simple/",
     "long_description_content_type": "text/markdown",
     "author": "Takashi Sato<takashi@tks.st>",
     "bdist_wheel": {
         "universal": true
@@ -22,37 +22,38 @@
     },
     "packages": [
         "cdk_ec2_spot_simple",
         "cdk_ec2_spot_simple._jsii"
     ],
     "package_data": {
         "cdk_ec2_spot_simple._jsii": [
-            "cdk-ec2-spot-simple@2.0.3.jsii.tgz"
+            "cdk-ec2-spot-simple@2.0.4.jsii.tgz"
         ],
         "cdk_ec2_spot_simple": [
             "py.typed"
         ]
     },
     "python_requires": "~=3.7",
     "install_requires": [
         "aws-cdk-lib>=2.24.0, <3.0.0",
         "constructs>=10.0.9, <11.0.0",
-        "jsii>=1.74.0, <2.0.0",
+        "jsii>=1.80.0, <2.0.0",
         "publication>=0.0.3",
         "typeguard~=2.13.3"
     ],
     "classifiers": [
         "Intended Audience :: Developers",
         "Operating System :: OS Independent",
         "Programming Language :: JavaScript",
         "Programming Language :: Python :: 3 :: Only",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
         "Typing :: Typed",
         "Development Status :: 5 - Production/Stable",
         "License :: OSI Approved"
     ],
     "scripts": []
 }
 """
```

### Comparing `cdk-ec2-spot-simple-2.0.3/src/cdk_ec2_spot_simple/__init__.py` & `cdk-ec2-spot-simple-2.0.4/src/cdk_ec2_spot_simple/__init__.py`

 * *Files identical despite different names*

### Comparing `cdk-ec2-spot-simple-2.0.3/src/cdk_ec2_spot_simple.egg-info/PKG-INFO` & `cdk-ec2-spot-simple-2.0.4/src/cdk_ec2_spot_simple.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: cdk-ec2-spot-simple
-Version: 2.0.3
+Version: 2.0.4
 Summary: CDK construct library to create EC2 Spot Instances simply.
 Home-page: https://github.com/tksst/cdk-ec2-spot-simple/
 Author: Takashi Sato<takashi@tks.st>
 License: Apache-2.0
 Project-URL: Source, https://github.com/tksst/cdk-ec2-spot-simple.git
-Platform: UNKNOWN
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: JavaScript
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Typing :: Typed
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved
 Requires-Python: ~=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
@@ -113,9 +113,7 @@
 ## Background
 
 The `Instance` construct in `aws-cdk-lib/aws-ec2` does not have any spot instance functionality.
 
 This `SpotInstance` construct creates `LaunchTemplate` that is enabled spot request internally and associate with `Instance`.
 
 Also, `SpotInstance` creates a Lambda-backed custom resource if the spot requiest type is PERSISTENT. That resource deletes the spot request when the stack is destroyed.
-
-
```

