# Comparing `tmp/flytekitplugins-polars-1.6.0b1.tar.gz` & `tmp/flytekitplugins-polars-1.6.0b2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flytekitplugins-polars-1.6.0b1.tar", last modified: Wed May  3 04:48:11 2023, max compression
+gzip compressed data, was "flytekitplugins-polars-1.6.0b2.tar", last modified: Fri May  5 17:49:49 2023, max compression
```

## Comparing `flytekitplugins-polars-1.6.0b1.tar` & `flytekitplugins-polars-1.6.0b2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 04:48:11.916320 flytekitplugins-polars-1.6.0b1/
--rw-r--r--   0 runner    (1001) docker     (123)      758 2023-05-03 04:48:11.916320 flytekitplugins-polars-1.6.0b1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      469 2023-05-03 04:47:44.000000 flytekitplugins-polars-1.6.0b1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 04:48:11.916320 flytekitplugins-polars-1.6.0b1/flytekitplugins/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 04:48:11.916320 flytekitplugins-polars-1.6.0b1/flytekitplugins/polars/
--rw-r--r--   0 runner    (1001) docker     (123)      400 2023-05-03 04:47:44.000000 flytekitplugins-polars-1.6.0b1/flytekitplugins/polars/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2936 2023-05-03 04:47:44.000000 flytekitplugins-polars-1.6.0b1/flytekitplugins/polars/sd_transformers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 04:48:11.916320 flytekitplugins-polars-1.6.0b1/flytekitplugins_polars.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      758 2023-05-03 04:48:11.000000 flytekitplugins-polars-1.6.0b1/flytekitplugins_polars.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      428 2023-05-03 04:48:11.000000 flytekitplugins-polars-1.6.0b1/flytekitplugins_polars.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-03 04:48:11.000000 flytekitplugins-polars-1.6.0b1/flytekitplugins_polars.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-05-03 04:48:11.000000 flytekitplugins-polars-1.6.0b1/flytekitplugins_polars.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-03 04:48:11.000000 flytekitplugins-polars-1.6.0b1/flytekitplugins_polars.egg-info/namespace_packages.txt
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-05-03 04:48:11.000000 flytekitplugins-polars-1.6.0b1/flytekitplugins_polars.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-03 04:48:11.000000 flytekitplugins-polars-1.6.0b1/flytekitplugins_polars.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-03 04:48:11.916320 flytekitplugins-polars-1.6.0b1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1254 2023-05-03 04:48:03.000000 flytekitplugins-polars-1.6.0b1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 17:49:49.086203 flytekitplugins-polars-1.6.0b2/
+-rw-r--r--   0 runner    (1001) docker     (123)      758 2023-05-05 17:49:49.086203 flytekitplugins-polars-1.6.0b2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      469 2023-05-05 17:49:25.000000 flytekitplugins-polars-1.6.0b2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 17:49:49.086203 flytekitplugins-polars-1.6.0b2/flytekitplugins/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 17:49:49.086203 flytekitplugins-polars-1.6.0b2/flytekitplugins/polars/
+-rw-r--r--   0 runner    (1001) docker     (123)      400 2023-05-05 17:49:25.000000 flytekitplugins-polars-1.6.0b2/flytekitplugins/polars/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2996 2023-05-05 17:49:25.000000 flytekitplugins-polars-1.6.0b2/flytekitplugins/polars/sd_transformers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 17:49:49.086203 flytekitplugins-polars-1.6.0b2/flytekitplugins_polars.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      758 2023-05-05 17:49:49.000000 flytekitplugins-polars-1.6.0b2/flytekitplugins_polars.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      428 2023-05-05 17:49:49.000000 flytekitplugins-polars-1.6.0b2/flytekitplugins_polars.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 17:49:49.000000 flytekitplugins-polars-1.6.0b2/flytekitplugins_polars.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-05-05 17:49:49.000000 flytekitplugins-polars-1.6.0b2/flytekitplugins_polars.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-05 17:49:49.000000 flytekitplugins-polars-1.6.0b2/flytekitplugins_polars.egg-info/namespace_packages.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-05-05 17:49:49.000000 flytekitplugins-polars-1.6.0b2/flytekitplugins_polars.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-05 17:49:49.000000 flytekitplugins-polars-1.6.0b2/flytekitplugins_polars.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-05 17:49:49.086203 flytekitplugins-polars-1.6.0b2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1254 2023-05-05 17:49:40.000000 flytekitplugins-polars-1.6.0b2/setup.py
```

### Comparing `flytekitplugins-polars-1.6.0b1/PKG-INFO` & `flytekitplugins-polars-1.6.0b2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flytekitplugins-polars
-Version: 1.6.0b1
+Version: 1.6.0b2
 Summary: Polars plugin for flytekit
 Author: Robin Kahlow
 License: apache2
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `flytekitplugins-polars-1.6.0b1/flytekitplugins/polars/sd_transformers.py` & `flytekitplugins-polars-1.6.0b2/flytekitplugins/polars/sd_transformers.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 import pandas as pd
 import polars as pl
 
 from flytekit import FlyteContext
 from flytekit.models import literals
 from flytekit.models.literals import StructuredDatasetMetadata
 from flytekit.models.types import StructuredDatasetType
+from flytekit.types.structured.basic_dfs import get_storage_options
 from flytekit.types.structured.structured_dataset import (
     PARQUET,
     StructuredDataset,
     StructuredDatasetDecoder,
     StructuredDatasetEncoder,
     StructuredDatasetTransformerEngine,
 )
@@ -58,18 +59,18 @@
 
     def decode(
         self,
         ctx: FlyteContext,
         flyte_value: literals.StructuredDataset,
         current_task_metadata: StructuredDatasetMetadata,
     ) -> pl.DataFrame:
-        local_dir = ctx.file_access.get_random_local_directory()
-        ctx.file_access.get_data(flyte_value.uri, local_dir, is_multipart=True)
+        uri = flyte_value.uri
+        kwargs = get_storage_options(ctx.file_access.data_config, uri)
         if current_task_metadata.structured_dataset_type and current_task_metadata.structured_dataset_type.columns:
             columns = [c.name for c in current_task_metadata.structured_dataset_type.columns]
-            return pl.read_parquet(local_dir, columns=columns, use_pyarrow=True)
-        return pl.read_parquet(local_dir, use_pyarrow=True)
+            return pl.read_parquet(uri, columns=columns, use_pyarrow=True, storage_options=kwargs)
+        return pl.read_parquet(uri, use_pyarrow=True, storage_options=kwargs)
 
 
 StructuredDatasetTransformerEngine.register(PolarsDataFrameToParquetEncodingHandler())
 StructuredDatasetTransformerEngine.register(ParquetToPolarsDataFrameDecodingHandler())
 StructuredDatasetTransformerEngine.register_renderer(pl.DataFrame, PolarsDataFrameRenderer())
```

### Comparing `flytekitplugins-polars-1.6.0b1/flytekitplugins_polars.egg-info/PKG-INFO` & `flytekitplugins-polars-1.6.0b2/flytekitplugins_polars.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flytekitplugins-polars
-Version: 1.6.0b1
+Version: 1.6.0b2
 Summary: Polars plugin for flytekit
 Author: Robin Kahlow
 License: apache2
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `flytekitplugins-polars-1.6.0b1/setup.py` & `flytekitplugins-polars-1.6.0b2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 microlib_name = f"flytekitplugins-{PLUGIN_NAME}"
 
 plugin_requires = [
     "flytekit>=1.3.0b2,<2.0.0",
     "polars>=0.8.27",
 ]
 
-__version__ = "1.6.0b1"
+__version__ = "1.6.0b2"
 
 setup(
     name=microlib_name,
     version=__version__,
     author="Robin Kahlow",
     description="Polars plugin for flytekit",
     namespace_packages=["flytekitplugins"],
```

