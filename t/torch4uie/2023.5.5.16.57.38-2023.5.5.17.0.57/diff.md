# Comparing `tmp/torch4uie-2023.5.5.16.57.38.tar.gz` & `tmp/torch4uie-2023.5.5.17.0.57.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "torch4uie-2023.5.5.16.57.38.tar", last modified: Fri May  5 08:57:38 2023, max compression
+gzip compressed data, was "torch4uie-2023.5.5.17.0.57.tar", last modified: Fri May  5 09:00:57 2023, max compression
```

## Comparing `torch4uie-2023.5.5.16.57.38.tar` & `torch4uie-2023.5.5.17.0.57.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-05-05 08:57:38.577217 torch4uie-2023.5.5.16.57.38/
--rw-r--r--   0 betterme   (501) staff       (20)     1196 2023-04-20 11:38:14.000000 torch4uie-2023.5.5.16.57.38/.gitignore
--rw-r--r--   0 betterme   (501) staff       (20)      289 2023-04-11 04:23:57.000000 torch4uie-2023.5.5.16.57.38/MANIFEST.in
--rw-r--r--   0 betterme   (501) staff       (20)    41295 2023-05-05 08:57:38.577057 torch4uie-2023.5.5.16.57.38/PKG-INFO
--rw-r--r--   0 betterme   (501) staff       (20)    40600 2023-05-05 08:24:54.000000 torch4uie-2023.5.5.16.57.38/README.md
--rw-r--r--   0 betterme   (501) staff       (20)       97 2023-05-05 08:57:37.000000 torch4uie-2023.5.5.16.57.38/requirements.txt
--rw-r--r--   0 betterme   (501) staff       (20)       38 2023-05-05 08:57:38.577260 torch4uie-2023.5.5.16.57.38/setup.cfg
--rw-r--r--   0 betterme   (501) staff       (20)     1754 2023-05-05 08:56:54.000000 torch4uie-2023.5.5.16.57.38/setup.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-05-05 08:57:38.574958 torch4uie-2023.5.5.16.57.38/torch4uie.egg-info/
--rw-r--r--   0 betterme   (501) staff       (20)    41295 2023-05-05 08:57:38.000000 torch4uie-2023.5.5.16.57.38/torch4uie.egg-info/PKG-INFO
--rw-r--r--   0 betterme   (501) staff       (20)      497 2023-05-05 08:57:38.000000 torch4uie-2023.5.5.16.57.38/torch4uie.egg-info/SOURCES.txt
--rw-r--r--   0 betterme   (501) staff       (20)        1 2023-05-05 08:57:38.000000 torch4uie-2023.5.5.16.57.38/torch4uie.egg-info/dependency_links.txt
--rw-r--r--   0 betterme   (501) staff       (20)       53 2023-05-05 08:57:38.000000 torch4uie-2023.5.5.16.57.38/torch4uie.egg-info/entry_points.txt
--rw-r--r--   0 betterme   (501) staff       (20)        1 2023-05-05 08:57:38.000000 torch4uie-2023.5.5.16.57.38/torch4uie.egg-info/not-zip-safe
--rw-r--r--   0 betterme   (501) staff       (20)      104 2023-05-05 08:57:38.000000 torch4uie-2023.5.5.16.57.38/torch4uie.egg-info/requires.txt
--rw-r--r--   0 betterme   (501) staff       (20)        4 2023-05-05 08:57:38.000000 torch4uie-2023.5.5.16.57.38/torch4uie.egg-info/top_level.txt
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-05-05 08:57:38.576780 torch4uie-2023.5.5.16.57.38/uie/
--rw-r--r--   0 betterme   (501) staff       (20)      266 2023-05-05 08:50:31.000000 torch4uie-2023.5.5.16.57.38/uie/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)    24308 2023-05-05 08:24:54.000000 torch4uie-2023.5.5.16.57.38/uie/convert.py
--rw-r--r--   0 betterme   (501) staff       (20)     8474 2023-05-05 08:24:54.000000 torch4uie-2023.5.5.16.57.38/uie/doccano.py
--rw-r--r--   0 betterme   (501) staff       (20)    48643 2023-05-05 08:24:54.000000 torch4uie-2023.5.5.16.57.38/uie/ernie.py
--rw-r--r--   0 betterme   (501) staff       (20)    43974 2023-05-05 08:24:54.000000 torch4uie-2023.5.5.16.57.38/uie/ernie_m.py
--rw-r--r--   0 betterme   (501) staff       (20)     6757 2023-05-05 08:24:54.000000 torch4uie-2023.5.5.16.57.38/uie/evaluate.py
--rw-r--r--   0 betterme   (501) staff       (20)     7802 2023-05-05 08:24:54.000000 torch4uie-2023.5.5.16.57.38/uie/export_model.py
--rw-r--r--   0 betterme   (501) staff       (20)    11286 2023-05-05 08:24:54.000000 torch4uie-2023.5.5.16.57.38/uie/finetune.py
--rw-r--r--   0 betterme   (501) staff       (20)     3707 2023-05-05 08:24:54.000000 torch4uie-2023.5.5.16.57.38/uie/labelstudio2doccano.py
--rw-r--r--   0 betterme   (501) staff       (20)    16534 2023-05-05 08:24:54.000000 torch4uie-2023.5.5.16.57.38/uie/model.py
--rw-r--r--   0 betterme   (501) staff       (20)    28015 2023-05-05 08:24:54.000000 torch4uie-2023.5.5.16.57.38/uie/tokenizer.py
--rw-r--r--   0 betterme   (501) staff       (20)    27756 2023-05-05 08:47:28.000000 torch4uie-2023.5.5.16.57.38/uie/uie.py
--rw-r--r--   0 betterme   (501) staff       (20)    46414 2023-05-05 08:24:54.000000 torch4uie-2023.5.5.16.57.38/uie/utils.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-05-05 09:00:57.373734 torch4uie-2023.5.5.17.0.57/
+-rw-r--r--   0 betterme   (501) staff       (20)     1196 2023-04-20 11:38:14.000000 torch4uie-2023.5.5.17.0.57/.gitignore
+-rw-r--r--   0 betterme   (501) staff       (20)      289 2023-04-11 04:23:57.000000 torch4uie-2023.5.5.17.0.57/MANIFEST.in
+-rw-r--r--   0 betterme   (501) staff       (20)    41294 2023-05-05 09:00:57.373539 torch4uie-2023.5.5.17.0.57/PKG-INFO
+-rw-r--r--   0 betterme   (501) staff       (20)    40600 2023-05-05 08:24:54.000000 torch4uie-2023.5.5.17.0.57/README.md
+-rw-r--r--   0 betterme   (501) staff       (20)       97 2023-05-05 08:57:37.000000 torch4uie-2023.5.5.17.0.57/requirements.txt
+-rw-r--r--   0 betterme   (501) staff       (20)       38 2023-05-05 09:00:57.373786 torch4uie-2023.5.5.17.0.57/setup.cfg
+-rw-r--r--   0 betterme   (501) staff       (20)     1754 2023-05-05 08:56:54.000000 torch4uie-2023.5.5.17.0.57/setup.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-05-05 09:00:57.371372 torch4uie-2023.5.5.17.0.57/torch4uie.egg-info/
+-rw-r--r--   0 betterme   (501) staff       (20)    41294 2023-05-05 09:00:57.000000 torch4uie-2023.5.5.17.0.57/torch4uie.egg-info/PKG-INFO
+-rw-r--r--   0 betterme   (501) staff       (20)      497 2023-05-05 09:00:57.000000 torch4uie-2023.5.5.17.0.57/torch4uie.egg-info/SOURCES.txt
+-rw-r--r--   0 betterme   (501) staff       (20)        1 2023-05-05 09:00:57.000000 torch4uie-2023.5.5.17.0.57/torch4uie.egg-info/dependency_links.txt
+-rw-r--r--   0 betterme   (501) staff       (20)       53 2023-05-05 09:00:57.000000 torch4uie-2023.5.5.17.0.57/torch4uie.egg-info/entry_points.txt
+-rw-r--r--   0 betterme   (501) staff       (20)        1 2023-05-05 09:00:57.000000 torch4uie-2023.5.5.17.0.57/torch4uie.egg-info/not-zip-safe
+-rw-r--r--   0 betterme   (501) staff       (20)      104 2023-05-05 09:00:57.000000 torch4uie-2023.5.5.17.0.57/torch4uie.egg-info/requires.txt
+-rw-r--r--   0 betterme   (501) staff       (20)        4 2023-05-05 09:00:57.000000 torch4uie-2023.5.5.17.0.57/torch4uie.egg-info/top_level.txt
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-05-05 09:00:57.373248 torch4uie-2023.5.5.17.0.57/uie/
+-rw-r--r--   0 betterme   (501) staff       (20)      266 2023-05-05 08:50:31.000000 torch4uie-2023.5.5.17.0.57/uie/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)    24308 2023-05-05 08:24:54.000000 torch4uie-2023.5.5.17.0.57/uie/convert.py
+-rw-r--r--   0 betterme   (501) staff       (20)     8474 2023-05-05 08:24:54.000000 torch4uie-2023.5.5.17.0.57/uie/doccano.py
+-rw-r--r--   0 betterme   (501) staff       (20)    48643 2023-05-05 08:24:54.000000 torch4uie-2023.5.5.17.0.57/uie/ernie.py
+-rw-r--r--   0 betterme   (501) staff       (20)    43974 2023-05-05 08:24:54.000000 torch4uie-2023.5.5.17.0.57/uie/ernie_m.py
+-rw-r--r--   0 betterme   (501) staff       (20)     6761 2023-05-05 09:00:55.000000 torch4uie-2023.5.5.17.0.57/uie/evaluate.py
+-rw-r--r--   0 betterme   (501) staff       (20)     7806 2023-05-05 09:00:55.000000 torch4uie-2023.5.5.17.0.57/uie/export_model.py
+-rw-r--r--   0 betterme   (501) staff       (20)    11294 2023-05-05 09:00:55.000000 torch4uie-2023.5.5.17.0.57/uie/finetune.py
+-rw-r--r--   0 betterme   (501) staff       (20)     3707 2023-05-05 08:24:54.000000 torch4uie-2023.5.5.17.0.57/uie/labelstudio2doccano.py
+-rw-r--r--   0 betterme   (501) staff       (20)    16542 2023-05-05 09:00:55.000000 torch4uie-2023.5.5.17.0.57/uie/model.py
+-rw-r--r--   0 betterme   (501) staff       (20)    28015 2023-05-05 08:24:54.000000 torch4uie-2023.5.5.17.0.57/uie/tokenizer.py
+-rw-r--r--   0 betterme   (501) staff       (20)    27760 2023-05-05 09:00:55.000000 torch4uie-2023.5.5.17.0.57/uie/uie.py
+-rw-r--r--   0 betterme   (501) staff       (20)    46414 2023-05-05 08:24:54.000000 torch4uie-2023.5.5.17.0.57/uie/utils.py
```

### Comparing `torch4uie-2023.5.5.16.57.38/.gitignore` & `torch4uie-2023.5.5.17.0.57/.gitignore`

 * *Files identical despite different names*

### Comparing `torch4uie-2023.5.5.16.57.38/PKG-INFO` & `torch4uie-2023.5.5.17.0.57/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: torch4uie
-Version: 2023.5.5.16.57.38
+Version: 2023.5.5.17.0.57
 Summary: Create a Python package.
 Home-page: https://github.com/yuanjie-ai/ChatLLM
 Author: yuanjie
 Author-email: 313303303@qq.com
 License: MIT license
 Keywords: uie
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `torch4uie-2023.5.5.16.57.38/README.md` & `torch4uie-2023.5.5.17.0.57/README.md`

 * *Files identical despite different names*

### Comparing `torch4uie-2023.5.5.16.57.38/setup.py` & `torch4uie-2023.5.5.17.0.57/setup.py`

 * *Files identical despite different names*

### Comparing `torch4uie-2023.5.5.16.57.38/torch4uie.egg-info/PKG-INFO` & `torch4uie-2023.5.5.17.0.57/torch4uie.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: torch4uie
-Version: 2023.5.5.16.57.38
+Version: 2023.5.5.17.0.57
 Summary: Create a Python package.
 Home-page: https://github.com/yuanjie-ai/ChatLLM
 Author: yuanjie
 Author-email: 313303303@qq.com
 License: MIT license
 Keywords: uie
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `torch4uie-2023.5.5.16.57.38/uie/convert.py` & `torch4uie-2023.5.5.17.0.57/uie/convert.py`

 * *Files identical despite different names*

### Comparing `torch4uie-2023.5.5.16.57.38/uie/doccano.py` & `torch4uie-2023.5.5.17.0.57/uie/doccano.py`

 * *Files identical despite different names*

### Comparing `torch4uie-2023.5.5.16.57.38/uie/ernie.py` & `torch4uie-2023.5.5.17.0.57/uie/ernie.py`

 * *Files identical despite different names*

### Comparing `torch4uie-2023.5.5.16.57.38/uie/ernie_m.py` & `torch4uie-2023.5.5.17.0.57/uie/ernie_m.py`

 * *Files identical despite different names*

### Comparing `torch4uie-2023.5.5.16.57.38/uie/evaluate.py` & `torch4uie-2023.5.5.17.0.57/uie/evaluate.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 import argparse
 from functools import partial
 
 import torch
 from transformers import BertTokenizerFast
 from torch.utils.data import DataLoader
 
-from utils import IEMapDataset, SpanEvaluator, IEDataset, convert_example, get_relation_type_dict, logger, tqdm, unify_prompt_name
+from uie.utils import IEMapDataset, SpanEvaluator, IEDataset, convert_example, get_relation_type_dict, logger, tqdm, unify_prompt_name
 
 
 @torch.no_grad()
 def evaluate(model, metric, data_loader, device='gpu', loss_fn=None, show_bar=True):
     """
     Given a dataset, it evals model and computes the metric.
     Args:
```

### Comparing `torch4uie-2023.5.5.16.57.38/uie/export_model.py` & `torch4uie-2023.5.5.17.0.57/uie/export_model.py`

 * *Files 0% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 
 import numpy as np
 import torch
 from transformers import (BertTokenizer, PreTrainedModel,
                           PreTrainedTokenizerBase)
 
 from model import UIE
-from utils import logger
+from uie.utils import logger
 
 
 def validate_onnx(tokenizer: PreTrainedTokenizerBase, pt_model: PreTrainedModel, onnx_path: Union[Path, str], strict: bool = True, atol: float = 1e-05):
 
     # 验证模型
     from onnxruntime import InferenceSession, SessionOptions
     from transformers import AutoTokenizer
```

### Comparing `torch4uie-2023.5.5.16.57.38/uie/finetune.py` & `torch4uie-2023.5.5.17.0.57/uie/finetune.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,18 +17,18 @@
 import sys
 import time
 import os
 import torch
 from torch.utils.data import DataLoader
 from transformers import BertTokenizerFast
 
-from utils import IEDataset, logger, tqdm
+from uie.utils import IEDataset, logger, tqdm
 from model import UIE
 from evaluate import evaluate
-from utils import set_seed, SpanEvaluator, EarlyStopping, logging_redirect_tqdm
+from uie.utils import set_seed, SpanEvaluator, EarlyStopping, logging_redirect_tqdm
 
 
 def do_train():
 
     set_seed(args.seed)
     show_bar = True
```

### Comparing `torch4uie-2023.5.5.16.57.38/uie/labelstudio2doccano.py` & `torch4uie-2023.5.5.17.0.57/uie/labelstudio2doccano.py`

 * *Files identical despite different names*

### Comparing `torch4uie-2023.5.5.16.57.38/uie/model.py` & `torch4uie-2023.5.5.17.0.57/uie/model.py`

 * *Files 1% similar despite different names*

```diff
@@ -15,16 +15,16 @@
 import torch
 import torch.nn as nn
 from dataclasses import dataclass
 from transformers import PretrainedConfig
 from transformers.utils import ModelOutput
 from typing import Optional, Tuple
 
-from ernie import ErnieModel, ErniePreTrainedModel
-from ernie_m import ErnieMModel, ErnieMPreTrainedModel
+from uie.ernie import ErnieModel, ErniePreTrainedModel
+from uie.ernie_m import ErnieMModel, ErnieMPreTrainedModel
 
 
 @dataclass
 class UIEModelOutput(ModelOutput):
     """
     Output class for outputs of UIE.
     Args:
```

### Comparing `torch4uie-2023.5.5.16.57.38/uie/tokenizer.py` & `torch4uie-2023.5.5.17.0.57/uie/tokenizer.py`

 * *Files identical despite different names*

### Comparing `torch4uie-2023.5.5.16.57.38/uie/uie.py` & `torch4uie-2023.5.5.17.0.57/uie/uie.py`

 * *Files 0% similar despite different names*

```diff
@@ -17,15 +17,15 @@
 import six
 
 
 import math
 import argparse
 import os.path
 
-from utils import logger, get_bool_ids_greater_than, get_span, get_id_and_prob, cut_chinese_sent, dbc2sbc
+from uie.utils import logger, get_bool_ids_greater_than, get_span, get_id_and_prob, cut_chinese_sent, dbc2sbc
 
 
 class ONNXInferBackend(object):
     def __init__(self,
                  model_path_prefix,
                  device='cpu',
                  use_fp16=False):
```

### Comparing `torch4uie-2023.5.5.16.57.38/uie/utils.py` & `torch4uie-2023.5.5.17.0.57/uie/utils.py`

 * *Files identical despite different names*

