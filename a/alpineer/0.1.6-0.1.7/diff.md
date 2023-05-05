# Comparing `tmp/alpineer-0.1.6.tar.gz` & `tmp/alpineer-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "alpineer-0.1.6.tar", max compression
+gzip compressed data, was "alpineer-0.1.7.tar", max compression
```

## Comparing `alpineer-0.1.6.tar` & `alpineer-0.1.7.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0    11845 2023-04-17 22:10:21.890788 alpineer-0.1.6/LICENSE
--rw-r--r--   0        0        0     4069 2023-04-17 22:10:21.890788 alpineer-0.1.6/README.md
--rw-r--r--   0        0        0     2847 2023-04-17 22:11:36.131760 alpineer-0.1.6/pyproject.toml
--rw-r--r--   0        0        0        0 2023-04-17 22:10:21.894788 alpineer-0.1.6/src/alpineer/__init__.py
--rw-r--r--   0        0        0     1398 2023-04-17 22:10:21.894788 alpineer-0.1.6/src/alpineer/data_utils.py
--rw-r--r--   0        0        0      939 2023-04-17 22:10:21.894788 alpineer-0.1.6/src/alpineer/image_utils.py
--rw-r--r--   0        0        0     7760 2023-04-17 22:10:21.894788 alpineer-0.1.6/src/alpineer/io_utils.py
--rw-r--r--   0        0        0    22804 2023-04-17 22:10:21.894788 alpineer-0.1.6/src/alpineer/load_utils.py
--rw-r--r--   0        0        0     8209 2023-04-17 22:10:21.894788 alpineer-0.1.6/src/alpineer/misc_utils.py
--rw-r--r--   0        0        0        0 2023-04-17 22:10:21.894788 alpineer-0.1.6/src/alpineer/py.typed
--rw-r--r--   0        0        0      223 2023-04-17 22:10:21.894788 alpineer-0.1.6/src/alpineer/settings.py
--rw-r--r--   0        0        0    20206 2023-04-17 22:10:21.894788 alpineer-0.1.6/src/alpineer/test_utils.py
--rw-r--r--   0        0        0     5109 2023-04-17 22:10:21.894788 alpineer-0.1.6/src/alpineer/tiff_utils.py
--rw-r--r--   0        0        0     5197 1970-01-01 00:00:00.000000 alpineer-0.1.6/PKG-INFO
+-rw-r--r--   0        0        0    11845 2023-05-05 20:26:14.594905 alpineer-0.1.7/LICENSE
+-rw-r--r--   0        0        0     5220 2023-05-05 20:26:14.594905 alpineer-0.1.7/README.md
+-rw-r--r--   0        0        0     2758 2023-05-05 20:26:46.391635 alpineer-0.1.7/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-05-05 20:26:14.598905 alpineer-0.1.7/src/alpineer/__init__.py
+-rw-r--r--   0        0        0     1398 2023-05-05 20:26:14.598905 alpineer-0.1.7/src/alpineer/data_utils.py
+-rw-r--r--   0        0        0      939 2023-05-05 20:26:14.598905 alpineer-0.1.7/src/alpineer/image_utils.py
+-rw-r--r--   0        0        0     7760 2023-05-05 20:26:14.598905 alpineer-0.1.7/src/alpineer/io_utils.py
+-rw-r--r--   0        0        0    22804 2023-05-05 20:26:14.598905 alpineer-0.1.7/src/alpineer/load_utils.py
+-rw-r--r--   0        0        0     8209 2023-05-05 20:26:14.598905 alpineer-0.1.7/src/alpineer/misc_utils.py
+-rw-r--r--   0        0        0        0 2023-05-05 20:26:14.598905 alpineer-0.1.7/src/alpineer/py.typed
+-rw-r--r--   0        0        0      223 2023-05-05 20:26:14.598905 alpineer-0.1.7/src/alpineer/settings.py
+-rw-r--r--   0        0        0    20206 2023-05-05 20:26:14.598905 alpineer-0.1.7/src/alpineer/test_utils.py
+-rw-r--r--   0        0        0     5109 2023-05-05 20:26:14.598905 alpineer-0.1.7/src/alpineer/tiff_utils.py
+-rw-r--r--   0        0        0     6298 1970-01-01 00:00:00.000000 alpineer-0.1.7/PKG-INFO
```

### Comparing `alpineer-0.1.6/LICENSE` & `alpineer-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `alpineer-0.1.6/pyproject.toml` & `alpineer-0.1.7/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "alpineer"
-version = "0.1.6"
+version = "0.1.7"
 description = "Toolbox for Multiplexed Imaging. Contains scripts and little tools which are used throughout ark-analysis, mibi-bin-tools, and toffy."
 authors = [
     "Noah Frey Greenwald <nfgreen@stanford.edu>",
     "Adam Kagel <ackagel@stanford.edu>",
     "Alex Kong <alkong@stanford.edu>",
     "Cami Laura Sowers <csowers@stanford.edu>",
     "Sricharan Reddy Varra <srivarra@stanford.edu>",
@@ -24,51 +24,49 @@
 enable = false
 vcs = "git"
 bump = true
 style = "pep440"
 metadata = false
 
 [tool.poetry.dependencies]
-python = "^3.8"
+python = "^3.9"
 numpy = "1.*"
 natsort = "^8"
 tifffile = "*"
 matplotlib = "^3"
 pillow = "^9"
 scikit-image = "0.*"
 xarray = "*"
 xmltodict = "^0.13.0"
 charset-normalizer = "^2.1.1"
 
 [tool.poetry.group.test]
 optional = true
 
 [tool.poetry.group.test.dependencies]
-pytest = "^7.1.3"
-coveralls = { version = "^3.3.1", extras = ["toml"] }
-pytest-cases = "^3.6.13"
-pytest-order = "^1.0.1"
-pytest-cov = "^4.0.0"
-pytest-mock = "^3.10.0"
-pytest-pycodestyle = "^2.3.0"
-pytest-asyncio = "^0.19.0"
+pytest = "^7"
+pytest-cases = "^3"
+pytest-cov = "^4"
+pytest-mock = "^3"
+pytest-pycodestyle = "^2"
+pytest-asyncio = "^0"
 
 [tool.poetry.group.dev]
 optional = true
 
 [tool.poetry.group.dev.dependencies]
 black = "^22.10.0"
 isort = "^5.10.1"
-mypy = "^0.982"
+mypy = "^1.2"
 jupyterlab = "^3.5.0"
 
 ## TYPE CHECKING ##
 
 [tool.mypy]
-python_version = "3.8"
+python_version = "3.9"
 mypy_path = "$MYPY_CONFIG_FILE_DIR/src:$MYPY_CONFIG_FILE_DIR/tests"
 warn_return_any = true
 warn_unused_configs = true
 warn_unused_ignores = false
 ignore_missing_imports = false
 
 [[tool.mypy.overrides]]
@@ -85,20 +83,20 @@
 ignore_missing_imports = true
 
 
 ## LINTING, FORMATTING ##
 
 [tool.black]
 line-length = 100
-target-version = ['py38']
+target-version = ["py39", "py310", "py311"]
 include = '\.pyi?$'
 preview = true
 
 [tool.isort]
-py_version = 38
+py_version = 39
 profile = "black"
 line_length = 100
 multi_line_output = 3
 
 ## COVERAGE ##
 
 [tool.coverage.paths]
```

### Comparing `alpineer-0.1.6/src/alpineer/data_utils.py` & `alpineer-0.1.7/src/alpineer/data_utils.py`

 * *Files identical despite different names*

### Comparing `alpineer-0.1.6/src/alpineer/image_utils.py` & `alpineer-0.1.7/src/alpineer/image_utils.py`

 * *Files identical despite different names*

### Comparing `alpineer-0.1.6/src/alpineer/io_utils.py` & `alpineer-0.1.7/src/alpineer/io_utils.py`

 * *Files identical despite different names*

### Comparing `alpineer-0.1.6/src/alpineer/load_utils.py` & `alpineer-0.1.7/src/alpineer/load_utils.py`

 * *Files identical despite different names*

### Comparing `alpineer-0.1.6/src/alpineer/misc_utils.py` & `alpineer-0.1.7/src/alpineer/misc_utils.py`

 * *Files identical despite different names*

### Comparing `alpineer-0.1.6/src/alpineer/test_utils.py` & `alpineer-0.1.7/src/alpineer/test_utils.py`

 * *Files identical despite different names*

### Comparing `alpineer-0.1.6/src/alpineer/tiff_utils.py` & `alpineer-0.1.7/src/alpineer/tiff_utils.py`

 * *Files identical despite different names*

### Comparing `alpineer-0.1.6/PKG-INFO` & `alpineer-0.1.7/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,37 +1,18 @@
-Metadata-Version: 2.1
-Name: alpineer
-Version: 0.1.6
-Summary: Toolbox for Multiplexed Imaging. Contains scripts and little tools which are used throughout ark-analysis, mibi-bin-tools, and toffy.
-Home-page: https://github.com/angelolab/tmi
-License: Modified Apache 2.0
-Author: Noah Frey Greenwald
-Author-email: nfgreen@stanford.edu
-Requires-Python: >=3.8,<4.0
-Classifier: License :: Other/Proprietary License
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: charset-normalizer (>=2.1.1,<3.0.0)
-Requires-Dist: matplotlib (>=3,<4)
-Requires-Dist: natsort (>=8,<9)
-Requires-Dist: numpy (>=1.0.0,<2.0.0)
-Requires-Dist: pillow (>=9,<10)
-Requires-Dist: scikit-image (<1.0.0)
-Requires-Dist: tifffile
-Requires-Dist: xarray
-Requires-Dist: xmltodict (>=0.13.0,<0.14.0)
-Project-URL: Documentation, https://tmi.readthedocs.io
-Project-URL: Repository, https://github.com/angelolab/tmi
-Description-Content-Type: text/markdown
-
 # Alpineer
 
+<div align="center">
+
+| | |
+| ---        |    ---  |
+| CI / CD | [![CI](https://github.com/angelolab/alpineer/actions/workflows/ci.yml/badge.svg)](https://github.com/angelolab/alpineer/actions/workflows/ci.yml) [![Coverage Status](https://coveralls.io/repos/github/angelolab/alpineer/badge.svg?branch=main)](https://coveralls.io/github/angelolab/mibi-bin-tools?branch=main) |
+| Package | [![PyPI - Version](https://img.shields.io/pypi/v/alpineer.svg?logo=pypi&label=PyPI&logoColor=gold)](https://pypi.org/project/alpineer/) [![PyPI - Downloads](https://img.shields.io/pypi/dm/alpineer.svg?color=blue&label=Downloads&logo=pypi&logoColor=gold)](https://pypi.org/project/alpineer/) [![PyPI - Python Version](https://img.shields.io/pypi/pyversions/alpineer.svg?logo=python&label=Python&logoColor=gold)](https://pypi.org/project/alpineer/) |
+|Meta | [![code style - Black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black) [![types - Mypy](https://img.shields.io/badge/types-Mypy-blue.svg)](https://github.com/python/mypy) [![PyPI - License](https://img.shields.io/pypi/l/alpineer?color=9400d3)](LICENSE) |
+</div>
+
 Toolbox for Multiplexed Imaging. Contains scripts and little tools which are used throughout [ark-analysis](https://github.com/angelolab/ark-analysis), [mibi-bin-tools](https://github.com/angelolab/mibi-bin-tools), and [toffy](https://github.com/angelolab/toffy)
 
 - [alpineer](#alpineer)
   - [Requirements](#requirements)
   - [Setup](#setup)
   - [Development Notes](#development-notes)
   - [Questions?](#questions)
@@ -109,8 +90,7 @@
 * In order to update `alpineer`'s dependencies we can run:
   *  `poetry update`: for all dependencies
   *  `poetry update <package>`: where `<package>` can be something like `numpy`.
 * To update Poetry itself, run `poetry self update`.
 ## Questions?
 
 Feel free to open an issue on our [GitHub page](https://github.com/angelolab/alpineer/issues)
-
```

