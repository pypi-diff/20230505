# Comparing `tmp/sdeclient-0.0.4.tar.gz` & `tmp/sdeclient-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sdeclient-0.0.4.tar", last modified: Fri May  5 15:19:31 2023, max compression
+gzip compressed data, was "sdeclient-0.0.5.tar", last modified: Fri May  5 15:30:31 2023, max compression
```

## Comparing `sdeclient-0.0.4.tar` & `sdeclient-0.0.5.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 bsawa      (501) staff       (20)        0 2023-05-05 15:19:31.545702 sdeclient-0.0.4/
--rw-r--r--   0 bsawa      (501) staff       (20)      527 2023-05-05 15:19:31.545319 sdeclient-0.0.4/PKG-INFO
-drwxr-xr-x   0 bsawa      (501) staff       (20)        0 2023-05-05 15:19:31.540962 sdeclient-0.0.4/sdeclient/
--rw-r--r--   0 bsawa      (501) staff       (20)        0 2023-05-05 15:19:26.000000 sdeclient-0.0.4/sdeclient/__init__.py
--rw-r--r--   0 bsawa      (501) staff       (20)    58272 2023-05-05 15:19:27.000000 sdeclient-0.0.4/sdeclient/sdeclient.py
--rw-r--r--   0 bsawa      (501) staff       (20)     8717 2023-05-05 15:19:28.000000 sdeclient-0.0.4/sdeclient/sdeutilities.py
--rw-r--r--   0 bsawa      (501) staff       (20)     3462 2023-05-04 15:42:28.000000 sdeclient-0.0.4/sdeclient/simplelog.py
-drwxr-xr-x   0 bsawa      (501) staff       (20)        0 2023-05-05 15:19:31.544421 sdeclient-0.0.4/sdeclient.egg-info/
--rw-r--r--   0 bsawa      (501) staff       (20)      527 2023-05-05 15:19:31.000000 sdeclient-0.0.4/sdeclient.egg-info/PKG-INFO
--rw-r--r--   0 bsawa      (501) staff       (20)      234 2023-05-05 15:19:31.000000 sdeclient-0.0.4/sdeclient.egg-info/SOURCES.txt
--rw-r--r--   0 bsawa      (501) staff       (20)        1 2023-05-05 15:19:31.000000 sdeclient-0.0.4/sdeclient.egg-info/dependency_links.txt
--rw-r--r--   0 bsawa      (501) staff       (20)       10 2023-05-05 15:19:31.000000 sdeclient-0.0.4/sdeclient.egg-info/top_level.txt
--rw-r--r--   0 bsawa      (501) staff       (20)       38 2023-05-05 15:19:31.545814 sdeclient-0.0.4/setup.cfg
--rw-r--r--   0 bsawa      (501) staff       (20)      750 2023-05-05 15:19:25.000000 sdeclient-0.0.4/setup.py
+drwxr-xr-x   0 bsawa      (501) staff       (20)        0 2023-05-05 15:30:31.626163 sdeclient-0.0.5/
+-rw-r--r--   0 bsawa      (501) staff       (20)      527 2023-05-05 15:30:31.625470 sdeclient-0.0.5/PKG-INFO
+drwxr-xr-x   0 bsawa      (501) staff       (20)        0 2023-05-05 15:30:31.620341 sdeclient-0.0.5/sdeclient/
+-rw-r--r--   0 bsawa      (501) staff       (20)        0 2023-05-05 15:19:26.000000 sdeclient-0.0.5/sdeclient/__init__.py
+-rw-r--r--   0 bsawa      (501) staff       (20)    58272 2023-05-05 15:19:27.000000 sdeclient-0.0.5/sdeclient/sdeclient.py
+-rw-r--r--   0 bsawa      (501) staff       (20)     8701 2023-05-05 15:28:13.000000 sdeclient-0.0.5/sdeclient/sdeutilities.py
+-rw-r--r--   0 bsawa      (501) staff       (20)     3454 2023-05-05 15:30:01.000000 sdeclient-0.0.5/sdeclient/simplelogging.py
+drwxr-xr-x   0 bsawa      (501) staff       (20)        0 2023-05-05 15:30:31.624685 sdeclient-0.0.5/sdeclient.egg-info/
+-rw-r--r--   0 bsawa      (501) staff       (20)      527 2023-05-05 15:30:31.000000 sdeclient-0.0.5/sdeclient.egg-info/PKG-INFO
+-rw-r--r--   0 bsawa      (501) staff       (20)      238 2023-05-05 15:30:31.000000 sdeclient-0.0.5/sdeclient.egg-info/SOURCES.txt
+-rw-r--r--   0 bsawa      (501) staff       (20)        1 2023-05-05 15:30:31.000000 sdeclient-0.0.5/sdeclient.egg-info/dependency_links.txt
+-rw-r--r--   0 bsawa      (501) staff       (20)       10 2023-05-05 15:30:31.000000 sdeclient-0.0.5/sdeclient.egg-info/top_level.txt
+-rw-r--r--   0 bsawa      (501) staff       (20)       38 2023-05-05 15:30:31.626324 sdeclient-0.0.5/setup.cfg
+-rw-r--r--   0 bsawa      (501) staff       (20)      750 2023-05-05 15:30:25.000000 sdeclient-0.0.5/setup.py
```

### Comparing `sdeclient-0.0.4/PKG-INFO` & `sdeclient-0.0.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sdeclient
-Version: 0.0.4
+Version: 0.0.5
 Summary: Set of tools for SD Elements. The main platform developed by Security Compass
 Author: Scott McDowell & Brian Sawa
 Author-email: noahpop77@gmail.com
 Keywords: python,sde,SD Elements,tools
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `sdeclient-0.0.4/sdeclient/sdeclient.py` & `sdeclient-0.0.5/sdeclient/sdeclient.py`

 * *Files identical despite different names*

### Comparing `sdeclient-0.0.4/sdeclient/sdeutilities.py` & `sdeclient-0.0.5/sdeclient/sdeutilities.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,15 +27,15 @@
 import csv
 import json
 import os
 import re
 from zipfile import ZipFile
 
 
-class SdeUtilities:
+class sdeutils:
     """
     Collection of static utility methods for use with SdeClient.
     """
 
     @staticmethod
     def get_bool_from_string(boolean_string):
         """
@@ -149,24 +149,24 @@
 
     @staticmethod
     def get_string_list_from_csv(csv_string):
         """
         Get list of string values from CSV string.
         Returns empty list when csv_string is empty.
         """
-        return SdeUtilities.get_string_list_from_separated_string(csv_string, ",")
+        return sdeutils.get_string_list_from_separated_string(csv_string, ",")
 
     @staticmethod
     def get_int_list_from_csv(csv_string):
         """
         Get list of int values from CSV string.
         """
         return [int(value)
                 for value
-                in SdeUtilities.get_string_list_from_csv(csv_string)]
+                in sdeutils.get_string_list_from_csv(csv_string)]
 
     @staticmethod
     def get_unique_item_list_from_lists(first_list, second_list):
         """
         Get a list of unique items from two lists that may included duplicates.
         """
         first_set = set(first_list)
@@ -174,15 +174,15 @@
         return list(first_set) + list(second_set - first_set)
 
     @staticmethod
     def get_dictionary_from_collection_with_ids(collection):
         """
         Get dictionary of objects with "id" value as key.
         """
-        return SdeUtilities.get_dictionary_from_collection_with_key(
+        return sdeutils.get_dictionary_from_collection_with_key(
             collection, "id"
         )
 
     @staticmethod
     def get_dictionary_from_collection_with_key(collection, key_name):
         """
         Get dictionary of objects with key_name value as key.
```

### Comparing `sdeclient-0.0.4/sdeclient/simplelog.py` & `sdeclient-0.0.5/sdeclient/simplelogging.py`

 * *Files 2% similar despite different names*

```diff
@@ -19,15 +19,15 @@
              used, for example LANG=en_US (ISO8859-1/latin-1).
 """
 
 
 import sys
 from datetime import datetime
 
-from sdeutilities import SdeUtilities
+from sdeutilities import sdeutils
 
 
 class SimpleLog:
     """
     Simple text log class.
     """
 
@@ -98,9 +98,9 @@
         self.add_line(1, f"Exception: {exception}")
 
     def write_log_file(self):
         """
         Write contents of the log to a CSV file.
         """
         if self.output_filename is not None:
-            SdeUtilities.write_report_lines_to_file(self.lines,
+            sdeutils.write_report_lines_to_file(self.lines,
                                                     self.output_filename)
```

### Comparing `sdeclient-0.0.4/sdeclient.egg-info/PKG-INFO` & `sdeclient-0.0.5/sdeclient.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sdeclient
-Version: 0.0.4
+Version: 0.0.5
 Summary: Set of tools for SD Elements. The main platform developed by Security Compass
 Author: Scott McDowell & Brian Sawa
 Author-email: noahpop77@gmail.com
 Keywords: python,sde,SD Elements,tools
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `sdeclient-0.0.4/setup.py` & `sdeclient-0.0.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from setuptools import setup, find_packages
 import os
 
-VERSION = '0.0.4'
+VERSION = '0.0.5'
 DESCRIPTION = 'Set of tools for SD Elements. The main platform developed by Security Compass'
 
 # Setting up
 setup(
     name="sdeclient",
     version=VERSION,
     author="Scott McDowell & Brian Sawa",
```

