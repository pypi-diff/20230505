# Comparing `tmp/yohsin3d-0.3.0.tar.gz` & `tmp/yohsin3d-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yohsin3d-0.3.0.tar", last modified: Wed Apr 12 23:18:25 2023, max compression
+gzip compressed data, was "yohsin3d-0.4.0.tar", last modified: Fri May  5 13:15:51 2023, max compression
```

## Comparing `yohsin3d-0.3.0.tar` & `yohsin3d-0.4.0.tar`

### file list

```diff
@@ -1,57 +1,71 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 23:18:25.846105 yohsin3d-0.3.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-04-12 23:18:17.000000 yohsin3d-0.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     6245 2023-04-12 23:18:25.846105 yohsin3d-0.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4860 2023-04-12 23:18:17.000000 yohsin3d-0.3.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-12 23:18:25.846105 yohsin3d-0.3.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1696 2023-04-12 23:18:17.000000 yohsin3d-0.3.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 23:18:25.842105 yohsin3d-0.3.0/yohsin3d/
--rw-r--r--   0 runner    (1001) docker     (123)      113 2023-04-12 23:18:17.000000 yohsin3d-0.3.0/yohsin3d/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 23:18:25.842105 yohsin3d-0.3.0/yohsin3d/communicators/
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-04-12 23:18:17.000000 yohsin3d-0.3.0/yohsin3d/communicators/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 23:18:25.842105 yohsin3d-0.3.0/yohsin3d/communicators/y3d_communicator/
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-04-12 23:18:17.000000 yohsin3d-0.3.0/yohsin3d/communicators/y3d_communicator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2343 2023-04-12 23:18:17.000000 yohsin3d-0.3.0/yohsin3d/communicators/y3d_communicator/bit_codec.py
--rw-r--r--   0 runner    (1001) docker     (123)     3366 2023-04-12 23:18:17.000000 yohsin3d-0.3.0/yohsin3d/communicators/y3d_communicator/communicator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 23:18:25.842105 yohsin3d-0.3.0/yohsin3d/core/
--rw-r--r--   0 runner    (1001) docker     (123)      238 2023-04-12 23:18:17.000000 yohsin3d-0.3.0/yohsin3d/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3266 2023-04-12 23:18:17.000000 yohsin3d-0.3.0/yohsin3d/core/agent.py
--rw-r--r--   0 runner    (1001) docker     (123)     3797 2023-04-12 23:18:17.000000 yohsin3d-0.3.0/yohsin3d/core/behavior.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 23:18:25.842105 yohsin3d-0.3.0/yohsin3d/core/body/
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-04-12 23:18:17.000000 yohsin3d-0.3.0/yohsin3d/core/body/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5237 2023-04-12 23:18:17.000000 yohsin3d-0.3.0/yohsin3d/core/body/body_model.py
--rw-r--r--   0 runner    (1001) docker     (123)      438 2023-04-12 23:18:17.000000 yohsin3d-0.3.0/yohsin3d/core/body/enums.py
--rw-r--r--   0 runner    (1001) docker     (123)      687 2023-04-12 23:18:17.000000 yohsin3d-0.3.0/yohsin3d/core/body/nao_joint.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 23:18:25.846105 yohsin3d-0.3.0/yohsin3d/core/common/
--rw-r--r--   0 runner    (1001) docker     (123)      138 2023-04-12 23:18:17.000000 yohsin3d-0.3.0/yohsin3d/core/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      320 2023-04-12 23:18:17.000000 yohsin3d-0.3.0/yohsin3d/core/common/agent_location.py
--rw-r--r--   0 runner    (1001) docker     (123)      367 2023-04-12 23:18:17.000000 yohsin3d-0.3.0/yohsin3d/core/common/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)      317 2023-04-12 23:18:17.000000 yohsin3d-0.3.0/yohsin3d/core/common/ground_truth_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     3109 2023-04-12 23:18:17.000000 yohsin3d-0.3.0/yohsin3d/core/common/joints.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 23:18:25.846105 yohsin3d-0.3.0/yohsin3d/core/communicator/
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-04-12 23:18:17.000000 yohsin3d-0.3.0/yohsin3d/core/communicator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1632 2023-04-12 23:18:17.000000 yohsin3d-0.3.0/yohsin3d/core/communicator/base_communicator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 23:18:25.846105 yohsin3d-0.3.0/yohsin3d/core/localizer/
--rw-r--r--   0 runner    (1001) docker     (123)      149 2023-04-12 23:18:17.000000 yohsin3d-0.3.0/yohsin3d/core/localizer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      404 2023-04-12 23:18:17.000000 yohsin3d-0.3.0/yohsin3d/core/localizer/base_localizer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 23:18:25.846105 yohsin3d-0.3.0/yohsin3d/core/network/
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-04-12 23:18:17.000000 yohsin3d-0.3.0/yohsin3d/core/network/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-04-12 23:18:17.000000 yohsin3d-0.3.0/yohsin3d/core/network/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)    12096 2023-04-12 23:18:17.000000 yohsin3d-0.3.0/yohsin3d/core/network/parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     1366 2023-04-12 23:18:17.000000 yohsin3d-0.3.0/yohsin3d/core/network/server.py
--rw-r--r--   0 runner    (1001) docker     (123)      677 2023-04-12 23:18:17.000000 yohsin3d-0.3.0/yohsin3d/core/spawner.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 23:18:25.846105 yohsin3d-0.3.0/yohsin3d/core/world/
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-04-12 23:18:17.000000 yohsin3d-0.3.0/yohsin3d/core/world/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1210 2023-04-12 23:18:17.000000 yohsin3d-0.3.0/yohsin3d/core/world/enums.py
--rw-r--r--   0 runner    (1001) docker     (123)     3396 2023-04-12 23:18:17.000000 yohsin3d-0.3.0/yohsin3d/core/world/world_model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 23:18:25.846105 yohsin3d-0.3.0/yohsin3d/localizers/
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-04-12 23:18:17.000000 yohsin3d-0.3.0/yohsin3d/localizers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      523 2023-04-12 23:18:17.000000 yohsin3d-0.3.0/yohsin3d/localizers/ground_truth_localizer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 23:18:25.846105 yohsin3d-0.3.0/yohsin3d/movement/
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-04-12 23:18:17.000000 yohsin3d-0.3.0/yohsin3d/movement/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4448 2023-04-12 23:18:17.000000 yohsin3d-0.3.0/yohsin3d/movement/movement.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-12 23:18:17.000000 yohsin3d-0.3.0/yohsin3d/movement/y3d_movements.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-12 23:18:25.842105 yohsin3d-0.3.0/yohsin3d.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6245 2023-04-12 23:18:25.000000 yohsin3d-0.3.0/yohsin3d.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1342 2023-04-12 23:18:25.000000 yohsin3d-0.3.0/yohsin3d.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-12 23:18:25.000000 yohsin3d-0.3.0/yohsin3d.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-12 23:18:25.000000 yohsin3d-0.3.0/yohsin3d.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 13:15:51.505665 yohsin3d-0.4.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1066 2023-05-05 13:15:36.000000 yohsin3d-0.4.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     6245 2023-05-05 13:15:51.505665 yohsin3d-0.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4860 2023-05-05 13:15:36.000000 yohsin3d-0.4.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-05 13:15:51.505665 yohsin3d-0.4.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1696 2023-05-05 13:15:36.000000 yohsin3d-0.4.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 13:15:51.497666 yohsin3d-0.4.0/yohsin3d/
+-rw-r--r--   0 runner    (1001) docker     (123)      113 2023-05-05 13:15:36.000000 yohsin3d-0.4.0/yohsin3d/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 13:15:51.497666 yohsin3d-0.4.0/yohsin3d/communicators/
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-05-05 13:15:36.000000 yohsin3d-0.4.0/yohsin3d/communicators/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 13:15:51.497666 yohsin3d-0.4.0/yohsin3d/communicators/y3d_communicator/
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-05-05 13:15:36.000000 yohsin3d-0.4.0/yohsin3d/communicators/y3d_communicator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2376 2023-05-05 13:15:36.000000 yohsin3d-0.4.0/yohsin3d/communicators/y3d_communicator/bit_codec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3467 2023-05-05 13:15:36.000000 yohsin3d-0.4.0/yohsin3d/communicators/y3d_communicator/communicator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 13:15:51.501665 yohsin3d-0.4.0/yohsin3d/core/
+-rw-r--r--   0 runner    (1001) docker     (123)      265 2023-05-05 13:15:36.000000 yohsin3d-0.4.0/yohsin3d/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3323 2023-05-05 13:15:36.000000 yohsin3d-0.4.0/yohsin3d/core/agent.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3846 2023-05-05 13:15:36.000000 yohsin3d-0.4.0/yohsin3d/core/behavior.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 13:15:51.501665 yohsin3d-0.4.0/yohsin3d/core/body/
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-05 13:15:36.000000 yohsin3d-0.4.0/yohsin3d/core/body/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5459 2023-05-05 13:15:36.000000 yohsin3d-0.4.0/yohsin3d/core/body/body_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)      438 2023-05-05 13:15:36.000000 yohsin3d-0.4.0/yohsin3d/core/body/enums.py
+-rw-r--r--   0 runner    (1001) docker     (123)      687 2023-05-05 13:15:36.000000 yohsin3d-0.4.0/yohsin3d/core/body/nao_joint.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 13:15:51.501665 yohsin3d-0.4.0/yohsin3d/core/common/
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2023-05-05 13:15:36.000000 yohsin3d-0.4.0/yohsin3d/core/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      442 2023-05-05 13:15:36.000000 yohsin3d-0.4.0/yohsin3d/core/common/agent_location.py
+-rw-r--r--   0 runner    (1001) docker     (123)      367 2023-05-05 13:15:36.000000 yohsin3d-0.4.0/yohsin3d/core/common/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)      329 2023-05-05 13:15:36.000000 yohsin3d-0.4.0/yohsin3d/core/common/ground_truth_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3109 2023-05-05 13:15:36.000000 yohsin3d-0.4.0/yohsin3d/core/common/joints.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 13:15:51.501665 yohsin3d-0.4.0/yohsin3d/core/communicator/
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-05-05 13:15:36.000000 yohsin3d-0.4.0/yohsin3d/core/communicator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1651 2023-05-05 13:15:36.000000 yohsin3d-0.4.0/yohsin3d/core/communicator/base_communicator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 13:15:51.501665 yohsin3d-0.4.0/yohsin3d/core/localizer/
+-rw-r--r--   0 runner    (1001) docker     (123)      149 2023-05-05 13:15:36.000000 yohsin3d-0.4.0/yohsin3d/core/localizer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      406 2023-05-05 13:15:36.000000 yohsin3d-0.4.0/yohsin3d/core/localizer/base_localizer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 13:15:51.501665 yohsin3d-0.4.0/yohsin3d/core/network/
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-05-05 13:15:36.000000 yohsin3d-0.4.0/yohsin3d/core/network/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-05 13:15:36.000000 yohsin3d-0.4.0/yohsin3d/core/network/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12190 2023-05-05 13:15:36.000000 yohsin3d-0.4.0/yohsin3d/core/network/parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1366 2023-05-05 13:15:36.000000 yohsin3d-0.4.0/yohsin3d/core/network/server.py
+-rw-r--r--   0 runner    (1001) docker     (123)      677 2023-05-05 13:15:36.000000 yohsin3d-0.4.0/yohsin3d/core/spawner.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 13:15:51.501665 yohsin3d-0.4.0/yohsin3d/core/world/
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-05-05 13:15:36.000000 yohsin3d-0.4.0/yohsin3d/core/world/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1602 2023-05-05 13:15:36.000000 yohsin3d-0.4.0/yohsin3d/core/world/enums.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3477 2023-05-05 13:15:36.000000 yohsin3d-0.4.0/yohsin3d/core/world/world_model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 13:15:51.501665 yohsin3d-0.4.0/yohsin3d/drawing/
+-rw-r--r--   0 runner    (1001) docker     (123)       35 2023-05-05 13:15:36.000000 yohsin3d-0.4.0/yohsin3d/drawing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5627 2023-05-05 13:15:36.000000 yohsin3d-0.4.0/yohsin3d/drawing/rv_draw.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 13:15:51.505665 yohsin3d-0.4.0/yohsin3d/localizers/
+-rw-r--r--   0 runner    (1001) docker     (123)      109 2023-05-05 13:15:36.000000 yohsin3d-0.4.0/yohsin3d/localizers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4607 2023-05-05 13:15:36.000000 yohsin3d-0.4.0/yohsin3d/localizers/geometric_localizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      527 2023-05-05 13:15:36.000000 yohsin3d-0.4.0/yohsin3d/localizers/ground_truth_localizer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 13:15:51.505665 yohsin3d-0.4.0/yohsin3d/locomotors/
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-05-05 13:15:36.000000 yohsin3d-0.4.0/yohsin3d/locomotors/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 13:15:51.505665 yohsin3d-0.4.0/yohsin3d/locomotors/getup/
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-05-05 13:15:36.000000 yohsin3d-0.4.0/yohsin3d/locomotors/getup/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36762 2023-05-05 13:15:36.000000 yohsin3d-0.4.0/yohsin3d/locomotors/getup/fall_recovery.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 13:15:51.505665 yohsin3d-0.4.0/yohsin3d/locomotors/pfs/
+-rw-r--r--   0 runner    (1001) docker     (123)      352 2023-05-05 13:15:36.000000 yohsin3d-0.4.0/yohsin3d/locomotors/pfs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5297 2023-05-05 13:15:36.000000 yohsin3d-0.4.0/yohsin3d/locomotors/pfs/pfs_turn.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10854 2023-05-05 13:15:36.000000 yohsin3d-0.4.0/yohsin3d/locomotors/pfs/pfs_walk.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2105 2023-05-05 13:15:36.000000 yohsin3d-0.4.0/yohsin3d/locomotors/pfs/utility.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 13:15:51.505665 yohsin3d-0.4.0/yohsin3d/movement/
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-05-05 13:15:36.000000 yohsin3d-0.4.0/yohsin3d/movement/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4574 2023-05-05 13:15:36.000000 yohsin3d-0.4.0/yohsin3d/movement/movement.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 13:15:36.000000 yohsin3d-0.4.0/yohsin3d/movement/y3d_movements.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 13:15:51.497666 yohsin3d-0.4.0/yohsin3d.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6245 2023-05-05 13:15:51.000000 yohsin3d-0.4.0/yohsin3d.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1698 2023-05-05 13:15:51.000000 yohsin3d-0.4.0/yohsin3d.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 13:15:51.000000 yohsin3d-0.4.0/yohsin3d.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-05 13:15:51.000000 yohsin3d-0.4.0/yohsin3d.egg-info/top_level.txt
```

### Comparing `yohsin3d-0.3.0/LICENSE` & `yohsin3d-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `yohsin3d-0.3.0/PKG-INFO` & `yohsin3d-0.4.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yohsin3d
-Version: 0.3.0
+Version: 0.4.0
 Summary: Program your own RoboCup 3D soccer playing agents in python
 Home-page: https://github.com/FC-Yohsin/yohsin3d
 Author: Habib Shahzad, Abuzar Rasool, Faaz Abidi
 Author-email: habibshehzad55@gmail.com, availabuzar@gmail.com, hasanfaaz10@gmail.com
 License: MIT
 Keywords: robocup,soccer,3d,simulation,agents,robotics,machine learning,python,artificial intelligence,locomotion,localization
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `yohsin3d-0.3.0/README.md` & `yohsin3d-0.4.0/README.md`

 * *Files identical despite different names*

### Comparing `yohsin3d-0.3.0/setup.py` & `yohsin3d-0.4.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from pathlib import Path
 
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(
     name='yohsin3d',
-    version='0.3.0',
+    version='0.4.0',
     description='Program your own RoboCup 3D soccer playing agents in python',
     long_description=long_description,
     long_description_content_type='text/markdown',
     author='Habib Shahzad, Abuzar Rasool, Faaz Abidi',
     author_email='habibshehzad55@gmail.com, availabuzar@gmail.com, hasanfaaz10@gmail.com',
     url='https://github.com/FC-Yohsin/yohsin3d',
     license="MIT",
```

### Comparing `yohsin3d-0.3.0/yohsin3d/communicators/y3d_communicator/bit_codec.py` & `yohsin3d-0.4.0/yohsin3d/communicators/y3d_communicator/bit_codec.py`

 * *Files 17% similar despite different names*

```diff
@@ -6,27 +6,27 @@
 
     @staticmethod
     def bits_to_int(bits: List, start, end):
         if start < 0 or end >= len(bits):
             return 0
 
         n = 0
-        for i in range(start, end+1):
+        for i in range(start, end + 1):
             n *= 2
             n += bits[i]
 
         return n
 
     @staticmethod
     def int_to_bits(n: int, num_bits: int) -> List[int]:
         if n < 0:
             return []
 
         bits = [0] * num_bits
-        for i in range(num_bits-1, -1, -1):
+        for i in range(num_bits - 1, -1, -1):
             bits[i] = n % 2
             n //= 2
 
         return bits
 
     @staticmethod
     def bits_to_string(bitfield_list):
@@ -74,8 +74,9 @@
         value = int(((clipped - min_value) * max_size) /
                     (max_value - min_value) + 0.5)
         return BitCodec.int_to_bits(value, num_bits)
 
     @staticmethod
     def decode_bit_array(bits, min_value, max_value, num_bits=10):
         value = BitCodec.bits_to_int(bits, 0, num_bits - 1)
-        return min_value + (value * (max_value - min_value)) / ((1 << num_bits) - 1)
+        return min_value + (value * (max_value - min_value)
+                            ) / ((1 << num_bits) - 1)
```

### Comparing `yohsin3d-0.3.0/yohsin3d/communicators/y3d_communicator/communicator.py` & `yohsin3d-0.4.0/yohsin3d/communicators/y3d_communicator/communicator.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,21 @@
 from ...core.common.constants import *
 from ...core import BaseCommunicator
 from .bit_codec import BitCodec
 
 
 class CommunicationData:
-    def __init__(self, heard_from=None, time=None, ball_x=None, ball_y=None, my_x=None, my_y=None):
+    def __init__(
+            self,
+            heard_from=None,
+            time=None,
+            ball_x=None,
+            ball_y=None,
+            my_x=None,
+            my_y=None):
         self.heard_from = heard_from
         self.time = time
         self.ball_x = ball_x
         self.ball_y = ball_y
         self.my_x = my_x
         self.my_y = my_y
 
@@ -60,27 +67,27 @@
 
         ctr = 0
 
         cycles = BitCodec.bits_to_int(bits, ctr, ctr + 15)
         time = cycles * 0.02
         ctr += 16
 
-        bx_bits = bits[ctr:ctr+10]
+        bx_bits = bits[ctr:ctr + 10]
         ballX = BitCodec.decode_bit_array(bx_bits, min_ball_x, max_ball_x)
         ctr += 10
 
-        by_bits = bits[ctr:ctr+10]
+        by_bits = bits[ctr:ctr + 10]
         ballY = BitCodec.decode_bit_array(by_bits, min_ball_y, max_ball_y)
         ctr += 10
 
-        ax_bits = bits[ctr:ctr+10]
+        ax_bits = bits[ctr:ctr + 10]
         agentX = BitCodec.decode_bit_array(ax_bits, min_agent_x, max_agent_x)
         ctr += 10
 
-        ay_bits = bits[ctr:ctr+10]
+        ay_bits = bits[ctr:ctr + 10]
         agentY = BitCodec.decode_bit_array(ay_bits, min_agent_y, max_agent_y)
         ctr += 10
 
         return time, ballX, ballY, agentX, agentY
 
     def hear(self) -> None:
         heard_message = self.heard_message
@@ -93,12 +100,12 @@
         bits = BitCodec.string_to_bits(message)
         time, ballX, ballY, agentX, agentY = self.bits_to_data(bits)
 
         heard_time = heard_message.heard_time
         delta_game_time = self.world_model.get_time() - self.world_model.get_gametime()
         heard_server_time = heard_time + delta_game_time
 
-        time += int((heard_server_time-time)/1310.72)*1310.72
+        time += int((heard_server_time - time) / 1310.72) * 1310.72
         cycles = int(time * 50 + 0.1)
-        unum = (cycles % (NUM_AGENTS*2)) // 2 + 1
+        unum = (cycles % (NUM_AGENTS * 2)) // 2 + 1
         self.heard_data = CommunicationData(
             unum, time, ballX, ballY, agentX, agentY)
```

### Comparing `yohsin3d-0.3.0/yohsin3d/core/agent.py` & `yohsin3d-0.4.0/yohsin3d/core/agent.py`

 * *Files 3% similar despite different names*

```diff
@@ -31,14 +31,15 @@
         self.global_port = global_port
         self.monitor_port = monitor_port
 
         self.global_socket = Server()
         self.monitor_socket = Server()
         self.behavior: BaseBehavior = behavior
         self.behavior.initialize(team_name)
+        self.behavior.body_model.agent_type = agent_type
 
     def done(self):
         self.global_socket.close()
         if self.monitor_port != -1:
             self.monitor_socket.close()
 
     def setup_message(self):
```

### Comparing `yohsin3d-0.3.0/yohsin3d/core/behavior.py` & `yohsin3d-0.4.0/yohsin3d/core/behavior.py`

 * *Files 4% similar despite different names*

```diff
@@ -4,15 +4,19 @@
 from .network import Parser
 from .communicator import BaseCommunicator
 from .common import AgentLocation, Joint
 
 
 class BaseBehavior:
 
-    def __init__(self, beam_location: AgentLocation, localizer: BaseLocalizer = None, communicator: BaseCommunicator = None) -> None:
+    def __init__(
+            self,
+            beam_location: AgentLocation,
+            localizer: BaseLocalizer = None,
+            communicator: BaseCommunicator = None) -> None:
         self.beam_location = beam_location
         self.monitor_msg = ""
         self.initialized = False
         self.init_beamed = False
         self.localizer: BaseLocalizer = localizer
         self.communicator: BaseCommunicator = communicator
```

### Comparing `yohsin3d-0.3.0/yohsin3d/core/body/body_model.py` & `yohsin3d-0.4.0/yohsin3d/core/body/body_model.py`

 * *Files 8% similar despite different names*

```diff
@@ -10,83 +10,89 @@
 
 class BodyModel:
     def __init__(self, worldModel: WorldModel) -> None:
         self.gyro_rates = (0, 0, 0)
         self.prev_gyro_rates = (0, 0, 0)
         self.accel_rates = (0, 0, 0)
         self.walk_angle = None
+        self.agent_type = None
 
         self.world_model = worldModel
         self.joints_list: List[NaoJoint] = [
             None for _ in range(len(Joint))
         ]
 
         self.previous_joints_list: list[NaoJoint] = [
             None for _ in range(len(Joint))
         ]
 
         self.initialise_joints()
 
     def set_initial_head(self):
 
-        self.set_target_angle(Joint.H1, 0)
-        self.set_target_angle(Joint.H2, -45)
+        gain = 7.0
+        self.set_target_angle(Joint.H1, 0, gain)
+        self.set_target_angle(Joint.H2, -45, gain)
 
     def target_reached(self, joint: Joint):
         return abs(self.joints_list[joint].current_angle -
                    self.joints_list[joint].target_angle
                    ) < self.joints_list[joint].error_tolerance
 
     def set_initial_arm(self, arm) -> bool:
 
         ang1 = -50.0
         ang2 = 30.0
         ang3 = 0
         ang4 = -50.0
 
+        gain = 7.0
+
         if (arm == BodyParts.ARM_LEFT):
 
-            self.set_target_angle(Joint.LA1, ang1)
-            self.set_target_angle(Joint.LA2, ang2)
-            self.set_target_angle(Joint.LA3, ang3)
-            self.set_target_angle(Joint.LA4, ang4)
+            self.set_target_angle(Joint.LA1, ang1, gain)
+            self.set_target_angle(Joint.LA2, ang2, gain)
+            self.set_target_angle(Joint.LA3, ang3, gain)
+            self.set_target_angle(Joint.LA4, ang4, gain)
 
         else:
 
-            self.set_target_angle(Joint.RA1, ang1)
-            self.set_target_angle(Joint.RA2, -ang2)
-            self.set_target_angle(Joint.RA3, -ang3)
-            self.set_target_angle(Joint.RA4, -ang4)
+            self.set_target_angle(Joint.RA1, ang1, gain)
+            self.set_target_angle(Joint.RA2, -ang2, gain)
+            self.set_target_angle(Joint.RA3, -ang3, gain)
+            self.set_target_angle(Joint.RA4, -ang4, gain)
 
     def set_initial_leg(self, leg) -> bool:
 
         ang1 = 0
         ang2 = 6.0
         ang3 = 18.0
         ang4 = -30.0
         ang5 = 18.0
         ang6 = -6.0
 
+        gain = 7.0
+
         if (leg == BodyParts.LEG_LEFT):
 
-            self.set_target_angle(Joint.LL1, ang1)
-            self.set_target_angle(Joint.LL2, ang2)
-            self.set_target_angle(Joint.LL3, ang3)
-            self.set_target_angle(Joint.LL4, ang4)
-            self.set_target_angle(Joint.LL5, ang5)
-            self.set_target_angle(Joint.LL6, ang6)
+            self.set_target_angle(Joint.LL1, ang1, gain)
+            self.set_target_angle(Joint.LL2, ang2, gain)
+            self.set_target_angle(Joint.LL3, ang3, gain)
+            self.set_target_angle(Joint.LL4, ang4, gain)
+            self.set_target_angle(Joint.LL5, ang5, gain)
+            self.set_target_angle(Joint.LL6, ang6, gain)
 
         else:
 
-            self.set_target_angle(Joint.RL1, ang1)
-            self.set_target_angle(Joint.RL2, -ang2)
-            self.set_target_angle(Joint.RL3, ang3)
-            self.set_target_angle(Joint.RL4, ang4)
-            self.set_target_angle(Joint.RL5, ang5)
-            self.set_target_angle(Joint.RL6, -ang6)
+            self.set_target_angle(Joint.RL1, ang1, gain)
+            self.set_target_angle(Joint.RL2, -ang2, gain)
+            self.set_target_angle(Joint.RL3, ang3, gain)
+            self.set_target_angle(Joint.RL4, ang4, gain)
+            self.set_target_angle(Joint.RL5, ang5, gain)
+            self.set_target_angle(Joint.RL6, -ang6, gain)
 
     def set_current_angle(self, joint: Joint, angle):
         self.previous_joints_list[joint] = self.joints_list[
             joint].current_angle
         self.joints_list[joint].current_angle = angle
 
     def gettarget_angle(self, joint: Joint):
```

### Comparing `yohsin3d-0.3.0/yohsin3d/core/body/nao_joint.py` & `yohsin3d-0.4.0/yohsin3d/core/body/nao_joint.py`

 * *Files identical despite different names*

### Comparing `yohsin3d-0.3.0/yohsin3d/core/common/joints.py` & `yohsin3d-0.4.0/yohsin3d/core/common/joints.py`

 * *Files identical despite different names*

### Comparing `yohsin3d-0.3.0/yohsin3d/core/communicator/base_communicator.py` & `yohsin3d-0.4.0/yohsin3d/core/communicator/base_communicator.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,15 +21,16 @@
 
     def __init__(self) -> None:
         self.said_message: str = ""
         self.heard_message: HeardMessage = HeardMessage()
         self.world_model: WorldModel = None
         self.localizer: BaseLocalizer = None
 
-    def initialize(self, world_model: WorldModel, localizer: BaseLocalizer) -> None:
+    def initialize(self, world_model: WorldModel,
+                   localizer: BaseLocalizer) -> None:
         self.world_model = world_model
         self.localizer = localizer
 
     def can_say(self):
 
         if not self.world_model.is_my_number_set():
             return False
```

### Comparing `yohsin3d-0.3.0/yohsin3d/core/network/parser.py` & `yohsin3d-0.4.0/yohsin3d/core/network/parser.py`

 * *Files 2% similar despite different names*

```diff
@@ -73,15 +73,16 @@
     def __get_xyz(self, string, start):
         x, y, z = self.__parser_helper(start, string).split()
         return float(x), float(y), float(z)
 
     def __parse_accelerometer(self, string):
         rateX, rateY, rateZ = self.__get_xyz(string, "a")
 
-        #  Sometimes spurious (very high or NaN) readings come through. Clip them.
+        # Sometimes spurious (very high or NaN) readings come through. Clip
+        # them.
         spuriousThreshold = 20.0
         if ((abs(rateX) > spuriousThreshold)):
             rateX = 0
 
         if ((abs(rateY) > spuriousThreshold)):
             rateY = 0
 
@@ -100,15 +101,17 @@
         correctedRateY = K * lastAccel[1] + (1 - K) * correctedRateY
         correctedRateZ = K * lastAccel[2] + (1 - K) * correctedRateZ
 
         self.body_model.set_accel_rates(
             (correctedRateX, correctedRateY, correctedRateZ))
 
     def __segment(self, string):
-        return re.findall(r'\(([^()]*(?:\(([^()]*(?:\((?:[^()]*(?:\([^()]*\)[^()]*)*)\)[^()]*)*)\)[^()]*)*)\)', string)
+        return re.findall(
+            r'\(([^()]*(?:\(([^()]*(?:\((?:[^()]*(?:\([^()]*\)[^()]*)*)\)[^()]*)*)\)[^()]*)*)\)',
+            string)
 
     def __parse_hinge_joint(self, string):
         effector_name = perceptor_to_joint[self.__parser_helper("n", string)]
         effector_angle = float(self.__parser_helper("ax", string))
 
         self.body_model.set_current_angle(effector_name, effector_angle)
         return True
@@ -130,16 +133,16 @@
         x, y, z = self.__get_xyz(string, "pol")
         name = VisibleObjects(name)
         self.world_model.simple_vision_objects[name] = (x, y, z)
         return True
 
     def __parse_line(self, string):
         '''
-        Parse Line is not complete yet. There are multiple lines data coming from the server. We need to figure out how to 
-        process that. 
+        Parse Line is not complete yet. There are multiple lines data coming from the server. We need to figure out how to
+        process that.
 
         TODO: Need to undderstand the concept of the lines
         '''
         tokens = self.tokenise(string)
 
         r = float(tokens[2])
         theta = float(tokens[3])
@@ -153,15 +156,16 @@
         return True
 
     def __parse_player(self, string):
 
         valid = False
 
         tokens = self.tokenise(string)
-        # based on the assumption that the max characters in a team name will be 100
+        # based on the assumption that the max characters in a team name will
+        # be 100
         valid = (len(tokens) == 30)
 
         if valid:
             agent_num = (tokens[4]).zfill(2)
             team_name = tokens[2]
 
             agent_num = int(agent_num)
@@ -183,28 +187,30 @@
                 self.world_model.opponent_info[agent_num].update_from_dict(
                     player_info)
 
         return valid
 
     def __reset_simple_non_visible_objects(self, string):
         for object in VisibleObjects:
-            if not re.search(f"[(]{object.value}\s", string):
+            if not re.search(f"[(]{object.value}\\s", string):
                 self.world_model.simple_vision_objects[object] = None
 
     def __is_player_visible(self, string, num, team):
-        regex = f"\(P\s+\(team\s+{team}\)\s+\(id\s+{num}\)"
+        regex = f"\\(P\\s+\\(team\\s+{team}\\)\\s+\\(id\\s+{num}\\)"
         return re.search(regex, string) is not None
 
     def __reset_player_information(self, string):
         for object in self.world_model.teammate_info.keys():
-            if not self.__is_player_visible(string, object, self.world_model.my_team_name):
+            if not self.__is_player_visible(
+                    string, object, self.world_model.my_team_name):
                 self.world_model.teammate_info[object].is_visible = False
 
         for object in self.world_model.opponent_info.keys():
-            if not self.__is_player_visible(string, object, self.world_model.opponent_team_name):
+            if not self.__is_player_visible(
+                    string, object, self.world_model.opponent_team_name):
                 self.world_model.opponent_info[object].is_visible = False
 
     def __parse_position_groundtruth(self, string):
         tokens = self.tokenise(string)
         self.world_model.set_position_groundtruth(
             (float(tokens[1]), float(tokens[2]), float(tokens[3])))
```

### Comparing `yohsin3d-0.3.0/yohsin3d/core/network/server.py` & `yohsin3d-0.4.0/yohsin3d/core/network/server.py`

 * *Files identical despite different names*

### Comparing `yohsin3d-0.3.0/yohsin3d/core/spawner.py` & `yohsin3d-0.4.0/yohsin3d/core/spawner.py`

 * *Files identical despite different names*

### Comparing `yohsin3d-0.3.0/yohsin3d/core/world/world_model.py` & `yohsin3d-0.4.0/yohsin3d/core/world/world_model.py`

 * *Files 9% similar despite different names*

```diff
@@ -89,15 +89,15 @@
     def get_my_number(self):
         return self.my_number
 
     def set_my_number(self, num):
         self.my_number = num
 
     def is_my_number_set(self):
-        return self.my_number != None
+        return self.my_number is not None
 
     def set_position_groundtruth(self, new_pos):
         self.groundtruth.my_location.update_position(new_pos)
 
     def set_orientation_groundtruth(self, new_orientation):
         self.groundtruth.my_location.update_orientation(new_orientation)
 
@@ -107,19 +107,25 @@
     def get_side(self):
         return self.side
 
     def set_side(self, side):
         self.side = side
 
     def is_side_set(self):
-        return self.side != None
+        return self.side is not None
 
 
 class PlayerInfo:
-    def __init__(self, head=None, rlowerarm=None, llowerarm=None, rfoot=None, lfoot=None):
+    def __init__(
+            self,
+            head=None,
+            rlowerarm=None,
+            llowerarm=None,
+            rfoot=None,
+            lfoot=None):
         self.head = head
         self.rlowerarm = rlowerarm
         self.llowerarm = llowerarm
         self.rfoot = rfoot
         self.lfoot = lfoot
 
         self.is_visible = False
```

### Comparing `yohsin3d-0.3.0/yohsin3d/localizers/ground_truth_localizer.py` & `yohsin3d-0.4.0/yohsin3d/localizers/ground_truth_localizer.py`

 * *Files 24% similar despite different names*

```diff
@@ -2,16 +2,16 @@
 from ..core import BaseLocalizer
 
 
 GROUNDTRUTH_NOT_ENABLED_ERROR = "Ground truth not enabled"
 
 
 class GroundTruthLocalizer(BaseLocalizer):
-    def _init_(self) -> None:
-        super()._init_()
+    def __init__(self) -> None:
+        super().__init__()
 
     def check_validity(self) -> None:
         assert self.world_model.groundtruth.is_enabled(), GROUNDTRUTH_NOT_ENABLED_ERROR
 
     def update(self) -> None:
         self.check_validity()
         self.my_location = self.world_model.groundtruth.my_location
```

### Comparing `yohsin3d-0.3.0/yohsin3d/movement/movement.py` & `yohsin3d-0.4.0/yohsin3d/movement/movement.py`

 * *Files 1% similar despite different names*

```diff
@@ -46,19 +46,16 @@
 class Movement:
     def __init__(self, name="None") -> None:
         self.name = name
         self.phases: List[MovementPhase] = []
         self.current_index = 0
 
     @staticmethod
-    def from_file(path):
-
-        file = open(path, 'r')
+    def from_string(content: str):
         movement = Movement()
-        content = file.read()
         phases: list = list(re.findall(
             r"start phase((.|\n)*?)end phase", content))
 
         for phase in phases:
             phase_details: str = phase[0]
             lines = phase_details.splitlines()
             first_line = lines[0].strip()
@@ -77,14 +74,21 @@
                     speed = float(line[3])
                     movement_phase.add(joint, angle, speed)
                 else:
                     raise Exception("Invalid file")
 
             movement.add(movement_phase)
 
+        return movement
+
+    @staticmethod
+    def from_file(path):
+        file = open(path, 'r')
+        content = file.read()
+        movement = Movement.from_string(content)
         file.close()
         return movement
 
     def is_finished(self):
         finished = self.current_index >= len(self.phases)
         return finished
```

### Comparing `yohsin3d-0.3.0/yohsin3d.egg-info/PKG-INFO` & `yohsin3d-0.4.0/yohsin3d.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yohsin3d
-Version: 0.3.0
+Version: 0.4.0
 Summary: Program your own RoboCup 3D soccer playing agents in python
 Home-page: https://github.com/FC-Yohsin/yohsin3d
 Author: Habib Shahzad, Abuzar Rasool, Faaz Abidi
 Author-email: habibshehzad55@gmail.com, availabuzar@gmail.com, hasanfaaz10@gmail.com
 License: MIT
 Keywords: robocup,soccer,3d,simulation,agents,robotics,machine learning,python,artificial intelligence,locomotion,localization
 Classifier: Development Status :: 3 - Alpha
```

