# Comparing `tmp/innvestigate-2.0.2.tar.gz` & `tmp/innvestigate-2.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "innvestigate-2.0.2.tar", max compression
+gzip compressed data, was "innvestigate-2.1.0.tar", max compression
```

## Comparing `innvestigate-2.0.2.tar` & `innvestigate-2.1.0.tar`

### file list

```diff
@@ -1,28 +1,27 @@
--rw-r--r--   0        0        0     1954 2023-01-31 16:40:22.138158 innvestigate-2.0.2/LICENSE
--rw-r--r--   0        0        0    11179 2023-01-31 16:52:05.590120 innvestigate-2.0.2/README.md
--rw-r--r--   0        0        0     3763 2023-01-31 17:23:52.055844 innvestigate-2.0.2/pyproject.toml
--rw-r--r--   0        0        0      263 2023-01-31 16:52:05.589970 innvestigate-2.0.2/src/innvestigate/__init__.py
--rw-r--r--   0        0        0     3330 2023-01-31 16:53:18.644819 innvestigate-2.0.2/src/innvestigate/analyzer/__init__.py
--rw-r--r--   0        0        0     7513 2023-01-31 16:53:18.643809 innvestigate-2.0.2/src/innvestigate/analyzer/base.py
--rw-r--r--   0        0        0     6914 2023-01-31 16:53:18.645221 innvestigate-2.0.2/src/innvestigate/analyzer/deeptaylor.py
--rw-r--r--   0        0        0     9934 2023-01-31 16:53:18.643485 innvestigate-2.0.2/src/innvestigate/analyzer/gradient_based.py
--rw-r--r--   0        0        0     2089 2023-01-31 16:53:18.645295 innvestigate-2.0.2/src/innvestigate/analyzer/misc.py
--rw-r--r--   0        0        0    12220 2023-01-31 16:53:18.643625 innvestigate-2.0.2/src/innvestigate/analyzer/network_base.py
--rw-r--r--   0        0        0        0 2023-01-31 16:52:05.590324 innvestigate-2.0.2/src/innvestigate/analyzer/relevance_based/__init__.py
--rw-r--r--   0        0        0    29199 2023-01-31 16:53:18.644970 innvestigate-2.0.2/src/innvestigate/analyzer/relevance_based/relevance_analyzer.py
--rw-r--r--   0        0        0    20893 2023-01-31 16:53:18.644276 innvestigate-2.0.2/src/innvestigate/analyzer/relevance_based/relevance_rule.py
--rw-r--r--   0        0        0     3121 2023-01-31 16:53:18.645440 innvestigate-2.0.2/src/innvestigate/analyzer/relevance_based/utils.py
--rw-r--r--   0        0        0    16004 2023-01-31 16:53:18.642150 innvestigate-2.0.2/src/innvestigate/analyzer/reverse_base.py
--rw-r--r--   0        0        0    12620 2023-01-31 16:53:18.644613 innvestigate-2.0.2/src/innvestigate/analyzer/wrapper.py
--rw-r--r--   0        0        0     6728 2023-01-31 16:53:18.644456 innvestigate-2.0.2/src/innvestigate/backend/__init__.py
--rw-r--r--   0        0        0     9150 2023-01-31 16:53:18.643308 innvestigate-2.0.2/src/innvestigate/backend/checks.py
--rw-r--r--   0        0        0    45128 2023-01-31 17:22:09.896873 innvestigate-2.0.2/src/innvestigate/backend/graph.py
--rw-r--r--   0        0        0     2940 2023-01-31 16:41:02.307809 innvestigate-2.0.2/src/innvestigate/backend/types.py
--rw-r--r--   0        0        0    13689 2023-01-31 16:53:18.643879 innvestigate-2.0.2/src/innvestigate/layers.py
--rw-r--r--   0        0        0        0 2023-01-31 16:52:05.591616 innvestigate-2.0.2/src/innvestigate/tools/__init__.py
--rw-r--r--   0        0        0    18703 2023-01-31 16:53:18.645727 innvestigate-2.0.2/src/innvestigate/tools/perturbate.py
--rw-r--r--   0        0        0     2317 2023-01-31 16:53:18.645873 innvestigate-2.0.2/src/innvestigate/utils/__init__.py
--rw-r--r--   0        0        0     2385 2023-01-31 16:53:18.645602 innvestigate-2.0.2/src/innvestigate/utils/sequence.py
--rw-r--r--   0        0        0     4337 2023-01-31 16:53:18.646064 innvestigate-2.0.2/src/innvestigate/utils/visualizations.py
--rw-r--r--   0        0        0    12420 1970-01-01 00:00:00.000000 innvestigate-2.0.2/setup.py
--rw-r--r--   0        0        0    12619 1970-01-01 00:00:00.000000 innvestigate-2.0.2/PKG-INFO
+-rw-r--r--   0        0        0     1954 2023-01-31 16:40:22.138158 innvestigate-2.1.0/LICENSE
+-rw-r--r--   0        0        0    11179 2023-05-05 17:13:08.474228 innvestigate-2.1.0/README.md
+-rw-r--r--   0        0        0     3944 2023-05-05 17:13:22.820379 innvestigate-2.1.0/pyproject.toml
+-rw-r--r--   0        0        0      304 2023-05-05 17:14:37.771956 innvestigate-2.1.0/src/innvestigate/__init__.py
+-rw-r--r--   0        0        0     3330 2023-01-31 16:53:18.644819 innvestigate-2.1.0/src/innvestigate/analyzer/__init__.py
+-rw-r--r--   0        0        0     7513 2023-01-31 16:53:18.643809 innvestigate-2.1.0/src/innvestigate/analyzer/base.py
+-rw-r--r--   0        0        0     6912 2023-05-05 17:10:27.891438 innvestigate-2.1.0/src/innvestigate/analyzer/deeptaylor.py
+-rw-r--r--   0        0        0     9930 2023-05-05 17:10:27.921966 innvestigate-2.1.0/src/innvestigate/analyzer/gradient_based.py
+-rw-r--r--   0        0        0     2089 2023-01-31 16:53:18.645295 innvestigate-2.1.0/src/innvestigate/analyzer/misc.py
+-rw-r--r--   0        0        0    12220 2023-01-31 16:53:18.643625 innvestigate-2.1.0/src/innvestigate/analyzer/network_base.py
+-rw-r--r--   0        0        0        0 2023-01-31 16:52:05.590324 innvestigate-2.1.0/src/innvestigate/analyzer/relevance_based/__init__.py
+-rw-r--r--   0        0        0    29249 2023-05-05 14:15:34.580366 innvestigate-2.1.0/src/innvestigate/analyzer/relevance_based/relevance_analyzer.py
+-rw-r--r--   0        0        0    20892 2023-05-05 17:10:28.179145 innvestigate-2.1.0/src/innvestigate/analyzer/relevance_based/relevance_rule.py
+-rw-r--r--   0        0        0     3121 2023-01-31 16:53:18.645440 innvestigate-2.1.0/src/innvestigate/analyzer/relevance_based/utils.py
+-rw-r--r--   0        0        0    16002 2023-05-05 17:10:27.971902 innvestigate-2.1.0/src/innvestigate/analyzer/reverse_base.py
+-rw-r--r--   0        0        0    12619 2023-05-05 17:10:27.987380 innvestigate-2.1.0/src/innvestigate/analyzer/wrapper.py
+-rw-r--r--   0        0        0     6728 2023-01-31 16:53:18.644456 innvestigate-2.1.0/src/innvestigate/backend/__init__.py
+-rw-r--r--   0        0        0     9028 2023-05-05 14:15:34.580478 innvestigate-2.1.0/src/innvestigate/backend/checks.py
+-rw-r--r--   0        0        0    45544 2023-05-05 17:10:28.407379 innvestigate-2.1.0/src/innvestigate/backend/graph.py
+-rw-r--r--   0        0        0     2940 2023-01-31 16:41:02.307809 innvestigate-2.1.0/src/innvestigate/backend/types.py
+-rw-r--r--   0        0        0    13689 2023-01-31 16:53:18.643879 innvestigate-2.1.0/src/innvestigate/layers.py
+-rw-r--r--   0        0        0        0 2023-01-31 16:52:05.591616 innvestigate-2.1.0/src/innvestigate/tools/__init__.py
+-rw-r--r--   0        0        0    18703 2023-01-31 16:53:18.645727 innvestigate-2.1.0/src/innvestigate/tools/perturbate.py
+-rw-r--r--   0        0        0     2317 2023-01-31 16:53:18.645873 innvestigate-2.1.0/src/innvestigate/utils/__init__.py
+-rw-r--r--   0        0        0     2385 2023-01-31 16:53:18.645602 innvestigate-2.1.0/src/innvestigate/utils/sequence.py
+-rw-r--r--   0        0        0     4337 2023-01-31 16:53:18.646064 innvestigate-2.1.0/src/innvestigate/utils/visualizations.py
+-rw-r--r--   0        0        0    12658 1970-01-01 00:00:00.000000 innvestigate-2.1.0/PKG-INFO
```

### Comparing `innvestigate-2.0.2/LICENSE` & `innvestigate-2.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `innvestigate-2.0.2/README.md` & `innvestigate-2.1.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 
 [![PyPI package version](https://img.shields.io/pypi/v/innvestigate)](https://pypi.org/project/innvestigate/)
 [![GitHub package version](https://img.shields.io/github/v/tag/albermax/innvestigate)](https://github.com/albermax/innvestigate/tags)
 [![License: BSD-2](https://img.shields.io/badge/License-BSD--2-purple.svg)](https://github.com/albermax/innvestigate/blob/master/LICENSE)
 [![Black](https://img.shields.io/badge/code_style-black-black.svg)](https://github.com/psf/black)
 
 [![Python](https://img.shields.io/pypi/pyversions/innvestigate.svg)](https://badge.fury.io/py/innvestigate)
-[![TensorFlow package version](https://img.shields.io/badge/TensorFlow-2.6_--_2.11-orange.svg)](https://github.com/albermax/innvestigate)
+[![TensorFlow package version](https://img.shields.io/badge/TensorFlow-2.6_--_2.12-orange.svg)](https://github.com/albermax/innvestigate)
 
 ![Different explanation methods on ImageNet.](https://github.com/albermax/innvestigate/raw/master/examples/images/analysis_grid.png)
 
 ## Table of contents
 
 * [Introduction](#introduction)
 * [Installation](#installation)
```

### Comparing `innvestigate-2.0.2/pyproject.toml` & `innvestigate-2.1.0/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "innvestigate"
-version = "2.0.2"
+version = "2.1.0"
 description = "A toolbox to innvestigate neural networks' predictions."
 classifiers = [
     "License :: OSI Approved :: BSD License",
     "Development Status :: 5 - Production/Stable",
     "Environment :: Console", 
     "Intended Audience :: Science/Research",
     "Operating System :: POSIX :: Linux",
@@ -31,40 +31,45 @@
 readme = "README.md"
 homepage = "https://github.com/albermax/innvestigate"
 repository = "https://github.com/albermax/innvestigate"
 documentation = "https://innvestigate.readthedocs.io/en/latest/"
 keywords = ["XAI", "LRP", "Deep Taylor",]
 
 [tool.poetry.dependencies]
-python = ">=3.8,<3.11"
-tensorflow = ">=2.6,<2.12"
-future = "^0.18.2"
-numpy = "^1.22"
-matplotlib = "^3.5.1"
-
-[tool.poetry.dev-dependencies]
-black  = "^22.3"
-ruff = "^0.0.212"
-Pillow = "^9.0.0"
-pytest = "^7.2.0"
-pytest-cov = "^4.0.0"
-coverage = {extras = ["toml"], version = "^7.0.3"}
-codecov = "^2.1.11"
-rope = "^1.6.0"
-pylint = "^2.12.2"
-ipykernel = "^6.19.4"
-isort = "^5.10.1"
-mypy = "^0.991"
-MonkeyType = "^22.2.0"
-vulture = "^2.3"
-Sphinx = "^6.1.1"
-pandas = "^1.3"
-ftfy = "^6.1.1"
-pyupgrade = "^3.3.1"
-pre-commit = "^2.19.0"
+python = ">=3.8, <3.12"
+tensorflow = ">=2.6, <2.13"
+numpy = ">=1.22, <2"
+matplotlib = ">=3.5, <4"
+future = ">=0.18, <0.19"
+
+[tool.poetry.group.notebooks.dependencies]
+ipykernel = ">=6.19, <7"
+Pillow = ">=9.0, <10"
+ftfy = ">=6.1, <7"
+pandas = ">=1, <3"
+
+[tool.poetry.group.docs.dependencies]
+Sphinx = ">=6.1, <8"
+
+[tool.poetry.group.tests.dependencies]
+pytest = ">=7.2, <8"
+pytest-cov = ">=4.0, <5"
+coverage = {extras = ["toml"], version = ">=7, <8"}
+codecov = ">=2.1, <3"
+
+[tool.poetry.group.dev.dependencies]
+black  = ">=22.3, <24"
+ruff = ">=0.0.264, <0.1"
+rope = ">=1.6, <2"
+pylint = ">=2.12, <3"
+isort = ">=5.10, <6"
+mypy = ">=1, <2"
+vulture = ">=2.3, <3"
+pyupgrade = ">=3.3, <4"
+pre-commit = ">=2.19, <4"
 
 [tool.isort]
 profile = "black"
 multi_line_output = 3 
 known_first_party = "innvestigate"
 known_local_folder = "tests"
```

### Comparing `innvestigate-2.0.2/src/innvestigate/analyzer/__init__.py` & `innvestigate-2.1.0/src/innvestigate/analyzer/__init__.py`

 * *Files identical despite different names*

### Comparing `innvestigate-2.0.2/src/innvestigate/analyzer/base.py` & `innvestigate-2.1.0/src/innvestigate/analyzer/base.py`

 * *Files identical despite different names*

### Comparing `innvestigate-2.0.2/src/innvestigate/analyzer/deeptaylor.py` & `innvestigate-2.1.0/src/innvestigate/analyzer/deeptaylor.py`

 * *Files 0% similar despite different names*

```diff
@@ -35,15 +35,14 @@
             lambda layer: not ichecks.only_relu_activation(layer),
             "This DeepTaylor implementation only supports ReLU activations.",
             check_type="exception",
         )
         self._do_model_checks()
 
     def _create_analysis(self, *args: Any, **kwargs: Any):
-
         # Kernel layers.
         self._add_conditional_reverse_mapping(
             lambda l: (ichecks.contains_kernel(l) and ichecks.contains_activation(l)),
             lrp_rules.Alpha1Beta0IgnoreBiasRule,
             name="deep_taylor_kernel_w_relu",
         )
         self._add_conditional_reverse_mapping(
@@ -172,15 +171,14 @@
                 "Z-B (bounded rule) require both values."
             )
 
         self._bounds_low = low
         self._bounds_high = high
 
     def _create_analysis(self, *args, **kwargs):
-
         low, high = self._bounds_low, self._bounds_high
 
         class BoundedProxyRule(lrp_rules.BoundedRule):
             def __init__(self, *args, **kwargs):
                 super().__init__(*args, low=low, high=high, **kwargs)
 
         self._add_conditional_reverse_mapping(
```

### Comparing `innvestigate-2.0.2/src/innvestigate/analyzer/gradient_based.py` & `innvestigate-2.1.0/src/innvestigate/analyzer/gradient_based.py`

 * *Files 0% similar despite different names*

```diff
@@ -142,15 +142,14 @@
 class InputTimesGradient(Gradient):
     """Input*Gradient analyzer.
 
     :param model: A Keras model.
     """
 
     def __init__(self, model, **kwargs):
-
         super().__init__(model, **kwargs)
 
     def _create_analysis(self, model, stop_analysis_at_tensors=None):
         if stop_analysis_at_tensors is None:
             stop_analysis_at_tensors = []
 
         tensors_to_analyze = [
@@ -203,15 +202,14 @@
             lambda layer: not ichecks.only_relu_activation(layer),
             "Deconvnet is only specified for networks with ReLU activations.",
             check_type="exception",
         )
         self._do_model_checks()
 
     def _create_analysis(self, *args, **kwargs):
-
         self._add_conditional_reverse_mapping(
             lambda layer: ichecks.contains_activation(layer, "relu"),
             DeconvnetReverseReLULayer,
             name="deconvnet_reverse_relu_layer",
         )
 
         return super()._create_analysis(*args, **kwargs)
@@ -243,15 +241,14 @@
             lambda layer: not ichecks.only_relu_activation(layer),
             "GuidedBackprop is only specified for networks with ReLU activations.",
             check_type="exception",
         )
         self._do_model_checks()
 
     def _create_analysis(self, *args, **kwargs):
-
         self._add_conditional_reverse_mapping(
             lambda layer: ichecks.contains_activation(layer, "relu"),
             guided_backprop_reverse_relu_layer,
             name="guided_backprop_reverse_relu_layer",
         )
 
         return super()._create_analysis(*args, **kwargs)
@@ -317,15 +314,14 @@
         **kwargs,
     ):
         # If initialized through serialization:
         if "subanalyzer" in kwargs:
             subanalyzer = kwargs.pop("subanalyzer")
         # If initialized normally:
         else:
-
             subanalyzer = Gradient(
                 model,
                 neuron_selection_mode=neuron_selection_mode,
                 postprocess=postprocess,
             )
 
         super().__init__(
```

### Comparing `innvestigate-2.0.2/src/innvestigate/analyzer/misc.py` & `innvestigate-2.1.0/src/innvestigate/analyzer/misc.py`

 * *Files identical despite different names*

### Comparing `innvestigate-2.0.2/src/innvestigate/analyzer/network_base.py` & `innvestigate-2.1.0/src/innvestigate/analyzer/network_base.py`

 * *Files identical despite different names*

### Comparing `innvestigate-2.0.2/src/innvestigate/analyzer/relevance_based/relevance_analyzer.py` & `innvestigate-2.1.0/src/innvestigate/analyzer/relevance_based/relevance_analyzer.py`

 * *Files 0% similar despite different names*

```diff
@@ -390,15 +390,17 @@
             # rule is list of conditioned rules
             use_conditions = True
             rules = rule
 
         # apply rule to first self._until_layer_idx layers
         if self._until_layer_rule is not None and self._until_layer_idx is not None:
             for i in range(self._until_layer_idx + 1):
-                is_at_idx: LayerCheck = lambda layer: ichecks.is_layer_at_idx(layer, i)
+                is_at_idx: LayerCheck = lambda layer, i=i: ichecks.is_layer_at_idx(
+                    model, layer, i
+                )
                 rules.insert(0, (is_at_idx, self._until_layer_rule))
 
         # create a BoundedRule for input layer handling from given tuple
         if self._input_layer_rule is not None:
             input_layer_rule = self._input_layer_rule
             if isinstance(input_layer_rule, tuple):
                 low, high = input_layer_rule
```

### Comparing `innvestigate-2.0.2/src/innvestigate/analyzer/relevance_based/relevance_rule.py` & `innvestigate-2.1.0/src/innvestigate/analyzer/relevance_based/relevance_rule.py`

 * *Files 0% similar despite different names*

```diff
@@ -50,15 +50,14 @@
     def apply(
         self,
         Xs: list[Tensor],
         _Ys: list[Tensor],
         Rs: list[Tensor],
         _reverse_state,
     ) -> list[Tensor]:
-
         # Get activations.
         Zs = ibackend.apply(self._layer_wo_act, Xs)
         # Divide incoming relevance by the activations.
         tmp = [ibackend.safe_divide(a, b) for a, b in zip(Rs, Zs)]
         # Propagate the relevance to input neurons
         # using the gradient.
         grads = ibackend.gradients(Xs, Zs, tmp)
```

### Comparing `innvestigate-2.0.2/src/innvestigate/analyzer/relevance_based/utils.py` & `innvestigate-2.1.0/src/innvestigate/analyzer/relevance_based/utils.py`

 * *Files identical despite different names*

### Comparing `innvestigate-2.0.2/src/innvestigate/analyzer/reverse_base.py` & `innvestigate-2.1.0/src/innvestigate/analyzer/reverse_base.py`

 * *Files 0% similar despite different names*

```diff
@@ -250,15 +250,14 @@
             project_bottleneck_tensors=self._reverse_project_bottleneck_layers,
             return_all_reversed_tensors=return_all_reversed_tensors,
         )
 
     def _create_analysis(
         self, model: Model, stop_analysis_at_tensors: list[Tensor] = None
     ):
-
         if stop_analysis_at_tensors is None:
             stop_analysis_at_tensors = []
 
         return_all_reversed_tensors = (
             self._reverse_check_min_max_values
             or self._reverse_check_finite
             or self._reverse_keep_tensors
@@ -316,15 +315,14 @@
                 )
                 debug_tensors += tensors
 
             return ret, debug_tensors
         return ret
 
     def _handle_debug_output(self, debug_values):
-
         if self._reverse_check_min_max_values:
             indices = self._debug_tensors_indices["min"]
             tmp = debug_values[indices[0] : indices[1]]
             tmp = sorted(
                 (self._reverse_tensors_mapping[i], v) for i, v in enumerate(tmp)
             )
             print(f"Minimum values in tensors: ((NodeID, TensorID), Value) - {tmp}")
```

### Comparing `innvestigate-2.0.2/src/innvestigate/analyzer/wrapper.py` & `innvestigate-2.1.0/src/innvestigate/analyzer/wrapper.py`

 * *Files 0% similar despite different names*

```diff
@@ -80,15 +80,14 @@
         self,
         subanalyzer: AnalyzerNetworkBase,
         *args,
         augment_by_n: int = 2,
         neuron_selection_mode="max_activation",
         **kwargs,
     ):
-
         if neuron_selection_mode == "max_activation":
             # TODO: find a more transparent way.
             #
             # Since AugmentReduceBase analyzers augment the input,
             # it is possible that the neuron w/ max activation changes.
             # As a workaround, the index of the maximally activated neuron
             # w.r.t. the "unperturbed" input is computed and used in combination
```

### Comparing `innvestigate-2.0.2/src/innvestigate/backend/__init__.py` & `innvestigate-2.1.0/src/innvestigate/backend/__init__.py`

 * *Files identical despite different names*

### Comparing `innvestigate-2.0.2/src/innvestigate/backend/checks.py` & `innvestigate-2.1.0/src/innvestigate/backend/checks.py`

 * *Files 4% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 
 from __future__ import annotations
 
 import tensorflow.keras.layers as klayers
 from tensorflow import Module, keras
 
 import innvestigate.backend as ibackend
-from innvestigate.backend.types import Layer
+from innvestigate.backend.types import Layer, Model
 
 __all__ = [
     "get_activation_search_safe_layers",
     "contains_activation",
     "contains_kernel",
     "only_relu_activation",
     "is_module",
@@ -321,12 +321,10 @@
             else:
                 tmp.add(l)
         layer_inputs = tmp
 
     return all(isinstance(x, klayers.InputLayer) for x in layer_inputs)
 
 
-def is_layer_at_idx(layer: Layer, index, ignore_reshape_layers=True) -> bool:
-    """Checks if layer is a layer at index index,
-    by repeatedly applying is_input_layer()."""
-    # TODO: implement layer index check
-    raise NotImplementedError("Layer index checking hasn't been implemented yet.")
+def is_layer_at_idx(model: Model, layer: Layer, index) -> bool:
+    """Checks if layer is a layer at specified index of model."""
+    return layer == model.layers[index]
```

### Comparing `innvestigate-2.0.2/src/innvestigate/backend/graph.py` & `innvestigate-2.1.0/src/innvestigate/backend/graph.py`

 * *Files 1% similar despite different names*

```diff
@@ -26,16 +26,17 @@
 
 __all__ = [
     "get_kernel",
     "get_layer_inbound_count",
     "get_layer_neuronwise_io",
     "copy_layer_wo_activation",
     "copy_layer",
-    "pre_softmax_tensors",
+    "pre_output_tensors",
     "model_wo_softmax",
+    "model_wo_output_activation",
     "get_model_layers",
     "model_contains",
     "trace_model_execution",
     "get_model_execution_trace",
     "get_model_execution_graph",
     "print_model_execution_graph",
     "get_bottleneck_nodes",
@@ -334,40 +335,54 @@
                 if reuse_symbolic_tensors:
                     weights = layer.weights[:-1]
                 else:
                     weights = layer.get_weights()[:-1]
     return get_layer_from_config(layer, config, weights=weights, **kwargs)
 
 
-def pre_softmax_tensors(Xs: Tensor, should_find_softmax: bool = True) -> list[Tensor]:
-    """Finds the tensors that were preceeding a potential softmax."""
-    softmax_found = False
+def pre_output_tensors(Xs: Tensor, activation: str = None) -> list[Tensor]:
+    """Finds the tensors that were preceeding a potential activation."""
+    activation_found = False
 
     Xs = ibackend.to_list(Xs)
     ret = []
     for x in Xs:
         layer, node_index, _tensor_index = x._keras_history
-        if ichecks.contains_activation(layer, activation="softmax"):
-            softmax_found = True
+        if ichecks.contains_activation(layer, activation=activation):
+            activation_found = True
             if isinstance(layer, klayers.Activation):
                 ret.append(layer.get_input_at(node_index))
             else:
                 layer_wo_act = copy_layer_wo_activation(layer)
                 ret.append(layer_wo_act(layer.get_input_at(node_index)))
 
-    if should_find_softmax and not softmax_found:
-        raise Exception("No softmax found.")
+    if not activation_found:
+        if not activation == None:
+            raise Exception(f"No output activation found.")
+        else:
+            raise Exception(f"No {activation} found.")
 
     return ret
 
 
 def model_wo_softmax(model: Model) -> Model:
     """Creates a new model w/o the final softmax activation."""
     return kmodels.Model(
-        inputs=model.inputs, outputs=pre_softmax_tensors(model.outputs), name=model.name
+        inputs=model.inputs,
+        outputs=pre_output_tensors(model.outputs, activation="softmax"),
+        name=model.name,
+    )
+
+
+def model_wo_output_activation(model: Model) -> Model:
+    """Creates a new model w/o the final activation."""
+    return kmodels.Model(
+        inputs=model.inputs,
+        outputs=pre_output_tensors(model.outputs),
+        name=model.name,
     )
 
 
 ###############################################################################
 
 
 def get_model_layers(model: Model) -> list[Layer]:
@@ -523,15 +538,14 @@
 
             def actual_mapping(
                 Xs: list[Tensor],
                 Ys: list[Tensor],
                 reversed_Ys: list[Tensor],
                 reverse_state,
             ):
-
                 X2s = ibackend.apply(surrogate_layer1, Xs)
                 # Apply first mapping
                 # TODO (alber): update reverse state
                 reversed_X2s = actual_mapping_2(X2s, Ys, reversed_Ys, reverse_state)
                 return actual_mapping_1(Xs, X2s, reversed_X2s, reverse_state)
 
         return actual_mapping
@@ -769,15 +783,14 @@
     # Xs_layers = List[Layer]
     # Ys_layers = List[List[Layer]]
 
     nid_to_nodes = {t[0]: t for t in id_execution_trace}
 
     model_execution_trace = []
     for nid, l, Xs, Ys in id_execution_trace:
-
         if isinstance(l, klayers.InputLayer):
             # The nids that created or receive the tensors.
             Xs_nids = []  # Input layer does not receive.
             Ys_nids = [inputs_to_node[id(Y)] for Y in Ys]
             # The layers that created or receive the tensors.
             Xs_layers = []  # Input layer does not receive.
             Ys_layers = [
```

### Comparing `innvestigate-2.0.2/src/innvestigate/backend/types.py` & `innvestigate-2.1.0/src/innvestigate/backend/types.py`

 * *Files identical despite different names*

### Comparing `innvestigate-2.0.2/src/innvestigate/layers.py` & `innvestigate-2.1.0/src/innvestigate/layers.py`

 * *Files identical despite different names*

### Comparing `innvestigate-2.0.2/src/innvestigate/tools/perturbate.py` & `innvestigate-2.1.0/src/innvestigate/tools/perturbate.py`

 * *Files identical despite different names*

### Comparing `innvestigate-2.0.2/src/innvestigate/utils/__init__.py` & `innvestigate-2.1.0/src/innvestigate/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `innvestigate-2.0.2/src/innvestigate/utils/sequence.py` & `innvestigate-2.1.0/src/innvestigate/utils/sequence.py`

 * *Files identical despite different names*

### Comparing `innvestigate-2.0.2/src/innvestigate/utils/visualizations.py` & `innvestigate-2.1.0/src/innvestigate/utils/visualizations.py`

 * *Files identical despite different names*

### Comparing `innvestigate-2.0.2/setup.py` & `innvestigate-2.1.0/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,42 +1,243 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: innvestigate
+Version: 2.1.0
+Summary: A toolbox to innvestigate neural networks' predictions.
+Home-page: https://github.com/albermax/innvestigate
+License: BSD-2-Clause
+Keywords: XAI,LRP,Deep Taylor
+Author: Maxmilian Alber
+Author-email: workDoTalberDoTmaximilian@gmail.com
+Maintainer: Adrian Hill
+Maintainer-email: hill@tu-berlin.de
+Requires-Python: >=3.8,<3.12
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Environment :: Console
+Classifier: Intended Audience :: Science/Research
+Classifier: License :: OSI Approved :: BSD License
+Classifier: Operating System :: POSIX :: Linux
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
+Requires-Dist: future (>=0.18,<0.19)
+Requires-Dist: matplotlib (>=3.5,<4)
+Requires-Dist: numpy (>=1.22,<2)
+Requires-Dist: tensorflow (>=2.6,<2.13)
+Project-URL: Documentation, https://innvestigate.readthedocs.io/en/latest/
+Project-URL: Repository, https://github.com/albermax/innvestigate
+Description-Content-Type: text/markdown
+
+# [iNNvestigate neural networks!](https://github.com/albermax/innvestigate) [![Tweet](https://img.shields.io/twitter/url/http/shields.io.svg?style=social)](https://twitter.com/intent/tweet?text=iNNvestigate%20neural%20networks!&url=https://github.com/albermax/innvestigate&hashtags=iNNvestigate,artificialintelligence,machinelearning,deeplearning,datascience)
+
+[![Documentation](https://img.shields.io/badge/Documentation-stable-blue.svg)](https://innvestigate.readthedocs.io/en/latest/)
+[![Build Status](https://github.com/albermax/innvestigate/actions/workflows/ci.yml/badge.svg)](https://github.com/albermax/innvestigate/actions/workflows/ci.yml)
+
+[![PyPI package version](https://img.shields.io/pypi/v/innvestigate)](https://pypi.org/project/innvestigate/)
+[![GitHub package version](https://img.shields.io/github/v/tag/albermax/innvestigate)](https://github.com/albermax/innvestigate/tags)
+[![License: BSD-2](https://img.shields.io/badge/License-BSD--2-purple.svg)](https://github.com/albermax/innvestigate/blob/master/LICENSE)
+[![Black](https://img.shields.io/badge/code_style-black-black.svg)](https://github.com/psf/black)
+
+[![Python](https://img.shields.io/pypi/pyversions/innvestigate.svg)](https://badge.fury.io/py/innvestigate)
+[![TensorFlow package version](https://img.shields.io/badge/TensorFlow-2.6_--_2.12-orange.svg)](https://github.com/albermax/innvestigate)
+
+![Different explanation methods on ImageNet.](https://github.com/albermax/innvestigate/raw/master/examples/images/analysis_grid.png)
+
+## Table of contents
+
+* [Introduction](#introduction)
+* [Installation](#installation)
+* [Usage and Examples](#usage-and-examples)
+* [More documentation](#more-documentation)
+* [Contributing](#contributing)
+* [Releases](#releases)
+
+## Introduction
+
+In the recent years neural networks furthered the state of the art in many domains like, e.g., object detection and speech recognition.
+Despite the success neural networks are typically still treated as black boxes. Their internal workings are not fully understood and the basis for their predictions is unclear.
+In the attempt to understand neural networks better several methods were proposed, e.g., Saliency, Deconvnet, GuidedBackprop, SmoothGrad, IntegratedGradients, LRP, PatternNet and PatternAttribution.
+Due to the lack of a reference implementations comparing them is a major effort.
+This library addresses this by providing a common interface and out-of-the-box implementation for many analysis methods.
+Our goal is to make analyzing neural networks' predictions easy!
+
+
+### If you use this code please star the repository and cite the following paper:
+
+[Alber, M., Lapuschkin, S., Seegerer, P., Hägele, M., Schütt, K. T., Montavon, G., Samek, W., Müller, K. R., Dähne, S., & Kindermans, P. J. (2019). **iNNvestigate neural networks!** Journal of Machine Learning Research, 20.](https://jmlr.org/papers/v20/18-540.html)
+  ```
+  @article{JMLR:v20:18-540,
+  author  = {Maximilian Alber and Sebastian Lapuschkin and Philipp Seegerer and Miriam H{{\"a}}gele and Kristof T. Sch{{\"u}}tt and Gr{{\'e}}goire Montavon and Wojciech Samek and Klaus-Robert M{{\"u}}ller and Sven D{{\"a}}hne and Pieter-Jan Kindermans},
+  title   = {iNNvestigate Neural Networks!},
+  journal = {Journal of Machine Learning Research},
+  year    = {2019},
+  volume  = {20},
+  number  = {93},
+  pages   = {1-8},
+  url     = {http://jmlr.org/papers/v20/18-540.html}
+  }
+  ```
+
+## Installation
+
+iNNvestigate is based on Keras and TensorFlow 2 and can be installed with the following commands:
+
+```bash
+pip install innvestigate
+```
+
+**Please note that iNNvestigate currently requires disabling TF2's eager execution.**
+
+To use the example scripts and notebooks one additionally needs to install the package matplotlib:
+
+```bash
+pip install matplotlib
+```
+
+The library's tests can be executed via `pytest`. The easiest way to do reproducible development on iNNvestigate is to install all dev dependencies via [Poetry](https://python-poetry.org):
+```bash
+git clone https://github.com/albermax/innvestigate.git
+cd innvestigate
+
+poetry install
+poetry run pytest
+```
+
+## Usage and Examples
+
+The iNNvestigate library contains implementations for the following methods:
+
+* *function:*
+  * **gradient:** The gradient of the output neuron with respect to the input.
+  * **smoothgrad:** [SmoothGrad](https://arxiv.org/abs/1706.03825) averages the gradient over number of inputs with added noise.
+* *signal:*
+  * **deconvnet:** [DeConvNet](https://arxiv.org/abs/1311.2901) applies a ReLU in the gradient computation instead of the gradient of a ReLU.
+  * **guided:** [Guided BackProp](https://arxiv.org/abs/1412.6806) applies a ReLU in the gradient computation additionally to the gradient of a ReLU.
+  * **pattern.net:** [PatternNet](https://arxiv.org/abs/1705.05598) estimates the input signal of the output neuron. (*Note: not available in iNNvestigate 2.0*)
+* *attribution:*
+  * **input_t_gradient:** Input \* Gradient
+  * **deep_taylor[.bounded]:** [DeepTaylor](https://www.sciencedirect.com/science/article/pii/S0031320316303582?via%3Dihub) computes for each neuron a root point, that is close to the input, but which's output value is 0, and uses this difference to estimate the attribution of each neuron recursively.
+  * **lrp.\*:** [LRP](http://journals.plos.org/plosone/article?id=10.1371/journal.pone.0130140) attributes recursively to each neuron's input relevance proportional to its contribution of the neuron output.
+  * **integrated_gradients:** [IntegratedGradients](https://arxiv.org/abs/1703.01365) integrates the gradient along a path from the input to a reference.
+* *miscellaneous:*
+  * **input:** Returns the input.
+  * **random:** Returns random Gaussian noise.
+
+**The intention behind iNNvestigate is to make it easy to use analysis methods, but it is not to explain the underlying concepts and assumptions. Please, read the according publication(s) when using a certain method and when publishing please cite the according paper(s) (as well as the [iNNvestigate paper](https://arxiv.org/abs/1808.04260)). Thank you!**
+
+All the available methods have in common that they try to analyze the output of a specific neuron with respect to input to the neural network.
+Typically one analyses the neuron with the largest activation in the output layer.
+For example, given a Keras model, one can create a 'gradient' analyzer:
+
+```python
+import tensorflow as tf
+import innvestigate
+tf.compat.v1.disable_eager_execution()
+
+model = create_keras_model()
+
+analyzer = innvestigate.create_analyzer("gradient", model)
+```
+
+and analyze the influence of the neural network's input on the output neuron by:
+
+```python
+analysis = analyzer.analyze(inputs)
+```
+
+To analyze a neuron with the index i, one can use the following scheme:
+
+```python
+analyzer = innvestigate.create_analyzer("gradient",
+                                        model,
+					neuron_selection_mode="index")
+analysis = analyzer.analyze(inputs, i)
+```
+
+Let's look at an example ([code](https://github.com/albermax/innvestigate/blob/master/examples/readme_code_snippet.py)) with VGG16 and this image:
+
+![Input image.](https://github.com/albermax/innvestigate/raw/master/examples/images/readme_example_input.png)
+
+
+```python
+import tensorflow as tf
+import tensorflow.keras.applications.vgg16 as vgg16
+tf.compat.v1.disable_eager_execution()
+
+import innvestigate
+
+# Get model
+model, preprocess = vgg16.VGG16(), vgg16.preprocess_input
+# Strip softmax layer
+model = innvestigate.model_wo_softmax(model)
+
+# Create analyzer
+analyzer = innvestigate.create_analyzer("deep_taylor", model)
+
+# Add batch axis and preprocess
+x = preprocess(image[None])
+# Apply analyzer w.r.t. maximum activated output-neuron
+a = analyzer.analyze(x)
+
+# Aggregate along color channels and normalize to [-1, 1]
+a = a.sum(axis=np.argmax(np.asarray(a.shape) == 3))
+a /= np.max(np.abs(a))
+# Plot
+plt.imshow(a[0], cmap="seismic", clim=(-1, 1))
+```
+
+![Analysis image.](https://github.com/albermax/innvestigate/raw/master/examples/images/readme_example_analysis.png)
+
+### Tutorials
+
+In the directory [examples](https://github.com/albermax/innvestigate/blob/master/examples/) one can find different examples as Python scripts and as Jupyter notebooks:
+
+* **[Introduction to iNNvestigate](https://github.com/albermax/innvestigate/blob/master/examples/notebooks/introduction.ipynb):** shows how to use **iNNvestigate**.
+* **[Comparing methods on MNIST](https://github.com/albermax/innvestigate/blob/master/examples/notebooks/mnist_compare_methods.ipynb):** shows how to train and compare analyzers on MNIST.
+* **[Comparing output neurons on MNIST](https://github.com/albermax/innvestigate/blob/master/examples/notebooks/mnist_neuron_selection.ipynb):** shows how to analyze the prediction of different classes on MNIST.
+* **[Comparing methods on ImageNet](https://github.com/albermax/innvestigate/blob/master/examples/notebooks/imagenet_compare_methods.ipynb):** shows how to compare analyzers on ImageNet.
+* **[Comparing networks on ImageNet](https://github.com/albermax/innvestigate/blob/master/examples/notebooks/imagenet_compare_networks.ipynb):** shows how to compare analyzes for different networks on ImageNet.
+* **[Sentiment Analysis](https://github.com/albermax/innvestigate/blob/master/examples/notebooks/sentiment_analysis.ipynb)**.
+* **[Development with iNNvestigate](https://github.com/albermax/innvestigate/blob/master/examples/notebooks/introduction_development.ipynb):** shows how to develop with **iNNvestigate**.
+* **[Perturbation Analysis](https://github.com/albermax/innvestigate/blob/master/examples/notebooks/mnist_perturbation.ipynb)**.
+---
+
+**To use the ImageNet examples please download the example images first ([script](https://github.com/albermax/innvestigate/blob/master/examples/images/wget_imagenet_2011_samples.sh)).**
+
+## More documentation
+
+... can be found here:
+
+* Alber, M., Lapuschkin, S., Seegerer, P., Hägele, M., Schütt, K. T., Montavon, G., Samek, W., Müller, K. R., Dähne, S., & Kindermans, P. J. (2019). INNvestigate neural networks! Journal of Machine Learning Research, 20.](https://jmlr.org/papers/v20/18-540.html)
+  ```
+  @article{JMLR:v20:18-540,
+  author  = {Maximilian Alber and Sebastian Lapuschkin and Philipp Seegerer and Miriam H{{\"a}}gele and Kristof T. Sch{{\"u}}tt and Gr{{\'e}}goire Montavon and Wojciech Samek and Klaus-Robert M{{\"u}}ller and Sven D{{\"a}}hne and Pieter-Jan Kindermans},
+  title   = {iNNvestigate Neural Networks!},
+  journal = {Journal of Machine Learning Research},
+  year    = {2019},
+  volume  = {20},
+  number  = {93},
+  pages   = {1-8},
+  url     = {http://jmlr.org/papers/v20/18-540.html}
+  }
+  ```
+* [https://innvestigate.readthedocs.io/en/latest/](https://innvestigate.readthedocs.io/en/latest/)
+
+## Contributing
+
+If you would like to contribute or add your analysis method 
+please open an issue or submit a pull request.
 
-package_dir = \
-{'': 'src'}
+## Releases
 
-packages = \
-['innvestigate',
- 'innvestigate.analyzer',
- 'innvestigate.analyzer.relevance_based',
- 'innvestigate.backend',
- 'innvestigate.tools',
- 'innvestigate.utils']
-
-package_data = \
-{'': ['*']}
-
-install_requires = \
-['future>=0.18.2,<0.19.0',
- 'matplotlib>=3.5.1,<4.0.0',
- 'numpy>=1.22,<2.0',
- 'tensorflow>=2.6,<2.12']
-
-setup_kwargs = {
-    'name': 'innvestigate',
-    'version': '2.0.2',
-    'description': "A toolbox to innvestigate neural networks' predictions.",
-    'long_description': '# [iNNvestigate neural networks!](https://github.com/albermax/innvestigate) [![Tweet](https://img.shields.io/twitter/url/http/shields.io.svg?style=social)](https://twitter.com/intent/tweet?text=iNNvestigate%20neural%20networks!&url=https://github.com/albermax/innvestigate&hashtags=iNNvestigate,artificialintelligence,machinelearning,deeplearning,datascience)\n\n[![Documentation](https://img.shields.io/badge/Documentation-stable-blue.svg)](https://innvestigate.readthedocs.io/en/latest/)\n[![Build Status](https://github.com/albermax/innvestigate/actions/workflows/ci.yml/badge.svg)](https://github.com/albermax/innvestigate/actions/workflows/ci.yml)\n\n[![PyPI package version](https://img.shields.io/pypi/v/innvestigate)](https://pypi.org/project/innvestigate/)\n[![GitHub package version](https://img.shields.io/github/v/tag/albermax/innvestigate)](https://github.com/albermax/innvestigate/tags)\n[![License: BSD-2](https://img.shields.io/badge/License-BSD--2-purple.svg)](https://github.com/albermax/innvestigate/blob/master/LICENSE)\n[![Black](https://img.shields.io/badge/code_style-black-black.svg)](https://github.com/psf/black)\n\n[![Python](https://img.shields.io/pypi/pyversions/innvestigate.svg)](https://badge.fury.io/py/innvestigate)\n[![TensorFlow package version](https://img.shields.io/badge/TensorFlow-2.6_--_2.11-orange.svg)](https://github.com/albermax/innvestigate)\n\n![Different explanation methods on ImageNet.](https://github.com/albermax/innvestigate/raw/master/examples/images/analysis_grid.png)\n\n## Table of contents\n\n* [Introduction](#introduction)\n* [Installation](#installation)\n* [Usage and Examples](#usage-and-examples)\n* [More documentation](#more-documentation)\n* [Contributing](#contributing)\n* [Releases](#releases)\n\n## Introduction\n\nIn the recent years neural networks furthered the state of the art in many domains like, e.g., object detection and speech recognition.\nDespite the success neural networks are typically still treated as black boxes. Their internal workings are not fully understood and the basis for their predictions is unclear.\nIn the attempt to understand neural networks better several methods were proposed, e.g., Saliency, Deconvnet, GuidedBackprop, SmoothGrad, IntegratedGradients, LRP, PatternNet and PatternAttribution.\nDue to the lack of a reference implementations comparing them is a major effort.\nThis library addresses this by providing a common interface and out-of-the-box implementation for many analysis methods.\nOur goal is to make analyzing neural networks\' predictions easy!\n\n\n### If you use this code please star the repository and cite the following paper:\n\n[Alber, M., Lapuschkin, S., Seegerer, P., Hägele, M., Schütt, K. T., Montavon, G., Samek, W., Müller, K. R., Dähne, S., & Kindermans, P. J. (2019). **iNNvestigate neural networks!** Journal of Machine Learning Research, 20.](https://jmlr.org/papers/v20/18-540.html)\n  ```\n  @article{JMLR:v20:18-540,\n  author  = {Maximilian Alber and Sebastian Lapuschkin and Philipp Seegerer and Miriam H{{\\"a}}gele and Kristof T. Sch{{\\"u}}tt and Gr{{\\\'e}}goire Montavon and Wojciech Samek and Klaus-Robert M{{\\"u}}ller and Sven D{{\\"a}}hne and Pieter-Jan Kindermans},\n  title   = {iNNvestigate Neural Networks!},\n  journal = {Journal of Machine Learning Research},\n  year    = {2019},\n  volume  = {20},\n  number  = {93},\n  pages   = {1-8},\n  url     = {http://jmlr.org/papers/v20/18-540.html}\n  }\n  ```\n\n## Installation\n\niNNvestigate is based on Keras and TensorFlow 2 and can be installed with the following commands:\n\n```bash\npip install innvestigate\n```\n\n**Please note that iNNvestigate currently requires disabling TF2\'s eager execution.**\n\nTo use the example scripts and notebooks one additionally needs to install the package matplotlib:\n\n```bash\npip install matplotlib\n```\n\nThe library\'s tests can be executed via `pytest`. The easiest way to do reproducible development on iNNvestigate is to install all dev dependencies via [Poetry](https://python-poetry.org):\n```bash\ngit clone https://github.com/albermax/innvestigate.git\ncd innvestigate\n\npoetry install\npoetry run pytest\n```\n\n## Usage and Examples\n\nThe iNNvestigate library contains implementations for the following methods:\n\n* *function:*\n  * **gradient:** The gradient of the output neuron with respect to the input.\n  * **smoothgrad:** [SmoothGrad](https://arxiv.org/abs/1706.03825) averages the gradient over number of inputs with added noise.\n* *signal:*\n  * **deconvnet:** [DeConvNet](https://arxiv.org/abs/1311.2901) applies a ReLU in the gradient computation instead of the gradient of a ReLU.\n  * **guided:** [Guided BackProp](https://arxiv.org/abs/1412.6806) applies a ReLU in the gradient computation additionally to the gradient of a ReLU.\n  * **pattern.net:** [PatternNet](https://arxiv.org/abs/1705.05598) estimates the input signal of the output neuron. (*Note: not available in iNNvestigate 2.0*)\n* *attribution:*\n  * **input_t_gradient:** Input \\* Gradient\n  * **deep_taylor[.bounded]:** [DeepTaylor](https://www.sciencedirect.com/science/article/pii/S0031320316303582?via%3Dihub) computes for each neuron a root point, that is close to the input, but which\'s output value is 0, and uses this difference to estimate the attribution of each neuron recursively.\n  * **lrp.\\*:** [LRP](http://journals.plos.org/plosone/article?id=10.1371/journal.pone.0130140) attributes recursively to each neuron\'s input relevance proportional to its contribution of the neuron output.\n  * **integrated_gradients:** [IntegratedGradients](https://arxiv.org/abs/1703.01365) integrates the gradient along a path from the input to a reference.\n* *miscellaneous:*\n  * **input:** Returns the input.\n  * **random:** Returns random Gaussian noise.\n\n**The intention behind iNNvestigate is to make it easy to use analysis methods, but it is not to explain the underlying concepts and assumptions. Please, read the according publication(s) when using a certain method and when publishing please cite the according paper(s) (as well as the [iNNvestigate paper](https://arxiv.org/abs/1808.04260)). Thank you!**\n\nAll the available methods have in common that they try to analyze the output of a specific neuron with respect to input to the neural network.\nTypically one analyses the neuron with the largest activation in the output layer.\nFor example, given a Keras model, one can create a \'gradient\' analyzer:\n\n```python\nimport tensorflow as tf\nimport innvestigate\ntf.compat.v1.disable_eager_execution()\n\nmodel = create_keras_model()\n\nanalyzer = innvestigate.create_analyzer("gradient", model)\n```\n\nand analyze the influence of the neural network\'s input on the output neuron by:\n\n```python\nanalysis = analyzer.analyze(inputs)\n```\n\nTo analyze a neuron with the index i, one can use the following scheme:\n\n```python\nanalyzer = innvestigate.create_analyzer("gradient",\n                                        model,\n\t\t\t\t\tneuron_selection_mode="index")\nanalysis = analyzer.analyze(inputs, i)\n```\n\nLet\'s look at an example ([code](https://github.com/albermax/innvestigate/blob/master/examples/readme_code_snippet.py)) with VGG16 and this image:\n\n![Input image.](https://github.com/albermax/innvestigate/raw/master/examples/images/readme_example_input.png)\n\n\n```python\nimport tensorflow as tf\nimport tensorflow.keras.applications.vgg16 as vgg16\ntf.compat.v1.disable_eager_execution()\n\nimport innvestigate\n\n# Get model\nmodel, preprocess = vgg16.VGG16(), vgg16.preprocess_input\n# Strip softmax layer\nmodel = innvestigate.model_wo_softmax(model)\n\n# Create analyzer\nanalyzer = innvestigate.create_analyzer("deep_taylor", model)\n\n# Add batch axis and preprocess\nx = preprocess(image[None])\n# Apply analyzer w.r.t. maximum activated output-neuron\na = analyzer.analyze(x)\n\n# Aggregate along color channels and normalize to [-1, 1]\na = a.sum(axis=np.argmax(np.asarray(a.shape) == 3))\na /= np.max(np.abs(a))\n# Plot\nplt.imshow(a[0], cmap="seismic", clim=(-1, 1))\n```\n\n![Analysis image.](https://github.com/albermax/innvestigate/raw/master/examples/images/readme_example_analysis.png)\n\n### Tutorials\n\nIn the directory [examples](https://github.com/albermax/innvestigate/blob/master/examples/) one can find different examples as Python scripts and as Jupyter notebooks:\n\n* **[Introduction to iNNvestigate](https://github.com/albermax/innvestigate/blob/master/examples/notebooks/introduction.ipynb):** shows how to use **iNNvestigate**.\n* **[Comparing methods on MNIST](https://github.com/albermax/innvestigate/blob/master/examples/notebooks/mnist_compare_methods.ipynb):** shows how to train and compare analyzers on MNIST.\n* **[Comparing output neurons on MNIST](https://github.com/albermax/innvestigate/blob/master/examples/notebooks/mnist_neuron_selection.ipynb):** shows how to analyze the prediction of different classes on MNIST.\n* **[Comparing methods on ImageNet](https://github.com/albermax/innvestigate/blob/master/examples/notebooks/imagenet_compare_methods.ipynb):** shows how to compare analyzers on ImageNet.\n* **[Comparing networks on ImageNet](https://github.com/albermax/innvestigate/blob/master/examples/notebooks/imagenet_compare_networks.ipynb):** shows how to compare analyzes for different networks on ImageNet.\n* **[Sentiment Analysis](https://github.com/albermax/innvestigate/blob/master/examples/notebooks/sentiment_analysis.ipynb)**.\n* **[Development with iNNvestigate](https://github.com/albermax/innvestigate/blob/master/examples/notebooks/introduction_development.ipynb):** shows how to develop with **iNNvestigate**.\n* **[Perturbation Analysis](https://github.com/albermax/innvestigate/blob/master/examples/notebooks/mnist_perturbation.ipynb)**.\n---\n\n**To use the ImageNet examples please download the example images first ([script](https://github.com/albermax/innvestigate/blob/master/examples/images/wget_imagenet_2011_samples.sh)).**\n\n## More documentation\n\n... can be found here:\n\n* Alber, M., Lapuschkin, S., Seegerer, P., Hägele, M., Schütt, K. T., Montavon, G., Samek, W., Müller, K. R., Dähne, S., & Kindermans, P. J. (2019). INNvestigate neural networks! Journal of Machine Learning Research, 20.](https://jmlr.org/papers/v20/18-540.html)\n  ```\n  @article{JMLR:v20:18-540,\n  author  = {Maximilian Alber and Sebastian Lapuschkin and Philipp Seegerer and Miriam H{{\\"a}}gele and Kristof T. Sch{{\\"u}}tt and Gr{{\\\'e}}goire Montavon and Wojciech Samek and Klaus-Robert M{{\\"u}}ller and Sven D{{\\"a}}hne and Pieter-Jan Kindermans},\n  title   = {iNNvestigate Neural Networks!},\n  journal = {Journal of Machine Learning Research},\n  year    = {2019},\n  volume  = {20},\n  number  = {93},\n  pages   = {1-8},\n  url     = {http://jmlr.org/papers/v20/18-540.html}\n  }\n  ```\n* [https://innvestigate.readthedocs.io/en/latest/](https://innvestigate.readthedocs.io/en/latest/)\n\n## Contributing\n\nIf you would like to contribute or add your analysis method \nplease open an issue or submit a pull request.\n\n## Releases\n\n[Can be found here.](https://github.com/albermax/innvestigate/blob/master/VERSION.md)\n\n\n## Acknowledgements\n\n> Adrian Hill acknowledges support by the Federal Ministry of Education and Research (BMBF) for the Berlin Institute for the Foundations of Learning and Data (BIFOLD) (01IS18037A).',
-    'author': 'Maxmilian Alber',
-    'author_email': 'workDoTalberDoTmaximilian@gmail.com',
-    'maintainer': 'Adrian Hill',
-    'maintainer_email': 'hill@tu-berlin.de',
-    'url': 'https://github.com/albermax/innvestigate',
-    'package_dir': package_dir,
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'python_requires': '>=3.8,<3.11',
-}
+[Can be found here.](https://github.com/albermax/innvestigate/blob/master/VERSION.md)
 
 
-setup(**setup_kwargs)
+## Acknowledgements
+
+> Adrian Hill acknowledges support by the Federal Ministry of Education and Research (BMBF) for the Berlin Institute for the Foundations of Learning and Data (BIFOLD) (01IS18037A).
```

