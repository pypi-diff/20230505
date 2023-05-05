# Comparing `tmp/HTTP-PyServer-0.1.1.tar.gz` & `tmp/HTTP-PyServer-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "HTTP-PyServer-0.1.1.tar", last modified: Wed May  3 19:43:56 2023, max compression
+gzip compressed data, was "HTTP-PyServer-0.1.2.tar", last modified: Fri May  5 00:29:02 2023, max compression
```

## Comparing `HTTP-PyServer-0.1.1.tar` & `HTTP-PyServer-0.1.2.tar`

### file list

```diff
@@ -1,21 +1,23 @@
-drwxrwxrwx   0        0        0        0 2023-05-03 19:43:56.364440 HTTP-PyServer-0.1.1/
--rw-rw-rw-   0        0        0     1067 2023-04-12 19:57:31.000000 HTTP-PyServer-0.1.1/LICENSE
--rw-rw-rw-   0        0        0     2033 2023-05-03 19:43:56.363441 HTTP-PyServer-0.1.1/PKG-INFO
--rw-rw-rw-   0        0        0     1470 2023-05-03 19:36:27.000000 HTTP-PyServer-0.1.1/README.md
--rw-rw-rw-   0        0        0      641 2023-05-03 19:43:16.000000 HTTP-PyServer-0.1.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-03 19:43:56.365436 HTTP-PyServer-0.1.1/setup.cfg
-drwxrwxrwx   0        0        0        0 2023-05-03 19:43:56.212844 HTTP-PyServer-0.1.1/src/
-drwxrwxrwx   0        0        0        0 2023-05-03 19:43:56.271686 HTTP-PyServer-0.1.1/src/HTTP_PyServer.egg-info/
--rw-rw-rw-   0        0        0     2033 2023-05-03 19:43:56.000000 HTTP-PyServer-0.1.1/src/HTTP_PyServer.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      388 2023-05-03 19:43:56.000000 HTTP-PyServer-0.1.1/src/HTTP_PyServer.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-03 19:43:56.000000 HTTP-PyServer-0.1.1/src/HTTP_PyServer.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2023-05-03 19:43:56.000000 HTTP-PyServer-0.1.1/src/HTTP_PyServer.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-05-03 19:43:56.358461 HTTP-PyServer-0.1.1/src/server/
--rw-rw-rw-   0        0        0      318 2023-05-01 16:28:05.000000 HTTP-PyServer-0.1.1/src/server/__init__.py
--rw-rw-rw-   0        0        0     5374 2023-05-03 19:35:13.000000 HTTP-PyServer-0.1.1/src/server/render.py
--rw-rw-rw-   0        0        0     2358 2023-05-01 16:37:07.000000 HTTP-PyServer-0.1.1/src/server/request.py
--rw-rw-rw-   0        0        0     2122 2023-05-01 16:34:09.000000 HTTP-PyServer-0.1.1/src/server/response.py
--rw-rw-rw-   0        0        0     1618 2023-04-29 15:55:19.000000 HTTP-PyServer-0.1.1/src/server/response_codes.py
--rw-rw-rw-   0        0        0     2430 2023-04-29 15:55:27.000000 HTTP-PyServer-0.1.1/src/server/response_messages.py
--rw-rw-rw-   0        0        0     4773 2023-05-03 19:35:25.000000 HTTP-PyServer-0.1.1/src/server/routes.py
--rw-rw-rw-   0        0        0     6872 2023-05-03 19:25:21.000000 HTTP-PyServer-0.1.1/src/server/server.py
+drwxrwxrwx   0        0        0        0 2023-05-05 00:29:02.361660 HTTP-PyServer-0.1.2/
+-rw-rw-rw-   0        0        0     1067 2023-04-12 19:57:31.000000 HTTP-PyServer-0.1.2/LICENSE
+-rw-rw-rw-   0        0        0     2041 2023-05-05 00:29:02.359375 HTTP-PyServer-0.1.2/PKG-INFO
+-rw-rw-rw-   0        0        0     1478 2023-05-05 00:20:57.000000 HTTP-PyServer-0.1.2/README.md
+-rw-rw-rw-   0        0        0      641 2023-05-05 00:28:32.000000 HTTP-PyServer-0.1.2/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-05 00:29:02.361660 HTTP-PyServer-0.1.2/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-05 00:29:02.300325 HTTP-PyServer-0.1.2/src/
+drwxrwxrwx   0        0        0        0 2023-05-05 00:29:02.320391 HTTP-PyServer-0.1.2/src/HTTP_PyServer.egg-info/
+-rw-rw-rw-   0        0        0     2041 2023-05-05 00:29:02.000000 HTTP-PyServer-0.1.2/src/HTTP_PyServer.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      431 2023-05-05 00:29:02.000000 HTTP-PyServer-0.1.2/src/HTTP_PyServer.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-05 00:29:02.000000 HTTP-PyServer-0.1.2/src/HTTP_PyServer.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2023-05-05 00:29:02.000000 HTTP-PyServer-0.1.2/src/HTTP_PyServer.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-05 00:29:02.354280 HTTP-PyServer-0.1.2/src/server/
+-rw-rw-rw-   0        0        0      369 2023-05-04 03:39:37.000000 HTTP-PyServer-0.1.2/src/server/__init__.py
+-rw-rw-rw-   0        0        0     2529 2023-05-05 00:15:15.000000 HTTP-PyServer-0.1.2/src/server/cache.py
+-rw-rw-rw-   0        0        0     4851 2023-05-05 00:12:16.000000 HTTP-PyServer-0.1.2/src/server/render.py
+-rw-rw-rw-   0        0        0     2358 2023-05-01 16:37:07.000000 HTTP-PyServer-0.1.2/src/server/request.py
+-rw-rw-rw-   0        0        0     2126 2023-05-05 00:12:04.000000 HTTP-PyServer-0.1.2/src/server/response.py
+-rw-rw-rw-   0        0        0     1618 2023-04-29 15:55:19.000000 HTTP-PyServer-0.1.2/src/server/response_codes.py
+-rw-rw-rw-   0        0        0     2430 2023-04-29 15:55:27.000000 HTTP-PyServer-0.1.2/src/server/response_messages.py
+-rw-rw-rw-   0        0        0     4773 2023-05-03 19:35:25.000000 HTTP-PyServer-0.1.2/src/server/routes.py
+-rw-rw-rw-   0        0        0     6923 2023-05-04 23:56:20.000000 HTTP-PyServer-0.1.2/src/server/server.py
+-rw-rw-rw-   0        0        0     1055 2023-05-05 00:01:06.000000 HTTP-PyServer-0.1.2/src/server/template.py
```

### Comparing `HTTP-PyServer-0.1.1/LICENSE` & `HTTP-PyServer-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `HTTP-PyServer-0.1.1/PKG-INFO` & `HTTP-PyServer-0.1.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: HTTP-PyServer
-Version: 0.1.1
+Version: 0.1.2
 Summary: Simple way to make complex HTTP servers with python
 Author-email: Alex-Jando <alexjando2007@outlook.com>
 Project-URL: Homepage, https://github.com/Alex-Jando/HTTP-PyServer
 Project-URL: Bug Tracker, https://github.com/Alex-Jando/HTTP-PyServer/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -59,12 +59,13 @@
 Although, no external packages were used, the following packages were imported. All packages are native in `Python 3.11.2`. Not tested on any other versions, however it should work.
 
 - `threading`
 - `socket`
 - `typing`
 - `logging`
 - `pathlib`
+- `re`
 - `json`
 - `urllib`
 - `mimetypes`
 - `enum`
 - `ssl`
```

### Comparing `HTTP-PyServer-0.1.1/README.md` & `HTTP-PyServer-0.1.2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -45,12 +45,13 @@
 Although, no external packages were used, the following packages were imported. All packages are native in `Python 3.11.2`. Not tested on any other versions, however it should work.
 
 - `threading`
 - `socket`
 - `typing`
 - `logging`
 - `pathlib`
+- `re`
 - `json`
 - `urllib`
 - `mimetypes`
 - `enum`
 - `ssl`
```

### Comparing `HTTP-PyServer-0.1.1/pyproject.toml` & `HTTP-PyServer-0.1.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "HTTP-PyServer"
-version = "0.1.1"
+version = "0.1.2"
 authors = [
   { name="Alex-Jando", email="alexjando2007@outlook.com" },
 ]
 description = "Simple way to make complex HTTP servers with python"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `HTTP-PyServer-0.1.1/src/HTTP_PyServer.egg-info/PKG-INFO` & `HTTP-PyServer-0.1.2/src/HTTP_PyServer.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: HTTP-PyServer
-Version: 0.1.1
+Version: 0.1.2
 Summary: Simple way to make complex HTTP servers with python
 Author-email: Alex-Jando <alexjando2007@outlook.com>
 Project-URL: Homepage, https://github.com/Alex-Jando/HTTP-PyServer
 Project-URL: Bug Tracker, https://github.com/Alex-Jando/HTTP-PyServer/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -59,12 +59,13 @@
 Although, no external packages were used, the following packages were imported. All packages are native in `Python 3.11.2`. Not tested on any other versions, however it should work.
 
 - `threading`
 - `socket`
 - `typing`
 - `logging`
 - `pathlib`
+- `re`
 - `json`
 - `urllib`
 - `mimetypes`
 - `enum`
 - `ssl`
```

### Comparing `HTTP-PyServer-0.1.1/src/server/render.py` & `HTTP-PyServer-0.1.2/src/server/render.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,28 +1,14 @@
 import mimetypes
 import pathlib
 
 from . import response_codes
 from . import response
 from . import response_messages
-
-def _get_template(data: bytes,
-                  **template_vars) -> str:
-    '''Replaces all template variables in a data with their values.
-    Template variables are defined as {{var_name}},
-    and are replaced with the value of var_name in template_vars.'''
-    
-    for var_name, var_value in template_vars.items():
-
-        data = data.replace(f'{{{{{var_name}}}}}'.encode(encoding = 'utf-8',
-                                                         errors = 'ignore'),
-                            var_value.encode(encoding = 'utf-8',
-                                             errors = 'ignore'))
-
-    return data
+from . import template
 
 def text(text: str,
          *,
          filetype: str = 'txt',
          code: int | response_codes.ResponseCodes = 200,
          message: str | response_messages.ResponseMessages = 'OK',
          headers: dict = None) -> response.Response:
@@ -52,19 +38,19 @@
                              code = code,
                              message = message,
                              headers = headers,
                              body = text)
 
 def file(filepath: str,
          *,
-         templated_vars: dict = {},
          code: int | response_codes.ResponseCodes = 200,
          message: str | response_messages.ResponseMessages = 'OK',
-         headers: dict = None
-         ) -> response.Response:
+         headers: dict = None,
+         is_template: bool = False,
+         **templated_values) -> response.Response:
     '''Returns a file as a response. Use this to return HTML, CSS, JS, images, etc.'''
 
     if not headers:
 
         headers = {}
 
     if type(code) == response_codes.ResponseCodes:
@@ -81,41 +67,46 @@
             
     else:
 
         with open(filepath, 'rb') as file:
 
             data = file.read()
 
-    if templated_vars:
+    if is_template:
+
+        if not templated_values:
+
+            templated_values = {}
+
+        if isinstance(data, bytes):
+
+            data = data.decode(encoding = 'utf-8',
+                               errors = 'ignore')
 
-        data = _get_template(data = data,
-                             **templated_vars)
+        data = template._template(data = data,
+                                  **templated_values)
 
     headers['Content-Length'] = str(len(data))
     headers['Content-Type'] = mimetypes.guess_type(filepath)[0]\
                               or 'application/octet-stream'
 
     return response.Response(version = 1.1,
                              code = code,
                              message = message,
                              headers = headers,
                              body = data)
 
 def redirect(url: str) -> response.Response:
     '''Returns a redirect request to the specified URL.'''
 
-    redirect_request = f'HTTP/1.1 301 See Other\
-        \r\nLocation: {url}\
-        \r\nContent-Type: text/html\
-        \r\n\r\n\
-        <html>\
-            <head>\
-                <meta http-equiv="refresh" content="0;URL={url}" />\
-            </head>\
-        </html>'
+    redirect_request = f'''<html>
+    <head>
+        <meta http-equiv="refresh" content="0;URL={url}" />
+    </head>
+</html>'''
 
     return response.Response(version = 1.1,
                              code = response_codes.ResponseCodes.SEE_OTHER,
                              message = response_messages.ResponseMessages.SEE_OTHER,
                              headers = {'Location': url,
                                         'Content-Type': 'text/html',
                                         'Content-Length': str(len(redirect_request))},
```

### Comparing `HTTP-PyServer-0.1.1/src/server/request.py` & `HTTP-PyServer-0.1.2/src/server/request.py`

 * *Files identical despite different names*

### Comparing `HTTP-PyServer-0.1.1/src/server/response.py` & `HTTP-PyServer-0.1.2/src/server/response.py`

 * *Files 1% similar despite different names*

```diff
@@ -33,26 +33,26 @@
     def __str__(self):
         '''Returns the response as a string.
         This is not a valid HTTP response as the body is not encoded.'''
 
         return f'HTTP/{self.version} {self.code} {self.message}\r\n' \
 + '\r\n'.join([f'{key}: {value}' for key, value in self.headers.items()]) \
 + '\r\n\r\n' \
-+ self.body if isinstance(self.body, str) else self.body.decode(encoding = 'utf-8',
-                                                                errors = 'ignore')
++ (self.body if isinstance(self.body, str) else self.body.decode(encoding = 'utf-8',
+                                                                errors = 'ignore'))
 
     def __bytes__(self):
         '''Returns the response as a bytes object. This is a valid HTTP response.'''
 
         return (f'HTTP/{self.version} {self.code} {self.message}\r\n'\
 + '\r\n'.join([f'{key}: {value}' for key, value in self.headers.items()]) + '\r\n\r\n')\
 .encode(encoding = 'utf-8',
         errors = 'ignore')\
-+ self.body if isinstance(self.body, bytes) else self.body.encode(encoding = 'utf-8',
-                                                                  errors = 'ignore')
++ (self.body if isinstance(self.body, bytes) else self.body.encode(encoding = 'utf-8',
+                                                                  errors = 'ignore'))
     
     def __repr__(self):
         '''Returns representation of the response as a string.'''
 
         return f'<Response(version = {self.version}, \
 code = {self.code}, \
 message = {self.message})>'
```

### Comparing `HTTP-PyServer-0.1.1/src/server/response_codes.py` & `HTTP-PyServer-0.1.2/src/server/response_codes.py`

 * *Files identical despite different names*

### Comparing `HTTP-PyServer-0.1.1/src/server/response_messages.py` & `HTTP-PyServer-0.1.2/src/server/response_messages.py`

 * *Files identical despite different names*

### Comparing `HTTP-PyServer-0.1.1/src/server/routes.py` & `HTTP-PyServer-0.1.2/src/server/routes.py`

 * *Files identical despite different names*

### Comparing `HTTP-PyServer-0.1.1/src/server/server.py` & `HTTP-PyServer-0.1.2/src/server/server.py`

 * *Files 3% similar despite different names*

```diff
@@ -14,15 +14,15 @@
     def __init__(self,
                  *,
                  host: str = '127.0.0.1',
                  port: int = 80,
                  logger: logging.Logger = None,
                  _404route: str = '/404',
                  _500route: str = '/500',
-                 static_dir: str = '/static/',
+                 static_dir: str = 'static/',
                  ssl_context: ssl.SSLContext = None) -> None:
         '''Initializes the server class.'''
         
         self._host: str = host
 
         self._port: int = port
 
@@ -32,15 +32,17 @@
 
         self._500route: str = _500route
 
         self._static_dir: pathlib.Path = pathlib.Path(static_dir.strip('/'))
 
         if not self._static_dir.exists():
 
-            self._logger.warning('Static directory does not exist.')
+            if self._logger:
+
+                self._logger.warning(f'Static directory "{static_dir}" does not exist.')
 
         self._ssl_context: ssl.SSLContext = ssl_context
 
         super().__init__()
 
     def start(self) -> None:
         '''Starts the server.'''
```

