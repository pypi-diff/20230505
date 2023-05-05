# Comparing `tmp/twyn-0.20.0.tar.gz` & `tmp/twyn-0.20.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "twyn-0.20.0.tar", max compression
+gzip compressed data, was "twyn-0.20.1.tar", max compression
```

## Comparing `twyn-0.20.0.tar` & `twyn-0.20.1.tar`

### file list

```diff
@@ -1,28 +1,28 @@
--rw-r--r--   0        0        0     1081 2023-05-05 09:17:20.318797 twyn-0.20.0/LICENSE
--rw-r--r--   0        0        0     3362 2023-05-05 09:17:20.318797 twyn-0.20.0/README.md
--rw-r--r--   0        0        0     1938 2023-05-05 09:17:20.322797 twyn-0.20.0/pyproject.toml
--rw-r--r--   0        0        0        0 2023-05-05 09:17:20.322797 twyn-0.20.0/src/twyn/__init__.py
--rw-r--r--   0        0        0        0 2023-05-05 09:17:20.322797 twyn-0.20.0/src/twyn/base/__init__.py
--rw-r--r--   0        0        0      942 2023-05-05 09:17:20.322797 twyn-0.20.0/src/twyn/base/constants.py
--rw-r--r--   0        0        0      147 2023-05-05 09:17:20.322797 twyn-0.20.0/src/twyn/base/exceptions.py
--rw-r--r--   0        0        0     2331 2023-05-05 09:17:20.322797 twyn-0.20.0/src/twyn/cli.py
--rw-r--r--   0        0        0        0 2023-05-05 09:17:20.322797 twyn-0.20.0/src/twyn/core/__init__.py
--rw-r--r--   0        0        0     3298 2023-05-05 09:17:20.322797 twyn-0.20.0/src/twyn/core/config_handler.py
--rw-r--r--   0        0        0      513 2023-05-05 09:17:20.322797 twyn-0.20.0/src/twyn/core/exceptions.py
--rw-r--r--   0        0        0      221 2023-05-05 09:17:20.322797 twyn-0.20.0/src/twyn/dependency_parser/__init__.py
--rw-r--r--   0        0        0     1463 2023-05-05 09:17:20.322797 twyn-0.20.0/src/twyn/dependency_parser/abstract_parser.py
--rw-r--r--   0        0        0     2149 2023-05-05 09:17:20.322797 twyn-0.20.0/src/twyn/dependency_parser/dependency_selector.py
--rw-r--r--   0        0        0      554 2023-05-05 09:17:20.322797 twyn-0.20.0/src/twyn/dependency_parser/exceptions.py
--rw-r--r--   0        0        0      761 2023-05-05 09:17:20.322797 twyn-0.20.0/src/twyn/dependency_parser/poetry_lock.py
--rw-r--r--   0        0        0      804 2023-05-05 09:17:20.322797 twyn-0.20.0/src/twyn/dependency_parser/requirements_txt.py
--rw-r--r--   0        0        0     5114 2023-05-05 09:17:20.322797 twyn-0.20.0/src/twyn/main.py
--rw-r--r--   0        0        0        0 2023-05-05 09:17:20.322797 twyn-0.20.0/src/twyn/similarity/__init__.py
--rw-r--r--   0        0        0     2210 2023-05-05 09:17:20.322797 twyn-0.20.0/src/twyn/similarity/algorithm.py
--rw-r--r--   0        0        0      275 2023-05-05 09:17:20.322797 twyn-0.20.0/src/twyn/similarity/exceptions.py
--rw-r--r--   0        0        0      189 2023-05-05 09:17:20.322797 twyn-0.20.0/src/twyn/trusted_packages/__init__.py
--rw-r--r--   0        0        0     1497 2023-05-05 09:17:20.322797 twyn-0.20.0/src/twyn/trusted_packages/constants.py
--rw-r--r--   0        0        0      394 2023-05-05 09:17:20.322797 twyn-0.20.0/src/twyn/trusted_packages/exceptions.py
--rw-r--r--   0        0        0     2009 2023-05-05 09:17:20.322797 twyn-0.20.0/src/twyn/trusted_packages/references.py
--rw-r--r--   0        0        0     1907 2023-05-05 09:17:20.322797 twyn-0.20.0/src/twyn/trusted_packages/selectors.py
--rw-r--r--   0        0        0     2816 2023-05-05 09:17:20.322797 twyn-0.20.0/src/twyn/trusted_packages/trusted_packages.py
--rw-r--r--   0        0        0     4044 1970-01-01 00:00:00.000000 twyn-0.20.0/PKG-INFO
+-rw-r--r--   0        0        0     1081 2023-05-05 09:29:05.914574 twyn-0.20.1/LICENSE
+-rw-r--r--   0        0        0     3373 2023-05-05 09:29:05.914574 twyn-0.20.1/README.md
+-rw-r--r--   0        0        0     1938 2023-05-05 09:29:05.918574 twyn-0.20.1/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-05-05 09:29:05.918574 twyn-0.20.1/src/twyn/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-05 09:29:05.918574 twyn-0.20.1/src/twyn/base/__init__.py
+-rw-r--r--   0        0        0      942 2023-05-05 09:29:05.918574 twyn-0.20.1/src/twyn/base/constants.py
+-rw-r--r--   0        0        0      147 2023-05-05 09:29:05.918574 twyn-0.20.1/src/twyn/base/exceptions.py
+-rw-r--r--   0        0        0     2331 2023-05-05 09:29:05.918574 twyn-0.20.1/src/twyn/cli.py
+-rw-r--r--   0        0        0        0 2023-05-05 09:29:05.918574 twyn-0.20.1/src/twyn/core/__init__.py
+-rw-r--r--   0        0        0     3298 2023-05-05 09:29:05.918574 twyn-0.20.1/src/twyn/core/config_handler.py
+-rw-r--r--   0        0        0      513 2023-05-05 09:29:05.918574 twyn-0.20.1/src/twyn/core/exceptions.py
+-rw-r--r--   0        0        0      221 2023-05-05 09:29:05.918574 twyn-0.20.1/src/twyn/dependency_parser/__init__.py
+-rw-r--r--   0        0        0     1463 2023-05-05 09:29:05.918574 twyn-0.20.1/src/twyn/dependency_parser/abstract_parser.py
+-rw-r--r--   0        0        0     2149 2023-05-05 09:29:05.918574 twyn-0.20.1/src/twyn/dependency_parser/dependency_selector.py
+-rw-r--r--   0        0        0      554 2023-05-05 09:29:05.918574 twyn-0.20.1/src/twyn/dependency_parser/exceptions.py
+-rw-r--r--   0        0        0      761 2023-05-05 09:29:05.918574 twyn-0.20.1/src/twyn/dependency_parser/poetry_lock.py
+-rw-r--r--   0        0        0      804 2023-05-05 09:29:05.918574 twyn-0.20.1/src/twyn/dependency_parser/requirements_txt.py
+-rw-r--r--   0        0        0     5114 2023-05-05 09:29:05.918574 twyn-0.20.1/src/twyn/main.py
+-rw-r--r--   0        0        0        0 2023-05-05 09:29:05.918574 twyn-0.20.1/src/twyn/similarity/__init__.py
+-rw-r--r--   0        0        0     2210 2023-05-05 09:29:05.918574 twyn-0.20.1/src/twyn/similarity/algorithm.py
+-rw-r--r--   0        0        0      275 2023-05-05 09:29:05.918574 twyn-0.20.1/src/twyn/similarity/exceptions.py
+-rw-r--r--   0        0        0      189 2023-05-05 09:29:05.918574 twyn-0.20.1/src/twyn/trusted_packages/__init__.py
+-rw-r--r--   0        0        0     1497 2023-05-05 09:29:05.918574 twyn-0.20.1/src/twyn/trusted_packages/constants.py
+-rw-r--r--   0        0        0      394 2023-05-05 09:29:05.918574 twyn-0.20.1/src/twyn/trusted_packages/exceptions.py
+-rw-r--r--   0        0        0     2009 2023-05-05 09:29:05.918574 twyn-0.20.1/src/twyn/trusted_packages/references.py
+-rw-r--r--   0        0        0     1907 2023-05-05 09:29:05.918574 twyn-0.20.1/src/twyn/trusted_packages/selectors.py
+-rw-r--r--   0        0        0     2816 2023-05-05 09:29:05.918574 twyn-0.20.1/src/twyn/trusted_packages/trusted_packages.py
+-rw-r--r--   0        0        0     4055 1970-01-01 00:00:00.000000 twyn-0.20.1/PKG-INFO
```

### Comparing `twyn-0.20.0/LICENSE` & `twyn-0.20.1/LICENSE`

 * *Files identical despite different names*

### Comparing `twyn-0.20.0/README.md` & `twyn-0.20.1/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # Twyn
 
 ![Build Status](https://github.com/elementsinteractive/twyn/actions/workflows/test.yml/badge.svg)
 [![PyPI version](https://img.shields.io/pypi/v/twyn)](https://pypi.org/project/twyn/)
 [![Python Version](https://img.shields.io/pypi/pyversions/twyn?logo=python&logoColor=yellow)](https://pypi.org/project/twyn/)
 ![Code style](https://img.shields.io/badge/code%20style-black-000000.svg)
-[![License](https://img.shields.io/github/license/elementsinteractive/twyn)](LICENSE)
+[![License](https://github.com/elementsinteractive/typpel-migration/blob/main/LICENSE)](LICENSE)
 
 Twyn is a security tool that compares the name of your dependencies against a set of the most popular ones, 
 in order to determine if there is any similarity between them, preventing you from using a potentially illegitimate one.
 In short, Twyn protects you against [typosquatting attacks](https://en.wikipedia.org/wiki/Typosquatting).
 
 
 It works as follows:
```

### Comparing `twyn-0.20.0/pyproject.toml` & `twyn-0.20.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "twyn"
-version = "0.20.0"
+version = "0.20.1"
 description = ""
 authors = ["Daniel Sanz, Sergio Castillo, Ludo van Orden, Dmitrii Fedotov"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = ">=3.9,<4"
 requests = "^2.28.2"
@@ -95,9 +95,9 @@
 [tool.coverage.report]
 fail_under = 95
 exclude_lines = ["if TYPE_CHECKING:", "pragma: no cover"]
 
 
 [tool.commitizen]
 version_files = ["pyproject.toml:version"]
-version = "0.20.0"
+version = "0.20.1"
 tag_format = "v$version"
```

### Comparing `twyn-0.20.0/src/twyn/base/constants.py` & `twyn-0.20.1/src/twyn/base/constants.py`

 * *Files identical despite different names*

### Comparing `twyn-0.20.0/src/twyn/cli.py` & `twyn-0.20.1/src/twyn/cli.py`

 * *Files identical despite different names*

### Comparing `twyn-0.20.0/src/twyn/core/config_handler.py` & `twyn-0.20.1/src/twyn/core/config_handler.py`

 * *Files identical despite different names*

### Comparing `twyn-0.20.0/src/twyn/core/exceptions.py` & `twyn-0.20.1/src/twyn/core/exceptions.py`

 * *Files identical despite different names*

### Comparing `twyn-0.20.0/src/twyn/dependency_parser/abstract_parser.py` & `twyn-0.20.1/src/twyn/dependency_parser/abstract_parser.py`

 * *Files identical despite different names*

### Comparing `twyn-0.20.0/src/twyn/dependency_parser/dependency_selector.py` & `twyn-0.20.1/src/twyn/dependency_parser/dependency_selector.py`

 * *Files identical despite different names*

### Comparing `twyn-0.20.0/src/twyn/dependency_parser/exceptions.py` & `twyn-0.20.1/src/twyn/dependency_parser/exceptions.py`

 * *Files identical despite different names*

### Comparing `twyn-0.20.0/src/twyn/dependency_parser/poetry_lock.py` & `twyn-0.20.1/src/twyn/dependency_parser/poetry_lock.py`

 * *Files identical despite different names*

### Comparing `twyn-0.20.0/src/twyn/dependency_parser/requirements_txt.py` & `twyn-0.20.1/src/twyn/dependency_parser/requirements_txt.py`

 * *Files identical despite different names*

### Comparing `twyn-0.20.0/src/twyn/main.py` & `twyn-0.20.1/src/twyn/main.py`

 * *Files identical despite different names*

### Comparing `twyn-0.20.0/src/twyn/similarity/algorithm.py` & `twyn-0.20.1/src/twyn/similarity/algorithm.py`

 * *Files identical despite different names*

### Comparing `twyn-0.20.0/src/twyn/trusted_packages/constants.py` & `twyn-0.20.1/src/twyn/trusted_packages/constants.py`

 * *Files identical despite different names*

### Comparing `twyn-0.20.0/src/twyn/trusted_packages/references.py` & `twyn-0.20.1/src/twyn/trusted_packages/references.py`

 * *Files identical despite different names*

### Comparing `twyn-0.20.0/src/twyn/trusted_packages/selectors.py` & `twyn-0.20.1/src/twyn/trusted_packages/selectors.py`

 * *Files identical despite different names*

### Comparing `twyn-0.20.0/src/twyn/trusted_packages/trusted_packages.py` & `twyn-0.20.1/src/twyn/trusted_packages/trusted_packages.py`

 * *Files identical despite different names*

### Comparing `twyn-0.20.0/PKG-INFO` & `twyn-0.20.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: twyn
-Version: 0.20.0
+Version: 0.20.1
 Summary: 
 Author: Daniel Sanz, Sergio Castillo, Ludo van Orden, Dmitrii Fedotov
 Requires-Python: >=3.9,<4
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
@@ -19,15 +19,15 @@
 
 # Twyn
 
 ![Build Status](https://github.com/elementsinteractive/twyn/actions/workflows/test.yml/badge.svg)
 [![PyPI version](https://img.shields.io/pypi/v/twyn)](https://pypi.org/project/twyn/)
 [![Python Version](https://img.shields.io/pypi/pyversions/twyn?logo=python&logoColor=yellow)](https://pypi.org/project/twyn/)
 ![Code style](https://img.shields.io/badge/code%20style-black-000000.svg)
-[![License](https://img.shields.io/github/license/elementsinteractive/twyn)](LICENSE)
+[![License](https://github.com/elementsinteractive/typpel-migration/blob/main/LICENSE)](LICENSE)
 
 Twyn is a security tool that compares the name of your dependencies against a set of the most popular ones, 
 in order to determine if there is any similarity between them, preventing you from using a potentially illegitimate one.
 In short, Twyn protects you against [typosquatting attacks](https://en.wikipedia.org/wiki/Typosquatting).
 
 
 It works as follows:
```

