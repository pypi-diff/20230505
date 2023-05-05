# Comparing `tmp/bofire-0.0.3.tar.gz` & `tmp/bofire-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bofire-0.0.3.tar", last modified: Thu Nov  3 15:55:19 2022, max compression
+gzip compressed data, was "bofire-0.0.4.tar", last modified: Fri May  5 13:01:54 2023, max compression
```

## Comparing `bofire-0.0.3.tar` & `bofire-0.0.4.tar`

### file list

```diff
@@ -1,43 +1,253 @@
-drwxrwxrwx   0        0        0        0 2022-11-03 15:55:19.717350 bofire-0.0.3/
--rw-rw-rw-   0        0        0     1518 2022-11-03 12:03:47.000000 bofire-0.0.3/LICENSE
--rw-rw-rw-   0        0        0      962 2022-11-03 15:55:19.716350 bofire-0.0.3/PKG-INFO
--rw-rw-rw-   0        0        0      320 2022-11-03 14:55:32.000000 bofire-0.0.3/README.md
-drwxrwxrwx   0        0        0        0 2022-11-03 15:55:19.530353 bofire-0.0.3/bofire/
--rw-rw-rw-   0        0        0       22 2022-11-03 15:29:15.000000 bofire-0.0.3/bofire/__init__.py
-drwxrwxrwx   0        0        0        0 2022-11-03 15:55:19.603350 bofire-0.0.3/bofire/domain/
--rw-rw-rw-   0        0        0       48 2022-11-03 12:03:47.000000 bofire-0.0.3/bofire/domain/__init__.py
--rw-rw-rw-   0        0        0    11778 2022-11-03 12:04:19.000000 bofire-0.0.3/bofire/domain/constraints.py
--rw-rw-rw-   0        0        0    12196 2022-11-03 12:04:19.000000 bofire-0.0.3/bofire/domain/desirability_functions.py
--rw-rw-rw-   0        0        0    36810 2022-11-03 12:04:19.000000 bofire-0.0.3/bofire/domain/domain.py
--rw-rw-rw-   0        0        0    28934 2022-11-03 12:04:18.000000 bofire-0.0.3/bofire/domain/features.py
--rw-rw-rw-   0        0        0     1820 2022-11-03 12:03:47.000000 bofire-0.0.3/bofire/domain/util.py
-drwxrwxrwx   0        0        0        0 2022-11-03 15:55:19.547349 bofire-0.0.3/bofire.egg-info/
--rw-rw-rw-   0        0        0      962 2022-11-03 15:55:19.000000 bofire-0.0.3/bofire.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1027 2022-11-03 15:55:19.000000 bofire-0.0.3/bofire.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-11-03 15:55:19.000000 bofire-0.0.3/bofire.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       75 2022-11-03 15:55:19.000000 bofire-0.0.3/bofire.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2022-11-03 15:55:19.000000 bofire-0.0.3/bofire.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2022-11-03 15:55:19.717350 bofire-0.0.3/setup.cfg
--rw-rw-rw-   0        0        0     1432 2022-11-03 15:44:13.000000 bofire-0.0.3/setup.py
-drwxrwxrwx   0        0        0        0 2022-11-03 15:55:19.612351 bofire-0.0.3/tests/
--rw-rw-rw-   0        0        0        0 2022-11-03 12:03:47.000000 bofire-0.0.3/tests/__init__.py
-drwxrwxrwx   0        0        0        0 2022-11-03 15:55:19.613350 bofire-0.0.3/tests/bofire/
--rw-rw-rw-   0        0        0        0 2022-11-03 12:03:47.000000 bofire-0.0.3/tests/bofire/__init__.py
-drwxrwxrwx   0        0        0        0 2022-11-03 15:55:19.703349 bofire-0.0.3/tests/bofire/domain/
--rw-rw-rw-   0        0        0        0 2022-11-03 12:03:47.000000 bofire-0.0.3/tests/bofire/domain/__init__.py
--rw-rw-rw-   0        0        0      549 2022-11-03 12:04:24.000000 bofire-0.0.3/tests/bofire/domain/test_base_model.py
--rw-rw-rw-   0        0        0     5138 2022-11-03 12:04:24.000000 bofire-0.0.3/tests/bofire/domain/test_concurrency_constraints.py
--rw-rw-rw-   0        0        0     6602 2022-11-03 12:04:24.000000 bofire-0.0.3/tests/bofire/domain/test_constraint_fulfillment.py
--rw-rw-rw-   0        0        0     4010 2022-11-03 12:10:13.000000 bofire-0.0.3/tests/bofire/domain/test_constraints.py
--rw-rw-rw-   0        0        0     5678 2022-11-03 12:10:13.000000 bofire-0.0.3/tests/bofire/domain/test_desirability_functions.py
--rw-rw-rw-   0        0        0    20557 2022-11-03 12:04:23.000000 bofire-0.0.3/tests/bofire/domain/test_domain.py
--rw-rw-rw-   0        0        0    10223 2022-11-03 12:10:13.000000 bofire-0.0.3/tests/bofire/domain/test_domain_validators.py
--rw-rw-rw-   0        0        0    29102 2022-11-03 12:10:13.000000 bofire-0.0.3/tests/bofire/domain/test_features.py
--rw-rw-rw-   0        0        0     2952 2022-11-03 12:04:21.000000 bofire-0.0.3/tests/bofire/domain/test_util.py
--rw-rw-rw-   0        0        0      262 2022-11-03 12:03:47.000000 bofire-0.0.3/tests/bofire/domain/utils.py
-drwxrwxrwx   0        0        0        0 2022-11-03 15:55:19.714348 bofire-0.0.3/tests/bofire/utils/
--rw-rw-rw-   0        0        0        0 2022-11-03 12:03:47.000000 bofire-0.0.3/tests/bofire/utils/__init__.py
--rw-rw-rw-   0        0        0     7557 2022-11-03 12:04:20.000000 bofire-0.0.3/tests/bofire/utils/test_categoricalDescriptorEncoder.py
--rw-rw-rw-   0        0        0    18960 2022-11-03 12:34:05.000000 bofire-0.0.3/tests/bofire/utils/test_reduce.py
--rw-rw-rw-   0        0        0    11230 2022-11-03 12:10:11.000000 bofire-0.0.3/tests/bofire/utils/test_transformer.py
--rw-rw-rw-   0        0        0      590 2022-11-03 12:03:47.000000 bofire-0.0.3/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 13:01:54.681670 bofire-0.0.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1518 2023-05-05 13:01:43.000000 bofire-0.0.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2993 2023-05-05 13:01:54.681670 bofire-0.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2306 2023-05-05 13:01:43.000000 bofire-0.0.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 13:01:54.629670 bofire-0.0.4/bofire/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-05 13:01:43.000000 bofire-0.0.4/bofire/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 13:01:54.633670 bofire-0.0.4/bofire/benchmarks/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 13:01:43.000000 bofire-0.0.4/bofire/benchmarks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8047 2023-05-05 13:01:43.000000 bofire-0.0.4/bofire/benchmarks/aspen_benchmark.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5119 2023-05-05 13:01:43.000000 bofire-0.0.4/bofire/benchmarks/benchmark.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 13:01:54.633670 bofire-0.0.4/bofire/benchmarks/data/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 13:01:43.000000 bofire-0.0.4/bofire/benchmarks/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8591 2023-05-05 13:01:43.000000 bofire-0.0.4/bofire/benchmarks/data/aniline_cn_crosscoupling.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21299 2023-05-05 13:01:43.000000 bofire-0.0.4/bofire/benchmarks/multi.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12080 2023-05-05 13:01:43.000000 bofire-0.0.4/bofire/benchmarks/single.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 13:01:54.633670 bofire-0.0.4/bofire/data_models/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 13:01:43.000000 bofire-0.0.4/bofire/data_models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 13:01:54.633670 bofire-0.0.4/bofire/data_models/acquisition_functions/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 13:01:43.000000 bofire-0.0.4/bofire/data_models/acquisition_functions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      565 2023-05-05 13:01:43.000000 bofire-0.0.4/bofire/data_models/acquisition_functions/acquisition_function.py
+-rw-r--r--   0 runner    (1001) docker     (123)      309 2023-05-05 13:01:43.000000 bofire-0.0.4/bofire/data_models/acquisition_functions/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1655 2023-05-05 13:01:43.000000 bofire-0.0.4/bofire/data_models/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3711 2023-05-05 13:01:43.000000 bofire-0.0.4/bofire/data_models/base.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 13:01:54.637670 bofire-0.0.4/bofire/data_models/constraints/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 13:01:43.000000 bofire-0.0.4/bofire/data_models/constraints/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      724 2023-05-05 13:01:43.000000 bofire-0.0.4/bofire/data_models/constraints/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1729 2023-05-05 13:01:43.000000 bofire-0.0.4/bofire/data_models/constraints/constraint.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7039 2023-05-05 13:01:43.000000 bofire-0.0.4/bofire/data_models/constraints/linear.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4893 2023-05-05 13:01:43.000000 bofire-0.0.4/bofire/data_models/constraints/nchoosek.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2737 2023-05-05 13:01:43.000000 bofire-0.0.4/bofire/data_models/constraints/nonlinear.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 13:01:54.637670 bofire-0.0.4/bofire/data_models/domain/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 13:01:43.000000 bofire-0.0.4/bofire/data_models/domain/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      229 2023-05-05 13:01:43.000000 bofire-0.0.4/bofire/data_models/domain/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3752 2023-05-05 13:01:43.000000 bofire-0.0.4/bofire/data_models/domain/constraints.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26770 2023-05-05 13:01:43.000000 bofire-0.0.4/bofire/data_models/domain/domain.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26741 2023-05-05 13:01:43.000000 bofire-0.0.4/bofire/data_models/domain/features.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1004 2023-05-05 13:01:43.000000 bofire-0.0.4/bofire/data_models/enum.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 13:01:54.641670 bofire-0.0.4/bofire/data_models/features/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 13:01:43.000000 bofire-0.0.4/bofire/data_models/features/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1171 2023-05-05 13:01:43.000000 bofire-0.0.4/bofire/data_models/features/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14122 2023-05-05 13:01:43.000000 bofire-0.0.4/bofire/data_models/features/categorical.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5632 2023-05-05 13:01:43.000000 bofire-0.0.4/bofire/data_models/features/continuous.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10262 2023-05-05 13:01:43.000000 bofire-0.0.4/bofire/data_models/features/descriptor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3283 2023-05-05 13:01:43.000000 bofire-0.0.4/bofire/data_models/features/discrete.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4598 2023-05-05 13:01:43.000000 bofire-0.0.4/bofire/data_models/features/feature.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2442 2023-05-05 13:01:43.000000 bofire-0.0.4/bofire/data_models/features/molecular.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4835 2023-05-05 13:01:43.000000 bofire-0.0.4/bofire/data_models/features/numerical.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 13:01:54.641670 bofire-0.0.4/bofire/data_models/kernels/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 13:01:43.000000 bofire-0.0.4/bofire/data_models/kernels/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2999 2023-05-05 13:01:43.000000 bofire-0.0.4/bofire/data_models/kernels/aggregation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      805 2023-05-05 13:01:43.000000 bofire-0.0.4/bofire/data_models/kernels/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)      501 2023-05-05 13:01:43.000000 bofire-0.0.4/bofire/data_models/kernels/categorical.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1895 2023-05-05 13:01:43.000000 bofire-0.0.4/bofire/data_models/kernels/continuous.py
+-rw-r--r--   0 runner    (1001) docker     (123)      372 2023-05-05 13:01:43.000000 bofire-0.0.4/bofire/data_models/kernels/kernel.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 13:01:54.641670 bofire-0.0.4/bofire/data_models/objectives/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 13:01:43.000000 bofire-0.0.4/bofire/data_models/objectives/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      976 2023-05-05 13:01:43.000000 bofire-0.0.4/bofire/data_models/objectives/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3453 2023-05-05 13:01:43.000000 bofire-0.0.4/bofire/data_models/objectives/identity.py
+-rw-r--r--   0 runner    (1001) docker     (123)      994 2023-05-05 13:01:43.000000 bofire-0.0.4/bofire/data_models/objectives/objective.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2427 2023-05-05 13:01:43.000000 bofire-0.0.4/bofire/data_models/objectives/sigmoid.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2375 2023-05-05 13:01:43.000000 bofire-0.0.4/bofire/data_models/objectives/target.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 13:01:54.645670 bofire-0.0.4/bofire/data_models/priors/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 13:01:43.000000 bofire-0.0.4/bofire/data_models/priors/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      957 2023-05-05 13:01:43.000000 bofire-0.0.4/bofire/data_models/priors/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)      641 2023-05-05 13:01:43.000000 bofire-0.0.4/bofire/data_models/priors/gamma.py
+-rw-r--r--   0 runner    (1001) docker     (123)      582 2023-05-05 13:01:43.000000 bofire-0.0.4/bofire/data_models/priors/normal.py
+-rw-r--r--   0 runner    (1001) docker     (123)      401 2023-05-05 13:01:43.000000 bofire-0.0.4/bofire/data_models/priors/prior.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 13:01:43.000000 bofire-0.0.4/bofire/data_models/serialization.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 13:01:54.645670 bofire-0.0.4/bofire/data_models/strategies/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 13:01:43.000000 bofire-0.0.4/bofire/data_models/strategies/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1672 2023-05-05 13:01:43.000000 bofire-0.0.4/bofire/data_models/strategies/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1041 2023-05-05 13:01:43.000000 bofire-0.0.4/bofire/data_models/strategies/doe.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 13:01:54.645670 bofire-0.0.4/bofire/data_models/strategies/predictives/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 13:01:43.000000 bofire-0.0.4/bofire/data_models/strategies/predictives/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5909 2023-05-05 13:01:43.000000 bofire-0.0.4/bofire/data_models/strategies/predictives/botorch.py
+-rw-r--r--   0 runner    (1001) docker     (123)      914 2023-05-05 13:01:43.000000 bofire-0.0.4/bofire/data_models/strategies/predictives/multiobjective.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2402 2023-05-05 13:01:43.000000 bofire-0.0.4/bofire/data_models/strategies/predictives/predictive.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1943 2023-05-05 13:01:43.000000 bofire-0.0.4/bofire/data_models/strategies/predictives/qehvi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1115 2023-05-05 13:01:43.000000 bofire-0.0.4/bofire/data_models/strategies/predictives/qnehvi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1089 2023-05-05 13:01:43.000000 bofire-0.0.4/bofire/data_models/strategies/predictives/qparego.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2140 2023-05-05 13:01:43.000000 bofire-0.0.4/bofire/data_models/strategies/predictives/sobo.py
+-rw-r--r--   0 runner    (1001) docker     (123)      844 2023-05-05 13:01:43.000000 bofire-0.0.4/bofire/data_models/strategies/random.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 13:01:54.645670 bofire-0.0.4/bofire/data_models/strategies/samplers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 13:01:43.000000 bofire-0.0.4/bofire/data_models/strategies/samplers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1535 2023-05-05 13:01:43.000000 bofire-0.0.4/bofire/data_models/strategies/samplers/polytope.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1694 2023-05-05 13:01:43.000000 bofire-0.0.4/bofire/data_models/strategies/samplers/rejection.py
+-rw-r--r--   0 runner    (1001) docker     (123)      201 2023-05-05 13:01:43.000000 bofire-0.0.4/bofire/data_models/strategies/samplers/sampler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3527 2023-05-05 13:01:43.000000 bofire-0.0.4/bofire/data_models/strategies/strategy.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 13:01:54.649670 bofire-0.0.4/bofire/data_models/surrogates/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 13:01:43.000000 bofire-0.0.4/bofire/data_models/surrogates/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1281 2023-05-05 13:01:43.000000 bofire-0.0.4/bofire/data_models/surrogates/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1874 2023-05-05 13:01:43.000000 bofire-0.0.4/bofire/data_models/surrogates/botorch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4703 2023-05-05 13:01:43.000000 bofire-0.0.4/bofire/data_models/surrogates/botorch_surrogates.py
+-rw-r--r--   0 runner    (1001) docker     (123)      204 2023-05-05 13:01:43.000000 bofire-0.0.4/bofire/data_models/surrogates/empirical.py
+-rw-r--r--   0 runner    (1001) docker     (123)      746 2023-05-05 13:01:43.000000 bofire-0.0.4/bofire/data_models/surrogates/fully_bayesian.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1258 2023-05-05 13:01:43.000000 bofire-0.0.4/bofire/data_models/surrogates/mixed_single_task_gp.py
+-rw-r--r--   0 runner    (1001) docker     (123)      610 2023-05-05 13:01:43.000000 bofire-0.0.4/bofire/data_models/surrogates/mlp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1016 2023-05-05 13:01:43.000000 bofire-0.0.4/bofire/data_models/surrogates/random_forest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      229 2023-05-05 13:01:43.000000 bofire-0.0.4/bofire/data_models/surrogates/scaler.py
+-rw-r--r--   0 runner    (1001) docker     (123)      822 2023-05-05 13:01:43.000000 bofire-0.0.4/bofire/data_models/surrogates/single_task_gp.py
+-rw-r--r--   0 runner    (1001) docker     (123)      997 2023-05-05 13:01:43.000000 bofire-0.0.4/bofire/data_models/surrogates/surrogate.py
+-rw-r--r--   0 runner    (1001) docker     (123)      363 2023-05-05 13:01:43.000000 bofire-0.0.4/bofire/data_models/unions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2668 2023-05-05 13:01:43.000000 bofire-0.0.4/bofire/data_models/validated.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 13:01:54.649670 bofire-0.0.4/bofire/plot/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 13:01:43.000000 bofire-0.0.4/bofire/plot/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      244 2023-05-05 13:01:43.000000 bofire-0.0.4/bofire/plot/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4123 2023-05-05 13:01:43.000000 bofire-0.0.4/bofire/plot/feature_importance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1462 2023-05-05 13:01:43.000000 bofire-0.0.4/bofire/plot/objective.py
+-rw-r--r--   0 runner    (1001) docker     (123)      924 2023-05-05 13:01:43.000000 bofire-0.0.4/bofire/plot/prior.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 13:01:54.653670 bofire-0.0.4/bofire/strategies/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 13:01:43.000000 bofire-0.0.4/bofire/strategies/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1028 2023-05-05 13:01:43.000000 bofire-0.0.4/bofire/strategies/api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 13:01:54.653670 bofire-0.0.4/bofire/strategies/data_models/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 13:01:43.000000 bofire-0.0.4/bofire/strategies/data_models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1320 2023-05-05 13:01:43.000000 bofire-0.0.4/bofire/strategies/data_models/candidate.py
+-rw-r--r--   0 runner    (1001) docker     (123)      679 2023-05-05 13:01:43.000000 bofire-0.0.4/bofire/strategies/data_models/values.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 13:01:54.653670 bofire-0.0.4/bofire/strategies/doe/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 13:01:43.000000 bofire-0.0.4/bofire/strategies/doe/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9466 2023-05-05 13:01:43.000000 bofire-0.0.4/bofire/strategies/doe/design.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16789 2023-05-05 13:01:43.000000 bofire-0.0.4/bofire/strategies/doe/objective.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18128 2023-05-05 13:01:43.000000 bofire-0.0.4/bofire/strategies/doe/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1556 2023-05-05 13:01:43.000000 bofire-0.0.4/bofire/strategies/doe_strategy.py
+-rw-r--r--   0 runner    (1001) docker     (123)      267 2023-05-05 13:01:43.000000 bofire-0.0.4/bofire/strategies/enum.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1792 2023-05-05 13:01:43.000000 bofire-0.0.4/bofire/strategies/mapper.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 13:01:54.657670 bofire-0.0.4/bofire/strategies/predictives/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 13:01:43.000000 bofire-0.0.4/bofire/strategies/predictives/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19396 2023-05-05 13:01:43.000000 bofire-0.0.4/bofire/strategies/predictives/botorch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6391 2023-05-05 13:01:43.000000 bofire-0.0.4/bofire/strategies/predictives/predictive.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3713 2023-05-05 13:01:43.000000 bofire-0.0.4/bofire/strategies/predictives/qehvi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1720 2023-05-05 13:01:43.000000 bofire-0.0.4/bofire/strategies/predictives/qnehvi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3974 2023-05-05 13:01:43.000000 bofire-0.0.4/bofire/strategies/predictives/qparego.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4879 2023-05-05 13:01:43.000000 bofire-0.0.4/bofire/strategies/predictives/sobo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1528 2023-05-05 13:01:43.000000 bofire-0.0.4/bofire/strategies/random.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 13:01:54.657670 bofire-0.0.4/bofire/strategies/samplers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 13:01:43.000000 bofire-0.0.4/bofire/strategies/samplers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6764 2023-05-05 13:01:43.000000 bofire-0.0.4/bofire/strategies/samplers/polytope.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2119 2023-05-05 13:01:43.000000 bofire-0.0.4/bofire/strategies/samplers/rejection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3659 2023-05-05 13:01:43.000000 bofire-0.0.4/bofire/strategies/samplers/sampler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8150 2023-05-05 13:01:43.000000 bofire-0.0.4/bofire/strategies/strategy.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 13:01:54.661670 bofire-0.0.4/bofire/surrogates/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 13:01:43.000000 bofire-0.0.4/bofire/surrogates/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      734 2023-05-05 13:01:43.000000 bofire-0.0.4/bofire/surrogates/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2764 2023-05-05 13:01:43.000000 bofire-0.0.4/bofire/surrogates/botorch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5330 2023-05-05 13:01:43.000000 bofire-0.0.4/bofire/surrogates/botorch_surrogates.py
+-rw-r--r--   0 runner    (1001) docker     (123)      404 2023-05-05 13:01:43.000000 bofire-0.0.4/bofire/surrogates/cloudpickle_module.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15738 2023-05-05 13:01:43.000000 bofire-0.0.4/bofire/surrogates/diagnostics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1973 2023-05-05 13:01:43.000000 bofire-0.0.4/bofire/surrogates/empirical.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5506 2023-05-05 13:01:43.000000 bofire-0.0.4/bofire/surrogates/feature_importance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2409 2023-05-05 13:01:43.000000 bofire-0.0.4/bofire/surrogates/fully_bayesian.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1119 2023-05-05 13:01:43.000000 bofire-0.0.4/bofire/surrogates/mapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3310 2023-05-05 13:01:43.000000 bofire-0.0.4/bofire/surrogates/mixed_single_task_gp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7367 2023-05-05 13:01:43.000000 bofire-0.0.4/bofire/surrogates/mlp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5347 2023-05-05 13:01:43.000000 bofire-0.0.4/bofire/surrogates/random_forest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3908 2023-05-05 13:01:43.000000 bofire-0.0.4/bofire/surrogates/single_task_gp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3712 2023-05-05 13:01:43.000000 bofire-0.0.4/bofire/surrogates/surrogate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7319 2023-05-05 13:01:43.000000 bofire-0.0.4/bofire/surrogates/trainable.py
+-rw-r--r--   0 runner    (1001) docker     (123)      526 2023-05-05 13:01:43.000000 bofire-0.0.4/bofire/surrogates/values.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 13:01:54.665670 bofire-0.0.4/bofire/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 13:01:43.000000 bofire-0.0.4/bofire/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2801 2023-05-05 13:01:43.000000 bofire-0.0.4/bofire/utils/cheminformatics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1899 2023-05-05 13:01:43.000000 bofire-0.0.4/bofire/utils/doe.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5059 2023-05-05 13:01:43.000000 bofire-0.0.4/bofire/utils/multiobjective.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15585 2023-05-05 13:01:43.000000 bofire-0.0.4/bofire/utils/reduce.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2081 2023-05-05 13:01:43.000000 bofire-0.0.4/bofire/utils/subdomain.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14283 2023-05-05 13:01:43.000000 bofire-0.0.4/bofire/utils/torch_tools.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 13:01:54.629670 bofire-0.0.4/bofire.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2993 2023-05-05 13:01:54.000000 bofire-0.0.4/bofire.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8354 2023-05-05 13:01:54.000000 bofire-0.0.4/bofire.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 13:01:54.000000 bofire-0.0.4/bofire.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      384 2023-05-05 13:01:54.000000 bofire-0.0.4/bofire.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-05 13:01:54.000000 bofire-0.0.4/bofire.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      317 2023-05-05 13:01:54.681670 bofire-0.0.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2152 2023-05-05 13:01:43.000000 bofire-0.0.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 13:01:54.665670 bofire-0.0.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 13:01:43.000000 bofire-0.0.4/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 13:01:54.665670 bofire-0.0.4/tests/bofire/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 13:01:43.000000 bofire-0.0.4/tests/bofire/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 13:01:54.665670 bofire-0.0.4/tests/bofire/benchmarks/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 13:01:43.000000 bofire-0.0.4/tests/bofire/benchmarks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3476 2023-05-05 13:01:43.000000 bofire-0.0.4/tests/bofire/benchmarks/test_aspen_benchmark.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1549 2023-05-05 13:01:43.000000 bofire-0.0.4/tests/bofire/benchmarks/test_benchmark.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2601 2023-05-05 13:01:43.000000 bofire-0.0.4/tests/bofire/benchmarks/test_multi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3315 2023-05-05 13:01:43.000000 bofire-0.0.4/tests/bofire/benchmarks/test_single.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1234 2023-05-05 13:01:43.000000 bofire-0.0.4/tests/bofire/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 13:01:54.669670 bofire-0.0.4/tests/bofire/data_models/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 13:01:43.000000 bofire-0.0.4/tests/bofire/data_models/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 13:01:54.669670 bofire-0.0.4/tests/bofire/data_models/serialization/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 13:01:43.000000 bofire-0.0.4/tests/bofire/data_models/serialization/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2290 2023-05-05 13:01:43.000000 bofire-0.0.4/tests/bofire/data_models/serialization/test_deserialization.py
+-rw-r--r--   0 runner    (1001) docker     (123)      235 2023-05-05 13:01:43.000000 bofire-0.0.4/tests/bofire/data_models/serialization/test_schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1815 2023-05-05 13:01:43.000000 bofire-0.0.4/tests/bofire/data_models/serialization/test_serialization.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 13:01:54.673670 bofire-0.0.4/tests/bofire/data_models/specs/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 13:01:43.000000 bofire-0.0.4/tests/bofire/data_models/specs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      578 2023-05-05 13:01:43.000000 bofire-0.0.4/tests/bofire/data_models/specs/acquisition_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1041 2023-05-05 13:01:43.000000 bofire-0.0.4/tests/bofire/data_models/specs/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1191 2023-05-05 13:01:43.000000 bofire-0.0.4/tests/bofire/data_models/specs/constraints.py
+-rw-r--r--   0 runner    (1001) docker     (123)      858 2023-05-05 13:01:43.000000 bofire-0.0.4/tests/bofire/data_models/specs/domain.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2264 2023-05-05 13:01:43.000000 bofire-0.0.4/tests/bofire/data_models/specs/features.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1263 2023-05-05 13:01:43.000000 bofire-0.0.4/tests/bofire/data_models/specs/kernels.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1033 2023-05-05 13:01:43.000000 bofire-0.0.4/tests/bofire/data_models/specs/objectives.py
+-rw-r--r--   0 runner    (1001) docker     (123)      405 2023-05-05 13:01:43.000000 bofire-0.0.4/tests/bofire/data_models/specs/priors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3763 2023-05-05 13:01:43.000000 bofire-0.0.4/tests/bofire/data_models/specs/specs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3071 2023-05-05 13:01:43.000000 bofire-0.0.4/tests/bofire/data_models/specs/strategies.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4220 2023-05-05 13:01:43.000000 bofire-0.0.4/tests/bofire/data_models/specs/surrogates.py
+-rw-r--r--   0 runner    (1001) docker     (123)      530 2023-05-05 13:01:43.000000 bofire-0.0.4/tests/bofire/data_models/test_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6162 2023-05-05 13:01:43.000000 bofire-0.0.4/tests/bofire/data_models/test_constraint_fulfillment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6499 2023-05-05 13:01:43.000000 bofire-0.0.4/tests/bofire/data_models/test_constraints.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22806 2023-05-05 13:01:43.000000 bofire-0.0.4/tests/bofire/data_models/test_domain.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9961 2023-05-05 13:01:43.000000 bofire-0.0.4/tests/bofire/data_models/test_domain_validators.py
+-rw-r--r--   0 runner    (1001) docker     (123)    55338 2023-05-05 13:01:43.000000 bofire-0.0.4/tests/bofire/data_models/test_features.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7296 2023-05-05 13:01:43.000000 bofire-0.0.4/tests/bofire/data_models/test_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5465 2023-05-05 13:01:43.000000 bofire-0.0.4/tests/bofire/data_models/test_kernels.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2229 2023-05-05 13:01:43.000000 bofire-0.0.4/tests/bofire/data_models/test_molecular.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6120 2023-05-05 13:01:43.000000 bofire-0.0.4/tests/bofire/data_models/test_nchoosek_combinatorics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1203 2023-05-05 13:01:43.000000 bofire-0.0.4/tests/bofire/data_models/test_numeric.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2440 2023-05-05 13:01:43.000000 bofire-0.0.4/tests/bofire/data_models/test_priors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5263 2023-05-05 13:01:43.000000 bofire-0.0.4/tests/bofire/data_models/test_samplers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      709 2023-05-05 13:01:43.000000 bofire-0.0.4/tests/bofire/data_models/test_unions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7296 2023-05-05 13:01:43.000000 bofire-0.0.4/tests/bofire/data_models/test_util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 13:01:54.677670 bofire-0.0.4/tests/bofire/strategies/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 13:01:43.000000 bofire-0.0.4/tests/bofire/strategies/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 13:01:54.677670 bofire-0.0.4/tests/bofire/strategies/doe/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 13:01:43.000000 bofire-0.0.4/tests/bofire/strategies/doe/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15025 2023-05-05 13:01:43.000000 bofire-0.0.4/tests/bofire/strategies/doe/test_design.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20262 2023-05-05 13:01:43.000000 bofire-0.0.4/tests/bofire/strategies/doe/test_objective.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21977 2023-05-05 13:01:43.000000 bofire-0.0.4/tests/bofire/strategies/doe/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4994 2023-05-05 13:01:43.000000 bofire-0.0.4/tests/bofire/strategies/dummy.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10648 2023-05-05 13:01:43.000000 bofire-0.0.4/tests/bofire/strategies/specs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1592 2023-05-05 13:01:43.000000 bofire-0.0.4/tests/bofire/strategies/test_all.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3401 2023-05-05 13:01:43.000000 bofire-0.0.4/tests/bofire/strategies/test_ask.py
+-rw-r--r--   0 runner    (1001) docker     (123)    27492 2023-05-05 13:01:43.000000 bofire-0.0.4/tests/bofire/strategies/test_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6077 2023-05-05 13:01:43.000000 bofire-0.0.4/tests/bofire/strategies/test_doe.py
+-rw-r--r--   0 runner    (1001) docker     (123)      236 2023-05-05 13:01:43.000000 bofire-0.0.4/tests/bofire/strategies/test_from_data_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3911 2023-05-05 13:01:43.000000 bofire-0.0.4/tests/bofire/strategies/test_model_specs_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8383 2023-05-05 13:01:43.000000 bofire-0.0.4/tests/bofire/strategies/test_qehvi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7171 2023-05-05 13:01:43.000000 bofire-0.0.4/tests/bofire/strategies/test_qparego.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4075 2023-05-05 13:01:43.000000 bofire-0.0.4/tests/bofire/strategies/test_random.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5635 2023-05-05 13:01:43.000000 bofire-0.0.4/tests/bofire/strategies/test_sobo.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15655 2023-05-05 13:01:43.000000 bofire-0.0.4/tests/bofire/strategies/test_strategy.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 13:01:54.681670 bofire-0.0.4/tests/bofire/surrogates/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 13:01:43.000000 bofire-0.0.4/tests/bofire/surrogates/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6934 2023-05-05 13:01:43.000000 bofire-0.0.4/tests/bofire/surrogates/test_cross_validate.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13140 2023-05-05 13:01:43.000000 bofire-0.0.4/tests/bofire/surrogates/test_diagnostics.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3384 2023-05-05 13:01:43.000000 bofire-0.0.4/tests/bofire/surrogates/test_feature_importance.py
+-rw-r--r--   0 runner    (1001) docker     (123)      225 2023-05-05 13:01:43.000000 bofire-0.0.4/tests/bofire/surrogates/test_from_data_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1218 2023-05-05 13:01:43.000000 bofire-0.0.4/tests/bofire/surrogates/test_fully_bayesian.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8685 2023-05-05 13:01:43.000000 bofire-0.0.4/tests/bofire/surrogates/test_gps.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7702 2023-05-05 13:01:43.000000 bofire-0.0.4/tests/bofire/surrogates/test_mlp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3376 2023-05-05 13:01:43.000000 bofire-0.0.4/tests/bofire/surrogates/test_random_forest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3294 2023-05-05 13:01:43.000000 bofire-0.0.4/tests/bofire/surrogates/test_surrogates.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34238 2023-05-05 13:01:43.000000 bofire-0.0.4/tests/bofire/surrogates/test_torch_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)      590 2023-05-05 13:01:43.000000 bofire-0.0.4/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1160 2023-05-05 13:01:43.000000 bofire-0.0.4/tests/test_docs.py
```

### Comparing `bofire-0.0.3/LICENSE` & `bofire-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `bofire-0.0.3/bofire/domain/domain.py` & `bofire-0.0.4/bofire/data_models/domain/domain.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,159 +1,195 @@
+import collections.abc
 import itertools
-from copy import deepcopy
-from typing import Dict, List, Optional, Tuple, Type, Union
+from typing import (
+    Any,
+    Dict,
+    List,
+    Literal,
+    Optional,
+    Sequence,
+    Tuple,
+    Type,
+    Union,
+    get_args,
+    get_origin,
+)
 
 import numpy as np
 import pandas as pd
 from pydantic import Field, validator
 
-from bofire.domain.constraints import Constraint, LinearConstraint, NChooseKConstraint
-from bofire.domain.features import (
-    CategoricalInputFeature,
-    ContinuousInputFeature,
-    ContinuousOutputFeature,
-    ContinuousOutputFeature_woDesFunc,
+from bofire.data_models.base import BaseModel
+from bofire.data_models.constraints.api import (
+    AnyConstraint,
+    LinearConstraint,
+    NChooseKConstraint,
+)
+from bofire.data_models.domain.constraints import Constraints
+from bofire.data_models.domain.features import Features, Inputs, Outputs
+from bofire.data_models.features.api import (
+    AnyInput,
+    AnyOutput,
+    ContinuousInput,
+    ContinuousOutput,
     Feature,
-    InputFeature,
-    OutputFeature,
+    Input,
+    Output,
 )
-from bofire.domain.util import BaseModel, filter_by_class, is_categorical, is_numeric
+from bofire.data_models.objectives.api import Objective
+
+
+def isinstance_or_union(obj, of):
+    if get_origin(of) is Union:
+        of = get_args(of)
+    return isinstance(obj, of)
+
+
+def is_numeric(s: Union[pd.Series, pd.DataFrame]) -> bool:
+    if isinstance(s, pd.Series):
+        return pd.to_numeric(s, errors="coerce").notnull().all()
+    return s.apply(lambda s: pd.to_numeric(s, errors="coerce").notnull().all()).all()  # type: ignore
 
 
 class Domain(BaseModel):
+    type: Literal["Domain"] = "Domain"
+
+    inputs: Inputs = Field(default_factory=lambda: Inputs())
+    outputs: Outputs = Field(default_factory=lambda: Outputs())
+
+    constraints: Constraints = Field(default_factory=lambda: Constraints())
 
-    input_features: Optional[List[InputFeature]] = Field(default_factory=lambda: [])
-    output_features: Optional[List[OutputFeature]] = Field(default_factory=lambda: [])
-    constraints: Optional[List[Constraint]] = Field(default_factory=lambda: [])
-    experiments: Optional[pd.DataFrame]
-    candidates: Optional[pd.DataFrame]
     """Representation of the optimization problem/domain
 
     Attributes:
-        input_features (List[InputFeature], optional): List of input features. Defaults to [].
-        output_features (List[OutputFeature], optional): List of output features. Defaults to [].
+        inputs (List[Input], optional): List of input features. Defaults to [].
+        outputs (List[Output], optional): List of output features. Defaults to [].
         constraints (List[Constraint], optional): List of constraints. Defaults to [].
     """
 
-    @validator("output_features", always=True)
-    def validate_unique_output_feature_keys(cls, v, values):
-        """Validates if provided output feature keys are unique
+    @classmethod
+    def from_lists(
+        cls,
+        inputs: Optional[Sequence[AnyInput]] = None,
+        outputs: Optional[Sequence[AnyOutput]] = None,
+        constraints: Optional[Sequence[AnyConstraint]] = None,
+    ):
+        inputs = [] if inputs is None else inputs
+        outputs = [] if outputs is None else outputs
+        constraints = [] if constraints is None else constraints
+        return cls(
+            inputs=Inputs(features=inputs),
+            outputs=Outputs(features=outputs),
+            constraints=Constraints(constraints=constraints),
+        )
+
+    @validator("inputs", always=True, pre=True)
+    def validate_inputs_list(cls, v, values):
+        if isinstance(v, collections.abc.Sequence):
+            v = Inputs(features=v)
+            return v
+        if isinstance_or_union(v, AnyInput):
+            return Inputs(features=[v])
+        else:
+            return v
+
+    @validator("outputs", always=True, pre=True)
+    def validate_outputs_list(cls, v, values):
+        if isinstance(v, collections.abc.Sequence):
+            return Outputs(features=v)
+        if isinstance_or_union(v, AnyOutput):
+            return Outputs(features=[v])
+        else:
+            return v
+
+    @validator("constraints", always=True, pre=True)
+    def validate_constraints_list(cls, v, values):
+        if isinstance(v, list):
+            return Constraints(constraints=v)
+        if isinstance_or_union(v, AnyConstraint):
+            return Constraints(constraints=[v])
+        else:
+            return v
+
+    @validator("outputs", always=True)
+    def validate_unique_feature_keys(cls, v: Outputs, values) -> Outputs:
+        """Validates if provided input and output feature keys are unique
 
         Args:
-            v (List[OutputFeature]): List of all output features of the domain.
-            values (List[InputFeature]): Dict containing a list of input features as single entry.
+            v (Outputs): List of all output features of the domain.
+            value (Dict[str, Inputs]): Dict containing a list of input features as single entry.
 
         Raises:
             ValueError: Feature keys are not unique.
 
         Returns:
-            List[OutputFeature]: Returns the list of output features when no error is thrown.
+            Outputs: Keeps output features as given.
         """
-        if "input_features" not in values:
+        if "inputs" not in values:
             return v
-        features = v + values["input_features"]
+        features = v + values["inputs"]
         keys = [f.key for f in features]
         if len(set(keys)) != len(keys):
             raise ValueError("feature keys are not unique")
         return v
 
     @validator("constraints", always=True)
     def validate_constraints(cls, v, values):
         """Validate if all features included in the constraints are also defined as features for the domain.
 
         Args:
             v (List[Constraint]): List of constraints or empty if no constraints are defined
-            values (List[InputFeature]): List of input features of the domain
+            values (List[Input]): List of input features of the domain
 
         Raises:
             ValueError: Feature key in constraint is unknown.
 
         Returns:
             List[Constraint]: List of constraints defined for the domain
         """
-        if "input_features" not in values:
+        if "inputs" not in values:
             return v
-        keys = [f.key for f in values["input_features"]]
+        keys = [f.key for f in values["inputs"]]
         for c in v:
             if isinstance(c, LinearConstraint) or isinstance(c, NChooseKConstraint):
                 for f in c.features:
                     if f not in keys:
                         raise ValueError(f"feature {f} in constraint unknown ({keys})")
         return v
 
     @validator("constraints", always=True)
-    def validate_lower_bounds_in_nchoosek_constraints(cls, v, values):
-        """Validate the lower bound as well if the chosen number of allowed features is continuous.
+    def validate_linear_constraints(cls, v, values):
+        """Validate if all features included in linear constraints are continuous ones.
 
         Args:
-            v (List[Constraint]): List of all constraints defined for the domain
-            values (List[InputFeature]): _description_
-
-        Returns:
-            List[Constraint]: List of constraints defined for the domain
-        """
-        # gather continuous input_features in dictionary
-        continuous_input_features_dict = {}
-        for f in values["input_features"]:
-            if type(f) is ContinuousInputFeature:
-                continuous_input_features_dict[f.key] = f
+            v (List[Constraint]): List of constraints or empty if no constraints are defined
+            values (List[Input]): List of input features of the domain
 
-        # check if unfixed continuous features appearing in NChooseK constraints have lower bound of 0
-        for c in v:
-            if isinstance(c, NChooseKConstraint):
-                for f in c.features:
-                    assert (
-                        f in continuous_input_features_dict
-                    ), f"{f} must be continuous."
-                    assert (
-                        continuous_input_features_dict[f].lower_bound == 0
-                    ), f"lower bound of {f} must be 0 for NChooseK constraint."
-        return v
+        Raises:
+            ValueError: _description_
 
-    def to_config(self) -> Dict:
-        """Serializables itself to a dictionary.
 
         Returns:
-            Dict: Serialized version of the domain as dictionary.
+           List[Constraint]: List of constraints defined for the domain
         """
-        config = {
-            "input_features": [feat.to_config() for feat in self.input_features],
-            "output_features": [feat.to_config() for feat in self.output_features],
-            "constraints": [constraint.to_config() for constraint in self.constraints],
-        }
-        if self.experiments is not None:
-            config["experiments"] = self.experiments.to_dict()
-        if self.candidates is not None:
-            config["candidates"] = self.candidates.to_dict()
-        return config
+        if "inputs" not in values:
+            return v
 
-    @classmethod
-    def from_config(cls, config: Dict):
-        """Instantiates a `Domain` object from a dictionary created by the `to_config`method.
+        # gather continuous inputs in dictionary
+        continuous_inputs_dict = {}
+        for f in values["inputs"]:
+            if type(f) is ContinuousInput:
+                continuous_inputs_dict[f.key] = f
 
-        Args:
-            config (Dict): Serialized version of a domain as dictionary.
-        """
-        d = cls(
-            input_features=[
-                Feature.from_config(feat) for feat in config["input_features"]
-            ],
-            output_features=[
-                Feature.from_config(feat) for feat in config["output_features"]
-            ],
-            constraints=[
-                Constraint.from_config(constraint)
-                for constraint in config["constraints"]
-            ],
-        )
-        if "experiments" in config.keys():
-            d.add_experiments(experiments=config["experiments"])
-        if "candidates" in config.keys():
-            d.add_candidates(experiments=config["candidates"])
-        return d
+        # check if non continuous input features appear in linear constraints
+        for c in v:
+            if isinstance(c, LinearConstraint):
+                for f in c.features:
+                    assert f in continuous_inputs_dict, f"{f} must be continuous."
+        return v
 
     def get_feature_reps_df(self) -> pd.DataFrame:
         """Returns a pandas dataframe describing the features contained in the optimization domain."""
         df = pd.DataFrame(
             index=self.get_feature_keys(Feature),
             columns=["Type", "Description"],
             data={
@@ -168,74 +204,45 @@
     def get_constraint_reps_df(self):
         """Provides a tabular overwiev of all constraints within the domain
 
         Returns:
             pd.DataFrame: DataFrame listing all constraints of the domain with a description
         """
         df = pd.DataFrame(
-            index=range(len(self.get_constraints())),
+            index=range(len(self.constraints)),
             columns=["Type", "Description"],
             data={
-                "Type": [feat.__class__.__name__ for feat in self.get_constraints()],
+                "Type": [feat.__class__.__name__ for feat in self.constraints],
                 "Description": [
-                    constraint.__str__() for constraint in self.get_constraints()
+                    constraint.__str__() for constraint in self.constraints
                 ],
             },
         )
         return df
 
-    def get_constraints(
-        self,
-        includes: Union[Type, List[Type]] = Constraint,
-        excludes: Union[Type, List[Type]] = None,
-        exact: bool = False,
-    ) -> List[Constraint]:
-        """get constraints of the domain
-
-        Args:
-            includes (Union[Constraint, List[Constraint]], optional): Constraint class or list of specific constraint classes to be returned. Defaults to Constraint.
-            excludes (Union[Type, List[Type]], optional): Constraint class or list of specific constraint classes to be excluded from the return. Defaults to None.
-            exact (bool, optional): Boolean to distinguish if only the exact class listed in includes and no subclasses inherenting from this class shall be returned. Defaults to False.
-
-        Returns:
-            List[Constraint]: List of constraints in the domain fitting to the passed requirements.
-        """
-        return filter_by_class(
-            self.constraints,
-            includes=includes,
-            excludes=excludes,
-            exact=exact,
-        )
-
     def get_features(
         self,
-        includes: Union[Type, List[Type]] = Feature,
-        excludes: Union[Type, List[Type]] = None,
+        includes: Union[Type[Feature], List[Type[Feature]]] = Feature,
+        excludes: Union[Type[Feature], List[Type[Feature]], None] = None,
         exact: bool = False,
-    ) -> List[Feature]:
+    ) -> Features:
         """get features of the domain
 
         Args:
             includes (Union[Type, List[Type]], optional): Feature class or list of specific feature classes to be returned. Defaults to Feature.
             excludes (Union[Type, List[Type]], optional): Feature class or list of specific feature classes to be excluded from the return. Defaults to None.
             exact (bool, optional): Boolean to distinguish if only the exact class listed in includes and no subclasses inherenting from this class shall be returned. Defaults to False.
+            by_attribute (str, optional): If set it is filtered by the attribute specified in by `by_attribute`. Defaults to None.
 
         Returns:
             List[Feature]: List of features in the domain fitting to the passed requirements.
         """
-        return list(
-            sorted(
-                filter_by_class(
-                    self.input_features + self.output_features,
-                    includes=includes,
-                    excludes=excludes,
-                    exact=exact,
-                )
-            )
-        )
+        assert isinstance(self.inputs, Inputs)
+        features = self.inputs + self.outputs
+        return features.get(includes, excludes, exact)
 
     def get_feature_keys(
         self,
         includes: Union[Type, List[Type]] = Feature,
         excludes: Union[Type, List[Type]] = None,
         exact: bool = False,
     ) -> List[str]:
@@ -263,129 +270,60 @@
 
         Args:
             key (str): Feature key
 
         Returns:
             Feature: The feature with the passed key
         """
-        return {f.key: f for f in self.input_features + self.output_features}[key]
-
-    def add_constraint(self, constraint: Constraint):
-        """Add a constraint to the optimzation domain
-
-        Args:
-            constraint (Constraint): object of class Constraint, which is added to the list
-        """
-        self.constraints.append(constraint)
-
-    def add_feature(self, feature: Feature) -> None:
-        """add a feature to list domain.features
-
-        Args:
-            feature (Feature): object of class Feature, which is added to the list
-
-        Raises:
-            ValueError: if the feature key is already in the domain
-            TypeError: if the feature type is neither Input nor Output feature
-        """
-        if (self.experiments is not None) or (self.candidates is not None):
-            raise ValueError(
-                "Feature cannot be added as experiments/candidates are already set."
-            )
-        if feature.key in self.get_feature_keys():
-            raise ValueError(f"Feature with key {feature.key} already in domain.")
-        if isinstance(feature, InputFeature):
-            self.input_features.append(feature)
-        elif isinstance(feature, OutputFeature):
-            self.output_features.append(feature)
-        else:
-            raise TypeError(f"Cannot add feature of type {type(feature)}")
-
-    def remove_feature_by_key(self, key):
-        """removes a feature from domain indicated by its key
+        assert isinstance(self.inputs, Inputs)
+        return {f.key: f for f in self.inputs + self.outputs}[key]
 
-        Args:
-            key (str): feature key
-
-        Raises:
-            KeyError: when the key is not found in the domain
-            ValueError: when more than one feature with key is found
-        """
-        if (self.experiments is not None) or (self.candidates is not None):
-            raise ValueError(
-                f"Feature {key} cannot be removed as experiments/candidates are already set."
-            )
-        input_count = len([f for f in self.input_features if f.key == key])
-        output_count = len([f for f in self.output_features if f.key == key])
-        if input_count == 0 and output_count == 0:
-            raise KeyError(f"no feature with key {key} found")
-        if input_count + output_count > 1:
-            raise ValueError(f"more than one feature with key {key} found")
-        if input_count > 0:
-            self.input_features = [f for f in self.input_features if f.key != key]
-        if output_count > 0:
-            self.output_features = [f for f in self.output_features if f.key != key]
-
-    def get_categorical_combinations(
-        self, include: Feature = InputFeature, exclude: Feature = None
-    ):
-        """get a list of tuples pairing the feature keys with a list of valid categories
+    # TODO: tidy this up
+    def get_nchoosek_combinations(self, exhaustive: bool = False):  # noqa: C901
+        """get all possible NChooseK combinations
 
         Args:
-            include (Feature, optional): Features to be included. Defaults to InputFeature.
-            exclude (Feature, optional): Features to be excluded, e.g. subclasses of the included features. Defaults to None.
-
-        Returns:
-            List[(str, List[str])]: Returns a list of tuples pairing the feature keys with a list of valid categories (str)
-        """
-        features = [
-            f
-            for f in self.get_features(includes=include, excludes=exclude)
-            if isinstance(f, CategoricalInputFeature) and not f.is_fixed()
-        ]
-        list_of_lists = [
-            [(f.key, cat) for cat in f.get_allowed_categories()] for f in features
-        ]
-        return list(itertools.product(*list_of_lists))
-
-    # getting list of fixed values
-    def get_nchoosek_combinations(self):
-        """get all possible NChooseK combinations
+            exhaustive (bool, optional): if True all combinations are returned. Defaults to False.
 
         Returns:
             Tuple(used_features_list, unused_features_list): used_features_list is a list of lists containing features used in each NChooseK combination.
-             unused_features_list is a list of lists containing features unused in each NChooseK combination.
+                unused_features_list is a list of lists containing features unused in each NChooseK combination.
         """
 
-        if len(self.get_constraints(NChooseKConstraint)) == 0:
-            used_continuous_features = self.get_feature_keys(ContinuousInputFeature)
+        if len(self.constraints.get(NChooseKConstraint)) == 0:
+            used_continuous_features = self.get_feature_keys(ContinuousInput)
             return used_continuous_features, []
 
         used_features_list_all = []
 
         # loops through each NChooseK constraint
-        for con in self.get_constraints(NChooseKConstraint):
+        for con in self.constraints.get(NChooseKConstraint):
+            assert isinstance(con, NChooseKConstraint)
             used_features_list = []
 
-            for n in range(con.min_count, con.max_count + 1):
-                used_features_list.extend(itertools.combinations(con.features, n))
+            if exhaustive:
+                for n in range(con.min_count, con.max_count + 1):
+                    used_features_list.extend(itertools.combinations(con.features, n))
 
-            if con.none_also_valid:
-                used_features_list.append(tuple([]))
+                if con.none_also_valid:
+                    used_features_list.append(tuple([]))
+            else:
+                used_features_list.extend(
+                    itertools.combinations(con.features, con.max_count)
+                )
 
             used_features_list_all.append(used_features_list)
 
         used_features_list_all = list(
             itertools.product(*used_features_list_all)
         )  # product between NChooseK constraints
 
         # format into a list of used features
         used_features_list_formatted = []
         for used_features_list in used_features_list_all:
-
             used_features_list_flattened = [
                 item for sublist in used_features_list for item in sublist
             ]
             used_features_list_formatted.append(list(set(used_features_list_flattened)))
 
         # sort lists
         used_features_list_sorted = []
@@ -402,15 +340,16 @@
 
         # remove combinations not fulfilling constraints
         used_features_list_final = []
         for combo in used_features_list_no_dup:
             fulfil_constraints = (
                 []
             )  # list of bools tracking if constraints are fulfilled
-            for con in self.get_constraints(NChooseKConstraint):
+            for con in self.constraints.get(NChooseKConstraint):
+                assert isinstance(con, NChooseKConstraint)
                 count = 0  # count of features in combo that are in con.features
                 for f in combo:
                     if f in con.features:
                         count += 1
                 if count >= con.min_count and count <= con.max_count:
                     fulfil_constraints.append(True)
                 elif count == 0 and con.none_also_valid:
@@ -420,15 +359,16 @@
             if np.all(fulfil_constraints):
                 used_features_list_final.append(combo)
 
         # print(f"violators dropped: {len(used_features_list_no_dup)-len(used_features_list_final)}")
 
         # features unused
         features_in_cc = []
-        for con in self.get_constraints(NChooseKConstraint):
+        for con in self.constraints.get(NChooseKConstraint):
+            assert isinstance(con, NChooseKConstraint)
             features_in_cc.extend(con.features)
         features_in_cc = list(set(features_in_cc))
         features_in_cc.sort()
         unused_features_list = []
         for used_features in used_features_list_final:
             unused_features_list.append(
                 [f_key for f_key in features_in_cc if f_key not in used_features]
@@ -439,149 +379,25 @@
         # unused_features_list2 = []
         # for used, unused in zip(used_features_list_final,unused_features_list):
         #     if len(used) == 3:
         #         used_features_list_final2.append(used), unused_features_list2.append(unused)
 
         return used_features_list_final, unused_features_list
 
-    def is_fulfilled(self, experiments: pd.DataFrame) -> pd.Series:
-        """Method to check if all constraints are fulfilled on all rows of the provided dataframe
-
-        Args:
-            df_data (pd.DataFrame): Dataframe with data, the constraint validity should be tested on
-
-        Returns:
-            Boolean: True if all constraints are fulfilled for all rows, false if not
-        """
-        if len(self.constraints) == 0:
-            return pd.Series([True] * len(experiments), index=experiments.index)
-        return pd.concat(
-            [c.satisfied(experiments) for c in self.constraints], axis=1
-        ).all(axis=1)
-
-    # TODO: needs to be tested
-    def evaluate_constraints(self, experiments: pd.DataFrame) -> pd.DataFrame:
-        return pd.concat([c(experiments) for c in self.constraints], axis=1)
-
-    # TODO: needs to be tested
-    def evaluate_desirabilities(self, experiments: pd.DataFrame) -> pd.DataFrame:
-        return pd.concat(
-            [
-                feat.desirability_function(experiments[feat.name])
-                for feat in self.get_features(ContinuousOutputFeature)
-            ],
-            axis=1,
-        )
-
-    def preprocess_experiments_one_valid_output(
-        self,
-        output_feature_key: str,
-        experiments: Optional[pd.DataFrame] = None,
-    ) -> pd.DataFrame:
-        """Method to get a dataframe where non-valid entries of the provided output feature are removed
-
-        Args:
-            experiments (pd.DataFrame): Dataframe with experimental data
-            output_feature_key (str): The feature based on which non-valid entries rows are removed
-
-        Returns:
-            pd.DataFrame: Dataframe with all experiments where only valid entries of the specific feature are included
-        """
-        if experiments is None:
-            if self.experiments is not None:
-                experiments = self.experiments
-            else:
-                return None
-        clean_exp = experiments.loc[
-            (experiments["valid_%s" % output_feature_key] == 1)
-            & (experiments[output_feature_key].notna())
-        ]
-        # clean_exp = clean_exp.dropna()
-
-        return clean_exp
-
-    def preprocess_experiments_all_valid_outputs(
-        self,
-        experiments: Optional[pd.DataFrame] = None,
-        output_feature_keys: Optional[List] = None,
-    ) -> pd.DataFrame:
-        """Method to get a dataframe where non-valid entries of all output feature are removed
-
-        Args:
-            experiments (pd.DataFrame): Dataframe with experimental data
-            output_feature_keys (Optional[List], optional): List of output feature keys which should be considered for removal of invalid values. Defaults to None.
-
-        Returns:
-            pd.DataFrame: Dataframe with all experiments where only valid entries of the selected features are included
-        """
-        if experiments is None:
-            if self.experiments is not None:
-                experiments = self.experiments
-            else:
-                return None
-        if (output_feature_keys is None) or (len(output_feature_keys) == 0):
-            output_feature_keys = self.get_feature_keys(OutputFeature)
-        else:
-            for key in output_feature_keys:
-                feat = self.get_feature(key)
-                assert isinstance(
-                    feat, OutputFeature
-                ), f"feat {key} is not an OutputFeature"
-
-        clean_exp = experiments.query(
-            " & ".join(["(`valid_%s` > 0)" % key for key in output_feature_keys])
-        )
-        clean_exp = clean_exp.dropna(subset=output_feature_keys)
-
-        return clean_exp
-
-    def preprocess_experiments_any_valid_output(
-        self, experiments: Optional[pd.DataFrame] = None
-    ) -> pd.DataFrame:
-        """Method to get a dataframe where at least one output feature has a valid entry
-
-        Args:
-            experiments (pd.DataFrame): Dataframe with experimental data
-
-        Returns:
-            pd.DataFrame: Dataframe with all experiments where at least one output feature has a valid entry
-        """
-        if experiments is None:
-            if self.experiments is not None:
-                experiments = self.experiments
-            else:
-                return None
-
-        output_feature_keys = self.get_feature_keys(OutputFeature)
-
-        # clean_exp = experiments.query(" or ".join(["(valid_%s > 0)" % key for key in output_feature_keys]))
-        # clean_exp = clean_exp.query(" or ".join(["%s.notna()" % key for key in output_feature_keys]))
-
-        clean_exp = experiments.query(
-            " or ".join(
-                [
-                    "((`valid_%s` >0) & `%s`.notna())" % (key, key)
-                    for key in output_feature_keys
-                ]
-            )
-        )
-
-        return clean_exp
-
     def coerce_invalids(self, experiments: pd.DataFrame) -> pd.DataFrame:
         """Coerces all invalid output measurements to np.nan
 
         Args:
             experiments (pd.DataFrame): Dataframe containing experimental data
 
         Returns:
             pd.DataFrame: coerced dataframe
         """
         # coerce invalid to nan
-        for feat in self.get_feature_keys(OutputFeature):
+        for feat in self.get_feature_keys(Output):
             experiments.loc[experiments[f"valid_{feat}"] == 0, feat] = np.nan
         return experiments
 
     def aggregate_by_duplicates(
         self, experiments: pd.DataFrame, prec: int, delimiter: str = "-"
     ) -> Tuple[pd.DataFrame, list]:
         """Aggregate the dataframe by duplicate experiments
@@ -595,44 +411,49 @@
             prec (int): Precision of the rounding of the continuous input features
             delimiter (str, optional): Delimiter used when combining the orig. labcodes to a new one. Defaults to "-".
 
         Returns:
             Tuple[pd.DataFrame, list]: Dataframe holding the aggregated experiments, list of lists holding the labcodes of the duplicates
         """
         # prepare the parent frame
-        experiments = self.preprocess_experiments_any_valid_output(experiments).copy()
+
+        preprocessed = self.outputs.preprocess_experiments_any_valid_output(experiments)
+        assert preprocessed is not None
+        experiments = preprocessed.copy()
         if "labcode" not in experiments.columns:
             experiments["labcode"] = [
                 str(i + 1).zfill(int(np.ceil(np.log10(experiments.shape[0]))))
                 for i in range(experiments.shape[0])
             ]
 
         # round it
-        experiments[self.get_feature_keys(ContinuousInputFeature)] = experiments[
-            self.get_feature_keys(ContinuousInputFeature)
+        experiments[self.get_feature_keys(ContinuousInput)] = experiments[
+            self.get_feature_keys(ContinuousInput)
         ].round(prec)
 
         # coerce invalid to nan
         experiments = self.coerce_invalids(experiments)
 
         # group and aggregate
-        agg = {feat: "mean" for feat in self.get_feature_keys(ContinuousOutputFeature)}
+        agg: Dict[str, Any] = {
+            feat: "mean" for feat in self.get_feature_keys(ContinuousOutput)
+        }
         agg["labcode"] = lambda x: delimiter.join(sorted(x.tolist()))
-        for feat in self.get_feature_keys(OutputFeature):
+        for feat in self.get_feature_keys(Output):
             agg[f"valid_{feat}"] = lambda x: 1
 
-        grouped = experiments.groupby(self.get_feature_keys(InputFeature))
+        grouped = experiments.groupby(self.get_feature_keys(Input))
         duplicated_labcodes = [
-            sorted(group.labcode.values.tolist())
+            sorted(group.labcode.to_numpy().tolist())
             for _, group in grouped
             if group.shape[0] > 1
         ]
 
         experiments = grouped.aggregate(agg).reset_index(drop=False)
-        for feat in self.get_feature_keys(OutputFeature):
+        for feat in self.get_feature_keys(Output):
             experiments.loc[experiments[feat].isna(), f"valid_{feat}"] = 0
 
         experiments = experiments.sort_values(by="labcode")
         experiments = experiments.reset_index(drop=True)
         return experiments, sorted(duplicated_labcodes)
 
     def validate_experiments(
@@ -649,16 +470,16 @@
             ValueError: empty dataframe
             ValueError: the column for a specific feature is missing the provided data
             ValueError: there are labcodes with null value
             ValueError: there are labcodes with nan value
             ValueError: labcodes are not unique
             ValueError: the provided columns do no match to the defined domain
             ValueError: the provided columns do no match to the defined domain
-            ValueError: inputFeature with null values
-            ValueError: inputFeature with nan values
+            ValueError: Input with null values
+            ValueError: Input with nan values
 
         Returns:
             pd.DataFrame: The provided dataframe with experimental data
         """
 
         if len(experiments) == 0:
             raise ValueError("no experiments provided (empty dataframe)")
@@ -666,231 +487,180 @@
         feature_keys = self.get_feature_keys()
         for feature_key in feature_keys:
             if feature_key not in experiments:
                 raise ValueError(f"no col in experiments for feature {feature_key}")
         # add valid_{key} cols if missing
         valid_keys = [
             f"valid_{output_feature_key}"
-            for output_feature_key in self.get_feature_keys(OutputFeature)
+            for output_feature_key in self.get_feature_keys(Output)
         ]
         for valid_key in valid_keys:
             if valid_key not in experiments:
                 experiments[valid_key] = True
         # check all cols
         expected = feature_keys + valid_keys
         cols = list(experiments.columns)
         # we allow here for a column named labcode used to identify experiments
         if "labcode" in cols:
             # test that labcodes are not na
-            if experiments.labcode.isnull().values.any():
+            if experiments.labcode.isnull().to_numpy().any():
                 raise ValueError("there are labcodes with null value")
-            if experiments.labcode.isna().values.any():
+            if experiments.labcode.isna().to_numpy().any():
                 raise ValueError("there are labcodes with nan value")
             # test that labcodes are distinct
-            if len(set(experiments.labcode.values.tolist())) != experiments.shape[0]:
+            if (
+                len(set(experiments.labcode.to_numpy().tolist()))
+                != experiments.shape[0]
+            ):
                 raise ValueError("labcodes are not unique")
             # we remove the labcode from the cols list to proceed as before
             cols.remove("labcode")
         if len(expected) != len(cols):
             raise ValueError(f"expected the following cols: `{expected}`, got `{cols}`")
         if len(set(expected + cols)) != len(cols):
             raise ValueError(f"expected the following cols: `{expected}`, got `{cols}`")
         # check values of continuous input features
-        if experiments[self.get_feature_keys(InputFeature)].isnull().values.any():
+        if experiments[self.get_feature_keys(Input)].isnull().to_numpy().any():
             raise ValueError("there are null values")
-        if experiments[self.get_feature_keys(InputFeature)].isna().values.any():
+        if experiments[self.get_feature_keys(Input)].isna().to_numpy().any():
             raise ValueError("there are na values")
         # run the individual validators
-        for feat in self.get_features(InputFeature):
+        for feat in self.get_features(Input):
+            assert isinstance(feat, Input)
             feat.validate_experimental(experiments[feat.key], strict=strict)
         return experiments
 
     def describe_experiments(self, experiments: pd.DataFrame) -> pd.DataFrame:
         """Method to get a tabular overview of how many measurements and how many valid entries are included in the input data for each output feature
 
         Args:
             experiments (pd.DataFrame): Dataframe with experimental data
 
         Returns:
             pd.DataFrame: Dataframe with counts how many measurements and how many valid entries are included in the input data for each output feature
         """
         data = {}
-        for feat in self.get_feature_keys(OutputFeature):
+        for feat in self.get_feature_keys(Output):
             data[feat] = [
                 experiments.loc[experiments[feat].notna()].shape[0],
                 experiments.loc[experiments[feat].notna(), "valid_%s" % feat].sum(),
             ]
+        preprocessed = self.outputs.preprocess_experiments_all_valid_outputs(
+            experiments
+        )
+        assert preprocessed is not None
         data["all"] = [
             experiments.shape[0],
-            self.preprocess_experiments_all_valid_outputs(experiments).shape[0],
+            preprocessed.shape[0],
         ]
         return pd.DataFrame.from_dict(
             data, orient="index", columns=["measured", "valid"]
         )
 
     def validate_candidates(
-        self,
-        candidates: pd.DataFrame,
+        self, candidates: pd.DataFrame, only_inputs: bool = False, tol: float = 1e-5
     ) -> pd.DataFrame:
         """Method to check the validty of porposed candidates
 
         Args:
             candidates (pd.DataFrame): Dataframe with suggested new experiments (candidates)
+            only_inputs (bool,optional): If True, only the input columns are validated. Defaults to False.
+            tol (float,optional): tolerance parameter for constraints. A constraint is considered as not fulfilled if the violation
+                is larger than tol. Defaults to 1e-6.
 
         Raises:
             ValueError: when a column is missing for a defined input feature
             ValueError: when a column is missing for a defined output feature
             ValueError: when a non-numerical value is proposed
             ValueError: when the constraints are not fulfilled
             ValueError: when an additional column is found
 
         Returns:
             pd.DataFrame: dataframe with suggested experiments (candidates)
         """
         # check that each input feature has a col and is valid in itself
-        for feat in self.get_features(InputFeature):
-            if feat.key not in candidates:
-                raise ValueError(f"no col for input feature `{feat.key}`")
-            feat.validate_candidental(candidates[feat.key])
-        # for each output feature
-        for key in self.get_feature_keys(
-            OutputFeature, excludes=[ContinuousOutputFeature_woDesFunc]
-        ):
+        assert isinstance(self.inputs, Inputs)
+        self.inputs.validate_inputs(candidates)
+        # check if all constraints are fulfilled
+        if not self.constraints.is_fulfilled(candidates, tol=tol).all():
+            raise ValueError(f"Constraints not fulfilled: {candidates}")
+        # for each continuous output feature with an attached objective object
+        if not only_inputs:
+            assert isinstance(self.outputs, Outputs)
+
+            cols = list(
+                itertools.chain.from_iterable(
+                    [
+                        [f"{key}_pred", f"{key}_sd", f"{key}_des"]
+                        for key in self.outputs.get_keys_by_objective(Objective)
+                    ]
+                    + [
+                        [f"{key}_pred", f"{key}_sd"]
+                        for key in self.outputs.get_keys_by_objective(
+                            excludes=Objective, includes=None  # type: ignore
+                        )
+                    ]
+                )
+            )
+
             # check that pred, sd, and des cols are specified and numerical
-            for col in [f"{key}_pred", f"{key}_sd", f"{key}_des"]:
+            for col in cols:
                 if col not in candidates:
-                    raise ValueError("missing column {col}")
+                    raise ValueError(f"missing column {col}")
                 if (not is_numeric(candidates[col])) and (
-                    not candidates[col].isnull().values.all()
+                    not candidates[col].isnull().to_numpy().all()
                 ):
-                    raise ValueError(
-                        f"not all values of output feature `{key}` are numerical"
-                    )
-        # check if all constraints are fulfilled
-        if self.is_fulfilled(candidates).all() == False:
-            raise ValueError("Constraints not fulfilled.")
-        # validate no additional cols exist
-        if_count = len(self.get_features(InputFeature))
-        of_count = len(
-            self.get_features(
-                OutputFeature, excludes=[ContinuousOutputFeature_woDesFunc]
-            )
-        )
-        # input features, prediction, standard deviation and reward for each output feature, 3 additional usefull infos: reward, aquisition function, strategy
-        if len(candidates.columns) != if_count + 3 * of_count:
-            raise ValueError("additional columns found")
+                    raise ValueError(f"not all values of column `{col}` are numerical")
+
+            # validate no additional cols exist
+            if_count = len(self.get_features(Input))
+            of_count = len(self.outputs.get_by_objective(includes=Objective))
+            of_count_w = len(self.outputs.get_by_objective(excludes=Objective, includes=None))  # type: ignore
+            # input features, prediction, standard deviation and reward for each output feature, 3 additional usefull infos: reward, aquisition function, strategy
+            if len(candidates.columns) != if_count + 3 * of_count + 2 * of_count_w:
+                raise ValueError("additional columns found")
         return candidates
 
     @property
     def experiment_column_names(self):
         """the columns in the experimental dataframe
 
         Returns:
             List[str]: List of columns in the experiment dataframe (output feature keys + valid_output feature keys)
         """
         return self.get_feature_keys() + [
             f"valid_{output_feature_key}"
-            for output_feature_key in self.get_feature_keys(OutputFeature)
+            for output_feature_key in self.get_feature_keys(Output)
         ]
 
     @property
     def candidate_column_names(self):
         """the columns in the candidate dataframe
 
         Returns:
             List[str]: List of columns in the candidate dataframe (input feature keys + input feature keys_pred, input feature keys_sd, input feature keys_des)
         """
+        assert isinstance(self.outputs, Outputs)
         return (
-            self.get_feature_keys(InputFeature)
+            self.get_feature_keys(Input)
             + [
                 f"{output_feature_key}_pred"
-                for output_feature_key in self.get_feature_keys(
-                    OutputFeature, excludes=[ContinuousOutputFeature_woDesFunc]
-                )
+                for output_feature_key in self.outputs.get_keys_by_objective(Objective)
             ]
             + [
                 f"{output_feature_key}_sd"
-                for output_feature_key in self.get_feature_keys(
-                    OutputFeature, excludes=[ContinuousOutputFeature_woDesFunc]
-                )
+                for output_feature_key in self.outputs.get_keys_by_objective(Objective)
             ]
             + [
                 f"{output_feature_key}_des"
-                for output_feature_key in self.get_feature_keys(
-                    OutputFeature, excludes=[ContinuousOutputFeature_woDesFunc]
-                )
+                for output_feature_key in self.outputs.get_keys_by_objective(Objective)
             ]
         )
 
-    def add_candidates(self, candidates: pd.DataFrame):
-        candidates = self.validate_candidates(candidates)
-        if candidates is None:
-            self.candidates = candidates
-        else:
-            self._candidates = pd.concat(
-                (self._candidates, candidates), ignore_index=True
-            )
-
-    def add_experiments(self, experiments: pd.DataFrame):
-        experiments = self.validate_experiments(experiments)
-        if experiments is None:
-            self.experiments = None
-        else:
-            self.experiments = pd.concat(
-                (self.experiments, experiments), ignore_index=True
-            )
-
-
-def get_subdomain(
-    domain: Domain,
-    feature_keys: List,
-):
-    """removes all features not defined as argument creating a subdomain of the provided domain
-
-    Args:
-        domain (Domain): the original domain wherefrom a subdomain should be created
-        feature_keys (List): List of features that shall be included in the subdomain
-
-    Raises:
-        Assert: when in total less than 2 features are provided
-        ValueError: when a provided feature key is not present in the provided domain
-        Assert: when no output feature is provided
-        Assert: when no input feature is provided
-        ValueError: _description_
-
-    Returns:
-        Domain: A new domain containing only parts of the original domain
-    """
-    assert len(feature_keys) >= 2, "At least two features have to be provided."
-    output_feature_keys = []
-    input_feature_keys = []
-    subdomain = deepcopy(domain)
-    for key in feature_keys:
-        try:
-            feat = domain.get_feature(key)
-        except KeyError:
-            raise ValueError(f"Feature {key} not present in domain.")
-        if isinstance(feat, InputFeature):
-            input_feature_keys.append(key)
-        else:
-            output_feature_keys.append(key)
-    assert (
-        len(output_feature_keys) > 0
-    ), "At least one output feature has to be provided."
-    assert len(input_feature_keys) > 0, "At least one input feature has to be provided."
-    # loop over constraints and make sure that all features used in constraints are in the input_feature_keys
-    for c in domain.constraints:
-        for key in c.features:
-            if key not in input_feature_keys:
-                raise ValueError(
-                    f"Removed input feature {key} is used in a constraint."
-                )
-
-    for key in set(domain.get_feature_keys(Feature)) - set(feature_keys):
-        subdomain.remove_feature_by_key(key)
-    return subdomain
-
-
-class DomainError(Exception):
-    """A class defining a specific domain error"""
-
-    pass
+    def _set_constraints_unvalidated(
+        self, constraints: Union[Sequence[AnyConstraint], Constraints]
+    ):
+        """Hack for reduce_domain"""
+        self.constraints = Constraints(constraints=[])
+        if isinstance(constraints, Constraints):
+            constraints = constraints.constraints
+        self.constraints.constraints = constraints
```

### Comparing `bofire-0.0.3/bofire/domain/features.py` & `bofire-0.0.4/bofire/data_models/domain/features.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,843 +1,666 @@
-from abc import abstractmethod
-from os import name
-from typing import Dict, List, Optional, Union
+from __future__ import annotations
+
+import itertools
+import warnings
+from typing import Dict, List, Literal, Optional, Sequence, Tuple, Type, Union, cast
 
-import matplotlib.pyplot as plt
 import numpy as np
 import pandas as pd
-from pydantic import Field, validator
-from pydantic.class_validators import root_validator
-from pydantic.types import conlist, conset
-
-from bofire.domain.desirability_functions import (
-    DesirabilityFunction,
-    MaxIdentityDesirabilityFunction,
-    NoDesirabilityFunction,
-)
-from bofire.domain.util import KeyModel, is_numeric, name2key
+from pydantic import Field, validate_arguments
+from scipy.stats.qmc import LatinHypercube, Sobol
 
+from bofire.data_models.base import BaseModel, filter_by_attribute, filter_by_class
+from bofire.data_models.enum import CategoricalEncodingEnum, SamplingMethodEnum
+from bofire.data_models.features.api import (
+    _CAT_SEP,
+    AnyFeature,
+    AnyInput,
+    AnyOutput,
+    CategoricalDescriptorInput,
+    CategoricalInput,
+    ContinuousInput,
+    ContinuousOutput,
+    DiscreteInput,
+    Input,
+    Output,
+    TInputTransformSpecs,
+)
+from bofire.data_models.objectives.api import AbstractObjective, Objective
 
-class Feature(KeyModel):
-    """The base class for all features."""
+FeatureSequence = Union[List[AnyFeature], Tuple[AnyFeature]]
 
-    def __lt__(self, other) -> bool:
-        """
-        Method to compare two models to get them in the desired order.
-        Return True if other is larger than self, else False. (see FEATURE_ORDER)
 
-        Args:
-            other: The other class to compare to self
+class Features(BaseModel):
+    """Container of features, both input and output features are allowed.
 
-        Returns:
-            bool: True if the other class is larger than self, else False
-        """
-        order_self = FEATURE_ORDER[type(self)]
-        order_other = FEATURE_ORDER[type(other)]
-        if order_self == order_other:
-            return self.key < other.key
-        else:
-            return order_self < order_other
+    Attributes:
+        features (List(Features)): list of the features.
+    """
 
-    def to_config(self) -> Dict:
-        """Generate serialized version of the feature.
+    type: Literal["Features"] = "Features"
+    features: FeatureSequence = Field(default_factory=lambda: [])
 
-        Returns:
-            Dict: Serialized version of the feature as dictionary.
-        """
-        return {
-            "type": self.__class__.__name__,
-            **self.dict(),
-        }
+    def __iter__(self):
+        return iter(self.features)
 
-    @staticmethod
-    def from_config(config: Dict) -> "DesirabilityFunction":
-        """Generate desirability function out of serialized version.
+    def __len__(self):
+        return len(self.features)
 
-        Args:
-            config (Dict): Serialized version of a desirability function
+    def __getitem__(self, i):
+        return self.features[i]
 
-        Returns:
-            DesirabilityFunction: Instaniated desirability function of the type specified in the `config`.
-        """
-        input_mapper = {
-            "ContinuousInputFeature": ContinuousInputFeature,
-            "DiscreteInputFeature": DiscreteInputFeature,
-            "CategoricalInputFeature": CategoricalInputFeature,
-            "CategoricalDescriptorInputFeature": CategoricalDescriptorInputFeature,
-            "ContinuousDescriptorInputFeature": ContinuousDescriptorInputFeature,
-        }
-        output_mapper = {
-            "ContinuousOutputFeature_woDesFunc": ContinuousOutputFeature_woDesFunc,
-            "ContinuousOutputFeature": ContinuousOutputFeature,
-        }
-        if config["type"] in input_mapper.keys():
-            return input_mapper[config["type"]](**config)
+    def __add__(self, other: Union[Sequence[AnyFeature], Features]):
+        if isinstance(other, Features):
+            other_feature_seq = other.features
         else:
-            d = DesirabilityFunction.from_config(config=config["desirability_function"])
-            return output_mapper[config["type"]](
-                key=config["key"], desirability_function=d
-            )
-
-
-class InputFeature(Feature):
-    """Base class for all input features."""
-
-    @abstractmethod
-    def is_fixed() -> bool:
-        """Indicates if a variable is set to a fixed value.
-
-        Returns:
-            bool: True if fixed, els False.
-        """
-        pass
-
-    @abstractmethod
-    def fixed_value() -> Union[None, str, float]:
-        """Method to return the fixed value in case of a fixed feature.
+            other_feature_seq = other
+        new_feature_seq = list(itertools.chain(self.features, other_feature_seq))
 
-        Returns:
-            Union[None,str,float]: None in case the feature is not fixed, else the fixed value.
-        """
-        pass
+        def is_feats_of_type(feats, ftype_collection, ftype_element):
+            return isinstance(feats, ftype_collection) or (
+                not isinstance(feats, Features)
+                and (len(feats) > 0 and isinstance(feats[0], ftype_element))
+            )
 
-    @abstractmethod
-    def validate_experimental(
-        self, values: pd.Series, strict: bool = False
-    ) -> pd.Series:
-        """Abstract method to validate the experimental dataFrame
+        def is_infeats(feats):
+            return is_feats_of_type(feats, Inputs, Input)
 
-        Args:
-            values (pd.Series): A dataFrame with experiments
-            strict (bool, optional): Boolean to distinguish if the occurence of fixed features in the dataset should be considered or not. Defaults to False.
+        def is_outfeats(feats):
+            return is_feats_of_type(feats, Outputs, Output)
 
-        Returns:
-            pd.Series: The passed dataFrame with experiments
-        """
-        pass
+        if is_infeats(self) and is_infeats(other):
+            return Inputs(features=cast(Tuple[AnyInput, ...], new_feature_seq))
+        if is_outfeats(self) and is_outfeats(other):
+            return Outputs(features=cast(Tuple[AnyOutput, ...], new_feature_seq))
+        return Features(features=new_feature_seq)
 
-    @abstractmethod
-    def validate_candidental(self, values: pd.Series) -> pd.Series:
-        """Abstract method to validate the suggested candidates
+    def get_by_key(self, key: str) -> AnyFeature:
+        """Get a feature by its key.
 
         Args:
-            values (pd.Series): A dataFrame with candidates
+            key (str): Feature key of the feature of interest
 
         Returns:
-            pd.Series: The passed dataFrame with candidates
+            Feature: Feature of interest
         """
-        pass
+        return {f.key: f for f in self.features}[key]
 
-    @abstractmethod
-    def sample(self, n: int) -> pd.Series:
-        """Sample a series of allowed values.
+    def get_by_keys(self, keys: Sequence[str]) -> Features:
+        """Get features of the domain specified by its keys.
 
         Args:
-            n (int): Number of samples
-
-        Returns:
-            pd.Series: Sampled values.
-        """
-        pass
-
-
-class OutputFeature(Feature):
-    """Base class for all output features.
-
-    Attributes:
-        desirability_function (Desirability_function, optional): Desirability function of
-            the feature indicating in which direction it should be optimzed. Defaults to `MaxIdentityDesirabilityFunction`.
-    """
-
-    desirability_function: Optional[DesirabilityFunction] = Field(
-        default_factory=lambda: MaxIdentityDesirabilityFunction(w=1.0)
-    )
-
-    def to_config(self) -> Dict:
-        """Generate serialized version of the feature.
+            keys (Sequence[str]): List of the keys of the features that should be
+                returned.
 
         Returns:
-            Dict: Serialized version of the feature as dictionary.
+            Features: Features object with the requested features.
         """
-        return {
-            "type": self.__class__.__name__,
-            "key": self.key,
-            "desirability_function": self.desirability_function.to_config(),
-        }
+        return self.__class__(features=sorted([self.get_by_key(key) for key in keys]))
 
-    def plot(
+    def get(
         self,
-        lower: float,
-        upper: float,
-        df_data: Optional[pd.DataFrame] = None,
-        plot_details: bool = True,
-        line_options: Optional[Dict] = None,
-        scatter_options: Optional[Dict] = None,
-        label_options: Optional[Dict] = None,
-        title_options: Optional[Dict] = None,
-    ):
-        """Plot the assigned reward function.
-
-        Args:
-            lower (float): lower bound for the plot
-            upper (float): upper bound for the plot
-            df_data (Optional[pd.DataFrame], optional): If provided, scatter also the historical data in the plot. Defaults to None.
-        """
-        line_options = line_options or {}
-        scatter_options = scatter_options or {}
-        label_options = label_options or {}
-        title_options = title_options or {}
-
-        line_options["color"] = line_options.get("color", "black")
-        scatter_options["color"] = scatter_options.get("color", "red")
-
-        x = np.linspace(lower, upper, 5000)
-        reward = self.desirability_function.__call__(x)
-        fig, ax = plt.subplots()
-        ax.plot(x, reward, **line_options)
-        # TODO: validate dataframe
-        if df_data is not None:
-            x_data = df_data.loc[df_data[self.key].notna(), self.key].values
-            ax.scatter(
-                x_data,
-                self.desirability_function.__call__(x_data),
-                **scatter_options,
-            )
-        ax.set_title("Desirability %s" % self.key, **title_options)
-        ax.set_ylabel("Desirability", **label_options)
-        ax.set_xlabel(self.key, **label_options)
-        if plot_details:
-            ax = self.desirability_function.plot_details(ax=ax)
-        return fig, ax
-
-    def __str__(self) -> str:
-        return self.desirability_function.__class__.__name__
-
-
-class NumericalInputFeature(InputFeature):
-    """Abstracht base class for all numerical (ordinal) input features."""
-
-    def is_fixed(self):
-        """Method to check if the feature is fixed
-
-        Returns:
-            Boolean: True when the feature is fixed, false otherwise.
-        """
-        return self.lower_bound == self.upper_bound
-
-    def fixed_value(self):
-        """Method to get the value to which the feature is fixed
-
-        Returns:
-            Float: Return the feature value or None if the feature is not fixed.
-        """
-        if self.is_fixed():
-            return self.lower_bound
-        else:
-            return None
-
-    def validate_experimental(self, values: pd.Series, strict=False) -> pd.Series:
-        """Method to validate the experimental dataFrame
-
-        Args:
-            values (pd.Series): A dataFrame with experiments
-            strict (bool, optional): Boolean to distinguish if the occurence of fixed features in the dataset should be considered or not. Defaults to False.
-
-        Raises:
-            ValueError: when a value is not numerical
-            ValueError: when there is no variation in a feature provided by the experimental data
-
-        Returns:
-            pd.Series: A dataFrame with experiments
-        """
-        if not is_numeric(values):
-            raise ValueError(
-                f"not all values of input feature `{self.key}` are numerical"
-            )
-        if strict:
-            lower, upper = self.get_real_feature_bounds(values)
-            if lower == upper:
-                raise ValueError(
-                    f"No variation present or planned for feature {self.key}. Remove it."
+        includes: Union[Type, List[Type]] = AnyFeature,
+        excludes: Union[Type, List[Type]] = None,
+        exact: bool = False,
+    ) -> Features:
+        """get features of the domain
+
+        Args:
+            includes (Union[Type, List[Type]], optional): Feature class or list of specific feature classes to be returned. Defaults to Feature.
+            excludes (Union[Type, List[Type]], optional): Feature class or list of specific feature classes to be excluded from the return. Defaults to None.
+            exact (bool, optional): Boolean to distinguish if only the exact class listed in includes and no subclasses inherenting from this class shall be returned. Defaults to False.
+            by_attribute (str, optional): If set it is filtered by the attribute specified in by `by_attribute`. Defaults to None.
+
+        Returns:
+            List[Feature]: List of features in the domain fitting to the passed requirements.
+        """
+        return self.__class__(
+            features=sorted(
+                filter_by_class(
+                    self.features,
+                    includes=includes,
+                    excludes=excludes,
+                    exact=exact,
                 )
-        return values
-
-    def validate_candidental(self, values: pd.Series) -> pd.Series:
-        """Validate the suggested candidates for the feature.
-
-        Args:
-            values (pd.Series): suggested candidates for the feature
-
-        Raises:
-            ValueError: Error is raised when one of the values is not numerical.
-
-        Returns:
-            pd.Series: the original provided candidates
-        """
-        if not is_numeric(values):
-            raise ValueError(
-                f"not all values of input feature `{self.key}` are numerical"
             )
-        return values
+        )
 
-    def get_real_feature_bounds(self, values: pd.Series):
-        """Method to extract the feature boundaries from the provided experimental data
+    def get_keys(
+        self,
+        includes: Union[Type, List[Type]] = AnyFeature,
+        excludes: Union[Type, List[Type]] = None,
+        exact: bool = False,
+    ) -> List[str]:
+        """Method to get feature keys of the domain
 
         Args:
-            values (pd.Series): Experimental data
+            includes (Union[Type, List[Type]], optional): Feature class or list of specific feature classes to be returned. Defaults to Feature.
+            excludes (Union[Type, List[Type]], optional): Feature class or list of specific feature classes to be excluded from the return. Defaults to None.
+            exact (bool, optional): Boolean to distinguish if only the exact class listed in includes and no subclasses inherenting from this class shall be returned. Defaults to False.
 
         Returns:
-            (float, float): Returns lower and upper bound based on the passed data
+            List[str]: List of feature keys fitting to the passed requirements.
         """
-        lower = min(self.lower_bound, values.min())
-        upper = max(self.upper_bound, values.max())
-        return lower, upper
+        return [
+            f.key
+            for f in self.get(
+                includes=includes,
+                excludes=excludes,
+                exact=exact,
+            )
+        ]
 
 
-class ContinuousInputFeature(NumericalInputFeature):
-    """Base class for all continuous input features.
+class Inputs(Features):
+    """Container of input features, only input features are allowed.
 
     Attributes:
-        lower_bound (float): Lower bound of the feature in the optimization.
-        upper_bound (float): Upper bound of the feature in the optimization.
+        features (List(Inputs)): list of the features.
     """
 
-    lower_bound: float
-    upper_bound: float
-
-    @root_validator(pre=False)
-    def validate_lower_upper(cls, values):
-        """Validates that the lower bound is lower than the upper bound
-
-        Args:
-            values (Dict): Dictionary with attributes key, lower and upper bound
+    type: Literal["Inputs"] = "Inputs"
+    features: Sequence[AnyInput] = Field(default_factory=lambda: [])
 
-        Raises:
-            ValueError: when the lower bound is higher than the upper bound
+    def get_fixed(self) -> "Inputs":
+        """Gets all features in `self` that are fixed and returns them as new `Inputs` object.
 
         Returns:
-            Dict: The attributes as dictionary
+            Inputs: Input features object containing only fixed features.
         """
-        if values["lower_bound"] > values["upper_bound"]:
-            raise ValueError(
-                f'lower bound must be <= upper bound, got {values["lower_bound"]} > {values["upper_bound"]}'
-            )
-        return values
+        return Inputs(features=[feat for feat in self if feat.is_fixed()])  # type: ignore
 
-    def validate_candidental(self, values: pd.Series) -> pd.Series:
-        """Method to validate the suggested candidates
-
-        Args:
-            values (pd.Series): A dataFrame with candidates
-
-        Raises:
-            ValueError: when non numerical values are passed
-            ValueError: when values are larger than the upper bound of the feature
-            ValueError: when values are lower than the lower bound of the feature
+    def get_free(self) -> "Inputs":
+        """Gets all features in `self` that are not fixed and returns them as new `Inputs` object.
 
         Returns:
-            pd.Series: The passed dataFrame with candidates
-        """
-        noise = 10e-8
-        super().validate_candidental(values)
-        if (values < self.lower_bound - noise).any():
-            raise ValueError(
-                f"not all values of input feature `{self.key}`are larger than lower bound `{self.lower_bound}` "
-            )
-        if (values > self.upper_bound + noise).any():
-            raise ValueError(
-                f"not all values of input feature `{self.key}`are smaller than upper bound `{self.upper_bound}` "
-            )
-        return values
-
-    def sample(self, n: int) -> pd.Series:
-        """Draw random samples from the feature.
-
-        Args:
-            n (int): number of samples.
-
-        Returns:
-            pd.Series: drawn samples.
-        """
-        return pd.Series(
-            name=self.key,
-            data=np.random.uniform(self.lower_bound, self.upper_bound, n),
-        )
-
-    def __str__(self) -> str:
-        """Method to return a string of lower and upper bound
-
-        Returns:
-            str: String of a list with lower and upper bound
+            Inputs: Input features object containing only non-fixed features.
         """
-        return f"[{self.lower_bound},{self.upper_bound}]"
-
+        return Inputs(features=[feat for feat in self if not feat.is_fixed()])  # type: ignore
 
-class DiscreteInputFeature(NumericalInputFeature):
-    """Feature with discretized ordinal values allowed in the optimization.
-
-    Attributes:
-        key(str): key of the feature.
-        values(List[float]): the discretized allowed values during the optimization.
-    """
-
-    values: conlist(item_type=float, min_items=1)
-
-    @validator("values")
-    def validate_values_unique(cls, values):
-        """Validates that provided values are unique.
+    @validate_arguments
+    def sample(
+        self,
+        n: int = 1,
+        method: SamplingMethodEnum = SamplingMethodEnum.UNIFORM,
+    ) -> pd.DataFrame:
+        """Draw sobol samples
 
         Args:
-            values (List[float]): List of values
-
-        Raises:
-            ValueError: when values are non-unique.
+            n (int, optional): Number of samples, has to be larger than 0. Defaults to 1.
+            method (SamplingMethodEnum, optional): Method to use, implemented methods are `UNIFORM`, `SOBOL` and `LHS`.
+                Defaults to `UNIFORM`.
 
         Returns:
-            List[values]: Sorted list of values
+            pd.DataFrame: Dataframe containing the samples.
         """
-        if len(values) != len(set(values)):
-            raise ValueError("Discrete values must be unique")
-        return sorted(values)
-
-    @property
-    def lower_bound(self) -> float:
-        """Lower bound of the set of allowed values"""
-        return min(self.values)
-
-    @property
-    def upper_bound(self) -> float:
-        """Upper bound of the set of allowed values"""
-        return max(self.values)
+        if method == SamplingMethodEnum.UNIFORM:
+            return self.validate_inputs(
+                pd.concat([feat.sample(n) for feat in self.get(Input)], axis=1)  # type: ignore
+            )
+        free_features = self.get_free()
+        if method == SamplingMethodEnum.SOBOL:
+            with warnings.catch_warnings():
+                warnings.simplefilter("ignore")
+                X = Sobol(len(free_features)).random(n)
+        else:
+            X = LatinHypercube(len(free_features)).random(n)
+        res = []
+        for i, feat in enumerate(free_features):
+            if isinstance(feat, ContinuousInput):
+                x = feat.from_unit_range(X[:, i])
+            elif isinstance(feat, (DiscreteInput, CategoricalInput)):
+                if isinstance(feat, DiscreteInput):
+                    levels = feat.values
+                else:
+                    levels = feat.get_allowed_categories()
+                bins = np.linspace(0, 1, len(levels) + 1)
+                idx = np.digitize(X[:, i], bins) - 1
+                x = np.array(levels)[idx]
+            else:
+                raise (
+                    ValueError(
+                        f"Unknown input feature with key {feat.key} of type {feat.type}"
+                    )
+                )
+            res.append(pd.Series(x, name=feat.key))
+        samples = pd.concat(res, axis=1)
+        for feat in self.get_fixed():
+            samples[feat.key] = feat.fixed_value()[0]  # type: ignore
+        return self.validate_inputs(samples)[self.get_keys(Input)]
 
-    def validate_candidental(self, values: pd.Series) -> pd.Series:
-        """Method to validate the provided candidates.
+    # validate candidates, TODO rename and tidy up
+    def validate_inputs(self, inputs: pd.DataFrame) -> pd.DataFrame:
+        """Validate a pandas dataframe with input feature values.
 
         Args:
-            values (pd.Series): suggested candidates for the feature
+            inputs (pd.Dataframe): Inputs to validate.
 
         Raises:
-            ValueError: Raises error when one of the provided values is not contained in the list of allowed values.
-
-        Returns:
-            pd.Series: _uggested candidates for the feature
-        """
-        super().validate_candidental(values)
-        if not np.isin(values.values, np.array(self.values)).all():
-            raise ValueError(
-                f"Not allowed values in candidates for feature {self.key}."
-            )
-        return values
-
-    def sample(self, n: int) -> pd.Series:
-        """Draw random samples from the feature.
-
-        Args:
-            n (int): number of samples.
+            ValueError: Raises a Valueerror if a feature based validation raises an exception.
 
         Returns:
-            pd.Series: drawn samples.
+            pd.Dataframe: Validated dataframe
         """
-        return pd.Series(name=self.key, data=np.random.choice(self.values, n))
+        for feature in self:
+            if feature.key not in inputs:
+                raise ValueError(f"no col for input feature `{feature.key}`")
+            feature.validate_candidental(inputs[feature.key])  # type: ignore
+        return inputs
 
+    def validate_experiments(
+        self, experiments: pd.DataFrame, strict=False
+    ) -> pd.DataFrame:
+        for feature in self:
+            if feature.key not in experiments:
+                raise ValueError(f"no col for input feature `{feature.key}`")
+            feature.validate_experimental(experiments[feature.key], strict=strict)  # type: ignore
+        return experiments
 
-# TODO: write a Descriptor base class from which both Categorical and Continuous Descriptor are inheriting
-class ContinuousDescriptorInputFeature(ContinuousInputFeature):
-    """Class for continuous input features with descriptors
-
-    Attributes:
-        lower_bound (float): Lower bound of the feature in the optimization.
-        upper_bound (float): Upper bound of the feature in the optimization.
-        descriptors (List[str]): Names of the descriptors.
-        values (List[float]): Values of the descriptors.
-    """
-
-    descriptors: conlist(item_type=str, min_items=1)
-    values: conlist(item_type=float, min_items=1)
-
-    @validator("descriptors")
-    def descriptors_to_keys(cls, descriptors):
-        """validates the descriptor names and transforms it to valid keys
+    def get_categorical_combinations(
+        self,
+        include: Union[Type, List[Type]] = Input,
+        exclude: Union[Type, List[Type]] = None,
+    ):
+        """get a list of tuples pairing the feature keys with a list of valid categories
 
         Args:
-            descriptors (List[str]): List of descriptor names
+            include (Feature, optional): Features to be included. Defaults to Input.
+            exclude (Feature, optional): Features to be excluded, e.g. subclasses of the included features. Defaults to None.
 
         Returns:
-            List[str]: List of valid keys
+            List[(str, List[str])]: Returns a list of tuples pairing the feature keys with a list of valid categories (str)
         """
-        return [name2key(name) for name in descriptors]
+        features = [
+            f
+            for f in self.get(includes=include, excludes=exclude)
+            if (isinstance(f, CategoricalInput) and not f.is_fixed())
+        ]
+        list_of_lists = [
+            [(f.key, cat) for cat in f.get_allowed_categories()] for f in features
+        ]
+
+        discretes = [
+            f
+            for f in self.get(includes=include, excludes=exclude)
+            if (isinstance(f, DiscreteInput) and not f.is_fixed())
+        ]
+
+        list_of_lists_2 = [[(d.key, v) for v in d.values] for d in discretes]
+
+        list_of_lists = list_of_lists + list_of_lists_2
+
+        return list(itertools.product(*list_of_lists))
+
+    # transformation related methods
+    def _get_transform_info(
+        self, specs: TInputTransformSpecs
+    ) -> Tuple[Dict[str, Tuple[int]], Dict[str, Tuple[str]]]:
+        """Generates two dictionaries. The first one specifies which key is mapped to
+        which column indices when applying `transform`. The second one specifies
+        which key is mapped to which transformed keys.
+
+        Args:
+            specs (TInputTransformSpecs): Dictionary specifying which
+                input feature is transformed by which encoder.
+
+        Returns:
+            Dict[str, Tuple[int]]: Dictionary mapping feature keys to column indices.
+            Dict[str, Tuple[str]]: Dictionary mapping feature keys to transformed feature
+                keys.
+        """
+        self._validate_transform_specs(specs)
+        features2idx = {}
+        features2names = {}
+        counter = 0
+        for _, feat in enumerate(self.get()):
+            if feat.key not in specs.keys():
+                features2idx[feat.key] = (counter,)
+                features2names[feat.key] = (feat.key,)
+                counter += 1
+            elif specs[feat.key] == CategoricalEncodingEnum.ONE_HOT:
+                assert isinstance(feat, CategoricalInput)
+                features2idx[feat.key] = tuple(
+                    (np.array(range(len(feat.categories))) + counter).tolist()
+                )
+                features2names[feat.key] = tuple(
+                    [f"{feat.key}{_CAT_SEP}{c}" for c in feat.categories]
+                )
+                counter += len(feat.categories)
+            elif specs[feat.key] == CategoricalEncodingEnum.ORDINAL:
+                features2idx[feat.key] = (counter,)
+                features2names[feat.key] = (feat.key,)
+                counter += 1
+            elif specs[feat.key] == CategoricalEncodingEnum.DUMMY:
+                assert isinstance(feat, CategoricalInput)
+                features2idx[feat.key] = tuple(
+                    (np.array(range(len(feat.categories) - 1)) + counter).tolist()
+                )
+                features2names[feat.key] = tuple(
+                    [f"{feat.key}{_CAT_SEP}{c}" for c in feat.categories[1:]]
+                )
+                counter += len(feat.categories) - 1
+            elif specs[feat.key] == CategoricalEncodingEnum.DESCRIPTOR:
+                assert isinstance(feat, CategoricalDescriptorInput)
+                features2idx[feat.key] = tuple(
+                    (np.array(range(len(feat.descriptors))) + counter).tolist()
+                )
+                features2names[feat.key] = tuple(
+                    [f"{feat.key}{_CAT_SEP}{d}" for d in feat.descriptors]
+                )
+                counter += len(feat.descriptors)
+        return features2idx, features2names
+
+    def transform(
+        self, experiments: pd.DataFrame, specs: TInputTransformSpecs
+    ) -> pd.DataFrame:
+        """Transform a dataframe to the represenation specified in `specs`.
+
+        Currently only input categoricals are supported.
+
+        Args:
+            experiments (pd.DataFrame): Data dataframe to be transformed.
+            specs (TInputTransformSpecs): Dictionary specifying which
+                input feature is transformed by which encoder.
+
+        Returns:
+            pd.DataFrame: Transformed dataframe. Only input features are included.
+        """
+        specs = self._validate_transform_specs(specs)
+        transformed = []
+        for feat in self.get():
+            s = experiments[feat.key]
+            if feat.key not in specs.keys():
+                transformed.append(s)
+            elif specs[feat.key] == CategoricalEncodingEnum.ONE_HOT:
+                assert isinstance(feat, CategoricalInput)
+                transformed.append(feat.to_onehot_encoding(s))
+            elif specs[feat.key] == CategoricalEncodingEnum.ORDINAL:
+                assert isinstance(feat, CategoricalInput)
+                transformed.append(feat.to_ordinal_encoding(s))
+            elif specs[feat.key] == CategoricalEncodingEnum.DUMMY:
+                assert isinstance(feat, CategoricalInput)
+                transformed.append(feat.to_dummy_encoding(s))
+            elif specs[feat.key] == CategoricalEncodingEnum.DESCRIPTOR:
+                assert isinstance(feat, CategoricalDescriptorInput)
+                transformed.append(feat.to_descriptor_encoding(s))
+        return pd.concat(transformed, axis=1)
+
+    def inverse_transform(
+        self, experiments: pd.DataFrame, specs: TInputTransformSpecs
+    ) -> pd.DataFrame:
+        """Transform a dataframe back to the original representations.
+
+        The original applied transformation has to be provided via the specs dictionary.
+        Currently only input categoricals are supported.
+
+        Args:
+            experiments (pd.DataFrame): Transformed data dataframe.
+            specs (TInputTransformSpecs): Dictionary specifying which
+                input feature is transformed by which encoder.
+
+        Returns:
+            pd.DataFrame: Back transformed dataframe. Only input features are included.
+        """
+        self._validate_transform_specs(specs=specs)
+        transformed = []
+        for feat in self.get():
+            if isinstance(feat, DiscreteInput):
+                transformed.append(feat.from_continuous(experiments))
+            elif feat.key not in specs.keys():
+                transformed.append(experiments[feat.key])
+            elif specs[feat.key] == CategoricalEncodingEnum.ONE_HOT:
+                assert isinstance(feat, CategoricalInput)
+                transformed.append(feat.from_onehot_encoding(experiments))
+            elif specs[feat.key] == CategoricalEncodingEnum.ORDINAL:
+                assert isinstance(feat, CategoricalInput)
+                transformed.append(feat.from_ordinal_encoding(experiments[feat.key]))
+            elif specs[feat.key] == CategoricalEncodingEnum.DUMMY:
+                assert isinstance(feat, CategoricalInput)
+                transformed.append(feat.from_dummy_encoding(experiments))
+            elif specs[feat.key] == CategoricalEncodingEnum.DESCRIPTOR:
+                assert isinstance(feat, CategoricalDescriptorInput)
+                transformed.append(feat.from_descriptor_encoding(experiments))
+        return pd.concat(transformed, axis=1)
+
+    def _validate_transform_specs(self, specs: TInputTransformSpecs):
+        """Checks the validity of the transform specs .
+
+        Args:
+            specs (TInputTransformSpecs): Transform specs to be validated.
+        """
+        # first check that the keys in the specs dict are correct also correct feature keys
+        if len(set(specs.keys()) - set(self.get_keys(CategoricalInput))) > 0:
+            raise ValueError("Unknown features specified in transform specs.")
+        # next check that all values are of type CategoricalEncodingEnum
+        if not (
+            all([isinstance(enc, CategoricalEncodingEnum) for enc in specs.values()])
+        ):
+            raise ValueError("Unknown transform specified.")
+        # next check that only Categoricalwithdescriptor have the value DESCRIPTOR
+        descriptor_keys = [
+            key
+            for key, value in specs.items()
+            if value == CategoricalEncodingEnum.DESCRIPTOR
+        ]
+        if (
+            len(set(descriptor_keys) - set(self.get_keys(CategoricalDescriptorInput)))
+            > 0
+        ):
+            raise ValueError("Wrong features types assigned to DESCRIPTOR transform.")
+        return specs
 
-    @root_validator(pre=False)
-    def validate_list_lengths(cls, values):
-        """compares the length of the defined descriptors list with the provided values
+    def get_bounds(
+        self,
+        specs: TInputTransformSpecs,
+        experiments: Optional[pd.DataFrame] = None,
+    ) -> Tuple[List[float], List[float]]:
+        """Returns the boundaries of the optimization problem based on the transformations
+        defined in the  `specs` dictionary.
 
         Args:
-            values (Dict): Dictionary with all attribues
+            specs (TInputTransformSpecs): Dictionary specifying which
+                input feature is transformed by which encoder.
+            experiments (Optional[pd.DataFrame], optional): Dataframe with input features.
+                If provided the real feature bounds are returned based on both the opt.
+                feature bounds and the extreme points in the dataframe. Defaults to None,
 
         Raises:
-            ValueError: when the number of descriptors does not math the number of provided values
+            ValueError: If a feature type is not known.
+            ValueError: If no transformation is provided for a categorical feature.
 
         Returns:
-            Dict: Dict with the attributes
+            Tuple[List[float], List[float]]: list with lower bounds, list with upper bounds.
         """
-        if len(values["descriptors"]) != len(values["values"]):
-            raise ValueError(
-                'must provide same number of descriptors and values, got {len(values["descriptors"])} != {len(values["values"])}'
-            )
-        return values
+        self._validate_transform_specs(specs=specs)
 
-    def to_df(self) -> pd.DataFrame:
-        """tabular overview of the feature as DataFrame
+        lower = []
+        upper = []
 
-        Returns:
-            pd.DataFrame: tabular overview of the feature as DataFrame
-        """
-        return pd.DataFrame(
-            data=[self.values], index=[self.key], columns=self.descriptors
-        )
+        for feat in self.get():
+            l, u = feat.get_bounds(  # type: ignore
+                transform_type=specs.get(feat.key),  # type: ignore
+                values=experiments[feat.key] if experiments is not None else None,
+            )
+            lower += l
+            upper += u
+        return lower, upper
 
 
-class CategoricalInputFeature(InputFeature):
-    """Base class for all categorical input features.
+class Outputs(Features):
+    """Container of output features, only output features are allowed.
 
     Attributes:
-        categories (List[str]): Names of the categories.
-        allowed (List[bool]): List of bools indicating if a category is allowed within the optimization.
+        features (List(Outputs)): list of the features.
     """
 
-    categories: conlist(item_type=str, min_items=2)
-    allowed: Optional[conlist(item_type=bool, min_items=2)]
-
-    @validator("categories")
-    def validate_categories_unique(cls, categories):
-        """validates that categories have unique names
-
-        Args:
-            categories (List[str]): List of category names
-
-        Raises:
-            ValueError: when categories have non-unique names
-
-        Returns:
-            List[str]: List of the categories
-        """
-        categories = [name2key(name) for name in categories]
-        if len(categories) != len(set(categories)):
-            raise ValueError("categories must be unique")
-        return categories
-
-    @root_validator(pre=False)
-    def init_allowed(cls, values):
-        """validates the list of allowed/not allowed categories
+    type: Literal["Outputs"] = "Outputs"
+    features: Sequence[AnyOutput] = Field(default_factory=lambda: [])
 
-        Args:
-            values (Dict): Dictionary with attributes
-
-        Raises:
-            ValueError: when the number of allowences does not fit to the number of categories
-            ValueError: when no category is allowed
-
-        Returns:
-            Dict: Dictionary with attributes
-        """
-        if "categories" not in values or values["categories"] is None:
-            return values
-        if "allowed" not in values or values["allowed"] is None:
-            values["allowed"] = [True for _ in range(len(values["categories"]))]
-        if len(values["allowed"]) != len(values["categories"]):
-            raise ValueError("allowed must have same length as categories")
-        if sum(values["allowed"]) == 0:
-            raise ValueError("no category is allowed")
-        return values
-
-    def is_fixed(self):
-        """Returns True if there is only one allowed category.
-
-        Returns:
-            [bool]: True if there is only one allowed category
-        """
-        return sum(self.allowed) == 1
-
-    def fixed_value(self):
-        """Returns the categories to which the feature is fixed, None if the feature is not fixed
+    def get_by_objective(
+        self,
+        includes: Union[
+            List[Type[AbstractObjective]],
+            Type[AbstractObjective],
+            Type[Objective],
+        ] = Objective,
+        excludes: Union[
+            List[Type[AbstractObjective]],
+            Type[AbstractObjective],
+            None,
+        ] = None,
+        exact: bool = False,
+    ) -> "Outputs":
+        """Get output features filtered by the type of the attached objective.
+
+        Args:
+            includes (Union[List[TObjective], TObjective], optional): Objective class or list of objective classes
+                to be returned. Defaults to Objective.
+            excludes (Union[List[TObjective], TObjective, None], optional): Objective class or list of specific objective classes to be excluded from the return. Defaults to None.
+            exact (bool, optional): Boolean to distinguish if only the exact classes listed in includes and no subclasses inherenting from this class shall be returned. Defaults to False.
 
         Returns:
-            List[str]: List of categories or None
+            List[AnyOutput]: List of output features fitting to the passed requirements.
         """
-        if self.is_fixed():
-            return self.get_allowed_categories()[0]
+        if len(self.features) == 0:
+            return Outputs(features=[])
         else:
-            return None
-
-    def get_allowed_categories(self):
-        """Returns the allowed categories.
-
-        Returns:
-            list of str: The allowed categories
-        """
-        return [c for c, a in zip(self.categories, self.allowed) if a]
-
-    def validate_experimental(
-        self, values: pd.Series, strict: bool = False
-    ) -> pd.Series:
-        """Method to validate the experimental dataFrame
-
-        Args:
-            values (pd.Series): A dataFrame with experiments
-            strict (bool, optional): Boolean to distinguish if the occurence of fixed features in the dataset should be considered or not. Defaults to False.
-
-        Raises:
-            ValueError: when an entry is not in the list of allowed categories
-            ValueError: when there is no variation in a feature provided by the experimental data
-
-        Returns:
-            pd.Series: A dataFrame with experiments
-        """
-        if sum(values.isin(self.categories)) != len(values):
-            raise ValueError(
-                f"invalid values for `{self.key}`, allowed are: `{self.categories}`"
-            )
-        if strict:
-            possible_categories = self.get_possible_categories(values)
-            if len(possible_categories) != len(self.categories):
-                raise ValueError(
-                    f"Categories {list(set(self.categories)-set(possible_categories))} of feature {self.key} not used. Remove them."
+            return Outputs(
+                features=sorted(
+                    filter_by_attribute(
+                        self.get(ContinuousOutput).features,
+                        lambda of: of.objective,
+                        includes,
+                        excludes,
+                        exact,
+                    )
                 )
-        return values
-
-    def validate_candidental(self, values: pd.Series) -> pd.Series:
-        """Method to validate the suggested candidates
-
-        Args:
-            values (pd.Series): A dataFrame with candidates
-
-        Raises:
-            ValueError: when not all values for a feature are one of the allowed categories
-
-        Returns:
-            pd.Series: The passed dataFrame with candidates
-        """
-        if sum(values.isin(self.get_allowed_categories())) != len(values):
-            raise ValueError(
-                f"not all values of input feature `{self.key}` are a valid allowed category from {self.get_allowed_categories()}"
             )
-        return values
-
-    def get_forbidden_categories(self):
-        """Returns the non-allowed categories
 
-        Returns:
-            List[str]: List of the non-allowed categories
-        """
-        return list(set(self.categories) - set(self.get_allowed_categories()))
-
-    def get_possible_categories(self, values: pd.Series) -> list:
-        """Return the superset of categories that have been used in the experimental dataset and
-        that can be used in the optimization
+    def get_keys_by_objective(
+        self,
+        includes: Union[
+            List[Type[AbstractObjective]],
+            Type[AbstractObjective],
+            Type[Objective],
+        ] = Objective,
+        excludes: Union[
+            List[Type[AbstractObjective]], Type[AbstractObjective], None
+        ] = None,
+        exact: bool = False,
+    ) -> List[str]:
+        """Get keys of output features filtered by the type of the attached objective.
 
         Args:
-            values (pd.Series): Series with the values for this feature
+            includes (Union[List[TObjective], TObjective], optional): Objective class or list of objective classes
+                to be returned. Defaults to Objective.
+            excludes (Union[List[TObjective], TObjective, None], optional): Objective class or list of specific objective classes to be excluded from the return. Defaults to None.
+            exact (bool, optional): Boolean to distinguish if only the exact classes listed in includes and no subclasses inherenting from this class shall be returned. Defaults to False.
 
         Returns:
-            list: list of possible categories
+            List[str]: List of output feature keys fitting to the passed requirements.
         """
-        return sorted(
-            list(set(list(set(values.tolist())) + self.get_allowed_categories()))
-        )
+        return [f.key for f in self.get_by_objective(includes, excludes, exact)]
 
-    def sample(self, n: int) -> pd.Series:
-        """Draw random samples from the feature.
+    def __call__(
+        self, experiments: pd.DataFrame, predictions: bool = False
+    ) -> pd.DataFrame:
+        """Evaluate the objective for every feature.
 
         Args:
-            n (int): number of samples.
+            experiments (pd.DataFrame): Experiments for which the objectives should be evaluated.
+            predictions (bool, optional): If True use the prediction columns in the dataframe to calc the
+                desirabilities `f"{feat.key}_pred`.
 
         Returns:
-            pd.Series: drawn samples.
+            pd.DataFrame: Objective values for the experiments of interest.
         """
-        return pd.Series(
-            name=self.key, data=np.random.choice(self.get_allowed_categories(), n)
+        desis = pd.concat(
+            [
+                feat(experiments[f"{feat.key}_pred" if predictions else feat.key])  # type: ignore
+                for feat in self.features
+                if feat.objective is not None
+            ],
+            axis=1,
+        )
+        return desis.rename(
+            {
+                f"{feat.key}_pred" if predictions else feat.key: f"{feat.key}_des"
+                for feat in self.features
+                if feat.objective is not None
+            },
+            axis=1,
         )
 
-    def __str__(self) -> str:
-        """Returns the number of categories as str
-
-        Returns:
-            str: Number of categories
-        """
-        return f"{len(self.categories)} categories"
-
-
-class CategoricalDescriptorInputFeature(CategoricalInputFeature):
-    """Class for categorical input features with descriptors
-
-    Attributes:
-        categories (List[str]): Names of the categories.
-        allowed (List[bool]): List of bools indicating if a category is allowed within the optimization.
-        descriptors (List[str]): List of strings representing the names of the descriptors.
-        calues (List[List[float]]): List of lists representing the descriptor values.
-    """
-
-    descriptors: conlist(item_type=str, min_items=1)
-    values: conlist(item_type=conlist(item_type=float, min_items=1), min_items=1)
-
-    @validator("descriptors")
-    def validate_descriptors(cls, descriptors):
-        """validates that descriptors have unique names
-
-        Args:
-            categories (List[str]): List of descriptor names
-
-        Raises:
-            ValueError: when descriptors have non-unique names
-
-        Returns:
-            List[str]: List of the descriptors
-        """
-        descriptors = [name2key(name) for name in descriptors]
-        if len(descriptors) != len(set(descriptors)):
-            raise ValueError("descriptors must be unique")
-        return descriptors
-
-    @validator("values")
-    def validate_values(cls, v, values):
-        """validates the compatability of passed values for the descriptors and the defined categories
+    def preprocess_experiments_one_valid_output(
+        self,
+        output_feature_key: str,
+        experiments: pd.DataFrame,
+    ) -> pd.DataFrame:
+        """Method to get a dataframe where non-valid entries of the provided output feature are removed
 
         Args:
-            v (List[List[float]]): Nested list with descriptor values
-            values (Dict): Dictionary with attributes
-
-        Raises:
-            ValueError: when values have different length than categories
-            ValueError: when rows in values have different length than descriptors
-            ValueError: when a descriptor shows no variance in the data
+            experiments (pd.DataFrame): Dataframe with experimental data
+            output_feature_key (str): The feature based on which non-valid entries rows are removed
 
         Returns:
-            List[List[float]]: Nested list with descriptor values
+            pd.DataFrame: Dataframe with all experiments where only valid entries of the specific feature are included
         """
-        if len(v) != len(values["categories"]):
-            raise ValueError("values must have same length as categories")
-        for row in v:
-            if len(row) != len(values["descriptors"]):
-                raise ValueError("rows in values must have same length as descriptors")
-        a = np.array(v)
-        for i, d in enumerate(values["descriptors"]):
-            if len(set(a[:, i])) == 1:
-                raise ValueError("No variation for descriptor {d}.")
-        return v
-
-    def to_df(self):
-        """tabular overview of the feature as DataFrame
+        clean_exp = experiments.loc[
+            (experiments["valid_%s" % output_feature_key] == 1)
+            & (experiments[output_feature_key].notna())
+        ]
 
-        Returns:
-            pd.DataFrame: tabular overview of the feature as DataFrame
-        """
-        data = {cat: values for cat, values in zip(self.categories, self.values)}
-        return pd.DataFrame.from_dict(data, orient="index", columns=self.descriptors)
+        return clean_exp
 
-    def get_real_descriptor_bounds(self, values) -> pd.Series:
-        """Method to generate a dataFrame as tabular overview of lower and upper bounds of the descriptors (excluding non-allowed descriptors)
+    def preprocess_experiments_all_valid_outputs(
+        self,
+        experiments: pd.DataFrame,
+        output_feature_keys: Optional[List] = None,
+    ) -> pd.DataFrame:
+        """Method to get a dataframe where non-valid entries of all output feature are removed
 
         Args:
-            values (pd.Series): The categories present in the passed data for the considered feature
+            experiments (pd.DataFrame): Dataframe with experimental data
+            output_feature_keys (Optional[List], optional): List of output feature keys which should be considered for removal of invalid values. Defaults to None.
 
         Returns:
-            pd.Series: Tabular overview of lower and upper bounds of the descriptors
+            pd.DataFrame: Dataframe with all experiments where only valid entries of the selected features are included
         """
-        df = self.to_df().loc[self.get_possible_categories(values)]
-        data = {
-            "lower": [min(df[desc].tolist()) for desc in self.descriptors],
-            "upper": [max(df[desc].tolist()) for desc in self.descriptors],
-        }
-        return pd.DataFrame.from_dict(data, orient="index", columns=self.descriptors)
-
-    def validate_experimental(
-        self, values: pd.Series, strict: bool = False
-    ) -> pd.Series:
-        """Method to validate the experimental dataFrame
+        if (output_feature_keys is None) or (len(output_feature_keys) == 0):
+            output_feature_keys = self.get_keys(Output)
 
-        Args:
-            values (pd.Series): A dataFrame with experiments
-            strict (bool, optional): Boolean to distinguish if the occurence of fixed features in the dataset should be considered or not. Defaults to False.
+        clean_exp = experiments.query(
+            " & ".join(["(`valid_%s` > 0)" % key for key in output_feature_keys])
+        )
+        clean_exp = clean_exp.dropna(subset=output_feature_keys)
 
-        Raises:
-            ValueError: when an entry is not in the list of allowed categories
-            ValueError: when there is no variation in a feature provided by the experimental data
-            ValueError: when no variation is present or planed for a given descriptor
+        return clean_exp
 
-        Returns:
-            pd.Series: A dataFrame with experiments
-        """
-        values = super().validate_experimental(values, strict)
-        if strict:
-            bounds = self.get_real_descriptor_bounds(values)
-            for desc in self.descriptors:
-                if bounds.loc["lower", desc] == bounds.loc["upper", desc]:
-                    raise ValueError(
-                        f"No variation present or planned for descriptor {desc} for feature {self.key}. Remove the descriptor."
-                    )
-        return values
-
-    @classmethod
-    def from_df(cls, key: str, df: pd.DataFrame):
-        """Creates a feature from a dataframe
+    def preprocess_experiments_any_valid_output(
+        self, experiments: pd.DataFrame
+    ) -> pd.DataFrame:
+        """Method to get a dataframe where at least one output feature has a valid entry
 
         Args:
-            key (str): The name of the feature
-            df (pd.DataFrame): Categories as rows and descriptors as columns
+            experiments (pd.DataFrame): Dataframe with experimental data
 
         Returns:
-            _type_: _description_
+            pd.DataFrame: Dataframe with all experiments where at least one output feature has a valid entry
         """
-        return cls(
-            key=key,
-            categories=list(df.index),
-            allowed=[True for _ in range(len(df))],
-            descriptors=list(df.columns),
-            values=df.values.tolist(),
-        )
 
+        output_feature_keys = self.get_keys(Output)
 
-class ContinuousOutputFeature(OutputFeature):
-    """The base class for a continuous output feature
+        # clean_exp = experiments.query(" or ".join(["(valid_%s > 0)" % key for key in output_feature_keys]))
+        # clean_exp = clean_exp.query(" or ".join(["%s.notna()" % key for key in output_feature_keys]))
 
-    Attributes:
-        desirability_function (Desirability_function, optional): Desirability function of
-            the feature indicating in which direction it should be optimzed. Defaults to `MaxIdentityDesirabilityFunction`.
-    """
-
-    pass
-
-
-class ContinuousOutputFeature_woDesFunc(ContinuousOutputFeature):
-    """A class for continuous output features which should not be optimized. Deprecated."""
-
-    desirability_function = NoDesirabilityFunction
-
-
-# A helper constant for the default value of the weight parameter
-FEATURE_ORDER = {
-    ContinuousInputFeature: 1,
-    ContinuousDescriptorInputFeature: 2,
-    DiscreteInputFeature: 3,
-    CategoricalInputFeature: 4,
-    CategoricalDescriptorInputFeature: 5,
-    ContinuousOutputFeature: 6,
-    ContinuousOutputFeature_woDesFunc: 7,
-}
-
-## TODO: REMOVE THIS --> it is not needed!
-def is_continuous(var: Feature) -> bool:
-    """Checks if Feature is continous
-
-    Args:
-        var (Feature): Feature to be checked
+        assert experiments is not None
+        clean_exp = experiments.query(
+            " or ".join(
+                [
+                    "((`valid_%s` >0) & `%s`.notna())" % (key, key)
+                    for key in output_feature_keys
+                ]
+            )
+        )
 
-    Returns:
-        bool: True if continuous, else False
-    """
-    # TODO: generalize query via attribute continuousFeature (not existing yet!)
-    if isinstance(var, ContinuousInputFeature) or isinstance(
-        var, ContinuousOutputFeature
-    ):
-        return True
-    else:
-        False
+        return clean_exp
```

### Comparing `bofire-0.0.3/tests/bofire/domain/test_base_model.py` & `bofire-0.0.4/tests/bofire/data_models/test_base.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 import random
 import uuid
-from typing import List
 
 import pytest
 from pydantic.error_wrappers import ValidationError
 
-from bofire.domain.util import BaseModel
+from bofire.data_models.base import BaseModel
 
 
 class Bla(BaseModel):
     a: int = 1
 
 
 @pytest.fixture
```

### Comparing `bofire-0.0.3/tests/bofire/domain/test_concurrency_constraints.py` & `bofire-0.0.4/tests/bofire/data_models/test_nchoosek_combinatorics.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,20 +1,20 @@
-from typing import List
+import unittest
 
 import numpy as np
 import pandas as pd
 import pytest
 
-from bofire.domain.constraints import NChooseKConstraint
-from bofire.domain.domain import Domain
-from bofire.domain.features import (
-    CategoricalDescriptorInputFeature,
-    CategoricalInputFeature,
-    ContinuousInputFeature,
-    ContinuousOutputFeature,
+from bofire.data_models.constraints.api import NChooseKConstraint
+from bofire.data_models.domain.api import Constraints, Domain, Inputs
+from bofire.data_models.features.api import (
+    CategoricalDescriptorInput,
+    CategoricalInput,
+    ContinuousInput,
+    ContinuousOutput,
 )
 
 # NChooseKConstraint constraints 1
 cc1a = NChooseKConstraint(
     features=["0", "1", "2", "3"], min_count=2, max_count=3, none_also_valid=True
 )
 cc2a = NChooseKConstraint(
@@ -33,30 +33,30 @@
 cc3 = [
     NChooseKConstraint(
         features=["0", "1", "2", "3"], min_count=2, max_count=3, none_also_valid=True
     )
 ]
 
 # input features
-continuous_input_features = []
+continuous_inputs = []
 for i in range(6):
-    f = ContinuousInputFeature(key=str(i), lower_bound=0, upper_bound=1)
-    continuous_input_features.append(f)
-categorical_feature = CategoricalInputFeature(
+    f = ContinuousInput(key=str(i), bounds=(0, 1))
+    continuous_inputs.append(f)
+categorical_feature = CategoricalInput(
     key="categorical_feature", categories=["c1", "c2"]
 )
-categorical_descriptor_feature = CategoricalDescriptorInputFeature(
+categorical_descriptor_feature = CategoricalDescriptorInput(
     key="categorical_descriptor_feature",
     categories=["cd1", "cd2"],
     descriptors=["d1", "d2"],
     values=[[1.0, 1.0], [2.0, 2.0]],
 )
 
 # output feature
-output_features = [ContinuousOutputFeature(key="y")]
+outputs = [ContinuousOutput(key="y")]
 
 
 """
 TEST CASES:
 
 CASE 1: 6 continuous features, 2 overlapping NChooseKConstraint constraints, none_also_valid: True, True
 CASE 2: 6 continuous features, 2 overlapping NChooseKConstraint constraints, none_also_valid: False, True
@@ -143,34 +143,34 @@
 
 ##### LIST OF TASTE CASES #####
 
 test_cases = []
 
 # CASE 1
 test_case = {}
-domain = Domain(
-    input_features=continuous_input_features,
-    output_features=output_features,
+domain = Domain.from_lists(
+    inputs=continuous_inputs,
+    outputs=outputs,
     constraints=[cc1a, cc2a],
 )
 test_case["domain"] = domain
 test_case["experiments"] = experiments
 test_case["descriptor_method"] = None
 test_case["categorical_method"] = None
 test_case["descriptor_encoding"] = None
 test_case["categorical_encoding"] = None
 test_case["test_features_used"] = test_features_used_1
 test_case["test_features_unused"] = test_features_unused_1
 test_cases.append(test_case)
 
 # CASE 2
 test_case = {}
-domain = Domain(
-    input_features=continuous_input_features,
-    output_features=output_features,
+domain = Domain.from_lists(
+    continuous_inputs,
+    outputs,
     constraints=[cc1b, cc2b],
 )
 test_case["domain"] = domain
 test_case["experiments"] = experiments
 test_case["descriptor_method"] = None
 test_case["categorical_method"] = None
 test_case["descriptor_encoding"] = None
@@ -179,12 +179,51 @@
 test_case["test_features_unused"] = test_features_unused_2
 test_cases.append(test_case)
 
 
 @pytest.mark.parametrize("test_case", test_cases)
 def test_nchoosek_combinations_completeness(test_case):
     domain = test_case["domain"]
-    features_used, features_unused = domain.get_nchoosek_combinations()
+    features_used, features_unused = domain.get_nchoosek_combinations(exhaustive=True)
     for features in test_case["test_features_used"]:
         assert features in features_used
     for features in test_case["test_features_unused"]:
         assert features in features_unused
+
+
+def test_nchoosek_combinations_nonexhaustive():
+    domain = Domain(
+        inputs=Inputs(
+            features=[ContinuousInput(key=f"if{i+1}", bounds=(0, 1)) for i in range(6)]
+        ),
+        constraints=Constraints(
+            constraints=[
+                NChooseKConstraint(
+                    features=[f"if{i+1}" for i in range(4)],
+                    min_count=0,
+                    max_count=2,
+                    none_also_valid=True,
+                )
+            ]
+        ),
+    )
+    used, unused = domain.get_nchoosek_combinations(exhaustive=False)
+    expected_used = [
+        ["if1", "if2"],
+        ["if1", "if3"],
+        ["if1", "if4"],
+        ["if2", "if3"],
+        ["if2", "if4"],
+        ["if3", "if4"],
+    ]
+    expected_unused = [
+        ["if3", "if4"],
+        ["if2", "if4"],
+        ["if2", "if3"],
+        ["if1", "if4"],
+        ["if1", "if3"],
+        ["if1", "if2"],
+    ]
+    # print(combos, expected_combos)
+    c = unittest.TestCase()
+    c.assertCountEqual(used, expected_used)
+    c.assertCountEqual(unused, expected_unused)
```

### Comparing `bofire-0.0.3/tests/bofire/domain/test_constraint_fulfillment.py` & `bofire-0.0.4/tests/bofire/data_models/test_constraint_fulfillment.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 from typing import List
 
 import pandas as pd
 import pytest
 
-from bofire.domain.constraints import (
+from bofire.data_models.constraints.api import (
     LinearEqualityConstraint,
     LinearInequalityConstraint,
     NChooseKConstraint,
     NonlinearEqualityConstraint,
-    NonlinearInqualityConstraint,
+    NonlinearInequalityConstraint,
 )
 
 F = FEATURES = ["f" + str(i) for i in range(1, 11)]
 
 C = list(range(1, 11))
 
 
@@ -24,39 +24,35 @@
 
 @pytest.mark.parametrize(
     "df, constraint, fulfilled",
     [
         (
             get_row(F[:4], 1),
             NonlinearEqualityConstraint(
-                features=F[:4],
                 expression="f1 + f2 + f3 + f4 -4",
             ),
             True,
         ),
         (
             get_row(F[:4], 1),
             NonlinearEqualityConstraint(
-                features=F[:4],
                 expression="f1 + f2 + f3 + f4 -3",
             ),
             False,
         ),
         (
             get_row(F[:4], 1),
-            NonlinearInqualityConstraint(
-                features=F[:4],
+            NonlinearInequalityConstraint(
                 expression="f1 + f2 + f3 + f4 -5",
             ),
             True,
         ),
         (
             get_row(F[:4], 1),
-            NonlinearInqualityConstraint(
-                features=F[:4],
+            NonlinearInequalityConstraint(
                 expression="f1 + f2 + f3 + f4 -2",
             ),
             False,
         ),
         (
             get_row(F[:4], 1),
             LinearEqualityConstraint(features=F[:4], coefficients=C[:4], rhs=10),
@@ -122,109 +118,100 @@
             ),
             False,
         ),
         (
             get_row(F[:3], values=[1, 1, 1]),
             NChooseKConstraint(
                 features=F[:3],
-                coefficients=C[:3],
                 min_count=0,
                 max_count=3,
                 none_also_valid=True,
             ),
             True,
         ),
         (
             pd.concat(
                 [get_row(F[:3], values=[1, 1, 1]), get_row(F[:3], values=[1, 1, 1])]
             ),
             NChooseKConstraint(
                 features=F[:3],
-                coefficients=C[:3],
                 min_count=0,
                 max_count=3,
                 none_also_valid=True,
             ),
             True,
         ),
         (
             get_row(F[:3], values=[0, 2, 3]),
             NChooseKConstraint(
                 features=F[:3],
-                coefficients=C[:3],
                 min_count=2,
                 max_count=3,
                 none_also_valid=False,
             ),
             True,
         ),
         (
             get_row(F[:3], values=[1, 2, 3]),
             NChooseKConstraint(
                 features=F[:3],
-                coefficients=C[:3],
                 min_count=2,
                 max_count=2,
                 none_also_valid=False,
             ),
             False,
         ),
         (
             get_row(F[:3], values=[0, 0, 3]),
             NChooseKConstraint(
                 features=F[:3],
-                coefficients=C[:3],
                 min_count=2,
                 max_count=3,
                 none_also_valid=False,
             ),
             False,
         ),
         (
             get_row(F[:3], values=[0, 0, 0]),
             NChooseKConstraint(
                 features=F[:3],
-                coefficients=C[:3],
                 min_count=2,
                 max_count=3,
                 none_also_valid=False,
             ),
             False,
         ),
         (
             get_row(F[:3], values=[0, 0, 0]),
             NChooseKConstraint(
                 features=F[:3],
-                coefficients=C[:3],
                 min_count=2,
                 max_count=3,
                 none_also_valid=True,
             ),
             True,
         ),
         (
             pd.concat(
                 [get_row(F[:3], values=[0, 2, 3]), get_row(F[:3], values=[0, 0, 0])]
             ),
             NChooseKConstraint(
                 features=F[:3],
-                coefficients=C[:3],
                 min_count=2,
                 max_count=2,
                 none_also_valid=False,
             ),
             False,
         ),
         (
             pd.concat(
                 [get_row(F[:3], values=[0, 2, 3]), get_row(F[:3], values=[0, 0, 0])]
             ),
             NChooseKConstraint(
                 features=F[:3],
-                coefficients=C[:3],
                 min_count=2,
                 max_count=2,
                 none_also_valid=True,
             ),
             True,
         ),
     ],
```

### Comparing `bofire-0.0.3/tests/bofire/domain/test_domain.py` & `bofire-0.0.4/tests/bofire/data_models/test_domain.py`

 * *Files 20% similar despite different names*

```diff
@@ -2,108 +2,167 @@
 from math import nan
 
 import numpy as np
 import pandas as pd
 import pytest
 from pandas.testing import assert_frame_equal
 from pydantic.error_wrappers import ValidationError
-from pydantic.types import constr
+from pytest import fixture
 
-from bofire.domain.constraints import LinearEqualityConstraint, NChooseKConstraint
-from bofire.domain.desirability_functions import TargetDesirabilityFunction
-from bofire.domain.domain import Domain, get_subdomain
-from bofire.domain.features import (
-    CategoricalDescriptorInputFeature,
-    CategoricalInputFeature,
-    ContinuousInputFeature,
-    ContinuousOutputFeature,
-    ContinuousOutputFeature_woDesFunc,
+from bofire.data_models.api import Outputs
+from bofire.data_models.base import BaseModel
+from bofire.data_models.constraints.api import (
+    LinearEqualityConstraint,
+    NChooseKConstraint,
+)
+from bofire.data_models.domain.api import Domain
+from bofire.data_models.domain.constraints import Constraints
+from bofire.data_models.domain.features import Inputs
+from bofire.data_models.features.api import (
+    CategoricalDescriptorInput,
+    CategoricalInput,
+    ContinuousInput,
+    ContinuousOutput,
+    DiscreteInput,
     Feature,
-    InputFeature,
-    OutputFeature,
+    Input,
+    Output,
 )
-from bofire.domain.util import BaseModel
+from bofire.data_models.objectives.api import (
+    ConstrainedObjective,
+    MaximizeObjective,
+    MaximizeSigmoidObjective,
+    Objective,
+    TargetObjective,
+)
+from bofire.utils.subdomain import get_subdomain
 
 
 def test_empty_domain():
-    Domain(
-        input_features=[],
-        output_features=[],
-        constraints=[],
+    assert Domain() == Domain(
+        inputs=Inputs(), outputs=Outputs(), constraints=Constraints()
     )
 
 
-df = TargetDesirabilityFunction(
-    target_value=1,
-    steepness=2,
-    tolerance=3,
-    w=0.5,
-)
-
-
 class Bla(BaseModel):
     a: int
 
 
 nf = Bla(a=1)
 
-if_ = CategoricalInputFeature(key="if", categories=["a", "b"])
-of_ = ContinuousOutputFeature(key="of", desirability_function=df)
-
+obj = TargetObjective(target_value=1, steepness=2, tolerance=3, w=0.5)
 
-if1 = ContinuousInputFeature(key="f1", upper_bound=10, lower_bound=0)
-if1_ = ContinuousInputFeature(key="f1", upper_bound=10, lower_bound=1)
-if2 = ContinuousInputFeature(key="f2", upper_bound=10, lower_bound=0)
+if_ = CategoricalInput(key="if", categories=["a", "b"])
+of_ = ContinuousOutput(key="of", objective=obj)
+if1 = ContinuousInput(key="f1", bounds=(0, 10))
+if1_ = ContinuousInput(key="f1", bounds=(0, 1))
+if2 = ContinuousInput(key="f2", bounds=(0, 10))
+of1 = ContinuousOutput(key="f1", objective=obj)
+of1_ = ContinuousOutput(key="f1", objective=obj)
+of2 = ContinuousOutput(key="f2", objective=obj)
+of3 = ContinuousOutput(key="of3", objective=obj)
+
+
+@fixture
+def input_list():
+    return [
+        ContinuousInput(key="ci1", bounds=(0, 1)),
+        ContinuousInput(key="ci2", bounds=(0, 1)),
+    ]
+
+
+@fixture
+def output_list():
+    objective = TargetObjective(target_value=1, steepness=2, tolerance=3, w=0.5)
+    return [
+        ContinuousOutput(key="co1", objective=objective),
+        ContinuousOutput(key="co2", objective=objective),
+    ]
+
+
+@fixture
+def constraint_list(input_list):
+    return [
+        LinearEqualityConstraint(
+            features=[inp.key for inp in input_list],
+            coefficients=[1.0] * len(input_list),
+            rhs=11,
+        )
+    ]
 
-of1 = ContinuousOutputFeature(key="f1", desirability_function=df)
-of1_ = ContinuousOutputFeature(key="f1", desirability_function=df)
-of2 = ContinuousOutputFeature(key="f2", desirability_function=df)
 
-of3 = ContinuousOutputFeature(key="of3", desirability_function=df)
+def test_from_lists(input_list, output_list, constraint_list):
+    assert Domain.from_lists(
+        inputs=input_list, outputs=output_list, constraints=constraint_list
+    ) == Domain(
+        inputs=Inputs(features=input_list),
+        outputs=Outputs(features=output_list),
+        constraints=Constraints(constraints=constraint_list),
+    )
 
 
 @pytest.mark.parametrize(
-    "input_features, output_features",
+    "inputs, outputs",
     [
         ([if1, if1_], []),
         ([], [of1, of1_]),
         ([if1], [of1]),
     ],
 )
-def test_duplicate_feature_names(input_features, output_features):
+def test_duplicate_feature_names(inputs, outputs):
     with pytest.raises(ValidationError):
         Domain(
-            input_features=input_features,
-            output_features=output_features,
-            constraints=[],
+            inputs=inputs,
+            outputs=outputs,
         )
 
 
 @pytest.mark.parametrize(
-    "input_features, output_features, constraints",
+    "inputs, outputs, constraints",
     [
         # input features
         ([nf], [], []),
         # output features
         ([], [nf], []),
         # constraints
         # ([], [], [nf]),
     ],
 )
-def test_invalid_domain_arg_types(input_features, output_features, constraints):
+def test_invalid_domain_arg_types(inputs, outputs, constraints):
     with pytest.raises(Exception):
         Domain(
-            input_features=input_features,
-            output_features=output_features,
+            inputs=inputs,
+            outputs=outputs,
             constraints=constraints,
         )
 
 
 @pytest.mark.parametrize(
-    "input_features, output_features, constraints",
+    "inputs, constraints",
+    [
+        (
+            [
+                ContinuousInput(key="if1", bounds=(0, 1)),
+                DiscreteInput(key="if2", values=[0.2, 0.7, 1.0]),
+            ],
+            [
+                LinearEqualityConstraint(
+                    features=["if1", "if2"], coefficients=[1.0, 1.0], rhs=11
+                )
+            ],
+        )
+    ],
+)
+def test_invalid_type_in_linear_constraints(inputs, constraints):
+    with pytest.raises(ValidationError):
+        Domain(inputs=inputs, constraints=constraints)
+
+
+@pytest.mark.parametrize(
+    "inputs, outputs, constraints",
     [
         (
             [if1, if2],
             [of3],
             [
                 NChooseKConstraint(
                     features=["f1", "f2"],
@@ -123,24 +182,24 @@
                     max_count=2,
                     none_also_valid=True,
                 )
             ],
         ),
     ],
 )
-def test_valid_constraints_in_domain(output_features, input_features, constraints):
+def test_valid_constraints_in_domain(outputs, inputs, constraints):
     Domain(
-        input_features=input_features,
-        output_features=output_features,
+        inputs=inputs,
+        outputs=outputs,
         constraints=constraints,
     )
 
 
 @pytest.mark.parametrize(
-    "input_features, output_features, constraints",
+    "inputs, outputs, constraints",
     [
         (
             [],
             [],
             [
                 NChooseKConstraint(
                     features=["x", "t55"],
@@ -184,173 +243,177 @@
                     max_count=1,
                     none_also_valid=True,
                 )
             ],
         ),
     ],
 )
-def test_unknown_features_in_domain(output_features, input_features, constraints):
+def test_unknown_features_in_domain(outputs, inputs, constraints):
     with pytest.raises(ValidationError):
         Domain(
-            input_features=input_features,
-            output_features=output_features,
+            inputs=inputs,
+            outputs=outputs,
             constraints=constraints,
         )
 
 
 @pytest.mark.parametrize(
     "domain, data",
     [
         (
-            Domain(
-                input_features=[],
-                output_features=[],
-                constraints=[],
-            ),
+            Domain(),
             [],
         ),
         (
             Domain(
-                input_features=[
-                    CategoricalInputFeature(
-                        key="f1",
-                        categories=["c11", "c12"],
-                    ),
-                ],
-                output_features=[],
-                constraints=[],
+                inputs=Inputs(
+                    features=[
+                        CategoricalInput(
+                            key="f1",
+                            categories=["c11", "c12"],
+                        ),
+                    ]
+                ),
             ),
             [
                 [("f1", "c11"), ("f1", "c12")],
             ],
         ),
         (
             Domain(
-                input_features=[
-                    CategoricalInputFeature(
-                        key="f1",
-                        categories=["c11", "c12"],
-                    ),
-                    CategoricalInputFeature(
-                        key="f2",
-                        categories=["c21", "c22", "c23"],
-                    ),
-                    CategoricalInputFeature(
-                        key="f3",
-                        categories=["c31", "c32"],
-                    ),
-                ],
-                output_features=[],
-                constraints=[],
+                inputs=Inputs(
+                    features=[
+                        CategoricalInput(
+                            key="f1",
+                            categories=["c11", "c12"],
+                        ),
+                        CategoricalInput(
+                            key="f2",
+                            categories=["c21", "c22", "c23"],
+                        ),
+                        CategoricalInput(
+                            key="f3",
+                            categories=["c31", "c32"],
+                        ),
+                    ]
+                ),
             ),
             [
                 [("f1", "c11"), ("f1", "c12")],
                 [("f2", "c21"), ("f2", "c22"), ("f2", "c23")],
                 [("f3", "c31"), ("f3", "c32")],
             ],
         ),
     ],
 )
 def test_categorical_combinations_of_domain_defaults(domain, data):
     expected = list(itertools.product(*data))
-    assert domain.get_categorical_combinations() == expected
+    assert domain.inputs.get_categorical_combinations() == expected
 
 
 @pytest.mark.parametrize(
     "domain, data, include, exclude",
     [
         (
             Domain(
-                input_features=[
-                    CategoricalInputFeature(
-                        key="f1",
-                        categories=["c11", "c12"],
-                    ),
-                    CategoricalDescriptorInputFeature(
-                        key="f2",
-                        categories=["c21", "c22"],
-                        descriptors=["d21", "d22"],
-                        values=[[1, 2], [3, 4]],
-                    ),
-                ],
+                inputs=Inputs(
+                    features=[
+                        CategoricalInput(
+                            key="f1",
+                            categories=["c11", "c12"],
+                        ),
+                        CategoricalDescriptorInput(
+                            key="f2",
+                            categories=["c21", "c22"],
+                            descriptors=["d21", "d22"],
+                            values=[[1, 2], [3, 4]],
+                        ),
+                    ]
+                ),
             ),
             [
                 [("f1", "c11"), ("f1", "c12")],
             ],
-            CategoricalInputFeature,
-            CategoricalDescriptorInputFeature,
+            CategoricalInput,
+            CategoricalDescriptorInput,
         ),
         (
             Domain(
-                input_features=[
-                    CategoricalInputFeature(
-                        key="f1",
-                        categories=["c11", "c12"],
-                    ),
-                    CategoricalDescriptorInputFeature(
-                        key="f2",
-                        categories=["c21", "c22"],
-                        descriptors=["d21", "d22"],
-                        values=[[1, 2], [3, 4]],
-                    ),
-                ],
+                inputs=Inputs(
+                    features=[
+                        CategoricalInput(
+                            key="f1",
+                            categories=["c11", "c12"],
+                        ),
+                        CategoricalDescriptorInput(
+                            key="f2",
+                            categories=["c21", "c22"],
+                            descriptors=["d21", "d22"],
+                            values=[[1, 2], [3, 4]],
+                        ),
+                    ]
+                ),
             ),
             [
-                [("f1", "c11"), ("f1", "c12")],
                 [("f2", "c21"), ("f2", "c22")],
+                [("f1", "c11"), ("f1", "c12")],
             ],
-            CategoricalInputFeature,
+            CategoricalInput,
             None,
         ),
         (
             Domain(
-                input_features=[
-                    CategoricalInputFeature(
-                        key="f1",
-                        categories=["c11", "c12"],
-                    ),
-                    CategoricalDescriptorInputFeature(
-                        key="f2",
-                        categories=["c21", "c22"],
-                        descriptors=["d21", "d22"],
-                        values=[[1, 2], [3, 4]],
-                    ),
-                ],
+                inputs=Inputs(
+                    features=[
+                        CategoricalInput(
+                            key="f1",
+                            categories=["c11", "c12"],
+                        ),
+                        CategoricalDescriptorInput(
+                            key="f2",
+                            categories=["c21", "c22"],
+                            descriptors=["d21", "d22"],
+                            values=[[1, 2], [3, 4]],
+                        ),
+                    ]
+                ),
             ),
             [
                 [("f2", "c21"), ("f2", "c22")],
             ],
-            CategoricalDescriptorInputFeature,
+            CategoricalDescriptorInput,
             None,
         ),
         (
             Domain(
-                input_features=[
-                    CategoricalInputFeature(
-                        key="f1",
-                        categories=["c11", "c12"],
-                    ),
-                    CategoricalDescriptorInputFeature(
-                        key="f2",
-                        categories=["c21", "c22"],
-                        descriptors=["d21", "d22"],
-                        values=[[1, 2], [3, 4]],
-                    ),
-                ],
+                inputs=Inputs(
+                    features=[
+                        CategoricalInput(
+                            key="f1",
+                            categories=["c11", "c12"],
+                        ),
+                        CategoricalDescriptorInput(
+                            key="f2",
+                            categories=["c21", "c22"],
+                            descriptors=["d21", "d22"],
+                            values=[[1, 2], [3, 4]],
+                        ),
+                    ]
+                ),
             ),
             [],
-            CategoricalDescriptorInputFeature,
-            CategoricalInputFeature,
+            CategoricalDescriptorInput,
+            CategoricalInput,
         ),
     ],
 )
 def test_categorical_combinations_of_domain_filtered(domain, data, include, exclude):
     expected = list(itertools.product(*data))
     assert (
-        domain.get_categorical_combinations(include=include, exclude=exclude)
+        domain.inputs.get_categorical_combinations(include=include, exclude=exclude)
         == expected
     )
 
 
 data = pd.DataFrame.from_dict(
     {
         "x1": [1.0, 2.0, 3.0, 4.0, 5.0, 6.0],
@@ -358,35 +421,42 @@
         "out1": [nan, 1.0, 2.0, 3.0, nan, nan],
         "out2": [nan, 1.0, 2.0, 3.0, 4.0, 5.0],
         "valid_out1": [1, 0, 1, 1, 1, 1],
         "valid_out2": [1, 1, 0, 1, 1, 0],
     }
 )
 
-if1 = ContinuousInputFeature(key="x1", upper_bound=10, lower_bound=1)
-if2 = ContinuousInputFeature(key="x2", upper_bound=10, lower_bound=1)
+if1 = ContinuousInput(key="x1", bounds=(1, 10))
+if2 = ContinuousInput(key="x2", bounds=(1, 10))
 
-of1 = ContinuousOutputFeature(key="out1", desirability_function=df)
-of2 = ContinuousOutputFeature(key="out2", desirability_function=df)
+of1 = ContinuousOutput(key="out1", objective=obj)
+of2 = ContinuousOutput(key="out2", objective=obj)
 
 c1 = LinearEqualityConstraint(features=["x1", "x2"], coefficients=[5, 5], rhs=15.0)
 
-of1_ = ContinuousOutputFeature_woDesFunc(key="out3")
-of2_ = ContinuousOutputFeature_woDesFunc(key="out4")
+of1_ = ContinuousOutput(key="out3", objective=None)
+of2_ = ContinuousOutput(key="out4", objective=None)
 
-domain = Domain(input_features=[if1, if2], output_features=[of1, of2])
+domain = Domain(
+    inputs=Inputs(features=[if1, if2]), outputs=Outputs(features=[of1, of2])
+)
 domain2 = Domain(
-    input_features=[if1, if2], output_features=[of1, of2], constraints=[c1]
+    inputs=Inputs(features=[if1, if2]),
+    outputs=Outputs(features=[of1, of2]),
+    constraints=Constraints(constraints=[c1]),
 )
 
 
 @pytest.mark.parametrize("domain", [domain, domain2])
-def test_domain_serialie(domain):
-    config = domain.to_config()
-    ndomain = Domain.from_config(config=config)
+def test_domain_serialize(domain):
+    print("domain:", domain)
+    import json
+
+    print("dict:", json.dumps(domain.dict(), indent=4))
+    ndomain = Domain(**json.loads(domain.json()))
     assert ndomain == domain
 
 
 @pytest.mark.parametrize(
     "domain, data, output_feature_keys, expected",
     [
         (
@@ -450,27 +520,20 @@
             ),
         ),
     ],
 )
 def test_preprocess_experiments_all_valid_outputs(
     domain, data, output_feature_keys, expected
 ):
-    experiments = domain.preprocess_experiments_all_valid_outputs(
+    experiments = domain.outputs.preprocess_experiments_all_valid_outputs(
         data, output_feature_keys
     )
     assert_frame_equal(experiments.reset_index(drop=True), expected, check_dtype=False)
 
 
-def test_preprocess_experiments_all_valid_outputs_invalid():
-    with pytest.raises(AssertionError):
-        experiments = domain.preprocess_experiments_all_valid_outputs(
-            data, output_feature_keys=["x1"]
-        )
-
-
 @pytest.mark.parametrize(
     "domain, data, expected",
     [
         (
             domain,
             data,
             pd.DataFrame.from_dict(
@@ -483,15 +546,15 @@
                     "valid_out2": [1, 0, 1, 1],
                 }
             ),
         )
     ],
 )
 def test_preprocess_experiments_any_valid_output(domain, data, expected):
-    experiments = domain.preprocess_experiments_any_valid_output(data)
+    experiments = domain.outputs.preprocess_experiments_any_valid_output(data)
     assert experiments["x1"].tolist() == expected["x1"].tolist()
     assert experiments["out2"].tolist() == expected["out2"].tolist()
 
 
 @pytest.mark.parametrize(
     "domain, data, expected",
     [
@@ -508,22 +571,24 @@
                     "valid_out2": [1, 1, 1],
                 }
             ),
         )
     ],
 )
 def test_preprocess_experiments_one_valid_output(domain, data, expected):
-    experiments = domain.preprocess_experiments_one_valid_output("out2", data)
+    experiments = domain.outputs.preprocess_experiments_one_valid_output("out2", data)
     assert experiments["x1"].tolist() == expected["x1"].tolist()
     assert np.isnan(experiments["out1"].tolist()[2])
     assert experiments["out2"].tolist() == expected["out2"].tolist()
 
 
 def test_coerce_invalids():
-    domain = Domain(input_features=[if1, if2], output_features=[of1, of2])
+    domain = Domain(
+        inputs=Inputs(features=[if1, if2]), outputs=Outputs(features=[of1, of2])
+    )
     experiments = domain.coerce_invalids(data)
     expected = pd.DataFrame.from_dict(
         {
             "x1": [1.0, 2.0, 3.0, 4.0, 5.0, 6.0],
             "x2": [1.0, 2.0, 3.0, 4.0, 5.0, 6.0],
             "out1": [nan, nan, 2.0, 3.0, nan, nan],
             "out2": [nan, 1.0, nan, 3.0, 4.0, nan],
@@ -536,144 +601,170 @@
 
 def test_aggregate_by_duplicates():
     # dataframe with duplicates
     full = pd.DataFrame.from_dict(
         {
             "x1": [1.0, 2.0, 3.0, 1.0],
             "x2": [1.0, 2.0, 3.0, 1.0],
-            "out1": [
-                4.0,
-                5.0,
-                6.0,
-                3.0,
-            ],
-            "out2": [
-                -4.0,
-                -5.0,
-                -6.0,
-                -3.0,
-            ],
+            "out1": [4.0, 5.0, 6.0, 3.0],
+            "out2": [-4.0, -5.0, -6.0, -3.0],
             "valid_out1": [1, 1, 1, 1],
             "valid_out2": [1, 1, 1, 1],
         }
     )
     expected_aggregated = pd.DataFrame.from_dict(
         {
             "labcode": ["1-4", "2", "3"],
             "x1": [1.0, 2.0, 3.0],
-            "x2": [
-                1.0,
-                2.0,
-                3.0,
-            ],
+            "x2": [1.0, 2.0, 3.0],
             "out1": [3.5, 5.0, 6.0],
             "out2": [-3.5, -5.0, -6.0],
             "valid_out1": [1, 1, 1],
             "valid_out2": [1, 1, 1],
         }
     )
-    domain = Domain(input_features=[if1, if2], output_features=[of1, of2])
+    domain = Domain(
+        inputs=Inputs(features=[if1, if2]), outputs=Outputs(features=[of1, of2])
+    )
     aggregated, duplicated_labcodes = domain.aggregate_by_duplicates(full, prec=2)
     assert duplicated_labcodes == [["1", "4"]]
     assert_frame_equal(
         aggregated, expected_aggregated, check_dtype=False, check_like=True
     )
     # dataset without duplicates
     full = pd.DataFrame.from_dict(
         {
             "x1": [1.0, 2.0, 3.0, 4.0],
             "x2": [1.0, 2.0, 3.0, 4.0],
-            "out1": [
-                4.0,
-                5.0,
-                6.0,
-                3.0,
-            ],
-            "out2": [
-                -4.0,
-                -5.0,
-                -6.0,
-                -3.0,
-            ],
+            "out1": [4.0, 5.0, 6.0, 3.0],
+            "out2": [-4.0, -5.0, -6.0, -3.0],
             "valid_out1": [1, 1, 1, 1],
             "valid_out2": [1, 1, 1, 1],
         }
     )
     expected_aggregated = pd.DataFrame.from_dict(
         {
             "labcode": ["0", "1", "2", "3"],
             "x1": [1.0, 2.0, 3.0, 4.0],
             "x2": [1.0, 2.0, 3.0, 4.0],
-            "out1": [
-                4.0,
-                5.0,
-                6.0,
-                3.0,
-            ],
-            "out2": [
-                -4.0,
-                -5.0,
-                -6.0,
-                -3.0,
-            ],
+            "out1": [4.0, 5.0, 6.0, 3.0],
+            "out2": [-4.0, -5.0, -6.0, -3.0],
             "valid_out1": [1, 1, 1, 1],
             "valid_out2": [1, 1, 1, 1],
         }
     )
-    domain = Domain(input_features=[if1, if2], output_features=[of1, of2])
+    domain = Domain(
+        inputs=Inputs(features=[if1, if2]), outputs=Outputs(features=[of1, of2])
+    )
     aggregated, duplicated_labcodes = domain.aggregate_by_duplicates(full, prec=2)
     assert duplicated_labcodes == []
 
 
-domain = Domain(input_features=[if1, if2], output_features=[of1, of2, of1_, of2_])
+domain = Domain(
+    inputs=Inputs(features=[if1, if2]), outputs=Outputs(features=[of1, of2, of1_, of2_])
+)
 
 
 @pytest.mark.parametrize(
     "domain, FeatureType, exact, expected",
     [
-        (domain, OutputFeature, True, []),
-        (domain, OutputFeature, False, [of1, of2, of1_, of2_]),
-        (domain, OutputFeature, None, [of1, of2, of1_, of2_]),
-        (domain, ContinuousOutputFeature, True, [of1, of2]),
-        (domain, ContinuousOutputFeature, False, [of1, of2, of1_, of2_]),
-        (domain, ContinuousOutputFeature, None, [of1, of2, of1_, of2_]),
-        (domain, ContinuousOutputFeature_woDesFunc, True, [of1_, of2_]),
-        (domain, ContinuousOutputFeature_woDesFunc, False, [of1_, of2_]),
-        (domain, ContinuousOutputFeature_woDesFunc, None, [of1_, of2_]),
-        (domain, InputFeature, True, []),
-        (domain, InputFeature, False, [if1, if2]),
-        (domain, InputFeature, None, [if1, if2]),
+        (domain, Output, True, []),
+        (domain, Output, False, [of1, of2, of1_, of2_]),
+        (domain, Output, None, [of1, of2, of1_, of2_]),
+        (domain, ContinuousOutput, True, [of1, of2, of1_, of2_]),
+        (domain, ContinuousOutput, False, [of1, of2, of1_, of2_]),
+        (domain, ContinuousOutput, None, [of1, of2, of1_, of2_]),
+        (domain, Input, True, []),
+        (domain, Input, False, [if1, if2]),
+        (domain, Input, None, [if1, if2]),
     ],
 )
 def test_get_features(domain, FeatureType, exact, expected):
-    assert domain.get_features(FeatureType, exact=exact) == expected
+    assert domain.get_features(FeatureType, exact=exact).features == expected
+
+
+@pytest.mark.parametrize(
+    "domain, includes, excludes, exact, expected",
+    [
+        (domain, [Objective], [], True, []),
+        (domain, [Objective], [], False, [of1, of2]),
+        (domain, [TargetObjective], [], False, [of1, of2]),
+        (domain, [], [Objective], False, [of1_, of2_]),
+    ],
+)
+def test_get_outputs_by_objective(domain: Domain, includes, excludes, exact, expected):
+    assert (
+        domain.outputs.get_by_objective(
+            includes=includes,
+            excludes=excludes,
+            exact=exact,
+        ).features
+        == expected
+    )
+
+
+def test_get_outputs_by_objective_none():
+    outputs = Outputs(
+        features=[
+            ContinuousOutput(key="a", objective=None),
+            ContinuousOutput(
+                key="b", objective=MaximizeSigmoidObjective(w=1, steepness=1, tp=0)
+            ),
+            ContinuousOutput(key="c", objective=MaximizeObjective()),
+        ]
+    )
+    keys = outputs.get_keys_by_objective(excludes=ConstrainedObjective)
+    assert keys == ["c"]
+    assert outputs.get_keys().index("c") == 2
+    assert outputs.get_keys_by_objective(excludes=Objective, includes=[]) == ["a"]
+    assert outputs.get_by_objective(excludes=Objective, includes=[]) == Outputs(
+        features=[ContinuousOutput(key="a", objective=None)]
+    )
 
 
 @pytest.mark.parametrize(
     "domain, FeatureType, exact, expected",
     [
-        (domain, OutputFeature, True, []),
-        (domain, OutputFeature, False, ["out1", "out2", "out3", "out4"]),
-        (domain, OutputFeature, None, ["out1", "out2", "out3", "out4"]),
-        (domain, ContinuousOutputFeature, True, ["out1", "out2"]),
-        (domain, ContinuousOutputFeature, False, ["out1", "out2", "out3", "out4"]),
-        (domain, ContinuousOutputFeature, None, ["out1", "out2", "out3", "out4"]),
-        (domain, ContinuousOutputFeature_woDesFunc, True, ["out3", "out4"]),
-        (domain, ContinuousOutputFeature_woDesFunc, False, ["out3", "out4"]),
-        (domain, ContinuousOutputFeature_woDesFunc, None, ["out3", "out4"]),
-        (domain, InputFeature, True, []),
-        (domain, InputFeature, False, ["x1", "x2"]),
-        (domain, InputFeature, None, ["x1", "x2"]),
+        (domain, Output, True, []),
+        (domain, Output, False, ["out1", "out2", "out3", "out4"]),
+        (domain, Output, None, ["out1", "out2", "out3", "out4"]),
+        (domain, ContinuousOutput, True, ["out1", "out2", "out3", "out4"]),
+        (domain, ContinuousOutput, None, ["out1", "out2", "out3", "out4"]),
+        (domain, Input, True, []),
+        (domain, Input, False, ["x1", "x2"]),
+        (domain, Input, None, ["x1", "x2"]),
     ],
 )
 def test_get_feature_keys(domain, FeatureType, exact, expected):
     assert domain.get_feature_keys(FeatureType, exact=exact) == expected
 
 
 @pytest.mark.parametrize(
+    "domain, includes, excludes, exact, expected",
+    [
+        (domain, [Objective], [], False, ["out1", "out2"]),
+        (domain, [TargetObjective], [], False, ["out1", "out2"]),
+        (domain, [Objective], [], True, []),
+        (domain, [], [Objective], False, ["out3", "out4"]),
+    ],
+)
+def test_get_output_keys_by_objective(
+    domain: Domain, includes, excludes, exact, expected
+):
+    assert (
+        domain.outputs.get_keys_by_objective(
+            includes=includes,
+            excludes=excludes,
+            exact=exact,
+        )
+        == expected
+    )
+
+
+@pytest.mark.parametrize(
     "domain, feature_keys",
     [
         (domain, ["x1", "x2", "out1", "out2"]),
         (domain, ["x1", "x2", "out1"]),
         (domain, ["x1", "x2", "out1", "out3"]),
         (domain, ["x1", "out1", "out3", "out4"]),
         (domain2, ["x1", "x2", "out1", "out2"]),
```

### Comparing `bofire-0.0.3/tests/bofire/domain/test_domain_validators.py` & `bofire-0.0.4/tests/bofire/data_models/test_domain_validators.py`

 * *Files 15% similar despite different names*

```diff
@@ -2,212 +2,184 @@
 import uuid
 from typing import List
 
 import numpy as np
 import pandas as pd
 import pytest
 
-from bofire.domain.domain import Domain
-from bofire.domain.features import (
-    CategoricalDescriptorInputFeature,
-    CategoricalInputFeature,
-    ContinuousInputFeature,
-    ContinuousOutputFeature,
-    InputFeature,
-    OutputFeature,
-)
-from tests.bofire.domain.test_features import (
-    VALID_CATEGORICAL_DESCRIPTOR_INPUT_FEATURE_SPEC,
-    VALID_CATEGORICAL_INPUT_FEATURE_SPEC,
-    VALID_CONTINUOUS_INPUT_FEATURE_SPEC,
-    VALID_CONTINUOUS_OUTPUT_FEATURE_SPEC,
-    VALID_FIXED_CATEGORICAL_INPUT_FEATURE_SPEC,
-    VALID_FIXED_CONTINUOUS_INPUT_FEATURE_SPEC,
-)
-
-if1 = ContinuousInputFeature(
-    **{
-        **VALID_CONTINUOUS_INPUT_FEATURE_SPEC,
-        "key": "cont",
-    }
-)
-if2 = CategoricalInputFeature(
-    **{
-        **VALID_CATEGORICAL_INPUT_FEATURE_SPEC,
-        "key": "cat",
-    }
-)
-if3 = CategoricalDescriptorInputFeature(
-    **{
-        **VALID_CATEGORICAL_DESCRIPTOR_INPUT_FEATURE_SPEC,
-        "key": "cat_",
-    }
-)
-if4 = CategoricalInputFeature(
-    **{
-        **VALID_CATEGORICAL_INPUT_FEATURE_SPEC,
-        "key": "cat2",
-        "allowed": [True, True, False],
-    }
-)
-if5 = ContinuousInputFeature(
-    **{
-        **VALID_FIXED_CONTINUOUS_INPUT_FEATURE_SPEC,
-        "key": "if5",
-    }
-)
-if6 = CategoricalInputFeature(
-    **{
-        **VALID_FIXED_CATEGORICAL_INPUT_FEATURE_SPEC,
-        "key": "if6",
-    }
-)
-of1 = ContinuousOutputFeature(
-    **{
-        **VALID_CONTINUOUS_OUTPUT_FEATURE_SPEC,
-        "key": "out1",
-    }
-)
-of2 = ContinuousOutputFeature(
-    **{
-        **VALID_CONTINUOUS_OUTPUT_FEATURE_SPEC,
-        "key": "out2",
-    }
+import tests.bofire.data_models.specs.api as specs
+from bofire.data_models.constraints.api import LinearEqualityConstraint
+from bofire.data_models.domain.api import Domain
+from bofire.data_models.features.api import (
+    CategoricalDescriptorInput,
+    CategoricalInput,
+    ContinuousInput,
+    ContinuousOutput,
+    DiscreteInput,
+    Input,
+    Output,
+)
+
+if1 = specs.features.valid(ContinuousInput).obj(key="cont")
+if2 = specs.features.valid(CategoricalInput).obj(key="cat")
+if3 = specs.features.valid(CategoricalDescriptorInput).obj(key="cat_")
+if4 = specs.features.valid(CategoricalInput).obj(
+    key="cat2", allowed=[True, True, False]
+)
+if5 = specs.features.valid(ContinuousInput).obj(
+    key="if5",
+    bounds=(3, 3),
 )
+if6 = specs.features.valid(CategoricalInput).obj(
+    key="if6", categories=["c1", "c2", "c3"], allowed=[True, False, False]
+)
+of1 = specs.features.valid(ContinuousOutput).obj(key="out1")
+of2 = specs.features.valid(ContinuousOutput).obj(key="out2")
 
 
 def generate_experiments(
     domain: Domain,
     row_count: int = 5,
     tol: float = 0.0,
     only_allowed_categories: bool = False,
     force_all_categories: bool = False,
     include_labcode: bool = False,
 ):
     if only_allowed_categories:
-        assert force_all_categories == False
+        assert force_all_categories is False
     if force_all_categories:
-        assert only_allowed_categories == False
+        assert only_allowed_categories is False
     experiments = pd.DataFrame.from_dict(
         [
             {
                 **{
                     f.key: random.uniform(f.lower_bound - tol, f.upper_bound + tol)
-                    for f in domain.get_features(ContinuousInputFeature)
+                    for f in domain.get_features(ContinuousInput)
+                },
+                **{
+                    f.key: random.choice(f.values)
+                    for f in domain.get_features(DiscreteInput)
                 },
                 **{
                     k: random.random()
                     for k in [
-                        *domain.get_feature_keys(ContinuousOutputFeature),
+                        *domain.get_feature_keys(ContinuousOutput),
                     ]
                 },
                 **{
                     f.key: random.choice(f.categories)
                     if not only_allowed_categories
                     else random.choice(f.get_allowed_categories())
-                    for f in domain.get_features(CategoricalInputFeature)
+                    for f in domain.get_features(CategoricalInput)
                 },
             }
             for _ in range(row_count)
         ]
     )
     if include_labcode:
         experiments["labcode"] = [str(i) for i in range(row_count)]
     if force_all_categories:
-        for feat in domain.get_features(CategoricalInputFeature):
+        for feat in domain.get_features(CategoricalInput):
             categories = (
                 feat.categories
                 if len(feat.categories) <= row_count
                 else feat.categories[:row_count]
             )
             experiments.loc[: len(categories) - 1, feat.key] = categories
+
     return experiments
 
 
 def generate_candidates(domain: Domain, row_count: int = 5):
     return pd.DataFrame.from_dict(
         [
             {
                 **{
                     feat.key: random.uniform(feat.lower_bound, feat.upper_bound)
-                    for feat in domain.get_features(ContinuousInputFeature)
+                    for feat in domain.get_features(ContinuousInput)
                 },
                 **{
                     f"{k}_pred": random.random()
-                    for k in domain.get_feature_keys(ContinuousOutputFeature)
+                    for k in domain.get_feature_keys(ContinuousOutput)
                 },
                 **{
                     f"{k}_sd": random.random()
-                    for k in domain.get_feature_keys(ContinuousOutputFeature)
+                    for k in domain.get_feature_keys(ContinuousOutput)
                 },
                 **{
                     f"{k}_des": random.random()
-                    for k in domain.get_feature_keys(ContinuousOutputFeature)
+                    for k in domain.get_feature_keys(ContinuousOutput)
                 },
                 **{
                     f.key: random.choice(f.get_allowed_categories())
-                    for f in domain.get_features(CategoricalInputFeature)
+                    for f in domain.get_features(CategoricalInput)
                 },
             }
             for _ in range(row_count)
         ]
     )
 
 
 def generate_invalid_candidates_bounds(domain, row_count: int = 5, error="lower"):
     candidates = generate_candidates(domain, row_count)
     if error == "lower":
-        candidates.loc[0, domain.get_feature_keys(ContinuousInputFeature)[0]] = (
-            domain.get_features(ContinuousInputFeature)[0].lower_bound - 0.1
+        candidates.loc[0, domain.get_feature_keys(ContinuousInput)[0]] = (
+            domain.get_features(ContinuousInput)[0].lower_bound - 0.1
         )
     else:
-        candidates.loc[0, domain.get_feature_keys(ContinuousInputFeature)[0]] = (
-            domain.get_features(ContinuousInputFeature)[0].upper_bound + 0.1
+        candidates.loc[0, domain.get_feature_keys(ContinuousInput)[0]] = (
+            domain.get_features(ContinuousInput)[0].upper_bound + 0.1
         )
     return candidates
 
 
-domain0 = Domain(
-    input_features=[if1, if2, if3],
-    output_features=[of1, of2],
-    constraints=[],
-)
-
-domain1 = Domain(
-    input_features=[if1, if2],
-    output_features=[of1],
+domain0 = Domain.from_lists(
+    inputs=[if1, if2, if3],
+    outputs=[of1, of2],
     constraints=[],
 )
 
-domain2 = Domain(
-    input_features=[if1, if2, if3],
-    output_features=[of1],
+domain1 = Domain.from_lists(
+    inputs=[if1, if2],
+    outputs=[of1],
     constraints=[],
 )
 
-domain3 = Domain(
-    input_features=[if1, if2],
-    output_features=[of1, of2],
+domain2 = Domain.from_lists(
+    inputs=[if1, if2, if3],
+    outputs=[of1],
     constraints=[],
 )
 
-domain4 = Domain(
-    input_features=[if1, if2, if3, if4],
-    output_features=[of1, of2],
-    constraints=[],
-)
-domain5 = Domain(
-    input_features=[if1, if5],
-    output_features=[of1, of2],
-    constraints=[],
-)
-domain6 = Domain(
-    input_features=[if1, if6],
-    output_features=[of1, of2],
-    constraints=[],
+domain3 = Domain.from_lists(
+    [if1, if2],
+    [of1, of2],
+    [],
+)
+
+domain4 = Domain.from_lists(
+    [if1, if2, if3, if4],
+    [of1, of2],
+    [],
+)
+domain5 = Domain.from_lists(
+    [if1, if5],
+    [of1, of2],
+    [],
+)
+domain6 = Domain.from_lists(
+    [if1, if6],
+    [of1, of2],
+)
+domain7 = Domain.from_lists(
+    [if1, if5],
+    [of1, of2],
+    constraints=[
+        LinearEqualityConstraint(features=["cont", "if5"], coefficients=[1, 1], rhs=500)
+    ],
 )
 
 domains = [domain0, domain1, domain2, domain3, domain4]
 
 
 @pytest.mark.parametrize(
     "domain, experiments",
@@ -283,20 +255,20 @@
 
 
 @pytest.mark.parametrize(
     "domain, candidates",
     [
         (d, generate_candidates(d).drop(key, axis=1))
         for d in [domain0]
-        for key in d.get_feature_keys(InputFeature)
+        for key in d.get_feature_keys(Input)
     ]
     + [
         (d, generate_candidates(d).drop(key, axis=1))
         for d in [domain0]
-        for key_ in d.get_feature_keys(OutputFeature)
+        for key_ in d.get_feature_keys(Output)
         for key in [f"{key_}_pred", f"{key_}_sd", f"{key_}_des"]
     ],
 )
 def test_domain_validate_candidates_missing_cols(
     domain: Domain,
     candidates: pd.DataFrame,
 ):
@@ -347,24 +319,32 @@
 
 
 @pytest.mark.parametrize(
     "domain, candidates, key",
     [
         (d, generate_candidates(d), key)
         for d in domains
-        for key in d.get_feature_keys(InputFeature)
+        for key in d.get_feature_keys(Input)
     ]
     + [
         (d, generate_candidates(d), key)
         for d in domains
-        for key_ in d.get_feature_keys(ContinuousOutputFeature)
+        for key_ in d.get_feature_keys(ContinuousOutput)
         for key in [f"{key_}_pred", f"{key_}_sd", f"{key_}_des"]
     ],
 )
 def test_domain_validate_candidates_not_numerical(
     domain: Domain,
     candidates: pd.DataFrame,
     key: str,
 ):
     candidates[key] = str(uuid.uuid4())
     with pytest.raises(ValueError):
         domain.validate_candidates(candidates)
+
+
+@pytest.mark.parametrize(
+    "domain, candidates", [(d, generate_candidates(d)) for d in [domain7]]
+)
+def test_domain_validate_candidates_constraint_not_fulfilled(domain, candidates):
+    with pytest.raises(ValueError):
+        domain.validate_candidates(candidates)
```

### Comparing `bofire-0.0.3/tests/conftest.py` & `bofire-0.0.4/tests/conftest.py`

 * *Files identical despite different names*

