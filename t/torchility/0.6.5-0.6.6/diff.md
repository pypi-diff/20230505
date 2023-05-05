# Comparing `tmp/torchility-0.6.5.tar.gz` & `tmp/torchility-0.6.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "torchility-0.6.5.tar", last modified: Fri May  5 12:14:22 2023, max compression
+gzip compressed data, was "torchility-0.6.6.tar", last modified: Fri May  5 13:47:18 2023, max compression
```

## Comparing `torchility-0.6.5.tar` & `torchility-0.6.6.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 liuchen    (501) staff       (20)        0 2023-05-05 12:14:22.410032 torchility-0.6.5/
--rw-r--r--   0 liuchen    (501) staff       (20)     1073 2020-01-28 04:19:18.000000 torchility-0.6.5/LICENSE
--rw-r--r--   0 liuchen    (501) staff       (20)     2074 2023-05-05 12:14:22.406164 torchility-0.6.5/PKG-INFO
--rw-r--r--   0 liuchen    (501) staff       (20)     1595 2023-03-20 06:35:45.000000 torchility-0.6.5/README.md
-drwxr-xr-x   0 liuchen    (501) staff       (20)        0 2023-05-05 12:14:22.378023 torchility-0.6.5/examples/
--rw-r--r--   0 liuchen    (501) staff       (20)     1675 2023-03-27 12:31:34.000000 torchility-0.6.5/examples/1-mnist.py
--rw-r--r--   0 liuchen    (501) staff       (20)     2663 2023-03-28 13:54:47.000000 torchility-0.6.5/examples/2-mnist_callbacks.py
--rw-r--r--   0 liuchen    (501) staff       (20)     2223 2023-05-05 12:11:38.000000 torchility-0.6.5/examples/3-mnist_interpreter.py
--rw-r--r--   0 liuchen    (501) staff       (20)     1709 2022-03-31 07:25:03.000000 torchility-0.6.5/examples/4-mnist_model_analysis.py
--rw-r--r--   0 liuchen    (501) staff       (20)     1419 2022-05-28 01:44:42.000000 torchility-0.6.5/examples/5-mnist_lr_find.py
--rw-r--r--   0 liuchen    (501) staff       (20)     1962 2022-12-09 04:27:52.000000 torchility-0.6.5/examples/6-graph_node_clasification_DGL.py
--rw-r--r--   0 liuchen    (501) staff       (20)       38 2023-05-05 12:14:22.410206 torchility-0.6.5/setup.cfg
--rw-r--r--   0 liuchen    (501) staff       (20)     1117 2023-05-05 12:13:44.000000 torchility-0.6.5/setup.py
-drwxr-xr-x   0 liuchen    (501) staff       (20)        0 2023-05-05 12:14:22.389026 torchility-0.6.5/torchility/
--rw-r--r--   0 liuchen    (501) staff       (20)      503 2023-05-05 12:14:06.000000 torchility-0.6.5/torchility/__init__.py
-drwxr-xr-x   0 liuchen    (501) staff       (20)        0 2023-05-05 12:14:22.399275 torchility-0.6.5/torchility/callbacks/
--rw-r--r--   0 liuchen    (501) staff       (20)      101 2022-05-08 12:50:22.000000 torchility-0.6.5/torchility/callbacks/__init__.py
--rw-r--r--   0 liuchen    (501) staff       (20)     1153 2023-03-28 13:49:32.000000 torchility-0.6.5/torchility/callbacks/common.py
--rw-r--r--   0 liuchen    (501) staff       (20)     4730 2023-05-05 12:09:25.000000 torchility-0.6.5/torchility/callbacks/interpreters.py
--rw-r--r--   0 liuchen    (501) staff       (20)     3036 2023-03-19 07:43:59.000000 torchility-0.6.5/torchility/callbacks/performances.py
--rw-r--r--   0 liuchen    (501) staff       (20)    10012 2023-03-19 09:26:35.000000 torchility-0.6.5/torchility/callbacks/progress.py
--rw-r--r--   0 liuchen    (501) staff       (20)     2390 2021-06-09 14:49:55.000000 torchility-0.6.5/torchility/hooks.py
--rw-r--r--   0 liuchen    (501) staff       (20)      577 2021-06-10 07:05:35.000000 torchility-0.6.5/torchility/losses.py
--rw-r--r--   0 liuchen    (501) staff       (20)     4932 2023-03-28 13:36:07.000000 torchility-0.6.5/torchility/metrics.py
--rw-r--r--   0 liuchen    (501) staff       (20)     5971 2023-03-28 13:41:27.000000 torchility-0.6.5/torchility/tasks.py
--rw-r--r--   0 liuchen    (501) staff       (20)    11360 2023-03-28 13:33:59.000000 torchility-0.6.5/torchility/trainer.py
-drwxr-xr-x   0 liuchen    (501) staff       (20)        0 2023-05-05 12:14:22.403051 torchility-0.6.5/torchility/utils/
--rw-r--r--   0 liuchen    (501) staff       (20)       68 2022-06-01 16:09:54.000000 torchility-0.6.5/torchility/utils/__init__.py
--rw-r--r--   0 liuchen    (501) staff       (20)     4222 2022-06-02 14:28:56.000000 torchility-0.6.5/torchility/utils/plots.py
--rw-r--r--   0 liuchen    (501) staff       (20)     6050 2023-05-05 01:14:22.000000 torchility-0.6.5/torchility/utils/utils.py
--rw-r--r--   0 liuchen    (501) staff       (20)     3014 2022-08-04 03:32:03.000000 torchility-0.6.5/torchility/utils/yaml_config.py
-drwxr-xr-x   0 liuchen    (501) staff       (20)        0 2023-05-05 12:14:22.394754 torchility-0.6.5/torchility.egg-info/
--rw-r--r--   0 liuchen    (501) staff       (20)     2074 2023-05-05 12:14:22.000000 torchility-0.6.5/torchility.egg-info/PKG-INFO
--rw-r--r--   0 liuchen    (501) staff       (20)      795 2023-05-05 12:14:22.000000 torchility-0.6.5/torchility.egg-info/SOURCES.txt
--rw-r--r--   0 liuchen    (501) staff       (20)        1 2023-05-05 12:14:22.000000 torchility-0.6.5/torchility.egg-info/dependency_links.txt
--rw-r--r--   0 liuchen    (501) staff       (20)       83 2023-05-05 12:14:22.000000 torchility-0.6.5/torchility.egg-info/requires.txt
--rw-r--r--   0 liuchen    (501) staff       (20)       11 2023-05-05 12:14:22.000000 torchility-0.6.5/torchility.egg-info/top_level.txt
+drwxr-xr-x   0 liuchen    (501) staff       (20)        0 2023-05-05 13:47:18.445943 torchility-0.6.6/
+-rw-r--r--   0 liuchen    (501) staff       (20)     1073 2020-01-28 04:19:18.000000 torchility-0.6.6/LICENSE
+-rw-r--r--   0 liuchen    (501) staff       (20)     2074 2023-05-05 13:47:18.445508 torchility-0.6.6/PKG-INFO
+-rw-r--r--   0 liuchen    (501) staff       (20)     1595 2023-03-20 06:35:45.000000 torchility-0.6.6/README.md
+drwxr-xr-x   0 liuchen    (501) staff       (20)        0 2023-05-05 13:47:18.430550 torchility-0.6.6/examples/
+-rw-r--r--   0 liuchen    (501) staff       (20)     1675 2023-03-27 12:31:34.000000 torchility-0.6.6/examples/1-mnist.py
+-rw-r--r--   0 liuchen    (501) staff       (20)     2663 2023-03-28 13:54:47.000000 torchility-0.6.6/examples/2-mnist_callbacks.py
+-rw-r--r--   0 liuchen    (501) staff       (20)     2223 2023-05-05 13:45:53.000000 torchility-0.6.6/examples/3-mnist_interpreter.py
+-rw-r--r--   0 liuchen    (501) staff       (20)     1709 2022-03-31 07:25:03.000000 torchility-0.6.6/examples/4-mnist_model_analysis.py
+-rw-r--r--   0 liuchen    (501) staff       (20)     1419 2022-05-28 01:44:42.000000 torchility-0.6.6/examples/5-mnist_lr_find.py
+-rw-r--r--   0 liuchen    (501) staff       (20)     1962 2022-12-09 04:27:52.000000 torchility-0.6.6/examples/6-graph_node_clasification_DGL.py
+-rw-r--r--   0 liuchen    (501) staff       (20)       38 2023-05-05 13:47:18.446202 torchility-0.6.6/setup.cfg
+-rw-r--r--   0 liuchen    (501) staff       (20)     1117 2023-05-05 12:13:44.000000 torchility-0.6.6/setup.py
+drwxr-xr-x   0 liuchen    (501) staff       (20)        0 2023-05-05 13:47:18.435544 torchility-0.6.6/torchility/
+-rw-r--r--   0 liuchen    (501) staff       (20)      503 2023-05-05 13:44:59.000000 torchility-0.6.6/torchility/__init__.py
+drwxr-xr-x   0 liuchen    (501) staff       (20)        0 2023-05-05 13:47:18.441932 torchility-0.6.6/torchility/callbacks/
+-rw-r--r--   0 liuchen    (501) staff       (20)      101 2022-05-08 12:50:22.000000 torchility-0.6.6/torchility/callbacks/__init__.py
+-rw-r--r--   0 liuchen    (501) staff       (20)     1153 2023-03-28 13:49:32.000000 torchility-0.6.6/torchility/callbacks/common.py
+-rw-r--r--   0 liuchen    (501) staff       (20)     4840 2023-05-05 13:46:18.000000 torchility-0.6.6/torchility/callbacks/interpreters.py
+-rw-r--r--   0 liuchen    (501) staff       (20)     3036 2023-03-19 07:43:59.000000 torchility-0.6.6/torchility/callbacks/performances.py
+-rw-r--r--   0 liuchen    (501) staff       (20)    10012 2023-03-19 09:26:35.000000 torchility-0.6.6/torchility/callbacks/progress.py
+-rw-r--r--   0 liuchen    (501) staff       (20)     2390 2021-06-09 14:49:55.000000 torchility-0.6.6/torchility/hooks.py
+-rw-r--r--   0 liuchen    (501) staff       (20)      577 2021-06-10 07:05:35.000000 torchility-0.6.6/torchility/losses.py
+-rw-r--r--   0 liuchen    (501) staff       (20)     4932 2023-03-28 13:36:07.000000 torchility-0.6.6/torchility/metrics.py
+-rw-r--r--   0 liuchen    (501) staff       (20)     5971 2023-03-28 13:41:27.000000 torchility-0.6.6/torchility/tasks.py
+-rw-r--r--   0 liuchen    (501) staff       (20)    11360 2023-03-28 13:33:59.000000 torchility-0.6.6/torchility/trainer.py
+drwxr-xr-x   0 liuchen    (501) staff       (20)        0 2023-05-05 13:47:18.444491 torchility-0.6.6/torchility/utils/
+-rw-r--r--   0 liuchen    (501) staff       (20)       68 2022-06-01 16:09:54.000000 torchility-0.6.6/torchility/utils/__init__.py
+-rw-r--r--   0 liuchen    (501) staff       (20)     4222 2022-06-02 14:28:56.000000 torchility-0.6.6/torchility/utils/plots.py
+-rw-r--r--   0 liuchen    (501) staff       (20)     6050 2023-05-05 01:14:22.000000 torchility-0.6.6/torchility/utils/utils.py
+-rw-r--r--   0 liuchen    (501) staff       (20)     3014 2022-08-04 03:32:03.000000 torchility-0.6.6/torchility/utils/yaml_config.py
+drwxr-xr-x   0 liuchen    (501) staff       (20)        0 2023-05-05 13:47:18.438630 torchility-0.6.6/torchility.egg-info/
+-rw-r--r--   0 liuchen    (501) staff       (20)     2074 2023-05-05 13:47:18.000000 torchility-0.6.6/torchility.egg-info/PKG-INFO
+-rw-r--r--   0 liuchen    (501) staff       (20)      795 2023-05-05 13:47:18.000000 torchility-0.6.6/torchility.egg-info/SOURCES.txt
+-rw-r--r--   0 liuchen    (501) staff       (20)        1 2023-05-05 13:47:18.000000 torchility-0.6.6/torchility.egg-info/dependency_links.txt
+-rw-r--r--   0 liuchen    (501) staff       (20)       83 2023-05-05 13:47:18.000000 torchility-0.6.6/torchility.egg-info/requires.txt
+-rw-r--r--   0 liuchen    (501) staff       (20)       11 2023-05-05 13:47:18.000000 torchility-0.6.6/torchility.egg-info/top_level.txt
```

### Comparing `torchility-0.6.5/LICENSE` & `torchility-0.6.6/LICENSE`

 * *Files identical despite different names*

### Comparing `torchility-0.6.5/PKG-INFO` & `torchility-0.6.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: torchility
-Version: 0.6.5
+Version: 0.6.6
 Summary: UNKNOWN
 Home-page: https://github.com/hitlic/torchility
 Author: hitlic
 Author-email: liuchen.lic@gmail.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `torchility-0.6.5/README.md` & `torchility-0.6.6/README.md`

 * *Files identical despite different names*

### Comparing `torchility-0.6.5/examples/1-mnist.py` & `torchility-0.6.6/examples/1-mnist.py`

 * *Files identical despite different names*

### Comparing `torchility-0.6.5/examples/2-mnist_callbacks.py` & `torchility-0.6.6/examples/2-mnist_callbacks.py`

 * *Files identical despite different names*

### Comparing `torchility-0.6.5/examples/3-mnist_interpreter.py` & `torchility-0.6.6/examples/3-mnist_interpreter.py`

 * *Files 0% similar despite different names*

```diff
@@ -43,15 +43,15 @@
 # 4. --- 训练
 
 # 要计算每个样本的指标，因此不能reduction（即求和、平均等操作）
 metric = nn.CrossEntropyLoss(reduction='none')
 
 interpreter = ClassifierInterpreter(metric=metric, k=15, class_num=10, stage='test')          # 针对分类模型测试数据的解释器
 trainer = Trainer(model, F.cross_entropy, opt,                           # 训练器
-                  epochs=5, callbacks=[interpreter])
+                  epochs=1, callbacks=[interpreter])
 trainer.fit(train_dl, val_dl)                                            # 训练、验证
 trainer.test(test_dl)                                                    # 测试
 
 
 # 5. --- 解释
 
 # 返回测试集中损失最大的k个样本的信息
```

### Comparing `torchility-0.6.5/examples/4-mnist_model_analysis.py` & `torchility-0.6.6/examples/4-mnist_model_analysis.py`

 * *Files identical despite different names*

### Comparing `torchility-0.6.5/examples/5-mnist_lr_find.py` & `torchility-0.6.6/examples/5-mnist_lr_find.py`

 * *Files identical despite different names*

### Comparing `torchility-0.6.5/examples/6-graph_node_clasification_DGL.py` & `torchility-0.6.6/examples/6-graph_node_clasification_DGL.py`

 * *Files identical despite different names*

### Comparing `torchility-0.6.5/setup.py` & `torchility-0.6.6/setup.py`

 * *Files identical despite different names*

### Comparing `torchility-0.6.5/torchility/callbacks/common.py` & `torchility-0.6.6/torchility/callbacks/common.py`

 * *Files identical despite different names*

### Comparing `torchility-0.6.5/torchility/callbacks/interpreters.py` & `torchility-0.6.6/torchility/callbacks/interpreters.py`

 * *Files 10% similar despite different names*

```diff
@@ -39,36 +39,37 @@
     def on_test_epoch_start(self, trainer, pl_module):
         self.batch_recorder = []
 
     def on_train_batch_end(self, trainer, pl_module, outputs, batch, batch_idx):
         if self.stage == 'train':
             self.batch_recorder.append(pl_module.messages['train_batch'])
             _, preds, targets = pl_module.messages['train_batch']
-            self.put_queue(preds, targets, batch[0])
+            self.put_queue(preds, targets, *batch[:-1])
 
     def on_validation_batch_end(self, trainer, pl_module, outputs, batch, batch_idx):
         if self.stage == 'val':
             self.batch_recorder.append(pl_module.messages['val_batch'])
             _, preds, targets = pl_module.messages['val_batch']
-            self.put_queue(preds, targets, batch[0])
+            self.put_queue(preds, targets, *batch[:-1])
 
     def on_test_batch_end(self, trainer, pl_module, outputs, batch, batch_idx):
         if self.stage == 'test':
             self.batch_recorder.append(pl_module.messages['test_batch'])
             _, preds, targets = pl_module.messages['test_batch']
-            self.put_queue(preds, targets, batch[0])
+            self.put_queue(preds, targets, *batch[:-1])
 
-    def put_queue(self, preds, targets, inputs):
+    def put_queue(self, preds, targets, *inputs):
         if self.metric is None:
             return
         batch_m = self.metric(preds, targets)
         assert batch_m.shape[0] == preds.shape[0], 'The `metric` must not be reduced!'
-        for m, pred, target, x in zip(batch_m.cpu(), preds.cpu(), targets.cpu(), inputs.cpu()):
+        for m, pred, target, *xs in zip(batch_m.cpu(), preds.cpu(), targets.cpu(), *[ipt.cpu() for ipt in inputs]):
             v = -m if self.mode == 'min' else m
-            self.top_queue.put((v.item(), [m.item(), pred.detach().numpy(), target.detach().numpy(), x.detach().numpy()]))
+            feat = xs[0].detach().numpy() if len(xs)==1 else [x.detach().numpy() for x in xs]
+            self.top_queue.put((v.item(), [m.item(), pred.detach().numpy(), target.detach().numpy(), feat]))
 
     def top_samples(self):
         """
         Return: [metric_value, pred, target, input_feat] of top k samples 
         """
         samples = [item[1] for item in self.top_queue.items()]
         return samples
```

### Comparing `torchility-0.6.5/torchility/callbacks/performances.py` & `torchility-0.6.6/torchility/callbacks/performances.py`

 * *Files identical despite different names*

### Comparing `torchility-0.6.5/torchility/callbacks/progress.py` & `torchility-0.6.6/torchility/callbacks/progress.py`

 * *Files identical despite different names*

### Comparing `torchility-0.6.5/torchility/hooks.py` & `torchility-0.6.6/torchility/hooks.py`

 * *Files identical despite different names*

### Comparing `torchility-0.6.5/torchility/losses.py` & `torchility-0.6.6/torchility/losses.py`

 * *Files identical despite different names*

### Comparing `torchility-0.6.5/torchility/metrics.py` & `torchility-0.6.6/torchility/metrics.py`

 * *Files identical despite different names*

### Comparing `torchility-0.6.5/torchility/tasks.py` & `torchility-0.6.6/torchility/tasks.py`

 * *Files identical despite different names*

### Comparing `torchility-0.6.5/torchility/trainer.py` & `torchility-0.6.6/torchility/trainer.py`

 * *Files identical despite different names*

### Comparing `torchility-0.6.5/torchility/utils/plots.py` & `torchility-0.6.6/torchility/utils/plots.py`

 * *Files identical despite different names*

### Comparing `torchility-0.6.5/torchility/utils/utils.py` & `torchility-0.6.6/torchility/utils/utils.py`

 * *Files identical despite different names*

### Comparing `torchility-0.6.5/torchility/utils/yaml_config.py` & `torchility-0.6.6/torchility/utils/yaml_config.py`

 * *Files identical despite different names*

### Comparing `torchility-0.6.5/torchility.egg-info/PKG-INFO` & `torchility-0.6.6/torchility.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: torchility
-Version: 0.6.5
+Version: 0.6.6
 Summary: UNKNOWN
 Home-page: https://github.com/hitlic/torchility
 Author: hitlic
 Author-email: liuchen.lic@gmail.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `torchility-0.6.5/torchility.egg-info/SOURCES.txt` & `torchility-0.6.6/torchility.egg-info/SOURCES.txt`

 * *Files identical despite different names*

