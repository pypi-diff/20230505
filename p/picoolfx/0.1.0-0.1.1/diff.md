# Comparing `tmp/picoolfx-0.1.0.tar.gz` & `tmp/picoolfx-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "picoolfx-0.1.0.tar", last modified: Thu May  4 23:15:38 2023, max compression
+gzip compressed data, was "picoolfx-0.1.1.tar", last modified: Thu May  4 23:33:31 2023, max compression
```

## Comparing `picoolfx-0.1.0.tar` & `picoolfx-0.1.1.tar`

### file list

```diff
@@ -1,9 +1,10 @@
--rw-r--r--   0        0        0     1415 2023-04-24 14:59:59.764737 picoolfx-0.1.0/README.md
--rw-r--r--   0        0        0      286 2023-05-04 17:50:23.163487 picoolfx-0.1.0/picoolfx/__init__.py
--rw-r--r--   0        0        0    12180 2023-05-04 22:10:36.491818 picoolfx-0.1.0/picoolfx/picoolfx.py
--rw-r--r--   0        0        0     9218 2023-05-04 22:18:21.566056 picoolfx-0.1.0/picoolfx/utils.py
--rw-r--r--   0        0        0      598 2023-05-04 23:15:38.530476 picoolfx-0.1.0/pyproject.toml
--rw-r--r--   0        0        0        0 2023-05-03 19:56:06.828601 picoolfx-0.1.0/tests/__init__.py
--rw-r--r--   0        0        0   105627 2023-04-17 12:01:28.853226 picoolfx-0.1.0/tests/test_image.jpg
--rw-r--r--   0        0        0     2897 2023-05-04 22:49:58.028475 picoolfx-0.1.0/tests/test_picoolfx.py
--rw-r--r--   0        0        0     1888 1970-01-01 00:00:00.000000 picoolfx-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1077 2023-05-04 23:32:32.821011 picoolfx-0.1.1/LICENSE.txt
+-rw-r--r--   0        0        0      672 2023-05-04 23:32:49.938831 picoolfx-0.1.1/README.md
+-rw-r--r--   0        0        0      286 2023-05-04 17:50:23.163487 picoolfx-0.1.1/picoolfx/__init__.py
+-rw-r--r--   0        0        0    12180 2023-05-04 22:10:36.491818 picoolfx-0.1.1/picoolfx/picoolfx.py
+-rw-r--r--   0        0        0     9218 2023-05-04 22:18:21.566056 picoolfx-0.1.1/picoolfx/utils.py
+-rw-r--r--   0        0        0      737 2023-05-04 23:33:31.136236 picoolfx-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-05-03 19:56:06.828601 picoolfx-0.1.1/tests/__init__.py
+-rw-r--r--   0        0        0   105627 2023-04-17 12:01:28.853226 picoolfx-0.1.1/tests/test_image.jpg
+-rw-r--r--   0        0        0     2897 2023-05-04 22:49:58.028475 picoolfx-0.1.1/tests/test_picoolfx.py
+-rw-r--r--   0        0        0     1343 1970-01-01 00:00:00.000000 picoolfx-0.1.1/PKG-INFO
```

### Comparing `picoolfx-0.1.0/picoolfx/picoolfx.py` & `picoolfx-0.1.1/picoolfx/picoolfx.py`

 * *Files identical despite different names*

### Comparing `picoolfx-0.1.0/picoolfx/utils.py` & `picoolfx-0.1.1/picoolfx/utils.py`

 * *Files identical despite different names*

### Comparing `picoolfx-0.1.0/pyproject.toml` & `picoolfx-0.1.1/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -2,25 +2,35 @@
 requires = [
     "pdm-backend",
 ]
 build-backend = "pdm.backend"
 
 [project]
 name = "picoolfx"
-version = "0.1.0"
+version = "0.1.1"
 authors = [
     { name = "Nicola Cerutti", email = "nc@nicores.de" },
 ]
 description = "A small package that applies nice effects to images"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
+dependencies = [
+    "geopandas",
+    "matplotlib",
+    "noise",
+    "numpy",
+    "pandas",
+    "Pillow",
+    "rasterio",
+    "Shapely",
+]
 
 [project.urls]
 Homepage = "https://github.com/ncerutti/picoolfx"
 "Bug Tracker" = "https://github.com/ncerutti/picoolfx/issues"
 
 [tool]
```

### Comparing `picoolfx-0.1.0/tests/test_image.jpg` & `picoolfx-0.1.1/tests/test_image.jpg`

 * *Files identical despite different names*

### Comparing `picoolfx-0.1.0/tests/test_picoolfx.py` & `picoolfx-0.1.1/tests/test_picoolfx.py`

 * *Files identical despite different names*

