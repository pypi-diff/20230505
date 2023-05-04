# Comparing `tmp/unify-cli-3.2.1.tar.gz` & `tmp/unify-cli-3.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/unify-cli-3.2.1.tar", last modified: Fri Feb 24 22:47:48 2023, max compression
+gzip compressed data, was "dist/unify-cli-3.4.1.tar", last modified: Thu May  4 22:06:41 2023, max compression
```

## Comparing `unify-cli-3.2.1.tar` & `unify-cli-3.4.1.tar`

### file list

```diff
@@ -1,79 +1,81 @@
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-02-24 22:47:48.000000 unify-cli-3.2.1/
--rw-r--r--   0 circleci  (3434) circleci  (3434)    11358 2023-02-24 22:47:41.000000 unify-cli-3.2.1/LICENSE
--rw-r--r--   0 circleci  (3434) circleci  (3434)    10986 2023-02-24 22:47:48.000000 unify-cli-3.2.1/PKG-INFO
--rw-r--r--   0 circleci  (3434) circleci  (3434)    10552 2023-02-24 22:47:41.000000 unify-cli-3.2.1/README.md
--rw-r--r--   0 circleci  (3434) circleci  (3434)       38 2023-02-24 22:47:48.000000 unify-cli-3.2.1/setup.cfg
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1793 2023-02-24 22:47:41.000000 unify-cli-3.2.1/setup.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-02-24 22:47:48.000000 unify-cli-3.2.1/source/
--rw-r--r--   0 circleci  (3434) circleci  (3434)       34 2023-02-24 22:47:41.000000 unify-cli-3.2.1/source/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)       33 2023-02-24 22:47:41.000000 unify-cli-3.2.1/source/_version.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-02-24 22:47:48.000000 unify-cli-3.2.1/source/access/
--rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2023-02-24 22:47:41.000000 unify-cli-3.2.1/source/access/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2677 2023-02-24 22:47:41.000000 unify-cli-3.2.1/source/access/commands.py
--rwxr-xr-x   0 circleci  (3434) circleci  (3434)     2293 2023-02-24 22:47:41.000000 unify-cli-3.2.1/source/ah.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-02-24 22:47:48.000000 unify-cli-3.2.1/source/cluster/
--rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2023-02-24 22:47:41.000000 unify-cli-3.2.1/source/cluster/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3725 2023-02-24 22:47:41.000000 unify-cli-3.2.1/source/cluster/commands.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-02-24 22:47:48.000000 unify-cli-3.2.1/source/common/
--rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2023-02-24 22:47:41.000000 unify-cli-3.2.1/source/common/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1124 2023-02-24 22:47:41.000000 unify-cli-3.2.1/source/common/commands.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-02-24 22:47:48.000000 unify-cli-3.2.1/source/dataset/
--rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2023-02-24 22:47:41.000000 unify-cli-3.2.1/source/dataset/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     4854 2023-02-24 22:47:41.000000 unify-cli-3.2.1/source/dataset/commands.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-02-24 22:47:48.000000 unify-cli-3.2.1/source/datastream/
--rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2023-02-24 22:47:41.000000 unify-cli-3.2.1/source/datastream/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     4429 2023-02-24 22:47:41.000000 unify-cli-3.2.1/source/datastream/commands.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-02-24 22:47:48.000000 unify-cli-3.2.1/source/graph/
--rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2023-02-24 22:47:41.000000 unify-cli-3.2.1/source/graph/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2413 2023-02-24 22:47:41.000000 unify-cli-3.2.1/source/graph/commands.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-02-24 22:47:48.000000 unify-cli-3.2.1/source/hierarchy/
--rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2023-02-24 22:47:41.000000 unify-cli-3.2.1/source/hierarchy/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2474 2023-02-24 22:47:41.000000 unify-cli-3.2.1/source/hierarchy/commands.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-02-24 22:47:48.000000 unify-cli-3.2.1/source/org/
--rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2023-02-24 22:47:41.000000 unify-cli-3.2.1/source/org/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     4929 2023-02-24 22:47:41.000000 unify-cli-3.2.1/source/org/commands.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-02-24 22:47:48.000000 unify-cli-3.2.1/source/permissions/
--rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2023-02-24 22:47:41.000000 unify-cli-3.2.1/source/permissions/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2750 2023-02-24 22:47:41.000000 unify-cli-3.2.1/source/permissions/commands.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-02-24 22:47:48.000000 unify-cli-3.2.1/source/permissions/rules/
--rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2023-02-24 22:47:41.000000 unify-cli-3.2.1/source/permissions/rules/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     4854 2023-02-24 22:47:41.000000 unify-cli-3.2.1/source/permissions/rules/commands.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-02-24 22:47:48.000000 unify-cli-3.2.1/source/permissions/selectors/
--rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2023-02-24 22:47:41.000000 unify-cli-3.2.1/source/permissions/selectors/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2209 2023-02-24 22:47:41.000000 unify-cli-3.2.1/source/permissions/selectors/commands.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-02-24 22:47:48.000000 unify-cli-3.2.1/source/pipeline/
--rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2023-02-24 22:47:41.000000 unify-cli-3.2.1/source/pipeline/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1677 2023-02-24 22:47:41.000000 unify-cli-3.2.1/source/pipeline/commands.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-02-24 22:47:48.000000 unify-cli-3.2.1/source/template/
--rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2023-02-24 22:47:41.000000 unify-cli-3.2.1/source/template/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1281 2023-02-24 22:47:41.000000 unify-cli-3.2.1/source/template/commands.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-02-24 22:47:48.000000 unify-cli-3.2.1/source/user/
--rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2023-02-24 22:47:41.000000 unify-cli-3.2.1/source/user/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     5035 2023-02-24 22:47:41.000000 unify-cli-3.2.1/source/user/commands.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-02-24 22:47:48.000000 unify-cli-3.2.1/source/utils/
--rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2023-02-24 22:47:41.000000 unify-cli-3.2.1/source/utils/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      735 2023-02-24 22:47:41.000000 unify-cli-3.2.1/source/utils/util_methods.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-02-24 22:47:48.000000 unify-cli-3.2.1/source/workflow/
--rw-r--r--   0 circleci  (3434) circleci  (3434)        0 2023-02-24 22:47:41.000000 unify-cli-3.2.1/source/workflow/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     9700 2023-02-24 22:47:41.000000 unify-cli-3.2.1/source/workflow/commands.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-02-24 22:47:48.000000 unify-cli-3.2.1/tests/
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2289 2023-02-24 22:47:41.000000 unify-cli-3.2.1/tests/__init__.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1408 2023-02-24 22:47:41.000000 unify-cli-3.2.1/tests/properties.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2040 2023-02-24 22:47:41.000000 unify-cli-3.2.1/tests/test_asset_access.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3585 2023-02-24 22:47:41.000000 unify-cli-3.2.1/tests/test_cluster_command.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     4264 2023-02-24 22:47:41.000000 unify-cli-3.2.1/tests/test_datasets_commands.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2520 2023-02-24 22:47:41.000000 unify-cli-3.2.1/tests/test_graph_commands.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2292 2023-02-24 22:47:41.000000 unify-cli-3.2.1/tests/test_help.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)      209 2023-02-24 22:47:41.000000 unify-cli-3.2.1/tests/test_helper.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1462 2023-02-24 22:47:41.000000 unify-cli-3.2.1/tests/test_org_command.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     2536 2023-02-24 22:47:41.000000 unify-cli-3.2.1/tests/test_pipeline_commands.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1931 2023-02-24 22:47:41.000000 unify-cli-3.2.1/tests/test_templates_commands.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     3205 2023-02-24 22:47:41.000000 unify-cli-3.2.1/tests/test_user_commands.py
--rw-r--r--   0 circleci  (3434) circleci  (3434)     4061 2023-02-24 22:47:41.000000 unify-cli-3.2.1/tests/test_workflow_commands.py
-drwxr-xr-x   0 circleci  (3434) circleci  (3434)        0 2023-02-24 22:47:48.000000 unify-cli-3.2.1/unify_cli.egg-info/
--rw-r--r--   0 circleci  (3434) circleci  (3434)    10986 2023-02-24 22:47:48.000000 unify-cli-3.2.1/unify_cli.egg-info/PKG-INFO
--rw-r--r--   0 circleci  (3434) circleci  (3434)     1538 2023-02-24 22:47:48.000000 unify-cli-3.2.1/unify_cli.egg-info/SOURCES.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)        1 2023-02-24 22:47:48.000000 unify-cli-3.2.1/unify_cli.egg-info/dependency_links.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)       84 2023-02-24 22:47:48.000000 unify-cli-3.2.1/unify_cli.egg-info/entry_points.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)       34 2023-02-24 22:47:48.000000 unify-cli-3.2.1/unify_cli.egg-info/requires.txt
--rw-r--r--   0 circleci  (3434) circleci  (3434)       13 2023-02-24 22:47:48.000000 unify-cli-3.2.1/unify_cli.egg-info/top_level.txt
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-04 22:06:41.000000 unify-cli-3.4.1/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    11358 2023-05-04 22:06:15.000000 unify-cli-3.4.1/LICENSE
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    11718 2023-05-04 22:06:41.000000 unify-cli-3.4.1/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    11321 2023-05-04 22:06:15.000000 unify-cli-3.4.1/README.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       38 2023-05-04 22:06:41.000000 unify-cli-3.4.1/setup.cfg
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3218 2023-05-04 22:06:15.000000 unify-cli-3.4.1/setup.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-04 22:06:41.000000 unify-cli-3.4.1/source/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       34 2023-05-04 22:06:15.000000 unify-cli-3.4.1/source/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       33 2023-05-04 22:06:15.000000 unify-cli-3.4.1/source/_version.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-04 22:06:41.000000 unify-cli-3.4.1/source/access/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-05-04 22:06:15.000000 unify-cli-3.4.1/source/access/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2677 2023-05-04 22:06:15.000000 unify-cli-3.4.1/source/access/commands.py
+-rwxr-xr-x   0 circleci  (1001) circleci  (1002)     2293 2023-05-04 22:06:15.000000 unify-cli-3.4.1/source/ah.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-04 22:06:41.000000 unify-cli-3.4.1/source/cluster/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-05-04 22:06:15.000000 unify-cli-3.4.1/source/cluster/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3725 2023-05-04 22:06:15.000000 unify-cli-3.4.1/source/cluster/commands.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-04 22:06:41.000000 unify-cli-3.4.1/source/common/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-05-04 22:06:15.000000 unify-cli-3.4.1/source/common/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1124 2023-05-04 22:06:15.000000 unify-cli-3.4.1/source/common/commands.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-04 22:06:41.000000 unify-cli-3.4.1/source/dataset/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-05-04 22:06:15.000000 unify-cli-3.4.1/source/dataset/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4854 2023-05-04 22:06:15.000000 unify-cli-3.4.1/source/dataset/commands.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-04 22:06:41.000000 unify-cli-3.4.1/source/datastream/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-05-04 22:06:15.000000 unify-cli-3.4.1/source/datastream/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4429 2023-05-04 22:06:15.000000 unify-cli-3.4.1/source/datastream/commands.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)   485294 2023-05-04 22:06:15.000000 unify-cli-3.4.1/source/datastream/tags.csv
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-04 22:06:41.000000 unify-cli-3.4.1/source/graph/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-05-04 22:06:15.000000 unify-cli-3.4.1/source/graph/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2413 2023-05-04 22:06:15.000000 unify-cli-3.4.1/source/graph/commands.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-04 22:06:41.000000 unify-cli-3.4.1/source/hierarchy/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-05-04 22:06:15.000000 unify-cli-3.4.1/source/hierarchy/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2474 2023-05-04 22:06:15.000000 unify-cli-3.4.1/source/hierarchy/commands.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-04 22:06:41.000000 unify-cli-3.4.1/source/org/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-05-04 22:06:15.000000 unify-cli-3.4.1/source/org/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4929 2023-05-04 22:06:15.000000 unify-cli-3.4.1/source/org/commands.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-04 22:06:41.000000 unify-cli-3.4.1/source/permissions/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-05-04 22:06:15.000000 unify-cli-3.4.1/source/permissions/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2750 2023-05-04 22:06:15.000000 unify-cli-3.4.1/source/permissions/commands.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-04 22:06:41.000000 unify-cli-3.4.1/source/permissions/rules/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-05-04 22:06:15.000000 unify-cli-3.4.1/source/permissions/rules/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4854 2023-05-04 22:06:15.000000 unify-cli-3.4.1/source/permissions/rules/commands.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-04 22:06:41.000000 unify-cli-3.4.1/source/permissions/selectors/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-05-04 22:06:15.000000 unify-cli-3.4.1/source/permissions/selectors/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2209 2023-05-04 22:06:15.000000 unify-cli-3.4.1/source/permissions/selectors/commands.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-04 22:06:41.000000 unify-cli-3.4.1/source/pipeline/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-05-04 22:06:15.000000 unify-cli-3.4.1/source/pipeline/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1677 2023-05-04 22:06:15.000000 unify-cli-3.4.1/source/pipeline/commands.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-04 22:06:41.000000 unify-cli-3.4.1/source/template/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-05-04 22:06:15.000000 unify-cli-3.4.1/source/template/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1281 2023-05-04 22:06:15.000000 unify-cli-3.4.1/source/template/commands.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-04 22:06:41.000000 unify-cli-3.4.1/source/user/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-05-04 22:06:15.000000 unify-cli-3.4.1/source/user/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     9262 2023-05-04 22:06:15.000000 unify-cli-3.4.1/source/user/commands.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-04 22:06:41.000000 unify-cli-3.4.1/source/utils/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-05-04 22:06:15.000000 unify-cli-3.4.1/source/utils/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      735 2023-05-04 22:06:15.000000 unify-cli-3.4.1/source/utils/util_methods.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-04 22:06:41.000000 unify-cli-3.4.1/source/workflow/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        0 2023-05-04 22:06:15.000000 unify-cli-3.4.1/source/workflow/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     9700 2023-05-04 22:06:15.000000 unify-cli-3.4.1/source/workflow/commands.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-04 22:06:41.000000 unify-cli-3.4.1/tests/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2289 2023-05-04 22:06:15.000000 unify-cli-3.4.1/tests/__init__.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       19 2023-05-04 22:06:15.000000 unify-cli-3.4.1/tests/data_test.csv
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1408 2023-05-04 22:06:15.000000 unify-cli-3.4.1/tests/properties.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2040 2023-05-04 22:06:15.000000 unify-cli-3.4.1/tests/test_asset_access.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     3585 2023-05-04 22:06:15.000000 unify-cli-3.4.1/tests/test_cluster_command.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4264 2023-05-04 22:06:15.000000 unify-cli-3.4.1/tests/test_datasets_commands.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2520 2023-05-04 22:06:15.000000 unify-cli-3.4.1/tests/test_graph_commands.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2292 2023-05-04 22:06:15.000000 unify-cli-3.4.1/tests/test_help.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      209 2023-05-04 22:06:15.000000 unify-cli-3.4.1/tests/test_helper.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1462 2023-05-04 22:06:15.000000 unify-cli-3.4.1/tests/test_org_command.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     2536 2023-05-04 22:06:15.000000 unify-cli-3.4.1/tests/test_pipeline_commands.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1931 2023-05-04 22:06:15.000000 unify-cli-3.4.1/tests/test_templates_commands.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4049 2023-05-04 22:06:15.000000 unify-cli-3.4.1/tests/test_user_commands.py
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     4061 2023-05-04 22:06:15.000000 unify-cli-3.4.1/tests/test_workflow_commands.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-04 22:06:41.000000 unify-cli-3.4.1/unify_cli.egg-info/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    11718 2023-05-04 22:06:41.000000 unify-cli-3.4.1/unify_cli.egg-info/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1585 2023-05-04 22:06:41.000000 unify-cli-3.4.1/unify_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2023-05-04 22:06:41.000000 unify-cli-3.4.1/unify_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       59 2023-05-04 22:06:41.000000 unify-cli-3.4.1/unify_cli.egg-info/entry_points.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       34 2023-05-04 22:06:41.000000 unify-cli-3.4.1/unify_cli.egg-info/requires.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       13 2023-05-04 22:06:41.000000 unify-cli-3.4.1/unify_cli.egg-info/top_level.txt
```

### Comparing `unify-cli-3.2.1/LICENSE` & `unify-cli-3.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `unify-cli-3.2.1/PKG-INFO` & `unify-cli-3.4.1/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -1,22 +1,7 @@
-Metadata-Version: 2.1
-Name: unify-cli
-Version: 3.2.1
-Summary: Element Unify command line tool
-Home-page: https://github.com/ElementAnalytics/element-unify-cli
-Author: Element Analytics
-Author-email: platform@ean.io
-License: UNKNOWN
-Platform: UNKNOWN
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.7
-Requires-Python: >=3
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # Element Unify CLI
 
 The Unify CLI is a command line interface to Element Unify. It aims to supports all major APIs in Element Unify,
 and all common OSes (Mac, Windows, Linux). 
 
 It uses the command line tool library Click. https://click.palletsprojects.com/en/7.x/
 
@@ -318,8 +303,21 @@
   code_val=$(jq -r '.id' <<< "$jss")
   # Export each pipeline from the origin env and imported to the destination env
   unify wf export-pipeline --remote $ORIGIN_ENV --org $ORIGIN_ORG --pipeline $code_val --skip datasets --skip templates |  unify wf import-pipeline --remote $DESTINATION_ENV --org $DESTINATION_ORG --skip datasets --skip templates
 done
 
 ```
 
+# Developers Section
+
+Info for people developing against the CLI
+
+## Running the tests
+
+1. Initialize your virtual environment, either using virtualenv, pyenv & pyvenv-virtualenv, or however you have it set up.
+2. Install the test requirements: ``` pip install -r tests/requirements.txt ```
+3. Set the environment variables with cluster credentials (note, this should be a testing cluster for tests as it may not clean up after itself). These env var names may be edited in `tests/local.ini` if you like (don't check in the changes of course). Values for these can be found in 1password in the Engineering vault.
+    * LOCAL_API_URL
+    * LOCAL_ADMIN_NAME
+    * LOCAL_ADMIN_PASSWORD
+4. Run the tests: ``` nosetests --tc-file tests/local.ini --nocapture -v tests/ ```
```

### Comparing `unify-cli-3.2.1/README.md` & `unify-cli-3.4.1/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,7 +1,20 @@
+Metadata-Version: 2.1
+Name: unify-cli
+Version: 3.4.1
+Summary: Element Unify command line tool
+Home-page: https://github.com/ElementAnalytics/element-unify-cli
+Author: Element Analytics
+Author-email: platform@ean.io
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.7
+Requires-Python: >=3
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # Element Unify CLI
 
 The Unify CLI is a command line interface to Element Unify. It aims to supports all major APIs in Element Unify,
 and all common OSes (Mac, Windows, Linux). 
 
 It uses the command line tool library Click. https://click.palletsprojects.com/en/7.x/
 
@@ -302,7 +315,22 @@
 jq -c '.[]' <<< $PIPELINES | while read jss; do
   code_val=$(jq -r '.id' <<< "$jss")
   # Export each pipeline from the origin env and imported to the destination env
   unify wf export-pipeline --remote $ORIGIN_ENV --org $ORIGIN_ORG --pipeline $code_val --skip datasets --skip templates |  unify wf import-pipeline --remote $DESTINATION_ENV --org $DESTINATION_ORG --skip datasets --skip templates
 done
 
 ```
+
+# Developers Section
+
+Info for people developing against the CLI
+
+## Running the tests
+
+1. Initialize your virtual environment, either using virtualenv, pyenv & pyvenv-virtualenv, or however you have it set up.
+2. Install the test requirements: ``` pip install -r tests/requirements.txt ```
+3. Set the environment variables with cluster credentials (note, this should be a testing cluster for tests as it may not clean up after itself). These env var names may be edited in `tests/local.ini` if you like (don't check in the changes of course). Values for these can be found in 1password in the Engineering vault.
+    * LOCAL_API_URL
+    * LOCAL_ADMIN_NAME
+    * LOCAL_ADMIN_PASSWORD
+4. Run the tests: ``` nosetests --tc-file tests/local.ini --nocapture -v tests/ ```
+
```

### Comparing `unify-cli-3.2.1/source/access/commands.py` & `unify-cli-3.4.1/source/access/commands.py`

 * *Files identical despite different names*

### Comparing `unify-cli-3.2.1/source/ah.py` & `unify-cli-3.4.1/source/ah.py`

 * *Files identical despite different names*

### Comparing `unify-cli-3.2.1/source/cluster/commands.py` & `unify-cli-3.4.1/source/cluster/commands.py`

 * *Ordering differences only*

 * *Files 1% similar despite different names*

```diff
@@ -53,16 +53,16 @@
         )
 
     except Exception as err:
         click.echo(click.style(str(err), blink=False, bold=True, fg='red'))
 
 
 @cluster.command('login')
-@cluster_options
 @click.option('--display/--no-display', is_flag=True, default=False, show_default=True, help='Display the auth-token for the given remote')
+@cluster_options
 def login(remote, display):
 
     """
     Creates a auth token to the given cluster
     """
 
     try:
```

### Comparing `unify-cli-3.2.1/source/common/commands.py` & `unify-cli-3.4.1/source/common/commands.py`

 * *Files identical despite different names*

### Comparing `unify-cli-3.2.1/source/dataset/commands.py` & `unify-cli-3.4.1/source/dataset/commands.py`

 * *Files identical despite different names*

### Comparing `unify-cli-3.2.1/source/datastream/commands.py` & `unify-cli-3.4.1/source/datastream/commands.py`

 * *Files identical despite different names*

### Comparing `unify-cli-3.2.1/source/graph/commands.py` & `unify-cli-3.4.1/source/graph/commands.py`

 * *Files identical despite different names*

### Comparing `unify-cli-3.2.1/source/hierarchy/commands.py` & `unify-cli-3.4.1/source/hierarchy/commands.py`

 * *Files identical despite different names*

### Comparing `unify-cli-3.2.1/source/org/commands.py` & `unify-cli-3.4.1/source/org/commands.py`

 * *Files identical despite different names*

### Comparing `unify-cli-3.2.1/source/permissions/commands.py` & `unify-cli-3.4.1/source/permissions/commands.py`

 * *Files identical despite different names*

### Comparing `unify-cli-3.2.1/source/permissions/rules/commands.py` & `unify-cli-3.4.1/source/permissions/rules/commands.py`

 * *Files identical despite different names*

### Comparing `unify-cli-3.2.1/source/permissions/selectors/commands.py` & `unify-cli-3.4.1/source/permissions/selectors/commands.py`

 * *Files identical despite different names*

### Comparing `unify-cli-3.2.1/source/pipeline/commands.py` & `unify-cli-3.4.1/source/pipeline/commands.py`

 * *Files identical despite different names*

### Comparing `unify-cli-3.2.1/source/template/commands.py` & `unify-cli-3.4.1/source/template/commands.py`

 * *Files identical despite different names*

### Comparing `unify-cli-3.2.1/source/utils/util_methods.py` & `unify-cli-3.4.1/source/utils/util_methods.py`

 * *Files identical despite different names*

### Comparing `unify-cli-3.2.1/source/workflow/commands.py` & `unify-cli-3.4.1/source/workflow/commands.py`

 * *Files identical despite different names*

### Comparing `unify-cli-3.2.1/tests/__init__.py` & `unify-cli-3.4.1/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `unify-cli-3.2.1/tests/properties.py` & `unify-cli-3.4.1/tests/properties.py`

 * *Files identical despite different names*

### Comparing `unify-cli-3.2.1/tests/test_asset_access.py` & `unify-cli-3.4.1/tests/test_asset_access.py`

 * *Files identical despite different names*

### Comparing `unify-cli-3.2.1/tests/test_cluster_command.py` & `unify-cli-3.4.1/tests/test_cluster_command.py`

 * *Files identical despite different names*

### Comparing `unify-cli-3.2.1/tests/test_datasets_commands.py` & `unify-cli-3.4.1/tests/test_datasets_commands.py`

 * *Files identical despite different names*

### Comparing `unify-cli-3.2.1/tests/test_graph_commands.py` & `unify-cli-3.4.1/tests/test_graph_commands.py`

 * *Files identical despite different names*

### Comparing `unify-cli-3.2.1/tests/test_help.py` & `unify-cli-3.4.1/tests/test_help.py`

 * *Files identical despite different names*

### Comparing `unify-cli-3.2.1/tests/test_org_command.py` & `unify-cli-3.4.1/tests/test_org_command.py`

 * *Files identical despite different names*

### Comparing `unify-cli-3.2.1/tests/test_pipeline_commands.py` & `unify-cli-3.4.1/tests/test_pipeline_commands.py`

 * *Files identical despite different names*

### Comparing `unify-cli-3.2.1/tests/test_templates_commands.py` & `unify-cli-3.4.1/tests/test_templates_commands.py`

 * *Files identical despite different names*

### Comparing `unify-cli-3.2.1/tests/test_workflow_commands.py` & `unify-cli-3.4.1/tests/test_workflow_commands.py`

 * *Files identical despite different names*

### Comparing `unify-cli-3.2.1/unify_cli.egg-info/PKG-INFO` & `unify-cli-3.4.1/unify_cli.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 Metadata-Version: 2.1
 Name: unify-cli
-Version: 3.2.1
+Version: 3.4.1
 Summary: Element Unify command line tool
 Home-page: https://github.com/ElementAnalytics/element-unify-cli
 Author: Element Analytics
 Author-email: platform@ean.io
-License: UNKNOWN
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Requires-Python: >=3
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Element Unify CLI
@@ -318,8 +316,21 @@
   code_val=$(jq -r '.id' <<< "$jss")
   # Export each pipeline from the origin env and imported to the destination env
   unify wf export-pipeline --remote $ORIGIN_ENV --org $ORIGIN_ORG --pipeline $code_val --skip datasets --skip templates |  unify wf import-pipeline --remote $DESTINATION_ENV --org $DESTINATION_ORG --skip datasets --skip templates
 done
 
 ```
 
+# Developers Section
+
+Info for people developing against the CLI
+
+## Running the tests
+
+1. Initialize your virtual environment, either using virtualenv, pyenv & pyvenv-virtualenv, or however you have it set up.
+2. Install the test requirements: ``` pip install -r tests/requirements.txt ```
+3. Set the environment variables with cluster credentials (note, this should be a testing cluster for tests as it may not clean up after itself). These env var names may be edited in `tests/local.ini` if you like (don't check in the changes of course). Values for these can be found in 1password in the Engineering vault.
+    * LOCAL_API_URL
+    * LOCAL_ADMIN_NAME
+    * LOCAL_ADMIN_PASSWORD
+4. Run the tests: ``` nosetests --tc-file tests/local.ini --nocapture -v tests/ ```
```

### Comparing `unify-cli-3.2.1/unify_cli.egg-info/SOURCES.txt` & `unify-cli-3.4.1/unify_cli.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 source/cluster/commands.py
 source/common/__init__.py
 source/common/commands.py
 source/dataset/__init__.py
 source/dataset/commands.py
 source/datastream/__init__.py
 source/datastream/commands.py
+source/datastream/tags.csv
 source/graph/__init__.py
 source/graph/commands.py
 source/hierarchy/__init__.py
 source/hierarchy/commands.py
 source/org/__init__.py
 source/org/commands.py
 source/permissions/__init__.py
@@ -33,14 +34,15 @@
 source/user/__init__.py
 source/user/commands.py
 source/utils/__init__.py
 source/utils/util_methods.py
 source/workflow/__init__.py
 source/workflow/commands.py
 tests/__init__.py
+tests/data_test.csv
 tests/properties.py
 tests/test_asset_access.py
 tests/test_cluster_command.py
 tests/test_datasets_commands.py
 tests/test_graph_commands.py
 tests/test_help.py
 tests/test_helper.py
```

