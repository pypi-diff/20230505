# Comparing `tmp/mango-cli-0.0.9a1.tar.gz` & `tmp/mango-cli-0.0.9a2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mango-cli-0.0.9a1.tar", last modified: Fri May  5 19:26:37 2023, max compression
+gzip compressed data, was "mango-cli-0.0.9a2.tar", last modified: Fri May  5 19:28:27 2023, max compression
```

## Comparing `mango-cli-0.0.9a1.tar` & `mango-cli-0.0.9a2.tar`

### file list

```diff
@@ -1,14 +1,20 @@
-drwxr-xr-x   0 mangosoft   (502) staff       (20)        0 2023-05-05 19:26:37.311354 mango-cli-0.0.9a1/
--rw-r--r--   0 mangosoft   (502) staff       (20)      140 2023-05-05 19:26:37.311041 mango-cli-0.0.9a1/PKG-INFO
-drwxr-xr-x   0 mangosoft   (502) staff       (20)        0 2023-05-05 19:26:37.309623 mango-cli-0.0.9a1/app/
--rw-r--r--   0 mangosoft   (502) staff       (20)        0 2023-05-05 19:26:29.000000 mango-cli-0.0.9a1/app/__init__.py
--rw-r--r--   0 mangosoft   (502) staff       (20)      242 2023-05-05 17:22:31.000000 mango-cli-0.0.9a1/app/application.py
-drwxr-xr-x   0 mangosoft   (502) staff       (20)        0 2023-05-05 19:26:37.310770 mango-cli-0.0.9a1/mango_cli.egg-info/
--rw-r--r--   0 mangosoft   (502) staff       (20)      140 2023-05-05 19:26:37.000000 mango-cli-0.0.9a1/mango_cli.egg-info/PKG-INFO
--rw-r--r--   0 mangosoft   (502) staff       (20)      243 2023-05-05 19:26:37.000000 mango-cli-0.0.9a1/mango_cli.egg-info/SOURCES.txt
--rw-r--r--   0 mangosoft   (502) staff       (20)        1 2023-05-05 19:26:37.000000 mango-cli-0.0.9a1/mango_cli.egg-info/dependency_links.txt
--rw-r--r--   0 mangosoft   (502) staff       (20)       46 2023-05-05 19:26:37.000000 mango-cli-0.0.9a1/mango_cli.egg-info/entry_points.txt
--rw-r--r--   0 mangosoft   (502) staff       (20)      670 2023-05-05 19:26:37.000000 mango-cli-0.0.9a1/mango_cli.egg-info/requires.txt
--rw-r--r--   0 mangosoft   (502) staff       (20)        4 2023-05-05 19:26:37.000000 mango-cli-0.0.9a1/mango_cli.egg-info/top_level.txt
--rw-r--r--   0 mangosoft   (502) staff       (20)       38 2023-05-05 19:26:37.311484 mango-cli-0.0.9a1/setup.cfg
--rw-r--r--   0 mangosoft   (502) staff       (20)      510 2023-05-05 19:26:05.000000 mango-cli-0.0.9a1/setup.py
+drwxr-xr-x   0 mangosoft   (502) staff       (20)        0 2023-05-05 19:28:27.072373 mango-cli-0.0.9a2/
+-rw-r--r--   0 mangosoft   (502) staff       (20)      140 2023-05-05 19:28:27.072182 mango-cli-0.0.9a2/PKG-INFO
+drwxr-xr-x   0 mangosoft   (502) staff       (20)        0 2023-05-05 19:28:27.069414 mango-cli-0.0.9a2/app/
+-rw-r--r--   0 mangosoft   (502) staff       (20)        0 2023-05-05 19:26:29.000000 mango-cli-0.0.9a2/app/__init__.py
+-rw-r--r--   0 mangosoft   (502) staff       (20)      242 2023-05-05 17:22:31.000000 mango-cli-0.0.9a2/app/application.py
+drwxr-xr-x   0 mangosoft   (502) staff       (20)        0 2023-05-05 19:28:27.069877 mango-cli-0.0.9a2/app/handlers/
+-rw-r--r--   0 mangosoft   (502) staff       (20)        0 2023-05-05 19:28:09.000000 mango-cli-0.0.9a2/app/handlers/__init__.py
+-rw-r--r--   0 mangosoft   (502) staff       (20)      938 2023-05-05 19:11:04.000000 mango-cli-0.0.9a2/app/handlers/download_data.py
+drwxr-xr-x   0 mangosoft   (502) staff       (20)        0 2023-05-05 19:28:27.070337 mango-cli-0.0.9a2/app/services/
+-rw-r--r--   0 mangosoft   (502) staff       (20)        0 2023-05-05 19:28:09.000000 mango-cli-0.0.9a2/app/services/__init__.py
+-rw-r--r--   0 mangosoft   (502) staff       (20)      735 2023-05-05 16:39:20.000000 mango-cli-0.0.9a2/app/services/data.py
+drwxr-xr-x   0 mangosoft   (502) staff       (20)        0 2023-05-05 19:28:27.071795 mango-cli-0.0.9a2/mango_cli.egg-info/
+-rw-r--r--   0 mangosoft   (502) staff       (20)      140 2023-05-05 19:28:27.000000 mango-cli-0.0.9a2/mango_cli.egg-info/PKG-INFO
+-rw-r--r--   0 mangosoft   (502) staff       (20)      344 2023-05-05 19:28:27.000000 mango-cli-0.0.9a2/mango_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 mangosoft   (502) staff       (20)        1 2023-05-05 19:28:27.000000 mango-cli-0.0.9a2/mango_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 mangosoft   (502) staff       (20)       46 2023-05-05 19:28:27.000000 mango-cli-0.0.9a2/mango_cli.egg-info/entry_points.txt
+-rw-r--r--   0 mangosoft   (502) staff       (20)      670 2023-05-05 19:28:27.000000 mango-cli-0.0.9a2/mango_cli.egg-info/requires.txt
+-rw-r--r--   0 mangosoft   (502) staff       (20)        4 2023-05-05 19:28:27.000000 mango-cli-0.0.9a2/mango_cli.egg-info/top_level.txt
+-rw-r--r--   0 mangosoft   (502) staff       (20)       38 2023-05-05 19:28:27.072444 mango-cli-0.0.9a2/setup.cfg
+-rw-r--r--   0 mangosoft   (502) staff       (20)      510 2023-05-05 19:28:08.000000 mango-cli-0.0.9a2/setup.py
```

### Comparing `mango-cli-0.0.9a1/mango_cli.egg-info/requires.txt` & `mango-cli-0.0.9a2/mango_cli.egg-info/requires.txt`

 * *Files identical despite different names*

