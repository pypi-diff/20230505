# Comparing `tmp/rfcx-0.3.0.tar.gz` & `tmp/rfcx-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rfcx-0.3.0.tar", last modified: Fri May  5 09:40:56 2023, max compression
+gzip compressed data, was "rfcx-0.3.1.tar", last modified: Fri May  5 10:36:43 2023, max compression
```

## Comparing `rfcx-0.3.0.tar` & `rfcx-0.3.1.tar`

### file list

```diff
@@ -1,10 +1,23 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 09:40:56.660449 rfcx-0.3.0/
--rw-r--r--   0 root         (0) root         (0)      651 2023-05-05 09:40:56.658898 rfcx-0.3.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     2955 2023-05-05 09:40:52.000000 rfcx-0.3.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 09:40:56.654523 rfcx-0.3.0/rfcx.egg-info/
--rw-r--r--   0 root         (0) root         (0)      651 2023-05-05 09:40:56.000000 rfcx-0.3.0/rfcx.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      148 2023-05-05 09:40:56.000000 rfcx-0.3.0/rfcx.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-05 09:40:56.000000 rfcx-0.3.0/rfcx.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       40 2023-05-05 09:40:56.000000 rfcx-0.3.0/rfcx.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-05 09:40:56.000000 rfcx-0.3.0/rfcx.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-05-05 09:40:56.661629 rfcx-0.3.0/setup.cfg
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 10:36:43.307640 rfcx-0.3.1/
+-rw-r--r--   0 root         (0) root         (0)      651 2023-05-05 10:36:43.305650 rfcx-0.3.1/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 10:36:43.272508 rfcx-0.3.1/rfcx/
+-rw-r--r--   0 root         (0) root         (0)      254 2023-05-05 09:53:19.000000 rfcx-0.3.1/rfcx/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     5408 2022-12-16 14:56:19.000000 rfcx-0.3.1/rfcx/_api_auth.py
+-rw-r--r--   0 root         (0) root         (0)     4634 2023-05-02 16:02:40.000000 rfcx-0.3.1/rfcx/_api_rfcx.py
+-rw-r--r--   0 root         (0) root         (0)     5493 2023-02-27 10:08:48.000000 rfcx-0.3.1/rfcx/_audio.py
+-rw-r--r--   0 root         (0) root         (0)     6286 2023-05-02 15:53:36.000000 rfcx-0.3.1/rfcx/_authentication.py
+-rw-r--r--   0 root         (0) root         (0)     1155 2023-05-03 10:25:34.000000 rfcx-0.3.1/rfcx/_classifiers.py
+-rw-r--r--   0 root         (0) root         (0)     1459 2022-12-16 14:56:19.000000 rfcx-0.3.1/rfcx/_credentials.py
+-rw-r--r--   0 root         (0) root         (0)    10851 2022-12-16 14:56:19.000000 rfcx-0.3.1/rfcx/_helper.py
+-rw-r--r--   0 root         (0) root         (0)     2787 2023-03-03 09:42:14.000000 rfcx-0.3.1/rfcx/_ingest.py
+-rw-r--r--   0 root         (0) root         (0)     2081 2022-12-16 14:56:19.000000 rfcx-0.3.1/rfcx/_pkce.py
+-rw-r--r--   0 root         (0) root         (0)      388 2022-12-16 14:56:19.000000 rfcx-0.3.1/rfcx/_util.py
+-rw-r--r--   0 root         (0) root         (0)    14750 2023-05-05 09:18:59.000000 rfcx-0.3.1/rfcx/client.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 10:36:43.301729 rfcx-0.3.1/rfcx.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      651 2023-05-05 10:36:43.000000 rfcx-0.3.1/rfcx.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      356 2023-05-05 10:36:43.000000 rfcx-0.3.1/rfcx.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-05 10:36:43.000000 rfcx-0.3.1/rfcx.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       40 2023-05-05 10:36:43.000000 rfcx-0.3.1/rfcx.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        5 2023-05-05 10:36:43.000000 rfcx-0.3.1/rfcx.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-05-05 10:36:43.308599 rfcx-0.3.1/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     1010 2023-05-05 10:35:50.000000 rfcx-0.3.1/setup.py
```

### Comparing `rfcx-0.3.0/PKG-INFO` & `rfcx-0.3.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rfcx
-Version: 0.3.0
+Version: 0.3.1
 Summary: Client SDK for the Rainforest Connection and Arbimon platforms
 Home-page: https://github.com/rfcx/rfcx-sdk-python
 Author: Rainforest Connection
 Author-email: antony@rfcx.org
 License: None
 Platform: UNKNOWN
 Classifier: Development Status :: 1 - Planning
```

### Comparing `rfcx-0.3.0/rfcx.egg-info/PKG-INFO` & `rfcx-0.3.1/rfcx.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rfcx
-Version: 0.3.0
+Version: 0.3.1
 Summary: Client SDK for the Rainforest Connection and Arbimon platforms
 Home-page: https://github.com/rfcx/rfcx-sdk-python
 Author: Rainforest Connection
 Author-email: antony@rfcx.org
 License: None
 Platform: UNKNOWN
 Classifier: Development Status :: 1 - Planning
```

