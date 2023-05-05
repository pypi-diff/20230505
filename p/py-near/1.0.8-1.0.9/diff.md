# Comparing `tmp/py-near-1.0.8.tar.gz` & `tmp/py-near-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py-near-1.0.8.tar", last modified: Wed Jan 25 01:43:24 2023, max compression
+gzip compressed data, was "py-near-1.0.9.tar", last modified: Thu Feb 16 18:56:28 2023, max compression
```

## Comparing `py-near-1.0.8.tar` & `py-near-1.0.9.tar`

### file list

```diff
@@ -1,49 +1,49 @@
-drwxr-xr-x   0 petrvolnov   (501) staff       (20)        0 2023-01-25 01:43:24.764380 py-near-1.0.8/
--rw-r--r--   0 petrvolnov   (501) staff       (20)     1023 2022-06-08 20:31:53.000000 py-near-1.0.8/LICENSE
--rw-r--r--   0 petrvolnov   (501) staff       (20)     6013 2023-01-25 01:43:24.764177 py-near-1.0.8/PKG-INFO
--rw-r--r--   0 petrvolnov   (501) staff       (20)     3974 2023-01-24 19:13:04.000000 py-near-1.0.8/README.md
--rw-r--r--   0 petrvolnov   (501) staff       (20)     1550 2023-01-25 01:39:39.000000 py-near-1.0.8/pyproject.toml
--rw-r--r--   0 petrvolnov   (501) staff       (20)       38 2023-01-25 01:43:24.764423 py-near-1.0.8/setup.cfg
-drwxr-xr-x   0 petrvolnov   (501) staff       (20)        0 2023-01-25 01:43:24.754859 py-near-1.0.8/src/
-drwxr-xr-x   0 petrvolnov   (501) staff       (20)        0 2023-01-25 01:43:24.757904 py-near-1.0.8/src/py_near/
--rw-r--r--   0 petrvolnov   (501) staff       (20)       50 2023-01-24 19:13:04.000000 py-near-1.0.8/src/py_near/__init__.py
--rw-r--r--   0 petrvolnov   (501) staff       (20)    13347 2023-01-25 01:37:42.000000 py-near-1.0.8/src/py_near/account.py
--rw-r--r--   0 petrvolnov   (501) staff       (20)      163 2023-01-24 19:13:04.000000 py-near-1.0.8/src/py_near/constants.py
-drwxr-xr-x   0 petrvolnov   (501) staff       (20)        0 2023-01-25 01:43:24.759642 py-near-1.0.8/src/py_near/dapps/
--rw-r--r--   0 petrvolnov   (501) staff       (20)        0 2023-01-24 19:13:04.000000 py-near-1.0.8/src/py_near/dapps/__init__.py
--rw-r--r--   0 petrvolnov   (501) staff       (20)      231 2023-01-24 19:13:04.000000 py-near-1.0.8/src/py_near/dapps/core.py
-drwxr-xr-x   0 petrvolnov   (501) staff       (20)        0 2023-01-25 01:43:24.760455 py-near-1.0.8/src/py_near/dapps/ft/
--rw-r--r--   0 petrvolnov   (501) staff       (20)       29 2023-01-24 19:13:04.000000 py-near-1.0.8/src/py_near/dapps/ft/__init__.py
--rw-r--r--   0 petrvolnov   (501) staff       (20)     6717 2023-01-24 19:13:04.000000 py-near-1.0.8/src/py_near/dapps/ft/async_client.py
--rw-r--r--   0 petrvolnov   (501) staff       (20)       92 2023-01-24 19:13:04.000000 py-near-1.0.8/src/py_near/dapps/ft/exceptions.py
--rw-r--r--   0 petrvolnov   (501) staff       (20)      186 2023-01-24 19:13:04.000000 py-near-1.0.8/src/py_near/dapps/ft/models.py
--rw-r--r--   0 petrvolnov   (501) staff       (20)      856 2023-01-24 19:13:04.000000 py-near-1.0.8/src/py_near/dapps/fts.py
-drwxr-xr-x   0 petrvolnov   (501) staff       (20)        0 2023-01-25 01:43:24.761386 py-near-1.0.8/src/py_near/dapps/keypom/
--rw-r--r--   0 petrvolnov   (501) staff       (20)       32 2023-01-24 19:13:04.000000 py-near-1.0.8/src/py_near/dapps/keypom/__init__.py
--rw-r--r--   0 petrvolnov   (501) staff       (20)     1422 2023-01-24 19:13:04.000000 py-near-1.0.8/src/py_near/dapps/keypom/async_client.py
--rw-r--r--   0 petrvolnov   (501) staff       (20)       45 2023-01-24 19:13:04.000000 py-near-1.0.8/src/py_near/dapps/keypom/exceptions.py
--rw-r--r--   0 petrvolnov   (501) staff       (20)     2166 2023-01-24 19:13:04.000000 py-near-1.0.8/src/py_near/dapps/keypom/models.py
-drwxr-xr-x   0 petrvolnov   (501) staff       (20)        0 2023-01-25 01:43:24.762140 py-near-1.0.8/src/py_near/dapps/phone/
--rw-r--r--   0 petrvolnov   (501) staff       (20)       32 2023-01-24 19:13:04.000000 py-near-1.0.8/src/py_near/dapps/phone/__init__.py
--rw-r--r--   0 petrvolnov   (501) staff       (20)     6849 2023-01-24 19:13:04.000000 py-near-1.0.8/src/py_near/dapps/phone/async_client.py
--rw-r--r--   0 petrvolnov   (501) staff       (20)       45 2023-01-24 19:13:04.000000 py-near-1.0.8/src/py_near/dapps/phone/exceptions.py
--rw-r--r--   0 petrvolnov   (501) staff       (20)      332 2023-01-24 19:13:04.000000 py-near-1.0.8/src/py_near/dapps/phone/models.py
-drwxr-xr-x   0 petrvolnov   (501) staff       (20)        0 2023-01-25 01:43:24.763005 py-near-1.0.8/src/py_near/dapps/staking/
--rw-r--r--   0 petrvolnov   (501) staff       (20)       34 2023-01-24 19:13:04.000000 py-near-1.0.8/src/py_near/dapps/staking/__init__.py
--rw-r--r--   0 petrvolnov   (501) staff       (20)     5203 2023-01-24 19:13:04.000000 py-near-1.0.8/src/py_near/dapps/staking/async_client.py
--rw-r--r--   0 petrvolnov   (501) staff       (20)       92 2023-01-24 19:13:04.000000 py-near-1.0.8/src/py_near/dapps/staking/exceptions.py
--rw-r--r--   0 petrvolnov   (501) staff       (20)      124 2023-01-24 19:13:04.000000 py-near-1.0.8/src/py_near/dapps/staking/models.py
-drwxr-xr-x   0 petrvolnov   (501) staff       (20)        0 2023-01-25 01:43:24.763845 py-near-1.0.8/src/py_near/exceptions/
--rw-r--r--   0 petrvolnov   (501) staff       (20)        0 2023-01-24 19:13:04.000000 py-near-1.0.8/src/py_near/exceptions/__init__.py
--rw-r--r--   0 petrvolnov   (501) staff       (20)     4617 2023-01-25 01:37:42.000000 py-near-1.0.8/src/py_near/exceptions/exceptions.py
--rw-r--r--   0 petrvolnov   (501) staff       (20)     7642 2023-01-24 19:13:04.000000 py-near-1.0.8/src/py_near/exceptions/provider.py
--rw-r--r--   0 petrvolnov   (501) staff       (20)     3800 2023-01-25 01:38:09.000000 py-near-1.0.8/src/py_near/models.py
--rw-r--r--   0 petrvolnov   (501) staff       (20)     7792 2023-01-25 01:39:39.000000 py-near-1.0.8/src/py_near/providers.py
--rw-r--r--   0 petrvolnov   (501) staff       (20)     2330 2023-01-24 19:13:04.000000 py-near-1.0.8/src/py_near/transactions.py
--rw-r--r--   0 petrvolnov   (501) staff       (20)     1528 2023-01-24 19:13:04.000000 py-near-1.0.8/src/py_near/utils.py
-drwxr-xr-x   0 petrvolnov   (501) staff       (20)        0 2023-01-25 01:43:24.759113 py-near-1.0.8/src/py_near.egg-info/
--rw-r--r--   0 petrvolnov   (501) staff       (20)     6013 2023-01-25 01:43:24.000000 py-near-1.0.8/src/py_near.egg-info/PKG-INFO
--rw-r--r--   0 petrvolnov   (501) staff       (20)     1154 2023-01-25 01:43:24.000000 py-near-1.0.8/src/py_near.egg-info/SOURCES.txt
--rw-r--r--   0 petrvolnov   (501) staff       (20)        1 2023-01-25 01:43:24.000000 py-near-1.0.8/src/py_near.egg-info/dependency_links.txt
--rw-r--r--   0 petrvolnov   (501) staff       (20)       40 2023-01-25 01:43:24.000000 py-near-1.0.8/src/py_near.egg-info/requires.txt
--rw-r--r--   0 petrvolnov   (501) staff       (20)        8 2023-01-25 01:43:24.000000 py-near-1.0.8/src/py_near.egg-info/top_level.txt
+drwxr-xr-x   0 petrvolnov   (501) staff       (20)        0 2023-02-16 18:56:28.858235 py-near-1.0.9/
+-rw-r--r--   0 petrvolnov   (501) staff       (20)     1023 2022-06-08 20:31:53.000000 py-near-1.0.9/LICENSE
+-rw-r--r--   0 petrvolnov   (501) staff       (20)     6013 2023-02-16 18:56:28.858077 py-near-1.0.9/PKG-INFO
+-rw-r--r--   0 petrvolnov   (501) staff       (20)     3974 2023-01-24 19:13:04.000000 py-near-1.0.9/README.md
+-rw-r--r--   0 petrvolnov   (501) staff       (20)     1550 2023-02-16 18:54:32.000000 py-near-1.0.9/pyproject.toml
+-rw-r--r--   0 petrvolnov   (501) staff       (20)       38 2023-02-16 18:56:28.858281 py-near-1.0.9/setup.cfg
+drwxr-xr-x   0 petrvolnov   (501) staff       (20)        0 2023-02-16 18:56:28.849878 py-near-1.0.9/src/
+drwxr-xr-x   0 petrvolnov   (501) staff       (20)        0 2023-02-16 18:56:28.852521 py-near-1.0.9/src/py_near/
+-rw-r--r--   0 petrvolnov   (501) staff       (20)       50 2023-01-24 19:13:04.000000 py-near-1.0.9/src/py_near/__init__.py
+-rw-r--r--   0 petrvolnov   (501) staff       (20)    13347 2023-02-16 18:28:35.000000 py-near-1.0.9/src/py_near/account.py
+-rw-r--r--   0 petrvolnov   (501) staff       (20)      163 2023-01-24 19:13:04.000000 py-near-1.0.9/src/py_near/constants.py
+drwxr-xr-x   0 petrvolnov   (501) staff       (20)        0 2023-02-16 18:56:28.853797 py-near-1.0.9/src/py_near/dapps/
+-rw-r--r--   0 petrvolnov   (501) staff       (20)        0 2023-01-24 19:13:04.000000 py-near-1.0.9/src/py_near/dapps/__init__.py
+-rw-r--r--   0 petrvolnov   (501) staff       (20)      231 2023-01-24 19:13:04.000000 py-near-1.0.9/src/py_near/dapps/core.py
+drwxr-xr-x   0 petrvolnov   (501) staff       (20)        0 2023-02-16 18:56:28.854684 py-near-1.0.9/src/py_near/dapps/ft/
+-rw-r--r--   0 petrvolnov   (501) staff       (20)       29 2023-01-24 19:13:04.000000 py-near-1.0.9/src/py_near/dapps/ft/__init__.py
+-rw-r--r--   0 petrvolnov   (501) staff       (20)     6717 2023-01-24 19:13:04.000000 py-near-1.0.9/src/py_near/dapps/ft/async_client.py
+-rw-r--r--   0 petrvolnov   (501) staff       (20)       92 2023-01-24 19:13:04.000000 py-near-1.0.9/src/py_near/dapps/ft/exceptions.py
+-rw-r--r--   0 petrvolnov   (501) staff       (20)      186 2023-01-24 19:13:04.000000 py-near-1.0.9/src/py_near/dapps/ft/models.py
+-rw-r--r--   0 petrvolnov   (501) staff       (20)      856 2023-01-24 19:13:04.000000 py-near-1.0.9/src/py_near/dapps/fts.py
+drwxr-xr-x   0 petrvolnov   (501) staff       (20)        0 2023-02-16 18:56:28.855712 py-near-1.0.9/src/py_near/dapps/keypom/
+-rw-r--r--   0 petrvolnov   (501) staff       (20)       32 2023-01-24 19:13:04.000000 py-near-1.0.9/src/py_near/dapps/keypom/__init__.py
+-rw-r--r--   0 petrvolnov   (501) staff       (20)     1422 2023-01-24 19:13:04.000000 py-near-1.0.9/src/py_near/dapps/keypom/async_client.py
+-rw-r--r--   0 petrvolnov   (501) staff       (20)       45 2023-01-24 19:13:04.000000 py-near-1.0.9/src/py_near/dapps/keypom/exceptions.py
+-rw-r--r--   0 petrvolnov   (501) staff       (20)     2166 2023-01-24 19:13:04.000000 py-near-1.0.9/src/py_near/dapps/keypom/models.py
+drwxr-xr-x   0 petrvolnov   (501) staff       (20)        0 2023-02-16 18:56:28.856505 py-near-1.0.9/src/py_near/dapps/phone/
+-rw-r--r--   0 petrvolnov   (501) staff       (20)       32 2023-01-24 19:13:04.000000 py-near-1.0.9/src/py_near/dapps/phone/__init__.py
+-rw-r--r--   0 petrvolnov   (501) staff       (20)     6849 2023-01-24 19:13:04.000000 py-near-1.0.9/src/py_near/dapps/phone/async_client.py
+-rw-r--r--   0 petrvolnov   (501) staff       (20)       45 2023-01-24 19:13:04.000000 py-near-1.0.9/src/py_near/dapps/phone/exceptions.py
+-rw-r--r--   0 petrvolnov   (501) staff       (20)      332 2023-01-24 19:13:04.000000 py-near-1.0.9/src/py_near/dapps/phone/models.py
+drwxr-xr-x   0 petrvolnov   (501) staff       (20)        0 2023-02-16 18:56:28.857273 py-near-1.0.9/src/py_near/dapps/staking/
+-rw-r--r--   0 petrvolnov   (501) staff       (20)       34 2023-01-24 19:13:04.000000 py-near-1.0.9/src/py_near/dapps/staking/__init__.py
+-rw-r--r--   0 petrvolnov   (501) staff       (20)     5203 2023-01-24 19:13:04.000000 py-near-1.0.9/src/py_near/dapps/staking/async_client.py
+-rw-r--r--   0 petrvolnov   (501) staff       (20)       92 2023-01-24 19:13:04.000000 py-near-1.0.9/src/py_near/dapps/staking/exceptions.py
+-rw-r--r--   0 petrvolnov   (501) staff       (20)      124 2023-01-24 19:13:04.000000 py-near-1.0.9/src/py_near/dapps/staking/models.py
+drwxr-xr-x   0 petrvolnov   (501) staff       (20)        0 2023-02-16 18:56:28.857823 py-near-1.0.9/src/py_near/exceptions/
+-rw-r--r--   0 petrvolnov   (501) staff       (20)        0 2023-01-24 19:13:04.000000 py-near-1.0.9/src/py_near/exceptions/__init__.py
+-rw-r--r--   0 petrvolnov   (501) staff       (20)     4617 2023-01-25 01:37:42.000000 py-near-1.0.9/src/py_near/exceptions/exceptions.py
+-rw-r--r--   0 petrvolnov   (501) staff       (20)     7642 2023-01-24 19:13:04.000000 py-near-1.0.9/src/py_near/exceptions/provider.py
+-rw-r--r--   0 petrvolnov   (501) staff       (20)     6418 2023-02-16 18:54:14.000000 py-near-1.0.9/src/py_near/models.py
+-rw-r--r--   0 petrvolnov   (501) staff       (20)     8053 2023-01-29 18:06:54.000000 py-near-1.0.9/src/py_near/providers.py
+-rw-r--r--   0 petrvolnov   (501) staff       (20)     2330 2023-01-24 19:13:04.000000 py-near-1.0.9/src/py_near/transactions.py
+-rw-r--r--   0 petrvolnov   (501) staff       (20)     1528 2023-01-24 19:13:04.000000 py-near-1.0.9/src/py_near/utils.py
+drwxr-xr-x   0 petrvolnov   (501) staff       (20)        0 2023-02-16 18:56:28.853356 py-near-1.0.9/src/py_near.egg-info/
+-rw-r--r--   0 petrvolnov   (501) staff       (20)     6013 2023-02-16 18:56:28.000000 py-near-1.0.9/src/py_near.egg-info/PKG-INFO
+-rw-r--r--   0 petrvolnov   (501) staff       (20)     1154 2023-02-16 18:56:28.000000 py-near-1.0.9/src/py_near.egg-info/SOURCES.txt
+-rw-r--r--   0 petrvolnov   (501) staff       (20)        1 2023-02-16 18:56:28.000000 py-near-1.0.9/src/py_near.egg-info/dependency_links.txt
+-rw-r--r--   0 petrvolnov   (501) staff       (20)       40 2023-02-16 18:56:28.000000 py-near-1.0.9/src/py_near.egg-info/requires.txt
+-rw-r--r--   0 petrvolnov   (501) staff       (20)        8 2023-02-16 18:56:28.000000 py-near-1.0.9/src/py_near.egg-info/top_level.txt
```

### Comparing `py-near-1.0.8/LICENSE` & `py-near-1.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `py-near-1.0.8/PKG-INFO` & `py-near-1.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py-near
-Version: 1.0.8
+Version: 1.0.9
 Summary: Pretty simple and fully asynchronous framework for working with NEAR blockchaink
 Author-email: pvolnov <petr@herewallet.app>
 License: Permission is hereby granted, free of charge, to any
         person obtaining a copy of this software and associated
         documentation files (the "Software"), to deal in the
         Software without restriction, including without
         limitation the rights to use, copy, modify, merge,
```

### Comparing `py-near-1.0.8/README.md` & `py-near-1.0.9/README.md`

 * *Files identical despite different names*

### Comparing `py-near-1.0.8/pyproject.toml` & `py-near-1.0.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 flake8 = "^4.0.1"
 Sphinx = "^4.3.2"
 sphinx-rtd-theme = "^1.0.0"
 base58 = "^2.1.1"
 
 [project]
 name = "py-near"
-version = "1.0.8"
+version = "1.0.9"
 description = "Pretty simple and fully asynchronous framework for working with NEAR blockchaink"
 authors = [ {name = "pvolnov", email = "petr@herewallet.app"} ]
 requires-python = ">=3.7"
 license = {file = "LICENSE"}
 dependencies=["base58", "ed25519", "aiohttp", "pyonear", "pydantic"]
 keywords = ["python", "near", "async"]
 classifiers = [
```

### Comparing `py-near-1.0.8/src/py_near/account.py` & `py-near-1.0.9/src/py_near/account.py`

 * *Files identical despite different names*

### Comparing `py-near-1.0.8/src/py_near/dapps/ft/async_client.py` & `py-near-1.0.9/src/py_near/dapps/ft/async_client.py`

 * *Files identical despite different names*

### Comparing `py-near-1.0.8/src/py_near/dapps/fts.py` & `py-near-1.0.9/src/py_near/dapps/fts.py`

 * *Files identical despite different names*

### Comparing `py-near-1.0.8/src/py_near/dapps/keypom/async_client.py` & `py-near-1.0.9/src/py_near/dapps/keypom/async_client.py`

 * *Files identical despite different names*

### Comparing `py-near-1.0.8/src/py_near/dapps/keypom/models.py` & `py-near-1.0.9/src/py_near/dapps/keypom/models.py`

 * *Files identical despite different names*

### Comparing `py-near-1.0.8/src/py_near/dapps/phone/async_client.py` & `py-near-1.0.9/src/py_near/dapps/phone/async_client.py`

 * *Files identical despite different names*

### Comparing `py-near-1.0.8/src/py_near/dapps/staking/async_client.py` & `py-near-1.0.9/src/py_near/dapps/staking/async_client.py`

 * *Files identical despite different names*

### Comparing `py-near-1.0.8/src/py_near/exceptions/exceptions.py` & `py-near-1.0.9/src/py_near/exceptions/exceptions.py`

 * *Files identical despite different names*

### Comparing `py-near-1.0.8/src/py_near/exceptions/provider.py` & `py-near-1.0.9/src/py_near/exceptions/provider.py`

 * *Files identical despite different names*

### Comparing `py-near-1.0.8/src/py_near/providers.py` & `py-near-1.0.9/src/py_near/providers.py`

 * *Files 5% similar despite different names*

```diff
@@ -52,25 +52,27 @@
     async def call_rpc_request(self, method, params, timeout=60):
         j = {"method": method, "params": params, "id": "dontcare", "jsonrpc": "2.0"}
 
         content = None
         for rpc_addr in self._rpc_addresses:
             try:
                 async with aiohttp.ClientSession() as session:
-                    r = await session.post(rpc_addr, json=j, timeout=timeout)
+                    r = await session.post(rpc_addr, json=j, timeout=30)
                     r.raise_for_status()
                     content = json.loads(await r.text())
                 if self._rpc_addresses[0] != rpc_addr:
                     self._rpc_addresses.remove(rpc_addr)
                     self._rpc_addresses.insert(0, rpc_addr)
                 break
             except ClientResponseError:
                 continue
             except ClientConnectorError:
                 continue
+            except RpcTimeoutError:
+                continue
             except ConnectionError:
                 continue
         return content
 
     @staticmethod
     def get_error_from_response(content: dict):
         if "error" in content:
@@ -154,14 +156,21 @@
                 "request_type": "view_access_key_list",
                 "account_id": account_id,
                 "finality": finality,
             },
         )
 
     async def get_access_key(self, account_id, public_key, finality="optimistic"):
+        """
+
+        :param account_id:
+        :param public_key:
+        :param finality:
+        :return: {'block_hash': '..', 'block_height': int, 'nonce': int, 'permission': 'FullAccess'}
+        """
         return await self.json_rpc(
             "query",
             {
                 "request_type": "view_access_key",
                 "account_id": account_id,
                 "public_key": public_key,
                 "finality": finality,
```

### Comparing `py-near-1.0.8/src/py_near/transactions.py` & `py-near-1.0.9/src/py_near/transactions.py`

 * *Files identical despite different names*

### Comparing `py-near-1.0.8/src/py_near/utils.py` & `py-near-1.0.9/src/py_near/utils.py`

 * *Files identical despite different names*

### Comparing `py-near-1.0.8/src/py_near.egg-info/PKG-INFO` & `py-near-1.0.9/src/py_near.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py-near
-Version: 1.0.8
+Version: 1.0.9
 Summary: Pretty simple and fully asynchronous framework for working with NEAR blockchaink
 Author-email: pvolnov <petr@herewallet.app>
 License: Permission is hereby granted, free of charge, to any
         person obtaining a copy of this software and associated
         documentation files (the "Software"), to deal in the
         Software without restriction, including without
         limitation the rights to use, copy, modify, merge,
```

### Comparing `py-near-1.0.8/src/py_near.egg-info/SOURCES.txt` & `py-near-1.0.9/src/py_near.egg-info/SOURCES.txt`

 * *Files identical despite different names*

