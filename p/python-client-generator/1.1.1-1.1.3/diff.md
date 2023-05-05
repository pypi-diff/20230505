# Comparing `tmp/python-client-generator-1.1.1.tar.gz` & `tmp/python_client_generator-1.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python-client-generator-1.1.1.tar", max compression
+gzip compressed data, was "python_client_generator-1.1.3.tar", max compression
```

## Comparing `python-client-generator-1.1.1.tar` & `python_client_generator-1.1.3.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0     1069 2023-04-05 09:14:14.189891 python-client-generator-1.1.1/LICENSE
--rw-r--r--   0        0        0     1473 2023-04-05 09:14:14.189891 python-client-generator-1.1.1/README.md
--rw-r--r--   0        0        0     1751 2023-04-05 09:14:48.725695 python-client-generator-1.1.1/pyproject.toml
--rw-r--r--   0        0        0        0 2023-04-05 09:14:14.189891 python-client-generator-1.1.1/python_client_generator/__init__.py
--rw-r--r--   0        0        0       32 2023-04-05 09:14:14.189891 python-client-generator-1.1.1/python_client_generator/__main__.py
--rwxr-xr-x   0        0        0     6598 2023-04-05 09:14:14.189891 python-client-generator-1.1.1/python_client_generator/generate_apis.py
--rw-r--r--   0        0        0      493 2023-04-05 09:14:14.189891 python-client-generator-1.1.1/python_client_generator/generate_base_client.py
--rwxr-xr-x   0        0        0     6482 2023-04-05 09:14:14.189891 python-client-generator-1.1.1/python_client_generator/generate_models.py
--rw-r--r--   0        0        0      593 2023-04-05 09:14:14.189891 python-client-generator-1.1.1/python_client_generator/generate_pyproject.py
--rw-r--r--   0        0        0     1736 2023-04-05 09:14:14.189891 python-client-generator-1.1.1/python_client_generator/main.py
--rw-r--r--   0        0        0       42 2023-04-05 09:14:14.189891 python-client-generator-1.1.1/python_client_generator/templates/__init__.py
--rw-r--r--   0        0        0     2251 2023-04-05 09:14:14.189891 python-client-generator-1.1.1/python_client_generator/templates/apis.py.mustache
--rw-r--r--   0        0        0     1817 2023-04-05 09:14:14.189891 python-client-generator-1.1.1/python_client_generator/templates/base_client.py.mustache
--rw-r--r--   0        0        0      509 2023-04-05 09:14:14.189891 python-client-generator-1.1.1/python_client_generator/templates/models.py.mustache
--rw-r--r--   0        0        0      423 2023-04-05 09:14:14.189891 python-client-generator-1.1.1/python_client_generator/templates/pyproject.toml.mustache
--rw-r--r--   0        0        0     3140 2023-04-05 09:14:14.189891 python-client-generator-1.1.1/python_client_generator/utils.py
--rw-r--r--   0        0        0     2448 2023-04-05 09:14:49.256384 python-client-generator-1.1.1/setup.py
--rw-r--r--   0        0        0     2331 2023-04-05 09:14:49.256754 python-client-generator-1.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1069 2023-05-05 13:00:52.052894 python_client_generator-1.1.3/LICENSE
+-rw-r--r--   0        0        0     1568 2023-05-05 13:00:52.052894 python_client_generator-1.1.3/README.md
+-rw-r--r--   0        0        0     1769 2023-05-05 13:01:20.667187 python_client_generator-1.1.3/pyproject.toml
+-rw-r--r--   0        0        0        0 2023-05-05 13:00:52.052894 python_client_generator-1.1.3/python_client_generator/__init__.py
+-rw-r--r--   0        0        0       32 2023-05-05 13:00:52.052894 python_client_generator-1.1.3/python_client_generator/__main__.py
+-rw-r--r--   0        0        0       54 2023-05-05 13:00:52.052894 python_client_generator-1.1.3/python_client_generator/exceptions.py
+-rwxr-xr-x   0        0        0     6598 2023-05-05 13:00:52.052894 python_client_generator-1.1.3/python_client_generator/generate_apis.py
+-rw-r--r--   0        0        0      493 2023-05-05 13:00:52.052894 python_client_generator-1.1.3/python_client_generator/generate_base_client.py
+-rwxr-xr-x   0        0        0     6482 2023-05-05 13:00:52.052894 python_client_generator-1.1.3/python_client_generator/generate_models.py
+-rw-r--r--   0        0        0      593 2023-05-05 13:00:52.052894 python_client_generator-1.1.3/python_client_generator/generate_pyproject.py
+-rw-r--r--   0        0        0     1797 2023-05-05 13:00:52.052894 python_client_generator-1.1.3/python_client_generator/main.py
+-rw-r--r--   0        0        0       42 2023-05-05 13:00:52.052894 python_client_generator-1.1.3/python_client_generator/templates/__init__.py
+-rw-r--r--   0        0        0     2251 2023-05-05 13:00:52.052894 python_client_generator-1.1.3/python_client_generator/templates/apis.py.mustache
+-rw-r--r--   0        0        0     1817 2023-05-05 13:00:52.052894 python_client_generator-1.1.3/python_client_generator/templates/base_client.py.mustache
+-rw-r--r--   0        0        0      509 2023-05-05 13:00:52.052894 python_client_generator-1.1.3/python_client_generator/templates/models.py.mustache
+-rw-r--r--   0        0        0      423 2023-05-05 13:00:52.052894 python_client_generator-1.1.3/python_client_generator/templates/pyproject.toml.mustache
+-rw-r--r--   0        0        0     3490 2023-05-05 13:00:52.052894 python_client_generator-1.1.3/python_client_generator/utils.py
+-rw-r--r--   0        0        0     2477 1970-01-01 00:00:00.000000 python_client_generator-1.1.3/PKG-INFO
```

### Comparing `python-client-generator-1.1.1/LICENSE` & `python_client_generator-1.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `python-client-generator-1.1.1/README.md` & `python_client_generator-1.1.3/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 # python-client-generator
 
 Python package to generate an [httpx](https://github.com/encode/httpx)- and
 [pydantic](https://github.com/pydantic/pydantic)-based async (or sync) 
-client off an OpenAPI spec.
+client off an OpenAPI spec >= 3.0.
 
 ```mermaid
 flowchart LR
     generator["python-client-generator"]
     app["REST API app"]
     package["app HTTP client"]
 
     app -- "OpenAPI json" --> generator
     generator -- "generates" --> package
 ```
 
+> :warning: **Currently does not support OpenAPI 2.0**: PR for < 3.0 support are welcome
 
 ## Using the generator
 
 ```bash
 python -m python_client_generator --open-api openapi.json --package-name foo_bar --project-name foo-bar --outdir clients
 ```
 
@@ -43,10 +44,9 @@
                 body=patch_body,
                 contact_id=contact.id,
                 tenant=tenant,
                 body_serializer_args={"exclude_unset": True}
 )
 ```
 
-
 ## Contributing
 Please refer to [CONTRIBUTING.md](.github/CONTRIBUTING.md).
```

### Comparing `python-client-generator-1.1.1/pyproject.toml` & `python_client_generator-1.1.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "python-client-generator"
-version = "1.1.1"
+version = "1.1.3"
 description = "Python package to generate an httpx-based client off an OpenAPI spec"
 readme = "README.md"
 authors = ["Bogdan Petre <bogdan.petre@sennder.com>", "Trevor Pace <trevor.pace@sennder.com>"]
 repository = "https://github.com/sennder/python-client-generator"
 
 [tool.poetry.urls]
 download = "https://github.com/sennder/python-client-generator/releases"
@@ -23,14 +23,15 @@
 mypy = "^0.812"
 black = "22.3.0"
 import-linter = "^1.2.1"
 isort = "^5.7.0"
 httpx = "^0.23.0"
 fastapi = "^0.92.0"
 python-multipart = "^0.0.6"
+semver = "^3.0.0"
 
 
 [tool.poetry.scripts]
 poetry = "poetry.console:main"
 
 [tool.semantic_release]
 version_toml = [
```

### Comparing `python-client-generator-1.1.1/python_client_generator/generate_apis.py` & `python_client_generator-1.1.3/python_client_generator/generate_apis.py`

 * *Files identical despite different names*

### Comparing `python-client-generator-1.1.1/python_client_generator/generate_models.py` & `python_client_generator-1.1.3/python_client_generator/generate_models.py`

 * *Files identical despite different names*

### Comparing `python-client-generator-1.1.1/python_client_generator/generate_pyproject.py` & `python_client_generator-1.1.3/python_client_generator/generate_pyproject.py`

 * *Files identical despite different names*

### Comparing `python-client-generator-1.1.1/python_client_generator/main.py` & `python_client_generator-1.1.3/python_client_generator/main.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import argparse
 import json
 import os
 import shutil
 
 from pathlib import Path
 
-from python_client_generator.utils import dereference_swagger
+from python_client_generator.utils import assert_openapi_version, dereference_swagger
 
 from .generate_apis import generate_apis
 from .generate_base_client import generate_base_client
 from .generate_models import generate_models
 from .generate_pyproject import generate_pyproject
 
 
@@ -26,14 +26,16 @@
     parser.add_argument("--group-by-tags", action="store_true")
     parser.add_argument("--sync", action="store_true")
 
     args = parser.parse_args()
 
     with open(args.open_api, "r") as f:
         swagger = json.load(f)
+
+    assert_openapi_version(swagger)
     dereferenced_swagger = dereference_swagger(swagger, swagger)
 
     # Create root directory
     path = Path(args.outdir)
     path.mkdir(parents=True, exist_ok=True)
 
     generate_pyproject(dereferenced_swagger, path / "pyproject.toml", args.project_name)
```

### Comparing `python-client-generator-1.1.1/python_client_generator/templates/apis.py.mustache` & `python_client_generator-1.1.3/python_client_generator/templates/apis.py.mustache`

 * *Files identical despite different names*

### Comparing `python-client-generator-1.1.1/python_client_generator/templates/base_client.py.mustache` & `python_client_generator-1.1.3/python_client_generator/templates/base_client.py.mustache`

 * *Files identical despite different names*

### Comparing `python-client-generator-1.1.1/python_client_generator/utils.py` & `python_client_generator-1.1.3/python_client_generator/utils.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,11 +1,15 @@
 import re
 
 from typing import Any, Dict, List
 
+import semver
+
+from python_client_generator.exceptions import UnsupportedOpenAPISpec
+
 
 def lookup_by_ref_parts(obj: Dict[str, Any], ref_parts: List[str]) -> Dict[str, Any]:
     child = obj[ref_parts[0]]
     if len(ref_parts) == 1:
         return child
     else:
         return lookup_by_ref_parts(child, ref_parts[1:])
@@ -92,7 +96,12 @@
         return "int"
     elif schema["type"] == "number":
         return "float"
     elif schema["type"] == "array":
         return "List[" + resolve_type(schema["items"], depth + 1) + "]"
 
     raise Exception("property: ", schema)
+
+
+def assert_openapi_version(schema: Dict[str, Any]) -> None:
+    if not schema.get("openapi") or semver.Version.parse(schema.get("openapi")).major != 3:  # type: ignore # noqa: E501
+        raise UnsupportedOpenAPISpec("OpenAPI file provided is not version 3.x")
```

### Comparing `python-client-generator-1.1.1/PKG-INFO` & `python_client_generator-1.1.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,42 +1,44 @@
 Metadata-Version: 2.1
 Name: python-client-generator
-Version: 1.1.1
+Version: 1.1.3
 Summary: Python package to generate an httpx-based client off an OpenAPI spec
 Home-page: https://github.com/sennder/python-client-generator
 Author: Bogdan Petre
 Author-email: bogdan.petre@sennder.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: chevron (>=0.14.0,<0.15.0)
 Requires-Dist: pydantic (>=1.9.1,<2.0.0)
 Project-URL: Repository, https://github.com/sennder/python-client-generator
 Project-URL: download, https://github.com/sennder/python-client-generator/releases
 Project-URL: tracker, https://github.com/sennder/python-client-generator/issues
 Description-Content-Type: text/markdown
 
 # python-client-generator
 
 Python package to generate an [httpx](https://github.com/encode/httpx)- and
 [pydantic](https://github.com/pydantic/pydantic)-based async (or sync) 
-client off an OpenAPI spec.
+client off an OpenAPI spec >= 3.0.
 
 ```mermaid
 flowchart LR
     generator["python-client-generator"]
     app["REST API app"]
     package["app HTTP client"]
 
     app -- "OpenAPI json" --> generator
     generator -- "generates" --> package
 ```
 
+> :warning: **Currently does not support OpenAPI 2.0**: PR for < 3.0 support are welcome
 
 ## Using the generator
 
 ```bash
 python -m python_client_generator --open-api openapi.json --package-name foo_bar --project-name foo-bar --outdir clients
 ```
 
@@ -62,11 +64,10 @@
                 body=patch_body,
                 contact_id=contact.id,
                 tenant=tenant,
                 body_serializer_args={"exclude_unset": True}
 )
 ```
 
-
 ## Contributing
 Please refer to [CONTRIBUTING.md](.github/CONTRIBUTING.md).
```

