# Comparing `tmp/simplepytorch-1.3.0.tar.gz` & `tmp/simplepytorch-1.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "simplepytorch-1.3.0.tar", last modified: Thu May  4 15:20:22 2023, max compression
+gzip compressed data, was "simplepytorch-1.4.0.tar", last modified: Fri May  5 12:34:48 2023, max compression
```

## Comparing `simplepytorch-1.3.0.tar` & `simplepytorch-1.4.0.tar`

### file list

```diff
@@ -1,47 +1,47 @@
-drwxr-xr-x   0 alex      (1000) alex      (1000)        0 2023-05-04 15:20:22.863541 simplepytorch-1.3.0/
--rw-r--r--   0 alex      (1000) alex      (1000)     1068 2020-02-19 20:04:28.000000 simplepytorch-1.3.0/LICENSE
--rw-r--r--   0 alex      (1000) alex      (1000)     3278 2023-05-04 15:20:22.863541 simplepytorch-1.3.0/PKG-INFO
--rw-r--r--   0 alex      (1000) alex      (1000)     2847 2022-04-26 04:35:00.000000 simplepytorch-1.3.0/README.md
-drwxr-xr-x   0 alex      (1000) alex      (1000)        0 2023-05-04 15:20:22.856874 simplepytorch-1.3.0/bin/
--rwxr-xr-x   0 alex      (1000) alex      (1000)       48 2021-01-20 01:32:25.000000 simplepytorch-1.3.0/bin/simplepytorch
--rwxr-xr-x   0 alex      (1000) alex      (1000)       90 2021-01-20 01:32:25.000000 simplepytorch-1.3.0/bin/simplepytorch_debug
--rwxr-xr-x   0 alex      (1000) alex      (1000)       80 2021-01-21 15:57:18.000000 simplepytorch-1.3.0/bin/simplepytorch_plot
--rw-r--r--   0 alex      (1000) alex      (1000)      248 2023-05-04 15:20:22.863541 simplepytorch-1.3.0/setup.cfg
--rwxr-xr-x   0 alex      (1000) alex      (1000)     1160 2023-05-04 15:20:22.000000 simplepytorch-1.3.0/setup.py
-drwxr-xr-x   0 alex      (1000) alex      (1000)        0 2023-05-04 15:20:22.860208 simplepytorch-1.3.0/simplepytorch/
--rw-r--r--   0 alex      (1000) alex      (1000)       22 2023-05-04 15:20:22.000000 simplepytorch-1.3.0/simplepytorch/__init__.py
--rw-r--r--   0 alex      (1000) alex      (1000)       70 2020-06-07 00:23:22.000000 simplepytorch-1.3.0/simplepytorch/__main__.py
--rw-r--r--   0 alex      (1000) alex      (1000)     1204 2022-04-25 14:00:07.000000 simplepytorch-1.3.0/simplepytorch/api.py
--rw-r--r--   0 alex      (1000) alex      (1000)      893 2020-02-19 20:04:28.000000 simplepytorch-1.3.0/simplepytorch/cache.py
--rw-r--r--   0 alex      (1000) alex      (1000)    10311 2022-04-25 13:58:29.000000 simplepytorch-1.3.0/simplepytorch/cmdline.py
-drwxr-xr-x   0 alex      (1000) alex      (1000)        0 2023-05-04 15:20:22.863541 simplepytorch-1.3.0/simplepytorch/datasets/
--rw-r--r--   0 alex      (1000) alex      (1000)     6406 2021-06-13 22:51:00.000000 simplepytorch-1.3.0/simplepytorch/datasets/BBBC038v1_microscopy.py
--rw-r--r--   0 alex      (1000) alex      (1000)      680 2023-03-08 17:21:22.000000 simplepytorch-1.3.0/simplepytorch/datasets/__init__.py
--rw-r--r--   0 alex      (1000) alex      (1000)     1772 2020-02-19 20:04:28.000000 simplepytorch-1.3.0/simplepytorch/datasets/_shared.py
--rw-r--r--   0 alex      (1000) alex      (1000)    10986 2022-11-26 10:17:09.000000 simplepytorch-1.3.0/simplepytorch/datasets/chexpert.py
--rw-r--r--   0 alex      (1000) alex      (1000)     5543 2020-09-08 08:18:00.000000 simplepytorch-1.3.0/simplepytorch/datasets/drive.py
--rw-r--r--   0 alex      (1000) alex      (1000)     2255 2021-09-22 22:34:28.000000 simplepytorch-1.3.0/simplepytorch/datasets/eyepacs.py
--rw-r--r--   0 alex      (1000) alex      (1000)     1112 2021-09-22 22:34:44.000000 simplepytorch-1.3.0/simplepytorch/datasets/glob_image_dir.py
--rw-r--r--   0 alex      (1000) alex      (1000)     3778 2020-02-19 20:04:28.000000 simplepytorch-1.3.0/simplepytorch/datasets/idrid.py
--rw-r--r--   0 alex      (1000) alex      (1000)    16323 2022-05-16 13:41:31.000000 simplepytorch-1.3.0/simplepytorch/datasets/intel_mobileodt_cervical.py
--rw-r--r--   0 alex      (1000) alex      (1000)     1623 2022-05-31 17:45:19.000000 simplepytorch-1.3.0/simplepytorch/datasets/kimeye.py
--rw-r--r--   0 alex      (1000) alex      (1000)     4024 2020-02-19 20:04:28.000000 simplepytorch-1.3.0/simplepytorch/datasets/messidor.py
--rw-r--r--   0 alex      (1000) alex      (1000)     1385 2020-02-19 20:04:28.000000 simplepytorch-1.3.0/simplepytorch/datasets/pickled_dicts.py
--rw-r--r--   0 alex      (1000) alex      (1000)     1314 2022-04-13 00:39:21.000000 simplepytorch-1.3.0/simplepytorch/datasets/preprocess.py
--rw-r--r--   0 alex      (1000) alex      (1000)     9228 2022-04-25 16:29:13.000000 simplepytorch-1.3.0/simplepytorch/datasets/qualdr.py
--rw-r--r--   0 alex      (1000) alex      (1000)     3277 2020-02-19 20:04:28.000000 simplepytorch-1.3.0/simplepytorch/datasets/rite.py
--rw-r--r--   0 alex      (1000) alex      (1000)     1300 2020-02-19 20:04:28.000000 simplepytorch-1.3.0/simplepytorch/datasets/train_val_test_split.py
--rw-r--r--   0 alex      (1000) alex      (1000)     1681 2020-02-19 20:04:28.000000 simplepytorch-1.3.0/simplepytorch/early_stopping.py
--rw-r--r--   0 alex      (1000) alex      (1000)    16202 2022-04-25 13:56:13.000000 simplepytorch-1.3.0/simplepytorch/feedforward.py
--rw-r--r--   0 alex      (1000) alex      (1000)    17470 2022-04-25 23:56:47.000000 simplepytorch-1.3.0/simplepytorch/logging_tools.py
--rw-r--r--   0 alex      (1000) alex      (1000)    14712 2023-05-04 15:00:05.000000 simplepytorch-1.3.0/simplepytorch/metrics.py
--rwxr-xr-x   0 alex      (1000) alex      (1000)    21766 2023-02-07 12:06:45.000000 simplepytorch-1.3.0/simplepytorch/plot_perf.py
--rw-r--r--   0 alex      (1000) alex      (1000)     6102 2022-05-01 10:43:51.000000 simplepytorch-1.3.0/simplepytorch/raytunelib.py
--rw-r--r--   0 alex      (1000) alex      (1000)    21377 2023-05-04 15:18:50.000000 simplepytorch-1.3.0/simplepytorch/result.py
--rw-r--r--   0 alex      (1000) alex      (1000)    16501 2022-11-24 23:35:20.000000 simplepytorch-1.3.0/simplepytorch/trainlib.py
-drwxr-xr-x   0 alex      (1000) alex      (1000)        0 2023-05-04 15:20:22.860208 simplepytorch-1.3.0/simplepytorch.egg-info/
--rw-r--r--   0 alex      (1000) alex      (1000)     3278 2023-05-04 15:20:22.000000 simplepytorch-1.3.0/simplepytorch.egg-info/PKG-INFO
--rw-r--r--   0 alex      (1000) alex      (1000)     1229 2023-05-04 15:20:22.000000 simplepytorch-1.3.0/simplepytorch.egg-info/SOURCES.txt
--rw-r--r--   0 alex      (1000) alex      (1000)        1 2023-05-04 15:20:22.000000 simplepytorch-1.3.0/simplepytorch.egg-info/dependency_links.txt
--rw-r--r--   0 alex      (1000) alex      (1000)      180 2023-05-04 15:20:22.000000 simplepytorch-1.3.0/simplepytorch.egg-info/requires.txt
--rw-r--r--   0 alex      (1000) alex      (1000)       14 2023-05-04 15:20:22.000000 simplepytorch-1.3.0/simplepytorch.egg-info/top_level.txt
+drwxr-xr-x   0 alex      (1000) alex      (1000)        0 2023-05-05 12:34:48.027839 simplepytorch-1.4.0/
+-rw-r--r--   0 alex      (1000) alex      (1000)     1068 2020-02-19 20:04:28.000000 simplepytorch-1.4.0/LICENSE
+-rw-r--r--   0 alex      (1000) alex      (1000)     3278 2023-05-05 12:34:48.027839 simplepytorch-1.4.0/PKG-INFO
+-rw-r--r--   0 alex      (1000) alex      (1000)     2847 2022-04-26 04:35:00.000000 simplepytorch-1.4.0/README.md
+drwxr-xr-x   0 alex      (1000) alex      (1000)        0 2023-05-05 12:34:48.024506 simplepytorch-1.4.0/bin/
+-rwxr-xr-x   0 alex      (1000) alex      (1000)       48 2021-01-20 01:32:25.000000 simplepytorch-1.4.0/bin/simplepytorch
+-rwxr-xr-x   0 alex      (1000) alex      (1000)       90 2021-01-20 01:32:25.000000 simplepytorch-1.4.0/bin/simplepytorch_debug
+-rwxr-xr-x   0 alex      (1000) alex      (1000)       80 2021-01-21 15:57:18.000000 simplepytorch-1.4.0/bin/simplepytorch_plot
+-rw-r--r--   0 alex      (1000) alex      (1000)      248 2023-05-05 12:34:48.027839 simplepytorch-1.4.0/setup.cfg
+-rwxr-xr-x   0 alex      (1000) alex      (1000)     1160 2023-05-05 12:34:47.000000 simplepytorch-1.4.0/setup.py
+drwxr-xr-x   0 alex      (1000) alex      (1000)        0 2023-05-05 12:34:48.024506 simplepytorch-1.4.0/simplepytorch/
+-rw-r--r--   0 alex      (1000) alex      (1000)       22 2023-05-05 12:34:47.000000 simplepytorch-1.4.0/simplepytorch/__init__.py
+-rw-r--r--   0 alex      (1000) alex      (1000)       70 2020-06-07 00:23:22.000000 simplepytorch-1.4.0/simplepytorch/__main__.py
+-rw-r--r--   0 alex      (1000) alex      (1000)     1204 2022-04-25 14:00:07.000000 simplepytorch-1.4.0/simplepytorch/api.py
+-rw-r--r--   0 alex      (1000) alex      (1000)      893 2020-02-19 20:04:28.000000 simplepytorch-1.4.0/simplepytorch/cache.py
+-rw-r--r--   0 alex      (1000) alex      (1000)    10311 2022-04-25 13:58:29.000000 simplepytorch-1.4.0/simplepytorch/cmdline.py
+drwxr-xr-x   0 alex      (1000) alex      (1000)        0 2023-05-05 12:34:48.027839 simplepytorch-1.4.0/simplepytorch/datasets/
+-rw-r--r--   0 alex      (1000) alex      (1000)     6406 2021-06-13 22:51:00.000000 simplepytorch-1.4.0/simplepytorch/datasets/BBBC038v1_microscopy.py
+-rw-r--r--   0 alex      (1000) alex      (1000)      680 2023-03-08 17:21:22.000000 simplepytorch-1.4.0/simplepytorch/datasets/__init__.py
+-rw-r--r--   0 alex      (1000) alex      (1000)     1772 2020-02-19 20:04:28.000000 simplepytorch-1.4.0/simplepytorch/datasets/_shared.py
+-rw-r--r--   0 alex      (1000) alex      (1000)    10986 2022-11-26 10:17:09.000000 simplepytorch-1.4.0/simplepytorch/datasets/chexpert.py
+-rw-r--r--   0 alex      (1000) alex      (1000)     5543 2020-09-08 08:18:00.000000 simplepytorch-1.4.0/simplepytorch/datasets/drive.py
+-rw-r--r--   0 alex      (1000) alex      (1000)     2255 2021-09-22 22:34:28.000000 simplepytorch-1.4.0/simplepytorch/datasets/eyepacs.py
+-rw-r--r--   0 alex      (1000) alex      (1000)     1112 2021-09-22 22:34:44.000000 simplepytorch-1.4.0/simplepytorch/datasets/glob_image_dir.py
+-rw-r--r--   0 alex      (1000) alex      (1000)     3778 2020-02-19 20:04:28.000000 simplepytorch-1.4.0/simplepytorch/datasets/idrid.py
+-rw-r--r--   0 alex      (1000) alex      (1000)    16323 2022-05-16 13:41:31.000000 simplepytorch-1.4.0/simplepytorch/datasets/intel_mobileodt_cervical.py
+-rw-r--r--   0 alex      (1000) alex      (1000)     1623 2022-05-31 17:45:19.000000 simplepytorch-1.4.0/simplepytorch/datasets/kimeye.py
+-rw-r--r--   0 alex      (1000) alex      (1000)     4024 2020-02-19 20:04:28.000000 simplepytorch-1.4.0/simplepytorch/datasets/messidor.py
+-rw-r--r--   0 alex      (1000) alex      (1000)     1385 2020-02-19 20:04:28.000000 simplepytorch-1.4.0/simplepytorch/datasets/pickled_dicts.py
+-rw-r--r--   0 alex      (1000) alex      (1000)     1314 2022-04-13 00:39:21.000000 simplepytorch-1.4.0/simplepytorch/datasets/preprocess.py
+-rw-r--r--   0 alex      (1000) alex      (1000)     9228 2022-04-25 16:29:13.000000 simplepytorch-1.4.0/simplepytorch/datasets/qualdr.py
+-rw-r--r--   0 alex      (1000) alex      (1000)     3277 2020-02-19 20:04:28.000000 simplepytorch-1.4.0/simplepytorch/datasets/rite.py
+-rw-r--r--   0 alex      (1000) alex      (1000)     1300 2020-02-19 20:04:28.000000 simplepytorch-1.4.0/simplepytorch/datasets/train_val_test_split.py
+-rw-r--r--   0 alex      (1000) alex      (1000)     1681 2020-02-19 20:04:28.000000 simplepytorch-1.4.0/simplepytorch/early_stopping.py
+-rw-r--r--   0 alex      (1000) alex      (1000)    16202 2022-04-25 13:56:13.000000 simplepytorch-1.4.0/simplepytorch/feedforward.py
+-rw-r--r--   0 alex      (1000) alex      (1000)    17470 2022-04-25 23:56:47.000000 simplepytorch-1.4.0/simplepytorch/logging_tools.py
+-rw-r--r--   0 alex      (1000) alex      (1000)    14712 2023-05-04 15:00:05.000000 simplepytorch-1.4.0/simplepytorch/metrics.py
+-rwxr-xr-x   0 alex      (1000) alex      (1000)    21766 2023-02-07 12:06:45.000000 simplepytorch-1.4.0/simplepytorch/plot_perf.py
+-rw-r--r--   0 alex      (1000) alex      (1000)     6102 2022-05-01 10:43:51.000000 simplepytorch-1.4.0/simplepytorch/raytunelib.py
+-rw-r--r--   0 alex      (1000) alex      (1000)    22035 2023-05-05 12:32:38.000000 simplepytorch-1.4.0/simplepytorch/result.py
+-rw-r--r--   0 alex      (1000) alex      (1000)    16501 2022-11-24 23:35:20.000000 simplepytorch-1.4.0/simplepytorch/trainlib.py
+drwxr-xr-x   0 alex      (1000) alex      (1000)        0 2023-05-05 12:34:48.024506 simplepytorch-1.4.0/simplepytorch.egg-info/
+-rw-r--r--   0 alex      (1000) alex      (1000)     3278 2023-05-05 12:34:47.000000 simplepytorch-1.4.0/simplepytorch.egg-info/PKG-INFO
+-rw-r--r--   0 alex      (1000) alex      (1000)     1229 2023-05-05 12:34:47.000000 simplepytorch-1.4.0/simplepytorch.egg-info/SOURCES.txt
+-rw-r--r--   0 alex      (1000) alex      (1000)        1 2023-05-05 12:34:47.000000 simplepytorch-1.4.0/simplepytorch.egg-info/dependency_links.txt
+-rw-r--r--   0 alex      (1000) alex      (1000)      180 2023-05-05 12:34:47.000000 simplepytorch-1.4.0/simplepytorch.egg-info/requires.txt
+-rw-r--r--   0 alex      (1000) alex      (1000)       14 2023-05-05 12:34:47.000000 simplepytorch-1.4.0/simplepytorch.egg-info/top_level.txt
```

### Comparing `simplepytorch-1.3.0/LICENSE` & `simplepytorch-1.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `simplepytorch-1.3.0/PKG-INFO` & `simplepytorch-1.4.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: simplepytorch
-Version: 1.3.0
+Version: 1.4.0
 Summary: Setup and train deep nets with PyTorch. Opinionated and Simple.
 Home-page: https://github.com/adgaudio/simplepytorch
 Author: Alex Gaudio
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.8
 Description-Content-Type: text/markdown
```

### Comparing `simplepytorch-1.3.0/README.md` & `simplepytorch-1.4.0/README.md`

 * *Files identical despite different names*

### Comparing `simplepytorch-1.3.0/setup.py` & `simplepytorch-1.4.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 
 # The text of the README file
 README = (HERE / "README.md").read_text()
 
 
 setup(
     name='simplepytorch',
-    version='1.3.0',
+    version='1.4.0',
     description='Setup and train deep nets with PyTorch. Opinionated and Simple.',
     long_description=README,
     long_description_content_type="text/markdown",
     url="https://github.com/adgaudio/simplepytorch",
     author='Alex Gaudio',
     license="MIT",
     classifiers=[
```

### Comparing `simplepytorch-1.3.0/simplepytorch/api.py` & `simplepytorch-1.4.0/simplepytorch/api.py`

 * *Files identical despite different names*

### Comparing `simplepytorch-1.3.0/simplepytorch/cache.py` & `simplepytorch-1.4.0/simplepytorch/cache.py`

 * *Files identical despite different names*

### Comparing `simplepytorch-1.3.0/simplepytorch/cmdline.py` & `simplepytorch-1.4.0/simplepytorch/cmdline.py`

 * *Files identical despite different names*

### Comparing `simplepytorch-1.3.0/simplepytorch/datasets/BBBC038v1_microscopy.py` & `simplepytorch-1.4.0/simplepytorch/datasets/BBBC038v1_microscopy.py`

 * *Files identical despite different names*

### Comparing `simplepytorch-1.3.0/simplepytorch/datasets/__init__.py` & `simplepytorch-1.4.0/simplepytorch/datasets/__init__.py`

 * *Files identical despite different names*

### Comparing `simplepytorch-1.3.0/simplepytorch/datasets/_shared.py` & `simplepytorch-1.4.0/simplepytorch/datasets/_shared.py`

 * *Files identical despite different names*

### Comparing `simplepytorch-1.3.0/simplepytorch/datasets/chexpert.py` & `simplepytorch-1.4.0/simplepytorch/datasets/chexpert.py`

 * *Files identical despite different names*

### Comparing `simplepytorch-1.3.0/simplepytorch/datasets/drive.py` & `simplepytorch-1.4.0/simplepytorch/datasets/drive.py`

 * *Files identical despite different names*

### Comparing `simplepytorch-1.3.0/simplepytorch/datasets/eyepacs.py` & `simplepytorch-1.4.0/simplepytorch/datasets/eyepacs.py`

 * *Files identical despite different names*

### Comparing `simplepytorch-1.3.0/simplepytorch/datasets/glob_image_dir.py` & `simplepytorch-1.4.0/simplepytorch/datasets/glob_image_dir.py`

 * *Files identical despite different names*

### Comparing `simplepytorch-1.3.0/simplepytorch/datasets/idrid.py` & `simplepytorch-1.4.0/simplepytorch/datasets/idrid.py`

 * *Files identical despite different names*

### Comparing `simplepytorch-1.3.0/simplepytorch/datasets/intel_mobileodt_cervical.py` & `simplepytorch-1.4.0/simplepytorch/datasets/intel_mobileodt_cervical.py`

 * *Files identical despite different names*

### Comparing `simplepytorch-1.3.0/simplepytorch/datasets/kimeye.py` & `simplepytorch-1.4.0/simplepytorch/datasets/kimeye.py`

 * *Files identical despite different names*

### Comparing `simplepytorch-1.3.0/simplepytorch/datasets/messidor.py` & `simplepytorch-1.4.0/simplepytorch/datasets/messidor.py`

 * *Files identical despite different names*

### Comparing `simplepytorch-1.3.0/simplepytorch/datasets/pickled_dicts.py` & `simplepytorch-1.4.0/simplepytorch/datasets/pickled_dicts.py`

 * *Files identical despite different names*

### Comparing `simplepytorch-1.3.0/simplepytorch/datasets/preprocess.py` & `simplepytorch-1.4.0/simplepytorch/datasets/preprocess.py`

 * *Files identical despite different names*

### Comparing `simplepytorch-1.3.0/simplepytorch/datasets/qualdr.py` & `simplepytorch-1.4.0/simplepytorch/datasets/qualdr.py`

 * *Files identical despite different names*

### Comparing `simplepytorch-1.3.0/simplepytorch/datasets/rite.py` & `simplepytorch-1.4.0/simplepytorch/datasets/rite.py`

 * *Files identical despite different names*

### Comparing `simplepytorch-1.3.0/simplepytorch/datasets/train_val_test_split.py` & `simplepytorch-1.4.0/simplepytorch/datasets/train_val_test_split.py`

 * *Files identical despite different names*

### Comparing `simplepytorch-1.3.0/simplepytorch/early_stopping.py` & `simplepytorch-1.4.0/simplepytorch/early_stopping.py`

 * *Files identical despite different names*

### Comparing `simplepytorch-1.3.0/simplepytorch/feedforward.py` & `simplepytorch-1.4.0/simplepytorch/feedforward.py`

 * *Files identical despite different names*

### Comparing `simplepytorch-1.3.0/simplepytorch/logging_tools.py` & `simplepytorch-1.4.0/simplepytorch/logging_tools.py`

 * *Files identical despite different names*

### Comparing `simplepytorch-1.3.0/simplepytorch/metrics.py` & `simplepytorch-1.4.0/simplepytorch/metrics.py`

 * *Files identical despite different names*

### Comparing `simplepytorch-1.3.0/simplepytorch/plot_perf.py` & `simplepytorch-1.4.0/simplepytorch/plot_perf.py`

 * *Files identical despite different names*

### Comparing `simplepytorch-1.3.0/simplepytorch/raytunelib.py` & `simplepytorch-1.4.0/simplepytorch/raytunelib.py`

 * *Files identical despite different names*

### Comparing `simplepytorch-1.3.0/simplepytorch/result.py` & `simplepytorch-1.4.0/simplepytorch/result.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 import dataclasses as dc
 import abc
 import torch as T
 from termcolor import colored
 import numpy as np
 
 from simplepytorch import metrics
-from sklearn.metrics import roc_auc_score
+from sklearn.metrics import roc_auc_score, average_precision_score
 
 
 class Result(abc.ABC):
     """
     Accumulate and analyze results, for instance over the course of one epoch.
 
     This is an abstract base class, meant to be subclassed.
@@ -360,15 +360,15 @@
     """A result class for Multi-Label Binary Classification.
     Maintains one binary confusion matrix for each class and computes
     classification metrics from them.
 
     This class is useful to to aggregate results, for instance over the course
     of an epoch.
     """
-    ALL_METRICS = ('Loss', 'Num Samples', 'MCC', 'Precision', 'Recall', 'F1', 'F1micro', 'Acc', 'BAcc', 'cm', 'ROC_AUC')  # 'y', 'yhat',
+    ALL_METRICS = ('Loss', 'Num Samples', 'MCC', 'Precision', 'Recall', 'F1', 'F1micro', 'Acc', 'BAcc', 'cm', 'ROC_AUC', 'AP')  # 'y', 'yhat',
 
     @property
     def metrics(self):
         return self._metrics
 
     def __init__(self, class_names:list,
                  binarize_fn:Callable[[T.Tensor, float],T.Tensor]=None,
@@ -405,15 +405,15 @@
         self.loss = 0
         self.num_samples = 0
         self.report_avg = report_avg
         self.device = device
         self.low_ram_mode = low_ram_mode
         self._ydata_fast = []  # only used if prioritize ram over compute
         self._yhdata_fast = []  # only used if prioritize ram over compute
-        if any(x in metrics for x in ['y', 'yhat', 'ROC_AUC']):
+        if any(x in metrics for x in ['y', 'yhat', 'ROC_AUC', 'AP']):
             self._ydata = OrderedDict((k, []) for k in class_names)
             self._yhatdata = OrderedDict((k, []) for k in class_names)
 
     @property
     def acc(self):
         """Accuracy"""
         return self._on_each_cm('Acc {class_name}', metrics.accuracy)
@@ -464,14 +464,31 @@
     def yhat(self):
         self._yhatdata = {k: [T.cat(v, 0)] if len(v) > 1 else v
                           for k, v in self._yhatdata.items()}
         return {f'yhat {class_name}': v[0].cpu().numpy().tolist() if len(v) else np.array([])
                 for class_name, v in self._yhatdata.items()}
 
     @property
+    def ap(self):
+        rv = {}
+        for kls, yval, yhatval in zip(self._cms, self.y.values(), self.yhat.values()):
+            key = f'AP {kls}'
+            if len(yval) <= 0:
+                rv[key] = 0
+                continue
+            # try:
+            rv[key] = average_precision_score(
+                y_true=yval, y_score=yhatval, average=None)
+            # except ValueError:
+            #     rv[key] = 0  # e.g. degenerate case when all classes are "0" or all are "1"
+        if self.report_avg:
+            rv['AP Macro-AVG'] = sum(rv.values()) / len(rv)
+        return rv
+
+    @property
     def roc_auc(self):
         rv = {}
         for kls, yval, yhatval in zip(self._cms, self.y.values(), self.yhat.values()):
             key = f'ROC_AUC {kls}'
             if len(yval) <= 0:
                 rv[key] = 0
                 continue
@@ -520,17 +537,17 @@
         """Less RAM usage, but slower"""
         binarized = self._binarize_fn(yhat, .5)
         assert binarized.dtype in (T.long, T.bool, T.int), 'sanity check binarize fn'
         assert binarized.shape == y.shape, 'sanity check binarize fn'
 
         for i, (kls, cm) in enumerate(self._cms.items()):
             cm += metrics.confusion_matrix(y[:, i], binarized[:, i], num_classes=2).to(self.device, non_blocking=True)
-            if 'y' in self.metrics or 'ROC_AUC' in self.metrics:
+            if any(x in self.metrics for x in ('y', 'ROC_AUC', 'AP')):
                 self._ydata[kls].append(y[:, i].to(self.device, non_blocking=True))
-            if 'yhat' in self.metrics or 'ROC_AUC' in self.metrics:
+            if any(x in self.metrics for x in ('yhat', 'ROC_AUC', 'AP')):
                 self._yhatdata[kls].append(yhat[:, i].to(self.device, non_blocking=True))
 
     def _update_fast(self, yhat, y) -> None:
         """More RAM usage, but faster"""
         self._yhdata_fast.append(yhat.to(self.device, non_blocking=True))
         self._ydata_fast.append(y.to(self.device, non_blocking=True))
```

### Comparing `simplepytorch-1.3.0/simplepytorch/trainlib.py` & `simplepytorch-1.4.0/simplepytorch/trainlib.py`

 * *Files identical despite different names*

### Comparing `simplepytorch-1.3.0/simplepytorch.egg-info/PKG-INFO` & `simplepytorch-1.4.0/simplepytorch.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: simplepytorch
-Version: 1.3.0
+Version: 1.4.0
 Summary: Setup and train deep nets with PyTorch. Opinionated and Simple.
 Home-page: https://github.com/adgaudio/simplepytorch
 Author: Alex Gaudio
 License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3.8
 Description-Content-Type: text/markdown
```

### Comparing `simplepytorch-1.3.0/simplepytorch.egg-info/SOURCES.txt` & `simplepytorch-1.4.0/simplepytorch.egg-info/SOURCES.txt`

 * *Files identical despite different names*

