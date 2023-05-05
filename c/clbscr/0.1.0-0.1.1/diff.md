# Comparing `tmp/clbscr-0.1.0.tar.gz` & `tmp/clbscr-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/clbscr-0.1.0.tar", last modified: Fri May  5 17:29:13 2023, max compression
+gzip compressed data, was "dist/clbscr-0.1.1.tar", last modified: Fri May  5 17:47:34 2023, max compression
```

## Comparing `clbscr-0.1.0.tar` & `clbscr-0.1.1.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 dave       (501) staff       (20)        0 2023-05-05 17:29:13.000000 clbscr-0.1.0/
--rw-r--r--   0 dave       (501) staff       (20)      882 2023-05-05 17:29:13.000000 clbscr-0.1.0/PKG-INFO
--rw-r--r--   0 dave       (501) staff       (20)        0 2023-05-05 17:19:54.000000 clbscr-0.1.0/README.md
-drwxr-xr-x   0 dave       (501) staff       (20)        0 2023-05-05 17:29:13.000000 clbscr-0.1.0/clbscr/
--rw-r--r--   0 dave       (501) staff       (20)      169 2023-05-05 16:55:15.000000 clbscr-0.1.0/clbscr/__init__.py
--rw-r--r--   0 dave       (501) staff       (20)       32 2023-05-05 16:51:01.000000 clbscr-0.1.0/clbscr/maker.py
-drwxr-xr-x   0 dave       (501) staff       (20)        0 2023-05-05 17:29:13.000000 clbscr-0.1.0/clbscr.egg-info/
--rw-r--r--   0 dave       (501) staff       (20)      882 2023-05-05 17:29:13.000000 clbscr-0.1.0/clbscr.egg-info/PKG-INFO
--rw-r--r--   0 dave       (501) staff       (20)      173 2023-05-05 17:29:13.000000 clbscr-0.1.0/clbscr.egg-info/SOURCES.txt
--rw-r--r--   0 dave       (501) staff       (20)        1 2023-05-05 17:29:13.000000 clbscr-0.1.0/clbscr.egg-info/dependency_links.txt
--rw-r--r--   0 dave       (501) staff       (20)        7 2023-05-05 17:29:13.000000 clbscr-0.1.0/clbscr.egg-info/top_level.txt
--rw-r--r--   0 dave       (501) staff       (20)       38 2023-05-05 17:29:13.000000 clbscr-0.1.0/setup.cfg
--rw-r--r--   0 dave       (501) staff       (20)     1136 2023-05-05 17:29:11.000000 clbscr-0.1.0/setup.py
+drwxr-xr-x   0 dave       (501) staff       (20)        0 2023-05-05 17:47:34.000000 clbscr-0.1.1/
+-rw-r--r--   0 dave       (501) staff       (20)      882 2023-05-05 17:47:34.000000 clbscr-0.1.1/PKG-INFO
+-rw-r--r--   0 dave       (501) staff       (20)        0 2023-05-05 17:19:54.000000 clbscr-0.1.1/README.md
+drwxr-xr-x   0 dave       (501) staff       (20)        0 2023-05-05 17:47:34.000000 clbscr-0.1.1/clbscr/
+-rw-r--r--   0 dave       (501) staff       (20)      169 2023-05-05 16:55:15.000000 clbscr-0.1.1/clbscr/__init__.py
+-rw-r--r--   0 dave       (501) staff       (20)       34 2023-05-05 17:47:04.000000 clbscr-0.1.1/clbscr/maker.py
+drwxr-xr-x   0 dave       (501) staff       (20)        0 2023-05-05 17:47:34.000000 clbscr-0.1.1/clbscr.egg-info/
+-rw-r--r--   0 dave       (501) staff       (20)      882 2023-05-05 17:47:34.000000 clbscr-0.1.1/clbscr.egg-info/PKG-INFO
+-rw-r--r--   0 dave       (501) staff       (20)      173 2023-05-05 17:47:34.000000 clbscr-0.1.1/clbscr.egg-info/SOURCES.txt
+-rw-r--r--   0 dave       (501) staff       (20)        1 2023-05-05 17:47:34.000000 clbscr-0.1.1/clbscr.egg-info/dependency_links.txt
+-rw-r--r--   0 dave       (501) staff       (20)        7 2023-05-05 17:47:34.000000 clbscr-0.1.1/clbscr.egg-info/top_level.txt
+-rw-r--r--   0 dave       (501) staff       (20)       38 2023-05-05 17:47:34.000000 clbscr-0.1.1/setup.cfg
+-rw-r--r--   0 dave       (501) staff       (20)     1136 2023-05-05 17:47:29.000000 clbscr-0.1.1/setup.py
```

### Comparing `clbscr-0.1.0/PKG-INFO` & `clbscr-0.1.1/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: clbscr
-Version: 0.1.0
+Version: 0.1.1
 Summary: A package for doing some useful stuff
 Home-page: https://github.com/davegimo/clbscr
 Author: Davide Gimondo
 Author-email: davegimo@example.com
 License: MIT
 Description: UNKNOWN
 Keywords: my-package,example,demo
```

### Comparing `clbscr-0.1.0/clbscr.egg-info/PKG-INFO` & `clbscr-0.1.1/clbscr.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: clbscr
-Version: 0.1.0
+Version: 0.1.1
 Summary: A package for doing some useful stuff
 Home-page: https://github.com/davegimo/clbscr
 Author: Davide Gimondo
 Author-email: davegimo@example.com
 License: MIT
 Description: UNKNOWN
 Keywords: my-package,example,demo
```

### Comparing `clbscr-0.1.0/setup.py` & `clbscr-0.1.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='clbscr',
-    version='0.1.0',
+    version='0.1.1',
     author='Davide Gimondo',
     author_email='davegimo@example.com',
     description='A package for doing some useful stuff',
     long_description=open('README.md').read(),
     long_description_content_type='text/markdown',
     url='https://github.com/davegimo/clbscr',
     packages=find_packages(),
```

