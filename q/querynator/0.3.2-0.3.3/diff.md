# Comparing `tmp/querynator-0.3.2.tar.gz` & `tmp/querynator-0.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "querynator-0.3.2.tar", last modified: Fri May  5 11:29:59 2023, max compression
+gzip compressed data, was "querynator-0.3.3.tar", last modified: Fri May  5 12:11:21 2023, max compression
```

## Comparing `querynator-0.3.2.tar` & `querynator-0.3.3.tar`

### file list

```diff
@@ -1,55 +1,55 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 11:29:59.905329 querynator-0.3.2/
--rw-r--r--   0 runner    (1001) docker     (123)     2331 2023-05-05 11:28:59.000000 querynator-0.3.2/CHANGELOG.rst
--rw-r--r--   0 runner    (1001) docker     (123)     4833 2023-05-05 11:28:59.000000 querynator-0.3.2/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-05-05 11:28:59.000000 querynator-0.3.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      298 2023-05-05 11:28:59.000000 querynator-0.3.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     5701 2023-05-05 11:29:59.905329 querynator-0.3.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2706 2023-05-05 11:28:59.000000 querynator-0.3.2/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 11:29:59.901328 querynator-0.3.2/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      611 2023-05-05 11:28:59.000000 querynator-0.3.2/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-05-05 11:28:59.000000 querynator-0.3.2/docs/changelog.rst
--rwxr-xr-x   0 runner    (1001) docker     (123)     4881 2023-05-05 11:28:59.000000 querynator-0.3.2/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-05-05 11:28:59.000000 querynator-0.3.2/docs/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (123)      290 2023-05-05 11:28:59.000000 querynator-0.3.2/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1310 2023-05-05 11:28:59.000000 querynator-0.3.2/docs/installation.rst
--rw-r--r--   0 runner    (1001) docker     (123)      802 2023-05-05 11:28:59.000000 querynator-0.3.2/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (123)     1186 2023-05-05 11:28:59.000000 querynator-0.3.2/docs/modules.rst
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-05-05 11:28:59.000000 querynator-0.3.2/docs/readme.rst
--rw-r--r--   0 runner    (1001) docker     (123)     9198 2023-05-05 11:28:59.000000 querynator-0.3.2/docs/usage.rst
--rw-r--r--   0 runner    (1001) docker     (123)      476 2023-05-05 11:28:59.000000 querynator-0.3.2/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 11:29:59.901328 querynator-0.3.2/querynator/
--rw-r--r--   0 runner    (1001) docker     (123)      195 2023-05-05 11:28:59.000000 querynator-0.3.2/querynator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15304 2023-05-05 11:28:59.000000 querynator-0.3.2/querynator/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 11:29:59.901328 querynator-0.3.2/querynator/helper_functions/
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-05-05 11:28:59.000000 querynator-0.3.2/querynator/helper_functions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1702 2023-05-05 11:28:59.000000 querynator-0.3.2/querynator/helper_functions/helper_functions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 11:29:59.905329 querynator-0.3.2/querynator/query_api/
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-05-05 11:28:59.000000 querynator-0.3.2/querynator/query_api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7952 2023-05-05 11:28:59.000000 querynator-0.3.2/querynator/query_api/cancertypes.js
--rw-r--r--   0 runner    (1001) docker     (123)     8423 2023-05-05 11:28:59.000000 querynator-0.3.2/querynator/query_api/cgi_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    19214 2023-05-05 11:28:59.000000 querynator-0.3.2/querynator/query_api/civic_api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 11:29:59.905329 querynator-0.3.2/querynator/report_scripts/
--rw-r--r--   0 runner    (1001) docker     (123)      147 2023-05-05 11:28:59.000000 querynator-0.3.2/querynator/report_scripts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10267 2023-05-05 11:28:59.000000 querynator-0.3.2/querynator/report_scripts/combine_cgi.py
--rw-r--r--   0 runner    (1001) docker     (123)     2431 2023-05-05 11:28:59.000000 querynator-0.3.2/querynator/report_scripts/combine_cgi_civic.py
--rw-r--r--   0 runner    (1001) docker     (123)     4498 2023-05-05 11:28:59.000000 querynator-0.3.2/querynator/report_scripts/combine_civic.py
--rw-r--r--   0 runner    (1001) docker     (123)    23675 2023-05-05 11:28:59.000000 querynator-0.3.2/querynator/report_scripts/create_report.py
--rw-r--r--   0 runner    (1001) docker     (123)    16843 2023-05-05 11:28:59.000000 querynator-0.3.2/querynator/report_scripts/sort_variants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 11:29:59.905329 querynator-0.3.2/querynator/report_scripts/templates/
--rw-r--r--   0 runner    (1001) docker     (123)     3795 2023-05-05 11:28:59.000000 querynator-0.3.2/querynator/report_scripts/templates/template_individual.html
--rw-r--r--   0 runner    (1001) docker     (123)     4201 2023-05-05 11:28:59.000000 querynator-0.3.2/querynator/report_scripts/templates/template_overall_plotly_pieplots.html
--rw-r--r--   0 runner    (1001) docker     (123)     3519 2023-05-05 11:28:59.000000 querynator-0.3.2/querynator/report_scripts/templates/template_overall_upsetplots.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 11:29:59.901328 querynator-0.3.2/querynator.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5701 2023-05-05 11:29:59.000000 querynator-0.3.2/querynator.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1279 2023-05-05 11:29:59.000000 querynator-0.3.2/querynator.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 11:29:59.000000 querynator-0.3.2/querynator.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-05-05 11:29:59.000000 querynator-0.3.2/querynator.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 11:29:08.000000 querynator-0.3.2/querynator.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      201 2023-05-05 11:29:59.000000 querynator-0.3.2/querynator.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-05 11:29:59.000000 querynator-0.3.2/querynator.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      201 2023-05-05 11:28:59.000000 querynator-0.3.2/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-05 11:29:59.905329 querynator-0.3.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1498 2023-05-05 11:28:59.000000 querynator-0.3.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 11:29:59.905329 querynator-0.3.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-05-05 11:28:59.000000 querynator-0.3.2/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1978 2023-05-05 11:28:59.000000 querynator-0.3.2/tests/test_querynator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 12:11:21.601464 querynator-0.3.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     2487 2023-05-05 12:10:30.000000 querynator-0.3.3/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     4833 2023-05-05 12:10:30.000000 querynator-0.3.3/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-05-05 12:10:30.000000 querynator-0.3.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      298 2023-05-05 12:10:30.000000 querynator-0.3.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5857 2023-05-05 12:11:21.601464 querynator-0.3.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2706 2023-05-05 12:10:30.000000 querynator-0.3.3/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 12:11:21.601464 querynator-0.3.3/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      611 2023-05-05 12:10:30.000000 querynator-0.3.3/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-05-05 12:10:30.000000 querynator-0.3.3/docs/changelog.rst
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4881 2023-05-05 12:10:30.000000 querynator-0.3.3/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-05-05 12:10:30.000000 querynator-0.3.3/docs/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      290 2023-05-05 12:10:30.000000 querynator-0.3.3/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1310 2023-05-05 12:10:30.000000 querynator-0.3.3/docs/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      802 2023-05-05 12:10:30.000000 querynator-0.3.3/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (123)     1186 2023-05-05 12:10:30.000000 querynator-0.3.3/docs/modules.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-05-05 12:10:30.000000 querynator-0.3.3/docs/readme.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     9198 2023-05-05 12:10:30.000000 querynator-0.3.3/docs/usage.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      476 2023-05-05 12:10:30.000000 querynator-0.3.3/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 12:11:21.601464 querynator-0.3.3/querynator/
+-rw-r--r--   0 runner    (1001) docker     (123)      195 2023-05-05 12:10:30.000000 querynator-0.3.3/querynator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15304 2023-05-05 12:10:30.000000 querynator-0.3.3/querynator/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 12:11:21.601464 querynator-0.3.3/querynator/helper_functions/
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-05-05 12:10:30.000000 querynator-0.3.3/querynator/helper_functions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1702 2023-05-05 12:10:30.000000 querynator-0.3.3/querynator/helper_functions/helper_functions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 12:11:21.601464 querynator-0.3.3/querynator/query_api/
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-05-05 12:10:30.000000 querynator-0.3.3/querynator/query_api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7952 2023-05-05 12:10:30.000000 querynator-0.3.3/querynator/query_api/cancertypes.js
+-rw-r--r--   0 runner    (1001) docker     (123)     8423 2023-05-05 12:10:30.000000 querynator-0.3.3/querynator/query_api/cgi_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19214 2023-05-05 12:10:30.000000 querynator-0.3.3/querynator/query_api/civic_api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 12:11:21.601464 querynator-0.3.3/querynator/report_scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)      147 2023-05-05 12:10:30.000000 querynator-0.3.3/querynator/report_scripts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10267 2023-05-05 12:10:30.000000 querynator-0.3.3/querynator/report_scripts/combine_cgi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2431 2023-05-05 12:10:30.000000 querynator-0.3.3/querynator/report_scripts/combine_cgi_civic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4498 2023-05-05 12:10:30.000000 querynator-0.3.3/querynator/report_scripts/combine_civic.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23675 2023-05-05 12:10:30.000000 querynator-0.3.3/querynator/report_scripts/create_report.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16843 2023-05-05 12:10:30.000000 querynator-0.3.3/querynator/report_scripts/sort_variants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 12:11:21.601464 querynator-0.3.3/querynator/report_scripts/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)     3795 2023-05-05 12:10:30.000000 querynator-0.3.3/querynator/report_scripts/templates/template_individual.html
+-rw-r--r--   0 runner    (1001) docker     (123)     4201 2023-05-05 12:10:30.000000 querynator-0.3.3/querynator/report_scripts/templates/template_overall_plotly_pieplots.html
+-rw-r--r--   0 runner    (1001) docker     (123)     3519 2023-05-05 12:10:30.000000 querynator-0.3.3/querynator/report_scripts/templates/template_overall_upsetplots.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 12:11:21.601464 querynator-0.3.3/querynator.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5857 2023-05-05 12:11:21.000000 querynator-0.3.3/querynator.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1279 2023-05-05 12:11:21.000000 querynator-0.3.3/querynator.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 12:11:21.000000 querynator-0.3.3/querynator.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-05-05 12:11:21.000000 querynator-0.3.3/querynator.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 12:10:40.000000 querynator-0.3.3/querynator.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      211 2023-05-05 12:11:21.000000 querynator-0.3.3/querynator.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-05 12:11:21.000000 querynator-0.3.3/querynator.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      211 2023-05-05 12:10:30.000000 querynator-0.3.3/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-05 12:11:21.601464 querynator-0.3.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1498 2023-05-05 12:10:30.000000 querynator-0.3.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 12:11:21.601464 querynator-0.3.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-05-05 12:10:30.000000 querynator-0.3.3/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1978 2023-05-05 12:10:30.000000 querynator-0.3.3/tests/test_querynator.py
```

### Comparing `querynator-0.3.2/CHANGELOG.rst` & `querynator-0.3.3/CHANGELOG.rst`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,23 @@
 Changelog
 ============
 
+0.3.3 - Iron Mercury  (2023-05-05)
+---------------------------------------------
+
+**Added**
+
+**Fixed**
+
+* Fixed API docs
+
+**Dependencies**
+
+**Deprecated**
+
 0.3.2 - Iron Mercury  (2023-05-05)
 ---------------------------------------------
 
 **Added**
 
 **Fixed**
```

### Comparing `querynator-0.3.2/CONTRIBUTING.rst` & `querynator-0.3.3/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `querynator-0.3.2/LICENSE` & `querynator-0.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `querynator-0.3.2/PKG-INFO` & `querynator-0.3.3/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: querynator
-Version: 0.3.2
+Version: 0.3.3
 Summary: Python package to query cancer variant databases
 Home-page: https://github.com/qbic-pipelines/querynator
 Author: Susanne Jodoin, Mark Polster
 Author-email: susanne.jodoin@qbic.uni-tuebingen.de, mark.polster@uni-tuebingen.de
 License: MIT license
 Keywords: querynator
 Classifier: Development Status :: 2 - Pre-Alpha
@@ -76,14 +76,27 @@
 
 
 
 
 Changelog
 ============
 
+0.3.3 - Iron Mercury  (2023-05-05)
+---------------------------------------------
+
+**Added**
+
+**Fixed**
+
+* Fixed API docs
+
+**Dependencies**
+
+**Deprecated**
+
 0.3.2 - Iron Mercury  (2023-05-05)
 ---------------------------------------------
 
 **Added**
 
 **Fixed**
```

### Comparing `querynator-0.3.2/README.rst` & `querynator-0.3.3/README.rst`

 * *Files identical despite different names*

### Comparing `querynator-0.3.2/docs/Makefile` & `querynator-0.3.3/docs/Makefile`

 * *Files identical despite different names*

### Comparing `querynator-0.3.2/docs/conf.py` & `querynator-0.3.3/docs/conf.py`

 * *Files identical despite different names*

### Comparing `querynator-0.3.2/docs/installation.rst` & `querynator-0.3.3/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `querynator-0.3.2/docs/make.bat` & `querynator-0.3.3/docs/make.bat`

 * *Files identical despite different names*

### Comparing `querynator-0.3.2/docs/modules.rst` & `querynator-0.3.3/docs/modules.rst`

 * *Files identical despite different names*

### Comparing `querynator-0.3.2/docs/usage.rst` & `querynator-0.3.3/docs/usage.rst`

 * *Files identical despite different names*

### Comparing `querynator-0.3.2/querynator/__main__.py` & `querynator-0.3.3/querynator/__main__.py`

 * *Files identical despite different names*

### Comparing `querynator-0.3.2/querynator/helper_functions/helper_functions.py` & `querynator-0.3.3/querynator/helper_functions/helper_functions.py`

 * *Files identical despite different names*

### Comparing `querynator-0.3.2/querynator/query_api/cancertypes.js` & `querynator-0.3.3/querynator/query_api/cancertypes.js`

 * *Files identical despite different names*

### Comparing `querynator-0.3.2/querynator/query_api/cgi_api.py` & `querynator-0.3.3/querynator/query_api/cgi_api.py`

 * *Files identical despite different names*

### Comparing `querynator-0.3.2/querynator/query_api/civic_api.py` & `querynator-0.3.3/querynator/query_api/civic_api.py`

 * *Files identical despite different names*

### Comparing `querynator-0.3.2/querynator/report_scripts/combine_cgi.py` & `querynator-0.3.3/querynator/report_scripts/combine_cgi.py`

 * *Files identical despite different names*

### Comparing `querynator-0.3.2/querynator/report_scripts/combine_cgi_civic.py` & `querynator-0.3.3/querynator/report_scripts/combine_cgi_civic.py`

 * *Files identical despite different names*

### Comparing `querynator-0.3.2/querynator/report_scripts/combine_civic.py` & `querynator-0.3.3/querynator/report_scripts/combine_civic.py`

 * *Files identical despite different names*

### Comparing `querynator-0.3.2/querynator/report_scripts/create_report.py` & `querynator-0.3.3/querynator/report_scripts/create_report.py`

 * *Files identical despite different names*

### Comparing `querynator-0.3.2/querynator/report_scripts/sort_variants.py` & `querynator-0.3.3/querynator/report_scripts/sort_variants.py`

 * *Files identical despite different names*

### Comparing `querynator-0.3.2/querynator/report_scripts/templates/template_individual.html` & `querynator-0.3.3/querynator/report_scripts/templates/template_individual.html`

 * *Files identical despite different names*

### Comparing `querynator-0.3.2/querynator/report_scripts/templates/template_overall_plotly_pieplots.html` & `querynator-0.3.3/querynator/report_scripts/templates/template_overall_plotly_pieplots.html`

 * *Files identical despite different names*

### Comparing `querynator-0.3.2/querynator/report_scripts/templates/template_overall_upsetplots.html` & `querynator-0.3.3/querynator/report_scripts/templates/template_overall_upsetplots.html`

 * *Files identical despite different names*

### Comparing `querynator-0.3.2/querynator.egg-info/PKG-INFO` & `querynator-0.3.3/querynator.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: querynator
-Version: 0.3.2
+Version: 0.3.3
 Summary: Python package to query cancer variant databases
 Home-page: https://github.com/qbic-pipelines/querynator
 Author: Susanne Jodoin, Mark Polster
 Author-email: susanne.jodoin@qbic.uni-tuebingen.de, mark.polster@uni-tuebingen.de
 License: MIT license
 Keywords: querynator
 Classifier: Development Status :: 2 - Pre-Alpha
@@ -76,14 +76,27 @@
 
 
 
 
 Changelog
 ============
 
+0.3.3 - Iron Mercury  (2023-05-05)
+---------------------------------------------
+
+**Added**
+
+**Fixed**
+
+* Fixed API docs
+
+**Dependencies**
+
+**Deprecated**
+
 0.3.2 - Iron Mercury  (2023-05-05)
 ---------------------------------------------
 
 **Added**
 
 **Fixed**
```

### Comparing `querynator-0.3.2/querynator.egg-info/SOURCES.txt` & `querynator-0.3.3/querynator.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `querynator-0.3.2/setup.py` & `querynator-0.3.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -42,10 +42,10 @@
     keywords="querynator",
     name="querynator",
     packages=find_packages(exclude=("docs")),
     package_data={"": ["report_scripts/templates/*.html"]},
     test_suite="tests",
     tests_require=test_requirements,
     url="https://github.com/qbic-pipelines/querynator",
-    version="0.3.2",
+    version="0.3.3",
     zip_safe=False,
 )
```

### Comparing `querynator-0.3.2/tests/test_querynator.py` & `querynator-0.3.3/tests/test_querynator.py`

 * *Files identical despite different names*

