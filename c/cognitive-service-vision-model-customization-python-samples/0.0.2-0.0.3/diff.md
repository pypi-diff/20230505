# Comparing `tmp/cognitive-service-vision-model-customization-python-samples-0.0.2.tar.gz` & `tmp/cognitive-service-vision-model-customization-python-samples-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cognitive-service-vision-model-customization-python-samples-0.0.2.tar", last modified: Tue Mar 21 02:32:42 2023, max compression
+gzip compressed data, was "cognitive-service-vision-model-customization-python-samples-0.0.3.tar", last modified: Fri May  5 16:18:35 2023, max compression
```

## Comparing `cognitive-service-vision-model-customization-python-samples-0.0.2.tar` & `cognitive-service-vision-model-customization-python-samples-0.0.3.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 02:32:42.586088 cognitive-service-vision-model-customization-python-samples-0.0.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-03-21 02:32:25.000000 cognitive-service-vision-model-customization-python-samples-0.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1140 2023-03-21 02:32:25.000000 cognitive-service-vision-model-customization-python-samples-0.0.2/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)     2772 2023-03-21 02:32:42.586088 cognitive-service-vision-model-customization-python-samples-0.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2027 2023-03-21 02:32:25.000000 cognitive-service-vision-model-customization-python-samples-0.0.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 02:32:42.582088 cognitive-service-vision-model-customization-python-samples-0.0.2/cognitive_service_vision_model_customization_python_samples/
--rw-r--r--   0 runner    (1001) docker     (123)      798 2023-03-21 02:32:25.000000 cognitive-service-vision-model-customization-python-samples-0.0.2/cognitive_service_vision_model_customization_python_samples/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 02:32:42.582088 cognitive-service-vision-model-customization-python-samples-0.0.2/cognitive_service_vision_model_customization_python_samples/clients/
--rw-r--r--   0 runner    (1001) docker     (123)      318 2023-03-21 02:32:25.000000 cognitive-service-vision-model-customization-python-samples-0.0.2/cognitive_service_vision_model_customization_python_samples/clients/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2400 2023-03-21 02:32:25.000000 cognitive-service-vision-model-customization-python-samples-0.0.2/cognitive_service_vision_model_customization_python_samples/clients/client.py
--rw-r--r--   0 runner    (1001) docker     (123)      356 2023-03-21 02:32:25.000000 cognitive-service-vision-model-customization-python-samples-0.0.2/cognitive_service_vision_model_customization_python_samples/clients/common.py
--rw-r--r--   0 runner    (1001) docker     (123)      884 2023-03-21 02:32:25.000000 cognitive-service-vision-model-customization-python-samples-0.0.2/cognitive_service_vision_model_customization_python_samples/clients/dataset_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     1901 2023-03-21 02:32:25.000000 cognitive-service-vision-model-customization-python-samples-0.0.2/cognitive_service_vision_model_customization_python_samples/clients/evaluation_client.py
--rw-r--r--   0 runner    (1001) docker     (123)      270 2023-03-21 02:32:25.000000 cognitive-service-vision-model-customization-python-samples-0.0.2/cognitive_service_vision_model_customization_python_samples/clients/prediction_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     3541 2023-03-21 02:32:25.000000 cognitive-service-vision-model-customization-python-samples-0.0.2/cognitive_service_vision_model_customization_python_samples/clients/training_client.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 02:32:42.582088 cognitive-service-vision-model-customization-python-samples-0.0.2/cognitive_service_vision_model_customization_python_samples/data/
--rw-r--r--   0 runner    (1001) docker     (123)      197 2023-03-21 02:32:25.000000 cognitive-service-vision-model-customization-python-samples-0.0.2/cognitive_service_vision_model_customization_python_samples/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7586 2023-03-21 02:32:25.000000 cognitive-service-vision-model-customization-python-samples-0.0.2/cognitive_service_vision_model_customization_python_samples/data/check_coco_annotations.py
--rw-r--r--   0 runner    (1001) docker     (123)     8374 2023-03-21 02:32:25.000000 cognitive-service-vision-model-customization-python-samples-0.0.2/cognitive_service_vision_model_customization_python_samples/data/export_cvs_data_to_blob_storage.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 02:32:42.582088 cognitive-service-vision-model-customization-python-samples-0.0.2/cognitive_service_vision_model_customization_python_samples/models/
--rw-r--r--   0 runner    (1001) docker     (123)      580 2023-03-21 02:32:25.000000 cognitive-service-vision-model-customization-python-samples-0.0.2/cognitive_service_vision_model_customization_python_samples/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      346 2023-03-21 02:32:25.000000 cognitive-service-vision-model-customization-python-samples-0.0.2/cognitive_service_vision_model_customization_python_samples/models/common.py
--rw-r--r--   0 runner    (1001) docker     (123)     2974 2023-03-21 02:32:25.000000 cognitive-service-vision-model-customization-python-samples-0.0.2/cognitive_service_vision_model_customization_python_samples/models/dataset_models.py
--rw-r--r--   0 runner    (1001) docker     (123)     1789 2023-03-21 02:32:25.000000 cognitive-service-vision-model-customization-python-samples-0.0.2/cognitive_service_vision_model_customization_python_samples/models/evaluation_models.py
--rw-r--r--   0 runner    (1001) docker     (123)     3735 2023-03-21 02:32:25.000000 cognitive-service-vision-model-customization-python-samples-0.0.2/cognitive_service_vision_model_customization_python_samples/models/training_models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 02:32:42.582088 cognitive-service-vision-model-customization-python-samples-0.0.2/cognitive_service_vision_model_customization_python_samples.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2772 2023-03-21 02:32:42.000000 cognitive-service-vision-model-customization-python-samples-0.0.2/cognitive_service_vision_model_customization_python_samples.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1872 2023-03-21 02:32:42.000000 cognitive-service-vision-model-customization-python-samples-0.0.2/cognitive_service_vision_model_customization_python_samples.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-21 02:32:42.000000 cognitive-service-vision-model-customization-python-samples-0.0.2/cognitive_service_vision_model_customization_python_samples.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       82 2023-03-21 02:32:42.000000 cognitive-service-vision-model-customization-python-samples-0.0.2/cognitive_service_vision_model_customization_python_samples.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-03-21 02:32:42.000000 cognitive-service-vision-model-customization-python-samples-0.0.2/cognitive_service_vision_model_customization_python_samples.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-21 02:32:42.586088 cognitive-service-vision-model-customization-python-samples-0.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1602 2023-03-21 02:32:25.000000 cognitive-service-vision-model-customization-python-samples-0.0.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-21 02:32:42.586088 cognitive-service-vision-model-customization-python-samples-0.0.2/test/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-21 02:32:25.000000 cognitive-service-vision-model-customization-python-samples-0.0.2/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      744 2023-03-21 02:32:25.000000 cognitive-service-vision-model-customization-python-samples-0.0.2/test/test_clients.py
--rw-r--r--   0 runner    (1001) docker     (123)     1578 2023-03-21 02:32:25.000000 cognitive-service-vision-model-customization-python-samples-0.0.2/test/test_coco_check.py
--rw-r--r--   0 runner    (1001) docker     (123)     6503 2023-03-21 02:32:25.000000 cognitive-service-vision-model-customization-python-samples-0.0.2/test/test_e2e.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 16:18:35.331731 cognitive-service-vision-model-customization-python-samples-0.0.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1070 2023-05-05 16:18:22.000000 cognitive-service-vision-model-customization-python-samples-0.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1140 2023-05-05 16:18:22.000000 cognitive-service-vision-model-customization-python-samples-0.0.3/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2772 2023-05-05 16:18:35.331731 cognitive-service-vision-model-customization-python-samples-0.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2027 2023-05-05 16:18:22.000000 cognitive-service-vision-model-customization-python-samples-0.0.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 16:18:35.327731 cognitive-service-vision-model-customization-python-samples-0.0.3/cognitive_service_vision_model_customization_python_samples/
+-rw-r--r--   0 runner    (1001) docker     (123)      798 2023-05-05 16:18:22.000000 cognitive-service-vision-model-customization-python-samples-0.0.3/cognitive_service_vision_model_customization_python_samples/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 16:18:35.327731 cognitive-service-vision-model-customization-python-samples-0.0.3/cognitive_service_vision_model_customization_python_samples/clients/
+-rw-r--r--   0 runner    (1001) docker     (123)      318 2023-05-05 16:18:22.000000 cognitive-service-vision-model-customization-python-samples-0.0.3/cognitive_service_vision_model_customization_python_samples/clients/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2400 2023-05-05 16:18:22.000000 cognitive-service-vision-model-customization-python-samples-0.0.3/cognitive_service_vision_model_customization_python_samples/clients/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      356 2023-05-05 16:18:22.000000 cognitive-service-vision-model-customization-python-samples-0.0.3/cognitive_service_vision_model_customization_python_samples/clients/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)      884 2023-05-05 16:18:22.000000 cognitive-service-vision-model-customization-python-samples-0.0.3/cognitive_service_vision_model_customization_python_samples/clients/dataset_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1899 2023-05-05 16:18:22.000000 cognitive-service-vision-model-customization-python-samples-0.0.3/cognitive_service_vision_model_customization_python_samples/clients/evaluation_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)      270 2023-05-05 16:18:22.000000 cognitive-service-vision-model-customization-python-samples-0.0.3/cognitive_service_vision_model_customization_python_samples/clients/prediction_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3541 2023-05-05 16:18:22.000000 cognitive-service-vision-model-customization-python-samples-0.0.3/cognitive_service_vision_model_customization_python_samples/clients/training_client.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 16:18:35.327731 cognitive-service-vision-model-customization-python-samples-0.0.3/cognitive_service_vision_model_customization_python_samples/data/
+-rw-r--r--   0 runner    (1001) docker     (123)      197 2023-05-05 16:18:22.000000 cognitive-service-vision-model-customization-python-samples-0.0.3/cognitive_service_vision_model_customization_python_samples/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7586 2023-05-05 16:18:22.000000 cognitive-service-vision-model-customization-python-samples-0.0.3/cognitive_service_vision_model_customization_python_samples/data/check_coco_annotations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8374 2023-05-05 16:18:22.000000 cognitive-service-vision-model-customization-python-samples-0.0.3/cognitive_service_vision_model_customization_python_samples/data/export_cvs_data_to_blob_storage.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 16:18:35.331731 cognitive-service-vision-model-customization-python-samples-0.0.3/cognitive_service_vision_model_customization_python_samples/models/
+-rw-r--r--   0 runner    (1001) docker     (123)      580 2023-05-05 16:18:22.000000 cognitive-service-vision-model-customization-python-samples-0.0.3/cognitive_service_vision_model_customization_python_samples/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      346 2023-05-05 16:18:22.000000 cognitive-service-vision-model-customization-python-samples-0.0.3/cognitive_service_vision_model_customization_python_samples/models/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2974 2023-05-05 16:18:22.000000 cognitive-service-vision-model-customization-python-samples-0.0.3/cognitive_service_vision_model_customization_python_samples/models/dataset_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1789 2023-05-05 16:18:22.000000 cognitive-service-vision-model-customization-python-samples-0.0.3/cognitive_service_vision_model_customization_python_samples/models/evaluation_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3735 2023-05-05 16:18:22.000000 cognitive-service-vision-model-customization-python-samples-0.0.3/cognitive_service_vision_model_customization_python_samples/models/training_models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 16:18:35.327731 cognitive-service-vision-model-customization-python-samples-0.0.3/cognitive_service_vision_model_customization_python_samples.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2772 2023-05-05 16:18:35.000000 cognitive-service-vision-model-customization-python-samples-0.0.3/cognitive_service_vision_model_customization_python_samples.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1872 2023-05-05 16:18:35.000000 cognitive-service-vision-model-customization-python-samples-0.0.3/cognitive_service_vision_model_customization_python_samples.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 16:18:35.000000 cognitive-service-vision-model-customization-python-samples-0.0.3/cognitive_service_vision_model_customization_python_samples.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-05-05 16:18:35.000000 cognitive-service-vision-model-customization-python-samples-0.0.3/cognitive_service_vision_model_customization_python_samples.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-05-05 16:18:35.000000 cognitive-service-vision-model-customization-python-samples-0.0.3/cognitive_service_vision_model_customization_python_samples.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-05 16:18:35.331731 cognitive-service-vision-model-customization-python-samples-0.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1602 2023-05-05 16:18:22.000000 cognitive-service-vision-model-customization-python-samples-0.0.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 16:18:35.331731 cognitive-service-vision-model-customization-python-samples-0.0.3/test/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 16:18:22.000000 cognitive-service-vision-model-customization-python-samples-0.0.3/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      744 2023-05-05 16:18:22.000000 cognitive-service-vision-model-customization-python-samples-0.0.3/test/test_clients.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1578 2023-05-05 16:18:22.000000 cognitive-service-vision-model-customization-python-samples-0.0.3/test/test_coco_check.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6503 2023-05-05 16:18:22.000000 cognitive-service-vision-model-customization-python-samples-0.0.3/test/test_e2e.py
```

### Comparing `cognitive-service-vision-model-customization-python-samples-0.0.2/LICENSE` & `cognitive-service-vision-model-customization-python-samples-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `cognitive-service-vision-model-customization-python-samples-0.0.2/LICENSE.md` & `cognitive-service-vision-model-customization-python-samples-0.0.3/LICENSE.md`

 * *Files identical despite different names*

### Comparing `cognitive-service-vision-model-customization-python-samples-0.0.2/PKG-INFO` & `cognitive-service-vision-model-customization-python-samples-0.0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cognitive-service-vision-model-customization-python-samples
-Version: 0.0.2
+Version: 0.0.3
 Summary: A sample code repo for model customization using Python for Cognitive Service for Vision.
 Home-page: 
 Author: Ping Jin
 License: MIT
 Keywords: vision datasets classification detection
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `cognitive-service-vision-model-customization-python-samples-0.0.2/README.md` & `cognitive-service-vision-model-customization-python-samples-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `cognitive-service-vision-model-customization-python-samples-0.0.2/cognitive_service_vision_model_customization_python_samples/__init__.py` & `cognitive-service-vision-model-customization-python-samples-0.0.3/cognitive_service_vision_model_customization_python_samples/__init__.py`

 * *Files identical despite different names*

### Comparing `cognitive-service-vision-model-customization-python-samples-0.0.2/cognitive_service_vision_model_customization_python_samples/clients/client.py` & `cognitive-service-vision-model-customization-python-samples-0.0.3/cognitive_service_vision_model_customization_python_samples/clients/client.py`

 * *Files identical despite different names*

### Comparing `cognitive-service-vision-model-customization-python-samples-0.0.2/cognitive_service_vision_model_customization_python_samples/clients/dataset_client.py` & `cognitive-service-vision-model-customization-python-samples-0.0.3/cognitive_service_vision_model_customization_python_samples/clients/dataset_client.py`

 * *Files identical despite different names*

### Comparing `cognitive-service-vision-model-customization-python-samples-0.0.2/cognitive_service_vision_model_customization_python_samples/clients/evaluation_client.py` & `cognitive-service-vision-model-customization-python-samples-0.0.3/cognitive_service_vision_model_customization_python_samples/clients/evaluation_client.py`

 * *Files 7% similar despite different names*

```diff
@@ -19,15 +19,15 @@
     def query_run(self, name, model_name) -> EvaluationResponse:
         json_response = self.request_get(f'/models/{model_name}/evaluations/{name}')
         return EvaluationResponse.from_response(json_response)
 
     def wait_for_completion(self, name: str, model_name: str, check_wait_in_secs: int = 60) -> EvaluationResponse:
         start_time = time.time()
         while True:
-            eval_run = self.query_model(name, model_name)
+            eval_run = self.query_run(name, model_name)
             status = eval_run.status
             if status in [EvaluationStatus.FAILED, EvaluationStatus.SUCCEEDED]:
                 break
             time.sleep(check_wait_in_secs)
             total_elapsed = time.time() - start_time
             logging.info(f'Training {name} for {total_elapsed} seconds. Status {status}.')
```

### Comparing `cognitive-service-vision-model-customization-python-samples-0.0.2/cognitive_service_vision_model_customization_python_samples/clients/training_client.py` & `cognitive-service-vision-model-customization-python-samples-0.0.3/cognitive_service_vision_model_customization_python_samples/clients/training_client.py`

 * *Files identical despite different names*

### Comparing `cognitive-service-vision-model-customization-python-samples-0.0.2/cognitive_service_vision_model_customization_python_samples/data/check_coco_annotations.py` & `cognitive-service-vision-model-customization-python-samples-0.0.3/cognitive_service_vision_model_customization_python_samples/data/check_coco_annotations.py`

 * *Files identical despite different names*

### Comparing `cognitive-service-vision-model-customization-python-samples-0.0.2/cognitive_service_vision_model_customization_python_samples/data/export_cvs_data_to_blob_storage.py` & `cognitive-service-vision-model-customization-python-samples-0.0.3/cognitive_service_vision_model_customization_python_samples/data/export_cvs_data_to_blob_storage.py`

 * *Files identical despite different names*

### Comparing `cognitive-service-vision-model-customization-python-samples-0.0.2/cognitive_service_vision_model_customization_python_samples/models/__init__.py` & `cognitive-service-vision-model-customization-python-samples-0.0.3/cognitive_service_vision_model_customization_python_samples/models/__init__.py`

 * *Files identical despite different names*

### Comparing `cognitive-service-vision-model-customization-python-samples-0.0.2/cognitive_service_vision_model_customization_python_samples/models/dataset_models.py` & `cognitive-service-vision-model-customization-python-samples-0.0.3/cognitive_service_vision_model_customization_python_samples/models/dataset_models.py`

 * *Files identical despite different names*

### Comparing `cognitive-service-vision-model-customization-python-samples-0.0.2/cognitive_service_vision_model_customization_python_samples/models/evaluation_models.py` & `cognitive-service-vision-model-customization-python-samples-0.0.3/cognitive_service_vision_model_customization_python_samples/models/evaluation_models.py`

 * *Files identical despite different names*

### Comparing `cognitive-service-vision-model-customization-python-samples-0.0.2/cognitive_service_vision_model_customization_python_samples/models/training_models.py` & `cognitive-service-vision-model-customization-python-samples-0.0.3/cognitive_service_vision_model_customization_python_samples/models/training_models.py`

 * *Files identical despite different names*

### Comparing `cognitive-service-vision-model-customization-python-samples-0.0.2/cognitive_service_vision_model_customization_python_samples.egg-info/PKG-INFO` & `cognitive-service-vision-model-customization-python-samples-0.0.3/cognitive_service_vision_model_customization_python_samples.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cognitive-service-vision-model-customization-python-samples
-Version: 0.0.2
+Version: 0.0.3
 Summary: A sample code repo for model customization using Python for Cognitive Service for Vision.
 Home-page: 
 Author: Ping Jin
 License: MIT
 Keywords: vision datasets classification detection
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
```

### Comparing `cognitive-service-vision-model-customization-python-samples-0.0.2/cognitive_service_vision_model_customization_python_samples.egg-info/SOURCES.txt` & `cognitive-service-vision-model-customization-python-samples-0.0.3/cognitive_service_vision_model_customization_python_samples.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cognitive-service-vision-model-customization-python-samples-0.0.2/setup.py` & `cognitive-service-vision-model-customization-python-samples-0.0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import setuptools
 from os import path
 
-VERSION = '0.0.2'
+VERSION = '0.0.3'
 
 here = path.abspath(path.dirname(__file__))
 
 # Get the long description from the README file
 with open(path.join(here, 'README.md'), 'r') as f:
     long_description = f.read()
```

### Comparing `cognitive-service-vision-model-customization-python-samples-0.0.2/test/test_clients.py` & `cognitive-service-vision-model-customization-python-samples-0.0.3/test/test_clients.py`

 * *Files identical despite different names*

### Comparing `cognitive-service-vision-model-customization-python-samples-0.0.2/test/test_coco_check.py` & `cognitive-service-vision-model-customization-python-samples-0.0.3/test/test_coco_check.py`

 * *Files identical despite different names*

### Comparing `cognitive-service-vision-model-customization-python-samples-0.0.2/test/test_e2e.py` & `cognitive-service-vision-model-customization-python-samples-0.0.3/test/test_e2e.py`

 * *Files identical despite different names*

