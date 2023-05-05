# Comparing `tmp/TorchEase-0.0.1.tar.gz` & `tmp/TorchEase-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "TorchEase-0.0.1.tar", last modified: Fri May  5 15:16:04 2023, max compression
+gzip compressed data, was "TorchEase-0.0.2.tar", last modified: Fri May  5 15:37:58 2023, max compression
```

## Comparing `TorchEase-0.0.1.tar` & `TorchEase-0.0.2.tar`

### file list

```diff
@@ -1,16 +1,17 @@
-drwxrwxr-x   0 broxy     (1000) broxy     (1000)        0 2023-05-05 15:16:04.776245 TorchEase-0.0.1/
--rw-rw-r--   0 broxy     (1000) broxy     (1000)     1006 2023-05-05 15:16:04.772245 TorchEase-0.0.1/PKG-INFO
-drwxrwxr-x   0 broxy     (1000) broxy     (1000)        0 2023-05-05 15:16:04.772245 TorchEase-0.0.1/TorchEase/
--rw-rw-r--   0 broxy     (1000) broxy     (1000)      213 2023-05-05 15:15:14.000000 TorchEase-0.0.1/TorchEase/__init__.py
--rw-rw-r--   0 broxy     (1000) broxy     (1000)     6900 2023-05-05 11:31:46.000000 TorchEase-0.0.1/TorchEase/fuser.py
--rw-rw-r--   0 broxy     (1000) broxy     (1000)     3185 2023-05-05 11:37:01.000000 TorchEase-0.0.1/TorchEase/modelbase.py
--rw-rw-r--   0 broxy     (1000) broxy     (1000)     8303 2023-05-05 12:06:29.000000 TorchEase-0.0.1/TorchEase/trainer.py
--rw-rw-r--   0 broxy     (1000) broxy     (1000)     2107 2023-05-05 12:09:09.000000 TorchEase-0.0.1/TorchEase/user.py
--rw-rw-r--   0 broxy     (1000) broxy     (1000)     1733 2023-05-05 12:06:08.000000 TorchEase-0.0.1/TorchEase/utilities.py
-drwxrwxr-x   0 broxy     (1000) broxy     (1000)        0 2023-05-05 15:16:04.772245 TorchEase-0.0.1/TorchEase.egg-info/
--rw-rw-r--   0 broxy     (1000) broxy     (1000)     1006 2023-05-05 15:16:04.000000 TorchEase-0.0.1/TorchEase.egg-info/PKG-INFO
--rw-rw-r--   0 broxy     (1000) broxy     (1000)      266 2023-05-05 15:16:04.000000 TorchEase-0.0.1/TorchEase.egg-info/SOURCES.txt
--rw-rw-r--   0 broxy     (1000) broxy     (1000)        1 2023-05-05 15:16:04.000000 TorchEase-0.0.1/TorchEase.egg-info/dependency_links.txt
--rw-rw-r--   0 broxy     (1000) broxy     (1000)       10 2023-05-05 15:16:04.000000 TorchEase-0.0.1/TorchEase.egg-info/top_level.txt
--rw-rw-r--   0 broxy     (1000) broxy     (1000)       38 2023-05-05 15:16:04.776245 TorchEase-0.0.1/setup.cfg
--rw-rw-r--   0 broxy     (1000) broxy     (1000)     1319 2023-05-05 15:13:29.000000 TorchEase-0.0.1/setup.py
+drwxrwxr-x   0 broxy     (1000) broxy     (1000)        0 2023-05-05 15:37:58.626500 TorchEase-0.0.2/
+-rw-rw-r--   0 broxy     (1000) broxy     (1000)     1006 2023-05-05 15:37:58.626500 TorchEase-0.0.2/PKG-INFO
+drwxrwxr-x   0 broxy     (1000) broxy     (1000)        0 2023-05-05 15:37:58.622499 TorchEase-0.0.2/TorchEase/
+-rw-rw-r--   0 broxy     (1000) broxy     (1000)      213 2023-05-05 15:15:14.000000 TorchEase-0.0.2/TorchEase/__init__.py
+-rw-rw-r--   0 broxy     (1000) broxy     (1000)     6900 2023-05-05 11:31:46.000000 TorchEase-0.0.2/TorchEase/fuser.py
+-rw-rw-r--   0 broxy     (1000) broxy     (1000)     3185 2023-05-05 11:37:01.000000 TorchEase-0.0.2/TorchEase/modelbase.py
+-rw-rw-r--   0 broxy     (1000) broxy     (1000)     8253 2023-05-05 15:30:58.000000 TorchEase-0.0.2/TorchEase/trainer.py
+-rw-rw-r--   0 broxy     (1000) broxy     (1000)     2107 2023-05-05 12:09:09.000000 TorchEase-0.0.2/TorchEase/user.py
+-rw-rw-r--   0 broxy     (1000) broxy     (1000)     1733 2023-05-05 12:06:08.000000 TorchEase-0.0.2/TorchEase/utilities.py
+drwxrwxr-x   0 broxy     (1000) broxy     (1000)        0 2023-05-05 15:37:58.626500 TorchEase-0.0.2/TorchEase.egg-info/
+-rw-rw-r--   0 broxy     (1000) broxy     (1000)     1006 2023-05-05 15:37:58.000000 TorchEase-0.0.2/TorchEase.egg-info/PKG-INFO
+-rw-rw-r--   0 broxy     (1000) broxy     (1000)      298 2023-05-05 15:37:58.000000 TorchEase-0.0.2/TorchEase.egg-info/SOURCES.txt
+-rw-rw-r--   0 broxy     (1000) broxy     (1000)        1 2023-05-05 15:37:58.000000 TorchEase-0.0.2/TorchEase.egg-info/dependency_links.txt
+-rw-rw-r--   0 broxy     (1000) broxy     (1000)       37 2023-05-05 15:37:58.000000 TorchEase-0.0.2/TorchEase.egg-info/requires.txt
+-rw-rw-r--   0 broxy     (1000) broxy     (1000)       10 2023-05-05 15:37:58.000000 TorchEase-0.0.2/TorchEase.egg-info/top_level.txt
+-rw-rw-r--   0 broxy     (1000) broxy     (1000)       38 2023-05-05 15:37:58.626500 TorchEase-0.0.2/setup.cfg
+-rw-rw-r--   0 broxy     (1000) broxy     (1000)     1366 2023-05-05 15:36:53.000000 TorchEase-0.0.2/setup.py
```

### Comparing `TorchEase-0.0.1/PKG-INFO` & `TorchEase-0.0.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: TorchEase
-Version: 0.0.1
+Version: 0.0.2
 Summary: Simplifying working with PyTorch
 Author: Philipp Steigerwald
 Author-email: info@b-stream.info
 Keywords: python,torch,pytorch,early stop,trainer,tensor
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `TorchEase-0.0.1/TorchEase/fuser.py` & `TorchEase-0.0.2/TorchEase/fuser.py`

 * *Files identical despite different names*

### Comparing `TorchEase-0.0.1/TorchEase/modelbase.py` & `TorchEase-0.0.2/TorchEase/modelbase.py`

 * *Files identical despite different names*

### Comparing `TorchEase-0.0.1/TorchEase/trainer.py` & `TorchEase-0.0.2/TorchEase/trainer.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 import torch
-import alive_progress
 from .modelbase import ModelBase
 class Trainer(ModelBase):
     """
     A class for training, evaluating and testing PyTorch models.
 
     Parameters
     ----------
@@ -131,15 +130,14 @@
                     self.eval_loss = self.loss_fn(prediction, target)
             self.scheduler.step(self.eval_loss)
 
     def test(self):
         """
         Tests the model on the testing dataset.
         """
-        import torchmetrics
         self.model.eval()
         self.test_target = []
         self.test_prediction = []
         with torch.no_grad():
             self.model.eval()
             for batch, (feature, target) in enumerate(self.test_loader):
                 feature, target = feature.to(self.device), target.to(self.device)
```

### Comparing `TorchEase-0.0.1/TorchEase/user.py` & `TorchEase-0.0.2/TorchEase/user.py`

 * *Files identical despite different names*

### Comparing `TorchEase-0.0.1/TorchEase/utilities.py` & `TorchEase-0.0.2/TorchEase/utilities.py`

 * *Files identical despite different names*

### Comparing `TorchEase-0.0.1/TorchEase.egg-info/PKG-INFO` & `TorchEase-0.0.2/TorchEase.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: TorchEase
-Version: 0.0.1
+Version: 0.0.2
 Summary: Simplifying working with PyTorch
 Author: Philipp Steigerwald
 Author-email: info@b-stream.info
 Keywords: python,torch,pytorch,early stop,trainer,tensor
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `TorchEase-0.0.1/setup.py` & `TorchEase-0.0.2/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 from setuptools import setup, find_packages
 import codecs
 import os
 
-VERSION = '0.0.1'
+VERSION = '0.0.2'
 DESCRIPTION = 'Simplifying working with PyTorch'
 LONG_DESCRIPTION = 'TorchEase is a Python package that simplifies working with PyTorch, a popular deep learning framework. It provides a set of easy-to-use tools for training, testing, and deploying machine learning models. TorchEase includes features like early stopping, model fusing, and model evaluation, among others, which help streamline the model development process. Additionally, TorchEase is designed to be highly modular, making it easy to integrate into existing PyTorch projects.'
 
 # Setting up
 setup(
     name="TorchEase",
     version=VERSION,
     author="Philipp Steigerwald",
     author_email="info@b-stream.info",
     description=DESCRIPTION,
     long_description_content_type="text/markdown",
     long_description=LONG_DESCRIPTION,
     packages=find_packages(),
-    install_requires=[],
+    install_requires=["scikit-learn", "matplotlib", "pandas", "torch"],
     keywords=['python', 'torch', 'pytorch', 'early stop', 'trainer', 'tensor'],
     classifiers=[
         "Development Status :: 1 - Planning",
         "Intended Audience :: Developers",
         "Programming Language :: Python :: 3",
         "Operating System :: Unix",
         "Operating System :: MacOS :: MacOS X",
```

