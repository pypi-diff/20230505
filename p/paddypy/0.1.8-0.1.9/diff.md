# Comparing `tmp/paddypy-0.1.8.tar.gz` & `tmp/paddypy-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "paddypy-0.1.8.tar", last modified: Fri May  5 08:43:51 2023, max compression
+gzip compressed data, was "paddypy-0.1.9.tar", last modified: Fri May  5 08:50:03 2023, max compression
```

## Comparing `paddypy-0.1.8.tar` & `paddypy-0.1.9.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-05-05 08:43:51.873527 paddypy-0.1.8/
--rw-rw-rw-   0        0        0     1150 2022-05-16 06:26:09.000000 paddypy-0.1.8/LICENSE
--rw-rw-rw-   0        0        0     1795 2023-05-05 08:43:51.873027 paddypy-0.1.8/PKG-INFO
--rw-rw-rw-   0        0        0      918 2023-04-17 10:33:45.000000 paddypy-0.1.8/README.md
-drwxrwxrwx   0        0        0        0 2023-05-05 08:43:51.862525 paddypy-0.1.8/paddypy/
--rw-rw-rw-   0        0        0      102 2023-04-17 12:26:22.000000 paddypy-0.1.8/paddypy/__init__.py
--rw-rw-rw-   0        0        0     5772 2023-04-17 12:26:22.000000 paddypy-0.1.8/paddypy/access.py
--rw-rw-rw-   0        0        0     3883 2023-05-05 08:43:21.000000 paddypy-0.1.8/paddypy/log.py
-drwxrwxrwx   0        0        0        0 2023-05-05 08:43:51.872026 paddypy-0.1.8/paddypy.egg-info/
--rw-rw-rw-   0        0        0     1795 2023-05-05 08:43:51.000000 paddypy-0.1.8/paddypy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      233 2023-05-05 08:43:51.000000 paddypy-0.1.8/paddypy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-05 08:43:51.000000 paddypy-0.1.8/paddypy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      127 2023-05-05 08:43:51.000000 paddypy-0.1.8/paddypy.egg-info/requires.txt
--rw-rw-rw-   0        0        0        8 2023-05-05 08:43:51.000000 paddypy-0.1.8/paddypy.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-05 08:43:51.874026 paddypy-0.1.8/setup.cfg
--rw-rw-rw-   0        0        0     1480 2023-05-05 08:42:27.000000 paddypy-0.1.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-05 08:50:03.780842 paddypy-0.1.9/
+-rw-rw-rw-   0        0        0     1150 2022-05-16 06:26:09.000000 paddypy-0.1.9/LICENSE
+-rw-rw-rw-   0        0        0     1795 2023-05-05 08:50:03.780343 paddypy-0.1.9/PKG-INFO
+-rw-rw-rw-   0        0        0      918 2023-04-17 10:33:45.000000 paddypy-0.1.9/README.md
+drwxrwxrwx   0        0        0        0 2023-05-05 08:50:03.772842 paddypy-0.1.9/paddypy/
+-rw-rw-rw-   0        0        0      102 2023-04-17 12:26:22.000000 paddypy-0.1.9/paddypy/__init__.py
+-rw-rw-rw-   0        0        0     5772 2023-04-17 12:26:22.000000 paddypy-0.1.9/paddypy/access.py
+-rw-rw-rw-   0        0        0     4047 2023-05-05 08:48:50.000000 paddypy-0.1.9/paddypy/log.py
+drwxrwxrwx   0        0        0        0 2023-05-05 08:50:03.779342 paddypy-0.1.9/paddypy.egg-info/
+-rw-rw-rw-   0        0        0     1795 2023-05-05 08:50:03.000000 paddypy-0.1.9/paddypy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      233 2023-05-05 08:50:03.000000 paddypy-0.1.9/paddypy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-05 08:50:03.000000 paddypy-0.1.9/paddypy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      127 2023-05-05 08:50:03.000000 paddypy-0.1.9/paddypy.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        8 2023-05-05 08:50:03.000000 paddypy-0.1.9/paddypy.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-05 08:50:03.781342 paddypy-0.1.9/setup.cfg
+-rw-rw-rw-   0        0        0     1480 2023-05-05 08:49:23.000000 paddypy-0.1.9/setup.py
```

### Comparing `paddypy-0.1.8/LICENSE` & `paddypy-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `paddypy-0.1.8/PKG-INFO` & `paddypy-0.1.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: paddypy
-Version: 0.1.8
+Version: 0.1.9
 Summary: Collection of helpfull extensions
 Author: Patrik
 Author-email: <patrikhartl@gmail.com>
 Keywords: python,appconfiguration,azure
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `paddypy-0.1.8/README.md` & `paddypy-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `paddypy-0.1.8/paddypy/access.py` & `paddypy-0.1.9/paddypy/access.py`

 * *Files identical despite different names*

### Comparing `paddypy-0.1.8/paddypy/log.py` & `paddypy-0.1.9/paddypy/log.py`

 * *Files 10% similar despite different names*

```diff
@@ -85,7 +85,15 @@
             else:
                 log_msg = f'Function {func.__name__}{args} {kwargs} Took {total_time:.4f} seconds'
 
             self.logger.log(msg=log_msg, level=logging.INFO)
             return result
         return timeit_wrapper
 
+    def __get__(self, instance, owner):
+        def wrapper(*args, **kwargs):
+            return self(instance, *args, **kwargs)
+        return wrapper
+
+
+
+
```

### Comparing `paddypy-0.1.8/paddypy.egg-info/PKG-INFO` & `paddypy-0.1.9/paddypy.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: paddypy
-Version: 0.1.8
+Version: 0.1.9
 Summary: Collection of helpfull extensions
 Author: Patrik
 Author-email: <patrikhartl@gmail.com>
 Keywords: python,appconfiguration,azure
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `paddypy-0.1.8/setup.py` & `paddypy-0.1.9/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import os
 
 here = os.path.abspath(os.path.dirname(__file__))
 
 with codecs.open(os.path.join(here, "README.md"), encoding="utf-8") as fh:
     long_description = "\n" + fh.read()
 
-VERSION = '0.1.8'
+VERSION = '0.1.9'
 DESCRIPTION = 'Collection of helpfull extensions'
 LONG_DESCRIPTION = 'Collection of helpfull extensions'
 
 # Setting up
 setup(
     name="paddypy",
     version=VERSION,
```

