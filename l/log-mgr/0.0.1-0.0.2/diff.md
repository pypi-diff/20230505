# Comparing `tmp/log_mgr-0.0.1.tar.gz` & `tmp/log_mgr-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "log_mgr-0.0.1.tar", last modified: Wed Apr 19 18:39:49 2023, max compression
+gzip compressed data, was "log_mgr-0.0.2.tar", last modified: Fri May  5 18:56:27 2023, max compression
```

## Comparing `log_mgr-0.0.1.tar` & `log_mgr-0.0.2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 18:39:49.632317 log_mgr-0.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)      654 2023-04-19 18:39:49.632317 log_mgr-0.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      200 2023-04-19 18:39:39.000000 log_mgr-0.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 18:39:49.632317 log_mgr-0.0.1/log_mgr/
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-04-19 18:39:39.000000 log_mgr-0.0.1/log_mgr/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3331 2023-04-19 18:39:39.000000 log_mgr-0.0.1/log_mgr/logger.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 18:39:49.632317 log_mgr-0.0.1/log_mgr.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      654 2023-04-19 18:39:49.000000 log_mgr-0.0.1/log_mgr.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      219 2023-04-19 18:39:49.000000 log_mgr-0.0.1/log_mgr.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-19 18:39:49.000000 log_mgr-0.0.1/log_mgr.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-04-19 18:39:49.000000 log_mgr-0.0.1/log_mgr.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-19 18:39:49.632317 log_mgr-0.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      742 2023-04-19 18:39:39.000000 log_mgr-0.0.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 18:39:49.632317 log_mgr-0.0.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 18:39:39.000000 log_mgr-0.0.1/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      890 2023-04-19 18:39:39.000000 log_mgr-0.0.1/tests/test_config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 18:56:27.872301 log_mgr-0.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)      654 2023-05-05 18:56:27.872301 log_mgr-0.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      200 2023-05-05 18:56:17.000000 log_mgr-0.0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 18:56:27.872301 log_mgr-0.0.2/log_mgr/
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-05-05 18:56:17.000000 log_mgr-0.0.2/log_mgr/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4383 2023-05-05 18:56:17.000000 log_mgr-0.0.2/log_mgr/logger.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 18:56:27.872301 log_mgr-0.0.2/log_mgr.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      654 2023-05-05 18:56:27.000000 log_mgr-0.0.2/log_mgr.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      219 2023-05-05 18:56:27.000000 log_mgr-0.0.2/log_mgr.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 18:56:27.000000 log_mgr-0.0.2/log_mgr.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-05 18:56:27.000000 log_mgr-0.0.2/log_mgr.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-05 18:56:27.872301 log_mgr-0.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      742 2023-05-05 18:56:17.000000 log_mgr-0.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 18:56:27.872301 log_mgr-0.0.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 18:56:17.000000 log_mgr-0.0.2/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      918 2023-05-05 18:56:17.000000 log_mgr-0.0.2/tests/test_config.py
```

### Comparing `log_mgr-0.0.1/PKG-INFO` & `log_mgr-0.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: log_mgr
-Version: 0.0.1
+Version: 0.0.2
 Summary: Utility class for logging with handlers included
 Home-page: https://github.com/Phornee/log_mgr
 Author: Ismael Raya
 Author-email: phornee@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `log_mgr-0.0.1/log_mgr.egg-info/PKG-INFO` & `log_mgr-0.0.2/log_mgr.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: log-mgr
-Version: 0.0.1
+Version: 0.0.2
 Summary: Utility class for logging with handlers included
 Home-page: https://github.com/Phornee/log_mgr
 Author: Ismael Raya
 Author-email: phornee@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### Comparing `log_mgr-0.0.1/setup.py` & `log_mgr-0.0.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="log_mgr",
-    version="0.0.1",
+    version="0.0.2",
     author="Ismael Raya",
     author_email="phornee@gmail.com",
     description="Utility class for logging with handlers included",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/Phornee/log_mgr",
     packages=setuptools.find_packages(),
```

### Comparing `log_mgr-0.0.1/tests/test_config.py` & `log_mgr-0.0.2/tests/test_config.py`

 * *Files 13% similar despite different names*

```diff
@@ -9,19 +9,19 @@
 
 class Testing(unittest.TestCase):
     """Unittesting class"""
 
     def test_000_log_file(self):
         """Test for logging to file
         """
-        log_path = os.path.join(str(Path.home()), 'var', 'log', 'log_helper', 'logtest.log')
+        log_path = os.path.join(str(Path.home()), 'var', 'log', 'log_helper', 'dryrun_log', 'logtest.log')
         if os.path.exists(log_path):
             os.remove(log_path)
 
-        logger = Logger('log_helper', 'logtest', mode=LoggerMode.FILE, level=logging.INFO)
+        logger = Logger('log_helper', 'logtest', mode=LoggerMode.FILE, level=logging.INFO, dry_run=True)
 
         self.assertEqual(log_path, logger.get_log_path())
 
         logger.debug('debug message')
         logger.info('info message')
 
         content = logger.get_log_lines()
```

