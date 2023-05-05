# Comparing `tmp/ai_transform-0.31.0.tar.gz` & `tmp/ai_transform-0.31.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ai_transform-0.31.0.tar", last modified: Wed May  3 04:24:59 2023, max compression
+gzip compressed data, was "ai_transform-0.31.1.tar", last modified: Fri May  5 02:23:05 2023, max compression
```

## Comparing `ai_transform-0.31.0.tar` & `ai_transform-0.31.1.tar`

### file list

```diff
@@ -1,93 +1,93 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 04:24:59.480532 ai_transform-0.31.0/
--rw-r--r--   0 runner    (1001) docker     (123)    11346 2023-05-03 04:24:42.000000 ai_transform-0.31.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      271 2023-05-03 04:24:59.480532 ai_transform-0.31.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3348 2023-05-03 04:24:42.000000 ai_transform-0.31.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 04:24:59.472532 ai_transform-0.31.0/ai_transform/
--rw-r--r--   0 runner    (1001) docker     (123)      749 2023-05-03 04:24:42.000000 ai_transform-0.31.0/ai_transform/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 04:24:59.472532 ai_transform-0.31.0/ai_transform/api/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 04:24:42.000000 ai_transform-0.31.0/ai_transform/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    29326 2023-05-03 04:24:42.000000 ai_transform-0.31.0/ai_transform/api/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     4102 2023-05-03 04:24:42.000000 ai_transform-0.31.0/ai_transform/api/client.py
--rw-r--r--   0 runner    (1001) docker     (123)      333 2023-05-03 04:24:42.000000 ai_transform-0.31.0/ai_transform/api/endpoints.py
--rw-r--r--   0 runner    (1001) docker     (123)      790 2023-05-03 04:24:42.000000 ai_transform-0.31.0/ai_transform/api/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     2641 2023-05-03 04:24:42.000000 ai_transform-0.31.0/ai_transform/api/wrappers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 04:24:59.476532 ai_transform-0.31.0/ai_transform/components/
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-05-03 04:24:42.000000 ai_transform-0.31.0/ai_transform/components/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11976 2023-05-03 04:24:42.000000 ai_transform-0.31.0/ai_transform/components/components.py
--rw-r--r--   0 runner    (1001) docker     (123)     3788 2023-05-03 04:24:42.000000 ai_transform-0.31.0/ai_transform/config.py
--rw-r--r--   0 runner    (1001) docker     (123)      152 2023-05-03 04:24:42.000000 ai_transform-0.31.0/ai_transform/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 04:24:59.476532 ai_transform-0.31.0/ai_transform/dataset/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 04:24:42.000000 ai_transform-0.31.0/ai_transform/dataset/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11343 2023-05-03 04:24:42.000000 ai_transform-0.31.0/ai_transform/dataset/dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)    15147 2023-05-03 04:24:42.000000 ai_transform-0.31.0/ai_transform/dataset/field.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 04:24:59.476532 ai_transform-0.31.0/ai_transform/engine/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 04:24:42.000000 ai_transform-0.31.0/ai_transform/engine/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15346 2023-05-03 04:24:42.000000 ai_transform-0.31.0/ai_transform/engine/abstract_engine.py
--rw-r--r--   0 runner    (1001) docker     (123)     3252 2023-05-03 04:24:42.000000 ai_transform-0.31.0/ai_transform/engine/dense_output_engine.py
--rw-r--r--   0 runner    (1001) docker     (123)     1363 2023-05-03 04:24:42.000000 ai_transform-0.31.0/ai_transform/engine/in_memory_engine.py
--rw-r--r--   0 runner    (1001) docker     (123)     4505 2023-05-03 04:24:42.000000 ai_transform-0.31.0/ai_transform/engine/multipass_engine.py
--rw-r--r--   0 runner    (1001) docker     (123)     3313 2023-05-03 04:24:42.000000 ai_transform-0.31.0/ai_transform/engine/small_batch_stable_engine.py
--rw-r--r--   0 runner    (1001) docker     (123)     3639 2023-05-03 04:24:42.000000 ai_transform-0.31.0/ai_transform/engine/stable_engine.py
--rw-r--r--   0 runner    (1001) docker     (123)      826 2023-05-03 04:24:42.000000 ai_transform-0.31.0/ai_transform/errors.py
--rw-r--r--   0 runner    (1001) docker     (123)     1540 2023-05-03 04:24:42.000000 ai_transform-0.31.0/ai_transform/logger.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 04:24:59.476532 ai_transform-0.31.0/ai_transform/operator/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 04:24:42.000000 ai_transform-0.31.0/ai_transform/operator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7119 2023-05-03 04:24:42.000000 ai_transform-0.31.0/ai_transform/operator/abstract_operator.py
--rw-r--r--   0 runner    (1001) docker     (123)     1411 2023-05-03 04:24:42.000000 ai_transform-0.31.0/ai_transform/operator/dense_operator.py
--rw-r--r--   0 runner    (1001) docker     (123)      556 2023-05-03 04:24:42.000000 ai_transform-0.31.0/ai_transform/timer.py
--rw-r--r--   0 runner    (1001) docker     (123)      575 2023-05-03 04:24:42.000000 ai_transform-0.31.0/ai_transform/types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 04:24:59.476532 ai_transform-0.31.0/ai_transform/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      237 2023-05-03 04:24:42.000000 ai_transform-0.31.0/ai_transform/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8574 2023-05-03 04:24:42.000000 ai_transform-0.31.0/ai_transform/utils/document.py
--rw-r--r--   0 runner    (1001) docker     (123)     5971 2023-05-03 04:24:42.000000 ai_transform-0.31.0/ai_transform/utils/document_list.py
--rw-r--r--   0 runner    (1001) docker     (123)      139 2023-05-03 04:24:42.000000 ai_transform-0.31.0/ai_transform/utils/encode_parameters.py
--rw-r--r--   0 runner    (1001) docker     (123)     3383 2023-05-03 04:24:42.000000 ai_transform-0.31.0/ai_transform/utils/example_documents.py
--rw-r--r--   0 runner    (1001) docker     (123)     3240 2023-05-03 04:24:42.000000 ai_transform-0.31.0/ai_transform/utils/json_encoder.py
--rw-r--r--   0 runner    (1001) docker     (123)      940 2023-05-03 04:24:42.000000 ai_transform-0.31.0/ai_transform/utils/keyphrase.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 04:24:59.476532 ai_transform-0.31.0/ai_transform/workflow/
--rw-r--r--   0 runner    (1001) docker     (123)       79 2023-05-03 04:24:42.000000 ai_transform-0.31.0/ai_transform/workflow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3660 2023-05-03 04:24:42.000000 ai_transform-0.31.0/ai_transform/workflow/abstract_workflow.py
--rw-r--r--   0 runner    (1001) docker     (123)     7161 2023-05-03 04:24:42.000000 ai_transform-0.31.0/ai_transform/workflow/context_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     3017 2023-05-03 04:24:42.000000 ai_transform-0.31.0/ai_transform/workflow/helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 04:24:59.472532 ai_transform-0.31.0/ai_transform.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      271 2023-05-03 04:24:59.000000 ai_transform-0.31.0/ai_transform.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2488 2023-05-03 04:24:59.000000 ai_transform-0.31.0/ai_transform.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-03 04:24:59.000000 ai_transform-0.31.0/ai_transform.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      335 2023-05-03 04:24:59.000000 ai_transform-0.31.0/ai_transform.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-03 04:24:59.000000 ai_transform-0.31.0/ai_transform.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      128 2023-05-03 04:24:42.000000 ai_transform-0.31.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-03 04:24:59.480532 ai_transform-0.31.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      994 2023-05-03 04:24:42.000000 ai_transform-0.31.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 04:24:59.476532 ai_transform-0.31.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 04:24:42.000000 ai_transform-0.31.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      302 2023-05-03 04:24:42.000000 ai_transform-0.31.0/tests/components.py
--rw-r--r--   0 runner    (1001) docker     (123)    11140 2023-05-03 04:24:42.000000 ai_transform-0.31.0/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 04:24:59.476532 ai_transform-0.31.0/tests/core/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 04:24:42.000000 ai_transform-0.31.0/tests/core/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 04:24:59.476532 ai_transform-0.31.0/tests/core/test_api/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 04:24:42.000000 ai_transform-0.31.0/tests/core/test_api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1416 2023-05-03 04:24:42.000000 ai_transform-0.31.0/tests/core/test_api/test_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     1130 2023-05-03 04:24:42.000000 ai_transform-0.31.0/tests/core/test_api/test_endpoints.py
--rw-r--r--   0 runner    (1001) docker     (123)     1003 2023-05-03 04:24:42.000000 ai_transform-0.31.0/tests/core/test_api/test_keyphrase.py
--rw-r--r--   0 runner    (1001) docker     (123)     5382 2023-05-03 04:24:42.000000 ai_transform-0.31.0/tests/core/test_api/test_wrappers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 04:24:59.480532 ai_transform-0.31.0/tests/core/test_dataset/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 04:24:42.000000 ai_transform-0.31.0/tests/core/test_dataset/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5987 2023-05-03 04:24:42.000000 ai_transform-0.31.0/tests/core/test_dataset/test_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     2128 2023-05-03 04:24:42.000000 ai_transform-0.31.0/tests/core/test_dataset/test_field.py
--rw-r--r--   0 runner    (1001) docker     (123)      951 2023-05-03 04:24:42.000000 ai_transform-0.31.0/tests/core/test_dataset/test_keyphrase.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 04:24:59.480532 ai_transform-0.31.0/tests/core/test_engine/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 04:24:42.000000 ai_transform-0.31.0/tests/core/test_engine/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1910 2023-05-03 04:24:42.000000 ai_transform-0.31.0/tests/core/test_engine/test_dense_output_engine.py
--rw-r--r--   0 runner    (1001) docker     (123)     1977 2023-05-03 04:24:42.000000 ai_transform-0.31.0/tests/core/test_engine/test_engine.py
--rw-r--r--   0 runner    (1001) docker     (123)      699 2023-05-03 04:24:42.000000 ai_transform-0.31.0/tests/core/test_engine/test_engine_playground.py
--rw-r--r--   0 runner    (1001) docker     (123)     3327 2023-05-03 04:24:42.000000 ai_transform-0.31.0/tests/core/test_engine/test_multipass_engine.py
--rw-r--r--   0 runner    (1001) docker     (123)     1016 2023-05-03 04:24:42.000000 ai_transform-0.31.0/tests/core/test_engine/test_stable_engine.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 04:24:59.480532 ai_transform-0.31.0/tests/core/test_operator/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 04:24:42.000000 ai_transform-0.31.0/tests/core/test_operator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      624 2023-05-03 04:24:42.000000 ai_transform-0.31.0/tests/core/test_operator/test_abstract_operator.py
--rw-r--r--   0 runner    (1001) docker     (123)     2153 2023-05-03 04:24:42.000000 ai_transform-0.31.0/tests/core/test_operator/test_document_diff.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 04:24:59.480532 ai_transform-0.31.0/tests/core/test_workflow/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 04:24:42.000000 ai_transform-0.31.0/tests/core/test_workflow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1170 2023-05-03 04:24:42.000000 ai_transform-0.31.0/tests/core/test_workflow/test_context_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     3349 2023-05-03 04:24:42.000000 ai_transform-0.31.0/tests/core/test_workflow/test_workflow.py
--rw-r--r--   0 runner    (1001) docker     (123)      416 2023-05-03 04:24:42.000000 ai_transform-0.31.0/tests/test_connection_retry.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 02:23:05.548369 ai_transform-0.31.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    11346 2023-05-05 02:22:48.000000 ai_transform-0.31.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      271 2023-05-05 02:23:05.548369 ai_transform-0.31.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3348 2023-05-05 02:22:48.000000 ai_transform-0.31.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 02:23:05.544369 ai_transform-0.31.1/ai_transform/
+-rw-r--r--   0 runner    (1001) docker     (123)      749 2023-05-05 02:22:48.000000 ai_transform-0.31.1/ai_transform/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 02:23:05.544369 ai_transform-0.31.1/ai_transform/api/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 02:22:48.000000 ai_transform-0.31.1/ai_transform/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29452 2023-05-05 02:22:48.000000 ai_transform-0.31.1/ai_transform/api/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4186 2023-05-05 02:22:48.000000 ai_transform-0.31.1/ai_transform/api/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      333 2023-05-05 02:22:48.000000 ai_transform-0.31.1/ai_transform/api/endpoints.py
+-rw-r--r--   0 runner    (1001) docker     (123)      790 2023-05-05 02:22:48.000000 ai_transform-0.31.1/ai_transform/api/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2708 2023-05-05 02:22:48.000000 ai_transform-0.31.1/ai_transform/api/wrappers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 02:23:05.544369 ai_transform-0.31.1/ai_transform/components/
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-05-05 02:22:48.000000 ai_transform-0.31.1/ai_transform/components/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11976 2023-05-05 02:22:48.000000 ai_transform-0.31.1/ai_transform/components/components.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3788 2023-05-05 02:22:48.000000 ai_transform-0.31.1/ai_transform/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      152 2023-05-05 02:22:48.000000 ai_transform-0.31.1/ai_transform/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 02:23:05.544369 ai_transform-0.31.1/ai_transform/dataset/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 02:22:48.000000 ai_transform-0.31.1/ai_transform/dataset/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11343 2023-05-05 02:22:48.000000 ai_transform-0.31.1/ai_transform/dataset/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15147 2023-05-05 02:22:48.000000 ai_transform-0.31.1/ai_transform/dataset/field.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 02:23:05.544369 ai_transform-0.31.1/ai_transform/engine/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 02:22:48.000000 ai_transform-0.31.1/ai_transform/engine/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15346 2023-05-05 02:22:48.000000 ai_transform-0.31.1/ai_transform/engine/abstract_engine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3252 2023-05-05 02:22:48.000000 ai_transform-0.31.1/ai_transform/engine/dense_output_engine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1363 2023-05-05 02:22:48.000000 ai_transform-0.31.1/ai_transform/engine/in_memory_engine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4505 2023-05-05 02:22:48.000000 ai_transform-0.31.1/ai_transform/engine/multipass_engine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3313 2023-05-05 02:22:48.000000 ai_transform-0.31.1/ai_transform/engine/small_batch_stable_engine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3639 2023-05-05 02:22:48.000000 ai_transform-0.31.1/ai_transform/engine/stable_engine.py
+-rw-r--r--   0 runner    (1001) docker     (123)      826 2023-05-05 02:22:48.000000 ai_transform-0.31.1/ai_transform/errors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1540 2023-05-05 02:22:48.000000 ai_transform-0.31.1/ai_transform/logger.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 02:23:05.544369 ai_transform-0.31.1/ai_transform/operator/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 02:22:48.000000 ai_transform-0.31.1/ai_transform/operator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7119 2023-05-05 02:22:48.000000 ai_transform-0.31.1/ai_transform/operator/abstract_operator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1411 2023-05-05 02:22:48.000000 ai_transform-0.31.1/ai_transform/operator/dense_operator.py
+-rw-r--r--   0 runner    (1001) docker     (123)      556 2023-05-05 02:22:48.000000 ai_transform-0.31.1/ai_transform/timer.py
+-rw-r--r--   0 runner    (1001) docker     (123)      575 2023-05-05 02:22:48.000000 ai_transform-0.31.1/ai_transform/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 02:23:05.544369 ai_transform-0.31.1/ai_transform/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      237 2023-05-05 02:22:48.000000 ai_transform-0.31.1/ai_transform/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8623 2023-05-05 02:22:48.000000 ai_transform-0.31.1/ai_transform/utils/document.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6021 2023-05-05 02:22:48.000000 ai_transform-0.31.1/ai_transform/utils/document_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)      139 2023-05-05 02:22:48.000000 ai_transform-0.31.1/ai_transform/utils/encode_parameters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3383 2023-05-05 02:22:48.000000 ai_transform-0.31.1/ai_transform/utils/example_documents.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3240 2023-05-05 02:22:48.000000 ai_transform-0.31.1/ai_transform/utils/json_encoder.py
+-rw-r--r--   0 runner    (1001) docker     (123)      940 2023-05-05 02:22:48.000000 ai_transform-0.31.1/ai_transform/utils/keyphrase.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 02:23:05.548369 ai_transform-0.31.1/ai_transform/workflow/
+-rw-r--r--   0 runner    (1001) docker     (123)       79 2023-05-05 02:22:48.000000 ai_transform-0.31.1/ai_transform/workflow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3660 2023-05-05 02:22:48.000000 ai_transform-0.31.1/ai_transform/workflow/abstract_workflow.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7496 2023-05-05 02:22:48.000000 ai_transform-0.31.1/ai_transform/workflow/context_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3017 2023-05-05 02:22:48.000000 ai_transform-0.31.1/ai_transform/workflow/helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 02:23:05.544369 ai_transform-0.31.1/ai_transform.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      271 2023-05-05 02:23:05.000000 ai_transform-0.31.1/ai_transform.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2488 2023-05-05 02:23:05.000000 ai_transform-0.31.1/ai_transform.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 02:23:05.000000 ai_transform-0.31.1/ai_transform.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      335 2023-05-05 02:23:05.000000 ai_transform-0.31.1/ai_transform.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-05 02:23:05.000000 ai_transform-0.31.1/ai_transform.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      128 2023-05-05 02:22:48.000000 ai_transform-0.31.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-05 02:23:05.548369 ai_transform-0.31.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      994 2023-05-05 02:22:48.000000 ai_transform-0.31.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 02:23:05.548369 ai_transform-0.31.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 02:22:48.000000 ai_transform-0.31.1/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      302 2023-05-05 02:22:48.000000 ai_transform-0.31.1/tests/components.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11140 2023-05-05 02:22:48.000000 ai_transform-0.31.1/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 02:23:05.548369 ai_transform-0.31.1/tests/core/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 02:22:48.000000 ai_transform-0.31.1/tests/core/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 02:23:05.548369 ai_transform-0.31.1/tests/core/test_api/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 02:22:48.000000 ai_transform-0.31.1/tests/core/test_api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1416 2023-05-05 02:22:48.000000 ai_transform-0.31.1/tests/core/test_api/test_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1130 2023-05-05 02:22:48.000000 ai_transform-0.31.1/tests/core/test_api/test_endpoints.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1003 2023-05-05 02:22:48.000000 ai_transform-0.31.1/tests/core/test_api/test_keyphrase.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5382 2023-05-05 02:22:48.000000 ai_transform-0.31.1/tests/core/test_api/test_wrappers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 02:23:05.548369 ai_transform-0.31.1/tests/core/test_dataset/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 02:22:48.000000 ai_transform-0.31.1/tests/core/test_dataset/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5987 2023-05-05 02:22:48.000000 ai_transform-0.31.1/tests/core/test_dataset/test_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2128 2023-05-05 02:22:48.000000 ai_transform-0.31.1/tests/core/test_dataset/test_field.py
+-rw-r--r--   0 runner    (1001) docker     (123)      951 2023-05-05 02:22:48.000000 ai_transform-0.31.1/tests/core/test_dataset/test_keyphrase.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 02:23:05.548369 ai_transform-0.31.1/tests/core/test_engine/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 02:22:48.000000 ai_transform-0.31.1/tests/core/test_engine/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1910 2023-05-05 02:22:48.000000 ai_transform-0.31.1/tests/core/test_engine/test_dense_output_engine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1977 2023-05-05 02:22:48.000000 ai_transform-0.31.1/tests/core/test_engine/test_engine.py
+-rw-r--r--   0 runner    (1001) docker     (123)      699 2023-05-05 02:22:48.000000 ai_transform-0.31.1/tests/core/test_engine/test_engine_playground.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3327 2023-05-05 02:22:48.000000 ai_transform-0.31.1/tests/core/test_engine/test_multipass_engine.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1016 2023-05-05 02:22:48.000000 ai_transform-0.31.1/tests/core/test_engine/test_stable_engine.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 02:23:05.548369 ai_transform-0.31.1/tests/core/test_operator/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 02:22:48.000000 ai_transform-0.31.1/tests/core/test_operator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      624 2023-05-05 02:22:48.000000 ai_transform-0.31.1/tests/core/test_operator/test_abstract_operator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2153 2023-05-05 02:22:48.000000 ai_transform-0.31.1/tests/core/test_operator/test_document_diff.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 02:23:05.548369 ai_transform-0.31.1/tests/core/test_workflow/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 02:22:48.000000 ai_transform-0.31.1/tests/core/test_workflow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1170 2023-05-05 02:22:48.000000 ai_transform-0.31.1/tests/core/test_workflow/test_context_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3349 2023-05-05 02:22:48.000000 ai_transform-0.31.1/tests/core/test_workflow/test_workflow.py
+-rw-r--r--   0 runner    (1001) docker     (123)      456 2023-05-05 02:22:48.000000 ai_transform-0.31.1/tests/test_connection_retry.py
```

### Comparing `ai_transform-0.31.0/LICENSE` & `ai_transform-0.31.1/LICENSE`

 * *Files identical despite different names*

### Comparing `ai_transform-0.31.0/README.md` & `ai_transform-0.31.1/README.md`

 * *Files identical despite different names*

### Comparing `ai_transform-0.31.0/ai_transform/__init__.py` & `ai_transform-0.31.1/ai_transform/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = "0.31.0"
+__version__ = "0.31.1"
 
 from ai_transform.timer import Timer
 
 _TIMER = Timer()
 _TIMER.start()
```

### Comparing `ai_transform-0.31.0/ai_transform/api/api.py` & `ai_transform-0.31.1/ai_transform/api/api.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,17 @@
 import os
 import time
 import uuid
 import logging
 import requests
 
 from requests.models import Response
-from json import JSONDecodeError
 from functools import wraps
 
-from typing import Any, Dict, List, Optional, Literal
+from typing import Any, Dict, List, Optional, Literal, Callable
 
 from ai_transform.logger import format_logging_info
 from ai_transform.utils import document
 from ai_transform.types import Credentials, FieldTransformer, Filter, Schema
 from ai_transform.api.wrappers import request_wrapper
 
 from ai_transform import __version__
@@ -79,27 +78,33 @@
             # we still want to raise the right error for retrying
             # continue to raise exception so that any retry logic still holds
             raise no_content_e
 
 
 # We implement retry as a function for several reasons
 # first - we can get a
-def retry(num_of_retries: int = 3, timeout: int = 30):
+def retry(num_of_retries: int = 3, timeout: int = 30, retry_func: Callable = None):
     """
     Allows the function to retry upon failure.
     Args:
         num_of_retries: The number of times the function should retry
         timeout: The number of seconds to wait between each retry
     """
 
     def _retry(func):
         @wraps(func)
         def function_wrapper(*args, **kwargs):
             return request_wrapper(
-                func, args, kwargs, num_retries=num_of_retries, timeout=timeout, exponential_backoff=2
+                func,
+                args,
+                kwargs,
+                num_retries=num_of_retries,
+                timeout=timeout,
+                exponential_backoff=2,
+                retry_func=retry_func,
             )
 
         return function_wrapper
 
     return _retry
```

### Comparing `ai_transform-0.31.0/ai_transform/api/client.py` & `ai_transform-0.31.1/ai_transform/api/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -10,15 +10,17 @@
 from ai_transform.errors import AuthException
 from ai_transform.constants import WELCOME_MESSAGE
 from ai_transform.workflow.context_manager import WorkflowContextManager
 from ai_transform.logger import ic
 
 
 class Client:
-    def __init__(self, token: str, authenticate: bool = True) -> None:
+    def __init__(self, token: str = None, authenticate: bool = True) -> None:
+        if token is None:
+            token = os.getenv("DEVELOPMENT_TOKEN")
 
         self._credentials = process_token(token)
         self._token = token
         self._api = API(credentials=self.credentials)
 
         if authenticate:
             try:
```

### Comparing `ai_transform-0.31.0/ai_transform/api/helpers.py` & `ai_transform-0.31.1/ai_transform/api/helpers.py`

 * *Files identical despite different names*

### Comparing `ai_transform-0.31.0/ai_transform/api/wrappers.py` & `ai_transform-0.31.1/ai_transform/api/wrappers.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 import time
 import logging
 import requests
+import traceback
 
 from json import JSONDecodeError
 from ai_transform.logger import format_logging_info, ic
 from requests.models import Response
 from typing import Union, Sequence, Mapping, Callable, Any
 
 logger = logging.getLogger(__file__)
@@ -60,15 +61,15 @@
 
     if kwargs is None:
         kwargs = {}
 
     if retry_func is None:
         retry_func = lambda result: False
 
-    result: requests.Response
+    result: requests.Response = None
 
     for n in range(1, num_retries + 1):
         try:
             result = fn(*args, **kwargs)
 
             if not result.ok:
                 to_log = format_logging_info({"message": result.content.decode(), "status_code": result.status_code})
@@ -81,14 +82,14 @@
                 if output_to_stdout:
                     ic(to_log_for_retry)
                 raise ManualRetryError(to_log_for_retry)
 
             if is_json_decodable or key_for_error:
                 is_response_bad(result=result, key_for_error=key_for_error, output_to_stdout=output_to_stdout)
 
-        except (ResultNotOKError, ManualRetryError, JSONDecodeError, KeyError) as e:
-            ic(e)
+        except (ResultNotOKError, ManualRetryError, JSONDecodeError, KeyError, ConnectionResetError) as e:
+            ic(traceback.format_exc())
             time.sleep(timeout * exponential_backoff**n)
         else:
             return result
 
     return result
```

### Comparing `ai_transform-0.31.0/ai_transform/components/components.py` & `ai_transform-0.31.1/ai_transform/components/components.py`

 * *Files identical despite different names*

### Comparing `ai_transform-0.31.0/ai_transform/config.py` & `ai_transform-0.31.1/ai_transform/config.py`

 * *Files identical despite different names*

### Comparing `ai_transform-0.31.0/ai_transform/dataset/dataset.py` & `ai_transform-0.31.1/ai_transform/dataset/dataset.py`

 * *Files identical despite different names*

### Comparing `ai_transform-0.31.0/ai_transform/dataset/field.py` & `ai_transform-0.31.1/ai_transform/dataset/field.py`

 * *Files identical despite different names*

### Comparing `ai_transform-0.31.0/ai_transform/engine/abstract_engine.py` & `ai_transform-0.31.1/ai_transform/engine/abstract_engine.py`

 * *Files identical despite different names*

### Comparing `ai_transform-0.31.0/ai_transform/engine/dense_output_engine.py` & `ai_transform-0.31.1/ai_transform/engine/dense_output_engine.py`

 * *Files identical despite different names*

### Comparing `ai_transform-0.31.0/ai_transform/engine/in_memory_engine.py` & `ai_transform-0.31.1/ai_transform/engine/in_memory_engine.py`

 * *Files identical despite different names*

### Comparing `ai_transform-0.31.0/ai_transform/engine/multipass_engine.py` & `ai_transform-0.31.1/ai_transform/engine/multipass_engine.py`

 * *Files identical despite different names*

### Comparing `ai_transform-0.31.0/ai_transform/engine/small_batch_stable_engine.py` & `ai_transform-0.31.1/ai_transform/engine/small_batch_stable_engine.py`

 * *Files identical despite different names*

### Comparing `ai_transform-0.31.0/ai_transform/engine/stable_engine.py` & `ai_transform-0.31.1/ai_transform/engine/stable_engine.py`

 * *Files identical despite different names*

### Comparing `ai_transform-0.31.0/ai_transform/errors.py` & `ai_transform-0.31.1/ai_transform/errors.py`

 * *Files identical despite different names*

### Comparing `ai_transform-0.31.0/ai_transform/logger.py` & `ai_transform-0.31.1/ai_transform/logger.py`

 * *Files identical despite different names*

### Comparing `ai_transform-0.31.0/ai_transform/operator/abstract_operator.py` & `ai_transform-0.31.1/ai_transform/operator/abstract_operator.py`

 * *Files identical despite different names*

### Comparing `ai_transform-0.31.0/ai_transform/operator/dense_operator.py` & `ai_transform-0.31.1/ai_transform/operator/dense_operator.py`

 * *Files identical despite different names*

### Comparing `ai_transform-0.31.0/ai_transform/timer.py` & `ai_transform-0.31.1/ai_transform/timer.py`

 * *Files identical despite different names*

### Comparing `ai_transform-0.31.0/ai_transform/types.py` & `ai_transform-0.31.1/ai_transform/types.py`

 * *Files identical despite different names*

### Comparing `ai_transform-0.31.0/ai_transform/utils/document.py` & `ai_transform-0.31.1/ai_transform/utils/document.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 import re
 import uuid
+import pprint
 
 from typing import Dict, Any
 from copy import deepcopy
 from typing import Any, Optional
 from collections import UserDict
 
 from ai_transform.utils.json_encoder import json_encoder
 
 
 class Document(UserDict):
     def __repr__(self):
-        return repr(self.data)
+        return pprint.pformat(self.to_json(), indent=4, width=40)
 
     def __setitem__(self, key: Any, value: Any) -> None:
         try:
             fields = key.split(".")
         except:
             super().__setitem__(key, value)
         else:
```

### Comparing `ai_transform-0.31.0/ai_transform/utils/document_list.py` & `ai_transform-0.31.1/ai_transform/utils/document_list.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,11 @@
+import pprint
 import warnings
 import itertools
+
 from collections import UserList
 from typing import Any, Dict, List, Union
 
 from ai_transform.utils.document import Document
 
 
 class DocumentList(UserList):
@@ -13,15 +15,15 @@
         if initlist is not None:
             for index, document in enumerate(initlist):
                 if not isinstance(document, Document):
                     initlist[index] = Document(document)
         super().__init__(initlist)
 
     def __repr__(self):
-        return repr(self.data)
+        return pprint.pformat(self.to_json(), indent=4, width=40)
 
     def __getitem__(self, key: Union[str, int]) -> Document:
         if isinstance(key, str):
             return [document[key] for document in self.data]
         elif isinstance(key, slice):
             return self.__class__(self.data[key])
         elif isinstance(key, int):
```

### Comparing `ai_transform-0.31.0/ai_transform/utils/example_documents.py` & `ai_transform-0.31.1/ai_transform/utils/example_documents.py`

 * *Files identical despite different names*

### Comparing `ai_transform-0.31.0/ai_transform/utils/json_encoder.py` & `ai_transform-0.31.1/ai_transform/utils/json_encoder.py`

 * *Files identical despite different names*

### Comparing `ai_transform-0.31.0/ai_transform/utils/keyphrase.py` & `ai_transform-0.31.1/ai_transform/utils/keyphrase.py`

 * *Files identical despite different names*

### Comparing `ai_transform-0.31.0/ai_transform/workflow/abstract_workflow.py` & `ai_transform-0.31.1/ai_transform/workflow/abstract_workflow.py`

 * *Files identical despite different names*

### Comparing `ai_transform-0.31.0/ai_transform/workflow/context_manager.py` & `ai_transform-0.31.1/ai_transform/workflow/context_manager.py`

 * *Files 3% similar despite different names*

```diff
@@ -130,15 +130,15 @@
             worker_number=self.worker_number,
             user_errors=user_errors,
             output=self._get_output_to_status_obj(),
         )
         ic(result)
         return result
 
-    def __enter__(self):
+    def __enter__(self) -> "WorkflowContextManager":
         if self.operators is not None:
             self._set_field_children_recursively()
         self.set_workflow_status(status=self.IN_PROGRESS)
         return self
 
     def _handle_workflow_fail(
         self, exc_type: type, exc_value: BaseException, traceback: Traceback, user_errors: str = None
@@ -158,18 +158,25 @@
         if self.operators is not None:
             for operator in self.operators:
                 if operator.is_operator_based_pricing:
                     n_processed_pricing += operator.n_processed_pricing
                     is_automatic = False
 
         if is_automatic:
-            return self._calculate_n_processed_pricing_from_timer()
+            # Use document-based pricing if not manually specified
+            if getattr(self, "engine", None) is not None:
+                return self._calculate_n_processed_pricing_from_size()
+            else:
+                return self._calculate_n_processed_pricing_from_timer()
         else:
             return n_processed_pricing
 
+    def _calculate_n_processed_pricing_from_size(self):
+        return self.engine.size
+
     def _calculate_n_processed_pricing_from_timer(self):
         from ai_transform import _TIMER
 
         return _TIMER.stop()
 
     def set_workflow_pricing(self, n_processed_pricing: float):
         self._n_processed_pricing = n_processed_pricing
```

### Comparing `ai_transform-0.31.0/ai_transform/workflow/helpers.py` & `ai_transform-0.31.1/ai_transform/workflow/helpers.py`

 * *Files identical despite different names*

### Comparing `ai_transform-0.31.0/ai_transform.egg-info/SOURCES.txt` & `ai_transform-0.31.1/ai_transform.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ai_transform-0.31.0/setup.py` & `ai_transform-0.31.1/setup.py`

 * *Files identical despite different names*

### Comparing `ai_transform-0.31.0/tests/conftest.py` & `ai_transform-0.31.1/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `ai_transform-0.31.0/tests/core/test_api/test_client.py` & `ai_transform-0.31.1/tests/core/test_api/test_client.py`

 * *Files identical despite different names*

### Comparing `ai_transform-0.31.0/tests/core/test_api/test_endpoints.py` & `ai_transform-0.31.1/tests/core/test_api/test_endpoints.py`

 * *Files identical despite different names*

### Comparing `ai_transform-0.31.0/tests/core/test_api/test_keyphrase.py` & `ai_transform-0.31.1/tests/core/test_api/test_keyphrase.py`

 * *Files identical despite different names*

### Comparing `ai_transform-0.31.0/tests/core/test_api/test_wrappers.py` & `ai_transform-0.31.1/tests/core/test_api/test_wrappers.py`

 * *Files identical despite different names*

### Comparing `ai_transform-0.31.0/tests/core/test_dataset/test_dataset.py` & `ai_transform-0.31.1/tests/core/test_dataset/test_dataset.py`

 * *Files identical despite different names*

### Comparing `ai_transform-0.31.0/tests/core/test_dataset/test_field.py` & `ai_transform-0.31.1/tests/core/test_dataset/test_field.py`

 * *Files identical despite different names*

### Comparing `ai_transform-0.31.0/tests/core/test_dataset/test_keyphrase.py` & `ai_transform-0.31.1/tests/core/test_dataset/test_keyphrase.py`

 * *Files identical despite different names*

### Comparing `ai_transform-0.31.0/tests/core/test_engine/test_dense_output_engine.py` & `ai_transform-0.31.1/tests/core/test_engine/test_dense_output_engine.py`

 * *Files identical despite different names*

### Comparing `ai_transform-0.31.0/tests/core/test_engine/test_engine.py` & `ai_transform-0.31.1/tests/core/test_engine/test_engine.py`

 * *Files identical despite different names*

### Comparing `ai_transform-0.31.0/tests/core/test_engine/test_engine_playground.py` & `ai_transform-0.31.1/tests/core/test_engine/test_engine_playground.py`

 * *Files identical despite different names*

### Comparing `ai_transform-0.31.0/tests/core/test_engine/test_multipass_engine.py` & `ai_transform-0.31.1/tests/core/test_engine/test_multipass_engine.py`

 * *Files identical despite different names*

### Comparing `ai_transform-0.31.0/tests/core/test_engine/test_stable_engine.py` & `ai_transform-0.31.1/tests/core/test_engine/test_stable_engine.py`

 * *Files identical despite different names*

### Comparing `ai_transform-0.31.0/tests/core/test_operator/test_abstract_operator.py` & `ai_transform-0.31.1/tests/core/test_operator/test_abstract_operator.py`

 * *Files identical despite different names*

### Comparing `ai_transform-0.31.0/tests/core/test_operator/test_document_diff.py` & `ai_transform-0.31.1/tests/core/test_operator/test_document_diff.py`

 * *Files identical despite different names*

### Comparing `ai_transform-0.31.0/tests/core/test_workflow/test_context_manager.py` & `ai_transform-0.31.1/tests/core/test_workflow/test_context_manager.py`

 * *Files identical despite different names*

### Comparing `ai_transform-0.31.0/tests/core/test_workflow/test_workflow.py` & `ai_transform-0.31.1/tests/core/test_workflow/test_workflow.py`

 * *Files identical despite different names*

