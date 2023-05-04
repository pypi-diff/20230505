# Comparing `tmp/py-orca-1.1.0.tar.gz` & `tmp/py-orca-1.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py-orca-1.1.0.tar", last modified: Mon May  1 21:11:00 2023, max compression
+gzip compressed data, was "py-orca-1.2.0.tar", last modified: Thu May  4 22:22:36 2023, max compression
```

## Comparing `py-orca-1.1.0.tar` & `py-orca-1.2.0.tar`

### file list

```diff
@@ -1,110 +1,111 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 21:11:00.411938 py-orca-1.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)      609 2023-05-01 21:09:46.000000 py-orca-1.1.0/.coveragerc
--rw-r--r--   0 runner    (1001) docker     (123)     2912 2023-05-01 21:09:46.000000 py-orca-1.1.0/.env.example
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 21:11:00.387938 py-orca-1.1.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 21:11:00.399938 py-orca-1.1.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     5440 2023-05-01 21:09:46.000000 py-orca-1.1.0/.github/workflows/ci.yml
--rw-r--r--   0 runner    (1001) docker     (123)      622 2023-05-01 21:09:46.000000 py-orca-1.1.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-05-01 21:09:46.000000 py-orca-1.1.0/.isort.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1529 2023-05-01 21:09:46.000000 py-orca-1.1.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      490 2023-05-01 21:09:46.000000 py-orca-1.1.0/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (123)       93 2023-05-01 21:09:46.000000 py-orca-1.1.0/AUTHORS.md
--rw-r--r--   0 runner    (1001) docker     (123)     1640 2023-05-01 21:09:46.000000 py-orca-1.1.0/CHANGELOG.md
--rw-r--r--   0 runner    (1001) docker     (123)    11273 2023-05-01 21:09:46.000000 py-orca-1.1.0/CONTRIBUTING.md
--rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-01 21:09:46.000000 py-orca-1.1.0/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1860 2023-05-01 21:11:00.411938 py-orca-1.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      260 2023-05-01 21:09:46.000000 py-orca-1.1.0/Pipfile
--rw-r--r--   0 runner    (1001) docker     (123)   304810 2023-05-01 21:09:46.000000 py-orca-1.1.0/Pipfile.lock
--rw-r--r--   0 runner    (1001) docker     (123)     1055 2023-05-01 21:09:46.000000 py-orca-1.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 21:11:00.399938 py-orca-1.1.0/docs/
--rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-05-01 21:09:46.000000 py-orca-1.1.0/docs/Makefile
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 21:11:00.399938 py-orca-1.1.0/docs/_static/
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-01 21:09:46.000000 py-orca-1.1.0/docs/_static/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-05-01 21:09:46.000000 py-orca-1.1.0/docs/authors.md
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-05-01 21:09:46.000000 py-orca-1.1.0/docs/changelog.md
--rw-r--r--   0 runner    (1001) docker     (123)    10222 2023-05-01 21:09:46.000000 py-orca-1.1.0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-05-01 21:09:46.000000 py-orca-1.1.0/docs/contributing.md
--rw-r--r--   0 runner    (1001) docker     (123)      988 2023-05-01 21:09:46.000000 py-orca-1.1.0/docs/index.md
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-05-01 21:09:46.000000 py-orca-1.1.0/docs/license.md
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-05-01 21:09:46.000000 py-orca-1.1.0/docs/readme.md
--rw-r--r--   0 runner    (1001) docker     (123)      364 2023-05-01 21:09:46.000000 py-orca-1.1.0/docs/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      789 2023-05-01 21:09:46.000000 py-orca-1.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)     2555 2023-05-01 21:11:00.411938 py-orca-1.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      699 2023-05-01 21:09:46.000000 py-orca-1.1.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 21:11:00.391938 py-orca-1.1.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 21:11:00.399938 py-orca-1.1.0/src/docker/
--rw-r--r--   0 runner    (1001) docker     (123)      125 2023-05-01 21:09:46.000000 py-orca-1.1.0/src/docker/Dockerfile
--rw-r--r--   0 runner    (1001) docker     (123)      317 2023-05-01 21:09:46.000000 py-orca-1.1.0/src/docker/build.sh
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 21:11:00.399938 py-orca-1.1.0/src/orca/
--rw-r--r--   0 runner    (1001) docker     (123)      504 2023-05-01 21:09:46.000000 py-orca-1.1.0/src/orca/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 21:11:00.403938 py-orca-1.1.0/src/orca/airflow/
--rw-r--r--   0 runner    (1001) docker     (123)       90 2023-05-01 21:09:46.000000 py-orca-1.1.0/src/orca/airflow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1381 2023-05-01 21:09:46.000000 py-orca-1.1.0/src/orca/airflow/provider_info.py
--rw-r--r--   0 runner    (1001) docker     (123)      401 2023-05-01 21:09:46.000000 py-orca-1.1.0/src/orca/errors.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 21:11:00.403938 py-orca-1.1.0/src/orca/services/
--rw-r--r--   0 runner    (1001) docker     (123)     3164 2023-05-01 21:09:46.000000 py-orca-1.1.0/src/orca/services/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 21:11:00.403938 py-orca-1.1.0/src/orca/services/base/
--rw-r--r--   0 runner    (1001) docker     (123)      346 2023-05-01 21:09:46.000000 py-orca-1.1.0/src/orca/services/base/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3078 2023-05-01 21:09:46.000000 py-orca-1.1.0/src/orca/services/base/client_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     3824 2023-05-01 21:09:46.000000 py-orca-1.1.0/src/orca/services/base/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     3062 2023-05-01 21:09:46.000000 py-orca-1.1.0/src/orca/services/base/hook.py
--rw-r--r--   0 runner    (1001) docker     (123)     1226 2023-05-01 21:09:46.000000 py-orca-1.1.0/src/orca/services/base/ops.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 21:11:00.403938 py-orca-1.1.0/src/orca/services/nextflowtower/
--rw-r--r--   0 runner    (1001) docker     (123)      554 2023-05-01 21:09:46.000000 py-orca-1.1.0/src/orca/services/nextflowtower/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11280 2023-05-01 21:09:46.000000 py-orca-1.1.0/src/orca/services/nextflowtower/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     2035 2023-05-01 21:09:46.000000 py-orca-1.1.0/src/orca/services/nextflowtower/client_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     2661 2023-05-01 21:09:46.000000 py-orca-1.1.0/src/orca/services/nextflowtower/config.py
--rw-r--r--   0 runner    (1001) docker     (123)      917 2023-05-01 21:09:46.000000 py-orca-1.1.0/src/orca/services/nextflowtower/hook.py
--rw-r--r--   0 runner    (1001) docker     (123)     6325 2023-05-01 21:09:46.000000 py-orca-1.1.0/src/orca/services/nextflowtower/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     5545 2023-05-01 21:09:46.000000 py-orca-1.1.0/src/orca/services/nextflowtower/ops.py
--rw-r--r--   0 runner    (1001) docker     (123)      348 2023-05-01 21:09:46.000000 py-orca-1.1.0/src/orca/services/nextflowtower/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 21:11:00.403938 py-orca-1.1.0/src/orca/services/sevenbridges/
--rw-r--r--   0 runner    (1001) docker     (123)      455 2023-05-01 21:09:46.000000 py-orca-1.1.0/src/orca/services/sevenbridges/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2564 2023-05-01 21:09:46.000000 py-orca-1.1.0/src/orca/services/sevenbridges/client_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     2737 2023-05-01 21:09:46.000000 py-orca-1.1.0/src/orca/services/sevenbridges/config.py
--rw-r--r--   0 runner    (1001) docker     (123)      901 2023-05-01 21:09:46.000000 py-orca-1.1.0/src/orca/services/sevenbridges/hook.py
--rw-r--r--   0 runner    (1001) docker     (123)     4314 2023-05-01 21:09:46.000000 py-orca-1.1.0/src/orca/services/sevenbridges/ops.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 21:11:00.407938 py-orca-1.1.0/src/py_orca.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1860 2023-05-01 21:11:00.000000 py-orca-1.1.0/src/py_orca.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2571 2023-05-01 21:11:00.000000 py-orca-1.1.0/src/py_orca.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-01 21:11:00.000000 py-orca-1.1.0/src/py_orca.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-05-01 21:11:00.000000 py-orca-1.1.0/src/py_orca.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-01 21:11:00.000000 py-orca-1.1.0/src/py_orca.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      449 2023-05-01 21:11:00.000000 py-orca-1.1.0/src/py_orca.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-01 21:11:00.000000 py-orca-1.1.0/src/py_orca.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 21:11:00.407938 py-orca-1.1.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 21:09:46.000000 py-orca-1.1.0/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 21:11:00.407938 py-orca-1.1.0/tests/acceptance/
--rw-r--r--   0 runner    (1001) docker     (123)     1149 2023-05-01 21:09:46.000000 py-orca-1.1.0/tests/acceptance/test_cavatica.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 21:11:00.407938 py-orca-1.1.0/tests/airflow/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 21:09:46.000000 py-orca-1.1.0/tests/airflow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      868 2023-05-01 21:09:46.000000 py-orca-1.1.0/tests/airflow/test_provider_info.py
--rw-r--r--   0 runner    (1001) docker     (123)      416 2023-05-01 21:09:46.000000 py-orca-1.1.0/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 21:11:00.407938 py-orca-1.1.0/tests/services/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 21:09:46.000000 py-orca-1.1.0/tests/services/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 21:11:00.407938 py-orca-1.1.0/tests/services/base/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 21:09:46.000000 py-orca-1.1.0/tests/services/base/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2378 2023-05-01 21:09:46.000000 py-orca-1.1.0/tests/services/base/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     1553 2023-05-01 21:09:46.000000 py-orca-1.1.0/tests/services/base/test_client_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     2365 2023-05-01 21:09:46.000000 py-orca-1.1.0/tests/services/base/test_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1088 2023-05-01 21:09:46.000000 py-orca-1.1.0/tests/services/base/test_hook.py
--rw-r--r--   0 runner    (1001) docker     (123)      626 2023-05-01 21:09:46.000000 py-orca-1.1.0/tests/services/base/test_meta.py
--rw-r--r--   0 runner    (1001) docker     (123)      575 2023-05-01 21:09:46.000000 py-orca-1.1.0/tests/services/base/test_ops.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 21:11:00.411938 py-orca-1.1.0/tests/services/nextflowtower/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 21:09:46.000000 py-orca-1.1.0/tests/services/nextflowtower/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      956 2023-05-01 21:09:46.000000 py-orca-1.1.0/tests/services/nextflowtower/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     9729 2023-05-01 21:09:46.000000 py-orca-1.1.0/tests/services/nextflowtower/responses.py
--rw-r--r--   0 runner    (1001) docker     (123)     5223 2023-05-01 21:09:46.000000 py-orca-1.1.0/tests/services/nextflowtower/test_client.py
--rw-r--r--   0 runner    (1001) docker     (123)      766 2023-05-01 21:09:46.000000 py-orca-1.1.0/tests/services/nextflowtower/test_config.py
--rw-r--r--   0 runner    (1001) docker     (123)      784 2023-05-01 21:09:46.000000 py-orca-1.1.0/tests/services/nextflowtower/test_enums.py
--rw-r--r--   0 runner    (1001) docker     (123)     1209 2023-05-01 21:09:46.000000 py-orca-1.1.0/tests/services/nextflowtower/test_integration.py
--rw-r--r--   0 runner    (1001) docker     (123)     6376 2023-05-01 21:09:46.000000 py-orca-1.1.0/tests/services/nextflowtower/test_ops.py
--rw-r--r--   0 runner    (1001) docker     (123)      260 2023-05-01 21:09:46.000000 py-orca-1.1.0/tests/services/nextflowtower/test_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-01 21:11:00.411938 py-orca-1.1.0/tests/services/sevenbridges/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-01 21:09:46.000000 py-orca-1.1.0/tests/services/sevenbridges/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3404 2023-05-01 21:09:46.000000 py-orca-1.1.0/tests/services/sevenbridges/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     3088 2023-05-01 21:09:46.000000 py-orca-1.1.0/tests/services/sevenbridges/test_client_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     1235 2023-05-01 21:09:46.000000 py-orca-1.1.0/tests/services/sevenbridges/test_hook.py
--rw-r--r--   0 runner    (1001) docker     (123)     2919 2023-05-01 21:09:46.000000 py-orca-1.1.0/tests/services/sevenbridges/test_ops.py
--rw-r--r--   0 runner    (1001) docker     (123)      110 2023-05-01 21:09:46.000000 py-orca-1.1.0/tests/test_import.py
--rw-r--r--   0 runner    (1001) docker     (123)     2919 2023-05-01 21:09:46.000000 py-orca-1.1.0/tox.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 22:22:36.623104 py-orca-1.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)      609 2023-05-04 22:21:39.000000 py-orca-1.2.0/.coveragerc
+-rw-r--r--   0 runner    (1001) docker     (123)     2912 2023-05-04 22:21:39.000000 py-orca-1.2.0/.env.example
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 22:22:36.603104 py-orca-1.2.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 22:22:36.615104 py-orca-1.2.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     5440 2023-05-04 22:21:39.000000 py-orca-1.2.0/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      622 2023-05-04 22:21:39.000000 py-orca-1.2.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-05-04 22:21:39.000000 py-orca-1.2.0/.isort.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1529 2023-05-04 22:21:39.000000 py-orca-1.2.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      490 2023-05-04 22:21:39.000000 py-orca-1.2.0/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       93 2023-05-04 22:21:39.000000 py-orca-1.2.0/AUTHORS.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1640 2023-05-04 22:21:39.000000 py-orca-1.2.0/CHANGELOG.md
+-rw-r--r--   0 runner    (1001) docker     (123)    11273 2023-05-04 22:21:39.000000 py-orca-1.2.0/CONTRIBUTING.md
+-rw-r--r--   0 runner    (1001) docker     (123)    11357 2023-05-04 22:21:39.000000 py-orca-1.2.0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1860 2023-05-04 22:22:36.623104 py-orca-1.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      260 2023-05-04 22:21:39.000000 py-orca-1.2.0/Pipfile
+-rw-r--r--   0 runner    (1001) docker     (123)   304810 2023-05-04 22:21:39.000000 py-orca-1.2.0/Pipfile.lock
+-rw-r--r--   0 runner    (1001) docker     (123)     1055 2023-05-04 22:21:39.000000 py-orca-1.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 22:22:36.615104 py-orca-1.2.0/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-05-04 22:21:39.000000 py-orca-1.2.0/docs/Makefile
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 22:22:36.615104 py-orca-1.2.0/docs/_static/
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-04 22:21:39.000000 py-orca-1.2.0/docs/_static/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-05-04 22:21:39.000000 py-orca-1.2.0/docs/authors.md
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-05-04 22:21:39.000000 py-orca-1.2.0/docs/changelog.md
+-rw-r--r--   0 runner    (1001) docker     (123)    10222 2023-05-04 22:21:39.000000 py-orca-1.2.0/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-05-04 22:21:39.000000 py-orca-1.2.0/docs/contributing.md
+-rw-r--r--   0 runner    (1001) docker     (123)      988 2023-05-04 22:21:39.000000 py-orca-1.2.0/docs/index.md
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-05-04 22:21:39.000000 py-orca-1.2.0/docs/license.md
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-05-04 22:21:39.000000 py-orca-1.2.0/docs/readme.md
+-rw-r--r--   0 runner    (1001) docker     (123)      364 2023-05-04 22:21:39.000000 py-orca-1.2.0/docs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      789 2023-05-04 22:21:39.000000 py-orca-1.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)     2555 2023-05-04 22:22:36.623104 py-orca-1.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      699 2023-05-04 22:21:39.000000 py-orca-1.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 22:22:36.607104 py-orca-1.2.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 22:22:36.615104 py-orca-1.2.0/src/docker/
+-rw-r--r--   0 runner    (1001) docker     (123)      125 2023-05-04 22:21:39.000000 py-orca-1.2.0/src/docker/Dockerfile
+-rw-r--r--   0 runner    (1001) docker     (123)      317 2023-05-04 22:21:39.000000 py-orca-1.2.0/src/docker/build.sh
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 22:22:36.615104 py-orca-1.2.0/src/orca/
+-rw-r--r--   0 runner    (1001) docker     (123)      726 2023-05-04 22:21:39.000000 py-orca-1.2.0/src/orca/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 22:22:36.615104 py-orca-1.2.0/src/orca/airflow/
+-rw-r--r--   0 runner    (1001) docker     (123)       90 2023-05-04 22:21:39.000000 py-orca-1.2.0/src/orca/airflow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1381 2023-05-04 22:21:39.000000 py-orca-1.2.0/src/orca/airflow/provider_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)      401 2023-05-04 22:21:39.000000 py-orca-1.2.0/src/orca/errors.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 22:22:36.615104 py-orca-1.2.0/src/orca/services/
+-rw-r--r--   0 runner    (1001) docker     (123)     3164 2023-05-04 22:21:39.000000 py-orca-1.2.0/src/orca/services/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 22:22:36.619104 py-orca-1.2.0/src/orca/services/base/
+-rw-r--r--   0 runner    (1001) docker     (123)      346 2023-05-04 22:21:39.000000 py-orca-1.2.0/src/orca/services/base/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3078 2023-05-04 22:21:39.000000 py-orca-1.2.0/src/orca/services/base/client_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3824 2023-05-04 22:21:39.000000 py-orca-1.2.0/src/orca/services/base/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3062 2023-05-04 22:21:39.000000 py-orca-1.2.0/src/orca/services/base/hook.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1368 2023-05-04 22:21:39.000000 py-orca-1.2.0/src/orca/services/base/ops.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 22:22:36.619104 py-orca-1.2.0/src/orca/services/nextflowtower/
+-rw-r--r--   0 runner    (1001) docker     (123)      554 2023-05-04 22:21:39.000000 py-orca-1.2.0/src/orca/services/nextflowtower/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12390 2023-05-04 22:21:39.000000 py-orca-1.2.0/src/orca/services/nextflowtower/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2035 2023-05-04 22:21:39.000000 py-orca-1.2.0/src/orca/services/nextflowtower/client_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2661 2023-05-04 22:21:39.000000 py-orca-1.2.0/src/orca/services/nextflowtower/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      917 2023-05-04 22:21:39.000000 py-orca-1.2.0/src/orca/services/nextflowtower/hook.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9077 2023-05-04 22:21:39.000000 py-orca-1.2.0/src/orca/services/nextflowtower/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10184 2023-05-04 22:21:39.000000 py-orca-1.2.0/src/orca/services/nextflowtower/ops.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2235 2023-05-04 22:21:39.000000 py-orca-1.2.0/src/orca/services/nextflowtower/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 22:22:36.619104 py-orca-1.2.0/src/orca/services/sevenbridges/
+-rw-r--r--   0 runner    (1001) docker     (123)      455 2023-05-04 22:21:39.000000 py-orca-1.2.0/src/orca/services/sevenbridges/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2564 2023-05-04 22:21:39.000000 py-orca-1.2.0/src/orca/services/sevenbridges/client_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2737 2023-05-04 22:21:39.000000 py-orca-1.2.0/src/orca/services/sevenbridges/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      901 2023-05-04 22:21:39.000000 py-orca-1.2.0/src/orca/services/sevenbridges/hook.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4388 2023-05-04 22:21:39.000000 py-orca-1.2.0/src/orca/services/sevenbridges/ops.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 22:22:36.619104 py-orca-1.2.0/src/py_orca.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1860 2023-05-04 22:22:36.000000 py-orca-1.2.0/src/py_orca.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2615 2023-05-04 22:22:36.000000 py-orca-1.2.0/src/py_orca.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-04 22:22:36.000000 py-orca-1.2.0/src/py_orca.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-05-04 22:22:36.000000 py-orca-1.2.0/src/py_orca.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-04 22:22:36.000000 py-orca-1.2.0/src/py_orca.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      449 2023-05-04 22:22:36.000000 py-orca-1.2.0/src/py_orca.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-04 22:22:36.000000 py-orca-1.2.0/src/py_orca.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 22:22:36.619104 py-orca-1.2.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 22:21:39.000000 py-orca-1.2.0/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 22:22:36.619104 py-orca-1.2.0/tests/acceptance/
+-rw-r--r--   0 runner    (1001) docker     (123)     1149 2023-05-04 22:21:39.000000 py-orca-1.2.0/tests/acceptance/test_cavatica.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 22:22:36.619104 py-orca-1.2.0/tests/airflow/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 22:21:39.000000 py-orca-1.2.0/tests/airflow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      868 2023-05-04 22:21:39.000000 py-orca-1.2.0/tests/airflow/test_provider_info.py
+-rw-r--r--   0 runner    (1001) docker     (123)      416 2023-05-04 22:21:39.000000 py-orca-1.2.0/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 22:22:36.619104 py-orca-1.2.0/tests/services/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 22:21:39.000000 py-orca-1.2.0/tests/services/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 22:22:36.623104 py-orca-1.2.0/tests/services/base/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 22:21:39.000000 py-orca-1.2.0/tests/services/base/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2378 2023-05-04 22:21:39.000000 py-orca-1.2.0/tests/services/base/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1553 2023-05-04 22:21:39.000000 py-orca-1.2.0/tests/services/base/test_client_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2365 2023-05-04 22:21:39.000000 py-orca-1.2.0/tests/services/base/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1088 2023-05-04 22:21:39.000000 py-orca-1.2.0/tests/services/base/test_hook.py
+-rw-r--r--   0 runner    (1001) docker     (123)      626 2023-05-04 22:21:39.000000 py-orca-1.2.0/tests/services/base/test_meta.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-05-04 22:21:39.000000 py-orca-1.2.0/tests/services/base/test_ops.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 22:22:36.623104 py-orca-1.2.0/tests/services/nextflowtower/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 22:21:39.000000 py-orca-1.2.0/tests/services/nextflowtower/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1000 2023-05-04 22:21:39.000000 py-orca-1.2.0/tests/services/nextflowtower/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18981 2023-05-04 22:21:39.000000 py-orca-1.2.0/tests/services/nextflowtower/responses.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5558 2023-05-04 22:21:39.000000 py-orca-1.2.0/tests/services/nextflowtower/test_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      766 2023-05-04 22:21:39.000000 py-orca-1.2.0/tests/services/nextflowtower/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      844 2023-05-04 22:21:39.000000 py-orca-1.2.0/tests/services/nextflowtower/test_enums.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1259 2023-05-04 22:21:39.000000 py-orca-1.2.0/tests/services/nextflowtower/test_integration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2074 2023-05-04 22:21:39.000000 py-orca-1.2.0/tests/services/nextflowtower/test_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11259 2023-05-04 22:21:39.000000 py-orca-1.2.0/tests/services/nextflowtower/test_ops.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1738 2023-05-04 22:21:39.000000 py-orca-1.2.0/tests/services/nextflowtower/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 22:22:36.623104 py-orca-1.2.0/tests/services/sevenbridges/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 22:21:39.000000 py-orca-1.2.0/tests/services/sevenbridges/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3404 2023-05-04 22:21:39.000000 py-orca-1.2.0/tests/services/sevenbridges/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3088 2023-05-04 22:21:39.000000 py-orca-1.2.0/tests/services/sevenbridges/test_client_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1235 2023-05-04 22:21:39.000000 py-orca-1.2.0/tests/services/sevenbridges/test_hook.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2919 2023-05-04 22:21:39.000000 py-orca-1.2.0/tests/services/sevenbridges/test_ops.py
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-05-04 22:21:39.000000 py-orca-1.2.0/tests/test_import.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2919 2023-05-04 22:21:39.000000 py-orca-1.2.0/tox.ini
```

### Comparing `py-orca-1.1.0/.coveragerc` & `py-orca-1.2.0/.coveragerc`

 * *Files identical despite different names*

### Comparing `py-orca-1.1.0/.env.example` & `py-orca-1.2.0/.env.example`

 * *Files identical despite different names*

### Comparing `py-orca-1.1.0/.github/workflows/ci.yml` & `py-orca-1.2.0/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `py-orca-1.1.0/.gitignore` & `py-orca-1.2.0/.gitignore`

 * *Files identical despite different names*

### Comparing `py-orca-1.1.0/.pre-commit-config.yaml` & `py-orca-1.2.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `py-orca-1.1.0/CHANGELOG.md` & `py-orca-1.2.0/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `py-orca-1.1.0/CONTRIBUTING.md` & `py-orca-1.2.0/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `py-orca-1.1.0/LICENSE.txt` & `py-orca-1.2.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `py-orca-1.1.0/PKG-INFO` & `py-orca-1.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py-orca
-Version: 1.1.0
+Version: 1.2.0
 Summary: Python package for connecting services and building data pipelines
 Home-page: https://github.com/Sage-Bionetworks-Workflows/py-orca
 Author: Bruno Grande
 Author-email: bruno.grande@sagebase.org
 License: Apache-2.0
 Project-URL: Source, https://github.com/Sage-Bionetworks-Workflows/py-orca
 Project-URL: Tracker, https://github.com/Sage-Bionetworks-Workflows/py-orca/issues
```

### Comparing `py-orca-1.1.0/Pipfile.lock` & `py-orca-1.2.0/Pipfile.lock`

 * *Files identical despite different names*

### Comparing `py-orca-1.1.0/README.md` & `py-orca-1.2.0/README.md`

 * *Files identical despite different names*

### Comparing `py-orca-1.1.0/docs/Makefile` & `py-orca-1.2.0/docs/Makefile`

 * *Files identical despite different names*

### Comparing `py-orca-1.1.0/docs/conf.py` & `py-orca-1.2.0/docs/conf.py`

 * *Files identical despite different names*

### Comparing `py-orca-1.1.0/docs/index.md` & `py-orca-1.2.0/docs/index.md`

 * *Files identical despite different names*

### Comparing `py-orca-1.1.0/pyproject.toml` & `py-orca-1.2.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `py-orca-1.1.0/setup.cfg` & `py-orca-1.2.0/setup.cfg`

 * *Files identical despite different names*

### Comparing `py-orca-1.1.0/setup.py` & `py-orca-1.2.0/setup.py`

 * *Files identical despite different names*

### Comparing `py-orca-1.1.0/src/orca/airflow/provider_info.py` & `py-orca-1.2.0/src/orca/airflow/provider_info.py`

 * *Files identical despite different names*

### Comparing `py-orca-1.1.0/src/orca/services/__init__.py` & `py-orca-1.2.0/src/orca/services/__init__.py`

 * *Files identical despite different names*

### Comparing `py-orca-1.1.0/src/orca/services/base/client_factory.py` & `py-orca-1.2.0/src/orca/services/base/client_factory.py`

 * *Files identical despite different names*

### Comparing `py-orca-1.1.0/src/orca/services/base/config.py` & `py-orca-1.2.0/src/orca/services/base/config.py`

 * *Files identical despite different names*

### Comparing `py-orca-1.1.0/src/orca/services/base/hook.py` & `py-orca-1.2.0/src/orca/services/base/hook.py`

 * *Files identical despite different names*

### Comparing `py-orca-1.1.0/src/orca/services/base/ops.py` & `py-orca-1.2.0/src/orca/services/base/ops.py`

 * *Files 6% similar despite different names*

```diff
@@ -16,14 +16,16 @@
 
     Usage Instructions:
         1) Create a class that subclasses this base class.
         2) Decorate this class with ``@dataclass`` as this one does.
         3) Provide values to all class variables (defined below).
         4) Provide implementations for all abstract methods.
         5) Update the type hints for attributes and class variables.
+        6) Update the config attribute to have a default factory set to
+           the config class using the `dataclasses.field()` function.
 
     Attributes:
         config: A configuration object for this service.
 
     Class Variables:
         client_factory_class: The class for constructing clients.
     """
```

### Comparing `py-orca-1.1.0/src/orca/services/nextflowtower/__init__.py` & `py-orca-1.2.0/src/orca/services/nextflowtower/__init__.py`

 * *Files identical despite different names*

### Comparing `py-orca-1.1.0/src/orca/services/nextflowtower/client.py` & `py-orca-1.2.0/src/orca/services/nextflowtower/client.py`

 * *Files 3% similar despite different names*

```diff
@@ -79,15 +79,19 @@
         Raises:
             HTTPError: If something went wrong with the request.
 
         Returns:
             A dictionary from deserializing the JSON response.
         """
         response = self.request(method, path, **kwargs)
-        response.raise_for_status()
+        try:
+            response.raise_for_status()
+        except HTTPError as e:
+            # Add extra context if possible
+            raise HTTPError(response.text) from e
         return response.json()
 
     def request_paged(self, method: str, path: str, **kwargs) -> dict[str, Any]:
         """Iterate through pages of results for a given request.
 
         See ``TowerClient.request`` for argument definitions.
 
@@ -314,26 +318,54 @@
             workspace_id: Tower workspace ID.
 
         Returns:
             Workflow run ID.
         """
         path = "/workflow/launch"
         params = self.generate_params(workspace_id)
-        payload = launch_info.to_dict()
+        payload = launch_info.to_json()
         json = self.post(path, params=params, json=payload)
         return self.unwrap(json, "workflowId")
 
-    def get_workflow(self, workspace_id: int, workflow_id: str) -> dict:
-        """Gets available information about a workflow run
+    def get_workflow(
+        self,
+        workflow_id: str,
+        workspace_id: Optional[int] = None,
+    ) -> models.Workflow:
+        """Get information about a workflow run.
 
         Attributes:
-            workspace_id (int): The ID number of the workspace the workflow
-            exists within.
-            workflow_id (str): The ID number for a workflow run to get
-            information about.
+            workflow_id: The ID number for a workflow run to get
+                information about.
+            workspace_id: The ID number of the workspace the workflow
+                exists within. Defaults to None.
 
         Returns:
-            response (dict): Dictionary containing information about the workflow run
+            Workflow instance.
         """
         path = f"/workflow/{workflow_id}"
-        json = self.get(path=path, params={"workspaceId": workspace_id})
-        return json
+        params = self.generate_params(workspace_id)
+        json = self.get(path=path, params=params)
+        unwrapped = self.unwrap(json, "workflow")
+        return models.Workflow.from_json(unwrapped)
+
+    def list_workflows(
+        self,
+        search_filter: Optional[str] = None,
+        workspace_id: Optional[int] = None,
+    ) -> list[models.Workflow]:
+        """List available workflows that match search filter.
+
+        Attributes:
+            search_filter: A Nextflow Tower search query, as you would
+                compose it in the runs search bar. Defaults to None.
+            workspace_id: The ID number of the workspace the workflow
+                exists within. Defaults to None.
+
+        Returns:
+            List of workflow instances.
+        """
+        path = "/workflow"
+        params = self.generate_params(workspace_id, search=search_filter)
+        json = self.get(path=path, params=params)
+        items = self.unwrap(json, "workflows")
+        return [models.Workflow.from_json(item["workflow"]) for item in items]
```

### Comparing `py-orca-1.1.0/src/orca/services/nextflowtower/client_factory.py` & `py-orca-1.2.0/src/orca/services/nextflowtower/client_factory.py`

 * *Files identical despite different names*

### Comparing `py-orca-1.1.0/src/orca/services/nextflowtower/config.py` & `py-orca-1.2.0/src/orca/services/nextflowtower/config.py`

 * *Files identical despite different names*

### Comparing `py-orca-1.1.0/src/orca/services/nextflowtower/hook.py` & `py-orca-1.2.0/src/orca/services/nextflowtower/hook.py`

 * *Files identical despite different names*

### Comparing `py-orca-1.1.0/src/orca/services/sevenbridges/client_factory.py` & `py-orca-1.2.0/src/orca/services/sevenbridges/client_factory.py`

 * *Files identical despite different names*

### Comparing `py-orca-1.1.0/src/orca/services/sevenbridges/config.py` & `py-orca-1.2.0/src/orca/services/sevenbridges/config.py`

 * *Files identical despite different names*

### Comparing `py-orca-1.1.0/src/orca/services/sevenbridges/hook.py` & `py-orca-1.2.0/src/orca/services/sevenbridges/hook.py`

 * *Files identical despite different names*

### Comparing `py-orca-1.1.0/src/orca/services/sevenbridges/ops.py` & `py-orca-1.2.0/src/orca/services/sevenbridges/ops.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from __future__ import annotations
 
+from dataclasses import field
 from functools import cached_property
 from typing import Any, Optional, cast
 
 from pydantic.dataclasses import dataclass
 from sevenbridges.models.enums import TaskStatus
 
 from orca.errors import ConfigError, UnexpectedMatchError
@@ -19,15 +20,15 @@
     Attributes:
         config: A configuration object for this service.
 
     Class Variables:
         client_factory_class: The class for constructing clients.
     """
 
-    config: SevenBridgesConfig
+    config: SevenBridgesConfig = field(default_factory=SevenBridgesConfig)
 
     client_factory_class = SevenBridgesClientFactory
 
     @cached_property
     def project(self) -> str:
         """The currently active SevenBridges project."""
         if self.config.project is None:
```

### Comparing `py-orca-1.1.0/src/py_orca.egg-info/PKG-INFO` & `py-orca-1.2.0/src/py_orca.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py-orca
-Version: 1.1.0
+Version: 1.2.0
 Summary: Python package for connecting services and building data pipelines
 Home-page: https://github.com/Sage-Bionetworks-Workflows/py-orca
 Author: Bruno Grande
 Author-email: bruno.grande@sagebase.org
 License: Apache-2.0
 Project-URL: Source, https://github.com/Sage-Bionetworks-Workflows/py-orca
 Project-URL: Tracker, https://github.com/Sage-Bionetworks-Workflows/py-orca/issues
```

### Comparing `py-orca-1.1.0/src/py_orca.egg-info/SOURCES.txt` & `py-orca-1.2.0/src/py_orca.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -75,14 +75,15 @@
 tests/services/nextflowtower/__init__.py
 tests/services/nextflowtower/conftest.py
 tests/services/nextflowtower/responses.py
 tests/services/nextflowtower/test_client.py
 tests/services/nextflowtower/test_config.py
 tests/services/nextflowtower/test_enums.py
 tests/services/nextflowtower/test_integration.py
+tests/services/nextflowtower/test_models.py
 tests/services/nextflowtower/test_ops.py
 tests/services/nextflowtower/test_utils.py
 tests/services/sevenbridges/__init__.py
 tests/services/sevenbridges/conftest.py
 tests/services/sevenbridges/test_client_factory.py
 tests/services/sevenbridges/test_hook.py
 tests/services/sevenbridges/test_ops.py
```

### Comparing `py-orca-1.1.0/tests/acceptance/test_cavatica.py` & `py-orca-1.2.0/tests/acceptance/test_cavatica.py`

 * *Files identical despite different names*

### Comparing `py-orca-1.1.0/tests/airflow/test_provider_info.py` & `py-orca-1.2.0/tests/airflow/test_provider_info.py`

 * *Files identical despite different names*

### Comparing `py-orca-1.1.0/tests/services/base/conftest.py` & `py-orca-1.2.0/tests/services/base/conftest.py`

 * *Files identical despite different names*

### Comparing `py-orca-1.1.0/tests/services/base/test_client_factory.py` & `py-orca-1.2.0/tests/services/base/test_client_factory.py`

 * *Files identical despite different names*

### Comparing `py-orca-1.1.0/tests/services/base/test_config.py` & `py-orca-1.2.0/tests/services/base/test_config.py`

 * *Files identical despite different names*

### Comparing `py-orca-1.1.0/tests/services/base/test_hook.py` & `py-orca-1.2.0/tests/services/base/test_hook.py`

 * *Files identical despite different names*

### Comparing `py-orca-1.1.0/tests/services/base/test_meta.py` & `py-orca-1.2.0/tests/services/base/test_meta.py`

 * *Files identical despite different names*

### Comparing `py-orca-1.1.0/tests/services/nextflowtower/conftest.py` & `py-orca-1.2.0/tests/services/nextflowtower/conftest.py`

 * *Files 6% similar despite different names*

```diff
@@ -23,14 +23,15 @@
 
 
 @pytest.fixture
 def ops(config):
     yield NextflowTowerOps(config)
 
 
+# TODO: Mock `client` using a property mock
 @pytest.fixture
 def mocked_ops(config, client, mocker):
     mocker.patch.object(NextflowTowerOps, "client", return_value=client)
     mocker.patch.object(NextflowTowerOps, "workspace_id", return_value=98765)
     yield NextflowTowerOps(config)
```

### Comparing `py-orca-1.1.0/tests/services/nextflowtower/test_client.py` & `py-orca-1.2.0/tests/services/nextflowtower/test_client.py`

 * *Files 2% similar despite different names*

```diff
@@ -37,15 +37,15 @@
     mock = mocker.patch.object(client, "request_json")
     mock.return_value = expected
     actual = client.get_user_info()
     mock.assert_called_once()
     assert actual == models.User.from_json(expected["user"])
 
 
-def test_that_get_user_info_fails_with_nonstandard_response(client, mocker):
+def test_that_get_user_info_fails_with_400_response(client, mocker):
     mock = mocker.patch.object(client, "request_json")
     mock.return_value = {"message": "foobar"}
     with pytest.raises(HTTPError):
         client.get_user_info()
 
 
 def test_that_list_user_workspaces_works(client, mocker, get_response):
@@ -121,21 +121,30 @@
 
 def test_that_launch_workflow_works(client, mocker, get_response):
     mock = mocker.patch.object(client, "request_json")
     mock.return_value = get_response("launch_workflow")
     launch_spec = models.LaunchInfo(
         compute_env_id="foo",
         pipeline="bar",
+        run_name="foobar",
         work_dir="s3://path",
         profiles=["test"],
     )
     client.launch_workflow(launch_spec)
     mock.assert_called_once()
 
 
 def test_that_get_workflow_returns_expected_response(client, mocker, get_response):
-    expected = get_response("get_workflow")
-    mock = mocker.patch.object(client, "get")
-    mock.return_value = expected
+    response = get_response("get_workflow")
+    mock = mocker.patch.object(client, "request_json")
+    mock.return_value = response
     actual = client.get_workflow(workspace_id=98765, workflow_id="123456789")
     mock.assert_called_once()
-    assert actual == expected
+    assert actual == models.Workflow.from_json(response["workflow"])
+
+
+def test_that_list_workflows_works(client, mocker, get_response):
+    mock = mocker.patch.object(client, "request_json")
+    mock.return_value = get_response("list_workflows")
+    result = client.list_workflows()
+    mock.assert_called()
+    assert len(result) == 3
```

### Comparing `py-orca-1.1.0/tests/services/nextflowtower/test_config.py` & `py-orca-1.2.0/tests/services/nextflowtower/test_config.py`

 * *Files identical despite different names*

### Comparing `py-orca-1.1.0/tests/services/sevenbridges/conftest.py` & `py-orca-1.2.0/tests/services/sevenbridges/conftest.py`

 * *Files identical despite different names*

### Comparing `py-orca-1.1.0/tests/services/sevenbridges/test_client_factory.py` & `py-orca-1.2.0/tests/services/sevenbridges/test_client_factory.py`

 * *Files identical despite different names*

### Comparing `py-orca-1.1.0/tests/services/sevenbridges/test_hook.py` & `py-orca-1.2.0/tests/services/sevenbridges/test_hook.py`

 * *Files identical despite different names*

### Comparing `py-orca-1.1.0/tests/services/sevenbridges/test_ops.py` & `py-orca-1.2.0/tests/services/sevenbridges/test_ops.py`

 * *Files identical despite different names*

### Comparing `py-orca-1.1.0/tox.ini` & `py-orca-1.2.0/tox.ini`

 * *Files identical despite different names*

