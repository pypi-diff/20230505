# Comparing `tmp/LogAssist-1.0.3.tar.gz` & `tmp/LogAssist-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "LogAssist-1.0.3.tar", last modified: Fri May  5 01:16:55 2023, max compression
+gzip compressed data, was "LogAssist-1.0.4.tar", last modified: Fri May  5 08:57:38 2023, max compression
```

## Comparing `LogAssist-1.0.3.tar` & `LogAssist-1.0.4.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-05-05 01:16:55.683478 LogAssist-1.0.3/
--rw-rw-rw-   0        0        0     1087 2023-05-04 01:09:05.000000 LogAssist-1.0.3/LICENSE
-drwxrwxrwx   0        0        0        0 2023-05-05 01:16:55.672696 LogAssist-1.0.3/LogAssist/
--rw-rw-rw-   0        0        0        2 2023-05-04 07:39:48.000000 LogAssist-1.0.3/LogAssist/__init__.py
--rw-rw-rw-   0        0        0     7213 2023-05-05 01:15:39.000000 LogAssist-1.0.3/LogAssist/log.py
-drwxrwxrwx   0        0        0        0 2023-05-05 01:16:55.679991 LogAssist-1.0.3/LogAssist.egg-info/
--rw-rw-rw-   0        0        0     2420 2023-05-05 01:16:55.000000 LogAssist-1.0.3/LogAssist.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      212 2023-05-05 01:16:55.000000 LogAssist-1.0.3/LogAssist.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-05 01:16:55.000000 LogAssist-1.0.3/LogAssist.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       10 2023-05-05 01:16:55.000000 LogAssist-1.0.3/LogAssist.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     2420 2023-05-05 01:16:55.682460 LogAssist-1.0.3/PKG-INFO
--rw-rw-rw-   0        0        0     1735 2023-05-05 01:15:35.000000 LogAssist-1.0.3/README.md
--rw-rw-rw-   0        0        0      709 2023-05-05 01:15:55.000000 LogAssist-1.0.3/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-05 01:16:55.683478 LogAssist-1.0.3/setup.cfg
--rw-rw-rw-   0        0        0      874 2023-05-05 01:16:02.000000 LogAssist-1.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-05 08:57:38.854025 LogAssist-1.0.4/
+-rw-rw-rw-   0        0        0     1087 2023-05-04 01:09:05.000000 LogAssist-1.0.4/LICENSE
+drwxrwxrwx   0        0        0        0 2023-05-05 08:57:38.841626 LogAssist-1.0.4/LogAssist/
+-rw-rw-rw-   0        0        0        2 2023-05-04 07:39:48.000000 LogAssist-1.0.4/LogAssist/__init__.py
+-rw-rw-rw-   0        0        0     7282 2023-05-05 08:56:34.000000 LogAssist-1.0.4/LogAssist/log.py
+drwxrwxrwx   0        0        0        0 2023-05-05 08:57:38.850485 LogAssist-1.0.4/LogAssist.egg-info/
+-rw-rw-rw-   0        0        0     2420 2023-05-05 08:57:38.000000 LogAssist-1.0.4/LogAssist.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      212 2023-05-05 08:57:38.000000 LogAssist-1.0.4/LogAssist.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-05 08:57:38.000000 LogAssist-1.0.4/LogAssist.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       10 2023-05-05 08:57:38.000000 LogAssist-1.0.4/LogAssist.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     2420 2023-05-05 08:57:38.852967 LogAssist-1.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0     1735 2023-05-05 01:15:35.000000 LogAssist-1.0.4/README.md
+-rw-rw-rw-   0        0        0      709 2023-05-05 08:56:58.000000 LogAssist-1.0.4/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-05 08:57:38.855033 LogAssist-1.0.4/setup.cfg
+-rw-rw-rw-   0        0        0      874 2023-05-05 08:56:52.000000 LogAssist-1.0.4/setup.py
```

### Comparing `LogAssist-1.0.3/LICENSE` & `LogAssist-1.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `LogAssist-1.0.3/LogAssist/log.py` & `LogAssist-1.0.4/LogAssist/log.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 # A class that provides logging functionality
 
 
 class Logger:
 
     # A dictionary to map logging levels to integers
     level_list = {
+        'none': 99,
         'error': 40,
         'warning': 30,
         'warn': 30,
         'info': 20,
         'debug': 10,
         'verbose': 5,
         'verb': 5,
@@ -119,20 +120,21 @@
             log_f = f'{Logger.get_datetime()}[{Logger.level_str_list[level]}][{tag}]{message}\n'
             if exc_info:
                 traceback_str = "".join(traceback.format_exception(*exc_info))
                 log_p += "\n" + traceback_str
                 log_f += traceback_str
             if Logger.log_info['out_console']:
                 print(log_p)
-            new_dir_path = Logger.log_info['dir_name'] + "/"
-            if not os.path.exists(new_dir_path):
-                os.makedirs(new_dir_path)
             if Logger.log_info['out_file']:
-                with open(Logger.log_info['dir_name'] + "/" + Logger.log_info['log_file'], mode="a") as file:
-                    file.write(log_f)
+                new_dir_path = Logger.log_info['dir_name'] + "/"
+                if not os.path.exists(new_dir_path):
+                    os.makedirs(new_dir_path)
+                if Logger.log_info['out_file']:
+                    with open(new_dir_path + Logger.log_info['log_file'], mode="a") as file:
+                        file.write(log_f)
 
     # Log a verbose message
     @staticmethod
     def verbose(tag: str, message: str = "") -> None:
         """
         Logs a debug message.
```

### Comparing `LogAssist-1.0.3/LogAssist.egg-info/PKG-INFO` & `LogAssist-1.0.4/LogAssist.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: LogAssist
-Version: 1.0.3
+Version: 1.0.4
 Summary: A simple and customizable logging library for Python.
 Home-page: https://github.com/horrible-gh/LogAssist.git
 Author: horrible-gh
 Author-email: horrible <shinjpn1@gmail.com>
 Project-URL: Homepage, https://github.com/horrible-gh/Logger
 Project-URL: Bug Tracker, https://github.com/horrible-gh/Logger/issues
 Keywords: LogAssist,Log Assist,logassist,log assist,Logger,logger
```

### Comparing `LogAssist-1.0.3/PKG-INFO` & `LogAssist-1.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: LogAssist
-Version: 1.0.3
+Version: 1.0.4
 Summary: A simple and customizable logging library for Python.
 Home-page: https://github.com/horrible-gh/LogAssist.git
 Author: horrible-gh
 Author-email: horrible <shinjpn1@gmail.com>
 Project-URL: Homepage, https://github.com/horrible-gh/Logger
 Project-URL: Bug Tracker, https://github.com/horrible-gh/Logger/issues
 Keywords: LogAssist,Log Assist,logassist,log assist,Logger,logger
```

### Comparing `LogAssist-1.0.3/README.md` & `LogAssist-1.0.4/README.md`

 * *Files identical despite different names*

### Comparing `LogAssist-1.0.3/pyproject.toml` & `LogAssist-1.0.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "LogAssist"
-version = "1.0.3"
+version = "1.0.4"
 authors = [
   { name="horrible", email="shinjpn1@gmail.com" },
 ]
 description = "A simple and customizable logging library for Python."
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `LogAssist-1.0.3/setup.py` & `LogAssist-1.0.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='LogAssist',
-    version='1.0.3',
+    version='1.0.4',
     description='LogAssist package',
     author='horrible-gh',
     author_email='shinjpn1@gmail.com',
     url='https://github.com/horrible-gh/LogAssist.git',
     packages=find_packages(),
     classifiers=[
         'Development Status :: 3 - Alpha',
```

