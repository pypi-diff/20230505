# Comparing `tmp/katalytic-data-0.7.1.tar.gz` & `tmp/katalytic-data-0.8.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "katalytic-data-0.7.1.tar", last modified: Sun Apr 30 05:44:06 2023, max compression
+gzip compressed data, was "katalytic-data-0.8.0.tar", last modified: Fri May  5 17:31:25 2023, max compression
```

## Comparing `katalytic-data-0.7.1.tar` & `katalytic-data-0.8.0.tar`

### file list

```diff
@@ -1,10 +1,12 @@
--rw-r--r--   0        0        0       87 2023-04-16 12:25:23.268033 katalytic-data-0.7.1/.coveragerc
--rw-r--r--   0        0        0      651 2023-04-26 18:43:19.705157 katalytic-data-0.7.1/.gitignore
--rw-r--r--   0        0        0     3109 2023-04-27 17:15:54.916636 katalytic-data-0.7.1/.gitlab-ci.yml
--rw-r--r--   0        0        0    12580 2023-04-30 05:44:02.196844 katalytic-data-0.7.1/CHANGELOG.md
--rw-r--r--   0        0        0     1066 2023-04-16 12:25:23.268033 katalytic-data-0.7.1/LICENSE.txt
--rw-r--r--   0        0        0     2083 2023-04-16 12:25:23.268033 katalytic-data-0.7.1/README.md
--rw-r--r--   0        0        0     1245 2023-04-30 05:44:02.192844 katalytic-data-0.7.1/pyproject.toml
--rw-r--r--   0        0        0    21404 2023-04-30 05:34:31.790368 katalytic-data-0.7.1/src/katalytic/data.py
--rw-r--r--   0        0        0    41638 2023-04-30 05:38:20.462596 katalytic-data-0.7.1/tests/test_data.py
--rw-r--r--   0        0        0     3167 1970-01-01 00:00:00.000000 katalytic-data-0.7.1/PKG-INFO
+-rw-r--r--   0        0        0       87 2023-04-16 12:25:23.268033 katalytic-data-0.8.0/.coveragerc
+-rw-r--r--   0        0        0      651 2023-04-26 18:43:19.705157 katalytic-data-0.8.0/.gitignore
+-rw-r--r--   0        0        0     3242 2023-05-05 03:59:46.034609 katalytic-data-0.8.0/.gitlab-ci.yml
+-rw-r--r--   0        0        0    12893 2023-05-05 17:31:03.370151 katalytic-data-0.8.0/CHANGELOG.md
+-rw-r--r--   0        0        0     1066 2023-04-16 12:25:23.268033 katalytic-data-0.8.0/LICENSE.txt
+-rw-r--r--   0        0        0     1836 2023-04-30 14:20:58.779511 katalytic-data-0.8.0/README.md
+-rw-r--r--   0        0        0     1236 2023-05-05 17:31:03.342151 katalytic-data-0.8.0/pyproject.toml
+-rw-r--r--   0        0        0    21439 2023-05-05 10:55:06.685464 katalytic-data-0.8.0/src/katalytic/data/__init__.py
+-rw-r--r--   0        0        0     6192 2023-05-05 10:53:33.309343 katalytic-data-0.8.0/src/katalytic/data/checks.py
+-rw-r--r--   0        0        0    17113 2023-05-05 11:04:41.773899 katalytic-data-0.8.0/tests/test_checks.py
+-rw-r--r--   0        0        0    41654 2023-05-05 10:54:38.837287 katalytic-data-0.8.0/tests/test_data.py
+-rw-r--r--   0        0        0     2928 1970-01-01 00:00:00.000000 katalytic-data-0.8.0/PKG-INFO
```

### Comparing `katalytic-data-0.7.1/.gitignore` & `katalytic-data-0.8.0/.gitignore`

 * *Files identical despite different names*

### Comparing `katalytic-data-0.7.1/.gitlab-ci.yml` & `katalytic-data-0.8.0/.gitlab-ci.yml`

 * *Files 6% similar despite different names*

```diff
@@ -1,35 +1,39 @@
 include:
 - template: Security/SAST.gitlab-ci.yml
 
-image: python:3.9
+image: python:3.6
 
 stages:
   - coverage
   - test
   - security
   - release
 
 variables:
-  TOX_ENV: py39
   PIP_DISABLE_PIP_VERSION_CHECK: "1"
   PIP_NO_CACHE_DIR: "off"
 
-test_cov:
+coverage:
   image: python:3.6
   stage: coverage
   script:
     - pip install --upgrade pip
-    - pip install pytest pytest-cov pytest-randomly
-    - pip install -e .
-    - python -m pytest --cov-fail-under=100 --cov=src --cov-report term-missing || { echo "Tests failed. Exiting ..." && exit 1; }
+    - pip install -e .[dev]
+    - python -m pytest --cov-fail-under=100 --cov=src --cov-report=xml --cov-report=term-missing || { echo "Tests failed. Exiting ..." && exit 1; }
   rules:
     - if: '$CI_COMMIT_MESSAGE =~ /(feat|fix|refactor|perf|test|chore|style)/i'
       when: always
     - when: never
+  coverage: /(?i)total.*? (100(?:\.0+)?\%|[1-9]?\d(?:\.\d+)?\%)$/
+  artifacts:
+    reports:
+      coverage_report:
+        coverage_format: cobertura
+        path: "coverage.xml"
   allow_failure: false
 
 
 # test_py36:
 #   image: python:3.6
 #   stage: test
 #   script:
```

### Comparing `katalytic-data-0.7.1/CHANGELOG.md` & `katalytic-data-0.8.0/CHANGELOG.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,7 +1,14 @@
+## 0.8.0 (2023-05-05)
+### feat
+- [[`ae032f2`](https://gitlab.com/katalytic/katalytic-data/commit/ae032f23cf8e387387833a0648184ca6095bf9ed)] move katalytic-checks code into this repo
+### fix
+- [[`ddc044f`](https://gitlab.com/katalytic/katalytic-data/commit/ddc044f3bdf1a872306cfbb090843e220d7222f5)] all_types()
+
+
 ## 0.7.1 (2023-04-30)
 ### fix
 - [[`5a06ff8`](https://gitlab.com/katalytic/katalytic-data/commit/5a06ff8ee54e58e502c18fee5723bad8c4bf702a)] add missing categories of types and extend the tests
 
 
 ## 0.7.0 (2023-04-30)
 ### feat
```

### Comparing `katalytic-data-0.7.1/LICENSE.txt` & `katalytic-data-0.8.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `katalytic-data-0.7.1/README.md` & `katalytic-data-0.8.0/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 ## Description
 TODO: Let people know what your project can do specifically. Provide context and add a link to any reference visitors might be unfamiliar with. A list of Features or a Background subsection can also be added here. If there are alternatives to your project, this is a good place to list differentiating factors.
 
 [![version](https://img.shields.io/pypi/v/katalytic-data)](https://pypi.org/project/katalytic-data/)
-[![Build Status](https://app.travis-ci.com/katalytic/katalytic-data.svg?branch=main)](https://app.travis-ci.com/gitlab/katalytic/katalytic-data)
-[![Test Results](https://img.shields.io/travis/com/katalytic/katalytic-data?label=tests)](https://app.travis-ci.com/gitlab/katalytic/katalytic-data)
-[![Coverage Status](https://coveralls.io/repos/gitlab/katalytic/katalytic-data/badge.svg?branch=main)](https://coveralls.io/gitlab/katalytic/katalytic-data?branch=main)
-[![Docs Coverage](https://img.shields.io/readthedocs/katalytic-data.svg)](https://katalytic-data.readthedocs.io/en/latest/)
-[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
+[![tests](https://gitlab.com/katalytic/katalytic-data/badges/main/pipeline.svg?key_text=tests&key_width=38)](https://gitlab.com/katalytic/katalytic-data/-/commits/main)
+[![coverage](https://gitlab.com/katalytic/katalytic-data/badges/main/coverage.svg)](https://gitlab.com/katalytic/katalytic-data/-/commits/main)
+[![docs](https://img.shields.io/readthedocs/katalytic-data.svg)](https://katalytic-data.readthedocs.io/en/latest/)
+[![license: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
 
 ## Installation
 By itself
 ```bash
 pip install katalytic-data
 ```
 
@@ -20,18 +19,14 @@
 ```
 
 ## Usage
 TODO: Use examples liberally, and show the expected output if you can. It's helpful to have inline the smallest example of usage that you can demonstrate, while providing links to more sophisticated examples if they are too long to reasonably include in the README.
 
 ## Roadmap
 - converting data between formats
-- dict sorting by key/value
-- mapping dict keys/values
-- recursive map
-- recursive sort
 
 ## Contributing
 Contributions can be made in a number of ways:
 - Propose architectural or API improvements
 - Propose new features
 - Propose packaging, building, or deployment improvements
 - Report and fix bugs
```

### Comparing `katalytic-data-0.7.1/pyproject.toml` & `katalytic-data-0.8.0/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["flit_core >=3.2,<4"]
 build-backend = "flit_core.buildapi"
 
 [project]
 name = "katalytic-data"
-version = "0.7.1"
+version = "0.8.0"
 description = "This plugin adds utilities for working with data to the katalytic namespace"
 license = {file = "LICENSE.txt"}
 readme = "README.md"
 
 classifiers = [
     "Development Status :: 3 - Alpha",
     "Intended Audience :: Developers",
@@ -24,22 +24,22 @@
 	"high-level",
 	"data conversion",
 ]
 authors = [{name="Valentin Neagu", email="vali19th@protonmail.com"}]
 
 requires-python = ">=3.6"
 dependencies = [
-    "katalytic-checks>=0.0.1",
     "katalytic-pkg>=0.2.0",
 ]
 
 [project.optional-dependencies]
 dev = [
     "pytest",
     "pytest-cov",
+    "pytest-clarity",
     "pytest-randomly",
 ]
 
 [project.urls]
 homepage = "https://gitlab.com/katalytic/katalytic-data.git"
 repository = "https://gitlab.com/katalytic/katalytic-data.git"
```

### Comparing `katalytic-data-0.7.1/src/katalytic/data.py` & `katalytic-data-0.8.0/src/katalytic/data/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,41 +1,37 @@
+import copy
 from decimal import Decimal
 from fractions import Fraction
 from pathlib import Path
 
-from katalytic.checks import (
+from katalytic.data.checks import (
     is_any_of, is_generator, is_iterable, is_iterator, is_none_of, is_primitive, is_dict_of_sequences_uniform, is_sequence_of_sequences_uniform,
     is_sequence_of_dicts_uniform
 )
 
 from katalytic.pkg import get_version
 
 __version__, __version_info__ = get_version(__name__)
+_UNDEFINED = object()
+
+
+def _generator(): yield 1
+def _function(): pass
 
 
 class _C:
     def __call__(self, *args, **kwargs):
         pass
 
 
 _C_obj = _C()
 _obj = object()
-
-
-def _generator():
-    yield 1
-
-
-def _function():
-    pass
-
-
 _lambda = lambda x: x
 _generator_expr = (x for x in [])
-_sequences = [[], (), range(1)]
+_sequences = [[], (), range(0)]
 _dict_views = [{}.keys(), {}.values(), {}.items()]
 _iterators = [_generator, _generator_expr, iter([]), map(int, ''), enumerate([]), zip([], [])]
 _iterables = [*_dict_views, *_iterators, *_sequences, set(), {}]
 _collections = [(), set(), frozenset([]), {}, []]
 _singletons = [None, True, False]
 _primitives = [*_singletons, 0, 0.0, '', b'', bytearray(b'')]
 _callables = [_generator, _function, _lambda, _C_obj, _C]
@@ -46,27 +42,27 @@
 _strings = ['', b'', bytearray(b'')]
 
 _types = {
     'bool': False,
     'bytearray': bytearray(b''),
     'bytes': b'',
     'callables': _callables,
-    'callable object': _C_obj,
+    'callable_obj': _C_obj,
     'class': _C,
     'collections': _collections,
     'complex': 0 + 0j,
     'decimal': Decimal('0'),
     'dict': {},
     'dict_views': _dict_views,
     'float': 0.0,
     'fraction': Fraction(0, 1),
     'frozenset': frozenset([]),
     'functions': _functions,
-    'generator_expr': _generator_expr,
-    'generator_func': _generator,
+    'generator_expression': _generator_expr,
+    'generator_function': _generator,
     'generators': _generators,
     'int': 0,
     'iterables': _iterables,
     'iterators': _iterators,
     'list': [],
     'map': map(int, []),
     'none': None,
@@ -81,15 +77,15 @@
     'strings': _strings,
     'tuple': (),
 }
 
 
 def all_types(whitelist=None):
     if whitelist is None:
-        return flatten(_types.values())
+        return _flatten(_types.values())
     elif isinstance(whitelist, str):
         whitelist = [whitelist]
     elif not is_iterable(whitelist):
         raise TypeError(f'<whitelist> must be iterable. Got {type(whitelist).__name__}')
 
     unexpected = set(whitelist) - set(_types.keys())
     if unexpected:
```

### Comparing `katalytic-data-0.7.1/tests/test_data.py` & `katalytic-data-0.8.0/tests/test_data.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 from _decimal import Decimal
 from fractions import Fraction
 from pathlib import Path, PosixPath
 
 import pytest
 
-from katalytic.checks import is_iterator, dicts_share_key_order, dicts_share_value_order, is_equal
+from katalytic.data.checks import is_iterator, dicts_share_key_order, dicts_share_value_order, is_equal
 from katalytic.data import (
-    _C, _C_obj, _callables, _collections, _dict_views, _function, _functions, _generators, _iterables, _iterators, _lambda, _numbers, _obj, _objects, _primitives, _sequences, _singletons, _strings, _types, all_types, all_types_besides, as_list_of_dicts, as_list_of_lists, first, first_with_idx, flatten, flatten_recursive, last, last_with_idx, map_dict_keys, map_dict_values,
+    _C, _C_obj, _callables, _collections, _dict_views, _flatten, _function, _functions, _generators, _iterables, _iterators, _lambda, _numbers, _obj, _objects, _primitives, _sequences, _singletons, _strings, _types, all_types, all_types_besides, as_list_of_dicts, as_list_of_lists, first, first_with_idx, flatten, flatten_recursive, last, last_with_idx, map_dict_keys, map_dict_values,
     map_recursive, one, pick_all, pick_all_besides, pick_any, sort_dict_by_keys, sort_dict_by_keys_recursive, sort_dict_by_values, sort_dict_by_values_recursive,
     as_dict_of_lists, sort_recursive, xor, xor_with_idx, detect_fronts, detect_fronts_positive, detect_fronts_negative
 )
 
 
 def _is_list(x):
     return isinstance(x, list)
@@ -54,15 +54,15 @@
         ('iterators', _iterators),
         ('numbers', _numbers),
         ('objects', _objects),
         ('primitives', _primitives),
         ('sequences', _sequences),
         ('singletons', _singletons),
         ('strings', _strings),
-        (None, flatten(_types.values())),
+        (None, _flatten(_types.values())),
         (['iterables', 'objects', 'path'], [*_iterables, *_objects, Path('')]),
         (['iterables'], _iterables),
     ])
     def test_all_types(self, whitelist, expected):
         assert all_types(whitelist) == expected
```

### Comparing `katalytic-data-0.7.1/PKG-INFO` & `katalytic-data-0.8.0/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,42 +1,41 @@
 Metadata-Version: 2.1
 Name: katalytic-data
-Version: 0.7.1
+Version: 0.8.0
 Summary: This plugin adds utilities for working with data to the katalytic namespace
 Keywords: high-level,data conversion
 Author-email: Valentin Neagu <vali19th@protonmail.com>
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: System Administrators
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Utilities
-Requires-Dist: katalytic-checks>=0.0.1
 Requires-Dist: katalytic-pkg>=0.2.0
 Requires-Dist: pytest ; extra == "dev"
 Requires-Dist: pytest-cov ; extra == "dev"
+Requires-Dist: pytest-clarity ; extra == "dev"
 Requires-Dist: pytest-randomly ; extra == "dev"
 Project-URL: homepage, https://gitlab.com/katalytic/katalytic-data.git
 Project-URL: repository, https://gitlab.com/katalytic/katalytic-data.git
 Provides-Extra: dev
 
 ## Description
 TODO: Let people know what your project can do specifically. Provide context and add a link to any reference visitors might be unfamiliar with. A list of Features or a Background subsection can also be added here. If there are alternatives to your project, this is a good place to list differentiating factors.
 
 [![version](https://img.shields.io/pypi/v/katalytic-data)](https://pypi.org/project/katalytic-data/)
-[![Build Status](https://app.travis-ci.com/katalytic/katalytic-data.svg?branch=main)](https://app.travis-ci.com/gitlab/katalytic/katalytic-data)
-[![Test Results](https://img.shields.io/travis/com/katalytic/katalytic-data?label=tests)](https://app.travis-ci.com/gitlab/katalytic/katalytic-data)
-[![Coverage Status](https://coveralls.io/repos/gitlab/katalytic/katalytic-data/badge.svg?branch=main)](https://coveralls.io/gitlab/katalytic/katalytic-data?branch=main)
-[![Docs Coverage](https://img.shields.io/readthedocs/katalytic-data.svg)](https://katalytic-data.readthedocs.io/en/latest/)
-[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
+[![tests](https://gitlab.com/katalytic/katalytic-data/badges/main/pipeline.svg?key_text=tests&key_width=38)](https://gitlab.com/katalytic/katalytic-data/-/commits/main)
+[![coverage](https://gitlab.com/katalytic/katalytic-data/badges/main/coverage.svg)](https://gitlab.com/katalytic/katalytic-data/-/commits/main)
+[![docs](https://img.shields.io/readthedocs/katalytic-data.svg)](https://katalytic-data.readthedocs.io/en/latest/)
+[![license: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](https://opensource.org/licenses/MIT)
 
 ## Installation
 By itself
 ```bash
 pip install katalytic-data
 ```
 
@@ -46,18 +45,14 @@
 ```
 
 ## Usage
 TODO: Use examples liberally, and show the expected output if you can. It's helpful to have inline the smallest example of usage that you can demonstrate, while providing links to more sophisticated examples if they are too long to reasonably include in the README.
 
 ## Roadmap
 - converting data between formats
-- dict sorting by key/value
-- mapping dict keys/values
-- recursive map
-- recursive sort
 
 ## Contributing
 Contributions can be made in a number of ways:
 - Propose architectural or API improvements
 - Propose new features
 - Propose packaging, building, or deployment improvements
 - Report and fix bugs
```

