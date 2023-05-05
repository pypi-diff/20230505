# Comparing `tmp/torch4keras-0.0.6.tar.gz` & `tmp/torch4keras-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "torch4keras-0.0.6.tar", last modified: Sun Feb 12 15:21:59 2023, max compression
+gzip compressed data, was "torch4keras-0.0.7.tar", last modified: Fri May  5 14:04:39 2023, max compression
```

## Comparing `torch4keras-0.0.6.tar` & `torch4keras-0.0.7.tar`

### file list

```diff
@@ -1,15 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-02-12 15:21:59.208642 torch4keras-0.0.6/
--rw-rw-rw-   0        0        0    11558 2022-10-19 12:34:20.000000 torch4keras-0.0.6/LICENSE
--rw-rw-rw-   0        0        0     5834 2023-02-12 15:21:59.207641 torch4keras-0.0.6/PKG-INFO
--rw-rw-rw-   0        0        0     5580 2023-02-11 12:29:12.000000 torch4keras-0.0.6/README.md
--rw-rw-rw-   0        0        0       42 2023-02-12 15:21:59.208642 torch4keras-0.0.6/setup.cfg
--rw-rw-rw-   0        0        0      521 2023-02-12 15:21:24.000000 torch4keras-0.0.6/setup.py
-drwxrwxrwx   0        0        0        0 2023-02-12 15:21:59.193640 torch4keras-0.0.6/torch4keras/
--rw-rw-rw-   0        0        0        0 2022-10-21 12:52:53.000000 torch4keras-0.0.6/torch4keras/__init__.py
--rw-rw-rw-   0        0        0    21074 2023-02-11 12:22:50.000000 torch4keras-0.0.6/torch4keras/model.py
--rw-rw-rw-   0        0        0    49875 2023-02-11 15:34:14.000000 torch4keras-0.0.6/torch4keras/snippets.py
-drwxrwxrwx   0        0        0        0 2023-02-12 15:21:59.206640 torch4keras-0.0.6/torch4keras.egg-info/
--rw-rw-rw-   0        0        0     5834 2023-02-12 15:21:58.000000 torch4keras-0.0.6/torch4keras.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      235 2023-02-12 15:21:58.000000 torch4keras-0.0.6/torch4keras.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-02-12 15:21:58.000000 torch4keras-0.0.6/torch4keras.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       12 2023-02-12 15:21:58.000000 torch4keras-0.0.6/torch4keras.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-05 14:04:39.916319 torch4keras-0.0.7/
+-rw-rw-rw-   0        0        0    11558 2022-10-19 12:34:20.000000 torch4keras-0.0.7/LICENSE
+-rw-rw-rw-   0        0        0     6453 2023-05-05 14:04:39.915318 torch4keras-0.0.7/PKG-INFO
+-rw-rw-rw-   0        0        0     6199 2023-05-05 13:57:27.000000 torch4keras-0.0.7/README.md
+-rw-rw-rw-   0        0        0       42 2023-05-05 14:04:39.916319 torch4keras-0.0.7/setup.cfg
+-rw-rw-rw-   0        0        0      521 2023-04-24 15:56:30.000000 torch4keras-0.0.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-05 14:04:39.896319 torch4keras-0.0.7/torch4keras/
+-rw-rw-rw-   0        0        0        0 2022-10-21 12:52:53.000000 torch4keras-0.0.7/torch4keras/__init__.py
+-rw-rw-rw-   0        0        0    42265 2023-04-24 15:56:30.000000 torch4keras-0.0.7/torch4keras/callbacks.py
+-rw-rw-rw-   0        0        0    22581 2023-05-03 05:20:41.000000 torch4keras-0.0.7/torch4keras/model.py
+-rw-rw-rw-   0        0        0     8167 2023-04-24 15:56:30.000000 torch4keras-0.0.7/torch4keras/snippets.py
+drwxrwxrwx   0        0        0        0 2023-05-05 14:04:39.914316 torch4keras-0.0.7/torch4keras.egg-info/
+-rw-rw-rw-   0        0        0     6453 2023-05-05 14:04:39.000000 torch4keras-0.0.7/torch4keras.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      260 2023-05-05 14:04:39.000000 torch4keras-0.0.7/torch4keras.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-05 14:04:39.000000 torch4keras-0.0.7/torch4keras.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       12 2023-05-05 14:04:39.000000 torch4keras-0.0.7/torch4keras.egg-info/top_level.txt
```

### Comparing `torch4keras-0.0.6/LICENSE` & `torch4keras-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `torch4keras-0.0.6/PKG-INFO` & `torch4keras-0.0.7/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: torch4keras
-Version: 0.0.6
+Version: 0.0.7
 Summary: Use torch like keras
 Home-page: https://github.com/Tongjilibo/torch4keras
 Author: Tongjilibo
 License: Apache License
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
@@ -26,15 +26,15 @@
 ## 1. 下载安装
 安装稳定版
 ```shell
 pip install torch4keras
 ```
 安装最新版
 ```shell
-pip install git+https://www.github.com/Tongjilibo/torch4keras.git
+pip install git+https://github.com/Tongjilibo/torch4keras.git
 ```
 
 ## 2. 功能
 - 简述：抽象出来的Trainer，适用于一般神经网络的训练，仅需关注网络结构代码
 - 特色：进度条展示训练过程，自定义metric，自带Evaluator, Checkpoint, Tensorboard, Logger等Callback，也可自定义Callback
 - 初衷：前期功能是作为[bert4torch](https://github.com/Tongjilibo/bert4torch)和[rec4torch](https://github.com/Tongjilibo/rec4torch)的Trainer
 - 训练：
@@ -70,24 +70,27 @@
     ```
 
 ## 3. 快速上手
 - 参考[bert4torch](https://github.com/Tongjilibo/bert4torch)的训练过程
 - 简单示例: [turorials_mnist](https://github.com/Tongjilibo/torch4keras/blob/master/examples/turorials_mnist.py)
 
 ## 4. 版本说明
+- **v0.0.7**：20230505 独立出callbacks.py文件, fit允许输入形式为字典，load_weights支持list输入，save_weights支持仅保存可训练参数
+- **v0.0.6**：20230212 增加resume_from_checkpoint和save_to_checkpoint；增加add_trainer方法，重构了Trainer(BaseModel)的实现(增加几个成员变量、增加initilize()、删除对forward参数个数的判断、dp和ddp不解析module、修改use_amp参数为mixed_precision)，增加了AccelerateCallback
 - **v0.0.5**：20221217 增加Summary的Callback, 增加Tqdm的进度条展示，保留原有BaseModel的同时，增加Trainer(不从nn.Module继承), 从bert4torch的snippets迁移部分通用函数
 - **v0.0.4**：20221127 为callback增加on_train_step_end方法, 修复BaseModel(net)方式的bug
 - **v0.0.3.post2**：20221107 修复DDP下打印的bug
 - **v0.0.3**：20221106 参考Keras修改了callback的逻辑
 - **v0.0.2**：20221023 增加Checkpoint, Evaluator等自带Callback, 修改BaseModel(net)方式，修复DP和DDP的__init__()
 - **v0.0.1**：20221019 初始版本
 
 ## 5. 更新：
-- **20230207**：增加hf的accelerator测试用例, ddp需要外部控制执行callback, 混合精度支持bf16, 增加add_trainer方法
-- **20230116**：增加resume_from_checkpoint和save_to_checkpoint，动态为nn.Module增加Trainer的方法
+- **20230505**：独立出callbacks.py文件, fit允许输入形式为字典，load_weights支持list输入，save_weights支持仅保存可训练参数
+- **20230212**：增加hf的accelerator测试用例, ddp需要外部控制执行callback, 混合精度支持bf16
+- **20230116**：增加resume_from_checkpoint和save_to_checkpoint，动态为nn.Module增加Trainer的方法add_trainer
 - **20221217**：保留原有BaseModel的同时，增加Trainer(不从nn.Module继承), 从bert4torch的snippets迁移部分通用函数
 - **20221203**：增加Summary的Callback, 增加Tqdm的进度条展示
 - **20221127**：为callback增加on_train_step_end方法, 修复BaseModel(net)方式的bug
 - **20221107**：修复DDP下打印的bug，metrics中加入detach和auc
 - **20221106**：默认的Tensorboard的global_step+1, 参考Keras修改了callback的逻辑
 - **20221020**：增加Checkpoint, Evaluator等自带Callback, 修改BaseModel(net)方式，修复DP和DDP的__init__()
 - **20221019**：初版提交
```

### Comparing `torch4keras-0.0.6/README.md` & `torch4keras-0.0.7/torch4keras.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,7 +1,17 @@
+Metadata-Version: 2.1
+Name: torch4keras
+Version: 0.0.7
+Summary: Use torch like keras
+Home-page: https://github.com/Tongjilibo/torch4keras
+Author: Tongjilibo
+License: Apache License
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # torch4keras
 **Use torch like keras**
 
 [![licence](https://img.shields.io/github/license/Tongjilibo/torch4keras.svg?maxAge=3600)](https://github.com/Tongjilibo/torch4keras/blob/master/LICENSE) 
 [![GitHub release](https://img.shields.io/github/release/Tongjilibo/torch4keras.svg?maxAge=3600)](https://github.com/Tongjilibo/torch4keras/releases) 
 [![PyPI](https://img.shields.io/pypi/v/torch4keras?label=pypi%20package)](https://pypi.org/project/torch4keras/) 
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/torch4keras)](https://pypistats.org/packages/torch4keras)
@@ -16,15 +26,15 @@
 ## 1. 下载安装
 安装稳定版
 ```shell
 pip install torch4keras
 ```
 安装最新版
 ```shell
-pip install git+https://www.github.com/Tongjilibo/torch4keras.git
+pip install git+https://github.com/Tongjilibo/torch4keras.git
 ```
 
 ## 2. 功能
 - 简述：抽象出来的Trainer，适用于一般神经网络的训练，仅需关注网络结构代码
 - 特色：进度条展示训练过程，自定义metric，自带Evaluator, Checkpoint, Tensorboard, Logger等Callback，也可自定义Callback
 - 初衷：前期功能是作为[bert4torch](https://github.com/Tongjilibo/bert4torch)和[rec4torch](https://github.com/Tongjilibo/rec4torch)的Trainer
 - 训练：
@@ -60,24 +70,27 @@
     ```
 
 ## 3. 快速上手
 - 参考[bert4torch](https://github.com/Tongjilibo/bert4torch)的训练过程
 - 简单示例: [turorials_mnist](https://github.com/Tongjilibo/torch4keras/blob/master/examples/turorials_mnist.py)
 
 ## 4. 版本说明
+- **v0.0.7**：20230505 独立出callbacks.py文件, fit允许输入形式为字典，load_weights支持list输入，save_weights支持仅保存可训练参数
+- **v0.0.6**：20230212 增加resume_from_checkpoint和save_to_checkpoint；增加add_trainer方法，重构了Trainer(BaseModel)的实现(增加几个成员变量、增加initilize()、删除对forward参数个数的判断、dp和ddp不解析module、修改use_amp参数为mixed_precision)，增加了AccelerateCallback
 - **v0.0.5**：20221217 增加Summary的Callback, 增加Tqdm的进度条展示，保留原有BaseModel的同时，增加Trainer(不从nn.Module继承), 从bert4torch的snippets迁移部分通用函数
 - **v0.0.4**：20221127 为callback增加on_train_step_end方法, 修复BaseModel(net)方式的bug
 - **v0.0.3.post2**：20221107 修复DDP下打印的bug
 - **v0.0.3**：20221106 参考Keras修改了callback的逻辑
 - **v0.0.2**：20221023 增加Checkpoint, Evaluator等自带Callback, 修改BaseModel(net)方式，修复DP和DDP的__init__()
 - **v0.0.1**：20221019 初始版本
 
 ## 5. 更新：
-- **20230207**：增加hf的accelerator测试用例, ddp需要外部控制执行callback, 混合精度支持bf16, 增加add_trainer方法
-- **20230116**：增加resume_from_checkpoint和save_to_checkpoint，动态为nn.Module增加Trainer的方法
+- **20230505**：独立出callbacks.py文件, fit允许输入形式为字典，load_weights支持list输入，save_weights支持仅保存可训练参数
+- **20230212**：增加hf的accelerator测试用例, ddp需要外部控制执行callback, 混合精度支持bf16
+- **20230116**：增加resume_from_checkpoint和save_to_checkpoint，动态为nn.Module增加Trainer的方法add_trainer
 - **20221217**：保留原有BaseModel的同时，增加Trainer(不从nn.Module继承), 从bert4torch的snippets迁移部分通用函数
 - **20221203**：增加Summary的Callback, 增加Tqdm的进度条展示
 - **20221127**：为callback增加on_train_step_end方法, 修复BaseModel(net)方式的bug
 - **20221107**：修复DDP下打印的bug，metrics中加入detach和auc
 - **20221106**：默认的Tensorboard的global_step+1, 参考Keras修改了callback的逻辑
 - **20221020**：增加Checkpoint, Evaluator等自带Callback, 修改BaseModel(net)方式，修复DP和DDP的__init__()
 - **20221019**：初版提交
```

### Comparing `torch4keras-0.0.6/setup.py` & `torch4keras-0.0.7/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from setuptools import setup, find_packages
 
 with open("README.md", "r", encoding='utf-8') as fh:
     long_description = fh.read()
 
 setup(
     name='torch4keras',
-    version='0.0.6',
+    version='0.0.7',
     description='Use torch like keras',
     long_description=long_description,
     long_description_content_type="text/markdown",
     license='Apache License',
     url='https://github.com/Tongjilibo/torch4keras',
     author='Tongjilibo',
     install_requires=[],
```

### Comparing `torch4keras-0.0.6/torch4keras/model.py` & `torch4keras-0.0.7/torch4keras/model.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from torch import nn
 import torch
-from torch4keras.snippets import metric_mapping, ProgbarLogger, Callback, CallbackList, BaseLogger, History, TqdmProgressBar
+from torch4keras.snippets import metric_mapping
+from torch4keras.callbacks import ProgbarLogger, Callback, CallbackList, BaseLogger, History, TqdmProgressBar
 from collections import OrderedDict
 from inspect import isfunction
 import os
 
 
 class Trainer:
     """Trainer, 传入Module实例
@@ -83,15 +84,20 @@
         self.tqdmbar = kwargs.get('tqdmbar', False)
     
     def _forward(self, train_X):
         # 如果传入了网络结构module，则调用module的forward
         # 如果是继承方式，则调用自身的forward
         if isinstance(train_X, torch.Tensor):  # tensor不展开
             return self.get_module().forward(train_X)
-        return self.get_module().forward(*train_X)
+        elif isinstance(train_X, (tuple, list)):
+            return self.get_module().forward(*train_X)
+        elif isinstance(train_X, dict):
+            return self.get_module().forward(**train_X)
+        else:
+            return self.get_module().forward(train_X)
 
     def train_step(self, train_X, train_y):
         '''forward并返回loss
 
         :param train_X: List[torch.Tensor], 训练数据
         :param train_y: torch.Tensor/List[torch.Tensor], 标签信息
         :return: [output, loss, loss_detail] output: torch.Tensor/List[torch.Tensor], 模型输出; loss: nn.Tensor, 计算得到的loss; loss_detail: dict[nn.Tensor], 具体的各个loss
@@ -150,15 +156,15 @@
         self.train_dataloader = train_dataloader  # 设置为成员变量，可由外部的callbacks进行修改
         train_dataloader_iter = iter(self.train_dataloader)  # 循环epoch时不重生成
         verbose = self.verbose if hasattr(self, 'verbose') else verbose
 
         # callbacks设置
         if callbacks is None:
             callbacks = []
-        if not isinstance(callbacks, (list, tuple)):
+        elif isinstance(callbacks, Callback):
             callbacks = [callbacks]
         for callback in callbacks:
             assert isinstance(callback, Callback), "Args `callbacks` only support Callback() inputs"
 
         history = History()
         callbacks_ = [BaseLogger(self.stateful_metrics)]
 
@@ -208,24 +214,15 @@
                 except StopIteration:
                     self.callbacks.on_dataloader_end()  # 适用于数据量较大时，动态读取文件并重新生成self.train_dataloader的情况，如预训练
                     train_dataloader_iter = iter(self.train_dataloader)  # shuffle=True时候，其实顺序也重新生成了
                     self.bti = 0
                     batch = next(train_dataloader_iter)
                 self.train_X, self.train_y = batch
 
-                # 从train_X中取batch_size，最多允许嵌套两层，即encoder和decoder的((token_ids1, mask1), (token_ids2, mask2))
-                if isinstance(self.train_X, (list, tuple)) and isinstance(self.train_X[0], (list, tuple)):
-                    btz = self.train_X[0][0].size(0)
-                elif isinstance(self.train_X, (list, tuple)) and (not isinstance(self.train_X[0], (list, tuple))):
-                    btz = self.train_X[0].size(0)
-                elif isinstance(self.train_X, torch.Tensor):
-                    btz = self.train_X.size(0)
-                else:
-                    raise ValueError('Input only support `[list, tuple, tensor]`')
-                logs = {'size': btz}
+                logs = self.get_batch_size()
                 self.callbacks.on_batch_begin(self.global_step, self.local_step, logs)
 
                 self.get_module().train()  # 设置为train模式
 
                 # 入参个数判断，如果入参>=3表示是多个入参，如果=2则表示是一个入参
                 self.output, self.loss, self.loss_detail = self.train_step(self.train_X, self.train_y)
                 self.callbacks.on_train_step_end()
@@ -278,14 +275,32 @@
             self.callbacks.on_epoch_end(self.global_step, self.epoch, logs)
             # TerminateOnNaN、EarlyStopping等停止训练策略
             if callback_trainer.stop_training:
                 break
         self.callbacks.on_train_end(logs)
         return history
 
+    def get_batch_size(self):
+        '''获取batch_size，主要是用于callback中的BaseLogger和Callback
+        '''
+        # 从train_X中取batch_size，最多允许嵌套两层，即encoder和decoder的((token_ids1, mask1), (token_ids2, mask2))
+        if isinstance(self.train_X, (list, tuple)) and isinstance(self.train_X[0], (list, tuple)):
+            btz = self.train_X[0][0].size(0)
+        elif isinstance(self.train_X, (list, tuple)) and isinstance(self.train_X[0], torch.Tensor):
+            btz = self.train_X[0].size(0)
+        elif isinstance(self.train_X, (list, tuple)) and isinstance(self.train_X[0], dict):
+            btz = self.train_X[0].get('batch_size', 0)
+        elif isinstance(self.train_X, dict):
+            btz = self.train_X.get('batch_size', 0)
+        elif isinstance(self.train_X, torch.Tensor):
+            btz = self.train_X.size(0)
+        else:
+            raise ValueError('Input only support `[list, tuple, tensor]`')
+        return {'size': btz}
+
     @torch.no_grad()
     def predict(self, train_X, return_all=None):
         '''模型预测，调用forward()
 
         :param train_X: torch.Tensor, 预测用的数据集
         :param return_all: None/int, 若返回为多个时候指定仅返回第几个，默认为None表示全部返回
         :return: Any, 预测输出
@@ -315,38 +330,56 @@
         :param save_path: str, 训练过程参数保存路径
         '''
         step_params = {'resume_step': (self.local_step+1) % self.steps_per_epoch, 
                        'resume_epoch': self.epoch + (self.local_step+1) // self.steps_per_epoch}
         torch.save(step_params, save_path)
 
     def load_weights(self, load_path, strict=True, mapping={}):
-        '''加载模型权重
+        '''加载模型权重, 支持加载权重文件list
 
-        :param save_path: str, 权重加载路径
+        :param save_path: str/tuple/list, 权重加载路径
+        :param strict: bool, torch.load()是否严格加载
         :param mapping: dict, 指定key的映射
         '''
-        state_dict = torch.load(load_path, map_location='cpu')
         state_dict_raw = {}
-        for k, v in state_dict.items():
-            k = mapping.get(k, k)
-            state_dict_raw[k] = v
-        self.get_module().load_state_dict(state_dict_raw, strict=strict)
+        if isinstance(load_path, (tuple, list)):
+            strict = False  # 加载多个权重文件时候，strict设置为False
+        elif isinstance(load_path, str):
+            load_path = [load_path]
+        else:
+            raise ValueError('Args `load_path` only support str/tuple/list format')
+        
+        for load_path_i in load_path:
+            state_dict = torch.load(load_path_i, map_location='cpu')
+            for k, v in state_dict.items():
+                k = mapping.get(k, k)
+                state_dict_raw[k] = v
+            self.get_module().load_state_dict(state_dict_raw, strict=strict)
 
-    def save_weights(self, save_path, mapping={}):
+    def save_weights(self, save_path, mapping={}, trainable_only=False, verbose=1):
         '''保存模型权重
 
         :param save_path: str, 权重保存路径
         :param mapping: dict, 指定key的映射
+        :param trainable_only: bool, 指定仅保存可训练参数
         '''
         state_dict_raw = {}
         state_dict = self.get_module().state_dict()
+        trainable_parameters = set(p for p,v in self.get_module().named_parameters() if v.requires_grad)
         for k, v in state_dict.items():
+            # 只保存可训练的模型部分
+            if trainable_only and (k not in trainable_parameters):
+                continue
             k = mapping.get(k, k)
             state_dict_raw[k] = v
         torch.save(state_dict_raw, save_path)
+        if trainable_only and (verbose > 0):
+            params_all = sum(p.numel() for p in self.get_module().parameters())
+            params_trainable = sum(p.numel() for p in self.get_module().parameters() if p.requires_grad)
+            print(f"[INFO] Only trainable parameters saved and occupy {params_trainable}/{params_all} {params_trainable/params_all:.2f}%")
 
     def resume_from_checkpoint(self, model_path=None, optimizer_path=None, step_params_path=None):
         '''同时加载模型、优化器、训练过程参数
 
         :param model_path: str, 模型文件路径
         :param optimizer_path: str, 优化器文件路径
         :param step_params_path: str, 训练过程参数保存路径
@@ -385,33 +418,28 @@
         '''返回nn.Module模块
         '''
         if isinstance(self, nn.Module): return self
         return self.module if hasattr(self, 'module') else self
 
 
 class BaseModel(Trainer, nn.Module):
-    """BaseModel, 支持继承、传入Module实例两种方式, 建议使用继承的方式来使用
+    """BaseModel, 使用继承的方式来使用
     """
     def __init__(self, *args, **kwargs):
         nn.Module.__init__(self)
         Trainer.__init__(self, *args, **kwargs)
         
 
 class BaseModelDP(nn.DataParallel, BaseModel):
     '''DataParallel模式使用多gpu的方法, 父类顺序颠倒也会出问题
     '''
     def __init__(self, *args, **kwargs):
         BaseModel.__init__(self)
         nn.DataParallel.__init__(self, *args, **kwargs)
-    
-    # # 使用dp自身的forward()而不是module.forward()
-    # def _forward(self, train_X):
-    #     if isinstance(train_X, torch.Tensor):
-    #         return self.forward(train_X)
-    #     return self.forward(*train_X)
+
 
 class BaseModelDDP(nn.parallel.DistributedDataParallel, BaseModel):
     '''DistributedDataParallel模式使用多gpu的方法, 父类顺序颠倒也会出问题
     '''
     def __init__(self, *args, master_rank=0, **kwargs):
         BaseModel.__init__(self)
         nn.parallel.DistributedDataParallel.__init__(self, *args, **kwargs)
```

### Comparing `torch4keras-0.0.6/torch4keras/snippets.py` & `torch4keras-0.0.7/torch4keras/callbacks.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,34 +1,24 @@
-import numpy as np
-import torch
-import time
 import sys
 import collections
-import inspect
+import time
+import numpy as np
 from datetime import datetime
-from packaging import version
-from torch.utils.data import Dataset, IterableDataset
 from tqdm import tqdm
 import warnings
-import os
-import random
 from collections import deque
 import json
 import copy
-try:
-    from sklearn.metrics import roc_auc_score
-except ImportError:
-    roc_auc_score = None
+import os
 
 try:
     import requests
 except ImportError:
     requests = None
 
-
 class Progbar(object):
     """进度条，直接从keras引入
     """
     def __init__(self, target, width=30, verbose=1, interval=0.05, stateful_metrics=None):
         self.target = target
         self.width = width
         self.verbose = verbose
@@ -302,15 +292,15 @@
     def on_dataloader_end(self, logs=None):
         pass
     def on_train_step_end(self, logs=None):
         pass
 
 
 class BaseLogger(Callback):
-    """计算metrics的均值, 默认是callbacks中第一项
+    """计算metrics的均值, 默认是callbacks中第一项, 主要是为History服务
     
     :param stateful_metrics: List[str], 仅保留状态信息的指标
     """
     def __init__(self, stateful_metrics=None, **kwargs):
         super(BaseLogger, self).__init__(**kwargs)
         if stateful_metrics:
             self.stateful_metrics = set(stateful_metrics)
@@ -988,191 +978,7 @@
 
     def on_train_begin(self, logs=None):
         self.trainer.loss_backward = False
         self.trainer.get_module = self.get_module
 
     def on_train_step_end(self, logs=None):
         self.accelerator.backward(self.trainer.loss)
-
-        
-def take_along_dim(input_tensor, indices, dim=None):
-    '''兼容部分低版本pytorch没有torch.take_along_dim
-    '''
-    if version.parse(torch.__version__) > version.parse('1.8.1'):
-        return torch.take_along_dim(input_tensor, indices, dim)
-    else:
-        # 该逻辑仅在少量数据上测试，如有bug，欢迎反馈
-        if dim is None:
-            res = input_tensor.flatten()[indices]
-        else:
-            res = np.take_along_axis(input_tensor.cpu().numpy(), indices.cpu().numpy(), axis=dim)
-            res = torch.from_numpy(res).to(input_tensor.device)
-        # assert res.equal(torch.take_along_dim(input_tensor, indices, dim))
-        return res
-
-
-def torch_div(input, other, rounding_mode=None):
-    ''' torch.div兼容老版本
-    '''
-    if version.parse(torch.__version__) < version.parse('1.7.2'):
-        indices = input // other  # 兼容老版本
-    else:
-        indices = torch.div(input, other, rounding_mode=rounding_mode)  # 行索引
-    return indices
-
-
-def softmax(x, axis=-1):
-    """numpy版softmax
-    """
-    x = x - x.max(axis=axis, keepdims=True)
-    x = np.exp(x)
-    return x / x.sum(axis=axis, keepdims=True)
-
-
-def search_layer(model, layer_name, retrun_first=True):
-    '''根据layer_name搜索并返回参数/参数list
-    '''
-    return_list = []
-    for name, param in model.named_parameters():
-        if param.requires_grad and layer_name in name:
-            return_list.append(param)
-    if len(return_list) == 0:
-        return None
-    if retrun_first:
-        return return_list[0]
-    else:
-        return return_list
-
-
-class ListDataset(Dataset):
-    '''数据是List格式Dataset，支持传入file_path或者外部已读入的data(List格式)
-
-    :param file_path: str, 待读取的文件的路径，若无可以为None
-    :param data: List[Any], list格式的数据，和file_path至少有一个不为None
-    '''
-    def __init__(self, file_path=None, data=None, **kwargs):
-        self.kwargs = kwargs
-        if isinstance(file_path, (str, tuple, list)):
-            self.data = self.load_data(file_path)
-        elif isinstance(data, list):
-            self.data = data
-        else:
-            raise ValueError('The input args shall be str format file_path / list format dataset')
-
-    def __len__(self):
-        return len(self.data)
-
-    def __getitem__(self, index):
-        return self.data[index]
-
-    @staticmethod
-    def load_data(file_path):
-        return file_path
-
-
-class IterDataset(IterableDataset):
-    '''流式读取文件，用于大数据量、多小文件使用时候需要注意steps_per_epoch != None
-
-    :param file_path: str, 待读取的文件的路径，若无可以为None
-    '''
-    def __init__(self, file_path=None, **kwargs):
-        self.kwargs = kwargs
-        if isinstance(file_path, (str, tuple, list)):
-            self.file_path = file_path
-        else:
-            raise ValueError('The input args shall be str format file_path / list format dataset')
-    
-    def __iter__(self):
-        return self.load_data(self.file_path)
-
-    @staticmethod
-    def load_data(file_path, verbose=0):
-        if isinstance(file_path, (tuple, list)):
-            for file in file_path:
-                if verbose != 0:
-                    print("Load data: ", file)
-                with open(file, 'r') as file_obj:
-                    for line in file_obj:
-                        yield line
-        elif isinstance(file_path, str):
-            with open(file_path, 'r') as file_obj:
-                for line in file_obj:
-                    yield line
-
-
-def metric_mapping(metric, func, y_pred, y_true):
-    '''metric的计算
-
-    :param metric: str, 自带metrics的名称
-    :param func: function, 透传的用户自定的计算指标的函数
-    :param y_pred: torch.Tensor, 样本的预测结果
-    :param y_true: torch.Tensor, 样本的真实结果
-    '''
-    # 自定义metrics
-    if inspect.isfunction(func):
-        metric_res = func(y_pred, y_true)
-        if inspect.isfunction(metric):
-            # 如果直接传入回调函数（无key），要求回调函数返回Dict[String: Int/Float]类型
-            assert isinstance(metric_res, dict), 'Custom metrics callbacks should return `Dict[String: Int/Float]` value'
-        elif isinstance(metric, str):
-            # 如果直接传入回调函数（有key），要求回调函数返回Int/Float类型
-            assert isinstance(metric_res, (int, float)), 'Custom metrics callbacks should return `Int/Float value'
-        return metric_res
-    elif metric == 'loss':
-        pass
-    # 自带metrics
-    elif isinstance(metric, str):
-        # 如果forward返回了list, tuple，则选取第一项
-        y_pred_tmp = y_pred[0] if isinstance(y_pred, (list, tuple)) else y_pred
-        y_true_tmp = y_true[0] if isinstance(y_true, (list, tuple)) else y_true
-        y_pred_tmp = y_pred_tmp.detach()  # 训练过程中评估，detach不进入计算图
-
-        # 根据shape做预处理
-        if len(y_pred_tmp.shape) == len(y_true_tmp.shape) + 1:
-            y_pred_tmp = torch.argmax(y_pred_tmp, dim=-1)
-        elif len(y_pred_tmp.shape) == len(y_true_tmp.shape):
-            pass
-        else:
-            raise ValueError(f'y_pred_tmp.shape={y_pred_tmp.shape} while y_true_tmp.shape={y_true_tmp.shape}')
-
-        # 执行内置的metric
-        if metric in {'accuracy', 'acc'}:
-            return torch.sum(y_pred_tmp.eq(y_true_tmp)).item() / y_true_tmp.numel()
-        elif metric in {'auc'}:
-            if roc_auc_score is None:
-                raise ImportError('roc_auc_score requires the `sklearn` library.')
-            return roc_auc_score(y_true.cpu().numpy(), y_pred_tmp.cpu().numpy())            
-        elif metric in {'mae', 'MAE', 'mean_absolute_error'}:
-            return torch.mean(torch.abs(y_pred_tmp - y_true_tmp)).item()
-        elif metric in {'mse', 'MSE', 'mean_squared_error'}:
-            return torch.mean(torch.square(y_pred_tmp - y_true_tmp)).item()
-        elif metric in {'mape', 'MAPE', 'mean_absolute_percentage_error'}:
-            diff = torch.abs((y_true_tmp - y_pred_tmp) / torch.clamp(torch.abs(y_true_tmp), 1e-7, None))
-            return 100. * torch.mean(diff).item()
-        elif metric in {'msle', 'MSLE', 'mean_squared_logarithmic_error'}:
-            first_log = torch.log(torch.clamp(y_pred_tmp, 1e-7, None) + 1.)
-            second_log = torch.log(torch.clamp(y_true_tmp, 1e-7, None) + 1.)
-            return torch.mean(torch.square(first_log - second_log)).item()
-
-    return None
-
-
-def seed_everything(seed=None):
-    '''固定seed
-    
-    :param seed: int, 随机种子
-    '''
-    max_seed_value = np.iinfo(np.uint32).max
-    min_seed_value = np.iinfo(np.uint32).min
-
-    if (seed is None) or not (min_seed_value <= seed <= max_seed_value):
-        seed = random.randint(np.iinfo(np.uint32).min, np.iinfo(np.uint32).max)
-    print(f"Global seed set to {seed}")
-    os.environ["PYTHONHASHSEED"] = str(seed)
-    random.seed(seed)
-    np.random.seed(seed)
-    torch.manual_seed(seed)
-    torch.cuda.manual_seed(seed)
-    torch.cuda.manual_seed_all(seed)
-    torch.backends.cudnn.benchmark = False
-    torch.backends.cudnn.deterministic = True
-    return seed
```

### Comparing `torch4keras-0.0.6/torch4keras.egg-info/PKG-INFO` & `torch4keras-0.0.7/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,17 +1,7 @@
-Metadata-Version: 2.1
-Name: torch4keras
-Version: 0.0.6
-Summary: Use torch like keras
-Home-page: https://github.com/Tongjilibo/torch4keras
-Author: Tongjilibo
-License: Apache License
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # torch4keras
 **Use torch like keras**
 
 [![licence](https://img.shields.io/github/license/Tongjilibo/torch4keras.svg?maxAge=3600)](https://github.com/Tongjilibo/torch4keras/blob/master/LICENSE) 
 [![GitHub release](https://img.shields.io/github/release/Tongjilibo/torch4keras.svg?maxAge=3600)](https://github.com/Tongjilibo/torch4keras/releases) 
 [![PyPI](https://img.shields.io/pypi/v/torch4keras?label=pypi%20package)](https://pypi.org/project/torch4keras/) 
 [![PyPI - Downloads](https://img.shields.io/pypi/dm/torch4keras)](https://pypistats.org/packages/torch4keras)
@@ -26,15 +16,15 @@
 ## 1. 下载安装
 安装稳定版
 ```shell
 pip install torch4keras
 ```
 安装最新版
 ```shell
-pip install git+https://www.github.com/Tongjilibo/torch4keras.git
+pip install git+https://github.com/Tongjilibo/torch4keras.git
 ```
 
 ## 2. 功能
 - 简述：抽象出来的Trainer，适用于一般神经网络的训练，仅需关注网络结构代码
 - 特色：进度条展示训练过程，自定义metric，自带Evaluator, Checkpoint, Tensorboard, Logger等Callback，也可自定义Callback
 - 初衷：前期功能是作为[bert4torch](https://github.com/Tongjilibo/bert4torch)和[rec4torch](https://github.com/Tongjilibo/rec4torch)的Trainer
 - 训练：
@@ -70,24 +60,27 @@
     ```
 
 ## 3. 快速上手
 - 参考[bert4torch](https://github.com/Tongjilibo/bert4torch)的训练过程
 - 简单示例: [turorials_mnist](https://github.com/Tongjilibo/torch4keras/blob/master/examples/turorials_mnist.py)
 
 ## 4. 版本说明
+- **v0.0.7**：20230505 独立出callbacks.py文件, fit允许输入形式为字典，load_weights支持list输入，save_weights支持仅保存可训练参数
+- **v0.0.6**：20230212 增加resume_from_checkpoint和save_to_checkpoint；增加add_trainer方法，重构了Trainer(BaseModel)的实现(增加几个成员变量、增加initilize()、删除对forward参数个数的判断、dp和ddp不解析module、修改use_amp参数为mixed_precision)，增加了AccelerateCallback
 - **v0.0.5**：20221217 增加Summary的Callback, 增加Tqdm的进度条展示，保留原有BaseModel的同时，增加Trainer(不从nn.Module继承), 从bert4torch的snippets迁移部分通用函数
 - **v0.0.4**：20221127 为callback增加on_train_step_end方法, 修复BaseModel(net)方式的bug
 - **v0.0.3.post2**：20221107 修复DDP下打印的bug
 - **v0.0.3**：20221106 参考Keras修改了callback的逻辑
 - **v0.0.2**：20221023 增加Checkpoint, Evaluator等自带Callback, 修改BaseModel(net)方式，修复DP和DDP的__init__()
 - **v0.0.1**：20221019 初始版本
 
 ## 5. 更新：
-- **20230207**：增加hf的accelerator测试用例, ddp需要外部控制执行callback, 混合精度支持bf16, 增加add_trainer方法
-- **20230116**：增加resume_from_checkpoint和save_to_checkpoint，动态为nn.Module增加Trainer的方法
+- **20230505**：独立出callbacks.py文件, fit允许输入形式为字典，load_weights支持list输入，save_weights支持仅保存可训练参数
+- **20230212**：增加hf的accelerator测试用例, ddp需要外部控制执行callback, 混合精度支持bf16
+- **20230116**：增加resume_from_checkpoint和save_to_checkpoint，动态为nn.Module增加Trainer的方法add_trainer
 - **20221217**：保留原有BaseModel的同时，增加Trainer(不从nn.Module继承), 从bert4torch的snippets迁移部分通用函数
 - **20221203**：增加Summary的Callback, 增加Tqdm的进度条展示
 - **20221127**：为callback增加on_train_step_end方法, 修复BaseModel(net)方式的bug
 - **20221107**：修复DDP下打印的bug，metrics中加入detach和auc
 - **20221106**：默认的Tensorboard的global_step+1, 参考Keras修改了callback的逻辑
 - **20221020**：增加Checkpoint, Evaluator等自带Callback, 修改BaseModel(net)方式，修复DP和DDP的__init__()
 - **20221019**：初版提交
```

