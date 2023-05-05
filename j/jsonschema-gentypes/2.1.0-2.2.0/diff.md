# Comparing `tmp/jsonschema_gentypes-2.1.0.tar.gz` & `tmp/jsonschema_gentypes-2.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jsonschema_gentypes-2.1.0.tar", max compression
+gzip compressed data, was "jsonschema_gentypes-2.2.0.tar", max compression
```

## Comparing `jsonschema_gentypes-2.1.0.tar` & `jsonschema_gentypes-2.2.0.tar`

### file list

```diff
@@ -1,32 +1,32 @@
--rw-r--r--   0        0        0     1304 2023-05-02 14:36:20.657462 jsonschema_gentypes-2.1.0/LICENSE
--rw-r--r--   0        0        0     3358 2023-05-02 14:36:20.657462 jsonschema_gentypes-2.1.0/README.md
--rw-r--r--   0        0        0    21740 2023-05-02 14:36:20.657462 jsonschema_gentypes-2.1.0/jsonschema_gentypes/__init__.py
--rw-r--r--   0        0        0    17327 2023-05-02 14:36:20.657462 jsonschema_gentypes-2.1.0/jsonschema_gentypes/api.py
--rw-r--r--   0        0        0    12990 2023-05-02 14:36:20.657462 jsonschema_gentypes-2.1.0/jsonschema_gentypes/api_draft_04.py
--rw-r--r--   0        0        0     2574 2023-05-02 14:36:20.657462 jsonschema_gentypes-2.1.0/jsonschema_gentypes/api_draft_06.py
--rw-r--r--   0        0        0      149 2023-05-02 14:36:20.657462 jsonschema_gentypes-2.1.0/jsonschema_gentypes/api_draft_07.py
--rw-r--r--   0        0        0     3042 2023-05-02 14:36:20.657462 jsonschema_gentypes-2.1.0/jsonschema_gentypes/api_draft_2019_09.py
--rw-r--r--   0        0        0     4339 2023-05-02 14:36:20.657462 jsonschema_gentypes-2.1.0/jsonschema_gentypes/api_draft_2020_12.py
--rw-r--r--   0        0        0    15226 2023-05-02 14:36:20.657462 jsonschema_gentypes-2.1.0/jsonschema_gentypes/cli.py
--rw-r--r--   0        0        0     2538 2023-05-02 14:37:22.874370 jsonschema_gentypes-2.1.0/jsonschema_gentypes/configuration.py
--rw-r--r--   0        0        0     4982 2023-05-02 14:37:25.806417 jsonschema_gentypes-2.1.0/jsonschema_gentypes/jsonschema_draft_04.py
--rw-r--r--   0        0        0     5251 2023-05-02 14:37:28.478461 jsonschema_gentypes-2.1.0/jsonschema_gentypes/jsonschema_draft_06.py
--rw-r--r--   0        0        0     5481 2023-05-02 14:37:31.146504 jsonschema_gentypes-2.1.0/jsonschema_gentypes/jsonschema_draft_07.py
--rw-r--r--   0        0        0     1698 2023-05-02 14:37:33.790546 jsonschema_gentypes-2.1.0/jsonschema_gentypes/jsonschema_draft_2019_09.py
--rw-r--r--   0        0        0     1596 2023-05-02 14:37:41.358667 jsonschema_gentypes-2.1.0/jsonschema_gentypes/jsonschema_draft_2019_09_applicator.py
--rw-r--r--   0        0        0      384 2023-05-02 14:37:48.854789 jsonschema_gentypes-2.1.0/jsonschema_gentypes/jsonschema_draft_2019_09_content.py
--rw-r--r--   0        0        0     1260 2023-05-02 14:37:36.302586 jsonschema_gentypes-2.1.0/jsonschema_gentypes/jsonschema_draft_2019_09_core.py
--rw-r--r--   0        0        0      296 2023-05-02 14:37:46.378749 jsonschema_gentypes-2.1.0/jsonschema_gentypes/jsonschema_draft_2019_09_format.py
--rw-r--r--   0        0        0      973 2023-05-02 14:37:38.822626 jsonschema_gentypes-2.1.0/jsonschema_gentypes/jsonschema_draft_2019_09_meta_data.py
--rw-r--r--   0        0        0     3019 2023-05-02 14:37:43.906709 jsonschema_gentypes-2.1.0/jsonschema_gentypes/jsonschema_draft_2019_09_validation.py
--rw-r--r--   0        0        0     2569 2023-05-02 14:37:51.830837 jsonschema_gentypes-2.1.0/jsonschema_gentypes/jsonschema_draft_2020_12.py
--rw-r--r--   0        0        0     1691 2023-05-02 14:37:59.450962 jsonschema_gentypes-2.1.0/jsonschema_gentypes/jsonschema_draft_2020_12_applicator.py
--rw-r--r--   0        0        0      384 2023-05-02 14:38:04.543085 jsonschema_gentypes-2.1.0/jsonschema_gentypes/jsonschema_draft_2020_12_content.py
--rw-r--r--   0        0        0      859 2023-05-02 14:37:54.358878 jsonschema_gentypes-2.1.0/jsonschema_gentypes/jsonschema_draft_2020_12_core.py
--rw-r--r--   0        0        0      973 2023-05-02 14:37:56.894920 jsonschema_gentypes-2.1.0/jsonschema_gentypes/jsonschema_draft_2020_12_meta_data.py
--rw-r--r--   0        0        0     3019 2023-05-02 14:38:02.035009 jsonschema_gentypes-2.1.0/jsonschema_gentypes/jsonschema_draft_2020_12_validation.py
--rw-r--r--   0        0        0        0 2023-05-02 14:36:20.657462 jsonschema_gentypes-2.1.0/jsonschema_gentypes/py.typed
--rw-r--r--   0        0        0     5868 2023-05-02 14:36:20.657462 jsonschema_gentypes-2.1.0/jsonschema_gentypes/resolver.py
--rw-r--r--   0        0        0     3067 2023-05-02 14:36:20.657462 jsonschema_gentypes-2.1.0/jsonschema_gentypes/schema.json
--rw-r--r--   0        0        0     2514 2023-05-02 14:39:31.276556 jsonschema_gentypes-2.1.0/pyproject.toml
--rw-r--r--   0        0        0     4877 1970-01-01 00:00:00.000000 jsonschema_gentypes-2.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1304 2023-05-05 15:43:52.522914 jsonschema_gentypes-2.2.0/LICENSE
+-rw-r--r--   0        0        0     3358 2023-05-05 15:43:52.522914 jsonschema_gentypes-2.2.0/README.md
+-rw-r--r--   0        0        0    21740 2023-05-05 15:43:52.522914 jsonschema_gentypes-2.2.0/jsonschema_gentypes/__init__.py
+-rw-r--r--   0        0        0    17327 2023-05-05 15:43:52.522914 jsonschema_gentypes-2.2.0/jsonschema_gentypes/api.py
+-rw-r--r--   0        0        0    12990 2023-05-05 15:43:52.522914 jsonschema_gentypes-2.2.0/jsonschema_gentypes/api_draft_04.py
+-rw-r--r--   0        0        0     2574 2023-05-05 15:43:52.522914 jsonschema_gentypes-2.2.0/jsonschema_gentypes/api_draft_06.py
+-rw-r--r--   0        0        0      149 2023-05-05 15:43:52.522914 jsonschema_gentypes-2.2.0/jsonschema_gentypes/api_draft_07.py
+-rw-r--r--   0        0        0     3042 2023-05-05 15:43:52.522914 jsonschema_gentypes-2.2.0/jsonschema_gentypes/api_draft_2019_09.py
+-rw-r--r--   0        0        0     4339 2023-05-05 15:43:52.522914 jsonschema_gentypes-2.2.0/jsonschema_gentypes/api_draft_2020_12.py
+-rw-r--r--   0        0        0    15226 2023-05-05 15:43:52.522914 jsonschema_gentypes-2.2.0/jsonschema_gentypes/cli.py
+-rw-r--r--   0        0        0     2538 2023-05-05 15:44:45.386751 jsonschema_gentypes-2.2.0/jsonschema_gentypes/configuration.py
+-rw-r--r--   0        0        0     4982 2023-05-05 15:44:47.758740 jsonschema_gentypes-2.2.0/jsonschema_gentypes/jsonschema_draft_04.py
+-rw-r--r--   0        0        0     5251 2023-05-05 15:44:50.090729 jsonschema_gentypes-2.2.0/jsonschema_gentypes/jsonschema_draft_06.py
+-rw-r--r--   0        0        0     5481 2023-05-05 15:44:52.358718 jsonschema_gentypes-2.2.0/jsonschema_gentypes/jsonschema_draft_07.py
+-rw-r--r--   0        0        0     1698 2023-05-05 15:44:54.602707 jsonschema_gentypes-2.2.0/jsonschema_gentypes/jsonschema_draft_2019_09.py
+-rw-r--r--   0        0        0     1596 2023-05-05 15:45:00.890677 jsonschema_gentypes-2.2.0/jsonschema_gentypes/jsonschema_draft_2019_09_applicator.py
+-rw-r--r--   0        0        0      384 2023-05-05 15:45:07.170647 jsonschema_gentypes-2.2.0/jsonschema_gentypes/jsonschema_draft_2019_09_content.py
+-rw-r--r--   0        0        0     1260 2023-05-05 15:44:56.694697 jsonschema_gentypes-2.2.0/jsonschema_gentypes/jsonschema_draft_2019_09_core.py
+-rw-r--r--   0        0        0      296 2023-05-05 15:45:05.110656 jsonschema_gentypes-2.2.0/jsonschema_gentypes/jsonschema_draft_2019_09_format.py
+-rw-r--r--   0        0        0      973 2023-05-05 15:44:58.782687 jsonschema_gentypes-2.2.0/jsonschema_gentypes/jsonschema_draft_2019_09_meta_data.py
+-rw-r--r--   0        0        0     3019 2023-05-05 15:45:03.038666 jsonschema_gentypes-2.2.0/jsonschema_gentypes/jsonschema_draft_2019_09_validation.py
+-rw-r--r--   0        0        0     2569 2023-05-05 15:45:09.558635 jsonschema_gentypes-2.2.0/jsonschema_gentypes/jsonschema_draft_2020_12.py
+-rw-r--r--   0        0        0     1691 2023-05-05 15:45:15.894605 jsonschema_gentypes-2.2.0/jsonschema_gentypes/jsonschema_draft_2020_12_applicator.py
+-rw-r--r--   0        0        0      384 2023-05-05 15:45:20.106584 jsonschema_gentypes-2.2.0/jsonschema_gentypes/jsonschema_draft_2020_12_content.py
+-rw-r--r--   0        0        0      859 2023-05-05 15:45:11.638625 jsonschema_gentypes-2.2.0/jsonschema_gentypes/jsonschema_draft_2020_12_core.py
+-rw-r--r--   0        0        0      973 2023-05-05 15:45:13.714615 jsonschema_gentypes-2.2.0/jsonschema_gentypes/jsonschema_draft_2020_12_meta_data.py
+-rw-r--r--   0        0        0     3019 2023-05-05 15:45:18.034594 jsonschema_gentypes-2.2.0/jsonschema_gentypes/jsonschema_draft_2020_12_validation.py
+-rw-r--r--   0        0        0        0 2023-05-05 15:43:52.522914 jsonschema_gentypes-2.2.0/jsonschema_gentypes/py.typed
+-rw-r--r--   0        0        0     6112 2023-05-05 15:43:52.522914 jsonschema_gentypes-2.2.0/jsonschema_gentypes/resolver.py
+-rw-r--r--   0        0        0     3067 2023-05-05 15:43:52.522914 jsonschema_gentypes-2.2.0/jsonschema_gentypes/schema.json
+-rw-r--r--   0        0        0     2514 2023-05-05 15:46:34.190265 jsonschema_gentypes-2.2.0/pyproject.toml
+-rw-r--r--   0        0        0     4877 1970-01-01 00:00:00.000000 jsonschema_gentypes-2.2.0/PKG-INFO
```

### Comparing `jsonschema_gentypes-2.1.0/LICENSE` & `jsonschema_gentypes-2.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `jsonschema_gentypes-2.1.0/README.md` & `jsonschema_gentypes-2.2.0/README.md`

 * *Files identical despite different names*

### Comparing `jsonschema_gentypes-2.1.0/jsonschema_gentypes/__init__.py` & `jsonschema_gentypes-2.2.0/jsonschema_gentypes/__init__.py`

 * *Files identical despite different names*

### Comparing `jsonschema_gentypes-2.1.0/jsonschema_gentypes/api.py` & `jsonschema_gentypes-2.2.0/jsonschema_gentypes/api.py`

 * *Files identical despite different names*

### Comparing `jsonschema_gentypes-2.1.0/jsonschema_gentypes/api_draft_04.py` & `jsonschema_gentypes-2.2.0/jsonschema_gentypes/api_draft_04.py`

 * *Files identical despite different names*

### Comparing `jsonschema_gentypes-2.1.0/jsonschema_gentypes/api_draft_06.py` & `jsonschema_gentypes-2.2.0/jsonschema_gentypes/api_draft_06.py`

 * *Files identical despite different names*

### Comparing `jsonschema_gentypes-2.1.0/jsonschema_gentypes/api_draft_2019_09.py` & `jsonschema_gentypes-2.2.0/jsonschema_gentypes/api_draft_2019_09.py`

 * *Files identical despite different names*

### Comparing `jsonschema_gentypes-2.1.0/jsonschema_gentypes/api_draft_2020_12.py` & `jsonschema_gentypes-2.2.0/jsonschema_gentypes/api_draft_2020_12.py`

 * *Files identical despite different names*

### Comparing `jsonschema_gentypes-2.1.0/jsonschema_gentypes/cli.py` & `jsonschema_gentypes-2.2.0/jsonschema_gentypes/cli.py`

 * *Files identical despite different names*

### Comparing `jsonschema_gentypes-2.1.0/jsonschema_gentypes/configuration.py` & `jsonschema_gentypes-2.2.0/jsonschema_gentypes/configuration.py`

 * *Files identical despite different names*

### Comparing `jsonschema_gentypes-2.1.0/jsonschema_gentypes/jsonschema_draft_04.py` & `jsonschema_gentypes-2.2.0/jsonschema_gentypes/jsonschema_draft_04.py`

 * *Files identical despite different names*

### Comparing `jsonschema_gentypes-2.1.0/jsonschema_gentypes/jsonschema_draft_06.py` & `jsonschema_gentypes-2.2.0/jsonschema_gentypes/jsonschema_draft_06.py`

 * *Files identical despite different names*

### Comparing `jsonschema_gentypes-2.1.0/jsonschema_gentypes/jsonschema_draft_07.py` & `jsonschema_gentypes-2.2.0/jsonschema_gentypes/jsonschema_draft_07.py`

 * *Files identical despite different names*

### Comparing `jsonschema_gentypes-2.1.0/jsonschema_gentypes/jsonschema_draft_2019_09.py` & `jsonschema_gentypes-2.2.0/jsonschema_gentypes/jsonschema_draft_2019_09.py`

 * *Files identical despite different names*

### Comparing `jsonschema_gentypes-2.1.0/jsonschema_gentypes/jsonschema_draft_2019_09_applicator.py` & `jsonschema_gentypes-2.2.0/jsonschema_gentypes/jsonschema_draft_2019_09_applicator.py`

 * *Files identical despite different names*

### Comparing `jsonschema_gentypes-2.1.0/jsonschema_gentypes/jsonschema_draft_2019_09_core.py` & `jsonschema_gentypes-2.2.0/jsonschema_gentypes/jsonschema_draft_2019_09_core.py`

 * *Files identical despite different names*

### Comparing `jsonschema_gentypes-2.1.0/jsonschema_gentypes/jsonschema_draft_2019_09_meta_data.py` & `jsonschema_gentypes-2.2.0/jsonschema_gentypes/jsonschema_draft_2019_09_meta_data.py`

 * *Files identical despite different names*

### Comparing `jsonschema_gentypes-2.1.0/jsonschema_gentypes/jsonschema_draft_2019_09_validation.py` & `jsonschema_gentypes-2.2.0/jsonschema_gentypes/jsonschema_draft_2019_09_validation.py`

 * *Files identical despite different names*

### Comparing `jsonschema_gentypes-2.1.0/jsonschema_gentypes/jsonschema_draft_2020_12.py` & `jsonschema_gentypes-2.2.0/jsonschema_gentypes/jsonschema_draft_2020_12.py`

 * *Files identical despite different names*

### Comparing `jsonschema_gentypes-2.1.0/jsonschema_gentypes/jsonschema_draft_2020_12_applicator.py` & `jsonschema_gentypes-2.2.0/jsonschema_gentypes/jsonschema_draft_2020_12_applicator.py`

 * *Files identical despite different names*

### Comparing `jsonschema_gentypes-2.1.0/jsonschema_gentypes/jsonschema_draft_2020_12_core.py` & `jsonschema_gentypes-2.2.0/jsonschema_gentypes/jsonschema_draft_2020_12_core.py`

 * *Files identical despite different names*

### Comparing `jsonschema_gentypes-2.1.0/jsonschema_gentypes/jsonschema_draft_2020_12_meta_data.py` & `jsonschema_gentypes-2.2.0/jsonschema_gentypes/jsonschema_draft_2020_12_meta_data.py`

 * *Files identical despite different names*

### Comparing `jsonschema_gentypes-2.1.0/jsonschema_gentypes/jsonschema_draft_2020_12_validation.py` & `jsonschema_gentypes-2.2.0/jsonschema_gentypes/jsonschema_draft_2020_12_validation.py`

 * *Files identical despite different names*

### Comparing `jsonschema_gentypes-2.1.0/jsonschema_gentypes/resolver.py` & `jsonschema_gentypes-2.2.0/jsonschema_gentypes/resolver.py`

 * *Files 4% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 """
 
 import json
 import re
 from typing import Any, Dict, List, Optional, Union, cast
 
 import requests
+import yaml
 from referencing import Registry, Resource
 
 from jsonschema_gentypes import (
     jsonschema_draft_04,
     jsonschema_draft_06,
     jsonschema_draft_2019_09_core,
     jsonschema_draft_2020_12_applicator,
@@ -55,21 +56,26 @@
                     jsonschema_draft_2020_12_applicator.JSONSchemaItemD2020,
                 ],
                 response.json(),
             )
         )
     else:
         with open(uri, encoding="utf-8") as open_file:
+            file_content = open_file.read()
+            try:
+                schema = yaml.load(file_content, Loader=yaml.SafeLoader)
+            except Exception:  # pylint: disable=broad-except
+                schema = json.loads(file_content)
             return _openapi_schema(
                 cast(
                     Union[
                         jsonschema_draft_06.JSONSchemaItemD6,
                         jsonschema_draft_2020_12_applicator.JSONSchemaItemD2020,
                     ],
-                    json.load(open_file),
+                    schema,
                 )
             )
 
 
 def _open_uri_resolver(uri: str) -> Resource[Any]:
     if uri in _RESOURCE_CACHE:
         return _RESOURCE_CACHE[uri]
```

### Comparing `jsonschema_gentypes-2.1.0/jsonschema_gentypes/schema.json` & `jsonschema_gentypes-2.2.0/jsonschema_gentypes/schema.json`

 * *Files identical despite different names*

### Comparing `jsonschema_gentypes-2.1.0/pyproject.toml` & `jsonschema_gentypes-2.2.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -11,15 +11,15 @@
 warn_redundant_casts = true
 warn_unused_ignores = true
 ignore_missing_imports = true
 strict = true
 
 [tool.poetry]
 name = "jsonschema-gentypes"
-version = "2.1.0"
+version = "2.2.0"
 description = "Tool to generate Python types based on TypedDict from a JSON Schema"
 readme = "README.md"
 authors = ["Camptocamp <info@camptocamp.com>"]
 repository = "https://github.com/camptocamp/jsonschema-gentypes"
 license = "BSD-2-Clause"
 keywords = ["jsonschema", "types"]
 packages = [{ include = "jsonschema_gentypes" }]
```

### Comparing `jsonschema_gentypes-2.1.0/PKG-INFO` & `jsonschema_gentypes-2.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jsonschema-gentypes
-Version: 2.1.0
+Version: 2.2.0
 Summary: Tool to generate Python types based on TypedDict from a JSON Schema
 Home-page: https://github.com/camptocamp/jsonschema-gentypes
 License: BSD-2-Clause
 Keywords: jsonschema,types
 Author: Camptocamp
 Author-email: info@camptocamp.com
 Requires-Python: >=3.8,<4
```

