# Comparing `tmp/canals-0.0.3.tar.gz` & `tmp/canals-0.1.0.tar.gz`

## Comparing `canals-0.0.3.tar` & `canals-0.1.0.tar`

### file list

```diff
@@ -1,49 +1,61 @@
--rw-r--r--   0        0        0     1113 2020-02-02 00:00:00.000000 canals-0.0.3/.pre-commit-config.yaml
--rw-r--r--   0        0        0     1072 2020-02-02 00:00:00.000000 canals-0.0.3/mkdocs.yml
--rw-r--r--   0        0        0      485 2020-02-02 00:00:00.000000 canals-0.0.3/.github/workflows/api-docs.yml
--rw-r--r--   0        0        0      467 2020-02-02 00:00:00.000000 canals-0.0.3/.github/workflows/release.yml
--rw-r--r--   0        0        0     2812 2020-02-02 00:00:00.000000 canals-0.0.3/.github/workflows/tests.yml
--rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 canals-0.0.3/canals/__about__.py
--rw-r--r--   0        0        0      445 2020-02-02 00:00:00.000000 canals-0.0.3/canals/__init__.py
--rw-r--r--   0        0        0     8720 2020-02-02 00:00:00.000000 canals-0.0.3/canals/component.py
--rw-r--r--   0        0        0      288 2020-02-02 00:00:00.000000 canals-0.0.3/canals/pipeline/__init__.py
--rw-r--r--   0        0        0    30093 2020-02-02 00:00:00.000000 canals-0.0.3/canals/pipeline/pipeline.py
--rw-r--r--   0        0        0     8753 2020-02-02 00:00:00.000000 canals-0.0.3/canals/pipeline/save_load.py
--rw-r--r--   0        0        0     1203 2020-02-02 00:00:00.000000 canals-0.0.3/docs/index.md
--rw-r--r--   0        0        0       34 2020-02-02 00:00:00.000000 canals-0.0.3/docs/api-docs/component.md
--rw-r--r--   0        0        0      106 2020-02-02 00:00:00.000000 canals-0.0.3/docs/api-docs/pipeline.md
--rw-r--r--   0        0        0     5175 2020-02-02 00:00:00.000000 canals-0.0.3/docs/concepts/components.md
--rw-r--r--   0        0        0     4740 2020-02-02 00:00:00.000000 canals-0.0.3/docs/concepts/concepts.md
--rw-r--r--   0        0        0     1946 2020-02-02 00:00:00.000000 canals-0.0.3/docs/concepts/parameters.md
--rw-r--r--   0        0        0     3212 2020-02-02 00:00:00.000000 canals-0.0.3/docs/concepts/pipelines.md
--rw-r--r--   0        0        0     4225 2020-02-02 00:00:00.000000 canals-0.0.3/docs/concepts/save-load.md
--rw-r--r--   0        0        0    26250 2020-02-02 00:00:00.000000 canals-0.0.3/images/canals-logo-dark.png
--rw-r--r--   0        0        0    25601 2020-02-02 00:00:00.000000 canals-0.0.3/images/canals-logo-light.png
--rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 canals-0.0.3/test/__init__.py
--rw-r--r--   0        0        0     7316 2020-02-02 00:00:00.000000 canals-0.0.3/test/test_save_load.py
--rw-r--r--   0        0        0      528 2020-02-02 00:00:00.000000 canals-0.0.3/test/components/__init__.py
--rw-r--r--   0        0        0     3908 2020-02-02 00:00:00.000000 canals-0.0.3/test/components/test_accumulate.py
--rw-r--r--   0        0        0     1761 2020-02-02 00:00:00.000000 canals-0.0.3/test/components/test_add_value.py
--rw-r--r--   0        0        0     3026 2020-02-02 00:00:00.000000 canals-0.0.3/test/components/test_below.py
--rw-r--r--   0        0        0     1188 2020-02-02 00:00:00.000000 canals-0.0.3/test/components/test_double.py
--rw-r--r--   0        0        0     2090 2020-02-02 00:00:00.000000 canals-0.0.3/test/components/test_greet.py
--rw-r--r--   0        0        0     1362 2020-02-02 00:00:00.000000 canals-0.0.3/test/components/test_merge.py
--rw-r--r--   0        0        0     2826 2020-02-02 00:00:00.000000 canals-0.0.3/test/components/test_remainder.py
--rw-r--r--   0        0        0      978 2020-02-02 00:00:00.000000 canals-0.0.3/test/components/test_rename.py
--rw-r--r--   0        0        0     1251 2020-02-02 00:00:00.000000 canals-0.0.3/test/components/test_repeat.py
--rw-r--r--   0        0        0     1493 2020-02-02 00:00:00.000000 canals-0.0.3/test/components/test_subtract.py
--rw-r--r--   0        0        0     1412 2020-02-02 00:00:00.000000 canals-0.0.3/test/components/test_sum.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 canals-0.0.3/test/pipelines/__init__.py
--rw-r--r--   0        0        0     1360 2020-02-02 00:00:00.000000 canals-0.0.3/test/pipelines/_test_looping_and_merge_pipeline.py
--rw-r--r--   0        0        0     3598 2020-02-02 00:00:00.000000 canals-0.0.3/test/pipelines/test_complex_pipeline.py
--rw-r--r--   0        0        0     1484 2020-02-02 00:00:00.000000 canals-0.0.3/test/pipelines/test_decision_and_merge_pipeline.py
--rw-r--r--   0        0        0     1252 2020-02-02 00:00:00.000000 canals-0.0.3/test/pipelines/test_decision_pipeline.py
--rw-r--r--   0        0        0      869 2020-02-02 00:00:00.000000 canals-0.0.3/test/pipelines/test_linear_pipeline.py
--rw-r--r--   0        0        0     1374 2020-02-02 00:00:00.000000 canals-0.0.3/test/pipelines/test_looping_pipeline.py
--rw-r--r--   0        0        0     1146 2020-02-02 00:00:00.000000 canals-0.0.3/test/pipelines/test_merging_pipeline.py
--rw-r--r--   0        0        0     1392 2020-02-02 00:00:00.000000 canals-0.0.3/test/pipelines/test_parallel_branches_pipeline.py
--rw-r--r--   0        0        0     1810 2020-02-02 00:00:00.000000 canals-0.0.3/.gitignore
--rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 canals-0.0.3/LICENSE
--rw-r--r--   0        0        0     1356 2020-02-02 00:00:00.000000 canals-0.0.3/README.md
--rw-r--r--   0        0        0     2285 2020-02-02 00:00:00.000000 canals-0.0.3/pyproject.toml
--rw-r--r--   0        0        0     3008 2020-02-02 00:00:00.000000 canals-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0     1198 2020-02-02 00:00:00.000000 canals-0.1.0/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      971 2020-02-02 00:00:00.000000 canals-0.1.0/mkdocs.yml
+-rw-r--r--   0        0        0      485 2020-02-02 00:00:00.000000 canals-0.1.0/.github/workflows/api-docs.yml
+-rw-r--r--   0        0        0      467 2020-02-02 00:00:00.000000 canals-0.1.0/.github/workflows/release.yml
+-rw-r--r--   0        0        0     2844 2020-02-02 00:00:00.000000 canals-0.1.0/.github/workflows/tests.yml
+-rw-r--r--   0        0        0      122 2020-02-02 00:00:00.000000 canals-0.1.0/canals/__about__.py
+-rw-r--r--   0        0        0      427 2020-02-02 00:00:00.000000 canals-0.1.0/canals/__init__.py
+-rw-r--r--   0        0        0      296 2020-02-02 00:00:00.000000 canals-0.1.0/canals/errors.py
+-rw-r--r--   0        0        0      128 2020-02-02 00:00:00.000000 canals-0.1.0/canals/component/__init__.py
+-rw-r--r--   0        0        0     8469 2020-02-02 00:00:00.000000 canals-0.1.0/canals/component/component.py
+-rw-r--r--   0        0        0     2262 2020-02-02 00:00:00.000000 canals-0.1.0/canals/component/save_init_params.py
+-rw-r--r--   0        0        0       61 2020-02-02 00:00:00.000000 canals-0.1.0/canals/draw/__init__.py
+-rw-r--r--   0        0        0     3118 2020-02-02 00:00:00.000000 canals-0.1.0/canals/draw/draw.py
+-rw-r--r--   0        0        0     1687 2020-02-02 00:00:00.000000 canals-0.1.0/canals/draw/graphviz.py
+-rw-r--r--   0        0        0     3168 2020-02-02 00:00:00.000000 canals-0.1.0/canals/draw/mermaid.py
+-rw-r--r--   0        0        0      309 2020-02-02 00:00:00.000000 canals-0.1.0/canals/pipeline/__init__.py
+-rw-r--r--   0        0        0     7474 2020-02-02 00:00:00.000000 canals-0.1.0/canals/pipeline/_utils.py
+-rw-r--r--   0        0        0    26696 2020-02-02 00:00:00.000000 canals-0.1.0/canals/pipeline/pipeline.py
+-rw-r--r--   0        0        0     8637 2020-02-02 00:00:00.000000 canals-0.1.0/canals/pipeline/save_load.py
+-rw-r--r--   0        0        0     1368 2020-02-02 00:00:00.000000 canals-0.1.0/docs/index.md
+-rw-r--r--   0        0        0       83 2020-02-02 00:00:00.000000 canals-0.1.0/docs/api-docs/component.md
+-rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 canals-0.1.0/docs/api-docs/draw.md
+-rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 canals-0.1.0/docs/api-docs/pipeline.md
+-rw-r--r--   0        0        0     7458 2020-02-02 00:00:00.000000 canals-0.1.0/docs/concepts/components.md
+-rw-r--r--   0        0        0     3838 2020-02-02 00:00:00.000000 canals-0.1.0/docs/concepts/concepts.md
+-rw-r--r--   0        0        0     7097 2020-02-02 00:00:00.000000 canals-0.1.0/docs/concepts/pipelines.md
+-rw-r--r--   0        0        0    26250 2020-02-02 00:00:00.000000 canals-0.1.0/images/canals-logo-dark.png
+-rw-r--r--   0        0        0    25601 2020-02-02 00:00:00.000000 canals-0.1.0/images/canals-logo-light.png
+-rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 canals-0.1.0/test/__init__.py
+-rw-r--r--   0        0        0     6547 2020-02-02 00:00:00.000000 canals-0.1.0/test/test_save_load.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 canals-0.1.0/test/pipelines/integration/__init__.py
+-rw-r--r--   0        0        0     3316 2020-02-02 00:00:00.000000 canals-0.1.0/test/pipelines/integration/test_complex_pipeline.py
+-rw-r--r--   0        0        0     1441 2020-02-02 00:00:00.000000 canals-0.1.0/test/pipelines/integration/test_fixed_decision_and_merge_pipeline.py
+-rw-r--r--   0        0        0     1138 2020-02-02 00:00:00.000000 canals-0.1.0/test/pipelines/integration/test_fixed_decision_pipeline.py
+-rw-r--r--   0        0        0     1175 2020-02-02 00:00:00.000000 canals-0.1.0/test/pipelines/integration/test_fixed_merging_pipeline.py
+-rw-r--r--   0        0        0      797 2020-02-02 00:00:00.000000 canals-0.1.0/test/pipelines/integration/test_linear_pipeline.py
+-rw-r--r--   0        0        0     1352 2020-02-02 00:00:00.000000 canals-0.1.0/test/pipelines/integration/test_looping_and_merge_pipeline.py
+-rw-r--r--   0        0        0     1129 2020-02-02 00:00:00.000000 canals-0.1.0/test/pipelines/integration/test_looping_pipeline.py
+-rw-r--r--   0        0        0     1257 2020-02-02 00:00:00.000000 canals-0.1.0/test/pipelines/integration/test_parallel_branches_pipeline.py
+-rw-r--r--   0        0        0     1486 2020-02-02 00:00:00.000000 canals-0.1.0/test/pipelines/integration/test_variable_decision_and_merge_pipeline.py
+-rw-r--r--   0        0        0     1192 2020-02-02 00:00:00.000000 canals-0.1.0/test/pipelines/integration/test_variable_decision_pipeline.py
+-rw-r--r--   0        0        0     1202 2020-02-02 00:00:00.000000 canals-0.1.0/test/pipelines/integration/test_variable_merging_pipeline.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 canals-0.1.0/test/pipelines/unit/__init__.py
+-rw-r--r--   0        0        0     1172 2020-02-02 00:00:00.000000 canals-0.1.0/test/pipelines/unit/test_component.py
+-rw-r--r--   0        0        0      605 2020-02-02 00:00:00.000000 canals-0.1.0/test/test_components/__init__.py
+-rw-r--r--   0        0        0     3782 2020-02-02 00:00:00.000000 canals-0.1.0/test/test_components/test_accumulate.py
+-rw-r--r--   0        0        0      834 2020-02-02 00:00:00.000000 canals-0.1.0/test/test_components/test_add_value.py
+-rw-r--r--   0        0        0      585 2020-02-02 00:00:00.000000 canals-0.1.0/test/test_components/test_double.py
+-rw-r--r--   0        0        0     1515 2020-02-02 00:00:00.000000 canals-0.1.0/test/test_components/test_greet.py
+-rw-r--r--   0        0        0     3134 2020-02-02 00:00:00.000000 canals-0.1.0/test/test_components/test_merge_loop.py
+-rw-r--r--   0        0        0     1163 2020-02-02 00:00:00.000000 canals-0.1.0/test/test_components/test_parity.py
+-rw-r--r--   0        0        0     1147 2020-02-02 00:00:00.000000 canals-0.1.0/test/test_components/test_remainder.py
+-rw-r--r--   0        0        0     1134 2020-02-02 00:00:00.000000 canals-0.1.0/test/test_components/test_repeat.py
+-rw-r--r--   0        0        0      752 2020-02-02 00:00:00.000000 canals-0.1.0/test/test_components/test_subtract.py
+-rw-r--r--   0        0        0      922 2020-02-02 00:00:00.000000 canals-0.1.0/test/test_components/test_sum.py
+-rw-r--r--   0        0        0     1165 2020-02-02 00:00:00.000000 canals-0.1.0/test/test_components/test_threshold.py
+-rw-r--r--   0        0        0     1810 2020-02-02 00:00:00.000000 canals-0.1.0/.gitignore
+-rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 canals-0.1.0/LICENSE
+-rw-r--r--   0        0        0     1521 2020-02-02 00:00:00.000000 canals-0.1.0/README.md
+-rw-r--r--   0        0        0     2320 2020-02-02 00:00:00.000000 canals-0.1.0/pyproject.toml
+-rw-r--r--   0        0        0     3181 2020-02-02 00:00:00.000000 canals-0.1.0/PKG-INFO
```

### Comparing `canals-0.0.3/.pre-commit-config.yaml` & `canals-0.1.0/.pre-commit-config.yaml`

 * *Files 8% similar despite different names*

```diff
@@ -20,14 +20,16 @@
   hooks:
   - id: black-jupyter
 
 - repo: https://github.com/pre-commit/mirrors-mypy
   rev: 'v1.1.1'
   hooks:
   - id: mypy
+    args: [--ignore-missing-imports]
+    additional_dependencies: ['types-requests']
 
 - repo: https://github.com/pycqa/pylint
   rev: 'v2.17.0'
   hooks:
   - id: pylint
     exclude: ^test/
     args: [
```

### Comparing `canals-0.0.3/mkdocs.yml` & `canals-0.1.0/mkdocs.yml`

 * *Files 24% similar despite different names*

```diff
@@ -29,15 +29,14 @@
   - optionalConfig.js
   - https://unpkg.com/mermaid@9.4.0/dist/mermaid.min.js
   - extra-loader.js
 
 nav:
     - Get Started: index.md
     - Concepts:
-      - Components and Pipelines: concepts/concepts.md
-      - Creating Components: concepts/components.md
-      - Advanced Pipelines: concepts/pipelines.md
-      - Parameters: concepts/parameters.md
-      - Save and Load Your Pipelines: concepts/save-load.md
+      - Core Concepts: concepts/concepts.md
+      - Components: concepts/components.md
+      - Pipelines: concepts/pipelines.md
     - API Docs:
-      - Component: api-docs/component.md
       - Pipeline: api-docs/pipeline.md
+      - Component: api-docs/component.md
+      - Draw: api-docs/draw.md
```

### Comparing `canals-0.0.3/.github/workflows/tests.yml` & `canals-0.1.0/.github/workflows/tests.yml`

 * *Files 7% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 
       - name: Setup Python
         uses: actions/setup-python@v4
         with:
           python-version: '3.8'
 
       - name: Install Canals
-        run: pip install .[dev]
+        run: pip install .[mermaid,dev]
 
       - name: Mypy
         run: |
           mkdir .mypy_cache/
           mypy --install-types --non-interactive --ignore-missing-imports canals/
 
   pylint:
@@ -37,15 +37,15 @@
 
       - name: Setup Python
         uses: actions/setup-python@v4
         with:
           python-version: '3.8'
 
       - name: Install Canals
-        run: pip install .[dev]
+        run: pip install .[mermaid,dev]
 
       - name: Pylint
         run: pylint -ry -j 0 canals/
 
   black:
     runs-on: ubuntu-latest
     steps:
@@ -54,15 +54,15 @@
 
       - name: Setup Python
         uses: actions/setup-python@v4
         with:
           python-version: '3.8'
 
       - name: Install Canals
-        run: pip install .[dev]
+        run: pip install .[mermaid,dev]
 
       - name: Check status
         run: |
           if ! black canals/ --check; then
             git status
             echo "###################################################################################################"
             echo "# "
@@ -102,11 +102,11 @@
 
       - name: Setup Python
         uses: actions/setup-python@v4
         with:
           python-version: '3.8'
 
       - name: Install Canals
-        run: pip install .[dev]
+        run: pip install .[mermaid,dev]
 
       - name: Run
         run: hatch run cov
```

### Comparing `canals-0.0.3/canals/component.py` & `canals-0.1.0/canals/component/component.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,228 +1,175 @@
-from typing import Iterable
-
 import logging
 import inspect
-from functools import partial, wraps
-
-
-logger = logging.getLogger(__name__)
-
-
-class ComponentError(Exception):
-    pass
-
-
-def save_init_parameters(init_func, serializable=True):
-    """
-    Decorator that saves the init parameters of a component in a dictionary.
-    """
-
-    @wraps(init_func)
-    def wrapper_save_init_parameters(self, *args, **kwargs):
-
-        # Convert all args into kwargs
-        sig = inspect.signature(init_func)
-        arg_names = list(sig.parameters.keys())
-        if any(arg_names) and arg_names[0] in ["self", "cls"]:
-            arg_names.pop(0)
-        args_as_kwargs = {arg_name: arg for arg, arg_name in zip(args, arg_names)}
 
-        # Collect and store all the init parameters
-        self.init_parameters = {**args_as_kwargs, **kwargs}
+from canals.errors import ComponentError
+from canals.component.save_init_params import set_default_component_attributes
 
-        # Call the actuall __init__ function with the arguments
-        init_func(self, **self.init_parameters)
 
-        # Check if the component can be saved with `save_pipelines()`
-        if serializable:
-            is_serializable(self.init_parameters)
-
-    return wrapper_save_init_parameters
-
-
-def is_serializable(value):
-    """
-    Checks that the value given can be saved to disk with a writer like `json.dump`.
-    Very conservative check.
-    """
-    if isinstance(value, (bool, int, float, str)):
-        return
-    if isinstance(value, dict):
-        for val in value.values():
-            is_serializable(val)
-    elif isinstance(value, Iterable):
-        for val in value:
-            is_serializable(val)
-    else:
-        raise ComponentError(
-            f"'{value}' is not a bool, int, float, str, None, dict or iterable. "
-            "It can't be passed to the `__init__()` method of a component."
-        )
+logger = logging.getLogger(__name__)
 
 
-def component(class_, serializable=True):
+def component(class_):
     """
-    Marks a class as a component.
-    Any class decorated with `@component` can be used by a Pipeline.
+    Marks a class as a component. Any class decorated with `@component` can be used by a Pipeline.
 
-    All components MUST follow the contract below.
-    This docstring is the source of truth for components contract.
+    All components must follow the contract below. This docstring is the source of truth for components contract.
 
     ```python
     def __init__(self, [... components init parameters ...]):
     ```
-    Mandatory method.
-
-    Components should have an `__init__` method where they define:
-
-    - `self.inputs = [<expected_input_connection_name(s)>]`:
-        A list with all the connections they can possibly receive input from
+    Optional method.
 
-    - `self.outputs = [<expected_output_connection_name(s)>]`:
-        A list with the connections they might possibly produce as output
+    Components may have an `__init__` method where they define:
 
-    - `self.init_parameters = {<init parameters>}`:
-        Any state they wish to be persisted when they are saved.
-        These values will be given to the `__init__` method of a new instance
-        when the pipeline is loaded.
-        Note that by default the `@component` decorator saves the arguments
-        automatically. Components can assume that the dictionary exists and
-        can alter its content in the `__init__` method if needed.
-
-    Components should take only "basic" Python types as parameters of their
-    `__init__` function, or iterables and dictionaries containing only such values.
-    Anything else (objects, functions, etc) will raise an exception at init time.
-
-    _(TODO explain how to use classes and functions in init. In the meantime see
-    `test/components/test_accumulate.py`)_
-
-    If components want to let users customize their input and output connections (be it
-    the connection name, the connection count, etc...) they should provide properly
-    named init parameters:
-
-    - `input: str` or `inputs: List[str]` (always with proper defaults)
-    - `output: str` or `outputs: List[str]` (always with proper defaults)
-
-    All the rest is going to be interpreted as a regular init parameter that
-    has nothing to do with the component connections.
-
-    The `__init__` must be extrememly lightweight, because it's a frequent
-    operation during the construction and validation of the pipeline. If a component
-    has some heavy state to initialize (models, backends, etc...) refer to the
-    `warm_up()` method.
+    - `self.defaults = {parameter_name: parameter_default_value, ...}`:
+        All values defined here will be sent to the `run()` method when the Pipeline calls it.
+        If any of these parameters is also receiving input from other components, those have precedence.
+        This collection of values is supposed to replace the need for default values in `run()` and make them
+        dynamically configurable.
+
+    - `self.init_parameters = {same parameters that the __init__ method received}`:
+        In this dictionary you can store any state the components wish to be persisted when they are saved.
+        These values will be given to the `__init__` method of a new instance when the pipeline is loaded.
+        Note that by default the `@component` decorator saves the arguments automatically.
+        However, if a component sets their own `init_parameters` manually in `__init__()`, that will be used instead.
+        Note: all of the values contained here **must be JSON serializable**. Serialize them manually if needed.
+
+    Components should take only "basic" Python types as parameters of their `__init__` function, or iterables and
+    dictionaries containing only such values. Anything else (objects, functions, etc) will raise an exception at init
+    time. If there's the need for such values, consider serializing them to a string.
+
+    _(TODO explain how to use classes and functions in init. In the meantime see `test/components/test_accumulate.py`)_
+
+    The `__init__` must be extrememly lightweight, because it's a frequent operation during the construction and
+    validation of the pipeline. If a component has some heavy state to initialize (models, backends, etc...) refer to
+    the `warm_up()` method.
 
     ```
     def warm_up(self):
     ```
     Optional method.
 
-    This method is called by Pipeline before the graph execution.
-    Make sure to avoid double-initializations, because Pipeline will not keep
-    track of which components it called `warm_up()` on.
+    This method is called by Pipeline before the graph execution. Make sure to avoid double-initializations,
+    because Pipeline will not keep track of which components it called `warm_up()` on.
 
     ```
-    def run(
-        self,
-        name: str,
-        data: List[Tuple[str, Any]],
-        parameters: Dict[str, Dict[str, Any]],
-    ):
+    @dataclass
+    class Output:
+        <expected output fields>
     ```
-    Mandatory method.
+    Semi-mandatory method (either this or `self.output_types(self)`).
 
-    This is the method where the main functionality of the component should be carried out.
-    It's called by `Pipeline.run()`, which passes the following parameters to it:
+    This inner class defines how the output of this component looks like. For example, if the node is producing
+    a list of Documents, the fields of the class should be `documents: List[Document]`
 
-    - `name: str`: the name of the component. Allows the component to find its own parameters in
-        the `parameters` dictionary (see below).
+    Defaults are allowed, however `Optional`, `Union` and similar "generic" types are not. This is necessary to allow
+    proper validation of the connections, which rely on the type of these fields.
 
-    - `data: List[Tuple[str, Any]]`: the input data.
-        Pipeline guarantees that the following assert always passes:
+    Some components may need more dynamic output: for example, your component accepts a list of file extensions at
+    init time and wants to have one output field for each of those. For these scenarios, refer to `self.output_type()`.
 
-        `assert self.inputs == [name for name, value in data]`
+    Every component should define **either** `Output` or `self.output_types`.
 
-        which means that:
-        - `data` is of the same length as `self.inputs`.
-        - `data` contains one tuple for each string stored in `self.inputs`.
-        - no guarantee is given on the values of these tuples: notably, if there was a
-            decision component upstream, some values might be `None`.
-
-        For example, if a component declares `self.inputs = ["value", "value"]` (think of a
-        `Sum` component), `data` might look like:
-
-        `[("value", 1), ("value", 10)]`
+    ```
+    def output_types(self) -> dataclass:
+    ```
+    Semi-mandatory method (either this or `class Output`).
 
-        `[("value", None), ("value", 10)]`
+    This method defines how the output of this component looks like. For example, if the node is producing
+    a list of Documents, this method should return a dataclass with such fields, for example:
+    `return make_dataclass("Output", [(f"documents", List[Document], None)])`
 
-        `[("value", None), ("value", None)]`
+    Defaults are allowed, however `Optional`, `Union` and similar "generic" types are not. This is necessary to allow
+    proper validation of the connections, which rely on the type of these fields.
 
-        `[("value", 1), ("value", ["something", "unexpected"])]`
+    If the output is static, normally the `Output` dataclass is preferred, as it provides autocompletion for the users.
 
-        but it will never look like:
+    Every component should define **either** `Output` or `self.output_types`.
 
-        `[("value", 1), ("value", 10), ("value", 100)]`
+    ```
+    def run(self, <parameters, typed>) -> Output:
+    ```
+    Mandatory method.
 
-        `[("value": 15)]`
+    This is the method where the main functionality of the component should be carried out. It's called by
+    `Pipeline.run()`.
 
-        `[("value": 15), ("unexpected", 10)]`
+    When the component should run, Pipeline will call this method with:
 
-    - `parameters: Dict[str, Dict[str, Any]]`: a dictionary of dictionaries with all
-        the parameters for all components.
-        Note that all components have access to all parameters for all other components: this
-        might come handy to components like `Agent`s, that want to influence the behavior
-        of components downstream.
-        Components can access their own parameters using `name`, but they must **not** assume
-        their name is present in the dictionary.
-        Therefore, the best way to get the parameters is with
-        `my_parameters = parameters.get(name, {})`
+    - all the input values coming from "upstream" components connected to it,
+    - if any is missing, the corresponding value defined in `self.defaults`, if it exists.
 
-    Pipeline expect the output of this function to be a tuple of two dictionaries.
-    The first item is a dictionary that represents the output and it should always
-    abide to the following format:
+    All parameters of `run()` **must be typed**. The types are used by `Pipeline.connect()` to make sure the two
+    components agree on the type being passed, to try ensure the connection will be successful.
+    Defaults are allowed, however `Optional`, `Union` and similar "generic" types are not, just as for the outputs.
 
-    `{output_name: output_value for output_name in <subset of self.expected_output>}`
+    `run()` must return a single instance of the dataclass declared through either `Output` or `self.output_types()`.
 
-    Which means that:
-    - Components are not forced to produce output on all the expected outputs: for example,
-        components taking a decision, like classifiers, can produce output on a subset of
-        the expected output connections and Pipeline will figure out the rest.
-    - Components must not add any key in the data dictionary that is not present in `self.outputs`.
+    A variadic `run()` method is allowed if it respects the following rules:
 
-    The second item of the tuple is the `parameters` dictionary. This allows component to
-    propagate downstream any change they might have done to the `parameters` dictionary.
+    - It can take **either** regular parameters, or a single variadic positional (`*args`), NOT BOTH.
+    - `**kwargs` are not supported
+    - The variadic `*args` must be typed, for example `*args: int` if the component accepts any number of integers.
 
     Args:
         class_: the class that Canals should use as a component.
         serializable: whether to check, at init time, if the component can be saved with
         `save_pipelines()`.
 
     Returns:
-        A class that can be recognized by Canals as a component.
+        A class that can be recognized as a component.
 
     Raises:
-        ComponentError: if the class provided has no `run()` method.
+        ComponentError: if the class provided has no `run()` method or otherwise doesn't respect the component contract.
     """
     logger.debug("Registering %s as a component", class_)
 
     # '__canals_component__' is used to distinguish components from regular classes.
     # Its value is set to the desired component name: normally it is the class name, but it can technically be customized.
     class_.__canals_component__ = class_.__name__
 
     # Check for run()
     if not hasattr(class_, "run"):
-        # TODO check the component signature too
-        raise ComponentError("Components must have a 'run()' method. See the docs for more information.")
+        raise ComponentError(f"{class_.__name__} must have a 'run()' method. See the docs for more information.")
+    run_signature = inspect.signature(class_.run)
+
+    # Check the run() signature for keyword variadic arguments
+    if any(run_signature.parameters[param].kind == inspect.Parameter.VAR_KEYWORD for param in run_signature.parameters):
+        raise ComponentError(
+            f"{class_.__name__} can't have variadic keyword arguments like **kwargs in its 'run()' method."
+        )
 
-    # Check for __init__()
-    if not hasattr(class_, "__init__"):
-        # TODO check the component signature too
-        raise ComponentError("Components must have a '__init__()' method. See the docs for more information.")
+    # Check the run() signature for missing types in positional variadic arguments
+    if any(
+        run_signature.parameters[param].kind == inspect.Parameter.VAR_POSITIONAL
+        and run_signature.parameters[param].annotation == inspect.Parameter.empty
+        for param in run_signature.parameters
+    ):
+        raise ComponentError(
+            f"{class_.__name__} must type also variadic arguments like *args in its 'run()' method.\n"
+            "Hint: variadic arguments are typed in singular form, so if your component takes an arbitrary number of "
+            "strings, the signature of run() should look like 'def run(self, *my_strings: str) -> Output:'."
+        )
 
-    # Automatically registers all the init parameters in an instance attribute called `init_parameters`.
-    # See `save_init_parameters()`.
-    class_.__init__ = save_init_parameters(class_.__init__, serializable=serializable)
+    # Check the run() signature for other missing types
+    missing_types = [
+        parameter
+        for parameter in list(run_signature.parameters)[1:]  # First is 'self' and it doesn't matter.
+        if run_signature.parameters[parameter].annotation == inspect.Parameter.empty
+    ]
+    if missing_types:
+        raise ComponentError(
+            f"{class_.__name__}.run() must declare types for all its parameters, "
+            f"but these parameters are not typed: {', '.join(missing_types)}."
+        )
 
-    return class_
+    # Check for the return types
+    if run_signature.return_annotation == inspect.Parameter.empty:
+        if not hasattr(class_, "output_type"):
+            raise ComponentError(f"{class_.__name__}.run() must declare the type of its return value.")
 
+    # Automatically registers all the init parameters in an instance attribute called `_init_parameters`.
+    # See `save_init_parameters()`.
+    class_.__init__ = set_default_component_attributes(class_.__init__)
 
-non_serializable_component = partial(component, serializable=False)
+    return class_
```

### Comparing `canals-0.0.3/canals/pipeline/pipeline.py` & `canals-0.1.0/canals/pipeline/pipeline.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,78 +1,31 @@
-from typing import Optional, Any, Dict, List, Union, Tuple
+from typing import Optional, Any, Dict, List, Tuple, Literal
 
-from pathlib import Path
+import datetime
 import logging
+from pathlib import Path
 from copy import deepcopy
 from collections import OrderedDict
 
 import networkx as nx
-from networkx.drawing.nx_agraph import to_agraph
-
-
-logger = logging.getLogger(__name__)
-
-
-PYGRAPHVIZ_IMPORTED = False
-try:
-    import pygraphviz  # pylint: disable=unused-import
-
-    PYGRAPHVIZ_IMPORTED = True
-except ImportError:
-    logger.info(
-        "Could not import `pygraphviz`. Please install via: \n"
-        "pip install pygraphviz\n"
-        "(You might need to run this first: apt install libgraphviz-dev graphviz )"
-    )
-
-
-class PipelineError(Exception):
-    pass
-
-
-class PipelineRuntimeError(Exception):
-    pass
-
-
-class PipelineConnectError(PipelineError):
-    pass
-
-
-class PipelineValidationError(PipelineError):
-    pass
-
 
-class PipelineMaxLoops(PipelineError):
-    pass
+from canals.errors import PipelineConnectError, PipelineMaxLoops, PipelineRuntimeError, PipelineValidationError
+from canals.draw import draw, RenderingEngines
+from canals.pipeline._utils import (
+    InputSocket,
+    OutputSocket,
+    find_input_sockets,
+    find_output_sockets,
+    find_unambiguous_connection,
+    parse_connection_name,
+    validate_pipeline_input,
+)
 
 
-def locate_pipeline_input_components(graph) -> List[str]:
-    """
-    Collect the components with no input connections: they receive directly the pipeline inputs.
-
-    Args:
-        graph: the pipeline graph.
-
-    Returns:
-        A list of components that should directly receive the user's inputs.
-    """
-    return [node for node in graph.nodes if not graph.in_edges(node) or graph.nodes[node]["input_component"]]
-
-
-def locate_pipeline_output_components(graph) -> List[str]:
-    """
-    Collect the components with no output connections: these define the output of the pipeline.
-
-    Args:
-        graph: the pipeline graph.
-
-    Returns:
-        A list of components whose output goes back to the user.
-    """
-    return [node for node in graph.nodes if not graph.out_edges(node) or graph.nodes[node]["output_component"]]
+logger = logging.getLogger(__name__)
 
 
 class Pipeline:
     """
     Components orchestration engine.
 
     Builds a graph of components and orchestrates their execution according to the execution graph.
@@ -90,571 +43,530 @@
             metadata: arbitrary dictionary to store metadata about this pipeline. Make sure all the values contained in
                 this dictionary can be serialized and deserialized if you wish to save this pipeline to file with
                 `save_pipelines()/load_pipelines()`.
             max_loops_allowed: how many times the pipeline can run the same node before throwing an exception.
         """
         self.metadata = metadata or {}
         self.max_loops_allowed = max_loops_allowed
-        self.graph = nx.DiGraph()
-
-    def __eq__(self, other) -> bool:
-        # Equal pipelines share all nodes and metadata instances.
-        if not isinstance(other, type(self)):
-            return False
-        return (
-            self.metadata == other.metadata
-            and self.max_loops_allowed == other.max_loops_allowed
-            and self.graph == other.graph
-        )
+        self.graph = nx.MultiDiGraph()
+        self.debug: Dict[int, Dict[str, Any]] = {}
 
-    def add_component(
-        self,
-        name: str,
-        instance: Any,
-        parameters: Optional[Dict[str, Any]] = None,
-        input_component: bool = False,
-        output_output: bool = False,
-    ) -> None:
+    def add_component(self, name: str, instance: Any) -> None:
         """
         Create a component for the given component. Components are not connected to anything by default:
         use `Pipeline.connect()` to connect components together.
 
         Component names must be unique, but component instances can be reused if needed.
 
         Args:
             name: the name of the component.
             instance: the component instance.
-            parameters: default parameters to pass to this component's instance only then this specific component is
-                executed. These parameters are NOT shared across components that use the same instance.
-            input_component: whether this component should receive the input data given to `Pipeline.run()` directly, regardless
-                of its location in the Pipeline.
-            output_component: whether the output of this component should be returned as output, regardless of its
-                location in the Pipeline.
 
         Returns:
             None
 
         Raises:
-            ValueError: if a component with the same name already exists or `parameters` is not a dictionary
+            ValueError: if a component with the same name already exists
             PipelineValidationError: if the given instance is not a Canals component
         """
         # Component names are unique
         if name in self.graph.nodes:
-            raise ValueError(f"Component named '{name}' already exists: choose another name.")
+            raise ValueError(f"A component named '{name}' already exists in this pipeline: choose another name.")
+
+        # Components can't be named `_debug`
+        if name == "_debug":
+            raise ValueError("'_debug' is a reserved name for debug output. Choose another name.")
 
         # Component instances must be components
         if not hasattr(instance, "__canals_component__"):
             raise PipelineValidationError(
                 f"'{type(instance)}' doesn't seem to be a component. Is this class decorated with @component?"
             )
 
-        # Params must be a dict
-        if parameters and not isinstance(parameters, dict):
-            raise ValueError("'parameters' must be a dictionary.")
+        # Find inputs and outputs
+        input_sockets = find_input_sockets(instance)
+        output_sockets = find_output_sockets(instance)
 
         # Add component to the graph, disconnected
         logger.debug("Adding component '%s' (%s)", name, instance)
         self.graph.add_node(
             name,
             instance=instance,
+            input_sockets=input_sockets,
+            variadic_input=any(e.variadic for e in input_sockets.values()),
+            output_sockets=output_sockets,
             visits=0,
-            parameters=parameters,
-            input_component=input_component,
-            output_component=output_output,
         )
 
     def connect(self, connect_from: str, connect_to: str) -> None:
         """
-        Connect components together. All components to connect must exist in the pipeline.
-        If connecting to an component that has several output connections, specify its name with
+        Connects two components together. All components to connect must exist in the pipeline.
+        If connecting to an component that has several output connections, specify the inputs and output names as
         'component_name.connections_name'.
 
         Args:
-            connect_from: the component that deliver the values. This can be either a single component name or can be
+            connect_from: the component that delivers the value. This can be either just a component name or can be
                 in the format `component_name.connection_name` if the component has multiple outputs.
-            connect_to: the component that receives the values. This is always just the component name.
+            connect_to: the component that receives the value. This can be either just a component name or can be
+                in the format `component_name.connection_name` if the component has multiple inputs.
 
         Returns:
             None
 
         Raises:
             PipelineConnectError: if the two components cannot be connected (for example if one of the components is
-                not present in the pipeline, or the connections don't match, and so on).
+                not present in the pipeline, or the connections don't match by type, and so on).
         """
-        upstream_node_name = connect_from
-        downstream_node_name = connect_to
-
-        # Find out the name of the connection
-        edge_name = None
         # Edges may be named explicitly by passing 'node_name.edge_name' to connect().
-        # Specify the edge name for the upstream node only.
-        if "." in upstream_node_name:
-            upstream_node_name, edge_name = upstream_node_name.split(".", maxsplit=1)
-            upstream_node = self.graph.nodes[upstream_node_name]["instance"]
-        else:
-            # If the edge had no explicit name and the upstream node has multiple outputs, raise an exception
-            upstream_node = self.graph.nodes[upstream_node_name]["instance"]
-            if len(upstream_node.outputs) != 1:
+        from_node, from_socket_name = parse_connection_name(connect_from)
+        to_node, to_socket_name = parse_connection_name(connect_to)
+
+        # Get the nodes data.
+        try:
+            from_sockets = self.graph.nodes[from_node]["output_sockets"]
+        except KeyError as exc:
+            raise ValueError(f"Component named {from_node} not found in the pipeline.") from exc
+
+        try:
+            to_sockets = self.graph.nodes[to_node]["input_sockets"]
+        except KeyError as exc:
+            raise ValueError(f"Component named {to_node} not found in the pipeline.") from exc
+
+        # If the name of either socket is given, get the socket
+        if from_socket_name:
+            from_socket = from_sockets.get(from_socket_name, None)
+            if not from_socket:
                 raise PipelineConnectError(
-                    f"Please specify which output of '{upstream_node_name}' "
-                    f"'{downstream_node_name}' should connect to. Component '{upstream_node_name}' has the following "
-                    f"outputs: {upstream_node.outputs}"
+                    f"'{from_node}.{from_socket_name} does not exist. "
+                    f"Output connections of {from_node} are: "
+                    + ", ".join([f"{name} (type {socket.type.__name__})" for name, socket in from_sockets.items()])
+                )
+        if to_socket_name:
+            to_socket = to_sockets.get(to_socket_name, None)
+            if not to_socket:
+                raise PipelineConnectError(
+                    f"'{to_node}.{to_socket_name} does not exist. "
+                    f"Input connections of {to_node} are: "
+                    + ", ".join([f"{name} (type {socket.type.__name__})" for name, socket in to_sockets.items()])
                 )
-            edge_name = upstream_node.outputs[0]
 
-        # Remove edge name from downstream_node name (it's needed only when the node is upstream)
-        downstream_node_name = downstream_node_name.split(".", maxsplit=2)[0]
-        downstream_node = self.graph.nodes[downstream_node_name]["instance"]
-
-        # All nodes names must be in the pipeline already
-        if upstream_node_name not in self.graph.nodes:
-            raise PipelineConnectError(f"'{upstream_node_name}' is not present in the pipeline.")
-        if downstream_node_name not in self.graph.nodes:
-            raise PipelineConnectError(f"'{downstream_node_name}' is not present in the pipeline.")
-
-        # Check if the edge with that name already exists between those two nodes
-        if any(
-            edge[1] == downstream_node_name and edge[2]["label"] == edge_name
-            for edge in self.graph.edges.data(nbunch=upstream_node_name)
-        ):
-            logger.info(
-                "A connection called '%s' between component '%s' and component '%s' already exists: skipping.",
-                edge_name,
-                upstream_node_name,
-                downstream_node_name,
+        # If either one of the two sockets is not specified, look for an unambiguous connection
+        # Note that if there is more than one possible connection but two sockets match by name, they're paired.
+        if not to_socket_name or not from_socket_name:
+            from_sockets = [from_socket] if from_socket_name else from_sockets.values()
+            to_sockets = [to_socket] if to_socket_name else to_sockets.values()
+            from_socket, to_socket = find_unambiguous_connection(
+                from_node=from_node, from_sockets=from_sockets, to_node=to_node, to_sockets=to_sockets
             )
-            return
 
-        # Find all empty slots in the upstream and downstream nodes
-        free_downstream_inputs = deepcopy(downstream_node.inputs)
-        for _, __, data in self.graph.in_edges(downstream_node_name, data=True):
-            position = free_downstream_inputs.index(data["label"])
-            free_downstream_inputs.pop(position)
-
-        free_upstream_outputs = deepcopy(upstream_node.outputs)
-        for _, __, data in self.graph.out_edges(upstream_node_name, data=True):
-            position = free_upstream_outputs.index(data["label"])
-            free_upstream_outputs.pop(position)
-
-        # Make sure the edge is connecting one free input to one free output
-        if edge_name not in free_downstream_inputs or edge_name not in free_upstream_outputs:
-            inputs_string = "\n".join(
-                [
-                    " - " + edge[2]["label"] + f" (taken by {edge[0]})"
-                    for edge in self.graph.in_edges(downstream_node_name, data=True)
-                ]
-                + [f" - {free_in_edge} (free)" for free_in_edge in free_downstream_inputs]
-            )
-            outputs_string = "\n".join(
-                [
-                    " - " + edge[2]["label"] + f" (taken by {edge[1]})"
-                    for edge in self.graph.out_edges(upstream_node_name, data=True)
-                ]
-                + [f" - {free_out_edge} (free)" for free_out_edge in free_upstream_outputs]
+        # Connect the components on these sockets
+        self._direct_connect(from_node=from_node, from_socket=from_socket, to_node=to_node, to_socket=to_socket)
+
+    def _direct_connect(self, from_node: str, from_socket: OutputSocket, to_node: str, to_socket: InputSocket) -> None:
+        """
+        Directly connect socket to socket.
+        """
+        # Check that the types match. We need type equality: subclass relationships are not accepted, just like
+        # Optionals, Unions, and similar "aggregate" types. See https://github.com/python/typing/issues/570
+        if not from_socket.type == to_socket.type:
+            raise PipelineConnectError(
+                f"Cannot connect '{from_node}.{from_socket.name}' with '{to_node}.{to_socket.name}': "
+                f"their declared input and output types do not match.\n"
+                f" - {from_node}.{from_socket.name}: {from_socket.type.__name__}\n"
+                f" - {to_node}.{to_socket.name}: {to_socket.type.__name__}\n"
             )
+
+        # Make sure the receiving socket is not taken - sending sockets can be connected as many times as needed,
+        # so they don't need this check
+        if to_socket.taken_by:
             raise PipelineConnectError(
-                f"Cannot connect '{upstream_node_name}' with '{downstream_node_name}' "
-                f"with an connection named '{edge_name}': "
-                f"their declared inputs and outputs do not match.\n"
-                f"Upstream component '{upstream_node_name}' declared these outputs:\n{outputs_string}\n"
-                f"Downstream component '{downstream_node_name}' declared these inputs:\n{inputs_string}\n"
+                f"Cannot connect '{from_node}.{from_socket.name}' with '{to_node}.{to_socket.name}': "
+                f"{to_node}.{to_socket.name} is already connected to {to_socket.taken_by}.\n"
             )
+
         # Create the connection
-        logger.debug(
-            "Connecting component '%s' to component '%s' with connection name '%s'",
-            upstream_node_name,
-            downstream_node_name,
-            edge_name,
-        )
-        self.graph.add_edge(upstream_node_name, downstream_node_name, label=edge_name)
+        logger.debug("Connecting '%s.%s' to '%s.%s'", from_node, from_socket.name, to_node, to_socket.name)
+        edge_key = f"{from_socket.name}/{to_socket.name}"
+        self.graph.add_edge(from_node, to_node, key=edge_key, from_socket=from_socket, to_socket=to_socket)
 
-    def get_component(self, name: str) -> Dict[str, Any]:
+        # Mark the receiving socket as taken (unless is variadic - variadic sockets are never "taken")
+        if not to_socket.variadic:
+            to_socket.taken_by = from_node
+
+    def get_component(self, name: str) -> object:
         """
-        Returns all the data associated with a component.
+        Returns an instance of a component.
 
         Args:
             name: the name of the component
 
         Returns:
-            A dictionary containing all data that was given to `add_component()` (except for `name`)
+            The instance of that component.
 
         Raises:
-            ValueError: if a nocomponentde with that name is not present in the pipeline.
+            ValueError: if a component with that name is not present in the pipeline.
         """
-        candidates = [node for node in self.graph.nodes if node == name]
-        if not candidates:
-            raise ValueError(f"Component named {name} not found.")
-        return self.graph.nodes[candidates[0]]
+        try:
+            return self.graph.nodes[name]["instance"]
+        except KeyError as exc:
+            raise ValueError(f"Component named {name} not found in the pipeline.") from exc
 
-    def draw(self, path: Path) -> None:
+    def draw(self, path: Path, engine: RenderingEngines = "mermaid-img") -> None:
         """
-        Draws the pipeline. Requires `pygraphviz`.
-        Run `pip install canals[draw]` to install missing dependencies.
+        Draws the pipeline. Requires either `graphviz` as a system dependency, or an internet connection for Mermaid.
+        Run `pip install canals[graphviz]` or `pip install canals[mermaid]` to install missing dependencies.
 
         Args:
-            path: where to save the drawing.
+            path: where to save the diagram.
+            engine: which format to save the graph as. Accepts 'graphviz', 'mermaid-text', 'mermaid-img'.
+                Default is 'mermaid-img'.
 
         Returns:
             None
 
         Raises:
-            ImportError: if pygraphviz is not installed.
+            ImportError: if `engine='graphviz'` and `pygraphviz` is not installed.
+            HTTPConnectionError: (and similar) if the internet connection is down or other connection issues.
         """
-        if not PYGRAPHVIZ_IMPORTED:
-            raise ImportError(
-                "Could not import `pygraphviz`. Please install via: \n"
-                "pip install pygraphviz\n"
-                "(You might need to run this first: apt install libgraphviz-dev graphviz )"
-            )
-        graph = deepcopy(self.graph)
-
-        input_nodes = locate_pipeline_input_components(graph)
-        output_nodes = locate_pipeline_output_components(graph)
-
-        # Draw the input
-        graph.add_node("input", shape="plain")
-        for node in input_nodes:
-            for edge in graph.nodes[node]["instance"].inputs:
-                graph.add_edge("input", node, label=edge)
-
-        # Draw the output
-        graph.add_node("output", shape="plain")
-        for node in output_nodes:
-            for edge in graph.nodes[node]["instance"].outputs:
-                graph.add_edge(node, "output", label=edge)
-
-        graphviz = to_agraph(graph)
-        graphviz.layout("dot")
-        graphviz.draw(path)
-        logger.debug("Pipeline diagram saved at %s", path)
+        draw(graph=deepcopy(self.graph), path=path, engine=engine)
 
     def warm_up(self):
         """
         Make sure all nodes are warm.
 
         It's the node's responsibility to make sure this method can be called at every `Pipeline.run()`
         without re-initializing everything.
         """
         for node in self.graph.nodes:
             if hasattr(self.graph.nodes[node]["instance"], "warm_up"):
+                logger.info("Warming up component %s...", node)
                 self.graph.nodes[node]["instance"].warm_up()
 
-    def run(
-        self,
-        data: Union[Dict[str, Any], List[Tuple[str, Any]]],
-        parameters: Optional[Dict[str, Dict[str, Any]]] = None,
-        debug: bool = False,
-    ) -> Dict[str, Any]:
+    def run(self, data: Dict[str, Dict[str, Any]], debug: bool = False) -> Dict[str, Any]:
         """
         Runs the pipeline.
 
         Args:
             data: the inputs to give to the input components of the Pipeline.
             parameters: a dictionary with all the parameters of all the components, namespaced by component.
             debug: whether to collect and return debug information.
 
         Returns:
             A dictionary with the outputs of the output components of the Pipeline.
 
         Raises:
             PipelineRuntimeError: if the any of the components fail or return unexpected output.
         """
-        parameters = self._validate_parameters(parameters=parameters)
-        self.warm_up()
-        self._validate_pipeline()
-
         # **** The Pipeline.run() algorithm ****
         #
         # Nodes are run as soon as an input for them appears in the inputs buffer.
-        # When there's more than a node at once  in the buffer (which means some
+        # When there's more than a node at once in the buffer (which means some
         # branches are running in parallel or that there are loops) they are selected to
         # run in FIFO order by the `inputs_buffer` OrderedDict.
         #
         # Inputs are labeled with the name of the node they're aimed for:
         #
         #   ````
-        #   inputs_buffer[target_node] = [(input_edge, input_value), ...]
+        #   inputs_buffer[target_node] = {"input_name": input_value, ...}
         #   ```
         #
         # Nodes should wait until all the necessary input data has arrived before running.
         # If they're popped from the input_buffer before they're ready, they're put back in.
         # If the pipeline has branches of different lengths, it's possible that a node has to
         # wait a bit and let other nodes pass before receiving all the input data it needs.
         #
-        # Data access:
+        # Chetsheet for networkx data access:
         # - Name of the node       # self.graph.nodes  (List[str])
         # - Node instance          # self.graph.nodes[node]["instance"]
         # - Input nodes            # [e[0] for e in self.graph.in_edges(node)]
         # - Output nodes           # [e[1] for e in self.graph.out_edges(node)]
         # - Output edges           # [e[2]["label"] for e in self.graph.out_edges(node, data=True)]
+        #
+        # if debug:
+        #     os.makedirs("debug", exist_ok=True)
+
+        data = validate_pipeline_input(self.graph, inputs_values=data)
+        self._clear_visits_count()
+        self.warm_up()
+
         logger.info("Pipeline execution started.")
-        inputs_buffer: OrderedDict = OrderedDict()
+        inputs_buffer = OrderedDict(data)
+        pipeline_output: Dict[str, Dict[str, Any]] = {}
 
-        for node_name in locate_pipeline_input_components(self.graph):
-            # NOTE: We allow users to pass dictionaries just for convenience.
-            # The real input format is List[Tuple[str, Any]], to allow several input edges to have the same name.
-            if isinstance(data, dict):
-                data = list(data.items())
-            inputs_buffer[node_name] = {"data": data, "parameters": parameters}
+        if debug:
+            logger.info("Debug mode ON.")
+            self.debug = {}
 
         # *** PIPELINE EXECUTION LOOP ***
-        # We select the nodes to run by checking which keys are set in the
-        # inputs buffer. If the key exists, the node might be ready to run.
-        pipeline_results: Dict[str, List[Dict[str, Any]]] = {}
+        # We select the nodes to run by popping them in FIFO order from the inputs buffer.
+        step = 0
         while inputs_buffer:
-            logger.debug("> Current component queue: %s", inputs_buffer.keys())
+            step += 1
+            if debug:
+                self.debug[step] = {
+                    "time": datetime.datetime.now(),
+                    "inputs_buffer": list(inputs_buffer.items()),
+                    "pipeline_output": pipeline_output,
+                }
+            logger.debug("> Queue at step %s: %s", step, {k: list(v.keys()) for k, v in inputs_buffer.items()})
 
-            node_name, node_inputs = inputs_buffer.popitem(last=False)  # FIFO
+            component, inputs = inputs_buffer.popitem(last=False)  # FIFO
 
-            # Check if we looped over this node too many times
-            self._check_max_loops(node_name)
+            # if debug:
+            #     draw(deepcopy(self.graph), engine="graphviz", path=f"debug/step_{current_step}.jpg", running=component, queued=inputs_buffer.keys())
 
-            ready_to_run, inputs_buffer = self._ready_to_run(
-                component_name=node_name, component_inputs=node_inputs, inputs_buffer=inputs_buffer
-            )
-            if not ready_to_run:
-                continue
+            # **** IS IT MY TURN YET? ****
+            # Check if the node should be run or not
+            ready_to_run = self._ready_to_run(name=component, inputs=inputs, inputs_buffer=inputs_buffer)
 
-            # **** RUN THE NODE ****
-            # It is our turn! The node is ready to run and all inputs are ready
-            #
-            # Let's raise the visits count
-            self.graph.nodes[node_name]["visits"] += 1
-
-            # Check for default parameters and add them to the parameter's dictionary
-            # Default parameters are the one passed with the `pipeline.add_node()` method
-            # and have lower priority with respect to parameters passed through `pipeline.run()`
-            # or the modifications made by other nodes along the pipeline.
-            if self.graph.nodes[node_name]["parameters"]:
-                node_inputs["parameters"][node_name] = {
-                    **(self.graph.nodes[node_name]["parameters"] or {}),
-                    **parameters.get(node_name, {}),
-                }
+            # This component is missing data: let's put it back in the queue and wait.
+            if ready_to_run == "wait":
+                inputs_buffer[component] = inputs
+                continue
 
-            # Get the node
-            node_node = self.graph.nodes[node_name]["instance"]
+            # This component did not receive the input it needs: it must be on a skipped branch. Let's not run it.
+            if ready_to_run == "skip":
+                self.graph.nodes[component]["visits"] += 1
+                inputs_buffer = self._skip_downstream_nodes(component=component, inputs_buffer=inputs_buffer)
+                continue
 
-            # Call the node
-            try:
-                logger.info(
-                    "* Running %s (visits: %s)",
-                    node_name,
-                    self.graph.nodes[node_name]["visits"],
-                )
-                logger.debug("   '%s' inputs: %s", node_name, node_inputs)
-                node_results: Tuple[Dict[str, Any], Dict[str, Dict[str, Any]]]
-                node_results = node_node.run(
-                    name=node_name, data=node_inputs["data"], parameters=node_inputs["parameters"]
-                )
-                logger.debug("   '%s' outputs: %s\n", node_name, node_results)
-            except Exception as e:
-                raise PipelineRuntimeError(
-                    f"{node_name} raised '{e.__class__.__name__}: {e}' \ninputs={node_inputs['data']}\nparameters={node_inputs.get('parameters', None)}\n\n"
-                    "See the stacktrace above for more information."
-                ) from e
+            # **** RUN THE NODE ****
+            # It is our turn! The node is ready to run and all necessary inputs are present
+            output = self._run_component(name=component, inputs=inputs)
 
             # **** PROCESS THE OUTPUT ****
             # The node run successfully. Let's store or distribute the output it produced, if it's valid.
-            #
-            # Type-check the output
-            if (
-                len(node_results) != 2
-                or not isinstance(node_results[0], dict)
-                or not isinstance(node_results[1], dict)
-                or not all(isinstance(params, dict) for params in node_results[1].values())
-            ):
-                logger.debug("Component's output is malformed:\n%s", node_results)
-                raise PipelineRuntimeError(
-                    f"The component '{node_name}' did not return proper output. Check out the '@component' docstring."
-                )
-
-            # Process the output of the node
-            if not self.graph.out_edges(node_name):
-                # If there are no output edges, the output of this node is the output of the pipeline:
-                # store it in pipeline_results.
-                if not node_name in pipeline_results.keys():
-                    pipeline_results[node_name] = []
-                # We use append() to account for the case in which a node outputs several times
-                # (for example, it can happen if there's a loop upstream). The list gets unwrapped before
-                # returning it if there's only one output.
-                pipeline_results[node_name].append(node_results[0])
+            if not self.graph.out_edges(component):
+                # Note: if a node outputs many times (like in loops), the output will be overwritten
+                pipeline_output[component] = output
             else:
                 inputs_buffer = self._route_output(
-                    node_results=node_results, node_name=node_name, inputs_buffer=inputs_buffer
+                    node_results=output, node_name=component, inputs_buffer=inputs_buffer
                 )
 
-        logger.info("Pipeline executed successfully.")
-
-        # Simplify output for single edge, single output pipelines
-        pipeline_results = self._unwrap_results(pipeline_results)
-        return pipeline_results
+        if debug:
+            self.debug[step + 1] = {
+                "time": datetime.datetime.now(),
+                "inputs_buffer": list(inputs_buffer.items()),
+                "pipeline_output": pipeline_output,
+            }
+            pipeline_output["_debug"] = self.debug  # type: ignore
 
-    def _validate_parameters(self, parameters: Optional[Dict[str, Dict[str, Any]]]) -> Dict[str, Dict[str, Any]]:
-        """
-        Validate the input parameters.
-        """
-        if not parameters:
-            return {}
-
-        if any(node not in self.graph.nodes for node in parameters.keys()):
-            logging.warning(
-                "You passed parameters for one or more component(s) that do not exist in the pipeline: %s",
-                [node for node in parameters.keys() if node not in self.graph.nodes],
-            )
-        return parameters
+        logger.info("Pipeline executed successfully.")
+        return pipeline_output
 
-    def _validate_pipeline(self):
+    def _clear_visits_count(self):
         """
-        Make sure the pipeline has at least one input component and one output component.
+        Make sure all nodes's visits count is zero.
         """
-        if not locate_pipeline_input_components(self.graph):
-            raise ValueError("This pipeline has no input components!")
-
-        if not locate_pipeline_output_components(self.graph):
-            raise ValueError("This pipeline has no output components!")
+        for node in self.graph.nodes:
+            self.graph.nodes[node]["visits"] = 0
 
     def _check_max_loops(self, component_name: str):
         """
         Verify whether this component run too many times.
         """
         if self.graph.nodes[component_name]["visits"] > self.max_loops_allowed:
             raise PipelineMaxLoops(
                 f"Maximum loops count ({self.max_loops_allowed}) exceeded for component '{component_name}'."
             )
 
     def _ready_to_run(
-        self, component_name: str, component_inputs: Dict[str, Any], inputs_buffer: OrderedDict
-    ) -> Tuple[bool, OrderedDict]:
+        self, name: str, inputs: Dict[str, Any], inputs_buffer: OrderedDict
+    ) -> Literal["run", "wait", "skip"]:
         """
         Verify whether a component is ready to run.
 
-        Returns true if the component should run, false otherwise, and the updated inputs buffer.
+        Returns 'run', 'wait' or 'skip' depending on how the node should be treated and the log message explaining
+        the decision.
         """
-        # List all the inputs the current node should be waiting for.
-        inputs_received = [i[0] for i in component_inputs["data"]]
+        # Make sure it didn't run too many times already
+        self._check_max_loops(name)
 
-        # We should be wait on all edges except for the downstream ones, to support loops.
-        # This downstream check is enabled only for nodes taking more than one input
-        # (the "entrance" of the loop).
-        is_merge_node = len(self.graph.in_edges(component_name)) != 1
-        data_to_wait_for = [
-            (e[0], e[2]["label"])  # the node and the edge label
-            for e in self.graph.in_edges(component_name, data=True)  # for all input edges
-            # if there's a path in the graph leading back from the current node to the
-            # input node, in case of multiple input nodes.
-            if not is_merge_node or not nx.has_path(self.graph, component_name, e[0])
-        ]
+        # List all the component/socket pairs the current component should be waiting for.
+        expected_inputs = self._connections_to_wait_for(name=name)
 
-        if not data_to_wait_for:
-            # This is an input node, so it's ready to run.
-            logger.debug("'%s' is an input component and it's ready to run.")
-            return (True, inputs_buffer)
-
-        # Do we have all the inputs we expect?
-        nodes_to_wait_for, inputs_to_wait_for = zip(*data_to_wait_for)
-        if sorted(inputs_to_wait_for) == sorted(inputs_received):
-            return (True, inputs_buffer)
+        # Check if the expected inputs were all received
+        if self._check_received_vs_expected_inputs(name=name, inputs=inputs, expected_inputs=expected_inputs):
+            return "run"
+
+        # This node is missing some inputs. Did all the upstream nodes run?
+        nodes_to_wait_for, _ = zip(*expected_inputs) if expected_inputs else ([], [])
+
+        # Some node upstream didn't run yet, so we should wait for them.
+        if not self._all_nodes_to_wait_for_run(nodes_to_wait_for=nodes_to_wait_for):
+
+            if not inputs_buffer:
+                # What if there are no components to wait for?
+                raise PipelineRuntimeError(
+                    f"'{name}' is stuck waiting for input, but there are no other components to run. "
+                    "This is likely a Canals bug. Open an issue at https://github.com/deepset-ai/canals."
+                )
 
-        # This node is missing some inputs.
-        #
-        # Did all the upstream nodes run?
-        if not all(self.graph.nodes[node_to_wait_for]["visits"] > 0 for node_to_wait_for in nodes_to_wait_for):
-            # Some node upstream didn't run yet, so we should wait for them.
             logger.debug(
-                "Putting '%s' back in the queue, some inputs are missing "
-                "(inputs to wait for: %s, inputs_received: %s)",
-                component_name,
-                inputs_to_wait_for,
-                inputs_received,
+                "Putting '%s' back in the queue, some inputs are missing (inputs to wait for: %s, inputs_received: %s)",
+                name,
+                [f"{node}.{socket}" for node, socket in expected_inputs],
+                list(inputs.keys()),
             )
-            # Put back the node in the inputs buffer at the back...
-            inputs_buffer[component_name] = component_inputs
-            # ... and do not run this node (yet)
-            return (False, inputs_buffer)
+            return "wait"
 
         # All upstream nodes run, so it **must** be our turn.
-        #
-        # Are we missing ALL inputs or just a few?
-        if not inputs_received:
-            # ALL upstream nodes have been skipped.
-            #
-            # Let's skip this node and add all downstream nodes to the queue.
-            self.graph.nodes[component_name]["visits"] += 1
+        # However we're missing data, so this branch probably is being skipped.
+        if inputs and self.graph.nodes[name]["variadic_input"]:
             logger.debug(
-                "Skipping '%s', all input components were skipped and no inputs were received "
-                "(skipped components: %s, inputs: %s)",
-                component_name,
-                nodes_to_wait_for,
-                inputs_to_wait_for,
+                "Running '%s', even though some upstream component did not produced output. "
+                "(upstream components: %s, expected inputs: %s, n. of inputs received %s)",
+                name,
+                list(nodes_to_wait_for),
+                [f"{node}.{socket}" for node, socket in expected_inputs],
+                len(list(inputs.values())[0]) if inputs else 0,
             )
-            # Put all downstream nodes in the inputs buffer...
-            downstream_nodes = [e[1] for e in self.graph.out_edges(component_name)]
-            for downstream_node in downstream_nodes:
-                if not downstream_node in inputs_buffer:
-                    inputs_buffer[downstream_node] = {
-                        "data": [],
-                        "parameters": {},
-                    }
-            # ... and never run this node
-            return (False, inputs_buffer)
-
-        # If all nodes upstream have run and we received SOME input,
-        # this is a merge node that was waiting on a node that has been skipped, so it's ready to run.
-        # Let's pass None on the missing edges and go ahead.
-        #
-        # Example:
-        #
-        # --------------- value ----+
-        #                           |
-        #        +---X--- even ---+ |
-        #        |                | |
-        # -- parity_check         sum --
-        #        |                 |
-        #        +------ odd ------+
-        #
-        # If 'parity_check' produces output only on 'odd', 'sum' should run
-        # with 'value' and 'odd' only, because 'even' will never arrive.
-        #
-        inputs_to_wait_for = list(inputs_to_wait_for)
-        for input_expected in inputs_to_wait_for:
-            if input_expected in inputs_received:
-                inputs_to_wait_for.pop(inputs_to_wait_for.index(input_expected))
+            return "run"
+
         logger.debug(
-            "Some components upstream of '%s' were skipped, so some inputs will be None (missing inputs: %s)",
-            component_name,
-            inputs_to_wait_for,
+            "Skipping '%s', upstream component didn't produce output "
+            "(upstream components: %s, expected inputs: %s, inputs received: %s)",
+            name,
+            list(nodes_to_wait_for),
+            [f"{node}.{socket}" for node, socket in expected_inputs],
+            list(inputs.keys()),
         )
-        for missing_input in inputs_to_wait_for:
-            component_inputs["data"].append((missing_input, None))
+        return "skip"
+
+    def _check_received_vs_expected_inputs(
+        self, name: str, inputs: Dict[str, Any], expected_inputs: Tuple[str, str]
+    ) -> bool:
+        """
+        Check if all the inputs the component is expecting have been received.
+
+        Returns True if all the necessary inputs are received, False otherwise, and a message with the decision.
+        """
+        # Variadic nodes expect a single list regardless of how many incoming connections they have,
+        # but the length of the list should match the length of incoming connections.
+        if self.graph.nodes[name]["variadic_input"]:
+
+            # Variadic nodes need at least two values
+            if not inputs or len(inputs) < 2:
+                return False
+
+            if len(list(inputs.values())[0]) == len(expected_inputs):
+                logger.debug(
+                    "Component '%s' is ready to run: all connected inputs were received "
+                    "(expecting %s, received %s values).",
+                    name,
+                    len(expected_inputs),
+                    len(list(inputs.values())[0]),
+                )
+                return True
+        else:
+            # No input sockets are connected: this is an input node and should be always ready to run.
+            if not expected_inputs:
+                logger.debug("Component '%s' is ready to run: it's a starting node.", name)
+                return True
+
+            # Otherwise, just make sure there is one input key for each expected input key
+            _, expected_input_names = zip(*expected_inputs)
+            if set(expected_input_names).issubset(set(inputs.keys())):
+                logger.debug("Component '%s' is ready to run: all expected inputs were received.", name)
+                return True
 
-        return (True, inputs_buffer)
+        return False
+
+    def _connections_to_wait_for(self, name: str):
+        """
+        Return all the component/socket pairs this component is waiting for.
+        """
+        # We should be wait on all edges except for the downstream ones, to support loops.
+        # This downstream check is enabled only for nodes taking more than one input
+        # (the "entrance" of the loop).
+        data_to_wait_for = [
+            (from_node, data["to_socket"].name)
+            for from_node, _, data in self.graph.in_edges(name, data=True)
+            # ... if there's a path in the graph leading back from the current node to the
+            # input node, # and only in case this node accepts multiple inputs.
+            if not (nx.has_path(self.graph, name, from_node) and self.graph.nodes[name]["variadic_input"])
+        ]
+        return data_to_wait_for
+
+    def _all_nodes_to_wait_for_run(self, nodes_to_wait_for: List[str]) -> bool:
+        """
+        Check if all the nodes this component is waiting for has run or not.
+
+        FIXME: checking for `visits>0` might not be enough for all loops.
+        """
+        return all(self.graph.nodes[node_to_wait_for]["visits"] > 0 for node_to_wait_for in nodes_to_wait_for)
+
+    def _skip_downstream_nodes(self, component: str, inputs_buffer: OrderedDict) -> OrderedDict:
+        """
+        When a component is skipped, put all downstream nodes in the inputs buffer too: the might be skipped too,
+        unless they are merge/variadic nodes. They will be evaluated later by the pipeline execution loop.
+        """
+        downstream_nodes = [e[1] for e in self.graph.out_edges(component)]
+        for downstream_node in downstream_nodes:
+            if not downstream_node in inputs_buffer:
+                inputs_buffer[downstream_node] = {}
+        return inputs_buffer
+
+    def _run_component(self, name: str, inputs: Dict[str, Any]) -> Dict[str, Any]:
+        """
+        Once we're confident this component is ready to run, run it and collect the output.
+        """
+        self.graph.nodes[name]["visits"] += 1
+        instance = self.graph.nodes[name]["instance"]
+        try:
+            logger.info("* Running %s (visits: %s)", name, self.graph.nodes[name]["visits"])
+            logger.debug("   '%s' inputs: %s", name, inputs)
+
+            # If the node is variadic, unpack the input
+            if self.graph.nodes[name]["variadic_input"]:
+                inputs = list(inputs.values())[0]
+                output_dataclass = instance.run(*inputs)
+
+            # Otherwise pass the inputs as kwargs after adding the component's own defaults to them
+            else:
+                inputs = {**instance.defaults, **inputs}
+                output_dataclass = instance.run(**inputs)
+
+            # Unwrap the output
+            output = output_dataclass.__dict__
+            logger.debug("   '%s' outputs: %s\n", name, output)
+
+        except Exception as e:
+            raise PipelineRuntimeError(
+                f"{name} raised '{e.__class__.__name__}: {e}' \nInputs: {inputs}\n\n"
+                "See the stacktrace above for more information."
+            ) from e
+
+        return output
 
     def _route_output(
         self,
         node_name: str,
-        node_results: Tuple[Dict[str, Any], Dict[str, Dict[str, Any]]],
+        node_results: Dict[str, Any],
         inputs_buffer: OrderedDict,
     ) -> OrderedDict:
         """
         Distrubute the outputs of the component into the input buffer of downstream components.
 
         Returns the updated inputs buffer.
         """
         # This is not a terminal node: find out where the output goes, to which nodes and along which edge
         is_decision_node_for_loop = (
             any(nx.has_path(self.graph, edge[1], node_name) for edge in self.graph.out_edges(node_name))
             and len(self.graph.out_edges(node_name)) > 1
         )
         for edge_data in self.graph.out_edges(node_name, data=True):
-            edge = edge_data[2]["label"]
+            to_socket = edge_data[2]["to_socket"]
+            from_socket = edge_data[2]["from_socket"]
             target_node = edge_data[1]
 
             # If this is a decision node and a loop is involved, we add to the input buffer only the nodes
             # that received their expected output and we leave the others out of the queue.
-            if is_decision_node_for_loop and not edge in node_results[0].keys():
+            if is_decision_node_for_loop and node_results[from_socket.name] is None:
                 if nx.has_path(self.graph, target_node, node_name):
                     # In case we're choosing to leave a loop, do not put the loop's node in the buffer.
                     logger.debug(
                         "Not adding '%s' to the inputs buffer: we're leaving the loop.",
                         target_node,
                     )
                 else:
@@ -663,36 +575,17 @@
                         "Not adding '%s' to the inputs buffer: we're staying in the loop.",
                         target_node,
                     )
             else:
                 # In all other cases, populate the inputs buffer for all downstream nodes, setting None to any
                 # edge that did not receive input.
                 if not target_node in inputs_buffer:
-                    inputs_buffer[target_node] = {
-                        "data": []
-                    }  # Create the buffer for the downstream node if it's not there yet
-                if edge in node_results[0].keys():
-                    inputs_buffer[target_node]["data"].append((edge, node_results[0][edge]))
-                inputs_buffer[target_node]["parameters"] = node_results[1]
+                    inputs_buffer[target_node] = {}  # Create the buffer for the downstream node if it's not there yet
+                if node_results.get(from_socket.name, None):
+                    if to_socket.variadic:
+                        if not to_socket.name in inputs_buffer[target_node].keys():
+                            inputs_buffer[target_node][to_socket.name] = []
+                        inputs_buffer[target_node][to_socket.name].append(node_results[from_socket.name])
+                    else:
+                        inputs_buffer[target_node][to_socket.name] = node_results[from_socket.name]
 
         return inputs_buffer
-
-    def _unwrap_results(self, pipeline_results):
-        """
-        Simplifies the output of simple Pipelines:
-
-        - if the resuklt contains output of a single component, unwraps the dictionary to return the list only
-        - if the resulting list is only composed of one dictionary, returns the internal dictionary only.
-
-        So the output of `Pipeline.run()` might look like:
-
-        - Multi-component output: `{component: [{key: value, ... }, ... ], ... }`
-        - Single-component, repeated output: `[{key: value, ... }, ... ]`
-        - Single-component, single output: `{key: value, ... }`
-        """
-        if len(pipeline_results.keys()) == 1:
-            pipeline_results = pipeline_results[list(pipeline_results.keys())[0]]  # type: ignore
-
-            if len(pipeline_results) == 1:
-                pipeline_results = pipeline_results[0]  # type: ignore
-
-        return pipeline_results
```

### Comparing `canals-0.0.3/canals/pipeline/save_load.py` & `canals-0.1.0/canals/pipeline/save_load.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+# pylint: disable=protected-access
+
 from typing import Dict, List, Any, Tuple
 
 import sys
 import json
 import logging
 from pathlib import Path
 from inspect import getmembers, isclass, getmodule, ismodule
@@ -89,33 +91,27 @@
             # If no pointer was made in the previous step
             if not component_name in pipeline_repr["components"]:
                 # Save the components in the global components list
                 components.append((pipeline_name, component_name, component_instance))
                 # Serialize the components
                 component_repr = {
                     "type": component_instance.__class__.__name__,
-                    "init_parameters": component_instance.init_parameters,
+                    "init_parameters": component_instance._init_parameters,
                 }
                 pipeline_repr["components"][component_name] = component_repr
 
-            # Check for run parameters
-            if pipeline.graph.nodes[component_name]["parameters"]:
-                pipeline_repr["components"][component_name]["run_parameters"] = pipeline.graph.nodes[component_name][
-                    "parameters"
-                ]
-
         pipeline_repr["connections"] = list(pipeline.graph.edges)
         schema["pipelines"][pipeline_name] = pipeline_repr
 
     # Collect the dependencies
     schema["dependencies"] = _discover_dependencies(components=[component[2] for component in components])
     return schema
 
 
-def unmarshal_pipelines(schema: Dict[str, Any]) -> Dict[str, Pipeline]:
+def unmarshal_pipelines(schema: Dict[str, Any]) -> Dict[str, Pipeline]:  # pylint: disable=too-many-locals
     """
     Loads the content of a schema generated by `marshal_pipelines()` into
     a dictionary of named Pipelines.
 
     Args:
         schema: the schema of the pipelines, as generated by `marshal_pipelines()`.
 
@@ -145,28 +141,29 @@
 
         # Create the components or fish them from the buffer
         for component_name, component_schema in pipeline_schema["components"].items():
             if "refer_to" in component_schema.keys():
                 pipe.add_component(
                     name=component_name,
                     instance=component_instances[component_schema["refer_to"]],
-                    parameters=component_schema.get("run_parameters", {}),
                 )
             else:
                 component_class = classes[component_schema["type"]]
                 component_instance = component_class(**component_schema.get("init_parameters", {}))
                 component_instances[f"{pipeline_name}.{component_name}"] = component_instance
                 pipe.add_component(
                     name=component_name,
                     instance=component_instance,
-                    parameters=component_schema.get("run_parameters", {}),
                 )
 
-        for edge in pipeline_schema["connections"]:
-            pipe.connect(*edge)
+        for connect_from, connect_to, sockets in pipeline_schema["connections"]:
+            output_socket, input_socket = sockets.split("/", maxsplit=1)
+            connect_from += "." + output_socket
+            connect_to += "." + input_socket
+            pipe.connect(connect_from=connect_from, connect_to=connect_to)
 
         pipelines[pipeline_name] = pipe
 
     return pipelines
 
 
 def _discover_dependencies(components: List[object]) -> List[str]:
```

### Comparing `canals-0.0.3/docs/index.md` & `canals-0.1.0/docs/index.md`

 * *Files 12% similar despite different names*

```diff
@@ -19,13 +19,19 @@
 
 ```console
 pip install canals
 ```
 
 gives you the bare minimum necessary to run Canals.
 
-To be able to draw pipelines, please make sure you have [graphviz](https://graphviz.org/download/) installed:
+To be able to draw pipelines, please make sure you have either an internet connection (to reach the Mermaid graph renderer at `https://mermaid.ink`) or [graphviz](https://graphviz.org/download/) installed and then install Canals as:
 
+### Mermaid
 ```console
-sudo apt install graphviz  # You may need `graphviz-dev` too: sudo apt install graphviz-dev
-pip install canals[draw]
+pip install canals[mermaid]
+```
+
+### GraphViz
+```console
+sudo apt install graphviz  # You may need `graphviz-dev` too
+pip install canals[graphviz]
 ```
```

### Comparing `canals-0.0.3/docs/concepts/concepts.md` & `canals-0.1.0/docs/concepts/concepts.md`

 * *Files 26% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Components and Pipelines
+# Core concepts
 
 Canals is a **component orchestration engine**. It can be used to connect a group of smaller objects, called Components,
 that perform well-defined tasks into a network, called Pipeline, to achieve a larger goal.
 
 Components are Python objects that can execute a task, like reading a file, performing calculations, or making API
 calls. Canals connects these objects together: it builds a graph of components and takes care of managing their
 execution order, making sure that each object receives the input it expects from the other components of the pipeline.
@@ -12,111 +12,96 @@
 ## What is a Component?
 
 A Component is a Python class that performs a well-defined task: for example a REST API call, a mathematical operation,
 a data trasformation, writing something to a file or a database, and so on.
 
 To be recognized as a Component by Canals, a Python class needs to respect these rules:
 
-1. Must be decorated with the `@component` decorator
-2. Declare its inputs and outputs in the `__init__` function.
-3. Must have a `run()` method with a specific signature
-4. Must return output that Canals can interpret.
+1. Must be decorated with the `@component` decorator.
+3. Have a `run()` method with all the inputs and outputs typed.
+4. Must return a pre-defined dataclass called `Output`.
 
-For example, the following is a Component that sums up all its inputs:
+For example, the following is a Component that sums up two numbers:
 
 ```python
+from dataclasses import dataclass
 from canals import component
 
-# The mandatory 'component' decorator
 @component
-class Sum:
+class AddTwoValues:
     """
-    A Canals component that takes some input numbers and outputs their sum.
+    Adds the value of `add` to `value`. If not given, `add` defaults to 1.
     """
 
-    def __init__(
-        self,
-        input_names: str = ["first_number", "second_number"],
-        output_name: str = "value"
-    ):
-        # self.inputs and self.outputs are required by Canals
-        self.inputs = input_names
-        self.outputs = [output_name]
-        # self.init_parameters = {"input_names": input_names, "output_name": output_name}
-
-    # The signature of the run() method must be exactly this.
-    def run(
-        self,
-        name: str,  # The name of the component in the pipeline
-        data: List[Tuple[str, Any]],    # The data from other components
-        parameters: Dict[str, Any],     # All the parameters of all the nodes in the pipeline
-    ):
-        # Let's sum the values of all the inputs we've got
-        for _, value in data:
-            value += add
-
-        # We declared one output in the __init__, so the output should be:
-        # - a dictionary with that key
-        # - the parameters dictionary we received in input.
-        return ({self.outputs[0]: value}, parameters)
+    @dataclass
+    class Output:
+        value: int
+
+    def __init__(self, add: int = 1):
+        self.defaults = {"add": add}
+
+    def run(self, value: int, add: int) -> Output:
+        return AddTwoValues.Output(value=value + add)
 ```
 
 We will see the details of all of these requirements below.
 
 ## What is a Pipeline?
 
 A Pipeline is a network of Components. Pipelines define what components receive and send output to which other, makes
 sure all the connections are valid, and takes care of calling the component's `run()` method in the right order.
 
 Pipeline connects compoonents together through so-called connections, which are the edges of the pipeline graph.
 Pipeline is going to make sure that all the connections are valid based on the inputs and output that Components have
-declared (with their `self.inputs` and `self.outputs` attributes).
+declared.
 
-For example, if a component produces a value called `document`, among others, and another component expects an input
-called `document`, among others, Pipeline will be able to connect them. Otherwise, it will raise an exception.
+For example, if a component produces a value of type `List[Document]` and another component expects an input
+of type `List[Document]`, Pipeline will be able to connect them. Otherwise, it will raise an exception.
 
 This is a simple example of how a Pipeline is created:
 
 
 ```python
 from canals import Pipeline, component
 
 # Some Canals components
-from my_components import Sum, MultiplyBy
+from my_components import AddTwoValues, MultiplyTwoValues
 
-#
 pipeline = Pipeline()
 
 # Components can be initialized as standalone objects.
 # These instances can be added to the Pipeline in several places.
-multiplication = MultiplyBy(input_name="value", output_name="value", multiply_by=2)
-addition = Sum(input_names=["value", "value"], output_name="value")
+multiplication = MultiplyBy(multiply_by=2)
+addition = AddTwoValues(add=1)
 
 # Components are added with a name and an component
-pipeline.add_component("double", multiplication, input_component=True)
-pipeline.add_component("first_addition", addition, input_component=True)
-pipeline.add_component("second_addition", addition)  # Component instances can be reused
+pipeline.add_component("double", multiplication)
+pipeline.add_component("add_one", addition)
+pipeline.add_component("add_one_again", addition)  # Component instances can be reused
+pipeline.add_component("add_two", AddTwoValues(add=2))
 
 # Connect the components together
-pipeline.connect(connect_from="double", connect_to="first_addition")
-pipeline.connect(connect_from="double", connect_to="second_addition")
-pipeline.connect(connect_from="first_addition", connect_to="second_addition")
+pipeline.connect(connect_from="double", connect_to="add_one")
+pipeline.connect(connect_from="add_one", connect_to="add_one_again")
+pipeline.connect(connect_from="add_one_again", connect_to="add_two")
+
+# Pipeline can be drawn
+pipeline.draw("pipeline.jpg")
 
 # Pipelines are run by giving them the data that the input nodes expect.
-results = pipeline.run(data={"value": 1})
+results = pipeline.run(data={"double":{"value": 1}})
 
 print(results)
 
-# prints {"value": 5}
+# prints {"add_two": {"value": 6}}
 ```
 
 This is how the pipeline's graph looks like:
 
 ```mermaid
-graph TD
-I((input)) -- value --> B(first_addition)
-I((input)) -- value --> A(double)
-A -- value --> B
-A -- value --> C
-B -- value --> C(second addition)
-C -- value --> O((output))
+graph TD;
+double -- value -> value --> add_one
+add_one -- value -> value --> add_one_again
+add_one_again -- value -> value --> add_two
+IN([input]) -- value --> double
+add_two -- value --> OUT([output])
 ```
```

### Comparing `canals-0.0.3/images/canals-logo-dark.png` & `canals-0.1.0/images/canals-logo-dark.png`

 * *Files identical despite different names*

### Comparing `canals-0.0.3/images/canals-logo-light.png` & `canals-0.1.0/images/canals-logo-light.png`

 * *Files identical despite different names*

### Comparing `canals-0.0.3/test/test_save_load.py` & `canals-0.1.0/test/test_save_load.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,76 +1,73 @@
-from pathlib import Path
-
 import pytest
 
 from canals.pipeline import Pipeline, marshal_pipelines, unmarshal_pipelines
-from test.components import AddValue, Double
+from test.test_components import AddFixedValue, Double
 
 import logging
 
 logging.basicConfig(level=logging.DEBUG)
 
 
 def test_marshal():
-    add_1 = AddValue(add=1)
-    add_2 = AddValue(add=1)
+    add_1 = AddFixedValue(add=200)
+    add_2 = AddFixedValue()
 
     pipeline_1 = Pipeline(metadata={"type": "test pipeline", "author": "me"})
-    pipeline_1.add_component("first_addition", add_2, parameters={"add": 6})
-    pipeline_1.add_component("double", Double(input="value"))
-    pipeline_1.add_component("second_addition", add_1)
-    pipeline_1.add_component("third_addition", add_2)
+    pipeline_1.add_component("first_addition", add_1)
+    pipeline_1.add_component("double", Double())
+    pipeline_1.add_component("second_addition", add_2)
+    pipeline_1.add_component("third_addition", add_1)
 
     pipeline_1.connect("first_addition", "double")
     pipeline_1.connect("double", "second_addition")
     pipeline_1.connect("second_addition", "third_addition")
 
     pipeline_2 = Pipeline(metadata={"type": "another test pipeline", "author": "you"})
-    pipeline_2.add_component("first_addition", add_2, parameters={"add": 4})
-    pipeline_2.add_component("double", Double(input="value"))
-    pipeline_2.add_component("second_addition", add_1)
+    pipeline_2.add_component("first_addition", add_1)
+    pipeline_2.add_component("double", Double())
+    pipeline_2.add_component("second_addition", add_2)
 
     pipeline_2.connect("first_addition", "double")
     pipeline_2.connect("double", "second_addition")
 
     assert marshal_pipelines(pipelines={"pipe1": pipeline_1, "pipe2": pipeline_2}) == {
         "pipelines": {
             "pipe1": {
                 "metadata": {"type": "test pipeline", "author": "me"},
                 "max_loops_allowed": 100,
                 "components": {
                     "first_addition": {
-                        "type": "AddValue",
-                        "init_parameters": {"add": 1},
-                        "run_parameters": {"add": 6},
+                        "type": "AddFixedValue",
+                        "init_parameters": {"add": 200},
                     },
-                    "double": {"type": "Double", "init_parameters": {"input": "value"}},
+                    "double": {"type": "Double", "init_parameters": {}},
                     "second_addition": {
-                        "type": "AddValue",
-                        "init_parameters": {"add": 1},
+                        "type": "AddFixedValue",
+                        "init_parameters": {},
                     },
                     "third_addition": {"refer_to": "pipe1.first_addition"},
                 },
                 "connections": [
-                    ("first_addition", "double"),
-                    ("double", "second_addition"),
-                    ("second_addition", "third_addition"),
+                    ("first_addition", "double", "value/value"),
+                    ("double", "second_addition", "value/value"),
+                    ("second_addition", "third_addition", "value/value"),
                 ],
             },
             "pipe2": {
                 "metadata": {"type": "another test pipeline", "author": "you"},
                 "max_loops_allowed": 100,
                 "components": {
-                    "first_addition": {"refer_to": "pipe1.first_addition", "run_parameters": {"add": 4}},
-                    "double": {"type": "Double", "init_parameters": {"input": "value"}},
+                    "first_addition": {"refer_to": "pipe1.first_addition"},
+                    "double": {"type": "Double", "init_parameters": {}},
                     "second_addition": {"refer_to": "pipe1.second_addition"},
                 },
                 "connections": [
-                    ("first_addition", "double"),
-                    ("double", "second_addition"),
+                    ("first_addition", "double", "value/value"),
+                    ("double", "second_addition", "value/value"),
                 ],
             },
         },
         "dependencies": ["test", "canals"],
     }
 
 
@@ -79,100 +76,92 @@
         {
             "pipelines": {
                 "pipe1": {
                     "metadata": {"type": "test pipeline", "author": "me"},
                     "max_loops_allowed": 100,
                     "components": {
                         "first_addition": {
-                            "type": "AddValue",
-                            "init_parameters": {"add": 1, "input": "value", "output": "value"},
-                            "run_parameters": {"add": 6},
+                            "type": "AddFixedValue",
+                            "init_parameters": {"add": 300},
                         },
-                        "double": {"type": "Double", "init_parameters": {"input": "value", "output": "value"}},
+                        "double": {"type": "Double"},
                         "second_addition": {
-                            "type": "AddValue",
-                            "init_parameters": {"add": 1, "input": "value", "output": "value"},
+                            "type": "AddFixedValue",
+                            "init_parameters": {},
                         },
                         "third_addition": {"refer_to": "pipe1.first_addition"},
                     },
                     "connections": [
-                        ("first_addition", "double"),
-                        ("double", "second_addition"),
-                        ("second_addition", "third_addition"),
+                        ("first_addition", "double", "value/value"),
+                        ("double", "second_addition", "value/value"),
+                        ("second_addition", "third_addition", "value/value"),
                     ],
                 },
                 "pipe2": {
                     "metadata": {"type": "another test pipeline", "author": "you"},
                     "max_loops_allowed": 100,
                     "components": {
-                        "first_addition": {"refer_to": "pipe1.first_addition", "run_parameters": {"add": 4}},
-                        "double": {"type": "Double", "init_parameters": {"input": "value", "output": "value"}},
+                        "first_addition": {"refer_to": "pipe1.first_addition"},
+                        "double": {"type": "Double"},
                         "second_addition": {"refer_to": "pipe1.second_addition"},
                     },
                     "connections": [
-                        ("first_addition", "double"),
-                        ("double", "second_addition"),
+                        ("first_addition", "double", "value/value"),
+                        ("double", "second_addition", "value/value"),
                     ],
                 },
             },
             "dependencies": ["test", "canals"],
         }
     )
 
     pipe1 = pipelines["pipe1"]
     assert pipe1.metadata == {"type": "test pipeline", "author": "me"}
 
     first_addition = pipe1.get_component("first_addition")
-    assert type(first_addition["instance"]) == AddValue
-    assert first_addition["instance"].add == 1
-    assert first_addition["parameters"] == {"add": 6}
+    assert type(first_addition) == AddFixedValue
+    assert first_addition.defaults["add"] == 300
 
     second_addition = pipe1.get_component("second_addition")
-    assert type(second_addition["instance"]) == AddValue
-    assert second_addition["instance"].add == 1
-    assert second_addition["parameters"] == {}
-    assert second_addition["instance"] != first_addition["instance"]
+    assert type(second_addition) == AddFixedValue
+    assert second_addition.defaults["add"] == 1
+    assert second_addition != first_addition
 
     third_addition = pipe1.get_component("third_addition")
-    assert type(third_addition["instance"]) == AddValue
-    assert third_addition["instance"].add == 1
-    assert third_addition["parameters"] == {}
-    assert third_addition["instance"] == first_addition["instance"]
+    assert type(third_addition) == AddFixedValue
+    assert third_addition.defaults["add"] == 300
+    assert third_addition == first_addition
 
     double = pipe1.get_component("double")
-    assert type(double["instance"]) == Double
-    assert double["parameters"] == {}
+    assert type(double) == Double
 
     assert list(pipe1.graph.edges) == [
-        ("first_addition", "double"),
-        ("double", "second_addition"),
-        ("second_addition", "third_addition"),
+        ("first_addition", "double", "value/value"),
+        ("double", "second_addition", "value/value"),
+        ("second_addition", "third_addition", "value/value"),
     ]
 
     pipe2 = pipelines["pipe2"]
     assert pipe2.metadata == {"type": "another test pipeline", "author": "you"}
 
     first_addition_2 = pipe2.get_component("first_addition")
-    assert type(first_addition_2["instance"]) == AddValue
-    assert first_addition_2["instance"].add == 1
-    assert first_addition_2["parameters"] == {"add": 4}
-    assert first_addition_2["instance"] == first_addition["instance"]
+    assert type(first_addition_2) == AddFixedValue
+    assert first_addition_2.defaults["add"] == 300
+    assert first_addition_2 == first_addition
 
     second_addition_2 = pipe2.get_component("second_addition")
-    assert type(second_addition_2["instance"]) == AddValue
-    assert second_addition_2["instance"].add == 1
-    assert second_addition_2["parameters"] == {}
-    assert second_addition_2["instance"] != first_addition_2["instance"]
-    assert second_addition_2["instance"] == second_addition["instance"]
+    assert type(second_addition_2) == AddFixedValue
+    assert second_addition_2.defaults["add"] == 1
+    assert second_addition_2 != first_addition_2
+    assert second_addition_2 == second_addition
 
     with pytest.raises(ValueError):
         pipe2.get_component("third_addition")
 
     double_2 = pipe2.get_component("double")
-    assert type(double_2["instance"]) == Double
-    assert double_2["parameters"] == {}
-    assert double_2["instance"] != double["instance"]
+    assert type(double_2) == Double
+    assert double_2 != double
 
     assert list(pipe2.graph.edges) == [
-        ("first_addition", "double"),
-        ("double", "second_addition"),
+        ("first_addition", "double", "value/value"),
+        ("double", "second_addition", "value/value"),
     ]
```

### Comparing `canals-0.0.3/test/components/__init__.py` & `canals-0.1.0/test/test_components/__init__.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,11 +1,11 @@
-from test.components.test_accumulate import Accumulate
-from test.components.test_add_value import AddValue
-from test.components.test_below import Below
-from test.components.test_double import Double
-from test.components.test_greet import Greet
-from test.components.test_merge import Merge
-from test.components.test_remainder import Remainder
-from test.components.test_rename import Rename
-from test.components.test_repeat import Repeat
-from test.components.test_subtract import Subtract
-from test.components.test_sum import Sum
+from test.test_components.test_accumulate import Accumulate
+from test.test_components.test_add_value import AddFixedValue
+from test.test_components.test_double import Double
+from test.test_components.test_parity import Parity
+from test.test_components.test_greet import Greet
+from test.test_components.test_merge_loop import MergeLoop
+from test.test_components.test_remainder import Remainder
+from test.test_components.test_repeat import Repeat
+from test.test_components.test_subtract import Subtract
+from test.test_components.test_sum import Sum
+from test.test_components.test_threshold import Threshold
```

### Comparing `canals-0.0.3/test/components/test_accumulate.py` & `canals-0.1.0/test/test_components/test_accumulate.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,47 +1,52 @@
-from typing import Dict, Any, List, Tuple, Union, Callable, Optional
+from typing import Union, Callable, Optional
 import sys
 import builtins
 from importlib import import_module
 
-from canals import component  # , non_serializable_component
+from dataclasses import dataclass
+from canals import component
 
 
 @component
 class Accumulate:
     """
     Accumulates the value flowing through the connection into an internal attribute.
+    The sum function can be customized.
 
     Example of how to deal with serialization when some of the parameters
     are not directly serializable.
 
     Stateful, single input, single output component.
-
-    :param connection: the connection to read the value from.
-    :param function: the function to use to accumulate the values.
-        The function must take exactly two values.
-        If it's a callable, it's used as it is.
-        If it's a string, the component will look for it in sys.modules and
-        import it at need. This is also a parameter.
     """
 
-    def __init__(self, connection: str, function: Optional[Union[Callable, str]] = None):
+    @dataclass
+    class Output:
+        value: int
+
+    def __init__(self, function: Optional[Union[Callable, str]] = None):
+        """
+        :param function: the function to use to accumulate the values.
+            The function must take exactly two values.
+            If it's a callable, it's used as it is.
+            If it's a string, the component will look for it in sys.modules and
+            import it at need. This is also a parameter.
+        """
         self.state = 0
 
         if function is None:
             self.function = lambda x, y: x + y
         else:
             self.function = self._load_function(function)
+            # 'function' is not serializable by default, so we serialize it manually.
+            self._init_parameters = {"function": self._save_function(function)}
 
-        # 'function' is not serializable normally, so we serialize it manually.
-        if "function" in self.init_parameters.keys():  # type: ignore
-            self.init_parameters["function"] = self._save_function(self.init_parameters["function"])  # type: ignore
-
-        self.inputs = [connection]
-        self.outputs = [connection]
+    def run(self, value: int) -> Output:
+        self.state = self.function(self.state, value)
+        return Accumulate.Output(value=self.state)
 
     def _load_function(self, function: Union[Callable, str]):
         """
         Loads the function by trying to import it.
         """
         if not isinstance(function, str):
             return function
@@ -63,45 +68,55 @@
         module = sys.modules.get(function.__module__)
         if not module:
             raise ValueError("Could not locate the import module.")
         if module == builtins:
             return function.__name__
         return f"{module.__name__}.{function.__name__}"
 
-    def run(self, name: str, data: List[Tuple[str, Any]], parameters: Dict[str, Any]):
-        function = parameters.get(name, {}).get("function", self.function)
-        self.state = function(self.state, data[0][1])
-        return ({data[0][0]: data[0][1]}, parameters)
-
 
 def test_accumulate_default():
-    component = Accumulate(connection="test")
-    results = component.run(name="test_component", data=[("test", 10)], parameters={})
-    assert results == ({"test": 10}, {})
+    component = Accumulate()
+    results = component.run(value=10)
+    assert results == Accumulate.Output(value=10)
     assert component.state == 10
-    assert component.init_parameters == {"connection": "test"}
+
+    results = component.run(value=1)
+    assert results == Accumulate.Output(value=11)
+    assert component.state == 11
+
+    assert component._init_parameters == {}
 
 
 def my_subtract(first, second):
     return first - second
 
 
 def test_accumulate_callable():
-    component = Accumulate(connection="test", function=my_subtract)
-    results = component.run(name="test_component", data=[("test", 10)], parameters={})
-    assert results == ({"test": 10}, {})
+    component = Accumulate(function=my_subtract)
+
+    results = component.run(value=10)
+    assert results == Accumulate.Output(value=-10)
     assert component.state == -10
-    assert component.init_parameters == {
-        "connection": "test",
-        "function": "test.components.test_accumulate.my_subtract",
+
+    results = component.run(value=1)
+    assert results == Accumulate.Output(value=-11)
+    assert component.state == -11
+
+    assert component._init_parameters == {
+        "function": "test.test_components.test_accumulate.my_subtract",
     }
 
 
 def test_accumulate_string():
-    component = Accumulate(connection="test", function="test.components.test_accumulate.my_subtract")
-    results = component.run(name="test_component", data=[("test", 10)], parameters={})
-    assert results == ({"test": 10}, {})
+    component = Accumulate(function="test.test_components.test_accumulate.my_subtract")
+
+    results = component.run(value=10)
+    assert results == Accumulate.Output(value=-10)
     assert component.state == -10
-    assert component.init_parameters == {
-        "connection": "test",
-        "function": "test.components.test_accumulate.my_subtract",
+
+    results = component.run(value=1)
+    assert results == Accumulate.Output(value=-11)
+    assert component.state == -11
+
+    assert component._init_parameters == {
+        "function": "test.test_components.test_accumulate.my_subtract",
     }
```

### Comparing `canals-0.0.3/test/pipelines/_test_looping_and_merge_pipeline.py` & `canals-0.1.0/test/pipelines/integration/test_looping_pipeline.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,44 +1,38 @@
 from typing import *
 from pathlib import Path
 from pprint import pprint
 
 from canals.pipeline import Pipeline
-from test.components import Accumulate, AddValue, Below, Merge, Sum
+from test.test_components import Accumulate, AddFixedValue, Threshold, MergeLoop
 
 import logging
 
 logging.basicConfig(level=logging.DEBUG)
 
 
 def test_pipeline(tmp_path):
-    accumulator = Accumulate(connection="value")
+    accumulator = Accumulate()
 
     pipeline = Pipeline(max_loops_allowed=10)
-    pipeline.add_component("merge", Merge(), input_component=True)
-    pipeline.add_component("sum", Sum(inputs=["value", "value"]), input_component=True)
-    pipeline.add_component("below_10", Below(threshold=10))
-    pipeline.add_component("add_one", AddValue(add=1, input="below"))
-    pipeline.add_component("counter", accumulator)
-    pipeline.add_component("add_two", AddValue(add=2, input="above"))
+    pipeline.add_component("merge", MergeLoop(expected_type=int))
+    pipeline.add_component("below_10", Threshold(threshold=10))
+    pipeline.add_component("accumulator", accumulator)
+    pipeline.add_component("add_two", AddFixedValue(add=2))
 
     pipeline.connect("merge", "below_10")
-    pipeline.connect("below_10.below", "add_one")
-    pipeline.connect("add_one", "counter")
-    pipeline.connect("counter", "merge")
-    pipeline.connect("below_10.above", "add_two")
-    pipeline.connect("add_two", "sum")
-
-    pipeline.draw(tmp_path / "looping_and_merge_pipeline.png")
-
-    results = pipeline.run(
-        {"value": 3},
-    )
+    pipeline.connect("below_10.below", "accumulator")
+    pipeline.connect("accumulator", "merge")
+    pipeline.connect("below_10.above", "add_two.value")
+
+    pipeline.draw(tmp_path / "looping_pipeline.png")
+
+    results = pipeline.run({"merge": {"value": 4}})
     pprint(results)
-    print("accumulate: ", accumulator.state)
+    print("accumulator: ", accumulator.state)
 
-    assert results == {"sum": 15}
-    assert accumulator.state == 7
+    assert results == {"add_two": {"value": 18}}
+    assert accumulator.state == 16
 
 
 if __name__ == "__main__":
     test_pipeline(Path(__file__).parent)
```

### Comparing `canals-0.0.3/test/pipelines/test_decision_and_merge_pipeline.py` & `canals-0.1.0/test/pipelines/integration/test_variable_decision_pipeline.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,44 +1,38 @@
-import logging
 from pathlib import Path
 from pprint import pprint
 
 from canals.pipeline import Pipeline
-from test.components import AddValue, Remainder, Double, Sum
+from test.test_components import AddFixedValue, Remainder, Double
+
+import logging
 
 logging.basicConfig(level=logging.DEBUG)
 
 
 def test_pipeline(tmp_path):
-    add_one = AddValue(add=1, input="value")
+    add_one = AddFixedValue(add=1)
 
     pipeline = Pipeline()
     pipeline.add_component("add_one", add_one)
-    pipeline.add_component("remainder", Remainder(input="value", divisor=3))
-    pipeline.add_component("add_ten", AddValue(add=10, input="0"))
-    pipeline.add_component("double", Double(input="1", output="value"))
-    pipeline.add_component("add_three", AddValue(add=3, input="2"))
+    pipeline.add_component("remainder", Remainder(divisor=3))
+    pipeline.add_component("add_ten", AddFixedValue(add=10))
+    pipeline.add_component("double", Double())
+    pipeline.add_component("add_three", AddFixedValue(add=3))
     pipeline.add_component("add_one_again", add_one)
-    pipeline.add_component("sum", Sum(inputs=["value"] * 4), input_component=True)
 
     pipeline.connect("add_one", "remainder")
-    pipeline.connect("remainder.0", "add_ten")
-    pipeline.connect("remainder.1", "double")
-    pipeline.connect("add_ten", "sum")
-    pipeline.connect("double", "sum")
-    pipeline.connect("remainder.2", "add_three")
+    pipeline.connect("remainder.remainder_is_0", "add_ten.value")
+    pipeline.connect("remainder.remainder_is_1", "double")
+    pipeline.connect("remainder.remainder_is_2", "add_three.value")
     pipeline.connect("add_three", "add_one_again")
-    pipeline.connect("add_one_again", "sum")
 
-    try:
-        pipeline.draw(tmp_path / "decision_and_merge_pipeline.png")
-    except ImportError:
-        logging.warning("pygraphviz not found, pipeline is not being drawn.")
+    pipeline.draw(tmp_path / "variable_decision_pipeline.png")
 
-    results = pipeline.run({"value": 1})
+    results = pipeline.run({"add_one": {"value": 1}})
     pprint(results)
 
-    assert results == {"sum": 7}
+    assert results == {"add_one_again": {"value": 6}}
 
 
 if __name__ == "__main__":
     test_pipeline(Path(__file__).parent)
```

### Comparing `canals-0.0.3/test/pipelines/test_decision_pipeline.py` & `canals-0.1.0/test/pipelines/integration/test_variable_decision_and_merge_pipeline.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,41 +1,45 @@
+import logging
 from pathlib import Path
 from pprint import pprint
 
 from canals.pipeline import Pipeline
-from test.components import AddValue, Remainder, Double
-
-import logging
+from test.test_components import AddFixedValue, Remainder, Double, Sum
 
 logging.basicConfig(level=logging.DEBUG)
 
 
 def test_pipeline(tmp_path):
-    add_one = AddValue(add=1)
+    add_one = AddFixedValue()
 
     pipeline = Pipeline()
     pipeline.add_component("add_one", add_one)
-    pipeline.add_component("remainder", Remainder(input="value", divisor=3))
-    pipeline.add_component("add_ten", AddValue(add=10, input="0"))
-    pipeline.add_component("double", Double(input="1", output="value"))
-    pipeline.add_component("add_three", AddValue(add=3, input="2"))
+    pipeline.add_component("parity", Remainder())
+    pipeline.add_component("add_ten", AddFixedValue(add=10))
+    pipeline.add_component("double", Double())
+    pipeline.add_component("add_four", AddFixedValue(add=4))
     pipeline.add_component("add_one_again", add_one)
+    pipeline.add_component("sum", Sum())
 
-    pipeline.connect("add_one", "remainder")
-    pipeline.connect("remainder.0", "add_ten")
-    pipeline.connect("remainder.1", "double")
-    pipeline.connect("remainder.2", "add_three")
-    pipeline.connect("add_three", "add_one_again")
-
-    try:
-        pipeline.draw(tmp_path / "decision_pipeline.png")
-    except ImportError:
-        logging.warning("pygraphviz not found, pipeline is not being drawn.")
+    pipeline.connect("add_one", "parity")
+    pipeline.connect("parity.remainder_is_0", "add_ten.value")
+    pipeline.connect("parity.remainder_is_1", "double")
+    pipeline.connect("add_one", "sum")
+    pipeline.connect("add_ten", "sum")
+    pipeline.connect("double", "sum")
+    pipeline.connect("parity.remainder_is_1", "add_four.value")
+    pipeline.connect("add_four", "add_one_again")
+    pipeline.connect("add_one_again", "sum")
 
-    results = pipeline.run({"value": 1})
+    pipeline.draw(tmp_path / "variable_decision_and_merge_pipeline.png")
+
+    results = pipeline.run({"add_one": {"value": 1}})
     pprint(results)
+    assert results == {"sum": {"total": 14}}
 
-    assert results == {"value": 6}
+    results = pipeline.run({"add_one": {"value": 2}})
+    pprint(results)
+    assert results == {"sum": {"total": 17}}
 
 
 if __name__ == "__main__":
     test_pipeline(Path(__file__).parent)
```

### Comparing `canals-0.0.3/test/pipelines/test_linear_pipeline.py` & `canals-0.1.0/test/pipelines/integration/test_linear_pipeline.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,32 +1,29 @@
 from pathlib import Path
 from pprint import pprint
 
 from canals.pipeline import Pipeline
-from test.components import AddValue, Double
+from test.test_components import AddFixedValue, Double
 
 import logging
 
 logging.basicConfig(level=logging.DEBUG)
 
 
 def test_pipeline(tmp_path):
     pipeline = Pipeline()
-    pipeline.add_component("first_addition", AddValue(add=2))
-    pipeline.add_component("second_addition", AddValue(add=1))
-    pipeline.add_component("double", Double(input="value"))
+    pipeline.add_component("first_addition", AddFixedValue(add=2))
+    pipeline.add_component("second_addition", AddFixedValue())
+    pipeline.add_component("double", Double())
     pipeline.connect("first_addition", "double")
     pipeline.connect("double", "second_addition")
 
-    try:
-        pipeline.draw(tmp_path / "linear_pipeline.png")
-    except ImportError:
-        logging.warning("pygraphviz not found, pipeline is not being drawn.")
+    pipeline.draw(tmp_path / "linear_pipeline.png")
 
-    results = pipeline.run({"value": 1})
+    results = pipeline.run({"first_addition": {"value": 1}})
     pprint(results)
 
-    assert results == {"value": 7}
+    assert results == {"second_addition": {"value": 7}}
 
 
 if __name__ == "__main__":
     test_pipeline(Path(__file__).parent)
```

### Comparing `canals-0.0.3/test/pipelines/test_looping_pipeline.py` & `canals-0.1.0/test/pipelines/integration/test_looping_and_merge_pipeline.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,45 +1,44 @@
 from typing import *
 from pathlib import Path
 from pprint import pprint
 
 from canals.pipeline import Pipeline
-from test.components import Accumulate, AddValue, Below, Merge
+from test.test_components import Accumulate, AddFixedValue, Threshold, Sum, MergeLoop
 
 import logging
 
 logging.basicConfig(level=logging.DEBUG)
 
 
 def test_pipeline(tmp_path):
-    accumulator = Accumulate(connection="value")
+    accumulator = Accumulate()
 
     pipeline = Pipeline(max_loops_allowed=10)
-    pipeline.add_component("merge", Merge(inputs=["value", "value"]), input_component=True)
-    pipeline.add_component("below_10", Below(threshold=10))
-    pipeline.add_component("add_one", AddValue(add=1, input="below"))
-    pipeline.add_component("accumulator", accumulator)
-    pipeline.add_component("add_two", AddValue(add=2, input="above"))
+    pipeline.add_component("merge", MergeLoop(expected_type=int))
+    pipeline.add_component("sum", Sum())
+    pipeline.add_component("below_10", Threshold(threshold=10))
+    pipeline.add_component("add_one", AddFixedValue(add=1))
+    pipeline.add_component("counter", accumulator)
+    pipeline.add_component("add_two", AddFixedValue(add=2))
 
     pipeline.connect("merge", "below_10")
-    pipeline.connect("below_10.below", "add_one")
-    pipeline.connect("add_one", "accumulator")
-    pipeline.connect("accumulator", "merge")
-    pipeline.connect("below_10.above", "add_two")
-
-    try:
-        pipeline.draw(tmp_path / "looping_pipeline.png")
-    except ImportError:
-        logging.warning("pygraphviz not found, pipeline is not being drawn.")
+    pipeline.connect("below_10.below", "add_one.value")
+    pipeline.connect("add_one", "counter")
+    pipeline.connect("counter", "merge")
+    pipeline.connect("below_10.above", "add_two.value")
+    pipeline.connect("add_two", "sum")
+
+    pipeline.draw(tmp_path / "looping_and_merge_pipeline.png")
 
     results = pipeline.run(
-        {"value": 3},
+        {"merge": {"value": 8}, "sum": {"value": 2}},
     )
     pprint(results)
-    print("accumulator: ", accumulator.state)
+    print("accumulate: ", accumulator.state)
 
-    assert results == {"value": 12}
-    assert accumulator.state == 49
+    assert results == {"sum": {"total": 23}}
+    assert accumulator.state == 19
 
 
 if __name__ == "__main__":
     test_pipeline(Path(__file__).parent)
```

### Comparing `canals-0.0.3/test/pipelines/test_merging_pipeline.py` & `canals-0.1.0/test/pipelines/integration/test_variable_merging_pipeline.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,41 +1,44 @@
 from pathlib import Path
 from pprint import pprint
 
 from canals.pipeline import Pipeline
-from test.components import AddValue, Sum
+from test.test_components import AddFixedValue, Sum
 
 import logging
 
 logging.basicConfig(level=logging.DEBUG)
 
 
 def test_pipeline(tmp_path):
 
-    add_two = AddValue(add=2)
-    make_the_sum = Sum(inputs=["value"] * 2)
+    add_two = AddFixedValue(add=2)
+    make_the_sum = Sum()
 
     pipeline = Pipeline()
     pipeline.add_component("first_addition", add_two)
     pipeline.add_component("second_addition", add_two)
     pipeline.add_component("third_addition", add_two)
     pipeline.add_component("sum", make_the_sum)
-    pipeline.add_component("fourth_addition", AddValue(add=1, input="sum"))
+    pipeline.add_component("fourth_addition", AddFixedValue(add=1))
 
     pipeline.connect("first_addition", "second_addition")
+    pipeline.connect("first_addition", "sum")
     pipeline.connect("second_addition", "sum")
     pipeline.connect("third_addition", "sum")
-    pipeline.connect("sum", "fourth_addition")
+    pipeline.connect("sum", "fourth_addition.value")
 
-    try:
-        pipeline.draw(tmp_path / "merging_pipeline.png")
-    except ImportError:
-        logging.warning("pygraphviz not found, pipeline is not being drawn.")
+    pipeline.draw(tmp_path / "variable_merging_pipeline.png")
 
-    results = pipeline.run({"value": 1})
+    results = pipeline.run(
+        {
+            "first_addition": {"value": 1},
+            "third_addition": {"value": 1},
+        }
+    )
     pprint(results)
 
-    assert results == {"value": 9}
+    assert results == {"fourth_addition": {"value": 12}}
 
 
 if __name__ == "__main__":
     test_pipeline(Path(__file__).parent)
```

### Comparing `canals-0.0.3/.gitignore` & `canals-0.1.0/.gitignore`

 * *Files identical despite different names*

### Comparing `canals-0.0.3/LICENSE` & `canals-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `canals-0.0.3/README.md` & `canals-0.1.0/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -18,13 +18,19 @@
 
 ```console
 pip install canals
 ```
 
 gives you the bare minimum necessary to run Canals.
 
-To be able to draw pipelines, please make sure you have [graphviz](https://graphviz.org/download/) installed:
+To be able to draw pipelines, please make sure you have either an internet connection (to reach the Mermaid graph renderer at `https://mermaid.ink`) or [graphviz](https://graphviz.org/download/) installed and then install Canals as:
 
+### Mermaid
 ```console
-sudo apt install graphviz  # You may need `graphviz-dev` too: sudo apt install graphviz-dev
-pip install canals[draw]
+pip install canals[mermaid]
+```
+
+### GraphViz
+```console
+sudo apt install graphviz  # You may need `graphviz-dev` too
+pip install canals[graphviz]
 ```
```

### Comparing `canals-0.0.3/pyproject.toml` & `canals-0.1.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -26,47 +26,49 @@
 ]
 dynamic = ["version"]
 dependencies = [
   "networkx",  # Pipeline graphs
 ]
 
 [project.optional-dependencies]
-draw = [
+graphviz = [
   "pygraphviz", # Draw pipelines (requires the 'graphviz' system library)
 ]
+mermaid = [
+  "requests", # Draw pipelines (requires internet connectivity)
+]
 dev = [
   "hatch",
   "pre-commit",
   "mypy",
   "pylint==2.15.10",
   "black[jupyter]==22.6.0",
   "pytest",
   "coverage",
 ]
 docs = [
   "mkdocs-material",
   "mkdocstrings[python]",
   "mkdocs-mermaid2-plugin"
-
 ]
-all = ["canals[draw,dev]"]
 
 
 [project.urls]
 Documentation = "https://github.com/deepset-ai/canals#readme"
 Issues = "https://github.com/deepset-ai/canals/issues"
 Source = "https://github.com/deepset-ai/canals"
 
 [tool.hatch.version]
 path = "canals/__about__.py"
 
 [tool.hatch.envs.default]
 dependencies = [
   "pytest",
   "pytest-cov",
+  "requests",
 ]
 [tool.hatch.envs.default.scripts]
 cov = "pytest --cov-report=term-missing --cov-config=pyproject.toml --cov=canals --cov=tests {args}"
 no-cov = "cov --no-cov {args}"
 
 [[tool.hatch.envs.test.matrix]]
 python = ["38", "39", "310", "311"]
@@ -89,14 +91,13 @@
 line-length = 120
 
 [tool.pylint.'MESSAGES CONTROL']
 max-line-length=120
 good-names="e"
 max-args=10
 disable = [
-  "unused-argument", # REMOVE ME
   "fixme",
   "line-too-long",
   "missing-class-docstring",
   "missing-module-docstring",
   "consider-iterating-dictionary",  # horrible style imho :)
 ]
```

### Comparing `canals-0.0.3/PKG-INFO` & `canals-0.1.0/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: canals
-Version: 0.0.3
+Version: 0.1.0
 Summary: A component orchestration engine for Haystack
 Project-URL: Documentation, https://github.com/deepset-ai/canals#readme
 Project-URL: Issues, https://github.com/deepset-ai/canals/issues
 Project-URL: Source, https://github.com/deepset-ai/canals
 Author-email: ZanSara <sara.zanzottera@deepset.ai>
 License-Expression: Apache-2.0
 License-File: LICENSE
@@ -16,30 +16,30 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Requires-Python: >=3.8
 Requires-Dist: networkx
-Provides-Extra: all
-Requires-Dist: canals[dev,draw]; extra == 'all'
 Provides-Extra: dev
 Requires-Dist: black[jupyter]==22.6.0; extra == 'dev'
 Requires-Dist: coverage; extra == 'dev'
 Requires-Dist: hatch; extra == 'dev'
 Requires-Dist: mypy; extra == 'dev'
 Requires-Dist: pre-commit; extra == 'dev'
 Requires-Dist: pylint==2.15.10; extra == 'dev'
 Requires-Dist: pytest; extra == 'dev'
 Provides-Extra: docs
 Requires-Dist: mkdocs-material; extra == 'docs'
 Requires-Dist: mkdocs-mermaid2-plugin; extra == 'docs'
 Requires-Dist: mkdocstrings[python]; extra == 'docs'
-Provides-Extra: draw
-Requires-Dist: pygraphviz; extra == 'draw'
+Provides-Extra: graphviz
+Requires-Dist: pygraphviz; extra == 'graphviz'
+Provides-Extra: mermaid
+Requires-Dist: requests; extra == 'mermaid'
 Description-Content-Type: text/markdown
 
 # Canals
 
 <p align="center" float="left">
   <img alt="" src="https://raw.githubusercontent.com/deepset-ai/canals/main/images/canals-logo-light.png#gh-dark-mode-only"/>
   <img alt="" src="https://raw.githubusercontent.com/deepset-ai/canals/main/images/canals-logo-dark.png#gh-light-mode-only"/>
@@ -58,13 +58,19 @@
 
 ```console
 pip install canals
 ```
 
 gives you the bare minimum necessary to run Canals.
 
-To be able to draw pipelines, please make sure you have [graphviz](https://graphviz.org/download/) installed:
+To be able to draw pipelines, please make sure you have either an internet connection (to reach the Mermaid graph renderer at `https://mermaid.ink`) or [graphviz](https://graphviz.org/download/) installed and then install Canals as:
 
+### Mermaid
 ```console
-sudo apt install graphviz  # You may need `graphviz-dev` too: sudo apt install graphviz-dev
-pip install canals[draw]
+pip install canals[mermaid]
+```
+
+### GraphViz
+```console
+sudo apt install graphviz  # You may need `graphviz-dev` too
+pip install canals[graphviz]
 ```
```

