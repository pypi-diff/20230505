# Comparing `tmp/dask-cuda-23.6.0a230503.tar.gz` & `tmp/dask-cuda-23.6.0a230504.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dask-cuda-23.6.0a230503.tar", last modified: Wed May  3 05:02:19 2023, max compression
+gzip compressed data, was "dask-cuda-23.6.0a230504.tar", last modified: Fri May  5 05:02:21 2023, max compression
```

## Comparing `dask-cuda-23.6.0a230503.tar` & `dask-cuda-23.6.0a230504.tar`

### file list

```diff
@@ -1,67 +1,67 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 05:02:19.672383 dask-cuda-23.6.0a230503/
--rw-r--r--   0 root         (0) root         (0)    11348 2023-05-03 05:02:11.000000 dask-cuda-23.6.0a230503/LICENSE
--rw-r--r--   0 root         (0) root         (0)       30 2023-05-03 05:02:11.000000 dask-cuda-23.6.0a230503/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)     1924 2023-05-03 05:02:19.672383 dask-cuda-23.6.0a230503/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1115 2023-05-03 05:02:11.000000 dask-cuda-23.6.0a230503/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 05:02:19.672383 dask-cuda-23.6.0a230503/dask_cuda/
--rw-r--r--   0 root         (0) root         (0)     1522 2023-05-03 05:02:11.000000 dask-cuda-23.6.0a230503/dask_cuda/__init__.py
--rw-r--r--   0 root         (0) root         (0)      508 2023-05-03 05:02:19.672383 dask-cuda-23.6.0a230503/dask_cuda/_version.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 05:02:19.668383 dask-cuda-23.6.0a230503/dask_cuda/benchmarks/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-03 05:02:11.000000 dask-cuda-23.6.0a230503/dask_cuda/benchmarks/__init__.py
--rw-r--r--   0 root         (0) root         (0)     6393 2023-05-03 05:02:11.000000 dask-cuda-23.6.0a230503/dask_cuda/benchmarks/common.py
--rw-r--r--   0 root         (0) root         (0)     8894 2023-05-03 05:02:11.000000 dask-cuda-23.6.0a230503/dask_cuda/benchmarks/local_cudf_groupby.py
--rw-r--r--   0 root         (0) root         (0)    12437 2023-05-03 05:02:11.000000 dask-cuda-23.6.0a230503/dask_cuda/benchmarks/local_cudf_merge.py
--rw-r--r--   0 root         (0) root         (0)     8598 2023-05-03 05:02:11.000000 dask-cuda-23.6.0a230503/dask_cuda/benchmarks/local_cudf_shuffle.py
--rw-r--r--   0 root         (0) root         (0)    10752 2023-05-03 05:02:11.000000 dask-cuda-23.6.0a230503/dask_cuda/benchmarks/local_cupy.py
--rw-r--r--   0 root         (0) root         (0)     6432 2023-05-03 05:02:11.000000 dask-cuda-23.6.0a230503/dask_cuda/benchmarks/local_cupy_map_overlap.py
--rw-r--r--   0 root         (0) root         (0)    26888 2023-05-03 05:02:11.000000 dask-cuda-23.6.0a230503/dask_cuda/benchmarks/utils.py
--rw-r--r--   0 root         (0) root         (0)    15828 2023-05-03 05:02:11.000000 dask-cuda-23.6.0a230503/dask_cuda/cli.py
--rw-r--r--   0 root         (0) root         (0)     8589 2023-05-03 05:02:11.000000 dask-cuda-23.6.0a230503/dask_cuda/cuda_worker.py
--rw-r--r--   0 root         (0) root         (0)    11043 2023-05-03 05:02:11.000000 dask-cuda-23.6.0a230503/dask_cuda/device_host_file.py
--rw-r--r--   0 root         (0) root         (0)     6499 2023-05-03 05:02:11.000000 dask-cuda-23.6.0a230503/dask_cuda/disk_io.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 05:02:19.668383 dask-cuda-23.6.0a230503/dask_cuda/explicit_comms/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-03 05:02:11.000000 dask-cuda-23.6.0a230503/dask_cuda/explicit_comms/__init__.py
--rw-r--r--   0 root         (0) root         (0)    10478 2023-05-03 05:02:11.000000 dask-cuda-23.6.0a230503/dask_cuda/explicit_comms/comms.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 05:02:19.668383 dask-cuda-23.6.0a230503/dask_cuda/explicit_comms/dataframe/
--rw-r--r--   0 root         (0) root         (0)        0 2023-05-03 05:02:11.000000 dask-cuda-23.6.0a230503/dask_cuda/explicit_comms/dataframe/__init__.py
--rw-r--r--   0 root         (0) root         (0)    20062 2023-05-03 05:02:11.000000 dask-cuda-23.6.0a230503/dask_cuda/explicit_comms/dataframe/shuffle.py
--rw-r--r--   0 root         (0) root         (0)     3890 2023-05-03 05:02:11.000000 dask-cuda-23.6.0a230503/dask_cuda/get_device_memory_objects.py
--rw-r--r--   0 root         (0) root         (0)     5231 2023-05-03 05:02:11.000000 dask-cuda-23.6.0a230503/dask_cuda/initialize.py
--rw-r--r--   0 root         (0) root         (0)     1046 2023-05-03 05:02:11.000000 dask-cuda-23.6.0a230503/dask_cuda/is_device_object.py
--rw-r--r--   0 root         (0) root         (0)     1457 2023-05-03 05:02:11.000000 dask-cuda-23.6.0a230503/dask_cuda/is_spillable_object.py
--rw-r--r--   0 root         (0) root         (0)    17302 2023-05-03 05:02:11.000000 dask-cuda-23.6.0a230503/dask_cuda/local_cuda_cluster.py
--rw-r--r--   0 root         (0) root         (0)     8108 2023-05-03 05:02:11.000000 dask-cuda-23.6.0a230503/dask_cuda/proxify_device_objects.py
--rw-r--r--   0 root         (0) root         (0)    30850 2023-05-03 05:02:11.000000 dask-cuda-23.6.0a230503/dask_cuda/proxify_host_file.py
--rw-r--r--   0 root         (0) root         (0)    29880 2023-05-03 05:02:11.000000 dask-cuda-23.6.0a230503/dask_cuda/proxy_object.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 05:02:19.672383 dask-cuda-23.6.0a230503/dask_cuda/tests/
--rw-r--r--   0 root         (0) root         (0)     4910 2023-05-03 05:02:11.000000 dask-cuda-23.6.0a230503/dask_cuda/tests/test_cudf_builtin_spilling.py
--rw-r--r--   0 root         (0) root         (0)    15517 2023-05-03 05:02:11.000000 dask-cuda-23.6.0a230503/dask_cuda/tests/test_dask_cuda_worker.py
--rw-r--r--   0 root         (0) root         (0)     5882 2023-05-03 05:02:11.000000 dask-cuda-23.6.0a230503/dask_cuda/tests/test_device_host_file.py
--rw-r--r--   0 root         (0) root         (0)     6381 2023-05-03 05:02:11.000000 dask-cuda-23.6.0a230503/dask_cuda/tests/test_dgx.py
--rw-r--r--   0 root         (0) root         (0)    12036 2023-05-03 05:02:11.000000 dask-cuda-23.6.0a230503/dask_cuda/tests/test_explicit_comms.py
--rw-r--r--   0 root         (0) root         (0)     1513 2023-05-03 05:02:11.000000 dask-cuda-23.6.0a230503/dask_cuda/tests/test_gds.py
--rw-r--r--   0 root         (0) root         (0)     5235 2023-05-03 05:02:11.000000 dask-cuda-23.6.0a230503/dask_cuda/tests/test_initialize.py
--rw-r--r--   0 root         (0) root         (0)    15675 2023-05-03 05:02:11.000000 dask-cuda-23.6.0a230503/dask_cuda/tests/test_local_cuda_cluster.py
--rw-r--r--   0 root         (0) root         (0)    18492 2023-05-03 05:02:11.000000 dask-cuda-23.6.0a230503/dask_cuda/tests/test_proxify_host_file.py
--rw-r--r--   0 root         (0) root         (0)    23464 2023-05-03 05:02:11.000000 dask-cuda-23.6.0a230503/dask_cuda/tests/test_proxy.py
--rw-r--r--   0 root         (0) root         (0)     9386 2023-05-03 05:02:11.000000 dask-cuda-23.6.0a230503/dask_cuda/tests/test_spill.py
--rw-r--r--   0 root         (0) root         (0)     8832 2023-05-03 05:02:11.000000 dask-cuda-23.6.0a230503/dask_cuda/tests/test_utils.py
--rw-r--r--   0 root         (0) root         (0)     2399 2023-05-03 05:02:11.000000 dask-cuda-23.6.0a230503/dask_cuda/tests/test_worker_spec.py
--rw-r--r--   0 root         (0) root         (0)    29112 2023-05-03 05:02:11.000000 dask-cuda-23.6.0a230503/dask_cuda/utils.py
--rw-r--r--   0 root         (0) root         (0)     4356 2023-05-03 05:02:11.000000 dask-cuda-23.6.0a230503/dask_cuda/worker_spec.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 05:02:19.664383 dask-cuda-23.6.0a230503/dask_cuda.egg-info/
--rw-r--r--   0 root         (0) root         (0)     1924 2023-05-03 05:02:19.000000 dask-cuda-23.6.0a230503/dask_cuda.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1702 2023-05-03 05:02:19.000000 dask-cuda-23.6.0a230503/dask_cuda.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-03 05:02:19.000000 dask-cuda-23.6.0a230503/dask_cuda.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      136 2023-05-03 05:02:19.000000 dask-cuda-23.6.0a230503/dask_cuda.egg-info/entry_points.txt
--rw-r--r--   0 root         (0) root         (0)      209 2023-05-03 05:02:19.000000 dask-cuda-23.6.0a230503/dask_cuda.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       37 2023-05-03 05:02:19.000000 dask-cuda-23.6.0a230503/dask_cuda.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 05:02:19.656383 dask-cuda-23.6.0a230503/examples/
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 05:02:19.672383 dask-cuda-23.6.0a230503/examples/ucx/
--rw-r--r--   0 root         (0) root         (0)     1262 2023-05-03 05:02:11.000000 dask-cuda-23.6.0a230503/examples/ucx/client_initialize.py
--rw-r--r--   0 root         (0) root         (0)     1983 2023-05-03 05:02:11.000000 dask-cuda-23.6.0a230503/examples/ucx/local_cuda_cluster.py
--rw-r--r--   0 root         (0) root         (0)     3152 2023-05-03 05:02:11.000000 dask-cuda-23.6.0a230503/pyproject.toml
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-03 05:02:19.672383 dask-cuda-23.6.0a230503/rtd/
--rw-r--r--   0 root         (0) root         (0)     6223 2023-05-03 05:02:11.000000 dask-cuda-23.6.0a230503/rtd/conf.py
--rw-r--r--   0 root         (0) root         (0)       38 2023-05-03 05:02:19.672383 dask-cuda-23.6.0a230503/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      953 2023-05-03 05:02:11.000000 dask-cuda-23.6.0a230503/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 05:02:21.065800 dask-cuda-23.6.0a230504/
+-rw-r--r--   0 root         (0) root         (0)    11348 2023-05-05 05:02:12.000000 dask-cuda-23.6.0a230504/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       30 2023-05-05 05:02:12.000000 dask-cuda-23.6.0a230504/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     1924 2023-05-05 05:02:21.061800 dask-cuda-23.6.0a230504/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1115 2023-05-05 05:02:12.000000 dask-cuda-23.6.0a230504/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 05:02:21.065800 dask-cuda-23.6.0a230504/dask_cuda/
+-rw-r--r--   0 root         (0) root         (0)     1522 2023-05-05 05:02:12.000000 dask-cuda-23.6.0a230504/dask_cuda/__init__.py
+-rw-r--r--   0 root         (0) root         (0)      508 2023-05-05 05:02:21.065800 dask-cuda-23.6.0a230504/dask_cuda/_version.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 05:02:21.057799 dask-cuda-23.6.0a230504/dask_cuda/benchmarks/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-05 05:02:12.000000 dask-cuda-23.6.0a230504/dask_cuda/benchmarks/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     6393 2023-05-05 05:02:12.000000 dask-cuda-23.6.0a230504/dask_cuda/benchmarks/common.py
+-rw-r--r--   0 root         (0) root         (0)     8894 2023-05-05 05:02:12.000000 dask-cuda-23.6.0a230504/dask_cuda/benchmarks/local_cudf_groupby.py
+-rw-r--r--   0 root         (0) root         (0)    12437 2023-05-05 05:02:12.000000 dask-cuda-23.6.0a230504/dask_cuda/benchmarks/local_cudf_merge.py
+-rw-r--r--   0 root         (0) root         (0)     8598 2023-05-05 05:02:12.000000 dask-cuda-23.6.0a230504/dask_cuda/benchmarks/local_cudf_shuffle.py
+-rw-r--r--   0 root         (0) root         (0)    10752 2023-05-05 05:02:12.000000 dask-cuda-23.6.0a230504/dask_cuda/benchmarks/local_cupy.py
+-rw-r--r--   0 root         (0) root         (0)     6432 2023-05-05 05:02:12.000000 dask-cuda-23.6.0a230504/dask_cuda/benchmarks/local_cupy_map_overlap.py
+-rw-r--r--   0 root         (0) root         (0)    26888 2023-05-05 05:02:12.000000 dask-cuda-23.6.0a230504/dask_cuda/benchmarks/utils.py
+-rw-r--r--   0 root         (0) root         (0)    15828 2023-05-05 05:02:12.000000 dask-cuda-23.6.0a230504/dask_cuda/cli.py
+-rw-r--r--   0 root         (0) root         (0)     8589 2023-05-05 05:02:12.000000 dask-cuda-23.6.0a230504/dask_cuda/cuda_worker.py
+-rw-r--r--   0 root         (0) root         (0)     9856 2023-05-05 05:02:12.000000 dask-cuda-23.6.0a230504/dask_cuda/device_host_file.py
+-rw-r--r--   0 root         (0) root         (0)     6499 2023-05-05 05:02:12.000000 dask-cuda-23.6.0a230504/dask_cuda/disk_io.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 05:02:21.057799 dask-cuda-23.6.0a230504/dask_cuda/explicit_comms/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-05 05:02:12.000000 dask-cuda-23.6.0a230504/dask_cuda/explicit_comms/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    10478 2023-05-05 05:02:12.000000 dask-cuda-23.6.0a230504/dask_cuda/explicit_comms/comms.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 05:02:21.057799 dask-cuda-23.6.0a230504/dask_cuda/explicit_comms/dataframe/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-05-05 05:02:12.000000 dask-cuda-23.6.0a230504/dask_cuda/explicit_comms/dataframe/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    20062 2023-05-05 05:02:12.000000 dask-cuda-23.6.0a230504/dask_cuda/explicit_comms/dataframe/shuffle.py
+-rw-r--r--   0 root         (0) root         (0)     3890 2023-05-05 05:02:12.000000 dask-cuda-23.6.0a230504/dask_cuda/get_device_memory_objects.py
+-rw-r--r--   0 root         (0) root         (0)     5231 2023-05-05 05:02:12.000000 dask-cuda-23.6.0a230504/dask_cuda/initialize.py
+-rw-r--r--   0 root         (0) root         (0)     1046 2023-05-05 05:02:12.000000 dask-cuda-23.6.0a230504/dask_cuda/is_device_object.py
+-rw-r--r--   0 root         (0) root         (0)     1457 2023-05-05 05:02:12.000000 dask-cuda-23.6.0a230504/dask_cuda/is_spillable_object.py
+-rw-r--r--   0 root         (0) root         (0)    17302 2023-05-05 05:02:12.000000 dask-cuda-23.6.0a230504/dask_cuda/local_cuda_cluster.py
+-rw-r--r--   0 root         (0) root         (0)     8108 2023-05-05 05:02:12.000000 dask-cuda-23.6.0a230504/dask_cuda/proxify_device_objects.py
+-rw-r--r--   0 root         (0) root         (0)    30850 2023-05-05 05:02:12.000000 dask-cuda-23.6.0a230504/dask_cuda/proxify_host_file.py
+-rw-r--r--   0 root         (0) root         (0)    29880 2023-05-05 05:02:12.000000 dask-cuda-23.6.0a230504/dask_cuda/proxy_object.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 05:02:21.061800 dask-cuda-23.6.0a230504/dask_cuda/tests/
+-rw-r--r--   0 root         (0) root         (0)     4910 2023-05-05 05:02:12.000000 dask-cuda-23.6.0a230504/dask_cuda/tests/test_cudf_builtin_spilling.py
+-rw-r--r--   0 root         (0) root         (0)    15517 2023-05-05 05:02:12.000000 dask-cuda-23.6.0a230504/dask_cuda/tests/test_dask_cuda_worker.py
+-rw-r--r--   0 root         (0) root         (0)     5882 2023-05-05 05:02:12.000000 dask-cuda-23.6.0a230504/dask_cuda/tests/test_device_host_file.py
+-rw-r--r--   0 root         (0) root         (0)     6381 2023-05-05 05:02:12.000000 dask-cuda-23.6.0a230504/dask_cuda/tests/test_dgx.py
+-rw-r--r--   0 root         (0) root         (0)    12036 2023-05-05 05:02:12.000000 dask-cuda-23.6.0a230504/dask_cuda/tests/test_explicit_comms.py
+-rw-r--r--   0 root         (0) root         (0)     1513 2023-05-05 05:02:12.000000 dask-cuda-23.6.0a230504/dask_cuda/tests/test_gds.py
+-rw-r--r--   0 root         (0) root         (0)     5235 2023-05-05 05:02:12.000000 dask-cuda-23.6.0a230504/dask_cuda/tests/test_initialize.py
+-rw-r--r--   0 root         (0) root         (0)    15675 2023-05-05 05:02:12.000000 dask-cuda-23.6.0a230504/dask_cuda/tests/test_local_cuda_cluster.py
+-rw-r--r--   0 root         (0) root         (0)    18492 2023-05-05 05:02:12.000000 dask-cuda-23.6.0a230504/dask_cuda/tests/test_proxify_host_file.py
+-rw-r--r--   0 root         (0) root         (0)    23464 2023-05-05 05:02:12.000000 dask-cuda-23.6.0a230504/dask_cuda/tests/test_proxy.py
+-rw-r--r--   0 root         (0) root         (0)     9386 2023-05-05 05:02:12.000000 dask-cuda-23.6.0a230504/dask_cuda/tests/test_spill.py
+-rw-r--r--   0 root         (0) root         (0)     8832 2023-05-05 05:02:12.000000 dask-cuda-23.6.0a230504/dask_cuda/tests/test_utils.py
+-rw-r--r--   0 root         (0) root         (0)     2399 2023-05-05 05:02:12.000000 dask-cuda-23.6.0a230504/dask_cuda/tests/test_worker_spec.py
+-rw-r--r--   0 root         (0) root         (0)    29112 2023-05-05 05:02:12.000000 dask-cuda-23.6.0a230504/dask_cuda/utils.py
+-rw-r--r--   0 root         (0) root         (0)     4356 2023-05-05 05:02:12.000000 dask-cuda-23.6.0a230504/dask_cuda/worker_spec.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 05:02:21.053799 dask-cuda-23.6.0a230504/dask_cuda.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     1924 2023-05-05 05:02:21.000000 dask-cuda-23.6.0a230504/dask_cuda.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1702 2023-05-05 05:02:21.000000 dask-cuda-23.6.0a230504/dask_cuda.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-05 05:02:21.000000 dask-cuda-23.6.0a230504/dask_cuda.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      136 2023-05-05 05:02:21.000000 dask-cuda-23.6.0a230504/dask_cuda.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)      209 2023-05-05 05:02:21.000000 dask-cuda-23.6.0a230504/dask_cuda.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       37 2023-05-05 05:02:21.000000 dask-cuda-23.6.0a230504/dask_cuda.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 05:02:21.045799 dask-cuda-23.6.0a230504/examples/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 05:02:21.061800 dask-cuda-23.6.0a230504/examples/ucx/
+-rw-r--r--   0 root         (0) root         (0)     1262 2023-05-05 05:02:12.000000 dask-cuda-23.6.0a230504/examples/ucx/client_initialize.py
+-rw-r--r--   0 root         (0) root         (0)     1983 2023-05-05 05:02:12.000000 dask-cuda-23.6.0a230504/examples/ucx/local_cuda_cluster.py
+-rw-r--r--   0 root         (0) root         (0)     3152 2023-05-05 05:02:12.000000 dask-cuda-23.6.0a230504/pyproject.toml
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 05:02:21.061800 dask-cuda-23.6.0a230504/rtd/
+-rw-r--r--   0 root         (0) root         (0)     6223 2023-05-05 05:02:12.000000 dask-cuda-23.6.0a230504/rtd/conf.py
+-rw-r--r--   0 root         (0) root         (0)       38 2023-05-05 05:02:21.065800 dask-cuda-23.6.0a230504/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      953 2023-05-05 05:02:12.000000 dask-cuda-23.6.0a230504/setup.py
```

### Comparing `dask-cuda-23.6.0a230503/LICENSE` & `dask-cuda-23.6.0a230504/LICENSE`

 * *Files identical despite different names*

### Comparing `dask-cuda-23.6.0a230503/PKG-INFO` & `dask-cuda-23.6.0a230504/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: dask-cuda
-Version: 23.6.0a230503
+Version: 23.6.0a230504
 Summary: Utilities for Dask and CUDA interactions
 Author: NVIDIA Corporation
 License: Apache-2.0
 Project-URL: Homepage, https://github.com/rapidsai/dask-cuda
 Project-URL: Documentation, https://docs.rapids.ai/api/dask-cuda/stable/
 Project-URL: Source, https://github.com/rapidsai/dask-cuda
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Database
 Classifier: Topic :: Scientific/Engineering
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
-Requires-Python: >=3.8
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Provides-Extra: docs
 Provides-Extra: test
 License-File: LICENSE
 
 [![RTD](https://readthedocs.org/projects/dask-cuda/badge/?version=latest)](https://dask-cuda.readthedocs.io/en/latest/?badge=latest)
```

### Comparing `dask-cuda-23.6.0a230503/README.md` & `dask-cuda-23.6.0a230504/README.md`

 * *Files identical despite different names*

### Comparing `dask-cuda-23.6.0a230503/dask_cuda/__init__.py` & `dask-cuda-23.6.0a230504/dask_cuda/__init__.py`

 * *Files identical despite different names*

### Comparing `dask-cuda-23.6.0a230503/dask_cuda/benchmarks/common.py` & `dask-cuda-23.6.0a230504/dask_cuda/benchmarks/common.py`

 * *Files identical despite different names*

### Comparing `dask-cuda-23.6.0a230503/dask_cuda/benchmarks/local_cudf_groupby.py` & `dask-cuda-23.6.0a230504/dask_cuda/benchmarks/local_cudf_groupby.py`

 * *Files identical despite different names*

### Comparing `dask-cuda-23.6.0a230503/dask_cuda/benchmarks/local_cudf_merge.py` & `dask-cuda-23.6.0a230504/dask_cuda/benchmarks/local_cudf_merge.py`

 * *Files identical despite different names*

### Comparing `dask-cuda-23.6.0a230503/dask_cuda/benchmarks/local_cudf_shuffle.py` & `dask-cuda-23.6.0a230504/dask_cuda/benchmarks/local_cudf_shuffle.py`

 * *Files identical despite different names*

### Comparing `dask-cuda-23.6.0a230503/dask_cuda/benchmarks/local_cupy.py` & `dask-cuda-23.6.0a230504/dask_cuda/benchmarks/local_cupy.py`

 * *Files identical despite different names*

### Comparing `dask-cuda-23.6.0a230503/dask_cuda/benchmarks/local_cupy_map_overlap.py` & `dask-cuda-23.6.0a230504/dask_cuda/benchmarks/local_cupy_map_overlap.py`

 * *Files identical despite different names*

### Comparing `dask-cuda-23.6.0a230503/dask_cuda/benchmarks/utils.py` & `dask-cuda-23.6.0a230504/dask_cuda/benchmarks/utils.py`

 * *Files identical despite different names*

### Comparing `dask-cuda-23.6.0a230503/dask_cuda/cli.py` & `dask-cuda-23.6.0a230504/dask_cuda/cli.py`

 * *Files identical despite different names*

### Comparing `dask-cuda-23.6.0a230503/dask_cuda/cuda_worker.py` & `dask-cuda-23.6.0a230504/dask_cuda/cuda_worker.py`

 * *Files identical despite different names*

### Comparing `dask-cuda-23.6.0a230503/dask_cuda/device_host_file.py` & `dask-cuda-23.6.0a230504/dask_cuda/device_host_file.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,12 +1,11 @@
 import functools
 import itertools
 import logging
 import os
-import sys
 import time
 
 import numpy
 from zict import Buffer, File, Func
 from zict.common import ZictBase
 
 from distributed.protocol import (
@@ -236,42 +235,14 @@
 
         # For Worker compatibility only, where `fast` is host memory buffer
         self.fast = self.host_buffer if memory_limit is None else self.host_buffer.fast
 
         # Dict of objects that will not be spilled by DeviceHostFile.
         self.others = {}
 
-    if sys.version_info < (3, 9):
-
-        def __new__(
-            cls,
-            # So named such that dask will pass in the worker's local
-            # directory when constructing this through the "data" callback.
-            worker_local_directory,
-            *,
-            device_memory_limit=None,
-            memory_limit=None,
-            log_spilling=False,
-        ):
-            """
-            This is here to support Python 3.8. Right now (to support
-            3.8), ZictBase inherits from typing.MutableMapping through
-            which inspect.signature determines that the signature of
-            __init__ is just (*args, **kwargs). We need to advertise the
-            correct signature so that distributed will correctly figure
-            out that it needs to pass the worker's local directory. In
-            Python 3.9 and later, typing.MutableMapping is just an alias
-            for collections.abc.MutableMapping and we don't need to do
-            anything.
-
-            With this pass-through definition of __new__, the
-            signature of the constructor is correctly determined.
-            """
-            return super().__new__(cls)
-
     def __setitem__(self, key, value):
         if key in self.device_buffer:
             # Make sure we register the removal of an existing key
             del self[key]
 
         if is_spillable_object(value):
             self.others[key] = value
```

### Comparing `dask-cuda-23.6.0a230503/dask_cuda/disk_io.py` & `dask-cuda-23.6.0a230504/dask_cuda/disk_io.py`

 * *Files identical despite different names*

### Comparing `dask-cuda-23.6.0a230503/dask_cuda/explicit_comms/comms.py` & `dask-cuda-23.6.0a230504/dask_cuda/explicit_comms/comms.py`

 * *Files identical despite different names*

### Comparing `dask-cuda-23.6.0a230503/dask_cuda/explicit_comms/dataframe/shuffle.py` & `dask-cuda-23.6.0a230504/dask_cuda/explicit_comms/dataframe/shuffle.py`

 * *Files identical despite different names*

### Comparing `dask-cuda-23.6.0a230503/dask_cuda/get_device_memory_objects.py` & `dask-cuda-23.6.0a230504/dask_cuda/get_device_memory_objects.py`

 * *Files identical despite different names*

### Comparing `dask-cuda-23.6.0a230503/dask_cuda/initialize.py` & `dask-cuda-23.6.0a230504/dask_cuda/initialize.py`

 * *Files identical despite different names*

### Comparing `dask-cuda-23.6.0a230503/dask_cuda/is_device_object.py` & `dask-cuda-23.6.0a230504/dask_cuda/is_device_object.py`

 * *Files identical despite different names*

### Comparing `dask-cuda-23.6.0a230503/dask_cuda/is_spillable_object.py` & `dask-cuda-23.6.0a230504/dask_cuda/is_spillable_object.py`

 * *Files identical despite different names*

### Comparing `dask-cuda-23.6.0a230503/dask_cuda/local_cuda_cluster.py` & `dask-cuda-23.6.0a230504/dask_cuda/local_cuda_cluster.py`

 * *Files identical despite different names*

### Comparing `dask-cuda-23.6.0a230503/dask_cuda/proxify_device_objects.py` & `dask-cuda-23.6.0a230504/dask_cuda/proxify_device_objects.py`

 * *Files identical despite different names*

### Comparing `dask-cuda-23.6.0a230503/dask_cuda/proxify_host_file.py` & `dask-cuda-23.6.0a230504/dask_cuda/proxify_host_file.py`

 * *Files identical despite different names*

### Comparing `dask-cuda-23.6.0a230503/dask_cuda/proxy_object.py` & `dask-cuda-23.6.0a230504/dask_cuda/proxy_object.py`

 * *Files identical despite different names*

### Comparing `dask-cuda-23.6.0a230503/dask_cuda/tests/test_cudf_builtin_spilling.py` & `dask-cuda-23.6.0a230504/dask_cuda/tests/test_cudf_builtin_spilling.py`

 * *Files identical despite different names*

### Comparing `dask-cuda-23.6.0a230503/dask_cuda/tests/test_dask_cuda_worker.py` & `dask-cuda-23.6.0a230504/dask_cuda/tests/test_dask_cuda_worker.py`

 * *Files identical despite different names*

### Comparing `dask-cuda-23.6.0a230503/dask_cuda/tests/test_device_host_file.py` & `dask-cuda-23.6.0a230504/dask_cuda/tests/test_device_host_file.py`

 * *Files identical despite different names*

### Comparing `dask-cuda-23.6.0a230503/dask_cuda/tests/test_dgx.py` & `dask-cuda-23.6.0a230504/dask_cuda/tests/test_dgx.py`

 * *Files identical despite different names*

### Comparing `dask-cuda-23.6.0a230503/dask_cuda/tests/test_explicit_comms.py` & `dask-cuda-23.6.0a230504/dask_cuda/tests/test_explicit_comms.py`

 * *Files identical despite different names*

### Comparing `dask-cuda-23.6.0a230503/dask_cuda/tests/test_gds.py` & `dask-cuda-23.6.0a230504/dask_cuda/tests/test_gds.py`

 * *Files identical despite different names*

### Comparing `dask-cuda-23.6.0a230503/dask_cuda/tests/test_initialize.py` & `dask-cuda-23.6.0a230504/dask_cuda/tests/test_initialize.py`

 * *Files identical despite different names*

### Comparing `dask-cuda-23.6.0a230503/dask_cuda/tests/test_local_cuda_cluster.py` & `dask-cuda-23.6.0a230504/dask_cuda/tests/test_local_cuda_cluster.py`

 * *Files identical despite different names*

### Comparing `dask-cuda-23.6.0a230503/dask_cuda/tests/test_proxify_host_file.py` & `dask-cuda-23.6.0a230504/dask_cuda/tests/test_proxify_host_file.py`

 * *Files identical despite different names*

### Comparing `dask-cuda-23.6.0a230503/dask_cuda/tests/test_proxy.py` & `dask-cuda-23.6.0a230504/dask_cuda/tests/test_proxy.py`

 * *Files identical despite different names*

### Comparing `dask-cuda-23.6.0a230503/dask_cuda/tests/test_spill.py` & `dask-cuda-23.6.0a230504/dask_cuda/tests/test_spill.py`

 * *Files identical despite different names*

### Comparing `dask-cuda-23.6.0a230503/dask_cuda/tests/test_utils.py` & `dask-cuda-23.6.0a230504/dask_cuda/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `dask-cuda-23.6.0a230503/dask_cuda/tests/test_worker_spec.py` & `dask-cuda-23.6.0a230504/dask_cuda/tests/test_worker_spec.py`

 * *Files identical despite different names*

### Comparing `dask-cuda-23.6.0a230503/dask_cuda/utils.py` & `dask-cuda-23.6.0a230504/dask_cuda/utils.py`

 * *Files identical despite different names*

### Comparing `dask-cuda-23.6.0a230503/dask_cuda/worker_spec.py` & `dask-cuda-23.6.0a230504/dask_cuda/worker_spec.py`

 * *Files identical despite different names*

### Comparing `dask-cuda-23.6.0a230503/dask_cuda.egg-info/PKG-INFO` & `dask-cuda-23.6.0a230504/dask_cuda.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 Metadata-Version: 2.1
 Name: dask-cuda
-Version: 23.6.0a230503
+Version: 23.6.0a230504
 Summary: Utilities for Dask and CUDA interactions
 Author: NVIDIA Corporation
 License: Apache-2.0
 Project-URL: Homepage, https://github.com/rapidsai/dask-cuda
 Project-URL: Documentation, https://docs.rapids.ai/api/dask-cuda/stable/
 Project-URL: Source, https://github.com/rapidsai/dask-cuda
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Database
 Classifier: Topic :: Scientific/Engineering
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
-Requires-Python: >=3.8
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 Provides-Extra: docs
 Provides-Extra: test
 License-File: LICENSE
 
 [![RTD](https://readthedocs.org/projects/dask-cuda/badge/?version=latest)](https://dask-cuda.readthedocs.io/en/latest/?badge=latest)
```

### Comparing `dask-cuda-23.6.0a230503/dask_cuda.egg-info/SOURCES.txt` & `dask-cuda-23.6.0a230504/dask_cuda.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dask-cuda-23.6.0a230503/examples/ucx/client_initialize.py` & `dask-cuda-23.6.0a230504/examples/ucx/client_initialize.py`

 * *Files identical despite different names*

### Comparing `dask-cuda-23.6.0a230503/examples/ucx/local_cuda_cluster.py` & `dask-cuda-23.6.0a230504/examples/ucx/local_cuda_cluster.py`

 * *Files identical despite different names*

### Comparing `dask-cuda-23.6.0a230503/pyproject.toml` & `dask-cuda-23.6.0a230504/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 ]
 description = "Utilities for Dask and CUDA interactions"
 readme = { file = "README.md", content-type = "text/markdown" }
 authors = [
     { name = "NVIDIA Corporation" },
 ]
 license = { text = "Apache-2.0" }
-requires-python = ">=3.8"
+requires-python = ">=3.9"
 dependencies = [
     "dask ==2023.3.2",
     "distributed ==2023.3.2.1",
     "pynvml >=11.0.0,<11.5",
     "numpy >=1.21",
     "numba >=0.54",
     "pandas >=1.3,<1.6.0dev0",
```

### Comparing `dask-cuda-23.6.0a230503/rtd/conf.py` & `dask-cuda-23.6.0a230504/rtd/conf.py`

 * *Files identical despite different names*

### Comparing `dask-cuda-23.6.0a230503/setup.py` & `dask-cuda-23.6.0a230504/setup.py`

 * *Files identical despite different names*

