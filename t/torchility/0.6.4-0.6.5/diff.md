# Comparing `tmp/torchility-0.6.4.tar.gz` & `tmp/torchility-0.6.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "torchility-0.6.4.tar", last modified: Wed Mar 29 01:16:43 2023, max compression
+gzip compressed data, was "torchility-0.6.5.tar", last modified: Fri May  5 12:14:22 2023, max compression
```

## Comparing `torchility-0.6.4.tar` & `torchility-0.6.5.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 liuchen    (501) staff       (20)        0 2023-03-29 01:16:43.289930 torchility-0.6.4/
--rw-r--r--   0 liuchen    (501) staff       (20)     1073 2020-01-28 04:19:18.000000 torchility-0.6.4/LICENSE
--rw-r--r--   0 liuchen    (501) staff       (20)     2074 2023-03-29 01:16:43.289348 torchility-0.6.4/PKG-INFO
--rw-r--r--   0 liuchen    (501) staff       (20)     1595 2023-03-20 06:35:45.000000 torchility-0.6.4/README.md
-drwxr-xr-x   0 liuchen    (501) staff       (20)        0 2023-03-29 01:16:43.274587 torchility-0.6.4/examples/
--rw-r--r--   0 liuchen    (501) staff       (20)     1675 2023-03-27 12:31:34.000000 torchility-0.6.4/examples/1-mnist.py
--rw-r--r--   0 liuchen    (501) staff       (20)     2663 2023-03-28 13:54:47.000000 torchility-0.6.4/examples/2-mnist_callbacks.py
--rw-r--r--   0 liuchen    (501) staff       (20)     2085 2022-12-14 13:51:17.000000 torchility-0.6.4/examples/3-mnist_interpreter.py
--rw-r--r--   0 liuchen    (501) staff       (20)     1709 2022-03-31 07:25:03.000000 torchility-0.6.4/examples/4-mnist_model_analysis.py
--rw-r--r--   0 liuchen    (501) staff       (20)     1419 2022-05-28 01:44:42.000000 torchility-0.6.4/examples/5-mnist_lr_find.py
--rw-r--r--   0 liuchen    (501) staff       (20)     1962 2022-12-09 04:27:52.000000 torchility-0.6.4/examples/6-graph_node_clasification_DGL.py
--rw-r--r--   0 liuchen    (501) staff       (20)       38 2023-03-29 01:16:43.290287 torchility-0.6.4/setup.cfg
--rw-r--r--   0 liuchen    (501) staff       (20)     1117 2023-03-29 01:16:12.000000 torchility-0.6.4/setup.py
-drwxr-xr-x   0 liuchen    (501) staff       (20)        0 2023-03-29 01:16:43.278895 torchility-0.6.4/torchility/
--rw-r--r--   0 liuchen    (501) staff       (20)      503 2023-03-29 01:15:54.000000 torchility-0.6.4/torchility/__init__.py
-drwxr-xr-x   0 liuchen    (501) staff       (20)        0 2023-03-29 01:16:43.284513 torchility-0.6.4/torchility/callbacks/
--rw-r--r--   0 liuchen    (501) staff       (20)      101 2022-05-08 12:50:22.000000 torchility-0.6.4/torchility/callbacks/__init__.py
--rw-r--r--   0 liuchen    (501) staff       (20)     1153 2023-03-28 13:49:32.000000 torchility-0.6.4/torchility/callbacks/common.py
--rw-r--r--   0 liuchen    (501) staff       (20)     5169 2023-03-19 08:28:50.000000 torchility-0.6.4/torchility/callbacks/interpreters.py
--rw-r--r--   0 liuchen    (501) staff       (20)     3036 2023-03-19 07:43:59.000000 torchility-0.6.4/torchility/callbacks/performances.py
--rw-r--r--   0 liuchen    (501) staff       (20)    10012 2023-03-19 09:26:35.000000 torchility-0.6.4/torchility/callbacks/progress.py
--rw-r--r--   0 liuchen    (501) staff       (20)     2390 2021-06-09 14:49:55.000000 torchility-0.6.4/torchility/hooks.py
--rw-r--r--   0 liuchen    (501) staff       (20)      577 2021-06-10 07:05:35.000000 torchility-0.6.4/torchility/losses.py
--rw-r--r--   0 liuchen    (501) staff       (20)     4932 2023-03-28 13:36:07.000000 torchility-0.6.4/torchility/metrics.py
--rw-r--r--   0 liuchen    (501) staff       (20)     5971 2023-03-28 13:41:27.000000 torchility-0.6.4/torchility/tasks.py
--rw-r--r--   0 liuchen    (501) staff       (20)    11360 2023-03-28 13:33:59.000000 torchility-0.6.4/torchility/trainer.py
-drwxr-xr-x   0 liuchen    (501) staff       (20)        0 2023-03-29 01:16:43.288410 torchility-0.6.4/torchility/utils/
--rw-r--r--   0 liuchen    (501) staff       (20)       68 2022-06-01 16:09:54.000000 torchility-0.6.4/torchility/utils/__init__.py
--rw-r--r--   0 liuchen    (501) staff       (20)     4222 2022-06-02 14:28:56.000000 torchility-0.6.4/torchility/utils/plots.py
--rw-r--r--   0 liuchen    (501) staff       (20)     5587 2023-03-28 13:31:42.000000 torchility-0.6.4/torchility/utils/utils.py
--rw-r--r--   0 liuchen    (501) staff       (20)     3014 2022-08-04 03:32:03.000000 torchility-0.6.4/torchility/utils/yaml_config.py
-drwxr-xr-x   0 liuchen    (501) staff       (20)        0 2023-03-29 01:16:43.281765 torchility-0.6.4/torchility.egg-info/
--rw-r--r--   0 liuchen    (501) staff       (20)     2074 2023-03-29 01:16:42.000000 torchility-0.6.4/torchility.egg-info/PKG-INFO
--rw-r--r--   0 liuchen    (501) staff       (20)      795 2023-03-29 01:16:43.000000 torchility-0.6.4/torchility.egg-info/SOURCES.txt
--rw-r--r--   0 liuchen    (501) staff       (20)        1 2023-03-29 01:16:42.000000 torchility-0.6.4/torchility.egg-info/dependency_links.txt
--rw-r--r--   0 liuchen    (501) staff       (20)       83 2023-03-29 01:16:42.000000 torchility-0.6.4/torchility.egg-info/requires.txt
--rw-r--r--   0 liuchen    (501) staff       (20)       11 2023-03-29 01:16:42.000000 torchility-0.6.4/torchility.egg-info/top_level.txt
+drwxr-xr-x   0 liuchen    (501) staff       (20)        0 2023-05-05 12:14:22.410032 torchility-0.6.5/
+-rw-r--r--   0 liuchen    (501) staff       (20)     1073 2020-01-28 04:19:18.000000 torchility-0.6.5/LICENSE
+-rw-r--r--   0 liuchen    (501) staff       (20)     2074 2023-05-05 12:14:22.406164 torchility-0.6.5/PKG-INFO
+-rw-r--r--   0 liuchen    (501) staff       (20)     1595 2023-03-20 06:35:45.000000 torchility-0.6.5/README.md
+drwxr-xr-x   0 liuchen    (501) staff       (20)        0 2023-05-05 12:14:22.378023 torchility-0.6.5/examples/
+-rw-r--r--   0 liuchen    (501) staff       (20)     1675 2023-03-27 12:31:34.000000 torchility-0.6.5/examples/1-mnist.py
+-rw-r--r--   0 liuchen    (501) staff       (20)     2663 2023-03-28 13:54:47.000000 torchility-0.6.5/examples/2-mnist_callbacks.py
+-rw-r--r--   0 liuchen    (501) staff       (20)     2223 2023-05-05 12:11:38.000000 torchility-0.6.5/examples/3-mnist_interpreter.py
+-rw-r--r--   0 liuchen    (501) staff       (20)     1709 2022-03-31 07:25:03.000000 torchility-0.6.5/examples/4-mnist_model_analysis.py
+-rw-r--r--   0 liuchen    (501) staff       (20)     1419 2022-05-28 01:44:42.000000 torchility-0.6.5/examples/5-mnist_lr_find.py
+-rw-r--r--   0 liuchen    (501) staff       (20)     1962 2022-12-09 04:27:52.000000 torchility-0.6.5/examples/6-graph_node_clasification_DGL.py
+-rw-r--r--   0 liuchen    (501) staff       (20)       38 2023-05-05 12:14:22.410206 torchility-0.6.5/setup.cfg
+-rw-r--r--   0 liuchen    (501) staff       (20)     1117 2023-05-05 12:13:44.000000 torchility-0.6.5/setup.py
+drwxr-xr-x   0 liuchen    (501) staff       (20)        0 2023-05-05 12:14:22.389026 torchility-0.6.5/torchility/
+-rw-r--r--   0 liuchen    (501) staff       (20)      503 2023-05-05 12:14:06.000000 torchility-0.6.5/torchility/__init__.py
+drwxr-xr-x   0 liuchen    (501) staff       (20)        0 2023-05-05 12:14:22.399275 torchility-0.6.5/torchility/callbacks/
+-rw-r--r--   0 liuchen    (501) staff       (20)      101 2022-05-08 12:50:22.000000 torchility-0.6.5/torchility/callbacks/__init__.py
+-rw-r--r--   0 liuchen    (501) staff       (20)     1153 2023-03-28 13:49:32.000000 torchility-0.6.5/torchility/callbacks/common.py
+-rw-r--r--   0 liuchen    (501) staff       (20)     4730 2023-05-05 12:09:25.000000 torchility-0.6.5/torchility/callbacks/interpreters.py
+-rw-r--r--   0 liuchen    (501) staff       (20)     3036 2023-03-19 07:43:59.000000 torchility-0.6.5/torchility/callbacks/performances.py
+-rw-r--r--   0 liuchen    (501) staff       (20)    10012 2023-03-19 09:26:35.000000 torchility-0.6.5/torchility/callbacks/progress.py
+-rw-r--r--   0 liuchen    (501) staff       (20)     2390 2021-06-09 14:49:55.000000 torchility-0.6.5/torchility/hooks.py
+-rw-r--r--   0 liuchen    (501) staff       (20)      577 2021-06-10 07:05:35.000000 torchility-0.6.5/torchility/losses.py
+-rw-r--r--   0 liuchen    (501) staff       (20)     4932 2023-03-28 13:36:07.000000 torchility-0.6.5/torchility/metrics.py
+-rw-r--r--   0 liuchen    (501) staff       (20)     5971 2023-03-28 13:41:27.000000 torchility-0.6.5/torchility/tasks.py
+-rw-r--r--   0 liuchen    (501) staff       (20)    11360 2023-03-28 13:33:59.000000 torchility-0.6.5/torchility/trainer.py
+drwxr-xr-x   0 liuchen    (501) staff       (20)        0 2023-05-05 12:14:22.403051 torchility-0.6.5/torchility/utils/
+-rw-r--r--   0 liuchen    (501) staff       (20)       68 2022-06-01 16:09:54.000000 torchility-0.6.5/torchility/utils/__init__.py
+-rw-r--r--   0 liuchen    (501) staff       (20)     4222 2022-06-02 14:28:56.000000 torchility-0.6.5/torchility/utils/plots.py
+-rw-r--r--   0 liuchen    (501) staff       (20)     6050 2023-05-05 01:14:22.000000 torchility-0.6.5/torchility/utils/utils.py
+-rw-r--r--   0 liuchen    (501) staff       (20)     3014 2022-08-04 03:32:03.000000 torchility-0.6.5/torchility/utils/yaml_config.py
+drwxr-xr-x   0 liuchen    (501) staff       (20)        0 2023-05-05 12:14:22.394754 torchility-0.6.5/torchility.egg-info/
+-rw-r--r--   0 liuchen    (501) staff       (20)     2074 2023-05-05 12:14:22.000000 torchility-0.6.5/torchility.egg-info/PKG-INFO
+-rw-r--r--   0 liuchen    (501) staff       (20)      795 2023-05-05 12:14:22.000000 torchility-0.6.5/torchility.egg-info/SOURCES.txt
+-rw-r--r--   0 liuchen    (501) staff       (20)        1 2023-05-05 12:14:22.000000 torchility-0.6.5/torchility.egg-info/dependency_links.txt
+-rw-r--r--   0 liuchen    (501) staff       (20)       83 2023-05-05 12:14:22.000000 torchility-0.6.5/torchility.egg-info/requires.txt
+-rw-r--r--   0 liuchen    (501) staff       (20)       11 2023-05-05 12:14:22.000000 torchility-0.6.5/torchility.egg-info/top_level.txt
```

### Comparing `torchility-0.6.4/LICENSE` & `torchility-0.6.5/LICENSE`

 * *Files identical despite different names*

### Comparing `torchility-0.6.4/PKG-INFO` & `torchility-0.6.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: torchility
-Version: 0.6.4
+Version: 0.6.5
 Summary: UNKNOWN
 Home-page: https://github.com/hitlic/torchility
 Author: hitlic
 Author-email: liuchen.lic@gmail.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `torchility-0.6.4/README.md` & `torchility-0.6.5/README.md`

 * *Files identical despite different names*

### Comparing `torchility-0.6.4/examples/1-mnist.py` & `torchility-0.6.5/examples/1-mnist.py`

 * *Files identical despite different names*

### Comparing `torchility-0.6.4/examples/2-mnist_callbacks.py` & `torchility-0.6.5/examples/2-mnist_callbacks.py`

 * *Files identical despite different names*

### Comparing `torchility-0.6.4/examples/3-mnist_interpreter.py` & `torchility-0.6.5/examples/3-mnist_interpreter.py`

 * *Files 16% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 import matplotlib.pyplot as plt
 import warnings
 warnings.simplefilter("ignore")
 
 
 # 1. --- 数据
 data_dir = './datasets'
-transform = transforms.Compose([transforms.ToTensor(), transforms.Normalize((0.1307,), (0.3081,))])
+transform = transforms.Compose([transforms.ToTensor()])
 mnist_full = MNIST(data_dir, train=True, transform=transform, download=True)
 train_ds, val_ds = random_split(mnist_full, [55000, 5000])
 test_ds = MNIST(data_dir, train=False, transform=transform, download=True)
 train_dl = DataLoader(train_ds, batch_size=32)
 val_dl = DataLoader(val_ds, batch_size=32)
 test_dl = DataLoader(test_ds, batch_size=32)
 
@@ -37,21 +37,36 @@
 
 
 # 3. --- 优化器
 opt = torch.optim.Adam(model.parameters(), lr=2e-4)
 
 
 # 4. --- 训练
-interpreter = ClassifierInterpreter(class_num=10, stage='test')          # 针对分类模型测试数据的解释器
+
+# 要计算每个样本的指标，因此不能reduction（即求和、平均等操作）
+metric = nn.CrossEntropyLoss(reduction='none')
+
+interpreter = ClassifierInterpreter(metric=metric, k=15, class_num=10, stage='test')          # 针对分类模型测试数据的解释器
 trainer = Trainer(model, F.cross_entropy, opt,                           # 训练器
-                  epochs=2, callbacks=[interpreter]) 
+                  epochs=5, callbacks=[interpreter])
 trainer.fit(train_dl, val_dl)                                            # 训练、验证
 trainer.test(test_dl)                                                    # 测试
 
 
 # 5. --- 解释
-# 返回测试集中损失最大的10个样本的信息
-metric = nn.CrossEntropyLoss(reduction='none')  # 要计算每个样本的指标，因此不能reduction（即求和、平均等操作）
-tops = trainer.interpreter.top_samples(metric, k=10)                     # 返回metric值最大的10个样本的信息
-print(tops)
-trainer.interpreter.plot_confusion()                                     # 绘制混淆矩阵
+
+# 返回测试集中损失最大的k个样本的信息
+tops = trainer.interpreter.top_samples()
+
+# 绘制损失最大的k个样本
+plt.figure(figsize=[10, 6])
+for i, sample in enumerate(tops):
+    loss, pred, target, x = sample
+    plt.subplot(3, 5, i+1)
+    plt.imshow(sample[3][0])
+    plt.title(f'{sample[0]:.3},  {target}->{pred.argmax()}')
+    plt.xticks([])
+    plt.yticks([])
+
+# 绘制混淆矩阵
+trainer.interpreter.plot_confusion()
 plt.show()
```

### Comparing `torchility-0.6.4/examples/4-mnist_model_analysis.py` & `torchility-0.6.5/examples/4-mnist_model_analysis.py`

 * *Files identical despite different names*

### Comparing `torchility-0.6.4/examples/5-mnist_lr_find.py` & `torchility-0.6.5/examples/5-mnist_lr_find.py`

 * *Files identical despite different names*

### Comparing `torchility-0.6.4/examples/6-graph_node_clasification_DGL.py` & `torchility-0.6.5/examples/6-graph_node_clasification_DGL.py`

 * *Files identical despite different names*

### Comparing `torchility-0.6.4/setup.py` & `torchility-0.6.5/setup.py`

 * *Files identical despite different names*

### Comparing `torchility-0.6.4/torchility/callbacks/common.py` & `torchility-0.6.5/torchility/callbacks/common.py`

 * *Files identical despite different names*

### Comparing `torchility-0.6.4/torchility/callbacks/interpreters.py` & `torchility-0.6.5/torchility/callbacks/interpreters.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,124 +1,115 @@
+from typing import Any, Optional
+import pytorch_lightning as pl
 from pytorch_lightning.callbacks.callback import Callback
+from pytorch_lightning.utilities.types import STEP_OUTPUT
 from torchmetrics.classification import BinaryConfusionMatrix, MulticlassConfusionMatrix
 from itertools import chain
 import torch
-from ..utils import plot_confusion
+from ..utils import plot_confusion, TopKQueue
 
 
-class BatchRecorder(Callback):
-    def __init__(self, stage='test'):
+class Interpreter(Callback):
+    def __init__(self, metric=None, k=100, mode='max', stage='test'):
+        """
+        Args:
+            metric: none reducted callable
+            k: number of samples to keep
+            mode: 'max' or 'min'
+            stage: 'train', 'val' or 'test'
+        """
         super().__init__()
+        assert mode in ['min', 'max']
         assert stage in ['train', 'val', 'test']
+        self.metric = metric
         self.stage = stage
+        self.mode = mode
+        self.batch_recorder = []
+        self.top_queue = TopKQueue(k=k)
+
+    def on_fit_start(self, trainer, pl_module):
+        trainer.interpreter = self
+        pl_module.interpreter = self
 
     def on_train_epoch_start(self, trainer, pl_module):
-        self.recorder = []
+        self.batch_recorder = []
 
     def on_validation_epoch_start(self, trainer, pl_module):
-        self.recorder = []
+        self.batch_recorder = []
 
     def on_test_epoch_start(self, trainer, pl_module):
-        self.recorder = []
+        self.batch_recorder = []
 
     def on_train_batch_end(self, trainer, pl_module, outputs, batch, batch_idx):
         if self.stage == 'train':
-            self.recorder.append(pl_module.messages['train_batch'])
+            self.batch_recorder.append(pl_module.messages['train_batch'])
+            _, preds, targets = pl_module.messages['train_batch']
+            self.put_queue(preds, targets, batch[0])
 
-    def on_validation_batch_end(self, trainer: "pl.Trainer",
-                                pl_module: "pl.LightningModule",
-                                outputs,
-                                batch,
-                                batch_idx: int,
-                                dataloader_idx: int = 0):
+    def on_validation_batch_end(self, trainer, pl_module, outputs, batch, batch_idx):
         if self.stage == 'val':
-            self.recorder.append(pl_module.messages['val_batch'])
-        return super().on_validation_batch_end(trainer, pl_module, outputs, batch, batch_idx, dataloader_idx)
+            self.batch_recorder.append(pl_module.messages['val_batch'])
+            _, preds, targets = pl_module.messages['val_batch']
+            self.put_queue(preds, targets, batch[0])
 
-    def on_test_batch_end(self, trainer: "pl.Trainer",
-                          pl_module: "pl.LightningModule",
-                          outputs,
-                          batch,
-                          batch_idx: int,
-                          dataloader_idx: int = 0):
+    def on_test_batch_end(self, trainer, pl_module, outputs, batch, batch_idx):
         if self.stage == 'test':
-            self.recorder.append(pl_module.messages['test_batch'])
-        return super().on_test_batch_end(trainer, pl_module, outputs, batch, batch_idx, dataloader_idx)
-
+            self.batch_recorder.append(pl_module.messages['test_batch'])
+            _, preds, targets = pl_module.messages['test_batch']
+            self.put_queue(preds, targets, batch[0])
+
+    def put_queue(self, preds, targets, inputs):
+        if self.metric is None:
+            return
+        batch_m = self.metric(preds, targets)
+        assert batch_m.shape[0] == preds.shape[0], 'The `metric` must not be reduced!'
+        for m, pred, target, x in zip(batch_m.cpu(), preds.cpu(), targets.cpu(), inputs.cpu()):
+            v = -m if self.mode == 'min' else m
+            self.top_queue.put((v.item(), [m.item(), pred.detach().numpy(), target.detach().numpy(), x.detach().numpy()]))
 
-class Interpreter(BatchRecorder):
-    def on_fit_start(self, trainer, pl_module):
-        trainer.interpreter = self
-        pl_module.interpreter = self
-
-    def top_samples(self, metric, k=0, largest=True):
+    def top_samples(self):
         """
-        返回metric指标最大（largest=True）或最小（largest=False）的k个样本数据的信息。
-        Args:
-            metric: metric对于每个样本应当只输出一个数值。
-            larges: 排序方式
-            k: 返回数量
-        Return: [(batch_id, sample_id_within_batch), metric_value, pred, target), ... ]
-        """
-        # 检验 metric 是否正确
-        _, preds, targets = self.recorder[0]
-        values = metric(preds, targets)
-        assert values.size()[0] == preds.size()[0], 'The output of `metric` must not be reduced!'
-
-        info_batchs = []
-        with torch.no_grad():
-            for batch_id, preds, targets in self.recorder:
-                values = metric(preds, targets).flatten().detach().cpu()
-                ids = [(batch_id, i) for i in range(values.size()[0])]
-                info_batchs.append((ids, values, preds, targets))
-        sample_ids = chain(*[e[0] for e in info_batchs])
-        sample_values = torch.cat([e[1] for e in info_batchs]).numpy()
-        sample_preds = torch.cat([e[2] for e in info_batchs]).numpy()
-        sample_targets = torch.cat([e[3] for e in info_batchs]).numpy()
-        sample_infos = zip(sample_ids, sample_values, sample_preds, sample_targets)
-        sorted_samples = sorted(sample_infos, key=lambda e: e[1], reverse=largest)
-        if k > 0:
-            sorted_samples = sorted_samples[:k]
-        return sorted_samples
+        Return: [metric_value, pred, target, input_feat] of top k samples 
+        """
+        samples = [item[1] for item in self.top_queue.items()]
+        return samples
+
+    def top(self):
+        return self.top_samples()
 
 
 class ClassifierInterpreter(Interpreter):
     """
     分类模型的解释器
     """
-    def __init__(self, class_num, binary=False, normalize=False, stage='test', threshold=0.5):
+    def __init__(self, class_num, binary=False, normalize=False, metric=None, k=0, mode='max', stage='test', threshold=0.5):
         """
         class_num: number of class.
         binary: True of False
         normalize: normalize or not
+        metric: none reducted callable
+        k: number of samples
+        mode: 'max' or 'min'
         stage: 'train', 'val' or 'test'
         threshold: threshold of classification
         """
-        super().__init__(stage=stage)
+        super().__init__(metric, k=k, mode=mode, stage=stage)
         if binary:
             assert class_num == 2, "class_mnum must be 2 for binary classification!"
         norm = 'true' if normalize else 'none'
         if binary:
             self.conf_mat = BinaryConfusionMatrix(normalize=norm, threshold=threshold)
         else:
             self.conf_mat = MulticlassConfusionMatrix(class_num, normalize=norm, threshold=threshold)
         self.class_num = class_num
         self.normalize = normalize
 
     def confusion_matrix(self, argmax_pred=False, argmax_target=False):
-        for _, preds, targets in self.recorder:
+        for _, preds, targets in self.batch_recorder:
             b_preds = preds.argmax(dim=1) if argmax_pred else preds
             b_targets = targets.argmax(dim=1) if argmax_target else targets
             self.conf_mat.update(b_preds.cpu(), b_targets.cpu())
         return self.conf_mat.compute().detach().numpy()
 
     def plot_confusion(self, class_names=None, cmap='Blues', title_info='', argmax_pred=False, argmax_target=False):
         c_matrix = self.confusion_matrix(argmax_pred, argmax_target)
         return plot_confusion(c_matrix, self.class_num, class_names, self.normalize, cmap=cmap, info=title_info)
-
-
-class RegressorInterpreter(Interpreter):
-    """
-    回归模型解释器
-    """
-    # TODO
-    pass
```

### Comparing `torchility-0.6.4/torchility/callbacks/performances.py` & `torchility-0.6.5/torchility/callbacks/performances.py`

 * *Files identical despite different names*

### Comparing `torchility-0.6.4/torchility/callbacks/progress.py` & `torchility-0.6.5/torchility/callbacks/progress.py`

 * *Files identical despite different names*

### Comparing `torchility-0.6.4/torchility/hooks.py` & `torchility-0.6.5/torchility/hooks.py`

 * *Files identical despite different names*

### Comparing `torchility-0.6.4/torchility/losses.py` & `torchility-0.6.5/torchility/losses.py`

 * *Files identical despite different names*

### Comparing `torchility-0.6.4/torchility/metrics.py` & `torchility-0.6.5/torchility/metrics.py`

 * *Files identical despite different names*

### Comparing `torchility-0.6.4/torchility/tasks.py` & `torchility-0.6.5/torchility/tasks.py`

 * *Files identical despite different names*

### Comparing `torchility-0.6.4/torchility/trainer.py` & `torchility-0.6.5/torchility/trainer.py`

 * *Files identical despite different names*

### Comparing `torchility-0.6.4/torchility/utils/plots.py` & `torchility-0.6.5/torchility/utils/plots.py`

 * *Files identical despite different names*

### Comparing `torchility-0.6.4/torchility/utils/utils.py` & `torchility-0.6.5/torchility/utils/utils.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,33 @@
 from typing import Iterable
 import numpy as np
 import itertools
 import torch
 from matplotlib import pyplot as plt
 from matplotlib.pyplot import MultipleLocator
+from queue import PriorityQueue
+
+
+class TopKQueue(PriorityQueue):
+    """
+    能够保存最大值的优先队列
+    """
+    def __init__(self, k: int = 0):
+        super().__init__(maxsize=k)
+
+    def put(self, e):
+        if self.full():
+            if e[0] > self.queue[0][0]:
+                self.get()
+            else:
+                return
+        super().put(e)
+
+    def items(self):
+        return sorted(self.queue, key=lambda e: e[0], reverse=True)
 
 
 def batches(inputs, batch_size):
     """
     把inputs按batch_size进行划分
     """
     is_list_input = isinstance(inputs, (list, tuple))  # inputs是否是多个输入组成的列表或元素
```

### Comparing `torchility-0.6.4/torchility/utils/yaml_config.py` & `torchility-0.6.5/torchility/utils/yaml_config.py`

 * *Files identical despite different names*

### Comparing `torchility-0.6.4/torchility.egg-info/PKG-INFO` & `torchility-0.6.5/torchility.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: torchility
-Version: 0.6.4
+Version: 0.6.5
 Summary: UNKNOWN
 Home-page: https://github.com/hitlic/torchility
 Author: hitlic
 Author-email: liuchen.lic@gmail.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `torchility-0.6.4/torchility.egg-info/SOURCES.txt` & `torchility-0.6.5/torchility.egg-info/SOURCES.txt`

 * *Files identical despite different names*

