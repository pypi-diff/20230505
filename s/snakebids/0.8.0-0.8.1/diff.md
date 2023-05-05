# Comparing `tmp/snakebids-0.8.0.tar.gz` & `tmp/snakebids-0.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "snakebids-0.8.0.tar", max compression
+gzip compressed data, was "snakebids-0.8.1.tar", max compression
```

## Comparing `snakebids-0.8.0.tar` & `snakebids-0.8.1.tar`

### file list

```diff
@@ -1,42 +1,42 @@
--rw-r--r--   0        0        0     1065 2023-04-26 15:01:52.399305 snakebids-0.8.0/LICENSE
--rw-r--r--   0        0        0     2305 2023-04-26 15:01:52.399305 snakebids-0.8.0/README.md
--rw-r--r--   0        0        0     2906 2023-04-26 15:02:22.455957 snakebids-0.8.0/pyproject.toml
--rw-r--r--   0        0        0      654 2023-04-26 15:02:22.459957 snakebids-0.8.0/snakebids/__init__.py
--rw-r--r--   0        0        0     2007 2023-04-26 15:01:52.399305 snakebids-0.8.0/snakebids/admin.py
--rw-r--r--   0        0        0    10207 2023-04-26 15:01:52.399305 snakebids-0.8.0/snakebids/app.py
--rw-r--r--   0        0        0    10775 2023-04-26 15:01:52.399305 snakebids-0.8.0/snakebids/cli.py
--rw-r--r--   0        0        0      742 2023-04-26 15:01:52.399305 snakebids-0.8.0/snakebids/core/__init__.py
--rw-r--r--   0        0        0     8118 2023-04-26 15:01:52.403305 snakebids-0.8.0/snakebids/core/construct_bids.py
--rw-r--r--   0        0        0    18389 2023-04-26 15:01:52.403305 snakebids-0.8.0/snakebids/core/datasets.py
--rw-r--r--   0        0        0     9128 2023-04-26 15:01:52.403305 snakebids-0.8.0/snakebids/core/filtering.py
--rw-r--r--   0        0        0    24692 2023-04-26 15:01:52.403305 snakebids-0.8.0/snakebids/core/input_generation.py
--rw-r--r--   0        0        0      519 2023-04-26 15:01:52.403305 snakebids-0.8.0/snakebids/exceptions.py
--rw-r--r--   0        0        0     4219 2023-04-26 15:01:52.403305 snakebids-0.8.0/snakebids/io/console.py
--rw-r--r--   0        0        0     3271 2023-04-26 15:01:52.403305 snakebids-0.8.0/snakebids/io/printing.py
--rw-r--r--   0        0        0      317 2023-04-26 15:02:22.459957 snakebids-0.8.0/snakebids/project_template/cookiecutter.json
--rw-r--r--   0        0        0       73 2023-04-26 15:01:52.403305 snakebids-0.8.0/snakebids/project_template/{{cookiecutter.app_name}}/README.rst
--rw-r--r--   0        0        0     3253 2023-04-26 15:01:52.403305 snakebids-0.8.0/snakebids/project_template/{{cookiecutter.app_name}}/config/snakebids.yml
--rw-r--r--   0        0        0        7 2023-04-26 15:01:52.403305 snakebids-0.8.0/snakebids/project_template/{{cookiecutter.app_name}}/docs/.gitignore
--rw-r--r--   0        0        0      634 2023-04-26 15:01:52.403305 snakebids-0.8.0/snakebids/project_template/{{cookiecutter.app_name}}/docs/Makefile
--rw-r--r--   0        0        0     1978 2023-04-26 15:01:52.403305 snakebids-0.8.0/snakebids/project_template/{{cookiecutter.app_name}}/docs/conf.py
--rw-r--r--   0        0        0     3317 2023-04-26 15:01:52.403305 snakebids-0.8.0/snakebids/project_template/{{cookiecutter.app_name}}/docs/getting_started/installation.rst
--rw-r--r--   0        0        0      548 2023-04-26 15:01:52.403305 snakebids-0.8.0/snakebids/project_template/{{cookiecutter.app_name}}/docs/index.rst
--rw-r--r--   0        0        0       93 2023-04-26 15:01:52.403305 snakebids-0.8.0/snakebids/project_template/{{cookiecutter.app_name}}/docs/requirements.txt
--rw-r--r--   0        0        0      168 2023-04-26 15:01:52.403305 snakebids-0.8.0/snakebids/project_template/{{cookiecutter.app_name}}/docs/usage/app_cli.rst
--rw-r--r--   0        0        0      155 2023-04-26 15:01:52.403305 snakebids-0.8.0/snakebids/project_template/{{cookiecutter.app_name}}/docs/usage/snakemake_cli.rst
--rw-r--r--   0        0        0      570 2023-04-26 15:01:52.403305 snakebids-0.8.0/snakebids/project_template/{{cookiecutter.app_name}}/pipeline_description.json
--rw-r--r--   0        0        0     1194 2023-04-26 15:01:52.403305 snakebids-0.8.0/snakebids/project_template/{{cookiecutter.app_name}}/setup.py
--rw-r--r--   0        0        0     1592 2023-04-26 15:01:52.403305 snakebids-0.8.0/snakebids/project_template/{{cookiecutter.app_name}}/workflow/Snakefile
--rw-r--r--   0        0        0      399 2023-04-26 15:01:52.403305 snakebids-0.8.0/snakebids/project_template/{{cookiecutter.app_name}}/{{cookiecutter.app_name}}/run.py
--rw-r--r--   0        0        0        0 2023-04-26 15:01:52.403305 snakebids-0.8.0/snakebids/py.typed
--rw-r--r--   0        0        0       13 2023-04-26 15:01:52.403305 snakebids-0.8.0/snakebids/resources/__init__.py
--rw-r--r--   0        0        0     4216 2023-04-26 15:01:52.403305 snakebids-0.8.0/snakebids/resources/bids_tags.json
--rw-r--r--   0        0        0     3489 2023-04-26 15:01:52.403305 snakebids-0.8.0/snakebids/types.py
--rw-r--r--   0        0        0       70 2023-04-26 15:01:52.403305 snakebids-0.8.0/snakebids/utils/__init__.py
--rw-r--r--   0        0        0     5839 2023-04-26 15:01:52.403305 snakebids-0.8.0/snakebids/utils/output.py
--rw-r--r--   0        0        0      990 2023-04-26 15:01:52.403305 snakebids-0.8.0/snakebids/utils/sb_itertools.py
--rw-r--r--   0        0        0     4947 2023-04-26 15:01:52.403305 snakebids-0.8.0/snakebids/utils/snakemake_io.py
--rw-r--r--   0        0        0       91 2023-04-26 15:01:52.403305 snakebids-0.8.0/snakebids/utils/user_property.py
--rw-r--r--   0        0        0      242 2023-04-26 15:01:52.403305 snakebids-0.8.0/snakebids/utils/user_property.pyi
--rw-r--r--   0        0        0    10690 2023-04-26 15:01:52.403305 snakebids-0.8.0/snakebids/utils/utils.py
--rw-r--r--   0        0        0     3910 1970-01-01 00:00:00.000000 snakebids-0.8.0/PKG-INFO
+-rw-r--r--   0        0        0     1065 2023-05-05 16:11:05.997278 snakebids-0.8.1/LICENSE
+-rw-r--r--   0        0        0     2305 2023-05-05 16:11:05.997278 snakebids-0.8.1/README.md
+-rw-r--r--   0        0        0     3225 2023-05-05 16:11:35.901703 snakebids-0.8.1/pyproject.toml
+-rw-r--r--   0        0        0      654 2023-05-05 16:11:35.905703 snakebids-0.8.1/snakebids/__init__.py
+-rw-r--r--   0        0        0     2007 2023-05-05 16:11:06.001278 snakebids-0.8.1/snakebids/admin.py
+-rw-r--r--   0        0        0    10207 2023-05-05 16:11:06.001278 snakebids-0.8.1/snakebids/app.py
+-rw-r--r--   0        0        0    11003 2023-05-05 16:11:06.001278 snakebids-0.8.1/snakebids/cli.py
+-rw-r--r--   0        0        0      742 2023-05-05 16:11:06.001278 snakebids-0.8.1/snakebids/core/__init__.py
+-rw-r--r--   0        0        0     8118 2023-05-05 16:11:06.001278 snakebids-0.8.1/snakebids/core/construct_bids.py
+-rw-r--r--   0        0        0    18389 2023-05-05 16:11:06.001278 snakebids-0.8.1/snakebids/core/datasets.py
+-rw-r--r--   0        0        0     9128 2023-05-05 16:11:06.001278 snakebids-0.8.1/snakebids/core/filtering.py
+-rw-r--r--   0        0        0    24692 2023-05-05 16:11:06.001278 snakebids-0.8.1/snakebids/core/input_generation.py
+-rw-r--r--   0        0        0      519 2023-05-05 16:11:06.001278 snakebids-0.8.1/snakebids/exceptions.py
+-rw-r--r--   0        0        0     4219 2023-05-05 16:11:06.001278 snakebids-0.8.1/snakebids/io/console.py
+-rw-r--r--   0        0        0     3271 2023-05-05 16:11:06.001278 snakebids-0.8.1/snakebids/io/printing.py
+-rw-r--r--   0        0        0      317 2023-05-05 16:11:35.905703 snakebids-0.8.1/snakebids/project_template/cookiecutter.json
+-rw-r--r--   0        0        0       73 2023-05-05 16:11:06.001278 snakebids-0.8.1/snakebids/project_template/{{cookiecutter.app_name}}/README.rst
+-rw-r--r--   0        0        0     3253 2023-05-05 16:11:06.001278 snakebids-0.8.1/snakebids/project_template/{{cookiecutter.app_name}}/config/snakebids.yml
+-rw-r--r--   0        0        0        7 2023-05-05 16:11:06.001278 snakebids-0.8.1/snakebids/project_template/{{cookiecutter.app_name}}/docs/.gitignore
+-rw-r--r--   0        0        0      634 2023-05-05 16:11:06.001278 snakebids-0.8.1/snakebids/project_template/{{cookiecutter.app_name}}/docs/Makefile
+-rw-r--r--   0        0        0     1978 2023-05-05 16:11:06.001278 snakebids-0.8.1/snakebids/project_template/{{cookiecutter.app_name}}/docs/conf.py
+-rw-r--r--   0        0        0     3317 2023-05-05 16:11:06.001278 snakebids-0.8.1/snakebids/project_template/{{cookiecutter.app_name}}/docs/getting_started/installation.rst
+-rw-r--r--   0        0        0      548 2023-05-05 16:11:06.001278 snakebids-0.8.1/snakebids/project_template/{{cookiecutter.app_name}}/docs/index.rst
+-rw-r--r--   0        0        0       93 2023-05-05 16:11:06.001278 snakebids-0.8.1/snakebids/project_template/{{cookiecutter.app_name}}/docs/requirements.txt
+-rw-r--r--   0        0        0      168 2023-05-05 16:11:06.001278 snakebids-0.8.1/snakebids/project_template/{{cookiecutter.app_name}}/docs/usage/app_cli.rst
+-rw-r--r--   0        0        0      155 2023-05-05 16:11:06.001278 snakebids-0.8.1/snakebids/project_template/{{cookiecutter.app_name}}/docs/usage/snakemake_cli.rst
+-rw-r--r--   0        0        0      570 2023-05-05 16:11:06.001278 snakebids-0.8.1/snakebids/project_template/{{cookiecutter.app_name}}/pipeline_description.json
+-rw-r--r--   0        0        0     1194 2023-05-05 16:11:06.001278 snakebids-0.8.1/snakebids/project_template/{{cookiecutter.app_name}}/setup.py
+-rw-r--r--   0        0        0     1592 2023-05-05 16:11:06.001278 snakebids-0.8.1/snakebids/project_template/{{cookiecutter.app_name}}/workflow/Snakefile
+-rw-r--r--   0        0        0      399 2023-05-05 16:11:06.001278 snakebids-0.8.1/snakebids/project_template/{{cookiecutter.app_name}}/{{cookiecutter.app_name}}/run.py
+-rw-r--r--   0        0        0        0 2023-05-05 16:11:06.001278 snakebids-0.8.1/snakebids/py.typed
+-rw-r--r--   0        0        0       13 2023-05-05 16:11:06.001278 snakebids-0.8.1/snakebids/resources/__init__.py
+-rw-r--r--   0        0        0     4216 2023-05-05 16:11:06.001278 snakebids-0.8.1/snakebids/resources/bids_tags.json
+-rw-r--r--   0        0        0     3489 2023-05-05 16:11:06.005278 snakebids-0.8.1/snakebids/types.py
+-rw-r--r--   0        0        0       70 2023-05-05 16:11:06.005278 snakebids-0.8.1/snakebids/utils/__init__.py
+-rw-r--r--   0        0        0     5839 2023-05-05 16:11:06.005278 snakebids-0.8.1/snakebids/utils/output.py
+-rw-r--r--   0        0        0      990 2023-05-05 16:11:06.005278 snakebids-0.8.1/snakebids/utils/sb_itertools.py
+-rw-r--r--   0        0        0     4947 2023-05-05 16:11:06.005278 snakebids-0.8.1/snakebids/utils/snakemake_io.py
+-rw-r--r--   0        0        0       91 2023-05-05 16:11:06.005278 snakebids-0.8.1/snakebids/utils/user_property.py
+-rw-r--r--   0        0        0      242 2023-05-05 16:11:06.005278 snakebids-0.8.1/snakebids/utils/user_property.pyi
+-rw-r--r--   0        0        0    10690 2023-05-05 16:11:06.005278 snakebids-0.8.1/snakebids/utils/utils.py
+-rw-r--r--   0        0        0     4002 1970-01-01 00:00:00.000000 snakebids-0.8.1/PKG-INFO
```

### Comparing `snakebids-0.8.0/LICENSE` & `snakebids-0.8.1/LICENSE`

 * *Files identical despite different names*

### Comparing `snakebids-0.8.0/README.md` & `snakebids-0.8.1/README.md`

 * *Files identical despite different names*

### Comparing `snakebids-0.8.0/pyproject.toml` & `snakebids-0.8.1/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "snakebids"
-version = "0.8.0"
+version = "0.8.1"
 description = "BIDS integration into snakemake workflows"
 readme = "README.md"
 repository = "https://github.com/akhanf/snakebids"
 documentation = "https://snakebids.readthedocs.io/"
 authors = [
     "Ali Khan <alik@robarts.ca>",
     "Peter Van Dyken <pvandyk2@uwo.ca>",
@@ -21,28 +21,37 @@
 enable = false
 vcs = "git"
 dirty = true
 style = "pep440"
 bump = true
 
 [tool.poetry-dynamic-versioning.substitution]
-files = ['snakebids/project_template/cookiecutter.json', 'snakebids/__init__.py']
-patterns = ["(^\\s+\"snakebids_version\":\\s*\")[^'\"]*(\")", "(^__version__\\s*(?::.*?)?=\\s*['\"])[^'\"]*(['\"])"]
+files = [
+    'snakebids/project_template/cookiecutter.json',
+    'snakebids/__init__.py'
+]
+patterns = [
+    "(^\\s+\"snakebids_version\":\\s*\")[^'\"]*(\")",
+    "(^__version__\\s*(?::.*?)?=\\s*['\"])[^'\"]*(['\"])"
+]
 
 [tool.poetry.dependencies]
 python = ">=3.7,<3.12"
-pybids = "^0.15.0"
+pybids = [
+    { version="^0.15.0", python = "<3.8" },
+    { version="^0.16.0", python = ">=3.8" },
+]
 snakemake = [
     { version = ">=5.28.0", python = ">=3.7" },
     { version = ">=7.18.2", python = ">=3.11" },
 ]
 PyYAML = "^6"
 cookiecutter = "^2.1.1"
 typing-extensions = ">=3.10.0"
-attrs = ">=21.2.0,<23"
+attrs = ">=21.2.0,<24"
 boutiques = "^0.5.25"
 more-itertools = ">=8,<10"
 cached-property = "^1.5.2"
 pvandyken-deprecated = "0.0.3"
 
 #  Below are non-direct dependencies (i.e. dependencies of other depenencies)
 #  specified to ensure a version with a pre-built wheel is installed depending
@@ -58,40 +67,48 @@
 scipy = [
     { version = "<1.8", python = "3.7"},
     { version = ">=1.9.2", python = ">=3.11" }
 ]
 
 [tool.poetry.group.dev.dependencies]
 black = "^23.1.0"
-pybids = "^0.15.2"
+# We need at least 0.15.2 just for testing
+pybids = [
+    { version="^0.15.2", python = "<3.8" },
+    { version="^0.16.0", python = ">=3.8" },
+]
 pytest = "^7.0.0"
 pytest-mock = "^3.7.0"
 isort = "^5.10.1"
-poethepoet = "^0.18.1"
+poethepoet = "^0.19.0"
 # pre-commit==3.0.0 requires py38 or greater
 pre-commit = "^2.17.0"
 mkinit = "^1.0.0"
 hypothesis = "^6.34.1"
 pytest-benchmark = "^4.0.0"
 pyfakefs = "^5.1.0"
 pyparsing = "^3.0.9"
 pyright = "^1.1.302"
-ruff = "^0.0.261"
+ruff = "^0.0.263"
 
 [tool.poetry.scripts]
 snakebids = "snakebids.admin:main"
 
 [build-system]
 requires = ["poetry-core>=1.0.0", "poetry-dynamic-versioning"]
 build-backend = "poetry_dynamic_versioning.backend"
 
 [tool.poe.tasks]
 setup = "pre-commit install"
 quality = { shell = "isort snakebids && black snakebids && ruff snakebids" }
-test = "pytest --doctest-modules --ignore=docs --ignore=snakebids/project_template --benchmark-disable"
+fix = { shell = "isort snakebids && black snakebids && ruff --fix snakebids"}
+test = """
+pytest --doctest-modules --ignore=docs \
+    --ignore=snakebids/project_template --benchmark-disable
+"""
 mkinit = "mkinit --recursive --nomods --black -i snakebids"
 benchmark = "pytest --benchmark-only --benchmark-autosave"
 
 [tool.isort]
 profile = "black"
 multi_line_output = 3
```

### Comparing `snakebids-0.8.0/snakebids/__init__.py` & `snakebids-0.8.1/snakebids/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """Top-level namespace containing the core classes and functions"""
 __submodules__ = ["core"]
 
-__version__ = "0.8.0"
+__version__ = "0.8.1"
 
 # <AUTOGEN_INIT>
 from snakebids.core import (
     BidsComponent,
     BidsDataset,
     BidsDatasetDict,
     bids,
```

### Comparing `snakebids-0.8.0/snakebids/admin.py` & `snakebids-0.8.1/snakebids/admin.py`

 * *Files identical despite different names*

### Comparing `snakebids-0.8.0/snakebids/app.py` & `snakebids-0.8.1/snakebids/app.py`

 * *Files identical despite different names*

### Comparing `snakebids-0.8.0/snakebids/cli.py` & `snakebids-0.8.1/snakebids/cli.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 from __future__ import annotations
 
 import argparse
 import logging
-import os
 import pathlib
 import re
 from collections.abc import Sequence
-from typing import Any, Iterable, Mapping, Optional
+from typing import Any, Iterable, Mapping, Optional, TypeVar, overload
 
 import attr
 import snakemake
 
 from snakebids.types import InputsConfig
 
 # We define Path here in addition to pathlib to put both variables in globals()
@@ -311,17 +310,28 @@
             name,
             re.sub(r"\_", "-", name),
             f"--{re.sub(r'-', '_', name_part)}",
         }
     return {name}
 
 
-def _resolve_path(
-    path_candidate: Iterable["os.PathLike[str] | str"] | "os.PathLike[str]" | str,
-) -> Any:
+_T = TypeVar("_T")
+
+
+@overload
+def _resolve_path(path_candidate: Sequence[Any]) -> "list[Any]":
+    ...
+
+
+@overload
+def _resolve_path(path_candidate: _T) -> _T:
+    ...
+
+
+def _resolve_path(path_candidate: Any) -> Any:
     """Helper function to resolve any paths or list
     of paths it's passed. Otherwise, returns the argument
     unchanged.
 
     Parameters
     ----------
     command : list, os.Pathlike, object
@@ -330,14 +340,17 @@
     Returns
     -------
     list, Path, object
         If os.Pathlike or list  of os.Pathlike, the same paths resolved.
         Otherwise, the argument unchanged.
     """
 
-    if isinstance(path_candidate, Iterable) and not isinstance(path_candidate, str):
-        return [_resolve_path(p) for p in path_candidate]
+    if isinstance(path_candidate, Sequence) and not isinstance(path_candidate, str):
+        return [
+            _resolve_path(p)  # type: ignore[reportUnknownArgumentType]
+            for p in path_candidate  # type: ignore[reportUnknownVariableType]
+        ]
 
-    if isinstance(path_candidate, os.PathLike):
+    if isinstance(path_candidate, Path):
         return Path(path_candidate).resolve()
 
     return path_candidate
```

### Comparing `snakebids-0.8.0/snakebids/core/__init__.py` & `snakebids-0.8.1/snakebids/core/__init__.py`

 * *Files identical despite different names*

### Comparing `snakebids-0.8.0/snakebids/core/construct_bids.py` & `snakebids-0.8.1/snakebids/core/construct_bids.py`

 * *Files identical despite different names*

### Comparing `snakebids-0.8.0/snakebids/core/datasets.py` & `snakebids-0.8.1/snakebids/core/datasets.py`

 * *Files identical despite different names*

### Comparing `snakebids-0.8.0/snakebids/core/filtering.py` & `snakebids-0.8.1/snakebids/core/filtering.py`

 * *Files identical despite different names*

### Comparing `snakebids-0.8.0/snakebids/core/input_generation.py` & `snakebids-0.8.1/snakebids/core/input_generation.py`

 * *Files identical despite different names*

### Comparing `snakebids-0.8.0/snakebids/exceptions.py` & `snakebids-0.8.1/snakebids/exceptions.py`

 * *Files identical despite different names*

### Comparing `snakebids-0.8.0/snakebids/io/console.py` & `snakebids-0.8.1/snakebids/io/console.py`

 * *Files identical despite different names*

### Comparing `snakebids-0.8.0/snakebids/io/printing.py` & `snakebids-0.8.1/snakebids/io/printing.py`

 * *Files identical despite different names*

### Comparing `snakebids-0.8.0/snakebids/project_template/{{cookiecutter.app_name}}/config/snakebids.yml` & `snakebids-0.8.1/snakebids/project_template/{{cookiecutter.app_name}}/config/snakebids.yml`

 * *Files identical despite different names*

### Comparing `snakebids-0.8.0/snakebids/project_template/{{cookiecutter.app_name}}/docs/Makefile` & `snakebids-0.8.1/snakebids/project_template/{{cookiecutter.app_name}}/docs/Makefile`

 * *Files identical despite different names*

### Comparing `snakebids-0.8.0/snakebids/project_template/{{cookiecutter.app_name}}/docs/conf.py` & `snakebids-0.8.1/snakebids/project_template/{{cookiecutter.app_name}}/docs/conf.py`

 * *Files identical despite different names*

### Comparing `snakebids-0.8.0/snakebids/project_template/{{cookiecutter.app_name}}/docs/getting_started/installation.rst` & `snakebids-0.8.1/snakebids/project_template/{{cookiecutter.app_name}}/docs/getting_started/installation.rst`

 * *Files identical despite different names*

### Comparing `snakebids-0.8.0/snakebids/project_template/{{cookiecutter.app_name}}/docs/index.rst` & `snakebids-0.8.1/snakebids/project_template/{{cookiecutter.app_name}}/docs/index.rst`

 * *Files identical despite different names*

### Comparing `snakebids-0.8.0/snakebids/project_template/{{cookiecutter.app_name}}/pipeline_description.json` & `snakebids-0.8.1/snakebids/project_template/{{cookiecutter.app_name}}/pipeline_description.json`

 * *Files identical despite different names*

### Comparing `snakebids-0.8.0/snakebids/project_template/{{cookiecutter.app_name}}/setup.py` & `snakebids-0.8.1/snakebids/project_template/{{cookiecutter.app_name}}/setup.py`

 * *Files identical despite different names*

### Comparing `snakebids-0.8.0/snakebids/project_template/{{cookiecutter.app_name}}/workflow/Snakefile` & `snakebids-0.8.1/snakebids/project_template/{{cookiecutter.app_name}}/workflow/Snakefile`

 * *Files identical despite different names*

### Comparing `snakebids-0.8.0/snakebids/resources/bids_tags.json` & `snakebids-0.8.1/snakebids/resources/bids_tags.json`

 * *Files identical despite different names*

### Comparing `snakebids-0.8.0/snakebids/types.py` & `snakebids-0.8.1/snakebids/types.py`

 * *Files identical despite different names*

### Comparing `snakebids-0.8.0/snakebids/utils/output.py` & `snakebids-0.8.1/snakebids/utils/output.py`

 * *Files identical despite different names*

### Comparing `snakebids-0.8.0/snakebids/utils/sb_itertools.py` & `snakebids-0.8.1/snakebids/utils/sb_itertools.py`

 * *Files identical despite different names*

### Comparing `snakebids-0.8.0/snakebids/utils/snakemake_io.py` & `snakebids-0.8.1/snakebids/utils/snakemake_io.py`

 * *Files identical despite different names*

### Comparing `snakebids-0.8.0/snakebids/utils/utils.py` & `snakebids-0.8.1/snakebids/utils/utils.py`

 * *Files identical despite different names*

### Comparing `snakebids-0.8.0/PKG-INFO` & `snakebids-0.8.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,35 +1,36 @@
 Metadata-Version: 2.1
 Name: snakebids
-Version: 0.8.0
+Version: 0.8.1
 Summary: BIDS integration into snakemake workflows
 Home-page: https://github.com/akhanf/snakebids
 License: MIT
 Author: Ali Khan
 Author-email: alik@robarts.ca
 Requires-Python: >=3.7,<3.12
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: PyYAML (>=6,<7)
-Requires-Dist: attrs (>=21.2.0,<23)
+Requires-Dist: attrs (>=21.2.0,<24)
 Requires-Dist: boutiques (>=0.5.25,<0.6.0)
 Requires-Dist: cached-property (>=1.5.2,<2.0.0)
 Requires-Dist: cookiecutter (>=2.1.1,<3.0.0)
 Requires-Dist: more-itertools (>=8,<10)
 Requires-Dist: numpy (>=1.21.2) ; python_version == "3.10"
 Requires-Dist: numpy (>=1.23.2) ; python_version >= "3.11"
 Requires-Dist: pandas (>=1.3) ; python_full_version >= "3.7.1"
 Requires-Dist: pandas (>=1.5) ; python_version >= "3.11"
 Requires-Dist: pvandyken-deprecated (==0.0.3)
-Requires-Dist: pybids (>=0.15.0,<0.16.0)
+Requires-Dist: pybids (>=0.15.0,<0.16.0) ; python_version < "3.8"
+Requires-Dist: pybids (>=0.16.0,<0.17.0) ; python_version >= "3.8"
 Requires-Dist: scipy (<1.8) ; python_version == "3.7"
 Requires-Dist: scipy (>=1.9.2) ; python_version >= "3.11"
 Requires-Dist: snakemake (>=5.28.0) ; python_version >= "3.7"
 Requires-Dist: snakemake (>=7.18.2) ; python_version >= "3.11"
 Requires-Dist: typing-extensions (>=3.10.0)
 Project-URL: Documentation, https://snakebids.readthedocs.io/
 Project-URL: Repository, https://github.com/akhanf/snakebids
```

