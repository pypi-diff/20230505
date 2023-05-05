# Comparing `tmp/bizdates-0.1.0.tar.gz` & `tmp/bizdates-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\bizdates-0.1.0.tar", last modified: Fri May  5 08:46:33 2023, max compression
+gzip compressed data, was "dist\bizdates-1.0.0.tar", last modified: Fri May  5 09:07:49 2023, max compression
```

## Comparing `bizdates-0.1.0.tar` & `bizdates-1.0.0.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxrwxrwx   0        0        0        0 2023-05-05 08:46:33.970789 bizdates-0.1.0/
--rw-rw-rw-   0        0        0      721 2023-05-05 08:46:33.969788 bizdates-0.1.0/PKG-INFO
--rw-rw-rw-   0        0        0        0 2022-04-11 07:27:06.000000 bizdates-0.1.0/README.rst
-drwxrwxrwx   0        0        0        0 2023-05-05 08:46:33.956223 bizdates-0.1.0/bizdates/
--rw-rw-rw-   0        0        0      296 2022-06-27 12:12:41.000000 bizdates-0.1.0/bizdates/__init__.py
--rw-rw-rw-   0        0        0     1772 2022-07-12 08:55:07.000000 bizdates-0.1.0/bizdates/bizdates.py
-drwxrwxrwx   0        0        0        0 2023-05-05 08:46:33.967894 bizdates-0.1.0/bizdates.egg-info/
--rw-rw-rw-   0        0        0      721 2023-05-05 08:46:33.000000 bizdates-0.1.0/bizdates.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      220 2023-05-05 08:46:33.000000 bizdates-0.1.0/bizdates.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-05 08:46:33.000000 bizdates-0.1.0/bizdates.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-05-05 08:46:33.000000 bizdates-0.1.0/bizdates.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-05-05 08:46:33.000000 bizdates-0.1.0/bizdates.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-05 08:46:33.970789 bizdates-0.1.0/setup.cfg
--rw-rw-rw-   0        0        0      845 2022-04-11 08:30:27.000000 bizdates-0.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-05 09:07:49.142061 bizdates-1.0.0/
+-rw-rw-rw-   0        0        0      667 2023-05-05 09:07:49.140068 bizdates-1.0.0/PKG-INFO
+-rw-rw-rw-   0        0        0        0 2022-04-11 07:27:06.000000 bizdates-1.0.0/README.rst
+drwxrwxrwx   0        0        0        0 2023-05-05 09:07:49.118434 bizdates-1.0.0/bizdates/
+-rw-rw-rw-   0        0        0      296 2022-06-27 12:12:41.000000 bizdates-1.0.0/bizdates/__init__.py
+-rw-rw-rw-   0        0        0     1772 2022-07-12 08:55:07.000000 bizdates-1.0.0/bizdates/bizdates.py
+drwxrwxrwx   0        0        0        0 2023-05-05 09:07:49.138072 bizdates-1.0.0/bizdates.egg-info/
+-rw-rw-rw-   0        0        0      667 2023-05-05 09:07:48.000000 bizdates-1.0.0/bizdates.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      220 2023-05-05 09:07:48.000000 bizdates-1.0.0/bizdates.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-05 09:07:48.000000 bizdates-1.0.0/bizdates.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-05-05 09:07:48.000000 bizdates-1.0.0/bizdates.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-05-05 09:07:48.000000 bizdates-1.0.0/bizdates.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-05 09:07:49.142061 bizdates-1.0.0/setup.cfg
+-rw-rw-rw-   0        0        0      791 2023-05-05 09:07:39.000000 bizdates-1.0.0/setup.py
```

### Comparing `bizdates-0.1.0/PKG-INFO` & `bizdates-1.0.0/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: bizdates
-Version: 0.1.0
+Version: 1.0.0
 Summary: A Python package for working with business dates
-Home-page: https://github.com/shuds13/pyexample
+Home-page: 
 Author: Paul Gray
-Author-email: prgray86@gmail.com
+Author-email: 
 License: BSD 2-clause
 Platform: UNKNOWN
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 2
```

### Comparing `bizdates-0.1.0/bizdates/bizdates.py` & `bizdates-1.0.0/bizdates/bizdates.py`

 * *Files identical despite different names*

### Comparing `bizdates-0.1.0/bizdates.egg-info/PKG-INFO` & `bizdates-1.0.0/bizdates.egg-info/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: bizdates
-Version: 0.1.0
+Version: 1.0.0
 Summary: A Python package for working with business dates
-Home-page: https://github.com/shuds13/pyexample
+Home-page: 
 Author: Paul Gray
-Author-email: prgray86@gmail.com
+Author-email: 
 License: BSD 2-clause
 Platform: UNKNOWN
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 2
```

### Comparing `bizdates-0.1.0/setup.py` & `bizdates-1.0.0/setup.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 from setuptools import setup
 
 setup(
     name='bizdates',
-    version='0.1.0',    
+    version='1.0.0',    
     description='A Python package for working with business dates',
-    url='https://github.com/shuds13/pyexample',
+    url='',
     author='Paul Gray',
-    author_email='prgray86@gmail.com',
+    author_email='',
     license='BSD 2-clause',
     packages=['bizdates'],
     install_requires=['datetime'],
 
     classifiers=[
         'Development Status :: 1 - Planning',
         'Intended Audience :: Science/Research',
```

