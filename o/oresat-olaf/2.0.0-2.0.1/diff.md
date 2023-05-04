# Comparing `tmp/oresat-olaf-2.0.0.tar.gz` & `tmp/oresat-olaf-2.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "oresat-olaf-2.0.0.tar", last modified: Sun Apr 23 21:15:41 2023, max compression
+gzip compressed data, was "oresat-olaf-2.0.1.tar", last modified: Thu May  4 23:18:36 2023, max compression
```

## Comparing `oresat-olaf-2.0.0.tar` & `oresat-olaf-2.0.1.tar`

### file list

```diff
@@ -1,87 +1,87 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 21:15:41.569478 oresat-olaf-2.0.0/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-04-23 21:15:27.000000 oresat-olaf-2.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2652 2023-04-23 21:15:41.569478 oresat-olaf-2.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1649 2023-04-23 21:15:27.000000 oresat-olaf-2.0.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 21:15:41.557478 oresat-olaf-2.0.0/olaf/
--rw-r--r--   0 runner    (1001) docker     (123)     2902 2023-04-23 21:15:27.000000 oresat-olaf-2.0.0/olaf/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 21:15:41.557478 oresat-olaf-2.0.0/olaf/_internals/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-23 21:15:27.000000 oresat-olaf-2.0.0/olaf/_internals/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7033 2023-04-23 21:15:27.000000 oresat-olaf-2.0.0/olaf/_internals/app.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 21:15:41.557478 oresat-olaf-2.0.0/olaf/_internals/data/
--rw-r--r--   0 runner    (1001) docker     (123)    82085 2023-04-23 21:15:27.000000 oresat-olaf-2.0.0/olaf/_internals/data/oresat_app.eds
--rw-r--r--   0 runner    (1001) docker     (123)     3987 2023-04-23 21:15:27.000000 oresat-olaf-2.0.0/olaf/_internals/master_node.py
--rw-r--r--   0 runner    (1001) docker     (123)    16649 2023-04-23 21:15:27.000000 oresat-olaf-2.0.0/olaf/_internals/node.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 21:15:41.557478 oresat-olaf-2.0.0/olaf/_internals/resources/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-23 21:15:27.000000 oresat-olaf-2.0.0/olaf/_internals/resources/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1581 2023-04-23 21:15:27.000000 oresat-olaf-2.0.0/olaf/_internals/resources/ecss.py
--rw-r--r--   0 runner    (1001) docker     (123)     3091 2023-04-23 21:15:27.000000 oresat-olaf-2.0.0/olaf/_internals/resources/file_caches.py
--rw-r--r--   0 runner    (1001) docker     (123)     2620 2023-04-23 21:15:27.000000 oresat-olaf-2.0.0/olaf/_internals/resources/fread.py
--rw-r--r--   0 runner    (1001) docker     (123)     2182 2023-04-23 21:15:27.000000 oresat-olaf-2.0.0/olaf/_internals/resources/fwrite.py
--rw-r--r--   0 runner    (1001) docker     (123)     1559 2023-04-23 21:15:27.000000 oresat-olaf-2.0.0/olaf/_internals/resources/logs.py
--rw-r--r--   0 runner    (1001) docker     (123)     3030 2023-04-23 21:15:27.000000 oresat-olaf-2.0.0/olaf/_internals/resources/os_command.py
--rw-r--r--   0 runner    (1001) docker     (123)      742 2023-04-23 21:15:27.000000 oresat-olaf-2.0.0/olaf/_internals/resources/power_control.py
--rw-r--r--   0 runner    (1001) docker     (123)      587 2023-04-23 21:15:27.000000 oresat-olaf-2.0.0/olaf/_internals/resources/store_eds.py
--rw-r--r--   0 runner    (1001) docker     (123)     4855 2023-04-23 21:15:27.000000 oresat-olaf-2.0.0/olaf/_internals/resources/system_info.py
--rw-r--r--   0 runner    (1001) docker     (123)     2339 2023-04-23 21:15:27.000000 oresat-olaf-2.0.0/olaf/_internals/resources/updater.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 21:15:41.561478 oresat-olaf-2.0.0/olaf/_internals/rest_api/
--rw-r--r--   0 runner    (1001) docker     (123)     8360 2023-04-23 21:15:27.000000 oresat-olaf-2.0.0/olaf/_internals/rest_api/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 21:15:41.561478 oresat-olaf-2.0.0/olaf/_internals/rest_api/static/
--rw-r--r--   0 runner    (1001) docker     (123)    15406 2023-04-23 21:15:27.000000 oresat-olaf-2.0.0/olaf/_internals/rest_api/static/favicon.ico
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 21:15:41.561478 oresat-olaf-2.0.0/olaf/_internals/rest_api/templates/
--rw-r--r--   0 runner    (1001) docker     (123)     2886 2023-04-23 21:15:27.000000 oresat-olaf-2.0.0/olaf/_internals/rest_api/templates/base.html
--rw-r--r--   0 runner    (1001) docker     (123)     2971 2023-04-23 21:15:27.000000 oresat-olaf-2.0.0/olaf/_internals/rest_api/templates/fread.html
--rw-r--r--   0 runner    (1001) docker     (123)     1356 2023-04-23 21:15:27.000000 oresat-olaf-2.0.0/olaf/_internals/rest_api/templates/fwrite.html
--rw-r--r--   0 runner    (1001) docker     (123)      583 2023-04-23 21:15:27.000000 oresat-olaf-2.0.0/olaf/_internals/rest_api/templates/logs.html
--rw-r--r--   0 runner    (1001) docker     (123)     4057 2023-04-23 21:15:27.000000 oresat-olaf-2.0.0/olaf/_internals/rest_api/templates/od.html
--rw-r--r--   0 runner    (1001) docker     (123)     2073 2023-04-23 21:15:27.000000 oresat-olaf-2.0.0/olaf/_internals/rest_api/templates/os_command.html
--rw-r--r--   0 runner    (1001) docker     (123)      640 2023-04-23 21:15:27.000000 oresat-olaf-2.0.0/olaf/_internals/rest_api/templates/power_control.html
--rw-r--r--   0 runner    (1001) docker     (123)      338 2023-04-23 21:15:27.000000 oresat-olaf-2.0.0/olaf/_internals/rest_api/templates/root.html
--rw-r--r--   0 runner    (1001) docker     (123)     3753 2023-04-23 21:15:27.000000 oresat-olaf-2.0.0/olaf/_internals/rest_api/templates/system_info.html
--rw-r--r--   0 runner    (1001) docker     (123)     2348 2023-04-23 21:15:27.000000 oresat-olaf-2.0.0/olaf/_internals/rest_api/templates/updater.html
--rw-r--r--   0 runner    (1001) docker     (123)    15344 2023-04-23 21:15:27.000000 oresat-olaf-2.0.0/olaf/_internals/updater.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 21:15:41.561478 oresat-olaf-2.0.0/olaf/common/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-23 21:15:27.000000 oresat-olaf-2.0.0/olaf/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1291 2023-04-23 21:15:27.000000 oresat-olaf-2.0.0/olaf/common/cpufreq.py
--rw-r--r--   0 runner    (1001) docker     (123)     2449 2023-04-23 21:15:27.000000 oresat-olaf-2.0.0/olaf/common/ecss.py
--rw-r--r--   0 runner    (1001) docker     (123)     2254 2023-04-23 21:15:27.000000 oresat-olaf-2.0.0/olaf/common/gpio.py
--rw-r--r--   0 runner    (1001) docker     (123)     3081 2023-04-23 21:15:27.000000 oresat-olaf-2.0.0/olaf/common/oresat_file.py
--rw-r--r--   0 runner    (1001) docker     (123)     6256 2023-04-23 21:15:27.000000 oresat-olaf-2.0.0/olaf/common/oresat_file_cache.py
--rw-r--r--   0 runner    (1001) docker     (123)     1460 2023-04-23 21:15:27.000000 oresat-olaf-2.0.0/olaf/common/resource.py
--rw-r--r--   0 runner    (1001) docker     (123)     3983 2023-04-23 21:15:27.000000 oresat-olaf-2.0.0/olaf/common/timer_loop.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 21:15:41.565478 oresat-olaf-2.0.0/olaf/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-23 21:15:27.000000 oresat-olaf-2.0.0/olaf/scripts/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2482 2023-04-23 21:15:27.000000 oresat-olaf-2.0.0/olaf/scripts/file_transfer.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1832 2023-04-23 21:15:27.000000 oresat-olaf-2.0.0/olaf/scripts/new_eds.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1212 2023-04-23 21:15:27.000000 oresat-olaf-2.0.0/olaf/scripts/os_command.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5444 2023-04-23 21:15:27.000000 oresat-olaf-2.0.0/olaf/scripts/sdo_transfer.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      456 2023-04-23 21:15:27.000000 oresat-olaf-2.0.0/olaf/scripts/sync.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     3541 2023-04-23 21:15:27.000000 oresat-olaf-2.0.0/olaf/scripts/system_info.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 21:15:41.565478 oresat-olaf-2.0.0/oresat_olaf.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2652 2023-04-23 21:15:41.000000 oresat-olaf-2.0.0/oresat_olaf.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2337 2023-04-23 21:15:41.000000 oresat-olaf-2.0.0/oresat_olaf.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-23 21:15:41.000000 oresat-olaf-2.0.0/oresat_olaf.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      294 2023-04-23 21:15:41.000000 oresat-olaf-2.0.0/oresat_olaf.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-04-23 21:15:41.000000 oresat-olaf-2.0.0/oresat_olaf.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-23 21:15:41.000000 oresat-olaf-2.0.0/oresat_olaf.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-23 21:15:27.000000 oresat-olaf-2.0.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     1510 2023-04-23 21:15:41.569478 oresat-olaf-2.0.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 21:15:41.565478 oresat-olaf-2.0.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-23 21:15:27.000000 oresat-olaf-2.0.0/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 21:15:41.565478 oresat-olaf-2.0.0/tests/common/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-23 21:15:27.000000 oresat-olaf-2.0.0/tests/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      526 2023-04-23 21:15:27.000000 oresat-olaf-2.0.0/tests/common/test_ecss.py
--rw-r--r--   0 runner    (1001) docker     (123)     2066 2023-04-23 21:15:27.000000 oresat-olaf-2.0.0/tests/common/test_oresat_file.py
--rw-r--r--   0 runner    (1001) docker     (123)    10193 2023-04-23 21:15:27.000000 oresat-olaf-2.0.0/tests/common/test_oresat_file_cache.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 21:15:41.565478 oresat-olaf-2.0.0/tests/internals/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-23 21:15:27.000000 oresat-olaf-2.0.0/tests/internals/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 21:15:41.569478 oresat-olaf-2.0.0/tests/internals/resources/
--rw-r--r--   0 runner    (1001) docker     (123)     2242 2023-04-23 21:15:27.000000 oresat-olaf-2.0.0/tests/internals/resources/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      463 2023-04-23 21:15:27.000000 oresat-olaf-2.0.0/tests/internals/resources/test_ecss.py
--rw-r--r--   0 runner    (1001) docker     (123)     7161 2023-04-23 21:15:27.000000 oresat-olaf-2.0.0/tests/internals/resources/test_file_caches.py
--rw-r--r--   0 runner    (1001) docker     (123)     2046 2023-04-23 21:15:27.000000 oresat-olaf-2.0.0/tests/internals/resources/test_fread.py
--rw-r--r--   0 runner    (1001) docker     (123)     2297 2023-04-23 21:15:27.000000 oresat-olaf-2.0.0/tests/internals/resources/test_fwrite.py
--rw-r--r--   0 runner    (1001) docker     (123)     1426 2023-04-23 21:15:27.000000 oresat-olaf-2.0.0/tests/internals/resources/test_os_command.py
--rw-r--r--   0 runner    (1001) docker     (123)     2871 2023-04-23 21:15:27.000000 oresat-olaf-2.0.0/tests/internals/resources/test_system_info.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-23 21:15:41.569478 oresat-olaf-2.0.0/tests/internals/updater/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-23 21:15:27.000000 oresat-olaf-2.0.0/tests/internals/updater/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6556 2023-04-23 21:15:27.000000 oresat-olaf-2.0.0/tests/internals/updater/test_updater.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 23:18:36.917580 oresat-olaf-2.0.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-05-04 23:18:23.000000 oresat-olaf-2.0.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2652 2023-05-04 23:18:36.917580 oresat-olaf-2.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1649 2023-05-04 23:18:23.000000 oresat-olaf-2.0.1/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 23:18:36.897580 oresat-olaf-2.0.1/olaf/
+-rw-r--r--   0 runner    (1001) docker     (123)     2912 2023-05-04 23:18:23.000000 oresat-olaf-2.0.1/olaf/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 23:18:36.901580 oresat-olaf-2.0.1/olaf/_internals/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 23:18:23.000000 oresat-olaf-2.0.1/olaf/_internals/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7033 2023-05-04 23:18:23.000000 oresat-olaf-2.0.1/olaf/_internals/app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 23:18:36.901580 oresat-olaf-2.0.1/olaf/_internals/data/
+-rw-r--r--   0 runner    (1001) docker     (123)    82085 2023-05-04 23:18:23.000000 oresat-olaf-2.0.1/olaf/_internals/data/oresat_app.eds
+-rw-r--r--   0 runner    (1001) docker     (123)     3987 2023-05-04 23:18:23.000000 oresat-olaf-2.0.1/olaf/_internals/master_node.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16649 2023-05-04 23:18:23.000000 oresat-olaf-2.0.1/olaf/_internals/node.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 23:18:36.905580 oresat-olaf-2.0.1/olaf/_internals/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 23:18:23.000000 oresat-olaf-2.0.1/olaf/_internals/resources/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1581 2023-05-04 23:18:23.000000 oresat-olaf-2.0.1/olaf/_internals/resources/ecss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3091 2023-05-04 23:18:23.000000 oresat-olaf-2.0.1/olaf/_internals/resources/file_caches.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2620 2023-05-04 23:18:23.000000 oresat-olaf-2.0.1/olaf/_internals/resources/fread.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2182 2023-05-04 23:18:23.000000 oresat-olaf-2.0.1/olaf/_internals/resources/fwrite.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1559 2023-05-04 23:18:23.000000 oresat-olaf-2.0.1/olaf/_internals/resources/logs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3030 2023-05-04 23:18:23.000000 oresat-olaf-2.0.1/olaf/_internals/resources/os_command.py
+-rw-r--r--   0 runner    (1001) docker     (123)      742 2023-05-04 23:18:23.000000 oresat-olaf-2.0.1/olaf/_internals/resources/power_control.py
+-rw-r--r--   0 runner    (1001) docker     (123)      587 2023-05-04 23:18:23.000000 oresat-olaf-2.0.1/olaf/_internals/resources/store_eds.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4855 2023-05-04 23:18:23.000000 oresat-olaf-2.0.1/olaf/_internals/resources/system_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2339 2023-05-04 23:18:23.000000 oresat-olaf-2.0.1/olaf/_internals/resources/updater.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 23:18:36.905580 oresat-olaf-2.0.1/olaf/_internals/rest_api/
+-rw-r--r--   0 runner    (1001) docker     (123)     8360 2023-05-04 23:18:23.000000 oresat-olaf-2.0.1/olaf/_internals/rest_api/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 23:18:36.905580 oresat-olaf-2.0.1/olaf/_internals/rest_api/static/
+-rw-r--r--   0 runner    (1001) docker     (123)    15406 2023-05-04 23:18:23.000000 oresat-olaf-2.0.1/olaf/_internals/rest_api/static/favicon.ico
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 23:18:36.909580 oresat-olaf-2.0.1/olaf/_internals/rest_api/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)     2886 2023-05-04 23:18:23.000000 oresat-olaf-2.0.1/olaf/_internals/rest_api/templates/base.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2971 2023-05-04 23:18:23.000000 oresat-olaf-2.0.1/olaf/_internals/rest_api/templates/fread.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1356 2023-05-04 23:18:23.000000 oresat-olaf-2.0.1/olaf/_internals/rest_api/templates/fwrite.html
+-rw-r--r--   0 runner    (1001) docker     (123)      583 2023-05-04 23:18:23.000000 oresat-olaf-2.0.1/olaf/_internals/rest_api/templates/logs.html
+-rw-r--r--   0 runner    (1001) docker     (123)     4057 2023-05-04 23:18:23.000000 oresat-olaf-2.0.1/olaf/_internals/rest_api/templates/od.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2073 2023-05-04 23:18:23.000000 oresat-olaf-2.0.1/olaf/_internals/rest_api/templates/os_command.html
+-rw-r--r--   0 runner    (1001) docker     (123)      640 2023-05-04 23:18:23.000000 oresat-olaf-2.0.1/olaf/_internals/rest_api/templates/power_control.html
+-rw-r--r--   0 runner    (1001) docker     (123)      338 2023-05-04 23:18:23.000000 oresat-olaf-2.0.1/olaf/_internals/rest_api/templates/root.html
+-rw-r--r--   0 runner    (1001) docker     (123)     3753 2023-05-04 23:18:23.000000 oresat-olaf-2.0.1/olaf/_internals/rest_api/templates/system_info.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2348 2023-05-04 23:18:23.000000 oresat-olaf-2.0.1/olaf/_internals/rest_api/templates/updater.html
+-rw-r--r--   0 runner    (1001) docker     (123)    15344 2023-05-04 23:18:23.000000 oresat-olaf-2.0.1/olaf/_internals/updater.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 23:18:36.909580 oresat-olaf-2.0.1/olaf/common/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 23:18:23.000000 oresat-olaf-2.0.1/olaf/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1291 2023-05-04 23:18:23.000000 oresat-olaf-2.0.1/olaf/common/cpufreq.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2449 2023-05-04 23:18:23.000000 oresat-olaf-2.0.1/olaf/common/ecss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2254 2023-05-04 23:18:23.000000 oresat-olaf-2.0.1/olaf/common/gpio.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3081 2023-05-04 23:18:23.000000 oresat-olaf-2.0.1/olaf/common/oresat_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6256 2023-05-04 23:18:23.000000 oresat-olaf-2.0.1/olaf/common/oresat_file_cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1460 2023-05-04 23:18:23.000000 oresat-olaf-2.0.1/olaf/common/resource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3983 2023-05-04 23:18:23.000000 oresat-olaf-2.0.1/olaf/common/timer_loop.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 23:18:36.913580 oresat-olaf-2.0.1/olaf/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 23:18:23.000000 oresat-olaf-2.0.1/olaf/scripts/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2482 2023-05-04 23:18:23.000000 oresat-olaf-2.0.1/olaf/scripts/file_transfer.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1832 2023-05-04 23:18:23.000000 oresat-olaf-2.0.1/olaf/scripts/new_eds.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1212 2023-05-04 23:18:23.000000 oresat-olaf-2.0.1/olaf/scripts/os_command.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5444 2023-05-04 23:18:23.000000 oresat-olaf-2.0.1/olaf/scripts/sdo_transfer.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      456 2023-05-04 23:18:23.000000 oresat-olaf-2.0.1/olaf/scripts/sync.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     3541 2023-05-04 23:18:23.000000 oresat-olaf-2.0.1/olaf/scripts/system_info.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 23:18:36.913580 oresat-olaf-2.0.1/oresat_olaf.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2652 2023-05-04 23:18:36.000000 oresat-olaf-2.0.1/oresat_olaf.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2337 2023-05-04 23:18:36.000000 oresat-olaf-2.0.1/oresat_olaf.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-04 23:18:36.000000 oresat-olaf-2.0.1/oresat_olaf.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      294 2023-05-04 23:18:36.000000 oresat-olaf-2.0.1/oresat_olaf.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-05-04 23:18:36.000000 oresat-olaf-2.0.1/oresat_olaf.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-04 23:18:36.000000 oresat-olaf-2.0.1/oresat_olaf.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-05-04 23:18:23.000000 oresat-olaf-2.0.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     1510 2023-05-04 23:18:36.917580 oresat-olaf-2.0.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 23:18:36.913580 oresat-olaf-2.0.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 23:18:23.000000 oresat-olaf-2.0.1/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 23:18:36.917580 oresat-olaf-2.0.1/tests/common/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 23:18:23.000000 oresat-olaf-2.0.1/tests/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      526 2023-05-04 23:18:23.000000 oresat-olaf-2.0.1/tests/common/test_ecss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2066 2023-05-04 23:18:23.000000 oresat-olaf-2.0.1/tests/common/test_oresat_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10193 2023-05-04 23:18:23.000000 oresat-olaf-2.0.1/tests/common/test_oresat_file_cache.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 23:18:36.917580 oresat-olaf-2.0.1/tests/internals/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 23:18:23.000000 oresat-olaf-2.0.1/tests/internals/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 23:18:36.917580 oresat-olaf-2.0.1/tests/internals/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)     2242 2023-05-04 23:18:23.000000 oresat-olaf-2.0.1/tests/internals/resources/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      463 2023-05-04 23:18:23.000000 oresat-olaf-2.0.1/tests/internals/resources/test_ecss.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7161 2023-05-04 23:18:23.000000 oresat-olaf-2.0.1/tests/internals/resources/test_file_caches.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2046 2023-05-04 23:18:23.000000 oresat-olaf-2.0.1/tests/internals/resources/test_fread.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2297 2023-05-04 23:18:23.000000 oresat-olaf-2.0.1/tests/internals/resources/test_fwrite.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1426 2023-05-04 23:18:23.000000 oresat-olaf-2.0.1/tests/internals/resources/test_os_command.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2871 2023-05-04 23:18:23.000000 oresat-olaf-2.0.1/tests/internals/resources/test_system_info.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 23:18:36.917580 oresat-olaf-2.0.1/tests/internals/updater/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 23:18:23.000000 oresat-olaf-2.0.1/tests/internals/updater/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6556 2023-05-04 23:18:23.000000 oresat-olaf-2.0.1/tests/internals/updater/test_updater.py
```

### Comparing `oresat-olaf-2.0.0/LICENSE` & `oresat-olaf-2.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `oresat-olaf-2.0.0/PKG-INFO` & `oresat-olaf-2.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oresat-olaf
-Version: 2.0.0
+Version: 2.0.1
 Summary: Application framework for all OreSat Linux boards
 Home-page: https://github.com/oresat/oresat-olaf
 Author: PSAS
 Author-email: oresat@pdx.edu
 Maintainer: PSAS
 Maintainer-email: oresat@pdx.edu
 License: GPL-3.0
```

### Comparing `oresat-olaf-2.0.0/README.rst` & `oresat-olaf-2.0.1/README.rst`

 * *Files identical despite different names*

### Comparing `oresat-olaf-2.0.0/olaf/__init__.py` & `oresat-olaf-2.0.1/olaf/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,25 +2,25 @@
 import sys
 from logging.handlers import SysLogHandler
 from argparse import ArgumentParser, Namespace
 
 from loguru import logger
 
 from ._internals.app import app, App
-from ._internals.node import Node, NetworkError
+from ._internals.node import Node, NodeStop, NetworkError
 from ._internals.master_node import MasterNode
 from ._internals.rest_api import rest_api, RestAPI, render_olaf_template
 from .common.resource import Resource
 from .common.ecss import scet_int_from_time, scet_int_to_time, utc_int_from_time, utc_int_to_time
 from .common.oresat_file import OreSatFile, new_oresat_file
 from .common.oresat_file_cache import OreSatFileCache
 from .common.timer_loop import TimerLoop
 from .common.gpio import GPIO
 
-__version__ = '2.0.0'
+__version__ = '2.0.1'
 
 
 def olaf_setup(eds_path: str = None, master_node: bool = False) -> Namespace:
     '''
     Parse runtime args and setup the app and REST API.
 
     Parameters
```

### Comparing `oresat-olaf-2.0.0/olaf/_internals/app.py` & `oresat-olaf-2.0.1/olaf/_internals/app.py`

 * *Files identical despite different names*

### Comparing `oresat-olaf-2.0.0/olaf/_internals/data/oresat_app.eds` & `oresat-olaf-2.0.1/olaf/_internals/data/oresat_app.eds`

 * *Files identical despite different names*

### Comparing `oresat-olaf-2.0.0/olaf/_internals/master_node.py` & `oresat-olaf-2.0.1/olaf/_internals/master_node.py`

 * *Files identical despite different names*

### Comparing `oresat-olaf-2.0.0/olaf/_internals/node.py` & `oresat-olaf-2.0.1/olaf/_internals/node.py`

 * *Files identical despite different names*

### Comparing `oresat-olaf-2.0.0/olaf/_internals/resources/ecss.py` & `oresat-olaf-2.0.1/olaf/_internals/resources/ecss.py`

 * *Files identical despite different names*

### Comparing `oresat-olaf-2.0.0/olaf/_internals/resources/file_caches.py` & `oresat-olaf-2.0.1/olaf/_internals/resources/file_caches.py`

 * *Files identical despite different names*

### Comparing `oresat-olaf-2.0.0/olaf/_internals/resources/fread.py` & `oresat-olaf-2.0.1/olaf/_internals/resources/fread.py`

 * *Files identical despite different names*

### Comparing `oresat-olaf-2.0.0/olaf/_internals/resources/fwrite.py` & `oresat-olaf-2.0.1/olaf/_internals/resources/fwrite.py`

 * *Files identical despite different names*

### Comparing `oresat-olaf-2.0.0/olaf/_internals/resources/logs.py` & `oresat-olaf-2.0.1/olaf/_internals/resources/logs.py`

 * *Files identical despite different names*

### Comparing `oresat-olaf-2.0.0/olaf/_internals/resources/os_command.py` & `oresat-olaf-2.0.1/olaf/_internals/resources/os_command.py`

 * *Files identical despite different names*

### Comparing `oresat-olaf-2.0.0/olaf/_internals/resources/power_control.py` & `oresat-olaf-2.0.1/olaf/_internals/resources/power_control.py`

 * *Files identical despite different names*

### Comparing `oresat-olaf-2.0.0/olaf/_internals/resources/store_eds.py` & `oresat-olaf-2.0.1/olaf/_internals/resources/store_eds.py`

 * *Files identical despite different names*

### Comparing `oresat-olaf-2.0.0/olaf/_internals/resources/system_info.py` & `oresat-olaf-2.0.1/olaf/_internals/resources/system_info.py`

 * *Files identical despite different names*

### Comparing `oresat-olaf-2.0.0/olaf/_internals/resources/updater.py` & `oresat-olaf-2.0.1/olaf/_internals/resources/updater.py`

 * *Files identical despite different names*

### Comparing `oresat-olaf-2.0.0/olaf/_internals/rest_api/__init__.py` & `oresat-olaf-2.0.1/olaf/_internals/rest_api/__init__.py`

 * *Files identical despite different names*

### Comparing `oresat-olaf-2.0.0/olaf/_internals/rest_api/static/favicon.ico` & `oresat-olaf-2.0.1/olaf/_internals/rest_api/static/favicon.ico`

 * *Files identical despite different names*

### Comparing `oresat-olaf-2.0.0/olaf/_internals/rest_api/templates/base.html` & `oresat-olaf-2.0.1/olaf/_internals/rest_api/templates/base.html`

 * *Files 1% similar despite different names*

```diff
@@ -67,15 +67,15 @@
         },
         'body': JSON.stringify({
           'value': value,
         }),
       };
       
       let url = `http://${window.location.host}/od/${index}`;
-      if (subindex !== null || subindex !== '') {
+      if (subindex !== null && subindex !== '') {
         url = `http://${window.location.host}/od/${index}/${subindex}`;
       }
 
       return await fetch(url, options)
         .then(response => response.json())
         .then(data => { return data; });
     }
```

### Comparing `oresat-olaf-2.0.0/olaf/_internals/rest_api/templates/fread.html` & `oresat-olaf-2.0.1/olaf/_internals/rest_api/templates/fread.html`

 * *Files identical despite different names*

### Comparing `oresat-olaf-2.0.0/olaf/_internals/rest_api/templates/fwrite.html` & `oresat-olaf-2.0.1/olaf/_internals/rest_api/templates/fwrite.html`

 * *Files identical despite different names*

### Comparing `oresat-olaf-2.0.0/olaf/_internals/rest_api/templates/logs.html` & `oresat-olaf-2.0.1/olaf/_internals/rest_api/templates/logs.html`

 * *Files identical despite different names*

### Comparing `oresat-olaf-2.0.0/olaf/_internals/rest_api/templates/od.html` & `oresat-olaf-2.0.1/olaf/_internals/rest_api/templates/od.html`

 * *Files identical despite different names*

### Comparing `oresat-olaf-2.0.0/olaf/_internals/rest_api/templates/os_command.html` & `oresat-olaf-2.0.1/olaf/_internals/rest_api/templates/os_command.html`

 * *Files identical despite different names*

### Comparing `oresat-olaf-2.0.0/olaf/_internals/rest_api/templates/power_control.html` & `oresat-olaf-2.0.1/olaf/_internals/rest_api/templates/power_control.html`

 * *Files identical despite different names*

### Comparing `oresat-olaf-2.0.0/olaf/_internals/rest_api/templates/system_info.html` & `oresat-olaf-2.0.1/olaf/_internals/rest_api/templates/system_info.html`

 * *Files identical despite different names*

### Comparing `oresat-olaf-2.0.0/olaf/_internals/rest_api/templates/updater.html` & `oresat-olaf-2.0.1/olaf/_internals/rest_api/templates/updater.html`

 * *Files identical despite different names*

### Comparing `oresat-olaf-2.0.0/olaf/_internals/updater.py` & `oresat-olaf-2.0.1/olaf/_internals/updater.py`

 * *Files identical despite different names*

### Comparing `oresat-olaf-2.0.0/olaf/common/cpufreq.py` & `oresat-olaf-2.0.1/olaf/common/cpufreq.py`

 * *Files identical despite different names*

### Comparing `oresat-olaf-2.0.0/olaf/common/ecss.py` & `oresat-olaf-2.0.1/olaf/common/ecss.py`

 * *Files identical despite different names*

### Comparing `oresat-olaf-2.0.0/olaf/common/gpio.py` & `oresat-olaf-2.0.1/olaf/common/gpio.py`

 * *Files identical despite different names*

### Comparing `oresat-olaf-2.0.0/olaf/common/oresat_file.py` & `oresat-olaf-2.0.1/olaf/common/oresat_file.py`

 * *Files identical despite different names*

### Comparing `oresat-olaf-2.0.0/olaf/common/oresat_file_cache.py` & `oresat-olaf-2.0.1/olaf/common/oresat_file_cache.py`

 * *Files identical despite different names*

### Comparing `oresat-olaf-2.0.0/olaf/common/resource.py` & `oresat-olaf-2.0.1/olaf/common/resource.py`

 * *Files identical despite different names*

### Comparing `oresat-olaf-2.0.0/olaf/common/timer_loop.py` & `oresat-olaf-2.0.1/olaf/common/timer_loop.py`

 * *Files identical despite different names*

### Comparing `oresat-olaf-2.0.0/olaf/scripts/file_transfer.py` & `oresat-olaf-2.0.1/olaf/scripts/file_transfer.py`

 * *Files identical despite different names*

### Comparing `oresat-olaf-2.0.0/olaf/scripts/new_eds.py` & `oresat-olaf-2.0.1/olaf/scripts/new_eds.py`

 * *Files identical despite different names*

### Comparing `oresat-olaf-2.0.0/olaf/scripts/os_command.py` & `oresat-olaf-2.0.1/olaf/scripts/os_command.py`

 * *Files identical despite different names*

### Comparing `oresat-olaf-2.0.0/olaf/scripts/sdo_transfer.py` & `oresat-olaf-2.0.1/olaf/scripts/sdo_transfer.py`

 * *Files identical despite different names*

### Comparing `oresat-olaf-2.0.0/olaf/scripts/system_info.py` & `oresat-olaf-2.0.1/olaf/scripts/system_info.py`

 * *Files identical despite different names*

### Comparing `oresat-olaf-2.0.0/oresat_olaf.egg-info/PKG-INFO` & `oresat-olaf-2.0.1/oresat_olaf.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: oresat-olaf
-Version: 2.0.0
+Version: 2.0.1
 Summary: Application framework for all OreSat Linux boards
 Home-page: https://github.com/oresat/oresat-olaf
 Author: PSAS
 Author-email: oresat@pdx.edu
 Maintainer: PSAS
 Maintainer-email: oresat@pdx.edu
 License: GPL-3.0
```

### Comparing `oresat-olaf-2.0.0/oresat_olaf.egg-info/SOURCES.txt` & `oresat-olaf-2.0.1/oresat_olaf.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `oresat-olaf-2.0.0/setup.cfg` & `oresat-olaf-2.0.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `oresat-olaf-2.0.0/tests/common/test_ecss.py` & `oresat-olaf-2.0.1/tests/common/test_ecss.py`

 * *Files identical despite different names*

### Comparing `oresat-olaf-2.0.0/tests/common/test_oresat_file.py` & `oresat-olaf-2.0.1/tests/common/test_oresat_file.py`

 * *Files identical despite different names*

### Comparing `oresat-olaf-2.0.0/tests/common/test_oresat_file_cache.py` & `oresat-olaf-2.0.1/tests/common/test_oresat_file_cache.py`

 * *Files identical despite different names*

### Comparing `oresat-olaf-2.0.0/tests/internals/resources/__init__.py` & `oresat-olaf-2.0.1/tests/internals/resources/__init__.py`

 * *Files identical despite different names*

### Comparing `oresat-olaf-2.0.0/tests/internals/resources/test_file_caches.py` & `oresat-olaf-2.0.1/tests/internals/resources/test_file_caches.py`

 * *Files identical despite different names*

### Comparing `oresat-olaf-2.0.0/tests/internals/resources/test_fread.py` & `oresat-olaf-2.0.1/tests/internals/resources/test_fread.py`

 * *Files identical despite different names*

### Comparing `oresat-olaf-2.0.0/tests/internals/resources/test_fwrite.py` & `oresat-olaf-2.0.1/tests/internals/resources/test_fwrite.py`

 * *Files identical despite different names*

### Comparing `oresat-olaf-2.0.0/tests/internals/resources/test_os_command.py` & `oresat-olaf-2.0.1/tests/internals/resources/test_os_command.py`

 * *Files identical despite different names*

### Comparing `oresat-olaf-2.0.0/tests/internals/resources/test_system_info.py` & `oresat-olaf-2.0.1/tests/internals/resources/test_system_info.py`

 * *Files identical despite different names*

### Comparing `oresat-olaf-2.0.0/tests/internals/updater/test_updater.py` & `oresat-olaf-2.0.1/tests/internals/updater/test_updater.py`

 * *Files identical despite different names*

