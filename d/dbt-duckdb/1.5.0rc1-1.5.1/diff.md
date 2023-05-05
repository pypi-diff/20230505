# Comparing `tmp/dbt-duckdb-1.5.0rc1.tar.gz` & `tmp/dbt-duckdb-1.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dbt-duckdb-1.5.0rc1.tar", last modified: Wed Apr 19 20:36:09 2023, max compression
+gzip compressed data, was "dbt-duckdb-1.5.1.tar", last modified: Fri May  5 18:27:10 2023, max compression
```

## Comparing `dbt-duckdb-1.5.0rc1.tar` & `dbt-duckdb-1.5.1.tar`

### file list

```diff
@@ -1,57 +1,59 @@
-drwxr-xr-x   0 jwills     (501) staff       (20)        0 2023-04-19 20:36:09.855300 dbt-duckdb-1.5.0rc1/
--rw-r--r--   0 jwills     (501) staff       (20)    11357 2022-12-17 04:32:15.000000 dbt-duckdb-1.5.0rc1/LICENSE
--rw-r--r--   0 jwills     (501) staff       (20)       47 2022-12-17 04:32:15.000000 dbt-duckdb-1.5.0rc1/MANIFEST.in
--rw-r--r--   0 jwills     (501) staff       (20)    13051 2023-04-19 20:36:09.855118 dbt-duckdb-1.5.0rc1/PKG-INFO
--rw-r--r--   0 jwills     (501) staff       (20)    12744 2023-03-21 22:22:36.000000 dbt-duckdb-1.5.0rc1/README.md
-drwxr-xr-x   0 jwills     (501) staff       (20)        0 2023-04-19 20:36:09.846926 dbt-duckdb-1.5.0rc1/dbt/
--rw-r--r--   0 jwills     (501) staff       (20)       92 2022-12-17 04:32:15.000000 dbt-duckdb-1.5.0rc1/dbt/__init__.py
-drwxr-xr-x   0 jwills     (501) staff       (20)        0 2023-04-19 20:36:09.847184 dbt-duckdb-1.5.0rc1/dbt/adapters/
--rw-r--r--   0 jwills     (501) staff       (20)       92 2022-12-17 04:32:15.000000 dbt-duckdb-1.5.0rc1/dbt/adapters/__init__.py
-drwxr-xr-x   0 jwills     (501) staff       (20)        0 2023-04-19 20:36:09.849434 dbt-duckdb-1.5.0rc1/dbt/adapters/duckdb/
--rw-r--r--   0 jwills     (501) staff       (20)      407 2023-03-23 17:19:15.000000 dbt-duckdb-1.5.0rc1/dbt/adapters/duckdb/__init__.py
--rw-r--r--   0 jwills     (501) staff       (20)       21 2023-04-19 20:35:31.000000 dbt-duckdb-1.5.0rc1/dbt/adapters/duckdb/__version__.py
--rw-r--r--   0 jwills     (501) staff       (20)     1910 2023-04-17 03:57:27.000000 dbt-duckdb-1.5.0rc1/dbt/adapters/duckdb/buenavista.py
--rw-r--r--   0 jwills     (501) staff       (20)     3163 2023-04-17 03:57:27.000000 dbt-duckdb-1.5.0rc1/dbt/adapters/duckdb/connections.py
--rw-r--r--   0 jwills     (501) staff       (20)     6057 2023-04-17 03:57:27.000000 dbt-duckdb-1.5.0rc1/dbt/adapters/duckdb/credentials.py
--rw-r--r--   0 jwills     (501) staff       (20)     7866 2023-04-18 19:29:01.000000 dbt-duckdb-1.5.0rc1/dbt/adapters/duckdb/environments.py
--rw-r--r--   0 jwills     (501) staff       (20)     7965 2023-03-26 18:59:50.000000 dbt-duckdb-1.5.0rc1/dbt/adapters/duckdb/glue.py
--rw-r--r--   0 jwills     (501) staff       (20)     6984 2023-04-17 03:57:27.000000 dbt-duckdb-1.5.0rc1/dbt/adapters/duckdb/impl.py
-drwxr-xr-x   0 jwills     (501) staff       (20)        0 2023-04-19 20:36:09.850216 dbt-duckdb-1.5.0rc1/dbt/adapters/duckdb/plugins/
--rw-r--r--   0 jwills     (501) staff       (20)     1291 2023-04-17 03:57:27.000000 dbt-duckdb-1.5.0rc1/dbt/adapters/duckdb/plugins/__init__.py
--rw-r--r--   0 jwills     (501) staff       (20)      589 2023-04-17 03:57:27.000000 dbt-duckdb-1.5.0rc1/dbt/adapters/duckdb/plugins/excel.py
--rw-r--r--   0 jwills     (501) staff       (20)     1669 2023-04-17 03:57:27.000000 dbt-duckdb-1.5.0rc1/dbt/adapters/duckdb/plugins/gsheet.py
--rw-r--r--   0 jwills     (501) staff       (20)     1008 2023-04-18 19:29:01.000000 dbt-duckdb-1.5.0rc1/dbt/adapters/duckdb/plugins/iceberg.py
--rw-r--r--   0 jwills     (501) staff       (20)     1034 2023-04-17 03:57:27.000000 dbt-duckdb-1.5.0rc1/dbt/adapters/duckdb/plugins/sqlalchemy.py
--rw-r--r--   0 jwills     (501) staff       (20)     2050 2023-04-17 03:57:27.000000 dbt-duckdb-1.5.0rc1/dbt/adapters/duckdb/relation.py
--rw-r--r--   0 jwills     (501) staff       (20)     1141 2023-04-17 03:57:27.000000 dbt-duckdb-1.5.0rc1/dbt/adapters/duckdb/utils.py
-drwxr-xr-x   0 jwills     (501) staff       (20)        0 2023-04-19 20:36:09.850359 dbt-duckdb-1.5.0rc1/dbt/include/
--rw-r--r--   0 jwills     (501) staff       (20)       92 2022-12-17 04:32:15.000000 dbt-duckdb-1.5.0rc1/dbt/include/__init__.py
-drwxr-xr-x   0 jwills     (501) staff       (20)        0 2023-04-19 20:36:09.850641 dbt-duckdb-1.5.0rc1/dbt/include/duckdb/
--rw-r--r--   0 jwills     (501) staff       (20)       52 2022-12-17 04:32:15.000000 dbt-duckdb-1.5.0rc1/dbt/include/duckdb/__init__.py
--rw-r--r--   0 jwills     (501) staff       (20)       74 2022-12-17 04:32:15.000000 dbt-duckdb-1.5.0rc1/dbt/include/duckdb/dbt_project.yml
-drwxr-xr-x   0 jwills     (501) staff       (20)        0 2023-04-19 20:36:09.851551 dbt-duckdb-1.5.0rc1/dbt/include/duckdb/macros/
--rw-r--r--   0 jwills     (501) staff       (20)     7122 2023-03-21 22:22:36.000000 dbt-duckdb-1.5.0rc1/dbt/include/duckdb/macros/adapters.sql
--rw-r--r--   0 jwills     (501) staff       (20)      950 2023-03-21 22:16:25.000000 dbt-duckdb-1.5.0rc1/dbt/include/duckdb/macros/catalog.sql
-drwxr-xr-x   0 jwills     (501) staff       (20)        0 2023-04-19 20:36:09.852698 dbt-duckdb-1.5.0rc1/dbt/include/duckdb/macros/materializations/
--rw-r--r--   0 jwills     (501) staff       (20)     3916 2023-03-30 16:27:45.000000 dbt-duckdb-1.5.0rc1/dbt/include/duckdb/macros/materializations/external.sql
--rw-r--r--   0 jwills     (501) staff       (20)     4633 2023-02-15 20:16:22.000000 dbt-duckdb-1.5.0rc1/dbt/include/duckdb/macros/materializations/incremental.sql
--rw-r--r--   0 jwills     (501) staff       (20)     2529 2023-02-15 20:16:22.000000 dbt-duckdb-1.5.0rc1/dbt/include/duckdb/macros/materializations/table.sql
--rw-r--r--   0 jwills     (501) staff       (20)     1417 2023-04-03 22:00:10.000000 dbt-duckdb-1.5.0rc1/dbt/include/duckdb/macros/seed.sql
--rw-r--r--   0 jwills     (501) staff       (20)      862 2023-03-27 04:56:30.000000 dbt-duckdb-1.5.0rc1/dbt/include/duckdb/macros/snapshot_merge.sql
-drwxr-xr-x   0 jwills     (501) staff       (20)        0 2023-04-19 20:36:09.854144 dbt-duckdb-1.5.0rc1/dbt/include/duckdb/macros/utils/
--rw-r--r--   0 jwills     (501) staff       (20)       93 2022-12-17 04:32:15.000000 dbt-duckdb-1.5.0rc1/dbt/include/duckdb/macros/utils/any_value.sql
--rw-r--r--   0 jwills     (501) staff       (20)      175 2022-12-17 04:32:15.000000 dbt-duckdb-1.5.0rc1/dbt/include/duckdb/macros/utils/dateadd.sql
--rw-r--r--   0 jwills     (501) staff       (20)     2338 2022-12-17 04:32:15.000000 dbt-duckdb-1.5.0rc1/dbt/include/duckdb/macros/utils/datediff.sql
--rw-r--r--   0 jwills     (501) staff       (20)      357 2023-03-21 22:16:25.000000 dbt-duckdb-1.5.0rc1/dbt/include/duckdb/macros/utils/external_location.sql
--rw-r--r--   0 jwills     (501) staff       (20)      378 2022-12-17 04:32:15.000000 dbt-duckdb-1.5.0rc1/dbt/include/duckdb/macros/utils/lastday.sql
--rw-r--r--   0 jwills     (501) staff       (20)      568 2022-12-21 20:35:46.000000 dbt-duckdb-1.5.0rc1/dbt/include/duckdb/macros/utils/listagg.sql
--rw-r--r--   0 jwills     (501) staff       (20)      315 2022-12-17 04:32:15.000000 dbt-duckdb-1.5.0rc1/dbt/include/duckdb/macros/utils/splitpart.sql
--rw-r--r--   0 jwills     (501) staff       (20)     1724 2023-03-30 04:33:01.000000 dbt-duckdb-1.5.0rc1/dbt/include/duckdb/macros/utils/upstream.sql
-drwxr-xr-x   0 jwills     (501) staff       (20)        0 2023-04-19 20:36:09.854936 dbt-duckdb-1.5.0rc1/dbt_duckdb.egg-info/
--rw-r--r--   0 jwills     (501) staff       (20)    13051 2023-04-19 20:36:09.000000 dbt-duckdb-1.5.0rc1/dbt_duckdb.egg-info/PKG-INFO
--rw-r--r--   0 jwills     (501) staff       (20)     1551 2023-04-19 20:36:09.000000 dbt-duckdb-1.5.0rc1/dbt_duckdb.egg-info/SOURCES.txt
--rw-r--r--   0 jwills     (501) staff       (20)        1 2023-04-19 20:36:09.000000 dbt-duckdb-1.5.0rc1/dbt_duckdb.egg-info/dependency_links.txt
--rw-r--r--   0 jwills     (501) staff       (20)       63 2023-04-19 20:36:09.000000 dbt-duckdb-1.5.0rc1/dbt_duckdb.egg-info/requires.txt
--rw-r--r--   0 jwills     (501) staff       (20)        4 2023-04-19 20:36:09.000000 dbt-duckdb-1.5.0rc1/dbt_duckdb.egg-info/top_level.txt
--rw-r--r--   0 jwills     (501) staff       (20)       38 2023-04-19 20:36:09.855332 dbt-duckdb-1.5.0rc1/setup.cfg
--rw-r--r--   0 jwills     (501) staff       (20)     1369 2023-04-19 20:35:31.000000 dbt-duckdb-1.5.0rc1/setup.py
+drwxr-xr-x   0 jwills     (501) staff       (20)        0 2023-05-05 18:27:10.598988 dbt-duckdb-1.5.1/
+-rw-r--r--   0 jwills     (501) staff       (20)    11357 2022-12-17 04:32:15.000000 dbt-duckdb-1.5.1/LICENSE
+-rw-r--r--   0 jwills     (501) staff       (20)       47 2022-12-17 04:32:15.000000 dbt-duckdb-1.5.1/MANIFEST.in
+-rw-r--r--   0 jwills     (501) staff       (20)    13064 2023-05-05 18:27:10.598676 dbt-duckdb-1.5.1/PKG-INFO
+-rw-r--r--   0 jwills     (501) staff       (20)    12760 2023-05-05 18:08:44.000000 dbt-duckdb-1.5.1/README.md
+drwxr-xr-x   0 jwills     (501) staff       (20)        0 2023-05-05 18:27:10.587737 dbt-duckdb-1.5.1/dbt/
+-rw-r--r--   0 jwills     (501) staff       (20)       92 2022-12-17 04:32:15.000000 dbt-duckdb-1.5.1/dbt/__init__.py
+drwxr-xr-x   0 jwills     (501) staff       (20)        0 2023-05-05 18:27:10.587956 dbt-duckdb-1.5.1/dbt/adapters/
+-rw-r--r--   0 jwills     (501) staff       (20)       92 2022-12-17 04:32:15.000000 dbt-duckdb-1.5.1/dbt/adapters/__init__.py
+drwxr-xr-x   0 jwills     (501) staff       (20)        0 2023-05-05 18:27:10.590138 dbt-duckdb-1.5.1/dbt/adapters/duckdb/
+-rw-r--r--   0 jwills     (501) staff       (20)      407 2023-03-23 17:19:15.000000 dbt-duckdb-1.5.1/dbt/adapters/duckdb/__init__.py
+-rw-r--r--   0 jwills     (501) staff       (20)       18 2023-05-05 18:17:03.000000 dbt-duckdb-1.5.1/dbt/adapters/duckdb/__version__.py
+-rw-r--r--   0 jwills     (501) staff       (20)     3163 2023-05-03 15:42:01.000000 dbt-duckdb-1.5.1/dbt/adapters/duckdb/connections.py
+-rw-r--r--   0 jwills     (501) staff       (20)     6712 2023-05-05 18:08:44.000000 dbt-duckdb-1.5.1/dbt/adapters/duckdb/credentials.py
+drwxr-xr-x   0 jwills     (501) staff       (20)        0 2023-05-05 18:27:10.590911 dbt-duckdb-1.5.1/dbt/adapters/duckdb/environments/
+-rw-r--r--   0 jwills     (501) staff       (20)     5173 2023-05-05 18:08:44.000000 dbt-duckdb-1.5.1/dbt/adapters/duckdb/environments/__init__.py
+-rw-r--r--   0 jwills     (501) staff       (20)     1900 2023-05-05 18:08:44.000000 dbt-duckdb-1.5.1/dbt/adapters/duckdb/environments/buenavista.py
+-rw-r--r--   0 jwills     (501) staff       (20)     3871 2023-05-05 18:07:40.000000 dbt-duckdb-1.5.1/dbt/adapters/duckdb/environments/local.py
+-rw-r--r--   0 jwills     (501) staff       (20)     7965 2023-03-26 18:59:50.000000 dbt-duckdb-1.5.1/dbt/adapters/duckdb/glue.py
+-rw-r--r--   0 jwills     (501) staff       (20)     8611 2023-05-05 18:08:44.000000 dbt-duckdb-1.5.1/dbt/adapters/duckdb/impl.py
+drwxr-xr-x   0 jwills     (501) staff       (20)        0 2023-05-05 18:27:10.592344 dbt-duckdb-1.5.1/dbt/adapters/duckdb/plugins/
+-rw-r--r--   0 jwills     (501) staff       (20)     1291 2023-04-17 03:57:27.000000 dbt-duckdb-1.5.1/dbt/adapters/duckdb/plugins/__init__.py
+-rw-r--r--   0 jwills     (501) staff       (20)      589 2023-04-17 03:57:27.000000 dbt-duckdb-1.5.1/dbt/adapters/duckdb/plugins/excel.py
+-rw-r--r--   0 jwills     (501) staff       (20)     1669 2023-04-17 03:57:27.000000 dbt-duckdb-1.5.1/dbt/adapters/duckdb/plugins/gsheet.py
+-rw-r--r--   0 jwills     (501) staff       (20)     1008 2023-04-18 19:29:01.000000 dbt-duckdb-1.5.1/dbt/adapters/duckdb/plugins/iceberg.py
+-rw-r--r--   0 jwills     (501) staff       (20)     1034 2023-04-17 03:57:27.000000 dbt-duckdb-1.5.1/dbt/adapters/duckdb/plugins/sqlalchemy.py
+-rw-r--r--   0 jwills     (501) staff       (20)     2050 2023-04-17 03:57:27.000000 dbt-duckdb-1.5.1/dbt/adapters/duckdb/relation.py
+-rw-r--r--   0 jwills     (501) staff       (20)     1247 2023-05-05 18:05:09.000000 dbt-duckdb-1.5.1/dbt/adapters/duckdb/utils.py
+drwxr-xr-x   0 jwills     (501) staff       (20)        0 2023-05-05 18:27:10.592500 dbt-duckdb-1.5.1/dbt/include/
+-rw-r--r--   0 jwills     (501) staff       (20)       92 2022-12-17 04:32:15.000000 dbt-duckdb-1.5.1/dbt/include/__init__.py
+drwxr-xr-x   0 jwills     (501) staff       (20)        0 2023-05-05 18:27:10.592837 dbt-duckdb-1.5.1/dbt/include/duckdb/
+-rw-r--r--   0 jwills     (501) staff       (20)       52 2022-12-17 04:32:15.000000 dbt-duckdb-1.5.1/dbt/include/duckdb/__init__.py
+-rw-r--r--   0 jwills     (501) staff       (20)       74 2022-12-17 04:32:15.000000 dbt-duckdb-1.5.1/dbt/include/duckdb/dbt_project.yml
+drwxr-xr-x   0 jwills     (501) staff       (20)        0 2023-05-05 18:27:10.593757 dbt-duckdb-1.5.1/dbt/include/duckdb/macros/
+-rw-r--r--   0 jwills     (501) staff       (20)     8151 2023-05-05 18:08:44.000000 dbt-duckdb-1.5.1/dbt/include/duckdb/macros/adapters.sql
+-rw-r--r--   0 jwills     (501) staff       (20)      950 2023-03-21 22:16:25.000000 dbt-duckdb-1.5.1/dbt/include/duckdb/macros/catalog.sql
+drwxr-xr-x   0 jwills     (501) staff       (20)        0 2023-05-05 18:27:10.594633 dbt-duckdb-1.5.1/dbt/include/duckdb/macros/materializations/
+-rw-r--r--   0 jwills     (501) staff       (20)     3916 2023-03-30 16:27:45.000000 dbt-duckdb-1.5.1/dbt/include/duckdb/macros/materializations/external.sql
+-rw-r--r--   0 jwills     (501) staff       (20)     4633 2023-02-15 20:16:22.000000 dbt-duckdb-1.5.1/dbt/include/duckdb/macros/materializations/incremental.sql
+-rw-r--r--   0 jwills     (501) staff       (20)     2529 2023-02-15 20:16:22.000000 dbt-duckdb-1.5.1/dbt/include/duckdb/macros/materializations/table.sql
+-rw-r--r--   0 jwills     (501) staff       (20)     1417 2023-04-03 22:00:10.000000 dbt-duckdb-1.5.1/dbt/include/duckdb/macros/seed.sql
+-rw-r--r--   0 jwills     (501) staff       (20)      792 2023-05-05 18:08:44.000000 dbt-duckdb-1.5.1/dbt/include/duckdb/macros/snapshot_merge.sql
+drwxr-xr-x   0 jwills     (501) staff       (20)        0 2023-05-05 18:27:10.596771 dbt-duckdb-1.5.1/dbt/include/duckdb/macros/utils/
+-rw-r--r--   0 jwills     (501) staff       (20)       93 2022-12-17 04:32:15.000000 dbt-duckdb-1.5.1/dbt/include/duckdb/macros/utils/any_value.sql
+-rw-r--r--   0 jwills     (501) staff       (20)      175 2022-12-17 04:32:15.000000 dbt-duckdb-1.5.1/dbt/include/duckdb/macros/utils/dateadd.sql
+-rw-r--r--   0 jwills     (501) staff       (20)     2338 2022-12-17 04:32:15.000000 dbt-duckdb-1.5.1/dbt/include/duckdb/macros/utils/datediff.sql
+-rw-r--r--   0 jwills     (501) staff       (20)      357 2023-03-21 22:16:25.000000 dbt-duckdb-1.5.1/dbt/include/duckdb/macros/utils/external_location.sql
+-rw-r--r--   0 jwills     (501) staff       (20)      378 2022-12-17 04:32:15.000000 dbt-duckdb-1.5.1/dbt/include/duckdb/macros/utils/lastday.sql
+-rw-r--r--   0 jwills     (501) staff       (20)      568 2022-12-21 20:35:46.000000 dbt-duckdb-1.5.1/dbt/include/duckdb/macros/utils/listagg.sql
+-rw-r--r--   0 jwills     (501) staff       (20)      315 2022-12-17 04:32:15.000000 dbt-duckdb-1.5.1/dbt/include/duckdb/macros/utils/splitpart.sql
+-rw-r--r--   0 jwills     (501) staff       (20)     1724 2023-03-30 04:33:01.000000 dbt-duckdb-1.5.1/dbt/include/duckdb/macros/utils/upstream.sql
+drwxr-xr-x   0 jwills     (501) staff       (20)        0 2023-05-05 18:27:10.598343 dbt-duckdb-1.5.1/dbt_duckdb.egg-info/
+-rw-r--r--   0 jwills     (501) staff       (20)    13064 2023-05-05 18:27:10.000000 dbt-duckdb-1.5.1/dbt_duckdb.egg-info/PKG-INFO
+-rw-r--r--   0 jwills     (501) staff       (20)     1615 2023-05-05 18:27:10.000000 dbt-duckdb-1.5.1/dbt_duckdb.egg-info/SOURCES.txt
+-rw-r--r--   0 jwills     (501) staff       (20)        1 2023-05-05 18:27:10.000000 dbt-duckdb-1.5.1/dbt_duckdb.egg-info/dependency_links.txt
+-rw-r--r--   0 jwills     (501) staff       (20)       60 2023-05-05 18:27:10.000000 dbt-duckdb-1.5.1/dbt_duckdb.egg-info/requires.txt
+-rw-r--r--   0 jwills     (501) staff       (20)        4 2023-05-05 18:27:10.000000 dbt-duckdb-1.5.1/dbt_duckdb.egg-info/top_level.txt
+-rw-r--r--   0 jwills     (501) staff       (20)       38 2023-05-05 18:27:10.599029 dbt-duckdb-1.5.1/setup.cfg
+-rw-r--r--   0 jwills     (501) staff       (20)     1366 2023-05-05 18:08:44.000000 dbt-duckdb-1.5.1/setup.py
```

### Comparing `dbt-duckdb-1.5.0rc1/LICENSE` & `dbt-duckdb-1.5.1/LICENSE`

 * *Files identical despite different names*

### Comparing `dbt-duckdb-1.5.0rc1/PKG-INFO` & `dbt-duckdb-1.5.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbt-duckdb
-Version: 1.5.0rc1
+Version: 1.5.1
 Summary: The duckdb adapter plugin for dbt (data build tool)
 Home-page: https://github.com/jwills/dbt-duckdb
 Author: Josh Wills
 Author-email: joshwills+dbt@gmail.com
 Description-Content-Type: text/markdown
 Provides-Extra: glue
 License-File: LICENSE
@@ -21,15 +21,15 @@
 
 ### Installation
 
 This project is hosted on PyPI, so you should be able to install it and the necessary dependencies via:
 
 `pip3 install dbt-duckdb`
 
-The latest supported version targets `dbt-core` 1.4.x and `duckdb` version 0.7.x, but we work hard to ensure that newer
+The latest supported version targets `dbt-core` 1.5.x and `duckdb` version 0.7.x, but we work hard to ensure that newer
 versions of DuckDB will continue to work with the adapter as they are released. If you would like to use our new (and experimental!)
 support for persisting the tables that DuckDB creates to the [AWS Glue Catalog](https://aws.amazon.com/glue/), you should install
 `dbt-duckdb[glue]` in order to get the AWS dependencies as well.
 
 ### Configuring Your Profile
 
 A minimal dbt-duckdb profile only needs two settings, `type` and `path`:
@@ -101,17 +101,17 @@
 illustrates the usage of this feature to connect to a Localstack instance running S3 from dbt-duckdb [here](https://github.com/jwills/s3-demo).
 
 #### Fetching credentials from context
 Instead of specifying the credentials through the settings block, you can also use the use_credential_provider property. If you set this to `aws` (currently the only supported implementation) and you have `boto3` installed in your python environment, we will fetch your AWS credentials using the credential provider chain as described [here](https://boto3.amazonaws.com/v1/documentation/api/latest/guide/credentials.html). This means that you can use any supported mechanism from AWS to obtain credentials (e.g., web identity tokens).
 
 #### Attaching Additional Databases
 
-DuckDB version `0.7.0` and dbt-duckdb version `1.4.0` support [attaching additional databases](https://duckdb.org/docs/sql/statements/attach.html) to your dbt-duckdb run so that you can read
+DuckDB version `0.7.0` added support for [attaching additional databases](https://duckdb.org/docs/sql/statements/attach.html) to your dbt-duckdb run so that you can read
 and write from multiple databases. Additional databases may be configured using [dbt run hooks](https://docs.getdbt.com/docs/build/hooks-operations) or via the `attach` argument
-in your profile:
+in your profile that was added in dbt-duckdb `1.4.0`:
 
 ```
 default:
   outputs:
     dev:
       type: duckdb
       path: /tmp/dbt.duckdb
```

### Comparing `dbt-duckdb-1.5.0rc1/README.md` & `dbt-duckdb-1.5.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 
 ### Installation
 
 This project is hosted on PyPI, so you should be able to install it and the necessary dependencies via:
 
 `pip3 install dbt-duckdb`
 
-The latest supported version targets `dbt-core` 1.4.x and `duckdb` version 0.7.x, but we work hard to ensure that newer
+The latest supported version targets `dbt-core` 1.5.x and `duckdb` version 0.7.x, but we work hard to ensure that newer
 versions of DuckDB will continue to work with the adapter as they are released. If you would like to use our new (and experimental!)
 support for persisting the tables that DuckDB creates to the [AWS Glue Catalog](https://aws.amazon.com/glue/), you should install
 `dbt-duckdb[glue]` in order to get the AWS dependencies as well.
 
 ### Configuring Your Profile
 
 A minimal dbt-duckdb profile only needs two settings, `type` and `path`:
@@ -90,17 +90,17 @@
 illustrates the usage of this feature to connect to a Localstack instance running S3 from dbt-duckdb [here](https://github.com/jwills/s3-demo).
 
 #### Fetching credentials from context
 Instead of specifying the credentials through the settings block, you can also use the use_credential_provider property. If you set this to `aws` (currently the only supported implementation) and you have `boto3` installed in your python environment, we will fetch your AWS credentials using the credential provider chain as described [here](https://boto3.amazonaws.com/v1/documentation/api/latest/guide/credentials.html). This means that you can use any supported mechanism from AWS to obtain credentials (e.g., web identity tokens).
 
 #### Attaching Additional Databases
 
-DuckDB version `0.7.0` and dbt-duckdb version `1.4.0` support [attaching additional databases](https://duckdb.org/docs/sql/statements/attach.html) to your dbt-duckdb run so that you can read
+DuckDB version `0.7.0` added support for [attaching additional databases](https://duckdb.org/docs/sql/statements/attach.html) to your dbt-duckdb run so that you can read
 and write from multiple databases. Additional databases may be configured using [dbt run hooks](https://docs.getdbt.com/docs/build/hooks-operations) or via the `attach` argument
-in your profile:
+in your profile that was added in dbt-duckdb `1.4.0`:
 
 ```
 default:
   outputs:
     dev:
       type: duckdb
       path: /tmp/dbt.duckdb
```

### Comparing `dbt-duckdb-1.5.0rc1/dbt/adapters/duckdb/buenavista.py` & `dbt-duckdb-1.5.1/dbt/adapters/duckdb/environments/buenavista.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import json
 
 import psycopg2
 
-from . import credentials
-from . import utils
-from .environments import Environment
+from . import Environment
+from .. import credentials
+from .. import utils
 from dbt.contracts.connection import AdapterResponse
 
 
 class BVEnvironment(Environment):
     @classmethod
     def _get_conn(cls, dbname: str, remote: credentials.Remote):
         return psycopg2.connect(
```

### Comparing `dbt-duckdb-1.5.0rc1/dbt/adapters/duckdb/connections.py` & `dbt-duckdb-1.5.1/dbt/adapters/duckdb/connections.py`

 * *Files identical despite different names*

### Comparing `dbt-duckdb-1.5.0rc1/dbt/adapters/duckdb/credentials.py` & `dbt-duckdb-1.5.1/dbt/adapters/duckdb/credentials.py`

 * *Files 7% similar despite different names*

```diff
@@ -3,17 +3,19 @@
 from dataclasses import dataclass
 from functools import lru_cache
 from typing import Any
 from typing import Dict
 from typing import List
 from typing import Optional
 from typing import Tuple
+from urllib.parse import urlparse
 
 import duckdb
 
+import dbt.exceptions
 from dbt.adapters.base import Credentials
 from dbt.dataclass_schema import dbtClassMixin
 
 
 @dataclass
 class Attachment(dbtClassMixin):
     # The path to the database to be attached (may be a URL)
@@ -112,21 +114,33 @@
     # A list of dbt-duckdb plugins that can be used to customize the
     # behavior of loading source data and/or storing the relations that are
     # created by SQL or Python models; see the plugins module for more details.
     plugins: Optional[List[PluginConfig]] = None
 
     @classmethod
     def __pre_deserialize__(cls, data: Dict[Any, Any]) -> Dict[Any, Any]:
-        data = super().__pre_deserialize__(data)
-        path = data.get("path")
-        if path and "database" not in data and duckdb.__version__ >= "0.7.0":
-            if path == ":memory:":
-                data["database"] = "memory"
-            else:
-                data["database"] = os.path.splitext(os.path.basename(path))[0]
+        if duckdb.__version__ >= "0.7.0":
+            data = super().__pre_deserialize__(data)
+            if "database" not in data:
+                # if no database is specified in the profile, figure out
+                # the database value to use from the path argument
+                path = data.get("path")
+                if path is None or path == ":memory:":
+                    data["database"] = "memory"
+                else:
+                    parsed = urlparse(path)
+                    base_file = os.path.basename(parsed.path)
+                    db = os.path.splitext(base_file)[0]
+                    if db:
+                        data["database"] = db
+                    else:
+                        raise dbt.exceptions.DbtRuntimeError(
+                            "Unable to determine database name from path"
+                            " and no database was specified in profile"
+                        )
         return data
 
     @property
     def unique_field(self) -> str:
         if self.remote:
             return self.remote.host + str(self.remote.port)
         else:
```

### Comparing `dbt-duckdb-1.5.0rc1/dbt/adapters/duckdb/environments.py` & `dbt-duckdb-1.5.1/dbt/adapters/duckdb/impl.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,229 +1,243 @@
-import abc
-import importlib.util
 import os
-import tempfile
-from typing import Dict
+from typing import List
+from typing import Optional
+from typing import Sequence
 
+import agate
 import duckdb
 
-from .credentials import DuckDBCredentials
-from .plugins import Plugin
-from .utils import SourceConfig
+from dbt.adapters.base import BaseRelation
+from dbt.adapters.base.column import Column
+from dbt.adapters.base.impl import ConstraintSupport
+from dbt.adapters.base.meta import available
+from dbt.adapters.duckdb.connections import DuckDBConnectionManager
+from dbt.adapters.duckdb.glue import create_or_update_table
+from dbt.adapters.duckdb.relation import DuckDBRelation
+from dbt.adapters.sql import SQLAdapter
 from dbt.contracts.connection import AdapterResponse
+from dbt.contracts.graph.nodes import ColumnLevelConstraint
+from dbt.contracts.graph.nodes import ConstraintType
+from dbt.exceptions import DbtInternalError
 from dbt.exceptions import DbtRuntimeError
 
 
-def _ensure_event_loop():
-    """
-    Ensures the current thread has an event loop defined, and creates one if necessary.
-    """
-    import asyncio
-
-    try:
-        # Check that the current thread has an event loop attached
-        loop = asyncio.get_event_loop()
-    except RuntimeError:
-        # If the current thread doesn't have an event loop, create one
-        loop = asyncio.new_event_loop()
-        asyncio.set_event_loop(loop)
-
-
-class DuckDBCursorWrapper:
-    def __init__(self, cursor):
-        self._cursor = cursor
-
-    # forward along all non-execute() methods/attribute look-ups
-    def __getattr__(self, name):
-        return getattr(self._cursor, name)
-
-    def execute(self, sql, bindings=None):
-        try:
-            if bindings is None:
-                return self._cursor.execute(sql)
-            else:
-                return self._cursor.execute(sql, bindings)
-        except RuntimeError as e:
-            raise DbtRuntimeError(str(e))
-
-
-class DuckDBConnectionWrapper:
-    def __init__(self, cursor):
-        self._cursor = DuckDBCursorWrapper(cursor)
-
-    def close(self):
-        self._cursor.close()
-
-    def cursor(self):
-        return self._cursor
-
-
-class Environment(abc.ABC):
-    @abc.abstractmethod
-    def handle(self):
-        pass
-
-    @abc.abstractmethod
-    def submit_python_job(self, handle, parsed_model: dict, compiled_code: str) -> AdapterResponse:
-        pass
-
-    def get_binding_char(self) -> str:
-        return "?"
-
-    @abc.abstractmethod
-    def load_source(self, plugin_name: str, source_config: SourceConfig) -> str:
-        pass
+class DuckDBAdapter(SQLAdapter):
+    ConnectionManager = DuckDBConnectionManager
+    Relation = DuckDBRelation
+
+    CONSTRAINT_SUPPORT = {
+        ConstraintType.check: ConstraintSupport.ENFORCED,
+        ConstraintType.not_null: ConstraintSupport.ENFORCED,
+        ConstraintType.unique: ConstraintSupport.ENFORCED,
+        ConstraintType.primary_key: ConstraintSupport.ENFORCED,
+        ConstraintType.foreign_key: ConstraintSupport.ENFORCED,
+    }
 
     @classmethod
-    def initialize_db(cls, creds: DuckDBCredentials):
-        config = creds.config_options or {}
-        conn = duckdb.connect(creds.path, read_only=False, config=config)
-
-        # install any extensions on the connection
-        if creds.extensions is not None:
-            for extension in creds.extensions:
-                conn.execute(f"INSTALL '{extension}'")
-
-        # Attach any fsspec filesystems on the database
-        if creds.filesystems:
-            import fsspec
-
-            for spec in creds.filesystems:
-                curr = spec.copy()
-                fsimpl = curr.pop("fs")
-                fs = fsspec.filesystem(fsimpl, **curr)
-                conn.register_filesystem(fs)
-
-        # attach any databases that we will be using
-        if creds.attach:
-            for attachment in creds.attach:
-                conn.execute(attachment.to_sql())
-        return conn
+    def date_function(cls) -> str:
+        return "now()"
 
     @classmethod
-    def initialize_cursor(cls, creds: DuckDBCredentials, cursor):
-        # Extensions/settings need to be configured per cursor
-        for ext in creds.extensions or []:
-            cursor.execute(f"LOAD '{ext}'")
-        for key, value in creds.load_settings().items():
-            # Okay to set these as strings because DuckDB will cast them
-            # to the correct type
-            cursor.execute(f"SET {key} = '{value}'")
-        return cursor
+    def is_cancelable(cls) -> bool:
+        return False
 
-    @classmethod
-    def initialize_plugins(cls, creds: DuckDBCredentials) -> Dict[str, Plugin]:
-        ret = {}
-        for plugin in creds.plugins or []:
-            if plugin.name in ret:
-                raise Exception("Duplicate plugin name: " + plugin.name)
-            else:
-                if plugin.impl in Plugin.WELL_KNOWN_PLUGINS:
-                    plugin.impl = Plugin.WELL_KNOWN_PLUGINS[plugin.impl]
-                try:
-                    ret[plugin.name] = Plugin.create(plugin.impl, plugin.config or {})
-                except Exception as e:
-                    raise Exception(f"Error attempting to create plugin {plugin.name}", e)
-        return ret
-
-    @classmethod
-    def run_python_job(cls, con, load_df_function, identifier: str, compiled_code: str):
-        mod_file = tempfile.NamedTemporaryFile(suffix=".py", delete=False)
-        mod_file.write(compiled_code.lstrip().encode("utf-8"))
-        mod_file.close()
-
-        # Ensure that we have an event loop for async code to use since we may
-        # be running inside of a thread that doesn't have one defined
-        _ensure_event_loop()
-
-        try:
-            spec = importlib.util.spec_from_file_location(identifier, mod_file.name)
-            if not spec:
-                raise DbtRuntimeError(
-                    "Failed to load python model as module: {}".format(identifier)
-                )
-            module = importlib.util.module_from_spec(spec)
-            if spec.loader:
-                spec.loader.exec_module(module)
-            else:
-                raise DbtRuntimeError(
-                    "Python module spec is missing loader: {}".format(identifier)
+    @available
+    def convert_datetimes_to_strs(self, table: agate.Table) -> agate.Table:
+        for column in table.columns:
+            if isinstance(column.data_type, agate.DateTime):
+                table = table.compute(
+                    [
+                        (
+                            column.name,
+                            agate.Formula(agate.Text(), lambda row: str(row[column.name])),
+                        )
+                    ],
+                    replace=True,
                 )
+        return table
 
-            # Do the actual work to run the code here
-            dbt = module.dbtObj(load_df_function)
-            df = module.model(dbt, con)
-            module.materialize(df, con)
-        except Exception as err:
-            raise DbtRuntimeError(f"Python model failed:\n" f"{err}")
-        finally:
-            os.unlink(mod_file.name)
-
-
-class LocalEnvironment(Environment):
-    def __init__(self, credentials: DuckDBCredentials):
-        self.conn = self.initialize_db(credentials)
-        self._plugins = self.initialize_plugins(credentials)
-        self.creds = credentials
-
-    def handle(self):
-        # Extensions/settings need to be configured per cursor
-        cursor = self.initialize_cursor(self.creds, self.conn.cursor())
-        return DuckDBConnectionWrapper(cursor)
-
-    def submit_python_job(self, handle, parsed_model: dict, compiled_code: str) -> AdapterResponse:
-        con = handle.cursor()
-
-        def ldf(table_name):
-            return con.query(f"select * from {table_name}")
-
-        self.run_python_job(con, ldf, parsed_model["alias"], compiled_code)
-        return AdapterResponse(_message="OK")
-
-    def load_source(self, plugin_name: str, source_config: SourceConfig):
-        if plugin_name not in self._plugins:
-            raise Exception(
-                f"Plugin {plugin_name} not found; known plugins are: "
-                + ",".join(self._plugins.keys())
+    @available
+    def location_exists(self, location: str) -> bool:
+        try:
+            self.execute(
+                f"select 1 from '{location}' where 1=0",
+                auto_begin=False,
+                fetch=False,
             )
-        plugin = self._plugins[plugin_name]
-        handle = self.handle()
-        cursor = handle.cursor()
-        save_mode = source_config.meta.get("save_mode", "overwrite")
-        if save_mode in ("ignore", "error_if_exists"):
-            schema, identifier = source_config.schema, source_config.identifier
-            q = f"""SELECT COUNT(1)
-                FROM information_schema.tables
-                WHERE table_schema = '{schema}'
-                AND table_name = '{identifier}'
-                """
-            if cursor.execute(q).fetchone()[0]:
-                if save_mode == "error_if_exists":
-                    raise Exception(f"Source {source_config.table_name()} already exists!")
-                else:
-                    # Nothing to do (we ignore the existing table)
-                    return
-        df = plugin.load(source_config)
-        assert df is not None
-        materialization = source_config.meta.get("materialization", "table")
-        cursor.execute(
-            f"CREATE OR REPLACE {materialization} {source_config.table_name()} AS SELECT * FROM df"
+            return True
+        except DbtRuntimeError:
+            return False
+
+    @available
+    def register_glue_table(
+        self,
+        glue_database: str,
+        table: str,
+        column_list: Sequence[Column],
+        location: str,
+        file_format: str,
+    ) -> None:
+        create_or_update_table(
+            database=glue_database,
+            table=table,
+            column_list=column_list,
+            s3_path=location,
+            file_format=file_format,
+            settings=self.config.credentials.settings,
         )
-        cursor.close()
-        handle.close()
 
-    def close(self):
-        if self.conn:
-            self.conn.close()
-            self.conn = None
+    @available
+    def external_root(self) -> str:
+        return self.config.credentials.external_root
+
+    @available
+    def use_database(self) -> bool:
+        return duckdb.__version__ >= "0.7.0"
+
+    @available
+    def get_binding_char(self):
+        return DuckDBConnectionManager.env().get_binding_char()
+
+    @available
+    def external_write_options(self, write_location: str, rendered_options: dict) -> str:
+        if "format" not in rendered_options:
+            ext = os.path.splitext(write_location)[1].lower()
+            if ext:
+                rendered_options["format"] = ext[1:]
+            elif "delimiter" in rendered_options:
+                rendered_options["format"] = "csv"
+            else:
+                rendered_options["format"] = "parquet"
 
-    def __del__(self):
-        self.close()
+        if rendered_options["format"] == "csv":
+            if "header" not in rendered_options:
+                rendered_options["header"] = 1
+
+        if "partition_by" in rendered_options:
+            v = rendered_options["partition_by"]
+            if "," in v and not v.startswith("("):
+                rendered_options["partition_by"] = f"({v})"
+
+        ret = []
+        for k, v in rendered_options.items():
+            if k.lower() in {
+                "delimiter",
+                "quote",
+                "escape",
+                "null",
+            } and not v.startswith("'"):
+                ret.append(f"{k} '{v}'")
+            else:
+                ret.append(f"{k} {v}")
+        return ", ".join(ret)
 
+    @available
+    def external_read_location(self, write_location: str, rendered_options: dict) -> str:
+        if rendered_options.get("partition_by"):
+            globs = [write_location, "*"]
+            partition_by = str(rendered_options.get("partition_by"))
+            globs.extend(["*"] * len(partition_by.split(",")))
+            return ".".join(["/".join(globs), str(rendered_options.get("format", "parquet"))])
+        return write_location
+
+    def valid_incremental_strategies(self) -> Sequence[str]:
+        """DuckDB does not currently support MERGE statement."""
+        return ["append", "delete+insert"]
 
-def create(creds: DuckDBCredentials) -> Environment:
-    if creds.remote:
-        from .buenavista import BVEnvironment
+    def commit_if_has_connection(self) -> None:
+        """This is just a quick-fix. Python models do not execute begin function so the transaction_open is always false."""
+        try:
+            self.connections.commit_if_has_connection()
+        except DbtInternalError:
+            pass
+
+    def submit_python_job(self, parsed_model: dict, compiled_code: str) -> AdapterResponse:
+        connection = self.connections.get_if_exists()
+        if not connection:
+            connection = self.connections.get_thread_connection()
+        env = DuckDBConnectionManager.env()
+        return env.submit_python_job(connection.handle, parsed_model, compiled_code)
+
+    def get_rows_different_sql(
+        self,
+        relation_a: BaseRelation,
+        relation_b: BaseRelation,
+        column_names: Optional[List[str]] = None,
+        except_operator: str = "EXCEPT",
+    ) -> str:
+        """Generate SQL for a query that returns a single row with a two
+        columns: the number of rows that are different between the two
+        relations and the number of mismatched rows.
+
+        This method only really exists for test reasons.
+        """
+        names: List[str]
+        if column_names is None:
+            columns = self.get_columns_in_relation(relation_a)
+            names = sorted((self.quote(c.name) for c in columns))
+        else:
+            names = sorted((self.quote(n) for n in column_names))
+        columns_csv = ", ".join(names)
+
+        sql = COLUMNS_EQUAL_SQL.format(
+            columns=columns_csv,
+            relation_a=str(relation_a),
+            relation_b=str(relation_b),
+            except_op=except_operator,
+        )
+        return sql
 
-        return BVEnvironment(creds)
-    else:
-        return LocalEnvironment(creds)
+    @available.parse(lambda *a, **k: [])
+    def get_column_schema_from_query(self, sql: str) -> List[Column]:
+        """Get a list of the Columns with names and data types from the given sql."""
+
+        # Taking advantage of yet another amazing DuckDB SQL feature right here: the
+        # ability to DESCRIBE a query instead of a relation
+        describe_sql = f"DESCRIBE ({sql})"
+        _, cursor = self.connections.add_select_query(describe_sql)
+        ret = []
+        for row in cursor.fetchall():
+            name, dtype = row[0], row[1]
+            ret.append(Column.create(name, dtype))
+        return ret
+
+    @classmethod
+    def render_column_constraint(cls, constraint: ColumnLevelConstraint) -> Optional[str]:
+        """Render the given constraint as DDL text. Should be overriden by adapters which need custom constraint
+        rendering."""
+        if constraint.type == ConstraintType.foreign_key:
+            # DuckDB doesn't support 'foreign key' as an alias
+            return f"references {constraint.expression}"
+        else:
+            return super().render_column_constraint(constraint)
+
+
+# Change `table_a/b` to `table_aaaaa/bbbbb` to avoid duckdb binding issues when relation_a/b
+# is called "table_a" or "table_b" in some of the dbt tests
+COLUMNS_EQUAL_SQL = """
+with diff_count as (
+    SELECT
+        1 as id,
+        COUNT(*) as num_missing FROM (
+            (SELECT {columns} FROM {relation_a} {except_op}
+             SELECT {columns} FROM {relation_b})
+             UNION ALL
+            (SELECT {columns} FROM {relation_b} {except_op}
+             SELECT {columns} FROM {relation_a})
+        ) as a
+), table_aaaaa as (
+    SELECT COUNT(*) as num_rows FROM {relation_a}
+), table_bbbbb as (
+    SELECT COUNT(*) as num_rows FROM {relation_b}
+), row_count_diff as (
+    select
+        1 as id,
+        table_aaaaa.num_rows - table_bbbbb.num_rows as difference
+    from table_aaaaa, table_bbbbb
+)
+select
+    row_count_diff.difference as row_count_difference,
+    diff_count.num_missing as num_mismatched
+from row_count_diff
+join diff_count using (id)
+""".strip()
```

### Comparing `dbt-duckdb-1.5.0rc1/dbt/adapters/duckdb/glue.py` & `dbt-duckdb-1.5.1/dbt/adapters/duckdb/glue.py`

 * *Files identical despite different names*

### Comparing `dbt-duckdb-1.5.0rc1/dbt/adapters/duckdb/plugins/__init__.py` & `dbt-duckdb-1.5.1/dbt/adapters/duckdb/plugins/__init__.py`

 * *Files identical despite different names*

### Comparing `dbt-duckdb-1.5.0rc1/dbt/adapters/duckdb/plugins/excel.py` & `dbt-duckdb-1.5.1/dbt/adapters/duckdb/plugins/excel.py`

 * *Files identical despite different names*

### Comparing `dbt-duckdb-1.5.0rc1/dbt/adapters/duckdb/plugins/gsheet.py` & `dbt-duckdb-1.5.1/dbt/adapters/duckdb/plugins/gsheet.py`

 * *Files identical despite different names*

### Comparing `dbt-duckdb-1.5.0rc1/dbt/adapters/duckdb/plugins/iceberg.py` & `dbt-duckdb-1.5.1/dbt/adapters/duckdb/plugins/iceberg.py`

 * *Files identical despite different names*

### Comparing `dbt-duckdb-1.5.0rc1/dbt/adapters/duckdb/plugins/sqlalchemy.py` & `dbt-duckdb-1.5.1/dbt/adapters/duckdb/plugins/sqlalchemy.py`

 * *Files identical despite different names*

### Comparing `dbt-duckdb-1.5.0rc1/dbt/adapters/duckdb/relation.py` & `dbt-duckdb-1.5.1/dbt/adapters/duckdb/relation.py`

 * *Files identical despite different names*

### Comparing `dbt-duckdb-1.5.0rc1/dbt/adapters/duckdb/utils.py` & `dbt-duckdb-1.5.1/dbt/adapters/duckdb/utils.py`

 * *Files 8% similar despite different names*

```diff
@@ -30,14 +30,16 @@
         base.update(self.meta)
         return base
 
     @classmethod
     def create(cls, source: SourceDefinition) -> "SourceConfig":
         meta = source.source_meta.copy()
         meta.update(source.meta)
+        # Use the config properties as well if they are present
+        meta.update(source.config._extra)
         return SourceConfig(
             name=source.name,
             identifier=source.identifier,
             schema=source.schema,
             database=source.database,
             meta=meta,
         )
```

### Comparing `dbt-duckdb-1.5.0rc1/dbt/include/duckdb/macros/adapters.sql` & `dbt-duckdb-1.5.1/dbt/include/duckdb/macros/adapters.sql`

 * *Files 10% similar despite different names*

```diff
@@ -24,48 +24,77 @@
         select count(*)
         from information_schema.schemata
         where schema_name='{{ schema }}'
   {%- endset %}
   {{ return(run_query(sql)) }}
 {% endmacro %}
 
+{% macro get_column_names() %}
+  {# loop through user_provided_columns to get column names #}
+    {%- set user_provided_columns = model['columns'] -%}
+    (
+    {% for i in user_provided_columns %}
+      {% set col = user_provided_columns[i] %}
+      {{ col['name'] }} {{ "," if not loop.last }}
+    {% endfor %}
+  )
+{% endmacro %}
+
+
 {% macro duckdb__create_table_as(temporary, relation, compiled_code, language='sql') -%}
   {%- if language == 'sql' -%}
+    {% set contract_config = config.get('contract') %}
+    {% if contract_config.enforced %}
+      {{ get_assert_columns_equivalent(compiled_code) }}
+    {% endif %}
     {%- set sql_header = config.get('sql_header', none) -%}
 
     {{ sql_header if sql_header is not none }}
 
     create {% if temporary: -%}temporary{%- endif %} table
       {{ relation.include(database=(not temporary and adapter.use_database()), schema=(not temporary)) }}
+  {% if contract_config.enforced and not temporary %}
+    {#-- DuckDB doesnt support constraints on temp tables --#}
+    {{ get_table_columns_and_constraints() }} ;
+    insert into {{ relation }} {{ get_column_names() }} (
+      {{ get_select_subquery(compiled_code) }}
+    );
+  {% else %}
     as (
       {{ compiled_code }}
     );
+  {% endif %}
   {%- elif language == 'python' -%}
     {{ py_write_table(temporary=temporary, relation=relation, compiled_code=compiled_code) }}
   {%- else -%}
       {% do exceptions.raise_compiler_error("duckdb__create_table_as macro didn't get supported language, it got %s" % language) %}
   {%- endif -%}
 {% endmacro %}
 
 {% macro py_write_table(temporary, relation, compiled_code) -%}
 {{ compiled_code }}
 
 def materialize(df, con):
     try:
         import pyarrow
+        pyarrow_available = True
     except ImportError:
-        pass
+        pyarrow_available = False
     finally:
-        if isinstance(df, pyarrow.Table):
+        if pyarrow_available and isinstance(df, pyarrow.Table):
             # https://github.com/duckdb/duckdb/issues/6584
             import pyarrow.dataset
     con.execute('create table {{ relation.include(database=adapter.use_database()) }} as select * from df')
 {% endmacro %}
 
 {% macro duckdb__create_view_as(relation, sql) -%}
+  {% set contract_config = config.get('contract') %}
+  {% if contract_config.enforced %}
+    {{ get_assert_columns_equivalent(sql) }}
+  {%- endif %}
   {%- set sql_header = config.get('sql_header', none) -%}
 
   {{ sql_header if sql_header is not none }}
   create view {{ relation.include(database=adapter.use_database()) }} as (
     {{ sql }}
   );
 {% endmacro %}
```

### Comparing `dbt-duckdb-1.5.0rc1/dbt/include/duckdb/macros/catalog.sql` & `dbt-duckdb-1.5.1/dbt/include/duckdb/macros/catalog.sql`

 * *Files identical despite different names*

### Comparing `dbt-duckdb-1.5.0rc1/dbt/include/duckdb/macros/materializations/external.sql` & `dbt-duckdb-1.5.1/dbt/include/duckdb/macros/materializations/external.sql`

 * *Files identical despite different names*

### Comparing `dbt-duckdb-1.5.0rc1/dbt/include/duckdb/macros/materializations/incremental.sql` & `dbt-duckdb-1.5.1/dbt/include/duckdb/macros/materializations/incremental.sql`

 * *Files identical despite different names*

### Comparing `dbt-duckdb-1.5.0rc1/dbt/include/duckdb/macros/materializations/table.sql` & `dbt-duckdb-1.5.1/dbt/include/duckdb/macros/materializations/table.sql`

 * *Files identical despite different names*

### Comparing `dbt-duckdb-1.5.0rc1/dbt/include/duckdb/macros/seed.sql` & `dbt-duckdb-1.5.1/dbt/include/duckdb/macros/seed.sql`

 * *Files identical despite different names*

### Comparing `dbt-duckdb-1.5.0rc1/dbt/include/duckdb/macros/snapshot_merge.sql` & `dbt-duckdb-1.5.1/dbt/include/duckdb/macros/snapshot_merge.sql`

 * *Files 18% similar despite different names*

```diff
@@ -1,21 +1,18 @@
 {% macro duckdb__snapshot_merge_sql(target, source, insert_cols) -%}
     {%- set insert_cols_csv = insert_cols | join(', ') -%}
 
-    {% set insert_sql %}
+    update {{ target }}
+    set dbt_valid_to = DBT_INTERNAL_SOURCE.dbt_valid_to
+    from {{ source }} as DBT_INTERNAL_SOURCE
+    where DBT_INTERNAL_SOURCE.dbt_scd_id::text = {{ target }}.dbt_scd_id::text
+      and DBT_INTERNAL_SOURCE.dbt_change_type::text in ('update'::text, 'delete'::text)
+      and {{ target }}.dbt_valid_to is null;
+
     insert into {{ target }} ({{ insert_cols_csv }})
     select {% for column in insert_cols -%}
         DBT_INTERNAL_SOURCE.{{ column }} {%- if not loop.last %}, {%- endif %}
     {%- endfor %}
     from {{ source }} as DBT_INTERNAL_SOURCE
-    where DBT_INTERNAL_SOURCE.dbt_change_type = 'insert';
-    {% endset %}
+    where DBT_INTERNAL_SOURCE.dbt_change_type::text = 'insert'::text;
 
-    {% do adapter.add_query(insert_sql, auto_begin=False) %}
-
-    update {{ target }}
-    set dbt_valid_to = DBT_INTERNAL_SOURCE.dbt_valid_to
-    from {{ source }} as DBT_INTERNAL_SOURCE
-    where DBT_INTERNAL_SOURCE.dbt_scd_id = {{ target.identifier }}.dbt_scd_id
-      and DBT_INTERNAL_SOURCE.dbt_change_type = 'update'
-      and {{ target.identifier }}.dbt_valid_to is null;
 {% endmacro %}
```

### Comparing `dbt-duckdb-1.5.0rc1/dbt/include/duckdb/macros/utils/datediff.sql` & `dbt-duckdb-1.5.1/dbt/include/duckdb/macros/utils/datediff.sql`

 * *Files identical despite different names*

### Comparing `dbt-duckdb-1.5.0rc1/dbt/include/duckdb/macros/utils/listagg.sql` & `dbt-duckdb-1.5.1/dbt/include/duckdb/macros/utils/listagg.sql`

 * *Files identical despite different names*

### Comparing `dbt-duckdb-1.5.0rc1/dbt/include/duckdb/macros/utils/upstream.sql` & `dbt-duckdb-1.5.1/dbt/include/duckdb/macros/utils/upstream.sql`

 * *Files identical despite different names*

### Comparing `dbt-duckdb-1.5.0rc1/dbt_duckdb.egg-info/PKG-INFO` & `dbt-duckdb-1.5.1/dbt_duckdb.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbt-duckdb
-Version: 1.5.0rc1
+Version: 1.5.1
 Summary: The duckdb adapter plugin for dbt (data build tool)
 Home-page: https://github.com/jwills/dbt-duckdb
 Author: Josh Wills
 Author-email: joshwills+dbt@gmail.com
 Description-Content-Type: text/markdown
 Provides-Extra: glue
 License-File: LICENSE
@@ -21,15 +21,15 @@
 
 ### Installation
 
 This project is hosted on PyPI, so you should be able to install it and the necessary dependencies via:
 
 `pip3 install dbt-duckdb`
 
-The latest supported version targets `dbt-core` 1.4.x and `duckdb` version 0.7.x, but we work hard to ensure that newer
+The latest supported version targets `dbt-core` 1.5.x and `duckdb` version 0.7.x, but we work hard to ensure that newer
 versions of DuckDB will continue to work with the adapter as they are released. If you would like to use our new (and experimental!)
 support for persisting the tables that DuckDB creates to the [AWS Glue Catalog](https://aws.amazon.com/glue/), you should install
 `dbt-duckdb[glue]` in order to get the AWS dependencies as well.
 
 ### Configuring Your Profile
 
 A minimal dbt-duckdb profile only needs two settings, `type` and `path`:
@@ -101,17 +101,17 @@
 illustrates the usage of this feature to connect to a Localstack instance running S3 from dbt-duckdb [here](https://github.com/jwills/s3-demo).
 
 #### Fetching credentials from context
 Instead of specifying the credentials through the settings block, you can also use the use_credential_provider property. If you set this to `aws` (currently the only supported implementation) and you have `boto3` installed in your python environment, we will fetch your AWS credentials using the credential provider chain as described [here](https://boto3.amazonaws.com/v1/documentation/api/latest/guide/credentials.html). This means that you can use any supported mechanism from AWS to obtain credentials (e.g., web identity tokens).
 
 #### Attaching Additional Databases
 
-DuckDB version `0.7.0` and dbt-duckdb version `1.4.0` support [attaching additional databases](https://duckdb.org/docs/sql/statements/attach.html) to your dbt-duckdb run so that you can read
+DuckDB version `0.7.0` added support for [attaching additional databases](https://duckdb.org/docs/sql/statements/attach.html) to your dbt-duckdb run so that you can read
 and write from multiple databases. Additional databases may be configured using [dbt run hooks](https://docs.getdbt.com/docs/build/hooks-operations) or via the `attach` argument
-in your profile:
+in your profile that was added in dbt-duckdb `1.4.0`:
 
 ```
 default:
   outputs:
     dev:
       type: duckdb
       path: /tmp/dbt.duckdb
```

### Comparing `dbt-duckdb-1.5.0rc1/dbt_duckdb.egg-info/SOURCES.txt` & `dbt-duckdb-1.5.1/dbt_duckdb.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -2,22 +2,23 @@
 MANIFEST.in
 README.md
 setup.py
 dbt/__init__.py
 dbt/adapters/__init__.py
 dbt/adapters/duckdb/__init__.py
 dbt/adapters/duckdb/__version__.py
-dbt/adapters/duckdb/buenavista.py
 dbt/adapters/duckdb/connections.py
 dbt/adapters/duckdb/credentials.py
-dbt/adapters/duckdb/environments.py
 dbt/adapters/duckdb/glue.py
 dbt/adapters/duckdb/impl.py
 dbt/adapters/duckdb/relation.py
 dbt/adapters/duckdb/utils.py
+dbt/adapters/duckdb/environments/__init__.py
+dbt/adapters/duckdb/environments/buenavista.py
+dbt/adapters/duckdb/environments/local.py
 dbt/adapters/duckdb/plugins/__init__.py
 dbt/adapters/duckdb/plugins/excel.py
 dbt/adapters/duckdb/plugins/gsheet.py
 dbt/adapters/duckdb/plugins/iceberg.py
 dbt/adapters/duckdb/plugins/sqlalchemy.py
 dbt/include/__init__.py
 dbt/include/duckdb/__init__.py
```

### Comparing `dbt-duckdb-1.5.0rc1/setup.py` & `dbt-duckdb-1.5.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -33,14 +33,14 @@
     long_description_content_type="text/markdown",
     author="Josh Wills",
     author_email="joshwills+dbt@gmail.com",
     url="https://github.com/jwills/dbt-duckdb",
     packages=find_namespace_packages(include=["dbt", "dbt.*"]),
     include_package_data=True,
     install_requires=[
-        "dbt-core~=1.5.0rc1",
+        "dbt-core~=1.5.0",
         "duckdb>=0.5.0",
     ],
     extras_require={
         "glue": ["boto3", "mypy-boto3-glue"],
     },
 )
```

