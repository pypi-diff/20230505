# Comparing `tmp/numalogic-0.3.8.tar.gz` & `tmp/numalogic-0.4.dev3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "numalogic-0.3.8.tar", max compression
+gzip compressed data, was "numalogic-0.4.dev3.tar", max compression
```

## Comparing `numalogic-0.3.8.tar` & `numalogic-0.4.dev3.tar`

### file list

```diff
@@ -1,39 +1,42 @@
--rw-r--r--   0        0        0    11357 2023-04-18 18:28:11.595020 numalogic-0.3.8/LICENSE
--rw-r--r--   0        0        0     5248 2023-04-18 18:28:11.595020 numalogic-0.3.8/README.md
--rw-r--r--   0        0        0      895 2023-04-18 18:28:11.619021 numalogic-0.3.8/numalogic/__init__.py
--rw-r--r--   0        0        0      729 2023-04-18 18:28:11.619021 numalogic-0.3.8/numalogic/_constants.py
--rw-r--r--   0        0        0     1004 2023-04-18 18:28:11.619021 numalogic-0.3.8/numalogic/config/__init__.py
--rw-r--r--   0        0        0     2315 2023-04-18 18:28:11.619021 numalogic-0.3.8/numalogic/config/_config.py
--rw-r--r--   0        0        0     2824 2023-04-18 18:28:11.619021 numalogic-0.3.8/numalogic/config/factory.py
--rw-r--r--   0        0        0        0 2023-04-18 18:28:11.623021 numalogic-0.3.8/numalogic/models/__init__.py
--rw-r--r--   0        0        0      683 2023-04-18 18:28:11.623021 numalogic-0.3.8/numalogic/models/autoencoder/__init__.py
--rw-r--r--   0        0        0     2759 2023-04-18 18:28:11.623021 numalogic-0.3.8/numalogic/models/autoencoder/base.py
--rw-r--r--   0        0        0     2065 2023-04-18 18:28:11.623021 numalogic-0.3.8/numalogic/models/autoencoder/trainer.py
--rw-r--r--   0        0        0      581 2023-04-18 18:28:11.623021 numalogic-0.3.8/numalogic/models/autoencoder/variants/__init__.py
--rw-r--r--   0        0        0    11308 2023-04-18 18:28:11.623021 numalogic-0.3.8/numalogic/models/autoencoder/variants/conv.py
--rw-r--r--   0        0        0     6654 2023-04-18 18:28:11.623021 numalogic-0.3.8/numalogic/models/autoencoder/variants/lstm.py
--rw-r--r--   0        0        0    14372 2023-04-18 18:28:11.623021 numalogic-0.3.8/numalogic/models/autoencoder/variants/transformer.py
--rw-r--r--   0        0        0     8315 2023-04-18 18:28:11.623021 numalogic-0.3.8/numalogic/models/autoencoder/variants/vanilla.py
--rw-r--r--   0        0        0        0 2023-04-18 18:28:11.623021 numalogic-0.3.8/numalogic/models/forecast/__init__.py
--rw-r--r--   0        0        0      158 2023-04-18 18:28:11.623021 numalogic-0.3.8/numalogic/models/forecast/variants/__init__.py
--rw-r--r--   0        0        0     4323 2023-04-18 18:28:11.623021 numalogic-0.3.8/numalogic/models/forecast/variants/naive.py
--rw-r--r--   0        0        0      211 2023-04-18 18:28:11.623021 numalogic-0.3.8/numalogic/models/threshold/__init__.py
--rw-r--r--   0        0        0     4062 2023-04-18 18:28:11.623021 numalogic-0.3.8/numalogic/models/threshold/_static.py
--rw-r--r--   0        0        0     2518 2023-04-18 18:28:11.623021 numalogic-0.3.8/numalogic/models/threshold/_std.py
--rw-r--r--   0        0        0     6087 2023-04-18 18:28:11.623021 numalogic-0.3.8/numalogic/postprocess.py
--rw-r--r--   0        0        0      746 2023-04-18 18:28:11.623021 numalogic-0.3.8/numalogic/preprocess/__init__.py
--rw-r--r--   0        0        0     3654 2023-04-18 18:28:11.623021 numalogic-0.3.8/numalogic/preprocess/transformer.py
--rw-r--r--   0        0        0      906 2023-04-18 18:28:11.623021 numalogic-0.3.8/numalogic/registry/__init__.py
--rw-r--r--   0        0        0     2561 2023-04-18 18:28:11.623021 numalogic-0.3.8/numalogic/registry/artifact.py
--rw-r--r--   0        0        0    11670 2023-04-18 18:28:11.623021 numalogic-0.3.8/numalogic/registry/mlflow_registry.py
--rw-r--r--   0        0        0      841 2023-04-18 18:28:11.623021 numalogic-0.3.8/numalogic/synthetic/__init__.py
--rw-r--r--   0        0        0    11583 2023-04-18 18:28:11.623021 numalogic-0.3.8/numalogic/synthetic/anomalies.py
--rw-r--r--   0        0        0     1651 2023-04-18 18:28:11.623021 numalogic-0.3.8/numalogic/synthetic/sparsity.py
--rw-r--r--   0        0        0     3712 2023-04-18 18:28:11.623021 numalogic-0.3.8/numalogic/synthetic/timeseries.py
--rw-r--r--   0        0        0      215 2023-04-18 18:28:11.623021 numalogic-0.3.8/numalogic/tools/__init__.py
--rw-r--r--   0        0        0     1789 2023-04-18 18:28:11.623021 numalogic-0.3.8/numalogic/tools/callbacks.py
--rw-r--r--   0        0        0     5960 2023-04-18 18:28:11.623021 numalogic-0.3.8/numalogic/tools/data.py
--rw-r--r--   0        0        0      979 2023-04-18 18:28:11.623021 numalogic-0.3.8/numalogic/tools/exceptions.py
--rw-r--r--   0        0        0     1059 2023-04-18 18:28:11.623021 numalogic-0.3.8/numalogic/tools/types.py
--rw-r--r--   0        0        0     2013 2023-04-18 18:28:11.623021 numalogic-0.3.8/pyproject.toml
--rw-r--r--   0        0        0     6575 1970-01-01 00:00:00.000000 numalogic-0.3.8/PKG-INFO
+-rw-r--r--   0        0        0    11357 2023-05-05 18:43:20.600149 numalogic-0.4.dev3/LICENSE
+-rw-r--r--   0        0        0     5150 2023-05-05 18:43:20.600149 numalogic-0.4.dev3/README.md
+-rw-r--r--   0        0        0      895 2023-05-05 18:43:20.648150 numalogic-0.4.dev3/numalogic/__init__.py
+-rw-r--r--   0        0        0      729 2023-05-05 18:43:20.648150 numalogic-0.4.dev3/numalogic/_constants.py
+-rw-r--r--   0        0        0     1004 2023-05-05 18:43:20.648150 numalogic-0.4.dev3/numalogic/config/__init__.py
+-rw-r--r--   0        0        0     2479 2023-05-05 18:43:20.648150 numalogic-0.4.dev3/numalogic/config/_config.py
+-rw-r--r--   0        0        0     3189 2023-05-05 18:43:20.648150 numalogic-0.4.dev3/numalogic/config/factory.py
+-rw-r--r--   0        0        0        0 2023-05-05 18:43:20.648150 numalogic-0.4.dev3/numalogic/models/__init__.py
+-rw-r--r--   0        0        0      683 2023-05-05 18:43:20.648150 numalogic-0.4.dev3/numalogic/models/autoencoder/__init__.py
+-rw-r--r--   0        0        0     3829 2023-05-05 18:43:20.648150 numalogic-0.4.dev3/numalogic/models/autoencoder/base.py
+-rw-r--r--   0        0        0     2065 2023-05-05 18:43:20.648150 numalogic-0.4.dev3/numalogic/models/autoencoder/trainer.py
+-rw-r--r--   0        0        0      581 2023-05-05 18:43:20.648150 numalogic-0.4.dev3/numalogic/models/autoencoder/variants/__init__.py
+-rw-r--r--   0        0        0    11206 2023-05-05 18:43:20.648150 numalogic-0.4.dev3/numalogic/models/autoencoder/variants/conv.py
+-rw-r--r--   0        0        0     6581 2023-05-05 18:43:20.648150 numalogic-0.4.dev3/numalogic/models/autoencoder/variants/lstm.py
+-rw-r--r--   0        0        0    14239 2023-05-05 18:43:20.648150 numalogic-0.4.dev3/numalogic/models/autoencoder/variants/transformer.py
+-rw-r--r--   0        0        0     8271 2023-05-05 18:43:20.648150 numalogic-0.4.dev3/numalogic/models/autoencoder/variants/vanilla.py
+-rw-r--r--   0        0        0        0 2023-05-05 18:43:20.648150 numalogic-0.4.dev3/numalogic/models/forecast/__init__.py
+-rw-r--r--   0        0        0      158 2023-05-05 18:43:20.652150 numalogic-0.4.dev3/numalogic/models/forecast/variants/__init__.py
+-rw-r--r--   0        0        0     4291 2023-05-05 18:43:20.652150 numalogic-0.4.dev3/numalogic/models/forecast/variants/naive.py
+-rw-r--r--   0        0        0      211 2023-05-05 18:43:20.652150 numalogic-0.4.dev3/numalogic/models/threshold/__init__.py
+-rw-r--r--   0        0        0     4048 2023-05-05 18:43:20.652150 numalogic-0.4.dev3/numalogic/models/threshold/_static.py
+-rw-r--r--   0        0        0     2490 2023-05-05 18:43:20.652150 numalogic-0.4.dev3/numalogic/models/threshold/_std.py
+-rw-r--r--   0        0        0     6087 2023-05-05 18:43:20.652150 numalogic-0.4.dev3/numalogic/postprocess.py
+-rw-r--r--   0        0        0      746 2023-05-05 18:43:20.652150 numalogic-0.4.dev3/numalogic/preprocess/__init__.py
+-rw-r--r--   0        0        0     3654 2023-05-05 18:43:20.652150 numalogic-0.4.dev3/numalogic/preprocess/transformer.py
+-rw-r--r--   0        0        0     1142 2023-05-05 18:43:20.652150 numalogic-0.4.dev3/numalogic/registry/__init__.py
+-rw-r--r--   0        0        0      328 2023-05-05 18:43:20.652150 numalogic-0.4.dev3/numalogic/registry/_serialize.py
+-rw-r--r--   0        0        0     4571 2023-05-05 18:43:20.652150 numalogic-0.4.dev3/numalogic/registry/artifact.py
+-rw-r--r--   0        0        0     1608 2023-05-05 18:43:20.652150 numalogic-0.4.dev3/numalogic/registry/localcache.py
+-rw-r--r--   0        0        0    12045 2023-05-05 18:43:20.652150 numalogic-0.4.dev3/numalogic/registry/mlflow_registry.py
+-rw-r--r--   0        0        0     8636 2023-05-05 18:43:20.652150 numalogic-0.4.dev3/numalogic/registry/redis_registry.py
+-rw-r--r--   0        0        0      841 2023-05-05 18:43:20.652150 numalogic-0.4.dev3/numalogic/synthetic/__init__.py
+-rw-r--r--   0        0        0    11738 2023-05-05 18:43:20.652150 numalogic-0.4.dev3/numalogic/synthetic/anomalies.py
+-rw-r--r--   0        0        0     1650 2023-05-05 18:43:20.652150 numalogic-0.4.dev3/numalogic/synthetic/sparsity.py
+-rw-r--r--   0        0        0     3752 2023-05-05 18:43:20.652150 numalogic-0.4.dev3/numalogic/synthetic/timeseries.py
+-rw-r--r--   0        0        0      215 2023-05-05 18:43:20.652150 numalogic-0.4.dev3/numalogic/tools/__init__.py
+-rw-r--r--   0        0        0     1866 2023-05-05 18:43:20.652150 numalogic-0.4.dev3/numalogic/tools/callbacks.py
+-rw-r--r--   0        0        0     6218 2023-05-05 18:43:20.652150 numalogic-0.4.dev3/numalogic/tools/data.py
+-rw-r--r--   0        0        0     1082 2023-05-05 18:43:20.652150 numalogic-0.4.dev3/numalogic/tools/exceptions.py
+-rw-r--r--   0        0        0     1399 2023-05-05 18:43:20.652150 numalogic-0.4.dev3/numalogic/tools/types.py
+-rw-r--r--   0        0        0     2338 2023-05-05 18:43:20.652150 numalogic-0.4.dev3/pyproject.toml
+-rw-r--r--   0        0        0     6511 1970-01-01 00:00:00.000000 numalogic-0.4.dev3/PKG-INFO
```

### Comparing `numalogic-0.3.8/LICENSE` & `numalogic-0.4.dev3/LICENSE`

 * *Files identical despite different names*

### Comparing `numalogic-0.3.8/README.md` & `numalogic-0.4.dev3/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -5,35 +5,35 @@
 [![black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/ambv/black)
 [![License](https://img.shields.io/badge/License-Apache%202.0-blue.svg)](LICENSE)
 [![slack](https://img.shields.io/badge/slack-numaproj-brightgreen.svg?logo=slack)](https://join.slack.com/t/numaproj/shared_invite/zt-19svuv47m-YKHhsQ~~KK9mBv1E7pNzfg)
 [![Release Version](https://img.shields.io/github/v/release/numaproj/numalogic?label=numalogic)](https://github.com/numaproj/numalogic/releases/latest)
 
 
 ## Background
-Numalogic is a collection of ML models and algorithms for operation data analytics and AIOps. 
-At Intuit, we use Numalogic at scale for continuous real-time data enrichment including 
-anomaly scoring. We assign an anomaly score (ML inference) to any time-series 
-datum/event/message we receive on our streaming platform (say, Kafka). 95% of our 
-data sets are time-series, and we have a complex flowchart to execute ML inference on 
-our high throughput sources. We run multiple models on the same datum, say a model that is 
-sensitive towards +ve sentiments, another more tuned towards -ve sentiments, and another 
-optimized for neutral sentiments. We also have a couple of ML models trained for the same 
-data source to provide more accurate scores based on the data density in our model store. 
-An ensemble of models is required because some composite keys in the data tend to be less 
-dense than others, e.g., forgot-password interaction is less frequent than a status check 
-interaction. At runtime, for each datum that arrives, models are picked based on a conditional 
-forwarding filter set on the data density. ML engineers need to worry about only their 
+Numalogic is a collection of ML models and algorithms for operation data analytics and AIOps.
+At Intuit, we use Numalogic at scale for continuous real-time data enrichment including
+anomaly scoring. We assign an anomaly score (ML inference) to any time-series
+datum/event/message we receive on our streaming platform (say, Kafka). 95% of our
+data sets are time-series, and we have a complex flowchart to execute ML inference on
+our high throughput sources. We run multiple models on the same datum, say a model that is
+sensitive towards +ve sentiments, another more tuned towards -ve sentiments, and another
+optimized for neutral sentiments. We also have a couple of ML models trained for the same
+data source to provide more accurate scores based on the data density in our model store.
+An ensemble of models is required because some composite keys in the data tend to be less
+dense than others, e.g., forgot-password interaction is less frequent than a status check
+interaction. At runtime, for each datum that arrives, models are picked based on a conditional
+forwarding filter set on the data density. ML engineers need to worry about only their
 inference container; they do not have to worry about data movement and quality assurance.
 
-## Numalogic realtime training 
-For an always-on ML platform, the key requirement is the ability to train or retrain models 
-automatically based on the incoming messages. The composite key built at per message runtime 
-looks for a matching model, and if the model turns out to be stale or missing, an automatic 
-retriggering is applied. The conditional forwarding feature of the platform improves the 
-development velocity of the ML developer when they have to make a decision whether to forward 
+## Numalogic realtime training
+For an always-on ML platform, the key requirement is the ability to train or retrain models
+automatically based on the incoming messages. The composite key built at per message runtime
+looks for a matching model, and if the model turns out to be stale or missing, an automatic
+retriggering is applied. The conditional forwarding feature of the platform improves the
+development velocity of the ML developer when they have to make a decision whether to forward
 the result further or drop it after a trigger request.
 
 
 ## Key Features
 
 1. Ease of use: simple and efficient tools for predictive data analytics
 2. Reusability: all the functionalities can be re-used in various contexts
@@ -55,25 +55,20 @@
 
 
 ## Installation
 
 Numalogic requires Python 3.8 or higher.
 
 ### Prerequisites
-Numalogic needs [PyTorch](https://pytorch.org/) and 
-[PyTorch Lightning](https://pytorch-lightning.readthedocs.io/en/stable/) to work. 
-But since these packages are platform dependendent, 
+Numalogic needs [PyTorch](https://pytorch.org/) and
+[PyTorch Lightning](https://pytorch-lightning.readthedocs.io/en/stable/) to work.
+But since these packages are platform dependendent,
 they are not included in the numalogic package itself. Kindly install them first.
 
-Numalogic supports the following pytorch versions:
-- 1.11.x
-- 1.12.x
-- 1.13.x
-
-Other versions do work, it is just that they are not tested.
+Numalogic supports pytorch versions `2.0.0` and above.
 
 numalogic can be installed using pip.
 ```shell
 pip install numalogic
 ```
 
 If using mlflow for model registry, install using:
@@ -99,15 +94,15 @@
     ```
     poetry install --all-extras
     ```
 4. To run unit tests:
     ```
     make test
     ```
-5. To format code style using black:
+5. To format code style using black and ruff:
     ```
     make lint
     ```
 
 ## Contributing
 We would love contributions in the numalogic project in one of the following (but not limited to) areas:
```

### Comparing `numalogic-0.3.8/numalogic/__init__.py` & `numalogic-0.4.dev3/numalogic/__init__.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.3.8/numalogic/_constants.py` & `numalogic-0.4.dev3/numalogic/_constants.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.3.8/numalogic/config/__init__.py` & `numalogic-0.4.dev3/numalogic/config/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,26 +6,26 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 
-from numalogic.config._config import NumalogicConf, ModelInfo, LightningTrainerConf, RegistryConf
+from numalogic.config._config import NumalogicConf, ModelInfo, LightningTrainerConf, RegistryInfo
 from numalogic.config.factory import (
     ModelFactory,
     PreprocessFactory,
     PostprocessFactory,
     ThresholdFactory,
 )
 
 
 __all__ = [
     "NumalogicConf",
     "ModelInfo",
     "LightningTrainerConf",
-    "RegistryConf",
+    "RegistryInfo",
     "ModelFactory",
     "PreprocessFactory",
     "PostprocessFactory",
     "ThresholdFactory",
 ]
```

### Comparing `numalogic-0.3.8/numalogic/config/_config.py` & `numalogic-0.4.dev3/numalogic/config/_config.py`

 * *Files 14% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 
 from dataclasses import dataclass, field
-from typing import List, Optional, Any, Dict
+from typing import Optional, Any
 
 from omegaconf import MISSING
 
 
 @dataclass
 class ModelInfo:
     """
@@ -25,36 +25,42 @@
         name: name of the model; this should map to a supported list of models
               mentioned in the factory file
         conf: kwargs for instantiating the model class
         stateful: flag indicating if the model is stateful or not
     """
 
     name: str = MISSING
-    conf: Dict[str, Any] = field(default_factory=dict)
+    conf: dict[str, Any] = field(default_factory=dict)
     stateful: bool = True
 
 
 @dataclass
-class RegistryConf:
-    # TODO implement this
+class RegistryInfo:
     """
     Registry config base class
+
+    Args:
+        name: name of the registry
+        conf: kwargs for instantiating the model class
     """
-    pass
+
+    name: str = MISSING
+    conf: dict[str, Any] = field(default_factory=dict)
 
 
 @dataclass
 class LightningTrainerConf:
     """
     Schema for defining the Pytorch Lightning trainer behavior.
 
     More details on the arguments are provided here:
     https://pytorch-lightning.readthedocs.io/en/stable/common/trainer.html#trainer-class-api
     """
 
+    accelerator: str = "auto"
     max_epochs: int = 100
     logger: bool = False
     check_val_every_n_epoch: int = 5
     log_every_n_steps: int = 20
     enable_checkpointing: bool = False
     enable_progress_bar: bool = True
     enable_model_summary: bool = True
@@ -66,11 +72,11 @@
 class NumalogicConf:
     """
     Top level config schema for numalogic.
     """
 
     model: ModelInfo = field(default_factory=ModelInfo)
     trainer: LightningTrainerConf = field(default_factory=LightningTrainerConf)
-    registry: RegistryConf = field(default_factory=RegistryConf)
-    preprocess: List[ModelInfo] = field(default_factory=list)
+    registry: RegistryInfo = field(default_factory=RegistryInfo)
+    preprocess: list[ModelInfo] = field(default_factory=list)
     threshold: ModelInfo = field(default_factory=ModelInfo)
     postprocess: ModelInfo = field(default_factory=ModelInfo)
```

### Comparing `numalogic-0.3.8/numalogic/config/factory.py` & `numalogic-0.4.dev3/numalogic/config/factory.py`

 * *Files 9% similar despite different names*

```diff
@@ -4,48 +4,55 @@
 # You may obtain a copy of the License at
 #     http://www.apache.org/licenses/LICENSE-2.0
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
+from typing import Union
+
 from sklearn.preprocessing import StandardScaler, MinMaxScaler, MaxAbsScaler, RobustScaler
 
-from numalogic.config._config import ModelInfo
+from numalogic.config._config import ModelInfo, RegistryInfo
 from numalogic.models.autoencoder.variants import (
     VanillaAE,
     SparseVanillaAE,
     Conv1dAE,
     SparseConv1dAE,
     LSTMAE,
     SparseLSTMAE,
     TransformerAE,
     SparseTransformerAE,
 )
 from numalogic.models.threshold import StdDevThreshold, StaticThreshold, SigmoidThreshold
 from numalogic.postprocess import TanhNorm, ExpMovingAverage
 from numalogic.preprocess import LogTransformer, StaticPowerTransformer, TanhScaler
+from numalogic.registry import MLflowRegistry, RedisRegistry
 from numalogic.tools.exceptions import UnknownConfigArgsError
 
 
 class _ObjectFactory:
     _CLS_MAP = {}
 
-    def get_instance(self, model_info: ModelInfo):
+    def get_instance(self, object_info: Union[ModelInfo, RegistryInfo]):
         try:
-            _cls = self._CLS_MAP[model_info.name]
-        except KeyError:
-            raise UnknownConfigArgsError(f"Invalid model info instance provided: {model_info}")
-        return _cls(**model_info.conf)
+            _cls = self._CLS_MAP[object_info.name]
+        except KeyError as err:
+            raise UnknownConfigArgsError(
+                f"Invalid model info instance provided: {object_info}"
+            ) from err
+        return _cls(**object_info.conf)
 
-    def get_cls(self, model_info: ModelInfo):
+    def get_cls(self, object_info: Union[ModelInfo, RegistryInfo]):
         try:
-            return self._CLS_MAP[model_info.name]
-        except KeyError:
-            raise UnknownConfigArgsError(f"Invalid model info instance provided: {model_info}")
+            return self._CLS_MAP[object_info.name]
+        except KeyError as err:
+            raise UnknownConfigArgsError(
+                f"Invalid model info instance provided: {object_info}"
+            ) from err
 
 
 class PreprocessFactory(_ObjectFactory):
     _CLS_MAP = {
         "StandardScaler": StandardScaler,
         "MinMaxScaler": MinMaxScaler,
         "MaxAbsScaler": MaxAbsScaler,
@@ -53,18 +60,15 @@
         "LogTransformer": LogTransformer,
         "StaticPowerTransformer": StaticPowerTransformer,
         "TanhScaler": TanhScaler,
     }
 
 
 class PostprocessFactory(_ObjectFactory):
-    _CLS_MAP = {
-        "TanhNorm": TanhNorm,
-        "ExpMovingAverage": ExpMovingAverage,
-    }
+    _CLS_MAP = {"TanhNorm": TanhNorm, "ExpMovingAverage": ExpMovingAverage}
 
 
 class ThresholdFactory(_ObjectFactory):
     _CLS_MAP = {
         "StdDevThreshold": StdDevThreshold,
         "StaticThreshold": StaticThreshold,
         "SigmoidThreshold": SigmoidThreshold,
@@ -78,7 +82,14 @@
         "Conv1dAE": Conv1dAE,
         "SparseConv1dAE": SparseConv1dAE,
         "LSTMAE": LSTMAE,
         "SparseLSTMAE": SparseLSTMAE,
         "TransformerAE": TransformerAE,
         "SparseTransformerAE": SparseTransformerAE,
     }
+
+
+class RegistryFactory(_ObjectFactory):
+    _CLS_MAP = {
+        "RedisRegistry": RedisRegistry,
+        "MLflowRegistry": MLflowRegistry,
+    }
```

### Comparing `numalogic-0.3.8/numalogic/models/autoencoder/__init__.py` & `numalogic-0.4.dev3/numalogic/models/autoencoder/__init__.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.3.8/numalogic/models/autoencoder/base.py` & `numalogic-0.4.dev3/numalogic/models/autoencoder/base.py`

 * *Files 27% similar despite different names*

```diff
@@ -7,49 +7,81 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 
 from abc import ABCMeta
-from typing import Any, Dict
+from typing import Any
 
 import pytorch_lightning as pl
 import torch.nn.functional as F
 from torch import Tensor, optim
 
 
 class BaseAE(pl.LightningModule, metaclass=ABCMeta):
-    """
+    r"""
     Abstract Base class for all Pytorch based autoencoder models for time-series data.
+
+    Args:
+        loss_fn: loss function used to train the model
+                 supported values include: {huber, l1, mae}
+        optim_algo: optimizer algo to be used for training
+                    supported values include: {adam, adagrad, rmsprop}
+        lr: learning rate (default: 1e-3)
+        weight_decay: weight decay factor weight for regularization (default: 0.0)
     """
 
-    def __init__(self, loss_fn: str = "huber", optim_algo: str = "adam", lr: float = 1e-3):
+    def __init__(
+        self,
+        loss_fn: str = "huber",
+        optim_algo: str = "adam",
+        lr: float = 1e-3,
+        weight_decay: float = 0.0,
+    ):
         super().__init__()
         self.lr = lr
         self.optim_algo = optim_algo
         self.criterion = self.init_criterion(loss_fn)
+        self.weight_decay = weight_decay
+
+        self._total_train_loss = 0.0
+        self._total_val_loss = 0.0
+
+    @property
+    def total_train_loss(self):
+        return self._total_train_loss
+
+    @property
+    def total_val_loss(self):
+        return self._total_val_loss
+
+    def reset_train_loss(self):
+        self._total_train_loss = 0.0
+
+    def reset_val_loss(self):
+        self._total_val_loss = 0.0
 
     @staticmethod
     def init_criterion(loss_fn: str):
         if loss_fn == "huber":
             return F.huber_loss
         if loss_fn == "l1":
             return F.l1_loss
         if loss_fn == "mse":
             return F.mse_loss
         raise NotImplementedError(f"Unsupported loss function provided: {loss_fn}")
 
     def init_optimizer(self, optim_algo: str):
         if optim_algo == "adam":
-            return optim.Adam(self.parameters(), lr=self.lr)
+            return optim.Adam(self.parameters(), lr=self.lr, weight_decay=self.weight_decay)
         if optim_algo == "adagrad":
-            return optim.Adagrad(self.parameters(), lr=self.lr)
+            return optim.Adagrad(self.parameters(), lr=self.lr, weight_decay=self.weight_decay)
         if optim_algo == "rmsprop":
-            return optim.RMSprop(self.parameters(), lr=self.lr)
+            return optim.RMSprop(self.parameters(), lr=self.lr, weight_decay=self.weight_decay)
         raise NotImplementedError(f"Unsupported optimizer value provided: {optim_algo}")
 
     def configure_shape(self, batch: Tensor) -> Tensor:
         """
         Method to configure the batch shape for each type of model architecture.
         """
         return batch
@@ -58,18 +90,20 @@
         _, recon = self.forward(batch)
         return self.criterion(batch, recon)
 
     def reconstruction(self, batch: Tensor) -> Tensor:
         _, recon = self.forward(batch)
         return recon
 
-    def configure_optimizers(self) -> Dict[str, Any]:
+    def configure_optimizers(self) -> dict[str, Any]:
         optimizer = self.init_optimizer(self.optim_algo)
         return {"optimizer": optimizer}
 
     def training_step(self, batch: Tensor, batch_idx: int) -> Tensor:
         loss = self._get_reconstruction_loss(batch)
+        self._total_train_loss += loss.detach().item()
         return loss
 
     def validation_step(self, batch: Tensor, batch_idx: int) -> Tensor:
         loss = self._get_reconstruction_loss(batch)
+        self._total_val_loss += loss.detach().item()
         return loss
```

### Comparing `numalogic-0.3.8/numalogic/models/autoencoder/trainer.py` & `numalogic-0.4.dev3/numalogic/models/autoencoder/trainer.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.3.8/numalogic/models/autoencoder/variants/__init__.py` & `numalogic-0.4.dev3/numalogic/models/autoencoder/variants/__init__.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.3.8/numalogic/models/autoencoder/variants/conv.py` & `numalogic-0.4.dev3/numalogic/models/autoencoder/variants/conv.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,16 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 
 import logging
-from typing import Tuple, Sequence, Union
+from typing import Union
+from collections.abc import Sequence
 
 import torch
 from torch import nn, Tensor
 from torch.nn.init import calculate_gain
 
 from numalogic.models.autoencoder.base import BaseAE
 
@@ -117,23 +118,22 @@
                     ConvBlock(
                         out_channels=num_filters[idx], kernel_size=kernel_sizes[idx], padding=1
                     ),
                     nn.MaxPool1d(pool_k_size),
                 ]
             )
         # Latent layer
-        else:
-            layers.extend(
-                [
-                    nn.LazyConv1d(
-                        out_channels=num_filters[-1], kernel_size=kernel_sizes[-1], padding=1
-                    ),
-                    nn.ReLU(),
-                ]
-            )
+        layers.extend(
+            [
+                nn.LazyConv1d(
+                    out_channels=num_filters[-1], kernel_size=kernel_sizes[-1], padding=1
+                ),
+                nn.ReLU(),
+            ]
+        )
         return layers
 
     def forward(self, input_: Tensor) -> Tensor:
         return self.encoder(input_)
 
 
 class Decoder(nn.Module):
@@ -169,22 +169,21 @@
                 ConvTransposeBlock(
                     out_channels=num_filters[idx], kernel_size=kernel_sizes[idx], padding=1
                 )
             )
             layers.append(nn.Upsample(scale_factor=upscale_factor, mode="linear"))
 
         # Output layer
-        else:
-            layers.append(
-                nn.LazyConvTranspose1d(
-                    out_channels=num_filters[-1], kernel_size=kernel_sizes[-1], padding=1
-                ),
+        layers.append(
+            nn.LazyConvTranspose1d(
+                out_channels=num_filters[-1], kernel_size=kernel_sizes[-1], padding=1
             )
-            if final_activation:
-                layers.append(_get_activation_function(final_activation))
+        )
+        if final_activation:
+            layers.append(_get_activation_function(final_activation))
         return layers
 
     def forward(self, latent: Tensor) -> Tensor:
         return self.decoder(latent)
 
 
 class Conv1dAE(BaseAE):
@@ -229,23 +228,23 @@
             enc_kernel_sizes = [enc_kernel_sizes for _ in range(len(enc_channels))]
 
         elif isinstance(enc_kernel_sizes, (tuple, list)):
             assert len(enc_channels) == len(
                 enc_kernel_sizes
             ), "enc_channels and enc_kernel_sizes should be of the same length"
         else:
-            raise ValueError(f"Invalid enc_kernel_sizes type provided: {enc_kernel_sizes}")
+            raise TypeError(f"Invalid enc_kernel_sizes type provided: {enc_kernel_sizes}")
 
         self.encoder = Encoder(
             num_channels=enc_channels,
             kernel_sizes=enc_kernel_sizes,
             pool_kernel_size=pool_kernel_size,
         )
 
-        dec_channels = list(reversed((enc_channels[:-1])))
+        dec_channels = list(reversed(enc_channels[:-1]))
         dec_channels.append(in_channels)
 
         dec_kernel_sizes = list(reversed(enc_kernel_sizes))
         self.decoder = Decoder(
             num_channels=dec_channels,
             kernel_sizes=dec_kernel_sizes,
             upsample_scale_factor=pool_kernel_size,
@@ -261,15 +260,15 @@
         Initiate parameters in the convolutional
         and transpose convolutional layers.
         """
         for module in self.modules():
             if isinstance(module, (nn.Conv1d, nn.ConvTranspose1d)):
                 nn.init.xavier_normal_(module.weight, gain=calculate_gain("relu"))
 
-    def forward(self, batch: Tensor) -> Tuple[Tensor, Tensor]:
+    def forward(self, batch: Tensor) -> tuple[Tensor, Tensor]:
         batch = self.configure_shape(batch)
         encoded = self.encoder(batch)
         decoded = self.decoder(encoded)
         return encoded, decoded
 
     def configure_shape(self, batch: Tensor) -> Tensor:
         return batch.view(-1, self.in_channels, self.seq_len)
@@ -283,16 +282,15 @@
         x = batch.view(-1, self.in_channels, self.seq_len)
         return self.criterion(x, recon)
 
     def predict_step(self, batch: Tensor, batch_idx: int, dataloader_idx: int = 0) -> Tensor:
         """Returns reconstruction for streaming input"""
         recon = self.reconstruction(batch)
         recon = recon.view(-1, self.seq_len, self.in_channels)
-        recon_err = self.criterion(batch, recon, reduction="none")
-        return recon_err
+        return self.criterion(batch, recon, reduction="none")
 
 
 class SparseConv1dAE(Conv1dAE):
     r"""
     Sparse Autoencoder for a Conv1d network.
     It inherits from VanillaAE class and serves as a wrapper around base network models.
     Sparse Autoencoder is a type of autoencoder that applies sparsity constraint.
```

### Comparing `numalogic-0.3.8/numalogic/models/autoencoder/variants/lstm.py` & `numalogic-0.4.dev3/numalogic/models/autoencoder/variants/lstm.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,15 +7,14 @@
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 
 import logging
-from typing import Tuple
 
 import torch
 import torch.nn as nn
 from torch import Tensor
 from torch.nn.init import calculate_gain
 
 from numalogic.models.autoencoder.base import BaseAE
@@ -81,16 +80,15 @@
 
         self.fc = nn.Linear(self.hidden_size, output_size)
 
     def forward(self, x: Tensor) -> Tensor:
         x = x.unsqueeze(1).repeat(1, self.seq_len, 1)
         x, (_, __) = self.lstm(x)
         x = x.reshape((-1, self.seq_len, self.hidden_size))
-        out = self.fc(x)
-        return out
+        return self.fc(x)
 
 
 class LSTMAE(BaseAE):
     r"""
     Long Short-Term Memory (LSTM) based autoencoder.
 
     Args:
@@ -141,24 +139,23 @@
         """
         for node, param in m.named_parameters():
             if "bias" in node:
                 nn.init.zeros_(param)
             else:
                 nn.init.xavier_normal_(param, gain=calculate_gain("tanh"))
 
-    def forward(self, x: Tensor) -> Tuple[Tensor, Tensor]:
+    def forward(self, x: Tensor) -> tuple[Tensor, Tensor]:
         encoded = self.encoder(x)
         decoded = self.decoder(encoded)
         return encoded, decoded
 
     def predict_step(self, batch: Tensor, batch_idx: int, dataloader_idx: int = 0):
         """Returns reconstruction for streaming input"""
         recon = self.reconstruction(batch)
-        recon_err = self.criterion(batch, recon, reduction="none")
-        return recon_err
+        return self.criterion(batch, recon, reduction="none")
 
 
 class SparseLSTMAE(LSTMAE):
     r"""
     Sparse Autoencoder for an LSTM network.
     It inherits from VanillaAE class and serves as a wrapper around base network models.
     Sparse Autoencoder is a type of autoencoder that applies sparsity constraint.
```

### Comparing `numalogic-0.3.8/numalogic/models/autoencoder/variants/transformer.py` & `numalogic-0.4.dev3/numalogic/models/autoencoder/variants/transformer.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,16 +6,14 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 
-from typing import Tuple
-
 import torch
 import torch.nn.functional
 from numalogic.models.autoencoder.base import BaseAE
 from torch import nn, Tensor
 
 
 def _scaled_dot_product(query: Tensor, key: Tensor, value: Tensor) -> Tensor:
@@ -33,17 +31,15 @@
     temp = query.bmm(key.transpose(1, 2))
     scale = query.size(-1) ** 0.5
     softmax = torch.nn.functional.softmax(temp / scale, dim=-1)
     return softmax.bmm(value)
 
 
 def _positional_encoding(
-    feature: int,
-    seq_len: int,
-    device: torch.device = torch.device("cpu"),
+    feature: int, seq_len: int, device: torch.device = torch.device("cpu")
 ) -> Tensor:
     r"""
     Positional Encoding as described in
     `Attention Is All You Need <https://arxiv.org/abs/1706.03762>`_.
 
     Args:
         feature: number of features
@@ -66,17 +62,15 @@
         dim_input: sequence length / window length (default=1)
         dim_feedforward: the dimension of the feedforward network model (default=2048)
 
     Returns:
         nn.Module type
     """
     return nn.Sequential(
-        nn.Linear(dim_input, dim_feedforward),
-        nn.ReLU(),
-        nn.Linear(dim_feedforward, dim_input),
+        nn.Linear(dim_input, dim_feedforward), nn.ReLU(), nn.Linear(dim_feedforward, dim_input)
     )
 
 
 class _Residual(nn.Module):
     r"""
     Residual Class.
 
@@ -162,17 +156,15 @@
         dim_q = dim_k = max(dim_model // num_heads, 1)
         self.attention = _Residual(
             MultiHeadAttention(num_heads, dim_model, dim_q, dim_k),
             dimension=dim_model,
             dropout=dropout,
         )
         self.feed_forward = _Residual(
-            _feed_forward(dim_model, dim_feedforward),
-            dimension=dim_model,
-            dropout=dropout,
+            _feed_forward(dim_model, dim_feedforward), dimension=dim_model, dropout=dropout
         )
 
     def forward(self, src: Tensor) -> Tensor:
         src = self.attention(src, src, src)
         return self.feed_forward(src)
 
 
@@ -191,15 +183,14 @@
         self,
         num_layers: int = 6,
         dim_model: int = 1,
         num_heads: int = 6,
         dim_feedforward: int = 2048,
         dropout: float = 0.1,
     ):
-
         super().__init__()
         self.layers = nn.ModuleList(
             [
                 _EncoderLayer(dim_model, num_heads, dim_feedforward, dropout)
                 for _ in range(num_layers)
             ]
         )
@@ -239,17 +230,15 @@
         )
         self.attention_2 = _Residual(
             MultiHeadAttention(num_heads, dim_model, dim_q, dim_k),
             dimension=dim_model,
             dropout=dropout,
         )
         self.feed_forward = _Residual(
-            _feed_forward(dim_model, dim_feedforward),
-            dimension=dim_model,
-            dropout=dropout,
+            _feed_forward(dim_model, dim_feedforward), dimension=dim_model, dropout=dropout
         )
 
     def forward(self, tgt: Tensor, memory: Tensor) -> Tensor:
         tgt = self.attention_1(tgt, tgt, tgt)
         tgt = self.attention_2(tgt, memory, memory)
         return self.feed_forward(tgt)
 
@@ -345,31 +334,30 @@
     def init_weights(m: nn.Module) -> None:
         r"""
         Initiate parameters in the transformer model.
         """
         if type(m) in (nn.Linear,):
             nn.init.xavier_uniform_(m.weight, gain=2**0.5)
 
-    def forward(self, batch: Tensor) -> Tuple[Tensor, Tensor]:
+    def forward(self, batch: Tensor) -> tuple[Tensor, Tensor]:
         batch = batch.view(-1, self.n_features, self.seq_len)
         encoded = self.encoder(batch)
         decoded = self.decoder(batch, encoded)
         return encoded, decoded
 
     def _get_reconstruction_loss(self, batch):
         _, recon = self.forward(batch)
         x = batch.view(-1, self.n_features, self.seq_len)
         return self.criterion(x, recon)
 
     def predict_step(self, batch: Tensor, batch_idx: int, dataloader_idx: int = 0):
         """Returns reconstruction for streaming input"""
         recon = self.reconstruction(batch)
         recon = recon.view(-1, self.seq_len, self.n_features)
-        recon_err = self.criterion(batch, recon, reduction="none")
-        return recon_err
+        return self.criterion(batch, recon, reduction="none")
 
 
 class SparseTransformerAE(TransformerAE):
     r"""
     Sparse Autoencoder for a transformer network.
     It inherits from VanillaAE class and serves as a wrapper around base network models.
     Sparse Autoencoder is a type of autoencoder that applies sparsity constraint.
```

### Comparing `numalogic-0.3.8/numalogic/models/autoencoder/variants/vanilla.py` & `numalogic-0.4.dev3/numalogic/models/autoencoder/variants/vanilla.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 
-from typing import Tuple, Sequence
+from collections.abc import Sequence
 
 import torch
 from torch import nn, Tensor
 
 from numalogic.models.autoencoder.base import BaseAE
 from numalogic.tools.exceptions import LayerSizeMismatchError
 
@@ -145,16 +145,15 @@
         seq_len: int,
         n_features: int = 1,
         encoder_layersizes: Sequence[int] = (16, 8),
         decoder_layersizes: Sequence[int] = (8, 16),
         dropout_p: float = 0.25,
         **kwargs,
     ):
-
-        super(VanillaAE, self).__init__(**kwargs)
+        super().__init__(**kwargs)
         self.seq_len = seq_len
         self.dropout_prob = dropout_p
         self.n_features = n_features
 
         self.save_hyperparameters()
 
         if encoder_layersizes[-1] != decoder_layersizes[0]:
@@ -183,31 +182,30 @@
     def init_weights(m: nn.Module) -> None:
         r"""
         Initiate parameters in the transformer model.
         """
         if type(m) == nn.Linear:
             nn.init.xavier_normal_(m.weight)
 
-    def forward(self, batch: Tensor) -> Tuple[Tensor, Tensor]:
+    def forward(self, batch: Tensor) -> tuple[Tensor, Tensor]:
         batch = batch.view(-1, self.n_features, self.seq_len)
         encoded = self.encoder(batch)
         decoded = self.decoder(encoded)
         return encoded, decoded
 
     def _get_reconstruction_loss(self, batch):
         _, recon = self.forward(batch)
         x = batch.view(-1, self.n_features, self.seq_len)
         return self.criterion(x, recon)
 
     def predict_step(self, batch: Tensor, batch_idx: int, dataloader_idx: int = 0):
         """Returns reconstruction for streaming input"""
         recon = self.reconstruction(batch)
         recon = recon.view(-1, self.seq_len, self.n_features)
-        recon_err = self.criterion(batch, recon, reduction="none")
-        return recon_err
+        return self.criterion(batch, recon, reduction="none")
 
 
 class SparseVanillaAE(VanillaAE):
     r"""
     Sparse Autoencoder for a fully connected network.
     It inherits from VanillaAE class and serves as a wrapper around base network models.
     Sparse Autoencoder is a type of autoencoder that applies sparsity constraint.
```

### Comparing `numalogic-0.3.8/numalogic/models/forecast/variants/naive.py` & `numalogic-0.4.dev3/numalogic/models/forecast/variants/naive.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-from typing import Dict, Tuple
-
 import numpy as np
 import pandas as pd
 from sklearn.metrics import r2_score
 from sklearn.pipeline import make_pipeline
 from sklearn.preprocessing import StandardScaler, FunctionTransformer
 
 from numalogic.postprocess import tanh_norm
@@ -25,25 +23,25 @@
 
     def normalize(self, df: pd.DataFrame) -> pd.DataFrame:
         return pd.DataFrame(self.pipeline.transform(df), index=df.index, columns=df.columns)
 
     def inverse_normalize(self, df: pd.DataFrame) -> pd.DataFrame:
         return pd.DataFrame(self.pipeline.inverse_transform(df), index=df.index, columns=df.columns)
 
-    def find_threshold(self, train_df: pd.DataFrame, k=3) -> Dict[str, Tuple[float, float]]:
+    def find_threshold(self, train_df: pd.DataFrame, k=3) -> dict[str, tuple[float, float]]:
         for col in train_df.columns:
             mean = train_df[col].mean()
             std = max(1e-2, train_df[col].std())
             thresh_upper = mean + (k * std)
             thresh_lower = mean - (k * std)
             self.thresholds[col] = (thresh_lower, thresh_upper)
             self.means[col] = mean
         return self.thresholds
 
-    def fit(self, train_df: pd.DataFrame) -> Dict[str, Tuple[float, float]]:
+    def fit(self, train_df: pd.DataFrame) -> dict[str, tuple[float, float]]:
         self.pipeline.fit(train_df)
         scaled_train_df = self.normalize(train_df)
         return self.find_threshold(scaled_train_df)
 
     def predict(self, test_df: pd.DataFrame) -> pd.DataFrame:
         _all_series = {}
         for feature in self.means:
```

### Comparing `numalogic-0.3.8/numalogic/models/threshold/_static.py` & `numalogic-0.4.dev3/numalogic/models/threshold/_static.py`

 * *Files 1% similar despite different names*

```diff
@@ -106,9 +106,8 @@
 
     def score_samples(self, x: npt.NDArray[float]) -> npt.NDArray[float]:
         """
         Returns an array of same shape as input
         with values being anomaly scores.
         """
         x = x.copy()
-        y = 10 / (1 + np.exp(-self.coeff * (x - self.upper_limit)))
-        return y
+        return 10 / (1 + np.exp(-self.coeff * (x - self.upper_limit)))
```

### Comparing `numalogic-0.3.8/numalogic/models/threshold/_std.py` & `numalogic-0.4.dev3/numalogic/models/threshold/_std.py`

 * *Files 5% similar despite different names*

```diff
@@ -71,9 +71,8 @@
         y_pred[x_test >= self._threshold] = 1
         return y_pred
 
     def score_samples(self, x_test: NDArray[float]) -> NDArray[float]:
         """
         Returns an anomaly score array with the same shape as input.
         """
-        y_scores = x_test / self.threshold
-        return y_scores
+        return x_test / self.threshold
```

### Comparing `numalogic-0.3.8/numalogic/postprocess.py` & `numalogic-0.4.dev3/numalogic/postprocess.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.3.8/numalogic/preprocess/__init__.py` & `numalogic-0.4.dev3/numalogic/preprocess/__init__.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.3.8/numalogic/preprocess/transformer.py` & `numalogic-0.4.dev3/numalogic/preprocess/transformer.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.3.8/numalogic/registry/mlflow_registry.py` & `numalogic-0.4.dev3/numalogic/registry/mlflow_registry.py`

 * *Files 6% similar despite different names*

```diff
@@ -8,28 +8,29 @@
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 
 import logging
 from enum import Enum
-from typing import Optional, Sequence, Dict, Any, Tuple
+from typing import Optional, Any
 
 import mlflow.pyfunc
 import mlflow.pytorch
 from mlflow.entities.model_registry import ModelVersion
 from mlflow.exceptions import RestException
 from mlflow.protos.databricks_pb2 import ErrorCode, RESOURCE_DOES_NOT_EXIST
 from mlflow.tracking import MlflowClient
 
 from numalogic.registry import ArtifactManager, ArtifactData
+from numalogic.registry.artifact import ArtifactCache
 from numalogic.tools.exceptions import ModelVersionError
-from numalogic.tools.types import Artifact
+from numalogic.tools.types import artifact_t, KEYS, META_T
 
-_LOGGER = logging.getLogger()
+_LOGGER = logging.getLogger(__name__)
 
 
 class ModelStage(str, Enum):
     """
     Defines different stages the model state can be in mlflow
     """
 
@@ -66,59 +67,47 @@
     >>> data = [[0, 0], [0, 0], [1, 1], [1, 1]]
     >>> scaler = StandardScaler.fit(data)
     >>> registry = MLflowRegistry(tracking_uri="http://0.0.0.0:8080", artifact_type="pytorch")
     >>> registry.save(skeys=["model"], dkeys=["AE"], artifact=VanillaAE(10))
     >>> artifact_data = registry.load(skeys=["model"], dkeys=["AE"])
     """
 
-    __slots__ = ("client", "handler", "models_to_retain", "model_stage")
+    __slots__ = ("client", "handler", "models_to_retain", "model_stage", "cache_registry")
     _TRACKING_URI = None
 
     def __new__(
         cls,
         tracking_uri: Optional[str],
         artifact_type: str = "pytorch",
         models_to_retain: int = 5,
         model_stage: ModelStage = ModelStage.PRODUCTION,
+        cache_registry: ArtifactCache = None,
         *args,
         **kwargs,
     ):
         instance = super().__new__(cls, *args, **kwargs)
         if (not cls._TRACKING_URI) or (cls._TRACKING_URI != tracking_uri):
             cls._TRACKING_URI = tracking_uri
         return instance
 
     def __init__(
         self,
         tracking_uri: str,
         artifact_type: str = "pytorch",
         models_to_retain: int = 5,
         model_stage: str = ModelStage.PRODUCTION,
+        cache_registry: ArtifactCache = None,
     ):
         super().__init__(tracking_uri)
         mlflow.set_tracking_uri(tracking_uri)
         self.client = MlflowClient()
         self.handler = self.mlflow_handler(artifact_type)
         self.models_to_retain = models_to_retain
         self.model_stage = model_stage
-
-    @staticmethod
-    def construct_key(skeys: Sequence[str], dkeys: Sequence[str]) -> str:
-        """
-        Returns a single key comprising static and dynamic key fields.
-        Args:
-            skeys: static key fields as list/tuple of strings
-            dkeys: dynamic key fields as list/tuple of strings
-
-        Returns:
-            key
-        """
-        _static_key = ":".join(skeys)
-        _dynamic_key = ":".join(dkeys)
-        return "::".join([_static_key, _dynamic_key])
+        self.cache_registry = cache_registry
 
     @staticmethod
     def mlflow_handler(artifact_type: str):
         """
         Helper method to return the right handler given the artifact type.
         """
         if artifact_type == "pytorch":
@@ -127,62 +116,78 @@
             return mlflow.sklearn
         if artifact_type == "tensorflow":
             return mlflow.tensorflow
         if artifact_type == "pyfunc":
             return mlflow.pyfunc
         raise NotImplementedError("Artifact Type not Implemented")
 
+    def _load_from_cache(self, key: str) -> Optional[ArtifactData]:
+        if not self.cache_registry:
+            return None
+        return self.cache_registry.load(key)
+
+    def _save_in_cache(self, key: str, artifact_data: ArtifactData) -> None:
+        if self.cache_registry:
+            self.cache_registry.save(key, artifact_data)
+
+    def _clear_cache(self, key: str) -> Optional[ArtifactData]:
+        if self.cache_registry:
+            return self.cache_registry.delete(key)
+        return None
+
     def load(
-        self,
-        skeys: Sequence[str],
-        dkeys: Sequence[str],
-        latest: bool = True,
-        version: str = None,
+        self, skeys: KEYS, dkeys: KEYS, latest: bool = True, version: str = None
     ) -> Optional[ArtifactData]:
         model_key = self.construct_key(skeys, dkeys)
-        try:
-            if (latest and version) or (not latest and not version):
-                raise ValueError("Either One of 'latest' or 'version' needed in load method call")
 
-            elif latest:
+        if (latest and version) or (not latest and not version):
+            raise ValueError("Either One of 'latest' or 'version' needed in load method call")
+
+        try:
+            if latest:
+                cached_artifact = self._load_from_cache(model_key)
+                if cached_artifact:
+                    return cached_artifact
                 version_info = self.client.get_latest_versions(model_key, stages=[self.model_stage])
                 if not version_info:
                     raise ModelVersionError("Model version missing for key = %s" % model_key)
                 version_info = version_info[-1]
             else:
                 version_info = self.client.get_model_version(model_key, version)
             model, metadata = self.__load_artifacts(skeys, dkeys, version_info)
-            return ArtifactData(artifact=model, metadata=metadata, extras=dict(version_info))
-
         except RestException as mlflow_err:
             if ErrorCode.Value(mlflow_err.error_code) == RESOURCE_DOES_NOT_EXIST:
                 _LOGGER.info("Model not found with key: %s", model_key)
             else:
                 _LOGGER.exception(
                     "Mlflow error when loading a model with key: %s: %r", model_key, mlflow_err
                 )
             return None
         except ModelVersionError as model_missing_err:
             _LOGGER.error(
-                "No Model found found in %s ERROR: %r",
-                self.model_stage,
-                model_missing_err,
+                "No Model found found in %s ERROR: %r", self.model_stage, model_missing_err
             )
             return None
         except Exception as ex:
             _LOGGER.exception("Unexpected error: %s", ex)
             return None
+        else:
+            artifact_data = ArtifactData(
+                artifact=model, metadata=metadata, extras=dict(version_info)
+            )
+            self._save_in_cache(model_key, artifact_data)
+            return artifact_data
 
     def save(
         self,
-        skeys: Sequence[str],
-        dkeys: Sequence[str],
-        artifact: Artifact,
+        skeys: KEYS,
+        dkeys: KEYS,
+        artifact: artifact_t,
         run_id: str = None,
-        **metadata: str,
+        **metadata: META_T,
     ) -> Optional[ModelVersion]:
         """
         Saves the artifact into mlflow registry and updates version.
         Args:
             skeys: static key fields as list/tuple of strings
             dkeys: dynamic key fields as list/tuple of strings
             artifact: primary artifact to be saved
@@ -195,23 +200,24 @@
         model_key = self.construct_key(skeys, dkeys)
         try:
             mlflow.start_run(run_id=run_id)
             self.handler.log_model(artifact, "model", registered_model_name=model_key)
             if metadata:
                 mlflow.log_params(metadata)
             model_version = self.transition_stage(skeys=skeys, dkeys=dkeys)
-            _LOGGER.info("Successfully inserted model %s to Mlflow", model_key)
-            return model_version
         except Exception as ex:
             _LOGGER.exception("Unhandled error when saving a model with key: %s: %r", model_key, ex)
             return None
+        else:
+            _LOGGER.info("Successfully inserted model %s to Mlflow", model_key)
+            return model_version
         finally:
             mlflow.end_run()
 
-    def delete(self, skeys: Sequence[str], dkeys: Sequence[str], version: str) -> None:
+    def delete(self, skeys: KEYS, dkeys: KEYS, version: str) -> None:
         """
         Deletes the artifact with a specified version from mlflow registry.
         Args:
             skeys: static key fields as list/tuple of strings
             dkeys: dynamic key fields as list/tuple of strings
             version: explicit artifact version
 
@@ -220,18 +226,18 @@
         """
         model_key = self.construct_key(skeys, dkeys)
         try:
             self.client.delete_model_version(name=model_key, version=version)
             _LOGGER.info("Successfully deleted model %s", model_key)
         except Exception as ex:
             _LOGGER.exception("Error when deleting a model with key: %s: %r", model_key, ex)
+        else:
+            self._clear_cache(model_key)
 
-    def transition_stage(
-        self, skeys: Sequence[str], dkeys: Sequence[str]
-    ) -> Optional[ModelVersion]:
+    def transition_stage(self, skeys: KEYS, dkeys: KEYS) -> Optional[ModelVersion]:
         """
         Changes stage information for the given model. Sets new model to "Production". The old
         production model is set to "Staging" and the rest model versions are set to "Archived".
 
         Args:
             skeys: static key fields as list/tuple of strings
             dkeys: dynamic key fields as list/tuple of strings
@@ -242,49 +248,47 @@
         try:
             current_staging = self.client.get_latest_versions(
                 name=model_name, stages=[self.model_stage]
             )
             latest = self.client.get_latest_versions(name=model_name, stages=["None"])
 
             latest_model_data = self.client.transition_model_version_stage(
-                name=model_name,
-                version=str(latest[-1].version),
-                stage=self.model_stage,
+                name=model_name, version=str(latest[-1].version), stage=self.model_stage
             )
 
             if current_staging:
                 self.client.transition_model_version_stage(
                     name=model_name,
                     version=str(current_staging[-1].version),
                     stage=ModelStage.ARCHIVE,
                 )
 
             # only keep "models_to_retain" number of models.
             self.__delete_stale_models(skeys=skeys, dkeys=dkeys)
-
-            _LOGGER.info("Successfully transitioned model to Production stage")
-            return latest_model_data
         except RestException as ex:
             _LOGGER.exception(
                 "Error when transitioning a model: %s to different stage: %r", model_name, ex
             )
             return None
+        else:
+            _LOGGER.info("Successfully transitioned model to Production stage")
+            return latest_model_data
 
-    def __delete_stale_models(self, skeys: Sequence[str], dkeys: Sequence[str]):
+    def __delete_stale_models(self, skeys: KEYS, dkeys: KEYS):
         model_name = self.construct_key(skeys, dkeys)
         list_model_versions = list(self.client.search_model_versions(f"name='{model_name}'"))
         if len(list_model_versions) > self.models_to_retain:
             models_to_delete = list_model_versions[self.models_to_retain :]
             for stale_model in models_to_delete:
                 self.delete(skeys=skeys, dkeys=dkeys, version=stale_model.version)
                 _LOGGER.debug("Deleted stale model version : %s", stale_model.version)
 
     def __load_artifacts(
-        self, skeys: Sequence[str], dkeys: Sequence[str], version_info: ModelVersion
-    ) -> Tuple[Artifact, Dict[str, Any]]:
+        self, skeys: KEYS, dkeys: KEYS, version_info: ModelVersion
+    ) -> tuple[artifact_t, dict[str, Any]]:
         model_key = self.construct_key(skeys, dkeys)
         model = self.handler.load_model(model_uri=f"models:/{model_key}/{version_info.version}")
         _LOGGER.info("Successfully loaded model %s from Mlflow", model_key)
 
         run_info = mlflow.get_run(version_info.run_id)
         metadata = run_info.data.params or {}
         _LOGGER.info(
```

### Comparing `numalogic-0.3.8/numalogic/synthetic/__init__.py` & `numalogic-0.4.dev3/numalogic/synthetic/__init__.py`

 * *Files identical despite different names*

### Comparing `numalogic-0.3.8/numalogic/synthetic/anomalies.py` & `numalogic-0.4.dev3/numalogic/synthetic/anomalies.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 
-from typing import Sequence, List
+from collections.abc import Sequence
 
 import numpy as np
 import pandas as pd
 from sklearn.preprocessing import StandardScaler
 
 
 class AnomalyGenerator:
@@ -24,14 +24,15 @@
         self,
         ref_df: pd.DataFrame,
         anomaly_type: str = "global",
         anomaly_ratio: float = 0.1,
         anomaly_sign: str = "positive",
         mu: float = 0.1,
         sigma: float = 0.01,
+        random_seed: int = 42,
     ):
         """
         Class to inject synthetic anomaly to the input time series based on parameters.
         Args:
             ref_df: Reference Multivariate time series DataFrame
             anomaly_type: Type of anomaly to impute.
                 Possible values include:
@@ -43,34 +44,34 @@
                 to number of samples
             anomaly_sign: Positive or Negative anomaly to be injected
                 Possible values include:
                     - "positive": higher outlier value injected compared to the current actual value
                     - "negative": lower outliers injected compared to the current actual value
             mu: Distributions mean of the Gaussian Noise injected
             sigma: Distributions std of the Gaussian Noise injected
+            random_seed: seed for random number generator
         """
 
         self.anomaly_type = anomaly_type
         self.anomaly_ratio = anomaly_ratio
         self.anomaly_sign = anomaly_sign
         self.freq = ref_df.index.freq
         self.mu, self.sigma = mu, sigma
 
         self.scaler = StandardScaler()
         scaled_ref_df = pd.DataFrame(
-            self.scaler.fit_transform(ref_df.to_numpy()),
-            index=ref_df.index,
-            columns=ref_df.columns,
+            self.scaler.fit_transform(ref_df.to_numpy()), index=ref_df.index, columns=ref_df.columns
         )
         self.ref_stats_df = scaled_ref_df.describe()
         self.__injected_cols = []
         self.block_size = None
+        self._rnd_gen = np.random.default_rng(random_seed)
 
     @property
-    def injected_cols(self) -> List[str]:
+    def injected_cols(self) -> list[str]:
         return self.__injected_cols
 
     def add_impact_sign(self) -> int:
         if self.anomaly_sign == "positive":
             return 1
         if self.anomaly_sign == "negative":
             return -1
@@ -106,15 +107,15 @@
             sample = tseries[: -self.block_size].sample(1)
             idx_start = sample.index
             idx_end = idx_start + (self.block_size * self.freq)
             outlier_block = tseries[idx_start.values[0] : idx_end.values[0]]
             factor = abs(self.ref_stats_df.loc["max", col] - outlier_block.mean())
 
             # Add gaussian noise to the data
-            noise = np.random.normal(self.mu, self.sigma, outlier_block.shape)
+            noise = self._rnd_gen.normal(self.mu, self.sigma, outlier_block.shape)
             outlier_block += noise + impact * factor * abs(outlier_block) * self.add_impact_sign()
 
             # Add labels to the data
             anomaly_col = anomaly_df["is_anomaly"]
             anomaly_block = anomaly_col[idx_start.values[0] : idx_end.values[0]]
             anomaly_block += self.add_impact_sign()
 
@@ -135,15 +136,15 @@
             tseries = target_df[col]
             sample = tseries[: -self.block_size].sample(1)
             idx_start = sample.index
             idx_end = idx_start + (self.block_size * self.freq)
             outlier_block = tseries[idx_start.values[0] : idx_end.values[0]]
 
             # Add gaussian noise to the data
-            noise = np.random.normal(self.mu, self.sigma, outlier_block.shape)
+            noise = self._rnd_gen.normal(self.mu, self.sigma, outlier_block.shape)
 
             dist_from_min = np.linalg.norm(
                 outlier_block.to_numpy() - self.ref_stats_df.loc["min", col]
             )
             dist_from_max = np.linalg.norm(
                 outlier_block.to_numpy() - self.ref_stats_df.loc["max", col]
             )
@@ -181,15 +182,15 @@
         idx_end = idx_start + (self.block_size * self.freq)
 
         for col in self.__injected_cols:
             tseries = target_df[col]
             outlier_block = tseries[idx_start.values[0] : idx_end.values[0]]
 
             # Add gaussian noise to the data
-            noise = np.random.normal(self.mu, self.sigma, outlier_block.shape)
+            noise = self._rnd_gen.normal(self.mu, self.sigma, outlier_block.shape)
 
             dist_from_min = np.linalg.norm(
                 outlier_block.to_numpy() - self.ref_stats_df.loc["min", col]
             )
             dist_from_max = np.linalg.norm(
                 outlier_block.to_numpy() - self.ref_stats_df.loc["max", col]
             )
@@ -224,31 +225,31 @@
         idx_start = sample.index
 
         for col in self.__injected_cols:
             tseries = target_df[col]
             idx_end = idx_start + (self.block_size * self.freq)
             outlier_block = tseries[idx_start.values[0] : idx_end.values[0]]
             # Add gaussian noise to the data
-            noise = np.random.normal(self.mu, self.sigma, outlier_block.shape)
+            noise = self._rnd_gen.normal(self.mu, self.sigma, outlier_block.shape)
 
-            if np.random.binomial(1, 0.5):
+            if self._rnd_gen.binomial(1, 0.5):
                 factor = abs(self.ref_stats_df.loc["min", col] - outlier_block.mean())
                 outlier_block -= (
                     noise + impact * factor * abs(outlier_block) * self.add_impact_sign()
                 )
             else:
                 factor = abs(outlier_block.mean() - self.ref_stats_df.loc["max", col])
                 outlier_block += (
                     noise + impact * factor * abs(outlier_block) * self.add_impact_sign()
                 )
 
             anomaly_col = anomaly_df["is_anomaly"]
             anomaly_block = anomaly_col[idx_start.values[0] : idx_end.values[0]]
             anomaly_block += self.add_impact_sign()
-            gap = np.random.randint(*gap_range)
+            gap = self._rnd_gen.integers(*gap_range)
             idx_start = idx_end + (gap * self.freq)
 
         return pd.DataFrame(
             self.scaler.inverse_transform(target_df.to_numpy()),
             index=target_df.index,
             columns=target_df.columns,
         ).merge(anomaly_df, left_index=True, right_index=True)
@@ -258,10 +259,10 @@
         target_df = pd.DataFrame(
             self.scaler.transform(target_df.to_numpy()),
             index=target_df.index,
             columns=target_df.columns,
         )
         self.block_size = np.ceil(target_df.shape[0] * self.anomaly_ratio).astype(int)
         if not cols:
-            cols = np.random.choice(target_df.columns, self.__MIN_COLUMNS[self.anomaly_type])
+            cols = self._rnd_gen.choice(target_df.columns, self.__MIN_COLUMNS[self.anomaly_type])
         self.__injected_cols = cols
         return target_df
```

### Comparing `numalogic-0.3.8/numalogic/synthetic/sparsity.py` & `numalogic-0.4.dev3/numalogic/synthetic/sparsity.py`

 * *Files 0% similar despite different names*

```diff
@@ -32,15 +32,14 @@
         shape = self._data.shape
 
         # based on sparsity ratio generating the rows
         # to which the data is going to be imputed with 0
         rows = random.sample(range(0, shape[0]), int(shape[0] * self.sparse_ratio))
 
         for row in rows:
-
             # identifying the columns to which the data is going to be imputed with 0.
             columns = random.sample(range(0, shape[1]), int(shape[1] * self.sparse_ratio))
             self._data.iloc[row, columns] = 0
 
     @property
     def data(self):
         return self._data
```

### Comparing `numalogic-0.3.8/numalogic/synthetic/timeseries.py` & `numalogic-0.4.dev3/numalogic/synthetic/timeseries.py`

 * *Files 10% similar despite different names*

```diff
@@ -6,16 +6,14 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 
-from typing import Tuple
-
 import numpy as np
 import pandas as pd
 from datetime import date
 
 from numpy.typing import NDArray
 
 
@@ -29,15 +27,16 @@
         secondary_period=10080,
         seasonal_ts_prob=0.7,
         baseline_range=(200.0, 350.0),
         slope_range=(-0.001, 0.01),
         amplitude_range=(10, 40),
         cosine_ratio_range=(0.5, 0.9),
         noise_range=(5, 15),
-        phase_shift_range: Tuple[int, int] = None,
+        phase_shift_range: tuple[int, int] = None,
+        random_seed: int = 42,
     ):
         self.seq_len = seq_len
         self.num_series = num_series
         self.dt_index = pd.DatetimeIndex(
             pd.date_range(end=date.today(), periods=seq_len, freq=freq)
         )
         self.time_steps = np.arange(seq_len, dtype="float32")
@@ -46,55 +45,53 @@
         self.amplitude_range = amplitude_range
         self.cos_ratio_range = cosine_ratio_range
         self.noise_range = noise_range
         self.phase_range = phase_shift_range
         self.primary_period = primary_period
         self.secondary_period = secondary_period
         self.seasonal_ts_prob = seasonal_ts_prob
+        self.seed = random_seed
+        self._rnd_gen = np.random.default_rng(random_seed)
 
     def gen_tseries(self) -> pd.DataFrame:
         all_series = {}
-        is_seasonal = np.random.binomial(1, self.seasonal_ts_prob, self.num_series)
+        is_seasonal = self._rnd_gen.binomial(1, self.seasonal_ts_prob, self.num_series)
 
         for s_idx in range(self.num_series):
             if is_seasonal[s_idx]:
                 seasonality = self.seasonality(self.primary_period)
                 if self.secondary_period:
                     seasonality += self.seasonality(self.secondary_period, amp_reduction_factor=3)
             else:
                 seasonality = np.zeros(self.seq_len)
             all_series[f"s{s_idx+1}"] = self.baseline() + self.trend() + self.noise() + seasonality
 
         return pd.DataFrame(all_series, index=self.dt_index)
 
     def baseline(self) -> float:
-        baseline = np.random.uniform(*self.baseline_range)
-        return baseline
+        return self._rnd_gen.uniform(*self.baseline_range)
 
     def trend(self) -> NDArray[float]:
-        slope = np.random.uniform(*self.slope_range)
+        slope = self._rnd_gen.uniform(*self.slope_range)
         return slope * self.time_steps
 
     def seasonality(self, period: int, amp_reduction_factor=1) -> NDArray[float]:
-        phase = np.random.uniform(*self.phase_range) if self.phase_range else 0
-        cosine_ratio = np.random.uniform(*self.cos_ratio_range)
-        amplitude = np.random.uniform(*self.amplitude_range) / amp_reduction_factor
+        phase = self._rnd_gen.uniform(*self.phase_range) if self.phase_range else 0
+        cosine_ratio = self._rnd_gen.uniform(*self.cos_ratio_range)
+        amplitude = self._rnd_gen.uniform(*self.amplitude_range) / amp_reduction_factor
 
         season_time = ((self.time_steps + phase) % period) / period
 
         seasonal_pattern = np.where(
-            season_time < cosine_ratio,
-            np.cos(season_time * 2 * np.pi),
-            season_time,
+            season_time < cosine_ratio, np.cos(season_time * 2 * np.pi), season_time
         )
         return amplitude * seasonal_pattern
 
-    def noise(self, seed=42) -> NDArray[float]:
-        rnd = np.random.RandomState(seed)
-        noise_level = np.random.uniform(*self.noise_range)
-        return rnd.randn(self.seq_len) * noise_level
+    def noise(self) -> NDArray[float]:
+        noise_level = self._rnd_gen.uniform(*self.noise_range)
+        return self._rnd_gen.standard_normal(self.seq_len) * noise_level
 
     @classmethod
     def train_test_split(
         cls, df: pd.DataFrame, test_size: int
-    ) -> Tuple[pd.DataFrame, pd.DataFrame]:
+    ) -> tuple[pd.DataFrame, pd.DataFrame]:
         return df[:-test_size], df[-test_size:]
```

### Comparing `numalogic-0.3.8/numalogic/tools/callbacks.py` & `numalogic-0.4.dev3/numalogic/tools/callbacks.py`

 * *Files 22% similar despite different names*

```diff
@@ -9,21 +9,20 @@
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 
 import logging
 
 import pytorch_lightning as pl
-from pytorch_lightning.callbacks import ProgressBarBase
-
+from pytorch_lightning.callbacks import ProgressBar
 
 _LOGGER = logging.getLogger(__name__)
 
 
-class ProgressDetails(ProgressBarBase):
+class ProgressDetails(ProgressBar):
     r"""
     A lightweight training progress detail producer.
 
     Args:
          log_freq: Interval of epochs to log
     """
 
@@ -36,16 +35,18 @@
         self._enable = True
 
     def disable(self):
         self._enable = False
 
     def on_train_epoch_end(self, trainer: pl.Trainer, pl_module: pl.LightningModule) -> None:
         super().on_train_epoch_end(trainer, pl_module)
-        metrics = self.get_metrics(trainer, pl_module)
+        loss = pl_module.total_train_loss / trainer.num_training_batches
         curr_epoch = trainer.current_epoch
         if curr_epoch % self._log_freq == 0:
-            _LOGGER.info("epoch=%s, training_loss=%s", curr_epoch, metrics["loss"])
+            _LOGGER.info("epoch=%s, training_loss=%.5f", curr_epoch, loss)
+        pl_module.reset_train_loss()
 
     def on_validation_epoch_end(self, trainer: pl.Trainer, pl_module: pl.LightningModule) -> None:
         super().on_validation_epoch_end(trainer, pl_module)
-        metrics = self.get_metrics(trainer, pl_module)
-        _LOGGER.info("validation_loss=%s", metrics["loss"])
+        loss = pl_module.total_val_loss / trainer.num_val_batches[0]
+        _LOGGER.info("validation_loss=%.5f", loss)
+        pl_module.reset_val_loss()
```

### Comparing `numalogic-0.3.8/numalogic/tools/data.py` & `numalogic-0.4.dev3/numalogic/tools/data.py`

 * *Files 12% similar despite different names*

```diff
@@ -6,15 +6,16 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 import logging
-from typing import Optional, Generator, Iterator
+from typing import Optional
+from collections.abc import Generator, Iterator
 
 import numpy as np
 import numpy.typing as npt
 import pytorch_lightning as pl
 import torch
 from pytorch_lightning.utilities.types import TRAIN_DATALOADERS, EVAL_DATALOADERS
 from torch import Tensor
@@ -49,14 +50,21 @@
             raise InvalidDataShapeError(
                 f"Input data should have dim=2, received shape: {data.shape}"
             )
 
         self._seq_len = seq_len
         self._data = data.astype(np.float32)
 
+    @property
+    def data(self) -> npt.NDArray[float]:
+        """
+        Returns the reference data in the input shape
+        """
+        return self._data
+
     def create_seq(self, input_: npt.NDArray[float]) -> Generator[npt.NDArray[float], None, None]:
         r"""
         A generator function that yields sequences of specified length from the input data.
         Yields a subarray from the input data of size (seq_len, num_features)
 
         Args:
             input_: A numpy array containing the input data.
@@ -97,58 +105,60 @@
 class TimeseriesDataModule(pl.LightningDataModule):
     r"""
     A time series data module for use in PyTorch Lightning,
     using a StreamingDataset for training and validation datasets.
 
     Args:
         seq_len: The length of the sequences to be generated from the input data.
-        train_data: A numpy array containing the training data in the shape of (batch, num_features)
-        val_data: A numpy array containing the validation data in the shape of (batch, num_features)
+        data: A numpy array containing the training data in the shape of (batch, num_features)
+        val_split_ratio: ratio of data to be used for validation set
         batch_size: The size of each batch of data. Defaults to 64.
     """
 
     def __init__(
         self,
         seq_len: int,
-        train_data: npt.NDArray[float],
-        val_data: npt.NDArray[float] = None,
+        data: npt.NDArray[float],
+        val_split_ratio: float = 0.1,
         batch_size: int = 64,
     ):
         super().__init__()
         self.batch_size = batch_size
         self.seq_len = seq_len
-        self.train_data = train_data
-        self.val_data = val_data
+        self.data = data
+
+        if val_split_ratio <= 0.0 or val_split_ratio >= 1.0:
+            raise ValueError("val_split_ratio can only accept values between 0.0 and 1.0")
+
+        self.val_split_ratio = val_split_ratio
 
         self.train_dataset = None
         self.val_dataset = None
 
     def setup(self, stage: str) -> None:
         r"""
         Sets up the data module by initializing the train and validation datasets.
         """
         if stage == "fit":
-            self.train_dataset = StreamingDataset(self.train_data, self.seq_len)
-            if self.val_data is None:
-                return
-            self.val_dataset = StreamingDataset(self.val_data, self.seq_len)
+            val_size = np.floor(self.val_split_ratio * len(self.data)).astype(int)
+            _LOGGER.info("Size of validation set: %s", val_size)
+
+            self.train_dataset = StreamingDataset(self.data[:-val_size, :], self.seq_len)
+            self.val_dataset = StreamingDataset(self.data[-val_size:, :], self.seq_len)
 
     def train_dataloader(self) -> TRAIN_DATALOADERS:
         r"""
         Creates and returns a DataLoader for the training dataset.
         """
         return DataLoader(self.train_dataset, batch_size=self.batch_size)
 
     def val_dataloader(self) -> Optional[EVAL_DATALOADERS]:
         r"""
         Creates and returns a DataLoader for the validation dataset if validation data is provided.
         """
-        if self.val_data is None:
-            _LOGGER.warning("Validation data not provided in TimeseriesDataModule.")
-            return None
         return DataLoader(self.val_dataset, batch_size=self.batch_size)
 
     @staticmethod
     def unbatch_sequences(batched: Tensor) -> Tensor:
         r"""
         Utility method to transform a 3D tensor of shape: (batch_size, seq_len, num_features)
         back into a shape of (new_batch, num_feautres).
```

### Comparing `numalogic-0.3.8/numalogic/tools/exceptions.py` & `numalogic-0.4.dev3/numalogic/tools/exceptions.py`

 * *Files 4% similar despite different names*

```diff
@@ -36,7 +36,15 @@
 
 class UnknownConfigArgsError(Exception):
     pass
 
 
 class ModelVersionError(Exception):
     pass
+
+
+class RedisRegistryError(Exception):
+    pass
+
+
+class ModelKeyNotFound(RedisRegistryError):
+    pass
```

### Comparing `numalogic-0.3.8/numalogic/tools/types.py` & `numalogic-0.4.dev3/numalogic/tools/types.py`

 * *Files 26% similar despite different names*

```diff
@@ -6,19 +6,31 @@
 # Unless required by applicable law or agreed to in writing, software
 # distributed under the License is distributed on an "AS IS" BASIS,
 # WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 # See the License for the specific language governing permissions and
 # limitations under the License.
 
 
-from typing import Union, Dict, NewType, TypeVar, Sequence, Optional
+from typing import Union, TypeVar
+from collections.abc import Sequence
 
-from sklearn.base import BaseEstimator, TransformerMixin
-from sklearn.pipeline import Pipeline
+from redis.client import AbstractRedis
+from sklearn.base import BaseEstimator
 from torch import nn
 
-Artifact = NewType("Artifact", Union[nn.Module, BaseEstimator, TransformerMixin, Pipeline])
-ArtifactDict = NewType(
-    "ArtifactDict",
-    Optional[Dict[str, Union[Sequence[Artifact], Dict[str, Artifact], Artifact, None]]],
-)
-AutoencoderModel = TypeVar("AutoencoderModel", bound="TorchAE")
+artifact_t = TypeVar("artifact_t", bound=Union[nn.Module, BaseEstimator])
+META_T = TypeVar("META_T", bound=dict[str, Union[str, list, dict]])
+EXTRA_T = TypeVar("EXTRA_T", bound=dict[str, Union[str, list, dict]])
+redis_client_t = TypeVar("redis_client_t", bound=AbstractRedis, covariant=True)
+KEYS = TypeVar("KEYS", bound=Sequence[str], covariant=True)
+
+
+class Singleton(type):
+    r"""
+    Helper metaclass to use as a Singleton class.
+    """
+    _instances = {}
+
+    def __call__(cls, *args, **kwargs):
+        if cls not in cls._instances:
+            cls._instances[cls] = super().__call__(*args, **kwargs)
+        return cls._instances[cls]
```

### Comparing `numalogic-0.3.8/pyproject.toml` & `numalogic-0.4.dev3/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -1,70 +1,72 @@
 [tool.poetry]
 name = "numalogic"
-version = "0.3.8"
+version = "0.4.dev3"
 description = "Collection of operational Machine Learning models and tools."
 authors = ["Numalogic Developers"]
 packages = [{ include = "numalogic" }]
 readme = "README.md"
 license = "Apache-2.0"
 maintainers = [
     "Avik Basu <avikbasu93@gmail.com>",
     "Vigith Maurice <vigith@gmail.com>",
 ]
 classifiers = [
     "Topic :: Software Development :: Libraries",
     "License :: OSI Approved :: Apache Software License",
     "Intended Audience :: Developers",
     "Topic :: Scientific/Engineering :: Artificial Intelligence",
-    "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10"
 ]
 repository = "https://github.com/numaproj/numalogic"
 documentation = "https://numalogic.numaproj.io/"
 homepage = "https://numalogic.numaproj.io/"
 
 [tool.poetry.dependencies]
-python = ">=3.8, <3.11"
+python = ">=3.9, <3.11"
 numpy = "^1.23"
-pandas = "^1.4"
+pandas = "^2.0"
 scikit-learn = "^1.0"
 mlflow-skinny = { version = ">2.0, <2.3", optional = true }
 protobuf = "~3.20" # needed to support pytorch-lightning
 omegaconf = "^2.3.0"
+cachetools = "^5.3.0"
+redis = {extras = ["hiredis"], version = "^4.5.4", optional = true}
 
 [tool.poetry.extras]
 mlflow = ["mlflow-skinny"]
+redis = ["redis"]
 
 [tool.poetry.group.torch]
 optional = true
 
 [tool.poetry.group.torch.dependencies]
-pytorch-lightning = "^1.8"
+pytorch-lightning = "^2.0"
 
 [tool.poetry.group.dev]
 optional = true
 
 [tool.poetry.group.dev.dependencies]
 matplotlib = "^3.4.2"
-black = "^22.6"
+black = "^23.0"
 pytest = "^7.1"
 pytest-cov = "^4.0"
-pylint = "^2.14.2"
-flake8 = "^5.0"
 torchinfo = "^1.7.2"
+ruff = "^0.0.264"
+pre-commit = "^3.3.1"
+fakeredis = "^2.11.2"
 
 [tool.poetry.group.jupyter]
 optional = true
 
 [tool.poetry.group.jupyter.dependencies]
 jupyter = "^1.0.0"
 ipykernel = "^6.15.1"
 nb-black = "^1.0.7"
-black = "^22.6.0"
 ipympl = "^0.9.1"
 ipython-autotime = "^0.3.1"
 
 [tool.black]
 line-length = 100
 include = '\.pyi?$'
 exclude = '''
@@ -81,10 +83,19 @@
   | build
   | dist
   | examples/.*/venv
   | tests/.*/setup.py
 )/
 '''
 
+[tool.ruff]
+line-length = 100
+src = ["numalogic", "tests"]
+select = ["E", "F", "W", "C901", "NPY", "RUF", "TRY", "G", "PLE", "PLW", "UP", "ICN", "RET", "Q"]
+ignore = ["TRY003", "TRY301"]
+target-version = "py39"
+show-fixes = true
+show-source = true
+
 [build-system]
 requires = ["poetry-core>=1.0.0"]
-build-backend = "poetry.core.masonry.api"
+build-backend = "poetry.core.masonry.api"
```

### Comparing `numalogic-0.3.8/PKG-INFO` & `numalogic-0.4.dev3/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,34 +1,35 @@
 Metadata-Version: 2.1
 Name: numalogic
-Version: 0.3.8
+Version: 0.4.dev3
 Summary: Collection of operational Machine Learning models and tools.
 Home-page: https://numalogic.numaproj.io/
 License: Apache-2.0
 Author: Numalogic Developers
 Maintainer: Avik Basu
 Maintainer-email: avikbasu93@gmail.com
-Requires-Python: >=3.8,<3.11
+Requires-Python: >=3.9,<3.11
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.10
-Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Topic :: Software Development :: Libraries
 Provides-Extra: mlflow
+Provides-Extra: redis
+Requires-Dist: cachetools (>=5.3.0,<6.0.0)
 Requires-Dist: mlflow-skinny (>2.0,<2.3) ; extra == "mlflow"
 Requires-Dist: numpy (>=1.23,<2.0)
 Requires-Dist: omegaconf (>=2.3.0,<3.0.0)
-Requires-Dist: pandas (>=1.4,<2.0)
+Requires-Dist: pandas (>=2.0,<3.0)
 Requires-Dist: protobuf (>=3.20,<3.21)
+Requires-Dist: redis[hiredis] (>=4.5.4,<5.0.0) ; extra == "redis"
 Requires-Dist: scikit-learn (>=1.0,<2.0)
 Project-URL: Documentation, https://numalogic.numaproj.io/
 Project-URL: Repository, https://github.com/numaproj/numalogic
 Description-Content-Type: text/markdown
 
 # numalogic
 
@@ -37,35 +38,35 @@
 [![black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/ambv/black)
 [![License](https://img.shields.io/badge/License-Apache%202.0-blue.svg)](LICENSE)
 [![slack](https://img.shields.io/badge/slack-numaproj-brightgreen.svg?logo=slack)](https://join.slack.com/t/numaproj/shared_invite/zt-19svuv47m-YKHhsQ~~KK9mBv1E7pNzfg)
 [![Release Version](https://img.shields.io/github/v/release/numaproj/numalogic?label=numalogic)](https://github.com/numaproj/numalogic/releases/latest)
 
 
 ## Background
-Numalogic is a collection of ML models and algorithms for operation data analytics and AIOps. 
-At Intuit, we use Numalogic at scale for continuous real-time data enrichment including 
-anomaly scoring. We assign an anomaly score (ML inference) to any time-series 
-datum/event/message we receive on our streaming platform (say, Kafka). 95% of our 
-data sets are time-series, and we have a complex flowchart to execute ML inference on 
-our high throughput sources. We run multiple models on the same datum, say a model that is 
-sensitive towards +ve sentiments, another more tuned towards -ve sentiments, and another 
-optimized for neutral sentiments. We also have a couple of ML models trained for the same 
-data source to provide more accurate scores based on the data density in our model store. 
-An ensemble of models is required because some composite keys in the data tend to be less 
-dense than others, e.g., forgot-password interaction is less frequent than a status check 
-interaction. At runtime, for each datum that arrives, models are picked based on a conditional 
-forwarding filter set on the data density. ML engineers need to worry about only their 
+Numalogic is a collection of ML models and algorithms for operation data analytics and AIOps.
+At Intuit, we use Numalogic at scale for continuous real-time data enrichment including
+anomaly scoring. We assign an anomaly score (ML inference) to any time-series
+datum/event/message we receive on our streaming platform (say, Kafka). 95% of our
+data sets are time-series, and we have a complex flowchart to execute ML inference on
+our high throughput sources. We run multiple models on the same datum, say a model that is
+sensitive towards +ve sentiments, another more tuned towards -ve sentiments, and another
+optimized for neutral sentiments. We also have a couple of ML models trained for the same
+data source to provide more accurate scores based on the data density in our model store.
+An ensemble of models is required because some composite keys in the data tend to be less
+dense than others, e.g., forgot-password interaction is less frequent than a status check
+interaction. At runtime, for each datum that arrives, models are picked based on a conditional
+forwarding filter set on the data density. ML engineers need to worry about only their
 inference container; they do not have to worry about data movement and quality assurance.
 
-## Numalogic realtime training 
-For an always-on ML platform, the key requirement is the ability to train or retrain models 
-automatically based on the incoming messages. The composite key built at per message runtime 
-looks for a matching model, and if the model turns out to be stale or missing, an automatic 
-retriggering is applied. The conditional forwarding feature of the platform improves the 
-development velocity of the ML developer when they have to make a decision whether to forward 
+## Numalogic realtime training
+For an always-on ML platform, the key requirement is the ability to train or retrain models
+automatically based on the incoming messages. The composite key built at per message runtime
+looks for a matching model, and if the model turns out to be stale or missing, an automatic
+retriggering is applied. The conditional forwarding feature of the platform improves the
+development velocity of the ML developer when they have to make a decision whether to forward
 the result further or drop it after a trigger request.
 
 
 ## Key Features
 
 1. Ease of use: simple and efficient tools for predictive data analytics
 2. Reusability: all the functionalities can be re-used in various contexts
@@ -87,25 +88,20 @@
 
 
 ## Installation
 
 Numalogic requires Python 3.8 or higher.
 
 ### Prerequisites
-Numalogic needs [PyTorch](https://pytorch.org/) and 
-[PyTorch Lightning](https://pytorch-lightning.readthedocs.io/en/stable/) to work. 
-But since these packages are platform dependendent, 
+Numalogic needs [PyTorch](https://pytorch.org/) and
+[PyTorch Lightning](https://pytorch-lightning.readthedocs.io/en/stable/) to work.
+But since these packages are platform dependendent,
 they are not included in the numalogic package itself. Kindly install them first.
 
-Numalogic supports the following pytorch versions:
-- 1.11.x
-- 1.12.x
-- 1.13.x
-
-Other versions do work, it is just that they are not tested.
+Numalogic supports pytorch versions `2.0.0` and above.
 
 numalogic can be installed using pip.
 ```shell
 pip install numalogic
 ```
 
 If using mlflow for model registry, install using:
@@ -131,15 +127,15 @@
     ```
     poetry install --all-extras
     ```
 4. To run unit tests:
     ```
     make test
     ```
-5. To format code style using black:
+5. To format code style using black and ruff:
     ```
     make lint
     ```
 
 ## Contributing
 We would love contributions in the numalogic project in one of the following (but not limited to) areas:
```

