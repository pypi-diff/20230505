# Comparing `tmp/dspace_stats_collector-0.6.8.tar.gz` & `tmp/dspace_stats_collector-0.6.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dspace_stats_collector-0.6.8.tar", last modified: Fri May  5 13:41:14 2023, max compression
+gzip compressed data, was "dspace_stats_collector-0.6.9.tar", last modified: Fri May  5 15:15:55 2023, max compression
```

## Comparing `dspace_stats_collector-0.6.8.tar` & `dspace_stats_collector-0.6.9.tar`

### file list

```diff
@@ -1,78 +1,78 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 13:41:14.463250 dspace_stats_collector-0.6.8/
--rw-r--r--   0 runner    (1001) docker     (123)      364 2023-05-05 13:41:01.000000 dspace_stats_collector-0.6.8/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3713 2023-05-05 13:41:01.000000 dspace_stats_collector-0.6.8/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-05-05 13:41:01.000000 dspace_stats_collector-0.6.8/HISTORY.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1565 2023-05-05 13:41:01.000000 dspace_stats_collector-0.6.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      289 2023-05-05 13:41:01.000000 dspace_stats_collector-0.6.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     6046 2023-05-05 13:41:14.463250 dspace_stats_collector-0.6.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5246 2023-05-05 13:41:01.000000 dspace_stats_collector-0.6.8/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 13:41:14.451250 dspace_stats_collector-0.6.8/config/
--rw-r--r--   0 runner    (1001) docker     (123)    23785 2023-05-05 13:41:01.000000 dspace_stats_collector-0.6.8/config/COUNTER_Robots_list.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 13:41:14.455250 dspace_stats_collector-0.6.8/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      623 2023-05-05 13:41:01.000000 dspace_stats_collector-0.6.8/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)     4316 2023-05-05 13:41:01.000000 dspace_stats_collector-0.6.8/docs/README_BR.rst
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-05-05 13:41:01.000000 dspace_stats_collector-0.6.8/docs/authors.rst
--rw-r--r--   0 runner    (1001) docker     (123)     5044 2023-05-05 13:41:01.000000 dspace_stats_collector-0.6.8/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-05-05 13:41:01.000000 dspace_stats_collector-0.6.8/docs/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-05-05 13:41:01.000000 dspace_stats_collector-0.6.8/docs/history.rst
--rw-r--r--   0 runner    (1001) docker     (123)      325 2023-05-05 13:41:01.000000 dspace_stats_collector-0.6.8/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-05-05 13:41:01.000000 dspace_stats_collector-0.6.8/docs/installation.rst
--rw-r--r--   0 runner    (1001) docker     (123)      784 2023-05-05 13:41:01.000000 dspace_stats_collector-0.6.8/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (123)    52797 2023-05-05 13:41:01.000000 dspace_stats_collector-0.6.8/docs/pipeline-diagram.png
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-05-05 13:41:01.000000 dspace_stats_collector-0.6.8/docs/readme.rst
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-05 13:41:01.000000 dspace_stats_collector-0.6.8/docs/usage.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 13:41:14.459250 dspace_stats_collector-0.6.8/dspace_stats_collector/
--rw-r--r--   0 runner    (1001) docker     (123)      405 2023-05-05 13:41:01.000000 dspace_stats_collector-0.6.8/dspace_stats_collector/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7008 2023-05-05 13:41:01.000000 dspace_stats_collector-0.6.8/dspace_stats_collector/collector.py
--rw-r--r--   0 runner    (1001) docker     (123)    13599 2023-05-05 13:41:01.000000 dspace_stats_collector-0.6.8/dspace_stats_collector/configcontext.py
--rw-r--r--   0 runner    (1001) docker     (123)     4548 2023-05-05 13:41:01.000000 dspace_stats_collector-0.6.8/dspace_stats_collector/configure.py
--rw-r--r--   0 runner    (1001) docker     (123)     1690 2023-05-05 13:41:01.000000 dspace_stats_collector-0.6.8/dspace_stats_collector/counterfilter.py
--rw-r--r--   0 runner    (1001) docker     (123)     2309 2023-05-05 13:41:01.000000 dspace_stats_collector-0.6.8/dspace_stats_collector/croninstaller.py
--rw-r--r--   0 runner    (1001) docker     (123)     4541 2023-05-05 13:41:01.000000 dspace_stats_collector-0.6.8/dspace_stats_collector/dspacedb.py
--rw-r--r--   0 runner    (1001) docker     (123)     2312 2023-05-05 13:41:01.000000 dspace_stats_collector-0.6.8/dspace_stats_collector/dspacedb4.py
--rw-r--r--   0 runner    (1001) docker     (123)     2528 2023-05-05 13:41:01.000000 dspace_stats_collector-0.6.8/dspace_stats_collector/dspacedb5.py
--rw-r--r--   0 runner    (1001) docker     (123)     2532 2023-05-05 13:41:01.000000 dspace_stats_collector-0.6.8/dspace_stats_collector/dspacedb5cris.py
--rw-r--r--   0 runner    (1001) docker     (123)     2496 2023-05-05 13:41:01.000000 dspace_stats_collector-0.6.8/dspace_stats_collector/dspacedb5oracle.py
--rw-r--r--   0 runner    (1001) docker     (123)     2454 2023-05-05 13:41:01.000000 dspace_stats_collector-0.6.8/dspace_stats_collector/dspacedb6.py
--rw-r--r--   0 runner    (1001) docker     (123)     2725 2023-05-05 13:41:01.000000 dspace_stats_collector-0.6.8/dspace_stats_collector/dspacedb6oracle.py
--rw-r--r--   0 runner    (1001) docker     (123)     2454 2023-05-05 13:41:01.000000 dspace_stats_collector-0.6.8/dspace_stats_collector/dspacedb7.py
--rw-r--r--   0 runner    (1001) docker     (123)     1106 2023-05-05 13:41:01.000000 dspace_stats_collector-0.6.8/dspace_stats_collector/dspacefilter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1214 2023-05-05 13:41:01.000000 dspace_stats_collector-0.6.8/dspace_stats_collector/elasticoutput.py
--rw-r--r--   0 runner    (1001) docker     (123)     1745 2023-05-05 13:41:01.000000 dspace_stats_collector-0.6.8/dspace_stats_collector/eventpipeline.py
--rw-r--r--   0 runner    (1001) docker     (123)     9638 2023-05-05 13:41:01.000000 dspace_stats_collector-0.6.8/dspace_stats_collector/matomooutput.py
--rw-r--r--   0 runner    (1001) docker     (123)     2305 2023-05-05 13:41:01.000000 dspace_stats_collector-0.6.8/dspace_stats_collector/sessionfilter.py
--rw-r--r--   0 runner    (1001) docker     (123)     7079 2023-05-05 13:41:01.000000 dspace_stats_collector-0.6.8/dspace_stats_collector/solrinput.py
--rw-r--r--   0 runner    (1001) docker     (123)      373 2023-05-05 13:41:01.000000 dspace_stats_collector-0.6.8/dspace_stats_collector/test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 13:41:14.459250 dspace_stats_collector-0.6.8/dspace_stats_collector.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6046 2023-05-05 13:41:14.000000 dspace_stats_collector-0.6.8/dspace_stats_collector.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2363 2023-05-05 13:41:14.000000 dspace_stats_collector-0.6.8/dspace_stats_collector.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 13:41:14.000000 dspace_stats_collector-0.6.8/dspace_stats_collector.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      209 2023-05-05 13:41:14.000000 dspace_stats_collector-0.6.8/dspace_stats_collector.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 13:41:14.000000 dspace_stats_collector-0.6.8/dspace_stats_collector.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-05 13:41:14.000000 dspace_stats_collector-0.6.8/dspace_stats_collector.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      464 2023-05-05 13:41:14.467250 dspace_stats_collector-0.6.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2030 2023-05-05 13:41:01.000000 dspace_stats_collector-0.6.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 13:41:14.459250 dspace_stats_collector-0.6.8/tests/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 13:41:14.463250 dspace_stats_collector-0.6.8/tests/dspace_stats_collector/
--rw-r--r--   0 runner    (1001) docker     (123)      405 2023-05-05 13:41:01.000000 dspace_stats_collector-0.6.8/tests/dspace_stats_collector/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7008 2023-05-05 13:41:01.000000 dspace_stats_collector-0.6.8/tests/dspace_stats_collector/collector.py
--rw-r--r--   0 runner    (1001) docker     (123)    13599 2023-05-05 13:41:01.000000 dspace_stats_collector-0.6.8/tests/dspace_stats_collector/configcontext.py
--rw-r--r--   0 runner    (1001) docker     (123)     4548 2023-05-05 13:41:01.000000 dspace_stats_collector-0.6.8/tests/dspace_stats_collector/configure.py
--rw-r--r--   0 runner    (1001) docker     (123)     1690 2023-05-05 13:41:01.000000 dspace_stats_collector-0.6.8/tests/dspace_stats_collector/counterfilter.py
--rw-r--r--   0 runner    (1001) docker     (123)     2309 2023-05-05 13:41:01.000000 dspace_stats_collector-0.6.8/tests/dspace_stats_collector/croninstaller.py
--rw-r--r--   0 runner    (1001) docker     (123)     4541 2023-05-05 13:41:01.000000 dspace_stats_collector-0.6.8/tests/dspace_stats_collector/dspacedb.py
--rw-r--r--   0 runner    (1001) docker     (123)     2312 2023-05-05 13:41:01.000000 dspace_stats_collector-0.6.8/tests/dspace_stats_collector/dspacedb4.py
--rw-r--r--   0 runner    (1001) docker     (123)     2528 2023-05-05 13:41:01.000000 dspace_stats_collector-0.6.8/tests/dspace_stats_collector/dspacedb5.py
--rw-r--r--   0 runner    (1001) docker     (123)     2532 2023-05-05 13:41:01.000000 dspace_stats_collector-0.6.8/tests/dspace_stats_collector/dspacedb5cris.py
--rw-r--r--   0 runner    (1001) docker     (123)     2496 2023-05-05 13:41:01.000000 dspace_stats_collector-0.6.8/tests/dspace_stats_collector/dspacedb5oracle.py
--rw-r--r--   0 runner    (1001) docker     (123)     2454 2023-05-05 13:41:01.000000 dspace_stats_collector-0.6.8/tests/dspace_stats_collector/dspacedb6.py
--rw-r--r--   0 runner    (1001) docker     (123)     2725 2023-05-05 13:41:01.000000 dspace_stats_collector-0.6.8/tests/dspace_stats_collector/dspacedb6oracle.py
--rw-r--r--   0 runner    (1001) docker     (123)     2454 2023-05-05 13:41:01.000000 dspace_stats_collector-0.6.8/tests/dspace_stats_collector/dspacedb7.py
--rw-r--r--   0 runner    (1001) docker     (123)     1106 2023-05-05 13:41:01.000000 dspace_stats_collector-0.6.8/tests/dspace_stats_collector/dspacefilter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1214 2023-05-05 13:41:01.000000 dspace_stats_collector-0.6.8/tests/dspace_stats_collector/elasticoutput.py
--rw-r--r--   0 runner    (1001) docker     (123)     1745 2023-05-05 13:41:01.000000 dspace_stats_collector-0.6.8/tests/dspace_stats_collector/eventpipeline.py
--rw-r--r--   0 runner    (1001) docker     (123)     9638 2023-05-05 13:41:01.000000 dspace_stats_collector-0.6.8/tests/dspace_stats_collector/matomooutput.py
--rw-r--r--   0 runner    (1001) docker     (123)     2305 2023-05-05 13:41:01.000000 dspace_stats_collector-0.6.8/tests/dspace_stats_collector/sessionfilter.py
--rw-r--r--   0 runner    (1001) docker     (123)     7079 2023-05-05 13:41:01.000000 dspace_stats_collector-0.6.8/tests/dspace_stats_collector/solrinput.py
--rw-r--r--   0 runner    (1001) docker     (123)      373 2023-05-05 13:41:01.000000 dspace_stats_collector-0.6.8/tests/dspace_stats_collector/test.py
--rw-r--r--   0 runner    (1001) docker     (123)      423 2023-05-05 13:41:01.000000 dspace_stats_collector-0.6.8/tests/test_dspace_stats_collector.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 15:15:55.754534 dspace_stats_collector-0.6.9/
+-rw-r--r--   0 runner    (1001) docker     (123)      364 2023-05-05 15:15:35.000000 dspace_stats_collector-0.6.9/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3713 2023-05-05 15:15:35.000000 dspace_stats_collector-0.6.9/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-05-05 15:15:35.000000 dspace_stats_collector-0.6.9/HISTORY.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1565 2023-05-05 15:15:35.000000 dspace_stats_collector-0.6.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      289 2023-05-05 15:15:35.000000 dspace_stats_collector-0.6.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     6046 2023-05-05 15:15:55.754534 dspace_stats_collector-0.6.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5246 2023-05-05 15:15:35.000000 dspace_stats_collector-0.6.9/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 15:15:55.734534 dspace_stats_collector-0.6.9/config/
+-rw-r--r--   0 runner    (1001) docker     (123)    23785 2023-05-05 15:15:35.000000 dspace_stats_collector-0.6.9/config/COUNTER_Robots_list.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 15:15:55.738534 dspace_stats_collector-0.6.9/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      623 2023-05-05 15:15:35.000000 dspace_stats_collector-0.6.9/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     4316 2023-05-05 15:15:35.000000 dspace_stats_collector-0.6.9/docs/README_BR.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-05-05 15:15:35.000000 dspace_stats_collector-0.6.9/docs/authors.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     5044 2023-05-05 15:15:35.000000 dspace_stats_collector-0.6.9/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-05-05 15:15:35.000000 dspace_stats_collector-0.6.9/docs/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-05-05 15:15:35.000000 dspace_stats_collector-0.6.9/docs/history.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      325 2023-05-05 15:15:35.000000 dspace_stats_collector-0.6.9/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-05-05 15:15:35.000000 dspace_stats_collector-0.6.9/docs/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      784 2023-05-05 15:15:35.000000 dspace_stats_collector-0.6.9/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (123)    52797 2023-05-05 15:15:35.000000 dspace_stats_collector-0.6.9/docs/pipeline-diagram.png
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-05-05 15:15:35.000000 dspace_stats_collector-0.6.9/docs/readme.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-05 15:15:35.000000 dspace_stats_collector-0.6.9/docs/usage.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 15:15:55.746534 dspace_stats_collector-0.6.9/dspace_stats_collector/
+-rw-r--r--   0 runner    (1001) docker     (123)      405 2023-05-05 15:15:35.000000 dspace_stats_collector-0.6.9/dspace_stats_collector/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7008 2023-05-05 15:15:35.000000 dspace_stats_collector-0.6.9/dspace_stats_collector/collector.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13599 2023-05-05 15:15:35.000000 dspace_stats_collector-0.6.9/dspace_stats_collector/configcontext.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4548 2023-05-05 15:15:35.000000 dspace_stats_collector-0.6.9/dspace_stats_collector/configure.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1690 2023-05-05 15:15:35.000000 dspace_stats_collector-0.6.9/dspace_stats_collector/counterfilter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2309 2023-05-05 15:15:35.000000 dspace_stats_collector-0.6.9/dspace_stats_collector/croninstaller.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4541 2023-05-05 15:15:35.000000 dspace_stats_collector-0.6.9/dspace_stats_collector/dspacedb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2312 2023-05-05 15:15:35.000000 dspace_stats_collector-0.6.9/dspace_stats_collector/dspacedb4.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2528 2023-05-05 15:15:35.000000 dspace_stats_collector-0.6.9/dspace_stats_collector/dspacedb5.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2532 2023-05-05 15:15:35.000000 dspace_stats_collector-0.6.9/dspace_stats_collector/dspacedb5cris.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2496 2023-05-05 15:15:35.000000 dspace_stats_collector-0.6.9/dspace_stats_collector/dspacedb5oracle.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2454 2023-05-05 15:15:35.000000 dspace_stats_collector-0.6.9/dspace_stats_collector/dspacedb6.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2725 2023-05-05 15:15:35.000000 dspace_stats_collector-0.6.9/dspace_stats_collector/dspacedb6oracle.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2454 2023-05-05 15:15:35.000000 dspace_stats_collector-0.6.9/dspace_stats_collector/dspacedb7.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1106 2023-05-05 15:15:35.000000 dspace_stats_collector-0.6.9/dspace_stats_collector/dspacefilter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1214 2023-05-05 15:15:35.000000 dspace_stats_collector-0.6.9/dspace_stats_collector/elasticoutput.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1745 2023-05-05 15:15:35.000000 dspace_stats_collector-0.6.9/dspace_stats_collector/eventpipeline.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9638 2023-05-05 15:15:35.000000 dspace_stats_collector-0.6.9/dspace_stats_collector/matomooutput.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2452 2023-05-05 15:15:35.000000 dspace_stats_collector-0.6.9/dspace_stats_collector/sessionfilter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7079 2023-05-05 15:15:35.000000 dspace_stats_collector-0.6.9/dspace_stats_collector/solrinput.py
+-rw-r--r--   0 runner    (1001) docker     (123)      373 2023-05-05 15:15:35.000000 dspace_stats_collector-0.6.9/dspace_stats_collector/test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 15:15:55.746534 dspace_stats_collector-0.6.9/dspace_stats_collector.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6046 2023-05-05 15:15:55.000000 dspace_stats_collector-0.6.9/dspace_stats_collector.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2363 2023-05-05 15:15:55.000000 dspace_stats_collector-0.6.9/dspace_stats_collector.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 15:15:55.000000 dspace_stats_collector-0.6.9/dspace_stats_collector.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      209 2023-05-05 15:15:55.000000 dspace_stats_collector-0.6.9/dspace_stats_collector.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 15:15:55.000000 dspace_stats_collector-0.6.9/dspace_stats_collector.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-05 15:15:55.000000 dspace_stats_collector-0.6.9/dspace_stats_collector.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      464 2023-05-05 15:15:55.754534 dspace_stats_collector-0.6.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2030 2023-05-05 15:15:35.000000 dspace_stats_collector-0.6.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 15:15:55.746534 dspace_stats_collector-0.6.9/tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 15:15:55.750534 dspace_stats_collector-0.6.9/tests/dspace_stats_collector/
+-rw-r--r--   0 runner    (1001) docker     (123)      405 2023-05-05 15:15:35.000000 dspace_stats_collector-0.6.9/tests/dspace_stats_collector/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7008 2023-05-05 15:15:35.000000 dspace_stats_collector-0.6.9/tests/dspace_stats_collector/collector.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13599 2023-05-05 15:15:35.000000 dspace_stats_collector-0.6.9/tests/dspace_stats_collector/configcontext.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4548 2023-05-05 15:15:35.000000 dspace_stats_collector-0.6.9/tests/dspace_stats_collector/configure.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1690 2023-05-05 15:15:35.000000 dspace_stats_collector-0.6.9/tests/dspace_stats_collector/counterfilter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2309 2023-05-05 15:15:35.000000 dspace_stats_collector-0.6.9/tests/dspace_stats_collector/croninstaller.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4541 2023-05-05 15:15:35.000000 dspace_stats_collector-0.6.9/tests/dspace_stats_collector/dspacedb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2312 2023-05-05 15:15:35.000000 dspace_stats_collector-0.6.9/tests/dspace_stats_collector/dspacedb4.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2528 2023-05-05 15:15:35.000000 dspace_stats_collector-0.6.9/tests/dspace_stats_collector/dspacedb5.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2532 2023-05-05 15:15:35.000000 dspace_stats_collector-0.6.9/tests/dspace_stats_collector/dspacedb5cris.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2496 2023-05-05 15:15:35.000000 dspace_stats_collector-0.6.9/tests/dspace_stats_collector/dspacedb5oracle.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2454 2023-05-05 15:15:35.000000 dspace_stats_collector-0.6.9/tests/dspace_stats_collector/dspacedb6.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2725 2023-05-05 15:15:35.000000 dspace_stats_collector-0.6.9/tests/dspace_stats_collector/dspacedb6oracle.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2454 2023-05-05 15:15:35.000000 dspace_stats_collector-0.6.9/tests/dspace_stats_collector/dspacedb7.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1106 2023-05-05 15:15:35.000000 dspace_stats_collector-0.6.9/tests/dspace_stats_collector/dspacefilter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1214 2023-05-05 15:15:35.000000 dspace_stats_collector-0.6.9/tests/dspace_stats_collector/elasticoutput.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1745 2023-05-05 15:15:35.000000 dspace_stats_collector-0.6.9/tests/dspace_stats_collector/eventpipeline.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9638 2023-05-05 15:15:35.000000 dspace_stats_collector-0.6.9/tests/dspace_stats_collector/matomooutput.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2452 2023-05-05 15:15:35.000000 dspace_stats_collector-0.6.9/tests/dspace_stats_collector/sessionfilter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7079 2023-05-05 15:15:35.000000 dspace_stats_collector-0.6.9/tests/dspace_stats_collector/solrinput.py
+-rw-r--r--   0 runner    (1001) docker     (123)      373 2023-05-05 15:15:35.000000 dspace_stats_collector-0.6.9/tests/dspace_stats_collector/test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      423 2023-05-05 15:15:35.000000 dspace_stats_collector-0.6.9/tests/test_dspace_stats_collector.py
```

### Comparing `dspace_stats_collector-0.6.8/CONTRIBUTING.rst` & `dspace_stats_collector-0.6.9/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `dspace_stats_collector-0.6.8/LICENSE` & `dspace_stats_collector-0.6.9/LICENSE`

 * *Files identical despite different names*

### Comparing `dspace_stats_collector-0.6.8/PKG-INFO` & `dspace_stats_collector-0.6.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dspace_stats_collector
-Version: 0.6.8
+Version: 0.6.9
 Summary: A python library for sending usage stats events from Dspace to Matomo
 Home-page: https://github.com/lareferencia/dspace-stats-collector
 Author: LA Referencia
 Author-email: lareferencia.dev@gmail.com
 License: GNU General Public License v3
 Keywords: dspace_stats_collector
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `dspace_stats_collector-0.6.8/README.rst` & `dspace_stats_collector-0.6.9/README.rst`

 * *Files identical despite different names*

### Comparing `dspace_stats_collector-0.6.8/config/COUNTER_Robots_list.json` & `dspace_stats_collector-0.6.9/config/COUNTER_Robots_list.json`

 * *Files identical despite different names*

### Comparing `dspace_stats_collector-0.6.8/docs/Makefile` & `dspace_stats_collector-0.6.9/docs/Makefile`

 * *Files identical despite different names*

### Comparing `dspace_stats_collector-0.6.8/docs/README_BR.rst` & `dspace_stats_collector-0.6.9/docs/README_BR.rst`

 * *Files identical despite different names*

### Comparing `dspace_stats_collector-0.6.8/docs/conf.py` & `dspace_stats_collector-0.6.9/docs/conf.py`

 * *Files identical despite different names*

### Comparing `dspace_stats_collector-0.6.8/docs/make.bat` & `dspace_stats_collector-0.6.9/docs/make.bat`

 * *Files identical despite different names*

### Comparing `dspace_stats_collector-0.6.8/docs/pipeline-diagram.png` & `dspace_stats_collector-0.6.9/docs/pipeline-diagram.png`

 * *Files identical despite different names*

### Comparing `dspace_stats_collector-0.6.8/dspace_stats_collector/collector.py` & `dspace_stats_collector-0.6.9/dspace_stats_collector/collector.py`

 * *Files identical despite different names*

### Comparing `dspace_stats_collector-0.6.8/dspace_stats_collector/configcontext.py` & `dspace_stats_collector-0.6.9/dspace_stats_collector/configcontext.py`

 * *Files identical despite different names*

### Comparing `dspace_stats_collector-0.6.8/dspace_stats_collector/configure.py` & `dspace_stats_collector-0.6.9/dspace_stats_collector/configure.py`

 * *Files identical despite different names*

### Comparing `dspace_stats_collector-0.6.8/dspace_stats_collector/counterfilter.py` & `dspace_stats_collector-0.6.9/dspace_stats_collector/counterfilter.py`

 * *Files identical despite different names*

### Comparing `dspace_stats_collector-0.6.8/dspace_stats_collector/croninstaller.py` & `dspace_stats_collector-0.6.9/dspace_stats_collector/croninstaller.py`

 * *Files identical despite different names*

### Comparing `dspace_stats_collector-0.6.8/dspace_stats_collector/dspacedb.py` & `dspace_stats_collector-0.6.9/dspace_stats_collector/dspacedb.py`

 * *Files identical despite different names*

### Comparing `dspace_stats_collector-0.6.8/dspace_stats_collector/dspacedb4.py` & `dspace_stats_collector-0.6.9/dspace_stats_collector/dspacedb4.py`

 * *Files identical despite different names*

### Comparing `dspace_stats_collector-0.6.8/dspace_stats_collector/dspacedb5.py` & `dspace_stats_collector-0.6.9/dspace_stats_collector/dspacedb5.py`

 * *Files identical despite different names*

### Comparing `dspace_stats_collector-0.6.8/dspace_stats_collector/dspacedb5cris.py` & `dspace_stats_collector-0.6.9/dspace_stats_collector/dspacedb5cris.py`

 * *Files identical despite different names*

### Comparing `dspace_stats_collector-0.6.8/dspace_stats_collector/dspacedb5oracle.py` & `dspace_stats_collector-0.6.9/dspace_stats_collector/dspacedb5oracle.py`

 * *Files identical despite different names*

### Comparing `dspace_stats_collector-0.6.8/dspace_stats_collector/dspacedb6.py` & `dspace_stats_collector-0.6.9/dspace_stats_collector/dspacedb6.py`

 * *Files identical despite different names*

### Comparing `dspace_stats_collector-0.6.8/dspace_stats_collector/dspacedb6oracle.py` & `dspace_stats_collector-0.6.9/dspace_stats_collector/dspacedb6oracle.py`

 * *Files identical despite different names*

### Comparing `dspace_stats_collector-0.6.8/dspace_stats_collector/dspacedb7.py` & `dspace_stats_collector-0.6.9/dspace_stats_collector/dspacedb7.py`

 * *Files identical despite different names*

### Comparing `dspace_stats_collector-0.6.8/dspace_stats_collector/dspacefilter.py` & `dspace_stats_collector-0.6.9/dspace_stats_collector/dspacefilter.py`

 * *Files identical despite different names*

### Comparing `dspace_stats_collector-0.6.8/dspace_stats_collector/elasticoutput.py` & `dspace_stats_collector-0.6.9/dspace_stats_collector/elasticoutput.py`

 * *Files identical despite different names*

### Comparing `dspace_stats_collector-0.6.8/dspace_stats_collector/eventpipeline.py` & `dspace_stats_collector-0.6.9/dspace_stats_collector/eventpipeline.py`

 * *Files identical despite different names*

### Comparing `dspace_stats_collector-0.6.8/dspace_stats_collector/matomooutput.py` & `dspace_stats_collector-0.6.9/dspace_stats_collector/matomooutput.py`

 * *Files identical despite different names*

### Comparing `dspace_stats_collector-0.6.8/dspace_stats_collector/sessionfilter.py` & `dspace_stats_collector-0.6.9/dspace_stats_collector/sessionfilter.py`

 * *Files 5% similar despite different names*

```diff
@@ -38,15 +38,21 @@
                 if self._anonymize_ip_mask != self.FULL_IP_MASK:     
                     event._src['ip'] = anonymize_ip(event._src.get('ip','0.0.0.0'), self._anonymize_ip_mask)    
             
             except Exception as e:
 
                  # check if ip is folowing the format ip:port
                 if ':' in event._src.get('ip','0.0.0.0'):
-                    ip, port = event._src.get('ip','0.0.0.0').split(':')
+
+                    splited = event._src.get('ip','0.0.0.0').split(':')
+
+                    if len(splited) > 1:
+                        ip = splited[0]
+                    else:
+                        ip = '0.0.0.0'
                     
                     ## check the ip string is a valid ip address
                     try:
                         # this will raise a ValueError if the ip is not valid
                         ip_address(ip)
 
                         # anonymize ip
```

### Comparing `dspace_stats_collector-0.6.8/dspace_stats_collector/solrinput.py` & `dspace_stats_collector-0.6.9/dspace_stats_collector/solrinput.py`

 * *Files identical despite different names*

### Comparing `dspace_stats_collector-0.6.8/dspace_stats_collector.egg-info/PKG-INFO` & `dspace_stats_collector-0.6.9/dspace_stats_collector.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dspace-stats-collector
-Version: 0.6.8
+Version: 0.6.9
 Summary: A python library for sending usage stats events from Dspace to Matomo
 Home-page: https://github.com/lareferencia/dspace-stats-collector
 Author: LA Referencia
 Author-email: lareferencia.dev@gmail.com
 License: GNU General Public License v3
 Keywords: dspace_stats_collector
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `dspace_stats_collector-0.6.8/dspace_stats_collector.egg-info/SOURCES.txt` & `dspace_stats_collector-0.6.9/dspace_stats_collector.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dspace_stats_collector-0.6.8/setup.py` & `dspace_stats_collector-0.6.9/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -57,10 +57,10 @@
     packages=find_packages(include=['dspace_stats_collector']),
     entry_points=entry_points,
  #   package_data=package_data,
     setup_requires=setup_requirements,
     test_suite='tests',
     tests_require=test_requirements,
     url='https://github.com/lareferencia/dspace-stats-collector',
-    version='0.6.8',
+    version='0.6.9',
     zip_safe=False,
 )
```

### Comparing `dspace_stats_collector-0.6.8/tests/dspace_stats_collector/collector.py` & `dspace_stats_collector-0.6.9/tests/dspace_stats_collector/collector.py`

 * *Files identical despite different names*

### Comparing `dspace_stats_collector-0.6.8/tests/dspace_stats_collector/configcontext.py` & `dspace_stats_collector-0.6.9/tests/dspace_stats_collector/configcontext.py`

 * *Files identical despite different names*

### Comparing `dspace_stats_collector-0.6.8/tests/dspace_stats_collector/configure.py` & `dspace_stats_collector-0.6.9/tests/dspace_stats_collector/configure.py`

 * *Files identical despite different names*

### Comparing `dspace_stats_collector-0.6.8/tests/dspace_stats_collector/counterfilter.py` & `dspace_stats_collector-0.6.9/tests/dspace_stats_collector/counterfilter.py`

 * *Files identical despite different names*

### Comparing `dspace_stats_collector-0.6.8/tests/dspace_stats_collector/croninstaller.py` & `dspace_stats_collector-0.6.9/tests/dspace_stats_collector/croninstaller.py`

 * *Files identical despite different names*

### Comparing `dspace_stats_collector-0.6.8/tests/dspace_stats_collector/dspacedb.py` & `dspace_stats_collector-0.6.9/tests/dspace_stats_collector/dspacedb.py`

 * *Files identical despite different names*

### Comparing `dspace_stats_collector-0.6.8/tests/dspace_stats_collector/dspacedb4.py` & `dspace_stats_collector-0.6.9/tests/dspace_stats_collector/dspacedb4.py`

 * *Files identical despite different names*

### Comparing `dspace_stats_collector-0.6.8/tests/dspace_stats_collector/dspacedb5.py` & `dspace_stats_collector-0.6.9/tests/dspace_stats_collector/dspacedb5.py`

 * *Files identical despite different names*

### Comparing `dspace_stats_collector-0.6.8/tests/dspace_stats_collector/dspacedb5cris.py` & `dspace_stats_collector-0.6.9/tests/dspace_stats_collector/dspacedb5cris.py`

 * *Files identical despite different names*

### Comparing `dspace_stats_collector-0.6.8/tests/dspace_stats_collector/dspacedb5oracle.py` & `dspace_stats_collector-0.6.9/tests/dspace_stats_collector/dspacedb5oracle.py`

 * *Files identical despite different names*

### Comparing `dspace_stats_collector-0.6.8/tests/dspace_stats_collector/dspacedb6.py` & `dspace_stats_collector-0.6.9/tests/dspace_stats_collector/dspacedb6.py`

 * *Files identical despite different names*

### Comparing `dspace_stats_collector-0.6.8/tests/dspace_stats_collector/dspacedb6oracle.py` & `dspace_stats_collector-0.6.9/tests/dspace_stats_collector/dspacedb6oracle.py`

 * *Files identical despite different names*

### Comparing `dspace_stats_collector-0.6.8/tests/dspace_stats_collector/dspacedb7.py` & `dspace_stats_collector-0.6.9/tests/dspace_stats_collector/dspacedb7.py`

 * *Files identical despite different names*

### Comparing `dspace_stats_collector-0.6.8/tests/dspace_stats_collector/dspacefilter.py` & `dspace_stats_collector-0.6.9/tests/dspace_stats_collector/dspacefilter.py`

 * *Files identical despite different names*

### Comparing `dspace_stats_collector-0.6.8/tests/dspace_stats_collector/elasticoutput.py` & `dspace_stats_collector-0.6.9/tests/dspace_stats_collector/elasticoutput.py`

 * *Files identical despite different names*

### Comparing `dspace_stats_collector-0.6.8/tests/dspace_stats_collector/eventpipeline.py` & `dspace_stats_collector-0.6.9/tests/dspace_stats_collector/eventpipeline.py`

 * *Files identical despite different names*

### Comparing `dspace_stats_collector-0.6.8/tests/dspace_stats_collector/matomooutput.py` & `dspace_stats_collector-0.6.9/tests/dspace_stats_collector/matomooutput.py`

 * *Files identical despite different names*

### Comparing `dspace_stats_collector-0.6.8/tests/dspace_stats_collector/sessionfilter.py` & `dspace_stats_collector-0.6.9/tests/dspace_stats_collector/sessionfilter.py`

 * *Files 5% similar despite different names*

```diff
@@ -38,15 +38,21 @@
                 if self._anonymize_ip_mask != self.FULL_IP_MASK:     
                     event._src['ip'] = anonymize_ip(event._src.get('ip','0.0.0.0'), self._anonymize_ip_mask)    
             
             except Exception as e:
 
                  # check if ip is folowing the format ip:port
                 if ':' in event._src.get('ip','0.0.0.0'):
-                    ip, port = event._src.get('ip','0.0.0.0').split(':')
+
+                    splited = event._src.get('ip','0.0.0.0').split(':')
+
+                    if len(splited) > 1:
+                        ip = splited[0]
+                    else:
+                        ip = '0.0.0.0'
                     
                     ## check the ip string is a valid ip address
                     try:
                         # this will raise a ValueError if the ip is not valid
                         ip_address(ip)
 
                         # anonymize ip
```

### Comparing `dspace_stats_collector-0.6.8/tests/dspace_stats_collector/solrinput.py` & `dspace_stats_collector-0.6.9/tests/dspace_stats_collector/solrinput.py`

 * *Files identical despite different names*

