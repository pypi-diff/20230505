# Comparing `tmp/hyclib-0.1.8.tar.gz` & `tmp/hyclib-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hyclib-0.1.8.tar", last modified: Tue Mar 21 23:21:35 2023, max compression
+gzip compressed data, was "hyclib-0.1.9.tar", last modified: Wed Mar 22 18:51:52 2023, max compression
```

## Comparing `hyclib-0.1.8.tar` & `hyclib-0.1.9.tar`

### file list

```diff
@@ -1,57 +1,57 @@
-drwxr-xr-x   0 hoyinchau   (501) staff       (20)        0 2023-03-21 23:21:35.424204 hyclib-0.1.8/
--rw-r--r--   0 hoyinchau   (501) staff       (20)     1065 2022-11-07 08:10:59.000000 hyclib-0.1.8/LICENSE
--rw-r--r--   0 hoyinchau   (501) staff       (20)     2469 2023-03-21 23:21:35.424004 hyclib-0.1.8/PKG-INFO
--rw-r--r--   0 hoyinchau   (501) staff       (20)      759 2023-03-04 22:36:50.000000 hyclib-0.1.8/README.md
--rw-r--r--   0 hoyinchau   (501) staff       (20)      903 2023-03-21 23:20:57.000000 hyclib-0.1.8/pyproject.toml
--rw-r--r--   0 hoyinchau   (501) staff       (20)       38 2023-03-21 23:21:35.424261 hyclib-0.1.8/setup.cfg
-drwxr-xr-x   0 hoyinchau   (501) staff       (20)        0 2023-03-21 23:21:35.410659 hyclib-0.1.8/src/
-drwxr-xr-x   0 hoyinchau   (501) staff       (20)        0 2023-03-21 23:21:35.416737 hyclib-0.1.8/src/hyclib/
--rw-r--r--   0 hoyinchau   (501) staff       (20)      435 2023-03-20 23:36:22.000000 hyclib-0.1.8/src/hyclib/__init__.py
--rw-r--r--   0 hoyinchau   (501) staff       (20)     3440 2022-11-07 08:10:59.000000 hyclib-0.1.8/src/hyclib/argparse.py
-drwxr-xr-x   0 hoyinchau   (501) staff       (20)        0 2023-03-21 23:21:35.419377 hyclib-0.1.8/src/hyclib/bpd/
--rw-r--r--   0 hoyinchau   (501) staff       (20)       24 2023-02-26 00:25:44.000000 hyclib-0.1.8/src/hyclib/bpd/__init__.py
--rw-r--r--   0 hoyinchau   (501) staff       (20)    12150 2023-03-04 22:42:06.000000 hyclib-0.1.8/src/hyclib/bpd/array.py
--rw-r--r--   0 hoyinchau   (501) staff       (20)    28048 2023-03-04 22:41:05.000000 hyclib-0.1.8/src/hyclib/bpd/dataframe.py
--rw-r--r--   0 hoyinchau   (501) staff       (20)     3260 2023-03-01 07:35:43.000000 hyclib-0.1.8/src/hyclib/bpd/parsing.py
--rw-r--r--   0 hoyinchau   (501) staff       (20)     5258 2023-03-06 19:12:30.000000 hyclib-0.1.8/src/hyclib/config.py
--rw-r--r--   0 hoyinchau   (501) staff       (20)     7342 2023-03-04 22:37:55.000000 hyclib-0.1.8/src/hyclib/configurable.py
--rw-r--r--   0 hoyinchau   (501) staff       (20)      239 2022-11-07 08:10:59.000000 hyclib-0.1.8/src/hyclib/exceptions.py
--rw-r--r--   0 hoyinchau   (501) staff       (20)      798 2023-03-06 00:47:25.000000 hyclib-0.1.8/src/hyclib/functools.py
--rw-r--r--   0 hoyinchau   (501) staff       (20)    13626 2023-02-06 19:26:59.000000 hyclib-0.1.8/src/hyclib/io.py
--rw-r--r--   0 hoyinchau   (501) staff       (20)     5512 2023-03-20 23:47:08.000000 hyclib-0.1.8/src/hyclib/itertools.py
--rw-r--r--   0 hoyinchau   (501) staff       (20)      847 2023-03-06 19:24:15.000000 hyclib-0.1.8/src/hyclib/logging.py
-drwxr-xr-x   0 hoyinchau   (501) staff       (20)        0 2023-03-21 23:21:35.420112 hyclib-0.1.8/src/hyclib/np/
--rw-r--r--   0 hoyinchau   (501) staff       (20)       40 2023-03-20 23:33:57.000000 hyclib-0.1.8/src/hyclib/np/__init__.py
--rw-r--r--   0 hoyinchau   (501) staff       (20)     7750 2023-03-21 22:50:13.000000 hyclib-0.1.8/src/hyclib/np/core.py
--rw-r--r--   0 hoyinchau   (501) staff       (20)     4033 2023-03-21 23:01:48.000000 hyclib-0.1.8/src/hyclib/np/stats.py
--rw-r--r--   0 hoyinchau   (501) staff       (20)     6343 2022-12-31 20:51:27.000000 hyclib-0.1.8/src/hyclib/npf.py
--rw-r--r--   0 hoyinchau   (501) staff       (20)     7203 2023-03-18 18:21:51.000000 hyclib-0.1.8/src/hyclib/pd.py
--rw-r--r--   0 hoyinchau   (501) staff       (20)     7731 2023-03-04 22:39:25.000000 hyclib-0.1.8/src/hyclib/plot.py
--rw-r--r--   0 hoyinchau   (501) staff       (20)      569 2023-01-20 21:29:50.000000 hyclib-0.1.8/src/hyclib/pprint.py
-drwxr-xr-x   0 hoyinchau   (501) staff       (20)        0 2023-03-21 23:21:35.420623 hyclib-0.1.8/src/hyclib/pt/
--rw-r--r--   0 hoyinchau   (501) staff       (20)       60 2023-03-21 23:00:46.000000 hyclib-0.1.8/src/hyclib/pt/__init__.py
--rw-r--r--   0 hoyinchau   (501) staff       (20)    13402 2023-03-21 22:59:57.000000 hyclib-0.1.8/src/hyclib/pt/core.py
--rw-r--r--   0 hoyinchau   (501) staff       (20)     8665 2023-03-21 23:05:14.000000 hyclib-0.1.8/src/hyclib/pt/stats.py
--rw-r--r--   0 hoyinchau   (501) staff       (20)      475 2023-03-06 00:51:56.000000 hyclib-0.1.8/src/hyclib/random.py
-drwxr-xr-x   0 hoyinchau   (501) staff       (20)        0 2023-03-21 23:21:35.421081 hyclib-0.1.8/src/hyclib/sp/
--rw-r--r--   0 hoyinchau   (501) staff       (20)       19 2023-03-20 23:34:33.000000 hyclib-0.1.8/src/hyclib/sp/__init__.py
--rw-r--r--   0 hoyinchau   (501) staff       (20)    16294 2023-03-20 23:34:58.000000 hyclib-0.1.8/src/hyclib/sp/stats.py
--rw-r--r--   0 hoyinchau   (501) staff       (20)     1623 2023-03-06 00:33:18.000000 hyclib-0.1.8/src/hyclib/tempfile.py
--rw-r--r--   0 hoyinchau   (501) staff       (20)      699 2023-02-13 19:46:47.000000 hyclib-0.1.8/src/hyclib/timeit.py
--rw-r--r--   0 hoyinchau   (501) staff       (20)      547 2023-03-06 09:46:19.000000 hyclib-0.1.8/src/hyclib/warnings.py
-drwxr-xr-x   0 hoyinchau   (501) staff       (20)        0 2023-03-21 23:21:35.417915 hyclib-0.1.8/src/hyclib.egg-info/
--rw-r--r--   0 hoyinchau   (501) staff       (20)     2469 2023-03-21 23:21:35.000000 hyclib-0.1.8/src/hyclib.egg-info/PKG-INFO
--rw-r--r--   0 hoyinchau   (501) staff       (20)     1051 2023-03-21 23:21:35.000000 hyclib-0.1.8/src/hyclib.egg-info/SOURCES.txt
--rw-r--r--   0 hoyinchau   (501) staff       (20)        1 2023-03-21 23:21:35.000000 hyclib-0.1.8/src/hyclib.egg-info/dependency_links.txt
--rw-r--r--   0 hoyinchau   (501) staff       (20)       84 2023-03-21 23:21:35.000000 hyclib-0.1.8/src/hyclib.egg-info/requires.txt
--rw-r--r--   0 hoyinchau   (501) staff       (20)        7 2023-03-21 23:21:35.000000 hyclib-0.1.8/src/hyclib.egg-info/top_level.txt
-drwxr-xr-x   0 hoyinchau   (501) staff       (20)        0 2023-03-21 23:21:35.423747 hyclib-0.1.8/test/
--rw-r--r--   0 hoyinchau   (501) staff       (20)     2486 2023-03-04 22:59:07.000000 hyclib-0.1.8/test/test_argparse.py
--rw-r--r--   0 hoyinchau   (501) staff       (20)     1673 2023-03-04 22:59:22.000000 hyclib-0.1.8/test/test_config.py
--rw-r--r--   0 hoyinchau   (501) staff       (20)     1794 2023-03-04 22:59:38.000000 hyclib-0.1.8/test/test_configurable.py
--rw-r--r--   0 hoyinchau   (501) staff       (20)      806 2023-03-04 22:59:59.000000 hyclib-0.1.8/test/test_io.py
--rw-r--r--   0 hoyinchau   (501) staff       (20)     3724 2023-03-06 20:06:59.000000 hyclib-0.1.8/test/test_itertools.py
--rw-r--r--   0 hoyinchau   (501) staff       (20)      250 2023-03-04 23:00:22.000000 hyclib-0.1.8/test/test_logging.py
--rw-r--r--   0 hoyinchau   (501) staff       (20)     6583 2023-03-04 23:00:32.000000 hyclib-0.1.8/test/test_npf.py
--rw-r--r--   0 hoyinchau   (501) staff       (20)      386 2023-03-04 23:00:45.000000 hyclib-0.1.8/test/test_pprint.py
--rw-r--r--   0 hoyinchau   (501) staff       (20)     1170 2023-03-06 09:48:03.000000 hyclib-0.1.8/test/test_random.py
+drwxr-xr-x   0 hoyinchau   (501) staff       (20)        0 2023-03-22 18:51:52.234122 hyclib-0.1.9/
+-rw-r--r--   0 hoyinchau   (501) staff       (20)     1065 2022-11-07 08:10:59.000000 hyclib-0.1.9/LICENSE
+-rw-r--r--   0 hoyinchau   (501) staff       (20)     2469 2023-03-22 18:51:52.233810 hyclib-0.1.9/PKG-INFO
+-rw-r--r--   0 hoyinchau   (501) staff       (20)      759 2023-03-04 22:36:50.000000 hyclib-0.1.9/README.md
+-rw-r--r--   0 hoyinchau   (501) staff       (20)      903 2023-03-22 18:51:38.000000 hyclib-0.1.9/pyproject.toml
+-rw-r--r--   0 hoyinchau   (501) staff       (20)       38 2023-03-22 18:51:52.234199 hyclib-0.1.9/setup.cfg
+drwxr-xr-x   0 hoyinchau   (501) staff       (20)        0 2023-03-22 18:51:52.219254 hyclib-0.1.9/src/
+drwxr-xr-x   0 hoyinchau   (501) staff       (20)        0 2023-03-22 18:51:52.224017 hyclib-0.1.9/src/hyclib/
+-rw-r--r--   0 hoyinchau   (501) staff       (20)      435 2023-03-20 23:36:22.000000 hyclib-0.1.9/src/hyclib/__init__.py
+-rw-r--r--   0 hoyinchau   (501) staff       (20)     3440 2022-11-07 08:10:59.000000 hyclib-0.1.9/src/hyclib/argparse.py
+drwxr-xr-x   0 hoyinchau   (501) staff       (20)        0 2023-03-22 18:51:52.229144 hyclib-0.1.9/src/hyclib/bpd/
+-rw-r--r--   0 hoyinchau   (501) staff       (20)       24 2023-02-26 00:25:44.000000 hyclib-0.1.9/src/hyclib/bpd/__init__.py
+-rw-r--r--   0 hoyinchau   (501) staff       (20)    12150 2023-03-04 22:42:06.000000 hyclib-0.1.9/src/hyclib/bpd/array.py
+-rw-r--r--   0 hoyinchau   (501) staff       (20)    28048 2023-03-04 22:41:05.000000 hyclib-0.1.9/src/hyclib/bpd/dataframe.py
+-rw-r--r--   0 hoyinchau   (501) staff       (20)     3260 2023-03-01 07:35:43.000000 hyclib-0.1.9/src/hyclib/bpd/parsing.py
+-rw-r--r--   0 hoyinchau   (501) staff       (20)     5258 2023-03-06 19:12:30.000000 hyclib-0.1.9/src/hyclib/config.py
+-rw-r--r--   0 hoyinchau   (501) staff       (20)     7342 2023-03-04 22:37:55.000000 hyclib-0.1.9/src/hyclib/configurable.py
+-rw-r--r--   0 hoyinchau   (501) staff       (20)      239 2022-11-07 08:10:59.000000 hyclib-0.1.9/src/hyclib/exceptions.py
+-rw-r--r--   0 hoyinchau   (501) staff       (20)      798 2023-03-06 00:47:25.000000 hyclib-0.1.9/src/hyclib/functools.py
+-rw-r--r--   0 hoyinchau   (501) staff       (20)    13626 2023-02-06 19:26:59.000000 hyclib-0.1.9/src/hyclib/io.py
+-rw-r--r--   0 hoyinchau   (501) staff       (20)     5512 2023-03-20 23:47:08.000000 hyclib-0.1.9/src/hyclib/itertools.py
+-rw-r--r--   0 hoyinchau   (501) staff       (20)      847 2023-03-06 19:24:15.000000 hyclib-0.1.9/src/hyclib/logging.py
+drwxr-xr-x   0 hoyinchau   (501) staff       (20)        0 2023-03-22 18:51:52.229912 hyclib-0.1.9/src/hyclib/np/
+-rw-r--r--   0 hoyinchau   (501) staff       (20)       40 2023-03-20 23:33:57.000000 hyclib-0.1.9/src/hyclib/np/__init__.py
+-rw-r--r--   0 hoyinchau   (501) staff       (20)     7750 2023-03-21 22:50:13.000000 hyclib-0.1.9/src/hyclib/np/core.py
+-rw-r--r--   0 hoyinchau   (501) staff       (20)     4033 2023-03-21 23:01:48.000000 hyclib-0.1.9/src/hyclib/np/stats.py
+-rw-r--r--   0 hoyinchau   (501) staff       (20)     6343 2022-12-31 20:51:27.000000 hyclib-0.1.9/src/hyclib/npf.py
+-rw-r--r--   0 hoyinchau   (501) staff       (20)     7203 2023-03-18 18:21:51.000000 hyclib-0.1.9/src/hyclib/pd.py
+-rw-r--r--   0 hoyinchau   (501) staff       (20)     7731 2023-03-04 22:39:25.000000 hyclib-0.1.9/src/hyclib/plot.py
+-rw-r--r--   0 hoyinchau   (501) staff       (20)      569 2023-01-20 21:29:50.000000 hyclib-0.1.9/src/hyclib/pprint.py
+drwxr-xr-x   0 hoyinchau   (501) staff       (20)        0 2023-03-22 18:51:52.230386 hyclib-0.1.9/src/hyclib/pt/
+-rw-r--r--   0 hoyinchau   (501) staff       (20)       60 2023-03-21 23:00:46.000000 hyclib-0.1.9/src/hyclib/pt/__init__.py
+-rw-r--r--   0 hoyinchau   (501) staff       (20)    13580 2023-03-22 18:49:39.000000 hyclib-0.1.9/src/hyclib/pt/core.py
+-rw-r--r--   0 hoyinchau   (501) staff       (20)     8665 2023-03-21 23:05:14.000000 hyclib-0.1.9/src/hyclib/pt/stats.py
+-rw-r--r--   0 hoyinchau   (501) staff       (20)      475 2023-03-06 00:51:56.000000 hyclib-0.1.9/src/hyclib/random.py
+drwxr-xr-x   0 hoyinchau   (501) staff       (20)        0 2023-03-22 18:51:52.230857 hyclib-0.1.9/src/hyclib/sp/
+-rw-r--r--   0 hoyinchau   (501) staff       (20)       19 2023-03-20 23:34:33.000000 hyclib-0.1.9/src/hyclib/sp/__init__.py
+-rw-r--r--   0 hoyinchau   (501) staff       (20)    16294 2023-03-20 23:34:58.000000 hyclib-0.1.9/src/hyclib/sp/stats.py
+-rw-r--r--   0 hoyinchau   (501) staff       (20)     1623 2023-03-06 00:33:18.000000 hyclib-0.1.9/src/hyclib/tempfile.py
+-rw-r--r--   0 hoyinchau   (501) staff       (20)      699 2023-02-13 19:46:47.000000 hyclib-0.1.9/src/hyclib/timeit.py
+-rw-r--r--   0 hoyinchau   (501) staff       (20)      547 2023-03-06 09:46:19.000000 hyclib-0.1.9/src/hyclib/warnings.py
+drwxr-xr-x   0 hoyinchau   (501) staff       (20)        0 2023-03-22 18:51:52.224808 hyclib-0.1.9/src/hyclib.egg-info/
+-rw-r--r--   0 hoyinchau   (501) staff       (20)     2469 2023-03-22 18:51:52.000000 hyclib-0.1.9/src/hyclib.egg-info/PKG-INFO
+-rw-r--r--   0 hoyinchau   (501) staff       (20)     1051 2023-03-22 18:51:52.000000 hyclib-0.1.9/src/hyclib.egg-info/SOURCES.txt
+-rw-r--r--   0 hoyinchau   (501) staff       (20)        1 2023-03-22 18:51:52.000000 hyclib-0.1.9/src/hyclib.egg-info/dependency_links.txt
+-rw-r--r--   0 hoyinchau   (501) staff       (20)       84 2023-03-22 18:51:52.000000 hyclib-0.1.9/src/hyclib.egg-info/requires.txt
+-rw-r--r--   0 hoyinchau   (501) staff       (20)        7 2023-03-22 18:51:52.000000 hyclib-0.1.9/src/hyclib.egg-info/top_level.txt
+drwxr-xr-x   0 hoyinchau   (501) staff       (20)        0 2023-03-22 18:51:52.233493 hyclib-0.1.9/test/
+-rw-r--r--   0 hoyinchau   (501) staff       (20)     2486 2023-03-04 22:59:07.000000 hyclib-0.1.9/test/test_argparse.py
+-rw-r--r--   0 hoyinchau   (501) staff       (20)     1673 2023-03-04 22:59:22.000000 hyclib-0.1.9/test/test_config.py
+-rw-r--r--   0 hoyinchau   (501) staff       (20)     1794 2023-03-04 22:59:38.000000 hyclib-0.1.9/test/test_configurable.py
+-rw-r--r--   0 hoyinchau   (501) staff       (20)      806 2023-03-04 22:59:59.000000 hyclib-0.1.9/test/test_io.py
+-rw-r--r--   0 hoyinchau   (501) staff       (20)     3724 2023-03-06 20:06:59.000000 hyclib-0.1.9/test/test_itertools.py
+-rw-r--r--   0 hoyinchau   (501) staff       (20)      250 2023-03-04 23:00:22.000000 hyclib-0.1.9/test/test_logging.py
+-rw-r--r--   0 hoyinchau   (501) staff       (20)     6583 2023-03-04 23:00:32.000000 hyclib-0.1.9/test/test_npf.py
+-rw-r--r--   0 hoyinchau   (501) staff       (20)      386 2023-03-04 23:00:45.000000 hyclib-0.1.9/test/test_pprint.py
+-rw-r--r--   0 hoyinchau   (501) staff       (20)     1170 2023-03-06 09:48:03.000000 hyclib-0.1.9/test/test_random.py
```

### Comparing `hyclib-0.1.8/LICENSE` & `hyclib-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `hyclib-0.1.8/PKG-INFO` & `hyclib-0.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hyclib
-Version: 0.1.8
+Version: 0.1.9
 Summary: Commonly used tools across my own personal projects.
 Author: Ho Yin Chau
 License: MIT License
         
         Copyright (c) 2022 hchau630
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `hyclib-0.1.8/README.md` & `hyclib-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `hyclib-0.1.8/pyproject.toml` & `hyclib-0.1.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=64.0"] # editable install using setuptool available since v64.0.0
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "hyclib"
-version = "0.1.8"
+version = "0.1.9"
 description = "Commonly used tools across my own personal projects."
 readme = "README.md"
 requires-python = ">=3.9" # package developed with python v3.9.16
 license = {file = "LICENSE"}
 authors = [
     {name = "Ho Yin Chau"},
 ]
```

### Comparing `hyclib-0.1.8/src/hyclib/argparse.py` & `hyclib-0.1.9/src/hyclib/argparse.py`

 * *Files identical despite different names*

### Comparing `hyclib-0.1.8/src/hyclib/bpd/array.py` & `hyclib-0.1.9/src/hyclib/bpd/array.py`

 * *Files identical despite different names*

### Comparing `hyclib-0.1.8/src/hyclib/bpd/dataframe.py` & `hyclib-0.1.9/src/hyclib/bpd/dataframe.py`

 * *Files identical despite different names*

### Comparing `hyclib-0.1.8/src/hyclib/bpd/parsing.py` & `hyclib-0.1.9/src/hyclib/bpd/parsing.py`

 * *Files identical despite different names*

### Comparing `hyclib-0.1.8/src/hyclib/config.py` & `hyclib-0.1.9/src/hyclib/config.py`

 * *Files identical despite different names*

### Comparing `hyclib-0.1.8/src/hyclib/configurable.py` & `hyclib-0.1.9/src/hyclib/configurable.py`

 * *Files identical despite different names*

### Comparing `hyclib-0.1.8/src/hyclib/functools.py` & `hyclib-0.1.9/src/hyclib/functools.py`

 * *Files identical despite different names*

### Comparing `hyclib-0.1.8/src/hyclib/io.py` & `hyclib-0.1.9/src/hyclib/io.py`

 * *Files identical despite different names*

### Comparing `hyclib-0.1.8/src/hyclib/itertools.py` & `hyclib-0.1.9/src/hyclib/itertools.py`

 * *Files identical despite different names*

### Comparing `hyclib-0.1.8/src/hyclib/logging.py` & `hyclib-0.1.9/src/hyclib/logging.py`

 * *Files identical despite different names*

### Comparing `hyclib-0.1.8/src/hyclib/np/core.py` & `hyclib-0.1.9/src/hyclib/np/core.py`

 * *Files identical despite different names*

### Comparing `hyclib-0.1.8/src/hyclib/np/stats.py` & `hyclib-0.1.9/src/hyclib/np/stats.py`

 * *Files identical despite different names*

### Comparing `hyclib-0.1.8/src/hyclib/npf.py` & `hyclib-0.1.9/src/hyclib/npf.py`

 * *Files identical despite different names*

### Comparing `hyclib-0.1.8/src/hyclib/pd.py` & `hyclib-0.1.9/src/hyclib/pd.py`

 * *Files identical despite different names*

### Comparing `hyclib-0.1.8/src/hyclib/plot.py` & `hyclib-0.1.9/src/hyclib/plot.py`

 * *Files identical despite different names*

### Comparing `hyclib-0.1.8/src/hyclib/pprint.py` & `hyclib-0.1.9/src/hyclib/pprint.py`

 * *Files identical despite different names*

### Comparing `hyclib-0.1.8/src/hyclib/pt/core.py` & `hyclib-0.1.9/src/hyclib/pt/core.py`

 * *Files 2% similar despite different names*

```diff
@@ -100,15 +100,18 @@
     x = x.movedim(dim, 0)
     shape = x.shape
     x = x.reshape(shape[0], -1)
     
     # separate rows with nans from rows without nans and only compute unique on rows without nans.
     # This avoids torch.unique bug when dim is not None and input has nan.
     isnan = x.isnan().any(dim=1)
-    x_not_isnan, x_isnan = x[~isnan], x[isnan]
+    if not isnan.any():
+        x_not_isnan, x_isnan = x, torch.empty((0, x.shape[1]), dtype=x.dtype, device=x.device) # slighty optimization to prevent large copy
+    else:
+        x_not_isnan, x_isnan = x[~isnan], x[isnan]
     N_not_isnan = len(x_not_isnan)
 
     if return_index:
         # code copied from https://github.com/pytorch/pytorch/issues/36748#issuecomment-1474368922
         x_not_isnan, inverse, counts = torch.unique(x_not_isnan, dim=0, return_inverse=True, return_counts=True)
         inv_sort_idx = inverse.argsort(stable=True)
         tot_counts = torch.cat((counts.new_zeros(1), counts.cumsum(dim=0)))[:-1]
```

### Comparing `hyclib-0.1.8/src/hyclib/pt/stats.py` & `hyclib-0.1.9/src/hyclib/pt/stats.py`

 * *Files identical despite different names*

### Comparing `hyclib-0.1.8/src/hyclib/sp/stats.py` & `hyclib-0.1.9/src/hyclib/sp/stats.py`

 * *Files identical despite different names*

### Comparing `hyclib-0.1.8/src/hyclib/tempfile.py` & `hyclib-0.1.9/src/hyclib/tempfile.py`

 * *Files identical despite different names*

### Comparing `hyclib-0.1.8/src/hyclib/timeit.py` & `hyclib-0.1.9/src/hyclib/timeit.py`

 * *Files identical despite different names*

### Comparing `hyclib-0.1.8/src/hyclib/warnings.py` & `hyclib-0.1.9/src/hyclib/warnings.py`

 * *Files identical despite different names*

### Comparing `hyclib-0.1.8/src/hyclib.egg-info/PKG-INFO` & `hyclib-0.1.9/src/hyclib.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hyclib
-Version: 0.1.8
+Version: 0.1.9
 Summary: Commonly used tools across my own personal projects.
 Author: Ho Yin Chau
 License: MIT License
         
         Copyright (c) 2022 hchau630
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `hyclib-0.1.8/src/hyclib.egg-info/SOURCES.txt` & `hyclib-0.1.9/src/hyclib.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `hyclib-0.1.8/test/test_argparse.py` & `hyclib-0.1.9/test/test_argparse.py`

 * *Files identical despite different names*

### Comparing `hyclib-0.1.8/test/test_config.py` & `hyclib-0.1.9/test/test_config.py`

 * *Files identical despite different names*

### Comparing `hyclib-0.1.8/test/test_configurable.py` & `hyclib-0.1.9/test/test_configurable.py`

 * *Files identical despite different names*

### Comparing `hyclib-0.1.8/test/test_io.py` & `hyclib-0.1.9/test/test_io.py`

 * *Files identical despite different names*

### Comparing `hyclib-0.1.8/test/test_itertools.py` & `hyclib-0.1.9/test/test_itertools.py`

 * *Files identical despite different names*

### Comparing `hyclib-0.1.8/test/test_npf.py` & `hyclib-0.1.9/test/test_npf.py`

 * *Files identical despite different names*

### Comparing `hyclib-0.1.8/test/test_random.py` & `hyclib-0.1.9/test/test_random.py`

 * *Files identical despite different names*

