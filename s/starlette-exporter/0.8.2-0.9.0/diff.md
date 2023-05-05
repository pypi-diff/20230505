# Comparing `tmp/starlette_exporter-0.8.2.tar.gz` & `tmp/starlette_exporter-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "starlette_exporter-0.8.2.tar", last modified: Fri May 28 04:12:42 2021, max compression
+gzip compressed data, was "starlette_exporter-0.9.0.tar", last modified: Fri Jun 11 05:11:46 2021, max compression
```

## Comparing `starlette_exporter-0.8.2.tar` & `starlette_exporter-0.9.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 steve     (1000) wheel       (10)        0 2021-05-28 04:12:42.077556 starlette_exporter-0.8.2/
--rw-r--r--   0 steve     (1000) wheel       (10)    11357 2019-10-26 22:05:14.000000 starlette_exporter-0.8.2/LICENSE
--rw-r--r--   0 steve     (1000) wheel       (10)     4663 2021-05-28 04:12:42.077556 starlette_exporter-0.8.2/PKG-INFO
--rw-r--r--   0 steve     (1000) wheel       (10)     4298 2021-05-28 04:11:49.000000 starlette_exporter-0.8.2/README.md
--rw-r--r--   0 steve     (1000) wheel       (10)       38 2021-05-28 04:12:42.077556 starlette_exporter-0.8.2/setup.cfg
--rw-r--r--   0 steve     (1000) wheel       (10)      553 2021-05-28 04:06:08.000000 starlette_exporter-0.8.2/setup.py
-drwxr-xr-x   0 steve     (1000) wheel       (10)        0 2021-05-28 04:12:42.077556 starlette_exporter-0.8.2/starlette_exporter/
--rw-r--r--   0 steve     (1000) wheel       (10)      832 2021-05-28 04:08:28.000000 starlette_exporter-0.8.2/starlette_exporter/__init__.py
--rw-r--r--   0 steve     (1000) wheel       (10)     5204 2021-05-28 04:08:28.000000 starlette_exporter-0.8.2/starlette_exporter/middleware.py
-drwxr-xr-x   0 steve     (1000) wheel       (10)        0 2021-05-28 04:12:42.077556 starlette_exporter-0.8.2/starlette_exporter.egg-info/
--rw-r--r--   0 steve     (1000) wheel       (10)     4663 2021-05-28 04:12:42.000000 starlette_exporter-0.8.2/starlette_exporter.egg-info/PKG-INFO
--rw-r--r--   0 steve     (1000) wheel       (10)      299 2021-05-28 04:12:42.000000 starlette_exporter-0.8.2/starlette_exporter.egg-info/SOURCES.txt
--rw-r--r--   0 steve     (1000) wheel       (10)        1 2021-05-28 04:12:42.000000 starlette_exporter-0.8.2/starlette_exporter.egg-info/dependency_links.txt
--rw-r--r--   0 steve     (1000) wheel       (10)       28 2021-05-28 04:12:42.000000 starlette_exporter-0.8.2/starlette_exporter.egg-info/requires.txt
--rw-r--r--   0 steve     (1000) wheel       (10)       19 2021-05-28 04:12:42.000000 starlette_exporter-0.8.2/starlette_exporter.egg-info/top_level.txt
+drwxr-xr-x   0 steve     (1000) wheel       (10)        0 2021-06-11 05:11:46.391474 starlette_exporter-0.9.0/
+-rw-r--r--   0 steve     (1000) wheel       (10)    11357 2021-06-11 05:11:08.000000 starlette_exporter-0.9.0/LICENSE
+-rw-r--r--   0 steve     (1000) wheel       (10)     4663 2021-06-11 05:11:46.391474 starlette_exporter-0.9.0/PKG-INFO
+-rw-r--r--   0 steve     (1000) wheel       (10)     4298 2021-06-11 05:11:08.000000 starlette_exporter-0.9.0/README.md
+-rw-r--r--   0 steve     (1000) wheel       (10)       38 2021-06-11 05:11:46.391474 starlette_exporter-0.9.0/setup.cfg
+-rw-r--r--   0 steve     (1000) wheel       (10)      553 2021-06-11 05:11:08.000000 starlette_exporter-0.9.0/setup.py
+drwxr-xr-x   0 steve     (1000) wheel       (10)        0 2021-06-11 05:11:46.391474 starlette_exporter-0.9.0/starlette_exporter/
+-rw-r--r--   0 steve     (1000) wheel       (10)      832 2021-05-28 04:08:28.000000 starlette_exporter-0.9.0/starlette_exporter/__init__.py
+-rw-r--r--   0 steve     (1000) wheel       (10)     5897 2021-06-11 05:09:07.000000 starlette_exporter-0.9.0/starlette_exporter/middleware.py
+drwxr-xr-x   0 steve     (1000) wheel       (10)        0 2021-06-11 05:11:46.391474 starlette_exporter-0.9.0/starlette_exporter.egg-info/
+-rw-r--r--   0 steve     (1000) wheel       (10)     4663 2021-06-11 05:11:46.000000 starlette_exporter-0.9.0/starlette_exporter.egg-info/PKG-INFO
+-rw-r--r--   0 steve     (1000) wheel       (10)      299 2021-06-11 05:11:46.000000 starlette_exporter-0.9.0/starlette_exporter.egg-info/SOURCES.txt
+-rw-r--r--   0 steve     (1000) wheel       (10)        1 2021-06-11 05:11:46.000000 starlette_exporter-0.9.0/starlette_exporter.egg-info/dependency_links.txt
+-rw-r--r--   0 steve     (1000) wheel       (10)       28 2021-06-11 05:11:46.000000 starlette_exporter-0.9.0/starlette_exporter.egg-info/requires.txt
+-rw-r--r--   0 steve     (1000) wheel       (10)       19 2021-06-11 05:11:46.000000 starlette_exporter-0.9.0/starlette_exporter.egg-info/top_level.txt
```

### Comparing `starlette_exporter-0.8.2/LICENSE` & `starlette_exporter-0.9.0/LICENSE`

 * *Files identical despite different names*

### Comparing `starlette_exporter-0.8.2/PKG-INFO` & `starlette_exporter-0.9.0/starlette_exporter.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: starlette_exporter
-Version: 0.8.2
+Name: starlette-exporter
+Version: 0.9.0
 Summary: Prometheus metrics exporter for Starlette applications.
 Home-page: https://github.com/stephenhillier/starlette_exporter
 Author: Stephen Hillier
 Author-email: stephenhillier@gmail.com
 License: Apache License 2.0
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `starlette_exporter-0.8.2/README.md` & `starlette_exporter-0.9.0/README.md`

 * *Files identical despite different names*

### Comparing `starlette_exporter-0.8.2/setup.py` & `starlette_exporter-0.9.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
     name='starlette_exporter',
-    version='0.8.2',
+    version='0.9.0',
     author='Stephen Hillier',
     author_email='stephenhillier@gmail.com',
     packages=['starlette_exporter'],
     license='Apache License 2.0',
     url="https://github.com/stephenhillier/starlette_exporter",
     description='Prometheus metrics exporter for Starlette applications.',
     long_description=open('README.md').read(),
```

### Comparing `starlette_exporter-0.8.2/starlette_exporter/__init__.py` & `starlette_exporter-0.9.0/starlette_exporter/__init__.py`

 * *Files identical despite different names*

### Comparing `starlette_exporter-0.8.2/starlette_exporter/middleware.py` & `starlette_exporter-0.9.0/starlette_exporter/middleware.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,19 +1,43 @@
 """ Middleware for exporting Prometheus metrics using Starlette """
 import time
-from logging import getLogger
+import logging
 from typing import List, Optional, ClassVar, Dict
 
 from prometheus_client import Counter, Histogram
 from prometheus_client.metrics import MetricWrapperBase
 from starlette.requests import Request
-from starlette.types import ASGIApp, Message, Receive, Scope, Send
+from starlette.routing import Route, Match, Mount
+from starlette.types import ASGIApp, Message, Receive, Send, Scope
 
+logger = logging.getLogger("exporter")
 
-logger = getLogger("exporter")
+
+def get_matching_route_path(scope: Dict, routes: List[Route], route_name: Optional[str] = None) -> str:
+    """
+    Find a matching route and return its original path string
+
+    Will attempt to enter mounted routes and subrouters.
+
+    Credit to https://github.com/elastic/apm-agent-python
+    """
+    for route in routes:
+        match, child_scope = route.matches(scope)
+        if match == Match.FULL:
+            route_name = route.path
+            child_scope = {**scope, **child_scope}
+            if isinstance(route, Mount) and route.routes:
+                child_route_name = get_matching_route_path(child_scope, route.routes, route_name)
+                if child_route_name is None:
+                    route_name = None
+                else:
+                    route_name += child_route_name
+            return route_name
+        elif match == Match.PARTIAL and route_name is None:
+            route_name = route.path
 
 
 class PrometheusMiddleware:
     """ Middleware that collects Prometheus metrics for each request.
         Use in conjuction with the Prometheus exporter endpoint handler.
     """
     _metrics: ClassVar[Dict[str, MetricWrapperBase]] = {}
@@ -83,15 +107,15 @@
 
             await send(message)
 
         try:
             await self.app(scope, receive, wrapped_send)
         finally:
             if self.filter_unhandled_paths or self.group_paths:
-                grouped_path = self._get_router_path(request)
+                grouped_path = self._get_router_path(scope)
 
                 # filter_unhandled_paths removes any requests without mapped endpoint from the metrics.
                 if self.filter_unhandled_paths and grouped_path is None:
                     return
 
                 # group_paths enables returning the original router path (with url param names)
                 # for example, when using this option, requests to /api/product/1 and /api/product/3
@@ -106,29 +130,27 @@
             if end is None:
                 end = time.perf_counter()
 
             self.request_count.labels(*labels).inc()
             self.request_time.labels(*labels).observe(end - begin)
 
     @staticmethod
-    def _get_router_path(request: Request) -> Optional[str]:
+    def _get_router_path(scope: Scope) -> Optional[str]:
         """Returns the original router path (with url param names) for given request."""
-        try:
-            if not (request.scope.get('endpoint') and request.scope.get('router')):
-                return None
+        if not (scope.get("endpoint", None) and scope.get("router", None)):
+            return None
 
-            for route in request.scope['router'].routes:
-                if ((
-                        hasattr(route, 'endpoint')
-                        and route.endpoint == request.scope['endpoint']
-                    )
-                    # for endpoints handled by another app, like fastapi.staticfiles.StaticFiles,
-                    # check if the request endpoint matches a mounted app.
-                    or (
-                        hasattr(route, 'app')
-                        and route.app == request.scope['endpoint']
-                    )):
-                    return route.path
+        base_scope = {
+            "type": scope.get("type"),
+            "path": scope.get("root_path", "") + scope.get("path"),
+            "path_params": scope.get("path_params", {}),
+            "method": scope.get("method"),
+        }
+
+        try:
+            path = get_matching_route_path(base_scope, scope.get("router").routes)
+            return path
         except:
-            logger.exception("Failed to fetch router path.")
+            # unhandled path
+            pass
 
         return None
```

### Comparing `starlette_exporter-0.8.2/starlette_exporter.egg-info/PKG-INFO` & `starlette_exporter-0.9.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: starlette-exporter
-Version: 0.8.2
+Name: starlette_exporter
+Version: 0.9.0
 Summary: Prometheus metrics exporter for Starlette applications.
 Home-page: https://github.com/stephenhillier/starlette_exporter
 Author: Stephen Hillier
 Author-email: stephenhillier@gmail.com
 License: Apache License 2.0
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

