# Comparing `tmp/geocat.comp-2023.3.2.tar.gz` & `tmp/geocat.comp-2023.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "geocat.comp-2023.3.2.tar", last modified: Sat Apr  1 01:54:11 2023, max compression
+gzip compressed data, was "geocat.comp-2023.5.0.tar", last modified: Fri May  5 15:41:27 2023, max compression
```

## Comparing `geocat.comp-2023.3.2.tar` & `geocat.comp-2023.5.0.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-01 01:54:11.033527 geocat.comp-2023.3.2/
--rw-r--r--   0 runner    (1001) docker     (123)     5888 2023-04-01 01:53:43.000000 geocat.comp-2023.3.2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      998 2023-04-01 01:53:43.000000 geocat.comp-2023.3.2/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      476 2023-04-01 01:53:43.000000 geocat.comp-2023.3.2/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (123)      286 2023-04-01 01:53:43.000000 geocat.comp-2023.3.2/CITATION.cff
--rw-r--r--   0 runner    (1001) docker     (123)     4030 2023-04-01 01:53:43.000000 geocat.comp-2023.3.2/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)      175 2023-04-01 01:53:43.000000 geocat.comp-2023.3.2/INSTALLATION.md
--rw-r--r--   0 runner    (1001) docker     (123)    11377 2023-04-01 01:53:43.000000 geocat.comp-2023.3.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      247 2023-04-01 01:53:43.000000 geocat.comp-2023.3.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     6654 2023-04-01 01:54:11.033527 geocat.comp-2023.3.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5869 2023-04-01 01:53:43.000000 geocat.comp-2023.3.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-01 01:54:11.033527 geocat.comp-2023.3.2/build_envs/
--rw-r--r--   0 runner    (1001) docker     (123)      408 2023-04-01 01:53:43.000000 geocat.comp-2023.3.2/build_envs/docs.yml
--rw-r--r--   0 runner    (1001) docker     (123)      588 2023-04-01 01:53:43.000000 geocat.comp-2023.3.2/build_envs/environment.yml
--rw-r--r--   0 runner    (1001) docker     (123)      268 2023-04-01 01:53:43.000000 geocat.comp-2023.3.2/build_envs/upstream-dev-environment.yml
--rw-r--r--   0 runner    (1001) docker     (123)      161 2023-04-01 01:53:43.000000 geocat.comp-2023.3.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      363 2023-04-01 01:53:43.000000 geocat.comp-2023.3.2/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1512 2023-04-01 01:54:11.033527 geocat.comp-2023.3.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-04-01 01:53:43.000000 geocat.comp-2023.3.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-01 01:54:11.029527 geocat.comp-2023.3.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-01 01:54:11.033527 geocat.comp-2023.3.2/src/geocat/
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-04-01 01:53:43.000000 geocat.comp-2023.3.2/src/geocat/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-01 01:54:11.033527 geocat.comp-2023.3.2/src/geocat/comp/
--rw-r--r--   0 runner    (1001) docker     (123)     1427 2023-04-01 01:53:43.000000 geocat.comp-2023.3.2/src/geocat/comp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    30249 2023-04-01 01:53:43.000000 geocat.comp-2023.3.2/src/geocat/comp/climatologies.py
--rw-r--r--   0 runner    (1001) docker     (123)    11081 2023-04-01 01:53:43.000000 geocat.comp-2023.3.2/src/geocat/comp/fourier_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)      923 2023-04-01 01:53:43.000000 geocat.comp-2023.3.2/src/geocat/comp/gc_util.py
--rw-r--r--   0 runner    (1001) docker     (123)     8523 2023-04-01 01:53:43.000000 geocat.comp-2023.3.2/src/geocat/comp/gradient.py
--rw-r--r--   0 runner    (1001) docker     (123)    26715 2023-04-01 01:53:43.000000 geocat.comp-2023.3.2/src/geocat/comp/interpolation.py
--rw-r--r--   0 runner    (1001) docker     (123)    54706 2023-04-01 01:53:43.000000 geocat.comp-2023.3.2/src/geocat/comp/meteorology.py
--rw-r--r--   0 runner    (1001) docker     (123)     9297 2023-04-01 01:53:43.000000 geocat.comp-2023.3.2/src/geocat/comp/spherical.py
--rw-r--r--   0 runner    (1001) docker     (123)    20519 2023-04-01 01:53:43.000000 geocat.comp-2023.3.2/src/geocat/comp/stats.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-01 01:54:11.033527 geocat.comp-2023.3.2/src/geocat.comp.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6654 2023-04-01 01:54:10.000000 geocat.comp-2023.3.2/src/geocat.comp.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      788 2023-04-01 01:54:10.000000 geocat.comp-2023.3.2/src/geocat.comp.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-01 01:54:10.000000 geocat.comp-2023.3.2/src/geocat.comp.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-01 01:54:10.000000 geocat.comp-2023.3.2/src/geocat.comp.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      241 2023-04-01 01:54:10.000000 geocat.comp-2023.3.2/src/geocat.comp.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-01 01:54:10.000000 geocat.comp-2023.3.2/src/geocat.comp.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 15:41:27.626870 geocat.comp-2023.5.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     5888 2023-05-05 15:41:02.000000 geocat.comp-2023.5.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      998 2023-05-05 15:41:02.000000 geocat.comp-2023.5.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      476 2023-05-05 15:41:02.000000 geocat.comp-2023.5.0/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      286 2023-05-05 15:41:02.000000 geocat.comp-2023.5.0/CITATION.cff
+-rw-r--r--   0 runner    (1001) docker     (123)     4030 2023-05-05 15:41:02.000000 geocat.comp-2023.5.0/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)      175 2023-05-05 15:41:02.000000 geocat.comp-2023.5.0/INSTALLATION.md
+-rw-r--r--   0 runner    (1001) docker     (123)    11377 2023-05-05 15:41:02.000000 geocat.comp-2023.5.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      247 2023-05-05 15:41:02.000000 geocat.comp-2023.5.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     6654 2023-05-05 15:41:27.626870 geocat.comp-2023.5.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5869 2023-05-05 15:41:02.000000 geocat.comp-2023.5.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 15:41:27.626870 geocat.comp-2023.5.0/build_envs/
+-rw-r--r--   0 runner    (1001) docker     (123)      408 2023-05-05 15:41:02.000000 geocat.comp-2023.5.0/build_envs/docs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      588 2023-05-05 15:41:02.000000 geocat.comp-2023.5.0/build_envs/environment.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      268 2023-05-05 15:41:02.000000 geocat.comp-2023.5.0/build_envs/upstream-dev-environment.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      161 2023-05-05 15:41:02.000000 geocat.comp-2023.5.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      363 2023-05-05 15:41:02.000000 geocat.comp-2023.5.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1512 2023-05-05 15:41:27.630870 geocat.comp-2023.5.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-05-05 15:41:02.000000 geocat.comp-2023.5.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 15:41:27.622870 geocat.comp-2023.5.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 15:41:27.626870 geocat.comp-2023.5.0/src/geocat/
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-05-05 15:41:02.000000 geocat.comp-2023.5.0/src/geocat/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 15:41:27.626870 geocat.comp-2023.5.0/src/geocat/comp/
+-rw-r--r--   0 runner    (1001) docker     (123)     1427 2023-05-05 15:41:02.000000 geocat.comp-2023.5.0/src/geocat/comp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30249 2023-05-05 15:41:02.000000 geocat.comp-2023.5.0/src/geocat/comp/climatologies.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11081 2023-05-05 15:41:02.000000 geocat.comp-2023.5.0/src/geocat/comp/fourier_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)      923 2023-05-05 15:41:02.000000 geocat.comp-2023.5.0/src/geocat/comp/gc_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10065 2023-05-05 15:41:02.000000 geocat.comp-2023.5.0/src/geocat/comp/gradient.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26715 2023-05-05 15:41:02.000000 geocat.comp-2023.5.0/src/geocat/comp/interpolation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    54706 2023-05-05 15:41:02.000000 geocat.comp-2023.5.0/src/geocat/comp/meteorology.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9297 2023-05-05 15:41:02.000000 geocat.comp-2023.5.0/src/geocat/comp/spherical.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20519 2023-05-05 15:41:02.000000 geocat.comp-2023.5.0/src/geocat/comp/stats.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 15:41:27.626870 geocat.comp-2023.5.0/src/geocat.comp.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6654 2023-05-05 15:41:27.000000 geocat.comp-2023.5.0/src/geocat.comp.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      788 2023-05-05 15:41:27.000000 geocat.comp-2023.5.0/src/geocat.comp.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 15:41:27.000000 geocat.comp-2023.5.0/src/geocat.comp.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 15:41:27.000000 geocat.comp-2023.5.0/src/geocat.comp.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      241 2023-05-05 15:41:27.000000 geocat.comp-2023.5.0/src/geocat.comp.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-05 15:41:27.000000 geocat.comp-2023.5.0/src/geocat.comp.egg-info/top_level.txt
```

### Comparing `geocat.comp-2023.3.2/.gitignore` & `geocat.comp-2023.5.0/.gitignore`

 * *Files identical despite different names*

### Comparing `geocat.comp-2023.3.2/.pre-commit-config.yaml` & `geocat.comp-2023.5.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `geocat.comp-2023.3.2/CONTRIBUTING.md` & `geocat.comp-2023.5.0/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `geocat.comp-2023.3.2/LICENSE` & `geocat.comp-2023.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `geocat.comp-2023.3.2/PKG-INFO` & `geocat.comp-2023.5.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: geocat.comp
-Version: 2023.3.2
+Version: 2023.5.0
 Summary: GeoCAT-comp is computational component of the GeoCAT project and
 Home-page: https://geocat-comp.readthedocs.io
 Author: GeoCAT Team
 Author-email: geocat@ucar.edu
 License: Apache-2.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

### Comparing `geocat.comp-2023.3.2/README.md` & `geocat.comp-2023.5.0/README.md`

 * *Files identical despite different names*

### Comparing `geocat.comp-2023.3.2/build_envs/environment.yml` & `geocat.comp-2023.5.0/build_envs/environment.yml`

 * *Files identical despite different names*

### Comparing `geocat.comp-2023.3.2/setup.cfg` & `geocat.comp-2023.5.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `geocat.comp-2023.3.2/src/geocat/comp/__init__.py` & `geocat.comp-2023.5.0/src/geocat/comp/__init__.py`

 * *Files identical despite different names*

### Comparing `geocat.comp-2023.3.2/src/geocat/comp/climatologies.py` & `geocat.comp-2023.5.0/src/geocat/comp/climatologies.py`

 * *Files identical despite different names*

### Comparing `geocat.comp-2023.3.2/src/geocat/comp/fourier_filters.py` & `geocat.comp-2023.5.0/src/geocat/comp/fourier_filters.py`

 * *Files identical despite different names*

### Comparing `geocat.comp-2023.3.2/src/geocat/comp/gc_util.py` & `geocat.comp-2023.5.0/src/geocat/comp/gc_util.py`

 * *Files identical despite different names*

### Comparing `geocat.comp-2023.3.2/src/geocat/comp/gradient.py` & `geocat.comp-2023.5.0/src/geocat/comp/gradient.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 from typing import Union
 
 import numpy as np
 import xarray as xr
 
-SupportedTypes = Union[np.ndarray, xr.DataArray]
-XTypes = Union[xr.DataArray, xr.Dataset]
+SupportedTypes = Union[np.ndarray, xr.DataArray, xr.Dataset]
 
 d2r = 1.74532925199432957692369e-02  # degrees to radians conversion factor
 
 
 def _rad_lat_wgs84(lat: SupportedTypes,):
     r"""The radius calculation for the wgs84 ellipsoid at a latitude uses a
     taylor series from.
@@ -172,62 +171,91 @@
     `gradsf <https://www.ncl.ucar.edu/Document/Functions/Built-in/gradsf.shtml>`__,
     `gradsg <https://www.ncl.ucar.edu/Document/Functions/Built-in/gradsg.shtml>`__
     """
 
     return _rad_lat_wgs84(lat) * np.cos(lat * d2r) * lon * d2r
 
 
-def gradient(data: xr.DataArray) -> [xr.DataArray]:
+def gradient(data: SupportedTypes,
+             lon: SupportedTypes = None,
+             lat: SupportedTypes = None) -> xr.DataArray:
     r"""Extract and return the gradient values of a dataset at each point in the
     dataset. Assuming that the data points are on the surface of the WGS84
     ellipsoid.
 
     Parameters
     ----------
     data : :class:`numpy.ndarray`, :class:`xarray.DataArray`
         n-dimensional dataset, with orthographic latitude longitude coordinates
 
+    lon: :class:`numpy.ndarray`, :class:`xarray.DataArray`
+         1 or 2-dimensional dataset of longitudinal coordinates
+
+    lat: :class:`numpy.ndarray`, :class:`xarray.DataArray`
+        1 or 2-dimensional dataset of latitudinal coordinates
+
     Returns
     -------
     gradients : list of :class:`numpy.ndarray`, list of :class:`xarray.DataArray`
         longitudinal and latitudinal gradients calculated using th WGS84 geoid.
 
     See Also
     --------
     Related NCL Functions:
     `grad_latlon_cfd <https://www.ncl.ucar.edu/Document/Functions/Contributed/grad_latlon_cfd.shtml>`__,
     `gradsf <https://www.ncl.ucar.edu/Document/Functions/Built-in/gradsf.shtml>`__,
     `gradsg <https://www.ncl.ucar.edu/Document/Functions/Built-in/gradsg.shtml>`__
     """
 
-    lon2d, lat2d = np.meshgrid(data.coords['lon'], data.coords['lat'])
+    if (lat is None or lon is None):
+        if type(data) in [xr.core.dataarray.DataArray, xr.core.dataset.Dataset]:
+            if data.coords is not None:
+                if 'lat' in data.coords.keys() and 'lon' in data.coords.keys():
+                    lon = data.coords['lon']
+                    lat = data.coords['lat']
+        elif type(data) is type(np.ndarray):
+            raise Exception('lat or lon is None. \
+            If the input data are in a numpy.ndarray, \
+            lat and lon as either 1d or 2d ndarrays must be provided.')
+        else:
+            raise Exception('Input data of type ' + str(type(data)) +
+                            ' are not in supported data type. \
+            Supported types are [numpy.ndarray, xarray.DataArray, xarray.Dataset]'
+                           )
+    # at this point we know that we have *something* in lat and lon
+    if len(lon.shape) == 1 and len(lat.shape) == 1:  #in theroy can be split
+        lon2d, lat2d = np.meshgrid(lon, lat)
+    elif len(lon.shape) == 2 and len(lat.shape) == 2:
+        lon2d, lat2d = lon, lat
+    else:
+        raise ValueError("lat or lon must be either both 1d or 2d.")
+
+    axis0loc = _arc_lat_wgs84(lat2d)
+    axis1loc = _arc_lon_wgs84(lon2d, lat2d)
+
+    axis0dist = np.gradient(axis0loc, axis=0)
+    axis1dist = np.gradient(axis1loc, axis=1)
+
+    grad = np.gradient(data)
 
-    axis0loc = xr.DataArray(
-        _arc_lat_wgs84(lat2d),
-        coords=data.coords,
-        dims=data.dims,
-    )
-    axis1loc = xr.DataArray(
-        _arc_lon_wgs84(lon2d, lat2d),
-        coords=data.coords,
-        dims=data.dims,
-    )
-
-    axis0dist = xr.DataArray(
-        np.gradient(axis0loc, axis=0),
-        coords=data.coords,
-        dims=data.dims,
-    )
-    axis1dist = xr.DataArray(
-        np.gradient(axis1loc, axis=1),
-        coords=data.coords,
-        dims=data.dims,
-    )
-
-    grad = xr.DataArray(
-        np.gradient(data),
-        dims=('dir',) + data.dims,
-    )
     axis0grad = grad[0] / axis0dist
     axis1grad = grad[1] / axis1dist
 
+    if type(data) in [xr.core.dataarray.DataArray, xr.core.dataset.Dataset]:
+        axis0grad = xr.DataArray(
+            axis0grad,
+            dims=['x', 'y'],
+            coords=dict(
+                lon=(['x', 'y'], lon2d.data),
+                lat=(['x', 'y'], lat2d.data),
+            ),
+        )
+        axis1grad = xr.DataArray(
+            axis1grad,
+            dims=['x', 'y'],
+            coords=dict(
+                lon=(['x', 'y'], lon2d.data),
+                lat=(['x', 'y'], lat2d.data),
+            ),
+        )
+
     return [axis0grad, axis1grad]
```

### Comparing `geocat.comp-2023.3.2/src/geocat/comp/interpolation.py` & `geocat.comp-2023.5.0/src/geocat/comp/interpolation.py`

 * *Files identical despite different names*

### Comparing `geocat.comp-2023.3.2/src/geocat/comp/meteorology.py` & `geocat.comp-2023.5.0/src/geocat/comp/meteorology.py`

 * *Files identical despite different names*

### Comparing `geocat.comp-2023.3.2/src/geocat/comp/spherical.py` & `geocat.comp-2023.5.0/src/geocat/comp/spherical.py`

 * *Files identical despite different names*

### Comparing `geocat.comp-2023.3.2/src/geocat/comp/stats.py` & `geocat.comp-2023.5.0/src/geocat/comp/stats.py`

 * *Files identical despite different names*

### Comparing `geocat.comp-2023.3.2/src/geocat.comp.egg-info/PKG-INFO` & `geocat.comp-2023.5.0/src/geocat.comp.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: geocat.comp
-Version: 2023.3.2
+Version: 2023.5.0
 Summary: GeoCAT-comp is computational component of the GeoCAT project and
 Home-page: https://geocat-comp.readthedocs.io
 Author: GeoCAT Team
 Author-email: geocat@ucar.edu
 License: Apache-2.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

### Comparing `geocat.comp-2023.3.2/src/geocat.comp.egg-info/SOURCES.txt` & `geocat.comp-2023.5.0/src/geocat.comp.egg-info/SOURCES.txt`

 * *Files identical despite different names*

