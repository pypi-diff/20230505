# Comparing `tmp/autogluon.timeseries-0.7.1b20230504.tar.gz` & `tmp/autogluon.timeseries-0.7.1b20230505.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "autogluon.timeseries-0.7.1b20230504.tar", last modified: Thu May  4 09:04:28 2023, max compression
+gzip compressed data, was "autogluon.timeseries-0.7.1b20230505.tar", last modified: Fri May  5 09:04:37 2023, max compression
```

## Comparing `autogluon.timeseries-0.7.1b20230504.tar` & `autogluon.timeseries-0.7.1b20230505.tar`

### file list

```diff
@@ -1,73 +1,73 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:04:28.219674 autogluon.timeseries-0.7.1b20230504/
--rw-r--r--   0 runner    (1001) docker     (123)    12593 2023-05-04 09:04:28.219674 autogluon.timeseries-0.7.1b20230504/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-04 09:04:28.219674 autogluon.timeseries-0.7.1b20230504/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2245 2023-05-04 09:03:46.000000 autogluon.timeseries-0.7.1b20230504/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:04:28.199674 autogluon.timeseries-0.7.1b20230504/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:04:28.203674 autogluon.timeseries-0.7.1b20230504/src/autogluon/
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-05-04 09:03:46.000000 autogluon.timeseries-0.7.1b20230504/src/autogluon/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:04:28.207674 autogluon.timeseries-0.7.1b20230504/src/autogluon/timeseries/
--rw-r--r--   0 runner    (1001) docker     (123)      867 2023-05-04 09:03:46.000000 autogluon.timeseries-0.7.1b20230504/src/autogluon/timeseries/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:04:28.207674 autogluon.timeseries-0.7.1b20230504/src/autogluon/timeseries/configs/
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-05-04 09:03:46.000000 autogluon.timeseries-0.7.1b20230504/src/autogluon/timeseries/configs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      638 2023-05-04 09:03:46.000000 autogluon.timeseries-0.7.1b20230504/src/autogluon/timeseries/configs/presets_configs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:04:28.211674 autogluon.timeseries-0.7.1b20230504/src/autogluon/timeseries/dataset/
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-05-04 09:03:46.000000 autogluon.timeseries-0.7.1b20230504/src/autogluon/timeseries/dataset/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    37170 2023-05-04 09:03:46.000000 autogluon.timeseries-0.7.1b20230504/src/autogluon/timeseries/dataset/ts_dataframe.py
--rw-r--r--   0 runner    (1001) docker     (123)    11293 2023-05-04 09:03:46.000000 autogluon.timeseries-0.7.1b20230504/src/autogluon/timeseries/evaluator.py
--rw-r--r--   0 runner    (1001) docker     (123)    10081 2023-05-04 09:03:46.000000 autogluon.timeseries-0.7.1b20230504/src/autogluon/timeseries/learner.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:04:28.211674 autogluon.timeseries-0.7.1b20230504/src/autogluon/timeseries/models/
--rw-r--r--   0 runner    (1001) docker     (123)      676 2023-05-04 09:03:46.000000 autogluon.timeseries-0.7.1b20230504/src/autogluon/timeseries/models/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:04:28.211674 autogluon.timeseries-0.7.1b20230504/src/autogluon/timeseries/models/abstract/
--rw-r--r--   0 runner    (1001) docker     (123)      168 2023-05-04 09:03:46.000000 autogluon.timeseries-0.7.1b20230504/src/autogluon/timeseries/models/abstract/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    19723 2023-05-04 09:03:46.000000 autogluon.timeseries-0.7.1b20230504/src/autogluon/timeseries/models/abstract/abstract_timeseries_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     3735 2023-05-04 09:03:46.000000 autogluon.timeseries-0.7.1b20230504/src/autogluon/timeseries/models/abstract/model_trial.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:04:28.211674 autogluon.timeseries-0.7.1b20230504/src/autogluon/timeseries/models/autogluon_tabular/
--rw-r--r--   0 runner    (1001) docker     (123)      168 2023-05-04 09:03:46.000000 autogluon.timeseries-0.7.1b20230504/src/autogluon/timeseries/models/autogluon_tabular/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12707 2023-05-04 09:03:46.000000 autogluon.timeseries-0.7.1b20230504/src/autogluon/timeseries/models/autogluon_tabular/mlforecast.py
--rw-r--r--   0 runner    (1001) docker     (123)    17282 2023-05-04 09:03:46.000000 autogluon.timeseries-0.7.1b20230504/src/autogluon/timeseries/models/autogluon_tabular/tabular_model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:04:28.211674 autogluon.timeseries-0.7.1b20230504/src/autogluon/timeseries/models/ensemble/
--rw-r--r--   0 runner    (1001) docker     (123)      128 2023-05-04 09:03:46.000000 autogluon.timeseries-0.7.1b20230504/src/autogluon/timeseries/models/ensemble/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2733 2023-05-04 09:03:46.000000 autogluon.timeseries-0.7.1b20230504/src/autogluon/timeseries/models/ensemble/abstract_timeseries_ensemble.py
--rw-r--r--   0 runner    (1001) docker     (123)     5902 2023-05-04 09:03:46.000000 autogluon.timeseries-0.7.1b20230504/src/autogluon/timeseries/models/ensemble/greedy_ensemble.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:04:28.215674 autogluon.timeseries-0.7.1b20230504/src/autogluon/timeseries/models/gluonts/
--rw-r--r--   0 runner    (1001) docker     (123)      174 2023-05-04 09:03:46.000000 autogluon.timeseries-0.7.1b20230504/src/autogluon/timeseries/models/gluonts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18915 2023-05-04 09:03:46.000000 autogluon.timeseries-0.7.1b20230504/src/autogluon/timeseries/models/gluonts/abstract_gluonts.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:04:28.215674 autogluon.timeseries-0.7.1b20230504/src/autogluon/timeseries/models/gluonts/mx/
--rw-r--r--   0 runner    (1001) docker     (123)      932 2023-05-04 09:03:46.000000 autogluon.timeseries-0.7.1b20230504/src/autogluon/timeseries/models/gluonts/mx/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4053 2023-05-04 09:03:46.000000 autogluon.timeseries-0.7.1b20230504/src/autogluon/timeseries/models/gluonts/mx/callback.py
--rw-r--r--   0 runner    (1001) docker     (123)    22893 2023-05-04 09:03:46.000000 autogluon.timeseries-0.7.1b20230504/src/autogluon/timeseries/models/gluonts/mx/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:04:28.215674 autogluon.timeseries-0.7.1b20230504/src/autogluon/timeseries/models/gluonts/torch/
--rw-r--r--   0 runner    (1001) docker     (123)      190 2023-05-04 09:03:46.000000 autogluon.timeseries-0.7.1b20230504/src/autogluon/timeseries/models/gluonts/torch/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13902 2023-05-04 09:03:46.000000 autogluon.timeseries-0.7.1b20230504/src/autogluon/timeseries/models/gluonts/torch/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:04:28.215674 autogluon.timeseries-0.7.1b20230504/src/autogluon/timeseries/models/local/
--rw-r--r--   0 runner    (1001) docker     (123)      192 2023-05-04 09:03:46.000000 autogluon.timeseries-0.7.1b20230504/src/autogluon/timeseries/models/local/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6980 2023-05-04 09:03:46.000000 autogluon.timeseries-0.7.1b20230504/src/autogluon/timeseries/models/local/abstract_local_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     4123 2023-05-04 09:03:46.000000 autogluon.timeseries-0.7.1b20230504/src/autogluon/timeseries/models/local/naive.py
--rw-r--r--   0 runner    (1001) docker     (123)    12222 2023-05-04 09:03:46.000000 autogluon.timeseries-0.7.1b20230504/src/autogluon/timeseries/models/local/statsforecast.py
--rw-r--r--   0 runner    (1001) docker     (123)    15697 2023-05-04 09:03:46.000000 autogluon.timeseries-0.7.1b20230504/src/autogluon/timeseries/models/local/statsmodels.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:04:28.215674 autogluon.timeseries-0.7.1b20230504/src/autogluon/timeseries/models/multi_window/
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-05-04 09:03:46.000000 autogluon.timeseries-0.7.1b20230504/src/autogluon/timeseries/models/multi_window/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9000 2023-05-04 09:03:46.000000 autogluon.timeseries-0.7.1b20230504/src/autogluon/timeseries/models/multi_window/multi_window_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     9947 2023-05-04 09:03:46.000000 autogluon.timeseries-0.7.1b20230504/src/autogluon/timeseries/models/presets.py
--rw-r--r--   0 runner    (1001) docker     (123)    46742 2023-05-04 09:03:46.000000 autogluon.timeseries-0.7.1b20230504/src/autogluon/timeseries/predictor.py
--rw-r--r--   0 runner    (1001) docker     (123)     9252 2023-05-04 09:03:46.000000 autogluon.timeseries-0.7.1b20230504/src/autogluon/timeseries/splitter.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:04:28.219674 autogluon.timeseries-0.7.1b20230504/src/autogluon/timeseries/trainer/
--rw-r--r--   0 runner    (1001) docker     (123)      170 2023-05-04 09:03:46.000000 autogluon.timeseries-0.7.1b20230504/src/autogluon/timeseries/trainer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    41049 2023-05-04 09:03:46.000000 autogluon.timeseries-0.7.1b20230504/src/autogluon/timeseries/trainer/abstract_trainer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2751 2023-05-04 09:03:46.000000 autogluon.timeseries-0.7.1b20230504/src/autogluon/timeseries/trainer/auto_trainer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:04:28.219674 autogluon.timeseries-0.7.1b20230504/src/autogluon/timeseries/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 09:03:46.000000 autogluon.timeseries-0.7.1b20230504/src/autogluon/timeseries/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8270 2023-05-04 09:03:46.000000 autogluon.timeseries-0.7.1b20230504/src/autogluon/timeseries/utils/features.py
--rw-r--r--   0 runner    (1001) docker     (123)     1727 2023-05-04 09:03:46.000000 autogluon.timeseries-0.7.1b20230504/src/autogluon/timeseries/utils/forecast.py
--rw-r--r--   0 runner    (1001) docker     (123)      344 2023-05-04 09:03:46.000000 autogluon.timeseries-0.7.1b20230504/src/autogluon/timeseries/utils/random.py
--rw-r--r--   0 runner    (1001) docker     (123)      652 2023-05-04 09:03:46.000000 autogluon.timeseries-0.7.1b20230504/src/autogluon/timeseries/utils/seasonality.py
--rw-r--r--   0 runner    (1001) docker     (123)     2330 2023-05-04 09:03:46.000000 autogluon.timeseries-0.7.1b20230504/src/autogluon/timeseries/utils/warning_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-05-04 09:04:28.000000 autogluon.timeseries-0.7.1b20230504/src/autogluon/timeseries/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 09:04:28.207674 autogluon.timeseries-0.7.1b20230504/src/autogluon.timeseries.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    12593 2023-05-04 09:04:28.000000 autogluon.timeseries-0.7.1b20230504/src/autogluon.timeseries.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2624 2023-05-04 09:04:28.000000 autogluon.timeseries-0.7.1b20230504/src/autogluon.timeseries.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-04 09:04:28.000000 autogluon.timeseries-0.7.1b20230504/src/autogluon.timeseries.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-04 09:04:28.000000 autogluon.timeseries-0.7.1b20230504/src/autogluon.timeseries.egg-info/namespace_packages.txt
--rw-r--r--   0 runner    (1001) docker     (123)      504 2023-05-04 09:04:28.000000 autogluon.timeseries-0.7.1b20230504/src/autogluon.timeseries.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-04 09:04:28.000000 autogluon.timeseries-0.7.1b20230504/src/autogluon.timeseries.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-04 09:04:28.000000 autogluon.timeseries-0.7.1b20230504/src/autogluon.timeseries.egg-info/zip-safe
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 09:04:37.800071 autogluon.timeseries-0.7.1b20230505/
+-rw-r--r--   0 runner    (1001) docker     (123)    12593 2023-05-05 09:04:37.800071 autogluon.timeseries-0.7.1b20230505/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-05 09:04:37.800071 autogluon.timeseries-0.7.1b20230505/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2245 2023-05-05 09:03:33.000000 autogluon.timeseries-0.7.1b20230505/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 09:04:37.788071 autogluon.timeseries-0.7.1b20230505/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 09:04:37.788071 autogluon.timeseries-0.7.1b20230505/src/autogluon/
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-05-05 09:03:33.000000 autogluon.timeseries-0.7.1b20230505/src/autogluon/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 09:04:37.792071 autogluon.timeseries-0.7.1b20230505/src/autogluon/timeseries/
+-rw-r--r--   0 runner    (1001) docker     (123)      867 2023-05-05 09:03:33.000000 autogluon.timeseries-0.7.1b20230505/src/autogluon/timeseries/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 09:04:37.792071 autogluon.timeseries-0.7.1b20230505/src/autogluon/timeseries/configs/
+-rw-r--r--   0 runner    (1001) docker     (123)       98 2023-05-05 09:03:33.000000 autogluon.timeseries-0.7.1b20230505/src/autogluon/timeseries/configs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      638 2023-05-05 09:03:33.000000 autogluon.timeseries-0.7.1b20230505/src/autogluon/timeseries/configs/presets_configs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 09:04:37.792071 autogluon.timeseries-0.7.1b20230505/src/autogluon/timeseries/dataset/
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-05-05 09:03:33.000000 autogluon.timeseries-0.7.1b20230505/src/autogluon/timeseries/dataset/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37170 2023-05-05 09:03:33.000000 autogluon.timeseries-0.7.1b20230505/src/autogluon/timeseries/dataset/ts_dataframe.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11293 2023-05-05 09:03:33.000000 autogluon.timeseries-0.7.1b20230505/src/autogluon/timeseries/evaluator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10081 2023-05-05 09:03:33.000000 autogluon.timeseries-0.7.1b20230505/src/autogluon/timeseries/learner.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 09:04:37.792071 autogluon.timeseries-0.7.1b20230505/src/autogluon/timeseries/models/
+-rw-r--r--   0 runner    (1001) docker     (123)      676 2023-05-05 09:03:33.000000 autogluon.timeseries-0.7.1b20230505/src/autogluon/timeseries/models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 09:04:37.792071 autogluon.timeseries-0.7.1b20230505/src/autogluon/timeseries/models/abstract/
+-rw-r--r--   0 runner    (1001) docker     (123)      168 2023-05-05 09:03:33.000000 autogluon.timeseries-0.7.1b20230505/src/autogluon/timeseries/models/abstract/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19723 2023-05-05 09:03:33.000000 autogluon.timeseries-0.7.1b20230505/src/autogluon/timeseries/models/abstract/abstract_timeseries_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3735 2023-05-05 09:03:33.000000 autogluon.timeseries-0.7.1b20230505/src/autogluon/timeseries/models/abstract/model_trial.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 09:04:37.792071 autogluon.timeseries-0.7.1b20230505/src/autogluon/timeseries/models/autogluon_tabular/
+-rw-r--r--   0 runner    (1001) docker     (123)      168 2023-05-05 09:03:33.000000 autogluon.timeseries-0.7.1b20230505/src/autogluon/timeseries/models/autogluon_tabular/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12707 2023-05-05 09:03:33.000000 autogluon.timeseries-0.7.1b20230505/src/autogluon/timeseries/models/autogluon_tabular/mlforecast.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17282 2023-05-05 09:03:33.000000 autogluon.timeseries-0.7.1b20230505/src/autogluon/timeseries/models/autogluon_tabular/tabular_model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 09:04:37.796071 autogluon.timeseries-0.7.1b20230505/src/autogluon/timeseries/models/ensemble/
+-rw-r--r--   0 runner    (1001) docker     (123)      128 2023-05-05 09:03:33.000000 autogluon.timeseries-0.7.1b20230505/src/autogluon/timeseries/models/ensemble/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2733 2023-05-05 09:03:33.000000 autogluon.timeseries-0.7.1b20230505/src/autogluon/timeseries/models/ensemble/abstract_timeseries_ensemble.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5902 2023-05-05 09:03:33.000000 autogluon.timeseries-0.7.1b20230505/src/autogluon/timeseries/models/ensemble/greedy_ensemble.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 09:04:37.796071 autogluon.timeseries-0.7.1b20230505/src/autogluon/timeseries/models/gluonts/
+-rw-r--r--   0 runner    (1001) docker     (123)      174 2023-05-05 09:03:33.000000 autogluon.timeseries-0.7.1b20230505/src/autogluon/timeseries/models/gluonts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18915 2023-05-05 09:03:33.000000 autogluon.timeseries-0.7.1b20230505/src/autogluon/timeseries/models/gluonts/abstract_gluonts.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 09:04:37.796071 autogluon.timeseries-0.7.1b20230505/src/autogluon/timeseries/models/gluonts/mx/
+-rw-r--r--   0 runner    (1001) docker     (123)      932 2023-05-05 09:03:33.000000 autogluon.timeseries-0.7.1b20230505/src/autogluon/timeseries/models/gluonts/mx/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4053 2023-05-05 09:03:33.000000 autogluon.timeseries-0.7.1b20230505/src/autogluon/timeseries/models/gluonts/mx/callback.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22893 2023-05-05 09:03:33.000000 autogluon.timeseries-0.7.1b20230505/src/autogluon/timeseries/models/gluonts/mx/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 09:04:37.796071 autogluon.timeseries-0.7.1b20230505/src/autogluon/timeseries/models/gluonts/torch/
+-rw-r--r--   0 runner    (1001) docker     (123)      190 2023-05-05 09:03:33.000000 autogluon.timeseries-0.7.1b20230505/src/autogluon/timeseries/models/gluonts/torch/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13902 2023-05-05 09:03:33.000000 autogluon.timeseries-0.7.1b20230505/src/autogluon/timeseries/models/gluonts/torch/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 09:04:37.796071 autogluon.timeseries-0.7.1b20230505/src/autogluon/timeseries/models/local/
+-rw-r--r--   0 runner    (1001) docker     (123)      192 2023-05-05 09:03:33.000000 autogluon.timeseries-0.7.1b20230505/src/autogluon/timeseries/models/local/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6980 2023-05-05 09:03:33.000000 autogluon.timeseries-0.7.1b20230505/src/autogluon/timeseries/models/local/abstract_local_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4123 2023-05-05 09:03:33.000000 autogluon.timeseries-0.7.1b20230505/src/autogluon/timeseries/models/local/naive.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12222 2023-05-05 09:03:33.000000 autogluon.timeseries-0.7.1b20230505/src/autogluon/timeseries/models/local/statsforecast.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15697 2023-05-05 09:03:33.000000 autogluon.timeseries-0.7.1b20230505/src/autogluon/timeseries/models/local/statsmodels.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 09:04:37.796071 autogluon.timeseries-0.7.1b20230505/src/autogluon/timeseries/models/multi_window/
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-05-05 09:03:33.000000 autogluon.timeseries-0.7.1b20230505/src/autogluon/timeseries/models/multi_window/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9000 2023-05-05 09:03:33.000000 autogluon.timeseries-0.7.1b20230505/src/autogluon/timeseries/models/multi_window/multi_window_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9947 2023-05-05 09:03:33.000000 autogluon.timeseries-0.7.1b20230505/src/autogluon/timeseries/models/presets.py
+-rw-r--r--   0 runner    (1001) docker     (123)    46701 2023-05-05 09:03:33.000000 autogluon.timeseries-0.7.1b20230505/src/autogluon/timeseries/predictor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9252 2023-05-05 09:03:33.000000 autogluon.timeseries-0.7.1b20230505/src/autogluon/timeseries/splitter.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 09:04:37.800071 autogluon.timeseries-0.7.1b20230505/src/autogluon/timeseries/trainer/
+-rw-r--r--   0 runner    (1001) docker     (123)      170 2023-05-05 09:03:33.000000 autogluon.timeseries-0.7.1b20230505/src/autogluon/timeseries/trainer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41049 2023-05-05 09:03:33.000000 autogluon.timeseries-0.7.1b20230505/src/autogluon/timeseries/trainer/abstract_trainer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2751 2023-05-05 09:03:33.000000 autogluon.timeseries-0.7.1b20230505/src/autogluon/timeseries/trainer/auto_trainer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 09:04:37.800071 autogluon.timeseries-0.7.1b20230505/src/autogluon/timeseries/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 09:03:33.000000 autogluon.timeseries-0.7.1b20230505/src/autogluon/timeseries/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8270 2023-05-05 09:03:33.000000 autogluon.timeseries-0.7.1b20230505/src/autogluon/timeseries/utils/features.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1727 2023-05-05 09:03:33.000000 autogluon.timeseries-0.7.1b20230505/src/autogluon/timeseries/utils/forecast.py
+-rw-r--r--   0 runner    (1001) docker     (123)      344 2023-05-05 09:03:33.000000 autogluon.timeseries-0.7.1b20230505/src/autogluon/timeseries/utils/random.py
+-rw-r--r--   0 runner    (1001) docker     (123)      652 2023-05-05 09:03:33.000000 autogluon.timeseries-0.7.1b20230505/src/autogluon/timeseries/utils/seasonality.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2330 2023-05-05 09:03:33.000000 autogluon.timeseries-0.7.1b20230505/src/autogluon/timeseries/utils/warning_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-05-05 09:04:37.000000 autogluon.timeseries-0.7.1b20230505/src/autogluon/timeseries/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 09:04:37.792071 autogluon.timeseries-0.7.1b20230505/src/autogluon.timeseries.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    12593 2023-05-05 09:04:37.000000 autogluon.timeseries-0.7.1b20230505/src/autogluon.timeseries.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2624 2023-05-05 09:04:37.000000 autogluon.timeseries-0.7.1b20230505/src/autogluon.timeseries.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 09:04:37.000000 autogluon.timeseries-0.7.1b20230505/src/autogluon.timeseries.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-05 09:04:37.000000 autogluon.timeseries-0.7.1b20230505/src/autogluon.timeseries.egg-info/namespace_packages.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      504 2023-05-05 09:04:37.000000 autogluon.timeseries-0.7.1b20230505/src/autogluon.timeseries.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-05 09:04:37.000000 autogluon.timeseries-0.7.1b20230505/src/autogluon.timeseries.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 09:04:37.000000 autogluon.timeseries-0.7.1b20230505/src/autogluon.timeseries.egg-info/zip-safe
```

### Comparing `autogluon.timeseries-0.7.1b20230504/PKG-INFO` & `autogluon.timeseries-0.7.1b20230505/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autogluon.timeseries
-Version: 0.7.1b20230504
+Version: 0.7.1b20230505
 Summary: AutoML for Image, Text, and Tabular Data
 Home-page: https://github.com/autogluon/autogluon
 Author: AutoGluon Community
 License: Apache-2.0
 Project-URL: Documentation, https://auto.gluon.ai
 Project-URL: Bug Reports, https://github.com/autogluon/autogluon/issues
 Project-URL: Source, https://github.com/autogluon/autogluon/
```

### Comparing `autogluon.timeseries-0.7.1b20230504/setup.py` & `autogluon.timeseries-0.7.1b20230505/setup.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-0.7.1b20230504/src/autogluon/timeseries/__init__.py` & `autogluon.timeseries-0.7.1b20230505/src/autogluon/timeseries/__init__.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-0.7.1b20230504/src/autogluon/timeseries/configs/presets_configs.py` & `autogluon.timeseries-0.7.1b20230505/src/autogluon/timeseries/configs/presets_configs.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-0.7.1b20230504/src/autogluon/timeseries/dataset/ts_dataframe.py` & `autogluon.timeseries-0.7.1b20230505/src/autogluon/timeseries/dataset/ts_dataframe.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-0.7.1b20230504/src/autogluon/timeseries/evaluator.py` & `autogluon.timeseries-0.7.1b20230505/src/autogluon/timeseries/evaluator.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-0.7.1b20230504/src/autogluon/timeseries/learner.py` & `autogluon.timeseries-0.7.1b20230505/src/autogluon/timeseries/learner.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-0.7.1b20230504/src/autogluon/timeseries/models/__init__.py` & `autogluon.timeseries-0.7.1b20230505/src/autogluon/timeseries/models/__init__.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-0.7.1b20230504/src/autogluon/timeseries/models/abstract/abstract_timeseries_model.py` & `autogluon.timeseries-0.7.1b20230505/src/autogluon/timeseries/models/abstract/abstract_timeseries_model.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-0.7.1b20230504/src/autogluon/timeseries/models/abstract/model_trial.py` & `autogluon.timeseries-0.7.1b20230505/src/autogluon/timeseries/models/abstract/model_trial.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-0.7.1b20230504/src/autogluon/timeseries/models/autogluon_tabular/mlforecast.py` & `autogluon.timeseries-0.7.1b20230505/src/autogluon/timeseries/models/autogluon_tabular/mlforecast.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-0.7.1b20230504/src/autogluon/timeseries/models/autogluon_tabular/tabular_model.py` & `autogluon.timeseries-0.7.1b20230505/src/autogluon/timeseries/models/autogluon_tabular/tabular_model.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-0.7.1b20230504/src/autogluon/timeseries/models/ensemble/abstract_timeseries_ensemble.py` & `autogluon.timeseries-0.7.1b20230505/src/autogluon/timeseries/models/ensemble/abstract_timeseries_ensemble.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-0.7.1b20230504/src/autogluon/timeseries/models/ensemble/greedy_ensemble.py` & `autogluon.timeseries-0.7.1b20230505/src/autogluon/timeseries/models/ensemble/greedy_ensemble.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-0.7.1b20230504/src/autogluon/timeseries/models/gluonts/abstract_gluonts.py` & `autogluon.timeseries-0.7.1b20230505/src/autogluon/timeseries/models/gluonts/abstract_gluonts.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-0.7.1b20230504/src/autogluon/timeseries/models/gluonts/mx/__init__.py` & `autogluon.timeseries-0.7.1b20230505/src/autogluon/timeseries/models/gluonts/mx/__init__.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-0.7.1b20230504/src/autogluon/timeseries/models/gluonts/mx/callback.py` & `autogluon.timeseries-0.7.1b20230505/src/autogluon/timeseries/models/gluonts/mx/callback.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-0.7.1b20230504/src/autogluon/timeseries/models/gluonts/mx/models.py` & `autogluon.timeseries-0.7.1b20230505/src/autogluon/timeseries/models/gluonts/mx/models.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-0.7.1b20230504/src/autogluon/timeseries/models/gluonts/torch/models.py` & `autogluon.timeseries-0.7.1b20230505/src/autogluon/timeseries/models/gluonts/torch/models.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-0.7.1b20230504/src/autogluon/timeseries/models/local/abstract_local_model.py` & `autogluon.timeseries-0.7.1b20230505/src/autogluon/timeseries/models/local/abstract_local_model.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-0.7.1b20230504/src/autogluon/timeseries/models/local/naive.py` & `autogluon.timeseries-0.7.1b20230505/src/autogluon/timeseries/models/local/naive.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-0.7.1b20230504/src/autogluon/timeseries/models/local/statsforecast.py` & `autogluon.timeseries-0.7.1b20230505/src/autogluon/timeseries/models/local/statsforecast.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-0.7.1b20230504/src/autogluon/timeseries/models/local/statsmodels.py` & `autogluon.timeseries-0.7.1b20230505/src/autogluon/timeseries/models/local/statsmodels.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-0.7.1b20230504/src/autogluon/timeseries/models/multi_window/multi_window_model.py` & `autogluon.timeseries-0.7.1b20230505/src/autogluon/timeseries/models/multi_window/multi_window_model.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-0.7.1b20230504/src/autogluon/timeseries/models/presets.py` & `autogluon.timeseries-0.7.1b20230505/src/autogluon/timeseries/models/presets.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-0.7.1b20230504/src/autogluon/timeseries/predictor.py` & `autogluon.timeseries-0.7.1b20230505/src/autogluon/timeseries/predictor.py`

 * *Files 1% similar despite different names*

```diff
@@ -98,16 +98,14 @@
         ``TimeSeriesPredictor``.
     learner_kwargs : dict, optional
         Keyword arguments to send to the learner (for advanced users only). Options include ``trainer_type``, a
         class inheriting from ``AbstractTrainer`` which controls training of multiple models.
         If ``path`` and ``eval_metric`` are re-specified within ``learner_kwargs``, these are ignored.
     label : str, optional
         Alias for :attr:`target`.
-    quantiles : List[float], optional
-        Alias for :attr:`quantile_levels`.
     """
 
     predictor_file_name = "predictor.pkl"
 
     def __init__(
         self,
         target: Optional[str] = None,
@@ -145,24 +143,27 @@
         if self.target in known_covariates_names:
             raise ValueError(f"Target column {self.target} cannot be one of the known covariates.")
         self.known_covariates_names = known_covariates_names
 
         self.prediction_length = prediction_length
         self.eval_metric = eval_metric
         self.eval_metric_seasonal_period = eval_metric_seasonal_period
-        if quantile_levels is not None and quantiles is not None:
-            raise ValueError(
-                "Both `quantile_levels` and `quantiles` are specified. Please specify at most one of these arguments."
-            )
-        self.quantile_levels = quantile_levels or quantiles or [0.1, 0.2, 0.3, 0.4, 0.5, 0.6, 0.7, 0.8, 0.9]
+        if quantile_levels is None:
+            quantile_levels = [0.1, 0.2, 0.3, 0.4, 0.5, 0.6, 0.7, 0.8, 0.9]
+        self.quantile_levels = quantile_levels
 
         if validation_splitter is not None:
             warnings.warn(
-                "validation_splitter argument has been deprecated as of v0.8.0. "
-                "Please user the `num_val_windows` argument of `TimeSeriesPredictor.fit` instead."
+                "`validation_splitter` argument has been deprecated as of v0.8.0. "
+                "Please use the `num_val_windows` argument of `TimeSeriesPredictor.fit` instead."
+            )
+        if quantiles is not None:
+            warnings.warn(
+                "`quantiles` argument has been deprecated as of v0.8.0. "
+                "Please use the `quantile_levels` argument instead."
             )
 
         if learner_kwargs is None:
             learner_kwargs = {}
         learner_kwargs = learner_kwargs.copy()
         learner_kwargs.update(
             dict(
```

### Comparing `autogluon.timeseries-0.7.1b20230504/src/autogluon/timeseries/splitter.py` & `autogluon.timeseries-0.7.1b20230505/src/autogluon/timeseries/splitter.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-0.7.1b20230504/src/autogluon/timeseries/trainer/abstract_trainer.py` & `autogluon.timeseries-0.7.1b20230505/src/autogluon/timeseries/trainer/abstract_trainer.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-0.7.1b20230504/src/autogluon/timeseries/trainer/auto_trainer.py` & `autogluon.timeseries-0.7.1b20230505/src/autogluon/timeseries/trainer/auto_trainer.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-0.7.1b20230504/src/autogluon/timeseries/utils/features.py` & `autogluon.timeseries-0.7.1b20230505/src/autogluon/timeseries/utils/features.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-0.7.1b20230504/src/autogluon/timeseries/utils/forecast.py` & `autogluon.timeseries-0.7.1b20230505/src/autogluon/timeseries/utils/forecast.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-0.7.1b20230504/src/autogluon/timeseries/utils/seasonality.py` & `autogluon.timeseries-0.7.1b20230505/src/autogluon/timeseries/utils/seasonality.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-0.7.1b20230504/src/autogluon/timeseries/utils/warning_filters.py` & `autogluon.timeseries-0.7.1b20230505/src/autogluon/timeseries/utils/warning_filters.py`

 * *Files identical despite different names*

### Comparing `autogluon.timeseries-0.7.1b20230504/src/autogluon.timeseries.egg-info/PKG-INFO` & `autogluon.timeseries-0.7.1b20230505/src/autogluon.timeseries.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: autogluon.timeseries
-Version: 0.7.1b20230504
+Version: 0.7.1b20230505
 Summary: AutoML for Image, Text, and Tabular Data
 Home-page: https://github.com/autogluon/autogluon
 Author: AutoGluon Community
 License: Apache-2.0
 Project-URL: Documentation, https://auto.gluon.ai
 Project-URL: Bug Reports, https://github.com/autogluon/autogluon/issues
 Project-URL: Source, https://github.com/autogluon/autogluon/
```

### Comparing `autogluon.timeseries-0.7.1b20230504/src/autogluon.timeseries.egg-info/SOURCES.txt` & `autogluon.timeseries-0.7.1b20230505/src/autogluon.timeseries.egg-info/SOURCES.txt`

 * *Files identical despite different names*

