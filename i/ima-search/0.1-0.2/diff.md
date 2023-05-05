# Comparing `tmp/ima-search-0.1.tar.gz` & `tmp/ima-search-0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ima-search-0.1.tar", last modified: Fri May  5 17:23:31 2023, max compression
+gzip compressed data, was "ima-search-0.2.tar", last modified: Fri May  5 19:13:10 2023, max compression
```

## Comparing `ima-search-0.1.tar` & `ima-search-0.2.tar`

### file list

```diff
@@ -1,55 +1,57 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 17:23:31.957846 ima-search-0.1/
--rw-r--r--   0 runner    (1001) docker     (123)      586 2023-05-05 17:23:17.000000 ima-search-0.1/.coveragerc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 17:23:31.949845 ima-search-0.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 17:23:31.953845 ima-search-0.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1300 2023-05-05 17:23:17.000000 ima-search-0.1/.github/workflows/python-package.yml
--rw-r--r--   0 runner    (1001) docker     (123)      653 2023-05-05 17:23:17.000000 ima-search-0.1/.github/workflows/python-publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)      566 2023-05-05 17:23:17.000000 ima-search-0.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-05-05 17:23:17.000000 ima-search-0.1/AUTHORS.md
--rw-r--r--   0 runner    (1001) docker     (123)      128 2023-05-05 17:23:17.000000 ima-search-0.1/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)    32473 2023-05-05 17:23:17.000000 ima-search-0.1/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1621 2023-05-05 17:23:31.957846 ima-search-0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1156 2023-05-05 17:23:17.000000 ima-search-0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 17:23:31.953845 ima-search-0.1/bin/
--rw-r--r--   0 runner    (1001) docker     (123)      185 2023-05-05 17:23:17.000000 ima-search-0.1/bin/ima
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 17:23:31.953845 ima-search-0.1/docs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 17:23:31.953845 ima-search-0.1/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-05 17:23:17.000000 ima-search-0.1/docs/_static/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     2403 2023-05-05 17:23:17.000000 ima-search-0.1/docs/image.md
--rw-r--r--   0 runner    (1001) docker     (123)      238 2023-05-05 17:23:17.000000 ima-search-0.1/docs/introduction.md
--rw-r--r--   0 runner    (1001) docker     (123)     2069 2023-05-05 17:23:17.000000 ima-search-0.1/docs/search.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 17:23:31.953845 ima-search-0.1/man/
--rw-r--r--   0 runner    (1001) docker     (123)     4536 2023-05-05 17:23:17.000000 ima-search-0.1/man/ima.1
--rw-r--r--   0 runner    (1001) docker     (123)      346 2023-05-05 17:23:17.000000 ima-search-0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-05-05 17:23:17.000000 ima-search-0.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1177 2023-05-05 17:23:31.957846 ima-search-0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      698 2023-05-05 17:23:17.000000 ima-search-0.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 17:23:31.949845 ima-search-0.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 17:23:31.953845 ima-search-0.1/src/ima/
--rw-r--r--   0 runner    (1001) docker     (123)     9972 2023-05-05 17:23:17.000000 ima-search-0.1/src/ima/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      300 2023-05-05 17:23:17.000000 ima-search-0.1/src/ima/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      397 2023-05-05 17:23:17.000000 ima-search-0.1/src/ima/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     4802 2023-05-05 17:23:17.000000 ima-search-0.1/src/ima/image.py
--rw-r--r--   0 runner    (1001) docker     (123)     6170 2023-05-05 17:23:17.000000 ima-search-0.1/src/ima/options.py
--rw-r--r--   0 runner    (1001) docker     (123)    11207 2023-05-05 17:23:17.000000 ima-search-0.1/src/ima/search.py
--rw-r--r--   0 runner    (1001) docker     (123)    47090 2023-05-05 17:23:17.000000 ima-search-0.1/src/ima/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)       68 2023-05-05 17:23:17.000000 ima-search-0.1/src/ima/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 17:23:31.953845 ima-search-0.1/src/ima_search.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1621 2023-05-05 17:23:31.000000 ima-search-0.1/src/ima_search.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      827 2023-05-05 17:23:31.000000 ima-search-0.1/src/ima_search.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 17:23:31.000000 ima-search-0.1/src/ima_search.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 17:23:31.000000 ima-search-0.1/src/ima_search.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-05-05 17:23:31.000000 ima-search-0.1/src/ima_search.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-05-05 17:23:31.000000 ima-search-0.1/src/ima_search.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 17:23:31.953845 ima-search-0.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      311 2023-05-05 17:23:17.000000 ima-search-0.1/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 17:23:17.000000 ima-search-0.1/tests/test_image.py
--rw-r--r--   0 runner    (1001) docker     (123)      824 2023-05-05 17:23:17.000000 ima-search-0.1/tests/test_search.py
--rw-r--r--   0 runner    (1001) docker     (123)     2851 2023-05-05 17:23:17.000000 ima-search-0.1/tox.ini
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 17:23:31.957846 ima-search-0.1/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      319 2023-05-05 17:23:17.000000 ima-search-0.1/utils/body.md
--rw-r--r--   0 runner    (1001) docker     (123)      630 2023-05-05 17:23:17.000000 ima-search-0.1/utils/examples.md
--rw-r--r--   0 runner    (1001) docker     (123)       95 2023-05-05 17:23:17.000000 ima-search-0.1/utils/heading.md
--rw-r--r--   0 runner    (1001) docker     (123)       95 2023-05-05 17:23:17.000000 ima-search-0.1/utils/issues.md
--rw-r--r--   0 runner    (1001) docker     (123)       92 2023-05-05 17:23:17.000000 ima-search-0.1/utils/license.md
--rwxr-xr-x   0 runner    (1001) docker     (123)     2464 2023-05-05 17:23:17.000000 ima-search-0.1/utils/manit.pl
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 19:13:10.484748 ima-search-0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)      586 2023-05-05 19:12:57.000000 ima-search-0.2/.coveragerc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 19:13:10.476748 ima-search-0.2/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 19:13:10.476748 ima-search-0.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1375 2023-05-05 19:12:57.000000 ima-search-0.2/.github/workflows/python-package.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      653 2023-05-05 19:12:57.000000 ima-search-0.2/.github/workflows/python-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      566 2023-05-05 19:12:57.000000 ima-search-0.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-05-05 19:12:57.000000 ima-search-0.2/AUTHORS.md
+-rw-r--r--   0 runner    (1001) docker     (123)      128 2023-05-05 19:12:57.000000 ima-search-0.2/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)    32473 2023-05-05 19:12:57.000000 ima-search-0.2/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3651 2023-05-05 19:12:57.000000 ima-search-0.2/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     1611 2023-05-05 19:13:10.484748 ima-search-0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1162 2023-05-05 19:12:57.000000 ima-search-0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 19:13:10.476748 ima-search-0.2/bin/
+-rw-r--r--   0 runner    (1001) docker     (123)      185 2023-05-05 19:12:57.000000 ima-search-0.2/bin/ima
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 19:13:10.480748 ima-search-0.2/docs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 19:13:10.480748 ima-search-0.2/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-05 19:12:57.000000 ima-search-0.2/docs/_static/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     2403 2023-05-05 19:12:57.000000 ima-search-0.2/docs/image.md
+-rw-r--r--   0 runner    (1001) docker     (123)      238 2023-05-05 19:12:57.000000 ima-search-0.2/docs/introduction.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2069 2023-05-05 19:12:57.000000 ima-search-0.2/docs/search.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 19:13:10.480748 ima-search-0.2/man/
+-rw-r--r--   0 runner    (1001) docker     (123)     4536 2023-05-05 19:12:57.000000 ima-search-0.2/man/ima.1
+-rw-r--r--   0 runner    (1001) docker     (123)      346 2023-05-05 19:12:57.000000 ima-search-0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-05-05 19:12:57.000000 ima-search-0.2/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1196 2023-05-05 19:13:10.484748 ima-search-0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      698 2023-05-05 19:12:57.000000 ima-search-0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 19:13:10.476748 ima-search-0.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 19:13:10.480748 ima-search-0.2/src/ima/
+-rw-r--r--   0 runner    (1001) docker     (123)     9972 2023-05-05 19:12:57.000000 ima-search-0.2/src/ima/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      300 2023-05-05 19:12:57.000000 ima-search-0.2/src/ima/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      397 2023-05-05 19:12:57.000000 ima-search-0.2/src/ima/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4802 2023-05-05 19:12:57.000000 ima-search-0.2/src/ima/image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6170 2023-05-05 19:12:57.000000 ima-search-0.2/src/ima/options.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11207 2023-05-05 19:12:57.000000 ima-search-0.2/src/ima/search.py
+-rw-r--r--   0 runner    (1001) docker     (123)    47090 2023-05-05 19:12:57.000000 ima-search-0.2/src/ima/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)       68 2023-05-05 19:12:57.000000 ima-search-0.2/src/ima/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 19:13:10.480748 ima-search-0.2/src/ima_search.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1611 2023-05-05 19:13:10.000000 ima-search-0.2/src/ima_search.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      877 2023-05-05 19:13:10.000000 ima-search-0.2/src/ima_search.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 19:13:10.000000 ima-search-0.2/src/ima_search.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-05-05 19:13:10.000000 ima-search-0.2/src/ima_search.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 19:13:10.000000 ima-search-0.2/src/ima_search.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-05-05 19:13:10.000000 ima-search-0.2/src/ima_search.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-05-05 19:13:10.000000 ima-search-0.2/src/ima_search.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 19:13:10.480748 ima-search-0.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      311 2023-05-05 19:12:57.000000 ima-search-0.2/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 19:12:57.000000 ima-search-0.2/tests/test_image.py
+-rw-r--r--   0 runner    (1001) docker     (123)      824 2023-05-05 19:12:57.000000 ima-search-0.2/tests/test_search.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2851 2023-05-05 19:12:57.000000 ima-search-0.2/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 19:13:10.484748 ima-search-0.2/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      319 2023-05-05 19:12:57.000000 ima-search-0.2/utils/body.md
+-rw-r--r--   0 runner    (1001) docker     (123)      630 2023-05-05 19:12:57.000000 ima-search-0.2/utils/examples.md
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-05-05 19:12:57.000000 ima-search-0.2/utils/heading.md
+-rw-r--r--   0 runner    (1001) docker     (123)       95 2023-05-05 19:12:57.000000 ima-search-0.2/utils/issues.md
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-05-05 19:12:57.000000 ima-search-0.2/utils/license.md
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2464 2023-05-05 19:12:57.000000 ima-search-0.2/utils/manit.pl
```

### Comparing `ima-search-0.1/.coveragerc` & `ima-search-0.2/.coveragerc`

 * *Files identical despite different names*

### Comparing `ima-search-0.1/.github/workflows/python-package.yml` & `ima-search-0.2/.github/workflows/python-package.yml`

 * *Files 12% similar despite different names*

```diff
@@ -9,14 +9,17 @@
   pull_request:
     branches: [ "main" ]
 
 jobs:
   build:
 
     runs-on: ubuntu-latest
+    environment:
+      name: pypi
+      url: https://pypi.org/p/ima-search
     strategy:
       fail-fast: false
       matrix:
         python-version: ["3.9", "3.10"]
 
     steps:
     - uses: actions/checkout@v3
```

### Comparing `ima-search-0.1/.github/workflows/python-publish.yml` & `ima-search-0.2/.github/workflows/python-publish.yml`

 * *Files identical despite different names*

### Comparing `ima-search-0.1/.gitignore` & `ima-search-0.2/.gitignore`

 * *Files identical despite different names*

### Comparing `ima-search-0.1/LICENSE.txt` & `ima-search-0.2/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `ima-search-0.1/PKG-INFO` & `ima-search-0.2/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: ima-search
-Version: 0.1
-Summary: Query for and download images on the internet
+Version: 0.2
+Summary: Image searcher and downloader
 Home-page: https://github.com/tcheukueppo/ima/
 Author: tcheukueppo
 Author-email: tcheukueppo@tutanota.com
 License: GPL-3.0-only
 Platform: any
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python
@@ -17,36 +17,36 @@
 
 https://user-images.githubusercontent.com/90014847/235641562-67a09617-c1b6-4438-a38c-d1533326a43c.mp4
 
 
 ima
 ===
 
-Query with search engines and download images
+Image searcher and downloader
 
 - [Introduction](https://github.com/tcheukueppo/ima#Introduction)
 - [Installation](https://github.com/tcheukueppo/ima#Installation)
 - [Documentation](https://github.com/tcheukueppo/ima#Documentation)
 - [License](https://github.com/tcheukueppo/ima#License)
 - [Authors](https://github.com/tcheukueppo/ima#Authors)
 
-ima is an extremely tiny command line utility which permits you to query search engines(e.g DuckDuckGo)
+ima is an extremely tiny python library command line utility which permits you to query search engines(e.g DuckDuckGo)
 and download images from web pages.
 
 ima might be a utility of choice for the following purpose:
 
 - Downloading images from the internet to build up your dataset
 - Searching on the internet with Google, DuckDuckGo or Yahoo. You would want to
   use multiple search engines to obtain better results.
 - Caching your search results to later on use them locally.
 
 # Installation
 
 ```{python}
-pip install ima
+pip install ima-search
 ```
 
 # Documentation
 
 Read the documentation from [here](./docs/introduction.md)
 
 # License
```

### Comparing `ima-search-0.1/README.md` & `ima-search-0.2/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 
 https://user-images.githubusercontent.com/90014847/235641562-67a09617-c1b6-4438-a38c-d1533326a43c.mp4
 
 
 ima
 ===
 
-Query with search engines and download images
+Image searcher and downloader
 
 - [Introduction](https://github.com/tcheukueppo/ima#Introduction)
 - [Installation](https://github.com/tcheukueppo/ima#Installation)
 - [Documentation](https://github.com/tcheukueppo/ima#Documentation)
 - [License](https://github.com/tcheukueppo/ima#License)
 - [Authors](https://github.com/tcheukueppo/ima#Authors)
 
-ima is an extremely tiny command line utility which permits you to query search engines(e.g DuckDuckGo)
+ima is an extremely tiny python library command line utility which permits you to query search engines(e.g DuckDuckGo)
 and download images from web pages.
 
 ima might be a utility of choice for the following purpose:
 
 - Downloading images from the internet to build up your dataset
 - Searching on the internet with Google, DuckDuckGo or Yahoo. You would want to
   use multiple search engines to obtain better results.
 - Caching your search results to later on use them locally.
 
 # Installation
 
 ```{python}
-pip install ima
+pip install ima-search
 ```
 
 # Documentation
 
 Read the documentation from [here](./docs/introduction.md)
 
 # License
```

### Comparing `ima-search-0.1/docs/image.md` & `ima-search-0.2/docs/image.md`

 * *Files identical despite different names*

### Comparing `ima-search-0.1/docs/search.md` & `ima-search-0.2/docs/search.md`

 * *Files identical despite different names*

### Comparing `ima-search-0.1/man/ima.1` & `ima-search-0.2/man/ima.1`

 * *Files identical despite different names*

### Comparing `ima-search-0.1/setup.cfg` & `ima-search-0.2/setup.cfg`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = ima-search
-description = Query for and download images on the internet
+description = Image searcher and downloader
 author = tcheukueppo
 author_email = tcheukueppo@tutanota.com
 license = GPL-3.0-only
 license_files = LICENSE.txt
 long_description = file: README.md
 long_description_content_type = text/markdown; charset=UTF-8
 url = https://github.com/tcheukueppo/ima/
@@ -35,14 +35,16 @@
 [options.extras_require]
 testing = 
 	setuptools
 	pytest
 	pytest-cov
 
 [options.entry_points]
+console_scripts = 
+	ima = ima:main
 
 [tool:pytest]
 addopts = 
 	--cov ima --cov-report term-missing
 	--verbose
 norecursedirs = 
 	dist
```

### Comparing `ima-search-0.1/setup.py` & `ima-search-0.2/setup.py`

 * *Files identical despite different names*

### Comparing `ima-search-0.1/src/ima/__init__.py` & `ima-search-0.2/src/ima/__init__.py`

 * *Files identical despite different names*

### Comparing `ima-search-0.1/src/ima/image.py` & `ima-search-0.2/src/ima/image.py`

 * *Files identical despite different names*

### Comparing `ima-search-0.1/src/ima/options.py` & `ima-search-0.2/src/ima/options.py`

 * *Files identical despite different names*

### Comparing `ima-search-0.1/src/ima/search.py` & `ima-search-0.2/src/ima/search.py`

 * *Files identical despite different names*

### Comparing `ima-search-0.1/src/ima/utils.py` & `ima-search-0.2/src/ima/utils.py`

 * *Files identical despite different names*

### Comparing `ima-search-0.1/src/ima_search.egg-info/PKG-INFO` & `ima-search-0.2/src/ima_search.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: ima-search
-Version: 0.1
-Summary: Query for and download images on the internet
+Version: 0.2
+Summary: Image searcher and downloader
 Home-page: https://github.com/tcheukueppo/ima/
 Author: tcheukueppo
 Author-email: tcheukueppo@tutanota.com
 License: GPL-3.0-only
 Platform: any
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python
@@ -17,36 +17,36 @@
 
 https://user-images.githubusercontent.com/90014847/235641562-67a09617-c1b6-4438-a38c-d1533326a43c.mp4
 
 
 ima
 ===
 
-Query with search engines and download images
+Image searcher and downloader
 
 - [Introduction](https://github.com/tcheukueppo/ima#Introduction)
 - [Installation](https://github.com/tcheukueppo/ima#Installation)
 - [Documentation](https://github.com/tcheukueppo/ima#Documentation)
 - [License](https://github.com/tcheukueppo/ima#License)
 - [Authors](https://github.com/tcheukueppo/ima#Authors)
 
-ima is an extremely tiny command line utility which permits you to query search engines(e.g DuckDuckGo)
+ima is an extremely tiny python library command line utility which permits you to query search engines(e.g DuckDuckGo)
 and download images from web pages.
 
 ima might be a utility of choice for the following purpose:
 
 - Downloading images from the internet to build up your dataset
 - Searching on the internet with Google, DuckDuckGo or Yahoo. You would want to
   use multiple search engines to obtain better results.
 - Caching your search results to later on use them locally.
 
 # Installation
 
 ```{python}
-pip install ima
+pip install ima-search
 ```
 
 # Documentation
 
 Read the documentation from [here](./docs/introduction.md)
 
 # License
```

### Comparing `ima-search-0.1/src/ima_search.egg-info/SOURCES.txt` & `ima-search-0.2/src/ima_search.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 .coveragerc
 .gitignore
 AUTHORS.md
 CHANGELOG.md
 LICENSE.txt
+Makefile
 README.md
 pyproject.toml
 requirements.txt
 setup.cfg
 setup.py
 tox.ini
 .github/workflows/python-package.yml
@@ -24,14 +25,15 @@
 src/ima/options.py
 src/ima/search.py
 src/ima/utils.py
 src/ima/version.py
 src/ima_search.egg-info/PKG-INFO
 src/ima_search.egg-info/SOURCES.txt
 src/ima_search.egg-info/dependency_links.txt
+src/ima_search.egg-info/entry_points.txt
 src/ima_search.egg-info/not-zip-safe
 src/ima_search.egg-info/requires.txt
 src/ima_search.egg-info/top_level.txt
 tests/conftest.py
 tests/test_image.py
 tests/test_search.py
 utils/body.md
```

### Comparing `ima-search-0.1/tests/test_search.py` & `ima-search-0.2/tests/test_search.py`

 * *Files identical despite different names*

### Comparing `ima-search-0.1/tox.ini` & `ima-search-0.2/tox.ini`

 * *Files identical despite different names*

### Comparing `ima-search-0.1/utils/examples.md` & `ima-search-0.2/utils/examples.md`

 * *Files identical despite different names*

### Comparing `ima-search-0.1/utils/manit.pl` & `ima-search-0.2/utils/manit.pl`

 * *Files identical despite different names*

