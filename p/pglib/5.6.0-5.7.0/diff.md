# Comparing `tmp/pglib-5.6.0.tar.gz` & `tmp/pglib-5.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pglib-5.6.0.tar", last modified: Thu Mar 30 18:58:37 2023, max compression
+gzip compressed data, was "pglib-5.7.0.tar", last modified: Fri May  5 15:22:41 2023, max compression
```

## Comparing `pglib-5.6.0.tar` & `pglib-5.7.0.tar`

### file list

```diff
@@ -1,58 +1,57 @@
-drwxrwxr-x   0 mkleehammer  (1000) mkleehammer  (1000)        0 2023-03-30 18:58:37.156999 pglib-5.6.0/
--rw-rw-r--   0 mkleehammer  (1000) mkleehammer  (1000)     1075 2021-04-30 17:17:45.000000 pglib-5.6.0/LICENSE
--rw-rw-r--   0 mkleehammer  (1000) mkleehammer  (1000)      101 2021-04-30 17:17:45.000000 pglib-5.6.0/MANIFEST.in
--rw-rw-r--   0 mkleehammer  (1000) mkleehammer  (1000)      753 2023-03-30 18:58:37.156999 pglib-5.6.0/PKG-INFO
--rw-rw-r--   0 mkleehammer  (1000) mkleehammer  (1000)      509 2021-04-30 17:17:45.000000 pglib-5.6.0/README.rst
-drwxrwxr-x   0 mkleehammer  (1000) mkleehammer  (1000)        0 2023-03-30 18:58:37.156999 pglib-5.6.0/pglib/
--rw-rw-r--   0 mkleehammer  (1000) mkleehammer  (1000)      264 2021-04-30 17:17:45.000000 pglib-5.6.0/pglib/__init__.py
--rw-rw-r--   0 mkleehammer  (1000) mkleehammer  (1000)      471 2023-03-30 18:58:37.156999 pglib-5.6.0/pglib/_version.py
--rw-rw-r--   0 mkleehammer  (1000) mkleehammer  (1000)     9969 2022-07-23 05:57:37.000000 pglib-5.6.0/pglib/asyncpglib.py
-drwxrwxr-x   0 mkleehammer  (1000) mkleehammer  (1000)        0 2023-03-30 18:58:37.152999 pglib-5.6.0/pglib.egg-info/
--rw-rw-r--   0 mkleehammer  (1000) mkleehammer  (1000)      753 2023-03-30 18:58:37.000000 pglib-5.6.0/pglib.egg-info/PKG-INFO
--rw-rw-r--   0 mkleehammer  (1000) mkleehammer  (1000)     1613 2023-03-30 18:58:37.000000 pglib-5.6.0/pglib.egg-info/SOURCES.txt
--rw-rw-r--   0 mkleehammer  (1000) mkleehammer  (1000)        1 2023-03-30 18:58:37.000000 pglib-5.6.0/pglib.egg-info/dependency_links.txt
--rw-rw-r--   0 mkleehammer  (1000) mkleehammer  (1000)       13 2023-03-30 18:58:37.000000 pglib-5.6.0/pglib.egg-info/top_level.txt
--rw-rw-r--   0 mkleehammer  (1000) mkleehammer  (1000)      225 2023-03-30 18:58:37.156999 pglib-5.6.0/setup.cfg
--rwxrwxr-x   0 mkleehammer  (1000) mkleehammer  (1000)     5260 2022-07-05 15:04:07.000000 pglib-5.6.0/setup.py
-drwxrwxr-x   0 mkleehammer  (1000) mkleehammer  (1000)        0 2023-03-30 18:58:37.156999 pglib-5.6.0/src/
--rw-rw-r--   0 mkleehammer  (1000) mkleehammer  (1000)     1628 2021-04-30 17:17:45.000000 pglib-5.6.0/src/byteswap.h
--rw-rw-r--   0 mkleehammer  (1000) mkleehammer  (1000)    39610 2023-03-30 18:57:20.000000 pglib-5.6.0/src/connection.cpp
--rw-rw-r--   0 mkleehammer  (1000) mkleehammer  (1000)      764 2022-07-23 04:49:54.000000 pglib-5.6.0/src/connection.h
--rw-rw-r--   0 mkleehammer  (1000) mkleehammer  (1000)      540 2022-07-23 05:46:16.000000 pglib-5.6.0/src/conninfoopt.cpp
--rw-rw-r--   0 mkleehammer  (1000) mkleehammer  (1000)      353 2022-07-23 05:38:59.000000 pglib-5.6.0/src/conninfoopt.h
--rw-rw-r--   0 mkleehammer  (1000) mkleehammer  (1000)     1494 2021-04-30 17:17:45.000000 pglib-5.6.0/src/datatypes.cpp
--rw-rw-r--   0 mkleehammer  (1000) mkleehammer  (1000)      452 2021-04-30 17:17:45.000000 pglib-5.6.0/src/datatypes.h
--rw-rw-r--   0 mkleehammer  (1000) mkleehammer  (1000)      385 2021-04-30 17:17:45.000000 pglib-5.6.0/src/debug.cpp
--rw-rw-r--   0 mkleehammer  (1000) mkleehammer  (1000)       93 2021-04-30 17:17:45.000000 pglib-5.6.0/src/debug.h
--rw-rw-r--   0 mkleehammer  (1000) mkleehammer  (1000)      587 2021-04-30 17:17:45.000000 pglib-5.6.0/src/enums.cpp
--rw-rw-r--   0 mkleehammer  (1000) mkleehammer  (1000)       51 2021-04-30 17:17:45.000000 pglib-5.6.0/src/enums.h
--rw-rw-r--   0 mkleehammer  (1000) mkleehammer  (1000)     2867 2022-07-23 04:49:54.000000 pglib-5.6.0/src/errors.cpp
--rw-rw-r--   0 mkleehammer  (1000) mkleehammer  (1000)      347 2021-04-30 17:17:45.000000 pglib-5.6.0/src/errors.h
--rw-rw-r--   0 mkleehammer  (1000) mkleehammer  (1000)    10101 2022-07-23 05:55:49.000000 pglib-5.6.0/src/getdata.cpp
--rw-rw-r--   0 mkleehammer  (1000) mkleehammer  (1000)      178 2021-04-30 17:17:45.000000 pglib-5.6.0/src/getdata.h
--rw-rw-r--   0 mkleehammer  (1000) mkleehammer  (1000)     1613 2021-04-30 17:17:45.000000 pglib-5.6.0/src/juliandate.cpp
--rw-rw-r--   0 mkleehammer  (1000) mkleehammer  (1000)      239 2021-04-30 17:17:45.000000 pglib-5.6.0/src/juliandate.h
--rw-rw-r--   0 mkleehammer  (1000) mkleehammer  (1000)    15639 2022-09-24 04:45:37.000000 pglib-5.6.0/src/params.cpp
--rw-rw-r--   0 mkleehammer  (1000) mkleehammer  (1000)     3250 2021-04-30 17:17:45.000000 pglib-5.6.0/src/params.h
--rw-rw-r--   0 mkleehammer  (1000) mkleehammer  (1000)    13847 2021-04-30 17:17:45.000000 pglib-5.6.0/src/pgarrays.cpp
--rw-rw-r--   0 mkleehammer  (1000) mkleehammer  (1000)      362 2021-04-30 17:17:45.000000 pglib-5.6.0/src/pgarrays.h
--rw-rw-r--   0 mkleehammer  (1000) mkleehammer  (1000)     7182 2022-09-24 04:36:59.000000 pglib-5.6.0/src/pglib.cpp
--rw-rw-r--   0 mkleehammer  (1000) mkleehammer  (1000)     5541 2022-07-23 04:49:54.000000 pglib-5.6.0/src/pglib.h
--rw-rw-r--   0 mkleehammer  (1000) mkleehammer  (1000)      196 2021-04-30 17:17:45.000000 pglib-5.6.0/src/pgtypes.h
--rw-rw-r--   0 mkleehammer  (1000) mkleehammer  (1000)     7959 2021-04-30 17:17:45.000000 pglib-5.6.0/src/resultset.cpp
--rw-rw-r--   0 mkleehammer  (1000) mkleehammer  (1000)     1033 2021-04-30 17:17:45.000000 pglib-5.6.0/src/resultset.h
--rw-rw-r--   0 mkleehammer  (1000) mkleehammer  (1000)    12377 2021-04-30 17:17:45.000000 pglib-5.6.0/src/row.cpp
--rw-rw-r--   0 mkleehammer  (1000) mkleehammer  (1000)      432 2021-04-30 17:17:45.000000 pglib-5.6.0/src/row.h
--rw-rw-r--   0 mkleehammer  (1000) mkleehammer  (1000)     2421 2021-04-30 17:17:45.000000 pglib-5.6.0/src/runtime.cpp
--rw-rw-r--   0 mkleehammer  (1000) mkleehammer  (1000)       58 2021-04-30 17:17:45.000000 pglib-5.6.0/src/runtime.h
--rw-rw-r--   0 mkleehammer  (1000) mkleehammer  (1000)     4098 2022-07-23 05:00:28.000000 pglib-5.6.0/src/type_hstore.cpp
--rw-rw-r--   0 mkleehammer  (1000) mkleehammer  (1000)      387 2022-07-23 05:00:42.000000 pglib-5.6.0/src/type_hstore.h
--rw-rw-r--   0 mkleehammer  (1000) mkleehammer  (1000)     2703 2022-09-24 04:42:40.000000 pglib-5.6.0/src/type_json.cpp
--rw-rw-r--   0 mkleehammer  (1000) mkleehammer  (1000)      238 2022-09-24 04:42:23.000000 pglib-5.6.0/src/type_json.h
--rw-rw-r--   0 mkleehammer  (1000) mkleehammer  (1000)      627 2022-07-23 05:56:05.000000 pglib-5.6.0/src/type_ltree.cpp
--rw-rw-r--   0 mkleehammer  (1000) mkleehammer  (1000)      133 2022-07-23 05:50:42.000000 pglib-5.6.0/src/type_ltree.h
-drwxrwxr-x   0 mkleehammer  (1000) mkleehammer  (1000)        0 2023-03-30 18:58:37.156999 pglib-5.6.0/test/
--rw-rw-r--   0 mkleehammer  (1000) mkleehammer  (1000)     4469 2021-04-30 17:17:45.000000 pglib-5.6.0/test/test_async.py
--rw-rw-r--   0 mkleehammer  (1000) mkleehammer  (1000)    34582 2023-03-30 18:56:55.000000 pglib-5.6.0/test/test_sync.py
--rw-rw-r--   0 mkleehammer  (1000) mkleehammer  (1000)     2096 2021-04-30 17:17:45.000000 pglib-5.6.0/test/testutils.py
--rw-rw-r--   0 mkleehammer  (1000) mkleehammer  (1000)    65747 2021-04-30 17:17:45.000000 pglib-5.6.0/versioneer.py
+drwxrwxr-x   0 mkleehammer  (1000) mkleehammer  (1000)        0 2023-05-05 15:22:41.709025 pglib-5.7.0/
+-rw-rw-r--   0 mkleehammer  (1000) mkleehammer  (1000)     1075 2021-04-30 17:17:45.000000 pglib-5.7.0/LICENSE
+-rw-rw-r--   0 mkleehammer  (1000) mkleehammer  (1000)      101 2021-04-30 17:17:45.000000 pglib-5.7.0/MANIFEST.in
+-rw-rw-r--   0 mkleehammer  (1000) mkleehammer  (1000)      753 2023-05-05 15:22:41.709025 pglib-5.7.0/PKG-INFO
+-rw-rw-r--   0 mkleehammer  (1000) mkleehammer  (1000)      509 2021-04-30 17:17:45.000000 pglib-5.7.0/README.rst
+drwxrwxr-x   0 mkleehammer  (1000) mkleehammer  (1000)        0 2023-05-05 15:22:41.705025 pglib-5.7.0/pglib/
+-rw-rw-r--   0 mkleehammer  (1000) mkleehammer  (1000)      264 2021-04-30 17:17:45.000000 pglib-5.7.0/pglib/__init__.py
+-rw-rw-r--   0 mkleehammer  (1000) mkleehammer  (1000)    16739 2021-04-30 17:17:45.000000 pglib-5.7.0/pglib/_version.py
+-rw-rw-r--   0 mkleehammer  (1000) mkleehammer  (1000)     9969 2022-07-23 05:57:37.000000 pglib-5.7.0/pglib/asyncpglib.py
+drwxrwxr-x   0 mkleehammer  (1000) mkleehammer  (1000)        0 2023-05-05 15:22:41.705025 pglib-5.7.0/pglib.egg-info/
+-rw-rw-r--   0 mkleehammer  (1000) mkleehammer  (1000)      753 2023-05-05 15:22:41.000000 pglib-5.7.0/pglib.egg-info/PKG-INFO
+-rw-rw-r--   0 mkleehammer  (1000) mkleehammer  (1000)     1599 2023-05-05 15:22:41.000000 pglib-5.7.0/pglib.egg-info/SOURCES.txt
+-rw-rw-r--   0 mkleehammer  (1000) mkleehammer  (1000)        1 2023-05-05 15:22:41.000000 pglib-5.7.0/pglib.egg-info/dependency_links.txt
+-rw-rw-r--   0 mkleehammer  (1000) mkleehammer  (1000)       13 2023-05-05 15:22:41.000000 pglib-5.7.0/pglib.egg-info/top_level.txt
+-rw-rw-r--   0 mkleehammer  (1000) mkleehammer  (1000)       95 2023-05-05 15:22:41.713025 pglib-5.7.0/setup.cfg
+-rwxrwxr-x   0 mkleehammer  (1000) mkleehammer  (1000)     5147 2023-05-05 15:20:34.000000 pglib-5.7.0/setup.py
+drwxrwxr-x   0 mkleehammer  (1000) mkleehammer  (1000)        0 2023-05-05 15:22:41.709025 pglib-5.7.0/src/
+-rw-rw-r--   0 mkleehammer  (1000) mkleehammer  (1000)     1628 2021-04-30 17:17:45.000000 pglib-5.7.0/src/byteswap.h
+-rw-rw-r--   0 mkleehammer  (1000) mkleehammer  (1000)    44407 2023-05-05 15:14:30.000000 pglib-5.7.0/src/connection.cpp
+-rw-rw-r--   0 mkleehammer  (1000) mkleehammer  (1000)      764 2022-07-23 04:49:54.000000 pglib-5.7.0/src/connection.h
+-rw-rw-r--   0 mkleehammer  (1000) mkleehammer  (1000)      540 2022-07-23 05:46:16.000000 pglib-5.7.0/src/conninfoopt.cpp
+-rw-rw-r--   0 mkleehammer  (1000) mkleehammer  (1000)      353 2022-07-23 05:38:59.000000 pglib-5.7.0/src/conninfoopt.h
+-rw-rw-r--   0 mkleehammer  (1000) mkleehammer  (1000)     1494 2021-04-30 17:17:45.000000 pglib-5.7.0/src/datatypes.cpp
+-rw-rw-r--   0 mkleehammer  (1000) mkleehammer  (1000)      452 2021-04-30 17:17:45.000000 pglib-5.7.0/src/datatypes.h
+-rw-rw-r--   0 mkleehammer  (1000) mkleehammer  (1000)      385 2021-04-30 17:17:45.000000 pglib-5.7.0/src/debug.cpp
+-rw-rw-r--   0 mkleehammer  (1000) mkleehammer  (1000)       93 2021-04-30 17:17:45.000000 pglib-5.7.0/src/debug.h
+-rw-rw-r--   0 mkleehammer  (1000) mkleehammer  (1000)      587 2021-04-30 17:17:45.000000 pglib-5.7.0/src/enums.cpp
+-rw-rw-r--   0 mkleehammer  (1000) mkleehammer  (1000)       51 2021-04-30 17:17:45.000000 pglib-5.7.0/src/enums.h
+-rw-rw-r--   0 mkleehammer  (1000) mkleehammer  (1000)     2867 2022-07-23 04:49:54.000000 pglib-5.7.0/src/errors.cpp
+-rw-rw-r--   0 mkleehammer  (1000) mkleehammer  (1000)      347 2021-04-30 17:17:45.000000 pglib-5.7.0/src/errors.h
+-rw-rw-r--   0 mkleehammer  (1000) mkleehammer  (1000)    10101 2022-07-23 05:55:49.000000 pglib-5.7.0/src/getdata.cpp
+-rw-rw-r--   0 mkleehammer  (1000) mkleehammer  (1000)      178 2021-04-30 17:17:45.000000 pglib-5.7.0/src/getdata.h
+-rw-rw-r--   0 mkleehammer  (1000) mkleehammer  (1000)     1613 2021-04-30 17:17:45.000000 pglib-5.7.0/src/juliandate.cpp
+-rw-rw-r--   0 mkleehammer  (1000) mkleehammer  (1000)      239 2021-04-30 17:17:45.000000 pglib-5.7.0/src/juliandate.h
+-rw-rw-r--   0 mkleehammer  (1000) mkleehammer  (1000)    15639 2022-09-24 04:45:37.000000 pglib-5.7.0/src/params.cpp
+-rw-rw-r--   0 mkleehammer  (1000) mkleehammer  (1000)     3250 2021-04-30 17:17:45.000000 pglib-5.7.0/src/params.h
+-rw-rw-r--   0 mkleehammer  (1000) mkleehammer  (1000)    13847 2021-04-30 17:17:45.000000 pglib-5.7.0/src/pgarrays.cpp
+-rw-rw-r--   0 mkleehammer  (1000) mkleehammer  (1000)      362 2021-04-30 17:17:45.000000 pglib-5.7.0/src/pgarrays.h
+-rw-rw-r--   0 mkleehammer  (1000) mkleehammer  (1000)     7182 2022-09-24 04:36:59.000000 pglib-5.7.0/src/pglib.cpp
+-rw-rw-r--   0 mkleehammer  (1000) mkleehammer  (1000)     5541 2022-07-23 04:49:54.000000 pglib-5.7.0/src/pglib.h
+-rw-rw-r--   0 mkleehammer  (1000) mkleehammer  (1000)      196 2021-04-30 17:17:45.000000 pglib-5.7.0/src/pgtypes.h
+-rw-rw-r--   0 mkleehammer  (1000) mkleehammer  (1000)     7959 2021-04-30 17:17:45.000000 pglib-5.7.0/src/resultset.cpp
+-rw-rw-r--   0 mkleehammer  (1000) mkleehammer  (1000)     1033 2021-04-30 17:17:45.000000 pglib-5.7.0/src/resultset.h
+-rw-rw-r--   0 mkleehammer  (1000) mkleehammer  (1000)    12377 2021-04-30 17:17:45.000000 pglib-5.7.0/src/row.cpp
+-rw-rw-r--   0 mkleehammer  (1000) mkleehammer  (1000)      432 2021-04-30 17:17:45.000000 pglib-5.7.0/src/row.h
+-rw-rw-r--   0 mkleehammer  (1000) mkleehammer  (1000)     2421 2021-04-30 17:17:45.000000 pglib-5.7.0/src/runtime.cpp
+-rw-rw-r--   0 mkleehammer  (1000) mkleehammer  (1000)       58 2021-04-30 17:17:45.000000 pglib-5.7.0/src/runtime.h
+-rw-rw-r--   0 mkleehammer  (1000) mkleehammer  (1000)     4098 2022-07-23 05:00:28.000000 pglib-5.7.0/src/type_hstore.cpp
+-rw-rw-r--   0 mkleehammer  (1000) mkleehammer  (1000)      387 2022-07-23 05:00:42.000000 pglib-5.7.0/src/type_hstore.h
+-rw-rw-r--   0 mkleehammer  (1000) mkleehammer  (1000)     2703 2022-09-24 04:42:40.000000 pglib-5.7.0/src/type_json.cpp
+-rw-rw-r--   0 mkleehammer  (1000) mkleehammer  (1000)      238 2022-09-24 04:42:23.000000 pglib-5.7.0/src/type_json.h
+-rw-rw-r--   0 mkleehammer  (1000) mkleehammer  (1000)      627 2022-07-23 05:56:05.000000 pglib-5.7.0/src/type_ltree.cpp
+-rw-rw-r--   0 mkleehammer  (1000) mkleehammer  (1000)      133 2022-07-23 05:50:42.000000 pglib-5.7.0/src/type_ltree.h
+drwxrwxr-x   0 mkleehammer  (1000) mkleehammer  (1000)        0 2023-05-05 15:22:41.709025 pglib-5.7.0/test/
+-rw-rw-r--   0 mkleehammer  (1000) mkleehammer  (1000)     4469 2021-04-30 17:17:45.000000 pglib-5.7.0/test/test_async.py
+-rw-rw-r--   0 mkleehammer  (1000) mkleehammer  (1000)    34977 2023-05-05 15:17:33.000000 pglib-5.7.0/test/test_sync.py
+-rw-rw-r--   0 mkleehammer  (1000) mkleehammer  (1000)     2096 2021-04-30 17:17:45.000000 pglib-5.7.0/test/testutils.py
```

### Comparing `pglib-5.6.0/LICENSE` & `pglib-5.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pglib-5.6.0/PKG-INFO` & `pglib-5.7.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pglib
-Version: 5.6.0
+Version: 5.7.0
 Summary: A PostgreSQL interface
 Home-page: https://gitlab.com/mkleehammer/pglib
 Maintainer: Michael Kleehammer
 Maintainer-email: michael@kleehammer.com
 License: MIT
 Keywords: postgresql postgres
 Platform: UNKNOWN
```

### Comparing `pglib-5.6.0/pglib/asyncpglib.py` & `pglib-5.7.0/pglib/asyncpglib.py`

 * *Files identical despite different names*

### Comparing `pglib-5.6.0/pglib.egg-info/PKG-INFO` & `pglib-5.7.0/pglib.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pglib
-Version: 5.6.0
+Version: 5.7.0
 Summary: A PostgreSQL interface
 Home-page: https://gitlab.com/mkleehammer/pglib
 Maintainer: Michael Kleehammer
 Maintainer-email: michael@kleehammer.com
 License: MIT
 Keywords: postgresql postgres
 Platform: UNKNOWN
```

### Comparing `pglib-5.6.0/pglib.egg-info/SOURCES.txt` & `pglib-5.7.0/pglib.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,12 @@
 LICENSE
 MANIFEST.in
 README.rst
 setup.cfg
 setup.py
-versioneer.py
 /home/mkleehammer/dev/pglib/src/connection.cpp
 /home/mkleehammer/dev/pglib/src/conninfoopt.cpp
 /home/mkleehammer/dev/pglib/src/datatypes.cpp
 /home/mkleehammer/dev/pglib/src/debug.cpp
 /home/mkleehammer/dev/pglib/src/enums.cpp
 /home/mkleehammer/dev/pglib/src/errors.cpp
 /home/mkleehammer/dev/pglib/src/getdata.cpp
```

### Comparing `pglib-5.6.0/setup.py` & `pglib-5.7.0/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,15 +1,13 @@
 #!/usr/bin/env python3
 
 import sys, os, re
 import subprocess, sysconfig
 from os.path import join, abspath, dirname
 
-import versioneer
-
 try:
     from setuptools import setup, Extension
 except:
     from distutils.core import setup, Extension
 
 long_description = """\
 A PostgreSQL interface for Python.
@@ -29,15 +27,15 @@
 
     output = subprocess.check_output(['xcodebuild', '-version', '-sdk']).strip().decode('utf-8')
 
     highest = (0, 0)
     path    = None
 
     # MacOSX10.8.sdk - OS X 10.8 (macosx10.8)
-    resection = re.compile('^.*- (?:OS X|macOS) (\d+)\.(\d+)')
+    resection = re.compile(r'^.*- (?:OS X|macOS) (\d+)\.(\d+)')
     repath = re.compile('^Path: ([^\n]+)', re.MULTILINE)
 
     for section in output.split('\n\n'):
         match = resection.match(section)
         if not match:
             continue
 
@@ -128,24 +126,22 @@
         settings['extra_compile_args'] = ['-Wno-write-strings']
 
     return settings
 
 
 setup(
     name='pglib',
-    version=versioneer.get_version(),
+    version='5.7.0',
     description='A PostgreSQL interface',
     long_description=long_description,
     maintainer='Michael Kleehammer',
     maintainer_email='michael@kleehammer.com',
     packages=['pglib'],
     ext_modules=[Extension('_pglib', _get_files(), **_get_settings())],
-    cmdclass=versioneer.get_cmdclass(),
     keywords='postgresql postgres',
-    setup_requires=['pytest-runner'],
     tests_require=['pytest'],
     url='https://gitlab.com/mkleehammer/pglib',
     license='MIT',
     classifiers=[
         # https://pypi.python.org/pypi?%3Aaction=list_classifiers
         'Development Status :: 5 - Production/Stable',
         'Intended Audience :: Developers',
```

### Comparing `pglib-5.6.0/src/byteswap.h` & `pglib-5.7.0/src/byteswap.h`

 * *Files identical despite different names*

### Comparing `pglib-5.6.0/src/connection.cpp` & `pglib-5.7.0/src/connection.cpp`

 * *Files 3% similar despite different names*

```diff
@@ -199,14 +199,164 @@
         return SetResultError(result.Detach());
 
     default:
         Py_RETURN_NONE;
     }
 }
 
+const char* doc_copy_from =
+    "Connection.copy_from(command, source) --> int\n"
+    "\n"
+    "Executes the given COPY FROM command and returns the number of records copied.\n"
+    "\n"
+    "command\n"
+    "  The copy command which must be 'from stdin'.\n"
+    "\n"
+    "source\n"
+    "  The data to copy from.  This can be a string formatted as CSV or a file-like\n"
+    "  object (anything with a read method that returns a string or bytes object).\n"
+    "\n"
+    "Examples:\n"
+    "  cnxn.copy_from('copy from t1 from stdin csv header', open('test.csv'))\n"
+    "  cnxn.copy_from('copy from t1(a, b, c) from stdin csv header', open('test.csv'))\n"
+    "  cnxn.copy_from('copy from t1 from stdin csv header', gzip.open('test.csv'))\n"
+    "  cnxn.copy_from('copy from t1 from stdin csv', \"1,'one'\\n2,'two'\"))\n";
+
+static PyObject* Connection_copy_from(PyObject* self, PyObject* args)
+{
+    PyObject* command;
+    PyObject* source;
+    if (!PyArg_ParseTuple(args, "UO", &command, &source))
+        return 0;
+
+    // If source is a string (Unicode), store the UTF-encoded value in buffer. If a byte
+    // object, store directly in buffer.  Otherwise, buffer will be zero and `source` must be
+    // an object with a read method (e.g. file).
+    const char* buffer = 0;
+    Py_ssize_t buffer_size = 0;
+    PyObject* read_method = 0;
+
+    if (PyUnicode_Check(source))
+    {
+        buffer = PyUnicode_AsUTF8AndSize(source, &buffer_size);
+        if (buffer == 0)
+            return 0;
+    }
+    else
+    {
+        if (!PyObject_HasAttrString(source, "read"))
+            return PyErr_Format(Error, "CSV source must be a string or file-like object.");
+        read_method = PyObject_GetAttrString(source, "read");
+    }
+
+    Connection* cnxn = CastConnection(self, REQUIRE_OPEN);
+    if (!cnxn)
+        return 0;
+
+    const char* szSQL = PyUnicode_AsUTF8(command);
+    ResultHolder result;
+    Py_BEGIN_ALLOW_THREADS
+    result = PQexec(cnxn->pgconn, szSQL);
+    Py_END_ALLOW_THREADS
+
+    if (result == 0)
+        return 0;
+
+    switch (PQresultStatus(result)) {
+    case PGRES_COPY_IN:
+        // This is what we are expecting.
+        break;
+
+    case PGRES_BAD_RESPONSE:
+    case PGRES_NONFATAL_ERROR:
+    case PGRES_FATAL_ERROR:
+        return SetResultError(result.Detach());
+
+    default:
+        return PyErr_Format(Error, "Result was not PGRES_COPY_IN: %d", (int)PQresultStatus(result));
+    }
+
+    if (buffer != 0)
+    {
+        int copyStatus = 0;
+        Py_BEGIN_ALLOW_THREADS
+        copyStatus = PQputCopyData(cnxn->pgconn, buffer, (int)buffer_size);
+        Py_END_ALLOW_THREADS
+        if (copyStatus != 1)
+            return SetConnectionError(cnxn);
+    }
+    else
+    {
+        Object read_args(Py_BuildValue("(l)", 200 * 1024));
+        if (read_args == 0)
+            return 0;
+
+        for (;;)
+        {
+            Object s(PyObject_CallObject(read_method, read_args));
+            if (s == 0)
+                return 0;
+            if (PyBytes_Check(s))
+            {
+                buffer = PyBytes_AS_STRING(s.Get());
+                buffer_size = PyBytes_GET_SIZE(s.Get());
+            }
+            else if (PyUnicode_Check(s.Get()))
+            {
+                buffer = PyUnicode_AsUTF8AndSize(s.Get(), &buffer_size);
+            }
+            else
+            {
+                return PyErr_Format(Error, "Result of reading is not a bytes object: %R", s.Get());
+            }
+            if (buffer == 0)
+                return 0;
+            if (buffer_size == 0)
+                break;
+            int copyStatus = 0;
+            Py_BEGIN_ALLOW_THREADS
+            copyStatus = PQputCopyData(cnxn->pgconn, buffer, (int)buffer_size);
+            Py_END_ALLOW_THREADS
+            if (copyStatus != 1)
+                return SetConnectionError(cnxn);
+        }
+    }
+
+    if (PQputCopyEnd(cnxn->pgconn, 0) != 1)
+        return SetConnectionError(cnxn);
+
+    // After a copy, you have to get another result to know if it was successful.
+
+    ResultHolder final_result;
+    ExecStatusType status = PGRES_COMMAND_OK;
+    Py_BEGIN_ALLOW_THREADS
+    final_result = PQgetResult(cnxn->pgconn);
+    status = PQresultStatus(final_result);
+
+    // You must call PQgetResult until it returns NULL at the end of each command.
+    for (;;) {
+      PGresult* res = PQgetResult(cnxn->pgconn);
+      if (res == 0)
+        break;
+      PQclear(res);
+    }
+    Py_END_ALLOW_THREADS
+
+    if (status != PGRES_COMMAND_OK) {
+      // SetResultError will take ownership of `result`.
+      return SetResultError(final_result.Detach());
+    }
+
+    const char* sz = PQcmdTuples(final_result);
+    if (sz == 0 || *sz == 0)
+      Py_RETURN_NONE;
+    return PyLong_FromLong(atoi(sz));
+}
+
+
 const char* doc_copy_from_csv =
     "Connection.copy_from_csv(table, source, header=0) --> int\n"
     "\n"
     "Executes a COPY FROM command and returns the number of records copied.\n"
     "\n"
     "table\n"
     "  The table to copy to.  This can also contain the columns to populate.\n"
@@ -1303,14 +1453,15 @@
     { "fetchval", Connection_fetchval,  METH_VARARGS, 0 },
     { "fetchvals", Connection_fetchvals, METH_VARARGS, doc_fetchvals },
     { "row",     Connection_row,     METH_VARARGS, 0 },
     { "scalar",  Connection_fetchval,  METH_VARARGS, 0 }, // deprecated
     { "trace",   Connection_trace,   METH_VARARGS, 0 },
     { "reset",   Connection_reset,   METH_NOARGS,  0 },
     { "script",  Connection_script,  METH_VARARGS, doc_script },
+    { "copy_from", (PyCFunction) Connection_copy_from, METH_VARARGS | METH_KEYWORDS, doc_copy_from },
     { "copy_from_csv", (PyCFunction) Connection_copy_from_csv, METH_VARARGS | METH_KEYWORDS, doc_copy_from_csv },
     { "begin",    Connection_begin,   METH_NOARGS, doc_begin },
     { "commit",   Connection_commit,   METH_NOARGS, doc_commit },
     { "rollback", Connection_rollback,   METH_NOARGS, doc_rollback },
     { "close", Connection_close,   METH_NOARGS, doc_close },
     { "_connectPoll", Connection_connectPoll, METH_NOARGS, 0 },
     { "_sendQuery", Connection_sendQuery, METH_VARARGS, 0 },
```

### Comparing `pglib-5.6.0/src/connection.h` & `pglib-5.7.0/src/connection.h`

 * *Files identical despite different names*

### Comparing `pglib-5.6.0/src/conninfoopt.cpp` & `pglib-5.7.0/src/conninfoopt.cpp`

 * *Files identical despite different names*

### Comparing `pglib-5.6.0/src/datatypes.cpp` & `pglib-5.7.0/src/datatypes.cpp`

 * *Files identical despite different names*

### Comparing `pglib-5.6.0/src/enums.cpp` & `pglib-5.7.0/src/enums.cpp`

 * *Files identical despite different names*

### Comparing `pglib-5.6.0/src/errors.cpp` & `pglib-5.7.0/src/errors.cpp`

 * *Files identical despite different names*

### Comparing `pglib-5.6.0/src/getdata.cpp` & `pglib-5.7.0/src/getdata.cpp`

 * *Files identical despite different names*

### Comparing `pglib-5.6.0/src/juliandate.cpp` & `pglib-5.7.0/src/juliandate.cpp`

 * *Files identical despite different names*

### Comparing `pglib-5.6.0/src/params.cpp` & `pglib-5.7.0/src/params.cpp`

 * *Files identical despite different names*

### Comparing `pglib-5.6.0/src/params.h` & `pglib-5.7.0/src/params.h`

 * *Files identical despite different names*

### Comparing `pglib-5.6.0/src/pgarrays.cpp` & `pglib-5.7.0/src/pgarrays.cpp`

 * *Files identical despite different names*

### Comparing `pglib-5.6.0/src/pglib.cpp` & `pglib-5.7.0/src/pglib.cpp`

 * *Files identical despite different names*

### Comparing `pglib-5.6.0/src/pglib.h` & `pglib-5.7.0/src/pglib.h`

 * *Files identical despite different names*

### Comparing `pglib-5.6.0/src/resultset.cpp` & `pglib-5.7.0/src/resultset.cpp`

 * *Files identical despite different names*

### Comparing `pglib-5.6.0/src/resultset.h` & `pglib-5.7.0/src/resultset.h`

 * *Files identical despite different names*

### Comparing `pglib-5.6.0/src/row.cpp` & `pglib-5.7.0/src/row.cpp`

 * *Files identical despite different names*

### Comparing `pglib-5.6.0/src/runtime.cpp` & `pglib-5.7.0/src/runtime.cpp`

 * *Files identical despite different names*

### Comparing `pglib-5.6.0/src/type_hstore.cpp` & `pglib-5.7.0/src/type_hstore.cpp`

 * *Files identical despite different names*

### Comparing `pglib-5.6.0/src/type_json.cpp` & `pglib-5.7.0/src/type_json.cpp`

 * *Files identical despite different names*

### Comparing `pglib-5.6.0/src/type_ltree.cpp` & `pglib-5.7.0/src/type_ltree.cpp`

 * *Files identical despite different names*

### Comparing `pglib-5.6.0/test/test_async.py` & `pglib-5.7.0/test/test_async.py`

 * *Files identical despite different names*

### Comparing `pglib-5.6.0/test/test_sync.py` & `pglib-5.7.0/test/test_sync.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,14 @@
 import pytest
 
 from .import testutils
 testutils.add_to_path()
 
 import pglib
 
-
 CONNINFO = 'dbname=test'
 
 STR_FENCEPOST_SIZES = [0, 1, 255, 256, 510, 511, 512, 1023, 1024, 2047, 2048, 4000, 4095, 4096,
                        4097, 10 * 1024, 20 * 1024]
 STR_FENCEPOSTS = [testutils.generate_test_string(size) for size in STR_FENCEPOST_SIZES]
 
 
@@ -152,92 +151,102 @@
 
 def _datapath(filename):
     path = join(dirname(__file__), filename)
     assert exists(path)
     return path
 
 
-def test_copy_csv(cnxn):
+def test_copyfromcsv_csv(cnxn):
     cnxn.execute("create table t1(a int, b varchar(20))")
     count = cnxn.copy_from_csv("t1", open(_datapath('test-noheader.csv')))
     assert count == 2
     assert cnxn.fetchval("select count(*) from t1") == 2
     row = cnxn.fetchrow("select a,b from t1 where a=2")
     assert row.a == 2
     assert row.b == 'two'
 
 
-def test_copy_csv_header(cnxn):
+def test_copyfromcsv_csv_header(cnxn):
     cnxn.execute("create table t1(a int, b varchar(20))")
     count = cnxn.copy_from_csv("t1", open(_datapath('test-header.csv')), header=True)
     assert count == 2
     assert cnxn.fetchval("select count(*) from t1") == 2
     row = cnxn.fetchrow("select a,b from t1 where a=2")
     assert row.a == 2
     assert row.b == 'two'
 
 
-def test_copy_csv_error(cnxn):
+def test_copyfromcsv_csv_error(cnxn):
     """
     Ensure an error copying raises a Python error.
     """
     # We'll make the second column too small.
     cnxn.execute("create table t1(a int, b varchar(1) not null)")
     with pytest.raises(pglib.Error):
         cnxn.copy_from_csv("t1", open(_datapath('test-noheader.csv')))
 
 
-def test_copy_csv_gzip(cnxn):
+def test_copyfromcsv_csv_gzip(cnxn):
     # I don't remember why this test is here.  We're feeding it unzipped data.
     cnxn.execute("create table t1(a int, b varchar(20))")
     cnxn.copy_from_csv("t1", gzip.open(_datapath('test-header.csv.gz')), header=True)
     assert cnxn.fetchval("select count(*) from t1") == 2
     row = cnxn.fetchrow("select a,b from t1 where a=2")
     assert row.a == 2
     assert row.b == 'two'
 
 
-def test_copy_csv_string(cnxn):
+def test_copyfromcsv_csv_string(cnxn):
     cnxn.execute("create table t1(a int, b varchar(20))")
     count = cnxn.copy_from_csv("t1", '1,"one"\n2,"two"')
     assert count == 2
     row = cnxn.fetchrow("select a,b from t1 where a=2")
     assert row.a == 2
     assert row.b == 'two'
 
 
-def test_copy_csv_string_cols(cnxn):
+def test_copyfromcsv_csv_string_cols(cnxn):
     cnxn.execute("create table t1(a int, b varchar(20))")
     count = cnxn.copy_from_csv("t1(b, a)", '"one",1\n"two",2')  # reverse order of cols
     assert count == 2
     row = cnxn.fetchrow("select a,b from t1 where a=2")
     assert row.a == 2
     assert row.b == 'two'
 
 
-def test_copy_psv_string(cnxn):
+def test_copyfromcsv_psv_string(cnxn):
     cnxn.execute("create table t1(a int, b varchar(20))")
     count = cnxn.copy_from_csv("t1", '1|"one"\n2|"two"', delimiter='|')
     assert count == 2
     row = cnxn.fetchrow("select a,b from t1 where a=2")
     assert row.a == 2
     assert row.b == 'two'
 
-def test_copy_psv_quote(cnxn):
+def test_copyfromcsv_psv_quote(cnxn):
     # Send in some data with a quote in it as part of the string like 1/2".  We'll change the
     # quotes to something not in the data (a bel/7 character) and ensure it considered the quote
     # as part of the data.
 
     cnxn.execute("create table t1(a int, b varchar(20))")
     count = cnxn.copy_from_csv("t1", '1|1/2"\n2|3/4"', delimiter='|', quote="\x07")
     assert count == 2
     row = cnxn.fetchrow("select a,b from t1 where a=2")
     assert row.a == 2
     assert row.b == '3/4"'
 
+def test_copy_from_psv_quote(cnxn):
+    cmd = "copy t1 from stdin with csv delimiter '|' quote '\x07'"
+
+    cnxn.execute("create table t1(a int, b varchar(20))")
+    count = cnxn.copy_from(cmd, '1|1/2"\n2|3/4"')
+    assert count == 2
+    row = cnxn.fetchrow("select a,b from t1 where a=2")
+    assert row.a == 2
+    assert row.b == '3/4"'
+
 #
 # row
 #
 
 
 def test_row_zero(cnxn):
     cnxn.execute("create table t1(a int)")
```

### Comparing `pglib-5.6.0/test/testutils.py` & `pglib-5.7.0/test/testutils.py`

 * *Files identical despite different names*

