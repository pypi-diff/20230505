# Comparing `tmp/matplotlib_label_lines-0.5.2.tar.gz` & `tmp/matplotlib_label_lines-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "matplotlib_label_lines-0.5.2.tar", last modified: Thu Apr 13 09:12:25 2023, max compression
+gzip compressed data, was "matplotlib_label_lines-0.6.0.tar", last modified: Fri May  5 11:58:34 2023, max compression
```

## Comparing `matplotlib_label_lines-0.5.2.tar` & `matplotlib_label_lines-0.6.0.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 cphyc     (1000) cphyc     (1000)        0 2023-04-13 09:12:25.124145 matplotlib_label_lines-0.5.2/
--rw-r--r--   0 cphyc     (1000) cphyc     (1000)     1072 2017-12-31 16:20:51.000000 matplotlib_label_lines-0.5.2/LICENSE
--rw-r--r--   0 cphyc     (1000) cphyc     (1000)       26 2021-01-15 10:44:15.000000 matplotlib_label_lines-0.5.2/MANIFEST.in
--rw-r--r--   0 cphyc     (1000) cphyc     (1000)     3703 2023-04-13 09:12:25.124145 matplotlib_label_lines-0.5.2/PKG-INFO
--rw-r--r--   0 cphyc     (1000) cphyc     (1000)     2894 2023-04-13 09:05:24.000000 matplotlib_label_lines-0.5.2/Readme.md
-drwxr-xr-x   0 cphyc     (1000) cphyc     (1000)        0 2023-04-13 09:12:25.124145 matplotlib_label_lines-0.5.2/labellines/
--rw-r--r--   0 cphyc     (1000) cphyc     (1000)      101 2023-04-13 09:04:11.000000 matplotlib_label_lines-0.5.2/labellines/__init__.py
--rw-r--r--   0 cphyc     (1000) cphyc     (1000)     7929 2023-04-13 09:03:59.000000 matplotlib_label_lines-0.5.2/labellines/core.py
--rw-r--r--   0 cphyc     (1000) cphyc     (1000)     6777 2023-04-13 09:03:59.000000 matplotlib_label_lines-0.5.2/labellines/line_label.py
--rw-r--r--   0 cphyc     (1000) cphyc     (1000)     9763 2023-04-13 09:03:59.000000 matplotlib_label_lines-0.5.2/labellines/test.py
--rw-r--r--   0 cphyc     (1000) cphyc     (1000)     3714 2023-04-13 09:03:59.000000 matplotlib_label_lines-0.5.2/labellines/utils.py
-drwxr-xr-x   0 cphyc     (1000) cphyc     (1000)        0 2023-04-13 09:12:25.124145 matplotlib_label_lines-0.5.2/matplotlib_label_lines.egg-info/
--rw-r--r--   0 cphyc     (1000) cphyc     (1000)     3703 2023-04-13 09:12:25.000000 matplotlib_label_lines-0.5.2/matplotlib_label_lines.egg-info/PKG-INFO
--rw-r--r--   0 cphyc     (1000) cphyc     (1000)      398 2023-04-13 09:12:25.000000 matplotlib_label_lines-0.5.2/matplotlib_label_lines.egg-info/SOURCES.txt
--rw-r--r--   0 cphyc     (1000) cphyc     (1000)        1 2023-04-13 09:12:25.000000 matplotlib_label_lines-0.5.2/matplotlib_label_lines.egg-info/dependency_links.txt
--rw-r--r--   0 cphyc     (1000) cphyc     (1000)      120 2023-04-13 09:12:25.000000 matplotlib_label_lines-0.5.2/matplotlib_label_lines.egg-info/requires.txt
--rw-r--r--   0 cphyc     (1000) cphyc     (1000)       11 2023-04-13 09:12:25.000000 matplotlib_label_lines-0.5.2/matplotlib_label_lines.egg-info/top_level.txt
--rw-r--r--   0 cphyc     (1000) cphyc     (1000)      645 2023-02-22 17:22:22.000000 matplotlib_label_lines-0.5.2/pyproject.toml
--rw-r--r--   0 cphyc     (1000) cphyc     (1000)      997 2023-04-13 09:12:25.124145 matplotlib_label_lines-0.5.2/setup.cfg
--rw-r--r--   0 cphyc     (1000) cphyc     (1000)       38 2021-09-07 10:58:27.000000 matplotlib_label_lines-0.5.2/setup.py
+drwxr-xr-x   0 cphyc     (1000) cphyc     (1000)        0 2023-05-05 11:58:34.364327 matplotlib_label_lines-0.6.0/
+-rw-r--r--   0 cphyc     (1000) cphyc     (1000)     1072 2017-12-31 16:20:51.000000 matplotlib_label_lines-0.6.0/LICENSE
+-rw-r--r--   0 cphyc     (1000) cphyc     (1000)       26 2021-01-15 10:44:15.000000 matplotlib_label_lines-0.6.0/MANIFEST.in
+-rw-r--r--   0 cphyc     (1000) cphyc     (1000)     3703 2023-05-05 11:58:34.364327 matplotlib_label_lines-0.6.0/PKG-INFO
+-rw-r--r--   0 cphyc     (1000) cphyc     (1000)     2894 2023-05-05 11:57:57.000000 matplotlib_label_lines-0.6.0/Readme.md
+drwxr-xr-x   0 cphyc     (1000) cphyc     (1000)        0 2023-05-05 11:58:34.364327 matplotlib_label_lines-0.6.0/labellines/
+-rw-r--r--   0 cphyc     (1000) cphyc     (1000)      101 2023-05-05 11:57:57.000000 matplotlib_label_lines-0.6.0/labellines/__init__.py
+-rw-r--r--   0 cphyc     (1000) cphyc     (1000)     8004 2023-05-05 11:55:48.000000 matplotlib_label_lines-0.6.0/labellines/core.py
+-rw-r--r--   0 cphyc     (1000) cphyc     (1000)     6777 2023-04-13 09:03:59.000000 matplotlib_label_lines-0.6.0/labellines/line_label.py
+-rw-r--r--   0 cphyc     (1000) cphyc     (1000)     9766 2023-05-05 11:55:48.000000 matplotlib_label_lines-0.6.0/labellines/test.py
+-rw-r--r--   0 cphyc     (1000) cphyc     (1000)     2701 2023-05-05 11:41:47.000000 matplotlib_label_lines-0.6.0/labellines/utils.py
+drwxr-xr-x   0 cphyc     (1000) cphyc     (1000)        0 2023-05-05 11:58:34.364327 matplotlib_label_lines-0.6.0/matplotlib_label_lines.egg-info/
+-rw-r--r--   0 cphyc     (1000) cphyc     (1000)     3703 2023-05-05 11:58:34.000000 matplotlib_label_lines-0.6.0/matplotlib_label_lines.egg-info/PKG-INFO
+-rw-r--r--   0 cphyc     (1000) cphyc     (1000)      398 2023-05-05 11:58:34.000000 matplotlib_label_lines-0.6.0/matplotlib_label_lines.egg-info/SOURCES.txt
+-rw-r--r--   0 cphyc     (1000) cphyc     (1000)        1 2023-05-05 11:58:34.000000 matplotlib_label_lines-0.6.0/matplotlib_label_lines.egg-info/dependency_links.txt
+-rw-r--r--   0 cphyc     (1000) cphyc     (1000)      120 2023-05-05 11:58:34.000000 matplotlib_label_lines-0.6.0/matplotlib_label_lines.egg-info/requires.txt
+-rw-r--r--   0 cphyc     (1000) cphyc     (1000)       11 2023-05-05 11:58:34.000000 matplotlib_label_lines-0.6.0/matplotlib_label_lines.egg-info/top_level.txt
+-rw-r--r--   0 cphyc     (1000) cphyc     (1000)      645 2023-02-22 17:22:22.000000 matplotlib_label_lines-0.6.0/pyproject.toml
+-rw-r--r--   0 cphyc     (1000) cphyc     (1000)      997 2023-05-05 11:58:34.364327 matplotlib_label_lines-0.6.0/setup.cfg
+-rw-r--r--   0 cphyc     (1000) cphyc     (1000)       38 2021-09-07 10:58:27.000000 matplotlib_label_lines-0.6.0/setup.py
```

### Comparing `matplotlib_label_lines-0.5.2/LICENSE` & `matplotlib_label_lines-0.6.0/LICENSE`

 * *Files identical despite different names*

### Comparing `matplotlib_label_lines-0.5.2/PKG-INFO` & `matplotlib_label_lines-0.6.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: matplotlib_label_lines
-Version: 0.5.2
+Version: 0.6.0
 Summary: Label lines in matplotlib.
 Home-page: https://github.com/cphyc/matplotlib-label-lines
 Author: Corentin Cadiou
 Author-email: contact@cphyc.me
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
@@ -19,15 +19,15 @@
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: test
 License-File: LICENSE
 
 # matplotlib-label-lines
 [![Build status](https://github.com/cphyc/matplotlib-label-lines/actions/workflows/pytest.yml/badge.svg)](https://github.com/cphyc/matplotlib-label-lines/actions/workflows/pytest.yml)
-[![Supported Python Versions](https://img.shields.io/pypi/pyversions/matplotlib-label-lines/0.5.2)](https://pypi.org/project/matplotlib-label-lines/)
+[![Supported Python Versions](https://img.shields.io/pypi/pyversions/matplotlib-label-lines/0.6.0)](https://pypi.org/project/matplotlib-label-lines/)
 [![PyPI](https://img.shields.io/pypi/v/matplotlib-label-lines)](https://pypi.org/project/matplotlib-label-lines)
 [![codecov](https://codecov.io/gh/cphyc/matplotlib-label-lines/branch/master/graph/badge.svg)](https://codecov.io/gh/cphyc/matplotlib-label-lines)
 
 Easily label line(s) using matplotlib.
 
 The code is heavily based on http://stackoverflow.com/questions/16992038/inline-labels-in-matplotlib (original code from NauticalMile).
```

### Comparing `matplotlib_label_lines-0.5.2/Readme.md` & `matplotlib_label_lines-0.6.0/Readme.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 # matplotlib-label-lines
 [![Build status](https://github.com/cphyc/matplotlib-label-lines/actions/workflows/pytest.yml/badge.svg)](https://github.com/cphyc/matplotlib-label-lines/actions/workflows/pytest.yml)
-[![Supported Python Versions](https://img.shields.io/pypi/pyversions/matplotlib-label-lines/0.5.2)](https://pypi.org/project/matplotlib-label-lines/)
+[![Supported Python Versions](https://img.shields.io/pypi/pyversions/matplotlib-label-lines/0.6.0)](https://pypi.org/project/matplotlib-label-lines/)
 [![PyPI](https://img.shields.io/pypi/v/matplotlib-label-lines)](https://pypi.org/project/matplotlib-label-lines)
 [![codecov](https://codecov.io/gh/cphyc/matplotlib-label-lines/branch/master/graph/badge.svg)](https://codecov.io/gh/cphyc/matplotlib-label-lines)
 
 Easily label line(s) using matplotlib.
 
 The code is heavily based on http://stackoverflow.com/questions/16992038/inline-labels-in-matplotlib (original code from NauticalMile).
```

### Comparing `matplotlib_label_lines-0.5.2/labellines/core.py` & `matplotlib_label_lines-0.6.0/labellines/core.py`

 * *Files 2% similar despite different names*

```diff
@@ -123,27 +123,28 @@
        Optional arguments passed to ax.text
     """
     if lines:
         ax = lines[0].axes
     else:
         ax = plt.gca()
 
-    handles, all_labels = ax.get_legend_handles_labels()
+    handles, labels_of_handles = ax.get_legend_handles_labels()
 
-    all_lines = []
-    for h in handles:
+    all_lines, all_labels = [], []
+    for h, label in zip(handles, labels_of_handles):
         if isinstance(h, ErrorbarContainer):
             line = h.lines[0]
         else:
             line = h
 
         # If the user provided a list of lines to label, only label those
         if (lines is not None) and (line not in lines):
             continue
         all_lines.append(line)
+        all_labels.append(label)
 
     # Check that the lines passed to the function have all a label
     if lines is not None:
         for line in lines:
             if line in all_lines:
                 continue
 
@@ -202,19 +203,18 @@
         labels.append(label)
 
         # Move xlabel if it is outside valid range
         xdata, _ = normalize_xydata(line)
         if not (min(xdata) <= xv <= max(xdata)):
             warnings.warn(
                 (
-                    "The value at position %s in `xvals` is outside the range of its "
-                    "associated line (xmin=%s, xmax=%s, xval=%s). Clipping it "
+                    "The value at position {} in `xvals` is outside the range of its "
+                    "associated line (xmin={}, xmax={}, xval={}). Clipping it "
                     "into the allowed range."
-                )
-                % (i, min(xdata), max(xdata), xv),
+                ).format(i, min(xdata), max(xdata), xv),
                 UserWarning,
                 stacklevel=1,
             )
             new_xv = min(xdata) + (max(xdata) - min(xdata)) * 0.9
             xvals[i] = new_xv
 
     # Convert float values back to datetime in case of datetime axis
```

### Comparing `matplotlib_label_lines-0.5.2/labellines/line_label.py` & `matplotlib_label_lines-0.6.0/labellines/line_label.py`

 * *Files identical despite different names*

### Comparing `matplotlib_label_lines-0.5.2/labellines/test.py` & `matplotlib_label_lines-0.6.0/labellines/test.py`

 * *Files 1% similar despite different names*

```diff
@@ -199,27 +199,27 @@
 
 
 def test_nan_failure():
     x = np.array([0, 1])
     y = np.array([np.nan, np.nan])
 
     line = plt.plot(x, y, label="test")[0]
-    with pytest.raises(Exception):
+    with pytest.raises(ValueError):
         labelLine(line, 0.5)
 
 
 @pytest.mark.mpl_image_compare
 def test_label_range(setup_mpl):
     x = np.linspace(0, 1)
     line = plt.plot(x, x**2, label="lorem ipsum")[0]
 
     # This should fail
-    with pytest.raises(Exception):
+    with pytest.raises(ValueError):
         labelLine(line, -1)
-    with pytest.raises(Exception):
+    with pytest.raises(ValueError):
         labelLine(line, 2)
 
     # This should work
     labelLine(line, 0.5)
 
     return plt.gcf()
```

### Comparing `matplotlib_label_lines-0.5.2/labellines/utils.py` & `matplotlib_label_lines-0.6.0/labellines/utils.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,50 +1,24 @@
-from datetime import datetime
+from typing import Tuple
 
 import numpy as np
-from matplotlib.dates import date2num
 from matplotlib.lines import Line2D
 
 
-def normalize_xydata(line: Line2D) -> tuple[np.ndarray, np.ndarray]:
+def normalize_xydata(line: Line2D) -> Tuple[np.ndarray, np.ndarray]:
     """Make sure datetime values are properly converted to floats and convert
     into data coordinates."""
     # Convert the data into the data coordinates
     line_t = line.get_transform().transform
     axes_t = line.axes.transData.inverted().transform
     x, y = axes_t(line_t(line.get_xydata())).T
 
-    x, y = _convert_to_float(x), _convert_to_float(y)
     return x, y
 
 
-def _convert_to_float(value) -> float:
-    try:
-        # the last 3 boolean checks are for arrays with datetime64 and with
-        # a timezone, see these SO posts:
-        # https://stackoverflow.com/q/60714568/4549682
-        # https://stackoverflow.com/q/23063362/4549682
-        is_date_array = np.issubdtype(value.dtype, np.datetime64) or str(
-            value.dtype
-        ).startswith("datetime64")
-        is_array_of_dates = value.dtype == "O" and all(
-            isinstance(val, (datetime, np.datetime64)) for val in value
-        )
-        if (
-            isinstance(value, (datetime, np.datetime64))
-            or is_date_array
-            or is_array_of_dates
-        ):
-            return date2num(value)
-        else:  # another numpy dtype like float64
-            return np.asarray(value, dtype=float)
-    except AttributeError:  # possibly int or other float/int dtype
-        return value
-
-
 # From https://www.geeksforgeeks.org/maximum-bipartite-matching/
 class GFG:
     def __init__(self, graph):
         # residual graph
         self.graph = graph
         self.ppl = len(graph)
         self.jobs = len(graph[0])
```

### Comparing `matplotlib_label_lines-0.5.2/matplotlib_label_lines.egg-info/PKG-INFO` & `matplotlib_label_lines-0.6.0/matplotlib_label_lines.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: matplotlib-label-lines
-Version: 0.5.2
+Version: 0.6.0
 Summary: Label lines in matplotlib.
 Home-page: https://github.com/cphyc/matplotlib-label-lines
 Author: Corentin Cadiou
 Author-email: contact@cphyc.me
 License: MIT
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
@@ -19,15 +19,15 @@
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: test
 License-File: LICENSE
 
 # matplotlib-label-lines
 [![Build status](https://github.com/cphyc/matplotlib-label-lines/actions/workflows/pytest.yml/badge.svg)](https://github.com/cphyc/matplotlib-label-lines/actions/workflows/pytest.yml)
-[![Supported Python Versions](https://img.shields.io/pypi/pyversions/matplotlib-label-lines/0.5.2)](https://pypi.org/project/matplotlib-label-lines/)
+[![Supported Python Versions](https://img.shields.io/pypi/pyversions/matplotlib-label-lines/0.6.0)](https://pypi.org/project/matplotlib-label-lines/)
 [![PyPI](https://img.shields.io/pypi/v/matplotlib-label-lines)](https://pypi.org/project/matplotlib-label-lines)
 [![codecov](https://codecov.io/gh/cphyc/matplotlib-label-lines/branch/master/graph/badge.svg)](https://codecov.io/gh/cphyc/matplotlib-label-lines)
 
 Easily label line(s) using matplotlib.
 
 The code is heavily based on http://stackoverflow.com/questions/16992038/inline-labels-in-matplotlib (original code from NauticalMile).
```

### Comparing `matplotlib_label_lines-0.5.2/pyproject.toml` & `matplotlib_label_lines-0.6.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `matplotlib_label_lines-0.5.2/setup.cfg` & `matplotlib_label_lines-0.6.0/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = matplotlib_label_lines
-version = 0.5.2
+version = 0.6.0
 description = Label lines in matplotlib.
 long_description = file: Readme.md
 long_description_content_type = text/markdown
 url = https://github.com/cphyc/matplotlib-label-lines
 author = Corentin Cadiou
 author_email = contact@cphyc.me
 license = MIT
```

