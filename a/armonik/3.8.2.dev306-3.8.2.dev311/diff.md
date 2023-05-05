# Comparing `tmp/armonik-3.8.2.dev306.tar.gz` & `tmp/armonik-3.8.2.dev311.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "armonik-3.8.2.dev306.tar", last modified: Thu May  4 15:32:45 2023, max compression
+gzip compressed data, was "armonik-3.8.2.dev311.tar", last modified: Fri May  5 14:17:10 2023, max compression
```

## Comparing `armonik-3.8.2.dev306.tar` & `armonik-3.8.2.dev311.tar`

### file list

```diff
@@ -1,108 +1,108 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 15:32:45.683675 armonik-3.8.2.dev306/
--rw-r--r--   0 runner    (1001) docker     (123)     2163 2023-05-04 15:32:45.683675 armonik-3.8.2.dev306/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1736 2023-05-04 15:32:29.000000 armonik-3.8.2.dev306/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1026 2023-05-04 15:32:29.000000 armonik-3.8.2.dev306/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-04 15:32:45.683675 armonik-3.8.2.dev306/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 15:32:45.659674 armonik-3.8.2.dev306/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 15:32:45.663674 armonik-3.8.2.dev306/src/armonik/
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-05-04 15:32:29.000000 armonik-3.8.2.dev306/src/armonik/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      123 2023-05-04 15:32:39.000000 armonik-3.8.2.dev306/src/armonik/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 15:32:45.663674 armonik-3.8.2.dev306/src/armonik/client/
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-05-04 15:32:29.000000 armonik-3.8.2.dev306/src/armonik/client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12657 2023-05-04 15:32:29.000000 armonik-3.8.2.dev306/src/armonik/client/submitter.py
--rw-r--r--   0 runner    (1001) docker     (123)      782 2023-05-04 15:32:29.000000 armonik-3.8.2.dev306/src/armonik/client/tasks.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 15:32:45.667674 armonik-3.8.2.dev306/src/armonik/common/
--rw-r--r--   0 runner    (1001) docker     (123)      267 2023-05-04 15:32:29.000000 armonik-3.8.2.dev306/src/armonik/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      814 2023-05-04 15:32:29.000000 armonik-3.8.2.dev306/src/armonik/common/enumwrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     3714 2023-05-04 15:32:29.000000 armonik-3.8.2.dev306/src/armonik/common/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     6263 2023-05-04 15:32:29.000000 armonik-3.8.2.dev306/src/armonik/common/objects.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 15:32:45.663674 armonik-3.8.2.dev306/src/armonik/protogen/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 15:32:45.671674 armonik-3.8.2.dev306/src/armonik/protogen/client/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 15:32:39.000000 armonik-3.8.2.dev306/src/armonik/protogen/client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1572 2023-05-04 15:32:39.000000 armonik-3.8.2.dev306/src/armonik/protogen/client/applications_service_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      208 2023-05-04 15:32:39.000000 armonik-3.8.2.dev306/src/armonik/protogen/client/applications_service_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     4483 2023-05-04 15:32:39.000000 armonik-3.8.2.dev306/src/armonik/protogen/client/applications_service_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1321 2023-05-04 15:32:39.000000 armonik-3.8.2.dev306/src/armonik/protogen/client/auth_service_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      192 2023-05-04 15:32:39.000000 armonik-3.8.2.dev306/src/armonik/protogen/client/auth_service_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2581 2023-05-04 15:32:39.000000 armonik-3.8.2.dev306/src/armonik/protogen/client/auth_service_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1320 2023-05-04 15:32:39.000000 armonik-3.8.2.dev306/src/armonik/protogen/client/events_service_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      196 2023-05-04 15:32:39.000000 armonik-3.8.2.dev306/src/armonik/protogen/client/events_service_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     2739 2023-05-04 15:32:39.000000 armonik-3.8.2.dev306/src/armonik/protogen/client/events_service_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1519 2023-05-04 15:32:39.000000 armonik-3.8.2.dev306/src/armonik/protogen/client/partitions_service_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      204 2023-05-04 15:32:39.000000 armonik-3.8.2.dev306/src/armonik/protogen/client/partitions_service_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     4373 2023-05-04 15:32:39.000000 armonik-3.8.2.dev306/src/armonik/protogen/client/partitions_service_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     2493 2023-05-04 15:32:39.000000 armonik-3.8.2.dev306/src/armonik/protogen/client/results_service_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      247 2023-05-04 15:32:39.000000 armonik-3.8.2.dev306/src/armonik/protogen/client/results_service_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    14560 2023-05-04 15:32:39.000000 armonik-3.8.2.dev306/src/armonik/protogen/client/results_service_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1779 2023-05-04 15:32:39.000000 armonik-3.8.2.dev306/src/armonik/protogen/client/sessions_service_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      200 2023-05-04 15:32:39.000000 armonik-3.8.2.dev306/src/armonik/protogen/client/sessions_service_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     7535 2023-05-04 15:32:39.000000 armonik-3.8.2.dev306/src/armonik/protogen/client/sessions_service_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     3571 2023-05-04 15:32:39.000000 armonik-3.8.2.dev306/src/armonik/protogen/client/submitter_service_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      251 2023-05-04 15:32:39.000000 armonik-3.8.2.dev306/src/armonik/protogen/client/submitter_service_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    27332 2023-05-04 15:32:39.000000 armonik-3.8.2.dev306/src/armonik/protogen/client/submitter_service_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     2081 2023-05-04 15:32:39.000000 armonik-3.8.2.dev306/src/armonik/protogen/client/tasks_service_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      194 2023-05-04 15:32:39.000000 armonik-3.8.2.dev306/src/armonik/protogen/client/tasks_service_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    12105 2023-05-04 15:32:39.000000 armonik-3.8.2.dev306/src/armonik/protogen/client/tasks_service_pb2_grpc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 15:32:45.679674 armonik-3.8.2.dev306/src/armonik/protogen/common/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 15:32:39.000000 armonik-3.8.2.dev306/src/armonik/protogen/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8764 2023-05-04 15:32:39.000000 armonik-3.8.2.dev306/src/armonik/protogen/common/agent_common_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    13431 2023-05-04 15:32:39.000000 armonik-3.8.2.dev306/src/armonik/protogen/common/agent_common_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-04 15:32:39.000000 armonik-3.8.2.dev306/src/armonik/protogen/common/agent_common_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     3802 2023-05-04 15:32:39.000000 armonik-3.8.2.dev306/src/armonik/protogen/common/applications_common_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     4563 2023-05-04 15:32:39.000000 armonik-3.8.2.dev306/src/armonik/protogen/common/applications_common_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-04 15:32:39.000000 armonik-3.8.2.dev306/src/armonik/protogen/common/applications_common_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1484 2023-05-04 15:32:39.000000 armonik-3.8.2.dev306/src/armonik/protogen/common/auth_common_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     1145 2023-05-04 15:32:39.000000 armonik-3.8.2.dev306/src/armonik/protogen/common/auth_common_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-04 15:32:39.000000 armonik-3.8.2.dev306/src/armonik/protogen/common/auth_common_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     3771 2023-05-04 15:32:39.000000 armonik-3.8.2.dev306/src/armonik/protogen/common/events_common_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     4998 2023-05-04 15:32:39.000000 armonik-3.8.2.dev306/src/armonik/protogen/common/events_common_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-04 15:32:39.000000 armonik-3.8.2.dev306/src/armonik/protogen/common/events_common_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     5809 2023-05-04 15:32:39.000000 armonik-3.8.2.dev306/src/armonik/protogen/common/objects_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     8432 2023-05-04 15:32:39.000000 armonik-3.8.2.dev306/src/armonik/protogen/common/objects_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-04 15:32:39.000000 armonik-3.8.2.dev306/src/armonik/protogen/common/objects_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     4421 2023-05-04 15:32:39.000000 armonik-3.8.2.dev306/src/armonik/protogen/common/partitions_common_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     5565 2023-05-04 15:32:39.000000 armonik-3.8.2.dev306/src/armonik/protogen/common/partitions_common_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-04 15:32:39.000000 armonik-3.8.2.dev306/src/armonik/protogen/common/partitions_common_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1302 2023-05-04 15:32:39.000000 armonik-3.8.2.dev306/src/armonik/protogen/common/result_status_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      490 2023-05-04 15:32:39.000000 armonik-3.8.2.dev306/src/armonik/protogen/common/result_status_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-04 15:32:39.000000 armonik-3.8.2.dev306/src/armonik/protogen/common/result_status_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     8333 2023-05-04 15:32:39.000000 armonik-3.8.2.dev306/src/armonik/protogen/common/results_common_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    11856 2023-05-04 15:32:39.000000 armonik-3.8.2.dev306/src/armonik/protogen/common/results_common_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-04 15:32:39.000000 armonik-3.8.2.dev306/src/armonik/protogen/common/results_common_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1217 2023-05-04 15:32:39.000000 armonik-3.8.2.dev306/src/armonik/protogen/common/session_status_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      424 2023-05-04 15:32:39.000000 armonik-3.8.2.dev306/src/armonik/protogen/common/session_status_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-04 15:32:39.000000 armonik-3.8.2.dev306/src/armonik/protogen/common/session_status_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     5820 2023-05-04 15:32:39.000000 armonik-3.8.2.dev306/src/armonik/protogen/common/sessions_common_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     7902 2023-05-04 15:32:39.000000 armonik-3.8.2.dev306/src/armonik/protogen/common/sessions_common_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-04 15:32:39.000000 armonik-3.8.2.dev306/src/armonik/protogen/common/sessions_common_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     8650 2023-05-04 15:32:39.000000 armonik-3.8.2.dev306/src/armonik/protogen/common/submitter_common_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    12539 2023-05-04 15:32:39.000000 armonik-3.8.2.dev306/src/armonik/protogen/common/submitter_common_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-04 15:32:39.000000 armonik-3.8.2.dev306/src/armonik/protogen/common/submitter_common_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1534 2023-05-04 15:32:39.000000 armonik-3.8.2.dev306/src/armonik/protogen/common/task_status_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      673 2023-05-04 15:32:39.000000 armonik-3.8.2.dev306/src/armonik/protogen/common/task_status_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-04 15:32:39.000000 armonik-3.8.2.dev306/src/armonik/protogen/common/task_status_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     8922 2023-05-04 15:32:39.000000 armonik-3.8.2.dev306/src/armonik/protogen/common/tasks_common_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)    14658 2023-05-04 15:32:39.000000 armonik-3.8.2.dev306/src/armonik/protogen/common/tasks_common_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-04 15:32:39.000000 armonik-3.8.2.dev306/src/armonik/protogen/common/tasks_common_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     3302 2023-05-04 15:32:39.000000 armonik-3.8.2.dev306/src/armonik/protogen/common/worker_common_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)     4065 2023-05-04 15:32:39.000000 armonik-3.8.2.dev306/src/armonik/protogen/common/worker_common_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-04 15:32:39.000000 armonik-3.8.2.dev306/src/armonik/protogen/common/worker_common_pb2_grpc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 15:32:45.683675 armonik-3.8.2.dev306/src/armonik/protogen/worker/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 15:32:39.000000 armonik-3.8.2.dev306/src/armonik/protogen/worker/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2328 2023-05-04 15:32:39.000000 armonik-3.8.2.dev306/src/armonik/protogen/worker/agent_service_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      194 2023-05-04 15:32:39.000000 armonik-3.8.2.dev306/src/armonik/protogen/worker/agent_service_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)    15483 2023-05-04 15:32:39.000000 armonik-3.8.2.dev306/src/armonik/protogen/worker/agent_service_pb2_grpc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1455 2023-05-04 15:32:39.000000 armonik-3.8.2.dev306/src/armonik/protogen/worker/worker_service_pb2.py
--rw-r--r--   0 runner    (1001) docker     (123)      245 2023-05-04 15:32:39.000000 armonik-3.8.2.dev306/src/armonik/protogen/worker/worker_service_pb2.pyi
--rw-r--r--   0 runner    (1001) docker     (123)     4101 2023-05-04 15:32:39.000000 armonik-3.8.2.dev306/src/armonik/protogen/worker/worker_service_pb2_grpc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 15:32:45.683675 armonik-3.8.2.dev306/src/armonik/worker/
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-05-04 15:32:29.000000 armonik-3.8.2.dev306/src/armonik/worker/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5649 2023-05-04 15:32:29.000000 armonik-3.8.2.dev306/src/armonik/worker/seqlogger.py
--rw-r--r--   0 runner    (1001) docker     (123)     9247 2023-05-04 15:32:29.000000 armonik-3.8.2.dev306/src/armonik/worker/taskhandler.py
--rw-r--r--   0 runner    (1001) docker     (123)     2454 2023-05-04 15:32:29.000000 armonik-3.8.2.dev306/src/armonik/worker/worker.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 15:32:45.663674 armonik-3.8.2.dev306/src/armonik.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2163 2023-05-04 15:32:45.000000 armonik-3.8.2.dev306/src/armonik.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4461 2023-05-04 15:32:45.000000 armonik-3.8.2.dev306/src/armonik.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-04 15:32:45.000000 armonik-3.8.2.dev306/src/armonik.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-05-04 15:32:45.000000 armonik-3.8.2.dev306/src/armonik.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-04 15:32:45.000000 armonik-3.8.2.dev306/src/armonik.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 14:17:10.804678 armonik-3.8.2.dev311/
+-rw-r--r--   0 runner    (1001) docker     (123)     2163 2023-05-05 14:17:10.804678 armonik-3.8.2.dev311/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1736 2023-05-05 14:16:53.000000 armonik-3.8.2.dev311/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1026 2023-05-05 14:16:53.000000 armonik-3.8.2.dev311/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-05 14:17:10.804678 armonik-3.8.2.dev311/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 14:17:10.792678 armonik-3.8.2.dev311/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 14:17:10.792678 armonik-3.8.2.dev311/src/armonik/
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-05-05 14:16:53.000000 armonik-3.8.2.dev311/src/armonik/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-05-05 14:17:04.000000 armonik-3.8.2.dev311/src/armonik/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 14:17:10.792678 armonik-3.8.2.dev311/src/armonik/client/
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-05-05 14:16:53.000000 armonik-3.8.2.dev311/src/armonik/client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12657 2023-05-05 14:16:53.000000 armonik-3.8.2.dev311/src/armonik/client/submitter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      782 2023-05-05 14:16:53.000000 armonik-3.8.2.dev311/src/armonik/client/tasks.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 14:17:10.792678 armonik-3.8.2.dev311/src/armonik/common/
+-rw-r--r--   0 runner    (1001) docker     (123)      267 2023-05-05 14:16:53.000000 armonik-3.8.2.dev311/src/armonik/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      814 2023-05-05 14:16:53.000000 armonik-3.8.2.dev311/src/armonik/common/enumwrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3714 2023-05-05 14:16:53.000000 armonik-3.8.2.dev311/src/armonik/common/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6263 2023-05-05 14:16:53.000000 armonik-3.8.2.dev311/src/armonik/common/objects.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 14:17:10.792678 armonik-3.8.2.dev311/src/armonik/protogen/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 14:17:10.796678 armonik-3.8.2.dev311/src/armonik/protogen/client/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 14:17:04.000000 armonik-3.8.2.dev311/src/armonik/protogen/client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1572 2023-05-05 14:17:04.000000 armonik-3.8.2.dev311/src/armonik/protogen/client/applications_service_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      208 2023-05-05 14:17:04.000000 armonik-3.8.2.dev311/src/armonik/protogen/client/applications_service_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     4483 2023-05-05 14:17:04.000000 armonik-3.8.2.dev311/src/armonik/protogen/client/applications_service_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1321 2023-05-05 14:17:04.000000 armonik-3.8.2.dev311/src/armonik/protogen/client/auth_service_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      192 2023-05-05 14:17:04.000000 armonik-3.8.2.dev311/src/armonik/protogen/client/auth_service_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2581 2023-05-05 14:17:04.000000 armonik-3.8.2.dev311/src/armonik/protogen/client/auth_service_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1320 2023-05-05 14:17:04.000000 armonik-3.8.2.dev311/src/armonik/protogen/client/events_service_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      196 2023-05-05 14:17:04.000000 armonik-3.8.2.dev311/src/armonik/protogen/client/events_service_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     2739 2023-05-05 14:17:04.000000 armonik-3.8.2.dev311/src/armonik/protogen/client/events_service_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1519 2023-05-05 14:17:04.000000 armonik-3.8.2.dev311/src/armonik/protogen/client/partitions_service_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      204 2023-05-05 14:17:04.000000 armonik-3.8.2.dev311/src/armonik/protogen/client/partitions_service_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     4373 2023-05-05 14:17:04.000000 armonik-3.8.2.dev311/src/armonik/protogen/client/partitions_service_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2493 2023-05-05 14:17:04.000000 armonik-3.8.2.dev311/src/armonik/protogen/client/results_service_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      247 2023-05-05 14:17:04.000000 armonik-3.8.2.dev311/src/armonik/protogen/client/results_service_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    14560 2023-05-05 14:17:04.000000 armonik-3.8.2.dev311/src/armonik/protogen/client/results_service_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1779 2023-05-05 14:17:04.000000 armonik-3.8.2.dev311/src/armonik/protogen/client/sessions_service_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      200 2023-05-05 14:17:04.000000 armonik-3.8.2.dev311/src/armonik/protogen/client/sessions_service_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     7535 2023-05-05 14:17:04.000000 armonik-3.8.2.dev311/src/armonik/protogen/client/sessions_service_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3571 2023-05-05 14:17:04.000000 armonik-3.8.2.dev311/src/armonik/protogen/client/submitter_service_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      251 2023-05-05 14:17:04.000000 armonik-3.8.2.dev311/src/armonik/protogen/client/submitter_service_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    27332 2023-05-05 14:17:04.000000 armonik-3.8.2.dev311/src/armonik/protogen/client/submitter_service_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2081 2023-05-05 14:17:04.000000 armonik-3.8.2.dev311/src/armonik/protogen/client/tasks_service_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      194 2023-05-05 14:17:04.000000 armonik-3.8.2.dev311/src/armonik/protogen/client/tasks_service_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    12105 2023-05-05 14:17:04.000000 armonik-3.8.2.dev311/src/armonik/protogen/client/tasks_service_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 14:17:10.800678 armonik-3.8.2.dev311/src/armonik/protogen/common/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 14:17:04.000000 armonik-3.8.2.dev311/src/armonik/protogen/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8764 2023-05-05 14:17:04.000000 armonik-3.8.2.dev311/src/armonik/protogen/common/agent_common_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13431 2023-05-05 14:17:04.000000 armonik-3.8.2.dev311/src/armonik/protogen/common/agent_common_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-05 14:17:04.000000 armonik-3.8.2.dev311/src/armonik/protogen/common/agent_common_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3802 2023-05-05 14:17:04.000000 armonik-3.8.2.dev311/src/armonik/protogen/common/applications_common_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4563 2023-05-05 14:17:04.000000 armonik-3.8.2.dev311/src/armonik/protogen/common/applications_common_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-05 14:17:04.000000 armonik-3.8.2.dev311/src/armonik/protogen/common/applications_common_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1484 2023-05-05 14:17:04.000000 armonik-3.8.2.dev311/src/armonik/protogen/common/auth_common_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1145 2023-05-05 14:17:04.000000 armonik-3.8.2.dev311/src/armonik/protogen/common/auth_common_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-05 14:17:04.000000 armonik-3.8.2.dev311/src/armonik/protogen/common/auth_common_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3771 2023-05-05 14:17:04.000000 armonik-3.8.2.dev311/src/armonik/protogen/common/events_common_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4998 2023-05-05 14:17:04.000000 armonik-3.8.2.dev311/src/armonik/protogen/common/events_common_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-05 14:17:04.000000 armonik-3.8.2.dev311/src/armonik/protogen/common/events_common_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5809 2023-05-05 14:17:04.000000 armonik-3.8.2.dev311/src/armonik/protogen/common/objects_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8432 2023-05-05 14:17:04.000000 armonik-3.8.2.dev311/src/armonik/protogen/common/objects_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-05 14:17:04.000000 armonik-3.8.2.dev311/src/armonik/protogen/common/objects_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4421 2023-05-05 14:17:04.000000 armonik-3.8.2.dev311/src/armonik/protogen/common/partitions_common_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5565 2023-05-05 14:17:04.000000 armonik-3.8.2.dev311/src/armonik/protogen/common/partitions_common_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-05 14:17:04.000000 armonik-3.8.2.dev311/src/armonik/protogen/common/partitions_common_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1302 2023-05-05 14:17:04.000000 armonik-3.8.2.dev311/src/armonik/protogen/common/result_status_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      490 2023-05-05 14:17:04.000000 armonik-3.8.2.dev311/src/armonik/protogen/common/result_status_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-05 14:17:04.000000 armonik-3.8.2.dev311/src/armonik/protogen/common/result_status_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8333 2023-05-05 14:17:04.000000 armonik-3.8.2.dev311/src/armonik/protogen/common/results_common_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11856 2023-05-05 14:17:04.000000 armonik-3.8.2.dev311/src/armonik/protogen/common/results_common_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-05 14:17:04.000000 armonik-3.8.2.dev311/src/armonik/protogen/common/results_common_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1217 2023-05-05 14:17:04.000000 armonik-3.8.2.dev311/src/armonik/protogen/common/session_status_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      424 2023-05-05 14:17:04.000000 armonik-3.8.2.dev311/src/armonik/protogen/common/session_status_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-05 14:17:04.000000 armonik-3.8.2.dev311/src/armonik/protogen/common/session_status_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6087 2023-05-05 14:17:04.000000 armonik-3.8.2.dev311/src/armonik/protogen/common/sessions_common_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8280 2023-05-05 14:17:04.000000 armonik-3.8.2.dev311/src/armonik/protogen/common/sessions_common_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-05 14:17:04.000000 armonik-3.8.2.dev311/src/armonik/protogen/common/sessions_common_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8650 2023-05-05 14:17:04.000000 armonik-3.8.2.dev311/src/armonik/protogen/common/submitter_common_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12539 2023-05-05 14:17:04.000000 armonik-3.8.2.dev311/src/armonik/protogen/common/submitter_common_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-05 14:17:04.000000 armonik-3.8.2.dev311/src/armonik/protogen/common/submitter_common_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1534 2023-05-05 14:17:04.000000 armonik-3.8.2.dev311/src/armonik/protogen/common/task_status_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      673 2023-05-05 14:17:04.000000 armonik-3.8.2.dev311/src/armonik/protogen/common/task_status_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-05 14:17:04.000000 armonik-3.8.2.dev311/src/armonik/protogen/common/task_status_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9399 2023-05-05 14:17:04.000000 armonik-3.8.2.dev311/src/armonik/protogen/common/tasks_common_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15628 2023-05-05 14:17:04.000000 armonik-3.8.2.dev311/src/armonik/protogen/common/tasks_common_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-05 14:17:04.000000 armonik-3.8.2.dev311/src/armonik/protogen/common/tasks_common_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3302 2023-05-05 14:17:04.000000 armonik-3.8.2.dev311/src/armonik/protogen/common/worker_common_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4065 2023-05-05 14:17:04.000000 armonik-3.8.2.dev311/src/armonik/protogen/common/worker_common_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-05 14:17:04.000000 armonik-3.8.2.dev311/src/armonik/protogen/common/worker_common_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 14:17:10.800678 armonik-3.8.2.dev311/src/armonik/protogen/worker/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 14:17:04.000000 armonik-3.8.2.dev311/src/armonik/protogen/worker/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2328 2023-05-05 14:17:04.000000 armonik-3.8.2.dev311/src/armonik/protogen/worker/agent_service_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      194 2023-05-05 14:17:04.000000 armonik-3.8.2.dev311/src/armonik/protogen/worker/agent_service_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)    15483 2023-05-05 14:17:04.000000 armonik-3.8.2.dev311/src/armonik/protogen/worker/agent_service_pb2_grpc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1455 2023-05-05 14:17:04.000000 armonik-3.8.2.dev311/src/armonik/protogen/worker/worker_service_pb2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      245 2023-05-05 14:17:04.000000 armonik-3.8.2.dev311/src/armonik/protogen/worker/worker_service_pb2.pyi
+-rw-r--r--   0 runner    (1001) docker     (123)     4101 2023-05-05 14:17:04.000000 armonik-3.8.2.dev311/src/armonik/protogen/worker/worker_service_pb2_grpc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 14:17:10.804678 armonik-3.8.2.dev311/src/armonik/worker/
+-rw-r--r--   0 runner    (1001) docker     (123)      105 2023-05-05 14:16:53.000000 armonik-3.8.2.dev311/src/armonik/worker/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5649 2023-05-05 14:16:53.000000 armonik-3.8.2.dev311/src/armonik/worker/seqlogger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9247 2023-05-05 14:16:53.000000 armonik-3.8.2.dev311/src/armonik/worker/taskhandler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2454 2023-05-05 14:16:53.000000 armonik-3.8.2.dev311/src/armonik/worker/worker.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 14:17:10.792678 armonik-3.8.2.dev311/src/armonik.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2163 2023-05-05 14:17:10.000000 armonik-3.8.2.dev311/src/armonik.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4461 2023-05-05 14:17:10.000000 armonik-3.8.2.dev311/src/armonik.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 14:17:10.000000 armonik-3.8.2.dev311/src/armonik.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-05-05 14:17:10.000000 armonik-3.8.2.dev311/src/armonik.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-05 14:17:10.000000 armonik-3.8.2.dev311/src/armonik.egg-info/top_level.txt
```

### Comparing `armonik-3.8.2.dev306/PKG-INFO` & `armonik-3.8.2.dev311/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: armonik
-Version: 3.8.2.dev306
+Version: 3.8.2.dev311
 Summary: GRPC python binding for the ArmoniK orchestrator API
 License: Apache v2.0 LICENSE
 Project-URL: Homepage, https://github.com/aneoconsulting/ArmoniK.Api
 Project-URL: Bug Tracker, https://github.com/aneoconsulting/ArmoniK/issues
 Keywords: cloud,HTC,gRPC,ArmoniK,Aneo
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
```

### Comparing `armonik-3.8.2.dev306/README.md` & `armonik-3.8.2.dev311/README.md`

 * *Files identical despite different names*

### Comparing `armonik-3.8.2.dev306/pyproject.toml` & `armonik-3.8.2.dev311/pyproject.toml`

 * *Files identical despite different names*

### Comparing `armonik-3.8.2.dev306/src/armonik/client/submitter.py` & `armonik-3.8.2.dev311/src/armonik/client/submitter.py`

 * *Files identical despite different names*

### Comparing `armonik-3.8.2.dev306/src/armonik/client/tasks.py` & `armonik-3.8.2.dev311/src/armonik/client/tasks.py`

 * *Files identical despite different names*

### Comparing `armonik-3.8.2.dev306/src/armonik/common/enumwrapper.py` & `armonik-3.8.2.dev311/src/armonik/common/enumwrapper.py`

 * *Files identical despite different names*

### Comparing `armonik-3.8.2.dev306/src/armonik/common/helpers.py` & `armonik-3.8.2.dev311/src/armonik/common/helpers.py`

 * *Files identical despite different names*

### Comparing `armonik-3.8.2.dev306/src/armonik/common/objects.py` & `armonik-3.8.2.dev311/src/armonik/common/objects.py`

 * *Files identical despite different names*

### Comparing `armonik-3.8.2.dev306/src/armonik/protogen/client/applications_service_pb2.py` & `armonik-3.8.2.dev311/src/armonik/protogen/client/applications_service_pb2.py`

 * *Files identical despite different names*

### Comparing `armonik-3.8.2.dev306/src/armonik/protogen/client/applications_service_pb2_grpc.py` & `armonik-3.8.2.dev311/src/armonik/protogen/client/applications_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `armonik-3.8.2.dev306/src/armonik/protogen/client/auth_service_pb2.py` & `armonik-3.8.2.dev311/src/armonik/protogen/client/auth_service_pb2.py`

 * *Files identical despite different names*

### Comparing `armonik-3.8.2.dev306/src/armonik/protogen/client/auth_service_pb2_grpc.py` & `armonik-3.8.2.dev311/src/armonik/protogen/client/auth_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `armonik-3.8.2.dev306/src/armonik/protogen/client/events_service_pb2.py` & `armonik-3.8.2.dev311/src/armonik/protogen/client/events_service_pb2.py`

 * *Files identical despite different names*

### Comparing `armonik-3.8.2.dev306/src/armonik/protogen/client/events_service_pb2_grpc.py` & `armonik-3.8.2.dev311/src/armonik/protogen/client/events_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `armonik-3.8.2.dev306/src/armonik/protogen/client/partitions_service_pb2.py` & `armonik-3.8.2.dev311/src/armonik/protogen/client/partitions_service_pb2.py`

 * *Files identical despite different names*

### Comparing `armonik-3.8.2.dev306/src/armonik/protogen/client/partitions_service_pb2_grpc.py` & `armonik-3.8.2.dev311/src/armonik/protogen/client/partitions_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `armonik-3.8.2.dev306/src/armonik/protogen/client/results_service_pb2.py` & `armonik-3.8.2.dev311/src/armonik/protogen/client/results_service_pb2.py`

 * *Files identical despite different names*

### Comparing `armonik-3.8.2.dev306/src/armonik/protogen/client/results_service_pb2_grpc.py` & `armonik-3.8.2.dev311/src/armonik/protogen/client/results_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `armonik-3.8.2.dev306/src/armonik/protogen/client/sessions_service_pb2.py` & `armonik-3.8.2.dev311/src/armonik/protogen/client/sessions_service_pb2.py`

 * *Files identical despite different names*

### Comparing `armonik-3.8.2.dev306/src/armonik/protogen/client/sessions_service_pb2_grpc.py` & `armonik-3.8.2.dev311/src/armonik/protogen/client/sessions_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `armonik-3.8.2.dev306/src/armonik/protogen/client/submitter_service_pb2.py` & `armonik-3.8.2.dev311/src/armonik/protogen/client/submitter_service_pb2.py`

 * *Files identical despite different names*

### Comparing `armonik-3.8.2.dev306/src/armonik/protogen/client/submitter_service_pb2_grpc.py` & `armonik-3.8.2.dev311/src/armonik/protogen/client/submitter_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `armonik-3.8.2.dev306/src/armonik/protogen/client/tasks_service_pb2.py` & `armonik-3.8.2.dev311/src/armonik/protogen/client/tasks_service_pb2.py`

 * *Files identical despite different names*

### Comparing `armonik-3.8.2.dev306/src/armonik/protogen/client/tasks_service_pb2_grpc.py` & `armonik-3.8.2.dev311/src/armonik/protogen/client/tasks_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `armonik-3.8.2.dev306/src/armonik/protogen/common/agent_common_pb2.py` & `armonik-3.8.2.dev311/src/armonik/protogen/common/agent_common_pb2.py`

 * *Files identical despite different names*

### Comparing `armonik-3.8.2.dev306/src/armonik/protogen/common/agent_common_pb2.pyi` & `armonik-3.8.2.dev311/src/armonik/protogen/common/agent_common_pb2.pyi`

 * *Files identical despite different names*

### Comparing `armonik-3.8.2.dev306/src/armonik/protogen/common/applications_common_pb2.py` & `armonik-3.8.2.dev311/src/armonik/protogen/common/applications_common_pb2.py`

 * *Files identical despite different names*

### Comparing `armonik-3.8.2.dev306/src/armonik/protogen/common/applications_common_pb2.pyi` & `armonik-3.8.2.dev311/src/armonik/protogen/common/applications_common_pb2.pyi`

 * *Files identical despite different names*

### Comparing `armonik-3.8.2.dev306/src/armonik/protogen/common/auth_common_pb2.py` & `armonik-3.8.2.dev311/src/armonik/protogen/common/auth_common_pb2.py`

 * *Files identical despite different names*

### Comparing `armonik-3.8.2.dev306/src/armonik/protogen/common/auth_common_pb2.pyi` & `armonik-3.8.2.dev311/src/armonik/protogen/common/auth_common_pb2.pyi`

 * *Files identical despite different names*

### Comparing `armonik-3.8.2.dev306/src/armonik/protogen/common/events_common_pb2.py` & `armonik-3.8.2.dev311/src/armonik/protogen/common/events_common_pb2.py`

 * *Files identical despite different names*

### Comparing `armonik-3.8.2.dev306/src/armonik/protogen/common/events_common_pb2.pyi` & `armonik-3.8.2.dev311/src/armonik/protogen/common/events_common_pb2.pyi`

 * *Files identical despite different names*

### Comparing `armonik-3.8.2.dev306/src/armonik/protogen/common/objects_pb2.py` & `armonik-3.8.2.dev311/src/armonik/protogen/common/objects_pb2.py`

 * *Files identical despite different names*

### Comparing `armonik-3.8.2.dev306/src/armonik/protogen/common/objects_pb2.pyi` & `armonik-3.8.2.dev311/src/armonik/protogen/common/objects_pb2.pyi`

 * *Files identical despite different names*

### Comparing `armonik-3.8.2.dev306/src/armonik/protogen/common/partitions_common_pb2.py` & `armonik-3.8.2.dev311/src/armonik/protogen/common/partitions_common_pb2.py`

 * *Files identical despite different names*

### Comparing `armonik-3.8.2.dev306/src/armonik/protogen/common/partitions_common_pb2.pyi` & `armonik-3.8.2.dev311/src/armonik/protogen/common/partitions_common_pb2.pyi`

 * *Files identical despite different names*

### Comparing `armonik-3.8.2.dev306/src/armonik/protogen/common/result_status_pb2.py` & `armonik-3.8.2.dev311/src/armonik/protogen/common/result_status_pb2.py`

 * *Files identical despite different names*

### Comparing `armonik-3.8.2.dev306/src/armonik/protogen/common/results_common_pb2.py` & `armonik-3.8.2.dev311/src/armonik/protogen/common/results_common_pb2.py`

 * *Files identical despite different names*

### Comparing `armonik-3.8.2.dev306/src/armonik/protogen/common/results_common_pb2.pyi` & `armonik-3.8.2.dev311/src/armonik/protogen/common/results_common_pb2.pyi`

 * *Files identical despite different names*

### Comparing `armonik-3.8.2.dev306/src/armonik/protogen/common/session_status_pb2.py` & `armonik-3.8.2.dev311/src/armonik/protogen/common/session_status_pb2.py`

 * *Files identical despite different names*

### Comparing `armonik-3.8.2.dev306/src/armonik/protogen/common/sessions_common_pb2.py` & `armonik-3.8.2.dev311/src/armonik/protogen/common/sessions_common_pb2.py`

 * *Files 8% similar despite different names*

```diff
@@ -7,49 +7,50 @@
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
+from google.protobuf import duration_pb2 as google_dot_protobuf_dot_duration__pb2
 from google.protobuf import timestamp_pb2 as google_dot_protobuf_dot_timestamp__pb2
 from . import objects_pb2 as objects__pb2
 from . import session_status_pb2 as session__status__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x15sessions_common.proto\x12\x1c\x61rmonik.api.grpc.v1.sessions\x1a\x1fgoogle/protobuf/timestamp.proto\x1a\robjects.proto\x1a\x14session_status.proto\"\x8f\x02\n\nSessionRaw\x12\x12\n\nsession_id\x18\x01 \x01(\t\x12\x41\n\x06status\x18\x02 \x01(\x0e\x32\x31.armonik.api.grpc.v1.session_status.SessionStatus\x12\x15\n\rpartition_ids\x18\x03 \x03(\t\x12\x31\n\x07options\x18\x04 \x01(\x0b\x32 .armonik.api.grpc.v1.TaskOptions\x12.\n\ncreated_at\x18\x05 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x30\n\x0c\x63\x61ncelled_at\x18\x06 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\"\xfc\x01\n\x0eSessionSummary\x12\x12\n\nsession_id\x18\x01 \x01(\t\x12\x41\n\x06status\x18\x02 \x01(\x0e\x32\x31.armonik.api.grpc.v1.session_status.SessionStatus\x12.\n\ncreated_at\x18\x03 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x30\n\x0c\x63\x61ncelled_at\x18\x04 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x31\n\x07options\x18\x05 \x01(\x0b\x32 .armonik.api.grpc.v1.TaskOptions\"\x8a\x08\n\x13ListSessionsRequest\x12\x0c\n\x04page\x18\x01 \x01(\x05\x12\x11\n\tpage_size\x18\x02 \x01(\x05\x12H\n\x06\x66ilter\x18\x03 \x01(\x0b\x32\x38.armonik.api.grpc.v1.sessions.ListSessionsRequest.Filter\x12\x44\n\x04sort\x18\x04 \x01(\x0b\x32\x36.armonik.api.grpc.v1.sessions.ListSessionsRequest.Sort\x12\x19\n\x11with_task_options\x18\x05 \x01(\x08\x1a\xe8\x02\n\x06\x46ilter\x12\x18\n\x10\x61pplication_name\x18\x01 \x01(\t\x12\x1b\n\x13\x61pplication_version\x18\x02 \x01(\t\x12\x12\n\nsession_id\x18\x03 \x01(\t\x12\x31\n\rcreated_after\x18\x04 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x32\n\x0e\x63reated_before\x18\x05 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x33\n\x0f\x63\x61ncelled_after\x18\x06 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x34\n\x10\x63\x61ncelled_before\x18\x07 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x41\n\x06status\x18\x08 \x01(\x0e\x32\x31.armonik.api.grpc.v1.session_status.SessionStatus\x1a\xaa\x01\n\x04Sort\x12M\n\x05\x66ield\x18\x01 \x01(\x0e\x32>.armonik.api.grpc.v1.sessions.ListSessionsRequest.OrderByField\x12S\n\tdirection\x18\x02 \x01(\x0e\x32@.armonik.api.grpc.v1.sessions.ListSessionsRequest.OrderDirection\"\xa8\x01\n\x0cOrderByField\x12\x1e\n\x1aORDER_BY_FIELD_UNSPECIFIED\x10\x00\x12\x1d\n\x19ORDER_BY_FIELD_SESSION_ID\x10\x01\x12\x19\n\x15ORDER_BY_FIELD_STATUS\x10\x02\x12\x1d\n\x19ORDER_BY_FIELD_CREATED_AT\x10\x03\x12\x1f\n\x1bORDER_BY_FIELD_CANCELLED_AT\x10\x04\"d\n\x0eOrderDirection\x12\x1f\n\x1bORDER_DIRECTION_UNSPECIFIED\x10\x00\x12\x17\n\x13ORDER_DIRECTION_ASC\x10\x01\x12\x18\n\x14ORDER_DIRECTION_DESC\x10\x02\"\x86\x01\n\x14ListSessionsResponse\x12>\n\x08sessions\x18\x01 \x03(\x0b\x32,.armonik.api.grpc.v1.sessions.SessionSummary\x12\x0c\n\x04page\x18\x02 \x01(\x05\x12\x11\n\tpage_size\x18\x03 \x01(\x05\x12\r\n\x05total\x18\x04 \x01(\x05\"\'\n\x11GetSessionRequest\x12\x12\n\nsession_id\x18\x01 \x01(\t\"O\n\x12GetSessionResponse\x12\x39\n\x07session\x18\x01 \x01(\x0b\x32(.armonik.api.grpc.v1.sessions.SessionRaw\"*\n\x14\x43\x61ncelSessionRequest\x12\x12\n\nsession_id\x18\x01 \x01(\t\"R\n\x15\x43\x61ncelSessionResponse\x12\x39\n\x07session\x18\x01 \x01(\x0b\x32(.armonik.api.grpc.v1.sessions.SessionRaw\"/\n\x19\x43ountTasksByStatusRequest\x12\x12\n\nsession_id\x18\x01 \x01(\t\"N\n\x1a\x43ountTasksByStatusResponse\x12\x30\n\x06status\x18\x01 \x03(\x0b\x32 .armonik.api.grpc.v1.StatusCountB\x1f\xaa\x02\x1c\x41rmoniK.Api.gRPC.V1.Sessionsb\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x15sessions_common.proto\x12\x1c\x61rmonik.api.grpc.v1.sessions\x1a\x1egoogle/protobuf/duration.proto\x1a\x1fgoogle/protobuf/timestamp.proto\x1a\robjects.proto\x1a\x14session_status.proto\"\xbc\x02\n\nSessionRaw\x12\x12\n\nsession_id\x18\x01 \x01(\t\x12\x41\n\x06status\x18\x02 \x01(\x0e\x32\x31.armonik.api.grpc.v1.session_status.SessionStatus\x12\x15\n\rpartition_ids\x18\x03 \x03(\t\x12\x31\n\x07options\x18\x04 \x01(\x0b\x32 .armonik.api.grpc.v1.TaskOptions\x12.\n\ncreated_at\x18\x05 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x30\n\x0c\x63\x61ncelled_at\x18\x06 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12+\n\x08\x64uration\x18\x07 \x01(\x0b\x32\x19.google.protobuf.Duration\"\xa9\x02\n\x0eSessionSummary\x12\x12\n\nsession_id\x18\x01 \x01(\t\x12\x41\n\x06status\x18\x02 \x01(\x0e\x32\x31.armonik.api.grpc.v1.session_status.SessionStatus\x12.\n\ncreated_at\x18\x03 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x30\n\x0c\x63\x61ncelled_at\x18\x04 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12+\n\x08\x64uration\x18\x07 \x01(\x0b\x32\x19.google.protobuf.Duration\x12\x31\n\x07options\x18\x05 \x01(\x0b\x32 .armonik.api.grpc.v1.TaskOptions\"\x8a\x08\n\x13ListSessionsRequest\x12\x0c\n\x04page\x18\x01 \x01(\x05\x12\x11\n\tpage_size\x18\x02 \x01(\x05\x12H\n\x06\x66ilter\x18\x03 \x01(\x0b\x32\x38.armonik.api.grpc.v1.sessions.ListSessionsRequest.Filter\x12\x44\n\x04sort\x18\x04 \x01(\x0b\x32\x36.armonik.api.grpc.v1.sessions.ListSessionsRequest.Sort\x12\x19\n\x11with_task_options\x18\x05 \x01(\x08\x1a\xe8\x02\n\x06\x46ilter\x12\x18\n\x10\x61pplication_name\x18\x01 \x01(\t\x12\x1b\n\x13\x61pplication_version\x18\x02 \x01(\t\x12\x12\n\nsession_id\x18\x03 \x01(\t\x12\x31\n\rcreated_after\x18\x04 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x32\n\x0e\x63reated_before\x18\x05 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x33\n\x0f\x63\x61ncelled_after\x18\x06 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x34\n\x10\x63\x61ncelled_before\x18\x07 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x41\n\x06status\x18\x08 \x01(\x0e\x32\x31.armonik.api.grpc.v1.session_status.SessionStatus\x1a\xaa\x01\n\x04Sort\x12M\n\x05\x66ield\x18\x01 \x01(\x0e\x32>.armonik.api.grpc.v1.sessions.ListSessionsRequest.OrderByField\x12S\n\tdirection\x18\x02 \x01(\x0e\x32@.armonik.api.grpc.v1.sessions.ListSessionsRequest.OrderDirection\"\xa8\x01\n\x0cOrderByField\x12\x1e\n\x1aORDER_BY_FIELD_UNSPECIFIED\x10\x00\x12\x1d\n\x19ORDER_BY_FIELD_SESSION_ID\x10\x01\x12\x19\n\x15ORDER_BY_FIELD_STATUS\x10\x02\x12\x1d\n\x19ORDER_BY_FIELD_CREATED_AT\x10\x03\x12\x1f\n\x1bORDER_BY_FIELD_CANCELLED_AT\x10\x04\"d\n\x0eOrderDirection\x12\x1f\n\x1bORDER_DIRECTION_UNSPECIFIED\x10\x00\x12\x17\n\x13ORDER_DIRECTION_ASC\x10\x01\x12\x18\n\x14ORDER_DIRECTION_DESC\x10\x02\"\x86\x01\n\x14ListSessionsResponse\x12>\n\x08sessions\x18\x01 \x03(\x0b\x32,.armonik.api.grpc.v1.sessions.SessionSummary\x12\x0c\n\x04page\x18\x02 \x01(\x05\x12\x11\n\tpage_size\x18\x03 \x01(\x05\x12\r\n\x05total\x18\x04 \x01(\x05\"\'\n\x11GetSessionRequest\x12\x12\n\nsession_id\x18\x01 \x01(\t\"O\n\x12GetSessionResponse\x12\x39\n\x07session\x18\x01 \x01(\x0b\x32(.armonik.api.grpc.v1.sessions.SessionRaw\"*\n\x14\x43\x61ncelSessionRequest\x12\x12\n\nsession_id\x18\x01 \x01(\t\"R\n\x15\x43\x61ncelSessionResponse\x12\x39\n\x07session\x18\x01 \x01(\x0b\x32(.armonik.api.grpc.v1.sessions.SessionRaw\"/\n\x19\x43ountTasksByStatusRequest\x12\x12\n\nsession_id\x18\x01 \x01(\t\"N\n\x1a\x43ountTasksByStatusResponse\x12\x30\n\x06status\x18\x01 \x03(\x0b\x32 .armonik.api.grpc.v1.StatusCountB\x1f\xaa\x02\x1c\x41rmoniK.Api.gRPC.V1.Sessionsb\x06proto3')
 
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'sessions_common_pb2', globals())
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   DESCRIPTOR._serialized_options = b'\252\002\034ArmoniK.Api.gRPC.V1.Sessions'
-  _SESSIONRAW._serialized_start=126
-  _SESSIONRAW._serialized_end=397
-  _SESSIONSUMMARY._serialized_start=400
-  _SESSIONSUMMARY._serialized_end=652
-  _LISTSESSIONSREQUEST._serialized_start=655
-  _LISTSESSIONSREQUEST._serialized_end=1689
-  _LISTSESSIONSREQUEST_FILTER._serialized_start=883
-  _LISTSESSIONSREQUEST_FILTER._serialized_end=1243
-  _LISTSESSIONSREQUEST_SORT._serialized_start=1246
-  _LISTSESSIONSREQUEST_SORT._serialized_end=1416
-  _LISTSESSIONSREQUEST_ORDERBYFIELD._serialized_start=1419
-  _LISTSESSIONSREQUEST_ORDERBYFIELD._serialized_end=1587
-  _LISTSESSIONSREQUEST_ORDERDIRECTION._serialized_start=1589
-  _LISTSESSIONSREQUEST_ORDERDIRECTION._serialized_end=1689
-  _LISTSESSIONSRESPONSE._serialized_start=1692
-  _LISTSESSIONSRESPONSE._serialized_end=1826
-  _GETSESSIONREQUEST._serialized_start=1828
-  _GETSESSIONREQUEST._serialized_end=1867
-  _GETSESSIONRESPONSE._serialized_start=1869
-  _GETSESSIONRESPONSE._serialized_end=1948
-  _CANCELSESSIONREQUEST._serialized_start=1950
-  _CANCELSESSIONREQUEST._serialized_end=1992
-  _CANCELSESSIONRESPONSE._serialized_start=1994
-  _CANCELSESSIONRESPONSE._serialized_end=2076
-  _COUNTTASKSBYSTATUSREQUEST._serialized_start=2078
-  _COUNTTASKSBYSTATUSREQUEST._serialized_end=2125
-  _COUNTTASKSBYSTATUSRESPONSE._serialized_start=2127
-  _COUNTTASKSBYSTATUSRESPONSE._serialized_end=2205
+  _SESSIONRAW._serialized_start=158
+  _SESSIONRAW._serialized_end=474
+  _SESSIONSUMMARY._serialized_start=477
+  _SESSIONSUMMARY._serialized_end=774
+  _LISTSESSIONSREQUEST._serialized_start=777
+  _LISTSESSIONSREQUEST._serialized_end=1811
+  _LISTSESSIONSREQUEST_FILTER._serialized_start=1005
+  _LISTSESSIONSREQUEST_FILTER._serialized_end=1365
+  _LISTSESSIONSREQUEST_SORT._serialized_start=1368
+  _LISTSESSIONSREQUEST_SORT._serialized_end=1538
+  _LISTSESSIONSREQUEST_ORDERBYFIELD._serialized_start=1541
+  _LISTSESSIONSREQUEST_ORDERBYFIELD._serialized_end=1709
+  _LISTSESSIONSREQUEST_ORDERDIRECTION._serialized_start=1711
+  _LISTSESSIONSREQUEST_ORDERDIRECTION._serialized_end=1811
+  _LISTSESSIONSRESPONSE._serialized_start=1814
+  _LISTSESSIONSRESPONSE._serialized_end=1948
+  _GETSESSIONREQUEST._serialized_start=1950
+  _GETSESSIONREQUEST._serialized_end=1989
+  _GETSESSIONRESPONSE._serialized_start=1991
+  _GETSESSIONRESPONSE._serialized_end=2070
+  _CANCELSESSIONREQUEST._serialized_start=2072
+  _CANCELSESSIONREQUEST._serialized_end=2114
+  _CANCELSESSIONRESPONSE._serialized_start=2116
+  _CANCELSESSIONRESPONSE._serialized_end=2198
+  _COUNTTASKSBYSTATUSREQUEST._serialized_start=2200
+  _COUNTTASKSBYSTATUSREQUEST._serialized_end=2247
+  _COUNTTASKSBYSTATUSRESPONSE._serialized_start=2249
+  _COUNTTASKSBYSTATUSRESPONSE._serialized_end=2327
 # @@protoc_insertion_point(module_scope)
```

### Comparing `armonik-3.8.2.dev306/src/armonik/protogen/common/sessions_common_pb2.pyi` & `armonik-3.8.2.dev311/src/armonik/protogen/common/sessions_common_pb2.pyi`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+from google.protobuf import duration_pb2 as _duration_pb2
 from google.protobuf import timestamp_pb2 as _timestamp_pb2
 from . import objects_pb2 as _objects_pb2
 from . import session_status_pb2 as _session_status_pb2
 from google.protobuf.internal import containers as _containers
 from google.protobuf.internal import enum_type_wrapper as _enum_type_wrapper
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import message as _message
@@ -106,35 +107,39 @@
     page: int
     page_size: int
     sessions: _containers.RepeatedCompositeFieldContainer[SessionSummary]
     total: int
     def __init__(self, sessions: _Optional[_Iterable[_Union[SessionSummary, _Mapping]]] = ..., page: _Optional[int] = ..., page_size: _Optional[int] = ..., total: _Optional[int] = ...) -> None: ...
 
 class SessionRaw(_message.Message):
-    __slots__ = ["cancelled_at", "created_at", "options", "partition_ids", "session_id", "status"]
+    __slots__ = ["cancelled_at", "created_at", "duration", "options", "partition_ids", "session_id", "status"]
     CANCELLED_AT_FIELD_NUMBER: _ClassVar[int]
     CREATED_AT_FIELD_NUMBER: _ClassVar[int]
+    DURATION_FIELD_NUMBER: _ClassVar[int]
     OPTIONS_FIELD_NUMBER: _ClassVar[int]
     PARTITION_IDS_FIELD_NUMBER: _ClassVar[int]
     SESSION_ID_FIELD_NUMBER: _ClassVar[int]
     STATUS_FIELD_NUMBER: _ClassVar[int]
     cancelled_at: _timestamp_pb2.Timestamp
     created_at: _timestamp_pb2.Timestamp
+    duration: _duration_pb2.Duration
     options: _objects_pb2.TaskOptions
     partition_ids: _containers.RepeatedScalarFieldContainer[str]
     session_id: str
     status: _session_status_pb2.SessionStatus
-    def __init__(self, session_id: _Optional[str] = ..., status: _Optional[_Union[_session_status_pb2.SessionStatus, str]] = ..., partition_ids: _Optional[_Iterable[str]] = ..., options: _Optional[_Union[_objects_pb2.TaskOptions, _Mapping]] = ..., created_at: _Optional[_Union[_timestamp_pb2.Timestamp, _Mapping]] = ..., cancelled_at: _Optional[_Union[_timestamp_pb2.Timestamp, _Mapping]] = ...) -> None: ...
+    def __init__(self, session_id: _Optional[str] = ..., status: _Optional[_Union[_session_status_pb2.SessionStatus, str]] = ..., partition_ids: _Optional[_Iterable[str]] = ..., options: _Optional[_Union[_objects_pb2.TaskOptions, _Mapping]] = ..., created_at: _Optional[_Union[_timestamp_pb2.Timestamp, _Mapping]] = ..., cancelled_at: _Optional[_Union[_timestamp_pb2.Timestamp, _Mapping]] = ..., duration: _Optional[_Union[_duration_pb2.Duration, _Mapping]] = ...) -> None: ...
 
 class SessionSummary(_message.Message):
-    __slots__ = ["cancelled_at", "created_at", "options", "session_id", "status"]
+    __slots__ = ["cancelled_at", "created_at", "duration", "options", "session_id", "status"]
     CANCELLED_AT_FIELD_NUMBER: _ClassVar[int]
     CREATED_AT_FIELD_NUMBER: _ClassVar[int]
+    DURATION_FIELD_NUMBER: _ClassVar[int]
     OPTIONS_FIELD_NUMBER: _ClassVar[int]
     SESSION_ID_FIELD_NUMBER: _ClassVar[int]
     STATUS_FIELD_NUMBER: _ClassVar[int]
     cancelled_at: _timestamp_pb2.Timestamp
     created_at: _timestamp_pb2.Timestamp
+    duration: _duration_pb2.Duration
     options: _objects_pb2.TaskOptions
     session_id: str
     status: _session_status_pb2.SessionStatus
-    def __init__(self, session_id: _Optional[str] = ..., status: _Optional[_Union[_session_status_pb2.SessionStatus, str]] = ..., created_at: _Optional[_Union[_timestamp_pb2.Timestamp, _Mapping]] = ..., cancelled_at: _Optional[_Union[_timestamp_pb2.Timestamp, _Mapping]] = ..., options: _Optional[_Union[_objects_pb2.TaskOptions, _Mapping]] = ...) -> None: ...
+    def __init__(self, session_id: _Optional[str] = ..., status: _Optional[_Union[_session_status_pb2.SessionStatus, str]] = ..., created_at: _Optional[_Union[_timestamp_pb2.Timestamp, _Mapping]] = ..., cancelled_at: _Optional[_Union[_timestamp_pb2.Timestamp, _Mapping]] = ..., duration: _Optional[_Union[_duration_pb2.Duration, _Mapping]] = ..., options: _Optional[_Union[_objects_pb2.TaskOptions, _Mapping]] = ...) -> None: ...
```

### Comparing `armonik-3.8.2.dev306/src/armonik/protogen/common/submitter_common_pb2.py` & `armonik-3.8.2.dev311/src/armonik/protogen/common/submitter_common_pb2.py`

 * *Files identical despite different names*

### Comparing `armonik-3.8.2.dev306/src/armonik/protogen/common/submitter_common_pb2.pyi` & `armonik-3.8.2.dev311/src/armonik/protogen/common/submitter_common_pb2.pyi`

 * *Files identical despite different names*

### Comparing `armonik-3.8.2.dev306/src/armonik/protogen/common/task_status_pb2.py` & `armonik-3.8.2.dev311/src/armonik/protogen/common/task_status_pb2.py`

 * *Files identical despite different names*

### Comparing `armonik-3.8.2.dev306/src/armonik/protogen/common/task_status_pb2.pyi` & `armonik-3.8.2.dev311/src/armonik/protogen/common/task_status_pb2.pyi`

 * *Files identical despite different names*

### Comparing `armonik-3.8.2.dev306/src/armonik/protogen/common/tasks_common_pb2.py` & `armonik-3.8.2.dev311/src/armonik/protogen/common/tasks_common_pb2.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,67 +7,68 @@
 from google.protobuf import descriptor_pool as _descriptor_pool
 from google.protobuf import symbol_database as _symbol_database
 # @@protoc_insertion_point(imports)
 
 _sym_db = _symbol_database.Default()
 
 
+from google.protobuf import duration_pb2 as google_dot_protobuf_dot_duration__pb2
 from google.protobuf import timestamp_pb2 as google_dot_protobuf_dot_timestamp__pb2
 from . import objects_pb2 as objects__pb2
 from . import task_status_pb2 as task__status__pb2
 
 
-DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x12tasks_common.proto\x12\x19\x61rmonik.api.grpc.v1.tasks\x1a\x1fgoogle/protobuf/timestamp.proto\x1a\robjects.proto\x1a\x11task_status.proto\"\xf8\x05\n\x07TaskRaw\x12\n\n\x02id\x18\x01 \x01(\t\x12\x12\n\nsession_id\x18\x02 \x01(\t\x12\x14\n\x0cowner_pod_id\x18\x03 \x01(\t\x12\x17\n\x0fparent_task_ids\x18\x04 \x03(\t\x12\x19\n\x11\x64\x61ta_dependencies\x18\x05 \x03(\t\x12\x1b\n\x13\x65xpected_output_ids\x18\x06 \x03(\t\x12\x14\n\x0cretry_of_ids\x18\x07 \x03(\t\x12;\n\x06status\x18\x08 \x01(\x0e\x32+.armonik.api.grpc.v1.task_status.TaskStatus\x12\x16\n\x0estatus_message\x18\t \x01(\t\x12\x31\n\x07options\x18\n \x01(\x0b\x32 .armonik.api.grpc.v1.TaskOptions\x12.\n\ncreated_at\x18\x0b \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x30\n\x0csubmitted_at\x18\x0c \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12.\n\nstarted_at\x18\r \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12,\n\x08\x65nded_at\x18\x0e \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12+\n\x07pod_ttl\x18\x0f \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x39\n\x06output\x18\x10 \x01(\x0b\x32).armonik.api.grpc.v1.tasks.TaskRaw.Output\x12\x14\n\x0cpod_hostname\x18\x11 \x01(\t\x12/\n\x0breceived_at\x18\x12 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12/\n\x0b\x61\x63quired_at\x18\x13 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x1a(\n\x06Output\x12\x0f\n\x07success\x18\x01 \x01(\x08\x12\r\n\x05\x65rror\x18\x02 \x01(\t\"\xba\x02\n\x0bTaskSummary\x12\n\n\x02id\x18\x01 \x01(\t\x12\x12\n\nsession_id\x18\x02 \x01(\t\x12\x31\n\x07options\x18\x03 \x01(\x0b\x32 .armonik.api.grpc.v1.TaskOptions\x12;\n\x06status\x18\x04 \x01(\x0e\x32+.armonik.api.grpc.v1.task_status.TaskStatus\x12.\n\ncreated_at\x18\x05 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12.\n\nstarted_at\x18\x06 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12,\n\x08\x65nded_at\x18\x07 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\r\n\x05\x65rror\x18\x08 \x01(\t\"\xc2\x08\n\x10ListTasksRequest\x12\x0c\n\x04page\x18\x01 \x01(\x05\x12\x11\n\tpage_size\x18\x02 \x01(\x05\x12\x42\n\x06\x66ilter\x18\x03 \x01(\x0b\x32\x32.armonik.api.grpc.v1.tasks.ListTasksRequest.Filter\x12>\n\x04sort\x18\x04 \x01(\x0b\x32\x30.armonik.api.grpc.v1.tasks.ListTasksRequest.Sort\x12\x13\n\x0bwith_errors\x18\x05 \x01(\x08\x1a\x8a\x03\n\x06\x46ilter\x12\x12\n\nsession_id\x18\x01 \x01(\t\x12;\n\x06status\x18\x02 \x03(\x0e\x32+.armonik.api.grpc.v1.task_status.TaskStatus\x12\x31\n\rcreated_after\x18\x03 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x32\n\x0e\x63reated_before\x18\x04 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x31\n\rstarted_after\x18\x05 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x32\n\x0estarted_before\x18\x06 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12/\n\x0b\x65nded_after\x18\x07 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x30\n\x0c\x65nded_before\x18\x08 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x1a\x9e\x01\n\x04Sort\x12G\n\x05\x66ield\x18\x01 \x01(\x0e\x32\x38.armonik.api.grpc.v1.tasks.ListTasksRequest.OrderByField\x12M\n\tdirection\x18\x02 \x01(\x0e\x32:.armonik.api.grpc.v1.tasks.ListTasksRequest.OrderDirection\"\xdf\x01\n\x0cOrderByField\x12\x1e\n\x1aORDER_BY_FIELD_UNSPECIFIED\x10\x00\x12\x1a\n\x16ORDER_BY_FIELD_TASK_ID\x10\x01\x12\x1d\n\x19ORDER_BY_FIELD_SESSION_ID\x10\x02\x12\x19\n\x15ORDER_BY_FIELD_STATUS\x10\x03\x12\x1d\n\x19ORDER_BY_FIELD_CREATED_AT\x10\x04\x12\x1d\n\x19ORDER_BY_FIELD_STARTED_AT\x10\x05\x12\x1b\n\x17ORDER_BY_FIELD_ENDED_AT\x10\x06\"d\n\x0eOrderDirection\x12\x1f\n\x1bORDER_DIRECTION_UNSPECIFIED\x10\x00\x12\x17\n\x13ORDER_DIRECTION_ASC\x10\x01\x12\x18\n\x14ORDER_DIRECTION_DESC\x10\x02\"z\n\x11ListTasksResponse\x12\x35\n\x05tasks\x18\x01 \x03(\x0b\x32&.armonik.api.grpc.v1.tasks.TaskSummary\x12\x0c\n\x04page\x18\x02 \x01(\x05\x12\x11\n\tpage_size\x18\x03 \x01(\x05\x12\r\n\x05total\x18\x04 \x01(\x05\"y\n\x14ListTasksRawResponse\x12\x31\n\x05tasks\x18\x01 \x03(\x0b\x32\".armonik.api.grpc.v1.tasks.TaskRaw\x12\x0c\n\x04page\x18\x02 \x01(\x05\x12\x11\n\tpage_size\x18\x03 \x01(\x05\x12\r\n\x05total\x18\x04 \x01(\x05\"!\n\x0eGetTaskRequest\x12\x0f\n\x07task_id\x18\x01 \x01(\t\"C\n\x0fGetTaskResponse\x12\x30\n\x04task\x18\x01 \x01(\x0b\x32\".armonik.api.grpc.v1.tasks.TaskRaw\"&\n\x12\x43\x61ncelTasksRequest\x12\x10\n\x08task_ids\x18\x01 \x03(\t\"L\n\x13\x43\x61ncelTasksResponse\x12\x35\n\x05tasks\x18\x01 \x03(\x0b\x32&.armonik.api.grpc.v1.tasks.TaskSummary\"&\n\x13GetResultIdsRequest\x12\x0f\n\x07task_id\x18\x01 \x03(\t\"\xa1\x01\n\x14GetResultIdsResponse\x12S\n\x0ctask_results\x18\x01 \x03(\x0b\x32=.armonik.api.grpc.v1.tasks.GetResultIdsResponse.MapTaskResult\x1a\x34\n\rMapTaskResult\x12\x0f\n\x07task_id\x18\x01 \x01(\t\x12\x12\n\nresult_ids\x18\x02 \x03(\t\"\x1b\n\x19\x43ountTasksByStatusRequest\"N\n\x1a\x43ountTasksByStatusResponse\x12\x30\n\x06status\x18\x01 \x03(\x0b\x32 .armonik.api.grpc.v1.StatusCount\"\xca\x02\n\x12SubmitTasksRequest\x12\x12\n\nsession_id\x18\x01 \x01(\t\x12\x36\n\x0ctask_options\x18\x02 \x01(\x0b\x32 .armonik.api.grpc.v1.TaskOptions\x12R\n\x0etask_creations\x18\x03 \x03(\x0b\x32:.armonik.api.grpc.v1.tasks.SubmitTasksRequest.TaskCreation\x1a\x93\x01\n\x0cTaskCreation\x12\x1c\n\x14\x65xpected_output_keys\x18\x01 \x03(\t\x12\x19\n\x11\x64\x61ta_dependencies\x18\x02 \x03(\t\x12\x12\n\npayload_id\x18\x03 \x01(\t\x12\x36\n\x0ctask_options\x18\x04 \x01(\x0b\x32 .armonik.api.grpc.v1.TaskOptions\"\xcb\x01\n\x13SubmitTasksResponse\x12K\n\ntask_infos\x18\x01 \x03(\x0b\x32\x37.armonik.api.grpc.v1.tasks.SubmitTasksResponse.TaskInfo\x1ag\n\x08TaskInfo\x12\x0f\n\x07task_id\x18\x01 \x01(\t\x12\x1b\n\x13\x65xpected_output_ids\x18\x02 \x03(\t\x12\x19\n\x11\x64\x61ta_dependencies\x18\x03 \x03(\t\x12\x12\n\npayload_id\x18\x04 \x01(\tB\x1c\xaa\x02\x19\x41rmoniK.Api.gRPC.V1.Tasksb\x06proto3')
+DESCRIPTOR = _descriptor_pool.Default().AddSerializedFile(b'\n\x12tasks_common.proto\x12\x19\x61rmonik.api.grpc.v1.tasks\x1a\x1egoogle/protobuf/duration.proto\x1a\x1fgoogle/protobuf/timestamp.proto\x1a\robjects.proto\x1a\x11task_status.proto\"\xf4\x06\n\x07TaskRaw\x12\n\n\x02id\x18\x01 \x01(\t\x12\x12\n\nsession_id\x18\x02 \x01(\t\x12\x14\n\x0cowner_pod_id\x18\x03 \x01(\t\x12\x17\n\x0fparent_task_ids\x18\x04 \x03(\t\x12\x19\n\x11\x64\x61ta_dependencies\x18\x05 \x03(\t\x12\x1b\n\x13\x65xpected_output_ids\x18\x06 \x03(\t\x12\x14\n\x0cretry_of_ids\x18\x07 \x03(\t\x12;\n\x06status\x18\x08 \x01(\x0e\x32+.armonik.api.grpc.v1.task_status.TaskStatus\x12\x16\n\x0estatus_message\x18\t \x01(\t\x12\x31\n\x07options\x18\n \x01(\x0b\x32 .armonik.api.grpc.v1.TaskOptions\x12.\n\ncreated_at\x18\x0b \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x30\n\x0csubmitted_at\x18\x0c \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12.\n\nstarted_at\x18\r \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12,\n\x08\x65nded_at\x18\x0e \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12;\n\x18\x63reation_to_end_duration\x18\x14 \x01(\x0b\x32\x19.google.protobuf.Duration\x12=\n\x1aprocessing_to_end_duration\x18\x15 \x01(\x0b\x32\x19.google.protobuf.Duration\x12+\n\x07pod_ttl\x18\x0f \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x39\n\x06output\x18\x10 \x01(\x0b\x32).armonik.api.grpc.v1.tasks.TaskRaw.Output\x12\x14\n\x0cpod_hostname\x18\x11 \x01(\t\x12/\n\x0breceived_at\x18\x12 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12/\n\x0b\x61\x63quired_at\x18\x13 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x1a(\n\x06Output\x12\x0f\n\x07success\x18\x01 \x01(\x08\x12\r\n\x05\x65rror\x18\x02 \x01(\t\"\xb6\x03\n\x0bTaskSummary\x12\n\n\x02id\x18\x01 \x01(\t\x12\x12\n\nsession_id\x18\x02 \x01(\t\x12\x31\n\x07options\x18\x03 \x01(\x0b\x32 .armonik.api.grpc.v1.TaskOptions\x12;\n\x06status\x18\x04 \x01(\x0e\x32+.armonik.api.grpc.v1.task_status.TaskStatus\x12.\n\ncreated_at\x18\x05 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12.\n\nstarted_at\x18\x06 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12,\n\x08\x65nded_at\x18\x07 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12;\n\x18\x63reation_to_end_duration\x18\x0f \x01(\x0b\x32\x19.google.protobuf.Duration\x12=\n\x1aprocessing_to_end_duration\x18\x10 \x01(\x0b\x32\x19.google.protobuf.Duration\x12\r\n\x05\x65rror\x18\x08 \x01(\t\"\xc2\x08\n\x10ListTasksRequest\x12\x0c\n\x04page\x18\x01 \x01(\x05\x12\x11\n\tpage_size\x18\x02 \x01(\x05\x12\x42\n\x06\x66ilter\x18\x03 \x01(\x0b\x32\x32.armonik.api.grpc.v1.tasks.ListTasksRequest.Filter\x12>\n\x04sort\x18\x04 \x01(\x0b\x32\x30.armonik.api.grpc.v1.tasks.ListTasksRequest.Sort\x12\x13\n\x0bwith_errors\x18\x05 \x01(\x08\x1a\x8a\x03\n\x06\x46ilter\x12\x12\n\nsession_id\x18\x01 \x01(\t\x12;\n\x06status\x18\x02 \x03(\x0e\x32+.armonik.api.grpc.v1.task_status.TaskStatus\x12\x31\n\rcreated_after\x18\x03 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x32\n\x0e\x63reated_before\x18\x04 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x31\n\rstarted_after\x18\x05 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x32\n\x0estarted_before\x18\x06 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12/\n\x0b\x65nded_after\x18\x07 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x12\x30\n\x0c\x65nded_before\x18\x08 \x01(\x0b\x32\x1a.google.protobuf.Timestamp\x1a\x9e\x01\n\x04Sort\x12G\n\x05\x66ield\x18\x01 \x01(\x0e\x32\x38.armonik.api.grpc.v1.tasks.ListTasksRequest.OrderByField\x12M\n\tdirection\x18\x02 \x01(\x0e\x32:.armonik.api.grpc.v1.tasks.ListTasksRequest.OrderDirection\"\xdf\x01\n\x0cOrderByField\x12\x1e\n\x1aORDER_BY_FIELD_UNSPECIFIED\x10\x00\x12\x1a\n\x16ORDER_BY_FIELD_TASK_ID\x10\x01\x12\x1d\n\x19ORDER_BY_FIELD_SESSION_ID\x10\x02\x12\x19\n\x15ORDER_BY_FIELD_STATUS\x10\x03\x12\x1d\n\x19ORDER_BY_FIELD_CREATED_AT\x10\x04\x12\x1d\n\x19ORDER_BY_FIELD_STARTED_AT\x10\x05\x12\x1b\n\x17ORDER_BY_FIELD_ENDED_AT\x10\x06\"d\n\x0eOrderDirection\x12\x1f\n\x1bORDER_DIRECTION_UNSPECIFIED\x10\x00\x12\x17\n\x13ORDER_DIRECTION_ASC\x10\x01\x12\x18\n\x14ORDER_DIRECTION_DESC\x10\x02\"z\n\x11ListTasksResponse\x12\x35\n\x05tasks\x18\x01 \x03(\x0b\x32&.armonik.api.grpc.v1.tasks.TaskSummary\x12\x0c\n\x04page\x18\x02 \x01(\x05\x12\x11\n\tpage_size\x18\x03 \x01(\x05\x12\r\n\x05total\x18\x04 \x01(\x05\"y\n\x14ListTasksRawResponse\x12\x31\n\x05tasks\x18\x01 \x03(\x0b\x32\".armonik.api.grpc.v1.tasks.TaskRaw\x12\x0c\n\x04page\x18\x02 \x01(\x05\x12\x11\n\tpage_size\x18\x03 \x01(\x05\x12\r\n\x05total\x18\x04 \x01(\x05\"!\n\x0eGetTaskRequest\x12\x0f\n\x07task_id\x18\x01 \x01(\t\"C\n\x0fGetTaskResponse\x12\x30\n\x04task\x18\x01 \x01(\x0b\x32\".armonik.api.grpc.v1.tasks.TaskRaw\"&\n\x12\x43\x61ncelTasksRequest\x12\x10\n\x08task_ids\x18\x01 \x03(\t\"L\n\x13\x43\x61ncelTasksResponse\x12\x35\n\x05tasks\x18\x01 \x03(\x0b\x32&.armonik.api.grpc.v1.tasks.TaskSummary\"&\n\x13GetResultIdsRequest\x12\x0f\n\x07task_id\x18\x01 \x03(\t\"\xa1\x01\n\x14GetResultIdsResponse\x12S\n\x0ctask_results\x18\x01 \x03(\x0b\x32=.armonik.api.grpc.v1.tasks.GetResultIdsResponse.MapTaskResult\x1a\x34\n\rMapTaskResult\x12\x0f\n\x07task_id\x18\x01 \x01(\t\x12\x12\n\nresult_ids\x18\x02 \x03(\t\"\x1b\n\x19\x43ountTasksByStatusRequest\"N\n\x1a\x43ountTasksByStatusResponse\x12\x30\n\x06status\x18\x01 \x03(\x0b\x32 .armonik.api.grpc.v1.StatusCount\"\xca\x02\n\x12SubmitTasksRequest\x12\x12\n\nsession_id\x18\x01 \x01(\t\x12\x36\n\x0ctask_options\x18\x02 \x01(\x0b\x32 .armonik.api.grpc.v1.TaskOptions\x12R\n\x0etask_creations\x18\x03 \x03(\x0b\x32:.armonik.api.grpc.v1.tasks.SubmitTasksRequest.TaskCreation\x1a\x93\x01\n\x0cTaskCreation\x12\x1c\n\x14\x65xpected_output_keys\x18\x01 \x03(\t\x12\x19\n\x11\x64\x61ta_dependencies\x18\x02 \x03(\t\x12\x12\n\npayload_id\x18\x03 \x01(\t\x12\x36\n\x0ctask_options\x18\x04 \x01(\x0b\x32 .armonik.api.grpc.v1.TaskOptions\"\xcb\x01\n\x13SubmitTasksResponse\x12K\n\ntask_infos\x18\x01 \x03(\x0b\x32\x37.armonik.api.grpc.v1.tasks.SubmitTasksResponse.TaskInfo\x1ag\n\x08TaskInfo\x12\x0f\n\x07task_id\x18\x01 \x01(\t\x12\x1b\n\x13\x65xpected_output_ids\x18\x02 \x03(\t\x12\x19\n\x11\x64\x61ta_dependencies\x18\x03 \x03(\t\x12\x12\n\npayload_id\x18\x04 \x01(\tB\x1c\xaa\x02\x19\x41rmoniK.Api.gRPC.V1.Tasksb\x06proto3')
 
 _builder.BuildMessageAndEnumDescriptors(DESCRIPTOR, globals())
 _builder.BuildTopDescriptorsAndMessages(DESCRIPTOR, 'tasks_common_pb2', globals())
 if _descriptor._USE_C_DESCRIPTORS == False:
 
   DESCRIPTOR._options = None
   DESCRIPTOR._serialized_options = b'\252\002\031ArmoniK.Api.gRPC.V1.Tasks'
-  _TASKRAW._serialized_start=117
-  _TASKRAW._serialized_end=877
-  _TASKRAW_OUTPUT._serialized_start=837
-  _TASKRAW_OUTPUT._serialized_end=877
-  _TASKSUMMARY._serialized_start=880
-  _TASKSUMMARY._serialized_end=1194
-  _LISTTASKSREQUEST._serialized_start=1197
-  _LISTTASKSREQUEST._serialized_end=2287
-  _LISTTASKSREQUEST_FILTER._serialized_start=1404
-  _LISTTASKSREQUEST_FILTER._serialized_end=1798
-  _LISTTASKSREQUEST_SORT._serialized_start=1801
-  _LISTTASKSREQUEST_SORT._serialized_end=1959
-  _LISTTASKSREQUEST_ORDERBYFIELD._serialized_start=1962
-  _LISTTASKSREQUEST_ORDERBYFIELD._serialized_end=2185
-  _LISTTASKSREQUEST_ORDERDIRECTION._serialized_start=2187
-  _LISTTASKSREQUEST_ORDERDIRECTION._serialized_end=2287
-  _LISTTASKSRESPONSE._serialized_start=2289
-  _LISTTASKSRESPONSE._serialized_end=2411
-  _LISTTASKSRAWRESPONSE._serialized_start=2413
-  _LISTTASKSRAWRESPONSE._serialized_end=2534
-  _GETTASKREQUEST._serialized_start=2536
-  _GETTASKREQUEST._serialized_end=2569
-  _GETTASKRESPONSE._serialized_start=2571
-  _GETTASKRESPONSE._serialized_end=2638
-  _CANCELTASKSREQUEST._serialized_start=2640
-  _CANCELTASKSREQUEST._serialized_end=2678
-  _CANCELTASKSRESPONSE._serialized_start=2680
-  _CANCELTASKSRESPONSE._serialized_end=2756
-  _GETRESULTIDSREQUEST._serialized_start=2758
-  _GETRESULTIDSREQUEST._serialized_end=2796
-  _GETRESULTIDSRESPONSE._serialized_start=2799
-  _GETRESULTIDSRESPONSE._serialized_end=2960
-  _GETRESULTIDSRESPONSE_MAPTASKRESULT._serialized_start=2908
-  _GETRESULTIDSRESPONSE_MAPTASKRESULT._serialized_end=2960
-  _COUNTTASKSBYSTATUSREQUEST._serialized_start=2962
-  _COUNTTASKSBYSTATUSREQUEST._serialized_end=2989
-  _COUNTTASKSBYSTATUSRESPONSE._serialized_start=2991
-  _COUNTTASKSBYSTATUSRESPONSE._serialized_end=3069
-  _SUBMITTASKSREQUEST._serialized_start=3072
-  _SUBMITTASKSREQUEST._serialized_end=3402
-  _SUBMITTASKSREQUEST_TASKCREATION._serialized_start=3255
-  _SUBMITTASKSREQUEST_TASKCREATION._serialized_end=3402
-  _SUBMITTASKSRESPONSE._serialized_start=3405
-  _SUBMITTASKSRESPONSE._serialized_end=3608
-  _SUBMITTASKSRESPONSE_TASKINFO._serialized_start=3505
-  _SUBMITTASKSRESPONSE_TASKINFO._serialized_end=3608
+  _TASKRAW._serialized_start=149
+  _TASKRAW._serialized_end=1033
+  _TASKRAW_OUTPUT._serialized_start=993
+  _TASKRAW_OUTPUT._serialized_end=1033
+  _TASKSUMMARY._serialized_start=1036
+  _TASKSUMMARY._serialized_end=1474
+  _LISTTASKSREQUEST._serialized_start=1477
+  _LISTTASKSREQUEST._serialized_end=2567
+  _LISTTASKSREQUEST_FILTER._serialized_start=1684
+  _LISTTASKSREQUEST_FILTER._serialized_end=2078
+  _LISTTASKSREQUEST_SORT._serialized_start=2081
+  _LISTTASKSREQUEST_SORT._serialized_end=2239
+  _LISTTASKSREQUEST_ORDERBYFIELD._serialized_start=2242
+  _LISTTASKSREQUEST_ORDERBYFIELD._serialized_end=2465
+  _LISTTASKSREQUEST_ORDERDIRECTION._serialized_start=2467
+  _LISTTASKSREQUEST_ORDERDIRECTION._serialized_end=2567
+  _LISTTASKSRESPONSE._serialized_start=2569
+  _LISTTASKSRESPONSE._serialized_end=2691
+  _LISTTASKSRAWRESPONSE._serialized_start=2693
+  _LISTTASKSRAWRESPONSE._serialized_end=2814
+  _GETTASKREQUEST._serialized_start=2816
+  _GETTASKREQUEST._serialized_end=2849
+  _GETTASKRESPONSE._serialized_start=2851
+  _GETTASKRESPONSE._serialized_end=2918
+  _CANCELTASKSREQUEST._serialized_start=2920
+  _CANCELTASKSREQUEST._serialized_end=2958
+  _CANCELTASKSRESPONSE._serialized_start=2960
+  _CANCELTASKSRESPONSE._serialized_end=3036
+  _GETRESULTIDSREQUEST._serialized_start=3038
+  _GETRESULTIDSREQUEST._serialized_end=3076
+  _GETRESULTIDSRESPONSE._serialized_start=3079
+  _GETRESULTIDSRESPONSE._serialized_end=3240
+  _GETRESULTIDSRESPONSE_MAPTASKRESULT._serialized_start=3188
+  _GETRESULTIDSRESPONSE_MAPTASKRESULT._serialized_end=3240
+  _COUNTTASKSBYSTATUSREQUEST._serialized_start=3242
+  _COUNTTASKSBYSTATUSREQUEST._serialized_end=3269
+  _COUNTTASKSBYSTATUSRESPONSE._serialized_start=3271
+  _COUNTTASKSBYSTATUSRESPONSE._serialized_end=3349
+  _SUBMITTASKSREQUEST._serialized_start=3352
+  _SUBMITTASKSREQUEST._serialized_end=3682
+  _SUBMITTASKSREQUEST_TASKCREATION._serialized_start=3535
+  _SUBMITTASKSREQUEST_TASKCREATION._serialized_end=3682
+  _SUBMITTASKSRESPONSE._serialized_start=3685
+  _SUBMITTASKSRESPONSE._serialized_end=3888
+  _SUBMITTASKSRESPONSE_TASKINFO._serialized_start=3785
+  _SUBMITTASKSRESPONSE_TASKINFO._serialized_end=3888
 # @@protoc_insertion_point(module_scope)
```

### Comparing `armonik-3.8.2.dev306/src/armonik/protogen/common/tasks_common_pb2.pyi` & `armonik-3.8.2.dev311/src/armonik/protogen/common/tasks_common_pb2.pyi`

 * *Files 8% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+from google.protobuf import duration_pb2 as _duration_pb2
 from google.protobuf import timestamp_pb2 as _timestamp_pb2
 from . import objects_pb2 as _objects_pb2
 from . import task_status_pb2 as _task_status_pb2
 from google.protobuf.internal import containers as _containers
 from google.protobuf.internal import enum_type_wrapper as _enum_type_wrapper
 from google.protobuf import descriptor as _descriptor
 from google.protobuf import message as _message
@@ -175,74 +176,82 @@
         task_id: str
         def __init__(self, task_id: _Optional[str] = ..., expected_output_ids: _Optional[_Iterable[str]] = ..., data_dependencies: _Optional[_Iterable[str]] = ..., payload_id: _Optional[str] = ...) -> None: ...
     TASK_INFOS_FIELD_NUMBER: _ClassVar[int]
     task_infos: _containers.RepeatedCompositeFieldContainer[SubmitTasksResponse.TaskInfo]
     def __init__(self, task_infos: _Optional[_Iterable[_Union[SubmitTasksResponse.TaskInfo, _Mapping]]] = ...) -> None: ...
 
 class TaskRaw(_message.Message):
-    __slots__ = ["acquired_at", "created_at", "data_dependencies", "ended_at", "expected_output_ids", "id", "options", "output", "owner_pod_id", "parent_task_ids", "pod_hostname", "pod_ttl", "received_at", "retry_of_ids", "session_id", "started_at", "status", "status_message", "submitted_at"]
+    __slots__ = ["acquired_at", "created_at", "creation_to_end_duration", "data_dependencies", "ended_at", "expected_output_ids", "id", "options", "output", "owner_pod_id", "parent_task_ids", "pod_hostname", "pod_ttl", "processing_to_end_duration", "received_at", "retry_of_ids", "session_id", "started_at", "status", "status_message", "submitted_at"]
     class Output(_message.Message):
         __slots__ = ["error", "success"]
         ERROR_FIELD_NUMBER: _ClassVar[int]
         SUCCESS_FIELD_NUMBER: _ClassVar[int]
         error: str
         success: bool
         def __init__(self, success: bool = ..., error: _Optional[str] = ...) -> None: ...
     ACQUIRED_AT_FIELD_NUMBER: _ClassVar[int]
     CREATED_AT_FIELD_NUMBER: _ClassVar[int]
+    CREATION_TO_END_DURATION_FIELD_NUMBER: _ClassVar[int]
     DATA_DEPENDENCIES_FIELD_NUMBER: _ClassVar[int]
     ENDED_AT_FIELD_NUMBER: _ClassVar[int]
     EXPECTED_OUTPUT_IDS_FIELD_NUMBER: _ClassVar[int]
     ID_FIELD_NUMBER: _ClassVar[int]
     OPTIONS_FIELD_NUMBER: _ClassVar[int]
     OUTPUT_FIELD_NUMBER: _ClassVar[int]
     OWNER_POD_ID_FIELD_NUMBER: _ClassVar[int]
     PARENT_TASK_IDS_FIELD_NUMBER: _ClassVar[int]
     POD_HOSTNAME_FIELD_NUMBER: _ClassVar[int]
     POD_TTL_FIELD_NUMBER: _ClassVar[int]
+    PROCESSING_TO_END_DURATION_FIELD_NUMBER: _ClassVar[int]
     RECEIVED_AT_FIELD_NUMBER: _ClassVar[int]
     RETRY_OF_IDS_FIELD_NUMBER: _ClassVar[int]
     SESSION_ID_FIELD_NUMBER: _ClassVar[int]
     STARTED_AT_FIELD_NUMBER: _ClassVar[int]
     STATUS_FIELD_NUMBER: _ClassVar[int]
     STATUS_MESSAGE_FIELD_NUMBER: _ClassVar[int]
     SUBMITTED_AT_FIELD_NUMBER: _ClassVar[int]
     acquired_at: _timestamp_pb2.Timestamp
     created_at: _timestamp_pb2.Timestamp
+    creation_to_end_duration: _duration_pb2.Duration
     data_dependencies: _containers.RepeatedScalarFieldContainer[str]
     ended_at: _timestamp_pb2.Timestamp
     expected_output_ids: _containers.RepeatedScalarFieldContainer[str]
     id: str
     options: _objects_pb2.TaskOptions
     output: TaskRaw.Output
     owner_pod_id: str
     parent_task_ids: _containers.RepeatedScalarFieldContainer[str]
     pod_hostname: str
     pod_ttl: _timestamp_pb2.Timestamp
+    processing_to_end_duration: _duration_pb2.Duration
     received_at: _timestamp_pb2.Timestamp
     retry_of_ids: _containers.RepeatedScalarFieldContainer[str]
     session_id: str
     started_at: _timestamp_pb2.Timestamp
     status: _task_status_pb2.TaskStatus
     status_message: str
     submitted_at: _timestamp_pb2.Timestamp
-    def __init__(self, id: _Optional[str] = ..., session_id: _Optional[str] = ..., owner_pod_id: _Optional[str] = ..., parent_task_ids: _Optional[_Iterable[str]] = ..., data_dependencies: _Optional[_Iterable[str]] = ..., expected_output_ids: _Optional[_Iterable[str]] = ..., retry_of_ids: _Optional[_Iterable[str]] = ..., status: _Optional[_Union[_task_status_pb2.TaskStatus, str]] = ..., status_message: _Optional[str] = ..., options: _Optional[_Union[_objects_pb2.TaskOptions, _Mapping]] = ..., created_at: _Optional[_Union[_timestamp_pb2.Timestamp, _Mapping]] = ..., submitted_at: _Optional[_Union[_timestamp_pb2.Timestamp, _Mapping]] = ..., started_at: _Optional[_Union[_timestamp_pb2.Timestamp, _Mapping]] = ..., ended_at: _Optional[_Union[_timestamp_pb2.Timestamp, _Mapping]] = ..., pod_ttl: _Optional[_Union[_timestamp_pb2.Timestamp, _Mapping]] = ..., output: _Optional[_Union[TaskRaw.Output, _Mapping]] = ..., pod_hostname: _Optional[str] = ..., received_at: _Optional[_Union[_timestamp_pb2.Timestamp, _Mapping]] = ..., acquired_at: _Optional[_Union[_timestamp_pb2.Timestamp, _Mapping]] = ...) -> None: ...
+    def __init__(self, id: _Optional[str] = ..., session_id: _Optional[str] = ..., owner_pod_id: _Optional[str] = ..., parent_task_ids: _Optional[_Iterable[str]] = ..., data_dependencies: _Optional[_Iterable[str]] = ..., expected_output_ids: _Optional[_Iterable[str]] = ..., retry_of_ids: _Optional[_Iterable[str]] = ..., status: _Optional[_Union[_task_status_pb2.TaskStatus, str]] = ..., status_message: _Optional[str] = ..., options: _Optional[_Union[_objects_pb2.TaskOptions, _Mapping]] = ..., created_at: _Optional[_Union[_timestamp_pb2.Timestamp, _Mapping]] = ..., submitted_at: _Optional[_Union[_timestamp_pb2.Timestamp, _Mapping]] = ..., started_at: _Optional[_Union[_timestamp_pb2.Timestamp, _Mapping]] = ..., ended_at: _Optional[_Union[_timestamp_pb2.Timestamp, _Mapping]] = ..., creation_to_end_duration: _Optional[_Union[_duration_pb2.Duration, _Mapping]] = ..., processing_to_end_duration: _Optional[_Union[_duration_pb2.Duration, _Mapping]] = ..., pod_ttl: _Optional[_Union[_timestamp_pb2.Timestamp, _Mapping]] = ..., output: _Optional[_Union[TaskRaw.Output, _Mapping]] = ..., pod_hostname: _Optional[str] = ..., received_at: _Optional[_Union[_timestamp_pb2.Timestamp, _Mapping]] = ..., acquired_at: _Optional[_Union[_timestamp_pb2.Timestamp, _Mapping]] = ...) -> None: ...
 
 class TaskSummary(_message.Message):
-    __slots__ = ["created_at", "ended_at", "error", "id", "options", "session_id", "started_at", "status"]
+    __slots__ = ["created_at", "creation_to_end_duration", "ended_at", "error", "id", "options", "processing_to_end_duration", "session_id", "started_at", "status"]
     CREATED_AT_FIELD_NUMBER: _ClassVar[int]
+    CREATION_TO_END_DURATION_FIELD_NUMBER: _ClassVar[int]
     ENDED_AT_FIELD_NUMBER: _ClassVar[int]
     ERROR_FIELD_NUMBER: _ClassVar[int]
     ID_FIELD_NUMBER: _ClassVar[int]
     OPTIONS_FIELD_NUMBER: _ClassVar[int]
+    PROCESSING_TO_END_DURATION_FIELD_NUMBER: _ClassVar[int]
     SESSION_ID_FIELD_NUMBER: _ClassVar[int]
     STARTED_AT_FIELD_NUMBER: _ClassVar[int]
     STATUS_FIELD_NUMBER: _ClassVar[int]
     created_at: _timestamp_pb2.Timestamp
+    creation_to_end_duration: _duration_pb2.Duration
     ended_at: _timestamp_pb2.Timestamp
     error: str
     id: str
     options: _objects_pb2.TaskOptions
+    processing_to_end_duration: _duration_pb2.Duration
     session_id: str
     started_at: _timestamp_pb2.Timestamp
     status: _task_status_pb2.TaskStatus
-    def __init__(self, id: _Optional[str] = ..., session_id: _Optional[str] = ..., options: _Optional[_Union[_objects_pb2.TaskOptions, _Mapping]] = ..., status: _Optional[_Union[_task_status_pb2.TaskStatus, str]] = ..., created_at: _Optional[_Union[_timestamp_pb2.Timestamp, _Mapping]] = ..., started_at: _Optional[_Union[_timestamp_pb2.Timestamp, _Mapping]] = ..., ended_at: _Optional[_Union[_timestamp_pb2.Timestamp, _Mapping]] = ..., error: _Optional[str] = ...) -> None: ...
+    def __init__(self, id: _Optional[str] = ..., session_id: _Optional[str] = ..., options: _Optional[_Union[_objects_pb2.TaskOptions, _Mapping]] = ..., status: _Optional[_Union[_task_status_pb2.TaskStatus, str]] = ..., created_at: _Optional[_Union[_timestamp_pb2.Timestamp, _Mapping]] = ..., started_at: _Optional[_Union[_timestamp_pb2.Timestamp, _Mapping]] = ..., ended_at: _Optional[_Union[_timestamp_pb2.Timestamp, _Mapping]] = ..., creation_to_end_duration: _Optional[_Union[_duration_pb2.Duration, _Mapping]] = ..., processing_to_end_duration: _Optional[_Union[_duration_pb2.Duration, _Mapping]] = ..., error: _Optional[str] = ...) -> None: ...
```

### Comparing `armonik-3.8.2.dev306/src/armonik/protogen/common/worker_common_pb2.py` & `armonik-3.8.2.dev311/src/armonik/protogen/common/worker_common_pb2.py`

 * *Files identical despite different names*

### Comparing `armonik-3.8.2.dev306/src/armonik/protogen/common/worker_common_pb2.pyi` & `armonik-3.8.2.dev311/src/armonik/protogen/common/worker_common_pb2.pyi`

 * *Files identical despite different names*

### Comparing `armonik-3.8.2.dev306/src/armonik/protogen/worker/agent_service_pb2.py` & `armonik-3.8.2.dev311/src/armonik/protogen/worker/agent_service_pb2.py`

 * *Files identical despite different names*

### Comparing `armonik-3.8.2.dev306/src/armonik/protogen/worker/agent_service_pb2_grpc.py` & `armonik-3.8.2.dev311/src/armonik/protogen/worker/agent_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `armonik-3.8.2.dev306/src/armonik/protogen/worker/worker_service_pb2.py` & `armonik-3.8.2.dev311/src/armonik/protogen/worker/worker_service_pb2.py`

 * *Files identical despite different names*

### Comparing `armonik-3.8.2.dev306/src/armonik/protogen/worker/worker_service_pb2_grpc.py` & `armonik-3.8.2.dev311/src/armonik/protogen/worker/worker_service_pb2_grpc.py`

 * *Files identical despite different names*

### Comparing `armonik-3.8.2.dev306/src/armonik/worker/seqlogger.py` & `armonik-3.8.2.dev311/src/armonik/worker/seqlogger.py`

 * *Files identical despite different names*

### Comparing `armonik-3.8.2.dev306/src/armonik/worker/taskhandler.py` & `armonik-3.8.2.dev311/src/armonik/worker/taskhandler.py`

 * *Files identical despite different names*

### Comparing `armonik-3.8.2.dev306/src/armonik/worker/worker.py` & `armonik-3.8.2.dev311/src/armonik/worker/worker.py`

 * *Files identical despite different names*

### Comparing `armonik-3.8.2.dev306/src/armonik.egg-info/PKG-INFO` & `armonik-3.8.2.dev311/src/armonik.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: armonik
-Version: 3.8.2.dev306
+Version: 3.8.2.dev311
 Summary: GRPC python binding for the ArmoniK orchestrator API
 License: Apache v2.0 LICENSE
 Project-URL: Homepage, https://github.com/aneoconsulting/ArmoniK.Api
 Project-URL: Bug Tracker, https://github.com/aneoconsulting/ArmoniK/issues
 Keywords: cloud,HTC,gRPC,ArmoniK,Aneo
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
```

### Comparing `armonik-3.8.2.dev306/src/armonik.egg-info/SOURCES.txt` & `armonik-3.8.2.dev311/src/armonik.egg-info/SOURCES.txt`

 * *Files identical despite different names*

