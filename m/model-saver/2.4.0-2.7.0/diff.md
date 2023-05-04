# Comparing `tmp/model_saver-2.4.0.tar.gz` & `tmp/model_saver-2.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "model_saver-2.4.0.tar", last modified: Wed May  3 23:12:24 2023, max compression
+gzip compressed data, was "model_saver-2.7.0.tar", last modified: Thu May  4 22:40:53 2023, max compression
```

## Comparing `model_saver-2.4.0.tar` & `model_saver-2.7.0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-05-03 23:12:24.242690 model_saver-2.4.0/
--rw-rw-rw-   0        0        0     1069 2023-05-03 23:09:07.000000 model_saver-2.4.0/LICENSE
--rw-rw-rw-   0        0        0      738 2023-05-03 23:12:24.060690 model_saver-2.4.0/PKG-INFO
--rw-rw-rw-   0        0        0     1821 2023-05-03 23:09:07.000000 model_saver-2.4.0/README.md
-drwxrwxrwx   0        0        0        0 2023-05-03 23:12:23.301705 model_saver-2.4.0/model_saver/
--rw-rw-rw-   0        0        0       34 2023-05-03 23:09:07.000000 model_saver-2.4.0/model_saver/__init__.py
--rw-rw-rw-   0        0        0      477 2023-05-03 23:09:07.000000 model_saver-2.4.0/model_saver/modelSaver.py
-drwxrwxrwx   0        0        0        0 2023-05-03 23:12:24.057691 model_saver-2.4.0/model_saver.egg-info/
--rw-rw-rw-   0        0        0      738 2023-05-03 23:12:17.000000 model_saver-2.4.0/model_saver.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      216 2023-05-03 23:12:18.000000 model_saver-2.4.0/model_saver.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-03 23:12:18.000000 model_saver-2.4.0/model_saver.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       12 2023-05-03 23:12:18.000000 model_saver-2.4.0/model_saver.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-03 23:12:24.243689 model_saver-2.4.0/setup.cfg
--rw-rw-rw-   0        0        0      826 2023-05-03 23:09:07.000000 model_saver-2.4.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-04 22:40:53.878150 model_saver-2.7.0/
+-rw-rw-rw-   0        0        0     1069 2023-05-03 23:09:07.000000 model_saver-2.7.0/LICENSE
+-rw-rw-rw-   0        0        0      738 2023-05-04 22:40:53.876150 model_saver-2.7.0/PKG-INFO
+-rw-rw-rw-   0        0        0     1821 2023-05-03 23:09:07.000000 model_saver-2.7.0/README.md
+drwxrwxrwx   0        0        0        0 2023-05-04 22:40:53.842151 model_saver-2.7.0/model_saver/
+-rw-rw-rw-   0        0        0       35 2023-05-04 22:36:51.000000 model_saver-2.7.0/model_saver/__init__.py
+-rw-rw-rw-   0        0        0      477 2023-05-03 23:09:07.000000 model_saver-2.7.0/model_saver/modelSaver.py
+drwxrwxrwx   0        0        0        0 2023-05-04 22:40:53.873149 model_saver-2.7.0/model_saver.egg-info/
+-rw-rw-rw-   0        0        0      738 2023-05-04 22:40:52.000000 model_saver-2.7.0/model_saver.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      216 2023-05-04 22:40:52.000000 model_saver-2.7.0/model_saver.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-04 22:40:52.000000 model_saver-2.7.0/model_saver.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       12 2023-05-04 22:40:52.000000 model_saver-2.7.0/model_saver.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-04 22:40:53.878150 model_saver-2.7.0/setup.cfg
+-rw-rw-rw-   0        0        0      826 2023-05-04 22:39:02.000000 model_saver-2.7.0/setup.py
```

### Comparing `model_saver-2.4.0/LICENSE` & `model_saver-2.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `model_saver-2.4.0/PKG-INFO` & `model_saver-2.7.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: model_saver
-Version: 2.4.0
+Version: 2.7.0
 Summary: A package for saving and loading machine learning models using pickle
 Home-page: https://github.com/yourusername/model_saver
 Author: somkietacode
 Author-email: s.r.a.ouedraogo@gmail.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
```

### Comparing `model_saver-2.4.0/README.md` & `model_saver-2.7.0/README.md`

 * *Files identical despite different names*

### Comparing `model_saver-2.4.0/model_saver.egg-info/PKG-INFO` & `model_saver-2.7.0/model_saver.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: model-saver
-Version: 2.4.0
+Version: 2.7.0
 Summary: A package for saving and loading machine learning models using pickle
 Home-page: https://github.com/yourusername/model_saver
 Author: somkietacode
 Author-email: s.r.a.ouedraogo@gmail.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
```

### Comparing `model_saver-2.4.0/setup.py` & `model_saver-2.7.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
     name='model_saver',
-    version='2.4.0',
+    version='2.7.0',
     description='A package for saving and loading machine learning models using pickle',
     author='somkietacode',
     author_email='s.r.a.ouedraogo@gmail.com',
     url='https://github.com/yourusername/model_saver',
     packages=['model_saver'],
     install_requires=[
     ],
```

