# Comparing `tmp/paddypy-0.1.6.tar.gz` & `tmp/paddypy-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "paddypy-0.1.6.tar", last modified: Fri May  5 08:31:08 2023, max compression
+gzip compressed data, was "paddypy-0.1.7.tar", last modified: Fri May  5 08:40:19 2023, max compression
```

## Comparing `paddypy-0.1.6.tar` & `paddypy-0.1.7.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-05-05 08:31:08.765051 paddypy-0.1.6/
--rw-rw-rw-   0        0        0     1150 2022-05-16 06:26:09.000000 paddypy-0.1.6/LICENSE
--rw-rw-rw-   0        0        0     1795 2023-05-05 08:31:08.764552 paddypy-0.1.6/PKG-INFO
--rw-rw-rw-   0        0        0      918 2023-04-17 10:33:45.000000 paddypy-0.1.6/README.md
-drwxrwxrwx   0        0        0        0 2023-05-05 08:31:08.751353 paddypy-0.1.6/paddypy/
--rw-rw-rw-   0        0        0      102 2023-04-17 12:26:22.000000 paddypy-0.1.6/paddypy/__init__.py
--rw-rw-rw-   0        0        0     5772 2023-04-17 12:26:22.000000 paddypy-0.1.6/paddypy/access.py
--rw-rw-rw-   0        0        0     3769 2023-05-05 08:27:07.000000 paddypy-0.1.6/paddypy/log.py
-drwxrwxrwx   0        0        0        0 2023-05-05 08:31:08.763551 paddypy-0.1.6/paddypy.egg-info/
--rw-rw-rw-   0        0        0     1795 2023-05-05 08:31:08.000000 paddypy-0.1.6/paddypy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      233 2023-05-05 08:31:08.000000 paddypy-0.1.6/paddypy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-05 08:31:08.000000 paddypy-0.1.6/paddypy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      127 2023-05-05 08:31:08.000000 paddypy-0.1.6/paddypy.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-05-05 08:31:08.000000 paddypy-0.1.6/paddypy.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-05 08:31:08.765051 paddypy-0.1.6/setup.cfg
--rw-rw-rw-   0        0        0     1480 2023-05-05 08:27:21.000000 paddypy-0.1.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-05 08:40:19.111245 paddypy-0.1.7/
+-rw-rw-rw-   0        0        0     1150 2022-05-16 06:26:09.000000 paddypy-0.1.7/LICENSE
+-rw-rw-rw-   0        0        0     1795 2023-05-05 08:40:19.110746 paddypy-0.1.7/PKG-INFO
+-rw-rw-rw-   0        0        0      918 2023-04-17 10:33:45.000000 paddypy-0.1.7/README.md
+drwxrwxrwx   0        0        0        0 2023-05-05 08:40:19.097246 paddypy-0.1.7/paddypy/
+-rw-rw-rw-   0        0        0      102 2023-04-17 12:26:22.000000 paddypy-0.1.7/paddypy/__init__.py
+-rw-rw-rw-   0        0        0     5772 2023-04-17 12:26:22.000000 paddypy-0.1.7/paddypy/access.py
+-rw-rw-rw-   0        0        0     3849 2023-05-05 08:39:53.000000 paddypy-0.1.7/paddypy/log.py
+drwxrwxrwx   0        0        0        0 2023-05-05 08:40:19.109746 paddypy-0.1.7/paddypy.egg-info/
+-rw-rw-rw-   0        0        0     1795 2023-05-05 08:40:18.000000 paddypy-0.1.7/paddypy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      233 2023-05-05 08:40:19.000000 paddypy-0.1.7/paddypy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-05 08:40:18.000000 paddypy-0.1.7/paddypy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      127 2023-05-05 08:40:18.000000 paddypy-0.1.7/paddypy.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-05-05 08:40:18.000000 paddypy-0.1.7/paddypy.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-05 08:40:19.111245 paddypy-0.1.7/setup.cfg
+-rw-rw-rw-   0        0        0     1480 2023-05-05 08:40:08.000000 paddypy-0.1.7/setup.py
```

### Comparing `paddypy-0.1.6/LICENSE` & `paddypy-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `paddypy-0.1.6/PKG-INFO` & `paddypy-0.1.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: paddypy
-Version: 0.1.6
+Version: 0.1.7
 Summary: Collection of helpfull extensions
 Author: Patrik
 Author-email: <patrikhartl@gmail.com>
 Keywords: python,appconfiguration,azure
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `paddypy-0.1.6/README.md` & `paddypy-0.1.7/README.md`

 * *Files identical despite different names*

### Comparing `paddypy-0.1.6/paddypy/access.py` & `paddypy-0.1.7/paddypy/access.py`

 * *Files identical despite different names*

### Comparing `paddypy-0.1.6/paddypy/log.py` & `paddypy-0.1.7/paddypy/log.py`

 * *Files 8% similar despite different names*

```diff
@@ -62,15 +62,17 @@
                     kwarg_types = {key: type(val).__name__ for key, val in kwargs.items()}
                     log_msg = f'Function {func.__name__}{arg_types} {kwarg_types} Took {total_time:.4f} seconds'
                 else:
                     log_msg = f'Function {func.__name__}{args} {kwargs} Took {total_time:.4f} seconds'
 
                 self.logger.log(msg=log_msg, level=logging.INFO)
                 return result
-            return timeit_wrapper
+
+            return wraps(func)(timeit_wrapper)  # Use wraps here to preserve the original function's metadata
+
         return actual_decorator
 
 
     def except_block(self, inst, exceptionMessage="No message"):
         exceptionMessage = exceptionMessage
         exceptionTimne = str(datetime.datetime.now())
         exceptionType = str(type(inst))
```

### Comparing `paddypy-0.1.6/paddypy.egg-info/PKG-INFO` & `paddypy-0.1.7/paddypy.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: paddypy
-Version: 0.1.6
+Version: 0.1.7
 Summary: Collection of helpfull extensions
 Author: Patrik
 Author-email: <patrikhartl@gmail.com>
 Keywords: python,appconfiguration,azure
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `paddypy-0.1.6/setup.py` & `paddypy-0.1.7/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import os
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
-VERSION = '0.1.6'
+VERSION = '0.1.7'
 DESCRIPTION = 'Collection of helpfull extensions'
 LONG_DESCRIPTION = 'Collection of helpfull extensions'
 
 # Setting up
 setup(
     name="paddypy",
     version=VERSION,
```

