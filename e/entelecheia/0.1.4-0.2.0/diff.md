# Comparing `tmp/entelecheia-0.1.4.tar.gz` & `tmp/entelecheia-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "entelecheia-0.1.4.tar", max compression
+gzip compressed data, was "entelecheia-0.2.0.tar", max compression
```

## Comparing `entelecheia-0.1.4.tar` & `entelecheia-0.2.0.tar`

### file list

```diff
@@ -1,24 +1,26 @@
--rw-r--r--   0        0        0     1071 2023-04-26 10:27:06.308644 entelecheia-0.1.4/LICENSE
--rw-r--r--   0        0        0      915 2023-04-26 10:27:06.308644 entelecheia-0.1.4/README.md
--rw-r--r--   0        0        0     2981 2023-04-26 10:27:31.192546 entelecheia-0.1.4/pyproject.toml
--rw-r--r--   0        0        0      179 2023-04-26 10:27:06.312644 entelecheia-0.1.4/src/entelecheia/__cli__.py
--rw-r--r--   0        0        0      892 2023-04-26 10:27:06.312644 entelecheia-0.1.4/src/entelecheia/__init__.py
--rw-r--r--   0        0        0       22 2023-04-26 10:27:31.144546 entelecheia-0.1.4/src/entelecheia/_version.py
--rw-r--r--   0        0        0        0 2023-04-26 10:27:06.312644 entelecheia-0.1.4/src/entelecheia/conf/__init__.py
--rw-r--r--   0        0        0      351 2023-04-26 10:27:31.144546 entelecheia-0.1.4/src/entelecheia/conf/about/__init__.yaml
--rw-r--r--   0        0        0      331 2023-04-26 10:27:06.312644 entelecheia-0.1.4/src/entelecheia/conf/batch/__init__.yaml
--rw-r--r--   0        0        0      506 2023-04-26 10:27:06.312644 entelecheia-0.1.4/src/entelecheia/conf/config.yaml
--rw-r--r--   0        0        0      789 2023-04-26 10:27:06.312644 entelecheia-0.1.4/src/entelecheia/conf/dotenv/__init__.yaml
--rw-r--r--   0        0        0      502 2023-04-26 10:27:06.312644 entelecheia-0.1.4/src/entelecheia/conf/hconf.yaml
--rw-r--r--   0        0        0     1126 2023-04-26 10:27:06.312644 entelecheia-0.1.4/src/entelecheia/conf/hydra/help/help.yaml
--rw-r--r--   0        0        0      264 2023-04-26 10:27:06.312644 entelecheia-0.1.4/src/entelecheia/conf/hydra/job_logging/custom.yaml
--rw-r--r--   0        0        0      295 2023-04-26 10:27:06.312644 entelecheia-0.1.4/src/entelecheia/conf/joblib/__init__.yaml
--rw-r--r--   0        0        0      701 2023-04-26 10:27:06.312644 entelecheia-0.1.4/src/entelecheia/conf/mode/__init__.yaml
--rw-r--r--   0        0        0      231 2023-04-26 10:27:06.312644 entelecheia-0.1.4/src/entelecheia/conf/mode/debug.yaml
--rw-r--r--   0        0        0      164 2023-04-26 10:27:06.312644 entelecheia-0.1.4/src/entelecheia/conf/path/__batch__.yaml
--rw-r--r--   0        0        0      582 2023-04-26 10:27:06.312644 entelecheia-0.1.4/src/entelecheia/conf/path/__default__.yaml
--rw-r--r--   0        0        0      616 2023-04-26 10:27:06.312644 entelecheia-0.1.4/src/entelecheia/conf/path/__init__.yaml
--rw-r--r--   0        0        0      360 2023-04-26 10:27:06.312644 entelecheia-0.1.4/src/entelecheia/conf/project/__init__.yaml
--rw-r--r--   0        0        0       83 2023-04-26 10:27:06.312644 entelecheia-0.1.4/src/entelecheia/conf/task/__init__.yaml
--rw-r--r--   0        0        0        0 2023-04-26 10:27:06.312644 entelecheia-0.1.4/src/entelecheia/py.typed
--rw-r--r--   0        0        0     1674 1970-01-01 00:00:00.000000 entelecheia-0.1.4/PKG-INFO
+-rw-r--r--   0        0        0     1071 2023-05-05 20:33:47.130278 entelecheia-0.2.0/LICENSE
+-rw-r--r--   0        0        0      915 2023-05-05 20:33:47.130278 entelecheia-0.2.0/README.md
+-rw-r--r--   0        0        0     3064 2023-05-05 20:34:15.435340 entelecheia-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0      292 2023-05-05 20:33:47.130278 entelecheia-0.2.0/src/entelecheia/__cli__.py
+-rw-r--r--   0        0        0      379 2023-05-05 20:33:47.130278 entelecheia-0.2.0/src/entelecheia/__init__.py
+-rw-r--r--   0        0        0       22 2023-05-05 20:34:15.375338 entelecheia-0.2.0/src/entelecheia/_version.py
+-rw-r--r--   0        0        0        0 2023-05-05 20:33:47.134278 entelecheia-0.2.0/src/entelecheia/conf/__init__.py
+-rw-r--r--   0        0        0      353 2023-05-05 20:34:15.375338 entelecheia-0.2.0/src/entelecheia/conf/about/__init__.yaml
+-rw-r--r--   0        0        0      331 2023-05-05 20:33:47.134278 entelecheia-0.2.0/src/entelecheia/conf/batch/__init__.yaml
+-rw-r--r--   0        0        0       83 2023-05-05 20:33:47.134278 entelecheia-0.2.0/src/entelecheia/conf/cmd/about.yaml
+-rw-r--r--   0        0        0      167 2023-05-05 20:33:47.134278 entelecheia-0.2.0/src/entelecheia/conf/cmd/cpcfg.yaml
+-rw-r--r--   0        0        0      320 2023-05-05 20:33:47.134278 entelecheia-0.2.0/src/entelecheia/conf/config.yaml
+-rw-r--r--   0        0        0      552 2023-05-05 20:33:47.134278 entelecheia-0.2.0/src/entelecheia/conf/copier/conf.yaml
+-rw-r--r--   0        0        0      789 2023-05-05 20:33:47.134278 entelecheia-0.2.0/src/entelecheia/conf/dotenv/__init__.yaml
+-rw-r--r--   0        0        0      319 2023-05-05 20:33:47.134278 entelecheia-0.2.0/src/entelecheia/conf/hconf.yaml
+-rw-r--r--   0        0        0     1128 2023-05-05 20:33:47.134278 entelecheia-0.2.0/src/entelecheia/conf/hydra/help/help.yaml
+-rw-r--r--   0        0        0      264 2023-05-05 20:33:47.134278 entelecheia-0.2.0/src/entelecheia/conf/hydra/job_logging/custom.yaml
+-rw-r--r--   0        0        0      293 2023-05-05 20:33:47.134278 entelecheia-0.2.0/src/entelecheia/conf/joblib/__init__.yaml
+-rw-r--r--   0        0        0      701 2023-05-05 20:33:47.134278 entelecheia-0.2.0/src/entelecheia/conf/mode/__init__.yaml
+-rw-r--r--   0        0        0      231 2023-05-05 20:33:47.134278 entelecheia-0.2.0/src/entelecheia/conf/mode/debug.yaml
+-rw-r--r--   0        0        0      164 2023-05-05 20:33:47.134278 entelecheia-0.2.0/src/entelecheia/conf/path/__batch__.yaml
+-rw-r--r--   0        0        0      582 2023-05-05 20:33:47.134278 entelecheia-0.2.0/src/entelecheia/conf/path/__default__.yaml
+-rw-r--r--   0        0        0      616 2023-05-05 20:33:47.134278 entelecheia-0.2.0/src/entelecheia/conf/path/__init__.yaml
+-rw-r--r--   0        0        0      360 2023-05-05 20:33:47.134278 entelecheia-0.2.0/src/entelecheia/conf/project/__init__.yaml
+-rw-r--r--   0        0        0        0 2023-05-05 20:33:47.134278 entelecheia-0.2.0/src/entelecheia/py.typed
+-rw-r--r--   0        0        0     1673 1970-01-01 00:00:00.000000 entelecheia-0.2.0/PKG-INFO
```

### Comparing `entelecheia-0.1.4/LICENSE` & `entelecheia-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `entelecheia-0.1.4/README.md` & `entelecheia-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `entelecheia-0.1.4/pyproject.toml` & `entelecheia-0.2.0/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,35 +1,42 @@
 [tool.poetry]
 name = "entelecheia"
-version = "0.1.4"
+version = "0.2.0"
 description = "ἐντελέχεια is coined by Aristotle from ἐντελής (entelḗs, “complete, full, accomplished”) + ἔχειν (ékhein, “have, hold”)."
 authors = ["Young Joon Lee <entelecheia@hotmail.com>"]
 license = "MIT"
 homepage = "https://entelecheia.me"
 repository = "https://github.com/entelecheia/entelecheia"
 readme = "README.md"
 packages = [{ include = "entelecheia", from = "src" }]
 
 [tool.poetry.scripts]
 entelecheia = 'entelecheia.__cli__:main'
 
+
 [tool.poetry.dependencies]
 python = ">=3.8.1,<3.12"
-hyfi = "^0.2.20"
+hyfi = "^0.3.5"
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
 
+[tool.poe]
+include = [".tasks.toml", ".tasks-extra.toml"]
+
 [tool.black]
 exclude = ['_version.py', 'node_modules', '_build', 'docs', 'tests', 'venv', '.copier-template', '.refs']
 
 [tool.isort]
 profile = "black"
 skip = ['_version.py', 'node_modules', '_build', 'docs', 'tests', 'venv', '.copier-template', '.refs']
 
@@ -70,15 +77,14 @@
 addopts = "-p no:cacheprovider" # deactivating pytest caching.
 
 [tool.coverage.report]
 exclude_lines = ['if __name__ == "__main__":']
 
 [tool.commitizen]
 name = "cz_conventional_commits"
-version = "1.0.1"
 tag_format = "v$version"
 
 [tool.semantic_release]
 branch = "main"
 version_toml = "pyproject.toml:tool.poetry.version"
 version_variable = "src/entelecheia/_version.py:__version__"
 version_pattern = 'src/entelecheia/conf/about/__init__.yaml:version: "{version}"'
@@ -87,13 +93,14 @@
 commit_subject = "chore(release): :rocket: {version} [skip ci]"
 prerelease_tag = "rc"
 major_on_zero = true
 tag_commit = true
 changelog_file = "CHANGELOG.md"
 upload_to_repository = true
 upload_to_release = true
-build_command = "poetry build --no-cache"
 hvcs = "github" # hosting version control system, gitlab is also supported
+build_command = "poetry build --no-cache"
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
+
```

### Comparing `entelecheia-0.1.4/src/entelecheia/conf/dotenv/__init__.yaml` & `entelecheia-0.2.0/src/entelecheia/conf/dotenv/__init__.yaml`

 * *Files identical despite different names*

### Comparing `entelecheia-0.1.4/src/entelecheia/conf/hydra/help/help.yaml` & `entelecheia-0.2.0/src/entelecheia/conf/hydra/help/help.yaml`

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

### Comparing `entelecheia-0.1.4/src/entelecheia/conf/mode/__init__.yaml` & `entelecheia-0.2.0/src/entelecheia/conf/mode/__init__.yaml`

 * *Files identical despite different names*

### Comparing `entelecheia-0.1.4/src/entelecheia/conf/path/__default__.yaml` & `entelecheia-0.2.0/src/entelecheia/conf/path/__default__.yaml`

 * *Files identical despite different names*

### Comparing `entelecheia-0.1.4/src/entelecheia/conf/path/__init__.yaml` & `entelecheia-0.2.0/src/entelecheia/conf/path/__init__.yaml`

 * *Files identical despite different names*

### Comparing `entelecheia-0.1.4/PKG-INFO` & `entelecheia-0.2.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: entelecheia
-Version: 0.1.4
+Version: 0.2.0
 Summary: ἐντελέχεια is coined by Aristotle from ἐντελής (entelḗs, “complete, full, accomplished”) + ἔχειν (ékhein, “have, hold”).
 Home-page: https://entelecheia.me
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
+Requires-Dist: hyfi (>=0.3.5,<0.4.0)
 Project-URL: Repository, https://github.com/entelecheia/entelecheia
 Description-Content-Type: text/markdown
 
 # ἐντελέχεια 【en.te.lé.kʰeː.a】
 
 [![home-img]][home-url]
 [![course-img]][course-url]
```

