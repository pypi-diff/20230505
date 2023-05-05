# Comparing `tmp/BaseDT-0.0.3.tar.gz` & `tmp/BaseDT-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/BaseDT-0.0.3.tar", last modified: Wed Apr 26 07:41:42 2023, max compression
+gzip compressed data, was "dist/BaseDT-0.0.5.tar", last modified: Fri May  5 09:47:48 2023, max compression
```

## Comparing `BaseDT-0.0.3.tar` & `BaseDT-0.0.5.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxr-x   0 user      (1001) user      (1001)        0 2023-04-26 07:41:42.000000 BaseDT-0.0.3/
-drwxrwxr-x   0 user      (1001) user      (1001)        0 2023-04-26 07:41:42.000000 BaseDT-0.0.3/BaseDT/
--rw-rw-r--   0 user      (1001) user      (1001)        0 2023-04-26 07:17:02.000000 BaseDT-0.0.3/BaseDT/__init__.py
--rw-rw-r--   0 user      (1001) user      (1001)    16851 2023-04-26 07:17:02.000000 BaseDT-0.0.3/BaseDT/data.py
--rw-rw-r--   0 user      (1001) user      (1001)    12037 2023-04-26 07:17:02.000000 BaseDT-0.0.3/BaseDT/data_image.py
--rw-rw-r--   0 user      (1001) user      (1001)    31309 2023-04-26 07:17:02.000000 BaseDT-0.0.3/BaseDT/dataset.py
--rw-rw-r--   0 user      (1001) user      (1001)     1020 2023-04-26 07:17:02.000000 BaseDT-0.0.3/BaseDT/io.py
--rw-rw-r--   0 user      (1001) user      (1001)     6986 2023-04-26 07:19:34.000000 BaseDT-0.0.3/BaseDT/plot.py
-drwxrwxr-x   0 user      (1001) user      (1001)        0 2023-04-26 07:41:42.000000 BaseDT-0.0.3/BaseDT.egg-info/
--rw-rw-r--   0 user      (1001) user      (1001)      314 2023-04-26 07:41:41.000000 BaseDT-0.0.3/BaseDT.egg-info/PKG-INFO
--rw-rw-r--   0 user      (1001) user      (1001)      316 2023-04-26 07:41:41.000000 BaseDT-0.0.3/BaseDT.egg-info/SOURCES.txt
--rw-rw-r--   0 user      (1001) user      (1001)        1 2023-04-26 07:41:41.000000 BaseDT-0.0.3/BaseDT.egg-info/dependency_links.txt
--rw-rw-r--   0 user      (1001) user      (1001)       30 2023-04-26 07:41:41.000000 BaseDT-0.0.3/BaseDT.egg-info/requires.txt
--rw-rw-r--   0 user      (1001) user      (1001)        7 2023-04-26 07:41:41.000000 BaseDT-0.0.3/BaseDT.egg-info/top_level.txt
--rw-rw-r--   0 user      (1001) user      (1001)        1 2023-02-02 07:26:47.000000 BaseDT-0.0.3/BaseDT.egg-info/zip-safe
--rw-rw-r--   0 user      (1001) user      (1001)       40 2023-04-06 03:45:54.000000 BaseDT-0.0.3/MANIFEST.in
--rw-rw-r--   0 user      (1001) user      (1001)      314 2023-04-26 07:41:42.000000 BaseDT-0.0.3/PKG-INFO
--rw-rw-r--   0 user      (1001) user      (1001)       30 2023-02-02 07:23:17.000000 BaseDT-0.0.3/install_requires.txt
--rw-rw-r--   0 user      (1001) user      (1001)       38 2023-04-26 07:41:42.000000 BaseDT-0.0.3/setup.cfg
--rw-rw-r--   0 user      (1001) user      (1001)     4245 2023-04-26 07:40:56.000000 BaseDT-0.0.3/setup.py
+drwxrwxr-x   0 user      (1001) user      (1001)        0 2023-05-05 09:47:48.000000 BaseDT-0.0.5/
+drwxrwxr-x   0 user      (1001) user      (1001)        0 2023-05-05 09:47:48.000000 BaseDT-0.0.5/BaseDT/
+-rw-rw-r--   0 user      (1001) user      (1001)        0 2023-04-26 07:17:02.000000 BaseDT-0.0.5/BaseDT/__init__.py
+-rw-rw-r--   0 user      (1001) user      (1001)    16851 2023-05-05 09:45:53.000000 BaseDT-0.0.5/BaseDT/data.py
+-rw-rw-r--   0 user      (1001) user      (1001)    12037 2023-04-26 07:17:02.000000 BaseDT-0.0.5/BaseDT/data_image.py
+-rw-rw-r--   0 user      (1001) user      (1001)    31309 2023-04-26 07:17:02.000000 BaseDT-0.0.5/BaseDT/dataset.py
+-rw-rw-r--   0 user      (1001) user      (1001)     1020 2023-04-26 07:17:02.000000 BaseDT-0.0.5/BaseDT/io.py
+-rw-rw-r--   0 user      (1001) user      (1001)     6986 2023-04-26 07:19:34.000000 BaseDT-0.0.5/BaseDT/plot.py
+drwxrwxr-x   0 user      (1001) user      (1001)        0 2023-05-05 09:47:48.000000 BaseDT-0.0.5/BaseDT.egg-info/
+-rw-rw-r--   0 user      (1001) user      (1001)      314 2023-05-05 09:47:48.000000 BaseDT-0.0.5/BaseDT.egg-info/PKG-INFO
+-rw-rw-r--   0 user      (1001) user      (1001)      316 2023-05-05 09:47:48.000000 BaseDT-0.0.5/BaseDT.egg-info/SOURCES.txt
+-rw-rw-r--   0 user      (1001) user      (1001)        1 2023-05-05 09:47:48.000000 BaseDT-0.0.5/BaseDT.egg-info/dependency_links.txt
+-rw-rw-r--   0 user      (1001) user      (1001)       49 2023-05-05 09:47:48.000000 BaseDT-0.0.5/BaseDT.egg-info/requires.txt
+-rw-rw-r--   0 user      (1001) user      (1001)        7 2023-05-05 09:47:48.000000 BaseDT-0.0.5/BaseDT.egg-info/top_level.txt
+-rw-rw-r--   0 user      (1001) user      (1001)        1 2023-02-02 07:26:47.000000 BaseDT-0.0.5/BaseDT.egg-info/zip-safe
+-rw-rw-r--   0 user      (1001) user      (1001)       40 2023-04-06 03:45:54.000000 BaseDT-0.0.5/MANIFEST.in
+-rw-rw-r--   0 user      (1001) user      (1001)      314 2023-05-05 09:47:48.000000 BaseDT-0.0.5/PKG-INFO
+-rw-rw-r--   0 user      (1001) user      (1001)       49 2023-05-05 09:43:00.000000 BaseDT-0.0.5/install_requires.txt
+-rw-rw-r--   0 user      (1001) user      (1001)       38 2023-05-05 09:47:48.000000 BaseDT-0.0.5/setup.cfg
+-rw-rw-r--   0 user      (1001) user      (1001)     4245 2023-05-05 09:47:43.000000 BaseDT-0.0.5/setup.py
```

### Comparing `BaseDT-0.0.3/BaseDT/data.py` & `BaseDT-0.0.5/BaseDT/data.py`

 * *Files 0% similar despite different names*

```diff
@@ -300,15 +300,15 @@
     def map_orig_coords(self, boxes):
         #TODO 暂时只支持box的映射，后续应该支持单纯的坐标映射
         original_w, original_h = self.raw_value.shape[:2]
         processed_w, processed_h = self.value.shape[:2]
         sx, sy = original_w / processed_w, original_h / processed_h
         new_boxes = np.array([]).reshape(0, 5)
         for box in boxes:
-            new_box = [box[0] * sx, box[1] * sy, box[2] * sx, box[3] * sy, box[4]]
+            new_box = [box[0] * sy, box[1] * sx, box[2] * sy, box[3] * sx, box[4]]
             new_boxes = np.concatenate([new_boxes, [new_box]], axis=0)
         return new_boxes
 
 class TextData(object):
     _defaults = {
         "data_type": 'uint8',
         # 文本默认属性
```

### Comparing `BaseDT-0.0.3/BaseDT/data_image.py` & `BaseDT-0.0.5/BaseDT/data_image.py`

 * *Files identical despite different names*

### Comparing `BaseDT-0.0.3/BaseDT/dataset.py` & `BaseDT-0.0.5/BaseDT/dataset.py`

 * *Files identical despite different names*

### Comparing `BaseDT-0.0.3/BaseDT/io.py` & `BaseDT-0.0.5/BaseDT/io.py`

 * *Files identical despite different names*

### Comparing `BaseDT-0.0.3/BaseDT/plot.py` & `BaseDT-0.0.5/BaseDT/plot.py`

 * *Files identical despite different names*

### Comparing `BaseDT-0.0.3/setup.py` & `BaseDT-0.0.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -75,15 +75,15 @@
                 yield item
 
     packages = list(gen_packages_items())
     return packages
 
 setup(
     name='BaseDT',
-    version='0.0.3',
+    version='0.0.5',
     # version='0.0.1rc1',
     description='BaseDT is a data-processing  tool including data, dataset, io and plot.',
     license='MIT License',
     author='OpenXLab',
     author_email='wangbolun@pjlab.org.cn',
     url='https://github.com/OpenXLab-Edu/OpenMMLab-Edu',
     packages=find_packages(),
```

