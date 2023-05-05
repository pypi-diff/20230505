# Comparing `tmp/tf-utilities-0.1.8.tar.gz` & `tmp/tf-utilities-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tf-utilities-0.1.8.tar", last modified: Tue Apr  4 06:03:59 2023, max compression
+gzip compressed data, was "tf-utilities-0.1.9.tar", last modified: Fri May  5 05:42:43 2023, max compression
```

## Comparing `tf-utilities-0.1.8.tar` & `tf-utilities-0.1.9.tar`

### file list

```diff
@@ -1,24 +1,22 @@
-drwxr-xr-x   0 dwl2x     (1000) users      (100)        0 2023-04-04 06:03:59.162003 tf-utilities-0.1.8/
--rw-r--r--   0 dwl2x     (1000) users      (100)     1071 2022-08-18 23:47:52.000000 tf-utilities-0.1.8/LICENSE
--rw-r--r--   0 dwl2x     (1000) users      (100)     3634 2023-04-04 06:03:59.162003 tf-utilities-0.1.8/PKG-INFO
--rw-r--r--   0 dwl2x     (1000) users      (100)     1842 2022-08-18 23:47:52.000000 tf-utilities-0.1.8/README.md
--rw-r--r--   0 dwl2x     (1000) users      (100)      704 2023-04-03 03:26:43.000000 tf-utilities-0.1.8/pyproject.toml
--rw-r--r--   0 dwl2x     (1000) users      (100)       38 2023-04-04 06:03:59.162003 tf-utilities-0.1.8/setup.cfg
-drwxr-xr-x   0 dwl2x     (1000) users      (100)        0 2023-04-04 06:03:59.162003 tf-utilities-0.1.8/src/
-drwxr-xr-x   0 dwl2x     (1000) users      (100)        0 2023-04-04 06:03:59.162003 tf-utilities-0.1.8/src/tf_utilities/
--rw-r--r--   0 dwl2x     (1000) users      (100)      178 2023-04-03 03:27:11.000000 tf-utilities-0.1.8/src/tf_utilities/__init__.py
--rw-r--r--   0 dwl2x     (1000) users      (100)      444 2022-08-18 23:47:52.000000 tf-utilities-0.1.8/src/tf_utilities/config.py
--rw-r--r--   0 dwl2x     (1000) users      (100)     6447 2022-08-18 23:47:52.000000 tf-utilities-0.1.8/src/tf_utilities/data.py
--rw-r--r--   0 dwl2x     (1000) users      (100)      966 2022-08-18 23:47:52.000000 tf-utilities-0.1.8/src/tf_utilities/devices.py
--rw-r--r--   0 dwl2x     (1000) users      (100)    11469 2023-04-03 03:43:55.000000 tf-utilities-0.1.8/src/tf_utilities/scripting.py
--rw-r--r--   0 dwl2x     (1000) users      (100)      551 2022-11-04 03:54:52.000000 tf-utilities-0.1.8/src/tf_utilities/strategy.py
--rw-r--r--   0 dwl2x     (1000) users      (100)     2064 2023-03-29 18:40:29.000000 tf-utilities-0.1.8/src/tf_utilities/subbatching.py
--rw-r--r--   0 dwl2x     (1000) users      (100)      240 2023-03-29 18:40:38.000000 tf-utilities-0.1.8/src/tf_utilities/utils.py
-drwxr-xr-x   0 dwl2x     (1000) users      (100)        0 2023-04-04 06:03:59.162003 tf-utilities-0.1.8/src/tf_utilities.egg-info/
--rw-r--r--   0 dwl2x     (1000) users      (100)     3634 2023-04-04 06:03:59.000000 tf-utilities-0.1.8/src/tf_utilities.egg-info/PKG-INFO
--rw-r--r--   0 dwl2x     (1000) users      (100)      470 2023-04-04 06:03:59.000000 tf-utilities-0.1.8/src/tf_utilities.egg-info/SOURCES.txt
--rw-r--r--   0 dwl2x     (1000) users      (100)        1 2023-04-04 06:03:59.000000 tf-utilities-0.1.8/src/tf_utilities.egg-info/dependency_links.txt
--rw-r--r--   0 dwl2x     (1000) users      (100)       22 2023-04-04 06:03:59.000000 tf-utilities-0.1.8/src/tf_utilities.egg-info/requires.txt
--rw-r--r--   0 dwl2x     (1000) users      (100)       13 2023-04-04 06:03:59.000000 tf-utilities-0.1.8/src/tf_utilities.egg-info/top_level.txt
-drwxr-xr-x   0 dwl2x     (1000) users      (100)        0 2023-04-04 06:03:59.162003 tf-utilities-0.1.8/test/
--rw-r--r--   0 dwl2x     (1000) users      (100)        0 2023-03-16 06:13:35.000000 tf-utilities-0.1.8/test/test.py
+drwxr-xr-x   0 dwl2x     (1000) users      (100)        0 2023-05-05 05:42:43.682502 tf-utilities-0.1.9/
+-rw-r--r--   0 dwl2x     (1000) users      (100)     1071 2023-05-05 05:42:04.000000 tf-utilities-0.1.9/LICENSE
+-rw-r--r--   0 dwl2x     (1000) users      (100)     3634 2023-05-05 05:42:43.682502 tf-utilities-0.1.9/PKG-INFO
+-rw-r--r--   0 dwl2x     (1000) users      (100)     1842 2023-05-05 05:42:04.000000 tf-utilities-0.1.9/README.md
+-rw-r--r--   0 dwl2x     (1000) users      (100)      704 2023-05-05 05:42:17.000000 tf-utilities-0.1.9/pyproject.toml
+-rw-r--r--   0 dwl2x     (1000) users      (100)       38 2023-05-05 05:42:43.682502 tf-utilities-0.1.9/setup.cfg
+drwxr-xr-x   0 dwl2x     (1000) users      (100)        0 2023-05-05 05:42:43.682502 tf-utilities-0.1.9/src/
+drwxr-xr-x   0 dwl2x     (1000) users      (100)        0 2023-05-05 05:42:43.682502 tf-utilities-0.1.9/src/tf_utilities/
+-rw-r--r--   0 dwl2x     (1000) users      (100)      178 2023-05-05 05:42:31.000000 tf-utilities-0.1.9/src/tf_utilities/__init__.py
+-rw-r--r--   0 dwl2x     (1000) users      (100)      444 2023-05-05 05:42:04.000000 tf-utilities-0.1.9/src/tf_utilities/config.py
+-rw-r--r--   0 dwl2x     (1000) users      (100)     6447 2023-05-05 05:42:04.000000 tf-utilities-0.1.9/src/tf_utilities/data.py
+-rw-r--r--   0 dwl2x     (1000) users      (100)      966 2023-05-05 05:42:04.000000 tf-utilities-0.1.9/src/tf_utilities/devices.py
+-rw-r--r--   0 dwl2x     (1000) users      (100)    11469 2023-05-05 05:42:04.000000 tf-utilities-0.1.9/src/tf_utilities/scripting.py
+-rw-r--r--   0 dwl2x     (1000) users      (100)      563 2023-05-05 05:42:04.000000 tf-utilities-0.1.9/src/tf_utilities/strategy.py
+-rw-r--r--   0 dwl2x     (1000) users      (100)     2064 2023-05-05 05:42:04.000000 tf-utilities-0.1.9/src/tf_utilities/subbatching.py
+-rw-r--r--   0 dwl2x     (1000) users      (100)      240 2023-05-05 05:42:04.000000 tf-utilities-0.1.9/src/tf_utilities/utils.py
+drwxr-xr-x   0 dwl2x     (1000) users      (100)        0 2023-05-05 05:42:43.682502 tf-utilities-0.1.9/src/tf_utilities.egg-info/
+-rw-r--r--   0 dwl2x     (1000) users      (100)     3634 2023-05-05 05:42:43.000000 tf-utilities-0.1.9/src/tf_utilities.egg-info/PKG-INFO
+-rw-r--r--   0 dwl2x     (1000) users      (100)      457 2023-05-05 05:42:43.000000 tf-utilities-0.1.9/src/tf_utilities.egg-info/SOURCES.txt
+-rw-r--r--   0 dwl2x     (1000) users      (100)        1 2023-05-05 05:42:43.000000 tf-utilities-0.1.9/src/tf_utilities.egg-info/dependency_links.txt
+-rw-r--r--   0 dwl2x     (1000) users      (100)       22 2023-05-05 05:42:43.000000 tf-utilities-0.1.9/src/tf_utilities.egg-info/requires.txt
+-rw-r--r--   0 dwl2x     (1000) users      (100)       13 2023-05-05 05:42:43.000000 tf-utilities-0.1.9/src/tf_utilities.egg-info/top_level.txt
```

### Comparing `tf-utilities-0.1.8/LICENSE` & `tf-utilities-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `tf-utilities-0.1.8/PKG-INFO` & `tf-utilities-0.1.9/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tf-utilities
-Version: 0.1.8
+Version: 0.1.9
 Summary: A light-weight library of utilities for TensorFlow 2/Keras.
 Author-email: David Ludwig <davidludwigii@gmail.com>
 License: Copyright (c) 2012-2022 Scott Chacon and others
         
         Permission is hereby granted, free of charge, to any person obtaining
         a copy of this software and associated documentation files (the
         "Software"), to deal in the Software without restriction, including
```

### Comparing `tf-utilities-0.1.8/README.md` & `tf-utilities-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `tf-utilities-0.1.8/pyproject.toml` & `tf-utilities-0.1.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "tf-utilities"
-version = "0.1.8"
+version = "0.1.9"
 authors = [
   { name="David Ludwig", email="davidludwigii@gmail.com" },
 ]
 description = "A light-weight library of utilities for TensorFlow 2/Keras."
 readme = "README.md"
 license = { file="LICENSE" }
 requires-python = ">=3.7"
```

### Comparing `tf-utilities-0.1.8/src/tf_utilities/data.py` & `tf-utilities-0.1.9/src/tf_utilities/data.py`

 * *Files identical despite different names*

### Comparing `tf-utilities-0.1.8/src/tf_utilities/devices.py` & `tf-utilities-0.1.9/src/tf_utilities/devices.py`

 * *Files identical despite different names*

### Comparing `tf-utilities-0.1.8/src/tf_utilities/scripting.py` & `tf-utilities-0.1.9/src/tf_utilities/scripting.py`

 * *Files identical despite different names*

### Comparing `tf-utilities-0.1.8/src/tf_utilities/strategy.py` & `tf-utilities-0.1.9/src/tf_utilities/strategy.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import tensorflow as tf
 from . import devices
 
 def create_strategy(cpus=[], gpus=[]):
     ids = [devices.device_id(device) for device in cpus + gpus]
     if len(gpus) < 2:
         return tf.distribute.OneDeviceStrategy(ids[-1])
-    return tf.distribute.MirroredStrategy(ids)
+    return tf.distribute.MirroredStrategy(ids[len(cpus):])
 
 def cpu(index: int=0):
     cpus = devices.select_cpu(index)
     return create_strategy(cpus)
 
 def gpu(indices: int=None, cpu_index=0, use_dynamic_memory=True):
     cpus, gpus = devices.select_gpu(indices, cpu_index, use_dynamic_memory)
```

### Comparing `tf-utilities-0.1.8/src/tf_utilities/subbatching.py` & `tf-utilities-0.1.9/src/tf_utilities/subbatching.py`

 * *Files identical despite different names*

### Comparing `tf-utilities-0.1.8/src/tf_utilities.egg-info/PKG-INFO` & `tf-utilities-0.1.9/src/tf_utilities.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tf-utilities
-Version: 0.1.8
+Version: 0.1.9
 Summary: A light-weight library of utilities for TensorFlow 2/Keras.
 Author-email: David Ludwig <davidludwigii@gmail.com>
 License: Copyright (c) 2012-2022 Scott Chacon and others
         
         Permission is hereby granted, free of charge, to any person obtaining
         a copy of this software and associated documentation files (the
         "Software"), to deal in the Software without restriction, including
```

