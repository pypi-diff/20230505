# Comparing `tmp/astro-sdk-python-1.6.0a1.tar.gz` & `tmp/astro-sdk-python-1.7.0a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "astro-sdk-python-1.6.0a1.tar", last modified: Fri Apr 21 19:05:24 2023, max compression
+gzip compressed data, was "astro-sdk-python-1.7.0a1.tar", last modified: Fri May  5 14:23:20 2023, max compression
```

## Comparing `astro-sdk-python-1.6.0a1.tar` & `astro-sdk-python-1.7.0a1.tar`

### file list

```diff
@@ -1,93 +1,94 @@
-lrwxr-xr-x   0        0        0        0 2023-04-21 19:05:11.619546 astro-sdk-python-1.6.0a1/LICENSE -> ../LICENSE
--rw-r--r--   0        0        0     8344 2023-04-21 19:05:11.619546 astro-sdk-python-1.6.0a1/README.md
--rw-r--r--   0        0        0     5313 2023-04-21 19:05:11.631546 astro-sdk-python-1.6.0a1/pyproject.toml
--rw-r--r--   0        0        0      687 2023-04-21 19:05:11.631546 astro-sdk-python-1.6.0a1/src/astro/__init__.py
--rw-r--r--   0        0        0        0 2023-04-21 19:05:11.631546 astro-sdk-python-1.6.0a1/src/astro/airflow/__init__.py
--rw-r--r--   0        0        0     1605 2023-04-21 19:05:11.631546 astro-sdk-python-1.6.0a1/src/astro/airflow/datasets.py
--rw-r--r--   0        0        0     2018 2023-04-21 19:05:11.631546 astro-sdk-python-1.6.0a1/src/astro/constants.py
--rw-r--r--   0        0        0        0 2023-04-21 19:05:11.631546 astro-sdk-python-1.6.0a1/src/astro/custom_backend/__init__.py
--rw-r--r--   0        0        0     2187 2023-04-21 19:05:11.631546 astro-sdk-python-1.6.0a1/src/astro/custom_backend/astro_custom_backend.py
--rw-r--r--   0        0        0     3915 2023-04-21 19:05:11.631546 astro-sdk-python-1.6.0a1/src/astro/custom_backend/serializer.py
--rw-r--r--   0        0        0     1876 2023-04-21 19:05:11.631546 astro-sdk-python-1.6.0a1/src/astro/databases/__init__.py
--rw-r--r--   0        0        0        0 2023-04-21 19:05:11.631546 astro-sdk-python-1.6.0a1/src/astro/databases/aws/__init__.py
--rw-r--r--   0        0        0    18189 2023-04-21 19:05:11.631546 astro-sdk-python-1.6.0a1/src/astro/databases/aws/redshift.py
--rw-r--r--   0        0        0    37127 2023-04-21 19:05:11.631546 astro-sdk-python-1.6.0a1/src/astro/databases/base.py
--rw-r--r--   0        0        0        0 2023-04-21 19:05:11.631546 astro-sdk-python-1.6.0a1/src/astro/databases/databricks/__init__.py
--rw-r--r--   0        0        0     7247 2023-04-21 19:05:11.631546 astro-sdk-python-1.6.0a1/src/astro/databases/databricks/api_utils.py
--rw-r--r--   0        0        0    17788 2023-04-21 19:05:11.631546 astro-sdk-python-1.6.0a1/src/astro/databases/databricks/delta.py
--rw-r--r--   0        0        0        0 2023-04-21 19:05:11.631546 astro-sdk-python-1.6.0a1/src/astro/databases/databricks/load_file/__init__.py
--rw-r--r--   0        0        0      720 2023-04-21 19:05:11.631546 astro-sdk-python-1.6.0a1/src/astro/databases/databricks/load_file/jinja_templates/autoloader.py.jinja2
--rw-r--r--   0        0        0      647 2023-04-21 19:05:11.631546 astro-sdk-python-1.6.0a1/src/astro/databases/databricks/load_file/jinja_templates/copy_into.py.jinja2
--rw-r--r--   0        0        0      913 2023-04-21 19:05:11.631546 astro-sdk-python-1.6.0a1/src/astro/databases/databricks/load_file/jinja_templates/load_file_to_delta.py.jinja2
--rw-r--r--   0        0        0      512 2023-04-21 19:05:11.631546 astro-sdk-python-1.6.0a1/src/astro/databases/databricks/load_file/jinja_templates/load_secrets.py.jinja2
--rw-r--r--   0        0        0     6287 2023-04-21 19:05:11.631546 astro-sdk-python-1.6.0a1/src/astro/databases/databricks/load_file/load_file_job.py
--rw-r--r--   0        0        0      880 2023-04-21 19:05:11.631546 astro-sdk-python-1.6.0a1/src/astro/databases/databricks/load_file/load_file_python_code_generator.py
--rw-r--r--   0        0        0     2687 2023-04-21 19:05:11.631546 astro-sdk-python-1.6.0a1/src/astro/databases/databricks/load_options.py
--rw-r--r--   0        0        0     6181 2023-04-21 19:05:11.631546 astro-sdk-python-1.6.0a1/src/astro/databases/duckdb.py
--rw-r--r--   0        0        0        0 2023-04-21 19:05:11.631546 astro-sdk-python-1.6.0a1/src/astro/databases/google/__init__.py
--rw-r--r--   0        0        0    26823 2023-04-21 19:05:11.631546 astro-sdk-python-1.6.0a1/src/astro/databases/google/bigquery.py
--rw-r--r--   0        0        0    17049 2023-04-21 19:05:11.635546 astro-sdk-python-1.6.0a1/src/astro/databases/mssql.py
--rw-r--r--   0        0        0    10678 2023-04-21 19:05:11.635546 astro-sdk-python-1.6.0a1/src/astro/databases/postgres.py
--rw-r--r--   0        0        0    42201 2023-04-21 19:05:11.635546 astro-sdk-python-1.6.0a1/src/astro/databases/snowflake.py
--rw-r--r--   0        0        0     6508 2023-04-21 19:05:11.635546 astro-sdk-python-1.6.0a1/src/astro/databases/sqlite.py
--rw-r--r--   0        0        0        0 2023-04-21 19:05:11.635546 astro-sdk-python-1.6.0a1/src/astro/dataframes/__init__.py
--rw-r--r--   0        0        0     4116 2023-04-21 19:05:11.635546 astro-sdk-python-1.6.0a1/src/astro/dataframes/load_options.py
--rw-r--r--   0        0        0     1977 2023-04-21 19:05:11.635546 astro-sdk-python-1.6.0a1/src/astro/dataframes/pandas.py
--rw-r--r--   0        0        0     1137 2023-04-21 19:05:11.635546 astro-sdk-python-1.6.0a1/src/astro/exceptions.py
--rw-r--r--   0        0        0     1096 2023-04-21 19:05:11.635546 astro-sdk-python-1.6.0a1/src/astro/files/__init__.py
--rw-r--r--   0        0        0    10151 2023-04-21 19:05:11.635546 astro-sdk-python-1.6.0a1/src/astro/files/base.py
--rw-r--r--   0        0        0     1535 2023-04-21 19:05:11.635546 astro-sdk-python-1.6.0a1/src/astro/files/locations/__init__.py
--rw-r--r--   0        0        0        0 2023-04-21 19:05:11.635546 astro-sdk-python-1.6.0a1/src/astro/files/locations/amazon/__init__.py
--rw-r--r--   0        0        0     3605 2023-04-21 19:05:11.635546 astro-sdk-python-1.6.0a1/src/astro/files/locations/amazon/s3.py
--rw-r--r--   0        0        0        0 2023-04-21 19:05:11.635546 astro-sdk-python-1.6.0a1/src/astro/files/locations/azure/__init__.py
--rw-r--r--   0        0        0     4290 2023-04-21 19:05:11.635546 astro-sdk-python-1.6.0a1/src/astro/files/locations/azure/wasb.py
--rw-r--r--   0        0        0     6355 2023-04-21 19:05:11.635546 astro-sdk-python-1.6.0a1/src/astro/files/locations/base.py
--rw-r--r--   0        0        0     2374 2023-04-21 19:05:11.635546 astro-sdk-python-1.6.0a1/src/astro/files/locations/ftp.py
--rw-r--r--   0        0        0        0 2023-04-21 19:05:11.635546 astro-sdk-python-1.6.0a1/src/astro/files/locations/google/__init__.py
--rw-r--r--   0        0        0     4420 2023-04-21 19:05:11.635546 astro-sdk-python-1.6.0a1/src/astro/files/locations/google/gcs.py
--rw-r--r--   0        0        0     5006 2023-04-21 19:05:11.635546 astro-sdk-python-1.6.0a1/src/astro/files/locations/google/gdrive.py
--rw-r--r--   0        0        0     1303 2023-04-21 19:05:11.635546 astro-sdk-python-1.6.0a1/src/astro/files/locations/http.py
--rw-r--r--   0        0        0     1531 2023-04-21 19:05:11.635546 astro-sdk-python-1.6.0a1/src/astro/files/locations/local.py
--rw-r--r--   0        0        0     3267 2023-04-21 19:05:11.635546 astro-sdk-python-1.6.0a1/src/astro/files/locations/sftp.py
--rw-r--r--   0        0        0        0 2023-04-21 19:05:11.635546 astro-sdk-python-1.6.0a1/src/astro/files/operators/__init__.py
--rw-r--r--   0        0        0     1595 2023-04-21 19:05:11.635546 astro-sdk-python-1.6.0a1/src/astro/files/operators/files.py
--rw-r--r--   0        0        0     2576 2023-04-21 19:05:11.635546 astro-sdk-python-1.6.0a1/src/astro/files/types/__init__.py
--rw-r--r--   0        0        0     1504 2023-04-21 19:05:11.635546 astro-sdk-python-1.6.0a1/src/astro/files/types/base.py
--rw-r--r--   0        0        0     1900 2023-04-21 19:05:11.635546 astro-sdk-python-1.6.0a1/src/astro/files/types/csv.py
--rw-r--r--   0        0        0     2197 2023-04-21 19:05:11.635546 astro-sdk-python-1.6.0a1/src/astro/files/types/json.py
--rw-r--r--   0        0        0     3652 2023-04-21 19:05:11.635546 astro-sdk-python-1.6.0a1/src/astro/files/types/ndjson.py
--rw-r--r--   0        0        0     2848 2023-04-21 19:05:11.635546 astro-sdk-python-1.6.0a1/src/astro/files/types/parquet.py
--rw-r--r--   0        0        0      700 2023-04-21 19:05:11.635546 astro-sdk-python-1.6.0a1/src/astro/lineage/__init__.py
--rw-r--r--   0        0        0     4264 2023-04-21 19:05:11.635546 astro-sdk-python-1.6.0a1/src/astro/lineage/facets.py
--rw-r--r--   0        0        0     3910 2023-04-21 19:05:11.635546 astro-sdk-python-1.6.0a1/src/astro/options.py
--rw-r--r--   0        0        0     1117 2023-04-21 19:05:11.635546 astro-sdk-python-1.6.0a1/src/astro/query_modifier.py
--rw-r--r--   0        0        0     3791 2023-04-21 19:05:11.635546 astro-sdk-python-1.6.0a1/src/astro/settings.py
--rw-r--r--   0        0        0     3194 2023-04-21 19:05:11.635546 astro-sdk-python-1.6.0a1/src/astro/sql/__init__.py
--rw-r--r--   0        0        0        0 2023-04-21 19:05:11.635546 astro-sdk-python-1.6.0a1/src/astro/sql/operators/__init__.py
--rw-r--r--   0        0        0     7857 2023-04-21 19:05:11.635546 astro-sdk-python-1.6.0a1/src/astro/sql/operators/append.py
--rw-r--r--   0        0        0    18379 2023-04-21 19:05:11.635546 astro-sdk-python-1.6.0a1/src/astro/sql/operators/base_decorator.py
--rw-r--r--   0        0        0      334 2023-04-21 19:05:11.635546 astro-sdk-python-1.6.0a1/src/astro/sql/operators/base_operator.py
--rw-r--r--   0        0        0    11280 2023-04-21 19:05:11.635546 astro-sdk-python-1.6.0a1/src/astro/sql/operators/cleanup.py
--rw-r--r--   0        0        0     7870 2023-04-21 19:05:11.635546 astro-sdk-python-1.6.0a1/src/astro/sql/operators/data_validations/check_column.py
--rw-r--r--   0        0        0     3696 2023-04-21 19:05:11.635546 astro-sdk-python-1.6.0a1/src/astro/sql/operators/data_validations/check_table.py
--rw-r--r--   0        0        0    15366 2023-04-21 19:05:11.635546 astro-sdk-python-1.6.0a1/src/astro/sql/operators/dataframe.py
--rw-r--r--   0        0        0     1435 2023-04-21 19:05:11.635546 astro-sdk-python-1.6.0a1/src/astro/sql/operators/drop.py
--rw-r--r--   0        0        0     2693 2023-04-21 19:05:11.635546 astro-sdk-python-1.6.0a1/src/astro/sql/operators/export_file.py
--rw-r--r--   0        0        0     2715 2023-04-21 19:05:11.635546 astro-sdk-python-1.6.0a1/src/astro/sql/operators/export_table_to_file.py
--rw-r--r--   0        0        0     7035 2023-04-21 19:05:11.635546 astro-sdk-python-1.6.0a1/src/astro/sql/operators/export_to_file.py
--rw-r--r--   0        0        0    17274 2023-04-21 19:05:11.635546 astro-sdk-python-1.6.0a1/src/astro/sql/operators/load_file.py
--rw-r--r--   0        0        0     8824 2023-04-21 19:05:11.635546 astro-sdk-python-1.6.0a1/src/astro/sql/operators/merge.py
--rw-r--r--   0        0        0     9902 2023-04-21 19:05:11.635546 astro-sdk-python-1.6.0a1/src/astro/sql/operators/raw_sql.py
--rw-r--r--   0        0        0     7401 2023-04-21 19:05:11.635546 astro-sdk-python-1.6.0a1/src/astro/sql/operators/transform.py
--rw-r--r--   0        0        0      880 2023-04-21 19:05:11.635546 astro-sdk-python-1.6.0a1/src/astro/sql/operators/upstream_task_mixin.py
--rw-r--r--   0        0        0      160 2023-04-21 19:05:11.635546 astro-sdk-python-1.6.0a1/src/astro/sql/table.py
--rw-r--r--   0        0        0     8098 2023-04-21 19:05:11.635546 astro-sdk-python-1.6.0a1/src/astro/table.py
--rw-r--r--   0        0        0        0 2023-04-21 19:05:11.635546 astro-sdk-python-1.6.0a1/src/astro/utils/__init__.py
--rw-r--r--   0        0        0        0 2023-04-21 19:05:11.635546 astro-sdk-python-1.6.0a1/src/astro/utils/compat/__init__.py
--rw-r--r--   0        0        0      359 2023-04-21 19:05:11.635546 astro-sdk-python-1.6.0a1/src/astro/utils/compat/functools.py
--rw-r--r--   0        0        0      843 2023-04-21 19:05:11.635546 astro-sdk-python-1.6.0a1/src/astro/utils/compat/typing.py
--rw-r--r--   0        0        0     2022 2023-04-21 19:05:11.635546 astro-sdk-python-1.6.0a1/src/astro/utils/dataframe.py
--rw-r--r--   0        0        0     1581 2023-04-21 19:05:11.635546 astro-sdk-python-1.6.0a1/src/astro/utils/load.py
--rw-r--r--   0        0        0     2790 2023-04-21 19:05:11.635546 astro-sdk-python-1.6.0a1/src/astro/utils/path.py
--rw-r--r--   0        0        0     4025 2023-04-21 19:05:11.635546 astro-sdk-python-1.6.0a1/src/astro/utils/table.py
--rw-r--r--   0        0        0    13316 1970-01-01 00:00:00.000000 astro-sdk-python-1.6.0a1/PKG-INFO
+lrwxr-xr-x   0        0        0        0 2023-05-05 14:23:07.796431 astro-sdk-python-1.7.0a1/LICENSE -> ../LICENSE
+-rw-r--r--   0        0        0     8344 2023-05-05 14:23:07.796431 astro-sdk-python-1.7.0a1/README.md
+-rw-r--r--   0        0        0     5401 2023-05-05 14:23:07.808431 astro-sdk-python-1.7.0a1/pyproject.toml
+-rw-r--r--   0        0        0      687 2023-05-05 14:23:07.808431 astro-sdk-python-1.7.0a1/src/astro/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-05 14:23:07.808431 astro-sdk-python-1.7.0a1/src/astro/airflow/__init__.py
+-rw-r--r--   0        0        0     1605 2023-05-05 14:23:07.808431 astro-sdk-python-1.7.0a1/src/astro/airflow/datasets.py
+-rw-r--r--   0        0        0     2256 2023-05-05 14:23:07.808431 astro-sdk-python-1.7.0a1/src/astro/constants.py
+-rw-r--r--   0        0        0        0 2023-05-05 14:23:07.808431 astro-sdk-python-1.7.0a1/src/astro/custom_backend/__init__.py
+-rw-r--r--   0        0        0     2187 2023-05-05 14:23:07.808431 astro-sdk-python-1.7.0a1/src/astro/custom_backend/astro_custom_backend.py
+-rw-r--r--   0        0        0     3915 2023-05-05 14:23:07.808431 astro-sdk-python-1.7.0a1/src/astro/custom_backend/serializer.py
+-rw-r--r--   0        0        0     1876 2023-05-05 14:23:07.808431 astro-sdk-python-1.7.0a1/src/astro/databases/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-05 14:23:07.808431 astro-sdk-python-1.7.0a1/src/astro/databases/aws/__init__.py
+-rw-r--r--   0        0        0    18189 2023-05-05 14:23:07.808431 astro-sdk-python-1.7.0a1/src/astro/databases/aws/redshift.py
+-rw-r--r--   0        0        0    37369 2023-05-05 14:23:07.808431 astro-sdk-python-1.7.0a1/src/astro/databases/base.py
+-rw-r--r--   0        0        0        0 2023-05-05 14:23:07.808431 astro-sdk-python-1.7.0a1/src/astro/databases/databricks/__init__.py
+-rw-r--r--   0        0        0     7247 2023-05-05 14:23:07.808431 astro-sdk-python-1.7.0a1/src/astro/databases/databricks/api_utils.py
+-rw-r--r--   0        0        0    18097 2023-05-05 14:23:07.808431 astro-sdk-python-1.7.0a1/src/astro/databases/databricks/delta.py
+-rw-r--r--   0        0        0        0 2023-05-05 14:23:07.808431 astro-sdk-python-1.7.0a1/src/astro/databases/databricks/load_file/__init__.py
+-rw-r--r--   0        0        0      720 2023-05-05 14:23:07.808431 astro-sdk-python-1.7.0a1/src/astro/databases/databricks/load_file/jinja_templates/autoloader.py.jinja2
+-rw-r--r--   0        0        0      647 2023-05-05 14:23:07.808431 astro-sdk-python-1.7.0a1/src/astro/databases/databricks/load_file/jinja_templates/copy_into.py.jinja2
+-rw-r--r--   0        0        0      913 2023-05-05 14:23:07.808431 astro-sdk-python-1.7.0a1/src/astro/databases/databricks/load_file/jinja_templates/load_file_to_delta.py.jinja2
+-rw-r--r--   0        0        0      512 2023-05-05 14:23:07.808431 astro-sdk-python-1.7.0a1/src/astro/databases/databricks/load_file/jinja_templates/load_secrets.py.jinja2
+-rw-r--r--   0        0        0     6368 2023-05-05 14:23:07.808431 astro-sdk-python-1.7.0a1/src/astro/databases/databricks/load_file/load_file_job.py
+-rw-r--r--   0        0        0      880 2023-05-05 14:23:07.808431 astro-sdk-python-1.7.0a1/src/astro/databases/databricks/load_file/load_file_python_code_generator.py
+-rw-r--r--   0        0        0     2687 2023-05-05 14:23:07.808431 astro-sdk-python-1.7.0a1/src/astro/databases/databricks/load_options.py
+-rw-r--r--   0        0        0     6181 2023-05-05 14:23:07.808431 astro-sdk-python-1.7.0a1/src/astro/databases/duckdb.py
+-rw-r--r--   0        0        0        0 2023-05-05 14:23:07.808431 astro-sdk-python-1.7.0a1/src/astro/databases/google/__init__.py
+-rw-r--r--   0        0        0    26823 2023-05-05 14:23:07.808431 astro-sdk-python-1.7.0a1/src/astro/databases/google/bigquery.py
+-rw-r--r--   0        0        0    17049 2023-05-05 14:23:07.808431 astro-sdk-python-1.7.0a1/src/astro/databases/mssql.py
+-rw-r--r--   0        0        0     9267 2023-05-05 14:23:07.808431 astro-sdk-python-1.7.0a1/src/astro/databases/mysql.py
+-rw-r--r--   0        0        0    10678 2023-05-05 14:23:07.808431 astro-sdk-python-1.7.0a1/src/astro/databases/postgres.py
+-rw-r--r--   0        0        0    42201 2023-05-05 14:23:07.808431 astro-sdk-python-1.7.0a1/src/astro/databases/snowflake.py
+-rw-r--r--   0        0        0     6508 2023-05-05 14:23:07.808431 astro-sdk-python-1.7.0a1/src/astro/databases/sqlite.py
+-rw-r--r--   0        0        0        0 2023-05-05 14:23:07.808431 astro-sdk-python-1.7.0a1/src/astro/dataframes/__init__.py
+-rw-r--r--   0        0        0     4116 2023-05-05 14:23:07.808431 astro-sdk-python-1.7.0a1/src/astro/dataframes/load_options.py
+-rw-r--r--   0        0        0     2356 2023-05-05 14:23:07.808431 astro-sdk-python-1.7.0a1/src/astro/dataframes/pandas.py
+-rw-r--r--   0        0        0     1267 2023-05-05 14:23:07.808431 astro-sdk-python-1.7.0a1/src/astro/exceptions.py
+-rw-r--r--   0        0        0     1096 2023-05-05 14:23:07.808431 astro-sdk-python-1.7.0a1/src/astro/files/__init__.py
+-rw-r--r--   0        0        0    10151 2023-05-05 14:23:07.808431 astro-sdk-python-1.7.0a1/src/astro/files/base.py
+-rw-r--r--   0        0        0     1535 2023-05-05 14:23:07.808431 astro-sdk-python-1.7.0a1/src/astro/files/locations/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-05 14:23:07.812431 astro-sdk-python-1.7.0a1/src/astro/files/locations/amazon/__init__.py
+-rw-r--r--   0        0        0     3605 2023-05-05 14:23:07.812431 astro-sdk-python-1.7.0a1/src/astro/files/locations/amazon/s3.py
+-rw-r--r--   0        0        0        0 2023-05-05 14:23:07.812431 astro-sdk-python-1.7.0a1/src/astro/files/locations/azure/__init__.py
+-rw-r--r--   0        0        0     5867 2023-05-05 14:23:07.812431 astro-sdk-python-1.7.0a1/src/astro/files/locations/azure/wasb.py
+-rw-r--r--   0        0        0     6601 2023-05-05 14:23:07.812431 astro-sdk-python-1.7.0a1/src/astro/files/locations/base.py
+-rw-r--r--   0        0        0     2374 2023-05-05 14:23:07.812431 astro-sdk-python-1.7.0a1/src/astro/files/locations/ftp.py
+-rw-r--r--   0        0        0        0 2023-05-05 14:23:07.812431 astro-sdk-python-1.7.0a1/src/astro/files/locations/google/__init__.py
+-rw-r--r--   0        0        0     4420 2023-05-05 14:23:07.812431 astro-sdk-python-1.7.0a1/src/astro/files/locations/google/gcs.py
+-rw-r--r--   0        0        0     5006 2023-05-05 14:23:07.812431 astro-sdk-python-1.7.0a1/src/astro/files/locations/google/gdrive.py
+-rw-r--r--   0        0        0     1303 2023-05-05 14:23:07.812431 astro-sdk-python-1.7.0a1/src/astro/files/locations/http.py
+-rw-r--r--   0        0        0     1531 2023-05-05 14:23:07.812431 astro-sdk-python-1.7.0a1/src/astro/files/locations/local.py
+-rw-r--r--   0        0        0     3267 2023-05-05 14:23:07.812431 astro-sdk-python-1.7.0a1/src/astro/files/locations/sftp.py
+-rw-r--r--   0        0        0        0 2023-05-05 14:23:07.812431 astro-sdk-python-1.7.0a1/src/astro/files/operators/__init__.py
+-rw-r--r--   0        0        0     1595 2023-05-05 14:23:07.812431 astro-sdk-python-1.7.0a1/src/astro/files/operators/files.py
+-rw-r--r--   0        0        0     2576 2023-05-05 14:23:07.812431 astro-sdk-python-1.7.0a1/src/astro/files/types/__init__.py
+-rw-r--r--   0        0        0     1504 2023-05-05 14:23:07.812431 astro-sdk-python-1.7.0a1/src/astro/files/types/base.py
+-rw-r--r--   0        0        0     1900 2023-05-05 14:23:07.812431 astro-sdk-python-1.7.0a1/src/astro/files/types/csv.py
+-rw-r--r--   0        0        0     2197 2023-05-05 14:23:07.812431 astro-sdk-python-1.7.0a1/src/astro/files/types/json.py
+-rw-r--r--   0        0        0     3652 2023-05-05 14:23:07.812431 astro-sdk-python-1.7.0a1/src/astro/files/types/ndjson.py
+-rw-r--r--   0        0        0     2848 2023-05-05 14:23:07.812431 astro-sdk-python-1.7.0a1/src/astro/files/types/parquet.py
+-rw-r--r--   0        0        0      700 2023-05-05 14:23:07.812431 astro-sdk-python-1.7.0a1/src/astro/lineage/__init__.py
+-rw-r--r--   0        0        0     4264 2023-05-05 14:23:07.812431 astro-sdk-python-1.7.0a1/src/astro/lineage/facets.py
+-rw-r--r--   0        0        0     3910 2023-05-05 14:23:07.812431 astro-sdk-python-1.7.0a1/src/astro/options.py
+-rw-r--r--   0        0        0     1117 2023-05-05 14:23:07.812431 astro-sdk-python-1.7.0a1/src/astro/query_modifier.py
+-rw-r--r--   0        0        0     4168 2023-05-05 14:23:07.812431 astro-sdk-python-1.7.0a1/src/astro/settings.py
+-rw-r--r--   0        0        0     3194 2023-05-05 14:23:07.812431 astro-sdk-python-1.7.0a1/src/astro/sql/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-05 14:23:07.812431 astro-sdk-python-1.7.0a1/src/astro/sql/operators/__init__.py
+-rw-r--r--   0        0        0     7857 2023-05-05 14:23:07.812431 astro-sdk-python-1.7.0a1/src/astro/sql/operators/append.py
+-rw-r--r--   0        0        0    18419 2023-05-05 14:23:07.812431 astro-sdk-python-1.7.0a1/src/astro/sql/operators/base_decorator.py
+-rw-r--r--   0        0        0      334 2023-05-05 14:23:07.812431 astro-sdk-python-1.7.0a1/src/astro/sql/operators/base_operator.py
+-rw-r--r--   0        0        0    12688 2023-05-05 14:23:07.812431 astro-sdk-python-1.7.0a1/src/astro/sql/operators/cleanup.py
+-rw-r--r--   0        0        0     7870 2023-05-05 14:23:07.812431 astro-sdk-python-1.7.0a1/src/astro/sql/operators/data_validations/check_column.py
+-rw-r--r--   0        0        0     3696 2023-05-05 14:23:07.812431 astro-sdk-python-1.7.0a1/src/astro/sql/operators/data_validations/check_table.py
+-rw-r--r--   0        0        0    15362 2023-05-05 14:23:07.812431 astro-sdk-python-1.7.0a1/src/astro/sql/operators/dataframe.py
+-rw-r--r--   0        0        0     1435 2023-05-05 14:23:07.812431 astro-sdk-python-1.7.0a1/src/astro/sql/operators/drop.py
+-rw-r--r--   0        0        0     2693 2023-05-05 14:23:07.812431 astro-sdk-python-1.7.0a1/src/astro/sql/operators/export_file.py
+-rw-r--r--   0        0        0     2715 2023-05-05 14:23:07.812431 astro-sdk-python-1.7.0a1/src/astro/sql/operators/export_table_to_file.py
+-rw-r--r--   0        0        0     7035 2023-05-05 14:23:07.812431 astro-sdk-python-1.7.0a1/src/astro/sql/operators/export_to_file.py
+-rw-r--r--   0        0        0    17519 2023-05-05 14:23:07.812431 astro-sdk-python-1.7.0a1/src/astro/sql/operators/load_file.py
+-rw-r--r--   0        0        0     8824 2023-05-05 14:23:07.812431 astro-sdk-python-1.7.0a1/src/astro/sql/operators/merge.py
+-rw-r--r--   0        0        0     9898 2023-05-05 14:23:07.812431 astro-sdk-python-1.7.0a1/src/astro/sql/operators/raw_sql.py
+-rw-r--r--   0        0        0     7393 2023-05-05 14:23:07.812431 astro-sdk-python-1.7.0a1/src/astro/sql/operators/transform.py
+-rw-r--r--   0        0        0      880 2023-05-05 14:23:07.812431 astro-sdk-python-1.7.0a1/src/astro/sql/operators/upstream_task_mixin.py
+-rw-r--r--   0        0        0      160 2023-05-05 14:23:07.812431 astro-sdk-python-1.7.0a1/src/astro/sql/table.py
+-rw-r--r--   0        0        0     8747 2023-05-05 14:23:07.812431 astro-sdk-python-1.7.0a1/src/astro/table.py
+-rw-r--r--   0        0        0        0 2023-05-05 14:23:07.812431 astro-sdk-python-1.7.0a1/src/astro/utils/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-05 14:23:07.812431 astro-sdk-python-1.7.0a1/src/astro/utils/compat/__init__.py
+-rw-r--r--   0        0        0      359 2023-05-05 14:23:07.812431 astro-sdk-python-1.7.0a1/src/astro/utils/compat/functools.py
+-rw-r--r--   0        0        0      843 2023-05-05 14:23:07.812431 astro-sdk-python-1.7.0a1/src/astro/utils/compat/typing.py
+-rw-r--r--   0        0        0     2022 2023-05-05 14:23:07.812431 astro-sdk-python-1.7.0a1/src/astro/utils/dataframe.py
+-rw-r--r--   0        0        0     1581 2023-05-05 14:23:07.812431 astro-sdk-python-1.7.0a1/src/astro/utils/load.py
+-rw-r--r--   0        0        0     2790 2023-05-05 14:23:07.812431 astro-sdk-python-1.7.0a1/src/astro/utils/path.py
+-rw-r--r--   0        0        0     4025 2023-05-05 14:23:07.812431 astro-sdk-python-1.7.0a1/src/astro/utils/table.py
+-rw-r--r--   0        0        0    13466 1970-01-01 00:00:00.000000 astro-sdk-python-1.7.0a1/PKG-INFO
```

### Comparing `astro-sdk-python-1.6.0a1/README.md` & `astro-sdk-python-1.7.0a1/README.md`

 * *Files identical despite different names*

### Comparing `astro-sdk-python-1.6.0a1/pyproject.toml` & `astro-sdk-python-1.7.0a1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -94,14 +94,18 @@
 databricks = ["databricks-cli",
     "apache-airflow-providers-databricks"]
 
 mssql = [
     "apache-airflow-providers-microsoft-mssql>=3.2",
 ]
 
+mysql = [
+    "apache-airflow-providers-mysql",
+]
+
 duckdb = [
     "airflow-provider-duckdb>=0.0.2",
 ]
 
 all = [
     "apache-airflow-providers-amazon",
     "apache-airflow-providers-google>=6.4.0",
@@ -121,14 +125,15 @@
     "s3fs",
     "protobuf<=3.20", # Google bigquery client require protobuf <= 3.20.0. We can remove the limitation when this limitation is removed
     "openlineage-airflow>=0.17.0",
     "apache-airflow-providers-microsoft-azure",
     "azure-storage-blob",
     "apache-airflow-providers-microsoft-mssql>=3.2",
     "airflow-provider-duckdb>=0.0.2",
+    "apache-airflow-providers-mysql"
 ]
 doc = [
     "myst-parser>=0.17",
     "sphinx>=4.4.0",
     "sphinx-autoapi==2.0.0", # Multiple FileType class (same name) import is broken in sphinx-autoapi 2.0.1
     "sphinx-rtd-theme"
 ]
```

### Comparing `astro-sdk-python-1.6.0a1/src/astro/__init__.py` & `astro-sdk-python-1.7.0a1/src/astro/__init__.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 """A decorator that allows users to run SQL queries natively in Airflow."""
 
-__version__ = "1.6.0a1"
+__version__ = "1.7.0a1"
 
 
 # This is needed to allow Airflow to pick up specific metadata fields it needs
 # for certain features. We recognize it's a bit unclean to define these in
 # multiple places, but at this point it's the only workaround if you'd like
 # your custom conn type to show up in the Airflow UI.
 def get_provider_info() -> dict:
```

### Comparing `astro-sdk-python-1.6.0a1/src/astro/airflow/datasets.py` & `astro-sdk-python-1.7.0a1/src/astro/airflow/datasets.py`

 * *Files identical despite different names*

### Comparing `astro-sdk-python-1.6.0a1/src/astro/constants.py` & `astro-sdk-python-1.7.0a1/src/astro/constants.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from __future__ import annotations
 
 import sys
 from enum import Enum
 
 # typing.Literal was only introduced in Python 3.8, and we support Python 3.7
 if sys.version_info >= (3, 8):
-    from typing import Literal
+    from typing import Any, Literal
 else:
     from typing_extensions import Literal
 
 DEFAULT_SCHEMA = "tmp_astro"
 DEFAULT_CHUNK_SIZE = 1000000
 PYPI_PROJECT_NAME = "astro-sdk-python"
 
@@ -40,26 +40,36 @@
     NDJSON = "ndjson"
     PARQUET = "parquet"
     # [END filetypes]
 
     def __str__(self) -> str:
         return self.value
 
+    def serialize(self) -> dict[str, Any]:
+        return {
+            "value": self.value,
+        }
+
+    @staticmethod
+    def deserialize(data: dict[str, Any], _: int):
+        return FileType(data["value"])
+
 
 class Database(Enum):
     # [START database]
     POSTGRES = "postgres"
     POSTGRESQL = "postgres"
     SQLITE = "sqlite"
     DELTA = "delta"
     BIGQUERY = "bigquery"
     SNOWFLAKE = "snowflake"
     REDSHIFT = "redshift"
     MSSQL = "mssql"
     DUCKDB = "duckdb"
+    MYSQL = "mysql"
     # [END database]
 
     def __str__(self) -> str:
         return self.value
 
 
 class DatabricksLoadMode(str, Enum):
```

### Comparing `astro-sdk-python-1.6.0a1/src/astro/custom_backend/astro_custom_backend.py` & `astro-sdk-python-1.7.0a1/src/astro/custom_backend/astro_custom_backend.py`

 * *Files identical despite different names*

### Comparing `astro-sdk-python-1.6.0a1/src/astro/custom_backend/serializer.py` & `astro-sdk-python-1.7.0a1/src/astro/custom_backend/serializer.py`

 * *Files identical despite different names*

### Comparing `astro-sdk-python-1.6.0a1/src/astro/databases/__init__.py` & `astro-sdk-python-1.7.0a1/src/astro/databases/__init__.py`

 * *Files identical despite different names*

### Comparing `astro-sdk-python-1.6.0a1/src/astro/databases/aws/redshift.py` & `astro-sdk-python-1.7.0a1/src/astro/databases/aws/redshift.py`

 * *Files identical despite different names*

### Comparing `astro-sdk-python-1.6.0a1/src/astro/databases/base.py` & `astro-sdk-python-1.7.0a1/src/astro/databases/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -26,15 +26,20 @@
 from astro.dataframes.pandas import PandasDataframe
 from astro.exceptions import DatabaseCustomError, NonExistentTableException
 from astro.files import File, resolve_file_path_pattern
 from astro.files.types import create_file_type
 from astro.files.types.base import FileType as FileTypeConstants
 from astro.options import LoadOptions
 from astro.query_modifier import QueryModifier
-from astro.settings import LOAD_FILE_ENABLE_NATIVE_FALLBACK, LOAD_TABLE_AUTODETECT_ROWS_COUNT, SCHEMA
+from astro.settings import (
+    LOAD_FILE_ENABLE_NATIVE_FALLBACK,
+    LOAD_TABLE_AUTODETECT_ROWS_COUNT,
+    LOAD_TABLE_SCHEMA_EXISTS,
+    SCHEMA,
+)
 from astro.table import BaseTable, Metadata
 from astro.utils.compat.functools import cached_property
 
 
 class BaseDatabase(ABC):
     """
     Base class to represent all the Database interactions.
@@ -355,15 +360,15 @@
         statement = self._drop_table_statement.format(self.get_table_qualified_name(table))
         self.run_sql(statement)
 
     # ---------------------------------------------------------
     # Table load methods
     # ---------------------------------------------------------
 
-    def create_schema_and_table_if_needed(
+    def create_table_if_needed(
         self,
         table: BaseTable,
         file: File,
         normalize_config: dict | None = None,
         columns_names_capitalization: ColumnCapitalization = "original",
         if_exists: LoadExistStrategy = "replace",
         use_native_support: bool = True,
@@ -389,15 +394,14 @@
             use_native_support
             and file.is_pattern()
             and is_schema_autodetection_supported
             and is_file_pattern_based_schema_autodetection_supported
         ):
             return
 
-        self.create_schema_if_needed(table.metadata.schema)
         if if_exists == "replace" or not self.table_exists(table):
             files = resolve_file_path_pattern(
                 file.path,
                 file.conn_id,
                 normalize_config=normalize_config,
                 filetype=file.type.name,
                 load_options=file.load_options,
@@ -445,14 +449,15 @@
         normalize_config: dict | None = None,
         if_exists: LoadExistStrategy = "replace",
         chunk_size: int = DEFAULT_CHUNK_SIZE,
         use_native_support: bool = True,
         native_support_kwargs: dict | None = None,
         columns_names_capitalization: ColumnCapitalization = "original",
         enable_native_fallback: bool | None = LOAD_FILE_ENABLE_NATIVE_FALLBACK,
+        schema_exists: bool = LOAD_TABLE_SCHEMA_EXISTS,
         **kwargs,
     ):
         """
         Load content of multiple files in output_table.
         Multiple files are sourced from the file path, which can also be path pattern.
 
         :param input_file: File path and conn_id for object stores
@@ -461,24 +466,28 @@
         :param chunk_size: Specify the number of records in each batch to be written at a time
         :param use_native_support: Use native support for data transfer if available on the destination
         :param normalize_config: pandas json_normalize params config
         :param native_support_kwargs: kwargs to be used by method involved in native support flow
         :param columns_names_capitalization: determines whether to convert all columns to lowercase/uppercase
             in the resulting dataframe
         :param enable_native_fallback: Use enable_native_fallback=True to fall back to default transfer
+        :param schema_exists: Declare the table schema already exists and that load_file should not check if it exists
         """
         normalize_config = normalize_config or {}
         if self.check_for_minio_connection(input_file=input_file):
             logging.info(
                 "No native support available for the service provided via endpoint_url! Setting use_native_support"
                 " to False."
             )
             use_native_support = False
 
-        self.create_schema_and_table_if_needed(
+        if not schema_exists:
+            self.create_schema_if_needed(output_table.metadata.schema)
+
+        self.create_table_if_needed(
             file=input_file,
             table=output_table,
             columns_names_capitalization=columns_names_capitalization,
             if_exists=if_exists,
             normalize_config=normalize_config,
             use_native_support=use_native_support,
         )
```

### Comparing `astro-sdk-python-1.6.0a1/src/astro/databases/databricks/api_utils.py` & `astro-sdk-python-1.7.0a1/src/astro/databases/databricks/api_utils.py`

 * *Files identical despite different names*

### Comparing `astro-sdk-python-1.6.0a1/src/astro/databases/databricks/delta.py` & `astro-sdk-python-1.7.0a1/src/astro/databases/databricks/delta.py`

 * *Files 2% similar despite different names*

```diff
@@ -18,14 +18,15 @@
 from astro.databases.base import BaseDatabase
 from astro.databases.databricks.load_file.load_file_job import load_file_to_delta
 from astro.databases.databricks.load_options import DeltaLoadOptions
 from astro.dataframes.pandas import PandasDataframe
 from astro.files import File
 from astro.options import LoadOptions
 from astro.query_modifier import QueryModifier
+from astro.settings import LOAD_TABLE_SCHEMA_EXISTS
 from astro.table import BaseTable, Metadata
 
 
 class DeltaDatabase(BaseDatabase):
     LOAD_OPTIONS_CLASS_NAME = ("DeltaLoadOptions",)
     _create_table_statement: str = "CREATE TABLE IF NOT EXISTS {} USING DELTA AS {} "
 
@@ -119,14 +120,15 @@
         normalize_config: dict | None = None,
         if_exists: LoadExistStrategy = "replace",
         chunk_size: int = DEFAULT_CHUNK_SIZE,
         use_native_support: bool = True,
         native_support_kwargs: dict | None = None,
         columns_names_capitalization: ColumnCapitalization = "original",
         enable_native_fallback: bool | None = None,
+        schema_exists: bool = LOAD_TABLE_SCHEMA_EXISTS,
         databricks_job_name: str = "",
         **kwargs,
     ):
         """
         Load content of multiple files in output_table.
         Multiple files are sourced from the file path, which can also be path pattern.
 
@@ -138,15 +140,15 @@
         :param chunk_size: Specify the number of records in each batch to be written at a time
         :param use_native_support: Use native support for data transfer if available on the destination
         :param normalize_config: pandas json_normalize params config
         :param native_support_kwargs: kwargs to be used by method involved in native support flow
         :param columns_names_capitalization: determines whether to convert all columns to lowercase/uppercase
             in the resulting dataframe
         :param enable_native_fallback: Use enable_native_fallback=True to fall back to default transfer
-
+        :param schema_exists: Declare the table schema already exists and that load_file should not check if it exists
         """
         load_file_to_delta(
             input_file=input_file,
             delta_table=output_table,
             databricks_job_name=databricks_job_name,
             delta_load_options=self.load_options,  # type: ignore
             if_exists=if_exists,
@@ -154,14 +156,17 @@
 
     def openlineage_dataset_name(self, table: BaseTable) -> str:
         return ""
 
     def openlineage_dataset_namespace(self) -> str:
         return ""
 
+    def openlineage_dataset_uri(self, table: BaseTable) -> str:
+        return ""
+
     def create_table_from_select_statement(
         self,
         statement: str,
         target_table: BaseTable,
         parameters: dict | None = None,
         query_modifier=QueryModifier(),
     ) -> None:
```

### Comparing `astro-sdk-python-1.6.0a1/src/astro/databases/databricks/load_file/jinja_templates/autoloader.py.jinja2` & `astro-sdk-python-1.7.0a1/src/astro/databases/databricks/load_file/jinja_templates/autoloader.py.jinja2`

 * *Files identical despite different names*

### Comparing `astro-sdk-python-1.6.0a1/src/astro/databases/databricks/load_file/jinja_templates/copy_into.py.jinja2` & `astro-sdk-python-1.7.0a1/src/astro/databases/databricks/load_file/jinja_templates/copy_into.py.jinja2`

 * *Files identical despite different names*

### Comparing `astro-sdk-python-1.6.0a1/src/astro/databases/databricks/load_file/jinja_templates/load_file_to_delta.py.jinja2` & `astro-sdk-python-1.7.0a1/src/astro/databases/databricks/load_file/jinja_templates/load_file_to_delta.py.jinja2`

 * *Files identical despite different names*

### Comparing `astro-sdk-python-1.6.0a1/src/astro/databases/databricks/load_file/jinja_templates/load_secrets.py.jinja2` & `astro-sdk-python-1.7.0a1/src/astro/databases/databricks/load_file/jinja_templates/load_secrets.py.jinja2`

 * *Files identical despite different names*

### Comparing `astro-sdk-python-1.6.0a1/src/astro/databases/databricks/load_file/load_file_job.py` & `astro-sdk-python-1.7.0a1/src/astro/databases/databricks/load_file/load_file_job.py`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,21 @@
 )
 from astro.databases.databricks.load_options import DeltaLoadOptions
 from astro.files import File
 from astro.table import BaseTable
 
 cwd = pathlib.Path(__file__).parent
 
-supported_file_locations = [FileLocation.LOCAL, FileLocation.S3, FileLocation.GS]
+supported_file_locations = [
+    FileLocation.LOCAL,
+    FileLocation.S3,
+    FileLocation.GS,
+    FileLocation.WASB,
+    FileLocation.WASBS,
+]
 
 log = logging.getLogger(__file__)
 
 
 def load_file_to_delta(  # noqa: C901
     input_file: File,
     delta_table: BaseTable,
@@ -105,15 +111,15 @@
     if (
         databricks_options.load_mode == DatabricksLoadMode.AUTOLOADER
         and databricks_options.if_exists == "replace"
     ):
         databricks_options.autoloader_load_options["cloudFiles.allowOverwrites"] = "true"
 
     file_path = generate_file(
-        data_source_path=str(dbfs_file_path) if dbfs_file_path else input_file.path,
+        data_source_path=str(dbfs_file_path) if dbfs_file_path else input_file.location.databricks_uri,
         table_name=delta_table.name,
         source_type=str(input_file.location.location_type),
         output_file_path=Path(output_file.name),
         file_type=file_type or "",
         load_options=databricks_options,
     )
     dbfs_file_path = load_file_to_dbfs(
```

### Comparing `astro-sdk-python-1.6.0a1/src/astro/databases/databricks/load_file/load_file_python_code_generator.py` & `astro-sdk-python-1.7.0a1/src/astro/databases/databricks/load_file/load_file_python_code_generator.py`

 * *Files identical despite different names*

### Comparing `astro-sdk-python-1.6.0a1/src/astro/databases/databricks/load_options.py` & `astro-sdk-python-1.7.0a1/src/astro/databases/databricks/load_options.py`

 * *Files identical despite different names*

### Comparing `astro-sdk-python-1.6.0a1/src/astro/databases/duckdb.py` & `astro-sdk-python-1.7.0a1/src/astro/databases/duckdb.py`

 * *Files identical despite different names*

### Comparing `astro-sdk-python-1.6.0a1/src/astro/databases/google/bigquery.py` & `astro-sdk-python-1.7.0a1/src/astro/databases/google/bigquery.py`

 * *Files identical despite different names*

### Comparing `astro-sdk-python-1.6.0a1/src/astro/databases/mssql.py` & `astro-sdk-python-1.7.0a1/src/astro/databases/mssql.py`

 * *Files identical despite different names*

### Comparing `astro-sdk-python-1.6.0a1/src/astro/databases/postgres.py` & `astro-sdk-python-1.7.0a1/src/astro/databases/postgres.py`

 * *Files identical despite different names*

### Comparing `astro-sdk-python-1.6.0a1/src/astro/databases/snowflake.py` & `astro-sdk-python-1.7.0a1/src/astro/databases/snowflake.py`

 * *Files identical despite different names*

### Comparing `astro-sdk-python-1.6.0a1/src/astro/databases/sqlite.py` & `astro-sdk-python-1.7.0a1/src/astro/databases/sqlite.py`

 * *Files identical despite different names*

### Comparing `astro-sdk-python-1.6.0a1/src/astro/dataframes/load_options.py` & `astro-sdk-python-1.7.0a1/src/astro/dataframes/load_options.py`

 * *Files identical despite different names*

### Comparing `astro-sdk-python-1.6.0a1/src/astro/dataframes/pandas.py` & `astro-sdk-python-1.7.0a1/src/astro/dataframes/pandas.py`

 * *Files 21% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 
 import logging
 from typing import ClassVar
 
 from pandas import DataFrame, read_json
 
 from astro import settings
+from astro.exceptions import AstroSDKConfigError
 
 logger = logging.getLogger(__name__)
 
 
 class PandasDataframe(DataFrame):
     """Pandas-compatible dataframe class that can be serialized and deserialized into XCom by Airflow 2.5"""
 
@@ -17,26 +18,32 @@
 
     def serialize(self):
         # Store in the metadata DB if Dataframe < 100 kb
         df_size = self.memory_usage(deep=True).sum()
         if df_size < (settings.MAX_DATAFRAME_MEMORY_FOR_XCOM_DB * 1024):
             logger.info("Dataframe size: %s bytes. Storing it in Airflow's metadata DB", df_size)
             return {"data": self.to_json()}
-        else:
+        elif settings.DATAFRAME_STORAGE_CONN_ID is not None:
             # Avoid cyclic dependency
             from astro.utils.dataframe import convert_dataframe_to_file
 
             logger.info(
                 "Dataframe size: %s bytes. Storing it in Remote Storage (conn_id: %s | URL: %s)",
                 df_size,
                 settings.DATAFRAME_STORAGE_CONN_ID,
                 settings.DATAFRAME_STORAGE_URL,
             )
             return convert_dataframe_to_file(self).to_json()
 
+        raise AstroSDKConfigError(
+            "Dataframe size exceeds allowed limit for storing in Airflow's metadata DB. "
+            "Airflow config variable AIRFLOW__ASTRO_SDK__XCOM_STORAGE_CONN_ID needs to "
+            "be set for remote storage of the dataframe."
+        )
+
     @staticmethod
     def deserialize(data: dict, version: int):
         if version > 1:
             raise TypeError(f"version > {PandasDataframe.version}")
         if isinstance(data, dict) and data.get("class", "") == "File":
             # Avoid cyclic dependency
             from astro.files import File
```

### Comparing `astro-sdk-python-1.6.0a1/src/astro/exceptions.py` & `astro-sdk-python-1.7.0a1/src/astro/exceptions.py`

 * *Files 9% similar despite different names*

```diff
@@ -20,7 +20,11 @@
     Inappropriate argument value (of correct type) or attribute
     not found while running query. while running query
     """
 
 
 class PermissionNotSetError(Exception):
     """Raised if a permission to files present in locations are not accessible"""
+
+
+class AstroSDKConfigError(Exception):
+    """Raised if a configuration parameter required for Astro SDK is not set correctly"""
```

### Comparing `astro-sdk-python-1.6.0a1/src/astro/files/__init__.py` & `astro-sdk-python-1.7.0a1/src/astro/files/__init__.py`

 * *Files identical despite different names*

### Comparing `astro-sdk-python-1.6.0a1/src/astro/files/base.py` & `astro-sdk-python-1.7.0a1/src/astro/files/base.py`

 * *Files identical despite different names*

### Comparing `astro-sdk-python-1.6.0a1/src/astro/files/locations/__init__.py` & `astro-sdk-python-1.7.0a1/src/astro/files/locations/__init__.py`

 * *Files identical despite different names*

### Comparing `astro-sdk-python-1.6.0a1/src/astro/files/locations/amazon/s3.py` & `astro-sdk-python-1.7.0a1/src/astro/files/locations/amazon/s3.py`

 * *Files identical despite different names*

### Comparing `astro-sdk-python-1.6.0a1/src/astro/files/locations/azure/wasb.py` & `astro-sdk-python-1.7.0a1/src/astro/files/locations/sftp.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,84 +1,66 @@
 from __future__ import annotations
 
-from urllib.parse import urlparse, urlunparse
+import io
+from contextlib import contextmanager
+from urllib.parse import urlparse
 
-import smart_open
-from airflow.providers.microsoft.azure.hooks.wasb import WasbHook
-from azure.core.exceptions import ResourceNotFoundError
+from airflow.providers.sftp.hooks.sftp import SFTPHook
 
 from astro.constants import FileLocation
+from astro.exceptions import PermissionNotSetError
 from astro.files.locations.base import BaseFileLocation
-from astro.options import contains_required_option
 
 
-class WASBLocation(BaseFileLocation):
-    """Handler WASB object store operations"""
+class SFTPLocation(BaseFileLocation):
+    """
+    Handler SFTP object store operations.
+    While exporting to SFTP the user should have permission
+    to create the file in the desired location.
+    """
 
-    location_type = FileLocation.WASB
-    supported_conn_type = {WasbHook.conn_type, "wasbs"}
-    LOAD_OPTIONS_CLASS_NAME = ("WASBLocationLoadOptions",)
-    AZURE_HOST = "blob.core.windows.net"
-
-    def exists(self) -> bool:
-        """Check if the file exists or not"""
-        try:
-            with smart_open.open(self.smartopen_uri, mode="r", transport_params=self.transport_params):
-                return True
-        except ResourceNotFoundError:
-            return False
+    location_type = FileLocation.SFTP
+    supported_conn_type = {SFTPHook.conn_type}
 
     @property
-    def hook(self) -> WasbHook:
-        return WasbHook(wasb_conn_id=self.conn_id) if self.conn_id else WasbHook()
+    def hook(self) -> SFTPHook:
+        return SFTPHook(ssh_conn_id=self.conn_id) if self.conn_id else SFTPHook()
 
     @property
     def transport_params(self) -> dict:
-        """get WASB credentials for storage"""
-        client = self.hook.get_conn()
-        return {"client": client}
+        """Get SFTP credentials in order to access remote file system"""
+        client = self.hook.get_connection(self.conn_id)
+        extra_options = client.extra_dejson
+        if "key_file" in extra_options:
+            key_file = extra_options.get("key_file")
+            return {"connect_kwargs": {"key_filename": key_file}}
+        elif client.password:
+            return {"connect_kwargs": {"password": client.password}}
+        raise PermissionNotSetError("SFTP credentials are not set in the connection.")
 
     @property
     def paths(self) -> list[str]:
-        """Resolve WASB file paths with prefix"""
+        """Resolve SFTP file paths with prefix"""
         url = urlparse(self.path)
-        container_name = url.netloc
-        prefix = url.path[1:]
-        prefixes = self.hook.get_blobs_list(container_name=container_name, prefix=prefix)
-        paths = [urlunparse((url.scheme, url.netloc, keys, "", "", "")) for keys in prefixes]
+        uri = self.get_uri()
+        full_paths = []
+        prefixes = self.hook.get_tree_map(url.netloc, prefix=url.netloc + url.path)
+        for keys in prefixes:
+            if len(keys) > 0:
+                full_paths.extend(keys)
+        paths = [uri + "/" + path for path in full_paths]
         return paths
 
     @property
-    def smartopen_uri(self) -> str:
-        """
-        SmartOpen does not support URIs prefixed with wasb, so we need to change them to azure.
-
-        :return: URI compatible with SmartOpen for Azure BlobStorage.
-        """
-        parsed_url = urlparse(self.path)
-        if parsed_url.scheme == "wasbs":
-            return self.path.replace("wasbs", "azure")
-        elif parsed_url.scheme == "wasb":
-            return self.path.replace("wasb", "azure")
-        else:
-            return self.path
-
-    @property
     def size(self) -> int:
-        """Return file size for WASB location"""
+        """Return file size for SFTP location"""
         url = urlparse(self.path)
-        container_name = url.netloc
-        object_name = url.path
-        if object_name.startswith("/"):
-            object_name = object_name[1:]
-        return int(
-            self.hook.blob_service_client.get_blob_client(container=container_name, blob=object_name)
-            .get_blob_properties()
-            .size
-        )
+        conn = self.hook.get_conn()
+        stat = conn.stat(url.netloc + url.path).st_size
+        return int(stat) or -1
 
     @property
     def openlineage_dataset_namespace(self) -> str:
         """
         Returns the open lineage dataset namespace as per
         https://github.com/OpenLineage/OpenLineage/blob/main/spec/Naming.md
         """
@@ -89,29 +71,27 @@
     def openlineage_dataset_name(self) -> str:
         """
         Returns the open lineage dataset name as per
         https://github.com/OpenLineage/OpenLineage/blob/main/spec/Naming.md
         """
         return urlparse(self.path).path
 
-    @property
-    def snowflake_stage_path(self) -> str:
-        """
-        Get the altered path if needed for stage creation in snowflake stage creation. We need to modify the path since
-         Snowflake only accepts paths of format for stage creation:
-         "azure://<storage_account>.blob.core.windows.net/<container_name>/load/files/"
-         But SDK accepts paths
-         "wasb://<container_name>/<filename>" or "wasbs://<container_name>/<filename>"
-         To bridge the gap we use this method
-        """
-        if not contains_required_option(self.load_options, "storage_account"):
-            raise ValueError(
-                f"Required param missing 'storage_account', pass {self.LOAD_OPTIONS_CLASS_NAME[0]}"
-                f"(storage_account=<account_name>) to load_options"
-            )
-        url = urlparse(self.path)
-        url = url._replace(
-            scheme=str(FileLocation.AZURE),
-            path=f"{url.netloc}/",
-            netloc=f"{self.load_options.storage_account}.{self.AZURE_HOST}",  # type: ignore
-        )
-        return url.geturl()
+    def get_uri(self):
+        client = self.hook.get_connection(self.conn_id)
+        return client.get_uri()
+
+    def get_stream(self):
+        """return the custom SFTP read_buffer context to add file into given path"""
+        return self.sftp_stream()
+
+    @contextmanager
+    def sftp_stream(self):
+        """sftp_stream context to export a file to the given location."""
+        buffer = io.BytesIO()
+        try:
+            yield buffer
+        finally:
+            buffer.seek(0)
+            sftp = self.hook.get_conn()
+            parsed_url = urlparse(self.path)
+            sftp.putfo(buffer, parsed_url.netloc + parsed_url.path)
+            buffer.close()
```

### Comparing `astro-sdk-python-1.6.0a1/src/astro/files/locations/base.py` & `astro-sdk-python-1.7.0a1/src/astro/files/locations/base.py`

 * *Files 5% similar despite different names*

```diff
@@ -156,14 +156,23 @@
         """Check if the file exists or not"""
         try:
             with smart_open.open(self.smartopen_uri, mode="r", transport_params=self.transport_params):
                 return True
         except OSError:
             return False
 
+    @property
+    def databricks_uri(self) -> str:
+        """
+        Return a Databricks compatible URI. In most scenarios, it will be self.path. An exception is Microsoft WASB.
+
+        :return: self.path
+        """
+        return self.path
+
     def databricks_auth_settings(self) -> dict:
         """
         Required settings to upload this file into databricks. Only needed for cloud storage systems
         like S3
         :return: A dictionary of settings keys to settings values
         """
         return {}
```

### Comparing `astro-sdk-python-1.6.0a1/src/astro/files/locations/ftp.py` & `astro-sdk-python-1.7.0a1/src/astro/files/locations/ftp.py`

 * *Files identical despite different names*

### Comparing `astro-sdk-python-1.6.0a1/src/astro/files/locations/google/gcs.py` & `astro-sdk-python-1.7.0a1/src/astro/files/locations/google/gcs.py`

 * *Files identical despite different names*

### Comparing `astro-sdk-python-1.6.0a1/src/astro/files/locations/google/gdrive.py` & `astro-sdk-python-1.7.0a1/src/astro/files/locations/google/gdrive.py`

 * *Files identical despite different names*

### Comparing `astro-sdk-python-1.6.0a1/src/astro/files/locations/http.py` & `astro-sdk-python-1.7.0a1/src/astro/files/locations/http.py`

 * *Files identical despite different names*

### Comparing `astro-sdk-python-1.6.0a1/src/astro/files/locations/local.py` & `astro-sdk-python-1.7.0a1/src/astro/files/locations/local.py`

 * *Files identical despite different names*

### Comparing `astro-sdk-python-1.6.0a1/src/astro/files/operators/files.py` & `astro-sdk-python-1.7.0a1/src/astro/files/operators/files.py`

 * *Files identical despite different names*

### Comparing `astro-sdk-python-1.6.0a1/src/astro/files/types/__init__.py` & `astro-sdk-python-1.7.0a1/src/astro/files/types/__init__.py`

 * *Files identical despite different names*

### Comparing `astro-sdk-python-1.6.0a1/src/astro/files/types/base.py` & `astro-sdk-python-1.7.0a1/src/astro/files/types/base.py`

 * *Files identical despite different names*

### Comparing `astro-sdk-python-1.6.0a1/src/astro/files/types/csv.py` & `astro-sdk-python-1.7.0a1/src/astro/files/types/csv.py`

 * *Files identical despite different names*

### Comparing `astro-sdk-python-1.6.0a1/src/astro/files/types/json.py` & `astro-sdk-python-1.7.0a1/src/astro/files/types/json.py`

 * *Files identical despite different names*

### Comparing `astro-sdk-python-1.6.0a1/src/astro/files/types/ndjson.py` & `astro-sdk-python-1.7.0a1/src/astro/files/types/ndjson.py`

 * *Files identical despite different names*

### Comparing `astro-sdk-python-1.6.0a1/src/astro/files/types/parquet.py` & `astro-sdk-python-1.7.0a1/src/astro/files/types/parquet.py`

 * *Files identical despite different names*

### Comparing `astro-sdk-python-1.6.0a1/src/astro/lineage/__init__.py` & `astro-sdk-python-1.7.0a1/src/astro/lineage/__init__.py`

 * *Files identical despite different names*

### Comparing `astro-sdk-python-1.6.0a1/src/astro/lineage/facets.py` & `astro-sdk-python-1.7.0a1/src/astro/lineage/facets.py`

 * *Files identical despite different names*

### Comparing `astro-sdk-python-1.6.0a1/src/astro/options.py` & `astro-sdk-python-1.7.0a1/src/astro/options.py`

 * *Files identical despite different names*

### Comparing `astro-sdk-python-1.6.0a1/src/astro/query_modifier.py` & `astro-sdk-python-1.7.0a1/src/astro/query_modifier.py`

 * *Files identical despite different names*

### Comparing `astro-sdk-python-1.6.0a1/src/astro/settings.py` & `astro-sdk-python-1.7.0a1/src/astro/settings.py`

 * *Files 7% similar despite different names*

```diff
@@ -13,14 +13,15 @@
 
 SCHEMA = conf.get(SECTION_KEY, "sql_schema", fallback=DEFAULT_SCHEMA)
 POSTGRES_SCHEMA = conf.get(SECTION_KEY, "postgres_default_schema", fallback=SCHEMA)
 BIGQUERY_SCHEMA = conf.get(SECTION_KEY, "bigquery_default_schema", fallback=SCHEMA)
 SNOWFLAKE_SCHEMA = conf.get(SECTION_KEY, "snowflake_default_schema", fallback=SCHEMA)
 REDSHIFT_SCHEMA = conf.get(SECTION_KEY, "redshift_default_schema", fallback=SCHEMA)
 MSSQL_SCHEMA = conf.get(SECTION_KEY, "mssql_default_schema", fallback=SCHEMA)
+MYSQL_SCHEMA = conf.get(SECTION_KEY, "mysql_default_schema", fallback=SCHEMA)
 
 BIGQUERY_SCHEMA_LOCATION = conf.get(
     SECTION_KEY, "bigquery_dataset_location", fallback=DEFAULT_BIGQUERY_SCHEMA_LOCATION
 )
 
 LOAD_FILE_ENABLE_NATIVE_FALLBACK = conf.get(SECTION_KEY, "load_file_enable_native_fallback", fallback=False)
 
@@ -63,14 +64,26 @@
 )
 
 #: How many file rows should be loaded to infer the table columns types
 LOAD_TABLE_AUTODETECT_ROWS_COUNT = conf.getint(
     section=SECTION_KEY, key="load_table_autodetect_rows_count", fallback=1000
 )
 
-
 #: Reduce responses sizes returned by aql.run_raw_sql to avoid trashing the Airflow DB if the BaseXCom is used.
 RAW_SQL_MAX_RESPONSE_SIZE = conf.getint(section=SECTION_KEY, key="run_raw_sql_response_size", fallback=-1)
 
 # Temp changes
 # Should Astro SDK automatically add inlets/outlets to take advantage of Airflow 2.4 Data-aware scheduling
 AUTO_ADD_INLETS_OUTLETS = conf.getboolean(SECTION_KEY, "auto_add_inlets_outlets", fallback=True)
+
+LOAD_TABLE_SCHEMA_EXISTS = False
+
+
+def reload():
+    """
+    Reload settings from environment variable during runtime.
+    """
+    global LOAD_TABLE_SCHEMA_EXISTS  # skipcq: PYL-W0603
+    LOAD_TABLE_SCHEMA_EXISTS = conf.getboolean(SECTION_KEY, "load_table_schema_exists", fallback=False)
+
+
+reload()
```

### Comparing `astro-sdk-python-1.6.0a1/src/astro/sql/__init__.py` & `astro-sdk-python-1.7.0a1/src/astro/sql/__init__.py`

 * *Files identical despite different names*

### Comparing `astro-sdk-python-1.6.0a1/src/astro/sql/operators/append.py` & `astro-sdk-python-1.7.0a1/src/astro/sql/operators/append.py`

 * *Files identical despite different names*

### Comparing `astro-sdk-python-1.6.0a1/src/astro/sql/operators/base_decorator.py` & `astro-sdk-python-1.7.0a1/src/astro/sql/operators/base_decorator.py`

 * *Files 0% similar despite different names*

```diff
@@ -213,14 +213,15 @@
                 self.sql, self.parameters = returned_value
             else:
                 self.sql = returned_value
                 self.parameters = self.parameters or {}
         if self.sql.endswith(".sql"):
             with open(self.sql) as file:
                 self.sql = file.read().replace("\n", " ")
+        self.op_kwargs.pop("sql", None)
 
     def move_function_params_into_sql_params(self, context: dict) -> None:
         """
         Pulls values from the function op_args and op_kwargs and places them into
         parameters for SQLAlchemy to parse
 
         :param context: Airflow's Context dictionary used for rendering templates
```

### Comparing `astro-sdk-python-1.6.0a1/src/astro/sql/operators/cleanup.py` & `astro-sdk-python-1.7.0a1/src/astro/sql/operators/cleanup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,17 +1,19 @@
 from __future__ import annotations
 
 import time
 from datetime import timedelta
 from typing import Any
 
+from airflow import __version__ as airflow_version
 from airflow.decorators.base import get_unique_task_id
 from airflow.exceptions import AirflowException
 from airflow.models.baseoperator import BaseOperator
 from airflow.models.dagrun import DagRun
+from packaging import version
 
 try:
     # Airflow >= 2.3
     from airflow.models.mappedoperator import MappedOperator
 except ImportError:  # pragma: no cover
     # Airflow < 2.3
     MappedOperator = None
@@ -69,54 +71,83 @@
     :param retries: The number of retries that should be performed before failing the task.
         Very relevant if using a synchronous executor. The default is 3.
     :param retry_delay: Delay between running retries. Very relevant if using a synchronous executor.
         The default is 10s.
     :param run_sync_mode: Whether to wait for the DAG to finish or not. Set to True if you want
         to immediately clean all tables. Note that if you supply anything to `tables_to_cleanup`
         this argument is ignored.
+    :param skip_on_failure: Skip cleanup if any upstream task fails. Useful while debugging failed tasks,
+        to prevent temporary tables upstream from being deleted prematurely. The default is False.
     """
 
     template_fields = ("tables_to_cleanup",)
 
     def __init__(
         self,
         *,
         tables_to_cleanup: list[BaseTable] | None = None,
         task_id: str = "",
         retries: int = 3,
         retry_delay: timedelta = timedelta(seconds=10),
         run_sync_mode: bool = False,
+        skip_on_failure: bool = False,
         **kwargs,
     ):
         self.tables_to_cleanup = tables_to_cleanup or []
         self.run_immediately = run_sync_mode
+        self.skip_on_failure = skip_on_failure
         task_id = task_id or get_unique_task_id("cleanup")
 
         super().__init__(task_id=task_id, retries=retries, retry_delay=retry_delay, **kwargs)
 
     def execute(self, context: Context) -> None:
         self.log.info("Execute Cleanup")
         if not self.tables_to_cleanup:
             # tables not provided, attempt to either immediately run or wait for all other tasks to finish
             if not self.run_immediately:
                 self.wait_for_dag_to_finish(context)
             self.tables_to_cleanup = self.get_all_task_outputs(context=context)
+        if self.skip_on_failure:
+            task_instances = context["dag_run"].get_task_instances()
+            if self._has_task_failed(task_instances=task_instances):
+                return None
         temp_tables = filter_for_temp_tables(self.tables_to_cleanup)
         self.log.info(
             "Tables found for cleanup: %s",
             ",".join([t.name for t in temp_tables]),
         )
         for table in temp_tables:
             self.drop_table(table)
 
     def drop_table(self, table: BaseTable) -> None:
         db = create_database(conn_id=table.conn_id, table=table)
         self.log.info("Dropping table %s", table.name)
         db.drop_table(table)
 
+    def _has_task_failed(self, task_instances: list[TaskInstance]) -> bool:
+        """
+        Given a list of task instances, return True if at least one task has failed.
+
+        :param task_instances:
+        :return: boolean if at least one task besides this one has failed
+        """
+        failed_tasks = [
+            (ti.task_id, ti.state)
+            for ti in task_instances
+            if ti.task_id != self.task_id and ti.state == State.FAILED
+        ]
+        if failed_tasks:
+            self.log.info(
+                "skipping cleanup as the following tasks have failed: %s",
+                failed_tasks,
+            )
+            return True
+        else:
+            return False
+
     def _is_dag_running(self, task_instances: list[TaskInstance]) -> bool:
         """
         Given a list of task instances, determine whether the DAG (minus the current cleanup task) is still
         running.
 
         :param task_instances:
         :return: boolean to show if all tasks besides this one have completed
@@ -182,19 +213,22 @@
         executor: str = conf.get("core", "EXECUTOR")
         if job_id:
             executor = cls._get_executor_from_job_id(job_id) or executor
         return executor in ["SequentialExecutor", "DebugExecutor"]
 
     @staticmethod
     def _get_executor_from_job_id(job_id: int) -> str | None:
-        from airflow.jobs.base_job import BaseJob
+        if version.parse(airflow_version) >= version.parse("2.6"):
+            from airflow.jobs.job import Job
+        else:
+            from airflow.jobs.base_job import BaseJob as Job
         from airflow.utils.session import create_session
 
         with create_session() as session:
-            job = session.get(BaseJob, job_id)
+            job = session.get(Job, job_id)
         return job.executor_class if job else None
 
     def get_all_task_outputs(self, context: Context) -> list[BaseTable]:
         """
         In the scenario where we are not given a list of tasks to follow, we will want to gather all temporary tables
         To prevent scenarios where we grab objects that are not tables, we try to only follow up on SQL operators or
         the dataframe operator, as these are the operators that return temporary tables.
```

### Comparing `astro-sdk-python-1.6.0a1/src/astro/sql/operators/data_validations/check_column.py` & `astro-sdk-python-1.7.0a1/src/astro/sql/operators/data_validations/check_column.py`

 * *Files identical despite different names*

### Comparing `astro-sdk-python-1.6.0a1/src/astro/sql/operators/data_validations/check_table.py` & `astro-sdk-python-1.7.0a1/src/astro/sql/operators/data_validations/check_table.py`

 * *Files identical despite different names*

### Comparing `astro-sdk-python-1.6.0a1/src/astro/sql/operators/dataframe.py` & `astro-sdk-python-1.7.0a1/src/astro/sql/operators/dataframe.py`

 * *Files 0% similar despite different names*

```diff
@@ -309,18 +309,18 @@
     :param multiple_outputs: If set to True, the decorated function's return value will be unrolled to
         multiple XCom values. Dict will unroll to XCom values with its keys as XCom keys. Defaults to False.
     :param conn_id: Connection ID for the database you want to connect to. If you do
         not pass in a value for this object
         we can infer the connection ID from the first table passed into the python_callable function.
         (required if there are no table arguments)
     :param database: Database within the SQL instance you want to access. If left blank we will
-        default to the table.metatadata.database in the first Table passed
+        default to the table.metadata.database in the first Table passed
         to the function (required if there are no table arguments)
     :param schema: Schema within the SQL instance you want to access. If left blank we will
-        default to the table.metatadata.schema in the first Table passed to the
+        default to the table.metadata.schema in the first Table passed to the
         function (required if there are no table arguments)
     :param columns_names_capitalization: determines whether to convert all columns to lowercase/uppercase
         in the resulting dataframe
     :param if_exists: Overwrite when set to "replace" else "append"
     :param kwargs: Any keyword arguments supported by the BaseOperator is supported (e.g ``queue``, ``owner``)
     """
     kwargs.update(
```

### Comparing `astro-sdk-python-1.6.0a1/src/astro/sql/operators/drop.py` & `astro-sdk-python-1.7.0a1/src/astro/sql/operators/drop.py`

 * *Files identical despite different names*

### Comparing `astro-sdk-python-1.6.0a1/src/astro/sql/operators/export_file.py` & `astro-sdk-python-1.7.0a1/src/astro/sql/operators/export_file.py`

 * *Files identical despite different names*

### Comparing `astro-sdk-python-1.6.0a1/src/astro/sql/operators/export_table_to_file.py` & `astro-sdk-python-1.7.0a1/src/astro/sql/operators/export_table_to_file.py`

 * *Files identical despite different names*

### Comparing `astro-sdk-python-1.6.0a1/src/astro/sql/operators/export_to_file.py` & `astro-sdk-python-1.7.0a1/src/astro/sql/operators/export_to_file.py`

 * *Files identical despite different names*

### Comparing `astro-sdk-python-1.6.0a1/src/astro/sql/operators/load_file.py` & `astro-sdk-python-1.7.0a1/src/astro/sql/operators/load_file.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,28 +4,28 @@
 from typing import Any
 
 import pandas as pd
 from airflow.decorators.base import get_unique_task_id
 from airflow.hooks.base import BaseHook
 from airflow.models.xcom_arg import XComArg
 
+from astro import settings
 from astro.airflow.datasets import kwargs_with_datasets
 from astro.constants import DEFAULT_CHUNK_SIZE, ColumnCapitalization, LoadExistStrategy
 from astro.databases import create_database
 from astro.databases.base import BaseDatabase
 from astro.dataframes.load_options import (
     PandasCsvLoadOptions,
     PandasJsonLoadOptions,
     PandasNdjsonLoadOptions,
     PandasParquetLoadOptions,
 )
 from astro.dataframes.pandas import PandasDataframe
 from astro.files import File, resolve_file_path_pattern
 from astro.options import LoadOptions, LoadOptionsList
-from astro.settings import LOAD_FILE_ENABLE_NATIVE_FALLBACK
 from astro.sql.operators.base_operator import AstroSQLBaseOperator
 from astro.table import BaseTable
 from astro.utils.compat.typing import Context
 
 DEPRECATED_LOAD_OPTIONS_CLASSES = [
     PandasCsvLoadOptions,
     PandasJsonLoadOptions,
@@ -43,14 +43,15 @@
     :param chunk_size: Specify the number of records in each batch to be written at a time.
     :param if_exists: Overwrite file if exists. Default False.
     :param use_native_support: Use native support for data transfer if available on the destination.
     :param native_support_kwargs: kwargs to be used by method involved in native support flow
     :param columns_names_capitalization: determines whether to convert all columns to lowercase/uppercase
             in the resulting dataframe
     :param enable_native_fallback: Use enable_native_fallback=True to fall back to default transfer
+    :param schema_exists: Declare the table schema already exists and that load_file should not check if it exists
 
     :return: If ``output_table`` is passed this operator returns a Table object. If not
         passed, returns a dataframe.
     """
 
     template_fields = ("output_table", "input_file")
 
@@ -61,15 +62,16 @@
         chunk_size: int = DEFAULT_CHUNK_SIZE,
         if_exists: LoadExistStrategy = "replace",
         ndjson_normalize_sep: str = "_",
         use_native_support: bool = True,
         native_support_kwargs: dict | None = None,
         load_options: LoadOptions | list[LoadOptions] | None = None,
         columns_names_capitalization: ColumnCapitalization = "original",
-        enable_native_fallback: bool | None = LOAD_FILE_ENABLE_NATIVE_FALLBACK,
+        enable_native_fallback: bool | None = settings.LOAD_FILE_ENABLE_NATIVE_FALLBACK,
+        schema_exists: bool = settings.LOAD_TABLE_SCHEMA_EXISTS,
         **kwargs,
     ) -> None:
         kwargs.setdefault("task_id", get_unique_task_id("load_file"))
         super().__init__(
             **kwargs_with_datasets(
                 kwargs=kwargs,
                 input_datasets=input_file,
@@ -108,14 +110,15 @@
         self.if_exists = if_exists
         self.ndjson_normalize_sep = ndjson_normalize_sep
         self.normalize_config: dict[str, str] = {}
         self.use_native_support = use_native_support
         self.native_support_kwargs: dict[str, Any] = native_support_kwargs or {}
         self.columns_names_capitalization = columns_names_capitalization
         self.enable_native_fallback = enable_native_fallback
+        self.schema_exists = schema_exists
         self.load_options_list = LoadOptionsList(load_options)
 
     def execute(self, context: Context) -> BaseTable | File:  # skipcq: PYL-W0613
         """
         Load an existing dataset from a supported file into a SQL table or a Dataframe.
         """
         if self.input_file.conn_id:
@@ -155,14 +158,15 @@
             output_table=self.output_table,
             if_exists=self.if_exists,
             chunk_size=self.chunk_size,
             use_native_support=self.use_native_support,
             native_support_kwargs=self.native_support_kwargs,
             columns_names_capitalization=self.columns_names_capitalization,
             enable_native_fallback=self.enable_native_fallback,
+            schema_exists=self.schema_exists,
             databricks_job_name=f"Load data {self.dag_id}_{self.task_id}",
         )
         self.log.info("Completed loading the data into %s.", self.output_table)
         return self.output_table
 
     def load_data_to_dataframe(self, input_file: File) -> pd.DataFrame | None:
         """
```

### Comparing `astro-sdk-python-1.6.0a1/src/astro/sql/operators/merge.py` & `astro-sdk-python-1.7.0a1/src/astro/sql/operators/merge.py`

 * *Files identical despite different names*

### Comparing `astro-sdk-python-1.6.0a1/src/astro/sql/operators/raw_sql.py` & `astro-sdk-python-1.7.0a1/src/astro/sql/operators/raw_sql.py`

 * *Files 0% similar despite different names*

```diff
@@ -198,18 +198,18 @@
     :param python_callable: This parameter is filled in automatically when you use the transform function as a
         decorator. This is where the python function gets passed to the wrapping function
     :param conn_id: Connection ID for the database you want to connect to.
         If you do not pass in a value for this object we can infer the connection ID from the first table
         passed into the python_callable function. (required if there are no table arguments)
     :param parameters: parameters to pass into the SQL query
     :param database: Database within the SQL instance you want to access. If left blank we will default to the
-        table.metatadata.database in the first Table passed to the function
+        table.metadata.database in the first Table passed to the function
         (required if there are no table arguments)
     :param schema: Schema within the SQL instance you want to access. If left blank we will default to the
-        table.metatadata.schema in the first Table passed to the function
+        table.metadata.schema in the first Table passed to the function
         (required if there are no table arguments)
     :param handler: Handler function to process the result of the SQL query. For more information please consult
         https://docs.sqlalchemy.org/en/14/core/connections.html#sqlalchemy.engine.Result
     :param results_format: Format of the results returned by the SQL query. Overrides the handler, if provided.
     :param fail_on_empty: If True and a results_format is provided, raises an exception if the query returns no results.
     :param response_size: Used to trim the responses returned to avoid trashing the Airflow DB.
         The default value is -1, which means the response is not changed. Otherwise, if the response is a list,
```

### Comparing `astro-sdk-python-1.6.0a1/src/astro/sql/operators/transform.py` & `astro-sdk-python-1.7.0a1/src/astro/sql/operators/transform.py`

 * *Files 0% similar despite different names*

```diff
@@ -104,17 +104,17 @@
     :param python_callable: This parameter is filled in automatically when you use the transform function as a decorator
         This is where the python function gets passed to the wrapping function
     :param conn_id: Connection ID for the database you want to connect to. If you do not pass in a value for this object
         we can infer the connection ID from the first table passed into the python_callable function.
         (required if there are no table arguments)
     :param parameters: parameters to pass into the SQL query
     :param database: Database within the SQL instance you want to access. If left blank we will default to the
-        table.metatadata.database in the first Table passed to the function (required if there are no table arguments)
+        table.metadata.database in the first Table passed to the function (required if there are no table arguments)
     :param schema: Schema within the SQL instance you want to access. If left blank we will default to the
-        table.metatadata.schema in the first Table passed to the function (required if there are no table arguments)
+        table.metadata.schema in the first Table passed to the function (required if there are no table arguments)
     :param kwargs: Any keyword arguments supported by the BaseOperator is supported (e.g ``queue``, ``owner``)
     :return: Transform functions return a ``Table`` object that can be passed to future tasks.
         This table will be either an auto-generated temporary table,
         or will overwrite a table given in the `output_table` parameter.
     """
 
     kwargs.update(
@@ -149,17 +149,17 @@
     :param file_path: File path for the SQL file you would like to parse. Can be an absolute path, or you can use a
         relative path if the `template_searchpath` variable is set in your DAG
     :param conn_id: Connection ID for the database you want to connect to. If you do not pass in a value for this object
         we can infer the connection ID from the first table passed into the python_callable function.
         (required if there are no table arguments)
     :param parameters: parameters to pass into the SQL query
     :param database: Database within the SQL instance you want to access. If left blank we will default to the
-        table.metatadata.database in the first Table passed to the function (required if there are no table arguments)
+        table.metadata.database in the first Table passed to the function (required if there are no table arguments)
     :param schema: Schema within the SQL instance you want to access. If left blank we will default to the
-        table.metatadata.schema in the first Table passed to the function (required if there are no table arguments)
+        table.metadata.schema in the first Table passed to the function (required if there are no table arguments)
     :param kwargs: Any keyword arguments supported by the BaseOperator is supported (e.g ``queue``, ``owner``)
     :return: Transform functions return a ``Table`` object that can be passed to future tasks.
         This table will be either an auto-generated temporary table,
         or will overwrite a table given in the `output_table` parameter.
     """
 
     kwargs.update(
```

### Comparing `astro-sdk-python-1.6.0a1/src/astro/sql/operators/upstream_task_mixin.py` & `astro-sdk-python-1.7.0a1/src/astro/sql/operators/upstream_task_mixin.py`

 * *Files identical despite different names*

### Comparing `astro-sdk-python-1.6.0a1/src/astro/table.py` & `astro-sdk-python-1.7.0a1/src/astro/table.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from __future__ import annotations
 
 import random
 import string
-from typing import Any
+from typing import Any, ClassVar
 
 from attr import define, field, fields_dict
 from sqlalchemy import Column, MetaData
 
 from astro.airflow.datasets import Dataset
 from astro.databases import create_database
 from astro.settings import OPENLINEAGE_EMIT_TEMP_TABLE_EVENT
@@ -46,14 +46,15 @@
     :param conn_id: The Airflow connection id. This will be used to identify the right database type at the runtime
     :param metadata: A metadata object which will have database or schema name
     :param columns: columns which define the database table schema.
     :sphinx-autoapi-skip:
     """
 
     template_fields = ("name",)
+    version: ClassVar[int] = 1
 
     # TODO: discuss alternative names to this class, since it contains metadata as opposed to be the
     # SQL table itself
     # Some ideas: TableRef, TableMetadata, TableData, TableDataset
     name: str = field(default="")
     conn_id: str = field(default="")
     # Setting converter allows passing a dictionary to metadata arg
@@ -174,14 +175,33 @@
         Based on airflow config ```OPENLINEAGE_EMIT_TEMP_TABLE_EVENT``` value and table type
         check whether to emit temp table event in openlineage or not
         """
         return (not isinstance(self, TempTable)) or (
             isinstance(self, TempTable) and OPENLINEAGE_EMIT_TEMP_TABLE_EVENT
         )
 
+    def serialize(self) -> dict[str, Any]:
+        return {
+            "name": self.name,
+            "temp": self.temp,
+            "conn_id": self.conn_id,
+            "metadata": {"schema": self.metadata.schema, "database": self.metadata.database},
+        }
+
+    @staticmethod
+    def deserialize(data: dict[str, Any], version: int):
+        if version > 1:
+            raise TypeError(f"version > {BaseTable.version}")
+        return Table(
+            name=data["name"],
+            temp=data["temp"],
+            conn_id=data["conn_id"],
+            metadata=Metadata(**data["metadata"]),
+        )
+
 
 @define(slots=False)
 class TempTable(BaseTable):
     """
     Internal class to represent a Temporary table
 
     :sphinx-autoapi-skip:
```

### Comparing `astro-sdk-python-1.6.0a1/src/astro/utils/compat/typing.py` & `astro-sdk-python-1.7.0a1/src/astro/utils/compat/typing.py`

 * *Files identical despite different names*

### Comparing `astro-sdk-python-1.6.0a1/src/astro/utils/dataframe.py` & `astro-sdk-python-1.7.0a1/src/astro/utils/dataframe.py`

 * *Files identical despite different names*

### Comparing `astro-sdk-python-1.6.0a1/src/astro/utils/load.py` & `astro-sdk-python-1.7.0a1/src/astro/utils/load.py`

 * *Files identical despite different names*

### Comparing `astro-sdk-python-1.6.0a1/src/astro/utils/path.py` & `astro-sdk-python-1.7.0a1/src/astro/utils/path.py`

 * *Files identical despite different names*

### Comparing `astro-sdk-python-1.6.0a1/src/astro/utils/table.py` & `astro-sdk-python-1.7.0a1/src/astro/utils/table.py`

 * *Files identical despite different names*

### Comparing `astro-sdk-python-1.6.0a1/PKG-INFO` & `astro-sdk-python-1.7.0a1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: astro-sdk-python
-Version: 1.6.0a1
+Version: 1.7.0a1
 Summary: Astro SDK allows rapid and clean development of {Extract, Load, Transform} workflows using Python and SQL, powered by Apache Airflow.
 Keywords: airflow,provider,astronomer,sql,decorator,task flow,elt,etl,dag
 Author-email: Astronomer <humans@astronomer.io>
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: Apache Software License
@@ -40,14 +40,15 @@
 Requires-Dist: s3fs ; extra == "all"
 Requires-Dist: protobuf<=3.20 ; extra == "all"
 Requires-Dist: openlineage-airflow>=0.17.0 ; extra == "all"
 Requires-Dist: apache-airflow-providers-microsoft-azure ; extra == "all"
 Requires-Dist: azure-storage-blob ; extra == "all"
 Requires-Dist: apache-airflow-providers-microsoft-mssql>=3.2 ; extra == "all"
 Requires-Dist: airflow-provider-duckdb>=0.0.2 ; extra == "all"
+Requires-Dist: apache-airflow-providers-mysql ; extra == "all"
 Requires-Dist: apache-airflow-providers-amazon>=5.0.0 ; extra == "amazon"
 Requires-Dist: s3fs ; extra == "amazon"
 Requires-Dist: smart-open[s3]>=5.2.1 ; extra == "amazon"
 Requires-Dist: apache-airflow-providers-microsoft-azure ; extra == "azure"
 Requires-Dist: azure-storage-blob ; extra == "azure"
 Requires-Dist: smart-open[azure]>=5.2.1 ; extra == "azure"
 Requires-Dist: databricks-cli ; extra == "databricks"
@@ -60,14 +61,15 @@
 Requires-Dist: apache-airflow-providers-ftp>=3.0.0 ; extra == "ftp"
 Requires-Dist: smart-open>=5.2.1 ; extra == "ftp"
 Requires-Dist: protobuf<=3.20 ; extra == "google"
 Requires-Dist: apache-airflow-providers-google>=6.4.0 ; extra == "google"
 Requires-Dist: sqlalchemy-bigquery>=1.3.0 ; extra == "google"
 Requires-Dist: smart-open[gcs]>=5.2.1 ; extra == "google"
 Requires-Dist: apache-airflow-providers-microsoft-mssql>=3.2 ; extra == "mssql"
+Requires-Dist: apache-airflow-providers-mysql ; extra == "mysql"
 Requires-Dist: openlineage-airflow>=0.17.0 ; extra == "openlineage"
 Requires-Dist: apache-airflow-providers-postgres ; extra == "postgres"
 Requires-Dist: apache-airflow-providers-sftp>=4.0.0 ; extra == "sftp"
 Requires-Dist: smart-open[ssh]>=5.2.1 ; extra == "sftp"
 Requires-Dist: apache-airflow-providers-snowflake ; extra == "snowflake"
 Requires-Dist: snowflake-sqlalchemy>=1.2.0 ; extra == "snowflake"
 Requires-Dist: snowflake-connector-python[pandas]<3.0.0 ; extra == "snowflake"
@@ -88,14 +90,15 @@
 Provides-Extra: azure
 Provides-Extra: databricks
 Provides-Extra: doc
 Provides-Extra: duckdb
 Provides-Extra: ftp
 Provides-Extra: google
 Provides-Extra: mssql
+Provides-Extra: mysql
 Provides-Extra: openlineage
 Provides-Extra: postgres
 Provides-Extra: sftp
 Provides-Extra: snowflake
 Provides-Extra: tests
 
 <h1 align="center">
```

