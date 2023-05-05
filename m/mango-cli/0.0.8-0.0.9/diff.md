# Comparing `tmp/mango-cli-0.0.8.tar.gz` & `tmp/mango-cli-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mango-cli-0.0.8.tar", last modified: Fri May  5 19:13:22 2023, max compression
+gzip compressed data, was "mango-cli-0.0.9.tar", last modified: Fri May  5 19:14:37 2023, max compression
```

## Comparing `mango-cli-0.0.8.tar` & `mango-cli-0.0.9.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxr-xr-x   0 mangosoft   (502) staff       (20)        0 2023-05-05 19:13:22.042056 mango-cli-0.0.8/
--rw-r--r--   0 mangosoft   (502) staff       (20)      138 2023-05-05 19:13:22.041841 mango-cli-0.0.8/PKG-INFO
-drwxr-xr-x   0 mangosoft   (502) staff       (20)        0 2023-05-05 19:13:22.041418 mango-cli-0.0.8/mango_cli.egg-info/
--rw-r--r--   0 mangosoft   (502) staff       (20)      138 2023-05-05 19:13:22.000000 mango-cli-0.0.8/mango_cli.egg-info/PKG-INFO
--rw-r--r--   0 mangosoft   (502) staff       (20)      208 2023-05-05 19:13:22.000000 mango-cli-0.0.8/mango_cli.egg-info/SOURCES.txt
--rw-r--r--   0 mangosoft   (502) staff       (20)        1 2023-05-05 19:13:22.000000 mango-cli-0.0.8/mango_cli.egg-info/dependency_links.txt
--rw-r--r--   0 mangosoft   (502) staff       (20)       46 2023-05-05 19:13:22.000000 mango-cli-0.0.8/mango_cli.egg-info/entry_points.txt
--rw-r--r--   0 mangosoft   (502) staff       (20)      670 2023-05-05 19:13:22.000000 mango-cli-0.0.8/mango_cli.egg-info/requires.txt
--rw-r--r--   0 mangosoft   (502) staff       (20)        4 2023-05-05 19:13:22.000000 mango-cli-0.0.8/mango_cli.egg-info/top_level.txt
--rw-r--r--   0 mangosoft   (502) staff       (20)       38 2023-05-05 19:13:22.042135 mango-cli-0.0.8/setup.cfg
--rw-r--r--   0 mangosoft   (502) staff       (20)      533 2023-05-05 19:13:20.000000 mango-cli-0.0.8/setup.py
+drwxr-xr-x   0 mangosoft   (502) staff       (20)        0 2023-05-05 19:14:37.130789 mango-cli-0.0.9/
+-rw-r--r--   0 mangosoft   (502) staff       (20)      138 2023-05-05 19:14:37.130628 mango-cli-0.0.9/PKG-INFO
+drwxr-xr-x   0 mangosoft   (502) staff       (20)        0 2023-05-05 19:14:37.130350 mango-cli-0.0.9/mango_cli.egg-info/
+-rw-r--r--   0 mangosoft   (502) staff       (20)      138 2023-05-05 19:14:37.000000 mango-cli-0.0.9/mango_cli.egg-info/PKG-INFO
+-rw-r--r--   0 mangosoft   (502) staff       (20)      208 2023-05-05 19:14:37.000000 mango-cli-0.0.9/mango_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 mangosoft   (502) staff       (20)        1 2023-05-05 19:14:37.000000 mango-cli-0.0.9/mango_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 mangosoft   (502) staff       (20)       47 2023-05-05 19:14:37.000000 mango-cli-0.0.9/mango_cli.egg-info/entry_points.txt
+-rw-r--r--   0 mangosoft   (502) staff       (20)      670 2023-05-05 19:14:37.000000 mango-cli-0.0.9/mango_cli.egg-info/requires.txt
+-rw-r--r--   0 mangosoft   (502) staff       (20)        4 2023-05-05 19:14:37.000000 mango-cli-0.0.9/mango_cli.egg-info/top_level.txt
+-rw-r--r--   0 mangosoft   (502) staff       (20)       38 2023-05-05 19:14:37.130850 mango-cli-0.0.9/setup.cfg
+-rw-r--r--   0 mangosoft   (502) staff       (20)      534 2023-05-05 19:14:35.000000 mango-cli-0.0.9/setup.py
```

### Comparing `mango-cli-0.0.8/mango_cli.egg-info/requires.txt` & `mango-cli-0.0.9/mango_cli.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `mango-cli-0.0.8/setup.py` & `mango-cli-0.0.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 from setuptools import setup, find_packages
 with open("requirements.txt", "r", encoding="utf-8") as fh:
     requirements = fh.read()
 setup(
     name='mango-cli',
-    version='0.0.8',
+    version='0.0.9',
     packages=find_packages(),
     include_package_data=True,
     author='Mangosoft',
     author_email="wilson.mendoza@mango-soft.com",
     description="Mangosoft CLI",
     py_modules=["app"],
     include_dirs=["app"],
     install_requires=[requirements],
     entry_points='''
         [console_scripts]
-        mango=app.application:cli
+        mango=.app.application:cli
     '''
 )
```

