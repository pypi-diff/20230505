# Comparing `tmp/encoded_client-0.2.0.tar.gz` & `tmp/encoded_client-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "encoded_client-0.2.0.tar", last modified: Mon Oct  3 23:49:18 2022, max compression
+gzip compressed data, was "encoded_client-0.3.0.tar", last modified: Fri May  5 18:41:02 2023, max compression
```

## Comparing `encoded_client-0.2.0.tar` & `encoded_client-0.3.0.tar`

### file list

```diff
@@ -1,59 +1,59 @@
-drwxr-xr-x   0 diane     (1000) diane     (1000)        0 2022-10-03 23:49:18.962771 encoded_client-0.2.0/
-drwxr-xr-x   0 diane     (1000) diane     (1000)        0 2022-10-03 23:49:18.950771 encoded_client-0.2.0/.github/
-drwxr-xr-x   0 diane     (1000) diane     (1000)        0 2022-10-03 23:49:18.954771 encoded_client-0.2.0/.github/workflows/
--rw-r--r--   0 diane     (1000) diane     (1000)      643 2021-10-14 21:04:40.000000 encoded_client-0.2.0/.github/workflows/ci-test.yml
--rw-r--r--   0 diane     (1000) diane     (1000)       99 2022-10-03 22:33:48.000000 encoded_client-0.2.0/.gitignore
--rw-r--r--   0 diane     (1000) diane     (1000)     1345 2022-10-03 23:41:34.000000 encoded_client-0.2.0/Changelog.rst
--rw-r--r--   0 diane     (1000) diane     (1000)     1547 2022-06-22 18:55:52.000000 encoded_client-0.2.0/LICENSE.txt
--rw-r--r--   0 diane     (1000) diane     (1000)     1017 2022-10-03 23:49:18.962771 encoded_client-0.2.0/PKG-INFO
--rw-r--r--   0 diane     (1000) diane     (1000)      558 2022-06-22 20:26:32.000000 encoded_client-0.2.0/README.rst
-drwxr-xr-x   0 diane     (1000) diane     (1000)        0 2022-10-03 23:49:18.954771 encoded_client-0.2.0/docs/
--rw-r--r--   0 diane     (1000) diane     (1000)      634 2021-03-24 23:32:19.000000 encoded_client-0.2.0/docs/Makefile
--rw-r--r--   0 diane     (1000) diane     (1000)      152 2021-03-24 23:57:51.000000 encoded_client-0.2.0/docs/api.rst
--rw-r--r--   0 diane     (1000) diane     (1000)     1909 2021-03-25 00:08:08.000000 encoded_client-0.2.0/docs/conf.py
--rw-r--r--   0 diane     (1000) diane     (1000)      297 2021-03-25 00:03:06.000000 encoded_client-0.2.0/docs/index.rst
--rw-r--r--   0 diane     (1000) diane     (1000)      201 2021-03-25 00:05:14.000000 encoded_client-0.2.0/docs/installation.rst
--rw-r--r--   0 diane     (1000) diane     (1000)     1704 2021-03-25 05:05:51.000000 encoded_client-0.2.0/docs/introduction.rst
--rw-r--r--   0 diane     (1000) diane     (1000)      795 2021-03-24 23:32:19.000000 encoded_client-0.2.0/docs/make.bat
--rw-r--r--   0 diane     (1000) diane     (1000)     4081 2021-03-25 00:50:44.000000 encoded_client-0.2.0/docs/usage.rst
-drwxr-xr-x   0 diane     (1000) diane     (1000)        0 2022-10-03 23:49:18.958771 encoded_client-0.2.0/encoded_client/
--rw-r--r--   0 diane     (1000) diane     (1000)       29 2020-11-30 22:57:40.000000 encoded_client-0.2.0/encoded_client/__init__.py
--rw-r--r--   0 diane     (1000) diane     (1000)      176 2022-10-03 23:49:18.000000 encoded_client-0.2.0/encoded_client/_version.py
--rw-r--r--   0 diane     (1000) diane     (1000)    50501 2022-10-03 23:41:34.000000 encoded_client-0.2.0/encoded_client/encoded.py
--rw-r--r--   0 diane     (1000) diane     (1000)     2231 2021-11-08 18:28:20.000000 encoded_client-0.2.0/encoded_client/hashfile.py
--rw-r--r--   0 diane     (1000) diane     (1000)     5140 2021-12-16 01:06:27.000000 encoded_client-0.2.0/encoded_client/metadata.py
--rw-r--r--   0 diane     (1000) diane     (1000)    10410 2022-10-03 22:33:48.000000 encoded_client-0.2.0/encoded_client/rdfhelp.py
--rw-r--r--   0 diane     (1000) diane     (1000)      890 2020-11-30 22:57:40.000000 encoded_client-0.2.0/encoded_client/rdfns.py
-drwxr-xr-x   0 diane     (1000) diane     (1000)        0 2022-10-03 23:49:18.958771 encoded_client-0.2.0/encoded_client/schemas/
--rw-r--r--   0 diane     (1000) diane     (1000)     1075 2020-11-30 22:57:40.000000 encoded_client-0.2.0/encoded_client/schemas/dc.turtle
--rw-r--r--   0 diane     (1000) diane     (1000)    10996 2020-11-30 22:57:40.000000 encoded_client-0.2.0/encoded_client/schemas/htsworkflow.turtle
--rw-r--r--   0 diane     (1000) diane     (1000)    24076 2020-11-30 22:57:40.000000 encoded_client-0.2.0/encoded_client/schemas/owl.turtle
--rw-r--r--   0 diane     (1000) diane     (1000)     8606 2020-11-30 22:57:40.000000 encoded_client-0.2.0/encoded_client/schemas/rdf.turtle
--rw-r--r--   0 diane     (1000) diane     (1000)     4359 2020-11-30 22:57:40.000000 encoded_client-0.2.0/encoded_client/schemas/rdfs.turtle
--rw-r--r--   0 diane     (1000) diane     (1000)      946 2020-11-30 22:57:40.000000 encoded_client-0.2.0/encoded_client/schemas/xhtmlvocab.turtle
--rw-r--r--   0 diane     (1000) diane     (1000)      929 2022-10-03 22:33:48.000000 encoded_client-0.2.0/encoded_client/sheet.py
--rw-r--r--   0 diane     (1000) diane     (1000)     7926 2022-10-03 22:33:48.000000 encoded_client-0.2.0/encoded_client/submission.py
-drwxr-xr-x   0 diane     (1000) diane     (1000)        0 2022-10-03 23:49:18.962771 encoded_client-0.2.0/encoded_client/tests/
--rw-r--r--   0 diane     (1000) diane     (1000)        0 2020-11-30 22:57:40.000000 encoded_client-0.2.0/encoded_client/tests/__init__.py
--rw-r--r--   0 diane     (1000) diane     (1000)    45621 2021-12-07 23:47:59.000000 encoded_client-0.2.0/encoded_client/tests/biosample.json
--rw-r--r--   0 diane     (1000) diane     (1000)      241 2020-11-30 22:57:40.000000 encoded_client-0.2.0/encoded_client/tests/extra.turtle
--rw-r--r--   0 diane     (1000) diane     (1000)    68303 2021-12-07 23:47:59.000000 encoded_client-0.2.0/encoded_client/tests/file.json
--rw-r--r--   0 diane     (1000) diane     (1000)    24952 2021-12-07 23:47:59.000000 encoded_client-0.2.0/encoded_client/tests/library.json
--rw-r--r--   0 diane     (1000) diane     (1000)    16503 2021-12-07 23:47:59.000000 encoded_client-0.2.0/encoded_client/tests/star_solo_quality_metric.json
--rw-r--r--   0 diane     (1000) diane     (1000)    19362 2022-10-03 22:33:48.000000 encoded_client-0.2.0/encoded_client/tests/test_encoded.py
--rw-r--r--   0 diane     (1000) diane     (1000)      468 2021-10-29 16:41:20.000000 encoded_client-0.2.0/encoded_client/tests/test_hashfile.py
--rw-r--r--   0 diane     (1000) diane     (1000)     9035 2021-12-16 01:06:27.000000 encoded_client-0.2.0/encoded_client/tests/test_metadata.py
--rw-r--r--   0 diane     (1000) diane     (1000)     8444 2021-12-17 19:05:39.000000 encoded_client-0.2.0/encoded_client/tests/test_rdfhelp.py
--rw-r--r--   0 diane     (1000) diane     (1000)     1302 2021-12-17 19:05:39.000000 encoded_client-0.2.0/encoded_client/tests/test_sheet.py
--rw-r--r--   0 diane     (1000) diane     (1000)     1798 2021-12-17 19:05:39.000000 encoded_client-0.2.0/encoded_client/tests/test_submission.py
-drwxr-xr-x   0 diane     (1000) diane     (1000)        0 2022-10-03 23:49:18.958771 encoded_client-0.2.0/encoded_client.egg-info/
--rw-r--r--   0 diane     (1000) diane     (1000)     1017 2022-10-03 23:49:18.000000 encoded_client-0.2.0/encoded_client.egg-info/PKG-INFO
--rw-r--r--   0 diane     (1000) diane     (1000)     1406 2022-10-03 23:49:18.000000 encoded_client-0.2.0/encoded_client.egg-info/SOURCES.txt
--rw-r--r--   0 diane     (1000) diane     (1000)        1 2022-10-03 23:49:18.000000 encoded_client-0.2.0/encoded_client.egg-info/dependency_links.txt
--rw-r--r--   0 diane     (1000) diane     (1000)       69 2022-10-03 23:49:18.000000 encoded_client-0.2.0/encoded_client.egg-info/entry_points.txt
--rw-r--r--   0 diane     (1000) diane     (1000)        1 2021-10-14 18:54:48.000000 encoded_client-0.2.0/encoded_client.egg-info/not-zip-safe
--rw-r--r--   0 diane     (1000) diane     (1000)      157 2022-10-03 23:49:18.000000 encoded_client-0.2.0/encoded_client.egg-info/requires.txt
--rw-r--r--   0 diane     (1000) diane     (1000)       15 2022-10-03 23:49:18.000000 encoded_client-0.2.0/encoded_client.egg-info/top_level.txt
--rw-r--r--   0 diane     (1000) diane     (1000)      371 2022-10-03 23:42:59.000000 encoded_client-0.2.0/pyproject.toml
--rw-r--r--   0 diane     (1000) diane     (1000)      891 2022-10-03 23:49:18.962771 encoded_client-0.2.0/setup.cfg
--rw-r--r--   0 diane     (1000) diane     (1000)       69 2021-10-14 18:53:16.000000 encoded_client-0.2.0/setup.py
+drwxr-xr-x   0 diane     (1000) diane     (1000)        0 2023-05-05 18:41:02.112923 encoded_client-0.3.0/
+drwxr-xr-x   0 diane     (1000) diane     (1000)        0 2023-05-05 18:41:02.096922 encoded_client-0.3.0/.github/
+drwxr-xr-x   0 diane     (1000) diane     (1000)        0 2023-05-05 18:41:02.100923 encoded_client-0.3.0/.github/workflows/
+-rw-r--r--   0 diane     (1000) diane     (1000)      643 2021-10-14 21:04:40.000000 encoded_client-0.3.0/.github/workflows/ci-test.yml
+-rw-r--r--   0 diane     (1000) diane     (1000)      113 2023-05-04 22:28:48.000000 encoded_client-0.3.0/.gitignore
+-rw-r--r--   0 diane     (1000) diane     (1000)     2090 2023-05-04 22:42:03.000000 encoded_client-0.3.0/Changelog.rst
+-rw-r--r--   0 diane     (1000) diane     (1000)     1547 2022-06-22 18:55:52.000000 encoded_client-0.3.0/LICENSE.txt
+-rw-r--r--   0 diane     (1000) diane     (1000)     1017 2023-05-05 18:41:02.112923 encoded_client-0.3.0/PKG-INFO
+-rw-r--r--   0 diane     (1000) diane     (1000)      558 2022-06-22 20:26:32.000000 encoded_client-0.3.0/README.rst
+drwxr-xr-x   0 diane     (1000) diane     (1000)        0 2023-05-05 18:41:02.100923 encoded_client-0.3.0/docs/
+-rw-r--r--   0 diane     (1000) diane     (1000)      634 2021-03-24 23:32:19.000000 encoded_client-0.3.0/docs/Makefile
+-rw-r--r--   0 diane     (1000) diane     (1000)      152 2021-03-24 23:57:51.000000 encoded_client-0.3.0/docs/api.rst
+-rw-r--r--   0 diane     (1000) diane     (1000)     1909 2021-03-25 00:08:08.000000 encoded_client-0.3.0/docs/conf.py
+-rw-r--r--   0 diane     (1000) diane     (1000)      297 2021-03-25 00:03:06.000000 encoded_client-0.3.0/docs/index.rst
+-rw-r--r--   0 diane     (1000) diane     (1000)      201 2021-03-25 00:05:14.000000 encoded_client-0.3.0/docs/installation.rst
+-rw-r--r--   0 diane     (1000) diane     (1000)     1704 2021-03-25 05:05:51.000000 encoded_client-0.3.0/docs/introduction.rst
+-rw-r--r--   0 diane     (1000) diane     (1000)      795 2021-03-24 23:32:19.000000 encoded_client-0.3.0/docs/make.bat
+-rw-r--r--   0 diane     (1000) diane     (1000)     4081 2021-03-25 00:50:44.000000 encoded_client-0.3.0/docs/usage.rst
+drwxr-xr-x   0 diane     (1000) diane     (1000)        0 2023-05-05 18:41:02.104923 encoded_client-0.3.0/encoded_client/
+-rw-r--r--   0 diane     (1000) diane     (1000)       29 2020-11-30 22:57:40.000000 encoded_client-0.3.0/encoded_client/__init__.py
+-rw-r--r--   0 diane     (1000) diane     (1000)      160 2023-05-05 18:41:02.000000 encoded_client-0.3.0/encoded_client/_version.py
+-rw-r--r--   0 diane     (1000) diane     (1000)    52680 2023-05-04 22:28:48.000000 encoded_client-0.3.0/encoded_client/encoded.py
+-rw-r--r--   0 diane     (1000) diane     (1000)     2231 2021-11-08 18:28:20.000000 encoded_client-0.3.0/encoded_client/hashfile.py
+-rw-r--r--   0 diane     (1000) diane     (1000)     9019 2023-05-01 22:57:33.000000 encoded_client-0.3.0/encoded_client/metadata.py
+-rw-r--r--   0 diane     (1000) diane     (1000)    10410 2022-10-03 22:33:48.000000 encoded_client-0.3.0/encoded_client/rdfhelp.py
+-rw-r--r--   0 diane     (1000) diane     (1000)      890 2020-11-30 22:57:40.000000 encoded_client-0.3.0/encoded_client/rdfns.py
+drwxr-xr-x   0 diane     (1000) diane     (1000)        0 2023-05-05 18:41:02.108923 encoded_client-0.3.0/encoded_client/schemas/
+-rw-r--r--   0 diane     (1000) diane     (1000)     1075 2020-11-30 22:57:40.000000 encoded_client-0.3.0/encoded_client/schemas/dc.turtle
+-rw-r--r--   0 diane     (1000) diane     (1000)    10996 2020-11-30 22:57:40.000000 encoded_client-0.3.0/encoded_client/schemas/htsworkflow.turtle
+-rw-r--r--   0 diane     (1000) diane     (1000)    24076 2020-11-30 22:57:40.000000 encoded_client-0.3.0/encoded_client/schemas/owl.turtle
+-rw-r--r--   0 diane     (1000) diane     (1000)     8606 2020-11-30 22:57:40.000000 encoded_client-0.3.0/encoded_client/schemas/rdf.turtle
+-rw-r--r--   0 diane     (1000) diane     (1000)     4359 2020-11-30 22:57:40.000000 encoded_client-0.3.0/encoded_client/schemas/rdfs.turtle
+-rw-r--r--   0 diane     (1000) diane     (1000)      946 2020-11-30 22:57:40.000000 encoded_client-0.3.0/encoded_client/schemas/xhtmlvocab.turtle
+-rw-r--r--   0 diane     (1000) diane     (1000)      929 2022-10-03 22:33:48.000000 encoded_client-0.3.0/encoded_client/sheet.py
+-rw-r--r--   0 diane     (1000) diane     (1000)     9573 2023-05-04 22:28:48.000000 encoded_client-0.3.0/encoded_client/submission.py
+drwxr-xr-x   0 diane     (1000) diane     (1000)        0 2023-05-05 18:41:02.112923 encoded_client-0.3.0/encoded_client/tests/
+-rw-r--r--   0 diane     (1000) diane     (1000)        0 2020-11-30 22:57:40.000000 encoded_client-0.3.0/encoded_client/tests/__init__.py
+-rw-r--r--   0 diane     (1000) diane     (1000)    45621 2021-12-07 23:47:59.000000 encoded_client-0.3.0/encoded_client/tests/biosample.json
+-rw-r--r--   0 diane     (1000) diane     (1000)      241 2020-11-30 22:57:40.000000 encoded_client-0.3.0/encoded_client/tests/extra.turtle
+-rw-r--r--   0 diane     (1000) diane     (1000)    68303 2021-12-07 23:47:59.000000 encoded_client-0.3.0/encoded_client/tests/file.json
+-rw-r--r--   0 diane     (1000) diane     (1000)    24952 2021-12-07 23:47:59.000000 encoded_client-0.3.0/encoded_client/tests/library.json
+-rw-r--r--   0 diane     (1000) diane     (1000)    16503 2021-12-07 23:47:59.000000 encoded_client-0.3.0/encoded_client/tests/star_solo_quality_metric.json
+-rw-r--r--   0 diane     (1000) diane     (1000)    19362 2023-04-19 23:31:41.000000 encoded_client-0.3.0/encoded_client/tests/test_encoded.py
+-rw-r--r--   0 diane     (1000) diane     (1000)      468 2021-10-29 16:41:20.000000 encoded_client-0.3.0/encoded_client/tests/test_hashfile.py
+-rw-r--r--   0 diane     (1000) diane     (1000)     9035 2021-12-16 01:06:27.000000 encoded_client-0.3.0/encoded_client/tests/test_metadata.py
+-rw-r--r--   0 diane     (1000) diane     (1000)     8444 2021-12-17 19:05:39.000000 encoded_client-0.3.0/encoded_client/tests/test_rdfhelp.py
+-rw-r--r--   0 diane     (1000) diane     (1000)     1302 2021-12-17 19:05:39.000000 encoded_client-0.3.0/encoded_client/tests/test_sheet.py
+-rw-r--r--   0 diane     (1000) diane     (1000)     1959 2023-05-04 22:28:48.000000 encoded_client-0.3.0/encoded_client/tests/test_submission.py
+drwxr-xr-x   0 diane     (1000) diane     (1000)        0 2023-05-05 18:41:02.104923 encoded_client-0.3.0/encoded_client.egg-info/
+-rw-r--r--   0 diane     (1000) diane     (1000)     1017 2023-05-05 18:41:02.000000 encoded_client-0.3.0/encoded_client.egg-info/PKG-INFO
+-rw-r--r--   0 diane     (1000) diane     (1000)     1406 2023-05-05 18:41:02.000000 encoded_client-0.3.0/encoded_client.egg-info/SOURCES.txt
+-rw-r--r--   0 diane     (1000) diane     (1000)        1 2023-05-05 18:41:02.000000 encoded_client-0.3.0/encoded_client.egg-info/dependency_links.txt
+-rw-r--r--   0 diane     (1000) diane     (1000)       69 2023-05-05 18:41:02.000000 encoded_client-0.3.0/encoded_client.egg-info/entry_points.txt
+-rw-r--r--   0 diane     (1000) diane     (1000)        1 2021-10-14 18:54:48.000000 encoded_client-0.3.0/encoded_client.egg-info/not-zip-safe
+-rw-r--r--   0 diane     (1000) diane     (1000)      157 2023-05-05 18:41:02.000000 encoded_client-0.3.0/encoded_client.egg-info/requires.txt
+-rw-r--r--   0 diane     (1000) diane     (1000)       15 2023-05-05 18:41:02.000000 encoded_client-0.3.0/encoded_client.egg-info/top_level.txt
+-rw-r--r--   0 diane     (1000) diane     (1000)      365 2023-05-04 22:28:48.000000 encoded_client-0.3.0/pyproject.toml
+-rw-r--r--   0 diane     (1000) diane     (1000)      891 2023-05-05 18:41:02.112923 encoded_client-0.3.0/setup.cfg
+-rw-r--r--   0 diane     (1000) diane     (1000)       69 2021-10-14 18:53:16.000000 encoded_client-0.3.0/setup.py
```

### Comparing `encoded_client-0.2.0/.github/workflows/ci-test.yml` & `encoded_client-0.3.0/.github/workflows/ci-test.yml`

 * *Files identical despite different names*

### Comparing `encoded_client-0.2.0/LICENSE.txt` & `encoded_client-0.3.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `encoded_client-0.2.0/PKG-INFO` & `encoded_client-0.3.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: encoded_client
-Version: 0.2.0
+Version: 0.3.0
 Summary: interface to the ENCODE DCC portal
 Author: Diane Trout
 Author-email: diane@caltech.edu
 License: BSD-3
 Project-URL: Source, https://github.com/detrout/encoded_client
 Project-URL: Tracker, https://github.com/detrout/encoded_client
 Description-Content-Type: text/x-rst; charset=UTF-8
```

### Comparing `encoded_client-0.2.0/README.rst` & `encoded_client-0.3.0/README.rst`

 * *Files identical despite different names*

### Comparing `encoded_client-0.2.0/docs/Makefile` & `encoded_client-0.3.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `encoded_client-0.2.0/docs/conf.py` & `encoded_client-0.3.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `encoded_client-0.2.0/docs/introduction.rst` & `encoded_client-0.3.0/docs/introduction.rst`

 * *Files identical despite different names*

### Comparing `encoded_client-0.2.0/docs/make.bat` & `encoded_client-0.3.0/docs/make.bat`

 * *Files identical despite different names*

### Comparing `encoded_client-0.2.0/docs/usage.rst` & `encoded_client-0.3.0/docs/usage.rst`

 * *Files identical despite different names*

### Comparing `encoded_client-0.2.0/encoded_client/encoded.py` & `encoded_client-0.3.0/encoded_client/encoded.py`

 * *Files 3% similar despite different names*

```diff
@@ -296,17 +296,14 @@
         Alternative keyword arguments can be passed in and will be sent to the host.
 
         Known keywords are:
           limit - (integer or 'all') how many records to return, all for all of them
           embed - (bool) if true expands linking ids into their associated object.
           format - text/html or application/json
         """
-        if len(kwargs) == 0:
-            kwargs["limit"] = "all"
-
         kwargs["headers"] = self.json_headers
 
         response = self.get_response(obj_id, **kwargs)
         data = response.json()
         response.close()
         return data
 
@@ -387,19 +384,24 @@
 
         This is used by the sheet parsing code to know what column the
         objects accession is in.
         """
         collection_to_accession_name = {
             "/annotations/": "accession",
             "/biosamples/": "accession",
+            "/documents/": "uuid",
             "/experiments/": "accession",
             "/files/": "accession",
             "/libraries/": "accession",
+            "measurement_set": "accession",
             "/mouse-donors/": "accession",
             "/replicates/": "uuid",
+            "rodent_donor": "accession",
+            "sequence_data": "accession",
+            "tissue": "accession",
         }
 
         accession_name = collection_to_accession_name.get(collection, None)
         if accession_name is None:
             raise RuntimeError(
                 "Update list of collection to accession names for %s", collection
             )
@@ -616,15 +618,24 @@
                         del validator._aliases[alias]
 
     def search_jsonld(self, **kwargs):
         """Send search request to ENCODED
 
         to do a general search do
             searchTerm=term
+
+        Known keywords allowed on search:
+          limit - (integer or 'all') how many records to return, all for all of them
+             to be kinder to the server, set an arbitrary limit of 5,000. override
+             with all if all is really needed
+          type - object type
         """
+        if len(kwargs) == 0:
+            kwargs["limit"] = "5000"
+
         url = self.prepare_url("/search/")
         result = self.get_json(url, **kwargs)
         self.convert_search_to_jsonld(result)
         return result
 
     def convert_search_to_jsonld(self, result):
         """Add the context to search result
@@ -1087,24 +1098,54 @@
         self.uuid = uuid
         if uuid is None:
             return self.post(server, validator)
         else:
             return server.get_json(uuid, embed=False)
 
 
+class EncodeFileCache(Mapping):
+    def __init__(self, server, dataset, json=None):
+        self._server = server
+        self._dataset = dataset
+        self._file_cache = []
+
+    def _update_json(self, json):
+        for obj in json:
+            assert obj.get("@type") == ["File", "Item"]
+            assert obj.get("dataset") == self._dataset
+            self._file_cache[obj["@id"]] = obj
+
+    def __getitem__(self, key):
+        if key not in self._file_cache:
+            obj = self._server.get_json(key)
+            self._update_json([obj])
+
+        return self._file_cache[key]
+
+    def __iter__(self):
+        for key in self._file_cache:
+            yield key
+
+    def __len__(self):
+        return len(self._file_cache)
+
+
 class EncodeExperiment(Mapping):
     """Helper class for accessing ENCODED experiment objects"""
 
     def __init__(self, server, json=None):
         self._server = server
         self._json = json
+        self._preferred_analysis = None
         self._replicates = []
         self._schema_version_check()
         self._replicate_file_map = {}
         if self._json is not None:
+            self._files = EncodeFileCache(
+                self._server, self._json["@id"], self._json["files"])
             self._calculate_derived_from()
 
     def _schema_version_check(self):
         supported_versions = {"33", "34", "35", "36"}
         if self.schema_version not in supported_versions:
             LOGGER.warning(
                 "New schema version {} may not be supported".format(self.schema_version)
@@ -1115,22 +1156,26 @@
             if current_file in replicate_map:
                 return replicate_map[current_file]
             return find_source_replicate(
                 derived_map, derived_map[current_file], replicate_map
             )
 
         file_replicate_map = {}
+
+        # this finds replicate information attached to read files
         our_files = set((f["@id"] for f in self._json["files"]))
         for f in self._json["files"]:
             if "replicate" in f:
                 file_replicate_map[f["@id"]] = f["replicate"]["@id"]
 
         derived_map = {}
-        for f in self._json["files"]:
+        for file_id in self.preferred_analysis["files"]:
+            f = self._server.get_json(file_id)
             for derived_from in f.get("derived_from", []):
+                analyses = [x["@id"] for x in f.get("analyses", [])]
                 if derived_from in our_files:
                     derived_map[f["@id"]] = derived_from
 
         for derived_file in derived_map:
             file_replicate_map[derived_file] = find_source_replicate(
                 derived_map, derived_file, file_replicate_map
             )
@@ -1150,14 +1195,24 @@
 
         if len(self._replicates) != len(self._json["replicates"]):
             for replicate in self._json["replicates"]:
                 self._replicates.append(EncodeReplicate(replicate, self))
 
         return self._replicates
 
+    @property
+    def preferred_analysis(self):
+        if self._preferred_analysis is None:
+            default_analysis_id = self._json["default_analysis"]
+            for analysis in self._json["analyses"]:
+                if analysis["@id"] == default_analysis_id:
+                    self._preferred_analysis = analysis
+
+        return self._preferred_analysis
+
     def __getattr__(self, key):
         if self._json is None:
             LOGGER.warn("Uninitialized Experiment object")
             return
         else:
             return self._json[key]
 
@@ -1185,21 +1240,24 @@
             raise ValueError("Not a replicate type: {}".format(obj_type))
         self._json = replicate
         self._files = []
 
     @property
     def files(self):
         if self._json["@id"] not in self._experiment._replicate_file_map:
-            return
+            print("id not in", self._json["@id"])
+            return []
 
         file_ids = self._experiment._replicate_file_map[self._json["@id"]]
-        if len(self._files) != len(file_ids):
-            for f in self._experiment["files"]:
-                if f["@id"] in file_ids:
-                    self._files.append(EncodeFile(f, self))
+        known_files = [x["@id"] for x in self._files]
+        for file_id in file_ids:
+            if file_id not in known_files:
+                f = self._experiment._server.get_json(file_id)
+                LOGGER.debug("File", f["@id"], "dataset?", f["dataset"], "matches experiment", self._experiment["accession"])
+                self._files.append(EncodeFile(f, self))
 
         return self._files
 
     def __getattr__(self, key):
         return self._json.get(key)
 
     def __getitem__(self, key):
@@ -1429,15 +1487,15 @@
     "ScrnaSeqCountsSummaryQualityMetric": parse_scrna_seq_counts_summary,
 }
 
 
 def make_attachment(local_filename, mime_type=None, remote_filename=None):
     local_filename = Path(local_filename)
     if mime_type is None:
-        mime_type = document_mime_type_default[filename.suffix]
+        mime_type = document_mime_type_default[local_filename.suffix]
         if mime_type is None:
             raise ValueError("Unrecognized filename extension")
 
     with open(local_filename, "rb") as instream:
         document = instream.read()
 
     if remote_filename is None:
```

### Comparing `encoded_client-0.2.0/encoded_client/hashfile.py` & `encoded_client-0.3.0/encoded_client/hashfile.py`

 * *Files identical despite different names*

### Comparing `encoded_client-0.2.0/encoded_client/rdfhelp.py` & `encoded_client-0.3.0/encoded_client/rdfhelp.py`

 * *Files identical despite different names*

### Comparing `encoded_client-0.2.0/encoded_client/rdfns.py` & `encoded_client-0.3.0/encoded_client/rdfns.py`

 * *Files identical despite different names*

### Comparing `encoded_client-0.2.0/encoded_client/schemas/dc.turtle` & `encoded_client-0.3.0/encoded_client/schemas/dc.turtle`

 * *Files identical despite different names*

### Comparing `encoded_client-0.2.0/encoded_client/schemas/htsworkflow.turtle` & `encoded_client-0.3.0/encoded_client/schemas/htsworkflow.turtle`

 * *Files identical despite different names*

### Comparing `encoded_client-0.2.0/encoded_client/schemas/owl.turtle` & `encoded_client-0.3.0/encoded_client/schemas/owl.turtle`

 * *Files identical despite different names*

### Comparing `encoded_client-0.2.0/encoded_client/schemas/rdf.turtle` & `encoded_client-0.3.0/encoded_client/schemas/rdf.turtle`

 * *Files identical despite different names*

### Comparing `encoded_client-0.2.0/encoded_client/schemas/rdfs.turtle` & `encoded_client-0.3.0/encoded_client/schemas/rdfs.turtle`

 * *Files identical despite different names*

### Comparing `encoded_client-0.2.0/encoded_client/schemas/xhtmlvocab.turtle` & `encoded_client-0.3.0/encoded_client/schemas/xhtmlvocab.turtle`

 * *Files identical despite different names*

### Comparing `encoded_client-0.2.0/encoded_client/sheet.py` & `encoded_client-0.3.0/encoded_client/sheet.py`

 * *Files identical despite different names*

### Comparing `encoded_client-0.2.0/encoded_client/tests/biosample.json` & `encoded_client-0.3.0/encoded_client/tests/biosample.json`

 * *Files identical despite different names*

### Comparing `encoded_client-0.2.0/encoded_client/tests/file.json` & `encoded_client-0.3.0/encoded_client/tests/file.json`

 * *Files identical despite different names*

### Comparing `encoded_client-0.2.0/encoded_client/tests/library.json` & `encoded_client-0.3.0/encoded_client/tests/library.json`

 * *Files identical despite different names*

### Comparing `encoded_client-0.2.0/encoded_client/tests/star_solo_quality_metric.json` & `encoded_client-0.3.0/encoded_client/tests/star_solo_quality_metric.json`

 * *Files identical despite different names*

### Comparing `encoded_client-0.2.0/encoded_client/tests/test_encoded.py` & `encoded_client-0.3.0/encoded_client/tests/test_encoded.py`

 * *Files 0% similar despite different names*

```diff
@@ -471,15 +471,15 @@
         library_aliases_expected = set(["barbara-wold:13713", "barbara-wold:13714"])
         library_aliases_seen = set()
         for i, r in enumerate(replicates):
             for alias in r["library"]["aliases"]:
                 library_aliases_seen.add(alias)
             files = list(r.files)
             replicate_files[i] = [f["@id"] for f in files]
-            self.assertGreaterEqual(len(files), 24)
+            self.assertGreaterEqual(len(files), 12)
             file_formats_seen = set()
             output_types_seen = set()
             qc_seen = []
             qc_types_seen = set()
             for f in files:
                 file_formats_seen.add(f["file_format"])
                 output_types_seen.add(f["output_type"])
```

### Comparing `encoded_client-0.2.0/encoded_client/tests/test_metadata.py` & `encoded_client-0.3.0/encoded_client/tests/test_metadata.py`

 * *Files identical despite different names*

### Comparing `encoded_client-0.2.0/encoded_client/tests/test_rdfhelp.py` & `encoded_client-0.3.0/encoded_client/tests/test_rdfhelp.py`

 * *Files identical despite different names*

### Comparing `encoded_client-0.2.0/encoded_client/tests/test_sheet.py` & `encoded_client-0.3.0/encoded_client/tests/test_sheet.py`

 * *Files identical despite different names*

### Comparing `encoded_client-0.2.0/encoded_client/tests/test_submission.py` & `encoded_client-0.3.0/encoded_client/tests/test_submission.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import pandas
 import tempfile
 from unittest import TestCase
 import pytest
 
 from ..encoded import ENCODED
-from ..submission import process_files, main
+from ..submission import process_files, process_endpoint_files, main
 
 
 class TestSubmission(TestCase):
     def setUp(self):
         self.example_files = pandas.DataFrame(
             {
                 "uuid": [None],
@@ -32,15 +32,18 @@
             }
         )
 
     def test_process_files(self):
         server = ENCODED("test.encodedcc.org")
         self.assertIsNone(self.example_files.iloc[0]["uuid"])
         self.assertIsNone(self.example_files.iloc[0]["accession"])
-        process_files(server, self.example_files, dry_run=True)
+
+        self.assertRaises(
+            DeprecationWarning, process_files, server, self.example_files, dry_run=True)
+        process_endpoint_files(server, "/files/", self.example_files, dry_run=True)
 
         self.assertEqual(self.example_files.iloc[0]["accession"], "would create")
 
     def test_sumission_main(self):
         pytest.importorskip("openpyxl")
         with tempfile.NamedTemporaryFile(suffix="_encoded.xlsx") as out:
             self.example_files.to_excel(out, sheet_name="File", index=False)
```

### Comparing `encoded_client-0.2.0/encoded_client.egg-info/PKG-INFO` & `encoded_client-0.3.0/encoded_client.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: encoded-client
-Version: 0.2.0
+Version: 0.3.0
 Summary: interface to the ENCODE DCC portal
 Author: Diane Trout
 Author-email: diane@caltech.edu
 License: BSD-3
 Project-URL: Source, https://github.com/detrout/encoded_client
 Project-URL: Tracker, https://github.com/detrout/encoded_client
 Description-Content-Type: text/x-rst; charset=UTF-8
```

### Comparing `encoded_client-0.2.0/encoded_client.egg-info/SOURCES.txt` & `encoded_client-0.3.0/encoded_client.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `encoded_client-0.2.0/setup.cfg` & `encoded_client-0.3.0/setup.cfg`

 * *Files identical despite different names*

