# Comparing `tmp/proteus_cli-0.2.23.tar.gz` & `tmp/proteus_cli-0.2.25.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "proteus_cli-0.2.23.tar", max compression
+gzip compressed data, was "proteus_cli-0.2.25.tar", max compression
```

## Comparing `proteus_cli-0.2.23.tar` & `proteus_cli-0.2.25.tar`

### file list

```diff
@@ -1,51 +1,51 @@
--rw-r--r--   0        0        0     1330 2023-05-05 07:35:49.880817 proteus_cli-0.2.23/cli/__init__.py
--rw-r--r--   0        0        0      384 2023-05-05 07:35:49.880817 proteus_cli-0.2.23/cli/api/__init__.py
--rw-r--r--   0        0        0     1784 2023-05-05 07:35:49.880817 proteus_cli-0.2.23/cli/api/decorators.py
--rw-r--r--   0        0        0      849 2023-05-05 07:35:49.880817 proteus_cli-0.2.23/cli/api/hooks.py
--rw-r--r--   0        0        0        0 2023-05-05 07:35:49.880817 proteus_cli-0.2.23/cli/buckets/__init__.py
--rw-r--r--   0        0        0     1092 2023-05-05 07:35:49.880817 proteus_cli-0.2.23/cli/buckets/commands.py
--rw-r--r--   0        0        0     2621 2023-05-05 07:35:49.880817 proteus_cli-0.2.23/cli/config.py
--rw-r--r--   0        0        0        0 2023-05-05 07:35:49.880817 proteus_cli-0.2.23/cli/datasets/__init__.py
--rw-r--r--   0        0        0     1332 2023-05-05 07:35:49.880817 proteus_cli-0.2.23/cli/datasets/commands.py
--rw-r--r--   0        0        0        0 2023-05-05 07:35:49.880817 proteus_cli-0.2.23/cli/datasets/preprocessor/__init__.py
--rw-r--r--   0        0        0      939 2023-05-05 07:35:49.880817 proteus_cli-0.2.23/cli/datasets/preprocessor/config/__init__.py
--rw-r--r--   0        0        0      323 2023-05-05 07:35:49.880817 proteus_cli-0.2.23/cli/datasets/preprocessor/config/case/__init__.py
--rw-r--r--   0        0        0      851 2023-05-05 07:35:49.880817 proteus_cli-0.2.23/cli/datasets/preprocessor/config/case/cnn_pca.py
--rw-r--r--   0        0        0     3447 2023-05-05 07:35:49.880817 proteus_cli-0.2.23/cli/datasets/preprocessor/config/case/hm.py
--rw-r--r--   0        0        0     3054 2023-05-05 07:35:49.880817 proteus_cli-0.2.23/cli/datasets/preprocessor/config/case/well_model.py
--rw-r--r--   0        0        0      446 2023-05-05 07:35:49.880817 proteus_cli-0.2.23/cli/datasets/preprocessor/config/common/__init__.py
--rw-r--r--   0        0        0     3238 2023-05-05 07:35:49.880817 proteus_cli-0.2.23/cli/datasets/preprocessor/config/common/cnn_pca.py
--rw-r--r--   0        0        0     2009 2023-05-05 07:35:49.880817 proteus_cli-0.2.23/cli/datasets/preprocessor/config/common/hm.py
--rw-r--r--   0        0        0     1542 2023-05-05 07:35:49.880817 proteus_cli-0.2.23/cli/datasets/preprocessor/config/common/well_model.py
--rw-r--r--   0        0        0     2665 2023-05-05 07:35:49.880817 proteus_cli-0.2.23/cli/datasets/preprocessor/config/default.py
--rw-r--r--   0        0        0      418 2023-05-05 07:35:49.880817 proteus_cli-0.2.23/cli/datasets/preprocessor/config/step/__init__.py
--rw-r--r--   0        0        0      125 2023-05-05 07:35:49.880817 proteus_cli-0.2.23/cli/datasets/preprocessor/config/step/cnn_pca.py
--rw-r--r--   0        0        0     2415 2023-05-05 07:35:49.880817 proteus_cli-0.2.23/cli/datasets/preprocessor/config/step/hm.py
--rw-r--r--   0        0        0      128 2023-05-05 07:35:49.880817 proteus_cli-0.2.23/cli/datasets/preprocessor/config/step/well_model.py
--rw-r--r--   0        0        0      673 2023-05-05 07:35:49.880817 proteus_cli-0.2.23/cli/datasets/preprocessor/init_keywords.json
--rw-r--r--   0        0        0    13633 2023-05-05 07:35:49.880817 proteus_cli-0.2.23/cli/datasets/preprocessor/preprocess_functions.py
--rw-r--r--   0        0        0     4446 2023-05-05 07:35:49.880817 proteus_cli-0.2.23/cli/datasets/preprocessor/process_step.py
--rw-r--r--   0        0        0     8185 2023-05-05 07:35:49.880817 proteus_cli-0.2.23/cli/datasets/preprocessor/utils.py
--rw-r--r--   0        0        0      411 2023-05-05 07:35:49.880817 proteus_cli-0.2.23/cli/datasets/preprocessor/well_init_keywords.json
--rw-r--r--   0        0        0        0 2023-05-05 07:35:49.880817 proteus_cli-0.2.23/cli/datasets/sources/__init__.py
--rw-r--r--   0        0        0     4737 2023-05-05 07:35:49.880817 proteus_cli-0.2.23/cli/datasets/sources/az.py
--rw-r--r--   0        0        0      824 2023-05-05 07:35:49.880817 proteus_cli-0.2.23/cli/datasets/sources/common.py
--rw-r--r--   0        0        0     2366 2023-05-05 07:35:49.880817 proteus_cli-0.2.23/cli/datasets/sources/local.py
--rw-r--r--   0        0        0     1783 2023-05-05 07:35:49.880817 proteus_cli-0.2.23/cli/datasets/sources/s3.py
--rw-r--r--   0        0        0     9008 2023-05-05 07:35:49.880817 proteus_cli-0.2.23/cli/datasets/upload.py
--rw-r--r--   0        0        0        0 2023-05-05 07:35:49.880817 proteus_cli-0.2.23/cli/debugger/__init__.py
--rw-r--r--   0        0        0     2265 2023-05-05 07:35:49.880817 proteus_cli-0.2.23/cli/debugger/commands.py
--rw-r--r--   0        0        0     3926 2023-05-05 07:35:49.880817 proteus_cli-0.2.23/cli/debugger/init_keyword_check.py
--rw-r--r--   0        0        0        0 2023-05-05 07:35:49.880817 proteus_cli-0.2.23/cli/debugger/restart_keyword_check.py
--rw-r--r--   0        0        0        0 2023-05-05 07:35:49.880817 proteus_cli-0.2.23/cli/jobs/__init__.py
--rw-r--r--   0        0        0     1283 2023-05-05 07:35:49.880817 proteus_cli-0.2.23/cli/jobs/commands.py
--rw-r--r--   0        0        0     3026 2023-05-05 07:35:49.880817 proteus_cli-0.2.23/cli/jobs/list.py
--rw-r--r--   0        0        0      100 2023-05-05 07:35:49.880817 proteus_cli-0.2.23/cli/runtime.py
--rw-r--r--   0        0        0        0 2023-05-05 07:35:49.880817 proteus_cli-0.2.23/cli/simulations/__init__.py
--rw-r--r--   0        0        0     2460 2023-05-05 07:35:49.880817 proteus_cli-0.2.23/cli/simulations/commands.py
--rw-r--r--   0        0        0     7603 2023-05-05 07:35:49.880817 proteus_cli-0.2.23/cli/simulations/create.py
--rw-r--r--   0        0        0     4119 2023-05-05 07:35:49.880817 proteus_cli-0.2.23/cli/simulations/dependencySolver.py
--rw-r--r--   0        0        0     5190 2023-05-05 07:35:49.880817 proteus_cli-0.2.23/cli/simulations/opm.py
--rw-r--r--   0        0        0      449 2023-05-05 07:35:49.880817 proteus_cli-0.2.23/logging.ini
--rw-r--r--   0        0        0     1531 2023-05-05 07:35:49.884817 proteus_cli-0.2.23/pyproject.toml
--rw-r--r--   0        0        0      744 1970-01-01 00:00:00.000000 proteus_cli-0.2.23/PKG-INFO
+-rw-r--r--   0        0        0     1330 2023-05-05 10:15:26.286673 proteus_cli-0.2.25/cli/__init__.py
+-rw-r--r--   0        0        0      384 2023-05-05 10:15:26.286673 proteus_cli-0.2.25/cli/api/__init__.py
+-rw-r--r--   0        0        0     1784 2023-05-05 10:15:26.286673 proteus_cli-0.2.25/cli/api/decorators.py
+-rw-r--r--   0        0        0      849 2023-05-05 10:15:26.286673 proteus_cli-0.2.25/cli/api/hooks.py
+-rw-r--r--   0        0        0        0 2023-05-05 10:15:26.286673 proteus_cli-0.2.25/cli/buckets/__init__.py
+-rw-r--r--   0        0        0     1092 2023-05-05 10:15:26.286673 proteus_cli-0.2.25/cli/buckets/commands.py
+-rw-r--r--   0        0        0     2621 2023-05-05 10:15:26.286673 proteus_cli-0.2.25/cli/config.py
+-rw-r--r--   0        0        0        0 2023-05-05 10:15:26.286673 proteus_cli-0.2.25/cli/datasets/__init__.py
+-rw-r--r--   0        0        0     1332 2023-05-05 10:15:26.286673 proteus_cli-0.2.25/cli/datasets/commands.py
+-rw-r--r--   0        0        0        0 2023-05-05 10:15:26.286673 proteus_cli-0.2.25/cli/datasets/preprocessor/__init__.py
+-rw-r--r--   0        0        0      939 2023-05-05 10:15:26.286673 proteus_cli-0.2.25/cli/datasets/preprocessor/config/__init__.py
+-rw-r--r--   0        0        0      323 2023-05-05 10:15:26.286673 proteus_cli-0.2.25/cli/datasets/preprocessor/config/case/__init__.py
+-rw-r--r--   0        0        0      851 2023-05-05 10:15:26.286673 proteus_cli-0.2.25/cli/datasets/preprocessor/config/case/cnn_pca.py
+-rw-r--r--   0        0        0     3447 2023-05-05 10:15:26.286673 proteus_cli-0.2.25/cli/datasets/preprocessor/config/case/hm.py
+-rw-r--r--   0        0        0     3054 2023-05-05 10:15:26.286673 proteus_cli-0.2.25/cli/datasets/preprocessor/config/case/well_model.py
+-rw-r--r--   0        0        0      446 2023-05-05 10:15:26.286673 proteus_cli-0.2.25/cli/datasets/preprocessor/config/common/__init__.py
+-rw-r--r--   0        0        0     3238 2023-05-05 10:15:26.286673 proteus_cli-0.2.25/cli/datasets/preprocessor/config/common/cnn_pca.py
+-rw-r--r--   0        0        0     2009 2023-05-05 10:15:26.286673 proteus_cli-0.2.25/cli/datasets/preprocessor/config/common/hm.py
+-rw-r--r--   0        0        0     1542 2023-05-05 10:15:26.286673 proteus_cli-0.2.25/cli/datasets/preprocessor/config/common/well_model.py
+-rw-r--r--   0        0        0     2665 2023-05-05 10:15:26.286673 proteus_cli-0.2.25/cli/datasets/preprocessor/config/default.py
+-rw-r--r--   0        0        0      418 2023-05-05 10:15:26.286673 proteus_cli-0.2.25/cli/datasets/preprocessor/config/step/__init__.py
+-rw-r--r--   0        0        0      125 2023-05-05 10:15:26.286673 proteus_cli-0.2.25/cli/datasets/preprocessor/config/step/cnn_pca.py
+-rw-r--r--   0        0        0     2415 2023-05-05 10:15:26.286673 proteus_cli-0.2.25/cli/datasets/preprocessor/config/step/hm.py
+-rw-r--r--   0        0        0      128 2023-05-05 10:15:26.286673 proteus_cli-0.2.25/cli/datasets/preprocessor/config/step/well_model.py
+-rw-r--r--   0        0        0      673 2023-05-05 10:15:26.286673 proteus_cli-0.2.25/cli/datasets/preprocessor/init_keywords.json
+-rw-r--r--   0        0        0    13633 2023-05-05 10:15:26.286673 proteus_cli-0.2.25/cli/datasets/preprocessor/preprocess_functions.py
+-rw-r--r--   0        0        0     4446 2023-05-05 10:15:26.286673 proteus_cli-0.2.25/cli/datasets/preprocessor/process_step.py
+-rw-r--r--   0        0        0     8185 2023-05-05 10:15:26.286673 proteus_cli-0.2.25/cli/datasets/preprocessor/utils.py
+-rw-r--r--   0        0        0      411 2023-05-05 10:15:26.286673 proteus_cli-0.2.25/cli/datasets/preprocessor/well_init_keywords.json
+-rw-r--r--   0        0        0        0 2023-05-05 10:15:26.286673 proteus_cli-0.2.25/cli/datasets/sources/__init__.py
+-rw-r--r--   0        0        0     4737 2023-05-05 10:15:26.286673 proteus_cli-0.2.25/cli/datasets/sources/az.py
+-rw-r--r--   0        0        0      824 2023-05-05 10:15:26.286673 proteus_cli-0.2.25/cli/datasets/sources/common.py
+-rw-r--r--   0        0        0     2366 2023-05-05 10:15:26.286673 proteus_cli-0.2.25/cli/datasets/sources/local.py
+-rw-r--r--   0        0        0     1783 2023-05-05 10:15:26.286673 proteus_cli-0.2.25/cli/datasets/sources/s3.py
+-rw-r--r--   0        0        0     9008 2023-05-05 10:15:26.286673 proteus_cli-0.2.25/cli/datasets/upload.py
+-rw-r--r--   0        0        0        0 2023-05-05 10:15:26.286673 proteus_cli-0.2.25/cli/debugger/__init__.py
+-rw-r--r--   0        0        0     2265 2023-05-05 10:15:26.286673 proteus_cli-0.2.25/cli/debugger/commands.py
+-rw-r--r--   0        0        0     3926 2023-05-05 10:15:26.286673 proteus_cli-0.2.25/cli/debugger/init_keyword_check.py
+-rw-r--r--   0        0        0        0 2023-05-05 10:15:26.286673 proteus_cli-0.2.25/cli/debugger/restart_keyword_check.py
+-rw-r--r--   0        0        0        0 2023-05-05 10:15:26.290673 proteus_cli-0.2.25/cli/jobs/__init__.py
+-rw-r--r--   0        0        0     1283 2023-05-05 10:15:26.290673 proteus_cli-0.2.25/cli/jobs/commands.py
+-rw-r--r--   0        0        0     3026 2023-05-05 10:15:26.290673 proteus_cli-0.2.25/cli/jobs/list.py
+-rw-r--r--   0        0        0      100 2023-05-05 10:15:26.290673 proteus_cli-0.2.25/cli/runtime.py
+-rw-r--r--   0        0        0        0 2023-05-05 10:15:26.290673 proteus_cli-0.2.25/cli/simulations/__init__.py
+-rw-r--r--   0        0        0     2460 2023-05-05 10:15:26.290673 proteus_cli-0.2.25/cli/simulations/commands.py
+-rw-r--r--   0        0        0     7603 2023-05-05 10:15:26.290673 proteus_cli-0.2.25/cli/simulations/create.py
+-rw-r--r--   0        0        0     4119 2023-05-05 10:15:26.290673 proteus_cli-0.2.25/cli/simulations/dependencySolver.py
+-rw-r--r--   0        0        0     5190 2023-05-05 10:15:26.290673 proteus_cli-0.2.25/cli/simulations/opm.py
+-rw-r--r--   0        0        0      449 2023-05-05 10:15:26.290673 proteus_cli-0.2.25/logging.ini
+-rw-r--r--   0        0        0     1533 2023-05-05 10:15:26.290673 proteus_cli-0.2.25/pyproject.toml
+-rw-r--r--   0        0        0      758 1970-01-01 00:00:00.000000 proteus_cli-0.2.25/PKG-INFO
```

### Comparing `proteus_cli-0.2.23/cli/__init__.py` & `proteus_cli-0.2.25/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `proteus_cli-0.2.23/cli/api/decorators.py` & `proteus_cli-0.2.25/cli/api/decorators.py`

 * *Files identical despite different names*

### Comparing `proteus_cli-0.2.23/cli/api/hooks.py` & `proteus_cli-0.2.25/cli/api/hooks.py`

 * *Files identical despite different names*

### Comparing `proteus_cli-0.2.23/cli/buckets/commands.py` & `proteus_cli-0.2.25/cli/buckets/commands.py`

 * *Files identical despite different names*

### Comparing `proteus_cli-0.2.23/cli/config.py` & `proteus_cli-0.2.25/cli/config.py`

 * *Files identical despite different names*

### Comparing `proteus_cli-0.2.23/cli/datasets/commands.py` & `proteus_cli-0.2.25/cli/datasets/commands.py`

 * *Files identical despite different names*

### Comparing `proteus_cli-0.2.23/cli/datasets/preprocessor/config/__init__.py` & `proteus_cli-0.2.25/cli/datasets/preprocessor/config/__init__.py`

 * *Files identical despite different names*

### Comparing `proteus_cli-0.2.23/cli/datasets/preprocessor/config/case/cnn_pca.py` & `proteus_cli-0.2.25/cli/datasets/preprocessor/config/case/cnn_pca.py`

 * *Files identical despite different names*

### Comparing `proteus_cli-0.2.23/cli/datasets/preprocessor/config/case/hm.py` & `proteus_cli-0.2.25/cli/datasets/preprocessor/config/case/hm.py`

 * *Files identical despite different names*

### Comparing `proteus_cli-0.2.23/cli/datasets/preprocessor/config/case/well_model.py` & `proteus_cli-0.2.25/cli/datasets/preprocessor/config/case/well_model.py`

 * *Files identical despite different names*

### Comparing `proteus_cli-0.2.23/cli/datasets/preprocessor/config/common/cnn_pca.py` & `proteus_cli-0.2.25/cli/datasets/preprocessor/config/common/cnn_pca.py`

 * *Files identical despite different names*

### Comparing `proteus_cli-0.2.23/cli/datasets/preprocessor/config/common/hm.py` & `proteus_cli-0.2.25/cli/datasets/preprocessor/config/common/hm.py`

 * *Files identical despite different names*

### Comparing `proteus_cli-0.2.23/cli/datasets/preprocessor/config/common/well_model.py` & `proteus_cli-0.2.25/cli/datasets/preprocessor/config/common/well_model.py`

 * *Files identical despite different names*

### Comparing `proteus_cli-0.2.23/cli/datasets/preprocessor/config/default.py` & `proteus_cli-0.2.25/cli/datasets/preprocessor/config/default.py`

 * *Files identical despite different names*

### Comparing `proteus_cli-0.2.23/cli/datasets/preprocessor/config/step/hm.py` & `proteus_cli-0.2.25/cli/datasets/preprocessor/config/step/hm.py`

 * *Files identical despite different names*

### Comparing `proteus_cli-0.2.23/cli/datasets/preprocessor/init_keywords.json` & `proteus_cli-0.2.25/cli/datasets/preprocessor/init_keywords.json`

 * *Files identical despite different names*

### Comparing `proteus_cli-0.2.23/cli/datasets/preprocessor/preprocess_functions.py` & `proteus_cli-0.2.25/cli/datasets/preprocessor/preprocess_functions.py`

 * *Files identical despite different names*

### Comparing `proteus_cli-0.2.23/cli/datasets/preprocessor/process_step.py` & `proteus_cli-0.2.25/cli/datasets/preprocessor/process_step.py`

 * *Files identical despite different names*

### Comparing `proteus_cli-0.2.23/cli/datasets/preprocessor/utils.py` & `proteus_cli-0.2.25/cli/datasets/preprocessor/utils.py`

 * *Files identical despite different names*

### Comparing `proteus_cli-0.2.23/cli/datasets/sources/az.py` & `proteus_cli-0.2.25/cli/datasets/sources/az.py`

 * *Files identical despite different names*

### Comparing `proteus_cli-0.2.23/cli/datasets/sources/common.py` & `proteus_cli-0.2.25/cli/datasets/sources/common.py`

 * *Files identical despite different names*

### Comparing `proteus_cli-0.2.23/cli/datasets/sources/local.py` & `proteus_cli-0.2.25/cli/datasets/sources/local.py`

 * *Files identical despite different names*

### Comparing `proteus_cli-0.2.23/cli/datasets/sources/s3.py` & `proteus_cli-0.2.25/cli/datasets/sources/s3.py`

 * *Files identical despite different names*

### Comparing `proteus_cli-0.2.23/cli/datasets/upload.py` & `proteus_cli-0.2.25/cli/datasets/upload.py`

 * *Files identical despite different names*

### Comparing `proteus_cli-0.2.23/cli/debugger/commands.py` & `proteus_cli-0.2.25/cli/debugger/commands.py`

 * *Files identical despite different names*

### Comparing `proteus_cli-0.2.23/cli/debugger/init_keyword_check.py` & `proteus_cli-0.2.25/cli/debugger/init_keyword_check.py`

 * *Files identical despite different names*

### Comparing `proteus_cli-0.2.23/cli/jobs/commands.py` & `proteus_cli-0.2.25/cli/jobs/commands.py`

 * *Files identical despite different names*

### Comparing `proteus_cli-0.2.23/cli/jobs/list.py` & `proteus_cli-0.2.25/cli/jobs/list.py`

 * *Files identical despite different names*

### Comparing `proteus_cli-0.2.23/cli/simulations/commands.py` & `proteus_cli-0.2.25/cli/simulations/commands.py`

 * *Files identical despite different names*

### Comparing `proteus_cli-0.2.23/cli/simulations/create.py` & `proteus_cli-0.2.25/cli/simulations/create.py`

 * *Files identical despite different names*

### Comparing `proteus_cli-0.2.23/cli/simulations/dependencySolver.py` & `proteus_cli-0.2.25/cli/simulations/dependencySolver.py`

 * *Files identical despite different names*

### Comparing `proteus_cli-0.2.23/cli/simulations/opm.py` & `proteus_cli-0.2.25/cli/simulations/opm.py`

 * *Files identical despite different names*

### Comparing `proteus_cli-0.2.23/pyproject.toml` & `proteus_cli-0.2.25/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "proteus-cli"
-version = "0.2.23"
+version = "0.2.25"
 description = ""
 authors = []
 packages = [
     {include="cli"},
     {include="logging.ini"}
 ]
 
@@ -17,16 +17,16 @@
 boto3 = "^1.17.79"
 tqdm = "^4.61.0"
 tabulate = "^0.8.9"
 azure-storage-blob = "^12.8.1"
 readchar = "^3.0.4"
 azure-identity = "^1.12.0"
 markupsafe = "2.0.1"
-proteus-runtime = "0.2.17"
-proteus-preprocessing = "0.2.11"
+proteus-runtime = "^0.2.17"
+proteus-preprocessing = "^0.2.14"
 
 [tool.poetry.dev-dependencies]
 black = "^22.1.0"
 pre-commit = "^2.9.3"
 pytest-mock = "^3.5.1"
 requests-mock = "^1.8.0"
 pytest-bdd = "^5.0.0"
```

