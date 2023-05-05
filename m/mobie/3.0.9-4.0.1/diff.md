# Comparing `tmp/mobie-3.0.9.tar.gz` & `tmp/mobie-4.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mobie-3.0.9.tar", last modified: Fri Jan 13 13:45:03 2023, max compression
+gzip compressed data, was "mobie-4.0.1.tar", last modified: Fri May  5 12:25:21 2023, max compression
```

## Comparing `mobie-3.0.9.tar` & `mobie-4.0.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 tischer    (501) staff       (20)        0 2023-01-13 13:45:03.405661 mobie-3.0.9/
--rw-r--r--   0 tischer    (501) staff       (20)     1299 2023-01-13 13:43:12.000000 mobie-3.0.9/LICENSE
--rw-r--r--   0 tischer    (501) staff       (20)      280 2023-01-13 13:45:03.405254 mobie-3.0.9/PKG-INFO
--rw-r--r--   0 tischer    (501) staff       (20)       75 2023-01-13 12:00:34.000000 mobie-3.0.9/README
-drwxr-xr-x   0 tischer    (501) staff       (20)        0 2023-01-13 13:45:03.402100 mobie-3.0.9/mobie/
--rw-r--r--   0 tischer    (501) staff       (20)      530 2023-01-13 13:31:59.000000 mobie-3.0.9/mobie/__init__.py
-drwxr-xr-x   0 tischer    (501) staff       (20)        0 2023-01-13 13:45:03.404796 mobie-3.0.9/mobie.egg-info/
--rw-r--r--   0 tischer    (501) staff       (20)      280 2023-01-13 13:45:03.000000 mobie-3.0.9/mobie.egg-info/PKG-INFO
--rw-r--r--   0 tischer    (501) staff       (20)      217 2023-01-13 13:45:03.000000 mobie-3.0.9/mobie.egg-info/SOURCES.txt
--rw-r--r--   0 tischer    (501) staff       (20)        1 2023-01-13 13:45:03.000000 mobie-3.0.9/mobie.egg-info/dependency_links.txt
--rw-r--r--   0 tischer    (501) staff       (20)       45 2023-01-13 13:45:03.000000 mobie-3.0.9/mobie.egg-info/entry_points.txt
--rw-r--r--   0 tischer    (501) staff       (20)       11 2023-01-13 13:45:03.000000 mobie-3.0.9/mobie.egg-info/requires.txt
--rw-r--r--   0 tischer    (501) staff       (20)        6 2023-01-13 13:45:03.000000 mobie-3.0.9/mobie.egg-info/top_level.txt
--rw-r--r--   0 tischer    (501) staff       (20)       38 2023-01-13 13:45:03.405751 mobie-3.0.9/setup.cfg
--rw-r--r--   0 tischer    (501) staff       (20)      689 2023-01-13 13:34:41.000000 mobie-3.0.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 12:25:21.672637 mobie-4.0.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1299 2023-05-05 12:25:19.000000 mobie-4.0.1/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      468 2023-05-05 12:25:21.672637 mobie-4.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2105 2023-05-05 12:25:19.000000 mobie-4.0.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 12:25:21.668637 mobie-4.0.1/mobie/
+-rw-r--r--   0 runner    (1001) docker     (123)     1413 2023-05-05 12:25:19.000000 mobie-4.0.1/mobie/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 12:25:21.672637 mobie-4.0.1/mobie.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      468 2023-05-05 12:25:21.000000 mobie-4.0.1/mobie.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      224 2023-05-05 12:25:21.000000 mobie-4.0.1/mobie.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 12:25:21.000000 mobie-4.0.1/mobie.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-05 12:25:21.000000 mobie-4.0.1/mobie.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-05 12:25:21.000000 mobie-4.0.1/mobie.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-05 12:25:21.000000 mobie-4.0.1/mobie.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-05 12:25:21.672637 mobie-4.0.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      868 2023-05-05 12:25:19.000000 mobie-4.0.1/setup.py
```

### Comparing `mobie-3.0.9/LICENSE` & `mobie-4.0.1/LICENSE.txt`

 * *Files identical despite different names*

