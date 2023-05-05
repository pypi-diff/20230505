# Comparing `tmp/axiom_logger-1.0.2.tar.gz` & `tmp/axiom_logger-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "axiom_logger-1.0.2.tar", last modified: Thu May  4 10:46:15 2023, max compression
+gzip compressed data, was "axiom_logger-1.0.3.tar", last modified: Fri May  5 07:59:01 2023, max compression
```

## Comparing `axiom_logger-1.0.2.tar` & `axiom_logger-1.0.3.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 10:46:15.913614 axiom_logger-1.0.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-05-04 10:45:58.000000 axiom_logger-1.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3783 2023-05-04 10:46:15.913614 axiom_logger-1.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3253 2023-05-04 10:45:58.000000 axiom_logger-1.0.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      615 2023-05-04 10:45:58.000000 axiom_logger-1.0.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-04 10:46:15.913614 axiom_logger-1.0.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 10:46:15.913614 axiom_logger-1.0.2/src/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 10:45:58.000000 axiom_logger-1.0.2/src/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 10:46:15.913614 axiom_logger-1.0.2/src/axiom_logger.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3783 2023-05-04 10:46:15.000000 axiom_logger-1.0.2/src/axiom_logger.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      228 2023-05-04 10:46:15.000000 axiom_logger-1.0.2/src/axiom_logger.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-04 10:46:15.000000 axiom_logger-1.0.2/src/axiom_logger.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-04 10:46:15.000000 axiom_logger-1.0.2/src/axiom_logger.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     4252 2023-05-04 10:45:58.000000 axiom_logger-1.0.2/src/axiom_logger.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 07:59:01.100186 axiom_logger-1.0.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-05-05 07:58:40.000000 axiom_logger-1.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3783 2023-05-05 07:59:01.100186 axiom_logger-1.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3253 2023-05-05 07:58:40.000000 axiom_logger-1.0.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      615 2023-05-05 07:58:40.000000 axiom_logger-1.0.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-05 07:59:01.100186 axiom_logger-1.0.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 07:59:01.096186 axiom_logger-1.0.3/src/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 07:58:40.000000 axiom_logger-1.0.3/src/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 07:59:01.096186 axiom_logger-1.0.3/src/axiom_logger.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3783 2023-05-05 07:59:01.000000 axiom_logger-1.0.3/src/axiom_logger.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      228 2023-05-05 07:59:01.000000 axiom_logger-1.0.3/src/axiom_logger.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 07:59:01.000000 axiom_logger-1.0.3/src/axiom_logger.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-05 07:59:01.000000 axiom_logger-1.0.3/src/axiom_logger.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     4325 2023-05-05 07:58:40.000000 axiom_logger-1.0.3/src/axiom_logger.py
```

### Comparing `axiom_logger-1.0.2/LICENSE` & `axiom_logger-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `axiom_logger-1.0.2/PKG-INFO` & `axiom_logger-1.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: axiom_logger
-Version: 1.0.2
+Version: 1.0.3
 Summary: Python logging handler for the Axiom service
 Author-email: Stefano Maddè <sm@spforniture.it>
 Project-URL: Homepage, https://github.com/stemadde/axiom_logger
 Project-URL: Bug Tracker, https://github.com/stemadde/axiom_logger/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `axiom_logger-1.0.2/README.md` & `axiom_logger-1.0.3/README.md`

 * *Files identical despite different names*

### Comparing `axiom_logger-1.0.2/pyproject.toml` & `axiom_logger-1.0.3/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0", "requests"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "axiom_logger"
-version = "1.0.2"
+version = "1.0.3"
 authors = [
   { name="Stefano Maddè", email="sm@spforniture.it" },
 ]
 description = "Python logging handler for the Axiom service"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `axiom_logger-1.0.2/src/axiom_logger.egg-info/PKG-INFO` & `axiom_logger-1.0.3/src/axiom_logger.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: axiom-logger
-Version: 1.0.2
+Version: 1.0.3
 Summary: Python logging handler for the Axiom service
 Author-email: Stefano Maddè <sm@spforniture.it>
 Project-URL: Homepage, https://github.com/stemadde/axiom_logger
 Project-URL: Bug Tracker, https://github.com/stemadde/axiom_logger/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `axiom_logger-1.0.2/src/axiom_logger.py` & `axiom_logger-1.0.3/src/axiom_logger.py`

 * *Files 3% similar despite different names*

```diff
@@ -86,18 +86,20 @@
                 self.send()
         else:
             if not self.timer or not self.timer.is_alive():
                 self.timer = threading.Timer(self.elapsed_time, self.send)
                 self.timer.start()
 
     def axiom_format(self, record: LogRecord) -> dict:
-        return {
+        dict_ = {
             "_time": record.created,
-            "data": record.getMessage(),
+            "formatted_message": self.format(record),
         }
+        dict_.update(record.__dict__)
+        return dict_
 
     def send(self) -> None:
         if not self.record_pool:
             return
         self.is_sending = True
         res = self.session.post(self.endpoint, json=self.record_pool)
         if not res.status_code == 200:
```

