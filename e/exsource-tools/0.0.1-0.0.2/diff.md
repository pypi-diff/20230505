# Comparing `tmp/exsource_tools-0.0.1.tar.gz` & `tmp/exsource_tools-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/exsource_tools-0.0.1.tar", last modified: Mon Apr 17 21:25:25 2023, max compression
+gzip compressed data, was "dist/exsource_tools-0.0.2.tar", last modified: Fri May  5 19:48:33 2023, max compression
```

## Comparing `exsource_tools-0.0.1.tar` & `exsource_tools-0.0.2.tar`

### file list

```diff
@@ -1,18 +1,22 @@
-drwxrwxr-x   0 js3214    (1000) js3214    (1000)        0 2023-04-17 21:25:25.000000 exsource_tools-0.0.1/
--rw-rw-r--   0 js3214    (1000) js3214    (1000)     1352 2023-04-17 21:25:25.000000 exsource_tools-0.0.1/PKG-INFO
--rw-rw-r--   0 js3214    (1000) js3214    (1000)      546 2023-04-17 21:16:27.000000 exsource_tools-0.0.1/README.md
-drwxrwxr-x   0 js3214    (1000) js3214    (1000)        0 2023-04-17 21:25:25.000000 exsource_tools-0.0.1/exsource_tools/
--rw-rw-r--   0 js3214    (1000) js3214    (1000)       80 2023-04-17 15:18:17.000000 exsource_tools-0.0.1/exsource_tools/__init__.py
-drwxrwxr-x   0 js3214    (1000) js3214    (1000)        0 2023-04-17 21:25:25.000000 exsource_tools-0.0.1/exsource_tools/schemas/
--rw-rw-r--   0 js3214    (1000) js3214    (1000)     4226 2023-04-17 14:38:37.000000 exsource_tools-0.0.1/exsource_tools/schemas/exsource.schema.json
--rw-rw-r--   0 js3214    (1000) js3214    (1000)     7183 2023-04-17 21:02:01.000000 exsource_tools-0.0.1/exsource_tools/tools.py
-drwxrwxr-x   0 js3214    (1000) js3214    (1000)        0 2023-04-17 21:25:25.000000 exsource_tools-0.0.1/exsource_tools.egg-info/
--rw-rw-r--   0 js3214    (1000) js3214    (1000)     1352 2023-04-17 21:25:25.000000 exsource_tools-0.0.1/exsource_tools.egg-info/PKG-INFO
--rw-rw-r--   0 js3214    (1000) js3214    (1000)      380 2023-04-17 21:25:25.000000 exsource_tools-0.0.1/exsource_tools.egg-info/SOURCES.txt
--rw-rw-r--   0 js3214    (1000) js3214    (1000)        1 2023-04-17 21:25:25.000000 exsource_tools-0.0.1/exsource_tools.egg-info/dependency_links.txt
--rw-rw-r--   0 js3214    (1000) js3214    (1000)       61 2023-04-17 21:25:25.000000 exsource_tools-0.0.1/exsource_tools.egg-info/entry_points.txt
--rw-rw-r--   0 js3214    (1000) js3214    (1000)        1 2023-04-17 12:35:00.000000 exsource_tools-0.0.1/exsource_tools.egg-info/not-zip-safe
--rw-rw-r--   0 js3214    (1000) js3214    (1000)       52 2023-04-17 21:25:25.000000 exsource_tools-0.0.1/exsource_tools.egg-info/requires.txt
--rw-rw-r--   0 js3214    (1000) js3214    (1000)       15 2023-04-17 21:25:25.000000 exsource_tools-0.0.1/exsource_tools.egg-info/top_level.txt
--rw-rw-r--   0 js3214    (1000) js3214    (1000)       38 2023-04-17 21:25:25.000000 exsource_tools-0.0.1/setup.cfg
--rw-rw-r--   0 js3214    (1000) js3214    (1000)     2082 2023-04-17 15:08:33.000000 exsource_tools-0.0.1/setup.py
+drwxrwxr-x   0 js3214    (1000) js3214    (1000)        0 2023-05-05 19:48:33.000000 exsource_tools-0.0.2/
+-rw-rw-r--   0 js3214    (1000) js3214    (1000)     1352 2023-05-05 19:48:33.000000 exsource_tools-0.0.2/PKG-INFO
+-rw-rw-r--   0 js3214    (1000) js3214    (1000)      546 2023-04-17 21:16:27.000000 exsource_tools-0.0.2/README.md
+drwxrwxr-x   0 js3214    (1000) js3214    (1000)        0 2023-05-05 19:48:33.000000 exsource_tools-0.0.2/exsource_tools/
+-rw-rw-r--   0 js3214    (1000) js3214    (1000)      132 2023-04-21 09:46:07.000000 exsource_tools-0.0.2/exsource_tools/__init__.py
+drwxrwxr-x   0 js3214    (1000) js3214    (1000)        0 2023-05-05 19:48:33.000000 exsource_tools-0.0.2/exsource_tools/schemas/
+-rw-rw-r--   0 js3214    (1000) js3214    (1000)     5044 2023-05-03 14:26:55.000000 exsource_tools-0.0.2/exsource_tools/schemas/exsource.schema.json
+-rw-rw-r--   0 js3214    (1000) js3214    (1000)    25420 2023-05-05 17:35:45.000000 exsource_tools-0.0.2/exsource_tools/tools.py
+-rw-rw-r--   0 js3214    (1000) js3214    (1000)     3393 2023-05-03 13:22:06.000000 exsource_tools-0.0.2/exsource_tools/utils.py
+drwxrwxr-x   0 js3214    (1000) js3214    (1000)        0 2023-05-05 19:48:33.000000 exsource_tools-0.0.2/exsource_tools.egg-info/
+-rw-rw-r--   0 js3214    (1000) js3214    (1000)     1352 2023-05-05 19:48:33.000000 exsource_tools-0.0.2/exsource_tools.egg-info/PKG-INFO
+-rw-rw-r--   0 js3214    (1000) js3214    (1000)      442 2023-05-05 19:48:33.000000 exsource_tools-0.0.2/exsource_tools.egg-info/SOURCES.txt
+-rw-rw-r--   0 js3214    (1000) js3214    (1000)        1 2023-05-05 19:48:33.000000 exsource_tools-0.0.2/exsource_tools.egg-info/dependency_links.txt
+-rw-rw-r--   0 js3214    (1000) js3214    (1000)       61 2023-05-05 19:48:33.000000 exsource_tools-0.0.2/exsource_tools.egg-info/entry_points.txt
+-rw-rw-r--   0 js3214    (1000) js3214    (1000)        1 2023-04-17 12:35:00.000000 exsource_tools-0.0.2/exsource_tools.egg-info/not-zip-safe
+-rw-rw-r--   0 js3214    (1000) js3214    (1000)       52 2023-05-05 19:48:33.000000 exsource_tools-0.0.2/exsource_tools.egg-info/requires.txt
+-rw-rw-r--   0 js3214    (1000) js3214    (1000)       21 2023-05-05 19:48:33.000000 exsource_tools-0.0.2/exsource_tools.egg-info/top_level.txt
+-rw-rw-r--   0 js3214    (1000) js3214    (1000)       38 2023-05-05 19:48:33.000000 exsource_tools-0.0.2/setup.cfg
+-rw-rw-r--   0 js3214    (1000) js3214    (1000)     2082 2023-04-20 13:26:16.000000 exsource_tools-0.0.2/setup.py
+drwxrwxr-x   0 js3214    (1000) js3214    (1000)        0 2023-05-05 19:48:33.000000 exsource_tools-0.0.2/tests/
+-rw-rw-r--   0 js3214    (1000) js3214    (1000)        0 2023-04-21 09:39:47.000000 exsource_tools-0.0.2/tests/__init__.py
+-rw-rw-r--   0 js3214    (1000) js3214    (1000)     2330 2023-04-26 14:40:54.000000 exsource_tools-0.0.2/tests/test_tools.py
```

### Comparing `exsource_tools-0.0.1/PKG-INFO` & `exsource_tools-0.0.2/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: exsource_tools
-Version: 0.0.1
+Version: 0.0.2
 Summary: Python tools for using Exsource files
 Home-page: https://gitlab.com/gitbuilding/exsource-tools
 Author: Julian Stirling
 Author-email: julian@julianstirling.co.uk
 License: LGPLv3
 Project-URL: Bug Tracker, https://gitlab.com/gitbuilding/exsource-tools/issues
 Project-URL: Source Code, https://gitlab.com/gitbuilding/exsource-tools
```

### Comparing `exsource_tools-0.0.1/README.md` & `exsource_tools-0.0.2/README.md`

 * *Files identical despite different names*

### Comparing `exsource_tools-0.0.1/exsource_tools/schemas/exsource.schema.json` & `exsource_tools-0.0.2/exsource_tools/schemas/exsource.schema.json`

 * *Files 16% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.8333333333333334%*

 * *Differences: {"'properties'": "{replace: OrderedDict([('exports', OrderedDict([('additionalProperties', False), "*

 * *                 "('description', 'Contains a number of entries each with a custom "*

 * *                 'keyword/property name. Each entry should must define the application used to '*

 * *                 'generate the output files, and the input files to the application, and the '*

 * *                 'output files generated. Each entry should correspond to a single time the '*

 * *                 "application is run.'), […]*

```diff
@@ -24,31 +24,42 @@
                     "type": "object"
                 }
             ]
         }
     },
     "description": "A specification for a file that describes the relationship between hardware exchange files and their source",
     "properties": {
-        "outputs": {
+        "exports": {
             "additionalProperties": false,
-            "description": "Contains a number of entries each with a custom keyword/property name. Each entry should must define the application used to generate the ouptut files, and the input files to the application, and the output files generated. Each entry should correspond to a single time the application is run.",
+            "description": "Contains a number of entries each with a custom keyword/property name. Each entry should must define the application used to generate the output files, and the input files to the application, and the output files generated. Each entry should correspond to a single time the application is run.",
             "patternProperties": {
                 "^[a-zA-Z0-9-_]+$": {
                     "properties": {
                         "app-options": {
                             "description": "List of command line options to pass to application.",
                             "items": {
                                 "type": "string"
                             },
                             "type": "array"
                         },
                         "application": {
                             "description": "Name of the application that processes the input files into the output files",
                             "type": "string"
                         },
+                        "dependencies": {
+                            "description": "List of other files this file depends on. This list doesn't need to be exhaustive. It can be used to ensure outputs are processed in the correct order. If this list is exhaustive then the property `dependencies-exhaustive` should be set to true.",
+                            "items": {
+                                "$ref": "#/definitions/file"
+                            },
+                            "type": "array"
+                        },
+                        "dependencies-exhaustive": {
+                            "description": "This should be set to true if the dependencies list is exhaustive. If unset the value is assumed to be false.",
+                            "type": "boolean"
+                        },
                         "description": {
                             "description": "A human-friendly description of the output file(s)",
                             "type": "string"
                         },
                         "name": {
                             "description": "A human-friendly name of the output file(s). For example 'ACME A1 Crankshaft' rather than'a1_crankshaft_V14-final.step'",
                             "type": "string"
@@ -80,12 +91,12 @@
                     "type": "object"
                 }
             },
             "type": "object"
         }
     },
     "required": [
-        "outputs"
+        "exports"
     ],
     "title": "ExSource Schema",
     "type": "object"
 }
```

### Comparing `exsource_tools-0.0.1/exsource_tools.egg-info/PKG-INFO` & `exsource_tools-0.0.2/exsource_tools.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: exsource-tools
-Version: 0.0.1
+Version: 0.0.2
 Summary: Python tools for using Exsource files
 Home-page: https://gitlab.com/gitbuilding/exsource-tools
 Author: Julian Stirling
 Author-email: julian@julianstirling.co.uk
 License: LGPLv3
 Project-URL: Bug Tracker, https://gitlab.com/gitbuilding/exsource-tools/issues
 Project-URL: Source Code, https://gitlab.com/gitbuilding/exsource-tools
```

### Comparing `exsource_tools-0.0.1/setup.py` & `exsource_tools-0.0.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 '''Setup for the module'''
 
 __author__ = 'Julian Stirling'
-__version__ = '0.0.1'
+__version__ = '0.0.2'
 
 import sys
 from os import path
 import glob
 from setuptools import setup, find_packages
 
 def install():
```

