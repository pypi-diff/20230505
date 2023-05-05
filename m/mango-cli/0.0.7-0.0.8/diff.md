# Comparing `tmp/mango-cli-0.0.7.tar.gz` & `tmp/mango-cli-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mango-cli-0.0.7.tar", last modified: Fri May  5 17:38:32 2023, max compression
+gzip compressed data, was "mango-cli-0.0.8.tar", last modified: Fri May  5 19:13:22 2023, max compression
```

## Comparing `mango-cli-0.0.7.tar` & `mango-cli-0.0.8.tar`

### file list

```diff
@@ -1,20 +1,11 @@
-drwxr-xr-x   0 mangosoft   (502) staff       (20)        0 2023-05-05 17:38:32.926502 mango-cli-0.0.7/
--rw-r--r--   0 mangosoft   (502) staff       (20)      138 2023-05-05 17:38:32.926311 mango-cli-0.0.7/PKG-INFO
-drwxr-xr-x   0 mangosoft   (502) staff       (20)        0 2023-05-05 17:38:32.923675 mango-cli-0.0.7/app/
--rw-r--r--   0 mangosoft   (502) staff       (20)        0 2023-05-05 16:44:26.000000 mango-cli-0.0.7/app/__init__.py
--rw-r--r--   0 mangosoft   (502) staff       (20)      242 2023-05-05 17:22:31.000000 mango-cli-0.0.7/app/application.py
-drwxr-xr-x   0 mangosoft   (502) staff       (20)        0 2023-05-05 17:38:32.924019 mango-cli-0.0.7/app/handlers/
--rw-r--r--   0 mangosoft   (502) staff       (20)        0 2023-05-05 17:02:52.000000 mango-cli-0.0.7/app/handlers/__init__.py
--rw-r--r--   0 mangosoft   (502) staff       (20)      810 2023-05-05 17:23:15.000000 mango-cli-0.0.7/app/handlers/download_data.py
-drwxr-xr-x   0 mangosoft   (502) staff       (20)        0 2023-05-05 17:38:32.924379 mango-cli-0.0.7/app/services/
--rw-r--r--   0 mangosoft   (502) staff       (20)        0 2023-05-05 17:02:52.000000 mango-cli-0.0.7/app/services/__init__.py
--rw-r--r--   0 mangosoft   (502) staff       (20)      735 2023-05-05 16:39:20.000000 mango-cli-0.0.7/app/services/data.py
-drwxr-xr-x   0 mangosoft   (502) staff       (20)        0 2023-05-05 17:38:32.925949 mango-cli-0.0.7/mango_cli.egg-info/
--rw-r--r--   0 mangosoft   (502) staff       (20)      138 2023-05-05 17:38:32.000000 mango-cli-0.0.7/mango_cli.egg-info/PKG-INFO
--rw-r--r--   0 mangosoft   (502) staff       (20)      344 2023-05-05 17:38:32.000000 mango-cli-0.0.7/mango_cli.egg-info/SOURCES.txt
--rw-r--r--   0 mangosoft   (502) staff       (20)        1 2023-05-05 17:38:32.000000 mango-cli-0.0.7/mango_cli.egg-info/dependency_links.txt
--rw-r--r--   0 mangosoft   (502) staff       (20)       46 2023-05-05 17:38:32.000000 mango-cli-0.0.7/mango_cli.egg-info/entry_points.txt
--rw-r--r--   0 mangosoft   (502) staff       (20)      670 2023-05-05 17:38:32.000000 mango-cli-0.0.7/mango_cli.egg-info/requires.txt
--rw-r--r--   0 mangosoft   (502) staff       (20)        4 2023-05-05 17:38:32.000000 mango-cli-0.0.7/mango_cli.egg-info/top_level.txt
--rw-r--r--   0 mangosoft   (502) staff       (20)       38 2023-05-05 17:38:32.926567 mango-cli-0.0.7/setup.cfg
--rw-r--r--   0 mangosoft   (502) staff       (20)      533 2023-05-05 17:38:31.000000 mango-cli-0.0.7/setup.py
+drwxr-xr-x   0 mangosoft   (502) staff       (20)        0 2023-05-05 19:13:22.042056 mango-cli-0.0.8/
+-rw-r--r--   0 mangosoft   (502) staff       (20)      138 2023-05-05 19:13:22.041841 mango-cli-0.0.8/PKG-INFO
+drwxr-xr-x   0 mangosoft   (502) staff       (20)        0 2023-05-05 19:13:22.041418 mango-cli-0.0.8/mango_cli.egg-info/
+-rw-r--r--   0 mangosoft   (502) staff       (20)      138 2023-05-05 19:13:22.000000 mango-cli-0.0.8/mango_cli.egg-info/PKG-INFO
+-rw-r--r--   0 mangosoft   (502) staff       (20)      208 2023-05-05 19:13:22.000000 mango-cli-0.0.8/mango_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 mangosoft   (502) staff       (20)        1 2023-05-05 19:13:22.000000 mango-cli-0.0.8/mango_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 mangosoft   (502) staff       (20)       46 2023-05-05 19:13:22.000000 mango-cli-0.0.8/mango_cli.egg-info/entry_points.txt
+-rw-r--r--   0 mangosoft   (502) staff       (20)      670 2023-05-05 19:13:22.000000 mango-cli-0.0.8/mango_cli.egg-info/requires.txt
+-rw-r--r--   0 mangosoft   (502) staff       (20)        4 2023-05-05 19:13:22.000000 mango-cli-0.0.8/mango_cli.egg-info/top_level.txt
+-rw-r--r--   0 mangosoft   (502) staff       (20)       38 2023-05-05 19:13:22.042135 mango-cli-0.0.8/setup.cfg
+-rw-r--r--   0 mangosoft   (502) staff       (20)      533 2023-05-05 19:13:20.000000 mango-cli-0.0.8/setup.py
```

### Comparing `mango-cli-0.0.7/mango_cli.egg-info/requires.txt` & `mango-cli-0.0.8/mango_cli.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `mango-cli-0.0.7/setup.py` & `mango-cli-0.0.8/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 with open("requirements.txt", "r", encoding="utf-8") as fh:
     requirements = fh.read()
 setup(
     name='mango-cli',
-    version='0.0.7',
+    version='0.0.8',
     packages=find_packages(),
     include_package_data=True,
     author='Mangosoft',
     author_email="wilson.mendoza@mango-soft.com",
     description="Mangosoft CLI",
     py_modules=["app"],
     include_dirs=["app"],
```

