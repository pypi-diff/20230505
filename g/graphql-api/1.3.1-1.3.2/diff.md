# Comparing `tmp/graphql-api-1.3.1.tar.gz` & `tmp/graphql-api-1.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "graphql-api-1.3.1.tar", last modified: Mon Apr 24 14:17:59 2023, max compression
+gzip compressed data, was "graphql-api-1.3.2.tar", last modified: Fri May  5 12:27:33 2023, max compression
```

## Comparing `graphql-api-1.3.1.tar` & `graphql-api-1.3.2.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 14:17:59.895662 graphql-api-1.3.1/
--rwxrwxrwx   0 root         (0) root         (0)     1069 2023-04-24 14:17:50.000000 graphql-api-1.3.1/LICENSE
--rwxrwxrwx   0 root         (0) root         (0)       73 2023-04-24 14:17:50.000000 graphql-api-1.3.1/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     1946 2023-04-24 14:17:59.895662 graphql-api-1.3.1/PKG-INFO
--rwxrwxrwx   0 root         (0) root         (0)     1270 2023-04-24 14:17:50.000000 graphql-api-1.3.1/README.md
--rw-rw-rw-   0 root         (0) root         (0)        6 2023-04-24 14:17:59.000000 graphql-api-1.3.1/VERSION
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 14:17:59.890662 graphql-api-1.3.1/graphql_api/
--rwxrwxrwx   0 root         (0) root         (0)      286 2023-04-24 14:17:50.000000 graphql-api-1.3.1/graphql_api/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)     7527 2023-04-24 14:17:50.000000 graphql-api-1.3.1/graphql_api/api.py
--rwxrwxrwx   0 root         (0) root         (0)      558 2023-04-24 14:17:50.000000 graphql-api-1.3.1/graphql_api/context.py
--rwxrwxrwx   0 root         (0) root         (0)     3382 2023-04-24 14:17:50.000000 graphql-api-1.3.1/graphql_api/dataclass_mapping.py
--rw-rw-rw-   0 root         (0) root         (0)      403 2023-04-24 14:17:50.000000 graphql-api-1.3.1/graphql_api/decorators.py
--rwxrwxrwx   0 root         (0) root         (0)      593 2023-04-24 14:17:50.000000 graphql-api-1.3.1/graphql_api/error.py
--rwxrwxrwx   0 root         (0) root         (0)       52 2023-04-24 14:17:50.000000 graphql-api-1.3.1/graphql_api/exception.py
--rwxrwxrwx   0 root         (0) root         (0)     5868 2023-04-24 14:17:50.000000 graphql-api-1.3.1/graphql_api/executor.py
--rwxrwxrwx   0 root         (0) root         (0)    23879 2023-04-24 14:17:50.000000 graphql-api-1.3.1/graphql_api/mapper.py
--rwxrwxrwx   0 root         (0) root         (0)     3070 2023-04-24 14:17:50.000000 graphql-api-1.3.1/graphql_api/middleware.py
--rwxrwxrwx   0 root         (0) root         (0)     6756 2023-04-24 14:17:50.000000 graphql-api-1.3.1/graphql_api/reduce.py
--rwxrwxrwx   0 root         (0) root         (0)     3154 2023-04-24 14:17:50.000000 graphql-api-1.3.1/graphql_api/relay.py
--rwxrwxrwx   0 root         (0) root         (0)    32840 2023-04-24 14:17:50.000000 graphql-api-1.3.1/graphql_api/remote.py
--rwxrwxrwx   0 root         (0) root         (0)     3372 2023-04-24 14:17:50.000000 graphql-api-1.3.1/graphql_api/types.py
--rwxrwxrwx   0 root         (0) root         (0)     5612 2023-04-24 14:17:50.000000 graphql-api-1.3.1/graphql_api/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 14:17:59.891662 graphql-api-1.3.1/graphql_api.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1946 2023-04-24 14:17:59.000000 graphql-api-1.3.1/graphql_api.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      806 2023-04-24 14:17:59.000000 graphql-api-1.3.1/graphql_api.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-24 14:17:59.000000 graphql-api-1.3.1/graphql_api.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      150 2023-04-24 14:17:59.000000 graphql-api-1.3.1/graphql_api.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       18 2023-04-24 14:17:59.000000 graphql-api-1.3.1/graphql_api.egg-info/top_level.txt
--rwxrwxrwx   0 root         (0) root         (0)       79 2023-04-24 14:17:59.895662 graphql-api-1.3.1/setup.cfg
--rwxrwxrwx   0 root         (0) root         (0)     1413 2023-04-24 14:17:50.000000 graphql-api-1.3.1/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-24 14:17:59.894662 graphql-api-1.3.1/tests/
--rwxrwxrwx   0 root         (0) root         (0)      286 2023-04-24 14:17:50.000000 graphql-api-1.3.1/tests/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)     5129 2023-04-24 14:17:50.000000 graphql-api-1.3.1/tests/test_custom_types.py
--rwxrwxrwx   0 root         (0) root         (0)     5183 2023-04-24 14:17:50.000000 graphql-api-1.3.1/tests/test_docstrings.py
--rwxrwxrwx   0 root         (0) root         (0)     3316 2023-04-24 14:17:50.000000 graphql-api-1.3.1/tests/test_error.py
--rwxrwxrwx   0 root         (0) root         (0)     6939 2023-04-24 14:17:50.000000 graphql-api-1.3.1/tests/test_filtering.py
--rwxrwxrwx   0 root         (0) root         (0)    35981 2023-04-24 14:17:50.000000 graphql-api-1.3.1/tests/test_graphql.py
--rwxrwxrwx   0 root         (0) root         (0)     4026 2023-04-24 14:17:50.000000 graphql-api-1.3.1/tests/test_relay.py
--rwxrwxrwx   0 root         (0) root         (0)    17896 2023-04-24 14:17:50.000000 graphql-api-1.3.1/tests/test_remote.py
--rw-rw-rw-   0 root         (0) root         (0)     3198 2023-04-24 14:17:50.000000 graphql-api-1.3.1/tests/test_schema.py
--rw-rw-rw-   0 root         (0) root         (0)     3543 2023-04-24 14:17:50.000000 graphql-api-1.3.1/tests/test_subscriptions.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 12:27:33.984700 graphql-api-1.3.2/
+-rwxrwxrwx   0 root         (0) root         (0)     1069 2023-05-05 12:27:24.000000 graphql-api-1.3.2/LICENSE
+-rwxrwxrwx   0 root         (0) root         (0)       73 2023-05-05 12:27:24.000000 graphql-api-1.3.2/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     1946 2023-05-05 12:27:33.984700 graphql-api-1.3.2/PKG-INFO
+-rwxrwxrwx   0 root         (0) root         (0)     1270 2023-05-05 12:27:24.000000 graphql-api-1.3.2/README.md
+-rw-rw-rw-   0 root         (0) root         (0)        6 2023-05-05 12:27:33.000000 graphql-api-1.3.2/VERSION
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 12:27:33.979700 graphql-api-1.3.2/graphql_api/
+-rwxrwxrwx   0 root         (0) root         (0)      286 2023-05-05 12:27:24.000000 graphql-api-1.3.2/graphql_api/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)     7527 2023-05-05 12:27:24.000000 graphql-api-1.3.2/graphql_api/api.py
+-rwxrwxrwx   0 root         (0) root         (0)      558 2023-05-05 12:27:24.000000 graphql-api-1.3.2/graphql_api/context.py
+-rwxrwxrwx   0 root         (0) root         (0)     3382 2023-05-05 12:27:24.000000 graphql-api-1.3.2/graphql_api/dataclass_mapping.py
+-rw-rw-rw-   0 root         (0) root         (0)      403 2023-05-05 12:27:24.000000 graphql-api-1.3.2/graphql_api/decorators.py
+-rwxrwxrwx   0 root         (0) root         (0)      593 2023-05-05 12:27:24.000000 graphql-api-1.3.2/graphql_api/error.py
+-rwxrwxrwx   0 root         (0) root         (0)       52 2023-05-05 12:27:24.000000 graphql-api-1.3.2/graphql_api/exception.py
+-rwxrwxrwx   0 root         (0) root         (0)     5868 2023-05-05 12:27:24.000000 graphql-api-1.3.2/graphql_api/executor.py
+-rwxrwxrwx   0 root         (0) root         (0)    23879 2023-05-05 12:27:24.000000 graphql-api-1.3.2/graphql_api/mapper.py
+-rwxrwxrwx   0 root         (0) root         (0)     3070 2023-05-05 12:27:24.000000 graphql-api-1.3.2/graphql_api/middleware.py
+-rwxrwxrwx   0 root         (0) root         (0)     6756 2023-05-05 12:27:24.000000 graphql-api-1.3.2/graphql_api/reduce.py
+-rwxrwxrwx   0 root         (0) root         (0)     3154 2023-05-05 12:27:24.000000 graphql-api-1.3.2/graphql_api/relay.py
+-rwxrwxrwx   0 root         (0) root         (0)    32840 2023-05-05 12:27:24.000000 graphql-api-1.3.2/graphql_api/remote.py
+-rwxrwxrwx   0 root         (0) root         (0)     3372 2023-05-05 12:27:24.000000 graphql-api-1.3.2/graphql_api/types.py
+-rwxrwxrwx   0 root         (0) root         (0)     5612 2023-05-05 12:27:24.000000 graphql-api-1.3.2/graphql_api/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 12:27:33.980700 graphql-api-1.3.2/graphql_api.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1946 2023-05-05 12:27:33.000000 graphql-api-1.3.2/graphql_api.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      806 2023-05-05 12:27:33.000000 graphql-api-1.3.2/graphql_api.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-05 12:27:33.000000 graphql-api-1.3.2/graphql_api.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      150 2023-05-05 12:27:33.000000 graphql-api-1.3.2/graphql_api.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       18 2023-05-05 12:27:33.000000 graphql-api-1.3.2/graphql_api.egg-info/top_level.txt
+-rwxrwxrwx   0 root         (0) root         (0)       79 2023-05-05 12:27:33.984700 graphql-api-1.3.2/setup.cfg
+-rwxrwxrwx   0 root         (0) root         (0)     1413 2023-05-05 12:27:24.000000 graphql-api-1.3.2/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 12:27:33.983700 graphql-api-1.3.2/tests/
+-rwxrwxrwx   0 root         (0) root         (0)      286 2023-05-05 12:27:24.000000 graphql-api-1.3.2/tests/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)     5129 2023-05-05 12:27:24.000000 graphql-api-1.3.2/tests/test_custom_types.py
+-rwxrwxrwx   0 root         (0) root         (0)     5183 2023-05-05 12:27:24.000000 graphql-api-1.3.2/tests/test_docstrings.py
+-rwxrwxrwx   0 root         (0) root         (0)     3316 2023-05-05 12:27:24.000000 graphql-api-1.3.2/tests/test_error.py
+-rwxrwxrwx   0 root         (0) root         (0)     6939 2023-05-05 12:27:24.000000 graphql-api-1.3.2/tests/test_filtering.py
+-rwxrwxrwx   0 root         (0) root         (0)    35981 2023-05-05 12:27:24.000000 graphql-api-1.3.2/tests/test_graphql.py
+-rwxrwxrwx   0 root         (0) root         (0)     4026 2023-05-05 12:27:24.000000 graphql-api-1.3.2/tests/test_relay.py
+-rwxrwxrwx   0 root         (0) root         (0)    21648 2023-05-05 12:27:24.000000 graphql-api-1.3.2/tests/test_remote.py
+-rw-rw-rw-   0 root         (0) root         (0)     3198 2023-05-05 12:27:24.000000 graphql-api-1.3.2/tests/test_schema.py
+-rw-rw-rw-   0 root         (0) root         (0)     3543 2023-05-05 12:27:24.000000 graphql-api-1.3.2/tests/test_subscriptions.py
```

### Comparing `graphql-api-1.3.1/LICENSE` & `graphql-api-1.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `graphql-api-1.3.1/PKG-INFO` & `graphql-api-1.3.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: graphql-api
-Version: 1.3.1
+Version: 1.3.2
 Summary: A framework for building Python GraphQL APIs.
 Home-page: https://gitlab.com/parob/graphql-api
-Download-URL: https://gitlab.com/parob/graphql/-/archive/v1.3.1/graphql-api-v1.3.1.tar.gz
+Download-URL: https://gitlab.com/parob/graphql/-/archive/v1.3.2/graphql-api-v1.3.2.tar.gz
 Author: Robert Parker
 Author-email: rob@parob.com
 License: MIT
 Keywords: GraphQL,GraphQL-API,GraphQLAPI,Server
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `graphql-api-1.3.1/README.md` & `graphql-api-1.3.2/README.md`

 * *Files identical despite different names*

### Comparing `graphql-api-1.3.1/graphql_api/api.py` & `graphql-api-1.3.2/graphql_api/api.py`

 * *Files identical despite different names*

### Comparing `graphql-api-1.3.1/graphql_api/context.py` & `graphql-api-1.3.2/graphql_api/context.py`

 * *Files identical despite different names*

### Comparing `graphql-api-1.3.1/graphql_api/dataclass_mapping.py` & `graphql-api-1.3.2/graphql_api/dataclass_mapping.py`

 * *Files identical despite different names*

### Comparing `graphql-api-1.3.1/graphql_api/error.py` & `graphql-api-1.3.2/graphql_api/error.py`

 * *Files identical despite different names*

### Comparing `graphql-api-1.3.1/graphql_api/executor.py` & `graphql-api-1.3.2/graphql_api/executor.py`

 * *Files identical despite different names*

### Comparing `graphql-api-1.3.1/graphql_api/mapper.py` & `graphql-api-1.3.2/graphql_api/mapper.py`

 * *Files identical despite different names*

### Comparing `graphql-api-1.3.1/graphql_api/middleware.py` & `graphql-api-1.3.2/graphql_api/middleware.py`

 * *Files identical despite different names*

### Comparing `graphql-api-1.3.1/graphql_api/reduce.py` & `graphql-api-1.3.2/graphql_api/reduce.py`

 * *Files identical despite different names*

### Comparing `graphql-api-1.3.1/graphql_api/relay.py` & `graphql-api-1.3.2/graphql_api/relay.py`

 * *Files identical despite different names*

### Comparing `graphql-api-1.3.1/graphql_api/remote.py` & `graphql-api-1.3.2/graphql_api/remote.py`

 * *Files identical despite different names*

### Comparing `graphql-api-1.3.1/graphql_api/types.py` & `graphql-api-1.3.2/graphql_api/types.py`

 * *Files identical despite different names*

### Comparing `graphql-api-1.3.1/graphql_api/utils.py` & `graphql-api-1.3.2/graphql_api/utils.py`

 * *Files identical despite different names*

### Comparing `graphql-api-1.3.1/graphql_api.egg-info/PKG-INFO` & `graphql-api-1.3.2/graphql_api.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: graphql-api
-Version: 1.3.1
+Version: 1.3.2
 Summary: A framework for building Python GraphQL APIs.
 Home-page: https://gitlab.com/parob/graphql-api
-Download-URL: https://gitlab.com/parob/graphql/-/archive/v1.3.1/graphql-api-v1.3.1.tar.gz
+Download-URL: https://gitlab.com/parob/graphql/-/archive/v1.3.2/graphql-api-v1.3.2.tar.gz
 Author: Robert Parker
 Author-email: rob@parob.com
 License: MIT
 Keywords: GraphQL,GraphQL-API,GraphQLAPI,Server
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `graphql-api-1.3.1/graphql_api.egg-info/SOURCES.txt` & `graphql-api-1.3.2/graphql_api.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `graphql-api-1.3.1/setup.py` & `graphql-api-1.3.2/setup.py`

 * *Files identical despite different names*

### Comparing `graphql-api-1.3.1/tests/test_custom_types.py` & `graphql-api-1.3.2/tests/test_custom_types.py`

 * *Files identical despite different names*

### Comparing `graphql-api-1.3.1/tests/test_docstrings.py` & `graphql-api-1.3.2/tests/test_docstrings.py`

 * *Files identical despite different names*

### Comparing `graphql-api-1.3.1/tests/test_error.py` & `graphql-api-1.3.2/tests/test_error.py`

 * *Files identical despite different names*

### Comparing `graphql-api-1.3.1/tests/test_filtering.py` & `graphql-api-1.3.2/tests/test_filtering.py`

 * *Files identical despite different names*

### Comparing `graphql-api-1.3.1/tests/test_graphql.py` & `graphql-api-1.3.2/tests/test_graphql.py`

 * *Files identical despite different names*

### Comparing `graphql-api-1.3.1/tests/test_relay.py` & `graphql-api-1.3.2/tests/test_relay.py`

 * *Files identical despite different names*

### Comparing `graphql-api-1.3.1/tests/test_remote.py` & `graphql-api-1.3.2/tests/test_remote.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 import asyncio
 import enum
+import random
 import uuid
+from dataclasses import dataclass
 
 from typing import Optional, List
 from uuid import UUID
 
 import time
 import pytest
 
@@ -383,14 +385,126 @@
             assert house.value(garden=Garden(animal=Animal(age=5), size=10)) == 85
 
         assert (
             house.value(garden=Garden(animal=Animal(age=5), set_animal=True, size=10))
             == 85
         )
 
+    def test_remote_return_object(self):
+        api = GraphQLAPI()
+
+        @dataclass
+        class Door:
+            height: int
+
+        @api.type(root=True)
+        class House:
+            @api.field
+            def doors(self) -> List[Door]:
+                return [Door(height=180), Door(height=204)]
+
+            @api.field
+            def front_door(self) -> Door:
+                return Door(height=204)
+
+        house: House = GraphQLRemoteObject(executor=api.executor(), api=api)
+
+        assert house.doors()[0].height == 180
+        assert house.front_door().height == 204
+
+    def test_remote_return_object_call_count(self):
+        api = GraphQLAPI()
+
+        @dataclass
+        class Door:
+            height: int
+            weight: int
+
+        @api.type(root=True)
+        class House:
+            def __init__(self):
+                self.api_calls = 0
+
+            @api.field
+            def number(self) -> int:
+                self.api_calls += 1
+                return 18
+
+            @api.field
+            def front_door(self) -> Door:
+                self.api_calls += 1
+                return Door(height=204, weight=70)
+
+        root_house = House()
+
+        house: House = GraphQLRemoteObject(
+            executor=api.executor(root_value=root_house),
+            api=api,
+        )
+
+        front_door = house.front_door()
+        assert root_house.api_calls == 0
+
+        assert front_door.height == 204
+        assert front_door.weight == 70
+
+        assert root_house.api_calls == 2
+
+        assert front_door.height == 204
+
+        assert root_house.api_calls == 2
+
+        front_door = house.front_door()
+        assert root_house.api_calls == 2
+
+        assert front_door.height == 204
+
+        assert root_house.api_calls == 3
+        root_house.api_calls = 0
+
+        assert root_house.number() == 18
+        assert root_house.number() == 18
+        assert root_house.api_calls == 2
+
+    def test_remote_return_object_cache(self):
+        api = GraphQLAPI()
+
+        @dataclass
+        class Door:
+            id: str
+
+            @api.field
+            def rand(self, max: int = 100) -> int:
+                return random.randint(0, max)
+
+        @api.type(root=True)
+        class House:
+            @api.field
+            def front_door(self, id: str) -> Door:
+                return Door(id=id)
+
+        root_house = House()
+
+        house: House = GraphQLRemoteObject(
+            executor=api.executor(root_value=root_house),
+            api=api,
+        )
+
+        front_door = house.front_door(id="door_a")
+        random_int = front_door.rand()
+        assert random_int == front_door.rand()
+        assert random_int != front_door.rand(max=200)
+        assert random_int == front_door.rand()
+
+        front_door = house.front_door(id="door_a")
+        assert random_int != front_door.rand()
+
+        front_door = house.front_door(id="door_b")
+        assert random_int != front_door.rand()
+
     def test_remote_recursive_mutated(self):
         api = GraphQLAPI()
 
         class Flopper:
             def __init__(self):
                 self._flop = True
 
@@ -639,7 +753,34 @@
             sync_utc_now_list.append(api.now())
             api.clear_cache()  # Clear the API cache so that it re-fetches the request.
         sync_time = time.time() - sync_start
 
         assert len(set(sync_utc_now_list)) == request_count
 
         assert sync_time >= 1.25 * async_time
+
+    # noinspection DuplicatedCode,PyUnusedLocal
+    @pytest.mark.skipif(
+        not available(utc_time_api_url),
+        reason=f"The UTCTime API '{utc_time_api_url}' is unavailable",
+    )
+    def test_remote_get_async_await(self):
+        utc_time_api = GraphQLAPI()
+
+        remote_executor = GraphQLRemoteExecutor(url=self.utc_time_api_url)
+
+        @utc_time_api.type(root=True)
+        class UTCTimeAPI:
+            @utc_time_api.field
+            def now(self) -> str:
+                pass
+
+        api: UTCTimeAPI = GraphQLRemoteObject(
+            executor=remote_executor, api=utc_time_api
+        )
+
+        async def fetch():
+            return await api.call_async("now")
+
+        async_utc_now = asyncio.run(fetch())
+
+        assert async_utc_now
```

### Comparing `graphql-api-1.3.1/tests/test_schema.py` & `graphql-api-1.3.2/tests/test_schema.py`

 * *Files identical despite different names*

### Comparing `graphql-api-1.3.1/tests/test_subscriptions.py` & `graphql-api-1.3.2/tests/test_subscriptions.py`

 * *Files identical despite different names*

