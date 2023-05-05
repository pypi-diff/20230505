# Comparing `tmp/xugrid-0.3.0.tar.gz` & `tmp/xugrid-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xugrid-0.3.0.tar", last modified: Tue Mar 14 17:39:45 2023, max compression
+gzip compressed data, was "xugrid-0.4.0.tar", last modified: Fri May  5 15:07:53 2023, max compression
```

## Comparing `xugrid-0.3.0.tar` & `xugrid-0.4.0.tar`

### file list

```diff
@@ -1,64 +1,64 @@
-drwxrwxrwx   0        0        0        0 2023-03-14 17:39:45.200731 xugrid-0.3.0/
--rw-rw-rw-   0        0        0     1079 2021-09-15 16:10:43.000000 xugrid-0.3.0/LICENSE
--rw-rw-rw-   0        0        0       34 2021-10-06 12:44:47.000000 xugrid-0.3.0/MANIFEST.in
--rw-rw-rw-   0        0        0     3298 2023-03-14 17:39:45.201728 xugrid-0.3.0/PKG-INFO
--rw-rw-rw-   0        0        0     2157 2023-03-13 10:25:22.000000 xugrid-0.3.0/README.rst
--rw-rw-rw-   0        0        0     2199 2023-03-14 17:29:52.000000 xugrid-0.3.0/pyproject.toml
--rw-rw-rw-   0        0        0      159 2023-03-14 17:39:45.203839 xugrid-0.3.0/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-03-14 17:39:44.784832 xugrid-0.3.0/tests/
--rw-rw-rw-   0        0        0    13855 2023-03-13 10:25:22.000000 xugrid-0.3.0/tests/test_connectivity.py
--rw-rw-rw-   0        0        0    10108 2023-03-13 10:25:22.000000 xugrid-0.3.0/tests/test_conventions.py
--rw-rw-rw-   0        0        0     9027 2023-03-13 10:25:22.000000 xugrid-0.3.0/tests/test_conversion.py
--rw-rw-rw-   0        0        0     1008 2023-03-13 10:25:22.000000 xugrid-0.3.0/tests/test_data.py
--rw-rw-rw-   0        0        0      851 2023-03-13 10:25:22.000000 xugrid-0.3.0/tests/test_interpolate.py
--rw-rw-rw-   0        0        0     1219 2023-03-13 10:25:22.000000 xugrid-0.3.0/tests/test_meshkernel_utils.py
--rw-rw-rw-   0        0        0     9084 2023-03-13 10:25:22.000000 xugrid-0.3.0/tests/test_plot.py
--rw-rw-rw-   0        0        0     4245 2023-03-13 10:25:22.000000 xugrid-0.3.0/tests/test_snap.py
--rw-rw-rw-   0        0        0     9101 2023-03-13 10:25:22.000000 xugrid-0.3.0/tests/test_ugrid1d.py
--rw-rw-rw-   0        0        0    27735 2023-03-13 10:25:22.000000 xugrid-0.3.0/tests/test_ugrid2d.py
--rw-rw-rw-   0        0        0    24989 2023-03-13 10:25:22.000000 xugrid-0.3.0/tests/test_ugrid_dataset.py
--rw-rw-rw-   0        0        0     8360 2023-03-13 10:25:22.000000 xugrid-0.3.0/tests/test_voronoi.py
-drwxrwxrwx   0        0        0        0 2023-03-14 17:39:44.832816 xugrid-0.3.0/xugrid/
--rw-rw-rw-   0        0        0     1020 2023-03-13 10:25:22.000000 xugrid-0.3.0/xugrid/__init__.py
--rw-rw-rw-   0        0        0     1203 2023-03-13 10:25:22.000000 xugrid-0.3.0/xugrid/constants.py
--rw-rw-rw-   0        0        0     8398 2023-03-13 10:25:22.000000 xugrid-0.3.0/xugrid/conversion.py
-drwxrwxrwx   0        0        0        0 2023-03-14 17:39:44.911812 xugrid-0.3.0/xugrid/core/
--rw-rw-rw-   0        0        0     2434 2023-03-13 10:25:22.000000 xugrid-0.3.0/xugrid/core/accessorbase.py
--rw-rw-rw-   0        0        0     3516 2023-03-13 10:25:22.000000 xugrid-0.3.0/xugrid/core/common.py
--rw-rw-rw-   0        0        0    18426 2023-03-13 10:25:22.000000 xugrid-0.3.0/xugrid/core/dataarray_accessor.py
--rw-rw-rw-   0        0        0    11732 2023-03-13 10:25:22.000000 xugrid-0.3.0/xugrid/core/dataset_accessor.py
--rw-rw-rw-   0        0        0    11821 2023-03-13 10:25:22.000000 xugrid-0.3.0/xugrid/core/wrap.py
-drwxrwxrwx   0        0        0        0 2023-03-14 17:39:44.948361 xugrid-0.3.0/xugrid/data/
--rw-rw-rw-   0        0        0      126 2023-03-13 10:25:22.000000 xugrid-0.3.0/xugrid/data/__init__.py
--rw-rw-rw-   0        0        0      331 2023-03-13 10:25:22.000000 xugrid-0.3.0/xugrid/data/registry.txt
--rw-rw-rw-   0        0        0     2109 2023-03-13 10:25:22.000000 xugrid-0.3.0/xugrid/data/sample_data.py
--rw-rw-rw-   0        0        0     3083 2023-03-13 10:25:22.000000 xugrid-0.3.0/xugrid/data/synthetic.py
--rw-rw-rw-   0        0        0     1203 2023-03-13 10:25:22.000000 xugrid-0.3.0/xugrid/meshkernel_utils.py
-drwxrwxrwx   0        0        0        0 2023-03-14 17:39:44.976359 xugrid-0.3.0/xugrid/plot/
--rw-rw-rw-   0        0        0      149 2023-03-13 10:25:22.000000 xugrid-0.3.0/xugrid/plot/__init__.py
--rw-rw-rw-   0        0        0    23871 2023-03-13 10:25:22.000000 xugrid-0.3.0/xugrid/plot/plot.py
-drwxrwxrwx   0        0        0        0 2023-03-14 17:39:45.078609 xugrid-0.3.0/xugrid/regrid/
--rw-rw-rw-   0        0        0     7616 2023-03-13 10:25:22.000000 xugrid-0.3.0/xugrid/regrid/overlap_1d.py
--rw-rw-rw-   0        0        0     5015 2023-03-14 17:12:37.000000 xugrid-0.3.0/xugrid/regrid/reduce.py
--rw-rw-rw-   0        0        0    15067 2023-03-13 10:25:22.000000 xugrid-0.3.0/xugrid/regrid/regridder.py
--rw-rw-rw-   0        0        0     1998 2023-03-13 10:25:22.000000 xugrid-0.3.0/xugrid/regrid/structured.py
--rw-rw-rw-   0        0        0     4050 2023-03-13 10:25:22.000000 xugrid-0.3.0/xugrid/regrid/unstructured.py
--rw-rw-rw-   0        0        0      985 2023-03-13 10:25:22.000000 xugrid-0.3.0/xugrid/regrid/utils.py
--rw-rw-rw-   0        0        0     3661 2023-03-13 10:25:22.000000 xugrid-0.3.0/xugrid/regrid/weight_matrix.py
-drwxrwxrwx   0        0        0        0 2023-03-14 17:39:45.192732 xugrid-0.3.0/xugrid/ugrid/
--rw-rw-rw-   0        0        0        0 2023-03-13 10:25:22.000000 xugrid-0.3.0/xugrid/ugrid/__init__.py
--rw-rw-rw-   0        0        0    17652 2023-03-13 10:25:22.000000 xugrid-0.3.0/xugrid/ugrid/connectivity.py
--rw-rw-rw-   0        0        0    14380 2023-03-13 10:25:22.000000 xugrid-0.3.0/xugrid/ugrid/conventions.py
--rw-rw-rw-   0        0        0     4996 2023-03-13 10:25:22.000000 xugrid-0.3.0/xugrid/ugrid/interpolate.py
--rw-rw-rw-   0        0        0    10227 2023-03-13 10:25:22.000000 xugrid-0.3.0/xugrid/ugrid/partitioning.py
--rw-rw-rw-   0        0        0    14748 2023-03-13 10:25:22.000000 xugrid-0.3.0/xugrid/ugrid/snapping.py
--rw-rw-rw-   0        0        0    17809 2023-03-13 10:25:22.000000 xugrid-0.3.0/xugrid/ugrid/ugrid1d.py
--rw-rw-rw-   0        0        0    49530 2023-03-13 10:25:22.000000 xugrid-0.3.0/xugrid/ugrid/ugrid2d.py
--rw-rw-rw-   0        0        0    19739 2023-03-13 10:25:22.000000 xugrid-0.3.0/xugrid/ugrid/ugridbase.py
--rw-rw-rw-   0        0        0    13753 2023-03-13 10:25:22.000000 xugrid-0.3.0/xugrid/ugrid/voronoi.py
-drwxrwxrwx   0        0        0        0 2023-03-14 17:39:44.861889 xugrid-0.3.0/xugrid.egg-info/
--rw-rw-rw-   0        0        0     3298 2023-03-14 17:39:44.000000 xugrid-0.3.0/xugrid.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1311 2023-03-14 17:39:44.000000 xugrid-0.3.0/xugrid.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-14 17:39:44.000000 xugrid-0.3.0/xugrid.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      252 2023-03-14 17:39:44.000000 xugrid-0.3.0/xugrid.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-03-14 17:39:44.000000 xugrid-0.3.0/xugrid.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-05 15:07:53.242926 xugrid-0.4.0/
+-rw-rw-rw-   0        0        0     1079 2021-09-15 16:10:43.000000 xugrid-0.4.0/LICENSE
+-rw-rw-rw-   0        0        0       34 2021-10-06 12:44:47.000000 xugrid-0.4.0/MANIFEST.in
+-rw-rw-rw-   0        0        0     3298 2023-05-05 15:07:53.242926 xugrid-0.4.0/PKG-INFO
+-rw-rw-rw-   0        0        0     2157 2023-03-13 10:25:22.000000 xugrid-0.4.0/README.rst
+-rw-rw-rw-   0        0        0     2199 2023-05-05 15:03:53.000000 xugrid-0.4.0/pyproject.toml
+-rw-rw-rw-   0        0        0      159 2023-05-05 15:07:53.244925 xugrid-0.4.0/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-05 15:07:53.031921 xugrid-0.4.0/tests/
+-rw-rw-rw-   0        0        0    15587 2023-04-21 11:32:07.000000 xugrid-0.4.0/tests/test_connectivity.py
+-rw-rw-rw-   0        0        0    10108 2023-03-13 10:25:22.000000 xugrid-0.4.0/tests/test_conventions.py
+-rw-rw-rw-   0        0        0     9027 2023-03-13 10:25:22.000000 xugrid-0.4.0/tests/test_conversion.py
+-rw-rw-rw-   0        0        0     1008 2023-03-13 10:25:22.000000 xugrid-0.4.0/tests/test_data.py
+-rw-rw-rw-   0        0        0      851 2023-03-13 10:25:22.000000 xugrid-0.4.0/tests/test_interpolate.py
+-rw-rw-rw-   0        0        0     1219 2023-03-13 10:25:22.000000 xugrid-0.4.0/tests/test_meshkernel_utils.py
+-rw-rw-rw-   0        0        0     9084 2023-03-13 10:25:22.000000 xugrid-0.4.0/tests/test_plot.py
+-rw-rw-rw-   0        0        0     4245 2023-03-13 10:25:22.000000 xugrid-0.4.0/tests/test_snap.py
+-rw-rw-rw-   0        0        0     9280 2023-04-21 11:32:07.000000 xugrid-0.4.0/tests/test_ugrid1d.py
+-rw-rw-rw-   0        0        0    30534 2023-04-21 11:32:07.000000 xugrid-0.4.0/tests/test_ugrid2d.py
+-rw-rw-rw-   0        0        0    26751 2023-04-21 11:32:07.000000 xugrid-0.4.0/tests/test_ugrid_dataset.py
+-rw-rw-rw-   0        0        0    10444 2023-04-21 11:32:07.000000 xugrid-0.4.0/tests/test_voronoi.py
+drwxrwxrwx   0        0        0        0 2023-05-05 15:07:53.049922 xugrid-0.4.0/xugrid/
+-rw-rw-rw-   0        0        0     1020 2023-03-13 10:25:22.000000 xugrid-0.4.0/xugrid/__init__.py
+-rw-rw-rw-   0        0        0     1203 2023-03-13 10:25:22.000000 xugrid-0.4.0/xugrid/constants.py
+-rw-rw-rw-   0        0        0     8398 2023-03-13 10:25:22.000000 xugrid-0.4.0/xugrid/conversion.py
+drwxrwxrwx   0        0        0        0 2023-05-05 15:07:53.103930 xugrid-0.4.0/xugrid/core/
+-rw-rw-rw-   0        0        0     3303 2023-04-21 11:32:07.000000 xugrid-0.4.0/xugrid/core/accessorbase.py
+-rw-rw-rw-   0        0        0     3516 2023-03-13 10:25:22.000000 xugrid-0.4.0/xugrid/core/common.py
+-rw-rw-rw-   0        0        0    18334 2023-04-21 11:32:07.000000 xugrid-0.4.0/xugrid/core/dataarray_accessor.py
+-rw-rw-rw-   0        0        0    13439 2023-04-21 11:32:07.000000 xugrid-0.4.0/xugrid/core/dataset_accessor.py
+-rw-rw-rw-   0        0        0    11821 2023-03-13 10:25:22.000000 xugrid-0.4.0/xugrid/core/wrap.py
+drwxrwxrwx   0        0        0        0 2023-05-05 15:07:53.124929 xugrid-0.4.0/xugrid/data/
+-rw-rw-rw-   0        0        0      126 2023-03-13 10:25:22.000000 xugrid-0.4.0/xugrid/data/__init__.py
+-rw-rw-rw-   0        0        0      331 2023-04-21 11:32:07.000000 xugrid-0.4.0/xugrid/data/registry.txt
+-rw-rw-rw-   0        0        0     2109 2023-03-13 10:25:22.000000 xugrid-0.4.0/xugrid/data/sample_data.py
+-rw-rw-rw-   0        0        0     3083 2023-03-13 10:25:22.000000 xugrid-0.4.0/xugrid/data/synthetic.py
+-rw-rw-rw-   0        0        0     1203 2023-03-13 10:25:22.000000 xugrid-0.4.0/xugrid/meshkernel_utils.py
+drwxrwxrwx   0        0        0        0 2023-05-05 15:07:53.138920 xugrid-0.4.0/xugrid/plot/
+-rw-rw-rw-   0        0        0      149 2023-03-13 10:25:22.000000 xugrid-0.4.0/xugrid/plot/__init__.py
+-rw-rw-rw-   0        0        0    24058 2023-04-21 11:32:07.000000 xugrid-0.4.0/xugrid/plot/plot.py
+drwxrwxrwx   0        0        0        0 2023-05-05 15:07:53.175924 xugrid-0.4.0/xugrid/regrid/
+-rw-rw-rw-   0        0        0     7616 2023-03-13 10:25:22.000000 xugrid-0.4.0/xugrid/regrid/overlap_1d.py
+-rw-rw-rw-   0        0        0     5015 2023-03-14 17:12:37.000000 xugrid-0.4.0/xugrid/regrid/reduce.py
+-rw-rw-rw-   0        0        0    15067 2023-03-13 10:25:22.000000 xugrid-0.4.0/xugrid/regrid/regridder.py
+-rw-rw-rw-   0        0        0     1998 2023-03-13 10:25:22.000000 xugrid-0.4.0/xugrid/regrid/structured.py
+-rw-rw-rw-   0        0        0     4050 2023-03-13 10:25:22.000000 xugrid-0.4.0/xugrid/regrid/unstructured.py
+-rw-rw-rw-   0        0        0      985 2023-03-13 10:25:22.000000 xugrid-0.4.0/xugrid/regrid/utils.py
+-rw-rw-rw-   0        0        0     3661 2023-03-13 10:25:22.000000 xugrid-0.4.0/xugrid/regrid/weight_matrix.py
+drwxrwxrwx   0        0        0        0 2023-05-05 15:07:53.240925 xugrid-0.4.0/xugrid/ugrid/
+-rw-rw-rw-   0        0        0        0 2023-03-13 10:25:22.000000 xugrid-0.4.0/xugrid/ugrid/__init__.py
+-rw-rw-rw-   0        0        0    18746 2023-04-21 11:32:07.000000 xugrid-0.4.0/xugrid/ugrid/connectivity.py
+-rw-rw-rw-   0        0        0    14841 2023-04-21 11:32:07.000000 xugrid-0.4.0/xugrid/ugrid/conventions.py
+-rw-rw-rw-   0        0        0     4996 2023-03-13 10:25:22.000000 xugrid-0.4.0/xugrid/ugrid/interpolate.py
+-rw-rw-rw-   0        0        0    10227 2023-03-13 10:25:22.000000 xugrid-0.4.0/xugrid/ugrid/partitioning.py
+-rw-rw-rw-   0        0        0    14979 2023-05-05 14:49:08.000000 xugrid-0.4.0/xugrid/ugrid/snapping.py
+-rw-rw-rw-   0        0        0    17949 2023-04-21 11:32:07.000000 xugrid-0.4.0/xugrid/ugrid/ugrid1d.py
+-rw-rw-rw-   0        0        0    53962 2023-04-21 11:32:07.000000 xugrid-0.4.0/xugrid/ugrid/ugrid2d.py
+-rw-rw-rw-   0        0        0    19806 2023-04-21 11:32:07.000000 xugrid-0.4.0/xugrid/ugrid/ugridbase.py
+-rw-rw-rw-   0        0        0    14113 2023-04-21 11:32:07.000000 xugrid-0.4.0/xugrid/ugrid/voronoi.py
+drwxrwxrwx   0        0        0        0 2023-05-05 15:07:53.063936 xugrid-0.4.0/xugrid.egg-info/
+-rw-rw-rw-   0        0        0     3298 2023-05-05 15:07:52.000000 xugrid-0.4.0/xugrid.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1311 2023-05-05 15:07:52.000000 xugrid-0.4.0/xugrid.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-05 15:07:52.000000 xugrid-0.4.0/xugrid.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      252 2023-05-05 15:07:52.000000 xugrid-0.4.0/xugrid.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-05-05 15:07:52.000000 xugrid-0.4.0/xugrid.egg-info/top_level.txt
```

### Comparing `xugrid-0.3.0/LICENSE` & `xugrid-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `xugrid-0.3.0/PKG-INFO` & `xugrid-0.4.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xugrid
-Version: 0.3.0
+Version: 0.4.0
 Summary: Xarray extension for unstructured grids
 Maintainer-email: Huite Bootsma <huite.bootsma@deltares.nl>
 License: MIT
 Project-URL: Home, https://github.com/deltares/xugrid
 Project-URL: Code, https://github.com/deltares/xugrid
 Project-URL: Issues, https://github.com/deltares/xugrid/issues
 Keywords: mesh,ugrid,unstructured grid,xarray
```

### Comparing `xugrid-0.3.0/README.rst` & `xugrid-0.4.0/README.rst`

 * *Files identical despite different names*

### Comparing `xugrid-0.3.0/pyproject.toml` & `xugrid-0.4.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 requires = ["setuptools>=64.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "xugrid"
 description = "Xarray extension for unstructured grids"
 readme = { file = "README.rst", content-type = "text/x-rst" }
-version = "0.3.0"
+version = "0.4.0"
 maintainers = [{ name = "Huite Bootsma", email = "huite.bootsma@deltares.nl" }]
 requires-python = ">=3.7"
 dependencies = [
     'pandas',
     'numba',
     'numba_celltree',
     'numpy',
```

### Comparing `xugrid-0.3.0/tests/test_connectivity.py` & `xugrid-0.4.0/tests/test_connectivity.py`

 * *Files 6% similar despite different names*

```diff
@@ -164,14 +164,44 @@
             [1, -1],  # 3
             [1, -1],  # 4
         ]
     )
     assert np.array_equal(actual, expected)
 
 
+def test_to_dense(triangle_mesh):
+    faces, fill_value = triangle_mesh
+    sparse = connectivity.to_sparse(faces, fill_value)
+    actual = connectivity.to_dense(sparse, fill_value)
+    assert np.array_equal(actual, np.sort(faces, axis=1))
+
+    with pytest.raises(ValueError, match="n_columns 2 is too small"):
+        connectivity.to_dense(sparse, fill_value, n_columns=2)
+
+    # now pad
+    actual = connectivity.to_dense(sparse, fill_value, n_columns=4)
+    expected = np.array(
+        [
+            [0, 1, 2, fill_value],
+            [1, 2, 3, fill_value],
+        ]
+    )
+    assert np.array_equal(actual, expected)
+
+    # and twice
+    actual = connectivity.to_dense(sparse, fill_value, n_columns=5)
+    expected = np.array(
+        [
+            [0, 1, 2, fill_value, fill_value],
+            [1, 2, 3, fill_value, fill_value],
+        ]
+    )
+    assert np.array_equal(actual, expected)
+
+
 def test_renumber():
     a = np.array(
         [
             [0, 1, 2],
             [10, 11, 12],
             [30, 31, 32],
         ]
@@ -357,14 +387,44 @@
             [2.0 / 3.0, 1.0 / 3.0],
             [1.5, 0.5],
         ]
     )
     assert np.allclose(actual, expected)
 
 
+def test_circumcenters_error(mixed_mesh):
+    faces, fill_value = mixed_mesh
+    nodes = np.array(
+        [
+            [0.0, 0.0],
+            [1.0, 0.0],
+            [1.0, 1.0],
+            [2.0, 0.0],
+            [2.0, 1.0],
+        ]
+    )
+    with pytest.raises(NotImplementedError):
+        connectivity.circumcenters(faces, fill_value, nodes[:, 0], nodes[:, 1])
+
+
+def test_circumcenters(triangle_mesh):
+    faces, fill_value = triangle_mesh
+    nodes = np.array(
+        [
+            [0.0, 1.0],
+            [0.0, 0.0],
+            [2.0, 0.0],
+            [1.0, -2.0],
+        ]
+    )
+    actual = connectivity.circumcenters(faces, fill_value, nodes[:, 0], nodes[:, 1])
+    expected = np.array([[1.0, 0.5], [1.0, -0.75]])
+    assert np.allclose(actual, expected)
+
+
 def test_structured_connectivity():
     active = np.array(
         [
             [True, True, False],
             [True, True, True],
             [True, False, True],
         ]
```

### Comparing `xugrid-0.3.0/tests/test_conventions.py` & `xugrid-0.4.0/tests/test_conventions.py`

 * *Files identical despite different names*

### Comparing `xugrid-0.3.0/tests/test_conversion.py` & `xugrid-0.4.0/tests/test_conversion.py`

 * *Files identical despite different names*

### Comparing `xugrid-0.3.0/tests/test_data.py` & `xugrid-0.4.0/tests/test_data.py`

 * *Files identical despite different names*

### Comparing `xugrid-0.3.0/tests/test_interpolate.py` & `xugrid-0.4.0/tests/test_interpolate.py`

 * *Files identical despite different names*

### Comparing `xugrid-0.3.0/tests/test_meshkernel_utils.py` & `xugrid-0.4.0/tests/test_meshkernel_utils.py`

 * *Files identical despite different names*

### Comparing `xugrid-0.3.0/tests/test_plot.py` & `xugrid-0.4.0/tests/test_plot.py`

 * *Files identical despite different names*

### Comparing `xugrid-0.3.0/tests/test_snap.py` & `xugrid-0.4.0/tests/test_snap.py`

 * *Files identical despite different names*

### Comparing `xugrid-0.3.0/tests/test_ugrid1d.py` & `xugrid-0.4.0/tests/test_ugrid1d.py`

 * *Files 2% similar despite different names*

```diff
@@ -92,14 +92,15 @@
     expected_coords = [
         [[0.0, 0.0], [1.0, 1.0]],
         [[1.0, 1.0], [2.0, 2.0]],
     ]
     actual_coords = grid.edge_node_coordinates
     assert actual_coords.shape == (2, 2, 2)
     assert np.allclose(actual_coords, expected_coords)
+    assert isinstance(grid.attrs, dict)
 
 
 def test_ugrid1d_egde_bounds():
     grid = grid1d()
     expected = np.array(
         [
             [0.0, 0.0, 1.0, 1.0],
@@ -162,14 +163,18 @@
     assert f"{NAME}" in ds
     assert f"{NAME}_nNodes" in ds.dims
     assert f"{NAME}_nEdges" in ds.dims
     assert f"{NAME}_node_x" in ds.coords
     assert f"{NAME}_node_y" in ds.coords
     assert f"{NAME}_edge_nodes" in ds
 
+    ds = grid.to_dataset(optional_attributes=True)
+    assert f"{NAME}_edge_x" in ds.coords
+    assert f"{NAME}_edge_y" in ds.coords
+
 
 def test_ugrid1d_dataset_roundtrip():
     grid = grid1d()
     ds = grid.to_dataset()
     grid2 = xugrid.Ugrid1d.from_dataset(grid.to_dataset())
     assert isinstance(grid2._dataset, xr.Dataset)
     assert grid2._dataset == ds
```

### Comparing `xugrid-0.3.0/tests/test_ugrid2d.py` & `xugrid-0.4.0/tests/test_ugrid2d.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import re
 from typing import NamedTuple
 
 import geopandas as gpd
 import numba_celltree
 import numpy as np
 import pyproj
 import pytest
@@ -103,14 +104,30 @@
     assert grid._dataset is None
     assert grid.node_x.flags["C_CONTIGUOUS"]
     assert grid.node_y.flags["C_CONTIGUOUS"]
     assert grid._edge_node_connectivity is None
     assert grid._face_edge_connectivity is None
 
 
+def test_ugrid2d_init__invalid_edge_nodes():
+    edge_nodes = np.vstack((EDGE_NODES, [6, 7]))
+    msg = re.escape(
+        "edge_node_connectivity is invalid, the following edges "
+        "are not associated with any face: [10]"
+    )
+    with pytest.raises(ValueError, match=msg):
+        xugrid.Ugrid2d(
+            node_x=VERTICES[:, 0],
+            node_y=VERTICES[:, 1],
+            fill_value=-1,
+            face_node_connectivity=FACES,
+            edge_node_connectivity=edge_nodes,
+        )
+
+
 def test_ugrid2d_alternative_init():
     custom_attrs = {
         "node_dimension": "nNetNode",
         "name": "mesh1d",
         "node_coordinates": "mesh1d_node_x mesh1d_node_y",
     }
     indexes = {"node_x": "mesh1d_node_x", "node_y": "mesh1d_node_y"}
@@ -148,14 +165,15 @@
     edge_node_coords = grid.edge_node_coordinates
     face_node_coords = grid.face_node_coordinates
     assert edge_node_coords.shape == (10, 2, 2)
     assert face_node_coords.shape == (4, 4, 2)
     are_nan = np.isnan(face_node_coords)
     assert are_nan[2:, -1:, :].all()
     assert not are_nan[:, :-1, :].any()
+    assert isinstance(grid.attrs, dict)
 
 
 def test_ugrid2d_edge_bounds():
     grid = grid2d()
     expected = np.array(
         [
             [0.0, 0.0, 1.0, 0.0],
@@ -211,14 +229,26 @@
     assert f"{NAME}" in ds
     assert f"{NAME}_nNodes" in ds.dims
     assert f"{NAME}_nFaces" in ds.dims
     assert f"{NAME}_node_x" in ds.coords
     assert f"{NAME}_node_y" in ds.coords
     assert f"{NAME}_face_nodes" in ds
 
+    ds = grid.to_dataset(optional_attributes=True)
+    assert f"{NAME}_edge_nodes" in ds
+    assert f"{NAME}_face_nodes" in ds
+    assert f"{NAME}_face_edges" in ds
+    assert f"{NAME}_face_faces" in ds
+    assert f"{NAME}_edge_faces" in ds
+    assert f"{NAME}_boundary_nodes" in ds
+    assert f"{NAME}_face_x" in ds
+    assert f"{NAME}_face_y" in ds
+    assert f"{NAME}_edge_x" in ds
+    assert f"{NAME}_edge_y" in ds
+
 
 def test_ugrid2d_set_node_coords():
     grid = grid2d()
     ds = xr.Dataset()
     lonvalues = VERTICES[:, 0] + 10.0
     latvalues = VERTICES[:, 1] + 10.0
     ds["lon"] = xr.DataArray(lonvalues, dims=[grid.node_dimension])
@@ -529,14 +559,31 @@
             [0, 0, 1, 1],
         ]
     )
     assert np.allclose(x, [0.25, 0.75, 1.25, 1.75])
     assert np.allclose(y, [1.75, 1.25, 0.75, 0.25])
     assert np.array_equal(index, expected_index)
 
+    # Test with alternative bounds
+    bounds = (-1.0, -1.0, 2.0, 2.0)
+    x, y, index = grid.rasterize(resolution=0.5, bounds=bounds)
+    expected_index = np.array(
+        [
+            [-1, -1, -1, 2, -1, -1],
+            [-1, -1, 2, 2, 3, -1],
+            [-1, -1, 0, 0, 1, 1],
+            [-1, -1, 0, 0, 1, 1],
+            [-1, -1, -1, -1, -1, -1],
+            [-1, -1, -1, -1, -1, -1],
+        ]
+    )
+    assert np.allclose(x, [-0.75, -0.25, 0.25, 0.75, 1.25, 1.75])
+    assert np.allclose(y, [1.75, 1.25, 0.75, 0.25, -0.25, -0.75])
+    assert np.array_equal(index, expected_index)
+
 
 class TestUgrid2dSelection:
     @pytest.fixture(autouse=True)
     def setup(self):
         self.grid = grid2d()
         self.obj = xr.DataArray([0, 1, 2, 3], dims=[self.grid.face_dimension])
 
@@ -552,21 +599,28 @@
         actual = self.grid.sel_points(obj=self.obj, x=x, y=y)
         assert isinstance(actual, xr.DataArray)
 
         dim = f"{NAME}_nFaces"
         expected = xr.DataArray(
             data=[0, 3],
             coords={
+                "index": (dim, [0, 1]),
                 "x": (dim, x),
                 "y": (dim, y),
             },
             dims=[dim],
         )
         assert expected.equals(actual)
 
+    def test_sel_points_out_of_bounds(self):
+        x = [-10.0, 0.5, -20.0, 1.5, -30.0]
+        y = [-10.0, 0.5, -20.0, 1.25, -30.0]
+        actual = self.grid.sel_points(obj=self.obj, x=x, y=y)
+        assert np.array_equal(actual["index"], [1, 3])
+
     def test_validate_indexer(self):
         with pytest.raises(ValueError, match="slice stop should be larger than"):
             self.grid._validate_indexer(slice(2, 0))
         with pytest.raises(ValueError, match="step should be None"):
             self.grid._validate_indexer(slice(None, 2, 1))
         with pytest.raises(ValueError, match="step should be None"):
             self.grid._validate_indexer(slice(0, None, 1))
@@ -638,14 +692,15 @@
     def test_sel__points_from_scalar(self):
         def check_output(actual):
             assert isinstance(actual, xr.DataArray)
             dim = f"{NAME}_nFaces"
             expected = xr.DataArray(
                 data=[0],
                 coords={
+                    "index": (dim, [0]),
                     "x": (dim, [0.5]),
                     "y": (dim, [0.5]),
                 },
                 dims=[dim],
             )
             assert expected.equals(actual)
 
@@ -768,14 +823,49 @@
     voronoi = grid.tesselate_centroidal_voronoi(add_vertices=False)
     assert voronoi.n_face == 7
 
     voronoi = grid.tesselate_centroidal_voronoi()
     assert voronoi.n_face == 7
 
 
+def test_tesselate_circumcenter_voronoi():
+    grid = grid2d()
+
+    # Can only deal with triangular grids
+    with pytest.raises(NotImplementedError):
+        grid.tesselate_circumcenter_voronoi()
+
+    # Now test with triangular grid
+    vertices = np.array(
+        [
+            [0.0, 0.0],  # 0
+            [2.0, 0.0],  # 1
+            [1.0, 1.0],  # 2
+            [2.0, 2.0],  # 3
+            [0.0, 2.0],  # 4
+        ]
+    )
+    faces = np.array(
+        [
+            [0, 1, 2],
+            [1, 3, 2],
+            [3, 4, 2],
+            [4, 0, 2],
+        ]
+    )
+    grid = xugrid.Ugrid2d(
+        node_x=vertices[:, 0],
+        node_y=vertices[:, 1],
+        fill_value=-1,
+        face_node_connectivity=faces,
+    )
+    voronoi = grid.tesselate_circumcenter_voronoi()
+    assert voronoi.n_face == 5
+
+
 def test_reverse_cuthill_mckee():
     grid = grid2d()
     new, index = grid.reverse_cuthill_mckee()
     assert isinstance(new, xugrid.Ugrid2d)
     assert np.allclose(new.node_coordinates, grid.node_coordinates)
     assert np.array_equal(index, [3, 2, 1, 0])
```

### Comparing `xugrid-0.3.0/tests/test_ugrid_dataset.py` & `xugrid-0.4.0/tests/test_ugrid_dataset.py`

 * *Files 2% similar despite different names*

```diff
@@ -302,14 +302,29 @@
 
     def test_to_dataset(self):
         uda2 = self.uda.copy()
         uda2.ugrid.obj.name = "test"
         actual = uda2.to_dataset()
         assert isinstance(actual, xugrid.UgridDataset)
 
+    def test_ugrid_to_dataset(self):
+        uda2 = self.uda.copy()
+        uda2.ugrid.obj.name = "test"
+        ds = uda2.ugrid.to_dataset(optional_attributes=True)
+        assert "mesh2d_edge_nodes" in ds
+        assert "mesh2d_face_nodes" in ds
+        assert "mesh2d_face_edges" in ds
+        assert "mesh2d_face_faces" in ds
+        assert "mesh2d_edge_faces" in ds
+        assert "mesh2d_boundary_nodes" in ds
+        assert "mesh2d_face_x" in ds
+        assert "mesh2d_face_y" in ds
+        assert "mesh2d_edge_x" in ds
+        assert "mesh2d_edge_y" in ds
+
     def test_to_netcdf(self, tmp_path):
         uda2 = self.uda.copy()
         uda2.ugrid.obj.name = "test"
         path = tmp_path / "uda-test.nc"
         uda2.ugrid.to_netcdf(path)
         assert path.exists()
 
@@ -475,14 +490,32 @@
 
         actual = self.uds.ugrid.sel(x=slice(0, 1), y=slice(1, None))
         assert isinstance(actual, xugrid.UgridDataset)
         assert actual["a"].shape == (1,)
         assert actual["b"].shape == (1,)
         assert actual.ugrid.grids[0].n_face == 1
 
+    def test_rasterize(self):
+        actual = self.uds.ugrid.rasterize(resolution=0.5)
+        x = [0.25, 0.75, 1.25, 1.75]
+        y = [1.75, 1.25, 0.75, 0.25]
+        assert isinstance(actual, xr.Dataset)
+        assert actual["a"].shape == (4, 4)
+        assert actual["b"].shape == (4, 4)
+        assert np.allclose(actual["x"], x)
+        assert np.allclose(actual["y"], y)
+
+        da = xr.DataArray(np.empty((4, 4)), {"y": y, "x": x}, ["y", "x"])
+        actual = self.uds.ugrid.rasterize_like(other=da)
+        assert isinstance(actual, xr.Dataset)
+        assert actual["a"].shape == (4, 4)
+        assert actual["b"].shape == (4, 4)
+        assert np.allclose(actual["x"], x)
+        assert np.allclose(actual["y"], y)
+
     def test_crs(self):
         uds = self.uds
         crs = uds.ugrid.crs
         assert crs == {"mesh2d": None}
 
         with pytest.raises(ValueError, match="grid not found"):
             uds.ugrid.set_crs(epsg=28992, topology="grid")
@@ -592,18 +625,30 @@
     assert "mesh2d_node_x" in subset_ds
     assert "mesh2d_node_y" in subset_ds
     assert "mesh2d_node_lon" in subset_ds
     assert "mesh2d_node_lat" in subset_ds
     assert subset_ds["mesh2d"].attrs["node_coordinates"] == attrs["node_coordinates"]
 
 
-def test_to_dataset():
+def test_ugrid_to_dataset():
     uds = xugrid.UgridDataset(UGRID_DS())
     assert uds.ugrid.to_dataset() == UGRID_DS()
 
+    ds = uds.ugrid.to_dataset(optional_attributes=True)
+    assert "mesh2d_edge_nodes" in ds
+    assert "mesh2d_face_nodes" in ds
+    assert "mesh2d_face_edges" in ds
+    assert "mesh2d_face_faces" in ds
+    assert "mesh2d_edge_faces" in ds
+    assert "mesh2d_boundary_nodes" in ds
+    assert "mesh2d_face_x" in ds
+    assert "mesh2d_face_y" in ds
+    assert "mesh2d_edge_x" in ds
+    assert "mesh2d_edge_y" in ds
+
 
 def test_open_dataset(tmp_path):
     path = tmp_path / "ugrid-dataset.nc"
     uds = xugrid.UgridDataset(UGRID_DS())
     uds.ugrid.to_netcdf(path)
 
     back = xugrid.open_dataset(path)
```

### Comparing `xugrid-0.3.0/tests/test_voronoi.py` & `xugrid-0.4.0/tests/test_voronoi.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import numpy as np
 import pytest
 
+import xugrid as xu
 from xugrid.ugrid import connectivity, voronoi
 
 
 def rowsort(a):
     return a[np.lexsort(a.T)]
 
 
@@ -242,7 +243,94 @@
             np.concatenate([expected_vertices, self.additional_vertices])
         )
         # This introduces hanging nodes
         assert actual_faces.shape == (12, 5)
         assert np.allclose(rowsort(vertices), expected_vertices)
         assert (face_i == -1).sum() == 10
         assert np.allclose(mesh_area(vertices, actual_faces), 6.0)
+
+
+def test_projected_vertices_on_edge():
+    """
+    For certain triangles, the voronoi projection falls exactly on the edge.
+         x
+        ---
+      -------
+    x -- o -- x
+         |
+         |
+         v
+
+    Where:
+
+    * x: the triangle vertices
+    * o: the circumcenter
+    * -->: the orthogonal voronoi ray
+
+    This results in a centroid which is identical to the voronoi ray edge
+    intersection. This will then create a zero length edge, which is obviously
+    problematic.
+    """
+    nodes = np.array(
+        [
+            [0.0, 0.0],  # 0
+            [0.0, 2.0],  # 1
+            [2.0, 2.0],  # 2
+            [0.0, 2.0],  # 3
+            [1.0, 1.0],  # 4
+        ]
+    )
+    faces = np.array(
+        [
+            [0, 1, 4],
+            [1, 2, 4],
+            [2, 3, 4],
+            [3, 0, 4],
+        ]
+    )
+    grid = xu.Ugrid2d(nodes[:, 0], nodes[:, 1], -1, faces)
+    voronoi_grid = grid.tesselate_circumcenter_voronoi()
+    assert voronoi_grid.n_face == 5
+
+
+def test_isolated_face():
+    """
+    The centroid of the left-most face should not be included.
+
+          +--+
+          |  |
+    +--+--+--+
+    |  |  |  |
+    +--+--+--+
+          |  |
+          +--+
+
+    """
+    nodes = np.array(
+        [
+            [0.0, 0.0],  # 0
+            [1.0, 0.0],  # 1
+            [2.0, 0.0],  # 2
+            [3.0, 0.0],  # 3
+            [0.0, 1.0],  # 4
+            [1.0, 1.0],  # 5
+            [2.0, 1.0],  # 6
+            [3.0, 1.0],  # 7
+            [2.0, -1.0],  # 8
+            [3.0, -1.0],  # 9
+            [2.0, 2.0],  # 10
+            [3.0, 2.0],  # 11
+        ]
+    )
+    faces = np.array(
+        [
+            [0, 1, 5, 4],
+            [1, 2, 6, 5],
+            [2, 3, 7, 6],
+            [8, 9, 3, 2],
+            [6, 7, 11, 10],
+        ]
+    )
+    grid = xu.Ugrid2d(nodes[:, 0], nodes[:, 1], -1, faces)
+    voronoi_grid = grid.tesselate_centroidal_voronoi(False, False)
+    assert voronoi_grid.n_face == 2
+    assert voronoi_grid.n_node == 4
```

### Comparing `xugrid-0.3.0/xugrid/__init__.py` & `xugrid-0.4.0/xugrid/__init__.py`

 * *Files identical despite different names*

### Comparing `xugrid-0.3.0/xugrid/constants.py` & `xugrid-0.4.0/xugrid/constants.py`

 * *Files identical despite different names*

### Comparing `xugrid-0.3.0/xugrid/conversion.py` & `xugrid-0.4.0/xugrid/conversion.py`

 * *Files identical despite different names*

### Comparing `xugrid-0.3.0/xugrid/core/common.py` & `xugrid-0.4.0/xugrid/core/common.py`

 * *Files identical despite different names*

### Comparing `xugrid-0.3.0/xugrid/core/dataarray_accessor.py` & `xugrid-0.4.0/xugrid/core/dataarray_accessor.py`

 * *Files 2% similar despite different names*

```diff
@@ -132,68 +132,59 @@
         """
         return self._sel(self.obj, self.grid, x, y)
 
     def sel_points(self, x, y):
         """
         Select points in the unstructured grid.
 
+        Out-of-bounds points are ignored. They may be identified via the
+        ``index`` coordinate of the returned selection.
+
         Parameters
         ----------
         x: ndarray of floats with shape ``(n_points,)``
         y: ndarray of floats with shape ``(n_points,)``
 
         Returns
         -------
         points: Union[xr.DataArray, xr.Dataset]
         """
         return self.grid.sel_points(self.obj, x, y)
 
-    def _raster(self, x, y, index) -> xr.DataArray:
-        index = index.ravel()
-        # Cast to float for nodata values (NaN)
-        data = self.obj.isel({self.grid.face_dimension: index}).astype(float).values
-        data[index == -1] = np.nan
-        out = xr.DataArray(
-            data=data.reshape(y.size, x.size),
-            coords={"y": y, "x": x},
-            dims=["y", "x"],
-        )
-        return out
-
-    def rasterize(self, resolution: float):
+    def rasterize(self, resolution: float) -> xr.DataArray:
         """
         Rasterize unstructured grid by sampling.
 
         Parameters
         ----------
         resolution: float
             Spacing in x and y.
 
         Returns
         -------
-        rasterized: Union[xr.DataArray, xr.Dataset]
+        rasterized: xr.DataArray
         """
         x, y, index = self.grid.rasterize(resolution)
         return self._raster(x, y, index)
 
-    def rasterize_like(self, other: Union[xr.DataArray, xr.Dataset]):
+    def rasterize_like(self, other: Union[xr.DataArray, xr.Dataset]) -> xr.DataArray:
         """
         Rasterize unstructured grid by sampling on the x and y coordinates
         of ``other``.
 
         Parameters
         ----------
         resolution: float
             Spacing in x and y.
         other: Union[xr.DataArray, xr.Dataset]
             Object to take x and y coordinates from.
 
         Returns
         -------
-        rasterized: Union[xr.DataArray, xr.Dataset]
+        rasterized: xr.DataArray
         """
         x, y, index = self.grid.rasterize_like(
             x=other["x"].values,
             y=other["y"].values,
         )
         return self._raster(x, y, index)
 
@@ -507,19 +498,24 @@
             options=options,
             tol=tol,
             maxiter=maxiter,
         )
         da_filled = da.copy(data=filled)
         return UgridDataArray(da_filled, grid)
 
-    def to_dataset(self):
+    def to_dataset(self, optional_attributes: bool = False):
         """
         Converts this UgridDataArray or UgridDataset into a standard
         xarray.Dataset.
 
         The UGRID topology information is added as standard data variables.
 
+        Parameters
+        ----------
+        optional_attributes: bool, default: False.
+            Whether to generate the UGRID optional attributes.
+
         Returns
         -------
         dataset: UgridDataset
         """
-        return self.grid.to_dataset(self.obj)
+        return self.grid.to_dataset(self.obj, optional_attributes)
```

### Comparing `xugrid-0.3.0/xugrid/core/dataset_accessor.py` & `xugrid-0.4.0/xugrid/core/dataset_accessor.py`

 * *Files 14% similar despite different names*

```diff
@@ -138,40 +138,93 @@
             result = self._sel(result, grid, x, y)
         return result
 
     def sel_points(self, x, y):
         """
         Select points in the unstructured grid.
 
+        Out-of-bounds points are ignored. They may be identified via the
+        ``index`` coordinate of the returned selection.
+
         Parameters
         ----------
         x: ndarray of floats with shape ``(n_points,)``
         y: ndarray of floats with shape ``(n_points,)``
 
         Returns
         -------
         points: Union[xr.DataArray, xr.Dataset]
         """
         result = self.obj
         for grid in self.grids:
             result = grid.sel_points(result, x, y)
         return result
 
-    def to_dataset(self):
+    def rasterize(self, resolution: float) -> xr.Dataset:
+        """
+        Rasterize all face data on 2D unstructured grids by sampling.
+
+        Parameters
+        ----------
+        resolution: float
+            Spacing in x and y.
+
+        Returns
+        -------
+        rasterized: xr.Dataset
+        """
+        datasets = []
+        for grid in self.grids:
+            xx, yy, index = grid.rasterize(resolution, self.total_bounds)
+            datasets.append(self._raster(xx, yy, index))
+        return xr.merge(datasets)
+
+    def rasterize_like(self, other: Union[xr.DataArray, xr.Dataset]) -> xr.Dataset:
+        """
+        Rasterize unstructured all face data on 2D unstructured grids by
+        sampling on the x and y coordinates of ``other``.
+
+        Parameters
+        ----------
+        resolution: float
+            Spacing in x and y.
+        other: Union[xr.DataArray, xr.Dataset]
+            Object to take x and y coordinates from.
+
+        Returns
+        -------
+        rasterized: xr.Dataset
+        """
+        x = other["x"].values
+        y = other["y"].values
+        datasets = []
+        for grid in self.grids:
+            xx, yy, index = grid.rasterize_like(x, y)
+            datasets.append(self._raster(xx, yy, index))
+        return xr.merge(datasets)
+
+    def to_dataset(self, optional_attributes: bool = False):
         """
         Converts this UgridDataArray or UgridDataset into a standard
         xarray.Dataset.
 
         The UGRID topology information is added as standard data variables.
 
+        Parameters
+        ----------
+        optional_attributes: bool, default: False.
+            Whether to generate the UGRID optional attributes.
+
         Returns
         -------
         dataset: UgridDataset
         """
-        return xr.merge([grid.to_dataset(self.obj) for grid in self.grids])
+        return xr.merge(
+            [grid.to_dataset(self.obj, optional_attributes) for grid in self.grids]
+        )
 
     @property
     def crs(self):
         """
         The Coordinate Reference System (CRS) represented as a ``pyproj.CRS`` object.
 
         Returns None if the CRS is not set.
```

### Comparing `xugrid-0.3.0/xugrid/core/wrap.py` & `xugrid-0.4.0/xugrid/core/wrap.py`

 * *Files identical despite different names*

### Comparing `xugrid-0.3.0/xugrid/data/sample_data.py` & `xugrid-0.4.0/xugrid/data/sample_data.py`

 * *Files identical despite different names*

### Comparing `xugrid-0.3.0/xugrid/data/synthetic.py` & `xugrid-0.4.0/xugrid/data/synthetic.py`

 * *Files identical despite different names*

### Comparing `xugrid-0.3.0/xugrid/meshkernel_utils.py` & `xugrid-0.4.0/xugrid/meshkernel_utils.py`

 * *Files identical despite different names*

### Comparing `xugrid-0.3.0/xugrid/plot/plot.py` & `xugrid-0.4.0/xugrid/plot/plot.py`

 * *Files 2% similar despite different names*

```diff
@@ -518,14 +518,18 @@
     vertices = nodes[faces]
 
     # PolyCollection takes a norm, but not vmin, vmax.
     norm = kwargs.get("norm", None)
     vmin = kwargs.pop("vmin", None)
     vmax = kwargs.pop("vmax", None)
     kwargs["closed"] = False  # Vertices are closing.
+    # Set edgecolor to face by default, since we get a lot of white lines,
+    # especially for larger grids.
+    if "edgecolors" not in kwargs:
+        kwargs["edgecolors"] = "face"
 
     collection = PolyCollection(vertices, **kwargs)
     collection.set_array(da.values.ravel())
     collection._scale_norm(norm, vmin, vmax)
     primitive = ax.add_collection(collection, autolim=False)
 
     xmin, ymin, xmax, ymax = grid.bounds
```

### Comparing `xugrid-0.3.0/xugrid/regrid/overlap_1d.py` & `xugrid-0.4.0/xugrid/regrid/overlap_1d.py`

 * *Files identical despite different names*

### Comparing `xugrid-0.3.0/xugrid/regrid/reduce.py` & `xugrid-0.4.0/xugrid/regrid/reduce.py`

 * *Files identical despite different names*

### Comparing `xugrid-0.3.0/xugrid/regrid/regridder.py` & `xugrid-0.4.0/xugrid/regrid/regridder.py`

 * *Files identical despite different names*

### Comparing `xugrid-0.3.0/xugrid/regrid/structured.py` & `xugrid-0.4.0/xugrid/regrid/structured.py`

 * *Files identical despite different names*

### Comparing `xugrid-0.3.0/xugrid/regrid/unstructured.py` & `xugrid-0.4.0/xugrid/regrid/unstructured.py`

 * *Files identical despite different names*

### Comparing `xugrid-0.3.0/xugrid/regrid/utils.py` & `xugrid-0.4.0/xugrid/regrid/utils.py`

 * *Files identical despite different names*

### Comparing `xugrid-0.3.0/xugrid/regrid/weight_matrix.py` & `xugrid-0.4.0/xugrid/regrid/weight_matrix.py`

 * *Files identical despite different names*

### Comparing `xugrid-0.3.0/xugrid/ugrid/connectivity.py` & `xugrid-0.4.0/xugrid/ugrid/connectivity.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,21 +1,14 @@
 from typing import NamedTuple, Tuple
 
 import numba as nb
 import numpy as np
 from scipy import sparse
 
-from xugrid.constants import (
-    X_EPSILON,
-    BoolArray,
-    FloatArray,
-    IntArray,
-    IntDType,
-    SparseMatrix,
-)
+from xugrid.constants import BoolArray, FloatArray, IntArray, IntDType, SparseMatrix
 
 
 class AdjacencyMatrix(NamedTuple):
     indices: IntArray
     indptr: IntArray
     nnz: int
 
@@ -86,18 +79,25 @@
 
 def to_sparse(
     conn: IntArray, fill_value: int, sort_indices: bool = True
 ) -> sparse.csr_matrix:
     return _to_sparse(conn, fill_value, invert=False, sort_indices=sort_indices)
 
 
-def to_dense(conn: SparseMatrix, fill_value: int) -> IntArray:
+def to_dense(conn: SparseMatrix, fill_value: int, n_columns: int = None) -> IntArray:
     n, _ = conn.shape
     m_per_row = conn.getnnz(axis=1)
     m = m_per_row.max()
+    if n_columns is not None:
+        if n_columns < m:
+            raise ValueError(
+                f"n_columns {n_columns} is too small for the data, requires {m}"
+            )
+        m = n_columns
+
     # Allocate 2D array and create a flat view of the dense connectivity
     dense_conn = np.empty((n, m), dtype=IntDType)
     flat_conn = dense_conn.ravel()
     if (n * m) == conn.nnz:
         # Shortcut if fill_value is not present, when all of same geom. type
         # e.g. all triangles or all quadrangles
         valid = slice(None)  # a[:] equals a[slice(None)]
@@ -193,45 +193,36 @@
     reversed_orientation[replace] = in_reverse
     return reversed_orientation
 
 
 def counterclockwise(
     face_node_connectivity: IntArray, fill_value: int, nodes: FloatArray
 ) -> IntArray:
-    # In principle, we need only compute the cross product of the first three
-    # vertices to determine whether a polygon is ordered clockwise (cw) or ccw.
-    # However, this fails if there are hanging nodes amongst the first few.
-    # First, we try with just first triangles.
-    p = nodes[face_node_connectivity[:, :3]]
+    closed, _ = close_polygons(face_node_connectivity, fill_value)
+    p = nodes[closed]
     dxy = np.diff(p, axis=1)
-    normal = np.cross(dxy[:, 0], dxy[:, 1])
-    reverse = normal < 0
-
-    # Check whether there are any hanging nodes
-    hanging = np.abs(normal) < X_EPSILON
-    if hanging.any():
-        # For these rows, go through the entire polygon
-        n = hanging.sum()
-        m = face_node_connectivity.shape[1]
-        closed, _ = close_polygons(face_node_connectivity[hanging], fill_value)
-        p = nodes[closed]
-        dxy = np.diff(p, axis=1)
-        normal = np.empty((n, m))
-        for i in range(m - 1):
-            normal[:, i] = np.cross(dxy[:, i], dxy[:, i + 1])
-        reverse[hanging] = normal.sum(axis=1) < 0
-
+    reverse = (np.cross(dxy[:, :-1], dxy[:, 1:])).sum(axis=1) < 0
     ccw = face_node_connectivity.copy()
     if reverse.any():
         ccw[reverse] = reverse_orientation(face_node_connectivity[reverse], fill_value)
     return ccw
 
 
 # Derived connectivities
 # ----------------------
+def boundary_node_connectivity(
+    edge_face_connectivity: IntArray,
+    fill_value: int,
+    edge_node_connectivity: IntArray,
+) -> IntArray:
+    """Is a subset of the edge_node_connectivity"""
+    is_boundary = (edge_face_connectivity == fill_value).any(axis=1)
+    return edge_node_connectivity[is_boundary]
+
+
 def edge_connectivity(
     face_node_connectivity: IntArray,
     fill_value: int,
     edge_node_connectivity=None,
 ) -> Tuple[IntArray, IntArray]:
     """Derive new edge_node_connectivity and face_edge_connectivity."""
     prior = edge_node_connectivity
@@ -249,16 +240,18 @@
     # Now find the unique rows == unique edges
     edge_node_connectivity.sort(axis=1)
     edge_node_connectivity, inverse_indices = np.unique(
         ar=edge_node_connectivity, return_inverse=True, axis=0
     )
 
     if prior is not None:  # prior edge_node_connectivity exists
-        # argsort doesn't work on rows!
-        _, index = np.unique(np.sort(prior, axis=1), axis=0, return_index=True)
+        unique, index = np.unique(np.sort(prior, axis=1), axis=0, return_index=True)
+        # Check whether everything looks okay:
+        if not np.array_equal(unique, edge_node_connectivity):
+            raise ValueError("Invalid edge_node_connectivity")
         inverse_indices = index[inverse_indices]
         edge_node_connectivity = prior
 
     # Create face_edge_connectivity
     face_edge_connectivity = np.full((n, m), fill_value, dtype=np.int64)
     isnode = ~isfill[:, :-1]
     face_edge_connectivity[isnode] = inverse_indices
@@ -334,18 +327,16 @@
 ) -> FloatArray:
     n_face, n_max_node = face_node_connectivity.shape
     nodes = np.column_stack([node_x, node_y])
     # Check if it's fully triangular
     if n_max_node == 3:
         # Since it's triangular, computing the average of the vertices suffices
         coordinates = nodes[face_node_connectivity]
-        coordinates[face_node_connectivity == fill_value] = np.nan
         return np.nanmean(coordinates, axis=1)
     else:
-        # TODO: convex might be simpler
         # This is mathematically equivalent to triangulating, computing triangle centroids
         # and computing the area weighted average of those centroids
         centroid_coordinates = np.empty((n_face, 2), dtype=np.float64)
         closed, _ = close_polygons(face_node_connectivity, fill_value)
         coordinates = nodes[closed]
         # Shift coordinates to avoid precision loss
         a = coordinates[:, :-1]
@@ -354,14 +345,52 @@
         determinant = np.cross(a, b)
         area_weight = 1.0 / (3.0 * determinant.sum(axis=1))
         centroid_coordinates[:, 0] = area_weight * (c[..., 0] * determinant).sum(axis=1)
         centroid_coordinates[:, 1] = area_weight * (c[..., 1] * determinant).sum(axis=1)
         return centroid_coordinates
 
 
+@nb.njit(cache=True, parallel=True)
+def _circumcenters_triangle(xxx: FloatArray, yyy: FloatArray):
+    """Numba should nicely fuse these operations."""
+    a_x, b_x, c_x = xxx
+    a_y, b_y, c_y = yyy
+    D_inv = 0.5 / (
+        (a_y * c_x + b_y * a_x - b_y * c_x - a_y * b_x - c_y * a_x + c_y * b_x)
+    )
+    x = ((a_x - c_x) * (a_x + c_x) + (a_y - c_y) * (a_y + c_y)) * (b_y - c_y) - (
+        (b_x - c_x) * (b_x + c_x) + (b_y - c_y) * (b_y + c_y)
+    ) * (a_y - c_y)
+    y = ((b_x - c_x) * (b_x + c_x) + (b_y - c_y) * (b_y + c_y)) * (a_x - c_x) - (
+        (a_x - c_x) * (a_x + c_x) + (a_y - c_y) * (a_y + c_y)
+    ) * (b_x - c_x)
+    return D_inv * x, D_inv * y
+
+
+def circumcenters(
+    face_node_connectivity: IntArray,
+    fill_value: int,
+    node_x: FloatArray,
+    node_y: FloatArray,
+) -> FloatArray:
+    # TODO: Skyum or Welzl implementation for polygons -- although it's
+    # practical use is dubious?
+    n_max_node = face_node_connectivity.shape[1]
+    # Check if it's fully triangular
+    if n_max_node == 3:
+        xxx = node_x[face_node_connectivity.T]
+        yyy = node_y[face_node_connectivity.T]
+        x, y = _circumcenters_triangle(xxx, yyy)
+    else:
+        raise NotImplementedError(
+            "Circumcenters are only supported for triangular grids"
+        )
+    return np.column_stack((x, y))
+
+
 def _triangulate(i: IntArray, j: IntArray, n_triangle_per_row: IntArray) -> IntArray:
     n_triangle = n_triangle_per_row.sum()
     n_face = len(i)
     index_first = np.argwhere(np.diff(i, prepend=-1) != 0)
     index_second = index_first + 1
     index_last = np.argwhere(np.diff(i, append=-1) != 0)
```

### Comparing `xugrid-0.3.0/xugrid/ugrid/conventions.py` & `xugrid-0.4.0/xugrid/ugrid/conventions.py`

 * *Files 4% similar despite different names*

```diff
@@ -120,24 +120,29 @@
         "_FillValue": -1,
     },
     "face_edge_connectivity": {
         "cf_role": "face_edge_connectivity",
         "start_index": 0,
         "_FillValue": -1,
     },
-    # "face_face_connectivity": {
-    #    "cf_role": "face_face_connectivity",
-    #    "start_index": 0,
-    #    "_FillValue": -1,
-    # },
+    "face_face_connectivity": {
+        "cf_role": "face_face_connectivity",
+        "start_index": 0,
+        "_FillValue": -1,
+    },
     "edge_face_connectivity": {
         "cf_role": "edge_face_connectivity",
         "start_index": 0,
         "_FillValue": -1,
     },
+    "boundary_node_connectivity": {
+        "cf_role": "boundary_node_connectivity",
+        "start_index": 0,
+        "_FillValue": -1,
+    },
 }
 
 
 def default_topology_attrs(name: str, topology_dimension: int):
     if topology_dimension == 1:
         return {
             "cf_role": "mesh_topology",
@@ -154,16 +159,21 @@
             "cf_role": "mesh_topology",
             "long_name": "Topology data of 2D mesh",
             "topology_dimension": 2,
             "node_dimension": f"{name}_nNodes",
             "edge_dimension": f"{name}_nEdges",
             "face_dimension": f"{name}_nFaces",
             "max_face_nodes_dimension": f"{name}_nMax_face_nodes",
+            "boundary_edge_dimension": f"{name}_nBoundary_edges",
             "edge_node_connectivity": f"{name}_edge_nodes",
             "face_node_connectivity": f"{name}_face_nodes",
+            "face_edge_connectivity": f"{name}_face_edges",
+            "edge_face_connectivity": f"{name}_edge_faces",
+            "boundary_node_connectivity": f"{name}_boundary_nodes",
+            "face_face_connectivity": f"{name}_face_faces",
             "node_coordinates": f"{name}_node_x {name}_node_y",
             "edge_coordinates": f"{name}_edge_x {name}_edge_y",
             "face_coordinates": f"{name}_face_x {name}_face_y",
         }
     else:
         raise ValueError(
             f"topology_dimensions should be 1 or 2, received {topology_dimension}"
```

### Comparing `xugrid-0.3.0/xugrid/ugrid/interpolate.py` & `xugrid-0.4.0/xugrid/ugrid/interpolate.py`

 * *Files identical despite different names*

### Comparing `xugrid-0.3.0/xugrid/ugrid/partitioning.py` & `xugrid-0.4.0/xugrid/ugrid/partitioning.py`

 * *Files identical despite different names*

### Comparing `xugrid-0.3.0/xugrid/ugrid/snapping.py` & `xugrid-0.4.0/xugrid/ugrid/snapping.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """
 Snapes nodes at an arbitrary distance together.
 """
-from typing import Tuple, Union
+from typing import Tuple, TypeVar, Union
 
 import numba as nb
 import numpy as np
 import pandas as pd
 import xarray as xr
 from numba_celltree import CellTree2d
 from scipy import sparse
@@ -24,16 +24,20 @@
 )
 from xugrid.ugrid import connectivity
 from xugrid.ugrid.connectivity import AdjacencyMatrix
 from xugrid.ugrid.ugrid2d import Ugrid2d
 
 try:
     import geopandas as gpd
+
+    GeoDataFrameType = gpd.GeoDataFrame
 except ImportError:
     gpd = MissingOptionalModule("geopandas")
+    # https://stackoverflow.com/questions/61384752/how-to-type-hint-with-an-optional-import
+    GeoDataFrameType = TypeVar("GeoDataFrameType")  # avoid ImportError in typehints
 
 try:
     import shapely
 except ImportError:
     shapely = MissingOptionalModule("shapely")
 
 
@@ -211,15 +215,15 @@
 def left_of(a: Point, p: Point, U: Vector) -> bool:
     # Whether point a is left of vector U
     # U: p -> q direction vector
     # TODO: maybe add epsilon for floating point
     return U.x * (a.y - p.y) > U.y * (a.x - p.x)
 
 
-def coerce_geometry(lines: gpd.GeoDataFrame) -> LineArray:
+def coerce_geometry(lines: GeoDataFrameType) -> LineArray:
     geometry = lines.geometry.values
     geom_type = shapely.get_type_id(geometry)
     if not (geom_type == 1).all():
         raise ValueError("Geometry should contain only LineStrings")
     return geometry
 
 
@@ -301,15 +305,15 @@
 
     edges = edges[max_edge_index]
     line_index = line_index[max_edge_index]
     return edges, line_index
 
 
 def _create_output_dataset(
-    lines: gpd.GeoDataFrame,
+    lines: GeoDataFrameType,
     topology: "xu.Ugrid2d",
     edges: IntArray,
     line_index: IntArray,
 ) -> xu.UgridDataset:
     uds = xu.UgridDataset(grids=[topology])
     data = np.full(topology.n_edge, np.nan)
     data[edges] = line_index
@@ -340,18 +344,18 @@
     geometry = shapely.linestrings(edge_vertices)
     return gpd.GeoDataFrame(
         lines.drop(columns="geometry").iloc[line_index], geometry=geometry
     )
 
 
 def snap_to_grid(
-    lines: gpd.GeoDataFrame,
+    lines: GeoDataFrameType,
     grid: Union[xr.DataArray, xu.UgridDataArray],
     max_snap_distance: float,
-) -> Tuple[IntArray, Union[pd.DataFrame, gpd.GeoDataFrame]]:
+) -> Tuple[IntArray, Union[pd.DataFrame, GeoDataFrameType]]:
     """
     Snap a collection of lines to a grid.
 
     A line is included and snapped to a grid edge when the line separates
     the centroid of the cell with the centroid of the edge.
 
     When a line in a cell is snapped to an edge that is **not** shared with
```

### Comparing `xugrid-0.3.0/xugrid/ugrid/ugrid1d.py` & `xugrid-0.4.0/xugrid/ugrid/ugrid1d.py`

 * *Files 0% similar despite different names*

```diff
@@ -204,15 +204,17 @@
             fill_value=-1,
             edge_node_connectivity=mesh.edge_nodes.reshape((-1, 2)),
             name=name,
             projected=projected,
             crs=crs,
         )
 
-    def to_dataset(self, other: xr.Dataset = None) -> xr.Dataset:
+    def to_dataset(
+        self, other: xr.Dataset = None, optional_attributes: bool = False
+    ) -> xr.Dataset:
         node_x = self._indexes["node_x"]
         node_y = self._indexes["node_y"]
         edge_nodes = self._attrs["edge_node_connectivity"]
         edge_nodes_attrs = conventions.DEFAULT_ATTRS["edge_node_connectivity"]
 
         data_vars = {
             self.name: 0,
@@ -226,14 +228,16 @@
 
         if self._dataset:
             dataset.update(self._dataset)
         if other is not None:
             dataset = dataset.merge(other)
         if node_x not in dataset or node_y not in dataset:
             dataset = self.assign_node_coords(dataset)
+        if optional_attributes:
+            dataset = self.assign_edge_coords(dataset)
 
         dataset[self.name].attrs = self._filtered_attrs(dataset)
         return dataset
 
     @property
     def topology_dimension(self):
         """Highest dimensionality of the geometric elements: 1"""
```

### Comparing `xugrid-0.3.0/xugrid/ugrid/ugrid2d.py` & `xugrid-0.4.0/xugrid/ugrid/ugrid2d.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from itertools import chain
-from typing import Any, Dict, Tuple, Union
+from typing import Any, Dict, Optional, Tuple, Union
 
 import numpy as np
 import pandas as pd
 import xarray as xr
 from numba_celltree import CellTree2d
 from scipy.sparse import coo_matrix, csr_matrix
 from scipy.sparse.csgraph import reverse_cuthill_mckee
@@ -121,29 +121,31 @@
         self._meshkernel = None
         # Celltree
         self._celltree = None
         # Area
         self._area = None
         # Centroids
         self._centroids = None
+        self._circumcenters = None
         # Bounds
         self._xmin = None
         self._xmax = None
         self._ymin = None
         self._ymax = None
         # Edges
         self._edge_x = None
         self._edge_y = None
         # Connectivity
-        self._edge_node_connectivity = edge_node_connectivity
+        self.edge_node_connectivity = edge_node_connectivity
         self._edge_face_connectivity = None
         self._node_edge_connectivity = None
         self._node_face_connectivity = None
         self._face_edge_connectivity = None
         self._face_face_connectivity = None
+        self._boundary_node_connectivity = None
         # Derived topology
         self._triangulation = None
         self._voronoi_topology = None
         self._centroid_triangulation = None
         # crs
         if crs is None:
             self.crs = None
@@ -159,14 +161,15 @@
         self._meshkernel = None
         # Celltree
         self._celltree = None
         # Area
         self._area = None
         # Centroids
         self._centroids = None
+        self._circumcenters = None
         # Bounds
         self._xmin = None
         self._xmax = None
         self._ymin = None
         self._ymax = None
         # Edges
         self._edge_x = None
@@ -287,46 +290,85 @@
             edge_node_connectivity=edge_node_connectivity,
             dataset=ds[ugrid_vars],
             indexes=indexes,
             projected=projected,
             crs=None,
         )
 
-    def to_dataset(self, other: xr.Dataset = None) -> xr.Dataset:
+    def _get_name_and_attrs(self, name: str):
+        key = f"{name}_connectivity"
+        attrs = conventions.DEFAULT_ATTRS[key]
+        if "_FillValue" in attrs:
+            attrs["_FillValue"] = self.fill_value
+        return self._attrs[key], attrs
+
+    def to_dataset(
+        self, other: xr.Dataset = None, optional_attributes: bool = False
+    ) -> xr.Dataset:
         node_x = self._indexes["node_x"]
         node_y = self._indexes["node_y"]
-        face_nodes = self._attrs["face_node_connectivity"]
-        face_nodes_attrs = conventions.DEFAULT_ATTRS["face_node_connectivity"]
+        face_nodes, face_nodes_attrs = self._get_name_and_attrs("face_node")
         nmax_node_dim = self._attrs["max_face_nodes_dimension"]
-        edge_nodes = self._attrs["edge_node_connectivity"]
-        edge_nodes_attrs = conventions.DEFAULT_ATTRS["edge_node_connectivity"]
+        edge_nodes, edge_nodes_attrs = self._get_name_and_attrs("edge_node")
 
         data_vars = {
             self.name: 0,
             face_nodes: xr.DataArray(
                 data=self.face_node_connectivity,
                 attrs=face_nodes_attrs,
                 dims=(self.face_dimension, nmax_node_dim),
             ),
         }
-        if self.edge_node_connectivity is not None:
+        if self.edge_node_connectivity is not None or optional_attributes:
             data_vars[edge_nodes] = xr.DataArray(
                 data=self.edge_node_connectivity,
                 attrs=edge_nodes_attrs,
                 dims=(self.edge_dimension, "two"),
             )
+        if optional_attributes:
+            face_edges, face_edges_attrs = self._get_name_and_attrs("face_edge")
+            face_faces, face_faces_attrs = self._get_name_and_attrs("face_face")
+            edge_faces, edge_faces_attrs = self._get_name_and_attrs("edge_face")
+            bound_nodes, bound_nodes_attrs = self._get_name_and_attrs("boundary_node")
+            fill_value = self.fill_value
+            boundary_edge_dim = self._attrs["boundary_edge_dimension"]
+
+            data_vars[face_edges] = xr.DataArray(
+                data=self.face_edge_connectivity,
+                attrs=face_edges_attrs,
+                dims=(self.face_dimension, nmax_node_dim),
+            )
+            data_vars[face_faces] = xr.DataArray(
+                data=connectivity.to_dense(
+                    self.face_face_connectivity, fill_value, self.n_max_node_per_face
+                ),
+                attrs=face_faces_attrs,
+                dims=(self.face_dimension, nmax_node_dim),
+            )
+            data_vars[edge_faces] = xr.DataArray(
+                data=self.edge_face_connectivity,
+                attrs=edge_faces_attrs,
+                dims=(self.edge_dimension, "two"),
+            )
+            data_vars[bound_nodes] = xr.DataArray(
+                data=self.boundary_node_connectivity,
+                attrs=bound_nodes_attrs,
+                dims=(boundary_edge_dim, "two"),
+            )
 
         dataset = xr.Dataset(data_vars, attrs={"Conventions": "CF-1.8 UGRID-1.0"})
-
         if self._dataset:
             dataset.update(self._dataset)
         if other is not None:
             dataset = dataset.merge(other)
         if node_x not in dataset or node_y not in dataset:
             dataset = self.assign_node_coords(dataset)
+        if optional_attributes:
+            dataset = self.assign_face_coords(dataset)
+            dataset = self.assign_edge_coords(dataset)
 
         dataset[self.name].attrs = self._filtered_attrs(dataset)
         return dataset
 
     # These are all optional/derived UGRID attributes. They are not computed by
     # default, only when called upon.
     @property
@@ -392,33 +434,57 @@
         -------
         connectivity: ndarray of integers with shape ``(n_edge, 2)``.
         """
         if self._edge_node_connectivity is None:
             self._edge_connectivity()
         return self._edge_node_connectivity
 
+    @edge_node_connectivity.setter
+    def edge_node_connectivity(self, value):
+        if value is not None:
+            associated = np.isin(value, self.face_node_connectivity)
+            associated = associated[:, 0] & associated[:, 1]
+            if not associated.all():
+                raise ValueError(
+                    "edge_node_connectivity is invalid, the following edges are not "
+                    f"associated with any face: {np.flatnonzero(~associated)}"
+                )
+        self._edge_node_connectivity = value
+
     @property
     def face_edge_connectivity(self) -> csr_matrix:
         """
         Face to edge connectivity.
 
         Returns
         -------
         connectivity: csr_matrix
         """
         if self._face_edge_connectivity is None:
             self._edge_connectivity()
-            # if self._edge_node_connectivity is None:
-            #    self._edge_connectivity()
-            # else:
-            #    raise NotImplementedError
-        #                self._face_edge_connectivity =
         return self._face_edge_connectivity
 
     @property
+    def boundary_node_connectivity(self) -> IntArray:
+        """
+        Boundary node connectivity
+
+        Returns:
+        --------
+        connectivity: ndarray of integers with shape ``(n_boundary_edge, 2)``
+        """
+        if self._boundary_node_connectivity is None:
+            self._boundary_node_connectivity = connectivity.boundary_node_connectivity(
+                self.edge_face_connectivity,
+                self.fill_value,
+                self.edge_node_connectivity,
+            )
+        return self._boundary_node_connectivity
+
+    @property
     def centroids(self) -> FloatArray:
         """
         Centroid (x, y) of every face.
 
         Returns
         -------
         centroids: ndarray of floats with shape ``(n_face, 2)``
@@ -429,14 +495,25 @@
                 self.fill_value,
                 self.node_x,
                 self.node_y,
             )
         return self._centroids
 
     @property
+    def circumcenters(self):
+        if self._circumcenters is None:
+            self._circumcenters = connectivity.circumcenters(
+                self.face_node_connectivity,
+                self.fill_value,
+                self.node_x,
+                self.node_y,
+            )
+        return self._circumcenters
+
+    @property
     def area(self) -> FloatArray:
         if self._area is None:
             self._area = connectivity.area(
                 self.face_node_connectivity,
                 self.fill_value,
                 self.node_x,
                 self.node_y,
@@ -834,33 +911,41 @@
         face_index: 1d array of integers with shape ``(nrow * ncol,)``
         """
         yy, xx = np.meshgrid(y, x, indexing="ij")
         nodes = np.column_stack([xx.ravel(), yy.ravel()])
         index = self.celltree.locate_points(nodes).reshape((y.size, x.size))
         return x, y, index
 
-    def rasterize(self, resolution: float) -> Tuple[FloatArray, FloatArray, IntArray]:
+    def rasterize(
+        self,
+        resolution: float,
+        bounds: Optional[Tuple[float, float, float, float]] = None,
+    ) -> Tuple[FloatArray, FloatArray, IntArray]:
         """
         Rasterize unstructured grid by sampling.
 
         x and y coordinates are generated from the bounds of the UGRID2D
         topology and the provided resolution.
 
         Parameters
         ----------
         resolution: float
             Spacing in x and y.
+        bounds: tuple of four floats, optional
+            xmin, ymin, xmax, ymax
 
         Returns
         -------
         x: 1d array of floats with shape ``(ncol,)``
         y: 1d array of floats with shape ``(nrow,)``
         face_index: 1d array of integers with shape ``(nrow * ncol,)``
         """
-        xmin, ymin, xmax, ymax = self.bounds
+        if bounds is None:
+            bounds = self.bounds
+        xmin, ymin, xmax, ymax = bounds
         d = abs(resolution)
         xmin = np.floor(xmin / d) * d
         xmax = np.ceil(xmax / d) * d
         ymin = np.floor(ymin / d) * d
         ymax = np.ceil(ymax / d) * d
         x = np.arange(xmin + 0.5 * d, xmax, d)
         y = np.arange(ymax - 0.5 * d, ymin, -d)
@@ -1104,14 +1189,17 @@
         coords, index = section_coordinates(edges, xy, self.face_dimension, index)
         return obj.isel({self.face_dimension: index}).assign_coords(coords)
 
     def sel_points(self, obj, x: FloatArray, y: FloatArray):
         """
         Select points in the unstructured grid.
 
+        Out-of-bounds points are ignored. They may be identified via the
+        ``index`` coordinate of the returned selection.
+
         Parameters
         ----------
         x: 1d array of floats with shape ``(n_points,)``
         y: 1d array of floats with shape ``(n_points,)``
         obj: xr.DataArray or xr.Dataset
 
         Returns
@@ -1126,14 +1214,15 @@
             raise ValueError("x and y must be 1d")
         dim = self.face_dimension
         xy = np.column_stack([x, y])
         index = self.locate_points(xy)
         valid = index != -1
         index = index[valid]
         coords = {
+            "index": (dim, np.arange(len(valid))[valid]),
             "x": (dim, xy[valid, 0]),
             "y": (dim, xy[valid, 1]),
         }
         return obj.isel({dim: index}).assign_coords(coords)
 
     def sel(self, obj, x=None, y=None):
         """
@@ -1226,51 +1315,73 @@
         triangles: Ugrid2d
         """
         triangles, _ = connectivity.triangulate(
             self.face_node_connectivity, self.fill_value
         )
         return Ugrid2d(self.node_x, self.node_y, self.fill_value, triangles)
 
-    def tesselate_centroidal_voronoi(self, add_exterior=True, add_vertices=True):
-        """
-        Create a centroidal Voronoi tesselation of this UGRID2D topology.
-
-        Such a tesselation is not guaranteed to produce convex cells. To ensure
-        convexity, set ``add_vertices=False`` -- this will result in a
-        different exterior, however.
-
-        Parameters
-        ----------
-        add_exterior: bool, default: True
-        add_vertices: bool, default: True
-
-        Returns
-        -------
-        tesselation: Ugrid2d
-        """
+    def _tesselate_voronoi(self, centroids, add_exterior, add_vertices):
         if add_exterior:
             edge_face_connectivity = self.edge_face_connectivity
             edge_node_connectivity = self.edge_node_connectivity
         else:
             edge_face_connectivity = None
             edge_node_connectivity = None
 
         vertices, faces, _ = voronoi_topology(
             self.node_face_connectivity,
             self.node_coordinates,
-            self.centroids,
+            centroids,
             edge_face_connectivity,
             edge_node_connectivity,
             self.fill_value,
             add_exterior,
             add_vertices,
         )
         faces = connectivity.to_dense(faces, self.fill_value)
         return Ugrid2d(vertices[:, 0], vertices[:, 1], self.fill_value, faces)
 
+    def tesselate_centroidal_voronoi(self, add_exterior=True, add_vertices=True):
+        """
+        Create a centroidal Voronoi tesselation of this UGRID2D topology.
+
+        Such a tesselation is not guaranteed to produce convex cells. To ensure
+        convexity, set ``add_vertices=False`` -- this will result in a
+        different exterior, however.
+
+        Parameters
+        ----------
+        add_exterior: bool, default: True
+        add_vertices: bool, default: True
+
+        Returns
+        -------
+        tesselation: Ugrid2d
+        """
+        return self._tesselate_voronoi(self.centroids, add_exterior, add_vertices)
+
+    def tesselate_circumcenter_voronoi(self, add_exterior=True, add_vertices=True):
+        """
+        Create a circumcenter Voronoi tesselation of this UGRID2D topology.
+
+        Such a tesselation is not guaranteed to produce convex cells. To ensure
+        convexity, set ``add_vertices=False`` -- this will result in a
+        different exterior, however.
+
+        Parameters
+        ----------
+        add_exterior: bool, default: True
+        add_vertices: bool, default: True
+
+        Returns
+        -------
+        tesselation: Ugrid2d
+        """
+        return self._tesselate_voronoi(self.circumcenters, add_exterior, add_vertices)
+
     def reverse_cuthill_mckee(self, dimension=None):
         """
         Reduces bandwith of the connectivity matrix.
 
         Wraps :py:func:`scipy.sparse.csgraph.reverse_cuthill_mckee`.
 
         Returns
```

### Comparing `xugrid-0.3.0/xugrid/ugrid/ugridbase.py` & `xugrid-0.4.0/xugrid/ugrid/ugridbase.py`

 * *Files 1% similar despite different names*

```diff
@@ -210,14 +210,18 @@
         return True
 
     def copy(self):
         """Creates deepcopy"""
         return copy.deepcopy(self)
 
     @property
+    def attrs(self):
+        return self._attrs
+
+    @property
     def node_dimension(self):
         """Name of node dimension"""
         return self._attrs["node_dimension"]
 
     @property
     def edge_dimension(self):
         """Name of edge dimension"""
```

### Comparing `xugrid-0.3.0/xugrid/ugrid/voronoi.py` & `xugrid-0.4.0/xugrid/ugrid/voronoi.py`

 * *Files 5% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 """
 from typing import Tuple
 
 import numpy as np
 import pandas as pd
 from scipy import sparse
 
-from xugrid.constants import FloatArray, IntArray
+from xugrid.constants import X_EPSILON, FloatArray, IntArray
 from xugrid.ugrid.connectivity import renumber
 
 
 def dot_product2d(U: FloatArray, V: FloatArray):
     return U[:, 1] * V[:, 1] + U[:, 0] * V[:, 0]
 
 
@@ -97,38 +97,45 @@
     a = edge_vertices[:, 0, :]
     b = edge_vertices[:, 1, :]
     V = b - a
     U = centroid_vertices - a
     # np.dot(U, V) doesn't do the desired thing here
     projected_vertices = a + ((dot_product2d(U, V) / dot_product2d(V, V)) * V.T).T
 
-    # Create the numbering pointing to these new vertices
-    n_new = len(projected_vertices)
+    # Create the numbering pointing to these new vertices.
+    # Discard vertices that overlap with e.g. circumcenters.
+    keep = np.linalg.norm(projected_vertices - centroid_vertices, axis=1) > (
+        X_EPSILON * X_EPSILON
+    )
+    face_i = face_i[keep]
+    vertices_keep = projected_vertices[keep]
     n_centroid = len(centroids)
-    i = exterior_nodes.ravel()
-    n = n_centroid + n_new
-    j = np.repeat(np.arange(n_centroid, n), 2)
+    i_keep = exterior_nodes[keep].ravel()
+    n = n_centroid + len(vertices_keep)
+    j_keep = np.repeat(np.arange(n_centroid, n), 2)
     n_interpolated = 0
 
     # We add a substitution value for the actual vertex
     if add_vertices:
+        n_new = len(projected_vertices)
+        i = exterior_nodes.ravel()
         order = np.argsort(i)
         jj = np.repeat(np.arange(n_new), 2)[order]
         to_interpolate = projected_vertices[jj]
         interpolated = 0.5 * (to_interpolate[::2] + to_interpolate[1::2])
         n_interpolated = len(interpolated)
-        i = np.concatenate([i, i[order][::2]])
-        j = np.concatenate([j, np.arange(n, n + n_interpolated)])
-        projected_vertices = np.concatenate([projected_vertices, interpolated])
+        i_keep = np.concatenate([i_keep, i[order][::2]])
+        j_keep = np.concatenate([j_keep, np.arange(n, n + n_interpolated)])
+        vertices_keep = np.concatenate([vertices_keep, interpolated])
         # Create face index: the face of the original mesh associated with every
         # voronoi vertex is a centroid. The exterior vertices are an exception to
         # this: these are associated with two faces. So we set a value of -1 here.
         face_i = np.concatenate([face_i, np.full(n_interpolated, -1)])
 
-    return i, j, projected_vertices, face_i, n_interpolated
+    return i_keep, j_keep, vertices_keep, face_i, n_interpolated
 
 
 def exterior_topology(
     edge_face_connectivity: IntArray,
     edge_node_connectivity: IntArray,
     node_face_connectivity: sparse.csr_matrix,
     fill_value: int,
@@ -326,16 +333,16 @@
             centroids,
             add_vertices,
         )
         offset = node_i.max() + 1 if len(node_i > 0) else 0
         i = np.concatenate([node_i, exterior_i + offset])
         j = np.concatenate([j, exterior_j])
     else:
+        vor_vertices = centroids[np.unique(face_i)]
         face_i = np.arange(face_i.max() + 1)
-        vor_vertices = centroids.copy()
         i = node_i
         j = renumber(j)
 
     i = renumber(i)
     coo_content = (j, (i, j))
     face_node_connectivity = sparse.coo_matrix(coo_content)
     return vor_vertices, face_node_connectivity, face_i
```

### Comparing `xugrid-0.3.0/xugrid.egg-info/PKG-INFO` & `xugrid-0.4.0/xugrid.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xugrid
-Version: 0.3.0
+Version: 0.4.0
 Summary: Xarray extension for unstructured grids
 Maintainer-email: Huite Bootsma <huite.bootsma@deltares.nl>
 License: MIT
 Project-URL: Home, https://github.com/deltares/xugrid
 Project-URL: Code, https://github.com/deltares/xugrid
 Project-URL: Issues, https://github.com/deltares/xugrid/issues
 Keywords: mesh,ugrid,unstructured grid,xarray
```

### Comparing `xugrid-0.3.0/xugrid.egg-info/SOURCES.txt` & `xugrid-0.4.0/xugrid.egg-info/SOURCES.txt`

 * *Files identical despite different names*

