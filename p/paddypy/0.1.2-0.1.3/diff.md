# Comparing `tmp/paddypy-0.1.2.tar.gz` & `tmp/paddypy-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "paddypy-0.1.2.tar", last modified: Sat Apr 29 10:31:57 2023, max compression
+gzip compressed data, was "paddypy-0.1.3.tar", last modified: Fri May  5 07:54:12 2023, max compression
```

## Comparing `paddypy-0.1.2.tar` & `paddypy-0.1.3.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-04-29 10:31:57.934106 paddypy-0.1.2/
--rw-rw-rw-   0        0        0     1150 2022-05-16 06:26:09.000000 paddypy-0.1.2/LICENSE
--rw-rw-rw-   0        0        0     1795 2023-04-29 10:31:57.933606 paddypy-0.1.2/PKG-INFO
--rw-rw-rw-   0        0        0      918 2023-04-17 10:33:45.000000 paddypy-0.1.2/README.md
-drwxrwxrwx   0        0        0        0 2023-04-29 10:31:57.922105 paddypy-0.1.2/paddypy/
--rw-rw-rw-   0        0        0      102 2023-04-17 12:26:22.000000 paddypy-0.1.2/paddypy/__init__.py
--rw-rw-rw-   0        0        0     5772 2023-04-17 12:26:22.000000 paddypy-0.1.2/paddypy/access.py
--rw-rw-rw-   0        0        0     3391 2023-04-29 10:30:54.000000 paddypy-0.1.2/paddypy/log.py
-drwxrwxrwx   0        0        0        0 2023-04-29 10:31:57.932605 paddypy-0.1.2/paddypy.egg-info/
--rw-rw-rw-   0        0        0     1795 2023-04-29 10:31:57.000000 paddypy-0.1.2/paddypy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      233 2023-04-29 10:31:57.000000 paddypy-0.1.2/paddypy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-29 10:31:57.000000 paddypy-0.1.2/paddypy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      127 2023-04-29 10:31:57.000000 paddypy-0.1.2/paddypy.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-04-29 10:31:57.000000 paddypy-0.1.2/paddypy.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-29 10:31:57.934606 paddypy-0.1.2/setup.cfg
--rw-rw-rw-   0        0        0     1480 2023-04-29 10:30:34.000000 paddypy-0.1.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-05 07:54:12.400308 paddypy-0.1.3/
+-rw-rw-rw-   0        0        0     1150 2022-05-16 06:26:09.000000 paddypy-0.1.3/LICENSE
+-rw-rw-rw-   0        0        0     1795 2023-05-05 07:54:12.399810 paddypy-0.1.3/PKG-INFO
+-rw-rw-rw-   0        0        0      918 2023-04-17 10:33:45.000000 paddypy-0.1.3/README.md
+drwxrwxrwx   0        0        0        0 2023-05-05 07:54:12.381808 paddypy-0.1.3/paddypy/
+-rw-rw-rw-   0        0        0      102 2023-04-17 12:26:22.000000 paddypy-0.1.3/paddypy/__init__.py
+-rw-rw-rw-   0        0        0     5772 2023-04-17 12:26:22.000000 paddypy-0.1.3/paddypy/access.py
+-rw-rw-rw-   0        0        0     4277 2023-05-05 07:50:49.000000 paddypy-0.1.3/paddypy/log.py
+drwxrwxrwx   0        0        0        0 2023-05-05 07:54:12.398808 paddypy-0.1.3/paddypy.egg-info/
+-rw-rw-rw-   0        0        0     1795 2023-05-05 07:54:12.000000 paddypy-0.1.3/paddypy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      233 2023-05-05 07:54:12.000000 paddypy-0.1.3/paddypy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-05 07:54:12.000000 paddypy-0.1.3/paddypy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      127 2023-05-05 07:54:12.000000 paddypy-0.1.3/paddypy.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-05-05 07:54:12.000000 paddypy-0.1.3/paddypy.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-05 07:54:12.400809 paddypy-0.1.3/setup.cfg
+-rw-rw-rw-   0        0        0     1480 2023-05-05 07:49:32.000000 paddypy-0.1.3/setup.py
```

### Comparing `paddypy-0.1.2/LICENSE` & `paddypy-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `paddypy-0.1.2/PKG-INFO` & `paddypy-0.1.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: paddypy
-Version: 0.1.2
+Version: 0.1.3
 Summary: Collection of helpfull extensions
 Author: Patrik
 Author-email: <patrikhartl@gmail.com>
 Keywords: python,appconfiguration,azure
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `paddypy-0.1.2/README.md` & `paddypy-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `paddypy-0.1.2/paddypy/access.py` & `paddypy-0.1.3/paddypy/access.py`

 * *Files identical despite different names*

### Comparing `paddypy-0.1.2/paddypy/log.py` & `paddypy-0.1.3/paddypy/log.py`

 * *Files 17% similar despite different names*

```diff
@@ -58,15 +58,31 @@
             total_time = end_time - start_time
             self.logger.log(msg=f'Function {func.__name__}{args} {kwargs} Took {total_time:.4f} seconds', level=logging.INFO)
             #logging.log(f'Function {func.__name__}{args} {kwargs} Took {total_time:.4f} seconds', level=logging.DEBUG)
             return result
         return timeit_wrapper
 
 
+    def timeit(self, silence_args=False):
+        def decorator(func):
+            @wraps(func)
+            def timeit_wrapper(*args, **kwargs):
+                start_time = time.perf_counter()
+                result = func(*args, **kwargs)
+                end_time = time.perf_counter()
+                total_time = end_time - start_time
+                if silence_args:
+                    arg_types = tuple(type(arg).__name__ for arg in args)
+                    kwarg_types = {key: type(val).__name__ for key, val in kwargs.items()}
+                    log_msg = f'Function {func.__name__}{arg_types} {kwarg_types} Took {total_time:.4f} seconds'
+                else:
+                    log_msg = f'Function {func.__name__}{args} {kwargs} Took {total_time:.4f} seconds'
 
+                self.logger.log(msg=log_msg, level=logging.INFO)
+                return result
 
     def except_block(self, inst, exceptionMessage="No message"):
         exceptionMessage = exceptionMessage
         exceptionTimne = str(datetime.datetime.now())
         exceptionType = str(type(inst))
         exceptionArgument = str(inst.args)
         exceptionInstance = str(inst)
```

### Comparing `paddypy-0.1.2/paddypy.egg-info/PKG-INFO` & `paddypy-0.1.3/paddypy.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: paddypy
-Version: 0.1.2
+Version: 0.1.3
 Summary: Collection of helpfull extensions
 Author: Patrik
 Author-email: <patrikhartl@gmail.com>
 Keywords: python,appconfiguration,azure
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `paddypy-0.1.2/setup.py` & `paddypy-0.1.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import os
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
-VERSION = '0.1.2'
+VERSION = '0.1.3'
 DESCRIPTION = 'Collection of helpfull extensions'
 LONG_DESCRIPTION = 'Collection of helpfull extensions'
 
 # Setting up
 setup(
     name="paddypy",
     version=VERSION,
```

