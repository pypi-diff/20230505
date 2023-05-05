# Comparing `tmp/cornflow-client-1.0.8.tar.gz` & `tmp/cornflow-client-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/cornflow-client-1.0.8.tar", last modified: Mon Mar  6 09:05:53 2023, max compression
+gzip compressed data, was "dist/cornflow-client-1.0.9.tar", last modified: Mon Mar  6 09:54:00 2023, max compression
```

## Comparing `cornflow-client-1.0.8.tar` & `cornflow-client-1.0.9.tar`

### file list

```diff
@@ -1,74 +1,74 @@
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-03-06 09:05:53.000000 cornflow-client-1.0.8/
--rw-r--r--   0 runner    (1001) docker     (116)    10766 2023-03-06 09:05:52.000000 cornflow-client-1.0.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (116)      139 2023-03-06 09:05:52.000000 cornflow-client-1.0.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (116)     1754 2023-03-06 09:05:53.000000 cornflow-client-1.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)      923 2023-03-06 09:05:52.000000 cornflow-client-1.0.8/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-03-06 09:05:53.000000 cornflow-client-1.0.8/cornflow_client/
--rw-r--r--   0 runner    (1001) docker     (116)      411 2023-03-06 09:05:52.000000 cornflow-client-1.0.8/cornflow_client/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-03-06 09:05:53.000000 cornflow-client-1.0.8/cornflow_client/airflow/
--rw-r--r--   0 runner    (1001) docker     (116)        0 2023-03-06 09:05:52.000000 cornflow-client-1.0.8/cornflow_client/airflow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     5830 2023-03-06 09:05:52.000000 cornflow-client-1.0.8/cornflow_client/airflow/api.py
--rw-r--r--   0 runner    (1001) docker     (116)    10497 2023-03-06 09:05:52.000000 cornflow-client-1.0.8/cornflow_client/airflow/dag_utilities.py
--rw-r--r--   0 runner    (1001) docker     (116)     7982 2023-03-06 09:05:52.000000 cornflow-client-1.0.8/cornflow_client/constants.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-03-06 09:05:53.000000 cornflow-client-1.0.8/cornflow_client/core/
--rw-r--r--   0 runner    (1001) docker     (116)      202 2023-03-06 09:05:52.000000 cornflow-client-1.0.8/cornflow_client/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     8482 2023-03-06 09:05:52.000000 cornflow-client-1.0.8/cornflow_client/core/application.py
--rw-r--r--   0 runner    (1001) docker     (116)     1984 2023-03-06 09:05:52.000000 cornflow-client-1.0.8/cornflow_client/core/experiment.py
--rw-r--r--   0 runner    (1001) docker     (116)      839 2023-03-06 09:05:52.000000 cornflow-client-1.0.8/cornflow_client/core/instance.py
--rw-r--r--   0 runner    (1001) docker     (116)    14662 2023-03-06 09:05:52.000000 cornflow-client-1.0.8/cornflow_client/core/instance_solution.py
--rw-r--r--   0 runner    (1001) docker     (116)     2824 2023-03-06 09:05:52.000000 cornflow-client-1.0.8/cornflow_client/core/read_tools.py
--rw-r--r--   0 runner    (1001) docker     (116)      234 2023-03-06 09:05:52.000000 cornflow-client-1.0.8/cornflow_client/core/solution.py
--rw-r--r--   0 runner    (1001) docker     (116)      552 2023-03-06 09:05:52.000000 cornflow-client-1.0.8/cornflow_client/core/tools.py
--rw-r--r--   0 runner    (1001) docker     (116)     5496 2023-03-06 09:05:52.000000 cornflow-client-1.0.8/cornflow_client/cornflow_client.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-03-06 09:05:53.000000 cornflow-client-1.0.8/cornflow_client/data/
--rw-r--r--   0 runner    (1001) docker     (116)        0 2023-03-06 09:05:52.000000 cornflow-client-1.0.8/cornflow_client/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)      121 2023-03-06 09:05:52.000000 cornflow-client-1.0.8/cornflow_client/data/empty_schema.json
--rw-r--r--   0 runner    (1001) docker     (116)     2273 2023-03-06 09:05:52.000000 cornflow-client-1.0.8/cornflow_client/data/pulp_json_schema.json
--rw-r--r--   0 runner    (1001) docker     (116)     5549 2023-03-06 09:05:52.000000 cornflow-client-1.0.8/cornflow_client/data/schema_validator.json
--rw-r--r--   0 runner    (1001) docker     (116)      819 2023-03-06 09:05:52.000000 cornflow-client-1.0.8/cornflow_client/data/solver_config.json
--rw-r--r--   0 runner    (1001) docker     (116)      476 2023-03-06 09:05:52.000000 cornflow-client-1.0.8/cornflow_client/data/vrp_solution_schema.json
--rw-r--r--   0 runner    (1001) docker     (116)    30049 2023-03-06 09:05:52.000000 cornflow-client-1.0.8/cornflow_client/raw_cornflow_client.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-03-06 09:05:53.000000 cornflow-client-1.0.8/cornflow_client/schema/
--rw-r--r--   0 runner    (1001) docker     (116)        0 2023-03-06 09:05:52.000000 cornflow-client-1.0.8/cornflow_client/schema/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)    10903 2023-03-06 09:05:52.000000 cornflow-client-1.0.8/cornflow_client/schema/dictSchema.py
--rw-r--r--   0 runner    (1001) docker     (116)     3610 2023-03-06 09:05:52.000000 cornflow-client-1.0.8/cornflow_client/schema/dict_functions.py
--rw-r--r--   0 runner    (1001) docker     (116)     9404 2023-03-06 09:05:52.000000 cornflow-client-1.0.8/cornflow_client/schema/manager.py
--rw-r--r--   0 runner    (1001) docker     (116)     2200 2023-03-06 09:05:52.000000 cornflow-client-1.0.8/cornflow_client/schema/tools.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-03-06 09:05:53.000000 cornflow-client-1.0.8/cornflow_client/tests/
--rw-r--r--   0 runner    (1001) docker     (116)        0 2023-03-06 09:05:52.000000 cornflow-client-1.0.8/cornflow_client/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     5016 2023-03-06 09:05:52.000000 cornflow-client-1.0.8/cornflow_client/tests/const.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-03-06 09:05:53.000000 cornflow-client-1.0.8/cornflow_client/tests/data/
--rw-r--r--   0 runner    (1001) docker     (116)        0 2023-03-06 09:05:52.000000 cornflow-client-1.0.8/cornflow_client/tests/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)    30894 2023-03-06 09:05:52.000000 cornflow-client-1.0.8/cornflow_client/tests/data/data_input_bad.json
--rw-r--r--   0 runner    (1001) docker     (116)     1319 2023-03-06 09:05:52.000000 cornflow-client-1.0.8/cornflow_client/tests/data/data_schema.json
--rw-r--r--   0 runner    (1001) docker     (116)     3425 2023-03-06 09:05:52.000000 cornflow-client-1.0.8/cornflow_client/tests/data/gc_input.json
--rw-r--r--   0 runner    (1001) docker     (116)     1513 2023-03-06 09:05:52.000000 cornflow-client-1.0.8/cornflow_client/tests/data/gc_output.json
--rw-r--r--   0 runner    (1001) docker     (116)      611 2023-03-06 09:05:52.000000 cornflow-client-1.0.8/cornflow_client/tests/data/graph_coloring_input.json
--rw-r--r--   0 runner    (1001) docker     (116)      376 2023-03-06 09:05:52.000000 cornflow-client-1.0.8/cornflow_client/tests/data/graph_coloring_output.json
--rw-r--r--   0 runner    (1001) docker     (116)    30946 2023-03-06 09:05:52.000000 cornflow-client-1.0.8/cornflow_client/tests/data/hk_data_input.json
--rw-r--r--   0 runner    (1001) docker     (116)     1611 2023-03-06 09:05:52.000000 cornflow-client-1.0.8/cornflow_client/tests/data/hk_data_schema.json
--rw-r--r--   0 runner    (1001) docker     (116)      437 2023-03-06 09:05:52.000000 cornflow-client-1.0.8/cornflow_client/tests/data/hk_solution_schema.json
--rw-r--r--   0 runner    (1001) docker     (116)     1495 2023-03-06 09:05:52.000000 cornflow-client-1.0.8/cornflow_client/tests/data/instance-hackathon2.json
--rw-r--r--   0 runner    (1001) docker     (116)     1669 2023-03-06 09:05:52.000000 cornflow-client-1.0.8/cornflow_client/tests/data/name_problem_schema.json
--rw-r--r--   0 runner    (1001) docker     (116)   550476 2023-03-06 09:05:52.000000 cornflow-client-1.0.8/cornflow_client/tests/data/pulp_example_data.json
--rw-r--r--   0 runner    (1001) docker     (116)      911 2023-03-06 09:05:52.000000 cornflow-client-1.0.8/cornflow_client/tests/data/test_mps.mps
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-03-06 09:05:53.000000 cornflow-client-1.0.8/cornflow_client/tests/integration/
--rw-r--r--   0 runner    (1001) docker     (116)        0 2023-03-06 09:05:52.000000 cornflow-client-1.0.8/cornflow_client/tests/integration/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     2644 2023-03-06 09:05:52.000000 cornflow-client-1.0.8/cornflow_client/tests/integration/test_airflow_integration.py
--rw-r--r--   0 runner    (1001) docker     (116)    20676 2023-03-06 09:05:52.000000 cornflow-client-1.0.8/cornflow_client/tests/integration/test_cornflow_integration.py
--rw-r--r--   0 runner    (1001) docker     (116)    23785 2023-03-06 09:05:52.000000 cornflow-client-1.0.8/cornflow_client/tests/integration/test_raw_cornflow_integration.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-03-06 09:05:53.000000 cornflow-client-1.0.8/cornflow_client/tests/unit/
--rw-r--r--   0 runner    (1001) docker     (116)        0 2023-03-06 09:05:52.000000 cornflow-client-1.0.8/cornflow_client/tests/unit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     3739 2023-03-06 09:05:52.000000 cornflow-client-1.0.8/cornflow_client/tests/unit/test_abc.py
--rw-r--r--   0 runner    (1001) docker     (116)     1734 2023-03-06 09:05:52.000000 cornflow-client-1.0.8/cornflow_client/tests/unit/test_dag_utilities.py
--rw-r--r--   0 runner    (1001) docker     (116)    14225 2023-03-06 09:05:52.000000 cornflow-client-1.0.8/cornflow_client/tests/unit/test_instance_solution_methods.py
--rw-r--r--   0 runner    (1001) docker     (116)     9473 2023-03-06 09:05:52.000000 cornflow-client-1.0.8/cornflow_client/tests/unit/test_schema_manager.py
--rw-r--r--   0 runner    (1001) docker     (116)     4852 2023-03-06 09:05:52.000000 cornflow-client-1.0.8/cornflow_client/tests/unit/test_varnames.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-03-06 09:05:53.000000 cornflow-client-1.0.8/cornflow_client.egg-info/
--rw-r--r--   0 runner    (1001) docker     (116)     1754 2023-03-06 09:05:53.000000 cornflow-client-1.0.8/cornflow_client.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)     2415 2023-03-06 09:05:53.000000 cornflow-client-1.0.8/cornflow_client.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (116)        1 2023-03-06 09:05:53.000000 cornflow-client-1.0.8/cornflow_client.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (116)       64 2023-03-06 09:05:53.000000 cornflow-client-1.0.8/cornflow_client.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (116)       16 2023-03-06 09:05:53.000000 cornflow-client-1.0.8/cornflow_client.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (116)       38 2023-03-06 09:05:53.000000 cornflow-client-1.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (116)      983 2023-03-06 09:05:52.000000 cornflow-client-1.0.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-03-06 09:54:00.000000 cornflow-client-1.0.9/
+-rw-r--r--   0 runner    (1001) docker     (116)    10766 2023-03-06 09:53:58.000000 cornflow-client-1.0.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (116)      139 2023-03-06 09:53:58.000000 cornflow-client-1.0.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (116)     1754 2023-03-06 09:54:00.000000 cornflow-client-1.0.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (116)      923 2023-03-06 09:53:58.000000 cornflow-client-1.0.9/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-03-06 09:54:00.000000 cornflow-client-1.0.9/cornflow_client/
+-rw-r--r--   0 runner    (1001) docker     (116)      411 2023-03-06 09:53:58.000000 cornflow-client-1.0.9/cornflow_client/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-03-06 09:54:00.000000 cornflow-client-1.0.9/cornflow_client/airflow/
+-rw-r--r--   0 runner    (1001) docker     (116)        0 2023-03-06 09:53:58.000000 cornflow-client-1.0.9/cornflow_client/airflow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)     5264 2023-03-06 09:53:58.000000 cornflow-client-1.0.9/cornflow_client/airflow/api.py
+-rw-r--r--   0 runner    (1001) docker     (116)    10497 2023-03-06 09:53:58.000000 cornflow-client-1.0.9/cornflow_client/airflow/dag_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (116)     7982 2023-03-06 09:53:58.000000 cornflow-client-1.0.9/cornflow_client/constants.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-03-06 09:54:00.000000 cornflow-client-1.0.9/cornflow_client/core/
+-rw-r--r--   0 runner    (1001) docker     (116)      202 2023-03-06 09:53:58.000000 cornflow-client-1.0.9/cornflow_client/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)     8482 2023-03-06 09:53:58.000000 cornflow-client-1.0.9/cornflow_client/core/application.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1984 2023-03-06 09:53:58.000000 cornflow-client-1.0.9/cornflow_client/core/experiment.py
+-rw-r--r--   0 runner    (1001) docker     (116)      839 2023-03-06 09:53:58.000000 cornflow-client-1.0.9/cornflow_client/core/instance.py
+-rw-r--r--   0 runner    (1001) docker     (116)    14662 2023-03-06 09:53:58.000000 cornflow-client-1.0.9/cornflow_client/core/instance_solution.py
+-rw-r--r--   0 runner    (1001) docker     (116)     2824 2023-03-06 09:53:58.000000 cornflow-client-1.0.9/cornflow_client/core/read_tools.py
+-rw-r--r--   0 runner    (1001) docker     (116)      234 2023-03-06 09:53:58.000000 cornflow-client-1.0.9/cornflow_client/core/solution.py
+-rw-r--r--   0 runner    (1001) docker     (116)      552 2023-03-06 09:53:58.000000 cornflow-client-1.0.9/cornflow_client/core/tools.py
+-rw-r--r--   0 runner    (1001) docker     (116)     5496 2023-03-06 09:53:58.000000 cornflow-client-1.0.9/cornflow_client/cornflow_client.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-03-06 09:54:00.000000 cornflow-client-1.0.9/cornflow_client/data/
+-rw-r--r--   0 runner    (1001) docker     (116)        0 2023-03-06 09:53:58.000000 cornflow-client-1.0.9/cornflow_client/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)      121 2023-03-06 09:53:58.000000 cornflow-client-1.0.9/cornflow_client/data/empty_schema.json
+-rw-r--r--   0 runner    (1001) docker     (116)     2273 2023-03-06 09:53:58.000000 cornflow-client-1.0.9/cornflow_client/data/pulp_json_schema.json
+-rw-r--r--   0 runner    (1001) docker     (116)     5549 2023-03-06 09:53:58.000000 cornflow-client-1.0.9/cornflow_client/data/schema_validator.json
+-rw-r--r--   0 runner    (1001) docker     (116)      819 2023-03-06 09:53:58.000000 cornflow-client-1.0.9/cornflow_client/data/solver_config.json
+-rw-r--r--   0 runner    (1001) docker     (116)      476 2023-03-06 09:53:58.000000 cornflow-client-1.0.9/cornflow_client/data/vrp_solution_schema.json
+-rw-r--r--   0 runner    (1001) docker     (116)    30049 2023-03-06 09:53:58.000000 cornflow-client-1.0.9/cornflow_client/raw_cornflow_client.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-03-06 09:54:00.000000 cornflow-client-1.0.9/cornflow_client/schema/
+-rw-r--r--   0 runner    (1001) docker     (116)        0 2023-03-06 09:53:58.000000 cornflow-client-1.0.9/cornflow_client/schema/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)    10903 2023-03-06 09:53:58.000000 cornflow-client-1.0.9/cornflow_client/schema/dictSchema.py
+-rw-r--r--   0 runner    (1001) docker     (116)     3610 2023-03-06 09:53:58.000000 cornflow-client-1.0.9/cornflow_client/schema/dict_functions.py
+-rw-r--r--   0 runner    (1001) docker     (116)     9404 2023-03-06 09:53:58.000000 cornflow-client-1.0.9/cornflow_client/schema/manager.py
+-rw-r--r--   0 runner    (1001) docker     (116)     2200 2023-03-06 09:53:58.000000 cornflow-client-1.0.9/cornflow_client/schema/tools.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-03-06 09:54:00.000000 cornflow-client-1.0.9/cornflow_client/tests/
+-rw-r--r--   0 runner    (1001) docker     (116)        0 2023-03-06 09:53:58.000000 cornflow-client-1.0.9/cornflow_client/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)     5016 2023-03-06 09:53:58.000000 cornflow-client-1.0.9/cornflow_client/tests/const.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-03-06 09:54:00.000000 cornflow-client-1.0.9/cornflow_client/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (116)        0 2023-03-06 09:53:58.000000 cornflow-client-1.0.9/cornflow_client/tests/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)    30894 2023-03-06 09:53:58.000000 cornflow-client-1.0.9/cornflow_client/tests/data/data_input_bad.json
+-rw-r--r--   0 runner    (1001) docker     (116)     1319 2023-03-06 09:53:58.000000 cornflow-client-1.0.9/cornflow_client/tests/data/data_schema.json
+-rw-r--r--   0 runner    (1001) docker     (116)     3425 2023-03-06 09:53:58.000000 cornflow-client-1.0.9/cornflow_client/tests/data/gc_input.json
+-rw-r--r--   0 runner    (1001) docker     (116)     1513 2023-03-06 09:53:58.000000 cornflow-client-1.0.9/cornflow_client/tests/data/gc_output.json
+-rw-r--r--   0 runner    (1001) docker     (116)      611 2023-03-06 09:53:58.000000 cornflow-client-1.0.9/cornflow_client/tests/data/graph_coloring_input.json
+-rw-r--r--   0 runner    (1001) docker     (116)      376 2023-03-06 09:53:58.000000 cornflow-client-1.0.9/cornflow_client/tests/data/graph_coloring_output.json
+-rw-r--r--   0 runner    (1001) docker     (116)    30946 2023-03-06 09:53:58.000000 cornflow-client-1.0.9/cornflow_client/tests/data/hk_data_input.json
+-rw-r--r--   0 runner    (1001) docker     (116)     1611 2023-03-06 09:53:58.000000 cornflow-client-1.0.9/cornflow_client/tests/data/hk_data_schema.json
+-rw-r--r--   0 runner    (1001) docker     (116)      437 2023-03-06 09:53:58.000000 cornflow-client-1.0.9/cornflow_client/tests/data/hk_solution_schema.json
+-rw-r--r--   0 runner    (1001) docker     (116)     1495 2023-03-06 09:53:58.000000 cornflow-client-1.0.9/cornflow_client/tests/data/instance-hackathon2.json
+-rw-r--r--   0 runner    (1001) docker     (116)     1669 2023-03-06 09:53:58.000000 cornflow-client-1.0.9/cornflow_client/tests/data/name_problem_schema.json
+-rw-r--r--   0 runner    (1001) docker     (116)   550476 2023-03-06 09:53:58.000000 cornflow-client-1.0.9/cornflow_client/tests/data/pulp_example_data.json
+-rw-r--r--   0 runner    (1001) docker     (116)      911 2023-03-06 09:53:58.000000 cornflow-client-1.0.9/cornflow_client/tests/data/test_mps.mps
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-03-06 09:54:00.000000 cornflow-client-1.0.9/cornflow_client/tests/integration/
+-rw-r--r--   0 runner    (1001) docker     (116)        0 2023-03-06 09:53:58.000000 cornflow-client-1.0.9/cornflow_client/tests/integration/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)     2644 2023-03-06 09:53:58.000000 cornflow-client-1.0.9/cornflow_client/tests/integration/test_airflow_integration.py
+-rw-r--r--   0 runner    (1001) docker     (116)    20676 2023-03-06 09:53:58.000000 cornflow-client-1.0.9/cornflow_client/tests/integration/test_cornflow_integration.py
+-rw-r--r--   0 runner    (1001) docker     (116)    23785 2023-03-06 09:53:58.000000 cornflow-client-1.0.9/cornflow_client/tests/integration/test_raw_cornflow_integration.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-03-06 09:54:00.000000 cornflow-client-1.0.9/cornflow_client/tests/unit/
+-rw-r--r--   0 runner    (1001) docker     (116)        0 2023-03-06 09:53:58.000000 cornflow-client-1.0.9/cornflow_client/tests/unit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (116)     3739 2023-03-06 09:53:58.000000 cornflow-client-1.0.9/cornflow_client/tests/unit/test_abc.py
+-rw-r--r--   0 runner    (1001) docker     (116)     1734 2023-03-06 09:53:58.000000 cornflow-client-1.0.9/cornflow_client/tests/unit/test_dag_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (116)    14225 2023-03-06 09:53:58.000000 cornflow-client-1.0.9/cornflow_client/tests/unit/test_instance_solution_methods.py
+-rw-r--r--   0 runner    (1001) docker     (116)     9473 2023-03-06 09:53:58.000000 cornflow-client-1.0.9/cornflow_client/tests/unit/test_schema_manager.py
+-rw-r--r--   0 runner    (1001) docker     (116)     4852 2023-03-06 09:53:58.000000 cornflow-client-1.0.9/cornflow_client/tests/unit/test_varnames.py
+drwxr-xr-x   0 runner    (1001) docker     (116)        0 2023-03-06 09:54:00.000000 cornflow-client-1.0.9/cornflow_client.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (116)     1754 2023-03-06 09:54:00.000000 cornflow-client-1.0.9/cornflow_client.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (116)     2415 2023-03-06 09:54:00.000000 cornflow-client-1.0.9/cornflow_client.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (116)        1 2023-03-06 09:54:00.000000 cornflow-client-1.0.9/cornflow_client.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (116)       64 2023-03-06 09:54:00.000000 cornflow-client-1.0.9/cornflow_client.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (116)       16 2023-03-06 09:54:00.000000 cornflow-client-1.0.9/cornflow_client.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (116)       38 2023-03-06 09:54:00.000000 cornflow-client-1.0.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (116)      983 2023-03-06 09:53:58.000000 cornflow-client-1.0.9/setup.py
```

### Comparing `cornflow-client-1.0.8/LICENSE` & `cornflow-client-1.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `cornflow-client-1.0.8/PKG-INFO` & `cornflow-client-1.0.9/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cornflow-client
-Version: 1.0.8
+Version: 1.0.9
 Summary: Client to connect to a cornflow server
 Home-page: https://github.com/baobabsoluciones/cornflow
 Author: baobab soluciones
 Author-email: sistemas@baobabsoluciones.es
 License: UNKNOWN
 Description: Cornflow client
         ================
```

### Comparing `cornflow-client-1.0.8/README.rst` & `cornflow-client-1.0.9/README.rst`

 * *Files identical despite different names*

### Comparing `cornflow-client-1.0.8/cornflow_client/airflow/api.py` & `cornflow-client-1.0.9/cornflow_client/airflow/api.py`

 * *Files 17% similar despite different names*

```diff
@@ -3,20 +3,18 @@
 """
 
 # Full imports
 import json
 import requests
 
 # Partial imports
-from marshmallow import ValidationError
 from requests.auth import HTTPBasicAuth
 from requests.exceptions import ConnectionError, HTTPError
 
 # Imports from modules
-from cornflow_client import SchemaManager
 from cornflow_client.constants import AirflowError
 
 
 class Airflow(object):
     def __init__(self, url, user, pwd):
         self.url = f"{url}/api/v1"
         self.auth = HTTPBasicAuth(user, pwd)
@@ -142,22 +140,7 @@
     def get_internal_dags(self, method="GET"):
         url = f"{self.url}/dags?tags=internal"
         return self.request_headers_auth(method=method, url=url)
 
     def get_model_dags(self, method="GET"):
         url = f"{self.url}/dags?tags=model"
         return self.request_headers_auth(method=method, url=url)
-
-
-def get_schema(config, dag_name, schema="instance"):
-    """
-    Gets a schema by name from airflow server. We use the variable api.
-    We transform the jsonschema into a marshmallow class
-
-    """
-    af_client = Airflow.from_config(config)
-    if not af_client.is_alive():
-        raise AirflowError(error="Airflow is not accessible")
-
-    schema_json = af_client.get_one_schema(dag_name, schema)
-    manager = SchemaManager(schema_json)
-    return manager.jsonschema_to_flask()
```

### Comparing `cornflow-client-1.0.8/cornflow_client/airflow/dag_utilities.py` & `cornflow-client-1.0.9/cornflow_client/airflow/dag_utilities.py`

 * *Files identical despite different names*

### Comparing `cornflow-client-1.0.8/cornflow_client/constants.py` & `cornflow-client-1.0.9/cornflow_client/constants.py`

 * *Files identical despite different names*

### Comparing `cornflow-client-1.0.8/cornflow_client/core/application.py` & `cornflow-client-1.0.9/cornflow_client/core/application.py`

 * *Files identical despite different names*

### Comparing `cornflow-client-1.0.8/cornflow_client/core/experiment.py` & `cornflow-client-1.0.9/cornflow_client/core/experiment.py`

 * *Files identical despite different names*

### Comparing `cornflow-client-1.0.8/cornflow_client/core/instance.py` & `cornflow-client-1.0.9/cornflow_client/core/instance.py`

 * *Files identical despite different names*

### Comparing `cornflow-client-1.0.8/cornflow_client/core/instance_solution.py` & `cornflow-client-1.0.9/cornflow_client/core/instance_solution.py`

 * *Files identical despite different names*

### Comparing `cornflow-client-1.0.8/cornflow_client/core/read_tools.py` & `cornflow-client-1.0.9/cornflow_client/core/read_tools.py`

 * *Files identical despite different names*

### Comparing `cornflow-client-1.0.8/cornflow_client/core/tools.py` & `cornflow-client-1.0.9/cornflow_client/core/tools.py`

 * *Files identical despite different names*

### Comparing `cornflow-client-1.0.8/cornflow_client/cornflow_client.py` & `cornflow-client-1.0.9/cornflow_client/cornflow_client.py`

 * *Files identical despite different names*

### Comparing `cornflow-client-1.0.8/cornflow_client/data/pulp_json_schema.json` & `cornflow-client-1.0.9/cornflow_client/data/pulp_json_schema.json`

 * *Files identical despite different names*

### Comparing `cornflow-client-1.0.8/cornflow_client/data/schema_validator.json` & `cornflow-client-1.0.9/cornflow_client/data/schema_validator.json`

 * *Files identical despite different names*

### Comparing `cornflow-client-1.0.8/cornflow_client/data/solver_config.json` & `cornflow-client-1.0.9/cornflow_client/data/solver_config.json`

 * *Files identical despite different names*

### Comparing `cornflow-client-1.0.8/cornflow_client/raw_cornflow_client.py` & `cornflow-client-1.0.9/cornflow_client/raw_cornflow_client.py`

 * *Files identical despite different names*

### Comparing `cornflow-client-1.0.8/cornflow_client/schema/dictSchema.py` & `cornflow-client-1.0.9/cornflow_client/schema/dictSchema.py`

 * *Files identical despite different names*

### Comparing `cornflow-client-1.0.8/cornflow_client/schema/dict_functions.py` & `cornflow-client-1.0.9/cornflow_client/schema/dict_functions.py`

 * *Files identical despite different names*

### Comparing `cornflow-client-1.0.8/cornflow_client/schema/manager.py` & `cornflow-client-1.0.9/cornflow_client/schema/manager.py`

 * *Files identical despite different names*

### Comparing `cornflow-client-1.0.8/cornflow_client/schema/tools.py` & `cornflow-client-1.0.9/cornflow_client/schema/tools.py`

 * *Files identical despite different names*

### Comparing `cornflow-client-1.0.8/cornflow_client/tests/const.py` & `cornflow-client-1.0.9/cornflow_client/tests/const.py`

 * *Files identical despite different names*

### Comparing `cornflow-client-1.0.8/cornflow_client/tests/data/data_input_bad.json` & `cornflow-client-1.0.9/cornflow_client/tests/data/data_input_bad.json`

 * *Files identical despite different names*

### Comparing `cornflow-client-1.0.8/cornflow_client/tests/data/data_schema.json` & `cornflow-client-1.0.9/cornflow_client/tests/data/data_schema.json`

 * *Files identical despite different names*

### Comparing `cornflow-client-1.0.8/cornflow_client/tests/data/gc_input.json` & `cornflow-client-1.0.9/cornflow_client/tests/data/gc_input.json`

 * *Files identical despite different names*

### Comparing `cornflow-client-1.0.8/cornflow_client/tests/data/gc_output.json` & `cornflow-client-1.0.9/cornflow_client/tests/data/gc_output.json`

 * *Files identical despite different names*

### Comparing `cornflow-client-1.0.8/cornflow_client/tests/data/graph_coloring_input.json` & `cornflow-client-1.0.9/cornflow_client/tests/data/graph_coloring_input.json`

 * *Files identical despite different names*

### Comparing `cornflow-client-1.0.8/cornflow_client/tests/data/hk_data_input.json` & `cornflow-client-1.0.9/cornflow_client/tests/data/hk_data_input.json`

 * *Files identical despite different names*

### Comparing `cornflow-client-1.0.8/cornflow_client/tests/data/hk_data_schema.json` & `cornflow-client-1.0.9/cornflow_client/tests/data/hk_data_schema.json`

 * *Files identical despite different names*

### Comparing `cornflow-client-1.0.8/cornflow_client/tests/data/instance-hackathon2.json` & `cornflow-client-1.0.9/cornflow_client/tests/data/instance-hackathon2.json`

 * *Files identical despite different names*

### Comparing `cornflow-client-1.0.8/cornflow_client/tests/data/name_problem_schema.json` & `cornflow-client-1.0.9/cornflow_client/tests/data/name_problem_schema.json`

 * *Files identical despite different names*

### Comparing `cornflow-client-1.0.8/cornflow_client/tests/data/pulp_example_data.json` & `cornflow-client-1.0.9/cornflow_client/tests/data/pulp_example_data.json`

 * *Files identical despite different names*

### Comparing `cornflow-client-1.0.8/cornflow_client/tests/data/test_mps.mps` & `cornflow-client-1.0.9/cornflow_client/tests/data/test_mps.mps`

 * *Files identical despite different names*

### Comparing `cornflow-client-1.0.8/cornflow_client/tests/integration/test_airflow_integration.py` & `cornflow-client-1.0.9/cornflow_client/tests/integration/test_airflow_integration.py`

 * *Files identical despite different names*

### Comparing `cornflow-client-1.0.8/cornflow_client/tests/integration/test_cornflow_integration.py` & `cornflow-client-1.0.9/cornflow_client/tests/integration/test_cornflow_integration.py`

 * *Files identical despite different names*

### Comparing `cornflow-client-1.0.8/cornflow_client/tests/integration/test_raw_cornflow_integration.py` & `cornflow-client-1.0.9/cornflow_client/tests/integration/test_raw_cornflow_integration.py`

 * *Files identical despite different names*

### Comparing `cornflow-client-1.0.8/cornflow_client/tests/unit/test_abc.py` & `cornflow-client-1.0.9/cornflow_client/tests/unit/test_abc.py`

 * *Files identical despite different names*

### Comparing `cornflow-client-1.0.8/cornflow_client/tests/unit/test_dag_utilities.py` & `cornflow-client-1.0.9/cornflow_client/tests/unit/test_dag_utilities.py`

 * *Files identical despite different names*

### Comparing `cornflow-client-1.0.8/cornflow_client/tests/unit/test_instance_solution_methods.py` & `cornflow-client-1.0.9/cornflow_client/tests/unit/test_instance_solution_methods.py`

 * *Files identical despite different names*

### Comparing `cornflow-client-1.0.8/cornflow_client/tests/unit/test_schema_manager.py` & `cornflow-client-1.0.9/cornflow_client/tests/unit/test_schema_manager.py`

 * *Files identical despite different names*

### Comparing `cornflow-client-1.0.8/cornflow_client/tests/unit/test_varnames.py` & `cornflow-client-1.0.9/cornflow_client/tests/unit/test_varnames.py`

 * *Files identical despite different names*

### Comparing `cornflow-client-1.0.8/cornflow_client.egg-info/PKG-INFO` & `cornflow-client-1.0.9/cornflow_client.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cornflow-client
-Version: 1.0.8
+Version: 1.0.9
 Summary: Client to connect to a cornflow server
 Home-page: https://github.com/baobabsoluciones/cornflow
 Author: baobab soluciones
 Author-email: sistemas@baobabsoluciones.es
 License: UNKNOWN
 Description: Cornflow client
         ================
```

### Comparing `cornflow-client-1.0.8/cornflow_client.egg-info/SOURCES.txt` & `cornflow-client-1.0.9/cornflow_client.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cornflow-client-1.0.8/setup.py` & `cornflow-client-1.0.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
     required.append(fh.read().splitlines())
 
 extra_required = {"excel": ["openpyxl", "pandas"]}
 
 
 setuptools.setup(
     name="cornflow-client",
-    version="1.0.8",
+    version="1.0.9",
     author="baobab soluciones",
     author_email="sistemas@baobabsoluciones.es",
     description="Client to connect to a cornflow server",
     long_description=long_description,
     long_description_content_type="text/x-rst",
     url="https://github.com/baobabsoluciones/cornflow",
     packages=setuptools.find_packages(),
```

