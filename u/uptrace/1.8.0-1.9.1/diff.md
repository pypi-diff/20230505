# Comparing `tmp/uptrace-1.8.0.tar.gz` & `tmp/uptrace-1.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "uptrace-1.8.0.tar", last modified: Fri Dec 24 08:57:16 2021, max compression
+gzip compressed data, was "uptrace-1.9.1.tar", last modified: Wed Feb  2 07:22:09 2022, max compression
```

## Comparing `uptrace-1.8.0.tar` & `uptrace-1.9.1.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxr-x   0 vmihailenco  (1000) vmihailenco  (1000)        0 2021-12-24 08:57:16.628729 uptrace-1.8.0/
--rw-rw-r--   0 vmihailenco  (1000) vmihailenco  (1000)     2826 2021-12-24 08:57:16.628729 uptrace-1.8.0/PKG-INFO
--rw-r--r--   0 vmihailenco  (1000) vmihailenco  (1000)     1680 2021-10-28 11:46:07.000000 uptrace-1.8.0/README.md
--rw-rw-r--   0 vmihailenco  (1000) vmihailenco  (1000)     1070 2021-12-24 08:57:16.628729 uptrace-1.8.0/setup.cfg
--rw-r--r--   0 vmihailenco  (1000) vmihailenco  (1000)      186 2020-11-11 10:54:39.000000 uptrace-1.8.0/setup.py
-drwxrwxr-x   0 vmihailenco  (1000) vmihailenco  (1000)        0 2021-12-24 08:57:16.628729 uptrace-1.8.0/src/
-drwxrwxr-x   0 vmihailenco  (1000) vmihailenco  (1000)        0 2021-12-24 08:57:16.628729 uptrace-1.8.0/src/uptrace/
--rw-rw-r--   0 vmihailenco  (1000) vmihailenco  (1000)      299 2021-12-24 08:50:21.000000 uptrace-1.8.0/src/uptrace/__init__.py
--rw-rw-r--   0 vmihailenco  (1000) vmihailenco  (1000)     1114 2021-12-24 08:38:44.000000 uptrace-1.8.0/src/uptrace/client.py
--rw-rw-r--   0 vmihailenco  (1000) vmihailenco  (1000)      331 2021-03-28 13:42:32.000000 uptrace-1.8.0/src/uptrace/distro.py
--rw-rw-r--   0 vmihailenco  (1000) vmihailenco  (1000)     1659 2021-12-24 08:39:31.000000 uptrace-1.8.0/src/uptrace/dsn.py
--rw-rw-r--   0 vmihailenco  (1000) vmihailenco  (1000)     3253 2021-12-24 08:39:05.000000 uptrace-1.8.0/src/uptrace/uptrace.py
--rw-rw-r--   0 vmihailenco  (1000) vmihailenco  (1000)      106 2021-03-19 15:22:33.000000 uptrace-1.8.0/src/uptrace/util.py
--rw-r--r--   0 vmihailenco  (1000) vmihailenco  (1000)       54 2021-12-24 08:56:48.000000 uptrace-1.8.0/src/uptrace/version.py
-drwxrwxr-x   0 vmihailenco  (1000) vmihailenco  (1000)        0 2021-12-24 08:57:16.628729 uptrace-1.8.0/src/uptrace.egg-info/
--rw-rw-r--   0 vmihailenco  (1000) vmihailenco  (1000)     2826 2021-12-24 08:57:16.000000 uptrace-1.8.0/src/uptrace.egg-info/PKG-INFO
--rw-rw-r--   0 vmihailenco  (1000) vmihailenco  (1000)      448 2021-12-24 08:57:16.000000 uptrace-1.8.0/src/uptrace.egg-info/SOURCES.txt
--rw-rw-r--   0 vmihailenco  (1000) vmihailenco  (1000)        1 2021-12-24 08:57:16.000000 uptrace-1.8.0/src/uptrace.egg-info/dependency_links.txt
--rw-rw-r--   0 vmihailenco  (1000) vmihailenco  (1000)       70 2021-12-24 08:57:16.000000 uptrace-1.8.0/src/uptrace.egg-info/entry_points.txt
--rw-rw-r--   0 vmihailenco  (1000) vmihailenco  (1000)        1 2020-11-11 14:00:03.000000 uptrace-1.8.0/src/uptrace.egg-info/not-zip-safe
--rw-rw-r--   0 vmihailenco  (1000) vmihailenco  (1000)      123 2021-12-24 08:57:16.000000 uptrace-1.8.0/src/uptrace.egg-info/requires.txt
--rw-rw-r--   0 vmihailenco  (1000) vmihailenco  (1000)        8 2021-12-24 08:57:16.000000 uptrace-1.8.0/src/uptrace.egg-info/top_level.txt
-drwxrwxr-x   0 vmihailenco  (1000) vmihailenco  (1000)        0 2021-12-24 08:57:16.628729 uptrace-1.8.0/test/
--rw-rw-r--   0 vmihailenco  (1000) vmihailenco  (1000)     1202 2021-12-24 08:51:30.000000 uptrace-1.8.0/test/test_uptrace.py
+drwxrwxr-x   0 vmihailenco  (1000) vmihailenco  (1000)        0 2022-02-02 07:22:09.540920 uptrace-1.9.1/
+-rw-rw-r--   0 vmihailenco  (1000) vmihailenco  (1000)     2826 2022-02-02 07:22:09.540920 uptrace-1.9.1/PKG-INFO
+-rw-r--r--   0 vmihailenco  (1000) vmihailenco  (1000)     1680 2021-10-28 11:46:07.000000 uptrace-1.9.1/README.md
+-rw-rw-r--   0 vmihailenco  (1000) vmihailenco  (1000)     1070 2022-02-02 07:22:09.540920 uptrace-1.9.1/setup.cfg
+-rw-r--r--   0 vmihailenco  (1000) vmihailenco  (1000)      186 2020-11-11 10:54:39.000000 uptrace-1.9.1/setup.py
+drwxrwxr-x   0 vmihailenco  (1000) vmihailenco  (1000)        0 2022-02-02 07:22:09.540920 uptrace-1.9.1/src/
+drwxrwxr-x   0 vmihailenco  (1000) vmihailenco  (1000)        0 2022-02-02 07:22:09.540920 uptrace-1.9.1/src/uptrace/
+-rw-rw-r--   0 vmihailenco  (1000) vmihailenco  (1000)      299 2021-12-24 08:50:21.000000 uptrace-1.9.1/src/uptrace/__init__.py
+-rw-rw-r--   0 vmihailenco  (1000) vmihailenco  (1000)     1114 2021-12-24 08:38:44.000000 uptrace-1.9.1/src/uptrace/client.py
+-rw-rw-r--   0 vmihailenco  (1000) vmihailenco  (1000)      331 2021-03-28 13:42:32.000000 uptrace-1.9.1/src/uptrace/distro.py
+-rw-rw-r--   0 vmihailenco  (1000) vmihailenco  (1000)     1863 2022-02-02 07:21:20.000000 uptrace-1.9.1/src/uptrace/dsn.py
+-rw-rw-r--   0 vmihailenco  (1000) vmihailenco  (1000)     3781 2022-02-02 07:21:20.000000 uptrace-1.9.1/src/uptrace/uptrace.py
+-rw-rw-r--   0 vmihailenco  (1000) vmihailenco  (1000)      106 2021-03-19 15:22:33.000000 uptrace-1.9.1/src/uptrace/util.py
+-rw-r--r--   0 vmihailenco  (1000) vmihailenco  (1000)       54 2022-02-02 07:21:46.000000 uptrace-1.9.1/src/uptrace/version.py
+drwxrwxr-x   0 vmihailenco  (1000) vmihailenco  (1000)        0 2022-02-02 07:22:09.540920 uptrace-1.9.1/src/uptrace.egg-info/
+-rw-rw-r--   0 vmihailenco  (1000) vmihailenco  (1000)     2826 2022-02-02 07:22:09.000000 uptrace-1.9.1/src/uptrace.egg-info/PKG-INFO
+-rw-rw-r--   0 vmihailenco  (1000) vmihailenco  (1000)      448 2022-02-02 07:22:09.000000 uptrace-1.9.1/src/uptrace.egg-info/SOURCES.txt
+-rw-rw-r--   0 vmihailenco  (1000) vmihailenco  (1000)        1 2022-02-02 07:22:09.000000 uptrace-1.9.1/src/uptrace.egg-info/dependency_links.txt
+-rw-rw-r--   0 vmihailenco  (1000) vmihailenco  (1000)       70 2022-02-02 07:22:09.000000 uptrace-1.9.1/src/uptrace.egg-info/entry_points.txt
+-rw-rw-r--   0 vmihailenco  (1000) vmihailenco  (1000)        1 2020-11-11 14:00:03.000000 uptrace-1.9.1/src/uptrace.egg-info/not-zip-safe
+-rw-rw-r--   0 vmihailenco  (1000) vmihailenco  (1000)      123 2022-02-02 07:22:09.000000 uptrace-1.9.1/src/uptrace.egg-info/requires.txt
+-rw-rw-r--   0 vmihailenco  (1000) vmihailenco  (1000)        8 2022-02-02 07:22:09.000000 uptrace-1.9.1/src/uptrace.egg-info/top_level.txt
+drwxrwxr-x   0 vmihailenco  (1000) vmihailenco  (1000)        0 2022-02-02 07:22:09.540920 uptrace-1.9.1/test/
+-rw-rw-r--   0 vmihailenco  (1000) vmihailenco  (1000)     1275 2022-02-02 07:21:20.000000 uptrace-1.9.1/test/test_uptrace.py
```

### Comparing `uptrace-1.8.0/PKG-INFO` & `uptrace-1.9.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: uptrace
-Version: 1.8.0
+Version: 1.9.1
 Summary: Uptrace client for Python
 Home-page: https://uptrace.dev
 Author: Uptrace.dev
 Author-email: support@uptrace.dev
 License: BSD
 Description: # Uptrace for Python
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: uptrace Version: 1.8.0 Summary: Uptrace client for
+Metadata-Version: 2.1 Name: uptrace Version: 1.9.1 Summary: Uptrace client for
 Python Home-page: https://uptrace.dev Author: Uptrace.dev Author-email:
 support@uptrace.dev License: BSD Description: # Uptrace for Python ![build
 workflow](https://github.com/uptrace/uptrace-python/actions/workflows/
 build.yml/badge.svg) [![Documentation](https://img.shields.io/badge/uptrace-
 documentation-informational)](https://docs.uptrace.dev/guide/python.html)
 [https://docs.uptrace.dev/devicon/python-original.svg] ## Installation ##
 Introduction uptrace-python is an OpenTelemery distribution configured to
```

### Comparing `uptrace-1.8.0/README.md` & `uptrace-1.9.1/README.md`

 * *Files identical despite different names*

### Comparing `uptrace-1.8.0/setup.cfg` & `uptrace-1.9.1/setup.cfg`

 * *Files 10% similar despite different names*

```diff
@@ -23,18 +23,18 @@
 python_requires = >=3.6
 package_dir = 
 	=src
 packages = find_namespace:
 zip_safe = False
 include_package_data = True
 install_requires = 
-	opentelemetry-api==1.8.0
-	opentelemetry-sdk==1.8.0
-	opentelemetry-exporter-otlp==1.8.0
-	opentelemetry-instrumentation == 0.27b0
+	opentelemetry-api==1.9.1
+	opentelemetry-sdk==1.9.1
+	opentelemetry-exporter-otlp==1.9.1
+	opentelemetry-instrumentation == 0.28b1
 
 [options.packages.find]
 where = src
 include = *
 
 [options.entry_points]
 opentelemetry_distro =
```

### Comparing `uptrace-1.8.0/src/uptrace/client.py` & `uptrace-1.9.1/src/uptrace/client.py`

 * *Files identical despite different names*

### Comparing `uptrace-1.8.0/src/uptrace/dsn.py` & `uptrace-1.9.1/src/uptrace/dsn.py`

 * *Files 8% similar despite different names*

```diff
@@ -16,22 +16,28 @@
     def __str__(self):
         return self.str
 
     @property
     def app_addr(self):
         if self.host == "uptrace.dev":
             return f"{self.scheme}://app.uptrace.dev"
-        return f"{self.scheme}://{self.host}:14318"
+        return f"{self.scheme}://{self.host}:{self.port}"
 
     @property
-    def otlp_addr(self):
+    def otlp_http_addr(self):
         if self.host == "uptrace.dev":
             return "https://otlp.uptrace.dev"
         return f"{self.scheme}://{self.host}:{self.port}"
 
+    @property
+    def otlp_grpc_addr(self):
+        if self.host == "uptrace.dev":
+            return "https://otlp.uptrace.dev:4317"
+        return f"{self.scheme}://{self.host}:{self.port}"
+
 
 def parse_dsn(dsn: str) -> DSN:
     if dsn == "":
         raise ValueError("either dsn option or UPTRACE_DSN is required")
 
     o = urlparse(dsn)
     if not o.scheme:
```

### Comparing `uptrace-1.8.0/src/uptrace/uptrace.py` & `uptrace-1.9.1/src/uptrace/uptrace.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,26 +1,31 @@
 import logging
 import os
 from socket import gethostname
 from typing import Optional
 
 import grpc
-from opentelemetry import trace
+from opentelemetry import trace  # , _metrics
 from opentelemetry.sdk.trace import TracerProvider
 from opentelemetry.sdk.trace.export import BatchSpanProcessor
+
+# from opentelemetry.sdk._metrics import MeterProvider
+# from opentelemetry.sdk._metrics.export import PeriodicExportingMetricReader
 from opentelemetry.sdk.resources import Attributes, Resource
 from opentelemetry.exporter.otlp.proto.http import Compression
 from opentelemetry.exporter.otlp.proto.http.trace_exporter import OTLPSpanExporter
 
+# from opentelemetry.exporter.otlp.proto.grpc._metric_exporter import OTLPMetricExporter
+
 from .client import Client
 from .dsn import parse_dsn, DSN
 
 logger = logging.getLogger(__name__)
 
-_CLIENT = Client(parse_dsn("https://<key>@uptrace.dev/<project_id>"))
+_CLIENT = Client(parse_dsn("https://<token>@uptrace.dev/<project_id>"))
 
 # pylint: disable=too-many-arguments
 def configure_opentelemetry(
     dsn="",
     service_name: Optional[str] = "",
     service_version: Optional[str] = "",
     resource_attributes: Optional[Attributes] = None,
@@ -43,54 +48,63 @@
     try:
         dsn = parse_dsn(dsn)
     except ValueError as exc:
         # pylint:disable=logging-not-lazy
         logger.warning("Uptrace is disabled: %s", exc)
         return
 
-    _CLIENT = Client(dsn=dsn)
-    _configure_tracing(
-        dsn,
-        service_name=service_name,
-        service_version=service_version,
-        resource_attributes=resource_attributes,
-        resource=resource,
+    resource = _build_resource(
+        resource, resource_attributes, service_name, service_version
     )
 
+    _CLIENT = Client(dsn=dsn)
+    _configure_tracing(dsn, resource=resource)
+    # _configure_metrics(dsn, resource=resource)
+
 
 def _configure_tracing(
     dsn: DSN,
-    service_name: Optional[str] = "",
-    service_version: Optional[str] = "",
-    resource_attributes: Optional[Attributes] = None,
     resource: Optional[Resource] = None,
 ):
     if trace._TRACER_PROVIDER is None:
-        resource = _build_resource(
-            resource, resource_attributes, service_name, service_version
-        )
         provider = TracerProvider(resource=resource)
         trace.set_tracer_provider(provider)
 
     exporter = OTLPSpanExporter(
-        endpoint=f"{dsn.otlp_addr}/v1/traces",
+        endpoint=f"{dsn.otlp_http_addr}/v1/traces",
         headers=(("uptrace-dsn", dsn.str),),
         timeout=5,
         compression=Compression.Gzip,
     )
 
     bsp = BatchSpanProcessor(
         exporter,
         max_queue_size=1000,
         max_export_batch_size=1000,
         schedule_delay_millis=5000,
     )
     trace.get_tracer_provider().add_span_processor(bsp)
 
 
+# def _configure_metrics(
+#     dsn: DSN,
+#     resource: Optional[Resource] = None,
+# ):
+#     exporter = OTLPMetricExporter(
+#         endpoint=f"{dsn.otlp_grpc_addr}",
+#         headers=(("uptrace-dsn", dsn.str),),
+#         timeout=5,
+#         compression=grpc.Compression.Gzip,
+#     )
+#     reader = PeriodicExportingMetricReader(exporter, export_interval_millis=1000)
+#     provider = MeterProvider(metric_readers=[reader], resource=resource)
+#     print("SET", provider)
+#     _metrics.set_meter_provider(provider)
+
+
 def trace_url(span: Optional[trace.Span] = None) -> str:
     """Returns the trace URL for the span."""
 
     return _CLIENT.trace_url(span)
 
 
 def report_exception(exc: Exception) -> None:
```

### Comparing `uptrace-1.8.0/src/uptrace.egg-info/PKG-INFO` & `uptrace-1.9.1/src/uptrace.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: uptrace
-Version: 1.8.0
+Version: 1.9.1
 Summary: Uptrace client for Python
 Home-page: https://uptrace.dev
 Author: Uptrace.dev
 Author-email: support@uptrace.dev
 License: BSD
 Description: # Uptrace for Python
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: uptrace Version: 1.8.0 Summary: Uptrace client for
+Metadata-Version: 2.1 Name: uptrace Version: 1.9.1 Summary: Uptrace client for
 Python Home-page: https://uptrace.dev Author: Uptrace.dev Author-email:
 support@uptrace.dev License: BSD Description: # Uptrace for Python ![build
 workflow](https://github.com/uptrace/uptrace-python/actions/workflows/
 build.yml/badge.svg) [![Documentation](https://img.shields.io/badge/uptrace-
 documentation-informational)](https://docs.uptrace.dev/guide/python.html)
 [https://docs.uptrace.dev/devicon/python-original.svg] ## Installation ##
 Introduction uptrace-python is an OpenTelemery distribution configured to
```

### Comparing `uptrace-1.8.0/test/test_uptrace.py` & `uptrace-1.9.1/test/test_uptrace.py`

 * *Files 6% similar despite different names*

```diff
@@ -33,12 +33,13 @@
     url = uptrace.trace_url(span)
     assert url.startswith("https://app.uptrace.dev/traces/")
 
 
 def test_dsn():
     dsn = uptrace.parse_dsn("http://localhost:14318")
     assert dsn.app_addr == "http://localhost:14318"
-    assert dsn.otlp_addr == "http://localhost:14318"
+    assert dsn.otlp_http_addr == "http://localhost:14318"
+    assert dsn.otlp_grpc_addr == "http://localhost:14318"
 
     dsn = uptrace.parse_dsn("https://<key>@uptrace.dev/<project_id>")
     assert dsn.app_addr == "https://app.uptrace.dev"
-    assert dsn.otlp_addr == "https://otlp.uptrace.dev"
+    assert dsn.otlp_grpc_addr == "https://otlp.uptrace.dev:4317"
```

