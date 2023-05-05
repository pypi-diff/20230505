# Comparing `tmp/historical_timelines-0.2.2.tar.gz` & `tmp/historical_timelines-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "historical_timelines-0.2.2.tar", last modified: Tue Apr 18 22:44:42 2023, max compression
+gzip compressed data, was "historical_timelines-0.2.3.tar", last modified: Fri May  5 03:02:44 2023, max compression
```

## Comparing `historical_timelines-0.2.2.tar` & `historical_timelines-0.2.3.tar`

### file list

```diff
@@ -1,50 +1,50 @@
-drwxrwxr-x   0 darthbeep  (1000) darthbeep  (1000)        0 2023-04-18 22:44:42.010106 historical_timelines-0.2.2/
--rw-rw-r--   0 darthbeep  (1000) darthbeep  (1000)      409 2023-04-18 22:42:31.000000 historical_timelines-0.2.2/.bumpversion.cfg
--rw-rw-r--   0 darthbeep  (1000) darthbeep  (1000)      716 2023-04-18 22:36:14.000000 historical_timelines-0.2.2/.readthedocs.yaml
--rw-rw-r--   0 darthbeep  (1000) darthbeep  (1000)     9826 2023-03-29 03:29:39.000000 historical_timelines-0.2.2/CONTRIBUTING.md
--rw-rw-r--   0 darthbeep  (1000) darthbeep  (1000)     1066 2023-04-18 22:36:14.000000 historical_timelines-0.2.2/LICENSE
--rw-rw-r--   0 darthbeep  (1000) darthbeep  (1000)      581 2023-04-18 22:36:14.000000 historical_timelines-0.2.2/MANIFEST.in
--rw-rw-r--   0 darthbeep  (1000) darthbeep  (1000)     2314 2023-03-08 12:54:50.000000 historical_timelines-0.2.2/Makefile
--rw-rw-r--   0 darthbeep  (1000) darthbeep  (1000)     2755 2023-04-18 22:44:42.010106 historical_timelines-0.2.2/PKG-INFO
--rw-rw-r--   0 darthbeep  (1000) darthbeep  (1000)     2462 2023-04-18 22:36:14.000000 historical_timelines-0.2.2/README.md
-drwxrwxr-x   0 darthbeep  (1000) darthbeep  (1000)        0 2023-04-18 22:44:42.002106 historical_timelines-0.2.2/docs/
--rw-rw-r--   0 darthbeep  (1000) darthbeep  (1000)      638 2023-04-18 22:36:14.000000 historical_timelines-0.2.2/docs/Makefile
-drwxrwxr-x   0 darthbeep  (1000) darthbeep  (1000)        0 2023-04-18 22:44:42.006106 historical_timelines-0.2.2/docs/binder/
-drwxrwxr-x   0 darthbeep  (1000) darthbeep  (1000)        0 2023-04-18 22:44:42.006106 historical_timelines-0.2.2/docs/binder/.ipynb_checkpoints/
--rw-rw-r--   0 darthbeep  (1000) darthbeep  (1000)     2678 2023-04-18 22:26:22.000000 historical_timelines-0.2.2/docs/binder/.ipynb_checkpoints/tutorial-checkpoint.ipynb
--rw-rw-r--   0 darthbeep  (1000) darthbeep  (1000)     1967 2023-04-18 22:36:14.000000 historical_timelines-0.2.2/docs/binder/timeline_egypt.csv
--rw-rw-r--   0 darthbeep  (1000) darthbeep  (1000)     3034 2023-04-18 22:36:14.000000 historical_timelines-0.2.2/docs/binder/tutorial.ipynb
--rw-rw-r--   0 darthbeep  (1000) darthbeep  (1000)      804 2023-04-18 22:36:14.000000 historical_timelines-0.2.2/docs/make.bat
--rw-rw-r--   0 darthbeep  (1000) darthbeep  (1000)      173 2023-04-18 22:36:14.000000 historical_timelines-0.2.2/docs/requirements.txt
-drwxrwxr-x   0 darthbeep  (1000) darthbeep  (1000)        0 2023-04-18 22:44:42.006106 historical_timelines-0.2.2/docs/source/
-drwxrwxr-x   0 darthbeep  (1000) darthbeep  (1000)        0 2023-04-18 22:44:42.006106 historical_timelines-0.2.2/docs/source/_static/
--rw-rw-r--   0 darthbeep  (1000) darthbeep  (1000)    39113 2023-04-18 22:36:14.000000 historical_timelines-0.2.2/docs/source/_static/random_timeline.png
--rw-rw-r--   0 darthbeep  (1000) darthbeep  (1000)     1029 2023-04-18 22:36:14.000000 historical_timelines-0.2.2/docs/source/conf.py
--rw-rw-r--   0 darthbeep  (1000) darthbeep  (1000)      426 2023-04-18 22:36:14.000000 historical_timelines-0.2.2/docs/source/date.rst
--rw-rw-r--   0 darthbeep  (1000) darthbeep  (1000)      441 2023-04-18 22:36:14.000000 historical_timelines-0.2.2/docs/source/event.rst
--rw-rw-r--   0 darthbeep  (1000) darthbeep  (1000)      384 2023-04-18 22:36:14.000000 historical_timelines-0.2.2/docs/source/graphics.rst
--rw-rw-r--   0 darthbeep  (1000) darthbeep  (1000)      384 2023-04-18 22:36:14.000000 historical_timelines-0.2.2/docs/source/index.rst
--rw-rw-r--   0 darthbeep  (1000) darthbeep  (1000)      396 2023-04-18 22:36:14.000000 historical_timelines-0.2.2/docs/source/timeline.rst
-drwxrwxr-x   0 darthbeep  (1000) darthbeep  (1000)        0 2023-04-18 22:44:42.006106 historical_timelines-0.2.2/historical_timelines/
--rw-rw-r--   0 darthbeep  (1000) darthbeep  (1000)      112 2023-04-18 22:42:31.000000 historical_timelines-0.2.2/historical_timelines/__init__.py
--rw-rw-r--   0 darthbeep  (1000) darthbeep  (1000)     4391 2023-03-29 03:29:39.000000 historical_timelines-0.2.2/historical_timelines/date.py
--rw-rw-r--   0 darthbeep  (1000) darthbeep  (1000)     6302 2023-04-18 22:36:14.000000 historical_timelines-0.2.2/historical_timelines/event.py
--rw-rw-r--   0 darthbeep  (1000) darthbeep  (1000)     7437 2023-04-18 22:36:14.000000 historical_timelines-0.2.2/historical_timelines/graphics.py
-drwxrwxr-x   0 darthbeep  (1000) darthbeep  (1000)        0 2023-04-18 22:44:42.010106 historical_timelines-0.2.2/historical_timelines/tests/
--rw-rw-r--   0 darthbeep  (1000) darthbeep  (1000)        0 2023-03-05 02:42:04.000000 historical_timelines-0.2.2/historical_timelines/tests/__init__.py
--rw-rw-r--   0 darthbeep  (1000) darthbeep  (1000)     1053 2023-03-28 21:29:29.000000 historical_timelines-0.2.2/historical_timelines/tests/test_dates.py
--rw-rw-r--   0 darthbeep  (1000) darthbeep  (1000)      986 2023-03-28 21:29:29.000000 historical_timelines-0.2.2/historical_timelines/tests/test_events.py
--rw-rw-r--   0 darthbeep  (1000) darthbeep  (1000)      252 2023-03-28 21:29:29.000000 historical_timelines-0.2.2/historical_timelines/tests/test_graphics.py
--rw-rw-r--   0 darthbeep  (1000) darthbeep  (1000)     3208 2023-03-28 21:29:29.000000 historical_timelines-0.2.2/historical_timelines/tests/test_integration.py
--rw-rw-r--   0 darthbeep  (1000) darthbeep  (1000)      947 2023-03-28 21:29:29.000000 historical_timelines-0.2.2/historical_timelines/tests/test_timelines.py
--rw-rw-r--   0 darthbeep  (1000) darthbeep  (1000)     1967 2023-03-07 23:11:00.000000 historical_timelines-0.2.2/historical_timelines/tests/timeline_egypt.csv
--rw-rw-r--   0 darthbeep  (1000) darthbeep  (1000)     8017 2023-04-18 22:36:14.000000 historical_timelines-0.2.2/historical_timelines/timeline.py
-drwxrwxr-x   0 darthbeep  (1000) darthbeep  (1000)        0 2023-04-18 22:44:42.006106 historical_timelines-0.2.2/historical_timelines.egg-info/
--rw-rw-r--   0 darthbeep  (1000) darthbeep  (1000)     2755 2023-04-18 22:44:41.000000 historical_timelines-0.2.2/historical_timelines.egg-info/PKG-INFO
--rw-rw-r--   0 darthbeep  (1000) darthbeep  (1000)     1134 2023-04-18 22:44:41.000000 historical_timelines-0.2.2/historical_timelines.egg-info/SOURCES.txt
--rw-rw-r--   0 darthbeep  (1000) darthbeep  (1000)        1 2023-04-18 22:44:41.000000 historical_timelines-0.2.2/historical_timelines.egg-info/dependency_links.txt
--rw-rw-r--   0 darthbeep  (1000) darthbeep  (1000)        6 2023-04-18 22:44:41.000000 historical_timelines-0.2.2/historical_timelines.egg-info/requires.txt
--rw-rw-r--   0 darthbeep  (1000) darthbeep  (1000)       21 2023-04-18 22:44:41.000000 historical_timelines-0.2.2/historical_timelines.egg-info/top_level.txt
--rw-rw-r--   0 darthbeep  (1000) darthbeep  (1000)     2247 2023-04-18 22:42:31.000000 historical_timelines-0.2.2/pyproject.toml
--rw-rw-r--   0 darthbeep  (1000) darthbeep  (1000)       38 2023-04-18 22:44:42.010106 historical_timelines-0.2.2/setup.cfg
--rw-rw-r--   0 darthbeep  (1000) darthbeep  (1000)      528 2023-04-18 22:42:31.000000 historical_timelines-0.2.2/setup.py
+drwxrwxr-x   0 darthbeep  (1000) darthbeep  (1000)        0 2023-05-05 03:02:44.830590 historical_timelines-0.2.3/
+-rw-rw-r--   0 darthbeep  (1000) darthbeep  (1000)      409 2023-05-05 02:56:54.000000 historical_timelines-0.2.3/.bumpversion.cfg
+-rw-rw-r--   0 darthbeep  (1000) darthbeep  (1000)      716 2023-04-18 22:36:14.000000 historical_timelines-0.2.3/.readthedocs.yaml
+-rw-rw-r--   0 darthbeep  (1000) darthbeep  (1000)     9826 2023-03-29 03:29:39.000000 historical_timelines-0.2.3/CONTRIBUTING.md
+-rw-rw-r--   0 darthbeep  (1000) darthbeep  (1000)     1066 2023-04-18 22:36:14.000000 historical_timelines-0.2.3/LICENSE
+-rw-rw-r--   0 darthbeep  (1000) darthbeep  (1000)      581 2023-04-18 22:36:14.000000 historical_timelines-0.2.3/MANIFEST.in
+-rw-rw-r--   0 darthbeep  (1000) darthbeep  (1000)     2314 2023-03-08 12:54:50.000000 historical_timelines-0.2.3/Makefile
+-rw-rw-r--   0 darthbeep  (1000) darthbeep  (1000)     3051 2023-05-05 03:02:44.830590 historical_timelines-0.2.3/PKG-INFO
+-rw-rw-r--   0 darthbeep  (1000) darthbeep  (1000)     2758 2023-05-05 02:52:17.000000 historical_timelines-0.2.3/README.md
+drwxrwxr-x   0 darthbeep  (1000) darthbeep  (1000)        0 2023-05-05 03:02:44.826590 historical_timelines-0.2.3/docs/
+-rw-rw-r--   0 darthbeep  (1000) darthbeep  (1000)      638 2023-04-18 22:36:14.000000 historical_timelines-0.2.3/docs/Makefile
+drwxrwxr-x   0 darthbeep  (1000) darthbeep  (1000)        0 2023-05-05 03:02:44.826590 historical_timelines-0.2.3/docs/binder/
+drwxrwxr-x   0 darthbeep  (1000) darthbeep  (1000)        0 2023-05-05 03:02:44.826590 historical_timelines-0.2.3/docs/binder/.ipynb_checkpoints/
+-rw-rw-r--   0 darthbeep  (1000) darthbeep  (1000)    76516 2023-04-19 00:35:40.000000 historical_timelines-0.2.3/docs/binder/.ipynb_checkpoints/tutorial-checkpoint.ipynb
+-rw-rw-r--   0 darthbeep  (1000) darthbeep  (1000)     1967 2023-04-18 22:36:14.000000 historical_timelines-0.2.3/docs/binder/timeline_egypt.csv
+-rw-rw-r--   0 darthbeep  (1000) darthbeep  (1000)    76516 2023-05-05 02:52:17.000000 historical_timelines-0.2.3/docs/binder/tutorial.ipynb
+-rw-rw-r--   0 darthbeep  (1000) darthbeep  (1000)      804 2023-04-18 22:36:14.000000 historical_timelines-0.2.3/docs/make.bat
+-rw-rw-r--   0 darthbeep  (1000) darthbeep  (1000)      173 2023-04-18 22:36:14.000000 historical_timelines-0.2.3/docs/requirements.txt
+drwxrwxr-x   0 darthbeep  (1000) darthbeep  (1000)        0 2023-05-05 03:02:44.826590 historical_timelines-0.2.3/docs/source/
+drwxrwxr-x   0 darthbeep  (1000) darthbeep  (1000)        0 2023-05-05 03:02:44.826590 historical_timelines-0.2.3/docs/source/_static/
+-rw-rw-r--   0 darthbeep  (1000) darthbeep  (1000)    39113 2023-04-18 22:36:14.000000 historical_timelines-0.2.3/docs/source/_static/random_timeline.png
+-rw-rw-r--   0 darthbeep  (1000) darthbeep  (1000)     1029 2023-04-18 22:36:14.000000 historical_timelines-0.2.3/docs/source/conf.py
+-rw-rw-r--   0 darthbeep  (1000) darthbeep  (1000)      426 2023-04-18 22:36:14.000000 historical_timelines-0.2.3/docs/source/date.rst
+-rw-rw-r--   0 darthbeep  (1000) darthbeep  (1000)      441 2023-04-18 22:36:14.000000 historical_timelines-0.2.3/docs/source/event.rst
+-rw-rw-r--   0 darthbeep  (1000) darthbeep  (1000)      384 2023-04-18 22:36:14.000000 historical_timelines-0.2.3/docs/source/graphics.rst
+-rw-rw-r--   0 darthbeep  (1000) darthbeep  (1000)      384 2023-04-18 22:36:14.000000 historical_timelines-0.2.3/docs/source/index.rst
+-rw-rw-r--   0 darthbeep  (1000) darthbeep  (1000)      396 2023-04-18 22:36:14.000000 historical_timelines-0.2.3/docs/source/timeline.rst
+drwxrwxr-x   0 darthbeep  (1000) darthbeep  (1000)        0 2023-05-05 03:02:44.830590 historical_timelines-0.2.3/historical_timelines/
+-rw-rw-r--   0 darthbeep  (1000) darthbeep  (1000)      112 2023-05-05 02:56:54.000000 historical_timelines-0.2.3/historical_timelines/__init__.py
+-rw-rw-r--   0 darthbeep  (1000) darthbeep  (1000)     4391 2023-03-29 03:29:39.000000 historical_timelines-0.2.3/historical_timelines/date.py
+-rw-rw-r--   0 darthbeep  (1000) darthbeep  (1000)     6302 2023-04-18 22:36:14.000000 historical_timelines-0.2.3/historical_timelines/event.py
+-rw-rw-r--   0 darthbeep  (1000) darthbeep  (1000)     7437 2023-04-18 22:36:14.000000 historical_timelines-0.2.3/historical_timelines/graphics.py
+drwxrwxr-x   0 darthbeep  (1000) darthbeep  (1000)        0 2023-05-05 03:02:44.830590 historical_timelines-0.2.3/historical_timelines/tests/
+-rw-rw-r--   0 darthbeep  (1000) darthbeep  (1000)        0 2023-03-05 02:42:04.000000 historical_timelines-0.2.3/historical_timelines/tests/__init__.py
+-rw-rw-r--   0 darthbeep  (1000) darthbeep  (1000)     1053 2023-03-28 21:29:29.000000 historical_timelines-0.2.3/historical_timelines/tests/test_dates.py
+-rw-rw-r--   0 darthbeep  (1000) darthbeep  (1000)      986 2023-03-28 21:29:29.000000 historical_timelines-0.2.3/historical_timelines/tests/test_events.py
+-rw-rw-r--   0 darthbeep  (1000) darthbeep  (1000)      252 2023-03-28 21:29:29.000000 historical_timelines-0.2.3/historical_timelines/tests/test_graphics.py
+-rw-rw-r--   0 darthbeep  (1000) darthbeep  (1000)     3208 2023-03-28 21:29:29.000000 historical_timelines-0.2.3/historical_timelines/tests/test_integration.py
+-rw-rw-r--   0 darthbeep  (1000) darthbeep  (1000)      947 2023-03-28 21:29:29.000000 historical_timelines-0.2.3/historical_timelines/tests/test_timelines.py
+-rw-rw-r--   0 darthbeep  (1000) darthbeep  (1000)     1967 2023-03-07 23:11:00.000000 historical_timelines-0.2.3/historical_timelines/tests/timeline_egypt.csv
+-rw-rw-r--   0 darthbeep  (1000) darthbeep  (1000)     8353 2023-05-05 02:52:17.000000 historical_timelines-0.2.3/historical_timelines/timeline.py
+drwxrwxr-x   0 darthbeep  (1000) darthbeep  (1000)        0 2023-05-05 03:02:44.830590 historical_timelines-0.2.3/historical_timelines.egg-info/
+-rw-rw-r--   0 darthbeep  (1000) darthbeep  (1000)     3051 2023-05-05 03:02:44.000000 historical_timelines-0.2.3/historical_timelines.egg-info/PKG-INFO
+-rw-rw-r--   0 darthbeep  (1000) darthbeep  (1000)     1134 2023-05-05 03:02:44.000000 historical_timelines-0.2.3/historical_timelines.egg-info/SOURCES.txt
+-rw-rw-r--   0 darthbeep  (1000) darthbeep  (1000)        1 2023-05-05 03:02:44.000000 historical_timelines-0.2.3/historical_timelines.egg-info/dependency_links.txt
+-rw-rw-r--   0 darthbeep  (1000) darthbeep  (1000)        6 2023-05-05 03:02:44.000000 historical_timelines-0.2.3/historical_timelines.egg-info/requires.txt
+-rw-rw-r--   0 darthbeep  (1000) darthbeep  (1000)       21 2023-05-05 03:02:44.000000 historical_timelines-0.2.3/historical_timelines.egg-info/top_level.txt
+-rw-rw-r--   0 darthbeep  (1000) darthbeep  (1000)     2247 2023-05-05 02:56:54.000000 historical_timelines-0.2.3/pyproject.toml
+-rw-rw-r--   0 darthbeep  (1000) darthbeep  (1000)       38 2023-05-05 03:02:44.830590 historical_timelines-0.2.3/setup.cfg
+-rw-rw-r--   0 darthbeep  (1000) darthbeep  (1000)      528 2023-05-05 02:56:54.000000 historical_timelines-0.2.3/setup.py
```

### Comparing `historical_timelines-0.2.2/.readthedocs.yaml` & `historical_timelines-0.2.3/.readthedocs.yaml`

 * *Files identical despite different names*

### Comparing `historical_timelines-0.2.2/CONTRIBUTING.md` & `historical_timelines-0.2.3/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `historical_timelines-0.2.2/LICENSE` & `historical_timelines-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `historical_timelines-0.2.2/MANIFEST.in` & `historical_timelines-0.2.3/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `historical_timelines-0.2.2/Makefile` & `historical_timelines-0.2.3/Makefile`

 * *Files identical despite different names*

### Comparing `historical_timelines-0.2.2/PKG-INFO` & `historical_timelines-0.2.3/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: historical_timelines
-Version: 0.2.2
+Version: 0.2.3
 Summary: A Python package for making historical timelines
 Home-page: UNKNOWN
 Author: darthbeep
 Author-email: darthbeep@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
@@ -15,14 +15,15 @@
 
 [![Build Status](https://github.com/darthbeep/historical-timelines/workflows/Build%20Status/badge.svg?branch=main)](https://github.com/darthbeep/historical-timelines/actions)
 [![codecov](https://codecov.io/gh/darthbeep/historical-timelines/branch/main/graph/badge.svg)](https://codecov.io/gh/darthbeep/historical-timelines)
 [![license: MIT](https://img.shields.io/badge/license-MIT-blue.svg)](https://opensource.org/licenses/MIT)
 [![GitHub issues](https://img.shields.io/github/issues/darthbeep/historical-timelines)](https://github.com/darthbeep/historical-timelines/issues)
 [![PyPI](https://img.shields.io/pypi/v/historical_timelines)](https://pypi.org/project/historical-timelines/)
 [![Documentation Status](https://readthedocs.org/projects/historical-timelines/badge/?version=latest)](https://historical-timelines.readthedocs.io/en/latest/?badge=latest)
+[![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/darthbeep/historical-timelines/HEAD?labpath=docs%2Fbinder%2Ftutorial.ipynb)
 
 ## Overview
 
 historical-timelines is a python package for creating nice looking timelines, specifically with historical data in mind. historical-timelines uses [bokeh](https://bokeh.org/) to create images.
 
 ## Install
 
@@ -69,7 +70,9 @@
 timeline.render_timeline("timeline.html")
 ```
 
 ## Documentation
 
 The documentation can be found [here](https://historical-timelines.readthedocs.io/en/latest/).
 
+A jupyter tutorial can be found [here](https://mybinder.org/v2/gh/darthbeep/historical-timelines/HEAD?labpath=docs%2Fbinder%2Ftutorial.ipynb).
+
```

### Comparing `historical_timelines-0.2.2/README.md` & `historical_timelines-0.2.3/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 
 [![Build Status](https://github.com/darthbeep/historical-timelines/workflows/Build%20Status/badge.svg?branch=main)](https://github.com/darthbeep/historical-timelines/actions)
 [![codecov](https://codecov.io/gh/darthbeep/historical-timelines/branch/main/graph/badge.svg)](https://codecov.io/gh/darthbeep/historical-timelines)
 [![license: MIT](https://img.shields.io/badge/license-MIT-blue.svg)](https://opensource.org/licenses/MIT)
 [![GitHub issues](https://img.shields.io/github/issues/darthbeep/historical-timelines)](https://github.com/darthbeep/historical-timelines/issues)
 [![PyPI](https://img.shields.io/pypi/v/historical_timelines)](https://pypi.org/project/historical-timelines/)
 [![Documentation Status](https://readthedocs.org/projects/historical-timelines/badge/?version=latest)](https://historical-timelines.readthedocs.io/en/latest/?badge=latest)
+[![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/darthbeep/historical-timelines/HEAD?labpath=docs%2Fbinder%2Ftutorial.ipynb)
 
 ## Overview
 
 historical-timelines is a python package for creating nice looking timelines, specifically with historical data in mind. historical-timelines uses [bokeh](https://bokeh.org/) to create images.
 
 ## Install
 
@@ -55,8 +56,10 @@
 
 timeline.populate_timeline_from_dict(timeline_json)
 timeline.render_timeline("timeline.html")
 ```
 
 ## Documentation
 
-The documentation can be found [here](https://historical-timelines.readthedocs.io/en/latest/).
+The documentation can be found [here](https://historical-timelines.readthedocs.io/en/latest/).
+
+A jupyter tutorial can be found [here](https://mybinder.org/v2/gh/darthbeep/historical-timelines/HEAD?labpath=docs%2Fbinder%2Ftutorial.ipynb).
```

### Comparing `historical_timelines-0.2.2/docs/Makefile` & `historical_timelines-0.2.3/docs/Makefile`

 * *Files identical despite different names*

### Comparing `historical_timelines-0.2.2/docs/binder/timeline_egypt.csv` & `historical_timelines-0.2.3/docs/binder/timeline_egypt.csv`

 * *Files identical despite different names*

### Comparing `historical_timelines-0.2.2/docs/make.bat` & `historical_timelines-0.2.3/docs/make.bat`

 * *Files identical despite different names*

### Comparing `historical_timelines-0.2.2/docs/source/_static/random_timeline.png` & `historical_timelines-0.2.3/docs/source/_static/random_timeline.png`

 * *Files identical despite different names*

### Comparing `historical_timelines-0.2.2/docs/source/conf.py` & `historical_timelines-0.2.3/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `historical_timelines-0.2.2/historical_timelines/date.py` & `historical_timelines-0.2.3/historical_timelines/date.py`

 * *Files identical despite different names*

### Comparing `historical_timelines-0.2.2/historical_timelines/event.py` & `historical_timelines-0.2.3/historical_timelines/event.py`

 * *Files identical despite different names*

### Comparing `historical_timelines-0.2.2/historical_timelines/graphics.py` & `historical_timelines-0.2.3/historical_timelines/graphics.py`

 * *Files identical despite different names*

### Comparing `historical_timelines-0.2.2/historical_timelines/tests/test_dates.py` & `historical_timelines-0.2.3/historical_timelines/tests/test_dates.py`

 * *Files identical despite different names*

### Comparing `historical_timelines-0.2.2/historical_timelines/tests/test_events.py` & `historical_timelines-0.2.3/historical_timelines/tests/test_events.py`

 * *Files identical despite different names*

### Comparing `historical_timelines-0.2.2/historical_timelines/tests/test_integration.py` & `historical_timelines-0.2.3/historical_timelines/tests/test_integration.py`

 * *Files identical despite different names*

### Comparing `historical_timelines-0.2.2/historical_timelines/tests/test_timelines.py` & `historical_timelines-0.2.3/historical_timelines/tests/test_timelines.py`

 * *Files identical despite different names*

### Comparing `historical_timelines-0.2.2/historical_timelines/tests/timeline_egypt.csv` & `historical_timelines-0.2.3/historical_timelines/tests/timeline_egypt.csv`

 * *Files identical despite different names*

### Comparing `historical_timelines-0.2.2/historical_timelines/timeline.py` & `historical_timelines-0.2.3/historical_timelines/timeline.py`

 * *Files 6% similar despite different names*

```diff
@@ -117,38 +117,44 @@
         for _ in range(N):
             events.append(HistoricalEvent.get_random_event())
         self.add_events(events)
 
         if sort:
             self.sort()
 
-    def create_event_dict(self) -> dict[str, list]:
+    def create_event_dict(self, label_max_line_width: int = 10) -> dict[str, list]:
         """Create a dictionary that describes events to help with graphics
 
+        Args:
+            label_max_line_width (int, optional): The maximum line width for labels. Defaults to 10.
+
         Returns:
             dict[str, list]: An event dict for the graphics generator
         """
         dates = []
         titles = []
         descriptions = []
         labels = []
 
         for event in self.events:
             dates.append(event.get_adjusted_year())
-            titles.append(event.get_title_with_newlines())
+            titles.append(event.get_title_with_newlines(label_max_line_width))
             descriptions.append(event.description)
             labels.append(event.get_label_or_default())
 
         event_dict = {"dates": dates, "title": titles, "description": descriptions, "label": labels}
 
         return event_dict
 
-    def create_period_list(self) -> list[dict]:
+    def create_period_list(self, label_max_line_width: int = 10) -> list[dict]:
         """Create a list of periods that can be turned into a timeline image
 
+        Args:
+            label_max_line_width (int, optional): The maximum line width for labels. Defaults to 10.
+
         Returns:
             list[dict]: A list of dictionaries that can be turned into a timeline image
         """
         period_list = []
         period_groups = self.collision_sort()
         for period_group in period_groups:
             starts = []
@@ -159,15 +165,15 @@
             labels = []
 
             for event in period_group:
                 start, end = event.get_adjusted_year()
                 starts.append(start)
                 ends.append(end)
                 mids.append((start + end) / 2)
-                titles.append(event.get_title_with_newlines())
+                titles.append(event.get_title_with_newlines(label_max_line_width))
                 descriptions.append(event.description)
                 labels.append(event.label)
 
             event_dict = {
                 "start": starts,
                 "end": ends,
                 "mid": mids,
```

### Comparing `historical_timelines-0.2.2/historical_timelines.egg-info/PKG-INFO` & `historical_timelines-0.2.3/historical_timelines.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: historical-timelines
-Version: 0.2.2
+Version: 0.2.3
 Summary: A Python package for making historical timelines
 Home-page: UNKNOWN
 Author: darthbeep
 Author-email: darthbeep@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
@@ -15,14 +15,15 @@
 
 [![Build Status](https://github.com/darthbeep/historical-timelines/workflows/Build%20Status/badge.svg?branch=main)](https://github.com/darthbeep/historical-timelines/actions)
 [![codecov](https://codecov.io/gh/darthbeep/historical-timelines/branch/main/graph/badge.svg)](https://codecov.io/gh/darthbeep/historical-timelines)
 [![license: MIT](https://img.shields.io/badge/license-MIT-blue.svg)](https://opensource.org/licenses/MIT)
 [![GitHub issues](https://img.shields.io/github/issues/darthbeep/historical-timelines)](https://github.com/darthbeep/historical-timelines/issues)
 [![PyPI](https://img.shields.io/pypi/v/historical_timelines)](https://pypi.org/project/historical-timelines/)
 [![Documentation Status](https://readthedocs.org/projects/historical-timelines/badge/?version=latest)](https://historical-timelines.readthedocs.io/en/latest/?badge=latest)
+[![Binder](https://mybinder.org/badge_logo.svg)](https://mybinder.org/v2/gh/darthbeep/historical-timelines/HEAD?labpath=docs%2Fbinder%2Ftutorial.ipynb)
 
 ## Overview
 
 historical-timelines is a python package for creating nice looking timelines, specifically with historical data in mind. historical-timelines uses [bokeh](https://bokeh.org/) to create images.
 
 ## Install
 
@@ -69,7 +70,9 @@
 timeline.render_timeline("timeline.html")
 ```
 
 ## Documentation
 
 The documentation can be found [here](https://historical-timelines.readthedocs.io/en/latest/).
 
+A jupyter tutorial can be found [here](https://mybinder.org/v2/gh/darthbeep/historical-timelines/HEAD?labpath=docs%2Fbinder%2Ftutorial.ipynb).
+
```

### Comparing `historical_timelines-0.2.2/historical_timelines.egg-info/SOURCES.txt` & `historical_timelines-0.2.3/historical_timelines.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `historical_timelines-0.2.2/pyproject.toml` & `historical_timelines-0.2.3/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 build-backend="setuptools.build_meta"
 
 [project]
 name = "historical-timelines"
 authors = [{name = "darthbeep", email = "darthbeep@gmail.com"}]
 description="A python project to make historical timelines"
 readme = "README.md"
-version = "0.2.2"
+version = "0.2.3"
 requires-python = ">=3.7"
 
 dependencies = [
     "bokeh >= 3.1.0"
 ]
 
 classifiers = [
```

### Comparing `historical_timelines-0.2.2/setup.py` & `historical_timelines-0.2.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from pathlib import Path
 
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(
     name='historical_timelines',
-    version='0.2.2',
+    version='0.2.3',
     description='A Python package for making historical timelines',
     long_description=long_description,
     long_description_content_type='text/markdown',
     author='darthbeep',
     author_email='darthbeep@gmail.com',
     packages=['historical_timelines'],
     install_requires=[
```

