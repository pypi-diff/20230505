# Comparing `tmp/LogAssist-1.0.2.tar.gz` & `tmp/LogAssist-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "LogAssist-1.0.2.tar", last modified: Thu May  4 07:43:17 2023, max compression
+gzip compressed data, was "LogAssist-1.0.3.tar", last modified: Fri May  5 01:16:55 2023, max compression
```

## Comparing `LogAssist-1.0.2.tar` & `LogAssist-1.0.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-05-04 07:43:17.338762 LogAssist-1.0.2/
--rw-rw-rw-   0        0        0     1087 2023-05-04 01:09:05.000000 LogAssist-1.0.2/LICENSE
-drwxrwxrwx   0        0        0        0 2023-05-04 07:43:17.328730 LogAssist-1.0.2/LogAssist/
--rw-rw-rw-   0        0        0        2 2023-05-04 07:39:48.000000 LogAssist-1.0.2/LogAssist/__init__.py
--rw-rw-rw-   0        0        0     6519 2023-05-04 07:39:17.000000 LogAssist-1.0.2/LogAssist/log.py
-drwxrwxrwx   0        0        0        0 2023-05-04 07:43:17.336236 LogAssist-1.0.2/LogAssist.egg-info/
--rw-rw-rw-   0        0        0     2353 2023-05-04 07:43:16.000000 LogAssist-1.0.2/LogAssist.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      212 2023-05-04 07:43:17.000000 LogAssist-1.0.2/LogAssist.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-04 07:43:16.000000 LogAssist-1.0.2/LogAssist.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       10 2023-05-04 07:43:16.000000 LogAssist-1.0.2/LogAssist.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     2353 2023-05-04 07:43:17.337742 LogAssist-1.0.2/PKG-INFO
--rw-rw-rw-   0        0        0     1668 2023-05-04 02:43:50.000000 LogAssist-1.0.2/README.md
--rw-rw-rw-   0        0        0      709 2023-05-04 07:39:38.000000 LogAssist-1.0.2/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-04 07:43:17.338762 LogAssist-1.0.2/setup.cfg
--rw-rw-rw-   0        0        0      874 2023-05-04 07:39:42.000000 LogAssist-1.0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-05 01:16:55.683478 LogAssist-1.0.3/
+-rw-rw-rw-   0        0        0     1087 2023-05-04 01:09:05.000000 LogAssist-1.0.3/LICENSE
+drwxrwxrwx   0        0        0        0 2023-05-05 01:16:55.672696 LogAssist-1.0.3/LogAssist/
+-rw-rw-rw-   0        0        0        2 2023-05-04 07:39:48.000000 LogAssist-1.0.3/LogAssist/__init__.py
+-rw-rw-rw-   0        0        0     7213 2023-05-05 01:15:39.000000 LogAssist-1.0.3/LogAssist/log.py
+drwxrwxrwx   0        0        0        0 2023-05-05 01:16:55.679991 LogAssist-1.0.3/LogAssist.egg-info/
+-rw-rw-rw-   0        0        0     2420 2023-05-05 01:16:55.000000 LogAssist-1.0.3/LogAssist.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      212 2023-05-05 01:16:55.000000 LogAssist-1.0.3/LogAssist.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-05 01:16:55.000000 LogAssist-1.0.3/LogAssist.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       10 2023-05-05 01:16:55.000000 LogAssist-1.0.3/LogAssist.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     2420 2023-05-05 01:16:55.682460 LogAssist-1.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0     1735 2023-05-05 01:15:35.000000 LogAssist-1.0.3/README.md
+-rw-rw-rw-   0        0        0      709 2023-05-05 01:15:55.000000 LogAssist-1.0.3/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-05 01:16:55.683478 LogAssist-1.0.3/setup.cfg
+-rw-rw-rw-   0        0        0      874 2023-05-05 01:16:02.000000 LogAssist-1.0.3/setup.py
```

### Comparing `LogAssist-1.0.2/LICENSE` & `LogAssist-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `LogAssist-1.0.2/LogAssist/log.py` & `LogAssist-1.0.3/LogAssist/log.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,27 +6,30 @@
 # A class that provides logging functionality
 
 
 class Logger:
 
     # A dictionary to map logging levels to integers
     level_list = {
-        'error': 4,
-        'warning': 3,
-        'warn': 3,
-        'info': 2,
-        'debug': 1,
+        'error': 40,
+        'warning': 30,
+        'warn': 30,
+        'info': 20,
+        'debug': 10,
+        'verbose': 5,
+        'verb': 5,
     }
 
     # A dictionary to map integers to logging level strings
     level_str_list = {
-        1: 'DEBUG',
-        2: 'INFO',
-        3: 'WARN',
-        4: 'ERROR'
+        5: 'VERB',
+        10: 'DEBUG',
+        20: 'INFO',
+        30: 'WARN',
+        40: 'ERROR'
     }
 
     # Default file name for logging
     file_name = 'Logger.log'
 
     # Logger information and configuration
     log_info = {
@@ -37,15 +40,15 @@
         'log_file': 'Logger.log',
         'log_level': 'debug',
     }
 
     log_level = level_list['info']
 
     # Initialize the logger with the specified log level, file name, and log removal option
-    def init(log_level='debug', dir_name='./log', file_name='Logger.log', prev_log_remove=False, out_console=True, out_file=True):
+    def init(log_level='verbose', dir_name='./log', file_name='Logger.log', prev_log_remove=False, out_console=True, out_file=True):
         """
         Initialize the logger with the specified log level, directory name, file name, and log removal option.
 
         :param log_level: The log level to set (debug, info, warning, or error). Default is 'debug'.
         :param dir_name: The directory name to use for log files. Default is './log'.
         :param file_name: The file name to use for logging. Default is None, which will create a file named "Logger.log".
         :param prev_log_remove: Whether to remove the existing log file on initialization. Default is False.
@@ -123,61 +126,83 @@
             new_dir_path = Logger.log_info['dir_name'] + "/"
             if not os.path.exists(new_dir_path):
                 os.makedirs(new_dir_path)
             if Logger.log_info['out_file']:
                 with open(Logger.log_info['dir_name'] + "/" + Logger.log_info['log_file'], mode="a") as file:
                     file.write(log_f)
 
+    # Log a verbose message
+    @staticmethod
+    def verbose(tag: str, message: str = "") -> None:
+        """
+        Logs a debug message.
+
+        :param tag: The tag to use for the log message.
+        :param message: The message to log.
+        """
+        Logger.log_print(tag, message, 5)
+
+    # Log a verbose message
+    @staticmethod
+    def verb(tag: str, message: str = "") -> None:
+        """
+        Logs a debug message.
+
+        :param tag: The tag to use for the log message.
+        :param message: The message to log.
+        """
+        Logger.log_print(tag, message, 5)
+
     # Log a debug message
     @staticmethod
     def debug(tag: str, message: str = "") -> None:
         """
         Logs a debug message.
 
         :param tag: The tag to use for the log message.
         :param message: The message to log.
         """
-        Logger.log_print(tag, message, 1)
+        Logger.log_print(tag, message, 10)
 
     # Log an info message
     @staticmethod
     def info(tag: str, message: str = "") -> None:
         """
         Logs an info message.
 
         :param tag: The tag to use for the log message.
         :param message: The message to log.
         """
-        Logger.log_print(tag, message, 2)
+        Logger.log_print(tag, message, 20)
 
     # Log a warning message
     @staticmethod
     def warning(tag: str, message: str = "") -> None:
         """
         Logs a warning message.
 
         :param tag: The tag to use for the log message.
         :param message: The message to log.
         """
-        Logger.log_print(tag, message, 3)
+        Logger.log_print(tag, message, 30)
 
     # Log a warning message (alias for warning)
     @staticmethod
     def warn(tag: str, message: str = "") -> None:
         """
         Logs a warning message (alias for warning).
 
         :param tag: The tag to use for the log message.
         :param message: The message to log.
         """
-        Logger.log_print(tag, message, 3)
+        Logger.log_print(tag, message, 30)
 
     # Log an error message
     def error(tag: str, message: str = "", exc_info: tuple[None, None, None] = None) -> None:
         """
         Logs an error message.
 
         :param tag: The tag to use for the log message.
         :param message: The message to log.
         :param exc_info: The exception information to log.
         """
-        Logger.log_print(tag, message, 4, exc_info)
+        Logger.log_print(tag, message, 40, exc_info)
```

### Comparing `LogAssist-1.0.2/LogAssist.egg-info/PKG-INFO` & `LogAssist-1.0.3/LogAssist.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: LogAssist
-Version: 1.0.2
+Version: 1.0.3
 Summary: A simple and customizable logging library for Python.
 Home-page: https://github.com/horrible-gh/LogAssist.git
 Author: horrible-gh
 Author-email: horrible <shinjpn1@gmail.com>
 Project-URL: Homepage, https://github.com/horrible-gh/Logger
 Project-URL: Bug Tracker, https://github.com/horrible-gh/Logger/issues
 Keywords: LogAssist,Log Assist,logassist,log assist,Logger,logger
@@ -40,29 +40,30 @@
 ```python
 from LogAssist.log import Logger
 ```
 
 2. Initialize the logger with your desired settings:
 
 ```python
-Logger.init(log_level='debug', dir_name='./log', file_name='my_log.log', prev_log_remove=True, out_console=True, out_file=True)
+Logger.init(log_level='verbose', dir_name='./log', file_name='my_log.log', prev_log_remove=True, out_console=True, out_file=True)
 ```
 
 3. Use the logger in your code:
 
 ```python
+Logger.verbose('MyTag', 'This is a verbose message')
 Logger.debug('MyTag', 'This is a debug message')
 Logger.info('MyTag', 'This is an info message')
 Logger.warning('MyTag', 'This is a warning message')
 Logger.error('MyTag', 'This is an error message', exc_info=sys.exc_info())
 ```
 
 ## Configuration
 
 You can configure the logger using the init method or by passing a dictionary of logger information to the logger_init method. The available options are:
 
-- log_level: The log level to set (debug, info, warning, or error). Default is 'debug'.
+- log_level: The log level to set (verbose, debug, info, warning, or error). Default is 'verbose'.
 - dir_name: The directory name to use for log files. Default is './log'.
 - file_name: The file name to use for logging. Default is None, which will create a file named "Logger.log".
 - prev_log_remove: Whether to remove the existing log file on initialization. Default is False.
 - out_console: Whether to output log messages to the console. Default is True.
 - out_file: Whether to output log messages to a file. Default is True.
```

### Comparing `LogAssist-1.0.2/PKG-INFO` & `LogAssist-1.0.3/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: LogAssist
-Version: 1.0.2
+Version: 1.0.3
 Summary: A simple and customizable logging library for Python.
 Home-page: https://github.com/horrible-gh/LogAssist.git
 Author: horrible-gh
 Author-email: horrible <shinjpn1@gmail.com>
 Project-URL: Homepage, https://github.com/horrible-gh/Logger
 Project-URL: Bug Tracker, https://github.com/horrible-gh/Logger/issues
 Keywords: LogAssist,Log Assist,logassist,log assist,Logger,logger
@@ -40,29 +40,30 @@
 ```python
 from LogAssist.log import Logger
 ```
 
 2. Initialize the logger with your desired settings:
 
 ```python
-Logger.init(log_level='debug', dir_name='./log', file_name='my_log.log', prev_log_remove=True, out_console=True, out_file=True)
+Logger.init(log_level='verbose', dir_name='./log', file_name='my_log.log', prev_log_remove=True, out_console=True, out_file=True)
 ```
 
 3. Use the logger in your code:
 
 ```python
+Logger.verbose('MyTag', 'This is a verbose message')
 Logger.debug('MyTag', 'This is a debug message')
 Logger.info('MyTag', 'This is an info message')
 Logger.warning('MyTag', 'This is a warning message')
 Logger.error('MyTag', 'This is an error message', exc_info=sys.exc_info())
 ```
 
 ## Configuration
 
 You can configure the logger using the init method or by passing a dictionary of logger information to the logger_init method. The available options are:
 
-- log_level: The log level to set (debug, info, warning, or error). Default is 'debug'.
+- log_level: The log level to set (verbose, debug, info, warning, or error). Default is 'verbose'.
 - dir_name: The directory name to use for log files. Default is './log'.
 - file_name: The file name to use for logging. Default is None, which will create a file named "Logger.log".
 - prev_log_remove: Whether to remove the existing log file on initialization. Default is False.
 - out_console: Whether to output log messages to the console. Default is True.
 - out_file: Whether to output log messages to a file. Default is True.
```

### Comparing `LogAssist-1.0.2/README.md` & `LogAssist-1.0.3/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -23,29 +23,30 @@
 ```python
 from LogAssist.log import Logger
 ```
 
 2. Initialize the logger with your desired settings:
 
 ```python
-Logger.init(log_level='debug', dir_name='./log', file_name='my_log.log', prev_log_remove=True, out_console=True, out_file=True)
+Logger.init(log_level='verbose', dir_name='./log', file_name='my_log.log', prev_log_remove=True, out_console=True, out_file=True)
 ```
 
 3. Use the logger in your code:
 
 ```python
+Logger.verbose('MyTag', 'This is a verbose message')
 Logger.debug('MyTag', 'This is a debug message')
 Logger.info('MyTag', 'This is an info message')
 Logger.warning('MyTag', 'This is a warning message')
 Logger.error('MyTag', 'This is an error message', exc_info=sys.exc_info())
 ```
 
 ## Configuration
 
 You can configure the logger using the init method or by passing a dictionary of logger information to the logger_init method. The available options are:
 
-- log_level: The log level to set (debug, info, warning, or error). Default is 'debug'.
+- log_level: The log level to set (verbose, debug, info, warning, or error). Default is 'verbose'.
 - dir_name: The directory name to use for log files. Default is './log'.
 - file_name: The file name to use for logging. Default is None, which will create a file named "Logger.log".
 - prev_log_remove: Whether to remove the existing log file on initialization. Default is False.
 - out_console: Whether to output log messages to the console. Default is True.
 - out_file: Whether to output log messages to a file. Default is True.
```

### Comparing `LogAssist-1.0.2/pyproject.toml` & `LogAssist-1.0.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "LogAssist"
-version = "1.0.2"
+version = "1.0.3"
 authors = [
   { name="horrible", email="shinjpn1@gmail.com" },
 ]
 description = "A simple and customizable logging library for Python."
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `LogAssist-1.0.2/setup.py` & `LogAssist-1.0.3/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='LogAssist',
-    version='1.0.2',
+    version='1.0.3',
     description='LogAssist package',
     author='horrible-gh',
     author_email='shinjpn1@gmail.com',
     url='https://github.com/horrible-gh/LogAssist.git',
     packages=find_packages(),
     classifiers=[
         'Development Status :: 3 - Alpha',
```

