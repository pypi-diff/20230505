# Comparing `tmp/hi-ml-0.2.9.tar.gz` & `tmp/hi-ml-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/hi-ml-0.2.9.tar", last modified: Wed Nov  9 16:56:25 2022, max compression
+gzip compressed data, was "dist/hi-ml-0.3.0.tar", last modified: Fri May  5 17:32:53 2023, max compression
```

## Comparing `hi-ml-0.2.9.tar` & `hi-ml-0.3.0.tar`

### file list

```diff
@@ -1,59 +1,62 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-09 16:56:25.000000 hi-ml-0.2.9/
--rw-r--r--   0 runner    (1001) docker     (121)     1141 2022-11-09 16:56:08.000000 hi-ml-0.2.9/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)       76 2022-11-09 16:56:08.000000 hi-ml-0.2.9/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     2119 2022-11-09 16:56:25.000000 hi-ml-0.2.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1165 2022-11-09 16:56:08.000000 hi-ml-0.2.9/package_description.md
--rw-r--r--   0 runner    (1001) docker     (121)      211 2022-11-09 16:56:08.000000 hi-ml-0.2.9/run_requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-11-09 16:56:25.000000 hi-ml-0.2.9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     3861 2022-11-09 16:56:08.000000 hi-ml-0.2.9/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-09 16:56:25.000000 hi-ml-0.2.9/src/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-09 16:56:25.000000 hi-ml-0.2.9/src/health_ml/
--rw-r--r--   0 runner    (1001) docker     (121)      463 2022-11-09 16:56:08.000000 hi-ml-0.2.9/src/health_ml/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-09 16:56:25.000000 hi-ml-0.2.9/src/health_ml/configs/
--rw-r--r--   0 runner    (1001) docker     (121)    12445 2022-11-09 16:56:08.000000 hi-ml-0.2.9/src/health_ml/configs/hello_world.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-09 16:56:25.000000 hi-ml-0.2.9/src/health_ml/data/
--rw-r--r--   0 runner    (1001) docker     (121)      344 2022-11-09 16:56:08.000000 hi-ml-0.2.9/src/health_ml/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    35085 2022-11-09 16:56:08.000000 hi-ml-0.2.9/src/health_ml/deep_learning_config.py
--rw-r--r--   0 runner    (1001) docker     (121)     2220 2022-11-09 16:56:08.000000 hi-ml-0.2.9/src/health_ml/experiment_config.py
--rw-r--r--   0 runner    (1001) docker     (121)    13035 2022-11-09 16:56:08.000000 hi-ml-0.2.9/src/health_ml/lightning_container.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-09 16:56:25.000000 hi-ml-0.2.9/src/health_ml/losses/
--rw-r--r--   0 runner    (1001) docker     (121)      344 2022-11-09 16:56:08.000000 hi-ml-0.2.9/src/health_ml/losses/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    12014 2022-11-09 16:56:08.000000 hi-ml-0.2.9/src/health_ml/model_trainer.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-09 16:56:25.000000 hi-ml-0.2.9/src/health_ml/networks/
--rw-r--r--   0 runner    (1001) docker     (121)      344 2022-11-09 16:56:08.000000 hi-ml-0.2.9/src/health_ml/networks/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-09 16:56:25.000000 hi-ml-0.2.9/src/health_ml/networks/blocks/
--rw-r--r--   0 runner    (1001) docker     (121)      344 2022-11-09 16:56:08.000000 hi-ml-0.2.9/src/health_ml/networks/blocks/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-09 16:56:25.000000 hi-ml-0.2.9/src/health_ml/networks/layers/
--rw-r--r--   0 runner    (1001) docker     (121)      344 2022-11-09 16:56:08.000000 hi-ml-0.2.9/src/health_ml/networks/layers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    13135 2022-11-09 16:56:08.000000 hi-ml-0.2.9/src/health_ml/networks/layers/attention_layers.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-09 16:56:25.000000 hi-ml-0.2.9/src/health_ml/networks/nets/
--rw-r--r--   0 runner    (1001) docker     (121)      344 2022-11-09 16:56:08.000000 hi-ml-0.2.9/src/health_ml/networks/nets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    21270 2022-11-09 16:56:08.000000 hi-ml-0.2.9/src/health_ml/run_ml.py
--rwxr-xr-x   0 runner    (1001) docker     (121)    18032 2022-11-09 16:56:08.000000 hi-ml-0.2.9/src/health_ml/runner.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-09 16:56:25.000000 hi-ml-0.2.9/src/health_ml/utils/
--rw-r--r--   0 runner    (1001) docker     (121)      731 2022-11-09 16:56:08.000000 hi-ml-0.2.9/src/health_ml/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    10977 2022-11-09 16:56:08.000000 hi-ml-0.2.9/src/health_ml/utils/bag_utils.py
--rw-r--r--   0 runner    (1001) docker     (121)     5541 2022-11-09 16:56:08.000000 hi-ml-0.2.9/src/health_ml/utils/box_utils.py
--rw-r--r--   0 runner    (1001) docker     (121)     6507 2022-11-09 16:56:08.000000 hi-ml-0.2.9/src/health_ml/utils/checkpoint_handler.py
--rw-r--r--   0 runner    (1001) docker     (121)    11923 2022-11-09 16:56:08.000000 hi-ml-0.2.9/src/health_ml/utils/checkpoint_utils.py
--rw-r--r--   0 runner    (1001) docker     (121)     8023 2022-11-09 16:56:08.000000 hi-ml-0.2.9/src/health_ml/utils/common_utils.py
--rw-r--r--   0 runner    (1001) docker     (121)     7417 2022-11-09 16:56:08.000000 hi-ml-0.2.9/src/health_ml/utils/config_loader.py
--rw-r--r--   0 runner    (1001) docker     (121)     7779 2022-11-09 16:56:08.000000 hi-ml-0.2.9/src/health_ml/utils/data_augmentations.py
--rw-r--r--   0 runner    (1001) docker     (121)    17567 2022-11-09 16:56:08.000000 hi-ml-0.2.9/src/health_ml/utils/diagnostics.py
--rw-r--r--   0 runner    (1001) docker     (121)     1978 2022-11-09 16:56:08.000000 hi-ml-0.2.9/src/health_ml/utils/fixed_paths.py
--rw-r--r--   0 runner    (1001) docker     (121)     7007 2022-11-09 16:56:08.000000 hi-ml-0.2.9/src/health_ml/utils/lightning_loggers.py
--rw-r--r--   0 runner    (1001) docker     (121)    20298 2022-11-09 16:56:08.000000 hi-ml-0.2.9/src/health_ml/utils/logging.py
--rw-r--r--   0 runner    (1001) docker     (121)     7977 2022-11-09 16:56:08.000000 hi-ml-0.2.9/src/health_ml/utils/lr_scheduler.py
--rw-r--r--   0 runner    (1001) docker     (121)     1646 2022-11-09 16:56:08.000000 hi-ml-0.2.9/src/health_ml/utils/model_util.py
--rw-r--r--   0 runner    (1001) docker     (121)    12141 2022-11-09 16:56:08.000000 hi-ml-0.2.9/src/health_ml/utils/regression_test_utils.py
--rw-r--r--   0 runner    (1001) docker     (121)    26006 2022-11-09 16:56:08.000000 hi-ml-0.2.9/src/health_ml/utils/reports.py
--rw-r--r--   0 runner    (1001) docker     (121)     8895 2022-11-09 16:56:08.000000 hi-ml-0.2.9/src/health_ml/utils/serialization.py
--rw-r--r--   0 runner    (1001) docker     (121)    16599 2022-11-09 16:56:08.000000 hi-ml-0.2.9/src/health_ml/utils/split_dataset.py
--rw-r--r--   0 runner    (1001) docker     (121)      665 2022-11-09 16:56:08.000000 hi-ml-0.2.9/src/health_ml/utils/type_annotations.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-09 16:56:25.000000 hi-ml-0.2.9/src/hi_ml.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     2119 2022-11-09 16:56:24.000000 hi-ml-0.2.9/src/hi_ml.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1494 2022-11-09 16:56:25.000000 hi-ml-0.2.9/src/hi_ml.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-09 16:56:24.000000 hi-ml-0.2.9/src/hi_ml.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       55 2022-11-09 16:56:24.000000 hi-ml-0.2.9/src/hi_ml.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)      210 2022-11-09 16:56:24.000000 hi-ml-0.2.9/src/hi_ml.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       10 2022-11-09 16:56:24.000000 hi-ml-0.2.9/src/hi_ml.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-05 17:32:53.000000 hi-ml-0.3.0/
+-rw-r--r--   0 runner    (1001) docker     (122)     1141 2023-05-05 17:32:36.000000 hi-ml-0.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)       76 2023-05-05 17:32:36.000000 hi-ml-0.3.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)     2119 2023-05-05 17:32:53.000000 hi-ml-0.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     1165 2023-05-05 17:32:36.000000 hi-ml-0.3.0/package_description.md
+-rw-r--r--   0 runner    (1001) docker     (122)      225 2023-05-05 17:32:36.000000 hi-ml-0.3.0/run_requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-05-05 17:32:53.000000 hi-ml-0.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     3828 2023-05-05 17:32:36.000000 hi-ml-0.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-05 17:32:53.000000 hi-ml-0.3.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-05 17:32:53.000000 hi-ml-0.3.0/src/health_ml/
+-rw-r--r--   0 runner    (1001) docker     (122)      474 2023-05-05 17:32:36.000000 hi-ml-0.3.0/src/health_ml/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-05 17:32:53.000000 hi-ml-0.3.0/src/health_ml/configs/
+-rw-r--r--   0 runner    (1001) docker     (122)    13166 2023-05-05 17:32:36.000000 hi-ml-0.3.0/src/health_ml/configs/hello_world.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-05 17:32:53.000000 hi-ml-0.3.0/src/health_ml/data/
+-rw-r--r--   0 runner    (1001) docker     (122)      344 2023-05-05 17:32:36.000000 hi-ml-0.3.0/src/health_ml/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    31962 2023-05-05 17:32:36.000000 hi-ml-0.3.0/src/health_ml/deep_learning_config.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1248 2023-05-05 17:32:36.000000 hi-ml-0.3.0/src/health_ml/eval_runner.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4144 2023-05-05 17:32:36.000000 hi-ml-0.3.0/src/health_ml/experiment_config.py
+-rw-r--r--   0 runner    (1001) docker     (122)    14905 2023-05-05 17:32:36.000000 hi-ml-0.3.0/src/health_ml/lightning_container.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-05 17:32:53.000000 hi-ml-0.3.0/src/health_ml/losses/
+-rw-r--r--   0 runner    (1001) docker     (122)      344 2023-05-05 17:32:36.000000 hi-ml-0.3.0/src/health_ml/losses/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11742 2023-05-05 17:32:36.000000 hi-ml-0.3.0/src/health_ml/model_trainer.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-05 17:32:53.000000 hi-ml-0.3.0/src/health_ml/networks/
+-rw-r--r--   0 runner    (1001) docker     (122)      344 2023-05-05 17:32:36.000000 hi-ml-0.3.0/src/health_ml/networks/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-05 17:32:53.000000 hi-ml-0.3.0/src/health_ml/networks/blocks/
+-rw-r--r--   0 runner    (1001) docker     (122)      344 2023-05-05 17:32:36.000000 hi-ml-0.3.0/src/health_ml/networks/blocks/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-05 17:32:53.000000 hi-ml-0.3.0/src/health_ml/networks/layers/
+-rw-r--r--   0 runner    (1001) docker     (122)      344 2023-05-05 17:32:36.000000 hi-ml-0.3.0/src/health_ml/networks/layers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12693 2023-05-05 17:32:36.000000 hi-ml-0.3.0/src/health_ml/networks/layers/attention_layers.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-05 17:32:53.000000 hi-ml-0.3.0/src/health_ml/networks/nets/
+-rw-r--r--   0 runner    (1001) docker     (122)      344 2023-05-05 17:32:36.000000 hi-ml-0.3.0/src/health_ml/networks/nets/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)    20367 2023-05-05 17:32:36.000000 hi-ml-0.3.0/src/health_ml/runner.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12175 2023-05-05 17:32:36.000000 hi-ml-0.3.0/src/health_ml/runner_base.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12716 2023-05-05 17:32:36.000000 hi-ml-0.3.0/src/health_ml/training_runner.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-05 17:32:53.000000 hi-ml-0.3.0/src/health_ml/utils/
+-rw-r--r--   0 runner    (1001) docker     (122)      830 2023-05-05 17:32:36.000000 hi-ml-0.3.0/src/health_ml/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10571 2023-05-05 17:32:36.000000 hi-ml-0.3.0/src/health_ml/utils/bag_utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5358 2023-05-05 17:32:36.000000 hi-ml-0.3.0/src/health_ml/utils/box_utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7700 2023-05-05 17:32:36.000000 hi-ml-0.3.0/src/health_ml/utils/checkpoint_handler.py
+-rw-r--r--   0 runner    (1001) docker     (122)    22287 2023-05-05 17:32:36.000000 hi-ml-0.3.0/src/health_ml/utils/checkpoint_utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7857 2023-05-05 17:32:36.000000 hi-ml-0.3.0/src/health_ml/utils/common_utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7417 2023-05-05 17:32:36.000000 hi-ml-0.3.0/src/health_ml/utils/config_loader.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9953 2023-05-05 17:32:36.000000 hi-ml-0.3.0/src/health_ml/utils/data_augmentations.py
+-rw-r--r--   0 runner    (1001) docker     (122)    21038 2023-05-05 17:32:36.000000 hi-ml-0.3.0/src/health_ml/utils/diagnostics.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1978 2023-05-05 17:32:36.000000 hi-ml-0.3.0/src/health_ml/utils/fixed_paths.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6996 2023-05-05 17:32:36.000000 hi-ml-0.3.0/src/health_ml/utils/lightning_loggers.py
+-rw-r--r--   0 runner    (1001) docker     (122)    21251 2023-05-05 17:32:36.000000 hi-ml-0.3.0/src/health_ml/utils/logging.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7621 2023-05-05 17:32:36.000000 hi-ml-0.3.0/src/health_ml/utils/lr_scheduler.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1479 2023-05-05 17:32:36.000000 hi-ml-0.3.0/src/health_ml/utils/model_util.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2012 2023-05-05 17:32:36.000000 hi-ml-0.3.0/src/health_ml/utils/package_setup.py
+-rw-r--r--   0 runner    (1001) docker     (122)    20982 2023-05-05 17:32:36.000000 hi-ml-0.3.0/src/health_ml/utils/regression_test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)    26099 2023-05-05 17:32:36.000000 hi-ml-0.3.0/src/health_ml/utils/reports.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8773 2023-05-05 17:32:36.000000 hi-ml-0.3.0/src/health_ml/utils/serialization.py
+-rw-r--r--   0 runner    (1001) docker     (122)    16018 2023-05-05 17:32:36.000000 hi-ml-0.3.0/src/health_ml/utils/split_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (122)      665 2023-05-05 17:32:36.000000 hi-ml-0.3.0/src/health_ml/utils/type_annotations.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-05 17:32:53.000000 hi-ml-0.3.0/src/hi_ml.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     2119 2023-05-05 17:32:53.000000 hi-ml-0.3.0/src/hi_ml.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     1598 2023-05-05 17:32:53.000000 hi-ml-0.3.0/src/hi_ml.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-05 17:32:53.000000 hi-ml-0.3.0/src/hi_ml.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       55 2023-05-05 17:32:53.000000 hi-ml-0.3.0/src/hi_ml.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      224 2023-05-05 17:32:53.000000 hi-ml-0.3.0/src/hi_ml.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       10 2023-05-05 17:32:53.000000 hi-ml-0.3.0/src/hi_ml.egg-info/top_level.txt
```

### Comparing `hi-ml-0.2.9/LICENSE` & `hi-ml-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `hi-ml-0.2.9/PKG-INFO` & `hi-ml-0.3.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hi-ml
-Version: 0.2.9
+Version: 0.3.0
 Summary: Microsoft Health Futures package containing high level ML components
 Home-page: https://github.com/microsoft/hi-ml
 Author: Biomedical Imaging Team @ Microsoft Health Futures
 Author-email: innereyedev@microsoft.com
 License: MIT License
 Description: # Microsoft Health Intelligence Machine Learning Toolbox
```

### Comparing `hi-ml-0.2.9/package_description.md` & `hi-ml-0.3.0/package_description.md`

 * *Files identical despite different names*

### Comparing `hi-ml-0.2.9/setup.py` & `hi-ml-0.3.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -31,15 +31,15 @@
 # See also:
 # https://packaging.python.org/guides/publishing-package-distribution-releases-using-github-actions-ci-cd-workflows/
 # https://github.com/pypa/gh-action-pypi-publish
 GITHUB_REF_TAG_COMMIT = "refs/tags/v"
 
 github_ref = os.getenv("GITHUB_REF")
 if github_ref and github_ref.startswith(GITHUB_REF_TAG_COMMIT):
-    version = github_ref[len(GITHUB_REF_TAG_COMMIT):]
+    version = github_ref[len(GITHUB_REF_TAG_COMMIT) :]
 
 # Otherwise, if running from a GitHub Action, but not a tagged commit then GITHUB_RUN_NUMBER will be populated.
 # Use this as a post release number. For example if GITHUB_RUN_NUMBER = 124 then the version string will be
 # "0.1.2.post124". Although this is discouraged, see:
 # https://www.python.org/dev/peps/pep-0440/#post-releases
 # it is necessary here to avoid duplicate packages in Test.PyPI.
 if not version:
@@ -72,21 +72,17 @@
     author="Biomedical Imaging Team @ Microsoft Health Futures",
     author_email="innereyedev@microsoft.com",
     classifiers=[
         "Development Status :: 3 - Alpha",
         "Intended Audience :: Science/Research",
         "Topic :: Scientific/Engineering :: Medical Science Apps.",
         "License :: OSI Approved :: MIT License",
-        "Programming Language :: Python :: 3.7"
+        "Programming Language :: Python :: 3.7",
     ],
     keywords="Health Futures, Health Intelligence, AzureML",
     license="MIT License",
     packages=find_namespace_packages(where="src"),
     package_dir={"": "src"},
     include_package_data=True,
     install_requires=install_requires,
-    entry_points={
-        "console_scripts": [
-            "himl-runner = health_ml.runner:main"
-        ]
-    }
+    entry_points={"console_scripts": ["himl-runner = health_ml.runner:main"]},
 )
```

### Comparing `hi-ml-0.2.9/src/health_ml/configs/hello_world.py` & `hi-ml-0.3.0/src/health_ml/configs/hello_world.py`

 * *Files 4% similar despite different names*

```diff
@@ -12,14 +12,17 @@
 from torchmetrics import MeanAbsoluteError
 from torch.optim import Adam, Optimizer
 from torch.optim.lr_scheduler import StepLR, _LRScheduler
 from torch.utils.data import DataLoader, Dataset
 
 from health_ml.lightning_container import LightningContainer
 
+TEST_MSE_FILE = "test_mse.txt"
+TEST_MAE_FILE = "test_mae.txt"
+
 
 def _create_1d_regression_dataset(n: int = 100, seed: int = 0) -> torch.Tensor:
     """Creates a simple 1-D dataset of a noisy linear function.
 
     :param n: The number of datapoints to generate, defaults to 100
     :param seed: Random number generator seed, defaults to 0
     :return: A tensor that contains X values in [:, 0] and Y values in [:, 1]
@@ -75,27 +78,28 @@
 
 
 class HelloWorldDataModule(LightningDataModule):
     """
     A data module that gives the training, validation and test data for a simple 1-dim regression task.
     """
 
-    def __init__(self, crossval_count: int, crossval_index: int) -> None:
+    def __init__(self, crossval_count: int, crossval_index: Optional[int] = None, seed: int = 0) -> None:
         super().__init__()
         n_total = 200
-        xy = _create_1d_regression_dataset(n=n_total)
+        xy = _create_1d_regression_dataset(n=n_total, seed=seed)
         n_test = 40
         n_val = 50
         self.test = HelloWorldDataset(xy=xy[:n_test])
         if crossval_count <= 1:
-            self.val = HelloWorldDataset(xy=xy[n_test:(n_test + n_val)])
-            self.train = HelloWorldDataset(xy=xy[(n_test + n_val):])
+            self.val = HelloWorldDataset(xy=xy[n_test : (n_test + n_val)])
+            self.train = HelloWorldDataset(xy=xy[(n_test + n_val) :])
         else:
             # This could be done via a library function like sklearn's KFold function, but we don't want to add
             # scikit-learn as a dependency just for this example.
+            assert crossval_index is not None, "crossval_index must be set if crossval_count > 1"
             train, val = _split_crossval(xy[n_test:], crossval_count=crossval_count, crossval_index=crossval_index)
             self.val = HelloWorldDataset(xy=val)
             self.train = HelloWorldDataset(xy=train)
 
     def prepare_data(self, *args: Any, **kwargs: Any) -> None:
         pass
 
@@ -118,15 +122,15 @@
     """
 
     def __init__(self) -> None:
         super().__init__()
         self.model = torch.nn.Linear(in_features=1, out_features=1, bias=True)  # type: ignore
         self.test_mse: List[torch.Tensor] = []
         self.test_mae = MeanAbsoluteError()
-        self.run_extra_val_epoch = False
+        self._on_extra_val_epoch = False
 
     def forward(self, x: torch.Tensor) -> torch.Tensor:  # type: ignore
         """
         This method is part of the standard PyTorch Lightning interface. For an introduction, please see
         https://pytorch-lightning.readthedocs.io/en/stable/starter/converting.html
         It runs a forward pass of a tensor through the model.
 
@@ -224,18 +228,21 @@
         """
         This method is part of the standard PyTorch Lightning interface. For an introduction, please see
         https://pytorch-lightning.readthedocs.io/en/stable/starter/converting.html
         In this method, you can finish off anything to do with evaluating the model on the test set,
         for example writing aggregate metrics to disk.
         """
         average_mse = torch.mean(torch.stack(self.test_mse))
-        Path("test_mse.txt").write_text(str(average_mse.item()))
-        Path("test_mae.txt").write_text(str(self.test_mae.compute().item()))
+        Path(TEST_MSE_FILE).write_text(str(average_mse.item()))
+        Path(TEST_MAE_FILE).write_text(str(self.test_mae.compute().item()))
         self.log("test_mse", average_mse, on_epoch=True, on_step=False)
 
+    def on_run_extra_validation_epoch(self) -> None:
+        self._on_extra_val_epoch = True
+
 
 class HelloWorld(LightningContainer):
     """
     An example container for using the hi-ml runner. This container has methods
     to generate the actual Lightning model, and read out the datamodule that will be used for training.
     The number of training epochs is controlled at container level.
     You can train this model by running `python health_ml/runner.py --model=HelloWorld` on the local box,
@@ -258,17 +265,29 @@
     def get_data_module(self) -> LightningDataModule:
         assert self.local_dataset_dir is not None
         # If you would like to use the built-in cross validation functionality that runs training in parallel,
         # you need to provide the crossvalidation parameters in the LightningContainer to the datamodule. The
         # datamodule must carry out appropriate splitting of the data.
         return HelloWorldDataModule(crossval_count=self.crossval_count, crossval_index=self.crossval_index)
 
+    # This method is optional. Override it to supply a data module to use for evaluating the model on a new dataset.
+    # Only the test data loader from the data module will be used.
+    def get_eval_data_module(self) -> LightningDataModule:
+        return HelloWorldDataModule(crossval_count=1, seed=1)
+
     def get_callbacks(self) -> List[Callback]:
         if self.save_checkpoint:
-            return [ModelCheckpoint(dirpath=self.checkpoint_folder,
-                                    monitor="val_loss",
-                                    filename="checkpoint",
-                                    auto_insert_metric_name=False,
-                                    mode="min"),
-                    *super().get_callbacks()]
+            return [
+                ModelCheckpoint(
+                    dirpath=self.checkpoint_folder,
+                    monitor="val_loss",
+                    filename="checkpoint",
+                    auto_insert_metric_name=False,
+                    mode="min",
+                ),
+                *super().get_callbacks(),
+            ]
         else:
             return super().get_callbacks()
+
+    def get_additional_aml_run_tags(self) -> Dict[str, str]:
+        return {"max_epochs": str(self.max_epochs)}
```

### Comparing `hi-ml-0.2.9/src/health_ml/deep_learning_config.py` & `hi-ml-0.3.0/src/health_ml/deep_learning_config.py`

 * *Files 7% similar despite different names*

```diff
@@ -3,86 +3,105 @@
 #  Licensed under the MIT License (MIT). See LICENSE in the repo root for license information.
 #  ------------------------------------------------------------------------------------------
 from __future__ import annotations
 
 import logging
 import os
 import param
-import re
 from enum import Enum, unique
 from param import Parameterized
 from pathlib import Path
 from typing import Any, Dict, List, Optional
-from urllib.parse import urlparse
 
 from azureml.train.hyperdrive import HyperDriveConfig
 
 from health_azure import create_crossval_hyperdrive_config
-from health_azure.himl import (create_grid_hyperdrive_config, create_crossval_hyperparam_args_v2,
-                               create_grid_hyperparam_args_v2)
-from health_azure.amulet import (ENV_AMLT_PROJECT_NAME, ENV_AMLT_INPUT_OUTPUT,
-                                 ENV_AMLT_SNAPSHOT_DIR, ENV_AMLT_AZ_BATCHAI_DIR,
-                                 is_amulet_job, get_amulet_aml_working_dir)
-from health_azure.utils import (RUN_CONTEXT, PathOrString, is_global_rank_zero, is_running_in_azure_ml)
+from health_azure.himl import (
+    create_grid_hyperdrive_config,
+    create_crossval_hyperparam_args_v2,
+    create_grid_hyperparam_args_v2,
+)
+from health_azure.amulet import (
+    ENV_AMLT_PROJECT_NAME,
+    ENV_AMLT_INPUT_OUTPUT,
+    ENV_AMLT_SNAPSHOT_DIR,
+    ENV_AMLT_AZ_BATCHAI_DIR,
+    is_amulet_job,
+    get_amulet_aml_working_dir,
+)
+from health_azure.utils import RUN_CONTEXT, PathOrString, is_global_rank_zero, is_running_in_azure_ml
 from health_ml.utils import fixed_paths
-from health_ml.utils.common_utils import (CHECKPOINT_FOLDER,
-                                          create_unique_timestamp_id,
-                                          DEFAULT_AML_UPLOAD_DIR,
-                                          DEFAULT_LOGS_DIR_NAME)
+from health_ml.utils.checkpoint_utils import CheckpointParser
+from health_ml.utils.common_utils import (
+    CHECKPOINT_FOLDER,
+    create_unique_timestamp_id,
+    DEFAULT_AML_UPLOAD_DIR,
+    DEFAULT_LOGS_DIR_NAME,
+)
 from health_ml.utils.type_annotations import IntOrFloat, TupleFloat2
 
 
 @unique
 class LRWarmUpType(Enum):
     """
     Supported LR warm up types for model training
     """
+
     NoWarmUp = "NoWarmUp"
     Linear = "Linear"
 
 
 @unique
 class LRSchedulerType(Enum):
     """
     Supported lr scheduler types for model training
     """
+
     Exponential = "Exponential"
     Step = "Step"
     Polynomial = "Polynomial"
     Cosine = "Cosine"
     MultiStep = "MultiStep"
 
 
 @unique
 class OptimizerType(Enum):
     """
     Supported optimizers for model training
     """
+
     Adam = "Adam"
     AMSGrad = "AMSGrad"
     SGD = "SGD"
     RMSprop = "RMSprop"
 
 
 class ExperimentFolderHandler(Parameterized):
     """High level config to abstract the file system related settings for experiments"""
-    outputs_folder: Path = param.ClassSelector(class_=Path, default=Path(), instantiate=False,
-                                               doc="The folder where all training and test outputs should go.")
-    logs_folder: Path = param.ClassSelector(class_=Path, default=Path(), instantiate=False,
-                                            doc="The folder for all log files and Tensorboard event files")
-    project_root: Path = param.ClassSelector(class_=Path, default=Path(), instantiate=False,
-                                             doc="The root folder for the codebase that triggers the training run.")
-    run_folder: Path = param.ClassSelector(class_=Path, default=Path(), instantiate=False,
-                                           doc="The folder that contains outputs and the logs subfolder.")
+
+    outputs_folder: Path = param.ClassSelector(
+        class_=Path, default=Path(), instantiate=False, doc="The folder where all training and test outputs should go."
+    )
+    logs_folder: Path = param.ClassSelector(
+        class_=Path, default=Path(), instantiate=False, doc="The folder for all log files and Tensorboard event files"
+    )
+    project_root: Path = param.ClassSelector(
+        class_=Path,
+        default=Path(),
+        instantiate=False,
+        doc="The root folder for the codebase that triggers the training run.",
+    )
+    run_folder: Path = param.ClassSelector(
+        class_=Path, default=Path(), instantiate=False, doc="The folder that contains outputs and the logs subfolder."
+    )
 
     @staticmethod
-    def create(project_root: Path,
-               is_offline_run: bool,
-               model_name: str,
-               output_to: Optional[Path] = None) -> ExperimentFolderHandler:
+    def create(
+        project_root: Path, is_offline_run: bool, model_name: str, output_to: Optional[Path] = None
+    ) -> ExperimentFolderHandler:
         """
         Creates a new object that holds output folder configurations. When running inside of AzureML, the output
         folders will be directly under the project root. If not running inside AzureML, a folder with a timestamp
         will be created for all outputs and logs.
 
         :param project_root: The root folder that contains the code that submitted the present training run.
         When running inside the hi-ml repository, it is the git repo root. When consuming hi-ml as a package,
@@ -120,139 +139,125 @@
                 outputs_folder = project_root / DEFAULT_AML_UPLOAD_DIR
                 logs_folder = project_root / DEFAULT_LOGS_DIR_NAME
             else:
                 # Job submitted via Amulet
                 amlt_root_folder = Path(os.environ[ENV_AMLT_INPUT_OUTPUT])
                 project_name = os.environ[ENV_AMLT_PROJECT_NAME]
                 snapshot_dir = get_amulet_aml_working_dir()
-                assert snapshot_dir, \
-                    f"Either {ENV_AMLT_SNAPSHOT_DIR} or {ENV_AMLT_AZ_BATCHAI_DIR} must exist in env vars"
-                print(f"Found the following environment variables set by Amulet: "
-                      f"AZURE_ML_INPUT_OUTPUT: {amlt_root_folder}, AZUREML_ARM_PROJECT_NAME: {project_name}")
+                assert (
+                    snapshot_dir
+                ), f"Either {ENV_AMLT_SNAPSHOT_DIR} or {ENV_AMLT_AZ_BATCHAI_DIR} must exist in env vars"
+                print(
+                    f"Found the following environment variables set by Amulet: "
+                    f"AZURE_ML_INPUT_OUTPUT: {amlt_root_folder}, AZUREML_ARM_PROJECT_NAME: {project_name}"
+                )
                 run_id = RUN_CONTEXT.id
                 run_folder = amlt_root_folder / "projects" / project_name / "amlt-code" / run_id
                 outputs_folder = snapshot_dir / DEFAULT_AML_UPLOAD_DIR
                 logs_folder = snapshot_dir / DEFAULT_LOGS_DIR_NAME
 
-        print(f"Run outputs folder: {outputs_folder}")
-        print(f"Logs folder: {logs_folder}")
-        print(f"Run root directory: {run_folder}")
+        logging.info(f"Run outputs folder: {outputs_folder}")
+        logging.info(f"Logs folder: {logs_folder}")
+        logging.info(f"Run root directory: {run_folder}")
         return ExperimentFolderHandler(
-            outputs_folder=outputs_folder,
-            logs_folder=logs_folder,
-            project_root=project_root,
-            run_folder=run_folder
+            outputs_folder=outputs_folder, logs_folder=logs_folder, project_root=project_root, run_folder=run_folder
         )
 
 
-SRC_CHECKPOINT_FORMAT_DOC = ("<AzureML_run_id>:<optional/custom/path/to/checkpoints/><filename.ckpt>"
-                             "If no custom path is provided (e.g., <AzureML_run_id>:<filename.ckpt>)"
-                             "the checkpoint will be downloaded from the default checkpoint folder "
-                             "(e.g., 'outputs/checkpoints/'). If no filename is provided, (e.g., "
-                             "`src_checkpoint=<AzureML_run_id>`) the latest checkpoint (last.ckpt) "
-                             "will be used to initialize the model."
-                             )
-
-
 class WorkflowParams(param.Parameterized):
     """
     This class contains all parameters that affect how the whole training and testing workflow is executed.
     """
+
     random_seed: int = param.Integer(42, doc="The seed to use for all random number generators.")
-    src_checkpoint: str = param.String(default="",
-                                       doc="This flag can be used in 3 different scenarios:"
-                                           "1- Resume training from a checkpoint to train longer."
-                                           "2- Run inference-only using `run_inference_only` flag jointly."
-                                           "3- Transfer learning from a pretrained model checkpoint."
-                                           "We currently support three types of checkpoints: "
-                                           "    a. A local checkpoint folder that contains a checkpoint file."
-                                           "    b. A URL to a remote checkpoint to be downloaded."
-                                           "    c. A previous azureml run id where the checkpoint is supposed to be "
-                                           "       saved ('outputs/checkpoints/' folder by default.)"
-                                           "For the latter case 'c' : src_checkpoint should be in the format of "
-                                           f"{SRC_CHECKPOINT_FORMAT_DOC}")
-    crossval_count: int = param.Integer(default=1, bounds=(0, None),
-                                        doc="The number of splits to use when doing cross-validation. "
-                                            "Use 1 to disable cross-validation")
-    crossval_index: int = param.Integer(default=0, bounds=(0, None),
-                                        doc="When doing cross validation, this is the index of the current "
-                                            "split. Valid values: 0 .. (crossval_count -1)")
-    hyperdrive: bool = param.Boolean(False,
-                                     doc="If True, use the Hyperdrive configuration specified in the "
-                                         "LightningContainer to run hyperparameter tuning. If False, just "
-                                         "run a plain single training job. This cannot be combined with "
-                                         "the flags --different_seeds or --crossval_count.")
-    regression_test_folder: Optional[Path] = \
-        param.ClassSelector(class_=Path, default=None, allow_None=True,
-                            doc="A path to a folder that contains a set of files. At the end of training and "
-                                "model evaluation, all files given in that folder must be present in the job's output "
-                                "folder, and their contents must match exactly. When running in AzureML, you need to "
-                                "ensure that this folder is part of the snapshot that gets uploaded. The path should "
-                                "be relative to the repository root directory.")
-    regression_test_csv_tolerance: float = \
-        param.Number(default=0.0, allow_None=False,
-                     doc="When comparing CSV files during regression tests, use this value as the maximum allowed "
-                         "relative difference of actual and expected results. Default: 0.0 (must match exactly)")
+    src_checkpoint: CheckpointParser = param.ClassSelector(
+        class_=CheckpointParser, default=None, instantiate=False, doc=CheckpointParser.DOC
+    )
+    crossval_count: int = param.Integer(
+        default=1,
+        bounds=(0, None),
+        doc="The number of splits to use when doing cross-validation. Use 1 to disable cross-validation",
+    )
+    crossval_index: Optional[int] = param.Integer(
+        default=None,
+        bounds=(0, None),
+        allow_None=True,
+        doc="When doing cross validation, this is the index of the current "
+        "split. Valid values: 0 .. (crossval_count -1). Default: None"
+        "when launching a cross-validation run, this will be set by "
+        "the hyperdrive config. To submit a single cross-validation fold,"
+        "set this to the fold index along with --crossval_count > 1.",
+    )
+    hyperdrive: bool = param.Boolean(
+        False,
+        doc="If True, use the Hyperdrive configuration specified in the "
+        "LightningContainer to run hyperparameter tuning. If False, just "
+        "run a plain single training job. This cannot be combined with "
+        "the flags --different_seeds or --crossval_count.",
+    )
+    regression_test_folder: Optional[Path] = param.ClassSelector(
+        class_=Path,
+        default=None,
+        allow_None=True,
+        doc="A path to a folder that contains a set of files. At the end of training and "
+        "model evaluation, all files given in that folder must be present in the job's output "
+        "folder, and their contents must match exactly. When running in AzureML, you need to "
+        "ensure that this folder is part of the snapshot that gets uploaded. The path should "
+        "be relative to the repository root directory.",
+    )
+    regression_test_csv_tolerance: float = param.Number(
+        default=0.0,
+        allow_None=False,
+        doc="When comparing CSV files during regression tests, use this value as the maximum allowed "
+        "relative difference of actual and expected results. Default: 0.0 (must match exactly)",
+    )
     regression_metrics: str = param.String(default=None, doc="A list of names of metrics to compare")
-    run_inference_only: bool = param.Boolean(False, doc="If True, run only inference and skip training after loading"
-                                                        "model weights from the specified checkpoint in "
-                                                        "`src_checkpoint` flag. If False, run training and inference.")
+    run_inference_only: bool = param.Boolean(
+        False,
+        doc="If True, run only inference and skip training after loading"
+        "model weights from the specified checkpoint in "
+        "`src_checkpoint` flag. Inference is run on both validation "
+        "and test sets. If False, run training and inference.",
+    )
+    resume_training: bool = param.Boolean(False, doc="If True, resume training from the src_checkpoint.")
     tag: str = param.String(doc="A string that will be used as the display name of the run in AzureML.")
-    experiment: str = param.String(default="", doc="The name of the AzureML experiment to use for this run. If not "
-                                   "provided, the name of the model class will be used.")
-    log_from_vm: bool = param.Boolean(False, doc="If True, a training run outside AzureML will still log its "
-                                      "metrics to AzureML. Both intermediate validation metrics and final test results"
-                                      "will be recorded. You need to have an AzureML workspace config.json file "
-                                      "and will be asked for interactive authentication.")
-    different_seeds: int = param.Integer(default=0, bounds=(0, None),
-                                         doc="If > 0, run the same training job multiple times with different seeds. "
-                                         "This uses AzureML hyperdrive to run multiple jobs in parallel, and hence "
-                                         "cannot be used when running outside AzureML. "
-                                         "This cannot be combined with the --hyperdrive or the --crossval_count flags.")
+    experiment: str = param.String(
+        default="",
+        doc="The name of the AzureML experiment to use for this run. If not "
+        "provided, the name of the model class will be used.",
+    )
+    log_from_vm: bool = param.Boolean(
+        False,
+        doc="If True, a training run outside AzureML will still log its "
+        "metrics to AzureML. Both intermediate validation metrics and final test results"
+        "will be recorded. You need to have an AzureML workspace config.json file "
+        "and will be asked for interactive authentication.",
+    )
+    different_seeds: int = param.Integer(
+        default=0,
+        bounds=(0, None),
+        doc="If > 0, run the same training job multiple times with different seeds. "
+        "This uses AzureML hyperdrive to run multiple jobs in parallel, and hence "
+        "cannot be used when running outside AzureML. "
+        "This cannot be combined with the --hyperdrive or the --crossval_count flags.",
+    )
 
     CROSSVAL_INDEX_ARG_NAME = "crossval_index"
     CROSSVAL_COUNT_ARG_NAME = "crossval_count"
     RANDOM_SEED_ARG_NAME = "random_seed"
 
-    @property
-    def src_checkpoint_is_url(self) -> bool:
-        try:
-            result = urlparse(self.src_checkpoint)
-            return all([result.scheme, result.netloc])
-        except ValueError:
-            return False
-
-    @property
-    def src_checkpoint_is_local_file(self) -> bool:
-        return Path(self.src_checkpoint).is_file()
-
-    @property
-    def src_checkpoint_is_aml_run_id(self) -> bool:
-        match = re.match(r"[_\w-]*$", self.src_checkpoint.split(":")[0])
-        return match is not None and not self.src_checkpoint_is_url and not self.src_checkpoint_is_local_file
-
-    @property
-    def is_valid_src_checkpoint(self) -> bool:
-        if self.src_checkpoint:
-            return self.src_checkpoint_is_local_file or self.src_checkpoint_is_url or self.src_checkpoint_is_aml_run_id
-        return True
-
     def validate(self) -> None:
-        if not self.is_valid_src_checkpoint:
-            raise ValueError(f"Invalid src_checkpoint: {self.src_checkpoint}. Please provide a valid URL, local file "
-                             "or azureml run id.")
-        if self.crossval_count > 1:
+        if self.crossval_count > 1 and self.crossval_index is not None:
             if not (0 <= self.crossval_index < self.crossval_count):
                 raise ValueError(f"Attribute crossval_index out of bounds (crossval_count = {self.crossval_count})")
 
         if self.run_inference_only and not self.src_checkpoint:
-            raise ValueError("Cannot run inference without a src_checkpoint. Please specify a valid src_checkpoint."
-                             "You can either use a URL, a local file or an azureml run id. For custom checkpoint paths "
-                             "within an azureml run, (other than last.ckpt), provide a src_checkpoint in the format."
-                             f"{SRC_CHECKPOINT_FORMAT_DOC}")
+            raise ValueError(f"Cannot run inference without a src_checkpoint. {CheckpointParser.INFO_MESSAGE}")
+        if self.resume_training and not self.src_checkpoint:
+            raise ValueError(f"Cannot resume training without a src_checkpoint. {CheckpointParser.INFO_MESSAGE}")
 
     @property
     def is_running_in_aml(self) -> bool:
         """
         Whether the current run is executing inside Azure ML
 
         :return: True if the run is executing inside Azure ML, or False if outside AzureML.
@@ -263,104 +268,135 @@
         """
         Returns the random seed set as part of this configuration. If the configuration corresponds
         to a cross validation split, then the cross validation fold index will be added to the
         set random seed in order to return the effective random seed.
         :return:
         """
         seed = self.random_seed
-        if self.is_crossvalidation_enabled:
+        if self.is_crossvalidation_child_run:
             # Offset the random seed based on the cross validation split index so each
             # fold has a different initial random state. Cross validation index 0 will have
             # a different seed from a non cross validation run.
+            assert self.crossval_index is not None, "crossval_index must be set for cross validation child runs"
             seed += self.crossval_index + 1
         return seed
 
     @property
-    def is_crossvalidation_enabled(self) -> bool:
+    def is_crossvalidation_parent_run(self) -> bool:
+        """
+        Returns True if the present parameters indicate that this is cross-validation parent run that should trigger
+        a hyperdrive run.
+        """
+        return self.crossval_count > 1 and self.crossval_index is None
+
+    @property
+    def is_crossvalidation_child_run(self) -> bool:
         """
-        Returns True if the present parameters indicate that cross-validation should be used.
+        Returns True if the present parameters indicate that this is a cross-validation child run.
         """
-        return self.crossval_count > 1
+        return self.crossval_count > 1 and self.crossval_index is not None
 
     def get_crossval_hyperdrive_config(self) -> HyperDriveConfig:
         # For crossvalidation, the name of the metric to monitor does not matter because no early termination or such
         # is specified.
-        return create_crossval_hyperdrive_config(num_splits=self.crossval_count,
-                                                 cross_val_index_arg_name=self.CROSSVAL_INDEX_ARG_NAME,
-                                                 metric_name="val/loss"
-                                                 )
+        return create_crossval_hyperdrive_config(
+            num_splits=self.crossval_count,
+            cross_val_index_arg_name=self.CROSSVAL_INDEX_ARG_NAME,
+            metric_name="val/loss",
+        )
 
     def get_different_seeds_hyperdrive_config(self) -> HyperDriveConfig:
         """Returns a configuration object for AzureML Hyperdrive that varies the random seed for each run."""
-        return create_grid_hyperdrive_config(values=list(map(str, range(self.different_seeds))),
-                                             argument_name=self.RANDOM_SEED_ARG_NAME,
-                                             metric_name="val/loss"
-                                             )
+        return create_grid_hyperdrive_config(
+            values=list(map(str, range(self.different_seeds))),
+            argument_name=self.RANDOM_SEED_ARG_NAME,
+            metric_name="val/loss",
+        )
 
     def get_crossval_hyperparam_args_v2(self) -> Dict[str, Any]:
         """
         Wrapper function to create hyperparameter search arguments specifically for running cross validation
         with AML SDK v2
 
         :return: A dictionary of hyperparameter search arguments and values.
         """
-        return create_crossval_hyperparam_args_v2(num_splits=self.crossval_count,
-                                                  cross_val_index_arg_name=self.CROSSVAL_INDEX_ARG_NAME,
-                                                  metric_name="val/loss")
+        return create_crossval_hyperparam_args_v2(
+            num_splits=self.crossval_count,
+            cross_val_index_arg_name=self.CROSSVAL_INDEX_ARG_NAME,
+            metric_name="val/loss",
+        )
 
     def get_grid_hyperparam_args_v2(self) -> Dict[str, Any]:
         """
         Wrapper function to create hyperparameter search arguments specifically for running grid search
         with AML SDK v2
 
         :return: A dictionary of hyperparameter search arguments and values.
         """
-        return create_grid_hyperparam_args_v2(values=list(map(str, range(self.different_seeds))),
-                                              argument_name=self.RANDOM_SEED_ARG_NAME,
-                                              metric_name="val/loss")
+        return create_grid_hyperparam_args_v2(
+            values=list(map(str, range(self.different_seeds))),
+            argument_name=self.RANDOM_SEED_ARG_NAME,
+            metric_name="val/loss",
+        )
 
 
 class DatasetParams(param.Parameterized):
     datastore: str = param.String(default="", doc="Datastore to look for data in")
-    azure_datasets: List[str] = param.List(default=[], class_=str,
-                                           doc="If provided, the ID of one or more datasets to use when running in"
-                                               " AzureML. This dataset must exist as a folder of the same name "
-                                               "in the 'datasets' container in the datasets storage account. This "
-                                               "dataset will be mounted and made available at the 'local_dataset' "
-                                               "path when running in AzureML.")
-    local_datasets: List[Path] = param.List(default=[], class_=Path,
-                                            doc="A list of one or more paths to the dataset to use, when training"
-                                                " outside of Azure ML.")
-    dataset_mountpoints: List[Path] = param.List(default=[], class_=Path,
-                                                 doc="The path at which the AzureML dataset should be made "
-                                                     "available via mounting or downloading. This only affects "
-                                                     "jobs running in AzureML. If empty, use a random "
-                                                     "mount/download point.")
+    azure_datasets: List[str] = param.List(
+        default=[],
+        class_=str,
+        doc="If provided, the ID of one or more datasets to use when running in"
+        " AzureML. This dataset must exist as a folder of the same name "
+        "in the 'datasets' container in the datasets storage account. This "
+        "dataset will be mounted and made available at the 'local_dataset' "
+        "path when running in AzureML.",
+    )
+    local_datasets: List[Path] = param.List(
+        default=[],
+        class_=Path,
+        doc="A list of one or more paths to the dataset to use, when training outside of Azure ML.",
+    )
+    dataset_mountpoints: List[Path] = param.List(
+        default=[],
+        class_=Path,
+        doc="The path at which the AzureML dataset should be made "
+        "available via mounting or downloading. This only affects "
+        "jobs running in AzureML. If empty, use a random "
+        "mount/download point.",
+    )
 
     def validate(self) -> None:
         if (not self.azure_datasets) and (not self.local_datasets):
             raise ValueError("Either local_datasets or azure_datasets must be set.")
 
         if self.dataset_mountpoints and len(self.azure_datasets) != len(self.dataset_mountpoints):
-            raise ValueError(f"Expected the number of azure datasets to equal the number of mountpoints, "
-                             f"got datasets [{','.join(self.azure_datasets)}] "
-                             f"and mountpoints [{','.join([str(m) for m in self.dataset_mountpoints])}]")
+            raise ValueError(
+                f"Expected the number of azure datasets to equal the number of mountpoints, "
+                f"got datasets [{','.join(self.azure_datasets)}] "
+                f"and mountpoints [{','.join([str(m) for m in self.dataset_mountpoints])}]"
+            )
 
 
 class OutputParams(param.Parameterized):
-    output_to: Optional[Path] = param.ClassSelector(class_=Path, default=None,
-                                                    doc="If provided, the run outputs will be written to the given "
-                                                        "folder. If not provided, outputs will go into a subfolder "
-                                                        "of the project root folder.")
-    file_system_config: ExperimentFolderHandler = param.ClassSelector(default=ExperimentFolderHandler(),
-                                                                      class_=ExperimentFolderHandler,
-                                                                      instantiate=False,
-                                                                      doc="File system related configs")
-    _model_name: str = param.String("", doc="The human readable name of the model (for example, Liver). This is "
-                                            "usually set from the class name.")
+    output_to: Optional[Path] = param.ClassSelector(
+        class_=Path,
+        default=None,
+        doc="If provided, the run outputs will be written to the given "
+        "folder. If not provided, outputs will go into a subfolder "
+        "of the project root folder.",
+    )
+    file_system_config: ExperimentFolderHandler = param.ClassSelector(
+        default=ExperimentFolderHandler(),
+        class_=ExperimentFolderHandler,
+        instantiate=False,
+        doc="File system related configs",
+    )
+    _model_name: str = param.String(
+        "", doc="The human readable name of the model (for example, Liver). This is usually set from the class name."
+    )
 
     @property
     def model_name(self) -> str:
         """
         Gets the human readable name of the model (e.g., Liver). This is usually set from the class name.
 
         :return: A model name as a string.
@@ -384,15 +420,15 @@
 
         :param project_root: The root folder for the codebase that triggers the training run.
         """
         self.file_system_config = ExperimentFolderHandler.create(
             project_root=project_root,
             model_name=self.model_name,
             is_offline_run=not is_running_in_azure_ml(RUN_CONTEXT),
-            output_to=self.output_to
+            output_to=self.output_to,
         )
 
     @property
     def outputs_folder(self) -> Path:
         """Gets the full path in which the model outputs should be stored."""
         return self.file_system_config.outputs_folder
 
@@ -405,60 +441,68 @@
     def checkpoint_folder(self) -> Path:
         """Gets the full path in which the model checkpoints should be stored during training."""
         return self.outputs_folder / CHECKPOINT_FOLDER
 
 
 class OptimizerParams(param.Parameterized):
     l_rate: float = param.Number(1e-4, doc="The initial learning rate", bounds=(0, None))
-    _min_l_rate: float = param.Number(0.0,
-                                      doc="The minimum learning rate for the Polynomial and Cosine schedulers.",
-                                      bounds=(0.0, None))
-    l_rate_scheduler: LRSchedulerType = param.ClassSelector(default=LRSchedulerType.Polynomial,
-                                                            class_=LRSchedulerType,
-                                                            instantiate=False,
-                                                            doc="Learning rate decay method (Cosine, Polynomial, "
-                                                                "Step, MultiStep or Exponential)")
-    l_rate_exponential_gamma: float = param.Number(0.9, doc="Controls the rate of decay for the Exponential "
-                                                            "LR scheduler.")
-    l_rate_step_gamma: float = param.Number(0.1, doc="Controls the rate of decay for the "
-                                                     "Step LR scheduler.")
-    l_rate_step_step_size: int = param.Integer(50, bounds=(0, None),
-                                               doc="The step size for Step LR scheduler")
-    l_rate_multi_step_gamma: float = param.Number(0.1, doc="Controls the rate of decay for the "
-                                                           "MultiStep LR scheduler.")
-    l_rate_multi_step_milestones: Optional[List[int]] = param.List(None, bounds=(1, None),
-                                                                   allow_None=True, class_=int,
-                                                                   doc="The milestones for MultiStep decay.")
-    l_rate_polynomial_gamma: float = param.Number(1e-4, doc="Controls the rate of decay for the "
-                                                            "Polynomial LR scheduler.")
-    l_rate_warmup: LRWarmUpType = param.ClassSelector(default=LRWarmUpType.NoWarmUp, class_=LRWarmUpType,
-                                                      instantiate=False,
-                                                      doc="The type of learning rate warm up to use. "
-                                                          "Can be NoWarmUp (default) or Linear.")
-    l_rate_warmup_epochs: int = param.Integer(0, bounds=(0, None),
-                                              doc="Number of warmup epochs (linear warmup) before the "
-                                                  "scheduler starts decaying the learning rate. "
-                                                  "For example, if you are using MultiStepLR with "
-                                                  "milestones [50, 100, 200] and warmup epochs = 100, warmup "
-                                                  "will last for 100 epochs and the first decay of LR "
-                                                  "will happen on epoch 150")
-    optimizer_type: OptimizerType = param.ClassSelector(default=OptimizerType.Adam, class_=OptimizerType,
-                                                        instantiate=False, doc="The optimizer_type to use")
+    _min_l_rate: float = param.Number(
+        0.0, doc="The minimum learning rate for the Polynomial and Cosine schedulers.", bounds=(0.0, None)
+    )
+    l_rate_scheduler: LRSchedulerType = param.ClassSelector(
+        default=LRSchedulerType.Polynomial,
+        class_=LRSchedulerType,
+        instantiate=False,
+        doc="Learning rate decay method (Cosine, Polynomial, Step, MultiStep or Exponential)",
+    )
+    l_rate_exponential_gamma: float = param.Number(
+        0.9, doc="Controls the rate of decay for the Exponential LR scheduler."
+    )
+    l_rate_step_gamma: float = param.Number(0.1, doc="Controls the rate of decay for the Step LR scheduler.")
+    l_rate_step_step_size: int = param.Integer(50, bounds=(0, None), doc="The step size for Step LR scheduler")
+    l_rate_multi_step_gamma: float = param.Number(0.1, doc="Controls the rate of decay for the MultiStep LR scheduler.")
+    l_rate_multi_step_milestones: Optional[List[int]] = param.List(
+        None, bounds=(1, None), allow_None=True, class_=int, doc="The milestones for MultiStep decay."
+    )
+    l_rate_polynomial_gamma: float = param.Number(
+        1e-4, doc="Controls the rate of decay for the Polynomial LR scheduler."
+    )
+    l_rate_warmup: LRWarmUpType = param.ClassSelector(
+        default=LRWarmUpType.NoWarmUp,
+        class_=LRWarmUpType,
+        instantiate=False,
+        doc="The type of learning rate warm up to use. Can be NoWarmUp (default) or Linear.",
+    )
+    l_rate_warmup_epochs: int = param.Integer(
+        0,
+        bounds=(0, None),
+        doc="Number of warmup epochs (linear warmup) before the "
+        "scheduler starts decaying the learning rate. "
+        "For example, if you are using MultiStepLR with "
+        "milestones [50, 100, 200] and warmup epochs = 100, warmup "
+        "will last for 100 epochs and the first decay of LR "
+        "will happen on epoch 150",
+    )
+    optimizer_type: OptimizerType = param.ClassSelector(
+        default=OptimizerType.Adam, class_=OptimizerType, instantiate=False, doc="The optimizer_type to use"
+    )
     opt_eps: float = param.Number(1e-4, doc="The epsilon parameter of RMSprop or Adam")
     rms_alpha: float = param.Number(0.9, doc="The alpha parameter of RMSprop")
-    adam_betas: TupleFloat2 = param.NumericTuple((0.9, 0.999), length=2,
-                                                 doc="The betas parameter of Adam, default is (0.9, 0.999)")
+    adam_betas: TupleFloat2 = param.NumericTuple(
+        (0.9, 0.999), length=2, doc="The betas parameter of Adam, default is (0.9, 0.999)"
+    )
     momentum: float = param.Number(0.6, doc="The momentum parameter of the optimizers")
     weight_decay: float = param.Number(1e-4, doc="The weight decay used to control L2 regularization")
 
     def validate(self) -> None:
         if len(self.adam_betas) < 2:
             raise ValueError(
                 "The adam_betas parameter should be the coefficients used for computing running averages of "
-                "gradient and its square")
+                "gradient and its square"
+            )
 
         if self.l_rate_scheduler == LRSchedulerType.MultiStep:
             if not self.l_rate_multi_step_milestones:
                 raise ValueError("Must specify l_rate_multi_step_milestones to use LR scheduler MultiStep")
             if sorted(set(self.l_rate_multi_step_milestones)) != self.l_rate_multi_step_milestones:
                 raise ValueError("l_rate_multi_step_milestones must be a strictly increasing list")
             if self.l_rate_multi_step_milestones[0] <= 0:
@@ -473,104 +517,176 @@
         if value > self.l_rate:
             raise ValueError("l_rate must be >= min_l_rate, found: {}, {}".format(self.l_rate, value))
         self._min_l_rate = value
 
 
 class TrainerParams(param.Parameterized):
     max_epochs: int = param.Integer(100, bounds=(1, None), doc="Number of epochs to train.")
-    autosave_every_n_val_epochs: int = param.Integer(1, bounds=(0, None),
-                                                     doc="Save epoch checkpoints every N validation epochs. "
-                                                         "If pl_check_val_every_n_epoch > 1, this means that "
-                                                         "checkpoints are saved every "
-                                                         "N * pl_check_val_every_n_epoch training epochs.")
-    detect_anomaly: bool = param.Boolean(False,
-                                         doc="If true, test gradients for anomalies (NaN or Inf) during training.")
-    use_mixed_precision: bool = \
-        param.Boolean(True,
-                      doc="If True, use float16 precision (Native Adaptive Mixed Precision) during training. "
-                          "If False, use float32.")
-    max_num_gpus: int = param.Integer(default=-1,
-                                      doc="The maximum number of GPUS to use. If set to a value < 0, use"
-                                          "all available GPUs. In distributed training, this is the "
-                                          "maximum number of GPUs per node.")
-    pl_progress_bar_refresh_rate: Optional[int] = \
-        param.Integer(default=None,
-                      doc="PyTorch Lightning trainer flag 'progress_bar_refresh_rate': How often to refresh "
-                          "progress bar (in steps). Value 0 disables progress bar. If None choose, automatically.")
-    pl_num_sanity_val_steps: int = \
-        param.Integer(default=0,
-                      doc="PyTorch Lightning trainer flag 'num_sanity_val_steps': Number of validation "
-                          "steps to run before training, to identify possible problems")
-    pl_deterministic: bool = \
-        param.Boolean(default=False,
-                      doc="Controls the PyTorch Lightning trainer flags 'deterministic' and 'benchmark'. If "
-                          "'pl_deterministic' is True, results are perfectly reproducible. If False, they are not, "
-                          "but you may see training speed increases.")
-    pl_find_unused_parameters: bool = \
-        param.Boolean(default=False,
-                      doc="Controls the PyTorch Lightning flag 'find_unused_parameters' for the DDP plugin. "
-                          "Setting it to True comes with a performance hit.")
-    pl_limit_train_batches: Optional[IntOrFloat] = \
-        param.Number(default=None,
-                     doc="PyTorch Lightning trainer flag 'limit_train_batches': Limit the training dataset to the "
-                         "given number of batches if integer, or proportion of training dataset if float.")
-    pl_limit_val_batches: Optional[IntOrFloat] = \
-        param.Number(default=None,
-                     doc="PyTorch Lightning trainer flag 'limit_val_batches': Limit the validation dataset to the "
-                         "given number of batches if integer, or proportion of validation dataset if float.")
-    pl_limit_test_batches: Optional[IntOrFloat] = \
-        param.Number(default=None,
-                     doc="PyTorch Lightning trainer flag 'limit_test_batches': Limit the test dataset to the "
-                         "given number of batches if integer, or proportion of test dataset if float.")
-    pl_fast_dev_run: Optional[int] = \
-        param.Integer(default=0,
-                      doc="PyTorch Lightning trainer flag 'fast_dev_run': Runs n if set to 'n' batch(es) of train, val"
-                          "and test. Default to 0 to use all train, val and test batches available. Setting "
-                          "pl_fast_dev_run to n > 0 overrides pl_limit_{train, val, test}_batches to the same value n."
-                          "Additionally, by setting this argument, ALL (tuner, checkpoint callbacks, early stopping "
-                          "callbacks, loggers and loggger callbacks) will be disabled and run for only a single epoch."
-                          "This must be used only for debbuging purposes.")
-    pl_profiler: Optional[str] = \
-        param.String(default=None,
-                     doc="The value to use for the 'profiler' argument for the Lightning trainer. "
-                         "Set to either 'simple', 'advanced', or 'pytorch'")
-    monitor_gpu: bool = param.Boolean(default=False,
-                                      doc="If True, add the GPUStatsMonitor callback to the Lightning trainer object. "
-                                          "This will write GPU utilization metrics every 50 batches by default.")
-    monitor_loading: bool = param.Boolean(default=False,
-                                          doc="If True, add the BatchTimeCallback callback to the Lightning trainer "
-                                              "object. This will monitor how long individual batches take to load.")
-    run_extra_val_epoch: bool = param.Boolean(default=False,
-                                              doc="If True, run an additional validation epoch at the end of training "
-                                              "to produce plots outputs on the validation set. This is to reduce "
-                                              "any validation overheads during training time and produce "
-                                              "additional time or memory consuming outputs only once after "
-                                              "training is finished on the validation set.")
+    autosave_every_n_val_epochs: int = param.Integer(
+        1,
+        bounds=(0, None),
+        doc="Save epoch checkpoints every N validation epochs. "
+        "If pl_check_val_every_n_epoch > 1, this means that "
+        "checkpoints are saved every "
+        "N * pl_check_val_every_n_epoch training epochs.",
+    )
+    detect_anomaly: bool = param.Boolean(
+        False, doc="If true, test gradients for anomalies (NaN or Inf) during training."
+    )
+    use_mixed_precision: bool = param.Boolean(
+        True,
+        doc="If True, use float16 precision (Native Adaptive Mixed Precision) during training. "
+        "If False, use float32.",
+    )
+    max_num_gpus: int = param.Integer(
+        default=-1,
+        doc="The maximum number of GPUS to use. If set to a value < 0, use"
+        "all available GPUs. In distributed training, this is the "
+        "maximum number of GPUs per node.",
+    )
+    max_num_gpus_inference: int = param.Integer(
+        default=1,
+        doc="The maximum number of GPUS to use for inference. Default is 1 for "
+        "single device inference. This guarantees reproducibility of "
+        "results without any duplication of data. However, if you use "
+        "pl_replace_sampler_ddp=False, you can set this to a higher value "
+        "to speed up inference. Use a negative value to use all available "
+        "GPUs in the system.",
+    )
+    pl_progress_bar_refresh_rate: Optional[int] = param.Integer(
+        default=None,
+        doc="PyTorch Lightning trainer flag 'progress_bar_refresh_rate': How often to refresh "
+        "progress bar (in steps). Value 0 disables progress bar. If None choose, automatically.",
+    )
+    pl_num_sanity_val_steps: int = param.Integer(
+        default=0,
+        doc="PyTorch Lightning trainer flag 'num_sanity_val_steps': Number of validation "
+        "steps to run before training, to identify possible problems",
+    )
+    pl_deterministic: bool = param.Boolean(
+        default=False,
+        doc="Controls the PyTorch Lightning trainer flags 'deterministic' and 'benchmark'. If "
+        "'pl_deterministic' is True, results are perfectly reproducible. If False, they are not, "
+        "but you may see training speed increases.",
+    )
+    pl_find_unused_parameters: bool = param.Boolean(
+        default=False,
+        doc="Controls the PyTorch Lightning flag 'find_unused_parameters' for the DDP plugin. "
+        "Setting it to True comes with a performance hit.",
+    )
+    pl_limit_train_batches: Optional[IntOrFloat] = param.Number(
+        default=None,
+        doc="PyTorch Lightning trainer flag 'limit_train_batches': Limit the training dataset to the "
+        "given number of batches if integer, or proportion of training dataset if float.",
+    )
+    pl_limit_val_batches: Optional[IntOrFloat] = param.Number(
+        default=None,
+        doc="PyTorch Lightning trainer flag 'limit_val_batches': Limit the validation dataset to the "
+        "given number of batches if integer, or proportion of validation dataset if float.",
+    )
+    pl_limit_test_batches: Optional[IntOrFloat] = param.Number(
+        default=None,
+        doc="PyTorch Lightning trainer flag 'limit_test_batches': Limit the test dataset to the "
+        "given number of batches if integer, or proportion of test dataset if float.",
+    )
+    pl_fast_dev_run: Optional[int] = param.Integer(
+        default=0,
+        doc="PyTorch Lightning trainer flag 'fast_dev_run': Runs n if set to 'n' batch(es) of train, val"
+        "and test. Default to 0 to use all train, val and test batches available. Setting "
+        "pl_fast_dev_run to n > 0 overrides pl_limit_{train, val, test}_batches to the same value n."
+        "Additionally, by setting this argument, ALL (tuner, checkpoint callbacks, early stopping "
+        "callbacks, loggers and loggger callbacks) will be disabled and run for only a single epoch."
+        "This must be used only for debbuging purposes.",
+    )
+    pl_profiler: Optional[str] = param.String(
+        default=None,
+        doc="The value to use for the 'profiler' argument for the Lightning trainer. "
+        "Set to either 'simple', 'advanced', or 'pytorch'",
+    )
+    pl_sync_batchnorm: bool = param.Boolean(
+        default=True,
+        doc="PyTorch Lightning trainer flag 'sync_batchnorm': If True, "
+        "synchronize batchnorm across all GPUs when running in ddp mode."
+        "If False, batchnorm is not synchronized.",
+    )
+    pl_static_graph: bool = param.Boolean(
+        default=False, doc="PyTorch DDP flag 'static_graph': If True, the trained graph is static. Default is False."
+    )
+    monitor_gpu: bool = param.Boolean(
+        default=False,
+        doc="If True, add the GPUStatsMonitor callback to the Lightning trainer object. "
+        "This will write GPU utilization metrics every 50 batches by default.",
+    )
+    monitor_loading: bool = param.Boolean(
+        default=False,
+        doc="If True, add the BatchTimeCallback callback to the Lightning trainer "
+        "object. This will monitor how long individual batches take to load.",
+    )
+    monitor_training: bool = param.Boolean(
+        default=False,
+        doc="If True, add the TrainingDiagnosisCallback to the Lightning trainer "
+        "object. This will monitor when training, validation and test starts "
+        "and ends and also intermediate steps.",
+    )
+    run_extra_val_epoch: bool = param.Boolean(
+        default=False,
+        doc="If True, run an additional validation epoch at the end of training "
+        "to produce plots outputs on the validation set. This is to reduce "
+        "any validation overheads during training time and produce "
+        "additional time or memory consuming outputs only once after "
+        "training is finished on the validation set.",
+    )
+    pl_accumulate_grad_batches: int = param.Integer(
+        default=1,
+        doc="The number of batches over which gradients are accumulated, before a parameter update is done.",
+    )
+    pl_log_every_n_steps: int = param.Integer(
+        default=50,
+        doc="PyTorch Lightning trainer flag 'log_every_n_steps': How often to log within steps. Default to 50.",
+    )
+    pl_replace_sampler_ddp: bool = param.Boolean(
+        default=True,
+        doc="PyTorch Lightning trainer flag 'replace_sampler_ddp' that "
+        "sets the sampler for distributed training with shuffle=True during "
+        "training and shuffle=False during validation. Default to True. Set to"
+        "False to set your own sampler.",
+    )
+
+    def validate(self) -> None:
+        if self.max_num_gpus_inference > 1 and self.pl_replace_sampler_ddp:
+            logging.warning(
+                "The 'pl_replace_sampler_ddp' flag is set to True, but the 'max_num_gpus_inference' > 1. "
+                "This might bias the inference results due to duplicate samples. Consider setting "
+                "--pl_replace_sampler_ddp=False if you want to use multiple GPUs for inference."
+                "pytorch_lightning.overrides.distributed.UnrepeatedDistributedSampler can be used instead "
+                "of DistributedSampler."
+            )
 
     @property
     def use_gpu(self) -> bool:
         """
         Returns True if a GPU is available, and the self.max_num_gpus flag allows it to be used. Returns False
         otherwise (i.e., if there is no GPU available, or self.max_num_gpus==0)
         """
         if self.max_num_gpus == 0:
             return False
         from health_ml.utils.common_utils import is_gpu_available
+
         return is_gpu_available()
 
     def num_gpus_per_node(self) -> int:
         """
         Computes the number of gpus to use for each node: either the number of gpus available on the device
         or restrict it to max_num_gpu, whichever is smaller. Returns 0 if running on a CPU device.
         """
         import torch
+
         available_gpus = torch.cuda.device_count()  # type: ignore
         num_gpus = available_gpus if self.use_gpu else 0
         message_suffix = "" if self.use_gpu else ", but not using them because use_gpu == False"
         logging.info(f"Number of available GPUs: {available_gpus}{message_suffix}")
         if 0 <= self.max_num_gpus < num_gpus:
             num_gpus = self.max_num_gpus
             logging.info(f"Restricting the number of GPUs to {num_gpus}")
         elif self.max_num_gpus > num_gpus:
-            logging.warning(
-                f"You requested max_num_gpus {self.max_num_gpus} but there are only {num_gpus} available.")
+            logging.warning(f"You requested max_num_gpus {self.max_num_gpus} but there are only {num_gpus} available.")
         return num_gpus
```

### Comparing `hi-ml-0.2.9/src/health_ml/lightning_container.py` & `hi-ml-0.3.0/src/health_ml/lightning_container.py`

 * *Files 14% similar despite different names*

```diff
@@ -2,49 +2,47 @@
 #  Copyright (c) Microsoft Corporation. All rights reserved.
 #  Licensed under the MIT License (MIT). See LICENSE in the repo root for license information.
 #  ------------------------------------------------------------------------------------------
 from typing import Any, Dict, List, Optional, Tuple
 from pathlib import Path
 
 import param
+import logging
 from azureml.core import ScriptRunConfig
 from azureml.train.hyperdrive import HyperDriveConfig
 from pytorch_lightning import Callback, LightningDataModule, LightningModule
 from torch.optim import Optimizer
 from torch.optim.lr_scheduler import _LRScheduler
 
 from health_azure.utils import create_from_matching_params
-from health_ml.deep_learning_config import DatasetParams, OptimizerParams, OutputParams, TrainerParams, \
-    WorkflowParams
+from health_ml.deep_learning_config import DatasetParams, OptimizerParams, OutputParams, TrainerParams, WorkflowParams
 from health_ml.experiment_config import ExperimentConfig
 from health_ml.utils.checkpoint_utils import get_best_checkpoint_path
 from health_ml.utils.lr_scheduler import SchedulerWithWarmUp
 from health_ml.utils.model_util import create_optimizer
 
 
-class LightningContainer(WorkflowParams,
-                         DatasetParams,
-                         OutputParams,
-                         TrainerParams,
-                         OptimizerParams):
+class LightningContainer(WorkflowParams, DatasetParams, OutputParams, TrainerParams, OptimizerParams):
     """
     A LightningContainer contains all information to train a user-specified PyTorch Lightning model. The model that
     should be trained is returned by the `get_model` method. The training data must be returned in the form of
     a LightningDataModule, by the `get_data_module` method.
     """
 
     def __init__(self, **kwargs: Any) -> None:
         super().__init__(**kwargs)
         self._model: Optional[LightningModule] = None
         self._model_name = type(self).__name__
         self.num_nodes = 1
+        self.trained_weights_path: Optional[Path] = None
 
     def validate(self) -> None:
         WorkflowParams.validate(self)
         OptimizerParams.validate(self)
+        TrainerParams.validate(self)
 
     def setup(self) -> None:
         """
         This method is called as one of the first operations of the training/testing workflow, before any other
         operations on the present object. At the point when called, the datasets are already available in
         the locations given by self.local_datasets. Use this method to prepare datasets or data loaders, for example.
         """
@@ -63,14 +61,25 @@
         This should read datasets from the self.local_datasets folder or download from a web location.
         The format of the data is not specified any further.
 
         :return: A LightningDataModule
         """
         return None  # type: ignore
 
+    def get_eval_data_module(self) -> LightningDataModule:
+        """
+        Gets the data that is used when evaluating the model on a new dataset.
+        This data module should read datasets from the self.local_datasets folder or download from a web location.
+        Only the test dataloader is used, hence the method needs to put all data into the test dataloader, rather
+        than splitting into train/val/test.
+
+        :return: A LightningDataModule
+        """
+        return None  # type: ignore
+
     def get_trainer_arguments(self) -> Dict[str, Any]:
         """
         Gets additional parameters that will be passed on to the PyTorch Lightning trainer.
         """
         return dict()
 
     def get_callbacks(self) -> List[Callback]:
@@ -87,24 +96,28 @@
 
         The HyperDriveConfig config object needs to specify which parameters should be searched over, and which
         metric should be monitored.
 
         :param run_config: The ScriptRunConfig object that needs to be passed into the constructor of
             HyperDriveConfig.
         """
-        raise NotImplementedError("Parameter search is not implemented. Please override 'get_parameter_tuning_config' "
-                                  "in your model container.")
+        raise NotImplementedError(
+            "Parameter search is not implemented. Please override 'get_parameter_tuning_config' "
+            "in your model container."
+        )
 
     def get_parameter_tuning_args(self) -> Dict[str, Any]:
         """
         Returns a dictionary of hyperperameter argument names and values as expected by a AML SDK v2 job
         to perform hyperparameter search
         """
-        raise NotImplementedError("Parameter search is not implemented. Please override 'get_parameter_tuning_args' "
-                                  "in your model container.")
+        raise NotImplementedError(
+            "Parameter search is not implemented. Please override 'get_parameter_tuning_args' "
+            "in your model container."
+        )
 
     def update_experiment_config(self, experiment_config: ExperimentConfig) -> None:
         """
         This method allows overriding ExperimentConfig parameters from within a LightningContainer.
         It is called right after the ExperimentConfig and container are initialised.
         Be careful when using class parameters to override these values. If the parameter names clash,
         CLI values will be consumed by the ExperimentConfig, but container parameters will keep their defaults.
@@ -181,30 +194,30 @@
         Returns the HyperDrive config for either hyperparameter tuning, cross validation, or running with
         different seeds.
 
         :return: A configuration object for HyperDrive
         """
         if self.hyperdrive:
             return self.get_parameter_tuning_config(ScriptRunConfig(source_directory=""))
-        if self.is_crossvalidation_enabled:
+        if self.is_crossvalidation_parent_run:
             return self.get_crossval_hyperdrive_config()
         if self.different_seeds > 0:
             return self.get_different_seeds_hyperdrive_config()
         return None
 
     def get_hyperparam_args(self) -> Optional[Dict[str, Any]]:
         """
         Returns a dictionary of hyperparameter search arguments that will be passed to an AML v2 command to
         enable either hyperparameter tuning,  cross validation, or running with different seeds.
 
         :return: A dictionary of hyperparameter search arguments and values.
         """
         if self.hyperdrive:
             return self.get_parameter_tuning_args()
-        if self.is_crossvalidation_enabled:
+        if self.is_crossvalidation_parent_run:
             return self.get_crossval_hyperparam_args_v2()
         if self.different_seeds > 0:
             return self.get_grid_hyperparam_args_v2()
         return None
 
     def load_model_checkpoint(self, checkpoint_path: Path) -> None:
         """
@@ -216,16 +229,17 @@
         self._model = type(self._model).load_from_checkpoint(checkpoint_path=str(checkpoint_path))
 
     def __str__(self) -> str:
         """Returns a string describing the present object, as a list of key: value strings."""
         arguments_str = "\nContainer:\n"
         # Avoid callable params, the bindings that are printed out can be humongous.
         # Avoid dataframes
-        skip_params = {name for name, value in self.param.params().items()
-                       if isinstance(value, (param.Callable, param.DataFrame))}
+        skip_params = {
+            name for name, value in self.param.params().items() if isinstance(value, (param.Callable, param.DataFrame))
+        }
         for key, value in self.param.get_param_values():
             if key not in skip_params:
                 arguments_str += f"\t{key:40}: {value}\n"
         # Print out all other separate vars that are not under the guidance of the params library,
         # skipping the two that are introduced by params
         skip_vars = {"param", "initialized"}
         for key, value in vars(self).items():
@@ -242,32 +256,62 @@
 
     @property
     def effective_experiment_name(self) -> str:
         """Returns the name of the AzureML experiment that should be used. This is taken from the commandline
         argument `experiment`, falling back to the model class name if not set."""
         return self.experiment or self.model_name
 
+    def get_additional_aml_run_tags(self) -> Dict[str, str]:
+        """Returns a dictionary of tags that should be added to the AzureML run."""
+        return {}
+
+    def get_additional_environment_variables(self) -> Dict[str, str]:
+        """Returns a dictionary of environment variables that should be added to the AzureML run."""
+        return {}
+
+    def on_run_extra_validation_epoch(self) -> None:
+        if hasattr(self.model, "on_run_extra_validation_epoch"):
+            assert self._model, "Model is not initialized."
+            self.model.on_run_extra_validation_epoch()  # type: ignore
+        else:
+            logging.warning(
+                "Hook `on_run_extra_validation_epoch` is not implemented by lightning module."
+                "The extra validation epoch won't produce any extra outputs."
+            )
+
+    def set_model_variant(self, variant_name: str) -> None:
+        """Choose which variant of the model to use. A variant can for example have a different number of layers
+        compared to the base model. This method is called by the runner to set the variant that should be used, passing
+        in the variant name. A typical implement would set parameters of the object, based on the value of the
+        `variant_name` argument.
+
+        :param variant_name: The name of the model variant that should be set.
+        """
+        pass
+
 
 class LightningModuleWithOptimizer(LightningModule):
     """
     A base class that supplies a method to configure optimizers and LR schedulers. To use this in your model,
     inherit from this class instead of from LightningModule.
     If this class is used, all configuration options for the optimizers and LR schedulers will be also available as
-    commandline arguments (for example, you can supply the InnerEye runner with "--l_rate=1e-2" to change the learning
+    commandline arguments (for example, you can supply the hi-ml runner with "--l_rate=1e-2" to change the learning
     rate.
     """
+
     # These fields will be set by the LightningContainer when the model is created.
     _optimizer_params = OptimizerParams()
     _trainer_params = TrainerParams()
 
     def configure_optimizers(self) -> Tuple[List[Optimizer], List[_LRScheduler]]:
         """
         This is the default implementation of the method that provides the optimizer and LR scheduler for
         PyTorch Lightning. It reads out the optimizer and scheduler settings from the model fields,
         and creates the two objects.
         Override this method for full flexibility to define any optimizer and scheduler.
         :return: A tuple of (optimizer, LR scheduler)
         """
         optimizer = create_optimizer(self._optimizer_params, self.parameters())
-        l_rate_scheduler = SchedulerWithWarmUp(self._optimizer_params, optimizer,
-                                               num_epochs=self._trainer_params.max_epochs)
+        l_rate_scheduler = SchedulerWithWarmUp(
+            self._optimizer_params, optimizer, num_epochs=self._trainer_params.max_epochs
+        )
         return [optimizer], [l_rate_scheduler]
```

### Comparing `hi-ml-0.2.9/src/health_ml/model_trainer.py` & `hi-ml-0.3.0/src/health_ml/model_trainer.py`

 * *Files 6% similar despite different names*

```diff
@@ -15,14 +15,15 @@
 from pytorch_lightning.profiler import BaseProfiler, SimpleProfiler, AdvancedProfiler, PyTorchProfiler
 
 from health_azure.utils import RUN_CONTEXT, is_running_in_azure_ml
 
 from health_ml.lightning_container import LightningContainer
 from health_ml.utils import AzureMLProgressBar
 from health_ml.utils.common_utils import AUTOSAVE_CHECKPOINT_FILE_NAME, EXPERIMENT_SUMMARY_FILE
+from health_ml.utils.diagnostics import TrainingDiagnoticsCallback
 from health_ml.utils.lightning_loggers import StoringLogger, HimlMLFlowLogger
 
 
 T = TypeVar('T')
 
 
 def write_experiment_summary_file(config: Any, outputs_folder: Path) -> None:
@@ -36,33 +37,36 @@
     logging.info(output)
 
 
 def get_pl_profiler(pl_profiler: Optional[str], outputs_folder: Path) -> Optional[BaseProfiler]:
     if pl_profiler:
         pl_profilers = {"simple": SimpleProfiler, "advanced": AdvancedProfiler, "pytorch": PyTorchProfiler}
         if pl_profiler not in pl_profilers:
-            raise ValueError("Unsupported profiler. Please choose one of the following options: simple, advanced, "
-                             "pytorch. You can refer to https://pytorch-lightning.readthedocs.io/en/stable/advanced/"
-                             "profiler.html to learn more about each profiler. You can specify a custom profiler by "
-                             "overriding the default behavior of get_trainer_arguments() in your lightning container. "
-                             "You can find an example here https://github.com/microsoft/hi-ml/tree/main/docs/source/"
-                             "debugging.md#L145")
+            raise ValueError(
+                "Unsupported profiler. Please choose one of the following options: simple, advanced, "
+                "pytorch. You can refer to https://pytorch-lightning.readthedocs.io/en/stable/advanced/"
+                "profiler.html to learn more about each profiler. You can specify a custom profiler by "
+                "overriding the default behavior of get_trainer_arguments() in your lightning container. "
+                "You can find an example here https://github.com/microsoft/hi-ml/tree/main/docs/source/"
+                "debugging.md#L145"
+            )
         profiler = pl_profilers[pl_profiler](dirpath=outputs_folder / "profiler")
         return profiler
     else:
         return None
 
 
-def create_lightning_trainer(container: LightningContainer,
-                             resume_from_checkpoint: Optional[Path] = None,
-                             num_nodes: int = 1,
-                             multiple_trainloader_mode: str = "max_size_cycle",
-                             azureml_run_for_logging: Optional[Run] = None,
-                             mlflow_run_for_logging: Optional[str] = None) -> \
-        Tuple[Trainer, StoringLogger]:
+def create_lightning_trainer(
+    container: LightningContainer,
+    resume_from_checkpoint: Optional[Path] = None,
+    num_nodes: int = 1,
+    multiple_trainloader_mode: str = "max_size_cycle",
+    azureml_run_for_logging: Optional[Run] = None,
+    mlflow_run_for_logging: Optional[str] = None,
+) -> Tuple[Trainer, StoringLogger]:
     """
     Creates a Pytorch Lightning Trainer object for the given model configuration. It creates checkpoint handlers
     and loggers. That includes a diagnostic logger for use in unit tests, that is also returned as the second
     return value.
 
     :param container: The container with model and data.
     :param resume_from_checkpoint: If provided, training resumes from this checkpoint point.
@@ -85,36 +89,39 @@
         devices = num_gpus
         message = f"{devices} GPU"
         if effective_num_gpus > 1:
             # Accelerator should be "ddp" when running large models in AzureML (when using DDP_spawn, we get out of
             # GPU memory).
             # Initialize the DDP plugin. The default for pl_find_unused_parameters is False. If True, the plugin
             # prints out lengthy warnings about the performance impact of find_unused_parameters.
-            strategy = DDPStrategy(find_unused_parameters=container.pl_find_unused_parameters)
+            strategy = DDPStrategy(
+                find_unused_parameters=container.pl_find_unused_parameters,
+                static_graph=container.pl_static_graph,
+            )
             message += "s per node with DDP"
     logging.info(f"Using {message}")
     tensorboard_logger = TensorBoardLogger(save_dir=str(container.logs_folder), name="Lightning", version="")
     loggers: List[Any] = [tensorboard_logger]
 
     if is_running_in_azure_ml():
         mlflow_run_id = os.environ.get("MLFLOW_RUN_ID", None)
         logging.info(f"Logging to MLFlow run with id: {mlflow_run_id}")
-        mlflow_logger = HimlMLFlowLogger(
-            run_id=mlflow_run_id
-        )
+        mlflow_logger = HimlMLFlowLogger(run_id=mlflow_run_id)
         loggers.append(mlflow_logger)
     else:
         mlflow_run_dir = container.outputs_folder / "mlruns"
         try:
             mlflow_run_dir.mkdir(exist_ok=True)
             mlflow_tracking_uri = "file:" + str(mlflow_run_dir)
             mlflow_logger = HimlMLFlowLogger(run_id=mlflow_run_for_logging, tracking_uri=mlflow_tracking_uri)
             loggers.append(mlflow_logger)
-            logging.info(f"Logging to MLFlow run with id: {mlflow_run_for_logging}. Local MLFlow logs are stored in "
-                         f"{mlflow_tracking_uri}")
+            logging.info(
+                f"Logging to MLFlow run with id: {mlflow_run_for_logging}. Local MLFlow logs are stored in "
+                f"{mlflow_tracking_uri}"
+            )
         except FileNotFoundError as e:
             logging.warning(f"Unable to initialise MLFlowLogger due to error: {e}")
 
     storing_logger = StoringLogger()
     loggers.append(storing_logger)
     # Use 32bit precision when running on CPU. Otherwise, make it depend on use_mixed_precision flag.
     precision = 32 if num_gpus == 0 else 16 if container.use_mixed_precision else 32
@@ -131,29 +138,31 @@
     # The last checkpoint is considered the "best" checkpoint. For large segmentation
     # models, this still appears to be the best way of choosing them because validation loss on the relatively small
     # training patches is not stable enough. Going by the validation loss somehow works for the Prostate model, but
     # not for the HeadAndNeck model.
     # Note that "last" is somehow a misnomer, it should rather be "latest". There is a "last" checkpoint written in
     # every epoch. We could use that for recovery too, but it could happen that the job gets preempted right during
     # writing that file, and we would end up with an invalid file.
-    last_checkpoint_callback = ModelCheckpoint(dirpath=str(container.checkpoint_folder),
-                                               save_last=True,
-                                               save_top_k=0)
-    recovery_checkpoint_callback = ModelCheckpoint(dirpath=str(container.checkpoint_folder),
-                                                   filename=AUTOSAVE_CHECKPOINT_FILE_NAME,
-                                                   every_n_epochs=container.autosave_every_n_val_epochs,
-                                                   save_last=False)
+    last_checkpoint_callback = ModelCheckpoint(dirpath=str(container.checkpoint_folder), save_last=True, save_top_k=0)
+    recovery_checkpoint_callback = ModelCheckpoint(
+        dirpath=str(container.checkpoint_folder),
+        filename=AUTOSAVE_CHECKPOINT_FILE_NAME,
+        every_n_epochs=container.autosave_every_n_val_epochs,
+        save_last=False,
+    )
     callbacks: List[Callback] = [
         last_checkpoint_callback,
         recovery_checkpoint_callback,
     ]
     if container.monitor_loading:
         # TODO antonsc: Remove after fixing the callback.
         raise NotImplementedError("Monitoring batch loading times has been temporarily disabled.")
         # callbacks.append(BatchTimeCallback())
+    if container.monitor_training:
+        callbacks.append(TrainingDiagnoticsCallback())
     if num_gpus > 0 and container.monitor_gpu:
         logging.info("Adding monitoring for GPU utilization")
         callbacks.append(GPUStatsMonitor(intra_step_time=True, inter_step_time=True))
     # Add the additional callbacks that were specified in get_trainer_arguments for LightningContainers
     additional_args = container.get_trainer_arguments()
     # Callbacks can be specified via the "callbacks" argument (the legacy behaviour) or the new get_callbacks method
     if "callbacks" in additional_args:
@@ -167,46 +176,56 @@
     custom_profiler = additional_args.pop("profiler", None)
     profiler = get_pl_profiler(container.pl_profiler, container.outputs_folder)
     profiler = profiler if profiler else custom_profiler
     is_azureml_run = is_running_in_azure_ml(RUN_CONTEXT)
     progress_bar_refresh_rate = container.pl_progress_bar_refresh_rate
     if progress_bar_refresh_rate is None:
         progress_bar_refresh_rate = 50
-        logging.info(f"The progress bar refresh rate is not set. Using a default of {progress_bar_refresh_rate}. "
-                     f"To change, modify the pl_progress_bar_refresh_rate field of the container.")
+        logging.info(
+            f"The progress bar refresh rate is not set. Using a default of {progress_bar_refresh_rate}. "
+            f"To change, modify the pl_progress_bar_refresh_rate field of the container."
+        )
     if is_azureml_run:
-        callbacks.append(AzureMLProgressBar(refresh_rate=progress_bar_refresh_rate,
-                                            write_to_logging_info=True,
-                                            print_timestamp=False))
+        callbacks.append(
+            AzureMLProgressBar(
+                refresh_rate=progress_bar_refresh_rate, write_to_logging_info=True, print_timestamp=False
+            )
+        )
     else:
         # Use a local import here to be able to support older PL versions
         from pytorch_lightning.callbacks import TQDMProgressBar
+
         callbacks.append(TQDMProgressBar(refresh_rate=progress_bar_refresh_rate))
     # Read out additional model-specific args here.
     # We probably want to keep essential ones like numgpu and logging.
-    trainer = Trainer(default_root_dir=str(container.outputs_folder),
-                      deterministic=deterministic,
-                      benchmark=benchmark,
-                      accelerator=accelerator,
-                      strategy=strategy,
-                      max_epochs=container.max_epochs,
-                      # All of the following limit_batches  arguments can be integers or floats.
-                      # If integers, it is the number of batches.
-                      # If float, it's the fraction of batches. We default to 1.0 (processing all batches).
-                      limit_train_batches=container.pl_limit_train_batches or 1.0,
-                      limit_val_batches=container.pl_limit_val_batches or 1.0,
-                      limit_test_batches=container.pl_limit_test_batches or 1.0,
-                      fast_dev_run=container.pl_fast_dev_run,  # type: ignore
-                      num_sanity_val_steps=container.pl_num_sanity_val_steps,
-                      # check_val_every_n_epoch=container.pl_check_val_every_n_epoch,
-                      callbacks=callbacks,
-                      logger=loggers,
-                      num_nodes=num_nodes,
-                      devices=devices,
-                      precision=precision,
-                      sync_batchnorm=True,
-                      detect_anomaly=container.detect_anomaly,
-                      profiler=profiler,
-                      resume_from_checkpoint=str(resume_from_checkpoint) if resume_from_checkpoint else None,
-                      multiple_trainloader_mode=multiple_trainloader_mode,
-                      **additional_args)
+    trainer = Trainer(
+        default_root_dir=str(container.outputs_folder),
+        deterministic=deterministic,
+        benchmark=benchmark,
+        accelerator=accelerator,
+        strategy=strategy,
+        max_epochs=container.max_epochs,
+        # All of the following limit_batches  arguments can be integers or floats.
+        # If integers, it is the number of batches.
+        # If float, it's the fraction of batches. We default to 1.0 (processing all batches).
+        limit_train_batches=container.pl_limit_train_batches or 1.0,
+        limit_val_batches=container.pl_limit_val_batches or 1.0,
+        limit_test_batches=container.pl_limit_test_batches or 1.0,
+        fast_dev_run=container.pl_fast_dev_run,  # type: ignore
+        num_sanity_val_steps=container.pl_num_sanity_val_steps,
+        log_every_n_steps=container.pl_log_every_n_steps,
+        # check_val_every_n_epoch=container.pl_check_val_every_n_epoch,
+        callbacks=callbacks,
+        logger=loggers,
+        num_nodes=num_nodes,
+        devices=devices,
+        precision=precision,
+        sync_batchnorm=container.pl_sync_batchnorm,
+        detect_anomaly=container.detect_anomaly,
+        profiler=profiler,
+        resume_from_checkpoint=str(resume_from_checkpoint) if resume_from_checkpoint else None,
+        multiple_trainloader_mode=multiple_trainloader_mode,
+        accumulate_grad_batches=container.pl_accumulate_grad_batches,
+        replace_sampler_ddp=container.pl_replace_sampler_ddp,
+        **additional_args,
+    )
     return trainer, storing_logger
```

### Comparing `hi-ml-0.2.9/src/health_ml/networks/layers/attention_layers.py` & `hi-ml-0.3.0/src/health_ml/networks/layers/attention_layers.py`

 * *Files 12% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 
 
 class MeanPoolingLayer(nn.Module):
     """Mean pooling returns uniform weights and the average feature vector over the first axis"""
 
     def forward(self, features: Tensor) -> Tuple[Tensor, Tensor]:
         num_instances = features.shape[0]
-        attention_weights = torch.full((1, num_instances), 1. / num_instances)
+        attention_weights = torch.full((1, num_instances), 1.0 / num_instances)
         pooled_features = features.mean(dim=0)
         pooled_features = pooled_features.view(1, -1)
         return (attention_weights, pooled_features)
 
 
 class MaxPoolingLayer(nn.Module):
     """Max pooling returns uniform weights and the maximum feature vector over the first axis"""
@@ -34,74 +34,62 @@
         frequency_norm = frequency / sum(frequency)
         attention_weights = frequency_norm.view(1, num_instances)
         pooled_features = pooled_features.view(1, -1)
         return (attention_weights, pooled_features)
 
 
 class AttentionLayer(nn.Module):
-    """ AttentionLayer: Simple attention layer
+    """AttentionLayer: Simple attention layer
     Requires size of input L, hidden D, and attention layers K (default K=1)
     """
 
-    def __init__(self, input_dims: int,
-                 hidden_dims: int,
-                 attention_dims: int = 1) -> None:
+    def __init__(self, input_dims: int, hidden_dims: int, attention_dims: int = 1) -> None:
         super().__init__()
 
         # Attention layers
-        self.input_dims = input_dims                    # L
-        self.hidden_dims = hidden_dims                  # D
-        self.attention_dims = attention_dims            # K
+        self.input_dims = input_dims  # L
+        self.hidden_dims = hidden_dims  # D
+        self.attention_dims = attention_dims  # K
         self.attention = nn.Sequential(
-            nn.Linear(self.input_dims, self.hidden_dims),
-            nn.Tanh(),
-            nn.Linear(self.hidden_dims, self.attention_dims)
+            nn.Linear(self.input_dims, self.hidden_dims), nn.Tanh(), nn.Linear(self.hidden_dims, self.attention_dims)
         )
 
     def forward(self, features: Tensor) -> Tuple[Tensor, Tensor]:
-        features = features.view(-1, self.input_dims)            # N x L
-        attention_weights = self.attention(features)             # N x K
-        attention_weights = transpose(attention_weights, 1, 0)   # K x N
+        features = features.view(-1, self.input_dims)  # N x L
+        attention_weights = self.attention(features)  # N x K
+        attention_weights = transpose(attention_weights, 1, 0)  # K x N
         attention_weights = F.softmax(attention_weights, dim=1)  # Softmax over N : K x N
-        pooled_features = mm(attention_weights, features)        # Matrix multiplication : K x L
+        pooled_features = mm(attention_weights, features)  # Matrix multiplication : K x L
         return attention_weights, pooled_features
 
 
 class GatedAttentionLayer(nn.Module):
-    """ GatedAttentionLayer: Gated attention layer
+    """GatedAttentionLayer: Gated attention layer
     Requires size of input L, hidden D, and output layers K (default K=1)
     """
 
-    def __init__(self, input_dims: int,
-                 hidden_dims: int,
-                 attention_dims: int = 1) -> None:
+    def __init__(self, input_dims: int, hidden_dims: int, attention_dims: int = 1) -> None:
         super().__init__()
 
         # Gated attention layers
-        self.input_dims = input_dims                    # L
-        self.hidden_dims = hidden_dims                  # D
-        self.attention_dims = attention_dims            # K
-        self.attention_V = nn.Sequential(
-            nn.Linear(self.input_dims, self.hidden_dims),
-            nn.Tanh()
-        )
-        self.attention_U = nn.Sequential(
-            nn.Linear(self.input_dims, self.hidden_dims),
-            nn.Sigmoid()
-        )
+        self.input_dims = input_dims  # L
+        self.hidden_dims = hidden_dims  # D
+        self.attention_dims = attention_dims  # K
+        self.attention_V = nn.Sequential(nn.Linear(self.input_dims, self.hidden_dims), nn.Tanh())
+        self.attention_U = nn.Sequential(nn.Linear(self.input_dims, self.hidden_dims), nn.Sigmoid())
         self.attention_weights = nn.Linear(self.hidden_dims, self.attention_dims)
 
     def forward(self, features: Tensor) -> Tuple[Tensor, Tensor]:
-        features = features.view(-1, self.input_dims)            # N x L
-        A_V = self.attention_V(features)                         # N x D
-        A_U = self.attention_U(features)                         # N x D
-        attention_weights = self.attention_weights(A_V * A_U)    # Element-wise multiplication : N x K
-        attention_weights = transpose(attention_weights, 1, 0)   # K x N
+        features = features.view(-1, self.input_dims)  # N x L
+        A_V = self.attention_V(features)  # N x D
+        A_U = self.attention_U(features)  # N x D
+        attention_weights = self.attention_weights(A_V * A_U)  # Element-wise multiplication : N x K
+        attention_weights = transpose(attention_weights, 1, 0)  # K x N
         attention_weights = F.softmax(attention_weights, dim=1)  # Softmax over N : K x N
-        pooled_features = mm(attention_weights, features)        # Matrix multiplication : K x L
+        pooled_features = mm(attention_weights, features)  # Matrix multiplication : K x L
         return attention_weights, pooled_features
 
 
 class CustomTransformerEncoderLayer(TransformerEncoderLayer):
     """Adaptation of the pytorch TransformerEncoderLayer that always outputs the attention weights.
 
     TransformerEncoderLayer is made up of self-attn and feedforward network.
@@ -130,19 +118,23 @@
         >>> out, attention_weights = encoder_layer(src)
 
     Alternatively, when ``batch_first`` is ``True``:
         >>> encoder_layer = nn.TransformerEncoderLayer(d_model=512, nhead=8, batch_first=True)
         >>> src = torch.rand(32, 10, 512)
         >>> out, attention_weights = encoder_layer(src)
     """
+
     # new forward returns output as well as attention weights
 
-    def forward(self, src: torch.Tensor,  # type: ignore
-                src_mask: Optional[torch.Tensor] = None,
-                src_key_padding_mask: Optional[torch.Tensor] = None) -> Tuple[torch.Tensor, torch.Tensor]:
+    def forward(
+        self,
+        src: torch.Tensor,  # type: ignore
+        src_mask: Optional[torch.Tensor] = None,
+        src_key_padding_mask: Optional[torch.Tensor] = None,
+    ) -> Tuple[torch.Tensor, torch.Tensor]:
         """Pass the input through the encoder layer.
 
         Args:
             src: the sequence to the encoder layer (required).
             src_mask: the mask for the src sequence (optional).
             src_key_padding_mask: the mask for the src keys per batch (optional).
 
@@ -161,21 +153,20 @@
             sa_block_out, a = self._sa_block(x, src_mask, src_key_padding_mask)
             x = self.norm1(x + sa_block_out)
             x = self.norm2(x + self._ff_block(x))
 
         return x, a
 
     # new self-attention block, returns output as well as attention weights
-    def _sa_block(self, x: Tensor,  # type: ignore
-                  attn_mask: Optional[Tensor],
-                  key_padding_mask: Optional[Tensor]) -> Tuple[torch.Tensor, torch.Tensor]:
-        x, a = self.self_attn(x, x, x,
-                              attn_mask=attn_mask,
-                              key_padding_mask=key_padding_mask,
-                              need_weights=True)  # Just because of this flag I had to copy all of the code...
+    def _sa_block(
+        self, x: Tensor, attn_mask: Optional[Tensor], key_padding_mask: Optional[Tensor]  # type: ignore
+    ) -> Tuple[torch.Tensor, torch.Tensor]:
+        x, a = self.self_attn(
+            x, x, x, attn_mask=attn_mask, key_padding_mask=key_padding_mask, need_weights=True
+        )  # Just because of this flag I had to copy all of the code...
         x = x[0]
         return self.dropout1(x), a
 
 
 class TransformerPooling(Module):
     """Create a Transformer encoder module consisting of multiple Transformer encoder layers.
 
@@ -183,33 +174,37 @@
     appended to the list of tiles encodings. Second, we perform self-attention between all tile encodings and the cls
     token. Last, we extract the cls token and use it for classification.
 
     Args:
         num_layers: Number of Transformer encoder layers.
         num_heads: Number of attention heads per layer.
         dim_representation: Dimension of input encoding.
+        transformer_dropout: The dropout value of transformer encoder layers.
     """
 
-    def __init__(self, num_layers: int, num_heads: int, dim_representation: int) -> None:
+    def __init__(self, num_layers: int, num_heads: int, dim_representation: int, transformer_dropout: float) -> None:
         super(TransformerPooling, self).__init__()
         self.num_layers = num_layers
         self.num_heads = num_heads
         self.dim_representation = dim_representation
-
+        self.transformer_dropout = transformer_dropout
         self.cls_token = nn.Parameter(torch.zeros([1, dim_representation]))
 
         self.transformer_encoder_layers = []
         for _ in range(self.num_layers):
             self.transformer_encoder_layers.append(
-                CustomTransformerEncoderLayer(self.dim_representation,
-                                              self.num_heads,
-                                              dim_feedforward=self.dim_representation,
-                                              dropout=0.1,
-                                              activation=F.gelu,  # type: ignore
-                                              batch_first=True))
+                CustomTransformerEncoderLayer(
+                    self.dim_representation,
+                    self.num_heads,
+                    dim_feedforward=self.dim_representation,
+                    dropout=self.transformer_dropout,
+                    activation=F.gelu,
+                    batch_first=True,
+                )
+            )
         self.transformer_encoder_layers = torch.nn.ModuleList(self.transformer_encoder_layers)  # type: ignore
 
     def forward(self, features: Tensor) -> Tuple[torch.Tensor, torch.Tensor]:
         # Append cls token
         features = torch.vstack([self.cls_token, features]).unsqueeze(0)
 
         for i in range(self.num_layers):
@@ -235,34 +230,38 @@
     The transformer pooling is used in the implementation of (Myronenko et al. 2021).
     Example in https://github.com/Project-MONAI/tutorials/blob/master/pathology/multiple_instance_learning/
     panda_mil_train_evaluate_pytorch_gpu.py.
     Args:
         num_layers: Number of Transformer encoder layers.
         num_heads: Number of attention heads per layer.
         dim_representation: Dimension of input encoding.
+        transformer_dropout: The dropout value of transformer encoder layers.
     """
 
-    def __init__(self, num_layers: int, num_heads: int, dim_representation: int, hidden_dim: int) -> None:
+    def __init__(
+        self, num_layers: int, num_heads: int, dim_representation: int, hidden_dim: int, transformer_dropout: float
+    ) -> None:
         super().__init__()
         self.num_layers = num_layers
         self.num_heads = num_heads
         self.dim_representation = dim_representation
         self.hidden_dim = hidden_dim
-        transformer_layer = nn.TransformerEncoderLayer(d_model=self.dim_representation,
-                                                       nhead=self.num_heads,
-                                                       dropout=0.0,
-                                                       batch_first=True)
+        self.transformer_dropout = transformer_dropout
+        transformer_layer = nn.TransformerEncoderLayer(
+            d_model=self.dim_representation, nhead=self.num_heads, dropout=self.transformer_dropout, batch_first=True
+        )
         self.transformer = nn.TransformerEncoder(transformer_layer, num_layers=self.num_layers)
-        self.attention = nn.Sequential(nn.Linear(self.dim_representation, self.hidden_dim),
-                                       nn.Tanh(), nn.Linear(self.hidden_dim, 1))
+        self.attention = nn.Sequential(
+            nn.Linear(self.dim_representation, self.hidden_dim), nn.Tanh(), nn.Linear(self.hidden_dim, 1)
+        )
 
     def forward(self, x: torch.Tensor) -> Tuple[torch.Tensor, torch.Tensor]:
         """
         Input size is L, bag size N, hidden dimension is D, and attention layers K (default K=1).
         """
-        x = x.reshape(-1, x.shape[0], x.shape[1])                       # 1 x N X L
-        x = self.transformer(x)                                         # 1 x N X L
-        a = self.attention(x)                                           # 1 x N X K
-        attention_weights = torch.softmax(a, dim=1)                     # 1 x N x K
-        pooled_features = torch.sum(x * attention_weights, dim=1)       # K X L
-        attention_weights = attention_weights.permute(0, 2, 1)          # 1 x K X N
-        return (attention_weights.squeeze(0), pooled_features)          # K X N, K X L
+        x = x.reshape(-1, x.shape[0], x.shape[1])  # 1 x N X L
+        x = self.transformer(x)  # 1 x N X L
+        a = self.attention(x)  # 1 x N X K
+        attention_weights = torch.softmax(a, dim=1)  # 1 x N x K
+        pooled_features = torch.sum(x * attention_weights, dim=1)  # K X L
+        attention_weights = attention_weights.permute(0, 2, 1)  # 1 x K X N
+        return (attention_weights.squeeze(0), pooled_features)  # K X N, K X L
```

### Comparing `hi-ml-0.2.9/src/health_ml/runner.py` & `hi-ml-0.3.0/src/health_ml/runner.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,50 +1,62 @@
 #! /usr/bin/env python
 
 #  ------------------------------------------------------------------------------------------
 #  Copyright (c) Microsoft Corporation. All rights reserved.
 #  Licensed under the MIT License (MIT). See LICENSE in the repo root for license information.
 #  ------------------------------------------------------------------------------------------
 import argparse
+import contextlib
+from datetime import datetime
 import logging
 import os
+import traceback
 import param
 import sys
 from pathlib import Path
-from typing import Any, Dict, List, Optional, Tuple
+from typing import Dict, List, Optional, Tuple
 
-import matplotlib
-from azureml.core import Workspace, Run
+from azureml.core import Workspace
 
 # Add hi-ml packages to sys.path so that AML can find them if we are using the runner directly from the git repo
 himl_root = Path(__file__).resolve().parent.parent.parent.parent
-folders_to_add = [himl_root / "hi-ml" / "src",
-                  himl_root / "hi-ml-azure" / "src",
-                  himl_root / "hi-ml-cpath" / "src"]
+folders_to_add = [himl_root / "hi-ml" / "src", himl_root / "hi-ml-azure" / "src", himl_root / "hi-ml-cpath" / "src"]
 for folder in folders_to_add:
     if folder.is_dir():
         sys.path.insert(0, str(folder))
 
 from health_azure import AzureRunInfo, submit_to_azure_if_needed  # noqa: E402
+from health_azure.argparsing import create_argparser, parse_arguments, ParserResult, apply_overrides  # noqa: E402
+from health_azure.amulet import prepare_amulet_job, is_amulet_job  # noqa: E402
 from health_azure.datasets import create_dataset_configs  # noqa: E402
-from health_azure.logging import logging_to_stdout   # noqa: E402
+from health_azure.himl import DEFAULT_DOCKER_BASE_IMAGE, OUTPUT_FOLDER  # noqa: E402
+from health_azure.logging import logging_to_stdout  # noqa: E402
 from health_azure.paths import is_himl_used_from_git_repo  # noqa: E402
-from health_azure.amulet import prepare_amulet_job  # noqa: E402
-from health_azure.utils import (get_workspace, get_ml_client, is_local_rank_zero,  # noqa: E402
-                                is_running_in_azure_ml, set_environment_variables_for_multi_node,
-                                create_argparser, parse_arguments, ParserResult, apply_overrides,
-                                filter_v2_input_output_args)
+from health_azure.utils import (  # noqa: E402
+    ENV_LOCAL_RANK,
+    ENV_NODE_RANK,
+    get_workspace,
+    get_ml_client,
+    is_local_rank_zero,
+    is_running_in_azure_ml,
+    set_environment_variables_for_multi_node,
+    filter_v2_input_output_args,
+    is_global_rank_zero,
+)
 
-from health_ml.experiment_config import ExperimentConfig  # noqa: E402
+from health_ml.eval_runner import EvalRunner  # noqa: E402
+from health_ml.experiment_config import DEBUG_DDP_ENV_VAR, ExperimentConfig, RunnerMode  # noqa: E402
 from health_ml.lightning_container import LightningContainer  # noqa: E402
-from health_ml.run_ml import MLRunner  # noqa: E402
+from health_ml.runner_base import RunnerBase  # noqa: E402
+from health_ml.training_runner import TrainingRunner  # noqa: E402
 from health_ml.utils import fixed_paths  # noqa: E402
-from health_ml.utils.common_utils import (DEFAULT_DOCKER_BASE_IMAGE, check_conda_environment,  # noqa: E402
-                                          choose_conda_env_file, is_linux)
+from health_ml.utils.logging import ConsoleAndFileOutput  # noqa: E402
+from health_ml.utils.common_utils import check_conda_environment, choose_conda_env_file, is_linux  # noqa: E402
 from health_ml.utils.config_loader import ModelConfigLoader  # noqa: E402
+from health_ml.utils import health_ml_package_setup  # noqa: E402
 
 
 # We change the current working directory before starting the actual training. However, this throws off starting
 # the child training threads because sys.argv[0] is a relative path when running in AzureML. Turn that into an absolute
 # path.
 runner_path = Path(sys.argv[0])
 sys.argv[0] = str(runner_path.resolve())
@@ -54,47 +66,22 @@
     """
     On Linux only, import and initialize rpdb, to enable remote debugging if necessary.
     """
     # rpdb signal trapping does not work on Windows, as there is no SIGTRAP:
     if not is_linux():
         return
     import rpdb
+
     rpdb_port = 4444
     rpdb.handle_trap(port=rpdb_port)
     # For some reason, os.getpid() does not return the ID of what appears to be the currently running process.
-    logging.info("rpdb is handling traps. To debug: identify the main runner.py process, then as root: "
-                 f"kill -TRAP <process_id>; nc 127.0.0.1 {rpdb_port}")
-
-
-def package_setup_and_hacks() -> None:
-    """
-    Set up the Python packages where needed. In particular, reduce the logging level for some of the used
-    libraries, which are particularly talkative in DEBUG mode. Usually when running in DEBUG mode, we want
-    diagnostics about the model building itself, but not for the underlying libraries.
-    It also adds workarounds for known issues in some packages.
-    """
-    # Numba code generation is extremely talkative in DEBUG mode, disable that.
-    logging.getLogger('numba').setLevel(logging.WARNING)
-    # Matplotlib is also very talkative in DEBUG mode, filling half of the log file in a PR build.
-    logging.getLogger('matplotlib').setLevel(logging.INFO)
-    # Urllib3 prints out connection information for each call to write metrics, etc
-    logging.getLogger('urllib3').setLevel(logging.INFO)
-    logging.getLogger('msrest').setLevel(logging.INFO)
-    # AzureML prints too many details about logging metrics
-    logging.getLogger('azureml').setLevel(logging.INFO)
-    # Jupyter notebook report generation
-    logging.getLogger('papermill').setLevel(logging.INFO)
-    logging.getLogger('nbconvert').setLevel(logging.INFO)
-    # This is working around a spurious error message thrown by MKL, see
-    # https://github.com/pytorch/pytorch/issues/37377
-    os.environ['MKL_THREADING_LAYER'] = 'GNU'
-    # Workaround for issues with matplotlib on some X servers, see
-    # https://stackoverflow.com/questions/45993879/matplot-lib-fatal-io-error-25-inappropriate-ioctl-for-device-on-x
-    # -server-loc
-    matplotlib.use('Agg')
+    logging.info(
+        "rpdb is handling traps. To debug: identify the main runner.py process, then as root: "
+        f"kill -TRAP <process_id>; nc 127.0.0.1 {rpdb_port}"
+    )
 
 
 def create_runner_parser() -> argparse.ArgumentParser:
     """
     Creates a commandline parser, that understands all necessary arguments for training a model
 
     :return: An instance of ArgumentParser with args from ExperimentConfig added
@@ -112,16 +99,16 @@
     :param project_root: The root folder that contains all of the source code that should be executed.
     """
 
     def __init__(self, project_root: Path):
         self.project_root = project_root
         self.experiment_config: ExperimentConfig = ExperimentConfig()
         self.lightning_container: LightningContainer = None  # type: ignore
-        # This field stores the MLRunner object that has been created in the most recent call to the run() method.
-        self.ml_runner: Optional[MLRunner] = None
+        # This field stores the TrainingRunner object that has been created in the most recent call to the run() method.
+        self.ml_runner: Optional[RunnerBase] = None
 
     def parse_and_load_model(self) -> ParserResult:
         """
         Parses the command line arguments, and creates configuration objects for the model itself, and for the
         Azure-related parameters. Sets self.experiment_config to its proper values. Returns the
         parser output from parsing the model commandline arguments.
 
@@ -144,56 +131,72 @@
 
         # parse overrides and apply
         assert isinstance(container, param.Parameterized)
         parser2 = create_argparser(container)
         # For each parser, feed in the unknown settings from the previous parser. All commandline args should
         # be consumed by name, hence fail if there is something that is still unknown.
         parser2_result = parse_arguments(parser2, args=parser1_result.unknown, fail_on_unknown_args=True)
-        # Apply the overrides and validate. Overrides can come from either YAML settings or the commandline.
+        # Apply the commandline overrides and validate. Any parameters specified on the commandline should have
+        # higher priority than what is done in the model variant
+        assert isinstance(container, LightningContainer)
+        container.set_model_variant(experiment_config.model_variant)
         apply_overrides(container, parser2_result.overrides)  # type: ignore
         container.validate()
 
         self.lightning_container = container
 
         return parser2_result
 
     def validate(self) -> None:
         """
         Runs sanity checks on the whole experiment.
         """
         if not self.experiment_config.cluster:
             if self.lightning_container.hyperdrive:
-                raise ValueError("HyperDrive for hyperparameters tuning is only supported when submitting the job to "
-                                 "AzureML. You need to specify a compute cluster with the argument --cluster.")
-            if self.lightning_container.is_crossvalidation_enabled:
-                raise ValueError("Cross-validation is only supported when submitting the job to AzureML."
-                                 "You need to specify a compute cluster with the argument --cluster.")
+                raise ValueError(
+                    "HyperDrive for hyperparameters tuning is only supported when submitting the job to "
+                    "AzureML. You need to specify a compute cluster with the argument --cluster."
+                )
+            if self.lightning_container.is_crossvalidation_parent_run and not is_amulet_job():
+                raise ValueError(
+                    "Cross-validation is only supported when submitting the job to AzureML."
+                    "You need to specify a compute cluster with the argument --cluster."
+                )
 
     def additional_run_tags(self, script_params: List[str]) -> Dict[str, str]:
         """
         Gets the set of tags that will be added to the AzureML run as metadata.
 
         :param script_params: The commandline arguments used to invoke the present script.
         """
         return {
             "commandline_args": " ".join(script_params),
-            "tag": self.lightning_container.tag
+            "tag": self.lightning_container.tag,
+            **self.lightning_container.get_additional_aml_run_tags(),
+        }
+
+    def additional_environment_variables(self) -> Dict[str, str]:
+        return {
+            DEBUG_DDP_ENV_VAR: self.experiment_config.debug_ddp.value,
+            **self.lightning_container.get_additional_environment_variables(),
         }
 
     def run(self) -> Tuple[LightningContainer, AzureRunInfo]:
         """
         The main entry point for training and testing models from the commandline. This chooses a model to train
         via a commandline argument, runs training or testing, and writes all required info to disk and logs.
 
         :return: a tuple of the LightningContainer object and an AzureRunInfo containing all information about
             the present run (whether running in AzureML or not)
         """
-        # Usually, when we set logging to DEBUG, we want diagnostics about the model
-        # build itself, but not the tons of debug information that AzureML submissions create.
-        logging_to_stdout(logging.INFO if is_local_rank_zero() else "ERROR")
+        # Suppress the logging from all processes but the one for GPU 0 on each node, to make log files more readable
+        log_level = logging.INFO if is_local_rank_zero() else logging.ERROR
+        logging_to_stdout(log_level)
+        # When running in Azure, also output logging to a file. This can help in particular when jobs
+        # get preempted, but we don't get access to the logs from the previous incarnation of the job
         initialize_rpdb()
         self.parse_and_load_model()
         self.validate()
         azure_run_info = self.submit_to_azureml_if_needed()
         self.run_in_situ(azure_run_info)
         return self.lightning_container, azure_run_info
 
@@ -202,69 +205,60 @@
         Submit a job to AzureML, returning the resulting Run object, or exiting if we were asked to wait for
         completion and the Run did not succeed.
 
         :return: an AzureRunInfo object containing all of the details of the present run. If AzureML is not
             specified, the attribute 'run' will None, but the object still contains helpful information
             about datasets etc
         """
-
-        def after_submission_hook(azure_run: Run) -> None:
-            """
-            A function that will be called right after job submission.
-            """
-            # Set the default display name to what was provided as the "tag". This will affect single runs
-            # and Hyperdrive parent runs
-            if self.lightning_container.tag:
-                azure_run.display_name = self.lightning_container.tag
-
         root_folder = self.project_root
         entry_script = Path(sys.argv[0]).resolve()
         script_params = sys.argv[1:]
 
-        # TODO: Update environment variables
-        environment_variables: Dict[str, Any] = {}
+        environment_variables = self.additional_environment_variables()
 
         # Get default datastore from the provided workspace. Authentication can take a few seconds, hence only do
         # that if we are really submitting to AzureML.
         workspace: Optional[Workspace] = None
         if self.experiment_config.cluster:
             try:
-                workspace = get_workspace()
+                workspace = get_workspace(workspace_config_path=self.experiment_config.workspace_config_path)
             except ValueError:
-                raise ValueError("Unable to submit the script to AzureML because no workspace configuration file "
-                                 "(config.json) was found.")
+                raise ValueError(
+                    "Unable to submit the script to AzureML because no workspace configuration file "
+                    "(config.json) was found."
+                )
 
         if self.lightning_container.datastore:
             datastore = self.lightning_container.datastore
         elif workspace:
             datastore = workspace.get_default_datastore().name
         else:
             datastore = ""
 
         local_datasets = self.lightning_container.local_datasets
         all_local_datasets = [Path(p) for p in local_datasets] if len(local_datasets) > 0 else []
         # When running in AzureML, respect the commandline flag for mounting. Outside of AML, we always mount
         # datasets to be quicker.
         use_mounting = self.experiment_config.mount_in_azureml if self.experiment_config.cluster else True
-        input_datasets = \
-            create_dataset_configs(all_azure_dataset_ids=self.lightning_container.azure_datasets,
-                                   all_dataset_mountpoints=self.lightning_container.dataset_mountpoints,
-                                   all_local_datasets=all_local_datasets,  # type: ignore
-                                   datastore=datastore,
-                                   use_mounting=use_mounting)
-
-        if self.experiment_config.strictly_aml_v1:
-            hyperdrive_config = self.lightning_container.get_hyperdrive_config()
-            hyperparam_args = None
-        else:
-            hyperparam_args = self.lightning_container.get_hyperparam_args()
-            hyperdrive_config = None
+        input_datasets = create_dataset_configs(
+            all_azure_dataset_ids=self.lightning_container.azure_datasets,
+            all_dataset_mountpoints=self.lightning_container.dataset_mountpoints,
+            all_local_datasets=all_local_datasets,  # type: ignore
+            datastore=datastore,
+            use_mounting=use_mounting,
+        )
 
         if self.experiment_config.cluster and not is_running_in_azure_ml():
-            ml_client = get_ml_client()
+            if self.experiment_config.strictly_aml_v1:
+                hyperdrive_config = self.lightning_container.get_hyperdrive_config()
+                hyperparam_args = None
+            else:
+                hyperparam_args = self.lightning_container.get_hyperparam_args()
+                hyperdrive_config = None
+            ml_client = get_ml_client(aml_workspace=workspace) if not self.experiment_config.strictly_aml_v1 else None
 
             env_file = choose_conda_env_file(env_file=self.experiment_config.conda_env)
             logging.info(f"Using this Conda environment definition: {env_file}")
             check_conda_environment(env_file)
 
             azure_run_info = submit_to_azure_if_needed(
                 entry_script=entry_script,
@@ -276,86 +270,148 @@
                 compute_cluster_name=self.experiment_config.cluster,
                 environment_variables=environment_variables,
                 default_datastore=datastore,
                 experiment_name=self.lightning_container.effective_experiment_name,
                 input_datasets=input_datasets,  # type: ignore
                 num_nodes=self.experiment_config.num_nodes,
                 wait_for_completion=self.experiment_config.wait_for_completion,
+                max_run_duration=self.experiment_config.max_run_duration,
                 ignored_folders=[],
                 submit_to_azureml=bool(self.experiment_config.cluster),
                 docker_base_image=DEFAULT_DOCKER_BASE_IMAGE,
                 docker_shm_size=self.experiment_config.docker_shm_size,
                 hyperdrive_config=hyperdrive_config,
                 hyperparam_args=hyperparam_args,
-                create_output_folders=False,
-                after_submission=after_submission_hook,
+                display_name=self.lightning_container.tag,
                 tags=self.additional_run_tags(script_params),
                 strictly_aml_v1=self.experiment_config.strictly_aml_v1,
+                identity_based_auth=self.experiment_config.identity_based_auth,
             )
         else:
             azure_run_info = submit_to_azure_if_needed(
                 input_datasets=input_datasets,  # type: ignore
                 submit_to_azureml=False,
+                environment_variables=environment_variables,
                 strictly_aml_v1=self.experiment_config.strictly_aml_v1,
+                default_datastore=datastore,
             )
         if azure_run_info.run:
             # This code is only reached inside Azure. Set display name again - this will now affect
             # Hypdrive child runs (for other jobs, this has already been done after submission)
             suffix = None
-            if self.lightning_container.is_crossvalidation_enabled:
+            if self.lightning_container.is_crossvalidation_child_run:
                 suffix = f"crossval {self.lightning_container.crossval_index}"
             elif self.lightning_container.different_seeds > 0:
                 suffix = f"seed {self.lightning_container.random_seed}"
             if suffix:
                 current_name = self.lightning_container.tag or azure_run_info.run.display_name
                 azure_run_info.run.display_name = f"{current_name} {suffix}"
-
         # submit_to_azure_if_needed calls sys.exit after submitting to AzureML. We only reach this when running
         # the script locally or in AzureML.
         return azure_run_info
 
     def run_in_situ(self, azure_run_info: AzureRunInfo) -> None:
         """
         Actually run the AzureML job; this method will typically run on an Azure VM.
 
         :param azure_run_info: Contains all information about the present run in AzureML, in particular where the
         datasets are mounted.
         """
-        # Only set the logging level now. Usually, when we set logging to DEBUG, we want diagnostics about the model
-        # build itself, but not the tons of debug information that AzureML submissions create.
-        # Suppress the logging from all processes but the one for GPU 0 on each node, to make log files more readable
-        logging_to_stdout("INFO" if is_local_rank_zero() else "ERROR")
-        package_setup_and_hacks()
+        health_ml_package_setup()
         prepare_amulet_job()
 
-        # Set environment variables for multi-node training if needed. This function will terminate early
-        # if it detects that it is not in a multi-node environment.
-        if self.experiment_config.num_nodes > 1:
-            set_environment_variables_for_multi_node()
-        self.ml_runner = MLRunner(
-            experiment_config=self.experiment_config,
-            container=self.lightning_container,
-            project_root=self.project_root)
-        self.ml_runner.setup(azure_run_info)
-        self.ml_runner.run()
+        # Add tags and arguments to Amulet runs
+        if is_amulet_job():
+            assert azure_run_info.run is not None
+            azure_run_info.run.set_tags(self.additional_run_tags(sys.argv[1:]))
+
+        if self.experiment_config.mode == RunnerMode.TRAIN:
+            # Set environment variables for multi-node training if needed. This function will terminate early
+            # if it detects that it is not in a multi-node environment.
+            if self.experiment_config.num_nodes > 1:
+                set_environment_variables_for_multi_node()
+            self.ml_runner = TrainingRunner(
+                experiment_config=self.experiment_config,
+                container=self.lightning_container,
+                project_root=self.project_root,
+            )
+        elif self.experiment_config.mode == RunnerMode.EVAL_FULL:
+            self.ml_runner = EvalRunner(
+                experiment_config=self.experiment_config,
+                container=self.lightning_container,
+                project_root=self.project_root,
+            )
+        else:
+            raise ValueError(f"Unknown mode {self.experiment_config.mode}")
+        self.ml_runner.validate()
+        self.ml_runner.run_and_cleanup(azure_run_info)
 
 
 def run(project_root: Path) -> Tuple[LightningContainer, AzureRunInfo]:
     """
     The main entry point for training and testing models from the commandline. This chooses a model to train
     via a commandline argument, runs training or testing, and writes all required info to disk and logs.
 
     :param project_root: The root folder that contains all of the source code that should be executed.
     :return: If submitting to AzureML, returns the model configuration that was used for training,
-    including commandline overrides applied (if any). For details on the arguments, see the constructor of Runner.
+        including commandline overrides applied (if any). For details on the arguments, see the constructor of Runner.
+    """
+    if is_global_rank_zero():
+        print(f"Project root: {project_root}")
+    return Runner(project_root).run()
+
+
+def create_logging_filename() -> Path:
+    """Creates a file name for console logs, based on the current time and the DDP rank.
+    The filename is timestamped to seconds level, so that we also get a full history of all
+    low-priority preemptions, because each restart will create a logfile afresh.
+
+    :return: A full path to a file for console logs.
+    """
+    rank = os.getenv(ENV_LOCAL_RANK, "0")
+    node = os.getenv(ENV_NODE_RANK, "0")
+    timestamp = datetime.utcnow().strftime("%Y-%m-%dT%H%M%S")
+    cwd = Path.cwd()
+    logging_filename = cwd
+    # DDP subprocesses may already be running in the "outputs" folder. Add the "outputs" hence only if necessary.
+    if cwd.name != OUTPUT_FOLDER:
+        logging_filename = logging_filename / Path(OUTPUT_FOLDER)
+    logging_filename = logging_filename / "console_logs" / f"logging_{timestamp}_node{node}_rank{rank}.txt"
+    logging_filename.parent.mkdir(parents=True, exist_ok=True)
+    print(f"Rank {rank}: Redirecting all console logs to {logging_filename}")
+    return logging_filename
+
+
+def run_with_logging(project_root: Path) -> Tuple[LightningContainer, AzureRunInfo]:
+    """
+    Start the main main entry point for training and testing models from the commandline.
+    When running in Azure, this method also redirects the stdout stream, so that all console output is visible both on
+    the console and stored in a file. The filename is timestamped and contains the DDP rank of the current process.
+
+    :param project_root: The root folder that contains all of the source code that should be executed.
+    :return: If submitting to AzureML, returns the model configuration that was used for training,
+        including commandline overrides applied (if any). For details on the arguments, see the constructor of Runner.
     """
-    print(f"project root: {project_root}")
-    runner = Runner(project_root)
-    return runner.run()
+    if is_running_in_azure_ml():
+        logging_filename = create_logging_filename()
+        with logging_filename.open("w") as logging_file:
+            console_and_file = ConsoleAndFileOutput(logging_file)
+            with contextlib.redirect_stdout(console_and_file):
+                try:
+                    return run(project_root)
+                except:  # noqa
+                    # Exceptions would only be printed to the console at the very top level, and would not be visible
+                    # in the log file. Hence, write here specifically.
+                    traceback.print_exc(file=logging_file)
+                    raise
+                finally:
+                    logging_file.flush()
+    return run(project_root)
 
 
 def main() -> None:
-    run(project_root=fixed_paths.repository_root_directory() if is_himl_used_from_git_repo() else Path.cwd())
+    project_root = fixed_paths.repository_root_directory() if is_himl_used_from_git_repo() else Path.cwd()
+    run_with_logging(project_root)
 
 
 if __name__ == '__main__':
     main()
```

### Comparing `hi-ml-0.2.9/src/health_ml/utils/bag_utils.py` & `hi-ml-0.3.0/src/health_ml/utils/bag_utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -18,20 +18,22 @@
 
     >>> sampler = BagSampler([1, 1, 0, 2, 0, 1])
     >>> list(sampler)
     [[2, 4], [0, 1, 5], [3]]
     >>> loader = DataLoader(dataset, batch_sampler=sampler)
     """
 
-    def __init__(self,
-                 bag_ids: Sequence,
-                 shuffle_bags: bool = False,
-                 shuffle_samples: bool = False,
-                 max_bag_size: int = 0,
-                 generator: Optional[torch.Generator] = None) -> None:
+    def __init__(
+        self,
+        bag_ids: Sequence,
+        shuffle_bags: bool = False,
+        shuffle_samples: bool = False,
+        max_bag_size: int = 0,
+        generator: Optional[torch.Generator] = None,
+    ) -> None:
         """
         :param bag_ids: The bag IDs for each sample, of the same length as the dataset.
         :param shuffle_bags: Whether the bags should be iterated in random order.
         :param shuffle_samples: Whether the instances in each bag should be shuffled.
         :param max_bag_size: Upper bound on number of instances in each loaded bag. If 0 (default),
             will return all samples in each bag. If > 0 and `shuffle_samples=True`, bags larger than
             `max_bag_size` will yield random subsets of instances. Note that setting `max_bag_size > 0`
@@ -45,29 +47,27 @@
         self.shuffle_samples = shuffle_samples
         self.max_bag_size = max_bag_size
         self.generator = generator
 
     def __iter__(self) -> Iterator[List[int]]:
         generator = self.generator or _create_generator()
         n_bags = len(self.unique_bag_ids)
-        bag_sequence = torch.randperm(n_bags, generator=generator).tolist() \
-            if self.shuffle_bags else range(n_bags)
+        bag_sequence = torch.randperm(n_bags, generator=generator).tolist() if self.shuffle_bags else range(n_bags)
         for bag_idx in bag_sequence:
             yield self.get_bag(bag_idx, generator)
 
-    def get_bag(self, bag_index: int, generator: Optional[torch.Generator] = None) \
-            -> List[int]:
-        bag, = np.where(self.bag_indices == bag_index)
+    def get_bag(self, bag_index: int, generator: Optional[torch.Generator] = None) -> List[int]:
+        (bag,) = np.where(self.bag_indices == bag_index)
         if self.shuffle_samples:
             if generator is None:
                 generator = self.generator or _create_generator()
             perm = torch.randperm(len(bag), generator=generator)
             bag = np.atleast_1d(bag[perm])  # pytorch squeezes singleton tensors
         if self.max_bag_size > 0:
-            bag = bag[:self.max_bag_size]
+            bag = bag[: self.max_bag_size]
         return bag.tolist()
 
     def __len__(self) -> int:
         return len(self.unique_bag_ids)
 
     def __getstate__(self) -> Dict:
         # torch.Generator is not pickleable, so we need to serialise only its internal state.
@@ -87,21 +87,23 @@
             generator.set_state(d['generator'])
         self.generator = generator
 
 
 class BagDataset(Dataset):
     """A wrapper dataset that iterates a base dataset in user-specified 'bags'."""
 
-    def __init__(self,
-                 base_dataset: Sequence,
-                 bag_ids: Sequence[int],
-                 shuffle_samples: bool = False,
-                 max_bag_size: int = 0,
-                 generator: Optional[torch.Generator] = None,
-                 collate_fn: Callable[[List], Any] = default_collate) -> None:
+    def __init__(
+        self,
+        base_dataset: Sequence,
+        bag_ids: Sequence[int],
+        shuffle_samples: bool = False,
+        max_bag_size: int = 0,
+        generator: Optional[torch.Generator] = None,
+        collate_fn: Callable[[List], Any] = default_collate,
+    ) -> None:
         """
         :param base_dataset: The source dataset whose samples will be grouped in bags.
         :param bag_ids: The bag IDs for each sample, of the same length as the dataset.
         :param shuffle_samples: Whether the instances in each bag should be shuffled.
         :param max_bag_size: Upper bound on number of instances in each loaded bag. If 0 (default),
         will return all samples in each bag. If > 0 and `shuffle_samples=True`, bags larger than
         `max_bag_size` will yield random subsets of instances. Note that setting `max_bag_size > 0`
@@ -110,37 +112,41 @@
         :param generator: The pseudorandom number generator to use for shuffling. By default, creates
         one with a random seed.
         :param collate_fn: Function to aggregate individual samples into a batch. Uses the PyTorch
         default if unspecified, which stacks tensors along their first dimension.
         More details in https://pytorch.org/docs/stable/data.html#dataloader-collate-fn
         """
         if len(base_dataset) != len(bag_ids):
-            raise ValueError(f"Base dataset and bag IDs must have the same length, "
-                             f"got {len(base_dataset)} and {len(bag_ids)}")
+            raise ValueError(
+                f"Base dataset and bag IDs must have the same length, " f"got {len(base_dataset)} and {len(bag_ids)}"
+            )
 
         self.base_dataset = base_dataset
-        self.bag_sampler = BagSampler(bag_ids,
-                                      shuffle_bags=False,  # bag shuffling is handled by dataloader
-                                      shuffle_samples=shuffle_samples,
-                                      max_bag_size=max_bag_size,
-                                      generator=generator)
+        self.bag_sampler = BagSampler(
+            bag_ids,
+            shuffle_bags=False,  # bag shuffling is handled by dataloader
+            shuffle_samples=shuffle_samples,
+            max_bag_size=max_bag_size,
+            generator=generator,
+        )
         self.collate_fn = collate_fn
         self.bag_ids = bag_ids
 
     def __len__(self) -> int:
         return len(self.bag_sampler)
 
     def __getitem__(self, index: int) -> Any:
         bag_indices = self.bag_sampler.get_bag(index)
         bag_samples = [self.base_dataset[i] for i in bag_indices]
         return self.collate_fn(bag_samples)
 
 
 class BatchedDataset(Dataset):
-    """ A wrapper class that aggregates multiple bags in a batch"""
+    """A wrapper class that aggregates multiple bags in a batch"""
+
     # TODO: Just a stub for now; extend to enable shuffling and/or other batching strategies
 
     def __init__(self, base_dataset: Sequence, batch_size: int) -> None:
         self.base_dataset = base_dataset
         self.batch_size = batch_size
 
     def __len__(self) -> int:
@@ -171,20 +177,26 @@
         if not all(len(other) == elem_len for other in batch[1:]):
             raise RuntimeError("Every element in the batch should be of equal size")
         return tuple(zip(*batch))
 
     return batch  # return other types as a plain list
 
 
-def create_bag_dataloader(base_dataset: Sequence, bag_ids: Sequence,
-                          *,  # make following arguments keyword-only to avoid confusion
-                          shuffle_bags: bool, shuffle_samples: bool, max_bag_size: int = 0,
-                          batch_size: Optional[int] = 1, collate_fn: Callable[[List], Any] = default_collate,
-                          generator: Optional[torch.Generator] = None,
-                          **dataloader_kwargs: Any) -> DataLoader:
+def create_bag_dataloader(
+    base_dataset: Sequence,
+    bag_ids: Sequence,
+    *,  # make following arguments keyword-only to avoid confusion
+    shuffle_bags: bool,
+    shuffle_samples: bool,
+    max_bag_size: int = 0,
+    batch_size: Optional[int] = 1,
+    collate_fn: Callable[[List], Any] = default_collate,
+    generator: Optional[torch.Generator] = None,
+    **dataloader_kwargs: Any,
+) -> DataLoader:
     """Create a DataLoader that consumes the given dataset in batches grouped by bag ID.
 
     :param base_dataset: The source dataset whose samples will be grouped in bags.
     :param bag_ids: The bag IDs for each sample, of the same length as the dataset.
     :param shuffle_bags: Whether the bags should be iterated in random order.
     :param shuffle_samples: Whether the instances in each bag should be shuffled.
     :param max_bag_size: Upper bound on number of instances in each loaded bag. If 0 (default),
@@ -202,19 +214,23 @@
     :param generator: The pseudorandom number generator to use for shuffling. By default,
     creates one with a random seed.
     :param dataloader_kwargs: Further keyword arguments to be passed to the `DataLoader`, e.g.
     `num_workers`, `pin_memory`, etc.
     :return: The `DataLoader` configured to iterate one bag at a time.
     """
     generator = generator or _create_generator()
-    bag_dataset = BagDataset(base_dataset,
-                             bag_ids=bag_ids,
-                             max_bag_size=max_bag_size,
-                             shuffle_samples=shuffle_samples,
-                             generator=generator,
-                             collate_fn=collate_fn)
-    return DataLoader(bag_dataset,
-                      shuffle=shuffle_bags,
-                      generator=generator,
-                      batch_size=batch_size,
-                      collate_fn=None if batch_size is None else multibag_collate,
-                      **dataloader_kwargs)
+    bag_dataset = BagDataset(
+        base_dataset,
+        bag_ids=bag_ids,
+        max_bag_size=max_bag_size,
+        shuffle_samples=shuffle_samples,
+        generator=generator,
+        collate_fn=collate_fn,
+    )
+    return DataLoader(
+        bag_dataset,
+        shuffle=shuffle_bags,
+        generator=generator,
+        batch_size=batch_size,
+        collate_fn=None if batch_size is None else multibag_collate,
+        **dataloader_kwargs,
+    )
```

### Comparing `hi-ml-0.2.9/src/health_ml/utils/box_utils.py` & `hi-ml-0.3.0/src/health_ml/utils/box_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,14 +16,15 @@
 
     :param x: Horizontal coordinate of the top-left corner.
     :param y: Vertical coordinate of the top-left corner.
     :param w: Box width.
     :param h: Box height.
     :raises ValueError: If either `w` or `h` are <= 0.
     """
+
     x: int
     y: int
     w: int
     h: int
 
     def __post_init__(self) -> None:
         if self.w <= 0:
@@ -36,29 +37,23 @@
 
         :param shift: A length-2 sequence containing horizontal and vertical shifts.
         :return: A new box with updated `x = x + shift[0]` and `y = y + shift[1]`.
         :raises ValueError: If `shift` does not have two elements.
         """
         if len(shift) != 2:
             raise ValueError("Shift must be two-dimensional")
-        return Box(x=self.x + shift[0],
-                   y=self.y + shift[1],
-                   w=self.w,
-                   h=self.h)
+        return Box(x=self.x + shift[0], y=self.y + shift[1], w=self.w, h=self.h)
 
     def __mul__(self, factor: float) -> 'Box':
         """Scales the box by a given factor, e.g. when changing resolution.
 
         :param factor: The factor by which to multiply the box's location and dimensions.
         :return: The updated box, with location and dimensions rounded to `int`.
         """
-        return Box(x=int(self.x * factor),
-                   y=int(self.y * factor),
-                   w=int(self.w * factor),
-                   h=int(self.h * factor))
+        return Box(x=int(self.x * factor), y=int(self.y * factor), w=int(self.w * factor), h=int(self.h * factor))
 
     def __rmul__(self, factor: float) -> 'Box':
         """Scales the box by a given factor, e.g. when changing resolution.
 
         :param factor: The factor by which to multiply the box's location and dimensions.
         :return: The updated box, with location and dimensions rounded to `int`.
         """
@@ -66,26 +61,23 @@
 
     def __truediv__(self, factor: float) -> 'Box':
         """Scales the box by a given factor, e.g. when changing resolution.
 
         :param factor: The factor by which to divide the box's location and dimensions.
         :return: The updated box, with location and dimensions rounded to `int`.
         """
-        return self * (1. / factor)
+        return self * (1.0 / factor)
 
     def add_margin(self, margin: int) -> 'Box':
         """Adds a symmetric margin on all sides of the box.
 
         :param margin: The amount by which to enlarge the box.
         :return: A new box enlarged by `margin` on all sides.
         """
-        return Box(x=self.x - margin,
-                   y=self.y - margin,
-                   w=self.w + 2 * margin,
-                   h=self.h + 2 * margin)
+        return Box(x=self.x - margin, y=self.y - margin, w=self.w + 2 * margin, h=self.h + 2 * margin)
 
     def clip(self, other: 'Box') -> Optional['Box']:
         """Clips a box to the interior of another.
 
         This is useful to constrain a region to the interior of an image.
 
         :param other: Box representing the new constraints.
@@ -103,29 +95,30 @@
     def to_slices(self) -> Tuple[slice, slice]:
         """Converts the box to slices for indexing arrays.
 
         For example: `my_2d_array[my_box.to_slices()]`.
 
         :return: A 2-tuple with vertical and horizontal slices.
         """
-        return (slice(self.y, self.y + self.h),
-                slice(self.x, self.x + self.w))
+        return (slice(self.y, self.y + self.h), slice(self.x, self.x + self.w))
 
     @staticmethod
     def from_slices(slices: Sequence[slice]) -> 'Box':
         """Converts a pair of vertical and horizontal slices into a box.
 
         :param slices: A length-2 sequence containing vertical and horizontal `slice` objects.
         :return: A box with corresponding location and dimensions.
         """
         vert_slice, horz_slice = slices
-        return Box(x=horz_slice.start,
-                   y=vert_slice.start,
-                   w=horz_slice.stop - horz_slice.start,
-                   h=vert_slice.stop - vert_slice.start)
+        return Box(
+            x=horz_slice.start,
+            y=vert_slice.start,
+            w=horz_slice.stop - horz_slice.start,
+            h=vert_slice.stop - vert_slice.start,
+        )
 
 
 def get_bounding_box(mask: np.ndarray) -> Box:
     """Extracts a bounding box from a binary 2D array.
 
     :param mask: A 2D array with 0 (or `False`) as background and >0 (or `True`) as foreground.
     :return: The smallest box covering all non-zero elements of `mask`.
```

### Comparing `hi-ml-0.2.9/src/health_ml/utils/checkpoint_handler.py` & `hi-ml-0.3.0/src/health_ml/utils/checkpoint_handler.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,27 +1,24 @@
 #  -------------------------------------------------------------------------------------------
 #  Copyright (c) Microsoft Corporation. All rights reserved.
 #  Licensed under the MIT License (MIT). See LICENSE in the repo root for license information.
 #  -------------------------------------------------------------------------------------------
 
 import logging
-import os
-import uuid
+import tempfile
+from azureml.core import Run
 from pathlib import Path
 from typing import Optional
-from urllib.parse import urlparse
-
-import requests
-from azureml.core import Run
 
-from health_azure.utils import is_global_rank_zero
+from health_azure import RUN_CONTEXT
+from health_azure.utils import is_global_rank_zero, is_running_in_azure_ml
+from health_ml.utils.common_utils import DEFAULT_AML_UPLOAD_DIR
 from health_ml.lightning_container import LightningContainer
 from health_ml.utils.checkpoint_utils import (
-    MODEL_WEIGHTS_DIR_NAME,
-    CheckpointDownloader,
+    download_highest_epoch_checkpoint,
     find_recovery_checkpoint_on_disk_or_cloud,
 )
 
 
 class CheckpointHandler:
     """
     This class handles which checkpoints are used to initialize the model during train or test time
@@ -36,17 +33,19 @@
 
     def download_recovery_checkpoints_or_weights(self) -> None:
         """
         Download checkpoints from a run recovery object or from a given checkpoint. Set the checkpoints path based on
         the checkpoint_url, local_checkpoint or checkpoint from an azureml run id.
         This is called at the start of training.
         """
-
         if self.container.src_checkpoint:
-            self.trained_weights_path = self.get_local_checkpoints_path_or_download()
+            self.trained_weights_path = self.container.src_checkpoint.get_or_download_checkpoint(
+                download_dir=self.container.checkpoint_folder
+            )
+            self.container.trained_weights_path = self.trained_weights_path
 
     def additional_training_done(self) -> None:
         """
         Lets the handler know that training was done in this run.
         """
         self.has_continued_training = True
 
@@ -57,81 +56,86 @@
         prior to calling this function. Else, if the run gets pre-empted and automatically restarted in AML,
         the latest checkpoint will be present in this folder too.
 
         :return: Constructed checkpoint path to recover from.
         """
         if is_global_rank_zero():
             checkpoints = list(self.container.checkpoint_folder.rglob("*"))
-            logging.info(f"Available checkpoints: {len(checkpoints)}")
+            logging.info(f"There are {len(checkpoints)} checkpoints in the checkpoint folder:")
             for f in checkpoints:
-                logging.info(f)
+                logging.info(f.relative_to(self.container.checkpoint_folder))
         return find_recovery_checkpoint_on_disk_or_cloud(self.container.checkpoint_folder)
 
     def get_checkpoint_to_test(self) -> Path:
         """
-        Find the model checkpoint that should be used for inference. If the model
-        has been training, get the best checkpoint as defined by the container.
-        If the model was not trained in this run, then return the checkpoint from the trained_weights_path.
+        Find the model checkpoint that should be used for inference.
+
+        If the model has been doing training epochs, get the best checkpoint as defined by the container.
+        It is possible that the best checkpoint is not available on disk because the job got preempted. In those
+        cases, try to find the inference checkpoint by going through all inference checkpoints stored in the AzureML
+        run, downloading them and finding the one that has the highest epoch number (that must be the most recent
+        among the possibly multiple retry results).
+
+        If the model has not been doing training, but is set up to use a pre-trained
+        set of weights in `trained_weights_path`, return that.
         """
         if self.has_continued_training:
             # If model was trained, look for the best checkpoint
             checkpoint_from_current_run = self.container.get_checkpoint_to_test()
             if checkpoint_from_current_run.is_file():
                 logging.info(f"Using checkpoint from current run: {checkpoint_from_current_run}")
                 return checkpoint_from_current_run
-            else:
-                raise FileNotFoundError(f"Checkpoint file does not exist: {checkpoint_from_current_run}")
+            logging.warning(f"No inference checkpoint found from the current run: {checkpoint_from_current_run}")
+            logging.info("Trying to find an inference checkpoint in AzureML.")
+            downloaded_checkpoint = self.download_inference_checkpoint()
+            if downloaded_checkpoint is not None:
+                logging.info(f"Using a checkpoint found in the AzureML run: {downloaded_checkpoint}")
+                return downloaded_checkpoint
+            raise FileNotFoundError("No inference checkpoint file found locally nor in AzureML.")
         elif self.trained_weights_path:
             # Model was not trained, check if there is a local weight path.
             logging.info(f"Using pre-trained weights from {self.trained_weights_path}")
             return self.trained_weights_path
         raise ValueError("Unable to determine which checkpoint should be used for testing.")
 
-    @staticmethod
-    def download_weights(url: str, download_folder: Path) -> Path:
+    def get_relative_inference_checkpoint_path(self) -> Path:
+        """Returns the path of the model's inference checkpoint, relative to the container's output folder.
+
+        This will be the path where the inference checkpoint can be found in the AzureML run output (except
+        the `outputs` prefix that has to be added at the start)."""
+        expected_checkpoint_path = self.container.get_checkpoint_to_test()
+        try:
+            return expected_checkpoint_path.relative_to(self.container.outputs_folder)
+        except ValueError:
+            raise ValueError(
+                "Inference checkpoint path should be relative to the container's output folder. "
+                f"Checkpoint path: {expected_checkpoint_path}, "
+                f"output folder: {self.container.outputs_folder}"
+            )
+
+    def download_inference_checkpoint(self, download_folder: Optional[Path] = None) -> Optional[Path]:
         """
-        Download a checkpoint from checkpoint_url to the modelweights directory. The file name is determined from
-        from the file name in the URL. If that can't be determined, use a random file name.
+        For low-priority preemption that occured after training, try to download the inference checkpoint if that
+        is available in the AzureML run from a previous incarnation of the job. Downloads go into the `download_folder`.
+
+        The method returns None if no checkpoint was found, or if the
+        current code is executing outside of AzureML and hence can't access previous inference checkpoints in AzureML.
 
-        :param url: The URL from which the weights should be downloaded.
-        :param download_folder: The target folder for the download.
-        :return: A path to the downloaded file.
-        """
-        # assign the same filename as in the download url if possible, so that we can check for duplicates
-        # If that fails, map to a random uuid
-        file_name = os.path.basename(urlparse(url).path) or str(uuid.uuid4().hex)
-        checkpoint_path = download_folder / file_name
-        # only download if hasn't already been downloaded
-        if checkpoint_path.is_file():
-            logging.info(f"File already exists, skipping download: {checkpoint_path}")
-        else:
-            logging.info(f"Downloading weights from URL {url}")
-
-            response = requests.get(url, stream=True)
-            response.raise_for_status()
-            with open(checkpoint_path, "wb") as file:
-                for chunk in response.iter_content(chunk_size=1024):
-                    file.write(chunk)
-        return checkpoint_path
-
-    def get_local_checkpoints_path_or_download(self) -> Path:
-        """
-        Get the path to the local weights to use or download them.
-        """
-
-        if self.container.src_checkpoint_is_local_file:
-            checkpoint_path = Path(self.container.src_checkpoint)
-        elif self.container.src_checkpoint_is_url:
-            download_folder = self.container.checkpoint_folder / MODEL_WEIGHTS_DIR_NAME
-            download_folder.mkdir(exist_ok=True, parents=True)
-            checkpoint_path = self.download_weights(url=self.container.src_checkpoint, download_folder=download_folder)
-        elif self.container.src_checkpoint_is_aml_run_id:
-            downloader = CheckpointDownloader(
-                run_id=self.container.src_checkpoint, download_dir=self.container.outputs_folder
+        :param download_folder: The folder where the checkpoints should be downloaded to. If not provided, use a
+            temp folder.
+        :return: The path to a downloaded inference checkpoint, or None if no checkpoint was available.
+        """
+        # This logic will only trigger in AzureML. Download should only happen once per node.
+        if is_running_in_azure_ml() and is_global_rank_zero():
+            download_folder = download_folder or Path(tempfile.mkdtemp())
+            inference_checkpoint_azureml_path = (
+                Path(DEFAULT_AML_UPLOAD_DIR) / self.get_relative_inference_checkpoint_path()
+            ).as_posix()
+            highest_epoch_checkpoint = download_highest_epoch_checkpoint(
+                run=RUN_CONTEXT, checkpoint_suffix=inference_checkpoint_azureml_path, output_folder=download_folder
             )
-            checkpoint_path = downloader.local_checkpoint_path
-        else:
-            raise ValueError("Unable to determine how to get the checkpoint path.")
-
-        if checkpoint_path is None or not checkpoint_path.is_file():
-            raise FileNotFoundError(f"Could not find the weights file at {checkpoint_path}")
-        return checkpoint_path
+            if highest_epoch_checkpoint is None:
+                logging.info("No inference checkpoint was found in the AzureML run.")
+                return None
+            logging.info("An inference checkpoint was found in the AzureML run.")
+            return highest_epoch_checkpoint
+        return None
```

### Comparing `hi-ml-0.2.9/src/health_ml/utils/common_utils.py` & `hi-ml-0.3.0/src/health_ml/utils/common_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -45,15 +45,14 @@
 
 # run recovery
 RUN_RECOVERY_ID_KEY = "run_recovery_id"
 RUN_RECOVERY_FROM_ID_KEY_NAME = "recovered_from"
 
 # other
 EFFECTIVE_RANDOM_SEED_KEY_NAME = "effective_random_seed"
-DEFAULT_DOCKER_BASE_IMAGE = "mcr.microsoft.com/azureml/openmpi3.1.2-cuda10.2-cudnn8-ubuntu18.04"
 
 
 @unique
 class ModelExecutionMode(Enum):
     """
     Model execution mode
     """
@@ -131,20 +130,22 @@
     if env_file is not None:
         if env_file.is_file():
             return env_file
         raise FileNotFoundError(f"The Conda file specified on the commandline could not be found: {env_file}")
     # When running from the Git repo, then stop search for environment file at repository root. Otherwise,
     # search from current folder all the way up
     stop_at = [paths.git_repo_root_folder()] if paths.is_himl_used_from_git_repo() else []
-    env_file = find_file_in_parent_folders(paths.ENVIRONMENT_YAML_FILE_NAME,
-                                           start_at_path=Path.cwd(),
-                                           stop_at_path=stop_at)
+    env_file = find_file_in_parent_folders(
+        paths.ENVIRONMENT_YAML_FILE_NAME, start_at_path=Path.cwd(), stop_at_path=stop_at
+    )
     if env_file is None:
-        raise FileNotFoundError(f"No Conda environment file '{paths.ENVIRONMENT_YAML_FILE_NAME}' was found in the "
-                                "current folder or its parent folders")
+        raise FileNotFoundError(
+            f"No Conda environment file '{paths.ENVIRONMENT_YAML_FILE_NAME}' was found in the "
+            "current folder or its parent folders"
+        )
     return env_file
 
 
 def check_conda_environment(env_file: Path) -> None:
     """Tests if the given conda environment files is valid. In particular, it must not contain "include" statements
     in the pip section.
 
@@ -217,10 +218,11 @@
     """If the MONAI package is available, set its shared seed to make all MONAI operations deterministic.
     If MONAI is not available, nothing will happen.
 
     :param seed: The random seed to use for MONAI."""
     try:
         # MONAI is not part of the core hi-ml requirements, this import can fail.
         from monai.utils import set_determinism  # type: ignore
+
         set_determinism(seed=seed)
     except ImportError:
         pass
```

### Comparing `hi-ml-0.2.9/src/health_ml/utils/config_loader.py` & `hi-ml-0.3.0/src/health_ml/utils/config_loader.py`

 * *Files identical despite different names*

### Comparing `hi-ml-0.2.9/src/health_ml/utils/diagnostics.py` & `hi-ml-0.3.0/src/health_ml/utils/diagnostics.py`

 * *Files 24% similar despite different names*

```diff
@@ -5,26 +5,25 @@
 import logging
 import time
 from typing import Any, Optional, Set
 
 import torch
 from pytorch_lightning import Callback, LightningModule, Trainer
 from pytorch_lightning.utilities.distributed import rank_zero_only
+from pytorch_lightning.utilities.types import STEP_OUTPUT
 
 
 class EpochTimers:
     """
     Contains all information necessary to compute the IO metrics: Epoch times, batch times, loading times.
     """
 
-    def __init__(self,
-                 max_batch_load_time_seconds: float = 0.5,
-                 max_load_time_warnings: int = 3,
-                 max_load_time_epochs: int = 5
-                 ) -> None:
+    def __init__(
+        self, max_batch_load_time_seconds: float = 0.5, max_load_time_warnings: int = 3, max_load_time_epochs: int = 5
+    ) -> None:
         """
         :param max_batch_load_time_seconds: The maximum expected loading time for a minibatch (given in seconds).
             If the loading time exceeds this threshold, a warning is printed.
         :param max_load_time_warnings: The maximum number of warnings that will be printed per epoch.
         :param max_load_time_epochs: The maximum number of epochs where warnings about the loading time are printed.
         """
         self.max_batch_load_time_seconds = max_batch_load_time_seconds
@@ -96,18 +95,20 @@
         if batch_index == 0:
             logging.info(f"{message_prefix}: Loaded the first minibatch of data in {item_load_time:0.2f} sec.")
         elif item_load_time > self.max_batch_load_time_seconds:
             self.load_time_warning_epochs.add(epoch)
             self.num_load_time_exceeded += 1
             self.total_extra_load_time += item_load_time
             if self.num_load_time_warnings < self.max_load_time_warnings and self.should_warn_in_this_epoch:
-                logging.warning(f"{message_prefix}: Loading minibatch {batch_index} took {item_load_time:0.2f} sec. "
-                                "This can mean that there are not enough data loader worker processes, or that there "
-                                "is a performance problem in loading. This warning will be printed at most "
-                                f"{self.max_load_time_warnings} times in at most {self.max_load_time_epochs} epochs.")
+                logging.warning(
+                    f"{message_prefix}: Loading minibatch {batch_index} took {item_load_time:0.2f} sec. "
+                    "This can mean that there are not enough data loader worker processes, or that there "
+                    "is a performance problem in loading. This warning will be printed at most "
+                    f"{self.max_load_time_warnings} times in at most {self.max_load_time_epochs} epochs."
+                )
                 self.num_load_time_warnings += 1
         return item_load_time
 
     def batch_end(self) -> float:
         """
         Called after a minibatch has been processed (training or validation step completed). Returns the time it took
         to process the current batch (including loading).
@@ -150,38 +151,40 @@
     METRICS_PREFIX = "timing/"
     """The prefix for all metrics collected by this callback."""
     TRAIN_PREFIX = "train/"
     """The prefix for all metrics collected during training."""
     VAL_PREFIX = "val/"
     """The prefix for all metrics collected during validation."""
 
-    def __init__(self,
-                 max_batch_load_time_seconds: float = 0.5,
-                 max_load_time_warnings: int = 3,
-                 max_load_time_epochs: int = 5
-                 ) -> None:
+    def __init__(
+        self, max_batch_load_time_seconds: float = 0.5, max_load_time_warnings: int = 3, max_load_time_epochs: int = 5
+    ) -> None:
         """
         :param max_batch_load_time_seconds: The maximum expected loading time for a minibatch (given in seconds).
             If the loading time exceeds this threshold, a warning is printed. The maximum number of such warnings is
             controlled by the other arguments.
         :param max_load_time_warnings: The maximum number of warnings about increased loading time that will be printed
             per epoch. For example, if max_load_time_warnings=3, at most 3 of these warnings will be printed within an
             epoch. The 4th minibatch with loading time over the threshold would not generate any warning anymore.
             If set to 0, no warnings are printed at all.
         :param max_load_time_epochs: The maximum number of epochs where warnings about the loading time are printed.
             For example, if max_load_time_epochs=2, and at least 1 batch with increased loading time is observed in
             epochs 0 and 3, no further warnings about increased loading time would be printed from epoch 4 onwards.
         """
         # Timers for monitoring data loading time
-        self.train_timers = EpochTimers(max_batch_load_time_seconds=max_batch_load_time_seconds,
-                                        max_load_time_warnings=max_load_time_warnings,
-                                        max_load_time_epochs=max_load_time_epochs)
-        self.val_timers = EpochTimers(max_batch_load_time_seconds=max_batch_load_time_seconds,
-                                      max_load_time_warnings=max_load_time_warnings,
-                                      max_load_time_epochs=max_load_time_epochs)
+        self.train_timers = EpochTimers(
+            max_batch_load_time_seconds=max_batch_load_time_seconds,
+            max_load_time_warnings=max_load_time_warnings,
+            max_load_time_epochs=max_load_time_epochs,
+        )
+        self.val_timers = EpochTimers(
+            max_batch_load_time_seconds=max_batch_load_time_seconds,
+            max_load_time_warnings=max_load_time_warnings,
+            max_load_time_epochs=max_load_time_epochs,
+        )
         self.module: Optional[LightningModule] = None
 
     def on_fit_start(self, trainer: Trainer, pl_module: LightningModule) -> None:
         """
         This is called at the start of training. It stores the model that is being trained, because it will be used
         later to log values.
         """
@@ -207,50 +210,54 @@
         # In validation epochs, mark that it has been completed. Training epochs are marked completed already
         # at the start of the validation epoch.
         self.val_timers.epoch_end()
         # Write all IO stats here, so that the order on the console is Train start, train end, val start, val end.
         self.write_and_log_epoch_time(is_training=True)
         self.write_and_log_epoch_time(is_training=False)
 
-    def on_train_batch_start(self,  # type: ignore
-                             trainer: Trainer,
-                             pl_module: LightningModule,
-                             batch: Any,
-                             batch_idx: int,
-                             dataloader_idx: int,
-                             ) -> None:
+    def on_train_batch_start(
+        self,  # type: ignore
+        trainer: Trainer,
+        pl_module: LightningModule,
+        batch: Any,
+        batch_idx: int,
+        dataloader_idx: int,
+    ) -> None:
         self.batch_start(batch_idx=batch_idx, is_training=True)
 
-    def on_validation_batch_start(self,
-                                  trainer: Trainer,
-                                  pl_module: LightningModule,
-                                  batch: Any,
-                                  batch_idx: int,
-                                  dataloader_idx: int,
-                                  ) -> None:
+    def on_validation_batch_start(
+        self,
+        trainer: Trainer,
+        pl_module: LightningModule,
+        batch: Any,
+        batch_idx: int,
+        dataloader_idx: int,
+    ) -> None:
         self.batch_start(batch_idx=batch_idx, is_training=False)
 
-    def on_train_batch_end(self,  # type: ignore
-                           trainer: Trainer,
-                           pl_module: LightningModule,
-                           outputs: Any,
-                           batch: Any,
-                           batch_idx: int,
-                           dataloader_idx: int,
-                           ) -> None:
+    def on_train_batch_end(
+        self,  # type: ignore
+        trainer: Trainer,
+        pl_module: LightningModule,
+        outputs: Any,
+        batch: Any,
+        batch_idx: int,
+        dataloader_idx: int,
+    ) -> None:
         self.batch_end(is_training=True)
 
-    def on_validation_batch_end(self,
-                                trainer: Trainer,
-                                pl_module: LightningModule,
-                                outputs: Any,
-                                batch: Any,
-                                batch_idx: int,
-                                dataloader_idx: int,
-                                ) -> None:
+    def on_validation_batch_end(
+        self,
+        trainer: Trainer,
+        pl_module: LightningModule,
+        outputs: Any,
+        batch: Any,
+        batch_idx: int,
+        dataloader_idx: int,
+    ) -> None:
         self.batch_end(is_training=False)
 
     @rank_zero_only
     def batch_start(self, batch_idx: int, is_training: bool) -> None:
         """
         Shared code to keep track of minibatch loading times. This is only done on global rank zero.
 
@@ -270,51 +277,47 @@
         Shared code to keep track of minibatch loading times. This is only done on global rank zero.
 
         :param is_training: If true, this has been called from `on_train_batch_end`, otherwise it has been called from
             `on_validation_batch_end`.
         """
         timers = self.get_timers(is_training=is_training)
         batch_time = timers.batch_end()
-        self.log_metric(self.BATCH_TIME + " avg",
-                        value=batch_time,
-                        is_training=is_training)
-        self.log_metric(self.BATCH_TIME + " max",
-                        value=batch_time,
-                        is_training=is_training,
-                        reduce_max=True)
+        self.log_metric(self.BATCH_TIME + " avg", value=batch_time, is_training=is_training)
+        self.log_metric(self.BATCH_TIME + " max", value=batch_time, is_training=is_training, reduce_max=True)
 
     @rank_zero_only
     def write_and_log_epoch_time(self, is_training: bool) -> None:
         """
         Reads the IO timers for either the training or validation epoch, writes them to the console, and logs the
         time per epoch.
 
         :param is_training: If True, show and log the data for the training epoch. If False, use the data for the
             validation epoch.
         """
         timers = self.get_timers(is_training=is_training)
         epoch_time_seconds = timers.total_epoch_time
         status = "training" if is_training else "validation"
         assert self.module is not None
-        logging.info(f"Epoch {self.module.current_epoch} {status} took {epoch_time_seconds:0.2f}sec, of which waiting "
-                     f"for data took {timers.total_load_time:0.2f} sec total.")
+        logging.info(
+            f"Epoch {self.module.current_epoch} {status} took {epoch_time_seconds:0.2f}sec, of which waiting "
+            f"for data took {timers.total_load_time:0.2f} sec total."
+        )
         if timers.num_load_time_exceeded > 0 and timers.should_warn_in_this_epoch:
-            logging.warning("The dataloaders were not fast enough to always supply the next batch in less than "
-                            f"{timers.max_batch_load_time_seconds:0.2f}sec.")
+            logging.warning(
+                "The dataloaders were not fast enough to always supply the next batch in less than "
+                f"{timers.max_batch_load_time_seconds:0.2f}sec."
+            )
             logging.warning(
                 f"In this epoch, {timers.num_load_time_exceeded} out of {timers.num_batches} batches exceeded the load "
-                f"time threshold. Total loading time for the slow batches was {timers.total_extra_load_time:0.2f}sec.")
+                f"time threshold. Total loading time for the slow batches was {timers.total_extra_load_time:0.2f}sec."
+            )
         # This metric is only written at rank zero, and hence must not be synchronized across workers. If attempted,
         # training will get stuck.
-        self.log_metric(self.EPOCH_TIME,
-                        value=epoch_time_seconds,
-                        is_training=is_training)
-        self.log_metric(self.EXCESS_LOADING_TIME,
-                        value=timers.total_extra_load_time,
-                        is_training=is_training)
+        self.log_metric(self.EPOCH_TIME, value=epoch_time_seconds, is_training=is_training)
+        self.log_metric(self.EXCESS_LOADING_TIME, value=timers.total_extra_load_time, is_training=is_training)
 
     @rank_zero_only
     def log_metric(self, name_suffix: str, value: float, is_training: bool, reduce_max: bool = False) -> None:
         """
         Write a metric given as a name/value pair to the currently trained module. The full name of the metric is
         composed of a fixed prefix "timing/", followed by either "train/" or "val/", and then the given suffix.
 
@@ -324,16 +327,119 @@
         :param reduce_max: If True, use torch.max as the aggregation function for the logged values. If False, use
             torch.mean
         """
         # Metrics are only written at global rank 0, and hence must not be synchronized. Trying to synchronize will
         # block training.
         prefix = self.TRAIN_PREFIX if is_training else self.VAL_PREFIX
         assert self.module is not None
-        self.module.log(name=self.METRICS_PREFIX + prefix + name_suffix, value=value,  # type: ignore
-                        on_step=False, on_epoch=True, sync_dist=False,
-                        reduce_fx=max if reduce_max else torch.mean)
+        self.module.log(
+            name=self.METRICS_PREFIX + prefix + name_suffix,
+            value=value,  # type: ignore
+            on_step=False,
+            on_epoch=True,
+            sync_dist=False,
+            reduce_fx=max if reduce_max else torch.mean,
+        )
 
     def get_timers(self, is_training: bool) -> EpochTimers:
         """
         Gets the object that holds all metrics and timers, for either the validation or the training epoch.
         """
         return self.train_timers if is_training else self.val_timers
+
+
+class TrainingDiagnoticsCallback(Callback):
+    """Callback that logs information about the training process."""
+
+    def on_train_epoch_start(self, trainer: Trainer, pl_module: LightningModule) -> None:
+        logging.info(f"Reached on_train_epoch_start on global rank {pl_module.global_rank}")
+
+    def on_train_epoch_end(self, trainer: Trainer, pl_module: LightningModule) -> None:
+        logging.info(f"Reached on_train_epoch_end on global rank {pl_module.global_rank}")
+
+    def on_validation_epoch_start(self, trainer: Trainer, pl_module: LightningModule) -> None:
+        logging.info(f"Reached on_validation_epoch_start on global rank {pl_module.global_rank}")
+
+    def on_validation_epoch_end(self, trainer: Trainer, pl_module: LightningModule) -> None:
+        logging.info(f"Reached on_validation_epoch_end on global rank {pl_module.global_rank}")
+
+    def on_test_epoch_start(self, trainer: Trainer, pl_module: LightningModule) -> None:
+        logging.info(f"Reached on_test_epoch_start on global rank {pl_module.global_rank}")
+
+    def on_test_epoch_end(self, trainer: Trainer, pl_module: LightningModule) -> None:
+        logging.info(f"Reached on_test_epoch_end on global rank {pl_module.global_rank}")
+
+    def on_train_start(self, trainer: Trainer, pl_module: LightningModule) -> None:
+        logging.info(f"Reached on_train_start on global rank {pl_module.global_rank}")
+
+    def on_train_end(self, trainer: Trainer, pl_module: LightningModule) -> None:
+        logging.info(f"Reached from on_train_end on global rank {pl_module.global_rank}")
+
+    def on_validation_start(self, trainer: Trainer, pl_module: LightningModule) -> None:
+        logging.info(f"Reached from on_validation_start on global rank {pl_module.global_rank}")
+
+    def on_validation_end(self, trainer: Trainer, pl_module: LightningModule) -> None:
+        logging.info(f"Reached from on_validation_end on global rank {pl_module.global_rank}")
+
+    def on_test_start(self, trainer: Trainer, pl_module: LightningModule) -> None:
+        logging.info(f"Reached from on_test_start on global rank {pl_module.global_rank}")
+
+    def on_test_end(self, trainer: Trainer, pl_module: LightningModule) -> None:
+        logging.info(f"Reached from on_test_end on global rank {pl_module.global_rank}")
+
+    def on_train_batch_start(
+        self, trainer: Trainer, pl_module: LightningModule, batch: Any, batch_idx: int, unused: int = 0
+    ) -> None:
+        logging.info(
+            f"Reached from on_train_batch_start on global rank {pl_module.global_rank} for batch_idx {batch_idx}"
+        )
+
+    def on_train_batch_end(
+        self,
+        trainer: Trainer,
+        pl_module: LightningModule,
+        outputs: STEP_OUTPUT,
+        batch: Any,
+        batch_idx: int,
+        unused: int = 0,
+    ) -> None:
+        logging.info(
+            f"Reached from on_train_batch_end on global rank {pl_module.global_rank} for batch_idx {batch_idx}"
+        )
+
+    def on_validation_batch_start(
+        self, trainer: Trainer, pl_module: LightningModule, batch: Any, batch_idx: int, unused: int = 0
+    ) -> None:
+        logging.info(
+            f"Reached from on_validation_batch_start on global rank {pl_module.global_rank} for batch_idx {batch_idx}"
+        )
+
+    def on_validation_batch_end(
+        self,
+        trainer: Trainer,
+        pl_module: LightningModule,
+        outputs: Optional[STEP_OUTPUT],
+        batch: Any,
+        batch_idx: int,
+        dataloader_idx: int,
+    ) -> None:
+        logging.info(
+            f"Reached from on_validation_batch_end on global rank {pl_module.global_rank} for batch_idx {batch_idx}"
+        )
+
+    def on_test_batch_end(
+        self,
+        trainer: Trainer,
+        pl_module: LightningModule,
+        outputs: Optional[STEP_OUTPUT],
+        batch: Any,
+        batch_idx: int,
+        dataloader_idx: int,
+    ) -> None:
+        logging.info(f"Reached from on_test_batch_end on global rank {pl_module.global_rank} for batch_idx {batch_idx}")
+
+    def on_test_batch_start(
+        self, trainer: Trainer, pl_module: LightningModule, batch: Any, batch_idx: int, unused: int = 0
+    ) -> None:
+        logging.info(
+            f"Reached from on_test_batch_start on global rank {pl_module.global_rank} for batch_idx {batch_idx}"
+        )
```

### Comparing `hi-ml-0.2.9/src/health_ml/utils/fixed_paths.py` & `hi-ml-0.3.0/src/health_ml/utils/fixed_paths.py`

 * *Files identical despite different names*

### Comparing `hi-ml-0.2.9/src/health_ml/utils/lightning_loggers.py` & `hi-ml-0.3.0/src/health_ml/utils/lightning_loggers.py`

 * *Files 3% similar despite different names*

```diff
@@ -2,20 +2,18 @@
 #  Copyright (c) Microsoft Corporation. All rights reserved.
 #  Licensed under the MIT License (MIT). See LICENSE in the repo root for license information.
 #  ------------------------------------------------------------------------------------------
 import logging
 from argparse import Namespace
 from typing import Any, Dict, Iterable, List, Optional, Union
 
-import mlflow
 from pytorch_lightning import Trainer
 from pytorch_lightning.loggers import LightningLoggerBase, MLFlowLogger
 from pytorch_lightning.utilities.logger import _convert_params, _flatten_dict
 from pytorch_lightning.utilities.rank_zero import rank_zero_only, rank_zero_warn
-
 from health_ml.utils.type_annotations import DictStrFloat, DictStrFloatOrFloatList
 
 
 class StoringLogger(LightningLoggerBase):
     """
     A Pytorch Lightning logger that simply stores the metrics that are written to it.
     Used for diagnostic purposes in unit tests.
@@ -94,15 +92,15 @@
             raise KeyError(f"No results are stored for epoch {epoch}")
         filtered = {}
         for key, value in epoch_results.items():
             assert isinstance(key, str), f"All dictionary keys should be strings, but got: {type(key)}"
             # Add the metric if either there is no prefix filter (prefix does not matter), or if the prefix
             # filter is supplied and really matches the metric name
             if (not prefix_filter) or key.startswith(prefix_filter):
-                stripped_key = key[len(prefix_filter):]
+                stripped_key = key[len(prefix_filter) :]
                 filtered[stripped_key] = value  # type: ignore
         return filtered  # type: ignore
 
     def to_metrics_dicts(self, prefix_filter: str = "") -> Dict[int, DictStrFloat]:
         """
         Converts the results stored in the present object into a two-level dictionary, mapping from epoch number to
         metric name to metric value. Only metrics where the name starts with the given prefix are retained, and the
@@ -123,33 +121,32 @@
     def log_hyperparams(self, params: Union[Dict[str, Any], Namespace]) -> None:
         """
         Override underlying log_hyperparams message to avoid trying to log hyperparameters that have already
         been logged, thus causing MLFlow to raise an Exception.
 
         :param params: The original hyperparameters to be logged.
         """
-        run = mlflow.get_run(self.run_id)
+        run = self._mlflow_client.get_run(self.run_id)
         existing_hyperparams = run.data.params
 
         params = _convert_params(params)
         params = _flatten_dict(params)
         for k, v in params.items():
             if len(str(v)) > 250:
                 rank_zero_warn(
-                    f"Mlflow only allows parameters with up to 250 characters. Discard {k}={v}",
-                    category=RuntimeWarning
+                    f"Mlflow only allows parameters with up to 250 characters. Discard {k}={v}", category=RuntimeWarning
                 )
                 continue
             if k in existing_hyperparams:
                 continue
 
             self.experiment.log_param(self.run_id, k, v)
 
 
-def get_mlflow_run_id_from_trainer(trainer: Trainer) -> Optional[str]:
+def get_mlflow_run_id_from_trainer(trainer: Optional[Trainer]) -> Optional[str]:
     """
     If trainer has already been intialised with loggers, attempt to retrieve one of the type HimlMLFlowLogger,
     and return its run_id property in order to log to the same run. Otherwise, return None.
 
     :return: The mlflow run id from an existing HimlMLFlowLogger if available, else None.
     """
     if trainer is None:
```

### Comparing `hi-ml-0.2.9/src/health_ml/utils/logging.py` & `hi-ml-0.3.0/src/health_ml/utils/logging.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 #  ------------------------------------------------------------------------------------------
 #  Copyright (c) Microsoft Corporation. All rights reserved.
 #  Licensed under the MIT License (MIT). See LICENSE in the repo root for license information.
 #  ------------------------------------------------------------------------------------------
 import argparse
+from io import TextIOWrapper
 import logging
 import math
 import numbers
 import operator
 import sys
 import time
 from datetime import datetime
@@ -33,23 +34,24 @@
     """
 
     HYPERPARAMS_NAME = "hyperparams"
     """
     The name under which hyperparameters are written to the AzureML run.
     """
 
-    def __init__(self,
-                 enable_logging_outside_azure_ml: Optional[bool] = False,
-                 experiment_name: str = "azureml_logger",
-                 run: Optional[Run] = None,
-                 run_name: Optional[str] = None,
-                 workspace: Optional[Workspace] = None,
-                 workspace_config_path: Optional[Path] = None,
-                 snapshot_directory: Optional[PathOrString] = None
-                 ) -> None:
+    def __init__(
+        self,
+        enable_logging_outside_azure_ml: Optional[bool] = False,
+        experiment_name: str = "azureml_logger",
+        run: Optional[Run] = None,
+        run_name: Optional[str] = None,
+        workspace: Optional[Workspace] = None,
+        workspace_config_path: Optional[Path] = None,
+        snapshot_directory: Optional[PathOrString] = None,
+    ) -> None:
         """
         :param enable_logging_outside_azure_ml: If True, the AzureML logger will write metrics to AzureML even if
             executed outside of an AzureML run (for example, when working on a separate virtual machine). If False,
             the logger will only write metrics to AzureML if the code is actually running inside of AzureML. Default
             False, do not log outside of AzureML.
         :param experiment_name: The AzureML experiment that should hold the run when executed outside of AzureML.
         :param run: The AzureML run to log to when the ``enable_logging_outside_azure_ml`` flag is True. If None,
@@ -73,30 +75,34 @@
             self.run = RUN_CONTEXT
         elif enable_logging_outside_azure_ml:
             if run is not None:
                 self.run = run
                 self.has_user_provided_run = True
             else:
                 try:
-                    self.run = create_aml_run_object(experiment_name=experiment_name,
-                                                     run_name=run_name,
-                                                     workspace=workspace,
-                                                     workspace_config_path=workspace_config_path,
-                                                     snapshot_directory=snapshot_directory)
+                    self.run = create_aml_run_object(
+                        experiment_name=experiment_name,
+                        run_name=run_name,
+                        workspace=workspace,
+                        workspace_config_path=workspace_config_path,
+                        snapshot_directory=snapshot_directory,
+                    )
                     # Display name should already be set when creating the run object, but this does not happen.
                     # In unit tests, the run has the expected display name, but not here. Hence, set it again.
                     self.run.display_name = run_name
                 except Exception as ex:
                     logging.error(f"Unable to create an AzureML run to store the results because of {ex}.")
                     raise
             print(f"Writing metrics to run {self.run.id} in experiment {self.run.experiment.name}.")
             print(f"To check progress, visit this URL: {self.run.get_portal_url()}")
         else:
-            print("AzureMLLogger will not write any logs because it is running outside AzureML, and the "
-                  "'enable_logging_outside_azure_ml' flag is set to False")
+            print(
+                "AzureMLLogger will not write any logs because it is running outside AzureML, and the "
+                "'enable_logging_outside_azure_ml' flag is set to False"
+            )
 
     @rank_zero_only
     def log_metrics(self, metrics: Dict[str, float], step: Optional[int] = None) -> None:
         """
         Writes the given metrics dictionary to the AzureML run context. If the metrics dictionary has an `epoch` key,
         the `step` value (x-axis for plots) is left empty. If there is no `epoch` key, the `step` value is taken
         from the function argument. This is the case for metrics that are logged with the `on_step=True` flag.
@@ -123,16 +129,17 @@
         if self.run is None:
             return
         if params is None:
             return
         params_final = _preprocess_hyperparams(params)
         if len(params_final) > 0:
             # Log hyperparameters as a table with 2 columns. Each "step" is one hyperparameter
-            self.run.log_table(self.HYPERPARAMS_NAME, {"name": list(params_final.keys()),
-                                                       "value": list(params_final.values())})
+            self.run.log_table(
+                self.HYPERPARAMS_NAME, {"name": list(params_final.keys()), "value": list(params_final.values())}
+            )
 
     def experiment(self) -> Any:
         return None
 
     def name(self) -> Any:
         return ""
 
@@ -168,32 +175,28 @@
     PROGRESS_STAGE_VAL = "Validation"
     """A string that indicates that the trainer loop is presently in validation mode."""
     PROGRESS_STAGE_TEST = "Testing"
     """A string that indicates that the trainer loop is presently in testing mode."""
     PROGRESS_STAGE_PREDICT = "Prediction"
     """A string that indicates that the trainer loop is presently in prediction mode."""
 
-    def __init__(self,
-                 refresh_rate: int = 50,
-                 print_timestamp: bool = True,
-                 write_to_logging_info: bool = False
-                 ):
+    def __init__(self, refresh_rate: int = 50, print_timestamp: bool = True, write_to_logging_info: bool = False):
         """
         :param refresh_rate: The number of steps after which the progress should be printed out.
         :param print_timestamp: If True, each message that the progress bar prints will be prefixed with the current
             time in UTC. If False, no such prefix will be added.
         :param write_to_logging_info: If True, the progress information will be printed via logging.info. If False,
             it will be printed to stdout via print.
         """
         super().__init__()
         self._refresh_rate = refresh_rate
         self._enabled = True
         self.stage = ""
         self.stage_start_time = 0.0
-        self.total_num_batches = 0.
+        self.total_num_batches = 0.0
         self.write_to_logging_info = write_to_logging_info
         self.print_timestamp = print_timestamp
 
     @property
     def refresh_rate(self) -> int:
         return self._refresh_rate
 
@@ -275,16 +278,17 @@
         """
 
         def to_minutes(time_sec: float) -> str:
             minutes = int(time_sec / 60)
             seconds = int(time_sec % 60)
             return f"{minutes:02}:{seconds:02}"
 
-        should_update = (self.is_enabled and (batches_processed % self.refresh_rate == 0
-                                              or batches_processed == self.total_num_batches))  # noqa: W503
+        should_update = self.is_enabled and (
+            batches_processed % self.refresh_rate == 0 or batches_processed == self.total_num_batches
+        )  # noqa: W503
         if not should_update:
             return
         prefix = f"{self.stage}"
         assert self.trainer is not None and self.trainer.lightning_module is not None  # for pyright
         if self.stage in [self.PROGRESS_STAGE_TRAIN, self.PROGRESS_STAGE_VAL]:
             prefix += f" epoch {self.trainer.current_epoch}"
         if self.stage == self.PROGRESS_STAGE_TRAIN:
@@ -295,17 +299,19 @@
         if math.isinf(self.total_num_batches):
             # Can't print out per-cent progress or time estimates if the data is infinite
             message = f"{prefix}{batches_processed:4} batches completed, {time_elapsed_min} since epoch start"
         else:
             fraction_completed = batches_processed / self.total_num_batches
             percent_completed = int(fraction_completed * 100)
             estimated_epoch_duration = time_elapsed / fraction_completed
-            message = (f"{prefix}{batches_processed:4}/{self.total_num_batches} ({percent_completed:3}%) completed. "
-                       f"{time_elapsed_min} since epoch start, estimated total epoch time ~ "
-                       f"{to_minutes(estimated_epoch_duration)}")
+            message = (
+                f"{prefix}{batches_processed:4}/{self.total_num_batches} ({percent_completed:3}%) completed. "
+                f"{time_elapsed_min} since epoch start, estimated total epoch time ~ "
+                f"{to_minutes(estimated_epoch_duration)}"
+            )
         self._print(message)
 
     def _print(self, message: str) -> None:
         if self.print_timestamp:
             timestamp = datetime.utcnow().strftime("%Y-%m-%dT%H%M%SZ ")
             message = timestamp + message
         if self.write_to_logging_info:
@@ -330,20 +336,22 @@
     # Convert anything that is not a primitive type to str
     params_final = _sanitize_params(params)
     if not isinstance(params_final, dict):
         raise ValueError(f"Expected the converted hyperparameters to be a dictionary, but got {type(params)}")
     return {str(key): str(value) for key, value in params_final.items()}
 
 
-def log_on_epoch(module: LightningModule,
-                 name: Optional[str] = None,
-                 value: Optional[Any] = None,
-                 metrics: Optional[Mapping[str, Any]] = None,
-                 reduce_fx: Callable = torch.mean,
-                 sync_dist: Optional[bool] = None) -> None:
+def log_on_epoch(
+    module: LightningModule,
+    name: Optional[str] = None,
+    value: Optional[Any] = None,
+    metrics: Optional[Mapping[str, Any]] = None,
+    reduce_fx: Callable = torch.mean,
+    sync_dist: Optional[bool] = None,
+) -> None:
     """
     Write a dictionary with metrics and/or an individual metric as a name/value pair to the loggers of the given module.
     Metrics are always logged upon epoch completion.
     The metrics in question first synchronized across GPUs if DDP with >1 node is used,. Afterwards, they are
     aggregated across all steps via the reduce_fx (default: mean).
     Metrics that are fed in as plain numbers rather than tensors (for example, plain Python integers) are converted
     to tensors before logging, to enable synchronization across GPUs if needed.
@@ -367,19 +375,15 @@
         metrics[name] = value  # type: ignore
     metrics_as_tensors = {
         key: torch.tensor(value, dtype=torch.float, device=module.device)
         if isinstance(value, numbers.Number)
         else value
         for key, value in metrics.items()
     }
-    module.log_dict(metrics_as_tensors,
-                    on_epoch=True,
-                    on_step=False,
-                    sync_dist=is_sync_dist,
-                    reduce_fx=reduce_fx)
+    module.log_dict(metrics_as_tensors, on_epoch=True, on_step=False, sync_dist=is_sync_dist, reduce_fx=reduce_fx)
 
 
 def log_learning_rate(module: LightningModule, name: str = "learning_rate") -> None:
     """
     Logs the learning rate(s) used by the given module. Multiple learning rate schedulers and/or multiple rates per
     scheduler are supported. The learning rates are logged under the given name. If multiple scheduler and/or multiple
     rates are used, a suffix like "/0/1" is added, to indicate the learning rate for scheduler 0, index 1, for example.
@@ -398,7 +402,43 @@
     singleton_lr = single_scheduler and len(lr_0) == 1
     logged = {}
     for i, scheduler in enumerate(schedulers):  # type: ignore
         for j, lr_j in enumerate(scheduler.get_last_lr()):  # type: ignore
             full_name = name if singleton_lr else f"{name}/{i}/{j}"
             logged[full_name] = lr_j
     log_on_epoch(module, metrics=logged)
+
+
+class ConsoleAndFileOutput(TextIOWrapper):
+    """A file-like object that writes to both the console (sys.stdout) and an output file.
+    The caller needs to ensure that the file is closed properly after using this object.
+
+    :param TextIOWrapper: The file to write to.
+    """
+
+    def __init__(self, file: TextIOWrapper) -> None:
+        self.file = file
+        self.sys_stdout = sys.stdout
+
+    def write(self, __buffer: Any) -> int:
+        """Writes the buffer to both the file and to the console.
+
+        :param __buffer: The buffer to write.
+        :return: The number of bytes written to the console
+        """
+        self.file.write(__buffer)
+        return self.sys_stdout.write(__buffer)
+
+    def flush(self) -> None:
+        """Flush both the output file and the console."""
+        self.file.flush()
+        self.sys_stdout.flush()
+
+    def isatty(self) -> bool:
+        """Returns if the given file is a terminal. Since the class is writing to a file, this always returns False."""
+        return False
+
+    def read(self, size: int = -1) -> str:  # type: ignore
+        raise NotImplementedError("Read is not supported")
+
+    def readline(self, size: int = -1) -> str:  # type: ignore
+        raise NotImplementedError("Readline is not supported")
```

### Comparing `hi-ml-0.2.9/src/health_ml/utils/lr_scheduler.py` & `hi-ml-0.3.0/src/health_ml/utils/lr_scheduler.py`

 * *Files 6% similar despite different names*

```diff
@@ -48,15 +48,15 @@
         self.gamma = gamma
         self.l_rate = l_rate
         self.min_l_rate = min_l_rate
         self.epochs_after_warmup = epochs_after_warmup
 
     def get_lr(self, epoch: int) -> float:
         x = self.min_l_rate / self.l_rate
-        return (1 - x) * ((1. - float(epoch) / self.epochs_after_warmup) ** self.gamma) + x
+        return (1 - x) * ((1.0 - float(epoch) / self.epochs_after_warmup) ** self.gamma) + x
 
 
 class SchedulerWithWarmUp(_LRScheduler):
     """
     LR Scheduler which runs a warmup schedule (linear ramp-up) for a few iterations, and then switches to one
     of the normal schedulers.
     """
@@ -65,69 +65,74 @@
         self.optimizer = optimizer
         self.last_epoch = last_epoch
         self.num_epochs = num_epochs
         self.warmup_epochs = 0 if args.l_rate_warmup == LRWarmUpType.NoWarmUp else args.l_rate_warmup_epochs
         self._scheduler = self.get_scheduler(args)
         # This must be called after self.get_scheduler, because we want the optimizer to have the learning rate
         # guided by the warmup schedule
-        self._warmup = LinearWarmUp(optimizer,
-                                    warmup_epochs=self.warmup_epochs,
-                                    final_lr=args.l_rate,
-                                    last_epoch=last_epoch)
+        self._warmup = LinearWarmUp(
+            optimizer, warmup_epochs=self.warmup_epochs, final_lr=args.l_rate, last_epoch=last_epoch
+        )
         self._last_lr = get_current_learning_rates(optimizer)
         self.min_l_rate = args.min_l_rate
         super().__init__(optimizer, last_epoch)
 
     def get_scheduler(self, args: OptimizerParams) -> _LRScheduler:
         """
         Create the LR scheduler that will be used after warmup, based on the config params.
         """
         scheduler: _LRScheduler
         epochs_after_warmup = self.num_epochs - self.warmup_epochs
         if args.l_rate_scheduler == LRSchedulerType.Exponential:
-            scheduler = ExponentialLR(optimizer=self.optimizer,
-                                      gamma=args.l_rate_exponential_gamma,
-                                      last_epoch=self.last_epoch)
+            scheduler = ExponentialLR(
+                optimizer=self.optimizer, gamma=args.l_rate_exponential_gamma, last_epoch=self.last_epoch
+            )
         elif args.l_rate_scheduler == LRSchedulerType.Step:
-            scheduler = StepLR(optimizer=self.optimizer,
-                               step_size=args.l_rate_step_step_size,
-                               gamma=args.l_rate_step_gamma,
-                               last_epoch=self.last_epoch)
+            scheduler = StepLR(
+                optimizer=self.optimizer,
+                step_size=args.l_rate_step_step_size,
+                gamma=args.l_rate_step_gamma,
+                last_epoch=self.last_epoch,
+            )
         elif args.l_rate_scheduler == LRSchedulerType.MultiStep:
             assert args.l_rate_multi_step_milestones is not None
-            scheduler = MultiStepLR(optimizer=self.optimizer,
-                                    milestones=args.l_rate_multi_step_milestones,
-                                    gamma=args.l_rate_multi_step_gamma,
-                                    last_epoch=self.last_epoch)
+            scheduler = MultiStepLR(
+                optimizer=self.optimizer,
+                milestones=args.l_rate_multi_step_milestones,
+                gamma=args.l_rate_multi_step_gamma,
+                last_epoch=self.last_epoch,
+            )
         elif args.l_rate_scheduler == LRSchedulerType.Polynomial:
-            polynomial_lr = PolynomialLR(gamma=args.l_rate_polynomial_gamma,
-                                         l_rate=args.l_rate,
-                                         min_l_rate=args.min_l_rate,
-                                         epochs_after_warmup=epochs_after_warmup)
-            scheduler = LambdaLR(optimizer=self.optimizer,
-                                 lr_lambda=polynomial_lr.get_lr,
-                                 last_epoch=self.last_epoch)
+            polynomial_lr = PolynomialLR(
+                gamma=args.l_rate_polynomial_gamma,
+                l_rate=args.l_rate,
+                min_l_rate=args.min_l_rate,
+                epochs_after_warmup=epochs_after_warmup,
+            )
+            scheduler = LambdaLR(optimizer=self.optimizer, lr_lambda=polynomial_lr.get_lr, last_epoch=self.last_epoch)
         elif args.l_rate_scheduler == LRSchedulerType.Cosine:
-            scheduler = CosineAnnealingLR(optimizer=self.optimizer,
-                                          T_max=epochs_after_warmup,
-                                          eta_min=args.min_l_rate,
-                                          last_epoch=self.last_epoch)
+            scheduler = CosineAnnealingLR(
+                optimizer=self.optimizer, T_max=epochs_after_warmup, eta_min=args.min_l_rate, last_epoch=self.last_epoch
+            )
         else:
             raise ValueError("Unknown learning rate scheduler {}".format(args.l_rate_scheduler))
         return scheduler
 
     def state_dict(self) -> Dict:
         """
         Returns a dictionary with all the values in this objects __dict__.
         It creates the dictionary entry for variables "_scheduler" and "_warmup_scheduler" separately, by calling
         state_dict for these variables.
         The state dict does not include the state of the optimizer.
         """
-        state_dict = {key: val for key, val in self.__dict__.items()
-                      if key != "_scheduler" and key != "optimizer" and key != "_warmup"}
+        state_dict = {
+            key: val
+            for key, val in self.__dict__.items()
+            if key != "_scheduler" and key != "optimizer" and key != "_warmup"
+        }
 
         state_dict['_scheduler'] = self._scheduler.state_dict()
         state_dict['_warmup'] = self._warmup.state_dict()
         return state_dict
 
     def load_state_dict(self, state_dict: Dict) -> None:
         """
```

### Comparing `hi-ml-0.2.9/src/health_ml/utils/model_util.py` & `hi-ml-0.3.0/src/health_ml/utils/model_util.py`

 * *Files 18% similar despite different names*

```diff
@@ -10,27 +10,23 @@
 
 from health_ml.deep_learning_config import OptimizerParams, OptimizerType
 
 
 def create_optimizer(config: OptimizerParams, parameters: Iterator[Parameter]) -> Optimizer:
     # Select optimizer type
     if config.optimizer_type in [OptimizerType.Adam, OptimizerType.AMSGrad]:
-        return Adam(parameters,
-                    config.l_rate,
-                    config.adam_betas,
-                    config.opt_eps,
-                    config.weight_decay,
-                    amsgrad=config.optimizer_type == OptimizerType.AMSGrad)
+        return Adam(
+            parameters,
+            config.l_rate,
+            config.adam_betas,
+            config.opt_eps,
+            config.weight_decay,
+            amsgrad=config.optimizer_type == OptimizerType.AMSGrad,
+        )
     elif config.optimizer_type == OptimizerType.SGD:
-        return SGD(parameters,
-                   config.l_rate,
-                   config.momentum,
-                   weight_decay=config.weight_decay)
+        return SGD(parameters, config.l_rate, config.momentum, weight_decay=config.weight_decay)
     elif config.optimizer_type == OptimizerType.RMSprop:
-        return RMSprop(parameters,
-                       config.l_rate,
-                       config.rms_alpha,
-                       config.opt_eps,
-                       config.weight_decay,
-                       config.momentum)
+        return RMSprop(
+            parameters, config.l_rate, config.rms_alpha, config.opt_eps, config.weight_decay, config.momentum
+        )
     else:
         raise NotImplementedError(f"Optimizer type {config.optimizer_type.value} is not implemented")
```

### Comparing `hi-ml-0.2.9/src/health_ml/utils/regression_test_utils.py` & `hi-ml-0.3.0/src/health_ml/utils/regression_test_utils.py`

 * *Files 24% similar despite different names*

```diff
@@ -32,24 +32,22 @@
     """
     Function to give more clarity on the difference between two dictionaries.
 
     :param expected: The first dictionary to compare
     :param actual: The second dictionary to compare
     :param tolerance: The tolerance to allow when comparing numeric values, defaults to 1e-5
     """
+
     def _check_values_match(expected_v: Any, actual_v: Any, tolerance: float = 1e-5) -> None:
         if type(actual_v) in [float, int] and type(expected_v) in [float, int]:
             if not isclose(actual_v, expected_v, rel_tol=tolerance):
-                raise ValueError(f"Expected: {expected_v} does not match actual {actual_v}")
-            else:
-                return
+                logging.warning(f"Expected: {expected_v} does not match actual {actual_v}")
         else:
             if expected_v != actual_v:
-                raise ValueError(f"Expected: {expected_v} does not match actual {actual_v}")
-        return
+                logging.warning(f"Expected: {expected_v} does not match actual {actual_v}")
 
     for expected_key, expected_val in expected.items():
         if expected_key not in actual:
             logging.warning(f"Key {expected_key} is expected but not found in actual dictionary: {actual}")
         else:
             actual_val = actual[expected_key]
             expected_type = type(expected_val)
@@ -65,14 +63,182 @@
                 actual_len = len(actual_val)
                 if expected_len != actual_len:
                     logging.warning(f"Expected value to have length {expected_len} but found {actual_len}")
                 for expected_value, actual_value in zip(expected_val, actual_val):
                     _check_values_match(expected_value, actual_value, tolerance=tolerance)
 
 
+def _compare_metric_values(expected: Any, actual: Any, tolerance: float = 1e-5) -> str:
+    """Compares an expected and an actual value coming from a metrics dictionary. If the values are numeric
+    and are close enough (within the given tolerance), an empty string is returned. If the actual
+    and expected value are not matching, a string description of the discrepancy will be returned.
+
+    :param expected: The expected value
+    :param actual: The actual value
+    :param tolerance: For numerical values, this is the relative tolerance allowed, defaults to 1e-5
+    :return: An empty string if the expected and actual values match, otherwise a string describing the discrepancy.
+    """
+    if type(expected) in [float, int]:
+        if type(actual) in [float, int]:
+            if isclose(actual, expected, rel_tol=tolerance):
+                return ""
+            return f"Expected {expected} but got {actual} (allowed tolerance {tolerance})"
+        return f"Expected a numeric value, but got type {type(actual).__name__}"
+    return f"Don't know how to handle expected value of type {type(expected).__name__}"
+
+
+def _compare_metrics_list(expected: List, actual: List, tolerance: float = 1e-5) -> List[str]:
+    """Compares two lists of expected and actual values, coming from a metrics dictionary. The two lists are
+    considered matching if they have the same length, and matching list elements are within the given relative
+    tolerance.
+
+    :param expected: A list of expected values.
+    :param actual: A list with actual metric values.
+    :param tolerance: For numerical values, this is the relative tolerance allowed, defaults to 1e-5
+    :return: A list of strings describing the discrepancies between the two lists. If the lists match, the
+        return value is an empty list.
+    """
+    messages = []
+    expected_len = len(expected)
+    actual_len = len(actual)
+    if expected_len == actual_len:
+        for index, (expected_value, actual_value) in enumerate(zip(expected, actual)):
+            mismatch = _compare_metric_values(expected_value, actual_value, tolerance=tolerance)
+            if mismatch:
+                messages.append(f"Index {index}: {mismatch}")
+    else:
+        messages.append(f"Expected list of length {expected_len} but got {actual_len}")
+    return messages
+
+
+def compare_metrics_dictionaries(expected: Dict[str, Any], actual: Dict[str, Any], tolerance: float = 1e-5) -> str:
+    """
+    Function to compare two dictionaries that are expected to contain metrics (scalars or lists of scalars) or strings.
+    Discrepancies are logged via logging.warning. The function returns an empty string if the dictionaries are
+    identical, otherwise a string giving a short summary of the discrepancies.
+
+    :param expected: The first dictionary to compare
+    :param actual: The second dictionary to compare
+    :param tolerance: The tolerance to allow when comparing numeric values, defaults to 1e-5.
+    :return: An empty string if the dictionaries match, otherwise a string describing the discrepancies.
+    """
+
+    allowed_types = [float, int, str, list]
+    discrepancies = 0
+    for key, expected_val in expected.items():
+        messages = []
+        expected_type = type(expected_val)
+        if expected_type not in allowed_types:
+            raise ValueError(f"Expected value has type {expected_type.__name__} which is not handled.")
+        if key not in actual:
+            messages.append("No data found in actual metrics.")
+        else:
+            actual_val = actual[key]
+            actual_type = type(actual_val)
+            if actual_type not in allowed_types:
+                messages.append(f"Actual value has type {actual_type.__name__} which is not handled.")
+            elif expected_type is not actual_type:
+                messages.append(
+                    f"Actual value has type {actual_type.__name__} but we expected " f"{expected_type.__name__}."
+                )
+            elif expected_type is list:
+                messages.extend(_compare_metrics_list(expected_val, actual_val, tolerance=tolerance))
+            else:
+                mismatch = _compare_metric_values(expected_val, actual_val, tolerance=tolerance)
+                if mismatch:
+                    messages.append(mismatch)
+        for message in messages[:5]:
+            logging.warning(f"Metric '{key}': {message}")
+        if len(messages) > 0:
+            discrepancies += 1
+    return f"Mismatch for {discrepancies} out of {len(expected)} metrics" if discrepancies > 0 else ""
+
+
+def _load_json_dict(path: Path) -> Dict[str, Any]:
+    """Loads the contents of a JSON file. If the contents is a dictionary, this dictionary is returned.
+
+    :param path: The file to load.
+    :raises ValueError: If the file does not contain a JSON dictionary.
+    :return: The contents of the JSON file.
+    """
+    metrics_json = json.loads(path.read_text())
+    if not isinstance(metrics_json, Dict):
+        raise ValueError(
+            f"Expected metrics file {path} to contain a JSON dictionary, but got {type(metrics_json).__name__}"
+        )
+    return metrics_json
+
+
+def _is_nested_dict(d: Dict[str, Any], message: str) -> bool:
+    """Checks if a dictionary contains only dictionaries as values. Returns `True` if the dictionary contains
+    only dictionaries as values. Returns `False` if none of the dictionary values are dictionaries, or if the
+    dictionary is empty.
+    Raises an exception if the dictionary contains a mix of dictionaries and non-dictionaries.
+
+    :param d: The dictionary to check.
+    :param message: A message to include in the exception if the dictionary contains a mix of dictionaries.
+    :raises ValueError: If the dictionary contains a mix of dictionaries and non-dictionaries.
+    :return: True if the dictionary contains values, and all those are dictionaries in turn. False otherwise.
+    """
+    has_dict_value = [isinstance(v, Dict) for v in d.values()]
+    if len(d) == 0:
+        return False
+    if all(has_dict_value):
+        return True
+    if any(has_dict_value):
+        raise ValueError(
+            f"{message}: Metrics file has inconsistent type. Either all or none of the dictionary"
+            "values should be dictionaries"
+        )
+    return False
+
+
+def compare_metrics_files(expected: Path, actual: Path, tolerance: float = 1e-5) -> str:
+    """Reads two files that contain a JSON representation of expected and actual metrics. The two files are read
+    and the metrics are compared using compare_metrics_dictionaries. The function returns an empty string if the
+    metrics match, otherwise a string summarizing the discrepancies. Details about the discrepancies are logged
+    to `logging.warning`.
+
+    :param expected: A file that contains the expected metrics, as a JSON dictionary.
+    :param actual: A file that contains the actual metrics, as a JSON dictionary.
+    :param tolerance: The maximum allowed tolerance for comparing metrics, defaults to 1e-5
+    :return: An empty string if the metrics match, otherwise a string summarizing the discrepancies.
+    """
+    try:
+        expected_metrics = _load_json_dict(expected)
+        actual_metrics = _load_json_dict(actual)
+        if _is_nested_dict(expected_metrics, "Expected metrics"):
+            # For runs with child runs, loop over the child run dictionaries and compare them.
+            if not _is_nested_dict(actual_metrics, "Actual metrics"):
+                return "Expected a nested dictionary as the actual metrics, but got a flat dictionary"
+            messages = []
+            for key, expected_child in expected_metrics.items():
+                prefix = f"Child run '{key}'"
+                if key in actual_metrics:
+                    actual_child = actual_metrics[key]
+                    message = compare_metrics_dictionaries(expected_child, actual_child, tolerance=tolerance)
+                else:
+                    message = "Missing from the actual metrics"
+                if message:
+                    full_message = f"{prefix}: {message}"
+                    logging.warning(full_message)
+                    messages.append(message)
+            if len(messages) > 0:
+                return f"Mismatches for {len(messages)} child runs"
+            return ""
+        else:
+            # For simple runs without child runs: Compare the dictionaries.
+            if _is_nested_dict(actual_metrics, "Actual metrics"):
+                return "Expected a flat dictionary as the actual metrics, but got a nested dictionary"
+            return compare_metrics_dictionaries(expected_metrics, actual_metrics, tolerance=tolerance)
+    except Exception as e:
+        # This handles cases where the files cannot be found, are not JSON, or have inconsistent information.
+        return f"Error comparing metrics files: {e}"
+
+
 def compare_files(expected: Path, actual: Path, csv_relative_tolerance: float = 0.0) -> str:
     """
     Compares two individual files for regression testing. It returns an empty string if the two files appear identical.
     If the files are not identical, a brief error message is returned. Details about the mismatch are logged via
     logging.warning. This method handles CSV files (which are treated and compared as dataframes) and text files (TXT,
     JSON, HTML, MD, which are all compared while ignoring linebreaks. All other extensions are treated as binary,
     and compared on a byte-by-byte basis.
@@ -81,14 +247,15 @@
     based on the extension of this file.
     :param actual: A file to be checked against the expected file.
     :param csv_relative_tolerance: When comparing CSV files, maximum allowed relative discrepancy.
     If 0.0, do not allow any discrepancy.
     :return: An empty string if the files appear identical, or otherwise a brief error message. If there is a
     mismatch, details about the mismatch are printed via logging.warning.
     """
+
     def print_lines(prefix: str, lines: List[str]) -> None:
         num_lines = len(lines)
         count = min(5, num_lines)
         logging.warning(f"{prefix} {num_lines} lines, first {count} of those:")
         logging.warning(os.linesep.join(lines[:count]))
 
     def try_read_csv(prefix: str, file: Path) -> Optional[pd.DataFrame]:
@@ -119,15 +286,15 @@
             print_lines("Expected", expected_lines)
             print_lines("Actual", actual_lines)
             # Add additional context for json file mismatches
             if expected.suffix == ".json":
                 compare_dictionaries(
                     _load_json_from_text_lines(expected_lines),
                     _load_json_from_text_lines(actual_lines),
-                    tolerance=csv_relative_tolerance
+                    tolerance=csv_relative_tolerance,
                 )
             return CONTENTS_MISMATCH
     else:
         expected_binary = expected.read_bytes()
         actual_binary = actual.read_bytes()
         if expected_binary != actual_binary:
             logging.warning(f"Expected {len(expected_binary)} bytes, actual {len(actual_binary)} bytes")
@@ -175,16 +342,20 @@
             actual_file = actual_folder / file_relative
         elif temp_folder is not None and run is not None:
             actual_file = temp_folder / file_relative
             if file_relative in files_in_run:
                 run.download_file(name=str(file_relative), output_file_path=str(actual_file))
         else:
             raise ValueError("Either of the two arguments 'run' or 'actual_folder' must be provided")
-        message = compare_files(expected=file, actual=actual_file,
-                                csv_relative_tolerance=csv_relative_tolerance) if actual_file.exists() else MISSING_FILE
+        if file_relative == REGRESSION_TEST_METRICS_FILENAME:
+            message = compare_metrics_files(expected=file, actual=actual_file, tolerance=csv_relative_tolerance)
+        elif actual_file.exists():
+            message = compare_files(expected=file, actual=actual_file, csv_relative_tolerance=csv_relative_tolerance)
+        else:
+            message = MISSING_FILE
         if message:
             messages.append(f"{message}: {file_relative}")
             logging.warning(f"File {file_relative}: {message}")
         else:
             logging.info(f"File {file_relative}: OK")
     if temp_folder:
         shutil.rmtree(temp_folder)
@@ -207,28 +378,29 @@
     if not expected.is_dir():
         raise ValueError(f"Folder with expected files does not exist: {expected}")
     logging.debug(f"Current working directory: {Path.cwd()}")
     messages = []
     folders_to_check = [
         (REGRESSION_TEST_OUTPUT_FOLDER, "run output files", actual, None),
         (REGRESSION_TEST_AZUREML_FOLDER, "AzureML outputs in present run", None, RUN_CONTEXT),
-        (REGRESSION_TEST_AZUREML_PARENT_FOLDER, "AzureML outputs in parent run", None, PARENT_RUN_CONTEXT)
+        (REGRESSION_TEST_AZUREML_PARENT_FOLDER, "AzureML outputs in parent run", None, PARENT_RUN_CONTEXT),
     ]
-    for (subfolder, message_prefix, actual_folder, run_to_compare) in folders_to_check:
+    for subfolder, message_prefix, actual_folder, run_to_compare in folders_to_check:
         folder = expected / subfolder
         if folder.is_dir():
             logging.info(f"Comparing results in {folder} against {message_prefix}:")
             if actual_folder is None and run_to_compare is None:
                 logging.info("No AzureML run to compare against. Skipping")
                 continue
-            new_messages = compare_folder_contents(folder,
-                                                   actual_folder=actual_folder,
-                                                   run=run_to_compare,
-                                                   csv_relative_tolerance=csv_relative_tolerance)
+            new_messages = compare_folder_contents(
+                folder, actual_folder=actual_folder, run=run_to_compare, csv_relative_tolerance=csv_relative_tolerance
+            )
             if new_messages:
                 messages.append(f"Issues in {message_prefix}:")
                 messages.extend(new_messages)
         else:
             logging.info(f"Folder {subfolder} not found, skipping comparison against {message_prefix}")
     if messages:
-        raise ValueError(f"Some expected files were missing or did not have the expected contents:{os.linesep}"
-                         f"{os.linesep.join(messages)}")
+        raise ValueError(
+            f"Some expected files were missing or did not have the expected contents:{os.linesep}"
+            f"{os.linesep.join(messages)}"
+        )
```

### Comparing `hi-ml-0.2.9/src/health_ml/utils/reports.py` & `hi-ml-0.3.0/src/health_ml/utils/reports.py`

 * *Files 1% similar despite different names*

```diff
@@ -14,16 +14,19 @@
 
 import jinja2
 import ruamel.yaml
 import matplotlib.pyplot as plt
 import numpy as np
 import pandas as pd
 
-from health_azure.utils import (download_files_from_run_id, get_aml_run_from_run_id,
-                                download_files_from_hyperdrive_children)
+from health_azure.utils import (
+    download_files_from_run_id,
+    get_aml_run_from_run_id,
+    download_files_from_hyperdrive_children,
+)
 
 CLOSE_DOC_TAGS = "</p>\n</div>\n</body>\n</html>"
 IMAGE_KEY_HTML = "IMAGEPATHSHTML"
 TABLE_KEY_HTML = "TABLEKEYHTML"
 REPORT_CONTENTS_KEY = "report_contents"
 DEFAULT_OUTPUTS_FOLDER = "outputs"
 DEFAULT_FIGSIZE = (15, 15)
@@ -54,17 +57,15 @@
 
         self.report_folder = report_folder
         self.report_path_html = (report_folder / title.lower().replace(" ", "_")).with_suffix('.html')
         self.report_html = ""
         self.template = ""
         self.template_path = self._create_template()
 
-        self.env = jinja2.Environment(
-            loader=jinja2.FileSystemLoader('/')
-        )
+        self.env = jinja2.Environment(loader=jinja2.FileSystemLoader('/'))
         self.render_kwargs: Dict[str, Any] = {"title": title}
 
     def validate(self) -> None:
         """
         For our definition, the rendered HTML must contain exactly one open and closing tags doctype, head and body
         If any of these are missing from the repport_html, we raise a ValueError
 
@@ -75,16 +76,17 @@
         if len(self.report_html) == 0:
             self.render(save_html=False)
         expected_tags = ["<!DOCTYPE html>", "<head>", "</head>", "<body>", "</body>", "</html>"]
         for tag in expected_tags:
             if self.report_html.count(tag) < 1:
                 raise ValueError(f"report_html is missing the tag {tag}. This will cause problems with rendering")
             elif self.report_html.count(tag) > 1:
-                raise ValueError(f"report_html contains more than one tag {tag}. This will cause problems with"
-                                 "rendering")
+                raise ValueError(
+                    f"report_html contains more than one tag {tag}. This will cause problems with rendering"
+                )
 
     @staticmethod
     def _remove_html_end(report_stream: str) -> str:
         """
         Before adding additional components to the HTML report, we must remove the closing tags
 
         :param report_stream: A string representing the content of the report thus far
@@ -102,28 +104,31 @@
         self.template += f"{CLOSE_DOC_TAGS}"
         self.validate()
 
     def _create_template(self) -> Path:
         template_path = self.report_folder / "template.html"
         template_path.touch(exist_ok=True)
 
-        self.template += """<!DOCTYPE html>
+        self.template += (
+            """<!DOCTYPE html>
 <html lang="en">
 <head>
 <meta charset="UTF-8">
 <link href="https://cdn.jsdelivr.net/npm/bootstrap@5.1.3/dist/css/bootstrap.min.css" rel="stylesheet">
 <title> {{title}} </title>
 </head>
 <body>
 <div class="container-fluid">
 <div class="container">
 <h1> {{title}} </h1>
 </div>
 <p>
-""" + CLOSE_DOC_TAGS
+"""
+            + CLOSE_DOC_TAGS
+        )
 
         return template_path
 
     def add_to_template(self, template_addition: str) -> None:
         """
         Performs the three necessary tasks to add a section to the template. Firstly, removes existing closing
         tags. Next, adds the content (passed as a string to this method). Finally, adds back the closing tags.
@@ -174,26 +179,31 @@
 
         :param tables: A list of one or more Pandas DataFrame to be rendered in the report
         """
         for table in tables:
             num_existing_tables = self.template.count("table.to_html")
             table_key = f"{TABLE_KEY_HTML}_{num_existing_tables}"  # starts at zero
 
-            template_addition = """<div class="container" >
-            {% for table in """ + table_key + """ %}
+            template_addition = (
+                """<div class="container" >
+            {% for table in """
+                + table_key
+                + """ %}
                 {{ table.to_html(classes=[ "table"], justify="center") | safe }}
             {% endfor %}
             </div>
             <br>"""
+            )
             self.add_to_template(template_addition)
 
             self.render_kwargs.update({table_key: [table]})
 
-    def add_tables(self, tables: Optional[List[pd.DataFrame]] = None,
-                   table_paths_or_dir: Optional[List[Path]] = None) -> None:
+    def add_tables(
+        self, tables: Optional[List[pd.DataFrame]] = None, table_paths_or_dir: Optional[List[Path]] = None
+    ) -> None:
         """
         Add one or more tables to your report. The table can either be passed as a Pandas DataFrame object, or
         a list of path to one or more .csv files, or a directory of csv files containing your tables.
         If neither of these parameters are provided, an Exception will be raised.
 
         :param tables: An optional list of one or more Pandas DataFrames to be rendered in the report
         :param table_paths_or_dir: An optional list of one or more paths to .csv files containing the tables
@@ -233,20 +243,24 @@
 
         image_key_html = IMAGE_KEY_HTML + "_0"
         # Increment the image name so as not to replace other images
         num_existing_images = self.template.count("<img src=")
 
         image_key_html = image_key_html.split("_")[0] + f"_{num_existing_images}"
 
-        template_addition = """<div class="container">
-        {% for image_path in """ + image_key_html + """ %}
+        template_addition = (
+            """<div class="container">
+        {% for image_path in """
+            + image_key_html
+            + """ %}
             <img src={{image_path}} alt={{image_path}}>
         {% endfor %}
         </div>
         <br>"""
+        )
         self.add_to_template(template_addition)
 
         # Add these keys and paths to the keyword args for rendering later
         if base64_encode:
             with open(image_path, "rb") as f_path:
                 img_data = f_path.read()
                 img_data_base64_bytes = base64.b64encode(img_data)
@@ -276,16 +290,17 @@
             if image_path_or_dir.is_dir():
                 for image_path in image_path_or_dir.iterdir():
                     self.add_images([image_path], base64_encode=base64_encode)
             else:
                 self._add_image_to_report(image_path_or_dir, base64_encode=base64_encode)
 
     @classmethod
-    def load_imgs_onto_subplot(cls, img_folder_or_paths: List[Path], num_plot_columns: int = 2,
-                               figsize: Tuple[int, int] = DEFAULT_FIGSIZE) -> plt.Figure:
+    def load_imgs_onto_subplot(
+        cls, img_folder_or_paths: List[Path], num_plot_columns: int = 2, figsize: Tuple[int, int] = DEFAULT_FIGSIZE
+    ) -> plt.Figure:
         """
         Given a list of one or more paths, either to a folder containing multiple images, or multiple image
         paths, loads each of the images adds to a single chart
 
         :param img_folder_or_paths: A list containing either a single path to a folder containing all of the images to
             add to the gallery, or multiple paths to specific image files
         :param num_plot_columns: The number of columns of images to plot, defaults to 2
@@ -319,16 +334,21 @@
                 axs: plt.Axes = fig.add_subplot(num_plot_rows, num_plot_columns, plot_index + 1)
                 axs.set_axis_off()
                 plt.imshow(img_arr)
 
         plt.tight_layout()
         return fig
 
-    def add_image_gallery(self, image_folder_or_paths: List[Path], figsize: Tuple[int, int] = DEFAULT_FIGSIZE,
-                          num_cols: int = DEFAULT_NUM_COLS, base64_encode: bool = False) -> None:
+    def add_image_gallery(
+        self,
+        image_folder_or_paths: List[Path],
+        figsize: Tuple[int, int] = DEFAULT_FIGSIZE,
+        num_cols: int = DEFAULT_NUM_COLS,
+        base64_encode: bool = False,
+    ) -> None:
         """
         Given a list of one or more paths, either to a folder containing multiple images, or multiple image
         paths, loads each of the images adds to a single chart create a "gallery" i.e. a plot containing
         all of these images, and add it to the report
 
         :param image_folder_or_paths: A list containing either a single path to a folder containing all of the images
             to add to the gallery, or multiple paths to specific image files
@@ -338,16 +358,17 @@
         """
         fig = self.load_imgs_onto_subplot(image_folder_or_paths, figsize=figsize, num_plot_columns=num_cols)
         img_num = len(list(self.report_folder.glob("gallery_image_*")))
         gallery_img_path = self.report_folder / f"gallery_image_{img_num}.png"
         fig.savefig(str(gallery_img_path))
         self.add_images([gallery_img_path], base64_encode=base64_encode)
 
-    def add_plot(self, plot_path: Optional[Path] = None, fig: Optional[plt.Figure] = None,
-                 fig_title: Optional[str] = None) -> None:
+    def add_plot(
+        self, plot_path: Optional[Path] = None, fig: Optional[plt.Figure] = None, fig_title: Optional[str] = None
+    ) -> None:
         """
         Add a plot to your report. The plot can either be passed as a [matplotlib Figure object](
         https://matplotlib.org/stable/api/_as_gen/matplotlib.pyplot.figure.html), or as a path to
         a saved plot file.
 
         :param plot_path: Optional path to a saved plot file
         :param fig: Optional matplotlib Figure object
@@ -433,16 +454,17 @@
             elif component_type == ReportComponentKey.IMAGE_GALLERY.value:
                 self.add_image_gallery(dir_or_paths, figsize=figsize, num_cols=num_cols, base64_encode=base64_encode)
             elif component_type == ReportComponentKey.TEXT.value:
                 self.add_text(component_val)
             else:
                 raise ValueError("Key must either equal table, image or text")
 
-    def download_report_contents_from_aml(self, run_id: str, report_contents: List[Dict[str, Any]],
-                                          hyperdrive_hyperparam_name: str = '') -> List[Dict[str, Any]]:
+    def download_report_contents_from_aml(
+        self, run_id: str, report_contents: List[Dict[str, Any]], hyperdrive_hyperparam_name: str = ''
+    ) -> List[Dict[str, Any]]:
         """
         Downloads report contents (images, csv files etc, as specified in the ) from Azure ML Runs. If the
         run_id provided represents an AML HyperDrive run, will attempt to download each of the specified paths
         in report_contents from each of the child runs. These will be saved into separate folders in the
         report folder, and the return value will include a comma separated string of the paths to each
         downloaded file. Note that to retrieve these runs, you must provide a value for `hyperdrive_hyperparam_name`
         - i.e. the name of a hyperparameter that was sampled over during this run.
@@ -465,31 +487,34 @@
 
         updated_report_contents = []
         for component in report_contents:
             component_type = component[ReportComponentKey.TYPE.value]
             component_val = component[ReportComponentKey.VALUE.value]
             # If the component is text, we don't need to download anything
             if component_type == ReportComponentKey.TEXT.value:
-                updated_report_contents.append({ReportComponentKey.TYPE.value: component_type,
-                                                ReportComponentKey.VALUE.value: component_val})
+                updated_report_contents.append(
+                    {ReportComponentKey.TYPE.value: component_type, ReportComponentKey.VALUE.value: component_val}
+                )
             else:
                 if run.type == "hyperdrive":
                     artifact_paths = download_files_from_hyperdrive_children(
                         run,
                         component_val,
                         self.report_folder,
                         hyperparam_name=hyperdrive_hyperparam_name,
                     )
                     full_artifact_path = ",".join(artifact_paths)
                 else:
                     full_artifact_path = str(self.report_folder / component_val)
                     download_files_from_run_id(run_id, self.report_folder, prefix=component_val)
 
-                updated_component = {ReportComponentKey.TYPE.value: component_type,
-                                     ReportComponentKey.VALUE.value: full_artifact_path}
+                updated_component = {
+                    ReportComponentKey.TYPE.value: component_type,
+                    ReportComponentKey.VALUE.value: full_artifact_path,
+                }
 
                 # add back any other entries such as figsize, num_columns etc
                 additional_keys = set(component.keys()).difference(set(updated_component.keys()))
                 for k in additional_keys:
                     updated_component[k] = component[k]
                 updated_report_contents.append(updated_component)
 
@@ -515,14 +540,15 @@
         """
         Zip the report folder at the location '<report_folder>.zip', preserving the directory structure.
         Returns the path to the zipped folder
 
         :return: The path to the zipped folder
         """
         import zipfile
+
         report_files = self.report_folder.rglob("*.*")
         zipped_folder_path = self.report_folder.with_suffix(".zip")
         with zipfile.ZipFile(zipped_folder_path, "w") as zipped_folder:
             for report_file in report_files:
                 zipped_folder.write(report_file, arcname=report_file.relative_to(self.report_folder))
         print(f"Zipped folder path: {str(zipped_folder_path)}")
         return zipped_folder_path
```

### Comparing `hi-ml-0.2.9/src/health_ml/utils/serialization.py` & `hi-ml-0.3.0/src/health_ml/utils/serialization.py`

 * *Files 1% similar despite different names*

```diff
@@ -21,45 +21,46 @@
     stream = BytesIO()
     pickle.dump(o, file=stream)
     stream.seek(0)
     return stream
 
 
 class ModelInfo:
-    """Stores a model, its example input, and metadata that describes how the model was trained.
-    """
+    """Stores a model, its example input, and metadata that describes how the model was trained."""
+
     MODEL = "model"
     MODEL_EXAMPLE_INPUT = "model_example_input"
     MODEL_CONFIG_YAML = "model_config_yaml"
     GIT_REPOSITORY = "git_repository"
     GIT_COMMIT_HASH = "git_commit_hash"
     DATASET_NAME = "dataset_name"
     AZURE_ML_WORKSPACE = "azure_ml_workspace"
     AZURE_ML_RUN_ID = "azure_ml_run_id"
     TEXT_TOKENIZER = "text_tokenizer"
     IMAGE_PRE_PROCESSING = "image_pre_processing"
     IMAGE_DIMENSIONS = "image_dimensions"
     OTHER_INFO = "other_info"
     OTHER_DESCRIPTION = "other_description"
 
-    def __init__(self,
-                 model: Optional[Union[torch.nn.Module, torch.jit.ScriptModule]] = None,
-                 model_example_input: Optional[torch.Tensor] = None,
-                 model_config: Any = None,
-                 git_repository: str = "",
-                 git_commit_hash: str = "",
-                 dataset_name: str = "",
-                 azure_ml_workspace: str = "",
-                 azure_ml_run_id: str = "",
-                 text_tokenizer: Any = None,
-                 image_pre_processing: Optional[Callable] = None,
-                 image_dimensions: str = "",
-                 other_info: Any = None,
-                 other_description: str = "",
-                 ):
+    def __init__(
+        self,
+        model: Optional[Union[torch.nn.Module, torch.jit.ScriptModule]] = None,
+        model_example_input: Optional[torch.Tensor] = None,
+        model_config: Any = None,
+        git_repository: str = "",
+        git_commit_hash: str = "",
+        dataset_name: str = "",
+        azure_ml_workspace: str = "",
+        azure_ml_run_id: str = "",
+        text_tokenizer: Any = None,
+        image_pre_processing: Optional[Callable] = None,
+        image_dimensions: str = "",
+        other_info: Any = None,
+        other_description: str = "",
+    ):
         """
         :param model: The model that should be serialized, or the deserialized model, defaults to None
         :param model_example_input: A tensor that can be input to the forward pass of the model, defaults to None
         :param model_config: The configuration object that was used to start the training run, defaults to None
         :param git_repository: The name of the git repository that contains the training codebase, defaults to ""
         :param git_commit_hash: The git commit hash that was used to run the training, defaults to ""
         :param dataset_name: The name of the dataset that was used to train the model, defaults to ""
@@ -105,14 +106,15 @@
             self.git_commit_hash = properties.get("azureml.git.commit", "")
 
     def state_dict(self, strict: bool = True) -> Dict[str, Any]:
         """Creates a dictionary representation of the current object.
 
         :param strict: The setting for the 'strict' flag in the call to torch.jit.trace.
         """
+
         def bytes_or_none(o: Any) -> Optional[bytes]:
             return _dump_to_stream(o).getvalue() if o is not None else None
 
         if self.model is None or self.model_example_input is None:
             raise ValueError("To generate a state dict, the model and model_example_input must be present.")
         try:
             traced_model = torch.jit.trace(self.model, self.model_example_input, strict=strict)
@@ -133,22 +135,23 @@
             ModelInfo.DATASET_NAME: self.dataset_name,
             ModelInfo.AZURE_ML_WORKSPACE: self.azure_ml_workspace,
             ModelInfo.AZURE_ML_RUN_ID: self.azure_ml_run_id,
             ModelInfo.TEXT_TOKENIZER: bytes_or_none(self.text_tokenizer),
             ModelInfo.IMAGE_PRE_PROCESSING: bytes_or_none(self.image_pre_processing),
             ModelInfo.IMAGE_DIMENSIONS: self.image_dimensions,
             ModelInfo.OTHER_INFO: bytes_or_none(self.other_info),
-            ModelInfo.OTHER_DESCRIPTION: self.other_description
+            ModelInfo.OTHER_DESCRIPTION: self.other_description,
         }
 
     def load_state_dict(self, state_dict: Dict[str, Any]) -> None:
         """Loads a dictionary representation into the current object, overwriting all matching fields.
 
         :param state_dict: The dictionary to load from.
         """
+
         def unpickle_from_bytes(field: str) -> Any:
             if field not in state_dict:
                 raise KeyError(f"State_dict does not contain a field '{field}'")
             b = state_dict[field]
             if b is None:
                 return None
             stream = BytesIO(b)
```

### Comparing `hi-ml-0.2.9/src/health_ml/utils/split_dataset.py` & `hi-ml-0.3.0/src/health_ml/utils/split_dataset.py`

 * *Files 2% similar despite different names*

```diff
@@ -50,36 +50,42 @@
 
         if self.group_column is not None:
             groups_train = self.train[self.group_column].unique()
             groups_test = self.test[self.group_column].unique()
             groups_val = self.val[self.group_column].unique()
             group_intersection = pairwise_intersection(groups_train, groups_test, groups_val)
             if len(group_intersection) != 0:
-                raise ValueError("Train, Test, and Val splits must have no intersecting groups, found: {}"
-                                 .format(group_intersection))
+                raise ValueError(
+                    "Train, Test, and Val splits must have no intersecting groups, found: {}".format(group_intersection)
+                )
 
         if (not self.allow_empty) and any([len(x) == 0 for x in [unique_train, unique_val]]):
-            raise ValueError("train_ids({}), val_ids({}) must have at least one value"
-                             .format(len(unique_train), len(unique_val)))
+            raise ValueError(
+                "train_ids({}), val_ids({}) must have at least one value".format(len(unique_train), len(unique_val))
+            )
 
     def __str__(self) -> str:
         unique_train, unique_test, unique_val = self.unique_subjects()
-        return f'Train: {len(unique_train)}, Test: {len(unique_test)}, and Val: {len(unique_val)}. ' \
-               f'Total subjects: {len(unique_train) + len(unique_test) + len(unique_val)}'
+        return (
+            f'Train: {len(unique_train)}, Test: {len(unique_test)}, and Val: {len(unique_val)}. '
+            f'Total subjects: {len(unique_train) + len(unique_test) + len(unique_val)}'
+        )
 
     def unique_subjects(self) -> Tuple[Any, Any, Any]:
         """
         Return a tuple of pandas Series of unique subjects across train, test and validation data splits,
         based on self.subject_column
 
         :return: a tuple of pandas Series
         """
-        return (self.train[self.subject_column].unique(),
-                self.test[self.subject_column].unique(),
-                self.val[self.subject_column].unique())
+        return (
+            self.train[self.subject_column].unique(),
+            self.test[self.subject_column].unique(),
+            self.val[self.subject_column].unique(),
+        )
 
     def number_of_subjects(self) -> int:
         """
         Returns the sum of unique subjects in the dataset (identified by self.subject_column), summed
         over train, test and validation data splits
 
         :return: An integer representing the number of unique subjects
@@ -101,71 +107,75 @@
             return self.test
         elif mode == ModelExecutionMode.VAL:
             return self.val
         else:
             raise ValueError(f"Model execution mode not recognized: {mode}")
 
     @staticmethod
-    def get_subject_ranges_for_splits(population: Sequence[str],
-                                      proportion_train: float,
-                                      proportion_test: float,
-                                      proportion_val: float) \
-            -> Dict[ModelExecutionMode, Set[str]]:
+    def get_subject_ranges_for_splits(
+        population: Sequence[str], proportion_train: float, proportion_test: float, proportion_val: float
+    ) -> Dict[ModelExecutionMode, Set[str]]:
         """
         Get mutually exclusive subject ranges for each dataset split (w.r.t to the proportion provided)
         ensuring all sets have at least one item in them when possible.
 
         :param population: all subjects
         :param proportion_train: proportion for the train set.
         :param proportion_test: proportion for the test set.
         :param proportion_val: proportion for the validation set.
         :return: Train, Test, and Val splits
         """
         sum_proportions = proportion_train + proportion_val + proportion_test
         if not np.isclose(sum_proportions, 1):
-            raise ValueError("proportion_train({}) + proportion_val({}) + proportion_test({}) must be ~ 1, found: {}"
-                             .format(proportion_train, proportion_val, proportion_test, sum_proportions))
+            raise ValueError(
+                "proportion_train({}) + proportion_val({}) + proportion_test({}) must be ~ 1, found: {}".format(
+                    proportion_train, proportion_val, proportion_test, sum_proportions
+                )
+            )
 
         if not 0 <= proportion_test < 1:
-            raise ValueError("proportion_test({}) must be in range [0, 1)"
-                             .format(proportion_test))
+            raise ValueError("proportion_test({}) must be in range [0, 1)".format(proportion_test))
 
         if not all([0 < x < 1 for x in [proportion_train, proportion_val]]):
-            raise ValueError("proportion_train({}) and proportion_val({}) must be in range (0, 1)"
-                             .format(proportion_train, proportion_val))
+            raise ValueError(
+                "proportion_train({}) and proportion_val({}) must be in range (0, 1)".format(
+                    proportion_train, proportion_val
+                )
+            )
 
-        subjects_train, subjects_test, subjects_val = (set(population[0:1]),
-                                                       set(population[1:2]),
-                                                       set(population[2:3]))
+        subjects_train, subjects_test, subjects_val = (set(population[0:1]), set(population[1:2]), set(population[2:3]))
         remaining = list(population[3:])
         if proportion_test == 0:
             remaining = list(subjects_test) + remaining
             subjects_test = set()
 
         subjects_train |= set(remaining[: ceil(len(remaining) * proportion_train)])
         if len(subjects_test) > 0:
-            subjects_test |= set(remaining[len(subjects_train):
-                                           len(subjects_train) + ceil(len(remaining) * proportion_test)])
+            subjects_test |= set(
+                remaining[len(subjects_train) : len(subjects_train) + ceil(len(remaining) * proportion_test)]
+            )
         subjects_val |= set(remaining) - (subjects_train | subjects_test)
         result = {
             ModelExecutionMode.TRAIN: subjects_train,
             ModelExecutionMode.TEST: subjects_test,
-            ModelExecutionMode.VAL: subjects_val
+            ModelExecutionMode.VAL: subjects_val,
         }
         return result
 
     @staticmethod
-    def _from_split_keys(df: pd.DataFrame,
-                         train_keys: Sequence[str],
-                         test_keys: Sequence[str],
-                         val_keys: Sequence[str],
-                         *,  # make column names keyword-only arguments to avoid mistakes when providing both
-                         key_column: str,
-                         subject_column: str,
-                         group_column: Optional[str]) -> DatasetSplits:
+    def _from_split_keys(
+        df: pd.DataFrame,
+        train_keys: Sequence[str],
+        test_keys: Sequence[str],
+        val_keys: Sequence[str],
+        *,  # make column names keyword-only arguments to avoid mistakes when providing both
+        key_column: str,
+        subject_column: str,
+        group_column: Optional[str],
+    ) -> DatasetSplits:
         """
         Takes a slice of values from each data split train/test/val for the provided keys.
 
         :param df: the input DataFrame
         :param train_keys: keys for training.
         :param test_keys: keys for testing.
         :param val_keys: keys for validation.
@@ -175,27 +185,30 @@
             in the same subset (train, val, or test) and cross-validation fold.
         :return: Data splits with respected dataset split ids.
         """
         train_df = DatasetSplits.get_df_from_ids(df, train_keys, key_column)
         test_df = DatasetSplits.get_df_from_ids(df, test_keys, key_column)
         val_df = DatasetSplits.get_df_from_ids(df, val_keys, key_column)
 
-        return DatasetSplits(train=train_df, test=test_df, val=val_df,
-                             subject_column=subject_column, group_column=group_column)
+        return DatasetSplits(
+            train=train_df, test=test_df, val=val_df, subject_column=subject_column, group_column=group_column
+        )
 
     @staticmethod
-    def from_proportions(df: pd.DataFrame,
-                         proportion_train: float,
-                         proportion_test: float,
-                         proportion_val: float,
-                         *,  # make column names keyword-only arguments to avoid mistakes when providing both
-                         subject_column: str = "",
-                         group_column: Optional[str] = None,
-                         shuffle: bool = True,
-                         random_seed: int = 0) -> DatasetSplits:
+    def from_proportions(
+        df: pd.DataFrame,
+        proportion_train: float,
+        proportion_test: float,
+        proportion_val: float,
+        *,  # make column names keyword-only arguments to avoid mistakes when providing both
+        subject_column: str = "",
+        group_column: Optional[str] = None,
+        shuffle: bool = True,
+        random_seed: int = 0,
+    ) -> DatasetSplits:
         """
         Creates a split of a dataset into train, test, and validation set, according to fixed proportions using
         the "subject" column in the dataframe, or the group column, if given.
 
         :param df: The dataframe containing all subjects.
         :param proportion_train: proportion for the train set.
         :param proportion_test: proportion for the test set.
@@ -212,75 +225,94 @@
         if shuffle:
             # fix the random seed so we can guarantee reproducibility when working with shuffle
             random.Random(random_seed).shuffle(split_keys)
         ranges = DatasetSplits.get_subject_ranges_for_splits(
             split_keys,
             proportion_train=proportion_train,
             proportion_val=proportion_val,
-            proportion_test=proportion_test
+            proportion_test=proportion_test,
+        )
+        return DatasetSplits._from_split_keys(
+            df,
+            list(ranges[ModelExecutionMode.TRAIN]),
+            list(ranges[ModelExecutionMode.TEST]),
+            list(ranges[ModelExecutionMode.VAL]),
+            key_column=key_column,
+            subject_column=subject_column,
+            group_column=group_column,
         )
-        return DatasetSplits._from_split_keys(df,
-                                              list(ranges[ModelExecutionMode.TRAIN]),
-                                              list(ranges[ModelExecutionMode.TEST]),
-                                              list(ranges[ModelExecutionMode.VAL]),
-                                              key_column=key_column,
-                                              subject_column=subject_column,
-                                              group_column=group_column)
 
     @staticmethod
-    def from_subject_ids(df: pd.DataFrame,
-                         train_ids: Sequence[str],
-                         test_ids: Sequence[str],
-                         val_ids: Sequence[str],
-                         *,  # make column names keyword-only arguments to avoid mistakes when providing both
-                         subject_column: str = "",
-                         group_column: Optional[str] = None) -> DatasetSplits:
+    def from_subject_ids(
+        df: pd.DataFrame,
+        train_ids: Sequence[str],
+        test_ids: Sequence[str],
+        val_ids: Sequence[str],
+        *,  # make column names keyword-only arguments to avoid mistakes when providing both
+        subject_column: str = "",
+        group_column: Optional[str] = None,
+    ) -> DatasetSplits:
         """
         Assuming a DataFrame with columns subject
         Takes a slice of values from each data split train/test/val for the provided ids.
 
         :param df: the input DataFrame
         :param train_ids: ids for training.
         :param test_ids: ids for testing.
         :param val_ids: ids for validation.
         :param subject_column: subject id column name
         :param group_column: grouping column name; if given, samples from each group will always be
             in the same subset (train, val, or test) and cross-validation fold.
         :return: Data splits with respected dataset split ids.
         """
-        return DatasetSplits._from_split_keys(df, train_ids, test_ids, val_ids, key_column=subject_column,
-                                              subject_column=subject_column, group_column=group_column)
+        return DatasetSplits._from_split_keys(
+            df,
+            train_ids,
+            test_ids,
+            val_ids,
+            key_column=subject_column,
+            subject_column=subject_column,
+            group_column=group_column,
+        )
 
     @staticmethod
-    def from_groups(df: pd.DataFrame,
-                    train_groups: Sequence[str],
-                    test_groups: Sequence[str],
-                    val_groups: Sequence[str],
-                    *,  # make column names keyword-only arguments to avoid mistakes when providing both
-                    group_column: str,
-                    subject_column: str = "") -> DatasetSplits:
+    def from_groups(
+        df: pd.DataFrame,
+        train_groups: Sequence[str],
+        test_groups: Sequence[str],
+        val_groups: Sequence[str],
+        *,  # make column names keyword-only arguments to avoid mistakes when providing both
+        group_column: str,
+        subject_column: str = "",
+    ) -> DatasetSplits:
         """
         Assuming a DataFrame with columns subject
         Takes a slice of values from each data split train/test/val for the provided groups.
 
         :param df: the input DataFrame
         :param train_groups: groups for training.
         :param test_groups: groups for testing.
         :param val_groups: groups for validation.
         :param subject_column: subject id column name
         :param group_column: grouping column name; if given, samples from each group will always be
             in the same subset (train, val, or test) and cross-validation fold.
         :return: Data splits with respected dataset split ids.
         """
-        return DatasetSplits._from_split_keys(df, train_groups, test_groups, val_groups, key_column=group_column,
-                                              subject_column=subject_column, group_column=group_column)
+        return DatasetSplits._from_split_keys(
+            df,
+            train_groups,
+            test_groups,
+            val_groups,
+            key_column=group_column,
+            subject_column=subject_column,
+            group_column=group_column,
+        )
 
     @staticmethod
-    def get_df_from_ids(df: pd.DataFrame, ids: Sequence[str],
-                        subject_column: Optional[str] = "") -> pd.DataFrame:
+    def get_df_from_ids(df: pd.DataFrame, ids: Sequence[str], subject_column: Optional[str] = "") -> pd.DataFrame:
         """
         Retrieve a subset dataframe where the subject column is restricted to a sequence of provided ids
 
         :param df: The dataframe to restrict
         :param ids: The ids to lookup
         :param subject_column: The column to lookup ids in. Defaults to ""
         :return: A subset of the dataframe
@@ -320,11 +352,16 @@
             folds_gen = k_folds.split(subject_ids, groups=groups)
 
         def ids_from_indices(indices: Sequence[int]) -> List[str]:
             return [subject_ids[x] for x in indices]
 
         # create the number of requested splits of the dataset
         return [
-            DatasetSplits(train=self.get_df_from_ids(cv_dataset, ids_from_indices(train_indices), self.subject_column),
-                          val=self.get_df_from_ids(cv_dataset, ids_from_indices(val_indices), self.subject_column),
-                          test=self.test, subject_column=self.subject_column, group_column=self.group_column)
-            for train_indices, val_indices in folds_gen]
+            DatasetSplits(
+                train=self.get_df_from_ids(cv_dataset, ids_from_indices(train_indices), self.subject_column),
+                val=self.get_df_from_ids(cv_dataset, ids_from_indices(val_indices), self.subject_column),
+                test=self.test,
+                subject_column=self.subject_column,
+                group_column=self.group_column,
+            )
+            for train_indices, val_indices in folds_gen
+        ]
```

### Comparing `hi-ml-0.2.9/src/health_ml/utils/type_annotations.py` & `hi-ml-0.3.0/src/health_ml/utils/type_annotations.py`

 * *Files identical despite different names*

### Comparing `hi-ml-0.2.9/src/hi_ml.egg-info/PKG-INFO` & `hi-ml-0.3.0/src/hi_ml.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hi-ml
-Version: 0.2.9
+Version: 0.3.0
 Summary: Microsoft Health Futures package containing high level ML components
 Home-page: https://github.com/microsoft/hi-ml
 Author: Biomedical Imaging Team @ Microsoft Health Futures
 Author-email: innereyedev@microsoft.com
 License: MIT License
 Description: # Microsoft Health Intelligence Machine Learning Toolbox
```

### Comparing `hi-ml-0.2.9/src/hi_ml.egg-info/SOURCES.txt` & `hi-ml-0.3.0/src/hi_ml.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -1,19 +1,21 @@
 LICENSE
 MANIFEST.in
 package_description.md
 run_requirements.txt
 setup.py
 src/health_ml/__init__.py
 src/health_ml/deep_learning_config.py
+src/health_ml/eval_runner.py
 src/health_ml/experiment_config.py
 src/health_ml/lightning_container.py
 src/health_ml/model_trainer.py
-src/health_ml/run_ml.py
 src/health_ml/runner.py
+src/health_ml/runner_base.py
+src/health_ml/training_runner.py
 src/health_ml/configs/hello_world.py
 src/health_ml/data/__init__.py
 src/health_ml/losses/__init__.py
 src/health_ml/networks/__init__.py
 src/health_ml/networks/blocks/__init__.py
 src/health_ml/networks/layers/__init__.py
 src/health_ml/networks/layers/attention_layers.py
@@ -28,14 +30,15 @@
 src/health_ml/utils/data_augmentations.py
 src/health_ml/utils/diagnostics.py
 src/health_ml/utils/fixed_paths.py
 src/health_ml/utils/lightning_loggers.py
 src/health_ml/utils/logging.py
 src/health_ml/utils/lr_scheduler.py
 src/health_ml/utils/model_util.py
+src/health_ml/utils/package_setup.py
 src/health_ml/utils/regression_test_utils.py
 src/health_ml/utils/reports.py
 src/health_ml/utils/serialization.py
 src/health_ml/utils/split_dataset.py
 src/health_ml/utils/type_annotations.py
 src/hi_ml.egg-info/PKG-INFO
 src/hi_ml.egg-info/SOURCES.txt
```

