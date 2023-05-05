# Comparing `tmp/aiomodelz-0.4.6.tar.gz` & `tmp/aiomodelz-0.4.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aiomodelz-0.4.6.tar", last modified: Fri May  5 06:14:15 2023, max compression
+gzip compressed data, was "aiomodelz-0.4.7.tar", last modified: Fri May  5 06:17:25 2023, max compression
```

## Comparing `aiomodelz-0.4.6.tar` & `aiomodelz-0.4.7.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0    11105 2023-05-05 04:10:21.907425 aiomodelz-0.4.6/LICENSE
--rw-r--r--   0        0        0    11350 2023-05-02 16:04:13.511887 aiomodelz-0.4.6/LICENSE.modelz-py
--rw-r--r--   0        0        0     1027 2023-05-05 06:13:42.964739 aiomodelz-0.4.6/README.md
--rw-r--r--   0        0        0      146 2023-05-05 04:31:22.997827 aiomodelz-0.4.6/modelz/__init__.py
--rw-r--r--   0        0        0     4926 2023-05-05 05:55:32.213280 aiomodelz-0.4.6/modelz/aioclient.py
--rw-r--r--   0        0        0     1790 2023-05-05 04:24:36.559570 aiomodelz-0.4.6/modelz/args.py
--rw-r--r--   0        0        0     4690 2023-05-05 04:22:45.852756 aiomodelz-0.4.6/modelz/client.py
--rw-r--r--   0        0        0     2106 2023-05-02 16:04:13.514092 aiomodelz-0.4.6/modelz/cmd.py
--rw-r--r--   0        0        0      431 2023-05-02 16:04:13.514380 aiomodelz-0.4.6/modelz/env.py
--rw-r--r--   0        0        0     1284 2023-05-02 16:04:13.514716 aiomodelz-0.4.6/modelz/serde.py
--rw-r--r--   0        0        0     1333 2023-05-05 04:37:50.041199 aiomodelz-0.4.6/pyproject.toml
--rw-r--r--   0        0        0       34 2023-05-02 16:04:13.516523 aiomodelz-0.4.6/tests/dummy_test.py
--rw-r--r--   0        0        0     1506 1970-01-01 00:00:00.000000 aiomodelz-0.4.6/PKG-INFO
+-rw-r--r--   0        0        0    11105 2023-05-05 04:10:21.907425 aiomodelz-0.4.7/LICENSE
+-rw-r--r--   0        0        0    11350 2023-05-02 16:04:13.511887 aiomodelz-0.4.7/LICENSE.modelz-py
+-rw-r--r--   0        0        0     1087 2023-05-05 06:16:21.726560 aiomodelz-0.4.7/README.md
+-rw-r--r--   0        0        0      146 2023-05-05 04:31:22.997827 aiomodelz-0.4.7/modelz/__init__.py
+-rw-r--r--   0        0        0     4926 2023-05-05 05:55:32.213280 aiomodelz-0.4.7/modelz/aioclient.py
+-rw-r--r--   0        0        0     1790 2023-05-05 04:24:36.559570 aiomodelz-0.4.7/modelz/args.py
+-rw-r--r--   0        0        0     4690 2023-05-05 04:22:45.852756 aiomodelz-0.4.7/modelz/client.py
+-rw-r--r--   0        0        0     2106 2023-05-02 16:04:13.514092 aiomodelz-0.4.7/modelz/cmd.py
+-rw-r--r--   0        0        0      431 2023-05-02 16:04:13.514380 aiomodelz-0.4.7/modelz/env.py
+-rw-r--r--   0        0        0     1284 2023-05-02 16:04:13.514716 aiomodelz-0.4.7/modelz/serde.py
+-rw-r--r--   0        0        0     1333 2023-05-05 04:37:50.041199 aiomodelz-0.4.7/pyproject.toml
+-rw-r--r--   0        0        0       34 2023-05-02 16:04:13.516523 aiomodelz-0.4.7/tests/dummy_test.py
+-rw-r--r--   0        0        0     1566 1970-01-01 00:00:00.000000 aiomodelz-0.4.7/PKG-INFO
```

### Comparing `aiomodelz-0.4.6/LICENSE` & `aiomodelz-0.4.7/LICENSE`

 * *Files identical despite different names*

### Comparing `aiomodelz-0.4.6/LICENSE.modelz-py` & `aiomodelz-0.4.7/LICENSE.modelz-py`

 * *Files identical despite different names*

### Comparing `aiomodelz-0.4.6/README.md` & `aiomodelz-0.4.7/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -1,12 +1,12 @@
-# Modelz Python SDK
+# TensorChord Modelz Python SDK and CLI
 
 [modelz-py](https://github.com/tensorchord/modelz-py) with aiohttp
 
-- [Modelz Python SDK](#modelz-python-sdk)
+- [TensorChord Modelz Python SDK and CLI](#tensorchord-modelz-python-sdk-and-cli)
   - [Installation](#installation)
     - [pipx](#pipx)
     - [pip](#pip)
   - [CLI Usage](#cli-usage)
   - [Example Usage](#example-usage)
     - [Stable Diffusion](#stable-diffusion)
   - [Develop](#develop)
```

### Comparing `aiomodelz-0.4.6/modelz/aioclient.py` & `aiomodelz-0.4.7/modelz/aioclient.py`

 * *Files identical despite different names*

### Comparing `aiomodelz-0.4.6/modelz/args.py` & `aiomodelz-0.4.7/modelz/args.py`

 * *Files identical despite different names*

### Comparing `aiomodelz-0.4.6/modelz/client.py` & `aiomodelz-0.4.7/modelz/client.py`

 * *Files identical despite different names*

### Comparing `aiomodelz-0.4.6/modelz/cmd.py` & `aiomodelz-0.4.7/modelz/cmd.py`

 * *Files identical despite different names*

### Comparing `aiomodelz-0.4.6/modelz/serde.py` & `aiomodelz-0.4.7/modelz/serde.py`

 * *Files identical despite different names*

### Comparing `aiomodelz-0.4.6/pyproject.toml` & `aiomodelz-0.4.7/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -19,15 +19,15 @@
     "msgpack>=1.0.4",
     "typer[all]>=0.7.0",
     "rich>=12.6.0",
     "aiohttp>=3.8.4",
 ]
 requires-python = ">=3.7"
 readme = "README.md"
-version = "0.4.6"
+version = "0.4.7"
 
 [project.license]
 text = "Apache-2.0"
 
 [project.scripts]
 modelz = "modelz.cmd:main"
```

### Comparing `aiomodelz-0.4.6/PKG-INFO` & `aiomodelz-0.4.7/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: aiomodelz
-Version: 0.4.6
+Version: 0.4.7
 Summary: machine learning models
 License: Apache-2.0
 Keywords: machine learning,deep learning
 Author-email: Teddy Xinyuan Chen <45612704+tddschn@users.noreply.github.com>,TensorChord <modelz-support@tensorchord.ai>
 Requires-Python: >=3.7
 Classifier: Environment :: GPU
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Description-Content-Type: text/markdown
 
-# Modelz Python SDK
+# TensorChord Modelz Python SDK and CLI
 
 [modelz-py](https://github.com/tensorchord/modelz-py) with aiohttp
 
-- [Modelz Python SDK](#modelz-python-sdk)
+- [TensorChord Modelz Python SDK and CLI](#tensorchord-modelz-python-sdk-and-cli)
   - [Installation](#installation)
     - [pipx](#pipx)
     - [pip](#pip)
   - [CLI Usage](#cli-usage)
   - [Example Usage](#example-usage)
     - [Stable Diffusion](#stable-diffusion)
   - [Develop](#develop)
```

