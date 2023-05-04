# Comparing `tmp/fastpathplanning-0.1.1.tar.gz` & `tmp/fastpathplanning-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fastpathplanning-0.1.1.tar", last modified: Tue Apr 18 15:56:33 2023, max compression
+gzip compressed data, was "fastpathplanning-0.1.2.tar", last modified: Thu May  4 22:03:27 2023, max compression
```

## Comparing `fastpathplanning-0.1.1.tar` & `fastpathplanning-0.1.2.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-18 15:56:33.382723 fastpathplanning-0.1.1/
--rw-r--r--   0 root         (0) root         (0)    11357 2023-04-18 15:56:28.000000 fastpathplanning-0.1.1/LICENSE
--rw-r--r--   0 root         (0) root         (0)      744 2023-04-18 15:56:33.382723 fastpathplanning-0.1.1/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      425 2023-04-18 15:56:28.000000 fastpathplanning-0.1.1/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-18 15:56:33.382723 fastpathplanning-0.1.1/fastpathplanning/
--rw-r--r--   0 root         (0) root         (0)       60 2023-04-18 15:56:28.000000 fastpathplanning-0.1.1/fastpathplanning/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6176 2023-04-18 15:56:28.000000 fastpathplanning-0.1.1/fastpathplanning/boxes.py
--rw-r--r--   0 root         (0) root         (0)     1523 2023-04-18 15:56:28.000000 fastpathplanning-0.1.1/fastpathplanning/fastpathplanning.py
--rw-r--r--   0 root         (0) root         (0)     5483 2023-04-18 15:56:28.000000 fastpathplanning-0.1.1/fastpathplanning/graph.py
--rw-r--r--   0 root         (0) root         (0)     5361 2023-04-18 15:56:28.000000 fastpathplanning-0.1.1/fastpathplanning/polygonal.py
--rw-r--r--   0 root         (0) root         (0)    10920 2023-04-18 15:56:28.000000 fastpathplanning-0.1.1/fastpathplanning/smooth.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-18 15:56:33.382723 fastpathplanning-0.1.1/fastpathplanning.egg-info/
--rw-r--r--   0 root         (0) root         (0)      744 2023-04-18 15:56:33.000000 fastpathplanning-0.1.1/fastpathplanning.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      415 2023-04-18 15:56:33.000000 fastpathplanning-0.1.1/fastpathplanning.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-18 15:56:33.000000 fastpathplanning-0.1.1/fastpathplanning.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       35 2023-04-18 15:56:33.000000 fastpathplanning-0.1.1/fastpathplanning.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       17 2023-04-18 15:56:33.000000 fastpathplanning-0.1.1/fastpathplanning.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       97 2023-04-18 15:56:28.000000 fastpathplanning-0.1.1/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-04-18 15:56:33.382723 fastpathplanning-0.1.1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1294 2023-04-18 15:56:28.000000 fastpathplanning-0.1.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 22:03:27.514768 fastpathplanning-0.1.2/
+-rw-r--r--   0 root         (0) root         (0)    11357 2023-05-04 22:03:22.000000 fastpathplanning-0.1.2/LICENSE
+-rw-r--r--   0 root         (0) root         (0)      744 2023-05-04 22:03:27.514768 fastpathplanning-0.1.2/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      425 2023-05-04 22:03:22.000000 fastpathplanning-0.1.2/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 22:03:27.514768 fastpathplanning-0.1.2/fastpathplanning/
+-rw-r--r--   0 root         (0) root         (0)       60 2023-05-04 22:03:22.000000 fastpathplanning-0.1.2/fastpathplanning/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6176 2023-05-04 22:03:22.000000 fastpathplanning-0.1.2/fastpathplanning/boxes.py
+-rw-r--r--   0 root         (0) root         (0)     1523 2023-05-04 22:03:22.000000 fastpathplanning-0.1.2/fastpathplanning/fastpathplanning.py
+-rw-r--r--   0 root         (0) root         (0)     5483 2023-05-04 22:03:22.000000 fastpathplanning-0.1.2/fastpathplanning/graph.py
+-rw-r--r--   0 root         (0) root         (0)     5361 2023-05-04 22:03:22.000000 fastpathplanning-0.1.2/fastpathplanning/polygonal.py
+-rw-r--r--   0 root         (0) root         (0)    10920 2023-05-04 22:03:22.000000 fastpathplanning-0.1.2/fastpathplanning/smooth.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 22:03:27.514768 fastpathplanning-0.1.2/fastpathplanning.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      744 2023-05-04 22:03:27.000000 fastpathplanning-0.1.2/fastpathplanning.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      415 2023-05-04 22:03:27.000000 fastpathplanning-0.1.2/fastpathplanning.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-04 22:03:27.000000 fastpathplanning-0.1.2/fastpathplanning.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       35 2023-05-04 22:03:27.000000 fastpathplanning-0.1.2/fastpathplanning.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       17 2023-05-04 22:03:27.000000 fastpathplanning-0.1.2/fastpathplanning.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       97 2023-05-04 22:03:22.000000 fastpathplanning-0.1.2/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-05-04 22:03:27.514768 fastpathplanning-0.1.2/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1294 2023-05-04 22:03:22.000000 fastpathplanning-0.1.2/setup.py
```

### Comparing `fastpathplanning-0.1.1/LICENSE` & `fastpathplanning-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `fastpathplanning-0.1.1/PKG-INFO` & `fastpathplanning-0.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fastpathplanning
-Version: 0.1.1
+Version: 0.1.2
 Summary: An algorithm for path planning in sequences of safe boxes
 Home-page: https://github.com/cvxgrp/fpp.py
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `fastpathplanning-0.1.1/fastpathplanning/boxes.py` & `fastpathplanning-0.1.2/fastpathplanning/boxes.py`

 * *Files identical despite different names*

### Comparing `fastpathplanning-0.1.1/fastpathplanning/fastpathplanning.py` & `fastpathplanning-0.1.2/fastpathplanning/fastpathplanning.py`

 * *Files identical despite different names*

### Comparing `fastpathplanning-0.1.1/fastpathplanning/graph.py` & `fastpathplanning-0.1.2/fastpathplanning/graph.py`

 * *Files identical despite different names*

### Comparing `fastpathplanning-0.1.1/fastpathplanning/polygonal.py` & `fastpathplanning-0.1.2/fastpathplanning/polygonal.py`

 * *Files identical despite different names*

### Comparing `fastpathplanning-0.1.1/fastpathplanning/smooth.py` & `fastpathplanning-0.1.2/fastpathplanning/smooth.py`

 * *Files identical despite different names*

### Comparing `fastpathplanning-0.1.1/fastpathplanning.egg-info/PKG-INFO` & `fastpathplanning-0.1.2/fastpathplanning.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fastpathplanning
-Version: 0.1.1
+Version: 0.1.2
 Summary: An algorithm for path planning in sequences of safe boxes
 Home-page: https://github.com/cvxgrp/fpp.py
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `fastpathplanning-0.1.1/setup.py` & `fastpathplanning-0.1.2/setup.py`

 * *Files identical despite different names*

