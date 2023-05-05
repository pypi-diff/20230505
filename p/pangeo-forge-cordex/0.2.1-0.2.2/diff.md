# Comparing `tmp/pangeo-forge-cordex-0.2.1.tar.gz` & `tmp/pangeo-forge-cordex-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pangeo-forge-cordex-0.2.1.tar", last modified: Tue May  2 12:10:27 2023, max compression
+gzip compressed data, was "pangeo-forge-cordex-0.2.2.tar", last modified: Fri May  5 10:24:42 2023, max compression
```

## Comparing `pangeo-forge-cordex-0.2.1.tar` & `pangeo-forge-cordex-0.2.2.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 12:10:27.669967 pangeo-forge-cordex-0.2.1/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 12:10:27.665967 pangeo-forge-cordex-0.2.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 12:10:27.665967 pangeo-forge-cordex-0.2.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     2375 2023-05-02 12:10:17.000000 pangeo-forge-cordex-0.2.1/.github/workflows/ci.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      738 2023-05-02 12:10:17.000000 pangeo-forge-cordex-0.2.1/.github/workflows/release.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1831 2023-05-02 12:10:17.000000 pangeo-forge-cordex-0.2.1/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      475 2023-05-02 12:10:17.000000 pangeo-forge-cordex-0.2.1/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-05-02 12:10:17.000000 pangeo-forge-cordex-0.2.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1293 2023-05-02 12:10:27.669967 pangeo-forge-cordex-0.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      369 2023-05-02 12:10:17.000000 pangeo-forge-cordex-0.2.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 12:10:27.665967 pangeo-forge-cordex-0.2.1/ci/
--rw-r--r--   0 runner    (1001) docker     (123)      235 2023-05-02 12:10:17.000000 pangeo-forge-cordex-0.2.1/ci/environment.yml
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-05-02 12:10:17.000000 pangeo-forge-cordex-0.2.1/environment.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 12:10:27.665967 pangeo-forge-cordex-0.2.1/pangeo_forge_cordex/
--rw-r--r--   0 runner    (1001) docker     (123)      185 2023-05-02 12:10:17.000000 pangeo-forge-cordex-0.2.1/pangeo_forge_cordex/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-02 12:10:27.000000 pangeo-forge-cordex-0.2.1/pangeo_forge_cordex/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     2180 2023-05-02 12:10:17.000000 pangeo-forge-cordex-0.2.1/pangeo_forge_cordex/esgf_access.py
--rw-r--r--   0 runner    (1001) docker     (123)     5701 2023-05-02 12:10:17.000000 pangeo-forge-cordex-0.2.1/pangeo_forge_cordex/parsing.py
--rw-r--r--   0 runner    (1001) docker     (123)     2656 2023-05-02 12:10:17.000000 pangeo-forge-cordex-0.2.1/pangeo_forge_cordex/recipe.py
--rw-r--r--   0 runner    (1001) docker     (123)     1702 2023-05-02 12:10:17.000000 pangeo-forge-cordex-0.2.1/pangeo_forge_cordex/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 12:10:27.669967 pangeo-forge-cordex-0.2.1/pangeo_forge_cordex.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1293 2023-05-02 12:10:27.000000 pangeo-forge-cordex-0.2.1/pangeo_forge_cordex.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      689 2023-05-02 12:10:27.000000 pangeo-forge-cordex-0.2.1/pangeo_forge_cordex.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-02 12:10:27.000000 pangeo-forge-cordex-0.2.1/pangeo_forge_cordex.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-02 12:10:27.000000 pangeo-forge-cordex-0.2.1/pangeo_forge_cordex.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-02 12:10:27.000000 pangeo-forge-cordex-0.2.1/pangeo_forge_cordex.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-05-02 12:10:27.000000 pangeo-forge-cordex-0.2.1/pangeo_forge_cordex.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      426 2023-05-02 12:10:17.000000 pangeo-forge-cordex-0.2.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-05-02 12:10:17.000000 pangeo-forge-cordex-0.2.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1343 2023-05-02 12:10:27.669967 pangeo-forge-cordex-0.2.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-02 12:10:17.000000 pangeo-forge-cordex-0.2.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 12:10:27.669967 pangeo-forge-cordex-0.2.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-02 12:10:17.000000 pangeo-forge-cordex-0.2.1/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      951 2023-05-02 12:10:17.000000 pangeo-forge-cordex-0.2.1/tests/test_recipe_creation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 10:24:42.415635 pangeo-forge-cordex-0.2.2/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 10:24:42.411635 pangeo-forge-cordex-0.2.2/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 10:24:42.415635 pangeo-forge-cordex-0.2.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     2375 2023-05-05 10:24:32.000000 pangeo-forge-cordex-0.2.2/.github/workflows/ci.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      738 2023-05-05 10:24:32.000000 pangeo-forge-cordex-0.2.2/.github/workflows/release.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1831 2023-05-05 10:24:32.000000 pangeo-forge-cordex-0.2.2/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      475 2023-05-05 10:24:32.000000 pangeo-forge-cordex-0.2.2/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-05-05 10:24:32.000000 pangeo-forge-cordex-0.2.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1293 2023-05-05 10:24:42.415635 pangeo-forge-cordex-0.2.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      369 2023-05-05 10:24:32.000000 pangeo-forge-cordex-0.2.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 10:24:42.415635 pangeo-forge-cordex-0.2.2/ci/
+-rw-r--r--   0 runner    (1001) docker     (123)      235 2023-05-05 10:24:32.000000 pangeo-forge-cordex-0.2.2/ci/environment.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-05-05 10:24:32.000000 pangeo-forge-cordex-0.2.2/environment.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 10:24:42.415635 pangeo-forge-cordex-0.2.2/pangeo_forge_cordex/
+-rw-r--r--   0 runner    (1001) docker     (123)      185 2023-05-05 10:24:32.000000 pangeo-forge-cordex-0.2.2/pangeo_forge_cordex/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-05 10:24:42.000000 pangeo-forge-cordex-0.2.2/pangeo_forge_cordex/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2176 2023-05-05 10:24:32.000000 pangeo-forge-cordex-0.2.2/pangeo_forge_cordex/esgf_access.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5701 2023-05-05 10:24:32.000000 pangeo-forge-cordex-0.2.2/pangeo_forge_cordex/parsing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2665 2023-05-05 10:24:32.000000 pangeo-forge-cordex-0.2.2/pangeo_forge_cordex/recipe.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1702 2023-05-05 10:24:32.000000 pangeo-forge-cordex-0.2.2/pangeo_forge_cordex/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 10:24:42.415635 pangeo-forge-cordex-0.2.2/pangeo_forge_cordex.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1293 2023-05-05 10:24:42.000000 pangeo-forge-cordex-0.2.2/pangeo_forge_cordex.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      689 2023-05-05 10:24:42.000000 pangeo-forge-cordex-0.2.2/pangeo_forge_cordex.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 10:24:42.000000 pangeo-forge-cordex-0.2.2/pangeo_forge_cordex.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 10:24:42.000000 pangeo-forge-cordex-0.2.2/pangeo_forge_cordex.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-05 10:24:42.000000 pangeo-forge-cordex-0.2.2/pangeo_forge_cordex.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-05-05 10:24:42.000000 pangeo-forge-cordex-0.2.2/pangeo_forge_cordex.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      426 2023-05-05 10:24:32.000000 pangeo-forge-cordex-0.2.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-05-05 10:24:32.000000 pangeo-forge-cordex-0.2.2/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1343 2023-05-05 10:24:42.415635 pangeo-forge-cordex-0.2.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-05 10:24:32.000000 pangeo-forge-cordex-0.2.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 10:24:42.415635 pangeo-forge-cordex-0.2.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 10:24:32.000000 pangeo-forge-cordex-0.2.2/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1105 2023-05-05 10:24:32.000000 pangeo-forge-cordex-0.2.2/tests/test_recipe_creation.py
```

### Comparing `pangeo-forge-cordex-0.2.1/.github/workflows/ci.yaml` & `pangeo-forge-cordex-0.2.2/.github/workflows/ci.yaml`

 * *Files identical despite different names*

### Comparing `pangeo-forge-cordex-0.2.1/.github/workflows/release.yaml` & `pangeo-forge-cordex-0.2.2/.github/workflows/release.yaml`

 * *Files identical despite different names*

### Comparing `pangeo-forge-cordex-0.2.1/.gitignore` & `pangeo-forge-cordex-0.2.2/.gitignore`

 * *Files identical despite different names*

### Comparing `pangeo-forge-cordex-0.2.1/LICENSE` & `pangeo-forge-cordex-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pangeo-forge-cordex-0.2.1/PKG-INFO` & `pangeo-forge-cordex-0.2.2/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pangeo-forge-cordex
-Version: 0.2.1
+Version: 0.2.2
 Summary: "Using queries to the ESGF API to generate urls and keyword arguments for receipe generation in pangeo-forge"
 Home-page: https://github.com/euro-cordex/pangeo-forge-cordex
 Maintainer: Lars Buntemeyer
 Maintainer-email: lars.buntemeyer@hereon.de
 License: MIT
 Keywords: pangeo,data,esgf
 Classifier: Development Status :: 1 - Planning
```

### Comparing `pangeo-forge-cordex-0.2.1/pangeo_forge_cordex/esgf_access.py` & `pangeo-forge-cordex-0.2.2/pangeo_forge_cordex/esgf_access.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import requests
 
 from .utils import combine_response, parse_dataset_response, sort_files_by_dataset_id
 
 
 def logon():
     from pyesgf.logon import LogonManager
-    
+
     lm = LogonManager(verify=True)
     if not lm.is_logged_on():
         myproxy_host = "esgf-data.dkrz.de"
         # if we find those in environment, use them.
         if "ESGF_USER" in os.environ and "ESGF_PASSWORD" in os.environ:
             lm.logon(
                 hostname=myproxy_host,
```

### Comparing `pangeo-forge-cordex-0.2.1/pangeo_forge_cordex/parsing.py` & `pangeo-forge-cordex-0.2.2/pangeo_forge_cordex/parsing.py`

 * *Files identical despite different names*

### Comparing `pangeo-forge-cordex-0.2.1/pangeo_forge_cordex/recipe.py` & `pangeo-forge-cordex-0.2.2/pangeo_forge_cordex/recipe.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,15 @@
-import fsspec
-import pandas as pd
-import xarray as xr
-
 from .esgf_access import esgf_search
 from .parsing import facets_from_iid
 from .utils import freq_map
 
 
 def number_of_timesteps(dset):
+    import pandas as pd
+
     start = dset["datetime_start"]
     stop = dset["datetime_stop"]
     cf_freq = dset["time_frequency"][0]
     ntime = pd.date_range(start, stop, freq=freq_map[cf_freq]).size
     print(f"Found {ntime} timesteps!")
     return ntime
 
@@ -26,14 +24,17 @@
 
     Estimate time chunksize from the size of the
     first timestep in the dataset and the total number
     of timesteps defined by the frequency, datetime_start
     and datetime_stop.
 
     """
+    import fsspec
+    import xarray as xr
+
     ntime = number_of_timesteps(dset)
     var = dset["variable"][0]
     print(url)
     if url:
         fs = fsspec.filesystem("https")
         with xr.open_dataset(fs.open(url, ssl=ssl)) as ds:
             size = ds[var].isel(time=0).nbytes * ntime
@@ -72,15 +73,15 @@
 
     return create_recipe_inputs(dset_responses, ssl)
 
 
 def create_recipe(urls, recipe_kwargs=None, pattern_kwargs=None):
     from pangeo_forge_recipes.patterns import pattern_from_file_sequence
     from pangeo_forge_recipes.recipes import XarrayZarrRecipe
-    
+
     if recipe_kwargs is None:
         recipe_kwargs = {}
     if pattern_kwargs is None:
         pattern_kwargs = {}
     pattern = pattern_from_file_sequence(urls, "time", **pattern_kwargs)
     if urls is not None:
         return XarrayZarrRecipe(
```

### Comparing `pangeo-forge-cordex-0.2.1/pangeo_forge_cordex/utils.py` & `pangeo-forge-cordex-0.2.2/pangeo_forge_cordex/utils.py`

 * *Files identical despite different names*

### Comparing `pangeo-forge-cordex-0.2.1/pangeo_forge_cordex.egg-info/PKG-INFO` & `pangeo-forge-cordex-0.2.2/pangeo_forge_cordex.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pangeo-forge-cordex
-Version: 0.2.1
+Version: 0.2.2
 Summary: "Using queries to the ESGF API to generate urls and keyword arguments for receipe generation in pangeo-forge"
 Home-page: https://github.com/euro-cordex/pangeo-forge-cordex
 Maintainer: Lars Buntemeyer
 Maintainer-email: lars.buntemeyer@hereon.de
 License: MIT
 Keywords: pangeo,data,esgf
 Classifier: Development Status :: 1 - Planning
```

### Comparing `pangeo-forge-cordex-0.2.1/pangeo_forge_cordex.egg-info/SOURCES.txt` & `pangeo-forge-cordex-0.2.2/pangeo_forge_cordex.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pangeo-forge-cordex-0.2.1/setup.cfg` & `pangeo-forge-cordex-0.2.2/setup.cfg`

 * *Files identical despite different names*

### Comparing `pangeo-forge-cordex-0.2.1/tests/test_recipe_creation.py` & `pangeo-forge-cordex-0.2.2/tests/test_recipe_creation.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,16 +1,22 @@
+import pytest
 import xarray as xr
 from pangeo_forge_recipes.patterns import pattern_from_file_sequence
 from pangeo_forge_recipes.recipes import XarrayZarrRecipe
 
 from pangeo_forge_cordex import logon, recipe_inputs_from_iids
 
+iids = [
+    "cordex.output.EUR-11.DMI.ECMWF-ERAINT.evaluation.r1i1p1.HIRHAM5.v1.mon.tas.v20140620",
+    "cordex.output.EUR-11.GERICS.ECMWF-ERAINT.evaluation.r1i1p1.REMO2015.v1.day.tas.v20180813",
+]
 
-def test_recipe_inputs():
-    iid = "cordex.output.EUR-11.GERICS.ECMWF-ERAINT.evaluation.r1i1p1.REMO2015.v1.mon.tas.v20180813"
+
+@pytest.mark.parametrize("iid", iids)
+def test_recipe_inputs(iid):
     sslcontext = logon()
 
     recipe_inputs = recipe_inputs_from_iids(iid, sslcontext)
 
     urls = recipe_inputs[iid]["urls"]
     recipe_kwargs = recipe_inputs[iid]["recipe_kwargs"]
     pattern_kwargs = recipe_inputs[iid]["pattern_kwargs"]
```

