# Comparing `tmp/DynamicAnnotationDB-5.7.2.tar.gz` & `tmp/DynamicAnnotationDB-5.7.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "DynamicAnnotationDB-5.7.2.tar", last modified: Wed Apr 19 23:49:19 2023, max compression
+gzip compressed data, was "DynamicAnnotationDB-5.7.3.tar", last modified: Thu May  4 23:03:43 2023, max compression
```

## Comparing `DynamicAnnotationDB-5.7.2.tar` & `DynamicAnnotationDB-5.7.3.tar`

### file list

```diff
@@ -1,52 +1,52 @@
-drwxr-xr-x   0 forrestc   (503) staff       (20)        0 2023-04-19 23:49:19.337492 DynamicAnnotationDB-5.7.2/
-drwxr-xr-x   0 forrestc   (503) staff       (20)        0 2023-04-19 23:49:19.325642 DynamicAnnotationDB-5.7.2/DynamicAnnotationDB.egg-info/
--rw-r--r--   0 forrestc   (503) staff       (20)      920 2023-04-19 23:49:19.000000 DynamicAnnotationDB-5.7.2/DynamicAnnotationDB.egg-info/PKG-INFO
--rw-r--r--   0 forrestc   (503) staff       (20)     1821 2023-04-19 23:49:19.000000 DynamicAnnotationDB-5.7.2/DynamicAnnotationDB.egg-info/SOURCES.txt
--rw-r--r--   0 forrestc   (503) staff       (20)        1 2023-04-19 23:49:19.000000 DynamicAnnotationDB-5.7.2/DynamicAnnotationDB.egg-info/dependency_links.txt
--rw-r--r--   0 forrestc   (503) staff       (20)      125 2023-04-19 23:49:19.000000 DynamicAnnotationDB-5.7.2/DynamicAnnotationDB.egg-info/requires.txt
--rw-r--r--   0 forrestc   (503) staff       (20)       26 2023-04-19 23:49:19.000000 DynamicAnnotationDB-5.7.2/DynamicAnnotationDB.egg-info/top_level.txt
--rw-r--r--   0 forrestc   (503) staff       (20)       36 2020-06-11 04:40:08.000000 DynamicAnnotationDB-5.7.2/MANIFEST.in
--rw-r--r--   0 forrestc   (503) staff       (20)      920 2023-04-19 23:49:19.337657 DynamicAnnotationDB-5.7.2/PKG-INFO
--rw-r--r--   0 forrestc   (503) staff       (20)      474 2022-02-12 21:27:58.000000 DynamicAnnotationDB-5.7.2/README.md
--rw-r--r--   0 forrestc   (503) staff       (20)       67 2021-06-03 21:07:33.000000 DynamicAnnotationDB-5.7.2/doc_requirements.txt
-drwxr-xr-x   0 forrestc   (503) staff       (20)        0 2023-04-19 23:49:19.328553 DynamicAnnotationDB-5.7.2/dynamicannotationdb/
--rw-r--r--   0 forrestc   (503) staff       (20)       72 2023-04-19 23:49:15.000000 DynamicAnnotationDB-5.7.2/dynamicannotationdb/__init__.py
--rw-r--r--   0 forrestc   (503) staff       (20)    18140 2023-04-19 14:20:52.000000 DynamicAnnotationDB-5.7.2/dynamicannotationdb/annotation.py
--rw-r--r--   0 forrestc   (503) staff       (20)    13198 2023-04-18 17:23:16.000000 DynamicAnnotationDB-5.7.2/dynamicannotationdb/database.py
--rw-r--r--   0 forrestc   (503) staff       (20)     2064 2023-02-17 16:48:08.000000 DynamicAnnotationDB-5.7.2/dynamicannotationdb/errors.py
--rw-r--r--   0 forrestc   (503) staff       (20)     5969 2023-04-18 17:23:16.000000 DynamicAnnotationDB-5.7.2/dynamicannotationdb/interface.py
--rw-r--r--   0 forrestc   (503) staff       (20)     1139 2022-06-23 21:40:16.000000 DynamicAnnotationDB-5.7.2/dynamicannotationdb/key_utils.py
-drwxr-xr-x   0 forrestc   (503) staff       (20)        0 2023-04-19 23:49:19.329157 DynamicAnnotationDB-5.7.2/dynamicannotationdb/migration/
--rw-r--r--   0 forrestc   (503) staff       (20)      166 2023-04-19 23:49:15.000000 DynamicAnnotationDB-5.7.2/dynamicannotationdb/migration/__init__.py
-drwxr-xr-x   0 forrestc   (503) staff       (20)        0 2023-04-19 23:49:19.329951 DynamicAnnotationDB-5.7.2/dynamicannotationdb/migration/alembic/
--rw-r--r--   0 forrestc   (503) staff       (20)        0 2022-10-17 01:08:23.000000 DynamicAnnotationDB-5.7.2/dynamicannotationdb/migration/alembic/__init__.py
--rw-r--r--   0 forrestc   (503) staff       (20)     2373 2023-04-06 22:59:46.000000 DynamicAnnotationDB-5.7.2/dynamicannotationdb/migration/alembic/env.py
--rw-r--r--   0 forrestc   (503) staff       (20)     1100 2022-10-17 01:08:23.000000 DynamicAnnotationDB-5.7.2/dynamicannotationdb/migration/alembic/run.py
-drwxr-xr-x   0 forrestc   (503) staff       (20)        0 2023-04-19 23:49:19.334107 DynamicAnnotationDB-5.7.2/dynamicannotationdb/migration/alembic/versions/
--rw-r--r--   0 forrestc   (503) staff       (20)      747 2022-10-25 16:40:35.000000 DynamicAnnotationDB-5.7.2/dynamicannotationdb/migration/alembic/versions/309cf493a1e2_adding_warning_field.py
--rw-r--r--   0 forrestc   (503) staff       (20)      969 2022-10-17 01:08:23.000000 DynamicAnnotationDB-5.7.2/dynamicannotationdb/migration/alembic/versions/5a1d7c0ad006_add_status_column.py
--rw-r--r--   0 forrestc   (503) staff       (20)      515 2022-10-17 01:08:23.000000 DynamicAnnotationDB-5.7.2/dynamicannotationdb/migration/alembic/versions/6e7f580ff680_add_error_msg.py
--rw-r--r--   0 forrestc   (503) staff       (20)     1255 2023-04-06 22:59:46.000000 DynamicAnnotationDB-5.7.2/dynamicannotationdb/migration/alembic/versions/7c79eff751b4_add_parent_version_column.py
--rw-r--r--   0 forrestc   (503) staff       (20)     1063 2022-10-17 01:08:23.000000 DynamicAnnotationDB-5.7.2/dynamicannotationdb/migration/alembic/versions/814d72d74e3b_add_version_error_table.py
--rw-r--r--   0 forrestc   (503) staff       (20)     2066 2022-10-25 19:07:59.000000 DynamicAnnotationDB-5.7.2/dynamicannotationdb/migration/alembic/versions/8fdc843fc202_adding_permission_and_last_modified.py
--rw-r--r--   0 forrestc   (503) staff       (20)      685 2022-10-17 01:08:23.000000 DynamicAnnotationDB-5.7.2/dynamicannotationdb/migration/alembic/versions/975a79461cab_add_is_merged.py
--rw-r--r--   0 forrestc   (503) staff       (20)        0 2022-10-17 01:08:23.000000 DynamicAnnotationDB-5.7.2/dynamicannotationdb/migration/alembic/versions/__init__.py
--rw-r--r--   0 forrestc   (503) staff       (20)     4403 2023-04-06 22:59:46.000000 DynamicAnnotationDB-5.7.2/dynamicannotationdb/migration/alembic/versions/ef5c2d7f96d8_initial_live_db_models.py
--rw-r--r--   0 forrestc   (503) staff       (20)     1102 2023-03-14 16:48:52.000000 DynamicAnnotationDB-5.7.2/dynamicannotationdb/migration/alembic/versions/fac66b439033_add_view_model.py
--rw-r--r--   0 forrestc   (503) staff       (20)    22717 2023-04-19 23:49:05.000000 DynamicAnnotationDB-5.7.2/dynamicannotationdb/migration/migrate.py
--rw-r--r--   0 forrestc   (503) staff       (20)     6017 2023-04-19 14:20:52.000000 DynamicAnnotationDB-5.7.2/dynamicannotationdb/models.py
--rw-r--r--   0 forrestc   (503) staff       (20)     8351 2023-02-18 02:07:45.000000 DynamicAnnotationDB-5.7.2/dynamicannotationdb/schema.py
--rw-r--r--   0 forrestc   (503) staff       (20)    13779 2022-10-17 01:08:23.000000 DynamicAnnotationDB-5.7.2/dynamicannotationdb/segmentation.py
--rw-r--r--   0 forrestc   (503) staff       (20)      124 2022-11-21 01:05:53.000000 DynamicAnnotationDB-5.7.2/requirements.txt
--rw-r--r--   0 forrestc   (503) staff       (20)      140 2023-04-19 23:49:19.338162 DynamicAnnotationDB-5.7.2/setup.cfg
--rw-r--r--   0 forrestc   (503) staff       (20)     1303 2022-02-12 21:27:58.000000 DynamicAnnotationDB-5.7.2/setup.py
--rw-r--r--   0 forrestc   (503) staff       (20)       68 2021-06-03 21:07:33.000000 DynamicAnnotationDB-5.7.2/test_requirements.txt
-drwxr-xr-x   0 forrestc   (503) staff       (20)        0 2023-04-19 23:49:19.337201 DynamicAnnotationDB-5.7.2/tests/
--rw-r--r--   0 forrestc   (503) staff       (20)        0 2021-02-19 03:45:38.000000 DynamicAnnotationDB-5.7.2/tests/__init__.py
--rw-r--r--   0 forrestc   (503) staff       (20)     3308 2022-06-23 21:40:16.000000 DynamicAnnotationDB-5.7.2/tests/conftest.py
--rw-r--r--   0 forrestc   (503) staff       (20)     7393 2023-02-17 16:48:08.000000 DynamicAnnotationDB-5.7.2/tests/test_annotation.py
--rw-r--r--   0 forrestc   (503) staff       (20)     3799 2023-02-17 16:48:08.000000 DynamicAnnotationDB-5.7.2/tests/test_database.py
--rw-r--r--   0 forrestc   (503) staff       (20)     1433 2022-06-23 21:40:16.000000 DynamicAnnotationDB-5.7.2/tests/test_errors.py
--rw-r--r--   0 forrestc   (503) staff       (20)      391 2022-06-23 21:40:16.000000 DynamicAnnotationDB-5.7.2/tests/test_interface.py
--rw-r--r--   0 forrestc   (503) staff       (20)     3982 2022-09-13 20:07:43.000000 DynamicAnnotationDB-5.7.2/tests/test_schema.py
--rw-r--r--   0 forrestc   (503) staff       (20)     5705 2023-02-17 16:48:08.000000 DynamicAnnotationDB-5.7.2/tests/test_segmentation.py
+drwxr-xr-x   0 forrestc   (503) staff       (20)        0 2023-05-04 23:03:43.517332 DynamicAnnotationDB-5.7.3/
+drwxr-xr-x   0 forrestc   (503) staff       (20)        0 2023-05-04 23:03:43.495562 DynamicAnnotationDB-5.7.3/DynamicAnnotationDB.egg-info/
+-rw-r--r--   0 forrestc   (503) staff       (20)      920 2023-05-04 23:03:43.000000 DynamicAnnotationDB-5.7.3/DynamicAnnotationDB.egg-info/PKG-INFO
+-rw-r--r--   0 forrestc   (503) staff       (20)     1821 2023-05-04 23:03:43.000000 DynamicAnnotationDB-5.7.3/DynamicAnnotationDB.egg-info/SOURCES.txt
+-rw-r--r--   0 forrestc   (503) staff       (20)        1 2023-05-04 23:03:43.000000 DynamicAnnotationDB-5.7.3/DynamicAnnotationDB.egg-info/dependency_links.txt
+-rw-r--r--   0 forrestc   (503) staff       (20)      125 2023-05-04 23:03:43.000000 DynamicAnnotationDB-5.7.3/DynamicAnnotationDB.egg-info/requires.txt
+-rw-r--r--   0 forrestc   (503) staff       (20)       26 2023-05-04 23:03:43.000000 DynamicAnnotationDB-5.7.3/DynamicAnnotationDB.egg-info/top_level.txt
+-rw-r--r--   0 forrestc   (503) staff       (20)       36 2020-06-11 04:40:08.000000 DynamicAnnotationDB-5.7.3/MANIFEST.in
+-rw-r--r--   0 forrestc   (503) staff       (20)      920 2023-05-04 23:03:43.517625 DynamicAnnotationDB-5.7.3/PKG-INFO
+-rw-r--r--   0 forrestc   (503) staff       (20)      474 2022-02-12 21:27:58.000000 DynamicAnnotationDB-5.7.3/README.md
+-rw-r--r--   0 forrestc   (503) staff       (20)       67 2021-06-03 21:07:33.000000 DynamicAnnotationDB-5.7.3/doc_requirements.txt
+drwxr-xr-x   0 forrestc   (503) staff       (20)        0 2023-05-04 23:03:43.500064 DynamicAnnotationDB-5.7.3/dynamicannotationdb/
+-rw-r--r--   0 forrestc   (503) staff       (20)       72 2023-05-04 23:03:40.000000 DynamicAnnotationDB-5.7.3/dynamicannotationdb/__init__.py
+-rw-r--r--   0 forrestc   (503) staff       (20)    18101 2023-05-04 23:03:31.000000 DynamicAnnotationDB-5.7.3/dynamicannotationdb/annotation.py
+-rw-r--r--   0 forrestc   (503) staff       (20)    13198 2023-04-18 17:23:16.000000 DynamicAnnotationDB-5.7.3/dynamicannotationdb/database.py
+-rw-r--r--   0 forrestc   (503) staff       (20)     2064 2023-02-17 16:48:08.000000 DynamicAnnotationDB-5.7.3/dynamicannotationdb/errors.py
+-rw-r--r--   0 forrestc   (503) staff       (20)     5969 2023-04-18 17:23:16.000000 DynamicAnnotationDB-5.7.3/dynamicannotationdb/interface.py
+-rw-r--r--   0 forrestc   (503) staff       (20)     1139 2022-06-23 21:40:16.000000 DynamicAnnotationDB-5.7.3/dynamicannotationdb/key_utils.py
+drwxr-xr-x   0 forrestc   (503) staff       (20)        0 2023-05-04 23:03:43.501444 DynamicAnnotationDB-5.7.3/dynamicannotationdb/migration/
+-rw-r--r--   0 forrestc   (503) staff       (20)      166 2023-05-04 23:03:40.000000 DynamicAnnotationDB-5.7.3/dynamicannotationdb/migration/__init__.py
+drwxr-xr-x   0 forrestc   (503) staff       (20)        0 2023-05-04 23:03:43.502650 DynamicAnnotationDB-5.7.3/dynamicannotationdb/migration/alembic/
+-rw-r--r--   0 forrestc   (503) staff       (20)        0 2022-10-17 01:08:23.000000 DynamicAnnotationDB-5.7.3/dynamicannotationdb/migration/alembic/__init__.py
+-rw-r--r--   0 forrestc   (503) staff       (20)     2373 2023-04-06 22:59:46.000000 DynamicAnnotationDB-5.7.3/dynamicannotationdb/migration/alembic/env.py
+-rw-r--r--   0 forrestc   (503) staff       (20)     1100 2022-10-17 01:08:23.000000 DynamicAnnotationDB-5.7.3/dynamicannotationdb/migration/alembic/run.py
+drwxr-xr-x   0 forrestc   (503) staff       (20)        0 2023-05-04 23:03:43.511556 DynamicAnnotationDB-5.7.3/dynamicannotationdb/migration/alembic/versions/
+-rw-r--r--   0 forrestc   (503) staff       (20)      747 2022-10-25 16:40:35.000000 DynamicAnnotationDB-5.7.3/dynamicannotationdb/migration/alembic/versions/309cf493a1e2_adding_warning_field.py
+-rw-r--r--   0 forrestc   (503) staff       (20)      969 2022-10-17 01:08:23.000000 DynamicAnnotationDB-5.7.3/dynamicannotationdb/migration/alembic/versions/5a1d7c0ad006_add_status_column.py
+-rw-r--r--   0 forrestc   (503) staff       (20)      515 2022-10-17 01:08:23.000000 DynamicAnnotationDB-5.7.3/dynamicannotationdb/migration/alembic/versions/6e7f580ff680_add_error_msg.py
+-rw-r--r--   0 forrestc   (503) staff       (20)     1255 2023-04-06 22:59:46.000000 DynamicAnnotationDB-5.7.3/dynamicannotationdb/migration/alembic/versions/7c79eff751b4_add_parent_version_column.py
+-rw-r--r--   0 forrestc   (503) staff       (20)     1063 2022-10-17 01:08:23.000000 DynamicAnnotationDB-5.7.3/dynamicannotationdb/migration/alembic/versions/814d72d74e3b_add_version_error_table.py
+-rw-r--r--   0 forrestc   (503) staff       (20)     2066 2022-10-25 19:07:59.000000 DynamicAnnotationDB-5.7.3/dynamicannotationdb/migration/alembic/versions/8fdc843fc202_adding_permission_and_last_modified.py
+-rw-r--r--   0 forrestc   (503) staff       (20)      685 2022-10-17 01:08:23.000000 DynamicAnnotationDB-5.7.3/dynamicannotationdb/migration/alembic/versions/975a79461cab_add_is_merged.py
+-rw-r--r--   0 forrestc   (503) staff       (20)        0 2022-10-17 01:08:23.000000 DynamicAnnotationDB-5.7.3/dynamicannotationdb/migration/alembic/versions/__init__.py
+-rw-r--r--   0 forrestc   (503) staff       (20)     4403 2023-04-06 22:59:46.000000 DynamicAnnotationDB-5.7.3/dynamicannotationdb/migration/alembic/versions/ef5c2d7f96d8_initial_live_db_models.py
+-rw-r--r--   0 forrestc   (503) staff       (20)     1102 2023-03-14 16:48:52.000000 DynamicAnnotationDB-5.7.3/dynamicannotationdb/migration/alembic/versions/fac66b439033_add_view_model.py
+-rw-r--r--   0 forrestc   (503) staff       (20)    22717 2023-04-19 23:49:05.000000 DynamicAnnotationDB-5.7.3/dynamicannotationdb/migration/migrate.py
+-rw-r--r--   0 forrestc   (503) staff       (20)     6017 2023-04-19 14:20:52.000000 DynamicAnnotationDB-5.7.3/dynamicannotationdb/models.py
+-rw-r--r--   0 forrestc   (503) staff       (20)     8351 2023-02-18 02:07:45.000000 DynamicAnnotationDB-5.7.3/dynamicannotationdb/schema.py
+-rw-r--r--   0 forrestc   (503) staff       (20)    13779 2022-10-17 01:08:23.000000 DynamicAnnotationDB-5.7.3/dynamicannotationdb/segmentation.py
+-rw-r--r--   0 forrestc   (503) staff       (20)      124 2022-11-21 01:05:53.000000 DynamicAnnotationDB-5.7.3/requirements.txt
+-rw-r--r--   0 forrestc   (503) staff       (20)      140 2023-05-04 23:03:43.519103 DynamicAnnotationDB-5.7.3/setup.cfg
+-rw-r--r--   0 forrestc   (503) staff       (20)     1303 2022-02-12 21:27:58.000000 DynamicAnnotationDB-5.7.3/setup.py
+-rw-r--r--   0 forrestc   (503) staff       (20)       68 2021-06-03 21:07:33.000000 DynamicAnnotationDB-5.7.3/test_requirements.txt
+drwxr-xr-x   0 forrestc   (503) staff       (20)        0 2023-05-04 23:03:43.516375 DynamicAnnotationDB-5.7.3/tests/
+-rw-r--r--   0 forrestc   (503) staff       (20)        0 2021-02-19 03:45:38.000000 DynamicAnnotationDB-5.7.3/tests/__init__.py
+-rw-r--r--   0 forrestc   (503) staff       (20)     3308 2022-06-23 21:40:16.000000 DynamicAnnotationDB-5.7.3/tests/conftest.py
+-rw-r--r--   0 forrestc   (503) staff       (20)     7393 2023-02-17 16:48:08.000000 DynamicAnnotationDB-5.7.3/tests/test_annotation.py
+-rw-r--r--   0 forrestc   (503) staff       (20)     3799 2023-02-17 16:48:08.000000 DynamicAnnotationDB-5.7.3/tests/test_database.py
+-rw-r--r--   0 forrestc   (503) staff       (20)     1433 2022-06-23 21:40:16.000000 DynamicAnnotationDB-5.7.3/tests/test_errors.py
+-rw-r--r--   0 forrestc   (503) staff       (20)      391 2022-06-23 21:40:16.000000 DynamicAnnotationDB-5.7.3/tests/test_interface.py
+-rw-r--r--   0 forrestc   (503) staff       (20)     3982 2022-09-13 20:07:43.000000 DynamicAnnotationDB-5.7.3/tests/test_schema.py
+-rw-r--r--   0 forrestc   (503) staff       (20)     5705 2023-02-17 16:48:08.000000 DynamicAnnotationDB-5.7.3/tests/test_segmentation.py
```

### Comparing `DynamicAnnotationDB-5.7.2/DynamicAnnotationDB.egg-info/PKG-INFO` & `DynamicAnnotationDB-5.7.3/DynamicAnnotationDB.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: DynamicAnnotationDB
-Version: 5.7.2
+Version: 5.7.3
 Summary: Annotation Database pendant to the chunkedgraph
 Home-page: https://github.com/seung-lab/DynamicAnnotationDB
 Author: Sven Dorkenwald, Derrick Brittain
 Author-email: sdorkenw@princeton.edu
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: POSIX :: Linux
```

### Comparing `DynamicAnnotationDB-5.7.2/DynamicAnnotationDB.egg-info/SOURCES.txt` & `DynamicAnnotationDB-5.7.3/DynamicAnnotationDB.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `DynamicAnnotationDB-5.7.2/PKG-INFO` & `DynamicAnnotationDB-5.7.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: DynamicAnnotationDB
-Version: 5.7.2
+Version: 5.7.3
 Summary: Annotation Database pendant to the chunkedgraph
 Home-page: https://github.com/seung-lab/DynamicAnnotationDB
 Author: Sven Dorkenwald, Derrick Brittain
 Author-email: sdorkenw@princeton.edu
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: POSIX :: Linux
```

### Comparing `DynamicAnnotationDB-5.7.2/dynamicannotationdb/annotation.py` & `DynamicAnnotationDB-5.7.3/dynamicannotationdb/annotation.py`

 * *Files 2% similar despite different names*

```diff
@@ -322,23 +322,15 @@
             Exception raised when amount of annotations exceeds defined limit.
         """
         insertion_limit = 10_000
 
         if len(annotations) > insertion_limit:
             raise AnnotationInsertLimitExceeded(insertion_limit, len(annotations))
 
-        metadata = self.db.get_table_metadata(table_name)
-        schema_type = metadata["schema_type"]
-        
-        # load reference table into metadata if not already present 
-        ref_table = metadata.get("reference_table")
-        if ref_table:
-            reference_table_name = self.db.cached_table(ref_table)
-
-        AnnotationModel = self.db.cached_table(table_name)
+        schema_type, AnnotationModel = self._load_model(table_name)
 
         formatted_anno_data = []
         for annotation in annotations:
 
             annotation_data, __ = self.schema.split_flattened_schema_data(
                 schema_type, annotation
             )
@@ -378,25 +370,22 @@
             list of annotation ids to get
 
         Returns
         -------
         List[dict]
             list of returned annotations
         """
-        AnnotationModel = self.db.cached_table(table_name)
+        schema_type, AnnotationModel = self._load_model(table_name)
 
         annotations = (
             self.db.cached_session.query(AnnotationModel)
             .filter(AnnotationModel.id.in_(list(annotation_ids)))
             .all()
         )
 
-        metadata = self.db.get_table_metadata(table_name)
-        schema_type = metadata["schema_type"]
-
         anno_schema, __ = self.schema.split_flattened_schema(schema_type)
         schema = anno_schema(unknown=INCLUDE)
         try:
             data = []
 
             for anno in annotations:
                 anno_data = anno.__dict__
@@ -432,18 +421,16 @@
         ------
         NoAnnotationsFoundWithID:
             Raises if no Ids to be updated are found in the table.
         """
         anno_id = annotation.get("id")
         if not anno_id:
             return "Annotation requires an 'id' to update targeted row"
-        metadata = self.db.get_table_metadata(table_name)
-        schema_type = metadata["schema_type"]
+        schema_type, AnnotationModel = self._load_model(table_name)
 
-        AnnotationModel = self.db.cached_table(table_name)
         new_annotation, __ = self.schema.split_flattened_schema_data(
             schema_type, annotation
         )
 
         if hasattr(AnnotationModel, "created"):
             new_annotation["created"] = datetime.datetime.utcnow()
         if hasattr(AnnotationModel, "valid"):
@@ -500,15 +487,15 @@
             list of ids to delete
 
         Returns
         -------
         List[int]:
             List of ids that were marked as deleted and no longer valid.
         """
-        AnnotationModel = self.db.cached_table(table_name)
+        schema_type, AnnotationModel = self._load_model(table_name)
 
         annotations = (
             self.db.cached_session.query(AnnotationModel)
             .filter(AnnotationModel.id.in_(annotation_ids))
             .all()
         )
         deleted_ids = []
@@ -532,7 +519,19 @@
             )
 
             self.db.commit_session()
 
         else:
             return None
         return deleted_ids
+
+    def _load_model(self, table_name):
+        metadata = self.db.get_table_metadata(table_name)
+        schema_type = metadata["schema_type"]
+
+        # load reference table into metadata if not already present
+        ref_table = metadata.get("reference_table")
+        if ref_table:
+            reference_table_name = self.db.cached_table(ref_table)
+
+        AnnotationModel = self.db.cached_table(table_name)
+        return schema_type, AnnotationModel
```

### Comparing `DynamicAnnotationDB-5.7.2/dynamicannotationdb/database.py` & `DynamicAnnotationDB-5.7.3/dynamicannotationdb/database.py`

 * *Files identical despite different names*

### Comparing `DynamicAnnotationDB-5.7.2/dynamicannotationdb/errors.py` & `DynamicAnnotationDB-5.7.3/dynamicannotationdb/errors.py`

 * *Files identical despite different names*

### Comparing `DynamicAnnotationDB-5.7.2/dynamicannotationdb/interface.py` & `DynamicAnnotationDB-5.7.3/dynamicannotationdb/interface.py`

 * *Files identical despite different names*

### Comparing `DynamicAnnotationDB-5.7.2/dynamicannotationdb/key_utils.py` & `DynamicAnnotationDB-5.7.3/dynamicannotationdb/key_utils.py`

 * *Files identical despite different names*

### Comparing `DynamicAnnotationDB-5.7.2/dynamicannotationdb/migration/alembic/env.py` & `DynamicAnnotationDB-5.7.3/dynamicannotationdb/migration/alembic/env.py`

 * *Files identical despite different names*

### Comparing `DynamicAnnotationDB-5.7.2/dynamicannotationdb/migration/alembic/run.py` & `DynamicAnnotationDB-5.7.3/dynamicannotationdb/migration/alembic/run.py`

 * *Files identical despite different names*

### Comparing `DynamicAnnotationDB-5.7.2/dynamicannotationdb/migration/alembic/versions/309cf493a1e2_adding_warning_field.py` & `DynamicAnnotationDB-5.7.3/dynamicannotationdb/migration/alembic/versions/309cf493a1e2_adding_warning_field.py`

 * *Files identical despite different names*

### Comparing `DynamicAnnotationDB-5.7.2/dynamicannotationdb/migration/alembic/versions/5a1d7c0ad006_add_status_column.py` & `DynamicAnnotationDB-5.7.3/dynamicannotationdb/migration/alembic/versions/5a1d7c0ad006_add_status_column.py`

 * *Files identical despite different names*

### Comparing `DynamicAnnotationDB-5.7.2/dynamicannotationdb/migration/alembic/versions/6e7f580ff680_add_error_msg.py` & `DynamicAnnotationDB-5.7.3/dynamicannotationdb/migration/alembic/versions/6e7f580ff680_add_error_msg.py`

 * *Files identical despite different names*

### Comparing `DynamicAnnotationDB-5.7.2/dynamicannotationdb/migration/alembic/versions/7c79eff751b4_add_parent_version_column.py` & `DynamicAnnotationDB-5.7.3/dynamicannotationdb/migration/alembic/versions/7c79eff751b4_add_parent_version_column.py`

 * *Files identical despite different names*

### Comparing `DynamicAnnotationDB-5.7.2/dynamicannotationdb/migration/alembic/versions/814d72d74e3b_add_version_error_table.py` & `DynamicAnnotationDB-5.7.3/dynamicannotationdb/migration/alembic/versions/814d72d74e3b_add_version_error_table.py`

 * *Files identical despite different names*

### Comparing `DynamicAnnotationDB-5.7.2/dynamicannotationdb/migration/alembic/versions/8fdc843fc202_adding_permission_and_last_modified.py` & `DynamicAnnotationDB-5.7.3/dynamicannotationdb/migration/alembic/versions/8fdc843fc202_adding_permission_and_last_modified.py`

 * *Files identical despite different names*

### Comparing `DynamicAnnotationDB-5.7.2/dynamicannotationdb/migration/alembic/versions/975a79461cab_add_is_merged.py` & `DynamicAnnotationDB-5.7.3/dynamicannotationdb/migration/alembic/versions/975a79461cab_add_is_merged.py`

 * *Files identical despite different names*

### Comparing `DynamicAnnotationDB-5.7.2/dynamicannotationdb/migration/alembic/versions/ef5c2d7f96d8_initial_live_db_models.py` & `DynamicAnnotationDB-5.7.3/dynamicannotationdb/migration/alembic/versions/ef5c2d7f96d8_initial_live_db_models.py`

 * *Files identical despite different names*

### Comparing `DynamicAnnotationDB-5.7.2/dynamicannotationdb/migration/alembic/versions/fac66b439033_add_view_model.py` & `DynamicAnnotationDB-5.7.3/dynamicannotationdb/migration/alembic/versions/fac66b439033_add_view_model.py`

 * *Files identical despite different names*

### Comparing `DynamicAnnotationDB-5.7.2/dynamicannotationdb/migration/migrate.py` & `DynamicAnnotationDB-5.7.3/dynamicannotationdb/migration/migrate.py`

 * *Files identical despite different names*

### Comparing `DynamicAnnotationDB-5.7.2/dynamicannotationdb/models.py` & `DynamicAnnotationDB-5.7.3/dynamicannotationdb/models.py`

 * *Files identical despite different names*

### Comparing `DynamicAnnotationDB-5.7.2/dynamicannotationdb/schema.py` & `DynamicAnnotationDB-5.7.3/dynamicannotationdb/schema.py`

 * *Files identical despite different names*

### Comparing `DynamicAnnotationDB-5.7.2/dynamicannotationdb/segmentation.py` & `DynamicAnnotationDB-5.7.3/dynamicannotationdb/segmentation.py`

 * *Files identical despite different names*

### Comparing `DynamicAnnotationDB-5.7.2/setup.py` & `DynamicAnnotationDB-5.7.3/setup.py`

 * *Files identical despite different names*

### Comparing `DynamicAnnotationDB-5.7.2/tests/conftest.py` & `DynamicAnnotationDB-5.7.3/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `DynamicAnnotationDB-5.7.2/tests/test_annotation.py` & `DynamicAnnotationDB-5.7.3/tests/test_annotation.py`

 * *Files identical despite different names*

### Comparing `DynamicAnnotationDB-5.7.2/tests/test_database.py` & `DynamicAnnotationDB-5.7.3/tests/test_database.py`

 * *Files identical despite different names*

### Comparing `DynamicAnnotationDB-5.7.2/tests/test_errors.py` & `DynamicAnnotationDB-5.7.3/tests/test_errors.py`

 * *Files identical despite different names*

### Comparing `DynamicAnnotationDB-5.7.2/tests/test_schema.py` & `DynamicAnnotationDB-5.7.3/tests/test_schema.py`

 * *Files identical despite different names*

### Comparing `DynamicAnnotationDB-5.7.2/tests/test_segmentation.py` & `DynamicAnnotationDB-5.7.3/tests/test_segmentation.py`

 * *Files identical despite different names*

