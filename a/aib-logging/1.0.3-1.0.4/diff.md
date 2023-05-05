# Comparing `tmp/aib_logging-1.0.3.tar.gz` & `tmp/aib_logging-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aib_logging-1.0.3.tar", last modified: Fri May  5 10:13:57 2023, max compression
+gzip compressed data, was "aib_logging-1.0.4.tar", last modified: Fri May  5 10:57:49 2023, max compression
```

## Comparing `aib_logging-1.0.3.tar` & `aib_logging-1.0.4.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 akib_shaikh  (1000) akib_shaikh  (1000)        0 2023-05-05 10:13:57.329302 aib_logging-1.0.3/
--rw-r--r--   0 akib_shaikh  (1000) akib_shaikh  (1000)     1212 2023-03-28 08:02:11.000000 aib_logging-1.0.3/LICENSE.txt
--rw-r--r--   0 akib_shaikh  (1000) akib_shaikh  (1000)      528 2023-05-05 10:13:57.328302 aib_logging-1.0.3/PKG-INFO
--rw-r--r--   0 akib_shaikh  (1000) akib_shaikh  (1000)       20 2023-03-28 08:02:11.000000 aib_logging-1.0.3/README.md
--rw-r--r--   0 akib_shaikh  (1000) akib_shaikh  (1000)      639 2023-05-05 10:10:30.000000 aib_logging-1.0.3/pyproject.toml
--rw-r--r--   0 akib_shaikh  (1000) akib_shaikh  (1000)       38 2023-05-05 10:13:57.329302 aib_logging-1.0.3/setup.cfg
-drwxr-xr-x   0 akib_shaikh  (1000) akib_shaikh  (1000)        0 2023-05-05 10:13:57.323301 aib_logging-1.0.3/src/
-drwxr-xr-x   0 akib_shaikh  (1000) akib_shaikh  (1000)        0 2023-05-05 10:13:57.326301 aib_logging-1.0.3/src/aib_logging/
--rw-r--r--   0 akib_shaikh  (1000) akib_shaikh  (1000)        0 2023-03-29 01:38:32.000000 aib_logging-1.0.3/src/aib_logging/__init__.py
--rw-r--r--   0 akib_shaikh  (1000) akib_shaikh  (1000)    14858 2023-05-05 10:09:48.000000 aib_logging-1.0.3/src/aib_logging/logger.py
-drwxr-xr-x   0 akib_shaikh  (1000) akib_shaikh  (1000)        0 2023-05-05 10:13:57.328302 aib_logging-1.0.3/src/aib_logging.egg-info/
--rw-r--r--   0 akib_shaikh  (1000) akib_shaikh  (1000)      528 2023-05-05 10:13:57.000000 aib_logging-1.0.3/src/aib_logging.egg-info/PKG-INFO
--rw-r--r--   0 akib_shaikh  (1000) akib_shaikh  (1000)      284 2023-05-05 10:13:57.000000 aib_logging-1.0.3/src/aib_logging.egg-info/SOURCES.txt
--rw-r--r--   0 akib_shaikh  (1000) akib_shaikh  (1000)        1 2023-05-05 10:13:57.000000 aib_logging-1.0.3/src/aib_logging.egg-info/dependency_links.txt
--rw-r--r--   0 akib_shaikh  (1000) akib_shaikh  (1000)       30 2023-05-05 10:13:57.000000 aib_logging-1.0.3/src/aib_logging.egg-info/requires.txt
--rw-r--r--   0 akib_shaikh  (1000) akib_shaikh  (1000)       12 2023-05-05 10:13:57.000000 aib_logging-1.0.3/src/aib_logging.egg-info/top_level.txt
+drwxr-xr-x   0 akib_shaikh  (1000) akib_shaikh  (1000)        0 2023-05-05 10:57:49.053802 aib_logging-1.0.4/
+-rw-r--r--   0 akib_shaikh  (1000) akib_shaikh  (1000)     1212 2023-03-28 08:02:11.000000 aib_logging-1.0.4/LICENSE.txt
+-rw-r--r--   0 akib_shaikh  (1000) akib_shaikh  (1000)      528 2023-05-05 10:57:49.053802 aib_logging-1.0.4/PKG-INFO
+-rw-r--r--   0 akib_shaikh  (1000) akib_shaikh  (1000)       20 2023-03-28 08:02:11.000000 aib_logging-1.0.4/README.md
+-rw-r--r--   0 akib_shaikh  (1000) akib_shaikh  (1000)      635 2023-05-05 10:53:29.000000 aib_logging-1.0.4/pyproject.toml
+-rw-r--r--   0 akib_shaikh  (1000) akib_shaikh  (1000)       38 2023-05-05 10:57:49.053802 aib_logging-1.0.4/setup.cfg
+drwxr-xr-x   0 akib_shaikh  (1000) akib_shaikh  (1000)        0 2023-05-05 10:57:49.050802 aib_logging-1.0.4/src/
+drwxr-xr-x   0 akib_shaikh  (1000) akib_shaikh  (1000)        0 2023-05-05 10:57:49.051802 aib_logging-1.0.4/src/aib_logging/
+-rw-r--r--   0 akib_shaikh  (1000) akib_shaikh  (1000)        0 2023-03-29 01:38:32.000000 aib_logging-1.0.4/src/aib_logging/__init__.py
+-rw-r--r--   0 akib_shaikh  (1000) akib_shaikh  (1000)    14616 2023-05-05 10:57:19.000000 aib_logging-1.0.4/src/aib_logging/logger.py
+drwxr-xr-x   0 akib_shaikh  (1000) akib_shaikh  (1000)        0 2023-05-05 10:57:49.053802 aib_logging-1.0.4/src/aib_logging.egg-info/
+-rw-r--r--   0 akib_shaikh  (1000) akib_shaikh  (1000)      528 2023-05-05 10:57:49.000000 aib_logging-1.0.4/src/aib_logging.egg-info/PKG-INFO
+-rw-r--r--   0 akib_shaikh  (1000) akib_shaikh  (1000)      284 2023-05-05 10:57:49.000000 aib_logging-1.0.4/src/aib_logging.egg-info/SOURCES.txt
+-rw-r--r--   0 akib_shaikh  (1000) akib_shaikh  (1000)        1 2023-05-05 10:57:49.000000 aib_logging-1.0.4/src/aib_logging.egg-info/dependency_links.txt
+-rw-r--r--   0 akib_shaikh  (1000) akib_shaikh  (1000)       26 2023-05-05 10:57:49.000000 aib_logging-1.0.4/src/aib_logging.egg-info/requires.txt
+-rw-r--r--   0 akib_shaikh  (1000) akib_shaikh  (1000)       12 2023-05-05 10:57:49.000000 aib_logging-1.0.4/src/aib_logging.egg-info/top_level.txt
```

### Comparing `aib_logging-1.0.3/LICENSE.txt` & `aib_logging-1.0.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `aib_logging-1.0.3/PKG-INFO` & `aib_logging-1.0.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aib_logging
-Version: 1.0.3
+Version: 1.0.4
 Summary: A small example package
 Author-email: akib Shaikh <shaikhakib.k@gmail.com>
 Project-URL: Homepage, https://github.com/pypa/sampleproject
 Project-URL: Bug Tracker, https://github.com/pypa/sampleproject/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `aib_logging-1.0.3/pyproject.toml` & `aib_logging-1.0.4/pyproject.toml`

 * *Files 20% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "aib_logging"
-version = "1.0.3"
+version = "1.0.4"
 authors = [
   { name="akib Shaikh", email="shaikhakib.k@gmail.com" },
 ]
 description = "A small example package"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 dependencies = [
     "google-cloud-logging",
-    "datetime",
+    "time",
 ]
 
 [project.urls]
 "Homepage" = "https://github.com/pypa/sampleproject"
 "Bug Tracker" = "https://github.com/pypa/sampleproject/issues"
```

### Comparing `aib_logging-1.0.3/src/aib_logging/logger.py` & `aib_logging-1.0.4/src/aib_logging/logger.py`

 * *Files 2% similar despite different names*

```diff
@@ -76,32 +76,24 @@
             process_time(float): add CPU time taken by function/component
                 default is 0.0
             severity(str): default is INFO
         Returns:
             None
         """
         import inspect
-        import datetime 
+        import time
     
-        start_time = 0.0 
-        end_time = 0.0
-        
-        if status == 'start':
-            start_time = datetime.datetime.now()
-        elif status == 'end':
-            end_time = datetime.datetime.now()
-        
+        t_time = time.time()
         payload={
             "pipeline_run_name":self.pipeline_name,
             "region":self.region,
             "project":self.project,
             "component_name": inspect.stack()[1].function,
             "status":status,
-            "start_time":start_time,
-            "end_time":end_time,
+            "time":t_time,
             "clock_time":clock_time,
             "process_time":process_time,
             "message":msg,
         }
         self.logger.log_struct(payload, severity=severity.value)
```

### Comparing `aib_logging-1.0.3/src/aib_logging.egg-info/PKG-INFO` & `aib_logging-1.0.4/src/aib_logging.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aib-logging
-Version: 1.0.3
+Version: 1.0.4
 Summary: A small example package
 Author-email: akib Shaikh <shaikhakib.k@gmail.com>
 Project-URL: Homepage, https://github.com/pypa/sampleproject
 Project-URL: Bug Tracker, https://github.com/pypa/sampleproject/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

