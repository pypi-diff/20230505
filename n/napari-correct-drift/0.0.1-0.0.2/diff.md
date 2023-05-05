# Comparing `tmp/napari-correct-drift-0.0.1.tar.gz` & `tmp/napari-correct-drift-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "napari-correct-drift-0.0.1.tar", last modified: Wed Apr 26 15:25:04 2023, max compression
+gzip compressed data, was "napari-correct-drift-0.0.2.tar", last modified: Fri May  5 09:48:34 2023, max compression
```

## Comparing `napari-correct-drift-0.0.1.tar` & `napari-correct-drift-0.0.2.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 15:25:04.483776 napari-correct-drift-0.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1491 2023-04-26 15:24:44.000000 napari-correct-drift-0.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      117 2023-04-26 15:24:44.000000 napari-correct-drift-0.0.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3597 2023-04-26 15:25:04.483776 napari-correct-drift-0.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2292 2023-04-26 15:24:44.000000 napari-correct-drift-0.0.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      180 2023-04-26 15:24:44.000000 napari-correct-drift-0.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1738 2023-04-26 15:25:04.483776 napari-correct-drift-0.0.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 15:25:04.479776 napari-correct-drift-0.0.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 15:25:04.483776 napari-correct-drift-0.0.1/src/napari_correct_drift/
--rw-r--r--   0 runner    (1001) docker     (123)      375 2023-04-26 15:24:44.000000 napari-correct-drift-0.0.1/src/napari_correct_drift/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18159 2023-04-26 15:24:44.000000 napari-correct-drift-0.0.1/src/napari_correct_drift/_core.py
--rw-r--r--   0 runner    (1001) docker     (123)     3529 2023-04-26 15:24:44.000000 napari-correct-drift-0.0.1/src/napari_correct_drift/_sample_data.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 15:25:04.483776 napari-correct-drift-0.0.1/src/napari_correct_drift/_tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 15:24:44.000000 napari-correct-drift-0.0.1/src/napari_correct_drift/_tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6896 2023-04-26 15:24:44.000000 napari-correct-drift-0.0.1/src/napari_correct_drift/_tests/test_core.py
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-04-26 15:24:44.000000 napari-correct-drift-0.0.1/src/napari_correct_drift/_tests/test_sample_data.py
--rw-r--r--   0 runner    (1001) docker     (123)      845 2023-04-26 15:24:44.000000 napari-correct-drift-0.0.1/src/napari_correct_drift/_tests/test_widget.py
--rw-r--r--   0 runner    (1001) docker     (123)    18352 2023-04-26 15:24:44.000000 napari-correct-drift-0.0.1/src/napari_correct_drift/_widget.py
--rw-r--r--   0 runner    (1001) docker     (123)     1133 2023-04-26 15:24:44.000000 napari-correct-drift-0.0.1/src/napari_correct_drift/napari.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 15:25:04.483776 napari-correct-drift-0.0.1/src/napari_correct_drift.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3597 2023-04-26 15:25:04.000000 napari-correct-drift-0.0.1/src/napari_correct_drift.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      717 2023-04-26 15:25:04.000000 napari-correct-drift-0.0.1/src/napari_correct_drift.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-26 15:25:04.000000 napari-correct-drift-0.0.1/src/napari_correct_drift.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-04-26 15:25:04.000000 napari-correct-drift-0.0.1/src/napari_correct_drift.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-04-26 15:25:04.000000 napari-correct-drift-0.0.1/src/napari_correct_drift.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-04-26 15:25:04.000000 napari-correct-drift-0.0.1/src/napari_correct_drift.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 09:48:34.246965 napari-correct-drift-0.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1491 2023-05-05 09:48:07.000000 napari-correct-drift-0.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      117 2023-05-05 09:48:07.000000 napari-correct-drift-0.0.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3843 2023-05-05 09:48:34.246965 napari-correct-drift-0.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2538 2023-05-05 09:48:07.000000 napari-correct-drift-0.0.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      180 2023-05-05 09:48:07.000000 napari-correct-drift-0.0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1738 2023-05-05 09:48:34.246965 napari-correct-drift-0.0.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 09:48:34.242965 napari-correct-drift-0.0.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 09:48:34.242965 napari-correct-drift-0.0.2/src/napari_correct_drift/
+-rw-r--r--   0 runner    (1001) docker     (123)      375 2023-05-05 09:48:07.000000 napari-correct-drift-0.0.2/src/napari_correct_drift/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18849 2023-05-05 09:48:07.000000 napari-correct-drift-0.0.2/src/napari_correct_drift/_core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3529 2023-05-05 09:48:07.000000 napari-correct-drift-0.0.2/src/napari_correct_drift/_sample_data.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 09:48:34.246965 napari-correct-drift-0.0.2/src/napari_correct_drift/_tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 09:48:07.000000 napari-correct-drift-0.0.2/src/napari_correct_drift/_tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6896 2023-05-05 09:48:07.000000 napari-correct-drift-0.0.2/src/napari_correct_drift/_tests/test_core.py
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-05-05 09:48:07.000000 napari-correct-drift-0.0.2/src/napari_correct_drift/_tests/test_sample_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)      845 2023-05-05 09:48:07.000000 napari-correct-drift-0.0.2/src/napari_correct_drift/_tests/test_widget.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18236 2023-05-05 09:48:07.000000 napari-correct-drift-0.0.2/src/napari_correct_drift/_widget.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1133 2023-05-05 09:48:07.000000 napari-correct-drift-0.0.2/src/napari_correct_drift/napari.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 09:48:34.246965 napari-correct-drift-0.0.2/src/napari_correct_drift.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3843 2023-05-05 09:48:34.000000 napari-correct-drift-0.0.2/src/napari_correct_drift.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      717 2023-05-05 09:48:34.000000 napari-correct-drift-0.0.2/src/napari_correct_drift.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 09:48:34.000000 napari-correct-drift-0.0.2/src/napari_correct_drift.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-05-05 09:48:34.000000 napari-correct-drift-0.0.2/src/napari_correct_drift.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-05-05 09:48:34.000000 napari-correct-drift-0.0.2/src/napari_correct_drift.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-05 09:48:34.000000 napari-correct-drift-0.0.2/src/napari_correct_drift.egg-info/top_level.txt
```

### Comparing `napari-correct-drift-0.0.1/LICENSE` & `napari-correct-drift-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `napari-correct-drift-0.0.1/PKG-INFO` & `napari-correct-drift-0.0.2/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: napari-correct-drift
-Version: 0.0.1
+Version: 0.0.2
 Summary: Drift correction 2D/3D for Napari similar to Fijis Correct 3D drift
 Home-page: https://github.com/sommerc/napari-correct-drift
 Author: Christoph Sommer
 Author-email: christoph.sommer@ist.ac.at
 License: BSD-3-Clause
 Project-URL: Bug Tracker, https://github.com/sommerc/napari-correct-drift/issues
 Project-URL: Documentation, https://github.com/sommerc/napari-correct-drift#README.md
@@ -39,15 +39,15 @@
 Napari-correct-drift brings the functionality of Fiji’s popular Correct-3D-drift macro to Napari for flexible and efficient correction of stage and sample drift common in time-lapse microscopy.
 
 Napari-correct-drift supports drift correction for 2D/3D multi-channel data.
 
 ----------------------------------
 ## Example
 
-*to come soon*
+https://user-images.githubusercontent.com/895863/235100349-83379350-06a5-4fe7-9323-f3e5771cca2e.mp4
 
 
 ## Test data
 Napari-correct-drift contains synthetic sample data. To test it on real data download an example Arabidopsis growing [root tip](https://seafile.ist.ac.at/f/b05362d4f358430c8c59/?dl=1) file.
 
 ## Installation
 
@@ -63,15 +63,15 @@
 
 ## Roadmap
 
 - [x] Basic CorrectDrift interface
 - [x] Synthetic test data
 - [x] Unit tests
 - [x] 2D/3D multi-channel support
-- [x] ROI support
+- [x] ROI support (rectangles)
 - [x] Saving and loading of drift tables
 - [ ] [pyGPUreg](https://github.com/bionanopatterning/pyGPUreg) backend
 - [ ] Outlier handling
 - [ ] Speed optimizations
 - [ ] Sphinx documentation
 - [ ] How-tos
 - [ ] Tutorials and Guides
@@ -81,7 +81,10 @@
 Contributions are very welcome. Tests can be run with [tox], please ensure
 the coverage at least stays the same before you submit a pull request.
 
 ## License
 
 Distributed under the terms of the [BSD-3] license,
 "napari-correct-drift" is free and open source software
+
+### Acknowledgment
+This project has been made possible in part by grant number NP2-0000000051 from the napari Plugin Foundations Grants (Cycle 2).
```

### Comparing `napari-correct-drift-0.0.1/README.md` & `napari-correct-drift-0.0.2/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 Napari-correct-drift brings the functionality of Fiji’s popular Correct-3D-drift macro to Napari for flexible and efficient correction of stage and sample drift common in time-lapse microscopy.
 
 Napari-correct-drift supports drift correction for 2D/3D multi-channel data.
 
 ----------------------------------
 ## Example
 
-*to come soon*
+https://user-images.githubusercontent.com/895863/235100349-83379350-06a5-4fe7-9323-f3e5771cca2e.mp4
 
 
 ## Test data
 Napari-correct-drift contains synthetic sample data. To test it on real data download an example Arabidopsis growing [root tip](https://seafile.ist.ac.at/f/b05362d4f358430c8c59/?dl=1) file.
 
 ## Installation
 
@@ -34,15 +34,15 @@
 
 ## Roadmap
 
 - [x] Basic CorrectDrift interface
 - [x] Synthetic test data
 - [x] Unit tests
 - [x] 2D/3D multi-channel support
-- [x] ROI support
+- [x] ROI support (rectangles)
 - [x] Saving and loading of drift tables
 - [ ] [pyGPUreg](https://github.com/bionanopatterning/pyGPUreg) backend
 - [ ] Outlier handling
 - [ ] Speed optimizations
 - [ ] Sphinx documentation
 - [ ] How-tos
 - [ ] Tutorials and Guides
@@ -52,7 +52,10 @@
 Contributions are very welcome. Tests can be run with [tox], please ensure
 the coverage at least stays the same before you submit a pull request.
 
 ## License
 
 Distributed under the terms of the [BSD-3] license,
 "napari-correct-drift" is free and open source software
+
+### Acknowledgment
+This project has been made possible in part by grant number NP2-0000000051 from the napari Plugin Foundations Grants (Cycle 2).
```

### Comparing `napari-correct-drift-0.0.1/setup.cfg` & `napari-correct-drift-0.0.2/setup.cfg`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = napari-correct-drift
-version = 0.0.1
+version = 0.0.2
 description = Drift correction 2D/3D for Napari similar to Fijis Correct 3D drift
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/sommerc/napari-correct-drift
 author = Christoph Sommer
 author_email = christoph.sommer@ist.ac.at
 license = BSD-3-Clause
```

### Comparing `napari-correct-drift-0.0.1/src/napari_correct_drift/_core.py` & `napari-correct-drift-0.0.2/src/napari_correct_drift/_core.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,69 +1,79 @@
-"""
-doc
-"""
+import warnings
 
 import numpy as np
-from scipy.ndimage import shift
+from napari.utils import progress
 from scipy.interpolate import interp1d
+from scipy.ndimage import shift
 from skimage.registration import phase_cross_correlation
 
-from napari.utils import progress
-
 
 class ArrayAxesStandardizer:
     """
     A class designed to standardize the axes of numpy arrays.
 
     Attributes:
-        out_order (str): string representing the desired output order of the array axes
-        in_order (str): string representing the current order of the array axes
+        out_order (str): string representing the desired output
+        order of the array axes in_order (str): string representing
+        the current order of the array axes
 
-        out_order and in_order are given as string containing t,c,z,y,x
+        out_order and in_order are given as string containing
+        t,c,z,y,x
 
     Methods:
         __init__(self, out_order: str, in_order: str):
             Initializes the class and checks for any invalid inputs.
 
         _check_order_str(self, order: str):
             Checks for any duplicates in the input order.
 
         __call__(self, data: np.array):
-            Takes in an input numpy array and standardizes the axes according to the output order.
+            Takes in an input numpy array and standardizes the
+            axes according to the output order.
             It returns the standardized array view.
 
         inv(self, data: np.array):
-            Takes in a standardized numpy array and reverts the axes back to the original order.
+            Takes in a standardized numpy array and reverts the
+            axes back to the original order.
             It returns the reverted array.
 
         inverse_permutation(a):
-            A static method that returns the inverse permutation of an input permutation.
+            A static method that returns the inverse permutation
+            of an input permutation.
 
     Parameters:
-        out_order (str): a string representing the desired output order of the array axes.
-        in_order (str): a string representing the current order of the array axes.
-        data (np.array): a numpy array that needs to be standardized or reverted.
+        out_order (str): a string representing the desired output
+        order of the array axes.
+        in_order (str): a string representing the current order
+        of the array axes.
+        data (np.array): a numpy array that needs to be
+        standardized or reverted.
         a (np.array): an input permutation.
 
     Return Value:
         __call__(self, data: np.array): A standardized numpy array.
-        inv(self, data: np.array): A numpy array with the original axis order.
-        inverse_permutation(a): An inverse permutation of the input permutation.
+        inv(self, data: np.array): A numpy array with the original
+        axis order.
+        inverse_permutation(a): An inverse permutation of the input
+        permutation.
     """
 
     def __init__(self, out_order: str, in_order: str):
         """
         Initializes the class and checks for any invalid inputs.
 
         Args:
-            out_order (str): A string representing the desired output order of the array axes.
-            in_order (str): A string representing the current order of the array axes.
+            out_order (str): A string representing the desired output
+            order of the array axes.
+            in_order (str): A string representing the current order of
+            the array axes.
 
         Raises:
-            AssertionError: If in_order contains any elements not in out_order or if out_order or in_order contains duplicates.
+            AssertionError: If in_order contains any elements not in
+            out_order or if out_order or in_order contains duplicates.
         """
         self._check_order_str(out_order)
         self._check_order_str(in_order)
 
         assert set(in_order).issubset(
             set(out_order)
         ), "in_order not subset of out_order"
@@ -72,70 +82,78 @@
         self.in_order = in_order
 
     def _check_order_str(self, order: str):
         """
         Checks for any duplicates in the input order.
 
         Args:
-            order (str): A string representing the current order of the array axes.
+            order (str): A string representing the current order of
+            the array axes.
 
         Raises:
             AssertionError: If order contains duplicates.
         """
         assert len(set(order)) == len(
             order
         ), f"Duplicates in order found: '{order}'"
 
     def __call__(self, data: np.array):
         """
-        Takes in an input numpy array and standardizes the axes according to the output order.
+        Takes in an input numpy array and standardizes the axes according
+        to the output order.
         It returns the standardized array.
 
         Args:
             data (np.array): A numpy array that needs to be standardized.
 
         Returns:
             np.array: A standardized numpy array.
 
         Raises:
-            AssertionError: If the shape of the input array does not match the input order.
+            AssertionError: If the shape of the input array does not match
+            the input order.
         """
 
-        assert len(data.shape) == len(
-            self.in_order
-        ), f"Shape mismatch. Data shape is '{data.shape}', but in order is '{self.in_order}'"
+        assert len(data.shape) == len(self.in_order), (
+            f"Shape mismatch. Data shape is '{data.shape}'"
+            ", but in order is '{self.in_order}'"
+        )
         permute = []
         missing = []
         for i, dim in enumerate(self.out_order):
             j = self.in_order.find(dim)
             permute.append(j) if j > -1 else missing.append(i)
 
         data_rearranged = np.expand_dims(data.transpose(permute), missing)
-        assert not data_rearranged.flags["OWNDATA"], "not a view??"
+        # assert not data_rearranged.flags["OWNDATA"], "not a view??"
         return data_rearranged
 
     def inv(self, data: np.array):
         """
-        Applies the inverse transform to the input data. The input data is expected to be a numpy array with the shape
-        specified by the 'out_order' argument passed to the constructor. The output is a numpy array with the shape
+        Applies the inverse transform to the input data. The input data
+        is expected to be a numpy array with the shape
+        specified by the 'out_order' argument passed to the constructor.
+        The output is a numpy array with the shape
         specified by the 'in_order' argument passed to the constructor.
 
         Args:
             data (np.array): The input data to be transformed.
 
         Returns:
             np.array: The transformed data.
 
         Raises:
-            AssertionError: If the input data does not have the same shape as specified by the 'out_order' argument.
+            AssertionError: If the input data does not have the same shape
+            as specified by the 'out_order' argument.
         """
 
-        assert len(data.shape) == len(
-            self.out_order
-        ), f"Shape mismaatch. Data shape is '{data.shape}', but in order is '{self.out_order}'"
+        assert len(data.shape) == len(self.out_order), (
+            f"Shape mismaatch. Data shape is '{data.shape}',"
+            " but in order is '{self.out_order}'"
+        )
         permute = []
         missing = []
         for i, dim in enumerate(self.out_order):
             j = self.in_order.find(dim)
             permute.append(j) if j > -1 else missing.append(i)
 
         res = np.transpose(
@@ -196,15 +214,15 @@
 
         x_min = int(p_min[-1] + 0.5)
         x_max = int(p_max[-1] + 0.5)
 
         y_min = int(p_min[-2] + 0.5)
         y_max = int(p_max[-2] + 0.5)
 
-        if not "z" in dims:
+        if "z" not in dims:
             z_min = 0
             z_max = 1
 
         c0 = 0
         if "c" in dims:
             c = dims.find("c")
             c0 = int(p_min[c])
@@ -241,53 +259,59 @@
     def __str__(self):
         return f"""
         t0 {self.t0}
         c0 {self.c0}
         z: {self.z_min}, {self.z_max}
         y: {self.y_min}, {self.y_max}
         x: {self.x_min}, {self.x_max}
-        
+
         bbox: {self.bbox}
         """
 
 
 class CorrectDrift:
     """
     Class for drift correction of microscopy images.
 
     Parameters
     ----------
     data : np.array
-        The input data, with dimensions ordered according to the given `dims`.
+        The input data, with dimensions ordered according to
+        the given `dims`.
     dims : str
-        The dimension order of the input data. Must include axes 't', 'x', and 'y'.
+        The dimension order of the input data. Must include
+        axes 't', 'x', and 'y'.
 
     Attributes
     ----------
     is_multi_channel : bool
         True if the data has multiple channels.
     is_3d : bool
         True if the data has a z dimension.
     dims : str
         The dimension order of the input data.
     data_arranger : ArrayAxesStandardizer
         An ArrayAxesStandardizer instance used to rearrange the input data.
     data : np.array
         The rearranged input data.
     T, C, Z, Y, X : int
-        The number of time points, channels, z-slices, rows, and columns in the input data.
+        The number of time points, channels, z-slices, rows, and columns
+        in the input data.
 
     Methods
     -------
-    estimate_shifts_absolute(t0=0, channel=0, increment=1, upsample_factor=1, roi=None)
-        Estimates the absolute shifts for each time point using cross-correlation.
+    estimate_shifts_absolute(t0=0, channel=0, increment=1, upsample_factor=1,
+    roi=None)
+        Estimates the absolute shifts for each time point using cross-
+        correlation.
     iter_abs(T, t0, step)
         An iterator that generates time points for estimating absolute shifts.
     estimate_shifts_relative(t0=0, step=1, upsample_factor=1, roi=None)
-        Estimates the relative shifts for each time point using cross-correlation.
+        Estimates the relative shifts for each time point using cross-
+        correlation.
     iter_rel(T, t0, step)
         An iterator that generates time points for estimating relative shifts.
     interpolate_offsets(offsets)
         Interpolates any missing offsets using linear interpolation.
     apply_shifts(offsets, extend_output=False, order=1, mode='constant')
         Applies the given offsets to the input data to correct for drift.
 
@@ -418,21 +442,27 @@
 
                 ref_img[
                     : ref_img_crop.shape[0],
                     : ref_img_crop.shape[1],
                     : ref_img_crop.shape[2],
                 ] = ref_img_crop
 
-            offset, _, _ = phase_cross_correlation(
-                ref_img,
-                mov_img,
-                upsample_factor=upsample_factor,
-                return_error="always",
-                disambiguate=True,
-            )
+            with warnings.catch_warnings():
+                warnings.filterwarnings(
+                    action="ignore",
+                    category=RuntimeWarning,
+                )
+                offset, _, _ = phase_cross_correlation(
+                    ref_img,
+                    mov_img,
+                    upsample_factor=upsample_factor,
+                    return_error="always",
+                    disambiguate=True,
+                )
+
             offset = np.asarray(offset, dtype="float32")
 
             if roi is not None:
                 offset += mov_bbox[::2]
 
             if roi is not None:
                 mov_bbox[::2] -= np.round(offset).astype("int32")
@@ -488,21 +518,26 @@
 
         for _, m in progress(
             self.iter_abs(self.T, t0, increment),
             desc=f"Estimate drift (absolute to frame '{t0}')",
         ):
             mov_img = self.data[m, channel]
 
-            offset, _, _ = phase_cross_correlation(
-                ref_img,
-                mov_img,
-                upsample_factor=upsample_factor,
-                return_error="always",
-                disambiguate=True,
-            )
+            with warnings.catch_warnings():
+                warnings.filterwarnings(
+                    action="ignore",
+                    category=RuntimeWarning,
+                )
+                offset, _, _ = phase_cross_correlation(
+                    ref_img,
+                    mov_img,
+                    upsample_factor=upsample_factor,
+                    return_error="always",
+                    disambiguate=True,
+                )
 
             offset = -np.asarray(offset, dtype="float32")
 
             if roi is not None:
                 offset -= roi.bbox[::2]
 
             offsets[m] = offset
@@ -542,15 +577,15 @@
             # split shifts into integer and subpixel parts.
             # the ndi.shift takes care of subpixel part
             # the interger shifts are handled via giving an output slice
 
             offsets_px = -np.ceil(offsets - offsets.max(0)).astype("int")
             offsets_sub = -(offsets - offsets.max(0)) - offsets_px
 
-            for t in progress(range(self.T), desc=f"Applying drift"):
+            for t in progress(range(self.T), desc="Applying drift"):
                 for c in range(self.C):
                     img = self.data[t, c]
                     output_view = output[
                         t,
                         c,
                         offsets_px[t, 0] : offsets_px[t, 0] + img.shape[0],
                         offsets_px[t, 1] : offsets_px[t, 1] + img.shape[1],
@@ -564,15 +599,15 @@
                         order=order,
                         mode=mode,
                         prefilter=False,
                     )
 
         else:
             output = np.zeros_like(self.data)
-            for t in progress(range(self.T), desc=f"Applying drift"):
+            for t in progress(range(self.T), desc="Applying drift"):
                 for c in range(self.C):
                     img = self.data[t, c]
                     output[t, c] = shift(
                         img,
                         -offsets[t],
                         order=order,
                         mode=mode,
```

### Comparing `napari-correct-drift-0.0.1/src/napari_correct_drift/_sample_data.py` & `napari-correct-drift-0.0.2/src/napari_correct_drift/_sample_data.py`

 * *Files identical despite different names*

### Comparing `napari-correct-drift-0.0.1/src/napari_correct_drift/_tests/test_core.py` & `napari-correct-drift-0.0.2/src/napari_correct_drift/_tests/test_core.py`

 * *Files identical despite different names*

### Comparing `napari-correct-drift-0.0.1/src/napari_correct_drift/_tests/test_widget.py` & `napari-correct-drift-0.0.2/src/napari_correct_drift/_tests/test_widget.py`

 * *Files identical despite different names*

### Comparing `napari-correct-drift-0.0.1/src/napari_correct_drift/_widget.py` & `napari-correct-drift-0.0.2/src/napari_correct_drift/_widget.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,42 +4,36 @@
 It implements the Widget specification.
 see: https://napari.org/stable/plugins/guides.html?#widgets
 
 Replace code below according to your needs.
 """
 from typing import TYPE_CHECKING
 
+import numpy as np
 from napari.layers.image.image import Image as IMAGE_LAYER
 from napari.layers.shapes.shapes import Shapes as SHAPE_LAYER
 from napari.utils import notifications
-from numpy.lib.arraysetops import isin
-from qtpy.QtCore import Qt
-from qtpy.QtCore import QAbstractTableModel
+from pandas import DataFrame, read_csv
+from qtpy.QtCore import QAbstractTableModel, Qt
 from qtpy.QtWidgets import (
-    QButtonGroup,
     QCheckBox,
     QComboBox,
     QFileDialog,
     QGridLayout,
     QGroupBox,
     QHBoxLayout,
     QLabel,
     QPushButton,
-    QSlider,
     QSpinBox,
-    QTableWidget,
+    QTableView,
     QVBoxLayout,
     QWidget,
-    QTableWidgetItem,
-    QTableView,
 )
 
 from ._core import CorrectDrift, ROIRect
-from pandas import DataFrame, read_csv
-import numpy as np
 
 if TYPE_CHECKING:
     import napari
 
 
 class CorrectDriftDock(QWidget):
     ROI_LAYER_NAME = "ROI"
@@ -203,14 +197,17 @@
                     if isinstance(layer, SHAPE_LAYER) and (
                         layer.name == self.ROI_LAYER_NAME
                     ):
                         break
                 else:
                     ndim = self.get_current_input_layer().ndim
                     self.viewer.add_shapes(name=self.ROI_LAYER_NAME, ndim=ndim)
+                    notifications.show_info(
+                        f"Add a ROI to the created '{self.ROI_LAYER_NAME}' shape layer. \nThe ROI's key frame / channel will be used"
+                    )
 
         def toggle_z_selection(checked):
             for w in self.z_roi_sel_widgets:
                 w.setVisible(checked)
 
             self.key_frame.setDisabled(checked)
             self.key_channel.setDisabled(checked)
@@ -281,54 +278,44 @@
         self.input_layer.setToolTip("Select input layer for drift correction")
 
         self.estimate_drift_button.setToolTip("Estimate drift")
         self.load_drift_button.setToolTip("Load drift from .csv")
         self.apply_drift_button.setToolTip("Apply drift shown in dirft table")
 
         self.estimate_drift_mode.setToolTip(
-            (
-                "Mode for drift estimation:\n"
-                " - relative: estimate from previous frame. ROI will move along!\n"
-                " - absolute: estimate against absolute frame                    "
-            )
+            "Mode for drift estimation:\n"
+            " - relative: estimate from previous frame. ROI will move along!\n"
+            " - absolute: estimate against absolute frame                    "
         )
 
         self.key_frame.setToolTip(
-            (
-                "The frame number that should be stabilized during drift correction.\n"
-                "When ROI is enabled, the value is inferred from the ROI.            "
-            )
+            "The frame number that should be stabilized during drift correction.\n"
+            "When ROI is enabled, the value is inferred from the ROI.            "
         )
         self.key_channel.setToolTip(
-            (
-                "The channel number that should be stabilized during drift correction.\n"
-                "When ROI is enabled, the value is inferred from the ROI.              "
-            )
+            "The channel number that should be stabilized during drift correction.\n"
+            "When ROI is enabled, the value is inferred from the ROI.              "
         )
 
         self.roi_checkbox.setToolTip(
             "Use ROI from 'ROI' shape layer. By default 1st ROI is used"
         )
         self.roi_z_min.setToolTip("Minimum z-plane for the ROI")
         self.roi_z_max.setToolTip("Maximum z-plane for the ROI")
 
         self.increment_box.setToolTip(
-            (
-                "Time increment for drift estimation. Useful for faster estimation and \n"
-                "slow drifts. Skipped frames will be linearly interpolated.              "
-            )
+            "Time increment for drift estimation. Useful for faster estimation and \n"
+            "slow drifts. Skipped frames will be linearly interpolated.              "
         )
         self.upsample_box.setToolTip(
             "Subpixel drift estimation. Useful for slow drifts"
         )
         self.extend_output.setToolTip(
-            (
-                "Apply drifts with extended spatial dimensions. The raw image frames will\n"
-                "be fully contained in the output.                                         "
-            )
+            "Apply drifts with extended spatial dimensions. The raw image frames will\n"
+            "be fully contained in the output.                                         "
         )
 
     def _init_other_params(self):
         parameter_panel = QGroupBox("Parameters")
         parameter_layout = QGridLayout()
         parameter_panel.setLayout(parameter_layout)
         i = 1
```

### Comparing `napari-correct-drift-0.0.1/src/napari_correct_drift/napari.yaml` & `napari-correct-drift-0.0.2/src/napari_correct_drift/napari.yaml`

 * *Files identical despite different names*

### Comparing `napari-correct-drift-0.0.1/src/napari_correct_drift.egg-info/PKG-INFO` & `napari-correct-drift-0.0.2/src/napari_correct_drift.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: napari-correct-drift
-Version: 0.0.1
+Version: 0.0.2
 Summary: Drift correction 2D/3D for Napari similar to Fijis Correct 3D drift
 Home-page: https://github.com/sommerc/napari-correct-drift
 Author: Christoph Sommer
 Author-email: christoph.sommer@ist.ac.at
 License: BSD-3-Clause
 Project-URL: Bug Tracker, https://github.com/sommerc/napari-correct-drift/issues
 Project-URL: Documentation, https://github.com/sommerc/napari-correct-drift#README.md
@@ -39,15 +39,15 @@
 Napari-correct-drift brings the functionality of Fiji’s popular Correct-3D-drift macro to Napari for flexible and efficient correction of stage and sample drift common in time-lapse microscopy.
 
 Napari-correct-drift supports drift correction for 2D/3D multi-channel data.
 
 ----------------------------------
 ## Example
 
-*to come soon*
+https://user-images.githubusercontent.com/895863/235100349-83379350-06a5-4fe7-9323-f3e5771cca2e.mp4
 
 
 ## Test data
 Napari-correct-drift contains synthetic sample data. To test it on real data download an example Arabidopsis growing [root tip](https://seafile.ist.ac.at/f/b05362d4f358430c8c59/?dl=1) file.
 
 ## Installation
 
@@ -63,15 +63,15 @@
 
 ## Roadmap
 
 - [x] Basic CorrectDrift interface
 - [x] Synthetic test data
 - [x] Unit tests
 - [x] 2D/3D multi-channel support
-- [x] ROI support
+- [x] ROI support (rectangles)
 - [x] Saving and loading of drift tables
 - [ ] [pyGPUreg](https://github.com/bionanopatterning/pyGPUreg) backend
 - [ ] Outlier handling
 - [ ] Speed optimizations
 - [ ] Sphinx documentation
 - [ ] How-tos
 - [ ] Tutorials and Guides
@@ -81,7 +81,10 @@
 Contributions are very welcome. Tests can be run with [tox], please ensure
 the coverage at least stays the same before you submit a pull request.
 
 ## License
 
 Distributed under the terms of the [BSD-3] license,
 "napari-correct-drift" is free and open source software
+
+### Acknowledgment
+This project has been made possible in part by grant number NP2-0000000051 from the napari Plugin Foundations Grants (Cycle 2).
```

### Comparing `napari-correct-drift-0.0.1/src/napari_correct_drift.egg-info/SOURCES.txt` & `napari-correct-drift-0.0.2/src/napari_correct_drift.egg-info/SOURCES.txt`

 * *Files identical despite different names*

