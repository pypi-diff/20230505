# Comparing `tmp/invenio-indexer-2.1.1.tar.gz` & `tmp/invenio-indexer-2.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "invenio-indexer-2.1.1.tar", last modified: Fri Oct  7 12:17:24 2022, max compression
+gzip compressed data, was "invenio-indexer-2.1.2.tar", last modified: Fri May  5 12:53:07 2023, max compression
```

## Comparing `invenio-indexer-2.1.1.tar` & `invenio-indexer-2.1.2.tar`

### file list

```diff
@@ -1,90 +1,90 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-07 12:17:24.168861 invenio-indexer-2.1.1/
--rw-r--r--   0 runner    (1001) docker     (121)      124 2022-10-07 12:17:20.000000 invenio-indexer-2.1.1/.dockerignore
--rw-r--r--   0 runner    (1001) docker     (121)      666 2022-10-07 12:17:20.000000 invenio-indexer-2.1.1/.editorconfig
--rw-r--r--   0 runner    (1001) docker     (121)       41 2022-10-07 12:17:20.000000 invenio-indexer-2.1.1/.git-blame-ignore-revs
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-07 12:17:24.160861 invenio-indexer-2.1.1/.github/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-07 12:17:24.164861 invenio-indexer-2.1.1/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (121)      667 2022-10-07 12:17:20.000000 invenio-indexer-2.1.1/.github/workflows/pypi-publish.yml
--rw-r--r--   0 runner    (1001) docker     (121)     2320 2022-10-07 12:17:20.000000 invenio-indexer-2.1.1/.github/workflows/tests.yml
--rw-r--r--   0 runner    (1001) docker     (121)      539 2022-10-07 12:17:20.000000 invenio-indexer-2.1.1/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (121)     3023 2022-10-07 12:17:20.000000 invenio-indexer-2.1.1/CHANGES.rst
--rw-r--r--   0 runner    (1001) docker     (121)     3735 2022-10-07 12:17:20.000000 invenio-indexer-2.1.1/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (121)      731 2022-10-07 12:17:20.000000 invenio-indexer-2.1.1/INSTALL.rst
--rw-r--r--   0 runner    (1001) docker     (121)     1067 2022-10-07 12:17:20.000000 invenio-indexer-2.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)      693 2022-10-07 12:17:20.000000 invenio-indexer-2.1.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     5607 2022-10-07 12:17:24.168861 invenio-indexer-2.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1007 2022-10-07 12:17:20.000000 invenio-indexer-2.1.1/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-07 12:17:24.164861 invenio-indexer-2.1.1/docs/
--rw-r--r--   0 runner    (1001) docker     (121)     7445 2022-10-07 12:17:20.000000 invenio-indexer-2.1.1/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (121)      554 2022-10-07 12:17:20.000000 invenio-indexer-2.1.1/docs/api.rst
--rw-r--r--   0 runner    (1001) docker     (121)      247 2022-10-07 12:17:20.000000 invenio-indexer-2.1.1/docs/authors.rst
--rw-r--r--   0 runner    (1001) docker     (121)      247 2022-10-07 12:17:20.000000 invenio-indexer-2.1.1/docs/changes.rst
--rw-r--r--   0 runner    (1001) docker     (121)    10286 2022-10-07 12:17:20.000000 invenio-indexer-2.1.1/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (121)      300 2022-10-07 12:17:20.000000 invenio-indexer-2.1.1/docs/configuration.rst
--rw-r--r--   0 runner    (1001) docker     (121)      252 2022-10-07 12:17:20.000000 invenio-indexer-2.1.1/docs/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (121)      828 2022-10-07 12:17:20.000000 invenio-indexer-2.1.1/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (121)      247 2022-10-07 12:17:20.000000 invenio-indexer-2.1.1/docs/installation.rst
--rw-r--r--   0 runner    (1001) docker     (121)      253 2022-10-07 12:17:20.000000 invenio-indexer-2.1.1/docs/license.rst
--rw-r--r--   0 runner    (1001) docker     (121)     6999 2022-10-07 12:17:20.000000 invenio-indexer-2.1.1/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (121)       29 2022-10-07 12:17:20.000000 invenio-indexer-2.1.1/docs/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)      264 2022-10-07 12:17:20.000000 invenio-indexer-2.1.1/docs/usage.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-07 12:17:24.168861 invenio-indexer-2.1.1/invenio_indexer/
--rw-r--r--   0 runner    (1001) docker     (121)     6480 2022-10-07 12:17:20.000000 invenio-indexer-2.1.1/invenio_indexer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    16803 2022-10-07 12:17:20.000000 invenio-indexer-2.1.1/invenio_indexer/api.py
--rw-r--r--   0 runner    (1001) docker     (121)     4293 2022-10-07 12:17:20.000000 invenio-indexer-2.1.1/invenio_indexer/cli.py
--rw-r--r--   0 runner    (1001) docker     (121)     1343 2022-10-07 12:17:20.000000 invenio-indexer-2.1.1/invenio_indexer/config.py
--rw-r--r--   0 runner    (1001) docker     (121)     1725 2022-10-07 12:17:20.000000 invenio-indexer-2.1.1/invenio_indexer/ext.py
--rw-r--r--   0 runner    (1001) docker     (121)      703 2022-10-07 12:17:20.000000 invenio-indexer-2.1.1/invenio_indexer/proxies.py
--rw-r--r--   0 runner    (1001) docker     (121)     1250 2022-10-07 12:17:20.000000 invenio-indexer-2.1.1/invenio_indexer/registry.py
--rw-r--r--   0 runner    (1001) docker     (121)     2744 2022-10-07 12:17:20.000000 invenio-indexer-2.1.1/invenio_indexer/signals.py
--rw-r--r--   0 runner    (1001) docker     (121)     1872 2022-10-07 12:17:20.000000 invenio-indexer-2.1.1/invenio_indexer/tasks.py
--rw-r--r--   0 runner    (1001) docker     (121)     1611 2022-10-07 12:17:20.000000 invenio-indexer-2.1.1/invenio_indexer/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-07 12:17:24.168861 invenio-indexer-2.1.1/invenio_indexer.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     5607 2022-10-07 12:17:24.000000 invenio-indexer-2.1.1/invenio_indexer.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1800 2022-10-07 12:17:24.000000 invenio-indexer-2.1.1/invenio_indexer.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-10-07 12:17:24.000000 invenio-indexer-2.1.1/invenio_indexer.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)      208 2022-10-07 12:17:24.000000 invenio-indexer-2.1.1/invenio_indexer.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-10-07 12:17:24.000000 invenio-indexer-2.1.1/invenio_indexer.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)      411 2022-10-07 12:17:24.000000 invenio-indexer-2.1.1/invenio_indexer.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       16 2022-10-07 12:17:24.000000 invenio-indexer-2.1.1/invenio_indexer.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)      104 2022-10-07 12:17:20.000000 invenio-indexer-2.1.1/pyproject.toml
--rwxr-xr-x   0 runner    (1001) docker     (121)      756 2022-10-07 12:17:20.000000 invenio-indexer-2.1.1/run-tests.sh
--rw-r--r--   0 runner    (1001) docker     (121)     2176 2022-10-07 12:17:24.172861 invenio-indexer-2.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)      360 2022-10-07 12:17:20.000000 invenio-indexer-2.1.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-07 12:17:24.168861 invenio-indexer-2.1.1/tests/
--rw-r--r--   0 runner    (1001) docker     (121)     3049 2022-10-07 12:17:20.000000 invenio-indexer-2.1.1/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-07 12:17:24.168861 invenio-indexer-2.1.1/tests/data/
--rw-r--r--   0 runner    (1001) docker     (121)      258 2022-10-07 12:17:20.000000 invenio-indexer-2.1.1/tests/data/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-07 12:17:24.168861 invenio-indexer-2.1.1/tests/data/os-v1/
--rw-r--r--   0 runner    (1001) docker     (121)      260 2022-10-07 12:17:20.000000 invenio-indexer-2.1.1/tests/data/os-v1/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-07 12:17:24.168861 invenio-indexer-2.1.1/tests/data/os-v1/records/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-07 12:17:24.168861 invenio-indexer-2.1.1/tests/data/os-v1/records/authorities/
--rw-r--r--   0 runner    (1001) docker     (121)       17 2022-10-07 12:17:20.000000 invenio-indexer-2.1.1/tests/data/os-v1/records/authorities/authority-v1.0.0.json
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-07 12:17:24.168861 invenio-indexer-2.1.1/tests/data/os-v1/records/bibliographic/
--rw-r--r--   0 runner    (1001) docker     (121)       17 2022-10-07 12:17:20.000000 invenio-indexer-2.1.1/tests/data/os-v1/records/bibliographic/bibliographic-v1.0.0.json
--rw-r--r--   0 runner    (1001) docker     (121)       17 2022-10-07 12:17:20.000000 invenio-indexer-2.1.1/tests/data/os-v1/records/default-v1.0.0.json
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-07 12:17:24.168861 invenio-indexer-2.1.1/tests/data/os-v2/
--rw-r--r--   0 runner    (1001) docker     (121)      260 2022-10-07 12:17:20.000000 invenio-indexer-2.1.1/tests/data/os-v2/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-07 12:17:24.168861 invenio-indexer-2.1.1/tests/data/os-v2/records/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-07 12:17:24.168861 invenio-indexer-2.1.1/tests/data/os-v2/records/authorities/
--rw-r--r--   0 runner    (1001) docker     (121)       17 2022-10-07 12:17:20.000000 invenio-indexer-2.1.1/tests/data/os-v2/records/authorities/authority-v1.0.0.json
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-07 12:17:24.168861 invenio-indexer-2.1.1/tests/data/os-v2/records/bibliographic/
--rw-r--r--   0 runner    (1001) docker     (121)       17 2022-10-07 12:17:20.000000 invenio-indexer-2.1.1/tests/data/os-v2/records/bibliographic/bibliographic-v1.0.0.json
--rw-r--r--   0 runner    (1001) docker     (121)       17 2022-10-07 12:17:20.000000 invenio-indexer-2.1.1/tests/data/os-v2/records/default-v1.0.0.json
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-07 12:17:24.168861 invenio-indexer-2.1.1/tests/data/v7/
--rw-r--r--   0 runner    (1001) docker     (121)      268 2022-10-07 12:17:20.000000 invenio-indexer-2.1.1/tests/data/v7/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-07 12:17:24.168861 invenio-indexer-2.1.1/tests/data/v7/records/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-07 12:17:24.168861 invenio-indexer-2.1.1/tests/data/v7/records/authorities/
--rw-r--r--   0 runner    (1001) docker     (121)       17 2022-10-07 12:17:20.000000 invenio-indexer-2.1.1/tests/data/v7/records/authorities/authority-v1.0.0.json
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-07 12:17:24.168861 invenio-indexer-2.1.1/tests/data/v7/records/bibliographic/
--rw-r--r--   0 runner    (1001) docker     (121)       17 2022-10-07 12:17:20.000000 invenio-indexer-2.1.1/tests/data/v7/records/bibliographic/bibliographic-v1.0.0.json
--rw-r--r--   0 runner    (1001) docker     (121)       17 2022-10-07 12:17:20.000000 invenio-indexer-2.1.1/tests/data/v7/records/default-v1.0.0.json
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-07 12:17:24.168861 invenio-indexer-2.1.1/tests/demo/
--rw-r--r--   0 runner    (1001) docker     (121)      255 2022-10-07 12:17:20.000000 invenio-indexer-2.1.1/tests/demo/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      422 2022-10-07 12:17:20.000000 invenio-indexer-2.1.1/tests/demo/json_resolver.py
--rw-r--r--   0 runner    (1001) docker     (121)    14030 2022-10-07 12:17:20.000000 invenio-indexer-2.1.1/tests/test_api.py
--rw-r--r--   0 runner    (1001) docker     (121)     3284 2022-10-07 12:17:20.000000 invenio-indexer-2.1.1/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (121)     6002 2022-10-07 12:17:20.000000 invenio-indexer-2.1.1/tests/test_invenio_indexer.py
--rw-r--r--   0 runner    (1001) docker     (121)     1188 2022-10-07 12:17:20.000000 invenio-indexer-2.1.1/tests/test_registry.py
--rw-r--r--   0 runner    (1001) docker     (121)     1072 2022-10-07 12:17:20.000000 invenio-indexer-2.1.1/tests/test_tasks.py
--rw-r--r--   0 runner    (1001) docker     (121)     1372 2022-10-07 12:17:20.000000 invenio-indexer-2.1.1/tests/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-05 12:53:07.302495 invenio-indexer-2.1.2/
+-rw-r--r--   0 runner    (1001) docker     (122)      124 2023-05-05 12:52:58.000000 invenio-indexer-2.1.2/.dockerignore
+-rw-r--r--   0 runner    (1001) docker     (122)      666 2023-05-05 12:52:58.000000 invenio-indexer-2.1.2/.editorconfig
+-rw-r--r--   0 runner    (1001) docker     (122)       41 2023-05-05 12:52:58.000000 invenio-indexer-2.1.2/.git-blame-ignore-revs
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-05 12:53:07.290495 invenio-indexer-2.1.2/.github/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-05 12:53:07.294495 invenio-indexer-2.1.2/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (122)      667 2023-05-05 12:52:58.000000 invenio-indexer-2.1.2/.github/workflows/pypi-publish.yml
+-rw-r--r--   0 runner    (1001) docker     (122)     2347 2023-05-05 12:52:58.000000 invenio-indexer-2.1.2/.github/workflows/tests.yml
+-rw-r--r--   0 runner    (1001) docker     (122)      539 2023-05-05 12:52:58.000000 invenio-indexer-2.1.2/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     3204 2023-05-05 12:52:58.000000 invenio-indexer-2.1.2/CHANGES.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     3735 2023-05-05 12:52:58.000000 invenio-indexer-2.1.2/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      731 2023-05-05 12:52:58.000000 invenio-indexer-2.1.2/INSTALL.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     1067 2023-05-05 12:52:58.000000 invenio-indexer-2.1.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)      693 2023-05-05 12:52:58.000000 invenio-indexer-2.1.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)     5828 2023-05-05 12:53:07.302495 invenio-indexer-2.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     1007 2023-05-05 12:52:58.000000 invenio-indexer-2.1.2/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-05 12:53:07.294495 invenio-indexer-2.1.2/docs/
+-rw-r--r--   0 runner    (1001) docker     (122)     7445 2023-05-05 12:52:58.000000 invenio-indexer-2.1.2/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (122)      554 2023-05-05 12:52:58.000000 invenio-indexer-2.1.2/docs/api.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      247 2023-05-05 12:52:58.000000 invenio-indexer-2.1.2/docs/authors.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      247 2023-05-05 12:52:58.000000 invenio-indexer-2.1.2/docs/changes.rst
+-rw-r--r--   0 runner    (1001) docker     (122)    10286 2023-05-05 12:52:58.000000 invenio-indexer-2.1.2/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (122)      300 2023-05-05 12:52:58.000000 invenio-indexer-2.1.2/docs/configuration.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      252 2023-05-05 12:52:58.000000 invenio-indexer-2.1.2/docs/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      828 2023-05-05 12:52:58.000000 invenio-indexer-2.1.2/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      247 2023-05-05 12:52:58.000000 invenio-indexer-2.1.2/docs/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      253 2023-05-05 12:52:58.000000 invenio-indexer-2.1.2/docs/license.rst
+-rw-r--r--   0 runner    (1001) docker     (122)     6999 2023-05-05 12:52:58.000000 invenio-indexer-2.1.2/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (122)       29 2023-05-05 12:52:58.000000 invenio-indexer-2.1.2/docs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      264 2023-05-05 12:52:58.000000 invenio-indexer-2.1.2/docs/usage.rst
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-05 12:53:07.298495 invenio-indexer-2.1.2/invenio_indexer/
+-rw-r--r--   0 runner    (1001) docker     (122)     6480 2023-05-05 12:52:58.000000 invenio-indexer-2.1.2/invenio_indexer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    17246 2023-05-05 12:52:58.000000 invenio-indexer-2.1.2/invenio_indexer/api.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4293 2023-05-05 12:52:58.000000 invenio-indexer-2.1.2/invenio_indexer/cli.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1918 2023-05-05 12:52:58.000000 invenio-indexer-2.1.2/invenio_indexer/config.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1725 2023-05-05 12:52:58.000000 invenio-indexer-2.1.2/invenio_indexer/ext.py
+-rw-r--r--   0 runner    (1001) docker     (122)      703 2023-05-05 12:52:58.000000 invenio-indexer-2.1.2/invenio_indexer/proxies.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1250 2023-05-05 12:52:58.000000 invenio-indexer-2.1.2/invenio_indexer/registry.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2744 2023-05-05 12:52:58.000000 invenio-indexer-2.1.2/invenio_indexer/signals.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1872 2023-05-05 12:52:58.000000 invenio-indexer-2.1.2/invenio_indexer/tasks.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1611 2023-05-05 12:52:58.000000 invenio-indexer-2.1.2/invenio_indexer/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-05 12:53:07.298495 invenio-indexer-2.1.2/invenio_indexer.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     5828 2023-05-05 12:53:06.000000 invenio-indexer-2.1.2/invenio_indexer.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     1800 2023-05-05 12:53:07.000000 invenio-indexer-2.1.2/invenio_indexer.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-05 12:53:06.000000 invenio-indexer-2.1.2/invenio_indexer.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      208 2023-05-05 12:53:06.000000 invenio-indexer-2.1.2/invenio_indexer.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-05 12:53:06.000000 invenio-indexer-2.1.2/invenio_indexer.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (122)      411 2023-05-05 12:53:06.000000 invenio-indexer-2.1.2/invenio_indexer.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       16 2023-05-05 12:53:06.000000 invenio-indexer-2.1.2/invenio_indexer.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      104 2023-05-05 12:52:58.000000 invenio-indexer-2.1.2/pyproject.toml
+-rwxr-xr-x   0 runner    (1001) docker     (122)      756 2023-05-05 12:52:58.000000 invenio-indexer-2.1.2/run-tests.sh
+-rw-r--r--   0 runner    (1001) docker     (122)     2176 2023-05-05 12:53:07.302495 invenio-indexer-2.1.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)      360 2023-05-05 12:52:58.000000 invenio-indexer-2.1.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-05 12:53:07.298495 invenio-indexer-2.1.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)     3049 2023-05-05 12:52:58.000000 invenio-indexer-2.1.2/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-05 12:53:07.298495 invenio-indexer-2.1.2/tests/data/
+-rw-r--r--   0 runner    (1001) docker     (122)      258 2023-05-05 12:52:58.000000 invenio-indexer-2.1.2/tests/data/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-05 12:53:07.298495 invenio-indexer-2.1.2/tests/data/os-v1/
+-rw-r--r--   0 runner    (1001) docker     (122)      260 2023-05-05 12:52:58.000000 invenio-indexer-2.1.2/tests/data/os-v1/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-05 12:53:07.298495 invenio-indexer-2.1.2/tests/data/os-v1/records/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-05 12:53:07.298495 invenio-indexer-2.1.2/tests/data/os-v1/records/authorities/
+-rw-r--r--   0 runner    (1001) docker     (122)       17 2023-05-05 12:52:58.000000 invenio-indexer-2.1.2/tests/data/os-v1/records/authorities/authority-v1.0.0.json
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-05 12:53:07.298495 invenio-indexer-2.1.2/tests/data/os-v1/records/bibliographic/
+-rw-r--r--   0 runner    (1001) docker     (122)       17 2023-05-05 12:52:58.000000 invenio-indexer-2.1.2/tests/data/os-v1/records/bibliographic/bibliographic-v1.0.0.json
+-rw-r--r--   0 runner    (1001) docker     (122)       17 2023-05-05 12:52:58.000000 invenio-indexer-2.1.2/tests/data/os-v1/records/default-v1.0.0.json
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-05 12:53:07.298495 invenio-indexer-2.1.2/tests/data/os-v2/
+-rw-r--r--   0 runner    (1001) docker     (122)      260 2023-05-05 12:52:58.000000 invenio-indexer-2.1.2/tests/data/os-v2/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-05 12:53:07.298495 invenio-indexer-2.1.2/tests/data/os-v2/records/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-05 12:53:07.298495 invenio-indexer-2.1.2/tests/data/os-v2/records/authorities/
+-rw-r--r--   0 runner    (1001) docker     (122)       17 2023-05-05 12:52:58.000000 invenio-indexer-2.1.2/tests/data/os-v2/records/authorities/authority-v1.0.0.json
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-05 12:53:07.302495 invenio-indexer-2.1.2/tests/data/os-v2/records/bibliographic/
+-rw-r--r--   0 runner    (1001) docker     (122)       17 2023-05-05 12:52:58.000000 invenio-indexer-2.1.2/tests/data/os-v2/records/bibliographic/bibliographic-v1.0.0.json
+-rw-r--r--   0 runner    (1001) docker     (122)       17 2023-05-05 12:52:58.000000 invenio-indexer-2.1.2/tests/data/os-v2/records/default-v1.0.0.json
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-05 12:53:07.302495 invenio-indexer-2.1.2/tests/data/v7/
+-rw-r--r--   0 runner    (1001) docker     (122)      268 2023-05-05 12:52:58.000000 invenio-indexer-2.1.2/tests/data/v7/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-05 12:53:07.302495 invenio-indexer-2.1.2/tests/data/v7/records/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-05 12:53:07.302495 invenio-indexer-2.1.2/tests/data/v7/records/authorities/
+-rw-r--r--   0 runner    (1001) docker     (122)       17 2023-05-05 12:52:58.000000 invenio-indexer-2.1.2/tests/data/v7/records/authorities/authority-v1.0.0.json
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-05 12:53:07.302495 invenio-indexer-2.1.2/tests/data/v7/records/bibliographic/
+-rw-r--r--   0 runner    (1001) docker     (122)       17 2023-05-05 12:52:58.000000 invenio-indexer-2.1.2/tests/data/v7/records/bibliographic/bibliographic-v1.0.0.json
+-rw-r--r--   0 runner    (1001) docker     (122)       17 2023-05-05 12:52:58.000000 invenio-indexer-2.1.2/tests/data/v7/records/default-v1.0.0.json
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-05 12:53:07.302495 invenio-indexer-2.1.2/tests/demo/
+-rw-r--r--   0 runner    (1001) docker     (122)      255 2023-05-05 12:52:58.000000 invenio-indexer-2.1.2/tests/demo/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      422 2023-05-05 12:52:58.000000 invenio-indexer-2.1.2/tests/demo/json_resolver.py
+-rw-r--r--   0 runner    (1001) docker     (122)    14030 2023-05-05 12:52:58.000000 invenio-indexer-2.1.2/tests/test_api.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3284 2023-05-05 12:52:58.000000 invenio-indexer-2.1.2/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6002 2023-05-05 12:52:58.000000 invenio-indexer-2.1.2/tests/test_invenio_indexer.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1188 2023-05-05 12:52:58.000000 invenio-indexer-2.1.2/tests/test_registry.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1072 2023-05-05 12:52:58.000000 invenio-indexer-2.1.2/tests/test_tasks.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1372 2023-05-05 12:52:58.000000 invenio-indexer-2.1.2/tests/test_utils.py
```

### Comparing `invenio-indexer-2.1.1/.editorconfig` & `invenio-indexer-2.1.2/.editorconfig`

 * *Files identical despite different names*

### Comparing `invenio-indexer-2.1.1/.github/workflows/pypi-publish.yml` & `invenio-indexer-2.1.2/.github/workflows/pypi-publish.yml`

 * *Files identical despite different names*

### Comparing `invenio-indexer-2.1.1/.github/workflows/tests.yml` & `invenio-indexer-2.1.2/.github/workflows/tests.yml`

 * *Files 8% similar despite different names*

```diff
@@ -9,15 +9,17 @@
 
 name: CI
 
 on:
   push:
     branches: master
   pull_request:
-    branches: master
+    branches:
+      - master
+      - "maint-**"
   schedule:
     # * is a special character in YAML so you have to quote this string
     - cron: "0 3 * * 6"
   workflow_dispatch:
     inputs:
       reason:
         description: "Reason"
```

### Comparing `invenio-indexer-2.1.1/AUTHORS.rst` & `invenio-indexer-2.1.2/AUTHORS.rst`

 * *Files identical despite different names*

### Comparing `invenio-indexer-2.1.1/CHANGES.rst` & `invenio-indexer-2.1.2/CHANGES.rst`

 * *Files 5% similar despite different names*

```diff
@@ -1,23 +1,28 @@
 ..
     This file is part of Invenio.
-    Copyright (C) 2016-2022 CERN.
+    Copyright (C) 2016-2023 CERN.
 
     Invenio is free software; you can redistribute it and/or modify it
     under the terms of the MIT License; see LICENSE file for more details.
 
 Changes
 =======
 
-Version 2.1.1 (releases 2022-10-07)
+Version 2.1.2 (released 2023-05-05)
+
+- Allow passing message queue producer publish arguments via the ``RecordIndexer``
+  constructor and the ``INDEXER_MQ_PUBLISH_KWARGS`` config.
+
+Version 2.1.1 (released 2022-10-07)
 
 - Change `schema_to_index` to return only the index and not a tuple with index and
   doc type.
 
-Version 2.1.0 (releases 2022-10-03)
+Version 2.1.0 (released 2022-10-03)
 
 - Add support to OpenSearch v2
 - Remove `doc_type` param
 - Change `record_to_index` to return only the index and not a tuple with index and
   doc type.
 - Remove the config var `INDEXER_DEFAULT_DOC_TYPE`
```

### Comparing `invenio-indexer-2.1.1/CONTRIBUTING.rst` & `invenio-indexer-2.1.2/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `invenio-indexer-2.1.1/INSTALL.rst` & `invenio-indexer-2.1.2/INSTALL.rst`

 * *Files identical despite different names*

### Comparing `invenio-indexer-2.1.1/LICENSE` & `invenio-indexer-2.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `invenio-indexer-2.1.1/MANIFEST.in` & `invenio-indexer-2.1.2/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `invenio-indexer-2.1.1/PKG-INFO` & `invenio-indexer-2.1.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: invenio-indexer
-Version: 2.1.1
+Version: 2.1.2
 Summary: "Record indexer for Invenio."
 Home-page: https://github.com/inveniosoftware/invenio-indexer
 Author: CERN
 Author-email: info@inveniosoftware.org
 License: MIT
 Description: ..
             This file is part of Invenio.
@@ -33,28 +33,33 @@
         Record indexer for Invenio.
         
         Further documentation is available on
         https://invenio-indexer.readthedocs.io/
         
         ..
             This file is part of Invenio.
-            Copyright (C) 2016-2022 CERN.
+            Copyright (C) 2016-2023 CERN.
         
             Invenio is free software; you can redistribute it and/or modify it
             under the terms of the MIT License; see LICENSE file for more details.
         
         Changes
         =======
         
-        Version 2.1.1 (releases 2022-10-07)
+        Version 2.1.2 (released 2023-05-05)
+        
+        - Allow passing message queue producer publish arguments via the ``RecordIndexer``
+          constructor and the ``INDEXER_MQ_PUBLISH_KWARGS`` config.
+        
+        Version 2.1.1 (released 2022-10-07)
         
         - Change `schema_to_index` to return only the index and not a tuple with index and
           doc type.
         
-        Version 2.1.0 (releases 2022-10-03)
+        Version 2.1.0 (released 2022-10-03)
         
         - Add support to OpenSearch v2
         - Remove `doc_type` param
         - Change `record_to_index` to return only the index and not a tuple with index and
           doc type.
         - Remove the config var `INDEXER_DEFAULT_DOC_TYPE`
```

### Comparing `invenio-indexer-2.1.1/README.rst` & `invenio-indexer-2.1.2/README.rst`

 * *Files identical despite different names*

### Comparing `invenio-indexer-2.1.1/docs/Makefile` & `invenio-indexer-2.1.2/docs/Makefile`

 * *Files identical despite different names*

### Comparing `invenio-indexer-2.1.1/docs/api.rst` & `invenio-indexer-2.1.2/docs/api.rst`

 * *Files identical despite different names*

### Comparing `invenio-indexer-2.1.1/docs/conf.py` & `invenio-indexer-2.1.2/docs/conf.py`

 * *Files identical despite different names*

### Comparing `invenio-indexer-2.1.1/docs/index.rst` & `invenio-indexer-2.1.2/docs/index.rst`

 * *Files identical despite different names*

### Comparing `invenio-indexer-2.1.1/docs/make.bat` & `invenio-indexer-2.1.2/docs/make.bat`

 * *Files identical despite different names*

### Comparing `invenio-indexer-2.1.1/invenio_indexer/__init__.py` & `invenio-indexer-2.1.2/invenio_indexer/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # -*- coding: utf-8 -*-
 #
 # This file is part of Invenio.
-# Copyright (C) 2016-2022 CERN.
+# Copyright (C) 2016-2023 CERN.
 #
 # Invenio is free software; you can redistribute it and/or modify it
 # under the terms of the MIT License; see LICENSE file for more details.
 
 """Record indexer for Invenio.
 
 Invenio-Indexer is responsible for sending records for indexing to the search
@@ -176,10 +176,10 @@
 >>> res = before_record_index.dynamic_connect(
 ...     indexer_receiver, sender=app, index='authors-v1.0.0')
 """
 
 from .ext import InvenioIndexer
 from .proxies import current_record_to_index
 
-__version__ = "2.1.1"
+__version__ = "2.1.2"
 
 __all__ = ("__version__", "InvenioIndexer", "current_record_to_index")
```

### Comparing `invenio-indexer-2.1.1/invenio_indexer/api.py` & `invenio-indexer-2.1.2/invenio_indexer/api.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 from contextlib import contextmanager
 
 import pytz
 from celery import current_app as current_celery_app
 from flask import current_app
 from invenio_records.api import Record
 from invenio_search import current_search_client
-from invenio_search.engine import check_os_version, dsl, search
+from invenio_search.engine import dsl, search
 from invenio_search.utils import build_alias_name
 from kombu import Producer as KombuProducer
 from kombu.compat import Consumer
 from sqlalchemy.orm.exc import NoResultFound
 
 from .proxies import current_record_to_index
 from .signals import before_record_index
@@ -65,14 +65,15 @@
         exchange=None,
         queue=None,
         routing_key=None,
         version_type=None,
         record_to_index=None,
         record_cls=None,
         record_dumper=None,
+        publish_kwargs=None,
     ):
         """Initialize indexer.
 
         :param search_client: search engine client.
             (Default: ``current_search_client``)
         :param exchange: A :class:`kombu.Exchange` instance for message queue.
         :param queue: A :class:`kombu.Queue` instance for message queue.
@@ -89,14 +90,15 @@
         """
         self.client = search_client or current_search_client
         self._exchange = exchange
         self._queue = queue
         self._record_to_index = record_to_index or current_record_to_index
         self._routing_key = routing_key
         self._version_type = version_type or "external_gte"
+        self._publish_kwargs = publish_kwargs
 
         if record_cls:
             self.record_cls = record_cls
         if record_dumper:
             self.record_dumper = record_dumper
 
     def record_to_index(self, record):
@@ -140,14 +142,21 @@
     def mq_routing_key(self):
         """Message Queue routing key.
 
         :returns: The Message Queue routing key.
         """
         return self._routing_key or current_app.config["INDEXER_MQ_ROUTING_KEY"]
 
+    @property
+    def mq_publish_kwargs(self):
+        """Message Queue producer publish kwargs."""
+        if self._publish_kwargs is not None:  # this allows overriding to {}
+            return self._publish_kwargs
+        return current_app.config["INDEXER_MQ_PUBLISH_KWARGS"]
+
     #
     # High-level API
     #
     def index(self, record, arguments=None, **kwargs):
         """Index a record.
 
         The caller is responsible for ensuring that the record has already been
@@ -311,15 +320,19 @@
         with self.create_producer() as producer:
             for rec in record_id_iterator:
                 data = dict(
                     id=str(rec),
                     op=op_type,
                     index=index,
                 )
-                producer.publish(data, declare=[self.mq_queue])
+                producer.publish(
+                    data,
+                    declare=[self.mq_queue],
+                    **self.mq_publish_kwargs,
+                )
 
     def _actionsiter(self, message_iterator):
         """Iterate bulk actions.
 
         :param message_iterator: Iterator yielding messages from a queue.
         """
         for message in message_iterator:
```

### Comparing `invenio-indexer-2.1.1/invenio_indexer/cli.py` & `invenio-indexer-2.1.2/invenio_indexer/cli.py`

 * *Files identical despite different names*

### Comparing `invenio-indexer-2.1.1/invenio_indexer/ext.py` & `invenio-indexer-2.1.2/invenio_indexer/ext.py`

 * *Files identical despite different names*

### Comparing `invenio-indexer-2.1.1/invenio_indexer/proxies.py` & `invenio-indexer-2.1.2/invenio_indexer/proxies.py`

 * *Files identical despite different names*

### Comparing `invenio-indexer-2.1.1/invenio_indexer/registry.py` & `invenio-indexer-2.1.2/invenio_indexer/registry.py`

 * *Files identical despite different names*

### Comparing `invenio-indexer-2.1.1/invenio_indexer/signals.py` & `invenio-indexer-2.1.2/invenio_indexer/signals.py`

 * *Files identical despite different names*

### Comparing `invenio-indexer-2.1.1/invenio_indexer/tasks.py` & `invenio-indexer-2.1.2/invenio_indexer/tasks.py`

 * *Files identical despite different names*

### Comparing `invenio-indexer-2.1.1/invenio_indexer/utils.py` & `invenio-indexer-2.1.2/invenio_indexer/utils.py`

 * *Files identical despite different names*

### Comparing `invenio-indexer-2.1.1/invenio_indexer.egg-info/PKG-INFO` & `invenio-indexer-2.1.2/invenio_indexer.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: invenio-indexer
-Version: 2.1.1
+Version: 2.1.2
 Summary: "Record indexer for Invenio."
 Home-page: https://github.com/inveniosoftware/invenio-indexer
 Author: CERN
 Author-email: info@inveniosoftware.org
 License: MIT
 Description: ..
             This file is part of Invenio.
@@ -33,28 +33,33 @@
         Record indexer for Invenio.
         
         Further documentation is available on
         https://invenio-indexer.readthedocs.io/
         
         ..
             This file is part of Invenio.
-            Copyright (C) 2016-2022 CERN.
+            Copyright (C) 2016-2023 CERN.
         
             Invenio is free software; you can redistribute it and/or modify it
             under the terms of the MIT License; see LICENSE file for more details.
         
         Changes
         =======
         
-        Version 2.1.1 (releases 2022-10-07)
+        Version 2.1.2 (released 2023-05-05)
+        
+        - Allow passing message queue producer publish arguments via the ``RecordIndexer``
+          constructor and the ``INDEXER_MQ_PUBLISH_KWARGS`` config.
+        
+        Version 2.1.1 (released 2022-10-07)
         
         - Change `schema_to_index` to return only the index and not a tuple with index and
           doc type.
         
-        Version 2.1.0 (releases 2022-10-03)
+        Version 2.1.0 (released 2022-10-03)
         
         - Add support to OpenSearch v2
         - Remove `doc_type` param
         - Change `record_to_index` to return only the index and not a tuple with index and
           doc type.
         - Remove the config var `INDEXER_DEFAULT_DOC_TYPE`
```

### Comparing `invenio-indexer-2.1.1/invenio_indexer.egg-info/SOURCES.txt` & `invenio-indexer-2.1.2/invenio_indexer.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `invenio-indexer-2.1.1/run-tests.sh` & `invenio-indexer-2.1.2/run-tests.sh`

 * *Files identical despite different names*

### Comparing `invenio-indexer-2.1.1/setup.cfg` & `invenio-indexer-2.1.2/setup.cfg`

 * *Files identical despite different names*

### Comparing `invenio-indexer-2.1.1/tests/conftest.py` & `invenio-indexer-2.1.2/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `invenio-indexer-2.1.1/tests/test_api.py` & `invenio-indexer-2.1.2/tests/test_api.py`

 * *Files identical despite different names*

### Comparing `invenio-indexer-2.1.1/tests/test_cli.py` & `invenio-indexer-2.1.2/tests/test_cli.py`

 * *Files identical despite different names*

### Comparing `invenio-indexer-2.1.1/tests/test_invenio_indexer.py` & `invenio-indexer-2.1.2/tests/test_invenio_indexer.py`

 * *Files identical despite different names*

### Comparing `invenio-indexer-2.1.1/tests/test_registry.py` & `invenio-indexer-2.1.2/tests/test_registry.py`

 * *Files identical despite different names*

### Comparing `invenio-indexer-2.1.1/tests/test_tasks.py` & `invenio-indexer-2.1.2/tests/test_tasks.py`

 * *Files identical despite different names*

### Comparing `invenio-indexer-2.1.1/tests/test_utils.py` & `invenio-indexer-2.1.2/tests/test_utils.py`

 * *Files identical despite different names*

