# Comparing `tmp/postman-sdk-0.0.8.tar.gz` & `tmp/postman-sdk-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "postman-sdk-0.0.8.tar", last modified: Fri Mar 24 11:47:08 2023, max compression
+gzip compressed data, was "/Users/piyush.daga@postman.com/PostmanProjects/postman-python-sdk/dist/.tmp-a1dnv2jg/postman-sdk-0.0.9.tar", last modified: Wed Mar 29 12:40:13 2023, max compression
```

## Comparing `postman-sdk-0.0.8.tar` & `postman-sdk-0.0.9.tar`

### file list

```diff
@@ -1,52 +1,52 @@
-drwxr-xr-x   0 kartikay.bansalpostman.com   (502) staff       (20)        0 2023-03-24 11:47:08.239043 postman-sdk-0.0.8/
--rw-r--r--   0 kartikay.bansalpostman.com   (502) staff       (20)      221 2023-03-23 09:54:21.000000 postman-sdk-0.0.8/LICENSE.md
--rw-r--r--   0 kartikay.bansalpostman.com   (502) staff       (20)     3621 2023-03-24 11:47:08.238753 postman-sdk-0.0.8/PKG-INFO
--rw-r--r--   0 kartikay.bansalpostman.com   (502) staff       (20)     3361 2023-03-24 10:59:11.000000 postman-sdk-0.0.8/README.md
--rw-r--r--   0 kartikay.bansalpostman.com   (502) staff       (20)     1034 2023-03-24 11:45:32.000000 postman-sdk-0.0.8/pyproject.toml
--rw-r--r--   0 kartikay.bansalpostman.com   (502) staff       (20)       38 2023-03-24 11:47:08.239130 postman-sdk-0.0.8/setup.cfg
-drwxr-xr-x   0 kartikay.bansalpostman.com   (502) staff       (20)        0 2023-03-24 11:47:08.225898 postman-sdk-0.0.8/src/
-drwxr-xr-x   0 kartikay.bansalpostman.com   (502) staff       (20)        0 2023-03-24 11:47:08.228513 postman-sdk-0.0.8/src/postman_sdk/
--rw-r--r--   0 kartikay.bansalpostman.com   (502) staff       (20)     3196 2023-03-23 09:54:21.000000 postman-sdk-0.0.8/src/postman_sdk/__init__.py
-drwxr-xr-x   0 kartikay.bansalpostman.com   (502) staff       (20)        0 2023-03-24 11:47:08.230128 postman-sdk-0.0.8/src/postman_sdk/exceptions/
--rw-r--r--   0 kartikay.bansalpostman.com   (502) staff       (20)      145 2023-03-23 09:54:21.000000 postman-sdk-0.0.8/src/postman_sdk/exceptions/__init__.py
-drwxr-xr-x   0 kartikay.bansalpostman.com   (502) staff       (20)        0 2023-03-24 11:47:08.230500 postman-sdk-0.0.8/src/postman_sdk/instrumentor/
--rw-r--r--   0 kartikay.bansalpostman.com   (502) staff       (20)      556 2023-03-23 09:54:21.000000 postman-sdk-0.0.8/src/postman_sdk/instrumentor/__init__.py
-drwxr-xr-x   0 kartikay.bansalpostman.com   (502) staff       (20)        0 2023-03-24 11:47:08.230870 postman-sdk-0.0.8/src/postman_sdk/instrumentor/base_instrumentation/
--rw-r--r--   0 kartikay.bansalpostman.com   (502) staff       (20)     2428 2023-03-23 09:54:21.000000 postman-sdk-0.0.8/src/postman_sdk/instrumentor/base_instrumentation/__init__.py
-drwxr-xr-x   0 kartikay.bansalpostman.com   (502) staff       (20)        0 2023-03-24 11:47:08.231189 postman-sdk-0.0.8/src/postman_sdk/instrumentor/postman_flask_instrumentation/
--rw-r--r--   0 kartikay.bansalpostman.com   (502) staff       (20)     3971 2023-03-23 09:54:21.000000 postman-sdk-0.0.8/src/postman_sdk/instrumentor/postman_flask_instrumentation/__init__.py
-drwxr-xr-x   0 kartikay.bansalpostman.com   (502) staff       (20)        0 2023-03-24 11:47:08.231512 postman-sdk-0.0.8/src/postman_sdk/instrumentor/postman_requests_instrumentation/
--rw-r--r--   0 kartikay.bansalpostman.com   (502) staff       (20)     2338 2023-03-23 09:54:21.000000 postman-sdk-0.0.8/src/postman_sdk/instrumentor/postman_requests_instrumentation/__init__.py
-drwxr-xr-x   0 kartikay.bansalpostman.com   (502) staff       (20)        0 2023-03-24 11:47:08.233276 postman-sdk-0.0.8/src/postman_sdk/model/
--rw-r--r--   0 kartikay.bansalpostman.com   (502) staff       (20)        0 2023-03-23 09:54:21.000000 postman-sdk-0.0.8/src/postman_sdk/model/__init__.py
--rw-r--r--   0 kartikay.bansalpostman.com   (502) staff       (20)     1423 2023-03-23 09:54:21.000000 postman-sdk-0.0.8/src/postman_sdk/model/base_config.py
--rw-r--r--   0 kartikay.bansalpostman.com   (502) staff       (20)      415 2023-03-23 09:54:21.000000 postman-sdk-0.0.8/src/postman_sdk/model/data_redaction.py
--rw-r--r--   0 kartikay.bansalpostman.com   (502) staff       (20)     1239 2023-03-23 09:54:21.000000 postman-sdk-0.0.8/src/postman_sdk/model/dynamic_model.py
--rw-r--r--   0 kartikay.bansalpostman.com   (502) staff       (20)      651 2023-03-23 09:54:21.000000 postman-sdk-0.0.8/src/postman_sdk/model/http.py
--rw-r--r--   0 kartikay.bansalpostman.com   (502) staff       (20)      450 2023-03-23 09:54:21.000000 postman-sdk-0.0.8/src/postman_sdk/model/semantic_attributes.py
-drwxr-xr-x   0 kartikay.bansalpostman.com   (502) staff       (20)        0 2023-03-24 11:47:08.234178 postman-sdk-0.0.8/src/postman_sdk/plugins/
--rw-r--r--   0 kartikay.bansalpostman.com   (502) staff       (20)     2297 2023-03-24 11:45:32.000000 postman-sdk-0.0.8/src/postman_sdk/plugins/__init__.py
--rw-r--r--   0 kartikay.bansalpostman.com   (502) staff       (20)     6728 2023-03-23 09:54:21.000000 postman-sdk-0.0.8/src/postman_sdk/plugins/data_redaction.py
--rw-r--r--   0 kartikay.bansalpostman.com   (502) staff       (20)     3189 2023-03-24 11:45:32.000000 postman-sdk-0.0.8/src/postman_sdk/plugins/data_truncation.py
-drwxr-xr-x   0 kartikay.bansalpostman.com   (502) staff       (20)        0 2023-03-24 11:47:08.235133 postman-sdk-0.0.8/src/postman_sdk/postman_otel/
--rw-r--r--   0 kartikay.bansalpostman.com   (502) staff       (20)        0 2023-03-23 09:54:21.000000 postman-sdk-0.0.8/src/postman_sdk/postman_otel/__init__.py
--rw-r--r--   0 kartikay.bansalpostman.com   (502) staff       (20)     6984 2023-03-24 11:45:32.000000 postman-sdk-0.0.8/src/postman_sdk/postman_otel/postman_exporter.py
--rw-r--r--   0 kartikay.bansalpostman.com   (502) staff       (20)        0 2023-03-23 09:54:21.000000 postman-sdk-0.0.8/src/postman_sdk/postman_otel/postman_span_processor.py
--rw-r--r--   0 kartikay.bansalpostman.com   (502) staff       (20)     5424 2023-03-23 09:54:21.000000 postman-sdk-0.0.8/src/postman_sdk/postman_otel/postman_tracer.py
-drwxr-xr-x   0 kartikay.bansalpostman.com   (502) staff       (20)        0 2023-03-24 11:47:08.237132 postman-sdk-0.0.8/src/postman_sdk/receiver_service/
--rw-r--r--   0 kartikay.bansalpostman.com   (502) staff       (20)      141 2023-03-23 09:54:21.000000 postman-sdk-0.0.8/src/postman_sdk/receiver_service/__init__.py
--rw-r--r--   0 kartikay.bansalpostman.com   (502) staff       (20)     1232 2023-03-23 09:54:21.000000 postman-sdk-0.0.8/src/postman_sdk/receiver_service/bootstrap.py
--rw-r--r--   0 kartikay.bansalpostman.com   (502) staff       (20)     1411 2023-03-23 09:54:21.000000 postman-sdk-0.0.8/src/postman_sdk/receiver_service/client.py
--rw-r--r--   0 kartikay.bansalpostman.com   (502) staff       (20)      335 2023-03-23 09:54:21.000000 postman-sdk-0.0.8/src/postman_sdk/receiver_service/config.py
--rw-r--r--   0 kartikay.bansalpostman.com   (502) staff       (20)     3448 2023-03-23 09:54:21.000000 postman-sdk-0.0.8/src/postman_sdk/receiver_service/health_check.py
-drwxr-xr-x   0 kartikay.bansalpostman.com   (502) staff       (20)        0 2023-03-24 11:47:08.238299 postman-sdk-0.0.8/src/postman_sdk/util/
--rw-r--r--   0 kartikay.bansalpostman.com   (502) staff       (20)        0 2023-03-23 09:54:21.000000 postman-sdk-0.0.8/src/postman_sdk/util/__init__.py
--rw-r--r--   0 kartikay.bansalpostman.com   (502) staff       (20)      719 2023-03-23 09:54:21.000000 postman-sdk-0.0.8/src/postman_sdk/util/constants.py
--rw-r--r--   0 kartikay.bansalpostman.com   (502) staff       (20)     2605 2023-03-23 09:54:21.000000 postman-sdk-0.0.8/src/postman_sdk/util/helper.py
--rw-r--r--   0 kartikay.bansalpostman.com   (502) staff       (20)      546 2023-03-23 09:54:21.000000 postman-sdk-0.0.8/src/postman_sdk/util/logger.py
-drwxr-xr-x   0 kartikay.bansalpostman.com   (502) staff       (20)        0 2023-03-24 11:47:08.229858 postman-sdk-0.0.8/src/postman_sdk.egg-info/
--rw-r--r--   0 kartikay.bansalpostman.com   (502) staff       (20)     3621 2023-03-24 11:47:08.000000 postman-sdk-0.0.8/src/postman_sdk.egg-info/PKG-INFO
--rw-r--r--   0 kartikay.bansalpostman.com   (502) staff       (20)     1437 2023-03-24 11:47:08.000000 postman-sdk-0.0.8/src/postman_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 kartikay.bansalpostman.com   (502) staff       (20)        1 2023-03-24 11:47:08.000000 postman-sdk-0.0.8/src/postman_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 kartikay.bansalpostman.com   (502) staff       (20)      586 2023-03-24 11:47:08.000000 postman-sdk-0.0.8/src/postman_sdk.egg-info/requires.txt
--rw-r--r--   0 kartikay.bansalpostman.com   (502) staff       (20)       12 2023-03-24 11:47:08.000000 postman-sdk-0.0.8/src/postman_sdk.egg-info/top_level.txt
+drwxr-xr-x   0 piyush.daga@postman.com   (502) staff       (20)        0 2023-03-29 12:40:13.000000 postman-sdk-0.0.9/
+-rw-r--r--   0 piyush.daga@postman.com   (502) staff       (20)      221 2023-03-23 06:51:06.000000 postman-sdk-0.0.9/LICENSE.md
+-rw-r--r--   0 piyush.daga@postman.com   (502) staff       (20)     3880 2023-03-29 12:40:13.000000 postman-sdk-0.0.9/PKG-INFO
+-rw-r--r--   0 piyush.daga@postman.com   (502) staff       (20)     3620 2023-03-29 12:35:58.000000 postman-sdk-0.0.9/README.md
+-rw-r--r--   0 piyush.daga@postman.com   (502) staff       (20)     1034 2023-03-29 12:39:39.000000 postman-sdk-0.0.9/pyproject.toml
+-rw-r--r--   0 piyush.daga@postman.com   (502) staff       (20)       38 2023-03-29 12:40:13.000000 postman-sdk-0.0.9/setup.cfg
+drwxr-xr-x   0 piyush.daga@postman.com   (502) staff       (20)        0 2023-03-29 12:40:13.000000 postman-sdk-0.0.9/src/
+drwxr-xr-x   0 piyush.daga@postman.com   (502) staff       (20)        0 2023-03-29 12:40:13.000000 postman-sdk-0.0.9/src/postman_sdk/
+-rw-r--r--   0 piyush.daga@postman.com   (502) staff       (20)     3358 2023-03-29 12:35:58.000000 postman-sdk-0.0.9/src/postman_sdk/__init__.py
+drwxr-xr-x   0 piyush.daga@postman.com   (502) staff       (20)        0 2023-03-29 12:40:13.000000 postman-sdk-0.0.9/src/postman_sdk/exceptions/
+-rw-r--r--   0 piyush.daga@postman.com   (502) staff       (20)      145 2023-03-22 19:19:48.000000 postman-sdk-0.0.9/src/postman_sdk/exceptions/__init__.py
+drwxr-xr-x   0 piyush.daga@postman.com   (502) staff       (20)        0 2023-03-29 12:40:13.000000 postman-sdk-0.0.9/src/postman_sdk/instrumentor/
+-rw-r--r--   0 piyush.daga@postman.com   (502) staff       (20)      556 2023-03-22 19:19:48.000000 postman-sdk-0.0.9/src/postman_sdk/instrumentor/__init__.py
+drwxr-xr-x   0 piyush.daga@postman.com   (502) staff       (20)        0 2023-03-29 12:40:13.000000 postman-sdk-0.0.9/src/postman_sdk/instrumentor/base_instrumentation/
+-rw-r--r--   0 piyush.daga@postman.com   (502) staff       (20)     2428 2023-03-22 19:19:48.000000 postman-sdk-0.0.9/src/postman_sdk/instrumentor/base_instrumentation/__init__.py
+drwxr-xr-x   0 piyush.daga@postman.com   (502) staff       (20)        0 2023-03-29 12:40:13.000000 postman-sdk-0.0.9/src/postman_sdk/instrumentor/postman_flask_instrumentation/
+-rw-r--r--   0 piyush.daga@postman.com   (502) staff       (20)     3971 2023-03-22 19:19:48.000000 postman-sdk-0.0.9/src/postman_sdk/instrumentor/postman_flask_instrumentation/__init__.py
+drwxr-xr-x   0 piyush.daga@postman.com   (502) staff       (20)        0 2023-03-29 12:40:13.000000 postman-sdk-0.0.9/src/postman_sdk/instrumentor/postman_requests_instrumentation/
+-rw-r--r--   0 piyush.daga@postman.com   (502) staff       (20)     2338 2023-03-22 19:19:48.000000 postman-sdk-0.0.9/src/postman_sdk/instrumentor/postman_requests_instrumentation/__init__.py
+drwxr-xr-x   0 piyush.daga@postman.com   (502) staff       (20)        0 2023-03-29 12:40:13.000000 postman-sdk-0.0.9/src/postman_sdk/model/
+-rw-r--r--   0 piyush.daga@postman.com   (502) staff       (20)        0 2023-03-22 19:19:48.000000 postman-sdk-0.0.9/src/postman_sdk/model/__init__.py
+-rw-r--r--   0 piyush.daga@postman.com   (502) staff       (20)     1423 2023-03-23 06:51:06.000000 postman-sdk-0.0.9/src/postman_sdk/model/base_config.py
+-rw-r--r--   0 piyush.daga@postman.com   (502) staff       (20)      435 2023-03-29 12:35:58.000000 postman-sdk-0.0.9/src/postman_sdk/model/data_redaction.py
+-rw-r--r--   0 piyush.daga@postman.com   (502) staff       (20)     1239 2023-03-22 19:19:48.000000 postman-sdk-0.0.9/src/postman_sdk/model/dynamic_model.py
+-rw-r--r--   0 piyush.daga@postman.com   (502) staff       (20)      651 2023-03-22 19:19:48.000000 postman-sdk-0.0.9/src/postman_sdk/model/http.py
+-rw-r--r--   0 piyush.daga@postman.com   (502) staff       (20)      450 2023-03-22 19:19:48.000000 postman-sdk-0.0.9/src/postman_sdk/model/semantic_attributes.py
+drwxr-xr-x   0 piyush.daga@postman.com   (502) staff       (20)        0 2023-03-29 12:40:13.000000 postman-sdk-0.0.9/src/postman_sdk/plugins/
+-rw-r--r--   0 piyush.daga@postman.com   (502) staff       (20)     2440 2023-03-29 12:35:58.000000 postman-sdk-0.0.9/src/postman_sdk/plugins/__init__.py
+-rw-r--r--   0 piyush.daga@postman.com   (502) staff       (20)     7112 2023-03-29 12:35:58.000000 postman-sdk-0.0.9/src/postman_sdk/plugins/data_redaction.py
+-rw-r--r--   0 piyush.daga@postman.com   (502) staff       (20)     3189 2023-03-29 12:35:58.000000 postman-sdk-0.0.9/src/postman_sdk/plugins/data_truncation.py
+drwxr-xr-x   0 piyush.daga@postman.com   (502) staff       (20)        0 2023-03-29 12:40:13.000000 postman-sdk-0.0.9/src/postman_sdk/postman_otel/
+-rw-r--r--   0 piyush.daga@postman.com   (502) staff       (20)        0 2023-03-22 19:19:48.000000 postman-sdk-0.0.9/src/postman_sdk/postman_otel/__init__.py
+-rw-r--r--   0 piyush.daga@postman.com   (502) staff       (20)     6984 2023-03-29 12:35:58.000000 postman-sdk-0.0.9/src/postman_sdk/postman_otel/postman_exporter.py
+-rw-r--r--   0 piyush.daga@postman.com   (502) staff       (20)        0 2023-03-22 19:19:48.000000 postman-sdk-0.0.9/src/postman_sdk/postman_otel/postman_span_processor.py
+-rw-r--r--   0 piyush.daga@postman.com   (502) staff       (20)     5424 2023-03-23 06:51:06.000000 postman-sdk-0.0.9/src/postman_sdk/postman_otel/postman_tracer.py
+drwxr-xr-x   0 piyush.daga@postman.com   (502) staff       (20)        0 2023-03-29 12:40:13.000000 postman-sdk-0.0.9/src/postman_sdk/receiver_service/
+-rw-r--r--   0 piyush.daga@postman.com   (502) staff       (20)      141 2023-03-22 19:19:48.000000 postman-sdk-0.0.9/src/postman_sdk/receiver_service/__init__.py
+-rw-r--r--   0 piyush.daga@postman.com   (502) staff       (20)     1232 2023-03-22 19:19:48.000000 postman-sdk-0.0.9/src/postman_sdk/receiver_service/bootstrap.py
+-rw-r--r--   0 piyush.daga@postman.com   (502) staff       (20)     1411 2023-03-22 19:19:48.000000 postman-sdk-0.0.9/src/postman_sdk/receiver_service/client.py
+-rw-r--r--   0 piyush.daga@postman.com   (502) staff       (20)      335 2023-03-22 19:19:48.000000 postman-sdk-0.0.9/src/postman_sdk/receiver_service/config.py
+-rw-r--r--   0 piyush.daga@postman.com   (502) staff       (20)     3448 2023-03-22 19:19:48.000000 postman-sdk-0.0.9/src/postman_sdk/receiver_service/health_check.py
+drwxr-xr-x   0 piyush.daga@postman.com   (502) staff       (20)        0 2023-03-29 12:40:13.000000 postman-sdk-0.0.9/src/postman_sdk/util/
+-rw-r--r--   0 piyush.daga@postman.com   (502) staff       (20)        0 2023-03-22 19:19:48.000000 postman-sdk-0.0.9/src/postman_sdk/util/__init__.py
+-rw-r--r--   0 piyush.daga@postman.com   (502) staff       (20)      719 2023-03-22 19:19:48.000000 postman-sdk-0.0.9/src/postman_sdk/util/constants.py
+-rw-r--r--   0 piyush.daga@postman.com   (502) staff       (20)     2605 2023-03-22 19:19:48.000000 postman-sdk-0.0.9/src/postman_sdk/util/helper.py
+-rw-r--r--   0 piyush.daga@postman.com   (502) staff       (20)      546 2023-03-22 19:19:48.000000 postman-sdk-0.0.9/src/postman_sdk/util/logger.py
+drwxr-xr-x   0 piyush.daga@postman.com   (502) staff       (20)        0 2023-03-29 12:40:13.000000 postman-sdk-0.0.9/src/postman_sdk.egg-info/
+-rw-r--r--   0 piyush.daga@postman.com   (502) staff       (20)     3880 2023-03-29 12:40:13.000000 postman-sdk-0.0.9/src/postman_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 piyush.daga@postman.com   (502) staff       (20)     1437 2023-03-29 12:40:13.000000 postman-sdk-0.0.9/src/postman_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 piyush.daga@postman.com   (502) staff       (20)        1 2023-03-29 12:40:13.000000 postman-sdk-0.0.9/src/postman_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 piyush.daga@postman.com   (502) staff       (20)      586 2023-03-29 12:40:13.000000 postman-sdk-0.0.9/src/postman_sdk.egg-info/requires.txt
+-rw-r--r--   0 piyush.daga@postman.com   (502) staff       (20)       12 2023-03-29 12:40:13.000000 postman-sdk-0.0.9/src/postman_sdk.egg-info/top_level.txt
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive
+POSIX tar archive (GNU)
```

### Comparing `postman-sdk-0.0.8/PKG-INFO` & `postman-sdk-0.0.9/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: postman-sdk
-Version: 0.0.8
+Version: 0.0.9
 Summary: Postman SDK
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE.md
 
@@ -79,21 +79,27 @@
             "type": "int"
         }
     }
     ```
   - Type: ```boolean```
   - Default: ```True```
 
-- **redact_sensitive_data**: Redact sensitive data such as api_keys and auth tokens, before they leave the sdk. This is **enabled** by default. But **NO** rules are set.
+- **redact_sensitive_data**: Redact sensitive data such as api_keys and auth tokens, before they leave the sdk. This is **enabled** by default, and these are the redaction rules set:
+  ```python
+    {
+        "pm_postman_api_key": r"PMAK-[a-f0-9]{24}-[a-f0-9]{34}",
+        "pm_postman_access_key": r"PMAT-[0-9a-z]{26}",
+    }
+    ```
   - Example:
     ```python
     {
     "redact_sensitive_data": {
-        "enable": True(default),
-        "rules": {
+        "enable": True(default), 
+        "rules": { # This is optional, if the `rules` key is not passed, the default set of rules will be used.
             "<rule name>": "<regex to match the rule>", # such as -
             "basic_auth": r"\b[A-Za-z0-9._%+-]+@[A-Za-z0-9.-]+\.[A-Z|a-z]{2,7}\b",
             },
         }
     }
     ```
   - Type: ```object```
```

### Comparing `postman-sdk-0.0.8/README.md` & `postman-sdk-0.0.9/src/postman_sdk.egg-info/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,7 +1,17 @@
+Metadata-Version: 2.1
+Name: postman-sdk
+Version: 0.0.9
+Summary: Postman SDK
+Classifier: Programming Language :: Python :: 3
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.7
+Description-Content-Type: text/markdown
+License-File: LICENSE.md
+
 ## About
 
 This SDK instruments Python web frameworks to capture http requests and auto-generates Postman Live Collections.
 
 The minimum supported version for Python is: 3.7+.
 
 
@@ -69,21 +79,27 @@
             "type": "int"
         }
     }
     ```
   - Type: ```boolean```
   - Default: ```True```
 
-- **redact_sensitive_data**: Redact sensitive data such as api_keys and auth tokens, before they leave the sdk. This is **enabled** by default. But **NO** rules are set.
+- **redact_sensitive_data**: Redact sensitive data such as api_keys and auth tokens, before they leave the sdk. This is **enabled** by default, and these are the redaction rules set:
+  ```python
+    {
+        "pm_postman_api_key": r"PMAK-[a-f0-9]{24}-[a-f0-9]{34}",
+        "pm_postman_access_key": r"PMAT-[0-9a-z]{26}",
+    }
+    ```
   - Example:
     ```python
     {
     "redact_sensitive_data": {
-        "enable": True(default),
-        "rules": {
+        "enable": True(default), 
+        "rules": { # This is optional, if the `rules` key is not passed, the default set of rules will be used.
             "<rule name>": "<regex to match the rule>", # such as -
             "basic_auth": r"\b[A-Za-z0-9._%+-]+@[A-Za-z0-9.-]+\.[A-Z|a-z]{2,7}\b",
             },
         }
     }
     ```
   - Type: ```object```
```

### Comparing `postman-sdk-0.0.8/pyproject.toml` & `postman-sdk-0.0.9/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [tool.black]
 include = '/src\/.*\.py'
 
 [project]
 name = "postman-sdk"
-version = "0.0.8"
+version = "0.0.9"
 description = "Postman SDK"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
     "Programming Language :: Python :: 3",
     "Operating System :: OS Independent",
 ]
```

### Comparing `postman-sdk-0.0.8/src/postman_sdk/__init__.py` & `postman-sdk-0.0.9/src/postman_sdk/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -44,15 +44,20 @@
                     "type": "int"
                 }
             }
 
     redact_sensitive_data: Optional[DataRedactionConfig]
         Redact sensitive data such as api_keys and auth tokens, before they leave the sdk.
 
-        This is **enabled** by default. But **NO** rules are set.
+        This is **enabled** by default, and these are the redaction rules set:
+
+        {
+            "pm_postman_api_key": r"PMAK-[a-f0-9]{24}-[a-f0-9]{34}",
+            "pm_postman_access_key": r"PMAT-[0-9a-z]{26}",
+        }
 
         Example:
             {
                 "redact_sensitive_data": {
                     "enable": True (default)
                     "rules": {
                         "<rule name>": "<regex to match the rule>", such as
```

### Comparing `postman-sdk-0.0.8/src/postman_sdk/instrumentor/__init__.py` & `postman-sdk-0.0.9/src/postman_sdk/instrumentor/__init__.py`

 * *Files identical despite different names*

### Comparing `postman-sdk-0.0.8/src/postman_sdk/instrumentor/base_instrumentation/__init__.py` & `postman-sdk-0.0.9/src/postman_sdk/instrumentor/base_instrumentation/__init__.py`

 * *Files identical despite different names*

### Comparing `postman-sdk-0.0.8/src/postman_sdk/instrumentor/postman_flask_instrumentation/__init__.py` & `postman-sdk-0.0.9/src/postman_sdk/instrumentor/postman_flask_instrumentation/__init__.py`

 * *Files identical despite different names*

### Comparing `postman-sdk-0.0.8/src/postman_sdk/instrumentor/postman_requests_instrumentation/__init__.py` & `postman-sdk-0.0.9/src/postman_sdk/instrumentor/postman_requests_instrumentation/__init__.py`

 * *Files identical despite different names*

### Comparing `postman-sdk-0.0.8/src/postman_sdk/model/base_config.py` & `postman-sdk-0.0.9/src/postman_sdk/model/base_config.py`

 * *Files identical despite different names*

### Comparing `postman-sdk-0.0.8/src/postman_sdk/model/dynamic_model.py` & `postman-sdk-0.0.9/src/postman_sdk/model/dynamic_model.py`

 * *Files identical despite different names*

### Comparing `postman-sdk-0.0.8/src/postman_sdk/model/http.py` & `postman-sdk-0.0.9/src/postman_sdk/model/http.py`

 * *Files identical despite different names*

### Comparing `postman-sdk-0.0.8/src/postman_sdk/plugins/__init__.py` & `postman-sdk-0.0.9/src/postman_sdk/plugins/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,14 +7,19 @@
     DEFAULT_TRUNCATION_MAX_DEPTH,
 )
 
 HTTP_REQUEST_KEYS = {"uri": "http.target", "method": "http.method"}
 
 DEFAULT_REDACTION_REPLACEMENT_STRING = "************"
 
+DEFAULT_REDACTION_RULES = {
+    "pm_postman_api_key": r"PMAK-[a-f0-9]{24}-[a-f0-9]{34}",
+    "pm_postman_access_key": r"PMAT-[0-9a-z]{26}",
+}
+
 HTTP_ATTRIBUTES__REQUEST_REDACTION_MAP = {
     "body": {
         "attribute_key": "http.request.body",
         "redaction_function": "redact_body_data",
     },
     "headers": {
         "attribute_key": "http.request.headers",
```

### Comparing `postman-sdk-0.0.8/src/postman_sdk/plugins/data_redaction.py` & `postman-sdk-0.0.9/src/postman_sdk/plugins/data_redaction.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 """
 Data redaction module, will apply redaction on the values of attribute keys by the given reg rules.
 """
 import json
 import re
+from copy import deepcopy
 from json.decoder import JSONDecodeError
 
 from opentelemetry.util.types import Attributes
 
 from postman_sdk.model.data_redaction import (
     DataRedactionConfig,
 )
@@ -28,15 +29,24 @@
 
     def __compile_rules(self, rules):
         """
         Method to parse rules and index
         :param rules:
         :return:
         """
-        for rl_name, regex_rule_compiled in rules.get_items():
+        # Preventing circular import.
+        from postman_sdk.plugins import DEFAULT_REDACTION_RULES
+
+        combined_rules =  deepcopy(DEFAULT_REDACTION_RULES)
+
+        if hasattr(rules, "__root__"):
+            # In case of conflict, the items from rules will override the DEFAULT_REDACTION_RULES.
+            combined_rules.update(rules.__root__)
+
+        for rl_name, regex_rule_compiled in combined_rules.items():
             self.regex_redaction[rl_name] = re.compile(regex_rule_compiled, re.DOTALL)
 
     def run(self, span_attributes: Attributes):
         """
         Method to run the redaction.
         :param span_attributes:
         :return: span_attributes
```

### Comparing `postman-sdk-0.0.8/src/postman_sdk/plugins/data_truncation.py` & `postman-sdk-0.0.9/src/postman_sdk/plugins/data_truncation.py`

 * *Files identical despite different names*

### Comparing `postman-sdk-0.0.8/src/postman_sdk/postman_otel/postman_exporter.py` & `postman-sdk-0.0.9/src/postman_sdk/postman_otel/postman_exporter.py`

 * *Files identical despite different names*

### Comparing `postman-sdk-0.0.8/src/postman_sdk/postman_otel/postman_tracer.py` & `postman-sdk-0.0.9/src/postman_sdk/postman_otel/postman_tracer.py`

 * *Files identical despite different names*

### Comparing `postman-sdk-0.0.8/src/postman_sdk/receiver_service/bootstrap.py` & `postman-sdk-0.0.9/src/postman_sdk/receiver_service/bootstrap.py`

 * *Files identical despite different names*

### Comparing `postman-sdk-0.0.8/src/postman_sdk/receiver_service/client.py` & `postman-sdk-0.0.9/src/postman_sdk/receiver_service/client.py`

 * *Files identical despite different names*

### Comparing `postman-sdk-0.0.8/src/postman_sdk/receiver_service/health_check.py` & `postman-sdk-0.0.9/src/postman_sdk/receiver_service/health_check.py`

 * *Files identical despite different names*

### Comparing `postman-sdk-0.0.8/src/postman_sdk/util/constants.py` & `postman-sdk-0.0.9/src/postman_sdk/util/constants.py`

 * *Files identical despite different names*

### Comparing `postman-sdk-0.0.8/src/postman_sdk/util/helper.py` & `postman-sdk-0.0.9/src/postman_sdk/util/helper.py`

 * *Files identical despite different names*

### Comparing `postman-sdk-0.0.8/src/postman_sdk/util/logger.py` & `postman-sdk-0.0.9/src/postman_sdk/util/logger.py`

 * *Files identical despite different names*

### Comparing `postman-sdk-0.0.8/src/postman_sdk.egg-info/PKG-INFO` & `postman-sdk-0.0.9/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -1,17 +1,7 @@
-Metadata-Version: 2.1
-Name: postman-sdk
-Version: 0.0.8
-Summary: Postman SDK
-Classifier: Programming Language :: Python :: 3
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-License-File: LICENSE.md
-
 ## About
 
 This SDK instruments Python web frameworks to capture http requests and auto-generates Postman Live Collections.
 
 The minimum supported version for Python is: 3.7+.
 
 
@@ -79,21 +69,27 @@
             "type": "int"
         }
     }
     ```
   - Type: ```boolean```
   - Default: ```True```
 
-- **redact_sensitive_data**: Redact sensitive data such as api_keys and auth tokens, before they leave the sdk. This is **enabled** by default. But **NO** rules are set.
+- **redact_sensitive_data**: Redact sensitive data such as api_keys and auth tokens, before they leave the sdk. This is **enabled** by default, and these are the redaction rules set:
+  ```python
+    {
+        "pm_postman_api_key": r"PMAK-[a-f0-9]{24}-[a-f0-9]{34}",
+        "pm_postman_access_key": r"PMAT-[0-9a-z]{26}",
+    }
+    ```
   - Example:
     ```python
     {
     "redact_sensitive_data": {
-        "enable": True(default),
-        "rules": {
+        "enable": True(default), 
+        "rules": { # This is optional, if the `rules` key is not passed, the default set of rules will be used.
             "<rule name>": "<regex to match the rule>", # such as -
             "basic_auth": r"\b[A-Za-z0-9._%+-]+@[A-Za-z0-9.-]+\.[A-Z|a-z]{2,7}\b",
             },
         }
     }
     ```
   - Type: ```object```
```

### Comparing `postman-sdk-0.0.8/src/postman_sdk.egg-info/SOURCES.txt` & `postman-sdk-0.0.9/src/postman_sdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `postman-sdk-0.0.8/src/postman_sdk.egg-info/requires.txt` & `postman-sdk-0.0.9/src/postman_sdk.egg-info/requires.txt`

 * *Files identical despite different names*

