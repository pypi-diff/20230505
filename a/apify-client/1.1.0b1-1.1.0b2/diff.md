# Comparing `tmp/apify_client-1.1.0b1.tar.gz` & `tmp/apify_client-1.1.0b2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "apify_client-1.1.0b1.tar", last modified: Fri May  5 07:14:22 2023, max compression
+gzip compressed data, was "apify_client-1.1.0b2.tar", last modified: Fri May  5 08:13:10 2023, max compression
```

## Comparing `apify_client-1.1.0b1.tar` & `apify_client-1.1.0b2.tar`

### file list

```diff
@@ -1,23 +1,59 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 07:14:22.717162 apify_client-1.1.0b1/
--rw-r--r--   0 runner    (1001) docker     (123)    11355 2023-05-05 07:13:40.000000 apify_client-1.1.0b1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4528 2023-05-05 07:14:22.717162 apify_client-1.1.0b1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3390 2023-05-05 07:13:40.000000 apify_client-1.1.0b1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     2309 2023-05-05 07:14:18.000000 apify_client-1.1.0b1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-05 07:14:22.717162 apify_client-1.1.0b1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 07:14:22.717162 apify_client-1.1.0b1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 07:14:22.717162 apify_client-1.1.0b1/src/apify_client/
--rw-r--r--   0 runner    (1001) docker     (123)      192 2023-05-05 07:13:40.000000 apify_client-1.1.0b1/src/apify_client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2679 2023-05-05 07:13:40.000000 apify_client-1.1.0b1/src/apify_client/_errors.py
--rw-r--r--   0 runner    (1001) docker     (123)    10431 2023-05-05 07:13:40.000000 apify_client-1.1.0b1/src/apify_client/_http_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     4188 2023-05-05 07:13:40.000000 apify_client-1.1.0b1/src/apify_client/_logging.py
--rw-r--r--   0 runner    (1001) docker     (123)      405 2023-05-05 07:13:40.000000 apify_client-1.1.0b1/src/apify_client/_types.py
--rw-r--r--   0 runner    (1001) docker     (123)     9212 2023-05-05 07:13:40.000000 apify_client-1.1.0b1/src/apify_client/_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    17504 2023-05-05 07:13:40.000000 apify_client-1.1.0b1/src/apify_client/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     2875 2023-05-05 07:13:40.000000 apify_client-1.1.0b1/src/apify_client/consts.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 07:13:40.000000 apify_client-1.1.0b1/src/apify_client/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 07:14:22.717162 apify_client-1.1.0b1/src/apify_client.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4528 2023-05-05 07:14:22.000000 apify_client-1.1.0b1/src/apify_client.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      484 2023-05-05 07:14:22.000000 apify_client-1.1.0b1/src/apify_client.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 07:14:22.000000 apify_client-1.1.0b1/src/apify_client.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      601 2023-05-05 07:14:22.000000 apify_client-1.1.0b1/src/apify_client.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-05 07:14:22.000000 apify_client-1.1.0b1/src/apify_client.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 08:13:10.919109 apify_client-1.1.0b2/
+-rw-r--r--   0 runner    (1001) docker     (123)    11355 2023-05-05 08:12:24.000000 apify_client-1.1.0b2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4528 2023-05-05 08:13:10.919109 apify_client-1.1.0b2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3390 2023-05-05 08:12:24.000000 apify_client-1.1.0b2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2310 2023-05-05 08:13:06.000000 apify_client-1.1.0b2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-05 08:13:10.919109 apify_client-1.1.0b2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 08:13:10.907109 apify_client-1.1.0b2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 08:13:10.911109 apify_client-1.1.0b2/src/apify_client/
+-rw-r--r--   0 runner    (1001) docker     (123)      192 2023-05-05 08:12:24.000000 apify_client-1.1.0b2/src/apify_client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2679 2023-05-05 08:12:24.000000 apify_client-1.1.0b2/src/apify_client/_errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10431 2023-05-05 08:12:24.000000 apify_client-1.1.0b2/src/apify_client/_http_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4188 2023-05-05 08:12:24.000000 apify_client-1.1.0b2/src/apify_client/_logging.py
+-rw-r--r--   0 runner    (1001) docker     (123)      405 2023-05-05 08:12:24.000000 apify_client-1.1.0b2/src/apify_client/_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9212 2023-05-05 08:12:24.000000 apify_client-1.1.0b2/src/apify_client/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17504 2023-05-05 08:12:24.000000 apify_client-1.1.0b2/src/apify_client/client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 08:13:10.911109 apify_client-1.1.0b2/src/apify_client/clients/
+-rw-r--r--   0 runner    (1001) docker     (123)     3059 2023-05-05 08:12:24.000000 apify_client-1.1.0b2/src/apify_client/clients/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 08:13:10.915109 apify_client-1.1.0b2/src/apify_client/clients/base/
+-rw-r--r--   0 runner    (1001) docker     (123)      508 2023-05-05 08:12:24.000000 apify_client-1.1.0b2/src/apify_client/clients/base/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4944 2023-05-05 08:12:24.000000 apify_client-1.1.0b2/src/apify_client/clients/base/actor_job_base_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4399 2023-05-05 08:12:24.000000 apify_client-1.1.0b2/src/apify_client/clients/base/base_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2419 2023-05-05 08:12:24.000000 apify_client-1.1.0b2/src/apify_client/clients/base/resource_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2288 2023-05-05 08:12:24.000000 apify_client-1.1.0b2/src/apify_client/clients/base/resource_collection_client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 08:13:10.919109 apify_client-1.1.0b2/src/apify_client/clients/resource_clients/
+-rw-r--r--   0 runner    (1001) docker     (123)     3043 2023-05-05 08:12:24.000000 apify_client-1.1.0b2/src/apify_client/clients/resource_clients/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30492 2023-05-05 08:12:24.000000 apify_client-1.1.0b2/src/apify_client/clients/resource_clients/actor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9682 2023-05-05 08:12:24.000000 apify_client-1.1.0b2/src/apify_client/clients/resource_clients/actor_collection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4203 2023-05-05 08:12:24.000000 apify_client-1.1.0b2/src/apify_client/clients/resource_clients/actor_env_var.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3600 2023-05-05 08:12:24.000000 apify_client-1.1.0b2/src/apify_client/clients/resource_clients/actor_env_var_collection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9775 2023-05-05 08:12:24.000000 apify_client-1.1.0b2/src/apify_client/clients/resource_clients/actor_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7268 2023-05-05 08:12:24.000000 apify_client-1.1.0b2/src/apify_client/clients/resource_clients/actor_version_collection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3324 2023-05-05 08:12:24.000000 apify_client-1.1.0b2/src/apify_client/clients/resource_clients/build.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2792 2023-05-05 08:12:24.000000 apify_client-1.1.0b2/src/apify_client/clients/resource_clients/build_collection.py
+-rw-r--r--   0 runner    (1001) docker     (123)    46610 2023-05-05 08:12:24.000000 apify_client-1.1.0b2/src/apify_client/clients/resource_clients/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4163 2023-05-05 08:12:24.000000 apify_client-1.1.0b2/src/apify_client/clients/resource_clients/dataset_collection.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15646 2023-05-05 08:12:24.000000 apify_client-1.1.0b2/src/apify_client/clients/resource_clients/key_value_store.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4435 2023-05-05 08:12:24.000000 apify_client-1.1.0b2/src/apify_client/clients/resource_clients/key_value_store_collection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5035 2023-05-05 08:12:24.000000 apify_client-1.1.0b2/src/apify_client/clients/resource_clients/log.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10980 2023-05-05 08:12:24.000000 apify_client-1.1.0b2/src/apify_client/clients/resource_clients/request_queue.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3996 2023-05-05 08:12:24.000000 apify_client-1.1.0b2/src/apify_client/clients/resource_clients/request_queue_collection.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14114 2023-05-05 08:12:24.000000 apify_client-1.1.0b2/src/apify_client/clients/resource_clients/run.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3305 2023-05-05 08:12:24.000000 apify_client-1.1.0b2/src/apify_client/clients/resource_clients/run_collection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7686 2023-05-05 08:12:24.000000 apify_client-1.1.0b2/src/apify_client/clients/resource_clients/schedule.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6272 2023-05-05 08:12:24.000000 apify_client-1.1.0b2/src/apify_client/clients/resource_clients/schedule_collection.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21010 2023-05-05 08:12:24.000000 apify_client-1.1.0b2/src/apify_client/clients/resource_clients/task.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5912 2023-05-05 08:12:24.000000 apify_client-1.1.0b2/src/apify_client/clients/resource_clients/task_collection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1844 2023-05-05 08:12:24.000000 apify_client-1.1.0b2/src/apify_client/clients/resource_clients/user.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10414 2023-05-05 08:12:24.000000 apify_client-1.1.0b2/src/apify_client/clients/resource_clients/webhook.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8022 2023-05-05 08:12:24.000000 apify_client-1.1.0b2/src/apify_client/clients/resource_clients/webhook_collection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1628 2023-05-05 08:12:24.000000 apify_client-1.1.0b2/src/apify_client/clients/resource_clients/webhook_dispatch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2680 2023-05-05 08:12:24.000000 apify_client-1.1.0b2/src/apify_client/clients/resource_clients/webhook_dispatch_collection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2875 2023-05-05 08:12:24.000000 apify_client-1.1.0b2/src/apify_client/consts.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 08:12:24.000000 apify_client-1.1.0b2/src/apify_client/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 08:13:10.911109 apify_client-1.1.0b2/src/apify_client.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4528 2023-05-05 08:13:10.000000 apify_client-1.1.0b2/src/apify_client.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2379 2023-05-05 08:13:10.000000 apify_client-1.1.0b2/src/apify_client.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 08:13:10.000000 apify_client-1.1.0b2/src/apify_client.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      601 2023-05-05 08:13:10.000000 apify_client-1.1.0b2/src/apify_client.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-05 08:13:10.000000 apify_client-1.1.0b2/src/apify_client.egg-info/top_level.txt
```

### Comparing `apify_client-1.1.0b1/LICENSE` & `apify_client-1.1.0b2/LICENSE`

 * *Files identical despite different names*

### Comparing `apify_client-1.1.0b1/PKG-INFO` & `apify_client-1.1.0b2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apify_client
-Version: 1.1.0b1
+Version: 1.1.0b2
 Summary: Apify API client for Python
 Author-email: "Apify Technologies s.r.o." <support@apify.com>
 License: Apache Software License
 Project-URL: Homepage, https://docs.apify.com/api/client/python/
 Project-URL: Documentation, https://docs.apify.com/api/client/python/
 Project-URL: Source, https://github.com/apify/apify-client-python
 Project-URL: Issue tracker, https://github.com/apify/apify-client-python/issues
```

### Comparing `apify_client-1.1.0b1/README.md` & `apify_client-1.1.0b2/README.md`

 * *Files identical despite different names*

### Comparing `apify_client-1.1.0b1/pyproject.toml` & `apify_client-1.1.0b2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 [project]
 
 name = "apify_client"
 
-version = "1.1.0b1"
+version = "1.1.0b2"
 description = "Apify API client for Python"
 
 readme = "README.md"
 
 license = {text = "Apache Software License"}
 
 authors = [
@@ -139,14 +139,14 @@
 
 
 
 [tool.setuptools.packages.find]
 
 where = ["src"]
 
-include = ["apify_client"]
+include = ["apify_client*"]
 
 
 
 [tool.setuptools.package-data]
 
 apify_client = ["py.typed"]
```

### Comparing `apify_client-1.1.0b1/src/apify_client/_errors.py` & `apify_client-1.1.0b2/src/apify_client/_errors.py`

 * *Files identical despite different names*

### Comparing `apify_client-1.1.0b1/src/apify_client/_http_client.py` & `apify_client-1.1.0b2/src/apify_client/_http_client.py`

 * *Files identical despite different names*

### Comparing `apify_client-1.1.0b1/src/apify_client/_logging.py` & `apify_client-1.1.0b2/src/apify_client/_logging.py`

 * *Files identical despite different names*

### Comparing `apify_client-1.1.0b1/src/apify_client/_utils.py` & `apify_client-1.1.0b2/src/apify_client/_utils.py`

 * *Files identical despite different names*

### Comparing `apify_client-1.1.0b1/src/apify_client/client.py` & `apify_client-1.1.0b2/src/apify_client/client.py`

 * *Files identical despite different names*

### Comparing `apify_client-1.1.0b1/src/apify_client/consts.py` & `apify_client-1.1.0b2/src/apify_client/consts.py`

 * *Files identical despite different names*

### Comparing `apify_client-1.1.0b1/src/apify_client.egg-info/PKG-INFO` & `apify_client-1.1.0b2/src/apify_client.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apify-client
-Version: 1.1.0b1
+Version: 1.1.0b2
 Summary: Apify API client for Python
 Author-email: "Apify Technologies s.r.o." <support@apify.com>
 License: Apache Software License
 Project-URL: Homepage, https://docs.apify.com/api/client/python/
 Project-URL: Documentation, https://docs.apify.com/api/client/python/
 Project-URL: Source, https://github.com/apify/apify-client-python
 Project-URL: Issue tracker, https://github.com/apify/apify-client-python/issues
```

### Comparing `apify_client-1.1.0b1/src/apify_client.egg-info/requires.txt` & `apify_client-1.1.0b2/src/apify_client.egg-info/requires.txt`

 * *Files identical despite different names*

