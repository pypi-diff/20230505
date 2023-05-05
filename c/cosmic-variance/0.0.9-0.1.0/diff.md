# Comparing `tmp/cosmic_variance-0.0.9.tar.gz` & `tmp/cosmic_variance-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cosmic_variance-0.0.9.tar", last modified: Tue Jan 24 02:15:47 2023, max compression
+gzip compressed data, was "dist/cosmic_variance-0.1.0.tar", last modified: Fri May  5 02:50:53 2023, max compression
```

## Comparing `cosmic_variance-0.0.9.tar` & `cosmic_variance-0.1.0.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxr-xr-x   0 chri862z   (501) staff       (20)        0 2023-01-24 02:15:47.625243 cosmic_variance-0.0.9/
--rw-r--r--   0 chri862z   (501) staff       (20)      201 2023-01-24 01:54:31.000000 cosmic_variance-0.0.9/AUTHORS.rst
--rw-r--r--   0 chri862z   (501) staff       (20)     3626 2023-01-24 01:57:16.000000 cosmic_variance-0.0.9/CONTRIBUTING.rst
--rw-r--r--   0 chri862z   (501) staff       (20)      205 2023-01-24 02:03:30.000000 cosmic_variance-0.0.9/HISTORY.rst
--rw-r--r--   0 chri862z   (501) staff       (20)     1084 2023-01-23 16:17:52.000000 cosmic_variance-0.0.9/LICENSE
--rw-r--r--   0 chri862z   (501) staff       (20)      262 2023-01-24 01:54:36.000000 cosmic_variance-0.0.9/MANIFEST.in
--rw-r--r--   0 chri862z   (501) staff       (20)     4157 2023-01-24 02:15:47.625456 cosmic_variance-0.0.9/PKG-INFO
--rw-r--r--   0 chri862z   (501) staff       (20)     2837 2023-01-24 02:15:37.000000 cosmic_variance-0.0.9/README.rst
-drwxr-xr-x   0 chri862z   (501) staff       (20)        0 2023-01-24 02:15:47.611070 cosmic_variance-0.0.9/cosmic_variance/
--rw-r--r--   0 chri862z   (501) staff       (20)      213 2023-01-24 01:57:44.000000 cosmic_variance-0.0.9/cosmic_variance/__init__.py
--rw-r--r--   0 chri862z   (501) staff       (20)     3713 2023-01-24 01:58:03.000000 cosmic_variance-0.0.9/cosmic_variance/cosmic_variance.py
-drwxr-xr-x   0 chri862z   (501) staff       (20)        0 2023-01-24 02:15:47.614100 cosmic_variance-0.0.9/cosmic_variance/quickcv/
--rw-r--r--   0 chri862z   (501) staff       (20)        0 2023-01-24 01:57:57.000000 cosmic_variance-0.0.9/cosmic_variance/quickcv/__init__.py
--rw-r--r--   0 chri862z   (501) staff       (20)     2402 2023-01-24 01:57:04.000000 cosmic_variance-0.0.9/cosmic_variance/quickcv/quickcv.py
-drwxr-xr-x   0 chri862z   (501) staff       (20)        0 2023-01-24 02:15:47.615983 cosmic_variance-0.0.9/cosmic_variance/quickcv/utils/
--rw-r--r--   0 chri862z   (501) staff       (20)      100 2023-01-24 01:57:27.000000 cosmic_variance-0.0.9/cosmic_variance/quickcv/utils/__init__.py
--rw-r--r--   0 chri862z   (501) staff       (20)      351 2023-01-24 01:57:07.000000 cosmic_variance-0.0.9/cosmic_variance/quickcv/utils/dlin.py
--rw-r--r--   0 chri862z   (501) staff       (20)     1590 2023-01-24 01:56:54.000000 cosmic_variance-0.0.9/cosmic_variance/quickcv/utils/intpk4.py
--rw-r--r--   0 chri862z   (501) staff       (20)     1888 2023-01-24 01:56:58.000000 cosmic_variance-0.0.9/cosmic_variance/quickcv/utils/pofk.py
--rw-r--r--   0 chri862z   (501) staff       (20)     1431 2023-01-24 01:57:11.000000 cosmic_variance-0.0.9/cosmic_variance/quickcv/utils/rz.py
-drwxr-xr-x   0 chri862z   (501) staff       (20)        0 2023-01-24 02:15:47.613373 cosmic_variance-0.0.9/cosmic_variance.egg-info/
--rw-r--r--   0 chri862z   (501) staff       (20)     4157 2023-01-24 02:15:47.000000 cosmic_variance-0.0.9/cosmic_variance.egg-info/PKG-INFO
--rw-r--r--   0 chri862z   (501) staff       (20)      863 2023-01-24 02:15:47.000000 cosmic_variance-0.0.9/cosmic_variance.egg-info/SOURCES.txt
--rw-r--r--   0 chri862z   (501) staff       (20)        1 2023-01-24 02:15:47.000000 cosmic_variance-0.0.9/cosmic_variance.egg-info/dependency_links.txt
--rw-r--r--   0 chri862z   (501) staff       (20)        1 2023-01-23 16:47:07.000000 cosmic_variance-0.0.9/cosmic_variance.egg-info/not-zip-safe
--rw-r--r--   0 chri862z   (501) staff       (20)       41 2023-01-24 02:15:47.000000 cosmic_variance-0.0.9/cosmic_variance.egg-info/requires.txt
--rw-r--r--   0 chri862z   (501) staff       (20)       16 2023-01-24 02:15:47.000000 cosmic_variance-0.0.9/cosmic_variance.egg-info/top_level.txt
-drwxr-xr-x   0 chri862z   (501) staff       (20)        0 2023-01-24 02:15:47.621815 cosmic_variance-0.0.9/docs/
--rw-r--r--   0 chri862z   (501) staff       (20)      616 2023-01-23 16:17:53.000000 cosmic_variance-0.0.9/docs/Makefile
--rw-r--r--   0 chri862z   (501) staff       (20)       28 2023-01-23 16:17:53.000000 cosmic_variance-0.0.9/docs/authors.rst
--rwxr-xr-x   0 chri862z   (501) staff       (20)     4921 2023-01-23 16:17:53.000000 cosmic_variance-0.0.9/docs/conf.py
--rw-r--r--   0 chri862z   (501) staff       (20)       33 2023-01-23 16:17:53.000000 cosmic_variance-0.0.9/docs/contributing.rst
--rw-r--r--   0 chri862z   (501) staff       (20)       28 2023-01-23 16:17:53.000000 cosmic_variance-0.0.9/docs/history.rst
--rw-r--r--   0 chri862z   (501) staff       (20)      312 2023-01-23 16:17:53.000000 cosmic_variance-0.0.9/docs/index.rst
--rw-r--r--   0 chri862z   (501) staff       (20)     1190 2023-01-23 16:17:53.000000 cosmic_variance-0.0.9/docs/installation.rst
--rw-r--r--   0 chri862z   (501) staff       (20)      813 2023-01-23 16:17:53.000000 cosmic_variance-0.0.9/docs/make.bat
--rw-r--r--   0 chri862z   (501) staff       (20)       27 2023-01-23 16:17:53.000000 cosmic_variance-0.0.9/docs/readme.rst
--rw-r--r--   0 chri862z   (501) staff       (20)       85 2023-01-23 16:17:53.000000 cosmic_variance-0.0.9/docs/usage.rst
--rw-r--r--   0 chri862z   (501) staff       (20)      387 2023-01-24 02:15:47.626154 cosmic_variance-0.0.9/setup.cfg
--rw-r--r--   0 chri862z   (501) staff       (20)     1468 2023-01-24 02:15:42.000000 cosmic_variance-0.0.9/setup.py
-drwxr-xr-x   0 chri862z   (501) staff       (20)        0 2023-01-24 02:15:47.624513 cosmic_variance-0.0.9/tests/
--rw-r--r--   0 chri862z   (501) staff       (20)       45 2023-01-23 16:17:53.000000 cosmic_variance-0.0.9/tests/__init__.py
--rw-r--r--   0 chri862z   (501) staff       (20)      427 2023-01-23 16:17:53.000000 cosmic_variance-0.0.9/tests/test_cosmic_variance.py
+drwxr-xr-x   0 chri862z   (501) staff       (20)        0 2023-05-05 02:50:53.661141 cosmic_variance-0.1.0/
+-rw-r--r--   0 chri862z   (501) staff       (20)      201 2023-01-24 01:54:31.000000 cosmic_variance-0.1.0/AUTHORS.rst
+-rw-r--r--   0 chri862z   (501) staff       (20)     3626 2023-01-24 01:57:16.000000 cosmic_variance-0.1.0/CONTRIBUTING.rst
+-rw-r--r--   0 chri862z   (501) staff       (20)      205 2023-01-24 02:03:30.000000 cosmic_variance-0.1.0/HISTORY.rst
+-rw-r--r--   0 chri862z   (501) staff       (20)     1084 2023-01-23 16:17:52.000000 cosmic_variance-0.1.0/LICENSE
+-rw-r--r--   0 chri862z   (501) staff       (20)      262 2023-01-24 01:54:36.000000 cosmic_variance-0.1.0/MANIFEST.in
+-rw-r--r--   0 chri862z   (501) staff       (20)     4081 2023-05-05 02:50:53.661305 cosmic_variance-0.1.0/PKG-INFO
+-rw-r--r--   0 chri862z   (501) staff       (20)     2757 2023-05-05 02:48:15.000000 cosmic_variance-0.1.0/README.rst
+drwxr-xr-x   0 chri862z   (501) staff       (20)        0 2023-05-05 02:50:53.651596 cosmic_variance-0.1.0/cosmic_variance/
+-rw-r--r--   0 chri862z   (501) staff       (20)      213 2023-05-05 02:50:36.000000 cosmic_variance-0.1.0/cosmic_variance/__init__.py
+-rw-r--r--   0 chri862z   (501) staff       (20)     5227 2023-05-05 02:39:50.000000 cosmic_variance-0.1.0/cosmic_variance/cosmic_variance.py
+drwxr-xr-x   0 chri862z   (501) staff       (20)        0 2023-05-05 02:50:53.654478 cosmic_variance-0.1.0/cosmic_variance/quickcv/
+-rw-r--r--   0 chri862z   (501) staff       (20)        0 2023-05-05 02:35:17.000000 cosmic_variance-0.1.0/cosmic_variance/quickcv/__init__.py
+-rw-r--r--   0 chri862z   (501) staff       (20)     2519 2023-05-05 02:35:12.000000 cosmic_variance-0.1.0/cosmic_variance/quickcv/quickcv.py
+drwxr-xr-x   0 chri862z   (501) staff       (20)        0 2023-05-05 02:50:53.656259 cosmic_variance-0.1.0/cosmic_variance/quickcv/utils/
+-rw-r--r--   0 chri862z   (501) staff       (20)      100 2023-01-24 01:57:27.000000 cosmic_variance-0.1.0/cosmic_variance/quickcv/utils/__init__.py
+-rw-r--r--   0 chri862z   (501) staff       (20)      398 2023-05-05 02:31:58.000000 cosmic_variance-0.1.0/cosmic_variance/quickcv/utils/dlin.py
+-rw-r--r--   0 chri862z   (501) staff       (20)     1562 2023-05-05 02:32:03.000000 cosmic_variance-0.1.0/cosmic_variance/quickcv/utils/intpk4.py
+-rw-r--r--   0 chri862z   (501) staff       (20)     1096 2023-05-05 02:32:00.000000 cosmic_variance-0.1.0/cosmic_variance/quickcv/utils/pofk.py
+-rw-r--r--   0 chri862z   (501) staff       (20)     1477 2023-05-05 02:31:53.000000 cosmic_variance-0.1.0/cosmic_variance/quickcv/utils/rz.py
+drwxr-xr-x   0 chri862z   (501) staff       (20)        0 2023-05-05 02:50:53.653871 cosmic_variance-0.1.0/cosmic_variance.egg-info/
+-rw-r--r--   0 chri862z   (501) staff       (20)     4081 2023-05-05 02:50:53.000000 cosmic_variance-0.1.0/cosmic_variance.egg-info/PKG-INFO
+-rw-r--r--   0 chri862z   (501) staff       (20)      863 2023-05-05 02:50:53.000000 cosmic_variance-0.1.0/cosmic_variance.egg-info/SOURCES.txt
+-rw-r--r--   0 chri862z   (501) staff       (20)        1 2023-05-05 02:50:53.000000 cosmic_variance-0.1.0/cosmic_variance.egg-info/dependency_links.txt
+-rw-r--r--   0 chri862z   (501) staff       (20)        1 2023-01-23 16:47:07.000000 cosmic_variance-0.1.0/cosmic_variance.egg-info/not-zip-safe
+-rw-r--r--   0 chri862z   (501) staff       (20)       41 2023-05-05 02:50:53.000000 cosmic_variance-0.1.0/cosmic_variance.egg-info/requires.txt
+-rw-r--r--   0 chri862z   (501) staff       (20)       16 2023-05-05 02:50:53.000000 cosmic_variance-0.1.0/cosmic_variance.egg-info/top_level.txt
+drwxr-xr-x   0 chri862z   (501) staff       (20)        0 2023-05-05 02:50:53.660229 cosmic_variance-0.1.0/docs/
+-rw-r--r--   0 chri862z   (501) staff       (20)      616 2023-01-23 16:17:53.000000 cosmic_variance-0.1.0/docs/Makefile
+-rw-r--r--   0 chri862z   (501) staff       (20)       28 2023-01-23 16:17:53.000000 cosmic_variance-0.1.0/docs/authors.rst
+-rwxr-xr-x   0 chri862z   (501) staff       (20)     4921 2023-01-23 16:17:53.000000 cosmic_variance-0.1.0/docs/conf.py
+-rw-r--r--   0 chri862z   (501) staff       (20)       33 2023-01-23 16:17:53.000000 cosmic_variance-0.1.0/docs/contributing.rst
+-rw-r--r--   0 chri862z   (501) staff       (20)       28 2023-01-23 16:17:53.000000 cosmic_variance-0.1.0/docs/history.rst
+-rw-r--r--   0 chri862z   (501) staff       (20)      312 2023-01-23 16:17:53.000000 cosmic_variance-0.1.0/docs/index.rst
+-rw-r--r--   0 chri862z   (501) staff       (20)     1190 2023-01-23 16:17:53.000000 cosmic_variance-0.1.0/docs/installation.rst
+-rw-r--r--   0 chri862z   (501) staff       (20)      813 2023-01-23 16:17:53.000000 cosmic_variance-0.1.0/docs/make.bat
+-rw-r--r--   0 chri862z   (501) staff       (20)       27 2023-01-23 16:17:53.000000 cosmic_variance-0.1.0/docs/readme.rst
+-rw-r--r--   0 chri862z   (501) staff       (20)       85 2023-01-23 16:17:53.000000 cosmic_variance-0.1.0/docs/usage.rst
+-rw-r--r--   0 chri862z   (501) staff       (20)      387 2023-05-05 02:50:53.661872 cosmic_variance-0.1.0/setup.cfg
+-rw-r--r--   0 chri862z   (501) staff       (20)     1474 2023-05-05 02:50:31.000000 cosmic_variance-0.1.0/setup.py
+drwxr-xr-x   0 chri862z   (501) staff       (20)        0 2023-05-05 02:50:53.660867 cosmic_variance-0.1.0/tests/
+-rw-r--r--   0 chri862z   (501) staff       (20)       45 2023-01-23 16:17:53.000000 cosmic_variance-0.1.0/tests/__init__.py
+-rw-r--r--   0 chri862z   (501) staff       (20)      427 2023-01-23 16:17:53.000000 cosmic_variance-0.1.0/tests/test_cosmic_variance.py
```

### Comparing `cosmic_variance-0.0.9/CONTRIBUTING.rst` & `cosmic_variance-0.1.0/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `cosmic_variance-0.0.9/LICENSE` & `cosmic_variance-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `cosmic_variance-0.0.9/PKG-INFO` & `cosmic_variance-0.1.0/cosmic_variance.egg-info/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,32 +1,25 @@
 Metadata-Version: 2.1
-Name: cosmic_variance
-Version: 0.0.9
-Summary: Package to calculate cosmic variance in pencil-beam surveys
-Home-page: https://github.com/astrockragh/pythonCV
+Name: cosmic-variance
+Version: 0.1.0
+Summary: Package to calculate cosmic variance in rectangular pencil-beam surveys
+Home-page: https://github.com/astrockragh/cosmic_variance
 Author: Christian Kragh Jespersen
 Author-email: ckragh@princeton.edu
 License: MIT license
 Description: ===============================
         Cosmic Variance Calculator
         ===============================
         
         Package to calculate cosmic variance in pencil-beam surveys
         ---------------------------------------------------------------------------
         
         .. image:: https://img.shields.io/pypi/v/cosmic_variance.svg
                 :target: https://pypi.python.org/pypi/cosmic_variance
         
-        .. image:: https://img.shields.io/travis/astrockragh/cosmic_variance.svg
-                :target: https://travis-ci.com/astrockragh/cosmic_variance
-        
-        .. image:: https://readthedocs.org/projects/cosmic-variance/badge/?version=latest
-                :target: https://cosmic-variance.readthedocs.io/en/latest/?version=latest
-                :alt: Documentation Status
-        
         
         Python package based on the IDL code released with the Cosmic Variance Cookbook of Moster et al. (2010)
         
         The code is based on galaxy stellar mass bins (as described in https://arxiv.org/pdf/1001.1737.pdf), scaled to dark matter cosmic variance (as described in https://arxiv.org/pdf/astro-ph/0109130.pdf). 
         
         This is significantly more useful than dark matter - only variance, since the empirical galaxy variance is significantly higher.
         
@@ -49,33 +42,38 @@
         
         The main use of the package is through the get_cv function, which takes in a rectangular survey geometry with side lengths side1 and side2 (in degrees), and an array of redshift bin edges, and returns a pandas dataframe with the cosmic variance for 0.5 dex galaxy stellar mass bins for each redshift bin.
         
         .. code-block:: python
         
                 import cosmic_variance as cv
                 import numpy as np
-                # use the main function, get_cv to calculate
+                # Example of using the main function, get_cv to calculate
                 # cosmic variance for a single JWST pointing
         
                 #### these arguments are required ####
                 side1 = 2.2/60. # /60 to convert from arcmin to degrees
                 side2 = 2*2.2/60. # /60 to convert from arcmin to degrees
                 zarray = np.array([7,8,9,11,13]) # redshift bin edges
         
                 #### these arguments are optional ####
-                name = 'JWST' # name of the survey, if provided, the output file will be saved as dfs/{name}.csv along with a meta file
+                name = 'JWST' # name of the survey, if provided, the output file will be saved as dfs/{name}.csv along with a meta file.
+                # Default is None, in which case the output will not be saved
+        
                 acc = 'low' # accuracy of the calculation, 'low' or 'high, low is default, faster and sufficient for almost all applications
         
+                verbose = False # if True, will print out the progress of the calculation, default is False
+        
                 #If you want to use a different cosmology, you can specify it by the following in the get_cv call
-                # OmegaM = 0.308, OmegaL = 0.692, sig8 = 0.82
+                # OmegaM = 0.308, OmegaL = 0.692, OmegaBaryon = 0.022/(0.678)**2 sigma8 = 0.82, ns = 0.96, h = 0.678
         
-                cv_df = cv.get_cv(side1, side2, zarray, name = name, acc=acc)
+                cv_df = cv.get_cv(side1, side2, zarray, name = name, acc=acc, verbose = verbose)
         
         This will calculate the cosmic variance for a 2.2 arcmin x 4.4 arcmin survey in redshifts bin [7, 8], [8,9], [9,11], [11,13] and save the output.
-Keywords: Cosmology,Galaxies,Statistics,AstrostatisticsCosmic Variance
+        
+Keywords: Cosmology,Galaxies,Statistics,Astrostatistics,Cosmic Variance
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
```

### Comparing `cosmic_variance-0.0.9/README.rst` & `cosmic_variance-0.1.0/README.rst`

 * *Files 14% similar despite different names*

```diff
@@ -4,21 +4,14 @@
 
 Package to calculate cosmic variance in pencil-beam surveys
 ---------------------------------------------------------------------------
 
 .. image:: https://img.shields.io/pypi/v/cosmic_variance.svg
         :target: https://pypi.python.org/pypi/cosmic_variance
 
-.. image:: https://img.shields.io/travis/astrockragh/cosmic_variance.svg
-        :target: https://travis-ci.com/astrockragh/cosmic_variance
-
-.. image:: https://readthedocs.org/projects/cosmic-variance/badge/?version=latest
-        :target: https://cosmic-variance.readthedocs.io/en/latest/?version=latest
-        :alt: Documentation Status
-
 
 Python package based on the IDL code released with the Cosmic Variance Cookbook of Moster et al. (2010)
 
 The code is based on galaxy stellar mass bins (as described in https://arxiv.org/pdf/1001.1737.pdf), scaled to dark matter cosmic variance (as described in https://arxiv.org/pdf/astro-ph/0109130.pdf). 
 
 This is significantly more useful than dark matter - only variance, since the empirical galaxy variance is significantly higher.
 
@@ -41,25 +34,29 @@
 
 The main use of the package is through the get_cv function, which takes in a rectangular survey geometry with side lengths side1 and side2 (in degrees), and an array of redshift bin edges, and returns a pandas dataframe with the cosmic variance for 0.5 dex galaxy stellar mass bins for each redshift bin.
 
 .. code-block:: python
 
         import cosmic_variance as cv
         import numpy as np
-        # use the main function, get_cv to calculate
+        # Example of using the main function, get_cv to calculate
         # cosmic variance for a single JWST pointing
 
         #### these arguments are required ####
         side1 = 2.2/60. # /60 to convert from arcmin to degrees
         side2 = 2*2.2/60. # /60 to convert from arcmin to degrees
         zarray = np.array([7,8,9,11,13]) # redshift bin edges
 
         #### these arguments are optional ####
-        name = 'JWST' # name of the survey, if provided, the output file will be saved as dfs/{name}.csv along with a meta file
+        name = 'JWST' # name of the survey, if provided, the output file will be saved as dfs/{name}.csv along with a meta file.
+        # Default is None, in which case the output will not be saved
+
         acc = 'low' # accuracy of the calculation, 'low' or 'high, low is default, faster and sufficient for almost all applications
 
+        verbose = False # if True, will print out the progress of the calculation, default is False
+
         #If you want to use a different cosmology, you can specify it by the following in the get_cv call
-        # OmegaM = 0.308, OmegaL = 0.692, sig8 = 0.82
+        # OmegaM = 0.308, OmegaL = 0.692, OmegaBaryon = 0.022/(0.678)**2 sigma8 = 0.82, ns = 0.96, h = 0.678
 
-        cv_df = cv.get_cv(side1, side2, zarray, name = name, acc=acc)
+        cv_df = cv.get_cv(side1, side2, zarray, name = name, acc=acc, verbose = verbose)
 
-This will calculate the cosmic variance for a 2.2 arcmin x 4.4 arcmin survey in redshifts bin [7, 8], [8,9], [9,11], [11,13] and save the output.
+This will calculate the cosmic variance for a 2.2 arcmin x 4.4 arcmin survey in redshifts bin [7, 8], [8,9], [9,11], [11,13] and save the output.
```

### Comparing `cosmic_variance-0.0.9/cosmic_variance/cosmic_variance.py` & `cosmic_variance-0.1.0/cosmic_variance/cosmic_variance.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,42 +1,33 @@
-#rewritten by astrockragh (Christian Kragh Jespersen) to work in Python 3.8 (Jan-2023)
-#dependencies are numpy, scipy, and pandas
-#if anyone wants to optimize, the bottleneck is the intpk4 integral
+# Rewritten by Christian Kragh Jespersen, @astrockragh, to work in Python 3.8 (Jan-2023)
+# Dependencies are numpy, scipy, and pandas
+# If anyone (including future me) wants to optimize for speed, the bottleneck is the intpk4 integral
 
 
 import numpy as np
 import pandas as pd
-# from .quickcv import quickcv
 from .quickcv import quickcv
-import sys, os
+import os
 
-# if len( sys.argv ) == 2:
-#    name = str(sys.argv[1])
-# else:
-#    name = None
-#    print('Not saving output. To save, run the script with the name of the output file as an argument.')
+#### Sample parameter ####
 
 # ########### Input parameters ###########
 # s1 = 3.4/60 #side 1, in degrees 
 # s2 = 10.2/60 #side 2, in degrees
 # zarr = np.array([3,4,5,6.5]) #redshift bin edges
 # ############################################
 
 # ########### Cosmology ###########
 # OmegaM = 0.308
 # OmegaL = 0.692
-# sig8 = 0.82
+# sigma8 = 0.82
 # acc = 'low' # low takes about 20 seconds per calculation, high takes about 8 minutes per calculation
-
-##TODO - should include n_s, h, and w0 as well
-
 ############################################
 
-# The bias values for 7.0, 7.5, and 8.0 were incorrectly extrapolated 
-# set to be the same as for 8.5 in this version by astrockragh 19/11-2022
+# The bias values for 7.0, 7.5, and 8.0 were incorrectly extrapolated, here they are set to be the same as for 8.5 in this version by astrockragh 19/11-2022
 
 b070=0.062
 b170=2.59
 b270=1.025
 
 b075=0.062
 b175=2.59
@@ -66,45 +57,78 @@
 b1105=3.19
 b2105=1.269
 
 b0110=0.173
 b1110=2.89
 b2110=1.438
 
-def get_cv(side1, side2, zarr, name = None, OmegaM = 0.308, OmegaL = 0.692, sig8 = 0.82, acc = 'low'):
+def get_cv(side1, side2, zarr, name = None, dz = None, acc = 'low', OmegaM = 0.308, OmegaL = 0.692, OmegaBaryon = 0.022/(0.678)**2, sigma8 = 0.82, ns = 0.96, h = 0.678, verbose = False):
+   ''' Method to calculate the cosmic variance for a given survey area and redshift bins.
+      Give side lengths in degrees
+      side1: side length 1 [degrees]
+      side2: side length 2 [degrees]
+      zarr: array of redshift bin edges
+      name: name of the output file. File will be saved at dfs/name.csv if name is not None
+      dz: redshift bin size. If None, the redshift bin size will be the difference between the redshift bin edges. If dz is given, zarr is the redshift bin centers.
+      acc: accuracy of the calculation. 'low' or 'high'. 'low' is faster (20 sec per calculation), 'high' is more accurate (8 mins per calculation)
+      OmegaM, OmegaL, OmegaBaryon, sigma8, ns, h: cosmological parameters
+      verbose: whether to print out the time taken for the integral
+      
+      Output is dataframe with columns:
+      zmid: redshift bin center
+      dz: redshift bin size
+      cv_dm: cosmic variance for dark matter
+      cv_xx: cosmic variance for x.x - 0.25 < log(M_*/M_{sun}) < x.x + 0.25
+
+      if given name, the dataframe will be saved to dfs/name.csv, along with a df with metadata, dfs/name_meta.csv so that the runs don't have to be repeated
+      '''
 
    metadict = {'side1': side1,
             'side2': side2,
             'zarr': np.array(zarr),
+            'dz': dz,
+            'acc': acc,
             'OmegaM': OmegaM,
             'OmegaL': OmegaL,
-            'sig8': sig8,
-            'acc': acc}
+            'OmegaBaryon': OmegaBaryon, 
+            'sigma8': sigma8,
+            'ns': ns,
+            'h': h,
+            'verbose': verbose}
 
    df_meta = pd.DataFrame(metadict)
 
    nz = len(zarr)-1
 
    columns = ['zmid', 'dz', 'cv_dm', 'cv_70', "cv_75", "cv_80", "cv_85", "cv_90", "cv_95", "cv_100", "cv_105", "cv_110"]
    df_values = pd.DataFrame(index = np.arange(nz), columns = columns)
 
    for i in range(nz):
-      dz      = zarr[i+1]-zarr[i]
-      zmid    = zarr[i+1]+zarr[i]
-      zmid    = zmid/2
-      s       = quickcv.quickcv(side1, side2, np.array([zmid]), np.array([dz]), omegam = OmegaM, omegal = OmegaL, sig8 = sig8, acc = acc)
+      if dz is None:
+         dz      = zarr[i+1]-zarr[i]
+         zmid    = zarr[i+1]+zarr[i]
+         zmid    = zmid/2
+      else:
+         zmid    = zarr
+      
+      s       = quickcv.quickcv(side1, side2, np.array([zmid]), np.array([dz]), OmegaM = OmegaM, OmegaL = OmegaL, OmegaBaryon = OmegaBaryon, \
+                                sigma8 = sigma8, ns = ns, h = h, acc = acc, verbose = verbose)
+      
+      ## These are the linear bias values
       bias70  = b070  * (zmid+1)**b170  + b270
       bias75  = b075  * (zmid+1)**b175  + b275
       bias80  = b080  * (zmid+1)**b180  + b280
       bias85  = b085  * (zmid+1)**b185  + b285
       bias90  = b090  * (zmid+1)**b190  + b290
       bias95  = b095  * (zmid+1)**b195  + b295
       bias100 = b0100 * (zmid+1)**b1100 + b2100
       bias105 = b0105 * (zmid+1)**b1105 + b2105
       bias110 = b0110 * (zmid+1)**b1110 + b2110
+
+      ## All gg variables are galaxy-galaxy cosmic variance
       sgg70  = bias70  * s
       sgg75  = bias75  * s
       sgg80  = bias80  * s
       sgg85  = bias85  * s
       sgg90  = bias90  * s
       sgg95  = bias95  * s
       sgg100 = bias100 * s
@@ -120,9 +144,10 @@
          os.mkdir('dfs')
       print('Saving dataframes of values to dfs/' + name )
       print(df_values)
       df_values.to_csv('dfs/' + name + '.csv', index = False)
       df_meta.to_csv('dfs/' + name + '_meta' + '.csv', index = False)
    return df_values
 
-if __name__ == '__main__':
-   get_cv(3.4/60, 10.2/60, np.array([3,4,5,6.5]), name = 'test')
+## Sample use
+# if __name__ == '__main__':
+#    get_cv(3.4/60, 10.2/60, np.array([3,4,5,6.5]), name = 'test')
```

### Comparing `cosmic_variance-0.0.9/cosmic_variance/quickcv/quickcv.py` & `cosmic_variance-0.1.0/cosmic_variance/quickcv/quickcv.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,85 +1,85 @@
-# ;+
-# ; NAME:
-# ;
-# ;  QUICKCV
-# ;
-# ; PURPOSE:
-# ;
-# ;   calculate cosmic variance for some geometry
-# ;
-# ; CATEGORY:
-# ;
-# ;   cosmic variance
-# ;
-# ;
-# ; CALLING SEQUENCE:
-# ;
-# ;   fracerror=quickcv(side1,side2 [zarr,deltaz,sig8=sig8,npoints=npoints]) 
-# ;
-# ; INPUTS:
-# ;
-# ;   side1: length of 1 side of field on sky, in degrees (rect. geom)
-# ;   side2: length of other side of field on sky, in degrees
-# ;
-# ; OPTIONAL INPUTS:
-# ;   zarr: array of z's for which cosmic variance will be calculated; default:1
-# ;   deltaz: total length of volume in z direction; default: 0.1
-# ;
-# ; KEYWORD PARAMETERS:
-# ;   sig8: desired value of sigma_8; default: 0.77
-# ;   npoints: desired number of integration points for first part of 
-# ;     integration; default: 200
-# ;
-# ;
-# ; OUTPUTS:
-# ;
-# ;  fracerror: array containing the fractional error in a count,
-# ;  sigma/N, due to cosmic variance for objects with bias b=1 
-# ;  in a volume side1 x side2 degrees x delta_z centered at redshifts
-# ;  zarr.  NOTE THIS IS SIGMA, NOT VARIANCE!!!!
-# ;
-# ; RESTRICTIONS:
-# ;
-# ;  uses power spectrum in pofk.pro (gamma=0.1872, omega0=0.26), distance
-# ;  relation in rz.pro 
-# ;
-# ;
-# ; MODIFICATION HISTORY:
-# ; modified by rss july 2006 to include Dlin scaling with z
-# ; modified by bpm sep  2009 to wmap3 cosmology
-# ;-
+# +
+#  NAME:
+# 
+#   QUICKCV
+# 
+#  PURPOSE:
+# 
+#    calculate cosmic variance for some geometry
+# 
+#  CATEGORY:
+# 
+#    cosmic variance
+# 
+# 
+#  CALLING SEQUENCE:
+# 
+#    fracerror=quickcv(side1,side2 [zarr,deltaz,sig8=sig8,npoints=npoints]) 
+# 
+#  INPUTS:
+# 
+#    side1: length of 1 side of field on sky, in degrees (rect. geom)
+#    side2: length of other side of field on sky, in degrees
+# 
+#  OPTIONAL INPUTS:
+#    zarr: array of z's for which cosmic variance will be calculated default:1
+#    deltaz: total length of volume in z direction default: 0.1
+# 
+#  KEYWORD PARAMETERS:
+#    sig8: desired value of sigma_8 default: 0.77
+#    npoints: desired number of integration points for first part of 
+#      integration default: 200
+# 
+# 
+#  OUTPUTS:
+# 
+#   fracerror: array containing the fractional error in a count,
+#   sigma/N, due to cosmic variance for objects with bias b=1 
+#   in a volume side1 x side2 degrees x delta_z centered at redshifts
+#   zarr.  NOTE THIS IS SIGMA, NOT VARIANCE!!!!
+# 
+#  RESTRICTIONS:
+# 
+#   uses power spectrum in pofk.pro (gamma=0.1872, omega0=0.26), distance
+#   relation in rz.pro 
+# 
+# 
+#  MODIFICATION HISTORY:
+#  modified by rss july 2006 to include Dlin scaling with z
+#  modified by bpm sep  2009 to wmap3 cosmology
+# -
 
 import numpy as np
 from .utils.rz import rz
 from .utils.intpk4 import intpk4
 from .utils.dlin import Dlin
 
-def quickcv(side1,side2,za,deltaz, omegam = 0.31, omegal = 0.69, sig8=0.82, acc='low'):
+def quickcv(side1, side2, za, deltaz, OmegaM = 0.31, OmegaL = 0.69, OmegaBaryon = 0.022/(0.678)**2,sigma8 = 0.82, ns = 0.96, h = 0.678, verbose = False, acc='low'):
   """za and deltaz have to be np.arrays"""
   #sides in degrees, z is redshift bin middle, deltaz is redshift bin width, everything else is cosmology and integration parameters
   #see intpk4.py for acc options
 
   # assume LCDM
 
-  rza=rz(za, OmegaMatter=omegam, OmegaLambda=omegal)
-  rzmin=rz(za-deltaz/2, OmegaMatter=omegam, OmegaLambda=omegal)
-  rzmax=rz(za+deltaz/2, OmegaMatter=omegam, OmegaLambda=omegal)
+  rza=rz(za, OmegaM=OmegaM, OmegaL=OmegaL)
+  rzmin=rz(za-deltaz/2, OmegaM = OmegaM, OmegaL = OmegaL)
+  rzmax=rz(za+deltaz/2, OmegaM = OmegaM, OmegaL = OmegaL)
 
   radeg = 57.2958 # degrees per radians
 
   x1a=3000./2.*(rza * side1)/radeg
   x2a=3000./2.*(rza * side2)/radeg
   x3a=3000.*(rzmax-rzmin)/2.
   xs = np.array([x1a, x2a, x3a])
-  cvi = intpk4(xs, acc =  acc)
+  cvi = intpk4(xs, OmegaM = OmegaM, OmegaL = OmegaL, OmegaBaryon = OmegaBaryon, sigma8 = sigma8, ns = ns, h = h, acc =  acc, verbose =  verbose)
 
   #cvi is the fractional variance in a count in a rectangle
   #cvar is the fractional error (sigma), NOT VARIANCE
 
-  cvi = cvi*sig8**2 #normalize by sig8^2
-  d = Dlin(omegam, za)
+  cvi = cvi*sigma8**2 #normalize by sig8^2
+  d = Dlin(OmegaM, za)
   cvar = np.sqrt(cvi)*d
 
   return cvar[0]
 
 # print(quickcv(1,2, np.array([3]), np.array([1])))
```

### Comparing `cosmic_variance-0.0.9/cosmic_variance/quickcv/utils/intpk4.py` & `cosmic_variance-0.1.0/cosmic_variance/quickcv/utils/intpk4.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,16 +1,13 @@
 from .pofk import pofkint
 import numpy as np
 from scipy.integrate import nquad
-
 import time
 
-# xss = np.array([np.array([41.126813, 82.253627, 280.86420]), np.array([45.320475, 90.640949, 208.52065]), np.array([49.203843, 98.407686, 231.35671])]) #the unit is comoving megaparsec
-
-def intpk4(xs, acc = 'high', verbose = False):
+def intpk4(xs,  OmegaM = 0.308, OmegaBaryon = 0.022/(0.678)**2, sigma8 = 0.82, ns = 0.96, h = 0.678, acc = 'high', verbose = False):
 
 	"""" Solver for integral in equation 2 of https://arxiv.org/pdf/astro-ph/0109130.pdf
 	xs are the side lengths of the box in comoving Mpc
 	acc is the accuracy of the integral, 'high' or 'low', low is about 40 times faster and has about a 2% error
 	verbose is whether to print out the time taken for the integral
 
 	This version is written by Christian Kragh Jespersen, January 2023, rewritten from the IDL code by Jonathan Baker
@@ -25,19 +22,19 @@
 	kmax = (0.4+16/xs)*1.25 #this is to match from the idl code
 	kmax = kmax/acc
 
 	def window_idl(k0, k1, k2):
 		return np.sin(k0*xs[0])/(k0*xs[0])*np.sin(k1*xs[1])/(k1*xs[1])*np.sin(k2*xs[2])/(k2*xs[2]) 
 
 	def integrand_idl(k0,k1,k2):
-		return window_idl(k0, k1, k2)**2*pofkint(k0,k1,k2)
+		return window_idl(k0, k1, k2)**2*pofkint(k0,k1,k2,  OmegaM=OmegaM, OmegaBaryon=OmegaBaryon, sigma8=sigma8, ns = ns, h = h)
 
 	start = time.time()
 
 	integral = nquad(integrand_idl, [[0, kmax[0]], [0, kmax[1]], [0, kmax[2]]], opts = {"limlst": 10, "maxp1": 10})
 	end = time.time()
 
 	if verbose:
-		print(f'Integration time{end - start:.2f} seconds')
+		print(f'Integration time {end - start:.2f} seconds')
 
-	#factor of pi**3 is to normalize volume in k space, there are offsetting factors of 8 not included here
+	## factor of pi**3 is to normalize volume in k space, there are offsetting factors of 8 not included here
 	return integral[0]/np.pi**3
```

### Comparing `cosmic_variance-0.0.9/cosmic_variance/quickcv/utils/rz.py` & `cosmic_variance-0.1.0/cosmic_variance/quickcv/utils/rz.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,46 +1,36 @@
 
 
 # Routines for computing the Alcock-Paczynski distortion
 
 # January 2023, Christian Kragh Jespersen, rewritten from IDL
 
 
-#  H(z) in units where H(0) = 1
+# H(z) in units where H(0) = 1
 
 import numpy as np 
 from scipy.integrate import quad
 
-OmegaM = 0.308
-OmegaL = 0.692
-OmegaQ = 0.0
-wQ = 0.0
-eps = 1e-10
-
-def hubble(z):
+#get hubble parameter at redshift z relative to h at z=0
+def hubble(z, OmegaM = 0.308, OmegaL = 0.692):
     x = 1. + z
-    OmegaK = 1. - OmegaM - OmegaL - OmegaQ
-    h2 = OmegaM * x**3 + OmegaK * x**2 + OmegaL + OmegaQ * x**(3.+3.*wQ)
+    OmegaK = 1. - OmegaM - OmegaL #curvature.
+    h2 = OmegaM * x**3 + OmegaK * x**2 + OmegaL
     return np.sqrt(h2)
 
 # Compute d(chi)/dz where d(chi)^2 = dr^2 / (1-kr^2)
-
 def dchi_dz(z):
     return 1./hubble(z)
 
 # Compute coordinate distance r(z) for FRW metric
-
-def rz(z, OmegaMatter = OmegaM,
-            OmegaLambda = OmegaL,
-            OmegaQ = OmegaQ,
-            wQ = wQ,
-            eps = eps):
-    kurv = OmegaMatter + OmegaLambda + OmegaQ - 1.
+def rz(z, OmegaM = 0.308, OmegaL = 0.692, eps = 1e-10):
+    '''Compute coordinate distance r(z) for FRW metric, given cosmological parameters OmegaM and OmegaL and redshift z
+    eps parameter is the precision for scipy.integrate.quad'''
+    kurv = OmegaM + OmegaL - 1.
     nz = len(z)
-    # nz=1 
     dchi = np.zeros(nz)
     chi = np.zeros(nz)
     r = np.zeros(nz)
     z2 = z[0]
     if z2 == 0.:
         dchi[0] = 0.
     else:
@@ -54,10 +44,8 @@
         chi[i] = chi[i-1] + dchi[i]
     if abs(kurv) < 1.e-4: #flat
         r = chi
     elif kurv > 0.: #closed
         r = np.sin(chi*np.sqrt(kurv))/np.sqrt(kurv)
     else: #open
         r = np.sinh(chi*np.sqrt(-kurv))/np.sqrt(-kurv)
-    return r
-
-# print(rz([0,1]))
+    return r
```

### Comparing `cosmic_variance-0.0.9/cosmic_variance.egg-info/PKG-INFO` & `cosmic_variance-0.1.0/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,32 +1,25 @@
 Metadata-Version: 2.1
-Name: cosmic-variance
-Version: 0.0.9
-Summary: Package to calculate cosmic variance in pencil-beam surveys
-Home-page: https://github.com/astrockragh/pythonCV
+Name: cosmic_variance
+Version: 0.1.0
+Summary: Package to calculate cosmic variance in rectangular pencil-beam surveys
+Home-page: https://github.com/astrockragh/cosmic_variance
 Author: Christian Kragh Jespersen
 Author-email: ckragh@princeton.edu
 License: MIT license
 Description: ===============================
         Cosmic Variance Calculator
         ===============================
         
         Package to calculate cosmic variance in pencil-beam surveys
         ---------------------------------------------------------------------------
         
         .. image:: https://img.shields.io/pypi/v/cosmic_variance.svg
                 :target: https://pypi.python.org/pypi/cosmic_variance
         
-        .. image:: https://img.shields.io/travis/astrockragh/cosmic_variance.svg
-                :target: https://travis-ci.com/astrockragh/cosmic_variance
-        
-        .. image:: https://readthedocs.org/projects/cosmic-variance/badge/?version=latest
-                :target: https://cosmic-variance.readthedocs.io/en/latest/?version=latest
-                :alt: Documentation Status
-        
         
         Python package based on the IDL code released with the Cosmic Variance Cookbook of Moster et al. (2010)
         
         The code is based on galaxy stellar mass bins (as described in https://arxiv.org/pdf/1001.1737.pdf), scaled to dark matter cosmic variance (as described in https://arxiv.org/pdf/astro-ph/0109130.pdf). 
         
         This is significantly more useful than dark matter - only variance, since the empirical galaxy variance is significantly higher.
         
@@ -49,33 +42,38 @@
         
         The main use of the package is through the get_cv function, which takes in a rectangular survey geometry with side lengths side1 and side2 (in degrees), and an array of redshift bin edges, and returns a pandas dataframe with the cosmic variance for 0.5 dex galaxy stellar mass bins for each redshift bin.
         
         .. code-block:: python
         
                 import cosmic_variance as cv
                 import numpy as np
-                # use the main function, get_cv to calculate
+                # Example of using the main function, get_cv to calculate
                 # cosmic variance for a single JWST pointing
         
                 #### these arguments are required ####
                 side1 = 2.2/60. # /60 to convert from arcmin to degrees
                 side2 = 2*2.2/60. # /60 to convert from arcmin to degrees
                 zarray = np.array([7,8,9,11,13]) # redshift bin edges
         
                 #### these arguments are optional ####
-                name = 'JWST' # name of the survey, if provided, the output file will be saved as dfs/{name}.csv along with a meta file
+                name = 'JWST' # name of the survey, if provided, the output file will be saved as dfs/{name}.csv along with a meta file.
+                # Default is None, in which case the output will not be saved
+        
                 acc = 'low' # accuracy of the calculation, 'low' or 'high, low is default, faster and sufficient for almost all applications
         
+                verbose = False # if True, will print out the progress of the calculation, default is False
+        
                 #If you want to use a different cosmology, you can specify it by the following in the get_cv call
-                # OmegaM = 0.308, OmegaL = 0.692, sig8 = 0.82
+                # OmegaM = 0.308, OmegaL = 0.692, OmegaBaryon = 0.022/(0.678)**2 sigma8 = 0.82, ns = 0.96, h = 0.678
         
-                cv_df = cv.get_cv(side1, side2, zarray, name = name, acc=acc)
+                cv_df = cv.get_cv(side1, side2, zarray, name = name, acc=acc, verbose = verbose)
         
         This will calculate the cosmic variance for a 2.2 arcmin x 4.4 arcmin survey in redshifts bin [7, 8], [8,9], [9,11], [11,13] and save the output.
-Keywords: Cosmology,Galaxies,Statistics,AstrostatisticsCosmic Variance
+        
+Keywords: Cosmology,Galaxies,Statistics,Astrostatistics,Cosmic Variance
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
```

### Comparing `cosmic_variance-0.0.9/cosmic_variance.egg-info/SOURCES.txt` & `cosmic_variance-0.1.0/cosmic_variance.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cosmic_variance-0.0.9/docs/Makefile` & `cosmic_variance-0.1.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `cosmic_variance-0.0.9/docs/conf.py` & `cosmic_variance-0.1.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `cosmic_variance-0.0.9/docs/installation.rst` & `cosmic_variance-0.1.0/docs/installation.rst`

 * *Files identical despite different names*

### Comparing `cosmic_variance-0.0.9/docs/make.bat` & `cosmic_variance-0.1.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `cosmic_variance-0.0.9/setup.py` & `cosmic_variance-0.1.0/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -24,22 +24,22 @@
         'License :: OSI Approved :: MIT License',
         'Natural Language :: English',
         'Programming Language :: Python :: 3',
         'Programming Language :: Python :: 3.6',
         'Programming Language :: Python :: 3.7',
         'Programming Language :: Python :: 3.8',
     ],
-    description="Package to calculate cosmic variance in pencil-beam surveys",
+    description="Package to calculate cosmic variance in rectangular pencil-beam surveys",
     install_requires=requirements,
     license="MIT license",
     long_description = readme,
     long_description_content_type='text/x-rst',
     include_package_data = True,
-    keywords = ['Cosmology', 'Galaxies', 'Statistics', 'Astrostatistics' 'Cosmic Variance'],
+    keywords = ['Cosmology', 'Galaxies', 'Statistics', 'Astrostatistics', 'Cosmic Variance'],
     name = 'cosmic_variance',
     packages=find_packages(include=['cosmic_variance', 'cosmic_variance.*']),
     test_suite='tests',
     tests_require=test_requirements,
-    url='https://github.com/astrockragh/pythonCV', #change later
-    version='0.0.9',
+    url='https://github.com/astrockragh/cosmic_variance',
+    version='0.1.0',
     zip_safe=False,
 )
```

