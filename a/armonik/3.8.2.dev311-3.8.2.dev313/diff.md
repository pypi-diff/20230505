# Comparing `tmp/armonik-3.8.2.dev311.tar.gz` & `tmp/armonik-3.8.2.dev313.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "armonik-3.8.2.dev311.tar", last modified: Fri May  5 14:17:10 2023, max compression
+gzip compressed data, was "armonik-3.8.2.dev313.tar", last modified: Fri May  5 15:29:55 2023, max compression
```

## Comparing `armonik-3.8.2.dev311.tar` & `armonik-3.8.2.dev313.tar`

### file list

```diff
@@ -1,108 +1,108 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 14:17:10.804678 armonik-3.8.2.dev311/
--rw-r--r--   0 runner    (1001) docker     (123)     2163 2023-05-05 14:17:10.804678 armonik-3.8.2.dev311/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1736 2023-05-05 14:16:53.000000 armonik-3.8.2.dev311/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1026 2023-05-05 14:16:53.000000 armonik-3.8.2.dev311/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-05 14:17:10.804678 armonik-3.8.2.dev311/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 14:17:10.792678 armonik-3.8.2.dev311/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 14:17:10.792678 armonik-3.8.2.dev311/src/armonik/
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-05-05 14:16:53.000000 armonik-3.8.2.dev311/src/armonik/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      123 2023-05-05 14:17:04.000000 armonik-3.8.2.dev311/src/armonik/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 14:17:10.792678 armonik-3.8.2.dev311/src/armonik/client/
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-05-05 14:16:53.000000 armonik-3.8.2.dev311/src/armonik/client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12657 2023-05-05 14:16:53.000000 armonik-3.8.2.dev311/src/armonik/client/submitter.py
--rw-r--r--   0 runner    (1001) docker     (123)      782 2023-05-05 14:16:53.000000 armonik-3.8.2.dev311/src/armonik/client/tasks.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 14:17:10.792678 armonik-3.8.2.dev311/src/armonik/common/
--rw-r--r--   0 runner    (1001) docker     (123)      267 2023-05-05 14:16:53.000000 armonik-3.8.2.dev311/src/armonik/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      814 2023-05-05 14:16:53.000000 armonik-3.8.2.dev311/src/armonik/common/enumwrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     3714 2023-05-05 14:16:53.000000 armonik-3.8.2.dev311/src/armonik/common/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     6263 2023-05-05 14:16:53.000000 armonik-3.8.2.dev311/src/armonik/common/objects.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 14:17:10.792678 armonik-3.8.2.dev311/src/armonik/protogen/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 14:17:10.796678 armonik-3.8.2.dev311/src/armonik/protogen/client/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 14:17:04.000000 armonik-3.8.2.dev311/src/armonik/protogen/client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1572 2023-05-05 14:17:04.000000 armonik-3.8.2.dev311/src/armonik/protogen/client/applications_service_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      208 2023-05-05 14:17:04.000000 armonik-3.8.2.dev311/src/armonik/protogen/client/applications_service_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     4483 2023-05-05 14:17:04.000000 armonik-3.8.2.dev311/src/armonik/protogen/client/applications_service_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1321 2023-05-05 14:17:04.000000 armonik-3.8.2.dev311/src/armonik/protogen/client/auth_service_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      192 2023-05-05 14:17:04.000000 armonik-3.8.2.dev311/src/armonik/protogen/client/auth_service_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2581 2023-05-05 14:17:04.000000 armonik-3.8.2.dev311/src/armonik/protogen/client/auth_service_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1320 2023-05-05 14:17:04.000000 armonik-3.8.2.dev311/src/armonik/protogen/client/events_service_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      196 2023-05-05 14:17:04.000000 armonik-3.8.2.dev311/src/armonik/protogen/client/events_service_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2739 2023-05-05 14:17:04.000000 armonik-3.8.2.dev311/src/armonik/protogen/client/events_service_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1519 2023-05-05 14:17:04.000000 armonik-3.8.2.dev311/src/armonik/protogen/client/partitions_service_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      204 2023-05-05 14:17:04.000000 armonik-3.8.2.dev311/src/armonik/protogen/client/partitions_service_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     4373 2023-05-05 14:17:04.000000 armonik-3.8.2.dev311/src/armonik/protogen/client/partitions_service_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     2493 2023-05-05 14:17:04.000000 armonik-3.8.2.dev311/src/armonik/protogen/client/results_service_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      247 2023-05-05 14:17:04.000000 armonik-3.8.2.dev311/src/armonik/protogen/client/results_service_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    14560 2023-05-05 14:17:04.000000 armonik-3.8.2.dev311/src/armonik/protogen/client/results_service_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1779 2023-05-05 14:17:04.000000 armonik-3.8.2.dev311/src/armonik/protogen/client/sessions_service_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      200 2023-05-05 14:17:04.000000 armonik-3.8.2.dev311/src/armonik/protogen/client/sessions_service_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     7535 2023-05-05 14:17:04.000000 armonik-3.8.2.dev311/src/armonik/protogen/client/sessions_service_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     3571 2023-05-05 14:17:04.000000 armonik-3.8.2.dev311/src/armonik/protogen/client/submitter_service_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      251 2023-05-05 14:17:04.000000 armonik-3.8.2.dev311/src/armonik/protogen/client/submitter_service_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    27332 2023-05-05 14:17:04.000000 armonik-3.8.2.dev311/src/armonik/protogen/client/submitter_service_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     2081 2023-05-05 14:17:04.000000 armonik-3.8.2.dev311/src/armonik/protogen/client/tasks_service_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      194 2023-05-05 14:17:04.000000 armonik-3.8.2.dev311/src/armonik/protogen/client/tasks_service_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    12105 2023-05-05 14:17:04.000000 armonik-3.8.2.dev311/src/armonik/protogen/client/tasks_service_pb2_grpc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 14:17:10.800678 armonik-3.8.2.dev311/src/armonik/protogen/common/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 14:17:04.000000 armonik-3.8.2.dev311/src/armonik/protogen/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8764 2023-05-05 14:17:04.000000 armonik-3.8.2.dev311/src/armonik/protogen/common/agent_common_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    13431 2023-05-05 14:17:04.000000 armonik-3.8.2.dev311/src/armonik/protogen/common/agent_common_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-05 14:17:04.000000 armonik-3.8.2.dev311/src/armonik/protogen/common/agent_common_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     3802 2023-05-05 14:17:04.000000 armonik-3.8.2.dev311/src/armonik/protogen/common/applications_common_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     4563 2023-05-05 14:17:04.000000 armonik-3.8.2.dev311/src/armonik/protogen/common/applications_common_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-05 14:17:04.000000 armonik-3.8.2.dev311/src/armonik/protogen/common/applications_common_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1484 2023-05-05 14:17:04.000000 armonik-3.8.2.dev311/src/armonik/protogen/common/auth_common_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     1145 2023-05-05 14:17:04.000000 armonik-3.8.2.dev311/src/armonik/protogen/common/auth_common_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-05 14:17:04.000000 armonik-3.8.2.dev311/src/armonik/protogen/common/auth_common_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     3771 2023-05-05 14:17:04.000000 armonik-3.8.2.dev311/src/armonik/protogen/common/events_common_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     4998 2023-05-05 14:17:04.000000 armonik-3.8.2.dev311/src/armonik/protogen/common/events_common_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-05 14:17:04.000000 armonik-3.8.2.dev311/src/armonik/protogen/common/events_common_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     5809 2023-05-05 14:17:04.000000 armonik-3.8.2.dev311/src/armonik/protogen/common/objects_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     8432 2023-05-05 14:17:04.000000 armonik-3.8.2.dev311/src/armonik/protogen/common/objects_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-05 14:17:04.000000 armonik-3.8.2.dev311/src/armonik/protogen/common/objects_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     4421 2023-05-05 14:17:04.000000 armonik-3.8.2.dev311/src/armonik/protogen/common/partitions_common_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     5565 2023-05-05 14:17:04.000000 armonik-3.8.2.dev311/src/armonik/protogen/common/partitions_common_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-05 14:17:04.000000 armonik-3.8.2.dev311/src/armonik/protogen/common/partitions_common_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1302 2023-05-05 14:17:04.000000 armonik-3.8.2.dev311/src/armonik/protogen/common/result_status_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      490 2023-05-05 14:17:04.000000 armonik-3.8.2.dev311/src/armonik/protogen/common/result_status_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-05 14:17:04.000000 armonik-3.8.2.dev311/src/armonik/protogen/common/result_status_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     8333 2023-05-05 14:17:04.000000 armonik-3.8.2.dev311/src/armonik/protogen/common/results_common_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    11856 2023-05-05 14:17:04.000000 armonik-3.8.2.dev311/src/armonik/protogen/common/results_common_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-05 14:17:04.000000 armonik-3.8.2.dev311/src/armonik/protogen/common/results_common_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1217 2023-05-05 14:17:04.000000 armonik-3.8.2.dev311/src/armonik/protogen/common/session_status_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      424 2023-05-05 14:17:04.000000 armonik-3.8.2.dev311/src/armonik/protogen/common/session_status_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-05 14:17:04.000000 armonik-3.8.2.dev311/src/armonik/protogen/common/session_status_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     6087 2023-05-05 14:17:04.000000 armonik-3.8.2.dev311/src/armonik/protogen/common/sessions_common_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     8280 2023-05-05 14:17:04.000000 armonik-3.8.2.dev311/src/armonik/protogen/common/sessions_common_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-05 14:17:04.000000 armonik-3.8.2.dev311/src/armonik/protogen/common/sessions_common_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     8650 2023-05-05 14:17:04.000000 armonik-3.8.2.dev311/src/armonik/protogen/common/submitter_common_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    12539 2023-05-05 14:17:04.000000 armonik-3.8.2.dev311/src/armonik/protogen/common/submitter_common_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-05 14:17:04.000000 armonik-3.8.2.dev311/src/armonik/protogen/common/submitter_common_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1534 2023-05-05 14:17:04.000000 armonik-3.8.2.dev311/src/armonik/protogen/common/task_status_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      673 2023-05-05 14:17:04.000000 armonik-3.8.2.dev311/src/armonik/protogen/common/task_status_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-05 14:17:04.000000 armonik-3.8.2.dev311/src/armonik/protogen/common/task_status_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     9399 2023-05-05 14:17:04.000000 armonik-3.8.2.dev311/src/armonik/protogen/common/tasks_common_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    15628 2023-05-05 14:17:04.000000 armonik-3.8.2.dev311/src/armonik/protogen/common/tasks_common_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-05 14:17:04.000000 armonik-3.8.2.dev311/src/armonik/protogen/common/tasks_common_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     3302 2023-05-05 14:17:04.000000 armonik-3.8.2.dev311/src/armonik/protogen/common/worker_common_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     4065 2023-05-05 14:17:04.000000 armonik-3.8.2.dev311/src/armonik/protogen/common/worker_common_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-05 14:17:04.000000 armonik-3.8.2.dev311/src/armonik/protogen/common/worker_common_pb2_grpc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 14:17:10.800678 armonik-3.8.2.dev311/src/armonik/protogen/worker/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 14:17:04.000000 armonik-3.8.2.dev311/src/armonik/protogen/worker/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2328 2023-05-05 14:17:04.000000 armonik-3.8.2.dev311/src/armonik/protogen/worker/agent_service_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      194 2023-05-05 14:17:04.000000 armonik-3.8.2.dev311/src/armonik/protogen/worker/agent_service_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    15483 2023-05-05 14:17:04.000000 armonik-3.8.2.dev311/src/armonik/protogen/worker/agent_service_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1455 2023-05-05 14:17:04.000000 armonik-3.8.2.dev311/src/armonik/protogen/worker/worker_service_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      245 2023-05-05 14:17:04.000000 armonik-3.8.2.dev311/src/armonik/protogen/worker/worker_service_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     4101 2023-05-05 14:17:04.000000 armonik-3.8.2.dev311/src/armonik/protogen/worker/worker_service_pb2_grpc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 14:17:10.804678 armonik-3.8.2.dev311/src/armonik/worker/
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-05-05 14:16:53.000000 armonik-3.8.2.dev311/src/armonik/worker/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5649 2023-05-05 14:16:53.000000 armonik-3.8.2.dev311/src/armonik/worker/seqlogger.py
--rw-r--r--   0 runner    (1001) docker     (123)     9247 2023-05-05 14:16:53.000000 armonik-3.8.2.dev311/src/armonik/worker/taskhandler.py
--rw-r--r--   0 runner    (1001) docker     (123)     2454 2023-05-05 14:16:53.000000 armonik-3.8.2.dev311/src/armonik/worker/worker.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 14:17:10.792678 armonik-3.8.2.dev311/src/armonik.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2163 2023-05-05 14:17:10.000000 armonik-3.8.2.dev311/src/armonik.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4461 2023-05-05 14:17:10.000000 armonik-3.8.2.dev311/src/armonik.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 14:17:10.000000 armonik-3.8.2.dev311/src/armonik.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-05-05 14:17:10.000000 armonik-3.8.2.dev311/src/armonik.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-05 14:17:10.000000 armonik-3.8.2.dev311/src/armonik.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 15:29:55.133943 armonik-3.8.2.dev313/
+-rw-r--r--   0 runner    (1001) docker     (123)     2163 2023-05-05 15:29:55.133943 armonik-3.8.2.dev313/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1736 2023-05-05 15:29:39.000000 armonik-3.8.2.dev313/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1026 2023-05-05 15:29:39.000000 armonik-3.8.2.dev313/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-05 15:29:55.133943 armonik-3.8.2.dev313/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 15:29:55.121943 armonik-3.8.2.dev313/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 15:29:55.121943 armonik-3.8.2.dev313/src/armonik/
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-05-05 15:29:39.000000 armonik-3.8.2.dev313/src/armonik/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-05-05 15:29:49.000000 armonik-3.8.2.dev313/src/armonik/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 15:29:55.125943 armonik-3.8.2.dev313/src/armonik/client/
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-05-05 15:29:39.000000 armonik-3.8.2.dev313/src/armonik/client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12657 2023-05-05 15:29:39.000000 armonik-3.8.2.dev313/src/armonik/client/submitter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      782 2023-05-05 15:29:39.000000 armonik-3.8.2.dev313/src/armonik/client/tasks.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 15:29:55.125943 armonik-3.8.2.dev313/src/armonik/common/
+-rw-r--r--   0 runner    (1001) docker     (123)      267 2023-05-05 15:29:39.000000 armonik-3.8.2.dev313/src/armonik/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      814 2023-05-05 15:29:39.000000 armonik-3.8.2.dev313/src/armonik/common/enumwrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3714 2023-05-05 15:29:39.000000 armonik-3.8.2.dev313/src/armonik/common/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6263 2023-05-05 15:29:39.000000 armonik-3.8.2.dev313/src/armonik/common/objects.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 15:29:55.121943 armonik-3.8.2.dev313/src/armonik/protogen/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 15:29:55.125943 armonik-3.8.2.dev313/src/armonik/protogen/client/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 15:29:49.000000 armonik-3.8.2.dev313/src/armonik/protogen/client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1572 2023-05-05 15:29:49.000000 armonik-3.8.2.dev313/src/armonik/protogen/client/applications_service_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      208 2023-05-05 15:29:49.000000 armonik-3.8.2.dev313/src/armonik/protogen/client/applications_service_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     4483 2023-05-05 15:29:49.000000 armonik-3.8.2.dev313/src/armonik/protogen/client/applications_service_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1321 2023-05-05 15:29:49.000000 armonik-3.8.2.dev313/src/armonik/protogen/client/auth_service_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      192 2023-05-05 15:29:49.000000 armonik-3.8.2.dev313/src/armonik/protogen/client/auth_service_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2581 2023-05-05 15:29:49.000000 armonik-3.8.2.dev313/src/armonik/protogen/client/auth_service_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1320 2023-05-05 15:29:49.000000 armonik-3.8.2.dev313/src/armonik/protogen/client/events_service_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      196 2023-05-05 15:29:49.000000 armonik-3.8.2.dev313/src/armonik/protogen/client/events_service_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2739 2023-05-05 15:29:49.000000 armonik-3.8.2.dev313/src/armonik/protogen/client/events_service_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1519 2023-05-05 15:29:49.000000 armonik-3.8.2.dev313/src/armonik/protogen/client/partitions_service_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      204 2023-05-05 15:29:49.000000 armonik-3.8.2.dev313/src/armonik/protogen/client/partitions_service_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     4373 2023-05-05 15:29:49.000000 armonik-3.8.2.dev313/src/armonik/protogen/client/partitions_service_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2493 2023-05-05 15:29:49.000000 armonik-3.8.2.dev313/src/armonik/protogen/client/results_service_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      247 2023-05-05 15:29:49.000000 armonik-3.8.2.dev313/src/armonik/protogen/client/results_service_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    14560 2023-05-05 15:29:49.000000 armonik-3.8.2.dev313/src/armonik/protogen/client/results_service_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1779 2023-05-05 15:29:49.000000 armonik-3.8.2.dev313/src/armonik/protogen/client/sessions_service_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      200 2023-05-05 15:29:49.000000 armonik-3.8.2.dev313/src/armonik/protogen/client/sessions_service_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     7535 2023-05-05 15:29:49.000000 armonik-3.8.2.dev313/src/armonik/protogen/client/sessions_service_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3571 2023-05-05 15:29:49.000000 armonik-3.8.2.dev313/src/armonik/protogen/client/submitter_service_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      251 2023-05-05 15:29:49.000000 armonik-3.8.2.dev313/src/armonik/protogen/client/submitter_service_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    27332 2023-05-05 15:29:49.000000 armonik-3.8.2.dev313/src/armonik/protogen/client/submitter_service_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2081 2023-05-05 15:29:49.000000 armonik-3.8.2.dev313/src/armonik/protogen/client/tasks_service_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      194 2023-05-05 15:29:49.000000 armonik-3.8.2.dev313/src/armonik/protogen/client/tasks_service_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    12105 2023-05-05 15:29:49.000000 armonik-3.8.2.dev313/src/armonik/protogen/client/tasks_service_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 15:29:55.133943 armonik-3.8.2.dev313/src/armonik/protogen/common/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 15:29:49.000000 armonik-3.8.2.dev313/src/armonik/protogen/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8764 2023-05-05 15:29:49.000000 armonik-3.8.2.dev313/src/armonik/protogen/common/agent_common_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13431 2023-05-05 15:29:49.000000 armonik-3.8.2.dev313/src/armonik/protogen/common/agent_common_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-05 15:29:49.000000 armonik-3.8.2.dev313/src/armonik/protogen/common/agent_common_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3802 2023-05-05 15:29:49.000000 armonik-3.8.2.dev313/src/armonik/protogen/common/applications_common_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4563 2023-05-05 15:29:49.000000 armonik-3.8.2.dev313/src/armonik/protogen/common/applications_common_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-05 15:29:49.000000 armonik-3.8.2.dev313/src/armonik/protogen/common/applications_common_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1484 2023-05-05 15:29:49.000000 armonik-3.8.2.dev313/src/armonik/protogen/common/auth_common_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1145 2023-05-05 15:29:49.000000 armonik-3.8.2.dev313/src/armonik/protogen/common/auth_common_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-05 15:29:49.000000 armonik-3.8.2.dev313/src/armonik/protogen/common/auth_common_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3771 2023-05-05 15:29:49.000000 armonik-3.8.2.dev313/src/armonik/protogen/common/events_common_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4998 2023-05-05 15:29:49.000000 armonik-3.8.2.dev313/src/armonik/protogen/common/events_common_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-05 15:29:49.000000 armonik-3.8.2.dev313/src/armonik/protogen/common/events_common_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5809 2023-05-05 15:29:49.000000 armonik-3.8.2.dev313/src/armonik/protogen/common/objects_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8432 2023-05-05 15:29:49.000000 armonik-3.8.2.dev313/src/armonik/protogen/common/objects_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-05 15:29:49.000000 armonik-3.8.2.dev313/src/armonik/protogen/common/objects_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4421 2023-05-05 15:29:49.000000 armonik-3.8.2.dev313/src/armonik/protogen/common/partitions_common_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5565 2023-05-05 15:29:49.000000 armonik-3.8.2.dev313/src/armonik/protogen/common/partitions_common_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-05 15:29:49.000000 armonik-3.8.2.dev313/src/armonik/protogen/common/partitions_common_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1302 2023-05-05 15:29:49.000000 armonik-3.8.2.dev313/src/armonik/protogen/common/result_status_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      490 2023-05-05 15:29:49.000000 armonik-3.8.2.dev313/src/armonik/protogen/common/result_status_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-05 15:29:49.000000 armonik-3.8.2.dev313/src/armonik/protogen/common/result_status_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8333 2023-05-05 15:29:49.000000 armonik-3.8.2.dev313/src/armonik/protogen/common/results_common_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11856 2023-05-05 15:29:49.000000 armonik-3.8.2.dev313/src/armonik/protogen/common/results_common_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-05 15:29:49.000000 armonik-3.8.2.dev313/src/armonik/protogen/common/results_common_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1217 2023-05-05 15:29:49.000000 armonik-3.8.2.dev313/src/armonik/protogen/common/session_status_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      424 2023-05-05 15:29:49.000000 armonik-3.8.2.dev313/src/armonik/protogen/common/session_status_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-05 15:29:49.000000 armonik-3.8.2.dev313/src/armonik/protogen/common/session_status_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6087 2023-05-05 15:29:49.000000 armonik-3.8.2.dev313/src/armonik/protogen/common/sessions_common_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8280 2023-05-05 15:29:49.000000 armonik-3.8.2.dev313/src/armonik/protogen/common/sessions_common_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-05 15:29:49.000000 armonik-3.8.2.dev313/src/armonik/protogen/common/sessions_common_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8650 2023-05-05 15:29:49.000000 armonik-3.8.2.dev313/src/armonik/protogen/common/submitter_common_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12539 2023-05-05 15:29:49.000000 armonik-3.8.2.dev313/src/armonik/protogen/common/submitter_common_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-05 15:29:49.000000 armonik-3.8.2.dev313/src/armonik/protogen/common/submitter_common_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1534 2023-05-05 15:29:49.000000 armonik-3.8.2.dev313/src/armonik/protogen/common/task_status_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      673 2023-05-05 15:29:49.000000 armonik-3.8.2.dev313/src/armonik/protogen/common/task_status_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-05 15:29:49.000000 armonik-3.8.2.dev313/src/armonik/protogen/common/task_status_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9399 2023-05-05 15:29:49.000000 armonik-3.8.2.dev313/src/armonik/protogen/common/tasks_common_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15628 2023-05-05 15:29:49.000000 armonik-3.8.2.dev313/src/armonik/protogen/common/tasks_common_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-05 15:29:49.000000 armonik-3.8.2.dev313/src/armonik/protogen/common/tasks_common_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3302 2023-05-05 15:29:49.000000 armonik-3.8.2.dev313/src/armonik/protogen/common/worker_common_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4065 2023-05-05 15:29:49.000000 armonik-3.8.2.dev313/src/armonik/protogen/common/worker_common_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-05 15:29:49.000000 armonik-3.8.2.dev313/src/armonik/protogen/common/worker_common_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 15:29:55.133943 armonik-3.8.2.dev313/src/armonik/protogen/worker/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 15:29:49.000000 armonik-3.8.2.dev313/src/armonik/protogen/worker/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2328 2023-05-05 15:29:49.000000 armonik-3.8.2.dev313/src/armonik/protogen/worker/agent_service_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      194 2023-05-05 15:29:49.000000 armonik-3.8.2.dev313/src/armonik/protogen/worker/agent_service_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    15483 2023-05-05 15:29:49.000000 armonik-3.8.2.dev313/src/armonik/protogen/worker/agent_service_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1455 2023-05-05 15:29:49.000000 armonik-3.8.2.dev313/src/armonik/protogen/worker/worker_service_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      245 2023-05-05 15:29:49.000000 armonik-3.8.2.dev313/src/armonik/protogen/worker/worker_service_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     4101 2023-05-05 15:29:49.000000 armonik-3.8.2.dev313/src/armonik/protogen/worker/worker_service_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 15:29:55.133943 armonik-3.8.2.dev313/src/armonik/worker/
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-05-05 15:29:39.000000 armonik-3.8.2.dev313/src/armonik/worker/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5649 2023-05-05 15:29:39.000000 armonik-3.8.2.dev313/src/armonik/worker/seqlogger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9247 2023-05-05 15:29:39.000000 armonik-3.8.2.dev313/src/armonik/worker/taskhandler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2454 2023-05-05 15:29:39.000000 armonik-3.8.2.dev313/src/armonik/worker/worker.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 15:29:55.125943 armonik-3.8.2.dev313/src/armonik.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2163 2023-05-05 15:29:55.000000 armonik-3.8.2.dev313/src/armonik.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4461 2023-05-05 15:29:55.000000 armonik-3.8.2.dev313/src/armonik.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 15:29:55.000000 armonik-3.8.2.dev313/src/armonik.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-05-05 15:29:55.000000 armonik-3.8.2.dev313/src/armonik.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-05 15:29:55.000000 armonik-3.8.2.dev313/src/armonik.egg-info/top_level.txt
```

### Comparing `armonik-3.8.2.dev311/PKG-INFO` & `armonik-3.8.2.dev313/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: armonik
-Version: 3.8.2.dev311
+Version: 3.8.2.dev313
 Summary: GRPC python binding for the ArmoniK orchestrator API
 License: Apache v2.0 LICENSE
 Project-URL: Homepage, https://github.com/aneoconsulting/ArmoniK.Api
 Project-URL: Bug Tracker, https://github.com/aneoconsulting/ArmoniK/issues
 Keywords: cloud,HTC,gRPC,ArmoniK,Aneo
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
```

### Comparing `armonik-3.8.2.dev311/README.md` & `armonik-3.8.2.dev313/README.md`

 * *Files identical despite different names*

### Comparing `armonik-3.8.2.dev311/pyproject.toml` & `armonik-3.8.2.dev313/pyproject.toml`

 * *Files identical despite different names*

### Comparing `armonik-3.8.2.dev311/src/armonik/client/submitter.py` & `armonik-3.8.2.dev313/src/armonik/client/submitter.py`

 * *Files identical despite different names*

### Comparing `armonik-3.8.2.dev311/src/armonik/client/tasks.py` & `armonik-3.8.2.dev313/src/armonik/client/tasks.py`

 * *Files identical despite different names*

### Comparing `armonik-3.8.2.dev311/src/armonik/common/enumwrapper.py` & `armonik-3.8.2.dev313/src/armonik/common/enumwrapper.py`

 * *Files identical despite different names*

### Comparing `armonik-3.8.2.dev311/src/armonik/common/helpers.py` & `armonik-3.8.2.dev313/src/armonik/common/helpers.py`

 * *Files identical despite different names*

### Comparing `armonik-3.8.2.dev311/src/armonik/common/objects.py` & `armonik-3.8.2.dev313/src/armonik/common/objects.py`

 * *Files identical despite different names*

### Comparing `armonik-3.8.2.dev311/src/armonik/protogen/client/applications_service_pb2.py` & `armonik-3.8.2.dev313/src/armonik/protogen/client/applications_service_pb2.py`

 * *Files identical despite different names*

### Comparing `armonik-3.8.2.dev311/src/armonik/protogen/client/applications_service_pb2_grpc.py` & `armonik-3.8.2.dev313/src/armonik/protogen/client/applications_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `armonik-3.8.2.dev311/src/armonik/protogen/client/auth_service_pb2.py` & `armonik-3.8.2.dev313/src/armonik/protogen/client/auth_service_pb2.py`

 * *Files identical despite different names*

### Comparing `armonik-3.8.2.dev311/src/armonik/protogen/client/auth_service_pb2_grpc.py` & `armonik-3.8.2.dev313/src/armonik/protogen/client/auth_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `armonik-3.8.2.dev311/src/armonik/protogen/client/events_service_pb2.py` & `armonik-3.8.2.dev313/src/armonik/protogen/client/events_service_pb2.py`

 * *Files identical despite different names*

### Comparing `armonik-3.8.2.dev311/src/armonik/protogen/client/events_service_pb2_grpc.py` & `armonik-3.8.2.dev313/src/armonik/protogen/client/events_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `armonik-3.8.2.dev311/src/armonik/protogen/client/partitions_service_pb2.py` & `armonik-3.8.2.dev313/src/armonik/protogen/client/partitions_service_pb2.py`

 * *Files identical despite different names*

### Comparing `armonik-3.8.2.dev311/src/armonik/protogen/client/partitions_service_pb2_grpc.py` & `armonik-3.8.2.dev313/src/armonik/protogen/client/partitions_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `armonik-3.8.2.dev311/src/armonik/protogen/client/results_service_pb2.py` & `armonik-3.8.2.dev313/src/armonik/protogen/client/results_service_pb2.py`

 * *Files identical despite different names*

### Comparing `armonik-3.8.2.dev311/src/armonik/protogen/client/results_service_pb2_grpc.py` & `armonik-3.8.2.dev313/src/armonik/protogen/client/results_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `armonik-3.8.2.dev311/src/armonik/protogen/client/sessions_service_pb2.py` & `armonik-3.8.2.dev313/src/armonik/protogen/client/sessions_service_pb2.py`

 * *Files identical despite different names*

### Comparing `armonik-3.8.2.dev311/src/armonik/protogen/client/sessions_service_pb2_grpc.py` & `armonik-3.8.2.dev313/src/armonik/protogen/client/sessions_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `armonik-3.8.2.dev311/src/armonik/protogen/client/submitter_service_pb2.py` & `armonik-3.8.2.dev313/src/armonik/protogen/client/submitter_service_pb2.py`

 * *Files identical despite different names*

### Comparing `armonik-3.8.2.dev311/src/armonik/protogen/client/submitter_service_pb2_grpc.py` & `armonik-3.8.2.dev313/src/armonik/protogen/client/submitter_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `armonik-3.8.2.dev311/src/armonik/protogen/client/tasks_service_pb2.py` & `armonik-3.8.2.dev313/src/armonik/protogen/client/tasks_service_pb2.py`

 * *Files identical despite different names*

### Comparing `armonik-3.8.2.dev311/src/armonik/protogen/client/tasks_service_pb2_grpc.py` & `armonik-3.8.2.dev313/src/armonik/protogen/client/tasks_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `armonik-3.8.2.dev311/src/armonik/protogen/common/agent_common_pb2.py` & `armonik-3.8.2.dev313/src/armonik/protogen/common/agent_common_pb2.py`

 * *Files identical despite different names*

### Comparing `armonik-3.8.2.dev311/src/armonik/protogen/common/agent_common_pb2.pyi` & `armonik-3.8.2.dev313/src/armonik/protogen/common/agent_common_pb2.pyi`

 * *Files identical despite different names*

### Comparing `armonik-3.8.2.dev311/src/armonik/protogen/common/applications_common_pb2.py` & `armonik-3.8.2.dev313/src/armonik/protogen/common/applications_common_pb2.py`

 * *Files identical despite different names*

### Comparing `armonik-3.8.2.dev311/src/armonik/protogen/common/applications_common_pb2.pyi` & `armonik-3.8.2.dev313/src/armonik/protogen/common/applications_common_pb2.pyi`

 * *Files identical despite different names*

### Comparing `armonik-3.8.2.dev311/src/armonik/protogen/common/auth_common_pb2.py` & `armonik-3.8.2.dev313/src/armonik/protogen/common/auth_common_pb2.py`

 * *Files identical despite different names*

### Comparing `armonik-3.8.2.dev311/src/armonik/protogen/common/auth_common_pb2.pyi` & `armonik-3.8.2.dev313/src/armonik/protogen/common/auth_common_pb2.pyi`

 * *Files identical despite different names*

### Comparing `armonik-3.8.2.dev311/src/armonik/protogen/common/events_common_pb2.py` & `armonik-3.8.2.dev313/src/armonik/protogen/common/events_common_pb2.py`

 * *Files identical despite different names*

### Comparing `armonik-3.8.2.dev311/src/armonik/protogen/common/events_common_pb2.pyi` & `armonik-3.8.2.dev313/src/armonik/protogen/common/events_common_pb2.pyi`

 * *Files identical despite different names*

### Comparing `armonik-3.8.2.dev311/src/armonik/protogen/common/objects_pb2.py` & `armonik-3.8.2.dev313/src/armonik/protogen/common/objects_pb2.py`

 * *Files identical despite different names*

### Comparing `armonik-3.8.2.dev311/src/armonik/protogen/common/objects_pb2.pyi` & `armonik-3.8.2.dev313/src/armonik/protogen/common/objects_pb2.pyi`

 * *Files identical despite different names*

### Comparing `armonik-3.8.2.dev311/src/armonik/protogen/common/partitions_common_pb2.py` & `armonik-3.8.2.dev313/src/armonik/protogen/common/partitions_common_pb2.py`

 * *Files identical despite different names*

### Comparing `armonik-3.8.2.dev311/src/armonik/protogen/common/partitions_common_pb2.pyi` & `armonik-3.8.2.dev313/src/armonik/protogen/common/partitions_common_pb2.pyi`

 * *Files identical despite different names*

### Comparing `armonik-3.8.2.dev311/src/armonik/protogen/common/result_status_pb2.py` & `armonik-3.8.2.dev313/src/armonik/protogen/common/result_status_pb2.py`

 * *Files identical despite different names*

### Comparing `armonik-3.8.2.dev311/src/armonik/protogen/common/results_common_pb2.py` & `armonik-3.8.2.dev313/src/armonik/protogen/common/results_common_pb2.py`

 * *Files identical despite different names*

### Comparing `armonik-3.8.2.dev311/src/armonik/protogen/common/results_common_pb2.pyi` & `armonik-3.8.2.dev313/src/armonik/protogen/common/results_common_pb2.pyi`

 * *Files identical despite different names*

### Comparing `armonik-3.8.2.dev311/src/armonik/protogen/common/session_status_pb2.py` & `armonik-3.8.2.dev313/src/armonik/protogen/common/session_status_pb2.py`

 * *Files identical despite different names*

### Comparing `armonik-3.8.2.dev311/src/armonik/protogen/common/sessions_common_pb2.py` & `armonik-3.8.2.dev313/src/armonik/protogen/common/sessions_common_pb2.py`

 * *Files identical despite different names*

### Comparing `armonik-3.8.2.dev311/src/armonik/protogen/common/sessions_common_pb2.pyi` & `armonik-3.8.2.dev313/src/armonik/protogen/common/sessions_common_pb2.pyi`

 * *Files identical despite different names*

### Comparing `armonik-3.8.2.dev311/src/armonik/protogen/common/submitter_common_pb2.py` & `armonik-3.8.2.dev313/src/armonik/protogen/common/submitter_common_pb2.py`

 * *Files identical despite different names*

### Comparing `armonik-3.8.2.dev311/src/armonik/protogen/common/submitter_common_pb2.pyi` & `armonik-3.8.2.dev313/src/armonik/protogen/common/submitter_common_pb2.pyi`

 * *Files identical despite different names*

### Comparing `armonik-3.8.2.dev311/src/armonik/protogen/common/task_status_pb2.py` & `armonik-3.8.2.dev313/src/armonik/protogen/common/task_status_pb2.py`

 * *Files identical despite different names*

### Comparing `armonik-3.8.2.dev311/src/armonik/protogen/common/task_status_pb2.pyi` & `armonik-3.8.2.dev313/src/armonik/protogen/common/task_status_pb2.pyi`

 * *Files identical despite different names*

### Comparing `armonik-3.8.2.dev311/src/armonik/protogen/common/tasks_common_pb2.py` & `armonik-3.8.2.dev313/src/armonik/protogen/common/tasks_common_pb2.py`

 * *Files identical despite different names*

### Comparing `armonik-3.8.2.dev311/src/armonik/protogen/common/tasks_common_pb2.pyi` & `armonik-3.8.2.dev313/src/armonik/protogen/common/tasks_common_pb2.pyi`

 * *Files identical despite different names*

### Comparing `armonik-3.8.2.dev311/src/armonik/protogen/common/worker_common_pb2.py` & `armonik-3.8.2.dev313/src/armonik/protogen/common/worker_common_pb2.py`

 * *Files identical despite different names*

### Comparing `armonik-3.8.2.dev311/src/armonik/protogen/common/worker_common_pb2.pyi` & `armonik-3.8.2.dev313/src/armonik/protogen/common/worker_common_pb2.pyi`

 * *Files identical despite different names*

### Comparing `armonik-3.8.2.dev311/src/armonik/protogen/worker/agent_service_pb2.py` & `armonik-3.8.2.dev313/src/armonik/protogen/worker/agent_service_pb2.py`

 * *Files identical despite different names*

### Comparing `armonik-3.8.2.dev311/src/armonik/protogen/worker/agent_service_pb2_grpc.py` & `armonik-3.8.2.dev313/src/armonik/protogen/worker/agent_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `armonik-3.8.2.dev311/src/armonik/protogen/worker/worker_service_pb2.py` & `armonik-3.8.2.dev313/src/armonik/protogen/worker/worker_service_pb2.py`

 * *Files identical despite different names*

### Comparing `armonik-3.8.2.dev311/src/armonik/protogen/worker/worker_service_pb2_grpc.py` & `armonik-3.8.2.dev313/src/armonik/protogen/worker/worker_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `armonik-3.8.2.dev311/src/armonik/worker/seqlogger.py` & `armonik-3.8.2.dev313/src/armonik/worker/seqlogger.py`

 * *Files identical despite different names*

### Comparing `armonik-3.8.2.dev311/src/armonik/worker/taskhandler.py` & `armonik-3.8.2.dev313/src/armonik/worker/taskhandler.py`

 * *Files identical despite different names*

### Comparing `armonik-3.8.2.dev311/src/armonik/worker/worker.py` & `armonik-3.8.2.dev313/src/armonik/worker/worker.py`

 * *Files identical despite different names*

### Comparing `armonik-3.8.2.dev311/src/armonik.egg-info/PKG-INFO` & `armonik-3.8.2.dev313/src/armonik.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: armonik
-Version: 3.8.2.dev311
+Version: 3.8.2.dev313
 Summary: GRPC python binding for the ArmoniK orchestrator API
 License: Apache v2.0 LICENSE
 Project-URL: Homepage, https://github.com/aneoconsulting/ArmoniK.Api
 Project-URL: Bug Tracker, https://github.com/aneoconsulting/ArmoniK/issues
 Keywords: cloud,HTC,gRPC,ArmoniK,Aneo
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
```

### Comparing `armonik-3.8.2.dev311/src/armonik.egg-info/SOURCES.txt` & `armonik-3.8.2.dev313/src/armonik.egg-info/SOURCES.txt`

 * *Files identical despite different names*

