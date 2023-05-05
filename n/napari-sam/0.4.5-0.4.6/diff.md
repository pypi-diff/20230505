# Comparing `tmp/napari-sam-0.4.5.tar.gz` & `tmp/napari-sam-0.4.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "napari-sam-0.4.5.tar", last modified: Thu May  4 08:45:25 2023, max compression
+gzip compressed data, was "napari-sam-0.4.6.tar", last modified: Fri May  5 12:35:57 2023, max compression
```

## Comparing `napari-sam-0.4.5.tar` & `napari-sam-0.4.6.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 08:45:25.434451 napari-sam-0.4.5/
--rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-05-04 08:45:04.000000 napari-sam-0.4.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-04 08:45:04.000000 napari-sam-0.4.5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     5950 2023-05-04 08:45:25.434451 napari-sam-0.4.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4715 2023-05-04 08:45:04.000000 napari-sam-0.4.5/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      180 2023-05-04 08:45:04.000000 napari-sam-0.4.5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1715 2023-05-04 08:45:25.434451 napari-sam-0.4.5/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 08:45:25.430452 napari-sam-0.4.5/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 08:45:25.430452 napari-sam-0.4.5/src/napari_sam/
--rw-r--r--   0 runner    (1001) docker     (123)     2823 2023-05-04 08:45:04.000000 napari-sam-0.4.5/src/napari_sam/QCollapsibleBox.py
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-05-04 08:45:04.000000 napari-sam-0.4.5/src/napari_sam/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    64659 2023-05-04 08:45:04.000000 napari-sam-0.4.5/src/napari_sam/_widget.py
--rw-r--r--   0 runner    (1001) docker     (123)      274 2023-05-04 08:45:04.000000 napari-sam-0.4.5/src/napari_sam/napari.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     3767 2023-05-04 08:45:04.000000 napari-sam-0.4.5/src/napari_sam/slicer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2602 2023-05-04 08:45:04.000000 napari-sam-0.4.5/src/napari_sam/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 08:45:25.430452 napari-sam-0.4.5/src/napari_sam.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5950 2023-05-04 08:45:25.000000 napari-sam-0.4.5/src/napari_sam.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      447 2023-05-04 08:45:25.000000 napari-sam-0.4.5/src/napari_sam.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-04 08:45:25.000000 napari-sam-0.4.5/src/napari_sam.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-05-04 08:45:25.000000 napari-sam-0.4.5/src/napari_sam.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      115 2023-05-04 08:45:25.000000 napari-sam-0.4.5/src/napari_sam.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-04 08:45:25.000000 napari-sam-0.4.5/src/napari_sam.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 12:35:57.075731 napari-sam-0.4.6/
+-rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-05-05 12:35:37.000000 napari-sam-0.4.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-05 12:35:37.000000 napari-sam-0.4.6/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5950 2023-05-05 12:35:57.079731 napari-sam-0.4.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4715 2023-05-05 12:35:37.000000 napari-sam-0.4.6/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      180 2023-05-05 12:35:37.000000 napari-sam-0.4.6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1715 2023-05-05 12:35:57.079731 napari-sam-0.4.6/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 12:35:57.075731 napari-sam-0.4.6/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 12:35:57.075731 napari-sam-0.4.6/src/napari_sam/
+-rw-r--r--   0 runner    (1001) docker     (123)     2823 2023-05-05 12:35:37.000000 napari-sam-0.4.6/src/napari_sam/QCollapsibleBox.py
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-05-05 12:35:37.000000 napari-sam-0.4.6/src/napari_sam/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    65134 2023-05-05 12:35:37.000000 napari-sam-0.4.6/src/napari_sam/_widget.py
+-rw-r--r--   0 runner    (1001) docker     (123)      274 2023-05-05 12:35:37.000000 napari-sam-0.4.6/src/napari_sam/napari.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     3767 2023-05-05 12:35:37.000000 napari-sam-0.4.6/src/napari_sam/slicer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2602 2023-05-05 12:35:37.000000 napari-sam-0.4.6/src/napari_sam/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 12:35:57.075731 napari-sam-0.4.6/src/napari_sam.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5950 2023-05-05 12:35:57.000000 napari-sam-0.4.6/src/napari_sam.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      447 2023-05-05 12:35:57.000000 napari-sam-0.4.6/src/napari_sam.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 12:35:57.000000 napari-sam-0.4.6/src/napari_sam.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-05-05 12:35:57.000000 napari-sam-0.4.6/src/napari_sam.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      115 2023-05-05 12:35:57.000000 napari-sam-0.4.6/src/napari_sam.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-05 12:35:57.000000 napari-sam-0.4.6/src/napari_sam.egg-info/top_level.txt
```

### Comparing `napari-sam-0.4.5/LICENSE` & `napari-sam-0.4.6/LICENSE`

 * *Files identical despite different names*

### Comparing `napari-sam-0.4.5/PKG-INFO` & `napari-sam-0.4.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: napari-sam
-Version: 0.4.5
+Version: 0.4.6
 Summary: Segment anything with Meta AI's new SAM model!
 Home-page: https://github.com/MIC-DKFZ/napari-sam
 Author: Karol Gotkowski
 Author-email: karol.gotkowski@dkfz.de
 License: Apache-2.0
 Project-URL: Bug Tracker, https://github.com/MIC-DKFZ/napari-sam/issues
 Project-URL: Documentation, https://github.com/MIC-DKFZ/napari-sam#README.md
```

### Comparing `napari-sam-0.4.5/README.md` & `napari-sam-0.4.6/README.md`

 * *Files identical despite different names*

### Comparing `napari-sam-0.4.5/setup.cfg` & `napari-sam-0.4.6/setup.cfg`

 * *Files identical despite different names*

### Comparing `napari-sam-0.4.5/src/napari_sam/QCollapsibleBox.py` & `napari-sam-0.4.6/src/napari_sam/QCollapsibleBox.py`

 * *Files identical despite different names*

### Comparing `napari-sam-0.4.5/src/napari_sam/_widget.py` & `napari-sam-0.4.6/src/napari_sam/_widget.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 from qtpy import QtCore
 from qtpy.QtCore import Qt
 import napari
 import numpy as np
 from enum import Enum
 from collections import deque, defaultdict
 import inspect
-from segment_anything import SamPredictor, sam_model_registry
+from segment_anything import SamPredictor, build_sam_vit_h, build_sam_vit_l, build_sam_vit_b
 from segment_anything.automatic_mask_generator import SamAutomaticMaskGenerator
 from napari_sam.utils import normalize
 import torch
 from vispy.util.keys import CONTROL
 import copy
 import warnings
 from tqdm import tqdm
@@ -37,20 +37,20 @@
 
 
 class BboxState(Enum):
     CLICK = 0
     DRAG = 1
     RELEASE = 2
 
-
-SAM_WEIGHTS_URL = {
-    "default": "https://dl.fbaipublicfiles.com/segment_anything/sam_vit_h_4b8939.pth",
-    "vit_h": "https://dl.fbaipublicfiles.com/segment_anything/sam_vit_h_4b8939.pth",
-    "vit_l": "https://dl.fbaipublicfiles.com/segment_anything/sam_vit_l_0b3195.pth",
-    "vit_b": "https://dl.fbaipublicfiles.com/segment_anything/sam_vit_b_01ec64.pth",
+SAM_MODELS = {
+    "default": {"filename": "sam_vit_h_4b8939.pth", "url": "https://dl.fbaipublicfiles.com/segment_anything/sam_vit_h_4b8939.pth", "model": build_sam_vit_h},
+    "vit_h": {"filename": "sam_vit_h_4b8939.pth", "url": "https://dl.fbaipublicfiles.com/segment_anything/sam_vit_h_4b8939.pth", "model": build_sam_vit_h},
+    "vit_l": {"filename": "sam_vit_l_0b3195.pth", "url": "https://dl.fbaipublicfiles.com/segment_anything/sam_vit_l_0b3195.pth", "model": build_sam_vit_l},
+    "vit_b": {"filename": "sam_vit_b_01ec64.pth", "url": "https://dl.fbaipublicfiles.com/segment_anything/sam_vit_b_01ec64.pth", "model": build_sam_vit_b},
+    "MedSAM": {"filename": "sam_vit_b_01ec64_medsam.pth", "url": "https://syncandshare.desy.de/index.php/s/yLfdFbpfEGSHJWY/download/medsam_20230423_vit_b_0.0.1.pth", "model": build_sam_vit_b},
 }
 
 
 class SamWidget(QWidget):
     def __init__(self, napari_viewer):
         super().__init__()
         self.viewer = napari_viewer
@@ -440,15 +440,15 @@
         #     self.rb_auto.setStyleSheet("color: gray")
         # else:
         #     self.rb_auto.setEnabled(True)
         #     self.rb_auto.setStyleSheet("")
         pass
 
     def init_model_type_combobox(self):
-        model_types = list(sam_model_registry.keys())
+        model_types = list(SAM_MODELS.keys())
         cached_weight_types = self.get_cached_weight_types(model_types)
         # entries = []
         # for name, is_cached in cached_weight_types.items():
         #     if is_cached:
         #         entries.append("{} (Cached)".format(name))
         #     else:
         #         entries.append("{} (Auto-Download)".format(name))
@@ -459,15 +459,15 @@
             self.btn_load_model.setText("Load model")
         else:
             self.btn_load_model.setText("Download and load model")
 
         self.cb_model_type.currentTextChanged.connect(self.on_model_type_combobox_change)
 
     def update_model_type_combobox(self):
-        model_types = list(sam_model_registry.keys())
+        model_types = list(SAM_MODELS.keys())
         cached_weight_types = self.get_cached_weight_types(model_types)
         entries = []
         for name, is_cached in cached_weight_types.items():
             if name == self.loaded_model:
                 entries.append("{} (Loaded)".format(name))
             elif is_cached:
                 entries.append("{} (Cached)".format(name))
@@ -477,15 +477,15 @@
         self.cb_model_type.addItems(entries)
         if self.loaded_model is not None:
             loaded_model_index = self.cb_model_type.findText("{} (Loaded)".format(self.loaded_model))
             self.cb_model_type.setCurrentIndex(loaded_model_index)
 
 
     def on_model_type_combobox_change(self):
-        model_types = list(sam_model_registry.keys())
+        model_types = list(SAM_MODELS.keys())
         cached_weight_types = self.get_cached_weight_types(model_types)
 
         if cached_weight_types[list(cached_weight_types.keys())[self.cb_model_type.currentIndex()]]:
             self.btn_load_model.setText("Load model")
         else:
             self.btn_load_model.setText("Download and load model")
 
@@ -557,17 +557,17 @@
             self.btn_activate.setEnabled(True)
         else:
             self.btn_activate.setEnabled(False)
 
     def _load_model(self):
         self.cb_model_type.setEnabled(False)
         self.btn_load_model.setEnabled(False)
-        model_types = list(sam_model_registry.keys())
+        model_types = list(SAM_MODELS.keys())
         model_type = model_types[self.cb_model_type.currentIndex()]
-        self.sam_model = sam_model_registry[model_type](
+        self.sam_model = SAM_MODELS[model_type]["model"](
             self.get_weights_path(model_type)
         )
         self.sam_model.to(self.device)
         self.sam_predictor = SamPredictor(self.sam_model)
         self.loaded_model = model_type
         self.update_model_type_combobox()
         self.cb_model_type.setEnabled(True)
@@ -1310,34 +1310,34 @@
                 l_creating_features.deleteLater()
 
         # Close the progress bar and the URL
         progress_bar_tqdm.close()
         req.close()
 
     def get_weights_path(self, model_type):
-        weight_url = SAM_WEIGHTS_URL[model_type]
+        weight_url = SAM_MODELS[model_type]["url"]
 
         cache_dir = Path.home() / ".cache/napari-segment-anything"
         cache_dir.mkdir(parents=True, exist_ok=True)
 
-        weight_path = cache_dir / weight_url.split("/")[-1]
+        weight_path = cache_dir / SAM_MODELS[model_type]["filename"]
 
         if not weight_path.exists():
             print("Downloading {} to {} ...".format(weight_url, weight_path))
             self.download_with_progress(weight_url, weight_path)
 
         return weight_path
 
     def get_cached_weight_types(self, model_types):
         cached_weight_types = {}
         cache_dir = str(Path.home() / ".cache/napari-segment-anything")
 
         for model_type in model_types:
-            model_type_name = os.path.basename(SAM_WEIGHTS_URL[model_type])
-            if os.path.isfile(join(cache_dir, model_type_name)):
+            filename = os.path.basename(SAM_MODELS[model_type]["filename"])
+            if os.path.isfile(join(cache_dir, filename)):
                 cached_weight_types[model_type] = True
             else:
                 cached_weight_types[model_type] = False
 
         return cached_weight_types
 
     # def _myfilter(self, row, parent):
```

### Comparing `napari-sam-0.4.5/src/napari_sam/slicer.py` & `napari-sam-0.4.6/src/napari_sam/slicer.py`

 * *Files identical despite different names*

### Comparing `napari-sam-0.4.5/src/napari_sam/utils.py` & `napari-sam-0.4.6/src/napari_sam/utils.py`

 * *Files identical despite different names*

### Comparing `napari-sam-0.4.5/src/napari_sam.egg-info/PKG-INFO` & `napari-sam-0.4.6/src/napari_sam.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: napari-sam
-Version: 0.4.5
+Version: 0.4.6
 Summary: Segment anything with Meta AI's new SAM model!
 Home-page: https://github.com/MIC-DKFZ/napari-sam
 Author: Karol Gotkowski
 Author-email: karol.gotkowski@dkfz.de
 License: Apache-2.0
 Project-URL: Bug Tracker, https://github.com/MIC-DKFZ/napari-sam/issues
 Project-URL: Documentation, https://github.com/MIC-DKFZ/napari-sam#README.md
```

