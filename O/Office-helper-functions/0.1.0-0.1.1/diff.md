# Comparing `tmp/Office_helper_functions-0.1.0.tar.gz` & `tmp/Office_helper_functions-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Office_helper_functions-0.1.0.tar", last modified: Thu May  4 20:13:28 2023, max compression
+gzip compressed data, was "Office_helper_functions-0.1.1.tar", last modified: Thu May  4 20:54:09 2023, max compression
```

## Comparing `Office_helper_functions-0.1.0.tar` & `Office_helper_functions-0.1.1.tar`

### file list

```diff
@@ -1,11 +1,21 @@
-drwxrwxrwx   0        0        0        0 2023-05-04 20:13:28.031390 Office_helper_functions-0.1.0/
-drwxrwxrwx   0        0        0        0 2023-05-04 20:13:28.007823 Office_helper_functions-0.1.0/Office_helper_functions/
--rw-rw-rw-   0        0        0        0 2023-05-04 19:59:16.000000 Office_helper_functions-0.1.0/Office_helper_functions/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-04 20:13:28.023374 Office_helper_functions-0.1.0/Office_helper_functions.egg-info/
--rw-rw-rw-   0        0        0      211 2023-05-04 20:13:27.000000 Office_helper_functions-0.1.0/Office_helper_functions.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      232 2023-05-04 20:13:27.000000 Office_helper_functions-0.1.0/Office_helper_functions.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-04 20:13:27.000000 Office_helper_functions-0.1.0/Office_helper_functions.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       24 2023-05-04 20:13:27.000000 Office_helper_functions-0.1.0/Office_helper_functions.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      211 2023-05-04 20:13:28.023374 Office_helper_functions-0.1.0/PKG-INFO
--rw-rw-rw-   0        0        0       42 2023-05-04 20:13:28.031390 Office_helper_functions-0.1.0/setup.cfg
--rw-rw-rw-   0        0        0      352 2023-05-04 20:12:03.000000 Office_helper_functions-0.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-04 20:54:09.520306 Office_helper_functions-0.1.1/
+drwxrwxrwx   0        0        0        0 2023-05-04 20:54:09.469461 Office_helper_functions-0.1.1/Office_helper_functions/
+-rw-rw-rw-   0        0        0     3175 2023-05-04 20:51:57.000000 Office_helper_functions-0.1.1/Office_helper_functions/Dates.py
+drwxrwxrwx   0        0        0        0 2023-05-04 20:54:09.512154 Office_helper_functions-0.1.1/Office_helper_functions/Image/
+-rw-rw-rw-   0        0        0     1418 2023-05-04 20:40:27.000000 Office_helper_functions-0.1.1/Office_helper_functions/Image/Image_operations.py
+-rw-rw-rw-   0        0        0        0 2023-05-04 20:41:09.000000 Office_helper_functions-0.1.1/Office_helper_functions/Image/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-04 20:54:09.518214 Office_helper_functions-0.1.1/Office_helper_functions/Word/
+-rw-rw-rw-   0        0        0     2473 2023-05-04 20:48:38.000000 Office_helper_functions-0.1.1/Office_helper_functions/Word/Word_Image.py
+-rw-rw-rw-   0        0        0        0 2023-05-04 20:52:17.000000 Office_helper_functions-0.1.1/Office_helper_functions/Word/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-04 20:54:09.520306 Office_helper_functions-0.1.1/Office_helper_functions/Word/checkbox/
+-rw-rw-rw-   0        0        0        0 2023-05-04 19:59:26.000000 Office_helper_functions-0.1.1/Office_helper_functions/Word/checkbox/__init__.py
+-rw-rw-rw-   0        0        0     2094 2023-05-04 19:57:33.000000 Office_helper_functions-0.1.1/Office_helper_functions/Word/form_field.py
+-rw-rw-rw-   0        0        0        0 2023-05-04 19:59:16.000000 Office_helper_functions-0.1.1/Office_helper_functions/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-04 20:54:09.503901 Office_helper_functions-0.1.1/Office_helper_functions.egg-info/
+-rw-rw-rw-   0        0        0      201 2023-05-04 20:54:09.000000 Office_helper_functions-0.1.1/Office_helper_functions.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      534 2023-05-04 20:54:09.000000 Office_helper_functions-0.1.1/Office_helper_functions.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-04 20:54:09.000000 Office_helper_functions-0.1.1/Office_helper_functions.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       24 2023-05-04 20:54:09.000000 Office_helper_functions-0.1.1/Office_helper_functions.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      201 2023-05-04 20:54:09.520306 Office_helper_functions-0.1.1/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2023-05-04 20:54:09.520306 Office_helper_functions-0.1.1/setup.cfg
+-rw-rw-rw-   0        0        0      353 2023-05-04 20:53:56.000000 Office_helper_functions-0.1.1/setup.py
```

