# Comparing `tmp/mlcvzoo_yolox-6.0.0.tar.gz` & `tmp/mlcvzoo_yolox-6.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mlcvzoo_yolox-6.0.0.tar", max compression
+gzip compressed data, was "mlcvzoo_yolox-6.0.1.tar", max compression
```

## Comparing `mlcvzoo_yolox-6.0.0.tar` & `mlcvzoo_yolox-6.0.1.tar`

### file list

```diff
@@ -1,33 +1,33 @@
--rw-r--r--   0        0        0      409 2023-02-14 09:45:10.245350 mlcvzoo_yolox-6.0.0/README.md
--rw-r--r--   0        0        0      177 2023-02-14 16:02:42.669113 mlcvzoo_yolox-6.0.0/mlcvzoo_yolox/__init__.py
--rw-r--r--   0        0        0     6010 2023-02-14 16:02:42.669113 mlcvzoo_yolox-6.0.0/mlcvzoo_yolox/configuration.py
--rw-r--r--   0        0        0      154 2023-02-14 09:45:10.245350 mlcvzoo_yolox-6.0.0/mlcvzoo_yolox/core/__init__.py
--rw-r--r--   0        0        0     2248 2023-02-14 09:45:10.245350 mlcvzoo_yolox-6.0.0/mlcvzoo_yolox/core/trainer.py
--rw-r--r--   0        0        0      154 2023-02-14 09:45:10.245350 mlcvzoo_yolox-6.0.0/mlcvzoo_yolox/data/__init__.py
--rw-r--r--   0        0        0      154 2023-02-14 09:45:10.245350 mlcvzoo_yolox-6.0.0/mlcvzoo_yolox/data/datasets/__init__.py
--rw-r--r--   0        0        0     4905 2023-02-14 09:45:10.245350 mlcvzoo_yolox-6.0.0/mlcvzoo_yolox/data/datasets/dataset.py
--rw-r--r--   0        0        0      154 2023-02-14 09:45:10.245350 mlcvzoo_yolox-6.0.0/mlcvzoo_yolox/evaluators/__init__.py
--rw-r--r--   0        0        0     7298 2023-02-14 16:02:42.673113 mlcvzoo_yolox-6.0.0/mlcvzoo_yolox/evaluators/evaluator.py
--rw-r--r--   0        0        0      154 2023-02-14 09:45:10.245350 mlcvzoo_yolox-6.0.0/mlcvzoo_yolox/exp/__init__.py
--rw-r--r--   0        0        0     9642 2023-02-14 16:02:42.673113 mlcvzoo_yolox-6.0.0/mlcvzoo_yolox/exp/custom_yolox_exp.py
--rw-r--r--   0        0        0     1599 2023-02-14 09:45:10.249350 mlcvzoo_yolox-6.0.0/mlcvzoo_yolox/exp/default.py
--rw-r--r--   0        0        0    12944 2023-02-14 16:02:42.673113 mlcvzoo_yolox-6.0.0/mlcvzoo_yolox/model.py
--rw-r--r--   0        0        0     9371 2023-02-14 09:45:10.249350 mlcvzoo_yolox-6.0.0/mlcvzoo_yolox/model_utils.py
--rw-r--r--   0        0        0      154 2023-02-14 09:45:10.249350 mlcvzoo_yolox-6.0.0/mlcvzoo_yolox/py.typed
--rw-r--r--   0        0        0        0 2023-02-14 09:45:10.249350 mlcvzoo_yolox-6.0.0/mlcvzoo_yolox/third_party/__init__.py
--rw-r--r--   0        0        0    11352 2023-02-14 09:45:10.249350 mlcvzoo_yolox-6.0.0/mlcvzoo_yolox/third_party/yolox/LICENSE
--rw-r--r--   0        0        0      113 2023-02-14 09:45:10.249350 mlcvzoo_yolox-6.0.0/mlcvzoo_yolox/third_party/yolox/README.md
--rw-r--r--   0        0        0       49 2023-02-14 09:45:10.249350 mlcvzoo_yolox-6.0.0/mlcvzoo_yolox/third_party/yolox/__init__.py
--rw-r--r--   0        0        0       49 2023-02-14 09:45:10.249350 mlcvzoo_yolox-6.0.0/mlcvzoo_yolox/third_party/yolox/exps/__init__.py
--rw-r--r--   0        0        0     3338 2023-02-14 09:45:10.249350 mlcvzoo_yolox-6.0.0/mlcvzoo_yolox/third_party/yolox/exps/yolox_base.py
--rw-r--r--   0        0        0     1662 2023-02-14 09:45:10.249350 mlcvzoo_yolox-6.0.0/mlcvzoo_yolox/third_party/yolox/exps/yolox_nano.py
--rw-r--r--   0        0        0       49 2023-02-14 09:45:10.249350 mlcvzoo_yolox-6.0.0/mlcvzoo_yolox/third_party/yolox/models/__init__.py
--rw-r--r--   0        0        0     1154 2023-02-14 09:45:10.249350 mlcvzoo_yolox-6.0.0/mlcvzoo_yolox/third_party/yolox/models/yolo_head.py
--rw-r--r--   0        0        0       49 2023-02-14 09:45:10.249350 mlcvzoo_yolox-6.0.0/mlcvzoo_yolox/third_party/yolox/tools/__init__.py
--rw-r--r--   0        0        0     1528 2023-02-14 09:45:10.249350 mlcvzoo_yolox-6.0.0/mlcvzoo_yolox/third_party/yolox/tools/train.py
--rw-r--r--   0        0        0     2745 2023-02-14 09:45:10.249350 mlcvzoo_yolox-6.0.0/mlcvzoo_yolox/third_party/yolox/tools/trt.py
--rw-r--r--   0        0        0       49 2023-02-14 09:45:10.249350 mlcvzoo_yolox-6.0.0/mlcvzoo_yolox/third_party/yolox/utils/__init__.py
--rw-r--r--   0        0        0     2375 2023-02-14 09:45:10.249350 mlcvzoo_yolox-6.0.0/mlcvzoo_yolox/third_party/yolox/utils/boxes.py
--rw-r--r--   0        0        0     4627 2023-02-14 16:02:42.673113 mlcvzoo_yolox-6.0.0/pyproject.toml
--rw-r--r--   0        0        0     1904 1970-01-01 00:00:00.000000 mlcvzoo_yolox-6.0.0/setup.py
--rw-r--r--   0        0        0     2049 1970-01-01 00:00:00.000000 mlcvzoo_yolox-6.0.0/PKG-INFO
+-rw-r--r--   0        0        0      409 2023-05-02 10:18:08.305755 mlcvzoo_yolox-6.0.1/README.md
+-rw-r--r--   0        0        0      177 2023-05-05 09:21:26.582902 mlcvzoo_yolox-6.0.1/mlcvzoo_yolox/__init__.py
+-rw-r--r--   0        0        0     6009 2023-05-04 12:11:41.809631 mlcvzoo_yolox-6.0.1/mlcvzoo_yolox/configuration.py
+-rw-r--r--   0        0        0      154 2023-05-02 10:18:08.305755 mlcvzoo_yolox-6.0.1/mlcvzoo_yolox/core/__init__.py
+-rw-r--r--   0        0        0     2531 2023-05-03 12:33:28.187548 mlcvzoo_yolox-6.0.1/mlcvzoo_yolox/core/trainer.py
+-rw-r--r--   0        0        0      154 2023-05-02 10:18:08.305755 mlcvzoo_yolox-6.0.1/mlcvzoo_yolox/data/__init__.py
+-rw-r--r--   0        0        0      154 2023-05-02 10:18:08.305755 mlcvzoo_yolox-6.0.1/mlcvzoo_yolox/data/datasets/__init__.py
+-rw-r--r--   0        0        0     4904 2023-05-03 12:33:28.187548 mlcvzoo_yolox-6.0.1/mlcvzoo_yolox/data/datasets/dataset.py
+-rw-r--r--   0        0        0      154 2023-05-02 10:18:08.305755 mlcvzoo_yolox-6.0.1/mlcvzoo_yolox/evaluators/__init__.py
+-rw-r--r--   0        0        0     7282 2023-05-03 12:33:28.187548 mlcvzoo_yolox-6.0.1/mlcvzoo_yolox/evaluators/evaluator.py
+-rw-r--r--   0        0        0      154 2023-05-02 10:18:08.305755 mlcvzoo_yolox-6.0.1/mlcvzoo_yolox/exp/__init__.py
+-rw-r--r--   0        0        0     9641 2023-05-03 12:33:28.187548 mlcvzoo_yolox-6.0.1/mlcvzoo_yolox/exp/custom_yolox_exp.py
+-rw-r--r--   0        0        0     1598 2023-05-03 12:33:28.187548 mlcvzoo_yolox-6.0.1/mlcvzoo_yolox/exp/default.py
+-rw-r--r--   0        0        0    12944 2023-05-04 12:11:41.809631 mlcvzoo_yolox-6.0.1/mlcvzoo_yolox/model.py
+-rw-r--r--   0        0        0     9354 2023-05-04 12:11:41.809631 mlcvzoo_yolox-6.0.1/mlcvzoo_yolox/model_utils.py
+-rw-r--r--   0        0        0      154 2023-05-02 10:18:08.305755 mlcvzoo_yolox-6.0.1/mlcvzoo_yolox/py.typed
+-rw-r--r--   0        0        0        0 2023-05-02 10:18:08.309755 mlcvzoo_yolox-6.0.1/mlcvzoo_yolox/third_party/__init__.py
+-rw-r--r--   0        0        0    11352 2023-05-02 10:18:08.309755 mlcvzoo_yolox-6.0.1/mlcvzoo_yolox/third_party/yolox/LICENSE
+-rw-r--r--   0        0        0      113 2023-05-02 10:18:08.309755 mlcvzoo_yolox-6.0.1/mlcvzoo_yolox/third_party/yolox/README.md
+-rw-r--r--   0        0        0       49 2023-05-02 10:18:08.309755 mlcvzoo_yolox-6.0.1/mlcvzoo_yolox/third_party/yolox/__init__.py
+-rw-r--r--   0        0        0       49 2023-05-02 10:18:08.309755 mlcvzoo_yolox-6.0.1/mlcvzoo_yolox/third_party/yolox/exps/__init__.py
+-rw-r--r--   0        0        0     3338 2023-05-02 10:18:08.309755 mlcvzoo_yolox-6.0.1/mlcvzoo_yolox/third_party/yolox/exps/yolox_base.py
+-rw-r--r--   0        0        0     1662 2023-05-02 10:18:08.309755 mlcvzoo_yolox-6.0.1/mlcvzoo_yolox/third_party/yolox/exps/yolox_nano.py
+-rw-r--r--   0        0        0       49 2023-05-02 10:18:08.309755 mlcvzoo_yolox-6.0.1/mlcvzoo_yolox/third_party/yolox/models/__init__.py
+-rw-r--r--   0        0        0     1154 2023-05-02 10:18:08.309755 mlcvzoo_yolox-6.0.1/mlcvzoo_yolox/third_party/yolox/models/yolo_head.py
+-rw-r--r--   0        0        0       49 2023-05-02 10:18:08.309755 mlcvzoo_yolox-6.0.1/mlcvzoo_yolox/third_party/yolox/tools/__init__.py
+-rw-r--r--   0        0        0     1528 2023-05-02 10:18:08.309755 mlcvzoo_yolox-6.0.1/mlcvzoo_yolox/third_party/yolox/tools/train.py
+-rw-r--r--   0        0        0     2745 2023-05-02 10:18:08.309755 mlcvzoo_yolox-6.0.1/mlcvzoo_yolox/third_party/yolox/tools/trt.py
+-rw-r--r--   0        0        0       49 2023-05-02 10:18:08.309755 mlcvzoo_yolox-6.0.1/mlcvzoo_yolox/third_party/yolox/utils/__init__.py
+-rw-r--r--   0        0        0     2374 2023-05-03 12:33:28.187548 mlcvzoo_yolox-6.0.1/mlcvzoo_yolox/third_party/yolox/utils/boxes.py
+-rw-r--r--   0        0        0     5384 2023-05-05 09:21:26.586902 mlcvzoo_yolox-6.0.1/pyproject.toml
+-rw-r--r--   0        0        0     2005 1970-01-01 00:00:00.000000 mlcvzoo_yolox-6.0.1/setup.py
+-rw-r--r--   0        0        0     2289 1970-01-01 00:00:00.000000 mlcvzoo_yolox-6.0.1/PKG-INFO
```

### Comparing `mlcvzoo_yolox-6.0.0/mlcvzoo_yolox/configuration.py` & `mlcvzoo_yolox-6.0.1/mlcvzoo_yolox/configuration.py`

 * *Files 0% similar despite different names*

```diff
@@ -30,15 +30,14 @@
     # Dictionary for overwriting attributes of the loaded
     # base experiment
     attribute_overwrite: Dict[str, Any] = related.ChildField(
         cls=dict, default={}, required=False
     )
 
     def check_values(self) -> bool:
-
         if self.exp_type not in [str(d.value.upper()) for d in YOLOXExperiments]:
             raise ValueError(
                 f"Exp-type='{self.exp_type}' not valid. Please provide one of "
                 f"{[str(d.value.upper()) for d in YOLOXExperiments]}"
             )
 
         return True
```

### Comparing `mlcvzoo_yolox-6.0.0/mlcvzoo_yolox/core/trainer.py` & `mlcvzoo_yolox-6.0.1/mlcvzoo_yolox/core/trainer.py`

 * *Files 14% similar despite different names*

```diff
@@ -20,15 +20,14 @@
 class YoloxTrainer(Trainer):
     """
     Define a custom yolox Trainer class to adapt some of the
     predefined behavior.
     """
 
     def __init__(self, exp: CustomYOLOXExp, args: argparse.Namespace) -> None:
-
         Trainer.__init__(self, exp=exp, args=args)
 
         self.exp = cast(CustomYOLOXExp, self.exp)  # type: ignore
 
         # Save the original configured evaluation interval for use in the method before_epoch(...)
         self.original_eval_interval = self.exp.eval_interval
 
@@ -38,14 +37,19 @@
         # experiment name. This is an unwanted behavior.
         self.file_name = os.path.join(exp.output_dir)
 
     def after_epoch(self) -> None:
         """
         Define relevant steps that are executed after each training epoch
 
+        IMPORTANT: In the yolox Trainer base class, this method starts
+                   an evaluation. We decided to execute the evaluation
+                   separately from the training. Therefore, there is
+                   currently no evaluation routine during the training.
+
         Returns:
             None
         """
 
         if self.epoch % self.exp.checkpoint_interval == 0:
             all_reduce_norm(self.model)
             self.save_ckpt(ckpt_name=f"{self.exp.exp_name}_{self.epoch}")
```

### Comparing `mlcvzoo_yolox-6.0.0/mlcvzoo_yolox/data/datasets/dataset.py` & `mlcvzoo_yolox-6.0.1/mlcvzoo_yolox/data/datasets/dataset.py`

 * *Files 4% similar despite different names*

```diff
@@ -130,15 +130,14 @@
         Returns:
             a list containing lists of bounding boxes  [bbox coords, class name]
         """
 
         yolox_data_array = np.empty((0, 5))
 
         for bounding_box in annotation.get_bounding_boxes(include_segmentations=True):
-
             bndbox = [
                 bounding_box.box.xmin,
                 bounding_box.box.ymin,
                 bounding_box.box.xmax,
                 bounding_box.box.ymax,
                 bounding_box.class_id,
             ]
```

### Comparing `mlcvzoo_yolox-6.0.0/mlcvzoo_yolox/evaluators/evaluator.py` & `mlcvzoo_yolox-6.0.1/mlcvzoo_yolox/evaluators/evaluator.py`

 * *Files 2% similar despite different names*

```diff
@@ -86,15 +86,15 @@
             model = model.half()
 
         progress_bar = tqdm if is_main_process() else iter
 
         for cur_iter, (imgs, _, info_imgs, ids) in enumerate(
             progress_bar(self.dataloader)
         ):
-            with torch.no_grad():  # type: ignore
+            with torch.no_grad():
                 imgs = imgs.type(tensor_type)
 
                 _, bounding_boxes = predict_with_model(
                     model=model,
                     data_item=imgs,
                     preprocess=None,
                     inference_config=self.configuration.inference_config,
```

### Comparing `mlcvzoo_yolox-6.0.0/mlcvzoo_yolox/exp/custom_yolox_exp.py` & `mlcvzoo_yolox-6.0.1/mlcvzoo_yolox/exp/custom_yolox_exp.py`

 * *Files 0% similar despite different names*

```diff
@@ -130,15 +130,14 @@
         if self.configuration.train_config is None:
             raise ValueError(
                 "train_config is None! In order to be able to train a yolox model"
                 "a valid train_config has to be provided!"
             )
 
         with wait_for_the_master(local_rank):
-
             dataset = MLCVZooDataset(
                 annotation_handler=AnnotationHandler(
                     mapper=self.mapper,
                     configuration=self.configuration.train_config.train_annotation_handler_config,
                 ),
                 img_size=self.input_size,
                 preproc=TrainTransform(
```

### Comparing `mlcvzoo_yolox-6.0.0/mlcvzoo_yolox/exp/default.py` & `mlcvzoo_yolox-6.0.1/mlcvzoo_yolox/exp/default.py`

 * *Files 7% similar despite different names*

```diff
@@ -12,15 +12,14 @@
     S = "S"
     M = "M"
     L = "L"
     X = "X"
 
 
 class YOLOXSettingsTuple(NamedTuple):
-
     constructor: Type[YOLOXBaseExp]
     attribute_dict: Dict[str, Any]
 
 
 yolox_experiment_settings: Dict[str, YOLOXSettingsTuple] = {
     YOLOXExperiments.NANO.value.upper(): YOLOXSettingsTuple(
         constructor=YOLOXNanoExp, attribute_dict={}  # everything as in default
```

### Comparing `mlcvzoo_yolox-6.0.0/mlcvzoo_yolox/model.py` & `mlcvzoo_yolox-6.0.1/mlcvzoo_yolox/model.py`

 * *Files identical despite different names*

### Comparing `mlcvzoo_yolox-6.0.0/mlcvzoo_yolox/model_utils.py` & `mlcvzoo_yolox-6.0.1/mlcvzoo_yolox/model_utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -207,19 +207,18 @@
         image_tensor = transform_np_to_torch_image(
             np_image=preprocessed_np_image, inference_config=inference_config
         )
 
     # run prediction and postprocess the output
     # NOTE: mypy error 'Call to untyped function "close" in typed context'
     #       can be ignored
-    with torch.no_grad():  # type: ignore
+    with torch.no_grad():
         yolox_model_outputs = model(image_tensor)
 
         if decode_output:
-
             if strides is None:
                 raise ValueError(
                     "In order to be able to decode the output, the "
                     "'strides' parameters has to be provided!"
                 )
 
             output_dim = []
```

### Comparing `mlcvzoo_yolox-6.0.0/mlcvzoo_yolox/third_party/yolox/LICENSE` & `mlcvzoo_yolox-6.0.1/mlcvzoo_yolox/third_party/yolox/LICENSE`

 * *Files identical despite different names*

### Comparing `mlcvzoo_yolox-6.0.0/mlcvzoo_yolox/third_party/yolox/exps/yolox_base.py` & `mlcvzoo_yolox-6.0.1/mlcvzoo_yolox/third_party/yolox/exps/yolox_base.py`

 * *Files identical despite different names*

### Comparing `mlcvzoo_yolox-6.0.0/mlcvzoo_yolox/third_party/yolox/exps/yolox_nano.py` & `mlcvzoo_yolox-6.0.1/mlcvzoo_yolox/third_party/yolox/exps/yolox_nano.py`

 * *Files identical despite different names*

### Comparing `mlcvzoo_yolox-6.0.0/mlcvzoo_yolox/third_party/yolox/models/yolo_head.py` & `mlcvzoo_yolox-6.0.1/mlcvzoo_yolox/third_party/yolox/models/yolo_head.py`

 * *Files identical despite different names*

### Comparing `mlcvzoo_yolox-6.0.0/mlcvzoo_yolox/third_party/yolox/tools/train.py` & `mlcvzoo_yolox-6.0.1/mlcvzoo_yolox/third_party/yolox/tools/train.py`

 * *Files identical despite different names*

### Comparing `mlcvzoo_yolox-6.0.0/mlcvzoo_yolox/third_party/yolox/tools/trt.py` & `mlcvzoo_yolox-6.0.1/mlcvzoo_yolox/third_party/yolox/tools/trt.py`

 * *Files identical despite different names*

### Comparing `mlcvzoo_yolox-6.0.0/mlcvzoo_yolox/third_party/yolox/utils/boxes.py` & `mlcvzoo_yolox-6.0.1/mlcvzoo_yolox/third_party/yolox/utils/boxes.py`

 * *Files 0% similar despite different names*

```diff
@@ -21,15 +21,14 @@
     box_corner[:, :, 1] = prediction[:, :, 1] - prediction[:, :, 3] / 2
     box_corner[:, :, 2] = prediction[:, :, 0] + prediction[:, :, 2] / 2
     box_corner[:, :, 3] = prediction[:, :, 1] + prediction[:, :, 3] / 2
     prediction[:, :, :4] = box_corner[:, :, :4]
 
     output = [None for _ in range(len(prediction))]
     for i, image_pred in enumerate(prediction):
-
         # If none are remaining => process next image
         if not image_pred.size(0):
             continue
         # Get score and class with the highest confidence
         class_conf, class_pred = torch.max(
             image_pred[:, 5 : 5 + num_classes], 1, keepdim=True
         )
```

### Comparing `mlcvzoo_yolox-6.0.0/pyproject.toml` & `mlcvzoo_yolox-6.0.1/pyproject.toml`

 * *Files 27% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "mlcvzoo_yolox"
-version = "6.0.0"
+version = "6.0.1"
 license = "Open Logistics License Version 1.0"
 description = "MLCVZoo YOLOX Package"
 readme = "README.md"
 homepage = "https://git.openlogisticsfoundation.org/silicon-economy/base/ml-toolbox/mlcvzoo"
 repository = "https://git.openlogisticsfoundation.org/silicon-economy/base/ml-toolbox/mlcvzoo"
 documentation = "https://git.openlogisticsfoundation.org/silicon-economy/base/ml-toolbox/mlcvzoo/-/blob/main/documentation/index.adoc"
 classifiers = [
@@ -45,38 +45,54 @@
 nvidia-tensorrt = { version = "8.4.2.4", source = "nvidia-ngc", optional=true }
 # Builds and installs just fine but only _after_ torch is available, run
 #     poetry run python3 -m pip install "git+https://github.com/NVIDIA-AI-IOT/torch2trt.git@11073308f5fbbc06ba8c33bd41fe43e25d03a861"
 # after poetry install instead
 # torch2trt = { git = "https://github.com/NVIDIA-AI-IOT/torch2trt", rev = "11073308f5fbbc06ba8c33bd41fe43e25d03a861", optional=true }
 # 1.19.2 is oldest available on aarch64 but 1.19.5 leads to unbuildable pytorch there, all is well on amd64
 numpy = { version = ">=1.19.2,!=1.19.5" }
-nptyping = { version = "^2.0" }
+nptyping = { version = ">=2.0" }
 opencv-python = { version = "^4.5,!=4.5.5.64" }
 opencv-contrib-python = { version = "^4.5,!=4.5.5.64" }
-# TODO: remove when fixed by tensorboard: https://github.com/tensorflow/tensorboard/issues/5703
-protobuf =  { version = "<=3.20" }
-torch = { version = "^1.9" }
-torchvision = { version = "^0.10" }
-# This mioght fail because it needs --no-use-pep-517, so install it afterwards manually:
+torch = { version = ">=1.9" }
+torchvision = { version = ">=0.10" }
+# This might fail because it needs --no-use-pep-517, so install it afterwards manually:
 #    poetry run python -m pip install --no-use-pep517 --no-binary yolox
 # You may use build.sh as a wrapper for poetry install/update to automate this
-yolox = { version = "~0.3" }
+#yolox = { version = "~0.3" }
+#yolox = { git = "https://github.com/Megvii-BaseDetection/YOLOX.git", rev = "bb9185c095dfd7a8015a1b82f3e9a065090860b8" }
+# YOLOX is uninstallable in its current form on anything > python 3.8 so
+# just depend on YOLOX's dependencies as specified in bb9185c095dfd7a8015a1b82f3e9a065090860b8 and install
+# YOLOX afterwards. You may use build.sh as a wrapper for poetry install/update to automate this
+loguru = { version = "*" }
+tqdm = { version = "*" }
+thop = { version = "*" }
+ninja = { version = "*" }
+tabulate = { version = "*" }
+psutil = { version = "*" }
+tensorboard = { version = "*" }
+# verified versions
+# pycocotools corresponds to https://github.com/ppwwyyxx/cocoapi
+pycocotools = { version = ">=2.0.2" }
+onnx  = { version = ">=1.13.0", optional=true }
+onnx-simplifier  = { version = "==0.4.10", optional=true }
 
 [tool.poetry.extras]
 tensorrt = ["nvidia-tensorrt"]
+onnx = ["onnx", "onnx-simplifier"]
 
 [tool.poetry.dev-dependencies]
-mock = { version = "^4.0" }
-pytest = { version = "^7.0" }
-pytest-cov = { version = "^3.0.0" }
-black = { version = "^22" }
+mock = { version = ">=4.0" }
+pytest = { version = ">=7.0" }
+pytest-cov = { version = ">=3.0.0" }
+black = { version = ">=22" }
 mypy = { version = ">=0.961" }
-pylint = { version = "^2.9.6" }
-isort = { version = "^5.9" }
-pytest-mock = "^3.7"
+pylint = { version = ">=2.9.6" }
+isort = { version = ">=5.9" }
+pytest-mock = ">=3.7"
+torch = {version = "*"}
 
 [build-system]
 # NOTE: Don't remove setuptools, therefore require it from the build system
 requires = ["setuptools", "poetry_core>=1.0", "torch"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.isort]
```

### Comparing `mlcvzoo_yolox-6.0.0/setup.py` & `mlcvzoo_yolox-6.0.1/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -16,32 +16,39 @@
  'mlcvzoo_yolox.third_party.yolox.utils']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
 ['attrs>=20',
+ 'loguru',
  'mlcvzoo_base>=5.0,<6.0',
- 'nptyping>=2.0,<3.0',
+ 'ninja',
+ 'nptyping>=2.0',
  'numpy>=1.19.2,!=1.19.5',
  'opencv-contrib-python>=4.5,<5.0,!=4.5.5.64',
  'opencv-python>=4.5,<5.0,!=4.5.5.64',
- 'protobuf<=3.20',
+ 'psutil',
+ 'pycocotools>=2.0.2',
  'related-mltoolbox>=1.0,<2.0',
- 'torch>=1.9,<2.0',
- 'torchvision>=0.10,<0.11',
- 'yaml-config-builder>=8,<9',
- 'yolox>=0.3,<0.4']
+ 'tabulate',
+ 'tensorboard',
+ 'thop',
+ 'torch>=1.9',
+ 'torchvision>=0.10',
+ 'tqdm',
+ 'yaml-config-builder>=8,<9']
 
 extras_require = \
-{'tensorrt': ['nvidia-tensorrt==8.4.2.4']}
+{'onnx': ['onnx>=1.13.0', 'onnx-simplifier==0.4.10'],
+ 'tensorrt': ['nvidia-tensorrt==8.4.2.4']}
 
 setup_kwargs = {
     'name': 'mlcvzoo-yolox',
-    'version': '6.0.0',
+    'version': '6.0.1',
     'description': 'MLCVZoo YOLOX Package',
     'long_description': '# MLCVZoo YOLOX\n\nThe MLCVZoo is an SDK for simplifying the usage of various (machine learning driven)\ncomputer vision algorithms. The package **mlcvzoo_yolox** is the wrapper module for\nthe [yolox Object Detector](https://github.com/Megvii-BaseDetection/YOLOX).\n\nFurther information about the MLCVZoo can be found [here](../README.md).\n\n## Install\n`\npip install mlcvzoo-yolox\n`\n\n## Technology stack\n\n- Python\n',
     'author': 'Maximilian Otten',
     'author_email': 'maximilian.otten@iml.fraunhofer.de',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://git.openlogisticsfoundation.org/silicon-economy/base/ml-toolbox/mlcvzoo',
```

### Comparing `mlcvzoo_yolox-6.0.0/PKG-INFO` & `mlcvzoo_yolox-6.0.1/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mlcvzoo-yolox
-Version: 6.0.0
+Version: 6.0.1
 Summary: MLCVZoo YOLOX Package
 Home-page: https://git.openlogisticsfoundation.org/silicon-economy/base/ml-toolbox/mlcvzoo
 License: Open Logistics License Version 1.0
 Author: Maximilian Otten
 Author-email: maximilian.otten@iml.fraunhofer.de
 Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 5 - Production/Stable
@@ -12,28 +12,37 @@
 Classifier: License :: Other/Proprietary License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Provides-Extra: onnx
 Provides-Extra: tensorrt
 Requires-Dist: attrs (>=20)
+Requires-Dist: loguru
 Requires-Dist: mlcvzoo_base (>=5.0,<6.0)
-Requires-Dist: nptyping (>=2.0,<3.0)
+Requires-Dist: ninja
+Requires-Dist: nptyping (>=2.0)
 Requires-Dist: numpy (>=1.19.2,!=1.19.5)
 Requires-Dist: nvidia-tensorrt (==8.4.2.4) ; extra == "tensorrt"
+Requires-Dist: onnx (>=1.13.0) ; extra == "onnx"
+Requires-Dist: onnx-simplifier (==0.4.10) ; extra == "onnx"
 Requires-Dist: opencv-contrib-python (>=4.5,<5.0,!=4.5.5.64)
 Requires-Dist: opencv-python (>=4.5,<5.0,!=4.5.5.64)
-Requires-Dist: protobuf (<=3.20)
+Requires-Dist: psutil
+Requires-Dist: pycocotools (>=2.0.2)
 Requires-Dist: related-mltoolbox (>=1.0,<2.0)
-Requires-Dist: torch (>=1.9,<2.0)
-Requires-Dist: torchvision (>=0.10,<0.11)
+Requires-Dist: tabulate
+Requires-Dist: tensorboard
+Requires-Dist: thop
+Requires-Dist: torch (>=1.9)
+Requires-Dist: torchvision (>=0.10)
+Requires-Dist: tqdm
 Requires-Dist: yaml-config-builder (>=8,<9)
-Requires-Dist: yolox (>=0.3,<0.4)
 Project-URL: Documentation, https://git.openlogisticsfoundation.org/silicon-economy/base/ml-toolbox/mlcvzoo/-/blob/main/documentation/index.adoc
 Project-URL: Repository, https://git.openlogisticsfoundation.org/silicon-economy/base/ml-toolbox/mlcvzoo
 Description-Content-Type: text/markdown
 
 # MLCVZoo YOLOX
 
 The MLCVZoo is an SDK for simplifying the usage of various (machine learning driven)
```

