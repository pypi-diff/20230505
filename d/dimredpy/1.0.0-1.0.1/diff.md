# Comparing `tmp/dimredpy-1.0.0.tar.gz` & `tmp/dimredpy-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dimredpy-1.0.0.tar", max compression
+gzip compressed data, was "dimredpy-1.0.1.tar", max compression
```

## Comparing `dimredpy-1.0.0.tar` & `dimredpy-1.0.1.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1073 2023-05-05 14:24:08.481783 dimredpy-1.0.0/LICENSE
--rw-r--r--   0        0        0       61 2023-05-05 14:57:51.318530 dimredpy-1.0.0/README.md
--rw-r--r--   0        0        0     5744 2023-05-05 14:49:55.228360 dimredpy-1.0.0/dimpy/JaxLDA.py
--rw-r--r--   0        0        0     3202 2023-05-05 14:47:37.470995 dimredpy-1.0.0/dimpy/JaxPCA.py
--rw-r--r--   0        0        0     2487 2023-05-05 14:36:51.037036 dimredpy-1.0.0/dimpy/JaxRPCA.py
--rw-r--r--   0        0        0        0 2023-05-05 14:36:24.367685 dimredpy-1.0.0/dimpy/__init__.py
--rw-r--r--   0        0        0      542 2023-05-05 15:45:28.579627 dimredpy-1.0.0/pyproject.toml
--rw-r--r--   0        0        0      696 1970-01-01 00:00:00.000000 dimredpy-1.0.0/PKG-INFO
+-rw-r--r--   0        0        0     1073 2023-05-05 14:24:08.481783 dimredpy-1.0.1/LICENSE
+-rw-r--r--   0        0        0       61 2023-05-05 14:57:51.318530 dimredpy-1.0.1/README.md
+-rw-r--r--   0        0        0     5744 2023-05-05 14:49:55.228360 dimredpy-1.0.1/dimpy/JaxLDA.py
+-rw-r--r--   0        0        0     3202 2023-05-05 14:47:37.470995 dimredpy-1.0.1/dimpy/JaxPCA.py
+-rw-r--r--   0        0        0     2487 2023-05-05 14:36:51.037036 dimredpy-1.0.1/dimpy/JaxRPCA.py
+-rw-r--r--   0        0        0       84 2023-05-05 15:56:14.399824 dimredpy-1.0.1/dimpy/__init__.py
+-rw-r--r--   0        0        0      543 2023-05-05 15:58:16.265960 dimredpy-1.0.1/pyproject.toml
+-rw-r--r--   0        0        0      696 1970-01-01 00:00:00.000000 dimredpy-1.0.1/PKG-INFO
```

### Comparing `dimredpy-1.0.0/LICENSE` & `dimredpy-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `dimredpy-1.0.0/dimpy/JaxLDA.py` & `dimredpy-1.0.1/dimpy/JaxLDA.py`

 * *Files identical despite different names*

### Comparing `dimredpy-1.0.0/dimpy/JaxPCA.py` & `dimredpy-1.0.1/dimpy/JaxPCA.py`

 * *Files identical despite different names*

### Comparing `dimredpy-1.0.0/dimpy/JaxRPCA.py` & `dimredpy-1.0.1/dimpy/JaxRPCA.py`

 * *Files identical despite different names*

### Comparing `dimredpy-1.0.0/pyproject.toml` & `dimredpy-1.0.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "dimredpy"
-version = "1.0.0"
+version = "1.0.1"
 description = "Dimensionality reduction techniques in python, built on JAX"
 authors = ["Alex Kiefer <alkiefer@iu.edu>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "dimpy"}]
 
 [tool.poetry.dependencies]
@@ -18,8 +18,8 @@
 black = "^23.3.0"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [project.urls]
-"Homepage" = "https://github.com/alexk101/dimredpy"
+"Homepage" = "https://github.com/alexk101/dimredpy"
```

### Comparing `dimredpy-1.0.0/PKG-INFO` & `dimredpy-1.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dimredpy
-Version: 1.0.0
+Version: 1.0.1
 Summary: Dimensionality reduction techniques in python, built on JAX
 License: MIT
 Author: Alex Kiefer
 Author-email: alkiefer@iu.edu
 Requires-Python: >=3.8
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

