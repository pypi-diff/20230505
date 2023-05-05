# Comparing `tmp/pyFCST-0.0.1.tar.gz` & `tmp/pyFCST-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pyFCST-0.0.1.tar", last modified: Thu May  4 22:25:08 2023, max compression
+gzip compressed data, was "dist/pyFCST-0.0.2.tar", last modified: Fri May  5 00:18:20 2023, max compression
```

## Comparing `pyFCST-0.0.1.tar` & `pyFCST-0.0.2.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxr-x   0 james     (1000) james     (1000)        0 2023-05-04 22:25:08.616341 pyFCST-0.0.1/
--rw-rw-r--   0 james     (1000) james     (1000)      354 2023-05-04 22:25:08.616341 pyFCST-0.0.1/PKG-INFO
--rw-rw-r--   0 james     (1000) james     (1000)       68 2023-05-04 21:44:54.000000 pyFCST-0.0.1/README.rst
-drwxrwxr-x   0 james     (1000) james     (1000)        0 2023-05-04 22:25:08.616341 pyFCST-0.0.1/pyFCST/
--rw-rw-r--   0 james     (1000) james     (1000)     3325 2023-05-04 21:09:44.000000 pyFCST-0.0.1/pyFCST/__init__.py
-drwxrwxr-x   0 james     (1000) james     (1000)        0 2023-05-04 22:25:08.616341 pyFCST-0.0.1/pyFCST.egg-info/
--rw-rw-r--   0 james     (1000) james     (1000)      354 2023-05-04 22:25:08.000000 pyFCST-0.0.1/pyFCST.egg-info/PKG-INFO
--rw-rw-r--   0 james     (1000) james     (1000)      197 2023-05-04 22:25:08.000000 pyFCST-0.0.1/pyFCST.egg-info/SOURCES.txt
--rw-rw-r--   0 james     (1000) james     (1000)        1 2023-05-04 22:25:08.000000 pyFCST-0.0.1/pyFCST.egg-info/dependency_links.txt
--rw-rw-r--   0 james     (1000) james     (1000)      173 2023-05-04 22:25:08.000000 pyFCST-0.0.1/pyFCST.egg-info/requires.txt
--rw-rw-r--   0 james     (1000) james     (1000)        7 2023-05-04 22:25:08.000000 pyFCST-0.0.1/pyFCST.egg-info/top_level.txt
--rw-rw-r--   0 james     (1000) james     (1000)       38 2023-05-04 22:25:08.616341 pyFCST-0.0.1/setup.cfg
--rw-rw-r--   0 james     (1000) james     (1000)      752 2023-05-04 22:25:05.000000 pyFCST-0.0.1/setup.py
+drwxrwxr-x   0 james     (1000) james     (1000)        0 2023-05-05 00:18:20.208723 pyFCST-0.0.2/
+-rw-rw-r--   0 james     (1000) james     (1000)      354 2023-05-05 00:18:20.208723 pyFCST-0.0.2/PKG-INFO
+-rw-rw-r--   0 james     (1000) james     (1000)       68 2023-05-04 21:44:54.000000 pyFCST-0.0.2/README.rst
+drwxrwxr-x   0 james     (1000) james     (1000)        0 2023-05-05 00:18:20.208723 pyFCST-0.0.2/pyFCST/
+-rw-rw-r--   0 james     (1000) james     (1000)     3325 2023-05-04 21:09:44.000000 pyFCST-0.0.2/pyFCST/__init__.py
+drwxrwxr-x   0 james     (1000) james     (1000)        0 2023-05-05 00:18:20.208723 pyFCST-0.0.2/pyFCST.egg-info/
+-rw-rw-r--   0 james     (1000) james     (1000)      354 2023-05-05 00:18:20.000000 pyFCST-0.0.2/pyFCST.egg-info/PKG-INFO
+-rw-rw-r--   0 james     (1000) james     (1000)      197 2023-05-05 00:18:20.000000 pyFCST-0.0.2/pyFCST.egg-info/SOURCES.txt
+-rw-rw-r--   0 james     (1000) james     (1000)        1 2023-05-05 00:18:20.000000 pyFCST-0.0.2/pyFCST.egg-info/dependency_links.txt
+-rw-rw-r--   0 james     (1000) james     (1000)      172 2023-05-05 00:18:20.000000 pyFCST-0.0.2/pyFCST.egg-info/requires.txt
+-rw-rw-r--   0 james     (1000) james     (1000)        7 2023-05-05 00:18:20.000000 pyFCST-0.0.2/pyFCST.egg-info/top_level.txt
+-rw-rw-r--   0 james     (1000) james     (1000)       38 2023-05-05 00:18:20.208723 pyFCST-0.0.2/setup.cfg
+-rw-rw-r--   0 james     (1000) james     (1000)      751 2023-05-05 00:16:50.000000 pyFCST-0.0.2/setup.py
```

### Comparing `pyFCST-0.0.1/pyFCST/__init__.py` & `pyFCST-0.0.2/pyFCST/__init__.py`

 * *Files identical despite different names*

### Comparing `pyFCST-0.0.1/setup.py` & `pyFCST-0.0.2/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 from setuptools import setup
 from distutils.core import setup
 
 setup(
     name='pyFCST',
-    version='0.0.1',
+    version='0.0.2',
     author='FCST development group',
     author_email='jwoodfor@ualberta.ca',
     packages=['pyFCST'],
     python_requires='>=3.6',
     url='http://pypi.python.org/pypi/pyfcst/',
     license='LICENSE.txt',
     description='Utilities for pyFCST.',
     long_description=open('README.rst').read(),
     install_requires=[
         "scipy >= 0.9.0",
         "numpy >= 1.6.1",
-        "bittarray >= 2.7.3",
+        "bitarray >= 2.7.3",
         "vtk >= 8.2.0",
         "mayavi >= 4.7.1",
         "mahotas >= 1.4.13",
         "pillow >= 9.3.0",
         "scikit-image >= 0.19.3",
         "simpleitk >= 2.0.2",
         "sphinx >= 5.0.2",
```

