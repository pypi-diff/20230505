# Comparing `tmp/azure-monitor-opentelemetry-1.0.0b12.tar.gz` & `tmp/azure-monitor-opentelemetry-1.0.0b9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/ApplicationInsights-Python/ApplicationInsights-Python/dist/azure-monitor-opentelemetry-1.0.0b12.tar", last modified: Fri May  5 19:16:38 2023, max compression
+gzip compressed data, was "azure-monitor-opentelemetry-1.0.0b9.tar", last modified: Wed Feb 22 22:31:32 2023, max compression
```

## Comparing `azure-monitor-opentelemetry-1.0.0b12.tar` & `azure-monitor-opentelemetry-1.0.0b9.tar`

### file list

```diff
@@ -1,95 +1,33 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 19:16:38.000000 azure-monitor-opentelemetry-1.0.0b12/
--rw-r--r--   0 runner    (1001) docker     (123)     1074 2023-05-05 19:16:31.000000 azure-monitor-opentelemetry-1.0.0b12/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      270 2023-05-05 19:16:31.000000 azure-monitor-opentelemetry-1.0.0b12/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    12888 2023-05-05 19:16:38.000000 azure-monitor-opentelemetry-1.0.0b12/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    12022 2023-05-05 19:16:31.000000 azure-monitor-opentelemetry-1.0.0b12/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 19:16:38.000000 azure-monitor-opentelemetry-1.0.0b12/azure/
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-05-05 19:16:31.000000 azure-monitor-opentelemetry-1.0.0b12/azure/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 19:16:38.000000 azure-monitor-opentelemetry-1.0.0b12/azure/monitor/
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-05-05 19:16:31.000000 azure-monitor-opentelemetry-1.0.0b12/azure/monitor/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 19:16:38.000000 azure-monitor-opentelemetry-1.0.0b12/azure/monitor/opentelemetry/
--rw-r--r--   0 runner    (1001) docker     (123)      480 2023-05-05 19:16:31.000000 azure-monitor-opentelemetry-1.0.0b12/azure/monitor/opentelemetry/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6102 2023-05-05 19:16:31.000000 azure-monitor-opentelemetry-1.0.0b12/azure/monitor/opentelemetry/_configure.py
--rw-r--r--   0 runner    (1001) docker     (123)     2576 2023-05-05 19:16:31.000000 azure-monitor-opentelemetry-1.0.0b12/azure/monitor/opentelemetry/_constants.py
--rw-r--r--   0 runner    (1001) docker     (123)      709 2023-05-05 19:16:31.000000 azure-monitor-opentelemetry-1.0.0b12/azure/monitor/opentelemetry/_types.py
--rw-r--r--   0 runner    (1001) docker     (123)      328 2023-05-05 19:16:31.000000 azure-monitor-opentelemetry-1.0.0b12/azure/monitor/opentelemetry/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 19:16:38.000000 azure-monitor-opentelemetry-1.0.0b12/azure/monitor/opentelemetry/autoinstrumentation/
--rw-r--r--   0 runner    (1001) docker     (123)      305 2023-05-05 19:16:31.000000 azure-monitor-opentelemetry-1.0.0b12/azure/monitor/opentelemetry/autoinstrumentation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1093 2023-05-05 19:16:31.000000 azure-monitor-opentelemetry-1.0.0b12/azure/monitor/opentelemetry/autoinstrumentation/_configurator.py
--rw-r--r--   0 runner    (1001) docker     (123)     2746 2023-05-05 19:16:31.000000 azure-monitor-opentelemetry-1.0.0b12/azure/monitor/opentelemetry/autoinstrumentation/_distro.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 19:16:38.000000 azure-monitor-opentelemetry-1.0.0b12/azure/monitor/opentelemetry/diagnostics/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 19:16:31.000000 azure-monitor-opentelemetry-1.0.0b12/azure/monitor/opentelemetry/diagnostics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3130 2023-05-05 19:16:31.000000 azure-monitor-opentelemetry-1.0.0b12/azure/monitor/opentelemetry/diagnostics/_diagnostic_logging.py
--rw-r--r--   0 runner    (1001) docker     (123)     1933 2023-05-05 19:16:31.000000 azure-monitor-opentelemetry-1.0.0b12/azure/monitor/opentelemetry/diagnostics/_status_logger.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 19:16:38.000000 azure-monitor-opentelemetry-1.0.0b12/azure/monitor/opentelemetry/util/
--rw-r--r--   0 runner    (1001) docker     (123)      306 2023-05-05 19:16:31.000000 azure-monitor-opentelemetry-1.0.0b12/azure/monitor/opentelemetry/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3529 2023-05-05 19:16:31.000000 azure-monitor-opentelemetry-1.0.0b12/azure/monitor/opentelemetry/util/configurations.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 19:16:38.000000 azure-monitor-opentelemetry-1.0.0b12/azure_monitor_opentelemetry.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    12888 2023-05-05 19:16:38.000000 azure-monitor-opentelemetry-1.0.0b12/azure_monitor_opentelemetry.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2785 2023-05-05 19:16:38.000000 azure-monitor-opentelemetry-1.0.0b12/azure_monitor_opentelemetry.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 19:16:38.000000 azure-monitor-opentelemetry-1.0.0b12/azure_monitor_opentelemetry.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      295 2023-05-05 19:16:38.000000 azure-monitor-opentelemetry-1.0.0b12/azure_monitor_opentelemetry.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 19:16:38.000000 azure-monitor-opentelemetry-1.0.0b12/azure_monitor_opentelemetry.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      457 2023-05-05 19:16:38.000000 azure-monitor-opentelemetry-1.0.0b12/azure_monitor_opentelemetry.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-05 19:16:38.000000 azure-monitor-opentelemetry-1.0.0b12/azure_monitor_opentelemetry.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 19:16:38.000000 azure-monitor-opentelemetry-1.0.0b12/samples/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 19:16:38.000000 azure-monitor-opentelemetry-1.0.0b12/samples/logging/
--rw-r--r--   0 runner    (1001) docker     (123)      905 2023-05-05 19:16:31.000000 azure-monitor-opentelemetry-1.0.0b12/samples/logging/correlated_logs.py
--rw-r--r--   0 runner    (1001) docker     (123)      685 2023-05-05 19:16:31.000000 azure-monitor-opentelemetry-1.0.0b12/samples/logging/custom_properties.py
--rw-r--r--   0 runner    (1001) docker     (123)      878 2023-05-05 19:16:31.000000 azure-monitor-opentelemetry-1.0.0b12/samples/logging/exception_logs.py
--rw-r--r--   0 runner    (1001) docker     (123)      898 2023-05-05 19:16:31.000000 azure-monitor-opentelemetry-1.0.0b12/samples/logging/logs_with_traces.py
--rw-r--r--   0 runner    (1001) docker     (123)      669 2023-05-05 19:16:31.000000 azure-monitor-opentelemetry-1.0.0b12/samples/logging/simple.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 19:16:38.000000 azure-monitor-opentelemetry-1.0.0b12/samples/metrics/
--rw-r--r--   0 runner    (1001) docker     (123)      955 2023-05-05 19:16:31.000000 azure-monitor-opentelemetry-1.0.0b12/samples/metrics/attributes.py
--rw-r--r--   0 runner    (1001) docker     (123)     1630 2023-05-05 19:16:31.000000 azure-monitor-opentelemetry-1.0.0b12/samples/metrics/instruments.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 19:16:38.000000 azure-monitor-opentelemetry-1.0.0b12/samples/tracing/
--rw-r--r--   0 runner    (1001) docker     (123)      791 2023-05-05 19:16:31.000000 azure-monitor-opentelemetry-1.0.0b12/samples/tracing/db_psycopg2.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 19:16:38.000000 azure-monitor-opentelemetry-1.0.0b12/samples/tracing/django/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 19:16:38.000000 azure-monitor-opentelemetry-1.0.0b12/samples/tracing/django/sample/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 19:16:38.000000 azure-monitor-opentelemetry-1.0.0b12/samples/tracing/django/sample/example/
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-05-05 19:16:31.000000 azure-monitor-opentelemetry-1.0.0b12/samples/tracing/django/sample/example/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      157 2023-05-05 19:16:31.000000 azure-monitor-opentelemetry-1.0.0b12/samples/tracing/django/sample/example/admin.py
--rw-r--r--   0 runner    (1001) docker     (123)      240 2023-05-05 19:16:31.000000 azure-monitor-opentelemetry-1.0.0b12/samples/tracing/django/sample/example/apps.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 19:16:38.000000 azure-monitor-opentelemetry-1.0.0b12/samples/tracing/django/sample/example/migrations/
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-05-05 19:16:31.000000 azure-monitor-opentelemetry-1.0.0b12/samples/tracing/django/sample/example/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      151 2023-05-05 19:16:31.000000 azure-monitor-opentelemetry-1.0.0b12/samples/tracing/django/sample/example/models.py
--rw-r--r--   0 runner    (1001) docker     (123)      154 2023-05-05 19:16:31.000000 azure-monitor-opentelemetry-1.0.0b12/samples/tracing/django/sample/example/tests.py
--rw-r--r--   0 runner    (1001) docker     (123)      262 2023-05-05 19:16:31.000000 azure-monitor-opentelemetry-1.0.0b12/samples/tracing/django/sample/example/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)      824 2023-05-05 19:16:31.000000 azure-monitor-opentelemetry-1.0.0b12/samples/tracing/django/sample/example/views.py
--rw-r--r--   0 runner    (1001) docker     (123)      757 2023-05-05 19:16:31.000000 azure-monitor-opentelemetry-1.0.0b12/samples/tracing/django/sample/manage.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 19:16:38.000000 azure-monitor-opentelemetry-1.0.0b12/samples/tracing/django/sample/sample/
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-05-05 19:16:31.000000 azure-monitor-opentelemetry-1.0.0b12/samples/tracing/django/sample/sample/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      517 2023-05-05 19:16:31.000000 azure-monitor-opentelemetry-1.0.0b12/samples/tracing/django/sample/sample/asgi.py
--rw-r--r--   0 runner    (1001) docker     (123)     3376 2023-05-05 19:16:31.000000 azure-monitor-opentelemetry-1.0.0b12/samples/tracing/django/sample/sample/settings.py
--rw-r--r--   0 runner    (1001) docker     (123)      820 2023-05-05 19:16:31.000000 azure-monitor-opentelemetry-1.0.0b12/samples/tracing/django/sample/sample/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)      483 2023-05-05 19:16:31.000000 azure-monitor-opentelemetry-1.0.0b12/samples/tracing/django/sample/sample/wsgi.py
--rw-r--r--   0 runner    (1001) docker     (123)     1030 2023-05-05 19:16:31.000000 azure-monitor-opentelemetry-1.0.0b12/samples/tracing/http_fastapi.py
--rw-r--r--   0 runner    (1001) docker     (123)     1083 2023-05-05 19:16:31.000000 azure-monitor-opentelemetry-1.0.0b12/samples/tracing/http_flask.py
--rw-r--r--   0 runner    (1001) docker     (123)     1265 2023-05-05 19:16:31.000000 azure-monitor-opentelemetry-1.0.0b12/samples/tracing/http_requests.py
--rw-r--r--   0 runner    (1001) docker     (123)     1157 2023-05-05 19:16:31.000000 azure-monitor-opentelemetry-1.0.0b12/samples/tracing/http_urllib.py
--rw-r--r--   0 runner    (1001) docker     (123)     1138 2023-05-05 19:16:31.000000 azure-monitor-opentelemetry-1.0.0b12/samples/tracing/http_urllib3.py
--rw-r--r--   0 runner    (1001) docker     (123)     1055 2023-05-05 19:16:31.000000 azure-monitor-opentelemetry-1.0.0b12/samples/tracing/manual.py
--rw-r--r--   0 runner    (1001) docker     (123)      852 2023-05-05 19:16:31.000000 azure-monitor-opentelemetry-1.0.0b12/samples/tracing/sampling.py
--rw-r--r--   0 runner    (1001) docker     (123)      668 2023-05-05 19:16:31.000000 azure-monitor-opentelemetry-1.0.0b12/samples/tracing/simple.py
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-05-05 19:16:38.000000 azure-monitor-opentelemetry-1.0.0b12/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3653 2023-05-05 19:16:31.000000 azure-monitor-opentelemetry-1.0.0b12/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 19:16:38.000000 azure-monitor-opentelemetry-1.0.0b12/tests/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 19:16:38.000000 azure-monitor-opentelemetry-1.0.0b12/tests/autoinstrumentation/
--rw-r--r--   0 runner    (1001) docker     (123)     1210 2023-05-05 19:16:31.000000 azure-monitor-opentelemetry-1.0.0b12/tests/autoinstrumentation/test_distro.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 19:16:38.000000 azure-monitor-opentelemetry-1.0.0b12/tests/configuration/
--rw-r--r--   0 runner    (1001) docker     (123)    13101 2023-05-05 19:16:31.000000 azure-monitor-opentelemetry-1.0.0b12/tests/configuration/test_configure.py
--rw-r--r--   0 runner    (1001) docker     (123)     4293 2023-05-05 19:16:31.000000 azure-monitor-opentelemetry-1.0.0b12/tests/configuration/test_util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 19:16:38.000000 azure-monitor-opentelemetry-1.0.0b12/tests/diagnostics/
--rw-r--r--   0 runner    (1001) docker     (123)     7871 2023-05-05 19:16:31.000000 azure-monitor-opentelemetry-1.0.0b12/tests/diagnostics/test_diagnostic_logging.py
--rw-r--r--   0 runner    (1001) docker     (123)     8590 2023-05-05 19:16:31.000000 azure-monitor-opentelemetry-1.0.0b12/tests/diagnostics/test_status_logger.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 19:16:38.000000 azure-monitor-opentelemetry-1.0.0b12/tests/exporter/
--rw-r--r--   0 runner    (1001) docker     (123)     1365 2023-05-05 19:16:31.000000 azure-monitor-opentelemetry-1.0.0b12/tests/exporter/test_exporter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 19:16:38.000000 azure-monitor-opentelemetry-1.0.0b12/tests/instrumentation/
--rw-r--r--   0 runner    (1001) docker     (123)      755 2023-05-05 19:16:31.000000 azure-monitor-opentelemetry-1.0.0b12/tests/instrumentation/test_django.py
--rw-r--r--   0 runner    (1001) docker     (123)      840 2023-05-05 19:16:31.000000 azure-monitor-opentelemetry-1.0.0b12/tests/instrumentation/test_fastapi.py
--rw-r--r--   0 runner    (1001) docker     (123)      830 2023-05-05 19:16:31.000000 azure-monitor-opentelemetry-1.0.0b12/tests/instrumentation/test_flask.py
--rw-r--r--   0 runner    (1001) docker     (123)      765 2023-05-05 19:16:31.000000 azure-monitor-opentelemetry-1.0.0b12/tests/instrumentation/test_psycopg2.py
--rw-r--r--   0 runner    (1001) docker     (123)      765 2023-05-05 19:16:31.000000 azure-monitor-opentelemetry-1.0.0b12/tests/instrumentation/test_requests.py
--rw-r--r--   0 runner    (1001) docker     (123)      755 2023-05-05 19:16:31.000000 azure-monitor-opentelemetry-1.0.0b12/tests/instrumentation/test_urllib.py
--rw-r--r--   0 runner    (1001) docker     (123)      760 2023-05-05 19:16:31.000000 azure-monitor-opentelemetry-1.0.0b12/tests/instrumentation/test_urllib3.py
--rw-r--r--   0 runner    (1001) docker     (123)     5303 2023-05-05 19:16:31.000000 azure-monitor-opentelemetry-1.0.0b12/tests/test_constants.py
+drwxrwxrwx   0        0        0        0 2023-02-22 22:31:32.179282 azure-monitor-opentelemetry-1.0.0b9/
+-rw-rw-rw-   0        0        0     9608 2023-02-22 22:31:32.180284 azure-monitor-opentelemetry-1.0.0b9/PKG-INFO
+-rw-rw-rw-   0        0        0     8745 2023-02-22 22:28:31.000000 azure-monitor-opentelemetry-1.0.0b9/README.md
+drwxrwxrwx   0        0        0        0 2023-02-22 22:31:32.049037 azure-monitor-opentelemetry-1.0.0b9/azure/
+drwxrwxrwx   0        0        0        0 2023-02-22 22:31:32.050037 azure-monitor-opentelemetry-1.0.0b9/azure/monitor/
+drwxrwxrwx   0        0        0        0 2023-02-22 22:31:32.080216 azure-monitor-opentelemetry-1.0.0b9/azure/monitor/opentelemetry/
+-rw-rw-rw-   0        0        0      494 2023-02-22 21:27:14.000000 azure-monitor-opentelemetry-1.0.0b9/azure/monitor/opentelemetry/__init__.py
+-rw-rw-rw-   0        0        0     9163 2023-02-22 21:27:14.000000 azure-monitor-opentelemetry-1.0.0b9/azure/monitor/opentelemetry/_configure.py
+-rw-rw-rw-   0        0        0     2299 2023-02-22 21:27:14.000000 azure-monitor-opentelemetry-1.0.0b9/azure/monitor/opentelemetry/_constants.py
+-rw-rw-rw-   0        0        0      734 2023-02-22 21:27:14.000000 azure-monitor-opentelemetry-1.0.0b9/azure/monitor/opentelemetry/_types.py
+-rw-rw-rw-   0        0        0      334 2023-02-22 22:28:31.000000 azure-monitor-opentelemetry-1.0.0b9/azure/monitor/opentelemetry/_version.py
+drwxrwxrwx   0        0        0        0 2023-02-22 22:31:32.094215 azure-monitor-opentelemetry-1.0.0b9/azure/monitor/opentelemetry/autoinstrumentation/
+-rw-rw-rw-   0        0        0      310 2023-02-22 21:27:14.000000 azure-monitor-opentelemetry-1.0.0b9/azure/monitor/opentelemetry/autoinstrumentation/__init__.py
+-rw-rw-rw-   0        0        0     1125 2023-02-22 21:27:14.000000 azure-monitor-opentelemetry-1.0.0b9/azure/monitor/opentelemetry/autoinstrumentation/_configurator.py
+-rw-rw-rw-   0        0        0     2984 2023-02-22 21:27:14.000000 azure-monitor-opentelemetry-1.0.0b9/azure/monitor/opentelemetry/autoinstrumentation/_distro.py
+drwxrwxrwx   0        0        0        0 2023-02-22 22:31:32.107694 azure-monitor-opentelemetry-1.0.0b9/azure/monitor/opentelemetry/diagnostics/
+-rw-rw-rw-   0        0        0        0 2023-02-22 21:27:14.000000 azure-monitor-opentelemetry-1.0.0b9/azure/monitor/opentelemetry/diagnostics/__init__.py
+-rw-rw-rw-   0        0        0     3209 2023-02-22 21:27:14.000000 azure-monitor-opentelemetry-1.0.0b9/azure/monitor/opentelemetry/diagnostics/_diagnostic_logging.py
+-rw-rw-rw-   0        0        0     1987 2023-02-22 21:27:14.000000 azure-monitor-opentelemetry-1.0.0b9/azure/monitor/opentelemetry/diagnostics/_status_logger.py
+drwxrwxrwx   0        0        0        0 2023-02-22 22:31:32.112712 azure-monitor-opentelemetry-1.0.0b9/azure/monitor/opentelemetry/util/
+-rw-rw-rw-   0        0        0      647 2023-02-22 21:27:14.000000 azure-monitor-opentelemetry-1.0.0b9/azure/monitor/opentelemetry/util/__init__.py
+drwxrwxrwx   0        0        0        0 2023-02-22 22:31:32.175279 azure-monitor-opentelemetry-1.0.0b9/azure_monitor_opentelemetry.egg-info/
+-rw-rw-rw-   0        0        0     9608 2023-02-22 22:31:31.000000 azure-monitor-opentelemetry-1.0.0b9/azure_monitor_opentelemetry.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1014 2023-02-22 22:31:31.000000 azure-monitor-opentelemetry-1.0.0b9/azure_monitor_opentelemetry.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-02-22 22:31:31.000000 azure-monitor-opentelemetry-1.0.0b9/azure_monitor_opentelemetry.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      295 2023-02-22 22:31:31.000000 azure-monitor-opentelemetry-1.0.0b9/azure_monitor_opentelemetry.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        2 2023-02-22 21:49:02.000000 azure-monitor-opentelemetry-1.0.0b9/azure_monitor_opentelemetry.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0      320 2023-02-22 22:31:31.000000 azure-monitor-opentelemetry-1.0.0b9/azure_monitor_opentelemetry.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-02-22 22:31:31.000000 azure-monitor-opentelemetry-1.0.0b9/azure_monitor_opentelemetry.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       74 2023-02-22 22:31:32.195109 azure-monitor-opentelemetry-1.0.0b9/setup.cfg
+-rw-rw-rw-   0        0        0     3587 2023-02-22 22:28:31.000000 azure-monitor-opentelemetry-1.0.0b9/setup.py
+drwxrwxrwx   0        0        0        0 2023-02-22 22:31:32.178279 azure-monitor-opentelemetry-1.0.0b9/tests/
+-rw-rw-rw-   0        0        0     5452 2023-02-22 21:27:14.000000 azure-monitor-opentelemetry-1.0.0b9/tests/test_constants.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `azure-monitor-opentelemetry-1.0.0b12/azure/monitor/opentelemetry/_types.py` & `azure-monitor-opentelemetry-1.0.0b9/azure/monitor/opentelemetry/_types.py`

 * *Ordering differences only*

 * *Files 22% similar despite different names*

```diff
@@ -1,25 +1,25 @@
-# -------------------------------------------------------------------------
-# Copyright (c) Microsoft Corporation. All rights reserved.
-# Licensed under the MIT License. See License in the project root for
-# license information.
-# --------------------------------------------------------------------------
-
-from typing import Sequence, Union
-
-from opentelemetry.sdk.metrics.export import MetricReader
-from opentelemetry.sdk.metrics.view import View
-from opentelemetry.sdk.resources import Resource
-
-ConfigurationValue = Union[
-    str,
-    bool,
-    int,
-    float,
-    Resource,
-    Sequence[str],
-    Sequence[bool],
-    Sequence[int],
-    Sequence[float],
-    Sequence[MetricReader],
-    Sequence[View],
-]
+# -------------------------------------------------------------------------
+# Copyright (c) Microsoft Corporation. All rights reserved.
+# Licensed under the MIT License. See License in the project root for
+# license information.
+# --------------------------------------------------------------------------
+
+from typing import Sequence, Union
+
+from opentelemetry.sdk.metrics.export import MetricReader
+from opentelemetry.sdk.metrics.view import View
+from opentelemetry.sdk.resources import Resource
+
+ConfigurationValue = Union[
+    str,
+    bool,
+    int,
+    float,
+    Resource,
+    Sequence[str],
+    Sequence[bool],
+    Sequence[int],
+    Sequence[float],
+    Sequence[MetricReader],
+    Sequence[View],
+]
```

### Comparing `azure-monitor-opentelemetry-1.0.0b12/azure/monitor/opentelemetry/autoinstrumentation/_configurator.py` & `azure-monitor-opentelemetry-1.0.0b9/azure/monitor/opentelemetry/autoinstrumentation/_configurator.py`

 * *Ordering differences only*

 * *Files 14% similar despite different names*

```diff
@@ -1,32 +1,32 @@
-# -------------------------------------------------------------------------
-# Copyright (c) Microsoft Corporation. All rights reserved.
-# Licensed under the MIT License. See License in the project root for
-# license information.
-# --------------------------------------------------------------------------
-
-
-import logging
-
-from azure.monitor.opentelemetry.diagnostics._diagnostic_logging import (
-    AzureDiagnosticLogging,
-)
-from opentelemetry.sdk._configuration import _OTelSDKConfigurator
-
-_logger = logging.getLogger(__name__)
-
-
-class AzureMonitorConfigurator(_OTelSDKConfigurator):
-    def _configure(self, **kwargs):
-        try:
-            AzureDiagnosticLogging.enable(_logger)
-            super()._configure(**kwargs)
-        except ValueError as e:
-            _logger.error(
-                f"Azure Monitor Configurator failed during configuration due to a ValueError: {e}"
-            )
-            raise e
-        except Exception as e:
-            _logger.error(
-                f"Azure Monitor Configurator failed during configuration: {e}"
-            )
-            raise e
+# -------------------------------------------------------------------------
+# Copyright (c) Microsoft Corporation. All rights reserved.
+# Licensed under the MIT License. See License in the project root for
+# license information.
+# --------------------------------------------------------------------------
+
+
+import logging
+
+from azure.monitor.opentelemetry.diagnostics._diagnostic_logging import (
+    AzureDiagnosticLogging,
+)
+from opentelemetry.sdk._configuration import _OTelSDKConfigurator
+
+_logger = logging.getLogger(__name__)
+
+
+class AzureMonitorConfigurator(_OTelSDKConfigurator):
+    def _configure(self, **kwargs):
+        try:
+            AzureDiagnosticLogging.enable(_logger)
+            super()._configure(**kwargs)
+        except ValueError as e:
+            _logger.error(
+                f"Azure Monitor Configurator failed during configuration due to a ValueError: {e}"
+            )
+            raise e
+        except Exception as e:
+            _logger.error(
+                f"Azure Monitor Configurator failed during configuration: {e}"
+            )
+            raise e
```

### Comparing `azure-monitor-opentelemetry-1.0.0b12/azure/monitor/opentelemetry/autoinstrumentation/_distro.py` & `azure-monitor-opentelemetry-1.0.0b9/azure/monitor/opentelemetry/autoinstrumentation/_distro.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,75 +1,78 @@
-# -------------------------------------------------------------------------
-# Copyright (c) Microsoft Corporation. All rights reserved.
-# Licensed under the MIT License. See License in the project root for
-# license information.
-# --------------------------------------------------------------------------
-import logging
-from os import environ
-
-from azure.monitor.opentelemetry.diagnostics._diagnostic_logging import (
-    AzureDiagnosticLogging,
-)
-from azure.monitor.opentelemetry.diagnostics._status_logger import (
-    AzureStatusLogger,
-)
-from opentelemetry.environment_variables import (
-    OTEL_LOGS_EXPORTER,
-    OTEL_METRICS_EXPORTER,
-    OTEL_TRACES_EXPORTER,
-)
-from opentelemetry.instrumentation.distro import BaseDistro
-from opentelemetry.sdk.environment_variables import (
-    _OTEL_PYTHON_LOGGING_AUTO_INSTRUMENTATION_ENABLED,
-)
-
-_logger = logging.getLogger(__name__)
-_opentelemetry_logger = logging.getLogger("opentelemetry")
-# TODO: Enabled when duplicate logging issue is solved
-# _exporter_logger = logging.getLogger("azure.monitor.opentelemetry.exporter")
-
-
-class AzureMonitorDistro(BaseDistro):
-    def _configure(self, **kwargs) -> None:
-        try:
-            _configure_auto_instrumentation()
-        except Exception as ex:
-            _logger.exception(
-                ("Error occured auto-instrumenting AzureMonitorDistro")
-            )
-            raise ex
-
-
-def _configure_auto_instrumentation() -> None:
-    try:
-        AzureStatusLogger.log_status(False, "Distro being configured.")
-        AzureDiagnosticLogging.enable(_logger)
-        AzureDiagnosticLogging.enable(_opentelemetry_logger)
-        # TODO: Enabled when duplicate logging issue is solved
-        # if _EXPORTER_DIAGNOSTICS_ENABLED:
-        #     exporter_logger = logging.getLogger(
-        #         "azure.monitor.opentelemetry.exporter"
-        #     )
-        #     AzureDiagnosticLogging.enable(_exporter_logger)
-        environ.setdefault(
-            OTEL_METRICS_EXPORTER, "azure_monitor_opentelemetry_exporter"
-        )
-        environ.setdefault(
-            OTEL_TRACES_EXPORTER, "azure_monitor_opentelemetry_exporter"
-        )
-        environ.setdefault(
-            OTEL_LOGS_EXPORTER, "azure_monitor_opentelemetry_exporter"
-        )
-        environ.setdefault(
-            _OTEL_PYTHON_LOGGING_AUTO_INSTRUMENTATION_ENABLED, "true"
-        )
-        AzureStatusLogger.log_status(True)
-        _logger.info(
-            "Azure Monitor OpenTelemetry Distro configured successfully."
-        )
-    except Exception as exc:
-        AzureStatusLogger.log_status(False, reason=exc)
-        _logger.error(
-            "Azure Monitor OpenTelemetry Distro failed during "
-            + f"configuration: {exc}"
-        )
-        raise exc
+# -------------------------------------------------------------------------
+# Copyright (c) Microsoft Corporation. All rights reserved.
+# Licensed under the MIT License. See License in the project root for
+# license information.
+# --------------------------------------------------------------------------
+import logging
+from os import environ
+
+from azure.monitor.opentelemetry.diagnostics._diagnostic_logging import (
+    AzureDiagnosticLogging,
+)
+from azure.monitor.opentelemetry.diagnostics._status_logger import (
+    AzureStatusLogger,
+)
+from opentelemetry.environment_variables import (
+    OTEL_LOGS_EXPORTER,
+    OTEL_METRICS_EXPORTER,
+    OTEL_TRACES_EXPORTER,
+)
+from opentelemetry.instrumentation.distro import BaseDistro
+from opentelemetry.sdk.environment_variables import (
+    _OTEL_PYTHON_LOGGING_AUTO_INSTRUMENTATION_ENABLED,
+)
+
+_logger = logging.getLogger(__name__)
+_opentelemetry_logger = logging.getLogger("opentelemetry")
+# TODO: Enabled when duplicate logging issue is solved
+# _exporter_logger = logging.getLogger("azure.monitor.opentelemetry.exporter")
+
+
+class AzureMonitorDistro(BaseDistro):
+    def _configure(self, **kwargs) -> None:
+        try:
+            _configure_auto_instrumentation()
+        except Exception as ex:
+            _logger.exception(
+                ("Error occured auto-instrumenting AzureMonitorDistro")
+            )
+            raise ex
+
+
+def _configure_auto_instrumentation() -> None:
+    try:
+        AzureStatusLogger.log_status(False, "Distro being configured.")
+        AzureDiagnosticLogging.enable(_logger)
+        AzureDiagnosticLogging.enable(_opentelemetry_logger)
+        # TODO: Enabled when duplicate logging issue is solved
+        # if _EXPORTER_DIAGNOSTICS_ENABLED:
+        #     exporter_logger = logging.getLogger(
+        #         "azure.monitor.opentelemetry.exporter"
+        #     )
+        #     AzureDiagnosticLogging.enable(_exporter_logger)
+        # TODO: Uncomment when logging is out of preview
+        # environ.setdefault(OTEL_LOGS_EXPORTER,
+        #     "azure_monitor_opentelemetry_exporter")
+        environ.setdefault(
+            OTEL_METRICS_EXPORTER, "azure_monitor_opentelemetry_exporter"
+        )
+        environ.setdefault(
+            OTEL_TRACES_EXPORTER, "azure_monitor_opentelemetry_exporter"
+        )
+        environ.setdefault(
+            OTEL_LOGS_EXPORTER, "azure_monitor_opentelemetry_exporter"
+        )
+        environ.setdefault(
+            _OTEL_PYTHON_LOGGING_AUTO_INSTRUMENTATION_ENABLED, "true"
+        )
+        AzureStatusLogger.log_status(True)
+        _logger.info(
+            "Azure Monitor OpenTelemetry Distro configured successfully."
+        )
+    except Exception as exc:
+        AzureStatusLogger.log_status(False, reason=exc)
+        _logger.error(
+            "Azure Monitor OpenTelemetry Distro failed during "
+            + f"configuration: {exc}"
+        )
+        raise exc
```

### Comparing `azure-monitor-opentelemetry-1.0.0b12/azure/monitor/opentelemetry/diagnostics/_status_logger.py` & `azure-monitor-opentelemetry-1.0.0b9/azure/monitor/opentelemetry/diagnostics/_status_logger.py`

 * *Ordering differences only*

 * *Files 9% similar despite different names*

```diff
@@ -1,54 +1,54 @@
-# -------------------------------------------------------------------------
-# Copyright (c) Microsoft Corporation. All rights reserved.
-# Licensed under the MIT License. See License in the project root for
-# license information.
-# --------------------------------------------------------------------------
-
-from json import dumps
-from os import getpid, makedirs
-from os.path import exists, join
-from platform import node
-
-from azure.monitor.opentelemetry._constants import (
-    _CUSTOMER_IKEY,
-    _EXTENSION_VERSION,
-    _IS_DIAGNOSTICS_ENABLED,
-    _get_log_path,
-)
-from azure.monitor.opentelemetry._version import VERSION
-
-_MACHINE_NAME = node()
-_STATUS_LOG_PATH = _get_log_path(status_log_path=True)
-
-
-class AzureStatusLogger:
-    def _get_status_json(agent_initialized_successfully, pid, reason=None):
-        status_json = {
-            "AgentInitializedSuccessfully": agent_initialized_successfully,
-            "AppType": "python",
-            "MachineName": _MACHINE_NAME,
-            "PID": pid,
-            "SdkVersion": VERSION,
-            "Ikey": _CUSTOMER_IKEY,
-            "ExtensionVersion": _EXTENSION_VERSION,
-        }
-        if reason:
-            status_json["Reason"] = reason
-        return status_json
-
-    def log_status(agent_initialized_successfully, reason=None):
-        if _IS_DIAGNOSTICS_ENABLED and _STATUS_LOG_PATH:
-            pid = getpid()
-            status_json = AzureStatusLogger._get_status_json(
-                agent_initialized_successfully, pid, reason
-            )
-            if not exists(_STATUS_LOG_PATH):
-                makedirs(_STATUS_LOG_PATH)
-            # Change to be hostname and pid
-            status_logger_file_name = f"status_{_MACHINE_NAME}_{pid}.json"
-            with open(
-                join(_STATUS_LOG_PATH, status_logger_file_name), "w"
-            ) as f:
-                f.seek(0)
-                f.write(dumps(status_json))
-                f.truncate()
+# -------------------------------------------------------------------------
+# Copyright (c) Microsoft Corporation. All rights reserved.
+# Licensed under the MIT License. See License in the project root for
+# license information.
+# --------------------------------------------------------------------------
+
+from json import dumps
+from os import getpid, makedirs
+from os.path import exists, join
+from platform import node
+
+from azure.monitor.opentelemetry._constants import (
+    _CUSTOMER_IKEY,
+    _EXTENSION_VERSION,
+    _IS_DIAGNOSTICS_ENABLED,
+    _get_log_path,
+)
+from azure.monitor.opentelemetry._version import VERSION
+
+_MACHINE_NAME = node()
+_STATUS_LOG_PATH = _get_log_path(status_log_path=True)
+
+
+class AzureStatusLogger:
+    def _get_status_json(agent_initialized_successfully, pid, reason=None):
+        status_json = {
+            "AgentInitializedSuccessfully": agent_initialized_successfully,
+            "AppType": "python",
+            "MachineName": _MACHINE_NAME,
+            "PID": pid,
+            "SdkVersion": VERSION,
+            "Ikey": _CUSTOMER_IKEY,
+            "ExtensionVersion": _EXTENSION_VERSION,
+        }
+        if reason:
+            status_json["Reason"] = reason
+        return status_json
+
+    def log_status(agent_initialized_successfully, reason=None):
+        if _IS_DIAGNOSTICS_ENABLED and _STATUS_LOG_PATH:
+            pid = getpid()
+            status_json = AzureStatusLogger._get_status_json(
+                agent_initialized_successfully, pid, reason
+            )
+            if not exists(_STATUS_LOG_PATH):
+                makedirs(_STATUS_LOG_PATH)
+            # Change to be hostname and pid
+            status_logger_file_name = f"status_{_MACHINE_NAME}_{pid}.json"
+            with open(
+                join(_STATUS_LOG_PATH, status_logger_file_name), "w"
+            ) as f:
+                f.seek(0)
+                f.write(dumps(status_json))
+                f.truncate()
```

### Comparing `azure-monitor-opentelemetry-1.0.0b12/setup.py` & `azure-monitor-opentelemetry-1.0.0b9/setup.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,107 +1,104 @@
-#!/usr/bin/env python
-
-# -------------------------------------------------------------------------
-# Copyright (c) Microsoft Corporation. All rights reserved.
-# Licensed under the MIT License. See License.txt in the project root for
-# license information.
-# --------------------------------------------------------------------------
-
-
-import os
-import re
-
-from setuptools import find_packages, setup
-
-# Change the PACKAGE_NAME only to change folder and different name
-PACKAGE_NAME = "azure-monitor-opentelemetry"
-PACKAGE_PPRINT_NAME = "Azure Monitor Opentelemetry Distro"
-
-# a-b-c => a/b/c
-package_folder_path = PACKAGE_NAME.replace("-", "/")
-
-
-# azure v0.x is not compatible with this package
-# azure v0.x used to have a __version__ attribute (newer versions don't)
-try:
-    import azure
-
-    try:
-        ver = azure.__version__
-        raise Exception(
-            "This package is incompatible with azure=={}. ".format(ver)
-            + 'Uninstall it with "pip uninstall azure".'
-        )
-    except AttributeError:
-        pass
-except ImportError:
-    pass
-
-# Version extraction inspired from 'requests'
-with open(os.path.join(package_folder_path, "_version.py"), "r") as fd:
-    version = re.search(
-        r'^VERSION\s*=\s*[\'"]([^\'"]*)[\'"]', fd.read(), re.MULTILINE
-    ).group(1)
-
-if not version:
-    raise RuntimeError("Cannot find version information")
-
-setup(
-    name=PACKAGE_NAME,
-    version=version,
-    description="Microsoft {} Client Library for Python".format(
-        PACKAGE_PPRINT_NAME
-    ),
-    long_description=open("README.md", "r").read(),
-    long_description_content_type="text/markdown",
-    license="MIT License",
-    author="Microsoft Corporation",
-    author_email="ascl@microsoft.com",
-    url="https://github.com/microsoft/ApplicationInsights-Python/tree/main/azure-monitor-opentelemetry",
-    classifiers=[
-        "Development Status :: 4 - Beta",
-        "Programming Language :: Python",
-        "Programming Language :: Python :: 3",
-        "Programming Language :: Python :: 3.7",
-        "Programming Language :: Python :: 3.8",
-        "Programming Language :: Python :: 3.9",
-        "Programming Language :: Python :: 3.10",
-        "Programming Language :: Python :: 3.11",
-        "License :: OSI Approved :: MIT License",
-    ],
-    zip_safe=False,
-    packages=find_packages(
-        exclude=[
-            "tests",
-            "samples",
-            # Exclude packages that will be covered by PEP420 or nspkg
-            "azure",
-            "azure.monitor",
-        ]
-    ),
-    include_package_data=True,
-    package_data={
-        "pytyped": ["py.typed"],
-    },
-    python_requires=">=3.7",
-    install_requires=[
-        "azure-monitor-opentelemetry-exporter>=1.0.0b13",
-        "opentelemetry-instrumentation~=0.38b0",
-        "opentelemetry-instrumentation-django~=0.38b0",
-        "opentelemetry-instrumentation-fastapi~=0.38b0",
-        "opentelemetry-instrumentation-flask~=0.38b0",
-        "opentelemetry-instrumentation-psycopg2~=0.38b0",
-        "opentelemetry-instrumentation-requests~=0.38b0",
-        "opentelemetry-instrumentation-urllib~=0.38b0",
-        "opentelemetry-instrumentation-urllib3~=0.38b0",
-        "opentelemetry-api==1.17.0",
-        "opentelemetry-sdk==1.17.0",
-    ],
-    entry_points={
-        "opentelemetry_distro": [
-            "azure_monitor_opentelemetry_distro = azure.monitor.opentelemetry.autoinstrumentation._distro:AzureMonitorDistro"
-        ],
-        "opentelemetry_configurator": [
-            "azure_monitor_opentelemetry_configurator = azure.monitor.opentelemetry.autoinstrumentation._configurator:AzureMonitorConfigurator"
-        ],
-    },
-)
+#!/usr/bin/env python
+
+# -------------------------------------------------------------------------
+# Copyright (c) Microsoft Corporation. All rights reserved.
+# Licensed under the MIT License. See License.txt in the project root for
+# license information.
+# --------------------------------------------------------------------------
+
+
+import os
+import re
+
+from setuptools import find_packages, setup
+
+# Change the PACKAGE_NAME only to change folder and different name
+PACKAGE_NAME = "azure-monitor-opentelemetry"
+PACKAGE_PPRINT_NAME = "Azure Monitor Opentelemetry Distro"
+
+# a-b-c => a/b/c
+package_folder_path = PACKAGE_NAME.replace("-", "/")
+
+
+# azure v0.x is not compatible with this package
+# azure v0.x used to have a __version__ attribute (newer versions don't)
+try:
+    import azure
+
+    try:
+        ver = azure.__version__
+        raise Exception(
+            "This package is incompatible with azure=={}. ".format(ver)
+            + 'Uninstall it with "pip uninstall azure".'
+        )
+    except AttributeError:
+        pass
+except ImportError:
+    pass
+
+# Version extraction inspired from 'requests'
+with open(os.path.join(package_folder_path, "_version.py"), "r") as fd:
+    version = re.search(
+        r'^VERSION\s*=\s*[\'"]([^\'"]*)[\'"]', fd.read(), re.MULTILINE
+    ).group(1)
+
+if not version:
+    raise RuntimeError("Cannot find version information")
+
+setup(
+    name=PACKAGE_NAME,
+    version=version,
+    description="Microsoft {} Client Library for Python".format(
+        PACKAGE_PPRINT_NAME
+    ),
+    long_description=open("README.md", "r").read(),
+    long_description_content_type="text/markdown",
+    license="MIT License",
+    author="Microsoft Corporation",
+    author_email="ascl@microsoft.com",
+    url="https://github.com/microsoft/ApplicationInsights-Python/tree/main/azure-monitor-opentelemetry",
+    classifiers=[
+        "Development Status :: 4 - Beta",
+        "Programming Language :: Python",
+        "Programming Language :: Python :: 3",
+        "Programming Language :: Python :: 3.7",
+        "Programming Language :: Python :: 3.8",
+        "Programming Language :: Python :: 3.9",
+        "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
+        "License :: OSI Approved :: MIT License",
+    ],
+    zip_safe=False,
+    packages=find_packages(
+        exclude=[
+            "tests",
+            "samples",
+            # Exclude packages that will be covered by PEP420 or nspkg
+            "azure",
+            "azure.monitor",
+        ]
+    ),
+    include_package_data=True,
+    package_data={
+        "pytyped": ["py.typed"],
+    },
+    python_requires=">=3.7",
+    install_requires=[
+        "azure-monitor-opentelemetry-exporter>=1.0.0b12",
+        "opentelemetry-instrumentation~=0.36b0",
+        "opentelemetry-instrumentation-django~=0.36b0",
+        "opentelemetry-instrumentation-requests~=0.36b0",
+        "opentelemetry-instrumentation-flask~=0.36b0",
+        "opentelemetry-instrumentation-psycopg2~=0.36b0",
+        "opentelemetry-api==1.15.0",
+        "opentelemetry-sdk==1.15.0",
+    ],
+    entry_points={
+        "opentelemetry_distro": [
+            "azure_monitor_opentelemetry_distro = azure.monitor.opentelemetry.autoinstrumentation._distro:AzureMonitorDistro"
+        ],
+        "opentelemetry_configurator": [
+            "azure_monitor_opentelemetry_configurator = azure.monitor.opentelemetry.autoinstrumentation._configurator:AzureMonitorConfigurator"
+        ],
+    },
+)
```

### Comparing `azure-monitor-opentelemetry-1.0.0b12/tests/test_constants.py` & `azure-monitor-opentelemetry-1.0.0b9/tests/test_constants.py`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,149 +1,149 @@
-# -------------------------------------------------------------------------
-# Copyright (c) Microsoft Corporation. All rights reserved.
-# Licensed under the MIT License. See License in the project root for
-# license information.
-# --------------------------------------------------------------------------
-
-from importlib import reload
-from os import environ
-from unittest import TestCase
-from unittest.mock import patch
-
-from azure.monitor.opentelemetry import _constants
-
-TEST_VALUE = "TEST_VALUE"
-TEST_IKEY = "1234abcd-ab12-34cd-ab12-a23456abcdef"
-TEST_CONN_STR = f"InstrumentationKey={TEST_IKEY};IngestionEndpoint=https://centralus-2.in.applicationinsights.azure.com/;LiveEndpoint=https://centralus.livediagnostics.monitor.azure.com/"
-
-
-def clear_env_var(env_var):
-    if env_var in environ:
-        del environ[env_var]
-
-
-class TestConstants(TestCase):
-    @patch.dict(
-        "os.environ",
-        {"ApplicationInsightsAgent_EXTENSION_VERSION": TEST_VALUE},
-    )
-    def test_extension_version(self):
-        reload(_constants)
-        self.assertEqual(_constants._EXTENSION_VERSION, TEST_VALUE)
-
-    def test_extension_version_default(self):
-        clear_env_var("ApplicationInsightsAgent_EXTENSION_VERSION")
-        reload(_constants)
-        self.assertEqual(_constants._EXTENSION_VERSION, "disabled")
-
-    @patch.dict(
-        "os.environ", {"APPLICATIONINSIGHTS_CONNECTION_STRING": TEST_CONN_STR}
-    )
-    def test_ikey(self):
-        reload(_constants)
-        self.assertEqual(_constants._CUSTOMER_IKEY, TEST_IKEY)
-
-    def test_ikey_defaults(self):
-        clear_env_var("APPLICATIONINSIGHTS_CONNECTION_STRING")
-        reload(_constants)
-        self.assertEqual(_constants._CUSTOMER_IKEY, "unknown")
-
-    # TODO: Enabled when duplciate logging issue is solved
-    # @patch.dict(
-    #     "os.environ",
-    #     {"AZURE_MONITOR_OPENTELEMETRY_DISTRO_ENABLE_EXPORTER_DIAGNOSTICS": "True"},
-    # )
-    # def test_exporter_diagnostics_enabled(self):
-    #     reload(_constants)
-    #     self.assertTrue(_constants._EXPORTER_DIAGNOSTICS_ENABLED)
-
-    # def test_exporter_diagnostics_disabled(self):
-    #     clear_env_var("AZURE_MONITOR_OPENTELEMETRY_DISTRO_ENABLE_EXPORTER_DIAGNOSTICS")
-    #     reload(_constants)
-    #     self.assertFalse(_constants._EXPORTER_DIAGNOSTICS_ENABLED)
-
-    # @patch.dict(
-    #     "os.environ",
-    #     {"AZURE_MONITOR_OPENTELEMETRY_DISTRO_ENABLE_EXPORTER_DIAGNOSTICS": "foobar"},
-    # )
-    # def test_exporter_diagnostics_other(self):
-    #     reload(_constants)
-    #     self.assertFalse(_constants._EXPORTER_DIAGNOSTICS_ENABLED)
-
-    @patch.dict("os.environ", {"WEBSITE_SITE_NAME": TEST_VALUE})
-    def test_diagnostics_enabled(self):
-        reload(_constants)
-        self.assertTrue(_constants._IS_DIAGNOSTICS_ENABLED)
-
-    def test_diagnostics_disabled(self):
-        clear_env_var("WEBSITE_SITE_NAME")
-        reload(_constants)
-        self.assertFalse(_constants._IS_DIAGNOSTICS_ENABLED)
-
-    @patch(
-        "azure.monitor.opentelemetry._constants.platform.system",
-        return_value="Linux",
-    )
-    def test_log_path_linux(self, mock_system):
-        self.assertEqual(
-            _constants._get_log_path(), "/var/log/applicationinsights"
-        )
-
-    @patch(
-        "azure.monitor.opentelemetry._constants.platform.system",
-        return_value="Linux",
-    )
-    def test_status_log_path_linux(self, mock_system):
-        self.assertEqual(
-            _constants._get_log_path(status_log_path=True),
-            "/var/log/applicationinsights",
-        )
-
-    @patch(
-        "azure.monitor.opentelemetry._constants.platform.system",
-        return_value="Windows",
-    )
-    @patch("pathlib.Path.home", return_value="\\HOME\\DIR")
-    def test_log_path_windows(self, mock_system, mock_home):
-        self.assertEqual(
-            _constants._get_log_path(),
-            "\\HOME\\DIR\\LogFiles\\ApplicationInsights",
-        )
-
-    @patch(
-        "azure.monitor.opentelemetry._constants.platform.system",
-        return_value="Windows",
-    )
-    @patch("pathlib.Path.home", return_value="\\HOME\\DIR")
-    def test_status_log_path_windows(self, mock_system, mock_home):
-        self.assertEqual(
-            _constants._get_log_path(status_log_path=True),
-            "\\HOME\\DIR\\LogFiles\\ApplicationInsights\\status",
-        )
-
-    @patch(
-        "azure.monitor.opentelemetry._constants.platform.system",
-        return_value="Window",
-    )
-    def test_log_path_other(self, mock_platform):
-        self.assertIsNone(_constants._get_log_path())
-
-    @patch(
-        "azure.monitor.opentelemetry._constants.platform.system",
-        return_value="linux",
-    )
-    def test_status_log_path_other(self, mock_platform):
-        self.assertIsNone(_constants._get_log_path(status_log_path=True))
-
-    @patch.dict("os.environ", {"key": "value"})
-    def test_env_var_or_default(self):
-        self.assertEqual(_constants._env_var_or_default("key"), "value")
-
-    @patch.dict("os.environ", {})
-    def test_env_var_or_default_empty(self):
-        self.assertEqual(_constants._env_var_or_default("key"), "")
-
-    @patch.dict("os.environ", {})
-    def test_env_var_or_default_empty_with_defaults(self):
-        self.assertEqual(
-            _constants._env_var_or_default("key", default_val="value"), "value"
-        )
+# -------------------------------------------------------------------------
+# Copyright (c) Microsoft Corporation. All rights reserved.
+# Licensed under the MIT License. See License in the project root for
+# license information.
+# --------------------------------------------------------------------------
+
+from importlib import reload
+from os import environ
+from unittest import TestCase
+from unittest.mock import patch
+
+from azure.monitor.opentelemetry import _constants
+
+TEST_VALUE = "TEST_VALUE"
+TEST_IKEY = "1234abcd-ab12-34cd-ab12-a23456abcdef"
+TEST_CONN_STR = f"InstrumentationKey={TEST_IKEY};IngestionEndpoint=https://centralus-2.in.applicationinsights.azure.com/;LiveEndpoint=https://centralus.livediagnostics.monitor.azure.com/"
+
+
+def clear_env_var(env_var):
+    if env_var in environ:
+        del environ[env_var]
+
+
+class TestConstants(TestCase):
+    @patch.dict(
+        "os.environ",
+        {"ApplicationInsightsAgent_EXTENSION_VERSION": TEST_VALUE},
+    )
+    def test_extension_version(self):
+        reload(_constants)
+        self.assertEqual(_constants._EXTENSION_VERSION, TEST_VALUE)
+
+    def test_extension_version_default(self):
+        clear_env_var("ApplicationInsightsAgent_EXTENSION_VERSION")
+        reload(_constants)
+        self.assertEqual(_constants._EXTENSION_VERSION, "disabled")
+
+    @patch.dict(
+        "os.environ", {"APPLICATIONINSIGHTS_CONNECTION_STRING": TEST_CONN_STR}
+    )
+    def test_ikey(self):
+        reload(_constants)
+        self.assertEqual(_constants._CUSTOMER_IKEY, TEST_IKEY)
+
+    def test_ikey_defaults(self):
+        clear_env_var("APPLICATIONINSIGHTS_CONNECTION_STRING")
+        reload(_constants)
+        self.assertEqual(_constants._CUSTOMER_IKEY, "unknown")
+
+    # TODO: Enabled when duplciate logging issue is solved
+    # @patch.dict(
+    #     "os.environ",
+    #     {"AZURE_MONITOR_OPENTELEMETRY_DISTRO_ENABLE_EXPORTER_DIAGNOSTICS": "True"},
+    # )
+    # def test_exporter_diagnostics_enabled(self):
+    #     reload(_constants)
+    #     self.assertTrue(_constants._EXPORTER_DIAGNOSTICS_ENABLED)
+
+    # def test_exporter_diagnostics_disabled(self):
+    #     clear_env_var("AZURE_MONITOR_OPENTELEMETRY_DISTRO_ENABLE_EXPORTER_DIAGNOSTICS")
+    #     reload(_constants)
+    #     self.assertFalse(_constants._EXPORTER_DIAGNOSTICS_ENABLED)
+
+    # @patch.dict(
+    #     "os.environ",
+    #     {"AZURE_MONITOR_OPENTELEMETRY_DISTRO_ENABLE_EXPORTER_DIAGNOSTICS": "foobar"},
+    # )
+    # def test_exporter_diagnostics_other(self):
+    #     reload(_constants)
+    #     self.assertFalse(_constants._EXPORTER_DIAGNOSTICS_ENABLED)
+
+    @patch.dict("os.environ", {"WEBSITE_SITE_NAME": TEST_VALUE})
+    def test_diagnostics_enabled(self):
+        reload(_constants)
+        self.assertTrue(_constants._IS_DIAGNOSTICS_ENABLED)
+
+    def test_diagnostics_disabled(self):
+        clear_env_var("WEBSITE_SITE_NAME")
+        reload(_constants)
+        self.assertFalse(_constants._IS_DIAGNOSTICS_ENABLED)
+
+    @patch(
+        "azure.monitor.opentelemetry._constants.platform.system",
+        return_value="Linux",
+    )
+    def test_log_path_linux(self, mock_system):
+        self.assertEqual(
+            _constants._get_log_path(), "/var/log/applicationinsights"
+        )
+
+    @patch(
+        "azure.monitor.opentelemetry._constants.platform.system",
+        return_value="Linux",
+    )
+    def test_status_log_path_linux(self, mock_system):
+        self.assertEqual(
+            _constants._get_log_path(status_log_path=True),
+            "/var/log/applicationinsights",
+        )
+
+    @patch(
+        "azure.monitor.opentelemetry._constants.platform.system",
+        return_value="Windows",
+    )
+    @patch("pathlib.Path.home", return_value="\\HOME\\DIR")
+    def test_log_path_windows(self, mock_system, mock_home):
+        self.assertEqual(
+            _constants._get_log_path(),
+            "\\HOME\\DIR\\LogFiles\\ApplicationInsights",
+        )
+
+    @patch(
+        "azure.monitor.opentelemetry._constants.platform.system",
+        return_value="Windows",
+    )
+    @patch("pathlib.Path.home", return_value="\\HOME\\DIR")
+    def test_status_log_path_windows(self, mock_system, mock_home):
+        self.assertEqual(
+            _constants._get_log_path(status_log_path=True),
+            "\\HOME\\DIR\\LogFiles\\ApplicationInsights\\status",
+        )
+
+    @patch(
+        "azure.monitor.opentelemetry._constants.platform.system",
+        return_value="Window",
+    )
+    def test_log_path_other(self, mock_platform):
+        self.assertIsNone(_constants._get_log_path())
+
+    @patch(
+        "azure.monitor.opentelemetry._constants.platform.system",
+        return_value="linux",
+    )
+    def test_status_log_path_other(self, mock_platform):
+        self.assertIsNone(_constants._get_log_path(status_log_path=True))
+
+    @patch.dict("os.environ", {"key": "value"})
+    def test_env_var_or_default(self):
+        self.assertEqual(_constants._env_var_or_default("key"), "value")
+
+    @patch.dict("os.environ", {})
+    def test_env_var_or_default_empty(self):
+        self.assertEqual(_constants._env_var_or_default("key"), "")
+
+    @patch.dict("os.environ", {})
+    def test_env_var_or_default_empty_with_defaults(self):
+        self.assertEqual(
+            _constants._env_var_or_default("key", default_val="value"), "value"
+        )
```

