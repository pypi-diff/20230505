# Comparing `tmp/torch4uie-2023.5.5.17.7.51.tar.gz` & `tmp/torch4uie-2023.5.5.17.9.31.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "torch4uie-2023.5.5.17.7.51.tar", last modified: Fri May  5 09:07:51 2023, max compression
+gzip compressed data, was "torch4uie-2023.5.5.17.9.31.tar", last modified: Fri May  5 09:09:32 2023, max compression
```

## Comparing `torch4uie-2023.5.5.17.7.51.tar` & `torch4uie-2023.5.5.17.9.31.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-05-05 09:07:51.854908 torch4uie-2023.5.5.17.7.51/
--rw-r--r--   0 betterme   (501) staff       (20)     1196 2023-04-20 11:38:14.000000 torch4uie-2023.5.5.17.7.51/.gitignore
--rw-r--r--   0 betterme   (501) staff       (20)      289 2023-04-11 04:23:57.000000 torch4uie-2023.5.5.17.7.51/MANIFEST.in
--rw-r--r--   0 betterme   (501) staff       (20)    41294 2023-05-05 09:07:51.854727 torch4uie-2023.5.5.17.7.51/PKG-INFO
--rw-r--r--   0 betterme   (501) staff       (20)    40600 2023-05-05 08:24:54.000000 torch4uie-2023.5.5.17.7.51/README.md
--rw-r--r--   0 betterme   (501) staff       (20)      120 2023-05-05 09:07:46.000000 torch4uie-2023.5.5.17.7.51/requirements.txt
--rw-r--r--   0 betterme   (501) staff       (20)       38 2023-05-05 09:07:51.854958 torch4uie-2023.5.5.17.7.51/setup.cfg
--rw-r--r--   0 betterme   (501) staff       (20)     1754 2023-05-05 08:56:54.000000 torch4uie-2023.5.5.17.7.51/setup.py
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-05-05 09:07:51.852644 torch4uie-2023.5.5.17.7.51/torch4uie.egg-info/
--rw-r--r--   0 betterme   (501) staff       (20)    41294 2023-05-05 09:07:51.000000 torch4uie-2023.5.5.17.7.51/torch4uie.egg-info/PKG-INFO
--rw-r--r--   0 betterme   (501) staff       (20)      497 2023-05-05 09:07:51.000000 torch4uie-2023.5.5.17.7.51/torch4uie.egg-info/SOURCES.txt
--rw-r--r--   0 betterme   (501) staff       (20)        1 2023-05-05 09:07:51.000000 torch4uie-2023.5.5.17.7.51/torch4uie.egg-info/dependency_links.txt
--rw-r--r--   0 betterme   (501) staff       (20)       53 2023-05-05 09:07:51.000000 torch4uie-2023.5.5.17.7.51/torch4uie.egg-info/entry_points.txt
--rw-r--r--   0 betterme   (501) staff       (20)        1 2023-05-05 09:07:51.000000 torch4uie-2023.5.5.17.7.51/torch4uie.egg-info/not-zip-safe
--rw-r--r--   0 betterme   (501) staff       (20)      125 2023-05-05 09:07:51.000000 torch4uie-2023.5.5.17.7.51/torch4uie.egg-info/requires.txt
--rw-r--r--   0 betterme   (501) staff       (20)        4 2023-05-05 09:07:51.000000 torch4uie-2023.5.5.17.7.51/torch4uie.egg-info/top_level.txt
-drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-05-05 09:07:51.854433 torch4uie-2023.5.5.17.7.51/uie/
--rw-r--r--   0 betterme   (501) staff       (20)      266 2023-05-05 08:50:31.000000 torch4uie-2023.5.5.17.7.51/uie/__init__.py
--rw-r--r--   0 betterme   (501) staff       (20)    24308 2023-05-05 08:24:54.000000 torch4uie-2023.5.5.17.7.51/uie/convert.py
--rw-r--r--   0 betterme   (501) staff       (20)     8474 2023-05-05 08:24:54.000000 torch4uie-2023.5.5.17.7.51/uie/doccano.py
--rw-r--r--   0 betterme   (501) staff       (20)    48643 2023-05-05 08:24:54.000000 torch4uie-2023.5.5.17.7.51/uie/ernie.py
--rw-r--r--   0 betterme   (501) staff       (20)    43974 2023-05-05 08:24:54.000000 torch4uie-2023.5.5.17.7.51/uie/ernie_m.py
--rw-r--r--   0 betterme   (501) staff       (20)     6761 2023-05-05 09:00:55.000000 torch4uie-2023.5.5.17.7.51/uie/evaluate.py
--rw-r--r--   0 betterme   (501) staff       (20)     7806 2023-05-05 09:00:55.000000 torch4uie-2023.5.5.17.7.51/uie/export_model.py
--rw-r--r--   0 betterme   (501) staff       (20)    11294 2023-05-05 09:00:55.000000 torch4uie-2023.5.5.17.7.51/uie/finetune.py
--rw-r--r--   0 betterme   (501) staff       (20)     3707 2023-05-05 08:24:54.000000 torch4uie-2023.5.5.17.7.51/uie/labelstudio2doccano.py
--rw-r--r--   0 betterme   (501) staff       (20)    16542 2023-05-05 09:00:55.000000 torch4uie-2023.5.5.17.7.51/uie/model.py
--rw-r--r--   0 betterme   (501) staff       (20)    28015 2023-05-05 08:24:54.000000 torch4uie-2023.5.5.17.7.51/uie/tokenizer.py
--rw-r--r--   0 betterme   (501) staff       (20)    27827 2023-05-05 09:07:46.000000 torch4uie-2023.5.5.17.7.51/uie/uie.py
--rw-r--r--   0 betterme   (501) staff       (20)    46414 2023-05-05 08:24:54.000000 torch4uie-2023.5.5.17.7.51/uie/utils.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-05-05 09:09:32.069414 torch4uie-2023.5.5.17.9.31/
+-rw-r--r--   0 betterme   (501) staff       (20)     1196 2023-04-20 11:38:14.000000 torch4uie-2023.5.5.17.9.31/.gitignore
+-rw-r--r--   0 betterme   (501) staff       (20)      289 2023-04-11 04:23:57.000000 torch4uie-2023.5.5.17.9.31/MANIFEST.in
+-rw-r--r--   0 betterme   (501) staff       (20)    41294 2023-05-05 09:09:32.069247 torch4uie-2023.5.5.17.9.31/PKG-INFO
+-rw-r--r--   0 betterme   (501) staff       (20)    40600 2023-05-05 08:24:54.000000 torch4uie-2023.5.5.17.9.31/README.md
+-rw-r--r--   0 betterme   (501) staff       (20)      120 2023-05-05 09:07:46.000000 torch4uie-2023.5.5.17.9.31/requirements.txt
+-rw-r--r--   0 betterme   (501) staff       (20)       38 2023-05-05 09:09:32.069462 torch4uie-2023.5.5.17.9.31/setup.cfg
+-rw-r--r--   0 betterme   (501) staff       (20)     1754 2023-05-05 08:56:54.000000 torch4uie-2023.5.5.17.9.31/setup.py
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-05-05 09:09:32.066988 torch4uie-2023.5.5.17.9.31/torch4uie.egg-info/
+-rw-r--r--   0 betterme   (501) staff       (20)    41294 2023-05-05 09:09:31.000000 torch4uie-2023.5.5.17.9.31/torch4uie.egg-info/PKG-INFO
+-rw-r--r--   0 betterme   (501) staff       (20)      497 2023-05-05 09:09:32.000000 torch4uie-2023.5.5.17.9.31/torch4uie.egg-info/SOURCES.txt
+-rw-r--r--   0 betterme   (501) staff       (20)        1 2023-05-05 09:09:31.000000 torch4uie-2023.5.5.17.9.31/torch4uie.egg-info/dependency_links.txt
+-rw-r--r--   0 betterme   (501) staff       (20)       53 2023-05-05 09:09:31.000000 torch4uie-2023.5.5.17.9.31/torch4uie.egg-info/entry_points.txt
+-rw-r--r--   0 betterme   (501) staff       (20)        1 2023-05-05 09:09:31.000000 torch4uie-2023.5.5.17.9.31/torch4uie.egg-info/not-zip-safe
+-rw-r--r--   0 betterme   (501) staff       (20)      125 2023-05-05 09:09:31.000000 torch4uie-2023.5.5.17.9.31/torch4uie.egg-info/requires.txt
+-rw-r--r--   0 betterme   (501) staff       (20)        4 2023-05-05 09:09:31.000000 torch4uie-2023.5.5.17.9.31/torch4uie.egg-info/top_level.txt
+drwxr-xr-x   0 betterme   (501) staff       (20)        0 2023-05-05 09:09:32.068982 torch4uie-2023.5.5.17.9.31/uie/
+-rw-r--r--   0 betterme   (501) staff       (20)      266 2023-05-05 08:50:31.000000 torch4uie-2023.5.5.17.9.31/uie/__init__.py
+-rw-r--r--   0 betterme   (501) staff       (20)    24316 2023-05-05 09:09:25.000000 torch4uie-2023.5.5.17.9.31/uie/convert.py
+-rw-r--r--   0 betterme   (501) staff       (20)     8478 2023-05-05 09:09:25.000000 torch4uie-2023.5.5.17.9.31/uie/doccano.py
+-rw-r--r--   0 betterme   (501) staff       (20)    48643 2023-05-05 08:24:54.000000 torch4uie-2023.5.5.17.9.31/uie/ernie.py
+-rw-r--r--   0 betterme   (501) staff       (20)    43974 2023-05-05 08:24:54.000000 torch4uie-2023.5.5.17.9.31/uie/ernie_m.py
+-rw-r--r--   0 betterme   (501) staff       (20)     6761 2023-05-05 09:00:55.000000 torch4uie-2023.5.5.17.9.31/uie/evaluate.py
+-rw-r--r--   0 betterme   (501) staff       (20)     7806 2023-05-05 09:00:55.000000 torch4uie-2023.5.5.17.9.31/uie/export_model.py
+-rw-r--r--   0 betterme   (501) staff       (20)    11294 2023-05-05 09:00:55.000000 torch4uie-2023.5.5.17.9.31/uie/finetune.py
+-rw-r--r--   0 betterme   (501) staff       (20)     3707 2023-05-05 08:24:54.000000 torch4uie-2023.5.5.17.9.31/uie/labelstudio2doccano.py
+-rw-r--r--   0 betterme   (501) staff       (20)    16542 2023-05-05 09:00:55.000000 torch4uie-2023.5.5.17.9.31/uie/model.py
+-rw-r--r--   0 betterme   (501) staff       (20)    28019 2023-05-05 09:09:25.000000 torch4uie-2023.5.5.17.9.31/uie/tokenizer.py
+-rw-r--r--   0 betterme   (501) staff       (20)    27827 2023-05-05 09:07:46.000000 torch4uie-2023.5.5.17.9.31/uie/uie.py
+-rw-r--r--   0 betterme   (501) staff       (20)    46414 2023-05-05 08:24:54.000000 torch4uie-2023.5.5.17.9.31/uie/utils.py
```

### Comparing `torch4uie-2023.5.5.17.7.51/.gitignore` & `torch4uie-2023.5.5.17.9.31/.gitignore`

 * *Files identical despite different names*

### Comparing `torch4uie-2023.5.5.17.7.51/PKG-INFO` & `torch4uie-2023.5.5.17.9.31/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: torch4uie
-Version: 2023.5.5.17.7.51
+Version: 2023.5.5.17.9.31
 Summary: Create a Python package.
 Home-page: https://github.com/yuanjie-ai/ChatLLM
 Author: yuanjie
 Author-email: 313303303@qq.com
 License: MIT license
 Keywords: uie
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `torch4uie-2023.5.5.17.7.51/README.md` & `torch4uie-2023.5.5.17.9.31/README.md`

 * *Files identical despite different names*

### Comparing `torch4uie-2023.5.5.17.7.51/setup.py` & `torch4uie-2023.5.5.17.9.31/setup.py`

 * *Files identical despite different names*

### Comparing `torch4uie-2023.5.5.17.7.51/torch4uie.egg-info/PKG-INFO` & `torch4uie-2023.5.5.17.9.31/torch4uie.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: torch4uie
-Version: 2023.5.5.17.7.51
+Version: 2023.5.5.17.9.31
 Summary: Create a Python package.
 Home-page: https://github.com/yuanjie-ai/ChatLLM
 Author: yuanjie
 Author-email: 313303303@qq.com
 License: MIT license
 Keywords: uie
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `torch4uie-2023.5.5.17.7.51/uie/convert.py` & `torch4uie-2023.5.5.17.9.31/uie/convert.py`

 * *Files 0% similar despite different names*

```diff
@@ -23,19 +23,19 @@
 
 import torch
 try:
     import paddle
     from paddle.utils.download import get_path_from_url
     paddle_installed = True
 except (ImportError, ModuleNotFoundError):
-    from utils import get_path_from_url
+    from uie.utils import get_path_from_url
     paddle_installed = False
 
 from model import UIE, UIEM
-from utils import logger
+from uie.utils import logger
 
 MODEL_MAP = {
     # vocab.txt/special_tokens_map.json/tokenizer_config.json are common to the default model.
     "uie-base": {
         "resource_file_urls": {
             "model_state.pdparams":
             "https://bj.bcebos.com/paddlenlp/taskflow/information_extraction/uie_base_v1.0/model_state.pdparams",
```

### Comparing `torch4uie-2023.5.5.17.7.51/uie/doccano.py` & `torch4uie-2023.5.5.17.9.31/uie/doccano.py`

 * *Files 0% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 import os
 import time
 import argparse
 import json
 from decimal import Decimal
 import numpy as np
 
-from utils import set_seed, convert_ext_examples, convert_cls_examples, logger
+from uie.utils import set_seed, convert_ext_examples, convert_cls_examples, logger
 
 
 def do_convert():
     set_seed(args.seed)
 
     tic_time = time.time()
     if not os.path.exists(args.doccano_file):
```

### Comparing `torch4uie-2023.5.5.17.7.51/uie/ernie.py` & `torch4uie-2023.5.5.17.9.31/uie/ernie.py`

 * *Files identical despite different names*

### Comparing `torch4uie-2023.5.5.17.7.51/uie/ernie_m.py` & `torch4uie-2023.5.5.17.9.31/uie/ernie_m.py`

 * *Files identical despite different names*

### Comparing `torch4uie-2023.5.5.17.7.51/uie/evaluate.py` & `torch4uie-2023.5.5.17.9.31/uie/evaluate.py`

 * *Files identical despite different names*

### Comparing `torch4uie-2023.5.5.17.7.51/uie/export_model.py` & `torch4uie-2023.5.5.17.9.31/uie/export_model.py`

 * *Files identical despite different names*

### Comparing `torch4uie-2023.5.5.17.7.51/uie/finetune.py` & `torch4uie-2023.5.5.17.9.31/uie/finetune.py`

 * *Files identical despite different names*

### Comparing `torch4uie-2023.5.5.17.7.51/uie/labelstudio2doccano.py` & `torch4uie-2023.5.5.17.9.31/uie/labelstudio2doccano.py`

 * *Files identical despite different names*

### Comparing `torch4uie-2023.5.5.17.7.51/uie/model.py` & `torch4uie-2023.5.5.17.9.31/uie/model.py`

 * *Files identical despite different names*

### Comparing `torch4uie-2023.5.5.17.7.51/uie/tokenizer.py` & `torch4uie-2023.5.5.17.9.31/uie/tokenizer.py`

 * *Files 0% similar despite different names*

```diff
@@ -18,15 +18,15 @@
     print(e)
     from faster_tokenizer import Tokenizer, normalizers, pretokenizers, postprocessors
     from faster_tokenizer.models import BPE, Unigram
 
 from transformers.tokenization_utils import AddedToken, PreTrainedTokenizer
 from transformers.utils import SPIECE_UNDERLINE
 
-from utils import logger
+from uie.utils import logger
 
 
 VOCAB_FILES_NAMES = {
     "sentencepiece_model_file": "sentencepiece.bpe.model",
     "vocab_file": "vocab.txt",
 }
```

### Comparing `torch4uie-2023.5.5.17.7.51/uie/uie.py` & `torch4uie-2023.5.5.17.9.31/uie/uie.py`

 * *Files identical despite different names*

### Comparing `torch4uie-2023.5.5.17.7.51/uie/utils.py` & `torch4uie-2023.5.5.17.9.31/uie/utils.py`

 * *Files identical despite different names*

