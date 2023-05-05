# Comparing `tmp/sdmbc-0.1.tar.gz` & `tmp/sdmbc-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sdmbc-0.1.tar", last modified: Fri May  5 01:43:54 2023, max compression
+gzip compressed data, was "sdmbc-0.1.1.tar", last modified: Fri May  5 08:32:45 2023, max compression
```

## Comparing `sdmbc-0.1.tar` & `sdmbc-0.1.1.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 z5239661 (15239661) unsw      (5000)        0 2023-05-05 01:43:54.328585 sdmbc-0.1/
--rw-r--r--   0 z5239661 (15239661) unsw      (5000)     1068 2023-05-03 01:08:47.000000 sdmbc-0.1/LICENSE
--rw-r--r--   0 z5239661 (15239661) unsw      (5000)      670 2023-05-05 01:43:54.326584 sdmbc-0.1/PKG-INFO
--rw-r--r--   0 z5239661 (15239661) unsw      (5000)      138 2023-05-03 01:08:47.000000 sdmbc-0.1/README.md
-drwxr-xr-x   0 z5239661 (15239661) unsw      (5000)        0 2023-05-05 01:43:54.295584 sdmbc-0.1/sdmbc/
--rw-r--r--   0 z5239661 (15239661) unsw      (5000)       94 2023-05-03 08:16:04.000000 sdmbc-0.1/sdmbc/__init__.py
--rw-r--r--   0 z5239661 (15239661) unsw      (5000)     8482 2023-05-03 12:40:10.000000 sdmbc-0.1/sdmbc/analysis_plot.py
--rw-r--r--   0 z5239661 (15239661) unsw      (5000)     9555 2023-05-03 12:40:20.000000 sdmbc-0.1/sdmbc/bias_correction.py
--rw-r--r--   0 z5239661 (15239661) unsw      (5000)    23687 2023-05-03 12:39:54.000000 sdmbc-0.1/sdmbc/figurefunction.py
--rwxr-xr-x   0 z5239661 (15239661) unsw      (5000)   151600 2023-05-03 00:53:50.000000 sdmbc-0.1/sdmbc/main_biascorrection.exe
--rw-r--r--   0 z5239661 (15239661) unsw      (5000)    14217 2023-05-03 12:40:00.000000 sdmbc-0.1/sdmbc/output_reformatter.py
--rw-r--r--   0 z5239661 (15239661) unsw      (5000)     3661 2023-05-03 08:38:09.000000 sdmbc-0.1/sdmbc/user_input.py
-drwxr-xr-x   0 z5239661 (15239661) unsw      (5000)        0 2023-05-05 01:43:54.309584 sdmbc-0.1/sdmbc.egg-info/
--rw-r--r--   0 z5239661 (15239661) unsw      (5000)      670 2023-05-05 01:43:53.000000 sdmbc-0.1/sdmbc.egg-info/PKG-INFO
--rw-r--r--   0 z5239661 (15239661) unsw      (5000)      456 2023-05-05 01:43:53.000000 sdmbc-0.1/sdmbc.egg-info/SOURCES.txt
--rw-r--r--   0 z5239661 (15239661) unsw      (5000)        1 2023-05-05 01:43:53.000000 sdmbc-0.1/sdmbc.egg-info/dependency_links.txt
--rw-r--r--   0 z5239661 (15239661) unsw      (5000)     1859 2023-05-05 01:43:53.000000 sdmbc-0.1/sdmbc.egg-info/requires.txt
--rw-r--r--   0 z5239661 (15239661) unsw      (5000)       12 2023-05-05 01:43:53.000000 sdmbc-0.1/sdmbc.egg-info/top_level.txt
--rw-r--r--   0 z5239661 (15239661) unsw      (5000)       38 2023-05-05 01:43:54.328585 sdmbc-0.1/setup.cfg
--rw-r--r--   0 z5239661 (15239661) unsw      (5000)      991 2023-05-03 01:05:50.000000 sdmbc-0.1/setup.py
-drwxr-xr-x   0 z5239661 (15239661) unsw      (5000)        0 2023-05-05 01:43:54.323584 sdmbc-0.1/tests/
--rw-r--r--   0 z5239661 (15239661) unsw      (5000)       56 2023-05-03 01:27:31.000000 sdmbc-0.1/tests/__init__.py
--rw-r--r--   0 z5239661 (15239661) unsw      (5000)     8475 2023-05-03 01:26:45.000000 sdmbc-0.1/tests/analysis_plot.py
--rw-r--r--   0 z5239661 (15239661) unsw      (5000)     9543 2023-05-03 01:26:45.000000 sdmbc-0.1/tests/bias_correction.py
--rw-r--r--   0 z5239661 (15239661) unsw      (5000)    23797 2023-05-03 01:26:45.000000 sdmbc-0.1/tests/figurefunction.py
--rw-r--r--   0 z5239661 (15239661) unsw      (5000)    14217 2023-05-03 01:26:45.000000 sdmbc-0.1/tests/output_reformatter.py
+drwxr-xr-x   0 z5239661 (15239661) unsw      (5000)        0 2023-05-05 08:32:45.130835 sdmbc-0.1.1/
+-rw-r--r--   0 z5239661 (15239661) unsw      (5000)     1068 2023-05-03 01:08:47.000000 sdmbc-0.1.1/LICENSE
+-rw-r--r--   0 z5239661 (15239661) unsw      (5000)     8345 2023-05-05 08:32:45.129835 sdmbc-0.1.1/PKG-INFO
+-rw-r--r--   0 z5239661 (15239661) unsw      (5000)     7771 2023-05-05 08:27:19.000000 sdmbc-0.1.1/README.md
+drwxr-xr-x   0 z5239661 (15239661) unsw      (5000)        0 2023-05-05 08:32:45.094834 sdmbc-0.1.1/sdmbc/
+-rw-r--r--   0 z5239661 (15239661) unsw      (5000)       94 2023-05-03 08:16:04.000000 sdmbc-0.1.1/sdmbc/__init__.py
+-rw-r--r--   0 z5239661 (15239661) unsw      (5000)     8578 2023-05-05 07:25:45.000000 sdmbc-0.1.1/sdmbc/analysis_plot.py
+-rw-r--r--   0 z5239661 (15239661) unsw      (5000)     9609 2023-05-05 07:14:57.000000 sdmbc-0.1.1/sdmbc/bias_correction.py
+-rw-r--r--   0 z5239661 (15239661) unsw      (5000)    23687 2023-05-03 12:39:54.000000 sdmbc-0.1.1/sdmbc/figurefunction.py
+-rwxr-xr-x   0 z5239661 (15239661) unsw      (5000)   151600 2023-05-03 00:53:50.000000 sdmbc-0.1.1/sdmbc/main_biascorrection.exe
+-rw-r--r--   0 z5239661 (15239661) unsw      (5000)    14217 2023-05-03 12:40:00.000000 sdmbc-0.1.1/sdmbc/output_reformatter.py
+-rw-r--r--   0 z5239661 (15239661) unsw      (5000)     3661 2023-05-03 08:38:09.000000 sdmbc-0.1.1/sdmbc/user_input.py
+drwxr-xr-x   0 z5239661 (15239661) unsw      (5000)        0 2023-05-05 08:32:45.109835 sdmbc-0.1.1/sdmbc.egg-info/
+-rw-r--r--   0 z5239661 (15239661) unsw      (5000)     8345 2023-05-05 08:32:44.000000 sdmbc-0.1.1/sdmbc.egg-info/PKG-INFO
+-rw-r--r--   0 z5239661 (15239661) unsw      (5000)      456 2023-05-05 08:32:44.000000 sdmbc-0.1.1/sdmbc.egg-info/SOURCES.txt
+-rw-r--r--   0 z5239661 (15239661) unsw      (5000)        1 2023-05-05 08:32:44.000000 sdmbc-0.1.1/sdmbc.egg-info/dependency_links.txt
+-rw-r--r--   0 z5239661 (15239661) unsw      (5000)     1859 2023-05-05 08:32:44.000000 sdmbc-0.1.1/sdmbc.egg-info/requires.txt
+-rw-r--r--   0 z5239661 (15239661) unsw      (5000)       12 2023-05-05 08:32:44.000000 sdmbc-0.1.1/sdmbc.egg-info/top_level.txt
+-rw-r--r--   0 z5239661 (15239661) unsw      (5000)       38 2023-05-05 08:32:45.131835 sdmbc-0.1.1/setup.cfg
+-rw-r--r--   0 z5239661 (15239661) unsw      (5000)     1125 2023-05-05 08:32:12.000000 sdmbc-0.1.1/setup.py
+drwxr-xr-x   0 z5239661 (15239661) unsw      (5000)        0 2023-05-05 08:32:45.126835 sdmbc-0.1.1/tests/
+-rw-r--r--   0 z5239661 (15239661) unsw      (5000)       56 2023-05-03 01:27:31.000000 sdmbc-0.1.1/tests/__init__.py
+-rw-r--r--   0 z5239661 (15239661) unsw      (5000)     8475 2023-05-03 01:26:45.000000 sdmbc-0.1.1/tests/analysis_plot.py
+-rw-r--r--   0 z5239661 (15239661) unsw      (5000)     9543 2023-05-03 01:26:45.000000 sdmbc-0.1.1/tests/bias_correction.py
+-rw-r--r--   0 z5239661 (15239661) unsw      (5000)    23797 2023-05-03 01:26:45.000000 sdmbc-0.1.1/tests/figurefunction.py
+-rw-r--r--   0 z5239661 (15239661) unsw      (5000)    14217 2023-05-03 01:26:45.000000 sdmbc-0.1.1/tests/output_reformatter.py
```

### Comparing `sdmbc-0.1/LICENSE` & `sdmbc-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `sdmbc-0.1/sdmbc/analysis_plot.py` & `sdmbc-0.1.1/tests/analysis_plot.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 import pytest
 import numpy as np
 import xarray as xr
 import pandas as pd
 from scipy.stats import ks_2samp
 
 from user_input import *
-from sdmbc.figurefunction import (
+from figurefunction import (
     assign_w,
     save_figure_3d,
     save_figure_3d_cross,
     save_figure_surface,
     rounder,
     calculate_ks_matrix,
 )
@@ -170,15 +170,15 @@
 
         self.dgcm_sst = xr.open_dataset(f"{self.bc_path}{input_gcm_sst}")
         self.dobs_sst = xr.open_dataset(f"{self.bc_path}{input_obs_sst}")
         self.dbcd_sst = xr.open_dataset(f"{self.bc_path}{input_bcd_sst}")
 
         # Reformat time
         times = pd.date_range(
-            "%s-01-01" % (self.startyear), freq="6H", periods=len(self.dgcm_sst.time)
+            "%s-01-01" % (self.startyear), freq="6H", periods=len(self.dgcm_3d.time)
         )
 
         self.dgcm_sst = self.dgcm_sst.update({"time": times})
         self.dobs_sst = self.dobs_sst.update({"time": times})
         self.dbcd_sst = self.dbcd_sst.update({"time": times})
 
         # Add coordinates
```

### Comparing `sdmbc-0.1/sdmbc/bias_correction.py` & `sdmbc-0.1.1/tests/bias_correction.py`

 * *Files 0% similar despite different names*

```diff
@@ -34,16 +34,16 @@
 # 2023-03-20
 #
 # =======================================================================================
 import pytest
 import xarray as xr
 from user_input import *
 import subprocess
-from sdmbc.analysis_plot import AnalysisBC
-from sdmbc.output_reformatter import reformat_and_save_3d, reformat_and_save_2d
+from analysis_plot import AnalysisBC
+from output_reformatter import reformat_and_save_3d, reformat_and_save_2d
 
 
 class BiasCorrection:
     """
     A class to handle bias correction of climate variables.
 
     Attributes:
```

### Comparing `sdmbc-0.1/sdmbc/figurefunction.py` & `sdmbc-0.1.1/sdmbc/figurefunction.py`

 * *Files identical despite different names*

### Comparing `sdmbc-0.1/sdmbc/main_biascorrection.exe` & `sdmbc-0.1.1/sdmbc/main_biascorrection.exe`

 * *Files identical despite different names*

### Comparing `sdmbc-0.1/sdmbc/output_reformatter.py` & `sdmbc-0.1.1/sdmbc/output_reformatter.py`

 * *Files identical despite different names*

### Comparing `sdmbc-0.1/sdmbc/user_input.py` & `sdmbc-0.1.1/sdmbc/user_input.py`

 * *Files identical despite different names*

### Comparing `sdmbc-0.1/sdmbc.egg-info/requires.txt` & `sdmbc-0.1.1/sdmbc.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `sdmbc-0.1/setup.py` & `sdmbc-0.1.1/setup.py`

 * *Files 23% similar despite different names*

```diff
@@ -2,23 +2,27 @@
 
 with open("requirements.txt") as f:
     install_requires = f.read().splitlines()
 
 with open("requirements_doc.txt") as f:
     docs_requires = f.read().splitlines()
     
+with open('README.md', 'r', encoding='utf-8') as f:
+    long_description = f.read()
+    
 setup(
     name="sdmbc",
-    version="0.1",
+    version="0.1.1",
     description="Sub-Daily Multivariate Bias Correction (SDMBC)",
     author="Youngil Kim",
     author_email="youngil.kim@student.unsw.edu.au",
     packages=find_packages(),
     license='LICENSE',
-    long_description=open('README.md').read(),
+    long_description=long_description,
+    long_description_content_type='text/markdown',
     install_requires=install_requires,
     extras_require={
       'documentation': docs_requires
     },
     classifiers=[
         "Development Status :: 3 - Alpha",
         "License :: OSI Approved :: MIT License",
```

### Comparing `sdmbc-0.1/tests/analysis_plot.py` & `sdmbc-0.1.1/sdmbc/analysis_plot.py`

 * *Files 4% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 import pytest
 import numpy as np
 import xarray as xr
 import pandas as pd
 from scipy.stats import ks_2samp
 
 from user_input import *
-from figurefunction import (
+from sdmbc.figurefunction import (
     assign_w,
     save_figure_3d,
     save_figure_3d_cross,
     save_figure_surface,
     rounder,
     calculate_ks_matrix,
 )
@@ -57,39 +57,40 @@
         The path to save output figures.
     kstest : bool, optional
         If True, the Kolmogorov-Smirnov (K-S) test will be performed,
         otherwise not. Default is False.
     """
 
     def __init__(
-        self, bc_path, lat_range, lon_range, startyear, out_figure_path, kstest=False
+        self, bc_path, level, lat_range, lon_range, startyear, out_figure_path, kstest=False
     ):
         self.bc_path = bc_path
+        self.level = level
         self.lat_range = lat_range
         self.lon_range = lon_range
         self.startyear = startyear
         self.out_figure_path = out_figure_path
         self.kstest = kstest
 
     def figure_atmos(self):
         """
         Analyzes atmospheric variables and generates plots for bias-corrected data.
         Saves scatter plots of mean, standard deviation, and lag1 auto-correlation
         for the atmospheric variables, as well as cross-correlation between them.
         Optionally, it can also perform the Kolmogorov-Smirnov (K-S) test
         and print the results.
         """
-
-        input_gcm_3d = "3d.gcm.1.input.nc"
-        input_obs_3d = "3d.obs.1.input.nc"
-        input_bcd_3d = "3d.bcd.1.output.nc"
-
-        self.dgcm_3d = xr.open_dataset(f"{self.bc_path}{input_gcm_3d}")
-        self.dobs_3d = xr.open_dataset(f"{self.bc_path}{input_obs_3d}")
-        self.dbcd_3d = xr.open_dataset(f"{self.bc_path}{input_bcd_3d}")
+        
+        input_gcm_3d = self.bc_path + "3d.gcm." + str(self.level) + ".input.nc"
+        input_obs_3d = self.bc_path + "3d.obs." + str(self.level) + ".input.nc"
+        input_bcd_3d = self.bc_path + "3d.bcd." + str(self.level) + ".output.nc"
+
+        self.dgcm_3d = xr.open_dataset(input_gcm_3d)
+        self.dobs_3d = xr.open_dataset(input_obs_3d)
+        self.dbcd_3d = xr.open_dataset(input_bcd_3d)
 
         # Reformat time
         times = pd.date_range(
             "%s-01-01" % (self.startyear), freq="6H", periods=len(self.dgcm_3d.time)
         )
 
         self.dgcm_3d = self.dgcm_3d.update({"time": times})
@@ -170,15 +171,15 @@
 
         self.dgcm_sst = xr.open_dataset(f"{self.bc_path}{input_gcm_sst}")
         self.dobs_sst = xr.open_dataset(f"{self.bc_path}{input_obs_sst}")
         self.dbcd_sst = xr.open_dataset(f"{self.bc_path}{input_bcd_sst}")
 
         # Reformat time
         times = pd.date_range(
-            "%s-01-01" % (self.startyear), freq="6H", periods=len(self.dgcm_3d.time)
+            "%s-01-01" % (self.startyear), freq="6H", periods=len(self.dgcm_sst.time)
         )
 
         self.dgcm_sst = self.dgcm_sst.update({"time": times})
         self.dobs_sst = self.dobs_sst.update({"time": times})
         self.dbcd_sst = self.dbcd_sst.update({"time": times})
 
         # Add coordinates
```

### Comparing `sdmbc-0.1/tests/bias_correction.py` & `sdmbc-0.1.1/sdmbc/bias_correction.py`

 * *Files 0% similar despite different names*

```diff
@@ -34,16 +34,16 @@
 # 2023-03-20
 #
 # =======================================================================================
 import pytest
 import xarray as xr
 from user_input import *
 import subprocess
-from analysis_plot import AnalysisBC
-from output_reformatter import reformat_and_save_3d, reformat_and_save_2d
+from sdmbc.analysis_plot import AnalysisBC
+from sdmbc.output_reformatter import reformat_and_save_3d, reformat_and_save_2d
 
 
 class BiasCorrection:
     """
     A class to handle bias correction of climate variables.
 
     Attributes:
@@ -194,24 +194,26 @@
 
         if self.figure == 1:
             print("Drawing figures")
             if self.sub_daily_correction == 1:
                 print("K-S test has been included")
                 statistics = AnalysisBC(
                     bc_path,
+                    level,
                     lat_range,
                     lon_range,
                     startyear,
                     out_figure_path,
                     kstest=True,
                 )
             if self.sub_daily_correction == 0:
                 print("K-S test has not been included")
                 statistics = AnalysisBC(
                     bc_path,
+                    level,
                     lat_range,
                     lon_range,
                     startyear,
                     out_figure_path,
                     kstest=False,
                 )
             statistics.figure_atmos()
```

### Comparing `sdmbc-0.1/tests/figurefunction.py` & `sdmbc-0.1.1/tests/figurefunction.py`

 * *Files identical despite different names*

### Comparing `sdmbc-0.1/tests/output_reformatter.py` & `sdmbc-0.1.1/tests/output_reformatter.py`

 * *Files identical despite different names*

