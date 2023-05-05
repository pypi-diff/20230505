# Comparing `tmp/syngen-0.0.97.tar.gz` & `tmp/syngen-0.0.98.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "syngen-0.0.97.tar", last modified: Fri Apr 28 13:33:01 2023, max compression
+gzip compressed data, was "syngen-0.0.98.tar", last modified: Fri May  5 17:23:39 2023, max compression
```

## Comparing `syngen-0.0.97.tar` & `syngen-0.0.98.tar`

### file list

```diff
@@ -1,78 +1,78 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-28 13:33:01.838267 syngen-0.0.97/
--rw-r--r--   0 runner    (1001) docker     (122)      400 2023-04-28 13:31:35.000000 syngen-0.0.97/DESCRIPTION
--rw-r--r--   0 runner    (1001) docker     (122)    35149 2023-04-28 13:31:35.000000 syngen-0.0.97/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)      133 2023-04-28 13:31:35.000000 syngen-0.0.97/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)    14888 2023-04-28 13:33:01.838267 syngen-0.0.97/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)    14148 2023-04-28 13:31:35.000000 syngen-0.0.97/README.md
--rw-r--r--   0 runner    (1001) docker     (122)       99 2023-04-28 13:31:35.000000 syngen-0.0.97/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (122)     1307 2023-04-28 13:33:01.838267 syngen-0.0.97/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-28 13:33:01.814267 syngen-0.0.97/src/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-28 13:33:01.818267 syngen-0.0.97/src/syngen/
--rw-r--r--   0 runner    (1001) docker     (122)        7 2023-04-28 13:31:35.000000 syngen-0.0.97/src/syngen/VERSION
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-28 13:31:35.000000 syngen-0.0.97/src/syngen/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2935 2023-04-28 13:31:35.000000 syngen-0.0.97/src/syngen/infer.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-28 13:33:01.822267 syngen-0.0.97/src/syngen/ml/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-28 13:31:35.000000 syngen-0.0.97/src/syngen/ml/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-28 13:33:01.822267 syngen-0.0.97/src/syngen/ml/config/
--rw-r--r--   0 runner    (1001) docker     (122)      112 2023-04-28 13:31:35.000000 syngen-0.0.97/src/syngen/ml/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    10053 2023-04-28 13:31:35.000000 syngen-0.0.97/src/syngen/ml/config/configurations.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-28 13:33:01.822267 syngen-0.0.97/src/syngen/ml/convertor/
--rw-r--r--   0 runner    (1001) docker     (122)      163 2023-04-28 13:31:35.000000 syngen-0.0.97/src/syngen/ml/convertor/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2872 2023-04-28 13:31:35.000000 syngen-0.0.97/src/syngen/ml/convertor/convertor.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-28 13:33:01.822267 syngen-0.0.97/src/syngen/ml/data_loaders/
--rw-r--r--   0 runner    (1001) docker     (122)      172 2023-04-28 13:31:35.000000 syngen-0.0.97/src/syngen/ml/data_loaders/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     7274 2023-04-28 13:31:35.000000 syngen-0.0.97/src/syngen/ml/data_loaders/data_loaders.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-28 13:33:01.826267 syngen-0.0.97/src/syngen/ml/metrics/
--rw-r--r--   0 runner    (1001) docker     (122)      751 2023-04-28 13:31:35.000000 syngen-0.0.97/src/syngen/ml/metrics/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-28 13:33:01.826267 syngen-0.0.97/src/syngen/ml/metrics/accuracy_test/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-28 13:31:35.000000 syngen-0.0.97/src/syngen/ml/metrics/accuracy_test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)   723100 2023-04-28 13:31:35.000000 syngen-0.0.97/src/syngen/ml/metrics/accuracy_test/accuracy_report.html
--rw-r--r--   0 runner    (1001) docker     (122)     5496 2023-04-28 13:31:35.000000 syngen-0.0.97/src/syngen/ml/metrics/accuracy_test/accuracy_test.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-28 13:33:01.814267 syngen-0.0.97/src/syngen/ml/metrics/accuracy_test/src/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-28 13:33:01.826267 syngen-0.0.97/src/syngen/ml/metrics/accuracy_test/src/fonts/
--rw-r--r--   0 runner    (1001) docker     (122)   528976 2023-04-28 13:31:35.000000 syngen-0.0.97/src/syngen/ml/metrics/accuracy_test/src/fonts/OpenSans-VariableFont.ttf
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-28 13:33:01.830267 syngen-0.0.97/src/syngen/ml/metrics/metrics_classes/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-28 13:31:35.000000 syngen-0.0.97/src/syngen/ml/metrics/metrics_classes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    43412 2023-04-28 13:31:35.000000 syngen-0.0.97/src/syngen/ml/metrics/metrics_classes/metrics.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-28 13:33:01.830267 syngen-0.0.97/src/syngen/ml/metrics/sample_test/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-28 13:31:35.000000 syngen-0.0.97/src/syngen/ml/metrics/sample_test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)   708975 2023-04-28 13:31:35.000000 syngen-0.0.97/src/syngen/ml/metrics/sample_test/sample_report_template.html
--rw-r--r--   0 runner    (1001) docker     (122)     1958 2023-04-28 13:31:35.000000 syngen-0.0.97/src/syngen/ml/metrics/sample_test/sample_test.py
--rw-r--r--   0 runner    (1001) docker     (122)     1250 2023-04-28 13:31:35.000000 syngen-0.0.97/src/syngen/ml/metrics/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-28 13:33:01.830267 syngen-0.0.97/src/syngen/ml/reporters/
--rw-r--r--   0 runner    (1001) docker     (122)      224 2023-04-28 13:31:35.000000 syngen-0.0.97/src/syngen/ml/reporters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     6388 2023-04-28 13:31:35.000000 syngen-0.0.97/src/syngen/ml/reporters/reporters.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-28 13:33:01.830267 syngen-0.0.97/src/syngen/ml/strategies/
--rw-r--r--   0 runner    (1001) docker     (122)      169 2023-04-28 13:31:35.000000 syngen-0.0.97/src/syngen/ml/strategies/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     6945 2023-04-28 13:31:35.000000 syngen-0.0.97/src/syngen/ml/strategies/strategies.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-28 13:33:01.830267 syngen-0.0.97/src/syngen/ml/train_chain/
--rw-r--r--   0 runner    (1001) docker     (122)      303 2023-04-28 13:31:35.000000 syngen-0.0.97/src/syngen/ml/train_chain/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    14647 2023-04-28 13:31:35.000000 syngen-0.0.97/src/syngen/ml/train_chain/train_chain.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-28 13:33:01.834267 syngen-0.0.97/src/syngen/ml/utils/
--rw-r--r--   0 runner    (1001) docker     (122)      307 2023-04-28 13:31:35.000000 syngen-0.0.97/src/syngen/ml/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     5649 2023-04-28 13:31:35.000000 syngen-0.0.97/src/syngen/ml/utils/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-28 13:33:01.834267 syngen-0.0.97/src/syngen/ml/vae/
--rw-r--r--   0 runner    (1001) docker     (122)      173 2023-04-28 13:31:35.000000 syngen-0.0.97/src/syngen/ml/vae/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-28 13:33:01.834267 syngen-0.0.97/src/syngen/ml/vae/models/
--rw-r--r--   0 runner    (1001) docker     (122)       49 2023-04-28 13:31:35.000000 syngen-0.0.97/src/syngen/ml/vae/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2085 2023-04-28 13:31:35.000000 syngen-0.0.97/src/syngen/ml/vae/models/custom_layers.py
--rw-r--r--   0 runner    (1001) docker     (122)    30208 2023-04-28 13:31:35.000000 syngen-0.0.97/src/syngen/ml/vae/models/dataset.py
--rw-r--r--   0 runner    (1001) docker     (122)    24693 2023-04-28 13:31:35.000000 syngen-0.0.97/src/syngen/ml/vae/models/features.py
--rw-r--r--   0 runner    (1001) docker     (122)    10439 2023-04-28 13:31:35.000000 syngen-0.0.97/src/syngen/ml/vae/models/model.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-28 13:33:01.834267 syngen-0.0.97/src/syngen/ml/vae/wrappers/
--rw-r--r--   0 runner    (1001) docker     (122)      111 2023-04-28 13:31:35.000000 syngen-0.0.97/src/syngen/ml/vae/wrappers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    11543 2023-04-28 13:31:35.000000 syngen-0.0.97/src/syngen/ml/vae/wrappers/wrappers.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-28 13:33:01.834267 syngen-0.0.97/src/syngen/ml/validation_schema/
--rw-r--r--   0 runner    (1001) docker     (122)      153 2023-04-28 13:31:35.000000 syngen-0.0.97/src/syngen/ml/validation_schema/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     1795 2023-04-28 13:31:35.000000 syngen-0.0.97/src/syngen/ml/validation_schema/validation_schema.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-28 13:33:01.838267 syngen-0.0.97/src/syngen/ml/worker/
--rw-r--r--   0 runner    (1001) docker     (122)       43 2023-04-28 13:31:35.000000 syngen-0.0.97/src/syngen/ml/worker/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)    13012 2023-04-28 13:31:35.000000 syngen-0.0.97/src/syngen/ml/worker/worker.py
--rw-r--r--   0 runner    (1001) docker     (122)     3976 2023-04-28 13:31:35.000000 syngen-0.0.97/src/syngen/train.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-28 13:33:01.822267 syngen-0.0.97/src/syngen.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)    14888 2023-04-28 13:33:01.000000 syngen-0.0.97/src/syngen.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     1902 2023-04-28 13:33:01.000000 syngen-0.0.97/src/syngen.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-04-28 13:33:01.000000 syngen-0.0.97/src/syngen.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)       86 2023-04-28 13:33:01.000000 syngen-0.0.97/src/syngen.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (122)      299 2023-04-28 13:33:01.000000 syngen-0.0.97/src/syngen.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)        7 2023-04-28 13:33:01.000000 syngen-0.0.97/src/syngen.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-05 17:23:39.702504 syngen-0.0.98/
+-rw-r--r--   0 runner    (1001) docker     (122)      400 2023-05-05 17:22:19.000000 syngen-0.0.98/DESCRIPTION
+-rw-r--r--   0 runner    (1001) docker     (122)    35149 2023-05-05 17:22:19.000000 syngen-0.0.98/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)      133 2023-05-05 17:22:19.000000 syngen-0.0.98/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)    14888 2023-05-05 17:23:39.702504 syngen-0.0.98/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)    14148 2023-05-05 17:22:19.000000 syngen-0.0.98/README.md
+-rw-r--r--   0 runner    (1001) docker     (122)       99 2023-05-05 17:22:19.000000 syngen-0.0.98/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (122)     1307 2023-05-05 17:23:39.702504 syngen-0.0.98/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-05 17:23:39.686504 syngen-0.0.98/src/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-05 17:23:39.694504 syngen-0.0.98/src/syngen/
+-rw-r--r--   0 runner    (1001) docker     (122)        7 2023-05-05 17:22:19.000000 syngen-0.0.98/src/syngen/VERSION
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-05 17:22:19.000000 syngen-0.0.98/src/syngen/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2677 2023-05-05 17:22:19.000000 syngen-0.0.98/src/syngen/infer.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-05 17:23:39.698504 syngen-0.0.98/src/syngen/ml/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-05 17:22:19.000000 syngen-0.0.98/src/syngen/ml/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-05 17:23:39.698504 syngen-0.0.98/src/syngen/ml/config/
+-rw-r--r--   0 runner    (1001) docker     (122)      112 2023-05-05 17:22:19.000000 syngen-0.0.98/src/syngen/ml/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10174 2023-05-05 17:22:19.000000 syngen-0.0.98/src/syngen/ml/config/configurations.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-05 17:23:39.698504 syngen-0.0.98/src/syngen/ml/convertor/
+-rw-r--r--   0 runner    (1001) docker     (122)      163 2023-05-05 17:22:19.000000 syngen-0.0.98/src/syngen/ml/convertor/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2872 2023-05-05 17:22:19.000000 syngen-0.0.98/src/syngen/ml/convertor/convertor.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-05 17:23:39.698504 syngen-0.0.98/src/syngen/ml/data_loaders/
+-rw-r--r--   0 runner    (1001) docker     (122)      172 2023-05-05 17:22:19.000000 syngen-0.0.98/src/syngen/ml/data_loaders/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7287 2023-05-05 17:22:19.000000 syngen-0.0.98/src/syngen/ml/data_loaders/data_loaders.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-05 17:23:39.698504 syngen-0.0.98/src/syngen/ml/metrics/
+-rw-r--r--   0 runner    (1001) docker     (122)      751 2023-05-05 17:22:19.000000 syngen-0.0.98/src/syngen/ml/metrics/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-05 17:23:39.698504 syngen-0.0.98/src/syngen/ml/metrics/accuracy_test/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-05 17:22:19.000000 syngen-0.0.98/src/syngen/ml/metrics/accuracy_test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)   723100 2023-05-05 17:22:19.000000 syngen-0.0.98/src/syngen/ml/metrics/accuracy_test/accuracy_report.html
+-rw-r--r--   0 runner    (1001) docker     (122)     5496 2023-05-05 17:22:19.000000 syngen-0.0.98/src/syngen/ml/metrics/accuracy_test/accuracy_test.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-05 17:23:39.690504 syngen-0.0.98/src/syngen/ml/metrics/accuracy_test/src/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-05 17:23:39.698504 syngen-0.0.98/src/syngen/ml/metrics/accuracy_test/src/fonts/
+-rw-r--r--   0 runner    (1001) docker     (122)   528976 2023-05-05 17:22:19.000000 syngen-0.0.98/src/syngen/ml/metrics/accuracy_test/src/fonts/OpenSans-VariableFont.ttf
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-05 17:23:39.698504 syngen-0.0.98/src/syngen/ml/metrics/metrics_classes/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-05 17:22:19.000000 syngen-0.0.98/src/syngen/ml/metrics/metrics_classes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    43412 2023-05-05 17:22:19.000000 syngen-0.0.98/src/syngen/ml/metrics/metrics_classes/metrics.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-05 17:23:39.702504 syngen-0.0.98/src/syngen/ml/metrics/sample_test/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-05 17:22:19.000000 syngen-0.0.98/src/syngen/ml/metrics/sample_test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)   708975 2023-05-05 17:22:19.000000 syngen-0.0.98/src/syngen/ml/metrics/sample_test/sample_report_template.html
+-rw-r--r--   0 runner    (1001) docker     (122)     1958 2023-05-05 17:22:19.000000 syngen-0.0.98/src/syngen/ml/metrics/sample_test/sample_test.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1250 2023-05-05 17:22:19.000000 syngen-0.0.98/src/syngen/ml/metrics/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-05 17:23:39.702504 syngen-0.0.98/src/syngen/ml/reporters/
+-rw-r--r--   0 runner    (1001) docker     (122)      224 2023-05-05 17:22:19.000000 syngen-0.0.98/src/syngen/ml/reporters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6388 2023-05-05 17:22:19.000000 syngen-0.0.98/src/syngen/ml/reporters/reporters.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-05 17:23:39.702504 syngen-0.0.98/src/syngen/ml/strategies/
+-rw-r--r--   0 runner    (1001) docker     (122)      169 2023-05-05 17:22:19.000000 syngen-0.0.98/src/syngen/ml/strategies/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6945 2023-05-05 17:22:19.000000 syngen-0.0.98/src/syngen/ml/strategies/strategies.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-05 17:23:39.702504 syngen-0.0.98/src/syngen/ml/train_chain/
+-rw-r--r--   0 runner    (1001) docker     (122)      303 2023-05-05 17:22:19.000000 syngen-0.0.98/src/syngen/ml/train_chain/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    14647 2023-05-05 17:22:19.000000 syngen-0.0.98/src/syngen/ml/train_chain/train_chain.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-05 17:23:39.702504 syngen-0.0.98/src/syngen/ml/utils/
+-rw-r--r--   0 runner    (1001) docker     (122)      307 2023-05-05 17:22:19.000000 syngen-0.0.98/src/syngen/ml/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5649 2023-05-05 17:22:19.000000 syngen-0.0.98/src/syngen/ml/utils/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-05 17:23:39.702504 syngen-0.0.98/src/syngen/ml/vae/
+-rw-r--r--   0 runner    (1001) docker     (122)      173 2023-05-05 17:22:19.000000 syngen-0.0.98/src/syngen/ml/vae/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-05 17:23:39.702504 syngen-0.0.98/src/syngen/ml/vae/models/
+-rw-r--r--   0 runner    (1001) docker     (122)       49 2023-05-05 17:22:19.000000 syngen-0.0.98/src/syngen/ml/vae/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2085 2023-05-05 17:22:19.000000 syngen-0.0.98/src/syngen/ml/vae/models/custom_layers.py
+-rw-r--r--   0 runner    (1001) docker     (122)    30207 2023-05-05 17:22:19.000000 syngen-0.0.98/src/syngen/ml/vae/models/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (122)    24693 2023-05-05 17:22:19.000000 syngen-0.0.98/src/syngen/ml/vae/models/features.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10439 2023-05-05 17:22:19.000000 syngen-0.0.98/src/syngen/ml/vae/models/model.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-05 17:23:39.702504 syngen-0.0.98/src/syngen/ml/vae/wrappers/
+-rw-r--r--   0 runner    (1001) docker     (122)      111 2023-05-05 17:22:19.000000 syngen-0.0.98/src/syngen/ml/vae/wrappers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11543 2023-05-05 17:22:19.000000 syngen-0.0.98/src/syngen/ml/vae/wrappers/wrappers.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-05 17:23:39.702504 syngen-0.0.98/src/syngen/ml/validation_schema/
+-rw-r--r--   0 runner    (1001) docker     (122)      153 2023-05-05 17:22:19.000000 syngen-0.0.98/src/syngen/ml/validation_schema/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1795 2023-05-05 17:22:19.000000 syngen-0.0.98/src/syngen/ml/validation_schema/validation_schema.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-05 17:23:39.702504 syngen-0.0.98/src/syngen/ml/worker/
+-rw-r--r--   0 runner    (1001) docker     (122)       43 2023-05-05 17:22:19.000000 syngen-0.0.98/src/syngen/ml/worker/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    13012 2023-05-05 17:22:19.000000 syngen-0.0.98/src/syngen/ml/worker/worker.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3987 2023-05-05 17:22:19.000000 syngen-0.0.98/src/syngen/train.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-05 17:23:39.698504 syngen-0.0.98/src/syngen.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)    14888 2023-05-05 17:23:39.000000 syngen-0.0.98/src/syngen.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     1902 2023-05-05 17:23:39.000000 syngen-0.0.98/src/syngen.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-05 17:23:39.000000 syngen-0.0.98/src/syngen.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       86 2023-05-05 17:23:39.000000 syngen-0.0.98/src/syngen.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      299 2023-05-05 17:23:39.000000 syngen-0.0.98/src/syngen.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        7 2023-05-05 17:23:39.000000 syngen-0.0.98/src/syngen.egg-info/top_level.txt
```

### Comparing `syngen-0.0.97/LICENSE` & `syngen-0.0.98/LICENSE`

 * *Files identical despite different names*

### Comparing `syngen-0.0.97/PKG-INFO` & `syngen-0.0.98/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: syngen
-Version: 0.0.97
+Version: 0.0.98
 Summary: The tool uncovers patterns, trends, and correlations hidden within your production datasets.
 Home-page: https://github.com/tdspora/syngen
 Author: EPAM Systems, Inc.
 Maintainer: Pavel Bobyrev
 License: GPLv3 License
 Keywords: data,generation,synthetic,vae,tabular
 Classifier: Development Status :: 5 - Production/Stable
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: syngen Version: 0.0.97 Summary: The tool uncovers
+Metadata-Version: 2.1 Name: syngen Version: 0.0.98 Summary: The tool uncovers
 patterns, trends, and correlations hidden within your production datasets.
 Home-page: https://github.com/tdspora/syngen Author: EPAM Systems, Inc.
 Maintainer: Pavel Bobyrev License: GPLv3 License Keywords:
 data,generation,synthetic,vae,tabular Classifier: Development Status :: 5 -
 Production/Stable Classifier: Operating System :: POSIX :: Linux Classifier:
 Operating System :: Microsoft :: Windows Classifier: License :: OSI Approved ::
 GNU General Public License v3 (GPLv3) Classifier: Programming Language ::
```

### Comparing `syngen-0.0.97/README.md` & `syngen-0.0.98/README.md`

 * *Files identical despite different names*

### Comparing `syngen-0.0.97/setup.cfg` & `syngen-0.0.98/setup.cfg`

 * *Files identical despite different names*

### Comparing `syngen-0.0.97/src/syngen/infer.py` & `syngen-0.0.98/src/syngen/infer.py`

 * *Files 10% similar despite different names*

```diff
@@ -42,24 +42,20 @@
     batch_size
     print_report
     random_seed
     -------
 
     """
     if not metadata_path and not table_name:
-        raise AttributeError("It seems that the information of metadata_path or table_name is absent. "
-                             "Please provide either the information of metadata_path or the information of table_name.")
-    if metadata_path:
-        if table_name:
-            logger.warning("The information of metadata_path was provided. "
-                           "In this case the information of table_name will be ignored.")
-            table_name = None
-        if not metadata_path.endswith(('.yaml', '.yml')):
-            raise NotImplementedError("This format for metadata_path is not supported. "
-                                      "Please provide metadata_path in '.yaml' or in '.yml' format")
+        raise AttributeError("It seems that the information of 'metadata_path' or 'table_name' is absent. "
+                             "Please provide either the information of 'metadata_path' or the information of 'table_name'")
+    if metadata_path and table_name:
+        logger.warning("The information of 'metadata_path' was provided. "
+                       "In this case the information of 'table_name' will be ignored")
+        table_name = None
     settings = {
         "size": size,
         "run_parallel": run_parallel,
         "batch_size": batch_size,
         "print_report": print_report,
         "random_seed": random_seed
     }
```

### Comparing `syngen-0.0.97/src/syngen/ml/config/configurations.py` & `syngen-0.0.98/src/syngen/ml/config/configurations.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,28 +14,29 @@
     """
     The configuration class to set up the work of train process
     """
     source: Optional[str]
     epochs: int
     drop_null: bool
     row_limit: Optional[int]
+    random_state: Optional[int]
     table_name: Optional[str]
     metadata_path: Optional[str]
     print_report: bool
     batch_size: int
     paths: Dict = field(init=False)
     row_subset: int = field(init=False)
     schema: Dict = field(init=False)
     slugify_table_name: str = field(init=False)
 
     def __post_init__(self):
         self.paths = self._set_paths()
         self._prepare_dirs()
         data, self.schema = self._extract_data()
-        self._prepare_data(data)
+        self._prepare_data(data, self.random_state)
         self._set_batch_size()
 
     def to_dict(self) -> Dict:
         """
         Return the values of the settings of training process
         """
         return {
@@ -101,29 +102,30 @@
         Extract data and schema necessary for training process
         """
         data, schema = self._load_source()
         data, dropped_columns = self._remove_empty_columns(data)
         schema = self._mark_removed_columns(data, schema, dropped_columns)
         return data, schema
 
-    def _preprocess_data(self, data: pd.DataFrame) -> pd.DataFrame:
+    def _preprocess_data(self, data: pd.DataFrame, random_state) -> pd.DataFrame:
         """
         Preprocess data and set the parameter "row_subset" for training process
         """
         if self.drop_null:
             if not data.dropna().empty:
                 data = data.dropna()
             else:
                 logger.warning("The specified 'drop_null' argument results in the empty dataframe, "
                                "so it will be ignored")
 
         if self.row_limit:
             self.row_subset = min(self.row_limit, len(data))
 
-            data = data.sample(n=self.row_subset)
+            data = data.sample(n=self.row_subset, random_state=random_state)
+
             if len(data) < 100:
                 logger.warning("The input table is too small to provide any meaningful results. "
                                "Please consider 1) disable drop_null argument, 2) provide bigger table")
             elif len(data) < 500:
                 logger.warning(
                     f"The amount of data is {len(data)} rows. It seems that it isn't enough to supply "
                     f"high-quality results. To improve the quality of generated data please consider any of the steps: "
@@ -133,19 +135,19 @@
 
         self.row_subset = len(data)
         return data
 
     def _save_input_data(self, data: pd.DataFrame):
         DataLoader(self.paths["input_data_path"]).save_data(self.paths["input_data_path"], data)
 
-    def _prepare_data(self, data: pd.DataFrame):
+    def _prepare_data(self, data: pd.DataFrame, random_state):
         """
         Preprocess and save data necessary for training process
         """
-        data = self._preprocess_data(data)
+        data = self._preprocess_data(data, random_state)
         self._save_input_data(data)
 
     @slugify_attribute(table_name="slugify_table_name")
     def _set_paths(self) -> Dict:
         """
         Create the paths which used in training process
         """
```

### Comparing `syngen-0.0.97/src/syngen/ml/convertor/convertor.py` & `syngen-0.0.98/src/syngen/ml/convertor/convertor.py`

 * *Files identical despite different names*

### Comparing `syngen-0.0.97/src/syngen/ml/data_loaders/data_loaders.py` & `syngen-0.0.98/src/syngen/ml/data_loaders/data_loaders.py`

 * *Files 1% similar despite different names*

```diff
@@ -171,15 +171,15 @@
 
     def get_metadata_loader(self):
         if self.metadata_path is not None:
             path = Path(self.metadata_path)
             if path.suffix in ['.yaml', '.yml']:
                 return YAMLLoader()
             else:
-                raise NotImplementedError("File format not supported")
+                raise NotImplementedError("The format of metadata isn't supported")
 
     def load_data(self) -> dict:
         return self.metadata_loader.load_data(self.metadata_path)
 
     def save_data(self, path: str, df: pd.DataFrame, **kwargs):
         self.metadata_loader.save_data(path, df, **kwargs)
```

### Comparing `syngen-0.0.97/src/syngen/ml/metrics/__init__.py` & `syngen-0.0.98/src/syngen/ml/metrics/__init__.py`

 * *Files identical despite different names*

### Comparing `syngen-0.0.97/src/syngen/ml/metrics/accuracy_test/accuracy_report.html` & `syngen-0.0.98/src/syngen/ml/metrics/accuracy_test/accuracy_report.html`

 * *Files identical despite different names*

### Comparing `syngen-0.0.97/src/syngen/ml/metrics/accuracy_test/accuracy_test.py` & `syngen-0.0.98/src/syngen/ml/metrics/accuracy_test/accuracy_test.py`

 * *Files identical despite different names*

### Comparing `syngen-0.0.97/src/syngen/ml/metrics/accuracy_test/src/fonts/OpenSans-VariableFont.ttf` & `syngen-0.0.98/src/syngen/ml/metrics/accuracy_test/src/fonts/OpenSans-VariableFont.ttf`

 * *Files identical despite different names*

### Comparing `syngen-0.0.97/src/syngen/ml/metrics/metrics_classes/metrics.py` & `syngen-0.0.98/src/syngen/ml/metrics/metrics_classes/metrics.py`

 * *Files identical despite different names*

### Comparing `syngen-0.0.97/src/syngen/ml/metrics/sample_test/sample_report_template.html` & `syngen-0.0.98/src/syngen/ml/metrics/sample_test/sample_report_template.html`

 * *Files identical despite different names*

### Comparing `syngen-0.0.97/src/syngen/ml/metrics/sample_test/sample_test.py` & `syngen-0.0.98/src/syngen/ml/metrics/sample_test/sample_test.py`

 * *Files identical despite different names*

### Comparing `syngen-0.0.97/src/syngen/ml/metrics/utils.py` & `syngen-0.0.98/src/syngen/ml/metrics/utils.py`

 * *Files identical despite different names*

### Comparing `syngen-0.0.97/src/syngen/ml/reporters/reporters.py` & `syngen-0.0.98/src/syngen/ml/reporters/reporters.py`

 * *Files identical despite different names*

### Comparing `syngen-0.0.97/src/syngen/ml/strategies/strategies.py` & `syngen-0.0.98/src/syngen/ml/strategies/strategies.py`

 * *Files identical despite different names*

### Comparing `syngen-0.0.97/src/syngen/ml/train_chain/train_chain.py` & `syngen-0.0.98/src/syngen/ml/train_chain/train_chain.py`

 * *Files identical despite different names*

### Comparing `syngen-0.0.97/src/syngen/ml/utils/utils.py` & `syngen-0.0.98/src/syngen/ml/utils/utils.py`

 * *Files identical despite different names*

### Comparing `syngen-0.0.97/src/syngen/ml/vae/models/custom_layers.py` & `syngen-0.0.98/src/syngen/ml/vae/models/custom_layers.py`

 * *Files identical despite different names*

### Comparing `syngen-0.0.97/src/syngen/ml/vae/models/dataset.py` & `syngen-0.0.98/src/syngen/ml/vae/models/dataset.py`

 * *Files 0% similar despite different names*

```diff
@@ -293,15 +293,15 @@
             self.long_text_columns = set(data_subset.columns)
             if self.long_text_columns:
                 logger.info(
                     f"Please note that the columns - {self.long_text_columns} contain long texts (> 200 symbols). "
                     f"Such texts' handling consumes significant resources and results in poor quality content, "
                     f"therefore this column(-s) will be generated using a simplified statistical approach")
 
-    def _general_data_pipeline(self, df: pd.DataFrame, schema: Dict, check_object_on_float: bool = False):
+    def _general_data_pipeline(self, df: pd.DataFrame, schema: Dict, check_object_on_float: bool = True):
         """
         Divide columns in dataframe into groups - binary, categorical, integer, float, string, date
         in case metadata of the table is absent
         """
         if check_object_on_float:
             columns_nan_labels = get_nan_labels(df)
             df = nan_labels_to_float(df, columns_nan_labels)
```

### Comparing `syngen-0.0.97/src/syngen/ml/vae/models/features.py` & `syngen-0.0.98/src/syngen/ml/vae/models/features.py`

 * *Files identical despite different names*

### Comparing `syngen-0.0.97/src/syngen/ml/vae/models/model.py` & `syngen-0.0.98/src/syngen/ml/vae/models/model.py`

 * *Files identical despite different names*

### Comparing `syngen-0.0.97/src/syngen/ml/vae/wrappers/wrappers.py` & `syngen-0.0.98/src/syngen/ml/vae/wrappers/wrappers.py`

 * *Files identical despite different names*

### Comparing `syngen-0.0.97/src/syngen/ml/validation_schema/validation_schema.py` & `syngen-0.0.98/src/syngen/ml/validation_schema/validation_schema.py`

 * *Files identical despite different names*

### Comparing `syngen-0.0.97/src/syngen/ml/worker/worker.py` & `syngen-0.0.98/src/syngen/ml/worker/worker.py`

 * *Files identical despite different names*

### Comparing `syngen-0.0.97/src/syngen/train.py` & `syngen-0.0.98/src/syngen/train.py`

 * *Files 19% similar despite different names*

```diff
@@ -47,38 +47,37 @@
     drop_null
     row_limit
     print_report
     batch_size
     -------
 
     """
-    if not metadata_path and not source:
-        raise AttributeError("It seems that the information of metadata_path or source is absent. "
-                             "Please provide either the information of metadata_path or "
-                             "the information of source and table_name.")
-    if metadata_path:
-        if source:
-            logger.warning("The information of metadata_path was provided. "
-                           "In this case the information of source will be ignored.")
-        if table_name:
-            logger.warning("The information of metadata_path was provided. "
-                           "In this case the information of table_name will be ignored.")
-            table_name = None
-        if not metadata_path.endswith(('.yaml', '.yml')):
-            raise NotImplementedError("This format for metadata_path is not supported. "
-                                      "Please provide metadata_path in '.yaml' or '.yml' format")
-    if not metadata_path:
-        if source and not table_name:
-            raise AttributeError("It seems that the information of table_name is absent. "
-                                 "In the case the information of metadata_path is absent, "
-                                 "the information of source and table_name should be provided.")
-        if table_name and not source:
-            raise AttributeError("It seems that the information of source is absent. "
-                                 "In the case the information of metadata_path is absent, "
-                                 "the information of source and table_name should be provided.")
+    if not metadata_path and not source and not table_name:
+        raise AttributeError("It seems that the information of 'metadata_path' or 'table_name' and 'source' is absent. "
+                             "Please provide either the information of 'metadata_path' or "
+                             "the information of 'source' and 'table_name'")
+    elif metadata_path and table_name and source:
+        logger.warning("The information of 'metadata_path' was provided. "
+                       "In this case the information of 'table_name' and 'source' will be ignored")
+        table_name = None
+    elif metadata_path and source:
+        logger.warning("The information of 'metadata_path' was provided. "
+                       "In this case the information of 'source' will be ignored")
+    elif metadata_path and table_name:
+        logger.warning("The information of 'metadata_path' was provided. "
+                       "In this case the information of 'table_name' will be ignored")
+        table_name = None
+    elif source and not table_name:
+        raise AttributeError("It seems that the information of 'metadata_path' or 'table_name' is absent. "
+                             "Please provide either the information of 'metadata_path' or "
+                             "the information of 'source' and 'table_name'")
+    elif table_name and not source:
+        raise AttributeError("It seems that the information of 'metadata_path' or 'source' is absent. "
+                             "Please provide either the information of 'metadata_path' or "
+                             "the information of 'source' and 'table_name'")
     settings = {
         "source": source,
         "epochs": epochs,
         "drop_null": drop_null,
         "row_limit": row_limit,
         "batch_size": batch_size,
         "print_report": print_report
```

### Comparing `syngen-0.0.97/src/syngen.egg-info/PKG-INFO` & `syngen-0.0.98/src/syngen.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: syngen
-Version: 0.0.97
+Version: 0.0.98
 Summary: The tool uncovers patterns, trends, and correlations hidden within your production datasets.
 Home-page: https://github.com/tdspora/syngen
 Author: EPAM Systems, Inc.
 Maintainer: Pavel Bobyrev
 License: GPLv3 License
 Keywords: data,generation,synthetic,vae,tabular
 Classifier: Development Status :: 5 - Production/Stable
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: syngen Version: 0.0.97 Summary: The tool uncovers
+Metadata-Version: 2.1 Name: syngen Version: 0.0.98 Summary: The tool uncovers
 patterns, trends, and correlations hidden within your production datasets.
 Home-page: https://github.com/tdspora/syngen Author: EPAM Systems, Inc.
 Maintainer: Pavel Bobyrev License: GPLv3 License Keywords:
 data,generation,synthetic,vae,tabular Classifier: Development Status :: 5 -
 Production/Stable Classifier: Operating System :: POSIX :: Linux Classifier:
 Operating System :: Microsoft :: Windows Classifier: License :: OSI Approved ::
 GNU General Public License v3 (GPLv3) Classifier: Programming Language ::
```

### Comparing `syngen-0.0.97/src/syngen.egg-info/SOURCES.txt` & `syngen-0.0.98/src/syngen.egg-info/SOURCES.txt`

 * *Files identical despite different names*

