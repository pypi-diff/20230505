# Comparing `tmp/intake_dataframe_catalog-0.0.1.tar.gz` & `tmp/intake_dataframe_catalog-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "intake_dataframe_catalog-0.0.1.tar", last modified: Fri May  5 04:32:52 2023, max compression
+gzip compressed data, was "intake_dataframe_catalog-0.0.2.tar", last modified: Fri May  5 05:52:13 2023, max compression
```

## Comparing `intake_dataframe_catalog-0.0.1.tar` & `intake_dataframe_catalog-0.0.2.tar`

### file list

```diff
@@ -1,23 +1,20 @@
-drwxr-xr-x   0 dougiesquire   (501) staff       (20)        0 2023-05-05 04:32:52.067945 intake_dataframe_catalog-0.0.1/
--rw-r--r--   0 dougiesquire   (501) staff       (20)    11357 2023-03-27 22:20:51.000000 intake_dataframe_catalog-0.0.1/LICENSE
--rw-r--r--   0 dougiesquire   (501) staff       (20)      491 2023-05-05 04:32:52.068005 intake_dataframe_catalog-0.0.1/PKG-INFO
--rw-r--r--   0 dougiesquire   (501) staff       (20)     1672 2023-05-04 04:35:19.000000 intake_dataframe_catalog-0.0.1/README.md
--rw-r--r--   0 dougiesquire   (501) staff       (20)      433 2023-05-05 04:32:52.068300 intake_dataframe_catalog-0.0.1/setup.cfg
--rw-r--r--   0 dougiesquire   (501) staff       (20)      903 2023-05-05 04:30:42.000000 intake_dataframe_catalog-0.0.1/setup.py
-drwxr-xr-x   0 dougiesquire   (501) staff       (20)        0 2023-05-05 04:32:52.064454 intake_dataframe_catalog-0.0.1/src/
-drwxr-xr-x   0 dougiesquire   (501) staff       (20)        0 2023-05-05 04:32:52.068433 intake_dataframe_catalog-0.0.1/src/intake_dataframe_catalog/
--rw-r--r--   0 dougiesquire   (501) staff       (20)      219 2023-05-01 20:51:27.000000 intake_dataframe_catalog-0.0.1/src/intake_dataframe_catalog/__init__.py
--rw-r--r--   0 dougiesquire   (501) staff       (20)     4127 2023-05-05 00:44:57.000000 intake_dataframe_catalog-0.0.1/src/intake_dataframe_catalog/_search.py
--rw-r--r--   0 dougiesquire   (501) staff       (20)      497 2023-05-05 04:32:52.068466 intake_dataframe_catalog-0.0.1/src/intake_dataframe_catalog/_version.py
--rw-r--r--   0 dougiesquire   (501) staff       (20)    21064 2023-05-05 04:18:32.000000 intake_dataframe_catalog-0.0.1/src/intake_dataframe_catalog/core.py
-drwxr-xr-x   0 dougiesquire   (501) staff       (20)        0 2023-05-05 04:32:52.067354 intake_dataframe_catalog-0.0.1/src/intake_dataframe_catalog.egg-info/
--rw-r--r--   0 dougiesquire   (501) staff       (20)      491 2023-05-05 04:32:52.000000 intake_dataframe_catalog-0.0.1/src/intake_dataframe_catalog.egg-info/PKG-INFO
--rw-r--r--   0 dougiesquire   (501) staff       (20)      563 2023-05-05 04:32:52.000000 intake_dataframe_catalog-0.0.1/src/intake_dataframe_catalog.egg-info/SOURCES.txt
--rw-r--r--   0 dougiesquire   (501) staff       (20)        1 2023-05-05 04:32:52.000000 intake_dataframe_catalog-0.0.1/src/intake_dataframe_catalog.egg-info/dependency_links.txt
--rw-r--r--   0 dougiesquire   (501) staff       (20)       74 2023-05-05 04:32:52.000000 intake_dataframe_catalog-0.0.1/src/intake_dataframe_catalog.egg-info/entry_points.txt
--rw-r--r--   0 dougiesquire   (501) staff       (20)       14 2023-05-05 04:32:52.000000 intake_dataframe_catalog-0.0.1/src/intake_dataframe_catalog.egg-info/requires.txt
--rw-r--r--   0 dougiesquire   (501) staff       (20)       25 2023-05-05 04:32:52.000000 intake_dataframe_catalog-0.0.1/src/intake_dataframe_catalog.egg-info/top_level.txt
-drwxr-xr-x   0 dougiesquire   (501) staff       (20)        0 2023-05-05 04:32:52.067788 intake_dataframe_catalog-0.0.1/tests/
--rw-r--r--   0 dougiesquire   (501) staff       (20)    21272 2023-05-05 00:44:57.000000 intake_dataframe_catalog-0.0.1/tests/test_core.py
--rw-r--r--   0 dougiesquire   (501) staff       (20)     7026 2023-05-05 00:44:57.000000 intake_dataframe_catalog-0.0.1/tests/test_search.py
--rw-r--r--   0 dougiesquire   (501) staff       (20)    83780 2023-03-27 22:20:51.000000 intake_dataframe_catalog-0.0.1/versioneer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 05:52:13.756201 intake_dataframe_catalog-0.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-05 05:52:05.000000 intake_dataframe_catalog-0.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1490 2023-05-05 05:52:13.756201 intake_dataframe_catalog-0.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3428 2023-05-05 05:52:05.000000 intake_dataframe_catalog-0.0.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      433 2023-05-05 05:52:13.756201 intake_dataframe_catalog-0.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2026 2023-05-05 05:52:05.000000 intake_dataframe_catalog-0.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 05:52:13.756201 intake_dataframe_catalog-0.0.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 05:52:13.756201 intake_dataframe_catalog-0.0.2/src/intake_dataframe_catalog/
+-rw-r--r--   0 runner    (1001) docker     (123)      219 2023-05-05 05:52:05.000000 intake_dataframe_catalog-0.0.2/src/intake_dataframe_catalog/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4127 2023-05-05 05:52:05.000000 intake_dataframe_catalog-0.0.2/src/intake_dataframe_catalog/_search.py
+-rw-r--r--   0 runner    (1001) docker     (123)      497 2023-05-05 05:52:13.756201 intake_dataframe_catalog-0.0.2/src/intake_dataframe_catalog/_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21064 2023-05-05 05:52:05.000000 intake_dataframe_catalog-0.0.2/src/intake_dataframe_catalog/core.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 05:52:13.756201 intake_dataframe_catalog-0.0.2/src/intake_dataframe_catalog.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1490 2023-05-05 05:52:13.000000 intake_dataframe_catalog-0.0.2/src/intake_dataframe_catalog.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      523 2023-05-05 05:52:13.000000 intake_dataframe_catalog-0.0.2/src/intake_dataframe_catalog.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 05:52:13.000000 intake_dataframe_catalog-0.0.2/src/intake_dataframe_catalog.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       75 2023-05-05 05:52:13.000000 intake_dataframe_catalog-0.0.2/src/intake_dataframe_catalog.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-05 05:52:13.000000 intake_dataframe_catalog-0.0.2/src/intake_dataframe_catalog.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-05-05 05:52:13.000000 intake_dataframe_catalog-0.0.2/src/intake_dataframe_catalog.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    83780 2023-05-05 05:52:05.000000 intake_dataframe_catalog-0.0.2/versioneer.py
```

### Comparing `intake_dataframe_catalog-0.0.1/LICENSE` & `intake_dataframe_catalog-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `intake_dataframe_catalog-0.0.1/src/intake_dataframe_catalog/_search.py` & `intake_dataframe_catalog-0.0.2/src/intake_dataframe_catalog/_search.py`

 * *Files identical despite different names*

### Comparing `intake_dataframe_catalog-0.0.1/src/intake_dataframe_catalog/core.py` & `intake_dataframe_catalog-0.0.2/src/intake_dataframe_catalog/core.py`

 * *Files identical despite different names*

### Comparing `intake_dataframe_catalog-0.0.1/src/intake_dataframe_catalog.egg-info/SOURCES.txt` & `intake_dataframe_catalog-0.0.2/src/intake_dataframe_catalog.egg-info/SOURCES.txt`

 * *Files 25% similar despite different names*

```diff
@@ -8,10 +8,8 @@
 src/intake_dataframe_catalog/_version.py
 src/intake_dataframe_catalog/core.py
 src/intake_dataframe_catalog.egg-info/PKG-INFO
 src/intake_dataframe_catalog.egg-info/SOURCES.txt
 src/intake_dataframe_catalog.egg-info/dependency_links.txt
 src/intake_dataframe_catalog.egg-info/entry_points.txt
 src/intake_dataframe_catalog.egg-info/requires.txt
-src/intake_dataframe_catalog.egg-info/top_level.txt
-tests/test_core.py
-tests/test_search.py
+src/intake_dataframe_catalog.egg-info/top_level.txt
```

### Comparing `intake_dataframe_catalog-0.0.1/versioneer.py` & `intake_dataframe_catalog-0.0.2/versioneer.py`

 * *Files identical despite different names*

