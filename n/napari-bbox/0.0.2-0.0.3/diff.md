# Comparing `tmp/napari-bbox-0.0.2.tar.gz` & `tmp/napari-bbox-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "napari-bbox-0.0.2.tar", last modified: Fri Mar 24 12:56:32 2023, max compression
+gzip compressed data, was "napari-bbox-0.0.3.tar", last modified: Fri May  5 13:43:51 2023, max compression
```

## Comparing `napari-bbox-0.0.2.tar` & `napari-bbox-0.0.3.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 12:56:32.608511 napari-bbox-0.0.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1486 2023-03-24 12:56:24.000000 napari-bbox-0.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-03-24 12:56:24.000000 napari-bbox-0.0.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4244 2023-03-24 12:56:32.608511 napari-bbox-0.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3016 2023-03-24 12:56:24.000000 napari-bbox-0.0.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      180 2023-03-24 12:56:24.000000 napari-bbox-0.0.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1643 2023-03-24 12:56:32.608511 napari-bbox-0.0.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 12:56:32.604510 napari-bbox-0.0.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 12:56:32.604510 napari-bbox-0.0.2/src/napari_bbox/
--rw-r--r--   0 runner    (1001) docker     (123)     1009 2023-03-24 12:56:24.000000 napari-bbox-0.0.2/src/napari_bbox/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2854 2023-03-24 12:56:24.000000 napari-bbox-0.0.2/src/napari_bbox/_reader.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 12:56:32.608511 napari-bbox-0.0.2/src/napari_bbox/_tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-24 12:56:24.000000 napari-bbox-0.0.2/src/napari_bbox/_tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      971 2023-03-24 12:56:24.000000 napari-bbox-0.0.2/src/napari_bbox/_tests/test_reader.py
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-24 12:56:24.000000 napari-bbox-0.0.2/src/napari_bbox/_tests/test_widget.py
--rw-r--r--   0 runner    (1001) docker     (123)      120 2023-03-24 12:56:24.000000 napari-bbox-0.0.2/src/napari_bbox/_tests/test_writer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2829 2023-03-24 12:56:24.000000 napari-bbox-0.0.2/src/napari_bbox/_widget.py
--rw-r--r--   0 runner    (1001) docker     (123)      736 2023-03-24 12:56:24.000000 napari-bbox-0.0.2/src/napari_bbox/_writer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 12:56:32.608511 napari-bbox-0.0.2/src/napari_bbox/boundingbox/
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-03-24 12:56:24.000000 napari-bbox-0.0.2/src/napari_bbox/boundingbox/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1463 2023-03-24 12:56:24.000000 napari-bbox-0.0.2/src/napari_bbox/boundingbox/_bounding_box_constants.py
--rw-r--r--   0 runner    (1001) docker     (123)    32971 2023-03-24 12:56:24.000000 napari-bbox-0.0.2/src/napari_bbox/boundingbox/_bounding_box_list.py
--rw-r--r--   0 runner    (1001) docker     (123)    11632 2023-03-24 12:56:24.000000 napari-bbox-0.0.2/src/napari_bbox/boundingbox/_bounding_box_mouse_bindings.py
--rw-r--r--   0 runner    (1001) docker     (123)    35308 2023-03-24 12:56:24.000000 napari-bbox-0.0.2/src/napari_bbox/boundingbox/_bounding_box_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      986 2023-03-24 12:56:24.000000 napari-bbox-0.0.2/src/napari_bbox/boundingbox/_bounding_boxes_key_bindings.py
--rw-r--r--   0 runner    (1001) docker     (123)     3145 2023-03-24 12:56:24.000000 napari-bbox-0.0.2/src/napari_bbox/boundingbox/_mesh.py
--rw-r--r--   0 runner    (1001) docker     (123)    15282 2023-03-24 12:56:24.000000 napari-bbox-0.0.2/src/napari_bbox/boundingbox/bounding_box.py
--rw-r--r--   0 runner    (1001) docker     (123)    81191 2023-03-24 12:56:24.000000 napari-bbox-0.0.2/src/napari_bbox/boundingbox/bounding_boxes.py
--rw-r--r--   0 runner    (1001) docker     (123)    20179 2023-03-24 12:56:24.000000 napari-bbox-0.0.2/src/napari_bbox/boundingbox/qt_bounding_box_control.py
--rw-r--r--   0 runner    (1001) docker     (123)     5439 2023-03-24 12:56:24.000000 napari-bbox-0.0.2/src/napari_bbox/boundingbox/vispy_bounding_box_layer.py
--rw-r--r--   0 runner    (1001) docker     (123)      593 2023-03-24 12:56:24.000000 napari-bbox-0.0.2/src/napari_bbox/napari.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-24 12:56:32.608511 napari-bbox-0.0.2/src/napari_bbox.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4244 2023-03-24 12:56:32.000000 napari-bbox-0.0.2/src/napari_bbox.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1130 2023-03-24 12:56:32.000000 napari-bbox-0.0.2/src/napari_bbox.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-24 12:56:32.000000 napari-bbox-0.0.2/src/napari_bbox.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-03-24 12:56:32.000000 napari-bbox-0.0.2/src/napari_bbox.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-03-24 12:56:32.000000 napari-bbox-0.0.2/src/napari_bbox.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-03-24 12:56:32.000000 napari-bbox-0.0.2/src/napari_bbox.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 13:43:51.099442 napari-bbox-0.0.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1486 2023-05-05 13:43:41.000000 napari-bbox-0.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-05 13:43:41.000000 napari-bbox-0.0.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4119 2023-05-05 13:43:51.099442 napari-bbox-0.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2891 2023-05-05 13:43:41.000000 napari-bbox-0.0.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      180 2023-05-05 13:43:41.000000 napari-bbox-0.0.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1659 2023-05-05 13:43:51.099442 napari-bbox-0.0.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 13:43:51.091442 napari-bbox-0.0.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 13:43:51.091442 napari-bbox-0.0.3/src/napari_bbox/
+-rw-r--r--   0 runner    (1001) docker     (123)     1483 2023-05-05 13:43:41.000000 napari-bbox-0.0.3/src/napari_bbox/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2854 2023-05-05 13:43:41.000000 napari-bbox-0.0.3/src/napari_bbox/_reader.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 13:43:51.095442 napari-bbox-0.0.3/src/napari_bbox/_tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 13:43:41.000000 napari-bbox-0.0.3/src/napari_bbox/_tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      971 2023-05-05 13:43:41.000000 napari-bbox-0.0.3/src/napari_bbox/_tests/test_reader.py
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 13:43:41.000000 napari-bbox-0.0.3/src/napari_bbox/_tests/test_widget.py
+-rw-r--r--   0 runner    (1001) docker     (123)      120 2023-05-05 13:43:41.000000 napari-bbox-0.0.3/src/napari_bbox/_tests/test_writer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2829 2023-05-05 13:43:41.000000 napari-bbox-0.0.3/src/napari_bbox/_widget.py
+-rw-r--r--   0 runner    (1001) docker     (123)      736 2023-05-05 13:43:41.000000 napari-bbox-0.0.3/src/napari_bbox/_writer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 13:43:51.099442 napari-bbox-0.0.3/src/napari_bbox/boundingbox/
+-rw-r--r--   0 runner    (1001) docker     (123)      122 2023-05-05 13:43:41.000000 napari-bbox-0.0.3/src/napari_bbox/boundingbox/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1463 2023-05-05 13:43:41.000000 napari-bbox-0.0.3/src/napari_bbox/boundingbox/_bounding_box_constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33046 2023-05-05 13:43:41.000000 napari-bbox-0.0.3/src/napari_bbox/boundingbox/_bounding_box_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11648 2023-05-05 13:43:41.000000 napari-bbox-0.0.3/src/napari_bbox/boundingbox/_bounding_box_mouse_bindings.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35308 2023-05-05 13:43:41.000000 napari-bbox-0.0.3/src/napari_bbox/boundingbox/_bounding_box_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2228 2023-05-05 13:43:41.000000 napari-bbox-0.0.3/src/napari_bbox/boundingbox/_bounding_boxes_key_bindings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3145 2023-05-05 13:43:41.000000 napari-bbox-0.0.3/src/napari_bbox/boundingbox/_mesh.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15773 2023-05-05 13:43:41.000000 napari-bbox-0.0.3/src/napari_bbox/boundingbox/bounding_box.py
+-rw-r--r--   0 runner    (1001) docker     (123)    81060 2023-05-05 13:43:41.000000 napari-bbox-0.0.3/src/napari_bbox/boundingbox/bounding_boxes.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20680 2023-05-05 13:43:41.000000 napari-bbox-0.0.3/src/napari_bbox/boundingbox/qt_bounding_box_control.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5562 2023-05-05 13:43:41.000000 napari-bbox-0.0.3/src/napari_bbox/boundingbox/vispy_bounding_box_layer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      593 2023-05-05 13:43:41.000000 napari-bbox-0.0.3/src/napari_bbox/napari.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 13:43:51.095442 napari-bbox-0.0.3/src/napari_bbox.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4119 2023-05-05 13:43:51.000000 napari-bbox-0.0.3/src/napari_bbox.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1130 2023-05-05 13:43:51.000000 napari-bbox-0.0.3/src/napari_bbox.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 13:43:51.000000 napari-bbox-0.0.3/src/napari_bbox.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-05-05 13:43:51.000000 napari-bbox-0.0.3/src/napari_bbox.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-05-05 13:43:51.000000 napari-bbox-0.0.3/src/napari_bbox.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-05 13:43:51.000000 napari-bbox-0.0.3/src/napari_bbox.egg-info/top_level.txt
```

### Comparing `napari-bbox-0.0.2/LICENSE` & `napari-bbox-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `napari-bbox-0.0.2/PKG-INFO` & `napari-bbox-0.0.3/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: napari-bbox
-Version: 0.0.2
+Version: 0.0.3
 Summary: A new layer for bounding boxes in 2+ dimensions
 Home-page: https://github.com/bauerdavid/napari-bbox
 Author: David Bauer
 Author-email: dbauer@brc.hu
 License: BSD-3-Clause
 Project-URL: Bug Tracker, https://github.com/bauerdavid/napari-bbox/issues
 Project-URL: Documentation, https://github.com/bauerdavid/napari-bbox#README.md
@@ -36,16 +36,14 @@
 [![codecov](https://codecov.io/gh/bauerdavid/napari-bbox/branch/main/graph/badge.svg)](https://codecov.io/gh/bauerdavid/napari-bbox)
 [![napari hub](https://img.shields.io/endpoint?url=https://api.napari-hub.org/shields/napari-bbox)](https://napari-hub.org/plugins/napari-bbox)
 
 A new layer for bounding boxes in 2+ dimensions
 
 > **Note**: This plugin was originally part of [Annotation Toolbox](https://www.napari-hub.org/plugins/napari-nD-annotator), and was separated to allow other plugins to utilize it.
 
-> **Note**: Currently the plugin does not support `napari==0.4.17`, see https://github.com/bauerdavid/napari-bbox/issues/4.
-
 ----------------------------------
 
 ## Demo
 
 
 https://user-images.githubusercontent.com/36735863/227506511-d672ce5c-eab5-436f-a7fd-6080e118a9a8.mp4
```

### Comparing `napari-bbox-0.0.2/README.md` & `napari-bbox-0.0.3/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -7,16 +7,14 @@
 [![codecov](https://codecov.io/gh/bauerdavid/napari-bbox/branch/main/graph/badge.svg)](https://codecov.io/gh/bauerdavid/napari-bbox)
 [![napari hub](https://img.shields.io/endpoint?url=https://api.napari-hub.org/shields/napari-bbox)](https://napari-hub.org/plugins/napari-bbox)
 
 A new layer for bounding boxes in 2+ dimensions
 
 > **Note**: This plugin was originally part of [Annotation Toolbox](https://www.napari-hub.org/plugins/napari-nD-annotator), and was separated to allow other plugins to utilize it.
 
-> **Note**: Currently the plugin does not support `napari==0.4.17`, see https://github.com/bauerdavid/napari-bbox/issues/4.
-
 ----------------------------------
 
 ## Demo
 
 
 https://user-images.githubusercontent.com/36735863/227506511-d672ce5c-eab5-436f-a7fd-6080e118a9a8.mp4
```

### Comparing `napari-bbox-0.0.2/setup.cfg` & `napari-bbox-0.0.3/setup.cfg`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = napari-bbox
-version = 0.0.2
+version = 0.0.3
 description = A new layer for bounding boxes in 2+ dimensions
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/bauerdavid/napari-bbox
 author = David Bauer
 author_email = dbauer@brc.hu
 license = BSD-3-Clause
@@ -30,14 +30,15 @@
 
 [options]
 packages = find:
 install_requires = 
 	numpy
 	magicgui
 	qtpy
+	napari>=0.4.15
 python_requires = >=3.8
 include_package_data = True
 package_dir = 
 	=src
 
 [options.packages.find]
 where = src
```

### Comparing `napari-bbox-0.0.2/src/napari_bbox/__init__.py` & `napari-bbox-0.0.3/src/napari_bbox/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,13 +1,16 @@
-__version__ = "0.0.2"
+__version__ = "0.0.3"
+
+from napari import layers
+layers.NAMES.add("bounding_boxes")
 
-from napari.layers import NAMES
-NAMES.add("bounding_boxes")
 from napari import types
 types.Bounding_BoxesData = types.NewType("Bounding_BoxesData", types.ArrayBase)
+
+
 from .boundingbox import BoundingBoxLayer
 from ._reader import napari_get_reader
 from ._writer import write_single_bbox
 
 from ._widget import BoundingBoxCreator
 
 from napari import Viewer
@@ -28,9 +31,20 @@
     shapes = "shapes"
     surface = "surface"
     tracks = "tracks"
     vectors = "vectors"
     bounding_boxes = "bounding_boxes"
 
 
-npe2.manifest.contributions._writers.LayerType = LayerType
+# npe2.manifest.contributions._writers.LayerType = LayerType
+
+# This is an ugly solution to register every component correctly
+from .boundingbox.qt_bounding_box_control import register_layer_control
+from .boundingbox.vispy_bounding_box_layer import register_layer_visual
+register_layer_control(BoundingBoxLayer)
+register_layer_visual(BoundingBoxLayer)
+# register_bounding_boxes_actions(BoundingBoxLayer)
+import sys
+layers.__dict__["BoundingBoxLayer"] = BoundingBoxLayer
+layers.__dict__["bounding_boxes"] = sys.modules[__name__]
+
 __all__ = ["BoundingBoxCreator", "BoundingBoxLayer", "napari_get_reader", "write_single_bbox"]
```

### Comparing `napari-bbox-0.0.2/src/napari_bbox/_reader.py` & `napari-bbox-0.0.3/src/napari_bbox/_reader.py`

 * *Files identical despite different names*

### Comparing `napari-bbox-0.0.2/src/napari_bbox/_tests/test_reader.py` & `napari-bbox-0.0.3/src/napari_bbox/_tests/test_reader.py`

 * *Files identical despite different names*

### Comparing `napari-bbox-0.0.2/src/napari_bbox/_widget.py` & `napari-bbox-0.0.3/src/napari_bbox/_widget.py`

 * *Files identical despite different names*

### Comparing `napari-bbox-0.0.2/src/napari_bbox/_writer.py` & `napari-bbox-0.0.3/src/napari_bbox/_writer.py`

 * *Files identical despite different names*

### Comparing `napari-bbox-0.0.2/src/napari_bbox/boundingbox/_bounding_box_constants.py` & `napari-bbox-0.0.3/src/napari_bbox/boundingbox/_bounding_box_constants.py`

 * *Files identical despite different names*

### Comparing `napari-bbox-0.0.2/src/napari_bbox/boundingbox/_bounding_box_list.py` & `napari-bbox-0.0.3/src/napari_bbox/boundingbox/_bounding_box_list.py`

 * *Files 0% similar despite different names*

```diff
@@ -176,14 +176,16 @@
         if not np.all(self._slice_key == slice_key):
             self._slice_key = slice_key
             self._update_displayed()
 
     def _update_displayed(self):
         """Update the displayed data based on the slice key."""
         slice_key = np.array(self.slice_key)
+        if len(slice_key) != self.slice_keys.shape[-1]:
+            return
         if len(self.bounding_boxes) > 0:
             self._displayed = np.all(np.logical_and(self.slice_keys[:, 0, :] <= slice_key, slice_key <= self.slice_keys[:, 1, :]), axis=1)
         else:
             self._displayed = []
         disp_indices = np.where(self._displayed)[0]
 
         z_order = self._mesh.triangles_z_order
```

### Comparing `napari-bbox-0.0.2/src/napari_bbox/boundingbox/_bounding_box_mouse_bindings.py` & `napari-bbox-0.0.3/src/napari_bbox/boundingbox/_bounding_box_mouse_bindings.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 
     Once selected bounding boxes can be moved or resized, and vertices can be moved
     depending on the mode. Holding shift when resizing a bounding box will preserve
     the aspect ratio.
     """
     shift = 'Shift' in event.modifiers
     # on press
-    value = layer.get_value(event.position, world=True)
+    value = layer.get_value(event.position, world=True) or (None, None)
     layer._moving_value = copy(value)
     bounding_box_under_cursor, vertex_under_cursor = value
     if vertex_under_cursor is None:
         if shift and bounding_box_under_cursor is not None:
             if bounding_box_under_cursor in layer.selected_data:
                 layer.selected_data.remove(bounding_box_under_cursor)
             else:
```

### Comparing `napari-bbox-0.0.2/src/napari_bbox/boundingbox/_bounding_box_utils.py` & `napari-bbox-0.0.3/src/napari_bbox/boundingbox/_bounding_box_utils.py`

 * *Files identical despite different names*

### Comparing `napari-bbox-0.0.2/src/napari_bbox/boundingbox/_mesh.py` & `napari-bbox-0.0.3/src/napari_bbox/boundingbox/_mesh.py`

 * *Files identical despite different names*

### Comparing `napari-bbox-0.0.2/src/napari_bbox/boundingbox/bounding_box.py` & `napari-bbox-0.0.3/src/napari_bbox/boundingbox/bounding_box.py`

 * *Files 1% similar despite different names*

```diff
@@ -131,42 +131,49 @@
         self._data = data
         self._update_displayed_data()
 
     def _update_displayed_data(self):
         """Update the data that is to be displayed."""
         # Add four boundary lines and then two triangles for each
 
-
         if self.ndisplay == 2:
             self._set_meshes(self.data_displayed, face=False)
             self._face_vertices = self.data_displayed
             self._face_triangles = np.array([[0, 1, 2], [0, 2, 3]])
         else:
-            ordered_vertices = self.data_displayed[
-                [
-                    0, 1, 3, 2, 0, 4, 6, 2, 3, 7, 6, 4, 5, 7, 3, 1, 5
+            if len(self.data_displayed) == 4:
+                ordered_vertices = self.data_displayed[[0, 1, 3, 2, 0]]
+                self._set_meshes(ordered_vertices, closed=False, face=False)
+                self._face_triangles = np.array([
+                    [0, 1, 2],
+                    [2, 3, 1],
+                ])
+                self._face_vertices = self.data_displayed
+            else:
+                ordered_vertices = self.data_displayed[
+                    [0, 1, 3, 2, 0, 4, 6, 2, 3, 7, 6, 4, 5, 7, 3, 1, 5]
                 ]
-            ]
-            self._set_meshes(ordered_vertices, closed=False, face=False)
-            self._face_triangles = np.array([[0, 0, 0]])
-            # self._face_triangles = np.array([
-            #     [0, 1, 2],
-            #     [2, 3, 1],
-            #     [0, 4, 1],
-            #     [1, 4, 5],
-            #     [0, 2, 6],
-            #     [0, 6, 4],
-            #     [7, 4, 6],
-            #     [7, 5, 4],
-            #     [7, 6, 2],
-            #     [7, 2, 3],
-            #     [7, 3, 1],
-            #     [7, 1, 5]
-            # ])
+                self._set_meshes(ordered_vertices, closed=False, face=False)
+                # self._face_triangles = np.array([
+                #     [0, 1, 2],
+                #     [2, 1, 3],
+                #     [0, 4, 1],
+                #     [1, 4, 5],
+                #     [0, 2, 6],
+                #     [0, 6, 4],
+                #     [7, 4, 6],
+                #     [7, 5, 4],
+                #     [7, 6, 2],
+                #     [7, 2, 3],
+                #     [7, 3, 1],
+                #     [7, 1, 5]
+                # ])
             # self._face_triangles = np.append(self._face_triangles, np.fliplr(self._face_triangles), 0)
+            # self._face_vertices = self.data_displayed
+            self._face_triangles = np.array([[0, 0, 0]])
 
         if self.ndisplay == 2:
             self._box = rectangle_to_box(self.data_displayed)
 
         data_not_displayed = self.data[:, self.dims_not_displayed]
         self.slice_key = np.round(
             [
```

### Comparing `napari-bbox-0.0.2/src/napari_bbox/boundingbox/bounding_boxes.py` & `napari-bbox-0.0.3/src/napari_bbox/boundingbox/bounding_boxes.py`

 * *Files 0% similar despite different names*

```diff
@@ -66,15 +66,14 @@
                  rotate=None,
                  shear=None,
                  affine=None,
                  opacity=0.7,
                  blending='translucent',
                  visible=True,
     ):
-        print("constructor")
         if data is None:
             if ndim is None:
                 ndim = 2
             data = np.empty((0, 2, ndim))
         else:
             data = np.asarray(data)
             data_ndim = data.shape[-1]
@@ -703,14 +702,20 @@
         return len(self._data_view.bounding_boxes)
 
     @property
     def _indices_view(self):
         return np.where(self._data_view._displayed)[0]
 
     @property
+    def _view_text_color(self) -> np.ndarray:
+        """Get the colors of the text elements at the given indices."""
+        self.text.color._apply(self.features)
+        return self.text._view_color(self._indices_view)
+
+    @property
     def mode(self):
         """MODE: Interactive mode. The normal, default mode is PAN_ZOOM, which
         allows for normal interactivity with the canvas.
 
         The SELECT mode allows for entire bounding boxes to be selected, moved and
         resized.
 
@@ -2100,16 +2105,7 @@
             if self._ndisplay == 3:
                 self.editable = False
             else:
                 self.editable = True
 
         if not self.editable:
             self.mode = Mode.PAN_ZOOM
-
-
-# This is an ugly solution to register every component correctly
-register_layer_control(BoundingBoxLayer)
-register_layer_visual(BoundingBoxLayer)
-# register_bounding_boxes_actions(BoundingBoxLayer)
-import sys
-napari.layers.__dict__["BoundingBoxLayer"] = BoundingBoxLayer
-napari.layers.__dict__["bounding_boxes"] = sys.modules[__name__]
```

### Comparing `napari-bbox-0.0.2/src/napari_bbox/boundingbox/qt_bounding_box_control.py` & `napari-bbox-0.0.3/src/napari_bbox/boundingbox/qt_bounding_box_control.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 # A copy of napari._qt.layer_controls.qt_shapes_controls
 from typing import Iterable
 
 import napari
 from napari._qt.widgets.qt_color_swatch import QColorSwatchEdit
 from napari.utils.action_manager import action_manager
+from packaging import version
 from qtpy.QtCore import Qt
 from qtpy.QtWidgets import QButtonGroup, QGridLayout, QLabel, QHBoxLayout, QCheckBox, QComboBox
 from napari._qt.widgets._slider_compat import QDoubleSlider, QSlider
 from napari._qt.layer_controls.qt_layer_controls_base import QtLayerControls
 import numpy as np
 from napari._qt.utils import qt_signals_blocked, disable_with_opacity
 from napari._qt.widgets.qt_mode_buttons import QtModeRadioButton, QtModePushButton
@@ -233,18 +234,24 @@
         self._on_current_face_color_change()
         self.edgeColorEdit = QColorSwatchEdit(
             initial_color=self.layer.current_edge_color,
             tooltip=trans._('click to set current edge color'),
         )
         self._on_current_edge_color_change()
 
-        self.textColorEdit = QColorSwatchEdit(
-            initial_color=self.layer.text.color,
-            tooltip=trans._('click to set current text color'),
-        )
+        if version.parse(napari.__version__) < version.parse("0.4.17"):
+            self.textColorEdit = QColorSwatchEdit(
+                initial_color=self.layer.text.color,
+                tooltip=trans._('click to set current text color'),
+            )
+        else:
+            self.textColorEdit = QColorSwatchEdit(
+                initial_color=self.layer.text.color.constant,
+                tooltip=trans._('click to set current text color'),
+            )
         self._on_current_text_color_change()
 
         self.faceColorEdit.color_changed.connect(self.changeFaceColor)
         self.edgeColorEdit.color_changed.connect(self.changeEdgeColor)
         self.textColorEdit.color_changed.connect(self.changeTextColor)
 
         text_disp_cb = QCheckBox()
@@ -457,15 +464,18 @@
 
         Parameters
         ----------
         event : napari.utils.event.Event, optional
             The napari event that triggered this method, by default None.
         """
         with qt_signals_blocked(self.textColorEdit):
-            self.textColorEdit.setColor(self.layer.text.color)
+            if version.parse(napari.__version__) < version.parse("0.4.17"):
+                self.textColorEdit.setColor(self.layer.text.color)
+            else:
+                self.textColorEdit.setColor(self.layer.text.color.constant)
 
     def _on_editable_change(self, event=None):
         """Receive layer model editable change event & enable/disable buttons.
 
         Parameters
         ----------
         event : napari.utils.event.Event, optional
```

### Comparing `napari-bbox-0.0.2/src/napari_bbox/boundingbox/vispy_bounding_box_layer.py` & `napari-bbox-0.0.3/src/napari_bbox/boundingbox/vispy_bounding_box_layer.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 # A copy of napari._vispy.layers.shapes
 import numpy as np
+import vispy
 from napari._vispy.layers.base import VispyBaseLayer
 from napari._vispy.utils.text import update_text
 from napari.utils.events import disconnect_events
 from napari.settings import get_settings
+from packaging import version
 from vispy.scene import Compound, Mesh, Line, Markers, Text
 
 
 class VispyBoundingBoxLayer(VispyBaseLayer):
     def __init__(self, layer):
         # Create a compound visual with the following four subvisuals:
         # Markers: corresponding to the vertices of the interaction box or the
@@ -94,15 +96,15 @@
         self.node._subvisuals[3].set_data(
             vertices,
             size=size,
             face_color=face_color,
             edge_color=edge_color,
             edge_width=width,
             symbol='square',
-            scaling=False,
+            **({"scaling": False} if version.parse(vispy.__version__) <= version.parse("0.11.0") else {}),
         )
 
         if pos is None or len(pos) == 0:
             pos = np.zeros((1, self.layer._ndisplay))
             width = 0
 
         self.node._subvisuals[2].set_data(
```

### Comparing `napari-bbox-0.0.2/src/napari_bbox/napari.yaml` & `napari-bbox-0.0.3/src/napari_bbox/napari.yaml`

 * *Files identical despite different names*

### Comparing `napari-bbox-0.0.2/src/napari_bbox.egg-info/PKG-INFO` & `napari-bbox-0.0.3/src/napari_bbox.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: napari-bbox
-Version: 0.0.2
+Version: 0.0.3
 Summary: A new layer for bounding boxes in 2+ dimensions
 Home-page: https://github.com/bauerdavid/napari-bbox
 Author: David Bauer
 Author-email: dbauer@brc.hu
 License: BSD-3-Clause
 Project-URL: Bug Tracker, https://github.com/bauerdavid/napari-bbox/issues
 Project-URL: Documentation, https://github.com/bauerdavid/napari-bbox#README.md
@@ -36,16 +36,14 @@
 [![codecov](https://codecov.io/gh/bauerdavid/napari-bbox/branch/main/graph/badge.svg)](https://codecov.io/gh/bauerdavid/napari-bbox)
 [![napari hub](https://img.shields.io/endpoint?url=https://api.napari-hub.org/shields/napari-bbox)](https://napari-hub.org/plugins/napari-bbox)
 
 A new layer for bounding boxes in 2+ dimensions
 
 > **Note**: This plugin was originally part of [Annotation Toolbox](https://www.napari-hub.org/plugins/napari-nD-annotator), and was separated to allow other plugins to utilize it.
 
-> **Note**: Currently the plugin does not support `napari==0.4.17`, see https://github.com/bauerdavid/napari-bbox/issues/4.
-
 ----------------------------------
 
 ## Demo
 
 
 https://user-images.githubusercontent.com/36735863/227506511-d672ce5c-eab5-436f-a7fd-6080e118a9a8.mp4
```

### Comparing `napari-bbox-0.0.2/src/napari_bbox.egg-info/SOURCES.txt` & `napari-bbox-0.0.3/src/napari_bbox.egg-info/SOURCES.txt`

 * *Files identical despite different names*

