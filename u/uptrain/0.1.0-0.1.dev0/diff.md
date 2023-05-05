# Comparing `tmp/uptrain-0.1.0.tar.gz` & `tmp/uptrain-0.1.dev0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "uptrain-0.1.0.tar", last modified: Fri May  5 06:42:07 2023, max compression
+gzip compressed data, was "uptrain-0.1.dev0.tar", last modified: Mon Jan 23 18:48:28 2023, max compression
```

## Comparing `uptrain-0.1.0.tar` & `uptrain-0.1.dev0.tar`

### file list

```diff
@@ -1,112 +1,70 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 06:42:07.952540 uptrain-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-05 06:41:47.000000 uptrain-0.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    11238 2023-05-05 06:42:07.952540 uptrain-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    10448 2023-05-05 06:41:47.000000 uptrain-0.1.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-05 06:42:07.952540 uptrain-0.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1827 2023-05-05 06:41:47.000000 uptrain-0.1.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 06:42:07.940540 uptrain-0.1.0/uptrain/
--rw-r--r--   0 runner    (1001) docker     (123)      418 2023-05-05 06:41:47.000000 uptrain-0.1.0/uptrain/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2008 2023-05-05 06:41:47.000000 uptrain-0.1.0/uptrain/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 06:42:07.940540 uptrain-0.1.0/uptrain/core/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 06:41:47.000000 uptrain-0.1.0/uptrain/core/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 06:42:07.940540 uptrain-0.1.0/uptrain/core/classes/
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-05-05 06:41:47.000000 uptrain-0.1.0/uptrain/core/classes/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 06:42:07.940540 uptrain-0.1.0/uptrain/core/classes/algorithms/
--rw-r--r--   0 runner    (1001) docker     (123)       78 2023-05-05 06:41:47.000000 uptrain-0.1.0/uptrain/core/classes/algorithms/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10395 2023-05-05 06:41:47.000000 uptrain-0.1.0/uptrain/core/classes/algorithms/clustering.py
--rw-r--r--   0 runner    (1001) docker     (123)     1456 2023-05-05 06:41:47.000000 uptrain-0.1.0/uptrain/core/classes/algorithms/popularity_bias.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 06:42:07.944540 uptrain-0.1.0/uptrain/core/classes/distances/
--rw-r--r--   0 runner    (1001) docker     (123)      211 2023-05-05 06:41:47.000000 uptrain-0.1.0/uptrain/core/classes/distances/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      471 2023-05-05 06:41:47.000000 uptrain-0.1.0/uptrain/core/classes/distances/abstract_distance.py
--rw-r--r--   0 runner    (1001) docker     (123)     1730 2023-05-05 06:41:47.000000 uptrain-0.1.0/uptrain/core/classes/distances/cosine_distance.py
--rw-r--r--   0 runner    (1001) docker     (123)      536 2023-05-05 06:41:47.000000 uptrain-0.1.0/uptrain/core/classes/distances/distance_resolver.py
--rw-r--r--   0 runner    (1001) docker     (123)     1631 2023-05-05 06:41:47.000000 uptrain-0.1.0/uptrain/core/classes/distances/hamming_distance.py
--rw-r--r--   0 runner    (1001) docker     (123)     1008 2023-05-05 06:41:47.000000 uptrain-0.1.0/uptrain/core/classes/distances/l2_distance.py
--rw-r--r--   0 runner    (1001) docker     (123)     1279 2023-05-05 06:41:47.000000 uptrain-0.1.0/uptrain/core/classes/distances/norm_ratio.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 06:42:07.944540 uptrain-0.1.0/uptrain/core/classes/finetuning/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 06:41:47.000000 uptrain-0.1.0/uptrain/core/classes/finetuning/AbstractFinetune.py
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-05-05 06:41:47.000000 uptrain-0.1.0/uptrain/core/classes/finetuning/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5545 2023-05-05 06:41:47.000000 uptrain-0.1.0/uptrain/core/classes/finetuning/finetuning.py
--rw-r--r--   0 runner    (1001) docker     (123)    18088 2023-05-05 06:41:47.000000 uptrain-0.1.0/uptrain/core/classes/framework.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 06:42:07.944540 uptrain-0.1.0/uptrain/core/classes/helpers/
--rw-r--r--   0 runner    (1001) docker     (123)      132 2023-05-05 06:41:47.000000 uptrain-0.1.0/uptrain/core/classes/helpers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1146 2023-05-05 06:41:47.000000 uptrain-0.1.0/uptrain/core/classes/helpers/annotation_helper.py
--rw-r--r--   0 runner    (1001) docker     (123)     1814 2023-05-05 06:41:47.000000 uptrain-0.1.0/uptrain/core/classes/helpers/config_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     4171 2023-05-05 06:41:47.000000 uptrain-0.1.0/uptrain/core/classes/helpers/dataset_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     3141 2023-05-05 06:41:47.000000 uptrain-0.1.0/uptrain/core/classes/helpers/model_handler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 06:42:07.944540 uptrain-0.1.0/uptrain/core/classes/logging/
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-05-05 06:41:47.000000 uptrain-0.1.0/uptrain/core/classes/logging/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6193 2023-05-05 06:41:47.000000 uptrain-0.1.0/uptrain/core/classes/logging/log_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     6416 2023-05-05 06:41:47.000000 uptrain-0.1.0/uptrain/core/classes/logging/log_streamlit.py
--rw-r--r--   0 runner    (1001) docker     (123)     6120 2023-05-05 06:41:47.000000 uptrain-0.1.0/uptrain/core/classes/logging/new_log_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     9051 2023-05-05 06:41:47.000000 uptrain-0.1.0/uptrain/core/classes/logging/new_st_run.py
--rw-r--r--   0 runner    (1001) docker     (123)     1263 2023-05-05 06:41:47.000000 uptrain-0.1.0/uptrain/core/classes/logging/new_st_setup.py
--rw-r--r--   0 runner    (1001) docker     (123)    19630 2023-05-05 06:41:47.000000 uptrain-0.1.0/uptrain/core/classes/logging/st_run.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 06:42:07.944540 uptrain-0.1.0/uptrain/core/classes/managers/
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-05-05 06:41:47.000000 uptrain-0.1.0/uptrain/core/classes/managers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7147 2023-05-05 06:41:47.000000 uptrain-0.1.0/uptrain/core/classes/managers/check_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 06:42:07.948541 uptrain-0.1.0/uptrain/core/classes/measurables/
--rw-r--r--   0 runner    (1001) docker     (123)      648 2023-05-05 06:41:47.000000 uptrain-0.1.0/uptrain/core/classes/measurables/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1540 2023-05-05 06:41:47.000000 uptrain-0.1.0/uptrain/core/classes/measurables/abstract_measurable.py
--rw-r--r--   0 runner    (1001) docker     (123)     2056 2023-05-05 06:41:47.000000 uptrain-0.1.0/uptrain/core/classes/measurables/accuracy.py
--rw-r--r--   0 runner    (1001) docker     (123)     3056 2023-05-05 06:41:47.000000 uptrain-0.1.0/uptrain/core/classes/measurables/condition.py
--rw-r--r--   0 runner    (1001) docker     (123)     1615 2023-05-05 06:41:47.000000 uptrain-0.1.0/uptrain/core/classes/measurables/custom.py
--rw-r--r--   0 runner    (1001) docker     (123)     2041 2023-05-05 06:41:47.000000 uptrain-0.1.0/uptrain/core/classes/measurables/distance.py
--rw-r--r--   0 runner    (1001) docker     (123)     1558 2023-05-05 06:41:47.000000 uptrain-0.1.0/uptrain/core/classes/measurables/feature.py
--rw-r--r--   0 runner    (1001) docker     (123)      836 2023-05-05 06:41:47.000000 uptrain-0.1.0/uptrain/core/classes/measurables/feature_concat.py
--rw-r--r--   0 runner    (1001) docker     (123)      667 2023-05-05 06:41:47.000000 uptrain-0.1.0/uptrain/core/classes/measurables/input_feature.py
--rw-r--r--   0 runner    (1001) docker     (123)     4347 2023-05-05 06:41:47.000000 uptrain-0.1.0/uptrain/core/classes/measurables/measurable.py
--rw-r--r--   0 runner    (1001) docker     (123)     3001 2023-05-05 06:41:47.000000 uptrain-0.1.0/uptrain/core/classes/measurables/measurable_resolver.py
--rw-r--r--   0 runner    (1001) docker     (123)      596 2023-05-05 06:41:47.000000 uptrain-0.1.0/uptrain/core/classes/measurables/output_feature.py
--rw-r--r--   0 runner    (1001) docker     (123)      547 2023-05-05 06:41:47.000000 uptrain-0.1.0/uptrain/core/classes/measurables/recommendation_hit_rate.py
--rw-r--r--   0 runner    (1001) docker     (123)     1000 2023-05-05 06:41:47.000000 uptrain-0.1.0/uptrain/core/classes/measurables/scalar_from_embedding.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 06:42:07.948541 uptrain-0.1.0/uptrain/core/classes/monitors/
--rw-r--r--   0 runner    (1001) docker     (123)      431 2023-05-05 06:41:47.000000 uptrain-0.1.0/uptrain/core/classes/monitors/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3034 2023-05-05 06:41:47.000000 uptrain-0.1.0/uptrain/core/classes/monitors/abstract_check.py
--rw-r--r--   0 runner    (1001) docker     (123)     1510 2023-05-05 06:41:47.000000 uptrain-0.1.0/uptrain/core/classes/monitors/abstract_monitor.py
--rw-r--r--   0 runner    (1001) docker     (123)     1292 2023-05-05 06:41:47.000000 uptrain-0.1.0/uptrain/core/classes/monitors/accuracy.py
--rw-r--r--   0 runner    (1001) docker     (123)     4191 2023-05-05 06:41:47.000000 uptrain-0.1.0/uptrain/core/classes/monitors/concept_drift.py
--rw-r--r--   0 runner    (1001) docker     (123)      781 2023-05-05 06:41:47.000000 uptrain-0.1.0/uptrain/core/classes/monitors/custom_monitor.py
--rw-r--r--   0 runner    (1001) docker     (123)    15919 2023-05-05 06:41:47.000000 uptrain-0.1.0/uptrain/core/classes/monitors/data_drift.py
--rw-r--r--   0 runner    (1001) docker     (123)     4878 2023-05-05 06:41:47.000000 uptrain-0.1.0/uptrain/core/classes/monitors/data_integrity.py
--rw-r--r--   0 runner    (1001) docker     (123)     1386 2023-05-05 06:41:47.000000 uptrain-0.1.0/uptrain/core/classes/monitors/edge_case.py
--rw-r--r--   0 runner    (1001) docker     (123)     4430 2023-05-05 06:41:47.000000 uptrain-0.1.0/uptrain/core/classes/monitors/feature_drift.py
--rw-r--r--   0 runner    (1001) docker     (123)      969 2023-05-05 06:41:47.000000 uptrain-0.1.0/uptrain/core/classes/monitors/model_bias.py
--rw-r--r--   0 runner    (1001) docker     (123)     3157 2023-05-05 06:41:47.000000 uptrain-0.1.0/uptrain/core/classes/monitors/output_comparison.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 06:42:07.948541 uptrain-0.1.0/uptrain/core/classes/signals/
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-05-05 06:41:47.000000 uptrain-0.1.0/uptrain/core/classes/signals/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5481 2023-05-05 06:41:47.000000 uptrain-0.1.0/uptrain/core/classes/signals/signal.py
--rw-r--r--   0 runner    (1001) docker     (123)     1188 2023-05-05 06:41:47.000000 uptrain-0.1.0/uptrain/core/classes/signals/signal_manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 06:42:07.948541 uptrain-0.1.0/uptrain/core/classes/statistics/
--rw-r--r--   0 runner    (1001) docker     (123)      199 2023-05-05 06:41:47.000000 uptrain-0.1.0/uptrain/core/classes/statistics/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      122 2023-05-05 06:41:47.000000 uptrain-0.1.0/uptrain/core/classes/statistics/abstract_statistic.py
--rw-r--r--   0 runner    (1001) docker     (123)     9762 2023-05-05 06:41:47.000000 uptrain-0.1.0/uptrain/core/classes/statistics/convergence.py
--rw-r--r--   0 runner    (1001) docker     (123)     6784 2023-05-05 06:41:47.000000 uptrain-0.1.0/uptrain/core/classes/statistics/distance.py
--rw-r--r--   0 runner    (1001) docker     (123)     8554 2023-05-05 06:41:47.000000 uptrain-0.1.0/uptrain/core/classes/statistics/distribution.py
--rw-r--r--   0 runner    (1001) docker     (123)     3086 2023-05-05 06:41:47.000000 uptrain-0.1.0/uptrain/core/classes/statistics/norm_embedding.py
--rw-r--r--   0 runner    (1001) docker     (123)     7557 2023-05-05 06:41:47.000000 uptrain-0.1.0/uptrain/core/classes/statistics/old_distribution.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 06:42:07.952540 uptrain-0.1.0/uptrain/core/classes/visuals/
--rw-r--r--   0 runner    (1001) docker     (123)      152 2023-05-05 06:41:47.000000 uptrain-0.1.0/uptrain/core/classes/visuals/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      120 2023-05-05 06:41:47.000000 uptrain-0.1.0/uptrain/core/classes/visuals/abstract_visual.py
--rw-r--r--   0 runner    (1001) docker     (123)    13800 2023-05-05 06:41:47.000000 uptrain-0.1.0/uptrain/core/classes/visuals/dimensionality_reduction.py
--rw-r--r--   0 runner    (1001) docker     (123)     6557 2023-05-05 06:41:47.000000 uptrain-0.1.0/uptrain/core/classes/visuals/plot.py
--rw-r--r--   0 runner    (1001) docker     (123)     1267 2023-05-05 06:41:47.000000 uptrain-0.1.0/uptrain/core/classes/visuals/shap.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 06:42:07.952540 uptrain-0.1.0/uptrain/core/encoders/
--rw-r--r--   0 runner    (1001) docker     (123)      813 2023-05-05 06:41:47.000000 uptrain-0.1.0/uptrain/core/encoders/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 06:42:07.952540 uptrain-0.1.0/uptrain/core/lib/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 06:41:47.000000 uptrain-0.1.0/uptrain/core/lib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1403 2023-05-05 06:41:47.000000 uptrain-0.1.0/uptrain/core/lib/algorithms.py
--rw-r--r--   0 runner    (1001) docker     (123)     2335 2023-05-05 06:41:47.000000 uptrain-0.1.0/uptrain/core/lib/cache.py
--rw-r--r--   0 runner    (1001) docker     (123)     3550 2023-05-05 06:41:47.000000 uptrain-0.1.0/uptrain/core/lib/datastores.py
--rw-r--r--   0 runner    (1001) docker     (123)    11235 2023-05-05 06:41:47.000000 uptrain-0.1.0/uptrain/core/lib/helper_funcs.py
--rw-r--r--   0 runner    (1001) docker     (123)      690 2023-05-05 06:41:47.000000 uptrain-0.1.0/uptrain/core/lib/model_signal_funcs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 06:42:07.952540 uptrain-0.1.0/uptrain/io/
--rw-r--r--   0 runner    (1001) docker     (123)       88 2023-05-05 06:41:47.000000 uptrain-0.1.0/uptrain/io/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1184 2023-05-05 06:41:47.000000 uptrain-0.1.0/uptrain/io/binary.py
--rw-r--r--   0 runner    (1001) docker     (123)     1249 2023-05-05 06:41:47.000000 uptrain-0.1.0/uptrain/io/text.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 06:42:07.940540 uptrain-0.1.0/uptrain.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    11238 2023-05-05 06:42:07.000000 uptrain-0.1.0/uptrain.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3785 2023-05-05 06:42:07.000000 uptrain-0.1.0/uptrain.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 06:42:07.000000 uptrain-0.1.0/uptrain.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      123 2023-05-05 06:42:07.000000 uptrain-0.1.0/uptrain.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-05 06:42:07.000000 uptrain-0.1.0/uptrain.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-23 18:48:28.222094 uptrain-0.1.dev0/
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-01-23 18:48:18.000000 uptrain-0.1.dev0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      923 2023-01-23 18:48:28.222094 uptrain-0.1.dev0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4477 2023-01-23 18:48:18.000000 uptrain-0.1.dev0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-01-23 18:48:28.222094 uptrain-0.1.dev0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2049 2023-01-23 18:48:18.000000 uptrain-0.1.dev0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-23 18:48:28.202093 uptrain-0.1.dev0/uptrain/
+-rw-r--r--   0 runner    (1001) docker     (123)      297 2023-01-23 18:48:18.000000 uptrain-0.1.dev0/uptrain/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1136 2023-01-23 18:48:18.000000 uptrain-0.1.dev0/uptrain/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-23 18:48:28.206094 uptrain-0.1.dev0/uptrain/core/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-23 18:48:18.000000 uptrain-0.1.dev0/uptrain/core/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-23 18:48:28.206094 uptrain-0.1.dev0/uptrain/core/classes/
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-01-23 18:48:18.000000 uptrain-0.1.dev0/uptrain/core/classes/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-23 18:48:28.206094 uptrain-0.1.dev0/uptrain/core/classes/algorithms/
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-01-23 18:48:18.000000 uptrain-0.1.dev0/uptrain/core/classes/algorithms/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2325 2023-01-23 18:48:18.000000 uptrain-0.1.dev0/uptrain/core/classes/algorithms/data_drift_ddm.py
+-rw-r--r--   0 runner    (1001) docker     (123)      389 2023-01-23 18:48:18.000000 uptrain-0.1.dev0/uptrain/core/classes/algorithms/popularity_bias.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-23 18:48:28.210094 uptrain-0.1.dev0/uptrain/core/classes/anomalies/
+-rw-r--r--   0 runner    (1001) docker     (123)      288 2023-01-23 18:48:18.000000 uptrain-0.1.dev0/uptrain/core/classes/anomalies/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      351 2023-01-23 18:48:18.000000 uptrain-0.1.dev0/uptrain/core/classes/anomalies/abstract_anomaly.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1815 2023-01-23 18:48:18.000000 uptrain-0.1.dev0/uptrain/core/classes/anomalies/concept_drift.py
+-rw-r--r--   0 runner    (1001) docker     (123)      929 2023-01-23 18:48:18.000000 uptrain-0.1.dev0/uptrain/core/classes/anomalies/custom_anomaly.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15261 2023-01-23 18:48:18.000000 uptrain-0.1.dev0/uptrain/core/classes/anomalies/data_drift.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1768 2023-01-23 18:48:18.000000 uptrain-0.1.dev0/uptrain/core/classes/anomalies/data_integrity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1185 2023-01-23 18:48:18.000000 uptrain-0.1.dev0/uptrain/core/classes/anomalies/edge_case.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-23 18:48:28.210094 uptrain-0.1.dev0/uptrain/core/classes/anomalies/managers/
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-01-23 18:48:18.000000 uptrain-0.1.dev0/uptrain/core/classes/anomalies/managers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3340 2023-01-23 18:48:18.000000 uptrain-0.1.dev0/uptrain/core/classes/anomalies/managers/anomaly_manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-23 18:48:28.214094 uptrain-0.1.dev0/uptrain/core/classes/anomalies/measurables/
+-rw-r--r--   0 runner    (1001) docker     (123)      544 2023-01-23 18:48:18.000000 uptrain-0.1.dev0/uptrain/core/classes/anomalies/measurables/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      264 2023-01-23 18:48:18.000000 uptrain-0.1.dev0/uptrain/core/classes/anomalies/measurables/abstract_measurable.py
+-rw-r--r--   0 runner    (1001) docker     (123)      474 2023-01-23 18:48:18.000000 uptrain-0.1.dev0/uptrain/core/classes/anomalies/measurables/accuracy_measurable.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1944 2023-01-23 18:48:18.000000 uptrain-0.1.dev0/uptrain/core/classes/anomalies/measurables/condition_measurable.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1036 2023-01-23 18:48:18.000000 uptrain-0.1.dev0/uptrain/core/classes/anomalies/measurables/custom_measurable.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1147 2023-01-23 18:48:18.000000 uptrain-0.1.dev0/uptrain/core/classes/anomalies/measurables/feature_measurable.py
+-rw-r--r--   0 runner    (1001) docker     (123)      588 2023-01-23 18:48:18.000000 uptrain-0.1.dev0/uptrain/core/classes/anomalies/measurables/input_feature_measurable.py
+-rw-r--r--   0 runner    (1001) docker     (123)      550 2023-01-23 18:48:18.000000 uptrain-0.1.dev0/uptrain/core/classes/anomalies/measurables/measurable.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1863 2023-01-23 18:48:18.000000 uptrain-0.1.dev0/uptrain/core/classes/anomalies/measurables/measurable_resolver.py
+-rw-r--r--   0 runner    (1001) docker     (123)      457 2023-01-23 18:48:18.000000 uptrain-0.1.dev0/uptrain/core/classes/anomalies/measurables/output_feature_measurable.py
+-rw-r--r--   0 runner    (1001) docker     (123)      987 2023-01-23 18:48:18.000000 uptrain-0.1.dev0/uptrain/core/classes/anomalies/measurables/scalar_from_embedding_measurable.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1217 2023-01-23 18:48:18.000000 uptrain-0.1.dev0/uptrain/core/classes/anomalies/recommendation_bias.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-23 18:48:28.218094 uptrain-0.1.dev0/uptrain/core/classes/anomalies/signals/
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-01-23 18:48:18.000000 uptrain-0.1.dev0/uptrain/core/classes/anomalies/signals/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5397 2023-01-23 18:48:18.000000 uptrain-0.1.dev0/uptrain/core/classes/anomalies/signals/signal.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1198 2023-01-23 18:48:18.000000 uptrain-0.1.dev0/uptrain/core/classes/anomalies/signals/signal_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14322 2023-01-23 18:48:18.000000 uptrain-0.1.dev0/uptrain/core/classes/framework.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-23 18:48:28.218094 uptrain-0.1.dev0/uptrain/core/classes/helpers/
+-rw-r--r--   0 runner    (1001) docker     (123)      168 2023-01-23 18:48:18.000000 uptrain-0.1.dev0/uptrain/core/classes/helpers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1146 2023-01-23 18:48:18.000000 uptrain-0.1.dev0/uptrain/core/classes/helpers/annotation_helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1499 2023-01-23 18:48:18.000000 uptrain-0.1.dev0/uptrain/core/classes/helpers/config_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4059 2023-01-23 18:48:18.000000 uptrain-0.1.dev0/uptrain/core/classes/helpers/dataset_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2734 2023-01-23 18:48:18.000000 uptrain-0.1.dev0/uptrain/core/classes/helpers/log_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3141 2023-01-23 18:48:18.000000 uptrain-0.1.dev0/uptrain/core/classes/helpers/model_handler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-23 18:48:28.222094 uptrain-0.1.dev0/uptrain/core/classes/logging/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-23 18:48:18.000000 uptrain-0.1.dev0/uptrain/core/classes/logging/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4603 2023-01-23 18:48:18.000000 uptrain-0.1.dev0/uptrain/core/classes/logging/log_streamlit.py
+-rw-r--r--   0 runner    (1001) docker     (123)      510 2023-01-23 18:48:18.000000 uptrain-0.1.dev0/uptrain/core/classes/logging/log_tensorboard.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-23 18:48:28.222094 uptrain-0.1.dev0/uptrain/core/encoders/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-23 18:48:18.000000 uptrain-0.1.dev0/uptrain/core/encoders/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      413 2023-01-23 18:48:18.000000 uptrain-0.1.dev0/uptrain/core/encoders/numpy_encoder.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-23 18:48:28.222094 uptrain-0.1.dev0/uptrain/core/lib/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-01-23 18:48:18.000000 uptrain-0.1.dev0/uptrain/core/lib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4535 2023-01-23 18:48:18.000000 uptrain-0.1.dev0/uptrain/core/lib/helper_funcs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      690 2023-01-23 18:48:18.000000 uptrain-0.1.dev0/uptrain/core/lib/model_signal_funcs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-23 18:48:28.206094 uptrain-0.1.dev0/uptrain.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      923 2023-01-23 18:48:28.000000 uptrain-0.1.dev0/uptrain.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2422 2023-01-23 18:48:28.000000 uptrain-0.1.dev0/uptrain.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-23 18:48:28.000000 uptrain-0.1.dev0/uptrain.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      262 2023-01-23 18:48:28.000000 uptrain-0.1.dev0/uptrain.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-01-23 18:48:28.000000 uptrain-0.1.dev0/uptrain.egg-info/top_level.txt
```

### Comparing `uptrain-0.1.0/LICENSE` & `uptrain-0.1.dev0/LICENSE`

 * *Files identical despite different names*

### Comparing `uptrain-0.1.0/setup.py` & `uptrain-0.1.dev0/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,54 +1,60 @@
-"""
-A setuptools based setup module.
+"""A setuptools based setup module.
 """
 #!/usr/bin/env python
 
 # Always prefer setuptools over distutils
 from setuptools import setup, find_packages
 
-# read the contents of your README file
-from pathlib import Path
-
-this_directory = Path(__file__).parent
-long_description = (this_directory / "README.md").read_text()
-
 setup(
     name="uptrain",
-    version="0.1.0",
+    version="0.1.dev0",
     description="UpTrain - ML Observability and Retraining Framework",
-    long_description=long_description,
-    long_description_content_type="text/markdown",
+    long_description="Smart and Automated Model Refinement",
     # The project's main homepage.
     url="https://github.com/uptrain-ai/uptrain",
     # Author details
     maintainer="UpTrain AI Team",
     maintainer_email="uptrain.ai@gmail.com",
     # Choose your license
     license="Apache License 2.0",
     # See https://pypi.python.org/pypi?%3Aaction=list_classifiers
     classifiers=[
-        "Development Status :: 5 - Production/Stable",
+        # How mature is this project? Common values are
+        #   3 - Alpha
+        #   4 - Beta
+        #   5 - Production/Stable
+        "Development Status :: 4 - Beta",
         "Intended Audience :: Developers",
         "Topic :: Software Development :: Build Tools",
         # Pick your license as you wish (should match "license" above)
         "License :: OSI Approved :: Apache Software License",
         # Specify the Python versions you support here. In particular, ensure
+        "Programming Language :: Python :: 3",
+        "Programming Language :: Python :: 3.3",
+        "Programming Language :: Python :: 3.4",
+        "Programming Language :: Python :: 3.5",
+        "Programming Language :: Python :: 3.6",
+        "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
-        "Programming Language :: Python :: 3.9",
-        "Programming Language :: Python :: 3.10",
-        "Programming Language :: Python :: 3.11",
     ],
     keywords="uptrain ai retraining ML observability",
     packages=find_packages(),
     install_requires=[
-        "numpy>=1.23.0",
-        "pandas>=1.0.0",
-        "plotly>=5.0.0",
-        "pydantic>=1.9.0",
-        "river<=0.14",
-        "scikit_learn>=1.0.0",
-        "streamlit>=1.0.0",
-        "json-fix>=0.5.0"
+        "imgaug==0.4.0",
+        "numpy==1.24.1",
+        "pandas==1.5.2",
+        "plotly==5.11.0",
+        "pydantic==1.10.4",
+        "scikit_learn==1.2.0",
+        "scipy==1.10.0",
+        "seaborn==0.12.2",
+        "setuptools==65.6.3",
+        "streamlit==1.16.0",
+        "tensorboardX==2.5.1",
+        "torch==1.13.1",
+        "xgboost==1.7.3",
+        "joblib==1.2.0",
+        "tensorboard==2.11.0",
+        "jupyterlab==3.5.2",
     ],
-    tests_require=["pytest>=7.0", "torch", "imgaug", "gensim", "xgboost"]
 )
```

### Comparing `uptrain-0.1.0/uptrain/core/classes/framework.py` & `uptrain-0.1.dev0/uptrain/core/classes/framework.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,26 +1,20 @@
-from __future__ import annotations
 from copy import deepcopy
 import json
 import os
 import shutil
+import pandas as pd
 from datetime import datetime
 import random
-from queue import SimpleQueue
-from threading import Thread
-from typing import Optional
-
-import pandas as pd
 import numpy as np
 from sklearn.preprocessing import normalize
 
-from uptrain.core.classes.helpers import DatasetHandler, ModelHandler, config_handler
-from uptrain.core.classes.logging import LogHandler
-from uptrain.core.classes.logging.new_log_handler import LogHandler as NewLogHandler
-from uptrain.core.classes.managers import CheckManager
+from uptrain.core.classes.helpers import DatasetHandler, ModelHandler
+from uptrain.core.classes.helpers import config_handler, LogHandler
+from uptrain.core.classes.anomalies.managers import AnomalyManager
 from uptrain.core.lib.helper_funcs import (
     read_json,
     extract_data_points_from_batch,
     add_data_to_warehouse,
     get_df_indices_from_ids,
     get_feature_names_list,
     load_list_from_df,
@@ -54,94 +48,68 @@
         Parameters
         ----------
         cfg : dict
             Config to initialize uptrain framework
         """
 
         cfg = config_handler.Config(**cfg_dict)
-        self.config_obj = cfg
-        self.run_background_log_consumer = cfg.run_background_log_consumer
+        training_args = cfg.training_args
+        evaluation_args = cfg.evaluation_args
 
-        if self.run_background_log_consumer:
-            self.msg_queue = SimpleQueue()
-            cfg_copy = deepcopy(cfg_dict)
-            cfg_copy.update({"run_background_log_consumer": False})
-            daemon = Thread(
-                target=background_log_consumer_task,
-                args=(
-                    self.msg_queue,
-                    cfg_copy,
-                ),
-                daemon=True,
-                name="Background Log Consumer",
-            )
-            daemon.start()
-        else:
-            training_args = cfg.training_args
-            evaluation_args = cfg.evaluation_args
-
-            self.orig_training_file = training_args.orig_training_file
-            self.fold_name = cfg.retraining_folder
-            if os.path.exists(self.fold_name):
-                print("Deleting the folder: ", self.fold_name)
-                shutil.rmtree(self.fold_name)
-            os.mkdir(self.fold_name)
-
-            self.log_data = cfg.logging_args.log_data
-            self.use_cache = cfg.use_cache
-            self.cache = {}
-            self.predicted_count = 0
-            self.extra_args = {}
-            self.checks = cfg.checks
-            self.batch_size = None
-            self.feat_name_list = cfg.feat_name_list
-            self.retrain_after = cfg.retrain_after
-            self.data_id_type = cfg.data_id
-            self.version = 0
-            self.if_retraining = cfg.retrain
-            self.path_all_data = os.path.join(self.fold_name, "all_data.csv")
-
-            # TODO: placeholder till we decide on which way to go
-            if cfg.logging_args.use_new_handler:
-                self.log_handler = NewLogHandler(framework=self, cfg=cfg)
-            else:
-                self.log_handler = LogHandler(framework=self, cfg=cfg)
+        self.orig_training_file = training_args.orig_training_file
+        self.fold_name = cfg.retraining_folder
+        if os.path.exists(self.fold_name):
+            print("Deleting the folder: ", self.fold_name)
+            shutil.rmtree(self.fold_name)
+        os.mkdir(self.fold_name)
+
+        self.predicted_count = 0
+        self.extra_args = {}
+        self.checks = cfg.checks
+        self.batch_size = None
+        self.feat_name_list = cfg.feat_name_list
+        self.retrain_after = cfg.retrain_after
+        self.data_id_type = cfg.data_id
+        self.version = 0
+        self.if_retraining = cfg.retrain
+        self.path_all_data = os.path.join(self.fold_name, "all_data.csv")
+
+        self.dataset_handler = DatasetHandler(
+            cluster_plot_func=cfg.cluster_visualize_func
+        )
+        self.model_handler = ModelHandler()
+        self.log_handler = LogHandler(framework=self, cfg=cfg)
+        self.anomaly_manager = AnomalyManager(self, cfg.checks)
+        self.reset_retraining()
 
-            self.dataset_handler = DatasetHandler(framework=self, cfg=cfg)
-            self.model_handler = ModelHandler()
-            self.check_manager = CheckManager(self, self.checks)
-            self.reset_retraining()
-
-            if training_args.data_transformation_func:
-                self.set_data_transformation_func(
-                    training_args.data_transformation_func
-                )
-            if training_args.annotation_method:
-                am = training_args.annotation_method
-                self.set_annotation_method(am.method, args=am.args)
-            if evaluation_args.golden_testing_dataset:
-                self.set_golden_testing_dataset(evaluation_args.golden_testing_dataset)
-            if training_args.training_func:
-                self.set_training_func(training_args.training_func)
-            if evaluation_args.inference_func:
-                self.set_inference_func(evaluation_args.inference_func)
+        if training_args.data_transformation_func:
+            self.set_data_transformation_func(training_args.data_transformation_func)
+        if training_args.annotation_method:
+            am = training_args.annotation_method
+            self.set_annotation_method(am.method, args=am.args)
+        if evaluation_args.golden_testing_dataset:
+            self.set_golden_testing_dataset(evaluation_args.golden_testing_dataset)
+        if training_args.training_func:
+            self.set_training_func(training_args.training_func)
+        if evaluation_args.inference_func:
+            self.set_inference_func(evaluation_args.inference_func)
 
     def reset_retraining(self):
         self.version += 1
         self.selected_count = 0
         self.smart_data_ids = []
         retrain_folder = os.path.join(self.fold_name, str(self.version))
         if not os.path.exists(retrain_folder):
             os.mkdir(retrain_folder)
 
     def get_data_id(self, inputs):
         if self.data_id_type in inputs:
             ids = inputs[self.data_id_type]
-        elif self.data_id_type in inputs:
-            ids = inputs[self.data_id_type]
+        elif self.data_id_type in inputs["data"]:
+            ids = inputs["data"][self.data_id_type]
         elif self.data_id_type == "utc_timestamp":
             timestamp = str(datetime.utcnow().timestamp()).replace(".", "")
             rand_int = random.sample(
                 range(10 * self.batch_size), self.batch_size
             ).sort()
             ids = [int(timestamp + str(x)) for x in rand_int]
         elif self.data_id_type == "id":
@@ -158,110 +126,102 @@
         If yes, logs them to smart_data warehouse, which
         is used to create retraining dataset.
         """
 
         old_selected_count = self.selected_count
         smart_data = {}
 
-        is_interesting, reasons = self.is_data_interesting(
-            data, data["output"], data["gt"], extra_args=extra_args
+        is_interesting = self.is_data_interesting(
+            data["data"], data["output"], data["gt"], extra_args=extra_args
         )
         num_selected_datapoints = np.sum(np.array(is_interesting))
         self.selected_count += num_selected_datapoints
         self.smart_data_ids.extend(np.array(data["id"])[np.array(is_interesting)])
 
         """
-        Log only the interesting test cases to data
+        Log only the interesting test cases to data 
         warehouse. Logged under sub-folder 'smart_data'
         """
-        path_smart_data = os.path.join(
-            self.fold_name, str(self.version), "smart_data.csv"
-        )
-
-        if self.log_data and (num_selected_datapoints > 0):
-            data.update({"reasons": reasons})
+        if num_selected_datapoints > 0:
             smart_data = extract_data_points_from_batch(
                 data, np.where(is_interesting == True)[0]
             )
-            add_data_to_warehouse(deepcopy(smart_data), path_smart_data)
-
-        edge_cases_txt = (
-            str(self.selected_count)
-            + " edge cases identified out of "
-            + str(self.predicted_count)
-            + " total samples"
-        )
-        if self.selected_count > 0:
-            self.log_handler.add_alert(
-                "Number of edge cases collected", edge_cases_txt, "edge_cases"
+            path_smart_data = os.path.join(
+                self.fold_name, str(self.version), "smart_data.csv"
             )
+            add_data_to_warehouse(deepcopy(smart_data), path_smart_data)
 
         if (not (self.selected_count == old_selected_count)) and (
             not (int(self.selected_count / 50) == int(old_selected_count / 50))
         ):
-            print(edge_cases_txt)
+            print(
+                self.selected_count,
+                " edge cases identified out of ",
+                self.predicted_count,
+                " total samples",
+            )
 
     def infer_batch_size(self, inputs):
         batch_sizes = []
         for k, item in inputs.items():
-            item_batch_size = len(item)
+            if k == "data":
+                item_batch_size = self.infer_batch_size(inputs[k])
+            else:
+                item_batch_size = len(item)
             batch_sizes.append(item_batch_size)
         if np.var(np.array(batch_sizes)) > 0:
             # TODO: Raise warning on what is going wrong
             raise Exception("Batch size should be same for all input features")
         return batch_sizes[0]
 
     def check_and_add_data(self, inputs, outputs, gts=None, extra_args={}):
-        # inputs = dict(config_handler.InputArgs(**inputs))
+        inputs = dict(config_handler.InputArgs(**inputs))
         if ("id" in inputs) and (inputs["id"] is None):
             del inputs["id"]
         self.batch_size = self.infer_batch_size(inputs)
 
         ids = self.get_data_id(inputs)
         inputs.update({"id": ids})
 
         if self.feat_name_list is None:
             self.feat_name_list = get_feature_names_list(inputs)
 
-        outputs = list(outputs) if outputs is not None else [None] * self.batch_size
         gts = list(gts) if gts is not None else [None] * self.batch_size
         data = inputs
         data.update(
             {
                 "output": list(outputs),
                 "gt": gts,
             }
         )
 
-        # Check for any monitors
+        # Log all the data-points into all_data warehouse
+        add_data_to_warehouse(deepcopy(data), self.path_all_data)
+
+        # Check for any anomalies
         self.check(data, extra_args)
         self.predicted_count += self.batch_size
 
-        if self.log_data:
-            data.update(extra_args)
-            # Log all the data-points into all_data warehouse
-            add_data_to_warehouse(deepcopy(data), self.path_all_data)
-
         # Smartly add data for retraining
         self.smartly_add_data(data, extra_args)
         self.extra_args = extra_args
         return ids
 
     def check(self, data, extra_args={}):
         extra_args.update({"id": data["id"]})
-        self.check_manager.check(
-            data,
+        self.anomaly_manager.check(
+            data["data"],
             data["output"],
             gts=data["gt"],
             extra_args=extra_args,
         )
 
     def is_data_interesting(self, inputs, outputs, gts=None, extra_args={}):
         """A data-point is deemed interesting if the defined signal is positive"""
-        return self.check_manager.is_data_interesting(
+        return self.anomaly_manager.is_data_interesting(
             inputs, outputs, gts=gts, extra_args=extra_args
         )
 
     def set_data_transformation_func(self, func):
         """Attach data transformation func to convert
         logged data-point -> Training dataset"""
         self.dataset_handler.set_transformation_func(func)
@@ -346,36 +306,31 @@
 
         df = pd.read_csv(self.path_all_data)
         gt_id_indices = get_df_indices_from_ids(df, gt_data["id"])
         df.loc[gt_id_indices, "gt"] = np.array(gt_data["gt"], dtype="object")
         df.to_csv(self.path_all_data, index=False)
 
         """
-        TODO: Currently assumes that input is only one column.
-        In some cases, the input might have multiple data
-        structures (e.g., cascaded models).
+        TODO: Currently assumes that input is only one column. 
+        In some cases, the input might have multiple data 
+        structures (e.g., cascaded models). 
         """
         df_gt = df.loc[gt_id_indices]
-        data = dict(
-            zip(
+        data = {
+            "data": zip(
                 self.feat_name_list,
                 [load_list_from_df(df_gt, x) for x in self.feat_name_list],
-            )
-        )
-        data.update(
-            {
-                "output": load_list_from_df(df_gt, "output"),
-                "id": list(gt_data["id"]),
-                "gt": list(gt_data["gt"]),
-            }
-        )
+            ),
+            "output": load_list_from_df(df_gt, "output"),
+            "id": list(gt_data["id"]),
+            "gt": list(gt_data["gt"]),
+        }
         self.check(data, extra_args=self.extra_args)
         self.smartly_add_data(data, extra_args=self.extra_args)
 
-    # TODO: @Vipul - Do we need this?
     def feat_slicing(self, relevant_feat_list, limit_list):
         """
         This function checks anomalies for a subset of data.
         feat_name: Feature on which data slicing is done.
         lower_limit: Lower limit for feature value
         upper_limit: Upper limit for feature value
         """
@@ -398,102 +353,32 @@
         data = {
             "data": load_list_from_df(df_feat, "data"),
             "output": load_list_from_df(df_feat, "output"),
             "id": load_list_from_df(df_feat, "id"),
             "gt": load_list_from_df(df_feat, "gt"),
         }
         self.extra_args.update({"feat_name": feat_name})
-        self.check_manager = CheckManager(self, self.checks)
+        self.anomaly_manager = AnomalyManager(self, self.checks)
         self.check(data, extra_args=self.extra_args)
 
-    def log_measurable(self, ids, vals, col_name):
-        for idx in range(len(ids)):
-            self.cache[col_name].update(
-                {ids[idx]: extract_data_points_from_batch(vals, idx)}
-            )
+    def log_measurable(self, id, val, col_name):
+        data = {"id": [id], col_name: [val]}
+        # add_data_to_warehouse(data, self.path_all_data, row_update=True)
+
+    def log(self, inputs=None, outputs=None, gts=None, identifiers=None, extra=None):
+        if (inputs is not None) and (outputs is None):
+            raise Exception("Predictions should be present while logging inputs")
+        if (inputs is None) and (outputs is not None):
+            raise Exception("Inputs should be present while logging predictions")
+        if (gts is not None) and (identifiers is None):
+            raise Exception("Identifiers should be present while logging ground truths")
+
+        if inputs is not None:
+            identifiers = self.check_and_add_data(inputs, outputs)
 
-    def convert_inputs_table_to_dict(self, inputs):
-        cols = inputs.columns.tolist()
-        ids = inputs.index.tolist()
-        data = {}
-        for col in cols:
-            data.update({col: np.array(list(inputs[col]))})
-        if "id" not in cols:
-            data.update({"id": np.array(ids)})
-        return data
-
-    def convert_dict_values_to_numpy_values(self, inputs: dict) -> dict:
-        data = {}
-        for key, value in inputs.items():
-            data.update({key: np.array(value)})
-        return data
-
-    def log(
-        self,
-        inputs=None,
-        outputs=None,
-        gts=None,
-        identifiers=None,
-        extra=None,
-    ):
-        if self.run_background_log_consumer:
-            data = {
-                "inputs": inputs,
-                "outputs": outputs,
-                "gts": gts,
-                "identifiers": identifiers,
-                "extra": extra,
-            }
-            try:
-                self.msg_queue.put(data)
-            except:
-                print("Model monitoring failed!")
-            # Return identifiers by fetching it from the background thread
-            return
-        else:
-            # if (inputs is not None) and (outputs is None):
-            #     raise Exception("Predictions should be present while logging inputs")
-            if (inputs is None) and (outputs is not None):
-                raise Exception("Inputs should be present while logging predictions")
-            if (gts is not None) and (identifiers is None):
-                raise Exception(
-                    "Identifiers should be present while logging ground truths"
-                )
-
-            if inputs is not None:
-                if isinstance(inputs, pd.DataFrame):
-                    inputs = self.convert_inputs_table_to_dict(inputs)
-                elif isinstance(inputs, dict):
-                    inputs = self.convert_dict_values_to_numpy_values(inputs)
-                else:
-                    raise Exception(
-                        "Inputs was expected to be a Pandas Dataframe or Python Dictionary"
-                    )
-                identifiers = self.check_and_add_data(inputs, outputs)
-
-            if gts is not None:
-                self.attach_ground_truth({"id": identifiers, "gt": gts})
-
-            if self.need_retraining():
-                self.retrain()
-
-            return identifiers
-
-    def clear_cache(self):
-        self.cache = {}
-
-
-def background_log_consumer_task(msg_queue, cfg):
-    framework = Framework(cfg_dict=cfg)
-    # run forever
-    while True:
-        # get the next message
-        data = msg_queue.get()
-
-        # log the message
-        framework.log(
-            inputs=data["inputs"],
-            outputs=data["outputs"],
-            gts=data["gts"],
-            identifiers=data["identifiers"],
-            extra=data["extra"],
-        )
+        if gts is not None:
+            self.attach_ground_truth({"id": identifiers, "gt": gts})
+
+        if self.need_retraining():
+            self.retrain()
+
+        return identifiers
```

### Comparing `uptrain-0.1.0/uptrain/core/classes/helpers/annotation_helper.py` & `uptrain-0.1.dev0/uptrain/core/classes/helpers/annotation_helper.py`

 * *Files identical despite different names*

### Comparing `uptrain-0.1.0/uptrain/core/classes/helpers/config_handler.py` & `uptrain-0.1.dev0/uptrain/core/classes/helpers/config_handler.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,15 +1,12 @@
-from __future__ import annotations
+from pydantic import BaseModel
 import typing
 from datetime import datetime
-
-from pydantic import BaseModel
-import numpy as np
-
 from uptrain.constants import AnnotationMethod
+import numpy as np
 
 
 class AnnotationArgs(BaseModel):
     method: AnnotationMethod
     args: typing.Dict = {}
 
 
@@ -22,47 +19,36 @@
 
 class EvaluationArgs(BaseModel):
     inference_func: typing.Callable = None
     golden_testing_dataset: str = None
     metrics_to_check: typing.List[str] = []
 
 
-class LoggingArgs(BaseModel):
-    slack_webhook_url: str = None
-    dashboard_port: str = None
-    log_folder: str = "uptrain_logs"
-    log_data: bool = True
-    st_logging: bool = False
-    run_background_streamlit: bool = True
-    use_new_handler: bool = False
-
-
 class Config(BaseModel):
     training_args: TrainingArgs = TrainingArgs()
     evaluation_args: EvaluationArgs = EvaluationArgs()
-    logging_args: LoggingArgs = LoggingArgs()
     data_identifier: str = "id"
     checks: typing.List[typing.Dict] = []
     retrain: bool = True
-    retrain_after: int = 100000000000
-    retraining_folder: str = "uptrain_smart_data"
-    data_id: str = "id"
+    retrain_after: int = 250
+    retraining_folder: str = "uptrain_smart_data_" + str(datetime.utcnow())
+    data_id: typing.Literal["id", "utc_timestamp"] = "id"
+    log_folder: str = "uptrain_logs"
+    tb_logging: bool = False
+    st_logging: bool = False
     feat_name_list: list = None
     cluster_visualize_func: typing.Callable = None
-    use_cache: bool = False
-    run_background_log_consumer: bool = False
-    running_ee: bool = False
 
 
-# class InputArgs(BaseModel):
-#     data: dict
-#     id: typing.Optional[typing.Union[list, np.ndarray]]
+class InputArgs(BaseModel):
+    data: dict
+    id: typing.Optional[typing.Union[list, np.ndarray]]
 
-#     class Config:
-#         arbitrary_types_allowed = True
+    class Config:
+        arbitrary_types_allowed = True
 
 
 class GroundTruthArgs(BaseModel):
     gt: typing.Union[np.ndarray, list]
     id: typing.Union[np.ndarray, list]
 
     class Config:
```

### Comparing `uptrain-0.1.0/uptrain/core/classes/helpers/dataset_handler.py` & `uptrain-0.1.dev0/uptrain/core/classes/helpers/dataset_handler.py`

 * *Files 5% similar despite different names*

```diff
@@ -22,18 +22,17 @@
         Calls the Annotation Helper to add gt to retraining dataset
     set_transformation_func(func):
         Attach data transformation func to convert logged data-point -> Training dataset
     set_annotation_method(method):
         Set the annotation method
     """
 
-    def __init__(self, framework=None, cfg=None, transformation_func=(lambda x: x)):
+    def __init__(self, transformation_func=(lambda x: x), cluster_plot_func=None):
         self.transformation_func = transformation_func
-        self.cluster_plot_func = cfg.cluster_visualize_func
-        self.log_handler = framework.log_handler 
+        self.cluster_plot_func = cluster_plot_func
         np.random.seed(10)
 
     def add_annotations(self, dataset):
         """Adds gt to the dataset file by calling appropriate funcs on the annotation helper based on attached annotation method"""
 
         if self.annotation_method == AnnotationMethod.MASTER_FILE:
             annotated_data = self.annotation_helper.annotations_from_master_file(
@@ -73,15 +72,15 @@
         write_json(dataset_location + "/cleaned_dataset.json", new_data)
 
         if self.cluster_plot_func is not None:
             cluster_and_plot_data(
                 np.array([x["kps"] for x in new_data]),
                 9,
                 cluster_plot_func=self.cluster_plot_func,
-                plot_save_name=self.log_handler.get_plot_save_name("collected_edge_cases_clusters.png", "edge_cases"),
+                plot_save_name="collected_edge_cases_clusters.png",
             )
 
         new_data = self.add_annotations(dataset_location + "/cleaned_dataset.json")
         write_json(dataset_location + "/annotated_dataset.json", new_data)
         write_json(
             dataset_location + "/training_dataset.json",
             self.merge_training_datasets(
```

### Comparing `uptrain-0.1.0/uptrain/core/classes/helpers/model_handler.py` & `uptrain-0.1.dev0/uptrain/core/classes/helpers/model_handler.py`

 * *Files identical despite different names*

### Comparing `uptrain-0.1.0/uptrain/core/classes/measurables/__init__.py` & `uptrain-0.1.dev0/uptrain/core/classes/anomalies/measurables/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,13 +1,11 @@
 from .abstract_measurable import AbstractMeasurable
 from .measurable import Measurable
-from .input_feature import InputFeatureMeasurable
-from .feature_concat import FeatureConcatMeasurable
-from .output_feature import OutputFeatureMeasurable
-from .feature import FeatureMeasurable
-from .condition import ConditionMeasurable
-from .custom import CustomMeasurable
-from .accuracy import AccuracyMeasurable, MAEMeasurable, MAPEMeasurable
-from .scalar_from_embedding import ScalarFromEmbeddingMeasurable
-from .distance import DistanceMeasurable
-from .recommendation_hit_rate import RecHitRateMeasurable
+from .input_feature_measurable import InputFeatureMeasurable
+from .output_feature_measurable import OutputFeatureMeasurable
+from .feature_measurable import FeatureMeasurable
+from .condition_measurable import ConditionMeasurable
+from .custom_measurable import CustomMeasurable
+from .accuracy_measurable import AccuracyMeasurable
+from .scalar_from_embedding_measurable import ScalarFromEmbeddingMeasurable
+
 from .measurable_resolver import MeasurableResolver
```

### Comparing `uptrain-0.1.0/uptrain/core/classes/measurables/feature.py` & `uptrain-0.1.dev0/uptrain/core/classes/anomalies/measurables/feature_measurable.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,46 +1,32 @@
-from typing import Any
-
-from uptrain.core.classes.measurables import (
+from uptrain.core.classes.anomalies.measurables import (
     Measurable,
     InputFeatureMeasurable,
     OutputFeatureMeasurable,
 )
 
 
 class FeatureMeasurable(Measurable):
-    """Class that returns a feature as a result of computation."""
-
-    def __init__(self, framework, feature_name, dictn_type: str) -> None:
-        """Constructor for FeatureMeasurable class.
-        
-        Parameters
-        ----------
-        feature_name
-            Name of the feature that is to be measured/evaluated
-        dictn_type
-            Must be "inputs" or "outputs" depending on which feature to
-            measure/evaluate
-        """
+    def __init__(self, framework, feature_name, dictn_type) -> None:
         super().__init__(framework)
         self.feature_name = feature_name
         self.dictn_type = dictn_type
         if self.dictn_type == "inputs":
             self.helper = InputFeatureMeasurable(framework, feature_name)
         elif self.dictn_type == "outputs":
             self.helper = OutputFeatureMeasurable(framework, feature_name)
         else:
             raise Exception(
                 "Helper Measurable not defined for dictionary type %s" % self.dictn_type
             )
 
-    def _compute(self, inputs=None, outputs=None, gts=None, extra=None) -> Any:
+    def _compute(self, inputs=None, outputs=None, gts=None, extra=None) -> any:
         return self.helper._compute(
             inputs=inputs, outputs=outputs, gts=gts, extra=extra
         )
 
-    def col_name(self) -> str:
+    def col_name(self):
         return self.helper.col_name()
 
     # TODO: Decommission and find a generic way
     def extract_val_from_training_data(self, x):
         return self.helper.extract_val_from_training_data(x)
```

### Comparing `uptrain-0.1.0/uptrain/core/classes/measurables/measurable_resolver.py` & `uptrain-0.1.dev0/uptrain/core/classes/anomalies/measurables/measurable_resolver.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,79 +1,45 @@
-from uptrain.core.classes.measurables import (
+from uptrain.core.classes.anomalies.measurables import (
     Measurable,
-    InputFeatureMeasurable,
-    OutputFeatureMeasurable,
     FeatureMeasurable,
-    FeatureConcatMeasurable,
     ConditionMeasurable,
     CustomMeasurable,
     AccuracyMeasurable,
-    MAEMeasurable,
-    MAPEMeasurable,
     ScalarFromEmbeddingMeasurable,
-    DistanceMeasurable,
-    RecHitRateMeasurable,
 )
 from uptrain.constants import MeasurableType
 
 
 class MeasurableResolver:
-    """Class that resolves a measurable key to a measurable class instance."""
-
     def __init__(self, args) -> None:
         super().__init__()
         self._args = args
 
-    def has_valid_resolve_args(self) -> bool:
-        if self._args is None:
-            return False
-        if len(self._args) == 0:
-            return False
-        return True
-
     def resolve(self, framework) -> Measurable:
-        if not self.has_valid_resolve_args():
-            return None
-
         resolve_args = self._args
         measurable_type = resolve_args["type"]
         if measurable_type == MeasurableType.INPUT_FEATURE:
-            return InputFeatureMeasurable(framework, resolve_args["feature_name"])
-        elif measurable_type == MeasurableType.FEATURE_CONCAT:
-            return FeatureConcatMeasurable(framework, resolve_args["feat_name_list"])
+            return FeatureMeasurable(framework, resolve_args["feature_name"], "inputs")
         elif measurable_type == MeasurableType.PREDICTION:
-            return OutputFeatureMeasurable(framework)
+            return FeatureMeasurable(framework, resolve_args["feature_name"], "outputs")
         elif measurable_type == MeasurableType.CUSTOM:
             return CustomMeasurable(framework, resolve_args)
         elif measurable_type == MeasurableType.ACCURACY:
             return AccuracyMeasurable(framework)
-        elif measurable_type == MeasurableType.MAE:
-            return MAEMeasurable(framework)
-        elif measurable_type == MeasurableType.MAPE:
-            return MAPEMeasurable(framework)
         elif measurable_type == MeasurableType.CONDITION_ON_INPUT:
             return ConditionMeasurable(
                 framework,
-                InputFeatureMeasurable(framework, resolve_args["feature_name"]),
+                FeatureMeasurable(framework, resolve_args["feature_name"], "inputs"),
                 resolve_args["condition_args"],
             )
         elif measurable_type == MeasurableType.CONDITION_ON_PREDICTION:
             return ConditionMeasurable(
                 framework,
-                OutputFeatureMeasurable(framework),
+                FeatureMeasurable(framework, resolve_args["feature_name"], "outputs"),
                 resolve_args["condition_args"],
             )
         elif measurable_type == MeasurableType.SCALAR_FROM_EMBEDDING:
             return ScalarFromEmbeddingMeasurable(
                 framework, resolve_args["idx"], resolve_args["extract_from"]
             )
-        elif measurable_type == MeasurableType.DISTANCE:
-            return DistanceMeasurable(
-                framework,
-                resolve_args["base"],
-                resolve_args["reference"],
-                resolve_args["distance_types"],
-            )
-        elif measurable_type == MeasurableType.REC_HIT_RATE:
-            return RecHitRateMeasurable(framework)
         else:
             raise Exception("Resolver not defined")
```

### Comparing `uptrain-0.1.0/uptrain/core/classes/measurables/scalar_from_embedding.py` & `uptrain-0.1.dev0/uptrain/core/classes/anomalies/measurables/scalar_from_embedding_measurable.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,29 +1,30 @@
-from typing import Any
-
-from uptrain.core.classes.measurables import (
+from uptrain.core.classes.anomalies.measurables import (
     Measurable,
     InputFeatureMeasurable,
 )
 
 
 class ScalarFromEmbeddingMeasurable(Measurable):
-    """Class that extracts a scalar from a measurable embedding."""
-
     def __init__(self, framework, idx, extract_from_args) -> None:
         super().__init__(framework)
         self.idx = idx
         self.extract_from = InputFeatureMeasurable(
             framework, extract_from_args["feature_name"]
         )
 
-    def _compute(self, inputs=None, outputs=None, gts=None, extra=None) -> Any:
+    def _compute(self, inputs=None, outputs=None, gts=None, extra=None) -> any:
         return self.extract_from._compute(
             inputs=inputs, outputs=outputs, gts=gts, extra=extra
         )[self.idx]
 
-    def col_name(self) -> str:
-        return f"Scalar [Index: {str(self.idx)}] from Embedding: {str(self.extract_from.col_name())}"
+    def col_name(self):
+        return (
+            "Measurable: Scalar [Index:"
+            + str(self.idx)
+            + "] from Embedding: "
+            + str(self.extract_from.col_name())
+        )
 
     # TODO: Decommission and find a generic way
     def extract_val_from_training_data(self, x):
         return self.extract_from.extract_val_from_training_data(x)[self.idx]
```

### Comparing `uptrain-0.1.0/uptrain/core/classes/monitors/accuracy.py` & `uptrain-0.1.dev0/uptrain/core/classes/anomalies/data_integrity.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,35 +1,49 @@
 import numpy as np
 
-from uptrain.core.classes.monitors import AbstractMonitor
-from uptrain.constants import MeasurableType
-from uptrain.core.classes.measurables import MeasurableResolver
-from uptrain.constants import Monitor
-
-class Accuracy(AbstractMonitor):
-    dashboard_name = "accuracy"
-    monitor_type = Monitor.ACCURACY
-    
-    def base_init(self, fw, check):
-        if check.get("measurable_args", None):
-            self.measurable = MeasurableResolver(check["measurable_args"]).resolve(fw)
-            self.plot_name = check["measurable_args"]['type']
-        else:
-            self.measurable = MeasurableResolver(
-                {"type": MeasurableType.MAE}).resolve(fw)
-        self.abs_err_arr = np.array([])
-        self.avg_acc = 0
-        self.log_handler = fw.log_handler
+from uptrain.core.classes.anomalies import AbstractAnomaly
+from uptrain.core.classes.anomalies.measurables import MeasurableResolver
 
-    def need_ground_truth(self):
-        return True
-    
-    def base_check(self, inputs, outputs, gts=None, extra_args={}):
-        batch_abs_error = self.measurable.compute_and_log(inputs, outputs, gts, extra_args)
-        self.abs_err_arr = np.append(self.abs_err_arr, batch_abs_error)
 
+class DataIntegrity(AbstractAnomaly):
+    dashboard_name = "data_integrity"
+
+    def __init__(self, fw, check):
+        self.log_handler = fw.log_handler
+        self.log_handler.add_writer(self.dashboard_name)
+        self.measurable = MeasurableResolver(check["measurable_args"]).resolve(fw)
+        self.integrity_type = check["integrity_type"]
+        self.threshold = check.get("threshold", None)
+        self.count = 0
+        self.num_issues = 0
+
+    def check(self, inputs, outputs, gts=None, extra_args={}):
+        signal_value = self.measurable.compute_and_log(
+            inputs, outputs, gts=gts, extra=extra_args
+        )
+        if self.integrity_type == "non_null":
+            has_issue = signal_value == None
+        elif self.integrity_type == "less_than":
+            has_issue = signal_value > self.threshold
+        elif self.integrity_type == "greater_than":
+            has_issue = signal_value < self.threshold
+        self.count += len(signal_value)
+        self.num_issues += np.sum(np.array(has_issue))
+        plot_name = (
+            self.measurable.col_name()
+            + " "
+            + self.integrity_type
+            + " "
+            + str(self.threshold)
+        )
         self.log_handler.add_scalars(
-            self.plot_name,
-            {"y_" + self.plot_name: np.mean(self.abs_err_arr)},
-            len(self.abs_err_arr),
+            self.dashboard_name + "_" + plot_name,
+            {plot_name: 1 - self.num_issues / self.count},
+            self.count,
             self.dashboard_name,
-        )
+        )
+
+    def is_data_interesting(self, inputs, outputs, gts=None, extra_args={}):
+        return np.array([False] * len(extra_args["id"]))
+
+    def need_ground_truth(self):
+        return False
```

### Comparing `uptrain-0.1.0/uptrain/core/classes/monitors/data_drift.py` & `uptrain-0.1.dev0/uptrain/core/classes/anomalies/data_drift.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,327 +1,348 @@
 import numpy as np
-import copy
-import pandas as pd
 
-from uptrain.core.classes.monitors import AbstractMonitor
-from uptrain.constants import Monitor
-from uptrain.core.lib.helper_funcs import read_json
-from uptrain.core.lib.algorithms import estimate_earth_moving_cost
-from uptrain.core.classes.measurables import MeasurableResolver
-from uptrain.core.classes.algorithms import Clustering
+from uptrain.core.classes.anomalies import AbstractAnomaly
+from uptrain.constants import DataDriftAlgo
+from uptrain.core.lib.helper_funcs import read_json, cluster_and_plot_data
+from uptrain.core.classes.anomalies.measurables import MeasurableResolver
 
-class DataDrift(AbstractMonitor):
+
+class DataDrift(AbstractAnomaly):
     dashboard_name = "data_drift"
-    monitor_type = Monitor.DATA_DRIFT
     is_embedding = None
     mode = None
     NUM_BUCKETS = 20
-    INITIAL_SKIP = 2000
 
-    def model_choices(self, check):
-        self.is_embedding = check.get('is_embedding', None)
+    def __init__(self, fw, check, is_embedding=None):
+        self.measurable = None
+        self.measurable = MeasurableResolver(check["measurable_args"]).resolve(fw)
+        self.is_embedding = is_embedding
         if self.is_embedding == None:
-            return [{"is_embedding": False}, {"is_embedding": True}]
+            self.embedding_child_class = DataDrift(fw, check, is_embedding=True)
+            self.scalar_child_class = DataDrift(fw, check, is_embedding=False)
         else:
-            return [{"is_embedding": check['is_embedding']}]
-
-    def base_init(self, fw, check):
-        self.reference_dataset = check["reference_dataset"]
-        self.cluster_plot_func = fw.dataset_handler.cluster_plot_func
-        self.save_edge_cases = check.get("save_edge_cases", True)
-        self.NUM_BUCKETS = check.get("num_buckets", self.NUM_BUCKETS)
-        
-        # Also the step in calculating drift
-        self.INITIAL_SKIP = check.get("initial_skip", self.INITIAL_SKIP)
-        self.outlier_idxs = check.get("outlier_idxs", [])
-        self.do_low_density_check = check.get("do_low_density_check", False)
-        self.hover_measurable = MeasurableResolver(check.get("hover_label_args", None)).resolve(fw)
-        self.count = 0
-        self.bucket_labelling_info = {
-            'latest_idxs_added_to_clusters': np.array([None] * self.NUM_BUCKETS),
-            'idxs_closest_to_clusters': np.array([None] * self.NUM_BUCKETS),
-            'closest_idxs_distance': np.array([None] * self.NUM_BUCKETS),
-            'hover_vals_for_reference_clusters': np.array([' '] * self.NUM_BUCKETS),
-            'hover_vals_for_production_clusters': np.array([' '] * self.NUM_BUCKETS)
-        }
-        self.prod_dist_counts_arr = []
-        clustering_args = {
-            "num_buckets": self.NUM_BUCKETS,
-            'is_embedding': self.is_embedding,
-            'plot_save_name': self.log_handler.get_plot_save_name("training_dataset_clusters.png", self.dashboard_name),
-            'cluster_plot_func': self.cluster_plot_func,
-            'find_low_density_regions': self.do_low_density_check
-        }
-        self.clustering_helper = Clustering(clustering_args)
-        if self.is_embedding:
-            self.plot_name = "Embeddings_" + self.measurable.col_name()
-            self.emd_threshold = check.get("emd_threshold", 1)
-        else:
-            self.plot_name = "Scalar_" + self.measurable.col_name()
-        self.bucket_reference_dataset()
-        self.outliers = check.get("outlier_data", [])
-        if len(self.outliers):
-            self.outliers = np.array(self.outliers) / self.max_along_axis
+            self.log_handler = fw.log_handler
+            self.reference_dataset = check["reference_dataset"]
+            self.cluster_plot_func = fw.dataset_handler.cluster_plot_func
+            self.save_edge_cases = check.get("save_edge_cases", True)
+            self.count = 0
+            self.prod_dist_counts_arr = []
+            self.bucket_reference_dataset()
 
     def need_ground_truth(self):
         return False
 
     def check(self, inputs, outputs, gts=None, extra_args={}):
-        if len(self.children) > 0:
-            feats = self.measurable.compute_and_log(
-                inputs=inputs, outputs=outputs, gts=gts, extra=extra_args
-            )
-            if sum(list(feats.shape)[1:])/max(1,len(list(feats.shape)[1:])) <= 1:
-                self.children = [self.children[0]]
-            [x.check(inputs, outputs, gts=gts, extra_args=extra_args) for x in self.children]
+        if self.is_embedding == None:
+            if self.mode == "check_both":
+                self.embedding_child_class.check(
+                    inputs, outputs, gts=gts, extra_args=extra_args
+                )
+                self.scalar_child_class.check(
+                    inputs, outputs, gts=gts, extra_args=extra_args
+                )
+            elif self.mode == "check_scalar_only":
+                self.scalar_child_class.check(
+                    inputs, outputs, gts=gts, extra_args=extra_args
+                )
+            elif self.mode == "check_embeddings_only":
+                self.scalar_child_class.check(
+                    inputs, outputs, gts=gts, extra_args=extra_args
+                )
+            else:
+                feats = self.measurable.compute_and_log(
+                    inputs=inputs, outputs=outputs, gts=gts, extra=extra_args
+                )
+                if len(list(feats.shape)) > 2:
+                    self.mode = "check_both"
+                else:
+                    self.mode = "check_scalar_only"
+                self.check(inputs, outputs, gts=gts, extra_args=extra_args)
         else:
+            if self.count == 0:
+                self.log_handler.add_writer(self.dashboard_name)
+
             self.count += len(extra_args["id"])
 
             self.feats = self.measurable.compute_and_log(
                 inputs=inputs, outputs=outputs, gts=gts, extra=extra_args
             )
             feats_shape = list(self.feats.shape)
             feats_shape.insert(1, 1)
             if len(feats_shape) == 2:
                 feats_shape.insert(2, 1)
             self.feats = np.reshape(self.feats, tuple(feats_shape))
 
             if self.is_embedding:
-                self.feats = self.feats / np.expand_dims(self.max_along_axis, 0)
-
-            self.this_datapoint_cluster, self.prod_dist_counts = self.clustering_helper.infer_cluster_assignment(self.feats, self.prod_dist_counts)
-            #TODO: Extend for feature-wise clusters
-            if (self.hover_measurable is not None) and self.is_embedding:
-                hover_measurable_vals = np.array(self.hover_measurable.compute_and_log(
-                    inputs=inputs, outputs=outputs, gts=gts, extra=extra_args
-                ))
-                uniq_clusters, uniq_indexs = np.unique(self.this_datapoint_cluster, return_index=True)
-                query_indexs = np.zeros(self.NUM_BUCKETS)
-                self.bucket_labelling_info['latest_idxs_added_to_clusters'][uniq_clusters] = uniq_indexs
-                query_indexs[uniq_clusters] = uniq_indexs
-                query_indexs = np.array(query_indexs, dtype=int)
-                self.bucket_labelling_info['hover_vals_for_production_clusters'] = hover_measurable_vals[query_indexs]
-
-            self.prod_dist_counts_arr.append(self.prod_dist_counts.copy())
-
-            self.prod_dist = (
-                self.prod_dist_counts_arr[-1]
-                - self.prod_dist_counts_arr[
-                    int(max(self.count - self.INITIAL_SKIP, 0) / len(extra_args["id"]))
-                ]
-            ) / min(self.count, self.INITIAL_SKIP)
-
-            if self.ref_dist.shape[0] == 1:
-                if self.is_embedding:
-                    bar_graph_buckets = ["cluster_" + str(idx) for idx in range(len(list(np.reshape(self.clusters,-1))))]
-                else:
-                    bar_graph_buckets = list(np.reshape(self.clusters,-1))
-
-                self.log_handler.add_bar_graphs(
-                    self.plot_name,
-                    {
-                        "reference": dict(zip(bar_graph_buckets, list(np.reshape(np.array(self.ref_dist[0]), -1)))),
-                        "production": dict(zip(bar_graph_buckets, list(np.reshape(np.array(self.prod_dist[0]), -1)))),
-                    },
-                    self.dashboard_name,
-                    hover_data = {
-                        "reference": dict(zip(bar_graph_buckets, list(self.bucket_labelling_info['hover_vals_for_reference_clusters']))),
-                        "production": dict(zip(bar_graph_buckets, list(self.bucket_labelling_info['hover_vals_for_production_clusters'])))
-                    }
+                selected_cluster = np.argmin(
+                    np.sum(
+                        np.abs(self.clusters[0] - self.feats),
+                        axis=tuple(range(2, len(feats_shape))),
+                    ),
+                    axis=1,
                 )
+                for clus in selected_cluster:
+                    self.prod_dist_counts[0][clus] += 1
+                self.this_datapoint_cluster = selected_cluster
+                self.prod_dist_counts_arr.append(self.prod_dist_counts.copy())
+            else:
+                this_datapoint_cluster = []
+                for idx in range(self.feats.shape[2]):
+                    bucket_idx = np.searchsorted(
+                        self.buckets[idx], self.feats[:, :, idx]
+                    )[:, 0]
+                    this_datapoint_cluster.append(bucket_idx)
+                    self.prod_dist_counts[idx][bucket_idx] += 1
+                self.prod_dist_counts_arr.append(self.prod_dist_counts.copy())
+                self.this_datapoint_cluster = np.array(this_datapoint_cluster)
 
-            if self.count < self.INITIAL_SKIP:
+            if self.count < 1000:
                 self.drift_detected = False
                 return
             else:
+                self.prod_dist = (
+                    self.prod_dist_counts_arr[-1]
+                    - self.prod_dist_counts_arr[
+                        int(max(self.count - 2000, 0) / len(extra_args["id"]))
+                    ]
+                ) / min(self.count, 2000)
                 self.psis = np.zeros(self.ref_dist.shape[0])
                 self.costs = np.zeros(self.ref_dist.shape[0])
                 drift_detected = False
                 for idx in range(self.ref_dist.shape[0]):
                     if self.is_embedding:
-                        self.costs[idx] = estimate_earth_moving_cost(
+                        self.costs[idx] = self.estimate_earth_moving_cost(
                             self.prod_dist[idx], self.ref_dist[idx], self.clusters[idx]
                         )
-                        drift_detected = drift_detected or (self.costs[idx] > self.emd_threshold)
+                        drift_detected = drift_detected or (self.costs[idx] > 300)
                     else:
                         this_psi = sum(
                             [
                                 (self.prod_dist[idx][jdx] - self.ref_dist[idx][jdx])
                                 * np.log(
                                     max(self.prod_dist[idx][jdx], 0.0001)
                                     / self.ref_dist[idx][jdx]
                                 )
                                 for jdx in range(self.ref_dist.shape[1])
                             ]
                         )
                         self.psis[idx] = this_psi
                         drift_detected = drift_detected or (this_psi > 0.3)
                 self.drift_detected = drift_detected
-                if self.drift_detected:
-                    alert = "Data Drift last detected at " + str(self.count) + " for Embeddings with Earth moving distance = " + str(float(self.costs[0]))
-                    self.log_handler.add_alert(
-                        "Data Drift Alert 🚨",
-                        alert,
-                        self.dashboard_name
-                    )
 
             if self.is_embedding:
                 dict_emc = dict(
                     zip(
-                        ["y_" + self.measurable.col_name() for x in range(self.costs.shape[0])],
+                        ["feat_" + str(x) for x in range(self.costs.shape[0])],
                         [float(x) for x in list(self.costs)],
                     )
                 )
-                # dict_emc.update({"threshold": self.emd_threshold})
+                dict_emc.update({"threshold": 300})
                 self.log_handler.add_scalars(
-                    self.measurable.col_name() + " - earth_moving_costs",
+                    self.measurable.col_name() + " - earth_moving_costs_embedding",
                     dict_emc,
                     self.count,
                     self.dashboard_name,
-                    file_name="embeddings"
-                )
-                self.log_handler.add_scalars(
-                    self.measurable.col_name() + " - earth_moving_costs",
-                    {list(dict_emc.keys())[0]: self.emd_threshold},
-                    self.count,
-                    self.dashboard_name,
-                    file_name="threshold"
                 )
             else:
                 dict_psi = dict(
                     zip(
-                        ["y_" + self.measurable.col_name() + "_" + str(x) for x in range(self.psis.shape[0])],
+                        ["feat_" + str(x) for x in range(self.psis.shape[0])],
                         [float(x) for x in list(self.psis)],
                     )
                 )
                 dict_psi.update({"threshold": 0.3})
                 self.log_handler.add_scalars(
                     self.measurable.col_name() + " - population_stability_index_scalar",
                     dict_psi,
                     self.count,
                     self.dashboard_name,
                 )
 
-    def base_is_data_interesting(self, inputs, outputs, gts=None, extra_args={}):
-        is_interesting = np.array([False] * len(extra_args["id"]))
-        reasons = ["None"] * len(extra_args["id"])
-
-        if self.do_low_density_check and (len(self.low_density_regions) > 0):
-            dists_from_low_density_regions = np.min(np.sum(np.abs(self.feats - np.expand_dims(self.low_density_regions, axis=0)),axis=2),axis=1)
-            min_cluster_var = np.min(self.cluster_vars)
-            is_close = dists_from_low_density_regions < min_cluster_var
-            is_interesting = np.logical_or(is_close, is_interesting)
-            for lkdx in range(len(is_close)):
-                if is_close[lkdx]:
-                    reasons[lkdx] = "Lies_to_Low_Density_Regions_In_Training_Distribution"
-
-        if len(self.outliers):
-            dists_from_outliers = np.min(np.sum(np.abs(self.feats - np.expand_dims(self.outliers, axis=0)),axis=2),axis=1)
-            min_cluster_var = np.min(self.cluster_vars)
-            is_close = dists_from_outliers < 0.5 * min_cluster_var
-            is_interesting = np.logical_or(is_close, is_interesting)
-            for lkdx in range(len(is_close)):
-                if is_close[lkdx]:
-                    if dists_from_outliers[lkdx] < 0.0000001:
-                        reasons[lkdx] = "Outlier_annotated_by_the_user"
-                    else:
-                        reasons[lkdx] = "Close_to_User_annotated_Outliers"
-
-        if self.save_edge_cases and self.drift_detected and not isinstance(self.feats[0,0,0], str):
-            feats_shape = list(self.feats.shape)
-            del feats_shape[1]
-            self.feats = np.reshape(self.feats, tuple(feats_shape))
-            for idx in range(self.ref_dist.shape[0]):
-                if self.is_embedding:
-                    dist_from_cluster = (
-                        np.sum(
-                            np.abs(
-                                self.clusters[idx][self.this_datapoint_cluster]
-                                - self.feats
-                            ),
-                            axis=tuple(range(1, len(feats_shape))),
+    def is_data_interesting(self, inputs, outputs, gts=None, extra_args={}):
+        if self.is_embedding == None:
+            if self.mode == "check_both":
+                arr1 = self.embedding_child_class.is_data_interesting(
+                    inputs, outputs, gts=gts, extra_args=extra_args
+                )
+                arr2 = self.scalar_child_class.is_data_interesting(
+                    inputs, outputs, gts=gts, extra_args=extra_args
+                )
+                return np.logical_or(np.array(arr1), np.array(arr2))
+            elif self.mode == "check_scalar_only":
+                return self.scalar_child_class.is_data_interesting(
+                    inputs, outputs, gts=gts, extra_args=extra_args
+                )
+            elif self.mode == "check_embeddings_only":
+                return self.scalar_child_class.is_data_interesting(
+                    inputs, outputs, gts=gts, extra_args=extra_args
+                )
+            else:
+                raise Exception("Mode for data drift should be set in check func")
+        else:
+            is_interesting = np.array([False] * len(extra_args["id"]))
+            if self.save_edge_cases and self.drift_detected:
+                feats_shape = list(self.feats.shape)
+                del feats_shape[1]
+                self.feats = np.reshape(self.feats, tuple(feats_shape))
+                for idx in range(self.ref_dist.shape[0]):
+                    if self.is_embedding:
+                        dist_from_cluster = (
+                            np.sum(
+                                np.abs(
+                                    self.clusters[idx][self.this_datapoint_cluster]
+                                    - self.feats
+                                ),
+                                axis=tuple(range(1, len(feats_shape))),
+                            )
+                            / self.cluster_vars[idx][self.this_datapoint_cluster]
                         )
-                        / self.cluster_vars[idx][self.this_datapoint_cluster]
-                    )
-                else:
-                    dist_from_cluster = np.abs(
-                        np.reshape(
-                            self.clusters[idx][self.this_datapoint_cluster[idx]], -1
+                    else:
+                        dist_from_cluster = np.abs(
+                            np.reshape(
+                                self.clusters[idx][self.this_datapoint_cluster[idx]], -1
+                            )
+                            - self.feats[:, idx]
+                        ) / np.reshape(
+                            self.cluster_vars[idx][self.this_datapoint_cluster[idx]], -1
                         )
-                        - self.feats[:, idx]
-                    ) / np.reshape(
-                        self.cluster_vars[idx][self.this_datapoint_cluster[idx]], -1
-                    )
-                for jdx in range(dist_from_cluster.shape[0]):
-                    if dist_from_cluster[jdx] > 2:
-                        if self.is_embedding:
-                            min_dist_from_clusters = np.min(
-                                np.sum(
-                                    np.abs(self.clusters[idx] - self.feats[jdx]),
-                                    axis=tuple(range(1, len(feats_shape))),
+                    for jdx in range(dist_from_cluster.shape[0]):
+                        if dist_from_cluster[jdx] > 2:
+                            if self.is_embedding:
+                                min_dist_from_clusters = np.min(
+                                    np.sum(
+                                        np.abs(self.clusters[idx] - self.feats[jdx]),
+                                        axis=tuple(range(1, len(feats_shape))),
+                                    )
+                                    / self.cluster_vars[idx]
                                 )
-                                / self.cluster_vars[idx]
-                            )
-                        else:
-                            min_dist_from_clusters = np.min(
-                                np.abs(
-                                    np.reshape(self.clusters[idx], -1)
-                                    - self.feats[jdx, idx]
+                            else:
+                                min_dist_from_clusters = np.min(
+                                    np.abs(
+                                        np.reshape(self.clusters[idx], -1)
+                                        - self.feats[jdx, idx]
+                                    )
+                                    / np.reshape(self.cluster_vars[idx], -1)
                                 )
-                                / np.reshape(self.cluster_vars[idx], -1)
+                            is_interesting[jdx] = is_interesting[jdx] or (
+                                min_dist_from_clusters > 1
                             )
-                        is_interesting[jdx] = is_interesting[jdx] or (
-                            min_dist_from_clusters > 1
-                        )
-                        if min_dist_from_clusters > 1:
-                            reasons[jdx] = "Away_from_all_training_clusters"
-
-        return is_interesting, reasons
+            return is_interesting
 
+    def estimate_earth_moving_cost(self, prod_dist, ref_dist, clusters):
+        cost = 0
+        for jdx in range(self.ref_dist.shape[1]):
+            dirt_required = prod_dist[jdx] - ref_dist[jdx]
+            dictn = []
+            for kdx in range(self.clusters.shape[1]):
+                if jdx == kdx:
+                    dirt_can_be_transported = 0
+                else:
+                    dirt_can_be_transported = prod_dist[kdx] - ref_dist[kdx]
+                this_dirt = -dirt_can_be_transported
+                if this_dirt * dirt_required < 0:
+                    cost_per_dirt = 1000000000
+                else:
+                    cost_per_dirt = np.sum(np.abs(clusters[kdx] - clusters[jdx]))
+                dictn.append(
+                    {
+                        "dirt": np.abs(this_dirt),
+                        "idx": kdx,
+                        "cost_per_dirt": cost_per_dirt,
+                    }
+                )
+            dictn = sorted(dictn, key=lambda x: x["cost_per_dirt"])
+            this_cost = 0
+            dirt_required = np.abs(dirt_required)
+            for kdx in range(len(dictn)):
+                if dirt_required > 0:
+                    this_cost += (
+                        min(dictn[kdx]["dirt"], dirt_required)
+                        * dictn[kdx]["cost_per_dirt"]
+                    )
+                    dirt_required -= min(dictn[kdx]["dirt"], dirt_required)
+                else:
+                    break
+            cost += this_cost
+        return cost
 
     def bucket_reference_dataset(self):
         self.ref_dist = []
         self.prod_dist = []
         self.ref_dist_counts = []
         self.prod_dist_counts = []
-        if self.reference_dataset.split('.')[-1] == 'json':
-            data = read_json(self.reference_dataset)
-            all_inputs = np.array(
-                [self.measurable.extract_val_from_training_data(x) for x in data]
-            )
-        elif self.reference_dataset.split('.')[-1] == 'csv':
-            data = pd.read_csv(self.reference_dataset).to_dict()
-            for key in data:
-                data[key] = list(data[key].values())
-            all_inputs = np.array(self.measurable.extract_val_from_training_data(data))
-        else:
-            raise Exception("Reference data file type not recognized.")
-        
+        data = read_json(self.reference_dataset)
+        all_inputs = np.array(
+            [self.measurable.extract_val_from_training_data(x) for x in data]
+        )
         all_inputs_shape = list(all_inputs.shape)
         if len(all_inputs_shape) == 1:
             all_inputs_shape.insert(1, 1)
             all_inputs = np.reshape(all_inputs, all_inputs_shape)
 
-        clustering_results = self.clustering_helper.cluster_data(all_inputs)
-
-        self.buckets = np.array(clustering_results['buckets'])
-        self.clusters = np.array(clustering_results['clusters'])
-        self.cluster_vars = np.array(clustering_results['cluster_vars'])
-
-        self.ref_dist = np.array(clustering_results['dist'])
-        self.ref_dist_counts = np.array(clustering_results['dist_counts'])
-        self.max_along_axis = clustering_results['max_along_axis']
-        self.low_density_regions = clustering_results['low_density_regions']
-
-        if self.hover_measurable is not None:
-            all_hover_vals = np.array(
-                [self.hover_measurable.extract_val_from_training_data(x) for x in data]
-            )
-            hover_label_idxs = [x[0] for x in list(clustering_results['idxs_closest_to_cluster_centroids'].values())]
-            self.bucket_labelling_info['hover_vals_for_reference_clusters'] = all_hover_vals[hover_label_idxs]
-
-        self.prod_dist = np.zeros(self.ref_dist.shape)
-        self.prod_dist_counts = np.zeros(self.ref_dist_counts.shape)
-
-        self.prod_dist_counts_arr.append(copy.deepcopy(self.prod_dist_counts))
-        if len(self.outlier_idxs):
-            self.outliers = all_inputs[np.array(self.outlier_idxs)]
+        if self.is_embedding:
+            self.bucket_vector(all_inputs)
+        else:
+            buckets = []
+            clusters = []
+            cluster_vars = []
+            for idx in range(all_inputs.shape[1]):
+                this_inputs = all_inputs[:, idx]
+                this_buckets, this_clusters, this_cluster_vars = self.bucket_scalar(
+                    this_inputs
+                )
+                buckets.append(this_buckets)
+                clusters.append(this_clusters)
+                cluster_vars.append(this_cluster_vars)
+            self.buckets = np.array(buckets)
+            self.clusters = np.array(clusters)
+            self.cluster_vars = np.array(cluster_vars)
+
+        self.ref_dist = np.array(self.ref_dist)
+        self.ref_dist_counts = np.array(self.ref_dist_counts)
+        self.prod_dist = np.array(self.prod_dist)
+        self.prod_dist_counts = np.array(self.prod_dist_counts)
+
+    def bucket_scalar(self, arr):
+        sorted_arr = np.sort(arr)
+        buckets = []
+        clusters = []
+        cluster_vars = []
+        for idx in range(0, self.NUM_BUCKETS):
+            if idx > 0:
+                buckets.append(
+                    sorted_arr[int(idx * (len(sorted_arr) - 1) / self.NUM_BUCKETS)]
+                )
+            this_bucket_elems = sorted_arr[
+                int((idx) * (len(sorted_arr) - 1) / self.NUM_BUCKETS) : int(
+                    (idx + 1) * (len(sorted_arr) - 1) / self.NUM_BUCKETS
+                )
+            ]
+            gaussian_mean = np.mean(this_bucket_elems)
+            gaussian_var = np.var(this_bucket_elems)
+            clusters.append([gaussian_mean])
+            cluster_vars.append([gaussian_var])
+
+        self.ref_dist.append([[1 / self.NUM_BUCKETS] for x in range(self.NUM_BUCKETS)])
+        self.ref_dist_counts.append(
+            [[int(len(sorted_arr) / self.NUM_BUCKETS)] for x in range(self.NUM_BUCKETS)]
+        )
+        self.prod_dist.append([[0] for x in range(self.NUM_BUCKETS)])
+        self.prod_dist_counts.append([[0] for x in range(self.NUM_BUCKETS)])
+        return np.array(buckets), np.array(clusters), np.array(cluster_vars)
+
+    def bucket_vector(self, data):
+
+        all_clusters, counts, cluster_vars = cluster_and_plot_data(
+            data,
+            self.NUM_BUCKETS,
+            cluster_plot_func=self.cluster_plot_func,
+            plot_save_name="training_dataset_clusters.png",
+        )
+
+        self.clusters = np.array([all_clusters])
+        self.cluster_vars = np.array([cluster_vars])
+
+        self.ref_dist_counts = np.array([counts])
+        self.ref_dist = self.ref_dist_counts / data.shape[0]
+        self.prod_dist = np.zeros((1, self.NUM_BUCKETS))
+        self.prod_dist_counts = np.zeros((1, self.NUM_BUCKETS))
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `uptrain-0.1.0/uptrain/core/classes/monitors/model_bias.py` & `uptrain-0.1.dev0/uptrain/core/classes/anomalies/recommendation_bias.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,29 +1,34 @@
 import numpy as np
 
-from uptrain.core.classes.monitors import AbstractMonitor
+from uptrain.core.classes.anomalies import AbstractAnomaly
 from uptrain.core.classes.algorithms import PopularityBias
-from uptrain.constants import BiasAlgo, Monitor
+from uptrain.constants import BiasAlgo
 
 
-class ModelBias(AbstractMonitor):
-    dashboard_name = "popularity_bias"
-    monitor_type = Monitor.POPULARITY_BIAS
+class RecommendationBias(AbstractAnomaly):
+    dashboard_name = "pop_bias"
 
-    def base_init(self, fw, check):
+    def __init__(self, fw, check):
+        self.log_handler = fw.log_handler
+        self.log_handler.add_writer(self.dashboard_name)
         self.acc_arr = []
         if check["algorithm"] == BiasAlgo.POPULARITY_BIAS:
-            sessions = check.get("sessions", None)
-            self.algo = PopularityBias(sessions)
+            rec_list = check.get("rec_list", None)
+            pop_map = check.get("pop_map", None)
+            self.algo = PopularityBias(rec_list, pop_map)
         else:
-            raise Exception("Model bias type not supported")
+            raise Exception("Recommendation bias type not supported")
 
     def need_ground_truth(self):
         return False
 
-    def base_check(self, inputs, outputs, gts=None, extra_args={}):
+    def check(self, inputs, outputs, gts=None, extra_args={}):
         for y_pred in outputs:
-            self.algo.add_prediction(y_pred)
+            self.algo.add_prediction([y_pred])
             pop_arr = self.algo.all_popularity
             self.log_handler.add_histogram(
                 "popularity_bias", pop_arr, self.dashboard_name
             )
+
+    def is_data_interesting(self, inputs, outputs, gts=None, extra_args={}):
+        return np.array([False] * len(extra_args["id"]))
```

### Comparing `uptrain-0.1.0/uptrain/core/classes/signals/signal.py` & `uptrain-0.1.dev0/uptrain/core/classes/anomalies/signals/signal.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 import numpy as np
-import json_fix
 
 from uptrain.constants import MODEL_SIGNAL_TO_FN_MAPPING
 
 
 class Signal:
     """
     Signal Class to identify edge cases
@@ -34,17 +33,14 @@
                     "Evalution fn for signal: %s is not defined in constants" % name
                 )
             fn = MODEL_SIGNAL_TO_FN_MAPPING[name]
         self.fn = fn
         self.extra_args = extra_args
         self.children = []
 
-    def __json__(self):
-        return {"feature_name": str(self)}
-
     def base_evaluate(self, inputs, outputs, gts=None, extra_args={}):
         extra_args.update(self.extra_args)
         if self.fn is None:
             raise Exception("Evalution fn not defined for signal: ", self.name)
         return self.fn(inputs, outputs, gts=gts, extra_args=extra_args)
 
     def evaluate(self, inputs, outputs, gts=None, extra_args={}):
```

### Comparing `uptrain-0.1.0/uptrain/core/classes/signals/signal_manager.py` & `uptrain-0.1.dev0/uptrain/core/classes/anomalies/signals/signal_manager.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from uptrain.core.classes.signals import Signal
+from uptrain.core.classes.anomalies.signals import Signal
 from uptrain.constants import ModelSignal
 
 
 class SignalManager:
     """
     Manager class to help with signal evalutions
```

### Comparing `uptrain-0.1.0/uptrain/core/lib/model_signal_funcs.py` & `uptrain-0.1.dev0/uptrain/core/lib/model_signal_funcs.py`

 * *Files identical despite different names*

