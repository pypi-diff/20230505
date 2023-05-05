# Comparing `tmp/fastapi_profiler-1.1.0-py3-none-any.whl.zip` & `tmp/fastapi_profiler-1.2.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,10 +1,10 @@
-Zip file size: 4209 bytes, number of entries: 8
+Zip file size: 4374 bytes, number of entries: 8
 -rw-r--r--  2.0 unx       99 b- defN 23-Jan-03 06:17 fastapi_profiler/__init__.py
--rw-r--r--  2.0 unx       51 b- defN 23-Jan-03 06:20 fastapi_profiler/_version.py
--rw-r--r--  2.0 unx     4063 b- defN 23-Jan-03 06:23 fastapi_profiler/profiler.py
--rw-r--r--  2.0 unx     1063 b- defN 23-Jan-03 07:09 fastapi_profiler-1.1.0.dist-info/LICENSE
--rw-r--r--  2.0 unx     1031 b- defN 23-Jan-03 07:09 fastapi_profiler-1.1.0.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jan-03 07:09 fastapi_profiler-1.1.0.dist-info/WHEEL
--rw-r--r--  2.0 unx       17 b- defN 23-Jan-03 07:09 fastapi_profiler-1.1.0.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      682 b- defN 23-Jan-03 07:09 fastapi_profiler-1.1.0.dist-info/RECORD
-8 files, 7098 bytes uncompressed, 3003 bytes compressed:  57.7%
+-rw-r--r--  2.0 unx       51 b- defN 23-May-05 08:05 fastapi_profiler/_version.py
+-rw-r--r--  2.0 unx     5359 b- defN 23-May-05 08:02 fastapi_profiler/profiler.py
+-rw-r--r--  2.0 unx     1063 b- defN 23-May-05 08:09 fastapi_profiler-1.2.0.dist-info/LICENSE
+-rw-r--r--  2.0 unx      981 b- defN 23-May-05 08:09 fastapi_profiler-1.2.0.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-May-05 08:09 fastapi_profiler-1.2.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx       17 b- defN 23-May-05 08:09 fastapi_profiler-1.2.0.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      681 b- defN 23-May-05 08:09 fastapi_profiler-1.2.0.dist-info/RECORD
+8 files, 8343 bytes uncompressed, 3168 bytes compressed:  62.0%
```

## zipnote {}

```diff
@@ -3,23 +3,23 @@
 
 Filename: fastapi_profiler/_version.py
 Comment: 
 
 Filename: fastapi_profiler/profiler.py
 Comment: 
 
-Filename: fastapi_profiler-1.1.0.dist-info/LICENSE
+Filename: fastapi_profiler-1.2.0.dist-info/LICENSE
 Comment: 
 
-Filename: fastapi_profiler-1.1.0.dist-info/METADATA
+Filename: fastapi_profiler-1.2.0.dist-info/METADATA
 Comment: 
 
-Filename: fastapi_profiler-1.1.0.dist-info/WHEEL
+Filename: fastapi_profiler-1.2.0.dist-info/WHEEL
 Comment: 
 
-Filename: fastapi_profiler-1.1.0.dist-info/top_level.txt
+Filename: fastapi_profiler-1.2.0.dist-info/top_level.txt
 Comment: 
 
-Filename: fastapi_profiler-1.1.0.dist-info/RECORD
+Filename: fastapi_profiler-1.2.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## fastapi_profiler/_version.py

```diff
@@ -1,2 +1,2 @@
-__version__ = "1.1.0"
+__version__ = "1.2.0"
 __author__ = "sunhailin-Leo"
```

## fastapi_profiler/profiler.py

```diff
@@ -1,10 +1,12 @@
 import os
 import time
 import codecs
+import cProfile
+from io import StringIO
 from typing import Optional
 from logging import getLogger
 
 from pyinstrument import Profiler
 from pyinstrument.renderers import HTMLRenderer
 
 from starlette.routing import Router
@@ -13,79 +15,99 @@
 
 
 logger = getLogger("profiler")
 
 
 class PyInstrumentProfilerMiddleware:
     DEFAULT_HTML_FILENAME = "./fastapi-profiler.html"
+    DEFAULT_PROF_FILENAME = "./fastapi-profiler.prof"
 
     def __init__(
-        self, app: ASGIApp,
+        self,
+        app: ASGIApp,
         *,
         server_app: Optional[Router] = None,
         profiler_interval: float = 0.0001,
         profiler_output_type: str = "text",
         is_print_each_request: bool = True,
         async_mode: str = "enabled",
         html_file_name: Optional[str] = None,
+        prof_file_name: Optional[str] = None,
         open_in_browser: bool = False,
-        **profiler_kwargs
+        **profiler_kwargs,
     ):
         self.app = app
-        self._profiler = Profiler(interval=profiler_interval, async_mode=async_mode)
         self._output_type = profiler_output_type
         self._print_each_request = is_print_each_request
         self._html_file_name: Optional[str] = html_file_name
+        self._prof_file_name: Optional[str] = prof_file_name
         self._open_in_browser: bool = open_in_browser
         self._profiler_kwargs: dict = profiler_kwargs
 
         if profiler_output_type == "html" and server_app is None:
             raise RuntimeError(
                 "If profiler_output_type=html, must provide server_app argument "
                 "to set shutdown event handler to output profile."
             )
 
+        if profiler_output_type == "prof":
+            self._profiler = cProfile.Profile()
+            self._start_profiler = self._profiler.enable
+            self._stop_profiler = self._profiler.disable
+        else:
+            self._profiler = Profiler(interval=profiler_interval, async_mode=async_mode)
+            self._start_profiler = self._profiler.start
+            self._stop_profiler = self._profiler.stop
+
         # register an event handler for profiler stop
         if server_app is not None:
             server_app.add_event_handler("shutdown", self.get_profiler_result)
 
     async def __call__(self, scope: Scope, receive: Receive, send: Send) -> None:
         if scope["type"] != "http":
             await self.app(scope, receive, send)
             return
 
-        self._profiler.start()
+        self._start_profiler()
 
         request = Request(scope, receive=receive)
         method = request.method
         path = request.url.path
         begin = time.perf_counter()
 
         # Default status code used when the application does not return a valid response
         # or an unhandled exception occurs.
         status_code = 500
 
         async def wrapped_send(message: Message) -> None:
-            if message['type'] == 'http.response.start':
+            if message["type"] == "http.response.start":
                 nonlocal status_code
-                status_code = message['status']
+                status_code = message["status"]
             await send(message)
 
         try:
             await self.app(scope, receive, wrapped_send)
         finally:
             if scope["type"] == "http":
-                self._profiler.stop()
+                self._stop_profiler()
                 end = time.perf_counter()
                 if self._print_each_request:
-                    print(f"Method: {method}, "
-                          f"Path: {path}, "
-                          f"Duration: {end - begin}, "
-                          f"Status: {status_code}")
-                    print(self._profiler.output_text(**self._profiler_kwargs))
+                    print(
+                        f"Method: {method}, "
+                        f"Path: {path}, "
+                        f"Duration: {end - begin}, "
+                        f"Status: {status_code}"
+                    )
+
+                    if self._output_type == "prof":
+                        s = StringIO()
+                        self._profiler.print_stats(stream=s)
+                        print(s.getvalue())
+                    else:
+                        print(self._profiler.output_text(**self._profiler_kwargs))
 
     async def get_profiler_result(self):
         if self._output_type == "text":
             logger.info("Compiling and printing final profile")
             print(self._profiler.output_text(**self._profiler_kwargs))
         elif self._output_type == "html":
             html_file_name = self.DEFAULT_HTML_FILENAME
@@ -105,7 +127,19 @@
                 )
             else:
                 html_code = renderer.render(session=self._profiler.last_session)
                 with codecs.open(html_file_name, "w", "utf-8") as f:
                     f.write(html_code)
 
             logger.info("Done writing profile to %r", html_file_name)
+        elif self._output_type == "prof":
+            prof_file_name = self.DEFAULT_PROF_FILENAME
+            if self._prof_file_name is not None:
+                prof_file_name = self._prof_file_name
+
+            logger.info(
+                "Compiling and dumping final profile to %r - this may take some time",
+                prof_file_name,
+            )
+
+            self._profiler.dump_stats(prof_file_name)
+            logger.info("Done writing profile to %r", prof_file_name)
```

## Comparing `fastapi_profiler-1.1.0.dist-info/LICENSE` & `fastapi_profiler-1.2.0.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `fastapi_profiler-1.1.0.dist-info/METADATA` & `fastapi_profiler-1.2.0.dist-info/METADATA`

 * *Files 5% similar despite different names*

```diff
@@ -1,24 +1,23 @@
 Metadata-Version: 2.1
 Name: fastapi-profiler
-Version: 1.1.0
+Version: 1.2.0
 Summary: A FastAPI Middleware of pyinstrument to check your service performance.
 Home-page: https://github.com/sunhailin-Leo/fastapi_profiler
 Author: sunhailin-Leo
 Author-email: 379978424@qq.com
 License: MIT
 Keywords: fastapi,pyinstrument,profiler
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development :: Libraries
 Requires-Dist: fastapi
```

