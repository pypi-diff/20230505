# Comparing `tmp/torchtnt-nightly-2023.5.3.tar.gz` & `tmp/torchtnt-nightly-2023.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/torchtnt-nightly-2023.5.3.tar", last modified: Wed May  3 11:23:17 2023, max compression
+gzip compressed data, was "dist/torchtnt-nightly-2023.5.4.tar", last modified: Thu May  4 11:23:43 2023, max compression
```

## Comparing `torchtnt-nightly-2023.5.3.tar` & `torchtnt-nightly-2023.5.4.tar`

### file list

```diff
@@ -1,73 +1,73 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 11:23:17.000000 torchtnt-nightly-2023.5.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1533 2023-05-03 11:21:51.000000 torchtnt-nightly-2023.5.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2537 2023-05-03 11:23:17.000000 torchtnt-nightly-2023.5.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1777 2023-05-03 11:21:51.000000 torchtnt-nightly-2023.5.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-05-03 11:21:51.000000 torchtnt-nightly-2023.5.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-03 11:23:17.000000 torchtnt-nightly-2023.5.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2948 2023-05-03 11:21:51.000000 torchtnt-nightly-2023.5.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 11:23:17.000000 torchtnt-nightly-2023.5.3/torchtnt/
--rw-r--r--   0 runner    (1001) docker     (123)      231 2023-05-03 11:21:51.000000 torchtnt-nightly-2023.5.3/torchtnt/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 11:23:17.000000 torchtnt-nightly-2023.5.3/torchtnt/framework/
--rw-r--r--   0 runner    (1001) docker     (123)      956 2023-05-03 11:21:51.000000 torchtnt-nightly-2023.5.3/torchtnt/framework/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4046 2023-05-03 11:21:51.000000 torchtnt-nightly-2023.5.3/torchtnt/framework/_test_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    28872 2023-05-03 11:21:51.000000 torchtnt-nightly-2023.5.3/torchtnt/framework/auto_unit.py
--rw-r--r--   0 runner    (1001) docker     (123)     5020 2023-05-03 11:21:51.000000 torchtnt-nightly-2023.5.3/torchtnt/framework/callback.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 11:23:17.000000 torchtnt-nightly-2023.5.3/torchtnt/framework/callbacks/
--rw-r--r--   0 runner    (1001) docker     (123)     1054 2023-05-03 11:21:51.000000 torchtnt-nightly-2023.5.3/torchtnt/framework/callbacks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3358 2023-05-03 11:21:51.000000 torchtnt-nightly-2023.5.3/torchtnt/framework/callbacks/base_csv_writer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2907 2023-05-03 11:21:51.000000 torchtnt-nightly-2023.5.3/torchtnt/framework/callbacks/garbage_collector.py
--rw-r--r--   0 runner    (1001) docker     (123)     4452 2023-05-03 11:21:51.000000 torchtnt-nightly-2023.5.3/torchtnt/framework/callbacks/lambda_callback.py
--rw-r--r--   0 runner    (1001) docker     (123)     3582 2023-05-03 11:21:51.000000 torchtnt-nightly-2023.5.3/torchtnt/framework/callbacks/learning_rate_monitor.py
--rw-r--r--   0 runner    (1001) docker     (123)     3628 2023-05-03 11:21:51.000000 torchtnt-nightly-2023.5.3/torchtnt/framework/callbacks/module_summary.py
--rw-r--r--   0 runner    (1001) docker     (123)     1999 2023-05-03 11:21:51.000000 torchtnt-nightly-2023.5.3/torchtnt/framework/callbacks/pytorch_profiler.py
--rw-r--r--   0 runner    (1001) docker     (123)     3532 2023-05-03 11:21:51.000000 torchtnt-nightly-2023.5.3/torchtnt/framework/callbacks/system_resources_monitor.py
--rw-r--r--   0 runner    (1001) docker     (123)     1956 2023-05-03 11:21:51.000000 torchtnt-nightly-2023.5.3/torchtnt/framework/callbacks/tensorboard_parameter_monitor.py
--rw-r--r--   0 runner    (1001) docker     (123)    10455 2023-05-03 11:21:51.000000 torchtnt-nightly-2023.5.3/torchtnt/framework/callbacks/torchsnapshot_saver.py
--rw-r--r--   0 runner    (1001) docker     (123)     6771 2023-05-03 11:21:51.000000 torchtnt-nightly-2023.5.3/torchtnt/framework/callbacks/tqdm_progress_bar.py
--rw-r--r--   0 runner    (1001) docker     (123)     1819 2023-05-03 11:21:51.000000 torchtnt-nightly-2023.5.3/torchtnt/framework/callbacks/train_progress_monitor.py
--rw-r--r--   0 runner    (1001) docker     (123)     8521 2023-05-03 11:21:51.000000 torchtnt-nightly-2023.5.3/torchtnt/framework/evaluate.py
--rw-r--r--   0 runner    (1001) docker     (123)     8355 2023-05-03 11:21:51.000000 torchtnt-nightly-2023.5.3/torchtnt/framework/fit.py
--rw-r--r--   0 runner    (1001) docker     (123)     8839 2023-05-03 11:21:51.000000 torchtnt-nightly-2023.5.3/torchtnt/framework/predict.py
--rw-r--r--   0 runner    (1001) docker     (123)     2478 2023-05-03 11:21:51.000000 torchtnt-nightly-2023.5.3/torchtnt/framework/progress.py
--rw-r--r--   0 runner    (1001) docker     (123)     7158 2023-05-03 11:21:51.000000 torchtnt-nightly-2023.5.3/torchtnt/framework/state.py
--rw-r--r--   0 runner    (1001) docker     (123)    13305 2023-05-03 11:21:51.000000 torchtnt-nightly-2023.5.3/torchtnt/framework/train.py
--rw-r--r--   0 runner    (1001) docker     (123)    15360 2023-05-03 11:21:51.000000 torchtnt-nightly-2023.5.3/torchtnt/framework/unit.py
--rw-r--r--   0 runner    (1001) docker     (123)    10271 2023-05-03 11:21:51.000000 torchtnt-nightly-2023.5.3/torchtnt/framework/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 11:21:51.000000 torchtnt-nightly-2023.5.3/torchtnt/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 11:23:17.000000 torchtnt-nightly-2023.5.3/torchtnt/utils/
--rw-r--r--   0 runner    (1001) docker     (123)     2867 2023-05-03 11:21:51.000000 torchtnt-nightly-2023.5.3/torchtnt/utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 11:23:17.000000 torchtnt-nightly-2023.5.3/torchtnt/utils/data/
--rw-r--r--   0 runner    (1001) docker     (123)      794 2023-05-03 11:21:51.000000 torchtnt-nightly-2023.5.3/torchtnt/utils/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3836 2023-05-03 11:21:51.000000 torchtnt-nightly-2023.5.3/torchtnt/utils/data/data_prefetcher.py
--rw-r--r--   0 runner    (1001) docker     (123)    20345 2023-05-03 11:21:51.000000 torchtnt-nightly-2023.5.3/torchtnt/utils/data/iterators.py
--rw-r--r--   0 runner    (1001) docker     (123)     3386 2023-05-03 11:21:51.000000 torchtnt-nightly-2023.5.3/torchtnt/utils/data/multi_dataloader.py
--rw-r--r--   0 runner    (1001) docker     (123)    11235 2023-05-03 11:21:51.000000 torchtnt-nightly-2023.5.3/torchtnt/utils/device.py
--rw-r--r--   0 runner    (1001) docker     (123)    14158 2023-05-03 11:21:51.000000 torchtnt-nightly-2023.5.3/torchtnt/utils/distributed.py
--rw-r--r--   0 runner    (1001) docker     (123)     9897 2023-05-03 11:21:51.000000 torchtnt-nightly-2023.5.3/torchtnt/utils/early_stop_checker.py
--rw-r--r--   0 runner    (1001) docker     (123)     3354 2023-05-03 11:21:51.000000 torchtnt-nightly-2023.5.3/torchtnt/utils/env.py
--rw-r--r--   0 runner    (1001) docker     (123)      515 2023-05-03 11:21:51.000000 torchtnt-nightly-2023.5.3/torchtnt/utils/fsspec.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 11:23:17.000000 torchtnt-nightly-2023.5.3/torchtnt/utils/loggers/
--rw-r--r--   0 runner    (1001) docker     (123)      624 2023-05-03 11:21:51.000000 torchtnt-nightly-2023.5.3/torchtnt/utils/loggers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1524 2023-05-03 11:21:51.000000 torchtnt-nightly-2023.5.3/torchtnt/utils/loggers/csv.py
--rw-r--r--   0 runner    (1001) docker     (123)     2881 2023-05-03 11:21:51.000000 torchtnt-nightly-2023.5.3/torchtnt/utils/loggers/file.py
--rw-r--r--   0 runner    (1001) docker     (123)     2090 2023-05-03 11:21:51.000000 torchtnt-nightly-2023.5.3/torchtnt/utils/loggers/in_memory.py
--rw-r--r--   0 runner    (1001) docker     (123)     1355 2023-05-03 11:21:51.000000 torchtnt-nightly-2023.5.3/torchtnt/utils/loggers/json.py
--rw-r--r--   0 runner    (1001) docker     (123)     1253 2023-05-03 11:21:51.000000 torchtnt-nightly-2023.5.3/torchtnt/utils/loggers/logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     4897 2023-05-03 11:21:51.000000 torchtnt-nightly-2023.5.3/torchtnt/utils/loggers/tensorboard.py
--rw-r--r--   0 runner    (1001) docker     (123)      923 2023-05-03 11:21:51.000000 torchtnt-nightly-2023.5.3/torchtnt/utils/loggers/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      507 2023-05-03 11:21:51.000000 torchtnt-nightly-2023.5.3/torchtnt/utils/lr_scheduler.py
--rw-r--r--   0 runner    (1001) docker     (123)     4760 2023-05-03 11:21:51.000000 torchtnt-nightly-2023.5.3/torchtnt/utils/memory.py
--rw-r--r--   0 runner    (1001) docker     (123)     2538 2023-05-03 11:21:51.000000 torchtnt-nightly-2023.5.3/torchtnt/utils/misc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1151 2023-05-03 11:21:51.000000 torchtnt-nightly-2023.5.3/torchtnt/utils/oom.py
--rw-r--r--   0 runner    (1001) docker     (123)     2110 2023-05-03 11:21:51.000000 torchtnt-nightly-2023.5.3/torchtnt/utils/rank_zero_log.py
--rw-r--r--   0 runner    (1001) docker     (123)     2509 2023-05-03 11:21:51.000000 torchtnt-nightly-2023.5.3/torchtnt/utils/seed.py
--rw-r--r--   0 runner    (1001) docker     (123)      847 2023-05-03 11:21:51.000000 torchtnt-nightly-2023.5.3/torchtnt/utils/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     7670 2023-05-03 11:21:51.000000 torchtnt-nightly-2023.5.3/torchtnt/utils/timer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2205 2023-05-03 11:21:51.000000 torchtnt-nightly-2023.5.3/torchtnt/utils/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 11:23:17.000000 torchtnt-nightly-2023.5.3/torchtnt_nightly.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2537 2023-05-03 11:23:17.000000 torchtnt-nightly-2023.5.3/torchtnt_nightly.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2095 2023-05-03 11:23:17.000000 torchtnt-nightly-2023.5.3/torchtnt_nightly.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-03 11:23:17.000000 torchtnt-nightly-2023.5.3/torchtnt_nightly.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      188 2023-05-03 11:23:17.000000 torchtnt-nightly-2023.5.3/torchtnt_nightly.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-03 11:23:17.000000 torchtnt-nightly-2023.5.3/torchtnt_nightly.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-03 11:23:17.000000 torchtnt-nightly-2023.5.3/torchtnt_nightly.egg-info/zip-safe
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 11:23:43.000000 torchtnt-nightly-2023.5.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1533 2023-05-04 11:22:13.000000 torchtnt-nightly-2023.5.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2537 2023-05-04 11:23:43.000000 torchtnt-nightly-2023.5.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1777 2023-05-04 11:22:13.000000 torchtnt-nightly-2023.5.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-05-04 11:22:13.000000 torchtnt-nightly-2023.5.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-04 11:23:43.000000 torchtnt-nightly-2023.5.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2948 2023-05-04 11:22:13.000000 torchtnt-nightly-2023.5.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 11:23:43.000000 torchtnt-nightly-2023.5.4/torchtnt/
+-rw-r--r--   0 runner    (1001) docker     (123)      231 2023-05-04 11:22:13.000000 torchtnt-nightly-2023.5.4/torchtnt/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 11:23:43.000000 torchtnt-nightly-2023.5.4/torchtnt/framework/
+-rw-r--r--   0 runner    (1001) docker     (123)      956 2023-05-04 11:22:13.000000 torchtnt-nightly-2023.5.4/torchtnt/framework/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4046 2023-05-04 11:22:13.000000 torchtnt-nightly-2023.5.4/torchtnt/framework/_test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28872 2023-05-04 11:22:13.000000 torchtnt-nightly-2023.5.4/torchtnt/framework/auto_unit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5020 2023-05-04 11:22:13.000000 torchtnt-nightly-2023.5.4/torchtnt/framework/callback.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 11:23:43.000000 torchtnt-nightly-2023.5.4/torchtnt/framework/callbacks/
+-rw-r--r--   0 runner    (1001) docker     (123)     1054 2023-05-04 11:22:13.000000 torchtnt-nightly-2023.5.4/torchtnt/framework/callbacks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3358 2023-05-04 11:22:13.000000 torchtnt-nightly-2023.5.4/torchtnt/framework/callbacks/base_csv_writer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2907 2023-05-04 11:22:13.000000 torchtnt-nightly-2023.5.4/torchtnt/framework/callbacks/garbage_collector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4452 2023-05-04 11:22:13.000000 torchtnt-nightly-2023.5.4/torchtnt/framework/callbacks/lambda_callback.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3582 2023-05-04 11:22:13.000000 torchtnt-nightly-2023.5.4/torchtnt/framework/callbacks/learning_rate_monitor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3628 2023-05-04 11:22:13.000000 torchtnt-nightly-2023.5.4/torchtnt/framework/callbacks/module_summary.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1999 2023-05-04 11:22:13.000000 torchtnt-nightly-2023.5.4/torchtnt/framework/callbacks/pytorch_profiler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3532 2023-05-04 11:22:13.000000 torchtnt-nightly-2023.5.4/torchtnt/framework/callbacks/system_resources_monitor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1956 2023-05-04 11:22:13.000000 torchtnt-nightly-2023.5.4/torchtnt/framework/callbacks/tensorboard_parameter_monitor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11883 2023-05-04 11:22:13.000000 torchtnt-nightly-2023.5.4/torchtnt/framework/callbacks/torchsnapshot_saver.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6771 2023-05-04 11:22:13.000000 torchtnt-nightly-2023.5.4/torchtnt/framework/callbacks/tqdm_progress_bar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1819 2023-05-04 11:22:13.000000 torchtnt-nightly-2023.5.4/torchtnt/framework/callbacks/train_progress_monitor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8521 2023-05-04 11:22:13.000000 torchtnt-nightly-2023.5.4/torchtnt/framework/evaluate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8355 2023-05-04 11:22:13.000000 torchtnt-nightly-2023.5.4/torchtnt/framework/fit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8839 2023-05-04 11:22:13.000000 torchtnt-nightly-2023.5.4/torchtnt/framework/predict.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2478 2023-05-04 11:22:13.000000 torchtnt-nightly-2023.5.4/torchtnt/framework/progress.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7158 2023-05-04 11:22:13.000000 torchtnt-nightly-2023.5.4/torchtnt/framework/state.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13305 2023-05-04 11:22:13.000000 torchtnt-nightly-2023.5.4/torchtnt/framework/train.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15360 2023-05-04 11:22:13.000000 torchtnt-nightly-2023.5.4/torchtnt/framework/unit.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10271 2023-05-04 11:22:13.000000 torchtnt-nightly-2023.5.4/torchtnt/framework/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 11:22:13.000000 torchtnt-nightly-2023.5.4/torchtnt/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 11:23:43.000000 torchtnt-nightly-2023.5.4/torchtnt/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     2867 2023-05-04 11:22:13.000000 torchtnt-nightly-2023.5.4/torchtnt/utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 11:23:43.000000 torchtnt-nightly-2023.5.4/torchtnt/utils/data/
+-rw-r--r--   0 runner    (1001) docker     (123)      794 2023-05-04 11:22:13.000000 torchtnt-nightly-2023.5.4/torchtnt/utils/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3836 2023-05-04 11:22:13.000000 torchtnt-nightly-2023.5.4/torchtnt/utils/data/data_prefetcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20345 2023-05-04 11:22:13.000000 torchtnt-nightly-2023.5.4/torchtnt/utils/data/iterators.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3386 2023-05-04 11:22:13.000000 torchtnt-nightly-2023.5.4/torchtnt/utils/data/multi_dataloader.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11235 2023-05-04 11:22:13.000000 torchtnt-nightly-2023.5.4/torchtnt/utils/device.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14158 2023-05-04 11:22:13.000000 torchtnt-nightly-2023.5.4/torchtnt/utils/distributed.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9897 2023-05-04 11:22:13.000000 torchtnt-nightly-2023.5.4/torchtnt/utils/early_stop_checker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3354 2023-05-04 11:22:13.000000 torchtnt-nightly-2023.5.4/torchtnt/utils/env.py
+-rw-r--r--   0 runner    (1001) docker     (123)      515 2023-05-04 11:22:13.000000 torchtnt-nightly-2023.5.4/torchtnt/utils/fsspec.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 11:23:43.000000 torchtnt-nightly-2023.5.4/torchtnt/utils/loggers/
+-rw-r--r--   0 runner    (1001) docker     (123)      624 2023-05-04 11:22:13.000000 torchtnt-nightly-2023.5.4/torchtnt/utils/loggers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1524 2023-05-04 11:22:13.000000 torchtnt-nightly-2023.5.4/torchtnt/utils/loggers/csv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2881 2023-05-04 11:22:13.000000 torchtnt-nightly-2023.5.4/torchtnt/utils/loggers/file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2090 2023-05-04 11:22:13.000000 torchtnt-nightly-2023.5.4/torchtnt/utils/loggers/in_memory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1355 2023-05-04 11:22:13.000000 torchtnt-nightly-2023.5.4/torchtnt/utils/loggers/json.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1253 2023-05-04 11:22:13.000000 torchtnt-nightly-2023.5.4/torchtnt/utils/loggers/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4897 2023-05-04 11:22:13.000000 torchtnt-nightly-2023.5.4/torchtnt/utils/loggers/tensorboard.py
+-rw-r--r--   0 runner    (1001) docker     (123)      923 2023-05-04 11:22:13.000000 torchtnt-nightly-2023.5.4/torchtnt/utils/loggers/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      507 2023-05-04 11:22:13.000000 torchtnt-nightly-2023.5.4/torchtnt/utils/lr_scheduler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4760 2023-05-04 11:22:13.000000 torchtnt-nightly-2023.5.4/torchtnt/utils/memory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2538 2023-05-04 11:22:13.000000 torchtnt-nightly-2023.5.4/torchtnt/utils/misc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1151 2023-05-04 11:22:13.000000 torchtnt-nightly-2023.5.4/torchtnt/utils/oom.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2110 2023-05-04 11:22:13.000000 torchtnt-nightly-2023.5.4/torchtnt/utils/rank_zero_log.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2509 2023-05-04 11:22:13.000000 torchtnt-nightly-2023.5.4/torchtnt/utils/seed.py
+-rw-r--r--   0 runner    (1001) docker     (123)      847 2023-05-04 11:22:13.000000 torchtnt-nightly-2023.5.4/torchtnt/utils/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7670 2023-05-04 11:22:13.000000 torchtnt-nightly-2023.5.4/torchtnt/utils/timer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2205 2023-05-04 11:22:13.000000 torchtnt-nightly-2023.5.4/torchtnt/utils/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 11:23:43.000000 torchtnt-nightly-2023.5.4/torchtnt_nightly.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2537 2023-05-04 11:23:43.000000 torchtnt-nightly-2023.5.4/torchtnt_nightly.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2095 2023-05-04 11:23:43.000000 torchtnt-nightly-2023.5.4/torchtnt_nightly.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-04 11:23:43.000000 torchtnt-nightly-2023.5.4/torchtnt_nightly.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      188 2023-05-04 11:23:43.000000 torchtnt-nightly-2023.5.4/torchtnt_nightly.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-04 11:23:43.000000 torchtnt-nightly-2023.5.4/torchtnt_nightly.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-04 11:23:43.000000 torchtnt-nightly-2023.5.4/torchtnt_nightly.egg-info/zip-safe
```

### Comparing `torchtnt-nightly-2023.5.3/LICENSE` & `torchtnt-nightly-2023.5.4/LICENSE`

 * *Files identical despite different names*

### Comparing `torchtnt-nightly-2023.5.3/PKG-INFO` & `torchtnt-nightly-2023.5.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: torchtnt-nightly
-Version: 2023.5.3
+Version: 2023.5.4
 Summary: A lightweight library for PyTorch training tools and utilities
 Home-page: https://github.com/pytorch/tnt
 Author: PyTorch
 Author-email: daniellepintz@fb.com
 License: BSD-3
 Keywords: pytorch,torch,training,tools,utilities
 Classifier: Development Status :: 2 - Pre-Alpha
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: torchtnt-nightly Version: 2023.5.3 Summary: A
+Metadata-Version: 2.1 Name: torchtnt-nightly Version: 2023.5.4 Summary: A
 lightweight library for PyTorch training tools and utilities Home-page: https:/
 /github.com/pytorch/tnt Author: PyTorch Author-email: daniellepintz@fb.com
 License: BSD-3 Keywords: pytorch,torch,training,tools,utilities Classifier:
 Development Status :: 2 - Pre-Alpha Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research Classifier: License :: OSI
 Approved :: BSD License Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7 Classifier: Topic ::
```

### Comparing `torchtnt-nightly-2023.5.3/README.md` & `torchtnt-nightly-2023.5.4/README.md`

 * *Files identical despite different names*

### Comparing `torchtnt-nightly-2023.5.3/setup.py` & `torchtnt-nightly-2023.5.4/setup.py`

 * *Files identical despite different names*

### Comparing `torchtnt-nightly-2023.5.3/torchtnt/framework/__init__.py` & `torchtnt-nightly-2023.5.4/torchtnt/framework/__init__.py`

 * *Files identical despite different names*

### Comparing `torchtnt-nightly-2023.5.3/torchtnt/framework/_test_utils.py` & `torchtnt-nightly-2023.5.4/torchtnt/framework/_test_utils.py`

 * *Files identical despite different names*

### Comparing `torchtnt-nightly-2023.5.3/torchtnt/framework/auto_unit.py` & `torchtnt-nightly-2023.5.4/torchtnt/framework/auto_unit.py`

 * *Files identical despite different names*

### Comparing `torchtnt-nightly-2023.5.3/torchtnt/framework/callback.py` & `torchtnt-nightly-2023.5.4/torchtnt/framework/callback.py`

 * *Files identical despite different names*

### Comparing `torchtnt-nightly-2023.5.3/torchtnt/framework/callbacks/__init__.py` & `torchtnt-nightly-2023.5.4/torchtnt/framework/callbacks/__init__.py`

 * *Files identical despite different names*

### Comparing `torchtnt-nightly-2023.5.3/torchtnt/framework/callbacks/base_csv_writer.py` & `torchtnt-nightly-2023.5.4/torchtnt/framework/callbacks/base_csv_writer.py`

 * *Files identical despite different names*

### Comparing `torchtnt-nightly-2023.5.3/torchtnt/framework/callbacks/garbage_collector.py` & `torchtnt-nightly-2023.5.4/torchtnt/framework/callbacks/garbage_collector.py`

 * *Files identical despite different names*

### Comparing `torchtnt-nightly-2023.5.3/torchtnt/framework/callbacks/lambda_callback.py` & `torchtnt-nightly-2023.5.4/torchtnt/framework/callbacks/lambda_callback.py`

 * *Files identical despite different names*

### Comparing `torchtnt-nightly-2023.5.3/torchtnt/framework/callbacks/learning_rate_monitor.py` & `torchtnt-nightly-2023.5.4/torchtnt/framework/callbacks/learning_rate_monitor.py`

 * *Files identical despite different names*

### Comparing `torchtnt-nightly-2023.5.3/torchtnt/framework/callbacks/module_summary.py` & `torchtnt-nightly-2023.5.4/torchtnt/framework/callbacks/module_summary.py`

 * *Files identical despite different names*

### Comparing `torchtnt-nightly-2023.5.3/torchtnt/framework/callbacks/pytorch_profiler.py` & `torchtnt-nightly-2023.5.4/torchtnt/framework/callbacks/pytorch_profiler.py`

 * *Files identical despite different names*

### Comparing `torchtnt-nightly-2023.5.3/torchtnt/framework/callbacks/system_resources_monitor.py` & `torchtnt-nightly-2023.5.4/torchtnt/framework/callbacks/system_resources_monitor.py`

 * *Files identical despite different names*

### Comparing `torchtnt-nightly-2023.5.3/torchtnt/framework/callbacks/tensorboard_parameter_monitor.py` & `torchtnt-nightly-2023.5.4/torchtnt/framework/callbacks/tensorboard_parameter_monitor.py`

 * *Files identical despite different names*

### Comparing `torchtnt-nightly-2023.5.3/torchtnt/framework/callbacks/torchsnapshot_saver.py` & `torchtnt-nightly-2023.5.4/torchtnt/framework/callbacks/torchsnapshot_saver.py`

 * *Files 15% similar despite different names*

```diff
@@ -2,28 +2,32 @@
 # All rights reserved.
 #
 # This source code is licensed under the BSD-style license found in the
 # LICENSE file in the root directory of this source tree.
 
 import logging
 import os
-from typing import Dict, List, Optional, Set, Union
+from typing import Any, Dict, List, Optional, Set, Union
+
+import torch.distributed as dist
 
 from pyre_extensions import none_throws
 from torchsnapshot.snapshot import PendingSnapshot, Snapshot
 
 from torchtnt.framework.callback import Callback
 from torchtnt.framework.state import EntryPoint, State
 from torchtnt.framework.unit import (
     _Stateful as StatefulProtocol,
+    AppStateMixin,
     TEvalUnit,
     TPredictUnit,
     TTrainUnit,
 )
-from torchtnt.utils import rank_zero_info, rank_zero_warn
+from torchtnt.framework.utils import _construct_tracked_optimizers
+from torchtnt.utils import get_global_rank, rank_zero_info, rank_zero_warn
 
 try:
     import torchsnapshot
 
     _TStateful = torchsnapshot.Stateful
     _TORCHSNAPSHOT_AVAILABLE = True
 except Exception:
@@ -49,14 +53,16 @@
 
     Args:
         dirpath: Parent directory to save snapshots to.
         save_every_n_train_steps: Frequency of steps with which to save snapshots during the train epoch. If None, no intra-epoch snapshots are generated.
         save_every_n_epochs: Frequency of epochs with which to save snapshots during training. If None, no end-of-epoch snapshots are generated.
         replicated: A glob-pattern of replicated key names that indicate which application state entries have the same state across all processes.
             For more information, see https://pytorch.org/torchsnapshot/main/api_reference.html#torchsnapshot.Snapshot.take .
+
+            Note: If torch.distributed is available and default process group is initialized, the constructor will call a collective operation for rank 0 to broadcast the dirpath to all other ranks
     """
 
     def __init__(
         self,
         dirpath: str,
         *,
         save_every_n_train_steps: Optional[int] = None,
@@ -70,22 +76,41 @@
             )
         if save_every_n_epochs is not None and save_every_n_epochs < 0:
             raise ValueError(
                 f"Invalid value passed for save_every_n_epochs. Expected to receive either None or non-negative number, but received {save_every_n_epochs}"
             )
         self._save_every_n_epochs = save_every_n_epochs
         self._save_every_n_train_steps = save_every_n_train_steps
-        self._dirpath: str = dirpath
+        self._sync_dirpath_to_all_ranks(dirpath)
         self._replicated: Set[str] = set(replicated or [])
 
         self._prev_snapshot: Optional[PendingSnapshot] = None
 
+    def _sync_dirpath_to_all_ranks(self, dirpath: str) -> None:
+        if not (dist.is_available() and dist.is_initialized()):
+            self._dirpath: str = dirpath
+            return
+
+        dirpath_container = [dirpath] if get_global_rank() == 0 else [""]
+        # broadcast directory from global rank 0
+        dist.broadcast_object_list(dirpath_container, src=0)
+        updated_dirpath = dirpath_container[0]
+        if updated_dirpath != dirpath:
+            logger.warning(f"Updating dirpath to match rank 0: {updated_dirpath}")
+
+        self._dirpath: str = updated_dirpath
+
+    @property
+    def dirpath(self) -> str:
+        """Returns parent directory to save to."""
+        return self._dirpath
+
     def on_train_start(self, state: State, unit: TTrainUnit) -> None:
         """Validate there's no key collision for the app state."""
-        app_state = unit.app_state()
+        app_state = _app_state(unit)
         _check_app_state_collision(app_state)
 
     def on_train_step_end(self, state: State, unit: TTrainUnit) -> None:
         train_state = none_throws(state.train_state)
 
         global_step = train_state.progress.num_steps_completed
         save_every_n_train_steps = self._save_every_n_train_steps
@@ -177,15 +202,15 @@
         Since the class also manages saving the progress and dataloader states,
         this method handles their restoration. There are additional flags offered
         should the user want to skip loading these states. By default, the train progress,
         train dataloader, and eval progress are restored, if applicable.
         """
 
         _validate_snapshot_available()
-        app_state = unit.app_state()
+        app_state = _app_state(unit)
         _check_app_state_collision(app_state)
 
         snapshot = torchsnapshot.Snapshot(path)
 
         train_state = none_throws(state.train_state)
 
         rng_state = torchsnapshot.RNGState()
@@ -221,21 +246,29 @@
         )
 
 
 def _get_snapshot_save_path(dirpath: str, epoch: int, step: int) -> str:
     return os.path.join(dirpath, f"epoch_{epoch}_step_{step}")
 
 
+def _app_state(unit: AppStateMixin) -> Dict[str, Any]:
+    """Join together all of the tracked stateful entities to simplify registration of snapshottable states, deals with FSDP case"""
+    app_state = unit.app_state()
+    tracked_optimizers = _construct_tracked_optimizers(unit)  # handles fsdp
+    app_state.update(tracked_optimizers)
+    return app_state
+
+
 def _get_app_state(
     state: State, unit: TTrainUnit, replicated: Set[str], *, intra_epoch: bool
 ) -> Dict[str, _TStateful]:
     train_state = none_throws(state.train_state)
 
     train_progress = train_state.progress
-    app_state = unit.app_state()
+    app_state = _app_state(unit)
 
     rng_state = torchsnapshot.RNGState()
     app_state[_RNG_STATE_KEY] = rng_state
     app_state[_TRAIN_PROGRESS_STATE_KEY] = train_progress
     train_prog_glob = f"{_TRAIN_PROGRESS_STATE_KEY}/*"
     replicated.add(train_prog_glob)
```

### Comparing `torchtnt-nightly-2023.5.3/torchtnt/framework/callbacks/tqdm_progress_bar.py` & `torchtnt-nightly-2023.5.4/torchtnt/framework/callbacks/tqdm_progress_bar.py`

 * *Files identical despite different names*

### Comparing `torchtnt-nightly-2023.5.3/torchtnt/framework/callbacks/train_progress_monitor.py` & `torchtnt-nightly-2023.5.4/torchtnt/framework/callbacks/train_progress_monitor.py`

 * *Files identical despite different names*

### Comparing `torchtnt-nightly-2023.5.3/torchtnt/framework/evaluate.py` & `torchtnt-nightly-2023.5.4/torchtnt/framework/evaluate.py`

 * *Files identical despite different names*

### Comparing `torchtnt-nightly-2023.5.3/torchtnt/framework/fit.py` & `torchtnt-nightly-2023.5.4/torchtnt/framework/fit.py`

 * *Files identical despite different names*

### Comparing `torchtnt-nightly-2023.5.3/torchtnt/framework/predict.py` & `torchtnt-nightly-2023.5.4/torchtnt/framework/predict.py`

 * *Files identical despite different names*

### Comparing `torchtnt-nightly-2023.5.3/torchtnt/framework/progress.py` & `torchtnt-nightly-2023.5.4/torchtnt/framework/progress.py`

 * *Files identical despite different names*

### Comparing `torchtnt-nightly-2023.5.3/torchtnt/framework/state.py` & `torchtnt-nightly-2023.5.4/torchtnt/framework/state.py`

 * *Files identical despite different names*

### Comparing `torchtnt-nightly-2023.5.3/torchtnt/framework/train.py` & `torchtnt-nightly-2023.5.4/torchtnt/framework/train.py`

 * *Files identical despite different names*

### Comparing `torchtnt-nightly-2023.5.3/torchtnt/framework/unit.py` & `torchtnt-nightly-2023.5.4/torchtnt/framework/unit.py`

 * *Files identical despite different names*

### Comparing `torchtnt-nightly-2023.5.3/torchtnt/framework/utils.py` & `torchtnt-nightly-2023.5.4/torchtnt/framework/utils.py`

 * *Files identical despite different names*

### Comparing `torchtnt-nightly-2023.5.3/torchtnt/utils/__init__.py` & `torchtnt-nightly-2023.5.4/torchtnt/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `torchtnt-nightly-2023.5.3/torchtnt/utils/data/__init__.py` & `torchtnt-nightly-2023.5.4/torchtnt/utils/data/__init__.py`

 * *Files identical despite different names*

### Comparing `torchtnt-nightly-2023.5.3/torchtnt/utils/data/data_prefetcher.py` & `torchtnt-nightly-2023.5.4/torchtnt/utils/data/data_prefetcher.py`

 * *Files identical despite different names*

### Comparing `torchtnt-nightly-2023.5.3/torchtnt/utils/data/iterators.py` & `torchtnt-nightly-2023.5.4/torchtnt/utils/data/iterators.py`

 * *Files identical despite different names*

### Comparing `torchtnt-nightly-2023.5.3/torchtnt/utils/data/multi_dataloader.py` & `torchtnt-nightly-2023.5.4/torchtnt/utils/data/multi_dataloader.py`

 * *Files identical despite different names*

### Comparing `torchtnt-nightly-2023.5.3/torchtnt/utils/device.py` & `torchtnt-nightly-2023.5.4/torchtnt/utils/device.py`

 * *Files identical despite different names*

### Comparing `torchtnt-nightly-2023.5.3/torchtnt/utils/distributed.py` & `torchtnt-nightly-2023.5.4/torchtnt/utils/distributed.py`

 * *Files identical despite different names*

### Comparing `torchtnt-nightly-2023.5.3/torchtnt/utils/early_stop_checker.py` & `torchtnt-nightly-2023.5.4/torchtnt/utils/early_stop_checker.py`

 * *Files identical despite different names*

### Comparing `torchtnt-nightly-2023.5.3/torchtnt/utils/env.py` & `torchtnt-nightly-2023.5.4/torchtnt/utils/env.py`

 * *Files identical despite different names*

### Comparing `torchtnt-nightly-2023.5.3/torchtnt/utils/fsspec.py` & `torchtnt-nightly-2023.5.4/torchtnt/utils/fsspec.py`

 * *Files identical despite different names*

### Comparing `torchtnt-nightly-2023.5.3/torchtnt/utils/loggers/__init__.py` & `torchtnt-nightly-2023.5.4/torchtnt/utils/loggers/__init__.py`

 * *Files identical despite different names*

### Comparing `torchtnt-nightly-2023.5.3/torchtnt/utils/loggers/csv.py` & `torchtnt-nightly-2023.5.4/torchtnt/utils/loggers/csv.py`

 * *Files identical despite different names*

### Comparing `torchtnt-nightly-2023.5.3/torchtnt/utils/loggers/file.py` & `torchtnt-nightly-2023.5.4/torchtnt/utils/loggers/file.py`

 * *Files identical despite different names*

### Comparing `torchtnt-nightly-2023.5.3/torchtnt/utils/loggers/in_memory.py` & `torchtnt-nightly-2023.5.4/torchtnt/utils/loggers/in_memory.py`

 * *Files identical despite different names*

### Comparing `torchtnt-nightly-2023.5.3/torchtnt/utils/loggers/json.py` & `torchtnt-nightly-2023.5.4/torchtnt/utils/loggers/json.py`

 * *Files identical despite different names*

### Comparing `torchtnt-nightly-2023.5.3/torchtnt/utils/loggers/logger.py` & `torchtnt-nightly-2023.5.4/torchtnt/utils/loggers/logger.py`

 * *Files identical despite different names*

### Comparing `torchtnt-nightly-2023.5.3/torchtnt/utils/loggers/tensorboard.py` & `torchtnt-nightly-2023.5.4/torchtnt/utils/loggers/tensorboard.py`

 * *Files identical despite different names*

### Comparing `torchtnt-nightly-2023.5.3/torchtnt/utils/loggers/utils.py` & `torchtnt-nightly-2023.5.4/torchtnt/utils/loggers/utils.py`

 * *Files identical despite different names*

### Comparing `torchtnt-nightly-2023.5.3/torchtnt/utils/memory.py` & `torchtnt-nightly-2023.5.4/torchtnt/utils/memory.py`

 * *Files identical despite different names*

### Comparing `torchtnt-nightly-2023.5.3/torchtnt/utils/misc.py` & `torchtnt-nightly-2023.5.4/torchtnt/utils/misc.py`

 * *Files identical despite different names*

### Comparing `torchtnt-nightly-2023.5.3/torchtnt/utils/oom.py` & `torchtnt-nightly-2023.5.4/torchtnt/utils/oom.py`

 * *Files identical despite different names*

### Comparing `torchtnt-nightly-2023.5.3/torchtnt/utils/rank_zero_log.py` & `torchtnt-nightly-2023.5.4/torchtnt/utils/rank_zero_log.py`

 * *Files identical despite different names*

### Comparing `torchtnt-nightly-2023.5.3/torchtnt/utils/seed.py` & `torchtnt-nightly-2023.5.4/torchtnt/utils/seed.py`

 * *Files identical despite different names*

### Comparing `torchtnt-nightly-2023.5.3/torchtnt/utils/test_utils.py` & `torchtnt-nightly-2023.5.4/torchtnt/utils/test_utils.py`

 * *Files identical despite different names*

### Comparing `torchtnt-nightly-2023.5.3/torchtnt/utils/timer.py` & `torchtnt-nightly-2023.5.4/torchtnt/utils/timer.py`

 * *Files identical despite different names*

### Comparing `torchtnt-nightly-2023.5.3/torchtnt/utils/version.py` & `torchtnt-nightly-2023.5.4/torchtnt/utils/version.py`

 * *Files identical despite different names*

### Comparing `torchtnt-nightly-2023.5.3/torchtnt_nightly.egg-info/PKG-INFO` & `torchtnt-nightly-2023.5.4/torchtnt_nightly.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: torchtnt-nightly
-Version: 2023.5.3
+Version: 2023.5.4
 Summary: A lightweight library for PyTorch training tools and utilities
 Home-page: https://github.com/pytorch/tnt
 Author: PyTorch
 Author-email: daniellepintz@fb.com
 License: BSD-3
 Keywords: pytorch,torch,training,tools,utilities
 Classifier: Development Status :: 2 - Pre-Alpha
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: torchtnt-nightly Version: 2023.5.3 Summary: A
+Metadata-Version: 2.1 Name: torchtnt-nightly Version: 2023.5.4 Summary: A
 lightweight library for PyTorch training tools and utilities Home-page: https:/
 /github.com/pytorch/tnt Author: PyTorch Author-email: daniellepintz@fb.com
 License: BSD-3 Keywords: pytorch,torch,training,tools,utilities Classifier:
 Development Status :: 2 - Pre-Alpha Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research Classifier: License :: OSI
 Approved :: BSD License Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7 Classifier: Topic ::
```

### Comparing `torchtnt-nightly-2023.5.3/torchtnt_nightly.egg-info/SOURCES.txt` & `torchtnt-nightly-2023.5.4/torchtnt_nightly.egg-info/SOURCES.txt`

 * *Files identical despite different names*

