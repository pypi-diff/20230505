# Comparing `tmp/idelucs-0.1.6.tar.gz` & `tmp/idelucs-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "idelucs-0.1.6.tar", last modified: Thu May  4 21:29:25 2023, max compression
+gzip compressed data, was "idelucs-0.1.7.tar", last modified: Thu May  4 21:57:49 2023, max compression
```

## Comparing `idelucs-0.1.6.tar` & `idelucs-0.1.7.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxrwx   0        0        0        0 2023-05-04 21:29:25.196763 idelucs-0.1.6/
--rw-rw-rw-   0        0        0     1074 2023-05-04 00:59:28.000000 idelucs-0.1.6/LICENCE.md
--rw-rw-rw-   0        0        0      261 2023-05-04 21:29:25.195760 idelucs-0.1.6/PKG-INFO
--rw-rw-rw-   0        0        0     5274 2023-05-04 00:59:28.000000 idelucs-0.1.6/README.md
-drwxrwxrwx   0        0        0        0 2023-05-04 21:29:25.131763 idelucs-0.1.6/idelucs/
--rw-rw-rw-   0        0        0     3104 2023-05-04 00:59:31.000000 idelucs-0.1.6/idelucs/LossFunctions.py
--rw-rw-rw-   0        0        0     2584 2023-05-04 00:59:31.000000 idelucs-0.1.6/idelucs/PytorchUtils.py
--rw-rw-rw-   0        0        0     7524 2023-05-04 00:59:31.000000 idelucs-0.1.6/idelucs/ResNet.py
--rw-rw-rw-   0        0        0      488 2023-05-04 21:26:18.000000 idelucs-0.1.6/idelucs/__init__.py
--rw-rw-rw-   0        0        0    11548 2023-05-04 00:59:31.000000 idelucs-0.1.6/idelucs/__main__.py
--rw-rw-rw-   0        0        0     6108 2023-05-04 00:59:31.000000 idelucs-0.1.6/idelucs/kmers.pyx
--rw-rw-rw-   0        0        0     6731 2023-05-04 00:59:31.000000 idelucs-0.1.6/idelucs/models.py
--rw-rw-rw-   0        0        0    20750 2023-05-04 21:25:35.000000 idelucs-0.1.6/idelucs/utils.py
--rw-rw-rw-   0        0        0     2949 2023-05-04 00:59:31.000000 idelucs-0.1.6/idelucs/utils_GUI.py
-drwxrwxrwx   0        0        0        0 2023-05-04 21:29:25.193762 idelucs-0.1.6/idelucs.egg-info/
--rw-rw-rw-   0        0        0      261 2023-05-04 21:29:24.000000 idelucs-0.1.6/idelucs.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      413 2023-05-04 21:29:24.000000 idelucs-0.1.6/idelucs.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-04 21:29:24.000000 idelucs-0.1.6/idelucs.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       50 2023-05-04 21:29:24.000000 idelucs-0.1.6/idelucs.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      152 2023-05-04 21:29:24.000000 idelucs-0.1.6/idelucs.egg-info/requires.txt
--rw-rw-rw-   0        0        0       15 2023-05-04 21:29:24.000000 idelucs-0.1.6/idelucs.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1166 2023-05-04 13:39:52.000000 idelucs-0.1.6/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-04 21:29:25.196763 idelucs-0.1.6/setup.cfg
--rw-rw-rw-   0        0        0      419 2023-05-04 14:10:49.000000 idelucs-0.1.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-04 21:57:49.799095 idelucs-0.1.7/
+-rw-rw-rw-   0        0        0     1074 2023-05-04 00:59:28.000000 idelucs-0.1.7/LICENCE.md
+-rw-rw-rw-   0        0        0      261 2023-05-04 21:57:49.788094 idelucs-0.1.7/PKG-INFO
+-rw-rw-rw-   0        0        0     5274 2023-05-04 00:59:28.000000 idelucs-0.1.7/README.md
+drwxrwxrwx   0        0        0        0 2023-05-04 21:57:49.737100 idelucs-0.1.7/idelucs/
+-rw-rw-rw-   0        0        0     3104 2023-05-04 00:59:31.000000 idelucs-0.1.7/idelucs/LossFunctions.py
+-rw-rw-rw-   0        0        0     2584 2023-05-04 00:59:31.000000 idelucs-0.1.7/idelucs/PytorchUtils.py
+-rw-rw-rw-   0        0        0     7524 2023-05-04 00:59:31.000000 idelucs-0.1.7/idelucs/ResNet.py
+-rw-rw-rw-   0        0        0      488 2023-05-04 21:55:05.000000 idelucs-0.1.7/idelucs/__init__.py
+-rw-rw-rw-   0        0        0    11548 2023-05-04 00:59:31.000000 idelucs-0.1.7/idelucs/__main__.py
+-rw-rw-rw-   0        0        0     6108 2023-05-04 00:59:31.000000 idelucs-0.1.7/idelucs/kmers.pyx
+-rw-rw-rw-   0        0        0     6731 2023-05-04 00:59:31.000000 idelucs-0.1.7/idelucs/models.py
+-rw-rw-rw-   0        0        0    20761 2023-05-04 21:54:43.000000 idelucs-0.1.7/idelucs/utils.py
+-rw-rw-rw-   0        0        0     2949 2023-05-04 00:59:31.000000 idelucs-0.1.7/idelucs/utils_GUI.py
+drwxrwxrwx   0        0        0        0 2023-05-04 21:57:49.785095 idelucs-0.1.7/idelucs.egg-info/
+-rw-rw-rw-   0        0        0      261 2023-05-04 21:57:49.000000 idelucs-0.1.7/idelucs.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      413 2023-05-04 21:57:49.000000 idelucs-0.1.7/idelucs.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-04 21:57:49.000000 idelucs-0.1.7/idelucs.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       50 2023-05-04 21:57:49.000000 idelucs-0.1.7/idelucs.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      152 2023-05-04 21:57:49.000000 idelucs-0.1.7/idelucs.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       15 2023-05-04 21:57:49.000000 idelucs-0.1.7/idelucs.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1166 2023-05-04 13:39:52.000000 idelucs-0.1.7/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-04 21:57:49.799095 idelucs-0.1.7/setup.cfg
+-rw-rw-rw-   0        0        0      419 2023-05-04 14:10:49.000000 idelucs-0.1.7/setup.py
```

### Comparing `idelucs-0.1.6/LICENCE.md` & `idelucs-0.1.7/LICENCE.md`

 * *Files identical despite different names*

### Comparing `idelucs-0.1.6/README.md` & `idelucs-0.1.7/README.md`

 * *Files identical despite different names*

### Comparing `idelucs-0.1.6/idelucs/LossFunctions.py` & `idelucs-0.1.7/idelucs/LossFunctions.py`

 * *Files identical despite different names*

### Comparing `idelucs-0.1.6/idelucs/PytorchUtils.py` & `idelucs-0.1.7/idelucs/PytorchUtils.py`

 * *Files identical despite different names*

### Comparing `idelucs-0.1.6/idelucs/ResNet.py` & `idelucs-0.1.7/idelucs/ResNet.py`

 * *Files identical despite different names*

### Comparing `idelucs-0.1.6/idelucs/__main__.py` & `idelucs-0.1.7/idelucs/__main__.py`

 * *Files identical despite different names*

### Comparing `idelucs-0.1.6/idelucs/kmers.pyx` & `idelucs-0.1.7/idelucs/kmers.pyx`

 * *Files identical despite different names*

### Comparing `idelucs-0.1.6/idelucs/models.py` & `idelucs-0.1.7/idelucs/models.py`

 * *Files identical despite different names*

### Comparing `idelucs-0.1.6/idelucs/utils.py` & `idelucs-0.1.7/idelucs/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import os 
 import sys
 import pyximport 
 pyximport.install()
 
 from .kmers import kmer_counts, cgr
 
 import random, itertools
```

### Comparing `idelucs-0.1.6/idelucs/utils_GUI.py` & `idelucs-0.1.7/idelucs/utils_GUI.py`

 * *Files identical despite different names*

### Comparing `idelucs-0.1.6/pyproject.toml` & `idelucs-0.1.7/pyproject.toml`

 * *Files identical despite different names*

