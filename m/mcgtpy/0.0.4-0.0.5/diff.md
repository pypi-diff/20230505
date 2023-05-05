# Comparing `tmp/mcgtpy-0.0.4.tar.gz` & `tmp/mcgtpy-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mcgtpy-0.0.4.tar", last modified: Fri May  5 17:37:01 2023, max compression
+gzip compressed data, was "mcgtpy-0.0.5.tar", last modified: Fri May  5 18:32:06 2023, max compression
```

## Comparing `mcgtpy-0.0.4.tar` & `mcgtpy-0.0.5.tar`

### file list

```diff
@@ -1,14 +1,15 @@
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-05 17:37:01.172730 mcgtpy-0.0.4/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      465 2023-05-05 17:37:01.172730 mcgtpy-0.0.4/PKG-INFO
--rw-r--r--   0 circleci  (1001) circleci  (1002)       12 2023-05-05 17:37:00.000000 mcgtpy-0.0.4/README.md
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-05 17:37:01.172730 mcgtpy-0.0.4/mcgtpy/
--rw-r--r--   0 circleci  (1001) circleci  (1002)       79 2023-05-05 17:37:00.000000 mcgtpy-0.0.4/mcgtpy/__init__.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1262 2023-05-05 17:37:00.000000 mcgtpy-0.0.4/mcgtpy/helper_functions.py
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1545 2023-05-05 17:37:00.000000 mcgtpy-0.0.4/mcgtpy/my_stats.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-05 17:37:01.172730 mcgtpy-0.0.4/mcgtpy.egg-info/
--rw-r--r--   0 circleci  (1001) circleci  (1002)      465 2023-05-05 17:37:01.000000 mcgtpy-0.0.4/mcgtpy.egg-info/PKG-INFO
--rw-r--r--   0 circleci  (1001) circleci  (1002)      203 2023-05-05 17:37:01.000000 mcgtpy-0.0.4/mcgtpy.egg-info/SOURCES.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2023-05-05 17:37:01.000000 mcgtpy-0.0.4/mcgtpy.egg-info/dependency_links.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)        7 2023-05-05 17:37:01.000000 mcgtpy-0.0.4/mcgtpy.egg-info/top_level.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)       38 2023-05-05 17:37:01.172730 mcgtpy-0.0.4/setup.cfg
--rw-r--r--   0 circleci  (1001) circleci  (1002)      777 2023-05-05 17:37:00.000000 mcgtpy-0.0.4/setup.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-05 18:32:06.490954 mcgtpy-0.0.5/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      465 2023-05-05 18:32:06.490954 mcgtpy-0.0.5/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       12 2023-05-05 18:32:06.000000 mcgtpy-0.0.5/README.md
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-05 18:32:06.486955 mcgtpy-0.0.5/mcgtpy/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       79 2023-05-05 18:32:06.000000 mcgtpy-0.0.5/mcgtpy/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1262 2023-05-05 18:32:06.000000 mcgtpy-0.0.5/mcgtpy/helper_functions.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1545 2023-05-05 18:32:06.000000 mcgtpy-0.0.5/mcgtpy/my_stats.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-05 18:32:06.490954 mcgtpy-0.0.5/mcgtpy.egg-info/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      465 2023-05-05 18:32:06.000000 mcgtpy-0.0.5/mcgtpy.egg-info/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      232 2023-05-05 18:32:06.000000 mcgtpy-0.0.5/mcgtpy.egg-info/SOURCES.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2023-05-05 18:32:06.000000 mcgtpy-0.0.5/mcgtpy.egg-info/dependency_links.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       19 2023-05-05 18:32:06.000000 mcgtpy-0.0.5/mcgtpy.egg-info/requires.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        7 2023-05-05 18:32:06.000000 mcgtpy-0.0.5/mcgtpy.egg-info/top_level.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       38 2023-05-05 18:32:06.490954 mcgtpy-0.0.5/setup.cfg
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      870 2023-05-05 18:32:06.000000 mcgtpy-0.0.5/setup.py
```

### Comparing `mcgtpy-0.0.4/mcgtpy/helper_functions.py` & `mcgtpy-0.0.5/mcgtpy/helper_functions.py`

 * *Files identical despite different names*

### Comparing `mcgtpy-0.0.4/mcgtpy/my_stats.py` & `mcgtpy-0.0.5/mcgtpy/my_stats.py`

 * *Files identical despite different names*

