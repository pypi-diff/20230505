# Comparing `tmp/gantry-0.6.1.tar.gz` & `tmp/gantry-0.6.2a0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gantry-0.6.1.tar", last modified: Thu May  4 00:44:45 2023, max compression
+gzip compressed data, was "gantry-0.6.2a0.tar", last modified: Fri May  5 19:27:41 2023, max compression
```

## Comparing `gantry-0.6.1.tar` & `gantry-0.6.2a0.tar`

### file list

```diff
@@ -1,161 +1,162 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 00:44:45.930754 gantry-0.6.1/
--rw-r--r--   0 runner    (1001) docker     (123)    10947 2023-05-04 00:44:30.000000 gantry-0.6.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-05-04 00:44:30.000000 gantry-0.6.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      613 2023-05-04 00:44:45.930754 gantry-0.6.1/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 00:44:45.890754 gantry-0.6.1/gantry/
--rw-r--r--   0 runner    (1001) docker     (123)     3779 2023-05-04 00:44:30.000000 gantry-0.6.1/gantry/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 00:44:45.894754 gantry-0.6.1/gantry/alerts/
--rw-r--r--   0 runner    (1001) docker     (123)      508 2023-05-04 00:44:30.000000 gantry-0.6.1/gantry/alerts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18599 2023-05-04 00:44:30.000000 gantry-0.6.1/gantry/alerts/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     1088 2023-05-04 00:44:30.000000 gantry-0.6.1/gantry/alerts/globals.py
--rw-r--r--   0 runner    (1001) docker     (123)     2374 2023-05-04 00:44:30.000000 gantry-0.6.1/gantry/alerts/main.py
--rw-r--r--   0 runner    (1001) docker     (123)     3464 2023-05-04 00:44:30.000000 gantry-0.6.1/gantry/api_client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 00:44:45.894754 gantry-0.6.1/gantry/applications/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 00:44:30.000000 gantry-0.6.1/gantry/applications/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2048 2023-05-04 00:44:30.000000 gantry-0.6.1/gantry/applications/client.py
--rw-r--r--   0 runner    (1001) docker     (123)    19486 2023-05-04 00:44:30.000000 gantry-0.6.1/gantry/applications/core.py
--rw-r--r--   0 runner    (1001) docker     (123)     1865 2023-05-04 00:44:30.000000 gantry-0.6.1/gantry/applications/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 00:44:45.898754 gantry-0.6.1/gantry/automations/
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-05-04 00:44:30.000000 gantry-0.6.1/gantry/automations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1842 2023-05-04 00:44:30.000000 gantry-0.6.1/gantry/automations/actions.py
--rw-r--r--   0 runner    (1001) docker     (123)     3878 2023-05-04 00:44:30.000000 gantry-0.6.1/gantry/automations/automations.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 00:44:45.898754 gantry-0.6.1/gantry/automations/curators/
--rw-r--r--   0 runner    (1001) docker     (123)      866 2023-05-04 00:44:30.000000 gantry-0.6.1/gantry/automations/curators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    23267 2023-05-04 00:44:30.000000 gantry-0.6.1/gantry/automations/curators/curators.py
--rw-r--r--   0 runner    (1001) docker     (123)      296 2023-05-04 00:44:30.000000 gantry-0.6.1/gantry/automations/curators/globals.py
--rw-r--r--   0 runner    (1001) docker     (123)     2982 2023-05-04 00:44:30.000000 gantry-0.6.1/gantry/automations/curators/main.py
--rw-r--r--   0 runner    (1001) docker     (123)     1435 2023-05-04 00:44:30.000000 gantry-0.6.1/gantry/automations/curators/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     7580 2023-05-04 00:44:30.000000 gantry-0.6.1/gantry/automations/curators/selectors.py
--rw-r--r--   0 runner    (1001) docker     (123)    26177 2023-05-04 00:44:30.000000 gantry-0.6.1/gantry/automations/curators/stock_curators.py
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-04 00:44:30.000000 gantry-0.6.1/gantry/automations/globals.py
--rw-r--r--   0 runner    (1001) docker     (123)      716 2023-05-04 00:44:30.000000 gantry-0.6.1/gantry/automations/main.py
--rw-r--r--   0 runner    (1001) docker     (123)     3952 2023-05-04 00:44:30.000000 gantry-0.6.1/gantry/automations/triggers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 00:44:45.902754 gantry-0.6.1/gantry/cli/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 00:44:30.000000 gantry-0.6.1/gantry/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1281 2023-05-04 00:44:30.000000 gantry-0.6.1/gantry/cli/application.py
--rw-r--r--   0 runner    (1001) docker     (123)     3012 2023-05-04 00:44:30.000000 gantry-0.6.1/gantry/cli/bucket.py
--rw-r--r--   0 runner    (1001) docker     (123)     6749 2023-05-04 00:44:30.000000 gantry-0.6.1/gantry/cli/data_connector.py
--rw-r--r--   0 runner    (1001) docker     (123)    18425 2023-05-04 00:44:30.000000 gantry-0.6.1/gantry/cli/labeling.py
--rw-r--r--   0 runner    (1001) docker     (123)     1254 2023-05-04 00:44:30.000000 gantry-0.6.1/gantry/cli/main.py
--rw-r--r--   0 runner    (1001) docker     (123)    12740 2023-05-04 00:44:30.000000 gantry-0.6.1/gantry/cli/projection.py
--rw-r--r--   0 runner    (1001) docker     (123)     2236 2023-05-04 00:44:30.000000 gantry-0.6.1/gantry/cli/secret.py
--rw-r--r--   0 runner    (1001) docker     (123)      158 2023-05-04 00:44:30.000000 gantry-0.6.1/gantry/const.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 00:44:45.902754 gantry-0.6.1/gantry/data_generator/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 00:44:30.000000 gantry-0.6.1/gantry/data_generator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4757 2023-05-04 00:44:30.000000 gantry-0.6.1/gantry/data_generator/data_generator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 00:44:45.906754 gantry-0.6.1/gantry/dataset/
--rw-r--r--   0 runner    (1001) docker     (123)      426 2023-05-04 00:44:30.000000 gantry-0.6.1/gantry/dataset/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10492 2023-05-04 00:44:30.000000 gantry-0.6.1/gantry/dataset/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     2476 2023-05-04 00:44:30.000000 gantry-0.6.1/gantry/dataset/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)    64417 2023-05-04 00:44:30.000000 gantry-0.6.1/gantry/dataset/gantry_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     3828 2023-05-04 00:44:30.000000 gantry-0.6.1/gantry/dataset/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 00:44:45.906754 gantry-0.6.1/gantry/dataset/templates/
--rw-r--r--   0 runner    (1001) docker     (123)     2802 2023-05-04 00:44:30.000000 gantry-0.6.1/gantry/dataset/templates/load_script_template.py.jinja
--rw-r--r--   0 runner    (1001) docker     (123)     4706 2023-05-04 00:44:30.000000 gantry-0.6.1/gantry/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 00:44:45.910754 gantry-0.6.1/gantry/logger/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 00:44:30.000000 gantry-0.6.1/gantry/logger/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    93572 2023-05-04 00:44:30.000000 gantry-0.6.1/gantry/logger/client.py
--rw-r--r--   0 runner    (1001) docker     (123)      621 2023-05-04 00:44:30.000000 gantry-0.6.1/gantry/logger/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     5151 2023-05-04 00:44:30.000000 gantry-0.6.1/gantry/logger/consumer.py
--rw-r--r--   0 runner    (1001) docker     (123)     6574 2023-05-04 00:44:30.000000 gantry-0.6.1/gantry/logger/event_builder.py
--rw-r--r--   0 runner    (1001) docker     (123)     6587 2023-05-04 00:44:30.000000 gantry-0.6.1/gantry/logger/main.py
--rw-r--r--   0 runner    (1001) docker     (123)     7908 2023-05-04 00:44:30.000000 gantry-0.6.1/gantry/logger/stores.py
--rw-r--r--   0 runner    (1001) docker     (123)     3775 2023-05-04 00:44:30.000000 gantry-0.6.1/gantry/logger/types.py
--rw-r--r--   0 runner    (1001) docker     (123)    11640 2023-05-04 00:44:30.000000 gantry-0.6.1/gantry/logger/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 00:44:45.910754 gantry-0.6.1/gantry/query/
--rw-r--r--   0 runner    (1001) docker     (123)      655 2023-05-04 00:44:30.000000 gantry-0.6.1/gantry/query/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17533 2023-05-04 00:44:30.000000 gantry-0.6.1/gantry/query/client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 00:44:45.910754 gantry-0.6.1/gantry/query/core/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 00:44:30.000000 gantry-0.6.1/gantry/query/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      217 2023-05-04 00:44:30.000000 gantry-0.6.1/gantry/query/core/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)    35580 2023-05-04 00:44:30.000000 gantry-0.6.1/gantry/query/core/dataframe.py
--rw-r--r--   0 runner    (1001) docker     (123)     3369 2023-05-04 00:44:30.000000 gantry-0.6.1/gantry/query/core/distance.py
--rw-r--r--   0 runner    (1001) docker     (123)    18555 2023-05-04 00:44:30.000000 gantry-0.6.1/gantry/query/core/metric.py
--rw-r--r--   0 runner    (1001) docker     (123)    10200 2023-05-04 00:44:30.000000 gantry-0.6.1/gantry/query/core/queryframe.py
--rw-r--r--   0 runner    (1001) docker     (123)     6211 2023-05-04 00:44:30.000000 gantry-0.6.1/gantry/query/core/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 00:44:45.914754 gantry-0.6.1/gantry/query/distance/
--rw-r--r--   0 runner    (1001) docker     (123)      129 2023-05-04 00:44:30.000000 gantry-0.6.1/gantry/query/distance/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      948 2023-05-04 00:44:30.000000 gantry-0.6.1/gantry/query/distance/main.py
--rw-r--r--   0 runner    (1001) docker     (123)     1510 2023-05-04 00:44:30.000000 gantry-0.6.1/gantry/query/globals.py
--rw-r--r--   0 runner    (1001) docker     (123)     3098 2023-05-04 00:44:30.000000 gantry-0.6.1/gantry/query/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 00:44:45.914754 gantry-0.6.1/gantry/query/metric/
--rw-r--r--   0 runner    (1001) docker     (123)      508 2023-05-04 00:44:30.000000 gantry-0.6.1/gantry/query/metric/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2521 2023-05-04 00:44:30.000000 gantry-0.6.1/gantry/query/metric/main.py
--rw-r--r--   0 runner    (1001) docker     (123)      851 2023-05-04 00:44:30.000000 gantry-0.6.1/gantry/query/time_window.py
--rw-r--r--   0 runner    (1001) docker     (123)     3313 2023-05-04 00:44:30.000000 gantry-0.6.1/gantry/serializers.py
--rw-r--r--   0 runner    (1001) docker     (123)     9704 2023-05-04 00:44:30.000000 gantry-0.6.1/gantry/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2687 2023-05-04 00:44:30.000000 gantry-0.6.1/gantry/validators.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-04 00:44:30.000000 gantry-0.6.1/gantry/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 00:44:45.894754 gantry-0.6.1/gantry.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      613 2023-05-04 00:44:45.000000 gantry-0.6.1/gantry.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3666 2023-05-04 00:44:45.000000 gantry-0.6.1/gantry.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-04 00:44:45.000000 gantry-0.6.1/gantry.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-05-04 00:44:45.000000 gantry-0.6.1/gantry.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      465 2023-05-04 00:44:45.000000 gantry-0.6.1/gantry.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-04 00:44:45.000000 gantry-0.6.1/gantry.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-04 00:44:45.930754 gantry-0.6.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1959 2023-05-04 00:44:30.000000 gantry-0.6.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 00:44:45.914754 gantry-0.6.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 00:44:30.000000 gantry-0.6.1/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 00:44:45.918754 gantry-0.6.1/tests/alerts/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 00:44:30.000000 gantry-0.6.1/tests/alerts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       36 2023-05-04 00:44:30.000000 gantry-0.6.1/tests/alerts/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)    13052 2023-05-04 00:44:30.000000 gantry-0.6.1/tests/alerts/test_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     5201 2023-05-04 00:44:30.000000 gantry-0.6.1/tests/alerts/test_main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 00:44:45.918754 gantry-0.6.1/tests/cli/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 00:44:30.000000 gantry-0.6.1/tests/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4275 2023-05-04 00:44:30.000000 gantry-0.6.1/tests/cli/test_bucket.py
--rw-r--r--   0 runner    (1001) docker     (123)    14561 2023-05-04 00:44:30.000000 gantry-0.6.1/tests/cli/test_data_connector.py
--rw-r--r--   0 runner    (1001) docker     (123)    21081 2023-05-04 00:44:30.000000 gantry-0.6.1/tests/cli/test_labeling.py
--rw-r--r--   0 runner    (1001) docker     (123)      178 2023-05-04 00:44:30.000000 gantry-0.6.1/tests/cli/test_main.py
--rw-r--r--   0 runner    (1001) docker     (123)     5094 2023-05-04 00:44:30.000000 gantry-0.6.1/tests/cli/test_projection.py
--rw-r--r--   0 runner    (1001) docker     (123)     3580 2023-05-04 00:44:30.000000 gantry-0.6.1/tests/cli/test_secrets.py
--rw-r--r--   0 runner    (1001) docker     (123)     4657 2023-05-04 00:44:30.000000 gantry-0.6.1/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 00:44:45.918754 gantry-0.6.1/tests/curator/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 00:44:30.000000 gantry-0.6.1/tests/curator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1720 2023-05-04 00:44:30.000000 gantry-0.6.1/tests/curator/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     7926 2023-05-04 00:44:30.000000 gantry-0.6.1/tests/curator/test_curator.py
--rw-r--r--   0 runner    (1001) docker     (123)     3113 2023-05-04 00:44:30.000000 gantry-0.6.1/tests/curator/test_main.py
--rw-r--r--   0 runner    (1001) docker     (123)     6680 2023-05-04 00:44:30.000000 gantry-0.6.1/tests/curator/test_selectors.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 00:44:45.922754 gantry-0.6.1/tests/data_generator/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 00:44:30.000000 gantry-0.6.1/tests/data_generator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1509 2023-05-04 00:44:30.000000 gantry-0.6.1/tests/data_generator/test_data_generator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 00:44:45.922754 gantry-0.6.1/tests/dataset/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 00:44:30.000000 gantry-0.6.1/tests/dataset/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2035 2023-05-04 00:44:30.000000 gantry-0.6.1/tests/dataset/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     5970 2023-05-04 00:44:30.000000 gantry-0.6.1/tests/dataset/test_client.py
--rw-r--r--   0 runner    (1001) docker     (123)    49536 2023-05-04 00:44:30.000000 gantry-0.6.1/tests/dataset/test_gantry_dataset.py
--rw-r--r--   0 runner    (1001) docker     (123)     2646 2023-05-04 00:44:30.000000 gantry-0.6.1/tests/dataset/test_main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 00:44:45.926754 gantry-0.6.1/tests/logger/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 00:44:30.000000 gantry-0.6.1/tests/logger/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      416 2023-05-04 00:44:30.000000 gantry-0.6.1/tests/logger/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)   136361 2023-05-04 00:44:30.000000 gantry-0.6.1/tests/logger/test_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     6395 2023-05-04 00:44:30.000000 gantry-0.6.1/tests/logger/test_consumer.py
--rw-r--r--   0 runner    (1001) docker     (123)     3919 2023-05-04 00:44:30.000000 gantry-0.6.1/tests/logger/test_event_builder.py
--rw-r--r--   0 runner    (1001) docker     (123)     7689 2023-05-04 00:44:30.000000 gantry-0.6.1/tests/logger/test_main.py
--rw-r--r--   0 runner    (1001) docker     (123)     9427 2023-05-04 00:44:30.000000 gantry-0.6.1/tests/logger/test_stores.py
--rw-r--r--   0 runner    (1001) docker     (123)    20087 2023-05-04 00:44:30.000000 gantry-0.6.1/tests/logger/test_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 00:44:45.926754 gantry-0.6.1/tests/query/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 00:44:30.000000 gantry-0.6.1/tests/query/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6538 2023-05-04 00:44:30.000000 gantry-0.6.1/tests/query/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 00:44:45.930754 gantry-0.6.1/tests/query/core/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 00:44:30.000000 gantry-0.6.1/tests/query/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    11716 2023-05-04 00:44:30.000000 gantry-0.6.1/tests/query/core/test_dataframe.py
--rw-r--r--   0 runner    (1001) docker     (123)     4610 2023-05-04 00:44:30.000000 gantry-0.6.1/tests/query/core/test_distance.py
--rw-r--r--   0 runner    (1001) docker     (123)      660 2023-05-04 00:44:30.000000 gantry-0.6.1/tests/query/core/test_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)    12594 2023-05-04 00:44:30.000000 gantry-0.6.1/tests/query/core/test_metric.py
--rw-r--r--   0 runner    (1001) docker     (123)    23434 2023-05-04 00:44:30.000000 gantry-0.6.1/tests/query/core/test_queryframe.py
--rw-r--r--   0 runner    (1001) docker     (123)    35405 2023-05-04 00:44:30.000000 gantry-0.6.1/tests/query/core/test_series.py
--rw-r--r--   0 runner    (1001) docker     (123)    12002 2023-05-04 00:44:30.000000 gantry-0.6.1/tests/query/core/test_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 00:44:45.930754 gantry-0.6.1/tests/query/distance/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 00:44:30.000000 gantry-0.6.1/tests/query/distance/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      626 2023-05-04 00:44:30.000000 gantry-0.6.1/tests/query/distance/test_main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 00:44:45.930754 gantry-0.6.1/tests/query/metric/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 00:44:30.000000 gantry-0.6.1/tests/query/metric/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2687 2023-05-04 00:44:30.000000 gantry-0.6.1/tests/query/metric/test_main.py
--rw-r--r--   0 runner    (1001) docker     (123)    15575 2023-05-04 00:44:30.000000 gantry-0.6.1/tests/query/test_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     3628 2023-05-04 00:44:30.000000 gantry-0.6.1/tests/query/test_main.py
--rw-r--r--   0 runner    (1001) docker     (123)     3840 2023-05-04 00:44:30.000000 gantry-0.6.1/tests/test_api_client.py
--rw-r--r--   0 runner    (1001) docker     (123)      665 2023-05-04 00:44:30.000000 gantry-0.6.1/tests/test_init.py
--rw-r--r--   0 runner    (1001) docker     (123)     2068 2023-05-04 00:44:30.000000 gantry-0.6.1/tests/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1641 2023-05-04 00:44:30.000000 gantry-0.6.1/tests/test_validator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 19:27:41.249697 gantry-0.6.2a0/
+-rw-r--r--   0 runner    (1001) docker     (123)    10947 2023-05-05 19:27:30.000000 gantry-0.6.2a0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-05-05 19:27:30.000000 gantry-0.6.2a0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      615 2023-05-05 19:27:41.249697 gantry-0.6.2a0/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 19:27:41.233697 gantry-0.6.2a0/gantry/
+-rw-r--r--   0 runner    (1001) docker     (123)     3770 2023-05-05 19:27:30.000000 gantry-0.6.2a0/gantry/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 19:27:41.233697 gantry-0.6.2a0/gantry/alerts/
+-rw-r--r--   0 runner    (1001) docker     (123)      508 2023-05-05 19:27:30.000000 gantry-0.6.2a0/gantry/alerts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18599 2023-05-05 19:27:30.000000 gantry-0.6.2a0/gantry/alerts/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1088 2023-05-05 19:27:30.000000 gantry-0.6.2a0/gantry/alerts/globals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2374 2023-05-05 19:27:30.000000 gantry-0.6.2a0/gantry/alerts/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3464 2023-05-05 19:27:30.000000 gantry-0.6.2a0/gantry/api_client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 19:27:41.233697 gantry-0.6.2a0/gantry/applications/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 19:27:30.000000 gantry-0.6.2a0/gantry/applications/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2945 2023-05-05 19:27:30.000000 gantry-0.6.2a0/gantry/applications/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19486 2023-05-05 19:27:30.000000 gantry-0.6.2a0/gantry/applications/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4321 2023-05-05 19:27:30.000000 gantry-0.6.2a0/gantry/applications/llm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1865 2023-05-05 19:27:30.000000 gantry-0.6.2a0/gantry/applications/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 19:27:41.237697 gantry-0.6.2a0/gantry/automations/
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-05-05 19:27:30.000000 gantry-0.6.2a0/gantry/automations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1842 2023-05-05 19:27:30.000000 gantry-0.6.2a0/gantry/automations/actions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3878 2023-05-05 19:27:30.000000 gantry-0.6.2a0/gantry/automations/automations.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 19:27:41.237697 gantry-0.6.2a0/gantry/automations/curators/
+-rw-r--r--   0 runner    (1001) docker     (123)      866 2023-05-05 19:27:30.000000 gantry-0.6.2a0/gantry/automations/curators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23267 2023-05-05 19:27:30.000000 gantry-0.6.2a0/gantry/automations/curators/curators.py
+-rw-r--r--   0 runner    (1001) docker     (123)      296 2023-05-05 19:27:30.000000 gantry-0.6.2a0/gantry/automations/curators/globals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2982 2023-05-05 19:27:30.000000 gantry-0.6.2a0/gantry/automations/curators/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1435 2023-05-05 19:27:30.000000 gantry-0.6.2a0/gantry/automations/curators/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7580 2023-05-05 19:27:30.000000 gantry-0.6.2a0/gantry/automations/curators/selectors.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26177 2023-05-05 19:27:30.000000 gantry-0.6.2a0/gantry/automations/curators/stock_curators.py
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-05 19:27:30.000000 gantry-0.6.2a0/gantry/automations/globals.py
+-rw-r--r--   0 runner    (1001) docker     (123)      716 2023-05-05 19:27:30.000000 gantry-0.6.2a0/gantry/automations/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3952 2023-05-05 19:27:30.000000 gantry-0.6.2a0/gantry/automations/triggers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 19:27:41.237697 gantry-0.6.2a0/gantry/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 19:27:30.000000 gantry-0.6.2a0/gantry/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1281 2023-05-05 19:27:30.000000 gantry-0.6.2a0/gantry/cli/application.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3012 2023-05-05 19:27:30.000000 gantry-0.6.2a0/gantry/cli/bucket.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6749 2023-05-05 19:27:30.000000 gantry-0.6.2a0/gantry/cli/data_connector.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18425 2023-05-05 19:27:30.000000 gantry-0.6.2a0/gantry/cli/labeling.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1254 2023-05-05 19:27:30.000000 gantry-0.6.2a0/gantry/cli/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12740 2023-05-05 19:27:30.000000 gantry-0.6.2a0/gantry/cli/projection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2236 2023-05-05 19:27:30.000000 gantry-0.6.2a0/gantry/cli/secret.py
+-rw-r--r--   0 runner    (1001) docker     (123)      158 2023-05-05 19:27:30.000000 gantry-0.6.2a0/gantry/const.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 19:27:41.237697 gantry-0.6.2a0/gantry/data_generator/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 19:27:30.000000 gantry-0.6.2a0/gantry/data_generator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4757 2023-05-05 19:27:30.000000 gantry-0.6.2a0/gantry/data_generator/data_generator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 19:27:41.237697 gantry-0.6.2a0/gantry/dataset/
+-rw-r--r--   0 runner    (1001) docker     (123)      426 2023-05-05 19:27:30.000000 gantry-0.6.2a0/gantry/dataset/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10492 2023-05-05 19:27:30.000000 gantry-0.6.2a0/gantry/dataset/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2476 2023-05-05 19:27:30.000000 gantry-0.6.2a0/gantry/dataset/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)    64417 2023-05-05 19:27:30.000000 gantry-0.6.2a0/gantry/dataset/gantry_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3828 2023-05-05 19:27:30.000000 gantry-0.6.2a0/gantry/dataset/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 19:27:41.237697 gantry-0.6.2a0/gantry/dataset/templates/
+-rw-r--r--   0 runner    (1001) docker     (123)     2802 2023-05-05 19:27:30.000000 gantry-0.6.2a0/gantry/dataset/templates/load_script_template.py.jinja
+-rw-r--r--   0 runner    (1001) docker     (123)     4706 2023-05-05 19:27:30.000000 gantry-0.6.2a0/gantry/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 19:27:41.241697 gantry-0.6.2a0/gantry/logger/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 19:27:30.000000 gantry-0.6.2a0/gantry/logger/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    93643 2023-05-05 19:27:30.000000 gantry-0.6.2a0/gantry/logger/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      621 2023-05-05 19:27:30.000000 gantry-0.6.2a0/gantry/logger/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5151 2023-05-05 19:27:30.000000 gantry-0.6.2a0/gantry/logger/consumer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6574 2023-05-05 19:27:30.000000 gantry-0.6.2a0/gantry/logger/event_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6587 2023-05-05 19:27:30.000000 gantry-0.6.2a0/gantry/logger/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7908 2023-05-05 19:27:30.000000 gantry-0.6.2a0/gantry/logger/stores.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3775 2023-05-05 19:27:30.000000 gantry-0.6.2a0/gantry/logger/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11640 2023-05-05 19:27:30.000000 gantry-0.6.2a0/gantry/logger/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 19:27:41.241697 gantry-0.6.2a0/gantry/query/
+-rw-r--r--   0 runner    (1001) docker     (123)      655 2023-05-05 19:27:30.000000 gantry-0.6.2a0/gantry/query/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17533 2023-05-05 19:27:30.000000 gantry-0.6.2a0/gantry/query/client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 19:27:41.241697 gantry-0.6.2a0/gantry/query/core/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 19:27:30.000000 gantry-0.6.2a0/gantry/query/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      217 2023-05-05 19:27:30.000000 gantry-0.6.2a0/gantry/query/core/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35580 2023-05-05 19:27:30.000000 gantry-0.6.2a0/gantry/query/core/dataframe.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3369 2023-05-05 19:27:30.000000 gantry-0.6.2a0/gantry/query/core/distance.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18555 2023-05-05 19:27:30.000000 gantry-0.6.2a0/gantry/query/core/metric.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10200 2023-05-05 19:27:30.000000 gantry-0.6.2a0/gantry/query/core/queryframe.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6211 2023-05-05 19:27:30.000000 gantry-0.6.2a0/gantry/query/core/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 19:27:41.241697 gantry-0.6.2a0/gantry/query/distance/
+-rw-r--r--   0 runner    (1001) docker     (123)      129 2023-05-05 19:27:30.000000 gantry-0.6.2a0/gantry/query/distance/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      948 2023-05-05 19:27:30.000000 gantry-0.6.2a0/gantry/query/distance/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1510 2023-05-05 19:27:30.000000 gantry-0.6.2a0/gantry/query/globals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3098 2023-05-05 19:27:30.000000 gantry-0.6.2a0/gantry/query/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 19:27:41.241697 gantry-0.6.2a0/gantry/query/metric/
+-rw-r--r--   0 runner    (1001) docker     (123)      508 2023-05-05 19:27:30.000000 gantry-0.6.2a0/gantry/query/metric/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2521 2023-05-05 19:27:30.000000 gantry-0.6.2a0/gantry/query/metric/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)      851 2023-05-05 19:27:30.000000 gantry-0.6.2a0/gantry/query/time_window.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3313 2023-05-05 19:27:30.000000 gantry-0.6.2a0/gantry/serializers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9704 2023-05-05 19:27:30.000000 gantry-0.6.2a0/gantry/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2687 2023-05-05 19:27:30.000000 gantry-0.6.2a0/gantry/validators.py
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-05-05 19:27:30.000000 gantry-0.6.2a0/gantry/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 19:27:41.233697 gantry-0.6.2a0/gantry.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      615 2023-05-05 19:27:41.000000 gantry-0.6.2a0/gantry.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3693 2023-05-05 19:27:41.000000 gantry-0.6.2a0/gantry.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 19:27:41.000000 gantry-0.6.2a0/gantry.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-05-05 19:27:41.000000 gantry-0.6.2a0/gantry.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      465 2023-05-05 19:27:41.000000 gantry-0.6.2a0/gantry.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-05 19:27:41.000000 gantry-0.6.2a0/gantry.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-05 19:27:41.249697 gantry-0.6.2a0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1959 2023-05-05 19:27:30.000000 gantry-0.6.2a0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 19:27:41.241697 gantry-0.6.2a0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 19:27:30.000000 gantry-0.6.2a0/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 19:27:41.245697 gantry-0.6.2a0/tests/alerts/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 19:27:30.000000 gantry-0.6.2a0/tests/alerts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       36 2023-05-05 19:27:30.000000 gantry-0.6.2a0/tests/alerts/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13052 2023-05-05 19:27:30.000000 gantry-0.6.2a0/tests/alerts/test_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5201 2023-05-05 19:27:30.000000 gantry-0.6.2a0/tests/alerts/test_main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 19:27:41.245697 gantry-0.6.2a0/tests/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 19:27:30.000000 gantry-0.6.2a0/tests/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4275 2023-05-05 19:27:30.000000 gantry-0.6.2a0/tests/cli/test_bucket.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14561 2023-05-05 19:27:30.000000 gantry-0.6.2a0/tests/cli/test_data_connector.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21081 2023-05-05 19:27:30.000000 gantry-0.6.2a0/tests/cli/test_labeling.py
+-rw-r--r--   0 runner    (1001) docker     (123)      178 2023-05-05 19:27:30.000000 gantry-0.6.2a0/tests/cli/test_main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5094 2023-05-05 19:27:30.000000 gantry-0.6.2a0/tests/cli/test_projection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3580 2023-05-05 19:27:30.000000 gantry-0.6.2a0/tests/cli/test_secrets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4657 2023-05-05 19:27:30.000000 gantry-0.6.2a0/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 19:27:41.245697 gantry-0.6.2a0/tests/curator/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 19:27:30.000000 gantry-0.6.2a0/tests/curator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1720 2023-05-05 19:27:30.000000 gantry-0.6.2a0/tests/curator/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7926 2023-05-05 19:27:30.000000 gantry-0.6.2a0/tests/curator/test_curator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3113 2023-05-05 19:27:30.000000 gantry-0.6.2a0/tests/curator/test_main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6680 2023-05-05 19:27:30.000000 gantry-0.6.2a0/tests/curator/test_selectors.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 19:27:41.245697 gantry-0.6.2a0/tests/data_generator/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 19:27:30.000000 gantry-0.6.2a0/tests/data_generator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1509 2023-05-05 19:27:30.000000 gantry-0.6.2a0/tests/data_generator/test_data_generator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 19:27:41.245697 gantry-0.6.2a0/tests/dataset/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 19:27:30.000000 gantry-0.6.2a0/tests/dataset/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2035 2023-05-05 19:27:30.000000 gantry-0.6.2a0/tests/dataset/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5970 2023-05-05 19:27:30.000000 gantry-0.6.2a0/tests/dataset/test_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    49536 2023-05-05 19:27:30.000000 gantry-0.6.2a0/tests/dataset/test_gantry_dataset.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2646 2023-05-05 19:27:30.000000 gantry-0.6.2a0/tests/dataset/test_main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 19:27:41.249697 gantry-0.6.2a0/tests/logger/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 19:27:30.000000 gantry-0.6.2a0/tests/logger/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      416 2023-05-05 19:27:30.000000 gantry-0.6.2a0/tests/logger/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)   136361 2023-05-05 19:27:30.000000 gantry-0.6.2a0/tests/logger/test_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6395 2023-05-05 19:27:30.000000 gantry-0.6.2a0/tests/logger/test_consumer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3919 2023-05-05 19:27:30.000000 gantry-0.6.2a0/tests/logger/test_event_builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7689 2023-05-05 19:27:30.000000 gantry-0.6.2a0/tests/logger/test_main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9427 2023-05-05 19:27:30.000000 gantry-0.6.2a0/tests/logger/test_stores.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20087 2023-05-05 19:27:30.000000 gantry-0.6.2a0/tests/logger/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 19:27:41.249697 gantry-0.6.2a0/tests/query/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 19:27:30.000000 gantry-0.6.2a0/tests/query/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6538 2023-05-05 19:27:30.000000 gantry-0.6.2a0/tests/query/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 19:27:41.249697 gantry-0.6.2a0/tests/query/core/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 19:27:30.000000 gantry-0.6.2a0/tests/query/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11716 2023-05-05 19:27:30.000000 gantry-0.6.2a0/tests/query/core/test_dataframe.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4610 2023-05-05 19:27:30.000000 gantry-0.6.2a0/tests/query/core/test_distance.py
+-rw-r--r--   0 runner    (1001) docker     (123)      660 2023-05-05 19:27:30.000000 gantry-0.6.2a0/tests/query/core/test_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12594 2023-05-05 19:27:30.000000 gantry-0.6.2a0/tests/query/core/test_metric.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23434 2023-05-05 19:27:30.000000 gantry-0.6.2a0/tests/query/core/test_queryframe.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35405 2023-05-05 19:27:30.000000 gantry-0.6.2a0/tests/query/core/test_series.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12002 2023-05-05 19:27:30.000000 gantry-0.6.2a0/tests/query/core/test_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 19:27:41.249697 gantry-0.6.2a0/tests/query/distance/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 19:27:30.000000 gantry-0.6.2a0/tests/query/distance/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      626 2023-05-05 19:27:30.000000 gantry-0.6.2a0/tests/query/distance/test_main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 19:27:41.249697 gantry-0.6.2a0/tests/query/metric/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 19:27:30.000000 gantry-0.6.2a0/tests/query/metric/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2687 2023-05-05 19:27:30.000000 gantry-0.6.2a0/tests/query/metric/test_main.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15575 2023-05-05 19:27:30.000000 gantry-0.6.2a0/tests/query/test_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3628 2023-05-05 19:27:30.000000 gantry-0.6.2a0/tests/query/test_main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3840 2023-05-05 19:27:30.000000 gantry-0.6.2a0/tests/test_api_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      665 2023-05-05 19:27:30.000000 gantry-0.6.2a0/tests/test_init.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2068 2023-05-05 19:27:30.000000 gantry-0.6.2a0/tests/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1641 2023-05-05 19:27:30.000000 gantry-0.6.2a0/tests/test_validator.py
```

### Comparing `gantry-0.6.1/LICENSE` & `gantry-0.6.2a0/LICENSE`

 * *Files identical despite different names*

### Comparing `gantry-0.6.1/PKG-INFO` & `gantry-0.6.2a0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gantry
-Version: 0.6.1
+Version: 0.6.2a0
 Summary: Gantry Python Library
 Author: Gantry Systems, Inc.
 Author-email: oss@gantry.io
 License: Apache Software License v2
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `gantry-0.6.1/gantry/__init__.py` & `gantry-0.6.2a0/gantry/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -12,15 +12,14 @@
 from gantry.automations.curators.main import _init as curators_init
 from gantry.automations.main import _init as automations_init
 from gantry.dataset.main import _init as dataset_init
 from gantry.logger.main import LOGGING_LEVEL_T
 from gantry.logger.main import _init as logger_init
 from gantry.logger.main import (
     get_client,
-    log,
     log_file,
     log_from_data_connector,
     log_record,
     log_records,
     ping,
     ready,
     setup_logger,
```

### Comparing `gantry-0.6.1/gantry/alerts/client.py` & `gantry-0.6.2a0/gantry/alerts/client.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.1/gantry/alerts/globals.py` & `gantry-0.6.2a0/gantry/alerts/globals.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.1/gantry/alerts/main.py` & `gantry-0.6.2a0/gantry/alerts/main.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.1/gantry/api_client.py` & `gantry-0.6.2a0/gantry/api_client.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.1/gantry/applications/core.py` & `gantry-0.6.2a0/gantry/applications/core.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.1/gantry/applications/main.py` & `gantry-0.6.2a0/gantry/applications/main.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.1/gantry/automations/actions.py` & `gantry-0.6.2a0/gantry/automations/actions.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.1/gantry/automations/automations.py` & `gantry-0.6.2a0/gantry/automations/automations.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.1/gantry/automations/curators/__init__.py` & `gantry-0.6.2a0/gantry/automations/curators/__init__.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.1/gantry/automations/curators/curators.py` & `gantry-0.6.2a0/gantry/automations/curators/curators.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.1/gantry/automations/curators/main.py` & `gantry-0.6.2a0/gantry/automations/curators/main.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.1/gantry/automations/curators/models.py` & `gantry-0.6.2a0/gantry/automations/curators/models.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.1/gantry/automations/curators/selectors.py` & `gantry-0.6.2a0/gantry/automations/curators/selectors.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.1/gantry/automations/curators/stock_curators.py` & `gantry-0.6.2a0/gantry/automations/curators/stock_curators.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.1/gantry/automations/main.py` & `gantry-0.6.2a0/gantry/automations/main.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.1/gantry/automations/triggers.py` & `gantry-0.6.2a0/gantry/automations/triggers.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.1/gantry/cli/application.py` & `gantry-0.6.2a0/gantry/cli/application.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.1/gantry/cli/bucket.py` & `gantry-0.6.2a0/gantry/cli/bucket.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.1/gantry/cli/data_connector.py` & `gantry-0.6.2a0/gantry/cli/data_connector.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.1/gantry/cli/labeling.py` & `gantry-0.6.2a0/gantry/cli/labeling.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.1/gantry/cli/main.py` & `gantry-0.6.2a0/gantry/cli/main.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.1/gantry/cli/projection.py` & `gantry-0.6.2a0/gantry/cli/projection.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.1/gantry/cli/secret.py` & `gantry-0.6.2a0/gantry/cli/secret.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.1/gantry/data_generator/data_generator.py` & `gantry-0.6.2a0/gantry/data_generator/data_generator.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.1/gantry/dataset/client.py` & `gantry-0.6.2a0/gantry/dataset/client.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.1/gantry/dataset/constants.py` & `gantry-0.6.2a0/gantry/dataset/constants.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.1/gantry/dataset/gantry_dataset.py` & `gantry-0.6.2a0/gantry/dataset/gantry_dataset.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.1/gantry/dataset/main.py` & `gantry-0.6.2a0/gantry/dataset/main.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.1/gantry/dataset/templates/load_script_template.py.jinja` & `gantry-0.6.2a0/gantry/dataset/templates/load_script_template.py.jinja`

 * *Files identical despite different names*

### Comparing `gantry-0.6.1/gantry/exceptions.py` & `gantry-0.6.2a0/gantry/exceptions.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.1/gantry/logger/client.py` & `gantry-0.6.2a0/gantry/logger/client.py`

 * *Files 1% similar despite different names*

```diff
@@ -519,16 +519,19 @@
                 i-th record. Alternatively, tags may be specified by passing in a DataFrame, Series,
                 or Array, like inputs.
 
                 For batch global tags, use the 'global_tags' parameter instead.
             global_tags (optional, Dict[str, str]): Specify a set of tags that will be attached to
                 all ingested records from this batch. For record specific tags, you can use
                 'row_tags' param. Only used when log is not called within a run.
-            run_id (optional, str): This should never be provided by user. It will be populated automatically when logging within a run to group records together.
-            run_tags (optional, Dict[str, str]): This should never be provided by user. It will be populated automatically when logging within a run to provide global tags for all records in the run.
+            run_id (optional, str): Specify a run_id to group records together.
+            run_tags (optional, Dict[str, str]): Specify a set of tags that will be attached to
+                all ingested records from this batch. For record specific tags, you can use
+                'row_tags' param. If not provided, we will use the global_tags value.
+                If run_tags is provided, it will override the global_tags value.
         """
         if run_id:
             # Generate records/events to be logged as part of the Run.
 
             # Check if inputs, outputs, feedbacks, timestamps, and join keys are singular.
             # If so, convert to list with one element.
             if isinstance(inputs, dict):
@@ -1200,15 +1203,14 @@
         """
         Function to record a batch of events containing predictions (inputs and outputs),
         feedback, or both simultaneously.
         To log predictions using this method, both inputs and outputs must be passed.
         To log feedbacks using this method, both join_keys and feedbacks must be passed.
 
         Example:
-
         .. code-block:: python
 
             gantry.log_records(
                 application='foobar',
                 inputs=[{'A': 100}, {'A': 101}],
                 outputs=[{'B': 'foo'}, {'B': 'bar'}],
                 version=1,
```

### Comparing `gantry-0.6.1/gantry/logger/constants.py` & `gantry-0.6.2a0/gantry/logger/constants.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.1/gantry/logger/consumer.py` & `gantry-0.6.2a0/gantry/logger/consumer.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.1/gantry/logger/event_builder.py` & `gantry-0.6.2a0/gantry/logger/event_builder.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.1/gantry/logger/main.py` & `gantry-0.6.2a0/gantry/logger/main.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.1/gantry/logger/stores.py` & `gantry-0.6.2a0/gantry/logger/stores.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.1/gantry/logger/types.py` & `gantry-0.6.2a0/gantry/logger/types.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.1/gantry/logger/utils.py` & `gantry-0.6.2a0/gantry/logger/utils.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.1/gantry/query/__init__.py` & `gantry-0.6.2a0/gantry/query/__init__.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.1/gantry/query/client.py` & `gantry-0.6.2a0/gantry/query/client.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.1/gantry/query/core/dataframe.py` & `gantry-0.6.2a0/gantry/query/core/dataframe.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.1/gantry/query/core/distance.py` & `gantry-0.6.2a0/gantry/query/core/distance.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.1/gantry/query/core/metric.py` & `gantry-0.6.2a0/gantry/query/core/metric.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.1/gantry/query/core/queryframe.py` & `gantry-0.6.2a0/gantry/query/core/queryframe.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.1/gantry/query/core/utils.py` & `gantry-0.6.2a0/gantry/query/core/utils.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.1/gantry/query/distance/main.py` & `gantry-0.6.2a0/gantry/query/distance/main.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.1/gantry/query/globals.py` & `gantry-0.6.2a0/gantry/query/globals.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.1/gantry/query/main.py` & `gantry-0.6.2a0/gantry/query/main.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.1/gantry/query/metric/main.py` & `gantry-0.6.2a0/gantry/query/metric/main.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.1/gantry/query/time_window.py` & `gantry-0.6.2a0/gantry/query/time_window.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.1/gantry/serializers.py` & `gantry-0.6.2a0/gantry/serializers.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.1/gantry/utils.py` & `gantry-0.6.2a0/gantry/utils.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.1/gantry/validators.py` & `gantry-0.6.2a0/gantry/validators.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.1/gantry.egg-info/PKG-INFO` & `gantry-0.6.2a0/gantry.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: gantry
-Version: 0.6.1
+Version: 0.6.2a0
 Summary: Gantry Python Library
 Author: Gantry Systems, Inc.
 Author-email: oss@gantry.io
 License: Apache Software License v2
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `gantry-0.6.1/gantry.egg-info/SOURCES.txt` & `gantry-0.6.2a0/gantry.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -18,14 +18,15 @@
 gantry/alerts/__init__.py
 gantry/alerts/client.py
 gantry/alerts/globals.py
 gantry/alerts/main.py
 gantry/applications/__init__.py
 gantry/applications/client.py
 gantry/applications/core.py
+gantry/applications/llm.py
 gantry/applications/main.py
 gantry/automations/__init__.py
 gantry/automations/actions.py
 gantry/automations/automations.py
 gantry/automations/globals.py
 gantry/automations/main.py
 gantry/automations/triggers.py
```

### Comparing `gantry-0.6.1/setup.py` & `gantry-0.6.2a0/setup.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.1/tests/alerts/test_client.py` & `gantry-0.6.2a0/tests/alerts/test_client.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.1/tests/alerts/test_main.py` & `gantry-0.6.2a0/tests/alerts/test_main.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.1/tests/cli/test_bucket.py` & `gantry-0.6.2a0/tests/cli/test_bucket.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.1/tests/cli/test_data_connector.py` & `gantry-0.6.2a0/tests/cli/test_data_connector.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.1/tests/cli/test_labeling.py` & `gantry-0.6.2a0/tests/cli/test_labeling.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.1/tests/cli/test_projection.py` & `gantry-0.6.2a0/tests/cli/test_projection.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.1/tests/cli/test_secrets.py` & `gantry-0.6.2a0/tests/cli/test_secrets.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.1/tests/conftest.py` & `gantry-0.6.2a0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.1/tests/curator/conftest.py` & `gantry-0.6.2a0/tests/curator/conftest.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.1/tests/curator/test_curator.py` & `gantry-0.6.2a0/tests/curator/test_curator.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.1/tests/curator/test_main.py` & `gantry-0.6.2a0/tests/curator/test_main.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.1/tests/curator/test_selectors.py` & `gantry-0.6.2a0/tests/curator/test_selectors.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.1/tests/data_generator/test_data_generator.py` & `gantry-0.6.2a0/tests/data_generator/test_data_generator.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.1/tests/dataset/conftest.py` & `gantry-0.6.2a0/tests/dataset/conftest.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.1/tests/dataset/test_client.py` & `gantry-0.6.2a0/tests/dataset/test_client.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.1/tests/dataset/test_gantry_dataset.py` & `gantry-0.6.2a0/tests/dataset/test_gantry_dataset.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.1/tests/dataset/test_main.py` & `gantry-0.6.2a0/tests/dataset/test_main.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.1/tests/logger/test_client.py` & `gantry-0.6.2a0/tests/logger/test_client.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.1/tests/logger/test_consumer.py` & `gantry-0.6.2a0/tests/logger/test_consumer.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.1/tests/logger/test_event_builder.py` & `gantry-0.6.2a0/tests/logger/test_event_builder.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.1/tests/logger/test_main.py` & `gantry-0.6.2a0/tests/logger/test_main.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.1/tests/logger/test_stores.py` & `gantry-0.6.2a0/tests/logger/test_stores.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.1/tests/logger/test_utils.py` & `gantry-0.6.2a0/tests/logger/test_utils.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.1/tests/query/conftest.py` & `gantry-0.6.2a0/tests/query/conftest.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.1/tests/query/core/test_dataframe.py` & `gantry-0.6.2a0/tests/query/core/test_dataframe.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.1/tests/query/core/test_distance.py` & `gantry-0.6.2a0/tests/query/core/test_distance.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.1/tests/query/core/test_filters.py` & `gantry-0.6.2a0/tests/query/core/test_filters.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.1/tests/query/core/test_metric.py` & `gantry-0.6.2a0/tests/query/core/test_metric.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.1/tests/query/core/test_queryframe.py` & `gantry-0.6.2a0/tests/query/core/test_queryframe.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.1/tests/query/core/test_series.py` & `gantry-0.6.2a0/tests/query/core/test_series.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.1/tests/query/core/test_utils.py` & `gantry-0.6.2a0/tests/query/core/test_utils.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.1/tests/query/distance/test_main.py` & `gantry-0.6.2a0/tests/query/distance/test_main.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.1/tests/query/metric/test_main.py` & `gantry-0.6.2a0/tests/query/metric/test_main.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.1/tests/query/test_client.py` & `gantry-0.6.2a0/tests/query/test_client.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.1/tests/query/test_main.py` & `gantry-0.6.2a0/tests/query/test_main.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.1/tests/test_api_client.py` & `gantry-0.6.2a0/tests/test_api_client.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.1/tests/test_init.py` & `gantry-0.6.2a0/tests/test_init.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.1/tests/test_utils.py` & `gantry-0.6.2a0/tests/test_utils.py`

 * *Files identical despite different names*

### Comparing `gantry-0.6.1/tests/test_validator.py` & `gantry-0.6.2a0/tests/test_validator.py`

 * *Files identical despite different names*

