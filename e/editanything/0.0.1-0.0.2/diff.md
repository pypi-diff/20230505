# Comparing `tmp/editanything-0.0.1.tar.gz` & `tmp/editanything-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "editanything-0.0.1.tar", last modified: Fri May  5 10:13:12 2023, max compression
+gzip compressed data, was "editanything-0.0.2.tar", last modified: Fri May  5 10:25:09 2023, max compression
```

## Comparing `editanything-0.0.1.tar` & `editanything-0.0.2.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 alvin-pc   (501) staff       (20)        0 2023-05-05 10:13:12.481743 editanything-0.0.1/
--rw-r--r--   0 alvin-pc   (501) staff       (20)      377 2023-05-05 10:13:12.481454 editanything-0.0.1/PKG-INFO
--rw-r--r--   0 alvin-pc   (501) staff       (20)       58 2023-05-05 09:29:16.000000 editanything-0.0.1/README.md
-drwxr-xr-x   0 alvin-pc   (501) staff       (20)        0 2023-05-05 10:13:12.480223 editanything-0.0.1/editanything.egg-info/
--rw-r--r--   0 alvin-pc   (501) staff       (20)      377 2023-05-05 10:13:12.000000 editanything-0.0.1/editanything.egg-info/PKG-INFO
--rw-r--r--   0 alvin-pc   (501) staff       (20)      268 2023-05-05 10:13:12.000000 editanything-0.0.1/editanything.egg-info/SOURCES.txt
--rw-r--r--   0 alvin-pc   (501) staff       (20)        1 2023-05-05 10:13:12.000000 editanything-0.0.1/editanything.egg-info/dependency_links.txt
--rw-r--r--   0 alvin-pc   (501) staff       (20)       39 2023-05-05 10:13:12.000000 editanything-0.0.1/editanything.egg-info/entry_points.txt
--rw-r--r--   0 alvin-pc   (501) staff       (20)       77 2023-05-05 10:13:12.000000 editanything-0.0.1/editanything.egg-info/requires.txt
--rw-r--r--   0 alvin-pc   (501) staff       (20)        6 2023-05-05 10:13:12.000000 editanything-0.0.1/editanything.egg-info/top_level.txt
--rw-r--r--   0 alvin-pc   (501) staff       (20)       38 2023-05-05 10:13:12.481841 editanything-0.0.1/setup.cfg
--rw-r--r--   0 alvin-pc   (501) staff       (20)      816 2023-05-05 10:13:10.000000 editanything-0.0.1/setup.py
-drwxr-xr-x   0 alvin-pc   (501) staff       (20)        0 2023-05-05 10:13:12.481031 editanything-0.0.1/utils/
--rw-r--r--   0 alvin-pc   (501) staff       (20)        0 2023-05-05 10:11:42.000000 editanything-0.0.1/utils/__init__.py
--rw-r--r--   0 alvin-pc   (501) staff       (20)     3118 2023-04-10 10:02:47.000000 editanything-0.0.1/utils/file.py
+drwxr-xr-x   0 alvin-pc   (501) staff       (20)        0 2023-05-05 10:25:09.868817 editanything-0.0.2/
+-rw-r--r--   0 alvin-pc   (501) staff       (20)      377 2023-05-05 10:25:09.868524 editanything-0.0.2/PKG-INFO
+-rw-r--r--   0 alvin-pc   (501) staff       (20)       58 2023-05-05 09:29:16.000000 editanything-0.0.2/README.md
+drwxr-xr-x   0 alvin-pc   (501) staff       (20)        0 2023-05-05 10:25:09.867130 editanything-0.0.2/editanything.egg-info/
+-rw-r--r--   0 alvin-pc   (501) staff       (20)      377 2023-05-05 10:25:09.000000 editanything-0.0.2/editanything.egg-info/PKG-INFO
+-rw-r--r--   0 alvin-pc   (501) staff       (20)      268 2023-05-05 10:25:09.000000 editanything-0.0.2/editanything.egg-info/SOURCES.txt
+-rw-r--r--   0 alvin-pc   (501) staff       (20)        1 2023-05-05 10:25:09.000000 editanything-0.0.2/editanything.egg-info/dependency_links.txt
+-rw-r--r--   0 alvin-pc   (501) staff       (20)       44 2023-05-05 10:25:09.000000 editanything-0.0.2/editanything.egg-info/entry_points.txt
+-rw-r--r--   0 alvin-pc   (501) staff       (20)       77 2023-05-05 10:25:09.000000 editanything-0.0.2/editanything.egg-info/requires.txt
+-rw-r--r--   0 alvin-pc   (501) staff       (20)        6 2023-05-05 10:25:09.000000 editanything-0.0.2/editanything.egg-info/top_level.txt
+-rw-r--r--   0 alvin-pc   (501) staff       (20)       38 2023-05-05 10:25:09.868914 editanything-0.0.2/setup.cfg
+-rw-r--r--   0 alvin-pc   (501) staff       (20)      821 2023-05-05 10:24:53.000000 editanything-0.0.2/setup.py
+drwxr-xr-x   0 alvin-pc   (501) staff       (20)        0 2023-05-05 10:25:09.867746 editanything-0.0.2/utils/
+-rw-r--r--   0 alvin-pc   (501) staff       (20)        0 2023-05-05 10:11:42.000000 editanything-0.0.2/utils/__init__.py
+-rw-r--r--   0 alvin-pc   (501) staff       (20)     3118 2023-04-10 10:02:47.000000 editanything-0.0.2/utils/file.py
```

### Comparing `editanything-0.0.1/setup.py` & `editanything-0.0.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from setuptools import find_packages, setup
 import utils.file as utils
 
 
 
 setup(
     name='editanything',
-    version='0.0.1',
+    version='0.0.2',
     description='EditAnything',
     long_description=utils.get_file_content("README.md"),
     long_description_content_type='text/markdown',
     author='wfbi',
     author_email='myname@example.com',
     keywords='EditAnything',
     url='https://github.com/xxx/xxxx',
@@ -20,12 +20,12 @@
     classifiers=[
         'Development Status :: 3 - Alpha',
     ],
     license='Apache License 2.0',
     install_requires=utils.parse_requirements('requirements.txt'),
     entry_points={
         'console_scripts': [
-              'editanything = main'
+              'editanything = main:main'
           ]
     },
     ext_modules=[],
 )
```

### Comparing `editanything-0.0.1/utils/file.py` & `editanything-0.0.2/utils/file.py`

 * *Files identical despite different names*

