# Comparing `tmp/responsibleai_vision-0.1.0.tar.gz` & `tmp/responsibleai_vision-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "responsibleai_vision-0.1.0.tar", last modified: Mon May  1 14:36:56 2023, max compression
+gzip compressed data, was "responsibleai_vision-0.2.0.tar", last modified: Fri May  5 17:33:40 2023, max compression
```

## Comparing `responsibleai_vision-0.1.0.tar` & `responsibleai_vision-0.2.0.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxrwxrwx   0        0        0        0 2023-05-01 14:36:56.280883 responsibleai_vision-0.1.0/
--rw-rw-rw-   0        0        0     1403 2023-05-01 14:36:56.280883 responsibleai_vision-0.1.0/PKG-INFO
--rw-rw-rw-   0        0        0      691 2022-05-04 15:27:52.000000 responsibleai_vision-0.1.0/README.md
-drwxrwxrwx   0        0        0        0 2023-05-01 14:36:55.895663 responsibleai_vision-0.1.0/responsibleai_vision/
--rw-rw-rw-   0        0        0      367 2022-05-04 15:27:52.000000 responsibleai_vision-0.1.0/responsibleai_vision/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-01 14:36:56.023269 responsibleai_vision-0.1.0/responsibleai_vision/common/
--rw-rw-rw-   0        0        0      127 2022-05-04 15:27:52.000000 responsibleai_vision-0.1.0/responsibleai_vision/common/__init__.py
--rw-rw-rw-   0        0        0     2518 2023-04-18 20:29:06.000000 responsibleai_vision-0.1.0/responsibleai_vision/common/constants.py
--rw-rw-rw-   0        0        0      223 2022-09-01 02:31:14.000000 responsibleai_vision-0.1.0/responsibleai_vision/common/interfaces.py
-drwxrwxrwx   0        0        0        0 2023-05-01 14:36:56.097781 responsibleai_vision-0.1.0/responsibleai_vision/managers/
--rw-rw-rw-   0        0        0      109 2022-05-04 15:27:52.000000 responsibleai_vision-0.1.0/responsibleai_vision/managers/__init__.py
--rw-rw-rw-   0        0        0    13708 2023-04-26 20:03:15.000000 responsibleai_vision-0.1.0/responsibleai_vision/managers/error_analysis_manager.py
--rw-rw-rw-   0        0        0    24559 2023-04-28 19:33:16.000000 responsibleai_vision-0.1.0/responsibleai_vision/managers/explainer_manager.py
-drwxrwxrwx   0        0        0        0 2023-05-01 14:36:56.157766 responsibleai_vision-0.1.0/responsibleai_vision/rai_vision_insights/
--rw-rw-rw-   0        0        0      253 2022-05-04 15:27:52.000000 responsibleai_vision-0.1.0/responsibleai_vision/rai_vision_insights/__init__.py
--rw-rw-rw-   0        0        0    46888 2023-04-26 20:03:15.000000 responsibleai_vision-0.1.0/responsibleai_vision/rai_vision_insights/rai_vision_insights.py
-drwxrwxrwx   0        0        0        0 2023-05-01 14:36:56.230951 responsibleai_vision-0.1.0/responsibleai_vision/utils/
--rw-rw-rw-   0        0        0      129 2022-05-04 15:27:52.000000 responsibleai_vision-0.1.0/responsibleai_vision/utils/__init__.py
--rw-rw-rw-   0        0        0     2126 2023-04-13 17:35:46.000000 responsibleai_vision-0.1.0/responsibleai_vision/utils/feature_extractors.py
--rw-rw-rw-   0        0        0     2824 2023-04-18 20:29:06.000000 responsibleai_vision-0.1.0/responsibleai_vision/utils/image_reader.py
--rw-rw-rw-   0        0        0     2568 2023-04-13 17:35:46.000000 responsibleai_vision-0.1.0/responsibleai_vision/utils/image_utils.py
--rw-rw-rw-   0        0        0      194 2023-05-01 14:36:36.000000 responsibleai_vision-0.1.0/responsibleai_vision/version.py
-drwxrwxrwx   0        0        0        0 2023-05-01 14:36:55.957461 responsibleai_vision-0.1.0/responsibleai_vision.egg-info/
--rw-rw-rw-   0        0        0     1403 2023-05-01 14:36:55.000000 responsibleai_vision-0.1.0/responsibleai_vision.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1004 2023-05-01 14:36:55.000000 responsibleai_vision-0.1.0/responsibleai_vision.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-01 14:36:55.000000 responsibleai_vision-0.1.0/responsibleai_vision.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      147 2023-05-01 14:36:55.000000 responsibleai_vision-0.1.0/responsibleai_vision.egg-info/requires.txt
--rw-rw-rw-   0        0        0       21 2023-05-01 14:36:55.000000 responsibleai_vision-0.1.0/responsibleai_vision.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-01 14:36:56.280883 responsibleai_vision-0.1.0/setup.cfg
--rw-rw-rw-   0        0        0     1417 2022-05-04 15:27:52.000000 responsibleai_vision-0.1.0/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-01 14:36:56.270563 responsibleai_vision-0.1.0/tests/
--rw-rw-rw-   0        0        0     4575 2023-04-17 19:05:16.000000 responsibleai_vision-0.1.0/tests/test_rai_vision_automl_images_insights.py
--rw-rw-rw-   0        0        0     7899 2023-04-17 19:05:16.000000 responsibleai_vision-0.1.0/tests/test_rai_vision_insights.py
--rw-rw-rw-   0        0        0     3082 2023-04-17 19:05:16.000000 responsibleai_vision-0.1.0/tests/test_rai_vision_insights_save_and_load_scenarios.py
+drwxrwxrwx   0        0        0        0 2023-05-05 17:33:40.199850 responsibleai_vision-0.2.0/
+-rw-rw-rw-   0        0        0     1403 2023-05-05 17:33:40.199850 responsibleai_vision-0.2.0/PKG-INFO
+-rw-rw-rw-   0        0        0      691 2022-05-04 15:27:52.000000 responsibleai_vision-0.2.0/README.md
+drwxrwxrwx   0        0        0        0 2023-05-05 17:33:39.862868 responsibleai_vision-0.2.0/responsibleai_vision/
+-rw-rw-rw-   0        0        0      367 2022-05-04 15:27:52.000000 responsibleai_vision-0.2.0/responsibleai_vision/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-05 17:33:39.966630 responsibleai_vision-0.2.0/responsibleai_vision/common/
+-rw-rw-rw-   0        0        0      127 2022-05-04 15:27:52.000000 responsibleai_vision-0.2.0/responsibleai_vision/common/__init__.py
+-rw-rw-rw-   0        0        0     2518 2023-04-18 20:29:06.000000 responsibleai_vision-0.2.0/responsibleai_vision/common/constants.py
+-rw-rw-rw-   0        0        0      223 2022-09-01 02:31:14.000000 responsibleai_vision-0.2.0/responsibleai_vision/common/interfaces.py
+drwxrwxrwx   0        0        0        0 2023-05-05 17:33:40.016699 responsibleai_vision-0.2.0/responsibleai_vision/managers/
+-rw-rw-rw-   0        0        0      109 2022-05-04 15:27:52.000000 responsibleai_vision-0.2.0/responsibleai_vision/managers/__init__.py
+-rw-rw-rw-   0        0        0    13897 2023-05-05 17:29:08.000000 responsibleai_vision-0.2.0/responsibleai_vision/managers/error_analysis_manager.py
+-rw-rw-rw-   0        0        0    26315 2023-05-04 17:50:06.000000 responsibleai_vision-0.2.0/responsibleai_vision/managers/explainer_manager.py
+drwxrwxrwx   0        0        0        0 2023-05-05 17:33:40.055076 responsibleai_vision-0.2.0/responsibleai_vision/rai_vision_insights/
+-rw-rw-rw-   0        0        0      253 2022-05-04 15:27:52.000000 responsibleai_vision-0.2.0/responsibleai_vision/rai_vision_insights/__init__.py
+-rw-rw-rw-   0        0        0    46976 2023-05-05 17:29:08.000000 responsibleai_vision-0.2.0/responsibleai_vision/rai_vision_insights/rai_vision_insights.py
+drwxrwxrwx   0        0        0        0 2023-05-05 17:33:40.131971 responsibleai_vision-0.2.0/responsibleai_vision/utils/
+-rw-rw-rw-   0        0        0      129 2022-05-04 15:27:52.000000 responsibleai_vision-0.2.0/responsibleai_vision/utils/__init__.py
+-rw-rw-rw-   0        0        0     2329 2023-05-05 17:29:08.000000 responsibleai_vision-0.2.0/responsibleai_vision/utils/feature_extractors.py
+-rw-rw-rw-   0        0        0     2824 2023-04-18 20:29:06.000000 responsibleai_vision-0.2.0/responsibleai_vision/utils/image_reader.py
+-rw-rw-rw-   0        0        0     2568 2023-04-13 17:35:46.000000 responsibleai_vision-0.2.0/responsibleai_vision/utils/image_utils.py
+-rw-rw-rw-   0        0        0      194 2023-05-05 17:31:42.000000 responsibleai_vision-0.2.0/responsibleai_vision/version.py
+drwxrwxrwx   0        0        0        0 2023-05-05 17:33:39.927458 responsibleai_vision-0.2.0/responsibleai_vision.egg-info/
+-rw-rw-rw-   0        0        0     1403 2023-05-05 17:33:39.000000 responsibleai_vision-0.2.0/responsibleai_vision.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1004 2023-05-05 17:33:39.000000 responsibleai_vision-0.2.0/responsibleai_vision.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-05 17:33:39.000000 responsibleai_vision-0.2.0/responsibleai_vision.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      147 2023-05-05 17:33:39.000000 responsibleai_vision-0.2.0/responsibleai_vision.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       21 2023-05-05 17:33:39.000000 responsibleai_vision-0.2.0/responsibleai_vision.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-05 17:33:40.199850 responsibleai_vision-0.2.0/setup.cfg
+-rw-rw-rw-   0        0        0     1417 2022-05-04 15:27:52.000000 responsibleai_vision-0.2.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-05 17:33:40.199850 responsibleai_vision-0.2.0/tests/
+-rw-rw-rw-   0        0        0     4575 2023-04-17 19:05:16.000000 responsibleai_vision-0.2.0/tests/test_rai_vision_automl_images_insights.py
+-rw-rw-rw-   0        0        0     7899 2023-04-17 19:05:16.000000 responsibleai_vision-0.2.0/tests/test_rai_vision_insights.py
+-rw-rw-rw-   0        0        0     3082 2023-04-17 19:05:16.000000 responsibleai_vision-0.2.0/tests/test_rai_vision_insights_save_and_load_scenarios.py
```

### Comparing `responsibleai_vision-0.1.0/PKG-INFO` & `responsibleai_vision-0.2.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: responsibleai_vision
-Version: 0.1.0
+Version: 0.2.0
 Summary: SDK API to assess image Machine Learning models.
 Home-page: https://github.com/microsoft/responsible-ai-toolbox
 Author: Roman Lutz, Ilya Matiach, Ke Xu
 Author-email: raiwidgets-maintain@microsoft.com
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `responsibleai_vision-0.1.0/README.md` & `responsibleai_vision-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `responsibleai_vision-0.1.0/responsibleai_vision/common/constants.py` & `responsibleai_vision-0.2.0/responsibleai_vision/common/constants.py`

 * *Files identical despite different names*

### Comparing `responsibleai_vision-0.1.0/responsibleai_vision/managers/error_analysis_manager.py` & `responsibleai_vision-0.2.0/responsibleai_vision/managers/error_analysis_manager.py`

 * *Files 1% similar despite different names*

```diff
@@ -280,17 +280,20 @@
         inst.__dict__['_ea_config_list'] = ea_config_list
 
         feature_metadata = rai_insights._feature_metadata
         categorical_features = feature_metadata.categorical_features
         inst.__dict__['_categorical_features'] = categorical_features
         target_column = rai_insights.target_column
         true_y = rai_insights._ext_test_df[target_column]
-        dataset = rai_insights._ext_test_df.drop(columns=[target_column])
+        if isinstance(target_column, list):
+            dropped_cols = target_column
+        else:
+            dropped_cols = [target_column]
+        dataset = rai_insights._ext_test_df.drop(columns=dropped_cols)
         inst.__dict__['_dataset'] = dataset
-        inst.__dict__['_true_y'] = true_y
         feature_names = list(dataset.columns)
         inst.__dict__['_feature_names'] = feature_names
         task_type = rai_insights.task_type
         wrapped_model = wrap_model(rai_insights.model, dataset,
                                    rai_insights.task_type,
                                    classes=rai_insights._classes)
         inst.__dict__['_task_type'] = task_type
@@ -299,17 +302,19 @@
         index_dataset = rai_insights.test
         if isinstance(target_column, list) and not is_od:
             # create copy of dataset as we will make modifications to it
             index_dataset = index_dataset.copy()
             index_classes = target_column
             labels = _concat_labels_column(index_dataset, target_column,
                                            index_classes)
-            index_dataset[LABELS] = labels
             index_dataset.drop(columns=target_column, inplace=True)
+            index_dataset[LABELS] = labels
             target_column = LABELS
+            true_y = index_dataset[target_column]
+        inst.__dict__['_true_y'] = true_y
         index_predictor = ErrorAnalysisManager._create_index_predictor(
             wrapped_model, index_dataset, target_column,
             task_type, rai_insights.image_mode,
             rai_insights._transformations,
             rai_insights._classes)
         inst.__dict__['_analyzer'] = ModelAnalyzer(index_predictor,
                                                    dataset,
```

### Comparing `responsibleai_vision-0.1.0/responsibleai_vision/managers/explainer_manager.py` & `responsibleai_vision-0.2.0/responsibleai_vision/managers/explainer_manager.py`

 * *Files 3% similar despite different names*

```diff
@@ -120,25 +120,63 @@
 
     def compute(self, **kwargs):
         """Creates an explanation by running the explainer on the model."""
         if not self._is_added:
             return
         if self._is_run:
             return
-        if self._is_classification_task or self._is_object_detection_task:
-            self._explanation = []
+        self._explanation = []
+        if self._is_classification_task:
             for i in range(len(self._evaluation_examples)):
                 self._explanation.append(
                     self.compute_single_explanation(i, max_evals=100, **kwargs)
                 )
+        elif self._is_object_detection_task:
+            for i in range(len(self._evaluation_examples)):
+                self._explanation.append(
+                    self.compute_batch_explanation(i)
+                )
         else:
             raise ValueError('Unknown task type: {}'.format(self._task_type))
 
         self._is_run = True
 
+    def compute_batch_explanation(self,
+                                  index):
+        """
+        This function is a subroutine of the compute method.
+        It computes explanations using batching to optimize performance.
+
+        Currently only supported for object detection, in which all
+        explanations per image are computed in parallel (each image
+        may have multiple detections).
+
+        :param index: The index of the image to create the explanation for
+        :type index: int
+
+        :return: The computed explanations on the image level
+        :rtype: list of strings
+        """
+        if self._is_object_detection_task:
+            ex = self._evaluation_examples
+            img = ex.iloc[index:index+1, 0].values[0]
+            try:
+                # calling DRISE to generate saliency maps for all objects
+                fl, _, _, = get_drise_saliency_map(img,
+                                                   self._model,
+                                                   len(self._classes),
+                                                   savename=str(index),
+                                                   nummasks=50,
+                                                   max_figures=5000)
+            except BaseException:
+                fl = [self._get_fail_str()]
+            return fl
+        else:
+            raise ValueError('Unknown task type: {}'.format(self._task_type))
+
     def compute_single_explanation(self,
                                    index,
                                    max_evals=100,
                                    object_index=0,
                                    **kwargs):
         """Creates an explanation for a single image in the dataset
 
@@ -165,15 +203,18 @@
             xai_algo_name = ExplainabilityLiterals.SHAP
 
         if not self._is_added:
             self.add()
         if index < 0 or index > len(self._evaluation_examples) - 1:
             raise ValueError('Index out of range')
         if self._explanation is not None and index < len(self._explanation):
-            return self._explanation[index]
+            if self._task_type == ModelTask.OBJECT_DETECTION:
+                return self._explanation[index][object_index]
+            else:
+                return self._explanation[index]
         if self._is_classification_task:
             ex = self._evaluation_examples
             image = ex.iloc[index:index+1, 0].values[0]
             if isinstance(image, str):
                 if not self.automl_image_model:
                     image = get_image_from_path(image, self._image_mode)
             if xai_algo_name == ExplainabilityLiterals.SHAP:
@@ -198,45 +239,33 @@
                             xai_algo_name, type(self._model)
                         )
                     )
         if self._is_object_detection_task:
             ex = self._evaluation_examples
             img = ex.iloc[index:index+1, 0].values[0]
             try:
-                # if saliency map was already computed, do not rerun DRISE
-                image = get_image_from_path(
-                    str(index)+str(object_index)+".jpg",
-                    self._image_mode)
+                if (type(self._model) is not MLflowDRiseWrapper and
+                   type(self._model) is not PytorchDRiseWrapper):
+                    if is_automl_image_model(self._model):
+                        self._model = MLflowDRiseWrapper(self._model._model,
+                                                         self._classes)
+                    else:
+                        self._model = PytorchDRiseWrapper(self._model._model,
+                                                          len(self._classes))
+
+                # calling DRISE to generate saliency maps for all objects
+                fl, _, _, = get_drise_saliency_map(img,
+                                                   self._model,
+                                                   len(self._classes),
+                                                   savename=str(index),
+                                                   nummasks=50,
+                                                   max_figures=5000)
+                b64_string = fl[object_index]
             except BaseException:
-                try:
-                    # calling DRISE to generate saliency maps for all objects
-                    get_drise_saliency_map(img,
-                                           self._model,
-                                           len(self._classes),
-                                           savename=str(index),
-                                           nummasks=50,
-                                           max_figures=5000)
-                    # retrieving saliency map for selected object
-                    image = get_image_from_path(str(index)+str(object_index)
-                                                + ".jpg",
-                                                self._image_mode)
-                except BaseException:
-                    fail = Image.new('RGB', (100, 100))
-                    draw = ImageDraw.Draw(fail)
-                    font = ImageFont.load_default()
-                    text = "saliency map could not be created"
-                    textwidth, textheight = draw.textsize(text, font)
-                    x = (fail.width - textwidth) // 2
-                    y = (fail.height - textheight) // 2
-                    draw.text((x, y), text, fill="white", font=font)
-                    fail.show()
-                    fail.save('fail.jpg')
-                    image = get_image_from_path("fail.jpg", self._image_mode)
-            jpg_img = cv2.imencode('.jpg', image)
-            b64_string = base64.b64encode(jpg_img[1]).decode('utf-8')
+                b64_string = self._get_fail_str()
             return b64_string
         else:
             raise ValueError('Unknown task type: {}'.format(self._task_type))
 
     def get_shap_explanations(self, image, max_evals):
         """Generates an explanation using shap method.
 
@@ -524,14 +553,29 @@
         """Check if the task is an object detection task.
 
         :return: True if the task is an object detection task.
         :rtype: bool
         """
         return self._task_type == ModelTask.OBJECT_DETECTION
 
+    def _get_fail_str(self):
+        fail = Image.new('RGB', (100, 100))
+        draw = ImageDraw.Draw(fail)
+        font = ImageFont.load_default()
+        text = "saliency map could not be created"
+        textwidth, textheight = draw.textsize(text, font)
+        x = (fail.width - textwidth) // 2
+        y = (fail.height - textheight) // 2
+        draw.text((x, y), text, fill="white", font=font)
+        fail.show()
+        fail.save('fail.jpg')
+        image = get_image_from_path("fail.jpg", "RGB")
+        jpg_img = cv2.imencode('.jpg', image)
+        return base64.b64encode(jpg_img[1]).decode('utf-8')
+
     def _save(self, path):
         """Save the ExplainerManager to the given path.
 
         :param path: The directory path to save the ExplainerManager to.
         :type path: str
         """
         top_dir = Path(path)
```

### Comparing `responsibleai_vision-0.1.0/responsibleai_vision/rai_vision_insights/rai_vision_insights.py` & `responsibleai_vision-0.2.0/responsibleai_vision/rai_vision_insights/rai_vision_insights.py`

 * *Files 1% similar despite different names*

```diff
@@ -110,16 +110,17 @@
 
         :param model: The model to compute RAI insights for.
             A model that implements sklearn.predict or sklearn.predict_proba
             or function that accepts a 2d ndarray.
         :type model: object
         :param test: The test dataframe including the label column.
         :type test: pd.DataFrame
-        :param target_column: The name of the label column.
-        :type target_column: str
+        :param target_column: The name of the label column or list of columns.
+            This is a list of columns for multilabel models.
+        :type target_column:  str or list[str]
         :param task_type: The task to run.
         :type task_type: str
         :param classes: The class labels in the dataset.
         :type classes: numpy.ndarray
         :param serializer: Picklable custom serializer with save and load
             methods for custom model serialization.
             The save method writes the model to file given a parent directory.
@@ -364,15 +365,15 @@
         # Pick one row from dataset
         if not isinstance(target_column, list):
             target_column = [target_column]
         img = dataset.drop(
             target_column, axis=1).iloc[0][0]
         if isinstance(img, str):
             if self.automl_image_model:
-                if self._task_type == ModelTask.OBJECT_DETECTION.value:
+                if self._task_type == ModelTask.OBJECT_DETECTION:
                     img_data, img_size = get_base64_string_from_path(
                         img, return_image_size=True)
                     img = pd.DataFrame(
                         data=[[img_data, img_size]],
                         columns=[
                             MLFlowSchemaLiterals.INPUT_COLUMN_IMAGE,
                             MLFlowSchemaLiterals.INPUT_IMAGE_SIZE],
```

### Comparing `responsibleai_vision-0.1.0/responsibleai_vision/utils/feature_extractors.py` & `responsibleai_vision-0.2.0/responsibleai_vision/utils/feature_extractors.py`

 * *Files 8% similar despite different names*

```diff
@@ -13,40 +13,43 @@
                      target_column: str, task_type: str,
                      image_mode: str = None,
                      dropped_features: Optional[List[str]] = None):
     '''Extract tabular data features from the image dataset.
 
     :param image_dataset: A pandas dataframe containing the image data.
     :type image_dataset: pandas.DataFrame
-    :param target_column: The name of the column containing
-        the target values.
-    :type target_column: str
+    :param target_column: The name of the label column or list of columns.
+        This is a list of columns for multilabel models.
+    :type target_column: str or list[str]
     :param task_type: The type of task to be performed.
     :type task_type: str
     :param image_mode: The mode to open the image in.
         See pillow documentation for all modes:
         https://pillow.readthedocs.io/en/stable/handbook/concepts.html
     :type image_mode: str
     :return: The list of extracted features and the feature names.
     :rtype: list, list
     '''
     results = []
     feature_names = ["mean_pixel_value"]
     column_names = image_dataset.columns
     has_dropped_features = dropped_features is not None
-    for j in range(2, image_dataset.shape[1]):
+    start_meta_index = 2
+    if isinstance(target_column, list):
+        start_meta_index = len(target_column) + 1
+    for j in range(start_meta_index, image_dataset.shape[1]):
         if has_dropped_features and column_names[j] in dropped_features:
             continue
         feature_names.append(column_names[j])
     for i in tqdm(range(image_dataset.shape[0])):
         image = image_dataset.iloc[i][0]
         if isinstance(image, str):
             image = get_image_from_path(image, image_mode)
         mean_pixel_value = image.mean()
         row_feature_values = [mean_pixel_value]
         # append all features other than target column and label
-        for j in range(2, image_dataset.shape[1]):
+        for j in range(start_meta_index, image_dataset.shape[1]):
             if has_dropped_features and column_names[j] in dropped_features:
                 continue
             row_feature_values.append(image_dataset.iloc[i][j])
         results.append(row_feature_values)
     return results, feature_names
```

### Comparing `responsibleai_vision-0.1.0/responsibleai_vision/utils/image_reader.py` & `responsibleai_vision-0.2.0/responsibleai_vision/utils/image_reader.py`

 * *Files identical despite different names*

### Comparing `responsibleai_vision-0.1.0/responsibleai_vision/utils/image_utils.py` & `responsibleai_vision-0.2.0/responsibleai_vision/utils/image_utils.py`

 * *Files identical despite different names*

### Comparing `responsibleai_vision-0.1.0/responsibleai_vision.egg-info/PKG-INFO` & `responsibleai_vision-0.2.0/responsibleai_vision.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: responsibleai-vision
-Version: 0.1.0
+Version: 0.2.0
 Summary: SDK API to assess image Machine Learning models.
 Home-page: https://github.com/microsoft/responsible-ai-toolbox
 Author: Roman Lutz, Ilya Matiach, Ke Xu
 Author-email: raiwidgets-maintain@microsoft.com
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `responsibleai_vision-0.1.0/responsibleai_vision.egg-info/SOURCES.txt` & `responsibleai_vision-0.2.0/responsibleai_vision.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `responsibleai_vision-0.1.0/setup.py` & `responsibleai_vision-0.2.0/setup.py`

 * *Files identical despite different names*

### Comparing `responsibleai_vision-0.1.0/tests/test_rai_vision_automl_images_insights.py` & `responsibleai_vision-0.2.0/tests/test_rai_vision_automl_images_insights.py`

 * *Files identical despite different names*

### Comparing `responsibleai_vision-0.1.0/tests/test_rai_vision_insights.py` & `responsibleai_vision-0.2.0/tests/test_rai_vision_insights.py`

 * *Files identical despite different names*

### Comparing `responsibleai_vision-0.1.0/tests/test_rai_vision_insights_save_and_load_scenarios.py` & `responsibleai_vision-0.2.0/tests/test_rai_vision_insights_save_and_load_scenarios.py`

 * *Files identical despite different names*

