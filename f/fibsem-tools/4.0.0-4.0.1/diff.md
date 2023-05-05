# Comparing `tmp/fibsem_tools-4.0.0.tar.gz` & `tmp/fibsem_tools-4.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fibsem_tools-4.0.0.tar", max compression
+gzip compressed data, was "fibsem_tools-4.0.1.tar", max compression
```

## Comparing `fibsem_tools-4.0.0.tar` & `fibsem_tools-4.0.1.tar`

### file list

```diff
@@ -1,25 +1,25 @@
--rw-r--r--   0        0        0     1072 2023-02-21 23:22:56.299056 fibsem_tools-4.0.0/LICENSE
--rw-r--r--   0        0        0     1425 2023-05-04 18:41:40.840291 fibsem_tools-4.0.0/pyproject.toml
--rw-r--r--   0        0        0      183 2023-04-25 22:22:07.080776 fibsem_tools-4.0.0/src/fibsem_tools/__init__.py
--rw-r--r--   0        0        0      606 2023-04-02 16:17:29.203986 fibsem_tools-4.0.0/src/fibsem_tools/cli/tiff2zarr.css
--rw-r--r--   0        0        0    13481 2023-04-02 16:17:29.204298 fibsem_tools-4.0.0/src/fibsem_tools/cli/tiff2zarr.py
--rw-r--r--   0        0        0        0 2023-03-23 18:13:14.517927 fibsem_tools-4.0.0/src/fibsem_tools/io/__init__.py
--rw-r--r--   0        0        0     7427 2023-05-04 18:29:01.062775 fibsem_tools-4.0.0/src/fibsem_tools/io/core.py
--rw-r--r--   0        0        0    13817 2023-05-04 17:46:58.084105 fibsem_tools-4.0.0/src/fibsem_tools/io/dask.py
--rw-r--r--   0        0        0    31797 2023-05-04 18:29:01.063113 fibsem_tools-4.0.0/src/fibsem_tools/io/dat.py
--rw-r--r--   0        0        0     2258 2023-03-23 19:35:10.739676 fibsem_tools-4.0.0/src/fibsem_tools/io/h5.py
--rw-r--r--   0        0        0     5081 2023-05-04 18:29:01.063414 fibsem_tools-4.0.0/src/fibsem_tools/io/mrc.py
--rw-r--r--   0        0        0     6819 2023-05-04 18:29:01.063658 fibsem_tools-4.0.0/src/fibsem_tools/io/multiscale.py
--rw-r--r--   0        0        0       36 2023-03-23 19:35:10.687732 fibsem_tools-4.0.0/src/fibsem_tools/io/neuroglancer.py
--rw-r--r--   0        0        0     2341 2023-03-23 19:45:26.756642 fibsem_tools-4.0.0/src/fibsem_tools/io/server.py
--rw-r--r--   0        0        0      431 2023-05-04 18:29:01.063967 fibsem_tools-4.0.0/src/fibsem_tools/io/tif.py
--rw-r--r--   0        0        0     4340 2023-05-04 18:29:01.064387 fibsem_tools-4.0.0/src/fibsem_tools/io/util.py
--rw-r--r--   0        0        0     1504 2023-05-04 18:29:01.064928 fibsem_tools-4.0.0/src/fibsem_tools/io/xr.py
--rw-r--r--   0        0        0    15179 2023-05-04 18:29:01.065422 fibsem_tools-4.0.0/src/fibsem_tools/io/zarr.py
--rw-r--r--   0        0        0        0 2023-02-21 23:22:56.301100 fibsem_tools-4.0.0/src/fibsem_tools/metadata/__init__.py
--rw-r--r--   0        0        0     3195 2023-05-04 17:46:58.085649 fibsem_tools-4.0.0/src/fibsem_tools/metadata/cosem.py
--rw-r--r--   0        0        0     3479 2023-05-04 17:46:58.086178 fibsem_tools-4.0.0/src/fibsem_tools/metadata/groundtruth.py
--rw-r--r--   0        0        0     2123 2023-03-16 20:03:20.243743 fibsem_tools-4.0.0/src/fibsem_tools/metadata/neuroglancer.py
--rw-r--r--   0        0        0     3371 2023-05-04 18:29:01.065840 fibsem_tools-4.0.0/src/fibsem_tools/metadata/transform.py
--rw-r--r--   0        0        0        0 2023-03-23 17:36:07.629685 fibsem_tools-4.0.0/src/fibsem_tools/py.typed
--rw-r--r--   0        0        0     1337 1970-01-01 00:00:00.000000 fibsem_tools-4.0.0/PKG-INFO
+-rw-r--r--   0        0        0     1072 2023-02-21 23:22:56.299056 fibsem_tools-4.0.1/LICENSE
+-rw-r--r--   0        0        0     1425 2023-05-05 13:40:31.013597 fibsem_tools-4.0.1/pyproject.toml
+-rw-r--r--   0        0        0      183 2023-04-25 22:22:07.080776 fibsem_tools-4.0.1/src/fibsem_tools/__init__.py
+-rw-r--r--   0        0        0      606 2023-04-02 16:17:29.203986 fibsem_tools-4.0.1/src/fibsem_tools/cli/tiff2zarr.css
+-rw-r--r--   0        0        0    13481 2023-04-02 16:17:29.204298 fibsem_tools-4.0.1/src/fibsem_tools/cli/tiff2zarr.py
+-rw-r--r--   0        0        0        0 2023-03-23 18:13:14.517927 fibsem_tools-4.0.1/src/fibsem_tools/io/__init__.py
+-rw-r--r--   0        0        0     7453 2023-05-05 13:40:11.564507 fibsem_tools-4.0.1/src/fibsem_tools/io/core.py
+-rw-r--r--   0        0        0    13817 2023-05-04 17:46:58.084105 fibsem_tools-4.0.1/src/fibsem_tools/io/dask.py
+-rw-r--r--   0        0        0    31797 2023-05-04 18:29:01.063113 fibsem_tools-4.0.1/src/fibsem_tools/io/dat.py
+-rw-r--r--   0        0        0     2258 2023-03-23 19:35:10.739676 fibsem_tools-4.0.1/src/fibsem_tools/io/h5.py
+-rw-r--r--   0        0        0     5081 2023-05-04 18:29:01.063414 fibsem_tools-4.0.1/src/fibsem_tools/io/mrc.py
+-rw-r--r--   0        0        0     6819 2023-05-04 18:29:01.063658 fibsem_tools-4.0.1/src/fibsem_tools/io/multiscale.py
+-rw-r--r--   0        0        0       36 2023-03-23 19:35:10.687732 fibsem_tools-4.0.1/src/fibsem_tools/io/neuroglancer.py
+-rw-r--r--   0        0        0     2341 2023-03-23 19:45:26.756642 fibsem_tools-4.0.1/src/fibsem_tools/io/server.py
+-rw-r--r--   0        0        0      431 2023-05-04 18:29:01.063967 fibsem_tools-4.0.1/src/fibsem_tools/io/tif.py
+-rw-r--r--   0        0        0     4340 2023-05-04 18:29:01.064387 fibsem_tools-4.0.1/src/fibsem_tools/io/util.py
+-rw-r--r--   0        0        0     1504 2023-05-04 18:29:01.064928 fibsem_tools-4.0.1/src/fibsem_tools/io/xr.py
+-rw-r--r--   0        0        0    15179 2023-05-04 18:29:01.065422 fibsem_tools-4.0.1/src/fibsem_tools/io/zarr.py
+-rw-r--r--   0        0        0        0 2023-02-21 23:22:56.301100 fibsem_tools-4.0.1/src/fibsem_tools/metadata/__init__.py
+-rw-r--r--   0        0        0     3195 2023-05-04 17:46:58.085649 fibsem_tools-4.0.1/src/fibsem_tools/metadata/cosem.py
+-rw-r--r--   0        0        0     3479 2023-05-04 17:46:58.086178 fibsem_tools-4.0.1/src/fibsem_tools/metadata/groundtruth.py
+-rw-r--r--   0        0        0     2123 2023-03-16 20:03:20.243743 fibsem_tools-4.0.1/src/fibsem_tools/metadata/neuroglancer.py
+-rw-r--r--   0        0        0     3371 2023-05-04 18:29:01.065840 fibsem_tools-4.0.1/src/fibsem_tools/metadata/transform.py
+-rw-r--r--   0        0        0        0 2023-03-23 17:36:07.629685 fibsem_tools-4.0.1/src/fibsem_tools/py.typed
+-rw-r--r--   0        0        0     1337 1970-01-01 00:00:00.000000 fibsem_tools-4.0.1/PKG-INFO
```

### Comparing `fibsem_tools-4.0.0/LICENSE` & `fibsem_tools-4.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `fibsem_tools-4.0.0/pyproject.toml` & `fibsem_tools-4.0.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "fibsem-tools"
-version = "4.0.0"
+version = "4.0.1"
 description = "Tools for processing FIBSEM datasets"
 authors = ["Davis Vann Bennett <davis.v.bennett@gmail.com>"]
 license = "MIT"
 
 [tool.poetry.dependencies]
 python = "^3.9"
 distributed = ">=2021.10.0"
```

### Comparing `fibsem_tools-4.0.0/src/fibsem_tools/cli/tiff2zarr.css` & `fibsem_tools-4.0.1/src/fibsem_tools/cli/tiff2zarr.css`

 * *Files identical despite different names*

### Comparing `fibsem_tools-4.0.0/src/fibsem_tools/cli/tiff2zarr.py` & `fibsem_tools-4.0.1/src/fibsem_tools/cli/tiff2zarr.py`

 * *Files identical despite different names*

### Comparing `fibsem_tools-4.0.0/src/fibsem_tools/io/core.py` & `fibsem_tools-4.0.1/src/fibsem_tools/io/core.py`

 * *Files 0% similar despite different names*

```diff
@@ -27,15 +27,15 @@
 )
 
 import fibsem_tools.io.mrc
 import fibsem_tools.io.dat
 import fibsem_tools.io.xr
 import fibsem_tools.io.h5
 import fibsem_tools.io.zarr
-
+import fibsem_tools.io.tif
 
 _formats = (".dat", ".mrc", ".tif")
 _container_extensions = (".zarr", ".n5", ".h5")
 _suffixes = (*_formats, *_container_extensions)
 
 
 def access(
```

### Comparing `fibsem_tools-4.0.0/src/fibsem_tools/io/dask.py` & `fibsem_tools-4.0.1/src/fibsem_tools/io/dask.py`

 * *Files identical despite different names*

### Comparing `fibsem_tools-4.0.0/src/fibsem_tools/io/dat.py` & `fibsem_tools-4.0.1/src/fibsem_tools/io/dat.py`

 * *Files identical despite different names*

### Comparing `fibsem_tools-4.0.0/src/fibsem_tools/io/h5.py` & `fibsem_tools-4.0.1/src/fibsem_tools/io/h5.py`

 * *Files identical despite different names*

### Comparing `fibsem_tools-4.0.0/src/fibsem_tools/io/mrc.py` & `fibsem_tools-4.0.1/src/fibsem_tools/io/mrc.py`

 * *Files identical despite different names*

### Comparing `fibsem_tools-4.0.0/src/fibsem_tools/io/multiscale.py` & `fibsem_tools-4.0.1/src/fibsem_tools/io/multiscale.py`

 * *Files identical despite different names*

### Comparing `fibsem_tools-4.0.0/src/fibsem_tools/io/server.py` & `fibsem_tools-4.0.1/src/fibsem_tools/io/server.py`

 * *Files identical despite different names*

### Comparing `fibsem_tools-4.0.0/src/fibsem_tools/io/util.py` & `fibsem_tools-4.0.1/src/fibsem_tools/io/util.py`

 * *Files identical despite different names*

### Comparing `fibsem_tools-4.0.0/src/fibsem_tools/io/xr.py` & `fibsem_tools-4.0.1/src/fibsem_tools/io/xr.py`

 * *Files identical despite different names*

### Comparing `fibsem_tools-4.0.0/src/fibsem_tools/io/zarr.py` & `fibsem_tools-4.0.1/src/fibsem_tools/io/zarr.py`

 * *Files identical despite different names*

### Comparing `fibsem_tools-4.0.0/src/fibsem_tools/metadata/cosem.py` & `fibsem_tools-4.0.1/src/fibsem_tools/metadata/cosem.py`

 * *Files identical despite different names*

### Comparing `fibsem_tools-4.0.0/src/fibsem_tools/metadata/groundtruth.py` & `fibsem_tools-4.0.1/src/fibsem_tools/metadata/groundtruth.py`

 * *Files identical despite different names*

### Comparing `fibsem_tools-4.0.0/src/fibsem_tools/metadata/neuroglancer.py` & `fibsem_tools-4.0.1/src/fibsem_tools/metadata/neuroglancer.py`

 * *Files identical despite different names*

### Comparing `fibsem_tools-4.0.0/src/fibsem_tools/metadata/transform.py` & `fibsem_tools-4.0.1/src/fibsem_tools/metadata/transform.py`

 * *Files identical despite different names*

### Comparing `fibsem_tools-4.0.0/PKG-INFO` & `fibsem_tools-4.0.1/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fibsem-tools
-Version: 4.0.0
+Version: 4.0.1
 Summary: Tools for processing FIBSEM datasets
 License: MIT
 Author: Davis Vann Bennett
 Author-email: davis.v.bennett@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

