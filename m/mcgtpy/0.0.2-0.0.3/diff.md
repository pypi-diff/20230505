# Comparing `tmp/mcgtpy-0.0.2.tar.gz` & `tmp/mcgtpy-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mcgtpy-0.0.2.tar", last modified: Fri May  5 16:52:52 2023, max compression
+gzip compressed data, was "mcgtpy-0.0.3.tar", last modified: Fri May  5 17:31:15 2023, max compression
```

## Comparing `mcgtpy-0.0.2.tar` & `mcgtpy-0.0.3.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-05 16:52:52.346444 mcgtpy-0.0.2/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      465 2023-05-05 16:52:52.346444 mcgtpy-0.0.2/PKG-INFO
--rw-r--r--   0 circleci  (1001) circleci  (1002)       12 2023-05-05 16:52:52.000000 mcgtpy-0.0.2/README.md
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-05 16:52:52.346444 mcgtpy-0.0.2/mcgtpy/
--rw-r--r--   0 circleci  (1001) circleci  (1002)       79 2023-05-05 16:52:52.000000 mcgtpy-0.0.2/mcgtpy/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1109 2023-05-05 16:52:52.000000 mcgtpy-0.0.2/mcgtpy/helper_functions.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1545 2023-05-05 16:52:52.000000 mcgtpy-0.0.2/mcgtpy/my_stats.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-05 16:52:52.346444 mcgtpy-0.0.2/mcgtpy.egg-info/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      465 2023-05-05 16:52:52.000000 mcgtpy-0.0.2/mcgtpy.egg-info/PKG-INFO
--rw-r--r--   0 circleci  (1001) circleci  (1002)      203 2023-05-05 16:52:52.000000 mcgtpy-0.0.2/mcgtpy.egg-info/SOURCES.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2023-05-05 16:52:52.000000 mcgtpy-0.0.2/mcgtpy.egg-info/dependency_links.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)        7 2023-05-05 16:52:52.000000 mcgtpy-0.0.2/mcgtpy.egg-info/top_level.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)       38 2023-05-05 16:52:52.346444 mcgtpy-0.0.2/setup.cfg
--rw-r--r--   0 circleci  (1001) circleci  (1002)      777 2023-05-05 16:52:52.000000 mcgtpy-0.0.2/setup.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-05 17:31:15.103804 mcgtpy-0.0.3/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      465 2023-05-05 17:31:15.103804 mcgtpy-0.0.3/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       12 2023-05-05 17:31:14.000000 mcgtpy-0.0.3/README.md
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-05 17:31:15.103804 mcgtpy-0.0.3/mcgtpy/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       79 2023-05-05 17:31:14.000000 mcgtpy-0.0.3/mcgtpy/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1262 2023-05-05 17:31:14.000000 mcgtpy-0.0.3/mcgtpy/helper_functions.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1545 2023-05-05 17:31:14.000000 mcgtpy-0.0.3/mcgtpy/my_stats.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-05 17:31:15.103804 mcgtpy-0.0.3/mcgtpy.egg-info/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      465 2023-05-05 17:31:15.000000 mcgtpy-0.0.3/mcgtpy.egg-info/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      203 2023-05-05 17:31:15.000000 mcgtpy-0.0.3/mcgtpy.egg-info/SOURCES.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2023-05-05 17:31:15.000000 mcgtpy-0.0.3/mcgtpy.egg-info/dependency_links.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        7 2023-05-05 17:31:15.000000 mcgtpy-0.0.3/mcgtpy.egg-info/top_level.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       38 2023-05-05 17:31:15.103804 mcgtpy-0.0.3/setup.cfg
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      777 2023-05-05 17:31:14.000000 mcgtpy-0.0.3/setup.py
```

### Comparing `mcgtpy-0.0.2/mcgtpy/helper_functions.py` & `mcgtpy-0.0.3/mcgtpy/helper_functions.py`

 * *Files 24% similar despite different names*

```diff
@@ -5,17 +5,19 @@
     """
     new_col_names_list = []
     for col_name in old_col_names:
         # strip whitespace
         col_name_stripped = col_name.strip()
         # make lowercase
         col_name_stripped_and_lower = col_name_stripped.lower()
+        # replace " " with "_"
+        col_name_stripped_and_lower_and_spaces_removed = col_name_stripped_and_lower.replace(" ", "_")
         # remove weird characters
         new_col_name = "".join(
-            item for item in str(col_name_stripped_and_lower) if item.isalnum() or "_" in item
+            item for item in str(col_name_stripped_and_lower_and_spaces_removed) if item.isalnum() or "_" in item
         )
         # make sure there are 0 instances of 2 _'s next to each other
         while "__" in new_col_name:
             new_col_name = new_col_name.replace("__", "_")
         # make sure the column name does not lead or end with _
         while new_col_name[0] == "_":
             new_col_name = new_col_name[1 : len(new_col_name)]
```

### Comparing `mcgtpy-0.0.2/mcgtpy/my_stats.py` & `mcgtpy-0.0.3/mcgtpy/my_stats.py`

 * *Files identical despite different names*

### Comparing `mcgtpy-0.0.2/setup.py` & `mcgtpy-0.0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 
-VERSION = '0.0.2'
+VERSION = '0.0.3'
 DESCRIPTION = 'My first Python Package!'
 LONG_DESCRIPTION = 'This package will have everything I use on a daily basis to make life easier when coding in Python.'
 
 author_name = "Myles Thomas"
 author_email = "mylescgthomas@gmail.com"
 
 setup(
```

