# Comparing `tmp/UW-RestClients-HRP-1.3.1.1.tar.gz` & `tmp/UW-RestClients-HRP-1.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "UW-RestClients-HRP-1.3.1.1.tar", last modified: Sat Jan  7 00:42:43 2023, max compression
+gzip compressed data, was "UW-RestClients-HRP-1.3.2.tar", last modified: Thu May  4 22:01:06 2023, max compression
```

## Comparing `UW-RestClients-HRP-1.3.1.1.tar` & `UW-RestClients-HRP-1.3.2.tar`

### file list

```diff
@@ -1,54 +1,54 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-07 00:42:43.375649 UW-RestClients-HRP-1.3.1.1/
--rw-r--r--   0 runner    (1001) docker     (122)    11357 2023-01-07 00:42:35.000000 UW-RestClients-HRP-1.3.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)       50 2023-01-07 00:42:35.000000 UW-RestClients-HRP-1.3.1.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)      654 2023-01-07 00:42:43.375649 UW-RestClients-HRP-1.3.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      895 2023-01-07 00:42:35.000000 UW-RestClients-HRP-1.3.1.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-07 00:42:43.375649 UW-RestClients-HRP-1.3.1.1/UW_RestClients_HRP.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)      654 2023-01-07 00:42:43.000000 UW-RestClients-HRP-1.3.1.1/UW_RestClients_HRP.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     1808 2023-01-07 00:42:43.000000 UW-RestClients-HRP-1.3.1.1/UW_RestClients_HRP.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-01-07 00:42:43.000000 UW-RestClients-HRP-1.3.1.1/UW_RestClients_HRP.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)       36 2023-01-07 00:42:43.000000 UW-RestClients-HRP-1.3.1.1/UW_RestClients_HRP.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)        7 2023-01-07 00:42:43.000000 UW-RestClients-HRP-1.3.1.1/UW_RestClients_HRP.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-01-07 00:42:43.375649 UW-RestClients-HRP-1.3.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     1229 2023-01-07 00:42:35.000000 UW-RestClients-HRP-1.3.1.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-07 00:42:43.375649 UW-RestClients-HRP-1.3.1.1/uw_hrp/
--rw-r--r--   0 runner    (1001) docker     (122)        8 2023-01-07 00:42:42.000000 UW-RestClients-HRP-1.3.1.1/uw_hrp/VERSION
--rw-r--r--   0 runner    (1001) docker     (122)     3652 2023-01-07 00:42:35.000000 UW-RestClients-HRP-1.3.1.1/uw_hrp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      452 2023-01-07 00:42:35.000000 UW-RestClients-HRP-1.3.1.1/uw_hrp/dao.py
--rw-r--r--   0 runner    (1001) docker     (122)    11424 2023-01-07 00:42:35.000000 UW-RestClients-HRP-1.3.1.1/uw_hrp/models.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-07 00:42:43.371649 UW-RestClients-HRP-1.3.1.1/uw_hrp/resources/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-07 00:42:43.371649 UW-RestClients-HRP-1.3.1.1/uw_hrp/resources/hrpws/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-07 00:42:43.371649 UW-RestClients-HRP-1.3.1.1/uw_hrp/resources/hrpws/file/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-07 00:42:43.371649 UW-RestClients-HRP-1.3.1.1/uw_hrp/resources/hrpws/file/hrp/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-07 00:42:43.371649 UW-RestClients-HRP-1.3.1.1/uw_hrp/resources/hrpws/file/hrp/v1/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-07 00:42:43.375649 UW-RestClients-HRP-1.3.1.1/uw_hrp/resources/hrpws/file/hrp/v1/appointee/
--rw-r--r--   0 runner    (1001) docker     (122)     4837 2023-01-07 00:42:35.000000 UW-RestClients-HRP-1.3.1.1/uw_hrp/resources/hrpws/file/hrp/v1/appointee/123456789.json
--rw-r--r--   0 runner    (1001) docker     (122)     4837 2023-01-07 00:42:35.000000 UW-RestClients-HRP-1.3.1.1/uw_hrp/resources/hrpws/file/hrp/v1/appointee/9136CCB8F66711D5BE060004AC494FFE.json
--rw-r--r--   0 runner    (1001) docker     (122)     4837 2023-01-07 00:42:35.000000 UW-RestClients-HRP-1.3.1.1/uw_hrp/resources/hrpws/file/hrp/v1/appointee/javerage.json
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-07 00:42:43.375649 UW-RestClients-HRP-1.3.1.1/uw_hrp/resources/hrpws/file/hrp/v2/
--rw-r--r--   0 runner    (1001) docker     (122)      358 2023-01-07 00:42:35.000000 UW-RestClients-HRP-1.3.1.1/uw_hrp/resources/hrpws/file/hrp/v2/Worker.json_changed_since_2019_page_size_200_page_start_2
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-07 00:42:43.375649 UW-RestClients-HRP-1.3.1.1/uw_hrp/resources/hrpws/file/hrp/v2/worker/
--rw-r--r--   0 runner    (1001) docker     (122)    10331 2023-01-07 00:42:35.000000 UW-RestClients-HRP-1.3.1.1/uw_hrp/resources/hrpws/file/hrp/v2/worker/10000000000000000000000000000015.json
--rw-r--r--   0 runner    (1001) docker     (122)    10331 2023-01-07 00:42:35.000000 UW-RestClients-HRP-1.3.1.1/uw_hrp/resources/hrpws/file/hrp/v2/worker/10000000000000000000000000000015.json_workerpositionstate_current_future
--rw-r--r--   0 runner    (1001) docker     (122)    10331 2023-01-07 00:42:35.000000 UW-RestClients-HRP-1.3.1.1/uw_hrp/resources/hrpws/file/hrp/v2/worker/100000015.json
--rw-r--r--   0 runner    (1001) docker     (122)    10331 2023-01-07 00:42:35.000000 UW-RestClients-HRP-1.3.1.1/uw_hrp/resources/hrpws/file/hrp/v2/worker/100000015.json_workerpositionstate_current_future
--rw-r--r--   0 runner    (1001) docker     (122)    10331 2023-01-07 00:42:35.000000 UW-RestClients-HRP-1.3.1.1/uw_hrp/resources/hrpws/file/hrp/v2/worker/chair.json
--rw-r--r--   0 runner    (1001) docker     (122)     8018 2023-01-07 00:42:35.000000 UW-RestClients-HRP-1.3.1.1/uw_hrp/resources/hrpws/file/hrp/v2/worker/faculty.json
--rw-r--r--   0 runner    (1001) docker     (122)     8018 2023-01-07 00:42:35.000000 UW-RestClients-HRP-1.3.1.1/uw_hrp/resources/hrpws/file/hrp/v2/worker/faculty.json_workerpositionstate_current_future
--rw-r--r--   0 runner    (1001) docker     (122)      422 2023-01-07 00:42:35.000000 UW-RestClients-HRP-1.3.1.1/uw_hrp/resources/hrpws/file/hrp/v2/worker.json_changed_since_2019_page_size_200
--rw-r--r--   0 runner    (1001) docker     (122)       61 2023-01-07 00:42:35.000000 UW-RestClients-HRP-1.3.1.1/uw_hrp/resources/hrpws/file/hrp/v2/worker.json_changed_since_2020_page_size_200
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-07 00:42:43.375649 UW-RestClients-HRP-1.3.1.1/uw_hrp/resources/hrpws/file/hrp/v3/
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-07 00:42:43.375649 UW-RestClients-HRP-1.3.1.1/uw_hrp/resources/hrpws/file/hrp/v3/person/
--rw-r--r--   0 runner    (1001) docker     (122)    40857 2023-01-07 00:42:35.000000 UW-RestClients-HRP-1.3.1.1/uw_hrp/resources/hrpws/file/hrp/v3/person/000000005.json
--rw-r--r--   0 runner    (1001) docker     (122)    44463 2023-01-07 00:42:35.000000 UW-RestClients-HRP-1.3.1.1/uw_hrp/resources/hrpws/file/hrp/v3/person/9136CCB8F66711D5BE060004AC494FFE.json
--rw-r--r--   0 runner    (1001) docker     (122)    40857 2023-01-07 00:42:35.000000 UW-RestClients-HRP-1.3.1.1/uw_hrp/resources/hrpws/file/hrp/v3/person/faculty.json
--rw-r--r--   0 runner    (1001) docker     (122)    40857 2023-01-07 00:42:35.000000 UW-RestClients-HRP-1.3.1.1/uw_hrp/resources/hrpws/file/hrp/v3/person/faculty.json_future_worker_true
--rw-r--r--   0 runner    (1001) docker     (122)    27656 2023-01-07 00:42:35.000000 UW-RestClients-HRP-1.3.1.1/uw_hrp/resources/hrpws/file/hrp/v3/person.json_changed_since_date_2022-12-12_page_size_200
--rw-r--r--   0 runner    (1001) docker     (122)      463 2023-01-07 00:42:35.000000 UW-RestClients-HRP-1.3.1.1/uw_hrp/test.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-07 00:42:43.375649 UW-RestClients-HRP-1.3.1.1/uw_hrp/tests/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-01-07 00:42:35.000000 UW-RestClients-HRP-1.3.1.1/uw_hrp/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)      388 2023-01-07 00:42:35.000000 UW-RestClients-HRP-1.3.1.1/uw_hrp/tests/test_dao.py
--rw-r--r--   0 runner    (1001) docker     (122)     5019 2023-01-07 00:42:35.000000 UW-RestClients-HRP-1.3.1.1/uw_hrp/tests/test_hrp.py
--rw-r--r--   0 runner    (1001) docker     (122)    14599 2023-01-07 00:42:35.000000 UW-RestClients-HRP-1.3.1.1/uw_hrp/tests/test_models.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-01-07 00:42:43.375649 UW-RestClients-HRP-1.3.1.1/uw_hrp/util/
--rw-r--r--   0 runner    (1001) docker     (122)      215 2023-01-07 00:42:35.000000 UW-RestClients-HRP-1.3.1.1/uw_hrp/util/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-04 22:01:06.160029 UW-RestClients-HRP-1.3.2/
+-rw-r--r--   0 runner    (1001) docker     (122)    11357 2023-05-04 22:00:51.000000 UW-RestClients-HRP-1.3.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)       50 2023-05-04 22:00:51.000000 UW-RestClients-HRP-1.3.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)      652 2023-05-04 22:01:06.160029 UW-RestClients-HRP-1.3.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      895 2023-05-04 22:00:51.000000 UW-RestClients-HRP-1.3.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-04 22:01:06.160029 UW-RestClients-HRP-1.3.2/UW_RestClients_HRP.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)      652 2023-05-04 22:01:05.000000 UW-RestClients-HRP-1.3.2/UW_RestClients_HRP.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     1808 2023-05-04 22:01:06.000000 UW-RestClients-HRP-1.3.2/UW_RestClients_HRP.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-04 22:01:05.000000 UW-RestClients-HRP-1.3.2/UW_RestClients_HRP.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       36 2023-05-04 22:01:05.000000 UW-RestClients-HRP-1.3.2/UW_RestClients_HRP.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        7 2023-05-04 22:01:05.000000 UW-RestClients-HRP-1.3.2/UW_RestClients_HRP.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-05-04 22:01:06.160029 UW-RestClients-HRP-1.3.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     1229 2023-05-04 22:00:51.000000 UW-RestClients-HRP-1.3.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-04 22:01:06.160029 UW-RestClients-HRP-1.3.2/uw_hrp/
+-rw-r--r--   0 runner    (1001) docker     (122)        6 2023-05-04 22:01:04.000000 UW-RestClients-HRP-1.3.2/uw_hrp/VERSION
+-rw-r--r--   0 runner    (1001) docker     (122)     3652 2023-05-04 22:00:51.000000 UW-RestClients-HRP-1.3.2/uw_hrp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      452 2023-05-04 22:00:51.000000 UW-RestClients-HRP-1.3.2/uw_hrp/dao.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11430 2023-05-04 22:00:51.000000 UW-RestClients-HRP-1.3.2/uw_hrp/models.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-04 22:01:06.156029 UW-RestClients-HRP-1.3.2/uw_hrp/resources/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-04 22:01:06.156029 UW-RestClients-HRP-1.3.2/uw_hrp/resources/hrpws/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-04 22:01:06.156029 UW-RestClients-HRP-1.3.2/uw_hrp/resources/hrpws/file/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-04 22:01:06.156029 UW-RestClients-HRP-1.3.2/uw_hrp/resources/hrpws/file/hrp/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-04 22:01:06.156029 UW-RestClients-HRP-1.3.2/uw_hrp/resources/hrpws/file/hrp/v1/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-04 22:01:06.160029 UW-RestClients-HRP-1.3.2/uw_hrp/resources/hrpws/file/hrp/v1/appointee/
+-rw-r--r--   0 runner    (1001) docker     (122)     4837 2023-05-04 22:00:51.000000 UW-RestClients-HRP-1.3.2/uw_hrp/resources/hrpws/file/hrp/v1/appointee/123456789.json
+-rw-r--r--   0 runner    (1001) docker     (122)     4837 2023-05-04 22:00:51.000000 UW-RestClients-HRP-1.3.2/uw_hrp/resources/hrpws/file/hrp/v1/appointee/9136CCB8F66711D5BE060004AC494FFE.json
+-rw-r--r--   0 runner    (1001) docker     (122)     4837 2023-05-04 22:00:51.000000 UW-RestClients-HRP-1.3.2/uw_hrp/resources/hrpws/file/hrp/v1/appointee/javerage.json
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-04 22:01:06.160029 UW-RestClients-HRP-1.3.2/uw_hrp/resources/hrpws/file/hrp/v2/
+-rw-r--r--   0 runner    (1001) docker     (122)      358 2023-05-04 22:00:51.000000 UW-RestClients-HRP-1.3.2/uw_hrp/resources/hrpws/file/hrp/v2/Worker.json_changed_since_2019_page_size_200_page_start_2
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-04 22:01:06.160029 UW-RestClients-HRP-1.3.2/uw_hrp/resources/hrpws/file/hrp/v2/worker/
+-rw-r--r--   0 runner    (1001) docker     (122)    10331 2023-05-04 22:00:51.000000 UW-RestClients-HRP-1.3.2/uw_hrp/resources/hrpws/file/hrp/v2/worker/10000000000000000000000000000015.json
+-rw-r--r--   0 runner    (1001) docker     (122)    10331 2023-05-04 22:00:51.000000 UW-RestClients-HRP-1.3.2/uw_hrp/resources/hrpws/file/hrp/v2/worker/10000000000000000000000000000015.json_workerpositionstate_current_future
+-rw-r--r--   0 runner    (1001) docker     (122)    10331 2023-05-04 22:00:51.000000 UW-RestClients-HRP-1.3.2/uw_hrp/resources/hrpws/file/hrp/v2/worker/100000015.json
+-rw-r--r--   0 runner    (1001) docker     (122)    10331 2023-05-04 22:00:51.000000 UW-RestClients-HRP-1.3.2/uw_hrp/resources/hrpws/file/hrp/v2/worker/100000015.json_workerpositionstate_current_future
+-rw-r--r--   0 runner    (1001) docker     (122)    10331 2023-05-04 22:00:51.000000 UW-RestClients-HRP-1.3.2/uw_hrp/resources/hrpws/file/hrp/v2/worker/chair.json
+-rw-r--r--   0 runner    (1001) docker     (122)     8018 2023-05-04 22:00:51.000000 UW-RestClients-HRP-1.3.2/uw_hrp/resources/hrpws/file/hrp/v2/worker/faculty.json
+-rw-r--r--   0 runner    (1001) docker     (122)     8018 2023-05-04 22:00:51.000000 UW-RestClients-HRP-1.3.2/uw_hrp/resources/hrpws/file/hrp/v2/worker/faculty.json_workerpositionstate_current_future
+-rw-r--r--   0 runner    (1001) docker     (122)      422 2023-05-04 22:00:51.000000 UW-RestClients-HRP-1.3.2/uw_hrp/resources/hrpws/file/hrp/v2/worker.json_changed_since_2019_page_size_200
+-rw-r--r--   0 runner    (1001) docker     (122)       61 2023-05-04 22:00:51.000000 UW-RestClients-HRP-1.3.2/uw_hrp/resources/hrpws/file/hrp/v2/worker.json_changed_since_2020_page_size_200
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-04 22:01:06.160029 UW-RestClients-HRP-1.3.2/uw_hrp/resources/hrpws/file/hrp/v3/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-04 22:01:06.160029 UW-RestClients-HRP-1.3.2/uw_hrp/resources/hrpws/file/hrp/v3/person/
+-rw-r--r--   0 runner    (1001) docker     (122)    40857 2023-05-04 22:00:51.000000 UW-RestClients-HRP-1.3.2/uw_hrp/resources/hrpws/file/hrp/v3/person/000000005.json
+-rw-r--r--   0 runner    (1001) docker     (122)    44463 2023-05-04 22:00:51.000000 UW-RestClients-HRP-1.3.2/uw_hrp/resources/hrpws/file/hrp/v3/person/9136CCB8F66711D5BE060004AC494FFE.json
+-rw-r--r--   0 runner    (1001) docker     (122)    40857 2023-05-04 22:00:51.000000 UW-RestClients-HRP-1.3.2/uw_hrp/resources/hrpws/file/hrp/v3/person/faculty.json
+-rw-r--r--   0 runner    (1001) docker     (122)    40857 2023-05-04 22:00:51.000000 UW-RestClients-HRP-1.3.2/uw_hrp/resources/hrpws/file/hrp/v3/person/faculty.json_future_worker_true
+-rw-r--r--   0 runner    (1001) docker     (122)    27656 2023-05-04 22:00:51.000000 UW-RestClients-HRP-1.3.2/uw_hrp/resources/hrpws/file/hrp/v3/person.json_changed_since_date_2022-12-12_page_size_200
+-rw-r--r--   0 runner    (1001) docker     (122)      463 2023-05-04 22:00:51.000000 UW-RestClients-HRP-1.3.2/uw_hrp/test.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-04 22:01:06.160029 UW-RestClients-HRP-1.3.2/uw_hrp/tests/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-04 22:00:51.000000 UW-RestClients-HRP-1.3.2/uw_hrp/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      388 2023-05-04 22:00:51.000000 UW-RestClients-HRP-1.3.2/uw_hrp/tests/test_dao.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5019 2023-05-04 22:00:51.000000 UW-RestClients-HRP-1.3.2/uw_hrp/tests/test_hrp.py
+-rw-r--r--   0 runner    (1001) docker     (122)    14785 2023-05-04 22:00:51.000000 UW-RestClients-HRP-1.3.2/uw_hrp/tests/test_models.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-04 22:01:06.160029 UW-RestClients-HRP-1.3.2/uw_hrp/util/
+-rw-r--r--   0 runner    (1001) docker     (122)      215 2023-05-04 22:00:51.000000 UW-RestClients-HRP-1.3.2/uw_hrp/util/__init__.py
```

### Comparing `UW-RestClients-HRP-1.3.1.1/LICENSE` & `UW-RestClients-HRP-1.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `UW-RestClients-HRP-1.3.1.1/PKG-INFO` & `UW-RestClients-HRP-1.3.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: UW-RestClients-HRP
-Version: 1.3.1.1
+Version: 1.3.2
 Summary: A library for connecting to the UW Human Resources API
 Home-page: https://github.com/uw-it-aca/uw-restclients-hrp
 Author: UW-IT AXDD
 Author-email: aca-it@uw.edu
 License: Apache License, Version 2.0
 Description: 
         See the README on `GitHub
```

### Comparing `UW-RestClients-HRP-1.3.1.1/README.md` & `UW-RestClients-HRP-1.3.2/README.md`

 * *Files identical despite different names*

### Comparing `UW-RestClients-HRP-1.3.1.1/UW_RestClients_HRP.egg-info/PKG-INFO` & `UW-RestClients-HRP-1.3.2/UW_RestClients_HRP.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: UW-RestClients-HRP
-Version: 1.3.1.1
+Version: 1.3.2
 Summary: A library for connecting to the UW Human Resources API
 Home-page: https://github.com/uw-it-aca/uw-restclients-hrp
 Author: UW-IT AXDD
 Author-email: aca-it@uw.edu
 License: Apache License, Version 2.0
 Description: 
         See the README on `GitHub
```

### Comparing `UW-RestClients-HRP-1.3.1.1/UW_RestClients_HRP.egg-info/SOURCES.txt` & `UW-RestClients-HRP-1.3.2/UW_RestClients_HRP.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `UW-RestClients-HRP-1.3.1.1/setup.py` & `UW-RestClients-HRP-1.3.2/setup.py`

 * *Files identical despite different names*

### Comparing `UW-RestClients-HRP-1.3.1.1/uw_hrp/__init__.py` & `UW-RestClients-HRP-1.3.2/uw_hrp/__init__.py`

 * *Files identical despite different names*

### Comparing `UW-RestClients-HRP-1.3.1.1/uw_hrp/models.py` & `UW-RestClients-HRP-1.3.2/uw_hrp/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -31,19 +31,22 @@
                     emp_program_name = emp_program_name.split(" - ", 1)[1]
                 if " (" in emp_program_name:
                     emp_program_name = emp_program_name.split(" (", 1)[0]
                 return emp_program_name.strip()
 
 
 def get_org_code_name(organization_name):
-    if organization_name and ": " in organization_name:
+    org_code = ""
+    org_name = organization_name
+    if ": " in organization_name:
         (org_code, org_name) = organization_name.split(": ", 1)
-        if " (" in org_name:
-            org_name = org_name.split(" (", 1)[0]
-        return org_code.strip(), org_name.strip()
+
+    if " (" in org_name:
+        org_name = org_name.split(" (", 1)[0]
+    return org_code.strip(), org_name.strip()
 
 
 class EmploymentStatus(models.Model):
     status = models.CharField(max_length=32)
     is_active = models.BooleanField(default=False)
     is_retired = models.BooleanField(default=False)
     is_terminated = models.BooleanField(default=False)
@@ -176,15 +179,15 @@
         if data.get("PositionWorkerType") is not None:
             self.pos_type = data["PositionWorkerType"].get("Name")
 
         self.is_primary = data.get("PrimaryPosition")
         self.end_date = parse_date(data.get("PositionVacateDate"))
         self.start_date = parse_date(data.get("StartDate"))
 
-        if (data.get("SupervisoryOrganization") is not None and
+        if (data.get("SupervisoryOrganization") and
                 data["SupervisoryOrganization"].get("Name") is not None):
             self.org_code, self.org_name = get_org_code_name(
                 data["SupervisoryOrganization"]["Name"])
 
 
 class WorkerDetails(models.Model):
     worker_wid = models.CharField(max_length=32)
```

### Comparing `UW-RestClients-HRP-1.3.1.1/uw_hrp/resources/hrpws/file/hrp/v1/appointee/123456789.json` & `UW-RestClients-HRP-1.3.2/uw_hrp/resources/hrpws/file/hrp/v1/appointee/123456789.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-HRP-1.3.1.1/uw_hrp/resources/hrpws/file/hrp/v1/appointee/9136CCB8F66711D5BE060004AC494FFE.json` & `UW-RestClients-HRP-1.3.2/uw_hrp/resources/hrpws/file/hrp/v1/appointee/9136CCB8F66711D5BE060004AC494FFE.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-HRP-1.3.1.1/uw_hrp/resources/hrpws/file/hrp/v1/appointee/javerage.json` & `UW-RestClients-HRP-1.3.2/uw_hrp/resources/hrpws/file/hrp/v1/appointee/javerage.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-HRP-1.3.1.1/uw_hrp/resources/hrpws/file/hrp/v2/worker/10000000000000000000000000000015.json` & `UW-RestClients-HRP-1.3.2/uw_hrp/resources/hrpws/file/hrp/v2/worker/10000000000000000000000000000015.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-HRP-1.3.1.1/uw_hrp/resources/hrpws/file/hrp/v2/worker/10000000000000000000000000000015.json_workerpositionstate_current_future` & `UW-RestClients-HRP-1.3.2/uw_hrp/resources/hrpws/file/hrp/v2/worker/10000000000000000000000000000015.json_workerpositionstate_current_future`

 * *Files identical despite different names*

### Comparing `UW-RestClients-HRP-1.3.1.1/uw_hrp/resources/hrpws/file/hrp/v2/worker/100000015.json` & `UW-RestClients-HRP-1.3.2/uw_hrp/resources/hrpws/file/hrp/v2/worker/100000015.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-HRP-1.3.1.1/uw_hrp/resources/hrpws/file/hrp/v2/worker/100000015.json_workerpositionstate_current_future` & `UW-RestClients-HRP-1.3.2/uw_hrp/resources/hrpws/file/hrp/v2/worker/100000015.json_workerpositionstate_current_future`

 * *Files identical despite different names*

### Comparing `UW-RestClients-HRP-1.3.1.1/uw_hrp/resources/hrpws/file/hrp/v2/worker/chair.json` & `UW-RestClients-HRP-1.3.2/uw_hrp/resources/hrpws/file/hrp/v2/worker/chair.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-HRP-1.3.1.1/uw_hrp/resources/hrpws/file/hrp/v2/worker/faculty.json` & `UW-RestClients-HRP-1.3.2/uw_hrp/resources/hrpws/file/hrp/v2/worker/faculty.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-HRP-1.3.1.1/uw_hrp/resources/hrpws/file/hrp/v2/worker/faculty.json_workerpositionstate_current_future` & `UW-RestClients-HRP-1.3.2/uw_hrp/resources/hrpws/file/hrp/v2/worker/faculty.json_workerpositionstate_current_future`

 * *Files identical despite different names*

### Comparing `UW-RestClients-HRP-1.3.1.1/uw_hrp/resources/hrpws/file/hrp/v3/person/000000005.json` & `UW-RestClients-HRP-1.3.2/uw_hrp/resources/hrpws/file/hrp/v3/person/000000005.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-HRP-1.3.1.1/uw_hrp/resources/hrpws/file/hrp/v3/person/9136CCB8F66711D5BE060004AC494FFE.json` & `UW-RestClients-HRP-1.3.2/uw_hrp/resources/hrpws/file/hrp/v3/person/9136CCB8F66711D5BE060004AC494FFE.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-HRP-1.3.1.1/uw_hrp/resources/hrpws/file/hrp/v3/person/faculty.json` & `UW-RestClients-HRP-1.3.2/uw_hrp/resources/hrpws/file/hrp/v3/person/faculty.json`

 * *Files identical despite different names*

### Comparing `UW-RestClients-HRP-1.3.1.1/uw_hrp/resources/hrpws/file/hrp/v3/person/faculty.json_future_worker_true` & `UW-RestClients-HRP-1.3.2/uw_hrp/resources/hrpws/file/hrp/v3/person/faculty.json_future_worker_true`

 * *Files identical despite different names*

### Comparing `UW-RestClients-HRP-1.3.1.1/uw_hrp/resources/hrpws/file/hrp/v3/person.json_changed_since_date_2022-12-12_page_size_200` & `UW-RestClients-HRP-1.3.2/uw_hrp/resources/hrpws/file/hrp/v3/person.json_changed_since_date_2022-12-12_page_size_200`

 * *Files identical despite different names*

### Comparing `UW-RestClients-HRP-1.3.1.1/uw_hrp/tests/test_hrp.py` & `UW-RestClients-HRP-1.3.2/uw_hrp/tests/test_hrp.py`

 * *Files identical despite different names*

### Comparing `UW-RestClients-HRP-1.3.1.1/uw_hrp/tests/test_models.py` & `UW-RestClients-HRP-1.3.2/uw_hrp/tests/test_models.py`

 * *Files 2% similar despite different names*

```diff
@@ -41,14 +41,19 @@
 
     def test_get_org_code_name(self):
         data = "CAS: Chemistry: Theberge JM Student (...())"
         code, name = get_org_code_name(data)
         self.assertEqual(code, "CAS")
         self.assertEqual(name, "Chemistry: Theberge JM Student")
 
+        # exceptional case
+        code, name = get_org_code_name("School of Law (Lawson, Tamara F)")
+        self.assertEqual(code, "")
+        self.assertEqual(name, "School of Law")
+
     def test_employment_status(self):
         emp_status0 = EmploymentStatus(status="Active", is_active=True)
         self.assertIsNotNone(emp_status0)
         self.assertEqual(
             emp_status0.to_json(),
             {
                 'hire_date': None,
```

