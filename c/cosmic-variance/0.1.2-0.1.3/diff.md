# Comparing `tmp/cosmic_variance-0.1.2.tar.gz` & `tmp/cosmic_variance-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cosmic_variance-0.1.2.tar", last modified: Fri May  5 03:30:56 2023, max compression
+gzip compressed data, was "cosmic_variance-0.1.3.tar", last modified: Fri May  5 03:33:14 2023, max compression
```

## Comparing `cosmic_variance-0.1.2.tar` & `cosmic_variance-0.1.3.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxr-xr-x   0 chri862z   (501) staff       (20)        0 2023-05-05 03:30:56.435406 cosmic_variance-0.1.2/
--rw-r--r--   0 chri862z   (501) staff       (20)      201 2023-01-24 01:54:31.000000 cosmic_variance-0.1.2/AUTHORS.rst
--rw-r--r--   0 chri862z   (501) staff       (20)     3626 2023-01-24 01:57:16.000000 cosmic_variance-0.1.2/CONTRIBUTING.rst
--rw-r--r--   0 chri862z   (501) staff       (20)      205 2023-01-24 02:03:30.000000 cosmic_variance-0.1.2/HISTORY.rst
--rw-r--r--   0 chri862z   (501) staff       (20)     1084 2023-01-23 16:17:52.000000 cosmic_variance-0.1.2/LICENSE
--rw-r--r--   0 chri862z   (501) staff       (20)      262 2023-01-24 01:54:36.000000 cosmic_variance-0.1.2/MANIFEST.in
--rw-r--r--   0 chri862z   (501) staff       (20)     4149 2023-05-05 03:30:56.435548 cosmic_variance-0.1.2/PKG-INFO
--rw-r--r--   0 chri862z   (501) staff       (20)     2825 2023-05-05 03:25:05.000000 cosmic_variance-0.1.2/README.rst
-drwxr-xr-x   0 chri862z   (501) staff       (20)        0 2023-05-05 03:30:56.426578 cosmic_variance-0.1.2/cosmic_variance/
--rw-r--r--   0 chri862z   (501) staff       (20)      213 2023-05-05 03:30:25.000000 cosmic_variance-0.1.2/cosmic_variance/__init__.py
--rw-r--r--   0 chri862z   (501) staff       (20)     5277 2023-05-05 03:26:57.000000 cosmic_variance-0.1.2/cosmic_variance/cosmic_variance.py
-drwxr-xr-x   0 chri862z   (501) staff       (20)        0 2023-05-05 03:30:56.428673 cosmic_variance-0.1.2/cosmic_variance/quickcv/
--rw-r--r--   0 chri862z   (501) staff       (20)     2519 2023-05-05 03:29:28.000000 cosmic_variance-0.1.2/cosmic_variance/quickcv/quickcv.py
-drwxr-xr-x   0 chri862z   (501) staff       (20)        0 2023-05-05 03:30:56.430072 cosmic_variance-0.1.2/cosmic_variance/quickcv/utils/
--rw-r--r--   0 chri862z   (501) staff       (20)       91 2023-05-05 03:29:58.000000 cosmic_variance-0.1.2/cosmic_variance/quickcv/utils/__init__.py
--rw-r--r--   0 chri862z   (501) staff       (20)      398 2023-05-05 02:31:58.000000 cosmic_variance-0.1.2/cosmic_variance/quickcv/utils/dlin.py
--rw-r--r--   0 chri862z   (501) staff       (20)     1562 2023-05-05 03:29:09.000000 cosmic_variance-0.1.2/cosmic_variance/quickcv/utils/intpk4.py
--rw-r--r--   0 chri862z   (501) staff       (20)     1096 2023-05-05 02:32:00.000000 cosmic_variance-0.1.2/cosmic_variance/quickcv/utils/pofk.py
--rw-r--r--   0 chri862z   (501) staff       (20)     1477 2023-05-05 02:31:53.000000 cosmic_variance-0.1.2/cosmic_variance/quickcv/utils/rz.py
-drwxr-xr-x   0 chri862z   (501) staff       (20)        0 2023-05-05 03:30:56.428378 cosmic_variance-0.1.2/cosmic_variance.egg-info/
--rw-r--r--   0 chri862z   (501) staff       (20)     4149 2023-05-05 03:30:56.000000 cosmic_variance-0.1.2/cosmic_variance.egg-info/PKG-INFO
--rw-r--r--   0 chri862z   (501) staff       (20)      827 2023-05-05 03:30:56.000000 cosmic_variance-0.1.2/cosmic_variance.egg-info/SOURCES.txt
--rw-r--r--   0 chri862z   (501) staff       (20)        1 2023-05-05 03:30:56.000000 cosmic_variance-0.1.2/cosmic_variance.egg-info/dependency_links.txt
--rw-r--r--   0 chri862z   (501) staff       (20)        1 2023-01-23 16:47:07.000000 cosmic_variance-0.1.2/cosmic_variance.egg-info/not-zip-safe
--rw-r--r--   0 chri862z   (501) staff       (20)       41 2023-05-05 03:30:56.000000 cosmic_variance-0.1.2/cosmic_variance.egg-info/requires.txt
--rw-r--r--   0 chri862z   (501) staff       (20)       16 2023-05-05 03:30:56.000000 cosmic_variance-0.1.2/cosmic_variance.egg-info/top_level.txt
-drwxr-xr-x   0 chri862z   (501) staff       (20)        0 2023-05-05 03:30:56.434518 cosmic_variance-0.1.2/docs/
--rw-r--r--   0 chri862z   (501) staff       (20)      616 2023-01-23 16:17:53.000000 cosmic_variance-0.1.2/docs/Makefile
--rw-r--r--   0 chri862z   (501) staff       (20)       28 2023-01-23 16:17:53.000000 cosmic_variance-0.1.2/docs/authors.rst
--rwxr-xr-x   0 chri862z   (501) staff       (20)     4921 2023-01-23 16:17:53.000000 cosmic_variance-0.1.2/docs/conf.py
--rw-r--r--   0 chri862z   (501) staff       (20)       33 2023-01-23 16:17:53.000000 cosmic_variance-0.1.2/docs/contributing.rst
--rw-r--r--   0 chri862z   (501) staff       (20)       28 2023-01-23 16:17:53.000000 cosmic_variance-0.1.2/docs/history.rst
--rw-r--r--   0 chri862z   (501) staff       (20)      312 2023-01-23 16:17:53.000000 cosmic_variance-0.1.2/docs/index.rst
--rw-r--r--   0 chri862z   (501) staff       (20)     1190 2023-01-23 16:17:53.000000 cosmic_variance-0.1.2/docs/installation.rst
--rw-r--r--   0 chri862z   (501) staff       (20)      813 2023-01-23 16:17:53.000000 cosmic_variance-0.1.2/docs/make.bat
--rw-r--r--   0 chri862z   (501) staff       (20)       27 2023-01-23 16:17:53.000000 cosmic_variance-0.1.2/docs/readme.rst
--rw-r--r--   0 chri862z   (501) staff       (20)       85 2023-01-23 16:17:53.000000 cosmic_variance-0.1.2/docs/usage.rst
--rw-r--r--   0 chri862z   (501) staff       (20)      387 2023-05-05 03:30:56.436068 cosmic_variance-0.1.2/setup.cfg
--rw-r--r--   0 chri862z   (501) staff       (20)     1474 2023-05-05 03:30:21.000000 cosmic_variance-0.1.2/setup.py
-drwxr-xr-x   0 chri862z   (501) staff       (20)        0 2023-05-05 03:30:56.435170 cosmic_variance-0.1.2/tests/
--rw-r--r--   0 chri862z   (501) staff       (20)       45 2023-01-23 16:17:53.000000 cosmic_variance-0.1.2/tests/__init__.py
--rw-r--r--   0 chri862z   (501) staff       (20)      427 2023-01-23 16:17:53.000000 cosmic_variance-0.1.2/tests/test_cosmic_variance.py
+drwxr-xr-x   0 chri862z   (501) staff       (20)        0 2023-05-05 03:33:14.830947 cosmic_variance-0.1.3/
+-rw-r--r--   0 chri862z   (501) staff       (20)      201 2023-01-24 01:54:31.000000 cosmic_variance-0.1.3/AUTHORS.rst
+-rw-r--r--   0 chri862z   (501) staff       (20)     3626 2023-01-24 01:57:16.000000 cosmic_variance-0.1.3/CONTRIBUTING.rst
+-rw-r--r--   0 chri862z   (501) staff       (20)      205 2023-01-24 02:03:30.000000 cosmic_variance-0.1.3/HISTORY.rst
+-rw-r--r--   0 chri862z   (501) staff       (20)     1084 2023-01-23 16:17:52.000000 cosmic_variance-0.1.3/LICENSE
+-rw-r--r--   0 chri862z   (501) staff       (20)      262 2023-01-24 01:54:36.000000 cosmic_variance-0.1.3/MANIFEST.in
+-rw-r--r--   0 chri862z   (501) staff       (20)     4149 2023-05-05 03:33:14.831227 cosmic_variance-0.1.3/PKG-INFO
+-rw-r--r--   0 chri862z   (501) staff       (20)     2825 2023-05-05 03:25:05.000000 cosmic_variance-0.1.3/README.rst
+drwxr-xr-x   0 chri862z   (501) staff       (20)        0 2023-05-05 03:33:14.821022 cosmic_variance-0.1.3/cosmic_variance/
+-rw-r--r--   0 chri862z   (501) staff       (20)      213 2023-05-05 03:32:57.000000 cosmic_variance-0.1.3/cosmic_variance/__init__.py
+-rw-r--r--   0 chri862z   (501) staff       (20)     5277 2023-05-05 03:26:57.000000 cosmic_variance-0.1.3/cosmic_variance/cosmic_variance.py
+drwxr-xr-x   0 chri862z   (501) staff       (20)        0 2023-05-05 03:33:14.823256 cosmic_variance-0.1.3/cosmic_variance/quickcv/
+-rw-r--r--   0 chri862z   (501) staff       (20)     2519 2023-05-05 03:29:28.000000 cosmic_variance-0.1.3/cosmic_variance/quickcv/quickcv.py
+drwxr-xr-x   0 chri862z   (501) staff       (20)        0 2023-05-05 03:33:14.824780 cosmic_variance-0.1.3/cosmic_variance/quickcv/utils/
+-rw-r--r--   0 chri862z   (501) staff       (20)       94 2023-05-05 03:33:08.000000 cosmic_variance-0.1.3/cosmic_variance/quickcv/utils/__init__.py
+-rw-r--r--   0 chri862z   (501) staff       (20)      398 2023-05-05 02:31:58.000000 cosmic_variance-0.1.3/cosmic_variance/quickcv/utils/dlin.py
+-rw-r--r--   0 chri862z   (501) staff       (20)     1562 2023-05-05 03:32:41.000000 cosmic_variance-0.1.3/cosmic_variance/quickcv/utils/intpk4.py
+-rw-r--r--   0 chri862z   (501) staff       (20)     1096 2023-05-05 02:32:00.000000 cosmic_variance-0.1.3/cosmic_variance/quickcv/utils/pofk.py
+-rw-r--r--   0 chri862z   (501) staff       (20)     1477 2023-05-05 02:31:53.000000 cosmic_variance-0.1.3/cosmic_variance/quickcv/utils/rz.py
+drwxr-xr-x   0 chri862z   (501) staff       (20)        0 2023-05-05 03:33:14.822940 cosmic_variance-0.1.3/cosmic_variance.egg-info/
+-rw-r--r--   0 chri862z   (501) staff       (20)     4149 2023-05-05 03:33:14.000000 cosmic_variance-0.1.3/cosmic_variance.egg-info/PKG-INFO
+-rw-r--r--   0 chri862z   (501) staff       (20)      827 2023-05-05 03:33:14.000000 cosmic_variance-0.1.3/cosmic_variance.egg-info/SOURCES.txt
+-rw-r--r--   0 chri862z   (501) staff       (20)        1 2023-05-05 03:33:14.000000 cosmic_variance-0.1.3/cosmic_variance.egg-info/dependency_links.txt
+-rw-r--r--   0 chri862z   (501) staff       (20)        1 2023-01-23 16:47:07.000000 cosmic_variance-0.1.3/cosmic_variance.egg-info/not-zip-safe
+-rw-r--r--   0 chri862z   (501) staff       (20)       41 2023-05-05 03:33:14.000000 cosmic_variance-0.1.3/cosmic_variance.egg-info/requires.txt
+-rw-r--r--   0 chri862z   (501) staff       (20)       16 2023-05-05 03:33:14.000000 cosmic_variance-0.1.3/cosmic_variance.egg-info/top_level.txt
+drwxr-xr-x   0 chri862z   (501) staff       (20)        0 2023-05-05 03:33:14.829711 cosmic_variance-0.1.3/docs/
+-rw-r--r--   0 chri862z   (501) staff       (20)      616 2023-01-23 16:17:53.000000 cosmic_variance-0.1.3/docs/Makefile
+-rw-r--r--   0 chri862z   (501) staff       (20)       28 2023-01-23 16:17:53.000000 cosmic_variance-0.1.3/docs/authors.rst
+-rwxr-xr-x   0 chri862z   (501) staff       (20)     4921 2023-01-23 16:17:53.000000 cosmic_variance-0.1.3/docs/conf.py
+-rw-r--r--   0 chri862z   (501) staff       (20)       33 2023-01-23 16:17:53.000000 cosmic_variance-0.1.3/docs/contributing.rst
+-rw-r--r--   0 chri862z   (501) staff       (20)       28 2023-01-23 16:17:53.000000 cosmic_variance-0.1.3/docs/history.rst
+-rw-r--r--   0 chri862z   (501) staff       (20)      312 2023-01-23 16:17:53.000000 cosmic_variance-0.1.3/docs/index.rst
+-rw-r--r--   0 chri862z   (501) staff       (20)     1190 2023-01-23 16:17:53.000000 cosmic_variance-0.1.3/docs/installation.rst
+-rw-r--r--   0 chri862z   (501) staff       (20)      813 2023-01-23 16:17:53.000000 cosmic_variance-0.1.3/docs/make.bat
+-rw-r--r--   0 chri862z   (501) staff       (20)       27 2023-01-23 16:17:53.000000 cosmic_variance-0.1.3/docs/readme.rst
+-rw-r--r--   0 chri862z   (501) staff       (20)       85 2023-01-23 16:17:53.000000 cosmic_variance-0.1.3/docs/usage.rst
+-rw-r--r--   0 chri862z   (501) staff       (20)      387 2023-05-05 03:33:14.831800 cosmic_variance-0.1.3/setup.cfg
+-rw-r--r--   0 chri862z   (501) staff       (20)     1474 2023-05-05 03:33:01.000000 cosmic_variance-0.1.3/setup.py
+drwxr-xr-x   0 chri862z   (501) staff       (20)        0 2023-05-05 03:33:14.830464 cosmic_variance-0.1.3/tests/
+-rw-r--r--   0 chri862z   (501) staff       (20)       45 2023-01-23 16:17:53.000000 cosmic_variance-0.1.3/tests/__init__.py
+-rw-r--r--   0 chri862z   (501) staff       (20)      427 2023-01-23 16:17:53.000000 cosmic_variance-0.1.3/tests/test_cosmic_variance.py
```

### Comparing `cosmic_variance-0.1.2/CONTRIBUTING.rst` & `cosmic_variance-0.1.3/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `cosmic_variance-0.1.2/LICENSE` & `cosmic_variance-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `cosmic_variance-0.1.2/PKG-INFO` & `cosmic_variance-0.1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cosmic_variance
-Version: 0.1.2
+Version: 0.1.3
 Summary: Package to calculate cosmic variance in rectangular pencil-beam surveys
 Home-page: https://github.com/astrockragh/cosmic_variance
 Author: Christian Kragh Jespersen
 Author-email: ckragh@princeton.edu
 License: MIT license
 Description: ===============================
         Cosmic Variance Calculator
```

### Comparing `cosmic_variance-0.1.2/README.rst` & `cosmic_variance-0.1.3/README.rst`

 * *Files identical despite different names*

### Comparing `cosmic_variance-0.1.2/cosmic_variance/cosmic_variance.py` & `cosmic_variance-0.1.3/cosmic_variance/cosmic_variance.py`

 * *Files identical despite different names*

### Comparing `cosmic_variance-0.1.2/cosmic_variance/quickcv/quickcv.py` & `cosmic_variance-0.1.3/cosmic_variance/quickcv/quickcv.py`

 * *Files identical despite different names*

### Comparing `cosmic_variance-0.1.2/cosmic_variance/quickcv/utils/intpk4.py` & `cosmic_variance-0.1.3/cosmic_variance/quickcv/utils/intpk4.py`

 * *Files identical despite different names*

### Comparing `cosmic_variance-0.1.2/cosmic_variance/quickcv/utils/pofk.py` & `cosmic_variance-0.1.3/cosmic_variance/quickcv/utils/pofk.py`

 * *Files identical despite different names*

### Comparing `cosmic_variance-0.1.2/cosmic_variance/quickcv/utils/rz.py` & `cosmic_variance-0.1.3/cosmic_variance/quickcv/utils/rz.py`

 * *Files identical despite different names*

### Comparing `cosmic_variance-0.1.2/cosmic_variance.egg-info/PKG-INFO` & `cosmic_variance-0.1.3/cosmic_variance.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cosmic-variance
-Version: 0.1.2
+Version: 0.1.3
 Summary: Package to calculate cosmic variance in rectangular pencil-beam surveys
 Home-page: https://github.com/astrockragh/cosmic_variance
 Author: Christian Kragh Jespersen
 Author-email: ckragh@princeton.edu
 License: MIT license
 Description: ===============================
         Cosmic Variance Calculator
```

### Comparing `cosmic_variance-0.1.2/cosmic_variance.egg-info/SOURCES.txt` & `cosmic_variance-0.1.3/cosmic_variance.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cosmic_variance-0.1.2/docs/Makefile` & `cosmic_variance-0.1.3/docs/Makefile`

 * *Files identical despite different names*

### Comparing `cosmic_variance-0.1.2/docs/conf.py` & `cosmic_variance-0.1.3/docs/conf.py`

 * *Files identical despite different names*

### Comparing `cosmic_variance-0.1.2/docs/installation.rst` & `cosmic_variance-0.1.3/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `cosmic_variance-0.1.2/docs/make.bat` & `cosmic_variance-0.1.3/docs/make.bat`

 * *Files identical despite different names*

### Comparing `cosmic_variance-0.1.2/setup.py` & `cosmic_variance-0.1.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -36,10 +36,10 @@
     include_package_data = True,
     keywords = ['Cosmology', 'Galaxies', 'Statistics', 'Astrostatistics', 'Cosmic Variance'],
     name = 'cosmic_variance',
     packages=find_packages(include=['cosmic_variance', 'cosmic_variance.*']),
     test_suite='tests',
     tests_require=test_requirements,
     url='https://github.com/astrockragh/cosmic_variance',
-    version='0.1.2',
+    version='0.1.3',
     zip_safe=False,
 )
```

