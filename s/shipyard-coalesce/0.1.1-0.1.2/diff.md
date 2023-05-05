# Comparing `tmp/shipyard_coalesce-0.1.1.tar.gz` & `tmp/shipyard_coalesce-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shipyard_coalesce-0.1.1.tar", max compression
+gzip compressed data, was "shipyard_coalesce-0.1.2.tar", max compression
```

## Comparing `shipyard_coalesce-0.1.1.tar` & `shipyard_coalesce-0.1.2.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1098 2023-05-04 18:37:25.928580 shipyard_coalesce-0.1.1/README.md
--rw-r--r--   0        0        0      557 2023-05-04 23:37:09.893687 shipyard_coalesce-0.1.1/pyproject.toml
--rw-r--r--   0        0        0       36 2023-05-04 17:02:13.445484 shipyard_coalesce-0.1.1/shipyard_coalesce/__init__.py
--rw-r--r--   0        0        0     1182 2023-05-04 21:20:43.160884 shipyard_coalesce-0.1.1/shipyard_coalesce/cli/determine_status.py
--rw-r--r--   0        0        0     2308 2023-05-04 22:22:36.368929 shipyard_coalesce-0.1.1/shipyard_coalesce/cli/trigger_sync.py
--rw-r--r--   0        0        0     5682 2023-05-04 23:35:49.283240 shipyard_coalesce-0.1.1/shipyard_coalesce/coalesce.py
--rw-r--r--   0        0        0     1586 1970-01-01 00:00:00.000000 shipyard_coalesce-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1098 2023-05-04 18:37:25.928580 shipyard_coalesce-0.1.2/README.md
+-rw-r--r--   0        0        0      557 2023-05-05 02:20:31.274384 shipyard_coalesce-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0       36 2023-05-04 17:02:13.445484 shipyard_coalesce-0.1.2/shipyard_coalesce/__init__.py
+-rw-r--r--   0        0        0     1182 2023-05-04 21:20:43.160884 shipyard_coalesce-0.1.2/shipyard_coalesce/cli/determine_status.py
+-rw-r--r--   0        0        0     2492 2023-05-05 00:03:51.253151 shipyard_coalesce-0.1.2/shipyard_coalesce/cli/trigger_sync.py
+-rw-r--r--   0        0        0     5678 2023-05-05 02:19:47.302622 shipyard_coalesce-0.1.2/shipyard_coalesce/coalesce.py
+-rw-r--r--   0        0        0     1586 1970-01-01 00:00:00.000000 shipyard_coalesce-0.1.2/PKG-INFO
```

### Comparing `shipyard_coalesce-0.1.1/README.md` & `shipyard_coalesce-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `shipyard_coalesce-0.1.1/pyproject.toml` & `shipyard_coalesce-0.1.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "shipyard-coalesce"
-version = "0.1.1"
+version = "0.1.2"
 description = "A local client for connecting and working with Coalesce"
 authors = ["wrp801 <wespoulsen@gmail.com>"]
 readme = "README.md"
 packages = [{include = "shipyard_coalesce"}]
 
 [tool.poetry.dependencies]
 python = "^3.9"
```

### Comparing `shipyard_coalesce-0.1.1/shipyard_coalesce/cli/determine_status.py` & `shipyard_coalesce-0.1.2/shipyard_coalesce/cli/determine_status.py`

 * *Files identical despite different names*

### Comparing `shipyard_coalesce-0.1.1/shipyard_coalesce/cli/trigger_sync.py` & `shipyard_coalesce-0.1.2/shipyard_coalesce/cli/trigger_sync.py`

 * *Files 23% similar despite different names*

```diff
@@ -33,22 +33,22 @@
 
 
 def main():
     args = get_args()
     access_token = args.access_token
     sync_args = {
         "environment_id": args.environment_id,
-        "job_id": args.job_id,
+        "job_id": None if args.job_id == '' else args.job_id,
         "snowflake_username": args.snowflake_username,
         "snowflake_password": args.snowflake_password,
-        "snowflake_role": args.snowflake_role,
-        "snowflake_warehouse": args.snowflake_warehouse,
+        "snowflake_role": None if args.snowflake_role == '' else args.snowflake_role,
+        "snowflake_warehouse": None if args.snowflake_role == '' else args.snowflake_warehouse,
         "parallelism": args.parallelism,
-        "include_nodes_selector": args.include_nodes,
-        "exclude_nodes_selector": args.exclude_nodes,
+        "include_nodes_selector": None if args.include_nodes == '' else args.include_nodes,
+        "exclude_nodes_selector": None if args.exclude_nodes == '' else args.exclude_nodes
     }
     client = CoalesceClient(access_token)
     response = client.trigger_sync(**sync_args)
 
     # create artifacts folder to save response
     base_folder_name = shipyard.logs.determine_base_artifact_folder("coalesce")
     artifact_subfolder_paths = shipyard.logs.determine_artifact_subfolders(
```

### Comparing `shipyard_coalesce-0.1.1/shipyard_coalesce/coalesce.py` & `shipyard_coalesce-0.1.2/shipyard_coalesce/coalesce.py`

 * *Files 1% similar despite different names*

```diff
@@ -123,15 +123,15 @@
                 return self.EXIT_CODE_FINAL_STATUS_CANCELLED
             else:
                 self.logger.info(f"Status: {status}")
                 return self.EXIT_CODE_UNKNOWN_STATUS
 
         elif response.status_code == 400:
             self.logger.error(
-                f"There was an error when attempting to fetch the status of the job. The message returned from the API is {response['error']['errorString']}"
+                f"There was an error when attempting to fetch the status of the job. The message returned from the API is {json['error']['errorString']}"
             )
             return self.EXIT_CODE_BAD_REQUEST
 
         elif response.status_code == 401:
             self.logger.error(
                 "Error occurred when attempting to authenticate, please ensure that the token provided is valid"
             )
```

### Comparing `shipyard_coalesce-0.1.1/PKG-INFO` & `shipyard_coalesce-0.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shipyard-coalesce
-Version: 0.1.1
+Version: 0.1.2
 Summary: A local client for connecting and working with Coalesce
 Author: wrp801
 Author-email: wespoulsen@gmail.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

