# Comparing `tmp/deephaven-plugin-plotly-express-0.0.2.tar.gz` & `tmp/deephaven-plugin-plotly-express-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "deephaven-plugin-plotly-express-0.0.2.tar", last modified: Tue May  2 17:45:17 2023, max compression
+gzip compressed data, was "deephaven-plugin-plotly-express-0.0.3.tar", last modified: Fri May  5 20:51:50 2023, max compression
```

## Comparing `deephaven-plugin-plotly-express-0.0.2.tar` & `deephaven-plugin-plotly-express-0.0.3.tar`

### file list

```diff
@@ -1,45 +1,46 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 17:45:17.351501 deephaven-plugin-plotly-express-0.0.2/
--rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-05-02 17:45:04.000000 deephaven-plugin-plotly-express-0.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2075 2023-05-02 17:45:17.351501 deephaven-plugin-plotly-express-0.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-05-02 17:45:04.000000 deephaven-plugin-plotly-express-0.0.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-05-02 17:45:04.000000 deephaven-plugin-plotly-express-0.0.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1170 2023-05-02 17:45:17.351501 deephaven-plugin-plotly-express-0.0.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 17:45:17.343500 deephaven-plugin-plotly-express-0.0.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 17:45:17.343500 deephaven-plugin-plotly-express-0.0.2/src/deephaven/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 17:45:17.343500 deephaven-plugin-plotly-express-0.0.2/src/deephaven/plot/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 17:45:17.343500 deephaven-plugin-plotly-express-0.0.2/src/deephaven/plot/express/
--rw-r--r--   0 runner    (1001) docker     (123)     1015 2023-05-02 17:45:04.000000 deephaven-plugin-plotly-express-0.0.2/src/deephaven/plot/express/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 17:45:17.347500 deephaven-plugin-plotly-express-0.0.2/src/deephaven/plot/express/data_mapping/
--rw-r--r--   0 runner    (1001) docker     (123)     1952 2023-05-02 17:45:04.000000 deephaven-plugin-plotly-express-0.0.2/src/deephaven/plot/express/data_mapping/DataMapping.py
--rw-r--r--   0 runner    (1001) docker     (123)       82 2023-05-02 17:45:04.000000 deephaven-plugin-plotly-express-0.0.2/src/deephaven/plot/express/data_mapping/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6383 2023-05-02 17:45:04.000000 deephaven-plugin-plotly-express-0.0.2/src/deephaven/plot/express/data_mapping/data_mapping.py
--rw-r--r--   0 runner    (1001) docker     (123)     2715 2023-05-02 17:45:04.000000 deephaven-plugin-plotly-express-0.0.2/src/deephaven/plot/express/data_mapping/json_conversion.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 17:45:17.347500 deephaven-plugin-plotly-express-0.0.2/src/deephaven/plot/express/deephaven_figure/
--rw-r--r--   0 runner    (1001) docker     (123)     4916 2023-05-02 17:45:04.000000 deephaven-plugin-plotly-express-0.0.2/src/deephaven/plot/express/deephaven_figure/DeephavenFigure.py
--rw-r--r--   0 runner    (1001) docker     (123)      166 2023-05-02 17:45:04.000000 deephaven-plugin-plotly-express-0.0.2/src/deephaven/plot/express/deephaven_figure/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3221 2023-05-02 17:45:04.000000 deephaven-plugin-plotly-express-0.0.2/src/deephaven/plot/express/deephaven_figure/custom_draw.py
--rw-r--r--   0 runner    (1001) docker     (123)    21657 2023-05-02 17:45:04.000000 deephaven-plugin-plotly-express-0.0.2/src/deephaven/plot/express/deephaven_figure/generate.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 17:45:17.347500 deephaven-plugin-plotly-express-0.0.2/src/deephaven/plot/express/plots/
--rw-r--r--   0 runner    (1001) docker     (123)      431 2023-05-02 17:45:04.000000 deephaven-plugin-plotly-express-0.0.2/src/deephaven/plot/express/plots/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    23657 2023-05-02 17:45:04.000000 deephaven-plugin-plotly-express-0.0.2/src/deephaven/plot/express/plots/_private_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     5713 2023-05-02 17:45:04.000000 deephaven-plugin-plotly-express-0.0.2/src/deephaven/plot/express/plots/area.py
--rw-r--r--   0 runner    (1001) docker     (123)    12185 2023-05-02 17:45:04.000000 deephaven-plugin-plotly-express-0.0.2/src/deephaven/plot/express/plots/bar.py
--rw-r--r--   0 runner    (1001) docker     (123)    20355 2023-05-02 17:45:04.000000 deephaven-plugin-plotly-express-0.0.2/src/deephaven/plot/express/plots/distribution.py
--rw-r--r--   0 runner    (1001) docker     (123)     6331 2023-05-02 17:45:04.000000 deephaven-plugin-plotly-express-0.0.2/src/deephaven/plot/express/plots/financial.py
--rw-r--r--   0 runner    (1001) docker     (123)    10436 2023-05-02 17:45:04.000000 deephaven-plugin-plotly-express-0.0.2/src/deephaven/plot/express/plots/hierarchial.py
--rw-r--r--   0 runner    (1001) docker     (123)    16934 2023-05-02 17:45:04.000000 deephaven-plugin-plotly-express-0.0.2/src/deephaven/plot/express/plots/line.py
--rw-r--r--   0 runner    (1001) docker     (123)     2392 2023-05-02 17:45:04.000000 deephaven-plugin-plotly-express-0.0.2/src/deephaven/plot/express/plots/pie.py
--rw-r--r--   0 runner    (1001) docker     (123)    16874 2023-05-02 17:45:04.000000 deephaven-plugin-plotly-express-0.0.2/src/deephaven/plot/express/plots/scatter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 17:45:17.351501 deephaven-plugin-plotly-express-0.0.2/src/deephaven/plot/express/preprocess/
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-02 17:45:04.000000 deephaven-plugin-plotly-express-0.0.2/src/deephaven/plot/express/preprocess/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8791 2023-05-02 17:45:04.000000 deephaven-plugin-plotly-express-0.0.2/src/deephaven/plot/express/preprocess/preprocess.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 17:45:17.351501 deephaven-plugin-plotly-express-0.0.2/src/deephaven/plot/express/shared/
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-05-02 17:45:04.000000 deephaven-plugin-plotly-express-0.0.2/src/deephaven/plot/express/shared/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      962 2023-05-02 17:45:04.000000 deephaven-plugin-plotly-express-0.0.2/src/deephaven/plot/express/shared/shared.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 17:45:17.351501 deephaven-plugin-plotly-express-0.0.2/src/deephaven_plugin_plotly_express.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2075 2023-05-02 17:45:17.000000 deephaven-plugin-plotly-express-0.0.2/src/deephaven_plugin_plotly_express.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1530 2023-05-02 17:45:17.000000 deephaven-plugin-plotly-express-0.0.2/src/deephaven_plugin_plotly_express.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-02 17:45:17.000000 deephaven-plugin-plotly-express-0.0.2/src/deephaven_plugin_plotly_express.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-05-02 17:45:17.000000 deephaven-plugin-plotly-express-0.0.2/src/deephaven_plugin_plotly_express.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-05-02 17:45:17.000000 deephaven-plugin-plotly-express-0.0.2/src/deephaven_plugin_plotly_express.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-02 17:45:17.000000 deephaven-plugin-plotly-express-0.0.2/src/deephaven_plugin_plotly_express.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 20:51:50.075447 deephaven-plugin-plotly-express-0.0.3/
+-rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-05-05 20:51:40.000000 deephaven-plugin-plotly-express-0.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2075 2023-05-05 20:51:50.075447 deephaven-plugin-plotly-express-0.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1211 2023-05-05 20:51:40.000000 deephaven-plugin-plotly-express-0.0.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-05-05 20:51:40.000000 deephaven-plugin-plotly-express-0.0.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1170 2023-05-05 20:51:50.075447 deephaven-plugin-plotly-express-0.0.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 20:51:50.067447 deephaven-plugin-plotly-express-0.0.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 20:51:50.067447 deephaven-plugin-plotly-express-0.0.3/src/deephaven/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 20:51:50.067447 deephaven-plugin-plotly-express-0.0.3/src/deephaven/plot/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 20:51:50.071447 deephaven-plugin-plotly-express-0.0.3/src/deephaven/plot/express/
+-rw-r--r--   0 runner    (1001) docker     (123)     1030 2023-05-05 20:51:40.000000 deephaven-plugin-plotly-express-0.0.3/src/deephaven/plot/express/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 20:51:50.071447 deephaven-plugin-plotly-express-0.0.3/src/deephaven/plot/express/data_mapping/
+-rw-r--r--   0 runner    (1001) docker     (123)     1952 2023-05-05 20:51:40.000000 deephaven-plugin-plotly-express-0.0.3/src/deephaven/plot/express/data_mapping/DataMapping.py
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-05-05 20:51:40.000000 deephaven-plugin-plotly-express-0.0.3/src/deephaven/plot/express/data_mapping/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6383 2023-05-05 20:51:40.000000 deephaven-plugin-plotly-express-0.0.3/src/deephaven/plot/express/data_mapping/data_mapping.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2715 2023-05-05 20:51:40.000000 deephaven-plugin-plotly-express-0.0.3/src/deephaven/plot/express/data_mapping/json_conversion.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 20:51:50.071447 deephaven-plugin-plotly-express-0.0.3/src/deephaven/plot/express/deephaven_figure/
+-rw-r--r--   0 runner    (1001) docker     (123)     4962 2023-05-05 20:51:40.000000 deephaven-plugin-plotly-express-0.0.3/src/deephaven/plot/express/deephaven_figure/DeephavenFigure.py
+-rw-r--r--   0 runner    (1001) docker     (123)      166 2023-05-05 20:51:40.000000 deephaven-plugin-plotly-express-0.0.3/src/deephaven/plot/express/deephaven_figure/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3221 2023-05-05 20:51:40.000000 deephaven-plugin-plotly-express-0.0.3/src/deephaven/plot/express/deephaven_figure/custom_draw.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21657 2023-05-05 20:51:40.000000 deephaven-plugin-plotly-express-0.0.3/src/deephaven/plot/express/deephaven_figure/generate.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 20:51:50.075447 deephaven-plugin-plotly-express-0.0.3/src/deephaven/plot/express/plots/
+-rw-r--r--   0 runner    (1001) docker     (123)      467 2023-05-05 20:51:40.000000 deephaven-plugin-plotly-express-0.0.3/src/deephaven/plot/express/plots/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23555 2023-05-05 20:51:40.000000 deephaven-plugin-plotly-express-0.0.3/src/deephaven/plot/express/plots/_private_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5713 2023-05-05 20:51:40.000000 deephaven-plugin-plotly-express-0.0.3/src/deephaven/plot/express/plots/area.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12185 2023-05-05 20:51:40.000000 deephaven-plugin-plotly-express-0.0.3/src/deephaven/plot/express/plots/bar.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20355 2023-05-05 20:51:40.000000 deephaven-plugin-plotly-express-0.0.3/src/deephaven/plot/express/plots/distribution.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6331 2023-05-05 20:51:40.000000 deephaven-plugin-plotly-express-0.0.3/src/deephaven/plot/express/plots/financial.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10436 2023-05-05 20:51:40.000000 deephaven-plugin-plotly-express-0.0.3/src/deephaven/plot/express/plots/hierarchial.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16934 2023-05-05 20:51:40.000000 deephaven-plugin-plotly-express-0.0.3/src/deephaven/plot/express/plots/line.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2392 2023-05-05 20:51:40.000000 deephaven-plugin-plotly-express-0.0.3/src/deephaven/plot/express/plots/pie.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16874 2023-05-05 20:51:40.000000 deephaven-plugin-plotly-express-0.0.3/src/deephaven/plot/express/plots/scatter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7086 2023-05-05 20:51:40.000000 deephaven-plugin-plotly-express-0.0.3/src/deephaven/plot/express/plots/subplots.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 20:51:50.075447 deephaven-plugin-plotly-express-0.0.3/src/deephaven/plot/express/preprocess/
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-05 20:51:40.000000 deephaven-plugin-plotly-express-0.0.3/src/deephaven/plot/express/preprocess/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8791 2023-05-05 20:51:40.000000 deephaven-plugin-plotly-express-0.0.3/src/deephaven/plot/express/preprocess/preprocess.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 20:51:50.075447 deephaven-plugin-plotly-express-0.0.3/src/deephaven/plot/express/shared/
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-05-05 20:51:40.000000 deephaven-plugin-plotly-express-0.0.3/src/deephaven/plot/express/shared/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      962 2023-05-05 20:51:40.000000 deephaven-plugin-plotly-express-0.0.3/src/deephaven/plot/express/shared/shared.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 20:51:50.075447 deephaven-plugin-plotly-express-0.0.3/src/deephaven_plugin_plotly_express.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2075 2023-05-05 20:51:50.000000 deephaven-plugin-plotly-express-0.0.3/src/deephaven_plugin_plotly_express.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1575 2023-05-05 20:51:50.000000 deephaven-plugin-plotly-express-0.0.3/src/deephaven_plugin_plotly_express.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 20:51:50.000000 deephaven-plugin-plotly-express-0.0.3/src/deephaven_plugin_plotly_express.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-05-05 20:51:50.000000 deephaven-plugin-plotly-express-0.0.3/src/deephaven_plugin_plotly_express.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-05-05 20:51:50.000000 deephaven-plugin-plotly-express-0.0.3/src/deephaven_plugin_plotly_express.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-05 20:51:50.000000 deephaven-plugin-plotly-express-0.0.3/src/deephaven_plugin_plotly_express.egg-info/top_level.txt
```

### Comparing `deephaven-plugin-plotly-express-0.0.2/LICENSE` & `deephaven-plugin-plotly-express-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `deephaven-plugin-plotly-express-0.0.2/PKG-INFO` & `deephaven-plugin-plotly-express-0.0.3/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: deephaven-plugin-plotly-express
-Version: 0.0.2
+Version: 0.0.3
 Summary: Deephaven Chart Plugin
 Home-page: https://github.com/deephaven/deephaven-plugin-plotly-express
 Author: Devin Smith, Vlad Babich, Joe Numainville
 Author-email: josephnumainville@deephaven.io
 Project-URL: Source Code, https://github.com/deephaven/deephaven-plugin-plotly-express
 Project-URL: Bug Tracker, https://github.com/deephaven/deephaven-plugin-plotly-express/issues
 Keywords: deephaven,plugin,graph
```

### Comparing `deephaven-plugin-plotly-express-0.0.2/README.md` & `deephaven-plugin-plotly-express-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `deephaven-plugin-plotly-express-0.0.2/setup.cfg` & `deephaven-plugin-plotly-express-0.0.3/setup.cfg`

 * *Files identical despite different names*

### Comparing `deephaven-plugin-plotly-express-0.0.2/src/deephaven/plot/express/__init__.py` & `deephaven-plugin-plotly-express-0.0.3/src/deephaven/plot/express/__init__.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,17 +2,17 @@
 from deephaven.plugin.object import Exporter, ObjectType
 
 from .deephaven_figure import DeephavenFigure, export_figure
 
 from .plots import area, bar, frequency_bar, timeline, histogram, _ecdf, box, \
     violin, strip, ohlc, candlestick, treemap, sunburst, icicle, funnel, \
     funnel_area, line, line_polar, line_ternary, line_3d, scatter, scatter_3d, \
-    scatter_polar, scatter_ternary, pie, layer
+    scatter_polar, scatter_ternary, pie, layer, make_subplots
 
-__version__ = "0.0.2"
+__version__ = "0.0.3"
 
 NAME = "deephaven.plot.express.DeephavenFigure"
 
 
 class DeephavenFigureType(ObjectType):
     @property
     def name(self) -> str:
```

### Comparing `deephaven-plugin-plotly-express-0.0.2/src/deephaven/plot/express/data_mapping/DataMapping.py` & `deephaven-plugin-plotly-express-0.0.3/src/deephaven/plot/express/data_mapping/DataMapping.py`

 * *Files identical despite different names*

### Comparing `deephaven-plugin-plotly-express-0.0.2/src/deephaven/plot/express/data_mapping/data_mapping.py` & `deephaven-plugin-plotly-express-0.0.3/src/deephaven/plot/express/data_mapping/data_mapping.py`

 * *Files identical despite different names*

### Comparing `deephaven-plugin-plotly-express-0.0.2/src/deephaven/plot/express/data_mapping/json_conversion.py` & `deephaven-plugin-plotly-express-0.0.3/src/deephaven/plot/express/data_mapping/json_conversion.py`

 * *Files identical despite different names*

### Comparing `deephaven-plugin-plotly-express-0.0.2/src/deephaven/plot/express/deephaven_figure/DeephavenFigure.py` & `deephaven-plugin-plotly-express-0.0.3/src/deephaven/plot/express/deephaven_figure/DeephavenFigure.py`

 * *Files 4% similar despite different names*

```diff
@@ -74,15 +74,16 @@
             fig: Figure = None,
             call: Callable = None,
             call_args: dict[any] = None,
             data_mappings: list[DataMapping] = None,
             has_template: str = None,
             has_color: bool = False,
             trace_generator: Generator[dict[str, any]] = None,
-            has_subplots: bool = False
+            has_subplots: bool = False,
+            subplot_specs: list[dict] = None
     ):
         """
         Initialize a DeephavenFigure
 
         :param fig: The underlying plotly fig
         :param call_args: The arguments that were used to call px
         :param call: The (usually) px drawing function
```

### Comparing `deephaven-plugin-plotly-express-0.0.2/src/deephaven/plot/express/deephaven_figure/custom_draw.py` & `deephaven-plugin-plotly-express-0.0.3/src/deephaven/plot/express/deephaven_figure/custom_draw.py`

 * *Files identical despite different names*

### Comparing `deephaven-plugin-plotly-express-0.0.2/src/deephaven/plot/express/deephaven_figure/generate.py` & `deephaven-plugin-plotly-express-0.0.3/src/deephaven/plot/express/deephaven_figure/generate.py`

 * *Files identical despite different names*

### Comparing `deephaven-plugin-plotly-express-0.0.2/src/deephaven/plot/express/plots/_private_utils.py` & `deephaven-plugin-plotly-express-0.0.3/src/deephaven/plot/express/plots/_private_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from functools import partial
+from itertools import chain
 from typing import Callable
-from collections.abc import Generator
+from collections.abc import Generator, Iterator
 
 from plotly import subplots
 from plotly.graph_objects import Figure
 
 from deephaven.table import Table
 
 from ..deephaven_figure import generate_figure, DeephavenFigure, update_traces
@@ -370,25 +371,25 @@
     if not which_layout or which_layout == i:
         fig_layout.update(fig.to_dict()['layout'])
 
     return fig.data, fig_layout
 
 
 def layer(
-        *args: DeephavenFigure | Figure,
+        *figs: DeephavenFigure | Figure,
         which_layout: int = None,
         specs: list[dict[str, any]] = None,
         unsafe_update_figure: Callable = default_callback
 ) -> DeephavenFigure:
     """
     Layers the provided figures. Be default, the layouts are sequentially
     applied, so the layouts of later figures will override the layouts of early
     figures.
 
-    :param args: The charts to layer
+    :param figs: The charts to layer
     :param which_layout: None to layer layouts, or an index of which arg to
     take the layout from. Currently only valid if domains are not specified.
     :param specs: A list of dictionaries that contain keys of "x" and "y"
     that have values that are lists of two floats from 0 to 1. The chart that
     corresponds with a domain will be resized to that domain. Either x or y can
     be excluded if only resizing on one axis. Can also specify xaxis_update or
     yaxis_update with a dictionary value to update all axes with that dict.
@@ -396,15 +397,15 @@
     as an argument and optionally returns a plotly figure. If a figure is not
     returned, the plotly figure passed will be assumed to be the return value.
     Used to add any custom changes to the underlying plotly figure. Note that
     the existing data traces should not be removed. This may lead to unexpected
     behavior if traces are modified in a way that break data mappings.
     :return: The layered chart
     """
-    if len(args) == 0:
+    if len(figs) == 0:
         raise ValueError("No figures provided to compose")
 
     new_data = []
     new_layout = {}
     new_data_mappings = []
     new_has_template = False
     new_has_color = False
@@ -414,16 +415,19 @@
         "xaxis": 1,
         "yaxis": 1,
         "scene": 1,
         "polar": 1,
         "ternary": 1
     }
 
-    for i, arg in enumerate(args):
-        if isinstance(arg, Figure):
+    for i, arg in enumerate(figs):
+        if not arg:
+            continue
+
+        elif isinstance(arg, Figure):
             fig_data, fig_layout = fig_data_and_layout(
                 arg, i, specs, which_layout, new_axes_start
             )
 
         elif isinstance(arg, DeephavenFigure):
             offset = len(new_data)
             if arg.has_subplots:
@@ -685,17 +689,8 @@
 
     update_legend_and_titles(
         layered, var, cols, is_list,
         list_var_axis_name, list_val_axis_name,
         str_var_axis_name, str_val_axis_name
     )
 
-    return layered
-
-
-def _make_subplots(
-        rows=1,
-        cols=1
-):
-    # todo: not yet implemented
-    new_fig = subplots.make_subplots(rows=rows, cols=cols)
-    return DeephavenFigure(new_fig)
+    return layered
```

### Comparing `deephaven-plugin-plotly-express-0.0.2/src/deephaven/plot/express/plots/area.py` & `deephaven-plugin-plotly-express-0.0.3/src/deephaven/plot/express/plots/area.py`

 * *Files identical despite different names*

### Comparing `deephaven-plugin-plotly-express-0.0.2/src/deephaven/plot/express/plots/bar.py` & `deephaven-plugin-plotly-express-0.0.3/src/deephaven/plot/express/plots/bar.py`

 * *Files identical despite different names*

### Comparing `deephaven-plugin-plotly-express-0.0.2/src/deephaven/plot/express/plots/distribution.py` & `deephaven-plugin-plotly-express-0.0.3/src/deephaven/plot/express/plots/distribution.py`

 * *Files identical despite different names*

### Comparing `deephaven-plugin-plotly-express-0.0.2/src/deephaven/plot/express/plots/financial.py` & `deephaven-plugin-plotly-express-0.0.3/src/deephaven/plot/express/plots/financial.py`

 * *Files identical despite different names*

### Comparing `deephaven-plugin-plotly-express-0.0.2/src/deephaven/plot/express/plots/hierarchial.py` & `deephaven-plugin-plotly-express-0.0.3/src/deephaven/plot/express/plots/hierarchial.py`

 * *Files identical despite different names*

### Comparing `deephaven-plugin-plotly-express-0.0.2/src/deephaven/plot/express/plots/line.py` & `deephaven-plugin-plotly-express-0.0.3/src/deephaven/plot/express/plots/line.py`

 * *Files identical despite different names*

### Comparing `deephaven-plugin-plotly-express-0.0.2/src/deephaven/plot/express/plots/pie.py` & `deephaven-plugin-plotly-express-0.0.3/src/deephaven/plot/express/plots/pie.py`

 * *Files identical despite different names*

### Comparing `deephaven-plugin-plotly-express-0.0.2/src/deephaven/plot/express/plots/scatter.py` & `deephaven-plugin-plotly-express-0.0.3/src/deephaven/plot/express/plots/scatter.py`

 * *Files identical despite different names*

### Comparing `deephaven-plugin-plotly-express-0.0.2/src/deephaven/plot/express/preprocess/preprocess.py` & `deephaven-plugin-plotly-express-0.0.3/src/deephaven/plot/express/preprocess/preprocess.py`

 * *Files identical despite different names*

### Comparing `deephaven-plugin-plotly-express-0.0.2/src/deephaven/plot/express/shared/shared.py` & `deephaven-plugin-plotly-express-0.0.3/src/deephaven/plot/express/shared/shared.py`

 * *Files identical despite different names*

### Comparing `deephaven-plugin-plotly-express-0.0.2/src/deephaven_plugin_plotly_express.egg-info/PKG-INFO` & `deephaven-plugin-plotly-express-0.0.3/src/deephaven_plugin_plotly_express.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: deephaven-plugin-plotly-express
-Version: 0.0.2
+Version: 0.0.3
 Summary: Deephaven Chart Plugin
 Home-page: https://github.com/deephaven/deephaven-plugin-plotly-express
 Author: Devin Smith, Vlad Babich, Joe Numainville
 Author-email: josephnumainville@deephaven.io
 Project-URL: Source Code, https://github.com/deephaven/deephaven-plugin-plotly-express
 Project-URL: Bug Tracker, https://github.com/deephaven/deephaven-plugin-plotly-express/issues
 Keywords: deephaven,plugin,graph
```

### Comparing `deephaven-plugin-plotly-express-0.0.2/src/deephaven_plugin_plotly_express.egg-info/SOURCES.txt` & `deephaven-plugin-plotly-express-0.0.3/src/deephaven_plugin_plotly_express.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -17,14 +17,15 @@
 src/deephaven/plot/express/plots/bar.py
 src/deephaven/plot/express/plots/distribution.py
 src/deephaven/plot/express/plots/financial.py
 src/deephaven/plot/express/plots/hierarchial.py
 src/deephaven/plot/express/plots/line.py
 src/deephaven/plot/express/plots/pie.py
 src/deephaven/plot/express/plots/scatter.py
+src/deephaven/plot/express/plots/subplots.py
 src/deephaven/plot/express/preprocess/__init__.py
 src/deephaven/plot/express/preprocess/preprocess.py
 src/deephaven/plot/express/shared/__init__.py
 src/deephaven/plot/express/shared/shared.py
 src/deephaven_plugin_plotly_express.egg-info/PKG-INFO
 src/deephaven_plugin_plotly_express.egg-info/SOURCES.txt
 src/deephaven_plugin_plotly_express.egg-info/dependency_links.txt
```

