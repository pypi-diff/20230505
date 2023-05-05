# Comparing `tmp/pytest-logikal-1.7.0.tar.gz` & `tmp/pytest-logikal-1.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytest-logikal-1.7.0.tar", last modified: Thu Mar  9 21:16:49 2023, max compression
+gzip compressed data, was "pytest-logikal-1.8.0.tar", last modified: Fri May  5 11:07:40 2023, max compression
```

## Comparing `pytest-logikal-1.7.0.tar` & `pytest-logikal-1.8.0.tar`

### file list

```diff
@@ -1,44 +1,55 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-09 21:16:49.045146 pytest-logikal-1.7.0/
--rw-r--r--   0 runner    (1001) docker     (122)     1052 2023-03-09 21:16:19.000000 pytest-logikal-1.7.0/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (122)       56 2023-03-09 21:16:19.000000 pytest-logikal-1.7.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)     2462 2023-03-09 21:16:49.045146 pytest-logikal-1.7.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      280 2023-03-09 21:16:19.000000 pytest-logikal-1.7.0/README.rst
--rw-r--r--   0 runner    (1001) docker     (122)      458 2023-03-09 21:16:19.000000 pytest-logikal-1.7.0/entry_points.ini
--rw-r--r--   0 runner    (1001) docker     (122)     1985 2023-03-09 21:16:19.000000 pytest-logikal-1.7.0/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-09 21:16:49.041145 pytest-logikal-1.7.0/pytest_logikal/
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-03-09 21:16:19.000000 pytest-logikal-1.7.0/pytest_logikal/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)     2098 2023-03-09 21:16:19.000000 pytest-logikal-1.7.0/pytest_logikal/bandit.py
--rw-r--r--   0 runner    (1001) docker     (122)      181 2023-03-09 21:16:19.000000 pytest-logikal-1.7.0/pytest_logikal/bandit_config.yml
--rw-r--r--   0 runner    (1001) docker     (122)     7610 2023-03-09 21:16:19.000000 pytest-logikal-1.7.0/pytest_logikal/browser.py
--rw-r--r--   0 runner    (1001) docker     (122)     2103 2023-03-09 21:16:19.000000 pytest-logikal-1.7.0/pytest_logikal/build.py
--rw-r--r--   0 runner    (1001) docker     (122)     6462 2023-03-09 21:16:19.000000 pytest-logikal-1.7.0/pytest_logikal/core.py
--rw-r--r--   0 runner    (1001) docker     (122)      444 2023-03-09 21:16:19.000000 pytest-logikal-1.7.0/pytest_logikal/django.py
--rw-r--r--   0 runner    (1001) docker     (122)     1135 2023-03-09 21:16:19.000000 pytest-logikal-1.7.0/pytest_logikal/docs.py
--rw-r--r--   0 runner    (1001) docker     (122)     3339 2023-03-09 21:16:19.000000 pytest-logikal-1.7.0/pytest_logikal/file_checker.py
--rw-r--r--   0 runner    (1001) docker     (122)     1898 2023-03-09 21:16:19.000000 pytest-logikal-1.7.0/pytest_logikal/isort.py
--rw-r--r--   0 runner    (1001) docker     (122)     3587 2023-03-09 21:16:19.000000 pytest-logikal-1.7.0/pytest_logikal/licenses.py
--rw-r--r--   0 runner    (1001) docker     (122)     1767 2023-03-09 21:16:19.000000 pytest-logikal-1.7.0/pytest_logikal/plugin.py
--rw-r--r--   0 runner    (1001) docker     (122)        0 2023-03-09 21:16:19.000000 pytest-logikal-1.7.0/pytest_logikal/py.typed
--rw-r--r--   0 runner    (1001) docker     (122)     4662 2023-03-09 21:16:19.000000 pytest-logikal-1.7.0/pytest_logikal/pylint.py
--rw-r--r--   0 runner    (1001) docker     (122)     1396 2023-03-09 21:16:19.000000 pytest-logikal-1.7.0/pytest_logikal/requirements.py
--rw-r--r--   0 runner    (1001) docker     (122)     2240 2023-03-09 21:16:19.000000 pytest-logikal-1.7.0/pytest_logikal/style.py
--rw-r--r--   0 runner    (1001) docker     (122)     3888 2023-03-09 21:16:19.000000 pytest-logikal-1.7.0/pytest_logikal/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-09 21:16:49.041145 pytest-logikal-1.7.0/pytest_logikal.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     2462 2023-03-09 21:16:48.000000 pytest-logikal-1.7.0/pytest_logikal.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      969 2023-03-09 21:16:49.000000 pytest-logikal-1.7.0/pytest_logikal.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-03-09 21:16:48.000000 pytest-logikal-1.7.0/pytest_logikal.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)      458 2023-03-09 21:16:48.000000 pytest-logikal-1.7.0/pytest_logikal.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (122)      424 2023-03-09 21:16:48.000000 pytest-logikal-1.7.0/pytest_logikal.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       15 2023-03-09 21:16:48.000000 pytest-logikal-1.7.0/pytest_logikal.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-09 21:16:49.045146 pytest-logikal-1.7.0/requirements/
--rw-r--r--   0 runner    (1001) docker     (122)       27 2023-03-09 21:16:19.000000 pytest-logikal-1.7.0/requirements/build.txt
--rw-r--r--   0 runner    (1001) docker     (122)     1038 2023-03-09 21:16:19.000000 pytest-logikal-1.7.0/requirements/build.txt.lock
--rw-r--r--   0 runner    (1001) docker     (122)      327 2023-03-09 21:16:19.000000 pytest-logikal-1.7.0/requirements/core.txt
--rw-r--r--   0 runner    (1001) docker     (122)       58 2023-03-09 21:16:19.000000 pytest-logikal-1.7.0/requirements/dev.txt
--rw-r--r--   0 runner    (1001) docker     (122)     2541 2023-03-09 21:16:19.000000 pytest-logikal-1.7.0/requirements/dev.txt.lock
--rw-r--r--   0 runner    (1001) docker     (122)       60 2023-03-09 21:16:19.000000 pytest-logikal-1.7.0/requirements/docs.txt
--rw-r--r--   0 runner    (1001) docker     (122)     1816 2023-03-09 21:16:19.000000 pytest-logikal-1.7.0/requirements/docs.txt.lock
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-03-09 21:16:49.045146 pytest-logikal-1.7.0/requirements/extras/
--rw-r--r--   0 runner    (1001) docker     (122)       16 2023-03-09 21:16:19.000000 pytest-logikal-1.7.0/requirements/extras/browser.txt
--rw-r--r--   0 runner    (1001) docker     (122)       88 2023-03-09 21:16:19.000000 pytest-logikal-1.7.0/requirements/extras/django.txt
--rw-r--r--   0 runner    (1001) docker     (122)       38 2023-03-09 21:16:49.045146 pytest-logikal-1.7.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-05 11:07:40.673005 pytest-logikal-1.8.0/
+-rw-r--r--   0 runner    (1001) docker     (122)     1052 2023-05-05 11:07:16.000000 pytest-logikal-1.8.0/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       56 2023-05-05 11:07:16.000000 pytest-logikal-1.8.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)     2462 2023-05-05 11:07:40.673005 pytest-logikal-1.8.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      280 2023-05-05 11:07:16.000000 pytest-logikal-1.8.0/README.rst
+-rw-r--r--   0 runner    (1001) docker     (122)      217 2023-05-05 11:07:16.000000 pytest-logikal-1.8.0/compose.yml
+-rw-r--r--   0 runner    (1001) docker     (122)      626 2023-05-05 11:07:16.000000 pytest-logikal-1.8.0/entry_points.ini
+-rw-r--r--   0 runner    (1001) docker     (122)     2816 2023-05-05 11:07:16.000000 pytest-logikal-1.8.0/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-05 11:07:40.669005 pytest-logikal-1.8.0/pytest_logikal/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-05 11:07:16.000000 pytest-logikal-1.8.0/pytest_logikal/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2098 2023-05-05 11:07:16.000000 pytest-logikal-1.8.0/pytest_logikal/bandit.py
+-rw-r--r--   0 runner    (1001) docker     (122)      181 2023-05-05 11:07:16.000000 pytest-logikal-1.8.0/pytest_logikal/bandit_config.yml
+-rw-r--r--   0 runner    (1001) docker     (122)    12973 2023-05-05 11:07:16.000000 pytest-logikal-1.8.0/pytest_logikal/browser.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2228 2023-05-05 11:07:16.000000 pytest-logikal-1.8.0/pytest_logikal/build.py
+-rw-r--r--   0 runner    (1001) docker     (122)     8140 2023-05-05 11:07:16.000000 pytest-logikal-1.8.0/pytest_logikal/core.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2558 2023-05-05 11:07:16.000000 pytest-logikal-1.8.0/pytest_logikal/css.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3757 2023-05-05 11:07:16.000000 pytest-logikal-1.8.0/pytest_logikal/css_config.yml
+-rw-r--r--   0 runner    (1001) docker     (122)     3474 2023-05-05 11:07:16.000000 pytest-logikal-1.8.0/pytest_logikal/django.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3351 2023-05-05 11:07:16.000000 pytest-logikal-1.8.0/pytest_logikal/docker.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1135 2023-05-05 11:07:16.000000 pytest-logikal-1.8.0/pytest_logikal/docs.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3339 2023-05-05 11:07:16.000000 pytest-logikal-1.8.0/pytest_logikal/file_checker.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2948 2023-05-05 11:07:16.000000 pytest-logikal-1.8.0/pytest_logikal/html.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1898 2023-05-05 11:07:16.000000 pytest-logikal-1.8.0/pytest_logikal/isort.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1936 2023-05-05 11:07:16.000000 pytest-logikal-1.8.0/pytest_logikal/js.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5447 2023-05-05 11:07:16.000000 pytest-logikal-1.8.0/pytest_logikal/js_config.yml
+-rw-r--r--   0 runner    (1001) docker     (122)     4011 2023-05-05 11:07:16.000000 pytest-logikal-1.8.0/pytest_logikal/licenses.py
+-rw-r--r--   0 runner    (1001) docker     (122)    98728 2023-05-05 11:07:16.000000 pytest-logikal-1.8.0/pytest_logikal/package-lock.json
+-rw-r--r--   0 runner    (1001) docker     (122)      127 2023-05-05 11:07:16.000000 pytest-logikal-1.8.0/pytest_logikal/package.json
+-rw-r--r--   0 runner    (1001) docker     (122)     1801 2023-05-05 11:07:16.000000 pytest-logikal-1.8.0/pytest_logikal/plugin.py
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-05-05 11:07:16.000000 pytest-logikal-1.8.0/pytest_logikal/py.typed
+-rw-r--r--   0 runner    (1001) docker     (122)     4625 2023-05-05 11:07:16.000000 pytest-logikal-1.8.0/pytest_logikal/pylint.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1396 2023-05-05 11:07:16.000000 pytest-logikal-1.8.0/pytest_logikal/requirements.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2240 2023-05-05 11:07:16.000000 pytest-logikal-1.8.0/pytest_logikal/style.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1390 2023-05-05 11:07:16.000000 pytest-logikal-1.8.0/pytest_logikal/svg.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4371 2023-05-05 11:07:16.000000 pytest-logikal-1.8.0/pytest_logikal/utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2588 2023-05-05 11:07:16.000000 pytest-logikal-1.8.0/pytest_logikal/validator.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-05 11:07:40.669005 pytest-logikal-1.8.0/pytest_logikal.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     2462 2023-05-05 11:07:40.000000 pytest-logikal-1.8.0/pytest_logikal.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     1242 2023-05-05 11:07:40.000000 pytest-logikal-1.8.0/pytest_logikal.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-05 11:07:40.000000 pytest-logikal-1.8.0/pytest_logikal.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      626 2023-05-05 11:07:40.000000 pytest-logikal-1.8.0/pytest_logikal.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      540 2023-05-05 11:07:40.000000 pytest-logikal-1.8.0/pytest_logikal.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       15 2023-05-05 11:07:40.000000 pytest-logikal-1.8.0/pytest_logikal.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-05 11:07:40.673005 pytest-logikal-1.8.0/requirements/
+-rw-r--r--   0 runner    (1001) docker     (122)       27 2023-05-05 11:07:16.000000 pytest-logikal-1.8.0/requirements/build.txt
+-rw-r--r--   0 runner    (1001) docker     (122)     1038 2023-05-05 11:07:16.000000 pytest-logikal-1.8.0/requirements/build.txt.lock
+-rw-r--r--   0 runner    (1001) docker     (122)      342 2023-05-05 11:07:16.000000 pytest-logikal-1.8.0/requirements/core.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       58 2023-05-05 11:07:16.000000 pytest-logikal-1.8.0/requirements/dev.txt
+-rw-r--r--   0 runner    (1001) docker     (122)     2890 2023-05-05 11:07:16.000000 pytest-logikal-1.8.0/requirements/dev.txt.lock
+-rw-r--r--   0 runner    (1001) docker     (122)       60 2023-05-05 11:07:16.000000 pytest-logikal-1.8.0/requirements/docs.txt
+-rw-r--r--   0 runner    (1001) docker     (122)     1881 2023-05-05 11:07:16.000000 pytest-logikal-1.8.0/requirements/docs.txt.lock
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-05 11:07:40.673005 pytest-logikal-1.8.0/requirements/extras/
+-rw-r--r--   0 runner    (1001) docker     (122)       16 2023-05-05 11:07:16.000000 pytest-logikal-1.8.0/requirements/extras/browser.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      202 2023-05-05 11:07:16.000000 pytest-logikal-1.8.0/requirements/extras/django.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-05-05 11:07:40.673005 pytest-logikal-1.8.0/setup.cfg
```

### Comparing `pytest-logikal-1.7.0/LICENSE.txt` & `pytest-logikal-1.8.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pytest-logikal-1.7.0/PKG-INFO` & `pytest-logikal-1.8.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytest-logikal
-Version: 1.7.0
+Version: 1.8.0
 Summary: Common testing environment
 Author-email: Logikal GmbH <contact@logikal.io>
 License: Copyright 2022 Logikal GmbH
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and
         associated documentation files (the "Software"), to deal in the Software without restriction,
         including without limitation the rights to use, copy, modify, merge, publish, distribute,
```

### Comparing `pytest-logikal-1.7.0/pytest_logikal/bandit.py` & `pytest-logikal-1.8.0/pytest_logikal/bandit.py`

 * *Files identical despite different names*

### Comparing `pytest-logikal-1.7.0/pytest_logikal/build.py` & `pytest-logikal-1.8.0/pytest_logikal/build.py`

 * *Files 6% similar despite different names*

```diff
@@ -29,16 +29,19 @@
         process = subprocess.run(  # nosec: secure, not using untrusted input
             ['python3', '-m', 'build', '--sdist', '--wheel'],
             capture_output=True, text=True, check=False,
         )
         errors = (process.stderr or process.stdout) if process.returncode else process.stderr
         cleaned_errors = [
             error for error in (errors.strip().split('\n') if errors else [])
-            if '_BetaConfiguration' not in error and 'warnings.warn(' not in error
+            # Remove unnecessary warnings from output
+            if '_BetaConfiguration' not in error
+            and 'warnings.warn(' not in error
             and 'shallow and may cause errors' not in error
+            and 'config = read_configuration' not in error
         ]
         if cleaned_errors:
             raise ItemRunError('\n'.join(cleaned_errors))
 
         # Checking distribution
         process = subprocess.run(  # nosec: secure, not using untrusted input
             ['twine', 'check', '--strict', 'dist/*'], capture_output=True, text=True, check=False,
```

### Comparing `pytest-logikal-1.7.0/pytest_logikal/core.py` & `pytest-logikal-1.8.0/pytest_logikal/core.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,30 +1,38 @@
 import logging
 import os
 import shutil
+import subprocess
 import sys
 from importlib.util import find_spec
+from itertools import chain
 from pathlib import Path
-from typing import Callable, Dict, Iterator, List, Optional, Tuple, Union
+from typing import Any, Callable, Dict, Iterator, List, Optional, Tuple, Union
 
 import pytest
 import tomli
+from termcolor import colored
 
 sys.path.insert(0, os.getcwd())
 
 PYPROJECT = (
     tomli.loads(Path('pyproject.toml').read_text(encoding='utf-8'))
     if Path('pyproject.toml').exists() else {}
 )
-PLUGINS = [
-    'mypy', 'bandit', 'build', 'docs', 'isort', 'licenses', 'pylint', 'requirements', 'style',
-]
-DEFAULT_MAX_LINE_LENGTH = 99
-DEFAULT_MAX_COMPLEXITY = 10
-DEFAULT_MIN_COVERAGE = 100
+PLUGINS = {
+    'core': [
+        'mypy', 'bandit', 'build', 'docs', 'isort', 'licenses', 'pylint', 'requirements', 'style',
+    ],
+    'django': ['django', 'html', 'css', 'svg', 'js'],
+}
+DEFAULT_INI_OPTIONS: Dict[str, Any] = {
+    'max_line_length': {'value': 99, 'help': 'the maximum line length to use'},
+    'max_complexity': {'value': 10, 'help': 'the maximum complexity to allow'},
+    'cov_fail_under': {'value': 100, 'help': 'target coverage percentage'},
+}
 
 ReportInfoType = Tuple[Union[os.PathLike, str], Optional[int], str]
 
 
 def pytest_addoption(parser: pytest.Parser) -> None:
     group = parser.getgroup('logikal')
     group.addoption('--live', action='store_true', help='run live tests')
@@ -36,27 +44,30 @@
     group.addoption('--no-build', action='store_true', help='do not run build checks')
     group.addoption('--no-docs', action='store_true', help='do not run documentation checks')
     group.addoption('--no-isort', action='store_true', help='do not use isort')
     group.addoption('--no-licenses', action='store_true', help='do not check licenses')
     group.addoption('--no-pylint', action='store_true', help='do not use pylint')
     group.addoption('--no-requirements', action='store_true', help='do not check requirements')
     group.addoption('--no-style', action='store_true', help='do not use pycodestyle & pydocstyle')
-    parser.addini('max_line_length', default=str(DEFAULT_MAX_LINE_LENGTH),
-                  help='the maximum line length to use')
-    parser.addini('max_complexity', default=str(DEFAULT_MAX_COMPLEXITY),
-                  help='the maximum complexity to allow')
-    parser.addini('cov_fail_under', default=str(DEFAULT_MIN_COVERAGE),
-                  help='target coverage percentage')
+    group.addoption('--no-django', action='store_true', help='do not run django migration checks')
+    group.addoption('--no-html', action='store_true', help='do not run html template checks')
+    group.addoption('--no-css', action='store_true', help='do not run css checks')
+    group.addoption('--no-svg', action='store_true', help='do not run svg checks')
+    group.addoption('--no-js', action='store_true', help='do not run js checks')
+    group.addoption('--no-install', action='store_true', help='do not install packages')
+    for option, entry in DEFAULT_INI_OPTIONS.items():
+        parser.addini(option, default=str(entry['value']), help=entry['help'])
 
 
 def pytest_addhooks(pluginmanager: pytest.PytestPluginManager) -> None:
     if not find_spec('selenium'):
         pluginmanager.set_blocked('logikal_browser')
     if not find_spec('pytest_django'):
-        pluginmanager.set_blocked('logikal_django')
+        for plugin in PLUGINS['django']:
+            pluginmanager.set_blocked(f'logikal_{plugin}')
 
 
 # Untyped decorator (see https://github.com/pytest-dev/pytest/issues/7469)
 @pytest.hookimpl(hookwrapper=True)  # type: ignore[misc]
 def pytest_load_initial_conftests(early_config: pytest.Config, args: List[str]) -> Iterator[None]:
     if '--no-defaults' in args:
         yield
@@ -71,15 +82,15 @@
         args.append('--cache-clear')
         namespace.cacheclear = True
     if '-r' not in args:
         args.extend(['-r', 'fExX'])
     if '-n' not in args:
         args.extend(['-n', 'auto' if '--live' not in args else '0'])
         namespace.dist = 'load' if '--live' not in args else 'no'
-    for plugin in PLUGINS:
+    for plugin in chain.from_iterable(PLUGINS.values()):
         if '--fast' not in args and f'--no-{plugin}' not in args:
             args.append(f'--{plugin}')
             setattr(namespace, plugin, True)
     if all(arg not in args for arg in ['--cov', '--no-cov', '--live', '--fast']):
         args.extend(['--cov', '--no-cov-on-fail'])
         namespace.no_cov_on_fail = True
 
@@ -101,28 +112,47 @@
         'log_date_format': '%Y-%m-%d %H:%M:%S',
         'log_auto_indent': 'True',
     }
     early_config.inicfg = {**ini_defaults, **early_config.inicfg}
     yield
 
 
+def install_packages(node_prefix: Optional[Path] = None) -> None:
+    node_prefix = node_prefix or Path(__file__).parent
+    if not (node_prefix / 'node_modules').exists():
+        print(colored('Installing Node.js packages', attrs=['bold']))
+        command = ['npm', 'install', '--no-save', '--prefix', str(node_prefix)]
+        subprocess.run(command, text=True, check=True)  # nosec: secure, not using untrusted input
+
+
 def pytest_configure(config: pytest.Config) -> None:
+    # Installing Node.js packages
+    if find_spec('pytest_django') and not config.getoption('no_install'):
+        install_packages()
+
     # Clearing cache
     if config.getoption('clear'):
-        print('Clearing cache')
+        print(colored('Clearing cache', 'yellow', attrs=['bold']))
         Path('.coverage').unlink(missing_ok=True)
         shutil.rmtree('.pytest_cache', ignore_errors=True)
         shutil.rmtree('.mypy_cache', ignore_errors=True)
 
     # Hiding overly verbose debug and info log messages
-    logging.getLogger('faker').setLevel(logging.INFO)
-    logging.getLogger('filelock').setLevel(logging.WARNING)
-    logging.getLogger('PIL').setLevel(logging.INFO)
-    logging.getLogger('pydocstyle').setLevel(logging.WARNING)
-    logging.getLogger('matplotlib').setLevel(logging.INFO)
+    if not config.getoption('verbose'):
+        logging.getLogger('faker').setLevel(logging.INFO)
+        logging.getLogger('filelock').setLevel(logging.WARNING)
+        logging.getLogger('PIL').setLevel(logging.INFO)
+        logging.getLogger('pydocstyle').setLevel(logging.WARNING)
+        logging.getLogger('matplotlib').setLevel(logging.INFO)
+        logging.getLogger('django_migration_linter').setLevel(logging.WARNING)
+
+        # Hiding validator log messages
+        logging.getLogger('docker').setLevel(logging.INFO)
+        logging.getLogger('urllib3').setLevel(logging.INFO)
+        logging.getLogger('pytest_logikal.validator').setLevel(logging.INFO)
 
     # Hiding worker information lines
     if not config.getoption('verbose'):
         config.pluginmanager.get_plugin('reports').getworkerinfoline = lambda *_args, **_kwargs: ''
 
     # Configuring mypy
     mypy = config.pluginmanager.get_plugin('mypy')
```

### Comparing `pytest-logikal-1.7.0/pytest_logikal/docs.py` & `pytest-logikal-1.8.0/pytest_logikal/docs.py`

 * *Files identical despite different names*

### Comparing `pytest-logikal-1.7.0/pytest_logikal/file_checker.py` & `pytest-logikal-1.8.0/pytest_logikal/file_checker.py`

 * *Files identical despite different names*

### Comparing `pytest-logikal-1.7.0/pytest_logikal/isort.py` & `pytest-logikal-1.8.0/pytest_logikal/isort.py`

 * *Files identical despite different names*

### Comparing `pytest-logikal-1.7.0/pytest_logikal/licenses.py` & `pytest-logikal-1.8.0/pytest_logikal/licenses.py`

 * *Files 8% similar despite different names*

```diff
@@ -6,35 +6,41 @@
 
 from pytest_logikal.core import PYPROJECT, ReportInfoType
 from pytest_logikal.plugin import Item, ItemRunError, Plugin
 
 ALLOWED_LICENSES = [
     '3-Clause BSD License',
     'Apache 2.0',
+    'Apache License 2.0',
     'Apache Software License',
     'BSD 3-Clause',
     'BSD License',
     'BSD',
     'BSD-3-Clause',
     'GNU Lesser General Public License v2 (LGPLv2)',
     'GNU Lesser General Public License v2 or later (LGPLv2+)',
+    'GNU Lesser General Public License v3 (LGPLv3)',
+    'GNU Library or Lesser General Public License (LGPL)',
     'ISC License (ISCL)',
     'ISC',
     'MIT License',
     'MIT No Attribution License (MIT-0)',
     'MIT',
     'Mozilla Public License 2.0 (MPL 2.0)',
     'Public Domain',
     'Python Software Foundation License',
     'The MIT License (MIT)',
     'The Unlicense (Unlicense)',
 ]
 
 ALLOWED_PACKAGES = {
     'facebook-business': 'LICENSE.txt',  # only used as a connector
+    'djlint': 'GNU General Public License v3 or later (GPLv3+)',  # only used as a local tool
+    'html-tag-names': 'GNU General Public License v3 or later (GPLv3+)',  # djlint dependency
+    'html-void-elements': 'GNU General Public License v3 or later (GPLv3+)',  # djlint dependency
     'pkg_resources': 'UNKNOWN',  # caused by an Ubuntu bug, see [1]
     'pkg-resources': 'UNKNOWN',  # caused by an Ubuntu bug, see [1]
     'Pillow': 'Historical Permission Notice and Disclaimer (HPND)',  # license is BSD-like
     'pylint': 'GNU General Public License v2 (GPLv2)',  # only used as a local tool
     'pylint-django': 'GPLv2',  # only used as a local tool plugin
     'pylint-plugin-utils': 'GPLv2',  # only used as a local tool plugin
     'python-lsp-jsonrpc': 'UNKNOWN',  # license is MIT
```

### Comparing `pytest-logikal-1.7.0/pytest_logikal/plugin.py` & `pytest-logikal-1.8.0/pytest_logikal/plugin.py`

 * *Files 11% similar despite different names*

```diff
@@ -44,17 +44,15 @@
             raise AttributeError('You must provide a plugin name')
         if not hasattr(self, 'item'):
             raise AttributeError('You must provide an item type')
 
         self.config = config
 
     def pytest_collect_file(self, parent: pytest.Collector) -> Any:
-        """
-        Run a single test.
-        """
         plugin = self
 
         class File(pytest.File):
             def collect(self) -> Iterable[Item]:
-                if not any(isinstance(item, type(item)) for item in self.session.items):
+                # Ensure that a plugin item is added once and only once per session
+                if not any(isinstance(item, plugin.item) for item in self.session.items):
                     yield plugin.item.from_parent(parent=self, name=plugin.name)
         return File.from_parent(parent, path=Path('check'))
```

### Comparing `pytest-logikal-1.7.0/pytest_logikal/pylint.py` & `pytest-logikal-1.8.0/pytest_logikal/pylint.py`

 * *Files 1% similar despite different names*

```diff
@@ -66,15 +66,15 @@
             'consider-using-namedtuple-or-dataclass',  # unnamed tuples can be sometimes useful
         ]
         if 'DJANGO_SETTINGS_MODULE' in self.config.inicfg:
             disable += [
                 'too-few-public-methods',  # common error with some Django classes
                 'unsubscriptable-object',  # common error with generic types in django-stubs
             ]
-            plugins += ['pylint_django', 'pylint_django.checkers.migrations']
+            plugins += ['pylint_django']
             command += [
                 f'--django-settings-module={self.config.inicfg["DJANGO_SETTINGS_MODULE"]}',
                 r'--module-rgx=[^\WA-Z]*$',  # allow (migration) modules to start with digits
             ]
 
         pyproject_pylint = PYPROJECT.get('tool', {}).get('pylint', {}).get('messages_control', {})
         enable = pyproject_pylint.get('enable', enable)
```

### Comparing `pytest-logikal-1.7.0/pytest_logikal/requirements.py` & `pytest-logikal-1.8.0/pytest_logikal/requirements.py`

 * *Files identical despite different names*

### Comparing `pytest-logikal-1.7.0/pytest_logikal/style.py` & `pytest-logikal-1.8.0/pytest_logikal/style.py`

 * *Files identical despite different names*

### Comparing `pytest-logikal-1.7.0/pytest_logikal/utils.py` & `pytest-logikal-1.8.0/pytest_logikal/utils.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,36 +1,48 @@
 import sys
+from contextlib import contextmanager
 from io import BytesIO
 from logging import getLogger
 from operator import methodcaller
 from os import getcwd
 from pathlib import Path
 from shutil import copy
 from subprocess import run
-from typing import Any, Callable, Optional, Type, TypeVar
+from tempfile import TemporaryDirectory
+from typing import Any, Callable, Dict, Generator, Optional, Type, TypeVar
 
 from PIL import Image, ImageChops
 
-from pytest_logikal.core import DEFAULT_MAX_LINE_LENGTH, PYPROJECT
+from pytest_logikal.core import DEFAULT_INI_OPTIONS, PYPROJECT
 
 logger = getLogger(__name__)
 
 Function = TypeVar('Function', bound=Callable[..., Any])
 
 
-def get_max_line_length() -> int:
+def get_ini_option(name: str) -> Any:
     ini_options = PYPROJECT.get('tool', {}).get('pytest', {}).get('ini_options', {})
-    return int(ini_options.get('max_line_length', DEFAULT_MAX_LINE_LENGTH))
+    default = DEFAULT_INI_OPTIONS[name]['value']
+    return type(default)(ini_options.get(name, default))
 
 
 def hide_traceback(function: Function, error: Type[Exception] = AssertionError) -> Function:
     getattr(function, '__globals__')['__tracebackhide__'] = methodcaller('errisinstance', error)
     return function
 
 
+@contextmanager
+def render_template(path: Path, context: Dict[str, Any]) -> Generator[Path, None, None]:
+    with TemporaryDirectory(prefix='pytest_logikal_') as tmp_dir:
+        rendered = path.read_text(encoding='utf-8').format(**context)
+        config_path = Path(tmp_dir) / path.name
+        config_path.write_text(rendered)
+        yield config_path
+
+
 @hide_traceback
 def assert_image_equal(actual: bytes, expected: Path, temp_path: Path) -> None:
     temp_actual_path = temp_path / 'actual.png'
     temp_expected_path = temp_path / 'expected.png'
     temp_diff_path = temp_path / 'diff.png'
 
     logger.info(f'Checking expected image in "{expected}"')
```

### Comparing `pytest-logikal-1.7.0/pytest_logikal.egg-info/PKG-INFO` & `pytest-logikal-1.8.0/pytest_logikal.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytest-logikal
-Version: 1.7.0
+Version: 1.8.0
 Summary: Common testing environment
 Author-email: Logikal GmbH <contact@logikal.io>
 License: Copyright 2022 Logikal GmbH
         
         Permission is hereby granted, free of charge, to any person obtaining a copy of this software and
         associated documentation files (the "Software"), to deal in the Software without restriction,
         including without limitation the rights to use, copy, modify, merge, publish, distribute,
```

### Comparing `pytest-logikal-1.7.0/pytest_logikal.egg-info/SOURCES.txt` & `pytest-logikal-1.8.0/pytest_logikal.egg-info/SOURCES.txt`

 * *Files 27% similar despite different names*

```diff
@@ -1,29 +1,40 @@
 LICENSE.txt
 MANIFEST.in
 README.rst
+compose.yml
 entry_points.ini
 pyproject.toml
 pytest_logikal/__init__.py
 pytest_logikal/bandit.py
 pytest_logikal/bandit_config.yml
 pytest_logikal/browser.py
 pytest_logikal/build.py
 pytest_logikal/core.py
+pytest_logikal/css.py
+pytest_logikal/css_config.yml
 pytest_logikal/django.py
+pytest_logikal/docker.py
 pytest_logikal/docs.py
 pytest_logikal/file_checker.py
+pytest_logikal/html.py
 pytest_logikal/isort.py
+pytest_logikal/js.py
+pytest_logikal/js_config.yml
 pytest_logikal/licenses.py
+pytest_logikal/package-lock.json
+pytest_logikal/package.json
 pytest_logikal/plugin.py
 pytest_logikal/py.typed
 pytest_logikal/pylint.py
 pytest_logikal/requirements.py
 pytest_logikal/style.py
+pytest_logikal/svg.py
 pytest_logikal/utils.py
+pytest_logikal/validator.py
 pytest_logikal.egg-info/PKG-INFO
 pytest_logikal.egg-info/SOURCES.txt
 pytest_logikal.egg-info/dependency_links.txt
 pytest_logikal.egg-info/entry_points.txt
 pytest_logikal.egg-info/requires.txt
 pytest_logikal.egg-info/top_level.txt
 requirements/build.txt
```

### Comparing `pytest-logikal-1.7.0/requirements/build.txt.lock` & `pytest-logikal-1.8.0/requirements/build.txt.lock`

 * *Files identical despite different names*

### Comparing `pytest-logikal-1.7.0/requirements/dev.txt.lock` & `pytest-logikal-1.8.0/requirements/dev.txt.lock`

 * *Files 12% similar despite different names*

```diff
@@ -1,127 +1,145 @@
 ###################################################################################################
 ##
 ##  DO NOT EDIT THIS FILE.
 ##  This is a locked requirements file generated by pyorbs.
 ##
-##  Requirements hash: 70f43f4b31b3993e603ac683b2b5ac21591cab9dea5e1afe03ce962cb699aab9
+##  Requirements hash: 123e0923c12ca1679b00a6caddf9ddb565dc2ff87aef5e10a2dd2bcb172f2024
 ##
 ###################################################################################################
 -e .
 alabaster==0.7.13
+appdirs==1.4.4
 asgiref==3.6.0
-astroid==2.14.2
+astroid==2.15.4
 async-generator==1.10
-attrs==22.2.0
+attrs==23.1.0
 Babel==2.12.1
 backports.zoneinfo==0.2.1
-bandit==1.7.4
+bandit==1.7.5
 bleach==6.0.0
 build==0.10.0
 certifi==2022.12.7
 cffi==1.15.1
-charset-normalizer==3.0.1
+charset-normalizer==3.1.0
+click==8.1.3
 colorama==0.4.6
-coverage==7.2.1
-cryptography==39.0.1
+coverage==7.2.5
+cryptography==40.0.2
+cssbeautifier==1.14.7
 dill==0.3.6
-Django==4.1.7
-django-stubs==1.15.0
-django-stubs-ext==0.7.0
+Django==4.2.1
+django-migration-linter==4.1.0
+django-stubs==4.2.0
+django-stubs-ext==4.2.0
+djlint==1.25.0
+docker==6.0.1
 docutils==0.17.1
-exceptiongroup==1.1.0
+EditorConfig==0.12.3
+exceptiongroup==1.1.1
 execnet==1.9.0
 factory-boy==3.2.1
-Faker==17.3.0
-filelock==3.9.0
+Faker==18.6.2
+filelock==3.12.0
 gitdb==4.0.10
 GitPython==3.1.31
 h11==0.14.0
+html-tag-names==0.1.2
+html-void-elements==0.1.0
 idna==3.4
 imagesize==1.4.1
-importlib-metadata==6.0.0
+importlib-metadata==6.6.0
 importlib-resources==5.12.0
 inflection==0.5.1
 iniconfig==2.0.0
 isort==5.12.0
 jaraco.classes==3.2.3
 jeepney==0.8.0
 Jinja2==3.1.2
+jsbeautifier==1.14.7
 keyring==23.13.1
 lazy-object-proxy==1.9.0
 logikal-docs==1.1.3
 markdown-it-py==2.2.0
 MarkupSafe==2.1.2
 mccabe==0.7.0
 mdurl==0.1.2
 more-itertools==9.1.0
-mypy==1.0.1
+mypy==1.2.0
 mypy-extensions==1.0.0
 outcome==1.2.0
-packaging==23.0
+packaging==23.1
+pathspec==0.11.1
 pbr==5.11.1
-Pillow==9.4.0
-pip==23.0.1
-pip-licenses==4.0.3
+Pillow==9.5.0
+pip==23.1.2
+pip-licenses==4.3.0
 pkginfo==1.9.6
-platformdirs==3.0.0
+platformdirs==3.5.0
 pluggy==1.0.0
-prettytable==3.6.0
-psutil==5.9.4
+prettytable==3.7.0
+psutil==5.9.5
 pycodestyle==2.10.0
 pycparser==2.21
 pydocstyle==6.3.0
-Pygments==2.14.0
-pylint==2.16.2
+Pygments==2.15.1
+pylint==2.17.3
 pylint-django==2.5.3
 pylint-plugin-utils==0.7
 pyorbs==2.0.0
 pyproject_hooks==1.0.0
 PySocks==1.7.1
-pytest==7.2.1
+pytest==7.3.1
 pytest-cov==4.0.0
 pytest-django==4.5.2
 pytest-factoryboy==2.5.1
 pytest-mock==3.10.0
 pytest-mypy==0.10.3
-pytest-xdist==3.2.0
+pytest-xdist==3.2.1
 python-dateutil==2.8.2
-pytz==2022.7.1
+pytz==2023.3
 PyYAML==6.0
 readme-renderer==37.3
-requests==2.28.2
-requests-toolbelt==0.10.1
+regex==2023.5.5
+requests==2.30.0
+requests-toolbelt==1.0.0
 rfc3986==2.0.0
-rich==13.3.1
+rich==13.3.5
 SecretStorage==3.3.3
-selenium==4.8.2
-setuptools==67.4.0
+selenium==4.9.0
+setuptools==67.7.2
 six==1.16.0
 smmap==5.0.0
 sniffio==1.3.0
 snowballstemmer==2.2.0
 sortedcontainers==2.4.0
 Sphinx==5.3.0
 sphinx-rtd-theme==1.1.1
 sphinxcontrib-applehelp==1.0.4
 sphinxcontrib-devhelp==1.0.2
 sphinxcontrib-htmlhelp==2.0.1
 sphinxcontrib-jsmath==1.0.1
 sphinxcontrib-qthelp==1.0.3
 sphinxcontrib-serializinghtml==1.1.5
-sqlparse==0.4.3
+sqlparse==0.4.4
 stevedore==5.0.0
+termcolor==2.3.0
+toml==0.10.2
 tomli==2.0.1
-tomlkit==0.11.6
+tomlkit==0.11.8
+tqdm==4.65.0
 trio==0.22.0
-trio-websocket==0.9.2
+trio-websocket==0.10.2
 twine==4.0.2
-types-pytz==2022.7.1.2
-types-PyYAML==6.0.12.8
+types-pytz==2023.3.0.0
+types-PyYAML==6.0.12.9
+types-requests==2.29.0.0
+types-urllib3==1.26.25.12
 typing_extensions==4.5.0
-urllib3==1.26.14
+urllib3==1.26.15
 wcwidth==0.2.6
 webencodings==0.5.1
-wheel==0.38.4
+websocket-client==1.5.1
+wheel==0.40.0
 wrapt==1.15.0
 wsproto==1.2.0
 zipp==3.15.0
```

### Comparing `pytest-logikal-1.7.0/requirements/docs.txt.lock` & `pytest-logikal-1.8.0/requirements/docs.txt.lock`

 * *Files 11% similar despite different names*

```diff
@@ -1,89 +1,93 @@
 ###################################################################################################
 ##
 ##  DO NOT EDIT THIS FILE.
 ##  This is a locked requirements file generated by pyorbs.
 ##
-##  Requirements hash: 2eb891c05ab2fcff025a7ba67046951e20ab06294e9e4493f31a03aee349ebc4
+##  Requirements hash: bec45cef2a84abf1e23a4c575600549fc6d8ff56c4bf8627cf1c3dd1a58a25f9
 ##
 ###################################################################################################
 -e .
 alabaster==0.7.13
-astroid==2.14.2
+astroid==2.15.4
 async-generator==1.10
-attrs==22.2.0
+attrs==23.1.0
 Babel==2.12.1
-bandit==1.7.4
+bandit==1.7.5
 certifi==2022.12.7
-charset-normalizer==3.0.1
+charset-normalizer==3.1.0
 colorama==0.4.6
-coverage==7.2.1
+coverage==7.2.5
 dill==0.3.6
 docutils==0.17.1
-exceptiongroup==1.1.0
+exceptiongroup==1.1.1
 execnet==1.9.0
-filelock==3.9.0
+filelock==3.12.0
 gitdb==4.0.10
 GitPython==3.1.31
 h11==0.14.0
 idna==3.4
 imagesize==1.4.1
-importlib-metadata==6.0.0
+importlib-metadata==6.6.0
 iniconfig==2.0.0
 isort==5.12.0
 Jinja2==3.1.2
 lazy-object-proxy==1.9.0
 logikal-docs==1.1.3
+markdown-it-py==2.2.0
 MarkupSafe==2.1.2
 mccabe==0.7.0
-mypy==1.0.1
+mdurl==0.1.2
+mypy==1.2.0
 mypy-extensions==1.0.0
 outcome==1.2.0
-packaging==23.0
+packaging==23.1
 pbr==5.11.1
-Pillow==9.4.0
-pip==23.0.1
-pip-licenses==4.0.3
-platformdirs==3.0.0
+Pillow==9.5.0
+pip==23.1.2
+pip-licenses==4.3.0
+platformdirs==3.5.0
 pluggy==1.0.0
-prettytable==3.6.0
-psutil==5.9.4
+prettytable==3.7.0
+psutil==5.9.5
 pycodestyle==2.10.0
 pydocstyle==6.3.0
-Pygments==2.14.0
-pylint==2.16.2
+Pygments==2.15.1
+pylint==2.17.3
 pyorbs==2.0.0
 PySocks==1.7.1
-pytest==7.2.1
+pytest==7.3.1
 pytest-cov==4.0.0
 pytest-mock==3.10.0
 pytest-mypy==0.10.3
-pytest-xdist==3.2.0
-pytz==2022.7.1
+pytest-xdist==3.2.1
+pytz==2023.3
 PyYAML==6.0
-requests==2.28.2
-selenium==4.8.2
-setuptools==67.4.0
+requests==2.30.0
+rich==13.3.5
+selenium==4.9.0
+setuptools==67.7.2
 smmap==5.0.0
 sniffio==1.3.0
 snowballstemmer==2.2.0
 sortedcontainers==2.4.0
 Sphinx==5.3.0
 sphinx-rtd-theme==1.1.1
 sphinxcontrib-applehelp==1.0.4
 sphinxcontrib-devhelp==1.0.2
 sphinxcontrib-htmlhelp==2.0.1
 sphinxcontrib-jsmath==1.0.1
 sphinxcontrib-qthelp==1.0.3
 sphinxcontrib-serializinghtml==1.1.5
 stevedore==5.0.0
+termcolor==2.3.0
 tomli==2.0.1
-tomlkit==0.11.6
+tomlkit==0.11.8
 trio==0.22.0
-trio-websocket==0.9.2
+trio-websocket==0.10.2
 typing_extensions==4.5.0
-urllib3==1.26.14
+urllib3==1.26.15
 wcwidth==0.2.6
-wheel==0.38.4
+wheel==0.40.0
 wrapt==1.15.0
 wsproto==1.2.0
 zipp==3.15.0
```

