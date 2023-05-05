# Comparing `tmp/kedro_snowflake-0.1.1.tar.gz` & `tmp/kedro_snowflake-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kedro_snowflake-0.1.1.tar", max compression
+gzip compressed data, was "kedro_snowflake-0.1.2.tar", max compression
```

## Comparing `kedro_snowflake-0.1.1.tar` & `kedro_snowflake-0.1.2.tar`

### file list

```diff
@@ -1,66 +1,66 @@
--rw-r--r--   0        0        0    11338 2023-04-26 15:35:24.929358 kedro_snowflake-0.1.1/LICENSE
--rw-r--r--   0        0        0     4510 2023-04-26 15:35:24.929358 kedro_snowflake-0.1.1/README.md
--rw-r--r--   0        0        0       22 2023-04-26 15:35:24.933359 kedro_snowflake-0.1.1/kedro_snowflake/__init__.py
--rw-r--r--   0        0        0     4523 2023-04-26 15:35:24.933359 kedro_snowflake-0.1.1/kedro_snowflake/cli.py
--rw-r--r--   0        0        0     2282 2023-04-26 15:35:24.933359 kedro_snowflake-0.1.1/kedro_snowflake/cli_functions.py
--rw-r--r--   0        0        0     4444 2023-04-26 15:35:24.933359 kedro_snowflake-0.1.1/kedro_snowflake/config.py
--rw-r--r--   0        0        0        0 2023-04-26 15:35:24.933359 kedro_snowflake-0.1.1/kedro_snowflake/datasets/__init__.py
--rw-r--r--   0        0        0     5483 2023-04-26 15:35:24.933359 kedro_snowflake-0.1.1/kedro_snowflake/datasets/internal.py
--rw-r--r--   0        0        0     5660 2023-04-26 15:35:24.933359 kedro_snowflake-0.1.1/kedro_snowflake/datasets/native.py
--rw-r--r--   0        0        0    14301 2023-04-26 15:35:24.933359 kedro_snowflake-0.1.1/kedro_snowflake/generator.py
--rw-r--r--   0        0        0      119 2023-04-26 15:35:24.933359 kedro_snowflake-0.1.1/kedro_snowflake/misc.py
--rw-r--r--   0        0        0     3504 2023-04-26 15:35:24.933359 kedro_snowflake-0.1.1/kedro_snowflake/pipeline.py
--rw-r--r--   0        0        0     1526 2023-04-26 15:35:24.933359 kedro_snowflake-0.1.1/kedro_snowflake/runner.py
--rw-r--r--   0        0        0     1612 2023-04-26 15:35:24.933359 kedro_snowflake-0.1.1/kedro_snowflake/starters/snowflights/README.md
--rw-r--r--   0        0        0      524 2023-04-26 15:35:24.933359 kedro_snowflake-0.1.1/kedro_snowflake/starters/snowflights/cookiecutter.json
--rw-r--r--   0        0        0   162747 2023-04-26 15:35:24.933359 kedro_snowflake-0.1.1/kedro_snowflake/starters/snowflights/images/pipeline_visualisation_with_layers.png
--rw-r--r--   0        0        0   162747 2023-04-26 15:35:24.937358 kedro_snowflake-0.1.1/kedro_snowflake/starters/snowflights/pipeline_visualisation_with_layers.png
--rw-r--r--   0        0        0     1927 2023-04-26 15:35:24.937358 kedro_snowflake-0.1.1/kedro_snowflake/starters/snowflights/prompts.yml
--rw-r--r--   0        0        0     1785 2023-04-26 15:35:24.937358 kedro_snowflake-0.1.1/kedro_snowflake/starters/snowflights/{{ cookiecutter.repo_name }}/.gitignore
--rw-r--r--   0        0        0     3958 2023-04-26 15:35:24.937358 kedro_snowflake-0.1.1/kedro_snowflake/starters/snowflights/{{ cookiecutter.repo_name }}/README.md
--rw-r--r--   0        0        0     1083 2023-04-26 15:35:24.937358 kedro_snowflake-0.1.1/kedro_snowflake/starters/snowflights/{{ cookiecutter.repo_name }}/conf/README.md
--rw-r--r--   0        0        0     2778 2023-04-26 15:35:24.937358 kedro_snowflake-0.1.1/kedro_snowflake/starters/snowflights/{{ cookiecutter.repo_name }}/conf/base/catalog.yml
--rw-r--r--   0        0        0      901 2023-04-26 15:35:24.937358 kedro_snowflake-0.1.1/kedro_snowflake/starters/snowflights/{{ cookiecutter.repo_name }}/conf/base/logging.yml
--rw-r--r--   0        0        0        0 2023-04-26 15:35:24.937358 kedro_snowflake-0.1.1/kedro_snowflake/starters/snowflights/{{ cookiecutter.repo_name }}/conf/base/parameters/data_processing.yml
--rw-r--r--   0        0        0      232 2023-04-26 15:35:24.937358 kedro_snowflake-0.1.1/kedro_snowflake/starters/snowflights/{{ cookiecutter.repo_name }}/conf/base/parameters/data_science.yml
--rw-r--r--   0        0        0        0 2023-04-26 15:35:24.937358 kedro_snowflake-0.1.1/kedro_snowflake/starters/snowflights/{{ cookiecutter.repo_name }}/conf/base/parameters.yml
--rw-r--r--   0        0        0     2073 2023-04-26 15:35:24.937358 kedro_snowflake-0.1.1/kedro_snowflake/starters/snowflights/{{ cookiecutter.repo_name }}/conf/base/snowflake.yml
--rw-r--r--   0        0        0        0 2023-04-26 15:35:24.937358 kedro_snowflake-0.1.1/kedro_snowflake/starters/snowflights/{{ cookiecutter.repo_name }}/conf/local/.gitkeep
--rw-r--r--   0        0        0      431 2023-04-26 15:35:24.937358 kedro_snowflake-0.1.1/kedro_snowflake/starters/snowflights/{{ cookiecutter.repo_name }}/conf/local/credentials.yml
--rw-r--r--   0        0        0        0 2023-04-26 15:35:24.937358 kedro_snowflake-0.1.1/kedro_snowflake/starters/snowflights/{{ cookiecutter.repo_name }}/data/01_raw/.gitkeep
--rw-r--r--   0        0        0  1810602 2023-04-26 15:35:24.945359 kedro_snowflake-0.1.1/kedro_snowflake/starters/snowflights/{{ cookiecutter.repo_name }}/data/01_raw/companies.csv
--rw-r--r--   0        0        0  2937144 2023-04-26 15:35:24.957359 kedro_snowflake-0.1.1/kedro_snowflake/starters/snowflights/{{ cookiecutter.repo_name }}/data/01_raw/reviews.csv
--rw-r--r--   0        0        0  4195290 2023-04-26 15:35:24.985359 kedro_snowflake-0.1.1/kedro_snowflake/starters/snowflights/{{ cookiecutter.repo_name }}/data/01_raw/shuttles.xlsx
--rw-r--r--   0        0        0        0 2023-04-26 15:35:24.985359 kedro_snowflake-0.1.1/kedro_snowflake/starters/snowflights/{{ cookiecutter.repo_name }}/data/02_intermediate/.gitkeep
--rw-r--r--   0        0        0        0 2023-04-26 15:35:24.985359 kedro_snowflake-0.1.1/kedro_snowflake/starters/snowflights/{{ cookiecutter.repo_name }}/data/03_primary/.gitkeep
--rw-r--r--   0        0        0        0 2023-04-26 15:35:24.985359 kedro_snowflake-0.1.1/kedro_snowflake/starters/snowflights/{{ cookiecutter.repo_name }}/data/04_feature/.gitkeep
--rw-r--r--   0        0        0        0 2023-04-26 15:35:24.985359 kedro_snowflake-0.1.1/kedro_snowflake/starters/snowflights/{{ cookiecutter.repo_name }}/data/05_model_input/.gitkeep
--rw-r--r--   0        0        0        0 2023-04-26 15:35:24.985359 kedro_snowflake-0.1.1/kedro_snowflake/starters/snowflights/{{ cookiecutter.repo_name }}/data/06_models/.gitkeep
--rw-r--r--   0        0        0        0 2023-04-26 15:35:24.985359 kedro_snowflake-0.1.1/kedro_snowflake/starters/snowflights/{{ cookiecutter.repo_name }}/data/07_model_output/.gitkeep
--rw-r--r--   0        0        0        0 2023-04-26 15:35:24.985359 kedro_snowflake-0.1.1/kedro_snowflake/starters/snowflights/{{ cookiecutter.repo_name }}/data/08_reporting/.gitkeep
--rw-r--r--   0        0        0     6967 2023-04-26 15:35:24.985359 kedro_snowflake-0.1.1/kedro_snowflake/starters/snowflights/{{ cookiecutter.repo_name }}/docs/source/conf.py
--rw-r--r--   0        0        0      459 2023-04-26 15:35:24.985359 kedro_snowflake-0.1.1/kedro_snowflake/starters/snowflights/{{ cookiecutter.repo_name }}/docs/source/index.rst
--rw-r--r--   0        0        0        0 2023-04-26 15:35:24.985359 kedro_snowflake-0.1.1/kedro_snowflake/starters/snowflights/{{ cookiecutter.repo_name }}/logs/.gitkeep
--rw-r--r--   0        0        0        0 2023-04-26 15:35:24.985359 kedro_snowflake-0.1.1/kedro_snowflake/starters/snowflights/{{ cookiecutter.repo_name }}/notebooks/.gitkeep
--rw-r--r--   0        0        0      446 2023-04-26 15:35:24.985359 kedro_snowflake-0.1.1/kedro_snowflake/starters/snowflights/{{ cookiecutter.repo_name }}/pyproject.toml
--rw-r--r--   0        0        0       47 2023-04-26 15:35:24.985359 kedro_snowflake-0.1.1/kedro_snowflake/starters/snowflights/{{ cookiecutter.repo_name }}/setup.cfg
--rw-r--r--   0        0        0      395 2023-04-26 15:35:24.985359 kedro_snowflake-0.1.1/kedro_snowflake/starters/snowflights/{{ cookiecutter.repo_name }}/src/requirements.txt
--rw-r--r--   0        0        0     1198 2023-04-26 15:35:24.985359 kedro_snowflake-0.1.1/kedro_snowflake/starters/snowflights/{{ cookiecutter.repo_name }}/src/setup.py
--rw-r--r--   0        0        0        0 2023-04-26 15:35:24.985359 kedro_snowflake-0.1.1/kedro_snowflake/starters/snowflights/{{ cookiecutter.repo_name }}/src/tests/__init__.py
--rw-r--r--   0        0        0        0 2023-04-26 15:35:24.985359 kedro_snowflake-0.1.1/kedro_snowflake/starters/snowflights/{{ cookiecutter.repo_name }}/src/tests/pipelines/__init__.py
--rw-r--r--   0        0        0     1109 2023-04-26 15:35:24.985359 kedro_snowflake-0.1.1/kedro_snowflake/starters/snowflights/{{ cookiecutter.repo_name }}/src/tests/test_run.py
--rw-r--r--   0        0        0       60 2023-04-26 15:35:24.985359 kedro_snowflake-0.1.1/kedro_snowflake/starters/snowflights/{{ cookiecutter.repo_name }}/src/{{ cookiecutter.python_package }}/__init__.py
--rw-r--r--   0        0        0     1527 2023-04-26 15:35:24.989359 kedro_snowflake-0.1.1/kedro_snowflake/starters/snowflights/{{ cookiecutter.repo_name }}/src/{{ cookiecutter.python_package }}/__main__.py
--rw-r--r--   0        0        0      423 2023-04-26 15:35:24.989359 kedro_snowflake-0.1.1/kedro_snowflake/starters/snowflights/{{ cookiecutter.repo_name }}/src/{{ cookiecutter.python_package }}/pipeline_registry.py
--rw-r--r--   0        0        0        0 2023-04-26 15:35:24.989359 kedro_snowflake-0.1.1/kedro_snowflake/starters/snowflights/{{ cookiecutter.repo_name }}/src/{{ cookiecutter.python_package }}/pipelines/__init__.py
--rwxr-xr-x   0        0        0      117 2023-04-26 15:35:24.989359 kedro_snowflake-0.1.1/kedro_snowflake/starters/snowflights/{{ cookiecutter.repo_name }}/src/{{ cookiecutter.python_package }}/pipelines/data_processing/__init__.py
--rwxr-xr-x   0        0        0     2607 2023-04-26 15:35:24.989359 kedro_snowflake-0.1.1/kedro_snowflake/starters/snowflights/{{ cookiecutter.repo_name }}/src/{{ cookiecutter.python_package }}/pipelines/data_processing/nodes.py
--rwxr-xr-x   0        0        0     1192 2023-04-26 15:35:24.989359 kedro_snowflake-0.1.1/kedro_snowflake/starters/snowflights/{{ cookiecutter.repo_name }}/src/{{ cookiecutter.python_package }}/pipelines/data_processing/pipeline.py
--rwxr-xr-x   0        0        0      114 2023-04-26 15:35:24.989359 kedro_snowflake-0.1.1/kedro_snowflake/starters/snowflights/{{ cookiecutter.repo_name }}/src/{{ cookiecutter.python_package }}/pipelines/data_science/__init__.py
--rwxr-xr-x   0        0        0     1712 2023-04-26 15:35:24.989359 kedro_snowflake-0.1.1/kedro_snowflake/starters/snowflights/{{ cookiecutter.repo_name }}/src/{{ cookiecutter.python_package }}/pipelines/data_science/nodes.py
--rwxr-xr-x   0        0        0      866 2023-04-26 15:35:24.989359 kedro_snowflake-0.1.1/kedro_snowflake/starters/snowflights/{{ cookiecutter.repo_name }}/src/{{ cookiecutter.python_package }}/pipelines/data_science/pipeline.py
--rw-r--r--   0        0        0     1363 2023-04-26 15:35:24.989359 kedro_snowflake-0.1.1/kedro_snowflake/starters/snowflights/{{ cookiecutter.repo_name }}/src/{{ cookiecutter.python_package }}/settings.py
--rw-r--r--   0        0        0      263 2023-04-26 15:35:24.933359 kedro_snowflake-0.1.1/kedro_snowflake/starters.py
--rw-r--r--   0        0        0     5272 2023-04-26 15:35:24.989359 kedro_snowflake-0.1.1/kedro_snowflake/utils.py
--rw-r--r--   0        0        0     1697 2023-04-26 15:35:24.989359 kedro_snowflake-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     5734 1970-01-01 00:00:00.000000 kedro_snowflake-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0    11338 2023-05-05 10:45:27.909912 kedro_snowflake-0.1.2/LICENSE
+-rw-r--r--   0        0        0     4510 2023-05-05 10:45:27.909912 kedro_snowflake-0.1.2/README.md
+-rw-r--r--   0        0        0       22 2023-05-05 10:45:27.913912 kedro_snowflake-0.1.2/kedro_snowflake/__init__.py
+-rw-r--r--   0        0        0     4523 2023-05-05 10:45:27.913912 kedro_snowflake-0.1.2/kedro_snowflake/cli.py
+-rw-r--r--   0        0        0     2282 2023-05-05 10:45:27.913912 kedro_snowflake-0.1.2/kedro_snowflake/cli_functions.py
+-rw-r--r--   0        0        0     4444 2023-05-05 10:45:27.913912 kedro_snowflake-0.1.2/kedro_snowflake/config.py
+-rw-r--r--   0        0        0        0 2023-05-05 10:45:27.913912 kedro_snowflake-0.1.2/kedro_snowflake/datasets/__init__.py
+-rw-r--r--   0        0        0     5483 2023-05-05 10:45:27.913912 kedro_snowflake-0.1.2/kedro_snowflake/datasets/internal.py
+-rw-r--r--   0        0        0     5660 2023-05-05 10:45:27.913912 kedro_snowflake-0.1.2/kedro_snowflake/datasets/native.py
+-rw-r--r--   0        0        0    14301 2023-05-05 10:45:27.913912 kedro_snowflake-0.1.2/kedro_snowflake/generator.py
+-rw-r--r--   0        0        0      119 2023-05-05 10:45:27.913912 kedro_snowflake-0.1.2/kedro_snowflake/misc.py
+-rw-r--r--   0        0        0     3504 2023-05-05 10:45:27.913912 kedro_snowflake-0.1.2/kedro_snowflake/pipeline.py
+-rw-r--r--   0        0        0     1526 2023-05-05 10:45:27.913912 kedro_snowflake-0.1.2/kedro_snowflake/runner.py
+-rw-r--r--   0        0        0     1612 2023-05-05 10:45:27.913912 kedro_snowflake-0.1.2/kedro_snowflake/starters/snowflights/README.md
+-rw-r--r--   0        0        0      524 2023-05-05 10:45:27.913912 kedro_snowflake-0.1.2/kedro_snowflake/starters/snowflights/cookiecutter.json
+-rw-r--r--   0        0        0   162747 2023-05-05 10:45:27.913912 kedro_snowflake-0.1.2/kedro_snowflake/starters/snowflights/images/pipeline_visualisation_with_layers.png
+-rw-r--r--   0        0        0   162747 2023-05-05 10:45:27.913912 kedro_snowflake-0.1.2/kedro_snowflake/starters/snowflights/pipeline_visualisation_with_layers.png
+-rw-r--r--   0        0        0     1927 2023-05-05 10:45:27.917912 kedro_snowflake-0.1.2/kedro_snowflake/starters/snowflights/prompts.yml
+-rw-r--r--   0        0        0     1785 2023-05-05 10:45:27.917912 kedro_snowflake-0.1.2/kedro_snowflake/starters/snowflights/{{ cookiecutter.repo_name }}/.gitignore
+-rw-r--r--   0        0        0     3958 2023-05-05 10:45:27.917912 kedro_snowflake-0.1.2/kedro_snowflake/starters/snowflights/{{ cookiecutter.repo_name }}/README.md
+-rw-r--r--   0        0        0     1083 2023-05-05 10:45:27.917912 kedro_snowflake-0.1.2/kedro_snowflake/starters/snowflights/{{ cookiecutter.repo_name }}/conf/README.md
+-rw-r--r--   0        0        0     2778 2023-05-05 10:45:27.917912 kedro_snowflake-0.1.2/kedro_snowflake/starters/snowflights/{{ cookiecutter.repo_name }}/conf/base/catalog.yml
+-rw-r--r--   0        0        0      901 2023-05-05 10:45:27.917912 kedro_snowflake-0.1.2/kedro_snowflake/starters/snowflights/{{ cookiecutter.repo_name }}/conf/base/logging.yml
+-rw-r--r--   0        0        0        0 2023-05-05 10:45:27.917912 kedro_snowflake-0.1.2/kedro_snowflake/starters/snowflights/{{ cookiecutter.repo_name }}/conf/base/parameters/data_processing.yml
+-rw-r--r--   0        0        0      232 2023-05-05 10:45:27.917912 kedro_snowflake-0.1.2/kedro_snowflake/starters/snowflights/{{ cookiecutter.repo_name }}/conf/base/parameters/data_science.yml
+-rw-r--r--   0        0        0        0 2023-05-05 10:45:27.917912 kedro_snowflake-0.1.2/kedro_snowflake/starters/snowflights/{{ cookiecutter.repo_name }}/conf/base/parameters.yml
+-rw-r--r--   0        0        0     2073 2023-05-05 10:45:27.917912 kedro_snowflake-0.1.2/kedro_snowflake/starters/snowflights/{{ cookiecutter.repo_name }}/conf/base/snowflake.yml
+-rw-r--r--   0        0        0        0 2023-05-05 10:45:27.917912 kedro_snowflake-0.1.2/kedro_snowflake/starters/snowflights/{{ cookiecutter.repo_name }}/conf/local/.gitkeep
+-rw-r--r--   0        0        0      431 2023-05-05 10:45:27.917912 kedro_snowflake-0.1.2/kedro_snowflake/starters/snowflights/{{ cookiecutter.repo_name }}/conf/local/credentials.yml
+-rw-r--r--   0        0        0        0 2023-05-05 10:45:27.917912 kedro_snowflake-0.1.2/kedro_snowflake/starters/snowflights/{{ cookiecutter.repo_name }}/data/01_raw/.gitkeep
+-rw-r--r--   0        0        0  1810602 2023-05-05 10:45:27.925912 kedro_snowflake-0.1.2/kedro_snowflake/starters/snowflights/{{ cookiecutter.repo_name }}/data/01_raw/companies.csv
+-rw-r--r--   0        0        0  2937144 2023-05-05 10:45:27.937912 kedro_snowflake-0.1.2/kedro_snowflake/starters/snowflights/{{ cookiecutter.repo_name }}/data/01_raw/reviews.csv
+-rw-r--r--   0        0        0  4195290 2023-05-05 10:45:27.965913 kedro_snowflake-0.1.2/kedro_snowflake/starters/snowflights/{{ cookiecutter.repo_name }}/data/01_raw/shuttles.xlsx
+-rw-r--r--   0        0        0        0 2023-05-05 10:45:27.965913 kedro_snowflake-0.1.2/kedro_snowflake/starters/snowflights/{{ cookiecutter.repo_name }}/data/02_intermediate/.gitkeep
+-rw-r--r--   0        0        0        0 2023-05-05 10:45:27.965913 kedro_snowflake-0.1.2/kedro_snowflake/starters/snowflights/{{ cookiecutter.repo_name }}/data/03_primary/.gitkeep
+-rw-r--r--   0        0        0        0 2023-05-05 10:45:27.965913 kedro_snowflake-0.1.2/kedro_snowflake/starters/snowflights/{{ cookiecutter.repo_name }}/data/04_feature/.gitkeep
+-rw-r--r--   0        0        0        0 2023-05-05 10:45:27.965913 kedro_snowflake-0.1.2/kedro_snowflake/starters/snowflights/{{ cookiecutter.repo_name }}/data/05_model_input/.gitkeep
+-rw-r--r--   0        0        0        0 2023-05-05 10:45:27.965913 kedro_snowflake-0.1.2/kedro_snowflake/starters/snowflights/{{ cookiecutter.repo_name }}/data/06_models/.gitkeep
+-rw-r--r--   0        0        0        0 2023-05-05 10:45:27.965913 kedro_snowflake-0.1.2/kedro_snowflake/starters/snowflights/{{ cookiecutter.repo_name }}/data/07_model_output/.gitkeep
+-rw-r--r--   0        0        0        0 2023-05-05 10:45:27.965913 kedro_snowflake-0.1.2/kedro_snowflake/starters/snowflights/{{ cookiecutter.repo_name }}/data/08_reporting/.gitkeep
+-rw-r--r--   0        0        0     6967 2023-05-05 10:45:27.965913 kedro_snowflake-0.1.2/kedro_snowflake/starters/snowflights/{{ cookiecutter.repo_name }}/docs/source/conf.py
+-rw-r--r--   0        0        0      459 2023-05-05 10:45:27.965913 kedro_snowflake-0.1.2/kedro_snowflake/starters/snowflights/{{ cookiecutter.repo_name }}/docs/source/index.rst
+-rw-r--r--   0        0        0        0 2023-05-05 10:45:27.965913 kedro_snowflake-0.1.2/kedro_snowflake/starters/snowflights/{{ cookiecutter.repo_name }}/logs/.gitkeep
+-rw-r--r--   0        0        0        0 2023-05-05 10:45:27.965913 kedro_snowflake-0.1.2/kedro_snowflake/starters/snowflights/{{ cookiecutter.repo_name }}/notebooks/.gitkeep
+-rw-r--r--   0        0        0      446 2023-05-05 10:45:27.965913 kedro_snowflake-0.1.2/kedro_snowflake/starters/snowflights/{{ cookiecutter.repo_name }}/pyproject.toml
+-rw-r--r--   0        0        0       47 2023-05-05 10:45:27.965913 kedro_snowflake-0.1.2/kedro_snowflake/starters/snowflights/{{ cookiecutter.repo_name }}/setup.cfg
+-rw-r--r--   0        0        0      433 2023-05-05 10:45:27.965913 kedro_snowflake-0.1.2/kedro_snowflake/starters/snowflights/{{ cookiecutter.repo_name }}/src/requirements.txt
+-rw-r--r--   0        0        0     1198 2023-05-05 10:45:27.965913 kedro_snowflake-0.1.2/kedro_snowflake/starters/snowflights/{{ cookiecutter.repo_name }}/src/setup.py
+-rw-r--r--   0        0        0        0 2023-05-05 10:45:27.965913 kedro_snowflake-0.1.2/kedro_snowflake/starters/snowflights/{{ cookiecutter.repo_name }}/src/tests/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-05 10:45:27.965913 kedro_snowflake-0.1.2/kedro_snowflake/starters/snowflights/{{ cookiecutter.repo_name }}/src/tests/pipelines/__init__.py
+-rw-r--r--   0        0        0     1109 2023-05-05 10:45:27.965913 kedro_snowflake-0.1.2/kedro_snowflake/starters/snowflights/{{ cookiecutter.repo_name }}/src/tests/test_run.py
+-rw-r--r--   0        0        0       60 2023-05-05 10:45:27.965913 kedro_snowflake-0.1.2/kedro_snowflake/starters/snowflights/{{ cookiecutter.repo_name }}/src/{{ cookiecutter.python_package }}/__init__.py
+-rw-r--r--   0        0        0     1527 2023-05-05 10:45:27.965913 kedro_snowflake-0.1.2/kedro_snowflake/starters/snowflights/{{ cookiecutter.repo_name }}/src/{{ cookiecutter.python_package }}/__main__.py
+-rw-r--r--   0        0        0      423 2023-05-05 10:45:27.965913 kedro_snowflake-0.1.2/kedro_snowflake/starters/snowflights/{{ cookiecutter.repo_name }}/src/{{ cookiecutter.python_package }}/pipeline_registry.py
+-rw-r--r--   0        0        0        0 2023-05-05 10:45:27.965913 kedro_snowflake-0.1.2/kedro_snowflake/starters/snowflights/{{ cookiecutter.repo_name }}/src/{{ cookiecutter.python_package }}/pipelines/__init__.py
+-rwxr-xr-x   0        0        0      117 2023-05-05 10:45:27.965913 kedro_snowflake-0.1.2/kedro_snowflake/starters/snowflights/{{ cookiecutter.repo_name }}/src/{{ cookiecutter.python_package }}/pipelines/data_processing/__init__.py
+-rwxr-xr-x   0        0        0     2607 2023-05-05 10:45:27.965913 kedro_snowflake-0.1.2/kedro_snowflake/starters/snowflights/{{ cookiecutter.repo_name }}/src/{{ cookiecutter.python_package }}/pipelines/data_processing/nodes.py
+-rwxr-xr-x   0        0        0     1192 2023-05-05 10:45:27.965913 kedro_snowflake-0.1.2/kedro_snowflake/starters/snowflights/{{ cookiecutter.repo_name }}/src/{{ cookiecutter.python_package }}/pipelines/data_processing/pipeline.py
+-rwxr-xr-x   0        0        0      114 2023-05-05 10:45:27.965913 kedro_snowflake-0.1.2/kedro_snowflake/starters/snowflights/{{ cookiecutter.repo_name }}/src/{{ cookiecutter.python_package }}/pipelines/data_science/__init__.py
+-rwxr-xr-x   0        0        0     1712 2023-05-05 10:45:27.965913 kedro_snowflake-0.1.2/kedro_snowflake/starters/snowflights/{{ cookiecutter.repo_name }}/src/{{ cookiecutter.python_package }}/pipelines/data_science/nodes.py
+-rwxr-xr-x   0        0        0      866 2023-05-05 10:45:27.965913 kedro_snowflake-0.1.2/kedro_snowflake/starters/snowflights/{{ cookiecutter.repo_name }}/src/{{ cookiecutter.python_package }}/pipelines/data_science/pipeline.py
+-rw-r--r--   0        0        0     1363 2023-05-05 10:45:27.965913 kedro_snowflake-0.1.2/kedro_snowflake/starters/snowflights/{{ cookiecutter.repo_name }}/src/{{ cookiecutter.python_package }}/settings.py
+-rw-r--r--   0        0        0      263 2023-05-05 10:45:27.913912 kedro_snowflake-0.1.2/kedro_snowflake/starters.py
+-rw-r--r--   0        0        0     5272 2023-05-05 10:45:27.965913 kedro_snowflake-0.1.2/kedro_snowflake/utils.py
+-rw-r--r--   0        0        0     1712 2023-05-05 10:45:27.965913 kedro_snowflake-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     5762 1970-01-01 00:00:00.000000 kedro_snowflake-0.1.2/PKG-INFO
```

### Comparing `kedro_snowflake-0.1.1/LICENSE` & `kedro_snowflake-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `kedro_snowflake-0.1.1/README.md` & `kedro_snowflake-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `kedro_snowflake-0.1.1/kedro_snowflake/cli.py` & `kedro_snowflake-0.1.2/kedro_snowflake/cli.py`

 * *Files identical despite different names*

### Comparing `kedro_snowflake-0.1.1/kedro_snowflake/cli_functions.py` & `kedro_snowflake-0.1.2/kedro_snowflake/cli_functions.py`

 * *Files identical despite different names*

### Comparing `kedro_snowflake-0.1.1/kedro_snowflake/config.py` & `kedro_snowflake-0.1.2/kedro_snowflake/config.py`

 * *Files identical despite different names*

### Comparing `kedro_snowflake-0.1.1/kedro_snowflake/datasets/internal.py` & `kedro_snowflake-0.1.2/kedro_snowflake/datasets/internal.py`

 * *Files identical despite different names*

### Comparing `kedro_snowflake-0.1.1/kedro_snowflake/datasets/native.py` & `kedro_snowflake-0.1.2/kedro_snowflake/datasets/native.py`

 * *Files identical despite different names*

### Comparing `kedro_snowflake-0.1.1/kedro_snowflake/generator.py` & `kedro_snowflake-0.1.2/kedro_snowflake/generator.py`

 * *Files identical despite different names*

### Comparing `kedro_snowflake-0.1.1/kedro_snowflake/pipeline.py` & `kedro_snowflake-0.1.2/kedro_snowflake/pipeline.py`

 * *Files identical despite different names*

### Comparing `kedro_snowflake-0.1.1/kedro_snowflake/runner.py` & `kedro_snowflake-0.1.2/kedro_snowflake/runner.py`

 * *Files identical despite different names*

### Comparing `kedro_snowflake-0.1.1/kedro_snowflake/starters/snowflights/README.md` & `kedro_snowflake-0.1.2/kedro_snowflake/starters/snowflights/README.md`

 * *Files identical despite different names*

### Comparing `kedro_snowflake-0.1.1/kedro_snowflake/starters/snowflights/cookiecutter.json` & `kedro_snowflake-0.1.2/kedro_snowflake/starters/snowflights/cookiecutter.json`

 * *Files identical despite different names*

### Comparing `kedro_snowflake-0.1.1/kedro_snowflake/starters/snowflights/images/pipeline_visualisation_with_layers.png` & `kedro_snowflake-0.1.2/kedro_snowflake/starters/snowflights/images/pipeline_visualisation_with_layers.png`

 * *Files identical despite different names*

### Comparing `kedro_snowflake-0.1.1/kedro_snowflake/starters/snowflights/pipeline_visualisation_with_layers.png` & `kedro_snowflake-0.1.2/kedro_snowflake/starters/snowflights/pipeline_visualisation_with_layers.png`

 * *Files identical despite different names*

### Comparing `kedro_snowflake-0.1.1/kedro_snowflake/starters/snowflights/prompts.yml` & `kedro_snowflake-0.1.2/kedro_snowflake/starters/snowflights/prompts.yml`

 * *Files identical despite different names*

### Comparing `kedro_snowflake-0.1.1/kedro_snowflake/starters/snowflights/{{ cookiecutter.repo_name }}/.gitignore` & `kedro_snowflake-0.1.2/kedro_snowflake/starters/snowflights/{{ cookiecutter.repo_name }}/.gitignore`

 * *Files identical despite different names*

### Comparing `kedro_snowflake-0.1.1/kedro_snowflake/starters/snowflights/{{ cookiecutter.repo_name }}/README.md` & `kedro_snowflake-0.1.2/kedro_snowflake/starters/snowflights/{{ cookiecutter.repo_name }}/README.md`

 * *Files identical despite different names*

### Comparing `kedro_snowflake-0.1.1/kedro_snowflake/starters/snowflights/{{ cookiecutter.repo_name }}/conf/README.md` & `kedro_snowflake-0.1.2/kedro_snowflake/starters/snowflights/{{ cookiecutter.repo_name }}/conf/README.md`

 * *Files identical despite different names*

### Comparing `kedro_snowflake-0.1.1/kedro_snowflake/starters/snowflights/{{ cookiecutter.repo_name }}/conf/base/catalog.yml` & `kedro_snowflake-0.1.2/kedro_snowflake/starters/snowflights/{{ cookiecutter.repo_name }}/conf/base/catalog.yml`

 * *Files identical despite different names*

### Comparing `kedro_snowflake-0.1.1/kedro_snowflake/starters/snowflights/{{ cookiecutter.repo_name }}/conf/base/logging.yml` & `kedro_snowflake-0.1.2/kedro_snowflake/starters/snowflights/{{ cookiecutter.repo_name }}/conf/base/logging.yml`

 * *Files identical despite different names*

### Comparing `kedro_snowflake-0.1.1/kedro_snowflake/starters/snowflights/{{ cookiecutter.repo_name }}/conf/base/snowflake.yml` & `kedro_snowflake-0.1.2/kedro_snowflake/starters/snowflights/{{ cookiecutter.repo_name }}/conf/base/snowflake.yml`

 * *Files identical despite different names*

### Comparing `kedro_snowflake-0.1.1/kedro_snowflake/starters/snowflights/{{ cookiecutter.repo_name }}/data/01_raw/companies.csv` & `kedro_snowflake-0.1.2/kedro_snowflake/starters/snowflights/{{ cookiecutter.repo_name }}/data/01_raw/companies.csv`

 * *Files identical despite different names*

### Comparing `kedro_snowflake-0.1.1/kedro_snowflake/starters/snowflights/{{ cookiecutter.repo_name }}/data/01_raw/reviews.csv` & `kedro_snowflake-0.1.2/kedro_snowflake/starters/snowflights/{{ cookiecutter.repo_name }}/data/01_raw/reviews.csv`

 * *Files identical despite different names*

### Comparing `kedro_snowflake-0.1.1/kedro_snowflake/starters/snowflights/{{ cookiecutter.repo_name }}/data/01_raw/shuttles.xlsx` & `kedro_snowflake-0.1.2/kedro_snowflake/starters/snowflights/{{ cookiecutter.repo_name }}/data/01_raw/shuttles.xlsx`

 * *Files identical despite different names*

### Comparing `kedro_snowflake-0.1.1/kedro_snowflake/starters/snowflights/{{ cookiecutter.repo_name }}/docs/source/conf.py` & `kedro_snowflake-0.1.2/kedro_snowflake/starters/snowflights/{{ cookiecutter.repo_name }}/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `kedro_snowflake-0.1.1/kedro_snowflake/starters/snowflights/{{ cookiecutter.repo_name }}/src/setup.py` & `kedro_snowflake-0.1.2/kedro_snowflake/starters/snowflights/{{ cookiecutter.repo_name }}/src/setup.py`

 * *Files identical despite different names*

### Comparing `kedro_snowflake-0.1.1/kedro_snowflake/starters/snowflights/{{ cookiecutter.repo_name }}/src/tests/test_run.py` & `kedro_snowflake-0.1.2/kedro_snowflake/starters/snowflights/{{ cookiecutter.repo_name }}/src/tests/test_run.py`

 * *Files identical despite different names*

### Comparing `kedro_snowflake-0.1.1/kedro_snowflake/starters/snowflights/{{ cookiecutter.repo_name }}/src/{{ cookiecutter.python_package }}/__main__.py` & `kedro_snowflake-0.1.2/kedro_snowflake/starters/snowflights/{{ cookiecutter.repo_name }}/src/{{ cookiecutter.python_package }}/__main__.py`

 * *Files identical despite different names*

### Comparing `kedro_snowflake-0.1.1/kedro_snowflake/starters/snowflights/{{ cookiecutter.repo_name }}/src/{{ cookiecutter.python_package }}/pipelines/data_processing/nodes.py` & `kedro_snowflake-0.1.2/kedro_snowflake/starters/snowflights/{{ cookiecutter.repo_name }}/src/{{ cookiecutter.python_package }}/pipelines/data_processing/nodes.py`

 * *Files identical despite different names*

### Comparing `kedro_snowflake-0.1.1/kedro_snowflake/starters/snowflights/{{ cookiecutter.repo_name }}/src/{{ cookiecutter.python_package }}/pipelines/data_processing/pipeline.py` & `kedro_snowflake-0.1.2/kedro_snowflake/starters/snowflights/{{ cookiecutter.repo_name }}/src/{{ cookiecutter.python_package }}/pipelines/data_processing/pipeline.py`

 * *Files identical despite different names*

### Comparing `kedro_snowflake-0.1.1/kedro_snowflake/starters/snowflights/{{ cookiecutter.repo_name }}/src/{{ cookiecutter.python_package }}/pipelines/data_science/nodes.py` & `kedro_snowflake-0.1.2/kedro_snowflake/starters/snowflights/{{ cookiecutter.repo_name }}/src/{{ cookiecutter.python_package }}/pipelines/data_science/nodes.py`

 * *Files identical despite different names*

### Comparing `kedro_snowflake-0.1.1/kedro_snowflake/starters/snowflights/{{ cookiecutter.repo_name }}/src/{{ cookiecutter.python_package }}/pipelines/data_science/pipeline.py` & `kedro_snowflake-0.1.2/kedro_snowflake/starters/snowflights/{{ cookiecutter.repo_name }}/src/{{ cookiecutter.python_package }}/pipelines/data_science/pipeline.py`

 * *Files identical despite different names*

### Comparing `kedro_snowflake-0.1.1/kedro_snowflake/starters/snowflights/{{ cookiecutter.repo_name }}/src/{{ cookiecutter.python_package }}/settings.py` & `kedro_snowflake-0.1.2/kedro_snowflake/starters/snowflights/{{ cookiecutter.repo_name }}/src/{{ cookiecutter.python_package }}/settings.py`

 * *Files identical despite different names*

### Comparing `kedro_snowflake-0.1.1/kedro_snowflake/utils.py` & `kedro_snowflake-0.1.2/kedro_snowflake/utils.py`

 * *Files identical despite different names*

### Comparing `kedro_snowflake-0.1.1/pyproject.toml` & `kedro_snowflake-0.1.2/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "kedro-snowflake"
-version = "0.1.1"
+version = "0.1.2"
 description = "Kedro plugin with Snowflake / Snowpark support"
 readme = "README.md"
 authors = ['GetInData MLOPS <mlops@getindata.com>']
 maintainers = ['GetInData MLOPS <mlops@getindata.com>']
 homepage = "https://github.com/getindata/kedro-snowflake"
 repository = "https://github.com/getindata/kedro-snowflake"
 documentation = "https://kedro-snowflake.readthedocs.io/"
@@ -31,20 +31,21 @@
 [tool.isort]
 known_third_party = ["pydantic","semver","setuptools"]
 
 [tool.poetry.dependencies]
 python = ">=3.8,<3.9"
 kedro = ">=0.18.7,<0.19"
 snowflake-snowpark-python = {version = ">=1.0.0,<1.1.0", extras = ["pandas"]}
-kedro-datasets = {version = ">=1.2.0,<1.3.0", extras = ["pandas-csvdataset", "pandas-exceldataset", "pandas-parquetdataset", "snowflake-snowparktabledataset"]}
 backoff = "^2.2.1"
 cloudpickle = ">=1.6.0,<=2.0.0"
 zstandard = "^0.20.0"
 pydantic = "^1.10.7"
 tabulate = "^0.9.0"
+kedro-datasets = {version = ">=1.1.0", extras = ["pandas-csvdataset", "pandas-exceldataset", "pandas-parquetdataset", "snowflake-snowparktabledataset"]}
+pandas = ">=1.3,<3.0"
 
 [tool.poetry.dev-dependencies]
 pytest = "<7"
 pytest-cov = ">=2.8.0, <4.0.0"
 tox = ">=3.25.1"
 pre-commit = "2.20.0"
```

### Comparing `kedro_snowflake-0.1.1/PKG-INFO` & `kedro_snowflake-0.1.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kedro-snowflake
-Version: 0.1.1
+Version: 0.1.2
 Summary: Kedro plugin with Snowflake / Snowpark support
 Home-page: https://github.com/getindata/kedro-snowflake
 License: Apache-2.0
 Keywords: kedro,snowflake,snowpark,mlops
 Author: GetInData MLOPS
 Author-email: mlops@getindata.com
 Maintainer: GetInData MLOPS
@@ -13,15 +13,16 @@
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Requires-Dist: backoff (>=2.2.1,<3.0.0)
 Requires-Dist: cloudpickle (>=1.6.0,<=2.0.0)
 Requires-Dist: kedro (>=0.18.7,<0.19)
-Requires-Dist: kedro-datasets[pandas-csvdataset,pandas-exceldataset,pandas-parquetdataset,snowflake-snowparktabledataset] (>=1.2.0,<1.3.0)
+Requires-Dist: kedro-datasets[pandas-csvdataset,pandas-exceldataset,pandas-parquetdataset,snowflake-snowparktabledataset] (>=1.1.0)
+Requires-Dist: pandas (>=1.3,<3.0)
 Requires-Dist: pydantic (>=1.10.7,<2.0.0)
 Requires-Dist: snowflake-snowpark-python[pandas] (>=1.0.0,<1.1.0)
 Requires-Dist: tabulate (>=0.9.0,<0.10.0)
 Requires-Dist: zstandard (>=0.20.0,<0.21.0)
 Project-URL: Documentation, https://kedro-snowflake.readthedocs.io/
 Project-URL: Repository, https://github.com/getindata/kedro-snowflake
 Description-Content-Type: text/markdown
```

#### html2text {}

```diff
@@ -1,30 +1,30 @@
-Metadata-Version: 2.1 Name: kedro-snowflake Version: 0.1.1 Summary: Kedro
+Metadata-Version: 2.1 Name: kedro-snowflake Version: 0.1.2 Summary: Kedro
 plugin with Snowflake / Snowpark support Home-page: https://github.com/
 getindata/kedro-snowflake License: Apache-2.0 Keywords:
 kedro,snowflake,snowpark,mlops Author: GetInData MLOPS Author-email:
 mlops@getindata.com Maintainer: GetInData MLOPS Maintainer-email:
 mlops@getindata.com Requires-Python: >=3.8,<3.9 Classifier: Development Status
 :: 4 - Beta Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3 Classifier: Programming
 Language :: Python :: 3.8 Requires-Dist: backoff (>=2.2.1,<3.0.0) Requires-
 Dist: cloudpickle (>=1.6.0,<=2.0.0) Requires-Dist: kedro (>=0.18.7,<0.19)
 Requires-Dist: kedro-datasets[pandas-csvdataset,pandas-exceldataset,pandas-
-parquetdataset,snowflake-snowparktabledataset] (>=1.2.0,<1.3.0) Requires-Dist:
-pydantic (>=1.10.7,<2.0.0) Requires-Dist: snowflake-snowpark-python[pandas]
-(>=1.0.0,<1.1.0) Requires-Dist: tabulate (>=0.9.0,<0.10.0) Requires-Dist:
-zstandard (>=0.20.0,<0.21.0) Project-URL: Documentation, https://kedro-
-snowflake.readthedocs.io/ Project-URL: Repository, https://github.com/
-getindata/kedro-snowflake Description-Content-Type: text/markdown # Kedro
-Snowflake Pipelines plugin [![Python Version](https://img.shields.io/pypi/
-pyversions/kedro-snowflake)](https://github.com/getindata/kedro-snowflake) [!
-[License](https://img.shields.io/badge/license-Apache%202.0-blue.svg)](https://
-opensource.org/licenses/Apache-2.0) [![SemVer](https://img.shields.io/badge/
-semver-2.0.0-green)](https://semver.org/) [![PyPI version](https://
-badge.fury.io/py/kedro-snowflake.svg)](https://pypi.org/project/kedro-
+parquetdataset,snowflake-snowparktabledataset] (>=1.1.0) Requires-Dist: pandas
+(>=1.3,<3.0) Requires-Dist: pydantic (>=1.10.7,<2.0.0) Requires-Dist:
+snowflake-snowpark-python[pandas] (>=1.0.0,<1.1.0) Requires-Dist: tabulate
+(>=0.9.0,<0.10.0) Requires-Dist: zstandard (>=0.20.0,<0.21.0) Project-URL:
+Documentation, https://kedro-snowflake.readthedocs.io/ Project-URL: Repository,
+https://github.com/getindata/kedro-snowflake Description-Content-Type: text/
+markdown # Kedro Snowflake Pipelines plugin [![Python Version](https://
+img.shields.io/pypi/pyversions/kedro-snowflake)](https://github.com/getindata/
+kedro-snowflake) [![License](https://img.shields.io/badge/license-Apache%202.0-
+blue.svg)](https://opensource.org/licenses/Apache-2.0) [![SemVer](https://
+img.shields.io/badge/semver-2.0.0-green)](https://semver.org/) [![PyPI version]
+(https://badge.fury.io/py/kedro-snowflake.svg)](https://pypi.org/project/kedro-
 snowflake/) [![Downloads](https://pepy.tech/badge/kedro-snowflake)](https://
 pepy.tech/project/kedro-snowflake) [![Maintainability Rating](https://
 sonarcloud.io/api/project_badges/measure?project=getindata_kedro-
 snowflake&metric=sqale_rating)](https://sonarcloud.io/summary/
 new_code?id=getindata_kedro-snowflake) [![Coverage](https://sonarcloud.io/api/
 project_badges/measure?project=getindata_kedro-snowflake&metric=coverage)]
 (https://sonarcloud.io/summary/new_code?id=getindata_kedro-snowflake) [!
```

