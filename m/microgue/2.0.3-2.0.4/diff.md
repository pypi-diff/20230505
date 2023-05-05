# Comparing `tmp/microgue-2.0.3.tar.gz` & `tmp/microgue-2.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/microgue-2.0.3.tar", last modified: Tue May  2 14:25:30 2023, max compression
+gzip compressed data, was "dist/microgue-2.0.4.tar", last modified: Fri May  5 18:43:05 2023, max compression
```

## Comparing `microgue-2.0.3.tar` & `microgue-2.0.4.tar`

### file list

```diff
@@ -1,50 +1,50 @@
-drwxr-xr-x   0 mhudelso   (501) staff       (20)        0 2023-05-02 14:25:30.000000 microgue-2.0.3/
--rw-r--r--   0 mhudelso   (501) staff       (20)     3060 2023-05-02 14:25:30.000000 microgue-2.0.3/PKG-INFO
-drwxr-xr-x   0 mhudelso   (501) staff       (20)        0 2023-05-02 14:25:30.000000 microgue-2.0.3/microgue/
-drwxr-xr-x   0 mhudelso   (501) staff       (20)        0 2023-05-02 14:25:30.000000 microgue-2.0.3/microgue/storages/
--rw-r--r--   0 mhudelso   (501) staff       (20)        0 2021-01-25 18:39:15.000000 microgue-2.0.3/microgue/storages/__init__.py
--rw-r--r--   0 mhudelso   (501) staff       (20)     3348 2023-05-02 01:36:41.000000 microgue-2.0.3/microgue/storages/abstract_storage.py
-drwxr-xr-x   0 mhudelso   (501) staff       (20)        0 2023-05-02 14:25:30.000000 microgue-2.0.3/microgue/loggers/
--rw-r--r--   0 mhudelso   (501) staff       (20)        0 2021-01-25 18:39:15.000000 microgue-2.0.3/microgue/loggers/__init__.py
--rw-r--r--   0 mhudelso   (501) staff       (20)     1369 2023-05-01 20:10:53.000000 microgue-2.0.3/microgue/loggers/logger.py
-drwxr-xr-x   0 mhudelso   (501) staff       (20)        0 2023-05-02 14:25:30.000000 microgue-2.0.3/microgue/security/
--rw-r--r--   0 mhudelso   (501) staff       (20)      334 2023-04-30 02:18:57.000000 microgue-2.0.3/microgue/security/generic.py
--rw-r--r--   0 mhudelso   (501) staff       (20)        0 2021-01-25 18:39:15.000000 microgue-2.0.3/microgue/security/__init__.py
-drwxr-xr-x   0 mhudelso   (501) staff       (20)        0 2023-05-02 14:25:30.000000 microgue-2.0.3/microgue/secrets/
--rw-r--r--   0 mhudelso   (501) staff       (20)        0 2021-01-25 18:39:15.000000 microgue-2.0.3/microgue/secrets/__init__.py
--rw-r--r--   0 mhudelso   (501) staff       (20)     1014 2023-05-02 01:36:25.000000 microgue-2.0.3/microgue/secrets/secrets.py
-drwxr-xr-x   0 mhudelso   (501) staff       (20)        0 2023-05-02 14:25:30.000000 microgue-2.0.3/microgue/constants/
--rw-r--r--   0 mhudelso   (501) staff       (20)        0 2021-01-25 18:39:15.000000 microgue-2.0.3/microgue/constants/__init__.py
--rw-r--r--   0 mhudelso   (501) staff       (20)      378 2022-09-21 19:29:50.000000 microgue-2.0.3/microgue/constants/error_constants.py
--rw-r--r--   0 mhudelso   (501) staff       (20)        0 2021-01-25 18:39:15.000000 microgue-2.0.3/microgue/__init__.py
-drwxr-xr-x   0 mhudelso   (501) staff       (20)        0 2023-05-02 14:25:30.000000 microgue-2.0.3/microgue/objects/
--rw-r--r--   0 mhudelso   (501) staff       (20)     8817 2023-05-02 02:23:16.000000 microgue-2.0.3/microgue/objects/abstract_model_object.py
--rw-r--r--   0 mhudelso   (501) staff       (20)     2542 2023-05-02 02:23:16.000000 microgue-2.0.3/microgue/objects/object.py
--rw-r--r--   0 mhudelso   (501) staff       (20)        0 2021-01-25 18:39:15.000000 microgue-2.0.3/microgue/objects/__init__.py
--rw-r--r--   0 mhudelso   (501) staff       (20)     1483 2023-05-02 01:54:14.000000 microgue-2.0.3/microgue/objects/abstract_expiring_model_object.py
-drwxr-xr-x   0 mhudelso   (501) staff       (20)        0 2023-05-02 14:25:30.000000 microgue-2.0.3/microgue/models/
--rw-r--r--   0 mhudelso   (501) staff       (20)        0 2021-01-25 18:39:15.000000 microgue-2.0.3/microgue/models/__init__.py
--rw-r--r--   0 mhudelso   (501) staff       (20)    10589 2023-05-02 01:36:25.000000 microgue-2.0.3/microgue/models/abstract_model.py
--rw-r--r--   0 mhudelso   (501) staff       (20)     2737 2023-05-02 02:25:32.000000 microgue-2.0.3/microgue/utils.py
-drwxr-xr-x   0 mhudelso   (501) staff       (20)        0 2023-05-02 14:25:30.000000 microgue-2.0.3/microgue/queues/
--rw-r--r--   0 mhudelso   (501) staff       (20)     2887 2023-05-02 01:49:56.000000 microgue-2.0.3/microgue/queues/abstract_queue.py
--rw-r--r--   0 mhudelso   (501) staff       (20)        0 2021-01-25 18:39:15.000000 microgue-2.0.3/microgue/queues/__init__.py
-drwxr-xr-x   0 mhudelso   (501) staff       (20)        0 2023-05-02 14:25:30.000000 microgue-2.0.3/microgue/events/
--rw-r--r--   0 mhudelso   (501) staff       (20)        0 2021-03-09 20:40:18.000000 microgue-2.0.3/microgue/events/__init__.py
--rw-r--r--   0 mhudelso   (501) staff       (20)     1504 2023-05-02 02:23:16.000000 microgue-2.0.3/microgue/events/abstract_event_bus.py
--rw-r--r--   0 mhudelso   (501) staff       (20)     5220 2023-05-02 01:51:02.000000 microgue-2.0.3/microgue/abstract_app.py
-drwxr-xr-x   0 mhudelso   (501) staff       (20)        0 2023-05-02 14:25:30.000000 microgue-2.0.3/microgue/services/
--rw-r--r--   0 mhudelso   (501) staff       (20)     4041 2023-05-02 14:21:23.000000 microgue-2.0.3/microgue/services/service.py
--rw-r--r--   0 mhudelso   (501) staff       (20)        0 2021-01-25 18:39:15.000000 microgue-2.0.3/microgue/services/__init__.py
-drwxr-xr-x   0 mhudelso   (501) staff       (20)        0 2023-05-02 14:25:30.000000 microgue-2.0.3/microgue/caches/
--rw-r--r--   0 mhudelso   (501) staff       (20)     3039 2023-05-02 01:51:21.000000 microgue-2.0.3/microgue/caches/abstract_cache.py
--rw-r--r--   0 mhudelso   (501) staff       (20)        0 2021-01-25 18:39:15.000000 microgue-2.0.3/microgue/caches/__init__.py
--rw-r--r--   0 mhudelso   (501) staff       (20)     1907 2022-09-27 19:27:36.000000 microgue-2.0.3/README.md
--rw-r--r--   0 mhudelso   (501) staff       (20)      640 2023-05-02 14:25:03.000000 microgue-2.0.3/setup.py
--rw-r--r--   0 mhudelso   (501) staff       (20)       38 2023-05-02 14:25:30.000000 microgue-2.0.3/setup.cfg
-drwxr-xr-x   0 mhudelso   (501) staff       (20)        0 2023-05-02 14:25:30.000000 microgue-2.0.3/microgue.egg-info/
--rw-r--r--   0 mhudelso   (501) staff       (20)     3060 2023-05-02 14:25:30.000000 microgue-2.0.3/microgue.egg-info/PKG-INFO
--rw-r--r--   0 mhudelso   (501) staff       (20)     1010 2023-05-02 14:25:30.000000 microgue-2.0.3/microgue.egg-info/SOURCES.txt
--rw-r--r--   0 mhudelso   (501) staff       (20)       42 2023-05-02 14:25:30.000000 microgue-2.0.3/microgue.egg-info/requires.txt
--rw-r--r--   0 mhudelso   (501) staff       (20)        9 2023-05-02 14:25:30.000000 microgue-2.0.3/microgue.egg-info/top_level.txt
--rw-r--r--   0 mhudelso   (501) staff       (20)        1 2023-05-02 14:25:30.000000 microgue-2.0.3/microgue.egg-info/dependency_links.txt
+drwxr-xr-x   0 mhudelso   (501) staff       (20)        0 2023-05-05 18:43:05.000000 microgue-2.0.4/
+-rw-r--r--   0 mhudelso   (501) staff       (20)     3060 2023-05-05 18:43:05.000000 microgue-2.0.4/PKG-INFO
+drwxr-xr-x   0 mhudelso   (501) staff       (20)        0 2023-05-05 18:43:05.000000 microgue-2.0.4/microgue/
+drwxr-xr-x   0 mhudelso   (501) staff       (20)        0 2023-05-05 18:43:05.000000 microgue-2.0.4/microgue/storages/
+-rw-r--r--   0 mhudelso   (501) staff       (20)        0 2021-01-25 18:39:15.000000 microgue-2.0.4/microgue/storages/__init__.py
+-rw-r--r--   0 mhudelso   (501) staff       (20)     3789 2023-05-05 18:16:25.000000 microgue-2.0.4/microgue/storages/abstract_storage.py
+drwxr-xr-x   0 mhudelso   (501) staff       (20)        0 2023-05-05 18:43:05.000000 microgue-2.0.4/microgue/loggers/
+-rw-r--r--   0 mhudelso   (501) staff       (20)        0 2021-01-25 18:39:15.000000 microgue-2.0.4/microgue/loggers/__init__.py
+-rw-r--r--   0 mhudelso   (501) staff       (20)     1412 2023-05-05 17:01:37.000000 microgue-2.0.4/microgue/loggers/logger.py
+drwxr-xr-x   0 mhudelso   (501) staff       (20)        0 2023-05-05 18:43:05.000000 microgue-2.0.4/microgue/security/
+-rw-r--r--   0 mhudelso   (501) staff       (20)      334 2023-04-30 02:18:57.000000 microgue-2.0.4/microgue/security/generic.py
+-rw-r--r--   0 mhudelso   (501) staff       (20)        0 2021-01-25 18:39:15.000000 microgue-2.0.4/microgue/security/__init__.py
+drwxr-xr-x   0 mhudelso   (501) staff       (20)        0 2023-05-05 18:43:05.000000 microgue-2.0.4/microgue/secrets/
+-rw-r--r--   0 mhudelso   (501) staff       (20)        0 2021-01-25 18:39:15.000000 microgue-2.0.4/microgue/secrets/__init__.py
+-rw-r--r--   0 mhudelso   (501) staff       (20)     1065 2023-05-05 17:12:46.000000 microgue-2.0.4/microgue/secrets/secrets.py
+drwxr-xr-x   0 mhudelso   (501) staff       (20)        0 2023-05-05 18:43:05.000000 microgue-2.0.4/microgue/constants/
+-rw-r--r--   0 mhudelso   (501) staff       (20)        0 2021-01-25 18:39:15.000000 microgue-2.0.4/microgue/constants/__init__.py
+-rw-r--r--   0 mhudelso   (501) staff       (20)      378 2022-09-21 19:29:50.000000 microgue-2.0.4/microgue/constants/error_constants.py
+-rw-r--r--   0 mhudelso   (501) staff       (20)        0 2021-01-25 18:39:15.000000 microgue-2.0.4/microgue/__init__.py
+drwxr-xr-x   0 mhudelso   (501) staff       (20)        0 2023-05-05 18:43:05.000000 microgue-2.0.4/microgue/objects/
+-rw-r--r--   0 mhudelso   (501) staff       (20)     8817 2023-05-02 02:23:16.000000 microgue-2.0.4/microgue/objects/abstract_model_object.py
+-rw-r--r--   0 mhudelso   (501) staff       (20)     2707 2023-05-05 18:41:01.000000 microgue-2.0.4/microgue/objects/object.py
+-rw-r--r--   0 mhudelso   (501) staff       (20)        0 2021-01-25 18:39:15.000000 microgue-2.0.4/microgue/objects/__init__.py
+-rw-r--r--   0 mhudelso   (501) staff       (20)     1483 2023-05-02 01:54:14.000000 microgue-2.0.4/microgue/objects/abstract_expiring_model_object.py
+drwxr-xr-x   0 mhudelso   (501) staff       (20)        0 2023-05-05 18:43:05.000000 microgue-2.0.4/microgue/models/
+-rw-r--r--   0 mhudelso   (501) staff       (20)        0 2021-01-25 18:39:15.000000 microgue-2.0.4/microgue/models/__init__.py
+-rw-r--r--   0 mhudelso   (501) staff       (20)    10632 2023-05-05 18:33:37.000000 microgue-2.0.4/microgue/models/abstract_model.py
+-rw-r--r--   0 mhudelso   (501) staff       (20)     2737 2023-05-02 02:25:32.000000 microgue-2.0.4/microgue/utils.py
+drwxr-xr-x   0 mhudelso   (501) staff       (20)        0 2023-05-05 18:43:05.000000 microgue-2.0.4/microgue/queues/
+-rw-r--r--   0 mhudelso   (501) staff       (20)     3155 2023-05-05 18:16:25.000000 microgue-2.0.4/microgue/queues/abstract_queue.py
+-rw-r--r--   0 mhudelso   (501) staff       (20)        0 2021-01-25 18:39:15.000000 microgue-2.0.4/microgue/queues/__init__.py
+drwxr-xr-x   0 mhudelso   (501) staff       (20)        0 2023-05-05 18:43:05.000000 microgue-2.0.4/microgue/events/
+-rw-r--r--   0 mhudelso   (501) staff       (20)        0 2021-03-09 20:40:18.000000 microgue-2.0.4/microgue/events/__init__.py
+-rw-r--r--   0 mhudelso   (501) staff       (20)     1947 2023-05-05 18:16:25.000000 microgue-2.0.4/microgue/events/abstract_event_bus.py
+-rw-r--r--   0 mhudelso   (501) staff       (20)     5220 2023-05-02 01:51:02.000000 microgue-2.0.4/microgue/abstract_app.py
+drwxr-xr-x   0 mhudelso   (501) staff       (20)        0 2023-05-05 18:43:05.000000 microgue-2.0.4/microgue/services/
+-rw-r--r--   0 mhudelso   (501) staff       (20)     4053 2023-05-05 18:26:11.000000 microgue-2.0.4/microgue/services/service.py
+-rw-r--r--   0 mhudelso   (501) staff       (20)        0 2021-01-25 18:39:15.000000 microgue-2.0.4/microgue/services/__init__.py
+drwxr-xr-x   0 mhudelso   (501) staff       (20)        0 2023-05-05 18:43:05.000000 microgue-2.0.4/microgue/caches/
+-rw-r--r--   0 mhudelso   (501) staff       (20)     3189 2023-05-05 18:16:25.000000 microgue-2.0.4/microgue/caches/abstract_cache.py
+-rw-r--r--   0 mhudelso   (501) staff       (20)        0 2021-01-25 18:39:15.000000 microgue-2.0.4/microgue/caches/__init__.py
+-rw-r--r--   0 mhudelso   (501) staff       (20)     1907 2022-09-27 19:27:36.000000 microgue-2.0.4/README.md
+-rw-r--r--   0 mhudelso   (501) staff       (20)      640 2023-05-05 18:42:45.000000 microgue-2.0.4/setup.py
+-rw-r--r--   0 mhudelso   (501) staff       (20)       38 2023-05-05 18:43:05.000000 microgue-2.0.4/setup.cfg
+drwxr-xr-x   0 mhudelso   (501) staff       (20)        0 2023-05-05 18:43:05.000000 microgue-2.0.4/microgue.egg-info/
+-rw-r--r--   0 mhudelso   (501) staff       (20)     3060 2023-05-05 18:43:05.000000 microgue-2.0.4/microgue.egg-info/PKG-INFO
+-rw-r--r--   0 mhudelso   (501) staff       (20)     1010 2023-05-05 18:43:05.000000 microgue-2.0.4/microgue.egg-info/SOURCES.txt
+-rw-r--r--   0 mhudelso   (501) staff       (20)       42 2023-05-05 18:43:05.000000 microgue-2.0.4/microgue.egg-info/requires.txt
+-rw-r--r--   0 mhudelso   (501) staff       (20)        9 2023-05-05 18:43:05.000000 microgue-2.0.4/microgue.egg-info/top_level.txt
+-rw-r--r--   0 mhudelso   (501) staff       (20)        1 2023-05-05 18:43:05.000000 microgue-2.0.4/microgue.egg-info/dependency_links.txt
```

### Comparing `microgue-2.0.3/PKG-INFO` & `microgue-2.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: microgue
-Version: 2.0.3
+Version: 2.0.4
 Summary: This project contains bootstrap code to speed up the development of AWS based microservices
 Home-page: UNKNOWN
 Author: Michael Hudelson
 Author-email: michaelhudelson@gmail.com
 License: MIT
 Description: # AWS Microservice Bootstrap Code
```

### Comparing `microgue-2.0.3/microgue/storages/abstract_storage.py` & `microgue-2.0.4/microgue/storages/abstract_storage.py`

 * *Files 25% similar despite different names*

```diff
@@ -3,38 +3,48 @@
 import uuid
 from pathlib import Path
 from ..loggers.logger import Logger
 
 logger = Logger()
 
 
+class DeleteFailed(Exception): pass  # noqa
 class DownloadFailed(Exception): pass  # noqa
+class StorageConnectionFailed(Exception): pass  # noqa
 class UploadFailed(Exception): pass  # noqa
-class DeleteFailed(Exception): pass  # noqa
 
 
 class AbstractStorage:
+    # internal use only
+    storage = None
+
+    # extension required
+    bucket_name = None
+    bucket_public_url = None
+
     class File:
         def __init__(self, remote_path=None, local_path=None, url=None):
             self.remote_path = remote_path
             self.local_path = local_path
             self.url = url
 
-    storage = None
-    bucket_name = ""
-    bucket_public_url = ""
-
     def __init__(self, *args, **kwargs):
         logger.debug(f"{self.__class__.__name__}.__init__", priority=2)
         logger.debug(f"AbstractStorage.storage: {AbstractStorage.storage}")
-        if AbstractStorage.storage is None:
-            logger.debug("connecting to s3")
-            AbstractStorage.storage = boto3.client("s3")
-        else:
-            logger.debug("using existing connection to s3")
+        try:
+            if AbstractStorage.storage is None:
+                # share the storage connection at the application level
+                logger.debug("connecting to s3")
+                AbstractStorage.storage = boto3.client("s3")
+            else:
+                logger.debug("using existing connection to s3")
+        except Exception as e:
+            logger.error(f"{self.__class__.__name__}.__init__ - error", priority=3)
+            logger.error(f"{e.__class__.__name__}: {str(e)}")
+            raise StorageConnectionFailed(str(e))
 
     def upload(self, local_file_path, remote_file_path=None):
         if remote_file_path is None:
             remote_file_path = str(uuid.uuid4()) + "-" + local_file_path.split("/")[-1]
 
         logger.debug(f"{self.__class__.__name__}.upload", priority=2)
         logger.debug(f"local_file_path: {local_file_path}")
```

### Comparing `microgue-2.0.3/microgue/loggers/logger.py` & `microgue-2.0.4/microgue/loggers/logger.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 
 
 class Logger:
     __instance = None
     logger = None
 
     def __new__(cls, name=None, level=logging.DEBUG, *args, **kwargs):
+        # create the logger as a singleton
         if not cls.__instance:
             cls.__instance = super().__new__(cls)
             cls.__instance.logger = logging.getLogger(name)
             cls.__instance.logger.setLevel(level)
         return cls.__instance
 
     def debug(self, message, priority=None):
```

### Comparing `microgue-2.0.3/microgue/secrets/secrets.py` & `microgue-2.0.4/microgue/secrets/secrets.py`

 * *Files 22% similar despite different names*

```diff
@@ -6,18 +6,19 @@
 
 
 class GetSecretFailed(Exception): pass  # noqa
 class SecretsConnectionFailed(Exception): pass  # noqa
 
 
 class Secrets:
-    secrets = None
     __instance = None
+    secrets = None
 
     def __new__(cls, *args, **kwargs):
+        # create the secret manager as a singleton
         if not cls.__instance:
             cls.__instance = super().__new__(cls)
             try:
                 cls.__instance.secrets = boto3.client("secretsmanager")
             except Exception as e:
                 raise SecretsConnectionFailed(str(e))
         return cls.__instance
```

### Comparing `microgue-2.0.3/microgue/objects/abstract_model_object.py` & `microgue-2.0.4/microgue/objects/abstract_model_object.py`

 * *Files identical despite different names*

### Comparing `microgue-2.0.3/microgue/objects/object.py` & `microgue-2.0.4/microgue/objects/object.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-class Null:
-    """
-    Null: attribute value is None
-    None: attribute value is not set
-    """
-    pass
-
-
 class Object:
+    class Null:
+        """
+        used internally by Object to distinguish between an attribute being not set vs set to None
+
+        Null: attribute value is None
+        None: attribute value is not set
+        """
+        pass
     """
     attributes: defines the attributes of the Object
 
     hidden_attributes: attributes that should not be included when calling Object.serialize()
-        Unless passing in hide_attributes=False
+        Unless passing hide_attributes=False in to Object.serialize()
     """
     attributes = []
     hidden_attributes = []
 
     def __init__(self, attributes=None, raise_errors=True, *args, **kwargs):
         # defaults
         attributes = {} if attributes is None else attributes
@@ -30,35 +30,35 @@
             raise_errors=raise_errors
         )
 
         super().__init__(*args, **kwargs)
 
     def __getattribute__(self, key):
         value = super().__getattribute__(key)
-        if value is Null:
+        if value is Object.Null:
             return None
         else:
             return value
 
     def __setattr__(self, key, value):
         if key not in self.attributes:
             raise AttributeError(f"{self.__class__.__name__} object does not have {key} attribute to set")
         if value is None:
-            self.__dict__[key] = Null
+            self.__dict__[key] = Object.Null
         else:
             self.__dict__[key] = value
 
     def copy(self):
         return self.__class__(self.serialize(hide_attributes=False))
 
     def serialize(self, hide_attributes=True):
         attributes = dict()
         for key, value in self.__dict__.items():
             if value is not None:
-                if value is Null:
+                if value is Object.Null:
                     attributes[key] = None
                 else:
                     attributes[key] = value
         if hide_attributes:
             for key in self.hidden_attributes:
                 attributes.pop(key, None)
```

### Comparing `microgue-2.0.3/microgue/objects/abstract_expiring_model_object.py` & `microgue-2.0.4/microgue/objects/abstract_expiring_model_object.py`

 * *Files identical despite different names*

### Comparing `microgue-2.0.3/microgue/models/abstract_model.py` & `microgue-2.0.4/microgue/models/abstract_model.py`

 * *Files 2% similar despite different names*

```diff
@@ -15,34 +15,34 @@
 class ItemAlreadyExists(Exception): pass  # noqa
 class MissingKey(Exception): pass  # noqa
 class UpdateFailed(Exception): pass  # noqa
 
 
 class AbstractModel:
     """
-    database: the connection to dynamodb
-    table_name: name of table in dynamodb
+    database: the connection to dynamodb - internal use only
+    table_name: name of table in dynamodb - extension required
     pk: partion key of the table - defaulted to id
     auto_generate_pk: auto generate the pk value using uuid
     sk: sort key for the partition key of the table - defaulted to None
     auto_generate_sk: auto generate the pk value using uuid
     indexes: defines all indexes on your table
-        local secondary indexes (lsi) do no require the pk to be defined
+        local secondary indexes (lsi) do not require the pk to be defined
         global secondary indexes (gsi) do not require the sk to be defined
         {
             "example_index-index": {
                 "pk": "example_index_partition_key",
                 "sk": "example_index_sort_key"
             }
         }
-    mask_attributes: list of attributes to maske when logging
+    mask_attributes: list of attributes to mask when logging
     """
     database = None
 
-    table_name = ""
+    table_name = None
 
     pk = "id"
     auto_generate_pk = True
 
     sk = None
     auto_generate_sk = True
```

### Comparing `microgue-2.0.3/microgue/utils.py` & `microgue-2.0.4/microgue/utils.py`

 * *Files identical despite different names*

### Comparing `microgue-2.0.3/microgue/queues/abstract_queue.py` & `microgue-2.0.4/microgue/queues/abstract_queue.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,32 +1,38 @@
 import boto3
 import json
 from ..loggers.logger import Logger
 
 logger = Logger()
 
 
-class QueueConnectionFailed(Exception): pass  # noqa
 class DeleteFailed(Exception): pass  # noqa
+class QueueConnectionFailed(Exception): pass  # noqa
 
 
 class AbstractQueue:
+    # internal use only
     queue = None
-    queue_url = ""
+
+    # extension required
+    queue_url = None
 
     def __init__(self, *args, **kwargs):
         logger.debug(f"{self.__class__.__name__}.__init__", priority=2)
         logger.debug(f"AbstractQueue.queue: {AbstractQueue.queue}")
         try:
             if AbstractQueue.queue is None:
+                # share the queue connection at the application level
                 logger.debug("connecting to sqs")
                 AbstractQueue.queue = boto3.client("sqs")
             else:
                 logger.debug("using existing connection to sqs")
         except Exception as e:
+            logger.error(f"{self.__class__.__name__}.__init__ - error", priority=3)
+            logger.error(f"{e.__class__.__name__}: {str(e)}")
             raise QueueConnectionFailed(str(e))
 
     def send(self, message):
         logger.debug(f"{self.__class__.__name__}.send", priority=2)
         if type(message) is dict:
             message = json.dumps(message)
         try:
```

### Comparing `microgue-2.0.3/microgue/events/abstract_event_bus.py` & `microgue-2.0.4/microgue/events/abstract_event_bus.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,28 +1,40 @@
 import boto3
 import json
 from ..loggers.logger import Logger
 
 logger = Logger()
 
 
+class EventBusConnectionFailed(Exception): pass  # noqa
+
+
 class AbstractEventBus:
+    # internal use only
     event_bus = None
+
+    # extension required
     event_bus_name = None
     event_bus_region = None
     event_source = None
 
     def __init__(self, *args, **kwargs):
         logger.debug(f"{self.__class__.__name__}.__init__", priority=2)
         logger.debug(f"AbstractEventBus.event_bus: {AbstractEventBus.event_bus}")
-        if AbstractEventBus.event_bus is None:
-            logger.debug("connecting to eventbridge")
-            AbstractEventBus.event_bus = boto3.client(service_name="events", region_name=self.event_bus_region)
-        else:
-            logger.debug("using existing connection to eventbridge")
+        try:
+            if AbstractEventBus.event_bus is None:
+                # share the event bus connection at the application level
+                logger.debug("connecting to eventbridge")
+                AbstractEventBus.event_bus = boto3.client(service_name="events", region_name=self.event_bus_region)
+            else:
+                logger.debug("using existing connection to eventbridge")
+        except Exception as e:
+            logger.error(f"{self.__class__.__name__}.__init__ - error", priority=3)
+            logger.error(f"{e.__class__.__name__}: {str(e)}")
+            raise EventBusConnectionFailed(str(e))
 
     def publish(self, event_type, event_data=None):
         # defaults
         event_data = {} if event_data is None else event_data
 
         logger.debug(f"{self.__class__.__name__}.publish", priority=2)
         logger.debug(f"event_type: {event_type}")
```

### Comparing `microgue-2.0.3/microgue/abstract_app.py` & `microgue-2.0.4/microgue/abstract_app.py`

 * *Files identical despite different names*

### Comparing `microgue-2.0.3/microgue/services/service.py` & `microgue-2.0.4/microgue/services/service.py`

 * *Files 3% similar despite different names*

```diff
@@ -5,14 +5,19 @@
 from ..utils import mask_fields_in_data
 from ..loggers.logger import Logger
 
 logger = Logger()
 
 
 class Service:
+    # extension optional
+    request_base_url = ""
+    mask_request_headers_fields = []
+    mask_request_data_fields = []
+
     class Request:
         def __init__(
             self,
             url="",
             parameters=None,
             method="GET",
             headers=None,
@@ -44,17 +49,15 @@
             self.headers = {} if headers is None else headers
             self.cookies = {} if cookies is None else cookies
             self.data = {} if data is None else data
 
             self.status_code = status_code
 
     def __init__(self, *args, **kwargs):
-        self.request_base_url = ""
-        self.mask_request_headers_fields = []
-        self.mask_request_data_fields = []
+        pass
 
     def request(self, *args, **kwargs):
         return self.invoke(Service.Request(*args, **kwargs))
 
     def invoke(self, request):
         logger.debug(f"{self.__class__.__name__}.invoke", priority=2)
         logger.debug(f"request url: {request.url}")
```

### Comparing `microgue-2.0.3/microgue/caches/abstract_cache.py` & `microgue-2.0.4/microgue/caches/abstract_cache.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,27 +6,33 @@
 logger = Logger()
 
 
 class CacheConnectionFailed(Exception): pass  # noqa
 
 
 class AbstractCache:
+    # internal use only
     cache = None
-    host = ""
-    port = ""
-    prefix = ""
+
+    # extension required
+    host = None
+    port = None
+
+    # extension optional
+    prefix = None
     ttl = 900
     connection_timeout = 1
     connection_required = True
 
     def __init__(self, *args, **kwargs):
         logger.debug(f"{self.__class__.__name__}.__init__", priority=2)
         logger.debug(f"self.__class__.cache: {self.__class__.cache}")
         try:
             if self.__class__.cache is None:
+                # share the cache connection at the __class__ level
                 logger.debug("connecting to redis")
                 self.__class__.cache = redis.StrictRedis(host=self.host, port=self.port, socket_connect_timeout=self.connection_timeout)
                 self.__class__.cache.ping()
             else:
                 logger.debug("using existing connection to redis")
         except Exception as e:
             logger.error(f"{self.__class__.__name__}.__init__ - error", priority=3)
```

### Comparing `microgue-2.0.3/README.md` & `microgue-2.0.4/README.md`

 * *Files identical despite different names*

### Comparing `microgue-2.0.3/setup.py` & `microgue-2.0.4/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md") as f:
     long_description = f.read()
 
 setup(
     name="microgue",
-    version="2.0.3",
+    version="2.0.4",
     author="Michael Hudelson",
     author_email="michaelhudelson@gmail.com",
     description="This project contains bootstrap code to speed up the development of AWS based microservices",
     long_description=long_description,
     long_description_content_type="text/markdown",
     license="MIT",
     packages=find_packages(),
```

### Comparing `microgue-2.0.3/microgue.egg-info/PKG-INFO` & `microgue-2.0.4/microgue.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: microgue
-Version: 2.0.3
+Version: 2.0.4
 Summary: This project contains bootstrap code to speed up the development of AWS based microservices
 Home-page: UNKNOWN
 Author: Michael Hudelson
 Author-email: michaelhudelson@gmail.com
 License: MIT
 Description: # AWS Microservice Bootstrap Code
```

### Comparing `microgue-2.0.3/microgue.egg-info/SOURCES.txt` & `microgue-2.0.4/microgue.egg-info/SOURCES.txt`

 * *Files identical despite different names*

