# Comparing `tmp/cagen-0.2.0b5.tar.gz` & `tmp/cagen-0.2.0b6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cagen-0.2.0b5.tar", last modified: Fri May  5 16:35:41 2023, max compression
+gzip compressed data, was "cagen-0.2.0b6.tar", last modified: Fri May  5 16:39:39 2023, max compression
```

## Comparing `cagen-0.2.0b5.tar` & `cagen-0.2.0b6.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 xan       (1000) xan       (1000)        0 2023-05-05 16:35:41.063259 cagen-0.2.0b5/
--rw-r--r--   0 xan       (1000) xan       (1000)      177 2023-03-28 18:54:19.000000 cagen-0.2.0b5/MANIFEST.in
--rw-r--r--   0 xan       (1000) xan       (1000)     4358 2023-05-05 16:35:41.063259 cagen-0.2.0b5/PKG-INFO
--rw-r--r--   0 xan       (1000) xan       (1000)     3595 2023-04-24 11:33:16.000000 cagen-0.2.0b5/README.md
--rw-r--r--   0 xan       (1000) xan       (1000)     1187 2023-05-05 16:35:33.000000 cagen-0.2.0b5/pyproject.toml
--rw-r--r--   0 xan       (1000) xan       (1000)       38 2023-05-05 16:35:41.063259 cagen-0.2.0b5/setup.cfg
-drwxr-xr-x   0 xan       (1000) xan       (1000)        0 2023-05-05 16:35:41.059926 cagen-0.2.0b5/src/
-drwxr-xr-x   0 xan       (1000) xan       (1000)        0 2023-05-05 16:35:41.063259 cagen-0.2.0b5/src/cagen/
--rw-r--r--   0 xan       (1000) xan       (1000)      112 2023-03-28 18:54:41.000000 cagen-0.2.0b5/src/cagen/__init__.py
--rw-r--r--   0 xan       (1000) xan       (1000)     5337 2023-05-05 16:35:24.000000 cagen-0.2.0b5/src/cagen/cmd.py
--rw-r--r--   0 xan       (1000) xan       (1000)     8848 2023-04-24 08:23:27.000000 cagen-0.2.0b5/src/cagen/libcagen.py
-drwxr-xr-x   0 xan       (1000) xan       (1000)        0 2023-05-05 16:35:41.063259 cagen-0.2.0b5/src/cagen/templates/
--rw-r--r--   0 xan       (1000) xan       (1000)      414 2023-04-17 11:16:34.000000 cagen-0.2.0b5/src/cagen/templates/list.md.tmpl
--rw-r--r--   0 xan       (1000) xan       (1000)      107 2023-03-28 18:55:41.000000 cagen-0.2.0b5/src/cagen/templates/list.md.tmpl.license
--rw-r--r--   0 xan       (1000) xan       (1000)     1782 2023-04-17 20:18:26.000000 cagen-0.2.0b5/src/cagen/templates/schema.tmpl
--rw-r--r--   0 xan       (1000) xan       (1000)      107 2023-03-28 18:55:48.000000 cagen-0.2.0b5/src/cagen/templates/schema.tmpl.license
-drwxr-xr-x   0 xan       (1000) xan       (1000)        0 2023-05-05 16:35:41.063259 cagen-0.2.0b5/src/cagen.egg-info/
--rw-r--r--   0 xan       (1000) xan       (1000)     4358 2023-05-05 16:35:41.000000 cagen-0.2.0b5/src/cagen.egg-info/PKG-INFO
--rw-r--r--   0 xan       (1000) xan       (1000)      443 2023-05-05 16:35:41.000000 cagen-0.2.0b5/src/cagen.egg-info/SOURCES.txt
--rw-r--r--   0 xan       (1000) xan       (1000)        1 2023-05-05 16:35:41.000000 cagen-0.2.0b5/src/cagen.egg-info/dependency_links.txt
--rw-r--r--   0 xan       (1000) xan       (1000)      114 2023-05-05 16:35:41.000000 cagen-0.2.0b5/src/cagen.egg-info/entry_points.txt
--rw-r--r--   0 xan       (1000) xan       (1000)       53 2023-05-05 16:35:41.000000 cagen-0.2.0b5/src/cagen.egg-info/requires.txt
--rw-r--r--   0 xan       (1000) xan       (1000)        6 2023-05-05 16:35:41.000000 cagen-0.2.0b5/src/cagen.egg-info/top_level.txt
+drwxr-xr-x   0 xan       (1000) xan       (1000)        0 2023-05-05 16:39:39.100291 cagen-0.2.0b6/
+-rw-r--r--   0 xan       (1000) xan       (1000)      177 2023-03-28 18:54:19.000000 cagen-0.2.0b6/MANIFEST.in
+-rw-r--r--   0 xan       (1000) xan       (1000)     4358 2023-05-05 16:39:39.100291 cagen-0.2.0b6/PKG-INFO
+-rw-r--r--   0 xan       (1000) xan       (1000)     3595 2023-04-24 11:33:16.000000 cagen-0.2.0b6/README.md
+-rw-r--r--   0 xan       (1000) xan       (1000)     1187 2023-05-05 16:39:27.000000 cagen-0.2.0b6/pyproject.toml
+-rw-r--r--   0 xan       (1000) xan       (1000)       38 2023-05-05 16:39:39.100291 cagen-0.2.0b6/setup.cfg
+drwxr-xr-x   0 xan       (1000) xan       (1000)        0 2023-05-05 16:39:39.096958 cagen-0.2.0b6/src/
+drwxr-xr-x   0 xan       (1000) xan       (1000)        0 2023-05-05 16:39:39.100291 cagen-0.2.0b6/src/cagen/
+-rw-r--r--   0 xan       (1000) xan       (1000)      112 2023-03-28 18:54:41.000000 cagen-0.2.0b6/src/cagen/__init__.py
+-rw-r--r--   0 xan       (1000) xan       (1000)     5353 2023-05-05 16:39:18.000000 cagen-0.2.0b6/src/cagen/cmd.py
+-rw-r--r--   0 xan       (1000) xan       (1000)     8848 2023-04-24 08:23:27.000000 cagen-0.2.0b6/src/cagen/libcagen.py
+drwxr-xr-x   0 xan       (1000) xan       (1000)        0 2023-05-05 16:39:39.100291 cagen-0.2.0b6/src/cagen/templates/
+-rw-r--r--   0 xan       (1000) xan       (1000)      414 2023-04-17 11:16:34.000000 cagen-0.2.0b6/src/cagen/templates/list.md.tmpl
+-rw-r--r--   0 xan       (1000) xan       (1000)      107 2023-03-28 18:55:41.000000 cagen-0.2.0b6/src/cagen/templates/list.md.tmpl.license
+-rw-r--r--   0 xan       (1000) xan       (1000)     1782 2023-04-17 20:18:26.000000 cagen-0.2.0b6/src/cagen/templates/schema.tmpl
+-rw-r--r--   0 xan       (1000) xan       (1000)      107 2023-03-28 18:55:48.000000 cagen-0.2.0b6/src/cagen/templates/schema.tmpl.license
+drwxr-xr-x   0 xan       (1000) xan       (1000)        0 2023-05-05 16:39:39.100291 cagen-0.2.0b6/src/cagen.egg-info/
+-rw-r--r--   0 xan       (1000) xan       (1000)     4358 2023-05-05 16:39:39.000000 cagen-0.2.0b6/src/cagen.egg-info/PKG-INFO
+-rw-r--r--   0 xan       (1000) xan       (1000)      443 2023-05-05 16:39:39.000000 cagen-0.2.0b6/src/cagen.egg-info/SOURCES.txt
+-rw-r--r--   0 xan       (1000) xan       (1000)        1 2023-05-05 16:39:39.000000 cagen-0.2.0b6/src/cagen.egg-info/dependency_links.txt
+-rw-r--r--   0 xan       (1000) xan       (1000)      114 2023-05-05 16:39:39.000000 cagen-0.2.0b6/src/cagen.egg-info/entry_points.txt
+-rw-r--r--   0 xan       (1000) xan       (1000)       53 2023-05-05 16:39:39.000000 cagen-0.2.0b6/src/cagen.egg-info/requires.txt
+-rw-r--r--   0 xan       (1000) xan       (1000)        6 2023-05-05 16:39:39.000000 cagen-0.2.0b6/src/cagen.egg-info/top_level.txt
```

### Comparing `cagen-0.2.0b5/PKG-INFO` & `cagen-0.2.0b6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cagen
-Version: 0.2.0b5
+Version: 0.2.0b6
 Summary: A static site generator. Originally it was intended for cmpalgorithms project
 Author: Xavier B.
 Project-URL: Homepage, https://repo.or.cz/cagen.git
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
```

### Comparing `cagen-0.2.0b5/README.md` & `cagen-0.2.0b6/README.md`

 * *Files identical despite different names*

### Comparing `cagen-0.2.0b5/pyproject.toml` & `cagen-0.2.0b6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 [project.scripts]
 cagen = "cagen.cmd:cagen_cli"
 cagen-list = "cagen.cmd:cagen_list"
 cagen-make = "cagen.cmd:cagen_make"
 
 [project]
 name = "cagen"
-version = "0.2.0.beta-5"
+version = "0.2.0.beta-6"
 authors = [{'name'="Xavier B."}]
 description = "A static site generator. Originally it was intended for cmpalgorithms project"
 readme = "README.md"
 requires-python = ">=3.10"
 classifiers = [
         'Development Status :: 3 - Alpha',
         'Environment :: Console',
```

### Comparing `cagen-0.2.0b5/src/cagen/cmd.py` & `cagen-0.2.0b6/src/cagen/cmd.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 # SPDX-FileCopyrightText: 2023 Xavier Bordoy <somenxavier@posteo.net>
 #
 # SPDX-License-Identifier: GPL-2.0-only
 
 import cagen.libcagen as libcagen
 import argparse
-import os.path
+import os.path, pathlib
 import shutil
 from mako.template import Template
 import importlib.resources
 
 def cagen_cli():
     """Defines the `cagen` command line script function to call from pyproject.toml"""
 
@@ -107,13 +107,13 @@
 
     if args.init:
         with open("Makefile", "w") as f:
             f.write(maketemplate)
     elif args.templates:
         if not os.path.exists('templates'):
             os.makedirs('templates')
-            for f in importlib.resources.files('cagen', 'templates'):
+            for f in importlib.resources.files('cagen.templates').iterdir():
                 print(f)
                 #original = str(importlib.resources.files('cagen'))
                 #shutil.copy(original + f, 'templates'+f)
     else:
         print("See --help for hints")
```

### Comparing `cagen-0.2.0b5/src/cagen/libcagen.py` & `cagen-0.2.0b6/src/cagen/libcagen.py`

 * *Files identical despite different names*

### Comparing `cagen-0.2.0b5/src/cagen/templates/schema.tmpl` & `cagen-0.2.0b6/src/cagen/templates/schema.tmpl`

 * *Files identical despite different names*

### Comparing `cagen-0.2.0b5/src/cagen.egg-info/PKG-INFO` & `cagen-0.2.0b6/src/cagen.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cagen
-Version: 0.2.0b5
+Version: 0.2.0b6
 Summary: A static site generator. Originally it was intended for cmpalgorithms project
 Author: Xavier B.
 Project-URL: Homepage, https://repo.or.cz/cagen.git
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: GNU General Public License v2 (GPLv2)
```

