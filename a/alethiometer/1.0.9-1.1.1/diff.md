# Comparing `tmp/alethiometer-1.0.9.tar.gz` & `tmp/alethiometer-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "alethiometer-1.0.9.tar", last modified: Fri Apr 28 22:29:29 2023, max compression
+gzip compressed data, was "alethiometer-1.1.1.tar", last modified: Fri May  5 16:17:07 2023, max compression
```

## Comparing `alethiometer-1.0.9.tar` & `alethiometer-1.1.1.tar`

### file list

```diff
@@ -1,36 +1,39 @@
-drwxrwxr-x   0 u2280887  (1000) u2280887  (1000)        0 2023-04-28 22:29:29.938750 alethiometer-1.0.9/
--rw-rw-r--   0 u2280887  (1000) u2280887  (1000)    11357 2023-04-07 16:49:02.000000 alethiometer-1.0.9/LICENSE
--rw-rw-r--   0 u2280887  (1000) u2280887  (1000)     7068 2023-04-28 22:29:29.934750 alethiometer-1.0.9/PKG-INFO
--rw-rw-r--   0 u2280887  (1000) u2280887  (1000)     6358 2023-04-28 22:29:04.000000 alethiometer-1.0.9/README.md
-drwxrwxr-x   0 u2280887  (1000) u2280887  (1000)        0 2023-04-28 22:29:29.934750 alethiometer-1.0.9/alethiometer/
--rw-rw-r--   0 u2280887  (1000) u2280887  (1000)      313 2023-04-11 12:10:43.000000 alethiometer-1.0.9/alethiometer/__init__.py
--rw-rw-r--   0 u2280887  (1000) u2280887  (1000)      245 2023-04-28 22:28:17.000000 alethiometer-1.0.9/alethiometer/__version__.py
-drwxrwxr-x   0 u2280887  (1000) u2280887  (1000)        0 2023-04-28 22:29:29.934750 alethiometer-1.0.9/alethiometer/datasets/
--rw-rw-r--   0 u2280887  (1000) u2280887  (1000)      254 2023-04-07 17:54:55.000000 alethiometer-1.0.9/alethiometer/datasets/__init__.py
--rw-rw-r--   0 u2280887  (1000) u2280887  (1000)     4853 2023-04-17 13:10:20.000000 alethiometer-1.0.9/alethiometer/datasets/dataset.py
--rw-rw-r--   0 u2280887  (1000) u2280887  (1000)     2174 2023-04-07 17:54:22.000000 alethiometer-1.0.9/alethiometer/datasets/h5py_dataset.py
--rw-rw-r--   0 u2280887  (1000) u2280887  (1000)     5109 2023-04-07 17:55:28.000000 alethiometer-1.0.9/alethiometer/datasets/imagenet16.py
--rw-rw-r--   0 u2280887  (1000) u2280887  (1000)     1077 2023-04-07 15:01:32.000000 alethiometer-1.0.9/alethiometer/utils.py
--rw-rw-r--   0 u2280887  (1000) u2280887  (1000)     4968 2023-04-28 22:17:58.000000 alethiometer-1.0.9/alethiometer/zc_proxy.py
-drwxrwxr-x   0 u2280887  (1000) u2280887  (1000)        0 2023-04-28 22:29:29.934750 alethiometer-1.0.9/alethiometer/zero_cost_metrics/
--rw-rw-r--   0 u2280887  (1000) u2280887  (1000)     1660 2023-04-28 21:23:03.000000 alethiometer-1.0.9/alethiometer/zero_cost_metrics/__init__.py
--rw-rw-r--   0 u2280887  (1000) u2280887  (1000)     1475 2023-04-07 17:10:09.000000 alethiometer-1.0.9/alethiometer/zero_cost_metrics/grad_norm.py
--rw-rw-r--   0 u2280887  (1000) u2280887  (1000)     3624 2023-04-07 17:13:08.000000 alethiometer-1.0.9/alethiometer/zero_cost_metrics/grasp.py
--rw-rw-r--   0 u2280887  (1000) u2280887  (1000)     2926 2023-04-11 16:57:48.000000 alethiometer-1.0.9/alethiometer/zero_cost_metrics/naswot.py
--rw-rw-r--   0 u2280887  (1000) u2280887  (1000)     2079 2023-04-28 20:46:05.000000 alethiometer-1.0.9/alethiometer/zero_cost_metrics/naswot_relu.py
--rw-rw-r--   0 u2280887  (1000) u2280887  (1000)     2023 2023-04-07 17:09:49.000000 alethiometer-1.0.9/alethiometer/zero_cost_metrics/snip.py
--rw-rw-r--   0 u2280887  (1000) u2280887  (1000)     1928 2023-04-07 17:06:05.000000 alethiometer-1.0.9/alethiometer/zero_cost_metrics/synflow.py
--rw-rw-r--   0 u2280887  (1000) u2280887  (1000)    15593 2023-04-28 22:16:08.000000 alethiometer-1.0.9/alethiometer/zero_cost_metrics/tenas.py
--rw-rw-r--   0 u2280887  (1000) u2280887  (1000)     3420 2023-04-28 21:42:23.000000 alethiometer-1.0.9/alethiometer/zero_cost_metrics/zen.py
--rw-rw-r--   0 u2280887  (1000) u2280887  (1000)     2412 2023-04-23 12:05:26.000000 alethiometer-1.0.9/alethiometer/zero_cost_metrics/zico.py
-drwxrwxr-x   0 u2280887  (1000) u2280887  (1000)        0 2023-04-28 22:29:29.934750 alethiometer-1.0.9/alethiometer.egg-info/
--rw-rw-r--   0 u2280887  (1000) u2280887  (1000)     7068 2023-04-28 22:29:29.000000 alethiometer-1.0.9/alethiometer.egg-info/PKG-INFO
--rw-rw-r--   0 u2280887  (1000) u2280887  (1000)      898 2023-04-28 22:29:29.000000 alethiometer-1.0.9/alethiometer.egg-info/SOURCES.txt
--rw-rw-r--   0 u2280887  (1000) u2280887  (1000)        1 2023-04-28 22:29:29.000000 alethiometer-1.0.9/alethiometer.egg-info/dependency_links.txt
--rw-rw-r--   0 u2280887  (1000) u2280887  (1000)       37 2023-04-28 22:29:29.000000 alethiometer-1.0.9/alethiometer.egg-info/requires.txt
--rw-rw-r--   0 u2280887  (1000) u2280887  (1000)       13 2023-04-28 22:29:29.000000 alethiometer-1.0.9/alethiometer.egg-info/top_level.txt
--rw-rw-r--   0 u2280887  (1000) u2280887  (1000)       38 2023-04-28 22:29:29.938750 alethiometer-1.0.9/setup.cfg
--rw-rw-r--   0 u2280887  (1000) u2280887  (1000)     6031 2023-04-07 18:04:03.000000 alethiometer-1.0.9/setup.py
-drwxrwxr-x   0 u2280887  (1000) u2280887  (1000)        0 2023-04-28 22:29:29.934750 alethiometer-1.0.9/tests/
--rw-rw-r--   0 u2280887  (1000) u2280887  (1000)     1219 2023-04-25 09:05:55.000000 alethiometer-1.0.9/tests/test_nwot_api.py
--rw-rw-r--   0 u2280887  (1000) u2280887  (1000)     3098 2023-04-28 22:20:47.000000 alethiometer-1.0.9/tests/test_zc.py
+drwxrwxr-x   0 u2280887  (1000) u2280887  (1000)        0 2023-05-05 16:17:07.432465 alethiometer-1.1.1/
+-rw-rw-r--   0 u2280887  (1000) u2280887  (1000)    11357 2023-04-07 16:49:02.000000 alethiometer-1.1.1/LICENSE
+-rw-rw-r--   0 u2280887  (1000) u2280887  (1000)     8965 2023-05-05 16:17:07.432465 alethiometer-1.1.1/PKG-INFO
+-rw-rw-r--   0 u2280887  (1000) u2280887  (1000)     8255 2023-05-05 16:15:51.000000 alethiometer-1.1.1/README.md
+drwxrwxr-x   0 u2280887  (1000) u2280887  (1000)        0 2023-05-05 16:17:07.428465 alethiometer-1.1.1/alethiometer/
+-rw-rw-r--   0 u2280887  (1000) u2280887  (1000)      313 2023-04-11 12:10:43.000000 alethiometer-1.1.1/alethiometer/__init__.py
+-rw-rw-r--   0 u2280887  (1000) u2280887  (1000)      245 2023-05-05 16:15:55.000000 alethiometer-1.1.1/alethiometer/__version__.py
+drwxrwxr-x   0 u2280887  (1000) u2280887  (1000)        0 2023-05-05 16:17:07.428465 alethiometer-1.1.1/alethiometer/datasets/
+-rw-rw-r--   0 u2280887  (1000) u2280887  (1000)      254 2023-04-07 17:54:55.000000 alethiometer-1.1.1/alethiometer/datasets/__init__.py
+-rw-rw-r--   0 u2280887  (1000) u2280887  (1000)     4853 2023-04-17 13:10:20.000000 alethiometer-1.1.1/alethiometer/datasets/dataset.py
+-rw-rw-r--   0 u2280887  (1000) u2280887  (1000)     2174 2023-04-07 17:54:22.000000 alethiometer-1.1.1/alethiometer/datasets/h5py_dataset.py
+-rw-rw-r--   0 u2280887  (1000) u2280887  (1000)     5109 2023-04-07 17:55:28.000000 alethiometer-1.1.1/alethiometer/datasets/imagenet16.py
+-rw-rw-r--   0 u2280887  (1000) u2280887  (1000)     1077 2023-04-07 15:01:32.000000 alethiometer-1.1.1/alethiometer/utils.py
+-rw-rw-r--   0 u2280887  (1000) u2280887  (1000)     5512 2023-05-01 09:09:45.000000 alethiometer-1.1.1/alethiometer/zc_proxy.py
+drwxrwxr-x   0 u2280887  (1000) u2280887  (1000)        0 2023-05-05 16:17:07.432465 alethiometer-1.1.1/alethiometer/zero_cost_metrics/
+-rw-rw-r--   0 u2280887  (1000) u2280887  (1000)     1734 2023-04-30 15:50:05.000000 alethiometer-1.1.1/alethiometer/zero_cost_metrics/__init__.py
+-rw-rw-r--   0 u2280887  (1000) u2280887  (1000)     1475 2023-04-07 17:10:09.000000 alethiometer-1.1.1/alethiometer/zero_cost_metrics/grad_norm.py
+-rw-rw-r--   0 u2280887  (1000) u2280887  (1000)     3624 2023-04-07 17:13:08.000000 alethiometer-1.1.1/alethiometer/zero_cost_metrics/grasp.py
+-rw-rw-r--   0 u2280887  (1000) u2280887  (1000)     2926 2023-04-11 16:57:48.000000 alethiometer-1.1.1/alethiometer/zero_cost_metrics/naswot.py
+-rw-rw-r--   0 u2280887  (1000) u2280887  (1000)     2079 2023-04-28 20:46:05.000000 alethiometer-1.1.1/alethiometer/zero_cost_metrics/naswot_relu.py
+-rw-rw-r--   0 u2280887  (1000) u2280887  (1000)     2023 2023-04-07 17:09:49.000000 alethiometer-1.1.1/alethiometer/zero_cost_metrics/snip.py
+-rw-rw-r--   0 u2280887  (1000) u2280887  (1000)     1928 2023-04-07 17:06:05.000000 alethiometer-1.1.1/alethiometer/zero_cost_metrics/synflow.py
+-rw-rw-r--   0 u2280887  (1000) u2280887  (1000)     5830 2023-05-05 16:11:36.000000 alethiometer-1.1.1/alethiometer/zero_cost_metrics/t_cet.py
+-rw-rw-r--   0 u2280887  (1000) u2280887  (1000)    16377 2023-05-04 11:20:27.000000 alethiometer-1.1.1/alethiometer/zero_cost_metrics/tenas.py
+-rw-rw-r--   0 u2280887  (1000) u2280887  (1000)     3420 2023-04-28 21:42:23.000000 alethiometer-1.1.1/alethiometer/zero_cost_metrics/zen.py
+-rw-rw-r--   0 u2280887  (1000) u2280887  (1000)     4522 2023-05-01 21:46:32.000000 alethiometer-1.1.1/alethiometer/zero_cost_metrics/zico.py
+drwxrwxr-x   0 u2280887  (1000) u2280887  (1000)        0 2023-05-05 16:17:07.428465 alethiometer-1.1.1/alethiometer.egg-info/
+-rw-rw-r--   0 u2280887  (1000) u2280887  (1000)     8965 2023-05-05 16:17:07.000000 alethiometer-1.1.1/alethiometer.egg-info/PKG-INFO
+-rw-rw-r--   0 u2280887  (1000) u2280887  (1000)      976 2023-05-05 16:17:07.000000 alethiometer-1.1.1/alethiometer.egg-info/SOURCES.txt
+-rw-rw-r--   0 u2280887  (1000) u2280887  (1000)        1 2023-05-05 16:17:07.000000 alethiometer-1.1.1/alethiometer.egg-info/dependency_links.txt
+-rw-rw-r--   0 u2280887  (1000) u2280887  (1000)       37 2023-05-05 16:17:07.000000 alethiometer-1.1.1/alethiometer.egg-info/requires.txt
+-rw-rw-r--   0 u2280887  (1000) u2280887  (1000)       13 2023-05-05 16:17:07.000000 alethiometer-1.1.1/alethiometer.egg-info/top_level.txt
+-rw-rw-r--   0 u2280887  (1000) u2280887  (1000)       38 2023-05-05 16:17:07.432465 alethiometer-1.1.1/setup.cfg
+-rw-rw-r--   0 u2280887  (1000) u2280887  (1000)     6031 2023-04-07 18:04:03.000000 alethiometer-1.1.1/setup.py
+drwxrwxr-x   0 u2280887  (1000) u2280887  (1000)        0 2023-05-05 16:17:07.432465 alethiometer-1.1.1/tests/
+-rw-rw-r--   0 u2280887  (1000) u2280887  (1000)     1219 2023-04-25 09:05:55.000000 alethiometer-1.1.1/tests/test_nwot_api.py
+-rw-rw-r--   0 u2280887  (1000) u2280887  (1000)     1946 2023-04-30 16:15:53.000000 alethiometer-1.1.1/tests/test_tcet.py
+-rw-rw-r--   0 u2280887  (1000) u2280887  (1000)     3355 2023-04-29 09:46:22.000000 alethiometer-1.1.1/tests/test_zc.py
+-rw-rw-r--   0 u2280887  (1000) u2280887  (1000)     1319 2023-05-01 11:23:22.000000 alethiometer-1.1.1/tests/test_zico.py
```

### Comparing `alethiometer-1.0.9/LICENSE` & `alethiometer-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `alethiometer-1.0.9/alethiometer/datasets/dataset.py` & `alethiometer-1.1.1/alethiometer/datasets/dataset.py`

 * *Files identical despite different names*

### Comparing `alethiometer-1.0.9/alethiometer/datasets/h5py_dataset.py` & `alethiometer-1.1.1/alethiometer/datasets/h5py_dataset.py`

 * *Files identical despite different names*

### Comparing `alethiometer-1.0.9/alethiometer/datasets/imagenet16.py` & `alethiometer-1.1.1/alethiometer/datasets/imagenet16.py`

 * *Files identical despite different names*

### Comparing `alethiometer-1.0.9/alethiometer/utils.py` & `alethiometer-1.1.1/alethiometer/utils.py`

 * *Files identical despite different names*

### Comparing `alethiometer-1.0.9/alethiometer/zc_proxy.py` & `alethiometer-1.1.1/alethiometer/zc_proxy.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 '''
 Author: ViolinSolo
 Date: 2023-04-06 18:35:04
-LastEditTime: 2023-04-28 23:16:16
+LastEditTime: 2023-04-29 09:27:24
 LastEditors: ViolinSolo
 Description: entry program
 FilePath: /zero-cost-proxies/alethiometer/zc_proxy.py
 '''
 import types
 import copy
 import torch
@@ -32,14 +32,35 @@
     'snip',         # snip
     'synflow',      # synflow
     'synflow_bn',   # synflow with bn
     'zen',          # ZenNAS: https://github.com/idstcv/ZenNAS/blob/main/ZeroShotProxy/compute_zen_score.py
     'tenas',        # tenas.py contains three metrics: lrn, ntk, tenas
     'ntk',          # NTK
     'lrn',          # LRN
+    'zico',         # ZICO
+    'tcet',         # TCET ========================
+    'tcet_snip_none',
+    'tcet_snip_log',
+    'tcet_snip_log1p',
+    'tcet_snip_norm',
+    'tcet_syn_none',
+    'tcet_syn_log',
+    'tcet_syn_log1p',
+    'tcet_syn_norm',# TCET ========================
+    'snr_snip',     # SNR ========================
+    'snr_syn',
+    'snr_snip_none',
+    'snr_snip_log',
+    'snr_snip_log1p',
+    'snr_snip_norm',
+    'snr_syn_none',
+    'snr_syn_log',
+    'snr_syn_log1p',
+    'snr_syn_norm', # SNR ========================
+
 ]
 
 def no_op(self, x):
     return x
 
 def copynet(self, bn):
     net = copy.deepcopy(self)
```

### Comparing `alethiometer-1.0.9/alethiometer/zero_cost_metrics/__init__.py` & `alethiometer-1.1.1/alethiometer/zero_cost_metrics/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 '''
 Author: ViolinSolo
 Date: 2023-04-06 17:43:34
-LastEditTime: 2023-04-28 21:48:59
+LastEditTime: 2023-04-30 16:48:30
 LastEditors: ViolinSolo
 Description: init files 
 FilePath: /zero-cost-proxies/alethiometer/zero_cost_metrics/__init__.py
 '''
 
 import gc
 import torch
@@ -47,7 +47,9 @@
 from . import synflow
 from . import grasp
 from . import grad_norm
 from . import naswot # this is our NASWOT implementation (layer-wise or not, based on conv and fc)
 from . import naswot_relu  # this is original RELU based NASWOT implementation
 from . import zen 
 from . import tenas # this is TENAS implementation, including lrn, ntk, tenas
+from . import zico
+from . import t_cet # this is our t_cet implementation
```

### Comparing `alethiometer-1.0.9/alethiometer/zero_cost_metrics/grad_norm.py` & `alethiometer-1.1.1/alethiometer/zero_cost_metrics/grad_norm.py`

 * *Files identical despite different names*

### Comparing `alethiometer-1.0.9/alethiometer/zero_cost_metrics/grasp.py` & `alethiometer-1.1.1/alethiometer/zero_cost_metrics/grasp.py`

 * *Files identical despite different names*

### Comparing `alethiometer-1.0.9/alethiometer/zero_cost_metrics/naswot.py` & `alethiometer-1.1.1/alethiometer/zero_cost_metrics/naswot.py`

 * *Files identical despite different names*

### Comparing `alethiometer-1.0.9/alethiometer/zero_cost_metrics/naswot_relu.py` & `alethiometer-1.1.1/alethiometer/zero_cost_metrics/naswot_relu.py`

 * *Files identical despite different names*

### Comparing `alethiometer-1.0.9/alethiometer/zero_cost_metrics/snip.py` & `alethiometer-1.1.1/alethiometer/zero_cost_metrics/snip.py`

 * *Files identical despite different names*

### Comparing `alethiometer-1.0.9/alethiometer/zero_cost_metrics/synflow.py` & `alethiometer-1.1.1/alethiometer/zero_cost_metrics/synflow.py`

 * *Files identical despite different names*

### Comparing `alethiometer-1.0.9/alethiometer/zero_cost_metrics/tenas.py` & `alethiometer-1.1.1/alethiometer/zero_cost_metrics/tenas.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 '''
 Author: ViolinSolo
 Date: 2023-04-28 17:26:50
-LastEditTime: 2023-04-28 23:15:23
+LastEditTime: 2023-05-04 12:20:27
 LastEditors: ViolinSolo
 Description: TENAS score computation
-FilePath: /zero-cost-proxies/alethiometer/zero_cost_metrics/tenas.py
+FilePath: /zero-cost-test/home/u2280887/GitHub/zero-cost-proxies/alethiometer/zero_cost_metrics/tenas.py
 '''
 '''
 Copyright (C) 2010-2021 Alibaba Group Holding Limited.
 This file is modified from:
 https://github.com/VITA-Group/TENAS
 ------------------------------------------------------------
 modified by ViolinSolo from 
@@ -288,15 +288,27 @@
                     torch.cuda.empty_cache()
 
     ######
     grads = [torch.stack(_grads, 0) for _grads in grads]
     ntks = [torch.einsum('nc,mc->nm', [_grads, _grads]) for _grads in grads]
     conds = []
     for ntk in ntks:
-        eigenvalues, _ = torch.symeig(ntk)  # ascending
+        # eigenvalues, _ = torch.symeig(ntk)  # ascending
+        """ using following code to replace torch.symeig, because of the following warning:
+        UserWarning: torch.symeig is deprecated in favor of torch.linalg.eigh and will be removed in a future PyTorch release.
+        The default behavior has changed from using the upper triangular portion of the matrix by default to using the lower triangular portion.
+        L, _ = torch.symeig(A, upper=upper)
+        should be replaced with
+        L = torch.linalg.eigvalsh(A, UPLO='U' if upper else 'L')
+        and
+        L, V = torch.symeig(A, eigenvectors=True)
+        should be replaced with
+        L, V = torch.linalg.eigh(A, UPLO='U' if upper else 'L')
+        """
+        eigenvalues = torch.linalg.eigvalsh(ntk, UPLO='U') # ascending
         # conds.append(np.nan_to_num((eigenvalues[-1] / eigenvalues[0]).item(), copy=True, nan=100000.0))
         conds.append(np.nan_to_num((eigenvalues[-1] / eigenvalues[0]).item(), copy=True))
     return conds
 
 
 @metric('ntk', bn=True, num_batch=1)
 def compute_NTK_score(net: nn.Module, inputs, targets, split_data=1, loss_fn=None,  # these are necessary arguments limited by *zero_cost_metrics.__init__.calc_metric*, if you want to add more arguments, modify @metric decorator's parameters to provide dynamic default values.
```

### Comparing `alethiometer-1.0.9/alethiometer/zero_cost_metrics/zen.py` & `alethiometer-1.1.1/alethiometer/zero_cost_metrics/zen.py`

 * *Files identical despite different names*

### Comparing `alethiometer-1.0.9/alethiometer.egg-info/SOURCES.txt` & `alethiometer-1.1.1/alethiometer.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -17,12 +17,15 @@
 alethiometer/zero_cost_metrics/__init__.py
 alethiometer/zero_cost_metrics/grad_norm.py
 alethiometer/zero_cost_metrics/grasp.py
 alethiometer/zero_cost_metrics/naswot.py
 alethiometer/zero_cost_metrics/naswot_relu.py
 alethiometer/zero_cost_metrics/snip.py
 alethiometer/zero_cost_metrics/synflow.py
+alethiometer/zero_cost_metrics/t_cet.py
 alethiometer/zero_cost_metrics/tenas.py
 alethiometer/zero_cost_metrics/zen.py
 alethiometer/zero_cost_metrics/zico.py
 tests/test_nwot_api.py
-tests/test_zc.py
+tests/test_tcet.py
+tests/test_zc.py
+tests/test_zico.py
```

### Comparing `alethiometer-1.0.9/setup.py` & `alethiometer-1.1.1/setup.py`

 * *Files identical despite different names*

### Comparing `alethiometer-1.0.9/tests/test_nwot_api.py` & `alethiometer-1.1.1/tests/test_nwot_api.py`

 * *Files identical despite different names*

### Comparing `alethiometer-1.0.9/tests/test_zc.py` & `alethiometer-1.1.1/tests/test_zc.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 '''
 Author: ViolinSolo
 Date: 2023-04-07 19:25:08
-LastEditTime: 2023-04-28 23:18:57
+LastEditTime: 2023-04-29 10:45:56
 LastEditors: ViolinSolo
 Description: Test zc-proxies.
 FilePath: /zero-cost-proxies/tests/test_zc.py
 '''
 
 def test_dataloader():
     """
@@ -77,12 +77,19 @@
     
     if not hasattr(net, 'forward_before_global_avg_pool'):
         net.forward_before_global_avg_pool = types.MethodType(forward_pre_GAP, net)
 
     results = calc_zc_metrics(metrics=['zen'], model=net, train_queue=train_loader, device=device, aggregate=True)
     print(results)
 
+    # ==================== test zico ====================
+    # test zico
+    print('-'*20)
+    print('test zico .....')
+
+    results = calc_zc_metrics(metrics=['zico'], model=net, train_queue=train_loader, device=device, aggregate=True)
+    print(results)
 
 
 if __name__ == "__main__":
     test_dataloader()
     test_zc_proxies()
```

