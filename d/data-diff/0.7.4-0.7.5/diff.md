# Comparing `tmp/data_diff-0.7.4.tar.gz` & `tmp/data_diff-0.7.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "data_diff-0.7.4.tar", max compression
+gzip compressed data, was "data_diff-0.7.5.tar", max compression
```

## Comparing `data_diff-0.7.4.tar` & `data_diff-0.7.5.tar`

### file list

```diff
@@ -1,72 +1,72 @@
--rw-r--r--   0        0        0     1053 2023-04-03 18:06:26.931220 data_diff-0.7.4/LICENSE
--rw-r--r--   0        0        0     4773 2023-04-14 15:23:33.906410 data_diff-0.7.4/README.md
--rw-r--r--   0        0        0     8429 2023-04-21 21:58:08.193898 data_diff-0.7.4/data_diff/__init__.py
--rw-r--r--   0        0        0    15816 2023-04-21 21:58:08.194100 data_diff-0.7.4/data_diff/__main__.py
--rw-r--r--   0        0        0      108 2023-04-14 15:23:33.906548 data_diff-0.7.4/data_diff/cloud/__init__.py
--rw-r--r--   0        0        0    11594 2023-04-21 21:58:08.194331 data_diff-0.7.4/data_diff/cloud/data_source.py
--rw-r--r--   0        0        0     9253 2023-04-21 21:58:08.194472 data_diff-0.7.4/data_diff/cloud/datafold_api.py
--rw-r--r--   0        0        0     4044 2023-04-03 18:06:26.931568 data_diff-0.7.4/data_diff/config.py
--rw-r--r--   0        0        0      493 2023-04-21 21:58:08.194615 data_diff-0.7.4/data_diff/databases/__init__.py
--rw-r--r--   0        0        0     1353 2023-04-21 21:58:08.194720 data_diff-0.7.4/data_diff/databases/_connect.py
--rw-r--r--   0        0        0      174 2023-04-21 21:58:08.194816 data_diff-0.7.4/data_diff/databases/base.py
--rw-r--r--   0        0        0      257 2023-04-21 21:58:08.195148 data_diff-0.7.4/data_diff/databases/bigquery.py
--rw-r--r--   0        0        0      271 2023-04-21 21:58:08.195281 data_diff-0.7.4/data_diff/databases/clickhouse.py
--rw-r--r--   0        0        0      271 2023-04-21 21:58:08.195390 data_diff-0.7.4/data_diff/databases/databricks.py
--rw-r--r--   0        0        0      243 2023-04-21 21:58:08.195511 data_diff-0.7.4/data_diff/databases/duckdb.py
--rw-r--r--   0        0        0      236 2023-04-21 21:58:08.195617 data_diff-0.7.4/data_diff/databases/mysql.py
--rw-r--r--   0        0        0      243 2023-04-21 21:58:08.195713 data_diff-0.7.4/data_diff/databases/oracle.py
--rw-r--r--   0        0        0      275 2023-04-21 21:58:08.195827 data_diff-0.7.4/data_diff/databases/postgresql.py
--rw-r--r--   0        0        0      243 2023-04-21 21:58:08.195918 data_diff-0.7.4/data_diff/databases/presto.py
--rw-r--r--   0        0        0      257 2023-04-21 21:58:08.196013 data_diff-0.7.4/data_diff/databases/redshift.py
--rw-r--r--   0        0        0      264 2023-04-21 21:58:08.196109 data_diff-0.7.4/data_diff/databases/snowflake.py
--rw-r--r--   0        0        0      236 2023-04-21 21:58:08.196196 data_diff-0.7.4/data_diff/databases/trino.py
--rw-r--r--   0        0        0      250 2023-04-21 21:58:08.196288 data_diff-0.7.4/data_diff/databases/vertica.py
--rw-r--r--   0        0        0    13213 2023-04-25 22:24:15.790768 data_diff-0.7.4/data_diff/dbt.py
--rw-r--r--   0        0        0    13945 2023-04-25 22:24:15.790989 data_diff-0.7.4/data_diff/dbt_parser.py
--rw-r--r--   0        0        0    14376 2023-04-21 21:58:08.196773 data_diff-0.7.4/data_diff/diff_tables.py
--rw-r--r--   0        0        0     8567 2023-04-21 21:58:08.196909 data_diff-0.7.4/data_diff/hashdiff_tables.py
--rw-r--r--   0        0        0     1477 2023-04-03 18:06:26.932667 data_diff-0.7.4/data_diff/info_tree.py
--rw-r--r--   0        0        0    14768 2023-04-21 21:58:08.197074 data_diff-0.7.4/data_diff/joindiff_tables.py
--rw-r--r--   0        0        0     7557 2023-04-03 18:06:26.932827 data_diff-0.7.4/data_diff/lexicographic_space.py
--rw-r--r--   0        0        0     1783 2023-04-03 18:06:26.932897 data_diff-0.7.4/data_diff/parse_time.py
--rw-r--r--   0        0        0     1404 2023-04-21 21:58:08.197181 data_diff-0.7.4/data_diff/query_utils.py
--rw-r--r--   0        0        0       76 2023-04-21 21:58:08.197422 data_diff-0.7.4/data_diff/sqeleton/__init__.py
--rw-r--r--   0        0        0      279 2023-04-21 21:58:08.197521 data_diff-0.7.4/data_diff/sqeleton/__main__.py
--rw-r--r--   0        0        0      254 2023-04-21 21:58:08.197672 data_diff-0.7.4/data_diff/sqeleton/abcs/__init__.py
--rw-r--r--   0        0        0      409 2023-04-21 21:58:08.197743 data_diff-0.7.4/data_diff/sqeleton/abcs/compiler.py
--rw-r--r--   0        0        0    10339 2023-04-21 21:58:08.197842 data_diff-0.7.4/data_diff/sqeleton/abcs/database_types.py
--rw-r--r--   0        0        0     5909 2023-04-21 21:58:08.197929 data_diff-0.7.4/data_diff/sqeleton/abcs/mixins.py
--rw-r--r--   0        0        0     2425 2023-04-21 21:58:08.198003 data_diff-0.7.4/data_diff/sqeleton/bound_exprs.py
--rw-r--r--   0        0        0      554 2023-04-21 21:58:08.198154 data_diff-0.7.4/data_diff/sqeleton/databases/__init__.py
--rw-r--r--   0        0        0     9131 2023-04-21 21:58:08.198249 data_diff-0.7.4/data_diff/sqeleton/databases/_connect.py
--rw-r--r--   0        0        0    19920 2023-04-21 21:58:08.198404 data_diff-0.7.4/data_diff/sqeleton/databases/base.py
--rw-r--r--   0        0        0     7140 2023-04-21 21:58:08.198520 data_diff-0.7.4/data_diff/sqeleton/databases/bigquery.py
--rw-r--r--   0        0        0     6642 2023-04-21 21:58:08.198608 data_diff-0.7.4/data_diff/sqeleton/databases/clickhouse.py
--rw-r--r--   0        0        0     6959 2023-04-21 21:58:08.198702 data_diff-0.7.4/data_diff/sqeleton/databases/databricks.py
--rw-r--r--   0        0        0     6093 2023-04-21 21:58:08.198787 data_diff-0.7.4/data_diff/sqeleton/databases/duckdb.py
--rw-r--r--   0        0        0      910 2023-04-21 21:58:08.198859 data_diff-0.7.4/data_diff/sqeleton/databases/mssql.py
--rw-r--r--   0        0        0     4438 2023-04-21 21:58:08.198940 data_diff-0.7.4/data_diff/sqeleton/databases/mysql.py
--rw-r--r--   0        0        0     6523 2023-04-21 21:58:08.199025 data_diff-0.7.4/data_diff/sqeleton/databases/oracle.py
--rw-r--r--   0        0        0     5430 2023-04-21 21:58:08.199106 data_diff-0.7.4/data_diff/sqeleton/databases/postgresql.py
--rw-r--r--   0        0        0     6112 2023-04-21 21:58:08.199200 data_diff-0.7.4/data_diff/sqeleton/databases/presto.py
--rw-r--r--   0        0        0     4844 2023-04-21 21:58:08.199284 data_diff-0.7.4/data_diff/sqeleton/databases/redshift.py
--rw-r--r--   0        0        0     7742 2023-04-21 21:58:08.199375 data_diff-0.7.4/data_diff/sqeleton/databases/snowflake.py
--rw-r--r--   0        0        0     1297 2023-04-21 21:58:08.199477 data_diff-0.7.4/data_diff/sqeleton/databases/trino.py
--rw-r--r--   0        0        0     5426 2023-04-21 21:58:08.199590 data_diff-0.7.4/data_diff/sqeleton/databases/vertica.py
--rw-r--r--   0        0        0      464 2023-04-21 21:58:08.199708 data_diff-0.7.4/data_diff/sqeleton/queries/__init__.py
--rw-r--r--   0        0        0     5291 2023-04-21 21:58:08.199788 data_diff-0.7.4/data_diff/sqeleton/queries/api.py
--rw-r--r--   0        0        0    30646 2023-04-21 21:58:08.199945 data_diff-0.7.4/data_diff/sqeleton/queries/ast_classes.py
--rw-r--r--   0        0        0      367 2023-04-21 21:58:08.200018 data_diff-0.7.4/data_diff/sqeleton/queries/base.py
--rw-r--r--   0        0        0     2605 2023-04-21 21:58:08.200096 data_diff-0.7.4/data_diff/sqeleton/queries/compiler.py
--rw-r--r--   0        0        0     1985 2023-04-21 21:58:08.200163 data_diff-0.7.4/data_diff/sqeleton/queries/extras.py
--rw-r--r--   0        0        0     1404 2023-04-21 21:58:08.200227 data_diff-0.7.4/data_diff/sqeleton/query_utils.py
--rw-r--r--   0        0        0     1981 2023-04-21 21:58:08.200332 data_diff-0.7.4/data_diff/sqeleton/repl.py
--rw-r--r--   0        0        0      737 2023-04-21 21:58:08.200391 data_diff-0.7.4/data_diff/sqeleton/schema.py
--rw-r--r--   0        0        0     8907 2023-04-21 21:58:08.200481 data_diff-0.7.4/data_diff/sqeleton/utils.py
--rw-r--r--   0        0        0    10884 2023-04-21 21:58:08.200617 data_diff-0.7.4/data_diff/table_segment.py
--rw-r--r--   0        0        0     2651 2023-04-03 18:06:26.933183 data_diff-0.7.4/data_diff/thread_utils.py
--rw-r--r--   0        0        0     4121 2023-04-15 23:11:48.035287 data_diff-0.7.4/data_diff/tracking.py
--rw-r--r--   0        0        0     4306 2023-04-14 15:23:33.907379 data_diff-0.7.4/data_diff/utils.py
--rw-r--r--   0        0        0       22 2023-04-25 22:24:15.791131 data_diff-0.7.4/data_diff/version.py
--rwxr-xr-x   0        0        0     2865 2023-04-25 22:24:15.791298 data_diff-0.7.4/pyproject.toml
--rw-r--r--   0        0        0     7387 1970-01-01 00:00:00.000000 data_diff-0.7.4/PKG-INFO
+-rw-r--r--   0        0        0     1053 2023-04-03 18:06:26.931220 data_diff-0.7.5/LICENSE
+-rw-r--r--   0        0        0     2106 2023-05-05 21:08:17.221526 data_diff-0.7.5/README.md
+-rw-r--r--   0        0        0     8429 2023-04-21 21:58:08.193898 data_diff-0.7.5/data_diff/__init__.py
+-rw-r--r--   0        0        0    16024 2023-05-05 21:08:17.222127 data_diff-0.7.5/data_diff/__main__.py
+-rw-r--r--   0        0        0      108 2023-04-14 15:23:33.906548 data_diff-0.7.5/data_diff/cloud/__init__.py
+-rw-r--r--   0        0        0    11594 2023-04-21 21:58:08.194331 data_diff-0.7.5/data_diff/cloud/data_source.py
+-rw-r--r--   0        0        0     9253 2023-04-21 21:58:08.194472 data_diff-0.7.5/data_diff/cloud/datafold_api.py
+-rw-r--r--   0        0        0     4044 2023-04-03 18:06:26.931568 data_diff-0.7.5/data_diff/config.py
+-rw-r--r--   0        0        0      493 2023-04-21 21:58:08.194615 data_diff-0.7.5/data_diff/databases/__init__.py
+-rw-r--r--   0        0        0     1353 2023-04-21 21:58:08.194720 data_diff-0.7.5/data_diff/databases/_connect.py
+-rw-r--r--   0        0        0      174 2023-04-21 21:58:08.194816 data_diff-0.7.5/data_diff/databases/base.py
+-rw-r--r--   0        0        0      257 2023-04-21 21:58:08.195148 data_diff-0.7.5/data_diff/databases/bigquery.py
+-rw-r--r--   0        0        0      271 2023-04-21 21:58:08.195281 data_diff-0.7.5/data_diff/databases/clickhouse.py
+-rw-r--r--   0        0        0      271 2023-04-21 21:58:08.195390 data_diff-0.7.5/data_diff/databases/databricks.py
+-rw-r--r--   0        0        0      243 2023-04-21 21:58:08.195511 data_diff-0.7.5/data_diff/databases/duckdb.py
+-rw-r--r--   0        0        0      236 2023-04-21 21:58:08.195617 data_diff-0.7.5/data_diff/databases/mysql.py
+-rw-r--r--   0        0        0      243 2023-04-21 21:58:08.195713 data_diff-0.7.5/data_diff/databases/oracle.py
+-rw-r--r--   0        0        0      275 2023-04-21 21:58:08.195827 data_diff-0.7.5/data_diff/databases/postgresql.py
+-rw-r--r--   0        0        0      243 2023-04-21 21:58:08.195918 data_diff-0.7.5/data_diff/databases/presto.py
+-rw-r--r--   0        0        0      257 2023-04-21 21:58:08.196013 data_diff-0.7.5/data_diff/databases/redshift.py
+-rw-r--r--   0        0        0      264 2023-04-21 21:58:08.196109 data_diff-0.7.5/data_diff/databases/snowflake.py
+-rw-r--r--   0        0        0      236 2023-04-21 21:58:08.196196 data_diff-0.7.5/data_diff/databases/trino.py
+-rw-r--r--   0        0        0      250 2023-04-21 21:58:08.196288 data_diff-0.7.5/data_diff/databases/vertica.py
+-rw-r--r--   0        0        0    12878 2023-05-05 21:08:17.222295 data_diff-0.7.5/data_diff/dbt.py
+-rw-r--r--   0        0        0    16856 2023-05-05 21:08:17.222470 data_diff-0.7.5/data_diff/dbt_parser.py
+-rw-r--r--   0        0        0    14376 2023-04-21 21:58:08.196773 data_diff-0.7.5/data_diff/diff_tables.py
+-rw-r--r--   0        0        0     9333 2023-05-05 21:08:17.222755 data_diff-0.7.5/data_diff/hashdiff_tables.py
+-rw-r--r--   0        0        0     1477 2023-04-03 18:06:26.932667 data_diff-0.7.5/data_diff/info_tree.py
+-rw-r--r--   0        0        0    14768 2023-04-21 21:58:08.197074 data_diff-0.7.5/data_diff/joindiff_tables.py
+-rw-r--r--   0        0        0     7557 2023-04-03 18:06:26.932827 data_diff-0.7.5/data_diff/lexicographic_space.py
+-rw-r--r--   0        0        0     1783 2023-04-03 18:06:26.932897 data_diff-0.7.5/data_diff/parse_time.py
+-rw-r--r--   0        0        0     1404 2023-04-21 21:58:08.197181 data_diff-0.7.5/data_diff/query_utils.py
+-rw-r--r--   0        0        0       76 2023-04-21 21:58:08.197422 data_diff-0.7.5/data_diff/sqeleton/__init__.py
+-rw-r--r--   0        0        0      279 2023-04-21 21:58:08.197521 data_diff-0.7.5/data_diff/sqeleton/__main__.py
+-rw-r--r--   0        0        0      264 2023-05-05 21:08:17.222879 data_diff-0.7.5/data_diff/sqeleton/abcs/__init__.py
+-rw-r--r--   0        0        0      409 2023-04-21 21:58:08.197743 data_diff-0.7.5/data_diff/sqeleton/abcs/compiler.py
+-rw-r--r--   0        0        0    11118 2023-05-05 21:08:17.223038 data_diff-0.7.5/data_diff/sqeleton/abcs/database_types.py
+-rw-r--r--   0        0        0     6989 2023-05-05 21:08:17.223166 data_diff-0.7.5/data_diff/sqeleton/abcs/mixins.py
+-rw-r--r--   0        0        0     2425 2023-04-21 21:58:08.198003 data_diff-0.7.5/data_diff/sqeleton/bound_exprs.py
+-rw-r--r--   0        0        0      554 2023-04-21 21:58:08.198154 data_diff-0.7.5/data_diff/sqeleton/databases/__init__.py
+-rw-r--r--   0        0        0     9131 2023-04-21 21:58:08.198249 data_diff-0.7.5/data_diff/sqeleton/databases/_connect.py
+-rw-r--r--   0        0        0    20130 2023-05-05 21:08:17.223365 data_diff-0.7.5/data_diff/sqeleton/databases/base.py
+-rw-r--r--   0        0        0    10135 2023-05-05 21:08:17.223531 data_diff-0.7.5/data_diff/sqeleton/databases/bigquery.py
+-rw-r--r--   0        0        0     6642 2023-04-21 21:58:08.198608 data_diff-0.7.5/data_diff/sqeleton/databases/clickhouse.py
+-rw-r--r--   0        0        0     6959 2023-04-21 21:58:08.198702 data_diff-0.7.5/data_diff/sqeleton/databases/databricks.py
+-rw-r--r--   0        0        0     6093 2023-04-21 21:58:08.198787 data_diff-0.7.5/data_diff/sqeleton/databases/duckdb.py
+-rw-r--r--   0        0        0      910 2023-04-21 21:58:08.198859 data_diff-0.7.5/data_diff/sqeleton/databases/mssql.py
+-rw-r--r--   0        0        0     4438 2023-04-21 21:58:08.198940 data_diff-0.7.5/data_diff/sqeleton/databases/mysql.py
+-rw-r--r--   0        0        0     6550 2023-05-05 21:08:17.223666 data_diff-0.7.5/data_diff/sqeleton/databases/oracle.py
+-rw-r--r--   0        0        0     5551 2023-05-05 21:08:17.223788 data_diff-0.7.5/data_diff/sqeleton/databases/postgresql.py
+-rw-r--r--   0        0        0     6112 2023-04-21 21:58:08.199200 data_diff-0.7.5/data_diff/sqeleton/databases/presto.py
+-rw-r--r--   0        0        0     6312 2023-05-05 21:08:17.223928 data_diff-0.7.5/data_diff/sqeleton/databases/redshift.py
+-rw-r--r--   0        0        0     7742 2023-04-21 21:58:08.199375 data_diff-0.7.5/data_diff/sqeleton/databases/snowflake.py
+-rw-r--r--   0        0        0     1297 2023-04-21 21:58:08.199477 data_diff-0.7.5/data_diff/sqeleton/databases/trino.py
+-rw-r--r--   0        0        0     5426 2023-04-21 21:58:08.199590 data_diff-0.7.5/data_diff/sqeleton/databases/vertica.py
+-rw-r--r--   0        0        0      464 2023-04-21 21:58:08.199708 data_diff-0.7.5/data_diff/sqeleton/queries/__init__.py
+-rw-r--r--   0        0        0     5291 2023-04-21 21:58:08.199788 data_diff-0.7.5/data_diff/sqeleton/queries/api.py
+-rw-r--r--   0        0        0    30750 2023-05-05 21:08:17.224381 data_diff-0.7.5/data_diff/sqeleton/queries/ast_classes.py
+-rw-r--r--   0        0        0      367 2023-04-21 21:58:08.200018 data_diff-0.7.5/data_diff/sqeleton/queries/base.py
+-rw-r--r--   0        0        0     2605 2023-04-21 21:58:08.200096 data_diff-0.7.5/data_diff/sqeleton/queries/compiler.py
+-rw-r--r--   0        0        0     1985 2023-04-21 21:58:08.200163 data_diff-0.7.5/data_diff/sqeleton/queries/extras.py
+-rw-r--r--   0        0        0     1404 2023-04-21 21:58:08.200227 data_diff-0.7.5/data_diff/sqeleton/query_utils.py
+-rw-r--r--   0        0        0     1981 2023-04-21 21:58:08.200332 data_diff-0.7.5/data_diff/sqeleton/repl.py
+-rw-r--r--   0        0        0      737 2023-04-21 21:58:08.200391 data_diff-0.7.5/data_diff/sqeleton/schema.py
+-rw-r--r--   0        0        0     8907 2023-04-21 21:58:08.200481 data_diff-0.7.5/data_diff/sqeleton/utils.py
+-rw-r--r--   0        0        0    10884 2023-04-21 21:58:08.200617 data_diff-0.7.5/data_diff/table_segment.py
+-rw-r--r--   0        0        0     2651 2023-04-03 18:06:26.933183 data_diff-0.7.5/data_diff/thread_utils.py
+-rw-r--r--   0        0        0     4121 2023-04-15 23:11:48.035287 data_diff-0.7.5/data_diff/tracking.py
+-rw-r--r--   0        0        0     5247 2023-05-05 21:08:17.224565 data_diff-0.7.5/data_diff/utils.py
+-rw-r--r--   0        0        0       22 2023-05-05 21:08:17.224662 data_diff-0.7.5/data_diff/version.py
+-rwxr-xr-x   0        0        0     2865 2023-05-05 21:08:17.225592 data_diff-0.7.5/pyproject.toml
+-rw-r--r--   0        0        0     4720 1970-01-01 00:00:00.000000 data_diff-0.7.5/PKG-INFO
```

### Comparing `data_diff-0.7.4/LICENSE` & `data_diff-0.7.5/LICENSE`

 * *Files identical despite different names*

### Comparing `data_diff-0.7.4/data_diff/__init__.py` & `data_diff-0.7.5/data_diff/__init__.py`

 * *Files identical despite different names*

### Comparing `data_diff-0.7.4/data_diff/__main__.py` & `data_diff-0.7.5/data_diff/__main__.py`

 * *Files 2% similar despite different names*

```diff
@@ -224,14 +224,21 @@
 )
 @click.option(
     "--dbt-project-dir",
     default=None,
     metavar="PATH",
     help="Which directory to look in for the dbt_project.yml file. Default is the current working directory and its parents.",
 )
+@click.option(
+    "--select",
+    "-s",
+    default=None,
+    metavar="PATH",
+    help="select dbt resources to compare using dbt selection syntax",
+)
 def main(conf, run, **kw):
     if kw["table2"] is None and kw["database2"]:
         # Use the "database table table" form
         kw["table2"] = kw["database2"]
         kw["database2"] = kw["database1"]
 
     if kw["version"]:
@@ -260,14 +267,15 @@
 
     try:
         if kw["dbt"]:
             dbt_diff(
                 profiles_dir_override=kw["dbt_profiles_dir"],
                 project_dir_override=kw["dbt_project_dir"],
                 is_cloud=kw["cloud"],
+                dbt_selection=kw["select"],
             )
         else:
             return _data_diff(**kw)
     except Exception as e:
         logging.error(e)
         if kw["debug"]:
             raise
@@ -302,14 +310,15 @@
     materialize_all_rows,
     table_write_limit,
     materialize_to_table,
     dbt,
     cloud,
     dbt_profiles_dir,
     dbt_project_dir,
+    select,
     threads1=None,
     threads2=None,
     __conf__=None,
 ):
     if limit and stats:
         logging.error("Cannot specify a limit when using the -s/--stats switch")
         return
```

### Comparing `data_diff-0.7.4/data_diff/cloud/data_source.py` & `data_diff-0.7.5/data_diff/cloud/data_source.py`

 * *Files identical despite different names*

### Comparing `data_diff-0.7.4/data_diff/cloud/datafold_api.py` & `data_diff-0.7.5/data_diff/cloud/datafold_api.py`

 * *Files identical despite different names*

### Comparing `data_diff-0.7.4/data_diff/config.py` & `data_diff-0.7.5/data_diff/config.py`

 * *Files identical despite different names*

### Comparing `data_diff-0.7.4/data_diff/databases/_connect.py` & `data_diff-0.7.5/data_diff/databases/_connect.py`

 * *Files identical despite different names*

### Comparing `data_diff-0.7.4/data_diff/dbt.py` & `data_diff-0.7.5/data_diff/dbt.py`

 * *Files 2% similar despite different names*

```diff
@@ -14,25 +14,14 @@
 from .cloud import DatafoldAPI, TCloudApiDataDiff, get_or_create_data_source
 from .dbt_parser import DbtParser, PROJECT_FILE
 
 
 logger = getLogger(__name__)
 
 
-def import_dbt():
-    try:
-        from dbt_artifacts_parser.parser import parse_run_results, parse_manifest
-        from dbt.config.renderer import ProfileRenderer
-        import yaml
-    except ImportError:
-        raise RuntimeError("Could not import 'dbt' package. You can install it using: pip install 'data-diff[dbt]'.")
-
-    return parse_run_results, parse_manifest, ProfileRenderer, yaml
-
-
 from .tracking import (
     set_entrypoint_name,
     set_dbt_user_id,
     set_dbt_version,
     set_dbt_project_id,
     create_end_event_json,
     create_start_event_json,
@@ -50,20 +39,23 @@
     primary_keys: List[str]
     connection: Dict[str, str]
     threads: Optional[int]
     where_filter: Optional[str] = None
 
 
 def dbt_diff(
-    profiles_dir_override: Optional[str] = None, project_dir_override: Optional[str] = None, is_cloud: bool = False
+    profiles_dir_override: Optional[str] = None,
+    project_dir_override: Optional[str] = None,
+    is_cloud: bool = False,
+    dbt_selection: Optional[str] = None,
 ) -> None:
     diff_threads = []
     set_entrypoint_name("CLI-dbt")
     dbt_parser = DbtParser(profiles_dir_override, project_dir_override)
-    models = dbt_parser.get_models()
+    models = dbt_parser.get_models(dbt_selection)
     datadiff_variables = dbt_parser.get_datadiff_variables()
     config_prod_database = datadiff_variables.get("prod_database")
     config_prod_schema = datadiff_variables.get("prod_schema")
     config_prod_custom_schema = datadiff_variables.get("prod_custom_schema")
     datasource_id = datadiff_variables.get("datasource_id")
     set_dbt_user_id(dbt_parser.dbt_user_id)
     set_dbt_version(dbt_parser.dbt_version)
```

### Comparing `data_diff-0.7.4/data_diff/dbt_parser.py` & `data_diff-0.7.5/data_diff/dbt_parser.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,38 +1,59 @@
+from argparse import Namespace
 from collections import defaultdict
 import json
+import os
 from pathlib import Path
-from typing import List, Dict, Tuple, Set
+from typing import List, Dict, Tuple, Set, Optional
 
 from packaging.version import parse as parse_version
 
 from .utils import getLogger, get_from_dict_with_raise
 from .version import __version__
 
 
 logger = getLogger(__name__)
 
 
-def import_dbt():
+def import_dbt_dependencies():
     try:
         from dbt_artifacts_parser.parser import parse_run_results, parse_manifest
         from dbt.config.renderer import ProfileRenderer
         import yaml
     except ImportError:
         raise RuntimeError("Could not import 'dbt' package. You can install it using: pip install 'data-diff[dbt]'.")
 
-    return parse_run_results, parse_manifest, ProfileRenderer, yaml
+    # dbt 1.5+ specific stuff to power selection of models
+    try:
+        # ProfileRenderer.render_data() fails without instantiating global flag MACRO_DEBUGGING in dbt-core 1.5
+        from dbt.flags import set_flags
+
+        set_flags(Namespace(MACRO_DEBUGGING=False))
+    except:
+        pass
+
+    try:
+        from dbt.cli.main import dbtRunner
+    except ImportError:
+        dbtRunner = None
+
+    if dbtRunner is not None:
+        dbt_runner = dbtRunner()
+    else:
+        dbt_runner = None
+
+    return parse_run_results, parse_manifest, ProfileRenderer, yaml, dbt_runner
 
 
 RUN_RESULTS_PATH = "target/run_results.json"
 MANIFEST_PATH = "target/manifest.json"
 PROJECT_FILE = "dbt_project.yml"
 PROFILES_FILE = "profiles.yml"
 LOWER_DBT_V = "1.0.0"
-UPPER_DBT_V = "1.4.7"
+UPPER_DBT_V = "1.6.0"
 
 
 # https://github.com/dbt-labs/dbt-core/blob/c952d44ec5c2506995fbad75320acbae49125d3d/core/dbt/cli/resolvers.py#L6
 def default_project_dir() -> Path:
     paths = list(Path.cwd().parents)
     paths.insert(0, Path.cwd())
     return next((x for x in paths if (x / PROJECT_FILE).exists()), Path.cwd())
@@ -45,15 +66,21 @@
 
 def legacy_profiles_dir() -> Path:
     return Path.home() / ".dbt"
 
 
 class DbtParser:
     def __init__(self, profiles_dir_override: str, project_dir_override: str) -> None:
-        self.parse_run_results, self.parse_manifest, self.ProfileRenderer, self.yaml = import_dbt()
+        (
+            self.parse_run_results,
+            self.parse_manifest,
+            self.ProfileRenderer,
+            self.yaml,
+            self.dbt_runner,
+        ) = import_dbt_dependencies()
         self.profiles_dir = Path(profiles_dir_override or default_profiles_dir())
         self.project_dir = Path(project_dir_override or default_project_dir())
         self.connection = None
         self.project_dict = self.get_project_dict()
         self.manifest_obj = self.get_manifest_obj()
         self.dbt_user_id = self.manifest_obj.metadata.user_id
         self.dbt_version = self.manifest_obj.metadata.dbt_version
@@ -64,31 +91,83 @@
 
     def get_datadiff_variables(self) -> dict:
         doc_url = "https://docs.datafold.com/development_testing/open_source#configure-your-dbt-project"
         error_message = f"vars: data_diff: section not found in dbt_project.yml.\n\nTo solve this, please configure your dbt project: \n{doc_url}\n"
         vars = get_from_dict_with_raise(self.project_dict, "vars", error_message)
         return get_from_dict_with_raise(vars, "data_diff", error_message)
 
-    def get_models(self):
+    def get_models(self, dbt_selection: Optional[str] = None):
+        dbt_version = parse_version(self.dbt_version)
+        if dbt_selection:
+            if (dbt_version.major, dbt_version.minor) >= (1, 5):
+                if self.dbt_runner:
+                    return self.get_dbt_selection_models(dbt_selection)
+                # edge case if running data-diff from a separate env than dbt (likely local development)
+                else:
+                    raise Exception(
+                        "data-diff is using a dbt-core version < 1.5, update the environment's dbt-core version via pip install 'dbt-core>=1.5' in order to use `--select`"
+                    )
+            else:
+                raise Exception(
+                    f"Use of the `--select` feature requires dbt >= 1.5. Found dbt manifest: v{dbt_version}"
+                )
+        else:
+            return self.get_run_results_models()
+
+    def get_dbt_selection_models(self, dbt_selection: str) -> List[str]:
+        # log level and format settings needed to prevent dbt from printing to stdout
+        # ls command is used to get the list of model unique_ids
+        results = self.dbt_runner.invoke(
+            [
+                "--log-format",
+                "json",
+                "--log-level",
+                "none",
+                "ls",
+                "--select",
+                dbt_selection,
+                "--resource-type",
+                "model",
+                "--output",
+                "json",
+                "--output-keys",
+                "unique_id",
+                "--project-dir",
+                self.project_dir,
+            ]
+        )
+        if results.exception:
+            raise results.exception
+        elif results.success and results.result:
+            model_list = [json.loads(model)["unique_id"] for model in results.result]
+            models = [self.manifest_obj.nodes.get(x) for x in model_list]
+            return models
+        elif not results.result:
+            raise Exception(f"No dbt models found for `--select {dbt_selection}`")
+        else:
+            logger.debug(str(results))
+            raise Exception("Encountered an unexpected error while finding `--select` models")
+
+    def get_run_results_models(self):
         with open(self.project_dir / RUN_RESULTS_PATH) as run_results:
             logger.info(f"Parsing file {RUN_RESULTS_PATH}")
             run_results_dict = json.load(run_results)
             run_results_obj = self.parse_run_results(run_results=run_results_dict)
 
         dbt_version = parse_version(run_results_obj.metadata.dbt_version)
 
         if dbt_version < parse_version("1.3.0"):
             self.profiles_dir = legacy_profiles_dir()
 
         if dbt_version < parse_version(LOWER_DBT_V):
-            raise Exception(
-                f"Found dbt: v{dbt_version} Expected the dbt project's version to be >= {LOWER_DBT_V}"
-            )
+            raise Exception(f"Found dbt: v{dbt_version} Expected the dbt project's version to be >= {LOWER_DBT_V}")
         elif dbt_version >= parse_version(UPPER_DBT_V):
-            logger.warning(f"{dbt_version} is a recent version of dbt and may not be fully tested with data-diff! \nPlease report any issues to https://github.com/datafold/data-diff/issues")
+            logger.warning(
+                f"{dbt_version} is a recent version of dbt and may not be fully tested with data-diff! \nPlease report any issues to https://github.com/datafold/data-diff/issues"
+            )
 
         success_models = [x.unique_id for x in run_results_obj.results if x.status.name == "success"]
         models = [self.manifest_obj.nodes.get(x) for x in success_models]
         if not models:
             raise ValueError("Expected > 0 successful models runs from the last dbt command.")
 
         print(f"Running with data-diff={__version__}\n")
```

### Comparing `data_diff-0.7.4/data_diff/diff_tables.py` & `data_diff-0.7.5/data_diff/diff_tables.py`

 * *Files identical despite different names*

### Comparing `data_diff-0.7.4/data_diff/hashdiff_tables.py` & `data_diff-0.7.5/data_diff/hashdiff_tables.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,46 +3,56 @@
 import logging
 from collections import defaultdict
 from typing import Iterator
 from operator import attrgetter
 
 from runtype import dataclass
 
-from data_diff.sqeleton.abcs import ColType_UUID, NumericType, PrecisionType, StringType, Boolean
+from data_diff.sqeleton.abcs import ColType_UUID, NumericType, PrecisionType, StringType, Boolean, JSON
 
 from .info_tree import InfoTree
-from .utils import safezip
+from .utils import safezip, diffs_are_equiv_jsons
 from .thread_utils import ThreadedYielder
 from .table_segment import TableSegment
 
 from .diff_tables import TableDiffer
 
 BENCHMARK = os.environ.get("BENCHMARK", False)
 
 DEFAULT_BISECTION_THRESHOLD = 1024 * 16
 DEFAULT_BISECTION_FACTOR = 32
 
 logger = logging.getLogger("hashdiff_tables")
 
 
-def diff_sets(a: set, b: set) -> Iterator:
+def diff_sets(a: list, b: list, json_cols: dict = None) -> Iterator:
     sa = set(a)
     sb = set(b)
 
     # The first item is always the key (see TableDiffer.relevant_columns)
     # TODO update when we add compound keys to hashdiff
     d = defaultdict(list)
     for row in a:
         if row not in sb:
             d[row[0]].append(("-", row))
     for row in b:
         if row not in sa:
             d[row[0]].append(("+", row))
 
+    warned_diff_cols = set()
     for _k, v in sorted(d.items(), key=lambda i: i[0]):
+        if json_cols:
+            parsed_match, overriden_diff_cols = diffs_are_equiv_jsons(v, json_cols)
+            if parsed_match:
+                to_warn = overriden_diff_cols - warned_diff_cols
+                for w in to_warn:
+                    logger.warning(f"Equivalent JSON objects with different string representations detected "
+                                   f"in column '{w}'. These cases are NOT reported as differences.")
+                    warned_diff_cols.add(w)
+                continue
         yield from v
 
 
 @dataclass
 class HashDiffer(TableDiffer):
     """Finds the diff between two SQL tables
 
@@ -190,15 +200,17 @@
             max_rows = max_space_size
             info_tree.info.max_rows = max_rows
 
         # If count is below the threshold, just download and compare the columns locally
         # This saves time, as bisection speed is limited by ping and query performance.
         if max_rows < self.bisection_threshold or max_space_size < self.bisection_factor * 2:
             rows1, rows2 = self._threaded_call("get_values", [table1, table2])
-            diff = list(diff_sets(rows1, rows2))
+            json_cols = {i: colname for i, colname in enumerate(table1.extra_columns)
+                         if isinstance(table1._schema[colname], JSON)}
+            diff = list(diff_sets(rows1, rows2, json_cols))
 
             info_tree.info.set_diff(diff)
             info_tree.info.rowcounts = {1: len(rows1), 2: len(rows2)}
 
             logger.info(". " * level + f"Diff found {len(diff)} different rows.")
             self.stats["rows_downloaded"] = self.stats.get("rows_downloaded", 0) + max(len(rows1), len(rows2))
             return diff
```

### Comparing `data_diff-0.7.4/data_diff/info_tree.py` & `data_diff-0.7.5/data_diff/info_tree.py`

 * *Files identical despite different names*

### Comparing `data_diff-0.7.4/data_diff/joindiff_tables.py` & `data_diff-0.7.5/data_diff/joindiff_tables.py`

 * *Files identical despite different names*

### Comparing `data_diff-0.7.4/data_diff/lexicographic_space.py` & `data_diff-0.7.5/data_diff/lexicographic_space.py`

 * *Files identical despite different names*

### Comparing `data_diff-0.7.4/data_diff/parse_time.py` & `data_diff-0.7.5/data_diff/parse_time.py`

 * *Files identical despite different names*

### Comparing `data_diff-0.7.4/data_diff/query_utils.py` & `data_diff-0.7.5/data_diff/query_utils.py`

 * *Files identical despite different names*

### Comparing `data_diff-0.7.4/data_diff/sqeleton/abcs/database_types.py` & `data_diff-0.7.5/data_diff/sqeleton/abcs/database_types.py`

 * *Files 10% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 
 
 DbPath = Tuple[str, ...]
 DbKey = Union[int, str, bytes, ArithUUID, ArithAlphanumeric]
 DbTime = datetime
 
 
+@dataclass
 class ColType:
     supported = True
 
 
 @dataclass
 class PrecisionType(ColType):
     precision: int
@@ -130,14 +131,35 @@
 
 
 @dataclass
 class Text(StringType):
     supported = False
 
 
+# In majority of DBMSes, it is called JSON/JSONB. Only in Snowflake, it is OBJECT.
+@dataclass
+class JSON(ColType):
+    pass
+
+
+@dataclass
+class Array(ColType):
+    item_type: ColType
+
+
+# Unlike JSON, structs are not free-form and have a very specific set of fields and their types.
+# We do not parse & use those fields now, but we can do this later.
+# For example, in BigQuery:
+# - https://cloud.google.com/bigquery/docs/reference/standard-sql/data-types#struct_type
+# - https://cloud.google.com/bigquery/docs/reference/standard-sql/lexical#struct_literals
+@dataclass
+class Struct(ColType):
+    pass
+
+
 @dataclass
 class Integer(NumericType, IKey):
     precision: int = 0
     python_type: type = int
 
     def __post_init__(self):
         assert self.precision == 0
@@ -217,14 +239,18 @@
         type_repr: str,
         datetime_precision: int = None,
         numeric_precision: int = None,
         numeric_scale: int = None,
     ) -> ColType:
         "Parse type info as returned by the database"
 
+    @abstractmethod
+    def to_comparable(self, value: str, coltype: ColType) -> str:
+        """Ensure that the expression is comparable in ``IS DISTINCT FROM``."""
+
 
 from typing import TypeVar, Generic
 
 T_Dialect = TypeVar("T_Dialect", bound=AbstractDialect)
 
 
 class AbstractDatabase(Generic[T_Dialect]):
```

### Comparing `data_diff-0.7.4/data_diff/sqeleton/abcs/mixins.py` & `data_diff-0.7.5/data_diff/sqeleton/abcs/mixins.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,17 +1,22 @@
 from abc import ABC, abstractmethod
-from .database_types import TemporalType, FractionalType, ColType_UUID, Boolean, ColType, String_UUID
+from .database_types import Array, TemporalType, FractionalType, ColType_UUID, Boolean, ColType, String_UUID, JSON, Struct
 from .compiler import Compilable
 
 
 class AbstractMixin(ABC):
     "A mixin for a database dialect"
 
 
 class AbstractMixin_NormalizeValue(AbstractMixin):
+
+    @abstractmethod
+    def to_comparable(self, value: str, coltype: ColType) -> str:
+        """Ensure that the expression is comparable in ``IS DISTINCT FROM``."""
+
     @abstractmethod
     def normalize_timestamp(self, value: str, coltype: TemporalType) -> str:
         """Creates an SQL expression, that converts 'value' to a normalized timestamp.
 
         The returned expression must accept any SQL datetime/timestamp, and return a string.
 
         Date format: ``YYYY-MM-DD HH:mm:SS.FFFFFF``
@@ -45,14 +50,26 @@
 
     def normalize_uuid(self, value: str, coltype: ColType_UUID) -> str:
         """Creates an SQL expression, that strips uuids of artifacts like whitespace."""
         if isinstance(coltype, String_UUID):
             return f"TRIM({value})"
         return self.to_string(value)
 
+    def normalize_json(self, value: str, _coltype: JSON) -> str:
+        """Creates an SQL expression, that converts 'value' to its minified json string representation."""
+        return self.to_string(value)
+
+    def normalize_array(self, value: str, _coltype: Array) -> str:
+        """Creates an SQL expression, that serialized an array into a JSON string."""
+        return self.to_string(value)
+
+    def normalize_struct(self, value: str, _coltype: Struct) -> str:
+        """Creates an SQL expression, that serialized a typed struct into a JSON string."""
+        return self.to_string(value)
+
     def normalize_value_by_type(self, value: str, coltype: ColType) -> str:
         """Creates an SQL expression, that converts 'value' to a normalized representation.
 
         The returned expression must accept any SQL value, and return a string.
 
         The default implementation dispatches to a method according to `coltype`:
 
@@ -69,14 +86,20 @@
             return self.normalize_timestamp(value, coltype)
         elif isinstance(coltype, FractionalType):
             return self.normalize_number(value, coltype)
         elif isinstance(coltype, ColType_UUID):
             return self.normalize_uuid(value, coltype)
         elif isinstance(coltype, Boolean):
             return self.normalize_boolean(value, coltype)
+        elif isinstance(coltype, JSON):
+            return self.normalize_json(value, coltype)
+        elif isinstance(coltype, Array):
+            return self.normalize_array(value, coltype)
+        elif isinstance(coltype, Struct):
+            return self.normalize_struct(value, coltype)
         return self.to_string(value)
 
 
 class AbstractMixin_MD5(AbstractMixin):
     """Methods for calculating an MD6 hash as an integer."""
 
     @abstractmethod
```

### Comparing `data_diff-0.7.4/data_diff/sqeleton/bound_exprs.py` & `data_diff-0.7.5/data_diff/sqeleton/bound_exprs.py`

 * *Files identical despite different names*

### Comparing `data_diff-0.7.4/data_diff/sqeleton/databases/__init__.py` & `data_diff-0.7.5/data_diff/sqeleton/databases/__init__.py`

 * *Files identical despite different names*

### Comparing `data_diff-0.7.4/data_diff/sqeleton/databases/_connect.py` & `data_diff-0.7.5/data_diff/sqeleton/databases/_connect.py`

 * *Files identical despite different names*

### Comparing `data_diff-0.7.4/data_diff/sqeleton/databases/base.py` & `data_diff-0.7.5/data_diff/sqeleton/databases/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -13,15 +13,16 @@
 from runtype import dataclass
 
 from ..utils import is_uuid, safezip, Self
 from ..queries import Expr, Compiler, table, Select, SKIP, Explain, Code, this
 from ..queries.ast_classes import Random
 from ..abcs.database_types import (
     AbstractDatabase,
-    T_Dialect,
+    Array,
+    Struct,
     AbstractDialect,
     AbstractTable,
     ColType,
     Integer,
     Decimal,
     Float,
     Native_UUID,
@@ -31,14 +32,15 @@
     TemporalType,
     UnknownColType,
     TimestampTZ,
     Text,
     DbTime,
     DbPath,
     Boolean,
+    JSON
 )
 from ..abcs.mixins import Compilable
 from ..abcs.mixins import (
     AbstractMixin_Schema,
     AbstractMixin_RandomSample,
     AbstractMixin_NormalizeValue,
     AbstractMixin_OptimizerHints,
@@ -160,14 +162,18 @@
         return f"LIMIT {limit}"
 
     def concat(self, items: List[str]) -> str:
         assert len(items) > 1
         joined_exprs = ", ".join(items)
         return f"concat({joined_exprs})"
 
+    def to_comparable(self, value: str, coltype: ColType) -> str:
+        """Ensure that the expression is comparable in ``IS DISTINCT FROM``."""
+        return value
+
     def is_distinct_from(self, a: str, b: str) -> str:
         return f"{a} is distinct from {b}"
 
     def timestamp_value(self, t: DbTime) -> str:
         return f"'{t.isoformat()}'"
 
     def random(self) -> str:
@@ -224,15 +230,15 @@
         datetime_precision: int = None,
         numeric_precision: int = None,
         numeric_scale: int = None,
     ) -> ColType:
         """ """
 
         cls = self._parse_type_repr(type_repr)
-        if not cls:
+        if cls is None:
             return UnknownColType(type_repr)
 
         if issubclass(cls, TemporalType):
             return cls(
                 precision=datetime_precision if datetime_precision is not None else DEFAULT_DATETIME_PRECISION,
                 rounds=self.ROUNDS_ON_PREC_LOSS,
             )
@@ -252,15 +258,15 @@
             # assert numeric_scale is None
             return cls(
                 precision=self._convert_db_precision_to_digits(
                     numeric_precision if numeric_precision is not None else DEFAULT_NUMERIC_PRECISION
                 )
             )
 
-        elif issubclass(cls, (Text, Native_UUID)):
+        elif issubclass(cls, (JSON, Array, Struct, Text, Native_UUID)):
             return cls()
 
         raise TypeError(f"Parsing {type_repr} returned an unknown type '{cls}'.")
 
     def _convert_db_precision_to_digits(self, p: int) -> int:
         """Convert from binary precision, used by floats, to decimal precision."""
         # See: https://en.wikipedia.org/wiki/Single-precision_floating-point_format
```

### Comparing `data_diff-0.7.4/data_diff/sqeleton/databases/bigquery.py` & `data_diff-0.7.5/data_diff/sqeleton/databases/snowflake.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,213 +1,228 @@
-from typing import List, Union
+from typing import Union, List
+import logging
+
 from ..abcs.database_types import (
     Timestamp,
-    Datetime,
-    Integer,
+    TimestampTZ,
     Decimal,
     Float,
     Text,
-    DbPath,
     FractionalType,
     TemporalType,
+    DbPath,
     Boolean,
+    Date,
 )
 from ..abcs.mixins import (
     AbstractMixin_MD5,
     AbstractMixin_NormalizeValue,
     AbstractMixin_Schema,
     AbstractMixin_TimeTravel,
 )
 from ..abcs import Compilable
-from ..queries import this, table, SKIP, code
-from .base import BaseDialect, Database, import_helper, parse_table_name, ConnectError, apply_query, QueryResult
-from .base import TIMESTAMP_PRECISION_POS, ThreadLocalInterpreter, Mixin_RandomSample
+from data_diff.sqeleton.queries import table, this, SKIP, code
+from .base import (
+    BaseDialect,
+    ConnectError,
+    Database,
+    import_helper,
+    CHECKSUM_MASK,
+    ThreadLocalInterpreter,
+    Mixin_RandomSample,
+)
 
 
-@import_helper(text="Please install BigQuery and configure your google-cloud access.")
-def import_bigquery():
-    from google.cloud import bigquery
+@import_helper("snowflake")
+def import_snowflake():
+    import snowflake.connector
+    from cryptography.hazmat.primitives import serialization
+    from cryptography.hazmat.backends import default_backend
 
-    return bigquery
+    return snowflake, serialization, default_backend
 
 
 class Mixin_MD5(AbstractMixin_MD5):
     def md5_as_int(self, s: str) -> str:
-        return f"cast(cast( ('0x' || substr(TO_HEX(md5({s})), 18)) as int64) as numeric)"
+        return f"BITAND(md5_number_lower64({s}), {CHECKSUM_MASK})"
 
 
 class Mixin_NormalizeValue(AbstractMixin_NormalizeValue):
     def normalize_timestamp(self, value: str, coltype: TemporalType) -> str:
         if coltype.rounds:
-            timestamp = f"timestamp_micros(cast(round(unix_micros(cast({value} as timestamp))/1000000, {coltype.precision})*1000000 as int))"
-            return f"FORMAT_TIMESTAMP('%F %H:%M:%E6S', {timestamp})"
-
-        if coltype.precision == 0:
-            return f"FORMAT_TIMESTAMP('%F %H:%M:%S.000000', {value})"
-        elif coltype.precision == 6:
-            return f"FORMAT_TIMESTAMP('%F %H:%M:%E6S', {value})"
+            timestamp = f"to_timestamp(round(date_part(epoch_nanosecond, convert_timezone('UTC', {value})::timestamp(9))/1000000000, {coltype.precision}))"
+        else:
+            timestamp = f"cast(convert_timezone('UTC', {value}) as timestamp({coltype.precision}))"
 
-        timestamp6 = f"FORMAT_TIMESTAMP('%F %H:%M:%E6S', {value})"
-        return (
-            f"RPAD(LEFT({timestamp6}, {TIMESTAMP_PRECISION_POS+coltype.precision}), {TIMESTAMP_PRECISION_POS+6}, '0')"
-        )
+        return f"to_char({timestamp}, 'YYYY-MM-DD HH24:MI:SS.FF6')"
 
     def normalize_number(self, value: str, coltype: FractionalType) -> str:
-        return f"format('%.{coltype.precision}f', {value})"
+        return self.to_string(f"cast({value} as decimal(38, {coltype.precision}))")
 
     def normalize_boolean(self, value: str, _coltype: Boolean) -> str:
-        return self.to_string(f"cast({value} as int)")
+        return self.to_string(f"{value}::int")
 
 
 class Mixin_Schema(AbstractMixin_Schema):
+    def table_information(self) -> Compilable:
+        return table("INFORMATION_SCHEMA", "TABLES")
+
     def list_tables(self, table_schema: str, like: Compilable = None) -> Compilable:
         return (
-            table(table_schema, "INFORMATION_SCHEMA", "TABLES")
+            self.table_information()
             .where(
-                this.table_schema == table_schema,
-                this.table_name.like(like) if like is not None else SKIP,
-                this.table_type == "BASE TABLE",
+                this.TABLE_SCHEMA == table_schema,
+                this.TABLE_NAME.like(like) if like is not None else SKIP,
+                this.TABLE_TYPE == "BASE TABLE",
             )
-            .select(this.table_name)
+            .select(table_name=this.TABLE_NAME)
         )
 
 
 class Mixin_TimeTravel(AbstractMixin_TimeTravel):
     def time_travel(
         self,
         table: Compilable,
         before: bool = False,
         timestamp: Compilable = None,
         offset: Compilable = None,
         statement: Compilable = None,
     ) -> Compilable:
-        if before:
-            raise NotImplementedError("before=True not supported for BigQuery time-travel")
-
-        if statement is not None:
-            raise NotImplementedError("BigQuery time-travel doesn't support querying by statement id")
-
+        at_or_before = "AT" if before else "BEFORE"
         if timestamp is not None:
-            assert offset is None
-            return code("{table} FOR SYSTEM_TIME AS OF {timestamp}", table=table, timestamp=timestamp)
+            assert offset is None and statement is None
+            key = "timestamp"
+            value = timestamp
+        elif offset is not None:
+            assert statement is None
+            key = "offset"
+            value = offset
+        else:
+            assert statement is not None
+            key = "statement"
+            value = statement
 
-        assert offset is not None
-        return code(
-            "{table} FOR SYSTEM_TIME AS OF TIMESTAMP_SUB(CURRENT_TIMESTAMP(), INTERVAL {offset} HOUR);",
-            table=table,
-            offset=offset,
-        )
+        return code(f"{{table}} {at_or_before}({key} => {{value}})", table=table, value=value)
 
 
 class Dialect(BaseDialect, Mixin_Schema):
-    name = "BigQuery"
-    ROUNDS_ON_PREC_LOSS = False  # Technically BigQuery doesn't allow implicit rounding or truncation
+    name = "Snowflake"
+    ROUNDS_ON_PREC_LOSS = False
     TYPE_CLASSES = {
-        # Dates
-        "TIMESTAMP": Timestamp,
-        "DATETIME": Datetime,
+        # Timestamps
+        "TIMESTAMP_NTZ": Timestamp,
+        "TIMESTAMP_LTZ": Timestamp,
+        "TIMESTAMP_TZ": TimestampTZ,
+        "DATE": Date,
         # Numbers
-        "INT64": Integer,
-        "INT32": Integer,
-        "NUMERIC": Decimal,
-        "BIGNUMERIC": Decimal,
-        "FLOAT64": Float,
-        "FLOAT32": Float,
+        "NUMBER": Decimal,
+        "FLOAT": Float,
         # Text
-        "STRING": Text,
+        "TEXT": Text,
         # Boolean
-        "BOOL": Boolean,
+        "BOOLEAN": Boolean,
     }
     MIXINS = {Mixin_Schema, Mixin_MD5, Mixin_NormalizeValue, Mixin_TimeTravel, Mixin_RandomSample}
 
-    def random(self) -> str:
-        return "RAND()"
+    def explain_as_text(self, query: str) -> str:
+        return f"EXPLAIN USING TEXT {query}"
 
     def quote(self, s: str):
-        return f"`{s}`"
+        return f'"{s}"'
 
     def to_string(self, s: str):
         return f"cast({s} as string)"
 
-    def type_repr(self, t) -> str:
-        try:
-            return {str: "STRING", float: "FLOAT64"}[t]
-        except KeyError:
-            return super().type_repr(t)
+    def table_information(self) -> Compilable:
+        return table("INFORMATION_SCHEMA", "TABLES")
 
     def set_timezone_to_utc(self) -> str:
-        raise NotImplementedError()
+        return "ALTER SESSION SET TIMEZONE = 'UTC'"
 
+    def optimizer_hints(self, hints: str) -> str:
+        raise NotImplementedError("Optimizer hints not yet implemented in snowflake")
+
+    def type_repr(self, t) -> str:
+        if isinstance(t, TimestampTZ):
+            return f"timestamp_tz({t.precision})"
+        return super().type_repr(t)
 
-class BigQuery(Database):
-    CONNECT_URI_HELP = "bigquery://<project>/<dataset>"
-    CONNECT_URI_PARAMS = ["dataset"]
-    dialect = Dialect()
 
-    def __init__(self, project, *, dataset, **kw):
-        bigquery = import_bigquery()
+class Snowflake(Database):
+    dialect = Dialect()
+    CONNECT_URI_HELP = "snowflake://<user>:<password>@<account>/<database>/<SCHEMA>?warehouse=<WAREHOUSE>"
+    CONNECT_URI_PARAMS = ["database", "schema"]
+    CONNECT_URI_KWPARAMS = ["warehouse"]
+
+    def __init__(self, *, schema: str, **kw):
+        snowflake, serialization, default_backend = import_snowflake()
+        logging.getLogger("snowflake.connector").setLevel(logging.WARNING)
+
+        # Ignore the error: snowflake.connector.network.RetryRequest: could not find io module state
+        # It's a known issue: https://github.com/snowflakedb/snowflake-connector-python/issues/145
+        logging.getLogger("snowflake.connector.network").disabled = True
+
+        assert '"' not in schema, "Schema name should not contain quotes!"
+        # If a private key is used, read it from the specified path and pass it as "private_key" to the connector.
+        if "key" in kw:
+            with open(kw.get("key"), "rb") as key:
+                if "password" in kw:
+                    raise ConnectError("Cannot use password and key at the same time")
+                if kw.get("private_key_passphrase"):
+                    encoded_passphrase = kw.get("private_key_passphrase").encode()
+                else:
+                    encoded_passphrase = None
+                p_key = serialization.load_pem_private_key(
+                    key.read(),
+                    password=encoded_passphrase,
+                    backend=default_backend(),
+                )
+
+            kw["private_key"] = p_key.private_bytes(
+                encoding=serialization.Encoding.DER,
+                format=serialization.PrivateFormat.PKCS8,
+                encryption_algorithm=serialization.NoEncryption(),
+            )
 
-        self._client = bigquery.Client(project, **kw)
-        self.project = project
-        self.dataset = dataset
-
-        self.default_schema = dataset
-
-    def _normalize_returned_value(self, value):
-        if isinstance(value, bytes):
-            return value.decode()
-        return value
-
-    def _query_atom(self, sql_code: str):
-        from google.cloud import bigquery
-
-        try:
-            result = self._client.query(sql_code).result()
-            columns = [c.name for c in result.schema]
-            rows = list(result)
-        except Exception as e:
-            msg = "Exception when trying to execute SQL code:\n    %s\n\nGot error: %s"
-            raise ConnectError(msg % (sql_code, e))
-
-        if rows and isinstance(rows[0], bigquery.table.Row):
-            rows = [tuple(self._normalize_returned_value(v) for v in row.values()) for row in rows]
-        return QueryResult(rows, columns)
+        self._conn = snowflake.connector.connect(schema=f'"{schema}"', **kw)
 
-    def _query(self, sql_code: Union[str, ThreadLocalInterpreter]) -> QueryResult:
-        return apply_query(self._query_atom, sql_code)
+        self.default_schema = schema
 
     def close(self):
         super().close()
-        self._client.close()
+        self._conn.close()
+
+    def _query(self, sql_code: Union[str, ThreadLocalInterpreter]):
+        "Uses the standard SQL cursor interface"
+        return self._query_conn(self._conn, sql_code)
 
     def select_table_schema(self, path: DbPath) -> str:
-        project, schema, name = self._normalize_table_path(path)
+        """Provide SQL for selecting the table schema as (name, type, date_prec, num_prec)"""
+        database, schema, name = self._normalize_table_path(path)
+        info_schema_path = ["information_schema", "columns"]
+        if database:
+            info_schema_path.insert(0, database)
+
         return (
-            "SELECT column_name, data_type, 6 as datetime_precision, 38 as numeric_precision, 9 as numeric_scale "
-            f"FROM `{project}`.`{schema}`.INFORMATION_SCHEMA.COLUMNS "
+            "SELECT column_name, data_type, datetime_precision, numeric_precision, numeric_scale "
+            f"FROM {'.'.join(info_schema_path)} "
             f"WHERE table_name = '{name}' AND table_schema = '{schema}'"
         )
 
-    def query_table_unique_columns(self, path: DbPath) -> List[str]:
-        return []
-
     def _normalize_table_path(self, path: DbPath) -> DbPath:
-        if len(path) == 0:
-            raise ValueError(f"{self.name}: Bad table path for {self}: ()")
-        elif len(path) == 1:
-            return (self.project, self.default_schema, path[0])
+        if len(path) == 1:
+            return None, self.default_schema, path[0]
         elif len(path) == 2:
-            return (self.project,) + path
+            return None, path[0], path[1]
         elif len(path) == 3:
             return path
-        else:
-            raise ValueError(
-                f"{self.name}: Bad table path for {self}: '{'.'.join(path)}'. Expected form: [project.]schema.table"
-            )
 
-    def parse_table_name(self, name: str) -> DbPath:
-        path = parse_table_name(name)
-        return tuple(i for i in self._normalize_table_path(path) if i is not None)
+        raise ValueError(
+            f"{self.name}: Bad table path for {self}: '{'.'.join(path)}'. Expected format: table, schema.table, or database.schema.table"
+        )
 
     @property
     def is_autocommit(self) -> bool:
         return True
+
+    def query_table_unique_columns(self, path: DbPath) -> List[str]:
+        return []
```

### Comparing `data_diff-0.7.4/data_diff/sqeleton/databases/clickhouse.py` & `data_diff-0.7.5/data_diff/sqeleton/databases/clickhouse.py`

 * *Files identical despite different names*

### Comparing `data_diff-0.7.4/data_diff/sqeleton/databases/databricks.py` & `data_diff-0.7.5/data_diff/sqeleton/databases/databricks.py`

 * *Files identical despite different names*

### Comparing `data_diff-0.7.4/data_diff/sqeleton/databases/duckdb.py` & `data_diff-0.7.5/data_diff/sqeleton/databases/duckdb.py`

 * *Files identical despite different names*

### Comparing `data_diff-0.7.4/data_diff/sqeleton/databases/mssql.py` & `data_diff-0.7.5/data_diff/sqeleton/databases/mssql.py`

 * *Files identical despite different names*

### Comparing `data_diff-0.7.4/data_diff/sqeleton/databases/mysql.py` & `data_diff-0.7.5/data_diff/sqeleton/databases/mysql.py`

 * *Files identical despite different names*

### Comparing `data_diff-0.7.4/data_diff/sqeleton/databases/oracle.py` & `data_diff-0.7.5/data_diff/sqeleton/databases/oracle.py`

 * *Files 1% similar despite different names*

```diff
@@ -88,14 +88,15 @@
         "NUMBER": Decimal,
         "FLOAT": Float,
         # Text
         "CHAR": Text,
         "NCHAR": Text,
         "NVARCHAR2": Text,
         "VARCHAR2": Text,
+        "DATE": Timestamp,
     }
     ROUNDS_ON_PREC_LOSS = True
     PLACEHOLDER_TABLE = "DUAL"
     MIXINS = {Mixin_Schema, Mixin_MD5, Mixin_NormalizeValue, Mixin_RandomSample}
 
     def quote(self, s: str):
         return f'"{s}"'
```

### Comparing `data_diff-0.7.4/data_diff/sqeleton/databases/postgresql.py` & `data_diff-0.7.5/data_diff/sqeleton/databases/postgresql.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from ..abcs.database_types import (
     DbPath,
+    JSON,
     Timestamp,
     TimestampTZ,
     Float,
     Decimal,
     Integer,
     TemporalType,
     Native_UUID,
@@ -45,14 +46,17 @@
 
     def normalize_number(self, value: str, coltype: FractionalType) -> str:
         return self.to_string(f"{value}::decimal(38, {coltype.precision})")
 
     def normalize_boolean(self, value: str, _coltype: Boolean) -> str:
         return self.to_string(f"{value}::int")
 
+    def normalize_json(self, value: str, _coltype: JSON) -> str:
+        return f"{value}::text"
+
 
 class PostgresqlDialect(BaseDialect, Mixin_Schema):
     name = "PostgreSQL"
     ROUNDS_ON_PREC_LOSS = True
     SUPPORTS_PRIMARY_KEY = True
     SUPPORTS_INDEXES = True
     MIXINS = {Mixin_Schema, Mixin_MD5, Mixin_NormalizeValue, Mixin_RandomSample}
@@ -72,17 +76,18 @@
         "numeric": Decimal,
         "bigint": Integer,
         # Text
         "character": Text,
         "character varying": Text,
         "varchar": Text,
         "text": Text,
-        # UUID
+
+        "json": JSON,
+        "jsonb": JSON,
         "uuid": Native_UUID,
-        # Boolean
         "boolean": Boolean,
     }
 
     def quote(self, s: str):
         return f'"{s}"'
 
     def to_string(self, s: str):
```

### Comparing `data_diff-0.7.4/data_diff/sqeleton/databases/presto.py` & `data_diff-0.7.5/data_diff/sqeleton/databases/presto.py`

 * *Files identical despite different names*

### Comparing `data_diff-0.7.4/data_diff/sqeleton/databases/redshift.py` & `data_diff-0.7.5/data_diff/sqeleton/databases/redshift.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,9 +1,16 @@
 from typing import List, Dict
-from ..abcs.database_types import Float, TemporalType, FractionalType, DbPath, TimestampTZ
+from ..abcs.database_types import (
+    Float,
+    JSON,
+    TemporalType,
+    FractionalType,
+    DbPath,
+    TimestampTZ,
+)
 from ..abcs.mixins import AbstractMixin_MD5
 from .postgresql import (
     PostgreSQL,
     MD5_HEXDIGITS,
     CHECKSUM_HEXDIGITS,
     TIMESTAMP_PRECISION_POS,
     PostgresqlDialect,
@@ -36,21 +43,25 @@
         return (
             f"RPAD(LEFT({timestamp6}, {TIMESTAMP_PRECISION_POS+coltype.precision}), {TIMESTAMP_PRECISION_POS+6}, '0')"
         )
 
     def normalize_number(self, value: str, coltype: FractionalType) -> str:
         return self.to_string(f"{value}::decimal(38,{coltype.precision})")
 
+    def normalize_json(self, value: str, _coltype: JSON) -> str:
+        return f'nvl2({value}, json_serialize({value}), NULL)'
+
 
 class Dialect(PostgresqlDialect):
     name = "Redshift"
     TYPE_CLASSES = {
         **PostgresqlDialect.TYPE_CLASSES,
         "double": Float,
         "real": Float,
+        "super": JSON,
     }
     SUPPORTS_INDEXES = False
 
     def concat(self, items: List[str]) -> str:
         joined_exprs = " || ".join(items)
         return f"({joined_exprs})"
 
@@ -105,19 +116,56 @@
         if not rows:
             raise RuntimeError(f"{self.name}: Table '{'.'.join(path)}' does not exist, or has no columns")
 
         d = {r[0]: r for r in rows}
         assert len(d) == len(rows)
         return d
 
+    def select_view_columns(self, path: DbPath) -> str:
+        _, schema, table = self._normalize_table_path(path)
+
+        return (
+            """select * from pg_get_cols('{}.{}')
+                cols(view_schema name, view_name name, col_name name, col_type varchar, col_num int)
+            """.format(schema, table)
+        )
+
+    def query_pg_get_cols(self, path: DbPath) -> Dict[str, tuple]:
+        rows = self.query(self.select_view_columns(path), list)
+
+        if not rows:
+            raise RuntimeError(f"{self.name}: View '{'.'.join(path)}' does not exist, or has no columns")
+
+        output = {}
+        for r in rows:
+            col_name = r[2]
+            type_info = r[3].split('(')
+            base_type = type_info[0]
+            precision = None
+            scale = None
+
+            if len(type_info) > 1:
+                if base_type == 'numeric':
+                    precision, scale = type_info[1][:-1].split(',')
+                    precision = int(precision)
+                    scale = int(scale)
+                
+            out = [col_name, base_type, None, precision, scale]
+            output[col_name] = tuple(out)
+
+        return output
+
     def query_table_schema(self, path: DbPath) -> Dict[str, tuple]:
         try:
             return super().query_table_schema(path)
         except RuntimeError:
-            return self.query_external_table_schema(path)
+            try:
+                return self.query_external_table_schema(path)	
+            except RuntimeError:	
+                return self.query_pg_get_cols() 
 
     def _normalize_table_path(self, path: DbPath) -> DbPath:
         if len(path) == 1:
             return None, self.default_schema, path[0]
         elif len(path) == 2:
             return None, path[0], path[1]
         elif len(path) == 3:
```

### Comparing `data_diff-0.7.4/data_diff/sqeleton/databases/trino.py` & `data_diff-0.7.5/data_diff/sqeleton/databases/trino.py`

 * *Files identical despite different names*

### Comparing `data_diff-0.7.4/data_diff/sqeleton/databases/vertica.py` & `data_diff-0.7.5/data_diff/sqeleton/databases/vertica.py`

 * *Files identical despite different names*

### Comparing `data_diff-0.7.4/data_diff/sqeleton/queries/api.py` & `data_diff-0.7.5/data_diff/sqeleton/queries/api.py`

 * *Files identical despite different names*

### Comparing `data_diff-0.7.4/data_diff/sqeleton/queries/ast_classes.py` & `data_diff-0.7.5/data_diff/sqeleton/queries/ast_classes.py`

 * *Files 0% similar despite different names*

```diff
@@ -348,15 +348,17 @@
 @dataclass(eq=False, order=False)
 class IsDistinctFrom(ExprNode, LazyOps):
     a: Expr
     b: Expr
     type = bool
 
     def compile(self, c: Compiler) -> str:
-        return c.dialect.is_distinct_from(c.compile(self.a), c.compile(self.b))
+        a = c.dialect.to_comparable(c.compile(self.a), self.a.type)
+        b = c.dialect.to_comparable(c.compile(self.b), self.b.type)
+        return c.dialect.is_distinct_from(a, b)
 
 
 @dataclass(eq=False, order=False)
 class BinOp(ExprNode, LazyOps):
     op: str
     args: Sequence[Expr]
```

### Comparing `data_diff-0.7.4/data_diff/sqeleton/queries/compiler.py` & `data_diff-0.7.5/data_diff/sqeleton/queries/compiler.py`

 * *Files identical despite different names*

### Comparing `data_diff-0.7.4/data_diff/sqeleton/queries/extras.py` & `data_diff-0.7.5/data_diff/sqeleton/queries/extras.py`

 * *Files identical despite different names*

### Comparing `data_diff-0.7.4/data_diff/sqeleton/query_utils.py` & `data_diff-0.7.5/data_diff/sqeleton/query_utils.py`

 * *Files identical despite different names*

### Comparing `data_diff-0.7.4/data_diff/sqeleton/repl.py` & `data_diff-0.7.5/data_diff/sqeleton/repl.py`

 * *Files identical despite different names*

### Comparing `data_diff-0.7.4/data_diff/sqeleton/schema.py` & `data_diff-0.7.5/data_diff/sqeleton/schema.py`

 * *Files identical despite different names*

### Comparing `data_diff-0.7.4/data_diff/sqeleton/utils.py` & `data_diff-0.7.5/data_diff/sqeleton/utils.py`

 * *Files identical despite different names*

### Comparing `data_diff-0.7.4/data_diff/table_segment.py` & `data_diff-0.7.5/data_diff/table_segment.py`

 * *Files identical despite different names*

### Comparing `data_diff-0.7.4/data_diff/thread_utils.py` & `data_diff-0.7.5/data_diff/thread_utils.py`

 * *Files identical despite different names*

### Comparing `data_diff-0.7.4/data_diff/tracking.py` & `data_diff-0.7.5/data_diff/tracking.py`

 * *Files identical despite different names*

### Comparing `data_diff-0.7.4/data_diff/utils.py` & `data_diff-0.7.5/data_diff/utils.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+import json
 import logging
 import re
 from typing import Dict, Iterable, Sequence
 from urllib.parse import urlparse
 import operator
 import threading
 from datetime import datetime
@@ -140,7 +141,31 @@
 
     string_output += extra_info_str
 
     for k, v in extra_info_dict.items():
         string_output += f"\n{k}: {v}"
 
     return string_output
+
+
+def _jsons_equiv(a: str, b: str):
+    try:
+        return json.loads(a) == json.loads(b)
+    except (ValueError, TypeError, json.decoder.JSONDecodeError):  # not valid jsons
+        return False
+
+
+def diffs_are_equiv_jsons(diff: list, json_cols: dict):
+    overriden_diff_cols = set()
+    if (len(diff) != 2) or ({diff[0][0], diff[1][0]} != {'+', '-'}):
+        return False, overriden_diff_cols
+    match = True
+    for i, (col_a, col_b) in enumerate(safezip(diff[0][1][1:], diff[1][1][1:])):  # index 0 is extra_columns first elem
+        # we only attempt to parse columns of JSON type, but we still need to check if non-json columns don't match
+        match = col_a == col_b
+        if not match and (i in json_cols):
+            if _jsons_equiv(col_a, col_b):
+                overriden_diff_cols.add(json_cols[i])
+                match = True
+        if not match:
+            break
+    return match, overriden_diff_cols
```

### Comparing `data_diff-0.7.4/pyproject.toml` & `data_diff-0.7.5/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "data-diff"
-version = "0.7.4"
+version = "0.7.5"
 description = "Command-line tool and Python library to efficiently diff rows across two different databases."
 authors = ["Datafold <data-diff@datafold.com>"]
 license = "MIT"
 readme = "README.md"
 repository = "https://github.com/datafold/data-diff"
 documentation = ""
 classifiers = [
@@ -36,15 +36,15 @@
 psycopg2 = {version="*", optional=true}
 snowflake-connector-python = {version="^2.7.2", optional=true}
 cryptography = {version="*", optional=true}
 trino = {version="^0.314.0", optional=true}
 presto-python-client = {version="*", optional=true}
 clickhouse-driver = {version="*", optional=true}
 duckdb = {version="^0.7.0", optional=true}
-dbt-artifacts-parser = {version="^0.2.5", optional=true}
+dbt-artifacts-parser = {version="^0.3.0", optional=true}
 dbt-core = {version="^1.0.0", optional=true}
 keyring = "*"
 tabulate = "^0.9.0"
 preql = {version="^0.2.19", optional=true}
 cx_Oracle = {version="*", optional=true}
 vertica-python = {version="*", optional=true}
 
@@ -57,15 +57,15 @@
 snowflake-connector-python = "^2.7.2"
 cryptography = "*"
 trino = "^0.314.0"
 presto-python-client = "*"
 clickhouse-driver = "*"
 vertica-python = "*"
 duckdb = "^0.7.0"
-dbt-artifacts-parser = "^0.2.5"
+dbt-artifacts-parser = "^0.3.0"
 dbt-core = "^1.0.0"
 # google-cloud-bigquery = "*"
 # databricks-sql-connector = "*"
 
 [tool.poetry.extras]
 # When adding, update also: README + dev deps just above
 preql = ["preql"]
```

### Comparing `data_diff-0.7.4/PKG-INFO` & `data_diff-0.7.5/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: data-diff
-Version: 0.7.4
+Version: 0.7.5
 Summary: Command-line tool and Python library to efficiently diff rows across two different databases.
 Home-page: https://github.com/datafold/data-diff
 License: MIT
 Author: Datafold
 Author-email: data-diff@datafold.com
 Requires-Python: >=3.7,<4.0
 Classifier: Development Status :: 2 - Pre-Alpha
@@ -36,15 +36,15 @@
 Provides-Extra: snowflake
 Provides-Extra: trino
 Provides-Extra: vertica
 Requires-Dist: click (>=8.1,<9.0)
 Requires-Dist: clickhouse-driver ; extra == "clickhouse"
 Requires-Dist: cryptography ; extra == "snowflake"
 Requires-Dist: cx_Oracle ; extra == "oracle"
-Requires-Dist: dbt-artifacts-parser (>=0.2.5,<0.3.0) ; extra == "dbt"
+Requires-Dist: dbt-artifacts-parser (>=0.3.0,<0.4.0) ; extra == "dbt"
 Requires-Dist: dbt-core (>=1.0.0,<2.0.0) ; extra == "dbt"
 Requires-Dist: dsnparse (<0.2.0) ; python_version < "3.8.0"
 Requires-Dist: dsnparse ; python_version >= "3.8.0"
 Requires-Dist: duckdb (>=0.7.0,<0.8.0) ; extra == "duckdb"
 Requires-Dist: keyring
 Requires-Dist: mysql-connector-python (==8.0.29) ; extra == "mysql"
 Requires-Dist: preql (>=0.2.19,<0.3.0) ; extra == "preql"
@@ -60,141 +60,85 @@
 Project-URL: Repository, https://github.com/datafold/data-diff
 Description-Content-Type: text/markdown
 
 <p align="center">
     <img alt="Datafold" src="https://user-images.githubusercontent.com/1799931/196497110-d3de1113-a97f-4322-b531-026d859b867a.png" width="50%" />
 </p>
 
-# **data-diff**
+<h1 align="center">
+data-diff
+</h1>
+
+<h2 align="center">
+Develop dbt models faster by testing as you code.
+</h2>
+<h4 align="center">
+See how every change to dbt code affects the data produced in the modified model and downstream.
+</h4>
+<br>
 
 ## What is `data-diff`?
-data-diff is a **free, open-source tool** that enables data professionals to detect differences in values between any two tables.
 
-## Documentation
+data-diff is an open source package that you can use to see the impact of your dbt code changes on your dbt models as you code.
 
-[**🗎 Documentation**](https://docs.datafold.com/guides/os_data_diff) - our detailed documentation has everything you need to start diffing.
+<div align="center">
 
-### Databases we support
+![development_testing_gif](https://user-images.githubusercontent.com/1799931/236354286-d1d044cf-2168-4128-8a21-8c8ca7fd494c.gif)
 
-- PostgreSQL >=10
-- MySQL
-- Snowflake
-- BigQuery
-- Redshift
-- Oracle
-- Presto
-- Databricks
-- Trino
-- Clickhouse
-- Vertica
-- DuckDB >=0.6
-- SQLite (coming soon)
+</div>
 
-For their corresponding connection strings, check out our [detailed table](https://github.com/datafold/data-diff/blob/master/docs/supported-databases.md).
+<br>
 
-#### Looking for a database not on the list?
-If a database is not on the list, we'd still love to support it. [Please open an issue](https://github.com/datafold/data-diff/issues) to discuss it, or vote on existing requests to push them up our todo list.
-
-## Get started
-
-### Installation
-
-#### First, install `data-diff` using `pip`.
+## Getting Started
 
+**Install `data-diff`**
 ```
 pip install data-diff
 ```
 
-#### Then, install one or more driver(s) specific to the database(s) you want to connect to.
-
-- `pip install 'data-diff[mysql]'`
-
-- `pip install 'data-diff[postgresql]'`
-
-- `pip install 'data-diff[snowflake]'`
-
-- `pip install 'data-diff[presto]'`
-
-- `pip install 'data-diff[oracle]'`
-
-- `pip install 'data-diff[trino]'`
-
-- `pip install 'data-diff[clickhouse]'`
-
-- `pip install 'data-diff[vertica]'`
-
-- For BigQuery, see: https://pypi.org/project/google-cloud-bigquery/
-
-_Some drivers have dependencies that cannot be installed using `pip` and still need to be installed manually._
-
-### Run your first diff
-
-Once you've installed `data-diff`, you can run it from the command line.
-
+**Update a few lines in your `dbt_project.yml`**
 ```
-data-diff DB1_URI TABLE1_NAME DB2_URI TABLE2_NAME [OPTIONS]
+#dbt_project.yml
+vars:
+  data_diff:
+    prod_database: my_database
+    prod_schema: my_default_schema
 ```
 
-Be sure to read [the docs](https://docs.datafold.com/reference/open_source/cli) for detailed instructions how to build one of these commands depending on your database setup.
-
-#### Code Example: Diff Tables Between Databases
-Here's an example command for your copy/pasting, taken from the screenshot above when we diffed data between Snowflake and Postgres.
+**Run your first data diff!**
 
 ```
-data-diff \
-  postgresql://<username>:'<password>'@localhost:5432/<database> \
-  <table> \
-  "snowflake://<username>:<password>@<password>/<DATABASE>/<SCHEMA>?warehouse=<WAREHOUSE>&role=<ROLE>" \
-  <TABLE> \
-  -k activity_id \
-  -c activity \
-  -w "event_timestamp < '2022-10-10'"
+dbt run && data-diff --dbt
 ```
 
-#### Code Example: Diff Tables Within a Database
+We recommend you get started by walking through [our simple setup instructions](https://docs.datafold.com/development_testing/open_source) which contain examples and details.
 
-```
-data-diff \
-  "snowflake://<username>:<password>@<password>/<DATABASE>/<SCHEMA_1>?warehouse=<WAREHOUSE>&role=<ROLE>" <TABLE_1> \
-  <SCHEMA_2>.<TABLE_2> \
-  -k org_id \
-  -c created_at -c is_internal \
-  -w "org_id != 1 and org_id < 2000" \
-  -m test_results_%t \
-  --materialize-all-rows \
-  --table-write-limit 10000
-```
-
-In both code examples, I've used `<>` carrots to represent values that **should be replaced with your values** in the database connection strings. For the flags (`-k`, `-c`, etc.), I opted for "real" values (`org_id`, `is_internal`) to give you a more realistic view of what your command will look like.
+Please reach out on the dbt Slack in [#tools-datafold](https://getdbt.slack.com/archives/C03D25A92UU) if you have any trouble whatsoever getting started!
 
-### We're here to help!
+<br><br>
 
-We're here to help! Please post any questions in [GitHub Discussions](https://github.com/datafold/data-diff/discussions).
+### Diffing between databases
 
-## How to Use
+Check out our [documentation](https://github.com/datafold/data-diff/blob/master/docs/supported-databases.md) if you're looking to compare data across databases (for example, between Postgres and Snowflake).
 
-* [Examples with dbt, joindiff, and hashdiff](https://docs.datafold.com/reference/open_source/cli#examples)
-* [Examples with Python](https://data-diff.readthedocs.io/en/latest/python-api.html)
-* [How to use with TOML configuration file](https://docs.datafold.com/reference/open_source/cli#toml-config-file)
+<br>
 
-## How to Contribute
-* Feel free to open an issue or contribute to the project by working on an existing issue.
-* Please read the [contributing guidelines](https://github.com/datafold/data-diff/blob/master/CONTRIBUTING.md) to get started.
-* To add a new database driver, check out [docs](https://github.com/datafold/data-diff/blob/master/docs/new-database-driver-guide.rst).
+## Contributors
 
-Big thanks to everyone who contributed so far:
+We thank everyone who contributed so far!
 
 <a href="https://github.com/datafold/data-diff/graphs/contributors">
   <img src="https://contributors-img.web.app/image?repo=datafold/data-diff" />
 </a>
 
-## Technical Explanation
-
-Check out this [technical explanation](https://github.com/datafold/data-diff/blob/master/docs/technical-explanation.md) of how data-diff works.
+<br>
 
 ## Analytics
+
 * [Usage Analytics & Data Privacy](https://github.com/datafold/data-diff/blob/master/docs/usage_analytics.md)
 
+<br>
+
 ## License
 
 This project is licensed under the terms of the [MIT License](https://github.com/datafold/data-diff/blob/master/LICENSE).
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

