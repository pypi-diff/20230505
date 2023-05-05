# Comparing `tmp/cleanlab-studio-1.0.0.tar.gz` & `tmp/cleanlab-studio-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cleanlab-studio-1.0.0.tar", last modified: Wed May  3 02:00:04 2023, max compression
+gzip compressed data, was "cleanlab-studio-1.0.1.tar", last modified: Fri May  5 11:50:09 2023, max compression
```

## Comparing `cleanlab-studio-1.0.0.tar` & `cleanlab-studio-1.0.1.tar`

### file list

```diff
@@ -1,83 +1,83 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 02:00:04.929316 cleanlab-studio-1.0.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-05-03 01:59:47.000000 cleanlab-studio-1.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     8477 2023-05-03 02:00:04.929316 cleanlab-studio-1.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7311 2023-05-03 01:59:47.000000 cleanlab-studio-1.0.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 02:00:04.917315 cleanlab-studio-1.0.0/cleanlab_studio/
--rw-r--r--   0 runner    (1001) docker     (123)       83 2023-05-03 01:59:47.000000 cleanlab-studio-1.0.0/cleanlab_studio/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 02:00:04.925315 cleanlab-studio-1.0.0/cleanlab_studio/cli/
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-05-03 01:59:47.000000 cleanlab-studio-1.0.0/cleanlab_studio/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11615 2023-05-03 01:59:47.000000 cleanlab-studio-1.0.0/cleanlab_studio/cli/api_service.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 02:00:04.925315 cleanlab-studio-1.0.0/cleanlab_studio/cli/classes/
--rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-03 01:59:47.000000 cleanlab-studio-1.0.0/cleanlab_studio/cli/classes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1367 2023-05-03 01:59:47.000000 cleanlab-studio-1.0.0/cleanlab_studio/cli/classes/csv_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     2046 2023-05-03 01:59:47.000000 cleanlab-studio-1.0.0/cleanlab_studio/cli/classes/dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     2429 2023-05-03 01:59:47.000000 cleanlab-studio-1.0.0/cleanlab_studio/cli/classes/excel_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)      886 2023-05-03 01:59:47.000000 cleanlab-studio-1.0.0/cleanlab_studio/cli/classes/json_dataset.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 02:00:04.925315 cleanlab-studio-1.0.0/cleanlab_studio/cli/cleanset/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 01:59:47.000000 cleanlab-studio-1.0.0/cleanlab_studio/cli/cleanset/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      202 2023-05-03 01:59:47.000000 cleanlab-studio-1.0.0/cleanlab_studio/cli/cleanset/commands.py
--rw-r--r--   0 runner    (1001) docker     (123)     3734 2023-05-03 01:59:47.000000 cleanlab-studio-1.0.0/cleanlab_studio/cli/cleanset/download.py
--rw-r--r--   0 runner    (1001) docker     (123)     1366 2023-05-03 01:59:47.000000 cleanlab-studio-1.0.0/cleanlab_studio/cli/cleanset/download_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1852 2023-05-03 01:59:47.000000 cleanlab-studio-1.0.0/cleanlab_studio/cli/click_helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 02:00:04.925315 cleanlab-studio-1.0.0/cleanlab_studio/cli/dataset/
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-05-03 01:59:47.000000 cleanlab-studio-1.0.0/cleanlab_studio/cli/dataset/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      204 2023-05-03 01:59:47.000000 cleanlab-studio-1.0.0/cleanlab_studio/cli/dataset/commands.py
--rw-r--r--   0 runner    (1001) docker     (123)     1042 2023-05-03 01:59:47.000000 cleanlab-studio-1.0.0/cleanlab_studio/cli/dataset/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)      713 2023-05-03 01:59:47.000000 cleanlab-studio-1.0.0/cleanlab_studio/cli/dataset/image_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    14872 2023-05-03 01:59:47.000000 cleanlab-studio-1.0.0/cleanlab_studio/cli/dataset/schema_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     4911 2023-05-03 01:59:47.000000 cleanlab-studio-1.0.0/cleanlab_studio/cli/dataset/schema_types.py
--rw-r--r--   0 runner    (1001) docker     (123)     3064 2023-05-03 01:59:47.000000 cleanlab-studio-1.0.0/cleanlab_studio/cli/dataset/upload.py
--rw-r--r--   0 runner    (1001) docker     (123)    24955 2023-05-03 01:59:47.000000 cleanlab-studio-1.0.0/cleanlab_studio/cli/dataset/upload_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     2476 2023-05-03 01:59:47.000000 cleanlab-studio-1.0.0/cleanlab_studio/cli/dataset/upload_types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 02:00:04.925315 cleanlab-studio-1.0.0/cleanlab_studio/cli/decorators/
--rw-r--r--   0 runner    (1001) docker     (123)      113 2023-05-03 01:59:47.000000 cleanlab-studio-1.0.0/cleanlab_studio/cli/decorators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      974 2023-05-03 01:59:47.000000 cleanlab-studio-1.0.0/cleanlab_studio/cli/decorators/auth_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1805 2023-05-03 01:59:47.000000 cleanlab-studio-1.0.0/cleanlab_studio/cli/decorators/previous_state.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 02:00:04.925315 cleanlab-studio-1.0.0/cleanlab_studio/cli/login/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 01:59:47.000000 cleanlab-studio-1.0.0/cleanlab_studio/cli/login/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1809 2023-05-03 01:59:47.000000 cleanlab-studio-1.0.0/cleanlab_studio/cli/login/login.py
--rw-r--r--   0 runner    (1001) docker     (123)     1583 2023-05-03 01:59:47.000000 cleanlab-studio-1.0.0/cleanlab_studio/cli/main.py
--rw-r--r--   0 runner    (1001) docker     (123)      694 2023-05-03 01:59:47.000000 cleanlab-studio-1.0.0/cleanlab_studio/cli/types.py
--rw-r--r--   0 runner    (1001) docker     (123)     4796 2023-05-03 01:59:47.000000 cleanlab-studio-1.0.0/cleanlab_studio/cli/util.py
--rw-r--r--   0 runner    (1001) docker     (123)      530 2023-05-03 01:59:47.000000 cleanlab-studio-1.0.0/cleanlab_studio/errors.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 02:00:04.929316 cleanlab-studio-1.0.0/cleanlab_studio/internal/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 01:59:47.000000 cleanlab-studio-1.0.0/cleanlab_studio/internal/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 02:00:04.929316 cleanlab-studio-1.0.0/cleanlab_studio/internal/api/
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-03 01:59:47.000000 cleanlab-studio-1.0.0/cleanlab_studio/internal/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6533 2023-05-03 01:59:47.000000 cleanlab-studio-1.0.0/cleanlab_studio/internal/api/api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 02:00:04.929316 cleanlab-studio-1.0.0/cleanlab_studio/internal/dataset_source/
--rw-r--r--   0 runner    (1001) docker     (123)      451 2023-05-03 01:59:47.000000 cleanlab-studio-1.0.0/cleanlab_studio/internal/dataset_source/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1206 2023-05-03 01:59:47.000000 cleanlab-studio-1.0.0/cleanlab_studio/internal/dataset_source/dataframe_dataset_source.py
--rw-r--r--   0 runner    (1001) docker     (123)     1145 2023-05-03 01:59:47.000000 cleanlab-studio-1.0.0/cleanlab_studio/internal/dataset_source/dataset_source.py
--rw-r--r--   0 runner    (1001) docker     (123)      901 2023-05-03 01:59:47.000000 cleanlab-studio-1.0.0/cleanlab_studio/internal/dataset_source/filepath_dataset_source.py
--rw-r--r--   0 runner    (1001) docker     (123)      367 2023-05-03 01:59:47.000000 cleanlab-studio-1.0.0/cleanlab_studio/internal/dataset_source/pandas_dataset_source.py
--rw-r--r--   0 runner    (1001) docker     (123)      603 2023-05-03 01:59:47.000000 cleanlab-studio-1.0.0/cleanlab_studio/internal/dataset_source/pyspark_dataset_source.py
--rw-r--r--   0 runner    (1001) docker     (123)     3304 2023-05-03 01:59:47.000000 cleanlab-studio-1.0.0/cleanlab_studio/internal/settings.py
--rw-r--r--   0 runner    (1001) docker     (123)      217 2023-05-03 01:59:47.000000 cleanlab-studio-1.0.0/cleanlab_studio/internal/types.py
--rw-r--r--   0 runner    (1001) docker     (123)     2717 2023-05-03 01:59:47.000000 cleanlab-studio-1.0.0/cleanlab_studio/internal/upload_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     1882 2023-05-03 01:59:47.000000 cleanlab-studio-1.0.0/cleanlab_studio/internal/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 02:00:04.929316 cleanlab-studio-1.0.0/cleanlab_studio/studio/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 01:59:47.000000 cleanlab-studio-1.0.0/cleanlab_studio/studio/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5818 2023-05-03 01:59:47.000000 cleanlab-studio-1.0.0/cleanlab_studio/studio/studio.py
--rw-r--r--   0 runner    (1001) docker     (123)     1480 2023-05-03 01:59:47.000000 cleanlab-studio-1.0.0/cleanlab_studio/studio/upload.py
--rw-r--r--   0 runner    (1001) docker     (123)      196 2023-05-03 01:59:47.000000 cleanlab-studio-1.0.0/cleanlab_studio/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 02:00:04.921315 cleanlab-studio-1.0.0/cleanlab_studio.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8477 2023-05-03 02:00:04.000000 cleanlab-studio-1.0.0/cleanlab_studio.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2479 2023-05-03 02:00:04.000000 cleanlab-studio-1.0.0/cleanlab_studio.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-03 02:00:04.000000 cleanlab-studio-1.0.0/cleanlab_studio.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-05-03 02:00:04.000000 cleanlab-studio-1.0.0/cleanlab_studio.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      246 2023-05-03 02:00:04.000000 cleanlab-studio-1.0.0/cleanlab_studio.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-05-03 02:00:04.000000 cleanlab-studio-1.0.0/cleanlab_studio.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      109 2023-05-03 01:59:47.000000 cleanlab-studio-1.0.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-03 02:00:04.929316 cleanlab-studio-1.0.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2181 2023-05-03 01:59:47.000000 cleanlab-studio-1.0.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 02:00:04.929316 cleanlab-studio-1.0.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 01:59:47.000000 cleanlab-studio-1.0.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1727 2023-05-03 01:59:47.000000 cleanlab-studio-1.0.0/tests/bench.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 02:00:04.929316 cleanlab-studio-1.0.0/tests/datasets/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 01:59:47.000000 cleanlab-studio-1.0.0/tests/datasets/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      109 2023-05-03 01:59:47.000000 cleanlab-studio-1.0.0/tests/datasets/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     1774 2023-05-03 01:59:47.000000 cleanlab-studio-1.0.0/tests/datasets/test_csv_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     1941 2023-05-03 01:59:47.000000 cleanlab-studio-1.0.0/tests/datasets/test_excel_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     1850 2023-05-03 01:59:47.000000 cleanlab-studio-1.0.0/tests/datasets/test_json_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     3918 2023-05-03 01:59:47.000000 cleanlab-studio-1.0.0/tests/datasets/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 11:50:09.925400 cleanlab-studio-1.0.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-05-05 11:49:55.000000 cleanlab-studio-1.0.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     8477 2023-05-05 11:50:09.925400 cleanlab-studio-1.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7311 2023-05-05 11:49:55.000000 cleanlab-studio-1.0.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 11:50:09.917400 cleanlab-studio-1.0.1/cleanlab_studio/
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-05-05 11:49:55.000000 cleanlab-studio-1.0.1/cleanlab_studio/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 11:50:09.921400 cleanlab-studio-1.0.1/cleanlab_studio/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-05-05 11:49:55.000000 cleanlab-studio-1.0.1/cleanlab_studio/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11615 2023-05-05 11:49:55.000000 cleanlab-studio-1.0.1/cleanlab_studio/cli/api_service.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 11:50:09.921400 cleanlab-studio-1.0.1/cleanlab_studio/cli/classes/
+-rw-r--r--   0 runner    (1001) docker     (123)      159 2023-05-05 11:49:55.000000 cleanlab-studio-1.0.1/cleanlab_studio/cli/classes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1367 2023-05-05 11:49:55.000000 cleanlab-studio-1.0.1/cleanlab_studio/cli/classes/csv_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2046 2023-05-05 11:49:55.000000 cleanlab-studio-1.0.1/cleanlab_studio/cli/classes/dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2429 2023-05-05 11:49:55.000000 cleanlab-studio-1.0.1/cleanlab_studio/cli/classes/excel_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)      886 2023-05-05 11:49:55.000000 cleanlab-studio-1.0.1/cleanlab_studio/cli/classes/json_dataset.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 11:50:09.921400 cleanlab-studio-1.0.1/cleanlab_studio/cli/cleanset/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 11:49:55.000000 cleanlab-studio-1.0.1/cleanlab_studio/cli/cleanset/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      202 2023-05-05 11:49:55.000000 cleanlab-studio-1.0.1/cleanlab_studio/cli/cleanset/commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3734 2023-05-05 11:49:55.000000 cleanlab-studio-1.0.1/cleanlab_studio/cli/cleanset/download.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1366 2023-05-05 11:49:55.000000 cleanlab-studio-1.0.1/cleanlab_studio/cli/cleanset/download_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1852 2023-05-05 11:49:55.000000 cleanlab-studio-1.0.1/cleanlab_studio/cli/click_helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 11:50:09.921400 cleanlab-studio-1.0.1/cleanlab_studio/cli/dataset/
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-05-05 11:49:55.000000 cleanlab-studio-1.0.1/cleanlab_studio/cli/dataset/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      204 2023-05-05 11:49:55.000000 cleanlab-studio-1.0.1/cleanlab_studio/cli/dataset/commands.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1042 2023-05-05 11:49:55.000000 cleanlab-studio-1.0.1/cleanlab_studio/cli/dataset/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      713 2023-05-05 11:49:55.000000 cleanlab-studio-1.0.1/cleanlab_studio/cli/dataset/image_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14872 2023-05-05 11:49:55.000000 cleanlab-studio-1.0.1/cleanlab_studio/cli/dataset/schema_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4911 2023-05-05 11:49:55.000000 cleanlab-studio-1.0.1/cleanlab_studio/cli/dataset/schema_types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3064 2023-05-05 11:49:55.000000 cleanlab-studio-1.0.1/cleanlab_studio/cli/dataset/upload.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24955 2023-05-05 11:49:55.000000 cleanlab-studio-1.0.1/cleanlab_studio/cli/dataset/upload_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2476 2023-05-05 11:49:55.000000 cleanlab-studio-1.0.1/cleanlab_studio/cli/dataset/upload_types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 11:50:09.921400 cleanlab-studio-1.0.1/cleanlab_studio/cli/decorators/
+-rw-r--r--   0 runner    (1001) docker     (123)      113 2023-05-05 11:49:55.000000 cleanlab-studio-1.0.1/cleanlab_studio/cli/decorators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      974 2023-05-05 11:49:55.000000 cleanlab-studio-1.0.1/cleanlab_studio/cli/decorators/auth_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1805 2023-05-05 11:49:55.000000 cleanlab-studio-1.0.1/cleanlab_studio/cli/decorators/previous_state.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 11:50:09.925400 cleanlab-studio-1.0.1/cleanlab_studio/cli/login/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 11:49:55.000000 cleanlab-studio-1.0.1/cleanlab_studio/cli/login/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1809 2023-05-05 11:49:55.000000 cleanlab-studio-1.0.1/cleanlab_studio/cli/login/login.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1583 2023-05-05 11:49:55.000000 cleanlab-studio-1.0.1/cleanlab_studio/cli/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)      694 2023-05-05 11:49:55.000000 cleanlab-studio-1.0.1/cleanlab_studio/cli/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4796 2023-05-05 11:49:55.000000 cleanlab-studio-1.0.1/cleanlab_studio/cli/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)      530 2023-05-05 11:49:55.000000 cleanlab-studio-1.0.1/cleanlab_studio/errors.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 11:50:09.925400 cleanlab-studio-1.0.1/cleanlab_studio/internal/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 11:49:55.000000 cleanlab-studio-1.0.1/cleanlab_studio/internal/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 11:50:09.925400 cleanlab-studio-1.0.1/cleanlab_studio/internal/api/
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-05 11:49:55.000000 cleanlab-studio-1.0.1/cleanlab_studio/internal/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6533 2023-05-05 11:49:55.000000 cleanlab-studio-1.0.1/cleanlab_studio/internal/api/api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 11:50:09.925400 cleanlab-studio-1.0.1/cleanlab_studio/internal/dataset_source/
+-rw-r--r--   0 runner    (1001) docker     (123)      451 2023-05-05 11:49:55.000000 cleanlab-studio-1.0.1/cleanlab_studio/internal/dataset_source/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1206 2023-05-05 11:49:55.000000 cleanlab-studio-1.0.1/cleanlab_studio/internal/dataset_source/dataframe_dataset_source.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1145 2023-05-05 11:49:55.000000 cleanlab-studio-1.0.1/cleanlab_studio/internal/dataset_source/dataset_source.py
+-rw-r--r--   0 runner    (1001) docker     (123)      901 2023-05-05 11:49:55.000000 cleanlab-studio-1.0.1/cleanlab_studio/internal/dataset_source/filepath_dataset_source.py
+-rw-r--r--   0 runner    (1001) docker     (123)      367 2023-05-05 11:49:55.000000 cleanlab-studio-1.0.1/cleanlab_studio/internal/dataset_source/pandas_dataset_source.py
+-rw-r--r--   0 runner    (1001) docker     (123)      603 2023-05-05 11:49:55.000000 cleanlab-studio-1.0.1/cleanlab_studio/internal/dataset_source/pyspark_dataset_source.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3304 2023-05-05 11:49:55.000000 cleanlab-studio-1.0.1/cleanlab_studio/internal/settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)      217 2023-05-05 11:49:55.000000 cleanlab-studio-1.0.1/cleanlab_studio/internal/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2717 2023-05-05 11:49:55.000000 cleanlab-studio-1.0.1/cleanlab_studio/internal/upload_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1882 2023-05-05 11:49:55.000000 cleanlab-studio-1.0.1/cleanlab_studio/internal/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 11:50:09.925400 cleanlab-studio-1.0.1/cleanlab_studio/studio/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 11:49:55.000000 cleanlab-studio-1.0.1/cleanlab_studio/studio/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5875 2023-05-05 11:49:55.000000 cleanlab-studio-1.0.1/cleanlab_studio/studio/studio.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1480 2023-05-05 11:49:55.000000 cleanlab-studio-1.0.1/cleanlab_studio/studio/upload.py
+-rw-r--r--   0 runner    (1001) docker     (123)      196 2023-05-05 11:49:55.000000 cleanlab-studio-1.0.1/cleanlab_studio/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 11:50:09.921400 cleanlab-studio-1.0.1/cleanlab_studio.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8477 2023-05-05 11:50:09.000000 cleanlab-studio-1.0.1/cleanlab_studio.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2479 2023-05-05 11:50:09.000000 cleanlab-studio-1.0.1/cleanlab_studio.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 11:50:09.000000 cleanlab-studio-1.0.1/cleanlab_studio.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-05-05 11:50:09.000000 cleanlab-studio-1.0.1/cleanlab_studio.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      246 2023-05-05 11:50:09.000000 cleanlab-studio-1.0.1/cleanlab_studio.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-05-05 11:50:09.000000 cleanlab-studio-1.0.1/cleanlab_studio.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      109 2023-05-05 11:49:55.000000 cleanlab-studio-1.0.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-05 11:50:09.925400 cleanlab-studio-1.0.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2181 2023-05-05 11:49:55.000000 cleanlab-studio-1.0.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 11:50:09.925400 cleanlab-studio-1.0.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 11:49:55.000000 cleanlab-studio-1.0.1/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1727 2023-05-05 11:49:55.000000 cleanlab-studio-1.0.1/tests/bench.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 11:50:09.925400 cleanlab-studio-1.0.1/tests/datasets/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 11:49:55.000000 cleanlab-studio-1.0.1/tests/datasets/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      109 2023-05-05 11:49:55.000000 cleanlab-studio-1.0.1/tests/datasets/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1774 2023-05-05 11:49:55.000000 cleanlab-studio-1.0.1/tests/datasets/test_csv_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1941 2023-05-05 11:49:55.000000 cleanlab-studio-1.0.1/tests/datasets/test_excel_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1850 2023-05-05 11:49:55.000000 cleanlab-studio-1.0.1/tests/datasets/test_json_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3918 2023-05-05 11:49:55.000000 cleanlab-studio-1.0.1/tests/datasets/utils.py
```

### Comparing `cleanlab-studio-1.0.0/LICENSE` & `cleanlab-studio-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `cleanlab-studio-1.0.0/PKG-INFO` & `cleanlab-studio-1.0.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cleanlab-studio
-Version: 1.0.0
+Version: 1.0.1
 Summary: Client interface for all things Cleanlab Studio
 Home-page: https://github.com/cleanlab/cleanlab-studio
 Author: Cleanlab Inc
 Author-email: team@cleanlab.ai
 License: MIT
 Project-URL: Bug Tracker, https://github.com/cleanlab/cleanlab-studio/issues
 Keywords: cleanlab
```

### Comparing `cleanlab-studio-1.0.0/README.md` & `cleanlab-studio-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `cleanlab-studio-1.0.0/cleanlab_studio/cli/api_service.py` & `cleanlab-studio-1.0.1/cleanlab_studio/cli/api_service.py`

 * *Files identical despite different names*

### Comparing `cleanlab-studio-1.0.0/cleanlab_studio/cli/classes/csv_dataset.py` & `cleanlab-studio-1.0.1/cleanlab_studio/cli/classes/csv_dataset.py`

 * *Files identical despite different names*

### Comparing `cleanlab-studio-1.0.0/cleanlab_studio/cli/classes/dataset.py` & `cleanlab-studio-1.0.1/cleanlab_studio/cli/classes/dataset.py`

 * *Files identical despite different names*

### Comparing `cleanlab-studio-1.0.0/cleanlab_studio/cli/classes/excel_dataset.py` & `cleanlab-studio-1.0.1/cleanlab_studio/cli/classes/excel_dataset.py`

 * *Files identical despite different names*

### Comparing `cleanlab-studio-1.0.0/cleanlab_studio/cli/classes/json_dataset.py` & `cleanlab-studio-1.0.1/cleanlab_studio/cli/classes/json_dataset.py`

 * *Files identical despite different names*

### Comparing `cleanlab-studio-1.0.0/cleanlab_studio/cli/cleanset/download.py` & `cleanlab-studio-1.0.1/cleanlab_studio/cli/cleanset/download.py`

 * *Files identical despite different names*

### Comparing `cleanlab-studio-1.0.0/cleanlab_studio/cli/cleanset/download_helpers.py` & `cleanlab-studio-1.0.1/cleanlab_studio/cli/cleanset/download_helpers.py`

 * *Files identical despite different names*

### Comparing `cleanlab-studio-1.0.0/cleanlab_studio/cli/click_helpers.py` & `cleanlab-studio-1.0.1/cleanlab_studio/cli/click_helpers.py`

 * *Files identical despite different names*

### Comparing `cleanlab-studio-1.0.0/cleanlab_studio/cli/dataset/helpers.py` & `cleanlab-studio-1.0.1/cleanlab_studio/cli/dataset/helpers.py`

 * *Files identical despite different names*

### Comparing `cleanlab-studio-1.0.0/cleanlab_studio/cli/dataset/image_utils.py` & `cleanlab-studio-1.0.1/cleanlab_studio/cli/dataset/image_utils.py`

 * *Files identical despite different names*

### Comparing `cleanlab-studio-1.0.0/cleanlab_studio/cli/dataset/schema_helpers.py` & `cleanlab-studio-1.0.1/cleanlab_studio/cli/dataset/schema_helpers.py`

 * *Files identical despite different names*

### Comparing `cleanlab-studio-1.0.0/cleanlab_studio/cli/dataset/schema_types.py` & `cleanlab-studio-1.0.1/cleanlab_studio/cli/dataset/schema_types.py`

 * *Files identical despite different names*

### Comparing `cleanlab-studio-1.0.0/cleanlab_studio/cli/dataset/upload.py` & `cleanlab-studio-1.0.1/cleanlab_studio/cli/dataset/upload.py`

 * *Files identical despite different names*

### Comparing `cleanlab-studio-1.0.0/cleanlab_studio/cli/dataset/upload_helpers.py` & `cleanlab-studio-1.0.1/cleanlab_studio/cli/dataset/upload_helpers.py`

 * *Files identical despite different names*

### Comparing `cleanlab-studio-1.0.0/cleanlab_studio/cli/dataset/upload_types.py` & `cleanlab-studio-1.0.1/cleanlab_studio/cli/dataset/upload_types.py`

 * *Files identical despite different names*

### Comparing `cleanlab-studio-1.0.0/cleanlab_studio/cli/decorators/auth_config.py` & `cleanlab-studio-1.0.1/cleanlab_studio/cli/decorators/auth_config.py`

 * *Files identical despite different names*

### Comparing `cleanlab-studio-1.0.0/cleanlab_studio/cli/decorators/previous_state.py` & `cleanlab-studio-1.0.1/cleanlab_studio/cli/decorators/previous_state.py`

 * *Files identical despite different names*

### Comparing `cleanlab-studio-1.0.0/cleanlab_studio/cli/login/login.py` & `cleanlab-studio-1.0.1/cleanlab_studio/cli/login/login.py`

 * *Files identical despite different names*

### Comparing `cleanlab-studio-1.0.0/cleanlab_studio/cli/main.py` & `cleanlab-studio-1.0.1/cleanlab_studio/cli/main.py`

 * *Files identical despite different names*

### Comparing `cleanlab-studio-1.0.0/cleanlab_studio/cli/types.py` & `cleanlab-studio-1.0.1/cleanlab_studio/cli/types.py`

 * *Files identical despite different names*

### Comparing `cleanlab-studio-1.0.0/cleanlab_studio/cli/util.py` & `cleanlab-studio-1.0.1/cleanlab_studio/cli/util.py`

 * *Files identical despite different names*

### Comparing `cleanlab-studio-1.0.0/cleanlab_studio/errors.py` & `cleanlab-studio-1.0.1/cleanlab_studio/errors.py`

 * *Files identical despite different names*

### Comparing `cleanlab-studio-1.0.0/cleanlab_studio/internal/api/api.py` & `cleanlab-studio-1.0.1/cleanlab_studio/internal/api/api.py`

 * *Files identical despite different names*

### Comparing `cleanlab-studio-1.0.0/cleanlab_studio/internal/dataset_source/dataframe_dataset_source.py` & `cleanlab-studio-1.0.1/cleanlab_studio/internal/dataset_source/dataframe_dataset_source.py`

 * *Files identical despite different names*

### Comparing `cleanlab-studio-1.0.0/cleanlab_studio/internal/dataset_source/dataset_source.py` & `cleanlab-studio-1.0.1/cleanlab_studio/internal/dataset_source/dataset_source.py`

 * *Files identical despite different names*

### Comparing `cleanlab-studio-1.0.0/cleanlab_studio/internal/dataset_source/filepath_dataset_source.py` & `cleanlab-studio-1.0.1/cleanlab_studio/internal/dataset_source/filepath_dataset_source.py`

 * *Files identical despite different names*

### Comparing `cleanlab-studio-1.0.0/cleanlab_studio/internal/dataset_source/pyspark_dataset_source.py` & `cleanlab-studio-1.0.1/cleanlab_studio/internal/dataset_source/pyspark_dataset_source.py`

 * *Files identical despite different names*

### Comparing `cleanlab-studio-1.0.0/cleanlab_studio/internal/settings.py` & `cleanlab-studio-1.0.1/cleanlab_studio/internal/settings.py`

 * *Files identical despite different names*

### Comparing `cleanlab-studio-1.0.0/cleanlab_studio/internal/upload_helpers.py` & `cleanlab-studio-1.0.1/cleanlab_studio/internal/upload_helpers.py`

 * *Files identical despite different names*

### Comparing `cleanlab-studio-1.0.0/cleanlab_studio/internal/util.py` & `cleanlab-studio-1.0.1/cleanlab_studio/internal/util.py`

 * *Files identical despite different names*

### Comparing `cleanlab-studio-1.0.0/cleanlab_studio/studio/studio.py` & `cleanlab-studio-1.0.1/cleanlab_studio/studio/studio.py`

 * *Files 6% similar despite different names*

```diff
@@ -125,14 +125,15 @@
 
         elif isinstance(dataset, pd.DataFrame):
             project_id = api.get_project_of_cleanset(self._api_key, cleanset_id)
             label_column = api.get_label_column_of_project(self._api_key, project_id)
             id_col = api.get_id_column(self._api_key, cleanset_id)
             cl_cols = self._download_cleanlab_columns(cleanset_id, project_id, label_column)
 
-            joined_ds = dataset.join(cl_cols, on=id_col, rsuffix="clean")
-            joined_ds["__cleanlab_final_label"] = cl_cols["cleanlab_clean_label"].where(
-                cl_cols["cleanlab_clean_label"] != "None", dataset[label_column]
+            joined_ds = dataset.join(cl_cols.set_index(id_col), on=id_col)
+            joined_ds["__cleanlab_final_label"] = joined_ds["cleanlab_clean_label"].where(
+                joined_ds["cleanlab_clean_label"] != "None", dataset[label_column]
             )
 
-            dataset[label_column] = joined_ds["__cleanlab_final_label"]
-            return dataset
+            corrected_ds = dataset.copy()
+            corrected_ds[label_column] = joined_ds["__cleanlab_final_label"]
+            return corrected_ds
```

### Comparing `cleanlab-studio-1.0.0/cleanlab_studio/studio/upload.py` & `cleanlab-studio-1.0.1/cleanlab_studio/studio/upload.py`

 * *Files identical despite different names*

### Comparing `cleanlab-studio-1.0.0/cleanlab_studio.egg-info/PKG-INFO` & `cleanlab-studio-1.0.1/cleanlab_studio.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cleanlab-studio
-Version: 1.0.0
+Version: 1.0.1
 Summary: Client interface for all things Cleanlab Studio
 Home-page: https://github.com/cleanlab/cleanlab-studio
 Author: Cleanlab Inc
 Author-email: team@cleanlab.ai
 License: MIT
 Project-URL: Bug Tracker, https://github.com/cleanlab/cleanlab-studio/issues
 Keywords: cleanlab
```

### Comparing `cleanlab-studio-1.0.0/cleanlab_studio.egg-info/SOURCES.txt` & `cleanlab-studio-1.0.1/cleanlab_studio.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cleanlab-studio-1.0.0/setup.py` & `cleanlab-studio-1.0.1/setup.py`

 * *Files identical despite different names*

### Comparing `cleanlab-studio-1.0.0/tests/bench.py` & `cleanlab-studio-1.0.1/tests/bench.py`

 * *Files identical despite different names*

### Comparing `cleanlab-studio-1.0.0/tests/datasets/test_csv_dataset.py` & `cleanlab-studio-1.0.1/tests/datasets/test_csv_dataset.py`

 * *Files identical despite different names*

### Comparing `cleanlab-studio-1.0.0/tests/datasets/test_excel_dataset.py` & `cleanlab-studio-1.0.1/tests/datasets/test_excel_dataset.py`

 * *Files identical despite different names*

### Comparing `cleanlab-studio-1.0.0/tests/datasets/test_json_dataset.py` & `cleanlab-studio-1.0.1/tests/datasets/test_json_dataset.py`

 * *Files identical despite different names*

### Comparing `cleanlab-studio-1.0.0/tests/datasets/utils.py` & `cleanlab-studio-1.0.1/tests/datasets/utils.py`

 * *Files identical despite different names*

