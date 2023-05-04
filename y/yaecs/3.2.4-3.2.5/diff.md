# Comparing `tmp/yaecs-3.2.4.tar.gz` & `tmp/yaecs-3.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yaecs-3.2.4.tar", last modified: Thu May  4 11:44:51 2023, max compression
+gzip compressed data, was "yaecs-3.2.5.tar", last modified: Thu May  4 23:33:24 2023, max compression
```

## Comparing `yaecs-3.2.4.tar` & `yaecs-3.2.5.tar`

### file list

```diff
@@ -1,65 +1,82 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 11:44:51.226376 yaecs-3.2.4/
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-05-04 11:44:33.000000 yaecs-3.2.4/.flake8
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 11:44:51.218376 yaecs-3.2.4/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 11:44:51.222376 yaecs-3.2.4/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      595 2023-05-04 11:44:33.000000 yaecs-3.2.4/.github/workflows/pipy_deployment.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2963 2023-05-04 11:44:33.000000 yaecs-3.2.4/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)    20869 2023-05-04 11:44:33.000000 yaecs-3.2.4/.pylintrc
--rw-r--r--   0 runner    (1001) docker     (123)     7641 2023-05-04 11:44:33.000000 yaecs-3.2.4/COPYING.LESSER.md
--rw-r--r--   0 runner    (1001) docker     (123)    34915 2023-05-04 11:44:33.000000 yaecs-3.2.4/COPYING.md
--rw-r--r--   0 runner    (1001) docker     (123)    78683 2023-05-04 11:44:33.000000 yaecs-3.2.4/DOCUMENTATION_WIP.md
--rw-r--r--   0 runner    (1001) docker     (123)    34915 2023-05-04 11:44:33.000000 yaecs-3.2.4/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-05-04 11:44:33.000000 yaecs-3.2.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     5856 2023-05-04 11:44:51.226376 yaecs-3.2.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5420 2023-05-04 11:44:33.000000 yaecs-3.2.4/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1295 2023-05-04 11:44:33.000000 yaecs-3.2.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-05-04 11:44:33.000000 yaecs-3.2.4/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 11:44:51.222376 yaecs-3.2.4/resources/
--rw-r--r--   0 runner    (1001) docker     (123)   175062 2023-05-04 11:44:33.000000 yaecs-3.2.4/resources/yaecs_constructor_overview.png
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-04 11:44:51.226376 yaecs-3.2.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      841 2023-05-04 11:44:33.000000 yaecs-3.2.4/setup.py
--rw-r--r--   0 runner    (1001) docker     (123)     3393 2023-05-04 11:44:33.000000 yaecs-3.2.4/short-readme.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 11:44:51.218376 yaecs-3.2.4/unittests/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 11:44:51.222376 yaecs-3.2.4/unittests/config/
--rw-r--r--   0 runner    (1001) docker     (123)    10329 2023-05-04 11:44:33.000000 yaecs-3.2.4/unittests/config/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)    36401 2023-05-04 11:44:33.000000 yaecs-3.2.4/unittests/config/test_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1545 2023-05-04 11:44:33.000000 yaecs-3.2.4/unittests/config/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 11:44:51.222376 yaecs-3.2.4/usage_example/
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-04 11:44:33.000000 yaecs-3.2.4/usage_example/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      482 2023-05-04 11:44:33.000000 yaecs-3.2.4/usage_example/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 11:44:51.222376 yaecs-3.2.4/usage_example/configs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 11:44:51.222376 yaecs-3.2.4/usage_example/configs/default/
--rw-r--r--   0 runner    (1001) docker     (123)      250 2023-05-04 11:44:33.000000 yaecs-3.2.4/usage_example/configs/default/data_config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      372 2023-05-04 11:44:33.000000 yaecs-3.2.4/usage_example/configs/default/main_config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      118 2023-05-04 11:44:33.000000 yaecs-3.2.4/usage_example/configs/default/model_config.yaml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 11:44:51.222376 yaecs-3.2.4/usage_example/configs/experiment/
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-05-04 11:44:33.000000 yaecs-3.2.4/usage_example/configs/experiment/dummy_test.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      303 2023-05-04 11:44:33.000000 yaecs-3.2.4/usage_example/configs/experiment/grid_search.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-04 11:44:33.000000 yaecs-3.2.4/usage_example/configs/experiment/random_search.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     2067 2023-05-04 11:44:33.000000 yaecs-3.2.4/usage_example/configs/project_config.py
--rw-r--r--   0 runner    (1001) docker     (123)    10563 2023-05-04 11:44:33.000000 yaecs-3.2.4/usage_example/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 11:44:51.222376 yaecs-3.2.4/usage_example/project_utils/
--rw-r--r--   0 runner    (1001) docker     (123)     2914 2023-05-04 11:44:33.000000 yaecs-3.2.4/usage_example/project_utils/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 11:44:51.226376 yaecs-3.2.4/yaecs/
--rw-r--r--   0 runner    (1001) docker     (123)     2385 2023-05-04 11:44:33.000000 yaecs-3.2.4/yaecs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-04 11:44:51.000000 yaecs-3.2.4/yaecs/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 11:44:51.226376 yaecs-3.2.4/yaecs/config/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 11:44:33.000000 yaecs-3.2.4/yaecs/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    24515 2023-05-04 11:44:33.000000 yaecs-3.2.4/yaecs/config/config.py
--rw-r--r--   0 runner    (1001) docker     (123)    47611 2023-05-04 11:44:33.000000 yaecs-3.2.4/yaecs/config/config_base.py
--rw-r--r--   0 runner    (1001) docker     (123)    17271 2023-05-04 11:44:33.000000 yaecs-3.2.4/yaecs/config/config_convenience.py
--rw-r--r--   0 runner    (1001) docker     (123)    13615 2023-05-04 11:44:33.000000 yaecs-3.2.4/yaecs/config/config_getters.py
--rw-r--r--   0 runner    (1001) docker     (123)    14876 2023-05-04 11:44:33.000000 yaecs-3.2.4/yaecs/config/config_hooks.py
--rw-r--r--   0 runner    (1001) docker     (123)    10918 2023-05-04 11:44:33.000000 yaecs-3.2.4/yaecs/config/config_processing_functions.py
--rw-r--r--   0 runner    (1001) docker     (123)     6816 2023-05-04 11:44:33.000000 yaecs-3.2.4/yaecs/config/config_setters.py
--rw-r--r--   0 runner    (1001) docker     (123)    24448 2023-05-04 11:44:33.000000 yaecs-3.2.4/yaecs/config_history.py
--rw-r--r--   0 runner    (1001) docker     (123)    33455 2023-05-04 11:44:33.000000 yaecs-3.2.4/yaecs/experiment.py
--rw-r--r--   0 runner    (1001) docker     (123)     5232 2023-05-04 11:44:33.000000 yaecs-3.2.4/yaecs/pytorch_lightning_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    10315 2023-05-04 11:44:33.000000 yaecs-3.2.4/yaecs/user_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    35179 2023-05-04 11:44:33.000000 yaecs-3.2.4/yaecs/yaecs_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 11:44:51.226376 yaecs-3.2.4/yaecs.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5856 2023-05-04 11:44:51.000000 yaecs-3.2.4/yaecs.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1320 2023-05-04 11:44:51.000000 yaecs-3.2.4/yaecs.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-04 11:44:51.000000 yaecs-3.2.4/yaecs.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       24 2023-05-04 11:44:51.000000 yaecs-3.2.4/yaecs.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-04 11:44:51.000000 yaecs-3.2.4/yaecs.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 23:33:24.621513 yaecs-3.2.5/
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-05-04 23:33:05.000000 yaecs-3.2.5/.flake8
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 23:33:24.605512 yaecs-3.2.5/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 23:33:24.609513 yaecs-3.2.5/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      595 2023-05-04 23:33:05.000000 yaecs-3.2.5/.github/workflows/pipy_deployment.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2963 2023-05-04 23:33:05.000000 yaecs-3.2.5/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)    20869 2023-05-04 23:33:05.000000 yaecs-3.2.5/.pylintrc
+-rw-r--r--   0 runner    (1001) docker     (123)     7641 2023-05-04 23:33:05.000000 yaecs-3.2.5/COPYING.LESSER.md
+-rw-r--r--   0 runner    (1001) docker     (123)    34915 2023-05-04 23:33:05.000000 yaecs-3.2.5/COPYING.md
+-rw-r--r--   0 runner    (1001) docker     (123)    78683 2023-05-04 23:33:05.000000 yaecs-3.2.5/DOCUMENTATION_WIP.md
+-rw-r--r--   0 runner    (1001) docker     (123)    34915 2023-05-04 23:33:05.000000 yaecs-3.2.5/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-05-04 23:33:05.000000 yaecs-3.2.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5856 2023-05-04 23:33:24.621513 yaecs-3.2.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5420 2023-05-04 23:33:05.000000 yaecs-3.2.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 23:33:24.613513 yaecs-3.2.5/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      640 2023-05-04 23:33:05.000000 yaecs-3.2.5/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     2705 2023-05-04 23:33:05.000000 yaecs-3.2.5/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3545 2023-05-04 23:33:05.000000 yaecs-3.2.5/docs/getting_started.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1908 2023-05-04 23:33:05.000000 yaecs-3.2.5/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      327 2023-05-04 23:33:05.000000 yaecs-3.2.5/docs/installation.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1003 2023-05-04 23:33:05.000000 yaecs-3.2.5/docs/license.md
+-rw-r--r--   0 runner    (1001) docker     (123)      766 2023-05-04 23:33:05.000000 yaecs-3.2.5/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (123)      209 2023-05-04 23:33:05.000000 yaecs-3.2.5/docs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      761 2023-05-04 23:33:05.000000 yaecs-3.2.5/docs/yaecs.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1242 2023-05-04 23:33:05.000000 yaecs-3.2.5/docs/yaecs_config.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1295 2023-05-04 23:33:05.000000 yaecs-3.2.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-05-04 23:33:05.000000 yaecs-3.2.5/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       26 2023-05-04 23:33:05.000000 yaecs-3.2.5/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 23:33:24.613513 yaecs-3.2.5/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)   175062 2023-05-04 23:33:05.000000 yaecs-3.2.5/resources/yaecs_constructor_overview.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 23:33:24.613513 yaecs-3.2.5/scipts/
+-rw-r--r--   0 runner    (1001) docker     (123)      204 2023-05-04 23:33:05.000000 yaecs-3.2.5/scipts/build_docs.sh
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-05-04 23:33:05.000000 yaecs-3.2.5/scipts/tests.sh
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-04 23:33:24.621513 yaecs-3.2.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      841 2023-05-04 23:33:05.000000 yaecs-3.2.5/setup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3393 2023-05-04 23:33:05.000000 yaecs-3.2.5/short-readme.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 23:33:24.613513 yaecs-3.2.5/unittests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 23:33:05.000000 yaecs-3.2.5/unittests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 23:33:24.613513 yaecs-3.2.5/unittests/config/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 23:33:05.000000 yaecs-3.2.5/unittests/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10329 2023-05-04 23:33:05.000000 yaecs-3.2.5/unittests/config/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36418 2023-05-04 23:33:05.000000 yaecs-3.2.5/unittests/config/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1545 2023-05-04 23:33:05.000000 yaecs-3.2.5/unittests/config/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 23:33:24.613513 yaecs-3.2.5/usage_example/
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-04 23:33:05.000000 yaecs-3.2.5/usage_example/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      482 2023-05-04 23:33:05.000000 yaecs-3.2.5/usage_example/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 23:33:24.613513 yaecs-3.2.5/usage_example/configs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 23:33:24.617513 yaecs-3.2.5/usage_example/configs/default/
+-rw-r--r--   0 runner    (1001) docker     (123)      250 2023-05-04 23:33:05.000000 yaecs-3.2.5/usage_example/configs/default/data_config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      372 2023-05-04 23:33:05.000000 yaecs-3.2.5/usage_example/configs/default/main_config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      118 2023-05-04 23:33:05.000000 yaecs-3.2.5/usage_example/configs/default/model_config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 23:33:24.617513 yaecs-3.2.5/usage_example/configs/experiment/
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-05-04 23:33:05.000000 yaecs-3.2.5/usage_example/configs/experiment/dummy_test.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      303 2023-05-04 23:33:05.000000 yaecs-3.2.5/usage_example/configs/experiment/grid_search.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-04 23:33:05.000000 yaecs-3.2.5/usage_example/configs/experiment/random_search.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     2067 2023-05-04 23:33:05.000000 yaecs-3.2.5/usage_example/configs/project_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10563 2023-05-04 23:33:05.000000 yaecs-3.2.5/usage_example/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 23:33:24.617513 yaecs-3.2.5/usage_example/project_utils/
+-rw-r--r--   0 runner    (1001) docker     (123)     2914 2023-05-04 23:33:05.000000 yaecs-3.2.5/usage_example/project_utils/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 23:33:24.617513 yaecs-3.2.5/yaecs/
+-rw-r--r--   0 runner    (1001) docker     (123)     2385 2023-05-04 23:33:05.000000 yaecs-3.2.5/yaecs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-05-04 23:33:24.000000 yaecs-3.2.5/yaecs/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 23:33:24.621513 yaecs-3.2.5/yaecs/config/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 23:33:05.000000 yaecs-3.2.5/yaecs/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24639 2023-05-04 23:33:05.000000 yaecs-3.2.5/yaecs/config/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    47697 2023-05-04 23:33:05.000000 yaecs-3.2.5/yaecs/config/config_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17359 2023-05-04 23:33:05.000000 yaecs-3.2.5/yaecs/config/config_convenience.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13667 2023-05-04 23:33:05.000000 yaecs-3.2.5/yaecs/config/config_getters.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14915 2023-05-04 23:33:05.000000 yaecs-3.2.5/yaecs/config/config_hooks.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10940 2023-05-04 23:33:05.000000 yaecs-3.2.5/yaecs/config/config_processing_functions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6841 2023-05-04 23:33:05.000000 yaecs-3.2.5/yaecs/config/config_setters.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24448 2023-05-04 23:33:05.000000 yaecs-3.2.5/yaecs/config_history.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33565 2023-05-04 23:33:05.000000 yaecs-3.2.5/yaecs/experiment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5232 2023-05-04 23:33:05.000000 yaecs-3.2.5/yaecs/pytorch_lightning_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10441 2023-05-04 23:33:05.000000 yaecs-3.2.5/yaecs/user_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35237 2023-05-04 23:33:05.000000 yaecs-3.2.5/yaecs/yaecs_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 23:33:24.617513 yaecs-3.2.5/yaecs.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5856 2023-05-04 23:33:24.000000 yaecs-3.2.5/yaecs.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1605 2023-05-04 23:33:24.000000 yaecs-3.2.5/yaecs.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-04 23:33:24.000000 yaecs-3.2.5/yaecs.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       24 2023-05-04 23:33:24.000000 yaecs-3.2.5/yaecs.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-04 23:33:24.000000 yaecs-3.2.5/yaecs.egg-info/top_level.txt
```

### Comparing `yaecs-3.2.4/.github/workflows/pipy_deployment.yaml` & `yaecs-3.2.5/.github/workflows/pipy_deployment.yaml`

 * *Files identical despite different names*

### Comparing `yaecs-3.2.4/.gitignore` & `yaecs-3.2.5/.gitignore`

 * *Files identical despite different names*

### Comparing `yaecs-3.2.4/.pylintrc` & `yaecs-3.2.5/.pylintrc`

 * *Files identical despite different names*

### Comparing `yaecs-3.2.4/COPYING.LESSER.md` & `yaecs-3.2.5/COPYING.LESSER.md`

 * *Files identical despite different names*

### Comparing `yaecs-3.2.4/COPYING.md` & `yaecs-3.2.5/COPYING.md`

 * *Files identical despite different names*

### Comparing `yaecs-3.2.4/DOCUMENTATION_WIP.md` & `yaecs-3.2.5/DOCUMENTATION_WIP.md`

 * *Files identical despite different names*

### Comparing `yaecs-3.2.4/LICENSE.md` & `yaecs-3.2.5/LICENSE.md`

 * *Files identical despite different names*

### Comparing `yaecs-3.2.4/PKG-INFO` & `yaecs-3.2.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yaecs
-Version: 3.2.4
+Version: 3.2.5
 Summary: A Config System designed for experimental purposes
 Author: Reactive Reality AG
 Project-URL: Source, https://gitlab.com/reactivereality/public/yaecs
 Keywords: template,machine,learning
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
```

### Comparing `yaecs-3.2.4/README.md` & `yaecs-3.2.5/README.md`

 * *Files identical despite different names*

### Comparing `yaecs-3.2.4/pyproject.toml` & `yaecs-3.2.5/pyproject.toml`

 * *Files identical despite different names*

### Comparing `yaecs-3.2.4/resources/yaecs_constructor_overview.png` & `yaecs-3.2.5/resources/yaecs_constructor_overview.png`

 * *Files identical despite different names*

### Comparing `yaecs-3.2.4/setup.py` & `yaecs-3.2.5/setup.py`

 * *Files identical despite different names*

### Comparing `yaecs-3.2.4/short-readme.md` & `yaecs-3.2.5/short-readme.md`

 * *Files identical despite different names*

### Comparing `yaecs-3.2.4/unittests/config/conftest.py` & `yaecs-3.2.5/unittests/config/conftest.py`

 * *Files identical despite different names*

### Comparing `yaecs-3.2.4/unittests/config/test_config.py` & `yaecs-3.2.5/unittests/config/test_config.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,19 +17,19 @@
 """
 import logging
 import os.path as osp
 from pathlib import Path
 from typing import Any
 
 import pytest
-from utils import load_config, template
 
-from yaecs import assign_yaml_tag, assign_order, Configuration, Priority
-from yaecs.yaecs_utils import compare_string_pattern
+from unittests.config.utils import load_config, template
+from yaecs import Configuration, Priority, assign_order, assign_yaml_tag
 from yaecs.user_utils import make_config
+from yaecs.yaecs_utils import compare_string_pattern
 
 
 def check_integrity(config, p_1: Any = 0.1, p_2: Any = 2.0, p_3: Any = 30.0,
                     p_4: Any = "string"):
     assert config["param1"] == p_1
     assert config["subconfig1.param2"] == p_2
     assert config["subconfig2.param3"] == p_3
```

### Comparing `yaecs-3.2.4/unittests/config/utils.py` & `yaecs-3.2.5/unittests/config/utils.py`

 * *Files identical despite different names*

### Comparing `yaecs-3.2.4/usage_example/configs/project_config.py` & `yaecs-3.2.5/usage_example/configs/project_config.py`

 * *Files identical despite different names*

### Comparing `yaecs-3.2.4/usage_example/main.py` & `yaecs-3.2.5/usage_example/main.py`

 * *Files identical despite different names*

### Comparing `yaecs-3.2.4/usage_example/project_utils/utils.py` & `yaecs-3.2.5/usage_example/project_utils/utils.py`

 * *Files identical despite different names*

### Comparing `yaecs-3.2.4/yaecs/__init__.py` & `yaecs-3.2.5/yaecs/__init__.py`

 * *Files identical despite different names*

### Comparing `yaecs-3.2.4/yaecs/config/config.py` & `yaecs-3.2.5/yaecs/config/config.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,51 +17,57 @@
 """
 
 import logging
 import sys
 import time
 from typing import Callable, Dict, List, Optional, Union
 
-from .config_base import _ConfigurationBase
 from ..yaecs_utils import ConfigDeclarator, format_str
+from .config_base import _ConfigurationBase
 
 YAECS_LOGGER = logging.getLogger(__name__)
 
 
 class Configuration(_ConfigurationBase):
-    """ Superclass for YAECS configurations. The superclass implements constructors, while the behaviour is spread
+    """
+    Superclass for YAECS configurations. The superclass implements constructors, while the behaviour is spread
     across the parent classes in the following way :
-    - _ConfigurationBase implements the most basic functionalities such as creation and merging operations. It inherits
+
+    * _ConfigurationBase implements the most basic functionalities such as creation and merging operations. It inherits
       from all other parent classes as Mixins ;
-    - ConfigHooksMixin implements processing functions whose name start with "register_as_" and are decorated by the
+    * ConfigHooksMixin implements processing functions whose name start with `register_as_` and are decorated by the
       yaecs_utils.hook decorator. Users can use those processing either as pre- or post-processing functions, which will
       have the added effect of tagging the processed parameters as playing a certain pre-defined role in the config ;
-    - ConfigGettersMixin implements public getters to access some private attributes as well as other values which
+    * ConfigGettersMixin implements public getters to access some private attributes as well as other values which
       require boilerplate code to be rigorously queried, such as user-defined parameters ;
-    - ConfigSettersMixin implements a few setters which the config uses internally to manipulate private attributes of
+    * ConfigSettersMixin implements a few setters which the config uses internally to manipulate private attributes of
       other Configuration instances (such as sub-configs) ;
-    - ConfigConvenienceMixin implements all functions which are not of central importance to the behaviour of the config
-      but wrap convenient functionalities which can be used either internally of by the user. """
+    * ConfigConvenienceMixin implements all functions which are not of central importance to the behaviour of the config
+      but wrap convenient functionalities which can be used either internally of by the user.
+
+    """
 
     def __init__(self, name: str = "main", overwriting_regime: str = "auto-save",
                  config_path_or_dictionary: Optional[ConfigDeclarator] = None,
                  nesting_hierarchy: Optional[List[str]] = None, state: Optional[List[str]] = None,
                  main_config: Optional['Configuration'] = None, variation: Optional[str] = None,
                  do_not_pre_process: bool = False, do_not_post_process: bool = False, verbose: bool = True,
                  **kwargs):
         """
         Should never be called directly by the user. Please use one of the constructors instead (load_config,
         build_from_configs, build_from_argv), or the utils.make_config convenience function.
+
         :param name: name for the config or sub-config
         :param overwriting_regime: can be "auto-save" (default, when a param is overwritten it is merged instead and the
-        config is saved automatically if it had been saved previously), "locked" (params can't be overwritten except
-        using merge explicitly) or "unsafe" (params can be freely overwritten but reproducibility is not guaranteed).
+            config is saved automatically if it had been saved previously), "locked" (params can't be overwritten except
+            using merge explicitly) or "unsafe" (params can be freely overwritten but reproducibility
+            is not guaranteed).
         :param config_path_or_dictionary: path or dictionary to create the config from
         :param nesting_hierarchy: list containing the names of all the configs in the sub-config chain leading to this
-        config
+            config
         :param state: processing state used for state tracking and debugging
         :param main_config: main config corresponding to this sub-config, or None if this config is the main config
         :param variation: the name of the variation being created
         :param do_not_pre_process: if true, pre-processing is deactivated in this initialization
         :param do_not_post_process: if true, post-processing is deactivated in this initialization
         :param verbose: if set to false, message logging by this config will be deactivated
         :raises ValueError: if the overwriting regime is not valid
@@ -116,19 +122,21 @@
                                          ConfigDeclarator], default_config_path: Optional[ConfigDeclarator] = None,
                     overwriting_regime: str = "auto-save", do_not_merge_command_line: bool = False,
                     do_not_pre_process: bool = False, do_not_post_process: bool = False,
                     **kwargs) -> 'Configuration':
         """
         First creates a config using the default config, then merges config_path into it. If config_path is a list,
         successively merges all configs in the list instead from index 0 to the last.
+
         :param configs: config's path or dictionary, or list of default config's paths or dictionaries to merge
         :param default_config_path: default config's path or dictionary
         :param overwriting_regime: can be "auto-save" (default, when a param is overwritten it is merged instead and the
-        config is saved automatically if it had been saved previously), "locked" (params can't be overwritten except
-        using merge explicitly) or "unsafe" (params can be freely overwritten but reproducibility is not guaranteed).
+            config is saved automatically if it had been saved previously), "locked" (params can't be overwritten except
+            using merge explicitly) or "unsafe" (params can be freely overwritten but reproducibility
+            is not guaranteed).
         :param do_not_merge_command_line: if True, does not try to merge the command line parameters
         :param do_not_pre_process: if true, pre-processing is deactivated in this initialization
         :param do_not_post_process: if true, post-processing is deactivated in this initialization
         :param kwargs: additional parameters to pass to Configuration
         :return: instance of Configuration object containing the desired config
         """
         # This needs to access protected members of the Configuration class several times to prepare the config
@@ -155,18 +163,20 @@
     def build_from_configs(cls, *configs: Union[List[ConfigDeclarator], ConfigDeclarator],
                            overwriting_regime: str = "auto-save", do_not_merge_command_line: bool = False,
                            do_not_pre_process: bool = False, do_not_post_process: bool = False,
                            **kwargs) -> 'Configuration':
         """
         First creates a config using the first config provided (or the first config in the provided list), then merges
         the subsequent configs into it from index 1 to the last.
+
         :param configs: config's path or dictionary, or list of default config's paths or dictionaries to merge
         :param overwriting_regime: can be "auto-save" (default, when a param is overwritten it is merged instead and the
-        config is saved automatically if it had been saved previously), "locked" (params can't be overwritten except
-        using merge explicitly) or "unsafe" (params can be freely overwritten but reproducibility is not guaranteed).
+            config is saved automatically if it had been saved previously), "locked" (params can't be overwritten except
+            using merge explicitly) or "unsafe" (params can be freely overwritten but reproducibility
+            is not guaranteed).
         :param do_not_merge_command_line: if True, does not try to merge the command line parameters
         :param do_not_pre_process: if true, pre-processing is deactivated in this initialization
         :param do_not_post_process: if true, post-processing is deactivated in this initialization
         :param kwargs: additional parameters to pass to Configuration
         :raises TypeError: if configs is invalid
         :return: instance of Configuration object containing the desired config
         """
@@ -188,22 +198,24 @@
                         default_config_path: Optional[ConfigDeclarator] = None, overwriting_regime: str = "auto-save",
                         do_not_merge_command_line: bool = False, do_not_pre_process: bool = False,
                         do_not_post_process: bool = False, **kwargs) -> 'Configuration':
         """
         Assumes a pattern of the form '--config <path_to_config>' or '--config [<path1>,<path2>,...]' in sys.argv (the
         brackets are optional), and builds a config from the specified paths by merging them into the default config in
         the specified order.
+
         :param configs: config's path or dictionary, or list of config paths or dictionaries to merge. Those will be
-        merged to the default config before the config from the command line.
+            merged to the default config before the config from the command line.
         :param fallback: config path or dictionary, or list of config paths or dictionaries to fall back to if no config
-        was detected in the argv
+            was detected in the argv
         :param default_config_path: default config's path or dictionary
         :param overwriting_regime: can be "auto-save" (default, when a param is overwritten it is merged instead and the
-        config is saved automatically if it had been saved previously), "locked" (params can't be overwritten except
-        using merge explicitly) or "unsafe" (params can be freely overwritten but reproducibility is not guaranteed).
+            config is saved automatically if it had been saved previously), "locked" (params can't be overwritten except
+            using merge explicitly) or "unsafe" (params can be freely overwritten but reproducibility
+            is not guaranteed).
         :param do_not_merge_command_line: if True, does not try to merge the command line parameters
         :param do_not_pre_process: if true, pre-processing is deactivated in this initialization
         :param do_not_post_process: if true, post-processing is deactivated in this initialization
         :param kwargs: additional parameters to pass to Configuration
         :raises TypeError: if --config is not found and no fallback
         :return: instance of Configuration object containing the desired config
         """
@@ -221,14 +233,15 @@
                                do_not_pre_process=do_not_pre_process, do_not_post_process=do_not_post_process,
                                from_argv=True, **kwargs)
 
     def create_variations(self) -> List['Configuration']:
         """
         Creates a list of configs that are derived from the current config using the internally tracked variations and
         grids registered via the corresponding functions (register_as_config_variations and register_as_grid).
+
         :raises TypeError: if grid dimension is empty or not registered
         :return: the list of configs corresponding to the tracked variations
         """
         variations_names_to_use = [i[0] for i in self._configuration_variations]
         variations_names_to_use_changing = [i[0] for i in self._configuration_variations]
         variations_to_use = [i[1] for i in self._configuration_variations]
         variations_to_use_changing = [i[1] for i in self._configuration_variations]
@@ -298,14 +311,15 @@
                               f"from registered variation parameters.")
         return variation_configs
 
     @staticmethod
     def get_default_config_path() -> str:
         """
         Returns the path to the default config of the project. This function must be implemented at project-level.
+
         :return: string corresponding to the path to the default config of the project
         """
         raise NotImplementedError
 
     def parameters_pre_processing(self) -> Dict[str, Callable]:
         """
         Returns a dictionary where the keys are parameter names (supporting the '*' character as a replacement for any
@@ -344,14 +358,15 @@
         :return: dictionary of the post-processing functions
         """
         raise NotImplementedError
 
     def set_variation_name(self, name: str, deep: bool = False) -> None:
         """
         Sets the variation index of the config. This function is not intended to be used by the user.
+
         :param name: index to set the variation index with
         :param deep: whether to also recursively set the variation name of all sub-configs
         """
         object.__setattr__(self, "_variation_name", name)
         if deep:
             for subconfig in self._sub_configs_list:
                 subconfig.set_variation_name(name, deep=True)
```

### Comparing `yaecs-3.2.4/yaecs/config/config_base.py` & `yaecs-3.2.5/yaecs/config/config_base.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,34 +12,57 @@
     MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
     GNU Lesser General Public License for more details.
 
     You should have received a copy of the GNU Lesser General Public License
     along with this program.  If not, see <https://www.gnu.org/licenses/>.
 """
 
-from collections.abc import Iterable
 import copy
-from functools import partial
 import logging
-from numbers import Real
 import os
-from pathlib import Path
 import sys
-from typing import Any, Callable, Dict, List, Optional, Tuple, Type, TYPE_CHECKING, Union
+from collections.abc import Iterable
+from functools import partial
+from numbers import Real
+from pathlib import Path
+from typing import (
+    TYPE_CHECKING,
+    Any,
+    Callable,
+    Dict,
+    List,
+    Optional,
+    Tuple,
+    Type,
+    Union,
+)
+
 import yaml
 
+from ..yaecs_utils import (
+    YAML_EXPRESSIONS,
+    ConfigDeclarator,
+    TypeHint,
+    adapt_to_type,
+    are_same_sub_configs,
+    compare_string_pattern,
+    compose,
+    format_str,
+    get_order,
+    is_type_valid,
+    parse_type,
+    recursive_set_attribute,
+    set_function_attribute,
+    update_state,
+)
+from .config_convenience import ConfigConvenienceMixin
 from .config_getters import ConfigGettersMixin
 from .config_hooks import ConfigHooksMixin
-from .config_setters import ConfigSettersMixin
-from .config_convenience import ConfigConvenienceMixin
 from .config_processing_functions import ConfigProcessingFunctionsMixin
-
-from ..yaecs_utils import (adapt_to_type, are_same_sub_configs, compare_string_pattern, compose, ConfigDeclarator,
-                           format_str, get_order, is_type_valid, parse_type, recursive_set_attribute,
-                           set_function_attribute, TypeHint, update_state, YAML_EXPRESSIONS)
+from .config_setters import ConfigSettersMixin
 
 if TYPE_CHECKING:
     from .config import Configuration
 
 YAECS_LOGGER = logging.getLogger(__name__)
 
 
@@ -64,14 +87,15 @@
     _state: List[str]
     _verbose: bool
 
     def __init__(self, from_argv: bool = False, do_not_pre_process: bool = False, do_not_post_process: bool = False):
         """
         Should never be called directly by the user. Please use one of the constructors defined for the Configuration
         class instead, or the utils.make_config convenience function.
+
         :param from_argv: whether the config was created with configs passed from the command line arguments
         :param do_not_pre_process: if true, pre-processing is deactivated in this initialization
         :param do_not_post_process: if true, post-processing is deactivated in this initialization
         :raises ValueError: if the overwriting regime is not valid
         :return: none
         """
 
@@ -131,24 +155,26 @@
     def __iter__(self):
         return iter(self._get_user_defined_attributes())
 
     def check_type(self, type_or_types: TypeHint) -> Callable:
         """
         Returns a processing function that checks for given type. Can be used for example with the following line in a
         parameters post-processing dict:
-            "parameter_that_should_be_int": self.check_type(int),
-        - The type can be any of None, bool, int, float, str, dict, list. The value 0 instead means no type check.
-        - Unions are denoted by tuples of types.
-        - You can specify the type of the elements of your lists by using a list of types. This list should contain
-        either one type (in which case the list is expected to only contain elements of that type) or as many types as
-        there are elements in the list (in which case each element is tested with the corresponding type)
-        - You can specify the type of the elements of your dicts by using a dict or a set of types. If you use a set, it
-        can only contain one type (in which case the dict is expected to contain only values of that type). If you use a
-        dict of types, the keys used in that dict that match the keys in the parameter will be checked using the values
-        as types.
+        "parameter_that_should_be_int": self.check_type(int)
+
+        * The type can be any of None, bool, int, float, str, dict, list. The value 0 instead means no type check.
+        * Unions are denoted by tuples of types.
+        * You can specify the type of the elements of your lists by using a list of types. This list should contain
+          either one type (in which case the list is expected to only contain elements of that type) or as many types as
+          there are elements in the list (in which case each element is tested with the corresponding type)
+        * You can specify the type of the elements of your dicts by using a dict or a set of types. If you use a set, it
+          can only contain one type (in which case the dict is expected to contain only values of that type).
+          If you use a dict of types, the keys used in that dict that match the keys in the parameter will be checked
+          using the values as types.
+
         :param type_or_types: type for which to create the function
         :return: the processing function
         """
         def _check_type(value: Any, type_to_check: TypeHint, original_type: TypeHint) -> Any:
             def _wrong_type() -> None:
                 name = self.get_processed_param_name(full_path=False)
                 is_full = original_type == type_to_check
@@ -211,14 +237,15 @@
     def init_from_config(self, config_path_or_dict: ConfigDeclarator) -> None:
         """
         Entrypoint for all methods trying to get any value from outside the config to inside the config. This
         includes creating new parameters when creating the config or merging existing parameters after the creation.
         Users should only use this to merge or create parameters during a creation or merge operation (for instance in a
         processing function). If you want to merge parameters in your main code, outside a constructor or other
         operation, please use self.merge.
+
         :param config_path_or_dict: path or dictionary for the config to merge
         """
         if config_path_or_dict is not None:
             if isinstance(config_path_or_dict, str):
                 with open(self._find_path(config_path_or_dict), encoding='utf-8') as yaml_file:
                     for dictionary_to_add in yaml.load_all(yaml_file, Loader=self._get_yaml_loader()):
                         for item in dictionary_to_add.items():
@@ -227,27 +254,29 @@
                 for item in config_path_or_dict.items():
                     self._process_item_to_merge_or_add(item)
 
     def merge(self, config_path_or_dictionary: ConfigDeclarator, do_not_pre_process: bool = False,
               do_not_post_process: bool = False) -> None:
         """
         Merges provided config path of dictionary into the current config.
+
         :param config_path_or_dictionary: path or dictionary for the config to merge
         :param do_not_pre_process: if true, pre-processing is deactivated in this initialization
         :param do_not_post_process: if true, post-processing is deactivated in this initialization
         """
         self._manual_merge(config_path_or_dictionary=config_path_or_dictionary, do_not_pre_process=do_not_pre_process,
                            do_not_post_process=do_not_post_process)
 
     def merge_from_command_line(self, string_to_merge: Optional[str] = None,
                                 do_not_pre_process: bool = False, do_not_post_process: bool = False) -> None:
         """
         Formerly used to manually merge the command line arguments into the config, which is now done automatically and
         thus should no longer be done manually. Can still be used to manually merge a string emulating command line
         arguments.
+
         :param string_to_merge: if specified, merges this string instead of the sys.argv string
         :param do_not_pre_process: if true, pre-processing is deactivated in this initialization
         :param do_not_post_process: if true, post-processing is deactivated in this initialization
         """
         if self._verbose and string_to_merge is None:
             YAECS_LOGGER.warning("WARNING : merge_from_command_line is now deprecated and will automatically start "
                                  "after using any constructor.\nYou can remove the 'config.merge_from_command_line()' "
```

### Comparing `yaecs-3.2.4/yaecs/config/config_convenience.py` & `yaecs-3.2.5/yaecs/config/config_convenience.py`

 * *Files 5% similar despite different names*

```diff
@@ -12,25 +12,39 @@
     MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
     GNU Lesser General Public License for more details.
 
     You should have received a copy of the GNU Lesser General Public License
     along with this program.  If not, see <https://www.gnu.org/licenses/>.
 """
 
-from copy import deepcopy
 import difflib
-from functools import partial
 import logging
 import os
 import time
-from typing import (Any, Callable, Dict, ItemsView, KeysView, List, Optional, Tuple, Type, TYPE_CHECKING, Union,
-                    ValuesView)
+from copy import deepcopy
+from functools import partial
+from typing import (
+    TYPE_CHECKING,
+    Any,
+    Callable,
+    Dict,
+    ItemsView,
+    KeysView,
+    List,
+    Optional,
+    Tuple,
+    Type,
+    Union,
+    ValuesView,
+)
+
 import yaml
 
 from ..yaecs_utils import compare_string_pattern, dict_apply, format_str
+
 if TYPE_CHECKING:
     from .config import Configuration
 
 YAECS_LOGGER = logging.getLogger(__name__)
 
 
 class ConfigConvenienceMixin:
@@ -79,14 +93,15 @@
 
     def compare(self, other: 'Configuration', reduce: bool = False) -> List[Tuple[str, Optional[Any]]]:
         """
         Returns a list of tuples, where each tuple represents a parameter that is different between the "self"
         configuration and the "other" configuration. Tuples are written in the form :
         (parameter_name, parameter_value_in_other). If parameter_name does not exist in other, (parameter_name, None) is
         given instead.
+
         :param other: config to compare self with
         :param reduce: tries to reduce the size of the output text as much as possible
         :return: difference list
         """
 
         def _investigate_parameter(parameter_name, object_to_check):
             """ Get name and values to display. """
@@ -139,31 +154,33 @@
                 else:
                     differences.append((displayed_name, value_in_other))
         return differences
 
     def copy(self) -> 'ConfigConvenienceMixin':
         """
         Returns a safe, independent copy of the config
+
         :return: instance of Configuration that is a deep copy of the config
         """
         return deepcopy(self)
 
     def details(self, show_only: Optional[Union[str, List[str]]] = None,
                 expand_only: Optional[Union[str, List[str]]] = None, no_show: Optional[Union[str, List[str]]] = None,
                 no_expand: Optional[Union[str, List[str]]] = None) -> str:
         """
         Creates and returns a string describing all the parameters in the config and its sub-configs.
+
         :param show_only: if not None, list of names referring to params. Only params in the list are displayed in the
-        details.
+            details.
         :param expand_only: if not None, list of names referring to sub-configs. Only sub-configs in the list are
-        unrolled in the details.
+            unrolled in the details.
         :param no_show: if not None, list of names referring to params. Params in the list are not displayed in the
-        details.
+            details.
         :param no_expand: if not None, list of names referring to sub-configs. Sub-configs in the list are not unrolled
-        in the details.
+            in the details.
         :return: string containing the details
         """
         constraints = {"show_only": show_only, "expand_only": expand_only, "no_show": no_show, "no_expand": no_expand}
         constraints = dict_apply(constraints, self.match_params)
         string_to_return = "\n" + "\t" * len(self._nesting_hierarchy) + self.get_name().upper() + " CONFIG :\n"
         if not self._nesting_hierarchy:
             string_to_return += "Configuration hierarchy :\n"
@@ -198,50 +215,54 @@
                 string_to_return += str(self[attribute]) + "\n"
         return string_to_return
 
     def items(self, deep: bool = False) -> ItemsView:
         """
         Behaves as dict.items(). If deep is False, sub-configs remain sub-configs in the items. Otherwise, they are
         converted to dict.
+
         :param deep: how to return sub-configs that would appear among the items. If False, do not convert them, else
-        recursively convert them to dict
+            recursively convert them to dict
         :return: the items of the config as in dict.items()
         """
         return self.get_dict(deep).items()
 
     def keys(self) -> KeysView:
         """
         Behaves as dict.keys(), returning a _dict_keys instance containing the names of the params of the config.
+
         :return: the keys if the config as in dict.keys()
         """
         return self.get_dict(False).keys()
 
     def match_params(self, *patterns: Optional[Union[str, List[str]]]) -> Optional[List[str]]:
         """
         For a string, a list of strings or several strings, returns all params matching at least one of the input
         strings.
+
         :param patterns: string, a list of strings or several strings
         :return: all params matching at least one of the input string
         """
         patterns = (patterns[0] if len(patterns) == 1 and isinstance(patterns[0], list) else patterns)
         if patterns is None or (len(patterns) == 1 and patterns[0] is None):
             return None
         new_names = [n.strip(" ") for n in patterns if "*" not in n and n.strip(" ") in self.get_parameter_names(True)]
         for name in [n for n in patterns if "*" in n]:
             new_names = new_names + [p for p in self.get_parameter_names(True) if compare_string_pattern(p, name)]
         return new_names
 
     def save(self, filename: str = None, save_header: bool = True, save_hierarchy: str = True) -> None:
         """
         Saves the current config at the provided location. The saving format allows for a perfect recovery of the config
-        by using : config = Configuration.load_config(filename). If no filename is given, overwrites the last save.
+        by using : `config = Configuration.load_config(filename)`. If no filename is given, overwrites the last save.
+
         :param filename: path to the saving location of the config
         :param save_header: whether to save the config metadata as the fist parameter. This will tag the saved file as a
-        saved config in the eye of the config system when it gets merged, which will deactivate pre-processing
-        :param save_hierarchy: whether to save config hierarchy as a '*_hierarchy.yaml' file
+            saved config in the eye of the config system when it gets merged, which will deactivate pre-processing
+        :param save_hierarchy: whether to save config hierarchy as a `*_hierarchy.yaml` file
         :raises RuntimeError: no file name is provided and there is no previous save to overwrite
         """
         if filename is None:
             if self._was_last_saved_as is None:
                 raise RuntimeError("No filename was provided, but the config was never "
                                    "saved before so there is no previous save to overwrite.")
             filename = self._was_last_saved_as
@@ -269,16 +290,17 @@
         if self._verbose:
             YAECS_LOGGER.info(f"Configuration saved in : {format_str(os.path.abspath(config_dump_path))}.")
 
     def values(self, deep: bool = False) -> ValuesView:
         """
         Behaves as dict.values(). If deep is False, sub-configs remain sub-configs in the values. Otherwise, they are
         converted to dict.
+
         :param deep: how to return sub-configs that would appear among the values. If False, do not convert them, else
-        recursively convert them to dict
+            recursively convert them to dict
         :return: the values of the config as in dict.values()
         """
         return self.get_dict(deep).values()
 
     def _did_you_mean(self, name: str, filter_type: Optional[type] = None, suffix: str = "") -> str:
         """ Used to propose suggestions when the user tries to access a parameter which does not exist. """
         all_params = self.get_parameter_names(True)
@@ -313,15 +335,15 @@
             # pylint: disable=bad-continuation
             return yaml_dumper.represent_mapping(
                 "!" + class_instance.get_name().split("_VARIATION_")[0], {
                     a[3:] if a.startswith("___") else a: self._format_metadata() if a == "config_metadata" else
                     (b if (".".join(class_instance.get_nesting_hierarchy()
                                     + [a]) not in self.get_main_config().get_pre_post_processing_values()) else
                         (self.get_main_config().get_pre_post_processing_values(
-                             )[".".join(class_instance.get_nesting_hierarchy() + [a])]))
+                        )[".".join(class_instance.get_nesting_hierarchy() + [a])]))
                     for (a, b) in class_instance.__dict__.items()
                     if a not in self._protected_attributes
                     and not (class_instance.get_nesting_hierarchy() and a in ["config_metadata"])
                 },
             )
 
         dumper = yaml.Dumper
```

### Comparing `yaecs-3.2.4/yaecs/config/config_getters.py` & `yaecs-3.2.5/yaecs/config/config_getters.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,17 +13,18 @@
     GNU Lesser General Public License for more details.
 
     You should have received a copy of the GNU Lesser General Public License
     along with this program.  If not, see <https://www.gnu.org/licenses/>.
 """
 
 import logging
-from typing import Any, Callable, Dict, List, Optional, Tuple, TYPE_CHECKING, Union
+from typing import TYPE_CHECKING, Any, Callable, Dict, List, Optional, Tuple, Union
+
+from ..yaecs_utils import TypeHint, escape_symbols, get_param_as_parsable_string
 
-from ..yaecs_utils import get_param_as_parsable_string, escape_symbols, TypeHint
 if TYPE_CHECKING:
     from .config import Configuration
 
 YAECS_LOGGER = logging.getLogger(__name__)
 
 
 class ConfigGettersMixin:
@@ -47,58 +48,62 @@
 
     def __init__(self, *args, **kwargs):
         super().__init__(*args, **kwargs)
 
     def get(self, parameter_name: str, default_value: Any) -> Any:
         """
         Behaves similarly to dict.get(parameter_name, default_value)
+
         :param parameter_name: parameter to query
         :param default_value: value to return if the parameter does not exist
         :return: queried value
         """
         try:
             return self[parameter_name]
         except (AttributeError, TypeError):
             return default_value
 
     def get_all_linked_sub_configs(self) -> List['Configuration']:
         """
         Returns the list of all sub-configs that are directly linked to the root config by a chain of other sub-configs.
         For this to be the case, all of those sub-configs need to be contained directly in a parameter of another
         sub-config. For example, a sub-config stored in a list that is a parameter of a sub-config is not linked.
+
         :return: list corresponding to the linked sub-configs
         """
         all_linked_configs = []
         for i in self._get_user_defined_attributes():
             object_to_scan = getattr(self, "___" + i if i in self._methods else i)
             if isinstance(object_to_scan, ConfigGettersMixin):
                 all_linked_configs = (all_linked_configs + [object_to_scan]
                                       + object_to_scan.get_all_linked_sub_configs())
         return all_linked_configs
 
     def get_all_sub_configs(self) -> List['Configuration']:
         """
         Returns the list of all sub-configs, including sub-configs of other sub-configs
+
         :return: list corresponding to the sub-configs
         """
         all_configs = list(self._sub_configs_list)
         for i in self._sub_configs_list:
             all_configs = all_configs + i.get_all_sub_configs()
         return all_configs
 
     def get_command_line_argument(self, deep: bool = True, do_return_string: bool = False,
                                   ignore_unknown_types: bool = False,
                                   ) -> Union[List[str], str]:
         """
         Returns a list of command line parameters that can be used in a bash shell to re-create this exact config
         from the default. Can alternatively return the string itself with do_return_string=True.
+
         :param deep: whether to also take the sub-config parameters into account
         :param do_return_string: whether to return a string (True) or a list of strings (False, default)
         :param ignore_unknown_types: if False (default), types that cannot be parsed in YAML raise an error. Else, they
-        are skipped when creating the list.
+            are skipped when creating the list.
         :return: list or string containing the parameters
         """
         to_return = []
         for param in self.get_parameter_names(deep=deep):
             if not isinstance(self[param], ConfigGettersMixin):
                 full_name = self._get_full_path(param)
                 pair = get_param_as_parsable_string(
@@ -114,68 +119,75 @@
                     to_return.append(escape_symbols(f"--{param} {pair}", ["{", "}", "*"]))
 
         return " ".join(to_return) if do_return_string else to_return
 
     def get_dict(self, deep: bool = True) -> dict:
         """
         Returns a dictionary corresponding to the config.
+
         :param deep: whether to recursively turn sub-configs into dicts or keep them as sub-configs
         :return: dictionary corresponding to the config
         """
         return {
             key: (self[key] if not deep or not isinstance(self[key], ConfigGettersMixin)
                   else self[key].get_dict())
             for key in self._get_user_defined_attributes()
         }
 
     def get_main_config(self) -> 'Configuration':
         """
         Getter for the main config corresponding to this config or sub-config. Using this is often hacky.
+
         :return: the main config
         """
         return self._main_config
 
     def get_master_switch(self, processing_type: str) -> bool:
         """
         Getter for either the pre- or post-processing master switch depending on processing_type
+
         :param processing_type: can be 'pre' or 'post' : processing type to get the master switch for
         :return: the main config
         """
         return self._pre_process_master_switch if processing_type == "pre" else self._post_process_master_switch
 
     def get_modified_buffer(self) -> List[str]:
         """
         Getter for the buffer of modified parameters corresponding to this config or sub-config. This gets filled during
         a creation or merging operation to keep track of all the parameters modified by this operation. Then, it is
         emptied as all modified parameters get post-processed before the end of the operation.
+
         :return: the buffer of modified elements
         """
         return self._modified_buffer
 
     def get_name(self) -> str:
         """
         Returns the name of the config. It is composed of a specified part (or 'main' when unspecified) and an indicator
         of its index in the list of variations of its parent if it is a variation of a config. This indicator is
         prefixed by '_VARIATION_'.
+
         :return: string corresponding to the name
         """
         variation_suffix = ("_VARIATION_" + self._variation_name if self._variation_name is not None else "")
         return self._name + variation_suffix
 
     def get_nesting_hierarchy(self) -> List[str]:
         """
         Returns the nesting hierarchy of the config
+
         :return: list corresponding to the nesting hierarchy
         """
         return self._nesting_hierarchy
 
     def get_parameter_names(self, deep: bool = True, no_sub_config: bool = False) -> List[str]:
         """
         Returns the list of the names all parameters in this config. If deep is true, also returns the names of the
         parameters in the sub-configs using the dot convention.
+
         :param deep: whether to also return the names of the parameters in the sub-configs
         :param no_sub_config: if True, exclude names of sub-configs and only return real parameters
         :return: the list of the names of all parameters
         """
         complete_list = self._get_user_defined_attributes(no_sub_config=no_sub_config)
         if deep:
             order = len(self.get_nesting_hierarchy())
@@ -185,74 +197,84 @@
                     for param in subconfig.get_parameter_names(deep=False, no_sub_config=no_sub_config)
                 ]
         return complete_list
 
     def get_pre_post_processing_values(self) -> Dict[str, Any]:
         """
         Returns a dictionary containing :
-        - as keys : all the names of the parameters which have been post-processed
-        - as values : the values those parameters had before the post-processing operation
+
+        * as keys : all the names of the parameters which have been post-processed
+        * as values : the values those parameters had before the post-processing operation
+
         In particular, those values are the ones used when saving the config.
+
         :return: dictionary of values before post-processing
         """
         return self._pre_postprocessing_values
 
     def get_processed_param_name(self, full_path: bool = True) -> str:
         """
         When used in a processing function, returns the full path to that param in the config, or its path in self if
         full_path is False.
+
         :param full_path: if True, returns the path to the param in the main config, otherwise the path to the param in
-        self.
+            self.
         """
         if full_path:
             return self._get_full_path(self._get_param_name_from_state())
         return self._get_param_name_from_state()
 
     def get_save_file(self) -> Optional[str]:
         """
         If the config was saved previously, returns the path to this save. Otherwise, returns None.
+
         :return: the path to the save if it exists, None otherwise
         """
         return self._was_last_saved_as
 
     def get_reference_folder(self) -> Optional[str]:
         """
         If a reference folder has been registered, returns it. Otherwise, returns None.
+
         :return: the reference folder if it exists, None otherwise
         """
         return self._reference_folder
 
     def get_type_hint(self, param_name) -> TypeHint:
         """
         Returns the type hint for this param, or 0 if it has no type hint.
+
         :return: possible types for this param according to its type hint, 0 if no type hint defined
         """
         if param_name in self._type_hints:
             return self._type_hints[param_name]
         if "." in param_name:
             return self[".".join(param_name.split(".")[:-1])].get_type_hint(param_name.split(".")[-1])
         return 0
 
     def get_type_hints(self) -> Dict[str, TypeHint]:
         """
         Returns all the type hints for this config
+
         :return: dictionary with keys being parameter names and values being their possible types
         """
         return self._type_hints
 
     def get_variation_name(self) -> str:
         """
         Returns the variation name of the config
+
         :return: variation name
         """
         return self._variation_name
 
     def is_in_operation(self) -> bool:
         """
         Returns whether the config is currently in a creation or merging process.
+
         :return: True if the config is in a creation or merging process, False otherwise
         """
         return self._operating_creation_or_merging
 
     def _get_full_path(self, param_name: str) -> str:
         """ Get the full name of given param in the main config """
         return ".".join(self._nesting_hierarchy + [param_name])
```

### Comparing `yaecs-3.2.4/yaecs/config/config_hooks.py` & `yaecs-3.2.5/yaecs/config/config_hooks.py`

 * *Files 2% similar despite different names*

```diff
@@ -16,21 +16,29 @@
     along with this program.  If not, see <https://www.gnu.org/licenses/>.
 """
 
 import logging
 import os
 from typing import Any, Callable, List, Optional, Tuple, Union
 
-from ..yaecs_utils import assign_order, assign_yaml_tag, ConfigDeclarator, hook, Hooks, Priority, VariationDeclarator
+from ..yaecs_utils import (
+    ConfigDeclarator,
+    Hooks,
+    Priority,
+    VariationDeclarator,
+    assign_order,
+    assign_yaml_tag,
+    hook,
+)
 
 YAECS_LOGGER = logging.getLogger(__name__)
 
 
 class ConfigHooksMixin:
-    """ Hooks Mixin class for YAECS configurations. Implements processing functions whose name start with "register_as_"
+    """ Hooks Mixin class for YAECS configurations. Implements processing functions whose name start with `register_as_`
     and are decorated by the yaecs_utils.hook decorator. Users can use those processing either as pre- or
     post-processing functions, which will have the added effect of tagging the processed parameters as playing a certain
     pre-defined role in the config """
 
     __getattribute__: Callable[[str], Any]
     get_processed_param_name: Callable[[bool], str]
     get_variation_name: Callable[[], str]
@@ -44,26 +52,28 @@
         self._hooks = {}
         super().__init__(*args, **kwargs)
 
     def add_currently_processed_param_as_hook(self, hook_name: str) -> None:
         """
         Used within _ConfigurationBase._process_parameter to add the param currently being processed as a hook with
         given name. Instead of using this directly, users should consider decorating their hooking function with the
-        yaecs_utils.hook decorator.
+        `yaecs_utils.hook` decorator.
+
         :param hook_name: name of the hook to add.
         """
         parameter = self.get_processed_param_name(full_path=True)
         if hook_name not in self.get_hook():
             self._hooks[hook_name] = []
         if parameter not in self._hooks[hook_name]:
             self._hooks[hook_name].append(parameter)
 
     def get_experiment_path(self) -> str:
         """
         Returns the value of the parameter registered as the experiment path.
+
         :raises RuntimeError: when no experiment path has been registered in the config
         :raises RuntimeError: when more than one experiment path has been registered in the config
         :return: experiment path
         """
         path = self.get_hook("experiment_path")
         if not path:
             raise RuntimeError("No experiment path was registered. Please use self.register_as_experiment_path as a "
@@ -72,29 +82,29 @@
             raise RuntimeError("The self.register_as_experiment_path post-processing was used on more than one "
                                f"parameter : {path}.")
         return self[path[0]]
 
     def get_hook(self, hook_name: Optional[str] = None) -> Hooks:
         """
         Returns the parameters registered with given hook.
+
         :param hook_name: name of the hook, or None to get the dict of all hooked parameters
         :return: list of hooked parameter names
         """
         if hook_name is None:
             return self._hooks
         return self._hooks[hook_name] if hook_name in self._hooks else []
 
     @hook("additional_config_file")
     @assign_order(Priority.OFTEN_LAST)  # processing this param after this function makes it unclear which file was used
     @assign_yaml_tag("additional_config_file", "pre", "Optional[Union[str,List[str]]]")
     def register_as_additional_config_file(self, path: Union[str, List[str]]) -> Union[str, List[str]]:
         """
         Pre-processing function used to register the corresponding parameter as a path to another config file. The new
         config file will then also be used to build the config currently being built.
-
         Priority : OFTEN_LAST (10)
         YAML tag : additional_config_file
 
         :param path: config's path or list of paths
         :return: the same path as the input once the parameters from the new config have been added
         """
         if isinstance(path, list):
@@ -108,15 +118,14 @@
     @assign_order(Priority.INDIFFERENT)  # does not depend on or change parameter value, only processes parameter name
     @assign_yaml_tag("config_variations", "pre", "Optional[Union[List[Union[str,dict]],Dict[Union[str,dict]]]]")
     def register_as_config_variations(
             self, variation_to_register: Optional[VariationDeclarator]) -> Optional[VariationDeclarator]:
         """
         Pre-processing function used to register the corresponding parameter as a variation for the current config.
         Please note that config variations need to be declared in the root config.
-
         Priority : INDIFFERENT (0)
         YAML tag : config_variations
 
         :param variation_to_register: list of configs
         :return: the same list of configs once the configs have been added to the internal variation tracker
         :raises RuntimeError: register_as_config_variations is called outside _pre_process_parameter
         :raises RuntimeError: variation name invalid in sub-config
@@ -161,15 +170,14 @@
     def register_as_experiment_path(self, path: Optional[str]) -> Optional[str]:
         """
         Pre-processing function used to register the corresponding parameter as the folder used for the current
         experiment. This will automatically create the relevant folder structure and append an experiment index at the
         end of the folder name to avoid any overwriting. The path needs to be either None or an empty string (in which
         case the pre-processing does not happen), or an absolute path, or a path relative to the current working
         directory.
-
         Priority : OFTEN_FIRST (-10)
         YAML tag : experiment_path
 
         :param path: None, '', absolute path or path relative to the current working directory
         :return: the actual created path with its appended index
         """
         if not path:
@@ -198,15 +206,14 @@
     @assign_order(Priority.INDIFFERENT)  # does not depend on or change parameter value, only processes parameter name
     @assign_yaml_tag("grid", "pre", "Optional[List[str]]")
     def register_as_grid(self, list_to_register: Optional[List[str]]) -> Optional[List[str]]:
         """
         Pre-processing function used to register the corresponding parameter as a grid for the current config. Grids are
         made of several parameters registered as variations. Instead of adding the variations in those parameters to the
         list of variations for this config, a grid will be created and all its components will be added instead.
-
         Priority : INDIFFERENT (0)
         YAML tag : grid
 
         :param list_to_register: list of parameters composing the grid
         :raises TypeError: list_to_register is not recognised as a valid grid
         :return: the same list of parameters once the grid has been added to the internal grid tracker
         """
@@ -222,15 +229,14 @@
     @assign_yaml_tag("tracker_config", "pre", "dict")
     def register_as_tracker_config(self, tracker_config: dict) -> dict:  # pylint: disable=no-self-use
         """
         Pre-processing function used to register the corresponding parameter as the tracker config. The tracker config
         is a dict that contains at least one key : 'type'. Valid types are given by the 'ACCEPTED_TRACKERS' variable in
         experiment.py and refer to the type of tracker used. Other keys in the dict depend on the parameters required by
         corresponding tracker type.
-
         Priority : INDIFFERENT (0)
         YAML tag : tracker_config
 
         :param tracker_config: dict corresponding to the tracker config
         :raises: ValueError: if the tracker config is not a dict or does not contain at least a parameter called 'type'
         which is a string
         :raises: ValueError: if the 'type' is not recognised
```

### Comparing `yaecs-3.2.4/yaecs/config/config_processing_functions.py` & `yaecs-3.2.5/yaecs/config/config_processing_functions.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,25 @@
 """ This file defines a library of convenient processing functions. """
 
-from functools import partial
 import logging
 import os
-from typing import Any, Callable, List, Optional, TYPE_CHECKING
+from functools import partial
+from typing import TYPE_CHECKING, Any, Callable, List, Optional
 
-from ..yaecs_utils import assign_order, assign_yaml_tag, compare_string_pattern, Priority, set_function_attribute
+from ..yaecs_utils import (
+    Priority,
+    assign_order,
+    assign_yaml_tag,
+    compare_string_pattern,
+    set_function_attribute,
+)
 
 if TYPE_CHECKING:
     from numbers import Number
+
     from .config import Configuration
 
 YAECS_LOGGER = logging.getLogger(__name__)
 
 
 class ConfigProcessingFunctionsMixin:
     """ Pre- and Post-processing functions Mixin class for YAECS configurations. """
@@ -26,15 +33,16 @@
     # ----- PRE-PROCESSING -----
 
     def check_param_in_list(self, list_of_choices: List[Any]) -> Callable:
         """
         Returns a pre-processing function that checks if a param value belongs to a list. Returned function has
         order OFTEN_FIRST (-10).
         For example in your pre-processing dict there could be a line such as this :
-            "mode": self.check_param_in_list(["train", "val", "test", "infer"]),
+        "mode": self.check_param_in_list(["train", "val", "test", "infer"])
+
         :param list_of_choices: list of valid parameter values
         :return: checking function
         """
 
         def _check(param: Any, choices: List[Any], config: 'Configuration') -> Any:
             if param is None:
                 return param
@@ -58,15 +66,14 @@
     @assign_yaml_tag("copy", "pre", "str")
     def copy_param(self, path_to_copy: str) -> str:
         """
         This pre-processing function declares a param as being an exact copy of another param. Its default value must
         be name of the param it copies. It will be protected against modifications by further config merges (only the
         param being copied can be modified), but can still pe post-processed further after its copy by post-processing
         functions with an order above OFTEN_LAST (10).
-
         Priority : ALWAYS_LAST (20)
         YAML tag : copy
 
         :param path_to_copy: path of param from which to copy the value
         :return: path_to_copy
         """
 
@@ -99,15 +106,16 @@
         return self.protected_param(path_to_copy)
 
     def check_number_in_range(self, minimum: 'Number' = -float('inf'), maximum: 'Number' = float('inf')) -> Callable:
         """
         Returns a pre-processing function that checks if a numerical param value is in a range. Returned function has
         order OFTEN_FIRST (-10).
         For example in your pre-processing dict there could be a line such as this :
-            "probability": self.number_in_range(minimum=0, maximum=1),
+        "probability": self.number_in_range(minimum=0, maximum=1)
+
         :param minimum: minimal valid value for the parameter
         :param maximum: maximal valid value for the parameter
         :return: checking function
         """
 
         def _check(param: 'Number', minimum_: 'Number', maximum_: 'Number', config: 'Configuration') -> 'Number':
             if param is None:
@@ -124,15 +132,14 @@
 
     @assign_order(Priority.ALWAYS_LAST)  # there can never be any subsequent processing for this param
     @assign_yaml_tag("protected", "pre", "Any")
     def protected_param(self, param: Any) -> Any:
         """
         This pre-processing function declares a param as being protected against modifications. This means that only the
         default config can change its value, and any attempt to set it from another config will raise an error.
-
         Priority : ALWAYS_LAST (20)
         YAML tag : protected
 
         :param param: value of the param to protect
         :return: param
         """
         main = self.get_main_config()
@@ -147,15 +154,14 @@
 
     @assign_order(Priority.OFTEN_LAST)  # should happen after register_as_experiment_path
     @assign_yaml_tag("sub_folder", "post", "Optional[str]")
     def folder_in_experiment(self, folder: Optional[str]) -> Optional[str]:
         """
         Returns a post-processing function that extends a path assuming it is located in the experiment path, then the
         corresponding folder is created. Requires an experiment_folder to have been declared.
-
         Priority : OFTEN_LAST (10)
         YAML tag : sub_folder
 
         :param folder: path of the subfolder within the experiment folder
         :return: checking function
         """
         experiment_path = self.get_main_config().get_experiment_path()
@@ -165,21 +171,23 @@
 
     def folder_in_experiment_if(self, condition_list: List[tuple] = None) -> Callable:
         """
         Returns a post-processing function that extends a path assuming it is located in the experiment path. Then, if
         the conditions listed in condition_list ar all met, the corresponding folder is created. Returned function has
         order OFTEN_LAST (10).
         condition_list is a list of conditions represented by tuples of length 2 or 3 :
-        - when a condition is represented by a tuple of length 2, the first element should be the path to parameters in
-        the main config and the second element should be a value for those parameters. The condition will return true if
-        the corresponding parameters have the corresponding value ;
-        - when a condition is represented by a tuple of length 3, the behaviour is the same except the third element is
-        a function to apply to the parameters values before they are compared to the second element.
-        For example in your post-processing dict there could be a line such as this :
-            "save_weights_path": self.folder_in_experiment(condition_list=[("mode", "train")]),
+
+        * when a condition is represented by a tuple of length 2, the first element should be the path to parameters in
+          the main config and the second element should be a value for those parameters. The condition will return true
+          if the corresponding parameters have the corresponding value ;
+        * when a condition is represented by a tuple of length 3, the behaviour is the same except the third element is
+          a function to apply to the parameters values before they are compared to the second element.
+          For example in your post-processing dict there could be a line such as this :
+          "save_weights_path": self.folder_in_experiment(condition_list=[("mode", "train")])
+
         :param condition_list: list of conditions to be met for the path to be created
         :return: checking function
         """
 
         def _folder_in_experiment(folder: str, config: 'Configuration', conditions: list) -> str:
             experiment_path = config.get_experiment_path()
             path = os.path.join(experiment_path, folder).rstrip(os.path.sep)
```

### Comparing `yaecs-3.2.4/yaecs/config/config_setters.py` & `yaecs-3.2.5/yaecs/config/config_setters.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,17 +12,18 @@
     MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
     GNU Lesser General Public License for more details.
 
     You should have received a copy of the GNU Lesser General Public License
     along with this program.  If not, see <https://www.gnu.org/licenses/>.
 """
 import logging
-from typing import Any, Callable, Dict, TYPE_CHECKING, Union
+from typing import TYPE_CHECKING, Any, Callable, Dict, Union
 
 from ..yaecs_utils import TypeHint
+
 if TYPE_CHECKING:
     from .config import Configuration
 
 YAECS_LOGGER = logging.getLogger(__name__)
 
 
 class ConfigSettersMixin:
@@ -47,19 +48,20 @@
         new_processing = {set_name: function_to_add, **current_processing}
         object.__setattr__(self, attribute, new_processing)
 
     def add_processing_function_all(self, param_name: str, function_to_add: Union[str, Callable], processing_type: str
                                     ) -> None:
         """
         Triggers add_processing_function on the main config and all defined and future sub-configs.
+
         :param param_name: parameter(s) to which to add a postprocessing function. Expects paths with respect to the
-        main config.
+            main config.
         :param function_to_add: postprocessing function to add, using the generic name "function" if it has no name
         :param processing_type: choose between 'pre' to add a pre-processing function or 'post' to add a post-processing
-        function
+            function
         """
         if isinstance(function_to_add, str):
             check_function = self._assigned_as_yaml_tags[function_to_add[len("_tagged_method_"):]][0]
         else:
             check_function = function_to_add
         if hasattr(check_function, "assigned_yaml_tag"):
             if check_function.assigned_yaml_tag[1] != processing_type:
@@ -82,52 +84,58 @@
             set_name = set_name + " "
         new_processing = {set_name: function_to_add, **current_added_processing}
         setattr(self.__class__, attribute, lambda self: new_processing)
 
     def add_type_hint(self, name: str, type_hint: TypeHint) -> None:
         """
         Adds a type hint for a parameter to the list of type hints for automatic type checks.
+
         :param name: full path of the param in the main config
         :param type_hint: type of the param
         """
         self._type_hints[name] = type_hint
 
     def remove_value_before_postprocessing(self, name: str) -> None:
         """
         Function used for bookkeeping : it remove a parameter from the pre-post-processing archive.
+
         :param name: name of the parameter using the dot convention
         """
         if name in self._pre_postprocessing_values:
             del self._pre_postprocessing_values[name]
 
     def remove_type_hint(self, param_name: str) -> None:
         """
-        Removes a registered type hint from a param with given name
+        Removes a registered type hint from a param with given name.
+
         :param param_name: param from which to remove the type hint
         """
         if param_name in self._type_hints:
             del self._type_hints[param_name]
 
     def save_value_before_postprocessing(self, name: str, value: Any) -> None:
         """
         Function used for bookkeeping : it saves the value a parameter had before its post-processing.
+
         :param name: name of the parameter using the dot convention
         :param value: value of the parameter before post-processing
         """
         if name not in self._pre_postprocessing_values:
             self._pre_postprocessing_values[name] = value
 
     def set_post_processing(self, value: bool = True) -> None:
         """
         Sets the state of the master switch for pre-processing across the entire config object. Calling this for a
         sub-config will also affect the main config and all other sub-configs.
+
         :param value: value to set the pre-processing to
         """
         object.__setattr__(self._main_config, "_post_process_master_switch", value)
 
     def set_pre_processing(self, value: bool = True) -> None:
         """
         Sets the state of the master switch for pre-processing across the entire config object. Calling this for a
         sub-config will also affect the main config and all other sub-configs.
+
         :param value: value to set the pre-processing to
         """
         object.__setattr__(self._main_config, "_pre_process_master_switch", value)
```

### Comparing `yaecs-3.2.4/yaecs/config_history.py` & `yaecs-3.2.5/yaecs/config_history.py`

 * *Files identical despite different names*

### Comparing `yaecs-3.2.4/yaecs/experiment.py` & `yaecs-3.2.5/yaecs/experiment.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,20 +13,20 @@
     GNU Lesser General Public License for more details.
 
     You should have received a copy of the GNU Lesser General Public License
     along with this program.  If not, see <https://www.gnu.org/licenses/>.
 """
 import importlib.util
 import logging
+import os
 import sys
+import traceback
 from contextlib import ExitStack
-import os
 from functools import partial
-import traceback
-from typing import Optional, Callable, Dict, List, Any, Tuple, Union
+from typing import Any, Callable, Dict, List, Optional, Tuple, Union
 
 from mock import patch
 
 from .config.config import Configuration
 from .yaecs_utils import add_to_csv, compare_string_pattern, lazy_import, new_print
 
 # ClearML integration, see original package : https://clear.ml
@@ -49,28 +49,29 @@
                  experiment_name: Optional[str] = None, run_name: Optional[str] = None,
                  params_filter_fn: Optional[Callable[[Configuration],
                                                      List[str]]] = None, log_modified_params_only: bool = True,
                  only_params_to_log: Optional[List[str]] = None, params_not_to_log: Optional[List[str]] = None,
                  description_formatter: Optional[Callable[[Optional[str]], str]] = None):
         """
         Creates an instance of the Experiment class, which wraps around a main function.
+
         :param config: config used for the experiment
         :param main_function: function to run to perform the experiment
         :param experiment_name: name of the experiment, defaults to name
-        of the folder set as experiment path in the config
+            of the folder set as experiment path in the config
         :param run_name: name of the run, defaults as the index of the run in the experiment folder
         :param params_filter_fn: function to use instead of the default filter to get the list of the names of the
-        parameters to log to the tracker from the config. If this is used, then 'log_modified_params_only',
-        'only_params_to_log' and 'params_not_to_log' are ignored.
+            parameters to log to the tracker from the config. If this is used, then 'log_modified_params_only',
+            'only_params_to_log' and 'params_not_to_log' are ignored.
         :param log_modified_params_only: whether the parameters to filter using the other arguments are the parameters
-        that changed compared to the default config (True) or only those of the whole config (False)
+            that changed compared to the default config (True) or only those of the whole config (False)
         :param only_params_to_log: if provided, only the parameters whose names are given will be filtered and logged
         :param params_not_to_log: if provided, parameters whose names are given will be filtered out
         :param description_formatter: optional function to use to format the provided run description instead of the
-        default formatter self.default_formatter
+            default formatter self.default_formatter
         """
         self.config = config
         self.main_function = main_function
         if not hasattr(self, "number_of_runs"):
             self.number_of_runs = None
         self.current_run = None
         self.format_description = self.default_formatter if description_formatter is None else description_formatter
@@ -86,16 +87,17 @@
                                self, experiment_name=experiment_name, run_name=run_name,
                                params_filter_fn=params_filter_fn, log_modified_params_only=log_modified_params_only,
                                only_params_to_log=only_params_to_log, params_not_to_log=params_not_to_log)
 
     def default_formatter(self, description: Optional[str]) -> str:
         """
         This function formats the provided description before passing it to the trackers.
-        :param description: provided description to format. You can use the tag %h once in the description. Everything
-        before this tag will be considered the header of the description
+
+        :param description: provided description to format. You can use the tag `%h` once in the description. Everything
+            before this tag will be considered the header of the description
         :raises RuntimeError: when more than one header tag is detected in the description
         :return: formatted description
         """
         description = description if description else "unstated purpose"
         header = ""
         if "%h" in description:
             if description.count("%h") > 1:
@@ -104,16 +106,18 @@
             header = f"[{self.current_run + 1}/{self.number_of_runs}] {header}\n"
         description = f"{header}Purpose : {description}"
         return description
 
     def run(self, run_description: Optional[str] = None, **kwargs) -> Any:
         """
         Creates all variations of the config and starts a run for each of them.
+
         :param run_description: if passed, will serve as a description for the purpose of the current run. You can use
-        the tag %h once in the description. Everything before this tag will be considered the header of the description
+            the tag %h once in the description. Everything before this tag will be considered the header
+            of the description
         :param kwargs: arguments to pass to the main function aside from the config and the tracker
         :return: whatever the main function returns
         """
         variations = self.config.create_variations()
         self.number_of_runs = len(variations)
         description = run_description
         returns = []
@@ -141,16 +145,18 @@
                     description = f"Variation {variation.get_variation_name()}%h{description}"
             returns.append(self.run_single(description, **kwargs))
         return returns
 
     def run_single(self, run_description: Optional[str] = None, **kwargs) -> Any:
         """
         Runs a single experiment with the defined config. Does not check the config variations.
+
         :param run_description: if passed, will serve as a description for the purpose of the current run. You can use
-        the tag %h once in the description. Everything before this tag will be considered the header of the description
+            the tag %h once in the description. Everything before this tag will be considered the header
+            of the description
         :param kwargs: arguments to pass to the main function aside from the config and the tracker
         :return: whatever the main function returns
         """
         if os.getenv('NODE_RANK'):  # do not track if in a pytorch-lightning spawned process
             description = None
         else:
             description = (input("[TRACKER] Please describe the purpose of this run : ")
@@ -190,23 +196,24 @@
 
     def __init__(self, tracker_config: Dict[str, Any], experiment: Experiment, experiment_name: Optional[str] = None,
                  run_name: Optional[str] = None, params_filter_fn: Optional[Callable] = None,
                  log_modified_params_only: bool = True, only_params_to_log: Optional[List[str]] = None,
                  params_not_to_log: Optional[List[str]] = None):
         """
         Reads the tracker config from the general config to create a Tracker object used for logging during the run.
+
         :param tracker_config: tracker config from the general config
         :param experiment: passed automatically from the instance of Experiment this tracker originates from
         :param experiment_name: name for the experiment (inferred from the experiment path if not provided)
         :param run_name: name for the run (inferred from the experiment path if not provided)
         :param params_filter_fn: function to use instead of the default filter to get the list of the names of the
-        parameters to log to the tracker from the config. If this is used, then 'log_modified_params_only',
-        'only_params_to_log' and 'params_not_to_log' are ignored.
+            parameters to log to the tracker from the config. If this is used, then 'log_modified_params_only',
+            'only_params_to_log' and 'params_not_to_log' are ignored.
         :param log_modified_params_only: whether the parameters to filter using the other arguments are the parameters
-        that changed compared to the default config (True) or only those of the whole config (False)
+            that changed compared to the default config (True) or only those of the whole config (False)
         :param only_params_to_log: if provided, only the parameters whose names are given will be filtered and logged
         :param params_not_to_log: if provided, parameters whose names are given will be filtered out
         """
         # Do not track if in a pytorch-lightning spawned process.
         self.types = [] if os.getenv('NODE_RANK') else tracker_config['type']
         if "clearml" in self.types:
             if not os.path.isfile(os.path.expanduser("~/clearml.conf")):
@@ -246,14 +253,15 @@
         """
         Default parameters filtering function. Uses the pre-defined 'log_modified_params_only', 'only_params' and
         'except_params' attributes to filter out the parameters of the config.
         It starts with a list of all the params which were modified from the default config, except if
         log_modified_params_only was set to False in which case it starts from all the parameters in the config. Then,
         it filters out all hooks, then all parameters in except_params, and finally only keeps those that are also in
         only_params.
+
         :param config: instance of Configuration from which to filter the parameters
         :return: the list of the filtered parameters names
         """
         # Get params to filter
         if self.log_modified_params_only:
             default = config.__class__.build_from_configs(config.config_metadata["config_hierarchy"][0],
                                                           do_not_post_process=True, do_not_merge_command_line=True,
@@ -279,14 +287,15 @@
         return to_ret
 
     def extract_names(self) -> Tuple[str, str]:
         """
         Gets experiment and run names, using either names given when instantiating the Experiment (if provided) or
         inferring them from the config's experiment path. If nothing is provided and no experiment path is defined,
         raises an error.
+
         :raises RuntimeError: if no experiment path is defined in the config and no experiment or run name is provided
         :return: the experiment name and the run name
         """
         try:
             name_from_config = self.experiment.config.get_experiment_path()
         except RuntimeError:
             name_from_config = None
@@ -314,15 +323,15 @@
                 run_name = name_from_config.split(os.sep)[-2].split("_")[-1] + "_" + name_from_config.split(os.sep)[-1]
         else:
             run_name = self.run_name
         return exp_name, run_name
 
     def start_run(self, description: Optional[str] = None) -> None:
         """
-        Initialises the configured trackers, which most of the time means preparing their logger is self.loggers.
+        Initializes the configured trackers, which most of the time means preparing their logger is self.loggers.
         """
         experiment_name, run_name = self.extract_names()
         config = self.experiment.config
         params_to_log = {k: config[config.match_params("*" + k)[0]] for k in self.get_filtered_params(config)}
         for tracker_type in self.types:
             if tracker_type != "basic":
                 module = "tensorflow" if tracker_type == "tensorboard" else tracker_type
@@ -368,20 +377,21 @@
 
     def log_scalar(self, name: str, value: Union[float, int], step: Optional[int] = None,
                    sub_logger: Optional[str] = None, description: Optional[str] = None,
                    main_process_only: bool = False) -> None:
         """
         Logs the given value under the given name at given step in the configured trackers. The description is optional
         and can only be used if the tracker is tensorboard.
+
         :param name: name for the value to be logged
         :param value: value to be logged
         :param step: step at which the value is logged. If not provided, will default to 0 for the tensorboard tracker,
-        will default to -1 for the basic tracker and will be logged as a "single value" for the clearml tracker
+            will default to -1 for the basic tracker and will be logged as a "single value" for the clearml tracker
         :param sub_logger: if specified, logs to corresponding sub-logger. Can be interpreted as a sub-folder for the
-        scalar name most of the time, but in the case of tensorboard will actually use a different summary writer
+            scalar name most of the time, but in the case of tensorboard will actually use a different summary writer
         :param description: only used for the tensorboard tracker, corresponds to a short description of the value
         :param main_process_only: do not try to log in pytorch-lightning sub-processes
         """
         if not main_process_only or not os.getenv('NODE_RANK'):  # do not track in a pytorch-lightning spawned process
             value = float(value)
             if not self.types and self.basic_logger is None:
                 YAECS_LOGGER.warning("WARNING : no tracker configured, scalars will not be logged anywhere.")
@@ -436,19 +446,20 @@
                 if description is not None:
                     YAECS_LOGGER.warning("WARNING : in log_scalar : 'description' is not used in clearml.")
 
     def log_scalars(self, dictionary: Dict[str, Any], step: Optional[int] = None,
                     sub_logger: Optional[str] = None, main_process_only: bool = False) -> None:
         """
         Logs several values contained in a dictionary, one by one using Tracker.log_scalar.
+
         :param dictionary: dictionary containing the (name, value) pairs to be logged
         :param step: step at which the value is logged. If not provided, will default to 0 for the tensorboard tracker,
-        will default to -1 for the basic tracker and will be logged as a "single value" for the clearml tracker
+            will default to -1 for the basic tracker and will be logged as a "single value" for the clearml tracker
         :param sub_logger: if specified, logs to corresponding sub-logger. Can be interpreted as a sub-folder for the
-        scalar name most of the time, but in the case of tensorboard will actually use a different summary writer
+            scalar name most of the time, but in the case of tensorboard will actually use a different summary writer
         :param main_process_only: do not try to log in pytorch-lightning sub-processes
         """
         if not main_process_only or not os.getenv('NODE_RANK'):  # do not track in a pytorch-lightning spawned process
             if not self.types and self.basic_logger is None:
                 YAECS_LOGGER.warning("WARNING : no tracker configured, scalars will not be logged anywhere.")
                 if os.getenv('NODE_RANK'):
                     YAECS_LOGGER.warning("This is because trackers are deactivated in pytorch-lightning processes.\n"
@@ -458,15 +469,16 @@
 
 
 class BasicTrackerContext:
     """ Class used to set up the context for YAECS' basic tracker """
 
     def __init__(self, logger_path: str, runs: Optional[int], current: Optional[int]):
         """
-        Initialises a context used to declare the loggers required by the basic tracker.
+        Initializes a context used to declare the loggers required by the basic tracker.
+
         :param logger_path: path used by the basic tracker to log
         :param runs: number of runs in the experiment
         :param current: index of current run from 0 to runs-1
         """
         self.runs, self.current = runs, current
         self.logging_handlers = [logging.FileHandler(os.path.join(logger_path, "stdout.log")),
                                  logging.StreamHandler(sys.stdout)]
@@ -545,15 +557,16 @@
 
 
 class CMLContext:
     """ Class used to set up the context for ClearML's tracker """
 
     def __init__(self, tracker: Tracker):
         """
-        Initialises a context used to close the ClearML runs when they are done.
+        Initializes a context used to close the ClearML runs when they are done.
+
         :param tracker: tracker object where to find the ClearML runs
         """
         self.tracker = tracker
 
     def __enter__(self):
         pass
```

### Comparing `yaecs-3.2.4/yaecs/pytorch_lightning_utils.py` & `yaecs-3.2.5/yaecs/pytorch_lightning_utils.py`

 * *Files identical despite different names*

### Comparing `yaecs-3.2.4/yaecs/user_utils.py` & `yaecs-3.2.5/yaecs/user_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,26 +11,27 @@
     but WITHOUT ANY WARRANTY; without even the implied warranty of
     MERCHANTABILITY or FITNESS FOR A PARTICULAR PURPOSE.  See the
     GNU Lesser General Public License for more details.
 
     You should have received a copy of the GNU Lesser General Public License
     along with this program.  If not, see <https://www.gnu.org/licenses/>.
 """
-from typing import Callable, Dict, List, Optional, Type, Union
 import logging
+from typing import Callable, Dict, List, Optional, Type, Union
 
 from .config.config import Configuration
-from .yaecs_utils import TqdmLogger, ConfigDeclarator
+from .yaecs_utils import ConfigDeclarator, TqdmLogger
 
 YAECS_LOGGER = logging.getLogger(__name__)
 
 
 def tqdm_file():
     """
     Utility function which returns a file to which users can log their TQDM bars to make them YAECS-friendly.
+
     :return: TQDM file
     """
     return TqdmLogger(logging.getLogger("yaecs.print_catcher"))
 
 
 def get_template_class(default_config_path: Optional[ConfigDeclarator] = None,
                        pre_processing_dict: Optional[Dict[str, Callable]] = None,
@@ -38,35 +39,36 @@
                        experiment_path: str = None, tracker_config: str = None,
                        additional_configs_suffix: Optional[str] = None,
                        additional_configs_prefix: Optional[str] = None,
                        variations_suffix: Optional[str] = None, variations_prefix: Optional[str] = None,
                        grids_suffix: Optional[str] = None, grids_prefix: Optional[str] = None) -> Type[Configuration]:
     """
     Creates a template Configuration subclass to use in a small project where little customisation is needed.
+
     :param default_config_path: path to the default config to use for the template
     :param pre_processing_dict: pre-processing dict to use for the template. If this gets large, consider implementing
-    the subclass yourself as this will be clearer and more flexible.
+        the subclass yourself as this will be clearer and more flexible.
     :param post_processing_dict: post-processing dict to use for the template. If this gets large, consider implementing
-    the subclass yourself as this will be clearer and more flexible.
+        the subclass yourself as this will be clearer and more flexible.
     :param experiment_path: automatically adds relevant pre-processing rules to consider given parameter name the
-    experiment path
+        experiment path
     :param tracker_config: automatically adds relevant pre-processing rules to consider given parameter name the tracker
-    config
+        config
     :param additional_configs_suffix: automatically adds relevant pre-processing rules to consider parameter names
-    ending with 'additional_configs_suffix' as paths to additional config files
+        ending with 'additional_configs_suffix' as paths to additional config files
     :param additional_configs_prefix: automatically adds relevant pre-processing rules to consider parameter names
-    starting with 'additional_configs_prefix' as paths to additional config files
+        starting with 'additional_configs_prefix' as paths to additional config files
     :param variations_suffix: automatically adds relevant pre-processing rules to consider parameter names ending with
-    'variations_suffix' as config variations
+        'variations_suffix' as config variations
     :param variations_prefix: automatically adds relevant pre-processing rules to consider parameter names starting with
-    'variations_prefix' as config variations
+        'variations_prefix' as config variations
     :param grids_suffix: automatically adds relevant pre-processing rules to consider parameter names ending with
-    'grids_suffix' as grids
+        'grids_suffix' as grids
     :param grids_prefix: automatically adds relevant pre-processing rules to consider parameter names starting with
-    'grids_prefix' as grids
+        'grids_prefix' as grids
     :return: a template Configuration subclass
     """
 
     class Template(Configuration):
         """Template class."""
 
         @staticmethod
@@ -115,47 +117,48 @@
                 additional_configs_suffix: Optional[str] = None, additional_configs_prefix: Optional[str] = None,
                 variations_suffix: Optional[str] = None, variations_prefix: Optional[str] = None,
                 grids_suffix: Optional[str] = None, grids_prefix: Optional[str] = None,
                 **class_building_kwargs) -> Configuration:
     """
     One-liner wrapper to create a config from dicts/strings without the need for declaring a subclass. Useful for
     scripts or jupyter notebooks. Impractical/hacky for larger projects.
+
     :param configs: dicts and strings defining a config
     :param config_class: class to use to build the configuration. If not provided, use a template instead.
     :param pre_processing_dict: pre-processing dict to use for the template.
-    If this gets large, consider implementing the subclass yourself as this will be clearer and more flexible.
-    Only used if config_class is not provided.
+        If this gets large, consider implementing the subclass yourself as this will be clearer and more flexible.
+        Only used if config_class is not provided.
     :param post_processing_dict: post-processing dict to use for the template.
-    If this gets large, consider implementing the subclass yourself as this will be clearer and more flexible.
+        If this gets large, consider implementing the subclass yourself as this will be clearer and more flexible.
     :param experiment_path: automatically adds relevant pre-processing rules to consider given parameter name the
-    experiment path.
-    Only used if config_class is not provided.
+        experiment path.
+        Only used if config_class is not provided.
     :param tracker_config: automatically adds relevant pre-processing rules to consider given parameter name the tracker
-    config.
-    Only used if config_class is not provided.
+        config.
+        Only used if config_class is not provided.
     :param additional_configs_suffix: automatically adds relevant pre-processing rules to consider parameter names
-    ending with 'additional_configs_suffix' as paths to additional config files.
-    Only used if config_class is not provided.
+        ending with 'additional_configs_suffix' as paths to additional config files.
+        Only used if config_class is not provided.
     :param additional_configs_prefix: automatically adds relevant pre-processing rules to consider parameter names
-    starting with 'additional_configs_prefix' as paths to additional config files.
-    Only used if config_class is not provided.
+        starting with 'additional_configs_prefix' as paths to additional config files.
+        Only used if config_class is not provided.
     :param variations_suffix: automatically adds relevant pre-processing rules to consider parameter names ending with
-    'variations_suffix' as config variations.
-    Only used if config_class is not provided.
+        'variations_suffix' as config variations.
+        Only used if config_class is not provided.
     :param variations_prefix: automatically adds relevant pre-processing rules to consider parameter names starting with
-    'variations_prefix' as config variations.
-    Only used if config_class is not provided.
+        'variations_prefix' as config variations.
+        Only used if config_class is not provided.
     :param grids_suffix: automatically adds relevant pre-processing rules to consider parameter names ending with
-    'grids_suffix' as grids.
-    Only used if config_class is not provided.
+        'grids_suffix' as grids.
+        Only used if config_class is not provided.
     :param grids_prefix: automatically adds relevant pre-processing rules to consider parameter names starting with
-    'grids_prefix' as grids.
-    Only used if config_class is not provided.
+        'grids_prefix' as grids.
+        Only used if config_class is not provided.
     :param class_building_kwargs: same kwargs as those used in all Configuration constructors.
-    Only used if config_class is not provided.
+        Only used if config_class is not provided.
     :return: config object
     """
     class_args = {
         "pre_processing_dict": pre_processing_dict, "post_processing_dict": post_processing_dict,
         "experiment_path": experiment_path, "tracker_config": tracker_config,
         "additional_configs_suffix": additional_configs_suffix, "additional_configs_prefix": additional_configs_prefix,
         "variations_suffix": variations_suffix, "variations_prefix": variations_prefix,
```

### Comparing `yaecs-3.2.4/yaecs/yaecs_utils.py` & `yaecs-3.2.5/yaecs/yaecs_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -18,17 +18,17 @@
 import functools
 import importlib.util
 import io
 import logging
 import os
 import re
 import sys
-from enum import Enum
 from bisect import bisect
 from collections.abc import Mapping
+from enum import Enum
 from numbers import Real
 from types import ModuleType
 from typing import Any, Callable, Dict, List, Union
 
 YAECS_LOGGER = logging.getLogger(__name__)
 ConfigDeclarator = Union[str, dict]
 Hooks = Union[Dict[str, List[str]], List[str]]
@@ -37,17 +37,18 @@
 
 
 def adapt_to_type(previous_value: Any, value_to_adapt: str, force: str, param: str) -> Any:
     """
     Uses the previous value (more specifically, its type) of a parameter
     to parse a string containing its new value. Takes into account
     attempts from the user to force the new value to take a new type.
+
     :param previous_value: previous value taken by the parameter
     :param value_to_adapt: string corresponding to the new value of the
-    parameter
+        parameter
     :param force: previously-detected type-forcing tag
     :param param: name of the param for error logging
     :raises TypeError: if the new value type cannot be adapted
     :raises ValueError: the boolean value cannot be interpreted
     :return: new value for the param
     """
 
@@ -203,14 +204,15 @@
                          "- to get a True value : y, yes, true, 1\n"
                          "- to get a False value : n, no, false, 0")
 
 
 def add_to_csv(csv_path: str, name: str, value: Any, step: int) -> None:
     """
     Adds a logged value to the csv containing previously logged values
+
     :param csv_path: path to the csv containing the logged values
     :param name: name of the value to log
     :param value: value of the value to log
     :param step: step for which to log the value
     """
     if os.path.isfile(csv_path):
         with open(csv_path, encoding='utf-8') as csv_file:
@@ -240,28 +242,30 @@
             data = [str(step_to_log)] + [v[index] for v in values]
             csv_file.write(",".join(data) + "\n")
 
 
 def are_same_sub_configs(first, second) -> bool:
     """
     Checks if two sub-configs have identical nesting hierarchies.
+
     :param first: first sub-config to check
     :param second: second sub-config to check
     :return: result of the check
     """
     if first.get_name() != second.get_name():
         return False
     nh1, nh2 = first.get_nesting_hierarchy(), second.get_nesting_hierarchy()
     return len(nh1) == len(nh2) and all(nh1[i] == nh2[i] for i in range(len(nh1)))
 
 
 def assign_order(order: Union[Real, 'Priority'] = 0) -> Callable[[Callable], Callable]:
     """
     Decorator used to give an order to a processing function. If several processing functions would be called at a given
     step, they are called in increasing order.
+
     :param order: order to give the function
     :return: decorated function
     """
     def decorator_order(func: Callable) -> Callable:
         set_function_attribute(func, "order", order)
         return func
 
@@ -270,14 +274,15 @@
 
 def assign_yaml_tag(processor_tag: str, processor_type: str,
                     replacement_type_hint: str = "Any") -> Callable[[Callable], Callable]:
     """
     Decorator used to mark a function as a processor added automatically as pre or post processing function (as
     defined by processor_type) to parameters tagged with !type:<processor_tag>. Their type hint will be replaced by
     the type hint defined as replacement_type_hint.
+
     :param processor_tag: tag to use to mark a param in YAML as auto-processed by this function
     :param processor_type: 'pre' or 'post', type of processing function to add
     :param replacement_type_hint: type hint to use for any param tagged with this auto-processor
     :return: decorated function
     """
     def decorator_tag_assignment(func: Callable) -> Callable:
         func.__dict__["assigned_yaml_tag"] = (processor_tag, processor_type, replacement_type_hint)
@@ -286,14 +291,15 @@
     return decorator_tag_assignment
 
 
 def compare_string_pattern(name: str, pattern: str) -> bool:
     """
     Returns True when string 'name' matches string 'pattern',
     with the '*' character matching any number of characters.
+
     :param name: name to compare
     :param pattern: pattern to match
     :return: result of comparison
     """
     pattern = pattern.strip(" ").split("*")
     if len(pattern) == 1:
         return pattern[0] == name
@@ -307,14 +313,15 @@
     return True
 
 
 def compose(*functions: Callable) -> Callable:
     """
     Returns the composition of the functions given as argument. Functions are applied from left to right, ie :
     compose(f, g, h)(x) = h(g(f(x))).
+
     :param functions: all functions to compose, applied from left to right
     :return: the composed function
     """
     def compose_2(function_1, function_2):
         def composed(*args, **kwargs):
             return function_2(function_1(*args, **kwargs))
         orders = []
@@ -333,69 +340,74 @@
     return functools.reduce(compose_2, functions, lambda x: x)
 
 
 def dict_apply(dictionary: dict, function: Callable) -> dict:
     """
     Returns a copy of dict 'dictionary' where function 'function'
     was applied to all values.
+
     :param dictionary: dictionary to copy
     :param function: function to map
     :return: copied dictionary
     """
     return {k: function(v) for k, v in dictionary.items()}
 
 
 def escape_symbols(string_to_escape: str, symbols: Union[List[str], str]) -> str:
     """
     Take a string 'string_to_escape' as input and escapes characters
     as defined in 'symbols'.
+
     :param string_to_escape: string where the escaping operation takes
-    place
+        place
     :param symbols: list of strings to escape or string containing
-    the characters to escape
+        the characters to escape
     :return: escaped string
     """
     for symbol in symbols:
         string_to_escape = string_to_escape.replace(symbol, f"\\{symbol}")
     return string_to_escape
 
 
 def format_str(config_path_or_dictionary: ConfigDeclarator, size: int = 200) -> str:
     """
     Format helper to shorten configs to display depending on logging level.
+
     :param config_path_or_dictionary: config to display
     :param size: number of characters allowed to display
     :return: the formatted string
     """
     to_return = str(config_path_or_dictionary)
     if YAECS_LOGGER.level >= logging.INFO:
         return to_return if len(to_return) < size else f"{to_return[:size//2 - 3]} [...] {to_return[-size//2 - 3:]}"
     return to_return
 
 
 def get_order(func: Callable) -> Union[Real, 'Priority']:
     """
     If input function has an "order" attribute, returns it. Otherwise, returns Priority.INDIFFERENT.
+
     :param func: function to get the order of
     :return: the order value
     """
     return getattr(func, "order", Priority.INDIFFERENT)
 
 
 def get_param_as_parsable_string(param: Any, in_iterable: bool = False, ignore_unknown_types: bool = False) -> str:
     """
     Gets given value as a string that can be parsed by
     the Configuration.
+
     :param param:
     :param in_iterable: used only for bookkeeping in recursive calls
     :param ignore_unknown_types: how to treat types that cannot be
-    parsed by the Configuration
+        parsed by the Configuration
     :raises TypeError: if the type of 'param' cannot be enforced
     :return: string usable in the command line to reproduce the value
-    of param
+        of param
     """
     if param is None:
         return "none"
     if isinstance(param, list):
         to_ret = [get_param_as_parsable_string(i, True) for i in param]
         return f"[{','.join(to_ret)}] !list"
     if isinstance(param, dict):
@@ -424,14 +436,15 @@
     value = escape_symbols(value, ["'", '"', " "])
     return value + (f" !{type_forcing}" if type_forcing else "")
 
 
 def hook(hook_name: str) -> Callable[[Callable], Callable]:
     """
     Decorator used to keep track of registered params.
+
     :param hook_name: name of the hook to store
     :return: decorated function
     """
     def decorator_hook(func: Callable) -> Callable:
         if func.__name__.startswith("yaecs_config_hook__"):
             hooks = func.__name__.split("__")[1].split(",")
             if hook_name in hooks:
@@ -459,14 +472,15 @@
             raise RuntimeError(f"Invalid hook name {hook_name} : '{invalid_pattern}' is not allowed in hook names.")
     return decorator_hook
 
 
 def is_type_valid(value: Any, config_class: type) -> bool:
     """
     Checks whether input 'value' can be saved in a YAML file by Configuration's YAML Dumper.
+
     :param value: value to check the type of
     :param config_class: Configuration class, which must be passed as argument to avoid circular imports :(
     :return: result of the test
     """
     if isinstance(value, list):
         return all(is_type_valid(i, config_class) for i in value)
     if isinstance(value, (Mapping, config_class)):
@@ -474,14 +488,15 @@
     return isinstance(value, (int, float, str)) or value is None
 
 
 def lazy_import(name: str) -> ModuleType:
     """
     Imports a module in such a way that it is only loaded in memory when it is actually used.
     Implementation from https://docs.python.org/3/library/importlib.html#implementing-lazy-imports.
+
     :param name: name of the module to load
     :return: the loaded module
     """
     spec = importlib.util.find_spec(name)
     if not spec:
         return None
     loader = importlib.util.LazyLoader(spec.loader)
@@ -492,15 +507,16 @@
     return module
 
 
 def new_print(*args, sep: str = " ", end: str = "", file: io.TextIOWrapper = None, **keywords) -> None:
     """
     Replaces the builtin print function during an experiment run such that printed messages are also logged. Please note
     that the default file (None) logs to logging's root logger which will always go to the next line after each message.
-    Therefore, the "end" param does not replace '\n' as usual, but adds a suffix after the message and before the '\n'.
+    Therefore, the 'end' param does not replace \\n as usual, but adds a suffix after the message and before the \\n.
+
     :param args: objects to print
     :param sep: how to separate the different objects
     :param end: suffix to add after the message
     :param file: file to print to, defaults to a logging to logging's root logger with level logging.INFO
     :param keywords: might contain 'flush', in which case raise an error
     :raises TypeError: when the keyword arguments contain 'flush'
     """
@@ -515,14 +531,15 @@
             logging.getLogger("yaecs.print_catcher").info(message)
 
 
 def parse_type(string_to_process: str) -> TypeHint:
     """
     Parses an input string containing the type info for a parameter into a complex type as understood by the
     Configuration.check_type function.
+
     :param string_to_process: string to parse for type
     :return: complex type
     """
     if not string_to_process:
         raise ValueError("Invalid type hint : empty type hint.")
     string = string_to_process.lower()
     mapping_starts = {"tuple_0": "(", "tuple_1": "union[", "nonetuple": "optional[",
@@ -684,28 +701,30 @@
         return self == other
 
 
 def recursive_set_attribute(obj: Any, key: str, value: Any) -> None:
     """
     Recursively gets attributes of 'obj' until object.__setattr__
     can be used to force-set parameter 'key' to value 'value'.
+
     :param obj: object where to set the key to the value
     :param key: attribute of the object to set recursively
     :param value: value to set
     """
     if "." in key:
         subconfig, key = key.split(".", 1)
         recursive_set_attribute(obj[subconfig], key, value)
     else:
         object.__setattr__(obj, key, value)
 
 
 def set_function_attribute(func: Callable, attribute_name: str, value: Any) -> None:
     """
     Adds an attribute to a function object.
+
     :param func: function to add the attribute to
     :param attribute_name: name of the attribute to add
     :param value: value of the attribute
     """
     if attribute_name == "__name__":
         func.__name__ = value
     else:
@@ -715,14 +734,15 @@
             setattr(func, attribute_name, value)
 
 
 def update_state(state_descriptor: str) -> Callable[[Callable], Callable]:
     """
     Decorator used to store useful information in Configuration._state when using some recursive functions. Kind of a
     hack, but very useful to keep track of the loading state and also to debug.
+
     :param state_descriptor: string indicating what to store in Configuration._state
     :return: decorated function
     """
 
     def decorator_update_state(func: Callable) -> Callable:
 
         @functools.wraps(func)
```

### Comparing `yaecs-3.2.4/yaecs.egg-info/PKG-INFO` & `yaecs-3.2.5/yaecs.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yaecs
-Version: 3.2.4
+Version: 3.2.5
 Summary: A Config System designed for experimental purposes
 Author: Reactive Reality AG
 Project-URL: Source, https://gitlab.com/reactivereality/public/yaecs
 Keywords: template,machine,learning
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
```

### Comparing `yaecs-3.2.4/yaecs.egg-info/SOURCES.txt` & `yaecs-3.2.5/yaecs.egg-info/SOURCES.txt`

 * *Files 17% similar despite different names*

```diff
@@ -4,19 +4,34 @@
 COPYING.LESSER.md
 COPYING.md
 DOCUMENTATION_WIP.md
 LICENSE.md
 MANIFEST.in
 README.md
 pyproject.toml
+requirements-dev.txt
 requirements.txt
 setup.py
 short-readme.md
 .github/workflows/pipy_deployment.yaml
+docs/Makefile
+docs/conf.py
+docs/getting_started.md
+docs/index.rst
+docs/installation.md
+docs/license.md
+docs/make.bat
+docs/requirements.txt
+docs/yaecs.rst
+docs/yaecs_config.rst
 resources/yaecs_constructor_overview.png
+scipts/build_docs.sh
+scipts/tests.sh
+unittests/__init__.py
+unittests/config/__init__.py
 unittests/config/conftest.py
 unittests/config/test_config.py
 unittests/config/utils.py
 usage_example/.gitignore
 usage_example/README.md
 usage_example/main.py
 usage_example/configs/project_config.py
```

