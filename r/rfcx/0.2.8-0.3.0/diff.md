# Comparing `tmp/rfcx-0.2.8.tar.gz` & `tmp/rfcx-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rfcx-0.2.8.tar", last modified: Fri Mar  3 09:47:53 2023, max compression
+gzip compressed data, was "rfcx-0.3.0.tar", last modified: Fri May  5 09:40:56 2023, max compression
```

## Comparing `rfcx-0.2.8.tar` & `rfcx-0.3.0.tar`

### file list

```diff
@@ -1,22 +1,10 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-03 09:47:53.487356 rfcx-0.2.8/
--rw-r--r--   0 root         (0) root         (0)      644 2023-03-03 09:47:53.485868 rfcx-0.2.8/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-03 09:47:53.453057 rfcx-0.2.8/rfcx/
--rw-r--r--   0 root         (0) root         (0)      283 2022-12-16 14:56:19.000000 rfcx-0.2.8/rfcx/__init__.py
--rw-r--r--   0 root         (0) root         (0)     5408 2022-12-16 14:56:19.000000 rfcx-0.2.8/rfcx/_api_auth.py
--rw-r--r--   0 root         (0) root         (0)     4335 2022-12-20 10:55:51.000000 rfcx-0.2.8/rfcx/_api_rfcx.py
--rw-r--r--   0 root         (0) root         (0)     5493 2023-02-27 10:08:48.000000 rfcx-0.2.8/rfcx/_audio.py
--rw-r--r--   0 root         (0) root         (0)     6286 2022-12-16 14:56:19.000000 rfcx-0.2.8/rfcx/_authentication.py
--rw-r--r--   0 root         (0) root         (0)     1459 2022-12-16 14:56:19.000000 rfcx-0.2.8/rfcx/_credentials.py
--rw-r--r--   0 root         (0) root         (0)    10851 2022-12-16 14:56:19.000000 rfcx-0.2.8/rfcx/_helper.py
--rw-r--r--   0 root         (0) root         (0)     2787 2023-03-03 09:42:14.000000 rfcx-0.2.8/rfcx/_ingest.py
--rw-r--r--   0 root         (0) root         (0)     2081 2022-12-16 14:56:19.000000 rfcx-0.2.8/rfcx/_pkce.py
--rw-r--r--   0 root         (0) root         (0)      388 2022-12-16 14:56:19.000000 rfcx-0.2.8/rfcx/_util.py
--rw-r--r--   0 root         (0) root         (0)    13370 2023-02-27 12:56:06.000000 rfcx-0.2.8/rfcx/client.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-03-03 09:47:53.480583 rfcx-0.2.8/rfcx.egg-info/
--rw-r--r--   0 root         (0) root         (0)      644 2023-03-03 09:47:53.000000 rfcx-0.2.8/rfcx.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      335 2023-03-03 09:47:53.000000 rfcx-0.2.8/rfcx.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-03-03 09:47:53.000000 rfcx-0.2.8/rfcx.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       22 2023-03-03 09:47:53.000000 rfcx-0.2.8/rfcx.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        5 2023-03-03 09:47:53.000000 rfcx-0.2.8/rfcx.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-03-03 09:47:53.488253 rfcx-0.2.8/setup.cfg
--rw-r--r--   0 root         (0) root         (0)     1001 2023-03-03 09:47:13.000000 rfcx-0.2.8/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 09:40:56.660449 rfcx-0.3.0/
+-rw-r--r--   0 root         (0) root         (0)      651 2023-05-05 09:40:56.658898 rfcx-0.3.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     2955 2023-05-05 09:40:52.000000 rfcx-0.3.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 09:40:56.654523 rfcx-0.3.0/rfcx.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      651 2023-05-05 09:40:56.000000 rfcx-0.3.0/rfcx.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      148 2023-05-05 09:40:56.000000 rfcx-0.3.0/rfcx.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-05 09:40:56.000000 rfcx-0.3.0/rfcx.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       40 2023-05-05 09:40:56.000000 rfcx-0.3.0/rfcx.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-05 09:40:56.000000 rfcx-0.3.0/rfcx.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-05-05 09:40:56.661629 rfcx-0.3.0/setup.cfg
```

### Comparing `rfcx-0.2.8/PKG-INFO` & `rfcx-0.3.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 Metadata-Version: 2.1
 Name: rfcx
-Version: 0.2.8
-Summary: Python client SDK for connecting to the Rainforest Connection platform
+Version: 0.3.0
+Summary: Client SDK for the Rainforest Connection and Arbimon platforms
 Home-page: https://github.com/rfcx/rfcx-sdk-python
 Author: Rainforest Connection
 Author-email: antony@rfcx.org
 License: None
+Platform: UNKNOWN
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Science/Research
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 
-[See the documentation](https://rfcx.github.io/rfcx-sdk-python/) or [try an example](https://gist.github.com/antonyharfield/93231b3df86cd58fecee4f4d1ec9cc5b)
+[See the documentation](https://rfcx.github.io/rfcx-sdk-python/) and [try the examples](https://github.com/rfcx/rfcx-sdk-python/tree/master/package-rfcx)
+
```

### Comparing `rfcx-0.2.8/rfcx.egg-info/PKG-INFO` & `rfcx-0.3.0/rfcx.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,17 @@
 Metadata-Version: 2.1
 Name: rfcx
-Version: 0.2.8
-Summary: Python client SDK for connecting to the Rainforest Connection platform
+Version: 0.3.0
+Summary: Client SDK for the Rainforest Connection and Arbimon platforms
 Home-page: https://github.com/rfcx/rfcx-sdk-python
 Author: Rainforest Connection
 Author-email: antony@rfcx.org
 License: None
+Platform: UNKNOWN
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Science/Research
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 
-[See the documentation](https://rfcx.github.io/rfcx-sdk-python/) or [try an example](https://gist.github.com/antonyharfield/93231b3df86cd58fecee4f4d1ec9cc5b)
+[See the documentation](https://rfcx.github.io/rfcx-sdk-python/) and [try the examples](https://github.com/rfcx/rfcx-sdk-python/tree/master/package-rfcx)
+
```

