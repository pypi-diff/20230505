# Comparing `tmp/aiomodelz-0.4.8.tar.gz` & `tmp/aiomodelz-0.4.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aiomodelz-0.4.8.tar", last modified: Fri May  5 06:23:24 2023, max compression
+gzip compressed data, was "aiomodelz-0.4.9.tar", last modified: Fri May  5 07:24:24 2023, max compression
```

## Comparing `aiomodelz-0.4.8.tar` & `aiomodelz-0.4.9.tar`

### file list

```diff
@@ -1,13 +1,14 @@
--rw-r--r--   0        0        0    11105 2023-05-05 04:10:21.907425 aiomodelz-0.4.8/LICENSE
--rw-r--r--   0        0        0    11350 2023-05-02 16:04:13.511887 aiomodelz-0.4.8/LICENSE.modelz-py
--rw-r--r--   0        0        0     1277 2023-05-05 06:23:06.209699 aiomodelz-0.4.8/README.md
--rw-r--r--   0        0        0      146 2023-05-05 04:31:22.997827 aiomodelz-0.4.8/modelz/__init__.py
--rw-r--r--   0        0        0     4926 2023-05-05 05:55:32.213280 aiomodelz-0.4.8/modelz/aioclient.py
--rw-r--r--   0        0        0     1790 2023-05-05 04:24:36.559570 aiomodelz-0.4.8/modelz/args.py
--rw-r--r--   0        0        0     4690 2023-05-05 04:22:45.852756 aiomodelz-0.4.8/modelz/client.py
--rw-r--r--   0        0        0     2106 2023-05-02 16:04:13.514092 aiomodelz-0.4.8/modelz/cmd.py
--rw-r--r--   0        0        0      431 2023-05-02 16:04:13.514380 aiomodelz-0.4.8/modelz/env.py
--rw-r--r--   0        0        0     1284 2023-05-02 16:04:13.514716 aiomodelz-0.4.8/modelz/serde.py
--rw-r--r--   0        0        0     1333 2023-05-05 04:37:50.041199 aiomodelz-0.4.8/pyproject.toml
--rw-r--r--   0        0        0       34 2023-05-02 16:04:13.516523 aiomodelz-0.4.8/tests/dummy_test.py
--rw-r--r--   0        0        0     1756 1970-01-01 00:00:00.000000 aiomodelz-0.4.8/PKG-INFO
+-rw-r--r--   0        0        0    11105 2023-05-05 04:10:21.907425 aiomodelz-0.4.9/LICENSE
+-rw-r--r--   0        0        0    11350 2023-05-02 16:04:13.511887 aiomodelz-0.4.9/LICENSE.modelz-py
+-rw-r--r--   0        0        0     1664 2023-05-05 07:23:41.674893 aiomodelz-0.4.9/README.md
+-rw-r--r--   0        0        0      146 2023-05-05 04:31:22.997827 aiomodelz-0.4.9/modelz/__init__.py
+-rw-r--r--   0        0        0     5212 2023-05-05 06:42:26.364302 aiomodelz-0.4.9/modelz/aioclient.py
+-rw-r--r--   0        0        0     1790 2023-05-05 04:24:36.559570 aiomodelz-0.4.9/modelz/args.py
+-rw-r--r--   0        0        0     4690 2023-05-05 04:22:45.852756 aiomodelz-0.4.9/modelz/client.py
+-rw-r--r--   0        0        0     2106 2023-05-02 16:04:13.514092 aiomodelz-0.4.9/modelz/cmd.py
+-rw-r--r--   0        0        0      572 2023-05-05 06:38:19.733111 aiomodelz-0.4.9/modelz/env.py
+-rw-r--r--   0        0        0     1284 2023-05-02 16:04:13.514716 aiomodelz-0.4.9/modelz/serde.py
+-rw-r--r--   0        0        0      858 2023-05-05 06:36:57.723517 aiomodelz-0.4.9/modelz/utils.py
+-rw-r--r--   0        0        0     1333 2023-05-05 04:37:50.041199 aiomodelz-0.4.9/pyproject.toml
+-rw-r--r--   0        0        0       34 2023-05-02 16:04:13.516523 aiomodelz-0.4.9/tests/dummy_test.py
+-rw-r--r--   0        0        0     2143 1970-01-01 00:00:00.000000 aiomodelz-0.4.9/PKG-INFO
```

### Comparing `aiomodelz-0.4.8/LICENSE` & `aiomodelz-0.4.9/LICENSE`

 * *Files identical despite different names*

### Comparing `aiomodelz-0.4.8/LICENSE.modelz-py` & `aiomodelz-0.4.9/LICENSE.modelz-py`

 * *Files identical despite different names*

### Comparing `aiomodelz-0.4.8/README.md` & `aiomodelz-0.4.9/README.md`

 * *Files 17% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 # TensorChord Modelz Python SDK and CLI
 
 [modelz-py](https://github.com/tensorchord/modelz-py) with aiohttp
 
 Basically, [aioclient.py](modelz/aioclient.py) implements the async / aiohttp versions of `Modelz*` classes,  
-and [client.py](modelz/client.py) wraps around it with `asyncio.run()` calls.
+and [client.py](modelz/client.py) wraps around them with `asyncio.run()` calls.
 
 - [TensorChord Modelz Python SDK and CLI](#tensorchord-modelz-python-sdk-and-cli)
   - [Installation](#installation)
     - [pipx](#pipx)
     - [pip](#pip)
   - [CLI Usage](#cli-usage)
   - [Example Usage](#example-usage)
-    - [Stable Diffusion](#stable-diffusion)
+    - [CLI Inference](#cli-inference)
+    - [Python Interface](#python-interface)
   - [Develop](#develop)
 
 ## Installation
 
 ### pipx
 
 This is the recommended installation method if you only want to use the CLI.
@@ -44,20 +45,38 @@
   {inference,metrics,build}
 
 options:
   -h, --help            show this help message and exit
 ```
 
 ## Example Usage
-### Stable Diffusion
+### CLI Inference
 
 ```shell
 echo "cute cat" | modelz inference $PROJECT --serde msgpack --write-file cat.jpg --read-stdin
 ```
+### Python Interface
+
+```python
+# use dotenv to load env
+from dotenv import load_dotenv
+load_dotenv()
+
+# example .env:
+# MODELZ_API_KEY=mzi-*****
+# MODELZ_HOST=https://{}.cloud.modelz.dev/ # use this if you're using the dev modelz cluster
+# MODELZ_SSL_VERIFY=0 # disable ssl verification
+
+from modelz import AioModelzClient, ModelzClient
+...
+
+```
+
+
 
 ## Develop
 
 ```
 $ git clone https://github.com/tddschn/aiomodelz.git
 $ cd aiomodelz
 $ pdm install
-```
+```
```

### Comparing `aiomodelz-0.4.8/modelz/aioclient.py` & `aiomodelz-0.4.9/modelz/aioclient.py`

 * *Files 6% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 import aiohttp
 
 # from aiohttp import hdrs
 from rich.console import Console
 
 from .env import EnvConfig
 from .serde import Serde, SerdeEnum, TextSerde
+from modelz.utils import get_ssl_context_no_verify
 
 
 TIMEOUT = 300
 console = Console()
 DEFAULT_RESP_SERDE = TextSerde()
 DEFAULT_RETRY = 3
 
@@ -78,35 +79,38 @@
     ) -> None:
         # ...
         config = EnvConfig()
         self.host = host if host else config.host
         self.deployment = deployment
         self.auth = ModelzAuth(key)
         self.timeout = timeout
+        self.session_request_kwargs = {}
+        if not getattr(config, 'ssl_verify', True):
+            self.session_request_kwargs |= {'ssl': get_ssl_context_no_verify()}
 
     # async def _post(self, url, content, timeout):
     #     async with aiohttp.ClientSession() as session:
     #         async with session.post(url, data=content, headers=self.auth.auth_request, timeout=timeout) as response:
     #             return response
 
     # async def _get(self, url, timeout):
     #     async with aiohttp.ClientSession() as session:
     #         async with session.get(url, headers=self.auth.auth_request, timeout=timeout) as response:
     #             return response
 
     async def _post(self, url, content, timeout):
         headers = self.auth.get_headers()
         async with aiohttp.ClientSession() as session:
-            async with session.post(url, data=content, headers=headers, timeout=timeout) as response:
+            async with session.post(url, data=content, headers=headers, timeout=timeout, **self.session_request_kwargs) as response:
                 return response
 
     async def _get(self, url, timeout):
         headers = self.auth.get_headers()
         async with aiohttp.ClientSession() as session:
-            async with session.get(url, headers=headers, timeout=timeout) as response:
+            async with session.get(url, headers=headers, timeout=timeout, **self.session_request_kwargs) as response:
                 return response
 
     async def inference(
         self,
         params: Any,
         deployment: str | None = None,
         serde: str = "json",
```

### Comparing `aiomodelz-0.4.8/modelz/args.py` & `aiomodelz-0.4.9/modelz/args.py`

 * *Files identical despite different names*

### Comparing `aiomodelz-0.4.8/modelz/client.py` & `aiomodelz-0.4.9/modelz/client.py`

 * *Files identical despite different names*

### Comparing `aiomodelz-0.4.8/modelz/cmd.py` & `aiomodelz-0.4.9/modelz/cmd.py`

 * *Files identical despite different names*

### Comparing `aiomodelz-0.4.8/modelz/serde.py` & `aiomodelz-0.4.9/modelz/serde.py`

 * *Files identical despite different names*

### Comparing `aiomodelz-0.4.8/pyproject.toml` & `aiomodelz-0.4.9/pyproject.toml`

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
-version = "0.4.8"
+version = "0.4.9"
 
 [project.license]
 text = "Apache-2.0"
 
 [project.scripts]
 modelz = "modelz.cmd:main"
```

### Comparing `aiomodelz-0.4.8/PKG-INFO` & `aiomodelz-0.4.9/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aiomodelz
-Version: 0.4.8
+Version: 0.4.9
 Summary: machine learning models
 License: Apache-2.0
 Keywords: machine learning,deep learning
 Author-email: Teddy Xinyuan Chen <45612704+tddschn@users.noreply.github.com>,TensorChord <modelz-support@tensorchord.ai>
 Requires-Python: >=3.7
 Classifier: Environment :: GPU
 Classifier: Intended Audience :: Developers
@@ -12,23 +12,24 @@
 Description-Content-Type: text/markdown
 
 # TensorChord Modelz Python SDK and CLI
 
 [modelz-py](https://github.com/tensorchord/modelz-py) with aiohttp
 
 Basically, [aioclient.py](modelz/aioclient.py) implements the async / aiohttp versions of `Modelz*` classes,  
-and [client.py](modelz/client.py) wraps around it with `asyncio.run()` calls.
+and [client.py](modelz/client.py) wraps around them with `asyncio.run()` calls.
 
 - [TensorChord Modelz Python SDK and CLI](#tensorchord-modelz-python-sdk-and-cli)
   - [Installation](#installation)
     - [pipx](#pipx)
     - [pip](#pip)
   - [CLI Usage](#cli-usage)
   - [Example Usage](#example-usage)
-    - [Stable Diffusion](#stable-diffusion)
+    - [CLI Inference](#cli-inference)
+    - [Python Interface](#python-interface)
   - [Develop](#develop)
 
 ## Installation
 
 ### pipx
 
 This is the recommended installation method if you only want to use the CLI.
@@ -57,20 +58,39 @@
   {inference,metrics,build}
 
 options:
   -h, --help            show this help message and exit
 ```
 
 ## Example Usage
-### Stable Diffusion
+### CLI Inference
 
 ```shell
 echo "cute cat" | modelz inference $PROJECT --serde msgpack --write-file cat.jpg --read-stdin
 ```
+### Python Interface
+
+```python
+# use dotenv to load env
+from dotenv import load_dotenv
+load_dotenv()
+
+# example .env:
+# MODELZ_API_KEY=mzi-*****
+# MODELZ_HOST=https://{}.cloud.modelz.dev/ # use this if you're using the dev modelz cluster
+# MODELZ_SSL_VERIFY=0 # disable ssl verification
+
+from modelz import AioModelzClient, ModelzClient
+...
+
+```
+
+
 
 ## Develop
 
 ```
 $ git clone https://github.com/tddschn/aiomodelz.git
 $ cd aiomodelz
 $ pdm install
 ```
+
```

