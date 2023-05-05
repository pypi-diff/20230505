# Comparing `tmp/paddypy-0.1.7.tar.gz` & `tmp/paddypy-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "paddypy-0.1.7.tar", last modified: Fri May  5 08:40:19 2023, max compression
+gzip compressed data, was "paddypy-0.1.8.tar", last modified: Fri May  5 08:43:51 2023, max compression
```

## Comparing `paddypy-0.1.7.tar` & `paddypy-0.1.8.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-05-05 08:40:19.111245 paddypy-0.1.7/
--rw-rw-rw-   0        0        0     1150 2022-05-16 06:26:09.000000 paddypy-0.1.7/LICENSE
--rw-rw-rw-   0        0        0     1795 2023-05-05 08:40:19.110746 paddypy-0.1.7/PKG-INFO
--rw-rw-rw-   0        0        0      918 2023-04-17 10:33:45.000000 paddypy-0.1.7/README.md
-drwxrwxrwx   0        0        0        0 2023-05-05 08:40:19.097246 paddypy-0.1.7/paddypy/
--rw-rw-rw-   0        0        0      102 2023-04-17 12:26:22.000000 paddypy-0.1.7/paddypy/__init__.py
--rw-rw-rw-   0        0        0     5772 2023-04-17 12:26:22.000000 paddypy-0.1.7/paddypy/access.py
--rw-rw-rw-   0        0        0     3849 2023-05-05 08:39:53.000000 paddypy-0.1.7/paddypy/log.py
-drwxrwxrwx   0        0        0        0 2023-05-05 08:40:19.109746 paddypy-0.1.7/paddypy.egg-info/
--rw-rw-rw-   0        0        0     1795 2023-05-05 08:40:18.000000 paddypy-0.1.7/paddypy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      233 2023-05-05 08:40:19.000000 paddypy-0.1.7/paddypy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-05 08:40:18.000000 paddypy-0.1.7/paddypy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      127 2023-05-05 08:40:18.000000 paddypy-0.1.7/paddypy.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-05-05 08:40:18.000000 paddypy-0.1.7/paddypy.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-05 08:40:19.111245 paddypy-0.1.7/setup.cfg
--rw-rw-rw-   0        0        0     1480 2023-05-05 08:40:08.000000 paddypy-0.1.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-05 08:43:51.873527 paddypy-0.1.8/
+-rw-rw-rw-   0        0        0     1150 2022-05-16 06:26:09.000000 paddypy-0.1.8/LICENSE
+-rw-rw-rw-   0        0        0     1795 2023-05-05 08:43:51.873027 paddypy-0.1.8/PKG-INFO
+-rw-rw-rw-   0        0        0      918 2023-04-17 10:33:45.000000 paddypy-0.1.8/README.md
+drwxrwxrwx   0        0        0        0 2023-05-05 08:43:51.862525 paddypy-0.1.8/paddypy/
+-rw-rw-rw-   0        0        0      102 2023-04-17 12:26:22.000000 paddypy-0.1.8/paddypy/__init__.py
+-rw-rw-rw-   0        0        0     5772 2023-04-17 12:26:22.000000 paddypy-0.1.8/paddypy/access.py
+-rw-rw-rw-   0        0        0     3883 2023-05-05 08:43:21.000000 paddypy-0.1.8/paddypy/log.py
+drwxrwxrwx   0        0        0        0 2023-05-05 08:43:51.872026 paddypy-0.1.8/paddypy.egg-info/
+-rw-rw-rw-   0        0        0     1795 2023-05-05 08:43:51.000000 paddypy-0.1.8/paddypy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      233 2023-05-05 08:43:51.000000 paddypy-0.1.8/paddypy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-05 08:43:51.000000 paddypy-0.1.8/paddypy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      127 2023-05-05 08:43:51.000000 paddypy-0.1.8/paddypy.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-05-05 08:43:51.000000 paddypy-0.1.8/paddypy.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-05 08:43:51.874026 paddypy-0.1.8/setup.cfg
+-rw-rw-rw-   0        0        0     1480 2023-05-05 08:42:27.000000 paddypy-0.1.8/setup.py
```

### Comparing `paddypy-0.1.7/LICENSE` & `paddypy-0.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `paddypy-0.1.7/PKG-INFO` & `paddypy-0.1.8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: paddypy
-Version: 0.1.7
+Version: 0.1.8
 Summary: Collection of helpfull extensions
 Author: Patrik
 Author-email: <patrikhartl@gmail.com>
 Keywords: python,appconfiguration,azure
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `paddypy-0.1.7/README.md` & `paddypy-0.1.8/README.md`

 * *Files identical despite different names*

### Comparing `paddypy-0.1.7/paddypy/access.py` & `paddypy-0.1.8/paddypy/access.py`

 * *Files identical despite different names*

### Comparing `paddypy-0.1.7/paddypy/log.py` & `paddypy-0.1.8/paddypy/log.py`

 * *Files 11% similar despite different names*

```diff
@@ -46,41 +46,46 @@
             azure_handler = AzureLogHandler(connection_string=str(applicationinsights_key))
             azure_handler.setLevel(logger_level)
             logger.addHandler(azure_handler)
         return logger
 
     
     def timeit(self, silence_args=False):
-        def actual_decorator(func):
-            @wraps(func)
-            def timeit_wrapper(*args, **kwargs):
-                start_time = time.perf_counter()
-                result = func(*args, **kwargs)
-                end_time = time.perf_counter()
-                total_time = end_time - start_time
-                if silence_args:
-                    arg_types = tuple(type(arg).__name__ for arg in args)
-                    kwarg_types = {key: type(val).__name__ for key, val in kwargs.items()}
-                    log_msg = f'Function {func.__name__}{arg_types} {kwarg_types} Took {total_time:.4f} seconds'
-                else:
-                    log_msg = f'Function {func.__name__}{args} {kwargs} Took {total_time:.4f} seconds'
-
-                self.logger.log(msg=log_msg, level=logging.INFO)
-                return result
-
-            return wraps(func)(timeit_wrapper)  # Use wraps here to preserve the original function's metadata
-
-        return actual_decorator
+        return TimeitDecorator(self.logger, silence_args)
 
 
     def except_block(self, inst, exceptionMessage="No message"):
         exceptionMessage = exceptionMessage
         exceptionTimne = str(datetime.datetime.now())
         exceptionType = str(type(inst))
         exceptionArgument = str(inst.args)
         exceptionInstance = str(inst)
         self.logger.log(msg="Exception message: {message}".format(message=exceptionMessage), level=logging.ERROR)
         self.logger.log(msg="Exception occured at: {message}".format(message=exceptionTimne), level=logging.ERROR)
         self.logger.log(msg="Exception instance type: {message}".format(message=exceptionType), level=logging.ERROR)
         self.logger.log(msg="Exception argument: {message}".format(message=exceptionArgument), level=logging.ERROR)
         self.logger.log(msg="Exception instance: {message}".format(message=exceptionInstance), level=logging.ERROR)
 
+
+class TimeitDecorator:
+    def __init__(self, logger, silence_args):
+        self.logger = logger
+        self.silence_args = silence_args
+
+    def __call__(self, func):
+        @wraps(func)
+        def timeit_wrapper(*args, **kwargs):
+            start_time = time.perf_counter()
+            result = func(*args, **kwargs)
+            end_time = time.perf_counter()
+            total_time = end_time - start_time
+            if self.silence_args:
+                arg_types = tuple(type(arg).__name__ for arg in args)
+                kwarg_types = {key: type(val).__name__ for key, val in kwargs.items()}
+                log_msg = f'Function {func.__name__}{arg_types} {kwarg_types} Took {total_time:.4f} seconds'
+            else:
+                log_msg = f'Function {func.__name__}{args} {kwargs} Took {total_time:.4f} seconds'
+
+            self.logger.log(msg=log_msg, level=logging.INFO)
+            return result
+        return timeit_wrapper
+
```

### Comparing `paddypy-0.1.7/paddypy.egg-info/PKG-INFO` & `paddypy-0.1.8/paddypy.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: paddypy
-Version: 0.1.7
+Version: 0.1.8
 Summary: Collection of helpfull extensions
 Author: Patrik
 Author-email: <patrikhartl@gmail.com>
 Keywords: python,appconfiguration,azure
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `paddypy-0.1.7/setup.py` & `paddypy-0.1.8/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import os
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
-VERSION = '0.1.7'
+VERSION = '0.1.8'
 DESCRIPTION = 'Collection of helpfull extensions'
 LONG_DESCRIPTION = 'Collection of helpfull extensions'
 
 # Setting up
 setup(
     name="paddypy",
     version=VERSION,
```

