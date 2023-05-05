# Comparing `tmp/editanything-0.0.4.tar.gz` & `tmp/editanything-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "editanything-0.0.4.tar", last modified: Fri May  5 10:32:45 2023, max compression
+gzip compressed data, was "editanything-0.0.5.tar", last modified: Fri May  5 10:41:48 2023, max compression
```

## Comparing `editanything-0.0.4.tar` & `editanything-0.0.5.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 alvin-pc   (501) staff       (20)        0 2023-05-05 10:32:45.973443 editanything-0.0.4/
--rw-r--r--   0 alvin-pc   (501) staff       (20)      377 2023-05-05 10:32:45.973168 editanything-0.0.4/PKG-INFO
--rw-r--r--   0 alvin-pc   (501) staff       (20)       58 2023-05-05 09:29:16.000000 editanything-0.0.4/README.md
-drwxr-xr-x   0 alvin-pc   (501) staff       (20)        0 2023-05-05 10:32:45.971915 editanything-0.0.4/editanything.egg-info/
--rw-r--r--   0 alvin-pc   (501) staff       (20)      377 2023-05-05 10:32:45.000000 editanything-0.0.4/editanything.egg-info/PKG-INFO
--rw-r--r--   0 alvin-pc   (501) staff       (20)      268 2023-05-05 10:32:45.000000 editanything-0.0.4/editanything.egg-info/SOURCES.txt
--rw-r--r--   0 alvin-pc   (501) staff       (20)        1 2023-05-05 10:32:45.000000 editanything-0.0.4/editanything.egg-info/dependency_links.txt
--rw-r--r--   0 alvin-pc   (501) staff       (20)       39 2023-05-05 10:32:45.000000 editanything-0.0.4/editanything.egg-info/entry_points.txt
--rw-r--r--   0 alvin-pc   (501) staff       (20)       77 2023-05-05 10:32:45.000000 editanything-0.0.4/editanything.egg-info/requires.txt
--rw-r--r--   0 alvin-pc   (501) staff       (20)        6 2023-05-05 10:32:45.000000 editanything-0.0.4/editanything.egg-info/top_level.txt
--rw-r--r--   0 alvin-pc   (501) staff       (20)       38 2023-05-05 10:32:45.973580 editanything-0.0.4/setup.cfg
--rw-r--r--   0 alvin-pc   (501) staff       (20)      816 2023-05-05 10:32:43.000000 editanything-0.0.4/setup.py
-drwxr-xr-x   0 alvin-pc   (501) staff       (20)        0 2023-05-05 10:32:45.972432 editanything-0.0.4/utils/
--rw-r--r--   0 alvin-pc   (501) staff       (20)        0 2023-05-05 10:11:42.000000 editanything-0.0.4/utils/__init__.py
--rw-r--r--   0 alvin-pc   (501) staff       (20)     3118 2023-04-10 10:02:47.000000 editanything-0.0.4/utils/file.py
+drwxr-xr-x   0 alvin-pc   (501) staff       (20)        0 2023-05-05 10:41:48.062540 editanything-0.0.5/
+-rw-r--r--   0 alvin-pc   (501) staff       (20)      377 2023-05-05 10:41:48.062214 editanything-0.0.5/PKG-INFO
+-rw-r--r--   0 alvin-pc   (501) staff       (20)       58 2023-05-05 09:29:16.000000 editanything-0.0.5/README.md
+drwxr-xr-x   0 alvin-pc   (501) staff       (20)        0 2023-05-05 10:41:48.061030 editanything-0.0.5/editanything.egg-info/
+-rw-r--r--   0 alvin-pc   (501) staff       (20)      377 2023-05-05 10:41:47.000000 editanything-0.0.5/editanything.egg-info/PKG-INFO
+-rw-r--r--   0 alvin-pc   (501) staff       (20)      268 2023-05-05 10:41:48.000000 editanything-0.0.5/editanything.egg-info/SOURCES.txt
+-rw-r--r--   0 alvin-pc   (501) staff       (20)        1 2023-05-05 10:41:47.000000 editanything-0.0.5/editanything.egg-info/dependency_links.txt
+-rw-r--r--   0 alvin-pc   (501) staff       (20)       44 2023-05-05 10:41:47.000000 editanything-0.0.5/editanything.egg-info/entry_points.txt
+-rw-r--r--   0 alvin-pc   (501) staff       (20)       77 2023-05-05 10:41:47.000000 editanything-0.0.5/editanything.egg-info/requires.txt
+-rw-r--r--   0 alvin-pc   (501) staff       (20)        6 2023-05-05 10:41:47.000000 editanything-0.0.5/editanything.egg-info/top_level.txt
+-rw-r--r--   0 alvin-pc   (501) staff       (20)       38 2023-05-05 10:41:48.062640 editanything-0.0.5/setup.cfg
+-rw-r--r--   0 alvin-pc   (501) staff       (20)      821 2023-05-05 10:41:39.000000 editanything-0.0.5/setup.py
+drwxr-xr-x   0 alvin-pc   (501) staff       (20)        0 2023-05-05 10:41:48.061535 editanything-0.0.5/utils/
+-rw-r--r--   0 alvin-pc   (501) staff       (20)        0 2023-05-05 10:11:42.000000 editanything-0.0.5/utils/__init__.py
+-rw-r--r--   0 alvin-pc   (501) staff       (20)     3118 2023-04-10 10:02:47.000000 editanything-0.0.5/utils/file.py
```

### Comparing `editanything-0.0.4/setup.py` & `editanything-0.0.5/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from setuptools import find_packages, setup
 import utils.file as utils
 
 
 
 setup(
     name='editanything',
-    version='0.0.4',
+    version='0.0.5',
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

### Comparing `editanything-0.0.4/utils/file.py` & `editanything-0.0.5/utils/file.py`

 * *Files identical despite different names*

