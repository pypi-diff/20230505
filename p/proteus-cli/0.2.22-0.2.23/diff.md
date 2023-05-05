# Comparing `tmp/proteus_cli-0.2.22.tar.gz` & `tmp/proteus_cli-0.2.23.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "proteus_cli-0.2.22.tar", max compression
+gzip compressed data, was "proteus_cli-0.2.23.tar", max compression
```

## Comparing `proteus_cli-0.2.22.tar` & `proteus_cli-0.2.23.tar`

### file list

```diff
@@ -1,51 +1,51 @@
--rw-r--r--   0        0        0     1330 2023-04-27 12:51:31.160209 proteus_cli-0.2.22/cli/__init__.py
--rw-r--r--   0        0        0      384 2023-04-27 12:51:31.164209 proteus_cli-0.2.22/cli/api/__init__.py
--rw-r--r--   0        0        0     1784 2023-04-27 12:51:31.164209 proteus_cli-0.2.22/cli/api/decorators.py
--rw-r--r--   0        0        0      849 2023-04-27 12:51:31.164209 proteus_cli-0.2.22/cli/api/hooks.py
--rw-r--r--   0        0        0        0 2023-04-27 12:51:31.164209 proteus_cli-0.2.22/cli/buckets/__init__.py
--rw-r--r--   0        0        0     1092 2023-04-27 12:51:31.164209 proteus_cli-0.2.22/cli/buckets/commands.py
--rw-r--r--   0        0        0     2570 2023-04-27 12:51:31.164209 proteus_cli-0.2.22/cli/config.py
--rw-r--r--   0        0        0        0 2023-04-27 12:51:31.164209 proteus_cli-0.2.22/cli/datasets/__init__.py
--rw-r--r--   0        0        0     1332 2023-04-27 12:51:31.164209 proteus_cli-0.2.22/cli/datasets/commands.py
--rw-r--r--   0        0        0        0 2023-04-27 12:51:31.164209 proteus_cli-0.2.22/cli/datasets/preprocessor/__init__.py
--rw-r--r--   0        0        0      939 2023-04-27 12:51:31.164209 proteus_cli-0.2.22/cli/datasets/preprocessor/config/__init__.py
--rw-r--r--   0        0        0      323 2023-04-27 12:51:31.164209 proteus_cli-0.2.22/cli/datasets/preprocessor/config/case/__init__.py
--rw-r--r--   0        0        0      851 2023-04-27 12:51:31.164209 proteus_cli-0.2.22/cli/datasets/preprocessor/config/case/cnn_pca.py
--rw-r--r--   0        0        0     3447 2023-04-27 12:51:31.164209 proteus_cli-0.2.22/cli/datasets/preprocessor/config/case/hm.py
--rw-r--r--   0        0        0     3054 2023-04-27 12:51:31.164209 proteus_cli-0.2.22/cli/datasets/preprocessor/config/case/well_model.py
--rw-r--r--   0        0        0      446 2023-04-27 12:51:31.164209 proteus_cli-0.2.22/cli/datasets/preprocessor/config/common/__init__.py
--rw-r--r--   0        0        0     3238 2023-04-27 12:51:31.164209 proteus_cli-0.2.22/cli/datasets/preprocessor/config/common/cnn_pca.py
--rw-r--r--   0        0        0     2009 2023-04-27 12:51:31.164209 proteus_cli-0.2.22/cli/datasets/preprocessor/config/common/hm.py
--rw-r--r--   0        0        0     1542 2023-04-27 12:51:31.164209 proteus_cli-0.2.22/cli/datasets/preprocessor/config/common/well_model.py
--rw-r--r--   0        0        0     2665 2023-04-27 12:51:31.164209 proteus_cli-0.2.22/cli/datasets/preprocessor/config/default.py
--rw-r--r--   0        0        0      418 2023-04-27 12:51:31.164209 proteus_cli-0.2.22/cli/datasets/preprocessor/config/step/__init__.py
--rw-r--r--   0        0        0      125 2023-04-27 12:51:31.164209 proteus_cli-0.2.22/cli/datasets/preprocessor/config/step/cnn_pca.py
--rw-r--r--   0        0        0     2415 2023-04-27 12:51:31.164209 proteus_cli-0.2.22/cli/datasets/preprocessor/config/step/hm.py
--rw-r--r--   0        0        0      128 2023-04-27 12:51:31.164209 proteus_cli-0.2.22/cli/datasets/preprocessor/config/step/well_model.py
--rw-r--r--   0        0        0      673 2023-04-27 12:51:31.164209 proteus_cli-0.2.22/cli/datasets/preprocessor/init_keywords.json
--rw-r--r--   0        0        0    13633 2023-04-27 12:51:31.164209 proteus_cli-0.2.22/cli/datasets/preprocessor/preprocess_functions.py
--rw-r--r--   0        0        0     4446 2023-04-27 12:51:31.164209 proteus_cli-0.2.22/cli/datasets/preprocessor/process_step.py
--rw-r--r--   0        0        0     8185 2023-04-27 12:51:31.164209 proteus_cli-0.2.22/cli/datasets/preprocessor/utils.py
--rw-r--r--   0        0        0      411 2023-04-27 12:51:31.164209 proteus_cli-0.2.22/cli/datasets/preprocessor/well_init_keywords.json
--rw-r--r--   0        0        0        0 2023-04-27 12:51:31.164209 proteus_cli-0.2.22/cli/datasets/sources/__init__.py
--rw-r--r--   0        0        0     4690 2023-04-27 12:51:31.164209 proteus_cli-0.2.22/cli/datasets/sources/az.py
--rw-r--r--   0        0        0      824 2023-04-27 12:51:31.164209 proteus_cli-0.2.22/cli/datasets/sources/common.py
--rw-r--r--   0        0        0     2366 2023-04-27 12:51:31.164209 proteus_cli-0.2.22/cli/datasets/sources/local.py
--rw-r--r--   0        0        0     1783 2023-04-27 12:51:31.164209 proteus_cli-0.2.22/cli/datasets/sources/s3.py
--rw-r--r--   0        0        0     9008 2023-04-27 12:51:31.164209 proteus_cli-0.2.22/cli/datasets/upload.py
--rw-r--r--   0        0        0        0 2023-04-27 12:51:31.164209 proteus_cli-0.2.22/cli/debugger/__init__.py
--rw-r--r--   0        0        0     2265 2023-04-27 12:51:31.164209 proteus_cli-0.2.22/cli/debugger/commands.py
--rw-r--r--   0        0        0     3926 2023-04-27 12:51:31.164209 proteus_cli-0.2.22/cli/debugger/init_keyword_check.py
--rw-r--r--   0        0        0        0 2023-04-27 12:51:31.164209 proteus_cli-0.2.22/cli/debugger/restart_keyword_check.py
--rw-r--r--   0        0        0        0 2023-04-27 12:51:31.164209 proteus_cli-0.2.22/cli/jobs/__init__.py
--rw-r--r--   0        0        0     1283 2023-04-27 12:51:31.164209 proteus_cli-0.2.22/cli/jobs/commands.py
--rw-r--r--   0        0        0     3026 2023-04-27 12:51:31.164209 proteus_cli-0.2.22/cli/jobs/list.py
--rw-r--r--   0        0        0      100 2023-04-27 12:51:31.168209 proteus_cli-0.2.22/cli/runtime.py
--rw-r--r--   0        0        0        0 2023-04-27 12:51:31.168209 proteus_cli-0.2.22/cli/simulations/__init__.py
--rw-r--r--   0        0        0     2460 2023-04-27 12:51:31.168209 proteus_cli-0.2.22/cli/simulations/commands.py
--rw-r--r--   0        0        0     7603 2023-04-27 12:51:31.168209 proteus_cli-0.2.22/cli/simulations/create.py
--rw-r--r--   0        0        0     4119 2023-04-27 12:51:31.168209 proteus_cli-0.2.22/cli/simulations/dependencySolver.py
--rw-r--r--   0        0        0     5190 2023-04-27 12:51:31.168209 proteus_cli-0.2.22/cli/simulations/opm.py
--rw-r--r--   0        0        0      449 2023-04-27 12:51:31.168209 proteus_cli-0.2.22/logging.ini
--rw-r--r--   0        0        0     1531 2023-04-27 12:51:31.168209 proteus_cli-0.2.22/pyproject.toml
--rw-r--r--   0        0        0      744 1970-01-01 00:00:00.000000 proteus_cli-0.2.22/PKG-INFO
+-rw-r--r--   0        0        0     1330 2023-05-05 07:35:49.880817 proteus_cli-0.2.23/cli/__init__.py
+-rw-r--r--   0        0        0      384 2023-05-05 07:35:49.880817 proteus_cli-0.2.23/cli/api/__init__.py
+-rw-r--r--   0        0        0     1784 2023-05-05 07:35:49.880817 proteus_cli-0.2.23/cli/api/decorators.py
+-rw-r--r--   0        0        0      849 2023-05-05 07:35:49.880817 proteus_cli-0.2.23/cli/api/hooks.py
+-rw-r--r--   0        0        0        0 2023-05-05 07:35:49.880817 proteus_cli-0.2.23/cli/buckets/__init__.py
+-rw-r--r--   0        0        0     1092 2023-05-05 07:35:49.880817 proteus_cli-0.2.23/cli/buckets/commands.py
+-rw-r--r--   0        0        0     2621 2023-05-05 07:35:49.880817 proteus_cli-0.2.23/cli/config.py
+-rw-r--r--   0        0        0        0 2023-05-05 07:35:49.880817 proteus_cli-0.2.23/cli/datasets/__init__.py
+-rw-r--r--   0        0        0     1332 2023-05-05 07:35:49.880817 proteus_cli-0.2.23/cli/datasets/commands.py
+-rw-r--r--   0        0        0        0 2023-05-05 07:35:49.880817 proteus_cli-0.2.23/cli/datasets/preprocessor/__init__.py
+-rw-r--r--   0        0        0      939 2023-05-05 07:35:49.880817 proteus_cli-0.2.23/cli/datasets/preprocessor/config/__init__.py
+-rw-r--r--   0        0        0      323 2023-05-05 07:35:49.880817 proteus_cli-0.2.23/cli/datasets/preprocessor/config/case/__init__.py
+-rw-r--r--   0        0        0      851 2023-05-05 07:35:49.880817 proteus_cli-0.2.23/cli/datasets/preprocessor/config/case/cnn_pca.py
+-rw-r--r--   0        0        0     3447 2023-05-05 07:35:49.880817 proteus_cli-0.2.23/cli/datasets/preprocessor/config/case/hm.py
+-rw-r--r--   0        0        0     3054 2023-05-05 07:35:49.880817 proteus_cli-0.2.23/cli/datasets/preprocessor/config/case/well_model.py
+-rw-r--r--   0        0        0      446 2023-05-05 07:35:49.880817 proteus_cli-0.2.23/cli/datasets/preprocessor/config/common/__init__.py
+-rw-r--r--   0        0        0     3238 2023-05-05 07:35:49.880817 proteus_cli-0.2.23/cli/datasets/preprocessor/config/common/cnn_pca.py
+-rw-r--r--   0        0        0     2009 2023-05-05 07:35:49.880817 proteus_cli-0.2.23/cli/datasets/preprocessor/config/common/hm.py
+-rw-r--r--   0        0        0     1542 2023-05-05 07:35:49.880817 proteus_cli-0.2.23/cli/datasets/preprocessor/config/common/well_model.py
+-rw-r--r--   0        0        0     2665 2023-05-05 07:35:49.880817 proteus_cli-0.2.23/cli/datasets/preprocessor/config/default.py
+-rw-r--r--   0        0        0      418 2023-05-05 07:35:49.880817 proteus_cli-0.2.23/cli/datasets/preprocessor/config/step/__init__.py
+-rw-r--r--   0        0        0      125 2023-05-05 07:35:49.880817 proteus_cli-0.2.23/cli/datasets/preprocessor/config/step/cnn_pca.py
+-rw-r--r--   0        0        0     2415 2023-05-05 07:35:49.880817 proteus_cli-0.2.23/cli/datasets/preprocessor/config/step/hm.py
+-rw-r--r--   0        0        0      128 2023-05-05 07:35:49.880817 proteus_cli-0.2.23/cli/datasets/preprocessor/config/step/well_model.py
+-rw-r--r--   0        0        0      673 2023-05-05 07:35:49.880817 proteus_cli-0.2.23/cli/datasets/preprocessor/init_keywords.json
+-rw-r--r--   0        0        0    13633 2023-05-05 07:35:49.880817 proteus_cli-0.2.23/cli/datasets/preprocessor/preprocess_functions.py
+-rw-r--r--   0        0        0     4446 2023-05-05 07:35:49.880817 proteus_cli-0.2.23/cli/datasets/preprocessor/process_step.py
+-rw-r--r--   0        0        0     8185 2023-05-05 07:35:49.880817 proteus_cli-0.2.23/cli/datasets/preprocessor/utils.py
+-rw-r--r--   0        0        0      411 2023-05-05 07:35:49.880817 proteus_cli-0.2.23/cli/datasets/preprocessor/well_init_keywords.json
+-rw-r--r--   0        0        0        0 2023-05-05 07:35:49.880817 proteus_cli-0.2.23/cli/datasets/sources/__init__.py
+-rw-r--r--   0        0        0     4737 2023-05-05 07:35:49.880817 proteus_cli-0.2.23/cli/datasets/sources/az.py
+-rw-r--r--   0        0        0      824 2023-05-05 07:35:49.880817 proteus_cli-0.2.23/cli/datasets/sources/common.py
+-rw-r--r--   0        0        0     2366 2023-05-05 07:35:49.880817 proteus_cli-0.2.23/cli/datasets/sources/local.py
+-rw-r--r--   0        0        0     1783 2023-05-05 07:35:49.880817 proteus_cli-0.2.23/cli/datasets/sources/s3.py
+-rw-r--r--   0        0        0     9008 2023-05-05 07:35:49.880817 proteus_cli-0.2.23/cli/datasets/upload.py
+-rw-r--r--   0        0        0        0 2023-05-05 07:35:49.880817 proteus_cli-0.2.23/cli/debugger/__init__.py
+-rw-r--r--   0        0        0     2265 2023-05-05 07:35:49.880817 proteus_cli-0.2.23/cli/debugger/commands.py
+-rw-r--r--   0        0        0     3926 2023-05-05 07:35:49.880817 proteus_cli-0.2.23/cli/debugger/init_keyword_check.py
+-rw-r--r--   0        0        0        0 2023-05-05 07:35:49.880817 proteus_cli-0.2.23/cli/debugger/restart_keyword_check.py
+-rw-r--r--   0        0        0        0 2023-05-05 07:35:49.880817 proteus_cli-0.2.23/cli/jobs/__init__.py
+-rw-r--r--   0        0        0     1283 2023-05-05 07:35:49.880817 proteus_cli-0.2.23/cli/jobs/commands.py
+-rw-r--r--   0        0        0     3026 2023-05-05 07:35:49.880817 proteus_cli-0.2.23/cli/jobs/list.py
+-rw-r--r--   0        0        0      100 2023-05-05 07:35:49.880817 proteus_cli-0.2.23/cli/runtime.py
+-rw-r--r--   0        0        0        0 2023-05-05 07:35:49.880817 proteus_cli-0.2.23/cli/simulations/__init__.py
+-rw-r--r--   0        0        0     2460 2023-05-05 07:35:49.880817 proteus_cli-0.2.23/cli/simulations/commands.py
+-rw-r--r--   0        0        0     7603 2023-05-05 07:35:49.880817 proteus_cli-0.2.23/cli/simulations/create.py
+-rw-r--r--   0        0        0     4119 2023-05-05 07:35:49.880817 proteus_cli-0.2.23/cli/simulations/dependencySolver.py
+-rw-r--r--   0        0        0     5190 2023-05-05 07:35:49.880817 proteus_cli-0.2.23/cli/simulations/opm.py
+-rw-r--r--   0        0        0      449 2023-05-05 07:35:49.880817 proteus_cli-0.2.23/logging.ini
+-rw-r--r--   0        0        0     1531 2023-05-05 07:35:49.884817 proteus_cli-0.2.23/pyproject.toml
+-rw-r--r--   0        0        0      744 1970-01-01 00:00:00.000000 proteus_cli-0.2.23/PKG-INFO
```

### Comparing `proteus_cli-0.2.22/cli/__init__.py` & `proteus_cli-0.2.23/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `proteus_cli-0.2.22/cli/api/decorators.py` & `proteus_cli-0.2.23/cli/api/decorators.py`

 * *Files identical despite different names*

### Comparing `proteus_cli-0.2.22/cli/api/hooks.py` & `proteus_cli-0.2.23/cli/api/hooks.py`

 * *Files identical despite different names*

### Comparing `proteus_cli-0.2.22/cli/buckets/commands.py` & `proteus_cli-0.2.23/cli/buckets/commands.py`

 * *Files identical despite different names*

### Comparing `proteus_cli-0.2.22/cli/config.py` & `proteus_cli-0.2.23/cli/config.py`

 * *Files 6% similar despite different names*

```diff
@@ -33,14 +33,15 @@
     RETRY_INTERVAL = 25  # Seconds
     REFRESH_GAP = 100  # Seconds
     S3_REGION = "eu-west-3"
     WORKERS_COUNT = 5
     WORKERS_DOWNLOAD_COUNT = 10
     AZURE_STORAGE_CONNECTION_STRING = os.getenv("AZURE_STORAGE_CONNECTION_STRING")
     AZURE_STORAGE_ACCOUNT_URL = os.getenv("AZURE_STORAGE_ACCOUNT_URL")
+    AZURE_SAS_TOKEN = os.getenv("AZURE_SAS_TOKEN")
 
     STRESS_ITERATIONS = 10
 
     DATASET_VERSION = {
         "major": os.getenv("DATASET_MAJOR_VERSION", 1),
         "minor": os.getenv("DATASET_MINOR_VERSION", 0),
         "patch": os.getenv("DATASET_PATCH_VERSION", 0),
```

### Comparing `proteus_cli-0.2.22/cli/datasets/commands.py` & `proteus_cli-0.2.23/cli/datasets/commands.py`

 * *Files identical despite different names*

### Comparing `proteus_cli-0.2.22/cli/datasets/preprocessor/config/__init__.py` & `proteus_cli-0.2.23/cli/datasets/preprocessor/config/__init__.py`

 * *Files identical despite different names*

### Comparing `proteus_cli-0.2.22/cli/datasets/preprocessor/config/case/cnn_pca.py` & `proteus_cli-0.2.23/cli/datasets/preprocessor/config/case/cnn_pca.py`

 * *Files identical despite different names*

### Comparing `proteus_cli-0.2.22/cli/datasets/preprocessor/config/case/hm.py` & `proteus_cli-0.2.23/cli/datasets/preprocessor/config/case/hm.py`

 * *Files identical despite different names*

### Comparing `proteus_cli-0.2.22/cli/datasets/preprocessor/config/case/well_model.py` & `proteus_cli-0.2.23/cli/datasets/preprocessor/config/case/well_model.py`

 * *Files identical despite different names*

### Comparing `proteus_cli-0.2.22/cli/datasets/preprocessor/config/common/cnn_pca.py` & `proteus_cli-0.2.23/cli/datasets/preprocessor/config/common/cnn_pca.py`

 * *Files identical despite different names*

### Comparing `proteus_cli-0.2.22/cli/datasets/preprocessor/config/common/hm.py` & `proteus_cli-0.2.23/cli/datasets/preprocessor/config/common/hm.py`

 * *Files identical despite different names*

### Comparing `proteus_cli-0.2.22/cli/datasets/preprocessor/config/common/well_model.py` & `proteus_cli-0.2.23/cli/datasets/preprocessor/config/common/well_model.py`

 * *Files identical despite different names*

### Comparing `proteus_cli-0.2.22/cli/datasets/preprocessor/config/default.py` & `proteus_cli-0.2.23/cli/datasets/preprocessor/config/default.py`

 * *Files identical despite different names*

### Comparing `proteus_cli-0.2.22/cli/datasets/preprocessor/config/step/hm.py` & `proteus_cli-0.2.23/cli/datasets/preprocessor/config/step/hm.py`

 * *Files identical despite different names*

### Comparing `proteus_cli-0.2.22/cli/datasets/preprocessor/init_keywords.json` & `proteus_cli-0.2.23/cli/datasets/preprocessor/init_keywords.json`

 * *Files identical despite different names*

### Comparing `proteus_cli-0.2.22/cli/datasets/preprocessor/preprocess_functions.py` & `proteus_cli-0.2.23/cli/datasets/preprocessor/preprocess_functions.py`

 * *Files identical despite different names*

### Comparing `proteus_cli-0.2.22/cli/datasets/preprocessor/process_step.py` & `proteus_cli-0.2.23/cli/datasets/preprocessor/process_step.py`

 * *Files identical despite different names*

### Comparing `proteus_cli-0.2.22/cli/datasets/preprocessor/utils.py` & `proteus_cli-0.2.23/cli/datasets/preprocessor/utils.py`

 * *Files identical despite different names*

### Comparing `proteus_cli-0.2.22/cli/datasets/sources/az.py` & `proteus_cli-0.2.23/cli/datasets/sources/az.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,17 +1,20 @@
 import re
 
 # from azure.storage.blob._models import BlobProperties as AzureBlobProperties
 from io import BytesIO
 
-from azure.identity import DefaultAzureCredential
 from azure.storage.blob import ContainerClient
+from azure.core.credentials import AzureSasCredential
 
 from .common import Source, SourcedItem
 from ... import proteus
+from cli.config import config
+
+AZURE_SAS_TOKEN = config.AZURE_SAS_TOKEN
 
 CONTENT_CHUNK_SIZE = 10 * 1024 * 1024
 
 
 class AZSource(Source):
     URI_re = re.compile(
         r"^https:\/\/(?P<bucket_name>.*\.windows\.net)\/" r"(?P<container_name>[^\/]*)(\/)?(?P<prefix>.*)?$"
@@ -21,15 +24,15 @@
         super().__init__(uri)
         match = self.URI_re.match(uri.rstrip("/"))
         assert match is not None, f"{uri} must be an s3 URI"
         container_name = match.groupdict()["container_name"]
         storage_url = f'https://{match.groupdict()["bucket_name"]}'
         self.container_client = ContainerClient(
             storage_url,
-            credential=DefaultAzureCredential(exclude_managed_identity_credential=True),
+            credential=AzureSasCredential(AZURE_SAS_TOKEN),
             container_name=container_name,
         )
 
     @proteus.may_insist_up_to(5, 1)
     def list_contents(self, starts_with="", ends_with=None):
         bucket_uri = self.uri
         match = self.URI_re.match(bucket_uri.rstrip("/"))
```

### Comparing `proteus_cli-0.2.22/cli/datasets/sources/common.py` & `proteus_cli-0.2.23/cli/datasets/sources/common.py`

 * *Files identical despite different names*

### Comparing `proteus_cli-0.2.22/cli/datasets/sources/local.py` & `proteus_cli-0.2.23/cli/datasets/sources/local.py`

 * *Files identical despite different names*

### Comparing `proteus_cli-0.2.22/cli/datasets/sources/s3.py` & `proteus_cli-0.2.23/cli/datasets/sources/s3.py`

 * *Files identical despite different names*

### Comparing `proteus_cli-0.2.22/cli/datasets/upload.py` & `proteus_cli-0.2.23/cli/datasets/upload.py`

 * *Files identical despite different names*

### Comparing `proteus_cli-0.2.22/cli/debugger/commands.py` & `proteus_cli-0.2.23/cli/debugger/commands.py`

 * *Files identical despite different names*

### Comparing `proteus_cli-0.2.22/cli/debugger/init_keyword_check.py` & `proteus_cli-0.2.23/cli/debugger/init_keyword_check.py`

 * *Files identical despite different names*

### Comparing `proteus_cli-0.2.22/cli/jobs/commands.py` & `proteus_cli-0.2.23/cli/jobs/commands.py`

 * *Files identical despite different names*

### Comparing `proteus_cli-0.2.22/cli/jobs/list.py` & `proteus_cli-0.2.23/cli/jobs/list.py`

 * *Files identical despite different names*

### Comparing `proteus_cli-0.2.22/cli/simulations/commands.py` & `proteus_cli-0.2.23/cli/simulations/commands.py`

 * *Files identical despite different names*

### Comparing `proteus_cli-0.2.22/cli/simulations/create.py` & `proteus_cli-0.2.23/cli/simulations/create.py`

 * *Files identical despite different names*

### Comparing `proteus_cli-0.2.22/cli/simulations/dependencySolver.py` & `proteus_cli-0.2.23/cli/simulations/dependencySolver.py`

 * *Files identical despite different names*

### Comparing `proteus_cli-0.2.22/cli/simulations/opm.py` & `proteus_cli-0.2.23/cli/simulations/opm.py`

 * *Files identical despite different names*

### Comparing `proteus_cli-0.2.22/pyproject.toml` & `proteus_cli-0.2.23/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "proteus-cli"
-version = "0.2.22"
+version = "0.2.23"
 description = ""
 authors = []
 packages = [
     {include="cli"},
     {include="logging.ini"}
 ]
```

### Comparing `proteus_cli-0.2.22/PKG-INFO` & `proteus_cli-0.2.23/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: proteus-cli
-Version: 0.2.22
+Version: 0.2.23
 Summary: 
 Requires-Python: >=3.8,<3.9
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Requires-Dist: azure-identity (>=1.12.0,<2.0.0)
 Requires-Dist: azure-storage-blob (>=12.8.1,<13.0.0)
 Requires-Dist: boto3 (>=1.17.79,<2.0.0)
```

