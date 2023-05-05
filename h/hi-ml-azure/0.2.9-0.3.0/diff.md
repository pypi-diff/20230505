# Comparing `tmp/hi-ml-azure-0.2.9.tar.gz` & `tmp/hi-ml-azure-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/hi-ml-azure-0.2.9.tar", last modified: Wed Nov  9 16:56:29 2022, max compression
+gzip compressed data, was "dist/hi-ml-azure-0.3.0.tar", last modified: Fri May  5 17:32:48 2023, max compression
```

## Comparing `hi-ml-azure-0.2.9.tar` & `hi-ml-azure-0.3.0.tar`

### file list

```diff
@@ -1,30 +1,32 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-09 16:56:29.000000 hi-ml-azure-0.2.9/
--rw-r--r--   0 runner    (1001) docker     (121)     1141 2022-11-09 16:56:13.000000 hi-ml-azure-0.2.9/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)       76 2022-11-09 16:56:13.000000 hi-ml-azure-0.2.9/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     2016 2022-11-09 16:56:29.000000 hi-ml-azure-0.2.9/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1037 2022-11-09 16:56:13.000000 hi-ml-azure-0.2.9/package_description.md
--rw-r--r--   0 runner    (1001) docker     (121)      339 2022-11-09 16:56:13.000000 hi-ml-azure-0.2.9/run_requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-11-09 16:56:29.000000 hi-ml-azure-0.2.9/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     4097 2022-11-09 16:56:13.000000 hi-ml-azure-0.2.9/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-09 16:56:29.000000 hi-ml-azure-0.2.9/src/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-09 16:56:29.000000 hi-ml-azure-0.2.9/src/health_azure/
--rw-r--r--   0 runner    (1001) docker     (121)     1799 2022-11-09 16:56:13.000000 hi-ml-azure-0.2.9/src/health_azure/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     4174 2022-11-09 16:56:13.000000 hi-ml-azure-0.2.9/src/health_azure/amulet.py
--rw-r--r--   0 runner    (1001) docker     (121)    28502 2022-11-09 16:56:13.000000 hi-ml-azure-0.2.9/src/health_azure/datasets.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-09 16:56:29.000000 hi-ml-azure-0.2.9/src/health_azure/examples/
--rw-r--r--   0 runner    (1001) docker     (121)     1334 2022-11-09 16:56:13.000000 hi-ml-azure-0.2.9/src/health_azure/examples/elevate_this.py
--rw-r--r--   0 runner    (1001) docker     (121)    59266 2022-11-09 16:56:13.000000 hi-ml-azure-0.2.9/src/health_azure/himl.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     2143 2022-11-09 16:56:13.000000 hi-ml-azure-0.2.9/src/health_azure/himl_download.py
--rwxr-xr-x   0 runner    (1001) docker     (121)     5632 2022-11-09 16:56:13.000000 hi-ml-azure-0.2.9/src/health_azure/himl_tensorboard.py
--rw-r--r--   0 runner    (1001) docker     (121)     3911 2022-11-09 16:56:13.000000 hi-ml-azure-0.2.9/src/health_azure/logging.py
--rw-r--r--   0 runner    (1001) docker     (121)     1857 2022-11-09 16:56:13.000000 hi-ml-azure-0.2.9/src/health_azure/mlflow_utils.py
--rw-r--r--   0 runner    (1001) docker     (121)     2884 2022-11-09 16:56:13.000000 hi-ml-azure-0.2.9/src/health_azure/paths.py
--rw-r--r--   0 runner    (1001) docker     (121)    11400 2022-11-09 16:56:13.000000 hi-ml-azure-0.2.9/src/health_azure/traverse.py
--rw-r--r--   0 runner    (1001) docker     (121)   106873 2022-11-09 16:56:13.000000 hi-ml-azure-0.2.9/src/health_azure/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-09 16:56:29.000000 hi-ml-azure-0.2.9/src/hi_ml_azure.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     2016 2022-11-09 16:56:29.000000 hi-ml-azure-0.2.9/src/hi_ml_azure.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      673 2022-11-09 16:56:29.000000 hi-ml-azure-0.2.9/src/hi_ml_azure.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-09 16:56:29.000000 hi-ml-azure-0.2.9/src/hi_ml_azure.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)      112 2022-11-09 16:56:29.000000 hi-ml-azure-0.2.9/src/hi_ml_azure.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)      339 2022-11-09 16:56:29.000000 hi-ml-azure-0.2.9/src/hi_ml_azure.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       13 2022-11-09 16:56:29.000000 hi-ml-azure-0.2.9/src/hi_ml_azure.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-05 17:32:48.000000 hi-ml-azure-0.3.0/
+-rw-r--r--   0 runner    (1001) docker     (122)     1141 2023-05-05 17:32:35.000000 hi-ml-azure-0.3.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)       76 2023-05-05 17:32:35.000000 hi-ml-azure-0.3.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)     2016 2023-05-05 17:32:48.000000 hi-ml-azure-0.3.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     1037 2023-05-05 17:32:35.000000 hi-ml-azure-0.3.0/package_description.md
+-rw-r--r--   0 runner    (1001) docker     (122)      337 2023-05-05 17:32:35.000000 hi-ml-azure-0.3.0/run_requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-05-05 17:32:48.000000 hi-ml-azure-0.3.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     4101 2023-05-05 17:32:35.000000 hi-ml-azure-0.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-05 17:32:48.000000 hi-ml-azure-0.3.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-05 17:32:48.000000 hi-ml-azure-0.3.0/src/health_azure/
+-rw-r--r--   0 runner    (1001) docker     (122)     1873 2023-05-05 17:32:35.000000 hi-ml-azure-0.3.0/src/health_azure/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4174 2023-05-05 17:32:35.000000 hi-ml-azure-0.3.0/src/health_azure/amulet.py
+-rw-r--r--   0 runner    (1001) docker     (122)    20546 2023-05-05 17:32:35.000000 hi-ml-azure-0.3.0/src/health_azure/argparsing.py
+-rw-r--r--   0 runner    (1001) docker     (122)    30389 2023-05-05 17:32:35.000000 hi-ml-azure-0.3.0/src/health_azure/datasets.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-05 17:32:48.000000 hi-ml-azure-0.3.0/src/health_azure/examples/
+-rw-r--r--   0 runner    (1001) docker     (122)     1323 2023-05-05 17:32:35.000000 hi-ml-azure-0.3.0/src/health_azure/examples/elevate_this.py
+-rw-r--r--   0 runner    (1001) docker     (122)    61721 2023-05-05 17:32:35.000000 hi-ml-azure-0.3.0/src/health_azure/himl.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)     2115 2023-05-05 17:32:35.000000 hi-ml-azure-0.3.0/src/health_azure/himl_download.py
+-rwxr-xr-x   0 runner    (1001) docker     (122)     5570 2023-05-05 17:32:35.000000 hi-ml-azure-0.3.0/src/health_azure/himl_tensorboard.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5550 2023-05-05 17:32:35.000000 hi-ml-azure-0.3.0/src/health_azure/logging.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1825 2023-05-05 17:32:35.000000 hi-ml-azure-0.3.0/src/health_azure/mlflow_utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1982 2023-05-05 17:32:35.000000 hi-ml-azure-0.3.0/src/health_azure/package_setup.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2884 2023-05-05 17:32:35.000000 hi-ml-azure-0.3.0/src/health_azure/paths.py
+-rw-r--r--   0 runner    (1001) docker     (122)    11400 2023-05-05 17:32:35.000000 hi-ml-azure-0.3.0/src/health_azure/traverse.py
+-rw-r--r--   0 runner    (1001) docker     (122)    95134 2023-05-05 17:32:35.000000 hi-ml-azure-0.3.0/src/health_azure/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-05 17:32:48.000000 hi-ml-azure-0.3.0/src/hi_ml_azure.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     2016 2023-05-05 17:32:48.000000 hi-ml-azure-0.3.0/src/hi_ml_azure.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      738 2023-05-05 17:32:48.000000 hi-ml-azure-0.3.0/src/hi_ml_azure.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-05 17:32:48.000000 hi-ml-azure-0.3.0/src/hi_ml_azure.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      112 2023-05-05 17:32:48.000000 hi-ml-azure-0.3.0/src/hi_ml_azure.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      337 2023-05-05 17:32:48.000000 hi-ml-azure-0.3.0/src/hi_ml_azure.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       13 2023-05-05 17:32:48.000000 hi-ml-azure-0.3.0/src/hi_ml_azure.egg-info/top_level.txt
```

### Comparing `hi-ml-azure-0.2.9/LICENSE` & `hi-ml-azure-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `hi-ml-azure-0.2.9/PKG-INFO` & `hi-ml-azure-0.3.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hi-ml-azure
-Version: 0.2.9
+Version: 0.3.0
 Summary: Microsoft Health Futures package to elevate and monitor scripts to an AzureML workspace
 Home-page: https://github.com/microsoft/hi-ml
 Author: Biomedical Imaging Team @ Microsoft Health Futures
 Author-email: innereyedev@microsoft.com
 License: MIT License
 Description: # Microsoft Health Intelligence Machine Learning Azure Toolbox
```

### Comparing `hi-ml-azure-0.2.9/package_description.md` & `hi-ml-azure-0.3.0/package_description.md`

 * *Files identical despite different names*

### Comparing `hi-ml-azure-0.2.9/setup.py` & `hi-ml-azure-0.3.0/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -31,15 +31,15 @@
 # See also:
 # https://packaging.python.org/guides/publishing-package-distribution-releases-using-github-actions-ci-cd-workflows/
 # https://github.com/pypa/gh-action-pypi-publish
 GITHUB_REF_TAG_COMMIT = "refs/tags/v"
 
 github_ref = os.getenv("GITHUB_REF")
 if github_ref and github_ref.startswith(GITHUB_REF_TAG_COMMIT):
-    version = github_ref[len(GITHUB_REF_TAG_COMMIT):]
+    version = github_ref[len(GITHUB_REF_TAG_COMMIT) :]
 
 # Otherwise, if running from a GitHub Action, but not a tagged commit then GITHUB_RUN_NUMBER will be populated.
 # Use this as a post release number. For example if GITHUB_RUN_NUMBER = 124 then the version string will be
 # "99.99.post124". Although this is discouraged, see:
 # https://www.python.org/dev/peps/pep-0440/#post-releases
 # it is necessary here to avoid duplicate packages in Test.PyPI.
 if not version:
@@ -73,22 +73,22 @@
     author="Biomedical Imaging Team @ Microsoft Health Futures",
     author_email="innereyedev@microsoft.com",
     classifiers=[
         "Development Status :: 3 - Alpha",
         "Intended Audience :: Science/Research",
         "Topic :: Scientific/Engineering :: Medical Science Apps.",
         "License :: OSI Approved :: MIT License",
-        "Programming Language :: Python :: 3.7"
+        "Programming Language :: Python :: 3.7",
     ],
     keywords="Health Futures, Health Intelligence, AzureML",
     license="MIT License",
     packages=find_namespace_packages(where="src"),
     package_dir={"": "src"},
     include_package_data=True,
     install_requires=install_requires,
     entry_points={
         "console_scripts": [
             "himl-tb = health_azure.himl_tensorboard:main",
-            "himl-download = health_azure.himl_download:main"
+            "himl-download = health_azure.himl_download:main",
         ]
-    }
+    },
 )
```

### Comparing `hi-ml-azure-0.2.9/src/health_azure/__init__.py` & `hi-ml-azure-0.3.0/src/health_azure/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,20 +1,38 @@
 #  ------------------------------------------------------------------------------------------
 #  Copyright (c) Microsoft Corporation. All rights reserved.
 #  Licensed under the MIT License (MIT). See LICENSE in the repo root for license information.
 #  ------------------------------------------------------------------------------------------
 
 from health_azure.datasets import DatasetConfig
-from health_azure.himl import (AzureRunInfo, create_crossval_hyperdrive_config, create_run_configuration,
-                               create_script_run, get_workspace, submit_run, submit_to_azure_if_needed)
-from health_azure.utils import (RUN_CONTEXT, aggregate_hyperdrive_metrics, create_aml_run_object,
-                                download_checkpoints_from_run_id, download_files_from_run_id, download_from_datastore,
-                                fetch_run, get_most_recent_run, is_running_in_azure_ml,
-                                set_environment_variables_for_multi_node, split_recovery_id, torch_barrier,
-                                upload_to_datastore)
+from health_azure.himl import (
+    AzureRunInfo,
+    create_crossval_hyperdrive_config,
+    create_run_configuration,
+    create_script_run,
+    get_workspace,
+    submit_run,
+    submit_to_azure_if_needed,
+)
+from health_azure.package_setup import health_azure_package_setup, set_logging_levels
+from health_azure.utils import (
+    RUN_CONTEXT,
+    aggregate_hyperdrive_metrics,
+    create_aml_run_object,
+    download_checkpoints_from_run_id,
+    download_files_from_run_id,
+    download_from_datastore,
+    fetch_run,
+    get_most_recent_run,
+    is_running_in_azure_ml,
+    set_environment_variables_for_multi_node,
+    split_recovery_id,
+    torch_barrier,
+    upload_to_datastore,
+)
 from health_azure.traverse import object_to_yaml, write_yaml_to_object
 
 __all__ = [
     "AzureRunInfo",
     "DatasetConfig",
     "RUN_CONTEXT",
     "create_aml_run_object",
@@ -32,9 +50,11 @@
     "submit_run",
     "submit_to_azure_if_needed",
     "torch_barrier",
     "upload_to_datastore",
     "create_crossval_hyperdrive_config",
     "aggregate_hyperdrive_metrics",
     "object_to_yaml",
-    "write_yaml_to_object"
+    "write_yaml_to_object",
+    "health_azure_package_setup",
+    "set_logging_levels",
 ]
```

### Comparing `hi-ml-azure-0.2.9/src/health_azure/amulet.py` & `hi-ml-azure-0.3.0/src/health_azure/amulet.py`

 * *Files identical despite different names*

### Comparing `hi-ml-azure-0.2.9/src/health_azure/datasets.py` & `hi-ml-azure-0.3.0/src/health_azure/datasets.py`

 * *Files 8% similar despite different names*

```diff
@@ -31,29 +31,32 @@
     Retrieves a datastore of a given name from an AzureML workspace. The datastore_name argument can be omitted if
     the workspace only contains a single datastore. Raises a ValueError if there is no datastore of the given name.
 
     :param workspace: The AzureML workspace to read from.
     :param datastore_name: The name of the datastore to retrieve.
     :return: An AzureML datastore.
     """
+
     def _retrieve_v1_datastore(datastores: Dict[str, Datastore], datastore_name: str) -> Datastore:
         # First check if there is only one datastore, which is then obviously unique.
         # Only then try to use the default datastore, because there may not be a default set.
         existing_stores = list(datastores.keys())
         if not datastore_name:
             if len(existing_stores) == 1:
                 return datastores[existing_stores[0]]
             datastore = workspace.get_default_datastore()
             logging.info(f"Using the workspace default datastore {datastore.name} to access datasets.")
             return datastore
 
         if datastore_name in datastores:
             return datastores[datastore_name]
-        raise ValueError(f"Datastore \"{datastore_name}\" was not found in the \"{workspace.name}\" workspace. "
-                         f"Existing datastores: {existing_stores}")
+        raise ValueError(
+            f"Datastore \"{datastore_name}\" was not found in the \"{workspace.name}\" workspace. "
+            f"Existing datastores: {existing_stores}"
+        )
 
     def _retrieve_v2_datastore(datastores: DatastoreOperations, datastore_name: str) -> V2Datastore:
         existing_stores = list(datastores.list())
         if not datastore_name:
             if len(existing_stores) == 1:
                 return existing_stores[0]
             datastore = datastores.get_default()
@@ -84,16 +87,15 @@
     :return: A Dataset object if it is found, else None.
     """
     logging.info(f"Trying to retrieve AzureML Dataset '{dataset_name}'")
     azureml_dataset = Dataset.get_by_name(workspace, name=dataset_name)
     return azureml_dataset
 
 
-def _create_v1_dataset(datastore_name: str, dataset_name: str, workspace: Workspace
-                       ) -> FileDataset:
+def _create_v1_dataset(datastore_name: str, dataset_name: str, workspace: Workspace) -> FileDataset:
     """
     Create a v1 Dataset in the specified Datastore
 
     :param datastore_name: The AML Datastore to create the Dataset in.
     :param dataset_name: The name of the Dataset to create.
     :param workspace: An AML Workspace object.
     :return: An Azure ML (v1) FileDataset object.
@@ -122,83 +124,142 @@
     :param dataset_name: The name of the Dataset to be retrieved or registered.
     :param workspace: An Azure ML Workspace object.
     :return: An Azure ML Dataset object with the provided dataset name, in the provided datastore.
     """
     try:
         azureml_dataset = _retrieve_v1_dataset(dataset_name, workspace)
     except UserErrorException:
+        if datastore_name == "":
+            raise ValueError(
+                "When creating a new dataset, a datastore name must be provided. Please specify a datastore name using "
+                "the --datastore flag"
+            )
         azureml_dataset = _create_v1_dataset(datastore_name, dataset_name, workspace)
     return azureml_dataset
 
 
-def _retrieve_v2_dataset(dataset_name: str, ml_client: MLClient) -> Data:
+def _get_latest_v2_asset_version(ml_client: MLClient, data_asset_name: str) -> str:
+    """
+    Retrieve the version of a v2 data asset that has the highest value (version numbers are assumed to be integers).
+
+    :param ml_client: An Azure MLClient object for interacting with Azure resources.
+    :param data_asset_name: The name of the data asset to look for.
+    :raises ResourceNotFoundError: If no data asset can be found with a matching name.
+    :return: The latest version of the data asset if found, else None.
+    """
+    data_assets = ml_client.data.list(name=data_asset_name)
+    highest_version = float('-inf')
+
+    for data_asset in data_assets:
+        try:
+            data_asset_version = int(data_asset.version)
+        except ValueError as val_er:
+            logging.warning(f"Failed to convert data asset version to int: {val_er}")
+            continue
+
+        if data_asset_version > highest_version:
+            highest_version = data_asset_version
+
+    if highest_version == float('-inf'):
+        raise ResourceNotFoundError(f"No data asset found with the provided name: {data_asset_name}")
+
+    return str(highest_version)
+
+
+def _retrieve_v2_data_asset(
+    ml_client: MLClient,
+    data_asset_name: str,
+    version: Optional[str] = None,
+) -> Data:
     """
     Attempt to retrieve a v2 Data Asset using a provided Azure ML Workspace connection. If
     no Data asset can be found with a matching name, the underlying code will raise an Exception
 
-    :param dataset_name: The name of the dataset to look for.
     :param ml_client: An Azure MLClient object for interacting with Azure resources.
-    :return: An Azure Data asset representing the dataset if found, otherwise an Exception will be raised.
+    :param data_asset_name: The name of the data asset to look for.
+    :param version: version of the data asset to retrieve, latest version retrieved if None.
+    :return: An Azure Data asset representing the data asset if found.
     """
-    aml_data = ml_client.data.get(name=dataset_name)
+
+    if version is None:
+        version = _get_latest_v2_asset_version(ml_client, data_asset_name)
+
+    aml_data = ml_client.data.get(name=data_asset_name, version=version)
+    assert aml_data.version == version, f"Data asset version ({aml_data.version}) does not match version ({version})"
     return aml_data
 
 
-def _create_v2_dataset(datastore_name: str, dataset_name: str, ml_client: MLClient) -> Data:
+def _create_v2_data_asset(
+    ml_client: MLClient, datastore_name: str, data_asset_name: str, version: Optional[str] = None
+) -> Data:
     """
     Create or update a v2 Data asset in the specified Datastore
 
-    :param datastore_name: The name of the datastore in which to create or update the Data asset.
-    :param dataset_name: The name of the dataset to be created.
     :param ml_client: An Azure MLClient object for interacting with Azure resources.
-    :raises ValueError: If no datastore name is provided to define where to create the data
+    :param datastore_name: The name of the datastore in which to create or update the Data asset.
+    :param data_asset_name: The name of the data asset to be created.
+    :param version: The version of the data asset to be created.
+    :raises ValueError: If no data asset name is provided to define the new asset.
+    :raises ValueError: If no datastore name is provided to define where to create the data.
     :return: The created or updated Data asset.
     """
-    if not dataset_name:
-        raise ValueError(f"Cannot create data asset without a valid dataset name (received {dataset_name})")
+    if data_asset_name == "":
+        raise ValueError("Cannot create data asset with empty name.")
 
-    if not datastore_name:
-        default_datastore = ml_client.datastores.get_default()
-        datastore_name = default_datastore.name
+    if datastore_name == "":
+        raise ValueError(
+            "Cannot create data asset with empty datastore name. Please specify a datastore name using the --datastore flag."
+        )
 
-    logging.info(f"Creating a new Data asset from data in folder '{dataset_name}' in the datastore '{datastore_name}'")
+    logging.info(
+        f"Creating a new Data asset from data in folder '{data_asset_name}' in the datastore '{datastore_name}'"
+    )
     azureml_data_asset = Data(
-        path=f"azureml://datastores/{datastore_name}/paths/{dataset_name}/",
+        path=f"azureml://datastores/{datastore_name}/paths/{data_asset_name}/",
         type=AssetTypes.URI_FOLDER,
         description="<description>",
-        name=dataset_name,
-        version=None
+        name=data_asset_name,
+        version=version,
     )
-    ml_client.data.create_or_update(azureml_data_asset)
+
+    azureml_data_asset = ml_client.data.create_or_update(azureml_data_asset)
     return azureml_data_asset
 
 
-def _get_or_create_v2_dataset(datastore_name: str, dataset_name: str, ml_client: MLClient) -> Data:
+def _get_or_create_v2_data_asset(
+    ml_client: MLClient, datastore_name: str, data_asset_name: str, version: Optional[str] = None
+) -> Data:
     """
-    Attempt to retrieve a v2 Dataset object and return that, otherwise attempt to create and register
-    a v2 Dataset and return that.
+    Attempt to retrieve a v2 data asset object and return that, otherwise attempt to create and register
+    a v2 data asset and return that.
 
-    :param datastore_name: The name of the Datastore to either retrieve or create and register the Data asset in.
-    :param dataset_name: The name of the Data asset to be retrieved or registered.
     :param ml_client: An Azure MLClient object for interacting with Azure resources.
-    :return: An Azure Data asset object with the provided dataset name, in the provided datastore
+    :param datastore_name: The name of the Datastore to either retrieve or create and register the Data asset in.
+    :param data_asset_name: The name of the Data asset to be retrieved or registered.
+    :return: An Azure Data asset object with the provided asset name, in the provided datastore
     """
     try:
-        azureml_dataset = _retrieve_v2_dataset(dataset_name, ml_client)
-    except Exception:
-        azureml_dataset = _create_v2_dataset(datastore_name, dataset_name, ml_client)
-    return azureml_dataset
+        azureml_data_asset = _retrieve_v2_data_asset(ml_client, data_asset_name, version)
+    except ResourceNotFoundError:  # catch the exception and create the dataset, raise all other types of exceptions
+        logging.info(
+            f"Data asset {data_asset_name} not found in datastore {datastore_name}. Version specified: {version}."
+            "Attempting to create a new data asset with specified name and version."
+        )
+        azureml_data_asset = _create_v2_data_asset(ml_client, datastore_name, data_asset_name, version)
+
+    return azureml_data_asset
 
 
-def get_or_create_dataset(datastore_name: str,
-                          dataset_name: str,
-                          workspace: Workspace,
-                          strictly_aml_v1: bool,
-                          ml_client: Optional[MLClient] = None,
-                          ) -> V1OrV2DataType:
+def get_or_create_dataset(
+    datastore_name: str,
+    dataset_name: str,
+    workspace: Workspace,
+    strictly_aml_v1: bool,
+    ml_client: Optional[MLClient] = None,
+) -> V1OrV2DataType:
     """
     Looks in the AzureML datastore for a dataset of the given name. If there is no such dataset, a dataset is
     created and registered, assuming that the files are in a folder that has the same name as the dataset.
     For example, if dataset_name is 'foo', then the 'foo' dataset should be pointing to the folder
     <container_root>/datasets/dataset_name/.
 
     If the command line arg to strictly use AML SDK v1 is set to True, will attempt to retrieve a dataset using
@@ -217,15 +278,15 @@
         raise ValueError("No dataset name provided.")
     if strictly_aml_v1:
         aml_dataset = _get_or_create_v1_dataset(datastore_name, dataset_name, workspace)
         return aml_dataset
     else:
         try:
             ml_client = get_ml_client(ml_client=ml_client)
-            aml_dataset = _get_or_create_v2_dataset(datastore_name, dataset_name, ml_client)
+            aml_dataset = _get_or_create_v2_data_asset(ml_client, datastore_name, dataset_name)
         except HttpResponseError as e:
             if "Cannot create v2 Data Version in v1 Data Container" in e.message:
                 logging.info("This appears to be a v1 Data Container. Reverting to API v1 to create this Dataset")
             aml_dataset = _get_or_create_v1_dataset(datastore_name, dataset_name, workspace)
 
         return aml_dataset
 
@@ -239,26 +300,31 @@
 
 
 class DatasetConfig:
     """
     Contains information to use AzureML datasets as inputs or outputs.
     """
 
-    def __init__(self,
-                 name: str,
-                 datastore: str = "",
-                 version: Optional[int] = None,
-                 use_mounting: Optional[bool] = None,
-                 target_folder: Optional[PathOrString] = None,
-                 local_folder: Optional[PathOrString] = None):
+    def __init__(
+        self,
+        name: str,
+        datastore: str = "",
+        overwrite_existing: bool = True,
+        version: Optional[int] = None,
+        use_mounting: Optional[bool] = None,
+        target_folder: Optional[PathOrString] = None,
+        local_folder: Optional[PathOrString] = None,
+    ):
         """
         :param name: The name of the dataset, as it was registered in the AzureML workspace. For output datasets,
             this will be the name given to the newly created dataset.
         :param datastore: The name of the AzureML datastore that holds the dataset. This can be empty if the AzureML
             workspace has only a single datastore, or if the default datastore should be used.
+        :param overwrite_existing: Only applies to uploading datasets. If True, the dataset will be overwritten if it
+            already exists. If False, the dataset creation will fail if the dataset already exists.
         :param version: The version of the dataset that should be used. This is only used for input datasets.
             If the version is not specified, the latest version will be used.
         :param use_mounting: If True, the dataset will be "mounted", that is, individual files will be read
             or written on-demand over the network. If False, the dataset will be fully downloaded before the job starts,
             respectively fully uploaded at job end for output datasets.
             Defaults: False (downloading) for datasets that are script inputs, True (mounting) for datasets that are
             script outputs.
@@ -271,27 +337,29 @@
         # This class would be a good candidate for a dataclass, but having an explicit constructor makes
         # documentation tools in the editor work nicer.
         name = name.strip()
         if not name:
             raise ValueError("The name of the dataset must be a non-empty string.")
         self.name = name
         self.datastore = datastore
+        self.overwrite_existing = overwrite_existing
         self.version = version
         self.use_mounting = use_mounting
         # If target_folder is "" then convert to None
         self.target_folder = Path(target_folder) if target_folder else None
         if str(self.target_folder) == ".":
             raise ValueError("Can't mount or download a dataset to the current working directory.")
         self.local_folder = Path(local_folder) if local_folder else None
 
-    def to_input_dataset_local(self,
-                               strictly_aml_v1: bool,
-                               workspace: Workspace = None,
-                               ml_client: Optional[MLClient] = None,
-                               ) -> Tuple[Optional[Path], Optional[MountContext]]:
+    def to_input_dataset_local(
+        self,
+        strictly_aml_v1: bool,
+        workspace: Workspace = None,
+        ml_client: Optional[MLClient] = None,
+    ) -> Tuple[Optional[Path], Optional[MountContext]]:
         """
         Return a local path to the dataset when outside of an AzureML run.
         If local_folder is supplied, then this is assumed to be a local dataset, and this is returned.
         Otherwise the dataset is mounted or downloaded to either the target folder or a temporary folder and that is
         returned. If self.name refers to a v2 dataset, it is not possible to mount the data here,
         therefore a tuple of Nones will be returned.
 
@@ -305,21 +373,25 @@
 
         if self.local_folder is not None:
             status += f"obtained from local folder {str(self.local_folder)}"
             print(status)
             return self.local_folder, None
 
         if workspace is None:
-            raise ValueError(f"Unable to make dataset '{self.name} available for a local run because no AzureML "
-                             "workspace has been provided. Provide a workspace, or set a folder for local execution.")
-        azureml_dataset = get_or_create_dataset(workspace=workspace,
-                                                ml_client=ml_client,
-                                                dataset_name=self.name,
-                                                datastore_name=self.datastore,
-                                                strictly_aml_v1=strictly_aml_v1)
+            raise ValueError(
+                f"Unable to make dataset '{self.name} available for a local run because no AzureML "
+                "workspace has been provided. Provide a workspace, or set a folder for local execution."
+            )
+        azureml_dataset = get_or_create_dataset(
+            datastore_name=self.datastore,
+            dataset_name=self.name,
+            workspace=workspace,
+            strictly_aml_v1=strictly_aml_v1,
+            ml_client=ml_client,
+        )
         if isinstance(azureml_dataset, FileDataset):
             target_path = self.target_folder or Path(tempfile.mkdtemp())
             use_mounting = self.use_mounting if self.use_mounting is not None else False
             if use_mounting:
                 status += f"mounted at {target_path}"
 
                 mount_context = azureml_dataset.mount(mount_point=str(target_path))  # type: ignore
@@ -330,35 +402,38 @@
                 azureml_dataset.download(target_path=str(target_path), overwrite=False)  # type: ignore
                 result = target_path, None
             print(status)
             return result
         else:
             return None, None
 
-    def to_input_dataset(self,
-                         dataset_index: int,
-                         workspace: Workspace,
-                         strictly_aml_v1: bool,
-                         ml_client: Optional[MLClient] = None,
-                         ) -> Optional[DatasetConsumptionConfig]:
+    def to_input_dataset(
+        self,
+        dataset_index: int,
+        workspace: Workspace,
+        strictly_aml_v1: bool,
+        ml_client: Optional[MLClient] = None,
+    ) -> Optional[DatasetConsumptionConfig]:
         """
         Creates a configuration for using an AzureML dataset inside of an AzureML run. This will make the AzureML
         dataset with given name available as a named input, using INPUT_0 as the key for dataset index 0.
 
         :param workspace: The AzureML workspace to read from.
         :param dataset_index: Suffix for using datasets as named inputs, the dataset will be marked INPUT_{index}
         :param strictly_aml_v1: If True, use Azure ML SDK v1. Otherwise, attempt to use Azure ML SDK v2.
         :param ml_client: An Azure MLClient object for interacting with Azure resources.
         """
         status = f"In AzureML, dataset {self.name} (index {dataset_index}) will be "
-        azureml_dataset = get_or_create_dataset(workspace=workspace,
-                                                ml_client=ml_client,
-                                                dataset_name=self.name,
-                                                datastore_name=self.datastore,
-                                                strictly_aml_v1=strictly_aml_v1)
+        azureml_dataset = get_or_create_dataset(
+            datastore_name=self.datastore,
+            dataset_name=self.name,
+            workspace=workspace,
+            strictly_aml_v1=strictly_aml_v1,
+            ml_client=ml_client,
+        )
         # If running on windows then self.target_folder may be a WindowsPath, make sure it is
         # in posix format for Azure.
         use_mounting = False if self.use_mounting is None else self.use_mounting
         if isinstance(azureml_dataset, FileDataset):
             named_input = azureml_dataset.as_named_input(_input_dataset_key(index=dataset_index))  # type: ignore
             path_on_compute = self.target_folder.as_posix() if self.target_folder is not None else None
             if use_mounting:
@@ -372,66 +447,65 @@
             else:
                 status += "a randomly chosen folder."
             print(status)
             return result
         else:
             return None
 
-    def to_output_dataset(self,
-                          workspace: Workspace,
-                          dataset_index: int) -> OutputFileDatasetConfig:
+    def to_output_dataset(self, workspace: Workspace, dataset_index: int) -> OutputFileDatasetConfig:
         """
         Creates a configuration to write a script output to an AzureML dataset. The name and datastore of this new
         dataset will be taken from the present object.
 
         :param workspace: The AzureML workspace to read from.
         :param dataset_index: Suffix for using datasets as named inputs, the dataset will be marked OUTPUT_{index}
-        :return:
+        :return: An AzureML OutputFileDatasetConfig object, representing the output dataset.
         """
         status = f"Output dataset {self.name} (index {dataset_index}) will be "
         datastore = get_datastore(workspace, self.datastore)
-        dataset = OutputFileDatasetConfig(name=_output_dataset_key(index=dataset_index),
-                                          destination=(datastore, self.name + "/"))
+        dataset = OutputFileDatasetConfig(
+            name=_output_dataset_key(index=dataset_index), destination=(datastore, self.name + "/")
+        )
         # TODO: Can we get tags into here too?
         dataset = dataset.register_on_complete(name=self.name)
         if self.target_folder:
             raise ValueError("Output datasets can't have a target_folder set.")
         use_mounting = True if self.use_mounting is None else self.use_mounting
         if use_mounting:
             status += "uploaded while the job runs."
             result = dataset.as_mount()
         else:
             status += "uploaded when the job completes."
-            result = dataset.as_upload()
+            result = dataset.as_upload(overwrite=self.overwrite_existing)
         logging.info(status)
         return result
 
 
 StrOrDatasetConfig = Union[str, DatasetConfig]
 
 
-def _replace_string_datasets(datasets: List[StrOrDatasetConfig],
-                             default_datastore_name: str) -> List[DatasetConfig]:
+def _replace_string_datasets(datasets: List[StrOrDatasetConfig], default_datastore_name: str) -> List[DatasetConfig]:
     """
     Processes a list of input or output datasets. All entries in the list that are strings are turned into
     DatasetConfig objects, using the string as the dataset name, and pointing to the default datastore.
 
     :param datasets: A list of datasets, each given either as a string or a DatasetConfig object.
     :param default_datastore_name: The datastore to use for all datasets that are only specified via their name.
     :return: A list of DatasetConfig objects, in the same order as the input list.
     """
-    return [DatasetConfig(name=d, datastore=default_datastore_name) if isinstance(d, str) else d
-            for d in datasets]
+    return [DatasetConfig(name=d, datastore=default_datastore_name) if isinstance(d, str) else d for d in datasets]
 
 
-def create_dataset_configs(all_azure_dataset_ids: List[str],
-                           all_dataset_mountpoints: Sequence[PathOrString],
-                           all_local_datasets: List[Optional[Path]],
-                           datastore: Optional[str] = None,
-                           use_mounting: bool = False) -> List[DatasetConfig]:
+def create_dataset_configs(
+    all_azure_dataset_ids: List[str],
+    all_dataset_mountpoints: Sequence[PathOrString],
+    all_local_datasets: List[Optional[Path]],
+    datastore: Optional[str] = None,
+    use_mounting: bool = False,
+) -> List[DatasetConfig]:
     """
     Sets up all the dataset consumption objects for the datasets provided. The returned list will have the same length
     as there are non-empty azure dataset IDs.
 
     Valid arguments combinations:
     N azure datasets, 0 or N mount points, 0 or N local datasets
 
@@ -453,38 +527,42 @@
     if num_azure > 0 and (num_local == 0 or num_local == num_azure) and (num_mount == 0 or num_mount == num_azure):
         # Test for valid settings: If we have N azure datasets, the local datasets and mount points need to either
         # have exactly the same length, or 0. In the latter case, empty mount points and no local dataset will be
         # assumed below.
         count = num_azure
     elif num_azure == 0 and num_mount == 0:
         # No datasets in Azure at all: This is possible for runs that for example download their own data from the web.
-        # There can be any number of local datasets, but we are not checking that. In MLRunner.setup, there is a check
+        # There can be any number of local datasets, but we are not checking that. In TrainingRunner.setup, there is a check
         # that leaves local datasets intact if there are no Azure datasets.
         return []
     else:
-        raise ValueError("Invalid dataset setup. You need to specify N entries in azure_datasets and a matching "
-                         "number of local_datasets and dataset_mountpoints")
+        raise ValueError(
+            "Invalid dataset setup. You need to specify N entries in azure_datasets and a matching "
+            "number of local_datasets and dataset_mountpoints"
+        )
     for i in range(count):
         azure_dataset = all_azure_dataset_ids[i] if i < num_azure else ""
         if not azure_dataset:
             continue
         mount_point = all_dataset_mountpoints[i] if i < num_mount else ""
         local_dataset = all_local_datasets[i] if i < num_local else None
-        config = DatasetConfig(name=azure_dataset,
-                               target_folder=mount_point,
-                               local_folder=local_dataset,
-                               use_mounting=use_mounting,
-                               datastore=datastore or "")
+        config = DatasetConfig(
+            name=azure_dataset,
+            target_folder=mount_point,
+            local_folder=local_dataset,
+            use_mounting=use_mounting,
+            datastore=datastore or "",
+        )
         datasets.append(config)
     return datasets
 
 
-def find_workspace_for_local_datasets(aml_workspace: Optional[Workspace],
-                                      workspace_config_path: Optional[Path],
-                                      dataset_configs: List[DatasetConfig]) -> Optional[Workspace]:
+def find_workspace_for_local_datasets(
+    aml_workspace: Optional[Workspace], workspace_config_path: Optional[Path], dataset_configs: List[DatasetConfig]
+) -> Optional[Workspace]:
     """
     If any of the dataset_configs require an AzureML workspace then try to get one, otherwise return None.
 
     :param aml_workspace: There are two optional parameters used to glean an existing AzureML Workspace. The simplest is
         to pass it in as a parameter.
     :param workspace_config_path: The 2nd option is to specify the path to the config.json file downloaded from the
         Azure portal from which we can retrieve the existing Workspace.
@@ -499,20 +577,21 @@
             workspace = get_workspace(aml_workspace, workspace_config_path)
             logging.info(f"Found workspace for datasets: {workspace.name}")
         except Exception as ex:
             logging.info(f"Could not find workspace for datasets. Exception: {ex}")
     return workspace
 
 
-def setup_local_datasets(dataset_configs: List[DatasetConfig],
-                         strictly_aml_v1: bool,
-                         aml_workspace: Optional[Workspace] = None,
-                         ml_client: Optional[MLClient] = None,
-                         workspace_config_path: Optional[Path] = None,
-                         ) -> Tuple[List[Optional[Path]], List[MountContext]]:
+def setup_local_datasets(
+    dataset_configs: List[DatasetConfig],
+    strictly_aml_v1: bool,
+    aml_workspace: Optional[Workspace] = None,
+    ml_client: Optional[MLClient] = None,
+    workspace_config_path: Optional[Path] = None,
+) -> Tuple[List[Optional[Path]], List[MountContext]]:
     """
     When running outside of AzureML, setup datasets to be used locally.
 
     For each DatasetConfig, if local_folder is supplied, then this is assumed to be a local dataset, and this is
     used. Otherwise the dataset is mounted or downloaded to either the target folder or a temporary folder and that is
     used.
```

### Comparing `hi-ml-azure-0.2.9/src/health_azure/examples/elevate_this.py` & `hi-ml-azure-0.3.0/src/health_azure/examples/elevate_this.py`

 * *Files 4% similar despite different names*

```diff
@@ -20,17 +20,16 @@
 def main() -> None:
     """
     Write out the given message, in an AzureML 'experiment' if required.
 
     First call submit_to_azure_if_needed.
     """
     _ = submit_to_azure_if_needed(
-        compute_cluster_name="lite-testing-ds2",
-        wait_for_completion=True,
-        wait_for_completion_show_output=True)
+        compute_cluster_name="lite-testing-ds2", wait_for_completion=True, wait_for_completion_show_output=True
+    )
 
     parser = ArgumentParser()
     parser.add_argument("-m", "--message", type=str, required=True, help="The message to print out")
     args = parser.parse_args()
 
     print(f"The message was: {args.message}")
```

### Comparing `hi-ml-azure-0.2.9/src/health_azure/himl.py` & `hi-ml-azure-0.3.0/src/health_azure/himl.py`

 * *Files 6% similar despite different names*

```diff
@@ -9,75 +9,104 @@
 See examples/elevate_this.py for a very simple 'hello world' example of use.
 """
 
 import logging
 import os
 import re
 import sys
-import warnings
 from argparse import ArgumentParser
 from contextlib import contextmanager
 from dataclasses import dataclass
 from pathlib import Path
 from typing import Any, Callable, Dict, Generator, List, Optional, Tuple, Union
 
-from azure.ai.ml import MLClient, Input, Output, command
-from azure.ai.ml.constants import AssetTypes, InputOutputModes
-from azure.ai.ml.entities import Data, Job, Command, Sweep
+from azure.ai.ml import Input, MLClient, Output, command
+from azure.ai.ml.constants import InputOutputModes
+from azure.ai.ml.entities import Command, Data
 from azure.ai.ml.entities import Environment as EnvironmentV2
-
+from azure.ai.ml.entities import Job, Sweep, UserIdentityConfiguration
+from azure.ai.ml.entities._job.distribution import MpiDistribution, PyTorchDistribution
 from azure.ai.ml.sweep import Choice
 from azureml._base_sdk_common import user_agent
 from azureml.core import ComputeTarget, Environment, Experiment, Run, RunConfiguration, ScriptRunConfig, Workspace
 from azureml.core.runconfig import DockerConfiguration, MpiConfiguration
 from azureml.data import OutputFileDatasetConfig
 from azureml.data.dataset_consumption_config import DatasetConsumptionConfig
-from azureml.train.hyperdrive import HyperDriveConfig, GridParameterSampling, PrimaryMetricGoal, choice
 from azureml.dataprep.fuse.daemon import MountContext
+from azureml.train.hyperdrive import GridParameterSampling, HyperDriveConfig, PrimaryMetricGoal, choice
 
-from health_azure.amulet import (ENV_AMLT_DATAREFERENCE_DATA, ENV_AMLT_DATAREFERENCE_OUTPUT, is_amulet_job)
-from health_azure.utils import (create_python_environment, create_run_recovery_id, find_file_in_parent_to_pythonpath,
-                                is_run_and_child_runs_completed, is_running_in_azure_ml, register_environment,
-                                run_duration_string_to_seconds, to_azure_friendly_string, RUN_CONTEXT, get_workspace,
-                                PathOrString, DEFAULT_ENVIRONMENT_VARIABLES, get_ml_client,
-                                create_python_environment_v2, register_environment_v2, V2_INPUT_DATASET_PATTERN,
-                                V2_OUTPUT_DATASET_PATTERN)
-from health_azure.datasets import (DatasetConfig, StrOrDatasetConfig, setup_local_datasets,
-                                   _input_dataset_key, _output_dataset_key, _replace_string_datasets)
-
+from health_azure.amulet import ENV_AMLT_DATAREFERENCE_DATA, ENV_AMLT_DATAREFERENCE_OUTPUT, is_amulet_job
+from health_azure.datasets import (
+    DatasetConfig,
+    StrOrDatasetConfig,
+    _get_or_create_v2_data_asset,
+    _input_dataset_key,
+    _output_dataset_key,
+    _replace_string_datasets,
+    setup_local_datasets,
+)
+from health_azure.package_setup import health_azure_package_setup
+from health_azure.utils import (
+    DEFAULT_ENVIRONMENT_VARIABLES,
+    ENV_EXPERIMENT_NAME,
+    RUN_CONTEXT,
+    PathOrString,
+    create_python_environment,
+    create_python_environment_v2,
+    create_run_recovery_id,
+    create_v2_job_command_line_args_from_params,
+    find_file_in_parent_to_pythonpath,
+    get_ml_client,
+    get_workspace,
+    is_run_and_child_runs_completed,
+    is_running_in_azure_ml,
+    register_environment,
+    register_environment_v2,
+    run_duration_string_to_seconds,
+    to_azure_friendly_string,
+    wait_for_job_completion,
+)
 
 logger = logging.getLogger('health_azure')
 logger.setLevel(logging.DEBUG)
 
 AML_IGNORE_FILE = ".amlignore"
-AZUREML_COMMANDLINE_FLAG = "--azureml"
+AZUREML_FLAG = "--azureml"
 CONDA_ENVIRONMENT_FILE = "environment.yml"
 LOGS_FOLDER = "logs"
 OUTPUT_FOLDER = "outputs"
 RUN_RECOVERY_FILE = "most_recent_run.txt"
 SDK_NAME = "innereye"
 SDK_VERSION = "2.0"
 
+DEFAULT_DOCKER_BASE_IMAGE = "mcr.microsoft.com/azureml/openmpi4.1.0-cuda11.3-cudnn8-ubuntu20.04"
+DEFAULT_DOCKER_SHM_SIZE = "100g"
+
 # hyperparameter search args
 PARAM_SAMPLING_ARG = "parameter_sampling"
 MAX_TOTAL_TRIALS_ARG = "max_total_trials"
 PRIMARY_METRIC_ARG = "primary_metric"
 SAMPLING_ALGORITHM_ARG = "sampling_algorithm"
 GOAL_ARG = "goal"
 
+V2_INPUT_ASSET_IDENTIFIER = "INPUT_"
+V2_OUTPUT_ASSET_IDENTIFIER = "OUTPUT_"
+# TODO: upgrade to python 3.8+ and create a Literal type for the combination of the above two vars
+
 
 @dataclass
 class AzureRunInfo:
     """
     This class stores all information that a script needs to run inside and outside of AzureML. It is return
     from `submit_to_azure_if_needed`, where the return value depends on whether the script is inside or outside
     AzureML.
 
     Please check the source code for detailed documentation for all fields.
     """
+
     input_datasets: List[Optional[Path]]
     """A list of folders that contain all the datasets that the script uses as inputs. Input datasets must be
      specified when calling `submit_to_azure_if_needed`. Here, they are made available as Path objects. If no input
      datasets are specified, the list is empty."""
     output_datasets: List[Optional[Path]]
     """A list of folders that contain all the datasets that the script uses as outputs. Output datasets must be
          specified when calling `submit_to_azure_if_needed`. Here, they are made available as Path objects. If no output
@@ -87,18 +116,18 @@
     for each input dataset where there is no local_folder, there is a workspace, and use_mounting is set.
     This list is maintained only to prevent exit from these contexts until the RunInfo object is deleted."""
     run: Optional[Run]
     """An AzureML Run object if the present script is executing inside AzureML, or None if outside of AzureML.
     The Run object has methods to log metrics, upload files, etc."""
     is_running_in_azure_ml: bool
     """If True, the present script is executing inside AzureML. If False, outside AzureML."""
-    output_folder: Path
+    output_folder: Optional[Path]
     """The output folder into which all script outputs should be written, if they should be later available in the
     AzureML portal. Files written to this folder will be uploaded to blob storage at the end of the script run."""
-    logs_folder: Path
+    logs_folder: Optional[Path]
     """The folder into which all log files (for example, tensorboard) should be written. All files written to this
     folder will be uploaded to blob storage regularly during the script run."""
 
 
 def validate_num_nodes(compute_cluster: ComputeTarget, num_nodes: int) -> None:
     """
     Check that the user hasn't requested more nodes than the maximum number of nodes allowed by
@@ -108,28 +137,31 @@
         should be checked
     :param num_nodes: The number of nodes that the user has requested
     """
     max_cluster_nodes: int = compute_cluster.scale_settings.maximum_node_count
     if num_nodes > max_cluster_nodes:
         raise ValueError(
             f"You have requested {num_nodes} nodes, which is more than your compute cluster "
-            f"({compute_cluster.name})'s maximum of {max_cluster_nodes} nodes.")
+            f"({compute_cluster.name})'s maximum of {max_cluster_nodes} nodes."
+        )
 
 
 def validate_compute_name(existing_compute_targets: Dict[str, ComputeTarget], compute_target_name: str) -> None:
     """
     Check that a specified compute target is one of the available existing compute targets in a Workspace
 
     :param existing_compute_targets: A list of AML ComputeTarget objects available to a given AML Workspace
     :param compute_cluster_name: The name of the specific compute target whose name to look up in existing
         compute targets
     """
     if compute_target_name not in existing_compute_targets:
-        raise ValueError(f"Could not find the compute target {compute_target_name} in the AzureML workspace. ",
-                         f"Existing compute targets: {list(existing_compute_targets)}")
+        raise ValueError(
+            f"Could not find the compute target {compute_target_name} in the AzureML workspace. ",
+            f"Existing compute targets: {list(existing_compute_targets)}",
+        )
 
 
 def validate_compute_cluster(workspace: Workspace, compute_cluster_name: str, num_nodes: int) -> None:
     """
     Check that both the specified compute cluster exists in the given Workspace, and that it has enough
     nodes to spin up the requested number of nodes
 
@@ -139,28 +171,29 @@
     """
     existing_compute_clusters: Dict[str, ComputeTarget] = workspace.compute_targets
     validate_compute_name(existing_compute_clusters, compute_cluster_name)
     compute_cluster = existing_compute_clusters[compute_cluster_name]
     validate_num_nodes(compute_cluster, num_nodes)
 
 
-def create_run_configuration(workspace: Workspace,
-                             compute_cluster_name: str,
-                             conda_environment_file: Optional[Path] = None,
-                             aml_environment_name: str = "",
-                             environment_variables: Optional[Dict[str, str]] = None,
-                             pip_extra_index_url: str = "",
-                             private_pip_wheel_path: Optional[Path] = None,
-                             docker_base_image: str = "",
-                             docker_shm_size: str = "",
-                             num_nodes: int = 1,
-                             max_run_duration: str = "",
-                             input_datasets: Optional[List[DatasetConfig]] = None,
-                             output_datasets: Optional[List[DatasetConfig]] = None,
-                             ) -> RunConfiguration:
+def create_run_configuration(
+    workspace: Workspace,
+    compute_cluster_name: str,
+    conda_environment_file: Optional[Path] = None,
+    aml_environment_name: str = "",
+    environment_variables: Optional[Dict[str, str]] = None,
+    pip_extra_index_url: str = "",
+    private_pip_wheel_path: Optional[Path] = None,
+    docker_base_image: str = "",
+    docker_shm_size: str = "",
+    num_nodes: int = 1,
+    max_run_duration: str = "",
+    input_datasets: Optional[List[DatasetConfig]] = None,
+    output_datasets: Optional[List[DatasetConfig]] = None,
+) -> RunConfiguration:
     """
     Creates an AzureML run configuration, that contains information about environment, multi node execution, and
     Docker.
 
     :param workspace: The AzureML Workspace to use.
     :param aml_environment_name: The name of an AzureML environment that should be used to submit the script. If not
         provided, an environment will be created from the arguments to this function (conda_environment_file,
@@ -194,15 +227,16 @@
         # Create an AzureML environment, then check if it exists already. If it exists, use the registered
         # environment, otherwise register the new environment.
         new_environment = create_python_environment(
             conda_environment_file=conda_environment_file,
             pip_extra_index_url=pip_extra_index_url,
             workspace=workspace,
             private_pip_wheel_path=private_pip_wheel_path,
-            docker_base_image=docker_base_image)
+            docker_base_image=docker_base_image,
+        )
         conda_deps = new_environment.python.conda_dependencies
         if conda_deps.get_python_version() is None:
             raise ValueError("If specifying a conda environment file, you must specify the python version within it")
         registered_env = register_environment(workspace, new_environment)
         run_config.environment = registered_env
     else:
         raise ValueError("One of the two arguments 'aml_environment_name' or 'conda_environment_file' must be given.")
@@ -226,28 +260,27 @@
         distributed_job_config = MpiConfiguration(node_count=num_nodes)
         run_config.mpi = distributed_job_config
         run_config.framework = "Python"
         run_config.communicator = "IntelMpi"
         run_config.node_count = distributed_job_config.node_count
 
     if input_datasets or output_datasets:
-        inputs, outputs = convert_himl_to_azureml_datasets(cleaned_input_datasets=input_datasets or [],
-                                                           cleaned_output_datasets=output_datasets or [],
-                                                           workspace=workspace,
-                                                           strictly_aml_v1=True
-                                                           )
+        inputs, outputs = convert_himl_to_azureml_datasets(
+            cleaned_input_datasets=input_datasets or [],
+            cleaned_output_datasets=output_datasets or [],
+            workspace=workspace,
+            strictly_aml_v1=True,
+        )
         run_config.data = inputs
         run_config.output_data = outputs
 
     return run_config
 
 
-def create_grid_hyperdrive_config(values: List[str],
-                                  argument_name: str,
-                                  metric_name: str) -> HyperDriveConfig:
+def create_grid_hyperdrive_config(values: List[str], argument_name: str, metric_name: str) -> HyperDriveConfig:
     """
     Creates an Azure ML HyperDriveConfig object that runs a simple grid search. The Hyperdrive job will run one child
     job for each of the values provided in `values`, and each child job will have a suffix added to the commandline
     like `--argument_name value`.
 
     Note: this config expects that a metric is logged in your training script([see here](
     https://docs.microsoft.com/en-us/azure/machine-learning/how-to-tune-hyperparameters#log-metrics-for-hyperparameter-tuning))
@@ -256,32 +289,32 @@
     :param values: The list of values to try for the commandline argument given by `argument_name`.
     :param argument_name: The name of the commandline argument that each of the child runs gets, to
         indicate which value they should work on.
     :param metric_name: The name of the metric that the HyperDriveConfig will compare runs by. Please note that it is
         your responsibility to make sure a metric with this name is logged to the Run in your training script
     :return: an Azure ML HyperDriveConfig object
     """
-    logging.info(f"Creating a HyperDriveConfig. Please note that this expects to find the specified "
-                 f"metric '{metric_name}' logged to AzureML from your training script (for example, using the "
-                 f"AzureMLLogger with Pytorch Lightning)")
+    logging.info(
+        f"Creating a HyperDriveConfig. Please note that this expects to find the specified "
+        f"metric '{metric_name}' logged to AzureML from your training script (for example, using the "
+        f"AzureMLLogger with Pytorch Lightning)"
+    )
     parameter_dict = {
         argument_name: choice(values),
     }
     return HyperDriveConfig(
         run_config=ScriptRunConfig(""),
         hyperparameter_sampling=GridParameterSampling(parameter_dict),
         primary_metric_name=metric_name,
         primary_metric_goal=PrimaryMetricGoal.MINIMIZE,
-        max_total_runs=len(values)
+        max_total_runs=len(values),
     )
 
 
-def create_grid_hyperparam_args_v2(values: List[Any],
-                                   argument_name: str,
-                                   metric_name: str) -> Dict[str, Any]:
+def create_grid_hyperparam_args_v2(values: List[Any], argument_name: str, metric_name: str) -> Dict[str, Any]:
     """
     Create a dictionary of arguments to create an Azure ML v2 SDK Sweep job.
 
     :param values: The list of values to try for the commandline argument given by `argument_name`.
     :param argument_name: The name of the commandline argument that each of the child runs gets, to
         indicate which value they should work on.
     :param metric_name: The name of the metric that the sweep job will compare runs by. Please note that it is
@@ -290,69 +323,72 @@
     """
     param_sampling = {argument_name: Choice(values)}
     hyperparam_args = {
         MAX_TOTAL_TRIALS_ARG: len(values),
         PARAM_SAMPLING_ARG: param_sampling,
         SAMPLING_ALGORITHM_ARG: "grid",
         PRIMARY_METRIC_ARG: metric_name,
-        GOAL_ARG: "Minimize"
+        GOAL_ARG: "Minimize",
     }
     return hyperparam_args
 
 
-def create_crossval_hyperdrive_config(num_splits: int,
-                                      cross_val_index_arg_name: str = "crossval_index",
-                                      metric_name: str = "val/loss") -> HyperDriveConfig:
+def create_crossval_hyperdrive_config(
+    num_splits: int, cross_val_index_arg_name: str = "crossval_index", metric_name: str = "val/loss"
+) -> HyperDriveConfig:
     """
     Creates an Azure ML HyperDriveConfig object for running cross validation. Note: this config expects a metric
     named <metric_name> to be logged in your training script([see here](
     https://docs.microsoft.com/en-us/azure/machine-learning/how-to-tune-hyperparameters#log-metrics-for-hyperparameter-tuning))
 
     :param num_splits: The number of splits for k-fold cross validation
     :param cross_val_index_arg_name: The name of the commandline argument that each of the child runs gets, to
         indicate which split they should work on.
     :param metric_name: The name of the metric that the HyperDriveConfig will compare runs by. Please note that it is
         your responsibility to make sure a metric with this name is logged to the Run in your training script
     :return: an Azure ML HyperDriveConfig object
     """
-    return create_grid_hyperdrive_config(values=list(map(str, range(num_splits))),
-                                         argument_name=cross_val_index_arg_name,
-                                         metric_name=metric_name)
+    return create_grid_hyperdrive_config(
+        values=list(map(str, range(num_splits))), argument_name=cross_val_index_arg_name, metric_name=metric_name
+    )
 
 
-def create_crossval_hyperparam_args_v2(num_splits: int,
-                                       cross_val_index_arg_name: str = "crossval_index",
-                                       metric_name: str = "val/loss") -> Dict[str, Any]:
+def create_crossval_hyperparam_args_v2(
+    num_splits: int, cross_val_index_arg_name: str = "crossval_index", metric_name: str = "val/loss"
+) -> Dict[str, Any]:
     """
     Create a dictionary of arguments to create an Azure ML v2 SDK Sweep job.
 
     :param num_splits: The number of splits for k-fold cross validation
     :param cross_val_index_arg_name: The name of the commandline argument that each of the child runs gets, to
         indicate which split they should work on.
     :param metric_name: The name of the metric that the HyperDriveConfig will compare runs by. Please note that it is
         your responsibility to make sure a metric with this name is logged to the Run in your training script
     :return: A dictionary of arguments and values to pass in to the command job.
     """
-    return create_grid_hyperparam_args_v2(values=list(map(str, range(num_splits))),
-                                          argument_name=cross_val_index_arg_name,
-                                          metric_name=metric_name)
+    return create_grid_hyperparam_args_v2(
+        values=list(map(str, range(num_splits))), argument_name=cross_val_index_arg_name, metric_name=metric_name
+    )
 
 
-def create_script_run(snapshot_root_directory: Optional[Path] = None,
-                      entry_script: Optional[PathOrString] = None,
-                      script_params: Optional[List[str]] = None) -> ScriptRunConfig:
+def create_script_run(
+    script_params: List[str],
+    snapshot_root_directory: Optional[Path] = None,
+    entry_script: Optional[PathOrString] = None,
+) -> ScriptRunConfig:
     """
     Creates an AzureML ScriptRunConfig object, that holds the information about the snapshot, the entry script, and
     its arguments.
 
-    :param entry_script: The script that should be run in AzureML.
+    :param script_params: A list of parameter to pass on to the script as it runs in AzureML. Required arg. Script
+        parameters can be generated using the ``_get_script_params()`` function.
     :param snapshot_root_directory: The directory that contains all code that should be packaged and sent to AzureML.
         All Python code that the script uses must be copied over.
-    :param script_params: A list of parameter to pass on to the script as it runs in AzureML. If empty (or None, the
-        default) these will be copied over from sys.argv, omitting the --azureml flag.
+    :param entry_script: The script that should be run in AzureML. If None, the current main Python file will be
+        executed.
     :return:
     """
     if snapshot_root_directory is None:
         print("No snapshot root directory given. All files in the current working directory will be copied to AzureML.")
         snapshot_root_directory = Path.cwd()
     else:
         print(f"All files in this folder will be copied to AzureML: {snapshot_root_directory}")
@@ -362,192 +398,214 @@
     elif isinstance(entry_script, str):
         entry_script = Path(entry_script)
     if entry_script.is_absolute():
         try:
             # The entry script always needs to use Linux path separators, even when submitting from Windows
             entry_script_relative = entry_script.relative_to(snapshot_root_directory).as_posix()
         except ValueError:
-            raise ValueError("The entry script must be inside of the snapshot root directory. "
-                             f"Snapshot root: {snapshot_root_directory}, entry script: {entry_script}")
+            raise ValueError(
+                "The entry script must be inside of the snapshot root directory. "
+                f"Snapshot root: {snapshot_root_directory}, entry script: {entry_script}"
+            )
     else:
         entry_script_relative = str(entry_script)
-    script_params = _get_script_params(script_params)
     print(f"This command will be run in AzureML: {entry_script_relative} {' '.join(script_params)}")
     return ScriptRunConfig(
-        source_directory=str(snapshot_root_directory),
-        script=entry_script_relative,
-        arguments=script_params)
-
-
-def _generate_input_dataset_command(input_datasets_v2: Dict[str, Input]) -> str:
-    """
-    Generate command line arguments to pass AML v2 data assets into a script
-
-    :param input_datasets_v2: A dictionary of Input objects that have been passed into the AML command
-    :return: A string representing the input datasets that the script should expect
-    """
-    input_cmd = ""
-    for i, (input_data_name, input_dataset_v2) in enumerate(input_datasets_v2.items()):
-        input_name = f"INPUT_{i}"
-        input_str = "${{inputs." + f"{input_name}" + "}}"
-        input_cmd += f" --{input_name}={input_str}"
-    return input_cmd
-
-
-def _generate_output_dataset_command(output_datasets_v2: Dict[str, Output]) -> str:
-    """
-    Generate command line arguments to pass AML v2 outputs into a script
-
-    :param output_datasets_v2: A dictionary of Output objects that have been passed into the AML command
-    :return: A string representing the output values that the script should expect
-    """
-    output_cmd = ""
-    for i, (output_data_name, output_dataset_v2) in enumerate(output_datasets_v2.items()):
-        output_name = f"OUTPUT_{i}"
-        output_str = "${{outputs." + f"{output_name}" + "}}"
-        output_cmd += f" --{output_name}={output_str}"
-    return output_cmd
-
-
-def submit_run_v2(workspace: Optional[Workspace],
-                  experiment_name: str,
-                  environment: EnvironmentV2,
-                  input_datasets_v2: Optional[Dict[str, Input]] = None,
-                  output_datasets_v2: Optional[Dict[str, Output]] = None,
-                  snapshot_root_directory: Optional[Path] = None,
-                  entry_script: Optional[PathOrString] = None,
-                  script_params: Optional[List[str]] = None,
-                  compute_target: Optional[str] = None,
-                  tags: Optional[Dict[str, str]] = None,
-                  wait_for_completion: bool = False,
-                  wait_for_completion_show_output: bool = False,
-                  workspace_config_path: Optional[PathOrString] = None,
-                  ml_client: Optional[MLClient] = None,
-                  hyperparam_args: Optional[Dict[str, Any]] = None) -> Job:
+        source_directory=str(snapshot_root_directory), script=entry_script_relative, arguments=script_params
+    )
+
+
+def effective_experiment_name(experiment_name: Optional[str], entry_script: Optional[PathOrString] = None) -> str:
+    """Choose the experiment name to use for the run. If provided in the environment variable HIML_EXPERIMENT_NAME,
+    then use that. Otherwise, use the argument `experiment_name`, or fall back to the default based on the
+    entry point script. If script in the form "foo/bar/baz.py", then the experiment name will be "baz". If the script is
+    of the form "-m foo.bar.baz", then the experiment name will be "foo_bar_baz".
+
+    :param experiment_name: The name of the AzureML experiment in which the run should be submitted.
+    :param entry_script: The script that should be run in AzureML.
+    :return: The effective experiment name to use, based on the fallback rules above.
+    """
+    value_from_env = os.environ.get(ENV_EXPERIMENT_NAME, "")
+    if value_from_env:
+        raw_value = value_from_env
+    elif experiment_name:
+        raw_value = experiment_name
+    elif entry_script is not None:
+        if str(entry_script)[:3] == "-m ":
+            raw_value = str(entry_script)[3:]
+        else:
+            raw_value = Path(entry_script).stem
+    else:
+        raise ValueError("No experiment name provided, and no entry script provided. ")
+    cleaned_value = to_azure_friendly_string(raw_value)
+    assert cleaned_value is not None, "Expecting an actual string"
+    return cleaned_value
+
+
+def submit_run_v2(
+    workspace: Optional[Workspace],
+    environment: EnvironmentV2,
+    experiment_name: Optional[str] = None,
+    input_datasets_v2: Optional[Dict[str, Input]] = None,
+    output_datasets_v2: Optional[Dict[str, Output]] = None,
+    snapshot_root_directory: Optional[Path] = None,
+    entry_script: Optional[PathOrString] = None,
+    script_params: Optional[List[str]] = None,
+    compute_target: Optional[str] = None,
+    tags: Optional[Dict[str, str]] = None,
+    docker_shm_size: str = "",
+    wait_for_completion: bool = False,
+    identity_based_auth: bool = False,
+    workspace_config_path: Optional[PathOrString] = None,
+    ml_client: Optional[MLClient] = None,
+    hyperparam_args: Optional[Dict[str, Any]] = None,
+    num_nodes: int = 1,
+    pytorch_processes_per_node: Optional[int] = None,
+    display_name: Optional[str] = None,
+) -> Job:
     """
     Starts a v2 AML Job on a given workspace by submitting a command
 
     :param workspace: The AzureML workspace to use.
+    :param environment: An AML v2 Environment object.
     :param experiment_name: The name of the experiment that will be used or created. If the experiment name contains
         characters that are not valid in Azure, those will be removed.
-    :param environment: An AML v2 Environment object.
     :param input_datasets_v2: An optional dictionary of Inputs to pass in to the command.
     :param output_datasets_v2: An optional dictionary of Outputs to pass in to the command.
     :param snapshot_root_directory: The directory that contains all code that should be packaged and sent to AzureML.
         All Python code that the script uses must be copied over.
     :param entry_script: The script that should be run in AzureML.
     :param script_params: A list of parameter to pass on to the script as it runs in AzureML.
     :param compute_target: Optional name of a compute target in Azure ML to submit the job to. If None, will run
         locally.
     :param tags: A dictionary of string key/value pairs, that will be added as metadata to the run. If set to None,
         a default metadata field will be added that only contains the commandline arguments that started the run.
+    :param docker_shm_size: The Docker shared memory size that should be used when creating a new Docker image.
     :param wait_for_completion: If False (the default) return after the run is submitted to AzureML, otherwise wait for
         the completion of this run (if True).
-    :param wait_for_completion_show_output: If wait_for_completion is True this parameter indicates whether to show the
-        run output on sys.stdout.
     :param workspace_config_path: If not provided with an AzureML Workspace, then load one given the information in this
         config
     :param ml_client: An Azure MLClient object for interacting with Azure resources.
     :param hyperparam_args: A dictionary of hyperparameter search args to pass into a sweep job.
+    :param num_nodes: The number of nodes to use for the job in AzureML. The value must be 1 or greater.
+    :param pytorch_processes_per_node: For plain PyTorch multi-GPU processing: The number of processes per node.
+        If supplied, it will run a command job with the "pytorch" framework (rather than "Python"), and using "nccl"
+        as the communication backend.
+    :param display_name: The name for the run that will be displayed in the AML UI. If not provided, a random
+        display name will be generated by AzureML.
     :return: An AzureML Run object.
     """
     if ml_client is None:
         if workspace is not None:
             ml_client = get_ml_client(
                 subscription_id=workspace.subscription_id,
                 resource_group=workspace.resource_group,
-                workspace_name=workspace.name
+                workspace_name=workspace.name,
             )
         elif workspace_config_path is not None:
             ml_client = get_ml_client(workspace_config_path=workspace_config_path)
         else:
             raise ValueError("Either workspace or workspace_config_path must be specified to connect to the Workspace")
 
     assert compute_target is not None, "No compute_target has been provided"
     assert entry_script is not None, "No entry_script has been provided"
     snapshot_root_directory = snapshot_root_directory or Path.cwd()
     root_dir = Path(snapshot_root_directory)
-    entry_script = Path(entry_script).relative_to(root_dir).as_posix()
 
-    script_params = script_params or []
-    args = [p for p in script_params if "conda_env" not in p]
-    arg_str = " ".join(args)
-    cmd = "python " + str(entry_script) + " " + arg_str
+    if str(entry_script)[:2] != "-m":
+        entry_script = Path(entry_script).relative_to(root_dir).as_posix()
 
-    if input_datasets_v2:
-        cmd += _generate_input_dataset_command(input_datasets_v2)
-    else:
-        input_datasets_v2 = {}
+    experiment_name = effective_experiment_name(experiment_name, entry_script)
 
-    if output_datasets_v2:
-        cmd += _generate_output_dataset_command(output_datasets_v2)
-    else:
-        output_datasets_v2 = {}
+    script_params = script_params or []
+    script_param_str = create_v2_job_command_line_args_from_params(script_params)
 
-    job_to_submit: Union[Command, Sweep]
+    cmd = " ".join(["python", str(entry_script), script_param_str])
 
-    if hyperparam_args:
-        param_sampling = hyperparam_args[PARAM_SAMPLING_ARG]
+    print(f"The following command will be run in AzureML: {cmd}")
 
-        for sample_param, choices in param_sampling.items():
-            input_datasets_v2[sample_param] = choices.values[0]
-            cmd += f" --{sample_param}=" + "${{inputs." + sample_param + "}}"
+    job_to_submit: Union[Command, Sweep]
 
-        command_job = command(
+    # number of nodes and processes per node cannot be less than one
+    if num_nodes < 1:
+        raise ValueError("num_nodes must be >= 1")
+    num_nodes = num_nodes if num_nodes >= 1 else 1
+    if pytorch_processes_per_node is not None:
+        if pytorch_processes_per_node < 1:
+            raise ValueError("pytorch_processes_per_node must be >= 1")
+
+    def create_command_job(cmd: str) -> Command:
+        if pytorch_processes_per_node is None:
+            # On AML managed compute, we can set distribution to None for single node jobs.
+            # However, on Kubernetes compute, single node jobs don't see any GPUs. GPUs are visible for MpiDistribution
+            # jobs, so we set MpiDistribution even for single node jobs.
+            distribution: Union[MpiDistribution, PyTorchDistribution] = MpiDistribution(process_count_per_instance=1)
+        else:
+            distribution = PyTorchDistribution(process_count_per_instance=pytorch_processes_per_node)
+        return command(
             code=str(snapshot_root_directory),
             command=cmd,
             inputs=input_datasets_v2,
             outputs=output_datasets_v2,
             environment=environment.name + "@latest",
             compute=compute_target,
             experiment_name=experiment_name,
-            environment_variables={
-                "JOB_EXECUTION_MODE": "Basic",
-            }
+            tags=tags or {},
+            shm_size=docker_shm_size,
+            display_name=display_name,
+            instance_count=num_nodes,
+            distribution=distribution,
+            identity=UserIdentityConfiguration() if identity_based_auth else None,
         )
 
+    if hyperparam_args:
+        param_sampling = hyperparam_args[PARAM_SAMPLING_ARG]
+
+        if input_datasets_v2 is None:
+            input_datasets_v2 = {}
+
+        for sample_param, choices in param_sampling.items():
+            input_datasets_v2[sample_param] = choices.values[0]
+            cmd += f" --{sample_param}=" + "${{inputs." + sample_param + "}}"
+
+        command_job = create_command_job(cmd)
+
         del hyperparam_args[PARAM_SAMPLING_ARG]
         # override command with parameter expressions
         command_job = command_job(
             **param_sampling,
         )
 
         job_to_submit = command_job.sweep(
             compute=compute_target,  # AML docs suggest setting this here although already passed to command
-            **hyperparam_args
+            **hyperparam_args,
         )
 
         # AML docs state to reset certain properties here which aren't picked up from the
         # underlying command such as experiment name and max_total_trials
         job_to_submit.experiment_name = experiment_name
         job_to_submit.set_limits(max_total_trials=hyperparam_args.get(MAX_TOTAL_TRIALS_ARG, None))
 
     else:
-        job_to_submit = command(
-            code=str(snapshot_root_directory),
-            command=cmd,
-            inputs=input_datasets_v2,
-            outputs=output_datasets_v2,
-            environment=environment.name + "@latest",
-            compute=compute_target,
-            experiment_name=experiment_name,
-            environment_variables={
-                "JOB_EXECUTION_MODE": "Basic",
-            }
-        )
+        job_to_submit = create_command_job(cmd)
 
     returned_job = ml_client.jobs.create_or_update(job_to_submit)
-    logging.info(f"URL to job: {returned_job.services['Studio'].endpoint}")  # type: ignore
+    print(f"URL to job: {returned_job.services['Studio'].endpoint}")  # type: ignore
+    if wait_for_completion:
+        print("Waiting for the completion of the AzureML job.")
+        wait_for_job_completion(ml_client, job_name=returned_job.name)
+        print("AzureML job completed.")
+        # After waiting, ensure that the caller gets the latest version job object
+        returned_job = ml_client.jobs.get(returned_job.name)
     return returned_job
 
 
-def download_job_outputs_logs(ml_client: MLClient,
-                              job_name: str,
-                              file_to_download_path: str = "",
-                              download_dir: Optional[PathOrString] = None) -> None:
+def download_job_outputs_logs(
+    ml_client: MLClient, job_name: str, file_to_download_path: str = "", download_dir: Optional[PathOrString] = None
+) -> None:
     """
     Download output files from an mlflow job. Outputs will be downloaded to a folder named
     `<download_dir>/<job_name>` where download_dir is either provided to this function,
     or is "outputs". If a single file is required, the path to this file within the job can
     be specified with 'file_to_download_path'
 
     :param ml_client: An MLClient object.
@@ -557,165 +615,195 @@
     """
 
     download_dir = Path(download_dir) if download_dir else Path("outputs")
     download_dir = download_dir / job_name
     ml_client.jobs.download(job_name, output_name=file_to_download_path, download_path=download_dir)
 
 
-def submit_run(workspace: Workspace,
-               experiment_name: str,
-               script_run_config: Union[ScriptRunConfig, HyperDriveConfig],
-               tags: Optional[Dict[str, str]] = None,
-               wait_for_completion: bool = False,
-               wait_for_completion_show_output: bool = False,
-               ) -> Run:
+def submit_run(
+    workspace: Workspace,
+    experiment_name: str,
+    script_run_config: Union[ScriptRunConfig, HyperDriveConfig],
+    tags: Optional[Dict[str, str]] = None,
+    wait_for_completion: bool = False,
+    wait_for_completion_show_output: bool = False,
+    display_name: Optional[str] = None,
+) -> Run:
     """
     Starts an AzureML run on a given workspace, via the script_run_config.
 
     :param workspace: The AzureML workspace to use.
     :param experiment_name: The name of the experiment that will be used or created. If the experiment name contains
         characters that are not valid in Azure, those will be removed.
     :param script_run_config: The settings that describe which script should be run.
     :param tags: A dictionary of string key/value pairs, that will be added as metadata to the run. If set to None,
         a default metadata field will be added that only contains the commandline arguments that started the run.
     :param wait_for_completion: If False (the default) return after the run is submitted to AzureML, otherwise wait for
         the completion of this run (if True).
     :param wait_for_completion_show_output: If wait_for_completion is True this parameter indicates whether to show the
         run output on sys.stdout.
+    :param display_name: The name for the run that will be displayed in the AML UI. If not provided, a random
+        display name will be generated by AzureML.
     :return: An AzureML Run object.
     """
     cleaned_experiment_name = to_azure_friendly_string(experiment_name)
     experiment = Experiment(workspace=workspace, name=cleaned_experiment_name)
     user_agent.append(SDK_NAME, SDK_VERSION)
     run = experiment.submit(script_run_config)
     if tags is None:
-        if hasattr(script_run_config, 'arguments') and \
-                script_run_config.arguments is not None:
+        if hasattr(script_run_config, 'arguments') and script_run_config.arguments is not None:
             # It is probably a ScriptRunConfig
             tags = {"commandline_args": " ".join(script_run_config.arguments)}
-        elif hasattr(script_run_config, 'run_config') and \
-                hasattr(script_run_config.run_config, 'arguments') and \
-                script_run_config.run_config.arguments is not None:
+        elif (
+            hasattr(script_run_config, 'run_config')
+            and hasattr(script_run_config.run_config, 'arguments')
+            and script_run_config.run_config.arguments is not None
+        ):
             # It is probably a HyperDriveConfig
             tags = {"commandline_args": " ".join(script_run_config.run_config.arguments)}
     run.set_tags(tags)
+    if display_name:
+        run.display_name = display_name
 
     _write_run_recovery_file(run)
 
     # These need to be 'print' not 'logging.info' so that the calling script sees them outside AzureML
     print("\n==============================================================================")
     print(f"Successfully queued run number {run.number} (ID {run.id}) in experiment {run.experiment.name}")
     print(f"Experiment name and run ID are available in file {RUN_RECOVERY_FILE}")
     print(f"Experiment URL: {run.experiment.get_portal_url()}")
     print(f"Run URL: {run.get_portal_url()}")
     print("==============================================================================\n")
     if wait_for_completion:
         print("Waiting for the completion of the AzureML run.")
-        run.wait_for_completion(show_output=wait_for_completion_show_output,
-                                wait_post_processing=True,
-                                raise_on_error=True)
+        run.wait_for_completion(
+            show_output=wait_for_completion_show_output, wait_post_processing=True, raise_on_error=True
+        )
         if not is_run_and_child_runs_completed(run):
-            raise ValueError(f"Run {run.id} in experiment {run.experiment.name} or one of its child "
-                             "runs failed.")
+            raise ValueError(f"Run {run.id} in experiment {run.experiment.name} or one of its child runs failed.")
         print("AzureML completed.")
     return run
 
 
 def _str_to_path(s: Optional[PathOrString]) -> Optional[Path]:
     if isinstance(s, str):
         return Path(s)
     return s
 
 
+def get_data_asset_from_config(ml_client: MLClient, dataset_config: DatasetConfig) -> Data:
+    """Given a list of dataset configs, generates and returns a list of data assets.
+
+    :param ml_client: An MLClient object.
+    :param dataset_list: The list of datasets to create data assets for.
+    :raises ValueError: Raised if a data asset has no path.
+    :return: A list of data assets.
+    """
+
+    version = dataset_config.version
+    logging.info(
+        f"Trying to access data asset {dataset_config.name} version {version}, datastore {dataset_config.datastore}"
+    )
+
+    # if version is None, this function gets the latest version
+    data_asset: Data = _get_or_create_v2_data_asset(
+        ml_client,
+        dataset_config.datastore,
+        dataset_config.name,
+        version=str(version) if version else None,
+    )
+    if not data_asset.path:
+        raise ValueError(f"Data asset {data_asset.id} has no path.")
+
+    return data_asset
+
+
 def create_v2_inputs(ml_client: MLClient, input_datasets: List[DatasetConfig]) -> Dict[str, Input]:
     """
     Create a dictionary of Azure ML v2 Input objects, required for passing input data in to an AML job
 
     :param ml_client: An MLClient object.
     :param input_datasets: A list of DatasetConfigs to convert to Inputs.
     :return: A dictionary in the format "input_name": Input.
     """
-    inputs: Dict[str, Input] = {}
-    for i, input_dataset in enumerate(input_datasets):
-        input_name = f"INPUT_{i}"
-        version = input_dataset.version or 1
-        data_asset: Data = ml_client.data.get(input_dataset.name, version=str(version))
-        data_path = data_asset.id or ""
-        # Note that there are alternative formats that the input path can take, such as:
-        # v1_datastore_path = f"azureml://datastores/{input_dataset.datastore}/paths/<path_to_dataset>"
-        # v2_dataset_path = f"azureml:{input_dataset.name}:1"
-
-        inputs[input_name] = Input(  # type: ignore
-            type=AssetTypes.URI_FOLDER,
-            path=data_path,
-            mode=InputOutputModes.MOUNT,
+    input_assets = [get_data_asset_from_config(ml_client, input_dataset) for input_dataset in input_datasets]
+    # Data assets can be of type "uri_folder", "uri_file", "mltable", all of which are value types in Input
+    return {
+        f"{V2_INPUT_ASSET_IDENTIFIER}{i}": Input(  # type: ignore
+            type=data_asset.type,  # type: ignore
+            path=data_asset.path,
+            mode=InputOutputModes.MOUNT if input_datasets[i].use_mounting else InputOutputModes.DOWNLOAD,
         )
-    return inputs
+        for i, data_asset in enumerate(input_assets)
+    }
 
 
-def create_v2_outputs(output_datasets: List[DatasetConfig]) -> Dict[str, Output]:
+def create_v2_outputs(ml_client: MLClient, output_datasets: List[DatasetConfig]) -> Dict[str, Output]:
     """
     Create a dictionary of Azure ML v2 Output objects, required for passing output data in to an AML job
 
+    :ml_client: An MLClient object.
     :param output_datasets: A list of DatasetConfigs to convert to Outputs.
     :return: A dictionary in the format "output_name": Output.
     """
-    outputs = {}
-    for i, output_dataset in enumerate(output_datasets):
-        output_name = f"OUTPUT_{i}"
-        v1_datastore_path = f"azureml://datastores/{output_dataset.datastore}/paths/{output_dataset.name}"
-        # Note that there are alternative formats that the output path can take, such as:
-        # v2_data_asset_path = f"azureml:{output_dataset.name}@latest"
-        outputs[output_name] = Output(  # type: ignore
-            type=AssetTypes.URI_FOLDER,
-            path=v1_datastore_path,
-            mode=InputOutputModes.DIRECT,
+
+    output_assets = [get_data_asset_from_config(ml_client, output_dataset) for output_dataset in output_datasets]
+    return {
+        # Data assets can be of type "uri_folder", "uri_file", "mltable", all of which are value types in Input
+        f"{V2_OUTPUT_ASSET_IDENTIFIER}{i}": Output(  # type: ignore
+            type=data_asset.type,  # type: ignore
+            path=data_asset.path,
+            mode=InputOutputModes.MOUNT,  # hard-coded to mount for now, as this is the only mode that doesn't break
         )
-    return outputs
+        for i, data_asset in enumerate(output_assets)
+    }
 
 
 def submit_to_azure_if_needed(  # type: ignore
-        compute_cluster_name: str = "",
-        entry_script: Optional[PathOrString] = None,
-        aml_workspace: Optional[Workspace] = None,
-        workspace_config_file: Optional[PathOrString] = None,
-        ml_client: Optional[MLClient] = None,
-        snapshot_root_directory: Optional[PathOrString] = None,
-        script_params: Optional[List[str]] = None,
-        conda_environment_file: Optional[PathOrString] = None,
-        aml_environment_name: str = "",
-        experiment_name: Optional[str] = None,
-        environment_variables: Optional[Dict[str, str]] = None,
-        pip_extra_index_url: str = "",
-        private_pip_wheel_path: Optional[PathOrString] = None,
-        docker_base_image: str = "",
-        docker_shm_size: str = "",
-        ignored_folders: Optional[List[PathOrString]] = None,
-        default_datastore: str = "",
-        input_datasets: Optional[List[StrOrDatasetConfig]] = None,
-        output_datasets: Optional[List[StrOrDatasetConfig]] = None,
-        num_nodes: int = 1,
-        wait_for_completion: bool = False,
-        wait_for_completion_show_output: bool = False,
-        max_run_duration: str = "",
-        submit_to_azureml: Optional[bool] = None,
-        tags: Optional[Dict[str, str]] = None,
-        after_submission: Optional[Callable[[Run], None]] = None,
-        hyperdrive_config: Optional[HyperDriveConfig] = None,
-        hyperparam_args: Optional[Dict[str, Any]] = None,
-        create_output_folders: bool = True,
-        strictly_aml_v1: bool = False,
+    compute_cluster_name: str = "",
+    entry_script: Optional[PathOrString] = None,
+    aml_workspace: Optional[Workspace] = None,
+    workspace_config_file: Optional[PathOrString] = None,
+    ml_client: Optional[MLClient] = None,
+    snapshot_root_directory: Optional[PathOrString] = None,
+    script_params: Optional[List[str]] = None,
+    conda_environment_file: Optional[PathOrString] = None,
+    aml_environment_name: str = "",
+    experiment_name: Optional[str] = None,
+    environment_variables: Optional[Dict[str, str]] = None,
+    pip_extra_index_url: str = "",
+    private_pip_wheel_path: Optional[PathOrString] = None,
+    docker_base_image: str = DEFAULT_DOCKER_BASE_IMAGE,
+    docker_shm_size: str = DEFAULT_DOCKER_SHM_SIZE,
+    ignored_folders: Optional[List[PathOrString]] = None,
+    default_datastore: str = "",
+    input_datasets: Optional[List[StrOrDatasetConfig]] = None,
+    output_datasets: Optional[List[StrOrDatasetConfig]] = None,
+    num_nodes: int = 1,
+    wait_for_completion: bool = False,
+    wait_for_completion_show_output: bool = False,
+    max_run_duration: str = "",
+    submit_to_azureml: Optional[bool] = None,
+    tags: Optional[Dict[str, str]] = None,
+    after_submission: Optional[Union[Callable[[Run], None], Callable[[Job, MLClient], None]]] = None,
+    hyperdrive_config: Optional[HyperDriveConfig] = None,
+    hyperparam_args: Optional[Dict[str, Any]] = None,
+    strictly_aml_v1: bool = False,
+    identity_based_auth: bool = False,
+    pytorch_processes_per_node_v2: Optional[int] = None,
+    display_name: Optional[str] = None,
 ) -> AzureRunInfo:  # pragma: no cover
     """
     Submit a folder to Azure, if needed and run it.
     Use the commandline flag --azureml to submit to AzureML, and leave it out to run locally.
 
-    :param after_submission: A function that will be called directly after submitting the job to AzureML. The only
-        argument to this function is the run that was just submitted. Use this to, for example, add additional tags
-        or print information about the run.
+    :param after_submission: A function that will be called directly after submitting the job to AzureML.
+        Use this to, for example, add additional tags or print information about the run.
+        When using AzureML SDK V1, the only argument to this function is the Run object that was just submitted.
+        When using AzureML SDK V2, the arguments are (Job, MLClient).
     :param tags: A dictionary of string key/value pairs, that will be added as metadata to the run. If set to None,
         a default metadata field will be added that only contains the commandline arguments that started the run.
     :param aml_environment_name: The name of an AzureML environment that should be used to submit the script. If not
         provided, an environment will be created from the arguments to this function.
     :param max_run_duration: The maximum runtime that is allowed for this job in AzureML. This is given as a
         floating point number with a string suffix s, m, h, d for seconds, minutes, hours, day. Examples: '3.5h', '2d'
     :param experiment_name: The name of the AzureML experiment in which the run should be submitted. If omitted,
@@ -729,109 +817,126 @@
         to pass it in as a parameter.
     :param workspace_config_file: The 2nd option is to specify the path to the config.json file downloaded from the
         Azure portal from which we can retrieve the existing Workspace.
     :param ml_client: An Azure MLClient object for interacting with Azure resources.
     :param snapshot_root_directory: The directory that contains all code that should be packaged and sent to AzureML.
         All Python code that the script uses must be copied over.
     :param ignored_folders: A list of folders to exclude from the snapshot when copying it to AzureML.
-    :param script_params: A list of parameter to pass on to the script as it runs in AzureML. If empty (or None, the
-        default) these will be copied over from sys.argv, omitting the --azureml flag.
+    :param script_params: A list of parameters to pass on to the script as it runs in AzureML. If `None` (the
+        default), these will be copied over from `sys.argv` (excluding the `--azureml` flag, if found).
     :param environment_variables: The environment variables that should be set when running in AzureML.
     :param docker_base_image: The Docker base image that should be used when creating a new Docker image.
+        The list of available images can be found here: https://github.com/Azure/AzureML-Containers
+        The default image is `mcr.microsoft.com/azureml/openmpi3.1.2-cuda10.2-cudnn8-ubuntu18.04`
     :param docker_shm_size: The Docker shared memory size that should be used when creating a new Docker image.
+        Default value is '100g'.
     :param pip_extra_index_url: If provided, use this PIP package index to find additional packages when building
         the Docker image.
     :param private_pip_wheel_path: If provided, add this wheel as a private package to the AzureML workspace.
     :param default_datastore: The data store in your AzureML workspace, that points to your training data in blob
         storage. This is described in more detail in the README.
     :param input_datasets: The script will consume all data in folder in blob storage as the input. The folder must
         exist in blob storage, in the location that you gave when creating the datastore. Once the script has run, it
         will also register the data in this folder as an AzureML dataset.
     :param output_datasets: The script will create a temporary folder when running in AzureML, and while the job writes
         data to that folder, upload it to blob storage, in the data store.
-    :param num_nodes: The number of nodes to use in distributed training on AzureML.
+    :param num_nodes: The number of nodes to use in distributed training on AzureML. When using a value > 1, multiple
+        nodes in AzureML will be started. If `pytorch_processes_per_node_v2=None`, the job will be submitted
+        as a multi-node MPI job, with 1 process per node. This is suitable for PyTorch Lightning jobs.
+        If `pytorch_processes_per_node_v2` is not None,
+        a job with framework "PyTorch" and communication backend "nccl" will be started.
+        `pytorch_processes_per_node_v2` will guide the number of processes per node. This is suitable for plain PyTorch
+        training jobs without the use of frameworks like PyTorch Lightning.
     :param wait_for_completion: If False (the default) return after the run is submitted to AzureML, otherwise wait for
         the completion of this run (if True).
     :param wait_for_completion_show_output: If wait_for_completion is True this parameter indicates whether to show the
         run output on sys.stdout.
     :param submit_to_azureml: If True, the codepath to create an AzureML run will be executed. If False, the codepath
         for local execution (i.e., return immediately) will be executed. If not provided (None), submission to AzureML
         will be triggered if the commandline flag '--azureml' is present in sys.argv
     :param hyperdrive_config: A configuration object for Hyperdrive (hyperparameter search).
-    :param create_output_folders: If True (default), create folders "outputs" and "logs" in the current working folder.
     :param strictly_aml_v1: If True, use Azure ML SDK v1. Otherwise, attempt to use Azure ML SDK v2.
+    :param pytorch_processes_per_node_v2: For plain PyTorch multi-GPU processing: The number of processes per node. This
+        is only supported with AML SDK v2, and ignored in v1. If supplied, the job will be submitted as using the
+        "pytorch" framework (rather than "Python"), and using "nccl" as the communication backend.
+    :param display_name: The name for the run that will be displayed in the AML UI. If not provided, a random
+        display name will be generated by AzureML.
     :return: If the script is submitted to AzureML then we terminate python as the script should be executed in AzureML,
         otherwise we return a AzureRunInfo object.
     """
-    _package_setup()
+    health_azure_package_setup()
     workspace_config_path = _str_to_path(workspace_config_file)
     snapshot_root_directory = _str_to_path(snapshot_root_directory)
-    cleaned_input_datasets = _replace_string_datasets(input_datasets or [],
-                                                      default_datastore_name=default_datastore)
-    cleaned_output_datasets = _replace_string_datasets(output_datasets or [],
-                                                       default_datastore_name=default_datastore)
+    cleaned_input_datasets = _replace_string_datasets(input_datasets or [], default_datastore_name=default_datastore)
+    cleaned_output_datasets = _replace_string_datasets(output_datasets or [], default_datastore_name=default_datastore)
 
     # The present function will most likely be called from the script once it is running in AzureML.
     # The '--azureml' flag will not be present anymore, but we don't want to rely on that. From Run.get_context we
     # can infer if the present code is running in AzureML.
     in_azure = is_running_in_azure_ml(RUN_CONTEXT)
     if in_azure:
         if strictly_aml_v1:
             return _generate_azure_datasets(cleaned_input_datasets, cleaned_output_datasets)
         else:
             return _generate_v2_azure_datasets(cleaned_input_datasets, cleaned_output_datasets)
     # This codepath is reached when executing outside AzureML. Here we first check if a script submission to AzureML
     # is necessary. If not, return to the caller for local execution.
+    if submit_to_azureml is None:
+        submit_to_azureml = AZUREML_FLAG in sys.argv[1:]
     if not submit_to_azureml:
         # Set the environment variables for local execution.
-        environment_variables = {
-            **DEFAULT_ENVIRONMENT_VARIABLES,
-            **(environment_variables or {})
-        }
+        environment_variables = {**DEFAULT_ENVIRONMENT_VARIABLES, **(environment_variables or {})}
 
         for k, v in environment_variables.items():
             os.environ[k] = v
 
         output_folder = Path.cwd() / OUTPUT_FOLDER
         output_folder.mkdir(exist_ok=True)
 
         logs_folder = Path.cwd() / LOGS_FOLDER
         logs_folder.mkdir(exist_ok=True)
 
-        mounted_input_datasets, mount_contexts = setup_local_datasets(cleaned_input_datasets,
-                                                                      strictly_aml_v1,
-                                                                      aml_workspace=aml_workspace,
-                                                                      ml_client=ml_client,
-                                                                      workspace_config_path=workspace_config_path)
+        mounted_input_datasets, mount_contexts = setup_local_datasets(
+            cleaned_input_datasets,
+            strictly_aml_v1,
+            aml_workspace=aml_workspace,
+            ml_client=ml_client,
+            workspace_config_path=workspace_config_path,
+        )
 
         return AzureRunInfo(
             input_datasets=mounted_input_datasets,
             output_datasets=[d.local_folder for d in cleaned_output_datasets],
             mount_contexts=mount_contexts,
             run=None,
             is_running_in_azure_ml=False,
             output_folder=output_folder,
-            logs_folder=logs_folder
+            logs_folder=logs_folder,
         )
 
     if snapshot_root_directory is None:
         print(f"No snapshot root directory given. Uploading all files in the current directory {Path.cwd()}")
         snapshot_root_directory = Path.cwd()
 
     workspace = get_workspace(aml_workspace, workspace_config_path)
-    ml_client = get_ml_client(ml_client=ml_client, aml_workspace=workspace)
     print(f"Loaded AzureML workspace {workspace.name}")
 
     if conda_environment_file is None:
         conda_environment_file = find_file_in_parent_to_pythonpath(CONDA_ENVIRONMENT_FILE)
+        if conda_environment_file is None:
+            raise ValueError(
+                f"No conda environment file {CONDA_ENVIRONMENT_FILE} found in {Path.cwd()} or any parent directory."
+            )
         print(f"Using the Conda environment from this file: {conda_environment_file}")
     conda_environment_file = _str_to_path(conda_environment_file)
 
     amlignore_path = snapshot_root_directory / AML_IGNORE_FILE
     lines_to_append = [str(path) for path in (ignored_folders or [])]
+    script_params = _get_script_params(script_params)
+
     with append_to_amlignore(amlignore=amlignore_path, lines_to_append=lines_to_append):
         if strictly_aml_v1:
             run_config = create_run_configuration(
                 workspace=workspace,
                 compute_cluster_name=compute_cluster_name,
                 aml_environment_name=aml_environment_name,
                 conda_environment_file=conda_environment_file,
@@ -841,66 +946,76 @@
                 docker_base_image=docker_base_image,
                 docker_shm_size=docker_shm_size,
                 num_nodes=num_nodes,
                 max_run_duration=max_run_duration,
                 input_datasets=cleaned_input_datasets,
                 output_datasets=cleaned_output_datasets,
             )
-            script_run_config = create_script_run(snapshot_root_directory=snapshot_root_directory,
-                                                  entry_script=entry_script,
-                                                  script_params=script_params)
+
+            script_run_config = create_script_run(
+                script_params=script_params,
+                snapshot_root_directory=snapshot_root_directory,
+                entry_script=entry_script,
+            )
             script_run_config.run_config = run_config
 
             if hyperdrive_config:
                 config_to_submit: Union[ScriptRunConfig, HyperDriveConfig] = hyperdrive_config
                 config_to_submit._run_config = script_run_config
             else:
                 config_to_submit = script_run_config
 
-            effective_experiment_name = experiment_name or Path(script_run_config.script).stem
-
-            run = submit_run(workspace=workspace,
-                             experiment_name=effective_experiment_name,
-                             script_run_config=config_to_submit,
-                             tags=tags,
-                             wait_for_completion=wait_for_completion,
-                             wait_for_completion_show_output=wait_for_completion_show_output)
+            run = submit_run(
+                workspace=workspace,
+                experiment_name=effective_experiment_name(experiment_name, script_run_config.script),
+                script_run_config=config_to_submit,
+                tags=tags,
+                display_name=display_name,
+                wait_for_completion=wait_for_completion,
+                wait_for_completion_show_output=wait_for_completion_show_output,
+            )
+            if after_submission is not None:
+                after_submission(run)  # type: ignore
         else:
-
-            assert conda_environment_file is not None
+            if conda_environment_file is None:
+                raise ValueError("Argument 'conda_environment_file' must be specified when using AzureML v2")
             environment = create_python_environment_v2(
-                conda_environment_file=conda_environment_file,
-                docker_base_image=docker_base_image
+                conda_environment_file=conda_environment_file, docker_base_image=docker_base_image
             )
             if entry_script is None:
                 entry_script = Path(sys.argv[0])
-            script_params = script_params or sys.argv[1:]
-            effective_experiment_name = experiment_name or Path(entry_script).stem
 
+            ml_client = get_ml_client(ml_client=ml_client, aml_workspace=workspace)
             registered_env = register_environment_v2(environment, ml_client)
             input_datasets_v2 = create_v2_inputs(ml_client, cleaned_input_datasets)
-            output_datasets_v2 = create_v2_outputs(cleaned_output_datasets)
+            output_datasets_v2 = create_v2_outputs(ml_client, cleaned_output_datasets)
+
+            job = submit_run_v2(
+                workspace=workspace,
+                input_datasets_v2=input_datasets_v2,
+                output_datasets_v2=output_datasets_v2,
+                experiment_name=experiment_name,
+                environment=registered_env,
+                snapshot_root_directory=snapshot_root_directory,
+                entry_script=entry_script,
+                script_params=script_params,
+                compute_target=compute_cluster_name,
+                tags=tags,
+                display_name=display_name,
+                docker_shm_size=docker_shm_size,
+                wait_for_completion=wait_for_completion,
+                identity_based_auth=identity_based_auth,
+                hyperparam_args=hyperparam_args,
+                num_nodes=num_nodes,
+                pytorch_processes_per_node=pytorch_processes_per_node_v2,
+            )
 
-            run = submit_run_v2(workspace=workspace,
-                                input_datasets_v2=input_datasets_v2,
-                                output_datasets_v2=output_datasets_v2,
-                                experiment_name=effective_experiment_name,
-                                environment=registered_env,
-                                snapshot_root_directory=snapshot_root_directory,
-                                entry_script=entry_script,
-                                script_params=script_params,
-                                compute_target=compute_cluster_name,
-                                tags=tags,
-                                wait_for_completion=wait_for_completion,
-                                wait_for_completion_show_output=wait_for_completion_show_output,
-                                hyperparam_args=hyperparam_args
-                                )
+            if after_submission is not None:
+                after_submission(job, ml_client)  # type: ignore
 
-    if after_submission is not None and strictly_aml_v1:
-        after_submission(run)
     exit(0)
 
 
 def _write_run_recovery_file(run: Run) -> None:
     """
     Write the run recovery file
 
@@ -913,15 +1028,15 @@
     recovery_file.write_text(recovery_id)
 
 
 def convert_himl_to_azureml_datasets(
     cleaned_input_datasets: List[DatasetConfig],
     cleaned_output_datasets: List[DatasetConfig],
     workspace: Workspace,
-    strictly_aml_v1: bool
+    strictly_aml_v1: bool,
 ) -> Tuple[Dict[str, DatasetConsumptionConfig], Dict[str, OutputFileDatasetConfig]]:
     """
     Convert the cleaned input and output datasets into dictionaries of DatasetConsumptionConfigs for use in AzureML.
 
     :param cleaned_input_datasets: The list of input DatasetConfigs
     :param cleaned_output_datasets: The list of output DatasetConfigs
     :param workspace: The AzureML workspace
@@ -953,100 +1068,114 @@
 def _get_script_params(script_params: Optional[List[str]] = None) -> List[str]:
     """
     If script parameters are given then return them, otherwise derive them from sys.argv
 
     :param script_params: The optional script parameters
     :return: The given script parameters or ones derived from sys.argv
     """
-    if script_params:
+    if script_params is None:
+        return [p for p in sys.argv[1:] if p != AZUREML_FLAG]
+    else:
         return script_params
-    return [p for p in sys.argv[1:] if p != AZUREML_COMMANDLINE_FLAG]
 
 
 def _generate_azure_datasets(
-        cleaned_input_datasets: List[DatasetConfig],
-        cleaned_output_datasets: List[DatasetConfig]) -> AzureRunInfo:
+    cleaned_input_datasets: List[DatasetConfig], cleaned_output_datasets: List[DatasetConfig]
+) -> AzureRunInfo:
     """
     Generate returned datasets when running in AzureML.
 
     :param cleaned_input_datasets: The list of input dataset configs
     :param cleaned_output_datasets: The list of output dataset configs
     :return: The AzureRunInfo containing the AzureML input and output dataset lists etc.
     """
     if is_amulet_job():
         input_data_mount_folder = Path(os.environ[ENV_AMLT_DATAREFERENCE_DATA])
         logging.info(f"Path to mounted data: {ENV_AMLT_DATAREFERENCE_DATA}: {str(input_data_mount_folder)}")
-        returned_input_datasets = [input_data_mount_folder / input_dataset.name for input_dataset in
-                                   cleaned_input_datasets]
+        returned_input_datasets = [
+            input_data_mount_folder / input_dataset.name for input_dataset in cleaned_input_datasets
+        ]
 
         output_data_mount_folder = Path(os.environ[ENV_AMLT_DATAREFERENCE_OUTPUT])
         logging.info(f"Path to output datasets: {output_data_mount_folder}")
-        returned_output_datasets = [output_data_mount_folder / output_dataset.name for output_dataset in
-                                    cleaned_output_datasets]
+        returned_output_datasets = [
+            output_data_mount_folder / output_dataset.name for output_dataset in cleaned_output_datasets
+        ]
         logging.info(f"Stitched returned input datasets: {returned_input_datasets}")
         logging.info(f"Stitched returned output datasets: {returned_output_datasets}")
     else:
-        returned_input_datasets = [Path(RUN_CONTEXT.input_datasets[_input_dataset_key(index)])
-                                   for index in range(len(cleaned_input_datasets))]
-        returned_output_datasets = [Path(RUN_CONTEXT.output_datasets[_output_dataset_key(index)])
-                                    for index in range(len(cleaned_output_datasets))]
+        returned_input_datasets = [
+            Path(RUN_CONTEXT.input_datasets[_input_dataset_key(index)]) for index in range(len(cleaned_input_datasets))
+        ]
+        returned_output_datasets = [
+            Path(RUN_CONTEXT.output_datasets[_output_dataset_key(index)])
+            for index in range(len(cleaned_output_datasets))
+        ]
     return AzureRunInfo(
         input_datasets=returned_input_datasets,  # type: ignore
         output_datasets=returned_output_datasets,  # type: ignore
         mount_contexts=[],
         run=RUN_CONTEXT,
         is_running_in_azure_ml=True,
         output_folder=Path.cwd() / OUTPUT_FOLDER,
-        logs_folder=Path.cwd() / LOGS_FOLDER)
+        logs_folder=Path.cwd() / LOGS_FOLDER,
+    )
 
 
 def _get_dataset_names_from_string(sys_arg: str, pattern: str) -> Path:
     dataset_string = re.split(pattern, sys_arg)[-1]
     dataset_path = Path(dataset_string)
     return dataset_path
 
 
-def _extract_v2_inputs_outputs_from_args() -> Tuple[List[Path], List[Path]]:
-    """
-    Extract all command line arguments of the format INPUT_i=path_to_input or OUTPUT_i=path_to_output (where i is any
-    integer) and return a list of the Paths for each.
+def _extract_v2_data_asset_from_env_vars(asset_num: int, asset_type_identifier: str) -> Path:
+    """Provides path to the given data assets for v2 jobs by extracting it from the environment variables.
 
-    :return: A list of Input paths and a list of Output paths
+    :param asset_num: The id number of the data asset to extract
+    :param asset_type_identifier: The pattern to match the environment variables against, must be "INPUT_" or "OUTPUT_"
+    :return: The path to the data asset
     """
-    returned_input_datasets: List[Path] = []
-    returned_output_datasets: List[Path] = []
 
-    for sys_arg in sys.argv:
-        if re.match(V2_INPUT_DATASET_PATTERN, sys_arg):
-            returned_input_datasets += [_get_dataset_names_from_string(sys_arg, V2_INPUT_DATASET_PATTERN)]
-        if re.match(V2_OUTPUT_DATASET_PATTERN, sys_arg):
-            returned_output_datasets += [_get_dataset_names_from_string(sys_arg, V2_OUTPUT_DATASET_PATTERN)]
-    return returned_input_datasets, returned_output_datasets
+    asset_environment_variable = f"AZURE_ML_{asset_type_identifier}{asset_type_identifier}{asset_num}"
+    asset_path_str = os.environ.get(asset_environment_variable)
+    if asset_path_str is None:
+        raise ValueError(
+            f"Cannot find {asset_environment_variable} in environment variables, cannot retrieve data asset path."
+        )
 
+    return Path(asset_path_str)
 
-def _generate_v2_azure_datasets(cleaned_input_datasets: List[DatasetConfig],
-                                cleaned_output_datasets: List[DatasetConfig]) -> AzureRunInfo:
+
+def _generate_v2_azure_datasets(
+    cleaned_input_datasets: List[DatasetConfig], cleaned_output_datasets: List[DatasetConfig]
+) -> AzureRunInfo:
     """
     Generate returned datasets when running in AzureML. Assumes this is v2 Job, so we need to get
     the input datasets from the command line args
 
     :param cleaned_input_datasets: The list of input dataset configs
     :param cleaned_output_datasets: The list of output dataset configs
     :return: The AzureRunInfo containing the AzureML input and output dataset lists etc.
     """
-    returned_input_datasets, returned_output_datasets = _extract_v2_inputs_outputs_from_args()
+    returned_input_datasets = [
+        _extract_v2_data_asset_from_env_vars(i, V2_INPUT_ASSET_IDENTIFIER) for i in range(len(cleaned_input_datasets))
+    ]
+    returned_output_datasets = [
+        _extract_v2_data_asset_from_env_vars(i, V2_OUTPUT_ASSET_IDENTIFIER) for i in range(len(cleaned_output_datasets))
+    ]
 
     return AzureRunInfo(
         input_datasets=returned_input_datasets,  # type: ignore
         output_datasets=returned_output_datasets,  # type: ignore
         mount_contexts=[],
         run=RUN_CONTEXT,
         is_running_in_azure_ml=True,
         output_folder=Path.cwd() / OUTPUT_FOLDER,
-        logs_folder=Path.cwd() / LOGS_FOLDER)
+        logs_folder=Path.cwd() / LOGS_FOLDER,
+    )
 
 
 @contextmanager
 def append_to_amlignore(lines_to_append: List[str], amlignore: Optional[Path] = None) -> Generator:
     """
     Context manager that appends lines to the .amlignore file, and reverts to the previous contents after leaving
     the context.
@@ -1067,45 +1196,25 @@
     yield
     if amlignore_exists_already:
         amlignore.write_text(old_contents)
     elif new_text:
         amlignore.unlink()
 
 
-def _package_setup() -> None:
-    """
-    Set up the Python packages where needed. In particular, reduce the logging level for some of the used
-    libraries, which are particularly talkative in DEBUG mode. Usually when running in DEBUG mode, we want
-    diagnostics about the model building itself, but not for the underlying libraries.
-    It also adds workarounds for known issues in some packages.
-    """
-    # The adal package creates a logging.info line each time it gets an authentication token, avoid that.
-    logging.getLogger('adal-python').setLevel(logging.WARNING)
-    # Azure core prints full HTTP requests even in INFO mode
-    logging.getLogger('azure').setLevel(logging.WARNING)
-    # PyJWT prints out warnings that are beyond our control
-    warnings.filterwarnings("ignore", category=DeprecationWarning, module="jwt")
-    # Urllib3 prints out connection information for each call to write metrics, etc
-    logging.getLogger('urllib3').setLevel(logging.INFO)
-    logging.getLogger('msrest').setLevel(logging.INFO)
-    # AzureML prints too many details about logging metrics
-    logging.getLogger('azureml').setLevel(logging.INFO)
-
-
 def main() -> None:
     """
     Handle submit_to_azure if called from the command line.
     """
     parser = ArgumentParser()
     parser.add_argument("-p", "--workspace_config_file", type=str, required=False, help="AzureML workspace config file")
     parser.add_argument("-c", "--compute_cluster_name", type=str, required=True, help="AzureML cluster name")
-    parser.add_argument("-y", "--snapshot_root_directory", type=str, required=True,
-                        help="Root of snapshot to upload to AzureML")
-    parser.add_argument("-t", "--entry_script", type=str, required=True,
-                        help="The script to run in AzureML")
+    parser.add_argument(
+        "-y", "--snapshot_root_directory", type=str, required=True, help="Root of snapshot to upload to AzureML"
+    )
+    parser.add_argument("-t", "--entry_script", type=str, required=True, help="The script to run in AzureML")
     parser.add_argument("-d", "--conda_environment_file", type=str, required=True, help="The environment to use")
 
     args = parser.parse_args()
 
     submit_to_azure_if_needed(
         workspace_config_file=Path(args.workspace_config_file),
         compute_cluster_name=args.compute_cluster_name,
```

### Comparing `hi-ml-azure-0.2.9/src/health_azure/himl_download.py` & `hi-ml-azure-0.3.0/src/health_azure/himl_download.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,44 +2,52 @@
 #  ------------------------------------------------------------------------------------------
 #  Copyright (c) Microsoft Corporation. All rights reserved.
 #  Licensed under the MIT License (MIT). See LICENSE in the repo root for license information.
 #  ------------------------------------------------------------------------------------------
 import param
 import sys
 from pathlib import Path
-import health_azure.utils as azure_util
+from health_azure.argparsing import parse_args_and_update_config
 from health_azure.himl import download_job_outputs_logs
+from health_azure.utils import AmlRunScriptConfig, get_ml_client, get_workspace
 
 
-class HimlDownloadConfig(azure_util.AmlRunScriptConfig):
-    output_dir: Path = param.ClassSelector(class_=Path, default=Path("outputs"), instantiate=False,
-                                           doc="Path to directory to store files downloaded from the AML Run")
-    config_file: Path = param.ClassSelector(class_=Path, default=None, instantiate=False,
-                                            doc="Path to config.json where Workspace name is defined. If not provided, "
-                                                "the code will try to locate a config.json file in any of the parent "
-                                                "folders of the current working directory")
+class HimlDownloadConfig(AmlRunScriptConfig):
+    output_dir: Path = param.ClassSelector(
+        class_=Path,
+        default=Path("outputs"),
+        instantiate=False,
+        doc="Path to directory to store files downloaded from the AML Run",
+    )
+    config_file: Path = param.ClassSelector(
+        class_=Path,
+        default=None,
+        instantiate=False,
+        doc="Path to config.json where Workspace name is defined. If not provided, "
+        "the code will try to locate a config.json file in any of the parent "
+        "folders of the current working directory",
+    )
 
     files_to_download: str = param.String(default=None, allow_None=True, doc="Path to the file to download")
 
 
 def main() -> None:  # pragma: no cover
-
     download_config = HimlDownloadConfig()
-    download_config = azure_util.parse_args_and_update_config(download_config, sys.argv[1:])
+    download_config = parse_args_and_update_config(download_config, sys.argv[1:])
 
     output_dir = download_config.output_dir
     output_dir.mkdir(exist_ok=True)
 
     files_to_download = download_config.files_to_download
 
-    workspace = azure_util.get_workspace()
-    ml_client = azure_util.get_ml_client(
+    workspace = get_workspace()
+    ml_client = get_ml_client(
         subscription_id=workspace.subscription_id,
         resource_group=workspace.resource_group,
-        workspace_name=workspace.name
+        workspace_name=workspace.name,
     )
     for run_id in download_config.run:
         download_job_outputs_logs(ml_client, run_id, file_to_download_path=files_to_download, download_dir=output_dir)
         print("Successfully downloaded output and log files")
 
 
 if __name__ == "__main__":  # pragma: no cover
```

### Comparing `hi-ml-azure-0.2.9/src/health_azure/himl_tensorboard.py` & `hi-ml-azure-0.3.0/src/health_azure/himl_tensorboard.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,32 +13,35 @@
 from subprocess import PIPE, Popen
 from threading import Event
 from typing import Any, Optional
 
 from azureml._run_impl.run_watcher import RunWatcher
 from azureml.tensorboard import Tensorboard
 
-from health_azure import utils as azure_util
+from health_azure.argparsing import parse_args_and_update_config
 from health_azure.himl import get_workspace
+from health_azure.utils import AmlRunScriptConfig, _get_runs_from_script_config
 
 
 ROOT_DIR = Path.cwd()
 OUTPUT_DIR = ROOT_DIR / "outputs"
 TENSORBOARD_DIR = ROOT_DIR / "tensorboard_logs"
 
 
-class HimlTensorboardConfig(azure_util.AmlRunScriptConfig):
-    log_dir: Path = param.ClassSelector(class_=Path, default=Path("outputs"), instantiate=False,
-                                        doc="Path to directory in which Tensorboard  files"
-                                            "(summarywriter and TB logs) are stored")
+class HimlTensorboardConfig(AmlRunScriptConfig):
+    log_dir: Path = param.ClassSelector(
+        class_=Path,
+        default=Path("outputs"),
+        instantiate=False,
+        doc="Path to directory in which Tensorboard  files (summarywriter and TB logs) are stored",
+    )
     port: int = param.Integer(default=6006, doc="The port to run Tensorboard on")
 
 
 class WrappedTensorboard(Tensorboard):
-
     def __init__(self, remote_root: str, **kwargs: Any) -> None:
         super().__init__(**kwargs)
         self.remote_root = remote_root
 
     def start(self) -> Optional[str]:
         """
         Start the Tensorboard instance, and begin processing logs.
@@ -62,83 +65,82 @@
             local_log_dirs.append(f"{run.id}:{run_local_root}")
             run_watcher = RunWatcher(
                 run,
                 local_root=run_local_root,
                 remote_root=self.remote_root,
                 executor=self._executor,
                 event=self._event,
-                session=self._session)
+                session=self._session,
+            )
             self._run_watchers.append(run_watcher)
 
         for w in self._run_watchers:
             self._executor.submit(w.refresh_requeue)  # type: ignore
 
         # We use sys.executable here to ensure that we can import modules from the same environment
         # as the current process.
         # (using just "python" results in the global environment, which might not have a Tensorboard module)
         # sometimes, sys.executable might not give us what we want (i.e. in a notebook), and then we just have to hope
         # that "python" will give us something useful
         python_binary = sys.executable or "python"
-        python_command = [
-            python_binary, "-m", "tensorboard.main",
-            "--port", str(self._port)
-        ]
+        python_command = [python_binary, "-m", "tensorboard.main", "--port", str(self._port)]
         if len(local_log_dirs) > 1:
             # logdir_spec is not recommended but it is the only working way to display multiple dirs
             logdir_str = ','.join(local_log_dirs)
             python_command.append("--logdir_spec")
-            logging.info("Loading tensorboard files for > 1 run. You may notice reduced functionality as noted "
-                         "here: https://github.com/tensorflow/tensorboard#logdir--logdir_spec-legacy-mode ")
+            logging.info(
+                "Loading tensorboard files for > 1 run. You may notice reduced functionality as noted "
+                "here: https://github.com/tensorflow/tensorboard#logdir--logdir_spec-legacy-mode "
+            )
         else:
             logdir_str = run_local_root
             python_command.append("--logdir")
 
         python_command.append(logdir_str)
 
-        self._tb_proc = Popen(
-            python_command,
-            stderr=PIPE, stdout=PIPE, universal_newlines=True)
+        self._tb_proc = Popen(python_command, stderr=PIPE, stdout=PIPE, universal_newlines=True)
         if os.name == "nt":
             self._win32_kill_subprocess_on_exit(self._tb_proc)
 
         url = self._wait_for_url()
         # in notebooks, this shows as a clickable link (whereas the returned value is not parsed in output)
         logging.info(f"Tensorboard running at: {url}")
 
         return url
 
 
 def main() -> None:  # pragma: no cover
     tb_config = HimlTensorboardConfig()
-    tb_config = azure_util.parse_args_and_update_config(tb_config, sys.argv[1:])
+    tb_config = parse_args_and_update_config(tb_config, sys.argv[1:])
 
     config_path = tb_config.config_file
 
     if not config_path:
-        logging.info("You have not provided a config path. Therefore we will try to find one in your "
-                     "current directory, and its parents")
+        logging.info(
+            "You have not provided a config path. Therefore we will try to find one in your "
+            "current directory, and its parents"
+        )
 
     workspace = get_workspace(aml_workspace=None, workspace_config_path=config_path)
 
-    runs = azure_util._get_runs_from_script_config(tb_config, workspace)
+    runs = _get_runs_from_script_config(tb_config, workspace)
 
     print(f"Runs:\n{runs}")
     if len(runs) == 0:
         raise ValueError("No runs were found")
 
     local_logs_dir = ROOT_DIR / tb_config.log_dir
     logging.info(f"Creating directory {local_logs_dir} to store TensorBoard logs in")
     local_logs_dir.mkdir(exist_ok=True, parents=True)
 
     remote_logs_dir = local_logs_dir.relative_to(ROOT_DIR)
 
-    ts = WrappedTensorboard(remote_root=str(remote_logs_dir) + '/',
-                            runs=runs,
-                            local_root=str(local_logs_dir),
-                            port='6006')
+    ts = WrappedTensorboard(
+        remote_root=str(remote_logs_dir) + '/', runs=runs, local_root=str(local_logs_dir), port='6006'
+    )
 
     ts.start()
     print("=============================================================================\n\n")
     input("Press Enter to close TensorBoard...")
     ts.stop()
```

### Comparing `hi-ml-azure-0.2.9/src/health_azure/logging.py` & `hi-ml-azure-0.3.0/src/health_azure/logging.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,18 +1,20 @@
 #  -------------------------------------------------------------------------------------------
 #  Copyright (c) Microsoft Corporation. All rights reserved.
 #  Licensed under the MIT License (MIT). See LICENSE in the repo root for license information.
 #  -------------------------------------------------------------------------------------------
+import datetime
 import logging
+import os
 import sys
 import time
 from contextlib import contextmanager
 from typing import Generator, Optional, Union
 
-from health_azure.utils import check_is_any_of
+from health_azure.utils import ENV_LOCAL_RANK, check_is_any_of, is_global_rank_zero
 
 logging_stdout_handler: Optional[logging.StreamHandler] = None
 logging_to_file_handler: Optional[logging.StreamHandler] = None
 
 
 def logging_to_stdout(log_level: Union[int, str] = logging.INFO) -> None:
     """
@@ -25,22 +27,24 @@
     log_level = standardize_log_level(log_level)
     logger = logging.getLogger()
     # This function can be called multiple times, in particular in AzureML when we first run a training job and
     # then a couple of tests, which also often enable logging. This would then add multiple handlers, and repeated
     # logging lines.
     global logging_stdout_handler
     if not logging_stdout_handler:
-        print("Setting up logging to stdout.")
+        if is_global_rank_zero():
+            print("Setting up logging to stdout.")
         # At startup, logging has one handler set, that writes to stderr, with a log level of 0 (logging.NOTSET)
         if len(logger.handlers) == 1:
             logger.removeHandler(logger.handlers[0])
         logging_stdout_handler = logging.StreamHandler(stream=sys.stdout)
         _add_formatter(logging_stdout_handler)
         logger.addHandler(logging_stdout_handler)
-    print(f"Setting logging level to {log_level}")
+    if is_global_rank_zero():
+        print(f"Setting logging level to {log_level}")
     logging_stdout_handler.setLevel(log_level)
     logger.setLevel(log_level)
 
 
 def standardize_log_level(log_level: Union[int, str]) -> int:
     """
 
@@ -60,14 +64,31 @@
     """
     formatter = logging.Formatter(fmt="%(asctime)s %(levelname)-8s %(message)s", datefmt="%Y-%m-%dT%H:%M:%SZ")
     # noinspection PyTypeHints
     formatter.converter = time.gmtime  # type: ignore
     handler.setFormatter(formatter)
 
 
+def format_time_from_seconds(time_in_seconds: float) -> str:
+    """Formats a time in seconds as a string, e.g. 1.5 hours, 2.5 minutes, 3.5 seconds.
+
+    :param time_in_seconds: time in seconds.
+    :return: string expressing the time. If the time is more than an hour, it is expressed in hours, to 2 decimal
+        places. If the time is more than a minute, it is expressed in minutes, to 2 decimal places. Otherwise, it is
+        rounded to 2 decimal places and expressed in seconds.
+    """
+    if time_in_seconds >= 3600:
+        time_expr = f"{time_in_seconds / 3600:0.2f} hours"
+    elif time_in_seconds >= 60:
+        time_expr = f"{time_in_seconds / 60:0.2f} minutes"
+    else:
+        time_expr = f"{time_in_seconds:0.2f} seconds"
+    return time_expr
+
+
 @contextmanager
 def logging_section(gerund: str) -> Generator:
     """
     Context manager to print "**** STARTING: ..." and "**** FINISHED: ..." lines around sections of the log,
     to help people locate particular sections. Usage:
     with logging_section("doing this and that"):
        do_this_and_that()
@@ -80,16 +101,34 @@
     msg = f"**** STARTING: {gerund} "
     logging.info(msg + (100 - len(msg)) * "*")
     logging.info("")
     start_time = time()
     yield
     elapsed = time() - start_time
     logging.info("")
-    if elapsed >= 3600:
-        time_expr = f"{elapsed / 3600:0.2f} hours"
-    elif elapsed >= 60:
-        time_expr = f"{elapsed / 60:0.2f} minutes"
-    else:
-        time_expr = f"{elapsed:0.2f} seconds"
+    time_expr = format_time_from_seconds(elapsed)
     msg = f"**** FINISHED: {gerund} after {time_expr} "
     logging.info(msg + (100 - len(msg)) * "*")
     logging.info("")
+
+
+def print_message_with_rank_pid(message: str = '', level: str = 'DEBUG') -> None:
+    """Prints a message with the rank and PID of the current process.
+
+    :param message: message to print.
+    :param level: logging level to use.
+    """
+    print(f"{datetime.datetime.utcnow()} {level}    Rank {os.getenv(ENV_LOCAL_RANK)} - PID {os.getpid()} - {message}")
+
+
+@contextmanager
+def elapsed_timer(message: str, format_seconds: bool = False) -> Generator:
+    """Context manager to print the elapsed time for a block of code in addition to its local rank and PID.
+    Usage:
+    with elapsed_timer("doing this and that"):
+        print("doing this and that")
+    """
+    start = time.time()
+    yield
+    elapsed = time.time() - start
+    time_expr = format_time_from_seconds(elapsed) if format_seconds else f"{elapsed:0.2f} seconds"
+    print_message_with_rank_pid(f"{message} took {time_expr}")
```

### Comparing `hi-ml-azure-0.2.9/src/health_azure/mlflow_utils.py` & `hi-ml-azure-0.3.0/src/health_azure/mlflow_utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -29,16 +29,15 @@
     :param mlflow_run: the mlflow Run to retrieve metrics from
     :return: A dictionary of metric_name to value
     """
     metrics = mlflow_run.data.metrics
     return metrics
 
 
-def get_metric_from_mlflow_run(mlflow_client: MlflowClient, run_id: str, metric_name: str
-                               ) -> List[Metric]:
+def get_metric_from_mlflow_run(mlflow_client: MlflowClient, run_id: str, metric_name: str) -> List[Metric]:
     """
     For a given metric name, get the entire history of logged values from an mlflow Run
 
     :param mlflow_client: An MLFlowClient object.
     :param run_id: The id of the run to retrieve the metrics from.
     :param metric_name: The name of the metric to retrieve values for.
     :return: A list of mlflow Metric objects representing the all of the values of the given
```

### Comparing `hi-ml-azure-0.2.9/src/health_azure/paths.py` & `hi-ml-azure-0.3.0/src/health_azure/paths.py`

 * *Files identical despite different names*

### Comparing `hi-ml-azure-0.2.9/src/health_azure/traverse.py` & `hi-ml-azure-0.3.0/src/health_azure/traverse.py`

 * *Files identical despite different names*

### Comparing `hi-ml-azure-0.2.9/src/health_azure/utils.py` & `hi-ml-azure-0.3.0/src/health_azure/utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,62 +7,78 @@
 """
 import hashlib
 import json
 import logging
 import os
 import re
 import shutil
-import sys
 import tempfile
-from argparse import (_UNRECOGNIZED_ARGS_ATTR, OPTIONAL, SUPPRESS, ArgumentDefaultsHelpFormatter, ArgumentError,
-                      ArgumentParser, Namespace)
+import time
 from collections import defaultdict
 from contextlib import contextmanager
-from dataclasses import dataclass
 from enum import Enum
 from itertools import islice
 from pathlib import Path
-from typing import (Any, Callable, DefaultDict, Dict, Generator, Iterable, List, Optional, Set, Tuple, Type, TypeVar,
-                    Union)
+from typing import (
+    Any,
+    DefaultDict,
+    Dict,
+    Generator,
+    Iterable,
+    List,
+    Optional,
+    Tuple,
+    Type,
+    TypeVar,
+    Union,
+)
 
 import conda_merge
 import pandas as pd
 import param
 
 from azureml._restclient.constants import RunStatus
 from azureml.core import Environment, Experiment, Run, Workspace, get_run
 from azureml.core.authentication import InteractiveLoginAuthentication, ServicePrincipalAuthentication
 from azureml.core.conda_dependencies import CondaDependencies
 from azureml.core.run import _OfflineRun
 from azureml.data.azure_storage_datastore import AzureBlobDatastore
-from azureml.train.hyperdrive import HyperDriveRun
 
 from azure.ai.ml import MLClient
 from azure.ai.ml.entities import Job
 from azure.ai.ml.entities import Workspace as WorkspaceV2
 from azure.ai.ml.entities import Environment as EnvironmentV2
 from azure.core.credentials import TokenCredential
 from azure.core.exceptions import ClientAuthenticationError, ResourceNotFoundError
-from azure.identity import (ClientSecretCredential, DeviceCodeCredential,
-                            DefaultAzureCredential, InteractiveBrowserCredential)
+from azure.identity import (
+    ClientSecretCredential,
+    DeviceCodeCredential,
+    DefaultAzureCredential,
+    InteractiveBrowserCredential,
+)
 
+from health_azure.argparsing import EXPERIMENT_RUN_SEPARATOR, RunIdOrListParam, determine_run_id_type
+
+
+logger = logging.getLogger(__name__)
 
 T = TypeVar("T")
 
-EXPERIMENT_RUN_SEPARATOR = ":"
 DEFAULT_UPLOAD_TIMEOUT_SECONDS: int = 36_000  # 10 Hours
 
 # The version to use when creating an AzureML Python environment. We create all environments with a unique hashed
 # name, hence version will always be fixed
 ENVIRONMENT_VERSION = "1"
 
 # Environment variables used for authentication
 ENV_SERVICE_PRINCIPAL_ID = "HIML_SERVICE_PRINCIPAL_ID"
 ENV_SERVICE_PRINCIPAL_PASSWORD = "HIML_SERVICE_PRINCIPAL_PASSWORD"
 ENV_TENANT_ID = "HIML_TENANT_ID"
+
+# Environment variables used for workspace selection
 ENV_RESOURCE_GROUP = "HIML_RESOURCE_GROUP"
 ENV_SUBSCRIPTION_ID = "HIML_SUBSCRIPTION_ID"
 ENV_WORKSPACE_NAME = "HIML_WORKSPACE_NAME"
 
 # Environment variables used for multi-node training
 ENV_AZ_BATCHAI_MPI_MASTER_NODE = "AZ_BATCHAI_MPI_MASTER_NODE"
 ENV_AZ_BATCH_MASTER_NODE = "AZ_BATCH_MASTER_NODE"
@@ -72,14 +88,17 @@
 ENV_OMPI_COMM_WORLD_RANK = "OMPI_COMM_WORLD_RANK"
 ENV_NODE_RANK = "NODE_RANK"
 ENV_GLOBAL_RANK = "GLOBAL_RANK"
 ENV_LOCAL_RANK = "LOCAL_RANK"
 ENV_RANK = "RANK"
 MASTER_PORT_DEFAULT = 6105
 
+# Environment variables that affect job submission, in particular in builds
+ENV_EXPERIMENT_NAME = "HIML_EXPERIMENT_NAME"
+
 # Other Azure ML related variables
 ENVIRONMENT_VERSION = "1"
 FINAL_MODEL_FOLDER = "final_model"
 MODEL_ID_KEY_NAME = "model_id"
 PYTHON_ENVIRONMENT_NAME = "python_environment_name"
 RUN_CONTEXT: Run = Run.get_context()
 PARENT_RUN_CONTEXT = getattr(RUN_CONTEXT, "parent", None)
@@ -97,44 +116,37 @@
 DEFAULT_ENVIRONMENT_VARIABLES = {
     "AZUREML_OUTPUT_UPLOAD_TIMEOUT_SEC": "3600",
     # Occasionally uploading data during the run takes too long, and makes the job fail. Default is 300.
     "AZUREML_RUN_KILL_SIGNAL_TIMEOUT_SEC": "900",
     "MKL_SERVICE_FORCE_INTEL": "1",
     # Switching to a new software stack in AML for mounting datasets
     "RSLEX_DIRECT_VOLUME_MOUNT": "true",
-    "RSLEX_DIRECT_VOLUME_MOUNT_MAX_CACHE_SIZE": "1",
-    "DATASET_MOUNT_CACHE_SIZE": "1",
 }
 
 
 V2_INPUT_DATASET_PATTERN = r"--INPUT_\d[=| ]"
 V2_OUTPUT_DATASET_PATTERN = r"--OUTPUT_\d[=| ]"
 
 PathOrString = Union[Path, str]
+# An AML v1 Run or an AML v2 Job
+RunOrJob = Union[Run, Job]
 
 
-class IntTuple(param.NumericTuple):
-    """
-    Parameter class that must always have integer values
-    """
-
-    def _validate(self, val: Any) -> None:
-        """
-        Check that input "val" is indeed a tuple of integers. If it is a tuple of some other type, raises
-        a ValueError
+class JobStatus(Enum):
+    """String constants for the status of an AML v2 Job"""
 
-        :param val: The value to be checked
-        """
-        super()._validate(val)
-        if val is not None:
-            for i, n in enumerate(val):
-                if not isinstance(n, int):
-                    raise ValueError(
-                        f"{self.name}: tuple element at index {i} with value {n} in {val} is not an integer"
-                    )
+    COMPLETED = "Completed"
+    STARTING = "Starting"
+    FAILED = "Failed"
+    CANCELED = "Canceled"
+
+    @classmethod
+    def is_finished_state(cls, state_to_check: Optional[str]) -> bool:
+        """Checks if the given state is a finished state"""
+        return state_to_check in [cls.COMPLETED.value, cls.FAILED.value, cls.CANCELED.value]
 
 
 class GenericConfig(param.Parameterized):
     def __init__(self, should_validate: bool = True, throw_if_unknown_param: bool = False, **params: Any):
         """
         Instantiates the config class, ignoring parameters that are not overridable.
 
@@ -186,333 +198,14 @@
             config.set_param(key, value)
         except ValueError:
             setattr(config, key, value)
     if validate:
         config.validate()
 
 
-def create_argparser(
-    config: param.Parameterized,
-    usage: Optional[str] = None,
-    description: Optional[str] = None,
-    epilog: Optional[str] = None
-) -> ArgumentParser:
-    """
-    Creates an ArgumentParser with all fields of the given config that are overridable.
-
-    :param config: The config whose parameters should be used to populate the argument parser
-    :param usage: Brief information about correct usage that is printed if the script started with "--help". If not
-    provided, this is auto-generated from the complete set of arguments.
-    :param description: A description of the program that is printed if the script is started with "--help"
-    :param epilog: A text that is printed after the argument details if the script is started with "--help"
-    :return: ArgumentParser
-    """
-    assert isinstance(config, param.Parameterized)
-    parser = ArgumentParser(
-        formatter_class=ArgumentDefaultsHelpFormatter,
-        usage=usage,
-        description=description,
-        epilog=epilog
-    )
-    _add_overrideable_config_args_to_parser(config, parser)
-    return parser
-
-
-def _add_overrideable_config_args_to_parser(config: param.Parameterized, parser: ArgumentParser) -> ArgumentParser:
-    """
-    Adds all overridable fields of the config class to the given argparser.
-    Fields that are marked as readonly, constant or private are ignored.
-
-    :param parser: Parser to add properties to.
-    """
-
-    def parse_bool(x: str) -> bool:
-        """
-        Parse a string as a bool. Supported values are case insensitive and one of:
-        'on', 't', 'true', 'y', 'yes', '1' for True
-        'off', 'f', 'false', 'n', 'no', '0' for False.
-
-        :param x: string to test.
-        :return: Bool value if string valid, otherwise a ValueError is raised.
-        """
-        sx = str(x).lower()
-        if sx in ("on", "t", "true", "y", "yes", "1"):
-            return True
-        if sx in ("off", "f", "false", "n", "no", "0"):
-            return False
-        raise ValueError(f"Invalid value {x}, please supply one of True, true, false or False.")
-
-    def _get_basic_type(_p: param.Parameter) -> Union[type, Callable]:
-        """
-        Given a parameter, get its basic Python type, e.g.: param.Boolean -> bool.
-        Throw exception if it is not supported.
-
-        :param _p: parameter to get type and nargs for.
-        :return: Type
-        """
-        get_type: Callable
-        if isinstance(_p, param.Boolean):
-            get_type = parse_bool
-        elif isinstance(_p, param.Integer):
-            def to_int(x: str) -> int:
-                return _p.default if x == "" else int(x)
-            get_type = to_int
-        elif isinstance(_p, param.Number):
-            def to_float(x: str) -> float:
-                return _p.default if x == "" else float(x)
-            get_type = to_float
-        elif isinstance(_p, param.String):
-            get_type = str
-        elif isinstance(_p, param.List):
-            def to_list(x: str) -> List[Any]:
-                return [_p.class_(item) for item in x.split(",") if item]
-            get_type = to_list
-        elif isinstance(_p, param.NumericTuple):
-
-            def float_or_int(y: str) -> Union[int, float]:
-                return int(y) if isinstance(_p, IntTuple) else float(y)
-
-            def to_tuple(x: str) -> Tuple:
-                return tuple([float_or_int(item) for item in x.split(",")])
-            get_type = to_tuple
-        elif isinstance(_p, param.ClassSelector):
-            get_type = _p.class_
-        elif isinstance(_p, CustomTypeParam):
-            get_type = _p.from_string
-
-        else:
-            raise TypeError(f"Parameter of type {_p} is not supported")
-
-        return get_type
-
-    def add_boolean_argument(parser: ArgumentParser, k: str, p: param.Parameter) -> None:
-        """
-        Add a boolean argument.
-        If the parameter default is False then allow --flag (to set it True) and --flag=Bool as usual.
-        If the parameter default is True then allow --no-flag (to set it to False) and --flag=Bool as usual.
-
-        :param parser: parser to add a boolean argument to.
-        :param k: argument name.
-        :param p: boolean parameter.
-        """
-        if not p.default:
-            # If the parameter default is False then use nargs="?" (OPTIONAL).
-            # This means that the argument is optional.
-            # If it is not supplied, i.e. in the --flag mode, use the "const" value, i.e. True.
-            # Otherwise, i.e. in the --flag=value mode, try to parse the argument as a bool.
-            parser.add_argument("--" + k, help=p.doc, type=parse_bool, default=False, nargs=OPTIONAL, const=True)
-        else:
-            # If the parameter default is True then create an exclusive group of arguments.
-            # Either --flag=value as usual
-            # Or --no-flag to store False in the parameter k.
-            group = parser.add_mutually_exclusive_group(required=False)
-            group.add_argument("--" + k, help=p.doc, type=parse_bool)
-            group.add_argument("--no-" + k, dest=k, action="store_false")
-            parser.set_defaults(**{k: p.default})
-
-    for k, p in get_overridable_parameters(config).items():
-        # param.Booleans need to be handled separately, they are more complicated because they have
-        # an optional argument.
-        if isinstance(p, param.Boolean):
-            add_boolean_argument(parser, k, p)
-        else:
-            parser.add_argument("--" + k, help=p.doc, type=_get_basic_type(p), default=p.default)
-
-    return parser
-
-
-@dataclass
-class ParserResult:
-    """
-    Stores the results of running an argument parser, broken down into a argument-to-value dictionary,
-    arguments that the parser does not recognize.
-    """
-
-    args: Dict[str, Any]
-    unknown: List[str]
-    overrides: Dict[str, Any]
-
-
-def _create_default_namespace(parser: ArgumentParser) -> Namespace:
-    """
-    Creates an argparse Namespace with all parser-specific default values set.
-
-    :param parser: The parser to work with.
-    :return: the Namespace object
-    """
-    # This is copy/pasted from parser.parse_known_args
-    namespace = Namespace()
-    for action in parser._actions:
-        if action.dest is not SUPPRESS:
-            if not hasattr(namespace, action.dest):
-                if action.default is not SUPPRESS:
-                    setattr(namespace, action.dest, action.default)
-    for dest in parser._defaults:
-        if not hasattr(namespace, dest):
-            setattr(namespace, dest, parser._defaults[dest])
-    return namespace
-
-
-def parse_arguments(
-    parser: ArgumentParser, fail_on_unknown_args: bool = False, args: Optional[List[str]] = None
-) -> ParserResult:
-    """
-    Parses a list of commandline arguments with a given parser. Returns results broken down into a full
-    arguments dictionary, a dictionary of arguments that were set to non-default values, and unknown
-    arguments.
-
-    :param parser: The parser to use
-    :param fail_on_unknown_args: If True, raise an exception if the parser encounters an argument that it does
-        not recognize. If False, unrecognized arguments will be ignored, and added to the "unknown" field of
-        the parser result.
-    :param args: Arguments to parse. If not given, use those in sys.argv
-    :return: The parsed arguments, and overrides
-    """
-    if args is None:
-        args = sys.argv[1:]
-    # The following code is a slightly modified version of what happens in parser.parse_known_args. This had to be
-    # copied here because otherwise we would not be able to achieve the priority order that we desire.
-    namespace = _create_default_namespace(parser)
-
-    try:
-        namespace, unknown = parser._parse_known_args(args, namespace)
-        if hasattr(namespace, _UNRECOGNIZED_ARGS_ATTR):
-            unknown.extend(getattr(namespace, _UNRECOGNIZED_ARGS_ATTR))
-            delattr(namespace, _UNRECOGNIZED_ARGS_ATTR)
-    except ArgumentError:
-        parser.print_usage(sys.stderr)
-        err = sys.exc_info()[1]
-        parser._print_message(str(err), sys.stderr)
-        raise
-    # Parse the arguments a second time, without supplying defaults, to see which arguments actually differ
-    # from defaults.
-    namespace_without_defaults, _ = parser._parse_known_args(args, Namespace())
-    parsed_args = vars(namespace).copy()
-    overrides = vars(namespace_without_defaults).copy()
-    if len(unknown) > 0 and fail_on_unknown_args:
-        raise ValueError(f"Unknown arguments: {unknown}")
-    return ParserResult(
-        args=parsed_args,
-        unknown=unknown,
-        overrides=overrides,
-    )
-
-
-def parse_args_and_update_config(config: Any, args: List[str]) -> Any:
-    """
-    Given a model config and a list of command line arguments, creates an argparser, adds arguments from the config
-    parses the list of provided args and updates the config accordingly. Returns the updated config
-
-    :param config: The model configuration
-    :param args: A list of command line args to parse
-    :return: The config, updated with the values of the provided args
-    """
-    parser = create_argparser(config)
-    parser_results = parse_arguments(parser, args=args)
-    _ = apply_overrides(config, parser_results.args)
-    return config
-
-
-def get_overridable_parameters(config: Any) -> Dict[str, param.Parameter]:
-    """
-    Get properties that are not constant, readonly or private (eg: prefixed with an underscore).
-
-    :param config: The model configuration
-    :return: A dictionary of parameter names and their definitions.
-    """
-    assert isinstance(config, param.Parameterized)
-    return dict((k, v) for k, v in config.param.params().items() if reason_not_overridable(v) is None)
-
-
-def reason_not_overridable(value: param.Parameter) -> Optional[str]:
-    """
-    Given a parameter, check for attributes that denote it is not overrideable (e.g. readonly, constant,
-    private etc). If such an attribute exists, return a string containing a single-word description of the
-    reason. Otherwise returns None.
-
-    :param value: a parameter value
-    :return: None if the parameter is overridable; otherwise a one-word string explaining why not.
-    """
-    if value.readonly:
-        return "readonly"
-    elif value.constant:
-        return "constant"
-    elif is_private_field_name(value.name):
-        return "private"
-    elif isinstance(value, param.Callable):
-        return "callable"
-    return None
-
-
-def apply_overrides(
-    config: Any,
-    overrides_to_apply: Optional[Dict[str, Any]],
-    should_validate: bool = False,
-    keys_to_ignore: Optional[Set[str]] = None,
-) -> Dict[str, Any]:
-    """
-    Applies the provided `values` overrides to the config.
-    Only properties that are marked as overridable are actually overwritten.
-
-    :param config: The model configuration
-    :param overrides_to_apply: A dictionary mapping from field name to value.
-    :param should_validate: If true, run the .validate() method after applying overrides.
-    :param keys_to_ignore: keys to ignore in reporting failed overrides. If None, do not report.
-    :return: A dictionary with all the fields that were modified.
-    """
-
-    def _apply(_overrides: Optional[Dict[str, Any]]) -> Dict[str, Any]:
-        applied: Dict[str, Any] = {}
-        if _overrides is not None:
-            overridable_parameters = get_overridable_parameters(config).keys()
-            for k, v in _overrides.items():
-                if k in overridable_parameters:
-                    applied[k] = v
-                    setattr(config, k, v)
-
-        return applied
-
-    actual_overrides = _apply(overrides_to_apply)
-    if keys_to_ignore is not None:
-        report_on_overrides(config, overrides_to_apply, keys_to_ignore)  # type: ignore
-    if should_validate:
-        config.validate()
-    return actual_overrides
-
-
-def report_on_overrides(config: Any, overrides_to_apply: Dict[str, Any], keys_to_ignore: Set[str]) -> None:
-    """
-    Logs a warning for every parameter whose value is not as given in "overrides_to_apply", other than those
-    in keys_to_ignore.
-
-    :param config: The model configuration
-    :param overrides_to_apply: override dictionary, parameter names to values
-    :param keys_to_ignore: set of dictionary keys not to report on
-    """
-    assert isinstance(config, param.Parameterized)
-    current_params = config.param.params()
-    for key, desired in overrides_to_apply.items():
-        if key in keys_to_ignore:
-            continue
-        actual = getattr(config, key, None)
-        if actual == desired:
-            continue
-        if key not in current_params:
-            reason = "parameter is undefined"
-        else:
-            val = current_params[key]
-            reason = reason_not_overridable(val)  # type: ignore
-            if reason is None:
-                reason = "for UNKNOWN REASONS"
-            else:
-                reason = f"parameter is {reason}"
-        # We could raise an error here instead - to be discussed.
-        logging.warning(f"Override {key}={desired} failed: {reason} in class {config.__class__.name}")
-
-
 def create_from_matching_params(from_object: param.Parameterized, cls_: Type[T]) -> T:
     """
     Creates an object of the given target class, and then copies all attributes from the `from_object` to
     the newly created object, if there is a matching attribute. The target class must be a subclass of
     param.Parameterized.
 
     :param from_object: The object to read attributes from.
@@ -524,144 +217,43 @@
         raise ValueError(f"The created object must be a subclass of param.Parameterized, but got {type(c)}")
     for param_name, p in c.param.params().items():  # type: ignore
         if not p.constant and not p.readonly:
             setattr(c, param_name, getattr(from_object, param_name))
     return c
 
 
-class CustomTypeParam(param.Parameter):
-    def _validate(self, val: Any) -> None:
-        """
-        Validate that the input "val" has the expected format. For example, if this custom type should represent a
-        list, verify here that it is so.
-
-        :param val: the value to be verified
-        """
-        super()._validate(val)
-
-    def from_string(self, x: str) -> Any:
-        """
-        Base method for taking an input string and returning it evaluated as its expected type (e.g. from_string("3")
-        would most likely return int("3")"
-
-        :param x: The string to be evaluated
-        :return: The evaluated format of the string
-        """
-        raise NotImplementedError()
-
-
-class ListOrDictParam(CustomTypeParam):
+def create_v2_job_command_line_args_from_params(script_params: List[str]) -> str:
+    """Given a list of parameters as passed in from the command line, create a string that can be passed as a command
+    to execute a v2 AzureML job. Specifically, wraps any parameter string that contain double or single quotes in the
+    opposite type of quote to avoid escaping issues. E.g. --param1=['foo1', 'foo2'] becomes "--param1=['foo1', 'foo2']".
+
+    :param script_params: List of params, e.g. ["--param1", "--param2==foo"]
+    :raises ValueError: If a single parameter contains both a single quote and a double quote.
+    :return: The command line arguments as a v2 job-acceptable string.
     """
-    Wrapper class to allow either a List or Dict inside of a Parameterized object.
-    """
-
-    def _validate(self, val: Any) -> None:
-        """
-        Checks that input "val" is indeed a List or Dict object
-
-        :param val: the value to be checked
-        """
-
-        if val is None:
-            if not self.allow_None:
-                raise ValueError("Value must not be None")
-            else:
-                return
-        if not (isinstance(val, List) or isinstance(val, Dict)):
-            raise ValueError(f"{val} must be an instance of List or Dict, found {type(val)}")
-        super()._validate(val)
 
-    def from_string(self, x: str) -> Union[Dict, List]:
-        """
-        Parse a string as either a dictionary or list or, if not possible, raise a ValueError.
-
-        For example:
-            - from_string('{"x":3, "y":2}') will return a dictionary object
-            - from_string('["a", "b", "c"]') will return a list object
-            - from_string("['foo']") will return a list object
-            - from_string('["foo","bar"') will raise an Exception (missing close bracket)
-            - from_string({'learning':3"') will raise an Exception (missing close bracket)
-
-        :param x: the string to parse
-        :return: a List or Dict object, as evaluated from the input string
-        """
-        if x.startswith("{") or x.startswith("["):
-            res = json.loads(x.replace("'", '"'))
-        else:
-            res = [str(item) for item in x.split(",")]
-        if isinstance(res, Dict):
-            return res
-        elif isinstance(res, List):
-            return res
+    parsed_cmd_strings: List[str] = []
+    for script_param in script_params:
+        if "'" in script_param and '"' in script_param:
+            raise ValueError(
+                f"Script parameters cannot contain both single and double quotes. Problematic parameter: {script_param}"
+            )
+        elif "'" in script_param:
+            parsed_cmd_strings.append(f'"{script_param}"')
+        elif '"' in script_param:
+            parsed_cmd_strings.append(f"'{script_param}'")
         else:
-            raise ValueError("Parameter should resolve to List or Dict")
-
-
-class RunIdOrListParam(CustomTypeParam):
-    """
-    Wrapper class to allow either a List or string inside of a Parameterized object.
-    """
-
-    def _validate(self, val: Any) -> None:
-        """
-        Checks that the input "val" is indeed a non-empty list or string
-
-        :param val: The value to check
-        """
-        if val is None:
-            if not self.allow_None:
-                raise ValueError("Value must not be None")
-            else:
-                return
-        if len(val) == 0 or not (isinstance(val, str) or isinstance(val, list)):
-            raise ValueError(f"{val} must be an instance of List or string, found {type(val)}")
-        super()._validate(val)
-
-    def from_string(self, x: str) -> List[str]:
-        """
-        Given a string representing one or more run_ids, first attempts to split into a list, and then
-        evaluates each item in the list as a genuine run id
-
-        :param x: The string to evaluate
-        :return: a list of one or more strings representing run ids
-        """
-        res = [str(item) for item in x.split(",")]
-        return [determine_run_id_type(x) for x in res]
+            parsed_cmd_strings.append(f'{script_param}')
 
-
-def is_private_field_name(name: str) -> bool:
-    """
-    A private field is any Python class member that starts with an underscore eg: _hello
-
-    :param name: a string representing the name of the class member
-    """
-    return name.startswith("_")
-
-
-def determine_run_id_type(run_or_recovery_id: str) -> str:
-    """
-    Determine whether a run id is of type "run id" or "run recovery id". Run recovery ideas take the form
-    "experiment_name:run_id". If the input
-    string takes the format of a run recovery id, only the run id part will be returned. If it is a run id already,
-    it will be returned without transformation.
-
-    :param run_or_recovery_id: The id to determine as either a run id or a run recovery id
-    :return: A string representing the run id
-    """
-    if run_or_recovery_id is None:
-        raise ValueError("Expected run_id or run_recovery_id but got None")
-    parts = run_or_recovery_id.split(EXPERIMENT_RUN_SEPARATOR)
-    if len(parts) > 1:
-        # return only the run_id, which comes after the colon
-        return parts[1]
-    return run_or_recovery_id
+    return " ".join(parsed_cmd_strings)
 
 
-def find_file_in_parent_folders(file_name: str, stop_at_path: List[Path],
-                                start_at_path: Optional[Path] = None) -> Optional[Path]:
+def find_file_in_parent_folders(
+    file_name: str, stop_at_path: List[Path], start_at_path: Optional[Path] = None
+) -> Optional[Path]:
     """Searches for a file of the given name in the current working directory, or any of its parent folders.
     Searching stops if either the file is found, or no parent folder can be found, or the search has reached any
     of the given folders in stop_at_path.
 
     :param file_name: The name of the file to find.
     :param stop_at_path: A list of folders. If any of them is reached, search stops.
     :param start_at_path: An optional path to the directory in which to start searching. If not supplied,
@@ -694,51 +286,79 @@
     if "PYTHONPATH" in os.environ:
         pythonpaths = [Path(path_string) for path_string in os.environ["PYTHONPATH"].split(os.pathsep)]
     return find_file_in_parent_folders(file_name=file_name, stop_at_path=pythonpaths)
 
 
 def get_workspace(aml_workspace: Optional[Workspace] = None, workspace_config_path: Optional[Path] = None) -> Workspace:
     """
-    Retrieve an Azure ML Workspace from one of several places:
-      1. If the function has been called during an AML run (i.e. on an Azure agent), returns the associated workspace
-      2. If a Workspace object has been provided by the user, return that
-      3. If a path to a Workspace config file has been provided, load the workspace according to that.
+    Retrieve an Azure ML Workspace by going through the following steps:
 
-    If not running inside AML and neither a workspace nor the config file are provided, the code will try to locate a
-    config.json file in any of the parent folders of the current working directory. If that succeeds, that config.json
-    file will be used to instantiate the workspace.
+      1. If the function has been called from inside a run in AzureML, it returns the current AzureML workspace.
+
+      2. If a Workspace object has been provided in the `aml_workspace` argument, return that.
+
+      3. If a path to a Workspace config file has been provided, load the workspace according to that config file.
+
+      4. If a Workspace config file is present in the current working directory or one of its parents, load the
+        workspace according to that config file.
+
+      5. If 3 environment variables are found, use them to identify the workspace (`HIML_RESOURCE_GROUP`,
+        `HIML_SUBSCRIPTION_ID`, `HIML_WORKSPACE_NAME`)
+
+    If none of the above succeeds, an exception is raised.
 
     :param aml_workspace: If provided this is returned as the AzureML Workspace.
     :param workspace_config_path: If not provided with an AzureML Workspace, then load one given the information in this
         config
     :return: An AzureML workspace.
+    :raises ValueError: If none of the available options for accessing the workspace succeeds.
+    :raises FileNotFoundError: If the workspace config file is given in `workspace_config_path`, but is not present.
     """
     if is_running_in_azure_ml(RUN_CONTEXT):
         return RUN_CONTEXT.experiment.workspace
 
     # If aml_workspace has been provided, use that
     if aml_workspace:
         return aml_workspace
 
     if workspace_config_path is None:
+        logging.info(
+            f"Trying to locate the workspace config file '{WORKSPACE_CONFIG_JSON}' in the current folder "
+            "and its parent folders"
+        )
         workspace_config_path = find_file_in_parent_to_pythonpath(WORKSPACE_CONFIG_JSON)
         if workspace_config_path:
             logging.info(f"Using the workspace config file {str(workspace_config_path.absolute())}")
-        else:
-            raise ValueError("No workspace config file given, nor can we find one.")
 
-    if not isinstance(workspace_config_path, Path):
-        raise ValueError("Workspace config path is not a path, check your input.")
-    elif workspace_config_path.is_file():
-        auth = get_authentication()
+    auth = get_authentication()
+    if workspace_config_path is not None:
+        if not workspace_config_path.is_file():
+            raise FileNotFoundError(f"Workspace config file does not exist: {workspace_config_path}")
         workspace = Workspace.from_config(path=str(workspace_config_path), auth=auth)
-        logging.info(f"Logged into AzureML workspace {workspace.name}")
+        logging.info(
+            f"Logged into AzureML workspace {workspace.name} as specified in config file " f"{workspace_config_path}"
+        )
         return workspace
 
-    raise ValueError("Workspace config file does not exist or cannot be read.")
+    logging.info("Trying to load the environment variables that define the workspace.")
+    workspace_name = get_secret_from_environment(ENV_WORKSPACE_NAME, allow_missing=True)
+    subscription_id = get_secret_from_environment(ENV_SUBSCRIPTION_ID, allow_missing=True)
+    resource_group = get_secret_from_environment(ENV_RESOURCE_GROUP, allow_missing=True)
+    if bool(workspace_name) and bool(subscription_id) and bool(resource_group):
+        workspace = Workspace.get(
+            name=workspace_name, auth=auth, subscription_id=subscription_id, resource_group=resource_group
+        )
+        logging.info(f"Logged into AzureML workspace {workspace.name} as specified by environment variables")
+        return workspace
+
+    raise ValueError(
+        "Tried all ways of identifying the workspace, but failed. Please provide a workspace config "
+        f"file {WORKSPACE_CONFIG_JSON} or set the environment variables {ENV_RESOURCE_GROUP}, "
+        f"{ENV_SUBSCRIPTION_ID}, and {ENV_WORKSPACE_NAME}."
+    )
 
 
 def create_run_recovery_id(run: Run) -> str:
     """
      Creates a unique ID for a run, from which the experiment name and the run ID can be re-created
 
     :param run: an instantiated run.
@@ -815,15 +435,17 @@
 
     :return: A ServicePrincipalAuthentication object that has the application ID and key or None if the key is not
         present
     """
     service_principal_id = get_secret_from_environment(ENV_SERVICE_PRINCIPAL_ID, allow_missing=True)
     tenant_id = get_secret_from_environment(ENV_TENANT_ID, allow_missing=True)
     service_principal_password = get_secret_from_environment(ENV_SERVICE_PRINCIPAL_PASSWORD, allow_missing=True)
-    if service_principal_id and tenant_id and service_principal_password:
+    # Check if all 3 environment variables are set
+    if bool(service_principal_id) and bool(tenant_id) and bool(service_principal_password):
+        logging.info("Found all necessary environment variables for Service Principal authentication.")
         return ServicePrincipalAuthentication(
             tenant_id=tenant_id,
             service_principal_id=service_principal_id,
             service_principal_password=service_principal_password,
         )
     logging.info(
         "Using interactive login to Azure. To use Service Principal authentication, set the environment "
@@ -923,16 +545,17 @@
 
 
 class PinnedOperator(Enum):
     CONDA = "="
     PIP = "=="
 
 
-def _resolve_package_clash(duplicate_dependencies: List[PackageDependency], pinned_operator: PinnedOperator
-                           ) -> PackageDependency:
+def _resolve_package_clash(
+    duplicate_dependencies: List[PackageDependency], pinned_operator: PinnedOperator
+) -> PackageDependency:
     """Given a list of duplicate package names with conflicting versions, if exactly one of these
     is pinned, return that, otherwise raise a ValueError
 
     :param duplicate_dependencies: a list of PackageDependency objects with the same package name
     :raises ValueError: if none of the depencencies specify a pinned version
     :return: A single PackageDependency object specifying a pinned version (e.g. 'pkg==0.1')
     """
@@ -945,20 +568,21 @@
                 raise ValueError(f"Found more than one pinned dependency for package: {dependency.package_name}")
     if found_pinned_dependecy:
         return found_pinned_dependecy
     else:
         num_clashes = len(duplicate_dependencies)
         pkg_name = duplicate_dependencies[0].package_name
         raise ValueError(
-            f"Encountered {num_clashes} requirements for package {pkg_name}, none of which specify"
-            " a pinned version.")
+            f"Encountered {num_clashes} requirements for package {pkg_name}, none of which specify a pinned version."
+        )
 
 
-def _resolve_dependencies(all_dependencies: Dict[str, List[PackageDependency]], pinned_operator: PinnedOperator
-                          ) -> List[PackageDependency]:
+def _resolve_dependencies(
+    all_dependencies: Dict[str, List[PackageDependency]], pinned_operator: PinnedOperator
+) -> List[PackageDependency]:
     """Apply conflict resolution for pip package versions. Given a dictionary of package name: PackageDependency
     objects, applies the following logic:
         - if the package only appears once in all definitions, keep that package version
         - if the package appears in multiple definitions, and is pinned only once, keep that package version
         - otherwise, raise a ValueError
 
     :param all_dependencies: a dictionary of package name: list of PackageDependency objects including description of
@@ -1159,15 +783,15 @@
         return environment.register(workspace)
 
 
 def create_python_environment_v2(
     conda_environment_file: Path,
     pip_extra_index_url: str = "",
     private_pip_wheel_path: Optional[Path] = None,
-    docker_base_image: str = ""
+    docker_base_image: str = "",
 ) -> EnvironmentV2:
     """
     Creates a description for the V2 Python execution environment in AzureML, based on the arguments.
     The environment will have a name that uniquely identifies it (it is based on hashing the contents of the
     Conda file, the docker base image, environment variables and private wheels.
 
     :param docker_base_image: The Docker base image that should be used when creating a new Docker image.
@@ -1250,36 +874,33 @@
 
 def set_environment_variables_for_multi_node() -> None:
     """
     Sets the environment variables that PyTorch Lightning needs for multi-node training.
     """
     if ENV_AZ_BATCH_MASTER_NODE in os.environ:
         master_node = os.environ[ENV_AZ_BATCH_MASTER_NODE]
-        logging.debug(
-            f"Found AZ_BATCH_MASTER_NODE: {master_node} in environment variables")
+        logging.debug(f"Found AZ_BATCH_MASTER_NODE: {master_node} in environment variables")
         # For AML BATCHAI
         split_master_node_addr = master_node.split(":")
         if len(split_master_node_addr) == 2:
             master_addr, port = split_master_node_addr
             os.environ[ENV_MASTER_PORT] = port
         elif len(split_master_node_addr) == 1:
             master_addr = split_master_node_addr[0]
         else:
             raise ValueError(f"Format not recognized: {master_node}")
         os.environ[ENV_MASTER_ADDR] = master_addr
     elif ENV_AZ_BATCHAI_MPI_MASTER_NODE in os.environ and os.environ.get(ENV_AZ_BATCHAI_MPI_MASTER_NODE) != "localhost":
         mpi_master_node = os.environ[ENV_AZ_BATCHAI_MPI_MASTER_NODE]
-        logging.debug(
-            f"Found AZ_BATCHAI_MPI_MASTER_NODE: {mpi_master_node} in environment variables")
+        logging.debug(f"Found AZ_BATCHAI_MPI_MASTER_NODE: {mpi_master_node} in environment variables")
         # For AML BATCHAI
         os.environ[ENV_MASTER_ADDR] = mpi_master_node
     elif ENV_MASTER_IP in os.environ:
         master_ip = os.environ[ENV_MASTER_IP]
-        logging.debug(
-            f"Found MASTER_IP: {master_ip} in environment variables")
+        logging.debug(f"Found MASTER_IP: {master_ip} in environment variables")
         # AKS
         os.environ[ENV_MASTER_ADDR] = master_ip
     else:
         logging.info("No settings for the MPI central node found. Assuming that this is a single node training job.")
         return
 
     if ENV_MASTER_PORT not in os.environ:
@@ -1311,14 +932,41 @@
         return False
 
     runs = list(run.get_children())
     runs.append(run)
     return all(is_completed(run) for run in runs)
 
 
+def is_job_completed(job: Job) -> bool:
+    """Checks if the given AzureML v2 Job completed successfully.
+
+    :return: True if the job completed successfully, False for failures, job still running, etc."""
+    return job.status == JobStatus.COMPLETED.value
+
+
+def wait_for_job_completion(ml_client: MLClient, job_name: str) -> None:
+    """Wait until the job of the given ID is completed or failed with an error. If the job did not complete
+    successfully, a ValueError is raised.
+
+    :param ml_client: An MLClient object for the workspace where the job lives.
+    :param job_name: The name (id) of the job to wait for.
+    :raises ValueError: If the job did not complete successfully (any status other than Completed)
+    """
+
+    while True:
+        # Get the latest job status by reading the whole job info again via the MLClient
+        updated_job = ml_client.jobs.get(name=job_name)
+        current_job_status = updated_job.status
+        if JobStatus.is_finished_state(current_job_status):
+            break
+        time.sleep(10)
+    if not is_job_completed(updated_job):
+        raise ValueError(f"Job {updated_job.name} jobs failed with status {current_job_status}.")
+
+
 def get_most_recent_run_id(run_recovery_file: Path) -> str:
     """
     Gets the string name of the most recently executed AzureML run. This is picked up from the `most_recent_run.txt`
     file.
 
     :param run_recovery_file: The path of the run recovery file
     :return: The run id
@@ -1453,24 +1101,45 @@
     """
     workspace = get_workspace(aml_workspace=workspace, workspace_config_path=workspace_config_path)
     run = get_aml_run_from_run_id(run_id, aml_workspace=workspace)
     _download_files_from_run(run, output_folder, prefix=prefix, validate_checksum=validate_checksum)
     torch_barrier()
 
 
+def download_files_by_suffix(
+    run: Run, output_folder: Path, suffix: str, validate_checksum: bool = False
+) -> Iterable[Path]:
+    """Downloads all files from an AzureML run that have a given suffix, into a folder. The function returns an
+    Iterable, where a file path is emitted right after it has been downloaded.
+
+    :param run: The AzureML run from where the files should be downloaded.
+    :param suffix: The suffix for all files that should be returned.
+    :param output_folder: The folder where the files should be downloaded to. If a file `foo/bar.txt` is downloaded,
+        it will be downloaded as `<output_folder>/foo/bar.txt`.
+    :param validate_checksum: Whether to validate the content from HTTP response
+    :return: An Iterable with all downloaded files.
+    """
+    for file in get_run_file_names(run):
+        if file.endswith(suffix):
+            logging.info(f"Downloading file {file}")
+            output_folder.mkdir(parents=True, exist_ok=True)
+            output_file = output_folder / file
+            _download_file_from_run(run, file, output_file, validate_checksum=validate_checksum)
+            yield output_file
+
+
 def get_driver_log_file_text(run: Run, download_file: bool = True) -> Optional[str]:
     """
     Returns text stored in run log driver file.
 
     :param run: Run object representing the current run.
     :param download_file: If ``True``, download log file from the run.
     :return: Driver log file text if a file exists, ``None`` otherwise.
     """
     with tempfile.TemporaryDirectory() as tmp_dir_name:
-
         for log_file_path in VALID_LOG_FILE_PATHS:
             if download_file:
                 run.download_files(
                     prefix=str(log_file_path),
                     output_directory=tmp_dir_name,
                     append_prefix=False,
                 )
@@ -1519,15 +1188,14 @@
     :return: Local path to the downloaded file.
     """
     if not overwrite and output_file.exists():
         logging.info(f"File already exists at {output_file}")
     else:
         output_file.parent.mkdir(exist_ok=True, parents=True)
         _download_file_from_run(run, filename, output_file, validate_checksum=True)
-        assert output_file.exists()
         logging.info(f"File is downloaded at {output_file}")
     return output_file
 
 
 def is_global_rank_zero() -> bool:
     """
     Tries to guess if the current process is running as DDP rank zero, before the training has actually started,
@@ -1651,21 +1319,21 @@
     to your script (see HimlDownloadConfig and HimlTensorboardConfig for examples)
     """
 
     latest_run_file: Path = param.ClassSelector(
         class_=Path,
         default=None,
         instantiate=False,
-        doc="Optional path to most_recent_run.txt where the ID of the" "latest run is stored",
+        doc="Optional path to most_recent_run.txt where the ID of the latest run is stored",
     )
     experiment: str = param.String(
         default=None, allow_None=True, doc="The name of the AML Experiment that you wish to download Run files from"
     )
     num_runs: int = param.Integer(
-        default=1, allow_None=True, doc="The number of runs to download from the " "named experiment"
+        default=1, allow_None=True, doc="The number of runs to download from the named experiment"
     )
     config_file: Path = param.ClassSelector(
         class_=Path, default=None, instantiate=False, doc="Path to config.json where Workspace name is defined"
     )
     tags: Dict[str, Any] = param.Dict()
     run: List[str] = RunIdOrListParam(
         default=None,
@@ -1840,71 +1508,123 @@
     :param run_id: The id (type: str) of a parent/ HyperDrive run. Either this or run must be provided.
     :param keep_metrics: An optional list of metric names to filter the returned metrics by
     :param aml_workspace: If run_id is provided, this is an optional AML Workspace object to retrieve the Run from
     :param workspace_config_path: If run_id is provided, this is an optional path to a config containing details of the
         AML Workspace object to retrieve the Run from.
     :return: A Pandas DataFrame containing the aggregated metrics from each child run
     """
-    if run is None:
-        assert run_id is not None, "Either run or run_id must be provided"
-        workspace = get_workspace(aml_workspace=aml_workspace, workspace_config_path=workspace_config_path)
-        run = get_aml_run_from_run_id(run_id, aml_workspace=workspace)
-    assert isinstance(run, HyperDriveRun)
-    metrics: DefaultDict = defaultdict()
-    for child_run in run.get_children():  # type: ignore
-        child_run_metrics = child_run.get_metrics()
-        keep_metrics = keep_metrics or child_run_metrics.keys()
-
-        child_run_tag = get_tags_from_hyperdrive_run(child_run, child_run_arg_name)
-        for metric_name, metric_val in child_run_metrics.items():
-            if metric_name in keep_metrics:
-                if metric_name not in metrics:
-                    metrics[metric_name] = {}
-                metrics[metric_name][child_run_tag] = metric_val
-
-    df = pd.DataFrame.from_dict(metrics, orient="index")
+    metrics = get_metrics_for_hyperdrive_run(
+        child_run_arg_name=child_run_arg_name,
+        run_id=run_id,
+        run=run,
+        keep_metrics=keep_metrics,
+        aml_workspace=aml_workspace,
+        workspace_config_path=workspace_config_path,
+    )
+    metrics_swapped = {}
+    for run_tag, run_metrics in metrics.items():
+        for metric_name, metric_value in run_metrics.items():
+            if metric_name not in metrics_swapped:
+                metrics_swapped[metric_name] = {run_tag: metric_value}
+            else:
+                metrics_swapped[metric_name][run_tag] = metric_value
+    try:
+        df = pd.DataFrame.from_dict(metrics_swapped, orient="index")
+    except Exception:
+        raise ValueError(
+            "The metrics are not compatible with Pandas DataFrame. Likely cause is that some metrics are "
+            "scalars, and some are lists. Make sure that the lists come first."
+        )
     return df
 
 
-def get_metrics_for_childless_run(
+def get_metrics_for_run(
     run_id: Optional[str] = None,
     run: Optional[Run] = None,
     keep_metrics: Optional[List[str]] = None,
     aml_workspace: Optional[Workspace] = None,
     workspace_config_path: Optional[Path] = None,
-) -> pd.DataFrame:
+) -> Dict[str, Any]:
     """
-    For a given Run object or id, retrieves the metrics from that Run and returns them as a pandas DataFrame.
-    Optionally filters the metrics logged in the Run, by providing a list of metrics to keep. This function
-    expects a childless AML Run. If you wish to aggregate metrics for a Run with children (i.e. a HyperDriveRun),
-    please use the function ``aggregate_hyperdrive_metrics``.
+    For a given Run object or id, retrieves the metrics from that Run and returns them as a dictionary.
+    Optionally filters the metrics logged in the Run, by providing a list of metrics to keep.
+    If you wish to aggregate metrics for a Run with children (i.e. a HyperDriveRun),
+    please use the function ``get_metrics_for_hyperdrive_run``.
+
+    :param run: A Run object to retrieve the metrics from. Either this or run_id must be provided
+    :param run_id: The id (type: str) of an AML Run. Either this or run must be provided.
+    :param keep_metrics: An optional list of metric names to filter the returned metrics by. If the metric
+        is not logged in the run, a warning will be issued.
+    :param aml_workspace: If run_id is provided, this is an optional AML Workspace object to retrieve the Run from
+    :param workspace_config_path: If run_id is provided, this is an optional path to a config containing details of the
+        AML Workspace object to retrieve the Run from.
+    :return: A dictionary containing the metrics from the Run. The dictionary keys are the metric names, and the values
+        are the scalars or lists of scalars that were logged to the Run."""
+    if run is None:
+        if not run_id:
+            raise ValueError("Either run or run_id must be provided")
+        run = get_aml_run_from_run_id(run_id, aml_workspace=aml_workspace, workspace_config_path=workspace_config_path)
+    if isinstance(run, _OfflineRun):
+        logging.warning("Can't get metrics for _OfflineRun object")
+        return {}
+    if run.status != RunStatus.COMPLETED:  # type: ignore
+        logger.warning(
+            f"Run {run.id} is not completed, but has status '{run.status}'. "  # type: ignore
+            "Metrics may be incomplete."
+        )
+    all_metrics = run.get_metrics()  # type: ignore
+    if keep_metrics:
+        metrics = {}
+        for metric_name in keep_metrics:
+            if metric_name in all_metrics:
+                metrics[metric_name] = all_metrics[metric_name]
+            else:
+                logger.warning(f"Metric {metric_name} not found in run {run.id}")  # type: ignore
+        return metrics
+    return all_metrics
 
-    :param run: A (childless) Run object to retrieve the metrics from. Either this or run_id must be provided
-    :param run_id: The id (type: str) of a (childless) AML Run. Either this or run must be provided.
-    :param keep_metrics: An optional list of metric names to filter the returned metrics by
+
+def get_metrics_for_hyperdrive_run(
+    child_run_arg_name: str,
+    run_id: Optional[str] = None,
+    run: Optional[Run] = None,
+    keep_metrics: Optional[List[str]] = None,
+    aml_workspace: Optional[Workspace] = None,
+    workspace_config_path: Optional[Path] = None,
+) -> Dict[str, Any]:
+    """
+    For a given Run object or run id, retrieves the metrics for all the run's child runs.
+    Metrics are returned as a dictionary mapping from child run tag to metric name to metric value.
+    Optionally filters the metrics logged in the Run, by providing a list of metrics to keep.
+
+    :param run: A Run object to retrieve the metrics from. Either this or run_id must be provided
+    :param run_id: The id (type: str) of an AML Run. Either this or run must be provided.
+    :param keep_metrics: An optional list of metric names to filter the returned metrics by. If a metric is requested,
+        but not found on the run, a warning will be issued.
     :param aml_workspace: If run_id is provided, this is an optional AML Workspace object to retrieve the Run from
     :param workspace_config_path: If run_id is provided, this is an optional path to a config containing details of the
         AML Workspace object to retrieve the Run from.
-    :return: A Pandas DataFrame containing the metrics
+    :raises ValueError: If neither a run object nor a run ID are provided.
+    :return: A dictionary mapping from child run tag to the metrics that run. For each child run,
+        the dictionary keys are the metric names, and the values
+        are the scalars or lists of scalars that were logged to the Run.
     """
     if run is None:
-        assert run_id is not None, "Either run or run_id must be provided"
-        workspace = get_workspace(aml_workspace=aml_workspace, workspace_config_path=workspace_config_path)
-        run = get_aml_run_from_run_id(run_id, aml_workspace=workspace)
+        if not run_id:
+            raise ValueError("Either run or run_id must be provided")
+        run = get_aml_run_from_run_id(run_id, aml_workspace=aml_workspace, workspace_config_path=workspace_config_path)
     if isinstance(run, _OfflineRun):
-        logging.warning("Can't get metrics for _OfflineRun object")
-        return pd.DataFrame({})
+        logger.warning("Can't get metrics for _OfflineRun object")
+        return {}
     metrics = {}
-    run_metrics = run.get_metrics()  # type: ignore
-    keep_metrics = keep_metrics or run_metrics.keys()
-    for metric_name, metric_val in run_metrics.items():
-        if metric_name in keep_metrics:
-            metrics[metric_name] = metric_val
-    df = pd.DataFrame.from_dict(metrics, orient="index")
-    return df
+    for child_run in run.get_children():  # type: ignore
+        child_run_tag = get_tags_from_hyperdrive_run(child_run, child_run_arg_name)
+        child_run_metrics = get_metrics_for_run(run=child_run, keep_metrics=keep_metrics)
+        metrics[child_run_tag] = child_run_metrics
+    return metrics
 
 
 def download_files_from_hyperdrive_children(
     run: Run, remote_file_paths: str, local_download_folder: Path, hyperparam_name: str = ""
 ) -> List[str]:
     """
     Download a specified file or folder from each of the children of an Azure ML Hyperdrive run. For each child
@@ -1919,15 +1639,15 @@
     :param local_download_folder: The local folder to download the files to
     :param hyperparam_name: The name of one of the hyperparameters that was sampled during the HyperDrive
         run. This is used to ensure files are downloaded into logically-named folders
     :return: A list of paths to the downloaded files
     """
     if len(hyperparam_name) == 0:
         raise ValueError(
-            "To download results from a HyperDrive run you must provide the hyperparameter name" "that was sampled over"
+            "To download results from a HyperDrive run you must provide the hyperparameter name that was sampled over"
         )
 
     # For each child run we create a directory in the local_download_folder named after value of the
     # hyperparam sampled for this child.
     downloaded_file_paths = []
     for child_run in run.get_children():
         child_run_index = get_tags_from_hyperdrive_run(child_run, hyperparam_name)
@@ -1939,15 +1659,15 @@
         local_folder_child_run = local_download_folder / re.sub("[^A-Za-z0-9]+", "", str(child_run_index))
         local_folder_child_run.mkdir(exist_ok=True)
         for remote_file_path in remote_file_paths.split(","):
             download_files_from_run_id(child_run.id, local_folder_child_run, prefix=remote_file_path)
             downloaded_file_path = local_folder_child_run / remote_file_path
             if not downloaded_file_path.exists():
                 logging.warning(
-                    f"Unable to download the file {remote_file_path} from the datastore associated" "with this run."
+                    f"Unable to download the file {remote_file_path} from the datastore associated with this run."
                 )
             else:
                 downloaded_file_paths.append(str(downloaded_file_path))
 
     return downloaded_file_paths
 
 
@@ -2014,34 +1734,14 @@
     actual_workspace = get_workspace(aml_workspace=workspace, workspace_config_path=workspace_config_path)
     exp = Experiment(workspace=actual_workspace, name=experiment_name)
     if snapshot_directory is None or snapshot_directory == "":
         snapshot_directory = tempfile.mkdtemp()
     return exp.start_logging(display_name=run_name, snapshot_directory=str(snapshot_directory))  # type: ignore
 
 
-def aml_workspace_for_unittests() -> Workspace:
-    """
-    Gets the default AzureML workspace that is used for unit testing. It first tries to locate a workspace config.json
-    file in the present folder or its parents, and create a workspace from that if found. If no config.json file
-    is found, the workspace details are read from environment variables. Authentication information is also read
-    from environment variables.
-    """
-    config_json = find_file_in_parent_to_pythonpath(WORKSPACE_CONFIG_JSON)
-    if config_json is not None:
-        return Workspace.from_config(path=str(config_json))
-    else:
-        workspace_name = get_secret_from_environment(ENV_WORKSPACE_NAME, allow_missing=False)
-        subscription_id = get_secret_from_environment(ENV_SUBSCRIPTION_ID, allow_missing=False)
-        resource_group = get_secret_from_environment(ENV_RESOURCE_GROUP, allow_missing=False)
-        auth = get_authentication()
-        return Workspace.get(
-            name=workspace_name, auth=auth, subscription_id=subscription_id, resource_group=resource_group
-        )
-
-
 class UnitTestWorkspaceWrapper:
     """
     Wrapper around aml_workspace so that it is lazily loaded only once. Used for unit testing only.
     """
 
     def __init__(self) -> None:
         """
@@ -2051,15 +1751,15 @@
 
     @property
     def workspace(self) -> Workspace:
         """
         Lazily load the aml_workspace.
         """
         if self._workspace is None:
-            self._workspace = aml_workspace_for_unittests()
+            self._workspace = get_workspace()
         return self._workspace
 
 
 @contextmanager
 def check_config_json(script_folder: Path, shared_config_json: Path) -> Generator:
     """
     Create a workspace config.json file exists in the folder where we expect a test script. This is either copied
@@ -2084,20 +1784,22 @@
         resource_group = os.getenv(ENV_RESOURCE_GROUP, "")
         workspace_name = os.getenv(ENV_WORKSPACE_NAME, "")
         if subscription_id and resource_group and workspace_name:
             with open(str(target_config_json), 'w', encoding="utf-8") as file:
                 config = {
                     "subscription_id": subscription_id,
                     "resource_group": resource_group,
-                    "workspace_name": workspace_name
+                    "workspace_name": workspace_name,
                 }
                 json.dump(config, file)
         else:
-            raise ValueError("Either a shared config.json must be present, or all 3 environment variables for "
-                             "workspace creation must exist.")
+            raise ValueError(
+                "Either a shared config.json must be present, or all 3 environment variables for "
+                "workspace creation must exist."
+            )
     try:
         yield
     finally:
         if not target_config_exists:
             target_config_json.unlink()
 
 
@@ -2120,35 +1822,38 @@
     will succeed. Otherwise an exception will be raised
 
     :param credential: The credential object to validate.
     """
     credential.get_token("https://management.azure.com/.default")
 
 
-def _get_legitimate_service_principal_credential(tenant_id: str, service_principal_id: str,
-                                                 service_principal_password: str) -> TokenCredential:
+def _get_legitimate_service_principal_credential(
+    tenant_id: str, service_principal_id: str, service_principal_password: str
+) -> TokenCredential:
     """
     Create a ClientSecretCredential given a tenant id, service principal id and password
 
     :param tenant_id: The Azure tenant id.
     :param service_principal_id: The id of an existing Service Principal.
     :param service_principal_password: The password of an existing Service Principal.
     :raises ValueError: If the credential cannot be validated (i.e. authentication was unsucessful).
     :return: The validated credential.
     """
-    cred = ClientSecretCredential(tenant_id=tenant_id,
-                                  client_id=service_principal_id,
-                                  client_secret=service_principal_password)
+    cred = ClientSecretCredential(
+        tenant_id=tenant_id, client_id=service_principal_id, client_secret=service_principal_password
+    )
     try:
         _validate_credential(cred)
         return cred
     except ClientAuthenticationError as e:
-        raise ValueError(f"Found environment variables for {ENV_SERVICE_PRINCIPAL_ID}, "
-                         f"{ENV_SERVICE_PRINCIPAL_PASSWORD}, and {ENV_TENANT_ID} but was "
-                         f"not able to authenticate: {e}")
+        raise ValueError(
+            f"Found environment variables for {ENV_SERVICE_PRINCIPAL_ID}, "
+            f"{ENV_SERVICE_PRINCIPAL_PASSWORD}, and {ENV_TENANT_ID} but was "
+            f"not able to authenticate: {e}"
+        )
 
 
 def _get_legitimate_device_code_credential() -> Optional[TokenCredential]:
     """
     Create a DeviceCodeCredential for interacting with Azure resources. If the credential can't be
     validated, return None.
 
@@ -2160,25 +1865,21 @@
         return cred
     except ClientAuthenticationError:
         return None
 
 
 def _get_legitimate_default_credential() -> Optional[TokenCredential]:
     """
-    Create a DefaultAzure credential for interacting with Azure resources. If the credential can't be
-    validated, return None.
+    Create a DefaultAzure credential for interacting with Azure resources and validates it.
 
     :return: A valid Azure credential.
     """
     cred = DefaultAzureCredential(timeout=60)
-    try:
-        _validate_credential(cred)
-        return cred
-    except ClientAuthenticationError:
-        return None
+    _validate_credential(cred)
+    return cred
 
 
 def _get_legitimate_interactive_browser_credential() -> Optional[TokenCredential]:
     """
     Create an InteractiveBrowser credential for interacting with Azure resources. If the credential can't be
     validated, return None.
 
@@ -2220,25 +1921,28 @@
         if cred is not None:
             return cred
 
         cred = _get_legitimate_interactive_browser_credential()
         if cred is not None:
             return cred
 
-    raise ValueError("Unable to generate and validate a credential. Please see Azure ML documentation"
-                     "for instructions on diffrent options to get a credential")
+    raise ValueError(
+        "Unable to generate and validate a credential. Please see Azure ML documentation"
+        "for instructions on diffrent options to get a credential"
+    )
 
 
-def get_ml_client(ml_client: Optional[MLClient] = None,
-                  aml_workspace: Optional[Workspace] = None,
-                  workspace_config_path: Optional[PathOrString] = None,
-                  subscription_id: Optional[str] = None,
-                  resource_group: Optional[str] = None,
-                  workspace_name: str = "",
-                  ) -> MLClient:
+def get_ml_client(
+    ml_client: Optional[MLClient] = None,
+    aml_workspace: Optional[Workspace] = None,
+    workspace_config_path: Optional[PathOrString] = None,
+    subscription_id: Optional[str] = None,
+    resource_group: Optional[str] = None,
+    workspace_name: str = "",
+) -> MLClient:
     """
     Instantiate an MLClient for interacting with Azure resources via v2 of the Azure ML SDK.
     If a ml_client is provided, return that. Otherwise, create one using workspace details
     coming from either an existing Workspace object, a config.json file or passed in as an argument.
 
     :param ml_client: An optional existing MLClient object to be returned.
     :param aml_workspace: An optional Workspace object to take connection details from.
@@ -2255,41 +1959,41 @@
     if credential is None:
         raise ValueError("Can't connect to MLClient without a valid credential")
     if aml_workspace is not None:
         ml_client = MLClient(
             subscription_id=aml_workspace.subscription_id,
             resource_group_name=aml_workspace.resource_group,
             workspace_name=aml_workspace.name,
-            credential=credential)  # type: ignore
+            credential=credential,
+        )  # type: ignore
     elif workspace_config_path:
-        ml_client = MLClient.from_config(
-            credential=credential,  # type: ignore
-            path=str(workspace_config_path))
+        ml_client = MLClient.from_config(credential=credential, path=str(workspace_config_path))  # type: ignore
     elif subscription_id and resource_group and workspace_name:
         ml_client = MLClient(
             subscription_id=subscription_id,
             resource_group_name=resource_group,
             workspace_name=workspace_name,
-            credential=credential)  # type: ignore
+            credential=credential,
+        )  # type: ignore
     else:
         try:
             workspace = get_workspace()
             ml_client = MLClient(
                 subscription_id=workspace.subscription_id,
                 resource_group_name=workspace.resource_group,
                 workspace_name=workspace.name,
-                credential=credential)  # type: ignore
+                credential=credential,
+            )  # type: ignore
         except ValueError as e:
             raise ValueError(f"Couldn't connect to MLClient: {e}")
     logging.info(f"Logged into AzureML workspace {ml_client.workspace_name}")
     return ml_client
 
 
-def retrieve_workspace_from_client(ml_client: MLClient, workspace_name: Optional[str] = None
-                                   ) -> WorkspaceV2:
+def retrieve_workspace_from_client(ml_client: MLClient, workspace_name: Optional[str] = None) -> WorkspaceV2:
     """
     Get a v2 Workspace object from an MLClient object. If a workspace_name is passed, will attempt
     to retrieve a workspace with that name. Otherweise will use the MLClient's default workspace_name
 
     :param ml_client: An MLClient object to retrieve the Workspace from
     :param workspace_name: An optional name of the workspace to retrieve.
     :return: A v2 Workspace object.
@@ -2322,9 +2026,8 @@
     pass input and output arguments to a script via the command line, of which there can be an unknown number.
     Therefore we need to remove these from the list of args passed to the argument parsers.
 
     :param args: A list of arguments from which to remove input and output args
     :return: A filtered list of arguments, without entries in the format of INPUT_i or OUTPUT_i where i is
         any integer.
     """
-    return [a for a in args if
-            not re.match(V2_INPUT_DATASET_PATTERN, a) and not re.match(V2_OUTPUT_DATASET_PATTERN, a)]
+    return [a for a in args if not re.match(V2_INPUT_DATASET_PATTERN, a) and not re.match(V2_OUTPUT_DATASET_PATTERN, a)]
```

### Comparing `hi-ml-azure-0.2.9/src/hi_ml_azure.egg-info/PKG-INFO` & `hi-ml-azure-0.3.0/src/hi_ml_azure.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hi-ml-azure
-Version: 0.2.9
+Version: 0.3.0
 Summary: Microsoft Health Futures package to elevate and monitor scripts to an AzureML workspace
 Home-page: https://github.com/microsoft/hi-ml
 Author: Biomedical Imaging Team @ Microsoft Health Futures
 Author-email: innereyedev@microsoft.com
 License: MIT License
 Description: # Microsoft Health Intelligence Machine Learning Azure Toolbox
```

### Comparing `hi-ml-azure-0.2.9/src/hi_ml_azure.egg-info/SOURCES.txt` & `hi-ml-azure-0.3.0/src/hi_ml_azure.egg-info/SOURCES.txt`

 * *Files 21% similar despite different names*

```diff
@@ -1,20 +1,22 @@
 LICENSE
 MANIFEST.in
 package_description.md
 run_requirements.txt
 setup.py
 src/health_azure/__init__.py
 src/health_azure/amulet.py
+src/health_azure/argparsing.py
 src/health_azure/datasets.py
 src/health_azure/himl.py
 src/health_azure/himl_download.py
 src/health_azure/himl_tensorboard.py
 src/health_azure/logging.py
 src/health_azure/mlflow_utils.py
+src/health_azure/package_setup.py
 src/health_azure/paths.py
 src/health_azure/traverse.py
 src/health_azure/utils.py
 src/health_azure/examples/elevate_this.py
 src/hi_ml_azure.egg-info/PKG-INFO
 src/hi_ml_azure.egg-info/SOURCES.txt
 src/hi_ml_azure.egg-info/dependency_links.txt
```

