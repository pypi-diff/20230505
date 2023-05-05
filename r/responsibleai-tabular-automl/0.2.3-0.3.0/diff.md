# Comparing `tmp/responsibleai_tabular_automl-0.2.3.tar.gz` & `tmp/responsibleai_tabular_automl-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "responsibleai_tabular_automl-0.2.3.tar", last modified: Fri Apr  7 16:26:17 2023, max compression
+gzip compressed data, was "responsibleai_tabular_automl-0.3.0.tar", last modified: Fri May  5 21:47:35 2023, max compression
```

## Comparing `responsibleai_tabular_automl-0.2.3.tar` & `responsibleai_tabular_automl-0.3.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-04-07 16:26:17.522941 responsibleai_tabular_automl-0.2.3/
--rw-rw-rw-   0        0        0      778 2023-04-07 16:26:17.522941 responsibleai_tabular_automl-0.2.3/PKG-INFO
--rw-rw-rw-   0        0        0      134 2023-01-18 23:36:24.000000 responsibleai_tabular_automl-0.2.3/README.md
-drwxrwxrwx   0        0        0        0 2023-04-07 16:26:17.462535 responsibleai_tabular_automl-0.2.3/responsibleai_tabular_automl/
--rw-rw-rw-   0        0        0      284 2023-03-07 22:09:35.000000 responsibleai_tabular_automl-0.2.3/responsibleai_tabular_automl/__init__.py
--rw-rw-rw-   0        0        0     6104 2023-03-11 03:45:17.000000 responsibleai_tabular_automl-0.2.3/responsibleai_tabular_automl/_loggerfactory.py
--rw-rw-rw-   0        0        0    11682 2023-03-28 18:22:08.000000 responsibleai_tabular_automl-0.2.3/responsibleai_tabular_automl/automl_inference_run.py
--rw-rw-rw-   0        0        0    10433 2023-04-07 16:22:59.000000 responsibleai_tabular_automl-0.2.3/responsibleai_tabular_automl/rai_automl.py
--rw-rw-rw-   0        0        0      210 2023-04-07 16:23:50.000000 responsibleai_tabular_automl-0.2.3/responsibleai_tabular_automl/version.py
-drwxrwxrwx   0        0        0        0 2023-04-07 16:26:17.510432 responsibleai_tabular_automl-0.2.3/responsibleai_tabular_automl.egg-info/
--rw-rw-rw-   0        0        0      778 2023-04-07 16:26:17.000000 responsibleai_tabular_automl-0.2.3/responsibleai_tabular_automl.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      526 2023-04-07 16:26:17.000000 responsibleai_tabular_automl-0.2.3/responsibleai_tabular_automl.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-07 16:26:17.000000 responsibleai_tabular_automl-0.2.3/responsibleai_tabular_automl.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       72 2023-04-07 16:26:17.000000 responsibleai_tabular_automl-0.2.3/responsibleai_tabular_automl.egg-info/requires.txt
--rw-rw-rw-   0        0        0       29 2023-04-07 16:26:17.000000 responsibleai_tabular_automl-0.2.3/responsibleai_tabular_automl.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-07 16:26:17.522941 responsibleai_tabular_automl-0.2.3/setup.cfg
--rw-rw-rw-   0        0        0     1399 2023-03-07 22:09:35.000000 responsibleai_tabular_automl-0.2.3/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-07 16:26:17.522941 responsibleai_tabular_automl-0.2.3/tests/
--rw-rw-rw-   0        0        0     1654 2023-03-30 17:25:44.000000 responsibleai_tabular_automl-0.2.3/tests/test_rai_automl.py
+drwxrwxrwx   0        0        0        0 2023-05-05 21:47:35.551896 responsibleai_tabular_automl-0.3.0/
+-rw-rw-rw-   0        0        0      778 2023-05-05 21:47:35.551896 responsibleai_tabular_automl-0.3.0/PKG-INFO
+-rw-rw-rw-   0        0        0      134 2023-01-18 23:36:24.000000 responsibleai_tabular_automl-0.3.0/README.md
+drwxrwxrwx   0        0        0        0 2023-05-05 21:47:35.511897 responsibleai_tabular_automl-0.3.0/responsibleai_tabular_automl/
+-rw-rw-rw-   0        0        0      284 2023-03-07 22:09:35.000000 responsibleai_tabular_automl-0.3.0/responsibleai_tabular_automl/__init__.py
+-rw-rw-rw-   0        0        0     6104 2023-05-04 20:34:24.000000 responsibleai_tabular_automl-0.3.0/responsibleai_tabular_automl/_loggerfactory.py
+-rw-rw-rw-   0        0        0    12436 2023-05-05 17:35:09.000000 responsibleai_tabular_automl-0.3.0/responsibleai_tabular_automl/automl_inference_run.py
+-rw-rw-rw-   0        0        0    10641 2023-05-05 21:28:52.000000 responsibleai_tabular_automl-0.3.0/responsibleai_tabular_automl/rai_automl.py
+-rw-rw-rw-   0        0        0      210 2023-05-05 21:40:10.000000 responsibleai_tabular_automl-0.3.0/responsibleai_tabular_automl/version.py
+drwxrwxrwx   0        0        0        0 2023-05-05 21:47:35.536927 responsibleai_tabular_automl-0.3.0/responsibleai_tabular_automl.egg-info/
+-rw-rw-rw-   0        0        0      778 2023-05-05 21:47:35.000000 responsibleai_tabular_automl-0.3.0/responsibleai_tabular_automl.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      526 2023-05-05 21:47:35.000000 responsibleai_tabular_automl-0.3.0/responsibleai_tabular_automl.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-05 21:47:35.000000 responsibleai_tabular_automl-0.3.0/responsibleai_tabular_automl.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       72 2023-05-05 21:47:35.000000 responsibleai_tabular_automl-0.3.0/responsibleai_tabular_automl.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       29 2023-05-05 21:47:35.000000 responsibleai_tabular_automl-0.3.0/responsibleai_tabular_automl.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-05 21:47:35.551896 responsibleai_tabular_automl-0.3.0/setup.cfg
+-rw-rw-rw-   0        0        0     1399 2023-03-07 22:09:35.000000 responsibleai_tabular_automl-0.3.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-05 21:47:35.549897 responsibleai_tabular_automl-0.3.0/tests/
+-rw-rw-rw-   0        0        0     1654 2023-05-03 22:59:55.000000 responsibleai_tabular_automl-0.3.0/tests/test_rai_automl.py
```

### Comparing `responsibleai_tabular_automl-0.2.3/PKG-INFO` & `responsibleai_tabular_automl-0.3.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: responsibleai_tabular_automl
-Version: 0.2.3
+Version: 0.3.0
 Summary: SDK for computing RAI insights for AutoML models.
 Home-page: 
 Author: Gaurav Gupta, Ke Xu
 Author-email: raiwidgets-maintain@microsoft.com
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `responsibleai_tabular_automl-0.2.3/responsibleai_tabular_automl/_loggerfactory.py` & `responsibleai_tabular_automl-0.3.0/responsibleai_tabular_automl/_loggerfactory.py`

 * *Files identical despite different names*

### Comparing `responsibleai_tabular_automl-0.2.3/responsibleai_tabular_automl/automl_inference_run.py` & `responsibleai_tabular_automl-0.3.0/responsibleai_tabular_automl/automl_inference_run.py`

 * *Files 8% similar despite different names*

```diff
@@ -280,15 +280,15 @@
     if hasattr(model, "classes_"):
         classes = _serialize_json_safe(list(model.classes_))
         return classes
     else:
         return None
 
 
-def upload_rai_artifacts_to_automl_child_run(
+def upload_rai_artifacts_to_automl_child_run_internal(
     parent_run_id: str, child_run_id: str
 ) -> None:
     X_raw, y, X_raw_valid, y_valid = automl_download_raw_data(parent_run_id)
     target_column, task_type = get_automl_task_type_and_target_column_name(
         parent_run_id
     )
     (
@@ -335,10 +335,34 @@
         json.dump(metadata, fp)
 
     run = Run.get_context()
     child_run = run.experiment.workspace.get_run(child_run_id)
     child_run.upload_folder("outputs/rai", "rai")
 
 
+def upload_rai_artifacts_to_automl_child_run(
+    parent_run_id: str, child_run_id: str
+) -> None:
+    try:
+        from azureml.automl.runtime.rai import (
+            inference_run as rai_inference_run,
+        )
+
+        execute_using_automl_sdk = True
+    except ImportError:
+        execute_using_automl_sdk = False
+
+    if execute_using_automl_sdk:
+        print("Using automl to compute prerequisites")
+        rai_inference_run.upload_rai_artifacts_to_automl_child_run(
+            parent_run_id, child_run_id
+        )
+    else:
+        print("Using proxy script for automl to compute prerequisites")
+        upload_rai_artifacts_to_automl_child_run_internal(
+            parent_run_id, child_run_id
+        )
+
+
 upload_rai_artifacts_to_automl_child_run(
     "<<automl_parent_run_id>>", "<<automl_child_run_id>>"
 )
```

### Comparing `responsibleai_tabular_automl-0.2.3/responsibleai_tabular_automl/rai_automl.py` & `responsibleai_tabular_automl-0.3.0/responsibleai_tabular_automl/rai_automl.py`

 * *Files 3% similar despite different names*

```diff
@@ -18,18 +18,19 @@
     PredictionsModelWrapperRegression,
 )
 
 from azureml.core.runconfig import RunConfiguration
 from azureml.core.run import Run
 from responsibleai import RAIInsights
 from responsibleai.serialization_utilities import serialize_json_safe
+from responsibleai.feature_metadata import FeatureMetadata
 from pathlib import Path
 from azureml.core import ScriptRunConfig
 
-from ._loggerfactory import _LoggerFactory, track
+from responsibleai_tabular_automl._loggerfactory import _LoggerFactory, track
 
 _ai_logger = None
 submit_locally_managed_run = False
 
 
 def _get_logger():
     global _ai_logger
@@ -111,24 +112,27 @@
         model_wrapper = PredictionsModelWrapperRegression(
             all_data, model_predict_output
         )
 
     train = train.drop(columns=dropped_features)
     test = test.drop(columns=dropped_features)
     if len(text_features) == 0 and len(datetime_features) == 0:
-        _ai_logger.info("Generating RAI insights for {} samples.".format(
-            len(test)))
+        _ai_logger.info(
+            "Generating RAI insights for {} samples.".format(len(test))
+        )
+        feature_metadata = FeatureMetadata(
+            categorical_features=categorical_features)
         rai_insights = RAIInsights(
             model=model_wrapper,
             train=train,
             test=test,
             target_column=target_column_name,
-            categorical_features=categorical_features,
             task_type=task_type,
             classes=classes,
+            feature_metadata=feature_metadata
         )
         rai_insights.explainer.add()
         rai_insights.error_analysis.add()
         rai_insights.compute()
         rai_insights.save("dashboard")
         current_run.upload_folder("dashboard", "dashboard")
 
@@ -140,18 +144,20 @@
         with open(json_filename, "w") as json_file:
             json.dump(rai_dict, json_file)
         current_run.upload_folder("ux_json", "ux_json")
         automl_child_run.tag("model_rai", "True")
         print("Successfully generated and uploaded the RAI insights")
         _ai_logger.info("Successfully generated and uploaded the RAI insights")
     else:
-        warnings.warn("Currently RAI is not supported for "
-                      "text and datetime features")
-        _ai_logger.info("Currently RAI is not supported for "
-                        "text and datetime features")
+        warnings.warn(
+            "Currently RAI is not supported for " "text and datetime features"
+        )
+        _ai_logger.info(
+            "Currently RAI is not supported for " "text and datetime features"
+        )
     current_run.complete()
 
 
 @track(_get_logger)
 def _create_project_folder(
     automl_parent_run_id: str, automl_child_run_id: str
 ):
@@ -245,56 +251,52 @@
     ]
     success, output = call_with_output(command)
 
     if not success:
         _ai_logger.info("Error running automl script in conda environment")
         raise Exception(output)
 
-    command = [
-        "conda",
-        "env",
-        "remove",
-        "--name",
-        automl_env_name,
-        "-y"
-    ]
+    command = ["conda", "env", "remove", "--name", automl_env_name, "-y"]
     success, output = call_with_output(command)
     print("Successfully generated predictions for AutoML model")
     _ai_logger.info("Successfully generated predictions for AutoML model")
 
 
 @track(_get_logger)
 def compute_and_upload_rai_insights(
     automl_parent_run_id: Optional[str] = None,
-    automl_child_run_id: Optional[str] = None
+    automl_child_run_id: Optional[str] = None,
 ):
     print("The automl child run-id is: " + str(automl_child_run_id))
+    _ai_logger.info("The automl child run-id is: " + str(automl_child_run_id))
     print("The automl parent run-id is: " + str(automl_parent_run_id))
 
     rai_run = Run.get_context()
     print("The current run-id is: " + rai_run.id)
 
     if submit_locally_managed_run:
-        _ai_logger.info("Submitting locally managed run to compute AutoML "
-                        "artifacts.")
+        _ai_logger.info(
+            "Submitting locally managed run to compute AutoML " "artifacts."
+        )
         project_folder = _create_project_folder(
             automl_parent_run_id, automl_child_run_id
         )
         run_configuration = _create_run_configuration(
             automl_child_run_id, rai_run.experiment.workspace
         )
 
         src = ScriptRunConfig(
             source_directory=project_folder, run_config=run_configuration
         )
         automl_inference_run = rai_run.experiment.submit(config=src)
         automl_inference_run.wait_for_completion()
     else:
-        _ai_logger.info("Creating local conda environment to compute "
-                        "AutoML artifacts.")
+        _ai_logger.info(
+            "Creating local conda environment to compute " "AutoML artifacts."
+        )
         # Create conda env from native commands and submit script
         project_folder = _create_project_folder(
             automl_parent_run_id, automl_child_run_id
         )
 
         execute_automl_inference_script(
             automl_child_run_id, rai_run.experiment.workspace
```

### Comparing `responsibleai_tabular_automl-0.2.3/responsibleai_tabular_automl.egg-info/PKG-INFO` & `responsibleai_tabular_automl-0.3.0/responsibleai_tabular_automl.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: responsibleai-tabular-automl
-Version: 0.2.3
+Version: 0.3.0
 Summary: SDK for computing RAI insights for AutoML models.
 Home-page: 
 Author: Gaurav Gupta, Ke Xu
 Author-email: raiwidgets-maintain@microsoft.com
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `responsibleai_tabular_automl-0.2.3/responsibleai_tabular_automl.egg-info/SOURCES.txt` & `responsibleai_tabular_automl-0.3.0/responsibleai_tabular_automl.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `responsibleai_tabular_automl-0.2.3/setup.py` & `responsibleai_tabular_automl-0.3.0/setup.py`

 * *Files identical despite different names*

### Comparing `responsibleai_tabular_automl-0.2.3/tests/test_rai_automl.py` & `responsibleai_tabular_automl-0.3.0/tests/test_rai_automl.py`

 * *Files identical despite different names*

