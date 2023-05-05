# Comparing `tmp/birdhouse-birdy-0.8.2.tar.gz` & `tmp/birdhouse-birdy-0.8.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "birdhouse-birdy-0.8.2.tar", last modified: Wed May  3 12:15:09 2023, max compression
+gzip compressed data, was "birdhouse-birdy-0.8.3.tar", last modified: Fri May  5 15:06:37 2023, max compression
```

## Comparing `birdhouse-birdy-0.8.2.tar` & `birdhouse-birdy-0.8.3.tar`

### file list

```diff
@@ -1,56 +1,56 @@
-drwxr-xr-x   0 pingu      (501) staff       (20)        0 2023-05-03 12:15:09.527940 birdhouse-birdy-0.8.2/
--rw-r--r--   0 pingu      (501) staff       (20)      221 2023-05-03 12:11:31.000000 birdhouse-birdy-0.8.2/AUTHORS.rst
--rw-r--r--   0 pingu      (501) staff       (20)     6489 2023-05-03 12:11:31.000000 birdhouse-birdy-0.8.2/CHANGES.rst
--rw-r--r--   0 pingu      (501) staff       (20)    11358 2023-05-03 12:11:31.000000 birdhouse-birdy-0.8.2/LICENSE.txt
--rw-r--r--   0 pingu      (501) staff       (20)      183 2023-05-03 12:11:31.000000 birdhouse-birdy-0.8.2/MANIFEST.in
--rw-r--r--   0 pingu      (501) staff       (20)     9468 2023-05-03 12:15:09.528091 birdhouse-birdy-0.8.2/PKG-INFO
--rw-r--r--   0 pingu      (501) staff       (20)     1904 2023-05-03 12:11:31.000000 birdhouse-birdy-0.8.2/README.rst
-drwxr-xr-x   0 pingu      (501) staff       (20)        0 2023-05-03 12:15:09.514851 birdhouse-birdy-0.8.2/birdhouse_birdy.egg-info/
--rw-r--r--   0 pingu      (501) staff       (20)     9468 2023-05-03 12:15:09.000000 birdhouse-birdy-0.8.2/birdhouse_birdy.egg-info/PKG-INFO
--rw-r--r--   0 pingu      (501) staff       (20)     1132 2023-05-03 12:15:09.000000 birdhouse-birdy-0.8.2/birdhouse_birdy.egg-info/SOURCES.txt
--rw-r--r--   0 pingu      (501) staff       (20)        1 2023-05-03 12:15:09.000000 birdhouse-birdy-0.8.2/birdhouse_birdy.egg-info/dependency_links.txt
--rw-r--r--   0 pingu      (501) staff       (20)       44 2023-05-03 12:15:09.000000 birdhouse-birdy-0.8.2/birdhouse_birdy.egg-info/entry_points.txt
--rw-r--r--   0 pingu      (501) staff       (20)      337 2023-05-03 12:15:09.000000 birdhouse-birdy-0.8.2/birdhouse_birdy.egg-info/requires.txt
--rw-r--r--   0 pingu      (501) staff       (20)       12 2023-05-03 12:15:09.000000 birdhouse-birdy-0.8.2/birdhouse_birdy.egg-info/top_level.txt
-drwxr-xr-x   0 pingu      (501) staff       (20)        0 2023-05-03 12:15:09.517108 birdhouse-birdy-0.8.2/birdy/
--rw-r--r--   0 pingu      (501) staff       (20)      192 2023-05-03 12:11:31.000000 birdhouse-birdy-0.8.2/birdy/__init__.py
-drwxr-xr-x   0 pingu      (501) staff       (20)        0 2023-05-03 12:15:09.519562 birdhouse-birdy-0.8.2/birdy/cli/
--rw-r--r--   0 pingu      (501) staff       (20)     2729 2023-05-03 12:11:31.000000 birdhouse-birdy-0.8.2/birdy/cli/__init__.py
--rw-r--r--   0 pingu      (501) staff       (20)     4941 2023-05-03 12:11:31.000000 birdhouse-birdy-0.8.2/birdy/cli/base.py
--rw-r--r--   0 pingu      (501) staff       (20)     1102 2023-05-03 12:11:31.000000 birdhouse-birdy-0.8.2/birdy/cli/misc.py
--rw-r--r--   0 pingu      (501) staff       (20)     2093 2023-05-03 12:11:31.000000 birdhouse-birdy-0.8.2/birdy/cli/run.py
--rw-r--r--   0 pingu      (501) staff       (20)      548 2023-05-03 12:11:31.000000 birdhouse-birdy-0.8.2/birdy/cli/types.py
-drwxr-xr-x   0 pingu      (501) staff       (20)        0 2023-05-03 12:15:09.521661 birdhouse-birdy-0.8.2/birdy/client/
--rw-r--r--   0 pingu      (501) staff       (20)     4734 2023-05-03 12:11:31.000000 birdhouse-birdy-0.8.2/birdy/client/__init__.py
--rw-r--r--   0 pingu      (501) staff       (20)    15876 2023-05-03 12:11:31.000000 birdhouse-birdy-0.8.2/birdy/client/base.py
--rw-r--r--   0 pingu      (501) staff       (20)    10685 2023-05-03 12:11:31.000000 birdhouse-birdy-0.8.2/birdy/client/converters.py
--rw-r--r--   0 pingu      (501) staff       (20)     9424 2023-05-03 12:11:31.000000 birdhouse-birdy-0.8.2/birdy/client/notebook.py
--rw-r--r--   0 pingu      (501) staff       (20)     2354 2023-05-03 12:11:31.000000 birdhouse-birdy-0.8.2/birdy/client/outputs.py
--rw-r--r--   0 pingu      (501) staff       (20)     9699 2023-05-03 12:11:31.000000 birdhouse-birdy-0.8.2/birdy/client/utils.py
--rw-r--r--   0 pingu      (501) staff       (20)      954 2023-05-03 12:11:31.000000 birdhouse-birdy-0.8.2/birdy/dependencies.py
--rw-r--r--   0 pingu      (501) staff       (20)      450 2023-05-03 12:11:31.000000 birdhouse-birdy-0.8.2/birdy/exceptions.py
-drwxr-xr-x   0 pingu      (501) staff       (20)        0 2023-05-03 12:15:09.522730 birdhouse-birdy-0.8.2/birdy/ipyleafletwfs/
--rw-r--r--   0 pingu      (501) staff       (20)     1092 2023-05-03 12:11:31.000000 birdhouse-birdy-0.8.2/birdy/ipyleafletwfs/README.md
--rw-r--r--   0 pingu      (501) staff       (20)       60 2023-05-03 12:11:31.000000 birdhouse-birdy-0.8.2/birdy/ipyleafletwfs/__init__.py
--rw-r--r--   0 pingu      (501) staff       (20)    15076 2023-05-03 12:11:31.000000 birdhouse-birdy-0.8.2/birdy/ipyleafletwfs/base.py
-drwxr-xr-x   0 pingu      (501) staff       (20)        0 2023-05-03 12:15:09.524036 birdhouse-birdy-0.8.2/birdy/ipyleafletwfs/examples/
--rw-r--r--   0 pingu      (501) staff       (20)     6092 2023-05-03 12:11:31.000000 birdhouse-birdy-0.8.2/birdy/ipyleafletwfs/examples/ipyleafletwfs_guide.ipynb
--rw-r--r--   0 pingu      (501) staff       (20)     1832 2023-05-03 12:11:31.000000 birdhouse-birdy-0.8.2/birdy/ipyleafletwfs/examples/quickstart-template.ipynb
--rw-r--r--   0 pingu      (501) staff       (20)     3037 2023-05-03 12:11:31.000000 birdhouse-birdy-0.8.2/birdy/ipyleafletwfs/examples/wfs_constructor.ipynb
-drwxr-xr-x   0 pingu      (501) staff       (20)        0 2023-05-03 12:15:09.524372 birdhouse-birdy-0.8.2/birdy/templates/
--rw-r--r--   0 pingu      (501) staff       (20)     3173 2023-05-03 12:11:31.000000 birdhouse-birdy-0.8.2/birdy/templates/cmd.py.j2
--rw-r--r--   0 pingu      (501) staff       (20)     5856 2023-05-03 12:11:31.000000 birdhouse-birdy-0.8.2/birdy/utils.py
--rw-r--r--   0 pingu      (501) staff       (20)       81 2023-05-03 12:11:31.000000 birdhouse-birdy-0.8.2/requirements.txt
--rw-r--r--   0 pingu      (501) staff       (20)      249 2023-05-03 12:11:31.000000 birdhouse-birdy-0.8.2/requirements_dev.txt
--rw-r--r--   0 pingu      (501) staff       (20)       82 2023-05-03 12:11:31.000000 birdhouse-birdy-0.8.2/requirements_extra.txt
--rw-r--r--   0 pingu      (501) staff       (20)      852 2023-05-03 12:15:09.528883 birdhouse-birdy-0.8.2/setup.cfg
--rw-r--r--   0 pingu      (501) staff       (20)     2139 2023-05-03 12:11:31.000000 birdhouse-birdy-0.8.2/setup.py
-drwxr-xr-x   0 pingu      (501) staff       (20)        0 2023-05-03 12:15:09.527662 birdhouse-birdy-0.8.2/tests/
--rw-r--r--   0 pingu      (501) staff       (20)       13 2023-05-03 12:11:31.000000 birdhouse-birdy-0.8.2/tests/__init__.py
--rw-r--r--   0 pingu      (501) staff       (20)      489 2023-05-03 12:11:31.000000 birdhouse-birdy-0.8.2/tests/common.py
--rw-r--r--   0 pingu      (501) staff       (20)     1413 2023-05-03 12:11:31.000000 birdhouse-birdy-0.8.2/tests/test_cli.py
--rw-r--r--   0 pingu      (501) staff       (20)    11959 2023-05-03 12:11:31.000000 birdhouse-birdy-0.8.2/tests/test_client.py
--rw-r--r--   0 pingu      (501) staff       (20)     2208 2023-05-03 12:11:31.000000 birdhouse-birdy-0.8.2/tests/test_converters.py
--rw-r--r--   0 pingu      (501) staff       (20)      180 2023-05-03 12:11:31.000000 birdhouse-birdy-0.8.2/tests/test_dependencies.py
--rw-r--r--   0 pingu      (501) staff       (20)      162 2023-05-03 12:11:31.000000 birdhouse-birdy-0.8.2/tests/test_notebook.py
--rw-r--r--   0 pingu      (501) staff       (20)     4521 2023-05-03 12:11:31.000000 birdhouse-birdy-0.8.2/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 15:06:37.506090 birdhouse-birdy-0.8.3/
+-rw-r--r--   0 runner    (1001) docker     (123)      221 2023-05-05 15:06:34.000000 birdhouse-birdy-0.8.3/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     6600 2023-05-05 15:06:34.000000 birdhouse-birdy-0.8.3/CHANGES.rst
+-rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-05-05 15:06:34.000000 birdhouse-birdy-0.8.3/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      183 2023-05-05 15:06:34.000000 birdhouse-birdy-0.8.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     9959 2023-05-05 15:06:37.506090 birdhouse-birdy-0.8.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2284 2023-05-05 15:06:34.000000 birdhouse-birdy-0.8.3/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 15:06:37.502090 birdhouse-birdy-0.8.3/birdhouse_birdy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     9959 2023-05-05 15:06:37.000000 birdhouse-birdy-0.8.3/birdhouse_birdy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1132 2023-05-05 15:06:37.000000 birdhouse-birdy-0.8.3/birdhouse_birdy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 15:06:37.000000 birdhouse-birdy-0.8.3/birdhouse_birdy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-05-05 15:06:37.000000 birdhouse-birdy-0.8.3/birdhouse_birdy.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      359 2023-05-05 15:06:37.000000 birdhouse-birdy-0.8.3/birdhouse_birdy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-05 15:06:37.000000 birdhouse-birdy-0.8.3/birdhouse_birdy.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 15:06:37.502090 birdhouse-birdy-0.8.3/birdy/
+-rw-r--r--   0 runner    (1001) docker     (123)      192 2023-05-05 15:06:34.000000 birdhouse-birdy-0.8.3/birdy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 15:06:37.502090 birdhouse-birdy-0.8.3/birdy/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)     2729 2023-05-05 15:06:34.000000 birdhouse-birdy-0.8.3/birdy/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4941 2023-05-05 15:06:34.000000 birdhouse-birdy-0.8.3/birdy/cli/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1102 2023-05-05 15:06:34.000000 birdhouse-birdy-0.8.3/birdy/cli/misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2093 2023-05-05 15:06:34.000000 birdhouse-birdy-0.8.3/birdy/cli/run.py
+-rw-r--r--   0 runner    (1001) docker     (123)      548 2023-05-05 15:06:34.000000 birdhouse-birdy-0.8.3/birdy/cli/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 15:06:37.502090 birdhouse-birdy-0.8.3/birdy/client/
+-rw-r--r--   0 runner    (1001) docker     (123)     4734 2023-05-05 15:06:34.000000 birdhouse-birdy-0.8.3/birdy/client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15876 2023-05-05 15:06:34.000000 birdhouse-birdy-0.8.3/birdy/client/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10685 2023-05-05 15:06:34.000000 birdhouse-birdy-0.8.3/birdy/client/converters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9424 2023-05-05 15:06:34.000000 birdhouse-birdy-0.8.3/birdy/client/notebook.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2354 2023-05-05 15:06:34.000000 birdhouse-birdy-0.8.3/birdy/client/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9699 2023-05-05 15:06:34.000000 birdhouse-birdy-0.8.3/birdy/client/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      954 2023-05-05 15:06:34.000000 birdhouse-birdy-0.8.3/birdy/dependencies.py
+-rw-r--r--   0 runner    (1001) docker     (123)      450 2023-05-05 15:06:34.000000 birdhouse-birdy-0.8.3/birdy/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 15:06:37.502090 birdhouse-birdy-0.8.3/birdy/ipyleafletwfs/
+-rw-r--r--   0 runner    (1001) docker     (123)     1092 2023-05-05 15:06:34.000000 birdhouse-birdy-0.8.3/birdy/ipyleafletwfs/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-05-05 15:06:34.000000 birdhouse-birdy-0.8.3/birdy/ipyleafletwfs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15076 2023-05-05 15:06:34.000000 birdhouse-birdy-0.8.3/birdy/ipyleafletwfs/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 15:06:37.502090 birdhouse-birdy-0.8.3/birdy/ipyleafletwfs/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)     6092 2023-05-05 15:06:34.000000 birdhouse-birdy-0.8.3/birdy/ipyleafletwfs/examples/ipyleafletwfs_guide.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     1832 2023-05-05 15:06:34.000000 birdhouse-birdy-0.8.3/birdy/ipyleafletwfs/examples/quickstart-template.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)     3037 2023-05-05 15:06:34.000000 birdhouse-birdy-0.8.3/birdy/ipyleafletwfs/examples/wfs_constructor.ipynb
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 15:06:37.502090 birdhouse-birdy-0.8.3/birdy/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)     3173 2023-05-05 15:06:34.000000 birdhouse-birdy-0.8.3/birdy/templates/cmd.py.j2
+-rw-r--r--   0 runner    (1001) docker     (123)     5856 2023-05-05 15:06:34.000000 birdhouse-birdy-0.8.3/birdy/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-05-05 15:06:34.000000 birdhouse-birdy-0.8.3/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      249 2023-05-05 15:06:34.000000 birdhouse-birdy-0.8.3/requirements_dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-05-05 15:06:34.000000 birdhouse-birdy-0.8.3/requirements_extra.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      856 2023-05-05 15:06:37.506090 birdhouse-birdy-0.8.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2139 2023-05-05 15:06:34.000000 birdhouse-birdy-0.8.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 15:06:37.506090 birdhouse-birdy-0.8.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-05 15:06:34.000000 birdhouse-birdy-0.8.3/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      489 2023-05-05 15:06:34.000000 birdhouse-birdy-0.8.3/tests/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1413 2023-05-05 15:06:34.000000 birdhouse-birdy-0.8.3/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11959 2023-05-05 15:06:34.000000 birdhouse-birdy-0.8.3/tests/test_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2208 2023-05-05 15:06:34.000000 birdhouse-birdy-0.8.3/tests/test_converters.py
+-rw-r--r--   0 runner    (1001) docker     (123)      180 2023-05-05 15:06:34.000000 birdhouse-birdy-0.8.3/tests/test_dependencies.py
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-05-05 15:06:34.000000 birdhouse-birdy-0.8.3/tests/test_notebook.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4521 2023-05-05 15:06:34.000000 birdhouse-birdy-0.8.3/tests/test_utils.py
```

### Comparing `birdhouse-birdy-0.8.2/CHANGES.rst` & `birdhouse-birdy-0.8.3/CHANGES.rst`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,17 @@
 Change History
 **************
 
+0.8.3 (2023-05-03)
+==================
+
+Changes:
+
+* Added the `packaging` library to the list of requirements.
+
 0.8.2 (2023-04-28)
 ==================
 
 Changes:
 
 * Relax dependency check on GeoTiff rioxarray and rasterio converters due to some mysterious gdal error.
 * Remove tests with live 52North WPS server since it seems offline.
```

### Comparing `birdhouse-birdy-0.8.2/LICENSE.txt` & `birdhouse-birdy-0.8.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `birdhouse-birdy-0.8.2/PKG-INFO` & `birdhouse-birdy-0.8.3/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: birdhouse-birdy
-Version: 0.8.2
+Version: 0.8.3
 Summary: Birdy provides a command-line tool to work with Web Processing Services.
 Home-page: https://github.com/bird-house/birdy
 Author: Carsten Ehbrecht
 Author-email: ehbrecht@dkrz.de
 License: Apache License v2.0
 Keywords: wps pywps owslib geopython birdy birdhouse
 Classifier: Development Status :: 4 - Beta
@@ -21,73 +21,89 @@
 License-File: LICENSE.txt
 License-File: AUTHORS.rst
 
 =====
 Birdy
 =====
 
-.. image:: https://img.shields.io/badge/docs-latest-brightgreen.svg
-   :target: http://birdy.readthedocs.io/en/latest/?badge=latest
-   :alt: Documentation Status
-
-.. image:: https://github.com/bird-house/birdy/workflows/build/badge.svg
-    :target: https://github.com/bird-house/birdy/actions
-    :alt: Build Status
-
-.. image:: https://api.codacy.com/project/badge/Grade/da14405a9a6d4c2e9c405d9c0c8babe7
-   :target: https://www.codacy.com/app/cehbrecht/birdy?utm_source=github.com&amp;utm_medium=referral&amp;utm_content=bird-house/birdy&amp;utm_campaign=Badge_Grade
-   :alt: Codacy Code Checks
-
-.. image:: https://img.shields.io/github/license/bird-house/birdy.svg
-   :target: https://github.com/bird-house/birdy/blob/master/LICENSE.txt
-   :alt: GitHub license
-
-.. image:: https://badges.gitter.im/bird-house/birdhouse.svg
-   :target: https://gitter.im/bird-house/birdhouse?utm_source=badge&utm_medium=badge&utm_campaign=pr-badge&utm_content=badge
-   :alt: Join the chat at https://gitter.im/bird-house/birdhouse
-
+|PyPI| |Docs| |Build| |Codacy| |License| |Gitter|
 
 Birdy (the bird)
    *Birdy is not a bird but likes to play with them.*
 
 Birdy is a Python library to work with Web Processing Services (WPS).
 It is using `OWSLib` from the `GeoPython` project.
 
 You can try Birdy online using Binder (just click on the binder link below),
 or view the notebooks on NBViewer.
 
-.. image:: https://mybinder.org/badge_logo.svg
-   :target: https://mybinder.org/v2/gh/bird-house/birdy.git/v0.8.2?filepath=notebooks
-   :alt: Binder Launcher
-
-.. image:: https://raw.githubusercontent.com/jupyter/design/master/logos/Badges/nbviewer_badge.svg
-   :target: https://nbviewer.jupyter.org/github/bird-house/birdy/tree/v0.8.2/notebooks/
-   :alt: NBViewer
-   :height: 20
+|Binder|
+
+|NBViewer|
 
 Birdy is part of the `Birdhouse`_ project.
 
 Full `documentation <http://birdy.readthedocs.org/en/latest/>`_ is on ReadTheDocs.
 
 .. _Birdhouse: http://bird-house.github.io/en/latest/
 
+.. |PyPI| image:: https://img.shields.io/pypi/v/birdhouse-birdy.svg
+        :target: https://pypi.python.org/pypi/birdhouse-birdy
+        :alt: Python Package Index Build
+
+.. |Docs| image:: https://img.shields.io/badge/docs-latest-brightgreen.svg
+        :target: http://birdy.readthedocs.io/en/latest/?badge=latest
+        :alt: Documentation Status
+
+.. |Build| image:: https://github.com/bird-house/birdy/workflows/build/badge.svg
+        :target: https://github.com/bird-house/birdy/actions
+        :alt: Build Status
+
+.. |Codacy| image:: https://api.codacy.com/project/badge/Grade/da14405a9a6d4c2e9c405d9c0c8babe7
+        :target: https://www.codacy.com/app/cehbrecht/birdy?utm_source=github.com&amp;utm_medium=referral&amp;utm_content=bird-house/birdy&amp;utm_campaign=Badge_Grade
+        :alt: Codacy Code Checks
+
+.. |License| image:: https://img.shields.io/github/license/bird-house/birdy.svg
+        :target: https://github.com/bird-house/birdy/blob/master/LICENSE.txt
+        :alt: GitHub license
+
+.. |Gitter| image:: https://badges.gitter.im/bird-house/birdhouse.svg
+        :target: https://gitter.im/bird-house/birdhouse?utm_source=badge&utm_medium=badge&utm_campaign=pr-badge&utm_content=badge
+        :alt: Join the chat at https://gitter.im/bird-house/birdhouse
+
+.. |Binder| image:: https://mybinder.org/badge_logo.svg
+        :target: https://mybinder.org/v2/gh/bird-house/birdy.git/v0.8.3?filepath=notebooks
+        :alt: Binder Launcher
+
+.. |NBViewer| image:: https://raw.githubusercontent.com/jupyter/design/master/logos/Badges/nbviewer_badge.svg
+        :target: https://nbviewer.jupyter.org/github/bird-house/birdy/tree/v0.8.3/notebooks/
+        :alt: NBViewer
+        :height: 20
+
 Authors
 *******
 
 * David Huard <huard.david@ouranos.ca>
 * Carsten Ehbrecht <ehbrecht@dkrz.de>
 
 Contributors
 ************
 
 * Trevor James Smith <smith.trevorj@ouranos.ca> `@Zeitsperre <https://www.github.com/Zeitsperre>`_
 
 Change History
 **************
 
+0.8.3 (2023-05-03)
+==================
+
+Changes:
+
+* Added the `packaging` library to the list of requirements.
+
 0.8.2 (2023-04-28)
 ==================
 
 Changes:
 
 * Relax dependency check on GeoTiff rioxarray and rasterio converters due to some mysterious gdal error.
 * Remove tests with live 52North WPS server since it seems offline.
```

### Comparing `birdhouse-birdy-0.8.2/README.rst` & `birdhouse-birdy-0.8.3/README.rst`

 * *Files 23% similar despite different names*

```diff
@@ -1,48 +1,57 @@
 =====
 Birdy
 =====
 
-.. image:: https://img.shields.io/badge/docs-latest-brightgreen.svg
-   :target: http://birdy.readthedocs.io/en/latest/?badge=latest
-   :alt: Documentation Status
-
-.. image:: https://github.com/bird-house/birdy/workflows/build/badge.svg
-    :target: https://github.com/bird-house/birdy/actions
-    :alt: Build Status
-
-.. image:: https://api.codacy.com/project/badge/Grade/da14405a9a6d4c2e9c405d9c0c8babe7
-   :target: https://www.codacy.com/app/cehbrecht/birdy?utm_source=github.com&amp;utm_medium=referral&amp;utm_content=bird-house/birdy&amp;utm_campaign=Badge_Grade
-   :alt: Codacy Code Checks
-
-.. image:: https://img.shields.io/github/license/bird-house/birdy.svg
-   :target: https://github.com/bird-house/birdy/blob/master/LICENSE.txt
-   :alt: GitHub license
-
-.. image:: https://badges.gitter.im/bird-house/birdhouse.svg
-   :target: https://gitter.im/bird-house/birdhouse?utm_source=badge&utm_medium=badge&utm_campaign=pr-badge&utm_content=badge
-   :alt: Join the chat at https://gitter.im/bird-house/birdhouse
-
+|PyPI| |Docs| |Build| |Codacy| |License| |Gitter|
 
 Birdy (the bird)
    *Birdy is not a bird but likes to play with them.*
 
 Birdy is a Python library to work with Web Processing Services (WPS).
 It is using `OWSLib` from the `GeoPython` project.
 
 You can try Birdy online using Binder (just click on the binder link below),
 or view the notebooks on NBViewer.
 
-.. image:: https://mybinder.org/badge_logo.svg
-   :target: https://mybinder.org/v2/gh/bird-house/birdy.git/v0.8.2?filepath=notebooks
-   :alt: Binder Launcher
-
-.. image:: https://raw.githubusercontent.com/jupyter/design/master/logos/Badges/nbviewer_badge.svg
-   :target: https://nbviewer.jupyter.org/github/bird-house/birdy/tree/v0.8.2/notebooks/
-   :alt: NBViewer
-   :height: 20
+|Binder|
+
+|NBViewer|
 
 Birdy is part of the `Birdhouse`_ project.
 
 Full `documentation <http://birdy.readthedocs.org/en/latest/>`_ is on ReadTheDocs.
 
 .. _Birdhouse: http://bird-house.github.io/en/latest/
+
+.. |PyPI| image:: https://img.shields.io/pypi/v/birdhouse-birdy.svg
+        :target: https://pypi.python.org/pypi/birdhouse-birdy
+        :alt: Python Package Index Build
+
+.. |Docs| image:: https://img.shields.io/badge/docs-latest-brightgreen.svg
+        :target: http://birdy.readthedocs.io/en/latest/?badge=latest
+        :alt: Documentation Status
+
+.. |Build| image:: https://github.com/bird-house/birdy/workflows/build/badge.svg
+        :target: https://github.com/bird-house/birdy/actions
+        :alt: Build Status
+
+.. |Codacy| image:: https://api.codacy.com/project/badge/Grade/da14405a9a6d4c2e9c405d9c0c8babe7
+        :target: https://www.codacy.com/app/cehbrecht/birdy?utm_source=github.com&amp;utm_medium=referral&amp;utm_content=bird-house/birdy&amp;utm_campaign=Badge_Grade
+        :alt: Codacy Code Checks
+
+.. |License| image:: https://img.shields.io/github/license/bird-house/birdy.svg
+        :target: https://github.com/bird-house/birdy/blob/master/LICENSE.txt
+        :alt: GitHub license
+
+.. |Gitter| image:: https://badges.gitter.im/bird-house/birdhouse.svg
+        :target: https://gitter.im/bird-house/birdhouse?utm_source=badge&utm_medium=badge&utm_campaign=pr-badge&utm_content=badge
+        :alt: Join the chat at https://gitter.im/bird-house/birdhouse
+
+.. |Binder| image:: https://mybinder.org/badge_logo.svg
+        :target: https://mybinder.org/v2/gh/bird-house/birdy.git/v0.8.3?filepath=notebooks
+        :alt: Binder Launcher
+
+.. |NBViewer| image:: https://raw.githubusercontent.com/jupyter/design/master/logos/Badges/nbviewer_badge.svg
+        :target: https://nbviewer.jupyter.org/github/bird-house/birdy/tree/v0.8.3/notebooks/
+        :alt: NBViewer
+        :height: 20
```

### Comparing `birdhouse-birdy-0.8.2/birdhouse_birdy.egg-info/PKG-INFO` & `birdhouse-birdy-0.8.3/birdhouse_birdy.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: birdhouse-birdy
-Version: 0.8.2
+Version: 0.8.3
 Summary: Birdy provides a command-line tool to work with Web Processing Services.
 Home-page: https://github.com/bird-house/birdy
 Author: Carsten Ehbrecht
 Author-email: ehbrecht@dkrz.de
 License: Apache License v2.0
 Keywords: wps pywps owslib geopython birdy birdhouse
 Classifier: Development Status :: 4 - Beta
@@ -21,73 +21,89 @@
 License-File: LICENSE.txt
 License-File: AUTHORS.rst
 
 =====
 Birdy
 =====
 
-.. image:: https://img.shields.io/badge/docs-latest-brightgreen.svg
-   :target: http://birdy.readthedocs.io/en/latest/?badge=latest
-   :alt: Documentation Status
-
-.. image:: https://github.com/bird-house/birdy/workflows/build/badge.svg
-    :target: https://github.com/bird-house/birdy/actions
-    :alt: Build Status
-
-.. image:: https://api.codacy.com/project/badge/Grade/da14405a9a6d4c2e9c405d9c0c8babe7
-   :target: https://www.codacy.com/app/cehbrecht/birdy?utm_source=github.com&amp;utm_medium=referral&amp;utm_content=bird-house/birdy&amp;utm_campaign=Badge_Grade
-   :alt: Codacy Code Checks
-
-.. image:: https://img.shields.io/github/license/bird-house/birdy.svg
-   :target: https://github.com/bird-house/birdy/blob/master/LICENSE.txt
-   :alt: GitHub license
-
-.. image:: https://badges.gitter.im/bird-house/birdhouse.svg
-   :target: https://gitter.im/bird-house/birdhouse?utm_source=badge&utm_medium=badge&utm_campaign=pr-badge&utm_content=badge
-   :alt: Join the chat at https://gitter.im/bird-house/birdhouse
-
+|PyPI| |Docs| |Build| |Codacy| |License| |Gitter|
 
 Birdy (the bird)
    *Birdy is not a bird but likes to play with them.*
 
 Birdy is a Python library to work with Web Processing Services (WPS).
 It is using `OWSLib` from the `GeoPython` project.
 
 You can try Birdy online using Binder (just click on the binder link below),
 or view the notebooks on NBViewer.
 
-.. image:: https://mybinder.org/badge_logo.svg
-   :target: https://mybinder.org/v2/gh/bird-house/birdy.git/v0.8.2?filepath=notebooks
-   :alt: Binder Launcher
-
-.. image:: https://raw.githubusercontent.com/jupyter/design/master/logos/Badges/nbviewer_badge.svg
-   :target: https://nbviewer.jupyter.org/github/bird-house/birdy/tree/v0.8.2/notebooks/
-   :alt: NBViewer
-   :height: 20
+|Binder|
+
+|NBViewer|
 
 Birdy is part of the `Birdhouse`_ project.
 
 Full `documentation <http://birdy.readthedocs.org/en/latest/>`_ is on ReadTheDocs.
 
 .. _Birdhouse: http://bird-house.github.io/en/latest/
 
+.. |PyPI| image:: https://img.shields.io/pypi/v/birdhouse-birdy.svg
+        :target: https://pypi.python.org/pypi/birdhouse-birdy
+        :alt: Python Package Index Build
+
+.. |Docs| image:: https://img.shields.io/badge/docs-latest-brightgreen.svg
+        :target: http://birdy.readthedocs.io/en/latest/?badge=latest
+        :alt: Documentation Status
+
+.. |Build| image:: https://github.com/bird-house/birdy/workflows/build/badge.svg
+        :target: https://github.com/bird-house/birdy/actions
+        :alt: Build Status
+
+.. |Codacy| image:: https://api.codacy.com/project/badge/Grade/da14405a9a6d4c2e9c405d9c0c8babe7
+        :target: https://www.codacy.com/app/cehbrecht/birdy?utm_source=github.com&amp;utm_medium=referral&amp;utm_content=bird-house/birdy&amp;utm_campaign=Badge_Grade
+        :alt: Codacy Code Checks
+
+.. |License| image:: https://img.shields.io/github/license/bird-house/birdy.svg
+        :target: https://github.com/bird-house/birdy/blob/master/LICENSE.txt
+        :alt: GitHub license
+
+.. |Gitter| image:: https://badges.gitter.im/bird-house/birdhouse.svg
+        :target: https://gitter.im/bird-house/birdhouse?utm_source=badge&utm_medium=badge&utm_campaign=pr-badge&utm_content=badge
+        :alt: Join the chat at https://gitter.im/bird-house/birdhouse
+
+.. |Binder| image:: https://mybinder.org/badge_logo.svg
+        :target: https://mybinder.org/v2/gh/bird-house/birdy.git/v0.8.3?filepath=notebooks
+        :alt: Binder Launcher
+
+.. |NBViewer| image:: https://raw.githubusercontent.com/jupyter/design/master/logos/Badges/nbviewer_badge.svg
+        :target: https://nbviewer.jupyter.org/github/bird-house/birdy/tree/v0.8.3/notebooks/
+        :alt: NBViewer
+        :height: 20
+
 Authors
 *******
 
 * David Huard <huard.david@ouranos.ca>
 * Carsten Ehbrecht <ehbrecht@dkrz.de>
 
 Contributors
 ************
 
 * Trevor James Smith <smith.trevorj@ouranos.ca> `@Zeitsperre <https://www.github.com/Zeitsperre>`_
 
 Change History
 **************
 
+0.8.3 (2023-05-03)
+==================
+
+Changes:
+
+* Added the `packaging` library to the list of requirements.
+
 0.8.2 (2023-04-28)
 ==================
 
 Changes:
 
 * Relax dependency check on GeoTiff rioxarray and rasterio converters due to some mysterious gdal error.
 * Remove tests with live 52North WPS server since it seems offline.
```

### Comparing `birdhouse-birdy-0.8.2/birdhouse_birdy.egg-info/SOURCES.txt` & `birdhouse-birdy-0.8.3/birdhouse_birdy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `birdhouse-birdy-0.8.2/birdy/cli/__init__.py` & `birdhouse-birdy-0.8.3/birdy/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `birdhouse-birdy-0.8.2/birdy/cli/base.py` & `birdhouse-birdy-0.8.3/birdy/cli/base.py`

 * *Files identical despite different names*

### Comparing `birdhouse-birdy-0.8.2/birdy/cli/misc.py` & `birdhouse-birdy-0.8.3/birdy/cli/misc.py`

 * *Files identical despite different names*

### Comparing `birdhouse-birdy-0.8.2/birdy/cli/run.py` & `birdhouse-birdy-0.8.3/birdy/cli/run.py`

 * *Files identical despite different names*

### Comparing `birdhouse-birdy-0.8.2/birdy/cli/types.py` & `birdhouse-birdy-0.8.3/birdy/cli/types.py`

 * *Files identical despite different names*

### Comparing `birdhouse-birdy-0.8.2/birdy/client/__init__.py` & `birdhouse-birdy-0.8.3/birdy/client/__init__.py`

 * *Files identical despite different names*

### Comparing `birdhouse-birdy-0.8.2/birdy/client/base.py` & `birdhouse-birdy-0.8.3/birdy/client/base.py`

 * *Files identical despite different names*

### Comparing `birdhouse-birdy-0.8.2/birdy/client/converters.py` & `birdhouse-birdy-0.8.3/birdy/client/converters.py`

 * *Files identical despite different names*

### Comparing `birdhouse-birdy-0.8.2/birdy/client/notebook.py` & `birdhouse-birdy-0.8.3/birdy/client/notebook.py`

 * *Files identical despite different names*

### Comparing `birdhouse-birdy-0.8.2/birdy/client/outputs.py` & `birdhouse-birdy-0.8.3/birdy/client/outputs.py`

 * *Files identical despite different names*

### Comparing `birdhouse-birdy-0.8.2/birdy/client/utils.py` & `birdhouse-birdy-0.8.3/birdy/client/utils.py`

 * *Files identical despite different names*

### Comparing `birdhouse-birdy-0.8.2/birdy/dependencies.py` & `birdhouse-birdy-0.8.3/birdy/dependencies.py`

 * *Files identical despite different names*

### Comparing `birdhouse-birdy-0.8.2/birdy/ipyleafletwfs/README.md` & `birdhouse-birdy-0.8.3/birdy/ipyleafletwfs/README.md`

 * *Files identical despite different names*

### Comparing `birdhouse-birdy-0.8.2/birdy/ipyleafletwfs/base.py` & `birdhouse-birdy-0.8.3/birdy/ipyleafletwfs/base.py`

 * *Files identical despite different names*

### Comparing `birdhouse-birdy-0.8.2/birdy/ipyleafletwfs/examples/ipyleafletwfs_guide.ipynb` & `birdhouse-birdy-0.8.3/birdy/ipyleafletwfs/examples/ipyleafletwfs_guide.ipynb`

 * *Files identical despite different names*

### Comparing `birdhouse-birdy-0.8.2/birdy/ipyleafletwfs/examples/quickstart-template.ipynb` & `birdhouse-birdy-0.8.3/birdy/ipyleafletwfs/examples/quickstart-template.ipynb`

 * *Files identical despite different names*

### Comparing `birdhouse-birdy-0.8.2/birdy/ipyleafletwfs/examples/wfs_constructor.ipynb` & `birdhouse-birdy-0.8.3/birdy/ipyleafletwfs/examples/wfs_constructor.ipynb`

 * *Files identical despite different names*

### Comparing `birdhouse-birdy-0.8.2/birdy/templates/cmd.py.j2` & `birdhouse-birdy-0.8.3/birdy/templates/cmd.py.j2`

 * *Files identical despite different names*

### Comparing `birdhouse-birdy-0.8.2/birdy/utils.py` & `birdhouse-birdy-0.8.3/birdy/utils.py`

 * *Files identical despite different names*

### Comparing `birdhouse-birdy-0.8.2/setup.cfg` & `birdhouse-birdy-0.8.3/setup.cfg`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 [bumpversion]
-current_version = 0.8.2
+current_version = 0.8.3
 commit = True
-tag = True
+tag = False
 
 [metadata]
 description-file = README.rst
 
 [bumpversion:file:birdy/__init__.py]
 search = __version__ = "{current_version}"
 replace = __version__ = "{new_version}"
@@ -17,15 +17,17 @@
 [bumpversion:file:README.rst]
 search = {current_version}
 replace = {new_version}
 
 [tool:pytest]
 python_files = test_*.py
 testpaths = tests
-addopts = --strict --tb=native
+addopts = 
+	--strict
+	--tb=native
 markers = 
 	online: mark test to need internet connection
 	slow: mark test to be slow
 
 [flake8]
 max-line-length = 120
 exclude =
```

### Comparing `birdhouse-birdy-0.8.2/setup.py` & `birdhouse-birdy-0.8.3/setup.py`

 * *Files identical despite different names*

### Comparing `birdhouse-birdy-0.8.2/tests/test_cli.py` & `birdhouse-birdy-0.8.3/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `birdhouse-birdy-0.8.2/tests/test_client.py` & `birdhouse-birdy-0.8.3/tests/test_client.py`

 * *Files identical despite different names*

### Comparing `birdhouse-birdy-0.8.2/tests/test_converters.py` & `birdhouse-birdy-0.8.3/tests/test_converters.py`

 * *Files identical despite different names*

### Comparing `birdhouse-birdy-0.8.2/tests/test_utils.py` & `birdhouse-birdy-0.8.3/tests/test_utils.py`

 * *Files identical despite different names*

