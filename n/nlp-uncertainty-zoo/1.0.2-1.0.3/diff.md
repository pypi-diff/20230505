# Comparing `tmp/nlp-uncertainty-zoo-1.0.2.tar.gz` & `tmp/nlp-uncertainty-zoo-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/nlp-uncertainty-zoo-1.0.2.tar", last modified: Sun Apr 16 20:58:23 2023, max compression
+gzip compressed data, was "dist/nlp-uncertainty-zoo-1.0.3.tar", last modified: Fri May  5 13:18:05 2023, max compression
```

## Comparing `nlp-uncertainty-zoo-1.0.2.tar` & `nlp-uncertainty-zoo-1.0.3.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxr-xr-x   0 deul       (502) staff       (20)        0 2023-04-16 20:58:23.000000 nlp-uncertainty-zoo-1.0.2/
--rw-r--r--   0 deul       (502) staff       (20)     9743 2023-04-16 20:58:23.000000 nlp-uncertainty-zoo-1.0.2/PKG-INFO
-drwxr-xr-x   0 deul       (502) staff       (20)        0 2023-04-16 20:58:23.000000 nlp-uncertainty-zoo-1.0.2/nlp_uncertainty_zoo/
--rw-r--r--   0 deul       (502) staff       (20)     1660 2023-01-23 16:34:19.000000 nlp-uncertainty-zoo-1.0.2/nlp_uncertainty_zoo/config.py
-drwxr-xr-x   0 deul       (502) staff       (20)        0 2023-04-16 20:58:23.000000 nlp-uncertainty-zoo-1.0.2/nlp_uncertainty_zoo/tests/
--rw-r--r--   0 deul       (502) staff       (20)    12617 2023-02-27 11:18:06.000000 nlp-uncertainty-zoo-1.0.2/nlp_uncertainty_zoo/tests/test_module_functions.py
--rw-r--r--   0 deul       (502) staff       (20)        0 2022-02-14 17:08:56.000000 nlp-uncertainty-zoo-1.0.2/nlp_uncertainty_zoo/tests/__init__.py
--rw-r--r--   0 deul       (502) staff       (20)     1164 2022-10-28 15:35:55.000000 nlp-uncertainty-zoo-1.0.2/nlp_uncertainty_zoo/__init__.py
-drwxr-xr-x   0 deul       (502) staff       (20)        0 2023-04-16 20:58:23.000000 nlp-uncertainty-zoo-1.0.2/nlp_uncertainty_zoo/utils/
--rw-r--r--   0 deul       (502) staff       (20)     3801 2022-05-25 13:35:12.000000 nlp-uncertainty-zoo-1.0.2/nlp_uncertainty_zoo/utils/metrics.py
--rw-r--r--   0 deul       (502) staff       (20)     2905 2023-02-27 11:18:06.000000 nlp-uncertainty-zoo-1.0.2/nlp_uncertainty_zoo/utils/task_eval.py
--rw-r--r--   0 deul       (502) staff       (20)        0 2022-02-14 17:08:56.000000 nlp-uncertainty-zoo-1.0.2/nlp_uncertainty_zoo/utils/__init__.py
--rw-r--r--   0 deul       (502) staff       (20)    12005 2023-02-27 11:18:06.000000 nlp-uncertainty-zoo-1.0.2/nlp_uncertainty_zoo/utils/calibration_eval.py
--rw-r--r--   0 deul       (502) staff       (20)      320 2023-02-27 11:18:06.000000 nlp-uncertainty-zoo-1.0.2/nlp_uncertainty_zoo/utils/custom_types.py
--rw-r--r--   0 deul       (502) staff       (20)    11899 2023-02-27 11:18:06.000000 nlp-uncertainty-zoo-1.0.2/nlp_uncertainty_zoo/utils/uncertainty_eval.py
--rw-rw-rw-   0 deul       (502) staff       (20)    19782 2022-03-29 13:22:55.000000 nlp-uncertainty-zoo-1.0.2/nlp_uncertainty_zoo/utils/samplers.py
--rw-r--r--   0 deul       (502) staff       (20)    15253 2023-02-27 14:49:13.000000 nlp-uncertainty-zoo-1.0.2/nlp_uncertainty_zoo/utils/data.py
-drwxr-xr-x   0 deul       (502) staff       (20)        0 2023-04-16 20:58:23.000000 nlp-uncertainty-zoo-1.0.2/nlp_uncertainty_zoo/models/
--rw-r--r--   0 deul       (502) staff       (20)    21413 2023-04-16 20:54:39.000000 nlp-uncertainty-zoo-1.0.2/nlp_uncertainty_zoo/models/ddu_transformer.py
--rw-r--r--   0 deul       (502) staff       (20)    15262 2023-02-27 11:18:06.000000 nlp-uncertainty-zoo-1.0.2/nlp_uncertainty_zoo/models/dpp_transformer.py
--rw-r--r--   0 deul       (502) staff       (20)     9369 2023-02-27 11:18:06.000000 nlp-uncertainty-zoo-1.0.2/nlp_uncertainty_zoo/models/st_tau_lstm.py
--rw-r--r--   0 deul       (502) staff       (20)    17167 2023-02-27 11:18:06.000000 nlp-uncertainty-zoo-1.0.2/nlp_uncertainty_zoo/models/lstm_ensemble.py
--rw-r--r--   0 deul       (502) staff       (20)    13935 2023-02-27 11:18:06.000000 nlp-uncertainty-zoo-1.0.2/nlp_uncertainty_zoo/models/variational_transformer.py
--rw-r--r--   0 deul       (502) staff       (20)     8219 2023-02-27 11:18:06.000000 nlp-uncertainty-zoo-1.0.2/nlp_uncertainty_zoo/models/bayesian_lstm.py
--rw-r--r--   0 deul       (502) staff       (20)     1093 2022-07-06 16:02:58.000000 nlp-uncertainty-zoo-1.0.2/nlp_uncertainty_zoo/models/__init__.py
--rw-r--r--   0 deul       (502) staff       (20)    24054 2023-02-27 11:18:06.000000 nlp-uncertainty-zoo-1.0.2/nlp_uncertainty_zoo/models/model.py
--rw-r--r--   0 deul       (502) staff       (20)    30916 2023-02-27 11:18:06.000000 nlp-uncertainty-zoo-1.0.2/nlp_uncertainty_zoo/models/sngp_transformer.py
--rw-r--r--   0 deul       (502) staff       (20)    10296 2023-02-27 11:18:06.000000 nlp-uncertainty-zoo-1.0.2/nlp_uncertainty_zoo/models/transformer.py
--rw-r--r--   0 deul       (502) staff       (20)    10731 2023-02-27 11:18:06.000000 nlp-uncertainty-zoo-1.0.2/nlp_uncertainty_zoo/models/spectral.py
--rw-r--r--   0 deul       (502) staff       (20)    14223 2023-02-27 11:18:06.000000 nlp-uncertainty-zoo-1.0.2/nlp_uncertainty_zoo/models/lstm.py
--rw-r--r--   0 deul       (502) staff       (20)    11830 2023-02-27 11:18:06.000000 nlp-uncertainty-zoo-1.0.2/nlp_uncertainty_zoo/models/bert.py
--rw-r--r--   0 deul       (502) staff       (20)    18963 2023-02-27 11:18:06.000000 nlp-uncertainty-zoo-1.0.2/nlp_uncertainty_zoo/models/variational_lstm.py
--rw-r--r--   0 deul       (502) staff       (20)    24659 2023-02-27 11:18:06.000000 nlp-uncertainty-zoo-1.0.2/nlp_uncertainty_zoo/defaults.py
-drwxr-xr-x   0 deul       (502) staff       (20)        0 2023-04-16 20:58:23.000000 nlp-uncertainty-zoo-1.0.2/nlp_uncertainty_zoo.egg-info/
--rw-r--r--   0 deul       (502) staff       (20)     9743 2023-04-16 20:58:23.000000 nlp-uncertainty-zoo-1.0.2/nlp_uncertainty_zoo.egg-info/PKG-INFO
--rw-r--r--   0 deul       (502) staff       (20)     1331 2023-04-16 20:58:23.000000 nlp-uncertainty-zoo-1.0.2/nlp_uncertainty_zoo.egg-info/SOURCES.txt
--rw-r--r--   0 deul       (502) staff       (20)      262 2023-04-16 20:58:23.000000 nlp-uncertainty-zoo-1.0.2/nlp_uncertainty_zoo.egg-info/requires.txt
--rw-r--r--   0 deul       (502) staff       (20)       20 2023-04-16 20:58:23.000000 nlp-uncertainty-zoo-1.0.2/nlp_uncertainty_zoo.egg-info/top_level.txt
--rw-r--r--   0 deul       (502) staff       (20)        1 2023-04-16 20:58:23.000000 nlp-uncertainty-zoo-1.0.2/nlp_uncertainty_zoo.egg-info/dependency_links.txt
--rw-r--r--   0 deul       (502) staff       (20)     8174 2023-02-27 11:21:57.000000 nlp-uncertainty-zoo-1.0.2/README.md
--rw-r--r--   0 deul       (502) staff       (20)     1141 2023-04-16 20:54:52.000000 nlp-uncertainty-zoo-1.0.2/setup.py
--rw-r--r--   0 deul       (502) staff       (20)       38 2023-04-16 20:58:23.000000 nlp-uncertainty-zoo-1.0.2/setup.cfg
+drwxr-xr-x   0 deul       (502) staff       (20)        0 2023-05-05 13:18:05.000000 nlp-uncertainty-zoo-1.0.3/
+-rw-r--r--   0 deul       (502) staff       (20)     9743 2023-05-05 13:18:05.000000 nlp-uncertainty-zoo-1.0.3/PKG-INFO
+drwxr-xr-x   0 deul       (502) staff       (20)        0 2023-05-05 13:18:05.000000 nlp-uncertainty-zoo-1.0.3/nlp_uncertainty_zoo/
+-rw-r--r--   0 deul       (502) staff       (20)     1660 2023-01-23 16:34:19.000000 nlp-uncertainty-zoo-1.0.3/nlp_uncertainty_zoo/config.py
+drwxr-xr-x   0 deul       (502) staff       (20)        0 2023-05-05 13:18:05.000000 nlp-uncertainty-zoo-1.0.3/nlp_uncertainty_zoo/tests/
+-rw-r--r--   0 deul       (502) staff       (20)    12617 2023-02-27 11:18:06.000000 nlp-uncertainty-zoo-1.0.3/nlp_uncertainty_zoo/tests/test_module_functions.py
+-rw-r--r--   0 deul       (502) staff       (20)        0 2022-02-14 17:08:56.000000 nlp-uncertainty-zoo-1.0.3/nlp_uncertainty_zoo/tests/__init__.py
+-rw-r--r--   0 deul       (502) staff       (20)     1164 2022-10-28 15:35:55.000000 nlp-uncertainty-zoo-1.0.3/nlp_uncertainty_zoo/__init__.py
+drwxr-xr-x   0 deul       (502) staff       (20)        0 2023-05-05 13:18:05.000000 nlp-uncertainty-zoo-1.0.3/nlp_uncertainty_zoo/utils/
+-rw-r--r--   0 deul       (502) staff       (20)     3801 2022-05-25 13:35:12.000000 nlp-uncertainty-zoo-1.0.3/nlp_uncertainty_zoo/utils/metrics.py
+-rw-r--r--   0 deul       (502) staff       (20)     2905 2023-02-27 11:18:06.000000 nlp-uncertainty-zoo-1.0.3/nlp_uncertainty_zoo/utils/task_eval.py
+-rw-r--r--   0 deul       (502) staff       (20)        0 2022-02-14 17:08:56.000000 nlp-uncertainty-zoo-1.0.3/nlp_uncertainty_zoo/utils/__init__.py
+-rw-r--r--   0 deul       (502) staff       (20)    12005 2023-02-27 11:18:06.000000 nlp-uncertainty-zoo-1.0.3/nlp_uncertainty_zoo/utils/calibration_eval.py
+-rw-r--r--   0 deul       (502) staff       (20)      320 2023-02-27 11:18:06.000000 nlp-uncertainty-zoo-1.0.3/nlp_uncertainty_zoo/utils/custom_types.py
+-rw-r--r--   0 deul       (502) staff       (20)    11899 2023-02-27 11:18:06.000000 nlp-uncertainty-zoo-1.0.3/nlp_uncertainty_zoo/utils/uncertainty_eval.py
+-rw-rw-rw-   0 deul       (502) staff       (20)    19782 2022-03-29 13:22:55.000000 nlp-uncertainty-zoo-1.0.3/nlp_uncertainty_zoo/utils/samplers.py
+-rw-r--r--   0 deul       (502) staff       (20)    15253 2023-02-27 14:49:13.000000 nlp-uncertainty-zoo-1.0.3/nlp_uncertainty_zoo/utils/data.py
+drwxr-xr-x   0 deul       (502) staff       (20)        0 2023-05-05 13:18:05.000000 nlp-uncertainty-zoo-1.0.3/nlp_uncertainty_zoo/models/
+-rw-r--r--   0 deul       (502) staff       (20)    21467 2023-05-05 13:15:02.000000 nlp-uncertainty-zoo-1.0.3/nlp_uncertainty_zoo/models/ddu_transformer.py
+-rw-r--r--   0 deul       (502) staff       (20)    15262 2023-02-27 11:18:06.000000 nlp-uncertainty-zoo-1.0.3/nlp_uncertainty_zoo/models/dpp_transformer.py
+-rw-r--r--   0 deul       (502) staff       (20)     9369 2023-02-27 11:18:06.000000 nlp-uncertainty-zoo-1.0.3/nlp_uncertainty_zoo/models/st_tau_lstm.py
+-rw-r--r--   0 deul       (502) staff       (20)    17167 2023-02-27 11:18:06.000000 nlp-uncertainty-zoo-1.0.3/nlp_uncertainty_zoo/models/lstm_ensemble.py
+-rw-r--r--   0 deul       (502) staff       (20)    13935 2023-02-27 11:18:06.000000 nlp-uncertainty-zoo-1.0.3/nlp_uncertainty_zoo/models/variational_transformer.py
+-rw-r--r--   0 deul       (502) staff       (20)     8219 2023-02-27 11:18:06.000000 nlp-uncertainty-zoo-1.0.3/nlp_uncertainty_zoo/models/bayesian_lstm.py
+-rw-r--r--   0 deul       (502) staff       (20)     1093 2022-07-06 16:02:58.000000 nlp-uncertainty-zoo-1.0.3/nlp_uncertainty_zoo/models/__init__.py
+-rw-r--r--   0 deul       (502) staff       (20)    24054 2023-02-27 11:18:06.000000 nlp-uncertainty-zoo-1.0.3/nlp_uncertainty_zoo/models/model.py
+-rw-r--r--   0 deul       (502) staff       (20)    30916 2023-02-27 11:18:06.000000 nlp-uncertainty-zoo-1.0.3/nlp_uncertainty_zoo/models/sngp_transformer.py
+-rw-r--r--   0 deul       (502) staff       (20)    10296 2023-02-27 11:18:06.000000 nlp-uncertainty-zoo-1.0.3/nlp_uncertainty_zoo/models/transformer.py
+-rw-r--r--   0 deul       (502) staff       (20)    10731 2023-02-27 11:18:06.000000 nlp-uncertainty-zoo-1.0.3/nlp_uncertainty_zoo/models/spectral.py
+-rw-r--r--   0 deul       (502) staff       (20)    14223 2023-02-27 11:18:06.000000 nlp-uncertainty-zoo-1.0.3/nlp_uncertainty_zoo/models/lstm.py
+-rw-r--r--   0 deul       (502) staff       (20)    11830 2023-02-27 11:18:06.000000 nlp-uncertainty-zoo-1.0.3/nlp_uncertainty_zoo/models/bert.py
+-rw-r--r--   0 deul       (502) staff       (20)    18963 2023-02-27 11:18:06.000000 nlp-uncertainty-zoo-1.0.3/nlp_uncertainty_zoo/models/variational_lstm.py
+-rw-r--r--   0 deul       (502) staff       (20)    24659 2023-02-27 11:18:06.000000 nlp-uncertainty-zoo-1.0.3/nlp_uncertainty_zoo/defaults.py
+drwxr-xr-x   0 deul       (502) staff       (20)        0 2023-05-05 13:18:05.000000 nlp-uncertainty-zoo-1.0.3/nlp_uncertainty_zoo.egg-info/
+-rw-r--r--   0 deul       (502) staff       (20)     9743 2023-05-05 13:18:05.000000 nlp-uncertainty-zoo-1.0.3/nlp_uncertainty_zoo.egg-info/PKG-INFO
+-rw-r--r--   0 deul       (502) staff       (20)     1331 2023-05-05 13:18:05.000000 nlp-uncertainty-zoo-1.0.3/nlp_uncertainty_zoo.egg-info/SOURCES.txt
+-rw-r--r--   0 deul       (502) staff       (20)      262 2023-05-05 13:18:05.000000 nlp-uncertainty-zoo-1.0.3/nlp_uncertainty_zoo.egg-info/requires.txt
+-rw-r--r--   0 deul       (502) staff       (20)       20 2023-05-05 13:18:05.000000 nlp-uncertainty-zoo-1.0.3/nlp_uncertainty_zoo.egg-info/top_level.txt
+-rw-r--r--   0 deul       (502) staff       (20)        1 2023-05-05 13:18:05.000000 nlp-uncertainty-zoo-1.0.3/nlp_uncertainty_zoo.egg-info/dependency_links.txt
+-rw-r--r--   0 deul       (502) staff       (20)     8174 2023-02-27 11:21:57.000000 nlp-uncertainty-zoo-1.0.3/README.md
+-rw-r--r--   0 deul       (502) staff       (20)     1141 2023-05-05 13:15:09.000000 nlp-uncertainty-zoo-1.0.3/setup.py
+-rw-r--r--   0 deul       (502) staff       (20)       38 2023-05-05 13:18:05.000000 nlp-uncertainty-zoo-1.0.3/setup.cfg
```

### Comparing `nlp-uncertainty-zoo-1.0.2/PKG-INFO` & `nlp-uncertainty-zoo-1.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nlp-uncertainty-zoo
-Version: 1.0.2
+Version: 1.0.3
 Summary: PyTorch Implementation of Models used for Uncertainty Estimation in Natural Language Processing.
 Home-page: https://github.com/Kaleidophon/nlp-uncertainty-zoo
 Author: Dennis Ulmer
 License: GPL
 Description: # :robot::speech_balloon::question: nlp-uncertainty-zoo
         
         This repository contains implementations of several models used for uncertainty estimation in Natural Language processing,
```

### Comparing `nlp-uncertainty-zoo-1.0.2/nlp_uncertainty_zoo/config.py` & `nlp-uncertainty-zoo-1.0.3/nlp_uncertainty_zoo/config.py`

 * *Files identical despite different names*

### Comparing `nlp-uncertainty-zoo-1.0.2/nlp_uncertainty_zoo/tests/test_module_functions.py` & `nlp-uncertainty-zoo-1.0.3/nlp_uncertainty_zoo/tests/test_module_functions.py`

 * *Files identical despite different names*

### Comparing `nlp-uncertainty-zoo-1.0.2/nlp_uncertainty_zoo/__init__.py` & `nlp-uncertainty-zoo-1.0.3/nlp_uncertainty_zoo/__init__.py`

 * *Files identical despite different names*

### Comparing `nlp-uncertainty-zoo-1.0.2/nlp_uncertainty_zoo/utils/metrics.py` & `nlp-uncertainty-zoo-1.0.3/nlp_uncertainty_zoo/utils/metrics.py`

 * *Files identical despite different names*

### Comparing `nlp-uncertainty-zoo-1.0.2/nlp_uncertainty_zoo/utils/task_eval.py` & `nlp-uncertainty-zoo-1.0.3/nlp_uncertainty_zoo/utils/task_eval.py`

 * *Files identical despite different names*

### Comparing `nlp-uncertainty-zoo-1.0.2/nlp_uncertainty_zoo/utils/calibration_eval.py` & `nlp-uncertainty-zoo-1.0.3/nlp_uncertainty_zoo/utils/calibration_eval.py`

 * *Files identical despite different names*

### Comparing `nlp-uncertainty-zoo-1.0.2/nlp_uncertainty_zoo/utils/uncertainty_eval.py` & `nlp-uncertainty-zoo-1.0.3/nlp_uncertainty_zoo/utils/uncertainty_eval.py`

 * *Files identical despite different names*

### Comparing `nlp-uncertainty-zoo-1.0.2/nlp_uncertainty_zoo/utils/samplers.py` & `nlp-uncertainty-zoo-1.0.3/nlp_uncertainty_zoo/utils/samplers.py`

 * *Files identical despite different names*

### Comparing `nlp-uncertainty-zoo-1.0.2/nlp_uncertainty_zoo/utils/data.py` & `nlp-uncertainty-zoo-1.0.3/nlp_uncertainty_zoo/utils/data.py`

 * *Files identical despite different names*

### Comparing `nlp-uncertainty-zoo-1.0.2/nlp_uncertainty_zoo/models/ddu_transformer.py` & `nlp-uncertainty-zoo-1.0.3/nlp_uncertainty_zoo/models/ddu_transformer.py`

 * *Files 1% similar despite different names*

```diff
@@ -98,15 +98,15 @@
                         torch.stack([input_ids != idx for idx in self.ignore_indices]), dim=0
                     )
                     labels = labels[batch_mask]
                     hidden = hidden[batch_mask]
 
                 else:
                     hidden = (
-                        self.get_sequence_representation(hidden).squeeze(1)
+                        self.get_sequence_representation_from_hidden(hidden).squeeze(1)
                     )
 
                 hiddens.append(hidden)
                 all_labels.append(labels)
 
             hiddens = torch.cat(hiddens, dim=0)
             all_labels = torch.cat(all_labels, dim=0).to(self.device)
@@ -134,32 +134,32 @@
                 ).to(self.device) * (num_batch_classes - 1)
 
                 self.determinants[cls] = torch.det(
                     self.Sigma[cls, :, :]
                 )  # Compute determinant
                 self.Sigma[cls, :, :] = torch.linalg.inv(self.Sigma[cls, :, :])
 
-    def gmm_predict(self, input_: torch.LongTensor) -> torch.FloatTensor:
+    def gmm_predict(self, input_: torch.LongTensor, **kwargs) -> torch.FloatTensor:
         """
         Make a prediction with the Gaussian mixture Model for a batch of inputs.
 
         Parameters
         ----------
         input_: torch.LongTensor
             Batch of inputs in the form of indexed tokens.
 
         Returns
         -------
         torch.FloatTensor
             Probability of the input under every mixture component, with one component per class.
         """
         batch_size = input_.shape[0]
-        hidden = self.get_hidden_representation(input_)  # batch_size x seq_length x input_size
+        hidden = self.get_hidden_representation(input_, **kwargs)  # batch_size x seq_length x input_size
         hidden = (
-            self.get_sequence_representation(hidden).squeeze(1)
+            self.get_sequence_representation_from_hidden(hidden).squeeze(1)
             if self.is_sequence_classifier
             else rearrange(hidden, "b s i -> (b s) i")
         )
 
         if self.pca is not None:
             device = hidden.device
             hidden = torch.FloatTensor(self.pca.transform(hidden.cpu().detach().numpy())).to(device)
@@ -459,15 +459,15 @@
             Uncertainty scores for the current batch.
         """
         if metric_name is None:
             metric_name = self.default_uncertainty_metric
 
         if metric_name == "log_prob":
             with torch.no_grad():
-                return self.gmm_predict(input_)
+                return self.gmm_predict(input_, **kwargs)
 
         else:
             return super().get_uncertainty(input_, metric_name=metric_name, **kwargs)
 
 
 class DDUBert(Model):
     def __init__(
```

### Comparing `nlp-uncertainty-zoo-1.0.2/nlp_uncertainty_zoo/models/dpp_transformer.py` & `nlp-uncertainty-zoo-1.0.3/nlp_uncertainty_zoo/models/dpp_transformer.py`

 * *Files identical despite different names*

### Comparing `nlp-uncertainty-zoo-1.0.2/nlp_uncertainty_zoo/models/st_tau_lstm.py` & `nlp-uncertainty-zoo-1.0.3/nlp_uncertainty_zoo/models/st_tau_lstm.py`

 * *Files identical despite different names*

### Comparing `nlp-uncertainty-zoo-1.0.2/nlp_uncertainty_zoo/models/lstm_ensemble.py` & `nlp-uncertainty-zoo-1.0.3/nlp_uncertainty_zoo/models/lstm_ensemble.py`

 * *Files identical despite different names*

### Comparing `nlp-uncertainty-zoo-1.0.2/nlp_uncertainty_zoo/models/variational_transformer.py` & `nlp-uncertainty-zoo-1.0.3/nlp_uncertainty_zoo/models/variational_transformer.py`

 * *Files identical despite different names*

### Comparing `nlp-uncertainty-zoo-1.0.2/nlp_uncertainty_zoo/models/bayesian_lstm.py` & `nlp-uncertainty-zoo-1.0.3/nlp_uncertainty_zoo/models/bayesian_lstm.py`

 * *Files identical despite different names*

### Comparing `nlp-uncertainty-zoo-1.0.2/nlp_uncertainty_zoo/models/__init__.py` & `nlp-uncertainty-zoo-1.0.3/nlp_uncertainty_zoo/models/__init__.py`

 * *Files identical despite different names*

### Comparing `nlp-uncertainty-zoo-1.0.2/nlp_uncertainty_zoo/models/model.py` & `nlp-uncertainty-zoo-1.0.3/nlp_uncertainty_zoo/models/model.py`

 * *Files identical despite different names*

### Comparing `nlp-uncertainty-zoo-1.0.2/nlp_uncertainty_zoo/models/sngp_transformer.py` & `nlp-uncertainty-zoo-1.0.3/nlp_uncertainty_zoo/models/sngp_transformer.py`

 * *Files identical despite different names*

### Comparing `nlp-uncertainty-zoo-1.0.2/nlp_uncertainty_zoo/models/transformer.py` & `nlp-uncertainty-zoo-1.0.3/nlp_uncertainty_zoo/models/transformer.py`

 * *Files identical despite different names*

### Comparing `nlp-uncertainty-zoo-1.0.2/nlp_uncertainty_zoo/models/spectral.py` & `nlp-uncertainty-zoo-1.0.3/nlp_uncertainty_zoo/models/spectral.py`

 * *Files identical despite different names*

### Comparing `nlp-uncertainty-zoo-1.0.2/nlp_uncertainty_zoo/models/lstm.py` & `nlp-uncertainty-zoo-1.0.3/nlp_uncertainty_zoo/models/lstm.py`

 * *Files identical despite different names*

### Comparing `nlp-uncertainty-zoo-1.0.2/nlp_uncertainty_zoo/models/bert.py` & `nlp-uncertainty-zoo-1.0.3/nlp_uncertainty_zoo/models/bert.py`

 * *Files identical despite different names*

### Comparing `nlp-uncertainty-zoo-1.0.2/nlp_uncertainty_zoo/models/variational_lstm.py` & `nlp-uncertainty-zoo-1.0.3/nlp_uncertainty_zoo/models/variational_lstm.py`

 * *Files identical despite different names*

### Comparing `nlp-uncertainty-zoo-1.0.2/nlp_uncertainty_zoo/defaults.py` & `nlp-uncertainty-zoo-1.0.3/nlp_uncertainty_zoo/defaults.py`

 * *Files identical despite different names*

### Comparing `nlp-uncertainty-zoo-1.0.2/nlp_uncertainty_zoo.egg-info/PKG-INFO` & `nlp-uncertainty-zoo-1.0.3/nlp_uncertainty_zoo.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nlp-uncertainty-zoo
-Version: 1.0.2
+Version: 1.0.3
 Summary: PyTorch Implementation of Models used for Uncertainty Estimation in Natural Language Processing.
 Home-page: https://github.com/Kaleidophon/nlp-uncertainty-zoo
 Author: Dennis Ulmer
 License: GPL
 Description: # :robot::speech_balloon::question: nlp-uncertainty-zoo
         
         This repository contains implementations of several models used for uncertainty estimation in Natural Language processing,
```

### Comparing `nlp-uncertainty-zoo-1.0.2/nlp_uncertainty_zoo.egg-info/SOURCES.txt` & `nlp-uncertainty-zoo-1.0.3/nlp_uncertainty_zoo.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `nlp-uncertainty-zoo-1.0.2/README.md` & `nlp-uncertainty-zoo-1.0.3/README.md`

 * *Files identical despite different names*

### Comparing `nlp-uncertainty-zoo-1.0.2/setup.py` & `nlp-uncertainty-zoo-1.0.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     long_description = fh.read()
 
 with open("requirements.txt") as f:
     required = [line for line in f.read().splitlines() if not line.startswith("git")]
 
 setup(
     name="nlp-uncertainty-zoo",
-    version="1.0.2",
+    version="1.0.3",
     author="Dennis Ulmer",
     description="PyTorch Implementation of Models used for Uncertainty Estimation in Natural Language Processing.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/Kaleidophon/nlp-uncertainty-zoo",
     classifiers=[
         "Intended Audience :: Science/Research",
```

