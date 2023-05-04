# Comparing `tmp/shipyard_coalesce-0.1.0.tar.gz` & `tmp/shipyard_coalesce-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shipyard_coalesce-0.1.0.tar", max compression
+gzip compressed data, was "shipyard_coalesce-0.1.1.tar", max compression
```

## Comparing `shipyard_coalesce-0.1.0.tar` & `shipyard_coalesce-0.1.1.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1098 2023-05-04 18:37:25.928580 shipyard_coalesce-0.1.0/README.md
--rw-r--r--   0        0        0      557 2023-05-04 14:31:47.660236 shipyard_coalesce-0.1.0/pyproject.toml
--rw-r--r--   0        0        0       36 2023-05-04 17:02:13.445484 shipyard_coalesce-0.1.0/shipyard_coalesce/__init__.py
--rw-r--r--   0        0        0     1182 2023-05-04 21:20:43.160884 shipyard_coalesce-0.1.0/shipyard_coalesce/cli/determine_status.py
--rw-r--r--   0        0        0     2308 2023-05-04 21:23:52.494413 shipyard_coalesce-0.1.0/shipyard_coalesce/cli/trigger_sync.py
--rw-r--r--   0        0        0     5668 2023-05-04 21:21:19.678287 shipyard_coalesce-0.1.0/shipyard_coalesce/coalesce.py
--rw-r--r--   0        0        0     1586 1970-01-01 00:00:00.000000 shipyard_coalesce-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1098 2023-05-04 18:37:25.928580 shipyard_coalesce-0.1.1/README.md
+-rw-r--r--   0        0        0      557 2023-05-04 23:37:09.893687 shipyard_coalesce-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0       36 2023-05-04 17:02:13.445484 shipyard_coalesce-0.1.1/shipyard_coalesce/__init__.py
+-rw-r--r--   0        0        0     1182 2023-05-04 21:20:43.160884 shipyard_coalesce-0.1.1/shipyard_coalesce/cli/determine_status.py
+-rw-r--r--   0        0        0     2308 2023-05-04 22:22:36.368929 shipyard_coalesce-0.1.1/shipyard_coalesce/cli/trigger_sync.py
+-rw-r--r--   0        0        0     5682 2023-05-04 23:35:49.283240 shipyard_coalesce-0.1.1/shipyard_coalesce/coalesce.py
+-rw-r--r--   0        0        0     1586 1970-01-01 00:00:00.000000 shipyard_coalesce-0.1.1/PKG-INFO
```

### Comparing `shipyard_coalesce-0.1.0/README.md` & `shipyard_coalesce-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `shipyard_coalesce-0.1.0/pyproject.toml` & `shipyard_coalesce-0.1.1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 [tool.poetry]
 name = "shipyard-coalesce"
-version = "0.1.0"
+version = "0.1.1"
 description = "A local client for connecting and working with Coalesce"
 authors = ["wrp801 <wespoulsen@gmail.com>"]
 readme = "README.md"
 packages = [{include = "shipyard_coalesce"}]
 
 [tool.poetry.dependencies]
 python = "^3.9"
-requests = "^2.29.0"
+requests = "^2.28.0"
 
 
 [tool.poetry.group.dev.dependencies]
 shipyard-templates = {path = "../../shipyard-templates"}
 shipyard-bp-utils = {path = "../shipyard-bp-utils"}
 black = "^23.3.0"
```

### Comparing `shipyard_coalesce-0.1.0/shipyard_coalesce/cli/determine_status.py` & `shipyard_coalesce-0.1.1/shipyard_coalesce/cli/determine_status.py`

 * *Files identical despite different names*

### Comparing `shipyard_coalesce-0.1.0/shipyard_coalesce/cli/trigger_sync.py` & `shipyard_coalesce-0.1.1/shipyard_coalesce/cli/trigger_sync.py`

 * *Files identical despite different names*

### Comparing `shipyard_coalesce-0.1.0/shipyard_coalesce/coalesce.py` & `shipyard_coalesce-0.1.1/shipyard_coalesce/coalesce.py`

 * *Files 2% similar despite different names*

```diff
@@ -65,16 +65,16 @@
 
         response = requests.post(url=url, json=payload, headers=headers)
 
         if response.status_code == 200:
             self.logger.info("Successfully triggered job")
 
         else:
-            self.logger.error(f"Error message: {response['error']['errorString']}")
-            self.logger.error(f"Error details: {response['error']['errorDetail']}")
+            self.logger.error(f"Error message: {response.json()['error']['errorString']}")
+            self.logger.error(f"Error details: {response.json()['error']['errorDetail']}")
 
         return response.json()
 
     def get_run_status(self, run_counter: int) -> requests.Response:
         """Returns the HTTP response for a Coalesce job status
 
         Args:
```

### Comparing `shipyard_coalesce-0.1.0/PKG-INFO` & `shipyard_coalesce-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: shipyard-coalesce
-Version: 0.1.0
+Version: 0.1.1
 Summary: A local client for connecting and working with Coalesce
 Author: wrp801
 Author-email: wespoulsen@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: requests (>=2.29.0,<3.0.0)
+Requires-Dist: requests (>=2.28.0,<3.0.0)
 Description-Content-Type: text/markdown
 
 # shipyard-coalesce
 
 ## Description 
 A local client to trigger Coalesce job's and check statuses of past runs
```

