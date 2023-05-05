# Comparing `tmp/adfpy-0.1.0.tar.gz` & `tmp/adfpy-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "adfpy-0.1.0.tar", max compression
+gzip compressed data, was "adfpy-0.2.0.tar", max compression
```

## Comparing `adfpy-0.1.0.tar` & `adfpy-0.2.0.tar`

### file list

```diff
@@ -1,13 +1,12 @@
--rw-r--r--   0        0        0     1440 2022-07-25 11:03:03.472075 adfpy-0.1.0/README.md
--rw-r--r--   0        0        0        0 2022-07-25 11:03:03.472075 adfpy-0.1.0/adfpy/__init__.py
--rw-r--r--   0        0        0        0 2022-07-25 11:03:03.472075 adfpy-0.1.0/adfpy/activities/__init__.py
--rw-r--r--   0        0        0     3683 2022-07-25 11:03:03.472075 adfpy-0.1.0/adfpy/activities/control.py
--rw-r--r--   0        0        0     4802 2022-07-25 11:03:03.472075 adfpy-0.1.0/adfpy/activities/execution.py
--rw-r--r--   0        0        0     1858 2022-07-25 11:03:03.472075 adfpy-0.1.0/adfpy/activity.py
--rw-r--r--   0        0        0     7839 2022-07-25 11:03:03.472075 adfpy-0.1.0/adfpy/deploy.py
--rw-r--r--   0        0        0      263 2022-07-25 11:03:03.472075 adfpy-0.1.0/adfpy/error.py
--rw-r--r--   0        0        0     1505 2022-07-25 11:03:03.472075 adfpy-0.1.0/adfpy/pipeline.py
--rw-r--r--   0        0        0    16067 2022-07-25 11:03:03.472075 adfpy-0.1.0/adfpy/trigger.py
--rw-r--r--   0        0        0      819 2022-07-25 11:03:38.923772 adfpy-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     2359 2022-07-25 11:03:39.443758 adfpy-0.1.0/setup.py
--rw-r--r--   0        0        0     2246 2022-07-25 11:03:39.444120 adfpy-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1501 2023-05-05 14:05:39.919797 adfpy-0.2.0/README.md
+-rw-r--r--   0        0        0        0 2023-05-05 14:05:39.919797 adfpy-0.2.0/adfpy/__init__.py
+-rw-r--r--   0        0        0        0 2023-05-05 14:05:39.919797 adfpy-0.2.0/adfpy/activities/__init__.py
+-rw-r--r--   0        0        0     3683 2023-05-05 14:05:39.919797 adfpy-0.2.0/adfpy/activities/control.py
+-rw-r--r--   0        0        0     4802 2023-05-05 14:05:39.919797 adfpy-0.2.0/adfpy/activities/execution.py
+-rw-r--r--   0        0        0     1858 2023-05-05 14:05:39.919797 adfpy-0.2.0/adfpy/activity.py
+-rw-r--r--   0        0        0     9695 2023-05-05 14:05:39.919797 adfpy-0.2.0/adfpy/deploy.py
+-rw-r--r--   0        0        0      263 2023-05-05 14:05:39.919797 adfpy-0.2.0/adfpy/error.py
+-rw-r--r--   0        0        0     1505 2023-05-05 14:05:39.919797 adfpy-0.2.0/adfpy/pipeline.py
+-rw-r--r--   0        0        0    16067 2023-05-05 14:05:39.919797 adfpy-0.2.0/adfpy/trigger.py
+-rw-r--r--   0        0        0      827 2023-05-05 14:06:03.599726 adfpy-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0     2358 1970-01-01 00:00:00.000000 adfpy-0.2.0/PKG-INFO
```

### Comparing `adfpy-0.1.0/README.md` & `adfpy-0.2.0/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -8,22 +8,22 @@
 ```
 
 ## Usage
 Generally, using adfPy has 2 main components:
 1. Write your pipeline.
 2. Deploy your pipeline.
 
-adfPy has an opinionated syntax, which is heavily influenced by Airflow. For documentation on what the syntax looks like, please read the docs [here]().
+adfPy has an opinionated syntax, which is heavily influenced by Airflow. For documentation on what the syntax looks like, please read the docs [here](https://danielvdende.github.io/adfpy/).
 Some examples are provided in the examples directory of this repository.
 
 
 Once you've written your pipelines, it's time to deploy them! For this, you can use adfPy's deployment script:
 ```shell
 pip install adfpy
-adfpy-deploy
+adfpy-deploy --path <your_path_here>
 ```
 Note:
 - This script will ensure all pipelines in the provided path are present in your target ADF.
 - This script will also **remove** any ADF pipelines that are **not** in your path, but are in ADF.
 
 ## Still to come
 adfPy is still in development. As such, some ADF components are not yet supported:
```

### Comparing `adfpy-0.1.0/adfpy/activities/control.py` & `adfpy-0.2.0/adfpy/activities/control.py`

 * *Files identical despite different names*

### Comparing `adfpy-0.1.0/adfpy/activities/execution.py` & `adfpy-0.2.0/adfpy/activities/execution.py`

 * *Files identical despite different names*

### Comparing `adfpy-0.1.0/adfpy/activity.py` & `adfpy-0.2.0/adfpy/activity.py`

 * *Files identical despite different names*

### Comparing `adfpy-0.1.0/adfpy/deploy.py` & `adfpy-0.2.0/adfpy/deploy.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,22 +1,34 @@
 import importlib.util
+import logging
 import os
+import sys
 
 import click
 
 from dataclasses import dataclass
 from pathlib import Path
 from typing import Set, List
 
 from azure.identity import ClientSecretCredential
 from azure.mgmt.datafactory import DataFactoryManagementClient  # type: ignore
 
 from adfpy.error import PipelineModuleParseException
 from adfpy.pipeline import AdfPipeline
 
+stdout_handler = logging.StreamHandler(stream=sys.stdout)
+handlers = [stdout_handler]
+logging.basicConfig(
+    format='[%(asctime)s] {%(filename)s:%(lineno)d} %(levelname)s - %(message)s',
+    handlers=handlers
+)
+
+logger = logging.getLogger("adfPy")
+logger.setLevel(os.getenv("LOG_LEVEL", logging.INFO))
+
 
 @dataclass
 class ConfiguredDataFactory:
     resource_group: str
     name: str
     client: DataFactoryManagementClient
 
@@ -92,69 +104,80 @@
             load_pipelines_from_path(el, pipelines)
         else:
             pipelines = pipelines.union(load_pipelines_from_file(el))
     return pipelines
 
 
 def create_or_update_pipeline(adf: ConfiguredDataFactory,
-                              pipeline: AdfPipeline):
+                              pipeline: AdfPipeline,
+                              dry_run: bool = False):
     """Create or update a pipeline in Azure Data Factory based on the provided pipeline definition
 
     This function will also ensure that any pipelines that the provided pipeline depends on are created first. To
     achieve this, it makes use of the `processed_pipelines_names` global variable. After creating/updating a pipeline,
     this function will ensure that pipeline is added to this global, so it will not be created/updated again.
 
     Args:
         adf: ConfiguredDataFactory object
         pipeline: AdfPipeline object based on provided configuration
+        dry_run: boolean indicating whether the actions are to be executed as a dry-run. Defaults to False.
     """
     for required_pipeline in pipeline.depends_on_pipelines:
         # We only process a required pipeline if it hasn't been processed before
         if required_pipeline.name not in processed_pipelines_names:
-            create_or_update_pipeline(adf, required_pipeline)
-    print(f"Creating/updating {pipeline.name}")
-    adf.client.pipelines.create_or_update(adf.resource_group, adf.name, pipeline.name, pipeline.to_adf())
+            create_or_update_pipeline(adf, required_pipeline, dry_run)
+    logger.info(f"Creating/updating pipeline {pipeline.name}")
+    if not dry_run:
+        adf.client.pipelines.create_or_update(adf.resource_group, adf.name, pipeline.name, pipeline.to_adf())
     if pipeline.schedule:
-        adf.client.triggers.create_or_update(adf.resource_group,
-                                             adf.name,
-                                             pipeline.schedule.name,
-                                             pipeline.schedule.to_adf())
+        logger.info(f"Creating/updating trigger for {pipeline.name}")
+        if not dry_run:
+            adf.client.triggers.create_or_update(adf.resource_group,
+                                                 adf.name,
+                                                 pipeline.schedule.name,
+                                                 pipeline.schedule.to_adf())
     processed_pipelines_names.append(pipeline.name)
 
 
 def ensure_all_pipelines_up_to_date(pipelines: Set[AdfPipeline],
-                                    adf: ConfiguredDataFactory):
+                                    adf: ConfiguredDataFactory,
+                                    dry_run: bool = False):
     """Create or update pipelines in ADF based on a provided set of pipelines.
 
     This function checks with the global `processed_pipelines_names` variable to avoid duplicate processing.
     There is no functional requirement for this (i.e. it would be ok to process the same pipeline multiple times), but
     it's not very nice.
 
     Args:
         pipelines: Set of AdfPipeline objects retrieved from the local path
         adf: ConfiguredDataFactory object
+        dry_run: boolean indicating whether the actions are to be executed as a dry-run. Defaults to False.
     """
     for p in pipelines:
         if p.name not in processed_pipelines_names:
-            create_or_update_pipeline(adf, p)
+            create_or_update_pipeline(adf, p, dry_run)
 
 
-def remove_stale_pipelines(adf: ConfiguredDataFactory):
+def remove_stale_pipelines(adf: ConfiguredDataFactory, dry_run: bool = False):
     """Removes any pipelines that are (no longer) available in the configured (local) pipeline path
 
     This function is destructive, as any pipeline not managed by adfPy will be removed.
 
     Args:
         adf: ConfiguredDataFactory object
+        dry_run: boolean indicating whether the actions are to be executed as a dry-run. Defaults to False.
     """
     existing_pipelines = fetch_existing_pipelines(adf)
     for p in existing_pipelines:
         if p not in processed_pipelines_names:
-            print(f"Pipeline {p} no longer exists. Deleting from ADF")
-            adf.client.pipelines.delete(resource_group_name=adf.resource_group, factory_name=adf.name, pipeline_name=p)
+            logger.info(f"Deleting pipeline {p} from ADF. Pipeline {p} no longer exists in path")
+            if not dry_run:
+                adf.client.pipelines.delete(resource_group_name=adf.resource_group,
+                                            factory_name=adf.name,
+                                            pipeline_name=p)
 
 
 def configure_data_factory() -> ConfiguredDataFactory:
     """Configure your data factory, based mostly on environment variables
 
     Returns:
         A ConfiguredDataFactory object, with all required fields for interacting with ADF
@@ -173,33 +196,42 @@
 
 
 @click.command()
 @click.option('--path', required=True, type=Path, help='Path containing adfPy resources')
 @click.option('--delete-stale-resources/--no-delete-stale-resources', type=bool, default=True,
               help="Flag indicating whether or not to remove resources from ADF that are not available in the "
                    "configured path. Defaults to False")
-def run_deployment(path, delete_stale_resources):
+@click.option("--dry-run", type=bool, is_flag=True, default=False, help="Execute the deployment as a dry-run or not. If"
+                                                                        "enabled, the deploy script will only output "
+                                                                        "what will be changed rather than actually "
+                                                                        "executing the required action")
+def run_deployment(path, delete_stale_resources, dry_run):
     """Deploy your adfPy resources to ADF
 
     This tool deploys your adfPy resources. For authentication, you should set a number of
     environment variables:
 
     \b
     AZURE_SUBSCRIPTION_ID
     AZURE_RESOURCE_GROUP_NAME
     AZURE_DATA_FACTORY_NAME
     AZURE_SERVICE_PRINCIPAL_CLIENT_ID
     AZURE_SERVICE_PRINCIPAL_SECRET
     AZURE_TENANT_ID
     """
     configured_adf = configure_data_factory()
+    logger.info("Welcome to adfPy!")
+    logger.info(f"Starting up deployment to factory: {configured_adf.name}")
+    if dry_run:
+        logger.info("Dry run enabled. All changes below will not be executed")
 
     pipelines = load_pipelines_from_path(path)
+    logger.info(f"Loaded {len(pipelines)} pipelines")
 
-    ensure_all_pipelines_up_to_date(pipelines, configured_adf)
+    ensure_all_pipelines_up_to_date(pipelines, configured_adf, dry_run)
 
     if delete_stale_resources:
-        remove_stale_pipelines(configured_adf)
+        remove_stale_pipelines(configured_adf, dry_run)
 
 
 if __name__ == "__main__":
     run_deployment()
```

### Comparing `adfpy-0.1.0/adfpy/pipeline.py` & `adfpy-0.2.0/adfpy/pipeline.py`

 * *Files identical despite different names*

### Comparing `adfpy-0.1.0/adfpy/trigger.py` & `adfpy-0.2.0/adfpy/trigger.py`

 * *Files identical despite different names*

### Comparing `adfpy-0.1.0/pyproject.toml` & `adfpy-0.2.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 [tool.poetry]
 name = "adfpy"
-version = "0.1.0"
+version = "0.2.0"
 description = "A Pythonic wrapper for Azure Data Factory"
 authors = ["Daniel van der Ende <daniel.vanderende@gmail.com>"]
 license = "Apache"
 readme = "README.md"
 homepage = "https://github.com/danielvdende/adfpy"
 repository = "https://github.com/danielvdende/adfpy"
 keywords = ["azure", "data", "factory"]
 
 [tool.poetry.dependencies]
 python = "^3.8"
-azure-mgmt-datafactory = "^2.2.1"
+azure-mgmt-datafactory = "^2.2.1, <2.7.0"
 azure-identity = "^1.7.1"
 click = "^8.1.3"
 
 [tool.poetry.dev-dependencies]
-pytest = "^7.0.1"
+pytest = "^7.2.0"
 flake8 = "^4.0.1"
 coverage = "^6.3.2"
 pytest-cov = "^3.0.0"
 mypy = "^0.961"
 
 [tool.poetry.scripts]
 adfpy-deploy = "adfpy.deploy:run_deployment"
```

### Comparing `adfpy-0.1.0/PKG-INFO` & `adfpy-0.2.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 Metadata-Version: 2.1
 Name: adfpy
-Version: 0.1.0
+Version: 0.2.0
 Summary: A Pythonic wrapper for Azure Data Factory
 Home-page: https://github.com/danielvdende/adfpy
 License: Apache
 Keywords: azure,data,factory
 Author: Daniel van der Ende
 Author-email: daniel.vanderende@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Provides-Extra: docs
 Requires-Dist: azure-identity (>=1.7.1,<2.0.0)
-Requires-Dist: azure-mgmt-datafactory (>=2.2.1,<3.0.0)
+Requires-Dist: azure-mgmt-datafactory (>=2.2.1,<2.7.0)
 Requires-Dist: click (>=8.1.3,<9.0.0)
 Project-URL: Repository, https://github.com/danielvdende/adfpy
 Description-Content-Type: text/markdown
 
 ![tests](https://github.com/danielvdende/adfpy/actions/workflows/lint_test.yml/badge.svg)
 # 🏭🍰 adfPy
 adfPy aims to make developers lives easier by wrapping the Azure Data Factory Python SDK with an intuitive, powerful, and easy to use API that hopefully will remind people of working with Apache Airflow ;-). 
@@ -30,22 +31,22 @@
 ```
 
 ## Usage
 Generally, using adfPy has 2 main components:
 1. Write your pipeline.
 2. Deploy your pipeline.
 
-adfPy has an opinionated syntax, which is heavily influenced by Airflow. For documentation on what the syntax looks like, please read the docs [here]().
+adfPy has an opinionated syntax, which is heavily influenced by Airflow. For documentation on what the syntax looks like, please read the docs [here](https://danielvdende.github.io/adfpy/).
 Some examples are provided in the examples directory of this repository.
 
 
 Once you've written your pipelines, it's time to deploy them! For this, you can use adfPy's deployment script:
 ```shell
 pip install adfpy
-adfpy-deploy
+adfpy-deploy --path <your_path_here>
 ```
 Note:
 - This script will ensure all pipelines in the provided path are present in your target ADF.
 - This script will also **remove** any ADF pipelines that are **not** in your path, but are in ADF.
 
 ## Still to come
 adfPy is still in development. As such, some ADF components are not yet supported:
```

