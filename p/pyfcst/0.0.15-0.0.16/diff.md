# Comparing `tmp/pyfcst-0.0.15.tar.gz` & `tmp/pyfcst-0.0.16.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyfcst-0.0.15.tar", max compression
+gzip compressed data, was "pyfcst-0.0.16.tar", max compression
```

## Comparing `pyfcst-0.0.15.tar` & `pyfcst-0.0.16.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0     1078 2023-05-04 22:17:13.930214 pyfcst-0.0.15/LICENSE.txt
--rw-r--r--   0        0        0       68 2023-05-04 21:44:54.560223 pyfcst-0.0.15/README.md
--rw-r--r--   0        0        0       46 2023-05-05 16:42:50.512291 pyfcst-0.0.15/pyfcst/__init__.py
--rw-r--r--   0        0        0       52 2023-05-05 16:04:26.568156 pyfcst-0.0.15/pyfcst/ips/__init__.py
--rw-r--r--   0        0        0       33 2023-05-05 16:04:39.580397 pyfcst-0.0.15/pyfcst/ips/analysis/__init__.py
--rw-r--r--   0        0        0      173 2023-05-05 16:05:36.525416 pyfcst-0.0.15/pyfcst/ips/analysis/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0        0        0     5571 2023-05-05 16:05:36.525416 pyfcst-0.0.15/pyfcst/ips/analysis/__pycache__/distanceSD.cpython-38.pyc
--rw-r--r--   0        0        0     6166 2023-05-05 03:25:13.456073 pyfcst-0.0.15/pyfcst/ips/analysis/distanceSD.py
--rw-r--r--   0        0        0       67 2023-05-05 16:05:26.981249 pyfcst-0.0.15/pyfcst/ips/inout/__init__.py
--rw-r--r--   0        0        0      203 2023-05-05 16:05:36.301412 pyfcst-0.0.15/pyfcst/ips/inout/__pycache__/__init__.cpython-38.pyc
--rw-r--r--   0        0        0     7728 2023-05-05 16:05:36.301412 pyfcst-0.0.15/pyfcst/ips/inout/__pycache__/input.cpython-38.pyc
--rw-r--r--   0        0        0     4372 2023-05-05 16:05:36.525416 pyfcst-0.0.15/pyfcst/ips/inout/__pycache__/output.cpython-38.pyc
--rw-r--r--   0        0        0     1395 2023-05-05 16:05:36.525416 pyfcst-0.0.15/pyfcst/ips/inout/__pycache__/printlog.cpython-38.pyc
--rw-r--r--   0        0        0    11433 2023-02-22 23:48:52.000000 pyfcst-0.0.15/pyfcst/ips/inout/input.py
--rw-r--r--   0        0        0     4483 2023-02-22 23:48:52.000000 pyfcst-0.0.15/pyfcst/ips/inout/output.py
--rw-r--r--   0        0        0      875 2023-02-22 23:48:52.000000 pyfcst-0.0.15/pyfcst/ips/inout/printlog.py
--rw-r--r--   0        0        0       29 2023-05-05 03:26:52.003756 pyfcst-0.0.15/pyfcst/util/__init__.py
--rw-r--r--   0        0        0     4091 2023-05-04 21:09:44.163901 pyfcst-0.0.15/pyfcst/util/baseclass.py
--rw-r--r--   0        0        0      763 2023-05-05 17:45:57.521804 pyfcst-0.0.15/pyproject.toml
--rw-r--r--   0        0        0     1023 1970-01-01 00:00:00.000000 pyfcst-0.0.15/PKG-INFO
+-rw-r--r--   0        0        0     1078 2023-05-04 22:17:13.930214 pyfcst-0.0.16/LICENSE.txt
+-rw-r--r--   0        0        0       68 2023-05-04 21:44:54.560223 pyfcst-0.0.16/README.md
+-rw-r--r--   0        0        0       46 2023-05-05 16:42:50.512291 pyfcst-0.0.16/pyfcst/__init__.py
+-rw-r--r--   0        0        0       52 2023-05-05 16:04:26.568156 pyfcst-0.0.16/pyfcst/ips/__init__.py
+-rw-r--r--   0        0        0       33 2023-05-05 16:04:39.580397 pyfcst-0.0.16/pyfcst/ips/analysis/__init__.py
+-rw-r--r--   0        0        0      173 2023-05-05 16:05:36.525416 pyfcst-0.0.16/pyfcst/ips/analysis/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0        0        0     5571 2023-05-05 16:05:36.525416 pyfcst-0.0.16/pyfcst/ips/analysis/__pycache__/distanceSD.cpython-38.pyc
+-rw-r--r--   0        0        0     6137 2023-05-05 17:52:16.247948 pyfcst-0.0.16/pyfcst/ips/analysis/distanceSD.py
+-rw-r--r--   0        0        0       67 2023-05-05 16:05:26.981249 pyfcst-0.0.16/pyfcst/ips/inout/__init__.py
+-rw-r--r--   0        0        0      203 2023-05-05 16:05:36.301412 pyfcst-0.0.16/pyfcst/ips/inout/__pycache__/__init__.cpython-38.pyc
+-rw-r--r--   0        0        0     7728 2023-05-05 16:05:36.301412 pyfcst-0.0.16/pyfcst/ips/inout/__pycache__/input.cpython-38.pyc
+-rw-r--r--   0        0        0     4372 2023-05-05 16:05:36.525416 pyfcst-0.0.16/pyfcst/ips/inout/__pycache__/output.cpython-38.pyc
+-rw-r--r--   0        0        0     1395 2023-05-05 16:05:36.525416 pyfcst-0.0.16/pyfcst/ips/inout/__pycache__/printlog.cpython-38.pyc
+-rw-r--r--   0        0        0    11433 2023-02-22 23:48:52.000000 pyfcst-0.0.16/pyfcst/ips/inout/input.py
+-rw-r--r--   0        0        0     4483 2023-02-22 23:48:52.000000 pyfcst-0.0.16/pyfcst/ips/inout/output.py
+-rw-r--r--   0        0        0      875 2023-02-22 23:48:52.000000 pyfcst-0.0.16/pyfcst/ips/inout/printlog.py
+-rw-r--r--   0        0        0       29 2023-05-05 03:26:52.003756 pyfcst-0.0.16/pyfcst/util/__init__.py
+-rw-r--r--   0        0        0     4091 2023-05-04 21:09:44.163901 pyfcst-0.0.16/pyfcst/util/baseclass.py
+-rw-r--r--   0        0        0      763 2023-05-05 17:52:22.516179 pyfcst-0.0.16/pyproject.toml
+-rw-r--r--   0        0        0     1023 1970-01-01 00:00:00.000000 pyfcst-0.0.16/PKG-INFO
```

### Comparing `pyfcst-0.0.15/LICENSE.txt` & `pyfcst-0.0.16/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pyfcst-0.0.15/pyfcst/ips/analysis/__pycache__/distanceSD.cpython-38.pyc` & `pyfcst-0.0.16/pyfcst/ips/analysis/__pycache__/distanceSD.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `pyfcst-0.0.15/pyfcst/ips/analysis/distanceSD.py` & `pyfcst-0.0.16/pyfcst/ips/analysis/distanceSD.py`

 * *Files 2% similar despite different names*

```diff
@@ -47,15 +47,14 @@
         self._label=label
 
         self._spacing=voxelsize
 
         self._imSolidPore = 0
         self.imDistanceTransform = 0
         self.imPSD = 0
-        self._indent=indent
         im = np.asarray(image)
         self._format_color = cycle(['b','g','m','r','y','o'])
         self.scale=np.shape(im)[0]*np.shape(im)[1]
         self._rangeX=scipy.linspace(0,im.shape[0]*voxelsize[0],im.shape[0],endpoint=False)
         self._rangeY=scipy.linspace(0,im.shape[1]*voxelsize[1],im.shape[1],endpoint=False)
         self._rangeZ=scipy.linspace(0,im.shape[2]*voxelsize[2],im.shape[2],endpoint=False)
         self._voxelunit=voxelunit
```

### Comparing `pyfcst-0.0.15/pyfcst/ips/inout/__pycache__/input.cpython-38.pyc` & `pyfcst-0.0.16/pyfcst/ips/inout/__pycache__/input.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `pyfcst-0.0.15/pyfcst/ips/inout/__pycache__/output.cpython-38.pyc` & `pyfcst-0.0.16/pyfcst/ips/inout/__pycache__/output.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `pyfcst-0.0.15/pyfcst/ips/inout/__pycache__/printlog.cpython-38.pyc` & `pyfcst-0.0.16/pyfcst/ips/inout/__pycache__/printlog.cpython-38.pyc`

 * *Files identical despite different names*

### Comparing `pyfcst-0.0.15/pyfcst/ips/inout/input.py` & `pyfcst-0.0.16/pyfcst/ips/inout/input.py`

 * *Files identical despite different names*

### Comparing `pyfcst-0.0.15/pyfcst/ips/inout/output.py` & `pyfcst-0.0.16/pyfcst/ips/inout/output.py`

 * *Files identical despite different names*

### Comparing `pyfcst-0.0.15/pyfcst/ips/inout/printlog.py` & `pyfcst-0.0.16/pyfcst/ips/inout/printlog.py`

 * *Files identical despite different names*

### Comparing `pyfcst-0.0.15/pyfcst/util/baseclass.py` & `pyfcst-0.0.16/pyfcst/util/baseclass.py`

 * *Files identical despite different names*

### Comparing `pyfcst-0.0.15/pyproject.toml` & `pyfcst-0.0.16/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "pyfcst"
-version = "0.0.15"
+version = "0.0.16"
 description = "python library developed for use with OpenFCST"
 authors = ["james <jwoodfor@ualberta.ca>", "FCST Dev Group"]
 readme = "README.md"
 packages = [{include = "pyfcst"},
             {include = "pyfcst/ips/"},
             {include = "pyfcst/util/"}]
```

### Comparing `pyfcst-0.0.15/PKG-INFO` & `pyfcst-0.0.16/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyfcst
-Version: 0.0.15
+Version: 0.0.16
 Summary: python library developed for use with OpenFCST
 Author: james
 Author-email: jwoodfor@ualberta.ca
 Requires-Python: >=3.8,<3.9
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Requires-Dist: bitarray (>=2.7.3,<2.8.0)
```

