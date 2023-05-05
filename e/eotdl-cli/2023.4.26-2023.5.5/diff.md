# Comparing `tmp/eotdl_cli-2023.4.26.tar.gz` & `tmp/eotdl_cli-2023.5.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "eotdl_cli-2023.4.26.tar", max compression
+gzip compressed data, was "eotdl_cli-2023.5.5.tar", max compression
```

## Comparing `eotdl_cli-2023.4.26.tar` & `eotdl_cli-2023.5.5.tar`

### file list

```diff
@@ -1,26 +1,26 @@
--rw-r--r--   0        0        0       41 2023-03-08 12:48:38.254243 eotdl_cli-2023.4.26/README.md
--rw-r--r--   0        0        0        0 2023-03-08 12:48:38.254243 eotdl_cli-2023.4.26/eotdl_cli/__init__.py
--rw-r--r--   0        0        0        0 2023-03-14 08:10:21.438175 eotdl_cli-2023.4.26/eotdl_cli/commands/__init__.py
--rw-r--r--   0        0        0      920 2023-04-25 09:43:24.394687 eotdl_cli-2023.4.26/eotdl_cli/commands/auth.py
--rw-r--r--   0        0        0     1158 2023-04-26 14:28:57.085320 eotdl_cli-2023.4.26/eotdl_cli/commands/datasets.py
--rw-r--r--   0        0        0      479 2023-04-25 09:46:47.051348 eotdl_cli-2023.4.26/eotdl_cli/main.py
--rw-r--r--   0        0        0        0 2023-03-14 08:10:21.438175 eotdl_cli-2023.4.26/eotdl_cli/src/__init__.py
--rw-r--r--   0        0        0        0 2023-03-14 08:10:21.438175 eotdl_cli-2023.4.26/eotdl_cli/src/errors/__init__.py
--rw-r--r--   0        0        0      306 2023-03-14 08:10:21.438175 eotdl_cli-2023.4.26/eotdl_cli/src/errors/auth.py
--rw-r--r--   0        0        0     3499 2023-04-26 14:29:08.097360 eotdl_cli-2023.4.26/eotdl_cli/src/repos/APIRepo.py
--rw-r--r--   0        0        0      955 2023-04-11 08:30:40.653793 eotdl_cli-2023.4.26/eotdl_cli/src/repos/AuthRepo.py
--rw-r--r--   0        0        0       59 2023-03-14 08:10:21.442175 eotdl_cli-2023.4.26/eotdl_cli/src/repos/__init__.py
--rw-r--r--   0        0        0        0 2023-03-14 08:10:21.442175 eotdl_cli-2023.4.26/eotdl_cli/src/usecases/__init__.py
--rw-r--r--   0        0        0     1587 2023-04-11 08:30:40.653793 eotdl_cli-2023.4.26/eotdl_cli/src/usecases/auth/Auth.py
--rw-r--r--   0        0        0      332 2023-03-14 08:10:21.442175 eotdl_cli-2023.4.26/eotdl_cli/src/usecases/auth/IsLogged.py
--rw-r--r--   0        0        0      420 2023-03-14 08:10:21.442175 eotdl_cli-2023.4.26/eotdl_cli/src/usecases/auth/Logout.py
--rw-r--r--   0        0        0       54 2023-03-14 08:10:21.442175 eotdl_cli-2023.4.26/eotdl_cli/src/usecases/auth/__init__.py
--rw-r--r--   0        0        0      725 2023-03-14 15:04:32.741573 eotdl_cli-2023.4.26/eotdl_cli/src/usecases/auth/main.py
--rw-r--r--   0        0        0      458 2023-04-11 08:30:40.653793 eotdl_cli-2023.4.26/eotdl_cli/src/usecases/datasets/DownloadDataset.py
--rw-r--r--   0        0        0      973 2023-04-26 14:28:55.549314 eotdl_cli-2023.4.26/eotdl_cli/src/usecases/datasets/IngestDataset.py
--rw-r--r--   0        0        0      489 2023-04-11 08:30:40.657793 eotdl_cli-2023.4.26/eotdl_cli/src/usecases/datasets/RetrieveDataset.py
--rw-r--r--   0        0        0      427 2023-04-11 08:30:40.657793 eotdl_cli-2023.4.26/eotdl_cli/src/usecases/datasets/RetrieveDatasets.py
--rw-r--r--   0        0        0       69 2023-04-11 08:30:40.657793 eotdl_cli-2023.4.26/eotdl_cli/src/usecases/datasets/__init__.py
--rw-r--r--   0        0        0     1088 2023-04-26 14:28:52.429303 eotdl_cli-2023.4.26/eotdl_cli/src/usecases/datasets/main.py
--rw-r--r--   0        0        0      578 2023-04-26 14:29:25.381425 eotdl_cli-2023.4.26/pyproject.toml
--rw-r--r--   0        0        0      745 1970-01-01 00:00:00.000000 eotdl_cli-2023.4.26/PKG-INFO
+-rw-r--r--   0        0        0       41 2023-03-08 12:48:38.254243 eotdl_cli-2023.5.5/README.md
+-rw-r--r--   0        0        0        0 2023-03-08 12:48:38.254243 eotdl_cli-2023.5.5/eotdl_cli/__init__.py
+-rw-r--r--   0        0        0        0 2023-03-14 08:10:21.438175 eotdl_cli-2023.5.5/eotdl_cli/commands/__init__.py
+-rw-r--r--   0        0        0      920 2023-04-26 16:16:15.561454 eotdl_cli-2023.5.5/eotdl_cli/commands/auth.py
+-rw-r--r--   0        0        0     1158 2023-04-26 16:16:15.561454 eotdl_cli-2023.5.5/eotdl_cli/commands/datasets.py
+-rw-r--r--   0        0        0      479 2023-04-26 16:16:15.561454 eotdl_cli-2023.5.5/eotdl_cli/main.py
+-rw-r--r--   0        0        0        0 2023-03-14 08:10:21.438175 eotdl_cli-2023.5.5/eotdl_cli/src/__init__.py
+-rw-r--r--   0        0        0        0 2023-03-14 08:10:21.438175 eotdl_cli-2023.5.5/eotdl_cli/src/errors/__init__.py
+-rw-r--r--   0        0        0      306 2023-03-14 08:10:21.438175 eotdl_cli-2023.5.5/eotdl_cli/src/errors/auth.py
+-rw-r--r--   0        0        0     3471 2023-05-04 14:24:22.158984 eotdl_cli-2023.5.5/eotdl_cli/src/repos/APIRepo.py
+-rw-r--r--   0        0        0      955 2023-04-11 08:30:40.653793 eotdl_cli-2023.5.5/eotdl_cli/src/repos/AuthRepo.py
+-rw-r--r--   0        0        0       59 2023-03-14 08:10:21.442175 eotdl_cli-2023.5.5/eotdl_cli/src/repos/__init__.py
+-rw-r--r--   0        0        0        0 2023-03-14 08:10:21.442175 eotdl_cli-2023.5.5/eotdl_cli/src/usecases/__init__.py
+-rw-r--r--   0        0        0     1587 2023-04-11 08:30:40.653793 eotdl_cli-2023.5.5/eotdl_cli/src/usecases/auth/Auth.py
+-rw-r--r--   0        0        0      332 2023-03-14 08:10:21.442175 eotdl_cli-2023.5.5/eotdl_cli/src/usecases/auth/IsLogged.py
+-rw-r--r--   0        0        0      420 2023-03-14 08:10:21.442175 eotdl_cli-2023.5.5/eotdl_cli/src/usecases/auth/Logout.py
+-rw-r--r--   0        0        0       54 2023-03-14 08:10:21.442175 eotdl_cli-2023.5.5/eotdl_cli/src/usecases/auth/__init__.py
+-rw-r--r--   0        0        0      725 2023-03-14 15:04:32.741573 eotdl_cli-2023.5.5/eotdl_cli/src/usecases/auth/main.py
+-rw-r--r--   0        0        0      458 2023-04-11 08:30:40.653793 eotdl_cli-2023.5.5/eotdl_cli/src/usecases/datasets/DownloadDataset.py
+-rw-r--r--   0        0        0      973 2023-04-26 16:16:15.561454 eotdl_cli-2023.5.5/eotdl_cli/src/usecases/datasets/IngestDataset.py
+-rw-r--r--   0        0        0      489 2023-04-11 08:30:40.657793 eotdl_cli-2023.5.5/eotdl_cli/src/usecases/datasets/RetrieveDataset.py
+-rw-r--r--   0        0        0      427 2023-04-11 08:30:40.657793 eotdl_cli-2023.5.5/eotdl_cli/src/usecases/datasets/RetrieveDatasets.py
+-rw-r--r--   0        0        0       69 2023-04-11 08:30:40.657793 eotdl_cli-2023.5.5/eotdl_cli/src/usecases/datasets/__init__.py
+-rw-r--r--   0        0        0     1088 2023-04-26 16:16:15.561454 eotdl_cli-2023.5.5/eotdl_cli/src/usecases/datasets/main.py
+-rw-r--r--   0        0        0      602 2023-05-05 07:50:42.076183 eotdl_cli-2023.5.5/pyproject.toml
+-rw-r--r--   0        0        0      744 1970-01-01 00:00:00.000000 eotdl_cli-2023.5.5/PKG-INFO
```

### Comparing `eotdl_cli-2023.4.26/eotdl_cli/commands/auth.py` & `eotdl_cli-2023.5.5/eotdl_cli/commands/auth.py`

 * *Files identical despite different names*

### Comparing `eotdl_cli-2023.4.26/eotdl_cli/commands/datasets.py` & `eotdl_cli-2023.5.5/eotdl_cli/commands/datasets.py`

 * *Files identical despite different names*

### Comparing `eotdl_cli-2023.4.26/eotdl_cli/src/repos/APIRepo.py` & `eotdl_cli-2023.5.5/eotdl_cli/src/repos/APIRepo.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,14 @@
 import requests
 from tqdm import tqdm
 from pathlib import Path
 import os 
 
 class APIRepo():
-    # def __init__(self, url='http://localhost:8000/'):
-    def __init__(self, url='https://api.eotdl.com/'):
+    def __init__(self, url=os.getenv('EOTDL_API_URL', 'https://api.eotdl.com/')):
         self.url = url
 
     def login(self):
         return requests.get(self.url + 'auth/login')
     
     def token(self, code):
         return requests.get(self.url + 'auth/token?code=' + code)
```

### Comparing `eotdl_cli-2023.4.26/eotdl_cli/src/repos/AuthRepo.py` & `eotdl_cli-2023.5.5/eotdl_cli/src/repos/AuthRepo.py`

 * *Files identical despite different names*

### Comparing `eotdl_cli-2023.4.26/eotdl_cli/src/usecases/auth/Auth.py` & `eotdl_cli-2023.5.5/eotdl_cli/src/usecases/auth/Auth.py`

 * *Files identical despite different names*

### Comparing `eotdl_cli-2023.4.26/eotdl_cli/src/usecases/auth/main.py` & `eotdl_cli-2023.5.5/eotdl_cli/src/usecases/auth/main.py`

 * *Files identical despite different names*

### Comparing `eotdl_cli-2023.4.26/eotdl_cli/src/usecases/datasets/IngestDataset.py` & `eotdl_cli-2023.5.5/eotdl_cli/src/usecases/datasets/IngestDataset.py`

 * *Files identical despite different names*

### Comparing `eotdl_cli-2023.4.26/eotdl_cli/src/usecases/datasets/main.py` & `eotdl_cli-2023.5.5/eotdl_cli/src/usecases/datasets/main.py`

 * *Files identical despite different names*

### Comparing `eotdl_cli-2023.4.26/pyproject.toml` & `eotdl_cli-2023.5.5/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "eotdl-cli"
-version = "2023.04.26"
+version = "2023.05.05"
 description = ""
 authors = ["EarthPulse <it@earthpulse.es>"]
 license = "MIT"
 readme = "README.md"
 packages = [{include = "eotdl_cli"}]
 
 [tool.poetry.scripts]
@@ -18,11 +18,12 @@
 tqdm = "^4.65.0"
 pyjwt = "^2.6.0"
 
 
 [tool.poetry.group.dev.dependencies]
 pytest = "^7.2.2"
 pytest-cov = "^4.0.0"
+pytest-watch = "^4.2.0"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `eotdl_cli-2023.4.26/PKG-INFO` & `eotdl_cli-2023.5.5/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: eotdl-cli
-Version: 2023.4.26
+Version: 2023.5.5
 Summary: 
 License: MIT
 Author: EarthPulse
 Author-email: it@earthpulse.es
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

