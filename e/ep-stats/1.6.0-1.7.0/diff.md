# Comparing `tmp/ep-stats-1.6.0.tar.gz` & `tmp/ep-stats-1.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/ep-stats-1.6.0.tar", last modified: Fri Mar 17 09:39:34 2023, max compression
+gzip compressed data, was "dist/ep-stats-1.7.0.tar", last modified: Fri May  5 15:58:19 2023, max compression
```

## Comparing `ep-stats-1.6.0.tar` & `ep-stats-1.7.0.tar`

### file list

```diff
@@ -1,51 +1,51 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-17 09:39:34.000000 ep-stats-1.6.0/
--rw-r--r--   0 runner    (1001) docker     (123)     6417 2023-03-17 09:39:34.000000 ep-stats-1.6.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4786 2023-03-17 09:39:21.000000 ep-stats-1.6.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1602 2023-03-17 09:39:34.000000 ep-stats-1.6.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      396 2023-03-17 09:39:21.000000 ep-stats-1.6.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-17 09:39:34.000000 ep-stats-1.6.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-17 09:39:34.000000 ep-stats-1.6.0/src/ep_stats.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6417 2023-03-17 09:39:34.000000 ep-stats-1.6.0/src/ep_stats.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1461 2023-03-17 09:39:34.000000 ep-stats-1.6.0/src/ep_stats.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-17 09:39:34.000000 ep-stats-1.6.0/src/ep_stats.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-03-17 09:39:34.000000 ep-stats-1.6.0/src/ep_stats.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      464 2023-03-17 09:39:34.000000 ep-stats-1.6.0/src/ep_stats.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-03-17 09:39:34.000000 ep-stats-1.6.0/src/ep_stats.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-17 09:39:34.000000 ep-stats-1.6.0/src/epstats/
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-03-17 09:39:21.000000 ep-stats-1.6.0/src/epstats/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       31 2023-03-17 09:39:21.000000 ep-stats-1.6.0/src/epstats/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      751 2023-03-17 09:39:21.000000 ep-stats-1.6.0/src/epstats/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1156 2023-03-17 09:39:21.000000 ep-stats-1.6.0/src/epstats/locust.py
--rw-r--r--   0 runner    (1001) docker     (123)     1333 2023-03-17 09:39:21.000000 ep-stats-1.6.0/src/epstats/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-17 09:39:34.000000 ep-stats-1.6.0/src/epstats/server/
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-03-17 09:39:21.000000 ep-stats-1.6.0/src/epstats/server/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2724 2023-03-17 09:39:21.000000 ep-stats-1.6.0/src/epstats/server/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     2525 2023-03-17 09:39:21.000000 ep-stats-1.6.0/src/epstats/server/api_evaluate.py
--rw-r--r--   0 runner    (1001) docker     (123)     2031 2023-03-17 09:39:21.000000 ep-stats-1.6.0/src/epstats/server/api_sample_size_calculation.py
--rw-r--r--   0 runner    (1001) docker     (123)      412 2023-03-17 09:39:21.000000 ep-stats-1.6.0/src/epstats/server/api_settings.py
--rw-r--r--   0 runner    (1001) docker     (123)      401 2023-03-17 09:39:21.000000 ep-stats-1.6.0/src/epstats/server/json_response.py
--rw-r--r--   0 runner    (1001) docker     (123)    15192 2023-03-17 09:39:21.000000 ep-stats-1.6.0/src/epstats/server/req.py
--rw-r--r--   0 runner    (1001) docker     (123)    10339 2023-03-17 09:39:21.000000 ep-stats-1.6.0/src/epstats/server/res.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-17 09:39:34.000000 ep-stats-1.6.0/src/epstats/toolkit/
--rw-r--r--   0 runner    (1001) docker     (123)      319 2023-03-17 09:39:21.000000 ep-stats-1.6.0/src/epstats/toolkit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9542 2023-03-17 09:39:21.000000 ep-stats-1.6.0/src/epstats/toolkit/check.py
--rw-r--r--   0 runner    (1001) docker     (123)     1475 2023-03-17 09:39:21.000000 ep-stats-1.6.0/src/epstats/toolkit/dao.py
--rw-r--r--   0 runner    (1001) docker     (123)    31433 2023-03-17 09:39:21.000000 ep-stats-1.6.0/src/epstats/toolkit/experiment.py
--rw-r--r--   0 runner    (1001) docker     (123)     4993 2023-03-17 09:39:21.000000 ep-stats-1.6.0/src/epstats/toolkit/metric.py
--rw-r--r--   0 runner    (1001) docker     (123)    13518 2023-03-17 09:39:21.000000 ep-stats-1.6.0/src/epstats/toolkit/parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     4538 2023-03-17 09:39:21.000000 ep-stats-1.6.0/src/epstats/toolkit/results.py
--rw-r--r--   0 runner    (1001) docker     (123)    15215 2023-03-17 09:39:21.000000 ep-stats-1.6.0/src/epstats/toolkit/statistics.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-17 09:39:34.000000 ep-stats-1.6.0/src/epstats/toolkit/testing/
--rw-r--r--   0 runner    (1001) docker     (123)      303 2023-03-17 09:39:21.000000 ep-stats-1.6.0/src/epstats/toolkit/testing/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-17 09:39:34.000000 ep-stats-1.6.0/src/epstats/toolkit/testing/resources/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-17 09:39:21.000000 ep-stats-1.6.0/src/epstats/toolkit/testing/resources/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3366 2023-03-17 09:39:21.000000 ep-stats-1.6.0/src/epstats/toolkit/testing/resources/evaluations_checks.csv
--rw-r--r--   0 runner    (1001) docker     (123)     3730 2023-03-17 09:39:21.000000 ep-stats-1.6.0/src/epstats/toolkit/testing/resources/evaluations_exposures.csv
--rw-r--r--   0 runner    (1001) docker     (123)    13734 2023-03-17 09:39:21.000000 ep-stats-1.6.0/src/epstats/toolkit/testing/resources/evaluations_metrics.csv
--rw-r--r--   0 runner    (1001) docker     (123)    13894 2023-03-17 09:39:21.000000 ep-stats-1.6.0/src/epstats/toolkit/testing/resources/goals_agg.csv
--rw-r--r--   0 runner    (1001) docker     (123)     4429 2023-03-17 09:39:21.000000 ep-stats-1.6.0/src/epstats/toolkit/testing/resources/goals_by_unit.csv
--rw-r--r--   0 runner    (1001) docker     (123)      168 2023-03-17 09:39:21.000000 ep-stats-1.6.0/src/epstats/toolkit/testing/resources/goals_simple_agg.csv
--rw-r--r--   0 runner    (1001) docker     (123)     2962 2023-03-17 09:39:21.000000 ep-stats-1.6.0/src/epstats/toolkit/testing/test_dao.py
--rw-r--r--   0 runner    (1001) docker     (123)     3947 2023-03-17 09:39:21.000000 ep-stats-1.6.0/src/epstats/toolkit/testing/test_data.py
--rw-r--r--   0 runner    (1001) docker     (123)     5057 2023-03-17 09:39:21.000000 ep-stats-1.6.0/src/epstats/toolkit/testing/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     2831 2023-03-17 09:39:21.000000 ep-stats-1.6.0/src/epstats/toolkit/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 15:58:19.000000 ep-stats-1.7.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     6417 2023-05-05 15:58:19.000000 ep-stats-1.7.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4786 2023-05-05 15:58:05.000000 ep-stats-1.7.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1602 2023-05-05 15:58:19.000000 ep-stats-1.7.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      396 2023-05-05 15:58:05.000000 ep-stats-1.7.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 15:58:19.000000 ep-stats-1.7.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 15:58:19.000000 ep-stats-1.7.0/src/ep_stats.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6417 2023-05-05 15:58:19.000000 ep-stats-1.7.0/src/ep_stats.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1461 2023-05-05 15:58:19.000000 ep-stats-1.7.0/src/ep_stats.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 15:58:19.000000 ep-stats-1.7.0/src/ep_stats.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-05-05 15:58:19.000000 ep-stats-1.7.0/src/ep_stats.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      464 2023-05-05 15:58:19.000000 ep-stats-1.7.0/src/ep_stats.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-05 15:58:19.000000 ep-stats-1.7.0/src/ep_stats.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 15:58:19.000000 ep-stats-1.7.0/src/epstats/
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-05 15:58:05.000000 ep-stats-1.7.0/src/epstats/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       31 2023-05-05 15:58:05.000000 ep-stats-1.7.0/src/epstats/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      751 2023-05-05 15:58:05.000000 ep-stats-1.7.0/src/epstats/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1156 2023-05-05 15:58:05.000000 ep-stats-1.7.0/src/epstats/locust.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1333 2023-05-05 15:58:05.000000 ep-stats-1.7.0/src/epstats/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 15:58:19.000000 ep-stats-1.7.0/src/epstats/server/
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-05-05 15:58:05.000000 ep-stats-1.7.0/src/epstats/server/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2724 2023-05-05 15:58:05.000000 ep-stats-1.7.0/src/epstats/server/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2525 2023-05-05 15:58:05.000000 ep-stats-1.7.0/src/epstats/server/api_evaluate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2031 2023-05-05 15:58:05.000000 ep-stats-1.7.0/src/epstats/server/api_sample_size_calculation.py
+-rw-r--r--   0 runner    (1001) docker     (123)      412 2023-05-05 15:58:05.000000 ep-stats-1.7.0/src/epstats/server/api_settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)      401 2023-05-05 15:58:05.000000 ep-stats-1.7.0/src/epstats/server/json_response.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15192 2023-05-05 15:58:05.000000 ep-stats-1.7.0/src/epstats/server/req.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10339 2023-05-05 15:58:05.000000 ep-stats-1.7.0/src/epstats/server/res.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 15:58:19.000000 ep-stats-1.7.0/src/epstats/toolkit/
+-rw-r--r--   0 runner    (1001) docker     (123)      319 2023-05-05 15:58:05.000000 ep-stats-1.7.0/src/epstats/toolkit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9542 2023-05-05 15:58:05.000000 ep-stats-1.7.0/src/epstats/toolkit/check.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1475 2023-05-05 15:58:05.000000 ep-stats-1.7.0/src/epstats/toolkit/dao.py
+-rw-r--r--   0 runner    (1001) docker     (123)    31433 2023-05-05 15:58:05.000000 ep-stats-1.7.0/src/epstats/toolkit/experiment.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4993 2023-05-05 15:58:05.000000 ep-stats-1.7.0/src/epstats/toolkit/metric.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13803 2023-05-05 15:58:05.000000 ep-stats-1.7.0/src/epstats/toolkit/parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4538 2023-05-05 15:58:05.000000 ep-stats-1.7.0/src/epstats/toolkit/results.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15215 2023-05-05 15:58:05.000000 ep-stats-1.7.0/src/epstats/toolkit/statistics.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 15:58:19.000000 ep-stats-1.7.0/src/epstats/toolkit/testing/
+-rw-r--r--   0 runner    (1001) docker     (123)      303 2023-05-05 15:58:05.000000 ep-stats-1.7.0/src/epstats/toolkit/testing/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 15:58:19.000000 ep-stats-1.7.0/src/epstats/toolkit/testing/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 15:58:05.000000 ep-stats-1.7.0/src/epstats/toolkit/testing/resources/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3366 2023-05-05 15:58:05.000000 ep-stats-1.7.0/src/epstats/toolkit/testing/resources/evaluations_checks.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     3730 2023-05-05 15:58:05.000000 ep-stats-1.7.0/src/epstats/toolkit/testing/resources/evaluations_exposures.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    13734 2023-05-05 15:58:05.000000 ep-stats-1.7.0/src/epstats/toolkit/testing/resources/evaluations_metrics.csv
+-rw-r--r--   0 runner    (1001) docker     (123)    13894 2023-05-05 15:58:05.000000 ep-stats-1.7.0/src/epstats/toolkit/testing/resources/goals_agg.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     4429 2023-05-05 15:58:05.000000 ep-stats-1.7.0/src/epstats/toolkit/testing/resources/goals_by_unit.csv
+-rw-r--r--   0 runner    (1001) docker     (123)      168 2023-05-05 15:58:05.000000 ep-stats-1.7.0/src/epstats/toolkit/testing/resources/goals_simple_agg.csv
+-rw-r--r--   0 runner    (1001) docker     (123)     2962 2023-05-05 15:58:05.000000 ep-stats-1.7.0/src/epstats/toolkit/testing/test_dao.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3947 2023-05-05 15:58:05.000000 ep-stats-1.7.0/src/epstats/toolkit/testing/test_data.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5057 2023-05-05 15:58:05.000000 ep-stats-1.7.0/src/epstats/toolkit/testing/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2831 2023-05-05 15:58:05.000000 ep-stats-1.7.0/src/epstats/toolkit/utils.py
```

### Comparing `ep-stats-1.6.0/PKG-INFO` & `ep-stats-1.7.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ep-stats
-Version: 1.6.0
+Version: 1.7.0
 Summary: Statistical package to evaluate ab tests in experimentation platform.
 Home-page: https://github.com/avast/ep-stats
 Author: Ondrej Zahradnik
 Author-email: ondrej.zahradnik@avast.com
 License: UNKNOWN
 Description: ![](https://img.shields.io/github/workflow/status/avast/ep-stats/Code%20Checks?color=green)
         [![PyPI version](https://img.shields.io/pypi/v/ep-stats?color=green)](https://pypi.org/project/ep-stats/)
```

### Comparing `ep-stats-1.6.0/README.md` & `ep-stats-1.7.0/README.md`

 * *Files identical despite different names*

### Comparing `ep-stats-1.6.0/setup.cfg` & `ep-stats-1.7.0/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = ep-stats
-version = 1.6.0
+version = 1.7.0
 description = Statistical package to evaluate ab tests in experimentation platform.
 long_description = file: README.md
 long_description_content_type = text/markdown
 author = Ondrej Zahradnik
 author_email = ondrej.zahradnik@avast.com
 url = https://github.com/avast/ep-stats
 classifiers =
```

### Comparing `ep-stats-1.6.0/src/ep_stats.egg-info/PKG-INFO` & `ep-stats-1.7.0/src/ep_stats.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ep-stats
-Version: 1.6.0
+Version: 1.7.0
 Summary: Statistical package to evaluate ab tests in experimentation platform.
 Home-page: https://github.com/avast/ep-stats
 Author: Ondrej Zahradnik
 Author-email: ondrej.zahradnik@avast.com
 License: UNKNOWN
 Description: ![](https://img.shields.io/github/workflow/status/avast/ep-stats/Code%20Checks?color=green)
         [![PyPI version](https://img.shields.io/pypi/v/ep-stats?color=green)](https://pypi.org/project/ep-stats/)
```

### Comparing `ep-stats-1.6.0/src/ep_stats.egg-info/SOURCES.txt` & `ep-stats-1.7.0/src/ep_stats.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ep-stats-1.6.0/src/epstats/config.py` & `ep-stats-1.7.0/src/epstats/config.py`

 * *Files identical despite different names*

### Comparing `ep-stats-1.6.0/src/epstats/locust.py` & `ep-stats-1.7.0/src/epstats/locust.py`

 * *Files identical despite different names*

### Comparing `ep-stats-1.6.0/src/epstats/main.py` & `ep-stats-1.7.0/src/epstats/main.py`

 * *Files identical despite different names*

### Comparing `ep-stats-1.6.0/src/epstats/server/api.py` & `ep-stats-1.7.0/src/epstats/server/api.py`

 * *Files identical despite different names*

### Comparing `ep-stats-1.6.0/src/epstats/server/api_evaluate.py` & `ep-stats-1.7.0/src/epstats/server/api_evaluate.py`

 * *Files identical despite different names*

### Comparing `ep-stats-1.6.0/src/epstats/server/api_sample_size_calculation.py` & `ep-stats-1.7.0/src/epstats/server/api_sample_size_calculation.py`

 * *Files identical despite different names*

### Comparing `ep-stats-1.6.0/src/epstats/server/req.py` & `ep-stats-1.7.0/src/epstats/server/req.py`

 * *Files identical despite different names*

### Comparing `ep-stats-1.6.0/src/epstats/server/res.py` & `ep-stats-1.7.0/src/epstats/server/res.py`

 * *Files identical despite different names*

### Comparing `ep-stats-1.6.0/src/epstats/toolkit/check.py` & `ep-stats-1.7.0/src/epstats/toolkit/check.py`

 * *Files identical despite different names*

### Comparing `ep-stats-1.6.0/src/epstats/toolkit/dao.py` & `ep-stats-1.7.0/src/epstats/toolkit/dao.py`

 * *Files identical despite different names*

### Comparing `ep-stats-1.6.0/src/epstats/toolkit/experiment.py` & `ep-stats-1.7.0/src/epstats/toolkit/experiment.py`

 * *Files identical despite different names*

### Comparing `ep-stats-1.6.0/src/epstats/toolkit/metric.py` & `ep-stats-1.7.0/src/epstats/toolkit/metric.py`

 * *Files identical despite different names*

### Comparing `ep-stats-1.6.0/src/epstats/toolkit/parser.py` & `ep-stats-1.7.0/src/epstats/toolkit/parser.py`

 * *Files 4% similar despite different names*

```diff
@@ -23,15 +23,20 @@
     def __init__(self, nominator: str, denominator: str):
         func = Word(alphas)
         unit_type = Word(alphas + "_").setParseAction(UnitType)
         agg_type = Word(alphas).setParseAction(AggType)
         goal = Word(alphas + "_" + nums).setParseAction(Goal)
         number = Word(nums).setParseAction(Number)
         dimension = Word(alphas + "_").setParseAction(Dimension)
-        dimension_value = Word(alphanums + "_" + "-" + "." + "%" + " " + "/" + "|").setParseAction(DimensionValue)
+        dimension_value_chars = alphanums + "_" + "-" + "." + "%" + " " + "/" + "|"
+        # we allow either `dimension=dimension_value` or `dimension=^dimension_value`
+        dimension_value = (Word(dimension_value_chars) | ("^" + Word(dimension_value_chars))).setParseAction(
+            DimensionValue
+        )
+
         dimension_list = delimitedList(dimension + "=" + dimension_value)
 
         ep_goal = (func + "(" + unit_type + "." + agg_type + "." + goal + ")").setParseAction(EpGoal)
         ep_goal_with_dimensions = (
             func + "(" + unit_type + "." + agg_type + "." + goal + "(" + dimension_list + ")" + ")"
         ).setParseAction(EpGoal)
         operand = number | ep_goal | ep_goal_with_dimensions
@@ -176,15 +181,16 @@
         return self.dimension
 
     __repr__ = __str__
 
 
 class DimensionValue:
     def __init__(self, t):
-        self.dimension_value = t[0]
+        # if the hat operator is present, we need to join it with the value
+        self.dimension_value = "".join(t)
 
     def __str__(self):
         return self.dimension_value
 
     __repr__ = __str__
```

### Comparing `ep-stats-1.6.0/src/epstats/toolkit/results.py` & `ep-stats-1.7.0/src/epstats/toolkit/results.py`

 * *Files identical despite different names*

### Comparing `ep-stats-1.6.0/src/epstats/toolkit/statistics.py` & `ep-stats-1.7.0/src/epstats/toolkit/statistics.py`

 * *Files identical despite different names*

### Comparing `ep-stats-1.6.0/src/epstats/toolkit/testing/resources/evaluations_checks.csv` & `ep-stats-1.7.0/src/epstats/toolkit/testing/resources/evaluations_checks.csv`

 * *Files identical despite different names*

### Comparing `ep-stats-1.6.0/src/epstats/toolkit/testing/resources/evaluations_exposures.csv` & `ep-stats-1.7.0/src/epstats/toolkit/testing/resources/evaluations_exposures.csv`

 * *Files identical despite different names*

### Comparing `ep-stats-1.6.0/src/epstats/toolkit/testing/resources/evaluations_metrics.csv` & `ep-stats-1.7.0/src/epstats/toolkit/testing/resources/evaluations_metrics.csv`

 * *Files identical despite different names*

### Comparing `ep-stats-1.6.0/src/epstats/toolkit/testing/resources/goals_agg.csv` & `ep-stats-1.7.0/src/epstats/toolkit/testing/resources/goals_agg.csv`

 * *Files identical despite different names*

### Comparing `ep-stats-1.6.0/src/epstats/toolkit/testing/resources/goals_by_unit.csv` & `ep-stats-1.7.0/src/epstats/toolkit/testing/resources/goals_by_unit.csv`

 * *Files identical despite different names*

### Comparing `ep-stats-1.6.0/src/epstats/toolkit/testing/test_dao.py` & `ep-stats-1.7.0/src/epstats/toolkit/testing/test_dao.py`

 * *Files identical despite different names*

### Comparing `ep-stats-1.6.0/src/epstats/toolkit/testing/test_data.py` & `ep-stats-1.7.0/src/epstats/toolkit/testing/test_data.py`

 * *Files identical despite different names*

### Comparing `ep-stats-1.6.0/src/epstats/toolkit/testing/utils.py` & `ep-stats-1.7.0/src/epstats/toolkit/testing/utils.py`

 * *Files identical despite different names*

### Comparing `ep-stats-1.6.0/src/epstats/toolkit/utils.py` & `ep-stats-1.7.0/src/epstats/toolkit/utils.py`

 * *Files identical despite different names*

