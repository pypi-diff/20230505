# Comparing `tmp/gpt4all-0.1.3.tar.gz` & `tmp/gpt4all-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gpt4all-0.1.3.tar", last modified: Thu May  4 20:22:51 2023, max compression
+gzip compressed data, was "gpt4all-0.1.4.tar", last modified: Fri May  5 14:29:33 2023, max compression
```

## Comparing `gpt4all-0.1.3.tar` & `gpt4all-0.1.4.tar`

### file list

```diff
@@ -1,20 +1,24 @@
-drwxr-xr-x   0 richardguo   (501) staff       (20)        0 2023-05-04 20:22:51.457099 gpt4all-0.1.3/
--rw-r--r--   0 richardguo   (501) staff       (20)     1054 2023-05-04 16:02:39.000000 gpt4all-0.1.3/LICENSE.txt
--rw-r--r--   0 richardguo   (501) staff       (20)      424 2023-05-04 20:22:51.456955 gpt4all-0.1.3/PKG-INFO
--rw-r--r--   0 richardguo   (501) staff       (20)      987 2023-05-04 16:00:37.000000 gpt4all-0.1.3/README.md
-drwxr-xr-x   0 richardguo   (501) staff       (20)        0 2023-05-04 20:22:51.454529 gpt4all-0.1.3/gpt4all/
--rw-r--r--   0 richardguo   (501) staff       (20)       65 2023-05-03 19:06:54.000000 gpt4all-0.1.3/gpt4all/__init__.py
--rw-r--r--   0 richardguo   (501) staff       (20)     2418 2023-05-03 19:13:41.000000 gpt4all-0.1.3/gpt4all/gpt4all.py
--rw-r--r--   0 richardguo   (501) staff       (20)   285210 2023-05-04 20:22:29.000000 gpt4all-0.1.3/gpt4all/pyllmodel.c
-drwxr-xr-x   0 richardguo   (501) staff       (20)        0 2023-05-04 20:22:51.456120 gpt4all-0.1.3/gpt4all.egg-info/
--rw-r--r--   0 richardguo   (501) staff       (20)      424 2023-05-04 20:22:51.000000 gpt4all-0.1.3/gpt4all.egg-info/PKG-INFO
--rw-r--r--   0 richardguo   (501) staff       (20)      368 2023-05-04 20:22:51.000000 gpt4all-0.1.3/gpt4all.egg-info/SOURCES.txt
--rw-r--r--   0 richardguo   (501) staff       (20)        1 2023-05-04 20:22:51.000000 gpt4all-0.1.3/gpt4all.egg-info/dependency_links.txt
--rw-r--r--   0 richardguo   (501) staff       (20)       30 2023-05-04 20:22:51.000000 gpt4all-0.1.3/gpt4all.egg-info/requires.txt
--rw-r--r--   0 richardguo   (501) staff       (20)       14 2023-05-04 20:22:51.000000 gpt4all-0.1.3/gpt4all.egg-info/top_level.txt
--rw-r--r--   0 richardguo   (501) staff       (20)       38 2023-05-04 20:22:51.457146 gpt4all-0.1.3/setup.cfg
--rw-r--r--   0 richardguo   (501) staff       (20)     1465 2023-05-04 20:21:41.000000 gpt4all-0.1.3/setup.py
-drwxr-xr-x   0 richardguo   (501) staff       (20)        0 2023-05-04 20:22:51.456650 gpt4all-0.1.3/tests/
--rw-r--r--   0 richardguo   (501) staff       (20)        0 2023-05-03 19:03:47.000000 gpt4all-0.1.3/tests/__init__.py
--rw-r--r--   0 richardguo   (501) staff       (20)      687 2023-05-03 19:05:28.000000 gpt4all-0.1.3/tests/test_gpt4all.py
--rw-r--r--   0 richardguo   (501) staff       (20)     1129 2023-05-03 19:05:34.000000 gpt4all-0.1.3/tests/test_pyllmodel.py
+drwxr-xr-x   0 richardguo   (501) staff       (20)        0 2023-05-05 14:29:33.771147 gpt4all-0.1.4/
+-rw-r--r--   0 richardguo   (501) staff       (20)     1054 2023-05-04 16:02:39.000000 gpt4all-0.1.4/LICENSE.txt
+-rw-r--r--   0 richardguo   (501) staff       (20)      424 2023-05-05 14:29:33.770988 gpt4all-0.1.4/PKG-INFO
+-rw-r--r--   0 richardguo   (501) staff       (20)      987 2023-05-04 16:00:37.000000 gpt4all-0.1.4/README.md
+drwxr-xr-x   0 richardguo   (501) staff       (20)        0 2023-05-05 14:29:33.769194 gpt4all-0.1.4/gpt4all/
+-rw-r--r--   0 richardguo   (501) staff       (20)       65 2023-05-03 19:06:54.000000 gpt4all-0.1.4/gpt4all/__init__.py
+-rw-r--r--   0 richardguo   (501) staff       (20)     2418 2023-05-03 19:13:41.000000 gpt4all-0.1.4/gpt4all/gpt4all.py
+-rw-r--r--   0 richardguo   (501) staff       (20)   285210 2023-05-04 20:22:29.000000 gpt4all-0.1.4/gpt4all/pyllmodel.c
+drwxr-xr-x   0 richardguo   (501) staff       (20)        0 2023-05-05 14:29:33.769928 gpt4all-0.1.4/gpt4all.egg-info/
+-rw-r--r--   0 richardguo   (501) staff       (20)      424 2023-05-05 14:29:33.000000 gpt4all-0.1.4/gpt4all.egg-info/PKG-INFO
+-rw-r--r--   0 richardguo   (501) staff       (20)      384 2023-05-05 14:29:33.000000 gpt4all-0.1.4/gpt4all.egg-info/SOURCES.txt
+-rw-r--r--   0 richardguo   (501) staff       (20)        1 2023-05-05 14:29:33.000000 gpt4all-0.1.4/gpt4all.egg-info/dependency_links.txt
+-rw-r--r--   0 richardguo   (501) staff       (20)       30 2023-05-05 14:29:33.000000 gpt4all-0.1.4/gpt4all.egg-info/requires.txt
+-rw-r--r--   0 richardguo   (501) staff       (20)       14 2023-05-05 14:29:33.000000 gpt4all-0.1.4/gpt4all.egg-info/top_level.txt
+drwxr-xr-x   0 richardguo   (501) staff       (20)        0 2023-05-05 14:29:33.770027 gpt4all-0.1.4/llmodel_DO_NOT_MODIFY/
+drwxr-xr-x   0 richardguo   (501) staff       (20)        0 2023-05-05 14:29:33.770130 gpt4all-0.1.4/llmodel_DO_NOT_MODIFY/build/
+-rwxr-xr-x   0 richardguo   (501) staff       (20)   202605 2023-05-01 13:57:50.000000 gpt4all-0.1.4/llmodel_DO_NOT_MODIFY/build/libllmodel.dylib
+-rw-r--r--   0 richardguo   (501) staff       (20)     1553 2023-05-01 03:53:22.000000 gpt4all-0.1.4/llmodel_DO_NOT_MODIFY/llmodel.h
+-rw-r--r--   0 richardguo   (501) staff       (20)       38 2023-05-05 14:29:33.771201 gpt4all-0.1.4/setup.cfg
+-rw-r--r--   0 richardguo   (501) staff       (20)     3161 2023-05-05 14:29:21.000000 gpt4all-0.1.4/setup.py
+drwxr-xr-x   0 richardguo   (501) staff       (20)        0 2023-05-05 14:29:33.770690 gpt4all-0.1.4/tests/
+-rw-r--r--   0 richardguo   (501) staff       (20)        0 2023-05-03 19:03:47.000000 gpt4all-0.1.4/tests/__init__.py
+-rw-r--r--   0 richardguo   (501) staff       (20)      687 2023-05-03 19:05:28.000000 gpt4all-0.1.4/tests/test_gpt4all.py
+-rw-r--r--   0 richardguo   (501) staff       (20)     1129 2023-05-03 19:05:34.000000 gpt4all-0.1.4/tests/test_pyllmodel.py
```

### Comparing `gpt4all-0.1.3/LICENSE.txt` & `gpt4all-0.1.4/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `gpt4all-0.1.3/README.md` & `gpt4all-0.1.4/README.md`

 * *Files identical despite different names*

### Comparing `gpt4all-0.1.3/gpt4all/gpt4all.py` & `gpt4all-0.1.4/gpt4all/gpt4all.py`

 * *Files identical despite different names*

### Comparing `gpt4all-0.1.3/gpt4all/pyllmodel.c` & `gpt4all-0.1.4/gpt4all/pyllmodel.c`

 * *Files identical despite different names*

### Comparing `gpt4all-0.1.3/tests/test_gpt4all.py` & `gpt4all-0.1.4/tests/test_gpt4all.py`

 * *Files identical despite different names*

### Comparing `gpt4all-0.1.3/tests/test_pyllmodel.py` & `gpt4all-0.1.4/tests/test_pyllmodel.py`

 * *Files identical despite different names*

