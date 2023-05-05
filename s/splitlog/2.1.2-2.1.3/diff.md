# Comparing `tmp/splitlog-2.1.2.tar.gz` & `tmp/splitlog-2.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "splitlog-2.1.2.tar", max compression
+gzip compressed data, was "splitlog-2.1.3.tar", max compression
```

## Comparing `splitlog-2.1.2.tar` & `splitlog-2.1.3.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1097 2023-05-05 18:59:10.330361 splitlog-2.1.2/LICENSE
--rw-r--r--   0        0        0     1771 2023-05-05 18:59:10.330361 splitlog-2.1.2/README.md
--rw-r--r--   0        0        0     1163 2023-05-05 18:59:46.558156 splitlog-2.1.2/pyproject.toml
--rw-r--r--   0        0        0    11993 2023-05-05 18:59:10.330361 splitlog-2.1.2/splitlog/__init__.py
--rw-r--r--   0        0        0     3455 2023-05-05 18:59:10.330361 splitlog-2.1.2/splitlog/__main__.py
--rw-r--r--   0        0        0     7460 2023-05-05 18:59:10.330361 splitlog-2.1.2/splitlog/outputfolder.py
--rw-r--r--   0        0        0     3029 1970-01-01 00:00:00.000000 splitlog-2.1.2/PKG-INFO
+-rw-r--r--   0        0        0     1097 2023-05-05 21:03:37.087047 splitlog-2.1.3/LICENSE
+-rw-r--r--   0        0        0     1771 2023-05-05 21:03:37.087047 splitlog-2.1.3/README.md
+-rw-r--r--   0        0        0     1163 2023-05-05 21:03:51.395040 splitlog-2.1.3/pyproject.toml
+-rw-r--r--   0        0        0    11993 2023-05-05 21:03:37.087047 splitlog-2.1.3/splitlog/__init__.py
+-rw-r--r--   0        0        0     3455 2023-05-05 21:03:37.087047 splitlog-2.1.3/splitlog/__main__.py
+-rw-r--r--   0        0        0     7460 2023-05-05 21:03:37.087047 splitlog-2.1.3/splitlog/outputfolder.py
+-rw-r--r--   0        0        0     3029 1970-01-01 00:00:00.000000 splitlog-2.1.3/PKG-INFO
```

### Comparing `splitlog-2.1.2/LICENSE` & `splitlog-2.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `splitlog-2.1.2/README.md` & `splitlog-2.1.3/README.md`

 * *Files identical despite different names*

### Comparing `splitlog-2.1.2/pyproject.toml` & `splitlog-2.1.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "splitlog"
-version = "2.1.2"
+version = "2.1.3"
 description = "Utility to split aggregated logs from Apache Hadoop Yarn applications into a folder hierarchy"
 authors = ["Sebastian Klemke <pypi@nerdheim.de>"]
 license = "MIT"
 readme = "README.md"
 classifiers = [
     "Development Status :: 5 - Production/Stable",
     "Environment :: Console",
```

### Comparing `splitlog-2.1.2/splitlog/__init__.py` & `splitlog-2.1.3/splitlog/__init__.py`

 * *Files identical despite different names*

### Comparing `splitlog-2.1.2/splitlog/__main__.py` & `splitlog-2.1.3/splitlog/__main__.py`

 * *Files identical despite different names*

### Comparing `splitlog-2.1.2/splitlog/outputfolder.py` & `splitlog-2.1.3/splitlog/outputfolder.py`

 * *Files identical despite different names*

### Comparing `splitlog-2.1.2/PKG-INFO` & `splitlog-2.1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: splitlog
-Version: 2.1.2
+Version: 2.1.3
 Summary: Utility to split aggregated logs from Apache Hadoop Yarn applications into a folder hierarchy
 Home-page: https://github.com/splitlog/splitlog.git
 License: MIT
 Author: Sebastian Klemke
 Author-email: pypi@nerdheim.de
 Requires-Python: >=3.7.0,<4.0.0
 Classifier: Development Status :: 5 - Production/Stable
```

