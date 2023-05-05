# Comparing `tmp/libdyson-neon-1.0.1.tar.gz` & `tmp/libdyson-neon-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "libdyson-neon-1.0.1.tar", last modified: Thu May  4 21:14:50 2023, max compression
+gzip compressed data, was "libdyson-neon-1.0.2.tar", last modified: Fri May  5 16:00:04 2023, max compression
```

## Comparing `libdyson-neon-1.0.1.tar` & `libdyson-neon-1.0.2.tar`

### file list

```diff
@@ -1,65 +1,65 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 21:14:50.602812 libdyson-neon-1.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-04 21:14:36.000000 libdyson-neon-1.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-05-04 21:14:36.000000 libdyson-neon-1.0.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      966 2023-05-04 21:14:50.602812 libdyson-neon-1.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      404 2023-05-04 21:14:36.000000 libdyson-neon-1.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 21:14:50.594812 libdyson-neon-1.0.1/libdyson/
--rw-r--r--   0 runner    (1001) docker     (123)     2859 2023-05-04 21:14:36.000000 libdyson-neon-1.0.1/libdyson/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 21:14:50.598812 libdyson-neon-1.0.1/libdyson/cloud/
--rw-r--r--   0 runner    (1001) docker     (123)      304 2023-05-04 21:14:36.000000 libdyson-neon-1.0.1/libdyson/cloud/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8064 2023-05-04 21:14:36.000000 libdyson-neon-1.0.1/libdyson/cloud/account.py
--rw-r--r--   0 runner    (1001) docker     (123)     2014 2023-05-04 21:14:36.000000 libdyson-neon-1.0.1/libdyson/cloud/cloud_360_eye.py
--rw-r--r--   0 runner    (1001) docker     (123)      285 2023-05-04 21:14:36.000000 libdyson-neon-1.0.1/libdyson/cloud/cloud_device.py
--rw-r--r--   0 runner    (1001) docker     (123)      775 2023-05-04 21:14:36.000000 libdyson-neon-1.0.1/libdyson/cloud/device_info.py
--rw-r--r--   0 runner    (1001) docker     (123)      990 2023-05-04 21:14:36.000000 libdyson-neon-1.0.1/libdyson/cloud/regions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1004 2023-05-04 21:14:36.000000 libdyson-neon-1.0.1/libdyson/cloud/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     4525 2023-05-04 21:14:36.000000 libdyson-neon-1.0.1/libdyson/const.py
--rw-r--r--   0 runner    (1001) docker     (123)     2876 2023-05-04 21:14:36.000000 libdyson-neon-1.0.1/libdyson/discovery.py
--rw-r--r--   0 runner    (1001) docker     (123)      876 2023-05-04 21:14:36.000000 libdyson-neon-1.0.1/libdyson/dyson_360_eye.py
--rw-r--r--   0 runner    (1001) docker     (123)     2153 2023-05-04 21:14:36.000000 libdyson-neon-1.0.1/libdyson/dyson_360_heurist.py
--rw-r--r--   0 runner    (1001) docker     (123)    14678 2023-05-04 21:14:36.000000 libdyson-neon-1.0.1/libdyson/dyson_device.py
--rw-r--r--   0 runner    (1001) docker     (123)     5759 2023-05-04 21:14:36.000000 libdyson-neon-1.0.1/libdyson/dyson_pure_cool.py
--rw-r--r--   0 runner    (1001) docker     (123)     2879 2023-05-04 21:14:36.000000 libdyson-neon-1.0.1/libdyson/dyson_pure_cool_link.py
--rw-r--r--   0 runner    (1001) docker     (123)      222 2023-05-04 21:14:36.000000 libdyson-neon-1.0.1/libdyson/dyson_pure_hot_cool.py
--rw-r--r--   0 runner    (1001) docker     (123)      642 2023-05-04 21:14:36.000000 libdyson-neon-1.0.1/libdyson/dyson_pure_hot_cool_link.py
--rw-r--r--   0 runner    (1001) docker     (123)     3539 2023-05-04 21:14:36.000000 libdyson-neon-1.0.1/libdyson/dyson_pure_humidify_cool.py
--rw-r--r--   0 runner    (1001) docker     (123)     2286 2023-05-04 21:14:36.000000 libdyson-neon-1.0.1/libdyson/dyson_vacuum_device.py
--rw-r--r--   0 runner    (1001) docker     (123)     1411 2023-05-04 21:14:36.000000 libdyson-neon-1.0.1/libdyson/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1652 2023-05-04 21:14:36.000000 libdyson-neon-1.0.1/libdyson/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 21:14:50.598812 libdyson-neon-1.0.1/libdyson_neon.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      966 2023-05-04 21:14:50.000000 libdyson-neon-1.0.1/libdyson_neon.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1536 2023-05-04 21:14:50.000000 libdyson-neon-1.0.1/libdyson_neon.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-04 21:14:50.000000 libdyson-neon-1.0.1/libdyson_neon.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-05-04 21:14:50.000000 libdyson-neon-1.0.1/libdyson_neon.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-05-04 21:14:50.000000 libdyson-neon-1.0.1/libdyson_neon.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2657 2023-05-04 21:14:36.000000 libdyson-neon-1.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      942 2023-05-04 21:14:50.602812 libdyson-neon-1.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      224 2023-05-04 21:14:36.000000 libdyson-neon-1.0.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 21:14:50.602812 libdyson-neon-1.0.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      192 2023-05-04 21:14:36.000000 libdyson-neon-1.0.1/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 21:14:50.602812 libdyson-neon-1.0.1/tests/cloud/
--rw-r--r--   0 runner    (1001) docker     (123)      287 2023-05-04 21:14:36.000000 libdyson-neon-1.0.1/tests/cloud/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      388 2023-05-04 21:14:36.000000 libdyson-neon-1.0.1/tests/cloud/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     1451 2023-05-04 21:14:36.000000 libdyson-neon-1.0.1/tests/cloud/mocked_requests.py
--rw-r--r--   0 runner    (1001) docker     (123)      574 2023-05-04 21:14:36.000000 libdyson-neon-1.0.1/tests/cloud/test_bearer_auth.py
--rw-r--r--   0 runner    (1001) docker     (123)     3405 2023-05-04 21:14:36.000000 libdyson-neon-1.0.1/tests/cloud/test_cloud_360_eye.py
--rw-r--r--   0 runner    (1001) docker     (123)    12226 2023-05-04 21:14:36.000000 libdyson-neon-1.0.1/tests/cloud/test_dyson_account.py
--rw-r--r--   0 runner    (1001) docker     (123)      905 2023-05-04 21:14:36.000000 libdyson-neon-1.0.1/tests/cloud/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      795 2023-05-04 21:14:36.000000 libdyson-neon-1.0.1/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     3635 2023-05-04 21:14:36.000000 libdyson-neon-1.0.1/tests/mocked_mqtt.py
--rw-r--r--   0 runner    (1001) docker     (123)     2225 2023-05-04 21:14:36.000000 libdyson-neon-1.0.1/tests/test_360_eye.py
--rw-r--r--   0 runner    (1001) docker     (123)     3389 2023-05-04 21:14:36.000000 libdyson-neon-1.0.1/tests/test_360_heurist.py
--rw-r--r--   0 runner    (1001) docker     (123)     5323 2023-05-04 21:14:36.000000 libdyson-neon-1.0.1/tests/test_device.py
--rw-r--r--   0 runner    (1001) docker     (123)     3284 2023-05-04 21:14:36.000000 libdyson-neon-1.0.1/tests/test_discovery.py
--rw-r--r--   0 runner    (1001) docker     (123)     6062 2023-05-04 21:14:36.000000 libdyson-neon-1.0.1/tests/test_fan_device.py
--rw-r--r--   0 runner    (1001) docker     (123)     2247 2023-05-04 21:14:36.000000 libdyson-neon-1.0.1/tests/test_heating_device.py
--rw-r--r--   0 runner    (1001) docker     (123)     2180 2023-05-04 21:14:36.000000 libdyson-neon-1.0.1/tests/test_init.py
--rw-r--r--   0 runner    (1001) docker     (123)     7593 2023-05-04 21:14:36.000000 libdyson-neon-1.0.1/tests/test_pure_cool.py
--rw-r--r--   0 runner    (1001) docker     (123)     1903 2023-05-04 21:14:36.000000 libdyson-neon-1.0.1/tests/test_pure_cool_formaldehyde.py
--rw-r--r--   0 runner    (1001) docker     (123)     3695 2023-05-04 21:14:36.000000 libdyson-neon-1.0.1/tests/test_pure_cool_link.py
--rw-r--r--   0 runner    (1001) docker     (123)     3076 2023-05-04 21:14:36.000000 libdyson-neon-1.0.1/tests/test_pure_cool_missing_env_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     1305 2023-05-04 21:14:36.000000 libdyson-neon-1.0.1/tests/test_pure_hot_cool_link.py
--rw-r--r--   0 runner    (1001) docker     (123)     3762 2023-05-04 21:14:36.000000 libdyson-neon-1.0.1/tests/test_pure_humidify_cool.py
--rw-r--r--   0 runner    (1001) docker     (123)     2002 2023-05-04 21:14:36.000000 libdyson-neon-1.0.1/tests/test_purifier_humidify_cool_formaldehyde.py
--rw-r--r--   0 runner    (1001) docker     (123)     1191 2023-05-04 21:14:36.000000 libdyson-neon-1.0.1/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1812 2023-05-04 21:14:36.000000 libdyson-neon-1.0.1/tests/test_vacuum.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 16:00:04.884951 libdyson-neon-1.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-05 15:59:53.000000 libdyson-neon-1.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-05-05 15:59:53.000000 libdyson-neon-1.0.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      966 2023-05-05 16:00:04.884951 libdyson-neon-1.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      404 2023-05-05 15:59:53.000000 libdyson-neon-1.0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 16:00:04.880951 libdyson-neon-1.0.2/libdyson/
+-rw-r--r--   0 runner    (1001) docker     (123)     2859 2023-05-05 15:59:53.000000 libdyson-neon-1.0.2/libdyson/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 16:00:04.880951 libdyson-neon-1.0.2/libdyson/cloud/
+-rw-r--r--   0 runner    (1001) docker     (123)      304 2023-05-05 15:59:53.000000 libdyson-neon-1.0.2/libdyson/cloud/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8064 2023-05-05 15:59:53.000000 libdyson-neon-1.0.2/libdyson/cloud/account.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2014 2023-05-05 15:59:53.000000 libdyson-neon-1.0.2/libdyson/cloud/cloud_360_eye.py
+-rw-r--r--   0 runner    (1001) docker     (123)      285 2023-05-05 15:59:53.000000 libdyson-neon-1.0.2/libdyson/cloud/cloud_device.py
+-rw-r--r--   0 runner    (1001) docker     (123)      775 2023-05-05 15:59:53.000000 libdyson-neon-1.0.2/libdyson/cloud/device_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)      990 2023-05-05 15:59:53.000000 libdyson-neon-1.0.2/libdyson/cloud/regions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1004 2023-05-05 15:59:53.000000 libdyson-neon-1.0.2/libdyson/cloud/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4525 2023-05-05 15:59:53.000000 libdyson-neon-1.0.2/libdyson/const.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2876 2023-05-05 15:59:53.000000 libdyson-neon-1.0.2/libdyson/discovery.py
+-rw-r--r--   0 runner    (1001) docker     (123)      876 2023-05-05 15:59:53.000000 libdyson-neon-1.0.2/libdyson/dyson_360_eye.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2153 2023-05-05 15:59:53.000000 libdyson-neon-1.0.2/libdyson/dyson_360_heurist.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14696 2023-05-05 15:59:53.000000 libdyson-neon-1.0.2/libdyson/dyson_device.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5759 2023-05-05 15:59:53.000000 libdyson-neon-1.0.2/libdyson/dyson_pure_cool.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2879 2023-05-05 15:59:53.000000 libdyson-neon-1.0.2/libdyson/dyson_pure_cool_link.py
+-rw-r--r--   0 runner    (1001) docker     (123)      222 2023-05-05 15:59:53.000000 libdyson-neon-1.0.2/libdyson/dyson_pure_hot_cool.py
+-rw-r--r--   0 runner    (1001) docker     (123)      642 2023-05-05 15:59:53.000000 libdyson-neon-1.0.2/libdyson/dyson_pure_hot_cool_link.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3539 2023-05-05 15:59:53.000000 libdyson-neon-1.0.2/libdyson/dyson_pure_humidify_cool.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2286 2023-05-05 15:59:53.000000 libdyson-neon-1.0.2/libdyson/dyson_vacuum_device.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1411 2023-05-05 15:59:53.000000 libdyson-neon-1.0.2/libdyson/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1652 2023-05-05 15:59:53.000000 libdyson-neon-1.0.2/libdyson/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 16:00:04.880951 libdyson-neon-1.0.2/libdyson_neon.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      966 2023-05-05 16:00:04.000000 libdyson-neon-1.0.2/libdyson_neon.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1536 2023-05-05 16:00:04.000000 libdyson-neon-1.0.2/libdyson_neon.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 16:00:04.000000 libdyson-neon-1.0.2/libdyson_neon.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-05-05 16:00:04.000000 libdyson-neon-1.0.2/libdyson_neon.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-05-05 16:00:04.000000 libdyson-neon-1.0.2/libdyson_neon.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2657 2023-05-05 15:59:53.000000 libdyson-neon-1.0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      942 2023-05-05 16:00:04.884951 libdyson-neon-1.0.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      224 2023-05-05 15:59:53.000000 libdyson-neon-1.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 16:00:04.880951 libdyson-neon-1.0.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      192 2023-05-05 15:59:53.000000 libdyson-neon-1.0.2/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 16:00:04.884951 libdyson-neon-1.0.2/tests/cloud/
+-rw-r--r--   0 runner    (1001) docker     (123)      287 2023-05-05 15:59:53.000000 libdyson-neon-1.0.2/tests/cloud/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      388 2023-05-05 15:59:53.000000 libdyson-neon-1.0.2/tests/cloud/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1451 2023-05-05 15:59:53.000000 libdyson-neon-1.0.2/tests/cloud/mocked_requests.py
+-rw-r--r--   0 runner    (1001) docker     (123)      574 2023-05-05 15:59:53.000000 libdyson-neon-1.0.2/tests/cloud/test_bearer_auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3405 2023-05-05 15:59:53.000000 libdyson-neon-1.0.2/tests/cloud/test_cloud_360_eye.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12226 2023-05-05 15:59:53.000000 libdyson-neon-1.0.2/tests/cloud/test_dyson_account.py
+-rw-r--r--   0 runner    (1001) docker     (123)      905 2023-05-05 15:59:53.000000 libdyson-neon-1.0.2/tests/cloud/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      795 2023-05-05 15:59:53.000000 libdyson-neon-1.0.2/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3635 2023-05-05 15:59:53.000000 libdyson-neon-1.0.2/tests/mocked_mqtt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2225 2023-05-05 15:59:53.000000 libdyson-neon-1.0.2/tests/test_360_eye.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3389 2023-05-05 15:59:53.000000 libdyson-neon-1.0.2/tests/test_360_heurist.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5323 2023-05-05 15:59:53.000000 libdyson-neon-1.0.2/tests/test_device.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3284 2023-05-05 15:59:53.000000 libdyson-neon-1.0.2/tests/test_discovery.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6062 2023-05-05 15:59:53.000000 libdyson-neon-1.0.2/tests/test_fan_device.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2247 2023-05-05 15:59:53.000000 libdyson-neon-1.0.2/tests/test_heating_device.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2180 2023-05-05 15:59:53.000000 libdyson-neon-1.0.2/tests/test_init.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7593 2023-05-05 15:59:53.000000 libdyson-neon-1.0.2/tests/test_pure_cool.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1906 2023-05-05 15:59:53.000000 libdyson-neon-1.0.2/tests/test_pure_cool_formaldehyde.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3695 2023-05-05 15:59:53.000000 libdyson-neon-1.0.2/tests/test_pure_cool_link.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3080 2023-05-05 15:59:53.000000 libdyson-neon-1.0.2/tests/test_pure_cool_missing_env_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1305 2023-05-05 15:59:53.000000 libdyson-neon-1.0.2/tests/test_pure_hot_cool_link.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3762 2023-05-05 15:59:53.000000 libdyson-neon-1.0.2/tests/test_pure_humidify_cool.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2004 2023-05-05 15:59:53.000000 libdyson-neon-1.0.2/tests/test_purifier_humidify_cool_formaldehyde.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1191 2023-05-05 15:59:53.000000 libdyson-neon-1.0.2/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1812 2023-05-05 15:59:53.000000 libdyson-neon-1.0.2/tests/test_vacuum.py
```

### Comparing `libdyson-neon-1.0.1/LICENSE` & `libdyson-neon-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `libdyson-neon-1.0.1/PKG-INFO` & `libdyson-neon-1.0.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: libdyson-neon
-Version: 1.0.1
+Version: 1.0.2
 Summary: A Python library for Dyson devices.
 Home-page: https://github.com/libdyson-wg/libdyson-neon
 Author: The libdyson Working Group
 Author-email: dotvezz@gmail.com
 License: MIT License
 Description: # Dyson Python Library
```

### Comparing `libdyson-neon-1.0.1/libdyson/__init__.py` & `libdyson-neon-1.0.2/libdyson/__init__.py`

 * *Files identical despite different names*

### Comparing `libdyson-neon-1.0.1/libdyson/cloud/account.py` & `libdyson-neon-1.0.2/libdyson/cloud/account.py`

 * *Files identical despite different names*

### Comparing `libdyson-neon-1.0.1/libdyson/cloud/cloud_360_eye.py` & `libdyson-neon-1.0.2/libdyson/cloud/cloud_360_eye.py`

 * *Files identical despite different names*

### Comparing `libdyson-neon-1.0.1/libdyson/cloud/device_info.py` & `libdyson-neon-1.0.2/libdyson/cloud/device_info.py`

 * *Files identical despite different names*

### Comparing `libdyson-neon-1.0.1/libdyson/cloud/regions.py` & `libdyson-neon-1.0.2/libdyson/cloud/regions.py`

 * *Files identical despite different names*

### Comparing `libdyson-neon-1.0.1/libdyson/cloud/utils.py` & `libdyson-neon-1.0.2/libdyson/cloud/utils.py`

 * *Files identical despite different names*

### Comparing `libdyson-neon-1.0.1/libdyson/const.py` & `libdyson-neon-1.0.2/libdyson/const.py`

 * *Files identical despite different names*

### Comparing `libdyson-neon-1.0.1/libdyson/discovery.py` & `libdyson-neon-1.0.2/libdyson/discovery.py`

 * *Files identical despite different names*

### Comparing `libdyson-neon-1.0.1/libdyson/dyson_360_eye.py` & `libdyson-neon-1.0.2/libdyson/dyson_360_eye.py`

 * *Files identical despite different names*

### Comparing `libdyson-neon-1.0.1/libdyson/dyson_360_heurist.py` & `libdyson-neon-1.0.2/libdyson/dyson_360_heurist.py`

 * *Files identical despite different names*

### Comparing `libdyson-neon-1.0.1/libdyson/dyson_device.py` & `libdyson-neon-1.0.2/libdyson/dyson_device.py`

 * *Files 0% similar despite different names*

```diff
@@ -290,15 +290,15 @@
         try:
             return  state[field][1] if isinstance(state[field], list) else state[field]
         except:
             return None
 
     def _get_environmental_field_value(self, field, divisor=1) -> Optional[Union[int, float]]:
         value = self._get_field_value(self._environmental_data, field)
-        if value == "OFF":
+        if value == "OFF" or value == "off":
             return ENVIRONMENTAL_OFF
         if value == "INIT":
             return ENVIRONMENTAL_INIT
         if value == "FAIL":
             return ENVIRONMENTAL_FAIL
         if value == "NONE" or value is None:
             return None
```

### Comparing `libdyson-neon-1.0.1/libdyson/dyson_pure_cool.py` & `libdyson-neon-1.0.2/libdyson/dyson_pure_cool.py`

 * *Files identical despite different names*

### Comparing `libdyson-neon-1.0.1/libdyson/dyson_pure_cool_link.py` & `libdyson-neon-1.0.2/libdyson/dyson_pure_cool_link.py`

 * *Files identical despite different names*

### Comparing `libdyson-neon-1.0.1/libdyson/dyson_pure_hot_cool_link.py` & `libdyson-neon-1.0.2/libdyson/dyson_pure_hot_cool_link.py`

 * *Files identical despite different names*

### Comparing `libdyson-neon-1.0.1/libdyson/dyson_pure_humidify_cool.py` & `libdyson-neon-1.0.2/libdyson/dyson_pure_humidify_cool.py`

 * *Files identical despite different names*

### Comparing `libdyson-neon-1.0.1/libdyson/dyson_vacuum_device.py` & `libdyson-neon-1.0.2/libdyson/dyson_vacuum_device.py`

 * *Files identical despite different names*

### Comparing `libdyson-neon-1.0.1/libdyson/exceptions.py` & `libdyson-neon-1.0.2/libdyson/exceptions.py`

 * *Files identical despite different names*

### Comparing `libdyson-neon-1.0.1/libdyson/utils.py` & `libdyson-neon-1.0.2/libdyson/utils.py`

 * *Files identical despite different names*

### Comparing `libdyson-neon-1.0.1/libdyson_neon.egg-info/PKG-INFO` & `libdyson-neon-1.0.2/libdyson_neon.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: libdyson-neon
-Version: 1.0.1
+Version: 1.0.2
 Summary: A Python library for Dyson devices.
 Home-page: https://github.com/libdyson-wg/libdyson-neon
 Author: The libdyson Working Group
 Author-email: dotvezz@gmail.com
 License: MIT License
 Description: # Dyson Python Library
```

### Comparing `libdyson-neon-1.0.1/libdyson_neon.egg-info/SOURCES.txt` & `libdyson-neon-1.0.2/libdyson_neon.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `libdyson-neon-1.0.1/pyproject.toml` & `libdyson-neon-1.0.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `libdyson-neon-1.0.1/setup.cfg` & `libdyson-neon-1.0.2/setup.cfg`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = libdyson-neon
-version = 1.0.1
+version = 1.0.2
 author = The libdyson Working Group
 author_email = dotvezz@gmail.com
 license = MIT License
 license_file = LICENSE
 platforms = any
 description = A Python library for Dyson devices.
 long_description = file: README.md
```

### Comparing `libdyson-neon-1.0.1/tests/cloud/mocked_requests.py` & `libdyson-neon-1.0.2/tests/cloud/mocked_requests.py`

 * *Files identical despite different names*

### Comparing `libdyson-neon-1.0.1/tests/cloud/test_bearer_auth.py` & `libdyson-neon-1.0.2/tests/cloud/test_bearer_auth.py`

 * *Files identical despite different names*

### Comparing `libdyson-neon-1.0.1/tests/cloud/test_cloud_360_eye.py` & `libdyson-neon-1.0.2/tests/cloud/test_cloud_360_eye.py`

 * *Files identical despite different names*

### Comparing `libdyson-neon-1.0.1/tests/cloud/test_dyson_account.py` & `libdyson-neon-1.0.2/tests/cloud/test_dyson_account.py`

 * *Files identical despite different names*

### Comparing `libdyson-neon-1.0.1/tests/cloud/utils.py` & `libdyson-neon-1.0.2/tests/cloud/utils.py`

 * *Files identical despite different names*

### Comparing `libdyson-neon-1.0.1/tests/conftest.py` & `libdyson-neon-1.0.2/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `libdyson-neon-1.0.1/tests/mocked_mqtt.py` & `libdyson-neon-1.0.2/tests/mocked_mqtt.py`

 * *Files identical despite different names*

### Comparing `libdyson-neon-1.0.1/tests/test_360_eye.py` & `libdyson-neon-1.0.2/tests/test_360_eye.py`

 * *Files identical despite different names*

### Comparing `libdyson-neon-1.0.1/tests/test_360_heurist.py` & `libdyson-neon-1.0.2/tests/test_360_heurist.py`

 * *Files identical despite different names*

### Comparing `libdyson-neon-1.0.1/tests/test_device.py` & `libdyson-neon-1.0.2/tests/test_device.py`

 * *Files identical despite different names*

### Comparing `libdyson-neon-1.0.1/tests/test_discovery.py` & `libdyson-neon-1.0.2/tests/test_discovery.py`

 * *Files identical despite different names*

### Comparing `libdyson-neon-1.0.1/tests/test_fan_device.py` & `libdyson-neon-1.0.2/tests/test_fan_device.py`

 * *Files identical despite different names*

### Comparing `libdyson-neon-1.0.1/tests/test_heating_device.py` & `libdyson-neon-1.0.2/tests/test_heating_device.py`

 * *Files identical despite different names*

### Comparing `libdyson-neon-1.0.1/tests/test_init.py` & `libdyson-neon-1.0.2/tests/test_init.py`

 * *Files identical despite different names*

### Comparing `libdyson-neon-1.0.1/tests/test_pure_cool.py` & `libdyson-neon-1.0.2/tests/test_pure_cool.py`

 * *Files identical despite different names*

### Comparing `libdyson-neon-1.0.1/tests/test_pure_cool_formaldehyde.py` & `libdyson-neon-1.0.2/tests/test_pure_cool_formaldehyde.py`

 * *Files 1% similar despite different names*

```diff
@@ -60,10 +60,10 @@
             "hcho": "0001",
             "hchr": "0002",
         }
     }
     device.request_environmental_data()
     assert device.particulate_matter_2_5 == 9
     assert device.particulate_matter_10 == 5
-    assert device.volatile_organic_compounds == 4
-    assert device.nitrogen_dioxide == 11
+    assert device.volatile_organic_compounds == 0.4
+    assert device.nitrogen_dioxide == 1.1
     assert device.formaldehyde == 1
```

### Comparing `libdyson-neon-1.0.1/tests/test_pure_cool_link.py` & `libdyson-neon-1.0.2/tests/test_pure_cool_link.py`

 * *Files identical despite different names*

### Comparing `libdyson-neon-1.0.1/tests/test_pure_cool_missing_env_data.py` & `libdyson-neon-1.0.2/tests/test_pure_cool_missing_env_data.py`

 * *Files 1% similar despite different names*

```diff
@@ -60,16 +60,16 @@
             "hcho": "NONE",
             "hchr": "0002",
         }
     }
     device.request_environmental_data()
     assert device.particulate_matter_2_5 == 9
     assert device.particulate_matter_10 == 5
-    assert device.volatile_organic_compounds == 4
-    assert device.nitrogen_dioxide == 11
+    assert device.volatile_organic_compounds == .4
+    assert device.nitrogen_dioxide == 1.1
     assert device.formaldehyde is None
 
 
 def test_missing_data(mqtt_client: MockedMQTT):
     """Test properties of a case where (hcho in this case) data is missing for some reason."""
     device = DysonPureCool(SERIAL, CREDENTIAL, DEVICE_TYPE)
     device.connect(HOST)
@@ -94,10 +94,10 @@
             "sltm": "OFF",
             "hchr": "0002",
         }
     }
     device.request_environmental_data()
     assert device.particulate_matter_2_5 == 9
     assert device.particulate_matter_10 == 5
-    assert device.volatile_organic_compounds == 4
-    assert device.nitrogen_dioxide == 11
+    assert device.volatile_organic_compounds == .4
+    assert device.nitrogen_dioxide == 1.1
     assert device.formaldehyde is None
```

### Comparing `libdyson-neon-1.0.1/tests/test_pure_hot_cool_link.py` & `libdyson-neon-1.0.2/tests/test_pure_hot_cool_link.py`

 * *Files identical despite different names*

### Comparing `libdyson-neon-1.0.1/tests/test_pure_humidify_cool.py` & `libdyson-neon-1.0.2/tests/test_pure_humidify_cool.py`

 * *Files identical despite different names*

### Comparing `libdyson-neon-1.0.1/tests/test_purifier_humidify_cool_formaldehyde.py` & `libdyson-neon-1.0.2/tests/test_purifier_humidify_cool_formaldehyde.py`

 * *Files 1% similar despite different names*

```diff
@@ -60,10 +60,10 @@
             "hcho": "0001",
             "hchr": "0002",
         }
     }
     device.request_environmental_data()
     assert device.particulate_matter_2_5 == 9
     assert device.particulate_matter_10 == 5
-    assert device.volatile_organic_compounds == 4
-    assert device.nitrogen_dioxide == 11
+    assert device.volatile_organic_compounds == .4
+    assert device.nitrogen_dioxide == 1.1
     assert device.formaldehyde == 1
```

### Comparing `libdyson-neon-1.0.1/tests/test_utils.py` & `libdyson-neon-1.0.2/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `libdyson-neon-1.0.1/tests/test_vacuum.py` & `libdyson-neon-1.0.2/tests/test_vacuum.py`

 * *Files identical despite different names*

