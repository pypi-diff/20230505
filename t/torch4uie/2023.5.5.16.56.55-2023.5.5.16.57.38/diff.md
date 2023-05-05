# Comparing `tmp/torch4uie-2023.5.5.16.56.55.tar.gz` & `tmp/torch4uie-2023.5.5.16.57.38.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "torch4uie-2023.5.5.16.56.55.tar", last modified: Fri May  5 08:56:55 2023, max compression
+gzip compressed data, was "torch4uie-2023.5.5.16.57.38.tar", last modified: Fri May  5 08:57:38 2023, max compression
```

## Comparing `torch4uie-2023.5.5.16.56.55.tar` & `torch4uie-2023.5.5.16.57.38.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-05-05 08:56:55.286204 torch4uie-2023.5.5.16.56.55/
--rw-r--r--   0 betterme   (501) staff       (20)     1196 2023-04-20 11:38:14.000000 torch4uie-2023.5.5.16.56.55/.gitignore
--rw-r--r--   0 betterme   (501) staff       (20)      289 2023-04-11 04:23:57.000000 torch4uie-2023.5.5.16.56.55/MANIFEST.in
--rw-r--r--   0 betterme   (501) staff       (20)    41295 2023-05-05 08:56:55.285986 torch4uie-2023.5.5.16.56.55/PKG-INFO
--rw-r--r--   0 betterme   (501) staff       (20)    40600 2023-05-05 08:24:54.000000 torch4uie-2023.5.5.16.56.55/README.md
--rw-r--r--   0 betterme   (501) staff       (20)      104 2023-05-05 08:55:51.000000 torch4uie-2023.5.5.16.56.55/requirements.txt
--rw-r--r--   0 betterme   (501) staff       (20)       38 2023-05-05 08:56:55.286276 torch4uie-2023.5.5.16.56.55/setup.cfg
--rw-r--r--   0 betterme   (501) staff       (20)     1754 2023-05-05 08:56:54.000000 torch4uie-2023.5.5.16.56.55/setup.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-05-05 08:56:55.283427 torch4uie-2023.5.5.16.56.55/torch4uie.egg-info/
--rw-r--r--   0 betterme   (501) staff       (20)    41295 2023-05-05 08:56:55.000000 torch4uie-2023.5.5.16.56.55/torch4uie.egg-info/PKG-INFO
--rw-r--r--   0 betterme   (501) staff       (20)      497 2023-05-05 08:56:55.000000 torch4uie-2023.5.5.16.56.55/torch4uie.egg-info/SOURCES.txt
--rw-r--r--   0 betterme   (501) staff       (20)        1 2023-05-05 08:56:55.000000 torch4uie-2023.5.5.16.56.55/torch4uie.egg-info/dependency_links.txt
--rw-r--r--   0 betterme   (501) staff       (20)       53 2023-05-05 08:56:55.000000 torch4uie-2023.5.5.16.56.55/torch4uie.egg-info/entry_points.txt
--rw-r--r--   0 betterme   (501) staff       (20)        1 2023-05-05 08:56:55.000000 torch4uie-2023.5.5.16.56.55/torch4uie.egg-info/not-zip-safe
--rw-r--r--   0 betterme   (501) staff       (20)      111 2023-05-05 08:56:55.000000 torch4uie-2023.5.5.16.56.55/torch4uie.egg-info/requires.txt
--rw-r--r--   0 betterme   (501) staff       (20)        4 2023-05-05 08:56:55.000000 torch4uie-2023.5.5.16.56.55/torch4uie.egg-info/top_level.txt
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-05-05 08:56:55.285692 torch4uie-2023.5.5.16.56.55/uie/
--rw-r--r--   0 betterme   (501) staff       (20)      266 2023-05-05 08:50:31.000000 torch4uie-2023.5.5.16.56.55/uie/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)    24308 2023-05-05 08:24:54.000000 torch4uie-2023.5.5.16.56.55/uie/convert.py
--rw-r--r--   0 betterme   (501) staff       (20)     8474 2023-05-05 08:24:54.000000 torch4uie-2023.5.5.16.56.55/uie/doccano.py
--rw-r--r--   0 betterme   (501) staff       (20)    48643 2023-05-05 08:24:54.000000 torch4uie-2023.5.5.16.56.55/uie/ernie.py
--rw-r--r--   0 betterme   (501) staff       (20)    43974 2023-05-05 08:24:54.000000 torch4uie-2023.5.5.16.56.55/uie/ernie_m.py
--rw-r--r--   0 betterme   (501) staff       (20)     6757 2023-05-05 08:24:54.000000 torch4uie-2023.5.5.16.56.55/uie/evaluate.py
--rw-r--r--   0 betterme   (501) staff       (20)     7802 2023-05-05 08:24:54.000000 torch4uie-2023.5.5.16.56.55/uie/export_model.py
--rw-r--r--   0 betterme   (501) staff       (20)    11286 2023-05-05 08:24:54.000000 torch4uie-2023.5.5.16.56.55/uie/finetune.py
--rw-r--r--   0 betterme   (501) staff       (20)     3707 2023-05-05 08:24:54.000000 torch4uie-2023.5.5.16.56.55/uie/labelstudio2doccano.py
--rw-r--r--   0 betterme   (501) staff       (20)    16534 2023-05-05 08:24:54.000000 torch4uie-2023.5.5.16.56.55/uie/model.py
--rw-r--r--   0 betterme   (501) staff       (20)    28015 2023-05-05 08:24:54.000000 torch4uie-2023.5.5.16.56.55/uie/tokenizer.py
--rw-r--r--   0 betterme   (501) staff       (20)    27756 2023-05-05 08:47:28.000000 torch4uie-2023.5.5.16.56.55/uie/uie.py
--rw-r--r--   0 betterme   (501) staff       (20)    46414 2023-05-05 08:24:54.000000 torch4uie-2023.5.5.16.56.55/uie/utils.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-05-05 08:57:38.577217 torch4uie-2023.5.5.16.57.38/
+-rw-r--r--   0 betterme   (501) staff       (20)     1196 2023-04-20 11:38:14.000000 torch4uie-2023.5.5.16.57.38/.gitignore
+-rw-r--r--   0 betterme   (501) staff       (20)      289 2023-04-11 04:23:57.000000 torch4uie-2023.5.5.16.57.38/MANIFEST.in
+-rw-r--r--   0 betterme   (501) staff       (20)    41295 2023-05-05 08:57:38.577057 torch4uie-2023.5.5.16.57.38/PKG-INFO
+-rw-r--r--   0 betterme   (501) staff       (20)    40600 2023-05-05 08:24:54.000000 torch4uie-2023.5.5.16.57.38/README.md
+-rw-r--r--   0 betterme   (501) staff       (20)       97 2023-05-05 08:57:37.000000 torch4uie-2023.5.5.16.57.38/requirements.txt
+-rw-r--r--   0 betterme   (501) staff       (20)       38 2023-05-05 08:57:38.577260 torch4uie-2023.5.5.16.57.38/setup.cfg
+-rw-r--r--   0 betterme   (501) staff       (20)     1754 2023-05-05 08:56:54.000000 torch4uie-2023.5.5.16.57.38/setup.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-05-05 08:57:38.574958 torch4uie-2023.5.5.16.57.38/torch4uie.egg-info/
+-rw-r--r--   0 betterme   (501) staff       (20)    41295 2023-05-05 08:57:38.000000 torch4uie-2023.5.5.16.57.38/torch4uie.egg-info/PKG-INFO
+-rw-r--r--   0 betterme   (501) staff       (20)      497 2023-05-05 08:57:38.000000 torch4uie-2023.5.5.16.57.38/torch4uie.egg-info/SOURCES.txt
+-rw-r--r--   0 betterme   (501) staff       (20)        1 2023-05-05 08:57:38.000000 torch4uie-2023.5.5.16.57.38/torch4uie.egg-info/dependency_links.txt
+-rw-r--r--   0 betterme   (501) staff       (20)       53 2023-05-05 08:57:38.000000 torch4uie-2023.5.5.16.57.38/torch4uie.egg-info/entry_points.txt
+-rw-r--r--   0 betterme   (501) staff       (20)        1 2023-05-05 08:57:38.000000 torch4uie-2023.5.5.16.57.38/torch4uie.egg-info/not-zip-safe
+-rw-r--r--   0 betterme   (501) staff       (20)      104 2023-05-05 08:57:38.000000 torch4uie-2023.5.5.16.57.38/torch4uie.egg-info/requires.txt
+-rw-r--r--   0 betterme   (501) staff       (20)        4 2023-05-05 08:57:38.000000 torch4uie-2023.5.5.16.57.38/torch4uie.egg-info/top_level.txt
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-05-05 08:57:38.576780 torch4uie-2023.5.5.16.57.38/uie/
+-rw-r--r--   0 betterme   (501) staff       (20)      266 2023-05-05 08:50:31.000000 torch4uie-2023.5.5.16.57.38/uie/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)    24308 2023-05-05 08:24:54.000000 torch4uie-2023.5.5.16.57.38/uie/convert.py
+-rw-r--r--   0 betterme   (501) staff       (20)     8474 2023-05-05 08:24:54.000000 torch4uie-2023.5.5.16.57.38/uie/doccano.py
+-rw-r--r--   0 betterme   (501) staff       (20)    48643 2023-05-05 08:24:54.000000 torch4uie-2023.5.5.16.57.38/uie/ernie.py
+-rw-r--r--   0 betterme   (501) staff       (20)    43974 2023-05-05 08:24:54.000000 torch4uie-2023.5.5.16.57.38/uie/ernie_m.py
+-rw-r--r--   0 betterme   (501) staff       (20)     6757 2023-05-05 08:24:54.000000 torch4uie-2023.5.5.16.57.38/uie/evaluate.py
+-rw-r--r--   0 betterme   (501) staff       (20)     7802 2023-05-05 08:24:54.000000 torch4uie-2023.5.5.16.57.38/uie/export_model.py
+-rw-r--r--   0 betterme   (501) staff       (20)    11286 2023-05-05 08:24:54.000000 torch4uie-2023.5.5.16.57.38/uie/finetune.py
+-rw-r--r--   0 betterme   (501) staff       (20)     3707 2023-05-05 08:24:54.000000 torch4uie-2023.5.5.16.57.38/uie/labelstudio2doccano.py
+-rw-r--r--   0 betterme   (501) staff       (20)    16534 2023-05-05 08:24:54.000000 torch4uie-2023.5.5.16.57.38/uie/model.py
+-rw-r--r--   0 betterme   (501) staff       (20)    28015 2023-05-05 08:24:54.000000 torch4uie-2023.5.5.16.57.38/uie/tokenizer.py
+-rw-r--r--   0 betterme   (501) staff       (20)    27756 2023-05-05 08:47:28.000000 torch4uie-2023.5.5.16.57.38/uie/uie.py
+-rw-r--r--   0 betterme   (501) staff       (20)    46414 2023-05-05 08:24:54.000000 torch4uie-2023.5.5.16.57.38/uie/utils.py
```

### Comparing `torch4uie-2023.5.5.16.56.55/.gitignore` & `torch4uie-2023.5.5.16.57.38/.gitignore`

 * *Files identical despite different names*

### Comparing `torch4uie-2023.5.5.16.56.55/PKG-INFO` & `torch4uie-2023.5.5.16.57.38/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: torch4uie
-Version: 2023.5.5.16.56.55
+Version: 2023.5.5.16.57.38
 Summary: Create a Python package.
 Home-page: https://github.com/yuanjie-ai/ChatLLM
 Author: yuanjie
 Author-email: 313303303@qq.com
 License: MIT license
 Keywords: uie
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `torch4uie-2023.5.5.16.56.55/README.md` & `torch4uie-2023.5.5.16.57.38/README.md`

 * *Files identical despite different names*

### Comparing `torch4uie-2023.5.5.16.56.55/setup.py` & `torch4uie-2023.5.5.16.57.38/setup.py`

 * *Files identical despite different names*

### Comparing `torch4uie-2023.5.5.16.56.55/torch4uie.egg-info/PKG-INFO` & `torch4uie-2023.5.5.16.57.38/torch4uie.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: torch4uie
-Version: 2023.5.5.16.56.55
+Version: 2023.5.5.16.57.38
 Summary: Create a Python package.
 Home-page: https://github.com/yuanjie-ai/ChatLLM
 Author: yuanjie
 Author-email: 313303303@qq.com
 License: MIT license
 Keywords: uie
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `torch4uie-2023.5.5.16.56.55/uie/convert.py` & `torch4uie-2023.5.5.16.57.38/uie/convert.py`

 * *Files identical despite different names*

### Comparing `torch4uie-2023.5.5.16.56.55/uie/doccano.py` & `torch4uie-2023.5.5.16.57.38/uie/doccano.py`

 * *Files identical despite different names*

### Comparing `torch4uie-2023.5.5.16.56.55/uie/ernie.py` & `torch4uie-2023.5.5.16.57.38/uie/ernie.py`

 * *Files identical despite different names*

### Comparing `torch4uie-2023.5.5.16.56.55/uie/ernie_m.py` & `torch4uie-2023.5.5.16.57.38/uie/ernie_m.py`

 * *Files identical despite different names*

### Comparing `torch4uie-2023.5.5.16.56.55/uie/evaluate.py` & `torch4uie-2023.5.5.16.57.38/uie/evaluate.py`

 * *Files identical despite different names*

### Comparing `torch4uie-2023.5.5.16.56.55/uie/export_model.py` & `torch4uie-2023.5.5.16.57.38/uie/export_model.py`

 * *Files identical despite different names*

### Comparing `torch4uie-2023.5.5.16.56.55/uie/finetune.py` & `torch4uie-2023.5.5.16.57.38/uie/finetune.py`

 * *Files identical despite different names*

### Comparing `torch4uie-2023.5.5.16.56.55/uie/labelstudio2doccano.py` & `torch4uie-2023.5.5.16.57.38/uie/labelstudio2doccano.py`

 * *Files identical despite different names*

### Comparing `torch4uie-2023.5.5.16.56.55/uie/model.py` & `torch4uie-2023.5.5.16.57.38/uie/model.py`

 * *Files identical despite different names*

### Comparing `torch4uie-2023.5.5.16.56.55/uie/tokenizer.py` & `torch4uie-2023.5.5.16.57.38/uie/tokenizer.py`

 * *Files identical despite different names*

### Comparing `torch4uie-2023.5.5.16.56.55/uie/uie.py` & `torch4uie-2023.5.5.16.57.38/uie/uie.py`

 * *Files identical despite different names*

### Comparing `torch4uie-2023.5.5.16.56.55/uie/utils.py` & `torch4uie-2023.5.5.16.57.38/uie/utils.py`

 * *Files identical despite different names*

