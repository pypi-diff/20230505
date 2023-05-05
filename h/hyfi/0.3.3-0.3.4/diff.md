# Comparing `tmp/hyfi-0.3.3.tar.gz` & `tmp/hyfi-0.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hyfi-0.3.3.tar", max compression
+gzip compressed data, was "hyfi-0.3.4.tar", max compression
```

## Comparing `hyfi-0.3.3.tar` & `hyfi-0.3.4.tar`

### file list

```diff
@@ -1,69 +1,70 @@
--rw-r--r--   0        0        0     1071 2023-05-05 06:46:37.099479 hyfi-0.3.3/LICENSE
--rw-r--r--   0        0        0     1632 2023-05-05 06:46:37.099479 hyfi-0.3.3/README.md
--rw-r--r--   0        0        0     4212 2023-05-05 06:47:11.847585 hyfi-0.3.3/pyproject.toml
--rw-r--r--   0        0        0     2680 2023-05-05 06:46:37.103479 hyfi-0.3.3/src/hyfi/__cli__.py
--rw-r--r--   0        0        0      331 2023-05-05 06:46:37.103479 hyfi-0.3.3/src/hyfi/__init__.py
--rw-r--r--   0        0        0       22 2023-05-05 06:47:11.771585 hyfi-0.3.3/src/hyfi/_version.py
--rw-r--r--   0        0        0        0 2023-05-05 06:46:37.103479 hyfi-0.3.3/src/hyfi/conf/__init__.py
--rw-r--r--   0        0        0      233 2023-05-05 06:47:11.771585 hyfi-0.3.3/src/hyfi/conf/about/__init__.yaml
--rw-r--r--   0        0        0      331 2023-05-05 06:46:37.103479 hyfi-0.3.3/src/hyfi/conf/batch/__init__.yaml
--rw-r--r--   0        0        0       83 2023-05-05 06:46:37.103479 hyfi-0.3.3/src/hyfi/conf/cmd/about.yaml
--rw-r--r--   0        0        0      167 2023-05-05 06:46:37.103479 hyfi-0.3.3/src/hyfi/conf/cmd/cpcfg.yaml
--rw-r--r--   0        0        0      320 2023-05-05 06:46:37.103479 hyfi-0.3.3/src/hyfi/conf/config.yaml
--rw-r--r--   0        0        0      496 2023-05-05 06:46:37.103479 hyfi-0.3.3/src/hyfi/conf/copier/conf.yaml
--rw-r--r--   0        0        0      789 2023-05-05 06:46:37.103479 hyfi-0.3.3/src/hyfi/conf/dotenv/__init__.yaml
--rw-r--r--   0        0        0      319 2023-05-05 06:46:37.103479 hyfi-0.3.3/src/hyfi/conf/hconf.yaml
--rw-r--r--   0        0        0     1128 2023-05-05 06:46:37.103479 hyfi-0.3.3/src/hyfi/conf/hydra/help/help.yaml
--rw-r--r--   0        0        0      264 2023-05-05 06:46:37.103479 hyfi-0.3.3/src/hyfi/conf/hydra/job_logging/custom.yaml
--rw-r--r--   0        0        0      293 2023-05-05 06:46:37.103479 hyfi-0.3.3/src/hyfi/conf/joblib/__init__.yaml
--rw-r--r--   0        0        0      701 2023-05-05 06:46:37.103479 hyfi-0.3.3/src/hyfi/conf/mode/__init__.yaml
--rw-r--r--   0        0        0      231 2023-05-05 06:46:37.103479 hyfi-0.3.3/src/hyfi/conf/mode/debug.yaml
--rw-r--r--   0        0        0      164 2023-05-05 06:46:37.103479 hyfi-0.3.3/src/hyfi/conf/path/__batch__.yaml
--rw-r--r--   0        0        0      582 2023-05-05 06:46:37.103479 hyfi-0.3.3/src/hyfi/conf/path/__default__.yaml
--rw-r--r--   0        0        0      616 2023-05-05 06:46:37.103479 hyfi-0.3.3/src/hyfi/conf/path/__init__.yaml
--rw-r--r--   0        0        0      360 2023-05-05 06:46:37.103479 hyfi-0.3.3/src/hyfi/conf/project/__init__.yaml
--rw-r--r--   0        0        0       21 2023-05-05 06:46:37.103479 hyfi-0.3.3/src/hyfi/config/__init__.py
--rw-r--r--   0        0        0    14151 2023-05-05 06:46:37.103479 hyfi-0.3.3/src/hyfi/config/batch.py
--rw-r--r--   0        0        0    19819 2023-05-05 06:46:37.103479 hyfi-0.3.3/src/hyfi/env.py
--rw-r--r--   0        0        0    12903 2023-05-05 06:46:37.103479 hyfi-0.3.3/src/hyfi/hydra.py
--rw-r--r--   0        0        0        0 2023-05-05 06:46:37.103479 hyfi-0.3.3/src/hyfi/image/__init__.py
--rw-r--r--   0        0        0     8474 2023-05-05 06:46:37.103479 hyfi-0.3.3/src/hyfi/image/collage.py
--rw-r--r--   0        0        0     4341 2023-05-05 06:46:37.103479 hyfi-0.3.3/src/hyfi/image/motion.py
--rw-r--r--   0        0        0     2556 2023-05-05 06:46:37.103479 hyfi-0.3.3/src/hyfi/image/plot.py
--rw-r--r--   0        0        0     3358 2023-05-05 06:46:37.103479 hyfi-0.3.3/src/hyfi/image/utils.py
--rw-r--r--   0        0        0        0 2023-05-05 06:46:37.103479 hyfi-0.3.3/src/hyfi/io/__init__.py
--rw-r--r--   0        0        0     7152 2023-05-05 06:46:37.103479 hyfi-0.3.3/src/hyfi/io/cached_path.py
--rw-r--r--   0        0        0    12802 2023-05-05 06:46:37.103479 hyfi-0.3.3/src/hyfi/io/file.py
--rw-r--r--   0        0        0    26828 2023-05-05 06:46:37.103479 hyfi-0.3.3/src/hyfi/main.py
--rw-r--r--   0        0        0        0 2023-05-05 06:46:37.103479 hyfi-0.3.3/src/hyfi/py.typed
--rw-r--r--   0        0        0        0 2023-05-05 06:46:37.103479 hyfi-0.3.3/src/hyfi/utils/__init__.py
--rw-r--r--   0        0        0      111 2023-05-05 06:46:37.103479 hyfi-0.3.3/src/hyfi/utils/batch/__init__.py
--rw-r--r--   0        0        0     2934 2023-05-05 06:46:37.103479 hyfi-0.3.3/src/hyfi/utils/batch/apply.py
--rw-r--r--   0        0        0     2046 2023-05-05 06:46:37.103479 hyfi-0.3.3/src/hyfi/utils/batch/apply_batch.py
--rw-r--r--   0        0        0    17469 2023-05-05 06:46:37.107479 hyfi-0.3.3/src/hyfi/utils/batch/batcher.py
--rw-r--r--   0        0        0     1206 2023-05-05 06:46:37.107479 hyfi-0.3.3/src/hyfi/utils/cached_path/__init__.py
--rw-r--r--   0        0        0    14396 2023-05-05 06:46:37.107479 hyfi-0.3.3/src/hyfi/utils/cached_path/_cached_path.py
--rw-r--r--   0        0        0     1619 2023-05-05 06:46:37.107479 hyfi-0.3.3/src/hyfi/utils/cached_path/cache_file.py
--rw-r--r--   0        0        0     1110 2023-05-05 06:46:37.107479 hyfi-0.3.3/src/hyfi/utils/cached_path/common.py
--rw-r--r--   0        0        0     1923 2023-05-05 06:46:37.107479 hyfi-0.3.3/src/hyfi/utils/cached_path/file_lock.py
--rw-r--r--   0        0        0     3440 2023-05-05 06:46:37.107479 hyfi-0.3.3/src/hyfi/utils/cached_path/meta.py
--rw-r--r--   0        0        0     3326 2023-05-05 06:46:37.107479 hyfi-0.3.3/src/hyfi/utils/cached_path/progress.py
--rw-r--r--   0        0        0     1460 2023-05-05 06:46:37.107479 hyfi-0.3.3/src/hyfi/utils/cached_path/schemes/__init__.py
--rw-r--r--   0        0        0     1815 2023-05-05 06:46:37.107479 hyfi-0.3.3/src/hyfi/utils/cached_path/schemes/beaker.py
--rw-r--r--   0        0        0     2862 2023-05-05 06:46:37.107479 hyfi-0.3.3/src/hyfi/utils/cached_path/schemes/hf.py
--rw-r--r--   0        0        0     2999 2023-05-05 06:46:37.107479 hyfi-0.3.3/src/hyfi/utils/cached_path/schemes/http.py
--rw-r--r--   0        0        0     3645 2023-05-05 06:46:37.107479 hyfi-0.3.3/src/hyfi/utils/cached_path/schemes/scheme_client.py
--rw-r--r--   0        0        0     1244 2023-05-05 06:46:37.107479 hyfi-0.3.3/src/hyfi/utils/cached_path/testing.py
--rw-r--r--   0        0        0     4834 2023-05-05 06:46:37.107479 hyfi-0.3.3/src/hyfi/utils/cached_path/util.py
--rw-r--r--   0        0        0      464 2023-05-05 06:46:37.107479 hyfi-0.3.3/src/hyfi/utils/cached_path/version.py
--rw-r--r--   0        0        0     5464 2023-05-05 06:46:37.107479 hyfi-0.3.3/src/hyfi/utils/copier.py
--rw-r--r--   0        0        0     2281 2023-05-05 06:46:37.107479 hyfi-0.3.3/src/hyfi/utils/env.py
--rw-r--r--   0        0        0    10202 2023-05-05 06:46:37.107479 hyfi-0.3.3/src/hyfi/utils/func.py
--rw-r--r--   0        0        0     1046 2023-05-05 06:46:37.107479 hyfi-0.3.3/src/hyfi/utils/google.py
--rw-r--r--   0        0        0     3726 2023-05-05 06:46:37.107479 hyfi-0.3.3/src/hyfi/utils/gpu.py
--rw-r--r--   0        0        0     5234 2023-05-05 06:46:37.107479 hyfi-0.3.3/src/hyfi/utils/lib.py
--rw-r--r--   0        0        0     1074 2023-05-05 06:46:37.107479 hyfi-0.3.3/src/hyfi/utils/logging.py
--rw-r--r--   0        0        0    10003 2023-05-05 06:46:37.107479 hyfi-0.3.3/src/hyfi/utils/notebook.py
--rw-r--r--   0        0        0     2123 2023-05-05 06:46:37.107479 hyfi-0.3.3/src/hyfi/utils/pipe.py
--rw-r--r--   0        0        0     5488 2023-05-05 06:46:37.107479 hyfi-0.3.3/src/hyfi/utils/tools.py
--rw-r--r--   0        0        0     2948 1970-01-01 00:00:00.000000 hyfi-0.3.3/PKG-INFO
+-rw-r--r--   0        0        0     1071 2023-05-05 07:49:12.568156 hyfi-0.3.4/LICENSE
+-rw-r--r--   0        0        0     1632 2023-05-05 07:49:12.568156 hyfi-0.3.4/README.md
+-rw-r--r--   0        0        0     4212 2023-05-05 07:49:38.860510 hyfi-0.3.4/pyproject.toml
+-rw-r--r--   0        0        0     2708 2023-05-05 07:49:12.572156 hyfi-0.3.4/src/hyfi/__cli__.py
+-rw-r--r--   0        0        0      331 2023-05-05 07:49:12.572156 hyfi-0.3.4/src/hyfi/__init__.py
+-rw-r--r--   0        0        0       22 2023-05-05 07:49:38.800510 hyfi-0.3.4/src/hyfi/_version.py
+-rw-r--r--   0        0        0        0 2023-05-05 07:49:12.572156 hyfi-0.3.4/src/hyfi/conf/__init__.py
+-rw-r--r--   0        0        0      233 2023-05-05 07:49:38.804509 hyfi-0.3.4/src/hyfi/conf/about/__init__.yaml
+-rw-r--r--   0        0        0      331 2023-05-05 07:49:12.572156 hyfi-0.3.4/src/hyfi/conf/batch/__init__.yaml
+-rw-r--r--   0        0        0       83 2023-05-05 07:49:12.572156 hyfi-0.3.4/src/hyfi/conf/cmd/about.yaml
+-rw-r--r--   0        0        0      167 2023-05-05 07:49:12.572156 hyfi-0.3.4/src/hyfi/conf/cmd/cpcfg.yaml
+-rw-r--r--   0        0        0      320 2023-05-05 07:49:12.572156 hyfi-0.3.4/src/hyfi/conf/config.yaml
+-rw-r--r--   0        0        0      552 2023-05-05 07:49:12.572156 hyfi-0.3.4/src/hyfi/conf/copier/conf.yaml
+-rw-r--r--   0        0        0      789 2023-05-05 07:49:12.572156 hyfi-0.3.4/src/hyfi/conf/dotenv/__init__.yaml
+-rw-r--r--   0        0        0      319 2023-05-05 07:49:12.572156 hyfi-0.3.4/src/hyfi/conf/hconf.yaml
+-rw-r--r--   0        0        0     1128 2023-05-05 07:49:12.572156 hyfi-0.3.4/src/hyfi/conf/hydra/help/help.yaml
+-rw-r--r--   0        0        0      264 2023-05-05 07:49:12.572156 hyfi-0.3.4/src/hyfi/conf/hydra/job_logging/custom.yaml
+-rw-r--r--   0        0        0      293 2023-05-05 07:49:12.572156 hyfi-0.3.4/src/hyfi/conf/joblib/__init__.yaml
+-rw-r--r--   0        0        0      701 2023-05-05 07:49:12.572156 hyfi-0.3.4/src/hyfi/conf/mode/__init__.yaml
+-rw-r--r--   0        0        0      231 2023-05-05 07:49:12.572156 hyfi-0.3.4/src/hyfi/conf/mode/debug.yaml
+-rw-r--r--   0        0        0      164 2023-05-05 07:49:12.572156 hyfi-0.3.4/src/hyfi/conf/path/__batch__.yaml
+-rw-r--r--   0        0        0      582 2023-05-05 07:49:12.572156 hyfi-0.3.4/src/hyfi/conf/path/__default__.yaml
+-rw-r--r--   0        0        0      616 2023-05-05 07:49:12.572156 hyfi-0.3.4/src/hyfi/conf/path/__init__.yaml
+-rw-r--r--   0        0        0      360 2023-05-05 07:49:12.572156 hyfi-0.3.4/src/hyfi/conf/project/__init__.yaml
+-rw-r--r--   0        0        0       21 2023-05-05 07:49:12.572156 hyfi-0.3.4/src/hyfi/config/__init__.py
+-rw-r--r--   0        0        0    14151 2023-05-05 07:49:12.572156 hyfi-0.3.4/src/hyfi/config/batch.py
+-rw-r--r--   0        0        0    19819 2023-05-05 07:49:12.572156 hyfi-0.3.4/src/hyfi/env.py
+-rw-r--r--   0        0        0    12903 2023-05-05 07:49:12.572156 hyfi-0.3.4/src/hyfi/hydra.py
+-rw-r--r--   0        0        0        0 2023-05-05 07:49:12.572156 hyfi-0.3.4/src/hyfi/image/__init__.py
+-rw-r--r--   0        0        0     8474 2023-05-05 07:49:12.572156 hyfi-0.3.4/src/hyfi/image/collage.py
+-rw-r--r--   0        0        0     4341 2023-05-05 07:49:12.572156 hyfi-0.3.4/src/hyfi/image/motion.py
+-rw-r--r--   0        0        0     2556 2023-05-05 07:49:12.572156 hyfi-0.3.4/src/hyfi/image/plot.py
+-rw-r--r--   0        0        0     3358 2023-05-05 07:49:12.572156 hyfi-0.3.4/src/hyfi/image/utils.py
+-rw-r--r--   0        0        0        0 2023-05-05 07:49:12.572156 hyfi-0.3.4/src/hyfi/io/__init__.py
+-rw-r--r--   0        0        0     7152 2023-05-05 07:49:12.572156 hyfi-0.3.4/src/hyfi/io/cached_path.py
+-rw-r--r--   0        0        0    12802 2023-05-05 07:49:12.572156 hyfi-0.3.4/src/hyfi/io/file.py
+-rw-r--r--   0        0        0    26828 2023-05-05 07:49:12.572156 hyfi-0.3.4/src/hyfi/main.py
+-rw-r--r--   0        0        0        0 2023-05-05 07:49:12.572156 hyfi-0.3.4/src/hyfi/py.typed
+-rw-r--r--   0        0        0        0 2023-05-05 07:49:12.572156 hyfi-0.3.4/src/hyfi/utils/__init__.py
+-rw-r--r--   0        0        0      111 2023-05-05 07:49:12.572156 hyfi-0.3.4/src/hyfi/utils/batch/__init__.py
+-rw-r--r--   0        0        0     2934 2023-05-05 07:49:12.572156 hyfi-0.3.4/src/hyfi/utils/batch/apply.py
+-rw-r--r--   0        0        0     2046 2023-05-05 07:49:12.572156 hyfi-0.3.4/src/hyfi/utils/batch/apply_batch.py
+-rw-r--r--   0        0        0    17469 2023-05-05 07:49:12.572156 hyfi-0.3.4/src/hyfi/utils/batch/batcher.py
+-rw-r--r--   0        0        0     1206 2023-05-05 07:49:12.572156 hyfi-0.3.4/src/hyfi/utils/cached_path/__init__.py
+-rw-r--r--   0        0        0    14396 2023-05-05 07:49:12.572156 hyfi-0.3.4/src/hyfi/utils/cached_path/_cached_path.py
+-rw-r--r--   0        0        0     1619 2023-05-05 07:49:12.572156 hyfi-0.3.4/src/hyfi/utils/cached_path/cache_file.py
+-rw-r--r--   0        0        0     1110 2023-05-05 07:49:12.572156 hyfi-0.3.4/src/hyfi/utils/cached_path/common.py
+-rw-r--r--   0        0        0     1923 2023-05-05 07:49:12.572156 hyfi-0.3.4/src/hyfi/utils/cached_path/file_lock.py
+-rw-r--r--   0        0        0     3440 2023-05-05 07:49:12.572156 hyfi-0.3.4/src/hyfi/utils/cached_path/meta.py
+-rw-r--r--   0        0        0     3326 2023-05-05 07:49:12.572156 hyfi-0.3.4/src/hyfi/utils/cached_path/progress.py
+-rw-r--r--   0        0        0     1460 2023-05-05 07:49:12.572156 hyfi-0.3.4/src/hyfi/utils/cached_path/schemes/__init__.py
+-rw-r--r--   0        0        0     1815 2023-05-05 07:49:12.576156 hyfi-0.3.4/src/hyfi/utils/cached_path/schemes/beaker.py
+-rw-r--r--   0        0        0     2862 2023-05-05 07:49:12.576156 hyfi-0.3.4/src/hyfi/utils/cached_path/schemes/hf.py
+-rw-r--r--   0        0        0     2999 2023-05-05 07:49:12.576156 hyfi-0.3.4/src/hyfi/utils/cached_path/schemes/http.py
+-rw-r--r--   0        0        0     3645 2023-05-05 07:49:12.576156 hyfi-0.3.4/src/hyfi/utils/cached_path/schemes/scheme_client.py
+-rw-r--r--   0        0        0     1244 2023-05-05 07:49:12.576156 hyfi-0.3.4/src/hyfi/utils/cached_path/testing.py
+-rw-r--r--   0        0        0     4834 2023-05-05 07:49:12.576156 hyfi-0.3.4/src/hyfi/utils/cached_path/util.py
+-rw-r--r--   0        0        0      464 2023-05-05 07:49:12.576156 hyfi-0.3.4/src/hyfi/utils/cached_path/version.py
+-rw-r--r--   0        0        0     6131 2023-05-05 07:49:12.576156 hyfi-0.3.4/src/hyfi/utils/copier.py
+-rw-r--r--   0        0        0     2281 2023-05-05 07:49:12.576156 hyfi-0.3.4/src/hyfi/utils/env.py
+-rw-r--r--   0        0        0    10202 2023-05-05 07:49:12.576156 hyfi-0.3.4/src/hyfi/utils/func.py
+-rw-r--r--   0        0        0     1046 2023-05-05 07:49:12.576156 hyfi-0.3.4/src/hyfi/utils/google.py
+-rw-r--r--   0        0        0     3726 2023-05-05 07:49:12.576156 hyfi-0.3.4/src/hyfi/utils/gpu.py
+-rw-r--r--   0        0        0     5234 2023-05-05 07:49:12.576156 hyfi-0.3.4/src/hyfi/utils/lib.py
+-rw-r--r--   0        0        0     1074 2023-05-05 07:49:12.576156 hyfi-0.3.4/src/hyfi/utils/logging.py
+-rw-r--r--   0        0        0    10003 2023-05-05 07:49:12.576156 hyfi-0.3.4/src/hyfi/utils/notebook.py
+-rw-r--r--   0        0        0     2123 2023-05-05 07:49:12.576156 hyfi-0.3.4/src/hyfi/utils/pipe.py
+-rw-r--r--   0        0        0     5481 2023-05-05 07:49:12.576156 hyfi-0.3.4/src/hyfi/utils/tools.py
+-rw-r--r--   0        0        0      153 2023-05-05 07:49:12.576156 hyfi-0.3.4/src/hyfi/utils/types.py
+-rw-r--r--   0        0        0     2948 1970-01-01 00:00:00.000000 hyfi-0.3.4/PKG-INFO
```

### Comparing `hyfi-0.3.3/LICENSE` & `hyfi-0.3.4/LICENSE`

 * *Files identical despite different names*

### Comparing `hyfi-0.3.3/README.md` & `hyfi-0.3.4/README.md`

 * *Files identical despite different names*

### Comparing `hyfi-0.3.3/pyproject.toml` & `hyfi-0.3.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "hyfi"
-version = "0.3.3"
+version = "0.3.4"
 description = "Hydra Fast Interface (Hydra and Pydantic based interface framework)"
 authors = ["Young Joon Lee <entelecheia@hotmail.com>"]
 license = "MIT"
 homepage = "https://hyfi.entelecheia.ai"
 repository = "https://github.com/entelecheia/hyfi"
 readme = "README.md"
 packages = [{ include = "hyfi", from = "src" }]
```

### Comparing `hyfi-0.3.3/src/hyfi/__cli__.py` & `hyfi-0.3.4/src/hyfi/__cli__.py`

 * *Files 2% similar despite different names*

```diff
@@ -25,15 +25,16 @@
     cfg = HyfiConfig(**args)
     _about(cfg)
 
 
 def run_copy(**args):
     """Copy all config files in the config directory to the current working directory"""
     cfg = HyfiConfig(**args)
-    with Copier(**cfg.copier) as worker:
+    cfg = HyFI.to_dict(cfg.copier)
+    with Copier(**cfg) as worker:
         worker.run_copy()
 
 
 def cli_main(cfg: DictConfig) -> None:
     """Main function for the command line interface"""
     hyfi = HyfiConfig(**cfg)
     verbose = hyfi.verbose
```

### Comparing `hyfi-0.3.3/src/hyfi/conf/dotenv/__init__.yaml` & `hyfi-0.3.4/src/hyfi/conf/dotenv/__init__.yaml`

 * *Files identical despite different names*

### Comparing `hyfi-0.3.3/src/hyfi/conf/hydra/help/help.yaml` & `hyfi-0.3.4/src/hyfi/conf/hydra/help/help.yaml`

 * *Files identical despite different names*

### Comparing `hyfi-0.3.3/src/hyfi/conf/mode/__init__.yaml` & `hyfi-0.3.4/src/hyfi/conf/mode/__init__.yaml`

 * *Files identical despite different names*

### Comparing `hyfi-0.3.3/src/hyfi/conf/path/__default__.yaml` & `hyfi-0.3.4/src/hyfi/conf/path/__default__.yaml`

 * *Files identical despite different names*

### Comparing `hyfi-0.3.3/src/hyfi/conf/path/__init__.yaml` & `hyfi-0.3.4/src/hyfi/conf/path/__init__.yaml`

 * *Files identical despite different names*

### Comparing `hyfi-0.3.3/src/hyfi/config/batch.py` & `hyfi-0.3.4/src/hyfi/config/batch.py`

 * *Files identical despite different names*

### Comparing `hyfi-0.3.3/src/hyfi/env.py` & `hyfi-0.3.4/src/hyfi/env.py`

 * *Files identical despite different names*

### Comparing `hyfi-0.3.3/src/hyfi/hydra.py` & `hyfi-0.3.4/src/hyfi/hydra.py`

 * *Files identical despite different names*

### Comparing `hyfi-0.3.3/src/hyfi/image/collage.py` & `hyfi-0.3.4/src/hyfi/image/collage.py`

 * *Files identical despite different names*

### Comparing `hyfi-0.3.3/src/hyfi/image/motion.py` & `hyfi-0.3.4/src/hyfi/image/motion.py`

 * *Files identical despite different names*

### Comparing `hyfi-0.3.3/src/hyfi/image/plot.py` & `hyfi-0.3.4/src/hyfi/image/plot.py`

 * *Files identical despite different names*

### Comparing `hyfi-0.3.3/src/hyfi/image/utils.py` & `hyfi-0.3.4/src/hyfi/image/utils.py`

 * *Files identical despite different names*

### Comparing `hyfi-0.3.3/src/hyfi/io/cached_path.py` & `hyfi-0.3.4/src/hyfi/io/cached_path.py`

 * *Files identical despite different names*

### Comparing `hyfi-0.3.3/src/hyfi/io/file.py` & `hyfi-0.3.4/src/hyfi/io/file.py`

 * *Files identical despite different names*

### Comparing `hyfi-0.3.3/src/hyfi/main.py` & `hyfi-0.3.4/src/hyfi/main.py`

 * *Files identical despite different names*

### Comparing `hyfi-0.3.3/src/hyfi/utils/batch/apply.py` & `hyfi-0.3.4/src/hyfi/utils/batch/apply.py`

 * *Files identical despite different names*

### Comparing `hyfi-0.3.3/src/hyfi/utils/batch/apply_batch.py` & `hyfi-0.3.4/src/hyfi/utils/batch/apply_batch.py`

 * *Files identical despite different names*

### Comparing `hyfi-0.3.3/src/hyfi/utils/batch/batcher.py` & `hyfi-0.3.4/src/hyfi/utils/batch/batcher.py`

 * *Files identical despite different names*

### Comparing `hyfi-0.3.3/src/hyfi/utils/cached_path/__init__.py` & `hyfi-0.3.4/src/hyfi/utils/cached_path/__init__.py`

 * *Files identical despite different names*

### Comparing `hyfi-0.3.3/src/hyfi/utils/cached_path/_cached_path.py` & `hyfi-0.3.4/src/hyfi/utils/cached_path/_cached_path.py`

 * *Files identical despite different names*

### Comparing `hyfi-0.3.3/src/hyfi/utils/cached_path/cache_file.py` & `hyfi-0.3.4/src/hyfi/utils/cached_path/cache_file.py`

 * *Files identical despite different names*

### Comparing `hyfi-0.3.3/src/hyfi/utils/cached_path/common.py` & `hyfi-0.3.4/src/hyfi/utils/cached_path/common.py`

 * *Files identical despite different names*

### Comparing `hyfi-0.3.3/src/hyfi/utils/cached_path/file_lock.py` & `hyfi-0.3.4/src/hyfi/utils/cached_path/file_lock.py`

 * *Files identical despite different names*

### Comparing `hyfi-0.3.3/src/hyfi/utils/cached_path/meta.py` & `hyfi-0.3.4/src/hyfi/utils/cached_path/meta.py`

 * *Files identical despite different names*

### Comparing `hyfi-0.3.3/src/hyfi/utils/cached_path/progress.py` & `hyfi-0.3.4/src/hyfi/utils/cached_path/progress.py`

 * *Files identical despite different names*

### Comparing `hyfi-0.3.3/src/hyfi/utils/cached_path/schemes/__init__.py` & `hyfi-0.3.4/src/hyfi/utils/cached_path/schemes/__init__.py`

 * *Files identical despite different names*

### Comparing `hyfi-0.3.3/src/hyfi/utils/cached_path/schemes/beaker.py` & `hyfi-0.3.4/src/hyfi/utils/cached_path/schemes/beaker.py`

 * *Files identical despite different names*

### Comparing `hyfi-0.3.3/src/hyfi/utils/cached_path/schemes/hf.py` & `hyfi-0.3.4/src/hyfi/utils/cached_path/schemes/hf.py`

 * *Files identical despite different names*

### Comparing `hyfi-0.3.3/src/hyfi/utils/cached_path/schemes/http.py` & `hyfi-0.3.4/src/hyfi/utils/cached_path/schemes/http.py`

 * *Files identical despite different names*

### Comparing `hyfi-0.3.3/src/hyfi/utils/cached_path/schemes/scheme_client.py` & `hyfi-0.3.4/src/hyfi/utils/cached_path/schemes/scheme_client.py`

 * *Files identical despite different names*

### Comparing `hyfi-0.3.3/src/hyfi/utils/cached_path/testing.py` & `hyfi-0.3.4/src/hyfi/utils/cached_path/testing.py`

 * *Files identical despite different names*

### Comparing `hyfi-0.3.3/src/hyfi/utils/cached_path/util.py` & `hyfi-0.3.4/src/hyfi/utils/cached_path/util.py`

 * *Files identical despite different names*

### Comparing `hyfi-0.3.3/src/hyfi/utils/copier.py` & `hyfi-0.3.4/src/hyfi/utils/copier.py`

 * *Files 5% similar despite different names*

```diff
@@ -49,14 +49,17 @@
     Attributes:
         src_path:
             Source path where to find the template.
 
         dst_path:
             Destination path where to render the template.
 
+        filetypes:
+            Filetypes to copy.
+
         exclude:
             User-chosen additional file exclusion patterns.
 
         skip_if_exists:
             User-chosen additional file skip patterns.
 
         cleanup_on_error:
@@ -70,37 +73,41 @@
 
         verbose:
             When `True`, show all output.
     """
 
     src_path: Path = field(default=Path("config"))
     dst_path: Path = field(default=Path("."))
-    exclude: List[str] = field(default_factory=list)
-    skip_if_exists: List[str] = field(default_factory=list)
+    filetypes: List = field(default_factory=list)
+    exclude: List = field(default_factory=list)
+    skip_if_exists: bool = False
     cleanup_on_error: bool = True
     overwrite: bool = False
     dry_run: bool = False
     verbose: bool = True
 
     def __post_init__(self):
         """Initialize the path_spec attribute based on the exclude patterns."""
         # Validate and convert src_path and dst_path
         for attr_name in ["src_path", "dst_path"]:
             attr_value = getattr(self, attr_name)
             if not isinstance(attr_value, Path):
                 setattr(self, attr_name, Path(attr_value))
 
-        # Validate and convert exclude and skip_if_exists
-        for attr_name in ["exclude", "skip_if_exists"]:
+        # Validate and convert exclude and filetypes
+        for attr_name in ["exclude", "filetypes"]:
             attr_value = getattr(self, attr_name)
             if attr_value is None:
                 setattr(self, attr_name, [])
             elif not isinstance(attr_value, list):
                 setattr(self, attr_name, [attr_value])
 
+        if self.filetypes is None or len(self.filetypes) == 0:
+            self.filetypes = ["yaml", "yml", "py"]
+
         if not self.dst_path.is_absolute():
             self.dst_path = getcwd() / self.dst_path
         self.path_spec = PathSpec.from_lines("gitwildmatch", self.exclude)
         self.dst_path_existed = self.dst_path.exists()
 
     def __enter__(self):
         return self
@@ -120,38 +127,52 @@
         """Execute the copy process.
 
         Walk through the source directory, compare YAML files with the destination
         directory, and copy files based on the specified settings.
         """
         for root, _, files in os.walk(self.src_path):
             for filename in files:
+                if not any(filename.endswith(filetype) for filetype in self.filetypes):
+                    continue
+
                 src_file = Path(root, filename)
                 dst_file = self.dst_path / src_file.relative_to(self.src_path)
                 dst_file = dst_file.absolute()
 
                 if self.path_spec.match_file(src_file):
                     printf(
-                        "IGNORE", f"{src_file}", Style.IGNORE, verbose=self.verbose
+                        "EXCLUDED", f"{src_file}", Style.WARNING, verbose=self.verbose
                     )
                     continue
 
-                if dst_file.exists() and not self.overwrite:
+                if dst_file.exists():
+                    if self.skip_if_exists:
+                        printf(
+                            "SKIPPED",
+                            f"{src_file}",
+                            Style.WARNING,
+                            verbose=self.verbose,
+                        )
+                        continue
+
                     if filecmp.cmp(src_file, dst_file, shallow=False):
                         printf(
                             "UNCHANGED",
                             f"{src_file}",
-                            Style.OK,
+                            Style.IGNORE,
                             verbose=self.verbose,
                         )
                         continue
 
-                    answer = input(f"Overwrite {dst_file}? [Y/n]: ") or "Y"
+                    answer = "Y"
+                    if not self.overwrite:
+                        answer = input(f"Overwrite {dst_file}? [Y/n]: ") or "Y"
                     if answer.lower() != "y":
                         printf(
-                            "SKIPPED",
+                            "IGNORED",
                             f"{src_file}",
                             Style.WARNING,
                             verbose=self.verbose,
                         )
                         continue
 
                 if not self.dry_run:
```

### Comparing `hyfi-0.3.3/src/hyfi/utils/env.py` & `hyfi-0.3.4/src/hyfi/utils/env.py`

 * *Files identical despite different names*

### Comparing `hyfi-0.3.3/src/hyfi/utils/func.py` & `hyfi-0.3.4/src/hyfi/utils/func.py`

 * *Files identical despite different names*

### Comparing `hyfi-0.3.3/src/hyfi/utils/google.py` & `hyfi-0.3.4/src/hyfi/utils/google.py`

 * *Files identical despite different names*

### Comparing `hyfi-0.3.3/src/hyfi/utils/gpu.py` & `hyfi-0.3.4/src/hyfi/utils/gpu.py`

 * *Files identical despite different names*

### Comparing `hyfi-0.3.3/src/hyfi/utils/lib.py` & `hyfi-0.3.4/src/hyfi/utils/lib.py`

 * *Files identical despite different names*

### Comparing `hyfi-0.3.3/src/hyfi/utils/logging.py` & `hyfi-0.3.4/src/hyfi/utils/logging.py`

 * *Files identical despite different names*

### Comparing `hyfi-0.3.3/src/hyfi/utils/notebook.py` & `hyfi-0.3.4/src/hyfi/utils/notebook.py`

 * *Files identical despite different names*

### Comparing `hyfi-0.3.3/src/hyfi/utils/pipe.py` & `hyfi-0.3.4/src/hyfi/utils/pipe.py`

 * *Files identical despite different names*

### Comparing `hyfi-0.3.3/src/hyfi/utils/tools.py` & `hyfi-0.3.4/src/hyfi/utils/tools.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,22 +6,22 @@
 import stat
 import sys
 import tempfile
 import warnings
 from contextlib import suppress
 from pathlib import Path
 from types import TracebackType
-from typing import Any, Callable, Optional, Sequence, TextIO, Tuple, Union
+from typing import Any, Callable, Optional, TextIO, Tuple, Union
 
 import colorama
 from pydantic import StrictBool
 
-colorama.init()
+from .types import IntSeq
 
-IntSeq = Sequence[int]
+colorama.init()
 
 
 class Style:
     """Common color styles."""
 
     OK: IntSeq = [colorama.Fore.GREEN, colorama.Style.BRIGHT]
     WARNING: IntSeq = [colorama.Fore.YELLOW, colorama.Style.BRIGHT]
```

### Comparing `hyfi-0.3.3/PKG-INFO` & `hyfi-0.3.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hyfi
-Version: 0.3.3
+Version: 0.3.4
 Summary: Hydra Fast Interface (Hydra and Pydantic based interface framework)
 Home-page: https://hyfi.entelecheia.ai
 License: MIT
 Author: Young Joon Lee
 Author-email: entelecheia@hotmail.com
 Requires-Python: >=3.8.1,<3.12
 Classifier: License :: OSI Approved :: MIT License
```

