# Comparing `tmp/mlcvzoo_tf_classification-6.0.0.tar.gz` & `tmp/mlcvzoo_tf_classification-6.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mlcvzoo_tf_classification-6.0.0.tar", max compression
+gzip compressed data, was "mlcvzoo_tf_classification-6.0.1.tar", max compression
```

## Comparing `mlcvzoo_tf_classification-6.0.0.tar` & `mlcvzoo_tf_classification-6.0.1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0      434 2023-02-14 09:35:53.978926 mlcvzoo_tf_classification-6.0.0/README.md
--rw-r--r--   0        0        0      177 2023-02-14 15:51:06.331380 mlcvzoo_tf_classification-6.0.0/mlcvzoo_tf_classification/__init__.py
--rw-r--r--   0        0        0     1890 2023-02-14 15:51:06.331380 mlcvzoo_tf_classification-6.0.0/mlcvzoo_tf_classification/annotation_utils.py
--rw-r--r--   0        0        0    12346 2023-02-14 15:51:06.331380 mlcvzoo_tf_classification-6.0.0/mlcvzoo_tf_classification/base_model.py
--rw-r--r--   0        0        0     9170 2023-02-14 15:51:06.331380 mlcvzoo_tf_classification-6.0.0/mlcvzoo_tf_classification/configuration.py
--rw-r--r--   0        0        0     3040 2023-02-14 09:35:53.978926 mlcvzoo_tf_classification-6.0.0/mlcvzoo_tf_classification/const.py
--rw-r--r--   0        0        0      263 2023-02-14 09:35:53.978926 mlcvzoo_tf_classification-6.0.0/mlcvzoo_tf_classification/custom_block/__init__.py
--rw-r--r--   0        0        0     1073 2023-02-14 15:51:06.331380 mlcvzoo_tf_classification-6.0.0/mlcvzoo_tf_classification/custom_block/configuration.py
--rw-r--r--   0        0        0     4484 2023-02-14 09:35:53.978926 mlcvzoo_tf_classification-6.0.0/mlcvzoo_tf_classification/custom_block/model.py
--rw-r--r--   0        0        0    11815 2023-02-14 15:51:06.331380 mlcvzoo_tf_classification-6.0.0/mlcvzoo_tf_classification/image_generator.py
--rw-r--r--   0        0        0      154 2023-02-14 09:35:53.978926 mlcvzoo_tf_classification-6.0.0/mlcvzoo_tf_classification/py.typed
--rw-r--r--   0        0        0      279 2023-02-14 09:35:53.978926 mlcvzoo_tf_classification-6.0.0/mlcvzoo_tf_classification/xception/__init__.py
--rw-r--r--   0        0        0     1111 2023-02-14 15:51:06.335380 mlcvzoo_tf_classification-6.0.0/mlcvzoo_tf_classification/xception/configuration.py
--rw-r--r--   0        0        0     3804 2023-02-14 09:35:53.978926 mlcvzoo_tf_classification-6.0.0/mlcvzoo_tf_classification/xception/model.py
--rw-r--r--   0        0        0     3986 2023-02-14 16:20:00.913560 mlcvzoo_tf_classification-6.0.0/pyproject.toml
--rw-r--r--   0        0        0     1645 1970-01-01 00:00:00.000000 mlcvzoo_tf_classification-6.0.0/setup.py
--rw-r--r--   0        0        0     2033 1970-01-01 00:00:00.000000 mlcvzoo_tf_classification-6.0.0/PKG-INFO
+-rw-r--r--   0        0        0      434 2023-05-02 10:18:08.297754 mlcvzoo_tf_classification-6.0.1/README.md
+-rw-r--r--   0        0        0      177 2023-05-05 09:21:26.582902 mlcvzoo_tf_classification-6.0.1/mlcvzoo_tf_classification/__init__.py
+-rw-r--r--   0        0        0     1890 2023-05-02 10:18:08.297754 mlcvzoo_tf_classification-6.0.1/mlcvzoo_tf_classification/annotation_utils.py
+-rw-r--r--   0        0        0    12346 2023-05-02 10:18:08.297754 mlcvzoo_tf_classification-6.0.1/mlcvzoo_tf_classification/base_model.py
+-rw-r--r--   0        0        0     9170 2023-05-02 10:18:08.297754 mlcvzoo_tf_classification-6.0.1/mlcvzoo_tf_classification/configuration.py
+-rw-r--r--   0        0        0     3040 2023-05-02 10:18:08.297754 mlcvzoo_tf_classification-6.0.1/mlcvzoo_tf_classification/const.py
+-rw-r--r--   0        0        0      263 2023-05-02 10:18:08.297754 mlcvzoo_tf_classification-6.0.1/mlcvzoo_tf_classification/custom_block/__init__.py
+-rw-r--r--   0        0        0     1073 2023-05-02 10:18:08.297754 mlcvzoo_tf_classification-6.0.1/mlcvzoo_tf_classification/custom_block/configuration.py
+-rw-r--r--   0        0        0     4484 2023-05-02 10:18:08.297754 mlcvzoo_tf_classification-6.0.1/mlcvzoo_tf_classification/custom_block/model.py
+-rw-r--r--   0        0        0    11815 2023-05-02 10:18:08.297754 mlcvzoo_tf_classification-6.0.1/mlcvzoo_tf_classification/image_generator.py
+-rw-r--r--   0        0        0      154 2023-05-02 10:18:08.297754 mlcvzoo_tf_classification-6.0.1/mlcvzoo_tf_classification/py.typed
+-rw-r--r--   0        0        0      279 2023-05-02 10:18:08.301755 mlcvzoo_tf_classification-6.0.1/mlcvzoo_tf_classification/xception/__init__.py
+-rw-r--r--   0        0        0     1111 2023-05-02 10:18:08.301755 mlcvzoo_tf_classification-6.0.1/mlcvzoo_tf_classification/xception/configuration.py
+-rw-r--r--   0        0        0     3804 2023-05-02 10:18:08.301755 mlcvzoo_tf_classification-6.0.1/mlcvzoo_tf_classification/xception/model.py
+-rw-r--r--   0        0        0     3870 2023-05-05 09:21:26.582902 mlcvzoo_tf_classification-6.0.1/pyproject.toml
+-rw-r--r--   0        0        0     1608 1970-01-01 00:00:00.000000 mlcvzoo_tf_classification-6.0.1/setup.py
+-rw-r--r--   0        0        0     1982 1970-01-01 00:00:00.000000 mlcvzoo_tf_classification-6.0.1/PKG-INFO
```

### Comparing `mlcvzoo_tf_classification-6.0.0/mlcvzoo_tf_classification/annotation_utils.py` & `mlcvzoo_tf_classification-6.0.1/mlcvzoo_tf_classification/annotation_utils.py`

 * *Files identical despite different names*

### Comparing `mlcvzoo_tf_classification-6.0.0/mlcvzoo_tf_classification/base_model.py` & `mlcvzoo_tf_classification-6.0.1/mlcvzoo_tf_classification/base_model.py`

 * *Files identical despite different names*

### Comparing `mlcvzoo_tf_classification-6.0.0/mlcvzoo_tf_classification/configuration.py` & `mlcvzoo_tf_classification-6.0.1/mlcvzoo_tf_classification/configuration.py`

 * *Files identical despite different names*

### Comparing `mlcvzoo_tf_classification-6.0.0/mlcvzoo_tf_classification/const.py` & `mlcvzoo_tf_classification-6.0.1/mlcvzoo_tf_classification/const.py`

 * *Files identical despite different names*

### Comparing `mlcvzoo_tf_classification-6.0.0/mlcvzoo_tf_classification/custom_block/configuration.py` & `mlcvzoo_tf_classification-6.0.1/mlcvzoo_tf_classification/custom_block/configuration.py`

 * *Files identical despite different names*

### Comparing `mlcvzoo_tf_classification-6.0.0/mlcvzoo_tf_classification/custom_block/model.py` & `mlcvzoo_tf_classification-6.0.1/mlcvzoo_tf_classification/custom_block/model.py`

 * *Files identical despite different names*

### Comparing `mlcvzoo_tf_classification-6.0.0/mlcvzoo_tf_classification/image_generator.py` & `mlcvzoo_tf_classification-6.0.1/mlcvzoo_tf_classification/image_generator.py`

 * *Files identical despite different names*

### Comparing `mlcvzoo_tf_classification-6.0.0/mlcvzoo_tf_classification/xception/configuration.py` & `mlcvzoo_tf_classification-6.0.1/mlcvzoo_tf_classification/xception/configuration.py`

 * *Files identical despite different names*

### Comparing `mlcvzoo_tf_classification-6.0.0/mlcvzoo_tf_classification/xception/model.py` & `mlcvzoo_tf_classification-6.0.1/mlcvzoo_tf_classification/xception/model.py`

 * *Files identical despite different names*

### Comparing `mlcvzoo_tf_classification-6.0.0/pyproject.toml` & `mlcvzoo_tf_classification-6.0.1/pyproject.toml`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "mlcvzoo_tf_classification"
-version = "6.0.0"
+version = "6.0.1"
 license = "Open Logistics License Version 1.0"
 description = "MLCVZoo TF Classifcation Package"
 readme = "README.md"
 homepage = "https://git.openlogisticsfoundation.org/silicon-economy/base/ml-toolbox/mlcvzoo"
 repository = "https://git.openlogisticsfoundation.org/silicon-economy/base/ml-toolbox/mlcvzoo"
 documentation = "https://git.openlogisticsfoundation.org/silicon-economy/base/ml-toolbox/mlcvzoo/-/blob/main/documentation/index.adoc"
 classifiers = [
@@ -37,31 +37,29 @@
 mlcvzoo_base = { version = "^5.0" }
 
 attrs = { version = ">=20" }
 opencv-python = { version = "^4.5,!=4.5.5.64,!=4.6.0.66" }
 opencv-contrib-python = { version = "^4.5,!=4.5.5.64,!=4.6.0.66,!=4.7.0.68" }
 # 1.19.2 is oldest available on aarch64 but 1.19.5 leads to unbuildable pytorch there, all is well on amd64
 numpy = { version = ">=1.19.2,!=1.19.5" }
-nptyping = { version = "^2.0" }
-tensorflow-cpu = { version="^2.6" }
-keras = { version="^2.6" }
-keras-preprocessing = { version="^1" }
-pandas = { version="<=1.3.3" }
-# TODO: remove when fixed by tensorboard: https://github.com/tensorflow/tensorboard/issues/5703
-protobuf =  {version="<=3.20"}
+nptyping = { version = ">=2.0" }
+tensorflow-cpu = { version=">=2.6" }
+keras = { version=">=2.6" }
+keras-preprocessing = { version=">=1" }
+pandas = { version=">=1.3.3" }
 
 [tool.poetry.dev-dependencies]
-mock = { version = "^4.0" }
-pytest = { version = "^7.0" }
-pytest-cov = { version = "^3.0.0" }
-black = { version = "^22" }
+mock = { version = ">=4.0" }
+pytest = { version = ">=7.0" }
+pytest-cov = { version = ">=3.0.0" }
+black = { version = ">=22" }
 mypy = { version = ">=0.961" }
-pylint = { version = "^2.9.6" }
-isort = { version = "^5.9" }
-pytest-mock = "^3.7"
+pylint = { version = ">=2.9.6" }
+isort = { version = ">=5.9" }
+pytest-mock = ">=3.7"
 
 [build-system]
 # NOTE: Don't remove setuptools, therefore require it from the build system
 requires = ["setuptools", "poetry_core>=1.0"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.isort]
```

### Comparing `mlcvzoo_tf_classification-6.0.0/setup.py` & `mlcvzoo_tf_classification-6.0.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -7,30 +7,29 @@
  'mlcvzoo_tf_classification.xception']
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
 ['attrs>=20',
- 'keras-preprocessing>=1,<2',
- 'keras>=2.6,<3.0',
+ 'keras-preprocessing>=1',
+ 'keras>=2.6',
  'mlcvzoo_base>=5.0,<6.0',
- 'nptyping>=2.0,<3.0',
+ 'nptyping>=2.0',
  'numpy>=1.19.2,!=1.19.5',
  'opencv-contrib-python>=4.5,<5.0,!=4.5.5.64,!=4.6.0.66,!=4.7.0.68',
  'opencv-python>=4.5,<5.0,!=4.5.5.64,!=4.6.0.66',
- 'pandas<=1.3.3',
- 'protobuf<=3.20',
+ 'pandas>=1.3.3',
  'related-mltoolbox>=1.0,<2.0',
- 'tensorflow-cpu>=2.6,<3.0',
+ 'tensorflow-cpu>=2.6',
  'yaml-config-builder>=8,<9']
 
 setup_kwargs = {
     'name': 'mlcvzoo-tf-classification',
-    'version': '6.0.0',
+    'version': '6.0.1',
     'description': 'MLCVZoo TF Classifcation Package',
     'long_description': '# MLCVZoo TF Classification\n\nThe MLCVZoo is an SDK for simplifying the usage of various (machine learning driven)\ncomputer vision algorithms. The package **mlcvzoo_tf_classification** is the wrapper module\nfor classification algorithms that are implemented using tensorflow.\n\nFurther information about the MLCVZoo can be found [here](../README.md).\n\n## Install\n`\npip install mlcvzoo-tf-classification\n`\n\n## Technology stack\n\n- Python\n',
     'author': 'Maximilian Otten',
     'author_email': 'maximilian.otten@iml.fraunhofer.de',
     'maintainer': 'None',
     'maintainer_email': 'None',
     'url': 'https://git.openlogisticsfoundation.org/silicon-economy/base/ml-toolbox/mlcvzoo',
```

### Comparing `mlcvzoo_tf_classification-6.0.0/PKG-INFO` & `mlcvzoo_tf_classification-6.0.1/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mlcvzoo-tf-classification
-Version: 6.0.0
+Version: 6.0.1
 Summary: MLCVZoo TF Classifcation Package
 Home-page: https://git.openlogisticsfoundation.org/silicon-economy/base/ml-toolbox/mlcvzoo
 License: Open Logistics License Version 1.0
 Author: Maximilian Otten
 Author-email: maximilian.otten@iml.fraunhofer.de
 Requires-Python: >=3.8,<3.11
 Classifier: Development Status :: 5 - Production/Stable
@@ -12,25 +12,24 @@
 Classifier: License :: Other/Proprietary License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Requires-Dist: attrs (>=20)
-Requires-Dist: keras (>=2.6,<3.0)
-Requires-Dist: keras-preprocessing (>=1,<2)
+Requires-Dist: keras (>=2.6)
+Requires-Dist: keras-preprocessing (>=1)
 Requires-Dist: mlcvzoo_base (>=5.0,<6.0)
-Requires-Dist: nptyping (>=2.0,<3.0)
+Requires-Dist: nptyping (>=2.0)
 Requires-Dist: numpy (>=1.19.2,!=1.19.5)
 Requires-Dist: opencv-contrib-python (>=4.5,<5.0,!=4.5.5.64,!=4.6.0.66,!=4.7.0.68)
 Requires-Dist: opencv-python (>=4.5,<5.0,!=4.5.5.64,!=4.6.0.66)
-Requires-Dist: pandas (<=1.3.3)
-Requires-Dist: protobuf (<=3.20)
+Requires-Dist: pandas (>=1.3.3)
 Requires-Dist: related-mltoolbox (>=1.0,<2.0)
-Requires-Dist: tensorflow-cpu (>=2.6,<3.0)
+Requires-Dist: tensorflow-cpu (>=2.6)
 Requires-Dist: yaml-config-builder (>=8,<9)
 Project-URL: Documentation, https://git.openlogisticsfoundation.org/silicon-economy/base/ml-toolbox/mlcvzoo/-/blob/main/documentation/index.adoc
 Project-URL: Repository, https://git.openlogisticsfoundation.org/silicon-economy/base/ml-toolbox/mlcvzoo
 Description-Content-Type: text/markdown
 
 # MLCVZoo TF Classification
```

