# Comparing `tmp/sdeclient-0.0.8.tar.gz` & `tmp/sdeclient-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sdeclient-0.0.8.tar", last modified: Fri May  5 15:43:24 2023, max compression
+gzip compressed data, was "sdeclient-0.0.9.tar", last modified: Fri May  5 15:46:33 2023, max compression
```

## Comparing `sdeclient-0.0.8.tar` & `sdeclient-0.0.9.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 bsawa      (501) staff       (20)        0 2023-05-05 15:43:24.706853 sdeclient-0.0.8/
--rw-r--r--   0 bsawa      (501) staff       (20)      527 2023-05-05 15:43:24.705959 sdeclient-0.0.8/PKG-INFO
-drwxr-xr-x   0 bsawa      (501) staff       (20)        0 2023-05-05 15:43:24.691514 sdeclient-0.0.8/sdeclient/
--rw-r--r--   0 bsawa      (501) staff       (20)       72 2023-05-05 15:42:42.000000 sdeclient-0.0.8/sdeclient/__init__.py
--rw-r--r--   0 bsawa      (501) staff       (20)    58239 2023-05-05 15:42:56.000000 sdeclient-0.0.8/sdeclient/sdeclient.py
--rw-r--r--   0 bsawa      (501) staff       (20)     8701 2023-05-05 15:38:34.000000 sdeclient-0.0.8/sdeclient/sdeutilities.py
--rw-r--r--   0 bsawa      (501) staff       (20)     3454 2023-05-05 15:38:36.000000 sdeclient-0.0.8/sdeclient/simplelogging.py
-drwxr-xr-x   0 bsawa      (501) staff       (20)        0 2023-05-05 15:43:24.700458 sdeclient-0.0.8/sdeclient.egg-info/
--rw-r--r--   0 bsawa      (501) staff       (20)      527 2023-05-05 15:43:24.000000 sdeclient-0.0.8/sdeclient.egg-info/PKG-INFO
--rw-r--r--   0 bsawa      (501) staff       (20)      238 2023-05-05 15:43:24.000000 sdeclient-0.0.8/sdeclient.egg-info/SOURCES.txt
--rw-r--r--   0 bsawa      (501) staff       (20)        1 2023-05-05 15:43:24.000000 sdeclient-0.0.8/sdeclient.egg-info/dependency_links.txt
--rw-r--r--   0 bsawa      (501) staff       (20)       10 2023-05-05 15:43:24.000000 sdeclient-0.0.8/sdeclient.egg-info/top_level.txt
--rw-r--r--   0 bsawa      (501) staff       (20)       38 2023-05-05 15:43:24.707209 sdeclient-0.0.8/setup.cfg
--rw-r--r--   0 bsawa      (501) staff       (20)      750 2023-05-05 15:43:01.000000 sdeclient-0.0.8/setup.py
+drwxr-xr-x   0 bsawa      (501) staff       (20)        0 2023-05-05 15:46:33.422130 sdeclient-0.0.9/
+-rw-r--r--   0 bsawa      (501) staff       (20)      527 2023-05-05 15:46:33.421734 sdeclient-0.0.9/PKG-INFO
+drwxr-xr-x   0 bsawa      (501) staff       (20)        0 2023-05-05 15:46:33.416925 sdeclient-0.0.9/sdeclient/
+-rw-r--r--   0 bsawa      (501) staff       (20)       66 2023-05-05 15:45:52.000000 sdeclient-0.0.9/sdeclient/__init__.py
+-rw-r--r--   0 bsawa      (501) staff       (20)    58239 2023-05-05 15:42:56.000000 sdeclient-0.0.9/sdeclient/sdeclient.py
+-rw-r--r--   0 bsawa      (501) staff       (20)     3452 2023-05-05 15:46:09.000000 sdeclient-0.0.9/sdeclient/sdelogging.py
+-rw-r--r--   0 bsawa      (501) staff       (20)     8701 2023-05-05 15:38:34.000000 sdeclient-0.0.9/sdeclient/sdeutilities.py
+drwxr-xr-x   0 bsawa      (501) staff       (20)        0 2023-05-05 15:46:33.420839 sdeclient-0.0.9/sdeclient.egg-info/
+-rw-r--r--   0 bsawa      (501) staff       (20)      527 2023-05-05 15:46:33.000000 sdeclient-0.0.9/sdeclient.egg-info/PKG-INFO
+-rw-r--r--   0 bsawa      (501) staff       (20)      235 2023-05-05 15:46:33.000000 sdeclient-0.0.9/sdeclient.egg-info/SOURCES.txt
+-rw-r--r--   0 bsawa      (501) staff       (20)        1 2023-05-05 15:46:33.000000 sdeclient-0.0.9/sdeclient.egg-info/dependency_links.txt
+-rw-r--r--   0 bsawa      (501) staff       (20)       10 2023-05-05 15:46:33.000000 sdeclient-0.0.9/sdeclient.egg-info/top_level.txt
+-rw-r--r--   0 bsawa      (501) staff       (20)       38 2023-05-05 15:46:33.422286 sdeclient-0.0.9/setup.cfg
+-rw-r--r--   0 bsawa      (501) staff       (20)      750 2023-05-05 15:46:20.000000 sdeclient-0.0.9/setup.py
```

### Comparing `sdeclient-0.0.8/PKG-INFO` & `sdeclient-0.0.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sdeclient
-Version: 0.0.8
+Version: 0.0.9
 Summary: Set of tools for SD Elements. The main platform developed by Security Compass
 Author: Scott McDowell & Brian Sawa
 Author-email: noahpop77@gmail.com
 Keywords: python,sde,SD Elements,tools
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `sdeclient-0.0.8/sdeclient/sdeclient.py` & `sdeclient-0.0.9/sdeclient/sdeclient.py`

 * *Files identical despite different names*

### Comparing `sdeclient-0.0.8/sdeclient/sdeutilities.py` & `sdeclient-0.0.9/sdeclient/sdeutilities.py`

 * *Files identical despite different names*

### Comparing `sdeclient-0.0.8/sdeclient/simplelogging.py` & `sdeclient-0.0.9/sdeclient/sdelogging.py`

 * *Files 1% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 
 import sys
 from datetime import datetime
 
 from sdeutilities import sdeutils
 
 
-class simpleLog:
+class sdelogs:
     """
     Simple text log class.
     """
 
     def __init__(self, debug_mode=False, output_filename=None,
                  print_timestamps=True):
         assert isinstance(debug_mode, bool)
```

### Comparing `sdeclient-0.0.8/sdeclient.egg-info/PKG-INFO` & `sdeclient-0.0.9/sdeclient.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sdeclient
-Version: 0.0.8
+Version: 0.0.9
 Summary: Set of tools for SD Elements. The main platform developed by Security Compass
 Author: Scott McDowell & Brian Sawa
 Author-email: noahpop77@gmail.com
 Keywords: python,sde,SD Elements,tools
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `sdeclient-0.0.8/setup.py` & `sdeclient-0.0.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from setuptools import setup, find_packages
 import os
 
-VERSION = '0.0.8'
+VERSION = '0.0.9'
 DESCRIPTION = 'Set of tools for SD Elements. The main platform developed by Security Compass'
 
 # Setting up
 setup(
     name="sdeclient",
     version=VERSION,
     author="Scott McDowell & Brian Sawa",
```

