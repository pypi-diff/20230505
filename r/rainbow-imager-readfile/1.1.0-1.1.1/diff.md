# Comparing `tmp/rainbow_imager_readfile-1.1.0.tar.gz` & `tmp/rainbow_imager_readfile-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rainbow_imager_readfile-1.1.0.tar", max compression
+gzip compressed data, was "rainbow_imager_readfile-1.1.1.tar", max compression
```

## Comparing `rainbow_imager_readfile-1.1.0.tar` & `rainbow_imager_readfile-1.1.1.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1078 2021-06-16 15:28:11.000000 rainbow_imager_readfile-1.1.0/LICENSE
--rw-r--r--   0        0        0     2384 2023-05-04 21:39:27.812884 rainbow_imager_readfile-1.1.0/README.md
--rw-r--r--   0        0        0      665 2023-05-04 21:40:51.456457 rainbow_imager_readfile-1.1.0/pyproject.toml
--rw-r--r--   0        0        0       50 2023-05-04 21:40:51.501458 rainbow_imager_readfile-1.1.0/rainbow_imager_readfile/__init__.py
--rw-r--r--   0        0        0     7868 2021-11-17 16:50:19.000000 rainbow_imager_readfile-1.1.0/rainbow_imager_readfile/_rainbow.py
--rw-r--r--   0        0        0     3095 1970-01-01 00:00:00.000000 rainbow_imager_readfile-1.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1078 2021-06-16 15:28:11.000000 rainbow_imager_readfile-1.1.1/LICENSE
+-rw-r--r--   0        0        0     2384 2023-05-04 21:39:27.812884 rainbow_imager_readfile-1.1.1/README.md
+-rw-r--r--   0        0        0      671 2023-05-05 13:27:50.346960 rainbow_imager_readfile-1.1.1/pyproject.toml
+-rw-r--r--   0        0        0       50 2023-05-05 13:27:50.381960 rainbow_imager_readfile-1.1.1/rainbow_imager_readfile/__init__.py
+-rw-r--r--   0        0        0     7868 2021-11-17 16:50:19.000000 rainbow_imager_readfile-1.1.1/rainbow_imager_readfile/_rainbow.py
+-rw-r--r--   0        0        0     3095 1970-01-01 00:00:00.000000 rainbow_imager_readfile-1.1.1/PKG-INFO
```

### Comparing `rainbow_imager_readfile-1.1.0/LICENSE` & `rainbow_imager_readfile-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `rainbow_imager_readfile-1.1.0/README.md` & `rainbow_imager_readfile-1.1.1/README.md`

 * *Files identical despite different names*

### Comparing `rainbow_imager_readfile-1.1.0/pyproject.toml` & `rainbow_imager_readfile-1.1.1/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 [tool.poetry]
 name = "rainbow-imager-readfile"
-version = "1.1.0"
+version = "1.1.1"
 description = "Read functions for Rainbow ASI PNM raw files"
 readme = "README.md"
 homepage = "https://github.com/ucalgary-aurora/rainbow-imager-readfile"
 repository = "https://github.com/ucalgary-aurora/rainbow-imager-readfile"
 authors = ["Darren Chaddock <dchaddoc@ucalgary.ca>"]
 license = "MIT"
 packages = [
     { include = "rainbow_imager_readfile" },
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

### Comparing `rainbow_imager_readfile-1.1.0/rainbow_imager_readfile/_rainbow.py` & `rainbow_imager_readfile-1.1.1/rainbow_imager_readfile/_rainbow.py`

 * *Files identical despite different names*

### Comparing `rainbow_imager_readfile-1.1.0/PKG-INFO` & `rainbow_imager_readfile-1.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: rainbow-imager-readfile
-Version: 1.1.0
+Version: 1.1.1
 Summary: Read functions for Rainbow ASI PNM raw files
 Home-page: https://github.com/ucalgary-aurora/rainbow-imager-readfile
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
 Project-URL: Repository, https://github.com/ucalgary-aurora/rainbow-imager-readfile
 Description-Content-Type: text/markdown
 
 # Rainbow All-Sky Imager Raw PGM Data Readfile (GO-Canada AGO/CGSM Rainbow)
 
 [![Github Actions - Tests](https://github.com/ucalgary-aurora/rainbow-imager-readfile/workflows/tests/badge.svg)](https://github.com/ucalgary-aurora/rainbow-imager-readfile/actions?query=workflow%3Atests)
 [![PyPI version](https://img.shields.io/pypi/v/rainbow-imager-readfile.svg)](https://pypi.python.org/pypi/rainbow-imager-readfile/)
```

