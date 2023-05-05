# Comparing `tmp/sarus-0.6.0.tar.gz` & `tmp/sarus-0.6.0.dev0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sarus-0.6.0.tar", last modified: Fri May  5 06:37:29 2023, max compression
+gzip compressed data, was "dist/sarus-0.6.0.dev0.tar", last modified: Tue May  2 06:50:18 2023, max compression
```

## Comparing `sarus-0.6.0.tar` & `sarus-0.6.0.dev0.tar`

### file list

```diff
@@ -1,103 +1,101 @@
-drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2023-05-05 06:37:29.783113 sarus-0.6.0/
--rw-rw-r--   0 vincent   (1000) vincent   (1000)       25 2022-09-14 12:56:20.000000 sarus-0.6.0/MANIFEST.in
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     1553 2023-05-05 06:37:29.787113 sarus-0.6.0/PKG-INFO
--rw-rw-r--   0 vincent   (1000) vincent   (1000)      663 2021-08-24 10:18:30.000000 sarus-0.6.0/README.rst
--rw-rw-r--   0 vincent   (1000) vincent   (1000)      100 2021-09-06 19:14:48.000000 sarus-0.6.0/pyproject.toml
-drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2023-05-05 06:37:29.771113 sarus-0.6.0/sarus/
--rw-rw-r--   0 vincent   (1000) vincent   (1000)      544 2023-05-05 06:36:51.000000 sarus-0.6.0/sarus/__init__.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)    13051 2023-04-21 19:49:48.000000 sarus-0.6.0/sarus/config.yaml
-drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2023-05-05 06:37:29.771113 sarus-0.6.0/sarus/context/
--rw-rw-r--   0 vincent   (1000) vincent   (1000)        0 2022-09-14 12:56:20.000000 sarus-0.6.0/sarus/context/__init__.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     3069 2023-05-05 06:32:20.000000 sarus-0.6.0/sarus/context/local_sdk.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)      302 2023-05-05 06:32:20.000000 sarus-0.6.0/sarus/context/typing.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)    14156 2023-05-05 06:32:20.000000 sarus-0.6.0/sarus/dataspec_wrapper.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)      743 2023-04-21 19:49:48.000000 sarus-0.6.0/sarus/debug.py
-drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2023-05-05 06:37:29.771113 sarus-0.6.0/sarus/imblearn/
--rw-rw-r--   0 vincent   (1000) vincent   (1000)      265 2022-11-29 13:03:29.000000 sarus-0.6.0/sarus/imblearn/__init__.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)      578 2022-11-29 13:03:29.000000 sarus-0.6.0/sarus/imblearn/over_sampling.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)      558 2022-11-29 13:03:29.000000 sarus-0.6.0/sarus/imblearn/pipeline.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)      556 2022-11-29 13:03:29.000000 sarus-0.6.0/sarus/imblearn/under_sampling.py
-drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2023-05-05 06:37:29.771113 sarus-0.6.0/sarus/legacy/
--rw-rw-r--   0 vincent   (1000) vincent   (1000)       42 2022-11-29 13:03:29.000000 sarus-0.6.0/sarus/legacy/__init__.py
-drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2023-05-05 06:37:29.775113 sarus-0.6.0/sarus/legacy/pandas/
--rw-rw-r--   0 vincent   (1000) vincent   (1000)      100 2023-01-27 14:38:46.000000 sarus-0.6.0/sarus/legacy/pandas/__init__.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)    16606 2023-01-27 14:38:46.000000 sarus-0.6.0/sarus/legacy/pandas/dataframe.py
-drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2023-05-05 06:37:29.775113 sarus-0.6.0/sarus/legacy/tensorflow/
--rw-rw-r--   0 vincent   (1000) vincent   (1000)      132 2022-09-14 12:56:20.000000 sarus-0.6.0/sarus/legacy/tensorflow/__init__.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)    13194 2022-12-01 13:21:20.000000 sarus-0.6.0/sarus/legacy/tensorflow/dataset.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)    42361 2022-11-29 13:03:29.000000 sarus-0.6.0/sarus/legacy/tensorflow/model.py
-drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2023-05-05 06:37:29.775113 sarus-0.6.0/sarus/manager/
--rw-rw-r--   0 vincent   (1000) vincent   (1000)        0 2022-09-14 12:56:20.000000 sarus-0.6.0/sarus/manager/__init__.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     5360 2023-05-05 06:32:20.000000 sarus-0.6.0/sarus/manager/arrow_local.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     1949 2023-05-05 06:32:20.000000 sarus-0.6.0/sarus/manager/arrow_remote.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     3733 2023-05-05 06:32:20.000000 sarus-0.6.0/sarus/manager/cache_scalar_local.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     6201 2023-05-05 06:32:20.000000 sarus-0.6.0/sarus/manager/dataspec_api.py
-drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2023-05-05 06:37:29.775113 sarus-0.6.0/sarus/manager/ops/
--rw-rw-r--   0 vincent   (1000) vincent   (1000)        0 2022-09-14 12:56:20.000000 sarus-0.6.0/sarus/manager/ops/__init__.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)      921 2023-04-21 19:49:48.000000 sarus-0.6.0/sarus/manager/ops/api.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     3352 2023-05-05 06:32:20.000000 sarus-0.6.0/sarus/manager/parquet_local.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)    19293 2023-05-05 06:32:20.000000 sarus-0.6.0/sarus/manager/sdk_manager.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     2556 2023-05-04 12:45:45.000000 sarus-0.6.0/sarus/manager/typing.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     4599 2023-05-05 06:32:20.000000 sarus-0.6.0/sarus/manager/value_local.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     1595 2023-05-05 06:32:20.000000 sarus-0.6.0/sarus/manager/value_remote.py
-drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2023-05-05 06:37:29.775113 sarus-0.6.0/sarus/numpy/
--rw-rw-r--   0 vincent   (1000) vincent   (1000)      337 2022-09-14 12:56:20.000000 sarus-0.6.0/sarus/numpy/__init__.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)       81 2022-09-14 12:56:20.000000 sarus-0.6.0/sarus/numpy/random.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)      963 2022-09-14 12:56:20.000000 sarus-0.6.0/sarus/numpy/scalars.py
-drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2023-05-05 06:37:29.779113 sarus-0.6.0/sarus/pandas/
--rw-rw-r--   0 vincent   (1000) vincent   (1000)      197 2022-11-29 13:03:29.000000 sarus-0.6.0/sarus/pandas/__init__.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)      822 2022-11-29 13:03:29.000000 sarus-0.6.0/sarus/pandas/core.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     4918 2023-04-21 19:49:48.000000 sarus-0.6.0/sarus/pandas/dataframe.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)      206 2022-11-29 13:03:29.000000 sarus-0.6.0/sarus/pandas/io.py
-drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2023-05-05 06:37:29.779113 sarus-0.6.0/sarus/pandas_profiling/
--rw-rw-r--   0 vincent   (1000) vincent   (1000)       81 2022-09-14 12:56:20.000000 sarus-0.6.0/sarus/pandas_profiling/__init__.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)      841 2023-05-05 06:32:20.000000 sarus-0.6.0/sarus/pandas_profiling/profile_report.py
-drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2023-05-05 06:37:29.779113 sarus-0.6.0/sarus/plotly/
--rw-rw-r--   0 vincent   (1000) vincent   (1000)      108 2022-09-14 12:56:20.000000 sarus-0.6.0/sarus/plotly/__init__.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)      138 2022-09-14 12:56:20.000000 sarus-0.6.0/sarus/plotly/express.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)    55988 2023-05-05 06:32:20.000000 sarus-0.6.0/sarus/sarus.py
-drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2023-05-05 06:37:29.779113 sarus-0.6.0/sarus/scripts/
--rw-rw-r--   0 vincent   (1000) vincent   (1000)        0 2023-04-21 19:49:48.000000 sarus-0.6.0/sarus/scripts/__init__.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     4618 2023-04-21 19:49:48.000000 sarus-0.6.0/sarus/scripts/generate_op_list.py
-drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2023-05-05 06:37:29.783113 sarus-0.6.0/sarus/sklearn/
--rw-rw-r--   0 vincent   (1000) vincent   (1000)      680 2023-04-21 19:49:48.000000 sarus-0.6.0/sarus/sklearn/__init__.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     6604 2023-05-05 06:32:20.000000 sarus-0.6.0/sarus/sklearn/cluster.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)      766 2022-11-29 13:03:29.000000 sarus-0.6.0/sarus/sklearn/compose.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)      814 2023-05-05 06:32:20.000000 sarus-0.6.0/sarus/sklearn/decomposition.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)    11437 2023-05-05 06:32:20.000000 sarus-0.6.0/sarus/sklearn/ensemble.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)      566 2022-11-29 13:03:29.000000 sarus-0.6.0/sarus/sklearn/impute.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)      177 2022-09-14 12:56:20.000000 sarus-0.6.0/sarus/sklearn/inspection.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)      668 2023-04-21 19:49:48.000000 sarus-0.6.0/sarus/sklearn/linear_model.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)      174 2022-09-14 12:56:20.000000 sarus-0.6.0/sarus/sklearn/metrics.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     1112 2023-04-21 19:49:48.000000 sarus-0.6.0/sarus/sklearn/model_selection.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)      558 2022-11-29 13:03:29.000000 sarus-0.6.0/sarus/sklearn/pipeline.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     1569 2023-04-21 19:49:48.000000 sarus-0.6.0/sarus/sklearn/preprocessing.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)      594 2023-04-21 19:49:48.000000 sarus-0.6.0/sarus/sklearn/svm.py
-drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2023-05-05 06:37:29.783113 sarus-0.6.0/sarus/skopt/
--rw-rw-r--   0 vincent   (1000) vincent   (1000)      223 2022-11-29 13:03:29.000000 sarus-0.6.0/sarus/skopt/__init__.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)      929 2022-11-29 13:03:29.000000 sarus-0.6.0/sarus/skopt/searchcv.py
-drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2023-05-05 06:37:29.783113 sarus-0.6.0/sarus/std/
--rw-rw-r--   0 vincent   (1000) vincent   (1000)      154 2022-11-29 13:03:29.000000 sarus-0.6.0/sarus/std/__init__.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     1074 2022-11-29 13:03:29.000000 sarus-0.6.0/sarus/std/types.py
-drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2023-05-05 06:37:29.783113 sarus-0.6.0/sarus/storage/
--rw-rw-r--   0 vincent   (1000) vincent   (1000)        0 2023-01-27 14:38:46.000000 sarus-0.6.0/sarus/storage/__init__.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     4552 2023-01-27 14:38:46.000000 sarus-0.6.0/sarus/storage/legacy_local.py
-drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2023-05-05 06:37:29.783113 sarus-0.6.0/sarus/tensorflow/
--rw-rw-r--   0 vincent   (1000) vincent   (1000)        0 2022-09-14 12:56:20.000000 sarus-0.6.0/sarus/tensorflow/__init__.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     1708 2023-05-05 06:32:20.000000 sarus-0.6.0/sarus/typing.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)    10518 2023-05-05 06:32:20.000000 sarus-0.6.0/sarus/utils.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     1461 2023-04-21 19:49:48.000000 sarus-0.6.0/sarus/wrapper_factory.py
-drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2023-05-05 06:37:29.783113 sarus-0.6.0/sarus/xgboost/
--rw-rw-r--   0 vincent   (1000) vincent   (1000)      213 2022-09-14 12:56:20.000000 sarus-0.6.0/sarus/xgboost/__init__.py
--rw-rw-r--   0 vincent   (1000) vincent   (1000)      755 2023-05-05 06:32:20.000000 sarus-0.6.0/sarus/xgboost/xgboost.py
-drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2023-05-05 06:37:29.771113 sarus-0.6.0/sarus.egg-info/
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     1553 2023-05-05 06:37:29.000000 sarus-0.6.0/sarus.egg-info/PKG-INFO
--rw-rw-r--   0 vincent   (1000) vincent   (1000)     2057 2023-05-05 06:37:29.000000 sarus-0.6.0/sarus.egg-info/SOURCES.txt
--rw-rw-r--   0 vincent   (1000) vincent   (1000)        1 2023-05-05 06:37:29.000000 sarus-0.6.0/sarus.egg-info/dependency_links.txt
--rw-rw-r--   0 vincent   (1000) vincent   (1000)        1 2021-08-30 08:41:07.000000 sarus-0.6.0/sarus.egg-info/not-zip-safe
--rw-rw-r--   0 vincent   (1000) vincent   (1000)      344 2023-05-05 06:37:29.000000 sarus-0.6.0/sarus.egg-info/requires.txt
--rw-rw-r--   0 vincent   (1000) vincent   (1000)        6 2023-05-05 06:37:29.000000 sarus-0.6.0/sarus.egg-info/top_level.txt
--rwxrwxr-x   0 vincent   (1000) vincent   (1000)     1301 2023-05-05 06:37:29.787113 sarus-0.6.0/setup.cfg
--rwxrwxr-x   0 vincent   (1000) vincent   (1000)      106 2023-05-05 06:36:31.000000 sarus-0.6.0/setup.py
-drwxrwxr-x   0 vincent   (1000) vincent   (1000)        0 2023-05-05 06:37:29.783113 sarus-0.6.0/tests/
--rwxrwxr-x   0 vincent   (1000) vincent   (1000)      101 2021-09-06 19:14:48.000000 sarus-0.6.0/tests/test_sanity.py
+drwxrwxr-x   0 vl        (1001) vl        (1002)        0 2023-05-02 06:50:18.000000 sarus-0.6.0.dev0/
+-rw-rw-r--   0 vl        (1001) vl        (1002)      100 2023-05-02 06:49:37.000000 sarus-0.6.0.dev0/pyproject.toml
+-rwxrwxr-x   0 vl        (1001) vl        (1002)      111 2023-05-02 06:50:02.000000 sarus-0.6.0.dev0/setup.py
+-rw-rw-r--   0 vl        (1001) vl        (1002)      663 2023-05-02 06:49:37.000000 sarus-0.6.0.dev0/README.rst
+-rw-rw-r--   0 vl        (1001) vl        (1002)       25 2023-05-02 06:49:37.000000 sarus-0.6.0.dev0/MANIFEST.in
+drwxrwxr-x   0 vl        (1001) vl        (1002)        0 2023-05-02 06:50:18.000000 sarus-0.6.0.dev0/sarus/
+-rw-rw-r--   0 vl        (1001) vl        (1002)      743 2023-05-02 06:49:37.000000 sarus-0.6.0.dev0/sarus/debug.py
+drwxrwxr-x   0 vl        (1001) vl        (1002)        0 2023-05-02 06:50:18.000000 sarus-0.6.0.dev0/sarus/xgboost/
+-rw-rw-r--   0 vl        (1001) vl        (1002)      213 2023-05-02 06:49:37.000000 sarus-0.6.0.dev0/sarus/xgboost/__init__.py
+-rw-rw-r--   0 vl        (1001) vl        (1002)      755 2023-05-02 06:49:37.000000 sarus-0.6.0.dev0/sarus/xgboost/xgboost.py
+-rw-rw-r--   0 vl        (1001) vl        (1002)    10518 2023-05-02 06:49:37.000000 sarus-0.6.0.dev0/sarus/utils.py
+drwxrwxr-x   0 vl        (1001) vl        (1002)        0 2023-05-02 06:50:18.000000 sarus-0.6.0.dev0/sarus/pandas/
+-rw-rw-r--   0 vl        (1001) vl        (1002)      197 2023-05-02 06:49:37.000000 sarus-0.6.0.dev0/sarus/pandas/__init__.py
+-rw-rw-r--   0 vl        (1001) vl        (1002)     4918 2023-05-02 06:49:37.000000 sarus-0.6.0.dev0/sarus/pandas/dataframe.py
+-rw-rw-r--   0 vl        (1001) vl        (1002)      822 2023-05-02 06:49:37.000000 sarus-0.6.0.dev0/sarus/pandas/core.py
+-rw-rw-r--   0 vl        (1001) vl        (1002)      206 2023-05-02 06:49:37.000000 sarus-0.6.0.dev0/sarus/pandas/io.py
+drwxrwxr-x   0 vl        (1001) vl        (1002)        0 2023-05-02 06:50:18.000000 sarus-0.6.0.dev0/sarus/std/
+-rw-rw-r--   0 vl        (1001) vl        (1002)      154 2023-05-02 06:49:37.000000 sarus-0.6.0.dev0/sarus/std/__init__.py
+-rw-rw-r--   0 vl        (1001) vl        (1002)     1074 2023-05-02 06:49:37.000000 sarus-0.6.0.dev0/sarus/std/types.py
+drwxrwxr-x   0 vl        (1001) vl        (1002)        0 2023-05-02 06:50:18.000000 sarus-0.6.0.dev0/sarus/pandas_profiling/
+-rw-rw-r--   0 vl        (1001) vl        (1002)       81 2023-05-02 06:49:37.000000 sarus-0.6.0.dev0/sarus/pandas_profiling/__init__.py
+-rw-rw-r--   0 vl        (1001) vl        (1002)      841 2023-05-02 06:49:37.000000 sarus-0.6.0.dev0/sarus/pandas_profiling/profile_report.py
+-rw-rw-r--   0 vl        (1001) vl        (1002)      549 2023-05-02 06:50:02.000000 sarus-0.6.0.dev0/sarus/__init__.py
+drwxrwxr-x   0 vl        (1001) vl        (1002)        0 2023-05-02 06:50:18.000000 sarus-0.6.0.dev0/sarus/legacy/
+drwxrwxr-x   0 vl        (1001) vl        (1002)        0 2023-05-02 06:50:18.000000 sarus-0.6.0.dev0/sarus/legacy/pandas/
+-rw-rw-r--   0 vl        (1001) vl        (1002)      100 2023-05-02 06:49:37.000000 sarus-0.6.0.dev0/sarus/legacy/pandas/__init__.py
+-rw-rw-r--   0 vl        (1001) vl        (1002)    16606 2023-05-02 06:49:37.000000 sarus-0.6.0.dev0/sarus/legacy/pandas/dataframe.py
+-rw-rw-r--   0 vl        (1001) vl        (1002)       42 2023-05-02 06:49:37.000000 sarus-0.6.0.dev0/sarus/legacy/__init__.py
+drwxrwxr-x   0 vl        (1001) vl        (1002)        0 2023-05-02 06:50:18.000000 sarus-0.6.0.dev0/sarus/legacy/tensorflow/
+-rw-rw-r--   0 vl        (1001) vl        (1002)      132 2023-05-02 06:49:37.000000 sarus-0.6.0.dev0/sarus/legacy/tensorflow/__init__.py
+-rw-rw-r--   0 vl        (1001) vl        (1002)    42361 2023-05-02 06:49:37.000000 sarus-0.6.0.dev0/sarus/legacy/tensorflow/model.py
+-rw-rw-r--   0 vl        (1001) vl        (1002)    13194 2023-05-02 06:49:37.000000 sarus-0.6.0.dev0/sarus/legacy/tensorflow/dataset.py
+-rw-rw-r--   0 vl        (1001) vl        (1002)    13051 2023-05-02 06:49:37.000000 sarus-0.6.0.dev0/sarus/config.yaml
+-rw-rw-r--   0 vl        (1001) vl        (1002)     1708 2023-05-02 06:49:37.000000 sarus-0.6.0.dev0/sarus/typing.py
+-rw-rw-r--   0 vl        (1001) vl        (1002)    55988 2023-05-02 06:50:02.000000 sarus-0.6.0.dev0/sarus/sarus.py
+drwxrwxr-x   0 vl        (1001) vl        (1002)        0 2023-05-02 06:50:18.000000 sarus-0.6.0.dev0/sarus/plotly/
+-rw-rw-r--   0 vl        (1001) vl        (1002)      108 2023-05-02 06:49:37.000000 sarus-0.6.0.dev0/sarus/plotly/__init__.py
+-rw-rw-r--   0 vl        (1001) vl        (1002)      138 2023-05-02 06:49:37.000000 sarus-0.6.0.dev0/sarus/plotly/express.py
+drwxrwxr-x   0 vl        (1001) vl        (1002)        0 2023-05-02 06:50:18.000000 sarus-0.6.0.dev0/sarus/tensorflow/
+-rw-rw-r--   0 vl        (1001) vl        (1002)        0 2023-05-02 06:49:37.000000 sarus-0.6.0.dev0/sarus/tensorflow/__init__.py
+drwxrwxr-x   0 vl        (1001) vl        (1002)        0 2023-05-02 06:50:18.000000 sarus-0.6.0.dev0/sarus/context/
+-rw-rw-r--   0 vl        (1001) vl        (1002)        0 2023-05-02 06:49:37.000000 sarus-0.6.0.dev0/sarus/context/__init__.py
+-rw-rw-r--   0 vl        (1001) vl        (1002)      302 2023-05-02 06:49:37.000000 sarus-0.6.0.dev0/sarus/context/typing.py
+-rw-rw-r--   0 vl        (1001) vl        (1002)     3069 2023-05-02 06:49:37.000000 sarus-0.6.0.dev0/sarus/context/local_sdk.py
+-rw-rw-r--   0 vl        (1001) vl        (1002)     1461 2023-05-02 06:49:37.000000 sarus-0.6.0.dev0/sarus/wrapper_factory.py
+drwxrwxr-x   0 vl        (1001) vl        (1002)        0 2023-05-02 06:50:18.000000 sarus-0.6.0.dev0/sarus/sklearn/
+-rw-rw-r--   0 vl        (1001) vl        (1002)      766 2023-05-02 06:49:37.000000 sarus-0.6.0.dev0/sarus/sklearn/compose.py
+-rw-rw-r--   0 vl        (1001) vl        (1002)      680 2023-05-02 06:49:37.000000 sarus-0.6.0.dev0/sarus/sklearn/__init__.py
+-rw-rw-r--   0 vl        (1001) vl        (1002)      566 2023-05-02 06:49:37.000000 sarus-0.6.0.dev0/sarus/sklearn/impute.py
+-rw-rw-r--   0 vl        (1001) vl        (1002)      174 2023-05-02 06:49:37.000000 sarus-0.6.0.dev0/sarus/sklearn/metrics.py
+-rw-rw-r--   0 vl        (1001) vl        (1002)      594 2023-05-02 06:49:37.000000 sarus-0.6.0.dev0/sarus/sklearn/svm.py
+-rw-rw-r--   0 vl        (1001) vl        (1002)      668 2023-05-02 06:49:37.000000 sarus-0.6.0.dev0/sarus/sklearn/linear_model.py
+-rw-rw-r--   0 vl        (1001) vl        (1002)     1569 2023-05-02 06:49:37.000000 sarus-0.6.0.dev0/sarus/sklearn/preprocessing.py
+-rw-rw-r--   0 vl        (1001) vl        (1002)      814 2023-05-02 06:49:37.000000 sarus-0.6.0.dev0/sarus/sklearn/decomposition.py
+-rw-rw-r--   0 vl        (1001) vl        (1002)      558 2023-05-02 06:49:37.000000 sarus-0.6.0.dev0/sarus/sklearn/pipeline.py
+-rw-rw-r--   0 vl        (1001) vl        (1002)     6604 2023-05-02 06:49:37.000000 sarus-0.6.0.dev0/sarus/sklearn/cluster.py
+-rw-rw-r--   0 vl        (1001) vl        (1002)      177 2023-05-02 06:49:37.000000 sarus-0.6.0.dev0/sarus/sklearn/inspection.py
+-rw-rw-r--   0 vl        (1001) vl        (1002)     1112 2023-05-02 06:49:37.000000 sarus-0.6.0.dev0/sarus/sklearn/model_selection.py
+-rw-rw-r--   0 vl        (1001) vl        (1002)    11437 2023-05-02 06:49:37.000000 sarus-0.6.0.dev0/sarus/sklearn/ensemble.py
+drwxrwxr-x   0 vl        (1001) vl        (1002)        0 2023-05-02 06:50:18.000000 sarus-0.6.0.dev0/sarus/scripts/
+-rw-rw-r--   0 vl        (1001) vl        (1002)     4618 2023-05-02 06:49:37.000000 sarus-0.6.0.dev0/sarus/scripts/generate_op_list.py
+-rw-rw-r--   0 vl        (1001) vl        (1002)        0 2023-05-02 06:49:37.000000 sarus-0.6.0.dev0/sarus/scripts/__init__.py
+drwxrwxr-x   0 vl        (1001) vl        (1002)        0 2023-05-02 06:50:18.000000 sarus-0.6.0.dev0/sarus/numpy/
+-rw-rw-r--   0 vl        (1001) vl        (1002)      337 2023-05-02 06:49:37.000000 sarus-0.6.0.dev0/sarus/numpy/__init__.py
+-rw-rw-r--   0 vl        (1001) vl        (1002)       81 2023-05-02 06:49:37.000000 sarus-0.6.0.dev0/sarus/numpy/random.py
+-rw-rw-r--   0 vl        (1001) vl        (1002)      963 2023-05-02 06:49:37.000000 sarus-0.6.0.dev0/sarus/numpy/scalars.py
+drwxrwxr-x   0 vl        (1001) vl        (1002)        0 2023-05-02 06:50:18.000000 sarus-0.6.0.dev0/sarus/storage/
+-rw-rw-r--   0 vl        (1001) vl        (1002)        0 2023-05-02 06:49:37.000000 sarus-0.6.0.dev0/sarus/storage/__init__.py
+-rw-rw-r--   0 vl        (1001) vl        (1002)     4552 2023-05-02 06:49:37.000000 sarus-0.6.0.dev0/sarus/storage/legacy_local.py
+drwxrwxr-x   0 vl        (1001) vl        (1002)        0 2023-05-02 06:50:18.000000 sarus-0.6.0.dev0/sarus/imblearn/
+-rw-rw-r--   0 vl        (1001) vl        (1002)      265 2023-05-02 06:49:37.000000 sarus-0.6.0.dev0/sarus/imblearn/__init__.py
+-rw-rw-r--   0 vl        (1001) vl        (1002)      556 2023-05-02 06:49:37.000000 sarus-0.6.0.dev0/sarus/imblearn/under_sampling.py
+-rw-rw-r--   0 vl        (1001) vl        (1002)      558 2023-05-02 06:49:37.000000 sarus-0.6.0.dev0/sarus/imblearn/pipeline.py
+-rw-rw-r--   0 vl        (1001) vl        (1002)      578 2023-05-02 06:49:37.000000 sarus-0.6.0.dev0/sarus/imblearn/over_sampling.py
+-rw-rw-r--   0 vl        (1001) vl        (1002)    14156 2023-05-02 06:49:37.000000 sarus-0.6.0.dev0/sarus/dataspec_wrapper.py
+drwxrwxr-x   0 vl        (1001) vl        (1002)        0 2023-05-02 06:50:18.000000 sarus-0.6.0.dev0/sarus/manager/
+-rw-rw-r--   0 vl        (1001) vl        (1002)    19293 2023-05-02 06:50:02.000000 sarus-0.6.0.dev0/sarus/manager/sdk_manager.py
+-rw-rw-r--   0 vl        (1001) vl        (1002)     1949 2023-05-02 06:50:02.000000 sarus-0.6.0.dev0/sarus/manager/arrow_remote.py
+-rw-rw-r--   0 vl        (1001) vl        (1002)     1595 2023-05-02 06:50:02.000000 sarus-0.6.0.dev0/sarus/manager/value_remote.py
+-rw-rw-r--   0 vl        (1001) vl        (1002)        0 2023-05-02 06:49:37.000000 sarus-0.6.0.dev0/sarus/manager/__init__.py
+-rw-rw-r--   0 vl        (1001) vl        (1002)     2556 2023-05-02 06:50:02.000000 sarus-0.6.0.dev0/sarus/manager/typing.py
+-rw-rw-r--   0 vl        (1001) vl        (1002)     6201 2023-05-02 06:50:02.000000 sarus-0.6.0.dev0/sarus/manager/dataspec_api.py
+-rw-rw-r--   0 vl        (1001) vl        (1002)     5360 2023-05-02 06:50:02.000000 sarus-0.6.0.dev0/sarus/manager/arrow_local.py
+-rw-rw-r--   0 vl        (1001) vl        (1002)     3733 2023-05-02 06:50:02.000000 sarus-0.6.0.dev0/sarus/manager/cache_scalar_local.py
+-rw-rw-r--   0 vl        (1001) vl        (1002)     4599 2023-05-02 06:50:02.000000 sarus-0.6.0.dev0/sarus/manager/value_local.py
+-rw-rw-r--   0 vl        (1001) vl        (1002)     3352 2023-05-02 06:50:02.000000 sarus-0.6.0.dev0/sarus/manager/parquet_local.py
+drwxrwxr-x   0 vl        (1001) vl        (1002)        0 2023-05-02 06:50:18.000000 sarus-0.6.0.dev0/sarus/manager/ops/
+-rw-rw-r--   0 vl        (1001) vl        (1002)        0 2023-05-02 06:49:37.000000 sarus-0.6.0.dev0/sarus/manager/ops/__init__.py
+-rw-rw-r--   0 vl        (1001) vl        (1002)      921 2023-05-02 06:49:37.000000 sarus-0.6.0.dev0/sarus/manager/ops/api.py
+drwxrwxr-x   0 vl        (1001) vl        (1002)        0 2023-05-02 06:50:18.000000 sarus-0.6.0.dev0/sarus/skopt/
+-rw-rw-r--   0 vl        (1001) vl        (1002)      223 2023-05-02 06:49:37.000000 sarus-0.6.0.dev0/sarus/skopt/__init__.py
+-rw-rw-r--   0 vl        (1001) vl        (1002)      929 2023-05-02 06:49:37.000000 sarus-0.6.0.dev0/sarus/skopt/searchcv.py
+-rw-rw-r--   0 vl        (1001) vl        (1002)     1830 2023-05-02 06:50:18.000000 sarus-0.6.0.dev0/PKG-INFO
+drwxrwxr-x   0 vl        (1001) vl        (1002)        0 2023-05-02 06:50:18.000000 sarus-0.6.0.dev0/sarus.egg-info/
+-rw-rw-r--   0 vl        (1001) vl        (1002)        6 2023-05-02 06:50:18.000000 sarus-0.6.0.dev0/sarus.egg-info/top_level.txt
+-rw-rw-r--   0 vl        (1001) vl        (1002)        1 2023-05-02 06:50:18.000000 sarus-0.6.0.dev0/sarus.egg-info/dependency_links.txt
+-rw-rw-r--   0 vl        (1001) vl        (1002)     2036 2023-05-02 06:50:18.000000 sarus-0.6.0.dev0/sarus.egg-info/SOURCES.txt
+-rw-rw-r--   0 vl        (1001) vl        (1002)        1 2023-05-02 06:50:18.000000 sarus-0.6.0.dev0/sarus.egg-info/not-zip-safe
+-rw-rw-r--   0 vl        (1001) vl        (1002)     1830 2023-05-02 06:50:18.000000 sarus-0.6.0.dev0/sarus.egg-info/PKG-INFO
+-rw-rw-r--   0 vl        (1001) vl        (1002)      344 2023-05-02 06:50:18.000000 sarus-0.6.0.dev0/sarus.egg-info/requires.txt
+-rwxrwxr-x   0 vl        (1001) vl        (1002)     1301 2023-05-02 06:50:18.000000 sarus-0.6.0.dev0/setup.cfg
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive
+POSIX tar archive (GNU)
```

### Comparing `sarus-0.6.0/PKG-INFO` & `sarus-0.6.0.dev0/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,17 +1,50 @@
 Metadata-Version: 2.1
 Name: sarus
-Version: 0.6.0
+Version: 0.6.0.dev0
 Summary: Python client for the Sarus Gateway
 Home-page: https://sarus.tech
-Download-URL: 
 Author: Sarus Technologies
 Author-email: contact@sarus.tech
 License: Apache License 2.0
+Description: 
+        Sarus
+        
+        ===
+        
+        Python client for the Sarus Gateway. It provides simple connectors to leverage confidential data while ensuring data privacy. Users can explore & train AI models on sensitive data, via synthetic data browsing, remote training and differential privacy.
+        
+        Installation
+        ------------
+        
+        PIP
+        ^^^
+        
+        To install locally the latest available version :
+        
+        ``pip install sarus``
+        
+        Usage
+        -----
+        
+        Client
+        ^^^^^^
+        
+        Use this class to connect to **Sarus Gateway**.
+        
+        .. code-block:: python
+        
+           from sarus import Client
+        
+           client = Client(url="http://admin.sarus.tech:5000")
+           available = client.available_datasets()
+           print(f'Datasets available on the server: {available}')
+        
 Keywords: differential privacy,AI,Data privacy
+Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: License :: OSI Approved :: Apache Software License
@@ -21,40 +54,7 @@
 Provides-Extra: imblearn
 Provides-Extra: tensorflow
 Provides-Extra: pandas_profiling
 Provides-Extra: plotly
 Provides-Extra: xgboost
 Provides-Extra: skopt
 Provides-Extra: tests
-
-
-Sarus
-
-===
-
-Python client for the Sarus Gateway. It provides simple connectors to leverage confidential data while ensuring data privacy. Users can explore & train AI models on sensitive data, via synthetic data browsing, remote training and differential privacy.
-
-Installation
-------------
-
-PIP
-^^^
-
-To install locally the latest available version :
-
-``pip install sarus``
-
-Usage
------
-
-Client
-^^^^^^
-
-Use this class to connect to **Sarus Gateway**.
-
-.. code-block:: python
-
-   from sarus import Client
-
-   client = Client(url="http://admin.sarus.tech:5000")
-   available = client.available_datasets()
-   print(f'Datasets available on the server: {available}')
```

### Comparing `sarus-0.6.0/README.rst` & `sarus-0.6.0.dev0/README.rst`

 * *Files identical despite different names*

### Comparing `sarus-0.6.0/sarus/__init__.py` & `sarus-0.6.0.dev0/sarus/__init__.py`

 * *Files 21% similar despite different names*

```diff
@@ -13,15 +13,15 @@
         std,
         xgboost,
     )
 
     from .sarus import Client, Dataset
     from .utils import eval, eval_policy, floating, integer, length
 
-VERSION = "0.6.0"
+VERSION = "0.6.0.dev0"
 
 __all__ = [
     "Dataset",
     "Client",
     "length",
     "eval",
     "eval_policy",
```

### Comparing `sarus-0.6.0/sarus/config.yaml` & `sarus-0.6.0.dev0/sarus/config.yaml`

 * *Files identical despite different names*

### Comparing `sarus-0.6.0/sarus/context/local_sdk.py` & `sarus-0.6.0.dev0/sarus/context/local_sdk.py`

 * *Files identical despite different names*

### Comparing `sarus-0.6.0/sarus/dataspec_wrapper.py` & `sarus-0.6.0.dev0/sarus/dataspec_wrapper.py`

 * *Files identical despite different names*

### Comparing `sarus-0.6.0/sarus/debug.py` & `sarus-0.6.0.dev0/sarus/debug.py`

 * *Files identical despite different names*

### Comparing `sarus-0.6.0/sarus/imblearn/over_sampling.py` & `sarus-0.6.0.dev0/sarus/imblearn/over_sampling.py`

 * *Files identical despite different names*

### Comparing `sarus-0.6.0/sarus/imblearn/pipeline.py` & `sarus-0.6.0.dev0/sarus/imblearn/pipeline.py`

 * *Files identical despite different names*

### Comparing `sarus-0.6.0/sarus/imblearn/under_sampling.py` & `sarus-0.6.0.dev0/sarus/imblearn/under_sampling.py`

 * *Files identical despite different names*

### Comparing `sarus-0.6.0/sarus/legacy/pandas/dataframe.py` & `sarus-0.6.0.dev0/sarus/legacy/pandas/dataframe.py`

 * *Files identical despite different names*

### Comparing `sarus-0.6.0/sarus/legacy/tensorflow/dataset.py` & `sarus-0.6.0.dev0/sarus/legacy/tensorflow/dataset.py`

 * *Files identical despite different names*

### Comparing `sarus-0.6.0/sarus/legacy/tensorflow/model.py` & `sarus-0.6.0.dev0/sarus/legacy/tensorflow/model.py`

 * *Files identical despite different names*

### Comparing `sarus-0.6.0/sarus/manager/arrow_local.py` & `sarus-0.6.0.dev0/sarus/manager/arrow_local.py`

 * *Files identical despite different names*

### Comparing `sarus-0.6.0/sarus/manager/arrow_remote.py` & `sarus-0.6.0.dev0/sarus/manager/arrow_remote.py`

 * *Files identical despite different names*

### Comparing `sarus-0.6.0/sarus/manager/cache_scalar_local.py` & `sarus-0.6.0.dev0/sarus/manager/cache_scalar_local.py`

 * *Files identical despite different names*

### Comparing `sarus-0.6.0/sarus/manager/dataspec_api.py` & `sarus-0.6.0.dev0/sarus/manager/dataspec_api.py`

 * *Files identical despite different names*

### Comparing `sarus-0.6.0/sarus/manager/ops/api.py` & `sarus-0.6.0.dev0/sarus/manager/ops/api.py`

 * *Files identical despite different names*

### Comparing `sarus-0.6.0/sarus/manager/parquet_local.py` & `sarus-0.6.0.dev0/sarus/manager/parquet_local.py`

 * *Files identical despite different names*

### Comparing `sarus-0.6.0/sarus/manager/sdk_manager.py` & `sarus-0.6.0.dev0/sarus/manager/sdk_manager.py`

 * *Files identical despite different names*

### Comparing `sarus-0.6.0/sarus/manager/typing.py` & `sarus-0.6.0.dev0/sarus/manager/typing.py`

 * *Files identical despite different names*

### Comparing `sarus-0.6.0/sarus/manager/value_local.py` & `sarus-0.6.0.dev0/sarus/manager/value_local.py`

 * *Files identical despite different names*

### Comparing `sarus-0.6.0/sarus/manager/value_remote.py` & `sarus-0.6.0.dev0/sarus/manager/value_remote.py`

 * *Files identical despite different names*

### Comparing `sarus-0.6.0/sarus/numpy/scalars.py` & `sarus-0.6.0.dev0/sarus/numpy/scalars.py`

 * *Files identical despite different names*

### Comparing `sarus-0.6.0/sarus/pandas/core.py` & `sarus-0.6.0.dev0/sarus/pandas/core.py`

 * *Files identical despite different names*

### Comparing `sarus-0.6.0/sarus/pandas/dataframe.py` & `sarus-0.6.0.dev0/sarus/pandas/dataframe.py`

 * *Files identical despite different names*

### Comparing `sarus-0.6.0/sarus/pandas_profiling/profile_report.py` & `sarus-0.6.0.dev0/sarus/pandas_profiling/profile_report.py`

 * *Files identical despite different names*

### Comparing `sarus-0.6.0/sarus/sarus.py` & `sarus-0.6.0.dev0/sarus/sarus.py`

 * *Files identical despite different names*

### Comparing `sarus-0.6.0/sarus/scripts/generate_op_list.py` & `sarus-0.6.0.dev0/sarus/scripts/generate_op_list.py`

 * *Files identical despite different names*

### Comparing `sarus-0.6.0/sarus/sklearn/__init__.py` & `sarus-0.6.0.dev0/sarus/sklearn/__init__.py`

 * *Files identical despite different names*

### Comparing `sarus-0.6.0/sarus/sklearn/cluster.py` & `sarus-0.6.0.dev0/sarus/sklearn/cluster.py`

 * *Files identical despite different names*

### Comparing `sarus-0.6.0/sarus/sklearn/compose.py` & `sarus-0.6.0.dev0/sarus/sklearn/compose.py`

 * *Files identical despite different names*

### Comparing `sarus-0.6.0/sarus/sklearn/decomposition.py` & `sarus-0.6.0.dev0/sarus/sklearn/decomposition.py`

 * *Files identical despite different names*

### Comparing `sarus-0.6.0/sarus/sklearn/ensemble.py` & `sarus-0.6.0.dev0/sarus/sklearn/ensemble.py`

 * *Files identical despite different names*

### Comparing `sarus-0.6.0/sarus/sklearn/impute.py` & `sarus-0.6.0.dev0/sarus/sklearn/impute.py`

 * *Files identical despite different names*

### Comparing `sarus-0.6.0/sarus/sklearn/linear_model.py` & `sarus-0.6.0.dev0/sarus/sklearn/linear_model.py`

 * *Files identical despite different names*

### Comparing `sarus-0.6.0/sarus/sklearn/model_selection.py` & `sarus-0.6.0.dev0/sarus/sklearn/model_selection.py`

 * *Files identical despite different names*

### Comparing `sarus-0.6.0/sarus/sklearn/pipeline.py` & `sarus-0.6.0.dev0/sarus/sklearn/pipeline.py`

 * *Files identical despite different names*

### Comparing `sarus-0.6.0/sarus/sklearn/preprocessing.py` & `sarus-0.6.0.dev0/sarus/sklearn/preprocessing.py`

 * *Files identical despite different names*

### Comparing `sarus-0.6.0/sarus/sklearn/svm.py` & `sarus-0.6.0.dev0/sarus/sklearn/svm.py`

 * *Files identical despite different names*

### Comparing `sarus-0.6.0/sarus/skopt/searchcv.py` & `sarus-0.6.0.dev0/sarus/skopt/searchcv.py`

 * *Files identical despite different names*

### Comparing `sarus-0.6.0/sarus/std/types.py` & `sarus-0.6.0.dev0/sarus/std/types.py`

 * *Files identical despite different names*

### Comparing `sarus-0.6.0/sarus/storage/legacy_local.py` & `sarus-0.6.0.dev0/sarus/storage/legacy_local.py`

 * *Files identical despite different names*

### Comparing `sarus-0.6.0/sarus/typing.py` & `sarus-0.6.0.dev0/sarus/typing.py`

 * *Files identical despite different names*

### Comparing `sarus-0.6.0/sarus/utils.py` & `sarus-0.6.0.dev0/sarus/utils.py`

 * *Files identical despite different names*

### Comparing `sarus-0.6.0/sarus/wrapper_factory.py` & `sarus-0.6.0.dev0/sarus/wrapper_factory.py`

 * *Files identical despite different names*

### Comparing `sarus-0.6.0/sarus/xgboost/xgboost.py` & `sarus-0.6.0.dev0/sarus/xgboost/xgboost.py`

 * *Files identical despite different names*

### Comparing `sarus-0.6.0/sarus.egg-info/PKG-INFO` & `sarus-0.6.0.dev0/sarus.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,17 +1,50 @@
 Metadata-Version: 2.1
 Name: sarus
-Version: 0.6.0
+Version: 0.6.0.dev0
 Summary: Python client for the Sarus Gateway
 Home-page: https://sarus.tech
-Download-URL: 
 Author: Sarus Technologies
 Author-email: contact@sarus.tech
 License: Apache License 2.0
+Description: 
+        Sarus
+        
+        ===
+        
+        Python client for the Sarus Gateway. It provides simple connectors to leverage confidential data while ensuring data privacy. Users can explore & train AI models on sensitive data, via synthetic data browsing, remote training and differential privacy.
+        
+        Installation
+        ------------
+        
+        PIP
+        ^^^
+        
+        To install locally the latest available version :
+        
+        ``pip install sarus``
+        
+        Usage
+        -----
+        
+        Client
+        ^^^^^^
+        
+        Use this class to connect to **Sarus Gateway**.
+        
+        .. code-block:: python
+        
+           from sarus import Client
+        
+           client = Client(url="http://admin.sarus.tech:5000")
+           available = client.available_datasets()
+           print(f'Datasets available on the server: {available}')
+        
 Keywords: differential privacy,AI,Data privacy
+Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: License :: OSI Approved :: Apache Software License
@@ -21,40 +54,7 @@
 Provides-Extra: imblearn
 Provides-Extra: tensorflow
 Provides-Extra: pandas_profiling
 Provides-Extra: plotly
 Provides-Extra: xgboost
 Provides-Extra: skopt
 Provides-Extra: tests
-
-
-Sarus
-
-===
-
-Python client for the Sarus Gateway. It provides simple connectors to leverage confidential data while ensuring data privacy. Users can explore & train AI models on sensitive data, via synthetic data browsing, remote training and differential privacy.
-
-Installation
-------------
-
-PIP
-^^^
-
-To install locally the latest available version :
-
-``pip install sarus``
-
-Usage
------
-
-Client
-^^^^^^
-
-Use this class to connect to **Sarus Gateway**.
-
-.. code-block:: python
-
-   from sarus import Client
-
-   client = Client(url="http://admin.sarus.tech:5000")
-   available = client.available_datasets()
-   print(f'Datasets available on the server: {available}')
```

### Comparing `sarus-0.6.0/sarus.egg-info/SOURCES.txt` & `sarus-0.6.0.dev0/sarus.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -72,9 +72,8 @@
 sarus/skopt/searchcv.py
 sarus/std/__init__.py
 sarus/std/types.py
 sarus/storage/__init__.py
 sarus/storage/legacy_local.py
 sarus/tensorflow/__init__.py
 sarus/xgboost/__init__.py
-sarus/xgboost/xgboost.py
-tests/test_sanity.py
+sarus/xgboost/xgboost.py
```

### Comparing `sarus-0.6.0/setup.cfg` & `sarus-0.6.0.dev0/setup.cfg`

 * *Files identical despite different names*

