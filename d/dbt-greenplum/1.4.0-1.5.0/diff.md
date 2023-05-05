# Comparing `tmp/dbt-greenplum-1.4.0.tar.gz` & `tmp/dbt-greenplum-1.5.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dbt-greenplum-1.4.0.tar", last modified: Tue Mar 14 19:23:33 2023, max compression
+gzip compressed data, was "dbt-greenplum-1.5.0.tar", last modified: Fri May  5 13:20:44 2023, max compression
```

## Comparing `dbt-greenplum-1.4.0.tar` & `dbt-greenplum-1.5.0.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 markporoshin   (501) staff       (20)        0 2023-03-14 19:23:33.871534 dbt-greenplum-1.4.0/
--rw-r--r--   0 markporoshin   (501) staff       (20)       46 2022-05-25 06:56:05.000000 dbt-greenplum-1.4.0/MANIFEST.in
--rw-r--r--   0 markporoshin   (501) staff       (20)    11411 2023-03-14 19:23:33.871106 dbt-greenplum-1.4.0/PKG-INFO
--rw-r--r--   0 markporoshin   (501) staff       (20)    10552 2023-03-14 19:10:33.000000 dbt-greenplum-1.4.0/README.md
-drwxr-xr-x   0 markporoshin   (501) staff       (20)        0 2023-03-14 19:23:33.858685 dbt-greenplum-1.4.0/dbt/
-drwxr-xr-x   0 markporoshin   (501) staff       (20)        0 2023-03-14 19:23:33.861020 dbt-greenplum-1.4.0/dbt/adapters/
--rw-r--r--   0 markporoshin   (501) staff       (20)      338 2022-09-04 08:29:11.000000 dbt-greenplum-1.4.0/dbt/adapters/__init__.py
-drwxr-xr-x   0 markporoshin   (501) staff       (20)        0 2023-03-14 19:23:33.863227 dbt-greenplum-1.4.0/dbt/adapters/greenplum/
--rw-r--r--   0 markporoshin   (501) staff       (20)      445 2022-09-04 08:29:11.000000 dbt-greenplum-1.4.0/dbt/adapters/greenplum/__init__.py
--rw-r--r--   0 markporoshin   (501) staff       (20)       18 2023-03-14 19:10:33.000000 dbt-greenplum-1.4.0/dbt/adapters/greenplum/__version__.py
--rw-r--r--   0 markporoshin   (501) staff       (20)      366 2022-09-04 08:29:11.000000 dbt-greenplum-1.4.0/dbt/adapters/greenplum/connections.py
--rw-r--r--   0 markporoshin   (501) staff       (20)      211 2022-09-04 08:29:11.000000 dbt-greenplum-1.4.0/dbt/adapters/greenplum/impl.py
-drwxr-xr-x   0 markporoshin   (501) staff       (20)        0 2023-03-14 19:23:33.858797 dbt-greenplum-1.4.0/dbt/include/
-drwxr-xr-x   0 markporoshin   (501) staff       (20)        0 2023-03-14 19:23:33.864652 dbt-greenplum-1.4.0/dbt/include/greenplum/
--rw-r--r--   0 markporoshin   (501) staff       (20)       52 2022-09-04 08:29:11.000000 dbt-greenplum-1.4.0/dbt/include/greenplum/__init__.py
--rw-r--r--   0 markporoshin   (501) staff       (20)       76 2022-09-04 08:29:11.000000 dbt-greenplum-1.4.0/dbt/include/greenplum/dbt_project.yml
-drwxr-xr-x   0 markporoshin   (501) staff       (20)        0 2023-03-14 19:23:33.867632 dbt-greenplum-1.4.0/dbt/include/greenplum/macros/
--rw-r--r--   0 markporoshin   (501) staff       (20)     4732 2023-02-18 23:09:34.000000 dbt-greenplum-1.4.0/dbt/include/greenplum/macros/adapters.sql
--rw-r--r--   0 markporoshin   (501) staff       (20)      150 2022-09-04 08:29:11.000000 dbt-greenplum-1.4.0/dbt/include/greenplum/macros/catalog.sql
--rw-r--r--   0 markporoshin   (501) staff       (20)      398 2023-02-18 23:09:34.000000 dbt-greenplum-1.4.0/dbt/include/greenplum/macros/distribution.sql
-drwxr-xr-x   0 markporoshin   (501) staff       (20)        0 2023-03-14 19:23:33.868045 dbt-greenplum-1.4.0/dbt/include/greenplum/macros/materializations/
--rw-r--r--   0 markporoshin   (501) staff       (20)      163 2022-09-04 08:29:11.000000 dbt-greenplum-1.4.0/dbt/include/greenplum/macros/materializations/snapshot_merge.sql
--rw-r--r--   0 markporoshin   (501) staff       (20)     1138 2023-02-18 23:09:34.000000 dbt-greenplum-1.4.0/dbt/include/greenplum/macros/partitions.sql
--rw-r--r--   0 markporoshin   (501) staff       (20)      509 2023-02-18 23:09:34.000000 dbt-greenplum-1.4.0/dbt/include/greenplum/macros/storage_parameters.sql
--rw-r--r--   0 markporoshin   (501) staff       (20)      205 2022-04-01 05:56:39.000000 dbt-greenplum-1.4.0/dbt/include/greenplum/sample_profiles.yml
-drwxr-xr-x   0 markporoshin   (501) staff       (20)        0 2023-03-14 19:23:33.870584 dbt-greenplum-1.4.0/dbt_greenplum.egg-info/
--rw-r--r--   0 markporoshin   (501) staff       (20)    11411 2023-03-14 19:23:33.000000 dbt-greenplum-1.4.0/dbt_greenplum.egg-info/PKG-INFO
--rw-r--r--   0 markporoshin   (501) staff       (20)      821 2023-03-14 19:23:33.000000 dbt-greenplum-1.4.0/dbt_greenplum.egg-info/SOURCES.txt
--rw-r--r--   0 markporoshin   (501) staff       (20)        1 2023-03-14 19:23:33.000000 dbt-greenplum-1.4.0/dbt_greenplum.egg-info/dependency_links.txt
--rw-r--r--   0 markporoshin   (501) staff       (20)        1 2022-05-25 13:56:00.000000 dbt-greenplum-1.4.0/dbt_greenplum.egg-info/not-zip-safe
--rw-r--r--   0 markporoshin   (501) staff       (20)       57 2023-03-14 19:23:33.000000 dbt-greenplum-1.4.0/dbt_greenplum.egg-info/requires.txt
--rw-r--r--   0 markporoshin   (501) staff       (20)        4 2023-03-14 19:23:33.000000 dbt-greenplum-1.4.0/dbt_greenplum.egg-info/top_level.txt
--rw-r--r--   0 markporoshin   (501) staff       (20)       38 2023-03-14 19:23:33.871639 dbt-greenplum-1.4.0/setup.cfg
--rw-r--r--   0 markporoshin   (501) staff       (20)     3949 2023-03-14 19:10:33.000000 dbt-greenplum-1.4.0/setup.py
+drwxr-xr-x   0 markporoshin   (501) staff       (20)        0 2023-05-05 13:20:44.294606 dbt-greenplum-1.5.0/
+-rw-r--r--   0 markporoshin   (501) staff       (20)       46 2022-05-25 06:56:05.000000 dbt-greenplum-1.5.0/MANIFEST.in
+-rw-r--r--   0 markporoshin   (501) staff       (20)    11527 2023-05-05 13:20:44.293537 dbt-greenplum-1.5.0/PKG-INFO
+-rw-r--r--   0 markporoshin   (501) staff       (20)    10668 2023-05-05 13:20:08.000000 dbt-greenplum-1.5.0/README.md
+drwxr-xr-x   0 markporoshin   (501) staff       (20)        0 2023-05-05 13:20:44.273464 dbt-greenplum-1.5.0/dbt/
+drwxr-xr-x   0 markporoshin   (501) staff       (20)        0 2023-05-05 13:20:44.276096 dbt-greenplum-1.5.0/dbt/adapters/
+-rw-r--r--   0 markporoshin   (501) staff       (20)      338 2022-09-04 08:29:11.000000 dbt-greenplum-1.5.0/dbt/adapters/__init__.py
+drwxr-xr-x   0 markporoshin   (501) staff       (20)        0 2023-05-05 13:20:44.278578 dbt-greenplum-1.5.0/dbt/adapters/greenplum/
+-rw-r--r--   0 markporoshin   (501) staff       (20)      445 2022-09-04 08:29:11.000000 dbt-greenplum-1.5.0/dbt/adapters/greenplum/__init__.py
+-rw-r--r--   0 markporoshin   (501) staff       (20)       18 2023-05-05 13:20:08.000000 dbt-greenplum-1.5.0/dbt/adapters/greenplum/__version__.py
+-rw-r--r--   0 markporoshin   (501) staff       (20)      366 2022-09-04 08:29:11.000000 dbt-greenplum-1.5.0/dbt/adapters/greenplum/connections.py
+-rw-r--r--   0 markporoshin   (501) staff       (20)      211 2022-09-04 08:29:11.000000 dbt-greenplum-1.5.0/dbt/adapters/greenplum/impl.py
+drwxr-xr-x   0 markporoshin   (501) staff       (20)        0 2023-05-05 13:20:44.273576 dbt-greenplum-1.5.0/dbt/include/
+drwxr-xr-x   0 markporoshin   (501) staff       (20)        0 2023-05-05 13:20:44.280482 dbt-greenplum-1.5.0/dbt/include/greenplum/
+-rw-r--r--   0 markporoshin   (501) staff       (20)       52 2022-09-04 08:29:11.000000 dbt-greenplum-1.5.0/dbt/include/greenplum/__init__.py
+-rw-r--r--   0 markporoshin   (501) staff       (20)       76 2022-09-04 08:29:11.000000 dbt-greenplum-1.5.0/dbt/include/greenplum/dbt_project.yml
+drwxr-xr-x   0 markporoshin   (501) staff       (20)        0 2023-05-05 13:20:44.284472 dbt-greenplum-1.5.0/dbt/include/greenplum/macros/
+-rw-r--r--   0 markporoshin   (501) staff       (20)     4918 2023-05-05 13:20:08.000000 dbt-greenplum-1.5.0/dbt/include/greenplum/macros/adapters.sql
+-rw-r--r--   0 markporoshin   (501) staff       (20)      147 2023-05-05 13:20:08.000000 dbt-greenplum-1.5.0/dbt/include/greenplum/macros/catalog.sql
+-rw-r--r--   0 markporoshin   (501) staff       (20)      398 2023-02-18 23:09:34.000000 dbt-greenplum-1.5.0/dbt/include/greenplum/macros/distribution.sql
+drwxr-xr-x   0 markporoshin   (501) staff       (20)        0 2023-05-05 13:20:44.285569 dbt-greenplum-1.5.0/dbt/include/greenplum/macros/materializations/
+-rw-r--r--   0 markporoshin   (501) staff       (20)      163 2022-09-04 08:29:11.000000 dbt-greenplum-1.5.0/dbt/include/greenplum/macros/materializations/snapshot_merge.sql
+-rw-r--r--   0 markporoshin   (501) staff       (20)     1138 2023-02-18 23:09:34.000000 dbt-greenplum-1.5.0/dbt/include/greenplum/macros/partitions.sql
+-rw-r--r--   0 markporoshin   (501) staff       (20)      509 2023-02-18 23:09:34.000000 dbt-greenplum-1.5.0/dbt/include/greenplum/macros/storage_parameters.sql
+-rw-r--r--   0 markporoshin   (501) staff       (20)      205 2022-04-01 05:56:39.000000 dbt-greenplum-1.5.0/dbt/include/greenplum/sample_profiles.yml
+drwxr-xr-x   0 markporoshin   (501) staff       (20)        0 2023-05-05 13:20:44.292145 dbt-greenplum-1.5.0/dbt_greenplum.egg-info/
+-rw-r--r--   0 markporoshin   (501) staff       (20)    11527 2023-05-05 13:20:44.000000 dbt-greenplum-1.5.0/dbt_greenplum.egg-info/PKG-INFO
+-rw-r--r--   0 markporoshin   (501) staff       (20)      821 2023-05-05 13:20:44.000000 dbt-greenplum-1.5.0/dbt_greenplum.egg-info/SOURCES.txt
+-rw-r--r--   0 markporoshin   (501) staff       (20)        1 2023-05-05 13:20:44.000000 dbt-greenplum-1.5.0/dbt_greenplum.egg-info/dependency_links.txt
+-rw-r--r--   0 markporoshin   (501) staff       (20)        1 2022-05-25 13:56:00.000000 dbt-greenplum-1.5.0/dbt_greenplum.egg-info/not-zip-safe
+-rw-r--r--   0 markporoshin   (501) staff       (20)       57 2023-05-05 13:20:44.000000 dbt-greenplum-1.5.0/dbt_greenplum.egg-info/requires.txt
+-rw-r--r--   0 markporoshin   (501) staff       (20)        4 2023-05-05 13:20:44.000000 dbt-greenplum-1.5.0/dbt_greenplum.egg-info/top_level.txt
+-rw-r--r--   0 markporoshin   (501) staff       (20)       38 2023-05-05 13:20:44.294765 dbt-greenplum-1.5.0/setup.cfg
+-rw-r--r--   0 markporoshin   (501) staff       (20)     3949 2023-05-05 13:20:08.000000 dbt-greenplum-1.5.0/setup.py
```

### Comparing `dbt-greenplum-1.4.0/PKG-INFO` & `dbt-greenplum-1.5.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbt-greenplum
-Version: 1.4.0
+Version: 1.5.0
 Summary: The greenplum adapter plugin for dbt (data build tool)
 Home-page: https://github.com/markporoshin/dbt-greenplum
 Author: Mark Poroshin
 Author-email: mark.poroshin@yandex.ru
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
@@ -48,36 +48,38 @@
 Where `<version>` is same as your dbt version
 
 Available versions:
  - 0.19.2
  - 1.0.4
  - 1.2.0
  - 1.4.0
+ - 1.5.0
 
 ## Supported Features
 
-You can specify following preference 
- - starage type
+You can specify following settings:
+ - Storage type
    - heap
    - appendoptimized
- - distribution
+ - Distribution
    - `distributed randomly` by defaut
    - `distributed by (column, [ ... ] )` by setting up `distributed_by` parameter in the model config
- - table orientation
+   - `distributed replicated` by setting up `distributed_replicated=true` parameter in the model config
+ - Table orientation
    - `orientation=colum` by default
    - `orientation=row` by setting up `orientation` parameter in `row` in the model config
- - compress type, level and blocksize with default values
+ - Compress type, level and blocksize with default values
    ```bash
-    blocksize=32768,
     compresstype=ZLIB,
-    compresslevel=1
+    compresslevel=1,
+    blocksize=32768
    ``` 
     You can also specify `blocksize`, `compresstype`, `compresslevel` in the model config
- - appendonly|appendoptimized preference by default is `true`, also you can override it by setting up `appendoptimized` field in the model config
- - partitions (see "partition" chapter below)
+ - `appendoptimized` preference by default is `true`, also you can override it by setting up `appendoptimized` field in the model config
+ - Partitions (see "Partition" chapter below)
 
 ### Heap table example
 
 To create heap table set `appendoptimized` parameter value to `false` 
 
 ```SQL
 {{
@@ -195,15 +197,15 @@
        );
    {% endset %}
 
    {{
        config(
            materialized='table',
            distributed_by='id',
-           appendonly='true',
+           appendoptimized=true,
            orientation='column',
            compresstype='ZLIB',
            compresslevel=1,
            blocksize=32768,
            fields_string=fields_string,
            raw_partition=raw_partition,
            default_partition_name='other_data'
@@ -226,15 +228,15 @@
    will produce following sql code
    ```SQL
    create table if not exists "database"."schema"."my_first_dbt_model__dbt_tmp" (
        id int4 null,
        incomingdate timestamp NULL
    )
    with (
-       appendonly=true,
+       appendoptimized=true,
        blocksize=32768,
        orientation=column,
        compresstype=ZLIB,
        compresslevel=1
    )
    DISTRIBUTED BY (id)
    PARTITION BY RANGE (incomingdate)
@@ -279,15 +281,15 @@
        DEFAULT PARTITION extra
    {% endset %}
    
    {{
        config(
            materialized='table',
            distributed_by='id',
-           appendonly='true',
+           appendoptimized=true,
            orientation='column',
            compresstype='ZLIB',
            compresslevel=1,
            blocksize=32768,
            fields_string=fields_string,
            partition_type=partition_type,
            partition_column=partition_column,
@@ -324,15 +326,15 @@
    {%- set partition_every = '1 day' -%}
    
    
    {{
        config(
            materialized='table',
            distributed_by='id',
-           appendonly='true',
+           appendoptimized=true,
            orientation='column',
            compresstype='ZLIB',
            compresslevel=1,
            blocksize=32768,
            fields_string=fields_string,
            partition_type=partition_type,
            partition_column=partition_column,
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: dbt-greenplum Version: 1.4.0 Summary: The greenplum
+Metadata-Version: 2.1 Name: dbt-greenplum Version: 1.5.0 Summary: The greenplum
 adapter plugin for dbt (data build tool) Home-page: https://github.com/
 markporoshin/dbt-greenplum Author: Mark Poroshin Author-email:
 mark.poroshin@yandex.ru License: UNKNOWN Platform: UNKNOWN Classifier:
 Development Status :: 5 - Production/Stable Classifier: License :: OSI Approved
 :: Apache Software License Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: MacOS :: MacOS X Classifier: Operating System
 :: POSIX :: Linux Classifier: Programming Language :: Python :: 3.7 Classifier:
@@ -18,36 +18,38 @@
 filter, rename, and pre-aggregate the raw data in your warehouse so that it's
 ready for analysis. ## dbt-greenplum The `dbt-greenplum` package contains the
 code enabling dbt to work with Greenplum. This adapter based on [postgres-
 adapter](https://github.com/dbt-labs/dbt-core/blob/main/plugins/postgres/dbt/
 include/postgres/profile_template.yml) with a bit difference for a greenplum
 specific features ## Installation Easiest way to start use dbt-greenplum is to
 install it using pip `pip install dbt-greenplum==` Where `` is same as your dbt
-version Available versions: - 0.19.2 - 1.0.4 - 1.2.0 - 1.4.0 ## Supported
-Features You can specify following preference - starage type - heap -
-appendoptimized - distribution - `distributed randomly` by defaut -
+version Available versions: - 0.19.2 - 1.0.4 - 1.2.0 - 1.4.0 - 1.5.0 ##
+Supported Features You can specify following settings: - Storage type - heap -
+appendoptimized - Distribution - `distributed randomly` by defaut -
 `distributed by (column, [ ... ] )` by setting up `distributed_by` parameter in
-the model config - table orientation - `orientation=colum` by default -
-`orientation=row` by setting up `orientation` parameter in `row` in the model
-config - compress type, level and blocksize with default values ```bash
-blocksize=32768, compresstype=ZLIB, compresslevel=1 ``` You can also specify
-`blocksize`, `compresstype`, `compresslevel` in the model config -
-appendonly|appendoptimized preference by default is `true`, also you can
-override it by setting up `appendoptimized` field in the model config -
-partitions (see "partition" chapter below) ### Heap table example To create
-heap table set `appendoptimized` parameter value to `false` ```SQL {{ config
-( ... materialized='table', appendoptimized=false ... ) }} select 1 as "id" ```
-will produce following SQL code ```SQL create table "".""."" with
-( appendoptimized=false ) as ( select 1 as "id" ) DISTRIBUTED RANDOMLY; ``` ###
-Appendoptimized table example You can use `appendopimized` or `appendonly`
-(legacy) to create appendoptimized table Such model definition ```SQL {{ config
-( materialized='table', distributed_by='id', appendoptimized=true,
-orientation='column', compresstype='ZLIB', compresslevel=1, blocksize=32768 )
-}} with source_data as ( select 1 as id union all select null as id ) select *
-from source_data ``` will produce following sql code ```SQL create table
+the model config - `distributed replicated` by setting up
+`distributed_replicated=true` parameter in the model config - Table orientation
+- `orientation=colum` by default - `orientation=row` by setting up
+`orientation` parameter in `row` in the model config - Compress type, level and
+blocksize with default values ```bash compresstype=ZLIB, compresslevel=1,
+blocksize=32768 ``` You can also specify `blocksize`, `compresstype`,
+`compresslevel` in the model config - `appendoptimized` preference by default
+is `true`, also you can override it by setting up `appendoptimized` field in
+the model config - Partitions (see "Partition" chapter below) ### Heap table
+example To create heap table set `appendoptimized` parameter value to `false`
+```SQL {{ config( ... materialized='table', appendoptimized=false ... ) }}
+select 1 as "id" ``` will produce following SQL code ```SQL create table
+"".""."" with ( appendoptimized=false ) as ( select 1 as "id" ) DISTRIBUTED
+RANDOMLY; ``` ### Appendoptimized table example You can use `appendopimized` or
+`appendonly`(legacy) to create appendoptimized table Such model definition
+```SQL {{ config( materialized='table', distributed_by='id',
+appendoptimized=true, orientation='column', compresstype='ZLIB',
+compresslevel=1, blocksize=32768 ) }} with source_data as ( select 1 as id
+union all select null as id ) select * from source_data ``` will produce
+following sql code ```SQL create table
 "dvault"."dv"."my_first_dbt_model__dbt_tmp" with ( appendoptimized=true,
 blocksize=32768, orientation=column, compresstype=ZLIB, compresslevel=1 ) as
 ( with source_data as ( select 1 as id union all select null as id ) select *
 from source_data ) distributed by (id); alter table
 "dvault"."dv"."my_first_dbt_model__dbt_tmp" rename to "my_first_dbt_model"; ```
 ### Partitions Greenplum does not support partitions with `create table as`
 [construction](https://gpdb.docs.pivotal.io/6-9/ref_guide/sql_commands/
@@ -61,51 +63,52 @@
 `partition_values` - `default_partition_name` - name of default partition
 'other' by default Let consider examples of definition model with partitions -
 using `raw_partition` parameter ```SQL {% set fields_string %} id int4 null,
 incomingdate timestamp NULL {% endset %} {% set raw_partition %} PARTITION BY
 RANGE (incomingdate) ( START ('2021-01-01'::timestamp) INCLUSIVE END ('2023-01-
 01'::timestamp) EXCLUSIVE EVERY (INTERVAL '1 day'), DEFAULT PARTITION extra );
 {% endset %} {{ config( materialized='table', distributed_by='id',
-appendonly='true', orientation='column', compresstype='ZLIB', compresslevel=1,
-blocksize=32768, fields_string=fields_string, raw_partition=raw_partition,
-default_partition_name='other_data' ) }} with source_data as ( select 1 as id,
-'2022-02-22'::timestamp as incomingdate union all select null as id, '2022-02-
-25'::timestamp as incomingdate ) select * from source_data ``` will produce
-following sql code ```SQL create table if not exists
-"database"."schema"."my_first_dbt_model__dbt_tmp" ( id int4 null, incomingdate
-timestamp NULL ) with ( appendonly=true, blocksize=32768, orientation=column,
-compresstype=ZLIB, compresslevel=1 ) DISTRIBUTED BY (id) PARTITION BY RANGE
-(incomingdate) ( START ('2021-01-01'::timestamp) INCLUSIVE END ('2023-01-01'::
-timestamp) EXCLUSIVE EVERY (INTERVAL '1 day'), DEFAULT PARTITION extra );
-insert into "database"."schema"."my_first_dbt_model__dbt_tmp" ( with
+appendoptimized=true, orientation='column', compresstype='ZLIB',
+compresslevel=1, blocksize=32768, fields_string=fields_string,
+raw_partition=raw_partition, default_partition_name='other_data' ) }} with
 source_data as ( select 1 as id, '2022-02-22'::timestamp as incomingdate union
 all select null as id, '2022-02-25'::timestamp as incomingdate ) select * from
-source_data ); alter table "dvault"."dv"."my_first_dbt_model" rename to
+source_data ``` will produce following sql code ```SQL create table if not
+exists "database"."schema"."my_first_dbt_model__dbt_tmp" ( id int4 null,
+incomingdate timestamp NULL ) with ( appendoptimized=true, blocksize=32768,
+orientation=column, compresstype=ZLIB, compresslevel=1 ) DISTRIBUTED BY (id)
+PARTITION BY RANGE (incomingdate) ( START ('2021-01-01'::timestamp) INCLUSIVE
+END ('2023-01-01'::timestamp) EXCLUSIVE EVERY (INTERVAL '1 day'), DEFAULT
+PARTITION extra ); insert into
+"database"."schema"."my_first_dbt_model__dbt_tmp" ( with source_data as
+( select 1 as id, '2022-02-22'::timestamp as incomingdate union all select null
+as id, '2022-02-25'::timestamp as incomingdate ) select * from source_data );
+alter table "dvault"."dv"."my_first_dbt_model" rename to
 "my_first_dbt_model__dbt_backup"; drop table if exists
 "dvault"."dv"."my_first_dbt_model__dbt_backup" cascade; alter table
 "database"."schema"."my_first_dbt_model__dbt_tmp" rename to
 "my_first_dbt_model"; ``` - Same result you can get using `partition_type`,
 `partition_column`, `partition_spec` parameters ```SQL {% set fields_string %}
 id int4 null, incomingdate timestamp NULL {% endset %} {%- set partition_type =
 'RANGE' -%} {%- set partition_column = 'incomingdate' -%} {% set partition_spec
 %} START ('2021-01-01'::timestamp) INCLUSIVE END ('2023-01-01'::timestamp)
 EXCLUSIVE EVERY (INTERVAL '1 day'), DEFAULT PARTITION extra {% endset %} {
-{ config( materialized='table', distributed_by='id', appendonly='true',
+{ config( materialized='table', distributed_by='id', appendoptimized=true,
 orientation='column', compresstype='ZLIB', compresslevel=1, blocksize=32768,
 fields_string=fields_string, partition_type=partition_type,
 partition_column=partition_column, partition_spec=partition_spec,
 default_partition_name='other_data' ) }} with source_data as ( select 1 as id,
 '2022-02-22'::timestamp as incomingdate union all select null as id, '2022-02-
 25'::timestamp as incomingdate ) select * from source_data ``` - also, you can
 use third way ```SQL {% set fields_string %} id int4 null, incomingdate
 timestamp NULL {% endset %} {%- set partition_type = 'RANGE' -%} {%- set
 partition_column = 'incomingdate' -%} {%- set partition_start = "'2021-01-01'::
 timestamp" -%} {%- set partition_end = "'2022-01-01'::timestamp" -%} {%- set
 partition_every = '1 day' -%} {{ config( materialized='table',
-distributed_by='id', appendonly='true', orientation='column',
+distributed_by='id', appendoptimized=true, orientation='column',
 compresstype='ZLIB', compresslevel=1, blocksize=32768,
 fields_string=fields_string, partition_type=partition_type,
 partition_column=partition_column, partition_start=partition_start,
 partition_end=partition_end, partition_every=partition_every,
 default_partition_name='other_data' ) }} with source_data as ( select 1 as id,
 '2022-02-22'::timestamp as incomingdate union all select null as id, '2022-02-
 25'::timestamp as incomingdate ) select * from source_data ``` - example of
```

### Comparing `dbt-greenplum-1.4.0/README.md` & `dbt-greenplum-1.5.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -26,36 +26,38 @@
 Where `<version>` is same as your dbt version
 
 Available versions:
  - 0.19.2
  - 1.0.4
  - 1.2.0
  - 1.4.0
+ - 1.5.0
 
 ## Supported Features
 
-You can specify following preference 
- - starage type
+You can specify following settings:
+ - Storage type
    - heap
    - appendoptimized
- - distribution
+ - Distribution
    - `distributed randomly` by defaut
    - `distributed by (column, [ ... ] )` by setting up `distributed_by` parameter in the model config
- - table orientation
+   - `distributed replicated` by setting up `distributed_replicated=true` parameter in the model config
+ - Table orientation
    - `orientation=colum` by default
    - `orientation=row` by setting up `orientation` parameter in `row` in the model config
- - compress type, level and blocksize with default values
+ - Compress type, level and blocksize with default values
    ```bash
-    blocksize=32768,
     compresstype=ZLIB,
-    compresslevel=1
+    compresslevel=1,
+    blocksize=32768
    ``` 
     You can also specify `blocksize`, `compresstype`, `compresslevel` in the model config
- - appendonly|appendoptimized preference by default is `true`, also you can override it by setting up `appendoptimized` field in the model config
- - partitions (see "partition" chapter below)
+ - `appendoptimized` preference by default is `true`, also you can override it by setting up `appendoptimized` field in the model config
+ - Partitions (see "Partition" chapter below)
 
 ### Heap table example
 
 To create heap table set `appendoptimized` parameter value to `false` 
 
 ```SQL
 {{
@@ -173,15 +175,15 @@
        );
    {% endset %}
 
    {{
        config(
            materialized='table',
            distributed_by='id',
-           appendonly='true',
+           appendoptimized=true,
            orientation='column',
            compresstype='ZLIB',
            compresslevel=1,
            blocksize=32768,
            fields_string=fields_string,
            raw_partition=raw_partition,
            default_partition_name='other_data'
@@ -204,15 +206,15 @@
    will produce following sql code
    ```SQL
    create table if not exists "database"."schema"."my_first_dbt_model__dbt_tmp" (
        id int4 null,
        incomingdate timestamp NULL
    )
    with (
-       appendonly=true,
+       appendoptimized=true,
        blocksize=32768,
        orientation=column,
        compresstype=ZLIB,
        compresslevel=1
    )
    DISTRIBUTED BY (id)
    PARTITION BY RANGE (incomingdate)
@@ -257,15 +259,15 @@
        DEFAULT PARTITION extra
    {% endset %}
    
    {{
        config(
            materialized='table',
            distributed_by='id',
-           appendonly='true',
+           appendoptimized=true,
            orientation='column',
            compresstype='ZLIB',
            compresslevel=1,
            blocksize=32768,
            fields_string=fields_string,
            partition_type=partition_type,
            partition_column=partition_column,
@@ -302,15 +304,15 @@
    {%- set partition_every = '1 day' -%}
    
    
    {{
        config(
            materialized='table',
            distributed_by='id',
-           appendonly='true',
+           appendoptimized=true,
            orientation='column',
            compresstype='ZLIB',
            compresslevel=1,
            blocksize=32768,
            fields_string=fields_string,
            partition_type=partition_type,
            partition_column=partition_column,
```

#### html2text {}

```diff
@@ -6,36 +6,38 @@
 filter, rename, and pre-aggregate the raw data in your warehouse so that it's
 ready for analysis. ## dbt-greenplum The `dbt-greenplum` package contains the
 code enabling dbt to work with Greenplum. This adapter based on [postgres-
 adapter](https://github.com/dbt-labs/dbt-core/blob/main/plugins/postgres/dbt/
 include/postgres/profile_template.yml) with a bit difference for a greenplum
 specific features ## Installation Easiest way to start use dbt-greenplum is to
 install it using pip `pip install dbt-greenplum==` Where `` is same as your dbt
-version Available versions: - 0.19.2 - 1.0.4 - 1.2.0 - 1.4.0 ## Supported
-Features You can specify following preference - starage type - heap -
-appendoptimized - distribution - `distributed randomly` by defaut -
+version Available versions: - 0.19.2 - 1.0.4 - 1.2.0 - 1.4.0 - 1.5.0 ##
+Supported Features You can specify following settings: - Storage type - heap -
+appendoptimized - Distribution - `distributed randomly` by defaut -
 `distributed by (column, [ ... ] )` by setting up `distributed_by` parameter in
-the model config - table orientation - `orientation=colum` by default -
-`orientation=row` by setting up `orientation` parameter in `row` in the model
-config - compress type, level and blocksize with default values ```bash
-blocksize=32768, compresstype=ZLIB, compresslevel=1 ``` You can also specify
-`blocksize`, `compresstype`, `compresslevel` in the model config -
-appendonly|appendoptimized preference by default is `true`, also you can
-override it by setting up `appendoptimized` field in the model config -
-partitions (see "partition" chapter below) ### Heap table example To create
-heap table set `appendoptimized` parameter value to `false` ```SQL {{ config
-( ... materialized='table', appendoptimized=false ... ) }} select 1 as "id" ```
-will produce following SQL code ```SQL create table "".""."" with
-( appendoptimized=false ) as ( select 1 as "id" ) DISTRIBUTED RANDOMLY; ``` ###
-Appendoptimized table example You can use `appendopimized` or `appendonly`
-(legacy) to create appendoptimized table Such model definition ```SQL {{ config
-( materialized='table', distributed_by='id', appendoptimized=true,
-orientation='column', compresstype='ZLIB', compresslevel=1, blocksize=32768 )
-}} with source_data as ( select 1 as id union all select null as id ) select *
-from source_data ``` will produce following sql code ```SQL create table
+the model config - `distributed replicated` by setting up
+`distributed_replicated=true` parameter in the model config - Table orientation
+- `orientation=colum` by default - `orientation=row` by setting up
+`orientation` parameter in `row` in the model config - Compress type, level and
+blocksize with default values ```bash compresstype=ZLIB, compresslevel=1,
+blocksize=32768 ``` You can also specify `blocksize`, `compresstype`,
+`compresslevel` in the model config - `appendoptimized` preference by default
+is `true`, also you can override it by setting up `appendoptimized` field in
+the model config - Partitions (see "Partition" chapter below) ### Heap table
+example To create heap table set `appendoptimized` parameter value to `false`
+```SQL {{ config( ... materialized='table', appendoptimized=false ... ) }}
+select 1 as "id" ``` will produce following SQL code ```SQL create table
+"".""."" with ( appendoptimized=false ) as ( select 1 as "id" ) DISTRIBUTED
+RANDOMLY; ``` ### Appendoptimized table example You can use `appendopimized` or
+`appendonly`(legacy) to create appendoptimized table Such model definition
+```SQL {{ config( materialized='table', distributed_by='id',
+appendoptimized=true, orientation='column', compresstype='ZLIB',
+compresslevel=1, blocksize=32768 ) }} with source_data as ( select 1 as id
+union all select null as id ) select * from source_data ``` will produce
+following sql code ```SQL create table
 "dvault"."dv"."my_first_dbt_model__dbt_tmp" with ( appendoptimized=true,
 blocksize=32768, orientation=column, compresstype=ZLIB, compresslevel=1 ) as
 ( with source_data as ( select 1 as id union all select null as id ) select *
 from source_data ) distributed by (id); alter table
 "dvault"."dv"."my_first_dbt_model__dbt_tmp" rename to "my_first_dbt_model"; ```
 ### Partitions Greenplum does not support partitions with `create table as`
 [construction](https://gpdb.docs.pivotal.io/6-9/ref_guide/sql_commands/
@@ -49,51 +51,52 @@
 `partition_values` - `default_partition_name` - name of default partition
 'other' by default Let consider examples of definition model with partitions -
 using `raw_partition` parameter ```SQL {% set fields_string %} id int4 null,
 incomingdate timestamp NULL {% endset %} {% set raw_partition %} PARTITION BY
 RANGE (incomingdate) ( START ('2021-01-01'::timestamp) INCLUSIVE END ('2023-01-
 01'::timestamp) EXCLUSIVE EVERY (INTERVAL '1 day'), DEFAULT PARTITION extra );
 {% endset %} {{ config( materialized='table', distributed_by='id',
-appendonly='true', orientation='column', compresstype='ZLIB', compresslevel=1,
-blocksize=32768, fields_string=fields_string, raw_partition=raw_partition,
-default_partition_name='other_data' ) }} with source_data as ( select 1 as id,
-'2022-02-22'::timestamp as incomingdate union all select null as id, '2022-02-
-25'::timestamp as incomingdate ) select * from source_data ``` will produce
-following sql code ```SQL create table if not exists
-"database"."schema"."my_first_dbt_model__dbt_tmp" ( id int4 null, incomingdate
-timestamp NULL ) with ( appendonly=true, blocksize=32768, orientation=column,
-compresstype=ZLIB, compresslevel=1 ) DISTRIBUTED BY (id) PARTITION BY RANGE
-(incomingdate) ( START ('2021-01-01'::timestamp) INCLUSIVE END ('2023-01-01'::
-timestamp) EXCLUSIVE EVERY (INTERVAL '1 day'), DEFAULT PARTITION extra );
-insert into "database"."schema"."my_first_dbt_model__dbt_tmp" ( with
+appendoptimized=true, orientation='column', compresstype='ZLIB',
+compresslevel=1, blocksize=32768, fields_string=fields_string,
+raw_partition=raw_partition, default_partition_name='other_data' ) }} with
 source_data as ( select 1 as id, '2022-02-22'::timestamp as incomingdate union
 all select null as id, '2022-02-25'::timestamp as incomingdate ) select * from
-source_data ); alter table "dvault"."dv"."my_first_dbt_model" rename to
+source_data ``` will produce following sql code ```SQL create table if not
+exists "database"."schema"."my_first_dbt_model__dbt_tmp" ( id int4 null,
+incomingdate timestamp NULL ) with ( appendoptimized=true, blocksize=32768,
+orientation=column, compresstype=ZLIB, compresslevel=1 ) DISTRIBUTED BY (id)
+PARTITION BY RANGE (incomingdate) ( START ('2021-01-01'::timestamp) INCLUSIVE
+END ('2023-01-01'::timestamp) EXCLUSIVE EVERY (INTERVAL '1 day'), DEFAULT
+PARTITION extra ); insert into
+"database"."schema"."my_first_dbt_model__dbt_tmp" ( with source_data as
+( select 1 as id, '2022-02-22'::timestamp as incomingdate union all select null
+as id, '2022-02-25'::timestamp as incomingdate ) select * from source_data );
+alter table "dvault"."dv"."my_first_dbt_model" rename to
 "my_first_dbt_model__dbt_backup"; drop table if exists
 "dvault"."dv"."my_first_dbt_model__dbt_backup" cascade; alter table
 "database"."schema"."my_first_dbt_model__dbt_tmp" rename to
 "my_first_dbt_model"; ``` - Same result you can get using `partition_type`,
 `partition_column`, `partition_spec` parameters ```SQL {% set fields_string %}
 id int4 null, incomingdate timestamp NULL {% endset %} {%- set partition_type =
 'RANGE' -%} {%- set partition_column = 'incomingdate' -%} {% set partition_spec
 %} START ('2021-01-01'::timestamp) INCLUSIVE END ('2023-01-01'::timestamp)
 EXCLUSIVE EVERY (INTERVAL '1 day'), DEFAULT PARTITION extra {% endset %} {
-{ config( materialized='table', distributed_by='id', appendonly='true',
+{ config( materialized='table', distributed_by='id', appendoptimized=true,
 orientation='column', compresstype='ZLIB', compresslevel=1, blocksize=32768,
 fields_string=fields_string, partition_type=partition_type,
 partition_column=partition_column, partition_spec=partition_spec,
 default_partition_name='other_data' ) }} with source_data as ( select 1 as id,
 '2022-02-22'::timestamp as incomingdate union all select null as id, '2022-02-
 25'::timestamp as incomingdate ) select * from source_data ``` - also, you can
 use third way ```SQL {% set fields_string %} id int4 null, incomingdate
 timestamp NULL {% endset %} {%- set partition_type = 'RANGE' -%} {%- set
 partition_column = 'incomingdate' -%} {%- set partition_start = "'2021-01-01'::
 timestamp" -%} {%- set partition_end = "'2022-01-01'::timestamp" -%} {%- set
 partition_every = '1 day' -%} {{ config( materialized='table',
-distributed_by='id', appendonly='true', orientation='column',
+distributed_by='id', appendoptimized=true, orientation='column',
 compresstype='ZLIB', compresslevel=1, blocksize=32768,
 fields_string=fields_string, partition_type=partition_type,
 partition_column=partition_column, partition_start=partition_start,
 partition_end=partition_end, partition_every=partition_every,
 default_partition_name='other_data' ) }} with source_data as ( select 1 as id,
 '2022-02-22'::timestamp as incomingdate union all select null as id, '2022-02-
 25'::timestamp as incomingdate ) select * from source_data ``` - example of
```

### Comparing `dbt-greenplum-1.4.0/dbt/include/greenplum/macros/adapters.sql` & `dbt-greenplum-1.5.0/dbt/include/greenplum/macros/adapters.sql`

 * *Files 5% similar despite different names*

```diff
@@ -55,14 +55,20 @@
       {{ storage_parameters(appendoptimized, blocksize, orientation, compresstype, compresslevel) }}
       as (
         {{ sql }}
       )
       {{ distribution(distributed_by, distributed_replicated) }}
       ;
   {% endif %}
+
+  {% set contract_config = config.get('contract') %}
+  {% if contract_config.enforced %}
+     {{exceptions.warn("Model contracts cannot be enforced by dbt-greenplum!")}}
+  {% endif %}
+
 {%- endmacro %}
 
 
 {% macro greenplum__get_create_index_sql(relation, index_dict) -%}
   {{ return(postgres__get_create_index_sql(relation, index_dict)) }}
 {%- endmacro %}
```

### Comparing `dbt-greenplum-1.4.0/dbt/include/greenplum/macros/partitions.sql` & `dbt-greenplum-1.5.0/dbt/include/greenplum/macros/partitions.sql`

 * *Files identical despite different names*

### Comparing `dbt-greenplum-1.4.0/dbt_greenplum.egg-info/PKG-INFO` & `dbt-greenplum-1.5.0/dbt_greenplum.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dbt-greenplum
-Version: 1.4.0
+Version: 1.5.0
 Summary: The greenplum adapter plugin for dbt (data build tool)
 Home-page: https://github.com/markporoshin/dbt-greenplum
 Author: Mark Poroshin
 Author-email: mark.poroshin@yandex.ru
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Development Status :: 5 - Production/Stable
@@ -48,36 +48,38 @@
 Where `<version>` is same as your dbt version
 
 Available versions:
  - 0.19.2
  - 1.0.4
  - 1.2.0
  - 1.4.0
+ - 1.5.0
 
 ## Supported Features
 
-You can specify following preference 
- - starage type
+You can specify following settings:
+ - Storage type
    - heap
    - appendoptimized
- - distribution
+ - Distribution
    - `distributed randomly` by defaut
    - `distributed by (column, [ ... ] )` by setting up `distributed_by` parameter in the model config
- - table orientation
+   - `distributed replicated` by setting up `distributed_replicated=true` parameter in the model config
+ - Table orientation
    - `orientation=colum` by default
    - `orientation=row` by setting up `orientation` parameter in `row` in the model config
- - compress type, level and blocksize with default values
+ - Compress type, level and blocksize with default values
    ```bash
-    blocksize=32768,
     compresstype=ZLIB,
-    compresslevel=1
+    compresslevel=1,
+    blocksize=32768
    ``` 
     You can also specify `blocksize`, `compresstype`, `compresslevel` in the model config
- - appendonly|appendoptimized preference by default is `true`, also you can override it by setting up `appendoptimized` field in the model config
- - partitions (see "partition" chapter below)
+ - `appendoptimized` preference by default is `true`, also you can override it by setting up `appendoptimized` field in the model config
+ - Partitions (see "Partition" chapter below)
 
 ### Heap table example
 
 To create heap table set `appendoptimized` parameter value to `false` 
 
 ```SQL
 {{
@@ -195,15 +197,15 @@
        );
    {% endset %}
 
    {{
        config(
            materialized='table',
            distributed_by='id',
-           appendonly='true',
+           appendoptimized=true,
            orientation='column',
            compresstype='ZLIB',
            compresslevel=1,
            blocksize=32768,
            fields_string=fields_string,
            raw_partition=raw_partition,
            default_partition_name='other_data'
@@ -226,15 +228,15 @@
    will produce following sql code
    ```SQL
    create table if not exists "database"."schema"."my_first_dbt_model__dbt_tmp" (
        id int4 null,
        incomingdate timestamp NULL
    )
    with (
-       appendonly=true,
+       appendoptimized=true,
        blocksize=32768,
        orientation=column,
        compresstype=ZLIB,
        compresslevel=1
    )
    DISTRIBUTED BY (id)
    PARTITION BY RANGE (incomingdate)
@@ -279,15 +281,15 @@
        DEFAULT PARTITION extra
    {% endset %}
    
    {{
        config(
            materialized='table',
            distributed_by='id',
-           appendonly='true',
+           appendoptimized=true,
            orientation='column',
            compresstype='ZLIB',
            compresslevel=1,
            blocksize=32768,
            fields_string=fields_string,
            partition_type=partition_type,
            partition_column=partition_column,
@@ -324,15 +326,15 @@
    {%- set partition_every = '1 day' -%}
    
    
    {{
        config(
            materialized='table',
            distributed_by='id',
-           appendonly='true',
+           appendoptimized=true,
            orientation='column',
            compresstype='ZLIB',
            compresslevel=1,
            blocksize=32768,
            fields_string=fields_string,
            partition_type=partition_type,
            partition_column=partition_column,
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: dbt-greenplum Version: 1.4.0 Summary: The greenplum
+Metadata-Version: 2.1 Name: dbt-greenplum Version: 1.5.0 Summary: The greenplum
 adapter plugin for dbt (data build tool) Home-page: https://github.com/
 markporoshin/dbt-greenplum Author: Mark Poroshin Author-email:
 mark.poroshin@yandex.ru License: UNKNOWN Platform: UNKNOWN Classifier:
 Development Status :: 5 - Production/Stable Classifier: License :: OSI Approved
 :: Apache Software License Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: MacOS :: MacOS X Classifier: Operating System
 :: POSIX :: Linux Classifier: Programming Language :: Python :: 3.7 Classifier:
@@ -18,36 +18,38 @@
 filter, rename, and pre-aggregate the raw data in your warehouse so that it's
 ready for analysis. ## dbt-greenplum The `dbt-greenplum` package contains the
 code enabling dbt to work with Greenplum. This adapter based on [postgres-
 adapter](https://github.com/dbt-labs/dbt-core/blob/main/plugins/postgres/dbt/
 include/postgres/profile_template.yml) with a bit difference for a greenplum
 specific features ## Installation Easiest way to start use dbt-greenplum is to
 install it using pip `pip install dbt-greenplum==` Where `` is same as your dbt
-version Available versions: - 0.19.2 - 1.0.4 - 1.2.0 - 1.4.0 ## Supported
-Features You can specify following preference - starage type - heap -
-appendoptimized - distribution - `distributed randomly` by defaut -
+version Available versions: - 0.19.2 - 1.0.4 - 1.2.0 - 1.4.0 - 1.5.0 ##
+Supported Features You can specify following settings: - Storage type - heap -
+appendoptimized - Distribution - `distributed randomly` by defaut -
 `distributed by (column, [ ... ] )` by setting up `distributed_by` parameter in
-the model config - table orientation - `orientation=colum` by default -
-`orientation=row` by setting up `orientation` parameter in `row` in the model
-config - compress type, level and blocksize with default values ```bash
-blocksize=32768, compresstype=ZLIB, compresslevel=1 ``` You can also specify
-`blocksize`, `compresstype`, `compresslevel` in the model config -
-appendonly|appendoptimized preference by default is `true`, also you can
-override it by setting up `appendoptimized` field in the model config -
-partitions (see "partition" chapter below) ### Heap table example To create
-heap table set `appendoptimized` parameter value to `false` ```SQL {{ config
-( ... materialized='table', appendoptimized=false ... ) }} select 1 as "id" ```
-will produce following SQL code ```SQL create table "".""."" with
-( appendoptimized=false ) as ( select 1 as "id" ) DISTRIBUTED RANDOMLY; ``` ###
-Appendoptimized table example You can use `appendopimized` or `appendonly`
-(legacy) to create appendoptimized table Such model definition ```SQL {{ config
-( materialized='table', distributed_by='id', appendoptimized=true,
-orientation='column', compresstype='ZLIB', compresslevel=1, blocksize=32768 )
-}} with source_data as ( select 1 as id union all select null as id ) select *
-from source_data ``` will produce following sql code ```SQL create table
+the model config - `distributed replicated` by setting up
+`distributed_replicated=true` parameter in the model config - Table orientation
+- `orientation=colum` by default - `orientation=row` by setting up
+`orientation` parameter in `row` in the model config - Compress type, level and
+blocksize with default values ```bash compresstype=ZLIB, compresslevel=1,
+blocksize=32768 ``` You can also specify `blocksize`, `compresstype`,
+`compresslevel` in the model config - `appendoptimized` preference by default
+is `true`, also you can override it by setting up `appendoptimized` field in
+the model config - Partitions (see "Partition" chapter below) ### Heap table
+example To create heap table set `appendoptimized` parameter value to `false`
+```SQL {{ config( ... materialized='table', appendoptimized=false ... ) }}
+select 1 as "id" ``` will produce following SQL code ```SQL create table
+"".""."" with ( appendoptimized=false ) as ( select 1 as "id" ) DISTRIBUTED
+RANDOMLY; ``` ### Appendoptimized table example You can use `appendopimized` or
+`appendonly`(legacy) to create appendoptimized table Such model definition
+```SQL {{ config( materialized='table', distributed_by='id',
+appendoptimized=true, orientation='column', compresstype='ZLIB',
+compresslevel=1, blocksize=32768 ) }} with source_data as ( select 1 as id
+union all select null as id ) select * from source_data ``` will produce
+following sql code ```SQL create table
 "dvault"."dv"."my_first_dbt_model__dbt_tmp" with ( appendoptimized=true,
 blocksize=32768, orientation=column, compresstype=ZLIB, compresslevel=1 ) as
 ( with source_data as ( select 1 as id union all select null as id ) select *
 from source_data ) distributed by (id); alter table
 "dvault"."dv"."my_first_dbt_model__dbt_tmp" rename to "my_first_dbt_model"; ```
 ### Partitions Greenplum does not support partitions with `create table as`
 [construction](https://gpdb.docs.pivotal.io/6-9/ref_guide/sql_commands/
@@ -61,51 +63,52 @@
 `partition_values` - `default_partition_name` - name of default partition
 'other' by default Let consider examples of definition model with partitions -
 using `raw_partition` parameter ```SQL {% set fields_string %} id int4 null,
 incomingdate timestamp NULL {% endset %} {% set raw_partition %} PARTITION BY
 RANGE (incomingdate) ( START ('2021-01-01'::timestamp) INCLUSIVE END ('2023-01-
 01'::timestamp) EXCLUSIVE EVERY (INTERVAL '1 day'), DEFAULT PARTITION extra );
 {% endset %} {{ config( materialized='table', distributed_by='id',
-appendonly='true', orientation='column', compresstype='ZLIB', compresslevel=1,
-blocksize=32768, fields_string=fields_string, raw_partition=raw_partition,
-default_partition_name='other_data' ) }} with source_data as ( select 1 as id,
-'2022-02-22'::timestamp as incomingdate union all select null as id, '2022-02-
-25'::timestamp as incomingdate ) select * from source_data ``` will produce
-following sql code ```SQL create table if not exists
-"database"."schema"."my_first_dbt_model__dbt_tmp" ( id int4 null, incomingdate
-timestamp NULL ) with ( appendonly=true, blocksize=32768, orientation=column,
-compresstype=ZLIB, compresslevel=1 ) DISTRIBUTED BY (id) PARTITION BY RANGE
-(incomingdate) ( START ('2021-01-01'::timestamp) INCLUSIVE END ('2023-01-01'::
-timestamp) EXCLUSIVE EVERY (INTERVAL '1 day'), DEFAULT PARTITION extra );
-insert into "database"."schema"."my_first_dbt_model__dbt_tmp" ( with
+appendoptimized=true, orientation='column', compresstype='ZLIB',
+compresslevel=1, blocksize=32768, fields_string=fields_string,
+raw_partition=raw_partition, default_partition_name='other_data' ) }} with
 source_data as ( select 1 as id, '2022-02-22'::timestamp as incomingdate union
 all select null as id, '2022-02-25'::timestamp as incomingdate ) select * from
-source_data ); alter table "dvault"."dv"."my_first_dbt_model" rename to
+source_data ``` will produce following sql code ```SQL create table if not
+exists "database"."schema"."my_first_dbt_model__dbt_tmp" ( id int4 null,
+incomingdate timestamp NULL ) with ( appendoptimized=true, blocksize=32768,
+orientation=column, compresstype=ZLIB, compresslevel=1 ) DISTRIBUTED BY (id)
+PARTITION BY RANGE (incomingdate) ( START ('2021-01-01'::timestamp) INCLUSIVE
+END ('2023-01-01'::timestamp) EXCLUSIVE EVERY (INTERVAL '1 day'), DEFAULT
+PARTITION extra ); insert into
+"database"."schema"."my_first_dbt_model__dbt_tmp" ( with source_data as
+( select 1 as id, '2022-02-22'::timestamp as incomingdate union all select null
+as id, '2022-02-25'::timestamp as incomingdate ) select * from source_data );
+alter table "dvault"."dv"."my_first_dbt_model" rename to
 "my_first_dbt_model__dbt_backup"; drop table if exists
 "dvault"."dv"."my_first_dbt_model__dbt_backup" cascade; alter table
 "database"."schema"."my_first_dbt_model__dbt_tmp" rename to
 "my_first_dbt_model"; ``` - Same result you can get using `partition_type`,
 `partition_column`, `partition_spec` parameters ```SQL {% set fields_string %}
 id int4 null, incomingdate timestamp NULL {% endset %} {%- set partition_type =
 'RANGE' -%} {%- set partition_column = 'incomingdate' -%} {% set partition_spec
 %} START ('2021-01-01'::timestamp) INCLUSIVE END ('2023-01-01'::timestamp)
 EXCLUSIVE EVERY (INTERVAL '1 day'), DEFAULT PARTITION extra {% endset %} {
-{ config( materialized='table', distributed_by='id', appendonly='true',
+{ config( materialized='table', distributed_by='id', appendoptimized=true,
 orientation='column', compresstype='ZLIB', compresslevel=1, blocksize=32768,
 fields_string=fields_string, partition_type=partition_type,
 partition_column=partition_column, partition_spec=partition_spec,
 default_partition_name='other_data' ) }} with source_data as ( select 1 as id,
 '2022-02-22'::timestamp as incomingdate union all select null as id, '2022-02-
 25'::timestamp as incomingdate ) select * from source_data ``` - also, you can
 use third way ```SQL {% set fields_string %} id int4 null, incomingdate
 timestamp NULL {% endset %} {%- set partition_type = 'RANGE' -%} {%- set
 partition_column = 'incomingdate' -%} {%- set partition_start = "'2021-01-01'::
 timestamp" -%} {%- set partition_end = "'2022-01-01'::timestamp" -%} {%- set
 partition_every = '1 day' -%} {{ config( materialized='table',
-distributed_by='id', appendonly='true', orientation='column',
+distributed_by='id', appendoptimized=true, orientation='column',
 compresstype='ZLIB', compresslevel=1, blocksize=32768,
 fields_string=fields_string, partition_type=partition_type,
 partition_column=partition_column, partition_start=partition_start,
 partition_end=partition_end, partition_every=partition_every,
 default_partition_name='other_data' ) }} with source_data as ( select 1 as id,
 '2022-02-22'::timestamp as incomingdate union all select null as id, '2022-02-
 25'::timestamp as incomingdate ) select * from source_data ``` - example of
```

### Comparing `dbt-greenplum-1.4.0/dbt_greenplum.egg-info/SOURCES.txt` & `dbt-greenplum-1.5.0/dbt_greenplum.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `dbt-greenplum-1.4.0/setup.py` & `dbt-greenplum-1.5.0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -95,15 +95,15 @@
             "include/greenplum/sample_profiles.yml",
             "include/greenplum/macros/*.sql",
             "include/greenplum/macros/**/*.sql",
         ]
     },
     install_requires=[
         "dbt-core~={}".format(dbt_core_version),
-        "dbt-postgres=={}".format(package_version),
+        "dbt-postgres~={}".format(package_version),
         "{}~=2.8".format(DBT_PSYCOPG2_NAME),
     ],
     zip_safe=False,
     classifiers=[
         "Development Status :: 5 - Production/Stable",
         "License :: OSI Approved :: Apache Software License",
         "Operating System :: Microsoft :: Windows",
```

