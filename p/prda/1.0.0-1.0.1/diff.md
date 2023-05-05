# Comparing `tmp/prda-1.0.0.tar.gz` & `tmp/prda-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "prda-1.0.0.tar", last modified: Fri May  5 06:55:56 2023, max compression
+gzip compressed data, was "prda-1.0.1.tar", last modified: Fri May  5 07:38:19 2023, max compression
```

## Comparing `prda-1.0.0.tar` & `prda-1.0.1.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxr-xr-x   0 minshaojie   (501) staff       (20)        0 2023-05-05 06:55:56.521015 prda-1.0.0/
--rw-r--r--   0 minshaojie   (501) staff       (20)     1068 2023-05-05 06:38:57.000000 prda-1.0.0/LICENSE
--rw-r--r--   0 minshaojie   (501) staff       (20)     4369 2023-05-05 06:55:56.520856 prda-1.0.0/PKG-INFO
-drwxr-xr-x   0 minshaojie   (501) staff       (20)        0 2023-05-05 06:55:56.520684 prda-1.0.0/prda.egg-info/
--rw-r--r--   0 minshaojie   (501) staff       (20)     4369 2023-05-05 06:55:56.000000 prda-1.0.0/prda.egg-info/PKG-INFO
--rw-r--r--   0 minshaojie   (501) staff       (20)      155 2023-05-05 06:55:56.000000 prda-1.0.0/prda.egg-info/SOURCES.txt
--rw-r--r--   0 minshaojie   (501) staff       (20)        1 2023-05-05 06:55:56.000000 prda-1.0.0/prda.egg-info/dependency_links.txt
--rw-r--r--   0 minshaojie   (501) staff       (20)       68 2023-05-05 06:55:56.000000 prda-1.0.0/prda.egg-info/requires.txt
--rw-r--r--   0 minshaojie   (501) staff       (20)        1 2023-05-05 06:55:56.000000 prda-1.0.0/prda.egg-info/top_level.txt
--rw-r--r--   0 minshaojie   (501) staff       (20)       38 2023-05-05 06:55:56.521063 prda-1.0.0/setup.cfg
--rw-r--r--   0 minshaojie   (501) staff       (20)     1060 2023-05-05 06:55:53.000000 prda-1.0.0/setup.py
+drwxr-xr-x   0 minshaojie   (501) staff       (20)        0 2023-05-05 07:38:19.204540 prda-1.0.1/
+-rw-r--r--   0 minshaojie   (501) staff       (20)     1068 2023-05-05 06:38:57.000000 prda-1.0.1/LICENSE
+-rw-r--r--   0 minshaojie   (501) staff       (20)     1818 2023-05-05 07:38:19.204240 prda-1.0.1/PKG-INFO
+drwxr-xr-x   0 minshaojie   (501) staff       (20)        0 2023-05-05 07:38:19.204060 prda-1.0.1/prda.egg-info/
+-rw-r--r--   0 minshaojie   (501) staff       (20)     1818 2023-05-05 07:38:19.000000 prda-1.0.1/prda.egg-info/PKG-INFO
+-rw-r--r--   0 minshaojie   (501) staff       (20)      155 2023-05-05 07:38:19.000000 prda-1.0.1/prda.egg-info/SOURCES.txt
+-rw-r--r--   0 minshaojie   (501) staff       (20)        1 2023-05-05 07:38:19.000000 prda-1.0.1/prda.egg-info/dependency_links.txt
+-rw-r--r--   0 minshaojie   (501) staff       (20)       68 2023-05-05 07:38:19.000000 prda-1.0.1/prda.egg-info/requires.txt
+-rw-r--r--   0 minshaojie   (501) staff       (20)        1 2023-05-05 07:38:19.000000 prda-1.0.1/prda.egg-info/top_level.txt
+-rw-r--r--   0 minshaojie   (501) staff       (20)       38 2023-05-05 07:38:19.204585 prda-1.0.1/setup.cfg
+-rw-r--r--   0 minshaojie   (501) staff       (20)      901 2023-05-05 07:38:11.000000 prda-1.0.1/setup.py
```

### Comparing `prda-1.0.0/LICENSE` & `prda-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `prda-1.0.0/setup.py` & `prda-1.0.1/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,23 +1,19 @@
 from setuptools import setup, find_packages
 
 with open('LICENSE', 'r') as f:
     license = f.read()
 
-with open('../README.md', 'r') as f:
-    long_description = f.read()
 
 setup(
     name='prda',
-    version='1.0.0',
+    version='1.0.1',
     author='Shaojie Min',
     author_email='alexmin@cqu.edu.cn',
     description='Prda contains packages for data processing, analysis and visualization. The ultimate goal is to fill the “last mile” between analysts and packages.',
-    long_description=long_description,
-    long_description_content_type='text/markdown',
     url='https://github.com/4AlexMin/prda',
     license=license,
     packages=find_packages(),
     install_requires=[
         'scipy',
         'scikit-learn',
         'pyspark',
```

