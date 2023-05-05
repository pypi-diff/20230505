# Comparing `tmp/fluxoperator-0.0.21.tar.gz` & `tmp/fluxoperator-0.0.22.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fluxoperator-0.0.21.tar", last modified: Wed May  3 06:51:17 2023, max compression
+gzip compressed data, was "fluxoperator-0.0.22.tar", last modified: Fri May  5 19:00:14 2023, max compression
```

## Comparing `fluxoperator-0.0.21.tar` & `fluxoperator-0.0.22.tar`

### file list

```diff
@@ -1,67 +1,69 @@
-drwxrwxr-x   0 vanessa   (1000) vanessa   (1000)        0 2023-05-03 06:51:17.432146 fluxoperator-0.0.21/
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     2667 2023-05-03 06:51:17.432146 fluxoperator-0.0.21/PKG-INFO
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)      391 2023-05-02 07:00:33.000000 fluxoperator-0.0.21/README.md
-drwxrwxr-x   0 vanessa   (1000) vanessa   (1000)        0 2023-05-03 06:51:17.420147 fluxoperator-0.0.21/fluxoperator/
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1906 2023-05-02 07:00:33.000000 fluxoperator-0.0.21/fluxoperator/__init__.py
-drwxrwxr-x   0 vanessa   (1000) vanessa   (1000)        0 2023-05-03 06:51:17.420147 fluxoperator-0.0.21/fluxoperator/api/
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)       87 2023-05-02 07:00:33.000000 fluxoperator-0.0.21/fluxoperator/api/__init__.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)    27361 2023-05-02 07:00:33.000000 fluxoperator-0.0.21/fluxoperator/api_client.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)    13137 2023-05-02 21:28:30.000000 fluxoperator-0.0.21/fluxoperator/client.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)    16066 2023-05-02 07:00:33.000000 fluxoperator-0.0.21/fluxoperator/configuration.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)      756 2023-04-07 19:58:49.000000 fluxoperator-0.0.21/fluxoperator/decorator.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)       75 2023-04-07 19:58:49.000000 fluxoperator-0.0.21/fluxoperator/defaults.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     5061 2023-05-02 07:00:33.000000 fluxoperator-0.0.21/fluxoperator/exceptions.py
-drwxrwxr-x   0 vanessa   (1000) vanessa   (1000)        0 2023-05-03 06:51:17.428146 fluxoperator-0.0.21/fluxoperator/models/
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1430 2023-05-02 07:00:33.000000 fluxoperator-0.0.21/fluxoperator/models/__init__.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     8452 2023-05-02 07:00:32.000000 fluxoperator-0.0.21/fluxoperator/models/commands.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     4338 2023-05-02 07:00:32.000000 fluxoperator-0.0.21/fluxoperator/models/container_resources.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     4322 2023-05-02 07:00:33.000000 fluxoperator-0.0.21/fluxoperator/models/container_volume.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     6774 2023-05-02 07:00:33.000000 fluxoperator-0.0.21/fluxoperator/models/flux_restful.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     4119 2023-05-02 07:00:33.000000 fluxoperator-0.0.21/fluxoperator/models/flux_user.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     4402 2023-05-02 07:00:33.000000 fluxoperator-0.0.21/fluxoperator/models/life_cycle.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     6622 2023-05-02 21:28:30.000000 fluxoperator-0.0.21/fluxoperator/models/logging_spec.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     7375 2023-05-02 07:00:33.000000 fluxoperator-0.0.21/fluxoperator/models/mini_cluster.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     3612 2023-05-02 07:00:33.000000 fluxoperator-0.0.21/fluxoperator/models/mini_cluster_archive.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)    25818 2023-05-02 07:00:33.000000 fluxoperator-0.0.21/fluxoperator/models/mini_cluster_container.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     5483 2023-05-02 07:00:33.000000 fluxoperator-0.0.21/fluxoperator/models/mini_cluster_existing_volume.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     6969 2023-05-02 07:00:33.000000 fluxoperator-0.0.21/fluxoperator/models/mini_cluster_list.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)    14746 2023-05-02 07:00:33.000000 fluxoperator-0.0.21/fluxoperator/models/mini_cluster_spec.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     4844 2023-05-02 07:00:33.000000 fluxoperator-0.0.21/fluxoperator/models/mini_cluster_status.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     4434 2023-05-02 07:00:33.000000 fluxoperator-0.0.21/fluxoperator/models/mini_cluster_user.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)    13029 2023-05-02 07:00:33.000000 fluxoperator-0.0.21/fluxoperator/models/mini_cluster_volume.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     7124 2023-05-02 07:00:33.000000 fluxoperator-0.0.21/fluxoperator/models/pod_spec.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     3683 2023-05-02 07:00:33.000000 fluxoperator-0.0.21/fluxoperator/models/security_context.py
-drwxrwxr-x   0 vanessa   (1000) vanessa   (1000)        0 2023-05-03 06:51:17.428146 fluxoperator-0.0.21/fluxoperator/resource/
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)        0 2023-04-07 19:58:49.000000 fluxoperator-0.0.21/fluxoperator/resource/__init__.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1910 2023-04-07 19:58:49.000000 fluxoperator-0.0.21/fluxoperator/resource/network.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     5653 2023-05-02 21:28:30.000000 fluxoperator-0.0.21/fluxoperator/resource/pods.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)    12590 2023-05-02 07:00:33.000000 fluxoperator-0.0.21/fluxoperator/rest.py
-drwxrwxr-x   0 vanessa   (1000) vanessa   (1000)        0 2023-05-03 06:51:17.420147 fluxoperator-0.0.21/fluxoperator.egg-info/
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     2667 2023-05-03 06:51:16.000000 fluxoperator-0.0.21/fluxoperator.egg-info/PKG-INFO
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1867 2023-05-03 06:51:17.000000 fluxoperator-0.0.21/fluxoperator.egg-info/SOURCES.txt
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)        1 2023-05-03 06:51:16.000000 fluxoperator-0.0.21/fluxoperator.egg-info/dependency_links.txt
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)        1 2023-02-25 05:06:19.000000 fluxoperator-0.0.21/fluxoperator.egg-info/not-zip-safe
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)       20 2023-05-03 06:51:17.000000 fluxoperator-0.0.21/fluxoperator.egg-info/requires.txt
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)       18 2023-05-03 06:51:17.000000 fluxoperator-0.0.21/fluxoperator.egg-info/top_level.txt
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)       69 2023-05-03 06:51:17.432146 fluxoperator-0.0.21/setup.cfg
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     2153 2023-05-02 21:28:22.000000 fluxoperator-0.0.21/setup.py
-drwxrwxr-x   0 vanessa   (1000) vanessa   (1000)        0 2023-05-03 06:51:17.432146 fluxoperator-0.0.21/test/
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)        0 2023-05-02 07:00:33.000000 fluxoperator-0.0.21/test/__init__.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1224 2023-04-07 19:58:49.000000 fluxoperator-0.0.21/test/test_commands.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1351 2023-04-07 19:58:49.000000 fluxoperator-0.0.21/test/test_container_resources.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1335 2023-04-07 19:58:49.000000 fluxoperator-0.0.21/test/test_container_volume.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1271 2023-04-07 19:58:49.000000 fluxoperator-0.0.21/test/test_flux_restful.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1212 2023-04-07 19:58:49.000000 fluxoperator-0.0.21/test/test_flux_user.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1226 2023-04-07 19:58:49.000000 fluxoperator-0.0.21/test/test_life_cycle.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1277 2023-04-07 19:58:49.000000 fluxoperator-0.0.21/test/test_logging_spec.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     4925 2023-04-07 19:58:49.000000 fluxoperator-0.0.21/test/test_mini_cluster.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1316 2023-04-07 19:58:49.000000 fluxoperator-0.0.21/test/test_mini_cluster_archive.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     2676 2023-04-07 19:58:49.000000 fluxoperator-0.0.21/test/test_mini_cluster_container.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1504 2023-04-07 19:58:49.000000 fluxoperator-0.0.21/test/test_mini_cluster_existing_volume.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)    10360 2023-04-07 19:58:49.000000 fluxoperator-0.0.21/test/test_mini_cluster_list.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     6188 2023-04-07 19:58:49.000000 fluxoperator-0.0.21/test/test_mini_cluster_spec.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1364 2023-04-07 19:58:49.000000 fluxoperator-0.0.21/test/test_mini_cluster_status.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1334 2023-04-07 19:58:49.000000 fluxoperator-0.0.21/test/test_mini_cluster_user.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1578 2023-04-07 19:58:49.000000 fluxoperator-0.0.21/test/test_mini_cluster_volume.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1284 2023-04-07 19:58:49.000000 fluxoperator-0.0.21/test/test_pod_spec.py
--rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1289 2023-04-07 19:58:49.000000 fluxoperator-0.0.21/test/test_security_context.py
+drwxrwxr-x   0 vanessa   (1000) vanessa   (1000)        0 2023-05-05 19:00:14.632271 fluxoperator-0.0.22/
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     2694 2023-05-05 19:00:14.632271 fluxoperator-0.0.22/PKG-INFO
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)      391 2023-05-04 17:45:25.000000 fluxoperator-0.0.22/README.md
+drwxrwxr-x   0 vanessa   (1000) vanessa   (1000)        0 2023-05-05 19:00:14.624271 fluxoperator-0.0.22/fluxoperator/
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1957 2023-05-05 02:07:25.000000 fluxoperator-0.0.22/fluxoperator/__init__.py
+drwxrwxr-x   0 vanessa   (1000) vanessa   (1000)        0 2023-05-05 19:00:14.624271 fluxoperator-0.0.22/fluxoperator/api/
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)       87 2023-05-04 17:45:25.000000 fluxoperator-0.0.22/fluxoperator/api/__init__.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)    27361 2023-05-04 17:45:25.000000 fluxoperator-0.0.22/fluxoperator/api_client.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)    13137 2023-05-02 21:28:30.000000 fluxoperator-0.0.22/fluxoperator/client.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)    16066 2023-05-04 17:45:25.000000 fluxoperator-0.0.22/fluxoperator/configuration.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)      756 2023-04-07 19:58:49.000000 fluxoperator-0.0.22/fluxoperator/decorator.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)       75 2023-04-07 19:58:49.000000 fluxoperator-0.0.22/fluxoperator/defaults.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     5061 2023-05-04 17:45:25.000000 fluxoperator-0.0.22/fluxoperator/exceptions.py
+drwxrwxr-x   0 vanessa   (1000) vanessa   (1000)        0 2023-05-05 19:00:14.628271 fluxoperator-0.0.22/fluxoperator/models/
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1481 2023-05-05 02:07:25.000000 fluxoperator-0.0.22/fluxoperator/models/__init__.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     8452 2023-05-04 17:45:25.000000 fluxoperator-0.0.22/fluxoperator/models/commands.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     4338 2023-05-04 17:45:25.000000 fluxoperator-0.0.22/fluxoperator/models/container_resources.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     4322 2023-05-04 17:45:25.000000 fluxoperator-0.0.22/fluxoperator/models/container_volume.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     6774 2023-05-04 17:45:25.000000 fluxoperator-0.0.22/fluxoperator/models/flux_restful.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     5816 2023-05-05 02:07:25.000000 fluxoperator-0.0.22/fluxoperator/models/flux_spec.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     4119 2023-05-04 17:45:25.000000 fluxoperator-0.0.22/fluxoperator/models/flux_user.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     4402 2023-05-04 17:45:25.000000 fluxoperator-0.0.22/fluxoperator/models/life_cycle.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     6622 2023-05-04 17:45:25.000000 fluxoperator-0.0.22/fluxoperator/models/logging_spec.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     7375 2023-05-04 17:45:25.000000 fluxoperator-0.0.22/fluxoperator/models/mini_cluster.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     3612 2023-05-04 17:45:25.000000 fluxoperator-0.0.22/fluxoperator/models/mini_cluster_archive.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)    23480 2023-05-05 02:07:25.000000 fluxoperator-0.0.22/fluxoperator/models/mini_cluster_container.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     5483 2023-05-04 17:45:25.000000 fluxoperator-0.0.22/fluxoperator/models/mini_cluster_existing_volume.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     6969 2023-05-04 17:45:25.000000 fluxoperator-0.0.22/fluxoperator/models/mini_cluster_list.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)    16292 2023-05-05 02:07:25.000000 fluxoperator-0.0.22/fluxoperator/models/mini_cluster_spec.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     5811 2023-05-04 17:45:25.000000 fluxoperator-0.0.22/fluxoperator/models/mini_cluster_status.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     4434 2023-05-04 17:45:25.000000 fluxoperator-0.0.22/fluxoperator/models/mini_cluster_user.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)    13029 2023-05-04 17:45:25.000000 fluxoperator-0.0.22/fluxoperator/models/mini_cluster_volume.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     7124 2023-05-04 17:45:25.000000 fluxoperator-0.0.22/fluxoperator/models/pod_spec.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     3683 2023-05-04 17:45:25.000000 fluxoperator-0.0.22/fluxoperator/models/security_context.py
+drwxrwxr-x   0 vanessa   (1000) vanessa   (1000)        0 2023-05-05 19:00:14.628271 fluxoperator-0.0.22/fluxoperator/resource/
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)        0 2023-04-07 19:58:49.000000 fluxoperator-0.0.22/fluxoperator/resource/__init__.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1910 2023-04-07 19:58:49.000000 fluxoperator-0.0.22/fluxoperator/resource/network.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     5913 2023-05-05 02:07:25.000000 fluxoperator-0.0.22/fluxoperator/resource/pods.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)    12590 2023-05-04 17:45:25.000000 fluxoperator-0.0.22/fluxoperator/rest.py
+drwxrwxr-x   0 vanessa   (1000) vanessa   (1000)        0 2023-05-05 19:00:14.624271 fluxoperator-0.0.22/fluxoperator.egg-info/
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     2694 2023-05-05 19:00:13.000000 fluxoperator-0.0.22/fluxoperator.egg-info/PKG-INFO
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1923 2023-05-05 19:00:14.000000 fluxoperator-0.0.22/fluxoperator.egg-info/SOURCES.txt
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)        1 2023-05-05 19:00:14.000000 fluxoperator-0.0.22/fluxoperator.egg-info/dependency_links.txt
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)        1 2023-02-25 05:06:19.000000 fluxoperator-0.0.22/fluxoperator.egg-info/not-zip-safe
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)       20 2023-05-05 19:00:14.000000 fluxoperator-0.0.22/fluxoperator.egg-info/requires.txt
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)       18 2023-05-05 19:00:14.000000 fluxoperator-0.0.22/fluxoperator.egg-info/top_level.txt
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)       69 2023-05-05 19:00:14.632271 fluxoperator-0.0.22/setup.cfg
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     2153 2023-05-04 17:45:25.000000 fluxoperator-0.0.22/setup.py
+drwxrwxr-x   0 vanessa   (1000) vanessa   (1000)        0 2023-05-05 19:00:14.632271 fluxoperator-0.0.22/test/
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)        0 2023-05-04 17:45:25.000000 fluxoperator-0.0.22/test/__init__.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1224 2023-04-07 19:58:49.000000 fluxoperator-0.0.22/test/test_commands.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1351 2023-04-07 19:58:49.000000 fluxoperator-0.0.22/test/test_container_resources.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1335 2023-04-07 19:58:49.000000 fluxoperator-0.0.22/test/test_container_volume.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1271 2023-04-07 19:58:49.000000 fluxoperator-0.0.22/test/test_flux_restful.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1307 2023-05-05 02:07:25.000000 fluxoperator-0.0.22/test/test_flux_spec.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1212 2023-04-07 19:58:49.000000 fluxoperator-0.0.22/test/test_flux_user.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1226 2023-04-07 19:58:49.000000 fluxoperator-0.0.22/test/test_life_cycle.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1277 2023-04-07 19:58:49.000000 fluxoperator-0.0.22/test/test_logging_spec.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     8167 2023-05-05 02:07:25.000000 fluxoperator-0.0.22/test/test_mini_cluster.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1316 2023-04-07 19:58:49.000000 fluxoperator-0.0.22/test/test_mini_cluster_archive.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     3559 2023-05-05 02:07:25.000000 fluxoperator-0.0.22/test/test_mini_cluster_container.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1504 2023-04-07 19:58:49.000000 fluxoperator-0.0.22/test/test_mini_cluster_existing_volume.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)    17751 2023-05-05 02:07:25.000000 fluxoperator-0.0.22/test/test_mini_cluster_list.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)    12352 2023-05-05 02:07:25.000000 fluxoperator-0.0.22/test/test_mini_cluster_spec.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1364 2023-04-07 19:58:49.000000 fluxoperator-0.0.22/test/test_mini_cluster_status.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1334 2023-04-07 19:58:49.000000 fluxoperator-0.0.22/test/test_mini_cluster_user.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1578 2023-04-07 19:58:49.000000 fluxoperator-0.0.22/test/test_mini_cluster_volume.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1284 2023-04-07 19:58:49.000000 fluxoperator-0.0.22/test/test_pod_spec.py
+-rw-rw-r--   0 vanessa   (1000) vanessa   (1000)     1289 2023-04-07 19:58:49.000000 fluxoperator-0.0.22/test/test_security_context.py
```

### Comparing `fluxoperator-0.0.21/PKG-INFO` & `fluxoperator-0.0.22/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fluxoperator
-Version: 0.0.21
+Version: 0.0.22
 Summary: Python SDK for the Flux Operator
 Home-page: https://github.com/flux-framework/flux-operator/tree/main/python-sdk/v1alpha1
 Author: Vanessasaurus
 Author-email: vsoch@users.noreply.github.com
 Maintainer: Vanessasaurus
 License: Apache 2.0
 Keywords: flux-operator,flux-framework,kubernetes,workflows,jobs-api
@@ -78,14 +78,15 @@
 
 ## Documentation For Models
 
  - [Commands](Commands.md)
  - [ContainerResources](dContainerResources.md)
  - [ContainerVolume](ContainerVolume.md)
  - [FluxRestful](FluxRestful.md)
+ - [FluxSpec](FluxSpec.md)
  - [FluxUser](FluxUser.md)
  - [LifeCycle](LifeCycle.md)
  - [LoggingSpec](LoggingSpec.md)
  - [MiniCluster](MiniCluster.md)
  - [MiniClusterArchive](MiniClusterArchive.md)
  - [MiniClusterContainer](MiniClusterContainer.md)
  - [MiniClusterList](MiniClusterList.md)
```

### Comparing `fluxoperator-0.0.21/fluxoperator/__init__.py` & `fluxoperator-0.0.22/fluxoperator/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -28,14 +28,15 @@
 from fluxoperator.exceptions import ApiAttributeError
 from fluxoperator.exceptions import ApiException
 # import models into sdk package
 from fluxoperator.models.commands import Commands
 from fluxoperator.models.container_resources import ContainerResources
 from fluxoperator.models.container_volume import ContainerVolume
 from fluxoperator.models.flux_restful import FluxRestful
+from fluxoperator.models.flux_spec import FluxSpec
 from fluxoperator.models.flux_user import FluxUser
 from fluxoperator.models.life_cycle import LifeCycle
 from fluxoperator.models.logging_spec import LoggingSpec
 from fluxoperator.models.mini_cluster import MiniCluster
 from fluxoperator.models.mini_cluster_archive import MiniClusterArchive
 from fluxoperator.models.mini_cluster_container import MiniClusterContainer
 from fluxoperator.models.mini_cluster_existing_volume import MiniClusterExistingVolume
```

### Comparing `fluxoperator-0.0.21/fluxoperator/api_client.py` & `fluxoperator-0.0.22/fluxoperator/api_client.py`

 * *Files identical despite different names*

### Comparing `fluxoperator-0.0.21/fluxoperator/client.py` & `fluxoperator-0.0.22/fluxoperator/client.py`

 * *Files identical despite different names*

### Comparing `fluxoperator-0.0.21/fluxoperator/configuration.py` & `fluxoperator-0.0.22/fluxoperator/configuration.py`

 * *Files identical despite different names*

### Comparing `fluxoperator-0.0.21/fluxoperator/decorator.py` & `fluxoperator-0.0.22/fluxoperator/decorator.py`

 * *Files identical despite different names*

### Comparing `fluxoperator-0.0.21/fluxoperator/exceptions.py` & `fluxoperator-0.0.22/fluxoperator/exceptions.py`

 * *Files identical despite different names*

### Comparing `fluxoperator-0.0.21/fluxoperator/models/__init__.py` & `fluxoperator-0.0.22/fluxoperator/models/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 from __future__ import absolute_import
 
 # import models into model package
 from fluxoperator.models.commands import Commands
 from fluxoperator.models.container_resources import ContainerResources
 from fluxoperator.models.container_volume import ContainerVolume
 from fluxoperator.models.flux_restful import FluxRestful
+from fluxoperator.models.flux_spec import FluxSpec
 from fluxoperator.models.flux_user import FluxUser
 from fluxoperator.models.life_cycle import LifeCycle
 from fluxoperator.models.logging_spec import LoggingSpec
 from fluxoperator.models.mini_cluster import MiniCluster
 from fluxoperator.models.mini_cluster_archive import MiniClusterArchive
 from fluxoperator.models.mini_cluster_container import MiniClusterContainer
 from fluxoperator.models.mini_cluster_existing_volume import MiniClusterExistingVolume
```

### Comparing `fluxoperator-0.0.21/fluxoperator/models/commands.py` & `fluxoperator-0.0.22/fluxoperator/models/commands.py`

 * *Files identical despite different names*

### Comparing `fluxoperator-0.0.21/fluxoperator/models/container_resources.py` & `fluxoperator-0.0.22/fluxoperator/models/container_resources.py`

 * *Files identical despite different names*

### Comparing `fluxoperator-0.0.21/fluxoperator/models/container_volume.py` & `fluxoperator-0.0.22/fluxoperator/models/container_volume.py`

 * *Files identical despite different names*

### Comparing `fluxoperator-0.0.21/fluxoperator/models/flux_restful.py` & `fluxoperator-0.0.22/fluxoperator/models/flux_restful.py`

 * *Files identical despite different names*

### Comparing `fluxoperator-0.0.21/fluxoperator/models/flux_user.py` & `fluxoperator-0.0.22/fluxoperator/models/flux_user.py`

 * *Files identical despite different names*

### Comparing `fluxoperator-0.0.21/fluxoperator/models/life_cycle.py` & `fluxoperator-0.0.22/fluxoperator/models/life_cycle.py`

 * *Files identical despite different names*

### Comparing `fluxoperator-0.0.21/fluxoperator/models/logging_spec.py` & `fluxoperator-0.0.22/fluxoperator/models/logging_spec.py`

 * *Files identical despite different names*

### Comparing `fluxoperator-0.0.21/fluxoperator/models/mini_cluster.py` & `fluxoperator-0.0.22/fluxoperator/models/mini_cluster.py`

 * *Files identical despite different names*

### Comparing `fluxoperator-0.0.21/fluxoperator/models/mini_cluster_archive.py` & `fluxoperator-0.0.22/fluxoperator/models/mini_cluster_archive.py`

 * *Files identical despite different names*

### Comparing `fluxoperator-0.0.21/fluxoperator/models/mini_cluster_container.py` & `fluxoperator-0.0.22/fluxoperator/models/mini_cluster_container.py`

 * *Files 6% similar despite different names*

```diff
@@ -37,16 +37,14 @@
         'batch_raw': 'bool',
         'command': 'str',
         'commands': 'Commands',
         'cores': 'int',
         'diagnostics': 'bool',
         'environment': 'dict(str, str)',
         'existing_volumes': 'dict(str, MiniClusterExistingVolume)',
-        'flux_log_level': 'int',
-        'flux_option_flags': 'str',
         'flux_user': 'FluxUser',
         'image': 'str',
         'image_pull_secret': 'str',
         'launcher': 'bool',
         'life_cycle': 'LifeCycle',
         'logs': 'str',
         'name': 'str',
@@ -65,16 +63,14 @@
         'batch_raw': 'batchRaw',
         'command': 'command',
         'commands': 'commands',
         'cores': 'cores',
         'diagnostics': 'diagnostics',
         'environment': 'environment',
         'existing_volumes': 'existingVolumes',
-        'flux_log_level': 'fluxLogLevel',
-        'flux_option_flags': 'fluxOptionFlags',
         'flux_user': 'fluxUser',
         'image': 'image',
         'image_pull_secret': 'imagePullSecret',
         'launcher': 'launcher',
         'life_cycle': 'lifeCycle',
         'logs': 'logs',
         'name': 'name',
@@ -84,30 +80,28 @@
         'resources': 'resources',
         'run_flux': 'runFlux',
         'security_context': 'securityContext',
         'volumes': 'volumes',
         'working_dir': 'workingDir'
     }
 
-    def __init__(self, batch=False, batch_raw=False, command='', commands=None, cores=0, diagnostics=False, environment=None, existing_volumes=None, flux_log_level=6, flux_option_flags='', flux_user=None, image='ghcr.io/rse-ops/accounting:app-latest', image_pull_secret='', launcher=False, life_cycle=None, logs='', name='', ports=None, pre_command='', pull_always=False, resources=None, run_flux=False, security_context=None, volumes=None, working_dir='', local_vars_configuration=None):  # noqa: E501
+    def __init__(self, batch=False, batch_raw=False, command='', commands=None, cores=0, diagnostics=False, environment=None, existing_volumes=None, flux_user=None, image='ghcr.io/rse-ops/accounting:app-latest', image_pull_secret='', launcher=False, life_cycle=None, logs='', name='', ports=None, pre_command='', pull_always=False, resources=None, run_flux=False, security_context=None, volumes=None, working_dir='', local_vars_configuration=None):  # noqa: E501
         """MiniClusterContainer - a model defined in OpenAPI"""  # noqa: E501
         if local_vars_configuration is None:
             local_vars_configuration = Configuration.get_default_copy()
         self.local_vars_configuration = local_vars_configuration
 
         self._batch = None
         self._batch_raw = None
         self._command = None
         self._commands = None
         self._cores = None
         self._diagnostics = None
         self._environment = None
         self._existing_volumes = None
-        self._flux_log_level = None
-        self._flux_option_flags = None
         self._flux_user = None
         self._image = None
         self._image_pull_secret = None
         self._launcher = None
         self._life_cycle = None
         self._logs = None
         self._name = None
@@ -133,18 +127,14 @@
             self.cores = cores
         if diagnostics is not None:
             self.diagnostics = diagnostics
         if environment is not None:
             self.environment = environment
         if existing_volumes is not None:
             self.existing_volumes = existing_volumes
-        if flux_log_level is not None:
-            self.flux_log_level = flux_log_level
-        if flux_option_flags is not None:
-            self.flux_option_flags = flux_option_flags
         if flux_user is not None:
             self.flux_user = flux_user
         if image is not None:
             self.image = image
         if image_pull_secret is not None:
             self.image_pull_secret = image_pull_secret
         if launcher is not None:
@@ -351,60 +341,14 @@
         :param existing_volumes: The existing_volumes of this MiniClusterContainer.  # noqa: E501
         :type existing_volumes: dict(str, MiniClusterExistingVolume)
         """
 
         self._existing_volumes = existing_volumes
 
     @property
-    def flux_log_level(self):
-        """Gets the flux_log_level of this MiniClusterContainer.  # noqa: E501
-
-        Log level to use for flux logging (only in non TestMode)  # noqa: E501
-
-        :return: The flux_log_level of this MiniClusterContainer.  # noqa: E501
-        :rtype: int
-        """
-        return self._flux_log_level
-
-    @flux_log_level.setter
-    def flux_log_level(self, flux_log_level):
-        """Sets the flux_log_level of this MiniClusterContainer.
-
-        Log level to use for flux logging (only in non TestMode)  # noqa: E501
-
-        :param flux_log_level: The flux_log_level of this MiniClusterContainer.  # noqa: E501
-        :type flux_log_level: int
-        """
-
-        self._flux_log_level = flux_log_level
-
-    @property
-    def flux_option_flags(self):
-        """Gets the flux_option_flags of this MiniClusterContainer.  # noqa: E501
-
-        Flux option flags, usually provided with -o optional - if needed, default option flags for the server These can also be set in the user interface to override here. This is only valid for a FluxRunner \"runFlux\" true  # noqa: E501
-
-        :return: The flux_option_flags of this MiniClusterContainer.  # noqa: E501
-        :rtype: str
-        """
-        return self._flux_option_flags
-
-    @flux_option_flags.setter
-    def flux_option_flags(self, flux_option_flags):
-        """Sets the flux_option_flags of this MiniClusterContainer.
-
-        Flux option flags, usually provided with -o optional - if needed, default option flags for the server These can also be set in the user interface to override here. This is only valid for a FluxRunner \"runFlux\" true  # noqa: E501
-
-        :param flux_option_flags: The flux_option_flags of this MiniClusterContainer.  # noqa: E501
-        :type flux_option_flags: str
-        """
-
-        self._flux_option_flags = flux_option_flags
-
-    @property
     def flux_user(self):
         """Gets the flux_user of this MiniClusterContainer.  # noqa: E501
 
 
         :return: The flux_user of this MiniClusterContainer.  # noqa: E501
         :rtype: FluxUser
         """
```

### Comparing `fluxoperator-0.0.21/fluxoperator/models/mini_cluster_existing_volume.py` & `fluxoperator-0.0.22/fluxoperator/models/mini_cluster_existing_volume.py`

 * *Files identical despite different names*

### Comparing `fluxoperator-0.0.21/fluxoperator/models/mini_cluster_list.py` & `fluxoperator-0.0.22/fluxoperator/models/mini_cluster_list.py`

 * *Files identical despite different names*

### Comparing `fluxoperator-0.0.21/fluxoperator/models/mini_cluster_spec.py` & `fluxoperator-0.0.22/fluxoperator/models/mini_cluster_spec.py`

 * *Files 4% similar despite different names*

```diff
@@ -33,57 +33,63 @@
                             and the value is json key in definition.
     """
     openapi_types = {
         'archive': 'MiniClusterArchive',
         'cleanup': 'bool',
         'containers': 'list[MiniClusterContainer]',
         'deadline_seconds': 'int',
+        'flux': 'FluxSpec',
         'flux_restful': 'FluxRestful',
         'interactive': 'bool',
         'job_labels': 'dict(str, str)',
         'logging': 'LoggingSpec',
+        'max_size': 'int',
         'pod': 'PodSpec',
         'services': 'list[MiniClusterContainer]',
         'size': 'int',
         'tasks': 'int',
         'users': 'list[MiniClusterUser]',
         'volumes': 'dict(str, MiniClusterVolume)'
     }
 
     attribute_map = {
         'archive': 'archive',
         'cleanup': 'cleanup',
         'containers': 'containers',
         'deadline_seconds': 'deadlineSeconds',
+        'flux': 'flux',
         'flux_restful': 'fluxRestful',
         'interactive': 'interactive',
         'job_labels': 'jobLabels',
         'logging': 'logging',
+        'max_size': 'maxSize',
         'pod': 'pod',
         'services': 'services',
         'size': 'size',
         'tasks': 'tasks',
         'users': 'users',
         'volumes': 'volumes'
     }
 
-    def __init__(self, archive=None, cleanup=False, containers=None, deadline_seconds=31500000, flux_restful=None, interactive=False, job_labels=None, logging=None, pod=None, services=None, size=1, tasks=1, users=None, volumes=None, local_vars_configuration=None):  # noqa: E501
+    def __init__(self, archive=None, cleanup=False, containers=None, deadline_seconds=31500000, flux=None, flux_restful=None, interactive=False, job_labels=None, logging=None, max_size=None, pod=None, services=None, size=1, tasks=1, users=None, volumes=None, local_vars_configuration=None):  # noqa: E501
         """MiniClusterSpec - a model defined in OpenAPI"""  # noqa: E501
         if local_vars_configuration is None:
             local_vars_configuration = Configuration.get_default_copy()
         self.local_vars_configuration = local_vars_configuration
 
         self._archive = None
         self._cleanup = None
         self._containers = None
         self._deadline_seconds = None
+        self._flux = None
         self._flux_restful = None
         self._interactive = None
         self._job_labels = None
         self._logging = None
+        self._max_size = None
         self._pod = None
         self._services = None
         self._size = None
         self._tasks = None
         self._users = None
         self._volumes = None
         self.discriminator = None
@@ -91,22 +97,26 @@
         if archive is not None:
             self.archive = archive
         if cleanup is not None:
             self.cleanup = cleanup
         self.containers = containers
         if deadline_seconds is not None:
             self.deadline_seconds = deadline_seconds
+        if flux is not None:
+            self.flux = flux
         if flux_restful is not None:
             self.flux_restful = flux_restful
         if interactive is not None:
             self.interactive = interactive
         if job_labels is not None:
             self.job_labels = job_labels
         if logging is not None:
             self.logging = logging
+        if max_size is not None:
+            self.max_size = max_size
         if pod is not None:
             self.pod = pod
         if services is not None:
             self.services = services
         if size is not None:
             self.size = size
         if tasks is not None:
@@ -205,14 +215,35 @@
         :param deadline_seconds: The deadline_seconds of this MiniClusterSpec.  # noqa: E501
         :type deadline_seconds: int
         """
 
         self._deadline_seconds = deadline_seconds
 
     @property
+    def flux(self):
+        """Gets the flux of this MiniClusterSpec.  # noqa: E501
+
+
+        :return: The flux of this MiniClusterSpec.  # noqa: E501
+        :rtype: FluxSpec
+        """
+        return self._flux
+
+    @flux.setter
+    def flux(self, flux):
+        """Sets the flux of this MiniClusterSpec.
+
+
+        :param flux: The flux of this MiniClusterSpec.  # noqa: E501
+        :type flux: FluxSpec
+        """
+
+        self._flux = flux
+
+    @property
     def flux_restful(self):
         """Gets the flux_restful of this MiniClusterSpec.  # noqa: E501
 
 
         :return: The flux_restful of this MiniClusterSpec.  # noqa: E501
         :rtype: FluxRestful
         """
@@ -293,14 +324,37 @@
         :param logging: The logging of this MiniClusterSpec.  # noqa: E501
         :type logging: LoggingSpec
         """
 
         self._logging = logging
 
     @property
+    def max_size(self):
+        """Gets the max_size of this MiniClusterSpec.  # noqa: E501
+
+        MaxSize (maximum number of pods to allow scaling to)  # noqa: E501
+
+        :return: The max_size of this MiniClusterSpec.  # noqa: E501
+        :rtype: int
+        """
+        return self._max_size
+
+    @max_size.setter
+    def max_size(self, max_size):
+        """Sets the max_size of this MiniClusterSpec.
+
+        MaxSize (maximum number of pods to allow scaling to)  # noqa: E501
+
+        :param max_size: The max_size of this MiniClusterSpec.  # noqa: E501
+        :type max_size: int
+        """
+
+        self._max_size = max_size
+
+    @property
     def pod(self):
         """Gets the pod of this MiniClusterSpec.  # noqa: E501
 
 
         :return: The pod of this MiniClusterSpec.  # noqa: E501
         :rtype: PodSpec
         """
@@ -340,26 +394,26 @@
 
         self._services = services
 
     @property
     def size(self):
         """Gets the size of this MiniClusterSpec.  # noqa: E501
 
-        Size (number of job pods to run, size of minicluster in pods)  # noqa: E501
+        Size (number of job pods to run, size of minicluster in pods) This is also the minimum number required to start Flux  # noqa: E501
 
         :return: The size of this MiniClusterSpec.  # noqa: E501
         :rtype: int
         """
         return self._size
 
     @size.setter
     def size(self, size):
         """Sets the size of this MiniClusterSpec.
 
-        Size (number of job pods to run, size of minicluster in pods)  # noqa: E501
+        Size (number of job pods to run, size of minicluster in pods) This is also the minimum number required to start Flux  # noqa: E501
 
         :param size: The size of this MiniClusterSpec.  # noqa: E501
         :type size: int
         """
 
         self._size = size
```

### Comparing `fluxoperator-0.0.21/fluxoperator/models/mini_cluster_status.py` & `fluxoperator-0.0.22/fluxoperator/models/mini_cluster_status.py`

 * *Files 16% similar despite different names*

```diff
@@ -30,35 +30,39 @@
       openapi_types (dict): The key is attribute name
                             and the value is attribute type.
       attribute_map (dict): The key is attribute name
                             and the value is json key in definition.
     """
     openapi_types = {
         'conditions': 'list[V1Condition]',
-        'jobid': 'str'
+        'jobid': 'str',
+        'size': 'int'
     }
 
     attribute_map = {
         'conditions': 'conditions',
-        'jobid': 'jobid'
+        'jobid': 'jobid',
+        'size': 'size'
     }
 
-    def __init__(self, conditions=None, jobid='', local_vars_configuration=None):  # noqa: E501
+    def __init__(self, conditions=None, jobid='', size=0, local_vars_configuration=None):  # noqa: E501
         """MiniClusterStatus - a model defined in OpenAPI"""  # noqa: E501
         if local_vars_configuration is None:
             local_vars_configuration = Configuration.get_default_copy()
         self.local_vars_configuration = local_vars_configuration
 
         self._conditions = None
         self._jobid = None
+        self._size = None
         self.discriminator = None
 
         if conditions is not None:
             self.conditions = conditions
         self.jobid = jobid
+        self.size = size
 
     @property
     def conditions(self):
         """Gets the conditions of this MiniClusterStatus.  # noqa: E501
 
         conditions hold the latest Flux Job and MiniCluster states  # noqa: E501
 
@@ -100,14 +104,39 @@
         :type jobid: str
         """
         if self.local_vars_configuration.client_side_validation and jobid is None:  # noqa: E501
             raise ValueError("Invalid value for `jobid`, must not be `None`")  # noqa: E501
 
         self._jobid = jobid
 
+    @property
+    def size(self):
+        """Gets the size of this MiniClusterStatus.  # noqa: E501
+
+        We keep the original size of the MiniCluster request as this is the absolute maximum  # noqa: E501
+
+        :return: The size of this MiniClusterStatus.  # noqa: E501
+        :rtype: int
+        """
+        return self._size
+
+    @size.setter
+    def size(self, size):
+        """Sets the size of this MiniClusterStatus.
+
+        We keep the original size of the MiniCluster request as this is the absolute maximum  # noqa: E501
+
+        :param size: The size of this MiniClusterStatus.  # noqa: E501
+        :type size: int
+        """
+        if self.local_vars_configuration.client_side_validation and size is None:  # noqa: E501
+            raise ValueError("Invalid value for `size`, must not be `None`")  # noqa: E501
+
+        self._size = size
+
     def to_dict(self, serialize=False):
         """Returns the model properties as a dict"""
         result = {}
 
         def convert(x):
             if hasattr(x, "to_dict"):
                 args = inspect.getargspec(x.to_dict).args
```

### Comparing `fluxoperator-0.0.21/fluxoperator/models/mini_cluster_user.py` & `fluxoperator-0.0.22/fluxoperator/models/mini_cluster_user.py`

 * *Files identical despite different names*

### Comparing `fluxoperator-0.0.21/fluxoperator/models/mini_cluster_volume.py` & `fluxoperator-0.0.22/fluxoperator/models/mini_cluster_volume.py`

 * *Files identical despite different names*

### Comparing `fluxoperator-0.0.21/fluxoperator/models/pod_spec.py` & `fluxoperator-0.0.22/fluxoperator/models/pod_spec.py`

 * *Files identical despite different names*

### Comparing `fluxoperator-0.0.21/fluxoperator/models/security_context.py` & `fluxoperator-0.0.22/fluxoperator/models/security_context.py`

 * *Files identical despite different names*

### Comparing `fluxoperator-0.0.21/fluxoperator/resource/network.py` & `fluxoperator-0.0.22/fluxoperator/resource/network.py`

 * *Files identical despite different names*

### Comparing `fluxoperator-0.0.21/fluxoperator/resource/pods.py` & `fluxoperator-0.0.22/fluxoperator/resource/pods.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from kubernetes import client, config
 import fluxoperator.models as models
 
 import fluxoperator.defaults as defaults
 import sys
 
 # These are known objects we will parse
-_objects = ["logging", "volumes", "resources", "flux_restful", "container", "resources"]
+_objects = ["logging", "volumes", "resources", "flux_restful", "container", "resources", "flux"]
 
 
 def _get_logging_spec(logging):
     """
     Return models.Logging
     """
     logging_defaults = {
@@ -38,14 +38,24 @@
         for attr in models.ContainerVolume.attribute_map:
             if attr in volume:
                 volume_spec[attr] = volume[attr]
         volumeset[name] = models.ContainerVolume(**volume_spec)
     return volumeset
 
 
+def _get_flux_spec(flux):
+    """
+    Get flux spec
+    """
+    fluxspec = {}
+    for k in models.FluxSpec.attribute_map:
+        if k in flux:
+            fluxspec[k] = flux[k]
+    return models.FluxSpec(**fluxspec)
+
 def _get_container_spec(container):
     """
     Get the container spec.
     """
     # For now only one container support, it must run Flux
     container_kwargs = {"run_flux": True}
     for k in models.MiniClusterContainer.attribute_map:
@@ -130,27 +140,28 @@
     crd_api = client.CustomObjectsApi()
 
     # We assume that this is a single container to run flux
     # Multi-container support can eventually be added.
     # TODO when requested, add pod resources
     container = _get_container_spec(container)
 
-    # Logging spec with pre-defined defaults
+    flux_spec = _get_flux_spec(kwargs.get("flux"))
     logging_spec = _get_logging_spec(kwargs.get("logging"))
     flux_restful = _get_flux_restful_spec(kwargs.get("flux_restful"))
     volumes = _get_volumes_spec(kwargs.get("volumes"))
     minicluster_kwargs = _get_minicluster_spec(kwargs)
 
     # Create the MiniCluster
     minicluster = models.MiniCluster(
         kind="MiniCluster",
         api_version=f"flux-framework.org/{defaults.flux_operator_api_version}",
         metadata=V1ObjectMeta(name=name, namespace=namespace),
         spec=models.MiniClusterSpec(
             **minicluster_kwargs,
+            flux=flux_spec,
             logging=logging_spec,
             containers=[container],
             flux_restful=flux_restful,
             volumes=volumes,
         ),
     )
```

### Comparing `fluxoperator-0.0.21/fluxoperator/rest.py` & `fluxoperator-0.0.22/fluxoperator/rest.py`

 * *Files identical despite different names*

### Comparing `fluxoperator-0.0.21/fluxoperator.egg-info/PKG-INFO` & `fluxoperator-0.0.22/fluxoperator.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fluxoperator
-Version: 0.0.21
+Version: 0.0.22
 Summary: Python SDK for the Flux Operator
 Home-page: https://github.com/flux-framework/flux-operator/tree/main/python-sdk/v1alpha1
 Author: Vanessasaurus
 Author-email: vsoch@users.noreply.github.com
 Maintainer: Vanessasaurus
 License: Apache 2.0
 Keywords: flux-operator,flux-framework,kubernetes,workflows,jobs-api
@@ -78,14 +78,15 @@
 
 ## Documentation For Models
 
  - [Commands](Commands.md)
  - [ContainerResources](dContainerResources.md)
  - [ContainerVolume](ContainerVolume.md)
  - [FluxRestful](FluxRestful.md)
+ - [FluxSpec](FluxSpec.md)
  - [FluxUser](FluxUser.md)
  - [LifeCycle](LifeCycle.md)
  - [LoggingSpec](LoggingSpec.md)
  - [MiniCluster](MiniCluster.md)
  - [MiniClusterArchive](MiniClusterArchive.md)
  - [MiniClusterContainer](MiniClusterContainer.md)
  - [MiniClusterList](MiniClusterList.md)
```

### Comparing `fluxoperator-0.0.21/fluxoperator.egg-info/SOURCES.txt` & `fluxoperator-0.0.22/fluxoperator.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -17,14 +17,15 @@
 fluxoperator.egg-info/top_level.txt
 fluxoperator/api/__init__.py
 fluxoperator/models/__init__.py
 fluxoperator/models/commands.py
 fluxoperator/models/container_resources.py
 fluxoperator/models/container_volume.py
 fluxoperator/models/flux_restful.py
+fluxoperator/models/flux_spec.py
 fluxoperator/models/flux_user.py
 fluxoperator/models/life_cycle.py
 fluxoperator/models/logging_spec.py
 fluxoperator/models/mini_cluster.py
 fluxoperator/models/mini_cluster_archive.py
 fluxoperator/models/mini_cluster_container.py
 fluxoperator/models/mini_cluster_existing_volume.py
@@ -39,14 +40,15 @@
 fluxoperator/resource/network.py
 fluxoperator/resource/pods.py
 test/__init__.py
 test/test_commands.py
 test/test_container_resources.py
 test/test_container_volume.py
 test/test_flux_restful.py
+test/test_flux_spec.py
 test/test_flux_user.py
 test/test_life_cycle.py
 test/test_logging_spec.py
 test/test_mini_cluster.py
 test/test_mini_cluster_archive.py
 test/test_mini_cluster_container.py
 test/test_mini_cluster_existing_volume.py
```

### Comparing `fluxoperator-0.0.21/setup.py` & `fluxoperator-0.0.22/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 ################################################################################
 # MAIN #########################################################################
 ################################################################################
 
 if __name__ == "__main__":
     setup(
         name="fluxoperator",
-        version="0.0.21",
+        version="0.0.22",
         author="Vanessasaurus",
         author_email="vsoch@users.noreply.github.com",
         maintainer="Vanessasaurus",
         packages=find_packages(),
         include_package_data=True,
         zip_safe=False,
         url="https://github.com/flux-framework/flux-operator/tree/main/python-sdk/v1alpha1",
```

### Comparing `fluxoperator-0.0.21/test/test_commands.py` & `fluxoperator-0.0.22/test/test_commands.py`

 * *Files identical despite different names*

### Comparing `fluxoperator-0.0.21/test/test_container_resources.py` & `fluxoperator-0.0.22/test/test_container_resources.py`

 * *Files identical despite different names*

### Comparing `fluxoperator-0.0.21/test/test_container_volume.py` & `fluxoperator-0.0.22/test/test_container_volume.py`

 * *Files identical despite different names*

### Comparing `fluxoperator-0.0.21/test/test_flux_restful.py` & `fluxoperator-0.0.22/test/test_flux_restful.py`

 * *Files identical despite different names*

### Comparing `fluxoperator-0.0.21/test/test_flux_user.py` & `fluxoperator-0.0.22/test/test_flux_user.py`

 * *Files identical despite different names*

### Comparing `fluxoperator-0.0.21/test/test_life_cycle.py` & `fluxoperator-0.0.22/test/test_life_cycle.py`

 * *Files identical despite different names*

### Comparing `fluxoperator-0.0.21/test/test_logging_spec.py` & `fluxoperator-0.0.22/test/test_logging_spec.py`

 * *Files identical despite different names*

### Comparing `fluxoperator-0.0.21/test/test_mini_cluster_archive.py` & `fluxoperator-0.0.22/test/test_mini_cluster_archive.py`

 * *Files identical despite different names*

### Comparing `fluxoperator-0.0.21/test/test_mini_cluster_existing_volume.py` & `fluxoperator-0.0.22/test/test_mini_cluster_existing_volume.py`

 * *Files identical despite different names*

### Comparing `fluxoperator-0.0.21/test/test_mini_cluster_status.py` & `fluxoperator-0.0.22/test/test_mini_cluster_status.py`

 * *Files identical despite different names*

### Comparing `fluxoperator-0.0.21/test/test_mini_cluster_user.py` & `fluxoperator-0.0.22/test/test_mini_cluster_user.py`

 * *Files identical despite different names*

### Comparing `fluxoperator-0.0.21/test/test_mini_cluster_volume.py` & `fluxoperator-0.0.22/test/test_mini_cluster_volume.py`

 * *Files identical despite different names*

### Comparing `fluxoperator-0.0.21/test/test_pod_spec.py` & `fluxoperator-0.0.22/test/test_pod_spec.py`

 * *Files identical despite different names*

### Comparing `fluxoperator-0.0.21/test/test_security_context.py` & `fluxoperator-0.0.22/test/test_security_context.py`

 * *Files identical despite different names*

