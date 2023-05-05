# Comparing `tmp/sdeclient-0.0.3.tar.gz` & `tmp/sdeclient-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sdeclient-0.0.3.tar", last modified: Fri May  5 15:13:21 2023, max compression
+gzip compressed data, was "sdeclient-0.0.4.tar", last modified: Fri May  5 15:19:31 2023, max compression
```

## Comparing `sdeclient-0.0.3.tar` & `sdeclient-0.0.4.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 bsawa      (501) staff       (20)        0 2023-05-05 15:13:21.798206 sdeclient-0.0.3/
--rw-r--r--   0 bsawa      (501) staff       (20)      527 2023-05-05 15:13:21.797843 sdeclient-0.0.3/PKG-INFO
-drwxr-xr-x   0 bsawa      (501) staff       (20)        0 2023-05-05 15:13:21.793549 sdeclient-0.0.3/sdeclient/
--rw-r--r--   0 bsawa      (501) staff       (20)      101 2023-05-05 15:12:46.000000 sdeclient-0.0.3/sdeclient/__init__.py
--rw-r--r--   0 bsawa      (501) staff       (20)    58272 2023-05-05 15:12:42.000000 sdeclient-0.0.3/sdeclient/sdeclient.py
--rw-r--r--   0 bsawa      (501) staff       (20)     8717 2023-05-05 15:12:43.000000 sdeclient-0.0.3/sdeclient/sdeutilities.py
--rw-r--r--   0 bsawa      (501) staff       (20)     3462 2023-05-04 15:42:28.000000 sdeclient-0.0.3/sdeclient/simplelog.py
-drwxr-xr-x   0 bsawa      (501) staff       (20)        0 2023-05-05 15:13:21.797056 sdeclient-0.0.3/sdeclient.egg-info/
--rw-r--r--   0 bsawa      (501) staff       (20)      527 2023-05-05 15:13:21.000000 sdeclient-0.0.3/sdeclient.egg-info/PKG-INFO
--rw-r--r--   0 bsawa      (501) staff       (20)      234 2023-05-05 15:13:21.000000 sdeclient-0.0.3/sdeclient.egg-info/SOURCES.txt
--rw-r--r--   0 bsawa      (501) staff       (20)        1 2023-05-05 15:13:21.000000 sdeclient-0.0.3/sdeclient.egg-info/dependency_links.txt
--rw-r--r--   0 bsawa      (501) staff       (20)       10 2023-05-05 15:13:21.000000 sdeclient-0.0.3/sdeclient.egg-info/top_level.txt
--rw-r--r--   0 bsawa      (501) staff       (20)       38 2023-05-05 15:13:21.798327 sdeclient-0.0.3/setup.cfg
--rw-r--r--   0 bsawa      (501) staff       (20)      750 2023-05-05 15:12:48.000000 sdeclient-0.0.3/setup.py
+drwxr-xr-x   0 bsawa      (501) staff       (20)        0 2023-05-05 15:19:31.545702 sdeclient-0.0.4/
+-rw-r--r--   0 bsawa      (501) staff       (20)      527 2023-05-05 15:19:31.545319 sdeclient-0.0.4/PKG-INFO
+drwxr-xr-x   0 bsawa      (501) staff       (20)        0 2023-05-05 15:19:31.540962 sdeclient-0.0.4/sdeclient/
+-rw-r--r--   0 bsawa      (501) staff       (20)        0 2023-05-05 15:19:26.000000 sdeclient-0.0.4/sdeclient/__init__.py
+-rw-r--r--   0 bsawa      (501) staff       (20)    58272 2023-05-05 15:19:27.000000 sdeclient-0.0.4/sdeclient/sdeclient.py
+-rw-r--r--   0 bsawa      (501) staff       (20)     8717 2023-05-05 15:19:28.000000 sdeclient-0.0.4/sdeclient/sdeutilities.py
+-rw-r--r--   0 bsawa      (501) staff       (20)     3462 2023-05-04 15:42:28.000000 sdeclient-0.0.4/sdeclient/simplelog.py
+drwxr-xr-x   0 bsawa      (501) staff       (20)        0 2023-05-05 15:19:31.544421 sdeclient-0.0.4/sdeclient.egg-info/
+-rw-r--r--   0 bsawa      (501) staff       (20)      527 2023-05-05 15:19:31.000000 sdeclient-0.0.4/sdeclient.egg-info/PKG-INFO
+-rw-r--r--   0 bsawa      (501) staff       (20)      234 2023-05-05 15:19:31.000000 sdeclient-0.0.4/sdeclient.egg-info/SOURCES.txt
+-rw-r--r--   0 bsawa      (501) staff       (20)        1 2023-05-05 15:19:31.000000 sdeclient-0.0.4/sdeclient.egg-info/dependency_links.txt
+-rw-r--r--   0 bsawa      (501) staff       (20)       10 2023-05-05 15:19:31.000000 sdeclient-0.0.4/sdeclient.egg-info/top_level.txt
+-rw-r--r--   0 bsawa      (501) staff       (20)       38 2023-05-05 15:19:31.545814 sdeclient-0.0.4/setup.cfg
+-rw-r--r--   0 bsawa      (501) staff       (20)      750 2023-05-05 15:19:25.000000 sdeclient-0.0.4/setup.py
```

### Comparing `sdeclient-0.0.3/PKG-INFO` & `sdeclient-0.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sdeclient
-Version: 0.0.3
+Version: 0.0.4
 Summary: Set of tools for SD Elements. The main platform developed by Security Compass
 Author: Scott McDowell & Brian Sawa
 Author-email: noahpop77@gmail.com
 Keywords: python,sde,SD Elements,tools
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `sdeclient-0.0.3/sdeclient/sdeclient.py` & `sdeclient-0.0.4/sdeclient/sdeclient.py`

 * *Files identical despite different names*

### Comparing `sdeclient-0.0.3/sdeclient/sdeutilities.py` & `sdeclient-0.0.4/sdeclient/sdeutilities.py`

 * *Files identical despite different names*

### Comparing `sdeclient-0.0.3/sdeclient/simplelog.py` & `sdeclient-0.0.4/sdeclient/simplelog.py`

 * *Files identical despite different names*

### Comparing `sdeclient-0.0.3/sdeclient.egg-info/PKG-INFO` & `sdeclient-0.0.4/sdeclient.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sdeclient
-Version: 0.0.3
+Version: 0.0.4
 Summary: Set of tools for SD Elements. The main platform developed by Security Compass
 Author: Scott McDowell & Brian Sawa
 Author-email: noahpop77@gmail.com
 Keywords: python,sde,SD Elements,tools
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `sdeclient-0.0.3/setup.py` & `sdeclient-0.0.4/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from setuptools import setup, find_packages
 import os
 
-VERSION = '0.0.3'
+VERSION = '0.0.4'
 DESCRIPTION = 'Set of tools for SD Elements. The main platform developed by Security Compass'
 
 # Setting up
 setup(
     name="sdeclient",
     version=VERSION,
     author="Scott McDowell & Brian Sawa",
```

