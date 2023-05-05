# Comparing `tmp/nbdev-apl-0.0.753.tar.gz` & `tmp/nbdev-apl-0.0.754.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nbdev-apl-0.0.753.tar", last modified: Thu May  4 13:17:09 2023, max compression
+gzip compressed data, was "nbdev-apl-0.0.754.tar", last modified: Fri May  5 01:41:37 2023, max compression
```

## Comparing `nbdev-apl-0.0.753.tar` & `nbdev-apl-0.0.754.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 13:17:09.959384 nbdev-apl-0.0.753/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-04 13:06:14.000000 nbdev-apl-0.0.753/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-05-04 13:06:14.000000 nbdev-apl-0.0.753/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      839 2023-05-04 13:17:09.959384 nbdev-apl-0.0.753/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      122 2023-05-04 13:06:14.000000 nbdev-apl-0.0.753/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 13:17:09.959384 nbdev-apl-0.0.753/nbdev_apl/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 13:17:09.000000 nbdev-apl-0.0.753/nbdev_apl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5828 2023-05-04 13:06:14.000000 nbdev-apl-0.0.753/nbdev_apl/_modidx.py
--rw-r--r--   0 runner    (1001) docker     (123)      308 2023-05-04 13:17:09.000000 nbdev-apl-0.0.753/nbdev_apl/_nbdev.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 13:17:09.959384 nbdev-apl-0.0.753/nbdev_apl.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      839 2023-05-04 13:17:09.000000 nbdev-apl-0.0.753/nbdev_apl.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      346 2023-05-04 13:17:09.000000 nbdev-apl-0.0.753/nbdev_apl.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-04 13:17:09.000000 nbdev-apl-0.0.753/nbdev_apl.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-05-04 13:17:09.000000 nbdev-apl-0.0.753/nbdev_apl.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-04 13:17:09.000000 nbdev-apl-0.0.753/nbdev_apl.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-04 13:17:09.000000 nbdev-apl-0.0.753/nbdev_apl.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-04 13:17:09.000000 nbdev-apl-0.0.753/nbdev_apl.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      521 2023-05-04 13:17:09.000000 nbdev-apl-0.0.753/settings.ini
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-04 13:17:09.959384 nbdev-apl-0.0.753/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2746 2023-05-04 13:06:14.000000 nbdev-apl-0.0.753/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 01:41:37.040392 nbdev-apl-0.0.754/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-05 01:30:35.000000 nbdev-apl-0.0.754/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-05-05 01:30:35.000000 nbdev-apl-0.0.754/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      839 2023-05-05 01:41:37.040392 nbdev-apl-0.0.754/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      122 2023-05-05 01:30:35.000000 nbdev-apl-0.0.754/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 01:41:37.040392 nbdev-apl-0.0.754/nbdev_apl/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 01:41:36.000000 nbdev-apl-0.0.754/nbdev_apl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5828 2023-05-05 01:30:35.000000 nbdev-apl-0.0.754/nbdev_apl/_modidx.py
+-rw-r--r--   0 runner    (1001) docker     (123)      308 2023-05-05 01:41:36.000000 nbdev-apl-0.0.754/nbdev_apl/_nbdev.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 01:41:37.040392 nbdev-apl-0.0.754/nbdev_apl.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      839 2023-05-05 01:41:36.000000 nbdev-apl-0.0.754/nbdev_apl.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      346 2023-05-05 01:41:37.000000 nbdev-apl-0.0.754/nbdev_apl.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 01:41:36.000000 nbdev-apl-0.0.754/nbdev_apl.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-05-05 01:41:36.000000 nbdev-apl-0.0.754/nbdev_apl.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 01:41:36.000000 nbdev-apl-0.0.754/nbdev_apl.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-05 01:41:36.000000 nbdev-apl-0.0.754/nbdev_apl.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-05 01:41:36.000000 nbdev-apl-0.0.754/nbdev_apl.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      521 2023-05-05 01:41:36.000000 nbdev-apl-0.0.754/settings.ini
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-05 01:41:37.040392 nbdev-apl-0.0.754/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2746 2023-05-05 01:30:35.000000 nbdev-apl-0.0.754/setup.py
```

### Comparing `nbdev-apl-0.0.753/LICENSE` & `nbdev-apl-0.0.754/LICENSE`

 * *Files identical despite different names*

### Comparing `nbdev-apl-0.0.753/PKG-INFO` & `nbdev-apl-0.0.754/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nbdev-apl
-Version: 0.0.753
+Version: 0.0.754
 Summary: nbdev docs lookup for numpy
 Home-page: https://github.com/fastai/nbdev-index/tree/master/
 Author: Jeremy Howard
 Author-email: info@fast.ai
 License: Apache Software License 2.0
 Keywords: nbdev fastai python
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `nbdev-apl-0.0.753/nbdev_apl/_modidx.py` & `nbdev-apl-0.0.754/nbdev_apl/_modidx.py`

 * *Files identical despite different names*

### Comparing `nbdev-apl-0.0.753/nbdev_apl.egg-info/PKG-INFO` & `nbdev-apl-0.0.754/nbdev_apl.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nbdev-apl
-Version: 0.0.753
+Version: 0.0.754
 Summary: nbdev docs lookup for numpy
 Home-page: https://github.com/fastai/nbdev-index/tree/master/
 Author: Jeremy Howard
 Author-email: info@fast.ai
 License: Apache Software License 2.0
 Keywords: nbdev fastai python
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `nbdev-apl-0.0.753/setup.py` & `nbdev-apl-0.0.754/setup.py`

 * *Files identical despite different names*

