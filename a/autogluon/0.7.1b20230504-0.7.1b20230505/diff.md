# Comparing `tmp/autogluon-0.7.1b20230504.tar.gz` & `tmp/autogluon-0.7.1b20230505.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autogluon-0.7.1b20230504.tar", last modified: Thu May  4 09:04:32 2023, max compression
+gzip compressed data, was "autogluon-0.7.1b20230505.tar", last modified: Fri May  5 09:04:45 2023, max compression
```

## Comparing `autogluon-0.7.1b20230504.tar` & `autogluon-0.7.1b20230505.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:04:32.703671 autogluon-0.7.1b20230504/
--rw-r--r--   0 runner    (1001) docker     (123)    12540 2023-05-04 09:04:32.703671 autogluon-0.7.1b20230504/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-04 09:04:32.703671 autogluon-0.7.1b20230504/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1537 2023-05-04 09:03:46.000000 autogluon-0.7.1b20230504/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:04:32.699671 autogluon-0.7.1b20230504/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:04:32.703671 autogluon-0.7.1b20230504/src/autogluon/
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-05-04 09:03:46.000000 autogluon-0.7.1b20230504/src/autogluon/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-05-04 09:04:32.000000 autogluon-0.7.1b20230504/src/autogluon/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:04:32.703671 autogluon-0.7.1b20230504/src/autogluon.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    12540 2023-05-04 09:04:32.000000 autogluon-0.7.1b20230504/src/autogluon.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      321 2023-05-04 09:04:32.000000 autogluon-0.7.1b20230504/src/autogluon.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-04 09:04:32.000000 autogluon-0.7.1b20230504/src/autogluon.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-04 09:04:32.000000 autogluon-0.7.1b20230504/src/autogluon.egg-info/namespace_packages.txt
--rw-r--r--   0 runner    (1001) docker     (123)      189 2023-05-04 09:04:32.000000 autogluon-0.7.1b20230504/src/autogluon.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-04 09:04:32.000000 autogluon-0.7.1b20230504/src/autogluon.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-04 09:04:32.000000 autogluon-0.7.1b20230504/src/autogluon.egg-info/zip-safe
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 09:04:45.140150 autogluon-0.7.1b20230505/
+-rw-r--r--   0 runner    (1001) docker     (123)    12540 2023-05-05 09:04:45.136150 autogluon-0.7.1b20230505/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-05 09:04:45.140150 autogluon-0.7.1b20230505/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1537 2023-05-05 09:03:33.000000 autogluon-0.7.1b20230505/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 09:04:45.136150 autogluon-0.7.1b20230505/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 09:04:45.136150 autogluon-0.7.1b20230505/src/autogluon/
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-05-05 09:03:33.000000 autogluon-0.7.1b20230505/src/autogluon/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-05-05 09:04:44.000000 autogluon-0.7.1b20230505/src/autogluon/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 09:04:45.136150 autogluon-0.7.1b20230505/src/autogluon.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    12540 2023-05-05 09:04:45.000000 autogluon-0.7.1b20230505/src/autogluon.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      321 2023-05-05 09:04:45.000000 autogluon-0.7.1b20230505/src/autogluon.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 09:04:45.000000 autogluon-0.7.1b20230505/src/autogluon.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-05 09:04:45.000000 autogluon-0.7.1b20230505/src/autogluon.egg-info/namespace_packages.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      189 2023-05-05 09:04:45.000000 autogluon-0.7.1b20230505/src/autogluon.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-05 09:04:45.000000 autogluon-0.7.1b20230505/src/autogluon.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 09:04:45.000000 autogluon-0.7.1b20230505/src/autogluon.egg-info/zip-safe
```

### Comparing `autogluon-0.7.1b20230504/PKG-INFO` & `autogluon-0.7.1b20230505/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autogluon
-Version: 0.7.1b20230504
+Version: 0.7.1b20230505
 Summary: AutoML for Image, Text, and Tabular Data
 Home-page: https://github.com/autogluon/autogluon
 Author: AutoGluon Community
 License: Apache-2.0
 Project-URL: Documentation, https://auto.gluon.ai
 Project-URL: Bug Reports, https://github.com/autogluon/autogluon/issues
 Project-URL: Source, https://github.com/autogluon/autogluon/
```

### Comparing `autogluon-0.7.1b20230504/setup.py` & `autogluon-0.7.1b20230505/setup.py`

 * *Files identical despite different names*

### Comparing `autogluon-0.7.1b20230504/src/autogluon.egg-info/PKG-INFO` & `autogluon-0.7.1b20230505/src/autogluon.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autogluon
-Version: 0.7.1b20230504
+Version: 0.7.1b20230505
 Summary: AutoML for Image, Text, and Tabular Data
 Home-page: https://github.com/autogluon/autogluon
 Author: AutoGluon Community
 License: Apache-2.0
 Project-URL: Documentation, https://auto.gluon.ai
 Project-URL: Bug Reports, https://github.com/autogluon/autogluon/issues
 Project-URL: Source, https://github.com/autogluon/autogluon/
```

