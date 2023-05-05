# Comparing `tmp/tyba_client-0.2.1.tar.gz` & `tmp/tyba_client-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tyba_client-0.2.1.tar", max compression
+gzip compressed data, was "tyba_client-0.2.2.tar", max compression
```

## Comparing `tyba_client-0.2.1.tar` & `tyba_client-0.2.2.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1079 2021-11-05 19:13:19.360928 tyba_client-0.2.1/LICENSE
--rw-r--r--   0        0        0       17 2023-03-20 18:44:14.006817 tyba_client-0.2.1/README.md
--rw-r--r--   0        0        0      626 2023-04-26 00:52:01.121997 tyba_client-0.2.1/pyproject.toml
--rw-r--r--   0        0        0       22 2021-11-05 19:13:19.364928 tyba_client-0.2.1/tyba_client/__init__.py
--rw-r--r--   0        0        0     5187 2023-04-26 00:51:50.367119 tyba_client-0.2.1/tyba_client/client.py
--rw-r--r--   0        0        0    17644 2023-03-28 18:50:42.287839 tyba_client-0.2.1/tyba_client/models.py
--rw-r--r--   0        0        0     2037 2021-11-10 00:29:24.081096 tyba_client-0.2.1/tyba_client/utils.py
--rw-r--r--   0        0        0      857 1970-01-01 00:00:00.000000 tyba_client-0.2.1/setup.py
--rw-r--r--   0        0        0      889 1970-01-01 00:00:00.000000 tyba_client-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0     1079 2021-11-05 19:13:19.360928 tyba_client-0.2.2/LICENSE
+-rw-r--r--   0        0        0       17 2023-03-20 18:44:14.006817 tyba_client-0.2.2/README.md
+-rw-r--r--   0        0        0      626 2023-05-05 20:51:39.595475 tyba_client-0.2.2/pyproject.toml
+-rw-r--r--   0        0        0       22 2021-11-05 19:13:19.364928 tyba_client-0.2.2/tyba_client/__init__.py
+-rw-r--r--   0        0        0     5526 2023-05-05 20:51:05.755185 tyba_client-0.2.2/tyba_client/client.py
+-rw-r--r--   0        0        0    17644 2023-03-28 18:50:42.287839 tyba_client-0.2.2/tyba_client/models.py
+-rw-r--r--   0        0        0     2037 2021-11-10 00:29:24.081096 tyba_client-0.2.2/tyba_client/utils.py
+-rw-r--r--   0        0        0      857 1970-01-01 00:00:00.000000 tyba_client-0.2.2/setup.py
+-rw-r--r--   0        0        0      889 1970-01-01 00:00:00.000000 tyba_client-0.2.2/PKG-INFO
```

### Comparing `tyba_client-0.2.1/LICENSE` & `tyba_client-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `tyba_client-0.2.1/pyproject.toml` & `tyba_client-0.2.2/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "tyba-client"
-version = "0.2.1"
+version = "0.2.2"
 description = "A Python API client for the Tyba Public API"
 authors = ["Tyler Nisonoff <tyler@tybaenergy.com>"]
 license = "MIT"
 readme = "README.md"
 include = [
     "LICENSE",
 ]
```

### Comparing `tyba_client-0.2.1/tyba_client/client.py` & `tyba_client-0.2.2/tyba_client/client.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 import pandas as pd
+from requests import Response
 
 from tyba_client.models import GenerationModel, PVStorageModel, StandaloneStorageModel
 from generation_models import JobModel
 import json
 import requests
 import time
 from structlog import get_logger
+from typing import Callable
 
 logger = get_logger()
 
 
 class Ancillary(object):
     def __init__(self, prices):
         self.prices = prices
@@ -113,36 +115,43 @@
     def get_status(self, run_id: str):
         url = "get-status/" + run_id
         return self.get(url)
 
     def get_status_v1(self, run_id: str):
         return self.get(f"get-status/{run_id}", params={"fmt": "v1"})
 
-    def wait_on_result(self, run_id: str, wait_time: int = 5, log_progress: bool = False):
+    @staticmethod
+    def _wait_on_result(run_id: str, wait_time: int, log_progress: bool, getter: Callable[[str], Response]):
         while True:
-            res = self.get_status(run_id).json()
+            resp = getter(run_id)
+            resp.raise_for_status()
+            res = resp.json()
             if res["status"] == "complete":
                 return res["result"]
             elif res["status"] == "unknown":
                 raise UnknownRunId(f"No known model run with run_id '{run_id}'")
             message = {
                 "status": res["status"]
             }
             if res.get("progress") is not None:
                 message["progress"] = f"{float(res['progress']) * 100:3.1f}%"
             if log_progress:
                 logger.info("waiting on result", **message)
             time.sleep(wait_time)
 
+    def wait_on_result(self, run_id: str, wait_time: int = 5, log_progress: bool = False):
+        return self._wait_on_result(run_id, wait_time, log_progress, getter=self.get_status)
+
     def wait_on_result_v1(self, run_id: str, wait_time: int = 5, log_progress: bool = False):
-        res = self.wait_on_result(run_id, wait_time, log_progress)
+        res = self._wait_on_result(run_id, wait_time, log_progress, getter=self.get_status_v1)
         return parse_v1_result(res)
 
+
 def parse_v1_result(res: dict):
     return {
-        "hourly": pd.concat({k: pd.DataFrame(v) for k, v in res["result"]["hourly"].items()}, axis=1),
-        "waterfall": res["result"]["waterfall"]
+        "hourly": pd.concat({k: pd.DataFrame(v) for k, v in res["hourly"].items()}, axis=1),
+        "waterfall": res["waterfall"]
     }
 
 
 class UnknownRunId(ValueError):
     pass
```

### Comparing `tyba_client-0.2.1/tyba_client/models.py` & `tyba_client-0.2.2/tyba_client/models.py`

 * *Files identical despite different names*

### Comparing `tyba_client-0.2.1/tyba_client/utils.py` & `tyba_client-0.2.2/tyba_client/utils.py`

 * *Files identical despite different names*

### Comparing `tyba_client-0.2.1/setup.py` & `tyba_client-0.2.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,15 +14,15 @@
  'pandas>=1.3.2,<2.0.0',
  'requests>=2.25.1,<3.0.0',
  'structlog>=23.1.0,<24.0.0',
  'tyba-financial-model>=0.1.0,<0.2.0']
 
 setup_kwargs = {
     'name': 'tyba-client',
-    'version': '0.2.1',
+    'version': '0.2.2',
     'description': 'A Python API client for the Tyba Public API',
     'long_description': '# Tyba API Client',
     'author': 'Tyler Nisonoff',
     'author_email': 'tyler@tybaenergy.com',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'None',
```

### Comparing `tyba_client-0.2.1/PKG-INFO` & `tyba_client-0.2.2/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tyba-client
-Version: 0.2.1
+Version: 0.2.2
 Summary: A Python API client for the Tyba Public API
 License: MIT
 Author: Tyler Nisonoff
 Author-email: tyler@tybaenergy.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

