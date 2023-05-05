# Comparing `tmp/CSV to JSON Python-0.0.1.tar.gz` & `tmp/CSV to JSON Python-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "CSV to JSON Python-0.0.1.tar", last modified: Fri May  5 19:16:37 2023, max compression
+gzip compressed data, was "CSV to JSON Python-0.0.2.tar", last modified: Fri May  5 20:04:12 2023, max compression
```

## Comparing `CSV to JSON Python-0.0.1.tar` & `CSV to JSON Python-0.0.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 dabolabs   (504) staff       (20)        0 2023-05-05 19:16:37.896866 CSV to JSON Python-0.0.1/
--rw-r--r--   0 dabolabs   (504) staff       (20)     1068 2023-05-05 18:43:08.000000 CSV to JSON Python-0.0.1/LICENSE.txt
--rw-r--r--   0 dabolabs   (504) staff       (20)      556 2023-05-05 19:16:37.897106 CSV to JSON Python-0.0.1/PKG-INFO
--rw-r--r--   0 dabolabs   (504) staff       (20)        0 2023-05-05 18:37:30.000000 CSV to JSON Python-0.0.1/README.md
--rw-r--r--   0 dabolabs   (504) staff       (20)       84 2023-05-05 18:42:44.000000 CSV to JSON Python-0.0.1/pyproject.toml
--rw-r--r--   0 dabolabs   (504) staff       (20)      627 2023-05-05 19:16:37.898207 CSV to JSON Python-0.0.1/setup.cfg
--rw-r--r--   0 dabolabs   (504) staff       (20)      879 2023-05-05 19:16:09.000000 CSV to JSON Python-0.0.1/setup.py
-drwxr-xr-x   0 dabolabs   (504) staff       (20)        0 2023-05-05 19:16:37.885053 CSV to JSON Python-0.0.1/src/
-drwxr-xr-x   0 dabolabs   (504) staff       (20)        0 2023-05-05 19:16:37.892074 CSV to JSON Python-0.0.1/src/CSV_to_JSON_Python.egg-info/
--rw-r--r--   0 dabolabs   (504) staff       (20)      556 2023-05-05 19:16:37.000000 CSV to JSON Python-0.0.1/src/CSV_to_JSON_Python.egg-info/PKG-INFO
--rw-r--r--   0 dabolabs   (504) staff       (20)      298 2023-05-05 19:16:37.000000 CSV to JSON Python-0.0.1/src/CSV_to_JSON_Python.egg-info/SOURCES.txt
--rw-r--r--   0 dabolabs   (504) staff       (20)        1 2023-05-05 19:16:37.000000 CSV to JSON Python-0.0.1/src/CSV_to_JSON_Python.egg-info/dependency_links.txt
--rw-r--r--   0 dabolabs   (504) staff       (20)       12 2023-05-05 19:16:37.000000 CSV to JSON Python-0.0.1/src/CSV_to_JSON_Python.egg-info/top_level.txt
-drwxr-xr-x   0 dabolabs   (504) staff       (20)        0 2023-05-05 19:16:37.893358 CSV to JSON Python-0.0.1/src/csv_to_json/
--rw-r--r--   0 dabolabs   (504) staff       (20)        0 2023-05-05 18:41:15.000000 CSV to JSON Python-0.0.1/src/csv_to_json/__init__.py
--rw-r--r--   0 dabolabs   (504) staff       (20)       54 2023-05-05 18:41:17.000000 CSV to JSON Python-0.0.1/src/csv_to_json/hello_world.py
+drwxr-xr-x   0 dabolabs   (504) staff       (20)        0 2023-05-05 20:04:12.995422 CSV to JSON Python-0.0.2/
+-rw-r--r--   0 dabolabs   (504) staff       (20)     1068 2023-05-05 18:43:08.000000 CSV to JSON Python-0.0.2/LICENSE.txt
+-rw-r--r--   0 dabolabs   (504) staff       (20)      556 2023-05-05 20:04:12.995682 CSV to JSON Python-0.0.2/PKG-INFO
+-rw-r--r--   0 dabolabs   (504) staff       (20)        0 2023-05-05 18:37:30.000000 CSV to JSON Python-0.0.2/README.md
+-rw-r--r--   0 dabolabs   (504) staff       (20)       84 2023-05-05 18:42:44.000000 CSV to JSON Python-0.0.2/pyproject.toml
+-rw-r--r--   0 dabolabs   (504) staff       (20)      627 2023-05-05 20:04:12.996998 CSV to JSON Python-0.0.2/setup.cfg
+-rw-r--r--   0 dabolabs   (504) staff       (20)      879 2023-05-05 20:03:57.000000 CSV to JSON Python-0.0.2/setup.py
+drwxr-xr-x   0 dabolabs   (504) staff       (20)        0 2023-05-05 20:04:12.983223 CSV to JSON Python-0.0.2/src/
+drwxr-xr-x   0 dabolabs   (504) staff       (20)        0 2023-05-05 20:04:12.990661 CSV to JSON Python-0.0.2/src/CSV_to_JSON_Python.egg-info/
+-rw-r--r--   0 dabolabs   (504) staff       (20)      556 2023-05-05 20:04:12.000000 CSV to JSON Python-0.0.2/src/CSV_to_JSON_Python.egg-info/PKG-INFO
+-rw-r--r--   0 dabolabs   (504) staff       (20)      298 2023-05-05 20:04:12.000000 CSV to JSON Python-0.0.2/src/CSV_to_JSON_Python.egg-info/SOURCES.txt
+-rw-r--r--   0 dabolabs   (504) staff       (20)        1 2023-05-05 20:04:12.000000 CSV to JSON Python-0.0.2/src/CSV_to_JSON_Python.egg-info/dependency_links.txt
+-rw-r--r--   0 dabolabs   (504) staff       (20)       12 2023-05-05 20:04:12.000000 CSV to JSON Python-0.0.2/src/CSV_to_JSON_Python.egg-info/top_level.txt
+drwxr-xr-x   0 dabolabs   (504) staff       (20)        0 2023-05-05 20:04:12.991781 CSV to JSON Python-0.0.2/src/csv_to_json/
+-rw-r--r--   0 dabolabs   (504) staff       (20)        0 2023-05-05 18:41:15.000000 CSV to JSON Python-0.0.2/src/csv_to_json/__init__.py
+-rw-r--r--   0 dabolabs   (504) staff       (20)      143 2023-05-05 19:53:54.000000 CSV to JSON Python-0.0.2/src/csv_to_json/hello_world.py
```

### Comparing `CSV to JSON Python-0.0.1/LICENSE.txt` & `CSV to JSON Python-0.0.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `CSV to JSON Python-0.0.1/PKG-INFO` & `CSV to JSON Python-0.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: CSV to JSON Python
-Version: 0.0.1
+Version: 0.0.2
 Summary: This is a package used to convert csv data to a json object
 Home-page: https://testpypi.org/project/CSV to JSON Python/
 Author: Paul Ndambo
 Author-email: paulkadabo@gmail.com
 Project-URL: Bug Tracker, https://testpypi.org/project/CSV to JSON Python/
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `CSV to JSON Python-0.0.1/setup.cfg` & `CSV to JSON Python-0.0.2/setup.cfg`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = CSV to JSON Python
-version = 0.0.1
+version = 0.0.2
 author = Paul Ndambo
 author_email = author@example.com
 description = This is a package used to convert csv data to a json object
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://testpypi.org/project/CSV to JSON Python/
 project_urls =
```

### Comparing `CSV to JSON Python-0.0.1/setup.py` & `CSV to JSON Python-0.0.2/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding = "utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name = "CSV to JSON Python",
-    version = "0.0.1",
+    version = "0.0.2",
     author = "Paul Ndambo",
     author_email = "paulkadabo@gmail.com",
     description = "This is a package used to convert csv data to a json object",
     long_description = long_description,
     long_description_content_type = "text/markdown",
     url = "https://testpypi.org/project/CSV to JSON Python/",
     project_urls = {
```

### Comparing `CSV to JSON Python-0.0.1/src/CSV_to_JSON_Python.egg-info/PKG-INFO` & `CSV to JSON Python-0.0.2/src/CSV_to_JSON_Python.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: CSV-to-JSON-Python
-Version: 0.0.1
+Version: 0.0.2
 Summary: This is a package used to convert csv data to a json object
 Home-page: https://testpypi.org/project/CSV to JSON Python/
 Author: Paul Ndambo
 Author-email: paulkadabo@gmail.com
 Project-URL: Bug Tracker, https://testpypi.org/project/CSV to JSON Python/
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

