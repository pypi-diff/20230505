# Comparing `tmp/in-dbt-spark-1.2.512.tar.gz` & `tmp/in-dbt-spark-1.2.513.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "in-dbt-spark-1.2.512.tar", last modified: Fri Apr 28 10:15:06 2023, max compression
+gzip compressed data, was "in-dbt-spark-1.2.513.tar", last modified: Fri May  5 21:34:37 2023, max compression
```

## Comparing `in-dbt-spark-1.2.512.tar` & `in-dbt-spark-1.2.513.tar`

### file list

```diff
@@ -1,63 +1,63 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 10:15:06.597803 in-dbt-spark-1.2.512/
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-04-28 10:14:53.000000 in-dbt-spark-1.2.512/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     8027 2023-04-28 10:15:06.593803 in-dbt-spark-1.2.512/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7181 2023-04-28 10:14:53.000000 in-dbt-spark-1.2.512/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 10:15:06.585803 in-dbt-spark-1.2.512/dbt/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 10:15:06.585803 in-dbt-spark-1.2.512/dbt/adapters/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 10:15:06.589803 in-dbt-spark-1.2.512/dbt/adapters/setu/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-28 10:14:53.000000 in-dbt-spark-1.2.512/dbt/adapters/setu/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    10933 2023-04-28 10:14:53.000000 in-dbt-spark-1.2.512/dbt/adapters/setu/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     2833 2023-04-28 10:14:53.000000 in-dbt-spark-1.2.512/dbt/adapters/setu/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     8658 2023-04-28 10:14:53.000000 in-dbt-spark-1.2.512/dbt/adapters/setu/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     3604 2023-04-28 10:14:53.000000 in-dbt-spark-1.2.512/dbt/adapters/setu/session.py
--rw-r--r--   0 runner    (1001) docker     (123)     7518 2023-04-28 10:14:53.000000 in-dbt-spark-1.2.512/dbt/adapters/setu/session_cursor.py
--rw-r--r--   0 runner    (1001) docker     (123)     1867 2023-04-28 10:14:53.000000 in-dbt-spark-1.2.512/dbt/adapters/setu/session_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)    12139 2023-04-28 10:14:53.000000 in-dbt-spark-1.2.512/dbt/adapters/setu/session_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     8569 2023-04-28 10:14:53.000000 in-dbt-spark-1.2.512/dbt/adapters/setu/setu_session_request.py
--rw-r--r--   0 runner    (1001) docker     (123)     7236 2023-04-28 10:14:53.000000 in-dbt-spark-1.2.512/dbt/adapters/setu/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 10:15:06.589803 in-dbt-spark-1.2.512/dbt/adapters/spark/
--rw-r--r--   0 runner    (1001) docker     (123)      493 2023-04-28 10:14:53.000000 in-dbt-spark-1.2.512/dbt/adapters/spark/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-04-28 10:14:53.000000 in-dbt-spark-1.2.512/dbt/adapters/spark/__version__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2581 2023-04-28 10:14:53.000000 in-dbt-spark-1.2.512/dbt/adapters/spark/column.py
--rw-r--r--   0 runner    (1001) docker     (123)    24549 2023-04-28 10:14:53.000000 in-dbt-spark-1.2.512/dbt/adapters/spark/connections.py
--rw-r--r--   0 runner    (1001) docker     (123)    23998 2023-04-28 10:14:53.000000 in-dbt-spark-1.2.512/dbt/adapters/spark/impl.py
--rw-r--r--   0 runner    (1001) docker     (123)     1250 2023-04-28 10:14:53.000000 in-dbt-spark-1.2.512/dbt/adapters/spark/relation.py
--rw-r--r--   0 runner    (1001) docker     (123)     5315 2023-04-28 10:14:53.000000 in-dbt-spark-1.2.512/dbt/adapters/spark/session.py
--rw-r--r--   0 runner    (1001) docker     (123)      151 2023-04-28 10:14:53.000000 in-dbt-spark-1.2.512/dbt/adapters/spark/spark_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 10:15:06.585803 in-dbt-spark-1.2.512/dbt/include/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 10:15:06.589803 in-dbt-spark-1.2.512/dbt/include/spark/
--rw-r--r--   0 runner    (1001) docker     (123)       52 2023-04-28 10:14:53.000000 in-dbt-spark-1.2.512/dbt/include/spark/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-04-28 10:14:53.000000 in-dbt-spark-1.2.512/dbt/include/spark/dbt_project.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 10:15:06.589803 in-dbt-spark-1.2.512/dbt/include/spark/macros/
--rw-r--r--   0 runner    (1001) docker     (123)    14281 2023-04-28 10:14:53.000000 in-dbt-spark-1.2.512/dbt/include/spark/macros/adapters.sql
--rw-r--r--   0 runner    (1001) docker     (123)     3986 2023-04-28 10:14:53.000000 in-dbt-spark-1.2.512/dbt/include/spark/macros/apply_grants.sql
--rw-r--r--   0 runner    (1001) docker     (123)     1447 2023-04-28 10:14:53.000000 in-dbt-spark-1.2.512/dbt/include/spark/macros/apply_retention.sql
--rw-r--r--   0 runner    (1001) docker     (123)      582 2023-04-28 10:14:53.000000 in-dbt-spark-1.2.512/dbt/include/spark/macros/catalog.sql
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 10:15:06.593803 in-dbt-spark-1.2.512/dbt/include/spark/macros/materializations/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 10:15:06.593803 in-dbt-spark-1.2.512/dbt/include/spark/macros/materializations/incremental/
--rw-r--r--   0 runner    (1001) docker     (123)     2783 2023-04-28 10:14:53.000000 in-dbt-spark-1.2.512/dbt/include/spark/macros/materializations/incremental/incremental.sql
--rw-r--r--   0 runner    (1001) docker     (123)     3624 2023-04-28 10:14:53.000000 in-dbt-spark-1.2.512/dbt/include/spark/macros/materializations/incremental/strategies.sql
--rw-r--r--   0 runner    (1001) docker     (123)     2764 2023-04-28 10:14:53.000000 in-dbt-spark-1.2.512/dbt/include/spark/macros/materializations/seed.sql
--rw-r--r--   0 runner    (1001) docker     (123)    10684 2023-04-28 10:14:53.000000 in-dbt-spark-1.2.512/dbt/include/spark/macros/materializations/snapshot.sql
--rw-r--r--   0 runner    (1001) docker     (123)     1992 2023-04-28 10:14:53.000000 in-dbt-spark-1.2.512/dbt/include/spark/macros/materializations/table.sql
--rw-r--r--   0 runner    (1001) docker     (123)     4363 2023-04-28 10:14:53.000000 in-dbt-spark-1.2.512/dbt/include/spark/macros/materializations/validate.sql
--rw-r--r--   0 runner    (1001) docker     (123)      363 2023-04-28 10:14:53.000000 in-dbt-spark-1.2.512/dbt/include/spark/macros/materializations/view.sql
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 10:15:06.593803 in-dbt-spark-1.2.512/dbt/include/spark/macros/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      139 2023-04-28 10:14:53.000000 in-dbt-spark-1.2.512/dbt/include/spark/macros/utils/any_value.sql
--rw-r--r--   0 runner    (1001) docker     (123)      321 2023-04-28 10:14:53.000000 in-dbt-spark-1.2.512/dbt/include/spark/macros/utils/assert_not_null.sql
--rw-r--r--   0 runner    (1001) docker     (123)      372 2023-04-28 10:14:53.000000 in-dbt-spark-1.2.512/dbt/include/spark/macros/utils/bool_or.sql
--rw-r--r--   0 runner    (1001) docker     (123)       87 2023-04-28 10:14:53.000000 in-dbt-spark-1.2.512/dbt/include/spark/macros/utils/concat.sql
--rw-r--r--   0 runner    (1001) docker     (123)     2125 2023-04-28 10:14:53.000000 in-dbt-spark-1.2.512/dbt/include/spark/macros/utils/dateadd.sql
--rw-r--r--   0 runner    (1001) docker     (123)     4604 2023-04-28 10:14:53.000000 in-dbt-spark-1.2.512/dbt/include/spark/macros/utils/datediff.sql
--rw-r--r--   0 runner    (1001) docker     (123)      553 2023-04-28 10:14:53.000000 in-dbt-spark-1.2.512/dbt/include/spark/macros/utils/listagg.sql
--rw-r--r--   0 runner    (1001) docker     (123)      558 2023-04-28 10:14:53.000000 in-dbt-spark-1.2.512/dbt/include/spark/macros/utils/split_part.sql
--rw-r--r--   0 runner    (1001) docker     (123)      932 2023-04-28 10:14:53.000000 in-dbt-spark-1.2.512/dbt/include/spark/profile_template.yml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 10:15:06.593803 in-dbt-spark-1.2.512/in_dbt_spark.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8027 2023-04-28 10:15:06.000000 in-dbt-spark-1.2.512/in_dbt_spark.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1844 2023-04-28 10:15:06.000000 in-dbt-spark-1.2.512/in_dbt_spark.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-28 10:15:06.000000 in-dbt-spark-1.2.512/in_dbt_spark.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-28 10:15:06.000000 in-dbt-spark-1.2.512/in_dbt_spark.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      253 2023-04-28 10:15:06.000000 in-dbt-spark-1.2.512/in_dbt_spark.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        4 2023-04-28 10:15:06.000000 in-dbt-spark-1.2.512/in_dbt_spark.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-28 10:15:06.597803 in-dbt-spark-1.2.512/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3364 2023-04-28 10:14:53.000000 in-dbt-spark-1.2.512/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 21:34:37.938717 in-dbt-spark-1.2.513/
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-05-05 21:34:25.000000 in-dbt-spark-1.2.513/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     8027 2023-05-05 21:34:37.938717 in-dbt-spark-1.2.513/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7181 2023-05-05 21:34:25.000000 in-dbt-spark-1.2.513/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 21:34:37.934718 in-dbt-spark-1.2.513/dbt/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 21:34:37.934718 in-dbt-spark-1.2.513/dbt/adapters/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 21:34:37.934718 in-dbt-spark-1.2.513/dbt/adapters/setu/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 21:34:25.000000 in-dbt-spark-1.2.513/dbt/adapters/setu/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10933 2023-05-05 21:34:25.000000 in-dbt-spark-1.2.513/dbt/adapters/setu/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2833 2023-05-05 21:34:25.000000 in-dbt-spark-1.2.513/dbt/adapters/setu/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8658 2023-05-05 21:34:25.000000 in-dbt-spark-1.2.513/dbt/adapters/setu/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3604 2023-05-05 21:34:25.000000 in-dbt-spark-1.2.513/dbt/adapters/setu/session.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7518 2023-05-05 21:34:25.000000 in-dbt-spark-1.2.513/dbt/adapters/setu/session_cursor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1867 2023-05-05 21:34:25.000000 in-dbt-spark-1.2.513/dbt/adapters/setu/session_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12139 2023-05-05 21:34:25.000000 in-dbt-spark-1.2.513/dbt/adapters/setu/session_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8569 2023-05-05 21:34:25.000000 in-dbt-spark-1.2.513/dbt/adapters/setu/setu_session_request.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7236 2023-05-05 21:34:25.000000 in-dbt-spark-1.2.513/dbt/adapters/setu/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 21:34:37.938717 in-dbt-spark-1.2.513/dbt/adapters/spark/
+-rw-r--r--   0 runner    (1001) docker     (123)      493 2023-05-05 21:34:25.000000 in-dbt-spark-1.2.513/dbt/adapters/spark/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-05-05 21:34:25.000000 in-dbt-spark-1.2.513/dbt/adapters/spark/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2581 2023-05-05 21:34:25.000000 in-dbt-spark-1.2.513/dbt/adapters/spark/column.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24549 2023-05-05 21:34:25.000000 in-dbt-spark-1.2.513/dbt/adapters/spark/connections.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25223 2023-05-05 21:34:25.000000 in-dbt-spark-1.2.513/dbt/adapters/spark/impl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1250 2023-05-05 21:34:25.000000 in-dbt-spark-1.2.513/dbt/adapters/spark/relation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5315 2023-05-05 21:34:25.000000 in-dbt-spark-1.2.513/dbt/adapters/spark/session.py
+-rw-r--r--   0 runner    (1001) docker     (123)      151 2023-05-05 21:34:25.000000 in-dbt-spark-1.2.513/dbt/adapters/spark/spark_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 21:34:37.934718 in-dbt-spark-1.2.513/dbt/include/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 21:34:37.938717 in-dbt-spark-1.2.513/dbt/include/spark/
+-rw-r--r--   0 runner    (1001) docker     (123)       52 2023-05-05 21:34:25.000000 in-dbt-spark-1.2.513/dbt/include/spark/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-05-05 21:34:25.000000 in-dbt-spark-1.2.513/dbt/include/spark/dbt_project.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 21:34:37.938717 in-dbt-spark-1.2.513/dbt/include/spark/macros/
+-rw-r--r--   0 runner    (1001) docker     (123)    14409 2023-05-05 21:34:25.000000 in-dbt-spark-1.2.513/dbt/include/spark/macros/adapters.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     3986 2023-05-05 21:34:25.000000 in-dbt-spark-1.2.513/dbt/include/spark/macros/apply_grants.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     1524 2023-05-05 21:34:25.000000 in-dbt-spark-1.2.513/dbt/include/spark/macros/apply_retention.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      582 2023-05-05 21:34:25.000000 in-dbt-spark-1.2.513/dbt/include/spark/macros/catalog.sql
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 21:34:37.938717 in-dbt-spark-1.2.513/dbt/include/spark/macros/materializations/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 21:34:37.938717 in-dbt-spark-1.2.513/dbt/include/spark/macros/materializations/incremental/
+-rw-r--r--   0 runner    (1001) docker     (123)     3024 2023-05-05 21:34:25.000000 in-dbt-spark-1.2.513/dbt/include/spark/macros/materializations/incremental/incremental.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     3624 2023-05-05 21:34:25.000000 in-dbt-spark-1.2.513/dbt/include/spark/macros/materializations/incremental/strategies.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     2764 2023-05-05 21:34:25.000000 in-dbt-spark-1.2.513/dbt/include/spark/macros/materializations/seed.sql
+-rw-r--r--   0 runner    (1001) docker     (123)    10891 2023-05-05 21:34:25.000000 in-dbt-spark-1.2.513/dbt/include/spark/macros/materializations/snapshot.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     2225 2023-05-05 21:34:25.000000 in-dbt-spark-1.2.513/dbt/include/spark/macros/materializations/table.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     6562 2023-05-05 21:34:25.000000 in-dbt-spark-1.2.513/dbt/include/spark/macros/materializations/validate.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      363 2023-05-05 21:34:25.000000 in-dbt-spark-1.2.513/dbt/include/spark/macros/materializations/view.sql
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 21:34:37.938717 in-dbt-spark-1.2.513/dbt/include/spark/macros/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      139 2023-05-05 21:34:25.000000 in-dbt-spark-1.2.513/dbt/include/spark/macros/utils/any_value.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      321 2023-05-05 21:34:25.000000 in-dbt-spark-1.2.513/dbt/include/spark/macros/utils/assert_not_null.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      372 2023-05-05 21:34:25.000000 in-dbt-spark-1.2.513/dbt/include/spark/macros/utils/bool_or.sql
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-05-05 21:34:25.000000 in-dbt-spark-1.2.513/dbt/include/spark/macros/utils/concat.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     2125 2023-05-05 21:34:25.000000 in-dbt-spark-1.2.513/dbt/include/spark/macros/utils/dateadd.sql
+-rw-r--r--   0 runner    (1001) docker     (123)     4604 2023-05-05 21:34:25.000000 in-dbt-spark-1.2.513/dbt/include/spark/macros/utils/datediff.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      553 2023-05-05 21:34:25.000000 in-dbt-spark-1.2.513/dbt/include/spark/macros/utils/listagg.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      558 2023-05-05 21:34:25.000000 in-dbt-spark-1.2.513/dbt/include/spark/macros/utils/split_part.sql
+-rw-r--r--   0 runner    (1001) docker     (123)      932 2023-05-05 21:34:25.000000 in-dbt-spark-1.2.513/dbt/include/spark/profile_template.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 21:34:37.938717 in-dbt-spark-1.2.513/in_dbt_spark.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8027 2023-05-05 21:34:37.000000 in-dbt-spark-1.2.513/in_dbt_spark.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1844 2023-05-05 21:34:37.000000 in-dbt-spark-1.2.513/in_dbt_spark.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 21:34:37.000000 in-dbt-spark-1.2.513/in_dbt_spark.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 21:34:37.000000 in-dbt-spark-1.2.513/in_dbt_spark.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      253 2023-05-05 21:34:37.000000 in-dbt-spark-1.2.513/in_dbt_spark.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        4 2023-05-05 21:34:37.000000 in-dbt-spark-1.2.513/in_dbt_spark.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-05 21:34:37.942717 in-dbt-spark-1.2.513/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3364 2023-05-05 21:34:25.000000 in-dbt-spark-1.2.513/setup.py
```

### Comparing `in-dbt-spark-1.2.512/PKG-INFO` & `in-dbt-spark-1.2.513/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: in-dbt-spark
-Version: 1.2.512
+Version: 1.2.513
 Summary: Release for LinkedIn's changes to dbt-spark.
 Home-page: https://github.com/linkedin/in-dbt-spark
 Author: LinkedIn DBT Team
 Author-email: dbt-dev@linkedin.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: Microsoft :: Windows
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: in-dbt-spark Version: 1.2.512 Summary: Release for
+Metadata-Version: 2.1 Name: in-dbt-spark Version: 1.2.513 Summary: Release for
 LinkedIn's changes to dbt-spark. Home-page: https://github.com/linkedin/in-dbt-
 spark Author: LinkedIn DBT Team Author-email: dbt-dev@linkedin.com Classifier:
 Development Status :: 5 - Production/Stable Classifier: License :: OSI Approved
 :: Apache Software License Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: MacOS :: MacOS X Classifier: Operating System
 :: POSIX :: Linux Classifier: Programming Language :: Python :: 3.7 Classifier:
 Programming Language :: Python :: 3.8 Classifier: Programming Language ::
```

### Comparing `in-dbt-spark-1.2.512/README.md` & `in-dbt-spark-1.2.513/README.md`

 * *Files identical despite different names*

### Comparing `in-dbt-spark-1.2.512/dbt/adapters/setu/client.py` & `in-dbt-spark-1.2.513/dbt/adapters/setu/client.py`

 * *Files identical despite different names*

### Comparing `in-dbt-spark-1.2.512/dbt/adapters/setu/constants.py` & `in-dbt-spark-1.2.513/dbt/adapters/setu/constants.py`

 * *Files identical despite different names*

### Comparing `in-dbt-spark-1.2.512/dbt/adapters/setu/models.py` & `in-dbt-spark-1.2.513/dbt/adapters/setu/models.py`

 * *Files identical despite different names*

### Comparing `in-dbt-spark-1.2.512/dbt/adapters/setu/session.py` & `in-dbt-spark-1.2.513/dbt/adapters/setu/session.py`

 * *Files identical despite different names*

### Comparing `in-dbt-spark-1.2.512/dbt/adapters/setu/session_cursor.py` & `in-dbt-spark-1.2.513/dbt/adapters/setu/session_cursor.py`

 * *Files identical despite different names*

### Comparing `in-dbt-spark-1.2.512/dbt/adapters/setu/session_handler.py` & `in-dbt-spark-1.2.513/dbt/adapters/setu/session_handler.py`

 * *Files identical despite different names*

### Comparing `in-dbt-spark-1.2.512/dbt/adapters/setu/session_manager.py` & `in-dbt-spark-1.2.513/dbt/adapters/setu/session_manager.py`

 * *Files identical despite different names*

### Comparing `in-dbt-spark-1.2.512/dbt/adapters/setu/setu_session_request.py` & `in-dbt-spark-1.2.513/dbt/adapters/setu/setu_session_request.py`

 * *Files identical despite different names*

### Comparing `in-dbt-spark-1.2.512/dbt/adapters/setu/utils.py` & `in-dbt-spark-1.2.513/dbt/adapters/setu/utils.py`

 * *Files identical despite different names*

### Comparing `in-dbt-spark-1.2.512/dbt/adapters/spark/column.py` & `in-dbt-spark-1.2.513/dbt/adapters/spark/column.py`

 * *Files identical despite different names*

### Comparing `in-dbt-spark-1.2.512/dbt/adapters/spark/connections.py` & `in-dbt-spark-1.2.513/dbt/adapters/spark/connections.py`

 * *Files identical despite different names*

### Comparing `in-dbt-spark-1.2.512/dbt/adapters/spark/impl.py` & `in-dbt-spark-1.2.513/dbt/adapters/spark/impl.py`

 * *Files 4% similar despite different names*

```diff
@@ -16,18 +16,19 @@
 
 from dbt.adapters.base import AdapterConfig
 from dbt.adapters.base.impl import catch_as_completed
 from dbt.adapters.sql import SQLAdapter
 from dbt.adapters.spark import SparkConnectionManager
 from dbt.adapters.spark import SparkRelation
 from dbt.adapters.spark import SparkColumn
-from dbt.adapters.base import BaseRelation
+from dbt.adapters.base import BaseRelation, available
 from dbt.clients.agate_helper import DEFAULT_TYPE_TESTER
 from dbt.events import AdapterLogger
 from dbt.utils import executor, AttrDict
+from dbt.dataclass_schema import dbtClassMixin, ValidationError
 
 logger = AdapterLogger("Spark")
 
 GET_COLUMNS_IN_RELATION_RAW_MACRO_NAME = "get_columns_in_relation_raw"
 LIST_SCHEMAS_MACRO_NAME = "list_schemas"
 LIST_RELATIONS_MACRO_NAME = "list_relations_without_caching"
 LIST_RELATIONS_SHOW_TABLES_MACRO_NAME = "list_relations_show_tables_without_caching"
@@ -47,19 +48,42 @@
     "[TABLE_OR_VIEW_NOT_FOUND]",
     "Table or view not found",
     "NoSuchTableException",
 )
 
 
 @dataclass
+class PartitionConfig(dbtClassMixin):
+    field: str
+    data_type: str
+    granularity: Optional[str] = None
+
+    @classmethod
+    def parse(cls, partition_by) -> Optional["PartitionConfig"]:
+
+        if partition_by is None:
+            return None
+        try:
+            cls.validate(partition_by)
+            return cls.from_dict(partition_by)
+        except ValidationError as exc:
+            raise dbt.exceptions.ValidationException("Could not parse partition config") from exc
+        except TypeError:
+            raise dbt.exceptions.CompilationError(
+                f"Invalid partition_by config:\n"
+                f"  Got: {partition_by}\n"
+                f'  Expected a dictionary with "field" and "data_type" keys'
+            )
+
+
+@dataclass
 class SparkConfig(AdapterConfig):
     file_format: str = "openhouse"
     location_root: Optional[str] = None
-    partition_by: Optional[Union[List[str], str]] = None
-    partition_granularity: Optional[str] = None
+    partition_by: Optional[Union[List[Dict[str, str]], Dict[str, str]]] = None
     retention_period: Optional[str] = None
     clustered_by: Optional[Union[List[str], str]] = None
     buckets: Optional[int] = None
     options: Optional[Dict[str, str]] = None
     merge_update_columns: Optional[str] = None
 
 
@@ -563,14 +587,25 @@
                     else:
                         current_catalog = None
             yield
         finally:
             if current_catalog is not None:
                 self.execute_macro(USE_CATALOG_MACRO_NAME, kwargs=dict(catalog=current_catalog))
 
+    @available
+    def parse_partition_by(self, raw_partition_by: Any):
+        partition_by_list = []
+        if raw_partition_by is None:
+            return None
+        if isinstance(raw_partition_by, dict):
+            raw_partition_by = [raw_partition_by]
+        for partition_by in raw_partition_by:
+            partition_by_list.append(PartitionConfig.parse(partition_by))
+        return partition_by_list
+
 
 # spark does something interesting with joins when both tables have the same
 # static values for the join condition and complains that the join condition is
 # "trivial". Which is true, though it seems like an unreasonable cause for
 # failure! It also doesn't like the `from foo, bar` syntax as opposed to
 # `from foo cross join bar`.
 COLUMNS_EQUAL_SQL = """
```

### Comparing `in-dbt-spark-1.2.512/dbt/adapters/spark/relation.py` & `in-dbt-spark-1.2.513/dbt/adapters/spark/relation.py`

 * *Files identical despite different names*

### Comparing `in-dbt-spark-1.2.512/dbt/adapters/spark/session.py` & `in-dbt-spark-1.2.513/dbt/adapters/spark/session.py`

 * *Files identical despite different names*

### Comparing `in-dbt-spark-1.2.512/dbt/include/spark/macros/adapters.sql` & `in-dbt-spark-1.2.513/dbt/include/spark/macros/adapters.sql`

 * *Files 5% similar despite different names*

```diff
@@ -80,31 +80,30 @@
 
 
 {% macro partition_cols(label, required=false) %}
   {{ return(adapter.dispatch('partition_cols', 'dbt')(label, required)) }}
 {%- endmacro -%}
 
 {% macro spark__partition_cols(label, required=false) %}
-  {%- set cols = config.get('partition_by', validator=validation.any[list, basestring]) -%}
+  {%- set raw_partition_by = config.get('partition_by', validator=validation.any[list, dict]) -%}
   {%- set file_format = config.get('file_format', validator=validation.any[basestring]) -%}
-  {%- set granularity = config.get('partition_granularity', validator=validation.any[basestring]) -%}
 
-  {%- if cols is not none %}
-    {% if file_format == 'openhouse' and granularity is none %}
-      {{ exceptions.raise_compiler_error("For partitioned tables with file_format = 'openhouse', 'partition_granularity' must be supplied (one of 'hours', 'days', 'months', or 'years').") }}
-    {% endif %}
-    {%- if cols is string -%}
-      {%- set cols = [cols] -%}
-    {%- endif -%}
+  {%- if raw_partition_by is not none %}
     {{ label }} (
-    {%- for item in cols -%}
-      {%- if file_format == 'openhouse' -%}
-        {{ granularity }}({{ item }})
+    {%- set partition_by_list = adapter.parse_partition_by(raw_partition_by) -%}
+    {%- for partition_by in partition_by_list -%}
+      {%- if file_format == 'openhouse' and partition_by.data_type | lower in ['timestamp'] -%}
+        {%- if partition_by.granularity is none -%}
+          {% do exceptions.raise_compiler_error("For partitioned tables with file_format = 'openhouse' and data_type = 'timestamp', granularity must be provided") %}
+        {%- endif -%}
+        {{ partition_by.granularity }}({{ partition_by.field }})
+      {%- elif file_format == 'openhouse' and partition_by.data_type | lower in ['string'] -%}
+        {{ partition_by.field }}
       {%- else -%}
-        {{ item }}
+        {{ partition_by.field }}
       {%- endif -%}
       {%- if not loop.last -%},{%- endif -%}
     {%- endfor -%}
     )
   {%- endif %}
 {%- endmacro -%}
```

### Comparing `in-dbt-spark-1.2.512/dbt/include/spark/macros/apply_grants.sql` & `in-dbt-spark-1.2.513/dbt/include/spark/macros/apply_grants.sql`

 * *Files identical despite different names*

### Comparing `in-dbt-spark-1.2.512/dbt/include/spark/macros/catalog.sql` & `in-dbt-spark-1.2.513/dbt/include/spark/macros/catalog.sql`

 * *Files identical despite different names*

### Comparing `in-dbt-spark-1.2.512/dbt/include/spark/macros/materializations/incremental/incremental.sql` & `in-dbt-spark-1.2.513/dbt/include/spark/macros/materializations/incremental/incremental.sql`

 * *Files 15% similar despite different names*

```diff
@@ -1,45 +1,47 @@
 {% materialization incremental, adapter='spark' -%}
 
   {#-- Validate early so we don't run SQL if the file_format + strategy combo is invalid --#}
   {%- set raw_file_format = config.get('file_format', default='openhouse') -%}
   {%- set raw_strategy = config.get('incremental_strategy', default='append') -%}
   {%- set grant_config = config.get('grants') -%}
+  {%- set raw_retention = config.get('retention_period', none) -%}
 
   {%- set file_format = dbt_spark_validate_get_file_format(raw_file_format) -%}
   {%- set file_format = dbt_spark_validate_openhouse_configs(file_format) -%}
   {%- set strategy = dbt_spark_validate_get_incremental_strategy(raw_strategy, file_format) -%}
+  {%- set retention = dbt_spark_validate_retention_configs(raw_retention,file_format) -%}
 
   {%- set catalog -%}
     {%- if not file_format == 'openhouse' -%}
       spark_catalog
     {%- else %}
       openhouse
     {%- endif -%}
   {%- endset -%}
 
   {%- set unique_key = config.get('unique_key', none) -%}
-  {%- set partition_by = config.get('partition_by', none) -%}
+  {%- set raw_partition_by = config.get('partition_by', none) -%}
 
   {%- set full_refresh_mode = (should_full_refresh()) -%}
 
   {% set on_schema_change = incremental_validate_on_schema_change(config.get('on_schema_change'), default='ignore') %}
 
   {% set target_relation = this %}
   {% set existing_relation = load_relation(this) %}
   {% set tmp_relation = make_temp_relation(this) %}
 
-  {% if strategy == 'insert_overwrite' and partition_by %}
+  {% if strategy == 'insert_overwrite' and raw_partition_by %}
     {% call statement() %}
       set spark.sql.sources.partitionOverwriteMode = DYNAMIC
     {% endcall %}
   {% endif %}
 
-  {# -- First, run USE statement to select correct catalog between OH and Hive #}
-  {% do adapter.dispatch('use_catalog', 'dbt')(catalog) %}
+  {# -- TODO: DATAFND-1122 Hard coding the catalog as a workaround for APA-75325. Need to remove this once the spark v2 fix is deployed #}
+  {% do adapter.dispatch('use_catalog', 'dbt')('spark_catalog') %}
 
   {{ run_hooks(pre_hooks) }}
 
   {% set is_delta = (file_format == 'delta' and existing_relation.is_delta) %}
 
   {% if existing_relation is none %}
     {% set build_sql = create_table_as(False, target_relation, sql) %}
@@ -56,15 +58,15 @@
 
   {%- call statement('main') -%}
     {{ build_sql }}
   {%- endcall -%}
 
   {% set should_revoke = should_revoke(existing_relation, full_refresh_mode) %}
   {% do apply_grants(target_relation, grant_config, should_revoke) %}
-  {% do apply_retention(target_relation) %}
+  {% do apply_retention(target_relation, retention) %}
   {% do persist_docs(target_relation, model) %}
 
   {{ run_hooks(post_hooks) }}
 
   {{ return({'relations': [target_relation]}) }}
 
 {%- endmaterialization %}
```

### Comparing `in-dbt-spark-1.2.512/dbt/include/spark/macros/materializations/incremental/strategies.sql` & `in-dbt-spark-1.2.513/dbt/include/spark/macros/materializations/incremental/strategies.sql`

 * *Files identical despite different names*

### Comparing `in-dbt-spark-1.2.512/dbt/include/spark/macros/materializations/seed.sql` & `in-dbt-spark-1.2.513/dbt/include/spark/macros/materializations/seed.sql`

 * *Files identical despite different names*

### Comparing `in-dbt-spark-1.2.512/dbt/include/spark/macros/materializations/snapshot.sql` & `in-dbt-spark-1.2.513/dbt/include/spark/macros/materializations/snapshot.sql`

 * *Files 2% similar despite different names*

```diff
@@ -150,14 +150,17 @@
     {% do exceptions.raise_compiler_error("Self-serve schema creation is not currently supported in OpenHouse. Please reach out in #ask_openhouse to manually provision your database.") %}
   {% endif %}
 
   {%- if not target_relation.is_table -%}
     {% do exceptions.relation_wrong_type(target_relation, 'table') %}
   {%- endif -%}
 
+  {# -- TODO: DATAFND-1122 Hard coding the catalog as a workaround for APA-75325. Need to remove this once the spark v2 fix is deployed #}
+  {% do adapter.dispatch('use_catalog', 'dbt')('spark_catalog') %}
+
   {{ run_hooks(pre_hooks, inside_transaction=False) }}
 
   {{ run_hooks(pre_hooks, inside_transaction=True) }}
 
   {% set strategy_macro = strategy_dispatch(strategy_name) %}
   {% set strategy = strategy_macro(model, "snapshotted_data", "source_data", config, target_relation_exists) %}
```

### Comparing `in-dbt-spark-1.2.512/dbt/include/spark/macros/materializations/table.sql` & `in-dbt-spark-1.2.513/dbt/include/spark/macros/materializations/table.sql`

 * *Files 11% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 {% materialization table, adapter = 'spark' %}
 
   {%- set identifier = model['alias'] -%}
   {%- set grant_config = config.get('grants') -%}
+  {%- set raw_retention = config.get('retention_period', none) -%}
 
   {%- set raw_file_format = config.get('file_format', default='openhouse') -%}
   {%- set file_format = dbt_spark_validate_openhouse_configs(raw_file_format) -%}
+  {%- set retention = dbt_spark_validate_retention_configs(raw_retention,file_format) -%}
 
   {%- set catalog -%}
     {%- if not file_format == 'openhouse' -%}
       spark_catalog
     {%- else %}
       openhouse
     {%- endif -%}
@@ -16,16 +18,16 @@
 
   {%- set old_relation = adapter.get_relation(database=database, schema=schema, identifier=identifier) -%}
   {%- set target_relation = api.Relation.create(identifier=identifier,
                                                 schema=schema,
                                                 database=database,
                                                 type='table') -%}
 
-  {# -- First, run USE statement to select correct catalog between OH and Hive #}
-  {% do adapter.dispatch('use_catalog', 'dbt')(catalog) %}
+  {# -- TODO: DATAFND-1122 Hard coding the catalog as a workaround for APA-75325. Need to remove this once the spark v2 fix is deployed #}
+  {% do adapter.dispatch('use_catalog', 'dbt')('spark_catalog') %}
 
   {{ run_hooks(pre_hooks) }}
 
   -- setup: if the target relation already exists, drop it
   -- in case if the existing and future table is delta, we want to do a
   -- create or replace table instead of dropping, so we don't have the table unavailable
   {% if old_relation and not (old_relation.is_delta and file_format == 'delta') -%}
@@ -39,15 +41,15 @@
   -- build model
   {% call statement('main') -%}
     {{ create_table_as(False, target_relation, sql) }}
   {%- endcall %}
 
   {% set should_revoke = should_revoke(old_relation, full_refresh_mode=True) %}
   {% do apply_grants(target_relation, grant_config, should_revoke) %}
-  {% do apply_retention(target_relation) %}
+  {% do apply_retention(target_relation, retention) %}
   {% do persist_docs(target_relation, model) %}
 
   {{ run_hooks(post_hooks) }}
 
   {{ return({'relations': [target_relation]})}}
 
 {% endmaterialization %}
```

### Comparing `in-dbt-spark-1.2.512/dbt/include/spark/macros/utils/dateadd.sql` & `in-dbt-spark-1.2.513/dbt/include/spark/macros/utils/dateadd.sql`

 * *Files identical despite different names*

### Comparing `in-dbt-spark-1.2.512/dbt/include/spark/macros/utils/datediff.sql` & `in-dbt-spark-1.2.513/dbt/include/spark/macros/utils/datediff.sql`

 * *Files identical despite different names*

### Comparing `in-dbt-spark-1.2.512/dbt/include/spark/macros/utils/listagg.sql` & `in-dbt-spark-1.2.513/dbt/include/spark/macros/utils/listagg.sql`

 * *Files identical despite different names*

### Comparing `in-dbt-spark-1.2.512/dbt/include/spark/macros/utils/split_part.sql` & `in-dbt-spark-1.2.513/dbt/include/spark/macros/utils/split_part.sql`

 * *Files identical despite different names*

### Comparing `in-dbt-spark-1.2.512/dbt/include/spark/profile_template.yml` & `in-dbt-spark-1.2.513/dbt/include/spark/profile_template.yml`

 * *Files identical despite different names*

### Comparing `in-dbt-spark-1.2.512/in_dbt_spark.egg-info/PKG-INFO` & `in-dbt-spark-1.2.513/in_dbt_spark.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: in-dbt-spark
-Version: 1.2.512
+Version: 1.2.513
 Summary: Release for LinkedIn's changes to dbt-spark.
 Home-page: https://github.com/linkedin/in-dbt-spark
 Author: LinkedIn DBT Team
 Author-email: dbt-dev@linkedin.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: Microsoft :: Windows
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: in-dbt-spark Version: 1.2.512 Summary: Release for
+Metadata-Version: 2.1 Name: in-dbt-spark Version: 1.2.513 Summary: Release for
 LinkedIn's changes to dbt-spark. Home-page: https://github.com/linkedin/in-dbt-
 spark Author: LinkedIn DBT Team Author-email: dbt-dev@linkedin.com Classifier:
 Development Status :: 5 - Production/Stable Classifier: License :: OSI Approved
 :: Apache Software License Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: MacOS :: MacOS X Classifier: Operating System
 :: POSIX :: Linux Classifier: Programming Language :: Python :: 3.7 Classifier:
 Programming Language :: Python :: 3.8 Classifier: Programming Language ::
```

### Comparing `in-dbt-spark-1.2.512/in_dbt_spark.egg-info/SOURCES.txt` & `in-dbt-spark-1.2.513/in_dbt_spark.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `in-dbt-spark-1.2.512/setup.py` & `in-dbt-spark-1.2.513/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -46,15 +46,15 @@
     parts = _get_plugin_version_dict()
     minor = "{major}.{minor}.0".format(**parts)
     pre = parts["prekind"] + "1" if parts["prekind"] else ""
     return f"{minor}{pre}"
 
 
 package_name = "in-dbt-spark"
-package_version = "1.2.512"
+package_version = "1.2.513"
 dbt_core_version = _get_dbt_core_version()
 description = """Release for LinkedIn's changes to dbt-spark."""
 
 odbc_extras = ["pyodbc>=4.0.30"]
 pyhive_extras = [
     "PyHive[hive]>=0.6.0,<0.7.0",
     "thrift>=0.11.0,<0.16.0",
```

