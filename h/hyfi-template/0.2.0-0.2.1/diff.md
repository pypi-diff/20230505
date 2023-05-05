# Comparing `tmp/hyfi_template-0.2.0.tar.gz` & `tmp/hyfi_template-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hyfi_template-0.2.0.tar", max compression
+gzip compressed data, was "hyfi_template-0.2.1.tar", max compression
```

## Comparing `hyfi_template-0.2.0.tar` & `hyfi_template-0.2.1.tar`

### file list

```diff
@@ -1,24 +1,26 @@
--rw-r--r--   0        0        0     1071 2023-04-29 10:18:02.224290 hyfi_template-0.2.0/LICENSE
--rw-r--r--   0        0        0     2001 2023-04-29 10:18:02.224290 hyfi_template-0.2.0/README.md
--rw-r--r--   0        0        0     2964 2023-04-29 10:18:26.744812 hyfi_template-0.2.0/pyproject.toml
--rw-r--r--   0        0        0      181 2023-04-29 10:18:02.228289 hyfi_template-0.2.0/src/hyfi_template/__cli__.py
--rw-r--r--   0        0        0      894 2023-04-29 10:18:02.228289 hyfi_template-0.2.0/src/hyfi_template/__init__.py
--rw-r--r--   0        0        0       22 2023-04-29 10:18:26.692811 hyfi_template-0.2.0/src/hyfi_template/_version.py
--rw-r--r--   0        0        0        0 2023-04-29 10:18:02.228289 hyfi_template-0.2.0/src/hyfi_template/conf/__init__.py
--rw-r--r--   0        0        0      255 2023-04-29 10:18:26.692811 hyfi_template-0.2.0/src/hyfi_template/conf/about/__init__.yaml
--rw-r--r--   0        0        0      331 2023-04-29 10:18:02.228289 hyfi_template-0.2.0/src/hyfi_template/conf/batch/__init__.yaml
--rw-r--r--   0        0        0      506 2023-04-29 10:18:02.228289 hyfi_template-0.2.0/src/hyfi_template/conf/config.yaml
--rw-r--r--   0        0        0      789 2023-04-29 10:18:02.228289 hyfi_template-0.2.0/src/hyfi_template/conf/dotenv/__init__.yaml
--rw-r--r--   0        0        0      502 2023-04-29 10:18:02.228289 hyfi_template-0.2.0/src/hyfi_template/conf/hconf.yaml
--rw-r--r--   0        0        0     1126 2023-04-29 10:18:02.228289 hyfi_template-0.2.0/src/hyfi_template/conf/hydra/help/help.yaml
--rw-r--r--   0        0        0      264 2023-04-29 10:18:02.228289 hyfi_template-0.2.0/src/hyfi_template/conf/hydra/job_logging/custom.yaml
--rw-r--r--   0        0        0      295 2023-04-29 10:18:02.228289 hyfi_template-0.2.0/src/hyfi_template/conf/joblib/__init__.yaml
--rw-r--r--   0        0        0      701 2023-04-29 10:18:02.228289 hyfi_template-0.2.0/src/hyfi_template/conf/mode/__init__.yaml
--rw-r--r--   0        0        0      231 2023-04-29 10:18:02.228289 hyfi_template-0.2.0/src/hyfi_template/conf/mode/debug.yaml
--rw-r--r--   0        0        0      164 2023-04-29 10:18:02.228289 hyfi_template-0.2.0/src/hyfi_template/conf/path/__batch__.yaml
--rw-r--r--   0        0        0      582 2023-04-29 10:18:02.228289 hyfi_template-0.2.0/src/hyfi_template/conf/path/__default__.yaml
--rw-r--r--   0        0        0      616 2023-04-29 10:18:02.228289 hyfi_template-0.2.0/src/hyfi_template/conf/path/__init__.yaml
--rw-r--r--   0        0        0      360 2023-04-29 10:18:02.228289 hyfi_template-0.2.0/src/hyfi_template/conf/project/__init__.yaml
--rw-r--r--   0        0        0       83 2023-04-29 10:18:02.228289 hyfi_template-0.2.0/src/hyfi_template/conf/task/__init__.yaml
--rw-r--r--   0        0        0        0 2023-04-29 10:18:02.228289 hyfi_template-0.2.0/src/hyfi_template/py.typed
--rw-r--r--   0        0        0     2674 1970-01-01 00:00:00.000000 hyfi_template-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1071 2023-05-05 07:58:36.281279 hyfi_template-0.2.1/LICENSE
+-rw-r--r--   0        0        0     2001 2023-05-05 07:58:36.281279 hyfi_template-0.2.1/README.md
+-rw-r--r--   0        0        0     3082 2023-05-05 07:59:08.892189 hyfi_template-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0      294 2023-05-05 07:58:36.285282 hyfi_template-0.2.1/src/hyfi_template/__cli__.py
+-rw-r--r--   0        0        0      379 2023-05-05 07:58:36.285282 hyfi_template-0.2.1/src/hyfi_template/__init__.py
+-rw-r--r--   0        0        0       22 2023-05-05 07:59:08.832184 hyfi_template-0.2.1/src/hyfi_template/_version.py
+-rw-r--r--   0        0        0        0 2023-05-05 07:58:36.285282 hyfi_template-0.2.1/src/hyfi_template/conf/__init__.py
+-rw-r--r--   0        0        0      233 2023-05-05 07:59:08.832184 hyfi_template-0.2.1/src/hyfi_template/conf/about/__init__.yaml
+-rw-r--r--   0        0        0      331 2023-05-05 07:58:36.285282 hyfi_template-0.2.1/src/hyfi_template/conf/batch/__init__.yaml
+-rw-r--r--   0        0        0       83 2023-05-05 07:58:36.285282 hyfi_template-0.2.1/src/hyfi_template/conf/cmd/about.yaml
+-rw-r--r--   0        0        0      167 2023-05-05 07:58:36.285282 hyfi_template-0.2.1/src/hyfi_template/conf/cmd/cpcfg.yaml
+-rw-r--r--   0        0        0      320 2023-05-05 07:58:36.285282 hyfi_template-0.2.1/src/hyfi_template/conf/config.yaml
+-rw-r--r--   0        0        0      552 2023-05-05 07:58:36.285282 hyfi_template-0.2.1/src/hyfi_template/conf/copier/conf.yaml
+-rw-r--r--   0        0        0      789 2023-05-05 07:58:36.285282 hyfi_template-0.2.1/src/hyfi_template/conf/dotenv/__init__.yaml
+-rw-r--r--   0        0        0      319 2023-05-05 07:58:36.285282 hyfi_template-0.2.1/src/hyfi_template/conf/hconf.yaml
+-rw-r--r--   0        0        0     1128 2023-05-05 07:58:36.285282 hyfi_template-0.2.1/src/hyfi_template/conf/hydra/help/help.yaml
+-rw-r--r--   0        0        0      264 2023-05-05 07:58:36.285282 hyfi_template-0.2.1/src/hyfi_template/conf/hydra/job_logging/custom.yaml
+-rw-r--r--   0        0        0      293 2023-05-05 07:58:36.285282 hyfi_template-0.2.1/src/hyfi_template/conf/joblib/__init__.yaml
+-rw-r--r--   0        0        0      701 2023-05-05 07:58:36.285282 hyfi_template-0.2.1/src/hyfi_template/conf/mode/__init__.yaml
+-rw-r--r--   0        0        0      231 2023-05-05 07:58:36.285282 hyfi_template-0.2.1/src/hyfi_template/conf/mode/debug.yaml
+-rw-r--r--   0        0        0      164 2023-05-05 07:58:36.285282 hyfi_template-0.2.1/src/hyfi_template/conf/path/__batch__.yaml
+-rw-r--r--   0        0        0      582 2023-05-05 07:58:36.285282 hyfi_template-0.2.1/src/hyfi_template/conf/path/__default__.yaml
+-rw-r--r--   0        0        0      616 2023-05-05 07:58:36.285282 hyfi_template-0.2.1/src/hyfi_template/conf/path/__init__.yaml
+-rw-r--r--   0        0        0      360 2023-05-05 07:58:36.285282 hyfi_template-0.2.1/src/hyfi_template/conf/project/__init__.yaml
+-rw-r--r--   0        0        0        0 2023-05-05 07:58:36.285282 hyfi_template-0.2.1/src/hyfi_template/py.typed
+-rw-r--r--   0        0        0     2678 1970-01-01 00:00:00.000000 hyfi_template-0.2.1/PKG-INFO
```

### Comparing `hyfi_template-0.2.0/LICENSE` & `hyfi_template-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `hyfi_template-0.2.0/README.md` & `hyfi_template-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `hyfi_template-0.2.0/pyproject.toml` & `hyfi_template-0.2.1/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,40 +1,42 @@
 [tool.poetry]
 name = "hyfi-template"
-version = "0.2.0"
+version = "0.2.1"
 description = "A GitHub Template Repository for HyFI-based Projects"
 authors = ["Young Joon Lee <entelecheia@hotmail.com>"]
 license = "MIT"
 homepage = "https://hyfi-template.entelecheia.ai"
 repository = "https://github.com/entelecheia/hyfi-template"
 readme = "README.md"
 packages = [{ include = "hyfi_template", from = "src" }]
 
 [tool.poetry.scripts]
 hyfi_template = 'hyfi_template.__cli__:main'
 
 [tool.poetry.dependencies]
 python = ">=3.8.1,<3.12"
-hyfi = "^0.2.20"
+hyfi = {extras = ["all"], version = "^0.3.3"}
 
 [tool.poetry.group.dev]
 optional = true
 
 [tool.poetry.group.dev.dependencies]
 python-semantic-release = "^7.33.1"
 isort = "^5.12.0"
 black = "^23.1.0"
 flake8 = "^6.0.0"
 mypy = "^1.0.0"
 flake8-pyproject = "^1.2.2"
 pytest = "^7.2.1"
 pytest-cov = "^4.0.0"
+ipykernel = "^6.22.0"
+# hyfi = {path = "../hyfi", develop = true}
 
 [tool.poe]
-include = ".tasks.toml"
+include = [".tasks.toml", ".tasks-extra.toml"]
 
 [tool.black]
 exclude = ['_version.py', 'node_modules', '_build', 'docs', 'tests', 'venv', '.copier-template', '.refs']
 
 [tool.isort]
 profile = "black"
 skip = ['_version.py', 'node_modules', '_build', 'docs', 'tests', 'venv', '.copier-template', '.refs']
```

### Comparing `hyfi_template-0.2.0/src/hyfi_template/conf/dotenv/__init__.yaml` & `hyfi_template-0.2.1/src/hyfi_template/conf/dotenv/__init__.yaml`

 * *Files identical despite different names*

### Comparing `hyfi_template-0.2.0/src/hyfi_template/conf/hydra/help/help.yaml` & `hyfi_template-0.2.1/src/hyfi_template/conf/hydra/help/help.yaml`

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

### Comparing `hyfi_template-0.2.0/src/hyfi_template/conf/mode/__init__.yaml` & `hyfi_template-0.2.1/src/hyfi_template/conf/mode/__init__.yaml`

 * *Files identical despite different names*

### Comparing `hyfi_template-0.2.0/src/hyfi_template/conf/path/__default__.yaml` & `hyfi_template-0.2.1/src/hyfi_template/conf/path/__default__.yaml`

 * *Files identical despite different names*

### Comparing `hyfi_template-0.2.0/src/hyfi_template/conf/path/__init__.yaml` & `hyfi_template-0.2.1/src/hyfi_template/conf/path/__init__.yaml`

 * *Files identical despite different names*

### Comparing `hyfi_template-0.2.0/PKG-INFO` & `hyfi_template-0.2.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: hyfi-template
-Version: 0.2.0
+Version: 0.2.1
 Summary: A GitHub Template Repository for HyFI-based Projects
 Home-page: https://hyfi-template.entelecheia.ai
 License: MIT
 Author: Young Joon Lee
 Author-email: entelecheia@hotmail.com
 Requires-Python: >=3.8.1,<3.12
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
-Requires-Dist: hyfi (>=0.2.20,<0.3.0)
+Requires-Dist: hyfi[all] (>=0.3.3,<0.4.0)
 Project-URL: Repository, https://github.com/entelecheia/hyfi-template
 Description-Content-Type: text/markdown
 
 # HyFI Template
 
 [![pypi-image]][pypi-url]
 [![version-image]][release-url]
```

