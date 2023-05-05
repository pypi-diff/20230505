# Comparing `tmp/themis_imager_readfile-1.1.0.tar.gz` & `tmp/themis_imager_readfile-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "themis_imager_readfile-1.1.0.tar", max compression
+gzip compressed data, was "themis_imager_readfile-1.1.1.tar", max compression
```

## Comparing `themis_imager_readfile-1.1.0.tar` & `themis_imager_readfile-1.1.1.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1078 2020-10-18 22:39:44.000000 themis_imager_readfile-1.1.0/LICENSE
--rw-r--r--   0        0        0     2475 2023-05-04 21:32:07.373602 themis_imager_readfile-1.1.0/README.md
--rw-r--r--   0        0        0      660 2023-05-04 21:29:32.176684 themis_imager_readfile-1.1.0/pyproject.toml
--rw-r--r--   0        0        0       49 2023-05-04 21:29:32.214684 themis_imager_readfile-1.1.0/themis_imager_readfile/__init__.py
--rw-r--r--   0        0        0     8458 2021-11-17 16:36:55.000000 themis_imager_readfile-1.1.0/themis_imager_readfile/_themis.py
--rw-r--r--   0        0        0     3182 1970-01-01 00:00:00.000000 themis_imager_readfile-1.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1078 2020-10-18 22:39:44.000000 themis_imager_readfile-1.1.1/LICENSE
+-rw-r--r--   0        0        0     2475 2023-05-04 21:32:07.373602 themis_imager_readfile-1.1.1/README.md
+-rw-r--r--   0        0        0      666 2023-05-05 13:23:43.203365 themis_imager_readfile-1.1.1/pyproject.toml
+-rw-r--r--   0        0        0       49 2023-05-05 13:23:43.230366 themis_imager_readfile-1.1.1/themis_imager_readfile/__init__.py
+-rw-r--r--   0        0        0     8458 2021-11-17 16:36:55.000000 themis_imager_readfile-1.1.1/themis_imager_readfile/_themis.py
+-rw-r--r--   0        0        0     3182 1970-01-01 00:00:00.000000 themis_imager_readfile-1.1.1/PKG-INFO
```

### Comparing `themis_imager_readfile-1.1.0/LICENSE` & `themis_imager_readfile-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `themis_imager_readfile-1.1.0/README.md` & `themis_imager_readfile-1.1.1/README.md`

 * *Files identical despite different names*

### Comparing `themis_imager_readfile-1.1.0/pyproject.toml` & `themis_imager_readfile-1.1.1/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 [tool.poetry]
 name = "themis-imager-readfile"
-version = "1.1.0"
+version = "1.1.1"
 description = "Read functions for THEMIS ASI PGM raw files"
 readme = "README.md"
 homepage = "https://github.com/ucalgary-aurora/themis-imager-readfile"
 repository = "https://github.com/ucalgary-aurora/themis-imager-readfile"
 authors = ["Darren Chaddock <dchaddoc@ucalgary.ca>"]
 license = "MIT"
 packages = [
     { include = "themis_imager_readfile" },
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

### Comparing `themis_imager_readfile-1.1.0/themis_imager_readfile/_themis.py` & `themis_imager_readfile-1.1.1/themis_imager_readfile/_themis.py`

 * *Files identical despite different names*

### Comparing `themis_imager_readfile-1.1.0/PKG-INFO` & `themis_imager_readfile-1.1.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: themis-imager-readfile
-Version: 1.1.0
+Version: 1.1.1
 Summary: Read functions for THEMIS ASI PGM raw files
 Home-page: https://github.com/ucalgary-aurora/themis-imager-readfile
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
 Project-URL: Repository, https://github.com/ucalgary-aurora/themis-imager-readfile
 Description-Content-Type: text/markdown
 
 # THEMIS All-Sky Imager Raw PGM Data Readfile
 
 [![Github Actions - Tests](https://github.com/ucalgary-aurora/themis-imager-readfile/workflows/tests/badge.svg)](https://github.com/ucalgary-aurora/themis-imager-readfile/actions?query=workflow%3Atests)
 [![PyPI version](https://img.shields.io/pypi/v/themis-imager-readfile.svg)](https://pypi.python.org/pypi/themis-imager-readfile/)
```

