# Comparing `tmp/hyfi-0.3.4.tar.gz` & `tmp/hyfi-0.3.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hyfi-0.3.4.tar", max compression
+gzip compressed data, was "hyfi-0.3.5.tar", max compression
```

## Comparing `hyfi-0.3.4.tar` & `hyfi-0.3.5.tar`

### file list

```diff
@@ -1,70 +1,70 @@
--rw-r--r--   0        0        0     1071 2023-05-05 07:49:12.568156 hyfi-0.3.4/LICENSE
--rw-r--r--   0        0        0     1632 2023-05-05 07:49:12.568156 hyfi-0.3.4/README.md
--rw-r--r--   0        0        0     4212 2023-05-05 07:49:38.860510 hyfi-0.3.4/pyproject.toml
--rw-r--r--   0        0        0     2708 2023-05-05 07:49:12.572156 hyfi-0.3.4/src/hyfi/__cli__.py
--rw-r--r--   0        0        0      331 2023-05-05 07:49:12.572156 hyfi-0.3.4/src/hyfi/__init__.py
--rw-r--r--   0        0        0       22 2023-05-05 07:49:38.800510 hyfi-0.3.4/src/hyfi/_version.py
--rw-r--r--   0        0        0        0 2023-05-05 07:49:12.572156 hyfi-0.3.4/src/hyfi/conf/__init__.py
--rw-r--r--   0        0        0      233 2023-05-05 07:49:38.804509 hyfi-0.3.4/src/hyfi/conf/about/__init__.yaml
--rw-r--r--   0        0        0      331 2023-05-05 07:49:12.572156 hyfi-0.3.4/src/hyfi/conf/batch/__init__.yaml
--rw-r--r--   0        0        0       83 2023-05-05 07:49:12.572156 hyfi-0.3.4/src/hyfi/conf/cmd/about.yaml
--rw-r--r--   0        0        0      167 2023-05-05 07:49:12.572156 hyfi-0.3.4/src/hyfi/conf/cmd/cpcfg.yaml
--rw-r--r--   0        0        0      320 2023-05-05 07:49:12.572156 hyfi-0.3.4/src/hyfi/conf/config.yaml
--rw-r--r--   0        0        0      552 2023-05-05 07:49:12.572156 hyfi-0.3.4/src/hyfi/conf/copier/conf.yaml
--rw-r--r--   0        0        0      789 2023-05-05 07:49:12.572156 hyfi-0.3.4/src/hyfi/conf/dotenv/__init__.yaml
--rw-r--r--   0        0        0      319 2023-05-05 07:49:12.572156 hyfi-0.3.4/src/hyfi/conf/hconf.yaml
--rw-r--r--   0        0        0     1128 2023-05-05 07:49:12.572156 hyfi-0.3.4/src/hyfi/conf/hydra/help/help.yaml
--rw-r--r--   0        0        0      264 2023-05-05 07:49:12.572156 hyfi-0.3.4/src/hyfi/conf/hydra/job_logging/custom.yaml
--rw-r--r--   0        0        0      293 2023-05-05 07:49:12.572156 hyfi-0.3.4/src/hyfi/conf/joblib/__init__.yaml
--rw-r--r--   0        0        0      701 2023-05-05 07:49:12.572156 hyfi-0.3.4/src/hyfi/conf/mode/__init__.yaml
--rw-r--r--   0        0        0      231 2023-05-05 07:49:12.572156 hyfi-0.3.4/src/hyfi/conf/mode/debug.yaml
--rw-r--r--   0        0        0      164 2023-05-05 07:49:12.572156 hyfi-0.3.4/src/hyfi/conf/path/__batch__.yaml
--rw-r--r--   0        0        0      582 2023-05-05 07:49:12.572156 hyfi-0.3.4/src/hyfi/conf/path/__default__.yaml
--rw-r--r--   0        0        0      616 2023-05-05 07:49:12.572156 hyfi-0.3.4/src/hyfi/conf/path/__init__.yaml
--rw-r--r--   0        0        0      360 2023-05-05 07:49:12.572156 hyfi-0.3.4/src/hyfi/conf/project/__init__.yaml
--rw-r--r--   0        0        0       21 2023-05-05 07:49:12.572156 hyfi-0.3.4/src/hyfi/config/__init__.py
--rw-r--r--   0        0        0    14151 2023-05-05 07:49:12.572156 hyfi-0.3.4/src/hyfi/config/batch.py
--rw-r--r--   0        0        0    19819 2023-05-05 07:49:12.572156 hyfi-0.3.4/src/hyfi/env.py
--rw-r--r--   0        0        0    12903 2023-05-05 07:49:12.572156 hyfi-0.3.4/src/hyfi/hydra.py
--rw-r--r--   0        0        0        0 2023-05-05 07:49:12.572156 hyfi-0.3.4/src/hyfi/image/__init__.py
--rw-r--r--   0        0        0     8474 2023-05-05 07:49:12.572156 hyfi-0.3.4/src/hyfi/image/collage.py
--rw-r--r--   0        0        0     4341 2023-05-05 07:49:12.572156 hyfi-0.3.4/src/hyfi/image/motion.py
--rw-r--r--   0        0        0     2556 2023-05-05 07:49:12.572156 hyfi-0.3.4/src/hyfi/image/plot.py
--rw-r--r--   0        0        0     3358 2023-05-05 07:49:12.572156 hyfi-0.3.4/src/hyfi/image/utils.py
--rw-r--r--   0        0        0        0 2023-05-05 07:49:12.572156 hyfi-0.3.4/src/hyfi/io/__init__.py
--rw-r--r--   0        0        0     7152 2023-05-05 07:49:12.572156 hyfi-0.3.4/src/hyfi/io/cached_path.py
--rw-r--r--   0        0        0    12802 2023-05-05 07:49:12.572156 hyfi-0.3.4/src/hyfi/io/file.py
--rw-r--r--   0        0        0    26828 2023-05-05 07:49:12.572156 hyfi-0.3.4/src/hyfi/main.py
--rw-r--r--   0        0        0        0 2023-05-05 07:49:12.572156 hyfi-0.3.4/src/hyfi/py.typed
--rw-r--r--   0        0        0        0 2023-05-05 07:49:12.572156 hyfi-0.3.4/src/hyfi/utils/__init__.py
--rw-r--r--   0        0        0      111 2023-05-05 07:49:12.572156 hyfi-0.3.4/src/hyfi/utils/batch/__init__.py
--rw-r--r--   0        0        0     2934 2023-05-05 07:49:12.572156 hyfi-0.3.4/src/hyfi/utils/batch/apply.py
--rw-r--r--   0        0        0     2046 2023-05-05 07:49:12.572156 hyfi-0.3.4/src/hyfi/utils/batch/apply_batch.py
--rw-r--r--   0        0        0    17469 2023-05-05 07:49:12.572156 hyfi-0.3.4/src/hyfi/utils/batch/batcher.py
--rw-r--r--   0        0        0     1206 2023-05-05 07:49:12.572156 hyfi-0.3.4/src/hyfi/utils/cached_path/__init__.py
--rw-r--r--   0        0        0    14396 2023-05-05 07:49:12.572156 hyfi-0.3.4/src/hyfi/utils/cached_path/_cached_path.py
--rw-r--r--   0        0        0     1619 2023-05-05 07:49:12.572156 hyfi-0.3.4/src/hyfi/utils/cached_path/cache_file.py
--rw-r--r--   0        0        0     1110 2023-05-05 07:49:12.572156 hyfi-0.3.4/src/hyfi/utils/cached_path/common.py
--rw-r--r--   0        0        0     1923 2023-05-05 07:49:12.572156 hyfi-0.3.4/src/hyfi/utils/cached_path/file_lock.py
--rw-r--r--   0        0        0     3440 2023-05-05 07:49:12.572156 hyfi-0.3.4/src/hyfi/utils/cached_path/meta.py
--rw-r--r--   0        0        0     3326 2023-05-05 07:49:12.572156 hyfi-0.3.4/src/hyfi/utils/cached_path/progress.py
--rw-r--r--   0        0        0     1460 2023-05-05 07:49:12.572156 hyfi-0.3.4/src/hyfi/utils/cached_path/schemes/__init__.py
--rw-r--r--   0        0        0     1815 2023-05-05 07:49:12.576156 hyfi-0.3.4/src/hyfi/utils/cached_path/schemes/beaker.py
--rw-r--r--   0        0        0     2862 2023-05-05 07:49:12.576156 hyfi-0.3.4/src/hyfi/utils/cached_path/schemes/hf.py
--rw-r--r--   0        0        0     2999 2023-05-05 07:49:12.576156 hyfi-0.3.4/src/hyfi/utils/cached_path/schemes/http.py
--rw-r--r--   0        0        0     3645 2023-05-05 07:49:12.576156 hyfi-0.3.4/src/hyfi/utils/cached_path/schemes/scheme_client.py
--rw-r--r--   0        0        0     1244 2023-05-05 07:49:12.576156 hyfi-0.3.4/src/hyfi/utils/cached_path/testing.py
--rw-r--r--   0        0        0     4834 2023-05-05 07:49:12.576156 hyfi-0.3.4/src/hyfi/utils/cached_path/util.py
--rw-r--r--   0        0        0      464 2023-05-05 07:49:12.576156 hyfi-0.3.4/src/hyfi/utils/cached_path/version.py
--rw-r--r--   0        0        0     6131 2023-05-05 07:49:12.576156 hyfi-0.3.4/src/hyfi/utils/copier.py
--rw-r--r--   0        0        0     2281 2023-05-05 07:49:12.576156 hyfi-0.3.4/src/hyfi/utils/env.py
--rw-r--r--   0        0        0    10202 2023-05-05 07:49:12.576156 hyfi-0.3.4/src/hyfi/utils/func.py
--rw-r--r--   0        0        0     1046 2023-05-05 07:49:12.576156 hyfi-0.3.4/src/hyfi/utils/google.py
--rw-r--r--   0        0        0     3726 2023-05-05 07:49:12.576156 hyfi-0.3.4/src/hyfi/utils/gpu.py
--rw-r--r--   0        0        0     5234 2023-05-05 07:49:12.576156 hyfi-0.3.4/src/hyfi/utils/lib.py
--rw-r--r--   0        0        0     1074 2023-05-05 07:49:12.576156 hyfi-0.3.4/src/hyfi/utils/logging.py
--rw-r--r--   0        0        0    10003 2023-05-05 07:49:12.576156 hyfi-0.3.4/src/hyfi/utils/notebook.py
--rw-r--r--   0        0        0     2123 2023-05-05 07:49:12.576156 hyfi-0.3.4/src/hyfi/utils/pipe.py
--rw-r--r--   0        0        0     5481 2023-05-05 07:49:12.576156 hyfi-0.3.4/src/hyfi/utils/tools.py
--rw-r--r--   0        0        0      153 2023-05-05 07:49:12.576156 hyfi-0.3.4/src/hyfi/utils/types.py
--rw-r--r--   0        0        0     2948 1970-01-01 00:00:00.000000 hyfi-0.3.4/PKG-INFO
+-rw-r--r--   0        0        0     1071 2023-05-05 08:04:32.973784 hyfi-0.3.5/LICENSE
+-rw-r--r--   0        0        0     1632 2023-05-05 08:04:32.973784 hyfi-0.3.5/README.md
+-rw-r--r--   0        0        0     4212 2023-05-05 08:05:06.340135 hyfi-0.3.5/pyproject.toml
+-rw-r--r--   0        0        0     2708 2023-05-05 08:04:32.977784 hyfi-0.3.5/src/hyfi/__cli__.py
+-rw-r--r--   0        0        0      331 2023-05-05 08:04:32.977784 hyfi-0.3.5/src/hyfi/__init__.py
+-rw-r--r--   0        0        0       22 2023-05-05 08:05:06.268130 hyfi-0.3.5/src/hyfi/_version.py
+-rw-r--r--   0        0        0        0 2023-05-05 08:04:32.977784 hyfi-0.3.5/src/hyfi/conf/__init__.py
+-rw-r--r--   0        0        0      233 2023-05-05 08:05:06.268130 hyfi-0.3.5/src/hyfi/conf/about/__init__.yaml
+-rw-r--r--   0        0        0      331 2023-05-05 08:04:32.977784 hyfi-0.3.5/src/hyfi/conf/batch/__init__.yaml
+-rw-r--r--   0        0        0       83 2023-05-05 08:04:32.977784 hyfi-0.3.5/src/hyfi/conf/cmd/about.yaml
+-rw-r--r--   0        0        0      167 2023-05-05 08:04:32.977784 hyfi-0.3.5/src/hyfi/conf/cmd/cpcfg.yaml
+-rw-r--r--   0        0        0      320 2023-05-05 08:04:32.977784 hyfi-0.3.5/src/hyfi/conf/config.yaml
+-rw-r--r--   0        0        0      552 2023-05-05 08:04:32.977784 hyfi-0.3.5/src/hyfi/conf/copier/conf.yaml
+-rw-r--r--   0        0        0      789 2023-05-05 08:04:32.977784 hyfi-0.3.5/src/hyfi/conf/dotenv/__init__.yaml
+-rw-r--r--   0        0        0      319 2023-05-05 08:04:32.977784 hyfi-0.3.5/src/hyfi/conf/hconf.yaml
+-rw-r--r--   0        0        0     1128 2023-05-05 08:04:32.977784 hyfi-0.3.5/src/hyfi/conf/hydra/help/help.yaml
+-rw-r--r--   0        0        0      264 2023-05-05 08:04:32.977784 hyfi-0.3.5/src/hyfi/conf/hydra/job_logging/custom.yaml
+-rw-r--r--   0        0        0      293 2023-05-05 08:04:32.977784 hyfi-0.3.5/src/hyfi/conf/joblib/__init__.yaml
+-rw-r--r--   0        0        0      701 2023-05-05 08:04:32.977784 hyfi-0.3.5/src/hyfi/conf/mode/__init__.yaml
+-rw-r--r--   0        0        0      231 2023-05-05 08:04:32.977784 hyfi-0.3.5/src/hyfi/conf/mode/debug.yaml
+-rw-r--r--   0        0        0      164 2023-05-05 08:04:32.977784 hyfi-0.3.5/src/hyfi/conf/path/__batch__.yaml
+-rw-r--r--   0        0        0      582 2023-05-05 08:04:32.977784 hyfi-0.3.5/src/hyfi/conf/path/__default__.yaml
+-rw-r--r--   0        0        0      616 2023-05-05 08:04:32.977784 hyfi-0.3.5/src/hyfi/conf/path/__init__.yaml
+-rw-r--r--   0        0        0      360 2023-05-05 08:04:32.977784 hyfi-0.3.5/src/hyfi/conf/project/__init__.yaml
+-rw-r--r--   0        0        0       21 2023-05-05 08:04:32.977784 hyfi-0.3.5/src/hyfi/config/__init__.py
+-rw-r--r--   0        0        0    14151 2023-05-05 08:04:32.977784 hyfi-0.3.5/src/hyfi/config/batch.py
+-rw-r--r--   0        0        0    19819 2023-05-05 08:04:32.977784 hyfi-0.3.5/src/hyfi/env.py
+-rw-r--r--   0        0        0    12903 2023-05-05 08:04:32.977784 hyfi-0.3.5/src/hyfi/hydra.py
+-rw-r--r--   0        0        0        0 2023-05-05 08:04:32.977784 hyfi-0.3.5/src/hyfi/image/__init__.py
+-rw-r--r--   0        0        0     8474 2023-05-05 08:04:32.977784 hyfi-0.3.5/src/hyfi/image/collage.py
+-rw-r--r--   0        0        0     4341 2023-05-05 08:04:32.977784 hyfi-0.3.5/src/hyfi/image/motion.py
+-rw-r--r--   0        0        0     2556 2023-05-05 08:04:32.977784 hyfi-0.3.5/src/hyfi/image/plot.py
+-rw-r--r--   0        0        0     3358 2023-05-05 08:04:32.977784 hyfi-0.3.5/src/hyfi/image/utils.py
+-rw-r--r--   0        0        0        0 2023-05-05 08:04:32.977784 hyfi-0.3.5/src/hyfi/io/__init__.py
+-rw-r--r--   0        0        0     7152 2023-05-05 08:04:32.977784 hyfi-0.3.5/src/hyfi/io/cached_path.py
+-rw-r--r--   0        0        0    12802 2023-05-05 08:04:32.977784 hyfi-0.3.5/src/hyfi/io/file.py
+-rw-r--r--   0        0        0    26828 2023-05-05 08:04:32.977784 hyfi-0.3.5/src/hyfi/main.py
+-rw-r--r--   0        0        0        0 2023-05-05 08:04:32.977784 hyfi-0.3.5/src/hyfi/py.typed
+-rw-r--r--   0        0        0        0 2023-05-05 08:04:32.977784 hyfi-0.3.5/src/hyfi/utils/__init__.py
+-rw-r--r--   0        0        0      111 2023-05-05 08:04:32.977784 hyfi-0.3.5/src/hyfi/utils/batch/__init__.py
+-rw-r--r--   0        0        0     2934 2023-05-05 08:04:32.977784 hyfi-0.3.5/src/hyfi/utils/batch/apply.py
+-rw-r--r--   0        0        0     2046 2023-05-05 08:04:32.977784 hyfi-0.3.5/src/hyfi/utils/batch/apply_batch.py
+-rw-r--r--   0        0        0    17469 2023-05-05 08:04:32.977784 hyfi-0.3.5/src/hyfi/utils/batch/batcher.py
+-rw-r--r--   0        0        0     1206 2023-05-05 08:04:32.977784 hyfi-0.3.5/src/hyfi/utils/cached_path/__init__.py
+-rw-r--r--   0        0        0    14396 2023-05-05 08:04:32.977784 hyfi-0.3.5/src/hyfi/utils/cached_path/_cached_path.py
+-rw-r--r--   0        0        0     1619 2023-05-05 08:04:32.977784 hyfi-0.3.5/src/hyfi/utils/cached_path/cache_file.py
+-rw-r--r--   0        0        0     1110 2023-05-05 08:04:32.977784 hyfi-0.3.5/src/hyfi/utils/cached_path/common.py
+-rw-r--r--   0        0        0     1923 2023-05-05 08:04:32.977784 hyfi-0.3.5/src/hyfi/utils/cached_path/file_lock.py
+-rw-r--r--   0        0        0     3440 2023-05-05 08:04:32.977784 hyfi-0.3.5/src/hyfi/utils/cached_path/meta.py
+-rw-r--r--   0        0        0     3326 2023-05-05 08:04:32.977784 hyfi-0.3.5/src/hyfi/utils/cached_path/progress.py
+-rw-r--r--   0        0        0     1460 2023-05-05 08:04:32.977784 hyfi-0.3.5/src/hyfi/utils/cached_path/schemes/__init__.py
+-rw-r--r--   0        0        0     1815 2023-05-05 08:04:32.977784 hyfi-0.3.5/src/hyfi/utils/cached_path/schemes/beaker.py
+-rw-r--r--   0        0        0     2862 2023-05-05 08:04:32.977784 hyfi-0.3.5/src/hyfi/utils/cached_path/schemes/hf.py
+-rw-r--r--   0        0        0     2999 2023-05-05 08:04:32.977784 hyfi-0.3.5/src/hyfi/utils/cached_path/schemes/http.py
+-rw-r--r--   0        0        0     3645 2023-05-05 08:04:32.977784 hyfi-0.3.5/src/hyfi/utils/cached_path/schemes/scheme_client.py
+-rw-r--r--   0        0        0     1244 2023-05-05 08:04:32.977784 hyfi-0.3.5/src/hyfi/utils/cached_path/testing.py
+-rw-r--r--   0        0        0     4834 2023-05-05 08:04:32.977784 hyfi-0.3.5/src/hyfi/utils/cached_path/util.py
+-rw-r--r--   0        0        0      464 2023-05-05 08:04:32.981784 hyfi-0.3.5/src/hyfi/utils/cached_path/version.py
+-rw-r--r--   0        0        0     6131 2023-05-05 08:04:32.981784 hyfi-0.3.5/src/hyfi/utils/copier.py
+-rw-r--r--   0        0        0     2281 2023-05-05 08:04:32.981784 hyfi-0.3.5/src/hyfi/utils/env.py
+-rw-r--r--   0        0        0    10202 2023-05-05 08:04:32.981784 hyfi-0.3.5/src/hyfi/utils/func.py
+-rw-r--r--   0        0        0     1046 2023-05-05 08:04:32.981784 hyfi-0.3.5/src/hyfi/utils/google.py
+-rw-r--r--   0        0        0     3726 2023-05-05 08:04:32.981784 hyfi-0.3.5/src/hyfi/utils/gpu.py
+-rw-r--r--   0        0        0     5234 2023-05-05 08:04:32.981784 hyfi-0.3.5/src/hyfi/utils/lib.py
+-rw-r--r--   0        0        0     1074 2023-05-05 08:04:32.981784 hyfi-0.3.5/src/hyfi/utils/logging.py
+-rw-r--r--   0        0        0    10003 2023-05-05 08:04:32.981784 hyfi-0.3.5/src/hyfi/utils/notebook.py
+-rw-r--r--   0        0        0     2123 2023-05-05 08:04:32.981784 hyfi-0.3.5/src/hyfi/utils/pipe.py
+-rw-r--r--   0        0        0     5481 2023-05-05 08:04:32.981784 hyfi-0.3.5/src/hyfi/utils/tools.py
+-rw-r--r--   0        0        0      154 2023-05-05 08:04:32.981784 hyfi-0.3.5/src/hyfi/utils/types.py
+-rw-r--r--   0        0        0     2948 1970-01-01 00:00:00.000000 hyfi-0.3.5/PKG-INFO
```

### Comparing `hyfi-0.3.4/LICENSE` & `hyfi-0.3.5/LICENSE`

 * *Files identical despite different names*

### Comparing `hyfi-0.3.4/README.md` & `hyfi-0.3.5/README.md`

 * *Files identical despite different names*

### Comparing `hyfi-0.3.4/pyproject.toml` & `hyfi-0.3.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "hyfi"
-version = "0.3.4"
+version = "0.3.5"
 description = "Hydra Fast Interface (Hydra and Pydantic based interface framework)"
 authors = ["Young Joon Lee <entelecheia@hotmail.com>"]
 license = "MIT"
 homepage = "https://hyfi.entelecheia.ai"
 repository = "https://github.com/entelecheia/hyfi"
 readme = "README.md"
 packages = [{ include = "hyfi", from = "src" }]
```

### Comparing `hyfi-0.3.4/src/hyfi/__cli__.py` & `hyfi-0.3.5/src/hyfi/__cli__.py`

 * *Files identical despite different names*

### Comparing `hyfi-0.3.4/src/hyfi/conf/copier/conf.yaml` & `hyfi-0.3.5/src/hyfi/conf/copier/conf.yaml`

 * *Files identical despite different names*

### Comparing `hyfi-0.3.4/src/hyfi/conf/dotenv/__init__.yaml` & `hyfi-0.3.5/src/hyfi/conf/dotenv/__init__.yaml`

 * *Files identical despite different names*

### Comparing `hyfi-0.3.4/src/hyfi/conf/hydra/help/help.yaml` & `hyfi-0.3.5/src/hyfi/conf/hydra/help/help.yaml`

 * *Files identical despite different names*

### Comparing `hyfi-0.3.4/src/hyfi/conf/mode/__init__.yaml` & `hyfi-0.3.5/src/hyfi/conf/mode/__init__.yaml`

 * *Files identical despite different names*

### Comparing `hyfi-0.3.4/src/hyfi/conf/path/__default__.yaml` & `hyfi-0.3.5/src/hyfi/conf/path/__default__.yaml`

 * *Files identical despite different names*

### Comparing `hyfi-0.3.4/src/hyfi/conf/path/__init__.yaml` & `hyfi-0.3.5/src/hyfi/conf/path/__init__.yaml`

 * *Files identical despite different names*

### Comparing `hyfi-0.3.4/src/hyfi/config/batch.py` & `hyfi-0.3.5/src/hyfi/config/batch.py`

 * *Files identical despite different names*

### Comparing `hyfi-0.3.4/src/hyfi/env.py` & `hyfi-0.3.5/src/hyfi/env.py`

 * *Files identical despite different names*

### Comparing `hyfi-0.3.4/src/hyfi/hydra.py` & `hyfi-0.3.5/src/hyfi/hydra.py`

 * *Files identical despite different names*

### Comparing `hyfi-0.3.4/src/hyfi/image/collage.py` & `hyfi-0.3.5/src/hyfi/image/collage.py`

 * *Files identical despite different names*

### Comparing `hyfi-0.3.4/src/hyfi/image/motion.py` & `hyfi-0.3.5/src/hyfi/image/motion.py`

 * *Files identical despite different names*

### Comparing `hyfi-0.3.4/src/hyfi/image/plot.py` & `hyfi-0.3.5/src/hyfi/image/plot.py`

 * *Files identical despite different names*

### Comparing `hyfi-0.3.4/src/hyfi/image/utils.py` & `hyfi-0.3.5/src/hyfi/image/utils.py`

 * *Files identical despite different names*

### Comparing `hyfi-0.3.4/src/hyfi/io/cached_path.py` & `hyfi-0.3.5/src/hyfi/io/cached_path.py`

 * *Files identical despite different names*

### Comparing `hyfi-0.3.4/src/hyfi/io/file.py` & `hyfi-0.3.5/src/hyfi/io/file.py`

 * *Files identical despite different names*

### Comparing `hyfi-0.3.4/src/hyfi/main.py` & `hyfi-0.3.5/src/hyfi/main.py`

 * *Files identical despite different names*

### Comparing `hyfi-0.3.4/src/hyfi/utils/batch/apply.py` & `hyfi-0.3.5/src/hyfi/utils/batch/apply.py`

 * *Files identical despite different names*

### Comparing `hyfi-0.3.4/src/hyfi/utils/batch/apply_batch.py` & `hyfi-0.3.5/src/hyfi/utils/batch/apply_batch.py`

 * *Files identical despite different names*

### Comparing `hyfi-0.3.4/src/hyfi/utils/batch/batcher.py` & `hyfi-0.3.5/src/hyfi/utils/batch/batcher.py`

 * *Files identical despite different names*

### Comparing `hyfi-0.3.4/src/hyfi/utils/cached_path/__init__.py` & `hyfi-0.3.5/src/hyfi/utils/cached_path/__init__.py`

 * *Files identical despite different names*

### Comparing `hyfi-0.3.4/src/hyfi/utils/cached_path/_cached_path.py` & `hyfi-0.3.5/src/hyfi/utils/cached_path/_cached_path.py`

 * *Files identical despite different names*

### Comparing `hyfi-0.3.4/src/hyfi/utils/cached_path/cache_file.py` & `hyfi-0.3.5/src/hyfi/utils/cached_path/cache_file.py`

 * *Files identical despite different names*

### Comparing `hyfi-0.3.4/src/hyfi/utils/cached_path/common.py` & `hyfi-0.3.5/src/hyfi/utils/cached_path/common.py`

 * *Files identical despite different names*

### Comparing `hyfi-0.3.4/src/hyfi/utils/cached_path/file_lock.py` & `hyfi-0.3.5/src/hyfi/utils/cached_path/file_lock.py`

 * *Files identical despite different names*

### Comparing `hyfi-0.3.4/src/hyfi/utils/cached_path/meta.py` & `hyfi-0.3.5/src/hyfi/utils/cached_path/meta.py`

 * *Files identical despite different names*

### Comparing `hyfi-0.3.4/src/hyfi/utils/cached_path/progress.py` & `hyfi-0.3.5/src/hyfi/utils/cached_path/progress.py`

 * *Files identical despite different names*

### Comparing `hyfi-0.3.4/src/hyfi/utils/cached_path/schemes/__init__.py` & `hyfi-0.3.5/src/hyfi/utils/cached_path/schemes/__init__.py`

 * *Files identical despite different names*

### Comparing `hyfi-0.3.4/src/hyfi/utils/cached_path/schemes/beaker.py` & `hyfi-0.3.5/src/hyfi/utils/cached_path/schemes/beaker.py`

 * *Files identical despite different names*

### Comparing `hyfi-0.3.4/src/hyfi/utils/cached_path/schemes/hf.py` & `hyfi-0.3.5/src/hyfi/utils/cached_path/schemes/hf.py`

 * *Files identical despite different names*

### Comparing `hyfi-0.3.4/src/hyfi/utils/cached_path/schemes/http.py` & `hyfi-0.3.5/src/hyfi/utils/cached_path/schemes/http.py`

 * *Files identical despite different names*

### Comparing `hyfi-0.3.4/src/hyfi/utils/cached_path/schemes/scheme_client.py` & `hyfi-0.3.5/src/hyfi/utils/cached_path/schemes/scheme_client.py`

 * *Files identical despite different names*

### Comparing `hyfi-0.3.4/src/hyfi/utils/cached_path/testing.py` & `hyfi-0.3.5/src/hyfi/utils/cached_path/testing.py`

 * *Files identical despite different names*

### Comparing `hyfi-0.3.4/src/hyfi/utils/cached_path/util.py` & `hyfi-0.3.5/src/hyfi/utils/cached_path/util.py`

 * *Files identical despite different names*

### Comparing `hyfi-0.3.4/src/hyfi/utils/copier.py` & `hyfi-0.3.5/src/hyfi/utils/copier.py`

 * *Files identical despite different names*

### Comparing `hyfi-0.3.4/src/hyfi/utils/env.py` & `hyfi-0.3.5/src/hyfi/utils/env.py`

 * *Files identical despite different names*

### Comparing `hyfi-0.3.4/src/hyfi/utils/func.py` & `hyfi-0.3.5/src/hyfi/utils/func.py`

 * *Files identical despite different names*

### Comparing `hyfi-0.3.4/src/hyfi/utils/google.py` & `hyfi-0.3.5/src/hyfi/utils/google.py`

 * *Files identical despite different names*

### Comparing `hyfi-0.3.4/src/hyfi/utils/gpu.py` & `hyfi-0.3.5/src/hyfi/utils/gpu.py`

 * *Files identical despite different names*

### Comparing `hyfi-0.3.4/src/hyfi/utils/lib.py` & `hyfi-0.3.5/src/hyfi/utils/lib.py`

 * *Files identical despite different names*

### Comparing `hyfi-0.3.4/src/hyfi/utils/logging.py` & `hyfi-0.3.5/src/hyfi/utils/logging.py`

 * *Files identical despite different names*

### Comparing `hyfi-0.3.4/src/hyfi/utils/notebook.py` & `hyfi-0.3.5/src/hyfi/utils/notebook.py`

 * *Files identical despite different names*

### Comparing `hyfi-0.3.4/src/hyfi/utils/pipe.py` & `hyfi-0.3.5/src/hyfi/utils/pipe.py`

 * *Files identical despite different names*

### Comparing `hyfi-0.3.4/src/hyfi/utils/tools.py` & `hyfi-0.3.5/src/hyfi/utils/tools.py`

 * *Files identical despite different names*

### Comparing `hyfi-0.3.4/PKG-INFO` & `hyfi-0.3.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: hyfi
-Version: 0.3.4
+Version: 0.3.5
 Summary: Hydra Fast Interface (Hydra and Pydantic based interface framework)
 Home-page: https://hyfi.entelecheia.ai
 License: MIT
 Author: Young Joon Lee
 Author-email: entelecheia@hotmail.com
 Requires-Python: >=3.8.1,<3.12
 Classifier: License :: OSI Approved :: MIT License
```

