# Comparing `tmp/apify_client-1.1.0a3.tar.gz` & `tmp/apify_client-1.1.0b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "apify_client-1.1.0a3.tar", last modified: Thu May  4 18:29:44 2023, max compression
+gzip compressed data, was "apify_client-1.1.0b1.tar", last modified: Fri May  5 07:14:22 2023, max compression
```

## Comparing `apify_client-1.1.0a3.tar` & `apify_client-1.1.0b1.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 18:29:44.646367 apify_client-1.1.0a3/
--rw-r--r--   0 runner    (1001) docker     (123)    11355 2023-05-04 18:29:08.000000 apify_client-1.1.0a3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4528 2023-05-04 18:29:44.646367 apify_client-1.1.0a3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3390 2023-05-04 18:29:08.000000 apify_client-1.1.0a3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     2309 2023-05-04 18:29:41.000000 apify_client-1.1.0a3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-04 18:29:44.646367 apify_client-1.1.0a3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 18:29:44.642367 apify_client-1.1.0a3/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 18:29:44.646367 apify_client-1.1.0a3/src/apify_client/
--rw-r--r--   0 runner    (1001) docker     (123)      192 2023-05-04 18:29:08.000000 apify_client-1.1.0a3/src/apify_client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2679 2023-05-04 18:29:08.000000 apify_client-1.1.0a3/src/apify_client/_errors.py
--rw-r--r--   0 runner    (1001) docker     (123)    10431 2023-05-04 18:29:08.000000 apify_client-1.1.0a3/src/apify_client/_http_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     4188 2023-05-04 18:29:08.000000 apify_client-1.1.0a3/src/apify_client/_logging.py
--rw-r--r--   0 runner    (1001) docker     (123)      405 2023-05-04 18:29:08.000000 apify_client-1.1.0a3/src/apify_client/_types.py
--rw-r--r--   0 runner    (1001) docker     (123)     9212 2023-05-04 18:29:08.000000 apify_client-1.1.0a3/src/apify_client/_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    17504 2023-05-04 18:29:08.000000 apify_client-1.1.0a3/src/apify_client/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     2875 2023-05-04 18:29:08.000000 apify_client-1.1.0a3/src/apify_client/consts.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 18:29:08.000000 apify_client-1.1.0a3/src/apify_client/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 18:29:44.646367 apify_client-1.1.0a3/src/apify_client.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4528 2023-05-04 18:29:44.000000 apify_client-1.1.0a3/src/apify_client.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      484 2023-05-04 18:29:44.000000 apify_client-1.1.0a3/src/apify_client.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-04 18:29:44.000000 apify_client-1.1.0a3/src/apify_client.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      601 2023-05-04 18:29:44.000000 apify_client-1.1.0a3/src/apify_client.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-04 18:29:44.000000 apify_client-1.1.0a3/src/apify_client.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 07:14:22.717162 apify_client-1.1.0b1/
+-rw-r--r--   0 runner    (1001) docker     (123)    11355 2023-05-05 07:13:40.000000 apify_client-1.1.0b1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4528 2023-05-05 07:14:22.717162 apify_client-1.1.0b1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3390 2023-05-05 07:13:40.000000 apify_client-1.1.0b1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2309 2023-05-05 07:14:18.000000 apify_client-1.1.0b1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-05 07:14:22.717162 apify_client-1.1.0b1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 07:14:22.717162 apify_client-1.1.0b1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 07:14:22.717162 apify_client-1.1.0b1/src/apify_client/
+-rw-r--r--   0 runner    (1001) docker     (123)      192 2023-05-05 07:13:40.000000 apify_client-1.1.0b1/src/apify_client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2679 2023-05-05 07:13:40.000000 apify_client-1.1.0b1/src/apify_client/_errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10431 2023-05-05 07:13:40.000000 apify_client-1.1.0b1/src/apify_client/_http_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4188 2023-05-05 07:13:40.000000 apify_client-1.1.0b1/src/apify_client/_logging.py
+-rw-r--r--   0 runner    (1001) docker     (123)      405 2023-05-05 07:13:40.000000 apify_client-1.1.0b1/src/apify_client/_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9212 2023-05-05 07:13:40.000000 apify_client-1.1.0b1/src/apify_client/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17504 2023-05-05 07:13:40.000000 apify_client-1.1.0b1/src/apify_client/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2875 2023-05-05 07:13:40.000000 apify_client-1.1.0b1/src/apify_client/consts.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 07:13:40.000000 apify_client-1.1.0b1/src/apify_client/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 07:14:22.717162 apify_client-1.1.0b1/src/apify_client.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4528 2023-05-05 07:14:22.000000 apify_client-1.1.0b1/src/apify_client.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      484 2023-05-05 07:14:22.000000 apify_client-1.1.0b1/src/apify_client.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 07:14:22.000000 apify_client-1.1.0b1/src/apify_client.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      601 2023-05-05 07:14:22.000000 apify_client-1.1.0b1/src/apify_client.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-05 07:14:22.000000 apify_client-1.1.0b1/src/apify_client.egg-info/top_level.txt
```

### Comparing `apify_client-1.1.0a3/LICENSE` & `apify_client-1.1.0b1/LICENSE`

 * *Files identical despite different names*

### Comparing `apify_client-1.1.0a3/PKG-INFO` & `apify_client-1.1.0b1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apify_client
-Version: 1.1.0a3
+Version: 1.1.0b1
 Summary: Apify API client for Python
 Author-email: "Apify Technologies s.r.o." <support@apify.com>
 License: Apache Software License
 Project-URL: Homepage, https://docs.apify.com/api/client/python/
 Project-URL: Documentation, https://docs.apify.com/api/client/python/
 Project-URL: Source, https://github.com/apify/apify-client-python
 Project-URL: Issue tracker, https://github.com/apify/apify-client-python/issues
```

### Comparing `apify_client-1.1.0a3/README.md` & `apify_client-1.1.0b1/README.md`

 * *Files identical despite different names*

### Comparing `apify_client-1.1.0a3/pyproject.toml` & `apify_client-1.1.0b1/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 [project]
 
 name = "apify_client"
 
-version = "1.1.0a3"
+version = "1.1.0b1"
 description = "Apify API client for Python"
 
 readme = "README.md"
 
 license = {text = "Apache Software License"}
 
 authors = [
```

### Comparing `apify_client-1.1.0a3/src/apify_client/_errors.py` & `apify_client-1.1.0b1/src/apify_client/_errors.py`

 * *Files identical despite different names*

### Comparing `apify_client-1.1.0a3/src/apify_client/_http_client.py` & `apify_client-1.1.0b1/src/apify_client/_http_client.py`

 * *Files identical despite different names*

### Comparing `apify_client-1.1.0a3/src/apify_client/_logging.py` & `apify_client-1.1.0b1/src/apify_client/_logging.py`

 * *Files identical despite different names*

### Comparing `apify_client-1.1.0a3/src/apify_client/_utils.py` & `apify_client-1.1.0b1/src/apify_client/_utils.py`

 * *Files identical despite different names*

### Comparing `apify_client-1.1.0a3/src/apify_client/client.py` & `apify_client-1.1.0b1/src/apify_client/client.py`

 * *Files identical despite different names*

### Comparing `apify_client-1.1.0a3/src/apify_client/consts.py` & `apify_client-1.1.0b1/src/apify_client/consts.py`

 * *Files identical despite different names*

### Comparing `apify_client-1.1.0a3/src/apify_client.egg-info/PKG-INFO` & `apify_client-1.1.0b1/src/apify_client.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: apify-client
-Version: 1.1.0a3
+Version: 1.1.0b1
 Summary: Apify API client for Python
 Author-email: "Apify Technologies s.r.o." <support@apify.com>
 License: Apache Software License
 Project-URL: Homepage, https://docs.apify.com/api/client/python/
 Project-URL: Documentation, https://docs.apify.com/api/client/python/
 Project-URL: Source, https://github.com/apify/apify-client-python
 Project-URL: Issue tracker, https://github.com/apify/apify-client-python/issues
```

### Comparing `apify_client-1.1.0a3/src/apify_client.egg-info/requires.txt` & `apify_client-1.1.0b1/src/apify_client.egg-info/requires.txt`

 * *Files identical despite different names*

