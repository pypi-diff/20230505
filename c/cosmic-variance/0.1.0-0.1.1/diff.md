# Comparing `tmp/cosmic_variance-0.1.0.tar.gz` & `tmp/cosmic_variance-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/cosmic_variance-0.1.0.tar", last modified: Fri May  5 02:50:53 2023, max compression
+gzip compressed data, was "cosmic_variance-0.1.1.tar", last modified: Fri May  5 03:27:21 2023, max compression
```

## Comparing `cosmic_variance-0.1.0.tar` & `cosmic_variance-0.1.1.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxr-xr-x   0 chri862z   (501) staff       (20)        0 2023-05-05 02:50:53.661141 cosmic_variance-0.1.0/
--rw-r--r--   0 chri862z   (501) staff       (20)      201 2023-01-24 01:54:31.000000 cosmic_variance-0.1.0/AUTHORS.rst
--rw-r--r--   0 chri862z   (501) staff       (20)     3626 2023-01-24 01:57:16.000000 cosmic_variance-0.1.0/CONTRIBUTING.rst
--rw-r--r--   0 chri862z   (501) staff       (20)      205 2023-01-24 02:03:30.000000 cosmic_variance-0.1.0/HISTORY.rst
--rw-r--r--   0 chri862z   (501) staff       (20)     1084 2023-01-23 16:17:52.000000 cosmic_variance-0.1.0/LICENSE
--rw-r--r--   0 chri862z   (501) staff       (20)      262 2023-01-24 01:54:36.000000 cosmic_variance-0.1.0/MANIFEST.in
--rw-r--r--   0 chri862z   (501) staff       (20)     4081 2023-05-05 02:50:53.661305 cosmic_variance-0.1.0/PKG-INFO
--rw-r--r--   0 chri862z   (501) staff       (20)     2757 2023-05-05 02:48:15.000000 cosmic_variance-0.1.0/README.rst
-drwxr-xr-x   0 chri862z   (501) staff       (20)        0 2023-05-05 02:50:53.651596 cosmic_variance-0.1.0/cosmic_variance/
--rw-r--r--   0 chri862z   (501) staff       (20)      213 2023-05-05 02:50:36.000000 cosmic_variance-0.1.0/cosmic_variance/__init__.py
--rw-r--r--   0 chri862z   (501) staff       (20)     5227 2023-05-05 02:39:50.000000 cosmic_variance-0.1.0/cosmic_variance/cosmic_variance.py
-drwxr-xr-x   0 chri862z   (501) staff       (20)        0 2023-05-05 02:50:53.654478 cosmic_variance-0.1.0/cosmic_variance/quickcv/
--rw-r--r--   0 chri862z   (501) staff       (20)        0 2023-05-05 02:35:17.000000 cosmic_variance-0.1.0/cosmic_variance/quickcv/__init__.py
--rw-r--r--   0 chri862z   (501) staff       (20)     2519 2023-05-05 02:35:12.000000 cosmic_variance-0.1.0/cosmic_variance/quickcv/quickcv.py
-drwxr-xr-x   0 chri862z   (501) staff       (20)        0 2023-05-05 02:50:53.656259 cosmic_variance-0.1.0/cosmic_variance/quickcv/utils/
--rw-r--r--   0 chri862z   (501) staff       (20)      100 2023-01-24 01:57:27.000000 cosmic_variance-0.1.0/cosmic_variance/quickcv/utils/__init__.py
--rw-r--r--   0 chri862z   (501) staff       (20)      398 2023-05-05 02:31:58.000000 cosmic_variance-0.1.0/cosmic_variance/quickcv/utils/dlin.py
--rw-r--r--   0 chri862z   (501) staff       (20)     1562 2023-05-05 02:32:03.000000 cosmic_variance-0.1.0/cosmic_variance/quickcv/utils/intpk4.py
--rw-r--r--   0 chri862z   (501) staff       (20)     1096 2023-05-05 02:32:00.000000 cosmic_variance-0.1.0/cosmic_variance/quickcv/utils/pofk.py
--rw-r--r--   0 chri862z   (501) staff       (20)     1477 2023-05-05 02:31:53.000000 cosmic_variance-0.1.0/cosmic_variance/quickcv/utils/rz.py
-drwxr-xr-x   0 chri862z   (501) staff       (20)        0 2023-05-05 02:50:53.653871 cosmic_variance-0.1.0/cosmic_variance.egg-info/
--rw-r--r--   0 chri862z   (501) staff       (20)     4081 2023-05-05 02:50:53.000000 cosmic_variance-0.1.0/cosmic_variance.egg-info/PKG-INFO
--rw-r--r--   0 chri862z   (501) staff       (20)      863 2023-05-05 02:50:53.000000 cosmic_variance-0.1.0/cosmic_variance.egg-info/SOURCES.txt
--rw-r--r--   0 chri862z   (501) staff       (20)        1 2023-05-05 02:50:53.000000 cosmic_variance-0.1.0/cosmic_variance.egg-info/dependency_links.txt
--rw-r--r--   0 chri862z   (501) staff       (20)        1 2023-01-23 16:47:07.000000 cosmic_variance-0.1.0/cosmic_variance.egg-info/not-zip-safe
--rw-r--r--   0 chri862z   (501) staff       (20)       41 2023-05-05 02:50:53.000000 cosmic_variance-0.1.0/cosmic_variance.egg-info/requires.txt
--rw-r--r--   0 chri862z   (501) staff       (20)       16 2023-05-05 02:50:53.000000 cosmic_variance-0.1.0/cosmic_variance.egg-info/top_level.txt
-drwxr-xr-x   0 chri862z   (501) staff       (20)        0 2023-05-05 02:50:53.660229 cosmic_variance-0.1.0/docs/
--rw-r--r--   0 chri862z   (501) staff       (20)      616 2023-01-23 16:17:53.000000 cosmic_variance-0.1.0/docs/Makefile
--rw-r--r--   0 chri862z   (501) staff       (20)       28 2023-01-23 16:17:53.000000 cosmic_variance-0.1.0/docs/authors.rst
--rwxr-xr-x   0 chri862z   (501) staff       (20)     4921 2023-01-23 16:17:53.000000 cosmic_variance-0.1.0/docs/conf.py
--rw-r--r--   0 chri862z   (501) staff       (20)       33 2023-01-23 16:17:53.000000 cosmic_variance-0.1.0/docs/contributing.rst
--rw-r--r--   0 chri862z   (501) staff       (20)       28 2023-01-23 16:17:53.000000 cosmic_variance-0.1.0/docs/history.rst
--rw-r--r--   0 chri862z   (501) staff       (20)      312 2023-01-23 16:17:53.000000 cosmic_variance-0.1.0/docs/index.rst
--rw-r--r--   0 chri862z   (501) staff       (20)     1190 2023-01-23 16:17:53.000000 cosmic_variance-0.1.0/docs/installation.rst
--rw-r--r--   0 chri862z   (501) staff       (20)      813 2023-01-23 16:17:53.000000 cosmic_variance-0.1.0/docs/make.bat
--rw-r--r--   0 chri862z   (501) staff       (20)       27 2023-01-23 16:17:53.000000 cosmic_variance-0.1.0/docs/readme.rst
--rw-r--r--   0 chri862z   (501) staff       (20)       85 2023-01-23 16:17:53.000000 cosmic_variance-0.1.0/docs/usage.rst
--rw-r--r--   0 chri862z   (501) staff       (20)      387 2023-05-05 02:50:53.661872 cosmic_variance-0.1.0/setup.cfg
--rw-r--r--   0 chri862z   (501) staff       (20)     1474 2023-05-05 02:50:31.000000 cosmic_variance-0.1.0/setup.py
-drwxr-xr-x   0 chri862z   (501) staff       (20)        0 2023-05-05 02:50:53.660867 cosmic_variance-0.1.0/tests/
--rw-r--r--   0 chri862z   (501) staff       (20)       45 2023-01-23 16:17:53.000000 cosmic_variance-0.1.0/tests/__init__.py
--rw-r--r--   0 chri862z   (501) staff       (20)      427 2023-01-23 16:17:53.000000 cosmic_variance-0.1.0/tests/test_cosmic_variance.py
+drwxr-xr-x   0 chri862z   (501) staff       (20)        0 2023-05-05 03:27:21.973472 cosmic_variance-0.1.1/
+-rw-r--r--   0 chri862z   (501) staff       (20)      201 2023-01-24 01:54:31.000000 cosmic_variance-0.1.1/AUTHORS.rst
+-rw-r--r--   0 chri862z   (501) staff       (20)     3626 2023-01-24 01:57:16.000000 cosmic_variance-0.1.1/CONTRIBUTING.rst
+-rw-r--r--   0 chri862z   (501) staff       (20)      205 2023-01-24 02:03:30.000000 cosmic_variance-0.1.1/HISTORY.rst
+-rw-r--r--   0 chri862z   (501) staff       (20)     1084 2023-01-23 16:17:52.000000 cosmic_variance-0.1.1/LICENSE
+-rw-r--r--   0 chri862z   (501) staff       (20)      262 2023-01-24 01:54:36.000000 cosmic_variance-0.1.1/MANIFEST.in
+-rw-r--r--   0 chri862z   (501) staff       (20)     4149 2023-05-05 03:27:21.973594 cosmic_variance-0.1.1/PKG-INFO
+-rw-r--r--   0 chri862z   (501) staff       (20)     2825 2023-05-05 03:25:05.000000 cosmic_variance-0.1.1/README.rst
+drwxr-xr-x   0 chri862z   (501) staff       (20)        0 2023-05-05 03:27:21.965196 cosmic_variance-0.1.1/cosmic_variance/
+-rw-r--r--   0 chri862z   (501) staff       (20)      213 2023-05-05 03:26:58.000000 cosmic_variance-0.1.1/cosmic_variance/__init__.py
+-rw-r--r--   0 chri862z   (501) staff       (20)     5277 2023-05-05 03:26:57.000000 cosmic_variance-0.1.1/cosmic_variance/cosmic_variance.py
+drwxr-xr-x   0 chri862z   (501) staff       (20)        0 2023-05-05 03:27:21.967071 cosmic_variance-0.1.1/cosmic_variance/quickcv/
+-rw-r--r--   0 chri862z   (501) staff       (20)        0 2023-05-05 02:35:17.000000 cosmic_variance-0.1.1/cosmic_variance/quickcv/__init__.py
+-rw-r--r--   0 chri862z   (501) staff       (20)     2519 2023-05-05 03:25:45.000000 cosmic_variance-0.1.1/cosmic_variance/quickcv/quickcv.py
+drwxr-xr-x   0 chri862z   (501) staff       (20)        0 2023-05-05 03:27:21.968430 cosmic_variance-0.1.1/cosmic_variance/quickcv/utils/
+-rw-r--r--   0 chri862z   (501) staff       (20)      100 2023-01-24 01:57:27.000000 cosmic_variance-0.1.1/cosmic_variance/quickcv/utils/__init__.py
+-rw-r--r--   0 chri862z   (501) staff       (20)      398 2023-05-05 02:31:58.000000 cosmic_variance-0.1.1/cosmic_variance/quickcv/utils/dlin.py
+-rw-r--r--   0 chri862z   (501) staff       (20)     1562 2023-05-05 02:32:03.000000 cosmic_variance-0.1.1/cosmic_variance/quickcv/utils/intpk4.py
+-rw-r--r--   0 chri862z   (501) staff       (20)     1096 2023-05-05 02:32:00.000000 cosmic_variance-0.1.1/cosmic_variance/quickcv/utils/pofk.py
+-rw-r--r--   0 chri862z   (501) staff       (20)     1477 2023-05-05 02:31:53.000000 cosmic_variance-0.1.1/cosmic_variance/quickcv/utils/rz.py
+drwxr-xr-x   0 chri862z   (501) staff       (20)        0 2023-05-05 03:27:21.966663 cosmic_variance-0.1.1/cosmic_variance.egg-info/
+-rw-r--r--   0 chri862z   (501) staff       (20)     4149 2023-05-05 03:27:21.000000 cosmic_variance-0.1.1/cosmic_variance.egg-info/PKG-INFO
+-rw-r--r--   0 chri862z   (501) staff       (20)      863 2023-05-05 03:27:21.000000 cosmic_variance-0.1.1/cosmic_variance.egg-info/SOURCES.txt
+-rw-r--r--   0 chri862z   (501) staff       (20)        1 2023-05-05 03:27:21.000000 cosmic_variance-0.1.1/cosmic_variance.egg-info/dependency_links.txt
+-rw-r--r--   0 chri862z   (501) staff       (20)        1 2023-01-23 16:47:07.000000 cosmic_variance-0.1.1/cosmic_variance.egg-info/not-zip-safe
+-rw-r--r--   0 chri862z   (501) staff       (20)       41 2023-05-05 03:27:21.000000 cosmic_variance-0.1.1/cosmic_variance.egg-info/requires.txt
+-rw-r--r--   0 chri862z   (501) staff       (20)       16 2023-05-05 03:27:21.000000 cosmic_variance-0.1.1/cosmic_variance.egg-info/top_level.txt
+drwxr-xr-x   0 chri862z   (501) staff       (20)        0 2023-05-05 03:27:21.972418 cosmic_variance-0.1.1/docs/
+-rw-r--r--   0 chri862z   (501) staff       (20)      616 2023-01-23 16:17:53.000000 cosmic_variance-0.1.1/docs/Makefile
+-rw-r--r--   0 chri862z   (501) staff       (20)       28 2023-01-23 16:17:53.000000 cosmic_variance-0.1.1/docs/authors.rst
+-rwxr-xr-x   0 chri862z   (501) staff       (20)     4921 2023-01-23 16:17:53.000000 cosmic_variance-0.1.1/docs/conf.py
+-rw-r--r--   0 chri862z   (501) staff       (20)       33 2023-01-23 16:17:53.000000 cosmic_variance-0.1.1/docs/contributing.rst
+-rw-r--r--   0 chri862z   (501) staff       (20)       28 2023-01-23 16:17:53.000000 cosmic_variance-0.1.1/docs/history.rst
+-rw-r--r--   0 chri862z   (501) staff       (20)      312 2023-01-23 16:17:53.000000 cosmic_variance-0.1.1/docs/index.rst
+-rw-r--r--   0 chri862z   (501) staff       (20)     1190 2023-01-23 16:17:53.000000 cosmic_variance-0.1.1/docs/installation.rst
+-rw-r--r--   0 chri862z   (501) staff       (20)      813 2023-01-23 16:17:53.000000 cosmic_variance-0.1.1/docs/make.bat
+-rw-r--r--   0 chri862z   (501) staff       (20)       27 2023-01-23 16:17:53.000000 cosmic_variance-0.1.1/docs/readme.rst
+-rw-r--r--   0 chri862z   (501) staff       (20)       85 2023-01-23 16:17:53.000000 cosmic_variance-0.1.1/docs/usage.rst
+-rw-r--r--   0 chri862z   (501) staff       (20)      387 2023-05-05 03:27:21.974077 cosmic_variance-0.1.1/setup.cfg
+-rw-r--r--   0 chri862z   (501) staff       (20)     1474 2023-05-05 03:27:03.000000 cosmic_variance-0.1.1/setup.py
+drwxr-xr-x   0 chri862z   (501) staff       (20)        0 2023-05-05 03:27:21.973170 cosmic_variance-0.1.1/tests/
+-rw-r--r--   0 chri862z   (501) staff       (20)       45 2023-01-23 16:17:53.000000 cosmic_variance-0.1.1/tests/__init__.py
+-rw-r--r--   0 chri862z   (501) staff       (20)      427 2023-01-23 16:17:53.000000 cosmic_variance-0.1.1/tests/test_cosmic_variance.py
```

### Comparing `cosmic_variance-0.1.0/CONTRIBUTING.rst` & `cosmic_variance-0.1.1/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `cosmic_variance-0.1.0/LICENSE` & `cosmic_variance-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `cosmic_variance-0.1.0/PKG-INFO` & `cosmic_variance-0.1.1/cosmic_variance.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: cosmic_variance
-Version: 0.1.0
+Name: cosmic-variance
+Version: 0.1.1
 Summary: Package to calculate cosmic variance in rectangular pencil-beam surveys
 Home-page: https://github.com/astrockragh/cosmic_variance
 Author: Christian Kragh Jespersen
 Author-email: ckragh@princeton.edu
 License: MIT license
 Description: ===============================
         Cosmic Variance Calculator
@@ -48,15 +48,15 @@
                 import numpy as np
                 # Example of using the main function, get_cv to calculate
                 # cosmic variance for a single JWST pointing
         
                 #### these arguments are required ####
                 side1 = 2.2/60. # /60 to convert from arcmin to degrees
                 side2 = 2*2.2/60. # /60 to convert from arcmin to degrees
-                zarray = np.array([7,8,9,11,13]) # redshift bin edges
+                zarray = np.array([7,8,9,11,13]) # redshift bin edges, if dz is given, this array will be the center of the redshift bins
         
                 #### these arguments are optional ####
                 name = 'JWST' # name of the survey, if provided, the output file will be saved as dfs/{name}.csv along with a meta file.
                 # Default is None, in which case the output will not be saved
         
                 acc = 'low' # accuracy of the calculation, 'low' or 'high, low is default, faster and sufficient for almost all applications
```

### Comparing `cosmic_variance-0.1.0/README.rst` & `cosmic_variance-0.1.1/README.rst`

 * *Files 3% similar despite different names*

```diff
@@ -40,15 +40,15 @@
         import numpy as np
         # Example of using the main function, get_cv to calculate
         # cosmic variance for a single JWST pointing
 
         #### these arguments are required ####
         side1 = 2.2/60. # /60 to convert from arcmin to degrees
         side2 = 2*2.2/60. # /60 to convert from arcmin to degrees
-        zarray = np.array([7,8,9,11,13]) # redshift bin edges
+        zarray = np.array([7,8,9,11,13]) # redshift bin edges, if dz is given, this array will be the center of the redshift bins
 
         #### these arguments are optional ####
         name = 'JWST' # name of the survey, if provided, the output file will be saved as dfs/{name}.csv along with a meta file.
         # Default is None, in which case the output will not be saved
 
         acc = 'low' # accuracy of the calculation, 'low' or 'high, low is default, faster and sufficient for almost all applications
```

### Comparing `cosmic_variance-0.1.0/cosmic_variance/cosmic_variance.py` & `cosmic_variance-0.1.1/cosmic_variance/cosmic_variance.py`

 * *Files 2% similar despite different names*

```diff
@@ -92,16 +92,18 @@
             'OmegaBaryon': OmegaBaryon, 
             'sigma8': sigma8,
             'ns': ns,
             'h': h,
             'verbose': verbose}
 
    df_meta = pd.DataFrame(metadict)
-
-   nz = len(zarr)-1
+   if dz is None:
+      nz = len(zarr)-1
+   else:
+      nz = len(zarr)
 
    columns = ['zmid', 'dz', 'cv_dm', 'cv_70', "cv_75", "cv_80", "cv_85", "cv_90", "cv_95", "cv_100", "cv_105", "cv_110"]
    df_values = pd.DataFrame(index = np.arange(nz), columns = columns)
 
    for i in range(nz):
       if dz is None:
          dz      = zarr[i+1]-zarr[i]
```

### Comparing `cosmic_variance-0.1.0/cosmic_variance/quickcv/quickcv.py` & `cosmic_variance-0.1.1/cosmic_variance/quickcv/quickcv.py`

 * *Files identical despite different names*

### Comparing `cosmic_variance-0.1.0/cosmic_variance/quickcv/utils/intpk4.py` & `cosmic_variance-0.1.1/cosmic_variance/quickcv/utils/intpk4.py`

 * *Files identical despite different names*

### Comparing `cosmic_variance-0.1.0/cosmic_variance/quickcv/utils/pofk.py` & `cosmic_variance-0.1.1/cosmic_variance/quickcv/utils/pofk.py`

 * *Files identical despite different names*

### Comparing `cosmic_variance-0.1.0/cosmic_variance/quickcv/utils/rz.py` & `cosmic_variance-0.1.1/cosmic_variance/quickcv/utils/rz.py`

 * *Files identical despite different names*

### Comparing `cosmic_variance-0.1.0/cosmic_variance.egg-info/PKG-INFO` & `cosmic_variance-0.1.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: cosmic-variance
-Version: 0.1.0
+Name: cosmic_variance
+Version: 0.1.1
 Summary: Package to calculate cosmic variance in rectangular pencil-beam surveys
 Home-page: https://github.com/astrockragh/cosmic_variance
 Author: Christian Kragh Jespersen
 Author-email: ckragh@princeton.edu
 License: MIT license
 Description: ===============================
         Cosmic Variance Calculator
@@ -48,15 +48,15 @@
                 import numpy as np
                 # Example of using the main function, get_cv to calculate
                 # cosmic variance for a single JWST pointing
         
                 #### these arguments are required ####
                 side1 = 2.2/60. # /60 to convert from arcmin to degrees
                 side2 = 2*2.2/60. # /60 to convert from arcmin to degrees
-                zarray = np.array([7,8,9,11,13]) # redshift bin edges
+                zarray = np.array([7,8,9,11,13]) # redshift bin edges, if dz is given, this array will be the center of the redshift bins
         
                 #### these arguments are optional ####
                 name = 'JWST' # name of the survey, if provided, the output file will be saved as dfs/{name}.csv along with a meta file.
                 # Default is None, in which case the output will not be saved
         
                 acc = 'low' # accuracy of the calculation, 'low' or 'high, low is default, faster and sufficient for almost all applications
```

### Comparing `cosmic_variance-0.1.0/cosmic_variance.egg-info/SOURCES.txt` & `cosmic_variance-0.1.1/cosmic_variance.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cosmic_variance-0.1.0/docs/Makefile` & `cosmic_variance-0.1.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `cosmic_variance-0.1.0/docs/conf.py` & `cosmic_variance-0.1.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `cosmic_variance-0.1.0/docs/installation.rst` & `cosmic_variance-0.1.1/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `cosmic_variance-0.1.0/docs/make.bat` & `cosmic_variance-0.1.1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `cosmic_variance-0.1.0/setup.py` & `cosmic_variance-0.1.1/setup.py`

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
-    version='0.1.0',
+    version='0.1.1',
     zip_safe=False,
 )
```

