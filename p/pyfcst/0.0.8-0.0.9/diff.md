# Comparing `tmp/pyfcst-0.0.8.tar.gz` & `tmp/pyfcst-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyfcst-0.0.8.tar", max compression
+gzip compressed data, was "pyfcst-0.0.9.tar", max compression
```

## Comparing `pyfcst-0.0.8.tar` & `pyfcst-0.0.9.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0     1078 2023-05-04 22:17:13.930214 pyfcst-0.0.8/LICENSE.txt
--rw-r--r--   0        0        0       68 2023-05-04 21:44:54.560223 pyfcst-0.0.8/README.md
--rw-r--r--   0        0        0       46 2023-05-05 16:42:50.512291 pyfcst-0.0.8/pyfcst/__init__.py
--rw-r--r--   0        0        0       52 2023-05-05 16:04:26.568156 pyfcst-0.0.8/pyfcst/ips/__init__.py
--rw-r--r--   0        0        0       33 2023-05-05 16:04:39.580397 pyfcst-0.0.8/pyfcst/ips/analysis/__init__.py
--rw-r--r--   0        0        0      173 2023-05-05 16:05:36.525416 pyfcst-0.0.8/pyfcst/ips/analysis/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0        0        0     5571 2023-05-05 16:05:36.525416 pyfcst-0.0.8/pyfcst/ips/analysis/__pycache__/distanceSD.cpython-38.pyc
--rw-r--r--   0        0        0     6166 2023-05-05 03:25:13.456073 pyfcst-0.0.8/pyfcst/ips/analysis/distanceSD.py
--rw-r--r--   0        0        0       67 2023-05-05 16:05:26.981249 pyfcst-0.0.8/pyfcst/ips/inout/__init__.py
--rw-r--r--   0        0        0      203 2023-05-05 16:05:36.301412 pyfcst-0.0.8/pyfcst/ips/inout/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0        0        0     7728 2023-05-05 16:05:36.301412 pyfcst-0.0.8/pyfcst/ips/inout/__pycache__/input.cpython-38.pyc
--rw-r--r--   0        0        0     4372 2023-05-05 16:05:36.525416 pyfcst-0.0.8/pyfcst/ips/inout/__pycache__/output.cpython-38.pyc
--rw-r--r--   0        0        0     1395 2023-05-05 16:05:36.525416 pyfcst-0.0.8/pyfcst/ips/inout/__pycache__/printlog.cpython-38.pyc
--rw-r--r--   0        0        0    11433 2023-02-22 23:48:52.000000 pyfcst-0.0.8/pyfcst/ips/inout/input.py
--rw-r--r--   0        0        0     4483 2023-02-22 23:48:52.000000 pyfcst-0.0.8/pyfcst/ips/inout/output.py
--rw-r--r--   0        0        0      875 2023-02-22 23:48:52.000000 pyfcst-0.0.8/pyfcst/ips/inout/printlog.py
--rw-r--r--   0        0        0       29 2023-05-05 03:26:52.003756 pyfcst-0.0.8/pyfcst/util/__init__.py
--rw-r--r--   0        0        0     4091 2023-05-04 21:09:44.163901 pyfcst-0.0.8/pyfcst/util/baseclass.py
--rw-r--r--   0        0        0      728 2023-05-05 17:22:15.408879 pyfcst-0.0.8/pyproject.toml
--rw-r--r--   0        0        0     1189 1970-01-01 00:00:00.000000 pyfcst-0.0.8/PKG-INFO
+-rw-r--r--   0        0        0     1078 2023-05-04 22:17:13.930214 pyfcst-0.0.9/LICENSE.txt
+-rw-r--r--   0        0        0       68 2023-05-04 21:44:54.560223 pyfcst-0.0.9/README.md
+-rw-r--r--   0        0        0       46 2023-05-05 16:42:50.512291 pyfcst-0.0.9/pyfcst/__init__.py
+-rw-r--r--   0        0        0       52 2023-05-05 16:04:26.568156 pyfcst-0.0.9/pyfcst/ips/__init__.py
+-rw-r--r--   0        0        0       33 2023-05-05 16:04:39.580397 pyfcst-0.0.9/pyfcst/ips/analysis/__init__.py
+-rw-r--r--   0        0        0      173 2023-05-05 16:05:36.525416 pyfcst-0.0.9/pyfcst/ips/analysis/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0        0        0     5571 2023-05-05 16:05:36.525416 pyfcst-0.0.9/pyfcst/ips/analysis/__pycache__/distanceSD.cpython-38.pyc
+-rw-r--r--   0        0        0     6166 2023-05-05 03:25:13.456073 pyfcst-0.0.9/pyfcst/ips/analysis/distanceSD.py
+-rw-r--r--   0        0        0       67 2023-05-05 16:05:26.981249 pyfcst-0.0.9/pyfcst/ips/inout/__init__.py
+-rw-r--r--   0        0        0      203 2023-05-05 16:05:36.301412 pyfcst-0.0.9/pyfcst/ips/inout/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0        0        0     7728 2023-05-05 16:05:36.301412 pyfcst-0.0.9/pyfcst/ips/inout/__pycache__/input.cpython-38.pyc
+-rw-r--r--   0        0        0     4372 2023-05-05 16:05:36.525416 pyfcst-0.0.9/pyfcst/ips/inout/__pycache__/output.cpython-38.pyc
+-rw-r--r--   0        0        0     1395 2023-05-05 16:05:36.525416 pyfcst-0.0.9/pyfcst/ips/inout/__pycache__/printlog.cpython-38.pyc
+-rw-r--r--   0        0        0    11433 2023-02-22 23:48:52.000000 pyfcst-0.0.9/pyfcst/ips/inout/input.py
+-rw-r--r--   0        0        0     4483 2023-02-22 23:48:52.000000 pyfcst-0.0.9/pyfcst/ips/inout/output.py
+-rw-r--r--   0        0        0      875 2023-02-22 23:48:52.000000 pyfcst-0.0.9/pyfcst/ips/inout/printlog.py
+-rw-r--r--   0        0        0       29 2023-05-05 03:26:52.003756 pyfcst-0.0.9/pyfcst/util/__init__.py
+-rw-r--r--   0        0        0     4091 2023-05-04 21:09:44.163901 pyfcst-0.0.9/pyfcst/util/baseclass.py
+-rw-r--r--   0        0        0      728 2023-05-05 17:24:35.765863 pyfcst-0.0.9/pyproject.toml
+-rw-r--r--   0        0        0      987 1970-01-01 00:00:00.000000 pyfcst-0.0.9/PKG-INFO
```

### Comparing `pyfcst-0.0.8/LICENSE.txt` & `pyfcst-0.0.9/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pyfcst-0.0.8/pyfcst/ips/analysis/__pycache__/distanceSD.cpython-38.pyc` & `pyfcst-0.0.9/pyfcst/ips/analysis/__pycache__/distanceSD.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `pyfcst-0.0.8/pyfcst/ips/analysis/distanceSD.py` & `pyfcst-0.0.9/pyfcst/ips/analysis/distanceSD.py`

 * *Files identical despite different names*

### Comparing `pyfcst-0.0.8/pyfcst/ips/inout/__pycache__/input.cpython-38.pyc` & `pyfcst-0.0.9/pyfcst/ips/inout/__pycache__/input.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `pyfcst-0.0.8/pyfcst/ips/inout/__pycache__/output.cpython-38.pyc` & `pyfcst-0.0.9/pyfcst/ips/inout/__pycache__/output.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `pyfcst-0.0.8/pyfcst/ips/inout/__pycache__/printlog.cpython-38.pyc` & `pyfcst-0.0.9/pyfcst/ips/inout/__pycache__/printlog.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `pyfcst-0.0.8/pyfcst/ips/inout/input.py` & `pyfcst-0.0.9/pyfcst/ips/inout/input.py`

 * *Files identical despite different names*

### Comparing `pyfcst-0.0.8/pyfcst/ips/inout/output.py` & `pyfcst-0.0.9/pyfcst/ips/inout/output.py`

 * *Files identical despite different names*

### Comparing `pyfcst-0.0.8/pyfcst/ips/inout/printlog.py` & `pyfcst-0.0.9/pyfcst/ips/inout/printlog.py`

 * *Files identical despite different names*

### Comparing `pyfcst-0.0.8/pyfcst/util/baseclass.py` & `pyfcst-0.0.9/pyfcst/util/baseclass.py`

 * *Files identical despite different names*

### Comparing `pyfcst-0.0.8/pyproject.toml` & `pyfcst-0.0.9/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 [tool.poetry]
 name = "pyfcst"
-version = "0.0.8"
+version = "0.0.9"
 description = "python library developed for use with OpenFCST"
 authors = ["james <jwoodfor@ualberta.ca>", "FCST Dev Group"]
 readme = "README.md"
 packages = [{include = "pyfcst"},
             {include = "pyfcst/ips/"},
             {include = "pyfcst/util/"}]
 
 
 
 [tool.poetry.dependencies]
-python = "^3.7"
+python = "~3.8"
 scipy = "1.10.1"
 numpy = "^1.24.1"
 bitarray = "~2.7.3"
 vtk = "~8.1.2"
 mayavi = "~4.7.1"
 mahotas = "1.4.13"
 pillow = "~9.3.0"
```

### Comparing `pyfcst-0.0.8/PKG-INFO` & `pyfcst-0.0.9/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,20 +1,16 @@
 Metadata-Version: 2.1
 Name: pyfcst
-Version: 0.0.8
+Version: 0.0.9
 Summary: python library developed for use with OpenFCST
 Author: james
 Author-email: jwoodfor@ualberta.ca
-Requires-Python: >=3.7,<4.0
+Requires-Python: >=3.8,<3.9
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
-Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: bitarray (>=2.7.3,<2.8.0)
 Requires-Dist: jedi (>=0.17.1,<0.18.0)
 Requires-Dist: mahotas (==1.4.13)
 Requires-Dist: mayavi (>=4.7.1,<4.8.0)
 Requires-Dist: numpy (>=1.24.1,<2.0.0)
 Requires-Dist: opencv-python (>=4.7.0.72,<4.8.0.0)
 Requires-Dist: parso (>=0.7.0,<0.8.0)
```

