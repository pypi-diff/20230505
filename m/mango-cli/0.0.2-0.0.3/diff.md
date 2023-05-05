# Comparing `tmp/mango-cli-0.0.2.tar.gz` & `tmp/mango-cli-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mango-cli-0.0.2.tar", last modified: Fri May  5 17:06:33 2023, max compression
+gzip compressed data, was "mango-cli-0.0.3.tar", last modified: Fri May  5 17:12:26 2023, max compression
```

## Comparing `mango-cli-0.0.2.tar` & `mango-cli-0.0.3.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 mangosoft   (502) staff       (20)        0 2023-05-05 17:06:33.941145 mango-cli-0.0.2/
--rw-r--r--   0 mangosoft   (502) staff       (20)      165 2023-05-05 17:06:33.940974 mango-cli-0.0.2/PKG-INFO
-drwxr-xr-x   0 mangosoft   (502) staff       (20)        0 2023-05-05 17:06:33.938197 mango-cli-0.0.2/app/
--rw-r--r--   0 mangosoft   (502) staff       (20)        0 2023-05-05 16:44:26.000000 mango-cli-0.0.2/app/__init__.py
--rw-r--r--   0 mangosoft   (502) staff       (20)      241 2023-05-05 16:49:45.000000 mango-cli-0.0.2/app/application.py
-drwxr-xr-x   0 mangosoft   (502) staff       (20)        0 2023-05-05 17:06:33.938683 mango-cli-0.0.2/app/handlers/
--rw-r--r--   0 mangosoft   (502) staff       (20)        0 2023-05-05 17:02:52.000000 mango-cli-0.0.2/app/handlers/__init__.py
--rw-r--r--   0 mangosoft   (502) staff       (20)      846 2023-05-05 16:37:03.000000 mango-cli-0.0.2/app/handlers/download_data.py
-drwxr-xr-x   0 mangosoft   (502) staff       (20)        0 2023-05-05 17:06:33.939272 mango-cli-0.0.2/app/services/
--rw-r--r--   0 mangosoft   (502) staff       (20)        0 2023-05-05 17:02:52.000000 mango-cli-0.0.2/app/services/__init__.py
--rw-r--r--   0 mangosoft   (502) staff       (20)      735 2023-05-05 16:39:20.000000 mango-cli-0.0.2/app/services/data.py
-drwxr-xr-x   0 mangosoft   (502) staff       (20)        0 2023-05-05 17:06:33.940700 mango-cli-0.0.2/mango_cli.egg-info/
--rw-r--r--   0 mangosoft   (502) staff       (20)      165 2023-05-05 17:06:33.000000 mango-cli-0.0.2/mango_cli.egg-info/PKG-INFO
--rw-r--r--   0 mangosoft   (502) staff       (20)      312 2023-05-05 17:06:33.000000 mango-cli-0.0.2/mango_cli.egg-info/SOURCES.txt
--rw-r--r--   0 mangosoft   (502) staff       (20)        1 2023-05-05 17:06:33.000000 mango-cli-0.0.2/mango_cli.egg-info/dependency_links.txt
--rw-r--r--   0 mangosoft   (502) staff       (20)       46 2023-05-05 17:06:33.000000 mango-cli-0.0.2/mango_cli.egg-info/entry_points.txt
--rw-r--r--   0 mangosoft   (502) staff       (20)        4 2023-05-05 17:06:33.000000 mango-cli-0.0.2/mango_cli.egg-info/top_level.txt
--rw-r--r--   0 mangosoft   (502) staff       (20)       38 2023-05-05 17:06:33.941208 mango-cli-0.0.2/setup.cfg
--rw-r--r--   0 mangosoft   (502) staff       (20)      417 2023-05-05 17:06:33.000000 mango-cli-0.0.2/setup.py
+drwxr-xr-x   0 mangosoft   (502) staff       (20)        0 2023-05-05 17:12:26.771793 mango-cli-0.0.3/
+-rw-r--r--   0 mangosoft   (502) staff       (20)      165 2023-05-05 17:12:26.771560 mango-cli-0.0.3/PKG-INFO
+drwxr-xr-x   0 mangosoft   (502) staff       (20)        0 2023-05-05 17:12:26.768826 mango-cli-0.0.3/app/
+-rw-r--r--   0 mangosoft   (502) staff       (20)        0 2023-05-05 16:44:26.000000 mango-cli-0.0.3/app/__init__.py
+-rw-r--r--   0 mangosoft   (502) staff       (20)      241 2023-05-05 16:49:45.000000 mango-cli-0.0.3/app/application.py
+drwxr-xr-x   0 mangosoft   (502) staff       (20)        0 2023-05-05 17:12:26.769183 mango-cli-0.0.3/app/handlers/
+-rw-r--r--   0 mangosoft   (502) staff       (20)        0 2023-05-05 17:02:52.000000 mango-cli-0.0.3/app/handlers/__init__.py
+-rw-r--r--   0 mangosoft   (502) staff       (20)      846 2023-05-05 16:37:03.000000 mango-cli-0.0.3/app/handlers/download_data.py
+drwxr-xr-x   0 mangosoft   (502) staff       (20)        0 2023-05-05 17:12:26.769787 mango-cli-0.0.3/app/services/
+-rw-r--r--   0 mangosoft   (502) staff       (20)        0 2023-05-05 17:02:52.000000 mango-cli-0.0.3/app/services/__init__.py
+-rw-r--r--   0 mangosoft   (502) staff       (20)      735 2023-05-05 16:39:20.000000 mango-cli-0.0.3/app/services/data.py
+drwxr-xr-x   0 mangosoft   (502) staff       (20)        0 2023-05-05 17:12:26.771216 mango-cli-0.0.3/mango_cli.egg-info/
+-rw-r--r--   0 mangosoft   (502) staff       (20)      165 2023-05-05 17:12:26.000000 mango-cli-0.0.3/mango_cli.egg-info/PKG-INFO
+-rw-r--r--   0 mangosoft   (502) staff       (20)      312 2023-05-05 17:12:26.000000 mango-cli-0.0.3/mango_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 mangosoft   (502) staff       (20)        1 2023-05-05 17:12:26.000000 mango-cli-0.0.3/mango_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 mangosoft   (502) staff       (20)       46 2023-05-05 17:12:26.000000 mango-cli-0.0.3/mango_cli.egg-info/entry_points.txt
+-rw-r--r--   0 mangosoft   (502) staff       (20)        4 2023-05-05 17:12:26.000000 mango-cli-0.0.3/mango_cli.egg-info/top_level.txt
+-rw-r--r--   0 mangosoft   (502) staff       (20)       38 2023-05-05 17:12:26.771877 mango-cli-0.0.3/setup.cfg
+-rw-r--r--   0 mangosoft   (502) staff       (20)      419 2023-05-05 17:12:26.000000 mango-cli-0.0.3/setup.py
```

### Comparing `mango-cli-0.0.2/app/handlers/download_data.py` & `mango-cli-0.0.3/app/handlers/download_data.py`

 * *Files identical despite different names*

### Comparing `mango-cli-0.0.2/app/services/data.py` & `mango-cli-0.0.3/app/services/data.py`

 * *Files identical despite different names*

