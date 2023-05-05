# Comparing `tmp/picsellia-6.6.0.tar.gz` & `tmp/picsellia-6.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "picsellia-6.6.0.tar", max compression
+gzip compressed data, was "picsellia-6.7.0.tar", max compression
```

## Comparing `picsellia-6.6.0.tar` & `picsellia-6.7.0.tar`

### file list

```diff
@@ -1,59 +1,62 @@
--rw-r--r--   0        0        0     8562 2023-04-06 12:19:37.409909 picsellia-6.6.0/CHANGELOG.md
--rw-r--r--   0        0        0     1074 2023-01-12 16:30:19.323635 picsellia-6.6.0/LICENSE
--rw-r--r--   0        0        0     1660 2023-04-03 08:29:20.904735 picsellia-6.6.0/README.md
--rw-r--r--   0        0        0     2590 2023-04-06 12:19:37.410211 picsellia-6.6.0/picsellia/__init__.py
--rw-r--r--   0        0        0    36033 2023-04-04 18:32:38.389566 picsellia-6.6.0/picsellia/client.py
--rw-r--r--   0        0        0      267 2022-12-27 14:36:57.989829 picsellia-6.6.0/picsellia/colors.py
--rw-r--r--   0        0        0     1706 2023-03-14 20:30:26.541657 picsellia-6.6.0/picsellia/decorators.py
--rw-r--r--   0        0        0     4805 2023-04-03 08:29:46.246452 picsellia-6.6.0/picsellia/exceptions.py
--rw-r--r--   0        0        0     3410 2023-03-14 10:34:40.324186 picsellia-6.6.0/picsellia/pxl_multithreading.py
--rw-r--r--   0        0        0        0 2022-02-27 20:17:17.529743 picsellia-6.6.0/picsellia/sdk/__init__.py
--rw-r--r--   0        0        0    21739 2023-02-22 18:00:24.947168 picsellia-6.6.0/picsellia/sdk/annotation.py
--rw-r--r--   0        0        0     3086 2023-04-03 08:29:46.246763 picsellia-6.6.0/picsellia/sdk/artifact.py
--rw-r--r--   0        0        0    16419 2023-04-03 08:29:46.246961 picsellia-6.6.0/picsellia/sdk/asset.py
--rw-r--r--   0        0        0     2509 2023-02-22 18:00:24.947763 picsellia-6.6.0/picsellia/sdk/classification.py
--rw-r--r--   0        0        0    19375 2023-04-03 08:29:46.247345 picsellia-6.6.0/picsellia/sdk/connexion.py
--rw-r--r--   0        0        0     1986 2023-02-22 18:00:24.947871 picsellia-6.6.0/picsellia/sdk/dao.py
--rw-r--r--   0        0        0     8470 2023-04-03 08:29:46.247535 picsellia-6.6.0/picsellia/sdk/data.py
--rw-r--r--   0        0        0    16868 2023-04-03 08:29:20.905885 picsellia-6.6.0/picsellia/sdk/datalake.py
--rw-r--r--   0        0        0     7127 2023-02-22 18:00:24.948727 picsellia-6.6.0/picsellia/sdk/dataset.py
--rw-r--r--   0        0        0    55723 2023-04-03 08:29:46.247881 picsellia-6.6.0/picsellia/sdk/dataset_version.py
--rw-r--r--   0        0        0     2113 2023-02-22 18:00:24.949197 picsellia-6.6.0/picsellia/sdk/datasource.py
--rw-r--r--   0        0        0    30514 2023-04-03 08:29:20.906404 picsellia-6.6.0/picsellia/sdk/deployment.py
--rw-r--r--   0        0        0     3480 2023-04-03 08:29:46.248107 picsellia-6.6.0/picsellia/sdk/downloadable.py
--rw-r--r--   0        0        0     4219 2023-04-04 18:32:38.389828 picsellia-6.6.0/picsellia/sdk/evaluation.py
--rw-r--r--   0        0        0    40686 2023-04-04 18:32:38.390254 picsellia-6.6.0/picsellia/sdk/experiment.py
--rw-r--r--   0        0        0     8130 2023-03-15 14:14:18.181467 picsellia-6.6.0/picsellia/sdk/job.py
--rw-r--r--   0        0        0     2096 2023-02-22 18:00:24.949930 picsellia-6.6.0/picsellia/sdk/label.py
--rw-r--r--   0        0        0     2871 2023-02-22 18:00:24.950036 picsellia-6.6.0/picsellia/sdk/line.py
--rw-r--r--   0        0        0     3473 2023-02-22 18:00:24.950135 picsellia-6.6.0/picsellia/sdk/log.py
--rw-r--r--   0        0        0     2720 2023-04-03 08:29:46.248342 picsellia-6.6.0/picsellia/sdk/logging_file.py
--rw-r--r--   0        0        0     7097 2023-02-22 18:00:24.950717 picsellia-6.6.0/picsellia/sdk/model.py
--rw-r--r--   0        0        0     5061 2023-02-22 18:00:24.950847 picsellia-6.6.0/picsellia/sdk/model_context.py
--rw-r--r--   0        0        0     2163 2023-04-03 08:29:46.248517 picsellia-6.6.0/picsellia/sdk/model_file.py
--rw-r--r--   0        0        0    11668 2023-03-10 16:25:34.204784 picsellia-6.6.0/picsellia/sdk/model_version.py
--rw-r--r--   0        0        0     4453 2023-01-12 16:30:19.325619 picsellia-6.6.0/picsellia/sdk/multi_object.py
--rw-r--r--   0        0        0     3024 2023-02-22 18:00:24.951455 picsellia-6.6.0/picsellia/sdk/point.py
--rw-r--r--   0        0        0     2926 2023-02-22 18:00:24.951556 picsellia-6.6.0/picsellia/sdk/polygon.py
--rw-r--r--   0        0        0    16760 2023-02-22 18:00:24.951727 picsellia-6.6.0/picsellia/sdk/project.py
--rw-r--r--   0        0        0     3403 2023-02-22 18:00:24.951872 picsellia-6.6.0/picsellia/sdk/rectangle.py
--rw-r--r--   0        0        0     5374 2023-02-22 18:00:24.951983 picsellia-6.6.0/picsellia/sdk/run.py
--rw-r--r--   0        0        0     6864 2023-02-22 18:00:24.952106 picsellia-6.6.0/picsellia/sdk/scan.py
--rw-r--r--   0        0        0     2957 2023-04-03 08:29:46.248678 picsellia-6.6.0/picsellia/sdk/scan_file.py
--rw-r--r--   0        0        0     4417 2023-02-22 18:00:24.952304 picsellia-6.6.0/picsellia/sdk/tag.py
--rw-r--r--   0        0        0     2959 2023-02-22 18:00:24.952399 picsellia-6.6.0/picsellia/sdk/taggable.py
--rw-r--r--   0        0        0     1492 2023-02-22 18:00:24.952484 picsellia-6.6.0/picsellia/sdk/worker.py
--rw-r--r--   0        0        0        0 2023-02-22 18:00:24.952511 picsellia-6.6.0/picsellia/services/__init__.py
--rw-r--r--   0        0        0     5988 2023-03-10 10:48:31.499966 picsellia-6.6.0/picsellia/services/coco_file_builder.py
--rw-r--r--   0        0        0     3558 2023-03-14 17:44:09.190594 picsellia-6.6.0/picsellia/services/coco_importer.py
--rw-r--r--   0        0        0     1941 2023-02-22 18:00:24.952711 picsellia-6.6.0/picsellia/services/datasource.py
--rw-r--r--   0        0        0      798 2023-03-15 14:13:21.588639 picsellia-6.6.0/picsellia/services/error_manager.py
--rw-r--r--   0        0        0     2658 2023-03-14 17:44:09.190754 picsellia-6.6.0/picsellia/services/voc_importer.py
--rw-r--r--   0        0        0     8268 2023-03-15 14:13:21.588900 picsellia-6.6.0/picsellia/services/yolo_importer.py
--rw-r--r--   0        0        0        0 2022-02-27 20:17:17.531530 picsellia-6.6.0/picsellia/types/__init__.py
--rw-r--r--   0        0        0     4363 2023-04-04 18:32:38.390686 picsellia-6.6.0/picsellia/types/enums.py
--rw-r--r--   0        0        0     4344 2023-04-04 18:32:38.391325 picsellia-6.6.0/picsellia/types/schemas.py
--rw-r--r--   0        0        0     3638 2022-12-27 14:36:57.996751 picsellia-6.6.0/picsellia/types/schemas_prediction.py
--rw-r--r--   0        0        0     8498 2023-03-15 10:31:12.587373 picsellia-6.6.0/picsellia/utils.py
--rw-r--r--   0        0        0     1368 2023-04-06 12:19:37.412124 picsellia-6.6.0/pyproject.toml
--rw-r--r--   0        0        0     3153 1970-01-01 00:00:00.000000 picsellia-6.6.0/PKG-INFO
+-rw-r--r--   0        0        0     9562 2023-05-05 17:03:12.733755 picsellia-6.7.0/CHANGELOG.md
+-rw-r--r--   0        0        0     1074 2023-03-15 15:46:10.361461 picsellia-6.7.0/LICENSE
+-rw-r--r--   0        0        0     1660 2023-04-27 07:58:44.075996 picsellia-6.7.0/README.md
+-rw-r--r--   0        0        0     2590 2023-05-05 17:03:12.733755 picsellia-6.7.0/picsellia/__init__.py
+-rw-r--r--   0        0        0    38919 2023-05-05 16:13:24.340832 picsellia-6.7.0/picsellia/client.py
+-rw-r--r--   0        0        0      267 2022-10-18 10:06:13.118336 picsellia-6.7.0/picsellia/colors.py
+-rw-r--r--   0        0        0     1706 2023-04-06 07:00:27.239227 picsellia-6.7.0/picsellia/decorators.py
+-rw-r--r--   0        0        0     4805 2023-04-27 07:58:44.079995 picsellia-6.7.0/picsellia/exceptions.py
+-rw-r--r--   0        0        0     3410 2023-04-06 07:00:27.239227 picsellia-6.7.0/picsellia/pxl_multithreading.py
+-rw-r--r--   0        0        0        0 2022-08-09 13:11:44.816343 picsellia-6.7.0/picsellia/sdk/__init__.py
+-rw-r--r--   0        0        0    21739 2023-03-15 15:46:10.365461 picsellia-6.7.0/picsellia/sdk/annotation.py
+-rw-r--r--   0        0        0     3227 2023-05-05 16:13:24.344832 picsellia-6.7.0/picsellia/sdk/artifact.py
+-rw-r--r--   0        0        0    16881 2023-05-05 16:54:06.773495 picsellia-6.7.0/picsellia/sdk/asset.py
+-rw-r--r--   0        0        0     2509 2023-03-15 15:46:10.365461 picsellia-6.7.0/picsellia/sdk/classification.py
+-rw-r--r--   0        0        0    19558 2023-05-05 16:13:24.344832 picsellia-6.7.0/picsellia/sdk/connexion.py
+-rw-r--r--   0        0        0     1986 2023-03-15 15:46:10.365461 picsellia-6.7.0/picsellia/sdk/dao.py
+-rw-r--r--   0        0        0     9082 2023-05-05 16:54:06.773495 picsellia-6.7.0/picsellia/sdk/data.py
+-rw-r--r--   0        0        0    16868 2023-05-02 14:54:36.755267 picsellia-6.7.0/picsellia/sdk/datalake.py
+-rw-r--r--   0        0        0     7203 2023-05-05 16:13:24.344832 picsellia-6.7.0/picsellia/sdk/dataset.py
+-rw-r--r--   0        0        0    60055 2023-05-05 16:54:06.773495 picsellia-6.7.0/picsellia/sdk/dataset_version.py
+-rw-r--r--   0        0        0     2113 2023-03-15 15:46:10.369461 picsellia-6.7.0/picsellia/sdk/datasource.py
+-rw-r--r--   0        0        0    30514 2023-05-04 07:34:02.705466 picsellia-6.7.0/picsellia/sdk/deployment.py
+-rw-r--r--   0        0        0     3485 2023-05-05 16:13:24.344832 picsellia-6.7.0/picsellia/sdk/downloadable.py
+-rw-r--r--   0        0        0     4219 2023-04-27 07:58:44.083995 picsellia-6.7.0/picsellia/sdk/evaluation.py
+-rw-r--r--   0        0        0    40686 2023-04-27 07:58:44.083995 picsellia-6.7.0/picsellia/sdk/experiment.py
+-rw-r--r--   0        0        0     8130 2023-04-06 07:00:27.251227 picsellia-6.7.0/picsellia/sdk/job.py
+-rw-r--r--   0        0        0     2096 2023-03-15 15:46:10.373461 picsellia-6.7.0/picsellia/sdk/label.py
+-rw-r--r--   0        0        0     2871 2023-03-15 15:46:10.373461 picsellia-6.7.0/picsellia/sdk/line.py
+-rw-r--r--   0        0        0     3473 2023-03-15 15:46:10.373461 picsellia-6.7.0/picsellia/sdk/log.py
+-rw-r--r--   0        0        0     2872 2023-05-05 16:13:24.344832 picsellia-6.7.0/picsellia/sdk/logging_file.py
+-rw-r--r--   0        0        0     8598 2023-05-05 16:13:24.344832 picsellia-6.7.0/picsellia/sdk/model.py
+-rw-r--r--   0        0        0     5061 2023-03-15 15:46:10.373461 picsellia-6.7.0/picsellia/sdk/model_context.py
+-rw-r--r--   0        0        0     2311 2023-05-05 16:13:24.344832 picsellia-6.7.0/picsellia/sdk/model_file.py
+-rw-r--r--   0        0        0    12795 2023-05-05 16:13:24.344832 picsellia-6.7.0/picsellia/sdk/model_version.py
+-rw-r--r--   0        0        0     4453 2023-05-05 09:14:03.113478 picsellia-6.7.0/picsellia/sdk/multi_object.py
+-rw-r--r--   0        0        0     3024 2023-03-15 15:46:10.373461 picsellia-6.7.0/picsellia/sdk/point.py
+-rw-r--r--   0        0        0     2926 2023-03-15 15:46:10.373461 picsellia-6.7.0/picsellia/sdk/polygon.py
+-rw-r--r--   0        0        0    16844 2023-05-05 16:13:24.344832 picsellia-6.7.0/picsellia/sdk/project.py
+-rw-r--r--   0        0        0     3403 2023-03-15 15:46:10.377461 picsellia-6.7.0/picsellia/sdk/rectangle.py
+-rw-r--r--   0        0        0     5374 2023-03-15 15:46:10.377461 picsellia-6.7.0/picsellia/sdk/run.py
+-rw-r--r--   0        0        0     6923 2023-05-05 16:13:24.344832 picsellia-6.7.0/picsellia/sdk/scan.py
+-rw-r--r--   0        0        0     3103 2023-05-05 16:13:24.344832 picsellia-6.7.0/picsellia/sdk/scan_file.py
+-rw-r--r--   0        0        0     4417 2023-03-15 15:46:10.377461 picsellia-6.7.0/picsellia/sdk/tag.py
+-rw-r--r--   0        0        0     2959 2023-03-15 15:46:10.377461 picsellia-6.7.0/picsellia/sdk/taggable.py
+-rw-r--r--   0        0        0     1492 2023-03-15 15:46:10.377461 picsellia-6.7.0/picsellia/sdk/worker.py
+-rw-r--r--   0        0        0        0 2023-03-15 15:46:10.377461 picsellia-6.7.0/picsellia/services/__init__.py
+-rw-r--r--   0        0        0     2112 2023-05-05 16:54:06.773495 picsellia-6.7.0/picsellia/services/asset_splitter.py
+-rw-r--r--   0        0        0     5988 2023-03-15 15:46:10.377461 picsellia-6.7.0/picsellia/services/coco_file_builder.py
+-rw-r--r--   0        0        0     3558 2023-04-06 07:00:27.251227 picsellia-6.7.0/picsellia/services/coco_importer.py
+-rw-r--r--   0        0        0     1941 2023-03-15 15:46:10.377461 picsellia-6.7.0/picsellia/services/datasource.py
+-rw-r--r--   0        0        0      798 2023-04-06 07:00:27.251227 picsellia-6.7.0/picsellia/services/error_manager.py
+-rw-r--r--   0        0        0      974 2023-05-05 16:54:06.773495 picsellia-6.7.0/picsellia/services/splitter.py
+-rw-r--r--   0        0        0     2658 2023-04-06 07:00:27.251227 picsellia-6.7.0/picsellia/services/voc_importer.py
+-rw-r--r--   0        0        0     8268 2023-04-06 07:00:27.251227 picsellia-6.7.0/picsellia/services/yolo_importer.py
+-rw-r--r--   0        0        0        0 2022-08-09 13:11:44.820343 picsellia-6.7.0/picsellia/types/__init__.py
+-rw-r--r--   0        0        0     4363 2023-04-27 07:58:44.087996 picsellia-6.7.0/picsellia/types/enums.py
+-rw-r--r--   0        0        0     4535 2023-05-05 16:54:06.773495 picsellia-6.7.0/picsellia/types/schemas.py
+-rw-r--r--   0        0        0     3658 2023-05-05 16:13:24.348832 picsellia-6.7.0/picsellia/types/schemas_prediction.py
+-rw-r--r--   0        0        0     8498 2023-05-03 14:48:53.249272 picsellia-6.7.0/picsellia/utils.py
+-rw-r--r--   0        0        0     1368 2023-05-05 17:03:12.733755 picsellia-6.7.0/pyproject.toml
+-rw-r--r--   0        0        0     2757 1970-01-01 00:00:00.000000 picsellia-6.7.0/setup.py
+-rw-r--r--   0        0        0     3153 1970-01-01 00:00:00.000000 picsellia-6.7.0/PKG-INFO
```

### Comparing `picsellia-6.6.0/CHANGELOG.md` & `picsellia-6.7.0/CHANGELOG.md`

 * *Files 10% similar despite different names*

```diff
@@ -1,17 +1,36 @@
 
 # Changelog
 
 Picsellia SDK Python is a library that allows users to connect to Picsellia backend.
 
 All notable changes to this project will be documented in this file.
 
+## [6.7.0] - 2023-05-05
+
+### Added
+- Add `Client.create_deployment()` to create a deployment. Allow user to create it without using Picsellia Serving
+- Add `DatasetVersion.retrieve_stats()` to retrieve stats of your dataset version
+- Add `DatasetVersion.train_test_val_split()` to split a dataset version into 3 different multi assets
+- Add `DatasetVersion.split_into_multi_assets()` to split a dataset version into N multi assets and return their label repartition
+- Add `MultiData.split()` and `MultiAsset.split()` to split from a given ratio a multi asset
+- Add User-Agent with picsellia version in headers of requests
+
+### Changed
+- Framework and type of Model are now configurable into ModelVersion
+- Get by id now use parent API to ensures object are in the same organization as the one connected
+- Methods manipulating tags on client are now calling other routes
+- Some minor fixes on documentation
+
+### Fixed
+- Segmentation format used in `monitor()` was not supported by monitoring service
+
 
 
-## [6.5.0] - 2023-04-06
+## [6.6.0] - 2023-04-06
 
 ### Added
 - `list_data` and `list_assets` have a new parameter `q` that can be used the same way the query language is used in the web platform
 - Deployment has new methods: `set_training_data`, `check_training_data_metrics_status` and `disable_training_data_reference`, that can be used for monitoring and unsupervised metrics.
 - `as_multidata` of MultiAsset can now be called with parameter
 - Artifact, Data, Asset, LoggingFile, ScanFile, ModelFile are now inheriting from Downloadable, and have `url` property that can be used to download files. These urls are presigned and expired at some point in the future.
 - Methods `add_evaluation`, `list_evaluations` and `compute_evaluations_metrics` of Experiment can be used to add, list and compute evaluation of an Experiment
```

### Comparing `picsellia-6.6.0/LICENSE` & `picsellia-6.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `picsellia-6.6.0/README.md` & `picsellia-6.7.0/README.md`

 * *Files identical despite different names*

### Comparing `picsellia-6.6.0/picsellia/__init__.py` & `picsellia-6.7.0/picsellia/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = "6.6.0"
+__version__ = "6.7.0"
 
 import logging.config
 import os
 
 from picsellia.client import Client
 from picsellia.sdk.annotation import Annotation
 from picsellia.sdk.artifact import Artifact
```

### Comparing `picsellia-6.6.0/picsellia/client.py` & `picsellia-6.7.0/picsellia/client.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 from uuid import UUID
 
 import orjson
 from beartype import beartype
 from beartype.roar import BeartypeDecorHintPep585DeprecationWarning
 
 import picsellia
+from picsellia import utils
 from picsellia.colors import Colors
 from picsellia.decorators import exception_handler
 from picsellia.exceptions import PicselliaError
 from picsellia.sdk.connexion import Connexion
 from picsellia.sdk.datalake import Datalake
 from picsellia.sdk.dataset import Dataset
 from picsellia.sdk.dataset_version import DatasetVersion
@@ -286,15 +287,18 @@
             id (str): id of the dataset to retrieve
 
         Returns:
             A (Dataset) that you can use and manipulate
         """
         if isinstance(id, str):
             id = UUID(id)
-        r = self.connexion.get(f"/sdk/dataset/{id}").json()
+        params = {"id": id}
+        r = self.connexion.get(
+            f"/sdk/organization/{self.id}/datasets/find", params=params
+        ).json()
         return Dataset(self.connexion, r)
 
     @exception_handler
     @beartype
     def list_datasets(
         self,
         limit: Optional[int] = None,
@@ -332,24 +336,27 @@
             id (str or UUID): id of the dataset version to retrieve
 
         Returns:
             A (DatasetVersion)
         """
         if isinstance(id, str):
             id = UUID(id)
-        r = self.connexion.get(f"/sdk/dataset/version/{id}").json()
+        params = {"id": id}
+        r = self.connexion.get(
+            f"/sdk/organization/{self.id}/datasetversions/find", params=params
+        ).json()
         return DatasetVersion(self.connexion, r)
 
     @exception_handler
     @beartype
     def create_model(
         self,
         name: str,
-        type: Union[str, InferenceType],
-        framework: Union[str, Framework] = Framework.TENSORFLOW,
+        type: Union[str, InferenceType] = None,
+        framework: Union[str, Framework] = None,
         private: bool = True,
         description: str = "A brand new model!",
     ) -> Model:
         """Create a new model.
 
         Arguments:
             name (str): Model name to create.
@@ -358,39 +365,38 @@
             private (bool): A public model can be seen by everyone. Defaults to true.
             description (str): Description of this model
 
 
         Returns:
             A (Model) object that you can manipulate
         """
-        type = InferenceType.validate(type)
-        if type not in [
-            InferenceType.NOT_CONFIGURED,
-            InferenceType.OBJECT_DETECTION,
-            InferenceType.SEGMENTATION,
-            InferenceType.CLASSIFICATION,
-        ]:
-            raise TypeError(f"Type {type} is not supported yet")
+        if type:
+            logging.warning(
+                "'type' parameter is deprecated and will be removed in future versions. "
+                "If you want to give a type to your model version, call update() on ModelVersion."
+            )
 
-        framework = Framework.validate(framework)
+        if framework:
+            logging.warning(
+                "'framework' parameter is deprecated and will be removed in future versions. "
+                "If you want to give a framework to your model version, call update() on your ModelVersion."
+            )
 
         payload = {
             "name": name,
-            "type": type,
-            "framework": framework,
             "private": private,
             "description": description,
         }
         r = self.connexion.post(
             f"/sdk/organization/{self.id}/models",
             data=orjson.dumps(payload),
         ).json()
         created_model = Model(self.connexion, r)
         logger.info(
-            f"📚 Model {created_model.name} created\n📊 Type: {created_model.type.name}\n🌐 Platform url: {created_model.get_resource_url_on_platform()}"
+            f"📚 Model {created_model.name} created\n📊 🌐 Platform url: {created_model.get_resource_url_on_platform()}"
         )
         return created_model
 
     @exception_handler
     @beartype
     def get_model_by_id(self, id: Union[UUID, str]) -> Model:
         """Retrieve a model by its id
@@ -403,15 +409,18 @@
             id (str): id of the model that you are looking for
 
         Returns:
             A (Model) object that you can manipulate
         """
         if isinstance(id, str):
             id = UUID(id)
-        r = self.connexion.get(f"/sdk/model/{id}").json()
+        params = {"id": id}
+        r = self.connexion.get(
+            f"/sdk/organization/{self.id}/models/find", params=params
+        ).json()
         return Model(self.connexion, r)
 
     def _do_get_model_by_name(self, url: str, name: str):
         params = {"name": name}
         r = self.connexion.get(url, params=params).json()
         return Model(self.connexion, r)
 
@@ -501,36 +510,32 @@
                 Defaults to None, all public models will be retrieved.
             offset (int, optional): Offset to begin with when listing public models.
                 Defaults to None, starting at 0.
             order_by (List[str], optional): Some fields to order models against.
                 Defaults to None, models will not be sorted
             name (str, optional): A name to filter public models. It will return models with name *containing*
                 this parameter. Defaults to None, models will not be filtered
-            type (str or InferenceType, optional): A type to filter public models. It will return models with this type.
-                Defaults to None, models will not be filtered.
 
         Examples:
             ```python
-            public_detection_models = client.list_public_models(type=InferenceType.OBJECT_DETECTION)
+            public_detection_models = client.list_public_models(name="yolo")
             ```
 
         Returns:
             A list of all public (Model) objects
         """
-        # Usage of enum value is needed because params will not be serialized and InferenceType is an enum
         if type:
-            if isinstance(type, str):
-                type = InferenceType(type)
-            type = type.value
+            logging.warning(
+                "'type' parameter is deprecated and will be removed in future versions."
+            )
 
         params = {
             "limit": limit,
             "offset": offset,
             "order_by": order_by,
-            "type": type,
             "name": name,
         }
         return self._do_list_models("/sdk/public/models", params=params)
 
     @exception_handler
     @beartype
     def get_model_version_by_id(self, id: Union[UUID, str]) -> ModelVersion:
@@ -545,15 +550,18 @@
             id (str or UUID): id of the model version to retrieve
 
         Returns:
             A (ModelVersion)
         """
         if isinstance(id, str):
             id = UUID(id)
-        r = self.connexion.get(f"/sdk/model/version/{id}").json()
+        params = {"id": id}
+        r = self.connexion.get(
+            f"/sdk/organization/{self.id}/modelversions/find", params=params
+        ).json()
         return ModelVersion(self.connexion, r)
 
     @exception_handler
     @beartype
     def create_project(
         self, name: str, description: Optional[str] = None, private: bool = True
     ) -> Project:
@@ -628,15 +636,17 @@
             id (str): id of the project to retrieve
 
         Returns:
             A (Project) of your organization, you can manipulate to run experiments, or attach dataset
         """
         if isinstance(id, str):
             id = UUID(id)
-        r = self.connexion.get(f"/sdk/project/{id}").json()
+        r = self.connexion.get(
+            f"/sdk/organization/{self.id}/projects/find?id={id}"
+        ).json()
         return Project(self.connexion, r)
 
     @exception_handler
     @beartype
     def list_projects(
         self,
         limit: Optional[int] = None,
@@ -676,15 +686,19 @@
             id (str or UUID): id of the experiment to retrieve
 
         Returns:
             A (Experiment)
         """
         if isinstance(id, str):
             id = UUID(id)
-        r = self.connexion.get(f"/sdk/experiment/{id}").json()
+
+        params = {"id": id}
+        r = self.connexion.get(
+            f"/sdk/organization/{self.id}/experiments/find", params=params
+        ).json()
         return Experiment(self.connexion, r)
 
     @exception_handler
     @beartype
     def get_deployment(self, name: str) -> Deployment:
         """Get a (Deployment) from its name.
 
@@ -721,15 +735,18 @@
             id (str): deployment id displayed in your deployment settings.
 
         Returns:
             A (Deployment) object connected and authenticated to all the services.
         """
         if isinstance(id, str):
             id = UUID(id)
-        r = self.connexion.get(f"/sdk/deployment/{id}").json()
+        params = {"id": id}
+        r = self.connexion.get(
+            f"/sdk/organization/{self.id}/deployments/find", params=params
+        ).json()
         return Deployment(self.connexion, r)
 
     @exception_handler
     @beartype
     def list_deployments(
         self,
         limit: Optional[int] = None,
@@ -755,14 +772,73 @@
         r = self.connexion.get(
             f"/sdk/organization/{self.id}/deployments", params=params
         ).json()
         return list(map(partial(Deployment, self.connexion), r["items"]))
 
     @exception_handler
     @beartype
+    def create_deployment(
+        self,
+        model_version: ModelVersion,
+        shadow_model_version: Optional[ModelVersion] = None,
+        name: Optional[str] = None,
+        min_threshold: Optional[float] = None,
+        target_datalake: Optional[Datalake] = None,
+        disable_serving: Optional[bool] = False,
+    ):
+        """Create a (Deployment) from a model.
+
+        This method allows you to create a (Deployment) on Picsellia. You will then have
+        access to the monitoring dashboard and eventually a hosted endpoint.
+
+        Examples:
+            Create a serverless deployment
+            ```python
+            model = client.get_model(name="my-awesome-model")
+            deployment = model.create_deployment()
+            ```
+
+        Arguments:
+            model_version (ModelVersion): ModelVersion to deploy.
+            shadow_model_version (ModelVersion, optional): ModelVersion to perform shadow predictions.
+            name (str, optional): Name of your deployment. Defaults to a random name.
+            min_threshold (float, optional): Threshold of detection scores used by models when predicting. Defaults to 0.
+            target_datalake (Datalake, optional): Datalake to use when data are pushed into Picsellia.
+                Defaults to organization default Datalake.
+            disable_serving (bool, optional): Whether to not use Picsellia Serving. Defaults to False.
+
+
+        Returns:
+            A (Deployment)
+        """
+        from picsellia.sdk.deployment import Deployment
+
+        payload = {
+            "model_version_id": model_version.id,
+            "name": name,
+            "min_threshold": min_threshold,
+        }
+        if target_datalake is not None:
+            payload["target_datalake_id"] = target_datalake.id
+        if shadow_model_version:
+            payload["shadow_model_version_id"] = shadow_model_version.id
+        if disable_serving:
+            payload["disable_serving"] = disable_serving
+
+        filtered_payload = utils.filter_payload(payload)
+        r = self.connexion.post(
+            f"/sdk/organization/{self.id}/deployments",
+            data=orjson.dumps(filtered_payload),
+        ).json()
+        deployment = Deployment(self.connexion, r)
+        logger.info(f"{model_version} is deployed on {deployment}")
+        return deployment
+
+    @exception_handler
+    @beartype
     def create_datasource(self, name: str) -> DataSource:
         """Create a data source into this organization
 
         Examples:
             ```python
             data_source = client.create_datasource()
             ```
@@ -828,17 +904,17 @@
         return DataSourceService.list_datasources(
             self.connexion, self._id, limit, offset, order_by
         )
 
     @exception_handler
     @beartype
     def _create_tag_organization_scoped(self, name: str, target: TagTarget) -> Tag:
-        payload = {"name": name}
+        payload = {"name": name, "target_type": target}
         r = self.connexion.post(
-            f"/sdk/organization/{self.id}/{target.value}/tags",
+            f"/sdk/organization/{self.id}/tags",
             data=orjson.dumps(payload),
         ).json()
         return Tag(self.connexion, r)
 
     @exception_handler
     @beartype
     def create_dataset_tag(self, name: str) -> Tag:
@@ -923,18 +999,19 @@
             A (Tag) object
         """
         return self._create_tag_organization_scoped(name, TagTarget.DEPLOYMENT)
 
     @exception_handler
     @beartype
     def _list_tags_organization_scoped(self, target: TagTarget) -> List[Tag]:
+        params = {"target_type": target.value}
         r = self.connexion.get(
-            f"/sdk/organization/{self.id}/{target.value}/tags"
+            f"/sdk/organization/{self.id}/tags", params=params
         ).json()
-        return list(map(partial(Tag, self.connexion), r))
+        return list(map(partial(Tag, self.connexion), r["items"]))
 
     @exception_handler
     @beartype
     def list_dataset_tags(self) -> List[Tag]:
         """List all Dataset tags, usable only on Dataset objects
 
         Examples:
@@ -1006,17 +1083,17 @@
             A list of (Tag) objects
         """
         return self._list_tags_organization_scoped(TagTarget.DEPLOYMENT)
 
     @exception_handler
     @beartype
     def _find_tag_organization_scoped(self, target: TagTarget, name: str) -> Tag:
-        params = {"name": name}
+        params = {"name": name, "target_type": target.value}
         r = self.connexion.get(
-            f"/sdk/organization/{self.id}/{target.value}/tags/find",
+            f"/sdk/organization/{self.id}/tags/find",
             params=params,
         ).json()
         return Tag(self.connexion, r)
 
     @exception_handler
     @beartype
     def find_dataset_tag(self, name: str) -> Tag:
@@ -1107,9 +1184,12 @@
             id (str): deployment id displayed in your deployment settings.
 
         Returns:
             A (Job) object .
         """
         if isinstance(id, str):
             id = UUID(id)
-        r = self.connexion.get(f"/sdk/v2/job/{id}").json()
+        params = {"id": id}
+        r = self.connexion.get(
+            f"/sdk/organization/{self.id}/jobv2s/find", params=params
+        ).json()
         return Job(self.connexion, r, version=2)
```

### Comparing `picsellia-6.6.0/picsellia/decorators.py` & `picsellia-6.7.0/picsellia/decorators.py`

 * *Files identical despite different names*

### Comparing `picsellia-6.6.0/picsellia/exceptions.py` & `picsellia-6.7.0/picsellia/exceptions.py`

 * *Files identical despite different names*

### Comparing `picsellia-6.6.0/picsellia/pxl_multithreading.py` & `picsellia-6.7.0/picsellia/pxl_multithreading.py`

 * *Files identical despite different names*

### Comparing `picsellia-6.6.0/picsellia/sdk/annotation.py` & `picsellia-6.7.0/picsellia/sdk/annotation.py`

 * *Files identical despite different names*

### Comparing `picsellia-6.6.0/picsellia/sdk/artifact.py` & `picsellia-6.7.0/picsellia/sdk/artifact.py`

 * *Files 3% similar despite different names*

```diff
@@ -63,14 +63,19 @@
         r = self.connexion.get(f"/sdk/artifact/{self.id}").json()
         self.refresh(r)
         return r
 
     @exception_handler
     @beartype
     def reset_url(self) -> str:
+        """Reset url property of this Artifact by calling platform.
+
+        Returns:
+            A url as str of this Artifact.
+        """
         self._url = self.connexion.init_download(self.object_name)
         return self._url
 
     @exception_handler
     @beartype
     def update(
         self,
```

### Comparing `picsellia-6.6.0/picsellia/sdk/asset.py` & `picsellia-6.7.0/picsellia/sdk/asset.py`

 * *Files 2% similar despite different names*

```diff
@@ -119,14 +119,19 @@
         r = self.connexion.get(f"/sdk/asset/{self.id}").json()
         self.refresh(r)
         return r
 
     @exception_handler
     @beartype
     def reset_url(self) -> str:
+        """Reset url property of this Asset by calling platform.
+
+        Returns:
+            A url as str of this Asset.
+        """
         self.sync()
         return self._url
 
     @exception_handler
     @beartype
     def to_data_schema(self) -> ImageSchema:
         if self.type != DataType.IMAGE:  # pragma: no cover
@@ -348,14 +353,22 @@
         return self
 
     def copy(self) -> "MultiAsset":
         return MultiAsset(self.connexion, self.dataset_version_id, self.items.copy())
 
     @exception_handler
     @beartype
+    def split(self, ratio: float) -> Tuple["MultiAsset", "MultiAsset"]:
+        s = round(ratio * len(self.items))
+        return MultiAsset(
+            self.connexion, self.dataset_version_id, self.items[:s]
+        ), MultiAsset(self.connexion, self.dataset_version_id, self.items[s:])
+
+    @exception_handler
+    @beartype
     def delete(self) -> None:
         """Delete assets from their dataset
 
         :warning: **DANGER ZONE**: Be very careful here!
 
         Remove these assets and its annotation from the dataset it belongs
```

### Comparing `picsellia-6.6.0/picsellia/sdk/classification.py` & `picsellia-6.7.0/picsellia/sdk/classification.py`

 * *Files identical despite different names*

### Comparing `picsellia-6.6.0/picsellia/sdk/connexion.py` & `picsellia-6.7.0/picsellia/sdk/connexion.py`

 * *Files 1% similar despite different names*

```diff
@@ -11,14 +11,15 @@
 import requests
 from beartype import beartype
 from beartype.roar import BeartypeDecorHintPep585DeprecationWarning
 from picsellia_connexion_services import TokenServiceConnexion
 from requests.exceptions import ConnectionError
 
 import picsellia.exceptions as exceptions
+from picsellia import __version__
 from picsellia.decorators import exception_handler, retry
 from picsellia.types.enums import ObjectDataType
 from picsellia.utils import (
     handle_response,
     print_line_return,
     print_start_section,
     print_stop_section,
@@ -34,14 +35,15 @@
         self, host: str, api_token: str, content_type: str = "application/json"
     ) -> None:
         super().__init__(
             host, api_token, authorization_key="Bearer", content_type=content_type
         )
         self._connector_id = None
         self._organization_id = None
+        self.add_header("User-Agent", f"Picsellia-SDK/{__version__}")
 
     @property
     def connector_id(self):
         if self._connector_id is None:
             raise exceptions.NoConnectorFound(
                 "This organization has no default connector, and connect retrieve and upload files."
             )
@@ -54,17 +56,17 @@
     @property
     def organization_id(self):
         return self._organization_id
 
     @organization_id.setter
     def organization_id(self, value):
         self._organization_id = value
+        self.add_header("X-Picsellia-Organization", str(self._organization_id))
 
     def __eq__(self, __o: object) -> bool:
-
         if isinstance(__o, Connexion):
             return self.host == __o.host and self.api_token == __o.api_token
 
         return False
 
     @handle_response
     def get(self, path: str, params: Optional[dict] = None, stream=False):
```

### Comparing `picsellia-6.6.0/picsellia/sdk/dao.py` & `picsellia-6.7.0/picsellia/sdk/dao.py`

 * *Files identical despite different names*

### Comparing `picsellia-6.6.0/picsellia/sdk/data.py` & `picsellia-6.7.0/picsellia/sdk/data.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import logging
 import warnings
 from functools import partial
 from operator import countOf
 from pathlib import Path
-from typing import List, Optional, Union
+from typing import List, Optional, Tuple, Union
 from uuid import UUID
 
 import orjson
 from beartype import beartype
 from beartype.roar import BeartypeDecorHintPep585DeprecationWarning
 
 from picsellia import exceptions as exceptions
@@ -119,14 +119,19 @@
         r = self.connexion.get(f"/sdk/data/{self.id}").json()
         self.refresh(r)
         return r
 
     @exception_handler
     @beartype
     def reset_url(self) -> str:
+        """Reset url property of this Data by calling platform.
+
+        Returns:
+            A url as a string of this Data.
+        """
         self.sync()
         return self._url
 
     @exception_handler
     @beartype
     def get_tags(self) -> List[Tag]:
         """Retrieve the tags of your data.
@@ -142,14 +147,19 @@
         """
         r = self.sync()
         return list(map(partial(Tag, self.connexion), r["tags"]))
 
     @exception_handler
     @beartype
     def get_datasource(self) -> Optional[DataSource]:
+        """Retrieve (DataSource) of this Data if it exists. Else, will return None.
+
+        Returns:
+            A (DataSource) object or None.
+        """
         r = self.sync()
         if "data_source" not in r or r["data_source"] is None:
             return None
 
         return DataSource(self.connexion, r["data_source"])
 
     @exception_handler
@@ -215,24 +225,32 @@
         return self
 
     def copy(self) -> "MultiData":
         return MultiData(self.connexion, self.datalake_id, self.items.copy())
 
     @exception_handler
     @beartype
+    def split(self, ratio: float) -> Tuple["MultiData", "MultiData"]:
+        s = round(ratio * len(self.items))
+        return MultiData(self.connexion, self.datalake_id, self.items[:s]), MultiData(
+            self.connexion, self.datalake_id, self.items[s:]
+        )
+
+    @exception_handler
+    @beartype
     def delete(self) -> None:
         """Delete a bunch of data and remove them from datalake.
 
         :warning: **DANGER ZONE**: Be very careful here!
 
         Remove a bunch of data from datalake, and all assets linked to each data.
 
         Examples:
             ```python
-            whole_data = datalake.fetch_data(quantity=3)
+            whole_data = datalake.list_data(limit=3)
             whole_data.delete()
             ```
         """
         payload = self.ids
         self.connexion.delete(
             f"/sdk/datalake/{self.datalake_id}/datas",
             data=orjson.dumps(payload),
@@ -248,15 +266,15 @@
         max_workers: Optional[int] = None,
     ) -> None:
         """Download this multi data in given target path
 
 
         Examples:
             ```python
-            bunch_of_data = client.get_datalake().fetch_data(25)
+            bunch_of_data = client.get_datalake().list_data(limit=25)
             bunch_of_data.download('./downloads/')
             ```
         Arguments:
             target_path (str or Path, optional): Target path where to download. Defaults to './'.
             force_replace: (bool, optional): Replace an existing file if exists. Defaults to False.
             max_workers (int, optional): Number of max workers used to download. Defaults to os.cpu_count() + 4.
         """
```

### Comparing `picsellia-6.6.0/picsellia/sdk/datalake.py` & `picsellia-6.7.0/picsellia/sdk/datalake.py`

 * *Files identical despite different names*

### Comparing `picsellia-6.6.0/picsellia/sdk/dataset.py` & `picsellia-6.7.0/picsellia/sdk/dataset.py`

 * *Files 2% similar despite different names*

```diff
@@ -169,15 +169,18 @@
         Examples:
             ```python
             my_dataset_version = my_dataset.get_version("first")
             ```
         """
         if isinstance(id, str):
             id = UUID(id)
-        r = self.connexion.get(f"/sdk/dataset/version/{id}").json()
+        params = {"id": id}
+        r = self.connexion.get(
+            f"/sdk/dataset/{self.id}/versions/find", params=params
+        ).json()
         return DatasetVersion(self.connexion, r)
 
     @exception_handler
     @beartype
     def create_version(
         self,
         version: str,
```

### Comparing `picsellia-6.6.0/picsellia/sdk/dataset_version.py` & `picsellia-6.7.0/picsellia/sdk/dataset_version.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 import logging
 import os
-import random
 import warnings
 from functools import partial
 from pathlib import Path
 from typing import Any, Dict, List, Optional, Tuple, Union
 from uuid import UUID
 
 import orjson
@@ -27,22 +26,23 @@
 from picsellia.sdk.data import Data, MultiData
 from picsellia.sdk.job import Job
 from picsellia.sdk.label import Label
 from picsellia.sdk.tag import Tag, TagTarget
 from picsellia.sdk.taggable import Taggable
 from picsellia.sdk.worker import Worker
 from picsellia.services import coco_importer, voc_importer, yolo_importer
+from picsellia.services.asset_splitter import AssetSplitter
 from picsellia.services.coco_file_builder import COCOFileBuilder
 from picsellia.types.enums import (
     AnnotationFileType,
     AnnotationStatus,
     ImportAnnotationMode,
     InferenceType,
 )
-from picsellia.types.schemas import DatasetVersionSchema
+from picsellia.types.schemas import DatasetVersionSchema, DatasetVersionStats
 from picsellia.utils import (
     combine_two_ql,
     convert_tag_list_to_query_language,
     filter_payload,
     flatten_dict,
 )
 
@@ -1229,15 +1229,15 @@
         Arguments:
             target_dir (str): directory to synchronize against
             do_download (bool): do download files when they are not in local directory
         """
         assert os.path.isdir(target_dir), "Please select a valid directory path"
         logger.info("⌛️ Scanning Dataset Assets..")
         assets: MultiAsset = self.list_assets()
-        filenames = set(map(lambda asset: asset.filename, assets))
+        filenames = set(map(lambda asset: asset.filename, assets.items))
         logger.info("🔍 Scanning Local Dataset Folder ..")
         local_filenames = set(
             [
                 e
                 for e in os.listdir(target_dir)
                 if os.path.isfile(os.path.join(target_dir, e))
             ]
@@ -1280,14 +1280,36 @@
             return multi_assets
         else:
             logger.info("✅ Dataset is up-to-date.")
             return None
 
     @exception_handler
     @beartype
+    def retrieve_stats(self) -> DatasetVersionStats:
+        """Retrieve statistics of this dataset version (label repartition, number of objects, number of annotations).
+
+        Examples:
+            ```python
+            stats = foo_dataset.retrieve_stats()
+            assert stats.label_repartition == {"cat": 23, "dog": 2}
+            assert stats.nb_objects == 25
+            assert stats.nb_annotations == 5
+            ```
+
+        Returns:
+            A DatasetVersionStats schema with keys:
+                - label_repartition: dict with label names as keys and number of shape with these labels as value
+                - nb_objects: total number of objects (sum of label_repartition values)
+                - nb_annotations: total number of (Annotation) objects of this dataset version
+        """
+        r = self.connexion.get(f"/sdk/dataset/version/{self.id}/stats").json()
+        return DatasetVersionStats(**r)
+
+    @exception_handler
+    @beartype
     def get_or_create_asset_tag(self, name: str) -> Tag:
         """Retrieve an asset tag used in this dataset version by its name.
         If tag does not exist, create it and return it.
 
         Examples:
             ```python
             tag = self.get_or_create_asset_tag("new_tag")
@@ -1388,25 +1410,14 @@
 
         Returns:
             A list of (Tag)
         """
         r = self.connexion.get(f"/sdk/dataset/version/{self.id}/tags").json()
         return list(map(partial(Tag, self.connexion), r["items"]))
 
-    @exception_handler
-    @beartype
-    def _do_list_assets_extended(
-        self, limit: int, offset: int
-    ) -> Tuple[List[Dict], int]:
-        params = {"limit": limit, "offset": offset}
-        r = self.connexion.get(
-            f"/sdk/dataset/version/{self.id}/assets/extended", params=params
-        ).json()
-        return r["items"], r["count"]
-
     @beartype
     def train_test_split(
         self,
         prop: float = 0.8,
         random_seed: Optional[Any] = None,
         load_asset_page_size: int = 100,
     ) -> Tuple[MultiAsset, MultiAsset, Dict[str, list], Dict[str, list], List[Label]]:
@@ -1421,106 +1432,190 @@
             random_seed (Any, optional): Use a seed to ensures same result if run multiple times. Defaults to None.
             load_asset_page_size (int, optional): Page size when loading assets. Defaults to 100.
 
         Returns:
             A tuple with all of this information (
                 list of train assets,
                 list of test assets,
-                dict of repartition of classes for train assets,
-                dict of repartition of classes for test assets,
+                dict of repartition of classes for train assets, with {"x": list of labels, "y":  list of label count},
+                dict of repartition of classes for test assets, with {"x": list of labels, "y":  list of label count},
                 list of labels
             )
         """
+        if prop > 1 or prop < 0:
+            raise ValueError("Please give a 'prop' parameter between 0 and 1")
 
-        extended_assets = mlt.do_paginate(
-            None, None, load_asset_page_size, self._do_list_assets_extended
+        multi_assets, label_distributions, labels = self.split_into_multi_assets(
+            [prop, 1.0 - prop], random_seed, load_asset_page_size
         )
-        if not extended_assets:
-            raise NoDataError("No asset with annotation found in this dataset")
+        distributions = [
+            {
+                "x": list(label_repartition.keys()),
+                "y": list(label_repartition.values()),
+            }
+            for label_repartition in label_distributions
+        ]
 
-        count = 0
-        items = []
-        for item in extended_assets:
-            if not item["annotations"]:
-                logger.debug(f"No annotation for asset {item['data']['filename']}")
-                continue
-
-            count += 1
-            items.append(item)
+        return (
+            multi_assets[0],
+            multi_assets[1],
+            distributions[0],
+            distributions[1],
+            labels,
+        )
 
-        if random_seed is not None:
-            random.seed(random_seed)
+    @beartype
+    def train_test_val_split(
+        self,
+        ratios: List[float] = None,
+        random_seed: Optional[Any] = None,
+        load_asset_page_size: int = 100,
+    ) -> Tuple[
+        MultiAsset,
+        MultiAsset,
+        MultiAsset,
+        Dict[str, list],
+        Dict[str, list],
+        Dict[str, list],
+        List[Label],
+    ]:
+        """Split a DatasetVersion into 3 MultiAssets and return their label repartition.
+        By default, will split with a ratio of 0.64, 0.16 and 0.20
 
-        nb_assets_train = int(count * prop)
-        train_eval_rep = [1] * nb_assets_train + [0] * (count - nb_assets_train)
-        random.shuffle(train_eval_rep)
+        Examples:
+            ```python
+            train_assets, test_assets, val_assets, count_train, count_test, count_val, labels = dataset.train_test_val_split()
+            ```
+        Arguments:
+            ratios (list of float, optional): Ratios of split used for training and eval set.
+                Defaults to [0.64, 0.16, 0.20]
+            random_seed (Any, optional): Use a seed to ensures same result if run multiple times. Defaults to None.
+            load_asset_page_size (int, optional): Page size when loading assets. Defaults to 100.
 
-        labels = self.list_labels()
-        label_names = {str(label.id): label.name for label in labels}
+        Returns:
+            A tuple with all of this information (
+                list of train assets,
+                list of test assets
+                list of val assets,
+                dict of repartition of classes for train assets, with {"x": list of labels, "y":  list of label count},
+                dict of repartition of classes for test assets, with {"x": list of labels, "y":  list of label count},
+                dict of repartition of classes for val assets, with {"x": list of labels, "y":  list of label count},
+                list of labels
+            )
+        """
+        if not ratios:
+            ratios = [0.64, 0.16, 0.20]
 
-        k = 0
+        if len(ratios) != 3:
+            raise ValueError("Ratios list should be a list of 3 elements")
 
-        train_assets = []
-        eval_assets = []
+        multi_assets, label_distributions, labels = self.split_into_multi_assets(
+            ratios, random_seed, load_asset_page_size
+        )
+        distributions = [
+            {
+                "x": list(label_repartition.keys()),
+                "y": list(label_repartition.values()),
+            }
+            for label_repartition in label_distributions
+        ]
 
-        train_label_count = {}
-        eval_label_count = {}
-        for item in items:
-            annotations = item["annotations"]
+        return (
+            multi_assets[0],
+            multi_assets[1],
+            multi_assets[2],
+            distributions[0],
+            distributions[1],
+            distributions[2],
+            labels,
+        )
 
-            # TODO: Get only from worker or status
-            annotation = annotations[0]
+    @beartype
+    def split_into_multi_assets(
+        self,
+        ratios: List[Union[float, int]],
+        random_seed: Optional[Any] = None,
+        load_asset_page_size: int = 100,
+    ) -> Tuple[List[MultiAsset], List[Dict[str, int]], List[Label]]:
+        """Split dataset into multiple MultiAsset, proportionally according to given ratios.
 
-            asset = Asset(self.connexion, dataset_version_id=self.id, data=item)
+        Examples:
+            ```python
+            split_assets, counts, labels = dataset.split_into_multi_assets([0.2, 0.5, 0.3])
+            train_assets = split_assets[0]
+            test_assets = split_assets[1]
+            val_assets = split_assets[2]
+            ```
+        Arguments:
+            ratios (list of float): Percentage of data that will go into each category.
+                Will be normalized but sum should be equals to one if you don't want to be confused.
+            random_seed (Any, optional): Use a seed to ensures same result if run multiple times. Defaults to None.
+            load_asset_page_size (int, optional): Page size when loading assets. Defaults to 100.
 
-            if train_eval_rep[k] == 0:
-                eval_assets.append(asset)
-                label_count_ref = eval_label_count
-            else:
-                train_assets.append(asset)
-                label_count_ref = train_label_count
+        Returns:
+            A tuple with all of this information (
+                list of MultiAsset,
+                dict of repartition of classes for each MultiAsset,
+                list of labels
+            )
+        """
+        if not ratios or len(ratios) < 2:
+            raise NoDataError("Please give at least two proportions")
 
-            k += 1
+        # Fetch assets and annotation
+        fetched_raw_assets = self._do_list_items_with_annotations(load_asset_page_size)
 
-            label_ids = []
-            for shape in annotation["rectangles"]:
-                label_ids.append(shape["label_id"])
-
-            for shape in annotation["classifications"]:
-                label_ids.append(shape["label_id"])
-
-            for shape in annotation["points"]:
-                label_ids.append(shape["label_id"])
-
-            for shape in annotation["polygons"]:
-                label_ids.append(shape["label_id"])
-
-            for shape in annotation["lines"]:
-                label_ids.append(shape["label_id"])
-
-            for label_id in label_ids:
-                try:
-                    label_name = label_names[label_id]
-                    if label_name not in label_count_ref:
-                        label_count_ref[label_name] = 1
-                    else:
-                        label_count_ref[label_name] += 1
-                except KeyError:  # pragma: no cover
-                    logger.warning(f"A shape has an unknown label ({label_id}).")
-
-        train_repartition = {
-            "x": list(train_label_count.keys()),
-            "y": list(train_label_count.values()),
-        }
+        # Fetch labels
+        labels = self.list_labels()
+        label_names = {str(label.id): label.name for label in labels}
 
-        eval_repartition = {
-            "x": list(eval_label_count.keys()),
-            "y": list(eval_label_count.values()),
-        }
+        # Split annotations according to ratios
+        ratios = AssetSplitter.normalize_ratios(ratios)
+        AssetSplitter.shuffle_items(fetched_raw_assets, random_seed)
+        split_items = AssetSplitter.split_with_ratios(fetched_raw_assets, ratios)
+
+        multi_assets: List[MultiAsset] = []
+        distributions: List[Dict[str, int]] = []
+        for raw_items in split_items:
+            assets, label_distribution = AssetSplitter.convert_items_to_assets(
+                self.connexion, self.id, raw_items, label_names
+            )
+            multi_assets.append(MultiAsset(self.connexion, self.id, assets))
+            distributions.append(label_distribution)
 
         return (
-            MultiAsset(self.connexion, self.id, train_assets),
-            MultiAsset(self.connexion, self.id, eval_assets),
-            train_repartition,
-            eval_repartition,
+            multi_assets,
+            distributions,
             labels,
         )
+
+    @exception_handler
+    @beartype
+    def _do_list_items_with_annotations(self, load_asset_page_size: int):
+        # Retrieve assets
+        extended_assets = mlt.do_paginate(
+            None, None, load_asset_page_size, self._do_list_assets_extended
+        )
+        if not extended_assets:
+            raise NoDataError("No asset with annotation found in this dataset")
+
+        # Retrieve annotations
+        items = []
+        for item in extended_assets:
+            if not item["annotations"]:
+                logger.debug(f"No annotation for asset {item['data']['filename']}")
+                continue
+
+            items.append(item)
+
+        return items
+
+    @exception_handler
+    @beartype
+    def _do_list_assets_extended(
+        self, limit: int, offset: int
+    ) -> Tuple[List[Dict], int]:
+        params = {"limit": limit, "offset": offset}
+        r = self.connexion.get(
+            f"/sdk/dataset/version/{self.id}/assets/extended", params=params
+        ).json()
+        return r["items"], r["count"]
```

### Comparing `picsellia-6.6.0/picsellia/sdk/datasource.py` & `picsellia-6.7.0/picsellia/sdk/datasource.py`

 * *Files identical despite different names*

### Comparing `picsellia-6.6.0/picsellia/sdk/deployment.py` & `picsellia-6.7.0/picsellia/sdk/deployment.py`

 * *Files identical despite different names*

### Comparing `picsellia-6.6.0/picsellia/sdk/downloadable.py` & `picsellia-6.7.0/picsellia/sdk/downloadable.py`

 * *Files 0% similar despite different names*

```diff
@@ -61,15 +61,15 @@
     def download(
         self, target_path: Union[str, Path] = "./", force_replace: bool = False
     ) -> None:
         """Download this object into given target_path
 
         Examples:
             ```python
-            data = clt.get_datalake().fetch_data(1)
+            data = clt.get_datalake().list_data(limit=1)
             data.download('./data/')
             ```
 
         Arguments:
             target_path (str, optional): Target path where data will be downloaded. Defaults to './'.
             force_replace: (bool, optional): Replace an existing file if exists. Defaults to False.
         """
```

### Comparing `picsellia-6.6.0/picsellia/sdk/evaluation.py` & `picsellia-6.7.0/picsellia/sdk/evaluation.py`

 * *Files identical despite different names*

### Comparing `picsellia-6.6.0/picsellia/sdk/experiment.py` & `picsellia-6.7.0/picsellia/sdk/experiment.py`

 * *Files identical despite different names*

### Comparing `picsellia-6.6.0/picsellia/sdk/job.py` & `picsellia-6.7.0/picsellia/sdk/job.py`

 * *Files identical despite different names*

### Comparing `picsellia-6.6.0/picsellia/sdk/label.py` & `picsellia-6.7.0/picsellia/sdk/label.py`

 * *Files identical despite different names*

### Comparing `picsellia-6.6.0/picsellia/sdk/line.py` & `picsellia-6.7.0/picsellia/sdk/line.py`

 * *Files identical despite different names*

### Comparing `picsellia-6.6.0/picsellia/sdk/log.py` & `picsellia-6.7.0/picsellia/sdk/log.py`

 * *Files identical despite different names*

### Comparing `picsellia-6.6.0/picsellia/sdk/logging_file.py` & `picsellia-6.7.0/picsellia/sdk/logging_file.py`

 * *Files 10% similar despite different names*

```diff
@@ -40,14 +40,19 @@
     def large(self) -> bool:
         """(LoggingFile) are usually not large file."""
         return False
 
     @exception_handler
     @beartype
     def reset_url(self) -> str:
+        """Reset url property of this LoggingFile by calling platform.
+
+        Returns:
+            A url as a string of this LoggingFile.
+        """
         self._url = self.connexion.init_download(self.object_name)
         return self._url
 
     @exception_handler
     @beartype
     def refresh(self, data: dict) -> LoggingFileSchema:
         schema = LoggingFileSchema(**data)
```

### Comparing `picsellia-6.6.0/picsellia/sdk/model.py` & `picsellia-6.7.0/picsellia/sdk/model.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import logging
 from functools import partial
 from typing import List, Optional, Union
 
 import orjson
 from beartype import beartype
+from deprecation import deprecated
 
 import picsellia.utils as utils
 from picsellia.colors import Colors
 from picsellia.decorators import exception_handler
 from picsellia.sdk.connexion import Connexion
 from picsellia.sdk.dao import Dao
 from picsellia.sdk.model_version import ModelVersion
@@ -26,31 +27,39 @@
 
     @property
     def name(self) -> str:
         """Name of this (Model)"""
         return self._name
 
     @property
+    @deprecated(
+        deprecated_in="6.7.0",
+        details="'type' property is deprecated and will be removed in future versions.",
+    )
     def type(self) -> InferenceType:
         """Type of this (Model)"""
         return self._type
 
     @property
+    @deprecated(
+        deprecated_in="6.7.0",
+        details="'framework' property is deprecated and will be removed in future versions.",
+    )
     def framework(self) -> Framework:
         """Framework of this (Model)"""
         return self._framework
 
     @property
     def private(self) -> bool:
         """Privacy of this (Model)"""
         return self._private
 
     def __str__(self):
         is_private = "" if self._private else "[PUBLIC]"
-        return f"{Colors.BLUE}{is_private} Model '{self.name}' with type {self.type.name} and framework {self.framework.name}  {Colors.ENDC} (id: {self.id})"
+        return f"{Colors.BLUE}{is_private} Model '{self.name}' {Colors.ENDC} (id: {self.id})"
 
     @exception_handler
     @beartype
     def get_resource_url_on_platform(self) -> str:
         """Get platform url of this resource.
 
         Examples:
@@ -95,31 +104,28 @@
         """Update a model with a new name, framework, privacy, description or type
 
         Examples:
             ```python
             model.update(description="Very cool model")
             ```
         """
-        if framework:
-            framework = Framework.validate(framework)
-
         if type:
-            type = InferenceType.validate(type)
+            logging.warning(
+                "'type' parameter is deprecated and will be removed in future versions. "
+                "If you want to give a type to your model version, call update() on ModelVersion."
+            )
 
-        if type and type not in [
-            InferenceType.CLASSIFICATION,
-            InferenceType.OBJECT_DETECTION,
-            InferenceType.SEGMENTATION,
-        ]:
-            raise TypeError(f"Type '{type}' not supported yet for model")
+        if framework:
+            logging.warning(
+                "'framework' parameter is deprecated and will be removed in future versions. "
+                "If you want to give a framework to your model version, call update() on your ModelVersion."
+            )
 
         payload = {
             "name": name,
-            "type": type,
-            "framework": framework,
             "private": private,
             "description": description,
         }
         filtered_payload = utils.filter_payload(payload)
         r = self.connexion.patch(
             f"/sdk/model/{self.id}", data=orjson.dumps(filtered_payload)
         ).json()
@@ -165,28 +171,47 @@
         docker_image_name: Optional[str] = None,
         docker_flags: Optional[List[str]] = None,
         thumb_object_name: Optional[str] = None,
         notebook_link: Optional[str] = None,
         labels: Optional[dict] = None,
         base_parameters: Optional[dict] = None,
         docker_env_variables: Optional[dict] = None,
+        name: Optional[str] = None,
+        framework: Union[str, Framework, None] = None,
+        type: Union[str, InferenceType, None] = None,
     ) -> ModelVersion:
         """Create a version of a model.
 
         The version number of this model will be defined by the platform. It is incremented automatically.
 
         Examples:
             ```python
-            model_v0 = model.create_version()
+            model_v0 = model.create_version(labels={"1": "cat", "2": "dog"}, framework=Framework.TENSORFLOW, type=InferenceType.OBJECT_DETECTION)
             ```
 
         Returns:
             A (ModelVersion) object
         """
+        if framework:
+            framework = Framework.validate(framework)
+
+        if type:
+            type = InferenceType.validate(type)
+
+        if type and type not in [
+            InferenceType.CLASSIFICATION,
+            InferenceType.OBJECT_DETECTION,
+            InferenceType.SEGMENTATION,
+        ]:
+            raise TypeError(f"Type '{type}' not supported yet for model version")
+
         payload = {
+            "name": name,
+            "type": type,
+            "framework": framework,
             "docker_image_name": docker_image_name,
             "docker_flags": docker_flags,
             "thumb_object_name": thumb_object_name,
             "notebook_link": notebook_link,
             "labels": labels,
             "base_parameters": base_parameters,
             "docker_env_variables": docker_env_variables,
@@ -196,26 +221,34 @@
             f"/sdk/model/{self.id}/versions",
             data=orjson.dumps(filtered_payload),
         ).json()
         return ModelVersion(self.connexion, r)
 
     @exception_handler
     @beartype
-    def get_version(self, version: int) -> ModelVersion:
-        """Retrieve a version of a model
+    def get_version(self, version: Union[int, str]) -> ModelVersion:
+        """Retrieve a version of a model from its version or its name
 
         Examples:
             ```python
-            version = model.get_version(0)
+            # Assuming model is a Model without version
+            model_version_a = model.create_version("first-version")
+            model_version_b = model.get_version(0)
+            model_version_c = model.get_version("first-version")
+            assert model_version_a == model_version_b
+            assert model_version_a == model_version_c
             ```
 
         Returns:
             A (ModelVersion) object
         """
-        params = {"version": version}
+        if isinstance(version, str):
+            params = {"name": version}
+        else:
+            params = {"version": version}
         r = self.connexion.get(
             f"/sdk/model/{self.id}/versions/find", params=params
         ).json()
         return ModelVersion(self.connexion, r)
 
     @exception_handler
     @beartype
```

### Comparing `picsellia-6.6.0/picsellia/sdk/model_context.py` & `picsellia-6.7.0/picsellia/sdk/model_context.py`

 * *Files identical despite different names*

### Comparing `picsellia-6.6.0/picsellia/sdk/model_file.py` & `picsellia-6.7.0/picsellia/sdk/model_file.py`

 * *Files 6% similar despite different names*

```diff
@@ -59,14 +59,19 @@
         self._large = schema.large
         self._url = schema.url
         return schema
 
     @exception_handler
     @beartype
     def reset_url(self) -> str:
+        """Reset url property of this ModelFile by calling platform.
+
+        Returns:
+            A url as a string of this ModelFile.
+        """
         self._url = self.connexion.init_download(self.object_name)
         return self._url
 
     @exception_handler
     @beartype
     def delete(self) -> None:
         """Delete this file
```

### Comparing `picsellia-6.6.0/picsellia/sdk/model_version.py` & `picsellia-6.7.0/picsellia/sdk/model_version.py`

 * *Files 8% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 from functools import partial
 from pathlib import Path
 from typing import List, Optional, Union
 from uuid import UUID
 
 import orjson
 from beartype import beartype
+from deprecation import deprecated
 
 import picsellia.exceptions as exceptions
 import picsellia.utils as utils
 from picsellia.colors import Colors
 from picsellia.decorators import exception_handler
 from picsellia.sdk.connexion import Connexion
 from picsellia.sdk.dao import Dao
@@ -27,24 +28,29 @@
 
 class ModelVersion(Dao, Taggable):
     def __init__(self, connexion: Connexion, data: dict):
         Dao.__init__(self, connexion, data)
         Taggable.__init__(self, TagTarget.MODEL_VERSION)
 
     @property
-    def name(self) -> str:
-        """Name of this (ModelVersion)"""
-        return self._name
+    def origin_name(self) -> str:
+        """Name of origin of this (ModelVersion)"""
+        return self._origin_name
 
     @property
     def origin_id(self) -> UUID:
         """UUID of the origin (Model) of this (ModelVersion)"""
         return self._origin_id
 
     @property
+    def name(self) -> str:
+        """Name of this (ModelVersion)"""
+        return self._name
+
+    @property
     def version(self) -> int:
         """Version number of this (ModelVersion)"""
         return self._version
 
     @property
     def type(self) -> InferenceType:
         """Type of this (ModelVersion)"""
@@ -56,15 +62,15 @@
         return self._framework
 
     @property
     def labels(self) -> Optional[dict]:
         return self._labels
 
     def __str__(self):
-        return f"{Colors.BLUE}Version {self.name} of Model '{self.version}' {Colors.ENDC} (id: {self.id})"
+        return f"{Colors.BLUE}Version {self.name} of Model '{self.version}' with type {self.type.name} and framework {self.framework.name} {Colors.ENDC} (id: {self.id})"
 
     @exception_handler
     @beartype
     def get_resource_url_on_platform(self) -> str:
         """Get platform url of this resource.
 
         Examples:
@@ -86,19 +92,20 @@
         self.refresh(r)
         return r
 
     @exception_handler
     @beartype
     def refresh(self, data: dict) -> ModelVersionSchema:
         schema = ModelVersionSchema(**data)
-        self._version = schema.version
-        self._name = schema.origin.name
+        self._origin_name = schema.origin.name
         self._origin_id = schema.origin.id
-        self._type = schema.origin.type
-        self._framework = schema.origin.framework
+        self._version = schema.version
+        self._name = schema.name
+        self._type = schema.type
+        self._framework = schema.framework
         self._labels = schema.labels
         return schema
 
     @exception_handler
     @beartype
     def get_tags(self) -> List[Tag]:
         """Retrieve the tags of your model version.
@@ -122,30 +129,49 @@
         labels: Optional[dict] = None,
         docker_image_name: Optional[str] = None,
         docker_flags: Optional[List[str]] = None,
         thumb_object_name: Optional[str] = None,
         notebook_link: Optional[str] = None,
         base_parameters: Optional[dict] = None,
         docker_env_variables: Optional[dict] = None,
+        framework: Union[str, Framework, None] = None,
+        type: Union[str, InferenceType, None] = None,
+        name: Optional[str] = None,
     ) -> None:
         """Update this model version with some new infos.
 
         Examples:
             ```python
             model_v1.update(docker_image_name="docker.io/model1")
             ```
         """
+        if framework:
+            framework = Framework.validate(framework)
+
+        if type:
+            type = InferenceType.validate(type)
+
+        if type and type not in [
+            InferenceType.CLASSIFICATION,
+            InferenceType.OBJECT_DETECTION,
+            InferenceType.SEGMENTATION,
+        ]:
+            raise TypeError(f"Type '{type}' not supported yet for model version")
+
         payload = {
             "labels": labels,
             "docker_image_name": docker_image_name,
             "docker_flags": docker_flags,
             "thumb_object_name": thumb_object_name,
             "notebook_link": notebook_link,
             "base_parameters": base_parameters,
             "docker_env_variables": docker_env_variables,
+            "type": type,
+            "framework": framework,
+            "name": name,
         }
         filtered_payload = utils.filter_payload(payload)
         r = self.connexion.patch(
             f"/sdk/model/version/{self.id}",
             data=orjson.dumps(filtered_payload),
         ).json()
         self.refresh(r)
@@ -284,14 +310,18 @@
         ).json()
         model_file = ModelFile(self.connexion, r)
         logger.info(f"{model_file} stored for {self}")
         return model_file
 
     @exception_handler
     @beartype
+    @deprecated(
+        deprecated_in="6.7.0",
+        details="update_thumbnail method will be removed in the future, you should use the web app instead",
+    )
     def update_thumbnail(self, path: Union[str, Path]) -> None:
         """Updates the model thumbnail.
 
         Update the model thumbnail with given file.
         File size shall be less than 5Mb.
 
         Examples:
@@ -332,28 +362,28 @@
     ):
         """Create a (Deployment) for a model.
 
         This method allows you to create a (Deployment) on Picsellia. You will then have
         access to the monitoring dashboard and the model management part!
 
         Examples:
-            Create a serverless deployment
             ```python
-            model = client.get_model(name="my-awesome-model")
-            deployment = model.create_deployment()
+            model_version = client.get_model(name="my-awesome-model").get_version(0)
+            deployment = model_version.deploy(name="my-awesome-deployment", min_threshold=0.5)
             ```
 
         Arguments:
             name (str): Name of your deployment. Defaults to a random name.
-            min_threshold (float): Threshold of detection scores used by models when predicting
-            target_datalake (Datalake): Datalake to use when data are pushed into Picsellia
+            min_threshold (float): Threshold of detection scores used by models when predicting. Defaults to 0.
+            target_datalake (Datalake): Datalake to use when data are pushed into Picsellia.
+                Defaults to organization default Datalake.
 
 
         Returns:
-            A (Deployment) that you can manipulate
+            A (Deployment)
         """
         from picsellia.sdk.deployment import Deployment
 
         payload = {
             "name": name,
             "min_threshold": min_threshold,
         }
```

### Comparing `picsellia-6.6.0/picsellia/sdk/multi_object.py` & `picsellia-6.7.0/picsellia/sdk/multi_object.py`

 * *Files identical despite different names*

### Comparing `picsellia-6.6.0/picsellia/sdk/point.py` & `picsellia-6.7.0/picsellia/sdk/point.py`

 * *Files identical despite different names*

### Comparing `picsellia-6.6.0/picsellia/sdk/polygon.py` & `picsellia-6.7.0/picsellia/sdk/polygon.py`

 * *Files identical despite different names*

### Comparing `picsellia-6.6.0/picsellia/sdk/project.py` & `picsellia-6.7.0/picsellia/sdk/project.py`

 * *Files 1% similar despite different names*

```diff
@@ -248,15 +248,18 @@
             Exception: Experiment not found
 
         Returns:
             An (Experiment) object that you can manipulate
         """
         if isinstance(id, str):
             id = UUID(id)
-        r = self.connexion.get(f"/sdk/experiment/{id}").json()
+        params = {"id": id}
+        r = self.connexion.get(
+            f"/sdk/project/{self.id}/experiments/find", params=params
+        ).json()
         return Experiment(self.connexion, r)
 
     @exception_handler
     @beartype
     def get_scan(self, name: str) -> Scan:
         """Retrieve an existing scan.
```

### Comparing `picsellia-6.6.0/picsellia/sdk/rectangle.py` & `picsellia-6.7.0/picsellia/sdk/rectangle.py`

 * *Files identical despite different names*

### Comparing `picsellia-6.6.0/picsellia/sdk/run.py` & `picsellia-6.7.0/picsellia/sdk/run.py`

 * *Files identical despite different names*

### Comparing `picsellia-6.6.0/picsellia/sdk/scan.py` & `picsellia-6.7.0/picsellia/sdk/scan.py`

 * *Files 2% similar despite different names*

```diff
@@ -160,15 +160,16 @@
             id (str): id (primary key) of the run on Picsellia
 
         Returns:
             A (Run) object manipulable
         """
         if isinstance(id, str):
             id = UUID(id)
-        r = self.connexion.get(f"/sdk/run/{id}").json()
+        params = {"id": id}
+        r = self.connexion.get(f"/sdk/scan/{self.id}/runs/find", params=params).json()
         return Run(self.connexion, r)
 
     @exception_handler
     @beartype
     def get_next_run(self) -> Run:
         """Get next available Run for Scan.
```

### Comparing `picsellia-6.6.0/picsellia/sdk/scan_file.py` & `picsellia-6.7.0/picsellia/sdk/scan_file.py`

 * *Files 5% similar despite different names*

```diff
@@ -62,14 +62,19 @@
         r = self.connexion.get(f"/sdk/scan/file/{self.id}").json()
         self.refresh(r)
         return r
 
     @exception_handler
     @beartype
     def reset_url(self) -> str:
+        """Reset url property of this ScanFile by calling platform.
+
+        Returns:
+            A url as a string of this ScanFile.
+        """
         self._url = self.connexion.init_download(self.object_name)
         return self._url
 
     @exception_handler
     @beartype
     def update(
         self,
```

### Comparing `picsellia-6.6.0/picsellia/sdk/tag.py` & `picsellia-6.7.0/picsellia/sdk/tag.py`

 * *Files identical despite different names*

### Comparing `picsellia-6.6.0/picsellia/sdk/taggable.py` & `picsellia-6.7.0/picsellia/sdk/taggable.py`

 * *Files identical despite different names*

### Comparing `picsellia-6.6.0/picsellia/sdk/worker.py` & `picsellia-6.7.0/picsellia/sdk/worker.py`

 * *Files identical despite different names*

### Comparing `picsellia-6.6.0/picsellia/services/coco_file_builder.py` & `picsellia-6.7.0/picsellia/services/coco_file_builder.py`

 * *Files identical despite different names*

### Comparing `picsellia-6.6.0/picsellia/services/coco_importer.py` & `picsellia-6.7.0/picsellia/services/coco_importer.py`

 * *Files identical despite different names*

### Comparing `picsellia-6.6.0/picsellia/services/datasource.py` & `picsellia-6.7.0/picsellia/services/datasource.py`

 * *Files identical despite different names*

### Comparing `picsellia-6.6.0/picsellia/services/error_manager.py` & `picsellia-6.7.0/picsellia/services/error_manager.py`

 * *Files identical despite different names*

### Comparing `picsellia-6.6.0/picsellia/services/voc_importer.py` & `picsellia-6.7.0/picsellia/services/voc_importer.py`

 * *Files identical despite different names*

### Comparing `picsellia-6.6.0/picsellia/services/yolo_importer.py` & `picsellia-6.7.0/picsellia/services/yolo_importer.py`

 * *Files identical despite different names*

### Comparing `picsellia-6.6.0/picsellia/types/enums.py` & `picsellia-6.7.0/picsellia/types/enums.py`

 * *Files identical despite different names*

### Comparing `picsellia-6.6.0/picsellia/types/schemas.py` & `picsellia-6.7.0/picsellia/types/schemas.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from typing import List, Optional, Union
+from typing import Dict, List, Optional, Union
 from uuid import UUID
 
 from pydantic import BaseModel, Field
 
 from picsellia.types.enums import (
     AnnotationStatus,
     DataType,
@@ -39,25 +39,34 @@
 class DatasetVersionSchema(DaoSchema):
     name: str = Field(alias="origin_name")
     origin_id: UUID = Field(alias="origin_id")
     version: str
     type: InferenceType
 
 
+class DatasetVersionStats(BaseModel):
+    label_repartition: Dict[str, int]
+    nb_objects: int
+    nb_annotations: int
+
+
 class ModelSchema(DaoSchema):
     name: str
     type: InferenceType
     framework: Framework
     private: bool
 
 
 class ModelVersionSchema(DaoSchema):
     origin: ModelSchema
+    name: str
     version: int
     labels: Optional[dict]
+    type: InferenceType
+    framework: Framework
 
 
 class ModelDataSchema(DaoSchema):
     name: str
     version_id: UUID
     repartition: dict
```

### Comparing `picsellia-6.6.0/picsellia/types/schemas_prediction.py` & `picsellia-6.7.0/picsellia/types/schemas_prediction.py`

 * *Files 2% similar despite different names*

```diff
@@ -31,20 +31,20 @@
 
     if len(v) < 1:
         raise ValueError("There must be at least one score")
 
     return v
 
 
-def masks_validator(v: List[List[int]]) -> List[List[int]]:
+def masks_validator(v: List[List[List[int]]]) -> List[List[List[int]]]:
     if not isinstance(v, List):
         raise TypeError(v)
 
     if len(v) < 1:
-        raise ValueError("There must be at least one id")
+        raise ValueError("There must be at least one mask")
 
     return v
 
 
 class PredictionFormat(BaseModel):
     @property
     def model_type(cls) -> InferenceType:
@@ -95,15 +95,15 @@
         return values
 
 
 class SegmentationPredictionFormat(PredictionFormat):
     detection_classes: List[int]
     detection_boxes: List[List[int]]
     detection_scores: List[float]
-    detection_masks: List[List[int]]
+    detection_masks: List[List[List[int]]]
 
     _validate_labels = validator("detection_classes", allow_reuse=True)(
         labels_validator
     )
     _validate_boxes = validator("detection_boxes", allow_reuse=True)(boxes_validator)
     _validate_scores = validator("detection_scores", allow_reuse=True)(scores_validator)
     _validate_masks = validator("detection_masks", allow_reuse=True)(masks_validator)
```

### Comparing `picsellia-6.6.0/picsellia/utils.py` & `picsellia-6.7.0/picsellia/utils.py`

 * *Files identical despite different names*

### Comparing `picsellia-6.6.0/pyproject.toml` & `picsellia-6.7.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 src_paths = ["picsellia", "tests"]
 
 [tool.pycln]
 all = true
 
 [tool.poetry]
 name = "picsellia"
-version = "6.6.0"
+version = "6.7.0"
 description = "Python SDK package for Picsellia MLOps platform"
 authors = ["Pierre-Nicolas Tiffreau <pierre-nicolas@picsellia.com>", "Thomas Darget <thomas.darget@picsellia.com>"]
 maintainers = ["Pierre-Nicolas Tiffreau <pierre-nicolas@picsellia.com>", "Thomas Darget <thomas.darget@picsellia.com>", "Lucien Haurat <lucien.haurat@picsellia.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://www.picsellia.com/"
 documentation = "https://documentation.picsellia.com/reference/client"
```

### Comparing `picsellia-6.6.0/PKG-INFO` & `picsellia-6.7.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: picsellia
-Version: 6.6.0
+Version: 6.7.0
 Summary: Python SDK package for Picsellia MLOps platform
 Home-page: https://www.picsellia.com/
 License: MIT
 Keywords: ai,picsellia,sdk,cvops
 Author: Pierre-Nicolas Tiffreau
 Author-email: pierre-nicolas@picsellia.com
 Maintainer: Pierre-Nicolas Tiffreau
```

