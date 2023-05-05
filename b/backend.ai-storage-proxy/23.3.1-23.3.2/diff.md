# Comparing `tmp/backend.ai-storage-proxy-23.3.1.tar.gz` & `tmp/backend.ai-storage-proxy-23.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "backend.ai-storage-proxy-23.3.1.tar", last modified: Thu May  4 05:10:16 2023, max compression
+gzip compressed data, was "backend.ai-storage-proxy-23.3.2.tar", last modified: Fri May  5 07:08:21 2023, max compression
```

## Comparing `backend.ai-storage-proxy-23.3.1.tar` & `backend.ai-storage-proxy-23.3.2.tar`

### file list

```diff
@@ -1,53 +1,53 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 05:10:16.954679 backend.ai-storage-proxy-23.3.1/
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-04 05:10:16.000000 backend.ai-storage-proxy-23.3.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     6684 2023-05-04 05:10:16.954679 backend.ai-storage-proxy-23.3.1/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 05:10:16.950679 backend.ai-storage-proxy-23.3.1/ai/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 05:10:16.950679 backend.ai-storage-proxy-23.3.1/ai/backend/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 05:10:16.950679 backend.ai-storage-proxy-23.3.1/ai/backend/storage/
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-04 05:10:16.000000 backend.ai-storage-proxy-23.3.1/ai/backend/storage/VERSION
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-04 05:10:16.000000 backend.ai-storage-proxy-23.3.1/ai/backend/storage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6431 2023-05-04 05:10:16.000000 backend.ai-storage-proxy-23.3.1/ai/backend/storage/abc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 05:10:16.950679 backend.ai-storage-proxy-23.3.1/ai/backend/storage/api/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 05:10:16.000000 backend.ai-storage-proxy-23.3.1/ai/backend/storage/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13343 2023-05-04 05:10:16.000000 backend.ai-storage-proxy-23.3.1/ai/backend/storage/api/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    23528 2023-05-04 05:10:16.000000 backend.ai-storage-proxy-23.3.1/ai/backend/storage/api/manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 05:10:16.950679 backend.ai-storage-proxy-23.3.1/ai/backend/storage/cephfs/
--rw-r--r--   0 runner    (1001) docker     (123)     3348 2023-05-04 05:10:16.000000 backend.ai-storage-proxy-23.3.1/ai/backend/storage/cephfs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4629 2023-05-04 05:10:16.000000 backend.ai-storage-proxy-23.3.1/ai/backend/storage/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     2025 2023-05-04 05:10:16.000000 backend.ai-storage-proxy-23.3.1/ai/backend/storage/context.py
--rw-r--r--   0 runner    (1001) docker     (123)     1034 2023-05-04 05:10:16.000000 backend.ai-storage-proxy-23.3.1/ai/backend/storage/exception.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 05:10:16.950679 backend.ai-storage-proxy-23.3.1/ai/backend/storage/gpfs/
--rw-r--r--   0 runner    (1001) docker     (123)     6490 2023-05-04 05:10:16.000000 backend.ai-storage-proxy-23.3.1/ai/backend/storage/gpfs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      721 2023-05-04 05:10:16.000000 backend.ai-storage-proxy-23.3.1/ai/backend/storage/gpfs/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    12362 2023-05-04 05:10:16.000000 backend.ai-storage-proxy-23.3.1/ai/backend/storage/gpfs/gpfs_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     5462 2023-05-04 05:10:16.000000 backend.ai-storage-proxy-23.3.1/ai/backend/storage/gpfs/types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 05:10:16.950679 backend.ai-storage-proxy-23.3.1/ai/backend/storage/netapp/
--rw-r--r--   0 runner    (1001) docker     (123)    14060 2023-05-04 05:10:16.000000 backend.ai-storage-proxy-23.3.1/ai/backend/storage/netapp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8329 2023-05-04 05:10:16.000000 backend.ai-storage-proxy-23.3.1/ai/backend/storage/netapp/netappclient.py
--rw-r--r--   0 runner    (1001) docker     (123)     5332 2023-05-04 05:10:16.000000 backend.ai-storage-proxy-23.3.1/ai/backend/storage/netapp/quotamanager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 05:10:16.950679 backend.ai-storage-proxy-23.3.1/ai/backend/storage/purestorage/
--rw-r--r--   0 runner    (1001) docker     (123)     9318 2023-05-04 05:10:16.000000 backend.ai-storage-proxy-23.3.1/ai/backend/storage/purestorage/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4946 2023-05-04 05:10:16.000000 backend.ai-storage-proxy-23.3.1/ai/backend/storage/purestorage/purity.py
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-04 05:10:16.000000 backend.ai-storage-proxy-23.3.1/ai/backend/storage/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     8726 2023-05-04 05:10:16.000000 backend.ai-storage-proxy-23.3.1/ai/backend/storage/server.py
--rw-r--r--   0 runner    (1001) docker     (123)     2252 2023-05-04 05:10:16.000000 backend.ai-storage-proxy-23.3.1/ai/backend/storage/types.py
--rw-r--r--   0 runner    (1001) docker     (123)     3924 2023-05-04 05:10:16.000000 backend.ai-storage-proxy-23.3.1/ai/backend/storage/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 05:10:16.950679 backend.ai-storage-proxy-23.3.1/ai/backend/storage/vfs/
--rw-r--r--   0 runner    (1001) docker     (123)    16485 2023-05-04 05:10:16.000000 backend.ai-storage-proxy-23.3.1/ai/backend/storage/vfs/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 05:10:16.954679 backend.ai-storage-proxy-23.3.1/ai/backend/storage/weka/
--rw-r--r--   0 runner    (1001) docker     (123)     6243 2023-05-04 05:10:16.000000 backend.ai-storage-proxy-23.3.1/ai/backend/storage/weka/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      622 2023-05-04 05:10:16.000000 backend.ai-storage-proxy-23.3.1/ai/backend/storage/weka/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)    12747 2023-05-04 05:10:16.000000 backend.ai-storage-proxy-23.3.1/ai/backend/storage/weka/weka_client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 05:10:16.954679 backend.ai-storage-proxy-23.3.1/ai/backend/storage/xfs/
--rw-r--r--   0 runner    (1001) docker     (123)    10645 2023-05-04 05:10:16.000000 backend.ai-storage-proxy-23.3.1/ai/backend/storage/xfs/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 05:10:16.954679 backend.ai-storage-proxy-23.3.1/backend.ai_storage_proxy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6684 2023-05-04 05:10:16.000000 backend.ai-storage-proxy-23.3.1/backend.ai_storage_proxy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1342 2023-05-04 05:10:16.000000 backend.ai-storage-proxy-23.3.1/backend.ai_storage_proxy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-04 05:10:16.000000 backend.ai-storage-proxy-23.3.1/backend.ai_storage_proxy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-04 05:10:16.000000 backend.ai-storage-proxy-23.3.1/backend.ai_storage_proxy.egg-info/namespace_packages.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-04 05:10:16.000000 backend.ai-storage-proxy-23.3.1/backend.ai_storage_proxy.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      308 2023-05-04 05:10:16.000000 backend.ai-storage-proxy-23.3.1/backend.ai_storage_proxy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        3 2023-05-04 05:10:16.000000 backend.ai-storage-proxy-23.3.1/backend.ai_storage_proxy.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      626 2023-05-04 05:10:16.000000 backend.ai-storage-proxy-23.3.1/backend_shim.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-04 05:10:16.954679 backend.ai-storage-proxy-23.3.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     8004 2023-05-04 05:10:16.000000 backend.ai-storage-proxy-23.3.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 07:08:21.426488 backend.ai-storage-proxy-23.3.2/
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-05 07:08:20.000000 backend.ai-storage-proxy-23.3.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     6684 2023-05-05 07:08:21.426488 backend.ai-storage-proxy-23.3.2/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 07:08:21.418488 backend.ai-storage-proxy-23.3.2/ai/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 07:08:21.418488 backend.ai-storage-proxy-23.3.2/ai/backend/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 07:08:21.418488 backend.ai-storage-proxy-23.3.2/ai/backend/storage/
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-05 07:08:20.000000 backend.ai-storage-proxy-23.3.2/ai/backend/storage/VERSION
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-05 07:08:20.000000 backend.ai-storage-proxy-23.3.2/ai/backend/storage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6431 2023-05-05 07:08:20.000000 backend.ai-storage-proxy-23.3.2/ai/backend/storage/abc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 07:08:21.422488 backend.ai-storage-proxy-23.3.2/ai/backend/storage/api/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 07:08:20.000000 backend.ai-storage-proxy-23.3.2/ai/backend/storage/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13343 2023-05-05 07:08:20.000000 backend.ai-storage-proxy-23.3.2/ai/backend/storage/api/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23528 2023-05-05 07:08:20.000000 backend.ai-storage-proxy-23.3.2/ai/backend/storage/api/manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 07:08:21.422488 backend.ai-storage-proxy-23.3.2/ai/backend/storage/cephfs/
+-rw-r--r--   0 runner    (1001) docker     (123)     3348 2023-05-05 07:08:20.000000 backend.ai-storage-proxy-23.3.2/ai/backend/storage/cephfs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4629 2023-05-05 07:08:20.000000 backend.ai-storage-proxy-23.3.2/ai/backend/storage/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2025 2023-05-05 07:08:20.000000 backend.ai-storage-proxy-23.3.2/ai/backend/storage/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1034 2023-05-05 07:08:20.000000 backend.ai-storage-proxy-23.3.2/ai/backend/storage/exception.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 07:08:21.422488 backend.ai-storage-proxy-23.3.2/ai/backend/storage/gpfs/
+-rw-r--r--   0 runner    (1001) docker     (123)     6490 2023-05-05 07:08:20.000000 backend.ai-storage-proxy-23.3.2/ai/backend/storage/gpfs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      721 2023-05-05 07:08:20.000000 backend.ai-storage-proxy-23.3.2/ai/backend/storage/gpfs/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12362 2023-05-05 07:08:20.000000 backend.ai-storage-proxy-23.3.2/ai/backend/storage/gpfs/gpfs_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5462 2023-05-05 07:08:20.000000 backend.ai-storage-proxy-23.3.2/ai/backend/storage/gpfs/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 07:08:21.422488 backend.ai-storage-proxy-23.3.2/ai/backend/storage/netapp/
+-rw-r--r--   0 runner    (1001) docker     (123)    14060 2023-05-05 07:08:20.000000 backend.ai-storage-proxy-23.3.2/ai/backend/storage/netapp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8329 2023-05-05 07:08:20.000000 backend.ai-storage-proxy-23.3.2/ai/backend/storage/netapp/netappclient.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5332 2023-05-05 07:08:20.000000 backend.ai-storage-proxy-23.3.2/ai/backend/storage/netapp/quotamanager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 07:08:21.422488 backend.ai-storage-proxy-23.3.2/ai/backend/storage/purestorage/
+-rw-r--r--   0 runner    (1001) docker     (123)     9318 2023-05-05 07:08:20.000000 backend.ai-storage-proxy-23.3.2/ai/backend/storage/purestorage/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4946 2023-05-05 07:08:20.000000 backend.ai-storage-proxy-23.3.2/ai/backend/storage/purestorage/purity.py
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-05 07:08:20.000000 backend.ai-storage-proxy-23.3.2/ai/backend/storage/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     8726 2023-05-05 07:08:20.000000 backend.ai-storage-proxy-23.3.2/ai/backend/storage/server.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2252 2023-05-05 07:08:20.000000 backend.ai-storage-proxy-23.3.2/ai/backend/storage/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3924 2023-05-05 07:08:20.000000 backend.ai-storage-proxy-23.3.2/ai/backend/storage/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 07:08:21.422488 backend.ai-storage-proxy-23.3.2/ai/backend/storage/vfs/
+-rw-r--r--   0 runner    (1001) docker     (123)    16485 2023-05-05 07:08:20.000000 backend.ai-storage-proxy-23.3.2/ai/backend/storage/vfs/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 07:08:21.422488 backend.ai-storage-proxy-23.3.2/ai/backend/storage/weka/
+-rw-r--r--   0 runner    (1001) docker     (123)     6243 2023-05-05 07:08:20.000000 backend.ai-storage-proxy-23.3.2/ai/backend/storage/weka/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      622 2023-05-05 07:08:20.000000 backend.ai-storage-proxy-23.3.2/ai/backend/storage/weka/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12747 2023-05-05 07:08:20.000000 backend.ai-storage-proxy-23.3.2/ai/backend/storage/weka/weka_client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 07:08:21.422488 backend.ai-storage-proxy-23.3.2/ai/backend/storage/xfs/
+-rw-r--r--   0 runner    (1001) docker     (123)    10645 2023-05-05 07:08:20.000000 backend.ai-storage-proxy-23.3.2/ai/backend/storage/xfs/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 07:08:21.422488 backend.ai-storage-proxy-23.3.2/backend.ai_storage_proxy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6684 2023-05-05 07:08:21.000000 backend.ai-storage-proxy-23.3.2/backend.ai_storage_proxy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1342 2023-05-05 07:08:21.000000 backend.ai-storage-proxy-23.3.2/backend.ai_storage_proxy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 07:08:21.000000 backend.ai-storage-proxy-23.3.2/backend.ai_storage_proxy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 07:08:21.000000 backend.ai-storage-proxy-23.3.2/backend.ai_storage_proxy.egg-info/namespace_packages.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 07:08:21.000000 backend.ai-storage-proxy-23.3.2/backend.ai_storage_proxy.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      310 2023-05-05 07:08:21.000000 backend.ai-storage-proxy-23.3.2/backend.ai_storage_proxy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        3 2023-05-05 07:08:21.000000 backend.ai-storage-proxy-23.3.2/backend.ai_storage_proxy.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      626 2023-05-05 07:08:20.000000 backend.ai-storage-proxy-23.3.2/backend_shim.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-05 07:08:21.426488 backend.ai-storage-proxy-23.3.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     8006 2023-05-05 07:08:20.000000 backend.ai-storage-proxy-23.3.2/setup.py
```

### Comparing `backend.ai-storage-proxy-23.3.1/PKG-INFO` & `backend.ai-storage-proxy-23.3.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: backend.ai-storage-proxy
-Version: 23.3.1
+Version: 23.3.2
 Summary: Backend.AI Storage Proxy
 Home-page: https://github.com/lablup/backend.ai
 Author: Lablup Inc. and contributors
 License: LGPLv3
 Project-URL: Documentation, https://docs.backend.ai/
 Project-URL: Source, https://github.com/lablup/backend.ai
 Classifier: Intended Audience :: Developers
```

### Comparing `backend.ai-storage-proxy-23.3.1/ai/backend/storage/abc.py` & `backend.ai-storage-proxy-23.3.2/ai/backend/storage/abc.py`

 * *Files identical despite different names*

### Comparing `backend.ai-storage-proxy-23.3.1/ai/backend/storage/api/client.py` & `backend.ai-storage-proxy-23.3.2/ai/backend/storage/api/client.py`

 * *Files identical despite different names*

### Comparing `backend.ai-storage-proxy-23.3.1/ai/backend/storage/api/manager.py` & `backend.ai-storage-proxy-23.3.2/ai/backend/storage/api/manager.py`

 * *Files identical despite different names*

### Comparing `backend.ai-storage-proxy-23.3.1/ai/backend/storage/cephfs/__init__.py` & `backend.ai-storage-proxy-23.3.2/ai/backend/storage/cephfs/__init__.py`

 * *Files identical despite different names*

### Comparing `backend.ai-storage-proxy-23.3.1/ai/backend/storage/config.py` & `backend.ai-storage-proxy-23.3.2/ai/backend/storage/config.py`

 * *Files identical despite different names*

### Comparing `backend.ai-storage-proxy-23.3.1/ai/backend/storage/context.py` & `backend.ai-storage-proxy-23.3.2/ai/backend/storage/context.py`

 * *Files identical despite different names*

### Comparing `backend.ai-storage-proxy-23.3.1/ai/backend/storage/exception.py` & `backend.ai-storage-proxy-23.3.2/ai/backend/storage/exception.py`

 * *Files identical despite different names*

### Comparing `backend.ai-storage-proxy-23.3.1/ai/backend/storage/gpfs/__init__.py` & `backend.ai-storage-proxy-23.3.2/ai/backend/storage/gpfs/__init__.py`

 * *Files identical despite different names*

### Comparing `backend.ai-storage-proxy-23.3.1/ai/backend/storage/gpfs/exceptions.py` & `backend.ai-storage-proxy-23.3.2/ai/backend/storage/gpfs/exceptions.py`

 * *Files identical despite different names*

### Comparing `backend.ai-storage-proxy-23.3.1/ai/backend/storage/gpfs/gpfs_client.py` & `backend.ai-storage-proxy-23.3.2/ai/backend/storage/gpfs/gpfs_client.py`

 * *Files identical despite different names*

### Comparing `backend.ai-storage-proxy-23.3.1/ai/backend/storage/gpfs/types.py` & `backend.ai-storage-proxy-23.3.2/ai/backend/storage/gpfs/types.py`

 * *Files identical despite different names*

### Comparing `backend.ai-storage-proxy-23.3.1/ai/backend/storage/netapp/__init__.py` & `backend.ai-storage-proxy-23.3.2/ai/backend/storage/netapp/__init__.py`

 * *Files identical despite different names*

### Comparing `backend.ai-storage-proxy-23.3.1/ai/backend/storage/netapp/netappclient.py` & `backend.ai-storage-proxy-23.3.2/ai/backend/storage/netapp/netappclient.py`

 * *Files identical despite different names*

### Comparing `backend.ai-storage-proxy-23.3.1/ai/backend/storage/netapp/quotamanager.py` & `backend.ai-storage-proxy-23.3.2/ai/backend/storage/netapp/quotamanager.py`

 * *Files identical despite different names*

### Comparing `backend.ai-storage-proxy-23.3.1/ai/backend/storage/purestorage/__init__.py` & `backend.ai-storage-proxy-23.3.2/ai/backend/storage/purestorage/__init__.py`

 * *Files identical despite different names*

### Comparing `backend.ai-storage-proxy-23.3.1/ai/backend/storage/purestorage/purity.py` & `backend.ai-storage-proxy-23.3.2/ai/backend/storage/purestorage/purity.py`

 * *Files identical despite different names*

### Comparing `backend.ai-storage-proxy-23.3.1/ai/backend/storage/server.py` & `backend.ai-storage-proxy-23.3.2/ai/backend/storage/server.py`

 * *Files identical despite different names*

### Comparing `backend.ai-storage-proxy-23.3.1/ai/backend/storage/types.py` & `backend.ai-storage-proxy-23.3.2/ai/backend/storage/types.py`

 * *Files identical despite different names*

### Comparing `backend.ai-storage-proxy-23.3.1/ai/backend/storage/utils.py` & `backend.ai-storage-proxy-23.3.2/ai/backend/storage/utils.py`

 * *Files identical despite different names*

### Comparing `backend.ai-storage-proxy-23.3.1/ai/backend/storage/vfs/__init__.py` & `backend.ai-storage-proxy-23.3.2/ai/backend/storage/vfs/__init__.py`

 * *Files identical despite different names*

### Comparing `backend.ai-storage-proxy-23.3.1/ai/backend/storage/weka/__init__.py` & `backend.ai-storage-proxy-23.3.2/ai/backend/storage/weka/__init__.py`

 * *Files identical despite different names*

### Comparing `backend.ai-storage-proxy-23.3.1/ai/backend/storage/weka/exceptions.py` & `backend.ai-storage-proxy-23.3.2/ai/backend/storage/weka/exceptions.py`

 * *Files identical despite different names*

### Comparing `backend.ai-storage-proxy-23.3.1/ai/backend/storage/weka/weka_client.py` & `backend.ai-storage-proxy-23.3.2/ai/backend/storage/weka/weka_client.py`

 * *Files identical despite different names*

### Comparing `backend.ai-storage-proxy-23.3.1/ai/backend/storage/xfs/__init__.py` & `backend.ai-storage-proxy-23.3.2/ai/backend/storage/xfs/__init__.py`

 * *Files identical despite different names*

### Comparing `backend.ai-storage-proxy-23.3.1/backend.ai_storage_proxy.egg-info/PKG-INFO` & `backend.ai-storage-proxy-23.3.2/backend.ai_storage_proxy.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: backend.ai-storage-proxy
-Version: 23.3.1
+Version: 23.3.2
 Summary: Backend.AI Storage Proxy
 Home-page: https://github.com/lablup/backend.ai
 Author: Lablup Inc. and contributors
 License: LGPLv3
 Project-URL: Documentation, https://docs.backend.ai/
 Project-URL: Source, https://github.com/lablup/backend.ai
 Classifier: Intended Audience :: Developers
```

### Comparing `backend.ai-storage-proxy-23.3.1/backend.ai_storage_proxy.egg-info/SOURCES.txt` & `backend.ai-storage-proxy-23.3.2/backend.ai_storage_proxy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `backend.ai-storage-proxy-23.3.1/backend_shim.py` & `backend.ai-storage-proxy-23.3.2/backend_shim.py`

 * *Files identical despite different names*

### Comparing `backend.ai-storage-proxy-23.3.1/setup.py` & `backend.ai-storage-proxy-23.3.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -23,24 +23,24 @@
         'PyJWT~=2.0',
         'aiofiles~=0.8.0',
         'aiohttp_cors~=0.7',
         'aiohttp~=3.8.1',
         'aiomonitor-ng~=0.7.2',
         'aiotools~=1.6.1',
         'attrs>=20.3',
-        """backend.ai-common==23.03.1
+        """backend.ai-common==23.03.2
 """,
         'click>=7.1.2',
         'dataclasses-json~=0.5.7',
         'janus~=1.0.0',
         'setproctitle~=1.2.2',
         'tenacity>=8.0',
         'trafaret~=2.1',
         'uvloop>=0.17; sys_platform != "Windows"',
-        'yarl>=1.7',
+        'yarl~=1.8.2',
         'zipstream-new~=1.1.8',
     ),
     'license': 'LGPLv3',
     'long_description': """# Backend.AI Storage Proxy
 
 Backend.AI Storage Proxy is an RPC daemon to manage vfolders used in Backend.AI agent, with quota and
 storage-specific optimization support.
@@ -243,11 +243,11 @@
     ),
     'project_urls': {
         'Documentation': 'https://docs.backend.ai/',
         'Source': 'https://github.com/lablup/backend.ai',
     },
     'python_requires': '>=3.11,<3.12',
     'url': 'https://github.com/lablup/backend.ai',
-    'version': """23.03.1
+    'version': """23.03.2
 """,
     'zip_safe': False,
 })
```

