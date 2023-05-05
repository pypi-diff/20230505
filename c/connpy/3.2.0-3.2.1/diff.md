# Comparing `tmp/connpy-3.2.0.tar.gz` & `tmp/connpy-3.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "connpy-3.2.0.tar", last modified: Fri May  5 16:42:49 2023, max compression
+gzip compressed data, was "connpy-3.2.1.tar", last modified: Fri May  5 17:20:30 2023, max compression
```

## Comparing `connpy-3.2.0.tar` & `connpy-3.2.1.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 16:42:49.592495 connpy-3.2.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-05-05 16:42:37.000000 connpy-3.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     9276 2023-05-05 16:42:49.592495 connpy-3.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8445 2023-05-05 16:42:37.000000 connpy-3.2.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 16:42:49.592495 connpy-3.2.0/connpy/
--rw-r--r--   0 runner    (1001) docker     (123)     8379 2023-05-05 16:42:37.000000 connpy-3.2.0/connpy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      181 2023-05-05 16:42:37.000000 connpy-3.2.0/connpy/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-05 16:42:37.000000 connpy-3.2.0/connpy/_version.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    14771 2023-05-05 16:42:37.000000 connpy-3.2.0/connpy/ai.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4713 2023-05-05 16:42:37.000000 connpy-3.2.0/connpy/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     3566 2023-05-05 16:42:37.000000 connpy-3.2.0/connpy/completion.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    15540 2023-05-05 16:42:37.000000 connpy-3.2.0/connpy/configfile.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    50300 2023-05-05 16:42:37.000000 connpy-3.2.0/connpy/connapp.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    28719 2023-05-05 16:42:37.000000 connpy-3.2.0/connpy/core.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 16:42:49.592495 connpy-3.2.0/connpy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     9276 2023-05-05 16:42:49.000000 connpy-3.2.0/connpy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      377 2023-05-05 16:42:49.000000 connpy-3.2.0/connpy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 16:42:49.000000 connpy-3.2.0/connpy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      126 2023-05-05 16:42:49.000000 connpy-3.2.0/connpy.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-05-05 16:42:49.000000 connpy-3.2.0/connpy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-05 16:42:49.000000 connpy-3.2.0/connpy.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1167 2023-05-05 16:42:49.592495 connpy-3.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-05-05 16:42:37.000000 connpy-3.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 17:20:30.069119 connpy-3.2.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-05-05 17:20:16.000000 connpy-3.2.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     9276 2023-05-05 17:20:30.069119 connpy-3.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8445 2023-05-05 17:20:16.000000 connpy-3.2.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 17:20:30.069119 connpy-3.2.1/connpy/
+-rw-r--r--   0 runner    (1001) docker     (123)     8379 2023-05-05 17:20:16.000000 connpy-3.2.1/connpy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      181 2023-05-05 17:20:16.000000 connpy-3.2.1/connpy/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-05 17:20:16.000000 connpy-3.2.1/connpy/_version.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    14755 2023-05-05 17:20:16.000000 connpy-3.2.1/connpy/ai.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4713 2023-05-05 17:20:16.000000 connpy-3.2.1/connpy/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3566 2023-05-05 17:20:16.000000 connpy-3.2.1/connpy/completion.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    15540 2023-05-05 17:20:16.000000 connpy-3.2.1/connpy/configfile.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    50300 2023-05-05 17:20:16.000000 connpy-3.2.1/connpy/connapp.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    28719 2023-05-05 17:20:16.000000 connpy-3.2.1/connpy/core.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 17:20:30.069119 connpy-3.2.1/connpy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     9276 2023-05-05 17:20:30.000000 connpy-3.2.1/connpy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      377 2023-05-05 17:20:30.000000 connpy-3.2.1/connpy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 17:20:30.000000 connpy-3.2.1/connpy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-05-05 17:20:30.000000 connpy-3.2.1/connpy.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       80 2023-05-05 17:20:30.000000 connpy-3.2.1/connpy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-05 17:20:30.000000 connpy-3.2.1/connpy.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1157 2023-05-05 17:20:30.069119 connpy-3.2.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-05-05 17:20:16.000000 connpy-3.2.1/setup.py
```

### Comparing `connpy-3.2.0/LICENSE` & `connpy-3.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `connpy-3.2.0/PKG-INFO` & `connpy-3.2.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: connpy
-Version: 3.2.0
+Version: 3.2.1
 Summary: Connpy is a SSH/Telnet connection manager and automation module
 Home-page: https://github.com/fluzzi/connpy
 Author: Federico Luzzi
 Author-email: fluzzi@gmail.com
 License: MIT License
 Project-URL: Bug Tracker, https://github.com/fluzzi/connpy/issues
 Project-URL: Documentation, https://fluzzi.github.io/connpy/
```

### Comparing `connpy-3.2.0/README.md` & `connpy-3.2.1/README.md`

 * *Files identical despite different names*

### Comparing `connpy-3.2.0/connpy/__init__.py` & `connpy-3.2.1/connpy/__init__.py`

 * *Files identical despite different names*

### Comparing `connpy-3.2.0/connpy/ai.py` & `connpy-3.2.1/connpy/ai.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 import openai
-import requests
 import json
 import re
 import ast
 from textwrap import dedent
 from .core import nodes
 
 class ai:
```

### Comparing `connpy-3.2.0/connpy/api.py` & `connpy-3.2.1/connpy/api.py`

 * *Files identical despite different names*

### Comparing `connpy-3.2.0/connpy/completion.py` & `connpy-3.2.1/connpy/completion.py`

 * *Files identical despite different names*

### Comparing `connpy-3.2.0/connpy/configfile.py` & `connpy-3.2.1/connpy/configfile.py`

 * *Files identical despite different names*

### Comparing `connpy-3.2.0/connpy/connapp.py` & `connpy-3.2.1/connpy/connapp.py`

 * *Files identical despite different names*

### Comparing `connpy-3.2.0/connpy/core.py` & `connpy-3.2.1/connpy/core.py`

 * *Files identical despite different names*

### Comparing `connpy-3.2.0/connpy.egg-info/PKG-INFO` & `connpy-3.2.1/connpy.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: connpy
-Version: 3.2.0
+Version: 3.2.1
 Summary: Connpy is a SSH/Telnet connection manager and automation module
 Home-page: https://github.com/fluzzi/connpy
 Author: Federico Luzzi
 Author-email: fluzzi@gmail.com
 License: MIT License
 Project-URL: Bug Tracker, https://github.com/fluzzi/connpy/issues
 Project-URL: Documentation, https://fluzzi.github.io/connpy/
```

### Comparing `connpy-3.2.0/setup.cfg` & `connpy-3.2.1/setup.cfg`

 * *Files 5% similar despite different names*

```diff
@@ -28,15 +28,14 @@
 	inquirer
 	pexpect
 	pycryptodome
 	Flask
 	waitress
 	PyYAML
 	openai
-	requests
 
 [options.extras_require]
 fuzzysearch = pyfzf
 
 [options.entry_points]
 console_scripts = 
 	conn = connpy.__main__:main
```

