# Comparing `tmp/pangeo-forge-cordex-0.2.2.tar.gz` & `tmp/pangeo-forge-cordex-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pangeo-forge-cordex-0.2.2.tar", last modified: Fri May  5 10:24:42 2023, max compression
+gzip compressed data, was "pangeo-forge-cordex-0.2.3.tar", last modified: Fri May  5 12:29:24 2023, max compression
```

## Comparing `pangeo-forge-cordex-0.2.2.tar` & `pangeo-forge-cordex-0.2.3.tar`

### file list

```diff
@@ -1,34 +1,35 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 10:24:42.415635 pangeo-forge-cordex-0.2.2/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 10:24:42.411635 pangeo-forge-cordex-0.2.2/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 10:24:42.415635 pangeo-forge-cordex-0.2.2/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     2375 2023-05-05 10:24:32.000000 pangeo-forge-cordex-0.2.2/.github/workflows/ci.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      738 2023-05-05 10:24:32.000000 pangeo-forge-cordex-0.2.2/.github/workflows/release.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1831 2023-05-05 10:24:32.000000 pangeo-forge-cordex-0.2.2/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      475 2023-05-05 10:24:32.000000 pangeo-forge-cordex-0.2.2/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-05-05 10:24:32.000000 pangeo-forge-cordex-0.2.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1293 2023-05-05 10:24:42.415635 pangeo-forge-cordex-0.2.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      369 2023-05-05 10:24:32.000000 pangeo-forge-cordex-0.2.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 10:24:42.415635 pangeo-forge-cordex-0.2.2/ci/
--rw-r--r--   0 runner    (1001) docker     (123)      235 2023-05-05 10:24:32.000000 pangeo-forge-cordex-0.2.2/ci/environment.yml
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-05-05 10:24:32.000000 pangeo-forge-cordex-0.2.2/environment.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 10:24:42.415635 pangeo-forge-cordex-0.2.2/pangeo_forge_cordex/
--rw-r--r--   0 runner    (1001) docker     (123)      185 2023-05-05 10:24:32.000000 pangeo-forge-cordex-0.2.2/pangeo_forge_cordex/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-05 10:24:42.000000 pangeo-forge-cordex-0.2.2/pangeo_forge_cordex/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     2176 2023-05-05 10:24:32.000000 pangeo-forge-cordex-0.2.2/pangeo_forge_cordex/esgf_access.py
--rw-r--r--   0 runner    (1001) docker     (123)     5701 2023-05-05 10:24:32.000000 pangeo-forge-cordex-0.2.2/pangeo_forge_cordex/parsing.py
--rw-r--r--   0 runner    (1001) docker     (123)     2665 2023-05-05 10:24:32.000000 pangeo-forge-cordex-0.2.2/pangeo_forge_cordex/recipe.py
--rw-r--r--   0 runner    (1001) docker     (123)     1702 2023-05-05 10:24:32.000000 pangeo-forge-cordex-0.2.2/pangeo_forge_cordex/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 10:24:42.415635 pangeo-forge-cordex-0.2.2/pangeo_forge_cordex.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1293 2023-05-05 10:24:42.000000 pangeo-forge-cordex-0.2.2/pangeo_forge_cordex.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      689 2023-05-05 10:24:42.000000 pangeo-forge-cordex-0.2.2/pangeo_forge_cordex.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 10:24:42.000000 pangeo-forge-cordex-0.2.2/pangeo_forge_cordex.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 10:24:42.000000 pangeo-forge-cordex-0.2.2/pangeo_forge_cordex.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-05 10:24:42.000000 pangeo-forge-cordex-0.2.2/pangeo_forge_cordex.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       26 2023-05-05 10:24:42.000000 pangeo-forge-cordex-0.2.2/pangeo_forge_cordex.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      426 2023-05-05 10:24:32.000000 pangeo-forge-cordex-0.2.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-05-05 10:24:32.000000 pangeo-forge-cordex-0.2.2/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1343 2023-05-05 10:24:42.415635 pangeo-forge-cordex-0.2.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-05 10:24:32.000000 pangeo-forge-cordex-0.2.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 10:24:42.415635 pangeo-forge-cordex-0.2.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 10:24:32.000000 pangeo-forge-cordex-0.2.2/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1105 2023-05-05 10:24:32.000000 pangeo-forge-cordex-0.2.2/tests/test_recipe_creation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 12:29:24.088386 pangeo-forge-cordex-0.2.3/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 12:29:24.080386 pangeo-forge-cordex-0.2.3/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 12:29:24.084386 pangeo-forge-cordex-0.2.3/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     2375 2023-05-05 12:29:09.000000 pangeo-forge-cordex-0.2.3/.github/workflows/ci.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      738 2023-05-05 12:29:09.000000 pangeo-forge-cordex-0.2.3/.github/workflows/release.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1831 2023-05-05 12:29:09.000000 pangeo-forge-cordex-0.2.3/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      475 2023-05-05 12:29:09.000000 pangeo-forge-cordex-0.2.3/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-05-05 12:29:09.000000 pangeo-forge-cordex-0.2.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1293 2023-05-05 12:29:24.088386 pangeo-forge-cordex-0.2.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      369 2023-05-05 12:29:09.000000 pangeo-forge-cordex-0.2.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 12:29:24.084386 pangeo-forge-cordex-0.2.3/ci/
+-rw-r--r--   0 runner    (1001) docker     (123)      235 2023-05-05 12:29:09.000000 pangeo-forge-cordex-0.2.3/ci/environment.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-05-05 12:29:09.000000 pangeo-forge-cordex-0.2.3/environment.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 12:29:24.084386 pangeo-forge-cordex-0.2.3/pangeo_forge_cordex/
+-rw-r--r--   0 runner    (1001) docker     (123)      288 2023-05-05 12:29:09.000000 pangeo-forge-cordex-0.2.3/pangeo_forge_cordex/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-05 12:29:23.000000 pangeo-forge-cordex-0.2.3/pangeo_forge_cordex/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2176 2023-05-05 12:29:09.000000 pangeo-forge-cordex-0.2.3/pangeo_forge_cordex/esgf_access.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6347 2023-05-05 12:29:09.000000 pangeo-forge-cordex-0.2.3/pangeo_forge_cordex/parsing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2665 2023-05-05 12:29:09.000000 pangeo-forge-cordex-0.2.3/pangeo_forge_cordex/recipe.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1702 2023-05-05 12:29:09.000000 pangeo-forge-cordex-0.2.3/pangeo_forge_cordex/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 12:29:24.088386 pangeo-forge-cordex-0.2.3/pangeo_forge_cordex.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1293 2023-05-05 12:29:24.000000 pangeo-forge-cordex-0.2.3/pangeo_forge_cordex.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      711 2023-05-05 12:29:24.000000 pangeo-forge-cordex-0.2.3/pangeo_forge_cordex.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 12:29:24.000000 pangeo-forge-cordex-0.2.3/pangeo_forge_cordex.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 12:29:24.000000 pangeo-forge-cordex-0.2.3/pangeo_forge_cordex.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-05 12:29:24.000000 pangeo-forge-cordex-0.2.3/pangeo_forge_cordex.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-05-05 12:29:24.000000 pangeo-forge-cordex-0.2.3/pangeo_forge_cordex.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      426 2023-05-05 12:29:09.000000 pangeo-forge-cordex-0.2.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-05-05 12:29:09.000000 pangeo-forge-cordex-0.2.3/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1343 2023-05-05 12:29:24.088386 pangeo-forge-cordex-0.2.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-05 12:29:09.000000 pangeo-forge-cordex-0.2.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 12:29:24.088386 pangeo-forge-cordex-0.2.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 12:29:09.000000 pangeo-forge-cordex-0.2.3/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      568 2023-05-05 12:29:09.000000 pangeo-forge-cordex-0.2.3/tests/test_parsing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1105 2023-05-05 12:29:09.000000 pangeo-forge-cordex-0.2.3/tests/test_recipe_creation.py
```

### Comparing `pangeo-forge-cordex-0.2.2/.github/workflows/ci.yaml` & `pangeo-forge-cordex-0.2.3/.github/workflows/ci.yaml`

 * *Files identical despite different names*

### Comparing `pangeo-forge-cordex-0.2.2/.github/workflows/release.yaml` & `pangeo-forge-cordex-0.2.3/.github/workflows/release.yaml`

 * *Files identical despite different names*

### Comparing `pangeo-forge-cordex-0.2.2/.gitignore` & `pangeo-forge-cordex-0.2.3/.gitignore`

 * *Files identical despite different names*

### Comparing `pangeo-forge-cordex-0.2.2/LICENSE` & `pangeo-forge-cordex-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pangeo-forge-cordex-0.2.2/PKG-INFO` & `pangeo-forge-cordex-0.2.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pangeo-forge-cordex
-Version: 0.2.2
+Version: 0.2.3
 Summary: "Using queries to the ESGF API to generate urls and keyword arguments for receipe generation in pangeo-forge"
 Home-page: https://github.com/euro-cordex/pangeo-forge-cordex
 Maintainer: Lars Buntemeyer
 Maintainer-email: lars.buntemeyer@hereon.de
 License: MIT
 Keywords: pangeo,data,esgf
 Classifier: Development Status :: 1 - Planning
```

### Comparing `pangeo-forge-cordex-0.2.2/pangeo_forge_cordex/esgf_access.py` & `pangeo-forge-cordex-0.2.3/pangeo_forge_cordex/esgf_access.py`

 * *Files identical despite different names*

### Comparing `pangeo-forge-cordex-0.2.2/pangeo_forge_cordex/parsing.py` & `pangeo-forge-cordex-0.2.3/pangeo_forge_cordex/parsing.py`

 * *Files 10% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 cordex_template = "project.product.domain.institute.driving_model.experiment.ensemble.rcm_name.rcm_version.time_frequency.variable.version"
 cordex_adjust_template = "project.product.domain.institute.driving_model.experiment.ensemble.rcm_name.bias_adjustment.time_frequency.variable.version"
 
 base_params = {
     # "type": "File",
     "format": "application/solr+json",
     # "fields": "instance_id",
-    "fields": "url,size,table_id,title,instance_id,replica,data_node,frequency,time_frequency,version",
+    "fields": "url,size,table_id,title,instance_id,replica,data_node,frequency,time_frequency,version,size,datetime_start,datetime_stop",
     "latest": True,
     "distrib": True,
     "limit": 500,
 }
 
 cordex_params = base_params
 
@@ -104,61 +104,82 @@
 
 
 def request_project_facets(project, url=None):
     template = get_dataset_id_template(project, url)
     return facets_from_template(template)
 
 
-def request_from_facets(url, project, **facets):
+def request_from_facets(url, project, type="Dataset", **facets):
     params = request_params[project].copy()
     params.update(facets)
     params["project"] = project
-    params["type"] = "Dataset"
+    params["type"] = type
     return requests.get(url=url, params=params)
 
 
 def instance_ids_from_request(json_dict):
     iids = [item["instance_id"] for item in json_dict["response"]["docs"]]
     uniqe_iids = list(set(iids))
     return uniqe_iids
 
 
-def parse_instance_ids(iid, url=None, project=None, **params):
+def parse_facets(iid, project):
+    facets = facets_from_iid(iid, project)
+    # convert string to list if square brackets are found
+    for k, v in facets.items():
+        if "[" in v:
+            v = (
+                v.replace("[", "")
+                .replace("]", "")
+                .replace("'", "")
+                .replace(" ", "")
+                .split(",")
+            )
+        facets[k] = v
+    return {k: v for k, v in facets.items() if v != "*" and k != "project"}
+
+
+def request_instance_ids(iid, url=None, project=None, type="Dataset", **params):
     """Parse an instance id with wildcards
 
     Examples:
     'cordex.output.EUR-11.GERICS.ICHEC-EC-EARTH.*.*.REMO2015.*.mon.tas'
     'cordex-reklies.output.EUR-11.GERICS.*.historical.r1i1p1.REMO2015.v1.*.tas'
     'cordex-adjust.*.EUR-11.*.MPI-M-MPI-ESM-LR.rcp45.*.*.*.mon.tasAdjust'
     'cordex-esd.*.EUR-11.*.MPI-M-MPI-ESM-LR.historical.*.*.*.*.tas'
 
-
     """
-    # TODO: I should make the node url a keyword argument. For now this works well enough
     if url is None:
-        # url = "https://esgf-node.llnl.gov/esg-search/search"
         url = "https://esgf-data.dkrz.de/esg-search/search"
     if project is None:
         # take project id from first iid entry by default
         project = ensure_project_str(iid.split(".")[0])
-    facets = facets_from_iid(iid, project)
-    # convert string to list if square brackets are found
-    for k, v in facets.items():
-        if "[" in v:
-            v = (
-                v.replace("[", "")
-                .replace("]", "")
-                .replace("'", "")
-                .replace(" ", "")
-                .split(",")
-            )
-        facets[k] = v
-    facets_filtered = {k: v for k, v in facets.items() if v != "*" and k != "project"}
+
+    facets_filtered = parse_facets(iid, project)
     params = facets_filtered | params
 
-    resp = request_from_facets(url, project, **params)
+    resp = request_from_facets(url, project, type, **params)
     if resp.status_code != 200:
         print(f"Request [{resp.url}] failed with {resp.status_code}")
         return resp
     else:
-        json_dict = resp.json()
-        return instance_ids_from_request(json_dict)
+        return resp.json()
+
+
+def parse_instance_ids(iid, url=None, project=None, **params):
+    """Parse an instance id with wildcards
+
+    Examples:
+    'cordex.output.EUR-11.GERICS.ICHEC-EC-EARTH.*.*.REMO2015.*.mon.tas'
+    'cordex-reklies.output.EUR-11.GERICS.*.historical.r1i1p1.REMO2015.v1.*.tas'
+    'cordex-adjust.*.EUR-11.*.MPI-M-MPI-ESM-LR.rcp45.*.*.*.mon.tasAdjust'
+    'cordex-esd.*.EUR-11.*.MPI-M-MPI-ESM-LR.historical.*.*.*.*.tas'
+
+    """
+    resp = request_instance_ids(iid, url, project, **params)
+
+    return instance_ids_from_request(resp)
+
+
+def total_size_ids(iid, url=None, project=None, **params):
+    resp = request_instance_ids(iid, url, project, **params)
+    return sum([r["size"] for r in resp["response"]["docs"]])
```

### Comparing `pangeo-forge-cordex-0.2.2/pangeo_forge_cordex/recipe.py` & `pangeo-forge-cordex-0.2.3/pangeo_forge_cordex/recipe.py`

 * *Files identical despite different names*

### Comparing `pangeo-forge-cordex-0.2.2/pangeo_forge_cordex/utils.py` & `pangeo-forge-cordex-0.2.3/pangeo_forge_cordex/utils.py`

 * *Files identical despite different names*

### Comparing `pangeo-forge-cordex-0.2.2/pangeo_forge_cordex.egg-info/PKG-INFO` & `pangeo-forge-cordex-0.2.3/pangeo_forge_cordex.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pangeo-forge-cordex
-Version: 0.2.2
+Version: 0.2.3
 Summary: "Using queries to the ESGF API to generate urls and keyword arguments for receipe generation in pangeo-forge"
 Home-page: https://github.com/euro-cordex/pangeo-forge-cordex
 Maintainer: Lars Buntemeyer
 Maintainer-email: lars.buntemeyer@hereon.de
 License: MIT
 Keywords: pangeo,data,esgf
 Classifier: Development Status :: 1 - Planning
```

### Comparing `pangeo-forge-cordex-0.2.2/pangeo_forge_cordex.egg-info/SOURCES.txt` & `pangeo-forge-cordex-0.2.3/pangeo_forge_cordex.egg-info/SOURCES.txt`

 * *Files 11% similar despite different names*

```diff
@@ -19,8 +19,9 @@
 pangeo_forge_cordex.egg-info/PKG-INFO
 pangeo_forge_cordex.egg-info/SOURCES.txt
 pangeo_forge_cordex.egg-info/dependency_links.txt
 pangeo_forge_cordex.egg-info/not-zip-safe
 pangeo_forge_cordex.egg-info/requires.txt
 pangeo_forge_cordex.egg-info/top_level.txt
 tests/__init__.py
+tests/test_parsing.py
 tests/test_recipe_creation.py
```

### Comparing `pangeo-forge-cordex-0.2.2/setup.cfg` & `pangeo-forge-cordex-0.2.3/setup.cfg`

 * *Files identical despite different names*

### Comparing `pangeo-forge-cordex-0.2.2/tests/test_recipe_creation.py` & `pangeo-forge-cordex-0.2.3/tests/test_recipe_creation.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from pangeo_forge_recipes.patterns import pattern_from_file_sequence
 from pangeo_forge_recipes.recipes import XarrayZarrRecipe
 
 from pangeo_forge_cordex import logon, recipe_inputs_from_iids
 
 iids = [
     "cordex.output.EUR-11.DMI.ECMWF-ERAINT.evaluation.r1i1p1.HIRHAM5.v1.mon.tas.v20140620",
-    "cordex.output.EUR-11.GERICS.ECMWF-ERAINT.evaluation.r1i1p1.REMO2015.v1.day.tas.v20180813",
+    "cordex.output.EUR-11.GERICS.ECMWF-ERAINT.evaluation.r1i1p1.REMO2015.v1.mon.tas.v20180813",
 ]
 
 
 @pytest.mark.parametrize("iid", iids)
 def test_recipe_inputs(iid):
     sslcontext = logon()
```

