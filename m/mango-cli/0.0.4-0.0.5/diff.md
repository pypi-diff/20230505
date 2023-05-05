# Comparing `tmp/mango-cli-0.0.4.tar.gz` & `tmp/mango-cli-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mango-cli-0.0.4.tar", last modified: Fri May  5 17:19:36 2023, max compression
+gzip compressed data, was "mango-cli-0.0.5.tar", last modified: Fri May  5 17:23:35 2023, max compression
```

## Comparing `mango-cli-0.0.4.tar` & `mango-cli-0.0.5.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 mangosoft   (502) staff       (20)        0 2023-05-05 17:19:36.061480 mango-cli-0.0.4/
--rw-r--r--   0 mangosoft   (502) staff       (20)      165 2023-05-05 17:19:36.061250 mango-cli-0.0.4/PKG-INFO
-drwxr-xr-x   0 mangosoft   (502) staff       (20)        0 2023-05-05 17:19:36.058354 mango-cli-0.0.4/app/
--rw-r--r--   0 mangosoft   (502) staff       (20)        0 2023-05-05 16:44:26.000000 mango-cli-0.0.4/app/__init__.py
--rw-r--r--   0 mangosoft   (502) staff       (20)      241 2023-05-05 17:15:32.000000 mango-cli-0.0.4/app/application.py
-drwxr-xr-x   0 mangosoft   (502) staff       (20)        0 2023-05-05 17:19:36.059007 mango-cli-0.0.4/app/handlers/
--rw-r--r--   0 mangosoft   (502) staff       (20)        0 2023-05-05 17:02:52.000000 mango-cli-0.0.4/app/handlers/__init__.py
--rw-r--r--   0 mangosoft   (502) staff       (20)      846 2023-05-05 16:37:03.000000 mango-cli-0.0.4/app/handlers/download_data.py
-drwxr-xr-x   0 mangosoft   (502) staff       (20)        0 2023-05-05 17:19:36.059521 mango-cli-0.0.4/app/services/
--rw-r--r--   0 mangosoft   (502) staff       (20)        0 2023-05-05 17:02:52.000000 mango-cli-0.0.4/app/services/__init__.py
--rw-r--r--   0 mangosoft   (502) staff       (20)      735 2023-05-05 16:39:20.000000 mango-cli-0.0.4/app/services/data.py
-drwxr-xr-x   0 mangosoft   (502) staff       (20)        0 2023-05-05 17:19:36.060798 mango-cli-0.0.4/mango_cli.egg-info/
--rw-r--r--   0 mangosoft   (502) staff       (20)      165 2023-05-05 17:19:36.000000 mango-cli-0.0.4/mango_cli.egg-info/PKG-INFO
--rw-r--r--   0 mangosoft   (502) staff       (20)      312 2023-05-05 17:19:36.000000 mango-cli-0.0.4/mango_cli.egg-info/SOURCES.txt
--rw-r--r--   0 mangosoft   (502) staff       (20)        1 2023-05-05 17:19:36.000000 mango-cli-0.0.4/mango_cli.egg-info/dependency_links.txt
--rw-r--r--   0 mangosoft   (502) staff       (20)       46 2023-05-05 17:19:36.000000 mango-cli-0.0.4/mango_cli.egg-info/entry_points.txt
--rw-r--r--   0 mangosoft   (502) staff       (20)        4 2023-05-05 17:19:36.000000 mango-cli-0.0.4/mango_cli.egg-info/top_level.txt
--rw-r--r--   0 mangosoft   (502) staff       (20)       38 2023-05-05 17:19:36.061570 mango-cli-0.0.4/setup.cfg
--rw-r--r--   0 mangosoft   (502) staff       (20)      443 2023-05-05 17:19:30.000000 mango-cli-0.0.4/setup.py
+drwxr-xr-x   0 mangosoft   (502) staff       (20)        0 2023-05-05 17:23:35.788736 mango-cli-0.0.5/
+-rw-r--r--   0 mangosoft   (502) staff       (20)      165 2023-05-05 17:23:35.788565 mango-cli-0.0.5/PKG-INFO
+drwxr-xr-x   0 mangosoft   (502) staff       (20)        0 2023-05-05 17:23:35.785932 mango-cli-0.0.5/app/
+-rw-r--r--   0 mangosoft   (502) staff       (20)        0 2023-05-05 16:44:26.000000 mango-cli-0.0.5/app/__init__.py
+-rw-r--r--   0 mangosoft   (502) staff       (20)      242 2023-05-05 17:22:31.000000 mango-cli-0.0.5/app/application.py
+drwxr-xr-x   0 mangosoft   (502) staff       (20)        0 2023-05-05 17:23:35.786366 mango-cli-0.0.5/app/handlers/
+-rw-r--r--   0 mangosoft   (502) staff       (20)        0 2023-05-05 17:02:52.000000 mango-cli-0.0.5/app/handlers/__init__.py
+-rw-r--r--   0 mangosoft   (502) staff       (20)      810 2023-05-05 17:23:15.000000 mango-cli-0.0.5/app/handlers/download_data.py
+drwxr-xr-x   0 mangosoft   (502) staff       (20)        0 2023-05-05 17:23:35.786874 mango-cli-0.0.5/app/services/
+-rw-r--r--   0 mangosoft   (502) staff       (20)        0 2023-05-05 17:02:52.000000 mango-cli-0.0.5/app/services/__init__.py
+-rw-r--r--   0 mangosoft   (502) staff       (20)      735 2023-05-05 16:39:20.000000 mango-cli-0.0.5/app/services/data.py
+drwxr-xr-x   0 mangosoft   (502) staff       (20)        0 2023-05-05 17:23:35.788261 mango-cli-0.0.5/mango_cli.egg-info/
+-rw-r--r--   0 mangosoft   (502) staff       (20)      165 2023-05-05 17:23:35.000000 mango-cli-0.0.5/mango_cli.egg-info/PKG-INFO
+-rw-r--r--   0 mangosoft   (502) staff       (20)      312 2023-05-05 17:23:35.000000 mango-cli-0.0.5/mango_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 mangosoft   (502) staff       (20)        1 2023-05-05 17:23:35.000000 mango-cli-0.0.5/mango_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 mangosoft   (502) staff       (20)       46 2023-05-05 17:23:35.000000 mango-cli-0.0.5/mango_cli.egg-info/entry_points.txt
+-rw-r--r--   0 mangosoft   (502) staff       (20)        4 2023-05-05 17:23:35.000000 mango-cli-0.0.5/mango_cli.egg-info/top_level.txt
+-rw-r--r--   0 mangosoft   (502) staff       (20)       38 2023-05-05 17:23:35.788795 mango-cli-0.0.5/setup.cfg
+-rw-r--r--   0 mangosoft   (502) staff       (20)      444 2023-05-05 17:23:35.000000 mango-cli-0.0.5/setup.py
```

### Comparing `mango-cli-0.0.4/app/handlers/download_data.py` & `mango-cli-0.0.5/app/handlers/download_data.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 import inquirer
 import boto3
 import os
-from services.data import Data
+from ..services.data import Data
 
 def download_data():
     dynamo = boto3.resource('dynamodb')
     tables = [table.name for table in dynamo.tables.all()]
-    deafult_output_path = os.getcwd()
 
     questions = [
         inquirer.List('table',
                       message="Select a table",
                       choices=tables,
                       autocomplete=True,
                       carousel=True,
```

### Comparing `mango-cli-0.0.4/app/services/data.py` & `mango-cli-0.0.5/app/services/data.py`

 * *Files identical despite different names*

