# Comparing `tmp/nascam_imager_readfile-1.2.0.tar.gz` & `tmp/nascam_imager_readfile-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nascam_imager_readfile-1.2.0.tar", max compression
+gzip compressed data, was "nascam_imager_readfile-1.2.1.tar", max compression
```

## Comparing `nascam_imager_readfile-1.2.0.tar` & `nascam_imager_readfile-1.2.1.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0     1078 2022-05-07 17:20:12.000000 nascam_imager_readfile-1.2.0/LICENSE
--rw-r--r--   0        0        0     2513 2023-01-03 00:16:12.000000 nascam_imager_readfile-1.2.0/README.md
--rw-r--r--   0        0        0       49 2023-05-04 21:35:49.239774 nascam_imager_readfile-1.2.0/nascam_imager_readfile/__init__.py
--rw-r--r--   0        0        0     8183 2023-05-04 21:33:12.222821 nascam_imager_readfile-1.2.0/nascam_imager_readfile/_nascam.py
--rw-r--r--   0        0        0      681 2023-05-04 21:35:49.204773 nascam_imager_readfile-1.2.0/pyproject.toml
--rw-r--r--   0        0        0     3262 1970-01-01 00:00:00.000000 nascam_imager_readfile-1.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1078 2022-05-07 17:20:12.000000 nascam_imager_readfile-1.2.1/LICENSE
+-rw-r--r--   0        0        0     2513 2023-05-04 21:39:35.746033 nascam_imager_readfile-1.2.1/README.md
+-rw-r--r--   0        0        0       49 2023-05-05 13:27:03.375086 nascam_imager_readfile-1.2.1/nascam_imager_readfile/__init__.py
+-rw-r--r--   0        0        0     8183 2023-05-04 21:33:12.222821 nascam_imager_readfile-1.2.1/nascam_imager_readfile/_nascam.py
+-rw-r--r--   0        0        0      687 2023-05-05 13:27:03.338086 nascam_imager_readfile-1.2.1/pyproject.toml
+-rw-r--r--   0        0        0     3262 1970-01-01 00:00:00.000000 nascam_imager_readfile-1.2.1/PKG-INFO
```

### Comparing `nascam_imager_readfile-1.2.0/LICENSE` & `nascam_imager_readfile-1.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `nascam_imager_readfile-1.2.0/README.md` & `nascam_imager_readfile-1.2.1/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 
 ```console
 $ python3 -m pip install nascam-imager-readfile
 ```
 
 ## Supported Python Versions
 
-nascam-imager-readfile officially supports Python 3.6+.
+nascam-imager-readfile officially supports Python 3.8+.
 
 ## Examples
 
 Example Python notebooks can be found in the "examples" directory. Further, some examples can be found in the "Usage" section below.
 
 ## Usage
```

### Comparing `nascam_imager_readfile-1.2.0/nascam_imager_readfile/_nascam.py` & `nascam_imager_readfile-1.2.1/nascam_imager_readfile/_nascam.py`

 * *Files identical despite different names*

### Comparing `nascam_imager_readfile-1.2.0/pyproject.toml` & `nascam_imager_readfile-1.2.1/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 [tool.poetry]
 name = "nascam-imager-readfile"
-version = "1.2.0"
+version = "1.2.1"
 description = "Read functions for NASCAM ASI raw files"
 readme = "README.md"
 homepage = "https://github.com/ucalgary-aurora/nascam-imager-readfile"
 repository = "https://github.com/ucalgary-aurora/nascam-imager-readfile"
 authors = ["Darren Chaddock <dchaddoc@ucalgary.ca>"]
 license = "MIT"
 packages = [
     { include = "nascam_imager_readfile" },
 ]
 
 [tool.poetry.dependencies]
 python = "^3.8.1"
-numpy = "^1.24.0"
-opencv-python = "^4.7.0"
+numpy = "^1.21.0"
+opencv-python = "^4.4.0"
 
-[tool.poetry.dev-dependencies]
+[tool.poetry.group.dev.dependencies]
 pytest = "^7.0.0"
 flake8 = "^6.0.0"
 pylint = "^2.16.0"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `nascam_imager_readfile-1.2.0/PKG-INFO` & `nascam_imager_readfile-1.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,23 +1,23 @@
 Metadata-Version: 2.1
 Name: nascam-imager-readfile
-Version: 1.2.0
+Version: 1.2.1
 Summary: Read functions for NASCAM ASI raw files
 Home-page: https://github.com/ucalgary-aurora/nascam-imager-readfile
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
-Requires-Dist: opencv-python (>=4.7.0,<5.0.0)
+Requires-Dist: numpy (>=1.21.0,<2.0.0)
+Requires-Dist: opencv-python (>=4.4.0,<5.0.0)
 Project-URL: Repository, https://github.com/ucalgary-aurora/nascam-imager-readfile
 Description-Content-Type: text/markdown
 
 # NASCAM All-Sky Imager Raw PGM Data Readfile
 
 [![Github Actions - Tests](https://github.com/ucalgary-aurora/nascam-imager-readfile/workflows/tests/badge.svg)](https://github.com/ucalgary-aurora/nascam-imager-readfile/actions?query=workflow%3Atests)
 [![PyPI version](https://img.shields.io/pypi/v/nascam-imager-readfile.svg)](https://pypi.python.org/pypi/nascam-imager-readfile/)
@@ -36,15 +36,15 @@
 
 ```console
 $ python3 -m pip install nascam-imager-readfile
 ```
 
 ## Supported Python Versions
 
-nascam-imager-readfile officially supports Python 3.6+.
+nascam-imager-readfile officially supports Python 3.8+.
 
 ## Examples
 
 Example Python notebooks can be found in the "examples" directory. Further, some examples can be found in the "Usage" section below.
 
 ## Usage
```

