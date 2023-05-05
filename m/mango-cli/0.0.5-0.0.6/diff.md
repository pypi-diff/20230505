# Comparing `tmp/mango-cli-0.0.5.tar.gz` & `tmp/mango-cli-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mango-cli-0.0.5.tar", last modified: Fri May  5 17:23:35 2023, max compression
+gzip compressed data, was "mango-cli-0.0.6.tar", last modified: Fri May  5 17:33:08 2023, max compression
```

## Comparing `mango-cli-0.0.5.tar` & `mango-cli-0.0.6.tar`

### file list

```diff
@@ -1,19 +1,20 @@
-drwxr-xr-x   0 mangosoft   (502) staff       (20)        0 2023-05-05 17:23:35.788736 mango-cli-0.0.5/
--rw-r--r--   0 mangosoft   (502) staff       (20)      165 2023-05-05 17:23:35.788565 mango-cli-0.0.5/PKG-INFO
-drwxr-xr-x   0 mangosoft   (502) staff       (20)        0 2023-05-05 17:23:35.785932 mango-cli-0.0.5/app/
--rw-r--r--   0 mangosoft   (502) staff       (20)        0 2023-05-05 16:44:26.000000 mango-cli-0.0.5/app/__init__.py
--rw-r--r--   0 mangosoft   (502) staff       (20)      242 2023-05-05 17:22:31.000000 mango-cli-0.0.5/app/application.py
-drwxr-xr-x   0 mangosoft   (502) staff       (20)        0 2023-05-05 17:23:35.786366 mango-cli-0.0.5/app/handlers/
--rw-r--r--   0 mangosoft   (502) staff       (20)        0 2023-05-05 17:02:52.000000 mango-cli-0.0.5/app/handlers/__init__.py
--rw-r--r--   0 mangosoft   (502) staff       (20)      810 2023-05-05 17:23:15.000000 mango-cli-0.0.5/app/handlers/download_data.py
-drwxr-xr-x   0 mangosoft   (502) staff       (20)        0 2023-05-05 17:23:35.786874 mango-cli-0.0.5/app/services/
--rw-r--r--   0 mangosoft   (502) staff       (20)        0 2023-05-05 17:02:52.000000 mango-cli-0.0.5/app/services/__init__.py
--rw-r--r--   0 mangosoft   (502) staff       (20)      735 2023-05-05 16:39:20.000000 mango-cli-0.0.5/app/services/data.py
-drwxr-xr-x   0 mangosoft   (502) staff       (20)        0 2023-05-05 17:23:35.788261 mango-cli-0.0.5/mango_cli.egg-info/
--rw-r--r--   0 mangosoft   (502) staff       (20)      165 2023-05-05 17:23:35.000000 mango-cli-0.0.5/mango_cli.egg-info/PKG-INFO
--rw-r--r--   0 mangosoft   (502) staff       (20)      312 2023-05-05 17:23:35.000000 mango-cli-0.0.5/mango_cli.egg-info/SOURCES.txt
--rw-r--r--   0 mangosoft   (502) staff       (20)        1 2023-05-05 17:23:35.000000 mango-cli-0.0.5/mango_cli.egg-info/dependency_links.txt
--rw-r--r--   0 mangosoft   (502) staff       (20)       46 2023-05-05 17:23:35.000000 mango-cli-0.0.5/mango_cli.egg-info/entry_points.txt
--rw-r--r--   0 mangosoft   (502) staff       (20)        4 2023-05-05 17:23:35.000000 mango-cli-0.0.5/mango_cli.egg-info/top_level.txt
--rw-r--r--   0 mangosoft   (502) staff       (20)       38 2023-05-05 17:23:35.788795 mango-cli-0.0.5/setup.cfg
--rw-r--r--   0 mangosoft   (502) staff       (20)      444 2023-05-05 17:23:35.000000 mango-cli-0.0.5/setup.py
+drwxr-xr-x   0 mangosoft   (502) staff       (20)        0 2023-05-05 17:33:08.879113 mango-cli-0.0.6/
+-rw-r--r--   0 mangosoft   (502) staff       (20)      138 2023-05-05 17:33:08.878939 mango-cli-0.0.6/PKG-INFO
+drwxr-xr-x   0 mangosoft   (502) staff       (20)        0 2023-05-05 17:33:08.875669 mango-cli-0.0.6/app/
+-rw-r--r--   0 mangosoft   (502) staff       (20)        0 2023-05-05 16:44:26.000000 mango-cli-0.0.6/app/__init__.py
+-rw-r--r--   0 mangosoft   (502) staff       (20)      242 2023-05-05 17:22:31.000000 mango-cli-0.0.6/app/application.py
+drwxr-xr-x   0 mangosoft   (502) staff       (20)        0 2023-05-05 17:33:08.876241 mango-cli-0.0.6/app/handlers/
+-rw-r--r--   0 mangosoft   (502) staff       (20)        0 2023-05-05 17:02:52.000000 mango-cli-0.0.6/app/handlers/__init__.py
+-rw-r--r--   0 mangosoft   (502) staff       (20)      810 2023-05-05 17:23:15.000000 mango-cli-0.0.6/app/handlers/download_data.py
+drwxr-xr-x   0 mangosoft   (502) staff       (20)        0 2023-05-05 17:33:08.876773 mango-cli-0.0.6/app/services/
+-rw-r--r--   0 mangosoft   (502) staff       (20)        0 2023-05-05 17:02:52.000000 mango-cli-0.0.6/app/services/__init__.py
+-rw-r--r--   0 mangosoft   (502) staff       (20)      735 2023-05-05 16:39:20.000000 mango-cli-0.0.6/app/services/data.py
+drwxr-xr-x   0 mangosoft   (502) staff       (20)        0 2023-05-05 17:33:08.878625 mango-cli-0.0.6/mango_cli.egg-info/
+-rw-r--r--   0 mangosoft   (502) staff       (20)      138 2023-05-05 17:33:08.000000 mango-cli-0.0.6/mango_cli.egg-info/PKG-INFO
+-rw-r--r--   0 mangosoft   (502) staff       (20)      344 2023-05-05 17:33:08.000000 mango-cli-0.0.6/mango_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 mangosoft   (502) staff       (20)        1 2023-05-05 17:33:08.000000 mango-cli-0.0.6/mango_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 mangosoft   (502) staff       (20)       46 2023-05-05 17:33:08.000000 mango-cli-0.0.6/mango_cli.egg-info/entry_points.txt
+-rw-r--r--   0 mangosoft   (502) staff       (20)       17 2023-05-05 17:33:08.000000 mango-cli-0.0.6/mango_cli.egg-info/requires.txt
+-rw-r--r--   0 mangosoft   (502) staff       (20)        4 2023-05-05 17:33:08.000000 mango-cli-0.0.6/mango_cli.egg-info/top_level.txt
+-rw-r--r--   0 mangosoft   (502) staff       (20)       38 2023-05-05 17:33:08.879180 mango-cli-0.0.6/setup.cfg
+-rw-r--r--   0 mangosoft   (502) staff       (20)      465 2023-05-05 17:33:00.000000 mango-cli-0.0.6/setup.py
```

### Comparing `mango-cli-0.0.5/app/handlers/download_data.py` & `mango-cli-0.0.6/app/handlers/download_data.py`

 * *Files identical despite different names*

### Comparing `mango-cli-0.0.5/app/services/data.py` & `mango-cli-0.0.6/app/services/data.py`

 * *Files identical despite different names*

