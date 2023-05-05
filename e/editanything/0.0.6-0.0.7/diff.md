# Comparing `tmp/editanything-0.0.6.tar.gz` & `tmp/editanything-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "editanything-0.0.6.tar", last modified: Fri May  5 10:45:55 2023, max compression
+gzip compressed data, was "editanything-0.0.7.tar", last modified: Fri May  5 10:52:23 2023, max compression
```

## Comparing `editanything-0.0.6.tar` & `editanything-0.0.7.tar`

### file list

```diff
@@ -1,18 +1,43 @@
-drwxr-xr-x   0 alvin-pc   (501) staff       (20)        0 2023-05-05 10:45:55.399985 editanything-0.0.6/
--rw-r--r--   0 alvin-pc   (501) staff       (20)      377 2023-05-05 10:45:55.399677 editanything-0.0.6/PKG-INFO
--rw-r--r--   0 alvin-pc   (501) staff       (20)       58 2023-05-05 09:29:16.000000 editanything-0.0.6/README.md
-drwxr-xr-x   0 alvin-pc   (501) staff       (20)        0 2023-05-05 10:45:55.397266 editanything-0.0.6/editanything.egg-info/
--rw-r--r--   0 alvin-pc   (501) staff       (20)      377 2023-05-05 10:45:55.000000 editanything-0.0.6/editanything.egg-info/PKG-INFO
--rw-r--r--   0 alvin-pc   (501) staff       (20)      300 2023-05-05 10:45:55.000000 editanything-0.0.6/editanything.egg-info/SOURCES.txt
--rw-r--r--   0 alvin-pc   (501) staff       (20)        1 2023-05-05 10:45:55.000000 editanything-0.0.6/editanything.egg-info/dependency_links.txt
--rw-r--r--   0 alvin-pc   (501) staff       (20)       45 2023-05-05 10:45:55.000000 editanything-0.0.6/editanything.egg-info/entry_points.txt
--rw-r--r--   0 alvin-pc   (501) staff       (20)       77 2023-05-05 10:45:55.000000 editanything-0.0.6/editanything.egg-info/requires.txt
--rw-r--r--   0 alvin-pc   (501) staff       (20)       12 2023-05-05 10:45:55.000000 editanything-0.0.6/editanything.egg-info/top_level.txt
-drwxr-xr-x   0 alvin-pc   (501) staff       (20)        0 2023-05-05 10:45:55.397928 editanything-0.0.6/entry/
--rw-r--r--   0 alvin-pc   (501) staff       (20)        0 2023-05-05 10:43:42.000000 editanything-0.0.6/entry/__init__.py
--rw-r--r--   0 alvin-pc   (501) staff       (20)     1785 2023-05-05 10:30:44.000000 editanything-0.0.6/entry/main.py
--rw-r--r--   0 alvin-pc   (501) staff       (20)       38 2023-05-05 10:45:55.400095 editanything-0.0.6/setup.cfg
--rw-r--r--   0 alvin-pc   (501) staff       (20)      822 2023-05-05 10:45:51.000000 editanything-0.0.6/setup.py
-drwxr-xr-x   0 alvin-pc   (501) staff       (20)        0 2023-05-05 10:45:55.398892 editanything-0.0.6/utils/
--rw-r--r--   0 alvin-pc   (501) staff       (20)        0 2023-05-05 10:11:42.000000 editanything-0.0.6/utils/__init__.py
--rw-r--r--   0 alvin-pc   (501) staff       (20)     3118 2023-04-10 10:02:47.000000 editanything-0.0.6/utils/file.py
+drwxr-xr-x   0 alvin-pc   (501) staff       (20)        0 2023-05-05 10:52:23.313559 editanything-0.0.7/
+-rw-r--r--   0 alvin-pc   (501) staff       (20)      377 2023-05-05 10:52:23.313018 editanything-0.0.7/PKG-INFO
+-rw-r--r--   0 alvin-pc   (501) staff       (20)       58 2023-05-05 09:29:16.000000 editanything-0.0.7/README.md
+drwxr-xr-x   0 alvin-pc   (501) staff       (20)        0 2023-05-05 10:52:23.300487 editanything-0.0.7/backend/
+-rw-r--r--   0 alvin-pc   (501) staff       (20)        0 2023-05-04 08:28:56.000000 editanything-0.0.7/backend/__init__.py
+drwxr-xr-x   0 alvin-pc   (501) staff       (20)        0 2023-05-05 10:52:23.300904 editanything-0.0.7/backend/constant/
+-rw-r--r--   0 alvin-pc   (501) staff       (20)        0 2023-05-04 08:28:56.000000 editanything-0.0.7/backend/constant/__init__.py
+-rw-r--r--   0 alvin-pc   (501) staff       (20)        0 2023-05-05 09:29:16.000000 editanything-0.0.7/backend/constant/biz_constants.py
+drwxr-xr-x   0 alvin-pc   (501) staff       (20)        0 2023-05-05 10:52:23.301109 editanything-0.0.7/backend/domain/
+-rw-r--r--   0 alvin-pc   (501) staff       (20)        0 2023-05-04 08:28:56.000000 editanything-0.0.7/backend/domain/__init__.py
+drwxr-xr-x   0 alvin-pc   (501) staff       (20)        0 2023-05-05 10:52:23.302869 editanything-0.0.7/backend/domain/dto/
+-rw-r--r--   0 alvin-pc   (501) staff       (20)        0 2023-05-04 08:28:56.000000 editanything-0.0.7/backend/domain/dto/__init__.py
+-rw-r--r--   0 alvin-pc   (501) staff       (20)      112 2023-05-05 09:29:16.000000 editanything-0.0.7/backend/domain/dto/req_classes.py
+-rw-r--r--   0 alvin-pc   (501) staff       (20)      124 2023-05-05 09:29:16.000000 editanything-0.0.7/backend/domain/dto/rsp_classes.py
+drwxr-xr-x   0 alvin-pc   (501) staff       (20)        0 2023-05-05 10:52:23.303755 editanything-0.0.7/backend/exception/
+-rw-r--r--   0 alvin-pc   (501) staff       (20)        0 2023-05-04 08:28:56.000000 editanything-0.0.7/backend/exception/__init__.py
+-rw-r--r--   0 alvin-pc   (501) staff       (20)     1221 2023-05-05 09:29:16.000000 editanything-0.0.7/backend/exception/exceptions.py
+drwxr-xr-x   0 alvin-pc   (501) staff       (20)        0 2023-05-05 10:52:23.304776 editanything-0.0.7/backend/inference/
+-rw-r--r--   0 alvin-pc   (501) staff       (20)        0 2023-05-04 08:28:56.000000 editanything-0.0.7/backend/inference/__init__.py
+-rw-r--r--   0 alvin-pc   (501) staff       (20)      158 2023-05-05 09:29:16.000000 editanything-0.0.7/backend/inference/inference.py
+drwxr-xr-x   0 alvin-pc   (501) staff       (20)        0 2023-05-05 10:52:23.305671 editanything-0.0.7/backend/process/
+-rw-r--r--   0 alvin-pc   (501) staff       (20)        0 2023-05-04 08:28:56.000000 editanything-0.0.7/backend/process/__init__.py
+-rw-r--r--   0 alvin-pc   (501) staff       (20)       65 2023-05-05 09:29:16.000000 editanything-0.0.7/backend/process/cv_process.py
+drwxr-xr-x   0 alvin-pc   (501) staff       (20)        0 2023-05-05 10:52:23.306572 editanything-0.0.7/backend/util/
+-rw-r--r--   0 alvin-pc   (501) staff       (20)        0 2023-05-04 08:28:56.000000 editanything-0.0.7/backend/util/__init__.py
+-rw-r--r--   0 alvin-pc   (501) staff       (20)      901 2023-05-05 09:29:16.000000 editanything-0.0.7/backend/util/str_utils.py
+drwxr-xr-x   0 alvin-pc   (501) staff       (20)        0 2023-05-05 10:52:23.309212 editanything-0.0.7/editanything.egg-info/
+-rw-r--r--   0 alvin-pc   (501) staff       (20)      377 2023-05-05 10:52:23.000000 editanything-0.0.7/editanything.egg-info/PKG-INFO
+-rw-r--r--   0 alvin-pc   (501) staff       (20)      762 2023-05-05 10:52:23.000000 editanything-0.0.7/editanything.egg-info/SOURCES.txt
+-rw-r--r--   0 alvin-pc   (501) staff       (20)        1 2023-05-05 10:52:23.000000 editanything-0.0.7/editanything.egg-info/dependency_links.txt
+-rw-r--r--   0 alvin-pc   (501) staff       (20)       45 2023-05-05 10:52:23.000000 editanything-0.0.7/editanything.egg-info/entry_points.txt
+-rw-r--r--   0 alvin-pc   (501) staff       (20)       77 2023-05-05 10:52:23.000000 editanything-0.0.7/editanything.egg-info/requires.txt
+-rw-r--r--   0 alvin-pc   (501) staff       (20)       35 2023-05-05 10:52:23.000000 editanything-0.0.7/editanything.egg-info/top_level.txt
+drwxr-xr-x   0 alvin-pc   (501) staff       (20)        0 2023-05-05 10:52:23.309980 editanything-0.0.7/entry/
+-rw-r--r--   0 alvin-pc   (501) staff       (20)        0 2023-05-05 10:43:42.000000 editanything-0.0.7/entry/__init__.py
+-rw-r--r--   0 alvin-pc   (501) staff       (20)     1785 2023-05-05 10:30:44.000000 editanything-0.0.7/entry/main.py
+drwxr-xr-x   0 alvin-pc   (501) staff       (20)        0 2023-05-05 10:52:23.311037 editanything-0.0.7/frontend/
+-rw-r--r--   0 alvin-pc   (501) staff       (20)        0 2023-05-04 08:28:56.000000 editanything-0.0.7/frontend/__init__.py
+-rw-r--r--   0 alvin-pc   (501) staff       (20)       38 2023-05-05 10:52:23.313720 editanything-0.0.7/setup.cfg
+-rw-r--r--   0 alvin-pc   (501) staff       (20)      822 2023-05-05 10:52:12.000000 editanything-0.0.7/setup.py
+drwxr-xr-x   0 alvin-pc   (501) staff       (20)        0 2023-05-05 10:52:23.311903 editanything-0.0.7/utils/
+-rw-r--r--   0 alvin-pc   (501) staff       (20)        0 2023-05-05 10:11:42.000000 editanything-0.0.7/utils/__init__.py
+-rw-r--r--   0 alvin-pc   (501) staff       (20)     3118 2023-04-10 10:02:47.000000 editanything-0.0.7/utils/file.py
```

### Comparing `editanything-0.0.6/entry/main.py` & `editanything-0.0.7/entry/main.py`

 * *Files identical despite different names*

### Comparing `editanything-0.0.6/setup.py` & `editanything-0.0.7/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from setuptools import find_packages, setup
 import utils.file as utils
 
 
 
 setup(
     name='editanything',
-    version='0.0.6',
+    version='0.0.7',
     description='EditAnything',
     long_description=utils.get_file_content("README.md"),
     long_description_content_type='text/markdown',
     author='wfbi',
     author_email='myname@example.com',
     keywords='EditAnything',
     url='https://github.com/xxx/xxxx',
```

### Comparing `editanything-0.0.6/utils/file.py` & `editanything-0.0.7/utils/file.py`

 * *Files identical despite different names*

