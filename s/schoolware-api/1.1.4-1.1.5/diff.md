# Comparing `tmp/schoolware_api-1.1.4.tar.gz` & `tmp/schoolware_api-1.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "schoolware_api-1.1.4.tar", last modified: Fri May  5 10:09:30 2023, max compression
+gzip compressed data, was "schoolware_api-1.1.5.tar", last modified: Fri May  5 11:12:59 2023, max compression
```

## Comparing `schoolware_api-1.1.4.tar` & `schoolware_api-1.1.5.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 10:09:30.375385 schoolware_api-1.1.4/
--rw-r--r--   0 runner    (1001) docker     (123)     1988 2023-05-05 10:09:30.375385 schoolware_api-1.1.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1484 2023-05-05 10:09:13.000000 schoolware_api-1.1.4/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      701 2023-05-05 10:09:13.000000 schoolware_api-1.1.4/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 10:09:30.375385 schoolware_api-1.1.4/schoolware_api/
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-05-05 10:09:13.000000 schoolware_api-1.1.4/schoolware_api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13850 2023-05-05 10:09:13.000000 schoolware_api-1.1.4/schoolware_api/schoolware_api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 10:09:30.375385 schoolware_api-1.1.4/schoolware_api.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1988 2023-05-05 10:09:30.000000 schoolware_api-1.1.4/schoolware_api.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      282 2023-05-05 10:09:30.000000 schoolware_api-1.1.4/schoolware_api.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 10:09:30.000000 schoolware_api-1.1.4/schoolware_api.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-05-05 10:09:30.000000 schoolware_api-1.1.4/schoolware_api.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-05-05 10:09:30.000000 schoolware_api-1.1.4/schoolware_api.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-05 10:09:30.375385 schoolware_api-1.1.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      392 2023-05-05 10:09:13.000000 schoolware_api-1.1.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 11:12:59.618101 schoolware_api-1.1.5/
+-rw-r--r--   0 runner    (1001) docker     (123)     1988 2023-05-05 11:12:59.618101 schoolware_api-1.1.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1484 2023-05-05 11:12:45.000000 schoolware_api-1.1.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      701 2023-05-05 11:12:45.000000 schoolware_api-1.1.5/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 11:12:59.614101 schoolware_api-1.1.5/schoolware_api/
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-05-05 11:12:45.000000 schoolware_api-1.1.5/schoolware_api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13934 2023-05-05 11:12:45.000000 schoolware_api-1.1.5/schoolware_api/schoolware_api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 11:12:59.614101 schoolware_api-1.1.5/schoolware_api.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1988 2023-05-05 11:12:59.000000 schoolware_api-1.1.5/schoolware_api.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      282 2023-05-05 11:12:59.000000 schoolware_api-1.1.5/schoolware_api.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 11:12:59.000000 schoolware_api-1.1.5/schoolware_api.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-05-05 11:12:59.000000 schoolware_api-1.1.5/schoolware_api.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-05-05 11:12:59.000000 schoolware_api-1.1.5/schoolware_api.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-05 11:12:59.618101 schoolware_api-1.1.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      392 2023-05-05 11:12:45.000000 schoolware_api-1.1.5/setup.py
```

### Comparing `schoolware_api-1.1.4/PKG-INFO` & `schoolware_api-1.1.5/schoolware_api.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: schoolware_api
-Version: 1.1.4
+Name: schoolware-api
+Version: 1.1.5
 Summary: A api for schoolware written in python
 Author: Maarten Buelens
 Author-email: MB <schoolware_api@mb-server.com>
 License: MIT
 Project-URL: Homepage, https://github.com/Maarten-buelens/schoolware_api
 Project-URL: Bug Tracker, https://github.com/Maarten-buelens/schoolware_api/issues
 Classifier: Programming Language :: Python :: 3
```

### Comparing `schoolware_api-1.1.4/README.md` & `schoolware_api-1.1.5/README.md`

 * *Files identical despite different names*

### Comparing `schoolware_api-1.1.4/pyproject.toml` & `schoolware_api-1.1.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "schoolware_api"
-version = "1.1.4"
+version = "1.1.5"
 authors = [
   { name="MB", email="schoolware_api@mb-server.com" },
 ]
 description = "A api for schoolware written in python"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `schoolware_api-1.1.4/schoolware_api/schoolware_api.py` & `schoolware_api-1.1.5/schoolware_api/schoolware_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -27,20 +27,20 @@
         if("debug" in config):
             self.verbose = config["debug"]
         else:
             self.verbose = False
         if("verbose" in config):
             self.verbose = config["verbose"]
             if(self.verbose):
-                logging.basicConfig(format='%(asctime)s - %(message)s', level=logging.DEBUG)
+                logging.basicConfig(format='[%(level)s] %(asctime)s - %(message)s', level=logging.DEBUG)
             else:
-                logging.basicConfig(format='%(asctime)s - %(message)s', level=logging.INFO)
+                logging.basicConfig(format='[%(level)s] %(asctime)s - %(message)s', level=logging.INFO)
         else:
             self.verbose = False
-            logging.basicConfig(format='%(asctime)s - %(message)s', level=logging.INFO)
+            logging.basicConfig(format='[%(level)s] %(asctime)s - %(message)s', level=logging.INFO)
         if("bg" in config):
             self.bg = config["bg"]
         else:
             self.bg = False
         
         if(self.bg):
             self.bg_p = threading.Thread(target=bg, args=(self,))
@@ -332,18 +332,19 @@
     """
     import telegram
     from time import sleep
     import asyncio
     
     self.bot = telegram.Bot(self.config["bot_token"])
     print(colored("telegram started","blue"))
+    num_prev = len(self.scores)
     while True:
         sleep(5*60)
         if(self.verbose):
-            print(colored("telegram checking","blue"))
+            verbose_print(message=f"telegram checking", level="debug")
         scores_now = self.punten()
         num_now = len(scores_now)
         if(num_prev < num_now):
             diff_list = [i for i in scores_now if i not in scores_prev]
             diff = len(diff_list)
             num_prev = num_now
             scores_prev = scores_now
```

### Comparing `schoolware_api-1.1.4/schoolware_api.egg-info/PKG-INFO` & `schoolware_api-1.1.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: schoolware-api
-Version: 1.1.4
+Name: schoolware_api
+Version: 1.1.5
 Summary: A api for schoolware written in python
 Author: Maarten Buelens
 Author-email: MB <schoolware_api@mb-server.com>
 License: MIT
 Project-URL: Homepage, https://github.com/Maarten-buelens/schoolware_api
 Project-URL: Bug Tracker, https://github.com/Maarten-buelens/schoolware_api/issues
 Classifier: Programming Language :: Python :: 3
```

