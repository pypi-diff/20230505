# Comparing `tmp/systematica-0.0.1.tar.gz` & `tmp/systematica-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "systematica-0.0.1.tar", last modified: Thu May  4 21:53:51 2023, max compression
+gzip compressed data, was "systematica-0.0.2.tar", last modified: Thu May  4 22:10:59 2023, max compression
```

## Comparing `systematica-0.0.1.tar` & `systematica-0.0.2.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxr-xr-x   0 tucudeanadrian   (502) staff       (20)        0 2023-05-04 21:53:51.594627 systematica-0.0.1/
--rw-r--r--   0 tucudeanadrian   (502) staff       (20)      597 2023-05-04 21:53:51.594130 systematica-0.0.1/PKG-INFO
-drwxr-xr-x   0 tucudeanadrian   (502) staff       (20)        0 2023-05-04 21:53:51.587188 systematica-0.0.1/libname/
--rw-r--r--   0 tucudeanadrian   (502) staff       (20)       37 2023-05-04 21:37:24.000000 systematica-0.0.1/libname/Systematica.py
--rw-r--r--   0 tucudeanadrian   (502) staff       (20)       29 2023-05-04 21:42:01.000000 systematica-0.0.1/libname/__init__.py
--rw-r--r--   0 tucudeanadrian   (502) staff       (20)       38 2023-05-04 21:53:51.594827 systematica-0.0.1/setup.cfg
--rw-r--r--   0 tucudeanadrian   (502) staff       (20)      976 2023-05-04 21:52:24.000000 systematica-0.0.1/setup.py
-drwxr-xr-x   0 tucudeanadrian   (502) staff       (20)        0 2023-05-04 21:53:51.593289 systematica-0.0.1/systematica.egg-info/
--rw-r--r--   0 tucudeanadrian   (502) staff       (20)      597 2023-05-04 21:53:51.000000 systematica-0.0.1/systematica.egg-info/PKG-INFO
--rw-r--r--   0 tucudeanadrian   (502) staff       (20)      225 2023-05-04 21:53:51.000000 systematica-0.0.1/systematica.egg-info/SOURCES.txt
--rw-r--r--   0 tucudeanadrian   (502) staff       (20)        1 2023-05-04 21:53:51.000000 systematica-0.0.1/systematica.egg-info/dependency_links.txt
--rw-r--r--   0 tucudeanadrian   (502) staff       (20)       21 2023-05-04 21:53:51.000000 systematica-0.0.1/systematica.egg-info/requires.txt
--rw-r--r--   0 tucudeanadrian   (502) staff       (20)        8 2023-05-04 21:53:51.000000 systematica-0.0.1/systematica.egg-info/top_level.txt
+drwxr-xr-x   0 tucudeanadrian   (502) staff       (20)        0 2023-05-04 22:10:59.816656 systematica-0.0.2/
+-rw-r--r--   0 tucudeanadrian   (502) staff       (20)      597 2023-05-04 22:10:59.815559 systematica-0.0.2/PKG-INFO
+drwxr-xr-x   0 tucudeanadrian   (502) staff       (20)        0 2023-05-04 22:10:59.806172 systematica-0.0.2/libname/
+-rw-r--r--   0 tucudeanadrian   (502) staff       (20)       37 2023-05-04 22:07:02.000000 systematica-0.0.2/libname/Systematica.py
+-rw-r--r--   0 tucudeanadrian   (502) staff       (20)       29 2023-05-04 22:07:02.000000 systematica-0.0.2/libname/__init__.py
+-rw-r--r--   0 tucudeanadrian   (502) staff       (20)       38 2023-05-04 22:10:59.817653 systematica-0.0.2/setup.cfg
+-rw-r--r--   0 tucudeanadrian   (502) staff       (20)      976 2023-05-04 22:07:02.000000 systematica-0.0.2/setup.py
+drwxr-xr-x   0 tucudeanadrian   (502) staff       (20)        0 2023-05-04 22:10:59.814450 systematica-0.0.2/systematica.egg-info/
+-rw-r--r--   0 tucudeanadrian   (502) staff       (20)      597 2023-05-04 22:10:59.000000 systematica-0.0.2/systematica.egg-info/PKG-INFO
+-rw-r--r--   0 tucudeanadrian   (502) staff       (20)      225 2023-05-04 22:10:59.000000 systematica-0.0.2/systematica.egg-info/SOURCES.txt
+-rw-r--r--   0 tucudeanadrian   (502) staff       (20)        1 2023-05-04 22:10:59.000000 systematica-0.0.2/systematica.egg-info/dependency_links.txt
+-rw-r--r--   0 tucudeanadrian   (502) staff       (20)       21 2023-05-04 22:10:59.000000 systematica-0.0.2/systematica.egg-info/requires.txt
+-rw-r--r--   0 tucudeanadrian   (502) staff       (20)        8 2023-05-04 22:10:59.000000 systematica-0.0.2/systematica.egg-info/top_level.txt
```

### Comparing `systematica-0.0.1/PKG-INFO` & `systematica-0.0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: systematica
-Version: 0.0.1
+Version: 0.0.2
 Summary: Simple Simulator for Computer Vision
 Author: TucuAI (Tucudean Adrian-Ionut)
 Author-email: <Tucudean.Adrian.Ionut@outlook.com>
 Keywords: python,simulator,computer vision,advanced driving,camera stream,camera handler
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `systematica-0.0.1/setup.py` & `systematica-0.0.2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from setuptools import setup,find_packages
-VERSION = '0.0.1'
+VERSION = '0.0.2'
 DESCRIPTION = 'Simple Simulator for Computer Vision'
 LONG_DESCRIPTION = 'A package that allows to test how computer vision algorithms for advanced driving systems performs '
 
 # Setting up
 setup(
     name="systematica",
     version=VERSION,
```

### Comparing `systematica-0.0.1/systematica.egg-info/PKG-INFO` & `systematica-0.0.2/systematica.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: systematica
-Version: 0.0.1
+Version: 0.0.2
 Summary: Simple Simulator for Computer Vision
 Author: TucuAI (Tucudean Adrian-Ionut)
 Author-email: <Tucudean.Adrian.Ionut@outlook.com>
 Keywords: python,simulator,computer vision,advanced driving,camera stream,camera handler
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

