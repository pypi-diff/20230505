# Comparing `tmp/mango_pycore-0.1.7a0.tar.gz` & `tmp/mango_pycore-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mango_pycore-0.1.7a0.tar", max compression
+gzip compressed data, was "mango_pycore-0.1.8.tar", max compression
```

## Comparing `mango_pycore-0.1.7a0.tar` & `mango_pycore-0.1.8.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0      193 2023-04-27 06:19:29.749731 mango_pycore-0.1.7a0/README.md
--rw-r--r--   0        0        0        0 2023-04-27 06:19:29.749731 mango_pycore-0.1.7a0/mango_pycore/__init__.py
--rw-r--r--   0        0        0        0 2023-04-27 06:19:29.749731 mango_pycore-0.1.7a0/mango_pycore/api/__init__.py
--rw-r--r--   0        0        0     3067 2023-04-27 06:19:29.749731 mango_pycore-0.1.7a0/mango_pycore/api/base_api.py
--rw-r--r--   0        0        0      290 2023-04-27 06:19:29.749731 mango_pycore-0.1.7a0/mango_pycore/api/exceptions.py
--rw-r--r--   0        0        0     2089 2023-04-27 06:19:29.749731 mango_pycore-0.1.7a0/mango_pycore/api/http_api.py
--rw-r--r--   0        0        0     4945 2023-04-27 06:19:29.749731 mango_pycore-0.1.7a0/mango_pycore/api/request.py
--rw-r--r--   0        0        0      627 2023-04-27 06:19:29.749731 mango_pycore-0.1.7a0/mango_pycore/api/response.py
--rw-r--r--   0        0        0     2089 2023-04-27 06:19:29.749731 mango_pycore-0.1.7a0/mango_pycore/api/rest_api.py
--rw-r--r--   0        0        0     2710 2023-04-27 06:19:29.749731 mango_pycore-0.1.7a0/mango_pycore/api/websocket_api.py
--rw-r--r--   0        0        0        0 2023-04-27 06:19:29.749731 mango_pycore-0.1.7a0/mango_pycore/stream/__init__.py
--rw-r--r--   0        0        0     3965 2023-04-27 06:19:29.749731 mango_pycore-0.1.7a0/mango_pycore/stream/dynamo.py
--rw-r--r--   0        0        0        0 2023-04-27 06:19:29.749731 mango_pycore-0.1.7a0/mango_pycore/tools/__init__.py
--rw-r--r--   0        0        0      175 2023-04-27 06:19:29.749731 mango_pycore-0.1.7a0/mango_pycore/tools/utils.py
--rw-r--r--   0        0        0        0 2023-04-27 06:19:29.749731 mango_pycore-0.1.7a0/mango_pycore/websocket/__init__.py
--rw-r--r--   0        0        0     1333 2023-04-27 06:19:29.749731 mango_pycore-0.1.7a0/mango_pycore/websocket/client.py
--rw-r--r--   0        0        0      373 2023-04-27 06:19:29.749731 mango_pycore-0.1.7a0/pyproject.toml
--rw-r--r--   0        0        0      739 1970-01-01 00:00:00.000000 mango_pycore-0.1.7a0/PKG-INFO
+-rw-r--r--   0        0        0      193 2023-05-05 19:17:49.319864 mango_pycore-0.1.8/README.md
+-rw-r--r--   0        0        0        0 2023-05-05 19:17:49.319864 mango_pycore-0.1.8/mango_pycore/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-05 19:17:49.319864 mango_pycore-0.1.8/mango_pycore/api/__init__.py
+-rw-r--r--   0        0        0     3076 2023-05-05 19:17:49.319864 mango_pycore-0.1.8/mango_pycore/api/base_api.py
+-rw-r--r--   0        0        0      290 2023-05-05 19:17:49.319864 mango_pycore-0.1.8/mango_pycore/api/exceptions.py
+-rw-r--r--   0        0        0     2089 2023-05-05 19:17:49.319864 mango_pycore-0.1.8/mango_pycore/api/http_api.py
+-rw-r--r--   0        0        0     4945 2023-05-05 19:17:49.319864 mango_pycore-0.1.8/mango_pycore/api/request.py
+-rw-r--r--   0        0        0      627 2023-05-05 19:17:49.319864 mango_pycore-0.1.8/mango_pycore/api/response.py
+-rw-r--r--   0        0        0     2089 2023-05-05 19:17:49.319864 mango_pycore-0.1.8/mango_pycore/api/rest_api.py
+-rw-r--r--   0        0        0     2710 2023-05-05 19:17:49.319864 mango_pycore-0.1.8/mango_pycore/api/websocket_api.py
+-rw-r--r--   0        0        0        0 2023-05-05 19:17:49.319864 mango_pycore-0.1.8/mango_pycore/stream/__init__.py
+-rw-r--r--   0        0        0     3965 2023-05-05 19:17:49.319864 mango_pycore-0.1.8/mango_pycore/stream/dynamo.py
+-rw-r--r--   0        0        0        0 2023-05-05 19:17:49.319864 mango_pycore-0.1.8/mango_pycore/tools/__init__.py
+-rw-r--r--   0        0        0      175 2023-05-05 19:17:49.319864 mango_pycore-0.1.8/mango_pycore/tools/utils.py
+-rw-r--r--   0        0        0        0 2023-05-05 19:17:49.319864 mango_pycore-0.1.8/mango_pycore/websocket/__init__.py
+-rw-r--r--   0        0        0     1333 2023-05-05 19:17:49.319864 mango_pycore-0.1.8/mango_pycore/websocket/client.py
+-rw-r--r--   0        0        0      371 2023-05-05 19:18:01.203884 mango_pycore-0.1.8/pyproject.toml
+-rw-r--r--   0        0        0      737 1970-01-01 00:00:00.000000 mango_pycore-0.1.8/PKG-INFO
```

### Comparing `mango_pycore-0.1.7a0/mango_pycore/api/base_api.py` & `mango_pycore-0.1.8/mango_pycore/api/base_api.py`

 * *Files 1% similar despite different names*

```diff
@@ -58,15 +58,15 @@
             rslt = midd(req)
             if isinstance(rslt, BaseRequest):
                 req = copy(rslt)
             if isinstance(rslt, Response):
                 raise MiddlewareShortCircuit(response=rslt.to_dict())
         return req
 
-    def _process_options_request(self):
+    def _process_options_request(self, request):
         return Response(
             code=200,
             headers=self.cors_headers
         )
 
     def _config_logging(self):
         logger = logging.getLogger(self.name)
```

### Comparing `mango_pycore-0.1.7a0/mango_pycore/api/http_api.py` & `mango_pycore-0.1.8/mango_pycore/api/http_api.py`

 * *Files identical despite different names*

### Comparing `mango_pycore-0.1.7a0/mango_pycore/api/request.py` & `mango_pycore-0.1.8/mango_pycore/api/request.py`

 * *Files identical despite different names*

### Comparing `mango_pycore-0.1.7a0/mango_pycore/api/response.py` & `mango_pycore-0.1.8/mango_pycore/api/response.py`

 * *Files identical despite different names*

### Comparing `mango_pycore-0.1.7a0/mango_pycore/api/rest_api.py` & `mango_pycore-0.1.8/mango_pycore/api/rest_api.py`

 * *Files identical despite different names*

### Comparing `mango_pycore-0.1.7a0/mango_pycore/api/websocket_api.py` & `mango_pycore-0.1.8/mango_pycore/api/websocket_api.py`

 * *Files identical despite different names*

### Comparing `mango_pycore-0.1.7a0/mango_pycore/stream/dynamo.py` & `mango_pycore-0.1.8/mango_pycore/stream/dynamo.py`

 * *Files identical despite different names*

### Comparing `mango_pycore-0.1.7a0/mango_pycore/websocket/client.py` & `mango_pycore-0.1.8/mango_pycore/websocket/client.py`

 * *Files identical despite different names*

### Comparing `mango_pycore-0.1.7a0/PKG-INFO` & `mango_pycore-0.1.8/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mango-pycore
-Version: 0.1.7a0
+Version: 0.1.8
 Summary: 
 Author: Ernesto Licea Martin
 Author-email: ernesto.licea@mango-soft.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

