# Comparing `tmp/merqube_client_lib-0.4.0.tar.gz` & `tmp/merqube_client_lib-0.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "merqube_client_lib-0.4.0.tar", max compression
+gzip compressed data, was "merqube_client_lib-0.5.0.tar", max compression
```

## Comparing `merqube_client_lib-0.4.0.tar` & `merqube_client_lib-0.5.0.tar`

### file list

```diff
@@ -1,15 +1,16 @@
--rw-r--r--   0        0        0    11357 2023-05-04 10:20:34.258592 merqube_client_lib-0.4.0/LICENSE
--rw-r--r--   0        0        0      377 2023-05-04 10:20:34.258592 merqube_client_lib-0.4.0/README.md
--rw-r--r--   0        0        0        0 2023-05-04 10:20:34.258592 merqube_client_lib-0.4.0/merqube_client_lib/__init__.py
--rw-r--r--   0        0        0      367 2023-05-04 10:20:34.258592 merqube_client_lib-0.4.0/merqube_client_lib/constants.py
--rw-r--r--   0        0        0      482 2023-05-04 10:20:34.258592 merqube_client_lib-0.4.0/merqube_client_lib/exceptions.py
--rw-r--r--   0        0        0     1934 2023-05-04 10:20:34.258592 merqube_client_lib-0.4.0/merqube_client_lib/logging.py
--rw-r--r--   0        0        0     3022 2023-05-04 10:20:34.258592 merqube_client_lib-0.4.0/merqube_client_lib/mocker.py
--rw-r--r--   0        0        0        0 2023-05-04 10:20:34.258592 merqube_client_lib-0.4.0/merqube_client_lib/py.typed
--rw-r--r--   0        0        0        0 2023-05-04 10:20:34.258592 merqube_client_lib-0.4.0/merqube_client_lib/secapi/__init__.py
--rw-r--r--   0        0        0     4930 2023-05-04 10:20:34.262593 merqube_client_lib-0.4.0/merqube_client_lib/secapi/client.py
--rw-r--r--   0        0        0    11209 2023-05-04 10:20:34.262593 merqube_client_lib-0.4.0/merqube_client_lib/session.py
--rw-r--r--   0        0        0      351 2023-05-04 10:20:34.262593 merqube_client_lib-0.4.0/merqube_client_lib/types/__init__.py
--rw-r--r--   0        0        0      418 2023-05-04 10:20:34.262593 merqube_client_lib-0.4.0/merqube_client_lib/types/secapi.py
--rw-r--r--   0        0        0     1713 2023-05-04 10:20:34.262593 merqube_client_lib-0.4.0/pyproject.toml
--rw-r--r--   0        0        0     1079 1970-01-01 00:00:00.000000 merqube_client_lib-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-05-04 22:45:53.374877 merqube_client_lib-0.5.0/LICENSE
+-rw-r--r--   0        0        0      377 2023-05-04 22:45:53.378877 merqube_client_lib-0.5.0/README.md
+-rw-r--r--   0        0        0        0 2023-05-04 22:45:53.378877 merqube_client_lib-0.5.0/merqube_client_lib/__init__.py
+-rw-r--r--   0        0        0      367 2023-05-04 22:45:53.378877 merqube_client_lib-0.5.0/merqube_client_lib/constants.py
+-rw-r--r--   0        0        0      482 2023-05-04 22:45:53.378877 merqube_client_lib-0.5.0/merqube_client_lib/exceptions.py
+-rw-r--r--   0        0        0     1934 2023-05-04 22:45:53.378877 merqube_client_lib-0.5.0/merqube_client_lib/logging.py
+-rw-r--r--   0        0        0     3022 2023-05-04 22:45:53.378877 merqube_client_lib-0.5.0/merqube_client_lib/mocker.py
+-rw-r--r--   0        0        0        0 2023-05-04 22:45:53.378877 merqube_client_lib-0.5.0/merqube_client_lib/py.typed
+-rw-r--r--   0        0        0        0 2023-05-04 22:45:53.378877 merqube_client_lib-0.5.0/merqube_client_lib/secapi/__init__.py
+-rw-r--r--   0        0        0    12563 2023-05-04 22:45:53.378877 merqube_client_lib-0.5.0/merqube_client_lib/secapi/client.py
+-rw-r--r--   0        0        0    11209 2023-05-04 22:45:53.378877 merqube_client_lib-0.5.0/merqube_client_lib/session.py
+-rw-r--r--   0        0        0      351 2023-05-04 22:45:53.378877 merqube_client_lib-0.5.0/merqube_client_lib/types/__init__.py
+-rw-r--r--   0        0        0      418 2023-05-04 22:45:53.378877 merqube_client_lib-0.5.0/merqube_client_lib/types/secapi.py
+-rw-r--r--   0        0        0      677 2023-05-04 22:45:53.378877 merqube_client_lib-0.5.0/merqube_client_lib/util.py
+-rw-r--r--   0        0        0     1713 2023-05-04 22:45:53.378877 merqube_client_lib-0.5.0/pyproject.toml
+-rw-r--r--   0        0        0     1079 1970-01-01 00:00:00.000000 merqube_client_lib-0.5.0/PKG-INFO
```

### Comparing `merqube_client_lib-0.4.0/LICENSE` & `merqube_client_lib-0.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `merqube_client_lib-0.4.0/merqube_client_lib/logging.py` & `merqube_client_lib-0.5.0/merqube_client_lib/logging.py`

 * *Files identical despite different names*

### Comparing `merqube_client_lib-0.4.0/merqube_client_lib/mocker.py` & `merqube_client_lib-0.5.0/merqube_client_lib/mocker.py`

 * *Files identical despite different names*

### Comparing `merqube_client_lib-0.4.0/merqube_client_lib/session.py` & `merqube_client_lib-0.5.0/merqube_client_lib/session.py`

 * *Files identical despite different names*

### Comparing `merqube_client_lib-0.4.0/pyproject.toml` & `merqube_client_lib-0.5.0/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "merqube-client-lib"
-version = "0.4.0"
+version = "0.5.0"
 description = "MerQube IndexAPI + SecAPI client library"
 authors = ["Merqube"]
 readme = "README.md"
 license = "APACHE-2.0"
 homepage = "https://github.com/merqube/merqube-client-lib"
 include = [
     "LICENSE",
```

### Comparing `merqube_client_lib-0.4.0/PKG-INFO` & `merqube_client_lib-0.5.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: merqube-client-lib
-Version: 0.4.0
+Version: 0.5.0
 Summary: MerQube IndexAPI + SecAPI client library
 Home-page: https://github.com/merqube/merqube-client-lib
 License: Apache-2.0
 Author: Merqube
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
```

