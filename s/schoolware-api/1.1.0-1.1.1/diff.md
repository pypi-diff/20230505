# Comparing `tmp/schoolware_api-1.1.0.tar.gz` & `tmp/schoolware_api-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "schoolware_api-1.1.0.tar", last modified: Fri May  5 08:11:56 2023, max compression
+gzip compressed data, was "schoolware_api-1.1.1.tar", last modified: Fri May  5 09:17:06 2023, max compression
```

## Comparing `schoolware_api-1.1.0.tar` & `schoolware_api-1.1.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 08:11:56.608121 schoolware_api-1.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1988 2023-05-05 08:11:56.608121 schoolware_api-1.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1484 2023-05-05 08:11:42.000000 schoolware_api-1.1.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      701 2023-05-05 08:11:42.000000 schoolware_api-1.1.0/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 08:11:56.608121 schoolware_api-1.1.0/schoolware_api/
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-05-05 08:11:42.000000 schoolware_api-1.1.0/schoolware_api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13606 2023-05-05 08:11:42.000000 schoolware_api-1.1.0/schoolware_api/schoolware_api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 08:11:56.608121 schoolware_api-1.1.0/schoolware_api.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1988 2023-05-05 08:11:56.000000 schoolware_api-1.1.0/schoolware_api.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      282 2023-05-05 08:11:56.000000 schoolware_api-1.1.0/schoolware_api.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 08:11:56.000000 schoolware_api-1.1.0/schoolware_api.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-05-05 08:11:56.000000 schoolware_api-1.1.0/schoolware_api.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-05-05 08:11:56.000000 schoolware_api-1.1.0/schoolware_api.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-05 08:11:56.608121 schoolware_api-1.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      392 2023-05-05 08:11:42.000000 schoolware_api-1.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 09:17:06.191524 schoolware_api-1.1.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1988 2023-05-05 09:17:06.187524 schoolware_api-1.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1484 2023-05-05 09:16:50.000000 schoolware_api-1.1.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      701 2023-05-05 09:16:50.000000 schoolware_api-1.1.1/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 09:17:06.187524 schoolware_api-1.1.1/schoolware_api/
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-05-05 09:16:50.000000 schoolware_api-1.1.1/schoolware_api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13613 2023-05-05 09:16:50.000000 schoolware_api-1.1.1/schoolware_api/schoolware_api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 09:17:06.187524 schoolware_api-1.1.1/schoolware_api.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1988 2023-05-05 09:17:06.000000 schoolware_api-1.1.1/schoolware_api.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      282 2023-05-05 09:17:06.000000 schoolware_api-1.1.1/schoolware_api.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 09:17:06.000000 schoolware_api-1.1.1/schoolware_api.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-05-05 09:17:06.000000 schoolware_api-1.1.1/schoolware_api.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-05-05 09:17:06.000000 schoolware_api-1.1.1/schoolware_api.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-05 09:17:06.191524 schoolware_api-1.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      392 2023-05-05 09:16:50.000000 schoolware_api-1.1.1/setup.py
```

### Comparing `schoolware_api-1.1.0/PKG-INFO` & `schoolware_api-1.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: schoolware_api
-Version: 1.1.0
+Version: 1.1.1
 Summary: A api for schoolware written in python
 Author: Maarten Buelens
 Author-email: MB <schoolware_api@mb-server.com>
 License: MIT
 Project-URL: Homepage, https://github.com/Maarten-buelens/schoolware_api
 Project-URL: Bug Tracker, https://github.com/Maarten-buelens/schoolware_api/issues
 Classifier: Programming Language :: Python :: 3
```

### Comparing `schoolware_api-1.1.0/README.md` & `schoolware_api-1.1.1/README.md`

 * *Files identical despite different names*

### Comparing `schoolware_api-1.1.0/pyproject.toml` & `schoolware_api-1.1.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "schoolware_api"
-version = "1.1.0"
+version = "1.1.1"
 authors = [
   { name="MB", email="schoolware_api@mb-server.com" },
 ]
 description = "A api for schoolware written in python"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `schoolware_api-1.1.0/schoolware_api/schoolware_api.py` & `schoolware_api-1.1.1/schoolware_api/schoolware_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -49,15 +49,15 @@
         self.user = self.config["user"]
         self.password = self.config["password"]
         self.token = ""
         self.cookie = ""
         self.rooster = []
         self.todo_list = []
         self.scores = []
-	verbose_print(self , message="starting schoolware_api",level="info")        
+        verbose_print(self , message="starting schoolware_api",level="info")        
         if(self.verbose):
             print("getting startup token")
         self.check_if_valid()
         self.num_points = len(self.punten())
         self.scores_prev = self.scores
         
 #Token&cookie stuff
```

### Comparing `schoolware_api-1.1.0/schoolware_api.egg-info/PKG-INFO` & `schoolware_api-1.1.1/schoolware_api.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: schoolware-api
-Version: 1.1.0
+Version: 1.1.1
 Summary: A api for schoolware written in python
 Author: Maarten Buelens
 Author-email: MB <schoolware_api@mb-server.com>
 License: MIT
 Project-URL: Homepage, https://github.com/Maarten-buelens/schoolware_api
 Project-URL: Bug Tracker, https://github.com/Maarten-buelens/schoolware_api/issues
 Classifier: Programming Language :: Python :: 3
```

