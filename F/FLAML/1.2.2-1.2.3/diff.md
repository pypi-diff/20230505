# Comparing `tmp/FLAML-1.2.2.tar.gz` & `tmp/FLAML-1.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "FLAML-1.2.2.tar", last modified: Tue Apr 25 03:33:14 2023, max compression
+gzip compressed data, was "FLAML-1.2.3.tar", last modified: Fri May  5 20:04:35 2023, max compression
```

## Comparing `FLAML-1.2.2.tar` & `FLAML-1.2.3.tar`

### file list

```diff
@@ -1,126 +1,132 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 03:33:14.070906 FLAML-1.2.2/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 03:33:14.058906 FLAML-1.2.2/FLAML.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8770 2023-04-25 03:33:14.000000 FLAML-1.2.2/FLAML.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2827 2023-04-25 03:33:14.000000 FLAML-1.2.2/FLAML.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-25 03:33:14.000000 FLAML-1.2.2/FLAML.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1249 2023-04-25 03:33:14.000000 FLAML-1.2.2/FLAML.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-25 03:33:14.000000 FLAML-1.2.2/FLAML.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1141 2023-04-25 03:32:17.000000 FLAML-1.2.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    15444 2023-04-25 03:32:17.000000 FLAML-1.2.2/NOTICE.md
--rw-r--r--   0 runner    (1001) docker     (123)     8770 2023-04-25 03:33:14.070906 FLAML-1.2.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7898 2023-04-25 03:32:17.000000 FLAML-1.2.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 03:33:14.058906 FLAML-1.2.2/flaml/
--rw-r--r--   0 runner    (1001) docker     (123)      354 2023-04-25 03:32:17.000000 FLAML-1.2.2/flaml/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 03:33:14.058906 FLAML-1.2.2/flaml/autogen/
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-04-25 03:32:17.000000 FLAML-1.2.2/flaml/autogen/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16169 2023-04-25 03:32:17.000000 FLAML-1.2.2/flaml/autogen/code_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 03:33:14.058906 FLAML-1.2.2/flaml/autogen/extensions/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 03:32:17.000000 FLAML-1.2.2/flaml/autogen/extensions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9963 2023-04-25 03:32:17.000000 FLAML-1.2.2/flaml/autogen/math_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 03:33:14.058906 FLAML-1.2.2/flaml/autogen/oai/
--rw-r--r--   0 runner    (1001) docker     (123)      112 2023-04-25 03:32:17.000000 FLAML-1.2.2/flaml/autogen/oai/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    37502 2023-04-25 03:32:17.000000 FLAML-1.2.2/flaml/autogen/oai/completion.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 03:33:14.062906 FLAML-1.2.2/flaml/automl/
--rw-r--r--   0 runner    (1001) docker     (123)      230 2023-04-25 03:32:17.000000 FLAML-1.2.2/flaml/automl/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   129453 2023-04-25 03:32:17.000000 FLAML-1.2.2/flaml/automl/automl.py
--rw-r--r--   0 runner    (1001) docker     (123)    18262 2023-04-25 03:32:17.000000 FLAML-1.2.2/flaml/automl/data.py
--rw-r--r--   0 runner    (1001) docker     (123)      207 2023-04-25 03:32:17.000000 FLAML-1.2.2/flaml/automl/logger.py
--rw-r--r--   0 runner    (1001) docker     (123)    23042 2023-04-25 03:32:17.000000 FLAML-1.2.2/flaml/automl/ml.py
--rw-r--r--   0 runner    (1001) docker     (123)   105084 2023-04-25 03:32:17.000000 FLAML-1.2.2/flaml/automl/model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 03:33:14.062906 FLAML-1.2.2/flaml/automl/nlp/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 03:32:17.000000 FLAML-1.2.2/flaml/automl/nlp/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 03:33:14.062906 FLAML-1.2.2/flaml/automl/nlp/huggingface/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 03:32:17.000000 FLAML-1.2.2/flaml/automl/nlp/huggingface/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1732 2023-04-25 03:32:17.000000 FLAML-1.2.2/flaml/automl/nlp/huggingface/data_collator.py
--rw-r--r--   0 runner    (1001) docker     (123)     3116 2023-04-25 03:32:17.000000 FLAML-1.2.2/flaml/automl/nlp/huggingface/trainer.py
--rw-r--r--   0 runner    (1001) docker     (123)     5600 2023-04-25 03:32:17.000000 FLAML-1.2.2/flaml/automl/nlp/huggingface/training_args.py
--rw-r--r--   0 runner    (1001) docker     (123)    16457 2023-04-25 03:32:17.000000 FLAML-1.2.2/flaml/automl/nlp/huggingface/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3309 2023-04-25 03:32:17.000000 FLAML-1.2.2/flaml/automl/nlp/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 03:33:14.062906 FLAML-1.2.2/flaml/automl/spark/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 03:32:17.000000 FLAML-1.2.2/flaml/automl/spark/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2139 2023-04-25 03:32:17.000000 FLAML-1.2.2/flaml/automl/spark/configs.py
--rw-r--r--   0 runner    (1001) docker     (123)     7827 2023-04-25 03:32:17.000000 FLAML-1.2.2/flaml/automl/spark/metrics.py
--rw-r--r--   0 runner    (1001) docker     (123)    10203 2023-04-25 03:32:17.000000 FLAML-1.2.2/flaml/automl/spark/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    16917 2023-04-25 03:32:17.000000 FLAML-1.2.2/flaml/automl/state.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 03:33:14.062906 FLAML-1.2.2/flaml/automl/task/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 03:32:17.000000 FLAML-1.2.2/flaml/automl/task/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      411 2023-04-25 03:32:17.000000 FLAML-1.2.2/flaml/automl/task/factory.py
--rw-r--r--   0 runner    (1001) docker     (123)    44736 2023-04-25 03:32:17.000000 FLAML-1.2.2/flaml/automl/task/generic_task.py
--rw-r--r--   0 runner    (1001) docker     (123)    13635 2023-04-25 03:32:17.000000 FLAML-1.2.2/flaml/automl/task/task.py
--rw-r--r--   0 runner    (1001) docker     (123)     5042 2023-04-25 03:32:17.000000 FLAML-1.2.2/flaml/automl/training_log.py
--rw-r--r--   0 runner    (1001) docker     (123)      703 2023-04-25 03:32:17.000000 FLAML-1.2.2/flaml/automl/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      386 2023-04-25 03:32:17.000000 FLAML-1.2.2/flaml/config.py
--rw-r--r--   0 runner    (1001) docker     (123)      174 2023-04-25 03:32:17.000000 FLAML-1.2.2/flaml/data.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 03:33:14.062906 FLAML-1.2.2/flaml/default/
--rw-r--r--   0 runner    (1001) docker     (123)      382 2023-04-25 03:32:17.000000 FLAML-1.2.2/flaml/default/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 03:33:14.062906 FLAML-1.2.2/flaml/default/all/
--rw-r--r--   0 runner    (1001) docker     (123)    22660 2023-04-25 03:32:17.000000 FLAML-1.2.2/flaml/default/all/binary.json
--rw-r--r--   0 runner    (1001) docker     (123)    34092 2023-04-25 03:32:17.000000 FLAML-1.2.2/flaml/default/all/multiclass.json
--rw-r--r--   0 runner    (1001) docker     (123)    21612 2023-04-25 03:32:17.000000 FLAML-1.2.2/flaml/default/all/regression.json
--rw-r--r--   0 runner    (1001) docker     (123)     6796 2023-04-25 03:32:17.000000 FLAML-1.2.2/flaml/default/estimator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 03:33:14.066906 FLAML-1.2.2/flaml/default/extra_tree/
--rw-r--r--   0 runner    (1001) docker     (123)     8013 2023-04-25 03:32:17.000000 FLAML-1.2.2/flaml/default/extra_tree/binary.json
--rw-r--r--   0 runner    (1001) docker     (123)     6766 2023-04-25 03:32:17.000000 FLAML-1.2.2/flaml/default/extra_tree/multiclass.json
--rw-r--r--   0 runner    (1001) docker     (123)     6596 2023-04-25 03:32:17.000000 FLAML-1.2.2/flaml/default/extra_tree/regression.json
--rw-r--r--   0 runner    (1001) docker     (123)     3424 2023-04-25 03:32:17.000000 FLAML-1.2.2/flaml/default/greedy.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 03:33:14.066906 FLAML-1.2.2/flaml/default/lgbm/
--rw-r--r--   0 runner    (1001) docker     (123)     8689 2023-04-25 03:32:17.000000 FLAML-1.2.2/flaml/default/lgbm/binary.json
--rw-r--r--   0 runner    (1001) docker     (123)    10021 2023-04-25 03:32:17.000000 FLAML-1.2.2/flaml/default/lgbm/multiclass.json
--rw-r--r--   0 runner    (1001) docker     (123)     6264 2023-04-25 03:32:17.000000 FLAML-1.2.2/flaml/default/lgbm/regression.json
--rw-r--r--   0 runner    (1001) docker     (123)     8249 2023-04-25 03:32:17.000000 FLAML-1.2.2/flaml/default/portfolio.py
--rw-r--r--   0 runner    (1001) docker     (123)     1399 2023-04-25 03:32:17.000000 FLAML-1.2.2/flaml/default/regret.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 03:33:14.066906 FLAML-1.2.2/flaml/default/rf/
--rw-r--r--   0 runner    (1001) docker     (123)     7353 2023-04-25 03:32:17.000000 FLAML-1.2.2/flaml/default/rf/binary.json
--rw-r--r--   0 runner    (1001) docker     (123)     7172 2023-04-25 03:32:17.000000 FLAML-1.2.2/flaml/default/rf/multiclass.json
--rw-r--r--   0 runner    (1001) docker     (123)     6357 2023-04-25 03:32:17.000000 FLAML-1.2.2/flaml/default/rf/regression.json
--rw-r--r--   0 runner    (1001) docker     (123)    11842 2023-04-25 03:32:17.000000 FLAML-1.2.2/flaml/default/suggest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 03:33:14.066906 FLAML-1.2.2/flaml/default/xgb_limitdepth/
--rw-r--r--   0 runner    (1001) docker     (123)     7785 2023-04-25 03:32:17.000000 FLAML-1.2.2/flaml/default/xgb_limitdepth/binary.json
--rw-r--r--   0 runner    (1001) docker     (123)     9144 2023-04-25 03:32:17.000000 FLAML-1.2.2/flaml/default/xgb_limitdepth/multiclass.json
--rw-r--r--   0 runner    (1001) docker     (123)     8254 2023-04-25 03:32:17.000000 FLAML-1.2.2/flaml/default/xgb_limitdepth/regression.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 03:33:14.066906 FLAML-1.2.2/flaml/default/xgboost/
--rw-r--r--   0 runner    (1001) docker     (123)     8986 2023-04-25 03:32:17.000000 FLAML-1.2.2/flaml/default/xgboost/binary.json
--rw-r--r--   0 runner    (1001) docker     (123)    13159 2023-04-25 03:32:17.000000 FLAML-1.2.2/flaml/default/xgboost/multiclass.json
--rw-r--r--   0 runner    (1001) docker     (123)     7203 2023-04-25 03:32:17.000000 FLAML-1.2.2/flaml/default/xgboost/regression.json
--rw-r--r--   0 runner    (1001) docker     (123)      168 2023-04-25 03:32:17.000000 FLAML-1.2.2/flaml/ml.py
--rw-r--r--   0 runner    (1001) docker     (123)      177 2023-04-25 03:32:17.000000 FLAML-1.2.2/flaml/model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 03:33:14.066906 FLAML-1.2.2/flaml/onlineml/
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-04-25 03:32:17.000000 FLAML-1.2.2/flaml/onlineml/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10010 2023-04-25 03:32:17.000000 FLAML-1.2.2/flaml/onlineml/autovw.py
--rw-r--r--   0 runner    (1001) docker     (123)    16667 2023-04-25 03:32:17.000000 FLAML-1.2.2/flaml/onlineml/trial.py
--rw-r--r--   0 runner    (1001) docker     (123)    24670 2023-04-25 03:32:17.000000 FLAML-1.2.2/flaml/onlineml/trial_runner.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 03:33:14.066906 FLAML-1.2.2/flaml/tune/
--rw-r--r--   0 runner    (1001) docker     (123)      956 2023-04-25 03:32:17.000000 FLAML-1.2.2/flaml/tune/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9648 2023-04-25 03:32:17.000000 FLAML-1.2.2/flaml/tune/analysis.py
--rw-r--r--   0 runner    (1001) docker     (123)     4455 2023-04-25 03:32:17.000000 FLAML-1.2.2/flaml/tune/result.py
--rw-r--r--   0 runner    (1001) docker     (123)    22060 2023-04-25 03:32:17.000000 FLAML-1.2.2/flaml/tune/sample.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 03:33:14.066906 FLAML-1.2.2/flaml/tune/scheduler/
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-04-25 03:32:17.000000 FLAML-1.2.2/flaml/tune/scheduler/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6088 2023-04-25 03:32:17.000000 FLAML-1.2.2/flaml/tune/scheduler/online_scheduler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1235 2023-04-25 03:32:17.000000 FLAML-1.2.2/flaml/tune/scheduler/trial_scheduler.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 03:33:14.070906 FLAML-1.2.2/flaml/tune/searcher/
--rw-r--r--   0 runner    (1001) docker     (123)      153 2023-04-25 03:32:17.000000 FLAML-1.2.2/flaml/tune/searcher/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    50302 2023-04-25 03:32:17.000000 FLAML-1.2.2/flaml/tune/searcher/blendsearch.py
--rw-r--r--   0 runner    (1001) docker     (123)      802 2023-04-25 03:32:17.000000 FLAML-1.2.2/flaml/tune/searcher/cfo_cat.py
--rw-r--r--   0 runner    (1001) docker     (123)    30648 2023-04-25 03:32:17.000000 FLAML-1.2.2/flaml/tune/searcher/flow2.py
--rw-r--r--   0 runner    (1001) docker     (123)    18065 2023-04-25 03:32:17.000000 FLAML-1.2.2/flaml/tune/searcher/online_searcher.py
--rw-r--r--   0 runner    (1001) docker     (123)     7310 2023-04-25 03:32:17.000000 FLAML-1.2.2/flaml/tune/searcher/search_thread.py
--rw-r--r--   0 runner    (1001) docker     (123)    31123 2023-04-25 03:32:17.000000 FLAML-1.2.2/flaml/tune/searcher/suggestion.py
--rw-r--r--   0 runner    (1001) docker     (123)    11031 2023-04-25 03:32:17.000000 FLAML-1.2.2/flaml/tune/searcher/variant_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)    22364 2023-04-25 03:32:17.000000 FLAML-1.2.2/flaml/tune/space.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 03:33:14.070906 FLAML-1.2.2/flaml/tune/spark/
--rw-r--r--   0 runner    (1001) docker     (123)      191 2023-04-25 03:32:17.000000 FLAML-1.2.2/flaml/tune/spark/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10357 2023-04-25 03:32:17.000000 FLAML-1.2.2/flaml/tune/spark/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     5975 2023-04-25 03:32:17.000000 FLAML-1.2.2/flaml/tune/trial.py
--rw-r--r--   0 runner    (1001) docker     (123)     5353 2023-04-25 03:32:17.000000 FLAML-1.2.2/flaml/tune/trial_runner.py
--rw-r--r--   0 runner    (1001) docker     (123)    37129 2023-04-25 03:32:17.000000 FLAML-1.2.2/flaml/tune/tune.py
--rw-r--r--   0 runner    (1001) docker     (123)      942 2023-04-25 03:32:17.000000 FLAML-1.2.2/flaml/tune/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-25 03:32:17.000000 FLAML-1.2.2/flaml/version.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-25 03:33:14.070906 FLAML-1.2.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3753 2023-04-25 03:32:17.000000 FLAML-1.2.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 03:33:14.070906 FLAML-1.2.2/test/
--rw-r--r--   0 runner    (1001) docker     (123)    15068 2023-04-25 03:32:17.000000 FLAML-1.2.2/test/test_autovw.py
--rw-r--r--   0 runner    (1001) docker     (123)      967 2023-04-25 03:32:17.000000 FLAML-1.2.2/test/test_conda_distribution.py
--rw-r--r--   0 runner    (1001) docker     (123)     3177 2023-04-25 03:32:17.000000 FLAML-1.2.2/test/test_gpu.py
--rw-r--r--   0 runner    (1001) docker     (123)     3419 2023-04-25 03:32:17.000000 FLAML-1.2.2/test/test_model.py
--rw-r--r--   0 runner    (1001) docker     (123)      253 2023-04-25 03:32:17.000000 FLAML-1.2.2/test/test_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 20:04:35.525714 FLAML-1.2.3/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 20:04:35.513713 FLAML-1.2.3/FLAML.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8813 2023-05-05 20:04:35.000000 FLAML-1.2.3/FLAML.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2978 2023-05-05 20:04:35.000000 FLAML-1.2.3/FLAML.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 20:04:35.000000 FLAML-1.2.3/FLAML.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1256 2023-05-05 20:04:35.000000 FLAML-1.2.3/FLAML.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-05 20:04:35.000000 FLAML-1.2.3/FLAML.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1141 2023-05-05 20:03:33.000000 FLAML-1.2.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    15444 2023-05-05 20:03:33.000000 FLAML-1.2.3/NOTICE.md
+-rw-r--r--   0 runner    (1001) docker     (123)     8813 2023-05-05 20:04:35.525714 FLAML-1.2.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7941 2023-05-05 20:03:33.000000 FLAML-1.2.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 20:04:35.513713 FLAML-1.2.3/flaml/
+-rw-r--r--   0 runner    (1001) docker     (123)      354 2023-05-05 20:03:33.000000 FLAML-1.2.3/flaml/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 20:04:35.513713 FLAML-1.2.3/flaml/autogen/
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-05-05 20:03:33.000000 FLAML-1.2.3/flaml/autogen/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 20:04:35.517713 FLAML-1.2.3/flaml/autogen/agent/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 20:03:33.000000 FLAML-1.2.3/flaml/autogen/agent/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1937 2023-05-05 20:03:33.000000 FLAML-1.2.3/flaml/autogen/agent/agent.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2601 2023-05-05 20:03:33.000000 FLAML-1.2.3/flaml/autogen/agent/coding_agent.py
+-rw-r--r--   0 runner    (1001) docker     (123)      991 2023-05-05 20:03:33.000000 FLAML-1.2.3/flaml/autogen/agent/execution_agent.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16129 2023-05-05 20:03:33.000000 FLAML-1.2.3/flaml/autogen/code_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 20:04:35.517713 FLAML-1.2.3/flaml/autogen/extensions/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 20:03:33.000000 FLAML-1.2.3/flaml/autogen/extensions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9946 2023-05-05 20:03:33.000000 FLAML-1.2.3/flaml/autogen/math_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 20:04:35.517713 FLAML-1.2.3/flaml/autogen/oai/
+-rw-r--r--   0 runner    (1001) docker     (123)      112 2023-05-05 20:03:33.000000 FLAML-1.2.3/flaml/autogen/oai/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    44488 2023-05-05 20:03:33.000000 FLAML-1.2.3/flaml/autogen/oai/completion.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 20:04:35.517713 FLAML-1.2.3/flaml/automl/
+-rw-r--r--   0 runner    (1001) docker     (123)      230 2023-05-05 20:03:33.000000 FLAML-1.2.3/flaml/automl/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   130309 2023-05-05 20:03:33.000000 FLAML-1.2.3/flaml/automl/automl.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18262 2023-05-05 20:03:33.000000 FLAML-1.2.3/flaml/automl/data.py
+-rw-r--r--   0 runner    (1001) docker     (123)      207 2023-05-05 20:03:33.000000 FLAML-1.2.3/flaml/automl/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23042 2023-05-05 20:03:33.000000 FLAML-1.2.3/flaml/automl/ml.py
+-rw-r--r--   0 runner    (1001) docker     (123)   104984 2023-05-05 20:03:33.000000 FLAML-1.2.3/flaml/automl/model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 20:04:35.517713 FLAML-1.2.3/flaml/automl/nlp/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 20:03:33.000000 FLAML-1.2.3/flaml/automl/nlp/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 20:04:35.517713 FLAML-1.2.3/flaml/automl/nlp/huggingface/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 20:03:33.000000 FLAML-1.2.3/flaml/automl/nlp/huggingface/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1732 2023-05-05 20:03:33.000000 FLAML-1.2.3/flaml/automl/nlp/huggingface/data_collator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3116 2023-05-05 20:03:33.000000 FLAML-1.2.3/flaml/automl/nlp/huggingface/trainer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5600 2023-05-05 20:03:33.000000 FLAML-1.2.3/flaml/automl/nlp/huggingface/training_args.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16528 2023-05-05 20:03:33.000000 FLAML-1.2.3/flaml/automl/nlp/huggingface/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3309 2023-05-05 20:03:33.000000 FLAML-1.2.3/flaml/automl/nlp/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 20:04:35.517713 FLAML-1.2.3/flaml/automl/spark/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 20:03:33.000000 FLAML-1.2.3/flaml/automl/spark/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2139 2023-05-05 20:03:33.000000 FLAML-1.2.3/flaml/automl/spark/configs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7827 2023-05-05 20:03:33.000000 FLAML-1.2.3/flaml/automl/spark/metrics.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10203 2023-05-05 20:03:33.000000 FLAML-1.2.3/flaml/automl/spark/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16917 2023-05-05 20:03:33.000000 FLAML-1.2.3/flaml/automl/state.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 20:04:35.517713 FLAML-1.2.3/flaml/automl/task/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 20:03:33.000000 FLAML-1.2.3/flaml/automl/task/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      411 2023-05-05 20:03:33.000000 FLAML-1.2.3/flaml/automl/task/factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)    44736 2023-05-05 20:03:33.000000 FLAML-1.2.3/flaml/automl/task/generic_task.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13635 2023-05-05 20:03:33.000000 FLAML-1.2.3/flaml/automl/task/task.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5042 2023-05-05 20:03:33.000000 FLAML-1.2.3/flaml/automl/training_log.py
+-rw-r--r--   0 runner    (1001) docker     (123)      703 2023-05-05 20:03:33.000000 FLAML-1.2.3/flaml/automl/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      386 2023-05-05 20:03:33.000000 FLAML-1.2.3/flaml/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      174 2023-05-05 20:03:33.000000 FLAML-1.2.3/flaml/data.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 20:04:35.517713 FLAML-1.2.3/flaml/default/
+-rw-r--r--   0 runner    (1001) docker     (123)      382 2023-05-05 20:03:33.000000 FLAML-1.2.3/flaml/default/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 20:04:35.521714 FLAML-1.2.3/flaml/default/all/
+-rw-r--r--   0 runner    (1001) docker     (123)    22660 2023-05-05 20:03:33.000000 FLAML-1.2.3/flaml/default/all/binary.json
+-rw-r--r--   0 runner    (1001) docker     (123)    34092 2023-05-05 20:03:33.000000 FLAML-1.2.3/flaml/default/all/multiclass.json
+-rw-r--r--   0 runner    (1001) docker     (123)    21612 2023-05-05 20:03:33.000000 FLAML-1.2.3/flaml/default/all/regression.json
+-rw-r--r--   0 runner    (1001) docker     (123)     6796 2023-05-05 20:03:33.000000 FLAML-1.2.3/flaml/default/estimator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 20:04:35.521714 FLAML-1.2.3/flaml/default/extra_tree/
+-rw-r--r--   0 runner    (1001) docker     (123)     8013 2023-05-05 20:03:33.000000 FLAML-1.2.3/flaml/default/extra_tree/binary.json
+-rw-r--r--   0 runner    (1001) docker     (123)     6766 2023-05-05 20:03:33.000000 FLAML-1.2.3/flaml/default/extra_tree/multiclass.json
+-rw-r--r--   0 runner    (1001) docker     (123)     6596 2023-05-05 20:03:33.000000 FLAML-1.2.3/flaml/default/extra_tree/regression.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3424 2023-05-05 20:03:33.000000 FLAML-1.2.3/flaml/default/greedy.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 20:04:35.521714 FLAML-1.2.3/flaml/default/lgbm/
+-rw-r--r--   0 runner    (1001) docker     (123)     8689 2023-05-05 20:03:33.000000 FLAML-1.2.3/flaml/default/lgbm/binary.json
+-rw-r--r--   0 runner    (1001) docker     (123)    10021 2023-05-05 20:03:33.000000 FLAML-1.2.3/flaml/default/lgbm/multiclass.json
+-rw-r--r--   0 runner    (1001) docker     (123)     6264 2023-05-05 20:03:33.000000 FLAML-1.2.3/flaml/default/lgbm/regression.json
+-rw-r--r--   0 runner    (1001) docker     (123)     8249 2023-05-05 20:03:33.000000 FLAML-1.2.3/flaml/default/portfolio.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1399 2023-05-05 20:03:33.000000 FLAML-1.2.3/flaml/default/regret.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 20:04:35.521714 FLAML-1.2.3/flaml/default/rf/
+-rw-r--r--   0 runner    (1001) docker     (123)     7353 2023-05-05 20:03:33.000000 FLAML-1.2.3/flaml/default/rf/binary.json
+-rw-r--r--   0 runner    (1001) docker     (123)     7172 2023-05-05 20:03:33.000000 FLAML-1.2.3/flaml/default/rf/multiclass.json
+-rw-r--r--   0 runner    (1001) docker     (123)     6357 2023-05-05 20:03:33.000000 FLAML-1.2.3/flaml/default/rf/regression.json
+-rw-r--r--   0 runner    (1001) docker     (123)    11842 2023-05-05 20:03:33.000000 FLAML-1.2.3/flaml/default/suggest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 20:04:35.521714 FLAML-1.2.3/flaml/default/xgb_limitdepth/
+-rw-r--r--   0 runner    (1001) docker     (123)     7785 2023-05-05 20:03:33.000000 FLAML-1.2.3/flaml/default/xgb_limitdepth/binary.json
+-rw-r--r--   0 runner    (1001) docker     (123)     9144 2023-05-05 20:03:33.000000 FLAML-1.2.3/flaml/default/xgb_limitdepth/multiclass.json
+-rw-r--r--   0 runner    (1001) docker     (123)     8254 2023-05-05 20:03:33.000000 FLAML-1.2.3/flaml/default/xgb_limitdepth/regression.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 20:04:35.521714 FLAML-1.2.3/flaml/default/xgboost/
+-rw-r--r--   0 runner    (1001) docker     (123)     8986 2023-05-05 20:03:33.000000 FLAML-1.2.3/flaml/default/xgboost/binary.json
+-rw-r--r--   0 runner    (1001) docker     (123)    13159 2023-05-05 20:03:33.000000 FLAML-1.2.3/flaml/default/xgboost/multiclass.json
+-rw-r--r--   0 runner    (1001) docker     (123)     7203 2023-05-05 20:03:33.000000 FLAML-1.2.3/flaml/default/xgboost/regression.json
+-rw-r--r--   0 runner    (1001) docker     (123)      168 2023-05-05 20:03:33.000000 FLAML-1.2.3/flaml/ml.py
+-rw-r--r--   0 runner    (1001) docker     (123)      177 2023-05-05 20:03:33.000000 FLAML-1.2.3/flaml/model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 20:04:35.521714 FLAML-1.2.3/flaml/onlineml/
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-05-05 20:03:33.000000 FLAML-1.2.3/flaml/onlineml/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10010 2023-05-05 20:03:33.000000 FLAML-1.2.3/flaml/onlineml/autovw.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16667 2023-05-05 20:03:33.000000 FLAML-1.2.3/flaml/onlineml/trial.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24670 2023-05-05 20:03:33.000000 FLAML-1.2.3/flaml/onlineml/trial_runner.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 20:04:35.521714 FLAML-1.2.3/flaml/tune/
+-rw-r--r--   0 runner    (1001) docker     (123)      956 2023-05-05 20:03:33.000000 FLAML-1.2.3/flaml/tune/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9648 2023-05-05 20:03:33.000000 FLAML-1.2.3/flaml/tune/analysis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4455 2023-05-05 20:03:33.000000 FLAML-1.2.3/flaml/tune/result.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22060 2023-05-05 20:03:33.000000 FLAML-1.2.3/flaml/tune/sample.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 20:04:35.521714 FLAML-1.2.3/flaml/tune/scheduler/
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-05 20:03:33.000000 FLAML-1.2.3/flaml/tune/scheduler/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6088 2023-05-05 20:03:33.000000 FLAML-1.2.3/flaml/tune/scheduler/online_scheduler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1235 2023-05-05 20:03:33.000000 FLAML-1.2.3/flaml/tune/scheduler/trial_scheduler.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 20:04:35.525714 FLAML-1.2.3/flaml/tune/searcher/
+-rw-r--r--   0 runner    (1001) docker     (123)      153 2023-05-05 20:03:33.000000 FLAML-1.2.3/flaml/tune/searcher/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    50302 2023-05-05 20:03:33.000000 FLAML-1.2.3/flaml/tune/searcher/blendsearch.py
+-rw-r--r--   0 runner    (1001) docker     (123)      802 2023-05-05 20:03:33.000000 FLAML-1.2.3/flaml/tune/searcher/cfo_cat.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30648 2023-05-05 20:03:33.000000 FLAML-1.2.3/flaml/tune/searcher/flow2.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18065 2023-05-05 20:03:33.000000 FLAML-1.2.3/flaml/tune/searcher/online_searcher.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7310 2023-05-05 20:03:33.000000 FLAML-1.2.3/flaml/tune/searcher/search_thread.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31123 2023-05-05 20:03:33.000000 FLAML-1.2.3/flaml/tune/searcher/suggestion.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11031 2023-05-05 20:03:33.000000 FLAML-1.2.3/flaml/tune/searcher/variant_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22364 2023-05-05 20:03:33.000000 FLAML-1.2.3/flaml/tune/space.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 20:04:35.525714 FLAML-1.2.3/flaml/tune/spark/
+-rw-r--r--   0 runner    (1001) docker     (123)      191 2023-05-05 20:03:33.000000 FLAML-1.2.3/flaml/tune/spark/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10357 2023-05-05 20:03:33.000000 FLAML-1.2.3/flaml/tune/spark/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5975 2023-05-05 20:03:33.000000 FLAML-1.2.3/flaml/tune/trial.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5353 2023-05-05 20:03:33.000000 FLAML-1.2.3/flaml/tune/trial_runner.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37002 2023-05-05 20:03:33.000000 FLAML-1.2.3/flaml/tune/tune.py
+-rw-r--r--   0 runner    (1001) docker     (123)      942 2023-05-05 20:03:33.000000 FLAML-1.2.3/flaml/tune/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-05 20:03:33.000000 FLAML-1.2.3/flaml/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1108 2023-05-05 20:03:33.000000 FLAML-1.2.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-05 20:04:35.525714 FLAML-1.2.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3811 2023-05-05 20:03:33.000000 FLAML-1.2.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 20:04:35.525714 FLAML-1.2.3/test/
+-rw-r--r--   0 runner    (1001) docker     (123)    15068 2023-05-05 20:03:33.000000 FLAML-1.2.3/test/test_autovw.py
+-rw-r--r--   0 runner    (1001) docker     (123)      967 2023-05-05 20:03:33.000000 FLAML-1.2.3/test/test_conda_distribution.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3177 2023-05-05 20:03:33.000000 FLAML-1.2.3/test/test_gpu.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3419 2023-05-05 20:03:33.000000 FLAML-1.2.3/test/test_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)      253 2023-05-05 20:03:33.000000 FLAML-1.2.3/test/test_version.py
```

### Comparing `FLAML-1.2.2/FLAML.egg-info/PKG-INFO` & `FLAML-1.2.3/FLAML.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: FLAML
-Version: 1.2.2
+Version: 1.2.3
 Summary: A fast library for automated machine learning and tuning
 Home-page: https://github.com/microsoft/FLAML
 Author: Microsoft Corporation
 Author-email: hpo@microsoft.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -44,26 +44,24 @@
 <p align="center">
     <img src="https://github.com/microsoft/FLAML/blob/main/website/static/img/flaml.svg"  width=200>
     <br>
 </p>
 
 :fire: v1.2.0 is released with support for ChatGPT and GPT-4.
 
-:fire: A [lab forum](https://github.com/microsoft/FLAML/tree/tutorial-aaai23/tutorial) on FLAML at AAAI 2023.
-
-:fire: A [hands-on tutorial](https://github.com/microsoft/FLAML/tree/tutorial/tutorial) on FLAML presented at KDD 2022
 
 ## What is FLAML
-FLAML is a lightweight Python library that finds accurate machine
-learning models automatically, efficiently and economically. It frees users from selecting
-models and hyperparameters for each model. It can also be used to tune generic hyperparameters for foundation models, MLOps/LMOps workflows, pipelines, mathematical/statistical models, algorithms, computing experiments, software configurations and so on.
-
-1. For common machine learning or AI tasks like classification, regression, and generation, it quickly finds quality models for user-provided data with low computational resources. It supports both classical machine learning models and deep neural networks, including foundation models such as the GPT series.
-1. It is easy to customize or extend. Users can find their desired customizability from a smooth range: minimal customization (computational resource budget), medium customization (e.g., scikit-style learner, search space and metric), or full customization (arbitrary training and evaluation code).
-1. It supports fast automatic tuning, capable of handling complex constraints/guidance/early stopping. FLAML is powered by a new, [cost-effective
+FLAML is a lightweight Python library for efficient automation of machine
+learning, including selection of
+models, hyperparameters, and other tunable choices of an application (e.g., inference hyperparameters for foundation models, configurations in MLOps/LMOps workflows, pipelines, mathematical/statistical models, algorithms, computing experiments, software configurations).
+
+* For foundation models like the GPT series, it automates the experimentation and optimization of their inference performance to maximize the effectiveness for downstream applications and minimize the inference cost.
+* For common machine learning tasks like classification and regression, it quickly finds quality models for user-provided data with low computational resources.
+* It is easy to customize or extend. Users can find their desired customizability from a smooth range: minimal customization (computational resource budget), medium customization (e.g., scikit-style learner, search space and metric), or full customization (arbitrary training/inference/evaluation code).
+* It supports fast automatic tuning, capable of handling complex constraints/guidance/early stopping. FLAML is powered by a [cost-effective
 hyperparameter optimization](https://microsoft.github.io/FLAML/docs/Use-Cases/Tune-User-Defined-Function/#hyperparameter-optimization-algorithm)
 and model selection method invented by Microsoft Research, and many followup [research studies](https://microsoft.github.io/FLAML/docs/Research).
 
 FLAML has a .NET implementation in [ML.NET](http://dot.net/ml), an open-source, cross-platform machine learning framework for .NET. In ML.NET, you can use FLAML via low-code solutions like [Model Builder](https://dotnet.microsoft.com/apps/machinelearning-ai/ml-dotnet/model-builder) Visual Studio extension and the cross-platform [ML.NET CLI](https://docs.microsoft.com/dotnet/machine-learning/automate-training-with-cli). Alternatively, you can use the [ML.NET AutoML API](https://www.nuget.org/packages/Microsoft.ML.AutoML/#versions-body-tab) for a code-first experience.
 
 
 ## Installation
@@ -89,14 +87,33 @@
 
 - [Install Model Builder](https://docs.microsoft.com/dotnet/machine-learning/how-to-guides/install-model-builder?tabs=visual-studio-2022)
 - [Install ML.NET CLI](https://docs.microsoft.com/dotnet/machine-learning/how-to-guides/install-ml-net-cli?tabs=windows)
 - [Microsoft.AutoML](https://www.nuget.org/packages/Microsoft.ML.AutoML/0.20.0)
 
 ## Quickstart
 
+* (New) You can optimize [generations](https://microsoft.github.io/FLAML/docs/Use-Cases/Auto-Generation) by ChatGPT or GPT-4 etc. with your own tuning data, success metrics and budgets.
+
+```python
+from flaml import oai
+
+config, analysis = oai.Completion.tune(
+    data=tune_data,
+    metric="success",
+    mode="max",
+    eval_func=eval_func,
+    inference_budget=0.05,
+    optimization_budget=3,
+    num_samples=-1,
+)
+```
+
+The automated experimentation and optimization can help you maximize the utility out of these expensive models.
+A suite of utilities such as caching and templating are offered to accelerate the experimentation and application development.
+
 * With three lines of code, you can start using this economical and fast
 AutoML engine as a [scikit-learn style estimator](https://microsoft.github.io/FLAML/docs/Use-Cases/Task-Oriented-AutoML).
 
 ```python
 from flaml import AutoML
 automl = AutoML()
 automl.fit(X_train, y_train, task="classification")
@@ -123,30 +140,14 @@
 
 # Use LGBMRegressor in the same way as you use lightgbm.LGBMRegressor.
 estimator = LGBMRegressor()
 # The hyperparameters are automatically set according to the training data.
 estimator.fit(X_train, y_train)
 ```
 
-* (New) You can optimize [generations](https://microsoft.github.io/FLAML/docs/Use-Cases/Auto-Generation) by ChatGPT or GPT-4 etc. with your own tuning data, success metrics and budgets.
-
-```python
-from flaml import oai
-
-config, analysis = oai.Completion.tune(
-    data=tune_data,
-    metric="success",
-    mode="max",
-    eval_func=eval_func,
-    inference_budget=0.05,
-    optimization_budget=3,
-    num_samples=-1,
-)
-```
-
 ## Documentation
 
 You can find a detailed documentation about FLAML [here](https://microsoft.github.io/FLAML/) where you can find the API documentation, use cases and examples.
 
 In addition, you can find:
 
 - Research around FLAML [here](https://microsoft.github.io/FLAML/docs/Research).
```

### Comparing `FLAML-1.2.2/FLAML.egg-info/SOURCES.txt` & `FLAML-1.2.3/FLAML.egg-info/SOURCES.txt`

 * *Files 20% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 LICENSE
 NOTICE.md
 README.md
+pyproject.toml
 setup.py
 FLAML.egg-info/PKG-INFO
 FLAML.egg-info/SOURCES.txt
 FLAML.egg-info/dependency_links.txt
 FLAML.egg-info/requires.txt
 FLAML.egg-info/top_level.txt
 flaml/__init__.py
@@ -12,14 +13,18 @@
 flaml/data.py
 flaml/ml.py
 flaml/model.py
 flaml/version.py
 flaml/autogen/__init__.py
 flaml/autogen/code_utils.py
 flaml/autogen/math_utils.py
+flaml/autogen/agent/__init__.py
+flaml/autogen/agent/agent.py
+flaml/autogen/agent/coding_agent.py
+flaml/autogen/agent/execution_agent.py
 flaml/autogen/extensions/__init__.py
 flaml/autogen/oai/__init__.py
 flaml/autogen/oai/completion.py
 flaml/automl/__init__.py
 flaml/automl/automl.py
 flaml/automl/data.py
 flaml/automl/logger.py
```

### Comparing `FLAML-1.2.2/FLAML.egg-info/requires.txt` & `FLAML-1.2.3/FLAML.egg-info/requires.txt`

 * *Files 13% similar despite different names*

```diff
@@ -66,22 +66,21 @@
 
 [synapse]
 joblibspark>=0.5.0
 optuna==2.8.0
 pyspark>=3.2.0
 
 [test]
-flake8>=3.8.4
 thop
 pytest>=6.1.1
 coverage>=5.3
 pre-commit
 torch
 torchvision
-catboost>=0.26
+catboost<1.2,>=0.26
 rgf-python
 optuna==2.8.0
 openml==0.10.2
 statsmodels>=0.12.2
 psutil==5.8.0
 dataclasses
 transformers[torch]==4.26
@@ -94,14 +93,15 @@
 mlflow
 pyspark>=3.2.0
 joblibspark>=0.5.0
 nbconvert
 nbformat
 ipykernel
 pytorch-lightning<1.9.1
+requests<2.29.0
 
 [ts_forecast]
 holidays<0.14
 prophet>=1.0.1
 statsmodels>=0.12.2
 hcrystalball==0.1.10
```

### Comparing `FLAML-1.2.2/LICENSE` & `FLAML-1.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `FLAML-1.2.2/NOTICE.md` & `FLAML-1.2.3/NOTICE.md`

 * *Files identical despite different names*

### Comparing `FLAML-1.2.2/PKG-INFO` & `FLAML-1.2.3/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: FLAML
-Version: 1.2.2
+Version: 1.2.3
 Summary: A fast library for automated machine learning and tuning
 Home-page: https://github.com/microsoft/FLAML
 Author: Microsoft Corporation
 Author-email: hpo@microsoft.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
@@ -44,26 +44,24 @@
 <p align="center">
     <img src="https://github.com/microsoft/FLAML/blob/main/website/static/img/flaml.svg"  width=200>
     <br>
 </p>
 
 :fire: v1.2.0 is released with support for ChatGPT and GPT-4.
 
-:fire: A [lab forum](https://github.com/microsoft/FLAML/tree/tutorial-aaai23/tutorial) on FLAML at AAAI 2023.
-
-:fire: A [hands-on tutorial](https://github.com/microsoft/FLAML/tree/tutorial/tutorial) on FLAML presented at KDD 2022
 
 ## What is FLAML
-FLAML is a lightweight Python library that finds accurate machine
-learning models automatically, efficiently and economically. It frees users from selecting
-models and hyperparameters for each model. It can also be used to tune generic hyperparameters for foundation models, MLOps/LMOps workflows, pipelines, mathematical/statistical models, algorithms, computing experiments, software configurations and so on.
-
-1. For common machine learning or AI tasks like classification, regression, and generation, it quickly finds quality models for user-provided data with low computational resources. It supports both classical machine learning models and deep neural networks, including foundation models such as the GPT series.
-1. It is easy to customize or extend. Users can find their desired customizability from a smooth range: minimal customization (computational resource budget), medium customization (e.g., scikit-style learner, search space and metric), or full customization (arbitrary training and evaluation code).
-1. It supports fast automatic tuning, capable of handling complex constraints/guidance/early stopping. FLAML is powered by a new, [cost-effective
+FLAML is a lightweight Python library for efficient automation of machine
+learning, including selection of
+models, hyperparameters, and other tunable choices of an application (e.g., inference hyperparameters for foundation models, configurations in MLOps/LMOps workflows, pipelines, mathematical/statistical models, algorithms, computing experiments, software configurations).
+
+* For foundation models like the GPT series, it automates the experimentation and optimization of their inference performance to maximize the effectiveness for downstream applications and minimize the inference cost.
+* For common machine learning tasks like classification and regression, it quickly finds quality models for user-provided data with low computational resources.
+* It is easy to customize or extend. Users can find their desired customizability from a smooth range: minimal customization (computational resource budget), medium customization (e.g., scikit-style learner, search space and metric), or full customization (arbitrary training/inference/evaluation code).
+* It supports fast automatic tuning, capable of handling complex constraints/guidance/early stopping. FLAML is powered by a [cost-effective
 hyperparameter optimization](https://microsoft.github.io/FLAML/docs/Use-Cases/Tune-User-Defined-Function/#hyperparameter-optimization-algorithm)
 and model selection method invented by Microsoft Research, and many followup [research studies](https://microsoft.github.io/FLAML/docs/Research).
 
 FLAML has a .NET implementation in [ML.NET](http://dot.net/ml), an open-source, cross-platform machine learning framework for .NET. In ML.NET, you can use FLAML via low-code solutions like [Model Builder](https://dotnet.microsoft.com/apps/machinelearning-ai/ml-dotnet/model-builder) Visual Studio extension and the cross-platform [ML.NET CLI](https://docs.microsoft.com/dotnet/machine-learning/automate-training-with-cli). Alternatively, you can use the [ML.NET AutoML API](https://www.nuget.org/packages/Microsoft.ML.AutoML/#versions-body-tab) for a code-first experience.
 
 
 ## Installation
@@ -89,14 +87,33 @@
 
 - [Install Model Builder](https://docs.microsoft.com/dotnet/machine-learning/how-to-guides/install-model-builder?tabs=visual-studio-2022)
 - [Install ML.NET CLI](https://docs.microsoft.com/dotnet/machine-learning/how-to-guides/install-ml-net-cli?tabs=windows)
 - [Microsoft.AutoML](https://www.nuget.org/packages/Microsoft.ML.AutoML/0.20.0)
 
 ## Quickstart
 
+* (New) You can optimize [generations](https://microsoft.github.io/FLAML/docs/Use-Cases/Auto-Generation) by ChatGPT or GPT-4 etc. with your own tuning data, success metrics and budgets.
+
+```python
+from flaml import oai
+
+config, analysis = oai.Completion.tune(
+    data=tune_data,
+    metric="success",
+    mode="max",
+    eval_func=eval_func,
+    inference_budget=0.05,
+    optimization_budget=3,
+    num_samples=-1,
+)
+```
+
+The automated experimentation and optimization can help you maximize the utility out of these expensive models.
+A suite of utilities such as caching and templating are offered to accelerate the experimentation and application development.
+
 * With three lines of code, you can start using this economical and fast
 AutoML engine as a [scikit-learn style estimator](https://microsoft.github.io/FLAML/docs/Use-Cases/Task-Oriented-AutoML).
 
 ```python
 from flaml import AutoML
 automl = AutoML()
 automl.fit(X_train, y_train, task="classification")
@@ -123,30 +140,14 @@
 
 # Use LGBMRegressor in the same way as you use lightgbm.LGBMRegressor.
 estimator = LGBMRegressor()
 # The hyperparameters are automatically set according to the training data.
 estimator.fit(X_train, y_train)
 ```
 
-* (New) You can optimize [generations](https://microsoft.github.io/FLAML/docs/Use-Cases/Auto-Generation) by ChatGPT or GPT-4 etc. with your own tuning data, success metrics and budgets.
-
-```python
-from flaml import oai
-
-config, analysis = oai.Completion.tune(
-    data=tune_data,
-    metric="success",
-    mode="max",
-    eval_func=eval_func,
-    inference_budget=0.05,
-    optimization_budget=3,
-    num_samples=-1,
-)
-```
-
 ## Documentation
 
 You can find a detailed documentation about FLAML [here](https://microsoft.github.io/FLAML/) where you can find the API documentation, use cases and examples.
 
 In addition, you can find:
 
 - Research around FLAML [here](https://microsoft.github.io/FLAML/docs/Research).
```

### Comparing `FLAML-1.2.2/README.md` & `FLAML-1.2.3/README.md`

 * *Files 10% similar despite different names*

```diff
@@ -12,26 +12,24 @@
 <p align="center">
     <img src="https://github.com/microsoft/FLAML/blob/main/website/static/img/flaml.svg"  width=200>
     <br>
 </p>
 
 :fire: v1.2.0 is released with support for ChatGPT and GPT-4.
 
-:fire: A [lab forum](https://github.com/microsoft/FLAML/tree/tutorial-aaai23/tutorial) on FLAML at AAAI 2023.
-
-:fire: A [hands-on tutorial](https://github.com/microsoft/FLAML/tree/tutorial/tutorial) on FLAML presented at KDD 2022
 
 ## What is FLAML
-FLAML is a lightweight Python library that finds accurate machine
-learning models automatically, efficiently and economically. It frees users from selecting
-models and hyperparameters for each model. It can also be used to tune generic hyperparameters for foundation models, MLOps/LMOps workflows, pipelines, mathematical/statistical models, algorithms, computing experiments, software configurations and so on.
-
-1. For common machine learning or AI tasks like classification, regression, and generation, it quickly finds quality models for user-provided data with low computational resources. It supports both classical machine learning models and deep neural networks, including foundation models such as the GPT series.
-1. It is easy to customize or extend. Users can find their desired customizability from a smooth range: minimal customization (computational resource budget), medium customization (e.g., scikit-style learner, search space and metric), or full customization (arbitrary training and evaluation code).
-1. It supports fast automatic tuning, capable of handling complex constraints/guidance/early stopping. FLAML is powered by a new, [cost-effective
+FLAML is a lightweight Python library for efficient automation of machine
+learning, including selection of
+models, hyperparameters, and other tunable choices of an application (e.g., inference hyperparameters for foundation models, configurations in MLOps/LMOps workflows, pipelines, mathematical/statistical models, algorithms, computing experiments, software configurations).
+
+* For foundation models like the GPT series, it automates the experimentation and optimization of their inference performance to maximize the effectiveness for downstream applications and minimize the inference cost.
+* For common machine learning tasks like classification and regression, it quickly finds quality models for user-provided data with low computational resources.
+* It is easy to customize or extend. Users can find their desired customizability from a smooth range: minimal customization (computational resource budget), medium customization (e.g., scikit-style learner, search space and metric), or full customization (arbitrary training/inference/evaluation code).
+* It supports fast automatic tuning, capable of handling complex constraints/guidance/early stopping. FLAML is powered by a [cost-effective
 hyperparameter optimization](https://microsoft.github.io/FLAML/docs/Use-Cases/Tune-User-Defined-Function/#hyperparameter-optimization-algorithm)
 and model selection method invented by Microsoft Research, and many followup [research studies](https://microsoft.github.io/FLAML/docs/Research).
 
 FLAML has a .NET implementation in [ML.NET](http://dot.net/ml), an open-source, cross-platform machine learning framework for .NET. In ML.NET, you can use FLAML via low-code solutions like [Model Builder](https://dotnet.microsoft.com/apps/machinelearning-ai/ml-dotnet/model-builder) Visual Studio extension and the cross-platform [ML.NET CLI](https://docs.microsoft.com/dotnet/machine-learning/automate-training-with-cli). Alternatively, you can use the [ML.NET AutoML API](https://www.nuget.org/packages/Microsoft.ML.AutoML/#versions-body-tab) for a code-first experience.
 
 
 ## Installation
@@ -57,14 +55,33 @@
 
 - [Install Model Builder](https://docs.microsoft.com/dotnet/machine-learning/how-to-guides/install-model-builder?tabs=visual-studio-2022)
 - [Install ML.NET CLI](https://docs.microsoft.com/dotnet/machine-learning/how-to-guides/install-ml-net-cli?tabs=windows)
 - [Microsoft.AutoML](https://www.nuget.org/packages/Microsoft.ML.AutoML/0.20.0)
 
 ## Quickstart
 
+* (New) You can optimize [generations](https://microsoft.github.io/FLAML/docs/Use-Cases/Auto-Generation) by ChatGPT or GPT-4 etc. with your own tuning data, success metrics and budgets.
+
+```python
+from flaml import oai
+
+config, analysis = oai.Completion.tune(
+    data=tune_data,
+    metric="success",
+    mode="max",
+    eval_func=eval_func,
+    inference_budget=0.05,
+    optimization_budget=3,
+    num_samples=-1,
+)
+```
+
+The automated experimentation and optimization can help you maximize the utility out of these expensive models.
+A suite of utilities such as caching and templating are offered to accelerate the experimentation and application development.
+
 * With three lines of code, you can start using this economical and fast
 AutoML engine as a [scikit-learn style estimator](https://microsoft.github.io/FLAML/docs/Use-Cases/Task-Oriented-AutoML).
 
 ```python
 from flaml import AutoML
 automl = AutoML()
 automl.fit(X_train, y_train, task="classification")
@@ -91,30 +108,14 @@
 
 # Use LGBMRegressor in the same way as you use lightgbm.LGBMRegressor.
 estimator = LGBMRegressor()
 # The hyperparameters are automatically set according to the training data.
 estimator.fit(X_train, y_train)
 ```
 
-* (New) You can optimize [generations](https://microsoft.github.io/FLAML/docs/Use-Cases/Auto-Generation) by ChatGPT or GPT-4 etc. with your own tuning data, success metrics and budgets.
-
-```python
-from flaml import oai
-
-config, analysis = oai.Completion.tune(
-    data=tune_data,
-    metric="success",
-    mode="max",
-    eval_func=eval_func,
-    inference_budget=0.05,
-    optimization_budget=3,
-    num_samples=-1,
-)
-```
-
 ## Documentation
 
 You can find a detailed documentation about FLAML [here](https://microsoft.github.io/FLAML/) where you can find the API documentation, use cases and examples.
 
 In addition, you can find:
 
 - Research around FLAML [here](https://microsoft.github.io/FLAML/docs/Research).
```

### Comparing `FLAML-1.2.2/flaml/autogen/code_utils.py` & `FLAML-1.2.3/flaml/autogen/code_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,29 +2,30 @@
 import subprocess
 import sys
 import os
 import pathlib
 from typing import List, Dict, Tuple, Optional, Union, Callable
 import re
 import time
+from hashlib import md5
 from flaml.autogen import oai, DEFAULT_MODEL, FAST_MODEL
 
 # Regular expression for finding a code block
-CODE_BLOCK_PATTERN = r"```\w*\n(.*?)\n```"
+CODE_BLOCK_PATTERN = r"```(\w*)\n(.*?)\n```"
 WORKING_DIR = os.path.join(os.path.dirname(os.path.realpath(__file__)), "extensions")
 
 
 def extract_code(text: str, pattern: str = CODE_BLOCK_PATTERN) -> str:
     # Use a regular expression to find the code block
     match = re.search(pattern, text, flags=re.DOTALL)
     # If a match is found, return the code
     if match:
-        return match.group(1)
+        return match.group(2), match.group(1)
     # If no code block is found, return the whole text
-    return text
+    return text, "unknown"
 
 
 def generate_code(pattern: str = CODE_BLOCK_PATTERN, **config) -> Tuple[str, float]:
     """Generate code.
 
     Args:
         pattern (Optional, str): The regular expression pattern for finding the code block.
@@ -32,15 +33,15 @@
         config (Optional, dict): The configuration for the API call.
 
     Returns:
         str: The generated code.
         float: The cost of the generation.
     """
     response = oai.Completion.create(**config)
-    cost = oai.Completion.cost(config["model"], response)
+    cost = oai.Completion.cost(response)
     return extract_code(oai.Completion.extract_text(response)[0], pattern), cost
 
 
 _IMPROVE_FUNCTION_CONFIG = {
     "prompt": """Improve the function '{func_name}' to achieve the objective '{objective}'.
 The current implementation of the function is as follows:
 {file_string}""",
@@ -54,15 +55,15 @@
     params = {**_IMPROVE_FUNCTION_CONFIG, **config}
     # read the entire file into a str
     with open(file_name, "r") as f:
         file_string = f.read()
     response = oai.Completion.create(
         {"func_name": func_name, "objective": objective, "file_string": file_string}, **params
     )
-    cost = oai.Completion.cost(params["model"], response)
+    cost = oai.Completion.cost(response)
     return oai.Completion.extract_text(response)[0], cost
 
 
 _IMPROVE_CODE_CONFIG = {
     "prompt": """Analyze the code in the following files and return a list of suggestions for improvement{followup}, to achieve the objective of '{objective}'.
 {code}
 """,
@@ -92,15 +93,15 @@
         code += f"""{file_name}:
 {file_string}
 
 """
     params = {**_IMPROVE_CODE_CONFIG, **config}
     followup = "" if suggest_only else " followed by the improved code"
     response = oai.Completion.create({"objective": objective, "code": code, "followup": followup}, **params)
-    cost = oai.Completion.cost(params["model"], response)
+    cost = oai.Completion.cost(response)
     return oai.Completion.extract_text(response)[0], cost
 
 
 def timeout_handler(signum, frame):
     raise TimeoutError("Timed out!")
 
 
@@ -137,25 +138,24 @@
         int: 0 if the code executes successfully.
         bytes: The error message if the code fails to execute; the stdout otherwise.
     """
     assert code is not None or filename is not None, "Either code or filename must be provided."
 
     original_filename = filename
     if filename is None:
-        code_hash = hash(code)
+        code_hash = md5(code.encode()).hexdigest()
         # create a file with a automatically generated name
         filename = f"tmp_code_{code_hash}.py"
     if work_dir is None:
         work_dir = WORKING_DIR
     filepath = os.path.join(work_dir, filename)
     file_dir = os.path.dirname(filepath)
     os.makedirs(file_dir, exist_ok=True)
 
     if code is not None:
-        code = code.strip()
         with open(filepath, "w") as fout:
             fout.write(code)
     # check if already running in a docker container
     in_docker_container = os.path.exists("/.dockerenv")
     if not use_docker or in_docker_container:
         # already running in a docker container
         signal.signal(signal.SIGALRM, timeout_handler)
@@ -277,15 +277,15 @@
         float: The cost of the generation.
     """
     params = {**_GENERATE_ASSERTIONS_CONFIG, **config}
     response = oai.Completion.create(
         {"definition": definition},
         **params,
     )
-    cost = oai.Completion.cost(params["model"], response)
+    cost = oai.Completion.cost(response)
     assertions = oai.Completion.extract_text(response)[0]
     return assertions, cost
 
 
 def _remove_check(response):
     """Remove the check function from the response."""
     # find the position of the check function
@@ -406,14 +406,14 @@
     """
     cost = 0
     configs = configs or _IMPLEMENT_CONFIGS
     if len(configs) > 1 and callable(assertions):
         assertions, cost = assertions(definition)
     for i, config in enumerate(configs):
         response = oai.Completion.create({"definition": definition}, **config)
-        cost += oai.Completion.cost(config["model"], response)
+        cost += oai.Completion.cost(response)
         responses = oai.Completion.extract_text(response)
         metrics = eval_function_completions(responses, definition, assertions=assertions)
         assertions = metrics["assertions"]
         cost += metrics["gen_cost"]
         if metrics["succeed_assertions"] or i == len(configs) - 1:
             return responses[metrics["index_selected"]], cost, i
```

### Comparing `FLAML-1.2.2/flaml/autogen/math_utils.py` & `FLAML-1.2.3/flaml/autogen/math_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,15 @@
         config (Optional, dict): The configuration for the API call.
 
     Returns:
         str: The solution to the problem.
     """
     params = {**_MATH_CONFIG, **config}
     response = oai.Completion.create({"problem": problem}, **params)
-    cost = oai.Completion.cost(params["model"], response)
+    cost = oai.Completion.cost(response)
     results = eval_math_responses(oai.Completion.extract_text(response))
     return results.get("voted_answer"), cost
 
 
 def remove_boxed(string: str) -> Optional[str]:
     """Source: https://github.com/hendrycks/math
     Extract the text within a \\boxed{...} environment.
```

### Comparing `FLAML-1.2.2/flaml/autogen/oai/completion.py` & `FLAML-1.2.3/flaml/autogen/oai/completion.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,31 +1,34 @@
 from time import sleep
 import logging
 import numpy as np
 import time
 from typing import List, Optional, Dict
 import sys
+import json
 from flaml import tune, BlendSearch
 from flaml.automl.logger import logger_formatter
 
 try:
     import openai
     from openai.error import (
         ServiceUnavailableError,
         RateLimitError,
         APIError,
         InvalidRequestError,
         APIConnectionError,
         Timeout,
     )
+    from openai import Completion as openai_Completion
     import diskcache
 
     ERROR = None
 except ImportError:
     ERROR = ImportError("please install flaml[openai] option to use the flaml.oai subpackage.")
+    openai_Completion = object
 logger = logging.getLogger(__name__)
 if not logger.handlers:
     # Add the console handler.
     _ch = logging.StreamHandler(stream=sys.stdout)
     _ch.setFormatter(logger_formatter)
     logger.addHandler(_ch)
 
@@ -35,22 +38,23 @@
 
     Args:
         config (dict or list): A configuration.
 
     Returns:
         tuple: A unique identifier which can be used as a key for a dict.
     """
-    if isinstance(config, dict):
-        return tuple(get_key(x) for x in sorted(config.items()))
-    if isinstance(config, list):
-        return tuple(get_key(x) for x in config)
-    return config
+    # if isinstance(config, dict):
+    #     return tuple(get_key(x) for x in sorted(config.items()))
+    # if isinstance(config, list):
+    #     return tuple(get_key(x) for x in config)
+    # return config
+    return json.dumps(config, sort_keys=True)
 
 
-class Completion:
+class Completion(openai_Completion):
     """A class for OpenAI completion API.
 
     It also supports: ChatCompletion, Azure OpenAI API.
     """
 
     # set of models that support chat completion
     chat_models = {
@@ -111,85 +115,130 @@
     # time out for request to openai server
     request_timeout = 60
 
     openai_completion_class = not ERROR and openai.Completion
     _total_cost = 0
     optimization_budget = None
 
+    _history_dict = _count_create = None
+
     @classmethod
     def set_cache(cls, seed=41, cache_path=".cache"):
         """Set cache path.
 
         Args:
             seed (int, Optional): The integer identifier for the pseudo seed.
                 Results corresponding to different seeds will be cached in different places.
             cache_path (str, Optional): The root path for the cache.
                 The complete cache path will be {cache_path}/{seed}.
         """
         cls.seed = seed
         cls.cache_path = f"{cache_path}/{seed}"
 
     @classmethod
-    def _get_response(cls, config: dict, eval_only=False, use_cache=True):
+    def _book_keeping(cls, config: Dict, response):
+        """Book keeping for the created completions."""
+        if cls._history_dict is None:
+            return
+        if cls._history_compact:
+            value = {
+                "created_at": [],
+                "cost": [],
+            }
+            if "messages" in config:
+                messages = config["messages"]
+                if len(messages) > 1 and messages[-1]["role"] != "assistant":
+                    existing_key = get_key(messages[:-1])
+                    value = cls._history_dict.pop(existing_key, value)
+                key = get_key(messages + [choice["message"] for choice in response["choices"]])
+            else:
+                key = get_key([config["prompt"]] + [choice.get("text") for choice in response["choices"]])
+            value["created_at"].append(cls._count_create)
+            value["cost"].append(cls.cost(response))
+            cls._history_dict[key] = value
+            cls._count_create += 1
+            return
+        cls._history_dict[cls._count_create] = {
+            "request": config,
+            "response": response.to_dict_recursive(),
+        }
+        cls._count_create += 1
+
+    @classmethod
+    def _get_response(cls, config: Dict, eval_only=False, use_cache=True):
         """Get the response from the openai api call.
 
         Try cache first. If not found, call the openai api. If the api call fails, retry after retry_time.
         """
+        config = config.copy()
+        openai.api_key = config.pop("api_key", openai.api_key)
+        openai.api_base = config.pop("api_base", openai.api_base)
+        openai.api_key_path = config.pop("api_key_path", openai.api_key_path)
+        openai.api_type = config.pop("api_type", openai.api_type)
+        openai.api_version = config.pop("api_version", openai.api_version)
         key = get_key(config)
         if use_cache:
             response = cls._cache.get(key, None)
             if response is not None and (response != -1 or not eval_only):
                 # print("using cached response")
+                cls._book_keeping(config, response)
                 return response
         openai_completion = openai.ChatCompletion if config["model"] in cls.chat_models else openai.Completion
         start_time = time.time()
         request_timeout = cls.request_timeout
         while True:
             try:
                 if "request_timeout" in config:
                     response = openai_completion.create(**config)
                 else:
                     response = openai_completion.create(request_timeout=request_timeout, **config)
             except (
                 ServiceUnavailableError,
-                APIError,
                 APIConnectionError,
             ):
                 # transient error
                 logger.warning(f"retrying in {cls.retry_time} seconds...", exc_info=1)
                 sleep(cls.retry_time)
-            except (RateLimitError, Timeout) as e:
+            except APIError as err:
+                error_code = err and err.json_body and err.json_body.get("error")
+                error_code = error_code and error_code.get("code")
+                if error_code == "content_filter":
+                    raise
+                # transient error
+                logger.warning(f"retrying in {cls.retry_time} seconds...", exc_info=1)
+                sleep(cls.retry_time)
+            except (RateLimitError, Timeout) as err:
                 time_left = cls.retry_timeout - (time.time() - start_time + cls.retry_time)
                 if (
                     time_left > 0
-                    and isinstance(e, RateLimitError)
+                    and isinstance(err, RateLimitError)
                     or time_left > request_timeout
-                    and isinstance(e, Timeout)
+                    and isinstance(err, Timeout)
                 ):
                     logger.info(f"retrying in {cls.retry_time} seconds...", exc_info=1)
                 elif eval_only:
                     raise
                 else:
                     break
-                if isinstance(e, Timeout):
+                if isinstance(err, Timeout):
                     if "request_timeout" in config:
                         raise
                     request_timeout <<= 1
                 request_timeout = min(request_timeout, time_left)
                 sleep(cls.retry_time)
             except InvalidRequestError:
                 if "azure" == openai.api_type and "model" in config:
                     # azure api uses "engine" instead of "model"
-                    config = config.copy()
                     config["engine"] = config.pop("model").replace("gpt-3.5-turbo", "gpt-35-turbo")
                 else:
                     raise
             else:
                 if use_cache:
                     cls._cache.set(key, response)
+                cls._book_keeping(config, response)
                 return response
         logger.warning(
             f"Failed to get response from openai api due to getting RateLimitError or Timeout for {cls.retry_timeout} seconds."
         )
         response = -1
         if use_cache:
             cls._cache.set(key, response)
@@ -623,35 +672,89 @@
         temperature_or_top_p = params.pop("temperature_or_top_p", None)
         if temperature_or_top_p:
             params.update(temperature_or_top_p)
         logger.setLevel(old_level)
         return params, analysis
 
     @classmethod
-    def create(cls, context: Optional[Dict] = None, use_cache: Optional[bool] = True, **config):
+    def create(
+        cls,
+        context: Optional[Dict] = None,
+        use_cache: Optional[bool] = True,
+        config_list: Optional[List] = None,
+        **config,
+    ):
         """Make a completion for a given context.
 
         Args:
-            context (dict, Optional): The context to instantiate the prompt.
+            context (Dict, Optional): The context to instantiate the prompt.
                 It needs to contain keys that are used by the prompt template.
-                E.g., `prompt="Complete the following sentence: {prefix}"`.
-                `context={"prefix": "Today I feel"}`.
-                The actual prompt sent to OpenAI will be:
+                E.g., `prompt="Complete the following sentence: {prefix}, context={"prefix": "Today I feel"}`.
+                The actual prompt will be:
                 "Complete the following sentence: Today I feel".
+                More examples can be found at [templating](/docs/Use-Cases/Auto-Generation#templating).
             use_cache (bool, Optional): Whether to use cached responses.
+            config_list (List, Optional): List of configurations for the completion to try.
+                The first one that does not raise an error will be used.
+                Only the differences from the default config need to be provided.
+                E.g.,
+
+        ```python
+        response = oai.Completion.create(
+            config_list=[
+                {
+                    "model": "gpt-4",
+                    "api_key": os.environ.get("AZURE_OPENAI_API_KEY"),
+                    "api_type": "azure",
+                    "api_base": os.environ.get("AZURE_OPENAI_API_BASE"),
+                    "api_version": "2023-03-15-preview",
+                },
+                {
+                    "model": "gpt-3.5-turbo",
+                    "api_key": os.environ.get("OPENAI_API_KEY"),
+                    "api_type": "open_ai",
+                    "api_base": "https://api.openai.com/v1",
+                    "api_version": None,
+                },
+                {
+                    "model": "llama-7B",
+                    "api_base": "http://127.0.0.1:8080",
+                    "api_type": "open_ai",
+                    "api_version": None,
+                }
+            ],
+            prompt="Hi",
+        )
+        ```
+
             **config: Configuration for the completion.
                 Besides the parameters for the openai API call, it can also contain a seed (int) for the cache.
                 This is useful when implementing "controlled randomness" for the completion.
                 Also, the "prompt" or "messages" parameter can contain a template (str or Callable) which will be instantiated with the context.
 
         Returns:
             Responses from OpenAI API.
         """
         if ERROR:
             raise ERROR
+        if config_list:
+            retry_timeout = cls.retry_timeout
+            for i, each_config in enumerate(config_list):
+                base_config = config.copy()
+                base_config.update(each_config)
+                try:
+                    cls.retry_timeout = 0 if i < len(config_list) - 1 else retry_timeout
+                    # retry_timeout = 0 to avoid retrying
+                    return cls.create(context, use_cache, **base_config)
+                except (RateLimitError, Timeout):
+                    logger.info(f"failed with config {i}", exc_info=1)
+                    if i == len(config_list) - 1:
+                        raise
+                finally:
+                    cls.retry_timeout = retry_timeout
         params = cls._construct_params(context, config)
         if not use_cache:
             return cls._get_response(params, eval_only=True, use_cache=False)
         seed = cls.seed
         if "seed" in params:
             cls.set_cache(params.pop("seed"))
         with diskcache.Cache(cls.cache_path) as cls._cache:
@@ -768,21 +871,20 @@
             None when no valid eval_func is provided in either test or tune;
             Otherwise, a dict of aggregated results, responses and per instance results if `return_responses_and_per_instance_result` is True;
             Otherwise, a dict of aggregated results (responses and per instance results are not returned).
         """
         result_agg, responses_list, result_list = {}, [], []
         metric_keys = None
         cost = 0
-        model = config["model"]
         old_level = logger.getEffectiveLevel()
         logger.setLevel(logging_level)
         for i, data_i in enumerate(data):
             logger.info(f"evaluating data instance {i}")
             response = cls.create(data_i, use_cache, **config)
-            cost += cls.cost(model, response)
+            cost += cls.cost(response)
             # evaluate the quality of the responses
             responses = cls.extract_text(response)
             if eval_func is not None:
                 metrics = eval_func(responses, **data_i)
             elif hasattr(cls, "_eval_func"):
                 metrics = cls._eval_func(responses, **data_i)
             else:
@@ -833,24 +935,24 @@
             result_agg["inference_cost"] = cost / len(data)
         if return_responses_and_per_instance_result:
             return result_agg, result_list, responses_list
         else:
             return result_agg
 
     @classmethod
-    def cost(cls, model: str, response: dict):
+    def cost(cls, response: dict):
         """Compute the cost of an API call.
 
         Args:
-            model (str): The model name.
             response (dict): The response from OpenAI API.
 
         Returns:
             The cost in USD.
         """
+        model = response["model"]
         if model not in cls.price1K:
             raise ValueError(f"Unknown model: {model}")
         usage = response["usage"]
         n_input_tokens = usage["prompt_tokens"]
         n_output_tokens = usage.get("completion_tokens", 0)
         price1K = cls.price1K[model]
         if isinstance(price1K, tuple):
@@ -868,14 +970,76 @@
             A list of text in the responses.
         """
         choices = response["choices"]
         if "text" in choices[0]:
             return [choice["text"] for choice in choices]
         return [choice["message"].get("content", "") for choice in choices]
 
+    @classmethod
+    @property
+    def logged_history(cls) -> Dict:
+        """Return the book keeping dictionary."""
+        return cls._history_dict
+
+    @classmethod
+    def start_logging(
+        cls, history_dict: Optional[Dict] = None, compact: Optional[bool] = True, reset_counter: Optional[bool] = True
+    ):
+        """Start book keeping.
+
+        Args:
+            history_dict (Dict): A dictionary for book keeping.
+                If no provided, a new one will be created.
+            compact (bool): Whether to keep the history dictionary compact.
+                Compact history contains one key per conversation, and the value is a dictionary
+                like:
+        ```python
+        {
+            "create_at": [0, 1],
+            "cost": [0.1, 0.2],
+        }
+        ```
+                where "created_at" is the index of API calls indicating the order of all the calls,
+                and "cost" is the cost of each call. This example shows that the conversation is based
+                on two API calls. The compact format is useful for condensing the history of a conversation.
+                If compact is False, the history dictionary will contain all the API calls: the key
+                is the index of the API call, and the value is a dictionary like:
+        ```python
+        {
+            "request": request_dict,
+            "response": response_dict,
+        }
+        ```
+                where request_dict is the request sent to OpenAI API, and response_dict is the response.
+                For a conversation containing two API calls, the non-compact history dictionary will be like:
+        ```python
+        {
+            0: {
+                "request": request_dict_0,
+                "response": response_dict_0,
+            },
+            1: {
+                "request": request_dict_1,
+                "response": response_dict_1,
+            },
+        ```
+                The first request's messages plus the response is equal to the second request's messages.
+                For a conversation with many turns, the non-compact history dictionary has a quadratic size
+                while the compact history dict has a linear size.
+            reset_counter (bool): whether to reset the counter of the number of API calls.
+        """
+        cls._history_dict = {} if history_dict is None else history_dict
+        cls._history_compact = compact
+        cls._count_create = 0 if reset_counter or cls._count_create is None else cls._count_create
+
+    @classmethod
+    def stop_logging(cls):
+        """End book keeping."""
+        cls._history_dict = cls._count_create = None
+
 
 class ChatCompletion(Completion):
     """A class for OpenAI API ChatCompletion."""
 
     default_search_space = Completion.default_search_space.copy()
     default_search_space["model"] = tune.choice(["gpt-3.5-turbo", "gpt-4"])
     openai_completion_class = not ERROR and openai.ChatCompletion
```

### Comparing `FLAML-1.2.2/flaml/automl/automl.py` & `FLAML-1.2.3/flaml/automl/automl.py`

 * *Files 2% similar despite different names*

```diff
@@ -337,14 +337,17 @@
         fit_kwargs_by_estimator = {
             "transformer": {
                 "output_dir": "test/data/output/",
                 "fp16": False,
             }
         }
         ```
+            mlflow_logging: boolean, default=True | Whether to log the training results to mlflow.
+                This requires mlflow to be installed and to have an active mlflow run.
+                FLAML will create nested runs.
 
         """
         self._track_iter = 0
         self._state = AutoMLState()
         self._state.learner_classes = {}
         self._settings = settings
         # no budget by default
@@ -386,14 +389,15 @@
             raise ValueError("use_ray and use_spark cannot be both True.")
         settings["free_mem_ratio"] = settings.get("free_mem_ratio", 0)
         settings["metric_constraints"] = settings.get("metric_constraints", [])
         settings["cv_score_agg_func"] = settings.get("cv_score_agg_func", None)
         settings["fit_kwargs_by_estimator"] = settings.get("fit_kwargs_by_estimator", {})
         settings["custom_hp"] = settings.get("custom_hp", {})
         settings["skip_transform"] = settings.get("skip_transform", False)
+        settings["mlflow_logging"] = settings.get("mlflow_logging", True)
 
         self._estimator_type = "classifier" if settings["task"] in CLASSIFICATION else "regressor"
 
     def get_params(self, deep: bool = False) -> dict:
         return self._settings.copy()
 
     @property
@@ -1209,14 +1213,15 @@
         use_ray=None,
         use_spark=None,
         free_mem_ratio=0,
         metric_constraints=None,
         custom_hp=None,
         cv_score_agg_func=None,
         skip_transform=None,
+        mlflow_logging=None,
         fit_kwargs_by_estimator=None,
         **fit_kwargs,
     ):
         """Find a model for a given task.
 
         Args:
             X_train: A numpy array or a pandas dataframe of training data in
@@ -1470,14 +1475,19 @@
                     if isinstance(metrics_to_log, dict)
                     else metrics_to_log / n
                 )
             return metric_to_minimize, metrics_to_log
         ```
 
             skip_transform: boolean, default=False | Whether to pre-process data prior to modeling.
+            mlflow_logging: boolean, default=None | Whether to log the training results to mlflow.
+                Default value is None, which means the logging decision is made based on
+                AutoML.__init__'s mlflow_logging argument.
+                This requires mlflow to be installed and to have an active mlflow run.
+                FLAML will create nested runs.
             fit_kwargs_by_estimator: dict, default=None | The user specified keywords arguments, grouped by estimator name.
                 For TransformersEstimator, available fit_kwargs can be found from
                 [TrainingArgumentsForAuto](nlp/huggingface/training_args).
                 e.g.,
 
         ```python
         fit_kwargs_by_estimator = {
@@ -1655,14 +1665,15 @@
         self._state.free_mem_ratio = self._settings.get("free_mem_ratio") if free_mem_ratio is None else free_mem_ratio
         self._state.task = task
         self._state.log_training_metric = log_training_metric
 
         self._state.fit_kwargs = fit_kwargs
         custom_hp = custom_hp or self._settings.get("custom_hp")
         self._skip_transform = self._settings.get("skip_transform") if skip_transform is None else skip_transform
+        self._mlflow_logging = self._settings.get("mlflow_logging") if mlflow_logging is None else mlflow_logging
         fit_kwargs_by_estimator = fit_kwargs_by_estimator or self._settings.get("fit_kwargs_by_estimator")
         self._state.fit_kwargs_by_estimator = fit_kwargs_by_estimator.copy()  # shallow copy of fit_kwargs_by_estimator
         self._state.weight_val = sample_weight_val
 
         task.validate_data(
             self,
             self._state,
@@ -2135,15 +2146,15 @@
                 search_state.trial_time,
                 self._state.time_from_start,
                 search_state.val_loss,
                 search_state.config,
                 estimator,
                 search_state.sample_size,
             )
-        if mlflow is not None and mlflow.active_run():
+        if self._mlflow_logging and mlflow is not None and mlflow.active_run():
             with mlflow.start_run(nested=True):
                 mlflow.log_metric("iter_counter", self._track_iter)
                 if (search_state.metric_for_logging is not None) and (
                     "intermediate_results" in search_state.metric_for_logging
                 ):
                     for each_entry in search_state.metric_for_logging["intermediate_results"]:
                         with mlflow.start_run(nested=True):
```

### Comparing `FLAML-1.2.2/flaml/automl/data.py` & `FLAML-1.2.3/flaml/automl/data.py`

 * *Files identical despite different names*

### Comparing `FLAML-1.2.2/flaml/automl/ml.py` & `FLAML-1.2.3/flaml/automl/ml.py`

 * *Files identical despite different names*

### Comparing `FLAML-1.2.2/flaml/automl/model.py` & `FLAML-1.2.3/flaml/automl/model.py`

 * *Files 1% similar despite different names*

```diff
@@ -1131,15 +1131,15 @@
         test_dataset = Dataset.from_pandas(X_test)
 
         new_trainer = self._init_model_for_predict()
         try:
             predictions = new_trainer.predict(test_dataset).predictions
         except ZeroDivisionError:
             logger.warning("Zero division error appeared in HuggingFace Transformers.")
-            predictions = np.array([-0.05] * len(test_dataset))
+            predictions = None
         return predictions
 
     def score(self, X_val: DataFrame, y_val: Series, **kwargs):
         import transformers
 
         transformers.logging.set_verbosity_error()
 
@@ -1167,15 +1167,15 @@
         new_trainer = self._init_model_for_predict()
 
         kwargs = {} if self._task not in NLG_TASKS else {"metric_key_prefix": "predict"}
         try:
             predictions = new_trainer.predict(test_dataset, **kwargs).predictions
         except ZeroDivisionError:
             logger.warning("Zero division error appeared in HuggingFace Transformers.")
-            predictions = np.array([0] * len(test_dataset))
+            predictions = None
         post_y_pred, _ = postprocess_prediction_and_true(
             task=self._task,
             y_pred=predictions,
             tokenizer=self.tokenizer,
             hf_args=self._training_args,
             X=X,
         )
@@ -2320,18 +2320,15 @@
         if (
             self.params["seasonal"] == "mul" and (train_df.y == 0).sum() > 0
         ):  # cannot have multiplicative seasonality in this case
             self.params["seasonal"] = "add"
         if self.params["trend"] == "mul" and (train_df.y == 0).sum() > 0:
             self.params["trend"] = "add"
 
-        if not self.params["seasonal"] or not self.params["trend"] in [
-            "mul",
-            "add",
-        ]:
+        if not self.params["seasonal"] or self.params["trend"] not in ["mul", "add"]:
             self.params["damped_trend"] = False
 
         model = HWExponentialSmoothing(
             train_df[[TS_VALUE_COL]],
             damped_trend=self.params["damped_trend"],
             seasonal=self.params["seasonal"],
             trend=self.params["trend"],
```

### Comparing `FLAML-1.2.2/flaml/automl/nlp/huggingface/data_collator.py` & `FLAML-1.2.3/flaml/automl/nlp/huggingface/data_collator.py`

 * *Files identical despite different names*

### Comparing `FLAML-1.2.2/flaml/automl/nlp/huggingface/trainer.py` & `FLAML-1.2.3/flaml/automl/nlp/huggingface/trainer.py`

 * *Files identical despite different names*

### Comparing `FLAML-1.2.2/flaml/automl/nlp/huggingface/training_args.py` & `FLAML-1.2.3/flaml/automl/nlp/huggingface/training_args.py`

 * *Files identical despite different names*

### Comparing `FLAML-1.2.2/flaml/automl/nlp/huggingface/utils.py` & `FLAML-1.2.3/flaml/automl/nlp/huggingface/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -307,14 +307,16 @@
         return [tokenized_example[x] for x in tmp_column_names], tmp_column_names
     else:
         return [tokenized_example[x] for x in tmp_column_names]
 
 
 def postprocess_prediction_and_true(task, y_pred, tokenizer, hf_args, y_true=None, X=None):
     # postprocess the matrix prediction y_pred and ground truth y_true into user readable format, e.g., for summarization, decode into text
+    if y_pred is None:
+        return np.array([0.0] * len(X)), y_true
     if task == SEQCLASSIFICATION:
         return np.argmax(y_pred, axis=1), y_true
     elif task == SEQREGRESSION:
         return np.squeeze(y_pred), y_true  # predictions.reshape((len(predictions),))
     elif task == TOKENCLASSIFICATION:
         assert (y_true is not None) or (X is not None), "One of y_true and X must not be None"
         ## If y_true is not None, we use y_true to remove the -100 in the prediction (postprocessing), and return the postprocessed y_true and prediction
```

### Comparing `FLAML-1.2.2/flaml/automl/nlp/utils.py` & `FLAML-1.2.3/flaml/automl/nlp/utils.py`

 * *Files identical despite different names*

### Comparing `FLAML-1.2.2/flaml/automl/spark/configs.py` & `FLAML-1.2.3/flaml/automl/spark/configs.py`

 * *Files identical despite different names*

### Comparing `FLAML-1.2.2/flaml/automl/spark/metrics.py` & `FLAML-1.2.3/flaml/automl/spark/metrics.py`

 * *Files identical despite different names*

### Comparing `FLAML-1.2.2/flaml/automl/spark/utils.py` & `FLAML-1.2.3/flaml/automl/spark/utils.py`

 * *Files identical despite different names*

### Comparing `FLAML-1.2.2/flaml/automl/state.py` & `FLAML-1.2.3/flaml/automl/state.py`

 * *Files identical despite different names*

### Comparing `FLAML-1.2.2/flaml/automl/task/generic_task.py` & `FLAML-1.2.3/flaml/automl/task/generic_task.py`

 * *Files identical despite different names*

### Comparing `FLAML-1.2.2/flaml/automl/task/task.py` & `FLAML-1.2.3/flaml/automl/task/task.py`

 * *Files identical despite different names*

### Comparing `FLAML-1.2.2/flaml/automl/training_log.py` & `FLAML-1.2.3/flaml/automl/training_log.py`

 * *Files identical despite different names*

### Comparing `FLAML-1.2.2/flaml/automl/utils.py` & `FLAML-1.2.3/flaml/automl/utils.py`

 * *Files identical despite different names*

### Comparing `FLAML-1.2.2/flaml/default/all/binary.json` & `FLAML-1.2.3/flaml/default/all/binary.json`

 * *Files identical despite different names*

### Comparing `FLAML-1.2.2/flaml/default/all/multiclass.json` & `FLAML-1.2.3/flaml/default/all/multiclass.json`

 * *Files identical despite different names*

### Comparing `FLAML-1.2.2/flaml/default/all/regression.json` & `FLAML-1.2.3/flaml/default/all/regression.json`

 * *Files identical despite different names*

### Comparing `FLAML-1.2.2/flaml/default/estimator.py` & `FLAML-1.2.3/flaml/default/estimator.py`

 * *Files identical despite different names*

### Comparing `FLAML-1.2.2/flaml/default/extra_tree/binary.json` & `FLAML-1.2.3/flaml/default/extra_tree/binary.json`

 * *Files identical despite different names*

### Comparing `FLAML-1.2.2/flaml/default/extra_tree/multiclass.json` & `FLAML-1.2.3/flaml/default/extra_tree/multiclass.json`

 * *Files identical despite different names*

### Comparing `FLAML-1.2.2/flaml/default/extra_tree/regression.json` & `FLAML-1.2.3/flaml/default/extra_tree/regression.json`

 * *Files identical despite different names*

### Comparing `FLAML-1.2.2/flaml/default/greedy.py` & `FLAML-1.2.3/flaml/default/greedy.py`

 * *Files identical despite different names*

### Comparing `FLAML-1.2.2/flaml/default/lgbm/binary.json` & `FLAML-1.2.3/flaml/default/lgbm/binary.json`

 * *Files identical despite different names*

### Comparing `FLAML-1.2.2/flaml/default/lgbm/multiclass.json` & `FLAML-1.2.3/flaml/default/lgbm/multiclass.json`

 * *Files identical despite different names*

### Comparing `FLAML-1.2.2/flaml/default/lgbm/regression.json` & `FLAML-1.2.3/flaml/default/lgbm/regression.json`

 * *Files identical despite different names*

### Comparing `FLAML-1.2.2/flaml/default/portfolio.py` & `FLAML-1.2.3/flaml/default/portfolio.py`

 * *Files identical despite different names*

### Comparing `FLAML-1.2.2/flaml/default/regret.py` & `FLAML-1.2.3/flaml/default/regret.py`

 * *Files identical despite different names*

### Comparing `FLAML-1.2.2/flaml/default/rf/binary.json` & `FLAML-1.2.3/flaml/default/rf/binary.json`

 * *Files identical despite different names*

### Comparing `FLAML-1.2.2/flaml/default/rf/multiclass.json` & `FLAML-1.2.3/flaml/default/rf/multiclass.json`

 * *Files identical despite different names*

### Comparing `FLAML-1.2.2/flaml/default/rf/regression.json` & `FLAML-1.2.3/flaml/default/rf/regression.json`

 * *Files identical despite different names*

### Comparing `FLAML-1.2.2/flaml/default/suggest.py` & `FLAML-1.2.3/flaml/default/suggest.py`

 * *Files identical despite different names*

### Comparing `FLAML-1.2.2/flaml/default/xgb_limitdepth/binary.json` & `FLAML-1.2.3/flaml/default/xgb_limitdepth/binary.json`

 * *Files identical despite different names*

### Comparing `FLAML-1.2.2/flaml/default/xgb_limitdepth/multiclass.json` & `FLAML-1.2.3/flaml/default/xgb_limitdepth/multiclass.json`

 * *Files identical despite different names*

### Comparing `FLAML-1.2.2/flaml/default/xgb_limitdepth/regression.json` & `FLAML-1.2.3/flaml/default/xgb_limitdepth/regression.json`

 * *Files identical despite different names*

### Comparing `FLAML-1.2.2/flaml/default/xgboost/binary.json` & `FLAML-1.2.3/flaml/default/xgboost/binary.json`

 * *Files identical despite different names*

### Comparing `FLAML-1.2.2/flaml/default/xgboost/multiclass.json` & `FLAML-1.2.3/flaml/default/xgboost/multiclass.json`

 * *Files identical despite different names*

### Comparing `FLAML-1.2.2/flaml/default/xgboost/regression.json` & `FLAML-1.2.3/flaml/default/xgboost/regression.json`

 * *Files identical despite different names*

### Comparing `FLAML-1.2.2/flaml/onlineml/autovw.py` & `FLAML-1.2.3/flaml/onlineml/autovw.py`

 * *Files identical despite different names*

### Comparing `FLAML-1.2.2/flaml/onlineml/trial.py` & `FLAML-1.2.3/flaml/onlineml/trial.py`

 * *Files identical despite different names*

### Comparing `FLAML-1.2.2/flaml/onlineml/trial_runner.py` & `FLAML-1.2.3/flaml/onlineml/trial_runner.py`

 * *Files identical despite different names*

### Comparing `FLAML-1.2.2/flaml/tune/__init__.py` & `FLAML-1.2.3/flaml/tune/__init__.py`

 * *Files identical despite different names*

### Comparing `FLAML-1.2.2/flaml/tune/analysis.py` & `FLAML-1.2.3/flaml/tune/analysis.py`

 * *Files identical despite different names*

### Comparing `FLAML-1.2.2/flaml/tune/result.py` & `FLAML-1.2.3/flaml/tune/result.py`

 * *Files identical despite different names*

### Comparing `FLAML-1.2.2/flaml/tune/sample.py` & `FLAML-1.2.3/flaml/tune/sample.py`

 * *Files identical despite different names*

### Comparing `FLAML-1.2.2/flaml/tune/scheduler/online_scheduler.py` & `FLAML-1.2.3/flaml/tune/scheduler/online_scheduler.py`

 * *Files identical despite different names*

### Comparing `FLAML-1.2.2/flaml/tune/scheduler/trial_scheduler.py` & `FLAML-1.2.3/flaml/tune/scheduler/trial_scheduler.py`

 * *Files identical despite different names*

### Comparing `FLAML-1.2.2/flaml/tune/searcher/blendsearch.py` & `FLAML-1.2.3/flaml/tune/searcher/blendsearch.py`

 * *Files identical despite different names*

### Comparing `FLAML-1.2.2/flaml/tune/searcher/cfo_cat.py` & `FLAML-1.2.3/flaml/tune/searcher/cfo_cat.py`

 * *Files identical despite different names*

### Comparing `FLAML-1.2.2/flaml/tune/searcher/flow2.py` & `FLAML-1.2.3/flaml/tune/searcher/flow2.py`

 * *Files identical despite different names*

### Comparing `FLAML-1.2.2/flaml/tune/searcher/online_searcher.py` & `FLAML-1.2.3/flaml/tune/searcher/online_searcher.py`

 * *Files identical despite different names*

### Comparing `FLAML-1.2.2/flaml/tune/searcher/search_thread.py` & `FLAML-1.2.3/flaml/tune/searcher/search_thread.py`

 * *Files identical despite different names*

### Comparing `FLAML-1.2.2/flaml/tune/searcher/suggestion.py` & `FLAML-1.2.3/flaml/tune/searcher/suggestion.py`

 * *Files identical despite different names*

### Comparing `FLAML-1.2.2/flaml/tune/searcher/variant_generator.py` & `FLAML-1.2.3/flaml/tune/searcher/variant_generator.py`

 * *Files identical despite different names*

### Comparing `FLAML-1.2.2/flaml/tune/space.py` & `FLAML-1.2.3/flaml/tune/space.py`

 * *Files identical despite different names*

### Comparing `FLAML-1.2.2/flaml/tune/spark/utils.py` & `FLAML-1.2.3/flaml/tune/spark/utils.py`

 * *Files identical despite different names*

### Comparing `FLAML-1.2.2/flaml/tune/trial.py` & `FLAML-1.2.3/flaml/tune/trial.py`

 * *Files identical despite different names*

### Comparing `FLAML-1.2.2/flaml/tune/trial_runner.py` & `FLAML-1.2.3/flaml/tune/trial_runner.py`

 * *Files identical despite different names*

### Comparing `FLAML-1.2.2/flaml/tune/tune.py` & `FLAML-1.2.3/flaml/tune/tune.py`

 * *Files 0% similar despite different names*

```diff
@@ -643,22 +643,18 @@
         The final number of concurrent trials is the minimum of `max_concurrent` and
         `num_executors` if `n_concurrent_trials<=0` (default, automl cases), otherwise the
         minimum of `max_concurrent` and `n_concurrent_trials` (tuning cases).
         """
         time_start = time.time()
         try:
             FLAML_MAX_CONCURRENT = int(os.getenv("FLAML_MAX_CONCURRENT", 0))
-            num_executors = max(num_executors, FLAML_MAX_CONCURRENT, 1)
         except ValueError:
             FLAML_MAX_CONCURRENT = 0
-        max_spark_parallelism = (
-            min(spark.sparkContext.defaultParallelism, FLAML_MAX_CONCURRENT)
-            if FLAML_MAX_CONCURRENT > 0
-            else spark.sparkContext.defaultParallelism
-        )
+        num_executors = max(num_executors, FLAML_MAX_CONCURRENT, 1)
+        max_spark_parallelism = max(spark.sparkContext.defaultParallelism, FLAML_MAX_CONCURRENT)
         if scheduler:
             scheduler.set_search_properties(metric=metric, mode=mode)
         if isinstance(search_alg, ConcurrencyLimiter):
             max_concurrent = max(1, search_alg.max_concurrent)
         else:
             max_concurrent = max(1, max_spark_parallelism)
         n_concurrent_trials = min(
```

### Comparing `FLAML-1.2.2/flaml/tune/utils.py` & `FLAML-1.2.3/flaml/tune/utils.py`

 * *Files identical despite different names*

### Comparing `FLAML-1.2.2/setup.py` & `FLAML-1.2.3/setup.py`

 * *Files 6% similar despite different names*

```diff
@@ -45,22 +45,21 @@
             "openml==0.10.2",
         ],
         "spark": [
             "pyspark>=3.2.0",
             "joblibspark>=0.5.0",
         ],
         "test": [
-            "flake8>=3.8.4",
             "thop",
             "pytest>=6.1.1",
             "coverage>=5.3",
             "pre-commit",
             "torch",
             "torchvision",
-            "catboost>=0.26",
+            "catboost>=0.26,<1.2",
             "rgf-python",
             "optuna==2.8.0",
             "openml==0.10.2",
             "statsmodels>=0.12.2",
             "psutil==5.8.0",
             "dataclasses",
             "transformers[torch]==4.26",
@@ -73,14 +72,15 @@
             "mlflow",
             "pyspark>=3.2.0",
             "joblibspark>=0.5.0",
             "nbconvert",
             "nbformat",
             "ipykernel",
             "pytorch-lightning<1.9.1",  # test_forecast_panel
+            "requests<2.29.0",  # https://github.com/docker/docker-py/issues/3113
         ],
         "catboost": ["catboost>=0.26"],
         "blendsearch": ["optuna==2.8.0"],
         "ray": [
             "ray[tune]~=1.13",
         ],
         "azureml": [
```

### Comparing `FLAML-1.2.2/test/test_autovw.py` & `FLAML-1.2.3/test/test_autovw.py`

 * *Files identical despite different names*

### Comparing `FLAML-1.2.2/test/test_conda_distribution.py` & `FLAML-1.2.3/test/test_conda_distribution.py`

 * *Files identical despite different names*

### Comparing `FLAML-1.2.2/test/test_gpu.py` & `FLAML-1.2.3/test/test_gpu.py`

 * *Files identical despite different names*

### Comparing `FLAML-1.2.2/test/test_model.py` & `FLAML-1.2.3/test/test_model.py`

 * *Files identical despite different names*

