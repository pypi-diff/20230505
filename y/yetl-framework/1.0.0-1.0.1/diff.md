# Comparing `tmp/yetl-framework-1.0.0.tar.gz` & `tmp/yetl-framework-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "yetl-framework-1.0.0.tar", last modified: Thu May  4 12:16:49 2023, max compression
+gzip compressed data, was "yetl-framework-1.0.1.tar", last modified: Fri May  5 08:06:18 2023, max compression
```

## Comparing `yetl-framework-1.0.0.tar` & `yetl-framework-1.0.1.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-04 12:16:49.997215 yetl-framework-1.0.0/
--rw-r--r--   0 vsts      (1001) docker     (123)     4615 2023-05-04 12:16:49.997215 yetl-framework-1.0.0/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (123)     4118 2023-05-04 12:15:59.000000 yetl-framework-1.0.0/README.md
--rw-r--r--   0 vsts      (1001) docker     (123)       38 2023-05-04 12:16:49.997215 yetl-framework-1.0.0/setup.cfg
--rw-r--r--   0 vsts      (1001) docker     (123)     1043 2023-05-04 12:15:59.000000 yetl-framework-1.0.0/setup.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-04 12:16:49.993215 yetl-framework-1.0.0/yetl/
--rw-r--r--   0 vsts      (1001) docker     (123)      455 2023-05-04 12:15:59.000000 yetl-framework-1.0.0/yetl/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (123)     3148 2023-05-04 12:15:59.000000 yetl-framework-1.0.0/yetl/_config.py
--rw-r--r--   0 vsts      (1001) docker     (123)     1994 2023-05-04 12:15:59.000000 yetl-framework-1.0.0/yetl/_decorators.py
--rw-r--r--   0 vsts      (1001) docker     (123)     2033 2023-05-04 12:15:59.000000 yetl-framework-1.0.0/yetl/_logging_config.py
--rw-r--r--   0 vsts      (1001) docker     (123)     1893 2023-05-04 12:15:59.000000 yetl-framework-1.0.0/yetl/_project.py
--rw-r--r--   0 vsts      (1001) docker     (123)     1399 2023-05-04 12:15:59.000000 yetl-framework-1.0.0/yetl/_spark_context.py
--rw-r--r--   0 vsts      (1001) docker     (123)      158 2023-05-04 12:15:59.000000 yetl-framework-1.0.0/yetl/_stage_type.py
--rw-r--r--   0 vsts      (1001) docker     (123)      305 2023-05-04 12:15:59.000000 yetl-framework-1.0.0/yetl/_table_mapping.py
--rw-r--r--   0 vsts      (1001) docker     (123)     7311 2023-05-04 12:15:59.000000 yetl-framework-1.0.0/yetl/_tables.py
--rw-r--r--   0 vsts      (1001) docker     (123)     5706 2023-05-04 12:15:59.000000 yetl-framework-1.0.0/yetl/_timeslice.py
--rw-r--r--   0 vsts      (1001) docker     (123)     4717 2023-05-04 12:15:59.000000 yetl-framework-1.0.0/yetl/_utils.py
--rw-r--r--   0 vsts      (1001) docker     (123)     6667 2023-05-04 12:15:59.000000 yetl-framework-1.0.0/yetl/datallake.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-04 12:16:49.993215 yetl-framework-1.0.0/yetl/dataset/
--rw-r--r--   0 vsts      (1001) docker     (123)      217 2023-05-04 12:15:59.000000 yetl-framework-1.0.0/yetl/dataset/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (123)     1203 2023-05-04 12:15:59.000000 yetl-framework-1.0.0/yetl/dataset/_dataset.py
--rw-r--r--   0 vsts      (1001) docker     (123)     3242 2023-05-04 12:15:59.000000 yetl-framework-1.0.0/yetl/dataset/_deltalake.py
--rw-r--r--   0 vsts      (1001) docker     (123)     3947 2023-05-04 12:15:59.000000 yetl-framework-1.0.0/yetl/dataset/_factory.py
--rw-r--r--   0 vsts      (1001) docker     (123)     5274 2023-05-04 12:15:59.000000 yetl-framework-1.0.0/yetl/dataset/_read.py
--rw-r--r--   0 vsts      (1001) docker     (123)      259 2023-05-04 12:15:59.000000 yetl-framework-1.0.0/yetl/dataset/_write.py
--rw-r--r--   0 vsts      (1001) docker     (123)      198 2023-05-04 12:15:59.000000 yetl-framework-1.0.0/yetl/dataset/dataset_type.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-04 12:16:49.993215 yetl-framework-1.0.0/yetl/workflow/
--rw-r--r--   0 vsts      (1001) docker     (123)      122 2023-05-04 12:15:59.000000 yetl-framework-1.0.0/yetl/workflow/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (123)     2596 2023-05-04 12:15:59.000000 yetl-framework-1.0.0/yetl/workflow/_multi_threaded.py
--rw-r--r--   0 vsts      (1001) docker     (123)      495 2023-05-04 12:15:59.000000 yetl-framework-1.0.0/yetl/workflow/_notebook.py
-drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-04 12:16:49.993215 yetl-framework-1.0.0/yetl_framework.egg-info/
--rw-r--r--   0 vsts      (1001) docker     (123)     4615 2023-05-04 12:16:49.000000 yetl-framework-1.0.0/yetl_framework.egg-info/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (123)      734 2023-05-04 12:16:49.000000 yetl-framework-1.0.0/yetl_framework.egg-info/SOURCES.txt
--rw-r--r--   0 vsts      (1001) docker     (123)        1 2023-05-04 12:16:49.000000 yetl-framework-1.0.0/yetl_framework.egg-info/dependency_links.txt
--rw-r--r--   0 vsts      (1001) docker     (123)        1 2023-05-04 12:16:49.000000 yetl-framework-1.0.0/yetl_framework.egg-info/not-zip-safe
--rw-r--r--   0 vsts      (1001) docker     (123)       23 2023-05-04 12:16:49.000000 yetl-framework-1.0.0/yetl_framework.egg-info/requires.txt
--rw-r--r--   0 vsts      (1001) docker     (123)        5 2023-05-04 12:16:49.000000 yetl-framework-1.0.0/yetl_framework.egg-info/top_level.txt
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-05 08:06:18.139489 yetl-framework-1.0.1/
+-rw-r--r--   0 vsts      (1001) docker     (123)     5770 2023-05-05 08:06:18.139489 yetl-framework-1.0.1/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (123)     5273 2023-05-05 08:05:21.000000 yetl-framework-1.0.1/README.md
+-rw-r--r--   0 vsts      (1001) docker     (123)       38 2023-05-05 08:06:18.139489 yetl-framework-1.0.1/setup.cfg
+-rw-r--r--   0 vsts      (1001) docker     (123)     1043 2023-05-05 08:05:21.000000 yetl-framework-1.0.1/setup.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-05 08:06:18.131489 yetl-framework-1.0.1/yetl/
+-rw-r--r--   0 vsts      (1001) docker     (123)      455 2023-05-05 08:05:21.000000 yetl-framework-1.0.1/yetl/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     3220 2023-05-05 08:05:21.000000 yetl-framework-1.0.1/yetl/_config.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     1994 2023-05-05 08:05:21.000000 yetl-framework-1.0.1/yetl/_decorators.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     2033 2023-05-05 08:05:21.000000 yetl-framework-1.0.1/yetl/_logging_config.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     1893 2023-05-05 08:05:21.000000 yetl-framework-1.0.1/yetl/_project.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     1399 2023-05-05 08:05:21.000000 yetl-framework-1.0.1/yetl/_spark_context.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      158 2023-05-05 08:05:21.000000 yetl-framework-1.0.1/yetl/_stage_type.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      305 2023-05-05 08:05:21.000000 yetl-framework-1.0.1/yetl/_table_mapping.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     7311 2023-05-05 08:05:21.000000 yetl-framework-1.0.1/yetl/_tables.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     5706 2023-05-05 08:05:21.000000 yetl-framework-1.0.1/yetl/_timeslice.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     4717 2023-05-05 08:05:21.000000 yetl-framework-1.0.1/yetl/_utils.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-05 08:06:18.135489 yetl-framework-1.0.1/yetl/dataset/
+-rw-r--r--   0 vsts      (1001) docker     (123)      217 2023-05-05 08:05:21.000000 yetl-framework-1.0.1/yetl/dataset/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     1268 2023-05-05 08:05:21.000000 yetl-framework-1.0.1/yetl/dataset/_dataset.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     3425 2023-05-05 08:05:21.000000 yetl-framework-1.0.1/yetl/dataset/_deltalake.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     4032 2023-05-05 08:05:21.000000 yetl-framework-1.0.1/yetl/dataset/_factory.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     5274 2023-05-05 08:05:21.000000 yetl-framework-1.0.1/yetl/dataset/_read.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      259 2023-05-05 08:05:21.000000 yetl-framework-1.0.1/yetl/dataset/_write.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      198 2023-05-05 08:05:21.000000 yetl-framework-1.0.1/yetl/dataset/dataset_type.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     7666 2023-05-05 08:05:21.000000 yetl-framework-1.0.1/yetl/deltalake.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-05 08:06:18.135489 yetl-framework-1.0.1/yetl/workflow/
+-rw-r--r--   0 vsts      (1001) docker     (123)      122 2023-05-05 08:05:21.000000 yetl-framework-1.0.1/yetl/workflow/__init__.py
+-rw-r--r--   0 vsts      (1001) docker     (123)     2596 2023-05-05 08:05:21.000000 yetl-framework-1.0.1/yetl/workflow/_multi_threaded.py
+-rw-r--r--   0 vsts      (1001) docker     (123)      495 2023-05-05 08:05:21.000000 yetl-framework-1.0.1/yetl/workflow/_notebook.py
+drwxr-xr-x   0 vsts      (1001) docker     (123)        0 2023-05-05 08:06:18.139489 yetl-framework-1.0.1/yetl_framework.egg-info/
+-rw-r--r--   0 vsts      (1001) docker     (123)     5770 2023-05-05 08:06:18.000000 yetl-framework-1.0.1/yetl_framework.egg-info/PKG-INFO
+-rw-r--r--   0 vsts      (1001) docker     (123)      734 2023-05-05 08:06:18.000000 yetl-framework-1.0.1/yetl_framework.egg-info/SOURCES.txt
+-rw-r--r--   0 vsts      (1001) docker     (123)        1 2023-05-05 08:06:18.000000 yetl-framework-1.0.1/yetl_framework.egg-info/dependency_links.txt
+-rw-r--r--   0 vsts      (1001) docker     (123)        1 2023-05-05 08:06:18.000000 yetl-framework-1.0.1/yetl_framework.egg-info/not-zip-safe
+-rw-r--r--   0 vsts      (1001) docker     (123)       23 2023-05-05 08:06:18.000000 yetl-framework-1.0.1/yetl_framework.egg-info/requires.txt
+-rw-r--r--   0 vsts      (1001) docker     (123)        5 2023-05-05 08:06:18.000000 yetl-framework-1.0.1/yetl_framework.egg-info/top_level.txt
```

### Comparing `yetl-framework-1.0.0/PKG-INFO` & `yetl-framework-1.0.1/README.md`

 * *Files 26% similar despite different names*

```diff
@@ -1,40 +1,31 @@
-Metadata-Version: 2.1
-Name: yetl-framework
-Version: 1.0.0
-Summary: yet (another spark) etl framework
-Home-page: https://www.yetl.io/
-Author: Shaun Ryan
-Author-email: shaun_chiburi@hotmail.com
-License: MIT
-Project-URL: GitHub, https://github.com/sibytes/yetl
-Project-URL: Documentation, https://www.yetl.io/
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
-Description-Content-Type: text/markdown
-
 # yetl
 
+Install
+```
+pip install yetl-framework
+```
+
 Configuration framework for databricks pipelines.
 Define configuration and table dependencies in yaml config then get the table mappings config model:
 
 Define your tables.
 
 ```yaml
-landing:
-  read:
+
+landing: # this is the landing stage in the deltalake house
+  read: # this is the type of spark asset that the pipeline needs to read
     landing_dbx_patterns:
       customer_details_1: null
       customer_details_2: null
 
-raw:
-  delta_lake:
-    raw_dbx_patterns:
-      customers:
+raw: # this is the bronze stage in the deltalake house
+  delta_lake: # this is the type of spark asset that the pipeline needs to read and write to
+    raw_dbx_patterns: # this is the database name
+      customers: # this is a table name and it's subsequent properties
         ids: id
         depends_on:
           - landing.landing_dbx_patterns.customer_details_1
           - landing.landing_dbx_patterns.customer_details_2
         warning_thresholds:
           invalid_ratio: 0.1
           invalid_rows: 0
@@ -44,55 +35,54 @@
           invalid_ratio: 0.2
           invalid_rows: 2
           max_rows: 1000
           min_rows: 0
         custom_properties:
           process_group: 1
 
-base:
-  delta_lake:
+base: # this is the silver stage in the delta lakehouse
+  delta_lake: # this is the type of spark asset that the pipeline needs to read and write to
     # delta table properties can be set at stage level or table level
     delta_properties:
       delta.appendOnly: true
       delta.autoOptimize.autoCompact: true    
       delta.autoOptimize.optimizeWrite: true  
       delta.enableChangeDataFeed: false
-    base_dbx_patterns:
-      customer_details_1:
+    base_dbx_patterns: # this is a database name
+      customer_details_1: # this is a table name and it's subsequent properties
         ids: id
         depends_on:
           - raw.raw_dbx_patterns.customers
         # delta table properties can be set at stage level or table level
         # table level properties will overwride stage level properties
         delta_properties:
             delta.enableChangeDataFeed: true
-      customer_details_2:
+      customer_details_2: # this is a table name and it's subsequent properties
         ids: id
         depends_on:
           - raw.raw_dbx_patterns.customers
 ```
 
 Define you load configuration:
 
 ```yaml
+version: 1.0.0
 tables: ./tables.yaml
 
-landing:
-  read:
+landing: # this is the landing stage in the deltalake house
+  read: # this is the type of spark asset that the pipeline needs to read from
     trigger: customerdetailscomplete-{{filename_date_format}}*.flg
     trigger_type: file
-    database: landing_dbx_patterns
-    table: "{{table}}"
     container: datalake
     root: "/mnt/{{container}}/data/landing/dbx_patterns/{{table}}/{{path_date_format}}"
     filename: "{{table}}-{{filename_date_format}}*.csv"
     filename_date_format: "%Y%m%d"
     path_date_format: "%Y%m%d"
     format: cloudFiles
-    spark_schema: ../Schema/{{table.lower()}}.yaml
+    spark_schema: ../schema/{{table.lower()}}.yaml
     options:
       # autoloader
       cloudFiles.format: csv
       cloudFiles.schemaLocation:  /mnt/{{container}}/checkpoint/{{checkpoint}}
       cloudFiles.useIncrementalListing: auto
       # schema
       inferSchema: false
@@ -105,57 +95,66 @@
       delimiter: ","
       escape: '"'
       nullValue: ""
       quote: '"'
       emptyValue: ""
     
 
-raw:
-  delta_lake:
+raw: # this is the bronze stage in the deltalake house
+  delta_lake: # this is the type of spark asset that the pipeline needs to read and write to
     # delta table properties can be set at stage level or table level
     delta_properties:
       delta.appendOnly: true
       delta.autoOptimize.autoCompact: true    
       delta.autoOptimize.optimizeWrite: true  
       delta.enableChangeDataFeed: false
-    database: raw_dbx_patterns
-    table: "{{table}}"
+    managed: false
+    create_table: true
     container: datalake
     root: /mnt/{{container}}/data/raw
     path: "{{database}}/{{table}}"
     options:
       checkpointLocation: /mnt/{{container}}/checkpoint/{{database}}_{{table}}
       mergeSchema: true
 ```
 
 Import the config objects into you pipeline:
 
 ```python
 from yetl import Config, Timeslice, StageType
 
-# build path to configuration file
-pattern = "auto_load_schema"
-config_path = f"../Config"
-
-# create a timeslice object for slice loading. Use * for all time (supports hrs, mins, seconds and sub-second).
+pipeline = "auto_load_schema"
+project = "test_project"
 timeslice = Timeslice(day="*", month="*", year="*")
-
-# parse and create a config objects
-config = Config(config_path=config_path, pattern=pattern)
-
-# get the configuration for a table mapping to load.
+config = Config(
+    project=project, pipeline=pipeline
+)
 table_mapping = config.get_table_mapping(
-    timeslice=timeslice, 
-    stage=StageType.raw, 
-    table="customers"
+    timeslice=timeslice, stage=StageType.raw, table="customers"
 )
 
 print(table_mapping)
 ```
 
+Use even less code and use the decorator pattern:
+
+```python
+@yetl_flow(
+        project="test_project", 
+        stage=StageType.raw
+)
+def auto_load_schema(table_mapping:TableMapping):
+
+    # << ADD YOUR PIPELINE LOGIC HERE - USING TABLE MAPPING CONFIG >>
+    return table_mapping # return whatever you want here.
+
+
+result = auto_load_schema(table="customers")
+```
+
 ## Development Setup
 
 ```
 pip install -r requirements.txt
 ```
 
 ## Unit Tests
@@ -163,14 +162,23 @@
 To run the unit tests with a coverage report.
 
 ```
 pip install -e .
 pytest test/unit --junitxml=junit/test-results.xml --cov=yetl --cov-report=xml --cov-report=html
 ```
 
+## Integration Tests
+
+To run the integration tests with a coverage report.
+
+```
+pip install -e .
+pytest test/integration --junitxml=junit/test-results.xml --cov=yetl --cov-report=xml --cov-report=html
+```
+
 ## Build
 
 ```
 python setup.py sdist bdist_wheel
 ```
 
 ## Publish
```

### Comparing `yetl-framework-1.0.0/setup.py` & `yetl-framework-1.0.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 # The text of the README file
 README = (HERE / "README.md").read_text()
 
 # This call to setup() does all the work
 setup(
     name="yetl-framework",
-    version="1.0.0",
+    version="1.0.1",
     description="yet (another spark) etl framework",
     long_description=README,
     long_description_content_type="text/markdown",
     url="https://www.yetl.io/",
     project_urls={
         "GitHub": "https://github.com/sibytes/yetl",
         "Documentation": "https://www.yetl.io/",
```

### Comparing `yetl-framework-1.0.0/yetl/_config.py` & `yetl-framework-1.0.1/yetl/_config.py`

 * *Files 2% similar despite different names*

```diff
@@ -8,14 +8,15 @@
 from ._logging_config import configure_logging
 from ._project import Project
 
 
 class Config:
     _TABLES = "tables"
     _CONFIG_PATH = "config_path"
+    _PROJECT = "project"
 
     def __init__(self, project: str, pipeline: str, config_path: str = None):
         self.config_path = get_config_path(project, config_path)
         configure_logging(project, self.config_path)
         self.project = self._load_project(project)
         self.pipeline = self._load_pipeline(pipeline)
         self.tables = self._load_tables()
@@ -34,14 +35,15 @@
         config_file_path = os.path.join(self.project.pipelines, pipeline_file)
         pipeline = load_yaml(config_file_path)
         check_version(pipeline)
 
         # add the configuration path into the confif dictionart
         # so that it gets passed to table config when created
         pipeline[self._CONFIG_PATH] = self.project.pipelines
+        pipeline[self._PROJECT] = self.project
         return pipeline
 
     def _load_tables(self):
         tables_path = self.pipeline[self._TABLES]
         tables_path = abs_config_path(
             self.project.pipelines, self.pipeline[self._TABLES]
         )
```

### Comparing `yetl-framework-1.0.0/yetl/_decorators.py` & `yetl-framework-1.0.1/yetl/_decorators.py`

 * *Files identical despite different names*

### Comparing `yetl-framework-1.0.0/yetl/_logging_config.py` & `yetl-framework-1.0.1/yetl/_logging_config.py`

 * *Files identical despite different names*

### Comparing `yetl-framework-1.0.0/yetl/_project.py` & `yetl-framework-1.0.1/yetl/_project.py`

 * *Files identical despite different names*

### Comparing `yetl-framework-1.0.0/yetl/_spark_context.py` & `yetl-framework-1.0.1/yetl/_spark_context.py`

 * *Files identical despite different names*

### Comparing `yetl-framework-1.0.0/yetl/_tables.py` & `yetl-framework-1.0.1/yetl/_tables.py`

 * *Files identical despite different names*

### Comparing `yetl-framework-1.0.0/yetl/_timeslice.py` & `yetl-framework-1.0.1/yetl/_timeslice.py`

 * *Files identical despite different names*

### Comparing `yetl-framework-1.0.0/yetl/_utils.py` & `yetl-framework-1.0.1/yetl/_utils.py`

 * *Files identical despite different names*

### Comparing `yetl-framework-1.0.0/yetl/datallake.py` & `yetl-framework-1.0.1/yetl/deltalake.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,228 +1,238 @@
 import json
 from pyspark.sql import DataFrame
 import logging
 from pyspark.sql.types import StructType, StructField
 import jinja2
 from typing import List
 from ._spark_context import get_spark_context
+from pydantic import BaseModel, Field
+from typing import Any
+from ._project import Project
+from pyspark.sql import SparkSession
 
-_logger = logging.getLogger(__name__)
-
-
-def get_partition_predicate(partition_values: dict):
-    predicates = []
-    for k, v in partition_values.items():
-        v = [str(val) for val in v]
-        p = f"`{k}` in ({','.join(v)})"
-        predicates.append(p)
-
-    predicate = " and ".join(predicates)
-
-    return predicate
-
-
-def table_exists(database: str, table: str):
-    spark = get_spark_context(project="test_project")
-    table_exists = (
-        spark.sql(f"SHOW TABLES in {database};")
-        .where(f"tableName='{table}' AND !isTemporary")
-        .count()
-        == 1
-    )
-    return table_exists
-
-
-def create_table(
-    database: str,
-    table: str,
-    path: str = None,
-    delta_properties: List[str] = None,
-    sql: str = None,
-):
-    _logger.debug(f"Creating table if not exists {database}.{table} at {path}")
-
-    if not sql:
-        sql = f"CREATE TABLE IF NOT EXISTS `{database}`.`{table}`"
-
-    # add in the delta properties if there are any
-    sql_properties = ""
-    if delta_properties:
-        sql_properties = [
-            f"{k.lower()} = {v.lower()}" for k, v in delta_properties.items()
-        ]
-        sql_properties = ", ".join(sql_properties)
-        sql_properties = f"TBLPROPERTIES({sql_properties})"
-
-    sql_path = ""
-    if path:
-        sql_path = f"USING DELTA LOCATION '{path}'"
-
-        sql = f"{sql}\n{sql_path}\n{sql_properties};"
-
-    spark = get_spark_context(project="test_project")
-    _logger.debug(f"{sql}")
-    spark.sql(sql)
-
-    return sql
-
-
-def create_database(database: str):
-    _logger.debug(f"Creating database if not exists `{database}`")
-    sql = f"CREATE DATABASE IF NOT EXISTS {database}"
-    spark = get_spark_context(project="test_project")
-    _logger.debug(sql)
-    spark.sql(sql)
-    return sql
-
-
-def alter_table_drop_constraint(database: str, table: str, name: str):
-    return f"ALTER TABLE `{database}`.`{table}` DROP CONSTRAINT {name};"
-
-
-def alter_table_add_constraint(database: str, table: str, name: str, constraint: str):
-    return f"ALTER TABLE `{database}`.`{table}` ADD CONSTRAINT {name} CHECK ({constraint});"
-
-
-def alter_table_set_tblproperties(database: str, table: str, properties: str):
-    return f"ALTER TABLE `{database}`.`{table}` SET TBLPROPERTIES ({properties});"
 
+_logger = logging.getLogger(__name__)
 
-def get_table_properties(database: str, table: str):
-    _logger.debug(f"getting existing table properties for table {database}.{table}")
-
-    spark = get_spark_context(project="test_project")
 
-    df: DataFrame = spark.sql(f"SHOW TBLPROPERTIES `{database}`.`{table}`").collect()
-    tbl_properties = {
-        c.asDict()["key"]: c.asDict()["value"]
-        for c in df
-        if not c["key"].startswith("delta.constraints")
-    }
-    tbl_constraints = {
-        c.asDict()["key"].split(".")[-1]: c.asDict()["value"]
-        for c in df
-        if c["key"].startswith("delta.constraints")
-    }
+class DeltaLakeFn(BaseModel):
+    def __init__(self, **data: Any) -> None:
+        super().__init__(**data)
+        self.spark = get_spark_context(self.project.name, self.project.spark.config)
+
+    project: Project = Field(...)
+    spark: SparkSession = Field(default=None)
+
+    def get_partition_predicate(self, partition_values: dict):
+        predicates = []
+        for k, v in partition_values.items():
+            v = [str(val) for val in v]
+            p = f"`{k}` in ({','.join(v)})"
+            predicates.append(p)
+
+        predicate = " and ".join(predicates)
+
+        return predicate
+
+    def table_exists(self, database: str, table: str):
+        table_exists = (
+            self.spark.sql(f"SHOW TABLES in {database};")
+            .where(f"tableName='{table}' AND !isTemporary")
+            .count()
+            == 1
+        )
+        return table_exists
 
-    properties = {
-        f"{database}.{table}": {
-            "constraints": tbl_constraints,
-            "properties": tbl_properties,
+    def create_table(
+        self,
+        database: str,
+        table: str,
+        path: str = None,
+        delta_properties: List[str] = None,
+        sql: str = None,
+    ):
+        _logger.debug(f"Creating table if not exists {database}.{table} at {path}")
+
+        if not sql:
+            sql = f"CREATE TABLE IF NOT EXISTS `{database}`.`{table}`"
+
+        # add in the delta properties if there are any
+        sql_properties = ""
+        if delta_properties:
+            sql_properties = [
+                f"{k.lower()} = {v.lower()}" for k, v in delta_properties.items()
+            ]
+            sql_properties = ", ".join(sql_properties)
+            sql_properties = f"TBLPROPERTIES({sql_properties})"
+
+        sql_path = ""
+        if path:
+            sql_path = f"USING DELTA LOCATION '{path}'"
+
+            sql = f"{sql}\n{sql_path}\n{sql_properties};"
+
+        _logger.debug(f"{sql}")
+        self.spark.sql(sql)
+
+        return sql
+
+    def create_database(self, database: str):
+        _logger.debug(f"Creating database if not exists `{database}`")
+        sql = f"CREATE DATABASE IF NOT EXISTS {database}"
+        _logger.debug(sql)
+        self.spark.sql(sql)
+        return sql
+
+    def alter_table_drop_constraint(self, database: str, table: str, name: str):
+        return f"ALTER TABLE `{database}`.`{table}` DROP CONSTRAINT {name};"
+
+    def alter_table_add_constraint(
+        self, database: str, table: str, name: str, constraint: str
+    ):
+        return f"ALTER TABLE `{database}`.`{table}` ADD CONSTRAINT {name} CHECK ({constraint});"
+
+    def alter_table_set_tblproperties(self, database: str, table: str, properties: str):
+        return f"ALTER TABLE `{database}`.`{table}` SET TBLPROPERTIES ({properties});"
+
+    def get_table_properties(self, database: str, table: str):
+        _logger.debug(f"getting existing table properties for table {database}.{table}")
+
+        df: DataFrame = self.spark.sql(
+            f"SHOW TBLPROPERTIES `{database}`.`{table}`"
+        ).collect()
+        tbl_properties = {
+            c.asDict()["key"]: c.asDict()["value"]
+            for c in df
+            if not c["key"].startswith("delta.constraints")
+        }
+        tbl_constraints = {
+            c.asDict()["key"].split(".")[-1]: c.asDict()["value"]
+            for c in df
+            if c["key"].startswith("delta.constraints")
         }
-    }
-    msg = json.dumps(properties, indent=4, default=str)
-    _logger.debug(msg)
-    return properties
-
-
-def optimize(database: str, table: str, partition_values: dict, zorder_by: list = []):
-    sql = f"OPTIMIZE `{database}`.`{table}`"
-
-    if partition_values:
-        predicate = get_partition_predicate(partition_values)
-        predicate = f" WHERE {predicate}"
-        sql = f"{sql}{predicate}"
-
-    if zorder_by:
-        sql_zorderby = ",".join([f"`{z}`" for z in zorder_by])
-        sql = f"{sql} ZORDER BY ({sql_zorderby})"
 
-    spark = get_spark_context(project="test_project")
-    _logger.debug(f"optimizing table {database}.{table}\n{sql}")
-    spark.sql(sql)
+        properties = {
+            f"{database}.{table}": {
+                "constraints": tbl_constraints,
+                "properties": tbl_properties,
+            }
+        }
+        msg = json.dumps(properties, indent=4, default=str)
+        _logger.debug(msg)
+        return properties
+
+    def optimize(
+        self, database: str, table: str, partition_values: dict, zorder_by: list = []
+    ):
+        sql = f"OPTIMIZE `{database}`.`{table}`"
+
+        if partition_values:
+            predicate = self.get_partition_predicate(partition_values)
+            predicate = f" WHERE {predicate}"
+            sql = f"{sql}{predicate}"
+
+        if zorder_by:
+            sql_zorderby = ",".join([f"`{z}`" for z in zorder_by])
+            sql = f"{sql} ZORDER BY ({sql_zorderby})"
+
+        _logger.debug(f"optimizing table {database}.{table}\n{sql}")
+        self.spark.sql(sql)
+
+    def get_table_details(self, database: str, table: str):
+        _logger.debug(
+            f"getting existing table details and partitions for table {database}.{table}"
+        )
 
+        df: DataFrame = self.spark.sql(
+            f"DESCRIBE TABLE EXTENDED `{database}`.`{table}`"
+        ).collect()
+
+        # get the details into a dictionary
+        details = {c.asDict()["col_name"]: c.asDict()["data_type"] for c in df}
+
+        # pull out the columns
+        columns = {}
+        ordinal = 0
+        for k, v in details.items():
+            if k and v:
+                columns[k] = {}
+                columns[k]["ordinal"] = ordinal
+                columns[k]["type"] = v
+                ordinal = +1
+            else:
+                break
+
+        # pull out the columns
+        partitions = [v for k, v in details.items() if k.startswith("Part ")]
+
+        details = {
+            f"{database}.{table}": {
+                "columns": columns,
+                "partitions": partitions,
+                "name": details.get("Name"),
+                "location": details.get("Location"),
+                "provider": details.get("Provider"),
+                "owner": details.get("Owner"),
+            }
+        }
 
-def get_table_details(database: str, table: str):
-    _logger.debug(
-        f"getting existing table details and partitions for table {database}.{table}"
+        msg = json.dumps(details, indent=4, default=str)
+        _logger.debug(msg)
+        return details
+
+    def create_column_ddl(self, field: StructField):
+        nullable = "" if field.nullable else "NOT NULL"
+        comment = f"COMMENT {field.metadata}" if field.metadata else ""
+        field_type = field.dataType.typeName()
+        field_name = f"`{field.name}`"
+
+        return f"\t{field_name} {field_type} {nullable} {comment}"
+
+    def create_table_dll(
+        self,
+        schema: StructType,
+        partition_fields: list = [],
+        format: str = "DELTA",
+        always_identity_column: str = None,
+    ):
+        field_ddl = [self.create_column_ddl(f) for f in schema.fields]
+        if always_identity_column:
+            always_identity_column = (
+                f"\t`{always_identity_column}` GENERATED ALWAYS AS IDENTITY"
+            )
+            field_ddl = [always_identity_column] + field_ddl
+
+        field_ddl = ",\n".join(field_ddl)
+
+        template_partition = jinja2.Template("PARTITIONED BY ({{partition_fields}})")
+        template_ddl = jinja2.Template(
+            """CREATE TABLE {{database_name}}.{{table_name}}
+    (
+    {{field_ddl}}
     )
-    spark = get_spark_context(project="test_project")
+    USING {{format}} LOCATION '{{path}}'
+    {{partition_ddl}}""",
+            undefined=jinja2.DebugUndefined,
+        )
 
-    df: DataFrame = spark.sql(
-        f"DESCRIBE TABLE EXTENDED `{database}`.`{table}`"
-    ).collect()
-
-    # get the details into a dictionary
-    details = {c.asDict()["col_name"]: c.asDict()["data_type"] for c in df}
-
-    # pull out the columns
-    columns = {}
-    ordinal = 0
-    for k, v in details.items():
-        if k and v:
-            columns[k] = {}
-            columns[k]["ordinal"] = ordinal
-            columns[k]["type"] = v
-            ordinal = +1
+        if partition_fields:
+            partition_fields = [f"`{p}`" for p in partition_fields]
+            partition_fields = ",".join(partition_fields)
+            partition_ddl: str = template_partition.render(
+                partition_fields=partition_fields
+            )
         else:
-            break
-
-    # pull out the columns
-    partitions = [v for k, v in details.items() if k.startswith("Part ")]
+            partition_ddl = ""
 
-    details = {
-        f"{database}.{table}": {
-            "columns": columns,
-            "partitions": partitions,
-            "name": details.get("Name"),
-            "location": details.get("Location"),
-            "provider": details.get("Provider"),
-            "owner": details.get("Owner"),
+        replace = {
+            "field_ddl": field_ddl,
+            "partition_ddl": partition_ddl,
+            "format": format,
         }
-    }
-
-    msg = json.dumps(details, indent=4, default=str)
-    _logger.debug(msg)
-    return details
-
-
-def create_column_ddl(field: StructField):
-    nullable = "" if field.nullable else "NOT NULL"
-    comment = f"COMMENT {field.metadata}" if field.metadata else ""
-    field_type = field.dataType.typeName()
-    field_name = f"`{field.name}`"
-
-    return f"\t{field_name} {field_type} {nullable} {comment}"
-
-
-def create_table_dll(
-    schema: StructType,
-    partition_fields: list = [],
-    format: str = "DELTA",
-    always_identity_column: str = None,
-):
-    field_ddl = [create_column_ddl(f) for f in schema.fields]
-    if always_identity_column:
-        always_identity_column = (
-            f"\t`{always_identity_column}` GENERATED ALWAYS AS IDENTITY"
-        )
-        field_ddl = [always_identity_column] + field_ddl
-
-    field_ddl = ",\n".join(field_ddl)
-
-    template_partition = jinja2.Template("PARTITIONED BY ({{partition_fields}})")
-    template_ddl = jinja2.Template(
-        """CREATE TABLE {{database_name}}.{{table_name}}
-(
-{{field_ddl}}
-)
-USING {{format}} LOCATION '{{path}}'
-{{partition_ddl}}""",
-        undefined=jinja2.DebugUndefined,
-    )
-
-    if partition_fields:
-        partition_fields = [f"`{p}`" for p in partition_fields]
-        partition_fields = ",".join(partition_fields)
-        partition_ddl: str = template_partition.render(
-            partition_fields=partition_fields
-        )
-    else:
-        partition_ddl = ""
 
-    replace = {"field_ddl": field_ddl, "partition_ddl": partition_ddl, "format": format}
+        table_ddl = template_ddl.render(replace)
+        table_ddl = f"{table_ddl};"
 
-    table_ddl = template_ddl.render(replace)
-    table_ddl = f"{table_ddl};"
+        return table_ddl
 
-    return table_ddl
+    class Config:
+        arbitrary_types_allowed = True
```

### Comparing `yetl-framework-1.0.0/yetl/dataset/_dataset.py` & `yetl-framework-1.0.1/yetl/dataset/_dataset.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import logging
 from pydantic import BaseModel, Field, PrivateAttr
 from .._utils import JinjaVariables
 from typing import Any, Dict, Union, List
 from .._timeslice import Timeslice
 from .._stage_type import StageType
 from .dataset_type import TableType
+from .._project import Project
 
 
 class Table(BaseModel):
     def __init__(self, **data: Any) -> None:
         super().__init__(**data)
 
     stage: StageType = Field(...)
@@ -25,14 +26,15 @@
 class DataSet(BaseModel):
     def __init__(self, **data: Any) -> None:
         super().__init__(**data)
         self._logger = logging.getLogger(self.__class__.__name__)
 
     _logger: Any = PrivateAttr(default=None)
     _replacements: Dict[JinjaVariables, str] = PrivateAttr(default=None)
+    project: Project = Field(...)
     container: str = Field(...)
     root: str = Field(...)
     path: str = Field(default=None)
     options: dict = Field(...)
     timeslice: Timeslice = Field(...)
     checkpoint: str = Field(default=None)
     config_path: str = Field(...)
```

### Comparing `yetl-framework-1.0.0/yetl/dataset/_deltalake.py` & `yetl-framework-1.0.1/yetl/dataset/_deltalake.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,15 +2,17 @@
 from pydantic import Field, PrivateAttr
 from .._utils import JinjaVariables, render_jinja, is_databricks
 from typing import Any, Dict, Union, List
 from .._timeslice import Timeslice
 import os
 from .._stage_type import StageType
 from ._dataset import DataSet, Table
-from ..datallake import create_database, create_table
+from ..deltalake import DeltaLakeFn
+
+# from ..datallake import create_database, create_table
 
 # try:
 #     from databricks.sdk.runtime import *  # noqa F403
 # except ModuleNotFoundError:
 #     pass
 
 
@@ -28,22 +30,24 @@
 
 
 class DeltaLake(DataSet, DeltaLakeTable):
     def __init__(self, **data: Any) -> None:
         super().__init__(**data)
         self._logger = logging.getLogger(self.__class__.__name__)
         self._render()
+        self._spark = DeltaLakeFn(project=self.project)
         self.create_delta_table()
 
     @classmethod
     def in_allowed_stages(cls, stage: StageType):
         return stage in (stage.raw, stage.base, stage.curated)
 
     _logger: Any = PrivateAttr(default=None)
     _replacements: Dict[JinjaVariables, str] = PrivateAttr(default=None)
+    _spark: DeltaLakeFn = PrivateAttr(default=None)
     options: Union[dict, None] = Field(default=None)
     timeslice: Timeslice = Field(...)
     location: str = Field(default=None)
     checkpoint_location: str = Field(default=None)
     stage: StageType = Field(...)
     managed: bool = Field(default=False)
     create_table: bool = Field(default=True)
@@ -68,22 +72,22 @@
         if not is_databricks():
             self.location = f"{self.config_path}/../data{self.location}"
             self.location = os.path.abspath(self.location)
 
     def create_delta_table(self):
         database_table = f"`{self.database}`.`{self.table}`"
         self._logger.info(f"Creating delta lake table {database_table}")
-        create_database(self.database)
+        self._spark.create_database(self.database)
 
         if self.managed:
-            create_table(
+            self._spark.create_table(
                 database=self.database,
                 table=self.table,
                 delta_properties=self.delta_properties,
             )
         else:
-            create_table(
+            self._spark.create_table(
                 database=self.database,
                 table=self.table,
                 delta_properties=self.delta_properties,
                 path=self.location,
             )
```

### Comparing `yetl-framework-1.0.0/yetl/dataset/_factory.py` & `yetl-framework-1.0.1/yetl/dataset/_factory.py`

 * *Files 2% similar despite different names*

```diff
@@ -9,14 +9,15 @@
 from .._timeslice import Timeslice
 from typing import Union
 
 
 class _DatasetFactory:
     _TIMESLICE = "timeslice"
     _CONFIG_PATH = "config_path"
+    _PROJECT = "project"
 
     def __init__(self) -> None:
         self._logger = logging.getLogger(self.__class__.__name__)
         self._dataset = {}
         self._table = {}
 
     def register_dataset_type(self, io_type: DataSetType, dataset_type: type):
@@ -92,14 +93,15 @@
                 f"""Table stage and type not found in configuration.
                 Table: {table.stage.name}.{table.table_type.value}
                 not int config:
                 {config}."""
             )
         stage_config[self._TIMESLICE] = timeslice
         stage_config[self._CONFIG_PATH] = config[self._CONFIG_PATH]
+        stage_config[self._PROJECT] = config[self._PROJECT]
         table_config = table.dict()
         stage_config = {**stage_config, **table_config}
 
         return stage_config
 
 
 factory = _DatasetFactory()
```

### Comparing `yetl-framework-1.0.0/yetl/dataset/_read.py` & `yetl-framework-1.0.1/yetl/dataset/_read.py`

 * *Files identical despite different names*

### Comparing `yetl-framework-1.0.0/yetl/workflow/_multi_threaded.py` & `yetl-framework-1.0.1/yetl/workflow/_multi_threaded.py`

 * *Files identical despite different names*

### Comparing `yetl-framework-1.0.0/yetl_framework.egg-info/SOURCES.txt` & `yetl-framework-1.0.1/yetl_framework.egg-info/SOURCES.txt`

 * *Files 15% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 yetl/_project.py
 yetl/_spark_context.py
 yetl/_stage_type.py
 yetl/_table_mapping.py
 yetl/_tables.py
 yetl/_timeslice.py
 yetl/_utils.py
-yetl/datallake.py
+yetl/deltalake.py
 yetl/dataset/__init__.py
 yetl/dataset/_dataset.py
 yetl/dataset/_deltalake.py
 yetl/dataset/_factory.py
 yetl/dataset/_read.py
 yetl/dataset/_write.py
 yetl/dataset/dataset_type.py
```

