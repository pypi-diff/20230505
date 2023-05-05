# Comparing `tmp/rfcxtf-0.0.2.tar.gz` & `tmp/rfcxtf-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rfcxtf-0.0.2.tar", last modified: Fri May  5 10:36:50 2023, max compression
+gzip compressed data, was "rfcxtf-0.0.3.tar", last modified: Fri May  5 11:19:31 2023, max compression
```

## Comparing `rfcxtf-0.0.2.tar` & `rfcxtf-0.0.3.tar`

### file list

```diff
@@ -1,14 +1,19 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 10:36:50.231644 rfcxtf-0.0.2/
--rw-r--r--   0 root         (0) root         (0)      482 2023-05-05 10:36:50.229963 rfcxtf-0.0.2/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 10:36:50.197663 rfcxtf-0.0.2/rfcxtf/
--rw-r--r--   0 root         (0) root         (0)      593 2023-05-04 09:58:45.000000 rfcxtf-0.0.2/rfcxtf/ClassifierBase.py
--rw-r--r--   0 root         (0) root         (0)     2602 2023-05-04 10:33:29.000000 rfcxtf-0.0.2/rfcxtf/ClassifierTF2.py
--rw-r--r--   0 root         (0) root         (0)       58 2023-05-04 10:26:02.000000 rfcxtf-0.0.2/rfcxtf/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 10:36:50.225754 rfcxtf-0.0.2/rfcxtf.egg-info/
--rw-r--r--   0 root         (0) root         (0)      482 2023-05-05 10:36:50.000000 rfcxtf-0.0.2/rfcxtf.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      225 2023-05-05 10:36:50.000000 rfcxtf-0.0.2/rfcxtf.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-05 10:36:50.000000 rfcxtf-0.0.2/rfcxtf.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       27 2023-05-05 10:36:50.000000 rfcxtf-0.0.2/rfcxtf.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        7 2023-05-05 10:36:50.000000 rfcxtf-0.0.2/rfcxtf.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-05-05 10:36:50.232666 rfcxtf-0.0.2/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      778 2023-05-05 10:36:01.000000 rfcxtf-0.0.2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 11:19:31.007766 rfcxtf-0.0.3/
+-rw-r--r--   0 root         (0) root         (0)      482 2023-05-05 11:19:31.006429 rfcxtf-0.0.3/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 11:19:30.950410 rfcxtf-0.0.3/rfcxtf/
+-rw-r--r--   0 root         (0) root         (0)      593 2023-05-04 09:58:45.000000 rfcxtf-0.0.3/rfcxtf/ClassifierBase.py
+-rw-r--r--   0 root         (0) root         (0)     2602 2023-05-04 10:33:29.000000 rfcxtf-0.0.3/rfcxtf/ClassifierTF2.py
+-rw-r--r--   0 root         (0) root         (0)       58 2023-05-04 10:26:02.000000 rfcxtf-0.0.3/rfcxtf/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 11:19:31.000812 rfcxtf-0.0.3/rfcxtf/utils/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-05 11:11:18.000000 rfcxtf-0.0.3/rfcxtf/utils/__init__.py
+-rw-r--r--   0 root         (0) root         (0)       48 2023-05-04 09:05:14.000000 rfcxtf-0.0.3/rfcxtf/utils/exceptions.py
+-rw-r--r--   0 root         (0) root         (0)      272 2023-05-04 09:05:14.000000 rfcxtf-0.0.3/rfcxtf/utils/io.py
+-rw-r--r--   0 root         (0) root         (0)      321 2023-05-04 09:05:14.000000 rfcxtf-0.0.3/rfcxtf/utils/postprocessor.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 11:19:30.978975 rfcxtf-0.0.3/rfcxtf.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      482 2023-05-05 11:19:30.000000 rfcxtf-0.0.3/rfcxtf.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      326 2023-05-05 11:19:30.000000 rfcxtf-0.0.3/rfcxtf.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-05 11:19:30.000000 rfcxtf-0.0.3/rfcxtf.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       27 2023-05-05 11:19:30.000000 rfcxtf-0.0.3/rfcxtf.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        7 2023-05-05 11:19:30.000000 rfcxtf-0.0.3/rfcxtf.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-05-05 11:19:31.008679 rfcxtf-0.0.3/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      778 2023-05-05 11:17:07.000000 rfcxtf-0.0.3/setup.py
```

### Comparing `rfcxtf-0.0.2/rfcxtf/ClassifierBase.py` & `rfcxtf-0.0.3/rfcxtf/ClassifierBase.py`

 * *Files identical despite different names*

### Comparing `rfcxtf-0.0.2/rfcxtf/ClassifierTF2.py` & `rfcxtf-0.0.3/rfcxtf/ClassifierTF2.py`

 * *Files identical despite different names*

### Comparing `rfcxtf-0.0.2/setup.py` & `rfcxtf-0.0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 
 REQUIRED_PACKAGES = ['tensorflow', 'pysndfile', 'numpy']
 
 setup(name='rfcxtf',
-      version='0.0.2',
+      version='0.0.3',
       url='https://github.com/rfcx/rfcx-sdk-python',
       license='None',
       author='Rainforest Connection',
       author_email='antony@rfcx.org',
       install_requires=REQUIRED_PACKAGES,
       description='Support for building TensorFlow classifiers on Arbimon and Guardian platforms',
       packages=find_packages(exclude=['tests']),
```

