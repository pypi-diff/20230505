# Comparing `tmp/astrohack-0.1.0.tar.gz` & `tmp/astrohack-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "astrohack-0.1.0.tar", last modified: Fri Apr 28 22:53:21 2023, max compression
+gzip compressed data, was "astrohack-0.1.1.tar", last modified: Fri May  5 20:40:13 2023, max compression
```

## Comparing `astrohack-0.1.0.tar` & `astrohack-0.1.1.tar`

### file list

```diff
@@ -1,96 +1,98 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 22:53:21.349583 astrohack-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-04-28 22:53:01.000000 astrohack-0.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-28 22:53:01.000000 astrohack-0.1.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2081 2023-04-28 22:53:21.349583 astrohack-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1737 2023-04-28 22:53:01.000000 astrohack-0.1.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 22:53:01.000000 astrohack-0.1.0/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1171 2023-04-28 22:53:01.000000 astrohack-0.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-28 22:53:21.349583 astrohack-0.1.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 22:53:21.329583 astrohack-0.1.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 22:53:21.333583 astrohack-0.1.0/src/astrohack/
--rw-r--r--   0 runner    (1001) docker     (123)      174 2023-04-28 22:53:01.000000 astrohack-0.1.0/src/astrohack/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 22:53:21.337583 astrohack-0.1.0/src/astrohack/_classes/
--rw-r--r--   0 runner    (1001) docker     (123)    27827 2023-04-28 22:53:01.000000 astrohack-0.1.0/src/astrohack/_classes/antenna_surface.py
--rw-r--r--   0 runner    (1001) docker     (123)    19699 2023-04-28 22:53:01.000000 astrohack-0.1.0/src/astrohack/_classes/base_panel.py
--rw-r--r--   0 runner    (1001) docker     (123)     2792 2023-04-28 22:53:01.000000 astrohack-0.1.0/src/astrohack/_classes/polygon_panel.py
--rw-r--r--   0 runner    (1001) docker     (123)     6291 2023-04-28 22:53:01.000000 astrohack-0.1.0/src/astrohack/_classes/ring_panel.py
--rw-r--r--   0 runner    (1001) docker     (123)     3452 2023-04-28 22:53:01.000000 astrohack-0.1.0/src/astrohack/_classes/telescope.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 22:53:21.337583 astrohack-0.1.0/src/astrohack/_utils/
--rw-r--r--   0 runner    (1001) docker     (123)      167 2023-04-28 22:53:01.000000 astrohack-0.1.0/src/astrohack/_utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10491 2023-04-28 22:53:01.000000 astrohack-0.1.0/src/astrohack/_utils/_algorithms.py
--rw-r--r--   0 runner    (1001) docker     (123)     1058 2023-04-28 22:53:01.000000 astrohack-0.1.0/src/astrohack/_utils/_constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     2834 2023-04-28 22:53:01.000000 astrohack-0.1.0/src/astrohack/_utils/_conversion.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 22:53:21.341583 astrohack-0.1.0/src/astrohack/_utils/_dask_plugins/
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-04-28 22:53:01.000000 astrohack-0.1.0/src/astrohack/_utils/_dask_plugins/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8071 2023-04-28 22:53:01.000000 astrohack-0.1.0/src/astrohack/_utils/_dask_plugins/_astrohack_scheduler.py
--rw-r--r--   0 runner    (1001) docker     (123)     2284 2023-04-28 22:53:01.000000 astrohack-0.1.0/src/astrohack/_utils/_dask_plugins/_astrohack_worker.py
--rw-r--r--   0 runner    (1001) docker     (123)    10590 2023-04-28 22:53:01.000000 astrohack-0.1.0/src/astrohack/_utils/_dio.py
--rw-r--r--   0 runner    (1001) docker     (123)    21572 2023-04-28 22:53:01.000000 astrohack-0.1.0/src/astrohack/_utils/_extract_holog.py
--rw-r--r--   0 runner    (1001) docker     (123)    12058 2023-04-28 22:53:01.000000 astrohack-0.1.0/src/astrohack/_utils/_extract_point.py
--rw-r--r--   0 runner    (1001) docker     (123)    12038 2023-04-28 22:53:01.000000 astrohack-0.1.0/src/astrohack/_utils/_holog.py
--rw-r--r--   0 runner    (1001) docker     (123)     6424 2023-04-28 22:53:01.000000 astrohack-0.1.0/src/astrohack/_utils/_imaging.py
--rw-r--r--   0 runner    (1001) docker     (123)    14344 2023-04-28 22:53:01.000000 astrohack-0.1.0/src/astrohack/_utils/_io.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 22:53:21.341583 astrohack-0.1.0/src/astrohack/_utils/_logger/
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-04-28 22:53:01.000000 astrohack-0.1.0/src/astrohack/_utils/_logger/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     5462 2023-04-28 22:53:01.000000 astrohack-0.1.0/src/astrohack/_utils/_logger/_astrohack_logger.py
--rw-r--r--   0 runner    (1001) docker     (123)    30815 2023-04-28 22:53:01.000000 astrohack-0.1.0/src/astrohack/_utils/_panel.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 22:53:21.341583 astrohack-0.1.0/src/astrohack/_utils/_parm_utils/
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-04-28 22:53:01.000000 astrohack-0.1.0/src/astrohack/_utils/_parm_utils/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2158 2023-04-28 22:53:01.000000 astrohack-0.1.0/src/astrohack/_utils/_parm_utils/_check_logger_parms.py
--rw-r--r--   0 runner    (1001) docker     (123)     5993 2023-04-28 22:53:01.000000 astrohack-0.1.0/src/astrohack/_utils/_parm_utils/_check_parms.py
--rw-r--r--   0 runner    (1001) docker     (123)      365 2023-04-28 22:53:01.000000 astrohack-0.1.0/src/astrohack/_utils/_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    25433 2023-04-28 22:53:01.000000 astrohack-0.1.0/src/astrohack/_utils/gaussfitter.py
--rw-r--r--   0 runner    (1001) docker     (123)     6379 2023-04-28 22:53:01.000000 astrohack-0.1.0/src/astrohack/astrohack_client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 22:53:21.329583 astrohack-0.1.0/src/astrohack/data/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 22:53:21.341583 astrohack-0.1.0/src/astrohack/data/.file_meta_data/
--rw-r--r--   0 runner    (1001) docker     (123)      537 2023-04-28 22:53:01.000000 astrohack-0.1.0/src/astrohack/data/.file_meta_data/ea25_cal_small_spw1_4_60_ea04_after.json
--rw-r--r--   0 runner    (1001) docker     (123)      667 2023-04-28 22:53:01.000000 astrohack-0.1.0/src/astrohack/data/.file_meta_data/ea25_cal_small_spw1_4_60_ea04_after_fixed.json
--rw-r--r--   0 runner    (1001) docker     (123)      512 2023-04-28 22:53:01.000000 astrohack-0.1.0/src/astrohack/data/.file_meta_data/ea25_cal_small_spw1_4_60_ea04_before.json
--rw-r--r--   0 runner    (1001) docker     (123)      641 2023-04-28 22:53:01.000000 astrohack-0.1.0/src/astrohack/data/.file_meta_data/ea25_cal_small_spw1_4_60_ea04_before_fixed.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 22:53:21.341583 astrohack-0.1.0/src/astrohack/data/telescopes/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 22:53:01.000000 astrohack-0.1.0/src/astrohack/data/telescopes/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 22:53:21.341583 astrohack-0.1.0/src/astrohack/data/telescopes/aca_7m.zarr/
--rw-r--r--   0 runner    (1001) docker     (123)     1036 2023-04-28 22:53:01.000000 astrohack-0.1.0/src/astrohack/data/telescopes/aca_7m.zarr/.zattrs
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-04-28 22:53:01.000000 astrohack-0.1.0/src/astrohack/data/telescopes/aca_7m.zarr/.zgroup
--rw-r--r--   0 runner    (1001) docker     (123)     1523 2023-04-28 22:53:01.000000 astrohack-0.1.0/src/astrohack/data/telescopes/aca_7m.zarr/.zmetadata
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 22:53:21.341583 astrohack-0.1.0/src/astrohack/data/telescopes/alma_da.zarr/
--rw-r--r--   0 runner    (1001) docker     (123)     1168 2023-04-28 22:53:01.000000 astrohack-0.1.0/src/astrohack/data/telescopes/alma_da.zarr/.zattrs
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-04-28 22:53:01.000000 astrohack-0.1.0/src/astrohack/data/telescopes/alma_da.zarr/.zgroup
--rw-r--r--   0 runner    (1001) docker     (123)     1655 2023-04-28 22:53:01.000000 astrohack-0.1.0/src/astrohack/data/telescopes/alma_da.zarr/.zmetadata
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 22:53:21.345583 astrohack-0.1.0/src/astrohack/data/telescopes/alma_dv.zarr/
--rw-r--r--   0 runner    (1001) docker     (123)     1282 2023-04-28 22:53:01.000000 astrohack-0.1.0/src/astrohack/data/telescopes/alma_dv.zarr/.zattrs
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-04-28 22:53:01.000000 astrohack-0.1.0/src/astrohack/data/telescopes/alma_dv.zarr/.zgroup
--rw-r--r--   0 runner    (1001) docker     (123)     1841 2023-04-28 22:53:01.000000 astrohack-0.1.0/src/astrohack/data/telescopes/alma_dv.zarr/.zmetadata
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 22:53:21.345583 astrohack-0.1.0/src/astrohack/data/telescopes/alma_tp.zarr/
--rw-r--r--   0 runner    (1001) docker     (123)     1286 2023-04-28 22:53:01.000000 astrohack-0.1.0/src/astrohack/data/telescopes/alma_tp.zarr/.zattrs
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-04-28 22:53:01.000000 astrohack-0.1.0/src/astrohack/data/telescopes/alma_tp.zarr/.zgroup
--rw-r--r--   0 runner    (1001) docker     (123)     1821 2023-04-28 22:53:01.000000 astrohack-0.1.0/src/astrohack/data/telescopes/alma_tp.zarr/.zmetadata
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 22:53:21.345583 astrohack-0.1.0/src/astrohack/data/telescopes/vla.zarr/
--rw-r--r--   0 runner    (1001) docker     (123)      858 2023-04-28 22:53:01.000000 astrohack-0.1.0/src/astrohack/data/telescopes/vla.zarr/.zattrs
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-04-28 22:53:01.000000 astrohack-0.1.0/src/astrohack/data/telescopes/vla.zarr/.zgroup
--rw-r--r--   0 runner    (1001) docker     (123)     1361 2023-04-28 22:53:01.000000 astrohack-0.1.0/src/astrohack/data/telescopes/vla.zarr/.zmetadata
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 22:53:21.345583 astrohack-0.1.0/src/astrohack/data/telescopes/vlba.zarr/
--rw-r--r--   0 runner    (1001) docker     (123)      863 2023-04-28 22:53:01.000000 astrohack-0.1.0/src/astrohack/data/telescopes/vlba.zarr/.zattrs
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-04-28 22:53:01.000000 astrohack-0.1.0/src/astrohack/data/telescopes/vlba.zarr/.zgroup
--rw-r--r--   0 runner    (1001) docker     (123)     1366 2023-04-28 22:53:01.000000 astrohack-0.1.0/src/astrohack/data/telescopes/vlba.zarr/.zmetadata
--rw-r--r--   0 runner    (1001) docker     (123)    14304 2023-04-28 22:53:01.000000 astrohack-0.1.0/src/astrohack/dio.py
--rw-r--r--   0 runner    (1001) docker     (123)    19785 2023-04-28 22:53:01.000000 astrohack-0.1.0/src/astrohack/extract_holog.py
--rw-r--r--   0 runner    (1001) docker     (123)     2535 2023-04-28 22:53:01.000000 astrohack-0.1.0/src/astrohack/gdown_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    12068 2023-04-28 22:53:01.000000 astrohack-0.1.0/src/astrohack/holog.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 22:53:01.000000 astrohack-0.1.0/src/astrohack/locit.py
--rw-r--r--   0 runner    (1001) docker     (123)    10840 2023-04-28 22:53:01.000000 astrohack-0.1.0/src/astrohack/panel.py
--rw-r--r--   0 runner    (1001) docker     (123)     1091 2023-04-28 22:53:01.000000 astrohack-0.1.0/src/astrohack/profiling.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 22:53:21.345583 astrohack-0.1.0/src/astrohack/visualization/
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-04-28 22:53:01.000000 astrohack-0.1.0/src/astrohack/visualization/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5201 2023-04-28 22:53:01.000000 astrohack-0.1.0/src/astrohack/visualization/viewer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 22:53:21.333583 astrohack-0.1.0/src/astrohack.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2081 2023-04-28 22:53:21.000000 astrohack-0.1.0/src/astrohack.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2986 2023-04-28 22:53:21.000000 astrohack-0.1.0/src/astrohack.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-28 22:53:21.000000 astrohack-0.1.0/src/astrohack.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      574 2023-04-28 22:53:21.000000 astrohack-0.1.0/src/astrohack.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-28 22:53:21.000000 astrohack-0.1.0/src/astrohack.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 22:53:21.345583 astrohack-0.1.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     5577 2023-04-28 22:53:01.000000 astrohack-0.1.0/tests/test_class_antenna_surface.py
--rw-r--r--   0 runner    (1001) docker     (123)    19791 2023-04-28 22:53:01.000000 astrohack-0.1.0/tests/test_class_base_panel.py
--rw-r--r--   0 runner    (1001) docker     (123)     3783 2023-04-28 22:53:01.000000 astrohack-0.1.0/tests/test_class_ring_panel.py
--rw-r--r--   0 runner    (1001) docker     (123)     2720 2023-04-28 22:53:01.000000 astrohack-0.1.0/tests/test_class_telescope.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 20:40:13.371443 astrohack-0.1.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-05-05 20:39:54.000000 astrohack-0.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-05 20:39:54.000000 astrohack-0.1.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2081 2023-05-05 20:40:13.371443 astrohack-0.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1737 2023-05-05 20:39:54.000000 astrohack-0.1.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 20:39:54.000000 astrohack-0.1.1/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1171 2023-05-05 20:39:54.000000 astrohack-0.1.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-05 20:40:13.371443 astrohack-0.1.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 20:40:13.359443 astrohack-0.1.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 20:40:13.363443 astrohack-0.1.1/src/astrohack/
+-rw-r--r--   0 runner    (1001) docker     (123)      174 2023-05-05 20:39:54.000000 astrohack-0.1.1/src/astrohack/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 20:40:13.363443 astrohack-0.1.1/src/astrohack/_classes/
+-rw-r--r--   0 runner    (1001) docker     (123)    30781 2023-05-05 20:39:54.000000 astrohack-0.1.1/src/astrohack/_classes/antenna_surface.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20815 2023-05-05 20:39:54.000000 astrohack-0.1.1/src/astrohack/_classes/base_panel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2792 2023-05-05 20:39:54.000000 astrohack-0.1.1/src/astrohack/_classes/polygon_panel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6439 2023-05-05 20:39:54.000000 astrohack-0.1.1/src/astrohack/_classes/ring_panel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3452 2023-05-05 20:39:54.000000 astrohack-0.1.1/src/astrohack/_classes/telescope.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 20:40:13.367443 astrohack-0.1.1/src/astrohack/_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      167 2023-05-05 20:39:54.000000 astrohack-0.1.1/src/astrohack/_utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10491 2023-05-05 20:39:54.000000 astrohack-0.1.1/src/astrohack/_utils/_algorithms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4256 2023-05-05 20:39:54.000000 astrohack-0.1.1/src/astrohack/_utils/_combine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-05-05 20:39:54.000000 astrohack-0.1.1/src/astrohack/_utils/_constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2834 2023-05-05 20:39:54.000000 astrohack-0.1.1/src/astrohack/_utils/_conversion.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 20:40:13.367443 astrohack-0.1.1/src/astrohack/_utils/_dask_plugins/
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-05-05 20:39:54.000000 astrohack-0.1.1/src/astrohack/_utils/_dask_plugins/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8071 2023-05-05 20:39:54.000000 astrohack-0.1.1/src/astrohack/_utils/_dask_plugins/_astrohack_scheduler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2284 2023-05-05 20:39:54.000000 astrohack-0.1.1/src/astrohack/_utils/_dask_plugins/_astrohack_worker.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10590 2023-05-05 20:39:54.000000 astrohack-0.1.1/src/astrohack/_utils/_dio.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21572 2023-05-05 20:39:54.000000 astrohack-0.1.1/src/astrohack/_utils/_extract_holog.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12058 2023-05-05 20:39:54.000000 astrohack-0.1.1/src/astrohack/_utils/_extract_point.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11880 2023-05-05 20:39:54.000000 astrohack-0.1.1/src/astrohack/_utils/_holog.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6424 2023-05-05 20:39:54.000000 astrohack-0.1.1/src/astrohack/_utils/_imaging.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14344 2023-05-05 20:39:54.000000 astrohack-0.1.1/src/astrohack/_utils/_io.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 20:40:13.367443 astrohack-0.1.1/src/astrohack/_utils/_logger/
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-05-05 20:39:54.000000 astrohack-0.1.1/src/astrohack/_utils/_logger/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     5462 2023-05-05 20:39:54.000000 astrohack-0.1.1/src/astrohack/_utils/_logger/_astrohack_logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31185 2023-05-05 20:39:54.000000 astrohack-0.1.1/src/astrohack/_utils/_panel.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 20:40:13.367443 astrohack-0.1.1/src/astrohack/_utils/_parm_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-05-05 20:39:54.000000 astrohack-0.1.1/src/astrohack/_utils/_parm_utils/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2158 2023-05-05 20:39:54.000000 astrohack-0.1.1/src/astrohack/_utils/_parm_utils/_check_logger_parms.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5993 2023-05-05 20:39:54.000000 astrohack-0.1.1/src/astrohack/_utils/_parm_utils/_check_parms.py
+-rw-r--r--   0 runner    (1001) docker     (123)      502 2023-05-05 20:39:54.000000 astrohack-0.1.1/src/astrohack/_utils/_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25433 2023-05-05 20:39:54.000000 astrohack-0.1.1/src/astrohack/_utils/gaussfitter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6379 2023-05-05 20:39:54.000000 astrohack-0.1.1/src/astrohack/astrohack_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4995 2023-05-05 20:39:54.000000 astrohack-0.1.1/src/astrohack/combine.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 20:40:13.359443 astrohack-0.1.1/src/astrohack/data/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 20:40:13.367443 astrohack-0.1.1/src/astrohack/data/.file_meta_data/
+-rw-r--r--   0 runner    (1001) docker     (123)      537 2023-05-05 20:39:54.000000 astrohack-0.1.1/src/astrohack/data/.file_meta_data/ea25_cal_small_spw1_4_60_ea04_after.json
+-rw-r--r--   0 runner    (1001) docker     (123)      667 2023-05-05 20:39:54.000000 astrohack-0.1.1/src/astrohack/data/.file_meta_data/ea25_cal_small_spw1_4_60_ea04_after_fixed.json
+-rw-r--r--   0 runner    (1001) docker     (123)      512 2023-05-05 20:39:54.000000 astrohack-0.1.1/src/astrohack/data/.file_meta_data/ea25_cal_small_spw1_4_60_ea04_before.json
+-rw-r--r--   0 runner    (1001) docker     (123)      641 2023-05-05 20:39:54.000000 astrohack-0.1.1/src/astrohack/data/.file_meta_data/ea25_cal_small_spw1_4_60_ea04_before_fixed.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 20:40:13.367443 astrohack-0.1.1/src/astrohack/data/telescopes/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 20:39:54.000000 astrohack-0.1.1/src/astrohack/data/telescopes/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 20:40:13.367443 astrohack-0.1.1/src/astrohack/data/telescopes/aca_7m.zarr/
+-rw-r--r--   0 runner    (1001) docker     (123)     1036 2023-05-05 20:39:54.000000 astrohack-0.1.1/src/astrohack/data/telescopes/aca_7m.zarr/.zattrs
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-05-05 20:39:54.000000 astrohack-0.1.1/src/astrohack/data/telescopes/aca_7m.zarr/.zgroup
+-rw-r--r--   0 runner    (1001) docker     (123)     1523 2023-05-05 20:39:54.000000 astrohack-0.1.1/src/astrohack/data/telescopes/aca_7m.zarr/.zmetadata
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 20:40:13.367443 astrohack-0.1.1/src/astrohack/data/telescopes/alma_da.zarr/
+-rw-r--r--   0 runner    (1001) docker     (123)     1168 2023-05-05 20:39:54.000000 astrohack-0.1.1/src/astrohack/data/telescopes/alma_da.zarr/.zattrs
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-05-05 20:39:54.000000 astrohack-0.1.1/src/astrohack/data/telescopes/alma_da.zarr/.zgroup
+-rw-r--r--   0 runner    (1001) docker     (123)     1655 2023-05-05 20:39:54.000000 astrohack-0.1.1/src/astrohack/data/telescopes/alma_da.zarr/.zmetadata
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 20:40:13.367443 astrohack-0.1.1/src/astrohack/data/telescopes/alma_dv.zarr/
+-rw-r--r--   0 runner    (1001) docker     (123)     1282 2023-05-05 20:39:54.000000 astrohack-0.1.1/src/astrohack/data/telescopes/alma_dv.zarr/.zattrs
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-05-05 20:39:54.000000 astrohack-0.1.1/src/astrohack/data/telescopes/alma_dv.zarr/.zgroup
+-rw-r--r--   0 runner    (1001) docker     (123)     1841 2023-05-05 20:39:54.000000 astrohack-0.1.1/src/astrohack/data/telescopes/alma_dv.zarr/.zmetadata
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 20:40:13.367443 astrohack-0.1.1/src/astrohack/data/telescopes/alma_tp.zarr/
+-rw-r--r--   0 runner    (1001) docker     (123)     1286 2023-05-05 20:39:54.000000 astrohack-0.1.1/src/astrohack/data/telescopes/alma_tp.zarr/.zattrs
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-05-05 20:39:54.000000 astrohack-0.1.1/src/astrohack/data/telescopes/alma_tp.zarr/.zgroup
+-rw-r--r--   0 runner    (1001) docker     (123)     1821 2023-05-05 20:39:54.000000 astrohack-0.1.1/src/astrohack/data/telescopes/alma_tp.zarr/.zmetadata
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 20:40:13.367443 astrohack-0.1.1/src/astrohack/data/telescopes/vla.zarr/
+-rw-r--r--   0 runner    (1001) docker     (123)      858 2023-05-05 20:39:54.000000 astrohack-0.1.1/src/astrohack/data/telescopes/vla.zarr/.zattrs
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-05-05 20:39:54.000000 astrohack-0.1.1/src/astrohack/data/telescopes/vla.zarr/.zgroup
+-rw-r--r--   0 runner    (1001) docker     (123)     1361 2023-05-05 20:39:54.000000 astrohack-0.1.1/src/astrohack/data/telescopes/vla.zarr/.zmetadata
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 20:40:13.371443 astrohack-0.1.1/src/astrohack/data/telescopes/vlba.zarr/
+-rw-r--r--   0 runner    (1001) docker     (123)      863 2023-05-05 20:39:54.000000 astrohack-0.1.1/src/astrohack/data/telescopes/vlba.zarr/.zattrs
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-05-05 20:39:54.000000 astrohack-0.1.1/src/astrohack/data/telescopes/vlba.zarr/.zgroup
+-rw-r--r--   0 runner    (1001) docker     (123)     1366 2023-05-05 20:39:54.000000 astrohack-0.1.1/src/astrohack/data/telescopes/vlba.zarr/.zmetadata
+-rw-r--r--   0 runner    (1001) docker     (123)    16694 2023-05-05 20:39:54.000000 astrohack-0.1.1/src/astrohack/dio.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19791 2023-05-05 20:39:54.000000 astrohack-0.1.1/src/astrohack/extract_holog.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2535 2023-05-05 20:39:54.000000 astrohack-0.1.1/src/astrohack/gdown_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11120 2023-05-05 20:39:54.000000 astrohack-0.1.1/src/astrohack/holog.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 20:39:54.000000 astrohack-0.1.1/src/astrohack/locit.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10898 2023-05-05 20:39:54.000000 astrohack-0.1.1/src/astrohack/panel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1091 2023-05-05 20:39:54.000000 astrohack-0.1.1/src/astrohack/profiling.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 20:40:13.371443 astrohack-0.1.1/src/astrohack/visualization/
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-05 20:39:54.000000 astrohack-0.1.1/src/astrohack/visualization/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5201 2023-05-05 20:39:54.000000 astrohack-0.1.1/src/astrohack/visualization/viewer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 20:40:13.363443 astrohack-0.1.1/src/astrohack.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2081 2023-05-05 20:40:13.000000 astrohack-0.1.1/src/astrohack.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3044 2023-05-05 20:40:13.000000 astrohack-0.1.1/src/astrohack.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 20:40:13.000000 astrohack-0.1.1/src/astrohack.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      574 2023-05-05 20:40:13.000000 astrohack-0.1.1/src/astrohack.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-05 20:40:13.000000 astrohack-0.1.1/src/astrohack.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 20:40:13.371443 astrohack-0.1.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     5577 2023-05-05 20:39:54.000000 astrohack-0.1.1/tests/test_class_antenna_surface.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19937 2023-05-05 20:39:54.000000 astrohack-0.1.1/tests/test_class_base_panel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3783 2023-05-05 20:39:54.000000 astrohack-0.1.1/tests/test_class_ring_panel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2720 2023-05-05 20:39:54.000000 astrohack-0.1.1/tests/test_class_telescope.py
```

### Comparing `astrohack-0.1.0/LICENSE` & `astrohack-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `astrohack-0.1.0/PKG-INFO` & `astrohack-0.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: astrohack
-Version: 0.1.0
+Version: 0.1.1
 Summary: Holography Antenna Commissioning Kit
 Author-email: Jan-Willem Steeb <jsteeb@nrao.edu>, Joshua Hoskins <jhoskins@nrao.edu>, Victor de Souza Magalhaes <vdesouza@nrao.edu>
 Requires-Python: <3.11,>=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: docs
 License-File: LICENSE
```

### Comparing `astrohack-0.1.0/README.md` & `astrohack-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `astrohack-0.1.0/pyproject.toml` & `astrohack-0.1.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "astrohack"
-version = "0.1.0"
+version = "0.1.1"
 description = "Holography Antenna Commissioning Kit"
 authors = [
     {name = "Jan-Willem Steeb", email="jsteeb@nrao.edu"},
     {name = "Joshua Hoskins", email="jhoskins@nrao.edu"}, 
     {name = "Victor de Souza Magalhaes", email="vdesouza@nrao.edu"}
 ]
 license = {file = "LICENSE.txt"}
```

### Comparing `astrohack-0.1.0/src/astrohack/_classes/antenna_surface.py` & `astrohack-0.1.1/src/astrohack/_classes/antenna_surface.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,18 +1,22 @@
+import numpy as np
 import xarray as xr
 from matplotlib import pyplot as plt
+from matplotlib import colormaps as cmaps
 from mpl_toolkits.axes_grid1 import make_axes_locatable
 from astrohack._classes.base_panel import panel_models, irigid
 from astrohack._classes.ring_panel import RingPanel
 from astrohack._utils._constants import *
 from astrohack._utils._conversion import _convert_to_db
 from astrohack._utils._conversion import _convert_unit
 from astrohack._utils._logger._astrohack_logger import _get_astrohack_logger
+from astrohack._utils._utils import _add_prefix
 
 lnbr = "\n"
+figsize = [5, 4]
 
 
 class AntennaSurface:
     def __init__(self, inputxds, telescope, cutoff=None, pmodel=None, crop=False, panel_margins=None, reread=False):
         """
         Antenna Surface description capable of computing RMS, Gains, and fitting the surface to obtain screw adjustments
         Args:
@@ -286,24 +290,26 @@
         """
         Build list of panels, specific for circular antennas with panels arranged in rings
         """
         self.panels = []
         for iring in range(self.telescope.nrings):
             angle = 2.0 * np.pi / self.telescope.npanel[iring]
             for ipanel in range(self.telescope.npanel[iring]):
+
                 panel = RingPanel(
                     self.panelmodel,
                     angle,
                     ipanel,
                     self._panel_label(iring, ipanel),
                     self.telescope.inrad[iring],
                     self.telescope.ourad[iring],
                     margin=self.panel_margins,
                     screw_scheme=self.telescope.screw_description,
-                    screw_offset=self.telescope.screw_offset
+                    screw_offset=self.telescope.screw_offset,
+                    plot_screw_size=0.006 * self.telescope.diam
                 )
                 self.panels.append(panel)
         return
 
     def _compile_panel_points_ringed(self):
         panels = np.zeros(self.rad.shape)
         panelsum = 0
@@ -435,127 +441,185 @@
     def print_misc(self):
         """
         Print miscelaneous information on the panels in the antenna surface
         """
         for panel in self.panels:
             panel.print_misc()
 
-    def plot_surface(self, filename=None, mask=False, screws=False, dpi=300, plotphase=False, unit=None):
+    def plot_mask(self, basename, screws=False, colormap=None, figuresize=None, dpi=300):
         """
-        Do plots of the antenna surface
+        Plot mask used in the selection of points to be fitted
         Args:
-            filename: Save plot to a file rather than displaying it with matplotlib widgets
-            mask: Display mask, amplitudes and panel assignment rather than deviation/phase images
-            plotphase: plot phase images rather than deviation images
-            screws: Display the screws on the panels
-            dpi: Plot resolution in DPI
-            unit: To do deviation/phase plots, defaults to mm for deviations and degrees for phase
-        """
-
-        if mask:
-            fig, ax = plt.subplots(1, 3, figsize=[15, 5])
-            title = "Mask"
-            self._plot_surface(
-                self.mask, title, fig, ax[0], 0, 1, screws=screws, mask=mask
-            )
-            vmin, vmax = np.nanmin(self.amplitude), np.nanmax(self.amplitude)
-            title = "Amplitude min={0:.5f}, max ={1:.5f} V".format(vmin, vmax)
-            self._plot_surface(
-                self.amplitude, title, fig, ax[1], vmin, vmax, screws=screws,
-                unit=self.amp_unit,
-            )
-            title = "Panel assignments"
-            paneldist = np.where(self.panel_distribution >= 0, self.panel_distribution, np.nan)
-            self._plot_surface(paneldist, title, fig, ax[2], 0, np.max(self.panel_distribution), unit='Panel #')
-            fig.tight_layout()
-        else:
-            if plotphase:
-                if unit is None:
-                    unit = 'deg'
-                fac = _convert_unit('rad', unit, 'trigonometric')
-                self._plot_three_surfaces(self.phase, self.phase_corrections, self.phase_residuals, unit,
-                                          fac, screws, 'Antenna surface phase')
-            else:
-                if unit is None:
-                    unit = 'mm'
-                fac = _convert_unit('m', unit, 'length')
-                self._plot_three_surfaces(self.deviation, self.corrections, self.residuals, unit, fac, screws,
-                                          'Antenna surface')
-        if filename is None:
-            plt.show()
-            plt.close()
-        else:
-            plt.savefig(filename, dpi=dpi)
-            plt.close()
-
-    def _plot_three_surfaces(self, original, corrections, residuals, unit, conversion, screws, suptitle):
-        """
-        Factorizes the plot of the combination of 3 maps
-        Args:
-            original: Original dataset
-            corrections: Corrections applied to the dataset
-            residuals: Residuals after correction
-            unit: Unit of the output data
-            conversion: Conversion factor between internal units and unit
-            screws: show screws (Bool)
-            suptitle: Superior title to be displayed on top of the figure
+            basename: basename for the plot, the prefix 'ancillary_mask' will be added to it
+            screws: Are screw positions to be shown in plot?
+            colormap: Colormap for amplitude plot
+            figuresize: 2 element array with the image sizes in inches
+            dpi: Plot resolution
+        """
+        plotmask = np.where(self.mask, 1, np.nan)
+        plotname = _add_prefix(basename, 'mask')
+        self._plot_map(plotname, plotmask, 'Mask', 0, 1, None, screws=screws, colormap=colormap, figuresize=figuresize,
+                       dpi=dpi, colorbar=False)
+
+    def plot_amplitude(self, basename, screws=False, colormap=None, figuresize=None, dpi=300):
+        """
+        Plot Amplitude map
+        Args:
+            basename: basename for the plot, the prefix 'ancillary_amplitude' will be added to it
+            screws: Are screw positions to be shown in plot?
+            colormap: Colormap for amplitude plot
+            figuresize: 2 element array with the image sizes in inches
+            dpi: Plot resolution
+        """
+        vmin, vmax = np.nanmin(self.amplitude), np.nanmax(self.amplitude)
+        title = "Amplitude min={0:.5f}, max ={1:.5f} V".format(vmin, vmax)
+        plotname = _add_prefix(basename, 'amplitude')
+        self._plot_map(plotname, self.amplitude, title, vmin, vmax, self.amp_unit, screws=screws, colormap=colormap,
+                       figuresize=figuresize, dpi=dpi)
+
+    def plot_phase(self, basename, screws=False, colormap=None, figuresize=None, dpi=300, unit=None):
+        """
+        Plot phase map(s)
+        Args:
+            basename: basename for the plot(s), the prefix 'phase_{original|corrections|residuals}' will be added to it/them
+            screws: Are screw positions to be shown in plot(s)?
+            colormap: Colormap for phase plots
+            figuresize: 2 element array with the image sizes in inches
+            dpi: Plot resolution
+            unit: Angle unit for plot(s)
+        """
+        if unit is None:
+            unit = 'deg'
+        fac = _convert_unit('rad', unit, 'trigonometric')
+        prefix = 'phase'
+        if self.residuals is None:
+            maps = [self.phase]
+            labels = ['original']
+        else:
+            maps = [self.phase, self.phase_corrections, self.phase_residuals]
+            labels = ['original', 'corrections', 'residuals']
+        self._multi_plot(maps, labels, prefix, basename, unit, fac, screws, colormap, figuresize, dpi)
+
+    def plot_deviation(self, basename, screws=False, colormap=None, figuresize=None, dpi=300, unit=None):
+        """
+        Plot deviation map(s)
+        Args:
+            basename: basename for the plot(s), the prefix 'deviation_{original|corrections|residuals}' will be added to it/them
+            screws: Are screw positions to be shown in plot(s)?
+            colormap: Colormap for deviation plots
+            figuresize: 2 element array with the image sizes in inches
+            dpi: Plot resolution
+            unit: Length unit for plot(s)
         """
-        vmax = np.nanmax(np.abs(conversion*original))
-        vmin = -vmax
-        in_rms = conversion * self._compute_rms_array(original)
+        if unit is None:
+            unit = 'mm'
+        fac = _convert_unit('m', unit, 'length')
+        prefix = 'deviation'
         if self.residuals is None:
-            fig, ax = plt.subplots()
-            title = "Before correction\nRMS = {0:8.5} ".format(in_rms)+unit
-            self._plot_surface(conversion * original, title, fig, ax, vmin, vmax, screws=screws, unit=unit)
-        else:
-            fig, ax = plt.subplots(1, 3, figsize=[15, 5])
-            out_rms = conversion * self._compute_rms_array(residuals)
-            title = "Before correction\nRMS = {0:.3} ".format(in_rms)+unit
-            self._plot_surface(conversion * original, title, fig, ax[0], vmin, vmax, screws=screws, unit=unit)
-            title = "Corrections"
-            self._plot_surface(conversion * corrections, title, fig, ax[1], vmin, vmax, screws=screws, unit=unit)
-            title = "After correction\nRMS = {0:.3} ".format(out_rms)+unit
-            self._plot_surface(conversion * residuals, title, fig, ax[2], vmin, vmax, screws=screws, unit=unit)
-        fig.suptitle(suptitle)
+            maps = [self.deviation]
+            labels = ['original']
+        else:
+            maps = [self.deviation, self.corrections, self.residuals]
+            labels = ['original', 'corrections', 'residuals']
+        self._multi_plot(maps, labels, prefix, basename, unit, fac, screws, colormap, figuresize, dpi)
+
+    def _multi_plot(self, maps, labels, prefix, basename, unit, conversion, screws, colormap=None, figuresize=None,
+                    dpi=300):
+        if len(maps) != len(labels):
+            raise Exception('Map list and label list must be of the same size')
+        nplots = len(maps)
+        vmax = np.nanmax(np.abs(conversion*maps[0]))
+        vmin = -vmax
+        for iplot in range(nplots):
+            title = f'{prefix.capitalize()} {labels[iplot]}'
+            plotname = _add_prefix(basename, labels[iplot])
+            plotname = _add_prefix(plotname, prefix)
+            self._plot_map(plotname, conversion*maps[iplot], title, vmin, vmax, unit, screws=screws, dpi=dpi)
+
+    def _plot_map(self, filename, data, title, vmin, vmax, unit, screws=False, colormap=None, figuresize=None, dpi=300,
+                  colorbar=True):
+        if colormap is None:
+            colormap = 'viridis'
+        if figuresize is None:
+            figuresize = figsize
+        fig, ax = plt.subplots(1, 1, figsize=figuresize)
+        ax.set_title(title)
+        # set the limits of the plot to the limits of the data
+        xmin = np.min(self.u_axis)
+        xmax = np.max(self.u_axis)
+        ymin = np.min(self.v_axis)
+        ymax = np.max(self.v_axis)
+        im = ax.imshow(data, cmap=colormap, interpolation="nearest", extent=[xmin, xmax, ymin, ymax],
+                       vmin=vmin, vmax=vmax,)
+        if colorbar:
+            divider = make_axes_locatable(ax)
+            cax = divider.append_axes("right", size="5%", pad=0.05)
+            fig.colorbar(im, label="Z Scale [" + unit + "]", cax=cax)
+        ax.set_xlabel("X axis [m]")
+        ax.set_ylabel("Y axis [m]")
+        for panel in self.panels:
+            panel.plot(ax, screws=screws)
         fig.tight_layout()
+        plt.savefig(filename, dpi=dpi)
+        plt.close()
 
-    def _plot_surface(self, data, title, fig, ax, vmin, vmax, screws=False, mask=False, unit="mm"):
+    def plot_screw_adjustments(self, filename, unit, threshold=None, colormap=None, figuresize=None, dpi=300):
         """
-        Does the plotting of a data array in a figure's subplot
+        Plot screw adjustments as circles over a blank canvas with the panel layout
         Args:
-            data: The array to be plotted
-            title: Title of the subplot
-            fig: Global figure containing the subplots
-            ax: matplotlib axes instance describing the subplot
-            vmin: minimum to the color scale
-            vmax: maximum to the color scale
-            screws: Display screws
-            mask: do not add colorbar if plotting a mask
-            unit: Unit of the data in the color scale
+            filename: Name of the output filename for the plot
+            unit: Unit to display the screw adjustments
+            threshold: Threshold below which data is considered negligable, value is assumed to be in the same unit as the plot, if not given defaults to 10% of the maximal deviation
+            colormap: Colormap to display the screw adjustments
+            figuresize: 2 element array with the image sizes in inches
+            dpi: Resolution in pixels per inch
         """
-        ax.set_title(title)
+        if colormap is None:
+            cmap = cmaps['RdBu_r']
+        else:
+            cmap = cmaps[colormap]
+        if figuresize is None or figuresize == 'None':
+            fig, ax = plt.subplots(1, 1, figsize=figsize)
+        else:
+            fig, ax = plt.subplots(1, 1, figsize=figuresize)
+        fac = _convert_unit('m', unit, 'length')
+        vmax = np.nanmax(np.abs(fac * self.screw_adjustments))
+        vmin = -vmax
+        if threshold is None:
+            threshold = 0.1*vmax
+        else:
+            threshold = np.abs(threshold)
+
+        fig.suptitle('Screw corrections', y=0.92, fontsize='large')
+        ax.set_title(f'\nThreshold = {threshold:.2f} {unit}', fontsize='small')
         # set the limits of the plot to the limits of the data
         xmin = np.min(self.u_axis)
         xmax = np.max(self.u_axis)
         ymin = np.min(self.v_axis)
         ymax = np.max(self.v_axis)
-        im = ax.imshow(data,
-                       cmap="viridis",
-                       interpolation="nearest",
-                       extent=[xmin, xmax, ymin, ymax],
-                       vmin=vmin,
-                       vmax=vmax,)
+        im = ax.imshow(np.full_like(self.deviation, fill_value=np.nan), cmap=cmap, interpolation="nearest",
+                       extent=[xmin, xmax, ymin, ymax], vmin=vmin, vmax=vmax)
         divider = make_axes_locatable(ax)
-        if not mask:
-            cax = divider.append_axes("right", size="5%", pad=0.05)
-            fig.colorbar(im, label="Z Scale [" + unit + "]", cax=cax)
+        cax = divider.append_axes("right", size="5%", pad=0.05)
+        colorbar = fig.colorbar(im, label="Screw adjustments [" + unit + "]", cax=cax)
+        if threshold>0:
+            line = threshold
+            while line < vmax:
+                colorbar.ax.axhline(y=line, color='black', linestyle='-', lw=0.2)
+                colorbar.ax.axhline(y=-line, color='black', linestyle='-', lw=0.2)
+                line += threshold
         ax.set_xlabel("X axis [m]")
         ax.set_ylabel("Y axis [m]")
-        for panel in self.panels:
-            panel.plot(ax, screws=screws)
+
+        for ipanel in range(len(self.panels)):
+            self.panels[ipanel].plot(ax, screws=False)
+            self.panels[ipanel].plot_corrections(ax, cmap, fac*self.screw_adjustments[ipanel], threshold, vmin, vmax)
+        fig.tight_layout()
+        plt.savefig(filename, dpi=dpi)
+        plt.close()
 
     def _build_panel_data_arrays(self):
         """
         Build arrays with data from the panels so that they can be stored on the XDS
         Returns:
             List with panel labels, panel fitting parameters, screw_adjustments
         """
@@ -580,15 +644,15 @@
         outfile = "Screw adjustments for {0:s} {1:s} antenna\n".format(self.telescope.name, self.antenna_name)
         outfile += "Adjustments are in " + unit + 2*lnbr
         outfile += "Lower means away from subreflector" + lnbr
         outfile += "Raise means toward the subreflector" + lnbr
         outfile += "LOWER the panel if the number is POSITIVE" + lnbr
         outfile += "RAISE the panel if the number is NEGATIVE" + lnbr
         outfile += 2 * lnbr
-        outfile += "{0:8s}".format('Panel')
+        outfile += "{0:16s}".format('Panel')
         nscrews = len(self.telescope.screw_description)
         for screw in self.telescope.screw_description:
             outfile += "{0:11s}".format(screw)
         outfile += lnbr
         fac = _convert_unit('m', unit, 'length')
         for ipanel in range(len(self.panel_labels)):
             outfile += "{0:8s}".format(self.panel_labels[ipanel])
```

### Comparing `astrohack-0.1.0/src/astrohack/_classes/base_panel.py` & `astrohack-0.1.1/src/astrohack/_classes/base_panel.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,10 @@
 from scipy import optimize as opt
+from matplotlib import pyplot as plt
+from matplotlib.colors import Normalize
 
 from astrohack._utils._algorithms import _gauss_elimination_numpy, _least_squares_fit
 from astrohack._utils._constants import *
 from astrohack._utils._conversion import _convert_unit
 from astrohack._utils._logger._astrohack_logger import _get_astrohack_logger
 
 panel_models = ["mean", "rigid", "corotated_scipy", "corotated_lst_sq", "corotated_robust", "xy_paraboloid",
@@ -34,15 +36,15 @@
     markers = ['X', 'o', '*', 'P', 'D']
     colors = ['g', 'g', 'r', 'r', 'b']
     fontsize = 4
     linewidth = 0.5
     markersize = 2
     linecolor = 'black'
 
-    def __init__(self, model, screws, label, center=None, zeta=None):
+    def __init__(self, model, screws, plot_screw_pos, plot_screw_size, label, center=None, zeta=None):
         """
         Initializes the base panel with the appropriated fitting methods and providing basic functionality
         Fitting method models are:
         AIPS fitting models:
             mean: The panel is corrected by the mean of its samples
             rigid: The panel samples are fitted to a rigid surface
         Corotated Paraboloids (the two bending axes are parallel and perpendicular to the radius of the antenna crossing
@@ -61,14 +63,16 @@
             center: Panel center
             zeta: panel center angle
         """
         self.model = model
         self.solved = False
         self.label = label
         self.screws = screws
+        self.plot_screw_pos = plot_screw_pos
+        self.plot_screw_size = plot_screw_size
         self.samples = []
         self.margins = []
         self.corr = None
 
         if center is None:
             self.center = [0, 0]
         else:
@@ -529,7 +533,30 @@
         Args:
             ax: matplotlib axes instance
         """
         for iscrew in range(self.screws.shape[0]):
             screw = self.screws[iscrew, ]
             ax.scatter(screw[1], screw[0], marker=self.markers[iscrew], lw=self.linewidth, s=self.markersize,
                        color=self.colors[iscrew])
+
+    def plot_corrections(self, ax, cmap, corrections, threshold, vmin, vmax):
+        """
+        Plot screw corrections onto an axis
+        Args:
+            ax: axis for plot
+            cmap: Colormap of the corrections
+            corrections: the screw corrections
+            threshold: Threshold below which data is considered negligable
+            vmin: bottom of the colormap
+            vmax: top of the colormap
+        """
+        norm = Normalize(vmin=vmin, vmax=vmax)
+        for iscrew in range(self.plot_screw_pos.shape[0]):
+            screw = self.plot_screw_pos[iscrew, ]
+            if np.abs(corrections[iscrew]) < threshold:
+                corr = 0
+            else:
+                corr = corrections[iscrew]
+            circle = plt.Circle((screw[1], screw[0]), self.plot_screw_size, color=cmap(norm(corr)),
+                                fill=True)
+            ax.add_artist(circle)
+
```

### Comparing `astrohack-0.1.0/src/astrohack/_classes/polygon_panel.py` & `astrohack-0.1.1/src/astrohack/_classes/polygon_panel.py`

 * *Files identical despite different names*

### Comparing `astrohack-0.1.0/src/astrohack/_classes/ring_panel.py` & `astrohack-0.1.1/src/astrohack/_classes/ring_panel.py`

 * *Files 10% similar despite different names*

```diff
@@ -4,15 +4,16 @@
 from astrohack._utils._constants import twopi
 
 
 class RingPanel(BasePanel):
     # This class describes and treats panels that are arranged in
     # rings on the Antenna surface
 
-    def __init__(self, kind, angle, ipanel, label, inrad, ourad, margin=0.20, screw_scheme=None, screw_offset=None):
+    def __init__(self, kind, angle, ipanel, label, inrad, ourad, margin=0.20, screw_scheme=None, screw_offset=None,
+                 plot_screw_size=0.20):
         """
         Initializes a panel that is a section of a ring in a circular antenna
         Fitting method kinds are:
         AIPS fitting kinds:
             mean: The panel is corrected by the mean of its samples
             rigid: The panel samples are fitted to a rigid surface
         Corotated Paraboloids (the two bending axes are parallel and perpendicular to the radius of the antenna crossing
@@ -44,16 +45,17 @@
         self.margin_inrad = inrad + margin * dradius
         self.margin_ourad = ourad - margin * dradius
         self.first = ipanel == 0
         zeta = (ipanel + 0.5) * angle
         rt = (self.inrad + self.ourad) / 2
         self.center = [rt * np.cos(zeta), rt * np.sin(zeta)]
         screws = self._init_screws(screw_scheme, screw_offset)
+        plot_screw_pos = self._init_screws(screw_scheme, 2*plot_screw_size)
         # Now we are ready to initialize the base object
-        super().__init__(kind, screws, label, center=self.center, zeta=zeta)
+        super().__init__(kind, screws, plot_screw_pos, plot_screw_size, label, center=self.center, zeta=zeta)
 
     def _init_screws(self, scheme, offset):
         """
         Initialize screws according to the scheme
         Args:
             scheme: Tuple of strings containing the positioning of the screws
             offset: How far from the edge of the panel are corner screws (meters)
```

### Comparing `astrohack-0.1.0/src/astrohack/_classes/telescope.py` & `astrohack-0.1.1/src/astrohack/_classes/telescope.py`

 * *Files identical despite different names*

### Comparing `astrohack-0.1.0/src/astrohack/_utils/_algorithms.py` & `astrohack-0.1.1/src/astrohack/_utils/_algorithms.py`

 * *Files identical despite different names*

### Comparing `astrohack-0.1.0/src/astrohack/_utils/_constants.py` & `astrohack-0.1.1/src/astrohack/_utils/_constants.py`

 * *Files 1% similar despite different names*

```diff
@@ -32,8 +32,8 @@
 
 # https://github.com/casacore/casacore/blob/dbf28794ef446bbf4e6150653dbe404379a3c429/measures/Measures/Stokes.h
 pol_codes_RL = np.array([5, 6, 7, 8]) #'RR','RL','LR','LL'
 pol_codes_XY = np.array([9, 10, 11, 12]) #['XX','XY','YX','YY']
 pol_str = np.array(['0','I','Q','U','V','RR','RL','LR','LL','XX','XY','YX','YY'])
 
 #Plot types
-plot_types = ['deviation', 'phase', 'ancillary']
+plot_types = ['deviation', 'phase', 'ancillary', 'all']
```

### Comparing `astrohack-0.1.0/src/astrohack/_utils/_conversion.py` & `astrohack-0.1.1/src/astrohack/_utils/_conversion.py`

 * *Files identical despite different names*

### Comparing `astrohack-0.1.0/src/astrohack/_utils/_dask_plugins/_astrohack_scheduler.py` & `astrohack-0.1.1/src/astrohack/_utils/_dask_plugins/_astrohack_scheduler.py`

 * *Files identical despite different names*

### Comparing `astrohack-0.1.0/src/astrohack/_utils/_dask_plugins/_astrohack_worker.py` & `astrohack-0.1.1/src/astrohack/_utils/_dask_plugins/_astrohack_worker.py`

 * *Files identical despite different names*

### Comparing `astrohack-0.1.0/src/astrohack/_utils/_dio.py` & `astrohack-0.1.1/src/astrohack/_utils/_dio.py`

 * *Files identical despite different names*

### Comparing `astrohack-0.1.0/src/astrohack/_utils/_extract_holog.py` & `astrohack-0.1.1/src/astrohack/_utils/_extract_holog.py`

 * *Files identical despite different names*

### Comparing `astrohack-0.1.0/src/astrohack/_utils/_extract_point.py` & `astrohack-0.1.1/src/astrohack/_utils/_extract_point.py`

 * *Files identical despite different names*

### Comparing `astrohack-0.1.0/src/astrohack/_utils/_holog.py` & `astrohack-0.1.1/src/astrohack/_utils/_holog.py`

 * *Files 2% similar despite different names*

```diff
@@ -67,25 +67,21 @@
     map0 = list(ant_data_dict[ddi].keys())[0]
     
     freq_chan = ant_data_dict[ddi][map0].chan.values
     n_chan = ant_data_dict[ddi][map0].dims["chan"]
     n_pol = ant_data_dict[ddi][map0].dims["pol"]
     
     if holog_chunk_params["chan_average"]:
-        reference_scaling_frequency = holog_chunk_params["reference_scaling_frequency"]
-
-        if reference_scaling_frequency is None:
-            reference_scaling_frequency = np.mean(freq_chan)
+        reference_scaling_frequency = np.mean(freq_chan)
 
         avg_chan_map, avg_freq = _create_average_chan_map(freq_chan, holog_chunk_params["chan_tolerance_factor"])
         
         # Only a single channel left after averaging.
         beam_grid = np.zeros((n_holog_map,) + (1, n_pol) + grid_l.shape, dtype=np.complex)
-        
-        
+
     else:
         beam_grid = np.zeros((n_holog_map,) + (n_chan, n_pol) + grid_l.shape, dtype=np.complex)
 
     time_centroid = []
 
     for holog_map_index, holog_map in enumerate(ant_data_dict[ddi].keys()):
         ant_xds = ant_data_dict[ddi][holog_map]
```

### Comparing `astrohack-0.1.0/src/astrohack/_utils/_imaging.py` & `astrohack-0.1.1/src/astrohack/_utils/_imaging.py`

 * *Files identical despite different names*

### Comparing `astrohack-0.1.0/src/astrohack/_utils/_io.py` & `astrohack-0.1.1/src/astrohack/_utils/_io.py`

 * *Files identical despite different names*

### Comparing `astrohack-0.1.0/src/astrohack/_utils/_logger/_astrohack_logger.py` & `astrohack-0.1.1/src/astrohack/_utils/_logger/_astrohack_logger.py`

 * *Files identical despite different names*

### Comparing `astrohack-0.1.0/src/astrohack/_utils/_panel.py` & `astrohack-0.1.1/src/astrohack/_utils/_panel.py`

 * *Files 3% similar despite different names*

```diff
@@ -625,25 +625,27 @@
     rms = np.zeros((ntime, nchan, npol))
     for time in range(ntime):
         for chan in range(nchan):
             for pol in range(npol):
                 rms[time, chan, pol] = np.sqrt(np.nanmean(phase_image[time, chan, pol] ** 2))
     return rms
 
+
 def _plot_antenna_chunk(parm_dict):
     antenna = parm_dict['this_antenna']
     ddi = parm_dict['this_ddi']
     destination = parm_dict['destination']
     plot_type = parm_dict['plot_type']
-    plot_name = f'{destination}/{plot_type}_{antenna}_{ddi}.png'
-
+    basename = f'{destination}/{antenna}_{ddi}'
     surface = parm_dict['panel_mds'].get_antenna(antenna, ddi)
     if plot_type == plot_types[0]:  # deviation plot
-        surface.plot_surface(filename=plot_name, mask=False, screws=parm_dict['plot_screws'], dpi=parm_dict['dpi'],
-                             plotphase=False, unit=parm_dict['unit'])
+        surface.plot_deviation(basename, screws=parm_dict['plot_screws'], dpi=parm_dict['dpi'], unit=parm_dict['unit'])
     elif plot_type == plot_types[1]:  # phase plot
-        surface.plot_surface(filename=plot_name, mask=False, screws=parm_dict['plot_screws'], dpi=parm_dict['dpi'],
-                             plotphase=True, unit=parm_dict['unit'])
-    else:  # Ancillary plot
-        surface.plot_surface(filename=plot_name, mask=True, screws=parm_dict['plot_screws'], dpi=parm_dict['dpi'],
-                             plotphase=False, unit=None)
-
+        surface.plot_phase(basename, screws=parm_dict['plot_screws'], dpi=parm_dict['dpi'], unit=parm_dict['unit'])
+    elif plot_type == plot_types[2]:  # Ancillary plot
+        surface.plot_mask(basename=basename, screws=parm_dict['plot_screws'], dpi=parm_dict['dpi'])
+        surface.plot_amplitude(basename=basename, screws=parm_dict['plot_screws'], dpi=parm_dict['dpi'])
+    else: # all plots
+        surface.plot_deviation(basename, screws=parm_dict['plot_screws'], dpi=parm_dict['dpi'], unit=parm_dict['unit'])
+        surface.plot_phase(basename, screws=parm_dict['plot_screws'], dpi=parm_dict['dpi'], unit=parm_dict['unit'])
+        surface.plot_mask(basename=basename, screws=parm_dict['plot_screws'], dpi=parm_dict['dpi'])
+        surface.plot_amplitude(basename=basename, screws=parm_dict['plot_screws'], dpi=parm_dict['dpi'])
```

### Comparing `astrohack-0.1.0/src/astrohack/_utils/_parm_utils/_check_logger_parms.py` & `astrohack-0.1.1/src/astrohack/_utils/_parm_utils/_check_logger_parms.py`

 * *Files identical despite different names*

### Comparing `astrohack-0.1.0/src/astrohack/_utils/_parm_utils/_check_parms.py` & `astrohack-0.1.1/src/astrohack/_utils/_parm_utils/_check_parms.py`

 * *Files identical despite different names*

### Comparing `astrohack-0.1.0/src/astrohack/_utils/gaussfitter.py` & `astrohack-0.1.1/src/astrohack/_utils/gaussfitter.py`

 * *Files identical despite different names*

### Comparing `astrohack-0.1.0/src/astrohack/astrohack_client.py` & `astrohack-0.1.1/src/astrohack/astrohack_client.py`

 * *Files identical despite different names*

### Comparing `astrohack-0.1.0/src/astrohack/data/.file_meta_data/ea25_cal_small_spw1_4_60_ea04_after.json` & `astrohack-0.1.1/src/astrohack/data/.file_meta_data/ea25_cal_small_spw1_4_60_ea04_after.json`

 * *Files identical despite different names*

### Comparing `astrohack-0.1.0/src/astrohack/data/.file_meta_data/ea25_cal_small_spw1_4_60_ea04_after_fixed.json` & `astrohack-0.1.1/src/astrohack/data/.file_meta_data/ea25_cal_small_spw1_4_60_ea04_after_fixed.json`

 * *Files identical despite different names*

### Comparing `astrohack-0.1.0/src/astrohack/data/.file_meta_data/ea25_cal_small_spw1_4_60_ea04_before.json` & `astrohack-0.1.1/src/astrohack/data/.file_meta_data/ea25_cal_small_spw1_4_60_ea04_before.json`

 * *Files identical despite different names*

### Comparing `astrohack-0.1.0/src/astrohack/data/.file_meta_data/ea25_cal_small_spw1_4_60_ea04_before_fixed.json` & `astrohack-0.1.1/src/astrohack/data/.file_meta_data/ea25_cal_small_spw1_4_60_ea04_before_fixed.json`

 * *Files identical despite different names*

### Comparing `astrohack-0.1.0/src/astrohack/data/telescopes/aca_7m.zarr/.zattrs` & `astrohack-0.1.1/src/astrohack/data/telescopes/aca_7m.zarr/.zattrs`

 * *Files identical despite different names*

### Comparing `astrohack-0.1.0/src/astrohack/data/telescopes/aca_7m.zarr/.zmetadata` & `astrohack-0.1.1/src/astrohack/data/telescopes/aca_7m.zarr/.zmetadata`

 * *Files identical despite different names*

### Comparing `astrohack-0.1.0/src/astrohack/data/telescopes/alma_da.zarr/.zattrs` & `astrohack-0.1.1/src/astrohack/data/telescopes/alma_da.zarr/.zattrs`

 * *Files identical despite different names*

### Comparing `astrohack-0.1.0/src/astrohack/data/telescopes/alma_da.zarr/.zmetadata` & `astrohack-0.1.1/src/astrohack/data/telescopes/alma_da.zarr/.zmetadata`

 * *Files identical despite different names*

### Comparing `astrohack-0.1.0/src/astrohack/data/telescopes/alma_dv.zarr/.zattrs` & `astrohack-0.1.1/src/astrohack/data/telescopes/alma_dv.zarr/.zattrs`

 * *Files identical despite different names*

### Comparing `astrohack-0.1.0/src/astrohack/data/telescopes/alma_dv.zarr/.zmetadata` & `astrohack-0.1.1/src/astrohack/data/telescopes/alma_dv.zarr/.zmetadata`

 * *Files identical despite different names*

### Comparing `astrohack-0.1.0/src/astrohack/data/telescopes/alma_tp.zarr/.zattrs` & `astrohack-0.1.1/src/astrohack/data/telescopes/alma_tp.zarr/.zattrs`

 * *Files identical despite different names*

### Comparing `astrohack-0.1.0/src/astrohack/data/telescopes/alma_tp.zarr/.zmetadata` & `astrohack-0.1.1/src/astrohack/data/telescopes/alma_tp.zarr/.zmetadata`

 * *Files identical despite different names*

### Comparing `astrohack-0.1.0/src/astrohack/data/telescopes/vla.zarr/.zattrs` & `astrohack-0.1.1/src/astrohack/data/telescopes/vla.zarr/.zattrs`

 * *Files identical despite different names*

### Comparing `astrohack-0.1.0/src/astrohack/data/telescopes/vla.zarr/.zmetadata` & `astrohack-0.1.1/src/astrohack/data/telescopes/vla.zarr/.zmetadata`

 * *Files identical despite different names*

### Comparing `astrohack-0.1.0/src/astrohack/data/telescopes/vlba.zarr/.zattrs` & `astrohack-0.1.1/src/astrohack/data/telescopes/vlba.zarr/.zattrs`

 * *Files identical despite different names*

### Comparing `astrohack-0.1.0/src/astrohack/data/telescopes/vlba.zarr/.zmetadata` & `astrohack-0.1.1/src/astrohack/data/telescopes/vlba.zarr/.zmetadata`

 * *Files identical despite different names*

### Comparing `astrohack-0.1.0/src/astrohack/dio.py` & `astrohack-0.1.1/src/astrohack/dio.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,71 +1,87 @@
 import os
 import dask
+import numbers
 import numpy as np
+from matplotlib import colormaps as cmaps
 
-from astropy.time import Time
 from casacore import tables
 
 from astrohack._utils._constants import length_units, trigo_units, plot_types
 from astrohack._utils._parm_utils._check_parms import _check_parms
 from astrohack._utils._logger._astrohack_logger import _get_astrohack_logger
 from astrohack._utils._utils import _parm_to_list
 
-from astrohack._utils._io import _load_point_file
-from astrohack._utils._io import _open_no_dask_zarr
-from astrohack._utils._io import _read_data_from_holog_json
-from astrohack._utils._io import _read_meta_data
-from astrohack._utils._io import _load_holog_file
-from astrohack._utils._io import _load_image_file
-from astrohack._utils._io import _load_panel_file
-
 from astrohack._utils._dio import AstrohackImageFile
 from astrohack._utils._dio import AstrohackHologFile
 from astrohack._utils._dio import AstrohackPanelFile
 from astrohack._utils._dio import AstrohackPointFile
 
 from astrohack._utils._panel import _plot_antenna_chunk
 
 
-def export_screws(panel_mds_name, destination, ant_name=None, ddi=None,  unit='mm'):
+def export_screws(panel_mds_name, destination, ant_name=None, ddi=None,  unit='mm', threshold=None, plot_map=False,
+                  colormap='seismic', figuresize=None, dpi=300):
     """ Export screw adjustment from panel to text file and save to disk.
 
     :param panel_mds_name: Input panel_mds file
     :type panel_mds_name: str
     :param destination: Name of the destination folder to contain exported screw adjustments
     :type destination: str
     :param ant_name: List of antennae/antenna to be exported, defaults to "all" when None
     :type ant_name: list or str, optional, ex. ant_ea25
     :param ddi: List of ddis/ddi to be exported, defaults to "all" when None
     :type ddi: list or str, optional, ex. ddi_0
     :param unit: Unit for screws adjustments, most length units supported, defaults to "mm"
     :type unit: str
+    :param threshold: Threshold below which data is considered negligable, value is assumed to be in the same unit as the plot, if not given defaults to 10% of the maximal deviation
+    :type threshold: float, optional
+    :param plot_map: Plot the map of screw adjustments, default is False
+    :type plot_map: bool
+    :param colormap: Colormap for screw adjustment map
+    :type colormap: str
+    :param figuresize: 2 element array/list/tuple with the screw adjustment map size in inches
+    :type figuresize: numpy.ndarray, list, tuple, optional
+    :param dpi: Screw adjustment map resolution in pixels per inch
+    :type dpi: int
 
     .. _Description:
 
     Produce the screw adjustments from ``astrohack.panel`` results to be used at the antenna site to improve the antenna surface
 
     """
     logger = _get_astrohack_logger()
     parm_dict = {'filename': panel_mds_name,
                  'ant_name': ant_name,
                  'ddi': ddi,
                  'destination': destination,
-                 'unit': unit}
+                 'unit': unit,
+                 'threshold': threshold,
+                 'plot_map': plot_map,
+                 'colormap': colormap,
+                 'figuresize': figuresize,
+                 'dpi': dpi}
 
     parms_passed = _check_parms(parm_dict, 'filename', [str], default=None)
     parms_passed = parms_passed and _check_parms(parm_dict, 'ant_name', [list], list_acceptable_data_types=[str],
                                                  default='all')
     parms_passed = parms_passed and _check_parms(parm_dict, 'ddi', [list], list_acceptable_data_types=[str],
                                                  default='all')
     parms_passed = parms_passed and _check_parms(parm_dict, 'destination', [str], default=None)
     parms_passed = parms_passed and _check_parms(parm_dict, 'unit', [str], acceptable_data=length_units, default='mm')
+    parms_passed = parms_passed and _check_parms(parm_dict, 'threshold', [numbers.Number], default=None)
+    parms_passed = parms_passed and _check_parms(parm_dict, 'plot_map', [bool], default=False)
+    parms_passed = parms_passed and _check_parms(parm_dict, 'colormap', [str], acceptable_data=cmaps, default='RdBu_r')
+    parms_passed = parms_passed and _check_parms(parm_dict, 'figuresize', [list, np.ndarray],
+                                                 list_acceptable_data_types=[numbers.Number], list_len=2,
+                                                 default='None', log_default_setting=False)
+    parms_passed = parms_passed and _check_parms(parm_dict, 'dpi', [int], default=300)
 
     if not parms_passed:
-        logger.error("export_scews parameter checking failed.")
+        logger.error("export_screws parameter checking failed.")
         raise Exception("export_screws parameter checking failed.")
 
     panel_mds = AstrohackPanelFile(panel_mds_name)
     panel_mds.open()
 
     try:
         os.mkdir(parm_dict['destination'])
@@ -74,39 +90,47 @@
 
     antennae = _parm_to_list(parm_dict['ant_name'], parm_dict['filename'])
     for antenna in antennae:
         if 'ant' in antenna:
             ddis = _parm_to_list(parm_dict['ddi'], parm_dict['filename']+'/'+antenna)
             for ddi in ddis:
                 if 'ddi' in ddi:
-                    export_name = parm_dict['destination']+f'/screws_{antenna}_{ddi}.txt'
+                    export_name = parm_dict['destination']+f'/screws_{antenna}_{ddi}.'
                     surface = panel_mds.get_antenna(antenna, ddi)
-                    surface.export_screws(export_name, unit=unit)
+                    surface.export_screws(export_name+'txt', unit=unit)
+                    if parm_dict['plot_map']:
+                        surface.plot_screw_adjustments(export_name+'png', unit=unit, threshold=parm_dict['threshold'],
+                                                       colormap=parm_dict['colormap'], figuresize=parm_dict['figuresize'],
+                                                       dpi=parm_dict['dpi'])
 
 
 def plot_antenna(panel_mds_name, destination, ant_name=None, ddi=None, plot_type='deviation', plot_screws=False,
-                 dpi=300, unit=None, parallel=True):
+                 unit=None, colormap='viridis', figuresize=None, dpi=300, parallel=True):
     """ Create diagnostic plots of antenna surface deviations from panel data file. Available plots listed in additional information.
 
     :param panel_mds_name: Input panel_mds file
     :type panel_mds_name: str
     :param destination: Name of the destination folder to contain plots
     :type destination: str
     :param ant_name: List of antennae/antenna to be plotted, defaults to "all" when None
     :type ant_name: list or str, optional, ex. ant_ea25
     :param ddi: List of ddis/ddi to be plotted, defaults to "all" when None
     :type ddi: list or str, optional, ex. ddi_0
     :param plot_type: type of plot to be produced, deviation, phase or ancillary
     :type plot_type: str
     :param plot_screws: Add screw positions to plot
     :type plot_screws: bool
-    :param dpi: dots per inch to be used in plots
-    :type dpi: int
     :param unit: Unit for phase or deviation plots, defaults to "mm" for deviation and 'deg' for phase
     :type unit: str
+    :param colormap: Colormap for plots
+    :type colormap: str
+    :param figuresize: 2 element array/list/tuple with the plot sizes in inches
+    :type figuresize: numpy.ndarray, list, tuple, optional
+    :param dpi: dots per inch to be used in plots
+    :type dpi: int
     :param parallel: If True will use an existing astrohack client to produce plots in parallel
     :type parallel: bool
 
     .. _Description:
 
     Produce plots from ``astrohack.panel`` results to be analyzed to judge the quality of the results
 
@@ -126,14 +150,16 @@
     parm_dict = {'filename': panel_mds_name,
                  'ant_name': ant_name,
                  'ddi': ddi,
                  'destination': destination,
                  'unit': unit,
                  'plot_type': plot_type,
                  'plot_screws': plot_screws,
+                 'colormap': colormap,
+                 'figuresize': figuresize,
                  'dpi': dpi,
                  'parallel': parallel}
 
     parms_passed = _check_parms(parm_dict, 'filename', [str], default=None)
     parms_passed = parms_passed and _check_parms(parm_dict, 'ant_name', [list], list_acceptable_data_types=[str],
                                                  default='all')
     parms_passed = parms_passed and _check_parms(parm_dict, 'ddi', [list], list_acceptable_data_types=[str],
@@ -147,19 +173,23 @@
     elif parm_dict['plot_type'] == plot_types[1]:  # Trigonometric units for phase plots
         parms_passed = parms_passed and _check_parms(parm_dict, 'unit', [str], acceptable_data=trigo_units,
                                                      default='deg')
     else:  # Units ignored for ancillary plots
         logger.info('Unit ignored for ancillary plots')
     parms_passed = parms_passed and _check_parms(parm_dict, 'parallel', [bool], default=True)
     parms_passed = parms_passed and _check_parms(parm_dict, 'plot_screws', [bool], default=False)
+    parms_passed = parms_passed and _check_parms(parm_dict, 'colormap', [str], acceptable_data=cmaps, default='viridis')
+    parms_passed = parms_passed and _check_parms(parm_dict, 'figuresize', [list, np.ndarray],
+                                                 list_acceptable_data_types=[numbers.Number], list_len=2,
+                                                 default='None', log_default_setting=False)
     parms_passed = parms_passed and _check_parms(parm_dict, 'dpi', [int], default=300)
 
     if not parms_passed:
-        logger.error("export_scews parameter checking failed.")
-        raise Exception("export_screws parameter checking failed.")
+        logger.error("plot_antenna parameter checking failed.")
+        raise Exception("plot_antenna parameter checking failed.")
 
     panel_mds = AstrohackPanelFile(panel_mds_name)
     panel_mds.open()
     parm_dict['panel_mds'] = panel_mds
 
     try:
         os.mkdir(parm_dict['destination'])
```

### Comparing `astrohack-0.1.0/src/astrohack/extract_holog.py` & `astrohack-0.1.1/src/astrohack/extract_holog.py`

 * *Files 1% similar despite different names*

```diff
@@ -53,15 +53,15 @@
 
     :param holog_obs_dict: The *holog_obs_dict* describes which scan and antenna data to extract from the measurement set. As detailed below, this compound dictionary also includes important meta data needed for preprocessing and extraction of the holography data from the measurement set. If not specified holog_obs_dict will be generated. For auto generation of the holog_obs_dict the assumtion is made that the same antanna beam is not mapped twice in a row (alternating sets of antennas is fine).
     :type holog_obs_dict: dict, optional
     
     :param ddi_sel:  Value(s) of DDI that should be extracted from the measurement set. Defaults to all DDI's in the ms.
     :type ddi_sel: int numpy.ndarray | int list, optional
        
-    :baseline_average_distance: To increase the signal to noise for a mapping antenna mutiple reference antennas can be used. The baseline_average_distance is the acceptable distance between a mapping antenna and a reference antenna. The baseline_average_distance is only used if the holog_obs_dict is not specified. If no distance is specified all reference antennas will be used.
+    :param baseline_average_distance: To increase the signal to noise for a mapping antenna mutiple reference antennas can be used. The baseline_average_distance is the acceptable distance between a mapping antenna and a reference antenna. The baseline_average_distance is only used if the holog_obs_dict is not specified. If no distance is specified all reference antennas will be used.
     :type holog_obs_dict: float, optional
 
     :param holog_name: Name of *<holog_name>.holog.zarr* file to create. Defaults to measurement set name with *holog.zarr* extension.
     :type holog_name: str, optional
 
     :param point_name: Name of *<point_name>.point.zarr* file to create. Defaults to measurement set name with *point.zarr* extension.
     :type point_name: str, optional
```

### Comparing `astrohack-0.1.0/src/astrohack/gdown_utils.py` & `astrohack-0.1.1/src/astrohack/gdown_utils.py`

 * *Files identical despite different names*

### Comparing `astrohack-0.1.0/src/astrohack/holog.py` & `astrohack-0.1.1/src/astrohack/holog.py`

 * *Files 8% similar despite different names*

```diff
@@ -20,15 +20,14 @@
     grid_size=None,
     cell_size=None,
     image_name=None,
     padding_factor=50,
     grid_interpolation_mode="nearest",
     chan_average=True,
     chan_tolerance_factor=0.005,
-    reference_scaling_frequency=None,
     scan_average=True,
     ant_list=None,
     to_stokes=True,
     apply_mask=True,
     phase_fit=True,
     overwrite=False,
     parallel=True):
@@ -57,17 +56,14 @@
 
     :param chan_average: Boolean dictating whether the channel average is computed and written to the output holog file., defaults to True
     :type chan_average: bool, optional
 
     :param chan_tolerance_factor: Tolerance used in channel averaging to determine the number of primary beam channels., defaults to 0.005
     :type chan_tolerance_factor: float, optional
 
-    :param reference_scaling_frequency: When computing the channel average the lm frequency values are scaled by frequency. If the default None is used, the scaling is simply unity, however if `reference_scaling_frequency` is set then the scaling is done according to (average_frequency/reference_scaling_frequency)., defaults to None
-    :type reference_scaling_frequency: float, optional
-
     :param scan_average: Boolean dicating whether averagin is done over scan., defaults to True
     :type scan_average: bool, optional
 
     :param ant_list: Optional list of sub-antennas to use when the user doesn't to do holography for all antennas, defaults to all antennas.
     :type ant_list: list, optional
 
     :param to_stokes: Dictates whether polarization is computed according to stokes values., defaults to True
@@ -121,15 +117,14 @@
         cell_size, 
         image_name, 
         padding_factor, 
         parallel, 
         grid_interpolation_mode, 
         chan_average, 
         chan_tolerance_factor, 
-        reference_scaling_frequency, 
         scan_average,
         ant_list, 
         to_stokes, 
         apply_mask, 
         phase_fit,
         overwrite
     )
@@ -196,28 +191,26 @@
     return image_mds
 
 
 
 def _check_holog_parms(holog_name,grid_size,cell_size,image_name,
                       padding_factor,parallel,grid_interpolation_mode,
                       chan_average,chan_tolerance_factor,
-                      reference_scaling_frequency,scan_average,
-                      ant_list,to_stokes,apply_mask,phase_fit,overwrite):
+                      scan_average,ant_list,to_stokes,apply_mask,phase_fit,overwrite):
 
     holog_params = {}
     holog_params["holog_file"] = holog_name
     holog_params["grid_size"] = grid_size
     holog_params["cell_size"] = cell_size
     holog_params["image_file"] = image_name
     holog_params["padding_factor"] = padding_factor
     holog_params["parallel"] = parallel
     holog_params["grid_interpolation_mode"] = grid_interpolation_mode
     holog_params["chan_average"] = chan_average
     holog_params["chan_tolerance_factor"] = chan_tolerance_factor
-    holog_params["reference_scaling_frequency"] = reference_scaling_frequency
     holog_params["scan_average"] = scan_average
     holog_params["ant_list"] = ant_list
     holog_params["to_stokes"] = to_stokes
     holog_params["apply_mask"] = apply_mask
     holog_params["phase_fit"] = phase_fit
     holog_params["overwrite"] = overwrite
     
@@ -249,19 +242,15 @@
    
     
     parms_passed = parms_passed and _check_parms(holog_params, 'chan_average', [bool],default=True)
 
     
     parms_passed = parms_passed and _check_parms(holog_params, 'chan_tolerance_factor', [float], acceptable_range=[0,1], default=0.005)
    
-    
-    parms_passed = parms_passed and _check_parms(holog_params, 'reference_scaling_frequency', [float,np.float],default='None',log_default_setting=False)
-    if (isinstance(holog_params['reference_scaling_frequency'],str)) and (holog_params['reference_scaling_frequency']) == 'None':
-        holog_params['reference_scaling_frequency'] =  None
-    
+
     parms_passed = parms_passed and _check_parms(holog_params, 'scan_average', [bool],default=True)
 
     parms_passed = parms_passed and _check_parms(holog_params, 'ant_list', [list,np.ndarray], list_acceptable_data_types=[str], default='all')
  
     parms_passed = parms_passed and _check_parms(holog_params, 'to_stokes', [bool],default=True)
```

### Comparing `astrohack-0.1.0/src/astrohack/panel.py` & `astrohack-0.1.1/src/astrohack/panel.py`

 * *Files 1% similar despite different names*

```diff
@@ -114,15 +114,15 @@
         for antenna in antennae:
             if 'ant_' in antenna:
                 panel_chunk_params['antenna'] = antenna
                 
                 if panel_chunk_params['sel_ddi'] == "all":
                     panel_chunk_params['sel_ddi'] = os.listdir(panel_chunk_params['image_name']+'/'+antenna)
 
-                for ddi in panel_chunk_params['sel_ddi'] :
+                for ddi in panel_chunk_params['sel_ddi']:
                     if 'ddi_' in ddi:
                         logger.info(f"Processing {ddi} for {antenna}")
                         panel_chunk_params['ddi'] = ddi
                         if parallel:
                             delayed_list.append(dask.delayed(_panel_chunk)(dask.delayed(panel_chunk_params)))
                         else:
                             _panel_chunk(panel_chunk_params)
@@ -196,14 +196,15 @@
                           
     #### Parameter Checking ####
     logger = _get_astrohack_logger()
     parms_passed = True
     
     parms_passed = parms_passed and _check_parms(panel_params, 'image_name', [str], default=None)
     base_name = _remove_suffix(panel_params['image_name'], '.image.zarr')
+    base_name = _remove_suffix(base_name, '.combine.zarr')
     parms_passed = parms_passed and _check_parms(panel_params, 'panel_name', [str], default=base_name+'.panel.zarr')
     parms_passed = parms_passed and _check_parms(panel_params, 'cutoff', [float], acceptable_range=[0, 1], default=0.2)
     parms_passed = parms_passed and _check_parms(panel_params, 'panel_kind', [str], acceptable_data=panel_models, default="rigid")
     parms_passed = parms_passed and _check_parms(panel_params, 'panel_margins', [float], acceptable_range=[0, 0.5], default=0.2)
     parms_passed = parms_passed and _check_parms(panel_params, 'parallel', [bool], default=False)
     parms_passed = parms_passed and _check_parms(panel_params, 'sel_ddi', [list, np.array], list_acceptable_data_types=[int, np.int], default='all')
     parms_passed = parms_passed and _check_parms(panel_params, 'overwrite', [bool], default=False)
```

### Comparing `astrohack-0.1.0/src/astrohack/profiling.py` & `astrohack-0.1.1/src/astrohack/profiling.py`

 * *Files identical despite different names*

### Comparing `astrohack-0.1.0/src/astrohack/visualization/viewer.py` & `astrohack-0.1.1/src/astrohack/visualization/viewer.py`

 * *Files identical despite different names*

### Comparing `astrohack-0.1.0/src/astrohack.egg-info/PKG-INFO` & `astrohack-0.1.1/src/astrohack.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: astrohack
-Version: 0.1.0
+Version: 0.1.1
 Summary: Holography Antenna Commissioning Kit
 Author-email: Jan-Willem Steeb <jsteeb@nrao.edu>, Joshua Hoskins <jhoskins@nrao.edu>, Victor de Souza Magalhaes <vdesouza@nrao.edu>
 Requires-Python: <3.11,>=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: docs
 License-File: LICENSE
```

### Comparing `astrohack-0.1.0/src/astrohack.egg-info/SOURCES.txt` & `astrohack-0.1.1/src/astrohack.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 LICENSE
 MANIFEST.in
 README.md
 README.rst
 pyproject.toml
 src/astrohack/__init__.py
 src/astrohack/astrohack_client.py
+src/astrohack/combine.py
 src/astrohack/dio.py
 src/astrohack/extract_holog.py
 src/astrohack/gdown_utils.py
 src/astrohack/holog.py
 src/astrohack/locit.py
 src/astrohack/panel.py
 src/astrohack/profiling.py
@@ -20,14 +21,15 @@
 src/astrohack/_classes/antenna_surface.py
 src/astrohack/_classes/base_panel.py
 src/astrohack/_classes/polygon_panel.py
 src/astrohack/_classes/ring_panel.py
 src/astrohack/_classes/telescope.py
 src/astrohack/_utils/__init__.py
 src/astrohack/_utils/_algorithms.py
+src/astrohack/_utils/_combine.py
 src/astrohack/_utils/_constants.py
 src/astrohack/_utils/_conversion.py
 src/astrohack/_utils/_dio.py
 src/astrohack/_utils/_extract_holog.py
 src/astrohack/_utils/_extract_point.py
 src/astrohack/_utils/_holog.py
 src/astrohack/_utils/_imaging.py
```

### Comparing `astrohack-0.1.0/src/astrohack.egg-info/requires.txt` & `astrohack-0.1.1/src/astrohack.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `astrohack-0.1.0/tests/test_class_antenna_surface.py` & `astrohack-0.1.1/tests/test_class_antenna_surface.py`

 * *Files identical despite different names*

### Comparing `astrohack-0.1.0/tests/test_class_base_panel.py` & `astrohack-0.1.1/tests/test_class_base_panel.py`

 * *Files 4% similar despite different names*

```diff
@@ -18,31 +18,31 @@
         vector = np.arange(size)
         for pos in range(size):
             assert _gauss_elimination_numpy(identity, vector)[pos] == vector[pos], 'Gaussian elimination failed'
 
     def test_init(self):
         screws = np.zeros([4, 2])
         label = 'TEST'
-        lepanel = BasePanel(panel_models[imean], screws, label)
+        lepanel = BasePanel(panel_models[imean], screws, screws, 0.1, label)
         assert lepanel.label == label, "Internal panel label not what expected"
         assert lepanel.model == panel_models[imean], "Internal model does not match input"
         assert lepanel.samples == [], 'List of samples should be empty'
         assert lepanel.margins == [], 'list of pixels in the margin should be empty'
         assert lepanel.corr is None, 'List of corrections should be None'
         assert not lepanel.solved, 'Panel cannot be solved at creation'
         with pytest.raises(Exception):
-            lepanel = BasePanel('xxx', screws, label)
+            lepanel = BasePanel('xxx', screws, screws, 0.1, label)
 
     def test_add_point(self):
         """
         Test the add point common function
         """
+        label = 'TEST'
         screws = np.zeros([4, 2])
-        ipanel = 0
-        lepanel = BasePanel(panel_models[imean], ipanel, screws)
+        lepanel = BasePanel(panel_models[imean], screws, screws, 0.1, label)
         nsamp = 30
         point = [0, 0, 0, 0, 0]
         for i in range(nsamp):
             lepanel.add_sample(point)
             lepanel.add_margin(point)
         assert len(lepanel.samples) == nsamp, 'Internal number of samples do not match the expected number of samples'
         assert len(lepanel.margins) == nsamp, 'Internal list of points does not have the expected size'
@@ -54,15 +54,15 @@
         """
         Tests the whole usage of a panel of the mean model
         """
         expectedmean = 3.5
         point = [0, 0, 0, 0, expectedmean]
         screws = np.zeros([4, 2])
         nsamp = 30
-        meanpanel = BasePanel(panel_models[imean], screws, 'test')
+        meanpanel = BasePanel(panel_models[imean], screws, screws, 0.1, 'test')
         assert meanpanel._solve_sub == meanpanel._solve_mean, 'Incorrect overloading of mean solving method'
         assert meanpanel.corr_point == meanpanel._corr_point_mean, 'Incorrect overloading of mean point correction ' \
                                                                    'method'
         for i in range(nsamp):
             meanpanel.add_sample(point)
         meanpanel.solve()
         assert abs(meanpanel.par[0] - expectedmean)/expectedmean < self.tolerance, 'Did not recover the expected mean'
@@ -85,15 +85,15 @@
     def test_rigid_model(self):
         """
         Tests the whole usage of a panel of the rigid model
         """
         expectedpar = [3.5, -2, 1]
         screws = np.zeros([4, 2])
         nside = 32
-        rigidpanel = BasePanel(panel_models[irigid], screws, 'test')
+        rigidpanel = BasePanel(panel_models[irigid], screws, screws, 0.1, 'test')
         assert rigidpanel._solve_sub == rigidpanel._solve_rigid, 'Incorrect overloading of rigid solving method'
         assert rigidpanel.corr_point == rigidpanel._corr_point_rigid, 'Incorrect overloading of rigid point ' \
                                                                       'correction method'
         for ix in range(nside):
             for iy in range(nside):
                 value = ix*expectedpar[0] + iy*expectedpar[1] + expectedpar[2]
                 rigidpanel.add_sample([ix, iy, ix, iy, value])
@@ -115,15 +115,15 @@
     def test_xyparaboloid_scipy_model(self):
         """
         Tests the whole usage of a panel of the xyparaboloid model
         """
         expectedpar = [150, 10, 2.5]
         screws = np.zeros([4, 2])
         nside = 32
-        xyparapanel = BasePanel(panel_models[ixypara], screws, 'test')
+        xyparapanel = BasePanel(panel_models[ixypara], screws, screws, 0.1, 'test')
         assert xyparapanel._solve_sub == xyparapanel._solve_scipy, 'Incorrect overloading of scipy solving method'
         assert xyparapanel.corr_point == xyparapanel._corr_point_scipy, 'Incorrect overloading of scipy point ' \
                                                                         'correction method'
         assert xyparapanel._fitting_function == xyparapanel._xyaxes_paraboloid, 'Incorrect overloading of XY '\
                                                                                 'paraboloid function'
         for ix in range(nside):
             for iy in range(nside):
@@ -148,15 +148,15 @@
         """
         Tests the whole usage of a panel of the rotatedparaboloid model
         """
         theta = 0
         expectedpar = [39, 10, 2.5, theta]
         screws = np.zeros([4, 2])
         nside = 32
-        rotparapanel = BasePanel(panel_models[irotpara], screws, 'test')
+        rotparapanel = BasePanel(panel_models[irotpara], screws, screws, 0.1, 'test')
         assert rotparapanel._solve_sub == rotparapanel._solve_scipy, 'Incorrect overloading of scipy solving method'
         assert rotparapanel.corr_point == rotparapanel._corr_point_scipy, 'Incorrect overloading of scipy point ' \
                                                                           'correction method'
         assert rotparapanel._fitting_function == rotparapanel._rotated_paraboloid, 'Incorrect overloading of paraboloid' \
                                                                                    ' function'
         for ix in range(nside):
             for iy in range(nside):
@@ -182,15 +182,15 @@
     def test_corotatedparaboloid_scipy_model(self):
         """
         Tests the whole usage of a panel of the corotatedparaboloid model solved with scipy
         """
         expectedpar = [75, 5, -2.0]
         screws = np.zeros([4, 2])
         nside = 32
-        corotparapanel = BasePanel(panel_models[icorscp], screws, 'test')
+        corotparapanel = BasePanel(panel_models[icorscp], screws, screws, 0.1, 'test')
         assert corotparapanel._solve_sub == corotparapanel._solve_scipy, 'Incorrect overloading of scipy solving method'
         assert corotparapanel.corr_point == corotparapanel._corr_point_scipy, 'Incorrect overloading of scipy point ' \
                                                                               'correction method'
         assert corotparapanel._fitting_function == corotparapanel._corotated_paraboloid, 'Incorrect overloading of ' \
                                                                                          'paraboloid function'
         for ix in range(nside):
             for iy in range(nside):
@@ -214,15 +214,15 @@
     def test_corotatedparaboloid_lst_model(self):
         """
         Tests the whole usage of a panel of the corotatedparaboloid model
         """
         expectedpar = [75, 5, -2.0]
         screws = np.zeros([4, 2])
         nside = 32
-        corotparapanel = BasePanel(panel_models[icorlst], screws, 'test')
+        corotparapanel = BasePanel(panel_models[icorlst], screws, screws, 0.1, 'test')
         assert corotparapanel._solve_sub == corotparapanel._solve_corotated_lst_sq, 'Incorrect overloading of ' \
                                                                                     'corotated least squares solving ' \
                                                                                     'method'
         assert corotparapanel.corr_point == corotparapanel._corr_point_corotated_lst_sq, 'Incorrect overloading of ' \
                                                                                          'corotated least squares ' \
                                                                                          'point correction method'
         for ix in range(nside):
@@ -247,15 +247,15 @@
     def test_corotatedparaboloid_robust_model(self):
         """
         Tests the whole usage of a panel of the corotatedparaboloid model
         """
         expectedpar = [75, 5, -2.0]
         screws = np.zeros([4, 2])
         nside = 32
-        corotparapanel = BasePanel(panel_models[icorrob], screws, 'test')
+        corotparapanel = BasePanel(panel_models[icorrob], screws, screws, 0.1, 'test')
         assert corotparapanel._solve_sub == corotparapanel._solve_robust, 'Incorrect overloading of robust solving ' \
                                                                           'method'
         assert corotparapanel.corr_point == corotparapanel._corr_point_corotated_lst_sq, 'Incorrect overloading of ' \
                                                                                          'corotated least squares ' \
                                                                                          'correction method'
         assert corotparapanel._fitting_function == corotparapanel._corotated_paraboloid, 'Incorrect overloading of ' \
                                                                                          'paraboloid function'
@@ -282,15 +282,15 @@
         """
         Tests the whole usage of a panel of the corotatedparaboloid model
         """
         expectedpar = [75, 5, -2.0, 3, -6, 8, 16, -3.5, 8]
         expectedscrew = 8000
         screws = np.zeros([4, 2])
         nside = 32
-        corotparapanel = BasePanel(panel_models[ifulllst], screws, 'test')
+        corotparapanel = BasePanel(panel_models[ifulllst], screws, screws, 0.1, 'test')
         assert corotparapanel._solve_sub == corotparapanel._solve_least_squares_paraboloid, 'Incorrect overloading of ' \
                                                                                             'full least squares ' \
                                                                                             'solving method'
         assert corotparapanel.corr_point == corotparapanel._corr_point_least_squares_paraboloid, 'Incorrect ' \
                                                                                                  'overloading of full' \
                                                                                                  ' least squares ' \
                                                                                                  'point correction ' \
```

### Comparing `astrohack-0.1.0/tests/test_class_ring_panel.py` & `astrohack-0.1.1/tests/test_class_ring_panel.py`

 * *Files identical despite different names*

### Comparing `astrohack-0.1.0/tests/test_class_telescope.py` & `astrohack-0.1.1/tests/test_class_telescope.py`

 * *Files identical despite different names*

