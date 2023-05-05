# Comparing `tmp/CSV to JSON Python-0.0.3.tar.gz` & `tmp/CSV to JSON Python-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "CSV to JSON Python-0.0.3.tar", last modified: Fri May  5 20:08:14 2023, max compression
+gzip compressed data, was "/home/runner/work/CSV-to-JSON-PyPI/CSV-to-JSON-PyPI/dist/.tmp-_1190w1m/CSV to JSON Python-0.0.4.tar", last modified: Fri May  5 20:46:13 2023, max compression
```

## Comparing `CSV to JSON Python-0.0.3.tar` & `CSV to JSON Python-0.0.4.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 dabolabs   (504) staff       (20)        0 2023-05-05 20:08:14.771237 CSV to JSON Python-0.0.3/
--rw-r--r--   0 dabolabs   (504) staff       (20)     1068 2023-05-05 18:43:08.000000 CSV to JSON Python-0.0.3/LICENSE.txt
--rw-r--r--   0 dabolabs   (504) staff       (20)      556 2023-05-05 20:08:14.771630 CSV to JSON Python-0.0.3/PKG-INFO
--rw-r--r--   0 dabolabs   (504) staff       (20)        0 2023-05-05 18:37:30.000000 CSV to JSON Python-0.0.3/README.md
--rw-r--r--   0 dabolabs   (504) staff       (20)       84 2023-05-05 18:42:44.000000 CSV to JSON Python-0.0.3/pyproject.toml
--rw-r--r--   0 dabolabs   (504) staff       (20)      627 2023-05-05 20:08:14.772914 CSV to JSON Python-0.0.3/setup.cfg
--rw-r--r--   0 dabolabs   (504) staff       (20)      879 2023-05-05 20:08:02.000000 CSV to JSON Python-0.0.3/setup.py
-drwxr-xr-x   0 dabolabs   (504) staff       (20)        0 2023-05-05 20:08:14.759900 CSV to JSON Python-0.0.3/src/
-drwxr-xr-x   0 dabolabs   (504) staff       (20)        0 2023-05-05 20:08:14.766629 CSV to JSON Python-0.0.3/src/CSV_to_JSON_Python.egg-info/
--rw-r--r--   0 dabolabs   (504) staff       (20)      556 2023-05-05 20:08:14.000000 CSV to JSON Python-0.0.3/src/CSV_to_JSON_Python.egg-info/PKG-INFO
--rw-r--r--   0 dabolabs   (504) staff       (20)      329 2023-05-05 20:08:14.000000 CSV to JSON Python-0.0.3/src/CSV_to_JSON_Python.egg-info/SOURCES.txt
--rw-r--r--   0 dabolabs   (504) staff       (20)        1 2023-05-05 20:08:14.000000 CSV to JSON Python-0.0.3/src/CSV_to_JSON_Python.egg-info/dependency_links.txt
--rw-r--r--   0 dabolabs   (504) staff       (20)       12 2023-05-05 20:08:14.000000 CSV to JSON Python-0.0.3/src/CSV_to_JSON_Python.egg-info/top_level.txt
-drwxr-xr-x   0 dabolabs   (504) staff       (20)        0 2023-05-05 20:08:14.770087 CSV to JSON Python-0.0.3/src/csv_to_json/
--rw-r--r--   0 dabolabs   (504) staff       (20)        0 2023-05-05 18:41:15.000000 CSV to JSON Python-0.0.3/src/csv_to_json/__init__.py
--rw-r--r--   0 dabolabs   (504) staff       (20)      756 2023-05-05 18:28:10.000000 CSV to JSON Python-0.0.3/src/csv_to_json/csv_to_json.py
--rw-r--r--   0 dabolabs   (504) staff       (20)      143 2023-05-05 19:53:54.000000 CSV to JSON Python-0.0.3/src/csv_to_json/hello_world.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 20:46:13.000000 CSV to JSON Python-0.0.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-05-05 20:45:56.000000 CSV to JSON Python-0.0.4/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      556 2023-05-05 20:46:13.000000 CSV to JSON Python-0.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 20:45:56.000000 CSV to JSON Python-0.0.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-05-05 20:45:56.000000 CSV to JSON Python-0.0.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      627 2023-05-05 20:46:13.000000 CSV to JSON Python-0.0.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      879 2023-05-05 20:45:56.000000 CSV to JSON Python-0.0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 20:46:13.000000 CSV to JSON Python-0.0.4/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 20:46:13.000000 CSV to JSON Python-0.0.4/src/CSV_to_JSON_Python.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      556 2023-05-05 20:46:13.000000 CSV to JSON Python-0.0.4/src/CSV_to_JSON_Python.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      329 2023-05-05 20:46:13.000000 CSV to JSON Python-0.0.4/src/CSV_to_JSON_Python.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 20:46:13.000000 CSV to JSON Python-0.0.4/src/CSV_to_JSON_Python.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-05 20:46:13.000000 CSV to JSON Python-0.0.4/src/CSV_to_JSON_Python.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 20:46:13.000000 CSV to JSON Python-0.0.4/src/csv_to_json/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 20:45:56.000000 CSV to JSON Python-0.0.4/src/csv_to_json/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      756 2023-05-05 20:45:56.000000 CSV to JSON Python-0.0.4/src/csv_to_json/csv_to_json.py
+-rw-r--r--   0 runner    (1001) docker     (123)      143 2023-05-05 20:45:56.000000 CSV to JSON Python-0.0.4/src/csv_to_json/hello_world.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive
+POSIX tar archive (GNU)
```

### Comparing `CSV to JSON Python-0.0.3/LICENSE.txt` & `CSV to JSON Python-0.0.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `CSV to JSON Python-0.0.3/PKG-INFO` & `CSV to JSON Python-0.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: CSV to JSON Python
-Version: 0.0.3
+Version: 0.0.4
 Summary: This is a package used to convert csv data to a json object
 Home-page: https://testpypi.org/project/CSV to JSON Python/
 Author: Paul Ndambo
 Author-email: paulkadabo@gmail.com
 Project-URL: Bug Tracker, https://testpypi.org/project/CSV to JSON Python/
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `CSV to JSON Python-0.0.3/setup.cfg` & `CSV to JSON Python-0.0.4/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = CSV to JSON Python
-version = 0.0.3
+version = 0.0.4
 author = Paul Ndambo
 author_email = author@example.com
 description = This is a package used to convert csv data to a json object
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://testpypi.org/project/CSV to JSON Python/
 project_urls =
```

### Comparing `CSV to JSON Python-0.0.3/setup.py` & `CSV to JSON Python-0.0.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding = "utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name = "CSV to JSON Python",
-    version = "0.0.3",
+    version = "0.0.4",
     author = "Paul Ndambo",
     author_email = "paulkadabo@gmail.com",
     description = "This is a package used to convert csv data to a json object",
     long_description = long_description,
     long_description_content_type = "text/markdown",
     url = "https://testpypi.org/project/CSV to JSON Python/",
     project_urls = {
```

### Comparing `CSV to JSON Python-0.0.3/src/CSV_to_JSON_Python.egg-info/PKG-INFO` & `CSV to JSON Python-0.0.4/src/CSV_to_JSON_Python.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: CSV-to-JSON-Python
-Version: 0.0.3
+Version: 0.0.4
 Summary: This is a package used to convert csv data to a json object
 Home-page: https://testpypi.org/project/CSV to JSON Python/
 Author: Paul Ndambo
 Author-email: paulkadabo@gmail.com
 Project-URL: Bug Tracker, https://testpypi.org/project/CSV to JSON Python/
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `CSV to JSON Python-0.0.3/src/csv_to_json/csv_to_json.py` & `CSV to JSON Python-0.0.4/src/csv_to_json/csv_to_json.py`

 * *Files identical despite different names*

