# Comparing `tmp/pyFCST-0.0.10.tar.gz` & `tmp/pyFCST-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyFCST-0.0.10.tar", last modified: Fri May  5 16:18:26 2023, max compression
+gzip compressed data, was "pyFCST-0.0.9.tar", last modified: Fri May  5 02:41:51 2023, max compression
```

## Comparing `pyFCST-0.0.10.tar` & `pyFCST-0.0.9.tar`

### file list

```diff
@@ -1,28 +1,24 @@
-drwxrwxr-x   0 james     (1000) james     (1000)        0 2023-05-05 16:18:26.120084 pyFCST-0.0.10/
--rw-rw-r--   0 james     (1000) james     (1000)      113 2023-05-04 22:17:05.000000 pyFCST-0.0.10/AUTHORS.rst
--rw-rw-r--   0 james     (1000) james     (1000)     1078 2023-05-04 22:17:13.000000 pyFCST-0.0.10/LICENSE
--rw-rw-r--   0 james     (1000) james     (1000)      172 2023-05-05 16:16:28.000000 pyFCST-0.0.10/MANIFEST.in
--rw-rw-r--   0 james     (1000) james     (1000)      559 2023-05-05 16:18:26.120084 pyFCST-0.0.10/PKG-INFO
--rw-rw-r--   0 james     (1000) james     (1000)       68 2023-05-04 21:44:54.000000 pyFCST-0.0.10/README.md
--rw-rw-r--   0 james     (1000) james     (1000)       68 2023-05-04 21:44:54.000000 pyFCST-0.0.10/README.rst
-drwxrwxr-x   0 james     (1000) james     (1000)        0 2023-05-05 16:18:26.120084 pyFCST-0.0.10/pyFCST/
--rw-rw-r--   0 james     (1000) james     (1000)       66 2023-05-05 16:08:24.000000 pyFCST-0.0.10/pyFCST/__init__.py
-drwxrwxr-x   0 james     (1000) james     (1000)        0 2023-05-05 16:18:26.120084 pyFCST-0.0.10/pyFCST/ips/
--rw-rw-r--   0 james     (1000) james     (1000)       52 2023-05-05 16:04:26.000000 pyFCST-0.0.10/pyFCST/ips/__init__.py
-drwxrwxr-x   0 james     (1000) james     (1000)        0 2023-05-05 16:18:26.120084 pyFCST-0.0.10/pyFCST/ips/analysis/
--rw-rw-r--   0 james     (1000) james     (1000)       33 2023-05-05 16:04:39.000000 pyFCST-0.0.10/pyFCST/ips/analysis/__init__.py
-drwxrwxr-x   0 james     (1000) james     (1000)        0 2023-05-05 16:18:26.120084 pyFCST-0.0.10/pyFCST/ips/inout/
--rw-rw-r--   0 james     (1000) james     (1000)       67 2023-05-05 16:05:26.000000 pyFCST-0.0.10/pyFCST/ips/inout/__init__.py
-drwxrwxr-x   0 james     (1000) james     (1000)        0 2023-05-05 16:18:26.120084 pyFCST-0.0.10/pyFCST/mesh/
--rw-rw-r--   0 james     (1000) james     (1000)       63 2023-05-05 16:00:43.000000 pyFCST-0.0.10/pyFCST/mesh/__init__.py
-drwxrwxr-x   0 james     (1000) james     (1000)        0 2023-05-05 16:18:26.120084 pyFCST-0.0.10/pyFCST/util/
--rw-rw-r--   0 james     (1000) james     (1000)       29 2023-05-05 03:26:52.000000 pyFCST-0.0.10/pyFCST/util/__init__.py
-drwxrwxr-x   0 james     (1000) james     (1000)        0 2023-05-05 16:18:26.120084 pyFCST-0.0.10/pyFCST.egg-info/
--rw-rw-r--   0 james     (1000) james     (1000)      559 2023-05-05 16:18:25.000000 pyFCST-0.0.10/pyFCST.egg-info/PKG-INFO
--rw-rw-r--   0 james     (1000) james     (1000)      386 2023-05-05 16:18:26.000000 pyFCST-0.0.10/pyFCST.egg-info/SOURCES.txt
--rw-rw-r--   0 james     (1000) james     (1000)        1 2023-05-05 16:18:25.000000 pyFCST-0.0.10/pyFCST.egg-info/dependency_links.txt
--rw-rw-r--   0 james     (1000) james     (1000)      229 2023-05-05 16:18:25.000000 pyFCST-0.0.10/pyFCST.egg-info/requires.txt
--rw-rw-r--   0 james     (1000) james     (1000)        7 2023-05-05 16:18:25.000000 pyFCST-0.0.10/pyFCST.egg-info/top_level.txt
--rw-rw-r--   0 james     (1000) james     (1000)      846 2023-05-05 16:17:36.000000 pyFCST-0.0.10/pyproject.toml
--rw-rw-r--   0 james     (1000) james     (1000)       38 2023-05-05 16:18:26.120084 pyFCST-0.0.10/setup.cfg
--rw-rw-r--   0 james     (1000) james     (1000)      861 2023-05-05 16:17:26.000000 pyFCST-0.0.10/setup.py
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

### Comparing `pyFCST-0.0.10/LICENSE` & `pyFCST-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `pyFCST-0.0.10/PKG-INFO` & `pyFCST-0.0.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyFCST
-Version: 0.0.10
+Version: 0.0.9
 Summary: Utilities for pyFCST
 Home-page: http://pypi.python.org/pypi/pyfcst/
 Author: FCST development group
 Author-email: FCST_DEVELOPERS <jwoodfor@ualberta.ca>
 License: LICENSE.txt
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `pyFCST-0.0.10/pyFCST.egg-info/PKG-INFO` & `pyFCST-0.0.9/pyFCST.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyFCST
-Version: 0.0.10
+Version: 0.0.9
 Summary: Utilities for pyFCST
 Home-page: http://pypi.python.org/pypi/pyfcst/
 Author: FCST development group
 Author-email: FCST_DEVELOPERS <jwoodfor@ualberta.ca>
 License: LICENSE.txt
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `pyFCST-0.0.10/pyproject.toml` & `pyFCST-0.0.9/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -15,15 +15,15 @@
         "pyqt5 < 5.13",
         "pyqtwebengine < 5.13",
         "parso == 0.7.0"
     ]
 build-backend="setuptools.build_meta"
 [project]
 name = "pyFCST"
-version = "0.0.10"
+version = "0.0.9"
 authors = [
   { name="FCST_DEVELOPERS", email="jwoodfor@ualberta.ca" },
 ]
 description = "Utilities for pyFCST"
 readme = "README.md"
 requires-python = ">=3.6"
 classifiers = [
```

### Comparing `pyFCST-0.0.10/setup.py` & `pyFCST-0.0.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup
 from distutils.core import setup
 
 setup(
     name='pyFCST',
-    version='0.0.10',
+    version='0.0.5',
     author='FCST development group',
     author_email='jwoodfor@ualberta.ca',
     packages=['pyFCST'],
     python_requires='>=3.6',
     url='http://pypi.python.org/pypi/pyfcst/',
     license='LICENSE.txt',
     description='Utilities for pyFCST.',
```

