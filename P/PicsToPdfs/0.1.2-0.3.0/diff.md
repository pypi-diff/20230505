# Comparing `tmp/PicsToPdfs-0.1.2.tar.gz` & `tmp/PicsToPdfs-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PicsToPdfs-0.1.2.tar", last modified: Tue Feb 28 05:51:54 2023, max compression
+gzip compressed data, was "PicsToPdfs-0.3.0.tar", last modified: Fri May  5 12:21:18 2023, max compression
```

## Comparing `PicsToPdfs-0.1.2.tar` & `PicsToPdfs-0.3.0.tar`

### file list

```diff
@@ -1,21 +1,18 @@
-drwxrwxrwx   0        0        0        0 2023-02-28 05:51:54.404118 PicsToPdfs-0.1.2/
--rw-rw-rw-   0        0        0     1090 2022-12-21 02:47:10.000000 PicsToPdfs-0.1.2/LICENSE.txt
--rw-rw-rw-   0        0        0       89 2022-12-21 03:16:16.000000 PicsToPdfs-0.1.2/MANIFEST.in
--rw-rw-rw-   0        0        0      481 2023-02-28 05:51:54.405120 PicsToPdfs-0.1.2/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-02-28 05:51:54.364121 PicsToPdfs-0.1.2/PicsToPdfs/
-drwxrwxrwx   0        0        0        0 2023-02-28 05:51:54.391128 PicsToPdfs-0.1.2/PicsToPdfs/Function/
--rw-rw-rw-   0        0        0        0 2023-02-28 03:46:50.000000 PicsToPdfs-0.1.2/PicsToPdfs/Function/__init__.py
--rw-rw-rw-   0        0        0     4806 2022-11-14 08:45:55.000000 PicsToPdfs-0.1.2/PicsToPdfs/Function/imgToPdf.py
--rw-rw-rw-   0        0        0     9329 2023-02-28 05:50:26.000000 PicsToPdfs-0.1.2/PicsToPdfs/PicToPdf.py
-drwxrwxrwx   0        0        0        0 2023-02-28 05:51:54.400123 PicsToPdfs-0.1.2/PicsToPdfs/Ui/
--rw-rw-rw-   0        0        0     6632 2023-02-28 03:54:18.000000 PicsToPdfs-0.1.2/PicsToPdfs/Ui/PicToPdfUi.py
--rw-rw-rw-   0        0        0        0 2023-02-28 03:46:36.000000 PicsToPdfs-0.1.2/PicsToPdfs/Ui/__init__.py
--rw-rw-rw-   0        0        0        0 2023-02-28 03:39:56.000000 PicsToPdfs-0.1.2/PicsToPdfs/__init__.py
-drwxrwxrwx   0        0        0        0 2023-02-28 05:51:54.381120 PicsToPdfs-0.1.2/PicsToPdfs.egg-info/
--rw-rw-rw-   0        0        0      481 2023-02-28 05:51:54.000000 PicsToPdfs-0.1.2/PicsToPdfs.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      352 2023-02-28 05:51:54.000000 PicsToPdfs-0.1.2/PicsToPdfs.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-02-28 05:51:54.000000 PicsToPdfs-0.1.2/PicsToPdfs.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       11 2023-02-28 05:51:54.000000 PicsToPdfs-0.1.2/PicsToPdfs.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       33 2023-02-21 06:55:26.000000 PicsToPdfs-0.1.2/README.md
--rw-rw-rw-   0        0        0      135 2023-02-28 05:51:54.407120 PicsToPdfs-0.1.2/setup.cfg
--rw-rw-rw-   0        0        0     1028 2023-02-28 05:50:26.000000 PicsToPdfs-0.1.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-05 12:21:18.802842 PicsToPdfs-0.3.0/
+-rw-rw-rw-   0        0        0     1090 2022-12-21 02:47:10.000000 PicsToPdfs-0.3.0/LICENSE.txt
+-rw-rw-rw-   0        0        0       89 2022-12-21 03:16:16.000000 PicsToPdfs-0.3.0/MANIFEST.in
+-rw-rw-rw-   0        0        0      481 2023-05-05 12:21:18.802842 PicsToPdfs-0.3.0/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-05-05 12:21:18.791833 PicsToPdfs-0.3.0/PicsToPdfs/
+drwxrwxrwx   0        0        0        0 2023-05-05 12:21:18.799861 PicsToPdfs-0.3.0/PicsToPdfs/Function/
+-rw-rw-rw-   0        0        0        0 2023-02-28 05:54:02.000000 PicsToPdfs-0.3.0/PicsToPdfs/Function/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-05 12:21:18.800831 PicsToPdfs-0.3.0/PicsToPdfs/Ui/
+-rw-rw-rw-   0        0        0        0 2023-02-28 05:54:02.000000 PicsToPdfs-0.3.0/PicsToPdfs/Ui/__init__.py
+-rw-rw-rw-   0        0        0        0 2023-02-28 05:54:02.000000 PicsToPdfs-0.3.0/PicsToPdfs/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-05 12:21:18.797831 PicsToPdfs-0.3.0/PicsToPdfs.egg-info/
+-rw-rw-rw-   0        0        0      481 2023-05-05 12:21:18.000000 PicsToPdfs-0.3.0/PicsToPdfs.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      269 2023-05-05 12:21:18.000000 PicsToPdfs-0.3.0/PicsToPdfs.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-05 12:21:18.000000 PicsToPdfs-0.3.0/PicsToPdfs.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       11 2023-05-05 12:21:18.000000 PicsToPdfs-0.3.0/PicsToPdfs.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       33 2023-02-21 06:55:26.000000 PicsToPdfs-0.3.0/README.md
+-rw-rw-rw-   0        0        0      135 2023-05-05 12:21:18.803829 PicsToPdfs-0.3.0/setup.cfg
+-rw-rw-rw-   0        0        0     1028 2023-05-05 12:21:12.000000 PicsToPdfs-0.3.0/setup.py
```

### Comparing `PicsToPdfs-0.1.2/LICENSE.txt` & `PicsToPdfs-0.3.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `PicsToPdfs-0.1.2/setup.py` & `PicsToPdfs-0.3.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 #!/usr/bin/env python
 #-*- coding:utf-8 -*-
 import os 
 from setuptools import setup, find_packages
 
 MAJOR = 0
-MINOR = 1
-PATCH = 2
+MINOR = 3
+PATCH = 0
 VERSION = f"{MAJOR}.{MINOR}.{PATCH}"
 
 def get_install_requires():
     reqs = []
     return reqs
 setup(
 	name = "PicsToPdfs",
```

