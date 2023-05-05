# Comparing `tmp/schoolware_api-1.1.2.tar.gz` & `tmp/schoolware_api-1.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "schoolware_api-1.1.2.tar", last modified: Fri May  5 09:57:34 2023, max compression
+gzip compressed data, was "schoolware_api-1.1.3.tar", last modified: Fri May  5 10:00:39 2023, max compression
```

## Comparing `schoolware_api-1.1.2.tar` & `schoolware_api-1.1.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 09:57:34.449897 schoolware_api-1.1.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1988 2023-05-05 09:57:34.449897 schoolware_api-1.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1484 2023-05-05 09:57:20.000000 schoolware_api-1.1.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      701 2023-05-05 09:57:20.000000 schoolware_api-1.1.2/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 09:57:34.449897 schoolware_api-1.1.2/schoolware_api/
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-05-05 09:57:20.000000 schoolware_api-1.1.2/schoolware_api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13569 2023-05-05 09:57:20.000000 schoolware_api-1.1.2/schoolware_api/schoolware_api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 09:57:34.449897 schoolware_api-1.1.2/schoolware_api.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1988 2023-05-05 09:57:34.000000 schoolware_api-1.1.2/schoolware_api.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      282 2023-05-05 09:57:34.000000 schoolware_api-1.1.2/schoolware_api.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 09:57:34.000000 schoolware_api-1.1.2/schoolware_api.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-05-05 09:57:34.000000 schoolware_api-1.1.2/schoolware_api.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-05-05 09:57:34.000000 schoolware_api-1.1.2/schoolware_api.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-05 09:57:34.449897 schoolware_api-1.1.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      392 2023-05-05 09:57:20.000000 schoolware_api-1.1.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 10:00:39.363437 schoolware_api-1.1.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1988 2023-05-05 10:00:39.363437 schoolware_api-1.1.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1484 2023-05-05 10:00:23.000000 schoolware_api-1.1.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      701 2023-05-05 10:00:23.000000 schoolware_api-1.1.3/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 10:00:39.363437 schoolware_api-1.1.3/schoolware_api/
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-05-05 10:00:23.000000 schoolware_api-1.1.3/schoolware_api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13634 2023-05-05 10:00:23.000000 schoolware_api-1.1.3/schoolware_api/schoolware_api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 10:00:39.363437 schoolware_api-1.1.3/schoolware_api.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1988 2023-05-05 10:00:39.000000 schoolware_api-1.1.3/schoolware_api.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      282 2023-05-05 10:00:39.000000 schoolware_api-1.1.3/schoolware_api.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 10:00:39.000000 schoolware_api-1.1.3/schoolware_api.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-05-05 10:00:39.000000 schoolware_api-1.1.3/schoolware_api.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-05-05 10:00:39.000000 schoolware_api-1.1.3/schoolware_api.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-05 10:00:39.363437 schoolware_api-1.1.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      392 2023-05-05 10:00:23.000000 schoolware_api-1.1.3/setup.py
```

### Comparing `schoolware_api-1.1.2/PKG-INFO` & `schoolware_api-1.1.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: schoolware_api
-Version: 1.1.2
+Version: 1.1.3
 Summary: A api for schoolware written in python
 Author: Maarten Buelens
 Author-email: MB <schoolware_api@mb-server.com>
 License: MIT
 Project-URL: Homepage, https://github.com/Maarten-buelens/schoolware_api
 Project-URL: Bug Tracker, https://github.com/Maarten-buelens/schoolware_api/issues
 Classifier: Programming Language :: Python :: 3
```

### Comparing `schoolware_api-1.1.2/README.md` & `schoolware_api-1.1.3/README.md`

 * *Files identical despite different names*

### Comparing `schoolware_api-1.1.2/pyproject.toml` & `schoolware_api-1.1.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "schoolware_api"
-version = "1.1.2"
+version = "1.1.3"
 authors = [
   { name="MB", email="schoolware_api@mb-server.com" },
 ]
 description = "A api for schoolware written in python"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `schoolware_api-1.1.2/schoolware_api/schoolware_api.py` & `schoolware_api-1.1.3/schoolware_api/schoolware_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,24 +18,26 @@
         | password | school microsoft password
         | bg | background procces to keep token valid
         | bot_token | telegram bot token to enable telegram bot
         | chat_id | id to send messages to
         | verbose | show a lot more info
         """
 
-        logging.basicConfig(level=logging.DEBUG)
+        
         self.config = config
         if("debug" in config):
             self.verbose = config["debug"]
         else:
             self.verbose = False
         if("verbose" in config):
             self.verbose = config["verbose"]
+            logging.basicConfig(level=logging.DEBUG)
         else:
             self.verbose = False
+            logging.basicConfig(level=logging.INFO)
         if("bg" in config):
             self.bg = config["bg"]
         else:
             self.bg = False
         
         if(self.bg):
             self.bg_p = threading.Thread(target=bg, args=(self,))
```

### Comparing `schoolware_api-1.1.2/schoolware_api.egg-info/PKG-INFO` & `schoolware_api-1.1.3/schoolware_api.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: schoolware-api
-Version: 1.1.2
+Version: 1.1.3
 Summary: A api for schoolware written in python
 Author: Maarten Buelens
 Author-email: MB <schoolware_api@mb-server.com>
 License: MIT
 Project-URL: Homepage, https://github.com/Maarten-buelens/schoolware_api
 Project-URL: Bug Tracker, https://github.com/Maarten-buelens/schoolware_api/issues
 Classifier: Programming Language :: Python :: 3
```

