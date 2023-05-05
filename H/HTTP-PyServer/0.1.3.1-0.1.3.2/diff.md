# Comparing `tmp/HTTP-PyServer-0.1.3.1.tar.gz` & `tmp/HTTP-PyServer-0.1.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "HTTP-PyServer-0.1.3.1.tar", last modified: Fri May  5 03:25:58 2023, max compression
+gzip compressed data, was "HTTP-PyServer-0.1.3.2.tar", last modified: Fri May  5 16:46:06 2023, max compression
```

## Comparing `HTTP-PyServer-0.1.3.1.tar` & `HTTP-PyServer-0.1.3.2.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0        0        0        0 2023-05-05 03:25:58.253263 HTTP-PyServer-0.1.3.1/
--rw-rw-rw-   0        0        0     1067 2023-04-12 19:57:31.000000 HTTP-PyServer-0.1.3.1/LICENSE
--rw-rw-rw-   0        0        0     2043 2023-05-05 03:25:58.252519 HTTP-PyServer-0.1.3.1/PKG-INFO
--rw-rw-rw-   0        0        0     1478 2023-05-05 00:20:57.000000 HTTP-PyServer-0.1.3.1/README.md
--rw-rw-rw-   0        0        0      643 2023-05-05 03:16:12.000000 HTTP-PyServer-0.1.3.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-05 03:25:58.253263 HTTP-PyServer-0.1.3.1/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-05-05 03:25:58.206598 HTTP-PyServer-0.1.3.1/src/
-drwxrwxrwx   0        0        0        0 2023-05-05 03:25:58.223211 HTTP-PyServer-0.1.3.1/src/HTTP_PyServer.egg-info/
--rw-rw-rw-   0        0        0     2043 2023-05-05 03:25:58.000000 HTTP-PyServer-0.1.3.1/src/HTTP_PyServer.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      431 2023-05-05 03:25:58.000000 HTTP-PyServer-0.1.3.1/src/HTTP_PyServer.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-05 03:25:58.000000 HTTP-PyServer-0.1.3.1/src/HTTP_PyServer.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2023-05-05 03:25:58.000000 HTTP-PyServer-0.1.3.1/src/HTTP_PyServer.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-05-05 03:25:58.249776 HTTP-PyServer-0.1.3.1/src/server/
--rw-rw-rw-   0        0        0      369 2023-05-04 03:39:37.000000 HTTP-PyServer-0.1.3.1/src/server/__init__.py
--rw-rw-rw-   0        0        0     2762 2023-05-05 03:22:33.000000 HTTP-PyServer-0.1.3.1/src/server/cache.py
--rw-rw-rw-   0        0        0     4851 2023-05-05 00:12:16.000000 HTTP-PyServer-0.1.3.1/src/server/render.py
--rw-rw-rw-   0        0        0     2358 2023-05-01 16:37:07.000000 HTTP-PyServer-0.1.3.1/src/server/request.py
--rw-rw-rw-   0        0        0     2126 2023-05-05 00:12:04.000000 HTTP-PyServer-0.1.3.1/src/server/response.py
--rw-rw-rw-   0        0        0     1618 2023-04-29 15:55:19.000000 HTTP-PyServer-0.1.3.1/src/server/response_codes.py
--rw-rw-rw-   0        0        0     2430 2023-04-29 15:55:27.000000 HTTP-PyServer-0.1.3.1/src/server/response_messages.py
--rw-rw-rw-   0        0        0     5060 2023-05-05 01:54:35.000000 HTTP-PyServer-0.1.3.1/src/server/routes.py
--rw-rw-rw-   0        0        0     6923 2023-05-05 01:45:04.000000 HTTP-PyServer-0.1.3.1/src/server/server.py
--rw-rw-rw-   0        0        0     1055 2023-05-05 00:01:06.000000 HTTP-PyServer-0.1.3.1/src/server/template.py
+drwxrwxrwx   0        0        0        0 2023-05-05 16:46:06.887152 HTTP-PyServer-0.1.3.2/
+-rw-rw-rw-   0        0        0     1067 2023-04-12 19:57:31.000000 HTTP-PyServer-0.1.3.2/LICENSE
+-rw-rw-rw-   0        0        0     2043 2023-05-05 16:46:06.883416 HTTP-PyServer-0.1.3.2/PKG-INFO
+-rw-rw-rw-   0        0        0     1478 2023-05-05 00:20:57.000000 HTTP-PyServer-0.1.3.2/README.md
+-rw-rw-rw-   0        0        0      643 2023-05-05 16:43:56.000000 HTTP-PyServer-0.1.3.2/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-05 16:46:06.887689 HTTP-PyServer-0.1.3.2/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-05 16:46:06.781257 HTTP-PyServer-0.1.3.2/src/
+drwxrwxrwx   0        0        0        0 2023-05-05 16:46:06.817711 HTTP-PyServer-0.1.3.2/src/HTTP_PyServer.egg-info/
+-rw-rw-rw-   0        0        0     2043 2023-05-05 16:46:06.000000 HTTP-PyServer-0.1.3.2/src/HTTP_PyServer.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      431 2023-05-05 16:46:06.000000 HTTP-PyServer-0.1.3.2/src/HTTP_PyServer.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-05 16:46:06.000000 HTTP-PyServer-0.1.3.2/src/HTTP_PyServer.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2023-05-05 16:46:06.000000 HTTP-PyServer-0.1.3.2/src/HTTP_PyServer.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-05 16:46:06.876435 HTTP-PyServer-0.1.3.2/src/server/
+-rw-rw-rw-   0        0        0      369 2023-05-04 03:39:37.000000 HTTP-PyServer-0.1.3.2/src/server/__init__.py
+-rw-rw-rw-   0        0        0     2762 2023-05-05 03:22:33.000000 HTTP-PyServer-0.1.3.2/src/server/cache.py
+-rw-rw-rw-   0        0        0     4851 2023-05-05 00:12:16.000000 HTTP-PyServer-0.1.3.2/src/server/render.py
+-rw-rw-rw-   0        0        0     2778 2023-05-05 16:43:20.000000 HTTP-PyServer-0.1.3.2/src/server/request.py
+-rw-rw-rw-   0        0        0     2126 2023-05-05 00:12:04.000000 HTTP-PyServer-0.1.3.2/src/server/response.py
+-rw-rw-rw-   0        0        0     1618 2023-04-29 15:55:19.000000 HTTP-PyServer-0.1.3.2/src/server/response_codes.py
+-rw-rw-rw-   0        0        0     2430 2023-04-29 15:55:27.000000 HTTP-PyServer-0.1.3.2/src/server/response_messages.py
+-rw-rw-rw-   0        0        0     5060 2023-05-05 01:54:35.000000 HTTP-PyServer-0.1.3.2/src/server/routes.py
+-rw-rw-rw-   0        0        0     6923 2023-05-05 01:45:04.000000 HTTP-PyServer-0.1.3.2/src/server/server.py
+-rw-rw-rw-   0        0        0     1055 2023-05-05 00:01:06.000000 HTTP-PyServer-0.1.3.2/src/server/template.py
```

### Comparing `HTTP-PyServer-0.1.3.1/LICENSE` & `HTTP-PyServer-0.1.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `HTTP-PyServer-0.1.3.1/PKG-INFO` & `HTTP-PyServer-0.1.3.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: HTTP-PyServer
-Version: 0.1.3.1
+Version: 0.1.3.2
 Summary: Simple way to make complex HTTP servers with python
 Author-email: Alex-Jando <alexjando2007@outlook.com>
 Project-URL: Homepage, https://github.com/Alex-Jando/HTTP-PyServer
 Project-URL: Bug Tracker, https://github.com/Alex-Jando/HTTP-PyServer/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `HTTP-PyServer-0.1.3.1/README.md` & `HTTP-PyServer-0.1.3.2/README.md`

 * *Files identical despite different names*

### Comparing `HTTP-PyServer-0.1.3.1/pyproject.toml` & `HTTP-PyServer-0.1.3.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "HTTP-PyServer"
-version = "0.1.3.1"
+version = "0.1.3.2"
 authors = [
   { name="Alex-Jando", email="alexjando2007@outlook.com" },
 ]
 description = "Simple way to make complex HTTP servers with python"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `HTTP-PyServer-0.1.3.1/src/HTTP_PyServer.egg-info/PKG-INFO` & `HTTP-PyServer-0.1.3.2/src/HTTP_PyServer.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: HTTP-PyServer
-Version: 0.1.3.1
+Version: 0.1.3.2
 Summary: Simple way to make complex HTTP servers with python
 Author-email: Alex-Jando <alexjando2007@outlook.com>
 Project-URL: Homepage, https://github.com/Alex-Jando/HTTP-PyServer
 Project-URL: Bug Tracker, https://github.com/Alex-Jando/HTTP-PyServer/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `HTTP-PyServer-0.1.3.1/src/server/cache.py` & `HTTP-PyServer-0.1.3.2/src/server/cache.py`

 * *Files identical despite different names*

### Comparing `HTTP-PyServer-0.1.3.1/src/server/render.py` & `HTTP-PyServer-0.1.3.2/src/server/render.py`

 * *Files identical despite different names*

### Comparing `HTTP-PyServer-0.1.3.1/src/server/request.py` & `HTTP-PyServer-0.1.3.2/src/server/request.py`

 * *Files 6% similar despite different names*

```diff
@@ -84,14 +84,33 @@
         '''Returns the request as an HTTP request string.'''
 
         return f'{self.method} {self.path} {self.version}\r\n' + \
 '\r\n'.join([f'{key}: {value}' for key, value in self.headers.items()]) + \
 '\r\n\r\n' + \
 self.body
 
+    def cookies(self):
+        '''Returns the request cookies as a dictionary.'''
+
+        try:
+
+            cookies = {}
+
+            for cookie in self.headers.get('Cookie').split(';'):
+
+                key, value = list(urllib.parse.parse_qs(cookie.strip()).items())[0]
+
+                cookies[key] = value[0]
+
+            return cookies
+        
+        except Exception:
+
+            return {}
+
     def json(self):
         '''Returns the request body as a JSON object.'''
 
         return json.loads(self.body)
     
     def form(self):
         '''Returns the request body as parsed urlencoded form data.'''
```

### Comparing `HTTP-PyServer-0.1.3.1/src/server/response.py` & `HTTP-PyServer-0.1.3.2/src/server/response.py`

 * *Files identical despite different names*

### Comparing `HTTP-PyServer-0.1.3.1/src/server/response_codes.py` & `HTTP-PyServer-0.1.3.2/src/server/response_codes.py`

 * *Files identical despite different names*

### Comparing `HTTP-PyServer-0.1.3.1/src/server/response_messages.py` & `HTTP-PyServer-0.1.3.2/src/server/response_messages.py`

 * *Files identical despite different names*

### Comparing `HTTP-PyServer-0.1.3.1/src/server/routes.py` & `HTTP-PyServer-0.1.3.2/src/server/routes.py`

 * *Files identical despite different names*

### Comparing `HTTP-PyServer-0.1.3.1/src/server/server.py` & `HTTP-PyServer-0.1.3.2/src/server/server.py`

 * *Files identical despite different names*

### Comparing `HTTP-PyServer-0.1.3.1/src/server/template.py` & `HTTP-PyServer-0.1.3.2/src/server/template.py`

 * *Files identical despite different names*

