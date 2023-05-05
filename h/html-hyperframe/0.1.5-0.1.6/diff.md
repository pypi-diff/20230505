# Comparing `tmp/html_hyperframe-0.1.5.tar.gz` & `tmp/html_hyperframe-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "html_hyperframe-0.1.5.tar", max compression
+gzip compressed data, was "html_hyperframe-0.1.6.tar", max compression
```

## Comparing `html_hyperframe-0.1.5.tar` & `html_hyperframe-0.1.6.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0    11344 2023-05-05 13:05:35.062134 html_hyperframe-0.1.5/LICENSE
--rw-r--r--   0        0        0     2834 2023-05-05 13:05:35.062134 html_hyperframe-0.1.5/README.md
--rw-r--r--   0        0        0      347 2023-05-05 13:05:35.062134 html_hyperframe-0.1.5/hyperframe/__init__.py
--rw-r--r--   0        0        0     4294 2023-05-05 13:05:35.062134 html_hyperframe-0.1.5/hyperframe/hyperpattern.py
--rw-r--r--   0        0        0        0 2023-05-05 13:05:35.062134 html_hyperframe-0.1.5/hyperframe/py.typed
--rw-r--r--   0        0        0     4599 2023-05-05 13:05:35.062134 html_hyperframe-0.1.5/hyperframe/tabulate.py
--rw-r--r--   0        0        0     1004 2023-05-05 13:05:35.062134 html_hyperframe-0.1.5/pyproject.toml
--rw-r--r--   0        0        0     3796 1970-01-01 00:00:00.000000 html_hyperframe-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0    11344 2023-05-05 15:46:02.767553 html_hyperframe-0.1.6/LICENSE
+-rw-r--r--   0        0        0     2834 2023-05-05 15:46:02.767553 html_hyperframe-0.1.6/README.md
+-rw-r--r--   0        0        0      347 2023-05-05 15:46:02.767553 html_hyperframe-0.1.6/hyperframe/__init__.py
+-rw-r--r--   0        0        0     4294 2023-05-05 15:46:02.767553 html_hyperframe-0.1.6/hyperframe/hyperpattern.py
+-rw-r--r--   0        0        0        0 2023-05-05 15:46:02.767553 html_hyperframe-0.1.6/hyperframe/py.typed
+-rw-r--r--   0        0        0     4599 2023-05-05 15:46:02.767553 html_hyperframe-0.1.6/hyperframe/tabulate.py
+-rw-r--r--   0        0        0     1004 2023-05-05 15:46:02.767553 html_hyperframe-0.1.6/pyproject.toml
+-rw-r--r--   0        0        0     3796 1970-01-01 00:00:00.000000 html_hyperframe-0.1.6/PKG-INFO
```

### Comparing `html_hyperframe-0.1.5/LICENSE` & `html_hyperframe-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `html_hyperframe-0.1.5/README.md` & `html_hyperframe-0.1.6/README.md`

 * *Files identical despite different names*

### Comparing `html_hyperframe-0.1.5/hyperframe/hyperpattern.py` & `html_hyperframe-0.1.6/hyperframe/hyperpattern.py`

 * *Files identical despite different names*

### Comparing `html_hyperframe-0.1.5/hyperframe/tabulate.py` & `html_hyperframe-0.1.6/hyperframe/tabulate.py`

 * *Files identical despite different names*

### Comparing `html_hyperframe-0.1.5/pyproject.toml` & `html_hyperframe-0.1.6/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.poetry]
 name = "html-hyperframe"
-version = "0.1.5"
+version = "0.1.6"
 description = ""
 authors = ["SamB <58937194+sam-lawrence@users.noreply.github.com>"]
 readme = "README.md"
 repository = "https://github.com/sam-lawrence/HyperFrame"
 classifiers = [
     "Operating System :: OS Independent",
     "Programming Language :: Python :: 3",
```

### Comparing `html_hyperframe-0.1.5/PKG-INFO` & `html_hyperframe-0.1.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: html-hyperframe
-Version: 0.1.5
+Version: 0.1.6
 Summary: 
 Home-page: https://github.com/sam-lawrence/HyperFrame
 Author: SamB
 Author-email: 58937194+sam-lawrence@users.noreply.github.com
 Requires-Python: >=3.9,<4.0
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
```

