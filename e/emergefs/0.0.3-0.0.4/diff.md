# Comparing `tmp/emergefs-0.0.3.tar.gz` & `tmp/emergefs-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "emergefs-0.0.3.tar", last modified: Mon Mar 20 13:30:00 2023, max compression
+gzip compressed data, was "emergefs-0.0.4.tar", last modified: Fri May  5 19:12:33 2023, max compression
```

## Comparing `emergefs-0.0.3.tar` & `emergefs-0.0.4.tar`

### file list

```diff
@@ -1,46 +1,46 @@
-drwxrwxr-x   0 darren    (1000) darren    (1000)        0 2023-03-20 13:30:00.844547 emergefs-0.0.3/
--rw-rw-r--   0 darren    (1000) darren    (1000)     1070 2022-08-25 15:31:03.000000 emergefs-0.0.3/LICENSE
--rw-rw-r--   0 darren    (1000) darren    (1000)    18175 2023-03-20 13:30:00.844547 emergefs-0.0.3/PKG-INFO
--rw-rw-r--   0 darren    (1000) darren    (1000)    17675 2023-03-19 14:12:01.000000 emergefs-0.0.3/README.md
-drwxrwxr-x   0 darren    (1000) darren    (1000)        0 2023-03-20 13:30:00.840547 emergefs-0.0.3/emerge/
--rw-rw-r--   0 darren    (1000) darren    (1000)      136 2023-03-18 21:05:54.000000 emergefs-0.0.3/emerge/__init__.py
--rw-rw-r--   0 darren    (1000) darren    (1000)      341 2023-03-20 13:29:11.000000 emergefs-0.0.3/emerge/__version__.py
-drwxrwxr-x   0 darren    (1000) darren    (1000)        0 2023-03-20 13:30:00.840547 emergefs-0.0.3/emerge/cli/
--rw-rw-r--   0 darren    (1000) darren    (1000)     8954 2023-03-17 19:00:51.000000 emergefs-0.0.3/emerge/cli/__init__.py
-drwxrwxr-x   0 darren    (1000) darren    (1000)        0 2023-03-20 13:30:00.840547 emergefs-0.0.3/emerge/compute/
--rw-rw-r--   0 darren    (1000) darren    (1000)      201 2022-08-28 17:01:25.000000 emergefs-0.0.3/emerge/compute/__init__.py
-drwxrwxr-x   0 darren    (1000) darren    (1000)        0 2023-03-20 13:30:00.840547 emergefs-0.0.3/emerge/core/
--rw-rw-r--   0 darren    (1000) darren    (1000)        0 2022-08-26 18:03:05.000000 emergefs-0.0.3/emerge/core/__init__.py
--rw-rw-r--   0 darren    (1000) darren    (1000)     3350 2023-03-17 18:38:29.000000 emergefs-0.0.3/emerge/core/client.py
--rw-rw-r--   0 darren    (1000) darren    (1000)     2095 2023-03-17 13:45:15.000000 emergefs-0.0.3/emerge/core/objects.py
-drwxrwxr-x   0 darren    (1000) darren    (1000)        0 2023-03-20 13:30:00.840547 emergefs-0.0.3/emerge/data/
--rw-rw-r--   0 darren    (1000) darren    (1000)      617 2023-01-13 17:22:25.000000 emergefs-0.0.3/emerge/data/__init__.py
-drwxrwxr-x   0 darren    (1000) darren    (1000)        0 2023-03-20 13:30:00.840547 emergefs-0.0.3/emerge/file/
--rw-rw-r--   0 darren    (1000) darren    (1000)        0 2022-08-25 15:32:44.000000 emergefs-0.0.3/emerge/file/__init__.py
-drwxrwxr-x   0 darren    (1000) darren    (1000)        0 2023-03-20 13:30:00.840547 emergefs-0.0.3/emerge/fs/
--rw-rw-r--   0 darren    (1000) darren    (1000)        0 2022-08-25 15:32:27.000000 emergefs-0.0.3/emerge/fs/__init__.py
--rw-rw-r--   0 darren    (1000) darren    (1000)     2604 2023-01-11 06:35:23.000000 emergefs-0.0.3/emerge/fs/filesystem.py
-drwxrwxr-x   0 darren    (1000) darren    (1000)        0 2023-03-20 13:30:00.840547 emergefs-0.0.3/emerge/node/
--rw-rw-r--   0 darren    (1000) darren    (1000)        0 2022-08-25 15:42:49.000000 emergefs-0.0.3/emerge/node/__init__.py
--rw-rw-r--   0 darren    (1000) darren    (1000)      648 2022-08-26 22:59:34.000000 emergefs-0.0.3/emerge/node/handlers.py
--rw-rw-r--   0 darren    (1000) darren    (1000)    41072 2023-03-19 14:14:08.000000 emergefs-0.0.3/emerge/node/server.py
-drwxrwxr-x   0 darren    (1000) darren    (1000)        0 2023-03-20 13:30:00.844547 emergefs-0.0.3/emerge/tests/
--rw-rw-r--   0 darren    (1000) darren    (1000)        0 2022-08-25 15:55:09.000000 emergefs-0.0.3/emerge/tests/__init__.py
--rw-rw-r--   0 darren    (1000) darren    (1000)      139 2023-01-07 16:44:46.000000 emergefs-0.0.3/emerge/tests/test_client.py
-drwxrwxr-x   0 darren    (1000) darren    (1000)        0 2023-03-20 13:30:00.844547 emergefs-0.0.3/emerge/zmq/
--rw-rw-r--   0 darren    (1000) darren    (1000)        0 2022-08-26 13:15:50.000000 emergefs-0.0.3/emerge/zmq/__init__.py
--rw-rw-r--   0 darren    (1000) darren    (1000)      411 2022-08-26 14:10:31.000000 emergefs-0.0.3/emerge/zmq/connection.py
--rw-rw-r--   0 darren    (1000) darren    (1000)     2052 2022-08-26 14:11:59.000000 emergefs-0.0.3/emerge/zmq/message.py
--rw-rw-r--   0 darren    (1000) darren    (1000)      700 2022-08-26 14:11:35.000000 emergefs-0.0.3/emerge/zmq/publisher.py
--rw-rw-r--   0 darren    (1000) darren    (1000)      114 2022-08-26 13:19:16.000000 emergefs-0.0.3/emerge/zmq/settings.py
--rw-rw-r--   0 darren    (1000) darren    (1000)     1910 2022-08-26 14:11:55.000000 emergefs-0.0.3/emerge/zmq/subscriber.py
-drwxrwxr-x   0 darren    (1000) darren    (1000)        0 2023-03-20 13:30:00.844547 emergefs-0.0.3/emergefs.egg-info/
--rw-rw-r--   0 darren    (1000) darren    (1000)    18175 2023-03-20 13:30:00.000000 emergefs-0.0.3/emergefs.egg-info/PKG-INFO
--rw-rw-r--   0 darren    (1000) darren    (1000)      770 2023-03-20 13:30:00.000000 emergefs-0.0.3/emergefs.egg-info/SOURCES.txt
--rw-rw-r--   0 darren    (1000) darren    (1000)        1 2023-03-20 13:30:00.000000 emergefs-0.0.3/emergefs.egg-info/dependency_links.txt
--rw-rw-r--   0 darren    (1000) darren    (1000)       43 2023-03-20 13:30:00.000000 emergefs-0.0.3/emergefs.egg-info/entry_points.txt
--rw-rw-r--   0 darren    (1000) darren    (1000)        1 2023-03-20 13:30:00.000000 emergefs-0.0.3/emergefs.egg-info/not-zip-safe
--rw-rw-r--   0 darren    (1000) darren    (1000)       40 2023-03-20 13:30:00.000000 emergefs-0.0.3/emergefs.egg-info/requires.txt
--rw-rw-r--   0 darren    (1000) darren    (1000)        7 2023-03-20 13:30:00.000000 emergefs-0.0.3/emergefs.egg-info/top_level.txt
--rw-rw-r--   0 darren    (1000) darren    (1000)       38 2023-03-20 13:30:00.844547 emergefs-0.0.3/setup.cfg
--rw-rw-r--   0 darren    (1000) darren    (1000)     4640 2023-03-20 13:29:11.000000 emergefs-0.0.3/setup.py
+drwxrwxr-x   0 darren    (1000) darren    (1000)        0 2023-05-05 19:12:33.262410 emergefs-0.0.4/
+-rw-rw-r--   0 darren    (1000) darren    (1000)     1070 2022-08-25 15:31:03.000000 emergefs-0.0.4/LICENSE
+-rw-rw-r--   0 darren    (1000) darren    (1000)    18173 2023-05-05 19:12:33.262410 emergefs-0.0.4/PKG-INFO
+-rw-rw-r--   0 darren    (1000) darren    (1000)    17675 2023-03-19 14:12:01.000000 emergefs-0.0.4/README.md
+drwxrwxr-x   0 darren    (1000) darren    (1000)        0 2023-05-05 19:12:33.258410 emergefs-0.0.4/emerge/
+-rw-rw-r--   0 darren    (1000) darren    (1000)      151 2023-05-04 13:31:13.000000 emergefs-0.0.4/emerge/__init__.py
+-rw-rw-r--   0 darren    (1000) darren    (1000)      341 2023-05-05 19:10:30.000000 emergefs-0.0.4/emerge/__version__.py
+drwxrwxr-x   0 darren    (1000) darren    (1000)        0 2023-05-05 19:12:33.258410 emergefs-0.0.4/emerge/cli/
+-rw-rw-r--   0 darren    (1000) darren    (1000)     8969 2023-05-04 13:30:42.000000 emergefs-0.0.4/emerge/cli/__init__.py
+drwxrwxr-x   0 darren    (1000) darren    (1000)        0 2023-05-05 19:12:33.258410 emergefs-0.0.4/emerge/compute/
+-rw-rw-r--   0 darren    (1000) darren    (1000)      201 2022-08-28 17:01:25.000000 emergefs-0.0.4/emerge/compute/__init__.py
+drwxrwxr-x   0 darren    (1000) darren    (1000)        0 2023-05-05 19:12:33.258410 emergefs-0.0.4/emerge/core/
+-rw-rw-r--   0 darren    (1000) darren    (1000)        0 2022-08-26 18:03:05.000000 emergefs-0.0.4/emerge/core/__init__.py
+-rw-rw-r--   0 darren    (1000) darren    (1000)     3698 2023-05-04 13:32:17.000000 emergefs-0.0.4/emerge/core/client.py
+-rw-rw-r--   0 darren    (1000) darren    (1000)     2095 2023-03-17 13:45:15.000000 emergefs-0.0.4/emerge/core/objects.py
+drwxrwxr-x   0 darren    (1000) darren    (1000)        0 2023-05-05 19:12:33.258410 emergefs-0.0.4/emerge/data/
+-rw-rw-r--   0 darren    (1000) darren    (1000)      617 2023-01-13 17:22:25.000000 emergefs-0.0.4/emerge/data/__init__.py
+drwxrwxr-x   0 darren    (1000) darren    (1000)        0 2023-05-05 19:12:33.258410 emergefs-0.0.4/emerge/file/
+-rw-rw-r--   0 darren    (1000) darren    (1000)        0 2022-08-25 15:32:44.000000 emergefs-0.0.4/emerge/file/__init__.py
+drwxrwxr-x   0 darren    (1000) darren    (1000)        0 2023-05-05 19:12:33.258410 emergefs-0.0.4/emerge/fs/
+-rw-rw-r--   0 darren    (1000) darren    (1000)        0 2022-08-25 15:32:27.000000 emergefs-0.0.4/emerge/fs/__init__.py
+-rw-rw-r--   0 darren    (1000) darren    (1000)     2604 2023-01-11 06:35:23.000000 emergefs-0.0.4/emerge/fs/filesystem.py
+drwxrwxr-x   0 darren    (1000) darren    (1000)        0 2023-05-05 19:12:33.262410 emergefs-0.0.4/emerge/node/
+-rw-rw-r--   0 darren    (1000) darren    (1000)        0 2022-08-25 15:42:49.000000 emergefs-0.0.4/emerge/node/__init__.py
+-rw-rw-r--   0 darren    (1000) darren    (1000)      648 2022-08-26 22:59:34.000000 emergefs-0.0.4/emerge/node/handlers.py
+-rw-rw-r--   0 darren    (1000) darren    (1000)    41062 2023-05-04 16:54:23.000000 emergefs-0.0.4/emerge/node/server.py
+drwxrwxr-x   0 darren    (1000) darren    (1000)        0 2023-05-05 19:12:33.262410 emergefs-0.0.4/emerge/tests/
+-rw-rw-r--   0 darren    (1000) darren    (1000)        0 2022-08-25 15:55:09.000000 emergefs-0.0.4/emerge/tests/__init__.py
+-rw-rw-r--   0 darren    (1000) darren    (1000)      139 2023-01-07 16:44:46.000000 emergefs-0.0.4/emerge/tests/test_client.py
+drwxrwxr-x   0 darren    (1000) darren    (1000)        0 2023-05-05 19:12:33.262410 emergefs-0.0.4/emerge/zmq/
+-rw-rw-r--   0 darren    (1000) darren    (1000)        0 2022-08-26 13:15:50.000000 emergefs-0.0.4/emerge/zmq/__init__.py
+-rw-rw-r--   0 darren    (1000) darren    (1000)      411 2022-08-26 14:10:31.000000 emergefs-0.0.4/emerge/zmq/connection.py
+-rw-rw-r--   0 darren    (1000) darren    (1000)     2052 2022-08-26 14:11:59.000000 emergefs-0.0.4/emerge/zmq/message.py
+-rw-rw-r--   0 darren    (1000) darren    (1000)      700 2022-08-26 14:11:35.000000 emergefs-0.0.4/emerge/zmq/publisher.py
+-rw-rw-r--   0 darren    (1000) darren    (1000)      114 2022-08-26 13:19:16.000000 emergefs-0.0.4/emerge/zmq/settings.py
+-rw-rw-r--   0 darren    (1000) darren    (1000)     1910 2022-08-26 14:11:55.000000 emergefs-0.0.4/emerge/zmq/subscriber.py
+drwxrwxr-x   0 darren    (1000) darren    (1000)        0 2023-05-05 19:12:33.262410 emergefs-0.0.4/emergefs.egg-info/
+-rw-rw-r--   0 darren    (1000) darren    (1000)    18173 2023-05-05 19:12:33.000000 emergefs-0.0.4/emergefs.egg-info/PKG-INFO
+-rw-rw-r--   0 darren    (1000) darren    (1000)      770 2023-05-05 19:12:33.000000 emergefs-0.0.4/emergefs.egg-info/SOURCES.txt
+-rw-rw-r--   0 darren    (1000) darren    (1000)        1 2023-05-05 19:12:33.000000 emergefs-0.0.4/emergefs.egg-info/dependency_links.txt
+-rw-rw-r--   0 darren    (1000) darren    (1000)       43 2023-05-05 19:12:33.000000 emergefs-0.0.4/emergefs.egg-info/entry_points.txt
+-rw-rw-r--   0 darren    (1000) darren    (1000)        1 2023-05-05 19:12:33.000000 emergefs-0.0.4/emergefs.egg-info/not-zip-safe
+-rw-rw-r--   0 darren    (1000) darren    (1000)       40 2023-05-05 19:12:33.000000 emergefs-0.0.4/emergefs.egg-info/requires.txt
+-rw-rw-r--   0 darren    (1000) darren    (1000)        7 2023-05-05 19:12:33.000000 emergefs-0.0.4/emergefs.egg-info/top_level.txt
+-rw-rw-r--   0 darren    (1000) darren    (1000)       38 2023-05-05 19:12:33.262410 emergefs-0.0.4/setup.cfg
+-rw-rw-r--   0 darren    (1000) darren    (1000)     4638 2023-05-05 19:12:05.000000 emergefs-0.0.4/setup.py
```

### Comparing `emergefs-0.0.3/LICENSE` & `emergefs-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `emergefs-0.0.3/PKG-INFO` & `emergefs-0.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: emergefs
-Version: 0.0.3
+Version: 0.0.4
 Summary: Emerge Computational Filesystem.
 Home-page: https://github.com/radiantone/emerge
 Author: Darren Govoni
 Author-email: darren@elasticcode.ai
 License: MIT License
 Keywords: cli,tools,utility
 Platform: UNKNOWN
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3.10
-Requires-Python: >=3.8.*
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 <img src="./images/logo.png" width="200">
 
 *Serverless, object-oriented, computational file system for python*
```

### Comparing `emergefs-0.0.3/README.md` & `emergefs-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `emergefs-0.0.3/emerge/cli/__init__.py` & `emergefs-0.0.4/emerge/cli/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -42,15 +42,15 @@
         )
     else:
         logging.basicConfig(
             format="%(asctime)s : %(name)s %(levelname)s : %(message)s",
             level=logging.INFO,
         )
 
-    from emerge.core.client import Client
+    from emerge.core.client import Z0RPCClient as Client
 
     """ Connect to specific Node """
 
     context.obj = {}
 
     if host is not None:
         splits = host.split(":")
```

### Comparing `emergefs-0.0.3/emerge/core/client.py` & `emergefs-0.0.4/emerge/core/client.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,27 +1,42 @@
 import logging
 from functools import partial
 
 import dill
 import zerorpc
 import zope
 
+ZERORPC_CLIENT = zerorpc.Client
+HTTP_CLIENT = ""
+
 
 class IClient(zope.interface.Interface):
     def search(self, where):
         raise NotImplementedError()
 
     def proxy(self, path):
         raise NotImplementedError()
 
+    def index(self):
+        raise NotImplementedError()
+
+    def searchtext(self, field, query):
+        raise NotImplementedError()
+
+
+@zope.interface.implementer(IClient)
+class RESTClient:
+    pass
+
 
 @zope.interface.implementer(IClient)
-class Client:
+class Z0RPCClient:
     def __init__(self, host, port):
-        self.client = zerorpc.Client()
+        # TODO: This is where the client implemenation should change
+        self.client = ZERORPC_CLIENT()
         self.client.connect("tcp://{}:{}".format(host, port))
 
     def searchtext(self, field, query):
         return self.client.searchtext(field, query)
 
     def index(self):
         return self.client.index()
@@ -121,7 +136,10 @@
                 file["obj"] = dill.loads(file["obj"])
             _files = file
 
         return _files
 
     def run(self, oid, method):
         return self.client.execute(oid, method)
+
+
+Client = Z0RPCClient
```

### Comparing `emergefs-0.0.3/emerge/core/objects.py` & `emergefs-0.0.4/emerge/core/objects.py`

 * *Files identical despite different names*

### Comparing `emergefs-0.0.3/emerge/data/__init__.py` & `emergefs-0.0.4/emerge/data/__init__.py`

 * *Files identical despite different names*

### Comparing `emergefs-0.0.3/emerge/fs/filesystem.py` & `emergefs-0.0.4/emerge/fs/filesystem.py`

 * *Files identical despite different names*

### Comparing `emergefs-0.0.3/emerge/node/handlers.py` & `emergefs-0.0.4/emerge/node/handlers.py`

 * *Files identical despite different names*

### Comparing `emergefs-0.0.3/emerge/node/server.py` & `emergefs-0.0.4/emerge/node/server.py`

 * *Files 0% similar despite different names*

```diff
@@ -745,15 +745,15 @@
                 # If not a dict then must be dilled
                 _obj = dill.loads(obj)
                 _obj.node = platform.node()
 
             connection = self.fs.db.open(tx_mgr)
 
             try:
-                with tx_mgr as tx_mgr:
+                with tx_mgr:
                     fsroot = connection.root()
 
                     # Make graphql schema for object
                     logging.info("_OBJ %s %s", type(_obj), obj)
                     _fields, self.schema = self._make_graphql(_obj)
 
                     # Store the updated schema
```

### Comparing `emergefs-0.0.3/emerge/zmq/message.py` & `emergefs-0.0.4/emerge/zmq/message.py`

 * *Files identical despite different names*

### Comparing `emergefs-0.0.3/emerge/zmq/publisher.py` & `emergefs-0.0.4/emerge/zmq/publisher.py`

 * *Files identical despite different names*

### Comparing `emergefs-0.0.3/emerge/zmq/subscriber.py` & `emergefs-0.0.4/emerge/zmq/subscriber.py`

 * *Files identical despite different names*

### Comparing `emergefs-0.0.3/emergefs.egg-info/PKG-INFO` & `emergefs-0.0.4/emergefs.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: emergefs
-Version: 0.0.3
+Version: 0.0.4
 Summary: Emerge Computational Filesystem.
 Home-page: https://github.com/radiantone/emerge
 Author: Darren Govoni
 Author-email: darren@elasticcode.ai
 License: MIT License
 Keywords: cli,tools,utility
 Platform: UNKNOWN
 Classifier: Development Status :: 2 - Pre-Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3.10
-Requires-Python: >=3.8.*
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 <img src="./images/logo.png" width="200">
 
 *Serverless, object-oriented, computational file system for python*
```

### Comparing `emergefs-0.0.3/emergefs.egg-info/SOURCES.txt` & `emergefs-0.0.4/emergefs.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `emergefs-0.0.3/setup.py` & `emergefs-0.0.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -119,15 +119,15 @@
     version=about['__version__'],
     author=about['__author__'],
     author_email=about['__author_email__'],
     url=about['__url__'],
     packages=['emerge', 'emerge.zmq', 'emerge.data', 'emerge.core', 'emerge.node', 'emerge.fs', 'emerge.file',
               'emerge.compute', 'emerge.cli', 'emerge.tests'],
     include_package_data=True,
-    python_requires=">=3.8.*",
+    python_requires=">=3.9",
     install_requires=[
         'pytest',
         'click',
         'black',
         'isort',
         'flake8',
         'zerorpc'
```

