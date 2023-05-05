# Comparing `tmp/hyfi-0.2.9.tar.gz` & `tmp/hyfi-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hyfi-0.2.9.tar", max compression
+gzip compressed data, was "hyfi-0.3.0.tar", max compression
```

## Comparing `hyfi-0.2.9.tar` & `hyfi-0.3.0.tar`

### file list

```diff
@@ -1,51 +1,54 @@
--rw-r--r--   0        0        0     1071 2023-04-21 11:02:36.885051 hyfi-0.2.9/LICENSE
--rw-r--r--   0        0        0     1949 2023-04-21 11:02:36.885051 hyfi-0.2.9/README.md
--rw-r--r--   0        0        0     3946 2023-04-21 11:03:10.591819 hyfi-0.2.9/pyproject.toml
--rw-r--r--   0        0        0     1700 2023-04-21 11:02:36.889051 hyfi-0.2.9/src/hyfi/__cli__.py
--rw-r--r--   0        0        0      331 2023-04-21 11:02:36.889051 hyfi-0.2.9/src/hyfi/__init__.py
--rw-r--r--   0        0        0       35 2023-04-21 11:03:10.523814 hyfi-0.2.9/src/hyfi/_version.py
--rw-r--r--   0        0        0        0 2023-04-21 11:02:36.889051 hyfi-0.2.9/src/hyfi/conf/__init__.py
--rw-r--r--   0        0        0      170 2023-04-21 11:02:36.889051 hyfi-0.2.9/src/hyfi/conf/about/__init__.yaml
--rw-r--r--   0        0        0      331 2023-04-21 11:02:36.889051 hyfi-0.2.9/src/hyfi/conf/batch/__init__.yaml
--rw-r--r--   0        0        0      506 2023-04-21 11:02:36.889051 hyfi-0.2.9/src/hyfi/conf/config.yaml
--rw-r--r--   0        0        0      789 2023-04-21 11:02:36.889051 hyfi-0.2.9/src/hyfi/conf/dotenv/__init__.yaml
--rw-r--r--   0        0        0      502 2023-04-21 11:02:36.889051 hyfi-0.2.9/src/hyfi/conf/hconf.yaml
--rw-r--r--   0        0        0     1126 2023-04-21 11:02:36.889051 hyfi-0.2.9/src/hyfi/conf/hydra/help/help.yaml
--rw-r--r--   0        0        0      264 2023-04-21 11:02:36.889051 hyfi-0.2.9/src/hyfi/conf/hydra/job_logging/custom.yaml
--rw-r--r--   0        0        0      295 2023-04-21 11:02:36.889051 hyfi-0.2.9/src/hyfi/conf/joblib/__init__.yaml
--rw-r--r--   0        0        0      701 2023-04-21 11:02:36.889051 hyfi-0.2.9/src/hyfi/conf/mode/__init__.yaml
--rw-r--r--   0        0        0      231 2023-04-21 11:02:36.889051 hyfi-0.2.9/src/hyfi/conf/mode/debug.yaml
--rw-r--r--   0        0        0      164 2023-04-21 11:02:36.889051 hyfi-0.2.9/src/hyfi/conf/path/__batch__.yaml
--rw-r--r--   0        0        0      582 2023-04-21 11:02:36.889051 hyfi-0.2.9/src/hyfi/conf/path/__default__.yaml
--rw-r--r--   0        0        0      616 2023-04-21 11:02:36.889051 hyfi-0.2.9/src/hyfi/conf/path/__init__.yaml
--rw-r--r--   0        0        0      360 2023-04-21 11:02:36.889051 hyfi-0.2.9/src/hyfi/conf/project/__init__.yaml
--rw-r--r--   0        0        0       79 2023-04-21 11:02:36.889051 hyfi-0.2.9/src/hyfi/conf/task/__init__.yaml
--rw-r--r--   0        0        0       21 2023-04-21 11:02:36.889051 hyfi-0.2.9/src/hyfi/config/__init__.py
--rw-r--r--   0        0        0    14151 2023-04-21 11:02:36.889051 hyfi-0.2.9/src/hyfi/config/batch.py
--rw-r--r--   0        0        0    19380 2023-04-21 11:02:36.889051 hyfi-0.2.9/src/hyfi/env.py
--rw-r--r--   0        0        0    12911 2023-04-21 11:02:36.889051 hyfi-0.2.9/src/hyfi/hydra.py
--rw-r--r--   0        0        0        0 2023-04-21 11:02:36.889051 hyfi-0.2.9/src/hyfi/image/__init__.py
--rw-r--r--   0        0        0     8474 2023-04-21 11:02:36.889051 hyfi-0.2.9/src/hyfi/image/collage.py
--rw-r--r--   0        0        0     4341 2023-04-21 11:02:36.889051 hyfi-0.2.9/src/hyfi/image/motion.py
--rw-r--r--   0        0        0     2556 2023-04-21 11:02:36.889051 hyfi-0.2.9/src/hyfi/image/plot.py
--rw-r--r--   0        0        0     3358 2023-04-21 11:02:36.889051 hyfi-0.2.9/src/hyfi/image/utils.py
--rw-r--r--   0        0        0        0 2023-04-21 11:02:36.889051 hyfi-0.2.9/src/hyfi/io/__init__.py
--rw-r--r--   0        0        0     5625 2023-04-21 11:02:36.889051 hyfi-0.2.9/src/hyfi/io/cached_path.py
--rw-r--r--   0        0        0    12802 2023-04-21 11:02:36.889051 hyfi-0.2.9/src/hyfi/io/file.py
--rw-r--r--   0        0        0    26361 2023-04-21 11:02:36.889051 hyfi-0.2.9/src/hyfi/main.py
--rw-r--r--   0        0        0     2134 2023-04-21 11:02:36.889051 hyfi-0.2.9/src/hyfi/pipe.py
--rw-r--r--   0        0        0      221 2023-04-21 11:02:36.889051 hyfi-0.2.9/src/hyfi/project.toml
--rw-r--r--   0        0        0        0 2023-04-21 11:02:36.889051 hyfi-0.2.9/src/hyfi/py.typed
--rw-r--r--   0        0        0        0 2023-04-21 11:02:36.893051 hyfi-0.2.9/src/hyfi/utils/__init__.py
--rw-r--r--   0        0        0      111 2023-04-21 11:02:36.893051 hyfi-0.2.9/src/hyfi/utils/batch/__init__.py
--rw-r--r--   0        0        0     2934 2023-04-21 11:02:36.893051 hyfi-0.2.9/src/hyfi/utils/batch/apply.py
--rw-r--r--   0        0        0     2046 2023-04-21 11:02:36.893051 hyfi-0.2.9/src/hyfi/utils/batch/apply_batch.py
--rw-r--r--   0        0        0    17469 2023-04-21 11:02:36.893051 hyfi-0.2.9/src/hyfi/utils/batch/batcher.py
--rw-r--r--   0        0        0     2281 2023-04-21 11:02:36.893051 hyfi-0.2.9/src/hyfi/utils/env.py
--rw-r--r--   0        0        0    10202 2023-04-21 11:02:36.893051 hyfi-0.2.9/src/hyfi/utils/func.py
--rw-r--r--   0        0        0     1046 2023-04-21 11:02:36.893051 hyfi-0.2.9/src/hyfi/utils/google.py
--rw-r--r--   0        0        0     3726 2023-04-21 11:02:36.893051 hyfi-0.2.9/src/hyfi/utils/gpu.py
--rw-r--r--   0        0        0     5234 2023-04-21 11:02:36.893051 hyfi-0.2.9/src/hyfi/utils/lib.py
--rw-r--r--   0        0        0     1074 2023-04-21 11:02:36.893051 hyfi-0.2.9/src/hyfi/utils/logging.py
--rw-r--r--   0        0        0    10003 2023-04-21 11:02:36.893051 hyfi-0.2.9/src/hyfi/utils/notebook.py
--rw-r--r--   0        0        0     3248 1970-01-01 00:00:00.000000 hyfi-0.2.9/PKG-INFO
+-rw-r--r--   0        0        0     1071 2023-05-05 00:43:33.833856 hyfi-0.3.0/LICENSE
+-rw-r--r--   0        0        0     1949 2023-05-05 00:43:33.833856 hyfi-0.3.0/README.md
+-rw-r--r--   0        0        0     4056 2023-05-05 00:44:07.426452 hyfi-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0     2680 2023-05-05 00:43:33.837856 hyfi-0.3.0/src/hyfi/__cli__.py
+-rw-r--r--   0        0        0      331 2023-05-05 00:43:33.837856 hyfi-0.3.0/src/hyfi/__init__.py
+-rw-r--r--   0        0        0       22 2023-05-05 00:44:07.370451 hyfi-0.3.0/src/hyfi/_version.py
+-rw-r--r--   0        0        0        0 2023-05-05 00:43:33.837856 hyfi-0.3.0/src/hyfi/conf/__init__.py
+-rw-r--r--   0        0        0      233 2023-05-05 00:44:07.370451 hyfi-0.3.0/src/hyfi/conf/about/__init__.yaml
+-rw-r--r--   0        0        0      331 2023-05-05 00:43:33.837856 hyfi-0.3.0/src/hyfi/conf/batch/__init__.yaml
+-rw-r--r--   0        0        0       83 2023-05-05 00:43:33.837856 hyfi-0.3.0/src/hyfi/conf/cmd/about.yaml
+-rw-r--r--   0        0        0      167 2023-05-05 00:43:33.837856 hyfi-0.3.0/src/hyfi/conf/cmd/cpcfg.yaml
+-rw-r--r--   0        0        0      320 2023-05-05 00:43:33.837856 hyfi-0.3.0/src/hyfi/conf/config.yaml
+-rw-r--r--   0        0        0      496 2023-05-05 00:43:33.837856 hyfi-0.3.0/src/hyfi/conf/copier/conf.yaml
+-rw-r--r--   0        0        0      789 2023-05-05 00:43:33.837856 hyfi-0.3.0/src/hyfi/conf/dotenv/__init__.yaml
+-rw-r--r--   0        0        0      319 2023-05-05 00:43:33.837856 hyfi-0.3.0/src/hyfi/conf/hconf.yaml
+-rw-r--r--   0        0        0     1128 2023-05-05 00:43:33.837856 hyfi-0.3.0/src/hyfi/conf/hydra/help/help.yaml
+-rw-r--r--   0        0        0      264 2023-05-05 00:43:33.837856 hyfi-0.3.0/src/hyfi/conf/hydra/job_logging/custom.yaml
+-rw-r--r--   0        0        0      293 2023-05-05 00:43:33.837856 hyfi-0.3.0/src/hyfi/conf/joblib/__init__.yaml
+-rw-r--r--   0        0        0      701 2023-05-05 00:43:33.837856 hyfi-0.3.0/src/hyfi/conf/mode/__init__.yaml
+-rw-r--r--   0        0        0      231 2023-05-05 00:43:33.837856 hyfi-0.3.0/src/hyfi/conf/mode/debug.yaml
+-rw-r--r--   0        0        0      164 2023-05-05 00:43:33.837856 hyfi-0.3.0/src/hyfi/conf/path/__batch__.yaml
+-rw-r--r--   0        0        0      582 2023-05-05 00:43:33.837856 hyfi-0.3.0/src/hyfi/conf/path/__default__.yaml
+-rw-r--r--   0        0        0      616 2023-05-05 00:43:33.837856 hyfi-0.3.0/src/hyfi/conf/path/__init__.yaml
+-rw-r--r--   0        0        0      360 2023-05-05 00:43:33.837856 hyfi-0.3.0/src/hyfi/conf/project/__init__.yaml
+-rw-r--r--   0        0        0       21 2023-05-05 00:43:33.837856 hyfi-0.3.0/src/hyfi/config/__init__.py
+-rw-r--r--   0        0        0    14151 2023-05-05 00:43:33.837856 hyfi-0.3.0/src/hyfi/config/batch.py
+-rw-r--r--   0        0        0    19819 2023-05-05 00:43:33.837856 hyfi-0.3.0/src/hyfi/env.py
+-rw-r--r--   0        0        0    12903 2023-05-05 00:43:33.837856 hyfi-0.3.0/src/hyfi/hydra.py
+-rw-r--r--   0        0        0        0 2023-05-05 00:43:33.837856 hyfi-0.3.0/src/hyfi/image/__init__.py
+-rw-r--r--   0        0        0     8474 2023-05-05 00:43:33.837856 hyfi-0.3.0/src/hyfi/image/collage.py
+-rw-r--r--   0        0        0     4341 2023-05-05 00:43:33.837856 hyfi-0.3.0/src/hyfi/image/motion.py
+-rw-r--r--   0        0        0     2556 2023-05-05 00:43:33.837856 hyfi-0.3.0/src/hyfi/image/plot.py
+-rw-r--r--   0        0        0     3358 2023-05-05 00:43:33.837856 hyfi-0.3.0/src/hyfi/image/utils.py
+-rw-r--r--   0        0        0        0 2023-05-05 00:43:33.837856 hyfi-0.3.0/src/hyfi/io/__init__.py
+-rw-r--r--   0        0        0     5625 2023-05-05 00:43:33.837856 hyfi-0.3.0/src/hyfi/io/cached_path.py
+-rw-r--r--   0        0        0    12802 2023-05-05 00:43:33.837856 hyfi-0.3.0/src/hyfi/io/file.py
+-rw-r--r--   0        0        0    26828 2023-05-05 00:43:33.837856 hyfi-0.3.0/src/hyfi/main.py
+-rw-r--r--   0        0        0        0 2023-05-05 00:43:33.837856 hyfi-0.3.0/src/hyfi/py.typed
+-rw-r--r--   0        0        0        0 2023-05-05 00:43:33.837856 hyfi-0.3.0/src/hyfi/utils/__init__.py
+-rw-r--r--   0        0        0      111 2023-05-05 00:43:33.837856 hyfi-0.3.0/src/hyfi/utils/batch/__init__.py
+-rw-r--r--   0        0        0     2934 2023-05-05 00:43:33.837856 hyfi-0.3.0/src/hyfi/utils/batch/apply.py
+-rw-r--r--   0        0        0     2046 2023-05-05 00:43:33.837856 hyfi-0.3.0/src/hyfi/utils/batch/apply_batch.py
+-rw-r--r--   0        0        0    17469 2023-05-05 00:43:33.837856 hyfi-0.3.0/src/hyfi/utils/batch/batcher.py
+-rw-r--r--   0        0        0     5651 2023-05-05 00:43:33.837856 hyfi-0.3.0/src/hyfi/utils/copier.py
+-rw-r--r--   0        0        0     2281 2023-05-05 00:43:33.837856 hyfi-0.3.0/src/hyfi/utils/env.py
+-rw-r--r--   0        0        0    10202 2023-05-05 00:43:33.837856 hyfi-0.3.0/src/hyfi/utils/func.py
+-rw-r--r--   0        0        0     1046 2023-05-05 00:43:33.837856 hyfi-0.3.0/src/hyfi/utils/google.py
+-rw-r--r--   0        0        0     3726 2023-05-05 00:43:33.837856 hyfi-0.3.0/src/hyfi/utils/gpu.py
+-rw-r--r--   0        0        0     5234 2023-05-05 00:43:33.837856 hyfi-0.3.0/src/hyfi/utils/lib.py
+-rw-r--r--   0        0        0     1074 2023-05-05 00:43:33.837856 hyfi-0.3.0/src/hyfi/utils/logging.py
+-rw-r--r--   0        0        0    10003 2023-05-05 00:43:33.837856 hyfi-0.3.0/src/hyfi/utils/notebook.py
+-rw-r--r--   0        0        0     2123 2023-05-05 00:43:33.837856 hyfi-0.3.0/src/hyfi/utils/pipe.py
+-rw-r--r--   0        0        0     5504 2023-05-05 00:43:33.837856 hyfi-0.3.0/src/hyfi/utils/tools.py
+-rw-r--r--   0        0        0     3391 1970-01-01 00:00:00.000000 hyfi-0.3.0/PKG-INFO
```

### Comparing `hyfi-0.2.9/LICENSE` & `hyfi-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `hyfi-0.2.9/README.md` & `hyfi-0.3.0/README.md`

 * *Files identical despite different names*

### Comparing `hyfi-0.2.9/pyproject.toml` & `hyfi-0.3.0/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,55 +1,58 @@
 [tool.poetry]
 name = "hyfi"
-version = "0.2.9"
+version = "0.3.0"
 description = "Hydra Fast Interface (Hydra and Pydantic based interface framework)"
 authors = ["Young Joon Lee <entelecheia@hotmail.com>"]
 license = "MIT"
+homepage = "https://hyfi.entelecheia.ai"
+repository = "https://github.com/entelecheia/hyfi"
 readme = "README.md"
 packages = [{ include = "hyfi", from = "src" }]
 
 [tool.poetry.scripts]
 hyfi = 'hyfi.__cli__:hydra_main'
 
 [tool.poetry.dependencies]
 python = "^3.8.1, <3.12"
 hydra-core = "^1.3.2"
 hydra-colorlog = "^1.2.0"
 pydantic = "^1.10.7"
-chardet = "<=4.0.0"
+chardet = "<=5.1.0"
 pandas = "^1.5.3"
 scipy = "^1.10.1"
 matplotlib = "^3.7.1"
 numpy = "<1.24"
 python-dotenv = "^1.0.0"
 gdown = "^4.6.6"
 requests = "^2.27.1"
 tqdm = "^4.64.1"
 cached-path = "^1.3.3"
+colorama = "^0.4.3"
 
 # A list of all of the optional dependencies, some of which are included in the
 # below `extras`. They can be opted into by apps.
-ipython = { version = "<=7.9.0", optional = true }
+ipython = { version = "<=8.12.0", optional = true }
 ipython-autotime = { version = "^0.3.1", optional = true }
 rich = { version = ">=11.1", optional = true }
-pygments = { version = "<=2.6.1", optional = true }
+pygments = { version = "<=2.15.1", optional = true }
 
 [tool.poetry.extras]
 ipython = ["ipython", "ipython-autotime", "rich", "pygments"]
 
 [tool.poetry.group.dev.dependencies]
 python-semantic-release = "^7.33.1"
-setuptools-scm = "^7.1.0"
 isort = "^5.12.0"
 black = "^23.1.0"
 flake8 = "^6.0.0"
 mypy = "^1.0.0"
 flake8-pyproject = "^1.2.2"
 pytest = "^7.2.1"
 pytest-cov = "^4.0.0"
+ipykernel = "^6.22.0"
 
 [tool.black]
 exclude = [
     '_version.py',
     'node_modules',
     '_build',
     'docs',
@@ -139,31 +142,30 @@
 
 [tool.commitizen]
 name = "cz_conventional_commits"
 version = "1.0.1"
 tag_format = "v$version"
 
 [tool.setuptools_scm]
-write_to = "src/hyfi/_version.py"
 write_to_template = '__version__ = "{version}"'
 tag_regex = '^(?P<prefix>v)?(?P<version>[^\+]+)(?P<suffix>.*)?$'
 
 [tool.semantic_release]
 branch = "main"
 version_variable = "src/hyfi/_version.py:__version__"
 version_toml = "pyproject.toml:tool.poetry.version"
+version_pattern = 'src/hyfi/conf/about/__init__.yaml:version: "{version}"'
 version_source = "tag"
-commit_version_number = true                                    # required for version_source = "tag"
+commit_version_number = true                                               # required for version_source = "tag"
 commit_subject = "chore(release): :rocket: {version} [skip ci]"
 prerelease_tag = "rc"
 major_on_zero = true
 tag_commit = true
-pre_commit_command = "make scm-version"
 changelog_file = "CHANGELOG.md"
 upload_to_repository = true
 upload_to_release = true
 build_command = "poetry build --no-cache"
-hvcs = "github"                                                 # hosting version control system, gitlab is also supported
+hvcs = "github"                                                            # hosting version control system, gitlab is also supported
 
 [build-system]
-requires = ["setuptools>=45", "setuptools_scm[toml]>=6.2"]
-build-backend = 'setuptools.build_meta'
+requires = ["poetry-core>=1.0.0"]
+build-backend = "poetry.core.masonry.api"
```

### Comparing `hyfi-0.2.9/src/hyfi/__cli__.py` & `hyfi-0.3.0/src/hyfi/__cli__.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,31 +1,40 @@
 """Command line interface for HyFI"""
 import os
+from typing import Optional
 
 import hydra
 
-from .env import HyfiConfig, __hydra_version_base__
-from .main import DictConfig, HyFI, getLogger
+from .env import HyfiConfig, __about__, __hydra_version_base__
+from .main import DictConfig, HyFI, _about, getLogger
+from .utils.copier import Copier
 
 logger = getLogger(__name__)
 
 
+__config_path__ = "conf"
+__config_name__ = "config"
+
+
 def cmd(**args):
     """Run the command defined in the config file"""
     HyFI.run(args)
 
 
 def about(**args):
     """Print the about information"""
     cfg = HyfiConfig(**args)
-    name = cfg.about.name
-    print()
-    for k, v in cfg.about.dict().items():
-        print(f"{k:11} : {v}")
-    print(f"\nExecute `{name} --help` to see what you can do with {name}")
+    _about(cfg)
+
+
+def run_copy(**args):
+    """Copy all config files in the config directory to the current working directory"""
+    cfg = HyfiConfig(**args)
+    with Copier(**cfg.copier) as worker:
+        worker.run_copy()
 
 
 def cli_main(cfg: DictConfig) -> None:
     """Main function for the command line interface"""
     hyfi = HyfiConfig(**cfg)
     verbose = hyfi.verbose
     app_name = hyfi.about.name
@@ -49,17 +58,33 @@
         logger.info(f"Orig working directory  : {hydra.utils.get_original_cwd()}")
 
     HyFI.instantiate(cfg)
 
     HyFI.terminate()
 
 
-def hydra_main() -> None:
-    """Main function for the command line interface of Hydra"""
+def hydra_main(
+    config_path: Optional[str] = __config_path__,
+    config_name: Optional[str] = __config_name__,
+) -> None:
+    """
+    Main function for the command line interface of Hydra
+    :param config_path: The config path, a directory where Hydra will search for
+                        config files. This path is added to Hydra's searchpath.
+                        Relative paths are interpreted relative to the declaring python
+                        file. Alternatively, you can use the prefix `pkg://` to specify
+                        a python package to add to the searchpath.
+                        If config_path is None no directory is added to the Config search path.
+    :param config_name: The name of the config (usually the file name without the .yaml extension)
+    """
+    if config_path is None:
+        config_path = __about__.config_path
     hydra.main(
-        config_path="conf", config_name="config", version_base=__hydra_version_base__
+        config_path=config_path,
+        config_name=config_name,
+        version_base=__hydra_version_base__,
     )(cli_main)()
 
 
 if __name__ == "__main__":
     """Run the command line interface"""
     hydra_main()
```

### Comparing `hyfi-0.2.9/src/hyfi/conf/dotenv/__init__.yaml` & `hyfi-0.3.0/src/hyfi/conf/dotenv/__init__.yaml`

 * *Files identical despite different names*

### Comparing `hyfi-0.2.9/src/hyfi/conf/hydra/help/help.yaml` & `hyfi-0.3.0/src/hyfi/conf/hydra/help/help.yaml`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 #
 # Configuration generated with overrides:
 #   $CONFIG : Generated config
 #
 template: |-
   ${hydra.help.header} 
   
-  author: ${about.author}
+  authors: ${about.authors}
   description: ${about.description}
 
   ${hydra.help.app_name} Command Line Interface for Hydra
 
   == Configuration groups ==
 
   Compose your configuration from those groups (task=task_name)
```

### Comparing `hyfi-0.2.9/src/hyfi/conf/mode/__init__.yaml` & `hyfi-0.3.0/src/hyfi/conf/mode/__init__.yaml`

 * *Files identical despite different names*

### Comparing `hyfi-0.2.9/src/hyfi/conf/path/__default__.yaml` & `hyfi-0.3.0/src/hyfi/conf/path/__default__.yaml`

 * *Files identical despite different names*

### Comparing `hyfi-0.2.9/src/hyfi/conf/path/__init__.yaml` & `hyfi-0.3.0/src/hyfi/conf/path/__init__.yaml`

 * *Files identical despite different names*

### Comparing `hyfi-0.2.9/src/hyfi/config/batch.py` & `hyfi-0.3.0/src/hyfi/config/batch.py`

 * *Files identical despite different names*

### Comparing `hyfi-0.2.9/src/hyfi/env.py` & `hyfi-0.3.0/src/hyfi/env.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,14 @@
 from .utils.env import load_dotenv
 from .utils.logging import getLogger, setLogger
 from .utils.notebook import is_notebook, load_extentions, set_matplotlib_formats
 
 logger = getLogger(__name__)
 
 __hydra_version_base__ = "1.2"
-__config_module__ = "hyfi.conf"
 
 
 def __version__():
     """Returns the version of HyFI"""
     from ._version import __version__
 
     return __version__
@@ -63,21 +62,35 @@
 ):
     return OmegaConf.create(cfg)
 
 
 class AboutConfig(BaseModel):
     """About Configuration"""
 
+    __package_name__: str = "hyfi"
     name: str = "HyFI"
-    author: str = "Young Joon Lee"
+    authors: str = "Young Joon Lee <entelecheia@hotmail.com>"
     description: str = (
         "Hydra Fast Interface (Hydra and Pydantic based interface framework)"
     )
     homepage: str = "https://hyfi.entelecheia.ai"
-    version: str = __version__()
+    license: str = "MIT"
+    version: str = "0.0.0"
+
+    class Config:
+        extra = "allow"
+        underscore_attrs_are_private = False
+
+    @property
+    def config_module(self) -> str:
+        return f"{self.__package_name__}.conf"
+
+    @property
+    def config_path(self) -> str:
+        return f"pkg://{self.config_module}"
 
 
 __about__ = AboutConfig()
 
 
 class DistFramwork(BaseModel):
     """Distributed Framework Configuration"""
@@ -112,15 +125,17 @@
 
     def __init__(
         self,
         config_name: str = "__init__",
         **data: Any,
     ):
         if not data:
-            data = _compose(f"joblib={config_name}", config_module=__config_module__)
+            data = _compose(
+                f"joblib={config_name}", config_module=__about__.config_module
+            )
             logger.debug(
                 "There are no arguments to initilize a config, using default config."
             )
         super().__init__(config_name=config_name, **data)
 
     def init_backend(
         self,
@@ -203,15 +218,17 @@
 
     def __init__(
         self,
         config_name: str = "__init__",
         **data: Any,
     ):
         if not data:
-            data = _compose(f"path={config_name}", config_module=__config_module__)
+            data = _compose(
+                f"path={config_name}", config_module=__about__.config_module
+            )
             logger.debug(
                 "There are no arguments to initilize a config, using default config."
             )
         super().__init__(config_name=config_name, **data)
 
     @property
     def log_dir(self):
@@ -316,15 +333,17 @@
 
     def __init__(
         self,
         config_name: str = "__init__",
         **data: Any,
     ):
         if not data:
-            data = _compose(f"project={config_name}", config_module=__config_module__)
+            data = _compose(
+                f"project={config_name}", config_module=__about__.config_module
+            )
             logger.debug(
                 "There are no arguments to initilize a config, using default config."
             )
         super().__init__(config_name=config_name, **data)
 
     @validator("project_name", allow_reuse=True)
     def _validate_project_name(cls, v):
@@ -415,16 +434,16 @@
             logger.debug("Set environment variable %s=%s", env_key, str(value))
     return value
 
 
 class HyfiConfig(BaseModel):
     """HyFI config primary class"""
 
-    hyfi_package_config_path: str = "pkg://hyfi.conf"
-    hyfi_config_module: str = __config_module__
+    hyfi_config_path: str = __about__.config_path
+    hyfi_config_module: str = __about__.config_module
     hyfi_user_config_path: str = None
 
     debug_mode: bool = False
     print_config: bool = False
     print_resolved_config: bool = False
     verbose: bool = False
     logging_level: str = "WARNING"
@@ -441,15 +460,15 @@
         arbitrary_types_allowed = True
         underscore_attrs_are_private = True
         validate_assignment = True
         extra = "allow"
 
     @root_validator()
     def _check_and_set_values(cls, values):
-        key = "hyfi_package_config_path"
+        key = "hyfi_config_path"
         val = _check_and_set_value(key, values.get(key))
         values[key] = val
         if val is not None:
             key = "hyfi_config_module"
             values[key] = _check_and_set_value(key, val.replace("pkg://", ""))
         return values
 
@@ -463,15 +482,15 @@
         if verbose and v == "WARNING":
             v = "INFO"
         logger.setLevel(v)
         return v
 
     def __init__(self, **data: Any):
         super().__init__(**data)
-        self.about = __about__
+        # self.about = __about__
 
     def init_workspace(
         self,
         workspace=None,
         project=None,
         task=None,
         log_level=None,
@@ -500,15 +519,15 @@
 
     def initialize(self, config: Union[DictConfig, Dict] = None):
         """Initialize hyfi config"""
         if self.__initilized__:
             return
         if config is None:
             config = _compose(
-                overrides=["+project=__init__"], config_module=__config_module__
+                overrides=["+project=__init__"], config_module=__about__.config_module
             )
             logger.debug("Using default config.")
 
         if "project" not in config:
             logger.warning(
                 "No project config found, skip project config initialization."
             )
```

### Comparing `hyfi-0.2.9/src/hyfi/hydra.py` & `hyfi-0.3.0/src/hyfi/hydra.py`

 * *Files 0% similar despite different names*

```diff
@@ -326,15 +326,15 @@
 
 
 def __home_path__():
     return Path.home().as_posix()
 
 
 def __search_package_path__():
-    return __global_config__.hyfi_package_config_path
+    return __global_config__.hyfi_config_path
 
 
 OmegaConf.register_new_resolver("__hyfi_path__", __hyfi_path__)
 OmegaConf.register_new_resolver("__search_package_path__", __search_package_path__)
 OmegaConf.register_new_resolver("__home_path__", __home_path__)
 OmegaConf.register_new_resolver("today", today)
 OmegaConf.register_new_resolver("to_datetime", strptime)
```

### Comparing `hyfi-0.2.9/src/hyfi/image/collage.py` & `hyfi-0.3.0/src/hyfi/image/collage.py`

 * *Files identical despite different names*

### Comparing `hyfi-0.2.9/src/hyfi/image/motion.py` & `hyfi-0.3.0/src/hyfi/image/motion.py`

 * *Files identical despite different names*

### Comparing `hyfi-0.2.9/src/hyfi/image/plot.py` & `hyfi-0.3.0/src/hyfi/image/plot.py`

 * *Files identical despite different names*

### Comparing `hyfi-0.2.9/src/hyfi/image/utils.py` & `hyfi-0.3.0/src/hyfi/image/utils.py`

 * *Files identical despite different names*

### Comparing `hyfi-0.2.9/src/hyfi/io/cached_path.py` & `hyfi-0.3.0/src/hyfi/io/cached_path.py`

 * *Files identical despite different names*

### Comparing `hyfi-0.2.9/src/hyfi/io/file.py` & `hyfi-0.3.0/src/hyfi/io/file.py`

 * *Files identical despite different names*

### Comparing `hyfi-0.2.9/src/hyfi/main.py` & `hyfi-0.3.0/src/hyfi/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -32,15 +32,15 @@
     _to_dict,
     _to_yaml,
     _update,
     _viewsource,
 )
 from .io.cached_path import cached_path
 from .io.file import exists, is_dir, is_file, join_path, mkdir
-from .pipe import _apply, _pipe
+from .utils.pipe import _apply, _pipe
 from .utils.env import get_osenv, load_dotenv, set_osenv
 from .utils.func import (
     dict_product,
     dict_to_dataframe,
     records_to_dataframe,
     to_dateparm,
     to_datetime,
@@ -66,27 +66,45 @@
     is_colab,
     is_notebook,
 )
 
 logger = getLogger(__name__)
 
 
+def _about(cfg):
+    pkg_name = cfg.about.__package_name__
+    name = cfg.about.name
+    print()
+    for k, v in cfg.about.dict().items():
+        if k.startswith("_"):
+            continue
+        print(f"{k:11} : {v}")
+    if pkg_name:
+        print(f"\nExecute `{pkg_name} --help` to see what you can do with {name}")
+
+
 class HyFI:
     """hyfi config primary class"""
 
     config = __global_config__
     SpeicialKeys = SpecialKeys
     __version__ = __global_config__.__version__
     __hyfi_path__ = __hyfi_path__()
     __home_path__ = __home_path__()
 
     def __init__(self) -> None:
         raise NotImplementedError("Use one of the static construction functions")
 
     @staticmethod
+    def about() -> None:
+        """Print the about information"""
+        cfg = __global_config__
+        _about(cfg)
+
+    @staticmethod
     def initialize(config: Union[DictConfig, Dict] = None):
         """Initialize the global config"""
         __global_config__.initialize(config)
 
     @staticmethod
     def terminate():
         """Terminate the global config"""
```

### Comparing `hyfi-0.2.9/src/hyfi/pipe.py` & `hyfi-0.3.0/src/hyfi/utils/pipe.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from tqdm.auto import tqdm
 
-from .hydra import SpecialKeys, _partial
-from .utils.batch import batcher, decorator_apply
-from .utils.logging import getLogger
+from ..hydra import SpecialKeys, _partial
+from .batch import batcher, decorator_apply
+from .logging import getLogger
 
 logger = getLogger(__name__)
 
 
 def _pipe(data, pipe):
     _func_ = pipe.get(SpecialKeys.FUNC)
     _fn = _partial(_func_)
```

### Comparing `hyfi-0.2.9/src/hyfi/utils/batch/apply.py` & `hyfi-0.3.0/src/hyfi/utils/batch/apply.py`

 * *Files identical despite different names*

### Comparing `hyfi-0.2.9/src/hyfi/utils/batch/apply_batch.py` & `hyfi-0.3.0/src/hyfi/utils/batch/apply_batch.py`

 * *Files identical despite different names*

### Comparing `hyfi-0.2.9/src/hyfi/utils/batch/batcher.py` & `hyfi-0.3.0/src/hyfi/utils/batch/batcher.py`

 * *Files identical despite different names*

### Comparing `hyfi-0.2.9/src/hyfi/utils/env.py` & `hyfi-0.3.0/src/hyfi/utils/env.py`

 * *Files identical despite different names*

### Comparing `hyfi-0.2.9/src/hyfi/utils/func.py` & `hyfi-0.3.0/src/hyfi/utils/func.py`

 * *Files identical despite different names*

### Comparing `hyfi-0.2.9/src/hyfi/utils/google.py` & `hyfi-0.3.0/src/hyfi/utils/google.py`

 * *Files identical despite different names*

### Comparing `hyfi-0.2.9/src/hyfi/utils/gpu.py` & `hyfi-0.3.0/src/hyfi/utils/gpu.py`

 * *Files identical despite different names*

### Comparing `hyfi-0.2.9/src/hyfi/utils/lib.py` & `hyfi-0.3.0/src/hyfi/utils/lib.py`

 * *Files identical despite different names*

### Comparing `hyfi-0.2.9/src/hyfi/utils/logging.py` & `hyfi-0.3.0/src/hyfi/utils/logging.py`

 * *Files identical despite different names*

### Comparing `hyfi-0.2.9/src/hyfi/utils/notebook.py` & `hyfi-0.3.0/src/hyfi/utils/notebook.py`

 * *Files identical despite different names*

### Comparing `hyfi-0.2.9/PKG-INFO` & `hyfi-0.3.0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,38 +1,41 @@
 Metadata-Version: 2.1
 Name: hyfi
-Version: 0.2.9
+Version: 0.3.0
 Summary: Hydra Fast Interface (Hydra and Pydantic based interface framework)
+Home-page: https://hyfi.entelecheia.ai
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
 Requires-Dist: cached-path (>=1.3.3,<2.0.0)
-Requires-Dist: chardet (<=4.0.0)
+Requires-Dist: chardet (<=5.1.0)
+Requires-Dist: colorama (>=0.4.3,<0.5.0)
 Requires-Dist: gdown (>=4.6.6,<5.0.0)
 Requires-Dist: hydra-colorlog (>=1.2.0,<2.0.0)
 Requires-Dist: hydra-core (>=1.3.2,<2.0.0)
-Requires-Dist: ipython (<=7.9.0) ; extra == "ipython"
+Requires-Dist: ipython (<=8.12.0) ; extra == "ipython"
 Requires-Dist: ipython-autotime (>=0.3.1,<0.4.0) ; extra == "ipython"
 Requires-Dist: matplotlib (>=3.7.1,<4.0.0)
 Requires-Dist: numpy (<1.24)
 Requires-Dist: pandas (>=1.5.3,<2.0.0)
 Requires-Dist: pydantic (>=1.10.7,<2.0.0)
-Requires-Dist: pygments (<=2.6.1) ; extra == "ipython"
+Requires-Dist: pygments (<=2.15.1) ; extra == "ipython"
 Requires-Dist: python-dotenv (>=1.0.0,<2.0.0)
 Requires-Dist: requests (>=2.27.1,<3.0.0)
 Requires-Dist: rich (>=11.1) ; extra == "ipython"
 Requires-Dist: scipy (>=1.10.1,<2.0.0)
 Requires-Dist: tqdm (>=4.64.1,<5.0.0)
+Project-URL: Repository, https://github.com/entelecheia/hyfi
 Description-Content-Type: text/markdown
 
 # HyFI: Hydra Fast Interface
 
 [![pypi-image]][pypi-url]
 [![version-image]][release-url]
 [![release-date-image]][release-url]
```

