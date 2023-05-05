# Comparing `tmp/hctest_basic_platform-3.0.tar.gz` & `tmp/hctest_basic_platform-4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/hctest_basic_platform-3.0.tar", last modified: Fri May  5 10:43:09 2023, max compression
+gzip compressed data, was "dist/hctest_basic_platform-4.0.tar", last modified: Fri May  5 10:52:04 2023, max compression
```

## Comparing `hctest_basic_platform-3.0.tar` & `hctest_basic_platform-4.0.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 mrding     (501) staff       (20)        0 2023-05-05 10:43:09.236269 hctest_basic_platform-3.0/
--rw-r--r--   0 mrding     (501) staff       (20)      395 2023-05-05 10:43:09.235599 hctest_basic_platform-3.0/PKG-INFO
-drwxr-xr-x   0 mrding     (501) staff       (20)        0 2023-05-05 10:43:09.231758 hctest_basic_platform-3.0/hctest_basic_platform/
--rw-r--r--   0 mrding     (501) staff       (20)      111 2023-05-05 10:31:35.000000 hctest_basic_platform-3.0/hctest_basic_platform/__init__.py
--rw-r--r--   0 mrding     (501) staff       (20)     3130 2023-05-05 09:07:48.000000 hctest_basic_platform-3.0/hctest_basic_platform/app.py
--rw-r--r--   0 mrding     (501) staff       (20)      585 2023-05-04 11:17:40.000000 hctest_basic_platform-3.0/hctest_basic_platform/fontview.py
--rw-r--r--   0 mrding     (501) staff       (20)      328 2023-05-05 08:42:21.000000 hctest_basic_platform-3.0/hctest_basic_platform/main.py
--rw-r--r--   0 mrding     (501) staff       (20)       70 2023-05-04 13:02:32.000000 hctest_basic_platform-3.0/hctest_basic_platform/run.py
--rw-r--r--   0 mrding     (501) staff       (20)     8038 2023-05-05 09:07:48.000000 hctest_basic_platform-3.0/hctest_basic_platform/sql_manage.py
--rw-r--r--   0 mrding     (501) staff       (20)      407 2023-05-04 06:00:45.000000 hctest_basic_platform-3.0/hctest_basic_platform/test_execute.py
-drwxr-xr-x   0 mrding     (501) staff       (20)        0 2023-05-05 10:43:09.234740 hctest_basic_platform-3.0/hctest_basic_platform.egg-info/
--rw-r--r--   0 mrding     (501) staff       (20)      395 2023-05-05 10:43:09.000000 hctest_basic_platform-3.0/hctest_basic_platform.egg-info/PKG-INFO
--rw-r--r--   0 mrding     (501) staff       (20)      462 2023-05-05 10:43:09.000000 hctest_basic_platform-3.0/hctest_basic_platform.egg-info/SOURCES.txt
--rw-r--r--   0 mrding     (501) staff       (20)        1 2023-05-05 10:43:09.000000 hctest_basic_platform-3.0/hctest_basic_platform.egg-info/dependency_links.txt
--rw-r--r--   0 mrding     (501) staff       (20)       55 2023-05-05 10:43:09.000000 hctest_basic_platform-3.0/hctest_basic_platform.egg-info/requires.txt
--rw-r--r--   0 mrding     (501) staff       (20)       22 2023-05-05 10:43:09.000000 hctest_basic_platform-3.0/hctest_basic_platform.egg-info/top_level.txt
--rw-r--r--   0 mrding     (501) staff       (20)       38 2023-05-05 10:43:09.236421 hctest_basic_platform-3.0/setup.cfg
--rw-r--r--   0 mrding     (501) staff       (20)     1106 2023-05-05 10:43:07.000000 hctest_basic_platform-3.0/setup.py
+drwxr-xr-x   0 mrding     (501) staff       (20)        0 2023-05-05 10:52:04.225850 hctest_basic_platform-4.0/
+-rw-r--r--   0 mrding     (501) staff       (20)      395 2023-05-05 10:52:04.225518 hctest_basic_platform-4.0/PKG-INFO
+drwxr-xr-x   0 mrding     (501) staff       (20)        0 2023-05-05 10:52:04.222988 hctest_basic_platform-4.0/hctest_basic_platform/
+-rw-r--r--   0 mrding     (501) staff       (20)      111 2023-05-05 10:31:35.000000 hctest_basic_platform-4.0/hctest_basic_platform/__init__.py
+-rw-r--r--   0 mrding     (501) staff       (20)     3130 2023-05-05 09:07:48.000000 hctest_basic_platform-4.0/hctest_basic_platform/app.py
+-rw-r--r--   0 mrding     (501) staff       (20)      585 2023-05-04 11:17:40.000000 hctest_basic_platform-4.0/hctest_basic_platform/fontview.py
+-rw-r--r--   0 mrding     (501) staff       (20)      325 2023-05-05 10:51:33.000000 hctest_basic_platform-4.0/hctest_basic_platform/main.py
+-rw-r--r--   0 mrding     (501) staff       (20)       70 2023-05-04 13:02:32.000000 hctest_basic_platform-4.0/hctest_basic_platform/run.py
+-rw-r--r--   0 mrding     (501) staff       (20)     8038 2023-05-05 09:07:48.000000 hctest_basic_platform-4.0/hctest_basic_platform/sql_manage.py
+-rw-r--r--   0 mrding     (501) staff       (20)      407 2023-05-04 06:00:45.000000 hctest_basic_platform-4.0/hctest_basic_platform/test_execute.py
+drwxr-xr-x   0 mrding     (501) staff       (20)        0 2023-05-05 10:52:04.225031 hctest_basic_platform-4.0/hctest_basic_platform.egg-info/
+-rw-r--r--   0 mrding     (501) staff       (20)      395 2023-05-05 10:52:04.000000 hctest_basic_platform-4.0/hctest_basic_platform.egg-info/PKG-INFO
+-rw-r--r--   0 mrding     (501) staff       (20)      462 2023-05-05 10:52:04.000000 hctest_basic_platform-4.0/hctest_basic_platform.egg-info/SOURCES.txt
+-rw-r--r--   0 mrding     (501) staff       (20)        1 2023-05-05 10:52:04.000000 hctest_basic_platform-4.0/hctest_basic_platform.egg-info/dependency_links.txt
+-rw-r--r--   0 mrding     (501) staff       (20)       55 2023-05-05 10:52:04.000000 hctest_basic_platform-4.0/hctest_basic_platform.egg-info/requires.txt
+-rw-r--r--   0 mrding     (501) staff       (20)       22 2023-05-05 10:52:04.000000 hctest_basic_platform-4.0/hctest_basic_platform.egg-info/top_level.txt
+-rw-r--r--   0 mrding     (501) staff       (20)       38 2023-05-05 10:52:04.225945 hctest_basic_platform-4.0/setup.cfg
+-rw-r--r--   0 mrding     (501) staff       (20)     1106 2023-05-05 10:51:56.000000 hctest_basic_platform-4.0/setup.py
```

### Comparing `hctest_basic_platform-3.0/hctest_basic_platform/app.py` & `hctest_basic_platform-4.0/hctest_basic_platform/app.py`

 * *Files identical despite different names*

### Comparing `hctest_basic_platform-3.0/hctest_basic_platform/fontview.py` & `hctest_basic_platform-4.0/hctest_basic_platform/fontview.py`

 * *Files identical despite different names*

### Comparing `hctest_basic_platform-3.0/hctest_basic_platform/sql_manage.py` & `hctest_basic_platform-4.0/hctest_basic_platform/sql_manage.py`

 * *Files identical despite different names*

### Comparing `hctest_basic_platform-3.0/setup.py` & `hctest_basic_platform-4.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 """
 python3 setup.py sdist bdist_wheel
 python3 -m twine upload dist/*
 Could not find 'apksigner.jar' in ["C:\\Users\\wxy\\SDK\\platform-tools\\apksigner.jar","C:\\Users\\wxy\\SDK\\emulator\\apksigner.jar","C:\\Users\\wxy\\SDK\\cmdline-tools\\latest\\bin\\apksigner.jar","C:\\Users\\wxy\\SDK\\tools\\apksigner.jar","C:\\Users\\wxy\\SDK\\tools\\bin\\apksigner.jar","C:\\Users\\wxy\\SDK\\apksigner.jar"]
 """
 setup(
     name="hctest_basic_platform",
-    version="3.0",
+    version="4.0",
     description="初级平台",
     author="cf",
     author_email="dingjun_baby@yeah.net",
     url="https://github.com/pypa/sampleproject",
     packages=find_packages(),
     install_requires=[
         "Flask",
```

