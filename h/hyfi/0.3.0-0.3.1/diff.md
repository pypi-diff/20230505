# Comparing `tmp/hyfi-0.3.0.tar.gz` & `tmp/hyfi-0.3.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hyfi-0.3.0.tar", max compression
+gzip compressed data, was "hyfi-0.3.1.tar", max compression
```

## Comparing `hyfi-0.3.0.tar` & `hyfi-0.3.1.tar`

### file list

```diff
@@ -1,54 +1,69 @@
--rw-r--r--   0        0        0     1071 2023-05-05 00:43:33.833856 hyfi-0.3.0/LICENSE
--rw-r--r--   0        0        0     1949 2023-05-05 00:43:33.833856 hyfi-0.3.0/README.md
--rw-r--r--   0        0        0     4056 2023-05-05 00:44:07.426452 hyfi-0.3.0/pyproject.toml
--rw-r--r--   0        0        0     2680 2023-05-05 00:43:33.837856 hyfi-0.3.0/src/hyfi/__cli__.py
--rw-r--r--   0        0        0      331 2023-05-05 00:43:33.837856 hyfi-0.3.0/src/hyfi/__init__.py
--rw-r--r--   0        0        0       22 2023-05-05 00:44:07.370451 hyfi-0.3.0/src/hyfi/_version.py
--rw-r--r--   0        0        0        0 2023-05-05 00:43:33.837856 hyfi-0.3.0/src/hyfi/conf/__init__.py
--rw-r--r--   0        0        0      233 2023-05-05 00:44:07.370451 hyfi-0.3.0/src/hyfi/conf/about/__init__.yaml
--rw-r--r--   0        0        0      331 2023-05-05 00:43:33.837856 hyfi-0.3.0/src/hyfi/conf/batch/__init__.yaml
--rw-r--r--   0        0        0       83 2023-05-05 00:43:33.837856 hyfi-0.3.0/src/hyfi/conf/cmd/about.yaml
--rw-r--r--   0        0        0      167 2023-05-05 00:43:33.837856 hyfi-0.3.0/src/hyfi/conf/cmd/cpcfg.yaml
--rw-r--r--   0        0        0      320 2023-05-05 00:43:33.837856 hyfi-0.3.0/src/hyfi/conf/config.yaml
--rw-r--r--   0        0        0      496 2023-05-05 00:43:33.837856 hyfi-0.3.0/src/hyfi/conf/copier/conf.yaml
--rw-r--r--   0        0        0      789 2023-05-05 00:43:33.837856 hyfi-0.3.0/src/hyfi/conf/dotenv/__init__.yaml
--rw-r--r--   0        0        0      319 2023-05-05 00:43:33.837856 hyfi-0.3.0/src/hyfi/conf/hconf.yaml
--rw-r--r--   0        0        0     1128 2023-05-05 00:43:33.837856 hyfi-0.3.0/src/hyfi/conf/hydra/help/help.yaml
--rw-r--r--   0        0        0      264 2023-05-05 00:43:33.837856 hyfi-0.3.0/src/hyfi/conf/hydra/job_logging/custom.yaml
--rw-r--r--   0        0        0      293 2023-05-05 00:43:33.837856 hyfi-0.3.0/src/hyfi/conf/joblib/__init__.yaml
--rw-r--r--   0        0        0      701 2023-05-05 00:43:33.837856 hyfi-0.3.0/src/hyfi/conf/mode/__init__.yaml
--rw-r--r--   0        0        0      231 2023-05-05 00:43:33.837856 hyfi-0.3.0/src/hyfi/conf/mode/debug.yaml
--rw-r--r--   0        0        0      164 2023-05-05 00:43:33.837856 hyfi-0.3.0/src/hyfi/conf/path/__batch__.yaml
--rw-r--r--   0        0        0      582 2023-05-05 00:43:33.837856 hyfi-0.3.0/src/hyfi/conf/path/__default__.yaml
--rw-r--r--   0        0        0      616 2023-05-05 00:43:33.837856 hyfi-0.3.0/src/hyfi/conf/path/__init__.yaml
--rw-r--r--   0        0        0      360 2023-05-05 00:43:33.837856 hyfi-0.3.0/src/hyfi/conf/project/__init__.yaml
--rw-r--r--   0        0        0       21 2023-05-05 00:43:33.837856 hyfi-0.3.0/src/hyfi/config/__init__.py
--rw-r--r--   0        0        0    14151 2023-05-05 00:43:33.837856 hyfi-0.3.0/src/hyfi/config/batch.py
--rw-r--r--   0        0        0    19819 2023-05-05 00:43:33.837856 hyfi-0.3.0/src/hyfi/env.py
--rw-r--r--   0        0        0    12903 2023-05-05 00:43:33.837856 hyfi-0.3.0/src/hyfi/hydra.py
--rw-r--r--   0        0        0        0 2023-05-05 00:43:33.837856 hyfi-0.3.0/src/hyfi/image/__init__.py
--rw-r--r--   0        0        0     8474 2023-05-05 00:43:33.837856 hyfi-0.3.0/src/hyfi/image/collage.py
--rw-r--r--   0        0        0     4341 2023-05-05 00:43:33.837856 hyfi-0.3.0/src/hyfi/image/motion.py
--rw-r--r--   0        0        0     2556 2023-05-05 00:43:33.837856 hyfi-0.3.0/src/hyfi/image/plot.py
--rw-r--r--   0        0        0     3358 2023-05-05 00:43:33.837856 hyfi-0.3.0/src/hyfi/image/utils.py
--rw-r--r--   0        0        0        0 2023-05-05 00:43:33.837856 hyfi-0.3.0/src/hyfi/io/__init__.py
--rw-r--r--   0        0        0     5625 2023-05-05 00:43:33.837856 hyfi-0.3.0/src/hyfi/io/cached_path.py
--rw-r--r--   0        0        0    12802 2023-05-05 00:43:33.837856 hyfi-0.3.0/src/hyfi/io/file.py
--rw-r--r--   0        0        0    26828 2023-05-05 00:43:33.837856 hyfi-0.3.0/src/hyfi/main.py
--rw-r--r--   0        0        0        0 2023-05-05 00:43:33.837856 hyfi-0.3.0/src/hyfi/py.typed
--rw-r--r--   0        0        0        0 2023-05-05 00:43:33.837856 hyfi-0.3.0/src/hyfi/utils/__init__.py
--rw-r--r--   0        0        0      111 2023-05-05 00:43:33.837856 hyfi-0.3.0/src/hyfi/utils/batch/__init__.py
--rw-r--r--   0        0        0     2934 2023-05-05 00:43:33.837856 hyfi-0.3.0/src/hyfi/utils/batch/apply.py
--rw-r--r--   0        0        0     2046 2023-05-05 00:43:33.837856 hyfi-0.3.0/src/hyfi/utils/batch/apply_batch.py
--rw-r--r--   0        0        0    17469 2023-05-05 00:43:33.837856 hyfi-0.3.0/src/hyfi/utils/batch/batcher.py
--rw-r--r--   0        0        0     5651 2023-05-05 00:43:33.837856 hyfi-0.3.0/src/hyfi/utils/copier.py
--rw-r--r--   0        0        0     2281 2023-05-05 00:43:33.837856 hyfi-0.3.0/src/hyfi/utils/env.py
--rw-r--r--   0        0        0    10202 2023-05-05 00:43:33.837856 hyfi-0.3.0/src/hyfi/utils/func.py
--rw-r--r--   0        0        0     1046 2023-05-05 00:43:33.837856 hyfi-0.3.0/src/hyfi/utils/google.py
--rw-r--r--   0        0        0     3726 2023-05-05 00:43:33.837856 hyfi-0.3.0/src/hyfi/utils/gpu.py
--rw-r--r--   0        0        0     5234 2023-05-05 00:43:33.837856 hyfi-0.3.0/src/hyfi/utils/lib.py
--rw-r--r--   0        0        0     1074 2023-05-05 00:43:33.837856 hyfi-0.3.0/src/hyfi/utils/logging.py
--rw-r--r--   0        0        0    10003 2023-05-05 00:43:33.837856 hyfi-0.3.0/src/hyfi/utils/notebook.py
--rw-r--r--   0        0        0     2123 2023-05-05 00:43:33.837856 hyfi-0.3.0/src/hyfi/utils/pipe.py
--rw-r--r--   0        0        0     5504 2023-05-05 00:43:33.837856 hyfi-0.3.0/src/hyfi/utils/tools.py
--rw-r--r--   0        0        0     3391 1970-01-01 00:00:00.000000 hyfi-0.3.0/PKG-INFO
+-rw-r--r--   0        0        0     1071 2023-05-05 04:39:19.750368 hyfi-0.3.1/LICENSE
+-rw-r--r--   0        0        0     1632 2023-05-05 04:39:19.750368 hyfi-0.3.1/README.md
+-rw-r--r--   0        0        0     4206 2023-05-05 04:39:50.931568 hyfi-0.3.1/pyproject.toml
+-rw-r--r--   0        0        0     2680 2023-05-05 04:39:19.754368 hyfi-0.3.1/src/hyfi/__cli__.py
+-rw-r--r--   0        0        0      331 2023-05-05 04:39:19.754368 hyfi-0.3.1/src/hyfi/__init__.py
+-rw-r--r--   0        0        0       22 2023-05-05 04:39:50.863565 hyfi-0.3.1/src/hyfi/_version.py
+-rw-r--r--   0        0        0        0 2023-05-05 04:39:19.754368 hyfi-0.3.1/src/hyfi/conf/__init__.py
+-rw-r--r--   0        0        0      233 2023-05-05 04:39:50.863565 hyfi-0.3.1/src/hyfi/conf/about/__init__.yaml
+-rw-r--r--   0        0        0      331 2023-05-05 04:39:19.754368 hyfi-0.3.1/src/hyfi/conf/batch/__init__.yaml
+-rw-r--r--   0        0        0       83 2023-05-05 04:39:19.754368 hyfi-0.3.1/src/hyfi/conf/cmd/about.yaml
+-rw-r--r--   0        0        0      167 2023-05-05 04:39:19.754368 hyfi-0.3.1/src/hyfi/conf/cmd/cpcfg.yaml
+-rw-r--r--   0        0        0      320 2023-05-05 04:39:19.754368 hyfi-0.3.1/src/hyfi/conf/config.yaml
+-rw-r--r--   0        0        0      496 2023-05-05 04:39:19.754368 hyfi-0.3.1/src/hyfi/conf/copier/conf.yaml
+-rw-r--r--   0        0        0      789 2023-05-05 04:39:19.754368 hyfi-0.3.1/src/hyfi/conf/dotenv/__init__.yaml
+-rw-r--r--   0        0        0      319 2023-05-05 04:39:19.754368 hyfi-0.3.1/src/hyfi/conf/hconf.yaml
+-rw-r--r--   0        0        0     1128 2023-05-05 04:39:19.754368 hyfi-0.3.1/src/hyfi/conf/hydra/help/help.yaml
+-rw-r--r--   0        0        0      264 2023-05-05 04:39:19.754368 hyfi-0.3.1/src/hyfi/conf/hydra/job_logging/custom.yaml
+-rw-r--r--   0        0        0      293 2023-05-05 04:39:19.754368 hyfi-0.3.1/src/hyfi/conf/joblib/__init__.yaml
+-rw-r--r--   0        0        0      701 2023-05-05 04:39:19.754368 hyfi-0.3.1/src/hyfi/conf/mode/__init__.yaml
+-rw-r--r--   0        0        0      231 2023-05-05 04:39:19.754368 hyfi-0.3.1/src/hyfi/conf/mode/debug.yaml
+-rw-r--r--   0        0        0      164 2023-05-05 04:39:19.754368 hyfi-0.3.1/src/hyfi/conf/path/__batch__.yaml
+-rw-r--r--   0        0        0      582 2023-05-05 04:39:19.754368 hyfi-0.3.1/src/hyfi/conf/path/__default__.yaml
+-rw-r--r--   0        0        0      616 2023-05-05 04:39:19.754368 hyfi-0.3.1/src/hyfi/conf/path/__init__.yaml
+-rw-r--r--   0        0        0      360 2023-05-05 04:39:19.754368 hyfi-0.3.1/src/hyfi/conf/project/__init__.yaml
+-rw-r--r--   0        0        0       21 2023-05-05 04:39:19.754368 hyfi-0.3.1/src/hyfi/config/__init__.py
+-rw-r--r--   0        0        0    14151 2023-05-05 04:39:19.754368 hyfi-0.3.1/src/hyfi/config/batch.py
+-rw-r--r--   0        0        0    19819 2023-05-05 04:39:19.754368 hyfi-0.3.1/src/hyfi/env.py
+-rw-r--r--   0        0        0    12903 2023-05-05 04:39:19.754368 hyfi-0.3.1/src/hyfi/hydra.py
+-rw-r--r--   0        0        0        0 2023-05-05 04:39:19.754368 hyfi-0.3.1/src/hyfi/image/__init__.py
+-rw-r--r--   0        0        0     8474 2023-05-05 04:39:19.754368 hyfi-0.3.1/src/hyfi/image/collage.py
+-rw-r--r--   0        0        0     4341 2023-05-05 04:39:19.754368 hyfi-0.3.1/src/hyfi/image/motion.py
+-rw-r--r--   0        0        0     2556 2023-05-05 04:39:19.754368 hyfi-0.3.1/src/hyfi/image/plot.py
+-rw-r--r--   0        0        0     3358 2023-05-05 04:39:19.754368 hyfi-0.3.1/src/hyfi/image/utils.py
+-rw-r--r--   0        0        0        0 2023-05-05 04:39:19.754368 hyfi-0.3.1/src/hyfi/io/__init__.py
+-rw-r--r--   0        0        0     7152 2023-05-05 04:39:19.754368 hyfi-0.3.1/src/hyfi/io/cached_path.py
+-rw-r--r--   0        0        0    12802 2023-05-05 04:39:19.754368 hyfi-0.3.1/src/hyfi/io/file.py
+-rw-r--r--   0        0        0    26828 2023-05-05 04:39:19.754368 hyfi-0.3.1/src/hyfi/main.py
+-rw-r--r--   0        0        0        0 2023-05-05 04:39:19.754368 hyfi-0.3.1/src/hyfi/py.typed
+-rw-r--r--   0        0        0        0 2023-05-05 04:39:19.754368 hyfi-0.3.1/src/hyfi/utils/__init__.py
+-rw-r--r--   0        0        0      111 2023-05-05 04:39:19.754368 hyfi-0.3.1/src/hyfi/utils/batch/__init__.py
+-rw-r--r--   0        0        0     2934 2023-05-05 04:39:19.754368 hyfi-0.3.1/src/hyfi/utils/batch/apply.py
+-rw-r--r--   0        0        0     2046 2023-05-05 04:39:19.754368 hyfi-0.3.1/src/hyfi/utils/batch/apply_batch.py
+-rw-r--r--   0        0        0    17469 2023-05-05 04:39:19.758368 hyfi-0.3.1/src/hyfi/utils/batch/batcher.py
+-rw-r--r--   0        0        0     1206 2023-05-05 04:39:19.758368 hyfi-0.3.1/src/hyfi/utils/cached_path/__init__.py
+-rw-r--r--   0        0        0    14396 2023-05-05 04:39:19.758368 hyfi-0.3.1/src/hyfi/utils/cached_path/_cached_path.py
+-rw-r--r--   0        0        0     1619 2023-05-05 04:39:19.758368 hyfi-0.3.1/src/hyfi/utils/cached_path/cache_file.py
+-rw-r--r--   0        0        0     1110 2023-05-05 04:39:19.758368 hyfi-0.3.1/src/hyfi/utils/cached_path/common.py
+-rw-r--r--   0        0        0     1923 2023-05-05 04:39:19.758368 hyfi-0.3.1/src/hyfi/utils/cached_path/file_lock.py
+-rw-r--r--   0        0        0     3440 2023-05-05 04:39:19.758368 hyfi-0.3.1/src/hyfi/utils/cached_path/meta.py
+-rw-r--r--   0        0        0     3326 2023-05-05 04:39:19.758368 hyfi-0.3.1/src/hyfi/utils/cached_path/progress.py
+-rw-r--r--   0        0        0     1460 2023-05-05 04:39:19.758368 hyfi-0.3.1/src/hyfi/utils/cached_path/schemes/__init__.py
+-rw-r--r--   0        0        0     1815 2023-05-05 04:39:19.758368 hyfi-0.3.1/src/hyfi/utils/cached_path/schemes/beaker.py
+-rw-r--r--   0        0        0     2862 2023-05-05 04:39:19.758368 hyfi-0.3.1/src/hyfi/utils/cached_path/schemes/hf.py
+-rw-r--r--   0        0        0     2999 2023-05-05 04:39:19.758368 hyfi-0.3.1/src/hyfi/utils/cached_path/schemes/http.py
+-rw-r--r--   0        0        0     3645 2023-05-05 04:39:19.758368 hyfi-0.3.1/src/hyfi/utils/cached_path/schemes/scheme_client.py
+-rw-r--r--   0        0        0     1244 2023-05-05 04:39:19.758368 hyfi-0.3.1/src/hyfi/utils/cached_path/testing.py
+-rw-r--r--   0        0        0     4834 2023-05-05 04:39:19.758368 hyfi-0.3.1/src/hyfi/utils/cached_path/util.py
+-rw-r--r--   0        0        0      464 2023-05-05 04:39:19.758368 hyfi-0.3.1/src/hyfi/utils/cached_path/version.py
+-rw-r--r--   0        0        0     5651 2023-05-05 04:39:19.758368 hyfi-0.3.1/src/hyfi/utils/copier.py
+-rw-r--r--   0        0        0     2281 2023-05-05 04:39:19.758368 hyfi-0.3.1/src/hyfi/utils/env.py
+-rw-r--r--   0        0        0    10202 2023-05-05 04:39:19.758368 hyfi-0.3.1/src/hyfi/utils/func.py
+-rw-r--r--   0        0        0     1046 2023-05-05 04:39:19.758368 hyfi-0.3.1/src/hyfi/utils/google.py
+-rw-r--r--   0        0        0     3726 2023-05-05 04:39:19.758368 hyfi-0.3.1/src/hyfi/utils/gpu.py
+-rw-r--r--   0        0        0     5234 2023-05-05 04:39:19.758368 hyfi-0.3.1/src/hyfi/utils/lib.py
+-rw-r--r--   0        0        0     1074 2023-05-05 04:39:19.758368 hyfi-0.3.1/src/hyfi/utils/logging.py
+-rw-r--r--   0        0        0    10003 2023-05-05 04:39:19.758368 hyfi-0.3.1/src/hyfi/utils/notebook.py
+-rw-r--r--   0        0        0     2123 2023-05-05 04:39:19.758368 hyfi-0.3.1/src/hyfi/utils/pipe.py
+-rw-r--r--   0        0        0     5488 2023-05-05 04:39:19.758368 hyfi-0.3.1/src/hyfi/utils/tools.py
+-rw-r--r--   0        0        0     2948 1970-01-01 00:00:00.000000 hyfi-0.3.1/PKG-INFO
```

### Comparing `hyfi-0.3.0/LICENSE` & `hyfi-0.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `hyfi-0.3.0/pyproject.toml` & `hyfi-0.3.1/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "hyfi"
-version = "0.3.0"
+version = "0.3.1"
 description = "Hydra Fast Interface (Hydra and Pydantic based interface framework)"
 authors = ["Young Joon Lee <entelecheia@hotmail.com>"]
 license = "MIT"
 homepage = "https://hyfi.entelecheia.ai"
 repository = "https://github.com/entelecheia/hyfi"
 readme = "README.md"
 packages = [{ include = "hyfi", from = "src" }]
@@ -19,41 +19,54 @@
 pydantic = "^1.10.7"
 chardet = "<=5.1.0"
 pandas = "^1.5.3"
 scipy = "^1.10.1"
 matplotlib = "^3.7.1"
 numpy = "<1.24"
 python-dotenv = "^1.0.0"
-gdown = "^4.6.6"
 requests = "^2.27.1"
 tqdm = "^4.64.1"
-cached-path = "^1.3.3"
 colorama = "^0.4.3"
+pathspec = ">=0.9.0"
+filelock = ">=3.4,<3.10"
+rich = ">=12.1,<14.0"
+gdown = "<=4.6.6"
+huggingface-hub = ">=0.8.1,<0.13.0"
+# google-cloud-storage = ">=1.32.0,<3.0"
+# boto3 = ">=1.0,<2.0"
 
+[tool.poetry.group.ipython]
+optional = true
+
+[tool.poetry.group.ipython.dependencies]
 # A list of all of the optional dependencies, some of which are included in the
 # below `extras`. They can be opted into by apps.
-ipython = { version = "<=8.12.0", optional = true }
-ipython-autotime = { version = "^0.3.1", optional = true }
-rich = { version = ">=11.1", optional = true }
-pygments = { version = "<=2.15.1", optional = true }
+ipython = "<=8.12.0"
+ipython-autotime = "^0.3.1"
 
 [tool.poetry.extras]
-ipython = ["ipython", "ipython-autotime", "rich", "pygments"]
+ipython = ["ipython", "ipython-autotime"]
+
+[tool.poetry.group.dev]
+optional = true
 
 [tool.poetry.group.dev.dependencies]
 python-semantic-release = "^7.33.1"
 isort = "^5.12.0"
 black = "^23.1.0"
 flake8 = "^6.0.0"
 mypy = "^1.0.0"
 flake8-pyproject = "^1.2.2"
 pytest = "^7.2.1"
 pytest-cov = "^4.0.0"
 ipykernel = "^6.22.0"
 
+[tool.poe]
+include = [".tasks.toml", ".tasks-extra.toml"]
+
 [tool.black]
 exclude = [
     '_version.py',
     'node_modules',
     '_build',
     'docs',
     'tests',
```

### Comparing `hyfi-0.3.0/src/hyfi/__cli__.py` & `hyfi-0.3.1/src/hyfi/__cli__.py`

 * *Files identical despite different names*

### Comparing `hyfi-0.3.0/src/hyfi/conf/dotenv/__init__.yaml` & `hyfi-0.3.1/src/hyfi/conf/dotenv/__init__.yaml`

 * *Files identical despite different names*

### Comparing `hyfi-0.3.0/src/hyfi/conf/hydra/help/help.yaml` & `hyfi-0.3.1/src/hyfi/conf/hydra/help/help.yaml`

 * *Files identical despite different names*

### Comparing `hyfi-0.3.0/src/hyfi/conf/mode/__init__.yaml` & `hyfi-0.3.1/src/hyfi/conf/mode/__init__.yaml`

 * *Files identical despite different names*

### Comparing `hyfi-0.3.0/src/hyfi/conf/path/__default__.yaml` & `hyfi-0.3.1/src/hyfi/conf/path/__default__.yaml`

 * *Files identical despite different names*

### Comparing `hyfi-0.3.0/src/hyfi/conf/path/__init__.yaml` & `hyfi-0.3.1/src/hyfi/conf/path/__init__.yaml`

 * *Files identical despite different names*

### Comparing `hyfi-0.3.0/src/hyfi/config/batch.py` & `hyfi-0.3.1/src/hyfi/config/batch.py`

 * *Files identical despite different names*

### Comparing `hyfi-0.3.0/src/hyfi/env.py` & `hyfi-0.3.1/src/hyfi/env.py`

 * *Files identical despite different names*

### Comparing `hyfi-0.3.0/src/hyfi/hydra.py` & `hyfi-0.3.1/src/hyfi/hydra.py`

 * *Files identical despite different names*

### Comparing `hyfi-0.3.0/src/hyfi/image/collage.py` & `hyfi-0.3.1/src/hyfi/image/collage.py`

 * *Files identical despite different names*

### Comparing `hyfi-0.3.0/src/hyfi/image/motion.py` & `hyfi-0.3.1/src/hyfi/image/motion.py`

 * *Files identical despite different names*

### Comparing `hyfi-0.3.0/src/hyfi/image/plot.py` & `hyfi-0.3.1/src/hyfi/image/plot.py`

 * *Files identical despite different names*

### Comparing `hyfi-0.3.0/src/hyfi/image/utils.py` & `hyfi-0.3.1/src/hyfi/image/utils.py`

 * *Files identical despite different names*

### Comparing `hyfi-0.3.0/src/hyfi/io/cached_path.py` & `hyfi-0.3.1/src/hyfi/io/cached_path.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,26 +1,44 @@
 import os
 from pathlib import Path
 
-import cached_path as _cpath
 import gdown
 
+from ..utils.cached_path import _cached_path as _cpath
 from ..utils.logging import getLogger
 
 logger = getLogger(__name__)
 
 
 def cached_path(
     url_or_filename,
     extract_archive: bool = False,
     force_extract: bool = False,
     return_parent_dir: bool = False,
     cache_dir=None,
     verbose: bool = False,
 ):
+    """
+    Attempts to cache a file or URL and return the path to the cached file.
+    If required libraries 'cached_path' and 'gdown' are not installed, raises an ImportError.
+
+    Args:
+        url_or_filename (str): The URL or filename to be cached.
+        extract_archive (bool, optional): Whether to extract the file if it's an archive. Defaults to False.
+        force_extract (bool, optional): Whether to force extraction even if the destination already exists. Defaults to False.
+        return_parent_dir (bool, optional): If True, returns the parent directory of the cached file. Defaults to False.
+        cache_dir (str, optional): Directory to store cached files. Defaults to None.
+        verbose (bool, optional): Whether to print informative messages during the process. Defaults to False.
+
+    Raises:
+        ImportError: If the required libraries 'cached_path' and 'gdown' are not imported.
+
+    Returns:
+        str: Path to the cached file or its parent directory, depending on the 'return_parent_dir' parameter.
+    """
     if url_or_filename is None:
         return None
     if verbose:
         logger.info(
             "caching path: {}, extract_archive: {}, force_extract: {}, cache_dir: {}".format(
                 url_or_filename, extract_archive, force_extract, cache_dir
             )
@@ -32,14 +50,20 @@
                 url_or_filename,
                 verbose=verbose,
                 extract_archive=extract_archive,
                 force_extract=force_extract,
                 cache_dir=cache_dir,
             )
         else:
+            if _cpath is None or gdown is None:
+                raise ImportError(
+                    "Error importing required libraries 'cached-path'. "
+                    "Please install them using 'pip install cached-path' and try again."
+                )
+
             if cache_dir is None:
                 cache_dir = Path.home() / ".hyfi" / ".cache" / "cached_path"
             else:
                 cache_dir = Path(cache_dir) / "cached_path"
 
             _path = _cpath.cached_path(
                 url_or_filename,
@@ -76,14 +100,19 @@
           ex) gd://id:path
     :type verbose: bool
     :type extract_archive: bool
     :type force_extract: bool
     :type cache_dir: str
     :returns: str
     """
+    if gdown is None:
+        raise ImportError(
+            "Error importing required libraries 'gdown'. "
+            "Please install them using 'pip install gdown' and try again."
+        )
 
     if verbose:
         logger.info(f"Downloading {url}...")
     if cache_dir is None:
         cache_dir = Path.home() / ".hyfi" / ".cache" / "gdown"
     else:
         cache_dir = Path(cache_dir) / "gdown"
```

### Comparing `hyfi-0.3.0/src/hyfi/io/file.py` & `hyfi-0.3.1/src/hyfi/io/file.py`

 * *Files identical despite different names*

### Comparing `hyfi-0.3.0/src/hyfi/main.py` & `hyfi-0.3.1/src/hyfi/main.py`

 * *Ordering differences only*

 * *Files 0% similar despite different names*

```diff
@@ -32,15 +32,14 @@
     _to_dict,
     _to_yaml,
     _update,
     _viewsource,
 )
 from .io.cached_path import cached_path
 from .io.file import exists, is_dir, is_file, join_path, mkdir
-from .utils.pipe import _apply, _pipe
 from .utils.env import get_osenv, load_dotenv, set_osenv
 from .utils.func import (
     dict_product,
     dict_to_dataframe,
     records_to_dataframe,
     to_dateparm,
     to_datetime,
@@ -62,14 +61,15 @@
     display,
     display_image,
     get_display,
     hide_code_in_slideshow,
     is_colab,
     is_notebook,
 )
+from .utils.pipe import _apply, _pipe
 
 logger = getLogger(__name__)
 
 
 def _about(cfg):
     pkg_name = cfg.about.__package_name__
     name = cfg.about.name
```

### Comparing `hyfi-0.3.0/src/hyfi/utils/batch/apply.py` & `hyfi-0.3.1/src/hyfi/utils/batch/apply.py`

 * *Files identical despite different names*

### Comparing `hyfi-0.3.0/src/hyfi/utils/batch/apply_batch.py` & `hyfi-0.3.1/src/hyfi/utils/batch/apply_batch.py`

 * *Files identical despite different names*

### Comparing `hyfi-0.3.0/src/hyfi/utils/batch/batcher.py` & `hyfi-0.3.1/src/hyfi/utils/batch/batcher.py`

 * *Files identical despite different names*

### Comparing `hyfi-0.3.0/src/hyfi/utils/copier.py` & `hyfi-0.3.1/src/hyfi/utils/copier.py`

 * *Files identical despite different names*

### Comparing `hyfi-0.3.0/src/hyfi/utils/env.py` & `hyfi-0.3.1/src/hyfi/utils/env.py`

 * *Files identical despite different names*

### Comparing `hyfi-0.3.0/src/hyfi/utils/func.py` & `hyfi-0.3.1/src/hyfi/utils/func.py`

 * *Files identical despite different names*

### Comparing `hyfi-0.3.0/src/hyfi/utils/google.py` & `hyfi-0.3.1/src/hyfi/utils/google.py`

 * *Files identical despite different names*

### Comparing `hyfi-0.3.0/src/hyfi/utils/gpu.py` & `hyfi-0.3.1/src/hyfi/utils/gpu.py`

 * *Files identical despite different names*

### Comparing `hyfi-0.3.0/src/hyfi/utils/lib.py` & `hyfi-0.3.1/src/hyfi/utils/lib.py`

 * *Files identical despite different names*

### Comparing `hyfi-0.3.0/src/hyfi/utils/logging.py` & `hyfi-0.3.1/src/hyfi/utils/logging.py`

 * *Files identical despite different names*

### Comparing `hyfi-0.3.0/src/hyfi/utils/notebook.py` & `hyfi-0.3.1/src/hyfi/utils/notebook.py`

 * *Files identical despite different names*

### Comparing `hyfi-0.3.0/src/hyfi/utils/pipe.py` & `hyfi-0.3.1/src/hyfi/utils/pipe.py`

 * *Files identical despite different names*

### Comparing `hyfi-0.3.0/src/hyfi/utils/tools.py` & `hyfi-0.3.1/src/hyfi/utils/tools.py`

 * *Files 1% similar despite different names*

```diff
@@ -48,15 +48,15 @@
     if not verbose:
         return None  # HACK: Satisfy MyPy
     _msg = str(msg)
     action = action.rjust(indent, " ")
     if not style:
         return action + _msg
 
-    out = style + [action] + Style.RESET + [INDENT, _msg]  # type: ignore
+    out = style + [action] + Style.RESET + [INDENT, _msg]
     print(*out, sep="", file=file_)
     return None  # HACK: Satisfy MyPy
 
 
 def printf_exception(
     e: Exception, action: str, msg: str = "", indent: int = 0, quiet: bool = False
 ) -> None:
```

### Comparing `hyfi-0.3.0/PKG-INFO` & `hyfi-0.3.1/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,63 +1,58 @@
 Metadata-Version: 2.1
 Name: hyfi
-Version: 0.3.0
+Version: 0.3.1
 Summary: Hydra Fast Interface (Hydra and Pydantic based interface framework)
 Home-page: https://hyfi.entelecheia.ai
 License: MIT
 Author: Young Joon Lee
 Author-email: entelecheia@hotmail.com
 Requires-Python: >=3.8.1,<3.12
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Provides-Extra: ipython
-Requires-Dist: cached-path (>=1.3.3,<2.0.0)
 Requires-Dist: chardet (<=5.1.0)
 Requires-Dist: colorama (>=0.4.3,<0.5.0)
-Requires-Dist: gdown (>=4.6.6,<5.0.0)
+Requires-Dist: filelock (>=3.4,<3.10)
+Requires-Dist: gdown (<=4.6.6)
+Requires-Dist: huggingface-hub (>=0.8.1,<0.13.0)
 Requires-Dist: hydra-colorlog (>=1.2.0,<2.0.0)
 Requires-Dist: hydra-core (>=1.3.2,<2.0.0)
-Requires-Dist: ipython (<=8.12.0) ; extra == "ipython"
-Requires-Dist: ipython-autotime (>=0.3.1,<0.4.0) ; extra == "ipython"
 Requires-Dist: matplotlib (>=3.7.1,<4.0.0)
 Requires-Dist: numpy (<1.24)
 Requires-Dist: pandas (>=1.5.3,<2.0.0)
+Requires-Dist: pathspec (>=0.9.0)
 Requires-Dist: pydantic (>=1.10.7,<2.0.0)
-Requires-Dist: pygments (<=2.15.1) ; extra == "ipython"
 Requires-Dist: python-dotenv (>=1.0.0,<2.0.0)
 Requires-Dist: requests (>=2.27.1,<3.0.0)
-Requires-Dist: rich (>=11.1) ; extra == "ipython"
+Requires-Dist: rich (>=12.1,<14.0)
 Requires-Dist: scipy (>=1.10.1,<2.0.0)
 Requires-Dist: tqdm (>=4.64.1,<5.0.0)
 Project-URL: Repository, https://github.com/entelecheia/hyfi
 Description-Content-Type: text/markdown
 
 # HyFI: Hydra Fast Interface
 
 [![pypi-image]][pypi-url]
 [![version-image]][release-url]
 [![release-date-image]][release-url]
-[![jupyter-book-image]][jupyter book]
 [![license-image]][license-url]
 
+
 <!-- Links: -->
-[pypi-image]: https://badge.fury.io/py/hyfi.svg
-[pypi-url]: https://badge.fury.io/py/hyfi
+[pypi-image]: https://img.shields.io/pypi/v/hyfi
 [license-image]: https://img.shields.io/github/license/entelecheia/hyfi
 [license-url]: https://github.com/entelecheia/hyfi/blob/main/LICENSE
 [version-image]: https://img.shields.io/github/v/release/entelecheia/hyfi?sort=semver
 [release-date-image]: https://img.shields.io/github/release-date/entelecheia/hyfi
 [release-url]: https://github.com/entelecheia/hyfi/releases
-[conventional-commits-image]: https://img.shields.io/badge/Conventional%20Commits-1.0.0-%23FE5196?logo=conventionalcommits&logoColor=white
-[conventional commits]: https://conventionalcommits.org
 [jupyter-book-image]: https://jupyterbook.org/en/stable/_images/badge.svg
-[jupyter book]: https://hyfi.entelecheia.ai
 
 [repo-url]: https://github.com/entelecheia/hyfi
 [pypi-url]: https://pypi.org/project/hyfi
 [docs-url]: https://hyfi.entelecheia.ai
 [changelog]: https://github.com/entelecheia/hyfi/blob/main/CHANGELOG.md
 [contributing guidelines]: https://github.com/entelecheia/hyfi/blob/main/CONTRIBUTING.md
 <!-- Links: -->
```

