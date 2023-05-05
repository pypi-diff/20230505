# Comparing `tmp/lincs-0.2.0.tar.gz` & `tmp/lincs-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lincs-0.2.0.tar", last modified: Fri May  5 13:57:19 2023, max compression
+gzip compressed data, was "lincs-0.2.1.tar", last modified: Fri May  5 14:06:38 2023, max compression
```

## Comparing `lincs-0.2.0.tar` & `lincs-0.2.1.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 user      (1002) user      (1002)        0 2023-05-05 13:57:19.840721 lincs-0.2.0/
--rw-r--r--   0 user      (1002) user      (1002)       58 2023-05-04 08:59:02.000000 lincs-0.2.0/MANIFEST.in
--rw-r--r--   0 user      (1002) user      (1002)    10332 2023-05-05 13:57:19.840721 lincs-0.2.0/PKG-INFO
--rw-r--r--   0 user      (1002) user      (1002)     9715 2023-05-05 13:53:52.000000 lincs-0.2.0/README.md
-drwxr-xr-x   0 user      (1002) user      (1002)        0 2023-05-05 13:57:19.840721 lincs-0.2.0/lincs/
--rw-rw-r--   0 user      (1002) user      (1002)      343 2023-05-05 13:09:35.000000 lincs-0.2.0/lincs/__init__.py
--rw-r--r--   0 user      (1002) user      (1002)      136 2023-05-04 08:59:02.000000 lincs-0.2.0/lincs/__main__.py
--rw-rw-r--   0 user      (1002) user      (1002)    18889 2023-05-05 13:44:47.000000 lincs-0.2.0/lincs/command_line_interface.py
-drwxr-xr-x   0 user      (1002) user      (1002)        0 2023-05-05 13:57:19.840721 lincs-0.2.0/lincs/liblincs/
--rw-rw-r--   0 user      (1002) user      (1002)     9114 2023-05-05 13:34:11.000000 lincs-0.2.0/lincs/liblincs/liblincs_module.cpp
--rw-rw-r--   0 user      (1002) user      (1002)    12319 2023-05-05 12:56:20.000000 lincs-0.2.0/lincs/liblincs/lincs.cpp
--rw-rw-r--   0 user      (1002) user      (1002)     4460 2023-05-05 13:32:55.000000 lincs-0.2.0/lincs/liblincs/lincs.hpp
--rw-rw-r--   0 user      (1002) user      (1002)      718 2023-05-05 13:51:37.000000 lincs-0.2.0/lincs/visualization.py
-drwxr-xr-x   0 user      (1002) user      (1002)        0 2023-05-05 13:57:19.840721 lincs-0.2.0/lincs.egg-info/
--rw-r--r--   0 user      (1002) user      (1002)    10332 2023-05-05 13:57:19.000000 lincs-0.2.0/lincs.egg-info/PKG-INFO
--rw-r--r--   0 user      (1002) user      (1002)      399 2023-05-05 13:57:19.000000 lincs-0.2.0/lincs.egg-info/SOURCES.txt
--rw-r--r--   0 user      (1002) user      (1002)        1 2023-05-05 13:57:19.000000 lincs-0.2.0/lincs.egg-info/dependency_links.txt
--rw-r--r--   0 user      (1002) user      (1002)       60 2023-05-05 13:57:19.000000 lincs-0.2.0/lincs.egg-info/entry_points.txt
--rw-r--r--   0 user      (1002) user      (1002)       27 2023-05-05 13:57:19.000000 lincs-0.2.0/lincs.egg-info/requires.txt
--rw-r--r--   0 user      (1002) user      (1002)       15 2023-05-05 13:57:19.000000 lincs-0.2.0/lincs.egg-info/top_level.txt
--rw-r--r--   0 user      (1002) user      (1002)       27 2023-05-05 13:01:57.000000 lincs-0.2.0/requirements.txt
--rw-r--r--   0 user      (1002) user      (1002)       38 2023-05-05 13:57:19.840721 lincs-0.2.0/setup.cfg
--rw-rw-r--   0 user      (1002) user      (1002)     1551 2023-05-05 13:55:12.000000 lincs-0.2.0/setup.py
+drwxr-xr-x   0 user      (1002) user      (1002)        0 2023-05-05 14:06:38.845341 lincs-0.2.1/
+-rw-r--r--   0 user      (1002) user      (1002)       58 2023-05-04 08:59:02.000000 lincs-0.2.1/MANIFEST.in
+-rw-r--r--   0 user      (1002) user      (1002)    10602 2023-05-05 14:06:38.845341 lincs-0.2.1/PKG-INFO
+-rw-r--r--   0 user      (1002) user      (1002)     9715 2023-05-05 13:53:52.000000 lincs-0.2.1/README.md
+drwxr-xr-x   0 user      (1002) user      (1002)        0 2023-05-05 14:06:38.845341 lincs-0.2.1/lincs/
+-rw-rw-r--   0 user      (1002) user      (1002)      343 2023-05-05 13:09:35.000000 lincs-0.2.1/lincs/__init__.py
+-rw-r--r--   0 user      (1002) user      (1002)      136 2023-05-04 08:59:02.000000 lincs-0.2.1/lincs/__main__.py
+-rw-rw-r--   0 user      (1002) user      (1002)    18889 2023-05-05 13:44:47.000000 lincs-0.2.1/lincs/command_line_interface.py
+drwxr-xr-x   0 user      (1002) user      (1002)        0 2023-05-05 14:06:38.845341 lincs-0.2.1/lincs/liblincs/
+-rw-rw-r--   0 user      (1002) user      (1002)     9114 2023-05-05 13:34:11.000000 lincs-0.2.1/lincs/liblincs/liblincs_module.cpp
+-rw-rw-r--   0 user      (1002) user      (1002)    12319 2023-05-05 12:56:20.000000 lincs-0.2.1/lincs/liblincs/lincs.cpp
+-rw-rw-r--   0 user      (1002) user      (1002)     4460 2023-05-05 13:32:55.000000 lincs-0.2.1/lincs/liblincs/lincs.hpp
+-rw-rw-r--   0 user      (1002) user      (1002)      718 2023-05-05 13:51:37.000000 lincs-0.2.1/lincs/visualization.py
+drwxr-xr-x   0 user      (1002) user      (1002)        0 2023-05-05 14:06:38.845341 lincs-0.2.1/lincs.egg-info/
+-rw-r--r--   0 user      (1002) user      (1002)    10602 2023-05-05 14:06:38.000000 lincs-0.2.1/lincs.egg-info/PKG-INFO
+-rw-r--r--   0 user      (1002) user      (1002)      399 2023-05-05 14:06:38.000000 lincs-0.2.1/lincs.egg-info/SOURCES.txt
+-rw-r--r--   0 user      (1002) user      (1002)        1 2023-05-05 14:06:38.000000 lincs-0.2.1/lincs.egg-info/dependency_links.txt
+-rw-r--r--   0 user      (1002) user      (1002)       60 2023-05-05 14:06:38.000000 lincs-0.2.1/lincs.egg-info/entry_points.txt
+-rw-r--r--   0 user      (1002) user      (1002)       27 2023-05-05 14:06:38.000000 lincs-0.2.1/lincs.egg-info/requires.txt
+-rw-r--r--   0 user      (1002) user      (1002)       15 2023-05-05 14:06:38.000000 lincs-0.2.1/lincs.egg-info/top_level.txt
+-rw-r--r--   0 user      (1002) user      (1002)       27 2023-05-05 13:01:57.000000 lincs-0.2.1/requirements.txt
+-rw-r--r--   0 user      (1002) user      (1002)       38 2023-05-05 14:06:38.845341 lincs-0.2.1/setup.cfg
+-rw-rw-r--   0 user      (1002) user      (1002)     1720 2023-05-05 14:06:10.000000 lincs-0.2.1/setup.py
```

### Comparing `lincs-0.2.0/PKG-INFO` & `lincs-0.2.1/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,24 +1,7 @@
-Metadata-Version: 2.1
-Name: lincs
-Version: 0.2.0
-Summary: MCDA algorithms
-Home-page: https://github.com/jacquev6/lincs
-Author: Vincent Jacques
-Author-email: vincent@vincent-jacques.net
-Classifier: Development Status :: 2 - Pre-Alpha
-Classifier: Environment :: Console
-Classifier: Intended Audience :: Developers
-Classifier: Intended Audience :: Science/Research
-Classifier: Operating System :: POSIX :: Linux
-Classifier: Programming Language :: C++
-Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
-Description-Content-Type: text/markdown
-
 *lincs* is a collection of MCDA algorithms, usable as a C++ library, a Python package and a command-line utility.
 
 Note that *lincs* is not licensed yet, so you don't have any rights besides reading it for now.
 
 # Get started
 
 ## Install
```

### Comparing `lincs-0.2.0/README.md` & `lincs-0.2.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,24 @@
+Metadata-Version: 2.1
+Name: lincs
+Version: 0.2.1
+Summary: MCDA algorithms
+Home-page: https://github.com/jacquev6/lincs
+Author: Vincent Jacques
+Author-email: vincent@vincent-jacques.net
+Classifier: Development Status :: 2 - Pre-Alpha
+Classifier: Environment :: Console
+Classifier: Intended Audience :: Developers
+Classifier: Intended Audience :: Science/Research
+Classifier: Operating System :: POSIX :: Linux
+Classifier: Programming Language :: C++
+Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
+Description-Content-Type: text/markdown
+
 *lincs* is a collection of MCDA algorithms, usable as a C++ library, a Python package and a command-line utility.
 
 Note that *lincs* is not licensed yet, so you don't have any rights besides reading it for now.
 
 # Get started
 
 ## Install
@@ -143,23 +160,23 @@
 <!-- EXTEND command-line-example/run.sh --><!--
     diff expected-model.yml model.yml
 --><!-- STOP -->
 
 You can visualize it using:
 
 <!-- EXTEND command-line-example/run.sh -->
-    lincs visualize model domain.yml model.yml model.png
+    lincs visualize model domain.yml model.yml https://github.com/jacquev6/lincs/raw/v0.2.1/model.png
 <!-- STOP -->
 <!-- EXTEND command-line-example/run.sh --><!--
-    cp model.png ../../..
+    cp https://github.com/jacquev6/lincs/raw/v0.2.1/model.png ../../..
 --><!-- STOP -->
 
 It should output something like:
 
-![Model visualization](model.png)
+![Model visualization](https://github.com/jacquev6/lincs/raw/v0.2.1/model.png)
 
 And finally generate a set of classified alternatives (@todo Link to concepts and file formats):
 
 <!-- EXTEND command-line-example/run.sh -->
     lincs generate classified-alternatives domain.yml model.yml 10 --output-classified-alternatives learning-set.csv
 <!-- APPEND-TO-LAST-LINE --random-seed 42 -->
 <!-- STOP -->
@@ -183,23 +200,23 @@
 <!-- EXTEND command-line-example/run.sh --><!--
     diff expected-learning-set.csv learning-set.csv
 --><!-- STOP -->
 
 You can visualize it using:
 
 <!-- EXTEND command-line-example/run.sh -->
-    lincs visualize model domain.yml model.yml --alternatives learning-set.csv alternatives.png
+    lincs visualize model domain.yml model.yml --alternatives learning-set.csv https://github.com/jacquev6/lincs/raw/v0.2.1/alternatives.png
 <!-- STOP -->
 <!-- EXTEND command-line-example/run.sh --><!--
-    cp alternatives.png ../../..
+    cp https://github.com/jacquev6/lincs/raw/v0.2.1/alternatives.png ../../..
 --><!-- STOP -->
 
 It should output something like:
 
-![Alternatives visualization](alternatives.png)
+![Alternatives visualization](https://github.com/jacquev6/lincs/raw/v0.2.1/alternatives.png)
 
 @todo Improve how this graph looks:
 
 - display categories as stacked solid colors
 - display alternatives in a color that matches their assigned category
 - remove the legend, place names (categories and alternatives) directly on the graph
```

### Comparing `lincs-0.2.0/lincs/command_line_interface.py` & `lincs-0.2.1/lincs/command_line_interface.py`

 * *Files identical despite different names*

### Comparing `lincs-0.2.0/lincs/liblincs/liblincs_module.cpp` & `lincs-0.2.1/lincs/liblincs/liblincs_module.cpp`

 * *Files identical despite different names*

### Comparing `lincs-0.2.0/lincs/liblincs/lincs.cpp` & `lincs-0.2.1/lincs/liblincs/lincs.cpp`

 * *Files identical despite different names*

### Comparing `lincs-0.2.0/lincs/liblincs/lincs.hpp` & `lincs-0.2.1/lincs/liblincs/lincs.hpp`

 * *Files identical despite different names*

### Comparing `lincs-0.2.0/lincs/visualization.py` & `lincs-0.2.1/lincs/visualization.py`

 * *Files identical despite different names*

### Comparing `lincs-0.2.0/lincs.egg-info/PKG-INFO` & `lincs-0.2.1/lincs.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lincs
-Version: 0.2.0
+Version: 0.2.1
 Summary: MCDA algorithms
 Home-page: https://github.com/jacquev6/lincs
 Author: Vincent Jacques
 Author-email: vincent@vincent-jacques.net
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
@@ -160,23 +160,23 @@
 <!-- EXTEND command-line-example/run.sh --><!--
     diff expected-model.yml model.yml
 --><!-- STOP -->
 
 You can visualize it using:
 
 <!-- EXTEND command-line-example/run.sh -->
-    lincs visualize model domain.yml model.yml model.png
+    lincs visualize model domain.yml model.yml https://github.com/jacquev6/lincs/raw/v0.2.1/model.png
 <!-- STOP -->
 <!-- EXTEND command-line-example/run.sh --><!--
-    cp model.png ../../..
+    cp https://github.com/jacquev6/lincs/raw/v0.2.1/model.png ../../..
 --><!-- STOP -->
 
 It should output something like:
 
-![Model visualization](model.png)
+![Model visualization](https://github.com/jacquev6/lincs/raw/v0.2.1/model.png)
 
 And finally generate a set of classified alternatives (@todo Link to concepts and file formats):
 
 <!-- EXTEND command-line-example/run.sh -->
     lincs generate classified-alternatives domain.yml model.yml 10 --output-classified-alternatives learning-set.csv
 <!-- APPEND-TO-LAST-LINE --random-seed 42 -->
 <!-- STOP -->
@@ -200,23 +200,23 @@
 <!-- EXTEND command-line-example/run.sh --><!--
     diff expected-learning-set.csv learning-set.csv
 --><!-- STOP -->
 
 You can visualize it using:
 
 <!-- EXTEND command-line-example/run.sh -->
-    lincs visualize model domain.yml model.yml --alternatives learning-set.csv alternatives.png
+    lincs visualize model domain.yml model.yml --alternatives learning-set.csv https://github.com/jacquev6/lincs/raw/v0.2.1/alternatives.png
 <!-- STOP -->
 <!-- EXTEND command-line-example/run.sh --><!--
-    cp alternatives.png ../../..
+    cp https://github.com/jacquev6/lincs/raw/v0.2.1/alternatives.png ../../..
 --><!-- STOP -->
 
 It should output something like:
 
-![Alternatives visualization](alternatives.png)
+![Alternatives visualization](https://github.com/jacquev6/lincs/raw/v0.2.1/alternatives.png)
 
 @todo Improve how this graph looks:
 
 - display categories as stacked solid colors
 - display alternatives in a color that matches their assigned category
 - remove the legend, place names (categories and alternatives) directly on the graph
```

### Comparing `lincs-0.2.0/setup.py` & `lincs-0.2.1/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 import setuptools
 
 
-version = "0.2.0"
+version = "0.2.1"
 
 with open("README.md") as f:
     long_description = f.read()
+for image in ["model", "alternatives"]:
+    long_description = long_description.replace(f"{image}.png", f"https://github.com/jacquev6/lincs/raw/v{version}/{image}.png")
 
 with open("requirements.txt") as f:
     install_requires = f.readlines()
 
 
 liblincs = setuptools.Extension(
     "liblincs",
```

