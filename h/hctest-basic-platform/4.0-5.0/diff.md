# Comparing `tmp/hctest_basic_platform-4.0.tar.gz` & `tmp/hctest_basic_platform-5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/hctest_basic_platform-4.0.tar", last modified: Fri May  5 10:52:04 2023, max compression
+gzip compressed data, was "dist/hctest_basic_platform-5.0.tar", last modified: Fri May  5 11:03:25 2023, max compression
```

## Comparing `hctest_basic_platform-4.0.tar` & `hctest_basic_platform-5.0.tar`

### file list

```diff
@@ -1,18 +1,27 @@
-drwxr-xr-x   0 mrding     (501) staff       (20)        0 2023-05-05 10:52:04.225850 hctest_basic_platform-4.0/
--rw-r--r--   0 mrding     (501) staff       (20)      395 2023-05-05 10:52:04.225518 hctest_basic_platform-4.0/PKG-INFO
-drwxr-xr-x   0 mrding     (501) staff       (20)        0 2023-05-05 10:52:04.222988 hctest_basic_platform-4.0/hctest_basic_platform/
--rw-r--r--   0 mrding     (501) staff       (20)      111 2023-05-05 10:31:35.000000 hctest_basic_platform-4.0/hctest_basic_platform/__init__.py
--rw-r--r--   0 mrding     (501) staff       (20)     3130 2023-05-05 09:07:48.000000 hctest_basic_platform-4.0/hctest_basic_platform/app.py
--rw-r--r--   0 mrding     (501) staff       (20)      585 2023-05-04 11:17:40.000000 hctest_basic_platform-4.0/hctest_basic_platform/fontview.py
--rw-r--r--   0 mrding     (501) staff       (20)      325 2023-05-05 10:51:33.000000 hctest_basic_platform-4.0/hctest_basic_platform/main.py
--rw-r--r--   0 mrding     (501) staff       (20)       70 2023-05-04 13:02:32.000000 hctest_basic_platform-4.0/hctest_basic_platform/run.py
--rw-r--r--   0 mrding     (501) staff       (20)     8038 2023-05-05 09:07:48.000000 hctest_basic_platform-4.0/hctest_basic_platform/sql_manage.py
--rw-r--r--   0 mrding     (501) staff       (20)      407 2023-05-04 06:00:45.000000 hctest_basic_platform-4.0/hctest_basic_platform/test_execute.py
-drwxr-xr-x   0 mrding     (501) staff       (20)        0 2023-05-05 10:52:04.225031 hctest_basic_platform-4.0/hctest_basic_platform.egg-info/
--rw-r--r--   0 mrding     (501) staff       (20)      395 2023-05-05 10:52:04.000000 hctest_basic_platform-4.0/hctest_basic_platform.egg-info/PKG-INFO
--rw-r--r--   0 mrding     (501) staff       (20)      462 2023-05-05 10:52:04.000000 hctest_basic_platform-4.0/hctest_basic_platform.egg-info/SOURCES.txt
--rw-r--r--   0 mrding     (501) staff       (20)        1 2023-05-05 10:52:04.000000 hctest_basic_platform-4.0/hctest_basic_platform.egg-info/dependency_links.txt
--rw-r--r--   0 mrding     (501) staff       (20)       55 2023-05-05 10:52:04.000000 hctest_basic_platform-4.0/hctest_basic_platform.egg-info/requires.txt
--rw-r--r--   0 mrding     (501) staff       (20)       22 2023-05-05 10:52:04.000000 hctest_basic_platform-4.0/hctest_basic_platform.egg-info/top_level.txt
--rw-r--r--   0 mrding     (501) staff       (20)       38 2023-05-05 10:52:04.225945 hctest_basic_platform-4.0/setup.cfg
--rw-r--r--   0 mrding     (501) staff       (20)     1106 2023-05-05 10:51:56.000000 hctest_basic_platform-4.0/setup.py
+drwxr-xr-x   0 mrding     (501) staff       (20)        0 2023-05-05 11:03:25.737718 hctest_basic_platform-5.0/
+-rw-r--r--   0 mrding     (501) staff       (20)      395 2023-05-05 11:03:25.737151 hctest_basic_platform-5.0/PKG-INFO
+drwxr-xr-x   0 mrding     (501) staff       (20)        0 2023-05-05 11:03:25.722602 hctest_basic_platform-5.0/hctest_basic_platform/
+-rw-r--r--   0 mrding     (501) staff       (20)      111 2023-05-05 10:31:35.000000 hctest_basic_platform-5.0/hctest_basic_platform/__init__.py
+-rw-r--r--   0 mrding     (501) staff       (20)     3130 2023-05-05 09:07:48.000000 hctest_basic_platform-5.0/hctest_basic_platform/app.py
+-rw-r--r--   0 mrding     (501) staff       (20)      585 2023-05-04 11:17:40.000000 hctest_basic_platform-5.0/hctest_basic_platform/fontview.py
+drwxr-xr-x   0 mrding     (501) staff       (20)        0 2023-05-05 11:03:25.728906 hctest_basic_platform-5.0/hctest_basic_platform/layui/
+-rw-r--r--   0 mrding     (501) staff       (20)    82241 2023-05-04 06:00:45.000000 hctest_basic_platform-5.0/hctest_basic_platform/layui/layui.css
+-rw-r--r--   0 mrding     (501) staff       (20)   291146 2023-05-04 06:00:45.000000 hctest_basic_platform-5.0/hctest_basic_platform/layui/layui.js
+-rw-r--r--   0 mrding     (501) staff       (20)      325 2023-05-05 10:51:33.000000 hctest_basic_platform-5.0/hctest_basic_platform/main.py
+-rw-r--r--   0 mrding     (501) staff       (20)       70 2023-05-04 13:02:32.000000 hctest_basic_platform-5.0/hctest_basic_platform/run.py
+-rw-r--r--   0 mrding     (501) staff       (20)     8038 2023-05-05 09:07:48.000000 hctest_basic_platform-5.0/hctest_basic_platform/sql_manage.py
+drwxr-xr-x   0 mrding     (501) staff       (20)        0 2023-05-05 11:03:25.736080 hctest_basic_platform-5.0/hctest_basic_platform/templates/
+-rw-r--r--   0 mrding     (501) staff       (20)     6620 2023-05-05 10:26:02.000000 hctest_basic_platform-5.0/hctest_basic_platform/templates/addTestCase.html
+-rw-r--r--   0 mrding     (501) staff       (20)     4486 2023-05-04 11:15:51.000000 hctest_basic_platform-5.0/hctest_basic_platform/templates/caseList.html
+-rw-r--r--   0 mrding     (501) staff       (20)     2176 2023-05-04 06:00:45.000000 hctest_basic_platform-5.0/hctest_basic_platform/templates/index.html
+-rw-r--r--   0 mrding     (501) staff       (20)     4493 2023-05-04 06:00:45.000000 hctest_basic_platform-5.0/hctest_basic_platform/templates/test.html
+-rw-r--r--   0 mrding     (501) staff       (20)     7614 2023-05-04 06:00:45.000000 hctest_basic_platform-5.0/hctest_basic_platform/templates/updateTestCase.html
+-rw-r--r--   0 mrding     (501) staff       (20)      407 2023-05-04 06:00:45.000000 hctest_basic_platform-5.0/hctest_basic_platform/test_execute.py
+drwxr-xr-x   0 mrding     (501) staff       (20)        0 2023-05-05 11:03:25.726441 hctest_basic_platform-5.0/hctest_basic_platform.egg-info/
+-rw-r--r--   0 mrding     (501) staff       (20)      395 2023-05-05 11:03:25.000000 hctest_basic_platform-5.0/hctest_basic_platform.egg-info/PKG-INFO
+-rw-r--r--   0 mrding     (501) staff       (20)      769 2023-05-05 11:03:25.000000 hctest_basic_platform-5.0/hctest_basic_platform.egg-info/SOURCES.txt
+-rw-r--r--   0 mrding     (501) staff       (20)        1 2023-05-05 11:03:25.000000 hctest_basic_platform-5.0/hctest_basic_platform.egg-info/dependency_links.txt
+-rw-r--r--   0 mrding     (501) staff       (20)       55 2023-05-05 11:03:25.000000 hctest_basic_platform-5.0/hctest_basic_platform.egg-info/requires.txt
+-rw-r--r--   0 mrding     (501) staff       (20)       22 2023-05-05 11:03:25.000000 hctest_basic_platform-5.0/hctest_basic_platform.egg-info/top_level.txt
+-rw-r--r--   0 mrding     (501) staff       (20)       38 2023-05-05 11:03:25.737933 hctest_basic_platform-5.0/setup.cfg
+-rw-r--r--   0 mrding     (501) staff       (20)     1193 2023-05-05 11:03:23.000000 hctest_basic_platform-5.0/setup.py
```

### Comparing `hctest_basic_platform-4.0/hctest_basic_platform/app.py` & `hctest_basic_platform-5.0/hctest_basic_platform/app.py`

 * *Files identical despite different names*

### Comparing `hctest_basic_platform-4.0/hctest_basic_platform/fontview.py` & `hctest_basic_platform-5.0/hctest_basic_platform/fontview.py`

 * *Files identical despite different names*

### Comparing `hctest_basic_platform-4.0/hctest_basic_platform/sql_manage.py` & `hctest_basic_platform-5.0/hctest_basic_platform/sql_manage.py`

 * *Files identical despite different names*

### Comparing `hctest_basic_platform-4.0/setup.py` & `hctest_basic_platform-5.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,24 +1,28 @@
 # -*- coding: utf-8 -*-
 # author: 华测-长风老师
 # file name：setup.py
-from setuptools import setup, find_packages
 """
 python3 setup.py sdist bdist_wheel
 python3 -m twine upload dist/*
 Could not find 'apksigner.jar' in ["C:\\Users\\wxy\\SDK\\platform-tools\\apksigner.jar","C:\\Users\\wxy\\SDK\\emulator\\apksigner.jar","C:\\Users\\wxy\\SDK\\cmdline-tools\\latest\\bin\\apksigner.jar","C:\\Users\\wxy\\SDK\\tools\\apksigner.jar","C:\\Users\\wxy\\SDK\\tools\\bin\\apksigner.jar","C:\\Users\\wxy\\SDK\\apksigner.jar"]
 """
+from setuptools import setup, find_packages
+
 setup(
     name="hctest_basic_platform",
-    version="4.0",
+    version="5.0",
     description="初级平台",
     author="cf",
     author_email="dingjun_baby@yeah.net",
     url="https://github.com/pypa/sampleproject",
     packages=find_packages(),
+    package_data={
+        'hctest_basic_platform': ['layui/*','templates/*'],
+    },
     install_requires=[
         "Flask",
         "Flask-Cors",
         "PyMySQL",
         "pytest",
         "requests",
         "allure-pytest",
```

