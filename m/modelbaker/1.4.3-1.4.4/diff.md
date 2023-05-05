# Comparing `tmp/modelbaker-1.4.3.tar.gz` & `tmp/modelbaker-1.4.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "modelbaker-1.4.3.tar", last modified: Thu Apr  6 07:32:41 2023, max compression
+gzip compressed data, was "modelbaker-1.4.4.tar", last modified: Fri May  5 13:56:13 2023, max compression
```

## Comparing `modelbaker-1.4.3.tar` & `modelbaker-1.4.4.tar`

### file list

```diff
@@ -1,120 +1,121 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 07:32:41.904065 modelbaker-1.4.3/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-04-06 07:32:28.000000 modelbaker-1.4.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3506 2023-04-06 07:32:41.904065 modelbaker-1.4.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2955 2023-04-06 07:32:28.000000 modelbaker-1.4.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 07:32:41.888064 modelbaker-1.4.3/modelbaker/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-06 07:32:28.000000 modelbaker-1.4.3/modelbaker/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 07:32:41.888064 modelbaker-1.4.3/modelbaker/dataobjects/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-06 07:32:28.000000 modelbaker-1.4.3/modelbaker/dataobjects/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2156 2023-04-06 07:32:28.000000 modelbaker-1.4.3/modelbaker/dataobjects/fields.py
--rw-r--r--   0 runner    (1001) docker     (123)     5050 2023-04-06 07:32:28.000000 modelbaker-1.4.3/modelbaker/dataobjects/form.py
--rw-r--r--   0 runner    (1001) docker     (123)    13081 2023-04-06 07:32:28.000000 modelbaker-1.4.3/modelbaker/dataobjects/layers.py
--rw-r--r--   0 runner    (1001) docker     (123)     4520 2023-04-06 07:32:28.000000 modelbaker-1.4.3/modelbaker/dataobjects/legend.py
--rw-r--r--   0 runner    (1001) docker     (123)    15631 2023-04-06 07:32:28.000000 modelbaker-1.4.3/modelbaker/dataobjects/project.py
--rw-r--r--   0 runner    (1001) docker     (123)     2334 2023-04-06 07:32:28.000000 modelbaker-1.4.3/modelbaker/dataobjects/relations.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 07:32:41.892064 modelbaker-1.4.3/modelbaker/db_factory/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-06 07:32:28.000000 modelbaker-1.4.3/modelbaker/db_factory/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3705 2023-04-06 07:32:28.000000 modelbaker-1.4.3/modelbaker/db_factory/db_command_config_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     4370 2023-04-06 07:32:28.000000 modelbaker-1.4.3/modelbaker/db_factory/db_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     3433 2023-04-06 07:32:28.000000 modelbaker-1.4.3/modelbaker/db_factory/db_simple_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     2092 2023-04-06 07:32:28.000000 modelbaker-1.4.3/modelbaker/db_factory/gpkg_command_config_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     1874 2023-04-06 07:32:28.000000 modelbaker-1.4.3/modelbaker/db_factory/gpkg_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     1531 2023-04-06 07:32:28.000000 modelbaker-1.4.3/modelbaker/db_factory/gpkg_layer_uri.py
--rw-r--r--   0 runner    (1001) docker     (123)     1815 2023-04-06 07:32:28.000000 modelbaker-1.4.3/modelbaker/db_factory/layer_uri.py
--rw-r--r--   0 runner    (1001) docker     (123)     4603 2023-04-06 07:32:28.000000 modelbaker-1.4.3/modelbaker/db_factory/mssql_command_config_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     1924 2023-04-06 07:32:28.000000 modelbaker-1.4.3/modelbaker/db_factory/mssql_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     2760 2023-04-06 07:32:28.000000 modelbaker-1.4.3/modelbaker/db_factory/mssql_layer_uri.py
--rw-r--r--   0 runner    (1001) docker     (123)     7981 2023-04-06 07:32:28.000000 modelbaker-1.4.3/modelbaker/db_factory/pg_command_config_manager.py
--rw-r--r--   0 runner    (1001) docker     (123)     3345 2023-04-06 07:32:28.000000 modelbaker-1.4.3/modelbaker/db_factory/pg_factory.py
--rw-r--r--   0 runner    (1001) docker     (123)     2508 2023-04-06 07:32:28.000000 modelbaker-1.4.3/modelbaker/db_factory/pg_layer_uri.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 07:32:41.892064 modelbaker-1.4.3/modelbaker/dbconnector/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-06 07:32:28.000000 modelbaker-1.4.3/modelbaker/dbconnector/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1966 2023-04-06 07:32:28.000000 modelbaker-1.4.3/modelbaker/dbconnector/config.py
--rw-r--r--   0 runner    (1001) docker     (123)    12596 2023-04-06 07:32:28.000000 modelbaker-1.4.3/modelbaker/dbconnector/db_connector.py
--rw-r--r--   0 runner    (1001) docker     (123)    36134 2023-04-06 07:32:28.000000 modelbaker-1.4.3/modelbaker/dbconnector/gpkg_connector.py
--rw-r--r--   0 runner    (1001) docker     (123)    38036 2023-04-06 07:32:28.000000 modelbaker-1.4.3/modelbaker/dbconnector/mssql_connector.py
--rw-r--r--   0 runner    (1001) docker     (123)    42595 2023-04-06 07:32:28.000000 modelbaker-1.4.3/modelbaker/dbconnector/pg_connector.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 07:32:41.892064 modelbaker-1.4.3/modelbaker/generator/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-06 07:32:28.000000 modelbaker-1.4.3/modelbaker/generator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      692 2023-04-06 07:32:28.000000 modelbaker-1.4.3/modelbaker/generator/config.py
--rw-r--r--   0 runner    (1001) docker     (123)    50554 2023-04-06 07:32:28.000000 modelbaker-1.4.3/modelbaker/generator/domain_relations_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)    30620 2023-04-06 07:32:28.000000 modelbaker-1.4.3/modelbaker/generator/generator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 07:32:41.892064 modelbaker-1.4.3/modelbaker/ilitoppingmaker/
--rw-r--r--   0 runner    (1001) docker     (123)     1251 2023-04-06 07:32:28.000000 modelbaker-1.4.3/modelbaker/ilitoppingmaker/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5494 2023-04-06 07:32:28.000000 modelbaker-1.4.3/modelbaker/ilitoppingmaker/ili2dbsettings.py
--rw-r--r--   0 runner    (1001) docker     (123)     6724 2023-04-06 07:32:28.000000 modelbaker-1.4.3/modelbaker/ilitoppingmaker/ilidata.py
--rw-r--r--   0 runner    (1001) docker     (123)     4211 2023-04-06 07:32:28.000000 modelbaker-1.4.3/modelbaker/ilitoppingmaker/iliprojecttopping.py
--rw-r--r--   0 runner    (1001) docker     (123)     3266 2023-04-06 07:32:28.000000 modelbaker-1.4.3/modelbaker/ilitoppingmaker/ilitarget.py
--rw-r--r--   0 runner    (1001) docker     (123)     6067 2023-04-06 07:32:28.000000 modelbaker-1.4.3/modelbaker/ilitoppingmaker/metaconfig.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 07:32:41.896064 modelbaker-1.4.3/modelbaker/iliwrapper/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-06 07:32:28.000000 modelbaker-1.4.3/modelbaker/iliwrapper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1200 2023-04-06 07:32:28.000000 modelbaker-1.4.3/modelbaker/iliwrapper/globals.py
--rw-r--r--   0 runner    (1001) docker     (123)     4537 2023-04-06 07:32:28.000000 modelbaker-1.4.3/modelbaker/iliwrapper/ili2dbargs.py
--rw-r--r--   0 runner    (1001) docker     (123)    16442 2023-04-06 07:32:28.000000 modelbaker-1.4.3/modelbaker/iliwrapper/ili2dbconfig.py
--rw-r--r--   0 runner    (1001) docker     (123)     2182 2023-04-06 07:32:28.000000 modelbaker-1.4.3/modelbaker/iliwrapper/ili2dbtools.py
--rw-r--r--   0 runner    (1001) docker     (123)    13089 2023-04-06 07:32:28.000000 modelbaker-1.4.3/modelbaker/iliwrapper/ili2dbutils.py
--rw-r--r--   0 runner    (1001) docker     (123)    38165 2023-04-06 07:32:28.000000 modelbaker-1.4.3/modelbaker/iliwrapper/ilicache.py
--rw-r--r--   0 runner    (1001) docker     (123)     6182 2023-04-06 07:32:28.000000 modelbaker-1.4.3/modelbaker/iliwrapper/iliexecutable.py
--rw-r--r--   0 runner    (1001) docker     (123)     1638 2023-04-06 07:32:28.000000 modelbaker-1.4.3/modelbaker/iliwrapper/iliexporter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1578 2023-04-06 07:32:28.000000 modelbaker-1.4.3/modelbaker/iliwrapper/iliimporter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1326 2023-04-06 07:32:28.000000 modelbaker-1.4.3/modelbaker/iliwrapper/iliupdater.py
--rw-r--r--   0 runner    (1001) docker     (123)     5894 2023-04-06 07:32:28.000000 modelbaker-1.4.3/modelbaker/iliwrapper/ilivalidator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 07:32:41.896064 modelbaker-1.4.3/modelbaker/libs/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-06 07:32:31.000000 modelbaker-1.4.3/modelbaker/libs/__init__.py
--rw-rw-r--   0 runner    (1001) docker     (123)    12895 2020-04-20 14:21:10.000000 modelbaker-1.4.3/modelbaker/libs/deprecation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 07:32:41.896064 modelbaker-1.4.3/modelbaker/libs/packaging/
--rw-rw-r--   0 runner    (1001) docker     (123)      501 2023-01-08 18:18:22.000000 modelbaker-1.4.3/modelbaker/libs/packaging/__init__.py
--rw-rw-r--   0 runner    (1001) docker     (123)     3266 2023-01-08 18:00:18.000000 modelbaker-1.4.3/modelbaker/libs/packaging/_elffile.py
--rw-rw-r--   0 runner    (1001) docker     (123)     8813 2022-12-08 23:11:50.000000 modelbaker-1.4.3/modelbaker/libs/packaging/_manylinux.py
--rw-rw-r--   0 runner    (1001) docker     (123)     2524 2022-12-08 23:11:50.000000 modelbaker-1.4.3/modelbaker/libs/packaging/_musllinux.py
--rw-rw-r--   0 runner    (1001) docker     (123)     9399 2023-01-08 18:00:18.000000 modelbaker-1.4.3/modelbaker/libs/packaging/_parser.py
--rw-rw-r--   0 runner    (1001) docker     (123)     1431 2022-12-08 23:11:50.000000 modelbaker-1.4.3/modelbaker/libs/packaging/_structures.py
--rw-rw-r--   0 runner    (1001) docker     (123)     5148 2022-12-13 07:03:34.000000 modelbaker-1.4.3/modelbaker/libs/packaging/_tokenizer.py
--rw-rw-r--   0 runner    (1001) docker     (123)     8161 2022-12-27 15:22:44.000000 modelbaker-1.4.3/modelbaker/libs/packaging/markers.py
--rw-rw-r--   0 runner    (1001) docker     (123)     3264 2022-12-08 23:11:50.000000 modelbaker-1.4.3/modelbaker/libs/packaging/requirements.py
--rw-rw-r--   0 runner    (1001) docker     (123)    39046 2023-01-08 18:00:18.000000 modelbaker-1.4.3/modelbaker/libs/packaging/specifiers.py
--rw-rw-r--   0 runner    (1001) docker     (123)    18065 2022-12-26 19:52:02.000000 modelbaker-1.4.3/modelbaker/libs/packaging/tags.py
--rw-rw-r--   0 runner    (1001) docker     (123)     4355 2022-12-08 23:11:50.000000 modelbaker-1.4.3/modelbaker/libs/packaging/utils.py
--rw-rw-r--   0 runner    (1001) docker     (123)    16295 2022-12-08 23:11:50.000000 modelbaker-1.4.3/modelbaker/libs/packaging/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 07:32:41.896064 modelbaker-1.4.3/modelbaker/libs/pgserviceparser/
--rw-rw-r--   0 runner    (1001) docker     (123)     1801 2022-06-27 10:25:36.000000 modelbaker-1.4.3/modelbaker/libs/pgserviceparser/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 07:32:41.900064 modelbaker-1.4.3/modelbaker/libs/toppingmaker/
--rw-rw-r--   0 runner    (1001) docker     (123)     1152 2022-12-16 08:01:28.000000 modelbaker-1.4.3/modelbaker/libs/toppingmaker/__init__.py
--rw-rw-r--   0 runner    (1001) docker     (123)     6582 2022-12-16 08:01:28.000000 modelbaker-1.4.3/modelbaker/libs/toppingmaker/exportsettings.py
--rw-rw-r--   0 runner    (1001) docker     (123)    26523 2022-12-16 08:01:28.000000 modelbaker-1.4.3/modelbaker/libs/toppingmaker/projecttopping.py
--rw-rw-r--   0 runner    (1001) docker     (123)     3366 2022-12-16 08:01:28.000000 modelbaker-1.4.3/modelbaker/libs/toppingmaker/target.py
--rw-rw-r--   0 runner    (1001) docker     (123)     1321 2022-12-16 08:01:28.000000 modelbaker-1.4.3/modelbaker/libs/toppingmaker/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 07:32:41.900064 modelbaker-1.4.3/modelbaker/utils/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-06 07:32:28.000000 modelbaker-1.4.3/modelbaker/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6394 2023-04-06 07:32:28.000000 modelbaker-1.4.3/modelbaker/utils/db_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1205 2023-04-06 07:32:28.000000 modelbaker-1.4.3/modelbaker/utils/globals.py
--rw-r--r--   0 runner    (1001) docker     (123)     4684 2023-04-06 07:32:28.000000 modelbaker-1.4.3/modelbaker/utils/qgis_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    10267 2023-04-06 07:32:28.000000 modelbaker-1.4.3/modelbaker/utils/qt_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 07:32:41.888064 modelbaker-1.4.3/modelbaker.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3506 2023-04-06 07:32:41.000000 modelbaker-1.4.3/modelbaker.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3545 2023-04-06 07:32:41.000000 modelbaker-1.4.3/modelbaker.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-06 07:32:41.000000 modelbaker-1.4.3/modelbaker.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-04-06 07:32:41.000000 modelbaker-1.4.3/modelbaker.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-06 07:32:41.904065 modelbaker-1.4.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      874 2023-04-06 07:32:28.000000 modelbaker-1.4.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 07:32:41.900064 modelbaker-1.4.3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)    12580 2023-04-06 07:32:28.000000 modelbaker-1.4.3/tests/test_dataset_handling.py
--rw-r--r--   0 runner    (1001) docker     (123)   151890 2023-04-06 07:32:28.000000 modelbaker-1.4.3/tests/test_domain_class_relations.py
--rw-r--r--   0 runner    (1001) docker     (123)     2831 2023-04-06 07:32:28.000000 modelbaker-1.4.3/tests/test_dump.py
--rw-r--r--   0 runner    (1001) docker     (123)    39104 2023-04-06 07:32:28.000000 modelbaker-1.4.3/tests/test_export.py
--rw-r--r--   0 runner    (1001) docker     (123)     3425 2023-04-06 07:32:28.000000 modelbaker-1.4.3/tests/test_get_models.py
--rw-r--r--   0 runner    (1001) docker     (123)     6555 2023-04-06 07:32:28.000000 modelbaker-1.4.3/tests/test_gpkg_pk.py
--rw-r--r--   0 runner    (1001) docker     (123)     2517 2023-04-06 07:32:28.000000 modelbaker-1.4.3/tests/test_ili2dbutils.py
--rw-r--r--   0 runner    (1001) docker     (123)    28912 2023-04-06 07:32:28.000000 modelbaker-1.4.3/tests/test_ilicache.py
--rw-r--r--   0 runner    (1001) docker     (123)    13620 2023-04-06 07:32:28.000000 modelbaker-1.4.3/tests/test_ilitoppingmaker.py
--rw-r--r--   0 runner    (1001) docker     (123)    17928 2023-04-06 07:32:28.000000 modelbaker-1.4.3/tests/test_import.py
--rw-r--r--   0 runner    (1001) docker     (123)      529 2023-04-06 07:32:28.000000 modelbaker-1.4.3/tests/test_libili2pg.py
--rw-r--r--   0 runner    (1001) docker     (123)    14531 2023-04-06 07:32:28.000000 modelbaker-1.4.3/tests/test_metaconfig.py
--rw-r--r--   0 runner    (1001) docker     (123)    11343 2023-04-06 07:32:28.000000 modelbaker-1.4.3/tests/test_pgservice.py
--rw-r--r--   0 runner    (1001) docker     (123)     1008 2023-04-06 07:32:28.000000 modelbaker-1.4.3/tests/test_plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)   166117 2023-04-06 07:32:28.000000 modelbaker-1.4.3/tests/test_projectgen.py
--rw-r--r--   0 runner    (1001) docker     (123)    15529 2023-04-06 07:32:28.000000 modelbaker-1.4.3/tests/test_projectgen_generic_databases.py
--rw-r--r--   0 runner    (1001) docker     (123)    51448 2023-04-06 07:32:28.000000 modelbaker-1.4.3/tests/test_projecttopping.py
--rw-r--r--   0 runner    (1001) docker     (123)     5779 2023-04-06 07:32:28.000000 modelbaker-1.4.3/tests/test_update.py
--rw-r--r--   0 runner    (1001) docker     (123)    25477 2023-04-06 07:32:28.000000 modelbaker-1.4.3/tests/test_validate.py
--rw-r--r--   0 runner    (1001) docker     (123)     2508 2023-04-06 07:32:28.000000 modelbaker-1.4.3/tests/test_z_geom.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 13:56:13.805563 modelbaker-1.4.4/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-05-05 13:56:02.000000 modelbaker-1.4.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3507 2023-05-05 13:56:13.805563 modelbaker-1.4.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2956 2023-05-05 13:56:02.000000 modelbaker-1.4.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 13:56:13.789562 modelbaker-1.4.4/modelbaker/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 13:56:02.000000 modelbaker-1.4.4/modelbaker/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 13:56:13.793563 modelbaker-1.4.4/modelbaker/dataobjects/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 13:56:02.000000 modelbaker-1.4.4/modelbaker/dataobjects/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2156 2023-05-05 13:56:02.000000 modelbaker-1.4.4/modelbaker/dataobjects/fields.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5050 2023-05-05 13:56:02.000000 modelbaker-1.4.4/modelbaker/dataobjects/form.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13081 2023-05-05 13:56:02.000000 modelbaker-1.4.4/modelbaker/dataobjects/layers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4520 2023-05-05 13:56:02.000000 modelbaker-1.4.4/modelbaker/dataobjects/legend.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15631 2023-05-05 13:56:02.000000 modelbaker-1.4.4/modelbaker/dataobjects/project.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2334 2023-05-05 13:56:02.000000 modelbaker-1.4.4/modelbaker/dataobjects/relations.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 13:56:13.793563 modelbaker-1.4.4/modelbaker/db_factory/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 13:56:02.000000 modelbaker-1.4.4/modelbaker/db_factory/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3705 2023-05-05 13:56:02.000000 modelbaker-1.4.4/modelbaker/db_factory/db_command_config_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4370 2023-05-05 13:56:02.000000 modelbaker-1.4.4/modelbaker/db_factory/db_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3433 2023-05-05 13:56:02.000000 modelbaker-1.4.4/modelbaker/db_factory/db_simple_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2092 2023-05-05 13:56:02.000000 modelbaker-1.4.4/modelbaker/db_factory/gpkg_command_config_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1874 2023-05-05 13:56:02.000000 modelbaker-1.4.4/modelbaker/db_factory/gpkg_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1531 2023-05-05 13:56:02.000000 modelbaker-1.4.4/modelbaker/db_factory/gpkg_layer_uri.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1815 2023-05-05 13:56:02.000000 modelbaker-1.4.4/modelbaker/db_factory/layer_uri.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4603 2023-05-05 13:56:02.000000 modelbaker-1.4.4/modelbaker/db_factory/mssql_command_config_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1924 2023-05-05 13:56:02.000000 modelbaker-1.4.4/modelbaker/db_factory/mssql_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2760 2023-05-05 13:56:02.000000 modelbaker-1.4.4/modelbaker/db_factory/mssql_layer_uri.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7981 2023-05-05 13:56:02.000000 modelbaker-1.4.4/modelbaker/db_factory/pg_command_config_manager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3345 2023-05-05 13:56:02.000000 modelbaker-1.4.4/modelbaker/db_factory/pg_factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2508 2023-05-05 13:56:02.000000 modelbaker-1.4.4/modelbaker/db_factory/pg_layer_uri.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 13:56:13.793563 modelbaker-1.4.4/modelbaker/dbconnector/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 13:56:02.000000 modelbaker-1.4.4/modelbaker/dbconnector/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1966 2023-05-05 13:56:02.000000 modelbaker-1.4.4/modelbaker/dbconnector/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12596 2023-05-05 13:56:02.000000 modelbaker-1.4.4/modelbaker/dbconnector/db_connector.py
+-rw-r--r--   0 runner    (1001) docker     (123)    36134 2023-05-05 13:56:02.000000 modelbaker-1.4.4/modelbaker/dbconnector/gpkg_connector.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38036 2023-05-05 13:56:02.000000 modelbaker-1.4.4/modelbaker/dbconnector/mssql_connector.py
+-rw-r--r--   0 runner    (1001) docker     (123)    42595 2023-05-05 13:56:02.000000 modelbaker-1.4.4/modelbaker/dbconnector/pg_connector.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 13:56:13.797562 modelbaker-1.4.4/modelbaker/generator/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 13:56:02.000000 modelbaker-1.4.4/modelbaker/generator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      692 2023-05-05 13:56:02.000000 modelbaker-1.4.4/modelbaker/generator/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    50554 2023-05-05 13:56:02.000000 modelbaker-1.4.4/modelbaker/generator/domain_relations_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30620 2023-05-05 13:56:02.000000 modelbaker-1.4.4/modelbaker/generator/generator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 13:56:13.797562 modelbaker-1.4.4/modelbaker/ilitoppingmaker/
+-rw-r--r--   0 runner    (1001) docker     (123)     1251 2023-05-05 13:56:02.000000 modelbaker-1.4.4/modelbaker/ilitoppingmaker/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5494 2023-05-05 13:56:02.000000 modelbaker-1.4.4/modelbaker/ilitoppingmaker/ili2dbsettings.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7337 2023-05-05 13:56:02.000000 modelbaker-1.4.4/modelbaker/ilitoppingmaker/ilidata.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4211 2023-05-05 13:56:02.000000 modelbaker-1.4.4/modelbaker/ilitoppingmaker/iliprojecttopping.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3266 2023-05-05 13:56:02.000000 modelbaker-1.4.4/modelbaker/ilitoppingmaker/ilitarget.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6067 2023-05-05 13:56:02.000000 modelbaker-1.4.4/modelbaker/ilitoppingmaker/metaconfig.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 13:56:13.797562 modelbaker-1.4.4/modelbaker/iliwrapper/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 13:56:02.000000 modelbaker-1.4.4/modelbaker/iliwrapper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1200 2023-05-05 13:56:02.000000 modelbaker-1.4.4/modelbaker/iliwrapper/globals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4537 2023-05-05 13:56:02.000000 modelbaker-1.4.4/modelbaker/iliwrapper/ili2dbargs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16442 2023-05-05 13:56:02.000000 modelbaker-1.4.4/modelbaker/iliwrapper/ili2dbconfig.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2182 2023-05-05 13:56:02.000000 modelbaker-1.4.4/modelbaker/iliwrapper/ili2dbtools.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13089 2023-05-05 13:56:02.000000 modelbaker-1.4.4/modelbaker/iliwrapper/ili2dbutils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41162 2023-05-05 13:56:02.000000 modelbaker-1.4.4/modelbaker/iliwrapper/ilicache.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6182 2023-05-05 13:56:02.000000 modelbaker-1.4.4/modelbaker/iliwrapper/iliexecutable.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1638 2023-05-05 13:56:02.000000 modelbaker-1.4.4/modelbaker/iliwrapper/iliexporter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1578 2023-05-05 13:56:02.000000 modelbaker-1.4.4/modelbaker/iliwrapper/iliimporter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1326 2023-05-05 13:56:02.000000 modelbaker-1.4.4/modelbaker/iliwrapper/iliupdater.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5894 2023-05-05 13:56:02.000000 modelbaker-1.4.4/modelbaker/iliwrapper/ilivalidator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 13:56:13.797562 modelbaker-1.4.4/modelbaker/libs/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 13:56:05.000000 modelbaker-1.4.4/modelbaker/libs/__init__.py
+-rw-rw-r--   0 runner    (1001) docker     (123)    12895 2020-04-20 14:21:10.000000 modelbaker-1.4.4/modelbaker/libs/deprecation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 13:56:13.801562 modelbaker-1.4.4/modelbaker/libs/packaging/
+-rw-rw-r--   0 runner    (1001) docker     (123)      501 2023-04-12 11:10:22.000000 modelbaker-1.4.4/modelbaker/libs/packaging/__init__.py
+-rw-rw-r--   0 runner    (1001) docker     (123)     3266 2023-01-30 09:29:48.000000 modelbaker-1.4.4/modelbaker/libs/packaging/_elffile.py
+-rw-rw-r--   0 runner    (1001) docker     (123)     8926 2023-04-12 11:05:06.000000 modelbaker-1.4.4/modelbaker/libs/packaging/_manylinux.py
+-rw-rw-r--   0 runner    (1001) docker     (123)     2524 2023-01-30 09:29:48.000000 modelbaker-1.4.4/modelbaker/libs/packaging/_musllinux.py
+-rw-rw-r--   0 runner    (1001) docker     (123)    10194 2023-04-12 11:05:06.000000 modelbaker-1.4.4/modelbaker/libs/packaging/_parser.py
+-rw-rw-r--   0 runner    (1001) docker     (123)     1431 2023-01-30 09:29:48.000000 modelbaker-1.4.4/modelbaker/libs/packaging/_structures.py
+-rw-rw-r--   0 runner    (1001) docker     (123)     5292 2023-04-12 11:05:06.000000 modelbaker-1.4.4/modelbaker/libs/packaging/_tokenizer.py
+-rw-rw-r--   0 runner    (1001) docker     (123)     8208 2023-04-12 11:05:28.000000 modelbaker-1.4.4/modelbaker/libs/packaging/markers.py
+-rw-rw-r--   0 runner    (1001) docker     (123)    16397 2023-04-12 11:05:06.000000 modelbaker-1.4.4/modelbaker/libs/packaging/metadata.py
+-rw-rw-r--   0 runner    (1001) docker     (123)     3287 2023-04-12 11:05:06.000000 modelbaker-1.4.4/modelbaker/libs/packaging/requirements.py
+-rw-rw-r--   0 runner    (1001) docker     (123)    39206 2023-04-12 11:05:06.000000 modelbaker-1.4.4/modelbaker/libs/packaging/specifiers.py
+-rw-rw-r--   0 runner    (1001) docker     (123)    18106 2023-04-12 11:05:06.000000 modelbaker-1.4.4/modelbaker/libs/packaging/tags.py
+-rw-rw-r--   0 runner    (1001) docker     (123)     4355 2023-01-30 09:29:48.000000 modelbaker-1.4.4/modelbaker/libs/packaging/utils.py
+-rw-rw-r--   0 runner    (1001) docker     (123)    16326 2023-04-12 11:05:06.000000 modelbaker-1.4.4/modelbaker/libs/packaging/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 13:56:13.801562 modelbaker-1.4.4/modelbaker/libs/pgserviceparser/
+-rw-rw-r--   0 runner    (1001) docker     (123)     1801 2022-06-27 10:25:36.000000 modelbaker-1.4.4/modelbaker/libs/pgserviceparser/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 13:56:13.801562 modelbaker-1.4.4/modelbaker/libs/toppingmaker/
+-rw-rw-r--   0 runner    (1001) docker     (123)     1152 2022-12-16 08:01:28.000000 modelbaker-1.4.4/modelbaker/libs/toppingmaker/__init__.py
+-rw-rw-r--   0 runner    (1001) docker     (123)     6582 2022-12-16 08:01:28.000000 modelbaker-1.4.4/modelbaker/libs/toppingmaker/exportsettings.py
+-rw-rw-r--   0 runner    (1001) docker     (123)    26523 2022-12-16 08:01:28.000000 modelbaker-1.4.4/modelbaker/libs/toppingmaker/projecttopping.py
+-rw-rw-r--   0 runner    (1001) docker     (123)     3366 2022-12-16 08:01:28.000000 modelbaker-1.4.4/modelbaker/libs/toppingmaker/target.py
+-rw-rw-r--   0 runner    (1001) docker     (123)     1321 2022-12-16 08:01:28.000000 modelbaker-1.4.4/modelbaker/libs/toppingmaker/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 13:56:13.801562 modelbaker-1.4.4/modelbaker/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 13:56:02.000000 modelbaker-1.4.4/modelbaker/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6394 2023-05-05 13:56:02.000000 modelbaker-1.4.4/modelbaker/utils/db_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1205 2023-05-05 13:56:02.000000 modelbaker-1.4.4/modelbaker/utils/globals.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4684 2023-05-05 13:56:02.000000 modelbaker-1.4.4/modelbaker/utils/qgis_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10267 2023-05-05 13:56:02.000000 modelbaker-1.4.4/modelbaker/utils/qt_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 13:56:13.793563 modelbaker-1.4.4/modelbaker.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3507 2023-05-05 13:56:13.000000 modelbaker-1.4.4/modelbaker.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3583 2023-05-05 13:56:13.000000 modelbaker-1.4.4/modelbaker.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 13:56:13.000000 modelbaker-1.4.4/modelbaker.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-05 13:56:13.000000 modelbaker-1.4.4/modelbaker.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-05 13:56:13.805563 modelbaker-1.4.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      874 2023-05-05 13:56:02.000000 modelbaker-1.4.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 13:56:13.805563 modelbaker-1.4.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    12580 2023-05-05 13:56:02.000000 modelbaker-1.4.4/tests/test_dataset_handling.py
+-rw-r--r--   0 runner    (1001) docker     (123)   151890 2023-05-05 13:56:02.000000 modelbaker-1.4.4/tests/test_domain_class_relations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2831 2023-05-05 13:56:02.000000 modelbaker-1.4.4/tests/test_dump.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39104 2023-05-05 13:56:02.000000 modelbaker-1.4.4/tests/test_export.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3425 2023-05-05 13:56:02.000000 modelbaker-1.4.4/tests/test_get_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6555 2023-05-05 13:56:02.000000 modelbaker-1.4.4/tests/test_gpkg_pk.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2517 2023-05-05 13:56:02.000000 modelbaker-1.4.4/tests/test_ili2dbutils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28912 2023-05-05 13:56:02.000000 modelbaker-1.4.4/tests/test_ilicache.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13620 2023-05-05 13:56:02.000000 modelbaker-1.4.4/tests/test_ilitoppingmaker.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17928 2023-05-05 13:56:02.000000 modelbaker-1.4.4/tests/test_import.py
+-rw-r--r--   0 runner    (1001) docker     (123)      529 2023-05-05 13:56:02.000000 modelbaker-1.4.4/tests/test_libili2pg.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14531 2023-05-05 13:56:02.000000 modelbaker-1.4.4/tests/test_metaconfig.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11343 2023-05-05 13:56:02.000000 modelbaker-1.4.4/tests/test_pgservice.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1008 2023-05-05 13:56:02.000000 modelbaker-1.4.4/tests/test_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)   166117 2023-05-05 13:56:02.000000 modelbaker-1.4.4/tests/test_projectgen.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15529 2023-05-05 13:56:02.000000 modelbaker-1.4.4/tests/test_projectgen_generic_databases.py
+-rw-r--r--   0 runner    (1001) docker     (123)    51448 2023-05-05 13:56:02.000000 modelbaker-1.4.4/tests/test_projecttopping.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5779 2023-05-05 13:56:02.000000 modelbaker-1.4.4/tests/test_update.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25477 2023-05-05 13:56:02.000000 modelbaker-1.4.4/tests/test_validate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2508 2023-05-05 13:56:02.000000 modelbaker-1.4.4/tests/test_z_geom.py
```

### Comparing `modelbaker-1.4.3/LICENSE` & `modelbaker-1.4.4/LICENSE`

 * *Files identical despite different names*

### Comparing `modelbaker-1.4.3/PKG-INFO` & `modelbaker-1.4.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: modelbaker
-Version: 1.4.3
+Version: 1.4.4
 Summary: The full model baker core
 Home-page: https://github.com/opengisch/QgisModelBakerLibrary
 Author: Dave Signer
 Author-email: david@opengis.ch
 Classifier: Topic :: Database
 Classifier: License :: OSI Approved :: GNU General Public License v2 or later (GPLv2+)
 Classifier: Programming Language :: Python :: 3
@@ -93,25 +93,25 @@
     ├── db_utils.py
     ├── globals.py
     ├── qgis_utils.py
     └── qt_utils.py
 ```
 
 ### ili2db
-In the current release we use ili2db version 4.6.1
+In the current release we use ili2db version 4.10
 
 ## Infos for Devs
 
 ### Code style
 
 Is enforced with pre-commit. To use, make:
 ```
 pip install pre-commit
 pre-commit install
-```
+```00
 And to run it over all the files (with infile changes):
 ```
 pre-commit run --color=always --all-file
 ```
 
 ### Needed packages from PyPI
```

### Comparing `modelbaker-1.4.3/README.md` & `modelbaker-1.4.4/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -77,25 +77,25 @@
     ├── db_utils.py
     ├── globals.py
     ├── qgis_utils.py
     └── qt_utils.py
 ```
 
 ### ili2db
-In the current release we use ili2db version 4.6.1
+In the current release we use ili2db version 4.10
 
 ## Infos for Devs
 
 ### Code style
 
 Is enforced with pre-commit. To use, make:
 ```
 pip install pre-commit
 pre-commit install
-```
+```00
 And to run it over all the files (with infile changes):
 ```
 pre-commit run --color=always --all-file
 ```
 
 ### Needed packages from PyPI
```

### Comparing `modelbaker-1.4.3/modelbaker/dataobjects/fields.py` & `modelbaker-1.4.4/modelbaker/dataobjects/fields.py`

 * *Files identical despite different names*

### Comparing `modelbaker-1.4.3/modelbaker/dataobjects/form.py` & `modelbaker-1.4.4/modelbaker/dataobjects/form.py`

 * *Files identical despite different names*

### Comparing `modelbaker-1.4.3/modelbaker/dataobjects/layers.py` & `modelbaker-1.4.4/modelbaker/dataobjects/layers.py`

 * *Files identical despite different names*

### Comparing `modelbaker-1.4.3/modelbaker/dataobjects/legend.py` & `modelbaker-1.4.4/modelbaker/dataobjects/legend.py`

 * *Files identical despite different names*

### Comparing `modelbaker-1.4.3/modelbaker/dataobjects/project.py` & `modelbaker-1.4.4/modelbaker/dataobjects/project.py`

 * *Files identical despite different names*

### Comparing `modelbaker-1.4.3/modelbaker/dataobjects/relations.py` & `modelbaker-1.4.4/modelbaker/dataobjects/relations.py`

 * *Files identical despite different names*

### Comparing `modelbaker-1.4.3/modelbaker/db_factory/db_command_config_manager.py` & `modelbaker-1.4.4/modelbaker/db_factory/db_command_config_manager.py`

 * *Files identical despite different names*

### Comparing `modelbaker-1.4.3/modelbaker/db_factory/db_factory.py` & `modelbaker-1.4.4/modelbaker/db_factory/db_factory.py`

 * *Files identical despite different names*

### Comparing `modelbaker-1.4.3/modelbaker/db_factory/db_simple_factory.py` & `modelbaker-1.4.4/modelbaker/db_factory/db_simple_factory.py`

 * *Files identical despite different names*

### Comparing `modelbaker-1.4.3/modelbaker/db_factory/gpkg_command_config_manager.py` & `modelbaker-1.4.4/modelbaker/db_factory/gpkg_command_config_manager.py`

 * *Files identical despite different names*

### Comparing `modelbaker-1.4.3/modelbaker/db_factory/gpkg_factory.py` & `modelbaker-1.4.4/modelbaker/db_factory/gpkg_factory.py`

 * *Files identical despite different names*

### Comparing `modelbaker-1.4.3/modelbaker/db_factory/gpkg_layer_uri.py` & `modelbaker-1.4.4/modelbaker/db_factory/gpkg_layer_uri.py`

 * *Files identical despite different names*

### Comparing `modelbaker-1.4.3/modelbaker/db_factory/layer_uri.py` & `modelbaker-1.4.4/modelbaker/db_factory/layer_uri.py`

 * *Files identical despite different names*

### Comparing `modelbaker-1.4.3/modelbaker/db_factory/mssql_command_config_manager.py` & `modelbaker-1.4.4/modelbaker/db_factory/mssql_command_config_manager.py`

 * *Files identical despite different names*

### Comparing `modelbaker-1.4.3/modelbaker/db_factory/mssql_factory.py` & `modelbaker-1.4.4/modelbaker/db_factory/mssql_factory.py`

 * *Files identical despite different names*

### Comparing `modelbaker-1.4.3/modelbaker/db_factory/mssql_layer_uri.py` & `modelbaker-1.4.4/modelbaker/db_factory/mssql_layer_uri.py`

 * *Files identical despite different names*

### Comparing `modelbaker-1.4.3/modelbaker/db_factory/pg_command_config_manager.py` & `modelbaker-1.4.4/modelbaker/db_factory/pg_command_config_manager.py`

 * *Files identical despite different names*

### Comparing `modelbaker-1.4.3/modelbaker/db_factory/pg_factory.py` & `modelbaker-1.4.4/modelbaker/db_factory/pg_factory.py`

 * *Files identical despite different names*

### Comparing `modelbaker-1.4.3/modelbaker/db_factory/pg_layer_uri.py` & `modelbaker-1.4.4/modelbaker/db_factory/pg_layer_uri.py`

 * *Files identical despite different names*

### Comparing `modelbaker-1.4.3/modelbaker/dbconnector/config.py` & `modelbaker-1.4.4/modelbaker/dbconnector/config.py`

 * *Files identical despite different names*

### Comparing `modelbaker-1.4.3/modelbaker/dbconnector/db_connector.py` & `modelbaker-1.4.4/modelbaker/dbconnector/db_connector.py`

 * *Files identical despite different names*

### Comparing `modelbaker-1.4.3/modelbaker/dbconnector/gpkg_connector.py` & `modelbaker-1.4.4/modelbaker/dbconnector/gpkg_connector.py`

 * *Files identical despite different names*

### Comparing `modelbaker-1.4.3/modelbaker/dbconnector/mssql_connector.py` & `modelbaker-1.4.4/modelbaker/dbconnector/mssql_connector.py`

 * *Files identical despite different names*

### Comparing `modelbaker-1.4.3/modelbaker/dbconnector/pg_connector.py` & `modelbaker-1.4.4/modelbaker/dbconnector/pg_connector.py`

 * *Files identical despite different names*

### Comparing `modelbaker-1.4.3/modelbaker/generator/config.py` & `modelbaker-1.4.4/modelbaker/generator/config.py`

 * *Files identical despite different names*

### Comparing `modelbaker-1.4.3/modelbaker/generator/domain_relations_generator.py` & `modelbaker-1.4.4/modelbaker/generator/domain_relations_generator.py`

 * *Files identical despite different names*

### Comparing `modelbaker-1.4.3/modelbaker/generator/generator.py` & `modelbaker-1.4.4/modelbaker/generator/generator.py`

 * *Files identical despite different names*

### Comparing `modelbaker-1.4.3/modelbaker/ilitoppingmaker/__init__.py` & `modelbaker-1.4.4/modelbaker/ilitoppingmaker/__init__.py`

 * *Files identical despite different names*

### Comparing `modelbaker-1.4.3/modelbaker/ilitoppingmaker/ili2dbsettings.py` & `modelbaker-1.4.4/modelbaker/ilitoppingmaker/ili2dbsettings.py`

 * *Files identical despite different names*

### Comparing `modelbaker-1.4.3/modelbaker/ilitoppingmaker/ilidata.py` & `modelbaker-1.4.4/modelbaker/ilitoppingmaker/ilidata.py`

 * *Files 12% similar despite different names*

```diff
@@ -48,15 +48,17 @@
         self.linking_models = linking_models
 
         self.version = dataset_version
         self.publishing_date = publishing_date
         self.owner = owner
         self.project_name = project_name
 
-        self.title = f"QGIS {self.file_type} file for {self.project_name} - {os.path.splitext(os.path.basename(self.file_path))}"
+        # the title is mostly what is displayed in a specific context
+        self.title = self.project_name
+        self.short_description = f"QGIS {self.file_type} file for {self.project_name} - {os.path.splitext(os.path.basename(self.file_path))}"
         self.file_mimetype = self._file_mime_type(self.file_path)
 
     def _file_mime_type(self, file_path: str = None) -> str:
         mimetype = mimetypes.guess_type(file_path)
         if mimetype[0] is None:
             # ugly fallback
             return "text/plain"
@@ -77,14 +79,24 @@
         )
         localisedtext = ET.SubElement(datsetidx16_multilingualtext, "LocalisedText")
         datasetidx16_localisedtext = ET.SubElement(
             localisedtext, "DatasetIdx16.LocalisedText"
         )
         ET.SubElement(datasetidx16_localisedtext, "Text").text = self.title
 
+        short_description = ET.SubElement(element, "shortDescription")
+        datsetidx16_multilingualtext = ET.SubElement(
+            short_description, "DatasetIdx16.MultilingualMText"
+        )
+        localisedtext = ET.SubElement(datsetidx16_multilingualtext, "LocalisedText")
+        datasetidx16_localisedtext = ET.SubElement(
+            localisedtext, "DatasetIdx16.LocalisedMText"
+        )
+        ET.SubElement(datasetidx16_localisedtext, "Text").text = self.short_description
+
         categories = ET.SubElement(element, "categories")
         type_datasetidx16_code = ET.SubElement(categories, "DatasetIdx16.Code_")
         ET.SubElement(
             type_datasetidx16_code, "value"
         ).text = f"http://codes.interlis.ch/type/{self.file_type}"
 
         if self.file_type in ["metaconfig", "referencedata"]:
```

### Comparing `modelbaker-1.4.3/modelbaker/ilitoppingmaker/iliprojecttopping.py` & `modelbaker-1.4.4/modelbaker/ilitoppingmaker/iliprojecttopping.py`

 * *Files identical despite different names*

### Comparing `modelbaker-1.4.3/modelbaker/ilitoppingmaker/ilitarget.py` & `modelbaker-1.4.4/modelbaker/ilitoppingmaker/ilitarget.py`

 * *Files identical despite different names*

### Comparing `modelbaker-1.4.3/modelbaker/ilitoppingmaker/metaconfig.py` & `modelbaker-1.4.4/modelbaker/ilitoppingmaker/metaconfig.py`

 * *Files identical despite different names*

### Comparing `modelbaker-1.4.3/modelbaker/iliwrapper/globals.py` & `modelbaker-1.4.4/modelbaker/iliwrapper/globals.py`

 * *Files identical despite different names*

### Comparing `modelbaker-1.4.3/modelbaker/iliwrapper/ili2dbargs.py` & `modelbaker-1.4.4/modelbaker/iliwrapper/ili2dbargs.py`

 * *Files identical despite different names*

### Comparing `modelbaker-1.4.3/modelbaker/iliwrapper/ili2dbconfig.py` & `modelbaker-1.4.4/modelbaker/iliwrapper/ili2dbconfig.py`

 * *Files identical despite different names*

### Comparing `modelbaker-1.4.3/modelbaker/iliwrapper/ili2dbtools.py` & `modelbaker-1.4.4/modelbaker/iliwrapper/ili2dbtools.py`

 * *Files identical despite different names*

### Comparing `modelbaker-1.4.3/modelbaker/iliwrapper/ili2dbutils.py` & `modelbaker-1.4.4/modelbaker/iliwrapper/ili2dbutils.py`

 * *Files identical despite different names*

### Comparing `modelbaker-1.4.3/modelbaker/iliwrapper/ilicache.py` & `modelbaker-1.4.4/modelbaker/iliwrapper/ilicache.py`

 * *Files 10% similar despite different names*

```diff
@@ -20,15 +20,15 @@
 import logging
 import os
 import re
 import urllib.parse
 import xml.etree.ElementTree as ET
 from enum import Enum
 
-from PyQt5.QtCore import QObject, Qt, pyqtSignal
+from PyQt5.QtCore import QObject, QSortFilterProxyModel, Qt, pyqtSignal
 from PyQt5.QtGui import QPalette, QRegion, QStandardItem, QStandardItemModel
 from PyQt5.QtWidgets import QGridLayout, QItemDelegate, QLabel, QStyle, QWidget
 from qgis.core import Qgis, QgsMessageLog
 
 from ..utils.qt_utils import download_file
 from .ili2dbutils import get_all_modeldir_in_path
 
@@ -42,14 +42,17 @@
         QObject.__init__(self)
         self.cache_path = os.path.expanduser("~/.ilicache")
         self.information_file = "ilimodels.xml"
         self.repositories = dict()
         self.base_configuration = configuration
         self.single_ili_file = single_ili_file
         self.model = IliModelItemModel()
+        self.sorted_model = QSortFilterProxyModel()
+        self.sorted_model.setSourceModel(self.model)
+        self.sorted_model.sort(0, Qt.AscendingOrder)
         self.directories = None
         if self.base_configuration:
             self.directories = self.base_configuration.model_directories
 
     def refresh(self):
         if not self.directories is None:
             for directory in self.directories:
@@ -361,15 +364,15 @@
             for model in repository:
                 # in case there is more than one version of the model with the same name, it shouldn't load it twice
                 if any(model["name"] == s for s in names):
                     continue
 
                 item = QStandardItem()
                 item.setData(model["name"], int(Qt.DisplayRole))
-                item.setData(model["name"], int(Qt.EditRole))
+                item.setData(model["name"], int(Qt.EditRole))  # considered in completer
                 item.setData(model["repository"], int(IliModelItemModel.Roles.ILIREPO))
                 item.setData(model["version"], int(IliModelItemModel.Roles.VERSION))
 
                 names.append(model["name"])
                 self.appendRow(item)
                 row += 1
 
@@ -428,15 +431,16 @@
         self.cache_path = os.path.expanduser("~/.ilimetaconfigcache")
         self.information_file = "ilidata.xml"
 
         self.model = IliDataItemModel()
         self.model.modelReset.connect(
             lambda: self.model_refreshed.emit(self.model.rowCount())
         )
-
+        self.sorted_model.setSourceModel(self.model)
+        self.sorted_model.sort(0, Qt.AscendingOrder)
         self.filter_models = models.split(";") if models else []
         self.type = type
         self.directories = (
             self.base_configuration.metaconfig_directories
             if self.base_configuration
             else []
         )
@@ -527,14 +531,50 @@
                                             localised_text_element.find(
                                                 "ili23:Text", self.ns
                                             )
                                         ),
                                     }
                                     title.append(title_information)
 
+                    short_description = list()
+
+                    for short_description_element in metaconfig_metadata.findall(
+                        "ili23:shortDescription", self.ns
+                    ):
+                        for (
+                            multilingual_text_element
+                        ) in short_description_element.findall(
+                            "ili23:DatasetIdx16.MultilingualMText", self.ns
+                        ):
+                            for (
+                                localised_text_element
+                            ) in multilingual_text_element.findall(
+                                "ili23:LocalisedText", self.ns
+                            ):
+                                for (
+                                    localised_text_element
+                                ) in localised_text_element.findall(
+                                    "ili23:DatasetIdx16.LocalisedMText", self.ns
+                                ):
+                                    short_description_information = {
+                                        "language": self.get_element_text(
+                                            localised_text_element.find(
+                                                "ili23:Language", self.ns
+                                            )
+                                        ),
+                                        "text": self.get_element_text(
+                                            localised_text_element.find(
+                                                "ili23:Text", self.ns
+                                            )
+                                        ),
+                                    }
+                                    short_description.append(
+                                        short_description_information
+                                    )
+
                     model_link_names = []
                     for basket_element in metaconfig_metadata.findall(
                         "ili23:baskets", self.ns
                     ):
                         for basket_metadata in basket_element.findall(
                             "ili23:DatasetIdx16.DataIndex.BasketMetadata", self.ns
                         ):
@@ -584,14 +624,20 @@
                                     metaconfig["url"] = url
                                     metaconfig["models"] = models
                                     metaconfig["relative_file_path"] = path
                                     if title is not None:
                                         metaconfig["title"] = title
                                     else:
                                         metaconfig["title"] = None
+                                    if short_description is not None:
+                                        metaconfig[
+                                            "short_description"
+                                        ] = short_description
+                                    else:
+                                        metaconfig["short_description"] = None
 
                                     metaconfig["model_link_names"] = model_link_names
                                     repo_metaconfigs.append(metaconfig)
 
         self.repositories[netloc] = sorted(
             repo_metaconfigs,
             key=lambda m: m["version"] if m["version"] else "0",
@@ -646,14 +692,15 @@
         MODELS = Qt.UserRole + 3
         RELATIVEFILEPATH = Qt.UserRole + 4
         OWNER = Qt.UserRole + 5
         TITLE = Qt.UserRole + 6
         ID = Qt.UserRole + 7
         URL = Qt.UserRole + 8
         MODEL_LINKS = Qt.UserRole + 9
+        SHORT_DESCRIPTION = Qt.UserRole + 10
 
         def __int__(self):
             return self.value
 
     def __init__(self, parent=None):
         super().__init__(0, 1, parent)
 
@@ -671,29 +718,40 @@
 
                 item = QStandardItem()
                 display_value = dataitem["id"]
                 if dataitem["title"] and "text" in dataitem["title"][0]:
                     # since there is no multilanguage handling we take the first entry
                     display_value = dataitem["title"][0]["text"]
 
+                short_description = None
+                if (
+                    dataitem["short_description"]
+                    and "text" in dataitem["short_description"][0]
+                ):
+                    short_description = dataitem["short_description"][0]["text"]
+
                 item.setData(display_value, int(Qt.DisplayRole))
                 item.setData(display_value, int(Qt.EditRole))
+                item.setData(short_description, int(Qt.ToolTipRole))
                 item.setData(dataitem["id"], int(IliDataItemModel.Roles.ID))
                 item.setData(
                     dataitem["repository"], int(IliDataItemModel.Roles.ILIREPO)
                 )
                 item.setData(dataitem["version"], int(IliDataItemModel.Roles.VERSION))
                 item.setData(dataitem["models"], int(IliDataItemModel.Roles.MODELS))
                 item.setData(
                     dataitem["relative_file_path"],
                     int(IliDataItemModel.Roles.RELATIVEFILEPATH),
                 )
                 item.setData(dataitem["owner"], int(IliDataItemModel.Roles.OWNER))
                 item.setData(dataitem["title"], int(IliDataItemModel.Roles.TITLE))
                 item.setData(dataitem["url"], int(IliDataItemModel.Roles.URL))
+                item.setData(
+                    short_description, int(IliDataItemModel.Roles.SHORT_DESCRIPTION)
+                )
 
                 item.setData(
                     dataitem["model_link_names"],
                     int(IliDataItemModel.Roles.MODEL_LINKS),
                 )
 
                 ids.append(dataitem["id"])
@@ -714,29 +772,27 @@
         self.widget.setLayout(QGridLayout())
         self.widget.layout().setContentsMargins(2, 0, 0, 0)
         self.metaconfig_label = QLabel()
         self.metaconfig_label.setAttribute(Qt.WA_TranslucentBackground)
         self.repository_label = QLabel()
         self.repository_label.setAlignment(Qt.AlignRight)
         self.widget.layout().addWidget(self.metaconfig_label, 0, 0)
-        self.widget.layout().addWidget(self.repository_label, 0, 2)
+        self.widget.layout().addWidget(self.repository_label, 0, 1)
 
     def paint(self, painter, option, index):
         option.index = index
         super().paint(painter, option, index)
 
     def drawDisplay(self, painter, option, rect, text):
         repository = option.index.data(int(IliDataItemModel.Roles.ILIREPO))
-        models = option.index.data(int(IliDataItemModel.Roles.MODELS))
-        owner = option.index.data(int(IliDataItemModel.Roles.OWNER))
         display_text = option.index.data(int(Qt.DisplayRole))
 
         self.repository_label.setText(
-            '<font color="#666666"><i>of {owner} with {models} at {repository}</i></font>'.format(
-                owner=owner, models="/".join(models), repository=repository
+            '<font color="#666666"><i>{repository}</i></font>'.format(
+                repository=repository
             )
         )
         self.metaconfig_label.setText(
             "{display_text}".format(display_text=display_text)
         )
         self.widget.setMinimumSize(rect.size())
 
@@ -758,14 +814,16 @@
     file_ids can contain ilidata: or file: information
     """
 
     def __init__(self, configuration, file_ids=None, tool_dir=None):
         IliDataCache.__init__(self, configuration)
         self.cache_path = os.path.expanduser("~/.ilitoppingfilescache")
         self.model = IliToppingFileItemModel()
+        self.sorted_model.setSourceModel(self.model)
+        self.sorted_model.sort(0, Qt.AscendingOrder)
         self.file_ids = file_ids
         self.tool_dir = (
             tool_dir
             if tool_dir
             else os.path.dirname(os.path.dirname(os.path.realpath(__file__)))
         )
         self.downloaded_files = list()
```

### Comparing `modelbaker-1.4.3/modelbaker/iliwrapper/iliexecutable.py` & `modelbaker-1.4.4/modelbaker/iliwrapper/iliexecutable.py`

 * *Files identical despite different names*

### Comparing `modelbaker-1.4.3/modelbaker/iliwrapper/iliexporter.py` & `modelbaker-1.4.4/modelbaker/iliwrapper/iliexporter.py`

 * *Files identical despite different names*

### Comparing `modelbaker-1.4.3/modelbaker/iliwrapper/iliimporter.py` & `modelbaker-1.4.4/modelbaker/iliwrapper/iliimporter.py`

 * *Files identical despite different names*

### Comparing `modelbaker-1.4.3/modelbaker/iliwrapper/iliupdater.py` & `modelbaker-1.4.4/modelbaker/iliwrapper/iliupdater.py`

 * *Files identical despite different names*

### Comparing `modelbaker-1.4.3/modelbaker/iliwrapper/ilivalidator.py` & `modelbaker-1.4.4/modelbaker/iliwrapper/ilivalidator.py`

 * *Files identical despite different names*

### Comparing `modelbaker-1.4.3/modelbaker/libs/deprecation.py` & `modelbaker-1.4.4/modelbaker/libs/deprecation.py`

 * *Files identical despite different names*

### Comparing `modelbaker-1.4.3/modelbaker/libs/packaging/_elffile.py` & `modelbaker-1.4.4/modelbaker/libs/packaging/_elffile.py`

 * *Files identical despite different names*

### Comparing `modelbaker-1.4.3/modelbaker/libs/packaging/_manylinux.py` & `modelbaker-1.4.4/modelbaker/libs/packaging/_manylinux.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,14 +10,16 @@
 from ._elffile import EIClass, EIData, ELFFile, EMachine
 
 EF_ARM_ABIMASK = 0xFF000000
 EF_ARM_ABI_VER5 = 0x05000000
 EF_ARM_ABI_FLOAT_HARD = 0x00000400
 
 
+# `os.PathLike` not a generic type until Python 3.9, so sticking with `str`
+# as the type for `path` until then.
 @contextlib.contextmanager
 def _parse_elf(path: str) -> Generator[Optional[ELFFile], None, None]:
     try:
         with open(path, "rb") as f:
             yield ELFFile(f)
     except (OSError, TypeError, ValueError):
         yield None
```

### Comparing `modelbaker-1.4.3/modelbaker/libs/packaging/_musllinux.py` & `modelbaker-1.4.4/modelbaker/libs/packaging/_musllinux.py`

 * *Files identical despite different names*

### Comparing `modelbaker-1.4.3/modelbaker/libs/packaging/_parser.py` & `modelbaker-1.4.4/modelbaker/libs/packaging/_parser.py`

 * *Files 4% similar despite different names*

```diff
@@ -159,15 +159,19 @@
 def _parse_extras(tokenizer: Tokenizer) -> List[str]:
     """
     extras = (LEFT_BRACKET wsp* extras_list? wsp* RIGHT_BRACKET)?
     """
     if not tokenizer.check("LEFT_BRACKET", peek=True):
         return []
 
-    with tokenizer.enclosing_tokens("LEFT_BRACKET", "RIGHT_BRACKET"):
+    with tokenizer.enclosing_tokens(
+        "LEFT_BRACKET",
+        "RIGHT_BRACKET",
+        around="extras",
+    ):
         tokenizer.consume("WS")
         extras = _parse_extras_list(tokenizer)
         tokenizer.consume("WS")
 
     return extras
 
 
@@ -199,29 +203,46 @@
 
 
 def _parse_specifier(tokenizer: Tokenizer) -> str:
     """
     specifier = LEFT_PARENTHESIS WS? version_many WS? RIGHT_PARENTHESIS
               | WS? version_many WS?
     """
-    with tokenizer.enclosing_tokens("LEFT_PARENTHESIS", "RIGHT_PARENTHESIS"):
+    with tokenizer.enclosing_tokens(
+        "LEFT_PARENTHESIS",
+        "RIGHT_PARENTHESIS",
+        around="version specifier",
+    ):
         tokenizer.consume("WS")
         parsed_specifiers = _parse_version_many(tokenizer)
         tokenizer.consume("WS")
 
     return parsed_specifiers
 
 
 def _parse_version_many(tokenizer: Tokenizer) -> str:
     """
     version_many = (SPECIFIER (WS? COMMA WS? SPECIFIER)*)?
     """
     parsed_specifiers = ""
     while tokenizer.check("SPECIFIER"):
+        span_start = tokenizer.position
         parsed_specifiers += tokenizer.read().text
+        if tokenizer.check("VERSION_PREFIX_TRAIL", peek=True):
+            tokenizer.raise_syntax_error(
+                ".* suffix can only be used with `==` or `!=` operators",
+                span_start=span_start,
+                span_end=tokenizer.position + 1,
+            )
+        if tokenizer.check("VERSION_LOCAL_LABEL_TRAIL", peek=True):
+            tokenizer.raise_syntax_error(
+                "Local version label can only be used with `==` or `!=` operators",
+                span_start=span_start,
+                span_end=tokenizer.position,
+            )
         tokenizer.consume("WS")
         if not tokenizer.check("COMMA"):
             break
         parsed_specifiers += tokenizer.read().text
         tokenizer.consume("WS")
 
     return parsed_specifiers
@@ -250,15 +271,19 @@
     """
     marker_atom = WS? LEFT_PARENTHESIS WS? marker WS? RIGHT_PARENTHESIS WS?
                 | WS? marker_item WS?
     """
 
     tokenizer.consume("WS")
     if tokenizer.check("LEFT_PARENTHESIS", peek=True):
-        with tokenizer.enclosing_tokens("LEFT_PARENTHESIS", "RIGHT_PARENTHESIS"):
+        with tokenizer.enclosing_tokens(
+            "LEFT_PARENTHESIS",
+            "RIGHT_PARENTHESIS",
+            around="marker expression",
+        ):
             tokenizer.consume("WS")
             marker: MarkerAtom = _parse_marker(tokenizer)
             tokenizer.consume("WS")
     else:
         marker = _parse_marker_item(tokenizer)
     tokenizer.consume("WS")
     return marker
```

### Comparing `modelbaker-1.4.3/modelbaker/libs/packaging/_structures.py` & `modelbaker-1.4.4/modelbaker/libs/packaging/_structures.py`

 * *Files identical despite different names*

### Comparing `modelbaker-1.4.3/modelbaker/libs/packaging/_tokenizer.py` & `modelbaker-1.4.4/modelbaker/libs/packaging/_tokenizer.py`

 * *Files 1% similar despite different names*

```diff
@@ -74,14 +74,16 @@
     "SPECIFIER": re.compile(
         Specifier._operator_regex_str + Specifier._version_regex_str,
         re.VERBOSE | re.IGNORECASE,
     ),
     "AT": r"\@",
     "URL": r"[^ \t]+",
     "IDENTIFIER": r"\b[a-zA-Z0-9][a-zA-Z0-9._-]*\b",
+    "VERSION_PREFIX_TRAIL": r"\.\*",
+    "VERSION_LOCAL_LABEL_TRAIL": r"\+[a-z0-9]+(?:[-_\.][a-z0-9]+)*",
     "WS": r"[ \t]+",
     "END": r"$",
 }
 
 
 class Tokenizer:
     """Context-sensitive token parsing.
@@ -163,26 +165,28 @@
         raise ParserSyntaxError(
             message,
             source=self.source,
             span=span,
         )
 
     @contextlib.contextmanager
-    def enclosing_tokens(self, open_token: str, close_token: str) -> Iterator[bool]:
+    def enclosing_tokens(
+        self, open_token: str, close_token: str, *, around: str
+    ) -> Iterator[None]:
         if self.check(open_token):
             open_position = self.position
             self.read()
         else:
             open_position = None
 
-        yield open_position is not None
+        yield
 
         if open_position is None:
             return
 
         if not self.check(close_token):
             self.raise_syntax_error(
-                f"Expected closing {close_token}",
+                f"Expected matching {close_token} for {open_token}, after {around}",
                 span_start=open_position,
             )
 
         self.read()
```

### Comparing `modelbaker-1.4.3/modelbaker/libs/packaging/markers.py` & `modelbaker-1.4.4/modelbaker/libs/packaging/markers.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,22 @@
 
 import operator
 import os
 import platform
 import sys
 from typing import Any, Callable, Dict, List, Optional, Tuple, Union
 
-from ._parser import MarkerAtom, MarkerList, Op, Value, Variable, parse_marker
+from ._parser import (
+    MarkerAtom,
+    MarkerList,
+    Op,
+    Value,
+    Variable,
+    parse_marker as _parse_marker,
+)
 from ._tokenizer import ParserSyntaxError
 from .specifiers import InvalidSpecifier, Specifier
 from .utils import canonicalize_name
 
 __all__ = [
     "InvalidMarker",
     "UndefinedComparison",
@@ -185,15 +192,15 @@
 
 class Marker:
     def __init__(self, marker: str) -> None:
         # Note: We create a Marker object without calling this constructor in
         #       packaging.requirements.Requirement. If any additional logic is
         #       added here, make sure to mirror/adapt Requirement.
         try:
-            self._markers = _normalize_extra_values(parse_marker(marker))
+            self._markers = _normalize_extra_values(_parse_marker(marker))
             # The attribute `_markers` can be described in terms of a recursive type:
             # MarkerList = List[Union[Tuple[Node, ...], str, MarkerList]]
             #
             # For example, the following expression:
             # python_version > "3.6" or (python_version == "3.6" and os_name == "unix")
             #
             # is parsed into:
```

### Comparing `modelbaker-1.4.3/modelbaker/libs/packaging/requirements.py` & `modelbaker-1.4.4/modelbaker/libs/packaging/requirements.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # This file is dual licensed under the terms of the Apache License, Version
 # 2.0, and the BSD License. See the LICENSE file in the root of this repository
 # for complete details.
 
 import urllib.parse
 from typing import Any, List, Optional, Set
 
-from ._parser import parse_requirement
+from ._parser import parse_requirement as _parse_requirement
 from ._tokenizer import ParserSyntaxError
 from .markers import Marker, _normalize_extra_values
 from .specifiers import SpecifierSet
 
 
 class InvalidRequirement(ValueError):
     """
@@ -28,15 +28,15 @@
     # TODO: Can we test whether something is contained within a requirement?
     #       If so how do we do that? Do we need to test against the _name_ of
     #       the thing as well as the version? What about the markers?
     # TODO: Can we normalize the name and extra name?
 
     def __init__(self, requirement_string: str) -> None:
         try:
-            parsed = parse_requirement(requirement_string)
+            parsed = _parse_requirement(requirement_string)
         except ParserSyntaxError as e:
             raise InvalidRequirement(str(e)) from e
 
         self.name: str = parsed.name
         if parsed.url:
             parsed_url = urllib.parse.urlparse(parsed.url)
             if parsed_url.scheme == "file":
```

### Comparing `modelbaker-1.4.3/modelbaker/libs/packaging/specifiers.py` & `modelbaker-1.4.4/modelbaker/libs/packaging/specifiers.py`

 * *Files 1% similar despite different names*

```diff
@@ -248,15 +248,16 @@
             match.group("operator").strip(),
             match.group("version").strip(),
         )
 
         # Store whether or not this Specifier should accept prereleases
         self._prereleases = prereleases
 
-    @property
+    # https://github.com/python/mypy/pull/13475#pullrequestreview-1079784515
+    @property  # type: ignore[override]
     def prereleases(self) -> bool:
         # If there is an explicit prereleases set for this, then we'll just
         # blindly use that.
         if self._prereleases is not None:
             return self._prereleases
 
         # Look at all of our specifiers and determine if they are inclusive
@@ -394,15 +395,17 @@
         )
 
     def _compare_equal(self, prospective: Version, spec: str) -> bool:
 
         # We need special logic to handle prefix matching
         if spec.endswith(".*"):
             # In the case of prefix matching we want to ignore local segment.
-            normalized_prospective = canonicalize_version(prospective.public)
+            normalized_prospective = canonicalize_version(
+                prospective.public, strip_trailing_zero=False
+            )
             # Get the normalized version string ignoring the trailing .*
             normalized_spec = canonicalize_version(spec[:-2], strip_trailing_zero=False)
             # Split the spec out by dots, and pretend that there is an implicit
             # dot in between a release segment and a pre-release segment.
             split_spec = _version_split(normalized_spec)
 
             # Split the prospective version out by dots, and pretend that there
```

### Comparing `modelbaker-1.4.3/modelbaker/libs/packaging/tags.py` & `modelbaker-1.4.4/modelbaker/libs/packaging/tags.py`

 * *Files 1% similar despite different names*

```diff
@@ -107,24 +107,24 @@
         for abi in abis.split("."):
             for platform_ in platforms.split("."):
                 tags.add(Tag(interpreter, abi, platform_))
     return frozenset(tags)
 
 
 def _get_config_var(name: str, warn: bool = False) -> Union[int, str, None]:
-    value = sysconfig.get_config_var(name)
+    value: Union[int, str, None] = sysconfig.get_config_var(name)
     if value is None and warn:
         logger.debug(
             "Config variable '%s' is unset, Python ABI tag may be incorrect", name
         )
     return value
 
 
 def _normalize_string(string: str) -> str:
-    return string.replace(".", "_").replace("-", "_")
+    return string.replace(".", "_").replace("-", "_").replace(" ", "_")
 
 
 def _abi3_applies(python_version: PythonVersion) -> bool:
     """
     Determine if the Python version supports abi3.
 
     PEP 384 was first implemented in Python 3.2.
```

### Comparing `modelbaker-1.4.3/modelbaker/libs/packaging/utils.py` & `modelbaker-1.4.4/modelbaker/libs/packaging/utils.py`

 * *Files identical despite different names*

### Comparing `modelbaker-1.4.3/modelbaker/libs/packaging/version.py` & `modelbaker-1.4.4/modelbaker/libs/packaging/version.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
     from packaging.version import parse, Version
 """
 
 import collections
 import itertools
 import re
-from typing import Callable, Optional, SupportsInt, Tuple, Union
+from typing import Any, Callable, Optional, SupportsInt, Tuple, Union
 
 from ._structures import Infinity, InfinityType, NegativeInfinity, NegativeInfinityType
 
 __all__ = ["VERSION_PATTERN", "parse", "Version", "InvalidVersion"]
 
 InfiniteTypes = Union[InfinityType, NegativeInfinityType]
 PrePostDevType = Union[InfiniteTypes, Tuple[str, int]]
@@ -59,15 +59,15 @@
     Traceback (most recent call last):
         ...
     packaging.version.InvalidVersion: Invalid version: 'invalid'
     """
 
 
 class _BaseVersion:
-    _key: CmpKey
+    _key: Tuple[Any, ...]
 
     def __hash__(self) -> int:
         return hash(self._key)
 
     # Please keep the duplicated `isinstance` check
     # in the six comparisons hereunder
     # unless you find a way to avoid adding overhead function calls.
@@ -175,14 +175,15 @@
     >>> v1 >= v2
     False
     >>> v1 <= v2
     True
     """
 
     _regex = re.compile(r"^\s*" + VERSION_PATTERN + r"\s*$", re.VERBOSE | re.IGNORECASE)
+    _key: CmpKey
 
     def __init__(self, version: str) -> None:
         """Initialize a Version object.
 
         :param version:
             The string representation of a version which will be parsed and normalized
             before use.
```

### Comparing `modelbaker-1.4.3/modelbaker/libs/pgserviceparser/__init__.py` & `modelbaker-1.4.4/modelbaker/libs/pgserviceparser/__init__.py`

 * *Files identical despite different names*

### Comparing `modelbaker-1.4.3/modelbaker/libs/toppingmaker/__init__.py` & `modelbaker-1.4.4/modelbaker/libs/toppingmaker/__init__.py`

 * *Files identical despite different names*

### Comparing `modelbaker-1.4.3/modelbaker/libs/toppingmaker/exportsettings.py` & `modelbaker-1.4.4/modelbaker/libs/toppingmaker/exportsettings.py`

 * *Files identical despite different names*

### Comparing `modelbaker-1.4.3/modelbaker/libs/toppingmaker/projecttopping.py` & `modelbaker-1.4.4/modelbaker/libs/toppingmaker/projecttopping.py`

 * *Files identical despite different names*

### Comparing `modelbaker-1.4.3/modelbaker/libs/toppingmaker/target.py` & `modelbaker-1.4.4/modelbaker/libs/toppingmaker/target.py`

 * *Files identical despite different names*

### Comparing `modelbaker-1.4.3/modelbaker/libs/toppingmaker/utils.py` & `modelbaker-1.4.4/modelbaker/libs/toppingmaker/utils.py`

 * *Files identical despite different names*

### Comparing `modelbaker-1.4.3/modelbaker/utils/db_utils.py` & `modelbaker-1.4.4/modelbaker/utils/db_utils.py`

 * *Files identical despite different names*

### Comparing `modelbaker-1.4.3/modelbaker/utils/globals.py` & `modelbaker-1.4.4/modelbaker/utils/globals.py`

 * *Files identical despite different names*

### Comparing `modelbaker-1.4.3/modelbaker/utils/qgis_utils.py` & `modelbaker-1.4.4/modelbaker/utils/qgis_utils.py`

 * *Files identical despite different names*

### Comparing `modelbaker-1.4.3/modelbaker/utils/qt_utils.py` & `modelbaker-1.4.4/modelbaker/utils/qt_utils.py`

 * *Files identical despite different names*

### Comparing `modelbaker-1.4.3/modelbaker.egg-info/PKG-INFO` & `modelbaker-1.4.4/modelbaker.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: modelbaker
-Version: 1.4.3
+Version: 1.4.4
 Summary: The full model baker core
 Home-page: https://github.com/opengisch/QgisModelBakerLibrary
 Author: Dave Signer
 Author-email: david@opengis.ch
 Classifier: Topic :: Database
 Classifier: License :: OSI Approved :: GNU General Public License v2 or later (GPLv2+)
 Classifier: Programming Language :: Python :: 3
@@ -93,25 +93,25 @@
     ├── db_utils.py
     ├── globals.py
     ├── qgis_utils.py
     └── qt_utils.py
 ```
 
 ### ili2db
-In the current release we use ili2db version 4.6.1
+In the current release we use ili2db version 4.10
 
 ## Infos for Devs
 
 ### Code style
 
 Is enforced with pre-commit. To use, make:
 ```
 pip install pre-commit
 pre-commit install
-```
+```00
 And to run it over all the files (with infile changes):
 ```
 pre-commit run --color=always --all-file
 ```
 
 ### Needed packages from PyPI
```

### Comparing `modelbaker-1.4.3/modelbaker.egg-info/SOURCES.txt` & `modelbaker-1.4.4/modelbaker.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -61,14 +61,15 @@
 modelbaker/libs/packaging/_elffile.py
 modelbaker/libs/packaging/_manylinux.py
 modelbaker/libs/packaging/_musllinux.py
 modelbaker/libs/packaging/_parser.py
 modelbaker/libs/packaging/_structures.py
 modelbaker/libs/packaging/_tokenizer.py
 modelbaker/libs/packaging/markers.py
+modelbaker/libs/packaging/metadata.py
 modelbaker/libs/packaging/requirements.py
 modelbaker/libs/packaging/specifiers.py
 modelbaker/libs/packaging/tags.py
 modelbaker/libs/packaging/utils.py
 modelbaker/libs/packaging/version.py
 modelbaker/libs/pgserviceparser/__init__.py
 modelbaker/libs/toppingmaker/__init__.py
```

### Comparing `modelbaker-1.4.3/setup.py` & `modelbaker-1.4.4/setup.py`

 * *Files identical despite different names*

### Comparing `modelbaker-1.4.3/tests/test_dataset_handling.py` & `modelbaker-1.4.4/tests/test_dataset_handling.py`

 * *Files identical despite different names*

### Comparing `modelbaker-1.4.3/tests/test_domain_class_relations.py` & `modelbaker-1.4.4/tests/test_domain_class_relations.py`

 * *Files identical despite different names*

### Comparing `modelbaker-1.4.3/tests/test_dump.py` & `modelbaker-1.4.4/tests/test_dump.py`

 * *Files identical despite different names*

### Comparing `modelbaker-1.4.3/tests/test_export.py` & `modelbaker-1.4.4/tests/test_export.py`

 * *Files identical despite different names*

### Comparing `modelbaker-1.4.3/tests/test_get_models.py` & `modelbaker-1.4.4/tests/test_get_models.py`

 * *Files identical despite different names*

### Comparing `modelbaker-1.4.3/tests/test_gpkg_pk.py` & `modelbaker-1.4.4/tests/test_gpkg_pk.py`

 * *Files identical despite different names*

### Comparing `modelbaker-1.4.3/tests/test_ili2dbutils.py` & `modelbaker-1.4.4/tests/test_ili2dbutils.py`

 * *Files identical despite different names*

### Comparing `modelbaker-1.4.3/tests/test_ilicache.py` & `modelbaker-1.4.4/tests/test_ilicache.py`

 * *Files identical despite different names*

### Comparing `modelbaker-1.4.3/tests/test_ilitoppingmaker.py` & `modelbaker-1.4.4/tests/test_ilitoppingmaker.py`

 * *Files identical despite different names*

### Comparing `modelbaker-1.4.3/tests/test_import.py` & `modelbaker-1.4.4/tests/test_import.py`

 * *Files identical despite different names*

### Comparing `modelbaker-1.4.3/tests/test_libili2pg.py` & `modelbaker-1.4.4/tests/test_libili2pg.py`

 * *Files identical despite different names*

### Comparing `modelbaker-1.4.3/tests/test_metaconfig.py` & `modelbaker-1.4.4/tests/test_metaconfig.py`

 * *Files identical despite different names*

### Comparing `modelbaker-1.4.3/tests/test_pgservice.py` & `modelbaker-1.4.4/tests/test_pgservice.py`

 * *Files identical despite different names*

### Comparing `modelbaker-1.4.3/tests/test_plugin.py` & `modelbaker-1.4.4/tests/test_plugin.py`

 * *Files identical despite different names*

### Comparing `modelbaker-1.4.3/tests/test_projectgen.py` & `modelbaker-1.4.4/tests/test_projectgen.py`

 * *Files identical despite different names*

### Comparing `modelbaker-1.4.3/tests/test_projectgen_generic_databases.py` & `modelbaker-1.4.4/tests/test_projectgen_generic_databases.py`

 * *Files identical despite different names*

### Comparing `modelbaker-1.4.3/tests/test_projecttopping.py` & `modelbaker-1.4.4/tests/test_projecttopping.py`

 * *Files identical despite different names*

### Comparing `modelbaker-1.4.3/tests/test_update.py` & `modelbaker-1.4.4/tests/test_update.py`

 * *Files identical despite different names*

### Comparing `modelbaker-1.4.3/tests/test_validate.py` & `modelbaker-1.4.4/tests/test_validate.py`

 * *Files identical despite different names*

### Comparing `modelbaker-1.4.3/tests/test_z_geom.py` & `modelbaker-1.4.4/tests/test_z_geom.py`

 * *Files identical despite different names*

