# Comparing `tmp/cellmaps_utils-0.1.0a1.tar.gz` & `tmp/cellmaps_utils-0.1.0a2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/cellmaps_utils-0.1.0a1.tar", last modified: Mon May  1 21:47:56 2023, max compression
+gzip compressed data, was "dist/cellmaps_utils-0.1.0a2.tar", last modified: Fri May  5 00:03:05 2023, max compression
```

## Comparing `cellmaps_utils-0.1.0a1.tar` & `cellmaps_utils-0.1.0a2.tar`

### file list

```diff
@@ -1,49 +1,49 @@
-drwxr-xr-x   0 churas     (504) staff       (20)        0 2023-05-01 21:47:56.000000 cellmaps_utils-0.1.0a1/
--rw-r--r--   0 churas     (504) staff       (20)      194 2023-05-01 21:45:35.000000 cellmaps_utils-0.1.0a1/AUTHORS.rst
--rw-r--r--   0 churas     (504) staff       (20)     3611 2023-02-09 20:10:13.000000 cellmaps_utils-0.1.0a1/CONTRIBUTING.rst
--rw-r--r--   0 churas     (504) staff       (20)       89 2023-05-01 21:45:35.000000 cellmaps_utils-0.1.0a1/HISTORY.rst
--rw-r--r--   0 churas     (504) staff       (20)     1102 2023-02-09 20:10:13.000000 cellmaps_utils-0.1.0a1/LICENSE
--rw-r--r--   0 churas     (504) staff       (20)      262 2023-02-09 20:10:13.000000 cellmaps_utils-0.1.0a1/MANIFEST.in
--rw-r--r--   0 churas     (504) staff       (20)     4726 2023-05-01 21:47:56.000000 cellmaps_utils-0.1.0a1/PKG-INFO
--rw-r--r--   0 churas     (504) staff       (20)     2813 2023-05-01 21:47:34.000000 cellmaps_utils-0.1.0a1/README.rst
-drwxr-xr-x   0 churas     (504) staff       (20)        0 2023-05-01 21:47:56.000000 cellmaps_utils-0.1.0a1/cellmaps_utils/
--rw-r--r--   0 churas     (504) staff       (20)      156 2023-05-01 21:45:35.000000 cellmaps_utils-0.1.0a1/cellmaps_utils/__init__.py
--rw-r--r--   0 churas     (504) staff       (20)      795 2023-05-01 21:45:35.000000 cellmaps_utils-0.1.0a1/cellmaps_utils/constants.py
--rw-r--r--   0 churas     (504) staff       (20)     8231 2023-04-14 18:52:11.000000 cellmaps_utils-0.1.0a1/cellmaps_utils/logutils.py
--rw-r--r--   0 churas     (504) staff       (20)     5947 2023-04-14 17:44:35.000000 cellmaps_utils-0.1.0a1/cellmaps_utils/music_utils.py
-drwxr-xr-x   0 churas     (504) staff       (20)        0 2023-05-01 21:47:56.000000 cellmaps_utils-0.1.0a1/cellmaps_utils.egg-info/
--rw-r--r--   0 churas     (504) staff       (20)     4726 2023-05-01 21:47:55.000000 cellmaps_utils-0.1.0a1/cellmaps_utils.egg-info/PKG-INFO
--rw-r--r--   0 churas     (504) staff       (20)      896 2023-05-01 21:47:55.000000 cellmaps_utils-0.1.0a1/cellmaps_utils.egg-info/SOURCES.txt
--rw-r--r--   0 churas     (504) staff       (20)        1 2023-05-01 21:47:55.000000 cellmaps_utils-0.1.0a1/cellmaps_utils.egg-info/dependency_links.txt
--rw-r--r--   0 churas     (504) staff       (20)        1 2023-05-01 21:47:55.000000 cellmaps_utils-0.1.0a1/cellmaps_utils.egg-info/not-zip-safe
--rw-r--r--   0 churas     (504) staff       (20)       37 2023-05-01 21:47:55.000000 cellmaps_utils-0.1.0a1/cellmaps_utils.egg-info/requires.txt
--rw-r--r--   0 churas     (504) staff       (20)       15 2023-05-01 21:47:55.000000 cellmaps_utils-0.1.0a1/cellmaps_utils.egg-info/top_level.txt
-drwxr-xr-x   0 churas     (504) staff       (20)        0 2023-05-01 21:47:56.000000 cellmaps_utils-0.1.0a1/docs/
--rw-r--r--   0 churas     (504) staff       (20)      615 2023-02-09 20:10:13.000000 cellmaps_utils-0.1.0a1/docs/Makefile
-drwxr-xr-x   0 churas     (504) staff       (20)        0 2023-05-01 21:47:56.000000 cellmaps_utils-0.1.0a1/docs/_build/
-drwxr-xr-x   0 churas     (504) staff       (20)        0 2023-05-01 21:47:56.000000 cellmaps_utils-0.1.0a1/docs/_build/html/
-drwxr-xr-x   0 churas     (504) staff       (20)        0 2023-05-01 21:47:56.000000 cellmaps_utils-0.1.0a1/docs/_build/html/_static/
--rw-r--r--   0 churas     (504) staff       (20)      286 2022-02-15 21:42:18.000000 cellmaps_utils-0.1.0a1/docs/_build/html/_static/file.png
--rw-r--r--   0 churas     (504) staff       (20)       90 2022-02-15 21:42:18.000000 cellmaps_utils-0.1.0a1/docs/_build/html/_static/minus.png
--rw-r--r--   0 churas     (504) staff       (20)       90 2022-02-15 21:42:18.000000 cellmaps_utils-0.1.0a1/docs/_build/html/_static/plus.png
--rw-r--r--   0 churas     (504) staff       (20)       28 2023-02-09 20:10:13.000000 cellmaps_utils-0.1.0a1/docs/authors.rst
--rw-r--r--   0 churas     (504) staff       (20)      500 2023-04-14 18:35:21.000000 cellmaps_utils-0.1.0a1/docs/cellmaps_utils.rst
--rwxr-xr-x   0 churas     (504) staff       (20)     5991 2023-02-09 20:10:13.000000 cellmaps_utils-0.1.0a1/docs/conf.py
--rw-r--r--   0 churas     (504) staff       (20)       33 2023-02-09 20:10:13.000000 cellmaps_utils-0.1.0a1/docs/contributing.rst
--rw-r--r--   0 churas     (504) staff       (20)      174 2023-02-09 20:10:13.000000 cellmaps_utils-0.1.0a1/docs/devbranches.rst
--rw-r--r--   0 churas     (504) staff       (20)      282 2023-02-09 20:10:13.000000 cellmaps_utils-0.1.0a1/docs/developer.rst
--rw-r--r--   0 churas     (504) staff       (20)       28 2023-02-09 20:10:13.000000 cellmaps_utils-0.1.0a1/docs/history.rst
--rw-r--r--   0 churas     (504) staff       (20)      852 2023-02-09 20:10:13.000000 cellmaps_utils-0.1.0a1/docs/index.rst
--rw-r--r--   0 churas     (504) staff       (20)     1174 2023-02-09 20:10:13.000000 cellmaps_utils-0.1.0a1/docs/installation.rst
--rw-r--r--   0 churas     (504) staff       (20)      442 2023-02-09 20:10:13.000000 cellmaps_utils-0.1.0a1/docs/integrationtesting.rst
--rw-r--r--   0 churas     (504) staff       (20)      812 2023-02-09 20:10:13.000000 cellmaps_utils-0.1.0a1/docs/make.bat
--rw-r--r--   0 churas     (504) staff       (20)       73 2023-02-09 20:10:13.000000 cellmaps_utils-0.1.0a1/docs/modules.rst
--rw-r--r--   0 churas     (504) staff       (20)     4304 2023-02-09 20:10:13.000000 cellmaps_utils-0.1.0a1/docs/newrelease.rst
--rw-r--r--   0 churas     (504) staff       (20)      784 2023-02-09 20:10:13.000000 cellmaps_utils-0.1.0a1/docs/pypircfile.rst
--rw-r--r--   0 churas     (504) staff       (20)      182 2023-04-14 18:36:55.000000 cellmaps_utils-0.1.0a1/docs/usage.rst
--rw-r--r--   0 churas     (504) staff       (20)      817 2023-02-09 20:10:13.000000 cellmaps_utils-0.1.0a1/docs/versioningscheme.rst
--rw-r--r--   0 churas     (504) staff       (20)      397 2023-05-01 21:47:56.000000 cellmaps_utils-0.1.0a1/setup.cfg
--rw-r--r--   0 churas     (504) staff       (20)     1901 2023-05-01 21:40:49.000000 cellmaps_utils-0.1.0a1/setup.py
-drwxr-xr-x   0 churas     (504) staff       (20)        0 2023-05-01 21:47:56.000000 cellmaps_utils-0.1.0a1/tests/
--rw-r--r--   0 churas     (504) staff       (20)       69 2023-02-09 20:10:13.000000 cellmaps_utils-0.1.0a1/tests/__init__.py
--rw-r--r--   0 churas     (504) staff       (20)     1541 2023-04-14 18:13:18.000000 cellmaps_utils-0.1.0a1/tests/test_logutils.py
+drwxr-xr-x   0 churas     (504) staff       (20)        0 2023-05-05 00:03:05.004344 cellmaps_utils-0.1.0a2/
+-rw-r--r--   0 churas     (504) staff       (20)      194 2023-05-01 21:45:35.000000 cellmaps_utils-0.1.0a2/AUTHORS.rst
+-rw-r--r--   0 churas     (504) staff       (20)     3611 2023-02-09 20:10:13.000000 cellmaps_utils-0.1.0a2/CONTRIBUTING.rst
+-rw-r--r--   0 churas     (504) staff       (20)       89 2023-05-01 21:45:35.000000 cellmaps_utils-0.1.0a2/HISTORY.rst
+-rw-r--r--   0 churas     (504) staff       (20)     1102 2023-02-09 20:10:13.000000 cellmaps_utils-0.1.0a2/LICENSE
+-rw-r--r--   0 churas     (504) staff       (20)      262 2023-02-09 20:10:13.000000 cellmaps_utils-0.1.0a2/MANIFEST.in
+-rw-r--r--   0 churas     (504) staff       (20)     4726 2023-05-05 00:03:05.004464 cellmaps_utils-0.1.0a2/PKG-INFO
+-rw-r--r--   0 churas     (504) staff       (20)     2813 2023-05-01 21:47:34.000000 cellmaps_utils-0.1.0a2/README.rst
+drwxr-xr-x   0 churas     (504) staff       (20)        0 2023-05-05 00:03:04.996921 cellmaps_utils-0.1.0a2/cellmaps_utils/
+-rw-r--r--   0 churas     (504) staff       (20)      156 2023-05-05 00:01:45.000000 cellmaps_utils-0.1.0a2/cellmaps_utils/__init__.py
+-rw-r--r--   0 churas     (504) staff       (20)      795 2023-05-01 21:45:35.000000 cellmaps_utils-0.1.0a2/cellmaps_utils/constants.py
+-rw-r--r--   0 churas     (504) staff       (20)     8281 2023-05-04 23:59:25.000000 cellmaps_utils-0.1.0a2/cellmaps_utils/logutils.py
+-rw-r--r--   0 churas     (504) staff       (20)     5947 2023-04-14 17:44:35.000000 cellmaps_utils-0.1.0a2/cellmaps_utils/music_utils.py
+drwxr-xr-x   0 churas     (504) staff       (20)        0 2023-05-05 00:03:04.998119 cellmaps_utils-0.1.0a2/cellmaps_utils.egg-info/
+-rw-r--r--   0 churas     (504) staff       (20)     4726 2023-05-05 00:03:04.000000 cellmaps_utils-0.1.0a2/cellmaps_utils.egg-info/PKG-INFO
+-rw-r--r--   0 churas     (504) staff       (20)      896 2023-05-05 00:03:04.000000 cellmaps_utils-0.1.0a2/cellmaps_utils.egg-info/SOURCES.txt
+-rw-r--r--   0 churas     (504) staff       (20)        1 2023-05-05 00:03:04.000000 cellmaps_utils-0.1.0a2/cellmaps_utils.egg-info/dependency_links.txt
+-rw-r--r--   0 churas     (504) staff       (20)        1 2023-05-05 00:03:04.000000 cellmaps_utils-0.1.0a2/cellmaps_utils.egg-info/not-zip-safe
+-rw-r--r--   0 churas     (504) staff       (20)       37 2023-05-05 00:03:04.000000 cellmaps_utils-0.1.0a2/cellmaps_utils.egg-info/requires.txt
+-rw-r--r--   0 churas     (504) staff       (20)       15 2023-05-05 00:03:04.000000 cellmaps_utils-0.1.0a2/cellmaps_utils.egg-info/top_level.txt
+drwxr-xr-x   0 churas     (504) staff       (20)        0 2023-05-05 00:03:05.002905 cellmaps_utils-0.1.0a2/docs/
+-rw-r--r--   0 churas     (504) staff       (20)      615 2023-02-09 20:10:13.000000 cellmaps_utils-0.1.0a2/docs/Makefile
+drwxr-xr-x   0 churas     (504) staff       (20)        0 2023-05-05 00:03:04.993441 cellmaps_utils-0.1.0a2/docs/_build/
+drwxr-xr-x   0 churas     (504) staff       (20)        0 2023-05-05 00:03:04.993521 cellmaps_utils-0.1.0a2/docs/_build/html/
+drwxr-xr-x   0 churas     (504) staff       (20)        0 2023-05-05 00:03:05.003696 cellmaps_utils-0.1.0a2/docs/_build/html/_static/
+-rw-r--r--   0 churas     (504) staff       (20)      286 2023-05-02 22:49:28.000000 cellmaps_utils-0.1.0a2/docs/_build/html/_static/file.png
+-rw-r--r--   0 churas     (504) staff       (20)       90 2023-05-02 22:49:28.000000 cellmaps_utils-0.1.0a2/docs/_build/html/_static/minus.png
+-rw-r--r--   0 churas     (504) staff       (20)       90 2023-05-02 22:49:28.000000 cellmaps_utils-0.1.0a2/docs/_build/html/_static/plus.png
+-rw-r--r--   0 churas     (504) staff       (20)       28 2023-02-09 20:10:13.000000 cellmaps_utils-0.1.0a2/docs/authors.rst
+-rw-r--r--   0 churas     (504) staff       (20)      500 2023-05-04 00:00:42.000000 cellmaps_utils-0.1.0a2/docs/cellmaps_utils.rst
+-rwxr-xr-x   0 churas     (504) staff       (20)     5991 2023-02-09 20:10:13.000000 cellmaps_utils-0.1.0a2/docs/conf.py
+-rw-r--r--   0 churas     (504) staff       (20)       33 2023-02-09 20:10:13.000000 cellmaps_utils-0.1.0a2/docs/contributing.rst
+-rw-r--r--   0 churas     (504) staff       (20)      174 2023-02-09 20:10:13.000000 cellmaps_utils-0.1.0a2/docs/devbranches.rst
+-rw-r--r--   0 churas     (504) staff       (20)      282 2023-02-09 20:10:13.000000 cellmaps_utils-0.1.0a2/docs/developer.rst
+-rw-r--r--   0 churas     (504) staff       (20)       28 2023-02-09 20:10:13.000000 cellmaps_utils-0.1.0a2/docs/history.rst
+-rw-r--r--   0 churas     (504) staff       (20)      852 2023-02-09 20:10:13.000000 cellmaps_utils-0.1.0a2/docs/index.rst
+-rw-r--r--   0 churas     (504) staff       (20)     1174 2023-02-09 20:10:13.000000 cellmaps_utils-0.1.0a2/docs/installation.rst
+-rw-r--r--   0 churas     (504) staff       (20)      442 2023-02-09 20:10:13.000000 cellmaps_utils-0.1.0a2/docs/integrationtesting.rst
+-rw-r--r--   0 churas     (504) staff       (20)      812 2023-02-09 20:10:13.000000 cellmaps_utils-0.1.0a2/docs/make.bat
+-rw-r--r--   0 churas     (504) staff       (20)       73 2023-02-09 20:10:13.000000 cellmaps_utils-0.1.0a2/docs/modules.rst
+-rw-r--r--   0 churas     (504) staff       (20)     4304 2023-02-09 20:10:13.000000 cellmaps_utils-0.1.0a2/docs/newrelease.rst
+-rw-r--r--   0 churas     (504) staff       (20)      784 2023-02-09 20:10:13.000000 cellmaps_utils-0.1.0a2/docs/pypircfile.rst
+-rw-r--r--   0 churas     (504) staff       (20)      182 2023-04-14 18:36:55.000000 cellmaps_utils-0.1.0a2/docs/usage.rst
+-rw-r--r--   0 churas     (504) staff       (20)      817 2023-02-09 20:10:13.000000 cellmaps_utils-0.1.0a2/docs/versioningscheme.rst
+-rw-r--r--   0 churas     (504) staff       (20)      397 2023-05-05 00:03:05.004896 cellmaps_utils-0.1.0a2/setup.cfg
+-rw-r--r--   0 churas     (504) staff       (20)     1901 2023-05-01 21:40:49.000000 cellmaps_utils-0.1.0a2/setup.py
+drwxr-xr-x   0 churas     (504) staff       (20)        0 2023-05-05 00:03:05.004165 cellmaps_utils-0.1.0a2/tests/
+-rw-r--r--   0 churas     (504) staff       (20)       69 2023-02-09 20:10:13.000000 cellmaps_utils-0.1.0a2/tests/__init__.py
+-rw-r--r--   0 churas     (504) staff       (20)     1541 2023-04-14 18:13:18.000000 cellmaps_utils-0.1.0a2/tests/test_logutils.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `cellmaps_utils-0.1.0a1/CONTRIBUTING.rst` & `cellmaps_utils-0.1.0a2/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `cellmaps_utils-0.1.0a1/LICENSE` & `cellmaps_utils-0.1.0a2/LICENSE`

 * *Files identical despite different names*

### Comparing `cellmaps_utils-0.1.0a1/PKG-INFO` & `cellmaps_utils-0.1.0a2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cellmaps_utils
-Version: 0.1.0a1
+Version: 0.1.0a2
 Summary: Utilities needed for Cell Maps for AI
 Home-page: https://github.com/idekerlab/cellmaps_utils
 Author: Clara Hu
 Author-email: mhu@health.ucsd.edu
 License: MIT license
 Description: ==============
         cellmaps_utils
```

### Comparing `cellmaps_utils-0.1.0a1/README.rst` & `cellmaps_utils-0.1.0a2/README.rst`

 * *Files identical despite different names*

### Comparing `cellmaps_utils-0.1.0a1/cellmaps_utils/constants.py` & `cellmaps_utils-0.1.0a2/cellmaps_utils/constants.py`

 * *Files identical despite different names*

### Comparing `cellmaps_utils-0.1.0a1/cellmaps_utils/logutils.py` & `cellmaps_utils-0.1.0a2/cellmaps_utils/logutils.py`

 * *Files 0% similar despite different names*

```diff
@@ -177,14 +177,15 @@
     """
     if handlerprefix is None:
         handlerprefix = 'cellmaps'
 
     err_log_file = os.path.join(outdir, constants.ERROR_LOG_FILE)
     out_log_file = os.path.join(outdir, constants.OUTPUT_LOG_FILE)
     logging.config.dictConfig({'version': 1,
+                               'propagate': True,
                                'disable_existing_loggers': False,
                                'loggers': {
                                  '': {
                                      'level': 'NOTSET',
                                      'handlers': [handlerprefix + '_file_handler',
                                                   handlerprefix + '_error_file_handler']
                                  }
```

### Comparing `cellmaps_utils-0.1.0a1/cellmaps_utils/music_utils.py` & `cellmaps_utils-0.1.0a2/cellmaps_utils/music_utils.py`

 * *Files identical despite different names*

### Comparing `cellmaps_utils-0.1.0a1/cellmaps_utils.egg-info/PKG-INFO` & `cellmaps_utils-0.1.0a2/cellmaps_utils.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cellmaps-utils
-Version: 0.1.0a1
+Version: 0.1.0a2
 Summary: Utilities needed for Cell Maps for AI
 Home-page: https://github.com/idekerlab/cellmaps_utils
 Author: Clara Hu
 Author-email: mhu@health.ucsd.edu
 License: MIT license
 Description: ==============
         cellmaps_utils
```

### Comparing `cellmaps_utils-0.1.0a1/cellmaps_utils.egg-info/SOURCES.txt` & `cellmaps_utils-0.1.0a2/cellmaps_utils.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cellmaps_utils-0.1.0a1/docs/Makefile` & `cellmaps_utils-0.1.0a2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `cellmaps_utils-0.1.0a1/docs/conf.py` & `cellmaps_utils-0.1.0a2/docs/conf.py`

 * *Files identical despite different names*

### Comparing `cellmaps_utils-0.1.0a1/docs/index.rst` & `cellmaps_utils-0.1.0a2/docs/index.rst`

 * *Files identical despite different names*

### Comparing `cellmaps_utils-0.1.0a1/docs/installation.rst` & `cellmaps_utils-0.1.0a2/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `cellmaps_utils-0.1.0a1/docs/make.bat` & `cellmaps_utils-0.1.0a2/docs/make.bat`

 * *Files identical despite different names*

### Comparing `cellmaps_utils-0.1.0a1/docs/newrelease.rst` & `cellmaps_utils-0.1.0a2/docs/newrelease.rst`

 * *Files identical despite different names*

### Comparing `cellmaps_utils-0.1.0a1/docs/pypircfile.rst` & `cellmaps_utils-0.1.0a2/docs/pypircfile.rst`

 * *Files identical despite different names*

### Comparing `cellmaps_utils-0.1.0a1/docs/versioningscheme.rst` & `cellmaps_utils-0.1.0a2/docs/versioningscheme.rst`

 * *Files identical despite different names*

### Comparing `cellmaps_utils-0.1.0a1/setup.py` & `cellmaps_utils-0.1.0a2/setup.py`

 * *Files identical despite different names*

### Comparing `cellmaps_utils-0.1.0a1/tests/test_logutils.py` & `cellmaps_utils-0.1.0a2/tests/test_logutils.py`

 * *Files identical despite different names*

