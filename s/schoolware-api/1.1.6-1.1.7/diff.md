# Comparing `tmp/schoolware_api-1.1.6.tar.gz` & `tmp/schoolware_api-1.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "schoolware_api-1.1.6.tar", last modified: Fri May  5 11:20:33 2023, max compression
+gzip compressed data, was "schoolware_api-1.1.7.tar", last modified: Fri May  5 11:44:39 2023, max compression
```

## Comparing `schoolware_api-1.1.6.tar` & `schoolware_api-1.1.7.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 11:20:33.370460 schoolware_api-1.1.6/
--rw-r--r--   0 runner    (1001) docker     (123)     1988 2023-05-05 11:20:33.370460 schoolware_api-1.1.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1484 2023-05-05 11:20:22.000000 schoolware_api-1.1.6/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      701 2023-05-05 11:20:22.000000 schoolware_api-1.1.6/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 11:20:33.370460 schoolware_api-1.1.6/schoolware_api/
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-05-05 11:20:22.000000 schoolware_api-1.1.6/schoolware_api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13946 2023-05-05 11:20:22.000000 schoolware_api-1.1.6/schoolware_api/schoolware_api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 11:20:33.370460 schoolware_api-1.1.6/schoolware_api.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1988 2023-05-05 11:20:33.000000 schoolware_api-1.1.6/schoolware_api.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      282 2023-05-05 11:20:33.000000 schoolware_api-1.1.6/schoolware_api.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 11:20:33.000000 schoolware_api-1.1.6/schoolware_api.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-05-05 11:20:33.000000 schoolware_api-1.1.6/schoolware_api.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-05-05 11:20:33.000000 schoolware_api-1.1.6/schoolware_api.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-05 11:20:33.370460 schoolware_api-1.1.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      392 2023-05-05 11:20:22.000000 schoolware_api-1.1.6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 11:44:39.646146 schoolware_api-1.1.7/
+-rw-r--r--   0 runner    (1001) docker     (123)     1988 2023-05-05 11:44:39.646146 schoolware_api-1.1.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1484 2023-05-05 11:44:27.000000 schoolware_api-1.1.7/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      701 2023-05-05 11:44:27.000000 schoolware_api-1.1.7/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 11:44:39.646146 schoolware_api-1.1.7/schoolware_api/
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-05-05 11:44:27.000000 schoolware_api-1.1.7/schoolware_api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13976 2023-05-05 11:44:27.000000 schoolware_api-1.1.7/schoolware_api/schoolware_api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 11:44:39.646146 schoolware_api-1.1.7/schoolware_api.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1988 2023-05-05 11:44:39.000000 schoolware_api-1.1.7/schoolware_api.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      282 2023-05-05 11:44:39.000000 schoolware_api-1.1.7/schoolware_api.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 11:44:39.000000 schoolware_api-1.1.7/schoolware_api.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-05-05 11:44:39.000000 schoolware_api-1.1.7/schoolware_api.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-05-05 11:44:39.000000 schoolware_api-1.1.7/schoolware_api.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-05 11:44:39.646146 schoolware_api-1.1.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      392 2023-05-05 11:44:27.000000 schoolware_api-1.1.7/setup.py
```

### Comparing `schoolware_api-1.1.6/PKG-INFO` & `schoolware_api-1.1.7/schoolware_api.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: schoolware_api
-Version: 1.1.6
+Name: schoolware-api
+Version: 1.1.7
 Summary: A api for schoolware written in python
 Author: Maarten Buelens
 Author-email: MB <schoolware_api@mb-server.com>
 License: MIT
 Project-URL: Homepage, https://github.com/Maarten-buelens/schoolware_api
 Project-URL: Bug Tracker, https://github.com/Maarten-buelens/schoolware_api/issues
 Classifier: Programming Language :: Python :: 3
```

### Comparing `schoolware_api-1.1.6/README.md` & `schoolware_api-1.1.7/README.md`

 * *Files identical despite different names*

### Comparing `schoolware_api-1.1.6/pyproject.toml` & `schoolware_api-1.1.7/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "schoolware_api"
-version = "1.1.6"
+version = "1.1.7"
 authors = [
   { name="MB", email="schoolware_api@mb-server.com" },
 ]
 description = "A api for schoolware written in python"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `schoolware_api-1.1.6/schoolware_api/schoolware_api.py` & `schoolware_api-1.1.7/schoolware_api/schoolware_api.py`

 * *Files 0% similar despite different names*

```diff
@@ -333,14 +333,15 @@
     import telegram
     from time import sleep
     import asyncio
     
     self.bot = telegram.Bot(self.config["bot_token"])
     print(colored("telegram started","blue"))
     num_prev = len(self.scores)
+    scores_prev = self.scores
     while True:
         sleep(5*60)
         if(self.verbose):
             verbose_print(message=f"telegram checking", level="debug")
         scores_now = self.punten()
         num_now = len(scores_now)
         if(num_prev < num_now):
```

### Comparing `schoolware_api-1.1.6/schoolware_api.egg-info/PKG-INFO` & `schoolware_api-1.1.7/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: schoolware-api
-Version: 1.1.6
+Name: schoolware_api
+Version: 1.1.7
 Summary: A api for schoolware written in python
 Author: Maarten Buelens
 Author-email: MB <schoolware_api@mb-server.com>
 License: MIT
 Project-URL: Homepage, https://github.com/Maarten-buelens/schoolware_api
 Project-URL: Bug Tracker, https://github.com/Maarten-buelens/schoolware_api/issues
 Classifier: Programming Language :: Python :: 3
```

