# Comparing `tmp/pyFCST-0.0.8.tar.gz` & `tmp/pyFCST-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyFCST-0.0.8.tar", last modified: Fri May  5 02:10:41 2023, max compression
+gzip compressed data, was "pyFCST-0.0.9.tar", last modified: Fri May  5 02:41:51 2023, max compression
```

## Comparing `pyFCST-0.0.8.tar` & `pyFCST-0.0.9.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxr-x   0 james     (1000) james     (1000)        0 2023-05-05 02:10:41.405663 pyFCST-0.0.8/
--rw-rw-r--   0 james     (1000) james     (1000)      113 2023-05-04 22:17:05.000000 pyFCST-0.0.8/AUTHORS.rst
--rw-rw-r--   0 james     (1000) james     (1000)     1078 2023-05-04 22:17:13.000000 pyFCST-0.0.8/LICENSE
--rw-rw-r--   0 james     (1000) james     (1000)      123 2023-05-05 02:09:28.000000 pyFCST-0.0.8/MANIFEST.in
--rw-rw-r--   0 james     (1000) james     (1000)      558 2023-05-05 02:10:41.405663 pyFCST-0.0.8/PKG-INFO
--rw-rw-r--   0 james     (1000) james     (1000)       68 2023-05-04 21:44:54.000000 pyFCST-0.0.8/README.md
--rw-rw-r--   0 james     (1000) james     (1000)       68 2023-05-04 21:44:54.000000 pyFCST-0.0.8/README.rst
-drwxrwxr-x   0 james     (1000) james     (1000)        0 2023-05-05 02:10:41.405663 pyFCST-0.0.8/pyFCST/
--rw-rw-r--   0 james     (1000) james     (1000)      192 2023-05-05 02:08:55.000000 pyFCST-0.0.8/pyFCST/__init__.py
-drwxrwxr-x   0 james     (1000) james     (1000)        0 2023-05-05 02:10:41.405663 pyFCST-0.0.8/pyFCST/mesh/
--rw-rw-r--   0 james     (1000) james     (1000)       86 2023-05-05 01:54:52.000000 pyFCST-0.0.8/pyFCST/mesh/__init__.py
-drwxrwxr-x   0 james     (1000) james     (1000)        0 2023-05-05 02:10:41.405663 pyFCST-0.0.8/pyFCST/util/
--rw-rw-r--   0 james     (1000) james     (1000)       50 2023-05-05 01:55:14.000000 pyFCST-0.0.8/pyFCST/util/__init__.py
-drwxrwxr-x   0 james     (1000) james     (1000)        0 2023-05-05 02:10:41.405663 pyFCST-0.0.8/pyFCST/visu/
--rw-rw-r--   0 james     (1000) james     (1000)       31 2023-05-05 01:55:33.000000 pyFCST-0.0.8/pyFCST/visu/__init__.py
-drwxrwxr-x   0 james     (1000) james     (1000)        0 2023-05-05 02:10:41.405663 pyFCST-0.0.8/pyFCST.egg-info/
--rw-rw-r--   0 james     (1000) james     (1000)      558 2023-05-05 02:10:41.000000 pyFCST-0.0.8/pyFCST.egg-info/PKG-INFO
--rw-rw-r--   0 james     (1000) james     (1000)      326 2023-05-05 02:10:41.000000 pyFCST-0.0.8/pyFCST.egg-info/SOURCES.txt
--rw-rw-r--   0 james     (1000) james     (1000)        1 2023-05-05 02:10:41.000000 pyFCST-0.0.8/pyFCST.egg-info/dependency_links.txt
--rw-rw-r--   0 james     (1000) james     (1000)      229 2023-05-05 02:10:41.000000 pyFCST-0.0.8/pyFCST.egg-info/requires.txt
--rw-rw-r--   0 james     (1000) james     (1000)        7 2023-05-05 02:10:41.000000 pyFCST-0.0.8/pyFCST.egg-info/top_level.txt
--rw-rw-r--   0 james     (1000) james     (1000)      845 2023-05-05 02:09:57.000000 pyFCST-0.0.8/pyproject.toml
--rw-rw-r--   0 james     (1000) james     (1000)       38 2023-05-05 02:10:41.405663 pyFCST-0.0.8/setup.cfg
--rw-rw-r--   0 james     (1000) james     (1000)      860 2023-05-05 00:44:21.000000 pyFCST-0.0.8/setup.py
+drwxrwxr-x   0 james     (1000) james     (1000)        0 2023-05-05 02:41:51.805120 pyFCST-0.0.9/
+-rw-rw-r--   0 james     (1000) james     (1000)      113 2023-05-04 22:17:05.000000 pyFCST-0.0.9/AUTHORS.rst
+-rw-rw-r--   0 james     (1000) james     (1000)     1078 2023-05-04 22:17:13.000000 pyFCST-0.0.9/LICENSE
+-rw-rw-r--   0 james     (1000) james     (1000)      123 2023-05-05 02:09:28.000000 pyFCST-0.0.9/MANIFEST.in
+-rw-rw-r--   0 james     (1000) james     (1000)      558 2023-05-05 02:41:51.805120 pyFCST-0.0.9/PKG-INFO
+-rw-rw-r--   0 james     (1000) james     (1000)       68 2023-05-04 21:44:54.000000 pyFCST-0.0.9/README.md
+-rw-rw-r--   0 james     (1000) james     (1000)       68 2023-05-04 21:44:54.000000 pyFCST-0.0.9/README.rst
+drwxrwxr-x   0 james     (1000) james     (1000)        0 2023-05-05 02:41:51.805120 pyFCST-0.0.9/pyFCST/
+-rw-rw-r--   0 james     (1000) james     (1000)       67 2023-05-05 02:15:57.000000 pyFCST-0.0.9/pyFCST/__init__.py
+drwxrwxr-x   0 james     (1000) james     (1000)        0 2023-05-05 02:41:51.805120 pyFCST-0.0.9/pyFCST/mesh/
+-rw-rw-r--   0 james     (1000) james     (1000)       89 2023-05-05 02:16:07.000000 pyFCST-0.0.9/pyFCST/mesh/__init__.py
+drwxrwxr-x   0 james     (1000) james     (1000)        0 2023-05-05 02:41:51.805120 pyFCST-0.0.9/pyFCST/util/
+-rw-rw-r--   0 james     (1000) james     (1000)       52 2023-05-05 02:16:16.000000 pyFCST-0.0.9/pyFCST/util/__init__.py
+drwxrwxr-x   0 james     (1000) james     (1000)        0 2023-05-05 02:41:51.805120 pyFCST-0.0.9/pyFCST/visu/
+-rw-rw-r--   0 james     (1000) james     (1000)       32 2023-05-05 02:16:23.000000 pyFCST-0.0.9/pyFCST/visu/__init__.py
+drwxrwxr-x   0 james     (1000) james     (1000)        0 2023-05-05 02:41:51.805120 pyFCST-0.0.9/pyFCST.egg-info/
+-rw-rw-r--   0 james     (1000) james     (1000)      558 2023-05-05 02:41:51.000000 pyFCST-0.0.9/pyFCST.egg-info/PKG-INFO
+-rw-rw-r--   0 james     (1000) james     (1000)      326 2023-05-05 02:41:51.000000 pyFCST-0.0.9/pyFCST.egg-info/SOURCES.txt
+-rw-rw-r--   0 james     (1000) james     (1000)        1 2023-05-05 02:41:51.000000 pyFCST-0.0.9/pyFCST.egg-info/dependency_links.txt
+-rw-rw-r--   0 james     (1000) james     (1000)      229 2023-05-05 02:41:51.000000 pyFCST-0.0.9/pyFCST.egg-info/requires.txt
+-rw-rw-r--   0 james     (1000) james     (1000)        7 2023-05-05 02:41:51.000000 pyFCST-0.0.9/pyFCST.egg-info/top_level.txt
+-rw-rw-r--   0 james     (1000) james     (1000)      845 2023-05-05 02:41:02.000000 pyFCST-0.0.9/pyproject.toml
+-rw-rw-r--   0 james     (1000) james     (1000)       38 2023-05-05 02:41:51.805120 pyFCST-0.0.9/setup.cfg
+-rw-rw-r--   0 james     (1000) james     (1000)      860 2023-05-05 00:44:21.000000 pyFCST-0.0.9/setup.py
```

### Comparing `pyFCST-0.0.8/LICENSE` & `pyFCST-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `pyFCST-0.0.8/PKG-INFO` & `pyFCST-0.0.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyFCST
-Version: 0.0.8
+Version: 0.0.9
 Summary: Utilities for pyFCST
 Home-page: http://pypi.python.org/pypi/pyfcst/
 Author: FCST development group
 Author-email: FCST_DEVELOPERS <jwoodfor@ualberta.ca>
 License: LICENSE.txt
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `pyFCST-0.0.8/pyFCST.egg-info/PKG-INFO` & `pyFCST-0.0.9/pyFCST.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyFCST
-Version: 0.0.8
+Version: 0.0.9
 Summary: Utilities for pyFCST
 Home-page: http://pypi.python.org/pypi/pyfcst/
 Author: FCST development group
 Author-email: FCST_DEVELOPERS <jwoodfor@ualberta.ca>
 License: LICENSE.txt
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `pyFCST-0.0.8/pyproject.toml` & `pyFCST-0.0.9/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -15,15 +15,15 @@
         "pyqt5 < 5.13",
         "pyqtwebengine < 5.13",
         "parso == 0.7.0"
     ]
 build-backend="setuptools.build_meta"
 [project]
 name = "pyFCST"
-version = "0.0.8"
+version = "0.0.9"
 authors = [
   { name="FCST_DEVELOPERS", email="jwoodfor@ualberta.ca" },
 ]
 description = "Utilities for pyFCST"
 readme = "README.md"
 requires-python = ">=3.6"
 classifiers = [
```

### Comparing `pyFCST-0.0.8/setup.py` & `pyFCST-0.0.9/setup.py`

 * *Files identical despite different names*

