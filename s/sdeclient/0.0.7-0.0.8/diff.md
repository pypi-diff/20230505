# Comparing `tmp/sdeclient-0.0.7.tar.gz` & `tmp/sdeclient-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sdeclient-0.0.7.tar", last modified: Fri May  5 15:38:49 2023, max compression
+gzip compressed data, was "sdeclient-0.0.8.tar", last modified: Fri May  5 15:43:24 2023, max compression
```

## Comparing `sdeclient-0.0.7.tar` & `sdeclient-0.0.8.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 bsawa      (501) staff       (20)        0 2023-05-05 15:38:49.501934 sdeclient-0.0.7/
--rw-r--r--   0 bsawa      (501) staff       (20)      527 2023-05-05 15:38:49.501400 sdeclient-0.0.7/PKG-INFO
-drwxr-xr-x   0 bsawa      (501) staff       (20)        0 2023-05-05 15:38:49.497019 sdeclient-0.0.7/sdeclient/
--rw-r--r--   0 bsawa      (501) staff       (20)       96 2023-05-05 15:38:32.000000 sdeclient-0.0.7/sdeclient/__init__.py
--rw-r--r--   0 bsawa      (501) staff       (20)    58246 2023-05-05 15:38:31.000000 sdeclient-0.0.7/sdeclient/sdeclient.py
--rw-r--r--   0 bsawa      (501) staff       (20)     8701 2023-05-05 15:38:34.000000 sdeclient-0.0.7/sdeclient/sdeutilities.py
--rw-r--r--   0 bsawa      (501) staff       (20)     3454 2023-05-05 15:38:36.000000 sdeclient-0.0.7/sdeclient/simplelogging.py
-drwxr-xr-x   0 bsawa      (501) staff       (20)        0 2023-05-05 15:38:49.500450 sdeclient-0.0.7/sdeclient.egg-info/
--rw-r--r--   0 bsawa      (501) staff       (20)      527 2023-05-05 15:38:49.000000 sdeclient-0.0.7/sdeclient.egg-info/PKG-INFO
--rw-r--r--   0 bsawa      (501) staff       (20)      238 2023-05-05 15:38:49.000000 sdeclient-0.0.7/sdeclient.egg-info/SOURCES.txt
--rw-r--r--   0 bsawa      (501) staff       (20)        1 2023-05-05 15:38:49.000000 sdeclient-0.0.7/sdeclient.egg-info/dependency_links.txt
--rw-r--r--   0 bsawa      (501) staff       (20)       10 2023-05-05 15:38:49.000000 sdeclient-0.0.7/sdeclient.egg-info/top_level.txt
--rw-r--r--   0 bsawa      (501) staff       (20)       38 2023-05-05 15:38:49.502074 sdeclient-0.0.7/setup.cfg
--rw-r--r--   0 bsawa      (501) staff       (20)      750 2023-05-05 15:38:29.000000 sdeclient-0.0.7/setup.py
+drwxr-xr-x   0 bsawa      (501) staff       (20)        0 2023-05-05 15:43:24.706853 sdeclient-0.0.8/
+-rw-r--r--   0 bsawa      (501) staff       (20)      527 2023-05-05 15:43:24.705959 sdeclient-0.0.8/PKG-INFO
+drwxr-xr-x   0 bsawa      (501) staff       (20)        0 2023-05-05 15:43:24.691514 sdeclient-0.0.8/sdeclient/
+-rw-r--r--   0 bsawa      (501) staff       (20)       72 2023-05-05 15:42:42.000000 sdeclient-0.0.8/sdeclient/__init__.py
+-rw-r--r--   0 bsawa      (501) staff       (20)    58239 2023-05-05 15:42:56.000000 sdeclient-0.0.8/sdeclient/sdeclient.py
+-rw-r--r--   0 bsawa      (501) staff       (20)     8701 2023-05-05 15:38:34.000000 sdeclient-0.0.8/sdeclient/sdeutilities.py
+-rw-r--r--   0 bsawa      (501) staff       (20)     3454 2023-05-05 15:38:36.000000 sdeclient-0.0.8/sdeclient/simplelogging.py
+drwxr-xr-x   0 bsawa      (501) staff       (20)        0 2023-05-05 15:43:24.700458 sdeclient-0.0.8/sdeclient.egg-info/
+-rw-r--r--   0 bsawa      (501) staff       (20)      527 2023-05-05 15:43:24.000000 sdeclient-0.0.8/sdeclient.egg-info/PKG-INFO
+-rw-r--r--   0 bsawa      (501) staff       (20)      238 2023-05-05 15:43:24.000000 sdeclient-0.0.8/sdeclient.egg-info/SOURCES.txt
+-rw-r--r--   0 bsawa      (501) staff       (20)        1 2023-05-05 15:43:24.000000 sdeclient-0.0.8/sdeclient.egg-info/dependency_links.txt
+-rw-r--r--   0 bsawa      (501) staff       (20)       10 2023-05-05 15:43:24.000000 sdeclient-0.0.8/sdeclient.egg-info/top_level.txt
+-rw-r--r--   0 bsawa      (501) staff       (20)       38 2023-05-05 15:43:24.707209 sdeclient-0.0.8/setup.cfg
+-rw-r--r--   0 bsawa      (501) staff       (20)      750 2023-05-05 15:43:01.000000 sdeclient-0.0.8/setup.py
```

### Comparing `sdeclient-0.0.7/PKG-INFO` & `sdeclient-0.0.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sdeclient
-Version: 0.0.7
+Version: 0.0.8
 Summary: Set of tools for SD Elements. The main platform developed by Security Compass
 Author: Scott McDowell & Brian Sawa
 Author-email: noahpop77@gmail.com
 Keywords: python,sde,SD Elements,tools
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `sdeclient-0.0.7/sdeclient/sdeclient.py` & `sdeclient-0.0.8/sdeclient/sdeclient.py`

 * *Files 0% similar despite different names*

```diff
@@ -72,53 +72,46 @@
              include archived projects in its response.
 2023-03-07 - Added get_business_units, get_business_unit, delete_project,
              delete_application, and delete_business_unit methods.
 
 #endregion Change Log
 """
 
-
 # Fall back to single-threaded pagination.
 try:
     from multiprocessing.pool import ThreadPool
 except:
     single_threaded_fallback = True
 else:
     single_threaded_fallback = False
 
 # https://pyyaml.org/
 # https://pypi.org/project/PyYAML/
 import yaml
-
 # https://requests.readthedocs.io/
 # https://pypi.org/project/requests/
 import requests
 from requests.adapters import HTTPAdapter
-
 # Verification warnings are disabled for individual requests to avoid flooding
 # the console. Add your own warning when you create an instance of SdeClient
 # with verify=false to notify the user.
 from requests.packages import urllib3
 urllib3.disable_warnings(urllib3.exceptions.InsecureRequestWarning)
-
 from urllib3.util.retry import Retry
-
 # Used to shim requests module's Session 'request' function to set a default
 # timeout value for all request methods.
 # Reference: https://stackoverflow.com/a/59317604
 import functools
-
 # Sleep method used to implement polling for job completion.
 import time
-
 # Datetime used to determine whether the Cube API JWT requires a refresh.
 from datetime import datetime
-
 import json
 
+
 from sdeutilities import sdeutils
 
 
 class sde:
     """
     Simple SD Elements API client that uses the requests library.
     """
```

### Comparing `sdeclient-0.0.7/sdeclient/sdeutilities.py` & `sdeclient-0.0.8/sdeclient/sdeutilities.py`

 * *Files identical despite different names*

### Comparing `sdeclient-0.0.7/sdeclient/simplelogging.py` & `sdeclient-0.0.8/sdeclient/simplelogging.py`

 * *Files identical despite different names*

### Comparing `sdeclient-0.0.7/sdeclient.egg-info/PKG-INFO` & `sdeclient-0.0.8/sdeclient.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sdeclient
-Version: 0.0.7
+Version: 0.0.8
 Summary: Set of tools for SD Elements. The main platform developed by Security Compass
 Author: Scott McDowell & Brian Sawa
 Author-email: noahpop77@gmail.com
 Keywords: python,sde,SD Elements,tools
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `sdeclient-0.0.7/setup.py` & `sdeclient-0.0.8/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from setuptools import setup, find_packages
 import os
 
-VERSION = '0.0.7'
+VERSION = '0.0.8'
 DESCRIPTION = 'Set of tools for SD Elements. The main platform developed by Security Compass'
 
 # Setting up
 setup(
     name="sdeclient",
     version=VERSION,
     author="Scott McDowell & Brian Sawa",
```

