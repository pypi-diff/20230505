# Comparing `tmp/jeeves_shell-2.1.5.tar.gz` & `tmp/jeeves_shell-2.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jeeves_shell-2.1.5.tar", max compression
+gzip compressed data, was "jeeves_shell-2.1.6.tar", max compression
```

## Comparing `jeeves_shell-2.1.5.tar` & `jeeves_shell-2.1.6.tar`

### file list

```diff
@@ -1,12 +1,11 @@
--rw-r--r--   0        0        0     1097 2022-11-04 16:58:55.671588 jeeves_shell-2.1.5/LICENSE
--rw-r--r--   0        0        0      956 2022-12-11 18:27:06.062169 jeeves_shell-2.1.5/README.md
--rw-r--r--   0        0        0       39 2022-12-11 18:23:17.084079 jeeves_shell-2.1.5/jeeves_shell/__init__.py
--rw-r--r--   0        0        0      797 2022-12-23 20:39:58.547042 jeeves_shell-2.1.5/jeeves_shell/cli.py
--rw-r--r--   0        0        0     3353 2023-04-15 21:43:00.746449 jeeves_shell-2.1.5/jeeves_shell/discover.py
--rw-r--r--   0        0        0      189 2022-12-09 17:35:01.246912 jeeves_shell-2.1.5/jeeves_shell/entry_points.py
--rw-r--r--   0        0        0      420 2022-12-09 20:33:49.924243 jeeves_shell-2.1.5/jeeves_shell/errors.py
--rw-r--r--   0        0        0      192 2023-04-15 21:18:06.757963 jeeves_shell-2.1.5/jeeves_shell/import_by_path.py
--rw-r--r--   0        0        0      307 2022-12-23 20:35:47.874000 jeeves_shell-2.1.5/jeeves_shell/jeeves.py
--rw-r--r--   0        0        0     1606 2023-04-15 21:43:21.558622 jeeves_shell-2.1.5/pyproject.toml
--rw-r--r--   0        0        0     1789 1970-01-01 00:00:00.000000 jeeves_shell-2.1.5/setup.py
--rw-r--r--   0        0        0     1896 1970-01-01 00:00:00.000000 jeeves_shell-2.1.5/PKG-INFO
+-rw-r--r--   0        0        0     1097 2022-11-04 16:58:55.671588 jeeves_shell-2.1.6/LICENSE
+-rw-r--r--   0        0        0      956 2022-12-11 18:27:06.062169 jeeves_shell-2.1.6/README.md
+-rw-r--r--   0        0        0       39 2022-12-11 18:23:17.084079 jeeves_shell-2.1.6/jeeves_shell/__init__.py
+-rw-r--r--   0        0        0      797 2022-12-23 20:39:58.547042 jeeves_shell-2.1.6/jeeves_shell/cli.py
+-rw-r--r--   0        0        0     3353 2023-04-15 21:43:00.746449 jeeves_shell-2.1.6/jeeves_shell/discover.py
+-rw-r--r--   0        0        0      189 2022-12-09 17:35:01.246912 jeeves_shell-2.1.6/jeeves_shell/entry_points.py
+-rw-r--r--   0        0        0      420 2022-12-09 20:33:49.924243 jeeves_shell-2.1.6/jeeves_shell/errors.py
+-rw-r--r--   0        0        0      256 2023-05-05 17:26:27.544054 jeeves_shell-2.1.6/jeeves_shell/import_by_path.py
+-rw-r--r--   0        0        0      307 2022-12-23 20:35:47.874000 jeeves_shell-2.1.6/jeeves_shell/jeeves.py
+-rw-r--r--   0        0        0     1562 2023-05-05 17:26:27.548054 jeeves_shell-2.1.6/pyproject.toml
+-rw-r--r--   0        0        0     1797 1970-01-01 00:00:00.000000 jeeves_shell-2.1.6/PKG-INFO
```

### Comparing `jeeves_shell-2.1.5/LICENSE` & `jeeves_shell-2.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `jeeves_shell-2.1.5/README.md` & `jeeves_shell-2.1.6/README.md`

 * *Files identical despite different names*

### Comparing `jeeves_shell-2.1.5/jeeves_shell/cli.py` & `jeeves_shell-2.1.6/jeeves_shell/cli.py`

 * *Files identical despite different names*

### Comparing `jeeves_shell-2.1.5/jeeves_shell/discover.py` & `jeeves_shell-2.1.6/jeeves_shell/discover.py`

 * *Files identical despite different names*

### Comparing `jeeves_shell-2.1.5/pyproject.toml` & `jeeves_shell-2.1.6/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 
 [tool.poetry]
 name = "jeeves-shell"
 description = "Pythonic replacement for GNU Make"
-version = "2.1.5"
+version = "2.1.6"
 license = "MIT"
 
 authors = []
 
 readme = "README.md"
 
 repository = "https://github.com/jeeves-sh/jeeves-shell"
@@ -26,29 +26,27 @@
 
 
 [tool.poetry.scripts]
 j = "jeeves_shell.cli:app"
 
 
 [tool.poetry.dependencies]
-python = ">=3.8,<4.0"
+python = ">=3.10,<4.0"
 typer = "^0.7.0"
 documented = "^0.1.1"
 more-itertools = "^9.0.0"
 
 
 [tool.poetry.group.dev.dependencies]
 m2r2 = "^0.2"
-mkdocs = "^1.2.2"
 mkdocstrings = "^0.19.1"
-mkdocs-material = "^8.5.11"
 
 markupsafe = "<2.1"   # Otherwise, `jinja2` will fail
 importlib-metadata = "<5.0"
-jeeves-yeti-pyproject = "^0.2.0"
+jeeves-yeti-pyproject = "^0.2.15"
 mkdocs-macros-plugin = "^0.7.0"
 dominate = "^2.7.0"
 
 [tool.flakeheaven.exceptions."jeeves_shell/jeeves.py"]
 wemake-python-styleguide = [
   "-WPS115",
   "-WPS600",
```

### Comparing `jeeves_shell-2.1.5/PKG-INFO` & `jeeves_shell-2.1.6/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,21 +1,19 @@
 Metadata-Version: 2.1
 Name: jeeves-shell
-Version: 2.1.5
+Version: 2.1.6
 Summary: Pythonic replacement for GNU Make
 Home-page: https://github.com/jeeves-sh/jeeves-shell
 License: MIT
-Requires-Python: >=3.8,<4.0
+Requires-Python: >=3.10,<4.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.8
-Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Requires-Dist: documented (>=0.1.1,<0.2.0)
 Requires-Dist: more-itertools (>=9.0.0,<10.0.0)
 Requires-Dist: typer (>=0.7.0,<0.8.0)
 Project-URL: Repository, https://github.com/jeeves-sh/jeeves-shell
```

