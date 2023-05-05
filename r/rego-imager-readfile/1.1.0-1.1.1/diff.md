# Comparing `tmp/rego_imager_readfile-1.1.0.tar.gz` & `tmp/rego_imager_readfile-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rego_imager_readfile-1.1.0.tar", max compression
+gzip compressed data, was "rego_imager_readfile-1.1.1.tar", max compression
```

## Comparing `rego_imager_readfile-1.1.0.tar` & `rego_imager_readfile-1.1.1.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1078 2021-02-25 19:14:26.000000 rego_imager_readfile-1.1.0/LICENSE
--rw-r--r--   0        0        0     2400 2023-05-05 00:57:47.375894 rego_imager_readfile-1.1.0/README.md
--rw-r--r--   0        0        0      650 2023-05-05 01:01:21.257426 rego_imager_readfile-1.1.0/pyproject.toml
--rw-r--r--   0        0        0       47 2023-05-05 01:01:21.301427 rego_imager_readfile-1.1.0/rego_imager_readfile/__init__.py
--rw-r--r--   0        0        0     7731 2021-03-29 15:25:44.000000 rego_imager_readfile-1.1.0/rego_imager_readfile/_rego.py
--rw-r--r--   0        0        0     3099 1970-01-01 00:00:00.000000 rego_imager_readfile-1.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1078 2021-02-25 19:14:26.000000 rego_imager_readfile-1.1.1/LICENSE
+-rw-r--r--   0        0        0     2400 2023-05-05 00:57:47.375894 rego_imager_readfile-1.1.1/README.md
+-rw-r--r--   0        0        0      656 2023-05-05 13:26:03.190968 rego_imager_readfile-1.1.1/pyproject.toml
+-rw-r--r--   0        0        0       47 2023-05-05 13:26:03.223968 rego_imager_readfile-1.1.1/rego_imager_readfile/__init__.py
+-rw-r--r--   0        0        0     7731 2021-03-29 15:25:44.000000 rego_imager_readfile-1.1.1/rego_imager_readfile/_rego.py
+-rw-r--r--   0        0        0     3099 1970-01-01 00:00:00.000000 rego_imager_readfile-1.1.1/PKG-INFO
```

### Comparing `rego_imager_readfile-1.1.0/LICENSE` & `rego_imager_readfile-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `rego_imager_readfile-1.1.0/README.md` & `rego_imager_readfile-1.1.1/README.md`

 * *Files identical despite different names*

### Comparing `rego_imager_readfile-1.1.0/pyproject.toml` & `rego_imager_readfile-1.1.1/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 [tool.poetry]
 name = "rego-imager-readfile"
-version = "1.1.0"
+version = "1.1.1"
 description = "Read functions for REGO ASI PGM raw files"
 readme = "README.md"
 homepage = "https://github.com/ucalgary-aurora/rego-imager-readfile"
 repository = "https://github.com/ucalgary-aurora/rego-imager-readfile"
 authors = ["Darren Chaddock <dchaddoc@ucalgary.ca>"]
 license = "MIT"
 packages = [
     { include = "rego_imager_readfile" },
 ]
 
 [tool.poetry.dependencies]
 python = "^3.8.1"
-numpy = "^1.24.0"
+numpy = "^1.21.0"
 
-[tool.poetry.dev-dependencies]
+[tool.poetry.group.dev.dependencies]
 pytest = "^7.0.0"
 flake8 = "^6.0.0"
 pylint = "^2.16.0"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `rego_imager_readfile-1.1.0/rego_imager_readfile/_rego.py` & `rego_imager_readfile-1.1.1/rego_imager_readfile/_rego.py`

 * *Files identical despite different names*

### Comparing `rego_imager_readfile-1.1.0/PKG-INFO` & `rego_imager_readfile-1.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: rego-imager-readfile
-Version: 1.1.0
+Version: 1.1.1
 Summary: Read functions for REGO ASI PGM raw files
 Home-page: https://github.com/ucalgary-aurora/rego-imager-readfile
 License: MIT
 Author: Darren Chaddock
 Author-email: dchaddoc@ucalgary.ca
 Requires-Python: >=3.8.1,<4.0.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: numpy (>=1.24.0,<2.0.0)
+Requires-Dist: numpy (>=1.21.0,<2.0.0)
 Project-URL: Repository, https://github.com/ucalgary-aurora/rego-imager-readfile
 Description-Content-Type: text/markdown
 
 # Redline All-Sky Imager Raw PGM Data Readfile (REGO)
 
 [![Github Actions - Tests](https://github.com/ucalgary-aurora/rego-imager-readfile/workflows/tests/badge.svg)](https://github.com/ucalgary-aurora/rego-imager-readfile/actions?query=workflow%3Atests)
 [![PyPI version](https://img.shields.io/pypi/v/rego-imager-readfile.svg)](https://pypi.python.org/pypi/rego-imager-readfile/)
```

