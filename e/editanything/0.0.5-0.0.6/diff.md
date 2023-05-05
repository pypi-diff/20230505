# Comparing `tmp/editanything-0.0.5.tar.gz` & `tmp/editanything-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "editanything-0.0.5.tar", last modified: Fri May  5 10:41:48 2023, max compression
+gzip compressed data, was "editanything-0.0.6.tar", last modified: Fri May  5 10:45:55 2023, max compression
```

## Comparing `editanything-0.0.5.tar` & `editanything-0.0.6.tar`

### file list

```diff
@@ -1,15 +1,18 @@
-drwxr-xr-x   0 alvin-pc   (501) staff       (20)        0 2023-05-05 10:41:48.062540 editanything-0.0.5/
--rw-r--r--   0 alvin-pc   (501) staff       (20)      377 2023-05-05 10:41:48.062214 editanything-0.0.5/PKG-INFO
--rw-r--r--   0 alvin-pc   (501) staff       (20)       58 2023-05-05 09:29:16.000000 editanything-0.0.5/README.md
-drwxr-xr-x   0 alvin-pc   (501) staff       (20)        0 2023-05-05 10:41:48.061030 editanything-0.0.5/editanything.egg-info/
--rw-r--r--   0 alvin-pc   (501) staff       (20)      377 2023-05-05 10:41:47.000000 editanything-0.0.5/editanything.egg-info/PKG-INFO
--rw-r--r--   0 alvin-pc   (501) staff       (20)      268 2023-05-05 10:41:48.000000 editanything-0.0.5/editanything.egg-info/SOURCES.txt
--rw-r--r--   0 alvin-pc   (501) staff       (20)        1 2023-05-05 10:41:47.000000 editanything-0.0.5/editanything.egg-info/dependency_links.txt
--rw-r--r--   0 alvin-pc   (501) staff       (20)       44 2023-05-05 10:41:47.000000 editanything-0.0.5/editanything.egg-info/entry_points.txt
--rw-r--r--   0 alvin-pc   (501) staff       (20)       77 2023-05-05 10:41:47.000000 editanything-0.0.5/editanything.egg-info/requires.txt
--rw-r--r--   0 alvin-pc   (501) staff       (20)        6 2023-05-05 10:41:47.000000 editanything-0.0.5/editanything.egg-info/top_level.txt
--rw-r--r--   0 alvin-pc   (501) staff       (20)       38 2023-05-05 10:41:48.062640 editanything-0.0.5/setup.cfg
--rw-r--r--   0 alvin-pc   (501) staff       (20)      821 2023-05-05 10:41:39.000000 editanything-0.0.5/setup.py
-drwxr-xr-x   0 alvin-pc   (501) staff       (20)        0 2023-05-05 10:41:48.061535 editanything-0.0.5/utils/
--rw-r--r--   0 alvin-pc   (501) staff       (20)        0 2023-05-05 10:11:42.000000 editanything-0.0.5/utils/__init__.py
--rw-r--r--   0 alvin-pc   (501) staff       (20)     3118 2023-04-10 10:02:47.000000 editanything-0.0.5/utils/file.py
+drwxr-xr-x   0 alvin-pc   (501) staff       (20)        0 2023-05-05 10:45:55.399985 editanything-0.0.6/
+-rw-r--r--   0 alvin-pc   (501) staff       (20)      377 2023-05-05 10:45:55.399677 editanything-0.0.6/PKG-INFO
+-rw-r--r--   0 alvin-pc   (501) staff       (20)       58 2023-05-05 09:29:16.000000 editanything-0.0.6/README.md
+drwxr-xr-x   0 alvin-pc   (501) staff       (20)        0 2023-05-05 10:45:55.397266 editanything-0.0.6/editanything.egg-info/
+-rw-r--r--   0 alvin-pc   (501) staff       (20)      377 2023-05-05 10:45:55.000000 editanything-0.0.6/editanything.egg-info/PKG-INFO
+-rw-r--r--   0 alvin-pc   (501) staff       (20)      300 2023-05-05 10:45:55.000000 editanything-0.0.6/editanything.egg-info/SOURCES.txt
+-rw-r--r--   0 alvin-pc   (501) staff       (20)        1 2023-05-05 10:45:55.000000 editanything-0.0.6/editanything.egg-info/dependency_links.txt
+-rw-r--r--   0 alvin-pc   (501) staff       (20)       45 2023-05-05 10:45:55.000000 editanything-0.0.6/editanything.egg-info/entry_points.txt
+-rw-r--r--   0 alvin-pc   (501) staff       (20)       77 2023-05-05 10:45:55.000000 editanything-0.0.6/editanything.egg-info/requires.txt
+-rw-r--r--   0 alvin-pc   (501) staff       (20)       12 2023-05-05 10:45:55.000000 editanything-0.0.6/editanything.egg-info/top_level.txt
+drwxr-xr-x   0 alvin-pc   (501) staff       (20)        0 2023-05-05 10:45:55.397928 editanything-0.0.6/entry/
+-rw-r--r--   0 alvin-pc   (501) staff       (20)        0 2023-05-05 10:43:42.000000 editanything-0.0.6/entry/__init__.py
+-rw-r--r--   0 alvin-pc   (501) staff       (20)     1785 2023-05-05 10:30:44.000000 editanything-0.0.6/entry/main.py
+-rw-r--r--   0 alvin-pc   (501) staff       (20)       38 2023-05-05 10:45:55.400095 editanything-0.0.6/setup.cfg
+-rw-r--r--   0 alvin-pc   (501) staff       (20)      822 2023-05-05 10:45:51.000000 editanything-0.0.6/setup.py
+drwxr-xr-x   0 alvin-pc   (501) staff       (20)        0 2023-05-05 10:45:55.398892 editanything-0.0.6/utils/
+-rw-r--r--   0 alvin-pc   (501) staff       (20)        0 2023-05-05 10:11:42.000000 editanything-0.0.6/utils/__init__.py
+-rw-r--r--   0 alvin-pc   (501) staff       (20)     3118 2023-04-10 10:02:47.000000 editanything-0.0.6/utils/file.py
```

### Comparing `editanything-0.0.5/setup.py` & `editanything-0.0.6/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from setuptools import find_packages, setup
 import utils.file as utils
 
 
 
 setup(
     name='editanything',
-    version='0.0.5',
+    version='0.0.6',
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
-              'editanything = main:main'
+              'editanything = entry:main'
           ]
     },
     ext_modules=[],
 )
```

### Comparing `editanything-0.0.5/utils/file.py` & `editanything-0.0.6/utils/file.py`

 * *Files identical despite different names*

