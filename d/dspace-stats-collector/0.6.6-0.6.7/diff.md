# Comparing `tmp/dspace_stats_collector-0.6.6.tar.gz` & `tmp/dspace_stats_collector-0.6.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dspace_stats_collector-0.6.6.tar", last modified: Tue Jan 24 11:54:10 2023, max compression
+gzip compressed data, was "dspace_stats_collector-0.6.7.tar", last modified: Thu May  4 20:52:32 2023, max compression
```

## Comparing `dspace_stats_collector-0.6.6.tar` & `dspace_stats_collector-0.6.7.tar`

### file list

```diff
@@ -1,78 +1,78 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-24 11:54:10.457239 dspace_stats_collector-0.6.6/
--rw-r--r--   0 runner    (1001) docker     (123)      364 2023-01-24 11:54:01.000000 dspace_stats_collector-0.6.6/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (123)     3713 2023-01-24 11:54:01.000000 dspace_stats_collector-0.6.6/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-01-24 11:54:01.000000 dspace_stats_collector-0.6.6/HISTORY.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1565 2023-01-24 11:54:01.000000 dspace_stats_collector-0.6.6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      289 2023-01-24 11:54:01.000000 dspace_stats_collector-0.6.6/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     6046 2023-01-24 11:54:10.457239 dspace_stats_collector-0.6.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5246 2023-01-24 11:54:01.000000 dspace_stats_collector-0.6.6/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-24 11:54:10.453239 dspace_stats_collector-0.6.6/config/
--rw-r--r--   0 runner    (1001) docker     (123)    23785 2023-01-24 11:54:01.000000 dspace_stats_collector-0.6.6/config/COUNTER_Robots_list.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-24 11:54:10.453239 dspace_stats_collector-0.6.6/docs/
--rw-r--r--   0 runner    (1001) docker     (123)      623 2023-01-24 11:54:01.000000 dspace_stats_collector-0.6.6/docs/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)     4316 2023-01-24 11:54:01.000000 dspace_stats_collector-0.6.6/docs/README_BR.rst
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-01-24 11:54:01.000000 dspace_stats_collector-0.6.6/docs/authors.rst
--rw-r--r--   0 runner    (1001) docker     (123)     5044 2023-01-24 11:54:01.000000 dspace_stats_collector-0.6.6/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-01-24 11:54:01.000000 dspace_stats_collector-0.6.6/docs/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-01-24 11:54:01.000000 dspace_stats_collector-0.6.6/docs/history.rst
--rw-r--r--   0 runner    (1001) docker     (123)      325 2023-01-24 11:54:01.000000 dspace_stats_collector-0.6.6/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-01-24 11:54:01.000000 dspace_stats_collector-0.6.6/docs/installation.rst
--rw-r--r--   0 runner    (1001) docker     (123)      784 2023-01-24 11:54:01.000000 dspace_stats_collector-0.6.6/docs/make.bat
--rw-r--r--   0 runner    (1001) docker     (123)    52797 2023-01-24 11:54:01.000000 dspace_stats_collector-0.6.6/docs/pipeline-diagram.png
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-01-24 11:54:01.000000 dspace_stats_collector-0.6.6/docs/readme.rst
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-01-24 11:54:01.000000 dspace_stats_collector-0.6.6/docs/usage.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-24 11:54:10.453239 dspace_stats_collector-0.6.6/dspace_stats_collector/
--rw-r--r--   0 runner    (1001) docker     (123)      405 2023-01-24 11:54:01.000000 dspace_stats_collector-0.6.6/dspace_stats_collector/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7008 2023-01-24 11:54:01.000000 dspace_stats_collector-0.6.6/dspace_stats_collector/collector.py
--rw-r--r--   0 runner    (1001) docker     (123)    13599 2023-01-24 11:54:01.000000 dspace_stats_collector-0.6.6/dspace_stats_collector/configcontext.py
--rw-r--r--   0 runner    (1001) docker     (123)     4548 2023-01-24 11:54:01.000000 dspace_stats_collector-0.6.6/dspace_stats_collector/configure.py
--rw-r--r--   0 runner    (1001) docker     (123)     1690 2023-01-24 11:54:01.000000 dspace_stats_collector-0.6.6/dspace_stats_collector/counterfilter.py
--rw-r--r--   0 runner    (1001) docker     (123)     2309 2023-01-24 11:54:01.000000 dspace_stats_collector-0.6.6/dspace_stats_collector/croninstaller.py
--rw-r--r--   0 runner    (1001) docker     (123)     4541 2023-01-24 11:54:01.000000 dspace_stats_collector-0.6.6/dspace_stats_collector/dspacedb.py
--rw-r--r--   0 runner    (1001) docker     (123)     2312 2023-01-24 11:54:01.000000 dspace_stats_collector-0.6.6/dspace_stats_collector/dspacedb4.py
--rw-r--r--   0 runner    (1001) docker     (123)     2528 2023-01-24 11:54:01.000000 dspace_stats_collector-0.6.6/dspace_stats_collector/dspacedb5.py
--rw-r--r--   0 runner    (1001) docker     (123)     2532 2023-01-24 11:54:01.000000 dspace_stats_collector-0.6.6/dspace_stats_collector/dspacedb5cris.py
--rw-r--r--   0 runner    (1001) docker     (123)     2496 2023-01-24 11:54:01.000000 dspace_stats_collector-0.6.6/dspace_stats_collector/dspacedb5oracle.py
--rw-r--r--   0 runner    (1001) docker     (123)     2454 2023-01-24 11:54:01.000000 dspace_stats_collector-0.6.6/dspace_stats_collector/dspacedb6.py
--rw-r--r--   0 runner    (1001) docker     (123)     2422 2023-01-24 11:54:01.000000 dspace_stats_collector-0.6.6/dspace_stats_collector/dspacedb6oracle.py
--rw-r--r--   0 runner    (1001) docker     (123)     2454 2023-01-24 11:54:01.000000 dspace_stats_collector-0.6.6/dspace_stats_collector/dspacedb7.py
--rw-r--r--   0 runner    (1001) docker     (123)     1106 2023-01-24 11:54:01.000000 dspace_stats_collector-0.6.6/dspace_stats_collector/dspacefilter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1214 2023-01-24 11:54:01.000000 dspace_stats_collector-0.6.6/dspace_stats_collector/elasticoutput.py
--rw-r--r--   0 runner    (1001) docker     (123)     1745 2023-01-24 11:54:01.000000 dspace_stats_collector-0.6.6/dspace_stats_collector/eventpipeline.py
--rw-r--r--   0 runner    (1001) docker     (123)     9638 2023-01-24 11:54:01.000000 dspace_stats_collector-0.6.6/dspace_stats_collector/matomooutput.py
--rw-r--r--   0 runner    (1001) docker     (123)     1463 2023-01-24 11:54:01.000000 dspace_stats_collector-0.6.6/dspace_stats_collector/sessionfilter.py
--rw-r--r--   0 runner    (1001) docker     (123)     7079 2023-01-24 11:54:01.000000 dspace_stats_collector-0.6.6/dspace_stats_collector/solrinput.py
--rw-r--r--   0 runner    (1001) docker     (123)      373 2023-01-24 11:54:01.000000 dspace_stats_collector-0.6.6/dspace_stats_collector/test.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-24 11:54:10.453239 dspace_stats_collector-0.6.6/dspace_stats_collector.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6046 2023-01-24 11:54:10.000000 dspace_stats_collector-0.6.6/dspace_stats_collector.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2363 2023-01-24 11:54:10.000000 dspace_stats_collector-0.6.6/dspace_stats_collector.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-24 11:54:10.000000 dspace_stats_collector-0.6.6/dspace_stats_collector.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      209 2023-01-24 11:54:10.000000 dspace_stats_collector-0.6.6/dspace_stats_collector.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-24 11:54:10.000000 dspace_stats_collector-0.6.6/dspace_stats_collector.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-01-24 11:54:10.000000 dspace_stats_collector-0.6.6/dspace_stats_collector.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      464 2023-01-24 11:54:10.457239 dspace_stats_collector-0.6.6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2030 2023-01-24 11:54:01.000000 dspace_stats_collector-0.6.6/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-24 11:54:10.453239 dspace_stats_collector-0.6.6/tests/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-24 11:54:10.457239 dspace_stats_collector-0.6.6/tests/dspace_stats_collector/
--rw-r--r--   0 runner    (1001) docker     (123)      405 2023-01-24 11:54:01.000000 dspace_stats_collector-0.6.6/tests/dspace_stats_collector/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7008 2023-01-24 11:54:01.000000 dspace_stats_collector-0.6.6/tests/dspace_stats_collector/collector.py
--rw-r--r--   0 runner    (1001) docker     (123)    13599 2023-01-24 11:54:01.000000 dspace_stats_collector-0.6.6/tests/dspace_stats_collector/configcontext.py
--rw-r--r--   0 runner    (1001) docker     (123)     4548 2023-01-24 11:54:01.000000 dspace_stats_collector-0.6.6/tests/dspace_stats_collector/configure.py
--rw-r--r--   0 runner    (1001) docker     (123)     1690 2023-01-24 11:54:01.000000 dspace_stats_collector-0.6.6/tests/dspace_stats_collector/counterfilter.py
--rw-r--r--   0 runner    (1001) docker     (123)     2309 2023-01-24 11:54:01.000000 dspace_stats_collector-0.6.6/tests/dspace_stats_collector/croninstaller.py
--rw-r--r--   0 runner    (1001) docker     (123)     4541 2023-01-24 11:54:01.000000 dspace_stats_collector-0.6.6/tests/dspace_stats_collector/dspacedb.py
--rw-r--r--   0 runner    (1001) docker     (123)     2312 2023-01-24 11:54:01.000000 dspace_stats_collector-0.6.6/tests/dspace_stats_collector/dspacedb4.py
--rw-r--r--   0 runner    (1001) docker     (123)     2528 2023-01-24 11:54:01.000000 dspace_stats_collector-0.6.6/tests/dspace_stats_collector/dspacedb5.py
--rw-r--r--   0 runner    (1001) docker     (123)     2532 2023-01-24 11:54:01.000000 dspace_stats_collector-0.6.6/tests/dspace_stats_collector/dspacedb5cris.py
--rw-r--r--   0 runner    (1001) docker     (123)     2496 2023-01-24 11:54:01.000000 dspace_stats_collector-0.6.6/tests/dspace_stats_collector/dspacedb5oracle.py
--rw-r--r--   0 runner    (1001) docker     (123)     2454 2023-01-24 11:54:01.000000 dspace_stats_collector-0.6.6/tests/dspace_stats_collector/dspacedb6.py
--rw-r--r--   0 runner    (1001) docker     (123)     2422 2023-01-24 11:54:01.000000 dspace_stats_collector-0.6.6/tests/dspace_stats_collector/dspacedb6oracle.py
--rw-r--r--   0 runner    (1001) docker     (123)     2454 2023-01-24 11:54:01.000000 dspace_stats_collector-0.6.6/tests/dspace_stats_collector/dspacedb7.py
--rw-r--r--   0 runner    (1001) docker     (123)     1106 2023-01-24 11:54:01.000000 dspace_stats_collector-0.6.6/tests/dspace_stats_collector/dspacefilter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1214 2023-01-24 11:54:01.000000 dspace_stats_collector-0.6.6/tests/dspace_stats_collector/elasticoutput.py
--rw-r--r--   0 runner    (1001) docker     (123)     1745 2023-01-24 11:54:01.000000 dspace_stats_collector-0.6.6/tests/dspace_stats_collector/eventpipeline.py
--rw-r--r--   0 runner    (1001) docker     (123)     9638 2023-01-24 11:54:01.000000 dspace_stats_collector-0.6.6/tests/dspace_stats_collector/matomooutput.py
--rw-r--r--   0 runner    (1001) docker     (123)     1463 2023-01-24 11:54:01.000000 dspace_stats_collector-0.6.6/tests/dspace_stats_collector/sessionfilter.py
--rw-r--r--   0 runner    (1001) docker     (123)     7079 2023-01-24 11:54:01.000000 dspace_stats_collector-0.6.6/tests/dspace_stats_collector/solrinput.py
--rw-r--r--   0 runner    (1001) docker     (123)      373 2023-01-24 11:54:01.000000 dspace_stats_collector-0.6.6/tests/dspace_stats_collector/test.py
--rw-r--r--   0 runner    (1001) docker     (123)      423 2023-01-24 11:54:01.000000 dspace_stats_collector-0.6.6/tests/test_dspace_stats_collector.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 20:52:32.783541 dspace_stats_collector-0.6.7/
+-rw-r--r--   0 runner    (1001) docker     (123)      364 2023-05-04 20:52:12.000000 dspace_stats_collector-0.6.7/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     3713 2023-05-04 20:52:12.000000 dspace_stats_collector-0.6.7/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-05-04 20:52:12.000000 dspace_stats_collector-0.6.7/HISTORY.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1565 2023-05-04 20:52:12.000000 dspace_stats_collector-0.6.7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      289 2023-05-04 20:52:12.000000 dspace_stats_collector-0.6.7/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     6046 2023-05-04 20:52:32.783541 dspace_stats_collector-0.6.7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5246 2023-05-04 20:52:12.000000 dspace_stats_collector-0.6.7/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 20:52:32.771541 dspace_stats_collector-0.6.7/config/
+-rw-r--r--   0 runner    (1001) docker     (123)    23785 2023-05-04 20:52:12.000000 dspace_stats_collector-0.6.7/config/COUNTER_Robots_list.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 20:52:32.775541 dspace_stats_collector-0.6.7/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)      623 2023-05-04 20:52:12.000000 dspace_stats_collector-0.6.7/docs/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)     4316 2023-05-04 20:52:12.000000 dspace_stats_collector-0.6.7/docs/README_BR.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-05-04 20:52:12.000000 dspace_stats_collector-0.6.7/docs/authors.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     5044 2023-05-04 20:52:12.000000 dspace_stats_collector-0.6.7/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-05-04 20:52:12.000000 dspace_stats_collector-0.6.7/docs/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-05-04 20:52:12.000000 dspace_stats_collector-0.6.7/docs/history.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      325 2023-05-04 20:52:12.000000 dspace_stats_collector-0.6.7/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-05-04 20:52:12.000000 dspace_stats_collector-0.6.7/docs/installation.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      784 2023-05-04 20:52:12.000000 dspace_stats_collector-0.6.7/docs/make.bat
+-rw-r--r--   0 runner    (1001) docker     (123)    52797 2023-05-04 20:52:12.000000 dspace_stats_collector-0.6.7/docs/pipeline-diagram.png
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-05-04 20:52:12.000000 dspace_stats_collector-0.6.7/docs/readme.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-04 20:52:12.000000 dspace_stats_collector-0.6.7/docs/usage.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 20:52:32.775541 dspace_stats_collector-0.6.7/dspace_stats_collector/
+-rw-r--r--   0 runner    (1001) docker     (123)      405 2023-05-04 20:52:12.000000 dspace_stats_collector-0.6.7/dspace_stats_collector/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7008 2023-05-04 20:52:12.000000 dspace_stats_collector-0.6.7/dspace_stats_collector/collector.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13599 2023-05-04 20:52:12.000000 dspace_stats_collector-0.6.7/dspace_stats_collector/configcontext.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4548 2023-05-04 20:52:12.000000 dspace_stats_collector-0.6.7/dspace_stats_collector/configure.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1690 2023-05-04 20:52:12.000000 dspace_stats_collector-0.6.7/dspace_stats_collector/counterfilter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2309 2023-05-04 20:52:12.000000 dspace_stats_collector-0.6.7/dspace_stats_collector/croninstaller.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4541 2023-05-04 20:52:12.000000 dspace_stats_collector-0.6.7/dspace_stats_collector/dspacedb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2312 2023-05-04 20:52:12.000000 dspace_stats_collector-0.6.7/dspace_stats_collector/dspacedb4.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2528 2023-05-04 20:52:12.000000 dspace_stats_collector-0.6.7/dspace_stats_collector/dspacedb5.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2532 2023-05-04 20:52:12.000000 dspace_stats_collector-0.6.7/dspace_stats_collector/dspacedb5cris.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2496 2023-05-04 20:52:12.000000 dspace_stats_collector-0.6.7/dspace_stats_collector/dspacedb5oracle.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2454 2023-05-04 20:52:12.000000 dspace_stats_collector-0.6.7/dspace_stats_collector/dspacedb6.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2725 2023-05-04 20:52:12.000000 dspace_stats_collector-0.6.7/dspace_stats_collector/dspacedb6oracle.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2454 2023-05-04 20:52:12.000000 dspace_stats_collector-0.6.7/dspace_stats_collector/dspacedb7.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1106 2023-05-04 20:52:12.000000 dspace_stats_collector-0.6.7/dspace_stats_collector/dspacefilter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1214 2023-05-04 20:52:12.000000 dspace_stats_collector-0.6.7/dspace_stats_collector/elasticoutput.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1745 2023-05-04 20:52:12.000000 dspace_stats_collector-0.6.7/dspace_stats_collector/eventpipeline.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9638 2023-05-04 20:52:12.000000 dspace_stats_collector-0.6.7/dspace_stats_collector/matomooutput.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2277 2023-05-04 20:52:12.000000 dspace_stats_collector-0.6.7/dspace_stats_collector/sessionfilter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7079 2023-05-04 20:52:12.000000 dspace_stats_collector-0.6.7/dspace_stats_collector/solrinput.py
+-rw-r--r--   0 runner    (1001) docker     (123)      373 2023-05-04 20:52:12.000000 dspace_stats_collector-0.6.7/dspace_stats_collector/test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 20:52:32.779541 dspace_stats_collector-0.6.7/dspace_stats_collector.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     6046 2023-05-04 20:52:32.000000 dspace_stats_collector-0.6.7/dspace_stats_collector.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2363 2023-05-04 20:52:32.000000 dspace_stats_collector-0.6.7/dspace_stats_collector.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-04 20:52:32.000000 dspace_stats_collector-0.6.7/dspace_stats_collector.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      209 2023-05-04 20:52:32.000000 dspace_stats_collector-0.6.7/dspace_stats_collector.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-04 20:52:32.000000 dspace_stats_collector-0.6.7/dspace_stats_collector.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-04 20:52:32.000000 dspace_stats_collector-0.6.7/dspace_stats_collector.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      464 2023-05-04 20:52:32.783541 dspace_stats_collector-0.6.7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2030 2023-05-04 20:52:12.000000 dspace_stats_collector-0.6.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 20:52:32.779541 dspace_stats_collector-0.6.7/tests/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 20:52:32.783541 dspace_stats_collector-0.6.7/tests/dspace_stats_collector/
+-rw-r--r--   0 runner    (1001) docker     (123)      405 2023-05-04 20:52:12.000000 dspace_stats_collector-0.6.7/tests/dspace_stats_collector/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7008 2023-05-04 20:52:12.000000 dspace_stats_collector-0.6.7/tests/dspace_stats_collector/collector.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13599 2023-05-04 20:52:12.000000 dspace_stats_collector-0.6.7/tests/dspace_stats_collector/configcontext.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4548 2023-05-04 20:52:12.000000 dspace_stats_collector-0.6.7/tests/dspace_stats_collector/configure.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1690 2023-05-04 20:52:12.000000 dspace_stats_collector-0.6.7/tests/dspace_stats_collector/counterfilter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2309 2023-05-04 20:52:12.000000 dspace_stats_collector-0.6.7/tests/dspace_stats_collector/croninstaller.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4541 2023-05-04 20:52:12.000000 dspace_stats_collector-0.6.7/tests/dspace_stats_collector/dspacedb.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2312 2023-05-04 20:52:12.000000 dspace_stats_collector-0.6.7/tests/dspace_stats_collector/dspacedb4.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2528 2023-05-04 20:52:12.000000 dspace_stats_collector-0.6.7/tests/dspace_stats_collector/dspacedb5.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2532 2023-05-04 20:52:12.000000 dspace_stats_collector-0.6.7/tests/dspace_stats_collector/dspacedb5cris.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2496 2023-05-04 20:52:12.000000 dspace_stats_collector-0.6.7/tests/dspace_stats_collector/dspacedb5oracle.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2454 2023-05-04 20:52:12.000000 dspace_stats_collector-0.6.7/tests/dspace_stats_collector/dspacedb6.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2725 2023-05-04 20:52:12.000000 dspace_stats_collector-0.6.7/tests/dspace_stats_collector/dspacedb6oracle.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2454 2023-05-04 20:52:12.000000 dspace_stats_collector-0.6.7/tests/dspace_stats_collector/dspacedb7.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1106 2023-05-04 20:52:12.000000 dspace_stats_collector-0.6.7/tests/dspace_stats_collector/dspacefilter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1214 2023-05-04 20:52:12.000000 dspace_stats_collector-0.6.7/tests/dspace_stats_collector/elasticoutput.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1745 2023-05-04 20:52:12.000000 dspace_stats_collector-0.6.7/tests/dspace_stats_collector/eventpipeline.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9638 2023-05-04 20:52:12.000000 dspace_stats_collector-0.6.7/tests/dspace_stats_collector/matomooutput.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2277 2023-05-04 20:52:12.000000 dspace_stats_collector-0.6.7/tests/dspace_stats_collector/sessionfilter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7079 2023-05-04 20:52:12.000000 dspace_stats_collector-0.6.7/tests/dspace_stats_collector/solrinput.py
+-rw-r--r--   0 runner    (1001) docker     (123)      373 2023-05-04 20:52:12.000000 dspace_stats_collector-0.6.7/tests/dspace_stats_collector/test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      423 2023-05-04 20:52:12.000000 dspace_stats_collector-0.6.7/tests/test_dspace_stats_collector.py
```

### Comparing `dspace_stats_collector-0.6.6/CONTRIBUTING.rst` & `dspace_stats_collector-0.6.7/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `dspace_stats_collector-0.6.6/LICENSE` & `dspace_stats_collector-0.6.7/LICENSE`

 * *Files identical despite different names*

### Comparing `dspace_stats_collector-0.6.6/PKG-INFO` & `dspace_stats_collector-0.6.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dspace_stats_collector
-Version: 0.6.6
+Version: 0.6.7
 Summary: A python library for sending usage stats events from Dspace to Matomo
 Home-page: https://github.com/lareferencia/dspace-stats-collector
 Author: LA Referencia
 Author-email: lareferencia.dev@gmail.com
 License: GNU General Public License v3
 Keywords: dspace_stats_collector
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `dspace_stats_collector-0.6.6/README.rst` & `dspace_stats_collector-0.6.7/README.rst`

 * *Files identical despite different names*

### Comparing `dspace_stats_collector-0.6.6/config/COUNTER_Robots_list.json` & `dspace_stats_collector-0.6.7/config/COUNTER_Robots_list.json`

 * *Files identical despite different names*

### Comparing `dspace_stats_collector-0.6.6/docs/Makefile` & `dspace_stats_collector-0.6.7/docs/Makefile`

 * *Files identical despite different names*

### Comparing `dspace_stats_collector-0.6.6/docs/README_BR.rst` & `dspace_stats_collector-0.6.7/docs/README_BR.rst`

 * *Files identical despite different names*

### Comparing `dspace_stats_collector-0.6.6/docs/conf.py` & `dspace_stats_collector-0.6.7/docs/conf.py`

 * *Files identical despite different names*

### Comparing `dspace_stats_collector-0.6.6/docs/make.bat` & `dspace_stats_collector-0.6.7/docs/make.bat`

 * *Files identical despite different names*

### Comparing `dspace_stats_collector-0.6.6/docs/pipeline-diagram.png` & `dspace_stats_collector-0.6.7/docs/pipeline-diagram.png`

 * *Files identical despite different names*

### Comparing `dspace_stats_collector-0.6.6/dspace_stats_collector/collector.py` & `dspace_stats_collector-0.6.7/dspace_stats_collector/collector.py`

 * *Files identical despite different names*

### Comparing `dspace_stats_collector-0.6.6/dspace_stats_collector/configcontext.py` & `dspace_stats_collector-0.6.7/dspace_stats_collector/configcontext.py`

 * *Files identical despite different names*

### Comparing `dspace_stats_collector-0.6.6/dspace_stats_collector/configure.py` & `dspace_stats_collector-0.6.7/dspace_stats_collector/configure.py`

 * *Files identical despite different names*

### Comparing `dspace_stats_collector-0.6.6/dspace_stats_collector/counterfilter.py` & `dspace_stats_collector-0.6.7/dspace_stats_collector/counterfilter.py`

 * *Files identical despite different names*

### Comparing `dspace_stats_collector-0.6.6/dspace_stats_collector/croninstaller.py` & `dspace_stats_collector-0.6.7/dspace_stats_collector/croninstaller.py`

 * *Files identical despite different names*

### Comparing `dspace_stats_collector-0.6.6/dspace_stats_collector/dspacedb.py` & `dspace_stats_collector-0.6.7/dspace_stats_collector/dspacedb.py`

 * *Files identical despite different names*

### Comparing `dspace_stats_collector-0.6.6/dspace_stats_collector/dspacedb4.py` & `dspace_stats_collector-0.6.7/dspace_stats_collector/dspacedb4.py`

 * *Files identical despite different names*

### Comparing `dspace_stats_collector-0.6.6/dspace_stats_collector/dspacedb5.py` & `dspace_stats_collector-0.6.7/dspace_stats_collector/dspacedb5.py`

 * *Files identical despite different names*

### Comparing `dspace_stats_collector-0.6.6/dspace_stats_collector/dspacedb5cris.py` & `dspace_stats_collector-0.6.7/dspace_stats_collector/dspacedb5cris.py`

 * *Files identical despite different names*

### Comparing `dspace_stats_collector-0.6.6/dspace_stats_collector/dspacedb5oracle.py` & `dspace_stats_collector-0.6.7/dspace_stats_collector/dspacedb5oracle.py`

 * *Files identical despite different names*

### Comparing `dspace_stats_collector-0.6.6/dspace_stats_collector/dspacedb6.py` & `dspace_stats_collector-0.6.7/dspace_stats_collector/dspacedb6.py`

 * *Files identical despite different names*

### Comparing `dspace_stats_collector-0.6.6/dspace_stats_collector/dspacedb6oracle.py` & `dspace_stats_collector-0.6.7/dspace_stats_collector/dspacedb7.py`

 * *Files 9% similar despite different names*

```diff
@@ -6,64 +6,64 @@
 logger = logging.getLogger()
 
 try:
     from .dspacedb import DSpaceDB
 except Exception: #ImportError
     from dspacedb import DSpaceDB
 
-class DSpaceDB6Oracle(DSpaceDB):
+class DSpaceDB7(DSpaceDB):
 
     def __init__(self, jdbcUrl, username, password):
 
         DSpaceDB.__init__(self,jdbcUrl, username, password)
 
         self._queryDownloadSQL = """
             SELECT mv.dspace_object_id::text AS id,
                     mv2.text_value AS record_title,
                     h.handle AS handle,
-                    1 AS is_download,
+                    true AS is_download,
                     i.item_id::text AS owning_item,
                     b.sequence_id AS sequence_id,
                     mv.text_value AS filename
-            FROM metadatavalue mv
-            RIGHT JOIN bitstream b ON mv.dspace_object_id = b.uuid
-            RIGHT JOIN bundle2bitstream bb ON b.uuid = bb.bitstream_id
-            RIGHT JOIN item2bundle i ON i.bundle_id = bb.bundle_id
-            RIGHT JOIN handle h ON h.resource_id = i.item_id
-            RIGHT JOIN metadatavalue mv2 ON mv2.dspace_object_id = i.item_id
+            FROM metadatavalue AS mv
+            RIGHT JOIN bitstream AS b ON mv.dspace_object_id = b.uuid
+            RIGHT JOIN bundle2bitstream AS bb ON b.uuid = bb.bitstream_id
+            RIGHT JOIN item2bundle AS i ON i.bundle_id = bb.bundle_id
+            RIGHT JOIN handle AS h ON h.resource_id = i.item_id
+            RIGHT JOIN metadatavalue AS mv2 ON mv2.dspace_object_id = i.item_id
             WHERE mv.metadata_field_id = {dcTitleId}
                 AND b.sequence_id IS NOT NULL
-                AND b.deleted = 0
+                AND b.deleted = FALSE
                 AND mv2.metadata_field_id = {dcTitleId}
-                AND mv.dspace_object_id = uuid('{bitstreamId}')
+                AND mv.dspace_object_id = uuid('{bitstreamId}');
         """
 
         self._queryItemSQL = """
             SELECT mv.dspace_object_id::text AS id,
                     mv.text_value AS record_title,
                     h.handle AS handle,
-                    0 AS is_download,
+                    false AS is_download,
                     NULL AS owning_item,
                     NULL AS sequence_id,
                     NULL AS filename
-            FROM metadatavalue mv
-            RIGHT JOIN handle h ON h.resource_id = mv.dspace_object_id
+            FROM metadatavalue AS mv
+            RIGHT JOIN handle AS h ON h.resource_id = mv.dspace_object_id
             WHERE metadata_field_id = {dcTitleId}
                 AND h.resource_type_id=2
-                AND mv.dspace_object_id = uuid('{itemId}')
+                AND mv.dspace_object_id = uuid('{itemId}');
         """
       
         self._queryTitleSQL = """
             SELECT metadata_field_id AS "dcTitleId"
                 FROM metadatafieldregistry mfr,
                     metadataschemaregistry msr
                 WHERE mfr.metadata_schema_id = msr.metadata_schema_id
                 AND short_id = 'dc'
                 AND element = 'title'
-                AND qualifier IS NULL
+                AND qualifier IS NULL;
         """
 
         self._dcTitleId = self.getDcTitleId()
```

### Comparing `dspace_stats_collector-0.6.6/dspace_stats_collector/dspacedb7.py` & `dspace_stats_collector-0.6.7/tests/dspace_stats_collector/dspacedb7.py`

 * *Files identical despite different names*

### Comparing `dspace_stats_collector-0.6.6/dspace_stats_collector/dspacefilter.py` & `dspace_stats_collector-0.6.7/dspace_stats_collector/dspacefilter.py`

 * *Files identical despite different names*

### Comparing `dspace_stats_collector-0.6.6/dspace_stats_collector/elasticoutput.py` & `dspace_stats_collector-0.6.7/dspace_stats_collector/elasticoutput.py`

 * *Files identical despite different names*

### Comparing `dspace_stats_collector-0.6.6/dspace_stats_collector/eventpipeline.py` & `dspace_stats_collector-0.6.7/dspace_stats_collector/eventpipeline.py`

 * *Files identical despite different names*

### Comparing `dspace_stats_collector-0.6.6/dspace_stats_collector/matomooutput.py` & `dspace_stats_collector-0.6.7/dspace_stats_collector/matomooutput.py`

 * *Files identical despite different names*

### Comparing `dspace_stats_collector-0.6.6/dspace_stats_collector/sessionfilter.py` & `dspace_stats_collector-0.6.7/dspace_stats_collector/sessionfilter.py`

 * *Files 16% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 
 import logging
 logger = logging.getLogger()
 
 from dateutil import parser as dateutil_parser
 from hashlib import md5
 from anonymizeip import anonymize_ip
+from ipaddress import ip_address
 
 
 class SimpleHashSessionFilter:
 
     FULL_IP_MASK = '255.255.255.255'
 
     def __init__(self, configContext):
@@ -34,13 +35,31 @@
 
             try:
                 # Anonymize IP
                 if self._anonymize_ip_mask != self.FULL_IP_MASK:     
                     event._src['ip'] = anonymize_ip(event._src.get('ip','0.0.0.0'), self._anonymize_ip_mask)    
             
             except Exception as e:
-                logger.error("Error anonymizing IP: {}".format(e))
-                event._src['ip'] = '0.0.0.0'
+
+                 # check if ip is folowing the format ip:port
+                if ':' in event._src.get('ip','0.0.0.0'):
+                    ip, port = ip.split(':')
+                    
+                    ## check the ip string is a valid ip address
+                    try:
+                        # this will raise a ValueError if the ip is not valid
+                        ip_address(ip)
+
+                        # anonymize ip
+                        event._src['ip'] = anonymize_ip(ip, self._anonymize_ip_mask)
+
+                    except ValueError:
+                        logger.error("Error anonymizing parsed IP from XXXX:port pattern: {}".format(e))         
+                        event._src['ip'] = '0.0.0.0'
+                        
+                else:
+                    logger.error("Error anonymizing IP: {}".format(e))
+                    event._src['ip'] = '0.0.0.0'
 
             logger.debug('SESSION_FILTER:: Event: {} Session string: {}'.format(event._id, srcString))
 
             yield event
```

### Comparing `dspace_stats_collector-0.6.6/dspace_stats_collector/solrinput.py` & `dspace_stats_collector-0.6.7/dspace_stats_collector/solrinput.py`

 * *Files identical despite different names*

### Comparing `dspace_stats_collector-0.6.6/dspace_stats_collector.egg-info/PKG-INFO` & `dspace_stats_collector-0.6.7/dspace_stats_collector.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dspace-stats-collector
-Version: 0.6.6
+Version: 0.6.7
 Summary: A python library for sending usage stats events from Dspace to Matomo
 Home-page: https://github.com/lareferencia/dspace-stats-collector
 Author: LA Referencia
 Author-email: lareferencia.dev@gmail.com
 License: GNU General Public License v3
 Keywords: dspace_stats_collector
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
```

### Comparing `dspace_stats_collector-0.6.6/dspace_stats_collector.egg-info/SOURCES.txt` & `dspace_stats_collector-0.6.7/dspace_stats_collector.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dspace_stats_collector-0.6.6/setup.py` & `dspace_stats_collector-0.6.7/setup.py`

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
-    version='0.6.6',
+    version='0.6.7',
     zip_safe=False,
 )
```

### Comparing `dspace_stats_collector-0.6.6/tests/dspace_stats_collector/collector.py` & `dspace_stats_collector-0.6.7/tests/dspace_stats_collector/collector.py`

 * *Files identical despite different names*

### Comparing `dspace_stats_collector-0.6.6/tests/dspace_stats_collector/configcontext.py` & `dspace_stats_collector-0.6.7/tests/dspace_stats_collector/configcontext.py`

 * *Files identical despite different names*

### Comparing `dspace_stats_collector-0.6.6/tests/dspace_stats_collector/configure.py` & `dspace_stats_collector-0.6.7/tests/dspace_stats_collector/configure.py`

 * *Files identical despite different names*

### Comparing `dspace_stats_collector-0.6.6/tests/dspace_stats_collector/counterfilter.py` & `dspace_stats_collector-0.6.7/tests/dspace_stats_collector/counterfilter.py`

 * *Files identical despite different names*

### Comparing `dspace_stats_collector-0.6.6/tests/dspace_stats_collector/croninstaller.py` & `dspace_stats_collector-0.6.7/tests/dspace_stats_collector/croninstaller.py`

 * *Files identical despite different names*

### Comparing `dspace_stats_collector-0.6.6/tests/dspace_stats_collector/dspacedb.py` & `dspace_stats_collector-0.6.7/tests/dspace_stats_collector/dspacedb.py`

 * *Files identical despite different names*

### Comparing `dspace_stats_collector-0.6.6/tests/dspace_stats_collector/dspacedb4.py` & `dspace_stats_collector-0.6.7/tests/dspace_stats_collector/dspacedb4.py`

 * *Files identical despite different names*

### Comparing `dspace_stats_collector-0.6.6/tests/dspace_stats_collector/dspacedb5.py` & `dspace_stats_collector-0.6.7/tests/dspace_stats_collector/dspacedb5.py`

 * *Files identical despite different names*

### Comparing `dspace_stats_collector-0.6.6/tests/dspace_stats_collector/dspacedb5cris.py` & `dspace_stats_collector-0.6.7/tests/dspace_stats_collector/dspacedb5cris.py`

 * *Files identical despite different names*

### Comparing `dspace_stats_collector-0.6.6/tests/dspace_stats_collector/dspacedb5oracle.py` & `dspace_stats_collector-0.6.7/tests/dspace_stats_collector/dspacedb5oracle.py`

 * *Files identical despite different names*

### Comparing `dspace_stats_collector-0.6.6/tests/dspace_stats_collector/dspacedb6.py` & `dspace_stats_collector-0.6.7/tests/dspace_stats_collector/dspacedb6.py`

 * *Files identical despite different names*

### Comparing `dspace_stats_collector-0.6.6/tests/dspace_stats_collector/dspacedb6oracle.py` & `dspace_stats_collector-0.6.7/dspace_stats_collector/dspacedb6oracle.py`

 * *Files 20% similar despite different names*

```diff
@@ -13,57 +13,54 @@
 class DSpaceDB6Oracle(DSpaceDB):
 
     def __init__(self, jdbcUrl, username, password):
 
         DSpaceDB.__init__(self,jdbcUrl, username, password)
 
         self._queryDownloadSQL = """
-            SELECT mv.dspace_object_id::text AS id,
+            SELECT regexp_replace(lower(mv.dspace_object_id), '(........)(....)(....)(....)(.*)', '\\1-\\2-\\3-\\4-\\5') AS id,            
                     mv2.text_value AS record_title,
                     h.handle AS handle,
                     1 AS is_download,
-                    i.item_id::text AS owning_item,
+                    regexp_replace(lower(i.item_id), '(........)(....)(....)(....)(.*)', '\\1-\\2-\\3-\\4-\\5') AS owning_item,                    
                     b.sequence_id AS sequence_id,
                     mv.text_value AS filename
             FROM metadatavalue mv
-            RIGHT JOIN bitstream b ON mv.dspace_object_id = b.uuid
-            RIGHT JOIN bundle2bitstream bb ON b.uuid = bb.bitstream_id
-            RIGHT JOIN item2bundle i ON i.bundle_id = bb.bundle_id
-            RIGHT JOIN handle h ON h.resource_id = i.item_id
-            RIGHT JOIN metadatavalue mv2 ON mv2.dspace_object_id = i.item_id
+            INNER JOIN bitstream b ON mv.dspace_object_id = b.uuid
+            INNER JOIN bundle2bitstream bb ON b.uuid = bb.bitstream_id
+            INNER JOIN item2bundle i ON i.bundle_id = bb.bundle_id
+            INNER JOIN handle h ON h.resource_id = i.item_id
+            INNER JOIN metadatavalue mv2 ON mv2.dspace_object_id = i.item_id
             WHERE mv.metadata_field_id = {dcTitleId}
                 AND b.sequence_id IS NOT NULL
                 AND b.deleted = 0
                 AND mv2.metadata_field_id = {dcTitleId}
-                AND mv.dspace_object_id = uuid('{bitstreamId}')
+                AND mv.dspace_object_id = upper(replace('{bitstreamId}','-',''))
         """
 
         self._queryItemSQL = """
-            SELECT mv.dspace_object_id::text AS id,
+            SELECT regexp_replace(lower(mv.dspace_object_id), '(........)(....)(....)(....)(.*)', '\\1-\\2-\\3-\\4-\\5') AS id,            
                     mv.text_value AS record_title,
                     h.handle AS handle,
                     0 AS is_download,
                     NULL AS owning_item,
                     NULL AS sequence_id,
                     NULL AS filename
             FROM metadatavalue mv
-            RIGHT JOIN handle h ON h.resource_id = mv.dspace_object_id
+            INNER JOIN handle h ON h.resource_id = mv.dspace_object_id
             WHERE metadata_field_id = {dcTitleId}
                 AND h.resource_type_id=2
-                AND mv.dspace_object_id = uuid('{itemId}')
+                AND mv.dspace_object_id = upper(replace('{itemId}','-',''))
         """
       
         self._queryTitleSQL = """
             SELECT metadata_field_id AS "dcTitleId"
                 FROM metadatafieldregistry mfr,
                     metadataschemaregistry msr
                 WHERE mfr.metadata_schema_id = msr.metadata_schema_id
                 AND short_id = 'dc'
                 AND element = 'title'
                 AND qualifier IS NULL
         """
 
         self._dcTitleId = self.getDcTitleId()
-
-
-
```

### Comparing `dspace_stats_collector-0.6.6/tests/dspace_stats_collector/dspacefilter.py` & `dspace_stats_collector-0.6.7/tests/dspace_stats_collector/dspacefilter.py`

 * *Files identical despite different names*

### Comparing `dspace_stats_collector-0.6.6/tests/dspace_stats_collector/elasticoutput.py` & `dspace_stats_collector-0.6.7/tests/dspace_stats_collector/elasticoutput.py`

 * *Files identical despite different names*

### Comparing `dspace_stats_collector-0.6.6/tests/dspace_stats_collector/eventpipeline.py` & `dspace_stats_collector-0.6.7/tests/dspace_stats_collector/eventpipeline.py`

 * *Files identical despite different names*

### Comparing `dspace_stats_collector-0.6.6/tests/dspace_stats_collector/matomooutput.py` & `dspace_stats_collector-0.6.7/tests/dspace_stats_collector/matomooutput.py`

 * *Files identical despite different names*

### Comparing `dspace_stats_collector-0.6.6/tests/dspace_stats_collector/sessionfilter.py` & `dspace_stats_collector-0.6.7/tests/dspace_stats_collector/sessionfilter.py`

 * *Files 16% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 
 import logging
 logger = logging.getLogger()
 
 from dateutil import parser as dateutil_parser
 from hashlib import md5
 from anonymizeip import anonymize_ip
+from ipaddress import ip_address
 
 
 class SimpleHashSessionFilter:
 
     FULL_IP_MASK = '255.255.255.255'
 
     def __init__(self, configContext):
@@ -34,13 +35,31 @@
 
             try:
                 # Anonymize IP
                 if self._anonymize_ip_mask != self.FULL_IP_MASK:     
                     event._src['ip'] = anonymize_ip(event._src.get('ip','0.0.0.0'), self._anonymize_ip_mask)    
             
             except Exception as e:
-                logger.error("Error anonymizing IP: {}".format(e))
-                event._src['ip'] = '0.0.0.0'
+
+                 # check if ip is folowing the format ip:port
+                if ':' in event._src.get('ip','0.0.0.0'):
+                    ip, port = ip.split(':')
+                    
+                    ## check the ip string is a valid ip address
+                    try:
+                        # this will raise a ValueError if the ip is not valid
+                        ip_address(ip)
+
+                        # anonymize ip
+                        event._src['ip'] = anonymize_ip(ip, self._anonymize_ip_mask)
+
+                    except ValueError:
+                        logger.error("Error anonymizing parsed IP from XXXX:port pattern: {}".format(e))         
+                        event._src['ip'] = '0.0.0.0'
+                        
+                else:
+                    logger.error("Error anonymizing IP: {}".format(e))
+                    event._src['ip'] = '0.0.0.0'
 
             logger.debug('SESSION_FILTER:: Event: {} Session string: {}'.format(event._id, srcString))
 
             yield event
```

### Comparing `dspace_stats_collector-0.6.6/tests/dspace_stats_collector/solrinput.py` & `dspace_stats_collector-0.6.7/tests/dspace_stats_collector/solrinput.py`

 * *Files identical despite different names*

