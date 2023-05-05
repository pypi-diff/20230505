# Comparing `tmp/pyFCST-0.0.7.tar.gz` & `tmp/pyFCST-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyFCST-0.0.7.tar", last modified: Fri May  5 01:57:33 2023, max compression
+gzip compressed data, was "pyFCST-0.0.8.tar", last modified: Fri May  5 02:10:41 2023, max compression
```

## Comparing `pyFCST-0.0.7.tar` & `pyFCST-0.0.8.tar`

### file list

```diff
@@ -1,18 +1,24 @@
-drwxrwxr-x   0 james     (1000) james     (1000)        0 2023-05-05 01:57:33.115634 pyFCST-0.0.7/
--rw-rw-r--   0 james     (1000) james     (1000)      113 2023-05-04 22:17:05.000000 pyFCST-0.0.7/AUTHORS.rst
--rw-rw-r--   0 james     (1000) james     (1000)     1078 2023-05-04 22:17:13.000000 pyFCST-0.0.7/LICENSE
--rw-rw-r--   0 james     (1000) james     (1000)       96 2023-05-05 01:56:17.000000 pyFCST-0.0.7/MANIFEST.in
--rw-rw-r--   0 james     (1000) james     (1000)      558 2023-05-05 01:57:33.115634 pyFCST-0.0.7/PKG-INFO
--rw-rw-r--   0 james     (1000) james     (1000)       68 2023-05-04 21:44:54.000000 pyFCST-0.0.7/README.md
--rw-rw-r--   0 james     (1000) james     (1000)       68 2023-05-04 21:44:54.000000 pyFCST-0.0.7/README.rst
-drwxrwxr-x   0 james     (1000) james     (1000)        0 2023-05-05 01:57:33.111633 pyFCST-0.0.7/pyFCST/
--rw-rw-r--   0 james     (1000) james     (1000)        5 2023-05-05 01:54:14.000000 pyFCST-0.0.7/pyFCST/__init__.py
-drwxrwxr-x   0 james     (1000) james     (1000)        0 2023-05-05 01:57:33.115634 pyFCST-0.0.7/pyFCST.egg-info/
--rw-rw-r--   0 james     (1000) james     (1000)      558 2023-05-05 01:57:33.000000 pyFCST-0.0.7/pyFCST.egg-info/PKG-INFO
--rw-rw-r--   0 james     (1000) james     (1000)      254 2023-05-05 01:57:33.000000 pyFCST-0.0.7/pyFCST.egg-info/SOURCES.txt
--rw-rw-r--   0 james     (1000) james     (1000)        1 2023-05-05 01:57:33.000000 pyFCST-0.0.7/pyFCST.egg-info/dependency_links.txt
--rw-rw-r--   0 james     (1000) james     (1000)      229 2023-05-05 01:57:33.000000 pyFCST-0.0.7/pyFCST.egg-info/requires.txt
--rw-rw-r--   0 james     (1000) james     (1000)        7 2023-05-05 01:57:33.000000 pyFCST-0.0.7/pyFCST.egg-info/top_level.txt
--rw-rw-r--   0 james     (1000) james     (1000)      845 2023-05-05 01:56:33.000000 pyFCST-0.0.7/pyproject.toml
--rw-rw-r--   0 james     (1000) james     (1000)       38 2023-05-05 01:57:33.115634 pyFCST-0.0.7/setup.cfg
--rw-rw-r--   0 james     (1000) james     (1000)      860 2023-05-05 00:44:21.000000 pyFCST-0.0.7/setup.py
+drwxrwxr-x   0 james     (1000) james     (1000)        0 2023-05-05 02:10:41.405663 pyFCST-0.0.8/
+-rw-rw-r--   0 james     (1000) james     (1000)      113 2023-05-04 22:17:05.000000 pyFCST-0.0.8/AUTHORS.rst
+-rw-rw-r--   0 james     (1000) james     (1000)     1078 2023-05-04 22:17:13.000000 pyFCST-0.0.8/LICENSE
+-rw-rw-r--   0 james     (1000) james     (1000)      123 2023-05-05 02:09:28.000000 pyFCST-0.0.8/MANIFEST.in
+-rw-rw-r--   0 james     (1000) james     (1000)      558 2023-05-05 02:10:41.405663 pyFCST-0.0.8/PKG-INFO
+-rw-rw-r--   0 james     (1000) james     (1000)       68 2023-05-04 21:44:54.000000 pyFCST-0.0.8/README.md
+-rw-rw-r--   0 james     (1000) james     (1000)       68 2023-05-04 21:44:54.000000 pyFCST-0.0.8/README.rst
+drwxrwxr-x   0 james     (1000) james     (1000)        0 2023-05-05 02:10:41.405663 pyFCST-0.0.8/pyFCST/
+-rw-rw-r--   0 james     (1000) james     (1000)      192 2023-05-05 02:08:55.000000 pyFCST-0.0.8/pyFCST/__init__.py
+drwxrwxr-x   0 james     (1000) james     (1000)        0 2023-05-05 02:10:41.405663 pyFCST-0.0.8/pyFCST/mesh/
+-rw-rw-r--   0 james     (1000) james     (1000)       86 2023-05-05 01:54:52.000000 pyFCST-0.0.8/pyFCST/mesh/__init__.py
+drwxrwxr-x   0 james     (1000) james     (1000)        0 2023-05-05 02:10:41.405663 pyFCST-0.0.8/pyFCST/util/
+-rw-rw-r--   0 james     (1000) james     (1000)       50 2023-05-05 01:55:14.000000 pyFCST-0.0.8/pyFCST/util/__init__.py
+drwxrwxr-x   0 james     (1000) james     (1000)        0 2023-05-05 02:10:41.405663 pyFCST-0.0.8/pyFCST/visu/
+-rw-rw-r--   0 james     (1000) james     (1000)       31 2023-05-05 01:55:33.000000 pyFCST-0.0.8/pyFCST/visu/__init__.py
+drwxrwxr-x   0 james     (1000) james     (1000)        0 2023-05-05 02:10:41.405663 pyFCST-0.0.8/pyFCST.egg-info/
+-rw-rw-r--   0 james     (1000) james     (1000)      558 2023-05-05 02:10:41.000000 pyFCST-0.0.8/pyFCST.egg-info/PKG-INFO
+-rw-rw-r--   0 james     (1000) james     (1000)      326 2023-05-05 02:10:41.000000 pyFCST-0.0.8/pyFCST.egg-info/SOURCES.txt
+-rw-rw-r--   0 james     (1000) james     (1000)        1 2023-05-05 02:10:41.000000 pyFCST-0.0.8/pyFCST.egg-info/dependency_links.txt
+-rw-rw-r--   0 james     (1000) james     (1000)      229 2023-05-05 02:10:41.000000 pyFCST-0.0.8/pyFCST.egg-info/requires.txt
+-rw-rw-r--   0 james     (1000) james     (1000)        7 2023-05-05 02:10:41.000000 pyFCST-0.0.8/pyFCST.egg-info/top_level.txt
+-rw-rw-r--   0 james     (1000) james     (1000)      845 2023-05-05 02:09:57.000000 pyFCST-0.0.8/pyproject.toml
+-rw-rw-r--   0 james     (1000) james     (1000)       38 2023-05-05 02:10:41.405663 pyFCST-0.0.8/setup.cfg
+-rw-rw-r--   0 james     (1000) james     (1000)      860 2023-05-05 00:44:21.000000 pyFCST-0.0.8/setup.py
```

### Comparing `pyFCST-0.0.7/LICENSE` & `pyFCST-0.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `pyFCST-0.0.7/PKG-INFO` & `pyFCST-0.0.8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyFCST
-Version: 0.0.7
+Version: 0.0.8
 Summary: Utilities for pyFCST
 Home-page: http://pypi.python.org/pypi/pyfcst/
 Author: FCST development group
 Author-email: FCST_DEVELOPERS <jwoodfor@ualberta.ca>
 License: LICENSE.txt
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `pyFCST-0.0.7/pyFCST.egg-info/PKG-INFO` & `pyFCST-0.0.8/pyFCST.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyFCST
-Version: 0.0.7
+Version: 0.0.8
 Summary: Utilities for pyFCST
 Home-page: http://pypi.python.org/pypi/pyfcst/
 Author: FCST development group
 Author-email: FCST_DEVELOPERS <jwoodfor@ualberta.ca>
 License: LICENSE.txt
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `pyFCST-0.0.7/pyproject.toml` & `pyFCST-0.0.8/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -15,15 +15,15 @@
         "pyqt5 < 5.13",
         "pyqtwebengine < 5.13",
         "parso == 0.7.0"
     ]
 build-backend="setuptools.build_meta"
 [project]
 name = "pyFCST"
-version = "0.0.7"
+version = "0.0.8"
 authors = [
   { name="FCST_DEVELOPERS", email="jwoodfor@ualberta.ca" },
 ]
 description = "Utilities for pyFCST"
 readme = "README.md"
 requires-python = ">=3.6"
 classifiers = [
```

### Comparing `pyFCST-0.0.7/setup.py` & `pyFCST-0.0.8/setup.py`

 * *Files identical despite different names*

