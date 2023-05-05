# Comparing `tmp/pyfcst-0.0.13.tar.gz` & `tmp/pyfcst-0.0.14.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyfcst-0.0.13.tar", max compression
+gzip compressed data, was "pyfcst-0.0.14.tar", max compression
```

## Comparing `pyfcst-0.0.13.tar` & `pyfcst-0.0.14.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0     1078 2023-05-04 22:17:13.930214 pyfcst-0.0.13/LICENSE.txt
--rw-r--r--   0        0        0       68 2023-05-04 21:44:54.560223 pyfcst-0.0.13/README.md
--rw-r--r--   0        0        0       46 2023-05-05 16:42:50.512291 pyfcst-0.0.13/pyfcst/__init__.py
--rw-r--r--   0        0        0       52 2023-05-05 16:04:26.568156 pyfcst-0.0.13/pyfcst/ips/__init__.py
--rw-r--r--   0        0        0       33 2023-05-05 16:04:39.580397 pyfcst-0.0.13/pyfcst/ips/analysis/__init__.py
--rw-r--r--   0        0        0      173 2023-05-05 16:05:36.525416 pyfcst-0.0.13/pyfcst/ips/analysis/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0        0        0     5571 2023-05-05 16:05:36.525416 pyfcst-0.0.13/pyfcst/ips/analysis/__pycache__/distanceSD.cpython-38.pyc
--rw-r--r--   0        0        0     6166 2023-05-05 03:25:13.456073 pyfcst-0.0.13/pyfcst/ips/analysis/distanceSD.py
--rw-r--r--   0        0        0       67 2023-05-05 16:05:26.981249 pyfcst-0.0.13/pyfcst/ips/inout/__init__.py
--rw-r--r--   0        0        0      203 2023-05-05 16:05:36.301412 pyfcst-0.0.13/pyfcst/ips/inout/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0        0        0     7728 2023-05-05 16:05:36.301412 pyfcst-0.0.13/pyfcst/ips/inout/__pycache__/input.cpython-38.pyc
--rw-r--r--   0        0        0     4372 2023-05-05 16:05:36.525416 pyfcst-0.0.13/pyfcst/ips/inout/__pycache__/output.cpython-38.pyc
--rw-r--r--   0        0        0     1395 2023-05-05 16:05:36.525416 pyfcst-0.0.13/pyfcst/ips/inout/__pycache__/printlog.cpython-38.pyc
--rw-r--r--   0        0        0    11433 2023-02-22 23:48:52.000000 pyfcst-0.0.13/pyfcst/ips/inout/input.py
--rw-r--r--   0        0        0     4483 2023-02-22 23:48:52.000000 pyfcst-0.0.13/pyfcst/ips/inout/output.py
--rw-r--r--   0        0        0      875 2023-02-22 23:48:52.000000 pyfcst-0.0.13/pyfcst/ips/inout/printlog.py
--rw-r--r--   0        0        0       29 2023-05-05 03:26:52.003756 pyfcst-0.0.13/pyfcst/util/__init__.py
--rw-r--r--   0        0        0     4091 2023-05-04 21:09:44.163901 pyfcst-0.0.13/pyfcst/util/baseclass.py
--rw-r--r--   0        0        0      747 2023-05-05 17:36:23.035256 pyfcst-0.0.13/pyproject.toml
--rw-r--r--   0        0        0     1023 1970-01-01 00:00:00.000000 pyfcst-0.0.13/PKG-INFO
+-rw-r--r--   0        0        0     1078 2023-05-04 22:17:13.930214 pyfcst-0.0.14/LICENSE.txt
+-rw-r--r--   0        0        0       68 2023-05-04 21:44:54.560223 pyfcst-0.0.14/README.md
+-rw-r--r--   0        0        0       46 2023-05-05 16:42:50.512291 pyfcst-0.0.14/pyfcst/__init__.py
+-rw-r--r--   0        0        0       52 2023-05-05 16:04:26.568156 pyfcst-0.0.14/pyfcst/ips/__init__.py
+-rw-r--r--   0        0        0       33 2023-05-05 16:04:39.580397 pyfcst-0.0.14/pyfcst/ips/analysis/__init__.py
+-rw-r--r--   0        0        0      173 2023-05-05 16:05:36.525416 pyfcst-0.0.14/pyfcst/ips/analysis/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0        0        0     5571 2023-05-05 16:05:36.525416 pyfcst-0.0.14/pyfcst/ips/analysis/__pycache__/distanceSD.cpython-38.pyc
+-rw-r--r--   0        0        0     6166 2023-05-05 03:25:13.456073 pyfcst-0.0.14/pyfcst/ips/analysis/distanceSD.py
+-rw-r--r--   0        0        0       67 2023-05-05 16:05:26.981249 pyfcst-0.0.14/pyfcst/ips/inout/__init__.py
+-rw-r--r--   0        0        0      203 2023-05-05 16:05:36.301412 pyfcst-0.0.14/pyfcst/ips/inout/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0        0        0     7728 2023-05-05 16:05:36.301412 pyfcst-0.0.14/pyfcst/ips/inout/__pycache__/input.cpython-38.pyc
+-rw-r--r--   0        0        0     4372 2023-05-05 16:05:36.525416 pyfcst-0.0.14/pyfcst/ips/inout/__pycache__/output.cpython-38.pyc
+-rw-r--r--   0        0        0     1395 2023-05-05 16:05:36.525416 pyfcst-0.0.14/pyfcst/ips/inout/__pycache__/printlog.cpython-38.pyc
+-rw-r--r--   0        0        0    11433 2023-02-22 23:48:52.000000 pyfcst-0.0.14/pyfcst/ips/inout/input.py
+-rw-r--r--   0        0        0     4483 2023-02-22 23:48:52.000000 pyfcst-0.0.14/pyfcst/ips/inout/output.py
+-rw-r--r--   0        0        0      875 2023-02-22 23:48:52.000000 pyfcst-0.0.14/pyfcst/ips/inout/printlog.py
+-rw-r--r--   0        0        0       29 2023-05-05 03:26:52.003756 pyfcst-0.0.14/pyfcst/util/__init__.py
+-rw-r--r--   0        0        0     4091 2023-05-04 21:09:44.163901 pyfcst-0.0.14/pyfcst/util/baseclass.py
+-rw-r--r--   0        0        0      747 2023-05-05 17:38:52.149312 pyfcst-0.0.14/pyproject.toml
+-rw-r--r--   0        0        0     1023 1970-01-01 00:00:00.000000 pyfcst-0.0.14/PKG-INFO
```

### Comparing `pyfcst-0.0.13/LICENSE.txt` & `pyfcst-0.0.14/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pyfcst-0.0.13/pyfcst/ips/analysis/__pycache__/distanceSD.cpython-38.pyc` & `pyfcst-0.0.14/pyfcst/ips/analysis/__pycache__/distanceSD.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `pyfcst-0.0.13/pyfcst/ips/analysis/distanceSD.py` & `pyfcst-0.0.14/pyfcst/ips/analysis/distanceSD.py`

 * *Files identical despite different names*

### Comparing `pyfcst-0.0.13/pyfcst/ips/inout/__pycache__/input.cpython-38.pyc` & `pyfcst-0.0.14/pyfcst/ips/inout/__pycache__/input.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `pyfcst-0.0.13/pyfcst/ips/inout/__pycache__/output.cpython-38.pyc` & `pyfcst-0.0.14/pyfcst/ips/inout/__pycache__/output.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `pyfcst-0.0.13/pyfcst/ips/inout/__pycache__/printlog.cpython-38.pyc` & `pyfcst-0.0.14/pyfcst/ips/inout/__pycache__/printlog.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `pyfcst-0.0.13/pyfcst/ips/inout/input.py` & `pyfcst-0.0.14/pyfcst/ips/inout/input.py`

 * *Files identical despite different names*

### Comparing `pyfcst-0.0.13/pyfcst/ips/inout/output.py` & `pyfcst-0.0.14/pyfcst/ips/inout/output.py`

 * *Files identical despite different names*

### Comparing `pyfcst-0.0.13/pyfcst/ips/inout/printlog.py` & `pyfcst-0.0.14/pyfcst/ips/inout/printlog.py`

 * *Files identical despite different names*

### Comparing `pyfcst-0.0.13/pyfcst/util/baseclass.py` & `pyfcst-0.0.14/pyfcst/util/baseclass.py`

 * *Files identical despite different names*

### Comparing `pyfcst-0.0.13/pyproject.toml` & `pyfcst-0.0.14/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pyfcst"
-version = "0.0.13"
+version = "0.0.14"
 description = "python library developed for use with OpenFCST"
 authors = ["james <jwoodfor@ualberta.ca>", "FCST Dev Group"]
 readme = "README.md"
 packages = [{include = "pyfcst"},
             {include = "pyfcst/ips/"},
             {include = "pyfcst/util/"}]
 
@@ -23,12 +23,12 @@
 simpleitk = "~2.0.2"
 sphinx = "~5.0.2"
 opencv-python = "~4.7.0.72"
 jedi = "~0.17.1"
 pyqt5 = "~5.13"
 pyqtwebengine = "~5.13"
 parso = "~0.7.0"
-libtiff = "^4.1.0"
+libtiff = "^0.4.0"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `pyfcst-0.0.13/PKG-INFO` & `pyfcst-0.0.14/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: pyfcst
-Version: 0.0.13
+Version: 0.0.14
 Summary: python library developed for use with OpenFCST
 Author: james
 Author-email: jwoodfor@ualberta.ca
 Requires-Python: >=3.8,<3.9
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Requires-Dist: bitarray (>=2.7.3,<2.8.0)
 Requires-Dist: jedi (>=0.17.1,<0.18.0)
-Requires-Dist: libtiff (>=4.1.0,<5.0.0)
+Requires-Dist: libtiff (>=0.4.0,<0.5.0)
 Requires-Dist: mahotas (==1.4.13)
 Requires-Dist: mayavi (==4.8.1)
 Requires-Dist: numpy (>=1.24.1,<1.25.0)
 Requires-Dist: opencv-python (>=4.7.0.72,<4.8.0.0)
 Requires-Dist: parso (>=0.7.0,<0.8.0)
 Requires-Dist: pillow (>=9.3.0,<9.4.0)
 Requires-Dist: pyqt5 (>=5.13,<5.14)
```

