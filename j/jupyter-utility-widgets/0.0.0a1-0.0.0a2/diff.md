# Comparing `tmp/jupyter-utility-widgets-0.0.0a1.tar.gz` & `tmp/jupyter-utility-widgets-0.0.0a2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jupyter-utility-widgets-0.0.0a1.tar", last modified: Thu Dec  1 19:52:18 2022, max compression
+gzip compressed data, was "jupyter-utility-widgets-0.0.0a2.tar", last modified: Fri May  5 16:07:38 2023, max compression
```

## Comparing `jupyter-utility-widgets-0.0.0a1.tar` & `jupyter-utility-widgets-0.0.0a2.tar`

### file list

```diff
@@ -1,17 +1,18 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-01 19:52:18.311721 jupyter-utility-widgets-0.0.0a1/
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2022-12-01 19:52:03.000000 jupyter-utility-widgets-0.0.0a1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      530 2022-12-01 19:52:18.311721 jupyter-utility-widgets-0.0.0a1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      398 2022-12-01 19:52:03.000000 jupyter-utility-widgets-0.0.0a1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-01 19:52:18.311721 jupyter-utility-widgets-0.0.0a1/jupyter_utility_widgets/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-01 19:52:03.000000 jupyter-utility-widgets-0.0.0a1/jupyter_utility_widgets/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-01 19:52:18.311721 jupyter-utility-widgets-0.0.0a1/jupyter_utility_widgets/selector/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2022-12-01 19:52:03.000000 jupyter-utility-widgets-0.0.0a1/jupyter_utility_widgets/selector/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1389 2022-12-01 19:52:03.000000 jupyter-utility-widgets-0.0.0a1/jupyter_utility_widgets/selector/index_selector.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-01 19:52:18.311721 jupyter-utility-widgets-0.0.0a1/jupyter_utility_widgets.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      530 2022-12-01 19:52:18.000000 jupyter-utility-widgets-0.0.0a1/jupyter_utility_widgets.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      398 2022-12-01 19:52:18.000000 jupyter-utility-widgets-0.0.0a1/jupyter_utility_widgets.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-01 19:52:18.000000 jupyter-utility-widgets-0.0.0a1/jupyter_utility_widgets.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2022-12-01 19:52:18.000000 jupyter-utility-widgets-0.0.0a1/jupyter_utility_widgets.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       24 2022-12-01 19:52:18.000000 jupyter-utility-widgets-0.0.0a1/jupyter_utility_widgets.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      208 2022-12-01 19:52:03.000000 jupyter-utility-widgets-0.0.0a1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2022-12-01 19:52:18.311721 jupyter-utility-widgets-0.0.0a1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 16:07:38.228983 jupyter-utility-widgets-0.0.0a2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-05-05 16:07:27.000000 jupyter-utility-widgets-0.0.0a2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      520 2023-05-05 16:07:38.224983 jupyter-utility-widgets-0.0.0a2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      388 2023-05-05 16:07:27.000000 jupyter-utility-widgets-0.0.0a2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 16:07:38.224983 jupyter-utility-widgets-0.0.0a2/jupyter_utility_widgets/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 16:07:27.000000 jupyter-utility-widgets-0.0.0a2/jupyter_utility_widgets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1025 2023-05-05 16:07:27.000000 jupyter-utility-widgets-0.0.0a2/jupyter_utility_widgets/file_explorer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 16:07:38.224983 jupyter-utility-widgets-0.0.0a2/jupyter_utility_widgets/selector/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 16:07:27.000000 jupyter-utility-widgets-0.0.0a2/jupyter_utility_widgets/selector/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1389 2023-05-05 16:07:27.000000 jupyter-utility-widgets-0.0.0a2/jupyter_utility_widgets/selector/index_selector.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 16:07:38.224983 jupyter-utility-widgets-0.0.0a2/jupyter_utility_widgets.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      520 2023-05-05 16:07:38.000000 jupyter-utility-widgets-0.0.0a2/jupyter_utility_widgets.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      439 2023-05-05 16:07:38.000000 jupyter-utility-widgets-0.0.0a2/jupyter_utility_widgets.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 16:07:38.000000 jupyter-utility-widgets-0.0.0a2/jupyter_utility_widgets.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-05 16:07:38.000000 jupyter-utility-widgets-0.0.0a2/jupyter_utility_widgets.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-05-05 16:07:38.000000 jupyter-utility-widgets-0.0.0a2/jupyter_utility_widgets.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      208 2023-05-05 16:07:27.000000 jupyter-utility-widgets-0.0.0a2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-05 16:07:38.228983 jupyter-utility-widgets-0.0.0a2/setup.cfg
```

### Comparing `jupyter-utility-widgets-0.0.0a1/LICENSE` & `jupyter-utility-widgets-0.0.0a2/LICENSE`

 * *Files identical despite different names*

### Comparing `jupyter-utility-widgets-0.0.0a1/PKG-INFO` & `jupyter-utility-widgets-0.0.0a2/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 Metadata-Version: 2.1
 Name: jupyter-utility-widgets
-Version: 0.0.0a1
+Version: 0.0.0a2
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# jupyter-utility-widgets
+# python-utility
 
-Seeing I have been using a few widgets "patterns" over and over, I have decided to share and package them in a convenient project.
+Seeing I have been using a few widgets "patterns" over and over, I have decided to share and pack them in a convenient manner.
 
 ## Installation
 
 `pip install jupyter-utility-widgets`
 
 may require jupyterlab installation.
 
 ## Widgets
 
 1. Index Selector
-    A simple combination of widgets that help exploring a list of options.
+    A simple combination of widgets that help exploring a list of options.  
     see `examples/index_selector.ipynb`
+
```

### Comparing `jupyter-utility-widgets-0.0.0a1/jupyter_utility_widgets/selector/index_selector.py` & `jupyter-utility-widgets-0.0.0a2/jupyter_utility_widgets/selector/index_selector.py`

 * *Files identical despite different names*

### Comparing `jupyter-utility-widgets-0.0.0a1/jupyter_utility_widgets.egg-info/PKG-INFO` & `jupyter-utility-widgets-0.0.0a2/jupyter_utility_widgets.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 Metadata-Version: 2.1
 Name: jupyter-utility-widgets
-Version: 0.0.0a1
+Version: 0.0.0a2
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-# jupyter-utility-widgets
+# python-utility
 
-Seeing I have been using a few widgets "patterns" over and over, I have decided to share and package them in a convenient project.
+Seeing I have been using a few widgets "patterns" over and over, I have decided to share and pack them in a convenient manner.
 
 ## Installation
 
 `pip install jupyter-utility-widgets`
 
 may require jupyterlab installation.
 
 ## Widgets
 
 1. Index Selector
-    A simple combination of widgets that help exploring a list of options.
+    A simple combination of widgets that help exploring a list of options.  
     see `examples/index_selector.ipynb`
+
```

