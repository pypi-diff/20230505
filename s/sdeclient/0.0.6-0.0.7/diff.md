# Comparing `tmp/sdeclient-0.0.6.tar.gz` & `tmp/sdeclient-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sdeclient-0.0.6.tar", last modified: Fri May  5 15:34:32 2023, max compression
+gzip compressed data, was "sdeclient-0.0.7.tar", last modified: Fri May  5 15:38:49 2023, max compression
```

## Comparing `sdeclient-0.0.6.tar` & `sdeclient-0.0.7.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 bsawa      (501) staff       (20)        0 2023-05-05 15:34:32.924281 sdeclient-0.0.6/
--rw-r--r--   0 bsawa      (501) staff       (20)      527 2023-05-05 15:34:32.923707 sdeclient-0.0.6/PKG-INFO
-drwxr-xr-x   0 bsawa      (501) staff       (20)        0 2023-05-05 15:34:32.910207 sdeclient-0.0.6/sdeclient/
--rw-r--r--   0 bsawa      (501) staff       (20)       95 2023-05-05 15:34:10.000000 sdeclient-0.0.6/sdeclient/__init__.py
--rw-r--r--   0 bsawa      (501) staff       (20)    58246 2023-05-05 15:32:59.000000 sdeclient-0.0.6/sdeclient/sdeclient.py
--rw-r--r--   0 bsawa      (501) staff       (20)     8701 2023-05-05 15:28:13.000000 sdeclient-0.0.6/sdeclient/sdeutilities.py
--rw-r--r--   0 bsawa      (501) staff       (20)     3454 2023-05-05 15:33:26.000000 sdeclient-0.0.6/sdeclient/simplelogging.py
-drwxr-xr-x   0 bsawa      (501) staff       (20)        0 2023-05-05 15:34:32.922477 sdeclient-0.0.6/sdeclient.egg-info/
--rw-r--r--   0 bsawa      (501) staff       (20)      527 2023-05-05 15:34:32.000000 sdeclient-0.0.6/sdeclient.egg-info/PKG-INFO
--rw-r--r--   0 bsawa      (501) staff       (20)      238 2023-05-05 15:34:32.000000 sdeclient-0.0.6/sdeclient.egg-info/SOURCES.txt
--rw-r--r--   0 bsawa      (501) staff       (20)        1 2023-05-05 15:34:32.000000 sdeclient-0.0.6/sdeclient.egg-info/dependency_links.txt
--rw-r--r--   0 bsawa      (501) staff       (20)       10 2023-05-05 15:34:32.000000 sdeclient-0.0.6/sdeclient.egg-info/top_level.txt
--rw-r--r--   0 bsawa      (501) staff       (20)       38 2023-05-05 15:34:32.924478 sdeclient-0.0.6/setup.cfg
--rw-r--r--   0 bsawa      (501) staff       (20)      750 2023-05-05 15:33:44.000000 sdeclient-0.0.6/setup.py
+drwxr-xr-x   0 bsawa      (501) staff       (20)        0 2023-05-05 15:38:49.501934 sdeclient-0.0.7/
+-rw-r--r--   0 bsawa      (501) staff       (20)      527 2023-05-05 15:38:49.501400 sdeclient-0.0.7/PKG-INFO
+drwxr-xr-x   0 bsawa      (501) staff       (20)        0 2023-05-05 15:38:49.497019 sdeclient-0.0.7/sdeclient/
+-rw-r--r--   0 bsawa      (501) staff       (20)       96 2023-05-05 15:38:32.000000 sdeclient-0.0.7/sdeclient/__init__.py
+-rw-r--r--   0 bsawa      (501) staff       (20)    58246 2023-05-05 15:38:31.000000 sdeclient-0.0.7/sdeclient/sdeclient.py
+-rw-r--r--   0 bsawa      (501) staff       (20)     8701 2023-05-05 15:38:34.000000 sdeclient-0.0.7/sdeclient/sdeutilities.py
+-rw-r--r--   0 bsawa      (501) staff       (20)     3454 2023-05-05 15:38:36.000000 sdeclient-0.0.7/sdeclient/simplelogging.py
+drwxr-xr-x   0 bsawa      (501) staff       (20)        0 2023-05-05 15:38:49.500450 sdeclient-0.0.7/sdeclient.egg-info/
+-rw-r--r--   0 bsawa      (501) staff       (20)      527 2023-05-05 15:38:49.000000 sdeclient-0.0.7/sdeclient.egg-info/PKG-INFO
+-rw-r--r--   0 bsawa      (501) staff       (20)      238 2023-05-05 15:38:49.000000 sdeclient-0.0.7/sdeclient.egg-info/SOURCES.txt
+-rw-r--r--   0 bsawa      (501) staff       (20)        1 2023-05-05 15:38:49.000000 sdeclient-0.0.7/sdeclient.egg-info/dependency_links.txt
+-rw-r--r--   0 bsawa      (501) staff       (20)       10 2023-05-05 15:38:49.000000 sdeclient-0.0.7/sdeclient.egg-info/top_level.txt
+-rw-r--r--   0 bsawa      (501) staff       (20)       38 2023-05-05 15:38:49.502074 sdeclient-0.0.7/setup.cfg
+-rw-r--r--   0 bsawa      (501) staff       (20)      750 2023-05-05 15:38:29.000000 sdeclient-0.0.7/setup.py
```

### Comparing `sdeclient-0.0.6/PKG-INFO` & `sdeclient-0.0.7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sdeclient
-Version: 0.0.6
+Version: 0.0.7
 Summary: Set of tools for SD Elements. The main platform developed by Security Compass
 Author: Scott McDowell & Brian Sawa
 Author-email: noahpop77@gmail.com
 Keywords: python,sde,SD Elements,tools
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `sdeclient-0.0.6/sdeclient/sdeclient.py` & `sdeclient-0.0.7/sdeclient/sdeclient.py`

 * *Files identical despite different names*

### Comparing `sdeclient-0.0.6/sdeclient/sdeutilities.py` & `sdeclient-0.0.7/sdeclient/sdeutilities.py`

 * *Files identical despite different names*

### Comparing `sdeclient-0.0.6/sdeclient/simplelogging.py` & `sdeclient-0.0.7/sdeclient/simplelogging.py`

 * *Files identical despite different names*

### Comparing `sdeclient-0.0.6/sdeclient.egg-info/PKG-INFO` & `sdeclient-0.0.7/sdeclient.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sdeclient
-Version: 0.0.6
+Version: 0.0.7
 Summary: Set of tools for SD Elements. The main platform developed by Security Compass
 Author: Scott McDowell & Brian Sawa
 Author-email: noahpop77@gmail.com
 Keywords: python,sde,SD Elements,tools
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `sdeclient-0.0.6/setup.py` & `sdeclient-0.0.7/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from setuptools import setup, find_packages
 import os
 
-VERSION = '0.0.6'
+VERSION = '0.0.7'
 DESCRIPTION = 'Set of tools for SD Elements. The main platform developed by Security Compass'
 
 # Setting up
 setup(
     name="sdeclient",
     version=VERSION,
     author="Scott McDowell & Brian Sawa",
```

