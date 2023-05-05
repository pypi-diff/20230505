# Comparing `tmp/potatorch-0.0.2.tar.gz` & `tmp/potatorch-0.0.3.tar.gz`

## Comparing `potatorch-0.0.2.tar` & `potatorch-0.0.3.tar`

### file list

```diff
@@ -1,28 +1,30 @@
--rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 potatorch-0.0.2/.dockerignore
--rw-r--r--   0        0        0      375 2020-02-02 00:00:00.000000 potatorch-0.0.2/Dockerfile.gpu
--rwxr-xr-x   0        0        0      416 2020-02-02 00:00:00.000000 potatorch-0.0.2/build.sh
--rw-r--r--   0        0        0   277664 2020-02-02 00:00:00.000000 potatorch-0.0.2/potatorch.png
--rwxr-xr-x   0        0        0      224 2020-02-02 00:00:00.000000 potatorch-0.0.2/run.sh
--rw-r--r--   0        0        0      146 2020-02-02 00:00:00.000000 potatorch-0.0.2/setup.py
--rw-r--r--   0        0        0     3342 2020-02-02 00:00:00.000000 potatorch-0.0.2/examples/grid_search.py
--rw-r--r--   0        0        0     1509 2020-02-02 00:00:00.000000 potatorch-0.0.2/examples/mlp.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 potatorch-0.0.2/src/potatorch/__init__.py
--rw-r--r--   0        0        0    13931 2020-02-02 00:00:00.000000 potatorch-0.0.2/src/potatorch/callbacks.py
--rw-r--r--   0        0        0    12561 2020-02-02 00:00:00.000000 potatorch-0.0.2/src/potatorch/training.py
--rw-r--r--   0        0        0      377 2020-02-02 00:00:00.000000 potatorch-0.0.2/src/potatorch/utils.py
--rw-r--r--   0        0        0      574 2020-02-02 00:00:00.000000 potatorch-0.0.2/src/potatorch/datasets/FilteredDataset.py
--rw-r--r--   0        0        0       45 2020-02-02 00:00:00.000000 potatorch-0.0.2/src/potatorch/datasets/__init__.py
--rw-r--r--   0        0        0     2858 2020-02-02 00:00:00.000000 potatorch-0.0.2/src/potatorch/datasets/utils.py
--rw-r--r--   0        0        0      860 2020-02-02 00:00:00.000000 potatorch-0.0.2/src/potatorch/losses/MSRELoss.py
--rw-r--r--   0        0        0      519 2020-02-02 00:00:00.000000 potatorch-0.0.2/src/potatorch/losses/WDLLoss.py
--rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 potatorch-0.0.2/src/potatorch/losses/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 potatorch-0.0.2/src/potatorch/models/__init__.py
--rw-r--r--   0        0        0     3956 2020-02-02 00:00:00.000000 potatorch-0.0.2/src/potatorch/models/cnn.py
--rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 potatorch-0.0.2/src/potatorch/optimization/__init__.py
--rw-r--r--   0        0        0     4153 2020-02-02 00:00:00.000000 potatorch-0.0.2/src/potatorch/optimization/bayesian_optimizer.py
--rw-r--r--   0        0        0     7521 2020-02-02 00:00:00.000000 potatorch-0.0.2/src/potatorch/optimization/tuning.py
--rw-r--r--   0        0        0     1799 2020-02-02 00:00:00.000000 potatorch-0.0.2/.gitignore
--rw-r--r--   0        0        0     1069 2020-02-02 00:00:00.000000 potatorch-0.0.2/LICENSE
--rw-r--r--   0        0        0     5556 2020-02-02 00:00:00.000000 potatorch-0.0.2/README.md
--rw-r--r--   0        0        0      716 2020-02-02 00:00:00.000000 potatorch-0.0.2/pyproject.toml
--rw-r--r--   0        0        0     6191 2020-02-02 00:00:00.000000 potatorch-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 potatorch-0.0.3/.dockerignore
+-rw-r--r--   0        0        0      375 2020-02-02 00:00:00.000000 potatorch-0.0.3/Dockerfile.gpu
+-rwxr-xr-x   0        0        0      416 2020-02-02 00:00:00.000000 potatorch-0.0.3/build.sh
+-rwxr-xr-x   0        0        0      224 2020-02-02 00:00:00.000000 potatorch-0.0.3/run.sh
+-rw-r--r--   0        0        0      146 2020-02-02 00:00:00.000000 potatorch-0.0.3/setup.py
+-rw-r--r--   0        0        0     1095 2020-02-02 00:00:00.000000 potatorch-0.0.3/.github/workflows/python-publish.yml
+-rw-r--r--   0        0        0 12024910 2020-02-02 00:00:00.000000 potatorch-0.0.3/docs/potatorch-banner.png
+-rw-r--r--   0        0        0   277664 2020-02-02 00:00:00.000000 potatorch-0.0.3/docs/potatorch.png
+-rw-r--r--   0        0        0     3342 2020-02-02 00:00:00.000000 potatorch-0.0.3/examples/grid_search.py
+-rw-r--r--   0        0        0     1509 2020-02-02 00:00:00.000000 potatorch-0.0.3/examples/mlp.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 potatorch-0.0.3/src/potatorch/__init__.py
+-rw-r--r--   0        0        0    13931 2020-02-02 00:00:00.000000 potatorch-0.0.3/src/potatorch/callbacks.py
+-rw-r--r--   0        0        0    12561 2020-02-02 00:00:00.000000 potatorch-0.0.3/src/potatorch/training.py
+-rw-r--r--   0        0        0      377 2020-02-02 00:00:00.000000 potatorch-0.0.3/src/potatorch/utils.py
+-rw-r--r--   0        0        0      574 2020-02-02 00:00:00.000000 potatorch-0.0.3/src/potatorch/datasets/FilteredDataset.py
+-rw-r--r--   0        0        0       45 2020-02-02 00:00:00.000000 potatorch-0.0.3/src/potatorch/datasets/__init__.py
+-rw-r--r--   0        0        0     2858 2020-02-02 00:00:00.000000 potatorch-0.0.3/src/potatorch/datasets/utils.py
+-rw-r--r--   0        0        0      860 2020-02-02 00:00:00.000000 potatorch-0.0.3/src/potatorch/losses/MSRELoss.py
+-rw-r--r--   0        0        0      519 2020-02-02 00:00:00.000000 potatorch-0.0.3/src/potatorch/losses/WDLLoss.py
+-rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 potatorch-0.0.3/src/potatorch/losses/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 potatorch-0.0.3/src/potatorch/models/__init__.py
+-rw-r--r--   0        0        0     3956 2020-02-02 00:00:00.000000 potatorch-0.0.3/src/potatorch/models/cnn.py
+-rw-r--r--   0        0        0       50 2020-02-02 00:00:00.000000 potatorch-0.0.3/src/potatorch/optimization/__init__.py
+-rw-r--r--   0        0        0     4153 2020-02-02 00:00:00.000000 potatorch-0.0.3/src/potatorch/optimization/bayesian_optimizer.py
+-rw-r--r--   0        0        0     7521 2020-02-02 00:00:00.000000 potatorch-0.0.3/src/potatorch/optimization/tuning.py
+-rw-r--r--   0        0        0     1799 2020-02-02 00:00:00.000000 potatorch-0.0.3/.gitignore
+-rw-r--r--   0        0        0     1069 2020-02-02 00:00:00.000000 potatorch-0.0.3/LICENSE
+-rw-r--r--   0        0        0     6048 2020-02-02 00:00:00.000000 potatorch-0.0.3/README.md
+-rw-r--r--   0        0        0      716 2020-02-02 00:00:00.000000 potatorch-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0     6683 2020-02-02 00:00:00.000000 potatorch-0.0.3/PKG-INFO
```

### Comparing `potatorch-0.0.2/potatorch.png` & `potatorch-0.0.3/docs/potatorch.png`

 * *Files identical despite different names*

### Comparing `potatorch-0.0.2/examples/grid_search.py` & `potatorch-0.0.3/examples/grid_search.py`

 * *Files identical despite different names*

### Comparing `potatorch-0.0.2/examples/mlp.py` & `potatorch-0.0.3/examples/mlp.py`

 * *Files identical despite different names*

### Comparing `potatorch-0.0.2/src/potatorch/callbacks.py` & `potatorch-0.0.3/src/potatorch/callbacks.py`

 * *Files identical despite different names*

### Comparing `potatorch-0.0.2/src/potatorch/training.py` & `potatorch-0.0.3/src/potatorch/training.py`

 * *Files identical despite different names*

### Comparing `potatorch-0.0.2/src/potatorch/datasets/FilteredDataset.py` & `potatorch-0.0.3/src/potatorch/datasets/FilteredDataset.py`

 * *Files identical despite different names*

### Comparing `potatorch-0.0.2/src/potatorch/datasets/utils.py` & `potatorch-0.0.3/src/potatorch/datasets/utils.py`

 * *Files identical despite different names*

### Comparing `potatorch-0.0.2/src/potatorch/losses/MSRELoss.py` & `potatorch-0.0.3/src/potatorch/losses/MSRELoss.py`

 * *Files identical despite different names*

### Comparing `potatorch-0.0.2/src/potatorch/losses/WDLLoss.py` & `potatorch-0.0.3/src/potatorch/losses/WDLLoss.py`

 * *Files identical despite different names*

### Comparing `potatorch-0.0.2/src/potatorch/models/cnn.py` & `potatorch-0.0.3/src/potatorch/models/cnn.py`

 * *Files identical despite different names*

### Comparing `potatorch-0.0.2/src/potatorch/optimization/bayesian_optimizer.py` & `potatorch-0.0.3/src/potatorch/optimization/bayesian_optimizer.py`

 * *Files identical despite different names*

### Comparing `potatorch-0.0.2/src/potatorch/optimization/tuning.py` & `potatorch-0.0.3/src/potatorch/optimization/tuning.py`

 * *Files identical despite different names*

### Comparing `potatorch-0.0.2/.gitignore` & `potatorch-0.0.3/.gitignore`

 * *Files identical despite different names*

### Comparing `potatorch-0.0.2/LICENSE` & `potatorch-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `potatorch-0.0.2/README.md` & `potatorch-0.0.3/README.md`

 * *Files 23% similar despite different names*

```diff
@@ -1,21 +1,25 @@
 
 <div align="center">
 
-# PotaTorch
-
-<img src="https://raw.githubusercontent.com/crybot/potatorch/main/potatorch.png" width="200" height="200" role="img">
+<img src="https://raw.githubusercontent.com/crybot/potatorch/main/docs/potatorch-banner.png" width="100%" role="img">
 
 **PotaTorch is a lightweight PyTorch framework specifically designed to run on hardware with limited resources.**
 
-**WIP:**
 ______________________________________________________________________
+
+<!-- [![PyPI Status](https://pepy.tech/badge/potatorch)](https://pepy.tech/project/potatorch) -->
+[![PyPI - Python Version](https://img.shields.io/pypi/pyversions/potatorch)](https://pypi.org/project/potatorch/)
+[![PyPI version](https://badge.fury.io/py/potatorch.svg)](https://badge.fury.io/py/potatorch)
+![GitHub commit activity](https://img.shields.io/github/commit-activity/w/crybot/potatorch)
+[![license](https://img.shields.io/badge/License-MIT-blue.svg)](https://github.com/crybot/potatorch/blob/main/LICENSE)
+
 </div>
 
-### Install PotaTorch
+### Installation
 PotaTorch is published on PyPI, you can install it through pip:
 ```bash
 pip install potatorch
 ```
 
 or you can install it from sources:
 ```bash
```

### Comparing `potatorch-0.0.2/pyproject.toml` & `potatorch-0.0.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "potatorch"
-version = "0.0.2"
+version = "0.0.3"
 authors = [
   { name="Marco Pampaloni", email="marco.pampaloni1@gmail.com" },
 ]
 description = "Lightweight high-level PyTorch framework that runs on potato machines"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `potatorch-0.0.2/PKG-INFO` & `potatorch-0.0.3/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: potatorch
-Version: 0.0.2
+Version: 0.0.3
 Summary: Lightweight high-level PyTorch framework that runs on potato machines
 Project-URL: Homepage, https://github.com/crybot/potatorch
 Project-URL: Bug Tracker, https://github.com/crybot/potatorch/issues
 Author-email: Marco Pampaloni <marco.pampaloni1@gmail.com>
 License-File: LICENSE
 Keywords: deep learning,framework,limited resources,machine learning,python,pytorch
 Classifier: License :: OSI Approved :: MIT License
@@ -12,25 +12,29 @@
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 
 
 <div align="center">
 
-# PotaTorch
-
-<img src="https://raw.githubusercontent.com/crybot/potatorch/main/potatorch.png" width="200" height="200" role="img">
+<img src="https://raw.githubusercontent.com/crybot/potatorch/main/docs/potatorch-banner.png" width="100%" role="img">
 
 **PotaTorch is a lightweight PyTorch framework specifically designed to run on hardware with limited resources.**
 
-**WIP:**
 ______________________________________________________________________
+
+<!-- [![PyPI Status](https://pepy.tech/badge/potatorch)](https://pepy.tech/project/potatorch) -->
+[![PyPI - Python Version](https://img.shields.io/pypi/pyversions/potatorch)](https://pypi.org/project/potatorch/)
+[![PyPI version](https://badge.fury.io/py/potatorch.svg)](https://badge.fury.io/py/potatorch)
+![GitHub commit activity](https://img.shields.io/github/commit-activity/w/crybot/potatorch)
+[![license](https://img.shields.io/badge/License-MIT-blue.svg)](https://github.com/crybot/potatorch/blob/main/LICENSE)
+
 </div>
 
-### Install PotaTorch
+### Installation
 PotaTorch is published on PyPI, you can install it through pip:
 ```bash
 pip install potatorch
 ```
 
 or you can install it from sources:
 ```bash
```

