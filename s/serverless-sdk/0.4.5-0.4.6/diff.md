# Comparing `tmp/serverless-sdk-0.4.5.tar.gz` & `tmp/serverless-sdk-0.4.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/console/console/python/packages/sdk/dist/.tmp-m7ky189x/serverless-sdk-0.4.5.tar", last modified: Wed Apr 26 15:20:43 2023, max compression
+gzip compressed data, was "/home/runner/work/console/console/python/packages/sdk/dist/.tmp-tii8obn0/serverless-sdk-0.4.6.tar", last modified: Fri May  5 17:09:37 2023, max compression
```

## Comparing `serverless-sdk-0.4.5.tar` & `serverless-sdk-0.4.6.tar`

### file list

```diff
@@ -1,41 +1,44 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 15:20:43.000000 serverless-sdk-0.4.5/
--rw-r--r--   0 runner    (1001) docker     (123)     2878 2023-04-26 15:20:43.000000 serverless-sdk-0.4.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2355 2023-04-26 15:20:16.000000 serverless-sdk-0.4.5/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1292 2023-04-26 15:20:16.000000 serverless-sdk-0.4.5/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 15:20:43.000000 serverless-sdk-0.4.5/serverless_sdk/
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-04-26 15:20:16.000000 serverless-sdk-0.4.5/serverless_sdk/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 15:20:43.000000 serverless-sdk-0.4.5/serverless_sdk.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2878 2023-04-26 15:20:43.000000 serverless-sdk-0.4.5/serverless_sdk.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      875 2023-04-26 15:20:43.000000 serverless-sdk-0.4.5/serverless_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-26 15:20:43.000000 serverless-sdk-0.4.5/serverless_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      270 2023-04-26 15:20:43.000000 serverless-sdk-0.4.5/serverless_sdk.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-26 15:20:43.000000 serverless-sdk-0.4.5/serverless_sdk.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-26 15:20:43.000000 serverless-sdk-0.4.5/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 15:20:43.000000 serverless-sdk-0.4.5/sls_sdk/
--rw-r--r--   0 runner    (1001) docker     (123)     5520 2023-04-26 15:20:16.000000 serverless-sdk-0.4.5/sls_sdk/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      482 2023-04-26 15:20:16.000000 serverless-sdk-0.4.5/sls_sdk/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      770 2023-04-26 15:20:16.000000 serverless-sdk-0.4.5/sls_sdk/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 15:20:43.000000 serverless-sdk-0.4.5/sls_sdk/lib/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-26 15:20:16.000000 serverless-sdk-0.4.5/sls_sdk/lib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2583 2023-04-26 15:20:16.000000 serverless-sdk-0.4.5/sls_sdk/lib/captured_event.py
--rw-r--r--   0 runner    (1001) docker     (123)      596 2023-04-26 15:20:16.000000 serverless-sdk-0.4.5/sls_sdk/lib/emitter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1430 2023-04-26 15:20:16.000000 serverless-sdk-0.4.5/sls_sdk/lib/error.py
--rw-r--r--   0 runner    (1001) docker     (123)     1919 2023-04-26 15:20:16.000000 serverless-sdk-0.4.5/sls_sdk/lib/error_captured_event.py
--rw-r--r--   0 runner    (1001) docker     (123)      326 2023-04-26 15:20:16.000000 serverless-sdk-0.4.5/sls_sdk/lib/id.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 15:20:43.000000 serverless-sdk-0.4.5/sls_sdk/lib/instrumentation/
--rw-r--r--   0 runner    (1001) docker     (123)     5559 2023-04-26 15:20:16.000000 serverless-sdk-0.4.5/sls_sdk/lib/instrumentation/flask.py
--rw-r--r--   0 runner    (1001) docker     (123)    16272 2023-04-26 15:20:16.000000 serverless-sdk-0.4.5/sls_sdk/lib/instrumentation/http.py
--rw-r--r--   0 runner    (1001) docker     (123)     2023 2023-04-26 15:20:16.000000 serverless-sdk-0.4.5/sls_sdk/lib/instrumentation/import_hook.py
--rw-r--r--   0 runner    (1001) docker     (123)     2321 2023-04-26 15:20:16.000000 serverless-sdk-0.4.5/sls_sdk/lib/instrumentation/logging.py
--rw-r--r--   0 runner    (1001) docker     (123)      986 2023-04-26 15:20:16.000000 serverless-sdk-0.4.5/sls_sdk/lib/name.py
--rw-r--r--   0 runner    (1001) docker     (123)      459 2023-04-26 15:20:16.000000 serverless-sdk-0.4.5/sls_sdk/lib/notice.py
--rw-r--r--   0 runner    (1001) docker     (123)      737 2023-04-26 15:20:16.000000 serverless-sdk-0.4.5/sls_sdk/lib/stack_trace_string.py
--rw-r--r--   0 runner    (1001) docker     (123)     5222 2023-04-26 15:20:16.000000 serverless-sdk-0.4.5/sls_sdk/lib/tags.py
--rw-r--r--   0 runner    (1001) docker     (123)      273 2023-04-26 15:20:16.000000 serverless-sdk-0.4.5/sls_sdk/lib/timing.py
--rw-r--r--   0 runner    (1001) docker     (123)     9244 2023-04-26 15:20:16.000000 serverless-sdk-0.4.5/sls_sdk/lib/trace.py
--rw-r--r--   0 runner    (1001) docker     (123)      559 2023-04-26 15:20:16.000000 serverless-sdk-0.4.5/sls_sdk/lib/warning.py
--rw-r--r--   0 runner    (1001) docker     (123)     1485 2023-04-26 15:20:16.000000 serverless-sdk-0.4.5/sls_sdk/lib/warning_captured_event.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-26 15:20:43.000000 serverless-sdk-0.4.5/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     6849 2023-04-26 15:20:16.000000 serverless-sdk-0.4.5/tests/test_sdk.py
--rw-r--r--   0 runner    (1001) docker     (123)      247 2023-04-26 15:20:16.000000 serverless-sdk-0.4.5/tests/test_sdk_alias.py
--rw-r--r--   0 runner    (1001) docker     (123)    16668 2023-04-26 15:20:16.000000 serverless-sdk-0.4.5/tests/test_thread_safety.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 17:09:37.000000 serverless-sdk-0.4.6/
+-rw-r--r--   0 runner    (1001) docker     (123)     3186 2023-05-05 17:09:37.000000 serverless-sdk-0.4.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2355 2023-05-05 17:09:15.000000 serverless-sdk-0.4.6/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1910 2023-05-05 17:09:15.000000 serverless-sdk-0.4.6/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 17:09:37.000000 serverless-sdk-0.4.6/serverless_sdk/
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-05-05 17:09:15.000000 serverless-sdk-0.4.6/serverless_sdk/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 17:09:37.000000 serverless-sdk-0.4.6/serverless_sdk.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3186 2023-05-05 17:09:37.000000 serverless-sdk-0.4.6/serverless_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      966 2023-05-05 17:09:37.000000 serverless-sdk-0.4.6/serverless_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 17:09:37.000000 serverless-sdk-0.4.6/serverless_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      280 2023-05-05 17:09:37.000000 serverless-sdk-0.4.6/serverless_sdk.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-05 17:09:37.000000 serverless-sdk-0.4.6/serverless_sdk.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-05 17:09:37.000000 serverless-sdk-0.4.6/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 17:09:37.000000 serverless-sdk-0.4.6/sls_sdk/
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-05 17:09:15.000000 serverless-sdk-0.4.6/sls_sdk/VERSION
+-rw-r--r--   0 runner    (1001) docker     (123)     5513 2023-05-05 17:09:15.000000 serverless-sdk-0.4.6/sls_sdk/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      520 2023-05-05 17:09:15.000000 serverless-sdk-0.4.6/sls_sdk/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      770 2023-05-05 17:09:15.000000 serverless-sdk-0.4.6/sls_sdk/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 17:09:37.000000 serverless-sdk-0.4.6/sls_sdk/lib/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 17:09:15.000000 serverless-sdk-0.4.6/sls_sdk/lib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2583 2023-05-05 17:09:15.000000 serverless-sdk-0.4.6/sls_sdk/lib/captured_event.py
+-rw-r--r--   0 runner    (1001) docker     (123)      636 2023-05-05 17:09:15.000000 serverless-sdk-0.4.6/sls_sdk/lib/emitter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1430 2023-05-05 17:09:15.000000 serverless-sdk-0.4.6/sls_sdk/lib/error.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1919 2023-05-05 17:09:15.000000 serverless-sdk-0.4.6/sls_sdk/lib/error_captured_event.py
+-rw-r--r--   0 runner    (1001) docker     (123)      326 2023-05-05 17:09:15.000000 serverless-sdk-0.4.6/sls_sdk/lib/id.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 17:09:37.000000 serverless-sdk-0.4.6/sls_sdk/lib/instrumentation/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 17:09:15.000000 serverless-sdk-0.4.6/sls_sdk/lib/instrumentation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5559 2023-05-05 17:09:15.000000 serverless-sdk-0.4.6/sls_sdk/lib/instrumentation/flask.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16308 2023-05-05 17:09:15.000000 serverless-sdk-0.4.6/sls_sdk/lib/instrumentation/http.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2023 2023-05-05 17:09:15.000000 serverless-sdk-0.4.6/sls_sdk/lib/instrumentation/import_hook.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2321 2023-05-05 17:09:15.000000 serverless-sdk-0.4.6/sls_sdk/lib/instrumentation/logging.py
+-rw-r--r--   0 runner    (1001) docker     (123)      986 2023-05-05 17:09:15.000000 serverless-sdk-0.4.6/sls_sdk/lib/name.py
+-rw-r--r--   0 runner    (1001) docker     (123)      459 2023-05-05 17:09:15.000000 serverless-sdk-0.4.6/sls_sdk/lib/notice.py
+-rw-r--r--   0 runner    (1001) docker     (123)      736 2023-05-05 17:09:15.000000 serverless-sdk-0.4.6/sls_sdk/lib/stack_trace_string.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5238 2023-05-05 17:09:15.000000 serverless-sdk-0.4.6/sls_sdk/lib/tags.py
+-rw-r--r--   0 runner    (1001) docker     (123)      273 2023-05-05 17:09:15.000000 serverless-sdk-0.4.6/sls_sdk/lib/timing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9307 2023-05-05 17:09:15.000000 serverless-sdk-0.4.6/sls_sdk/lib/trace.py
+-rw-r--r--   0 runner    (1001) docker     (123)      559 2023-05-05 17:09:15.000000 serverless-sdk-0.4.6/sls_sdk/lib/warning.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1485 2023-05-05 17:09:15.000000 serverless-sdk-0.4.6/sls_sdk/lib/warning_captured_event.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 17:09:15.000000 serverless-sdk-0.4.6/sls_sdk/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 17:09:37.000000 serverless-sdk-0.4.6/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     6958 2023-05-05 17:09:15.000000 serverless-sdk-0.4.6/tests/test_sdk.py
+-rw-r--r--   0 runner    (1001) docker     (123)      247 2023-05-05 17:09:15.000000 serverless-sdk-0.4.6/tests/test_sdk_alias.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16668 2023-05-05 17:09:15.000000 serverless-sdk-0.4.6/tests/test_thread_safety.py
```

### Comparing `serverless-sdk-0.4.5/PKG-INFO` & `serverless-sdk-0.4.6/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,16 +1,22 @@
 Metadata-Version: 2.1
 Name: serverless-sdk
-Version: 0.4.5
+Version: 0.4.6
 Summary: Serverless SDK for Python
 Author: serverlessinc
 Project-URL: changelog, https://github.com/serverless/console/blob/main/python/packages/sdk/CHANGELOG.md
 Project-URL: documentation, https://github.com/serverless/console/tree/main/python/packages/sdk
 Project-URL: homepage, https://www.serverless.com/console
 Project-URL: repository, https://github.com/serverless/console
+Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: tests
 
 # serverless-sdk
 
 ## [Serverless Console](https://www.serverless.com/console) SDK for Python
```

### Comparing `serverless-sdk-0.4.5/README.md` & `serverless-sdk-0.4.6/README.md`

 * *Files identical despite different names*

### Comparing `serverless-sdk-0.4.5/serverless_sdk.egg-info/PKG-INFO` & `serverless-sdk-0.4.6/serverless_sdk.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,16 +1,22 @@
 Metadata-Version: 2.1
 Name: serverless-sdk
-Version: 0.4.5
+Version: 0.4.6
 Summary: Serverless SDK for Python
 Author: serverlessinc
 Project-URL: changelog, https://github.com/serverless/console/blob/main/python/packages/sdk/CHANGELOG.md
 Project-URL: documentation, https://github.com/serverless/console/tree/main/python/packages/sdk
 Project-URL: homepage, https://www.serverless.com/console
 Project-URL: repository, https://github.com/serverless/console
+Classifier: Programming Language :: Python :: 3 :: Only
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: tests
 
 # serverless-sdk
 
 ## [Serverless Console](https://www.serverless.com/console) SDK for Python
```

### Comparing `serverless-sdk-0.4.5/serverless_sdk.egg-info/SOURCES.txt` & `serverless-sdk-0.4.6/serverless_sdk.egg-info/SOURCES.txt`

 * *Files 11% similar despite different names*

```diff
@@ -1,32 +1,36 @@
 README.md
 pyproject.toml
+./sls_sdk/VERSION
 serverless_sdk/__init__.py
 serverless_sdk.egg-info/PKG-INFO
 serverless_sdk.egg-info/SOURCES.txt
 serverless_sdk.egg-info/dependency_links.txt
 serverless_sdk.egg-info/requires.txt
 serverless_sdk.egg-info/top_level.txt
+sls_sdk/VERSION
 sls_sdk/__init__.py
 sls_sdk/base.py
 sls_sdk/exceptions.py
+sls_sdk/py.typed
 sls_sdk/lib/__init__.py
 sls_sdk/lib/captured_event.py
 sls_sdk/lib/emitter.py
 sls_sdk/lib/error.py
 sls_sdk/lib/error_captured_event.py
 sls_sdk/lib/id.py
 sls_sdk/lib/name.py
 sls_sdk/lib/notice.py
 sls_sdk/lib/stack_trace_string.py
 sls_sdk/lib/tags.py
 sls_sdk/lib/timing.py
 sls_sdk/lib/trace.py
 sls_sdk/lib/warning.py
 sls_sdk/lib/warning_captured_event.py
+sls_sdk/lib/instrumentation/__init__.py
 sls_sdk/lib/instrumentation/flask.py
 sls_sdk/lib/instrumentation/http.py
 sls_sdk/lib/instrumentation/import_hook.py
 sls_sdk/lib/instrumentation/logging.py
 tests/test_sdk.py
 tests/test_sdk_alias.py
 tests/test_thread_safety.py
```

### Comparing `serverless-sdk-0.4.5/sls_sdk/__init__.py` & `serverless-sdk-0.4.6/sls_sdk/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -61,16 +61,16 @@
         self.disable_flask_monitoring = (
             bool(environ.get("SLS_DISABLE_FLASK_MONITORING"))
             or disable_flask_monitoring
         )
 
 
 class ServerlessSdk:
-    name: Final[str] = __name__
-    version: Final[str] = __version__
+    name: str = __name__
+    version: str = __version__
     _event_emitter: EventEmitter
 
     trace_spans: TraceSpans
     instrumentation: Final = SimpleNamespace()
 
     org_id: Optional[str] = None
     _settings: ServerlessSdkSettings
@@ -100,15 +100,15 @@
         disable_request_response_monitoring: Optional[bool] = False,
         disable_http_monitoring: Optional[bool] = False,
         disable_flask_monitoring: Optional[bool] = False,
         **kwargs,
     ):
         if self._is_initialized:
             return
-        self.org_id = environ.get(SLS_ORG_ID, default=org_id)
+        self.org_id = environ.get(SLS_ORG_ID) or org_id
         self._is_debug_mode = bool(environ.get("SLS_SDK_DEBUG"))
         self._is_dev_mode = bool(environ.get("SLS_DEV_MODE_ORG_ID"))
         self._settings = ServerlessSdkSettings(
             disable_captured_events_stdout,
             disable_python_log_monitoring,
             disable_request_response_monitoring,
             disable_http_monitoring,
@@ -124,19 +124,21 @@
             install_http()
 
         if not self._settings.disable_flask_monitoring:
             from .lib.instrumentation.flask import install as install_flask
 
             install_flask()
 
-        if hasattr(self, "_initialize_extension"):
-            self._initialize_extension(*args, **kwargs)
+        self._initialize_extension(*args, **kwargs)
 
         self._is_initialized = True
 
+    def _initialize_extension(self, *args, **kwargs):
+        pass
+
     def _create_trace_span(
         self,
         name: str,
         input: Optional[str] = None,
         output: Optional[str] = None,
         start_time: Optional[Nanoseconds] = None,
         tags: Optional[Tags] = None,
```

### Comparing `serverless-sdk-0.4.5/sls_sdk/exceptions.py` & `serverless-sdk-0.4.6/sls_sdk/exceptions.py`

 * *Files identical despite different names*

### Comparing `serverless-sdk-0.4.5/sls_sdk/lib/captured_event.py` & `serverless-sdk-0.4.6/sls_sdk/lib/captured_event.py`

 * *Files identical despite different names*

### Comparing `serverless-sdk-0.4.5/sls_sdk/lib/error.py` & `serverless-sdk-0.4.6/sls_sdk/lib/error.py`

 * *Files identical despite different names*

### Comparing `serverless-sdk-0.4.5/sls_sdk/lib/error_captured_event.py` & `serverless-sdk-0.4.6/sls_sdk/lib/error_captured_event.py`

 * *Files identical despite different names*

### Comparing `serverless-sdk-0.4.5/sls_sdk/lib/instrumentation/flask.py` & `serverless-sdk-0.4.6/sls_sdk/lib/instrumentation/flask.py`

 * *Files identical despite different names*

### Comparing `serverless-sdk-0.4.5/sls_sdk/lib/instrumentation/http.py` & `serverless-sdk-0.4.6/sls_sdk/lib/instrumentation/http.py`

 * *Files 1% similar despite different names*

```diff
@@ -275,15 +275,15 @@
         return _func
 
     def _instrumented_getresponse(self):
         # See https://docs.python.org/3/library/http.client.html#http.client.HTTPConnection.getresponse
         # for the signature of the getresponse method
         def _func(_self, *args, **kwargs):
             trace_span = _HTTP_SPAN.get()
-            if _self._sls_ignore or not trace_span:
+            if getattr(self, "_sls_ignore", False) or not trace_span:
                 return self._original_getresponse(_self, *args, **kwargs)
 
             try:
                 response = self._original_getresponse(_self, *args, **kwargs)
                 trace_span.tags["http.status_code"] = response.status
                 self._capture_response_body(trace_span, response)
                 return response
@@ -328,14 +328,15 @@
 # being called recursively.
 _URLLIB3_IS_RECURSIVE_CALL = contextvars.ContextVar(
     "urllib3-recursive-call", default=False
 )
 
 
 class URLLib3Instrumenter(BaseInstrumenter):
+    @staticmethod
     @contextlib.contextmanager
     def _prevent_recursive_instrumentation():
         _URLLIB3_IS_RECURSIVE_CALL.set(True)
         _DISABLE_NATIVE_INSTRUMENTATION.set(True)
         try:
             yield
         finally:
```

### Comparing `serverless-sdk-0.4.5/sls_sdk/lib/instrumentation/import_hook.py` & `serverless-sdk-0.4.6/sls_sdk/lib/instrumentation/import_hook.py`

 * *Files identical despite different names*

### Comparing `serverless-sdk-0.4.5/sls_sdk/lib/instrumentation/logging.py` & `serverless-sdk-0.4.6/sls_sdk/lib/instrumentation/logging.py`

 * *Files identical despite different names*

### Comparing `serverless-sdk-0.4.5/sls_sdk/lib/name.py` & `serverless-sdk-0.4.6/sls_sdk/lib/name.py`

 * *Files identical despite different names*

### Comparing `serverless-sdk-0.4.5/sls_sdk/lib/stack_trace_string.py` & `serverless-sdk-0.4.6/sls_sdk/lib/stack_trace_string.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import inspect
 from typing import Optional, Any
 
 
 def resolve(error: Optional[Any] = None) -> str:
     if isinstance(error, BaseException):
         # in case of an actual Exception, stack trace is already set up.
-        return "".join(traceback.format_exception(error, error, error.__traceback__))
+        return "".join(traceback.format_exception(None, error, error.__traceback__))
     else:
         # in case of errors that are not exceptions, return the current stack trace
         # but exclude the most recent 3 frames to make sure stack trace ends at
         # customer's code and does not include SDK internal methods.
         depth = len(inspect.stack())
         relevant_frame = sys._getframe(3) if depth > 3 else None
         return "".join(traceback.format_stack(f=relevant_frame))
```

### Comparing `serverless-sdk-0.4.5/sls_sdk/lib/tags.py` & `serverless-sdk-0.4.6/sls_sdk/lib/tags.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from __future__ import annotations
 import re
 from datetime import datetime
 from math import inf, nan
 from re import Pattern
-from typing import Dict, List, Mapping, Tuple, Optional
+from typing import Dict, List, Mapping, Tuple, Optional, Any
 from js_regex import compile
 from typing_extensions import Final, get_args
 from threading import Lock
 from .error import report as report_error
 from ..base import TagType, ValidTags
 from ..exceptions import (
     DuplicateTraceSpanName,
@@ -118,15 +118,15 @@
     raise InvalidTraceSpanTagName(
         f"Invalid trace span tag {name}: {name.capitalize()} "
         f"should contain dot separated tokens that follow "
         f'"[a-z][a-z0-9_]*" pattern. Received {name}'
     )
 
 
-def ensure_tag_value(attr: str, value: str) -> ValidTags:
+def ensure_tag_value(attr: str, value: ValidTags) -> ValidTags:
     valid_types: Tuple[type] = get_args(TagType)  # type: ignore
     valid_types = (*valid_types, list)  # type: ignore
 
     if not isinstance(value, valid_types):
         raise InvalidTraceSpanTagValue(
             f"Invalid trace span tag value for {attr}: "
             f"Expected {valid_types}, received {value}"
@@ -168,15 +168,15 @@
 
 
 def _snake_to_camel_case(string):
     return re.sub(r"_(.)", lambda match: match.group(1).upper(), string)
 
 
 def convert_tags_to_protobuf(tags: Tags):
-    protobuf_tags = {}
+    protobuf_tags: Any = {}
     for key, value in tags.items():
         context = protobuf_tags
         key_tokens = key.split(".")
         key_tokens = [_snake_to_camel_case(token) for token in key_tokens]
         last_token = key_tokens.pop()
         for token in key_tokens:
             if token not in context:
```

### Comparing `serverless-sdk-0.4.5/sls_sdk/lib/trace.py` & `serverless-sdk-0.4.6/sls_sdk/lib/trace.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from collections.abc import Iterable
 import logging
 import time
 import threading
 from typing import List, Optional, Callable
 from contextvars import ContextVar
 from backports.cached_property import cached_property  # available in Python >=3.8
-from typing_extensions import Final, Self
+from typing_extensions import Final
 import json
 from .instrumentation.import_hook import ImportHook
 from .timing import to_protobuf_epoch_timestamp
 from ..base import Nanoseconds, TraceId
 from ..exceptions import (
     ClosureOnClosedSpan,
     FutureSpanStartTime,
@@ -52,23 +52,23 @@
 
 
 _import_hook = ImportHook("threading")
 _import_hook.enable(_install_thread_hook)
 
 
 class TraceSpan:
-    parent_span: Self
+    parent_span: "TraceSpan"
     name: str
     start_time: Nanoseconds
     end_time: Optional[Nanoseconds] = None
     _input: Optional[str] = None
     _output: Optional[str] = None
     tags: Tags
     custom_tags: Tags
-    sub_spans: List[Self]
+    sub_spans: List["TraceSpan"]
     _on_close_by_root: Optional[Callable] = None
 
     def __init__(
         self,
         name: str,
         input: Optional[str] = None,
         output: Optional[str] = None,
@@ -170,26 +170,26 @@
         return parent.trace_id if parent else generate_id()
 
     @property
     def spans(self) -> List[TraceSpan]:
         return [self] + list(_flatten([s.spans for s in self.sub_spans]))
 
     @property
-    def output(self) -> str:
+    def output(self) -> Optional[str]:
         return self._output
 
     @output.setter
     def output(self, value: str):
         if value is not None and not isinstance(value, str):
             raise InvalidType("`output` must be a string.")
 
         self._output = value
 
     @property
-    def input(self) -> str:
+    def input(self) -> Optional[str]:
         return self._input
 
     @input.setter
     def input(self, value: str):
         if value is not None and not isinstance(value, str):
             raise InvalidType("`input` must be a string.")
 
@@ -266,14 +266,17 @@
             "output": self.output,
             "tags": convert_tags_to_protobuf(self.tags),
         }
         if self.custom_tags:
             result["customTags"] = json.dumps(self.custom_tags)
         return result
 
+    def clear(self):
+        pass
+
 
 def _flatten(xs):
     # https://stackoverflow.com/a/2158532
     for x in xs:
         if isinstance(x, Iterable) and not isinstance(x, (str, bytes)):
             yield from _flatten(x)
         else:
```

### Comparing `serverless-sdk-0.4.5/sls_sdk/lib/warning.py` & `serverless-sdk-0.4.6/sls_sdk/lib/warning.py`

 * *Files identical despite different names*

### Comparing `serverless-sdk-0.4.5/sls_sdk/lib/warning_captured_event.py` & `serverless-sdk-0.4.6/sls_sdk/lib/warning_captured_event.py`

 * *Files identical despite different names*

### Comparing `serverless-sdk-0.4.5/tests/test_sdk.py` & `serverless-sdk-0.4.6/tests/test_sdk.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from __future__ import annotations
 from types import MethodType
+from importlib_metadata import version
 from unittest.mock import MagicMock
 
 from . import get_params
 
 
 def test_can_import_serverless_sdk(reset_sdk):
     try:
@@ -17,14 +18,15 @@
     assert hasattr(instrumented_sdk, "name")
     assert isinstance(instrumented_sdk.name, str)
 
 
 def test_has_version(instrumented_sdk):
     assert hasattr(instrumented_sdk, "version")
     assert isinstance(instrumented_sdk.version, str)
+    assert instrumented_sdk.version == version(instrumented_sdk.name)
 
 
 def test_has_tracespans(instrumented_sdk):
     assert hasattr(instrumented_sdk, "trace_spans")
 
 
 def test_has_instrumentation(instrumented_sdk):
```

### Comparing `serverless-sdk-0.4.5/tests/test_thread_safety.py` & `serverless-sdk-0.4.6/tests/test_thread_safety.py`

 * *Files identical despite different names*

