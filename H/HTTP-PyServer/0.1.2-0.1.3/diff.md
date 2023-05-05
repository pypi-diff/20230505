# Comparing `tmp/HTTP-PyServer-0.1.2.tar.gz` & `tmp/HTTP-PyServer-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "HTTP-PyServer-0.1.2.tar", last modified: Fri May  5 00:29:02 2023, max compression
+gzip compressed data, was "HTTP-PyServer-0.1.3.tar", last modified: Fri May  5 02:41:15 2023, max compression
```

## Comparing `HTTP-PyServer-0.1.2.tar` & `HTTP-PyServer-0.1.3.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0        0        0        0 2023-05-05 00:29:02.361660 HTTP-PyServer-0.1.2/
--rw-rw-rw-   0        0        0     1067 2023-04-12 19:57:31.000000 HTTP-PyServer-0.1.2/LICENSE
--rw-rw-rw-   0        0        0     2041 2023-05-05 00:29:02.359375 HTTP-PyServer-0.1.2/PKG-INFO
--rw-rw-rw-   0        0        0     1478 2023-05-05 00:20:57.000000 HTTP-PyServer-0.1.2/README.md
--rw-rw-rw-   0        0        0      641 2023-05-05 00:28:32.000000 HTTP-PyServer-0.1.2/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-05 00:29:02.361660 HTTP-PyServer-0.1.2/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-05-05 00:29:02.300325 HTTP-PyServer-0.1.2/src/
-drwxrwxrwx   0        0        0        0 2023-05-05 00:29:02.320391 HTTP-PyServer-0.1.2/src/HTTP_PyServer.egg-info/
--rw-rw-rw-   0        0        0     2041 2023-05-05 00:29:02.000000 HTTP-PyServer-0.1.2/src/HTTP_PyServer.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      431 2023-05-05 00:29:02.000000 HTTP-PyServer-0.1.2/src/HTTP_PyServer.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-05 00:29:02.000000 HTTP-PyServer-0.1.2/src/HTTP_PyServer.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2023-05-05 00:29:02.000000 HTTP-PyServer-0.1.2/src/HTTP_PyServer.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-05-05 00:29:02.354280 HTTP-PyServer-0.1.2/src/server/
--rw-rw-rw-   0        0        0      369 2023-05-04 03:39:37.000000 HTTP-PyServer-0.1.2/src/server/__init__.py
--rw-rw-rw-   0        0        0     2529 2023-05-05 00:15:15.000000 HTTP-PyServer-0.1.2/src/server/cache.py
--rw-rw-rw-   0        0        0     4851 2023-05-05 00:12:16.000000 HTTP-PyServer-0.1.2/src/server/render.py
--rw-rw-rw-   0        0        0     2358 2023-05-01 16:37:07.000000 HTTP-PyServer-0.1.2/src/server/request.py
--rw-rw-rw-   0        0        0     2126 2023-05-05 00:12:04.000000 HTTP-PyServer-0.1.2/src/server/response.py
--rw-rw-rw-   0        0        0     1618 2023-04-29 15:55:19.000000 HTTP-PyServer-0.1.2/src/server/response_codes.py
--rw-rw-rw-   0        0        0     2430 2023-04-29 15:55:27.000000 HTTP-PyServer-0.1.2/src/server/response_messages.py
--rw-rw-rw-   0        0        0     4773 2023-05-03 19:35:25.000000 HTTP-PyServer-0.1.2/src/server/routes.py
--rw-rw-rw-   0        0        0     6923 2023-05-04 23:56:20.000000 HTTP-PyServer-0.1.2/src/server/server.py
--rw-rw-rw-   0        0        0     1055 2023-05-05 00:01:06.000000 HTTP-PyServer-0.1.2/src/server/template.py
+drwxrwxrwx   0        0        0        0 2023-05-05 02:41:15.721046 HTTP-PyServer-0.1.3/
+-rw-rw-rw-   0        0        0     1067 2023-04-12 19:57:31.000000 HTTP-PyServer-0.1.3/LICENSE
+-rw-rw-rw-   0        0        0     2041 2023-05-05 02:41:15.718303 HTTP-PyServer-0.1.3/PKG-INFO
+-rw-rw-rw-   0        0        0     1478 2023-05-05 00:20:57.000000 HTTP-PyServer-0.1.3/README.md
+-rw-rw-rw-   0        0        0      641 2023-05-05 02:40:46.000000 HTTP-PyServer-0.1.3/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-05 02:41:15.721046 HTTP-PyServer-0.1.3/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-05 02:41:15.673612 HTTP-PyServer-0.1.3/src/
+drwxrwxrwx   0        0        0        0 2023-05-05 02:41:15.687118 HTTP-PyServer-0.1.3/src/HTTP_PyServer.egg-info/
+-rw-rw-rw-   0        0        0     2041 2023-05-05 02:41:15.000000 HTTP-PyServer-0.1.3/src/HTTP_PyServer.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      431 2023-05-05 02:41:15.000000 HTTP-PyServer-0.1.3/src/HTTP_PyServer.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-05 02:41:15.000000 HTTP-PyServer-0.1.3/src/HTTP_PyServer.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2023-05-05 02:41:15.000000 HTTP-PyServer-0.1.3/src/HTTP_PyServer.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-05 02:41:15.714873 HTTP-PyServer-0.1.3/src/server/
+-rw-rw-rw-   0        0        0      369 2023-05-04 03:39:37.000000 HTTP-PyServer-0.1.3/src/server/__init__.py
+-rw-rw-rw-   0        0        0     2497 2023-05-05 02:35:59.000000 HTTP-PyServer-0.1.3/src/server/cache.py
+-rw-rw-rw-   0        0        0     4851 2023-05-05 00:12:16.000000 HTTP-PyServer-0.1.3/src/server/render.py
+-rw-rw-rw-   0        0        0     2358 2023-05-01 16:37:07.000000 HTTP-PyServer-0.1.3/src/server/request.py
+-rw-rw-rw-   0        0        0     2126 2023-05-05 00:12:04.000000 HTTP-PyServer-0.1.3/src/server/response.py
+-rw-rw-rw-   0        0        0     1618 2023-04-29 15:55:19.000000 HTTP-PyServer-0.1.3/src/server/response_codes.py
+-rw-rw-rw-   0        0        0     2430 2023-04-29 15:55:27.000000 HTTP-PyServer-0.1.3/src/server/response_messages.py
+-rw-rw-rw-   0        0        0     5060 2023-05-05 01:54:35.000000 HTTP-PyServer-0.1.3/src/server/routes.py
+-rw-rw-rw-   0        0        0     6923 2023-05-05 01:45:04.000000 HTTP-PyServer-0.1.3/src/server/server.py
+-rw-rw-rw-   0        0        0     1055 2023-05-05 00:01:06.000000 HTTP-PyServer-0.1.3/src/server/template.py
```

### Comparing `HTTP-PyServer-0.1.2/LICENSE` & `HTTP-PyServer-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `HTTP-PyServer-0.1.2/PKG-INFO` & `HTTP-PyServer-0.1.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: HTTP-PyServer
-Version: 0.1.2
+Version: 0.1.3
 Summary: Simple way to make complex HTTP servers with python
 Author-email: Alex-Jando <alexjando2007@outlook.com>
 Project-URL: Homepage, https://github.com/Alex-Jando/HTTP-PyServer
 Project-URL: Bug Tracker, https://github.com/Alex-Jando/HTTP-PyServer/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `HTTP-PyServer-0.1.2/README.md` & `HTTP-PyServer-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `HTTP-PyServer-0.1.2/pyproject.toml` & `HTTP-PyServer-0.1.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "HTTP-PyServer"
-version = "0.1.2"
+version = "0.1.3"
 authors = [
   { name="Alex-Jando", email="alexjando2007@outlook.com" },
 ]
 description = "Simple way to make complex HTTP servers with python"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `HTTP-PyServer-0.1.2/src/HTTP_PyServer.egg-info/PKG-INFO` & `HTTP-PyServer-0.1.3/src/HTTP_PyServer.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: HTTP-PyServer
-Version: 0.1.2
+Version: 0.1.3
 Summary: Simple way to make complex HTTP servers with python
 Author-email: Alex-Jando <alexjando2007@outlook.com>
 Project-URL: Homepage, https://github.com/Alex-Jando/HTTP-PyServer
 Project-URL: Bug Tracker, https://github.com/Alex-Jando/HTTP-PyServer/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `HTTP-PyServer-0.1.2/src/server/cache.py` & `HTTP-PyServer-0.1.3/src/server/cache.py`

 * *Files 22% similar despite different names*

```diff
@@ -13,19 +13,25 @@
         self._items = {}
 
     def add(self,
             item: 'CacheItem') -> None:
         '''Adds an item to the cache.
         If the item already exists, it is overwritten.'''
         
-        item._set_parent(self)
+        item._parent = self
 
-        self._items[item.key] = item.value
+        if self._items.get(item.key):
 
-        item._set_expire()
+            self._items[item.key] = item.value
+
+        else:
+
+            self._items[item.key] = item.value
+
+            item._set_expire()
 
     def remove(self,
                key: str) -> None:
         '''Removes an item from the cache.
         If the item does not exist, nothing happens.'''
         
         try:
@@ -78,20 +84,14 @@
         '''Initializes the cache item class. expire is in seconds.
         If expire is 0, the item never expires.'''
 
         self.key = key
         self.value = value
         self._expire = expire
 
-    def _set_parent(self,
-                    parent: Cache) -> None:
-        '''Sets the parent cache.'''
-
-        self._parent = parent
-
     def _set_expire(self) -> None:
         '''Sets the expiration timer.'''
 
         t = threading.Timer(self._expire,
                             self._parent.remove,
                             args = (self.key,))
```

### Comparing `HTTP-PyServer-0.1.2/src/server/render.py` & `HTTP-PyServer-0.1.3/src/server/render.py`

 * *Files identical despite different names*

### Comparing `HTTP-PyServer-0.1.2/src/server/request.py` & `HTTP-PyServer-0.1.3/src/server/request.py`

 * *Files identical despite different names*

### Comparing `HTTP-PyServer-0.1.2/src/server/response.py` & `HTTP-PyServer-0.1.3/src/server/response.py`

 * *Files identical despite different names*

### Comparing `HTTP-PyServer-0.1.2/src/server/response_codes.py` & `HTTP-PyServer-0.1.3/src/server/response_codes.py`

 * *Files identical despite different names*

### Comparing `HTTP-PyServer-0.1.2/src/server/response_messages.py` & `HTTP-PyServer-0.1.3/src/server/response_messages.py`

 * *Files identical despite different names*

### Comparing `HTTP-PyServer-0.1.2/src/server/routes.py` & `HTTP-PyServer-0.1.3/src/server/routes.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,14 +7,16 @@
 from . import render
 
 class Routes:
     '''Stores, sorts, and handles a collection of routes.'''
 
     def __init__(self) -> None:
 
+        self._root = None
+
         self._routes: dict[str: callable] = {
 
             self._404route: lambda request: render.text('''<!DOCTYPE html>
 
 <html>
 
 <head>
@@ -82,14 +84,24 @@
 
             self._routes[path.rstrip('/')] = route_function
 
             return route_function
         
         return callable_route
     
+    def root(self) -> callable:
+
+        def callable_root(route_function):
+
+            self._root = route_function
+
+            return route_function
+
+        return callable_root
+    
     def _get_wildcard_path(self,
                            path: str,
                            *,
                            request: request.Request) -> bytes:
         '''Gets a route with wildcard values.'''
     
         for route in self._routes:
@@ -141,14 +153,18 @@
 
     def _get_route(self,
                   path: str,
                   *,
                   request: request.Request = request.Request()) -> bytes:
         '''Gets a route from the _routes dictionary.'''
 
+        if self._root:
+
+            self._root(request)
+
         if path in self._routes:
 
             message = self._routes[path](request)
 
             if isinstance(message, str):
 
                 return bytes(render.text(text = message))
```

### Comparing `HTTP-PyServer-0.1.2/src/server/server.py` & `HTTP-PyServer-0.1.3/src/server/server.py`

 * *Files identical despite different names*

### Comparing `HTTP-PyServer-0.1.2/src/server/template.py` & `HTTP-PyServer-0.1.3/src/server/template.py`

 * *Files identical despite different names*

