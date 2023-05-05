# Comparing `tmp/aiomodelz-0.4.1.tar.gz` & `tmp/aiomodelz-0.4.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aiomodelz-0.4.1.tar", last modified: Fri May  5 05:03:33 2023, max compression
+gzip compressed data, was "aiomodelz-0.4.2.tar", last modified: Fri May  5 05:05:16 2023, max compression
```

## Comparing `aiomodelz-0.4.1.tar` & `aiomodelz-0.4.2.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0    11105 2023-05-05 04:10:21.907425 aiomodelz-0.4.1/LICENSE
--rw-r--r--   0        0        0    11350 2023-05-02 16:04:13.511887 aiomodelz-0.4.1/LICENSE.modelz-py
--rw-r--r--   0        0        0      222 2023-05-02 16:04:13.512491 aiomodelz-0.4.1/README.md
--rw-r--r--   0        0        0      146 2023-05-05 04:31:22.997827 aiomodelz-0.4.1/modelz/__init__.py
--rw-r--r--   0        0        0     4261 2023-05-05 05:02:58.497756 aiomodelz-0.4.1/modelz/aioclient.py
--rw-r--r--   0        0        0     1790 2023-05-05 04:24:36.559570 aiomodelz-0.4.1/modelz/args.py
--rw-r--r--   0        0        0     4690 2023-05-05 04:22:45.852756 aiomodelz-0.4.1/modelz/client.py
--rw-r--r--   0        0        0     2106 2023-05-02 16:04:13.514092 aiomodelz-0.4.1/modelz/cmd.py
--rw-r--r--   0        0        0      431 2023-05-02 16:04:13.514380 aiomodelz-0.4.1/modelz/env.py
--rw-r--r--   0        0        0     1284 2023-05-02 16:04:13.514716 aiomodelz-0.4.1/modelz/serde.py
--rw-r--r--   0        0        0     1333 2023-05-05 04:37:50.041199 aiomodelz-0.4.1/pyproject.toml
--rw-r--r--   0        0        0       34 2023-05-02 16:04:13.516523 aiomodelz-0.4.1/tests/dummy_test.py
--rw-r--r--   0        0        0      701 1970-01-01 00:00:00.000000 aiomodelz-0.4.1/PKG-INFO
+-rw-r--r--   0        0        0    11105 2023-05-05 04:10:21.907425 aiomodelz-0.4.2/LICENSE
+-rw-r--r--   0        0        0    11350 2023-05-02 16:04:13.511887 aiomodelz-0.4.2/LICENSE.modelz-py
+-rw-r--r--   0        0        0      222 2023-05-02 16:04:13.512491 aiomodelz-0.4.2/README.md
+-rw-r--r--   0        0        0      146 2023-05-05 04:31:22.997827 aiomodelz-0.4.2/modelz/__init__.py
+-rw-r--r--   0        0        0     4290 2023-05-05 05:04:56.832178 aiomodelz-0.4.2/modelz/aioclient.py
+-rw-r--r--   0        0        0     1790 2023-05-05 04:24:36.559570 aiomodelz-0.4.2/modelz/args.py
+-rw-r--r--   0        0        0     4690 2023-05-05 04:22:45.852756 aiomodelz-0.4.2/modelz/client.py
+-rw-r--r--   0        0        0     2106 2023-05-02 16:04:13.514092 aiomodelz-0.4.2/modelz/cmd.py
+-rw-r--r--   0        0        0      431 2023-05-02 16:04:13.514380 aiomodelz-0.4.2/modelz/env.py
+-rw-r--r--   0        0        0     1284 2023-05-02 16:04:13.514716 aiomodelz-0.4.2/modelz/serde.py
+-rw-r--r--   0        0        0     1333 2023-05-05 04:37:50.041199 aiomodelz-0.4.2/pyproject.toml
+-rw-r--r--   0        0        0       34 2023-05-02 16:04:13.516523 aiomodelz-0.4.2/tests/dummy_test.py
+-rw-r--r--   0        0        0      701 1970-01-01 00:00:00.000000 aiomodelz-0.4.2/PKG-INFO
```

### Comparing `aiomodelz-0.4.1/LICENSE` & `aiomodelz-0.4.2/LICENSE`

 * *Files identical despite different names*

### Comparing `aiomodelz-0.4.1/LICENSE.modelz-py` & `aiomodelz-0.4.2/LICENSE.modelz-py`

 * *Files identical despite different names*

### Comparing `aiomodelz-0.4.1/modelz/aioclient.py` & `aiomodelz-0.4.2/modelz/aioclient.py`

 * *Files 2% similar despite different names*

```diff
@@ -70,14 +70,15 @@
         self,
         deployment: str | None = None,
         key: str | None = None,
         host: str | None = None,
         timeout: float = TIMEOUT,
     ) -> None:
         # ...
+        config = EnvConfig()
         self.host = host if host else config.host
         self.deployment = deployment
         self.auth = ModelzAuth(key)
         self.timeout = timeout
 
     async def _post(self, url, content, timeout):
         async with aiohttp.ClientSession() as session:
```

### Comparing `aiomodelz-0.4.1/modelz/args.py` & `aiomodelz-0.4.2/modelz/args.py`

 * *Files identical despite different names*

### Comparing `aiomodelz-0.4.1/modelz/client.py` & `aiomodelz-0.4.2/modelz/client.py`

 * *Files identical despite different names*

### Comparing `aiomodelz-0.4.1/modelz/cmd.py` & `aiomodelz-0.4.2/modelz/cmd.py`

 * *Files identical despite different names*

### Comparing `aiomodelz-0.4.1/modelz/serde.py` & `aiomodelz-0.4.2/modelz/serde.py`

 * *Files identical despite different names*

### Comparing `aiomodelz-0.4.1/pyproject.toml` & `aiomodelz-0.4.2/pyproject.toml`

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
-version = "0.4.1"
+version = "0.4.2"
 
 [project.license]
 text = "Apache-2.0"
 
 [project.scripts]
 modelz = "modelz.cmd:main"
```

### Comparing `aiomodelz-0.4.1/PKG-INFO` & `aiomodelz-0.4.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aiomodelz
-Version: 0.4.1
+Version: 0.4.2
 Summary: machine learning models
 License: Apache-2.0
 Keywords: machine learning,deep learning
 Author-email: Teddy Xinyuan Chen <45612704+tddschn@users.noreply.github.com>,TensorChord <modelz-support@tensorchord.ai>
 Requires-Python: >=3.7
 Classifier: Environment :: GPU
 Classifier: Intended Audience :: Developers
```

