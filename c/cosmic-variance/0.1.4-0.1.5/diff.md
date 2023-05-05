# Comparing `tmp/cosmic_variance-0.1.4.tar.gz` & `tmp/cosmic_variance-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cosmic_variance-0.1.4.tar", last modified: Fri May  5 03:35:09 2023, max compression
+gzip compressed data, was "cosmic_variance-0.1.5.tar", last modified: Fri May  5 03:40:51 2023, max compression
```

## Comparing `cosmic_variance-0.1.4.tar` & `cosmic_variance-0.1.5.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxr-xr-x   0 chri862z   (501) staff       (20)        0 2023-05-05 03:35:09.464345 cosmic_variance-0.1.4/
--rw-r--r--   0 chri862z   (501) staff       (20)      201 2023-01-24 01:54:31.000000 cosmic_variance-0.1.4/AUTHORS.rst
--rw-r--r--   0 chri862z   (501) staff       (20)     3626 2023-01-24 01:57:16.000000 cosmic_variance-0.1.4/CONTRIBUTING.rst
--rw-r--r--   0 chri862z   (501) staff       (20)      205 2023-01-24 02:03:30.000000 cosmic_variance-0.1.4/HISTORY.rst
--rw-r--r--   0 chri862z   (501) staff       (20)     1084 2023-01-23 16:17:52.000000 cosmic_variance-0.1.4/LICENSE
--rw-r--r--   0 chri862z   (501) staff       (20)      262 2023-01-24 01:54:36.000000 cosmic_variance-0.1.4/MANIFEST.in
--rw-r--r--   0 chri862z   (501) staff       (20)     4149 2023-05-05 03:35:09.464497 cosmic_variance-0.1.4/PKG-INFO
--rw-r--r--   0 chri862z   (501) staff       (20)     2825 2023-05-05 03:25:05.000000 cosmic_variance-0.1.4/README.rst
-drwxr-xr-x   0 chri862z   (501) staff       (20)        0 2023-05-05 03:35:09.456085 cosmic_variance-0.1.4/cosmic_variance/
--rw-r--r--   0 chri862z   (501) staff       (20)      213 2023-05-05 03:34:54.000000 cosmic_variance-0.1.4/cosmic_variance/__init__.py
--rw-r--r--   0 chri862z   (501) staff       (20)     5277 2023-05-05 03:26:57.000000 cosmic_variance-0.1.4/cosmic_variance/cosmic_variance.py
-drwxr-xr-x   0 chri862z   (501) staff       (20)        0 2023-05-05 03:35:09.458183 cosmic_variance-0.1.4/cosmic_variance/quickcv/
--rw-r--r--   0 chri862z   (501) staff       (20)     2502 2023-05-05 03:34:49.000000 cosmic_variance-0.1.4/cosmic_variance/quickcv/quickcv.py
-drwxr-xr-x   0 chri862z   (501) staff       (20)        0 2023-05-05 03:35:09.459729 cosmic_variance-0.1.4/cosmic_variance/quickcv/utils/
--rw-r--r--   0 chri862z   (501) staff       (20)       94 2023-05-05 03:33:08.000000 cosmic_variance-0.1.4/cosmic_variance/quickcv/utils/__init__.py
--rw-r--r--   0 chri862z   (501) staff       (20)      398 2023-05-05 02:31:58.000000 cosmic_variance-0.1.4/cosmic_variance/quickcv/utils/dlin.py
--rw-r--r--   0 chri862z   (501) staff       (20)     1562 2023-05-05 03:34:28.000000 cosmic_variance-0.1.4/cosmic_variance/quickcv/utils/intpk4.py
--rw-r--r--   0 chri862z   (501) staff       (20)     1096 2023-05-05 03:34:31.000000 cosmic_variance-0.1.4/cosmic_variance/quickcv/utils/pofk.py
--rw-r--r--   0 chri862z   (501) staff       (20)     1477 2023-05-05 02:31:53.000000 cosmic_variance-0.1.4/cosmic_variance/quickcv/utils/rz.py
-drwxr-xr-x   0 chri862z   (501) staff       (20)        0 2023-05-05 03:35:09.457899 cosmic_variance-0.1.4/cosmic_variance.egg-info/
--rw-r--r--   0 chri862z   (501) staff       (20)     4149 2023-05-05 03:35:09.000000 cosmic_variance-0.1.4/cosmic_variance.egg-info/PKG-INFO
--rw-r--r--   0 chri862z   (501) staff       (20)      827 2023-05-05 03:35:09.000000 cosmic_variance-0.1.4/cosmic_variance.egg-info/SOURCES.txt
--rw-r--r--   0 chri862z   (501) staff       (20)        1 2023-05-05 03:35:09.000000 cosmic_variance-0.1.4/cosmic_variance.egg-info/dependency_links.txt
--rw-r--r--   0 chri862z   (501) staff       (20)        1 2023-01-23 16:47:07.000000 cosmic_variance-0.1.4/cosmic_variance.egg-info/not-zip-safe
--rw-r--r--   0 chri862z   (501) staff       (20)       41 2023-05-05 03:35:09.000000 cosmic_variance-0.1.4/cosmic_variance.egg-info/requires.txt
--rw-r--r--   0 chri862z   (501) staff       (20)       16 2023-05-05 03:35:09.000000 cosmic_variance-0.1.4/cosmic_variance.egg-info/top_level.txt
-drwxr-xr-x   0 chri862z   (501) staff       (20)        0 2023-05-05 03:35:09.463360 cosmic_variance-0.1.4/docs/
--rw-r--r--   0 chri862z   (501) staff       (20)      616 2023-01-23 16:17:53.000000 cosmic_variance-0.1.4/docs/Makefile
--rw-r--r--   0 chri862z   (501) staff       (20)       28 2023-01-23 16:17:53.000000 cosmic_variance-0.1.4/docs/authors.rst
--rwxr-xr-x   0 chri862z   (501) staff       (20)     4921 2023-01-23 16:17:53.000000 cosmic_variance-0.1.4/docs/conf.py
--rw-r--r--   0 chri862z   (501) staff       (20)       33 2023-01-23 16:17:53.000000 cosmic_variance-0.1.4/docs/contributing.rst
--rw-r--r--   0 chri862z   (501) staff       (20)       28 2023-01-23 16:17:53.000000 cosmic_variance-0.1.4/docs/history.rst
--rw-r--r--   0 chri862z   (501) staff       (20)      312 2023-01-23 16:17:53.000000 cosmic_variance-0.1.4/docs/index.rst
--rw-r--r--   0 chri862z   (501) staff       (20)     1190 2023-01-23 16:17:53.000000 cosmic_variance-0.1.4/docs/installation.rst
--rw-r--r--   0 chri862z   (501) staff       (20)      813 2023-01-23 16:17:53.000000 cosmic_variance-0.1.4/docs/make.bat
--rw-r--r--   0 chri862z   (501) staff       (20)       27 2023-01-23 16:17:53.000000 cosmic_variance-0.1.4/docs/readme.rst
--rw-r--r--   0 chri862z   (501) staff       (20)       85 2023-01-23 16:17:53.000000 cosmic_variance-0.1.4/docs/usage.rst
--rw-r--r--   0 chri862z   (501) staff       (20)      387 2023-05-05 03:35:09.465028 cosmic_variance-0.1.4/setup.cfg
--rw-r--r--   0 chri862z   (501) staff       (20)     1474 2023-05-05 03:35:03.000000 cosmic_variance-0.1.4/setup.py
-drwxr-xr-x   0 chri862z   (501) staff       (20)        0 2023-05-05 03:35:09.464067 cosmic_variance-0.1.4/tests/
--rw-r--r--   0 chri862z   (501) staff       (20)       45 2023-01-23 16:17:53.000000 cosmic_variance-0.1.4/tests/__init__.py
--rw-r--r--   0 chri862z   (501) staff       (20)      427 2023-01-23 16:17:53.000000 cosmic_variance-0.1.4/tests/test_cosmic_variance.py
+drwxr-xr-x   0 chri862z   (501) staff       (20)        0 2023-05-05 03:40:51.979140 cosmic_variance-0.1.5/
+-rw-r--r--   0 chri862z   (501) staff       (20)      201 2023-01-24 01:54:31.000000 cosmic_variance-0.1.5/AUTHORS.rst
+-rw-r--r--   0 chri862z   (501) staff       (20)     3626 2023-01-24 01:57:16.000000 cosmic_variance-0.1.5/CONTRIBUTING.rst
+-rw-r--r--   0 chri862z   (501) staff       (20)      205 2023-01-24 02:03:30.000000 cosmic_variance-0.1.5/HISTORY.rst
+-rw-r--r--   0 chri862z   (501) staff       (20)     1084 2023-01-23 16:17:52.000000 cosmic_variance-0.1.5/LICENSE
+-rw-r--r--   0 chri862z   (501) staff       (20)      262 2023-01-24 01:54:36.000000 cosmic_variance-0.1.5/MANIFEST.in
+-rw-r--r--   0 chri862z   (501) staff       (20)     4149 2023-05-05 03:40:51.979281 cosmic_variance-0.1.5/PKG-INFO
+-rw-r--r--   0 chri862z   (501) staff       (20)     2825 2023-05-05 03:25:05.000000 cosmic_variance-0.1.5/README.rst
+drwxr-xr-x   0 chri862z   (501) staff       (20)        0 2023-05-05 03:40:51.971932 cosmic_variance-0.1.5/cosmic_variance/
+-rw-r--r--   0 chri862z   (501) staff       (20)      213 2023-05-05 03:40:39.000000 cosmic_variance-0.1.5/cosmic_variance/__init__.py
+-rw-r--r--   0 chri862z   (501) staff       (20)     5363 2023-05-05 03:40:06.000000 cosmic_variance-0.1.5/cosmic_variance/cosmic_variance.py
+drwxr-xr-x   0 chri862z   (501) staff       (20)        0 2023-05-05 03:40:51.973799 cosmic_variance-0.1.5/cosmic_variance/quickcv/
+-rw-r--r--   0 chri862z   (501) staff       (20)     2502 2023-05-05 03:40:43.000000 cosmic_variance-0.1.5/cosmic_variance/quickcv/quickcv.py
+drwxr-xr-x   0 chri862z   (501) staff       (20)        0 2023-05-05 03:40:51.975101 cosmic_variance-0.1.5/cosmic_variance/quickcv/utils/
+-rw-r--r--   0 chri862z   (501) staff       (20)       94 2023-05-05 03:40:18.000000 cosmic_variance-0.1.5/cosmic_variance/quickcv/utils/__init__.py
+-rw-r--r--   0 chri862z   (501) staff       (20)      398 2023-05-05 02:31:58.000000 cosmic_variance-0.1.5/cosmic_variance/quickcv/utils/dlin.py
+-rw-r--r--   0 chri862z   (501) staff       (20)     1562 2023-05-05 03:40:46.000000 cosmic_variance-0.1.5/cosmic_variance/quickcv/utils/intpk4.py
+-rw-r--r--   0 chri862z   (501) staff       (20)     1096 2023-05-05 03:40:44.000000 cosmic_variance-0.1.5/cosmic_variance/quickcv/utils/pofk.py
+-rw-r--r--   0 chri862z   (501) staff       (20)     1477 2023-05-05 02:31:53.000000 cosmic_variance-0.1.5/cosmic_variance/quickcv/utils/rz.py
+drwxr-xr-x   0 chri862z   (501) staff       (20)        0 2023-05-05 03:40:51.973532 cosmic_variance-0.1.5/cosmic_variance.egg-info/
+-rw-r--r--   0 chri862z   (501) staff       (20)     4149 2023-05-05 03:40:51.000000 cosmic_variance-0.1.5/cosmic_variance.egg-info/PKG-INFO
+-rw-r--r--   0 chri862z   (501) staff       (20)      827 2023-05-05 03:40:51.000000 cosmic_variance-0.1.5/cosmic_variance.egg-info/SOURCES.txt
+-rw-r--r--   0 chri862z   (501) staff       (20)        1 2023-05-05 03:40:51.000000 cosmic_variance-0.1.5/cosmic_variance.egg-info/dependency_links.txt
+-rw-r--r--   0 chri862z   (501) staff       (20)        1 2023-01-23 16:47:07.000000 cosmic_variance-0.1.5/cosmic_variance.egg-info/not-zip-safe
+-rw-r--r--   0 chri862z   (501) staff       (20)       41 2023-05-05 03:40:51.000000 cosmic_variance-0.1.5/cosmic_variance.egg-info/requires.txt
+-rw-r--r--   0 chri862z   (501) staff       (20)       16 2023-05-05 03:40:51.000000 cosmic_variance-0.1.5/cosmic_variance.egg-info/top_level.txt
+drwxr-xr-x   0 chri862z   (501) staff       (20)        0 2023-05-05 03:40:51.978270 cosmic_variance-0.1.5/docs/
+-rw-r--r--   0 chri862z   (501) staff       (20)      616 2023-01-23 16:17:53.000000 cosmic_variance-0.1.5/docs/Makefile
+-rw-r--r--   0 chri862z   (501) staff       (20)       28 2023-01-23 16:17:53.000000 cosmic_variance-0.1.5/docs/authors.rst
+-rwxr-xr-x   0 chri862z   (501) staff       (20)     4921 2023-01-23 16:17:53.000000 cosmic_variance-0.1.5/docs/conf.py
+-rw-r--r--   0 chri862z   (501) staff       (20)       33 2023-01-23 16:17:53.000000 cosmic_variance-0.1.5/docs/contributing.rst
+-rw-r--r--   0 chri862z   (501) staff       (20)       28 2023-01-23 16:17:53.000000 cosmic_variance-0.1.5/docs/history.rst
+-rw-r--r--   0 chri862z   (501) staff       (20)      312 2023-01-23 16:17:53.000000 cosmic_variance-0.1.5/docs/index.rst
+-rw-r--r--   0 chri862z   (501) staff       (20)     1190 2023-01-23 16:17:53.000000 cosmic_variance-0.1.5/docs/installation.rst
+-rw-r--r--   0 chri862z   (501) staff       (20)      813 2023-01-23 16:17:53.000000 cosmic_variance-0.1.5/docs/make.bat
+-rw-r--r--   0 chri862z   (501) staff       (20)       27 2023-01-23 16:17:53.000000 cosmic_variance-0.1.5/docs/readme.rst
+-rw-r--r--   0 chri862z   (501) staff       (20)       85 2023-01-23 16:17:53.000000 cosmic_variance-0.1.5/docs/usage.rst
+-rw-r--r--   0 chri862z   (501) staff       (20)      387 2023-05-05 03:40:51.979783 cosmic_variance-0.1.5/setup.cfg
+-rw-r--r--   0 chri862z   (501) staff       (20)     1474 2023-05-05 03:40:41.000000 cosmic_variance-0.1.5/setup.py
+drwxr-xr-x   0 chri862z   (501) staff       (20)        0 2023-05-05 03:40:51.978873 cosmic_variance-0.1.5/tests/
+-rw-r--r--   0 chri862z   (501) staff       (20)       45 2023-01-23 16:17:53.000000 cosmic_variance-0.1.5/tests/__init__.py
+-rw-r--r--   0 chri862z   (501) staff       (20)      427 2023-01-23 16:17:53.000000 cosmic_variance-0.1.5/tests/test_cosmic_variance.py
```

### Comparing `cosmic_variance-0.1.4/CONTRIBUTING.rst` & `cosmic_variance-0.1.5/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `cosmic_variance-0.1.4/LICENSE` & `cosmic_variance-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `cosmic_variance-0.1.4/PKG-INFO` & `cosmic_variance-0.1.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cosmic_variance
-Version: 0.1.4
+Version: 0.1.5
 Summary: Package to calculate cosmic variance in rectangular pencil-beam surveys
 Home-page: https://github.com/astrockragh/cosmic_variance
 Author: Christian Kragh Jespersen
 Author-email: ckragh@princeton.edu
 License: MIT license
 Description: ===============================
         Cosmic Variance Calculator
```

### Comparing `cosmic_variance-0.1.4/README.rst` & `cosmic_variance-0.1.5/README.rst`

 * *Files identical despite different names*

### Comparing `cosmic_variance-0.1.4/cosmic_variance/cosmic_variance.py` & `cosmic_variance-0.1.5/cosmic_variance/cosmic_variance.py`

 * *Files 2% similar despite different names*

```diff
@@ -106,15 +106,17 @@
 
    for i in range(nz):
       if dz is None:
          dz      = zarr[i+1]-zarr[i]
          zmid    = zarr[i+1]+zarr[i]
          zmid    = zmid/2
       else:
-         zmid    = zarr
+         if i == 0:
+            print('dz is given, zarr is redshift bin centers')
+         zmid    = zarr[i]
       
       s       = quickcv.quickcv(side1, side2, np.array([zmid]), np.array([dz]), OmegaM = OmegaM, OmegaL = OmegaL, OmegaBaryon = OmegaBaryon, \
                                 sigma8 = sigma8, ns = ns, h = h, acc = acc, verbose = verbose)
       
       ## These are the linear bias values
       bias70  = b070  * (zmid+1)**b170  + b270
       bias75  = b075  * (zmid+1)**b175  + b275
```

### Comparing `cosmic_variance-0.1.4/cosmic_variance/quickcv/quickcv.py` & `cosmic_variance-0.1.5/cosmic_variance/quickcv/quickcv.py`

 * *Files identical despite different names*

### Comparing `cosmic_variance-0.1.4/cosmic_variance/quickcv/utils/intpk4.py` & `cosmic_variance-0.1.5/cosmic_variance/quickcv/utils/intpk4.py`

 * *Files identical despite different names*

### Comparing `cosmic_variance-0.1.4/cosmic_variance/quickcv/utils/pofk.py` & `cosmic_variance-0.1.5/cosmic_variance/quickcv/utils/pofk.py`

 * *Files identical despite different names*

### Comparing `cosmic_variance-0.1.4/cosmic_variance/quickcv/utils/rz.py` & `cosmic_variance-0.1.5/cosmic_variance/quickcv/utils/rz.py`

 * *Files identical despite different names*

### Comparing `cosmic_variance-0.1.4/cosmic_variance.egg-info/PKG-INFO` & `cosmic_variance-0.1.5/cosmic_variance.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cosmic-variance
-Version: 0.1.4
+Version: 0.1.5
 Summary: Package to calculate cosmic variance in rectangular pencil-beam surveys
 Home-page: https://github.com/astrockragh/cosmic_variance
 Author: Christian Kragh Jespersen
 Author-email: ckragh@princeton.edu
 License: MIT license
 Description: ===============================
         Cosmic Variance Calculator
```

### Comparing `cosmic_variance-0.1.4/cosmic_variance.egg-info/SOURCES.txt` & `cosmic_variance-0.1.5/cosmic_variance.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cosmic_variance-0.1.4/docs/Makefile` & `cosmic_variance-0.1.5/docs/Makefile`

 * *Files identical despite different names*

### Comparing `cosmic_variance-0.1.4/docs/conf.py` & `cosmic_variance-0.1.5/docs/conf.py`

 * *Files identical despite different names*

### Comparing `cosmic_variance-0.1.4/docs/installation.rst` & `cosmic_variance-0.1.5/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `cosmic_variance-0.1.4/docs/make.bat` & `cosmic_variance-0.1.5/docs/make.bat`

 * *Files identical despite different names*

### Comparing `cosmic_variance-0.1.4/setup.py` & `cosmic_variance-0.1.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -36,10 +36,10 @@
     include_package_data = True,
     keywords = ['Cosmology', 'Galaxies', 'Statistics', 'Astrostatistics', 'Cosmic Variance'],
     name = 'cosmic_variance',
     packages=find_packages(include=['cosmic_variance', 'cosmic_variance.*']),
     test_suite='tests',
     tests_require=test_requirements,
     url='https://github.com/astrockragh/cosmic_variance',
-    version='0.1.4',
+    version='0.1.5',
     zip_safe=False,
 )
```

