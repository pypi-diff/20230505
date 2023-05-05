# Comparing `tmp/unstructured_inference-0.4.3.tar.gz` & `tmp/unstructured_inference-0.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "unstructured_inference-0.4.3.tar", last modified: Thu May  4 20:32:37 2023, max compression
+gzip compressed data, was "unstructured_inference-0.4.4.tar", last modified: Fri May  5 01:59:27 2023, max compression
```

## Comparing `unstructured_inference-0.4.3.tar` & `unstructured_inference-0.4.4.tar`

### file list

```diff
@@ -1,37 +1,40 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 20:32:37.363679 unstructured_inference-0.4.3/
--rw-r--r--   0 runner    (1001) docker     (123)       29 2023-05-04 20:30:39.000000 unstructured_inference-0.4.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     6802 2023-05-04 20:32:37.363679 unstructured_inference-0.4.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4731 2023-05-04 20:30:39.000000 unstructured_inference-0.4.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 20:32:37.355679 unstructured_inference-0.4.3/requirements/
--rw-r--r--   0 runner    (1001) docker     (123)      135 2023-05-04 20:30:39.000000 unstructured_inference-0.4.3/requirements/base.in
--rw-r--r--   0 runner    (1001) docker     (123)      257 2023-05-04 20:32:37.363679 unstructured_inference-0.4.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3313 2023-05-04 20:30:39.000000 unstructured_inference-0.4.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 20:32:37.355679 unstructured_inference-0.4.3/unstructured_inference/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 20:30:39.000000 unstructured_inference-0.4.3/unstructured_inference/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-05-04 20:30:39.000000 unstructured_inference-0.4.3/unstructured_inference/__version__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1733 2023-05-04 20:30:39.000000 unstructured_inference-0.4.3/unstructured_inference/api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 20:32:37.359679 unstructured_inference-0.4.3/unstructured_inference/inference/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 20:30:39.000000 unstructured_inference-0.4.3/unstructured_inference/inference/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11408 2023-05-04 20:30:39.000000 unstructured_inference-0.4.3/unstructured_inference/inference/elements.py
--rw-r--r--   0 runner    (1001) docker     (123)    12340 2023-05-04 20:30:39.000000 unstructured_inference-0.4.3/unstructured_inference/inference/layout.py
--rw-r--r--   0 runner    (1001) docker     (123)     2391 2023-05-04 20:30:39.000000 unstructured_inference-0.4.3/unstructured_inference/inference/layoutelement.py
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-05-04 20:30:39.000000 unstructured_inference-0.4.3/unstructured_inference/logger.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 20:32:37.363679 unstructured_inference-0.4.3/unstructured_inference/models/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 20:30:39.000000 unstructured_inference-0.4.3/unstructured_inference/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1147 2023-05-04 20:30:39.000000 unstructured_inference-0.4.3/unstructured_inference/models/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     3233 2023-05-04 20:30:39.000000 unstructured_inference-0.4.3/unstructured_inference/models/detectron2.py
--rw-r--r--   0 runner    (1001) docker     (123)     2822 2023-05-04 20:30:39.000000 unstructured_inference-0.4.3/unstructured_inference/models/donut.py
--rw-r--r--   0 runner    (1001) docker     (123)      332 2023-05-04 20:30:39.000000 unstructured_inference-0.4.3/unstructured_inference/models/paddle_ocr.py
--rw-r--r--   0 runner    (1001) docker     (123)    24106 2023-05-04 20:30:39.000000 unstructured_inference-0.4.3/unstructured_inference/models/table_postprocess.py
--rw-r--r--   0 runner    (1001) docker     (123)    23850 2023-05-04 20:30:39.000000 unstructured_inference-0.4.3/unstructured_inference/models/tables.py
--rw-r--r--   0 runner    (1001) docker     (123)      978 2023-05-04 20:30:39.000000 unstructured_inference-0.4.3/unstructured_inference/models/tesseract.py
--rw-r--r--   0 runner    (1001) docker     (123)     1137 2023-05-04 20:30:39.000000 unstructured_inference-0.4.3/unstructured_inference/models/unstructuredmodel.py
--rw-r--r--   0 runner    (1001) docker     (123)     8077 2023-05-04 20:30:39.000000 unstructured_inference-0.4.3/unstructured_inference/models/yolox.py
--rw-r--r--   0 runner    (1001) docker     (123)     1568 2023-05-04 20:30:39.000000 unstructured_inference-0.4.3/unstructured_inference/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     6663 2023-05-04 20:30:39.000000 unstructured_inference-0.4.3/unstructured_inference/visualize.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 20:32:37.359679 unstructured_inference-0.4.3/unstructured_inference.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6802 2023-05-04 20:32:37.000000 unstructured_inference-0.4.3/unstructured_inference.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-05-04 20:32:37.000000 unstructured_inference-0.4.3/unstructured_inference.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-04 20:32:37.000000 unstructured_inference-0.4.3/unstructured_inference.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      239 2023-05-04 20:32:37.000000 unstructured_inference-0.4.3/unstructured_inference.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-04 20:32:37.000000 unstructured_inference-0.4.3/unstructured_inference.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 01:59:27.276872 unstructured_inference-0.4.4/
+-rw-r--r--   0 runner    (1001) docker     (123)       29 2023-05-05 01:57:27.000000 unstructured_inference-0.4.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     6802 2023-05-05 01:59:27.276872 unstructured_inference-0.4.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4731 2023-05-05 01:57:27.000000 unstructured_inference-0.4.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 01:59:27.264872 unstructured_inference-0.4.4/requirements/
+-rw-r--r--   0 runner    (1001) docker     (123)      135 2023-05-05 01:57:27.000000 unstructured_inference-0.4.4/requirements/base.in
+-rw-r--r--   0 runner    (1001) docker     (123)      257 2023-05-05 01:59:27.276872 unstructured_inference-0.4.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3313 2023-05-05 01:57:27.000000 unstructured_inference-0.4.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 01:59:27.264872 unstructured_inference-0.4.4/unstructured_inference/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 01:57:27.000000 unstructured_inference-0.4.4/unstructured_inference/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-05-05 01:57:27.000000 unstructured_inference-0.4.4/unstructured_inference/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1733 2023-05-05 01:57:27.000000 unstructured_inference-0.4.4/unstructured_inference/api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 01:59:27.268872 unstructured_inference-0.4.4/unstructured_inference/inference/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 01:57:27.000000 unstructured_inference-0.4.4/unstructured_inference/inference/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11408 2023-05-05 01:57:27.000000 unstructured_inference-0.4.4/unstructured_inference/inference/elements.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12340 2023-05-05 01:57:27.000000 unstructured_inference-0.4.4/unstructured_inference/inference/layout.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2391 2023-05-05 01:57:27.000000 unstructured_inference-0.4.4/unstructured_inference/inference/layoutelement.py
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-05-05 01:57:27.000000 unstructured_inference-0.4.4/unstructured_inference/logger.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 01:59:27.276872 unstructured_inference-0.4.4/unstructured_inference/models/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 01:57:27.000000 unstructured_inference-0.4.4/unstructured_inference/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1147 2023-05-05 01:57:27.000000 unstructured_inference-0.4.4/unstructured_inference/models/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3233 2023-05-05 01:57:27.000000 unstructured_inference-0.4.4/unstructured_inference/models/detectron2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2822 2023-05-05 01:57:27.000000 unstructured_inference-0.4.4/unstructured_inference/models/donut.py
+-rw-r--r--   0 runner    (1001) docker     (123)      332 2023-05-05 01:57:27.000000 unstructured_inference-0.4.4/unstructured_inference/models/paddle_ocr.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24106 2023-05-05 01:57:27.000000 unstructured_inference-0.4.4/unstructured_inference/models/table_postprocess.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23850 2023-05-05 01:57:27.000000 unstructured_inference-0.4.4/unstructured_inference/models/tables.py
+-rw-r--r--   0 runner    (1001) docker     (123)      978 2023-05-05 01:57:27.000000 unstructured_inference-0.4.4/unstructured_inference/models/tesseract.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1137 2023-05-05 01:57:27.000000 unstructured_inference-0.4.4/unstructured_inference/models/unstructuredmodel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8077 2023-05-05 01:57:27.000000 unstructured_inference-0.4.4/unstructured_inference/models/yolox.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 01:59:27.276872 unstructured_inference-0.4.4/unstructured_inference/patches/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 01:57:27.000000 unstructured_inference-0.4.4/unstructured_inference/patches/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      743 2023-05-05 01:57:27.000000 unstructured_inference-0.4.4/unstructured_inference/patches/pdfminer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1568 2023-05-05 01:57:27.000000 unstructured_inference-0.4.4/unstructured_inference/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6663 2023-05-05 01:57:27.000000 unstructured_inference-0.4.4/unstructured_inference/visualize.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 01:59:27.268872 unstructured_inference-0.4.4/unstructured_inference.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6802 2023-05-05 01:59:26.000000 unstructured_inference-0.4.4/unstructured_inference.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1194 2023-05-05 01:59:27.000000 unstructured_inference-0.4.4/unstructured_inference.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 01:59:26.000000 unstructured_inference-0.4.4/unstructured_inference.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      239 2023-05-05 01:59:26.000000 unstructured_inference-0.4.4/unstructured_inference.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-05 01:59:26.000000 unstructured_inference-0.4.4/unstructured_inference.egg-info/top_level.txt
```

### Comparing `unstructured_inference-0.4.3/PKG-INFO` & `unstructured_inference-0.4.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: unstructured_inference
-Version: 0.4.3
+Version: 0.4.4
 Summary: A library for performing inference using trained models.
 Home-page: https://github.com/Unstructured-IO/unstructured-inference
 Author: Unstructured Technologies
 Author-email: devops@unstructuredai.io
 License: Apache-2.0
 Description: <h3 align="center">
           <img
```

### Comparing `unstructured_inference-0.4.3/README.md` & `unstructured_inference-0.4.4/README.md`

 * *Files identical despite different names*

### Comparing `unstructured_inference-0.4.3/setup.py` & `unstructured_inference-0.4.4/setup.py`

 * *Files identical despite different names*

### Comparing `unstructured_inference-0.4.3/unstructured_inference/api.py` & `unstructured_inference-0.4.4/unstructured_inference/api.py`

 * *Files identical despite different names*

### Comparing `unstructured_inference-0.4.3/unstructured_inference/inference/elements.py` & `unstructured_inference-0.4.4/unstructured_inference/inference/elements.py`

 * *Files identical despite different names*

### Comparing `unstructured_inference-0.4.3/unstructured_inference/inference/layout.py` & `unstructured_inference-0.4.4/unstructured_inference/inference/layout.py`

 * *Files identical despite different names*

### Comparing `unstructured_inference-0.4.3/unstructured_inference/inference/layoutelement.py` & `unstructured_inference-0.4.4/unstructured_inference/inference/layoutelement.py`

 * *Files identical despite different names*

### Comparing `unstructured_inference-0.4.3/unstructured_inference/models/base.py` & `unstructured_inference-0.4.4/unstructured_inference/models/base.py`

 * *Files identical despite different names*

### Comparing `unstructured_inference-0.4.3/unstructured_inference/models/detectron2.py` & `unstructured_inference-0.4.4/unstructured_inference/models/detectron2.py`

 * *Files identical despite different names*

### Comparing `unstructured_inference-0.4.3/unstructured_inference/models/donut.py` & `unstructured_inference-0.4.4/unstructured_inference/models/donut.py`

 * *Files identical despite different names*

### Comparing `unstructured_inference-0.4.3/unstructured_inference/models/table_postprocess.py` & `unstructured_inference-0.4.4/unstructured_inference/models/table_postprocess.py`

 * *Files identical despite different names*

### Comparing `unstructured_inference-0.4.3/unstructured_inference/models/tables.py` & `unstructured_inference-0.4.4/unstructured_inference/models/tables.py`

 * *Files identical despite different names*

### Comparing `unstructured_inference-0.4.3/unstructured_inference/models/tesseract.py` & `unstructured_inference-0.4.4/unstructured_inference/models/tesseract.py`

 * *Files identical despite different names*

### Comparing `unstructured_inference-0.4.3/unstructured_inference/models/unstructuredmodel.py` & `unstructured_inference-0.4.4/unstructured_inference/models/unstructuredmodel.py`

 * *Files identical despite different names*

### Comparing `unstructured_inference-0.4.3/unstructured_inference/models/yolox.py` & `unstructured_inference-0.4.4/unstructured_inference/models/yolox.py`

 * *Files identical despite different names*

### Comparing `unstructured_inference-0.4.3/unstructured_inference/utils.py` & `unstructured_inference-0.4.4/unstructured_inference/utils.py`

 * *Files identical despite different names*

### Comparing `unstructured_inference-0.4.3/unstructured_inference/visualize.py` & `unstructured_inference-0.4.4/unstructured_inference/visualize.py`

 * *Files identical despite different names*

### Comparing `unstructured_inference-0.4.3/unstructured_inference.egg-info/PKG-INFO` & `unstructured_inference-0.4.4/unstructured_inference.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: unstructured-inference
-Version: 0.4.3
+Version: 0.4.4
 Summary: A library for performing inference using trained models.
 Home-page: https://github.com/Unstructured-IO/unstructured-inference
 Author: Unstructured Technologies
 Author-email: devops@unstructuredai.io
 License: Apache-2.0
 Description: <h3 align="center">
           <img
```

### Comparing `unstructured_inference-0.4.3/unstructured_inference.egg-info/SOURCES.txt` & `unstructured_inference-0.4.4/unstructured_inference.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -23,8 +23,10 @@
 unstructured_inference/models/detectron2.py
 unstructured_inference/models/donut.py
 unstructured_inference/models/paddle_ocr.py
 unstructured_inference/models/table_postprocess.py
 unstructured_inference/models/tables.py
 unstructured_inference/models/tesseract.py
 unstructured_inference/models/unstructuredmodel.py
-unstructured_inference/models/yolox.py
+unstructured_inference/models/yolox.py
+unstructured_inference/patches/__init__.py
+unstructured_inference/patches/pdfminer.py
```

