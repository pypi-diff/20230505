# Comparing `tmp/schoolware_api-1.1.1.tar.gz` & `tmp/schoolware_api-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "schoolware_api-1.1.1.tar", last modified: Fri May  5 09:17:06 2023, max compression
+gzip compressed data, was "schoolware_api-1.1.2.tar", last modified: Fri May  5 09:57:34 2023, max compression
```

## Comparing `schoolware_api-1.1.1.tar` & `schoolware_api-1.1.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 09:17:06.191524 schoolware_api-1.1.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1988 2023-05-05 09:17:06.187524 schoolware_api-1.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1484 2023-05-05 09:16:50.000000 schoolware_api-1.1.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      701 2023-05-05 09:16:50.000000 schoolware_api-1.1.1/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 09:17:06.187524 schoolware_api-1.1.1/schoolware_api/
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-05-05 09:16:50.000000 schoolware_api-1.1.1/schoolware_api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13613 2023-05-05 09:16:50.000000 schoolware_api-1.1.1/schoolware_api/schoolware_api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 09:17:06.187524 schoolware_api-1.1.1/schoolware_api.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1988 2023-05-05 09:17:06.000000 schoolware_api-1.1.1/schoolware_api.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      282 2023-05-05 09:17:06.000000 schoolware_api-1.1.1/schoolware_api.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 09:17:06.000000 schoolware_api-1.1.1/schoolware_api.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-05-05 09:17:06.000000 schoolware_api-1.1.1/schoolware_api.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-05-05 09:17:06.000000 schoolware_api-1.1.1/schoolware_api.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-05 09:17:06.191524 schoolware_api-1.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      392 2023-05-05 09:16:50.000000 schoolware_api-1.1.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 09:57:34.449897 schoolware_api-1.1.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1988 2023-05-05 09:57:34.449897 schoolware_api-1.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1484 2023-05-05 09:57:20.000000 schoolware_api-1.1.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      701 2023-05-05 09:57:20.000000 schoolware_api-1.1.2/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 09:57:34.449897 schoolware_api-1.1.2/schoolware_api/
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-05-05 09:57:20.000000 schoolware_api-1.1.2/schoolware_api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13569 2023-05-05 09:57:20.000000 schoolware_api-1.1.2/schoolware_api/schoolware_api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 09:57:34.449897 schoolware_api-1.1.2/schoolware_api.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1988 2023-05-05 09:57:34.000000 schoolware_api-1.1.2/schoolware_api.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      282 2023-05-05 09:57:34.000000 schoolware_api-1.1.2/schoolware_api.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 09:57:34.000000 schoolware_api-1.1.2/schoolware_api.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-05-05 09:57:34.000000 schoolware_api-1.1.2/schoolware_api.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-05-05 09:57:34.000000 schoolware_api-1.1.2/schoolware_api.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-05 09:57:34.449897 schoolware_api-1.1.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      392 2023-05-05 09:57:20.000000 schoolware_api-1.1.2/setup.py
```

### Comparing `schoolware_api-1.1.1/PKG-INFO` & `schoolware_api-1.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: schoolware_api
-Version: 1.1.1
+Version: 1.1.2
 Summary: A api for schoolware written in python
 Author: Maarten Buelens
 Author-email: MB <schoolware_api@mb-server.com>
 License: MIT
 Project-URL: Homepage, https://github.com/Maarten-buelens/schoolware_api
 Project-URL: Bug Tracker, https://github.com/Maarten-buelens/schoolware_api/issues
 Classifier: Programming Language :: Python :: 3
```

### Comparing `schoolware_api-1.1.1/README.md` & `schoolware_api-1.1.2/README.md`

 * *Files identical despite different names*

### Comparing `schoolware_api-1.1.1/pyproject.toml` & `schoolware_api-1.1.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "schoolware_api"
-version = "1.1.1"
+version = "1.1.2"
 authors = [
   { name="MB", email="schoolware_api@mb-server.com" },
 ]
 description = "A api for schoolware written in python"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `schoolware_api-1.1.1/schoolware_api/schoolware_api.py` & `schoolware_api-1.1.2/schoolware_api/schoolware_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -17,15 +17,16 @@
         | user | school microsoft email
         | password | school microsoft password
         | bg | background procces to keep token valid
         | bot_token | telegram bot token to enable telegram bot
         | chat_id | id to send messages to
         | verbose | show a lot more info
         """
-#        verbose_print(self , message="starting schoolware_api",level="info")
+
+        logging.basicConfig(level=logging.DEBUG)
         self.config = config
         if("debug" in config):
             self.verbose = config["debug"]
         else:
             self.verbose = False
         if("verbose" in config):
             self.verbose = config["verbose"]
@@ -49,15 +50,15 @@
         self.user = self.config["user"]
         self.password = self.config["password"]
         self.token = ""
         self.cookie = ""
         self.rooster = []
         self.todo_list = []
         self.scores = []
-        verbose_print(self , message="starting schoolware_api",level="info")        
+        verbose_print(self , message="starting schoolware_api",level=1)        
         if(self.verbose):
             print("getting startup token")
         self.check_if_valid()
         self.num_points = len(self.punten())
         self.scores_prev = self.scores
         
 #Token&cookie stuff
@@ -354,24 +355,24 @@
     Args:
         msg (string): the message to send in telegram msg
     """
     async with self.bot:
         await self.bot.send_message(text=msg, chat_id=self.config["chat_id"])
 
 ##########VERBOSE##########
-def verbose_print(self,message, level="debug"):
+def verbose_print(self,message, level=0):
     """To print a message when verbose is set also times function
 
     Args:
         message (string): name of function to display
     """
     if(self.verbose):
         logging.debug(f"starting {message}")
 
-    if(level == "info"):
+    if(level == 1):
         logging.info(f"{message}")
 
 def verbose_end(self,message):
     """Ends verbose_print with done and the time for the function
 
     Args:
         message (string): name of function to display
```

### Comparing `schoolware_api-1.1.1/schoolware_api.egg-info/PKG-INFO` & `schoolware_api-1.1.2/schoolware_api.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: schoolware-api
-Version: 1.1.1
+Version: 1.1.2
 Summary: A api for schoolware written in python
 Author: Maarten Buelens
 Author-email: MB <schoolware_api@mb-server.com>
 License: MIT
 Project-URL: Homepage, https://github.com/Maarten-buelens/schoolware_api
 Project-URL: Bug Tracker, https://github.com/Maarten-buelens/schoolware_api/issues
 Classifier: Programming Language :: Python :: 3
```

