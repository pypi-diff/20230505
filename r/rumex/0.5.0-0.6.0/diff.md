# Comparing `tmp/rumex-0.5.0.tar.gz` & `tmp/rumex-0.6.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rumex-0.5.0.tar", max compression
+gzip compressed data, was "rumex-0.6.0.tar", max compression
```

## Comparing `rumex-0.5.0.tar` & `rumex-0.6.0.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rw-r--r--   0        0        0     1211 2022-10-01 01:54:46.296415 rumex-0.5.0/LICENSE
--rw-r--r--   0        0        0     1520 2023-04-23 22:18:05.688768 rumex-0.5.0/README.rst
--rw-r--r--   0        0        0      916 2023-05-03 23:39:13.199906 rumex-0.5.0/pyproject.toml
--rw-r--r--   0        0        0      133 2023-05-03 23:39:13.199906 rumex-0.5.0/rumex/__init__.py
--rw-r--r--   0        0        0        0 2022-10-01 01:54:46.296415 rumex-0.5.0/rumex/parsing/__init__.py
--rw-r--r--   0        0        0     3493 2023-05-03 23:39:13.199906 rumex-0.5.0/rumex/parsing/builder.py
--rw-r--r--   0        0        0     1032 2023-05-03 23:39:13.199906 rumex-0.5.0/rumex/parsing/core.py
--rw-r--r--   0        0        0     8906 2023-05-03 23:39:13.199906 rumex-0.5.0/rumex/parsing/parser.py
--rw-r--r--   0        0        0      990 2023-05-02 00:37:46.737147 rumex-0.5.0/rumex/parsing/table.py
--rw-r--r--   0        0        0     2797 2023-05-03 23:39:13.199906 rumex-0.5.0/rumex/parsing/tokenizer.py
--rw-r--r--   0        0        0    13747 2023-05-03 23:39:13.199906 rumex-0.5.0/rumex/runner.py
--rw-r--r--   0        0        0     1423 2023-04-23 21:55:25.650645 rumex-0.5.0/rumex/tests/__init__.py
--rw-r--r--   0        0        0     4206 2023-04-23 21:55:25.650645 rumex-0.5.0/rumex/tests/test_data.py
--rw-r--r--   0        0        0      810 2023-04-04 00:34:13.843051 rumex-0.5.0/rumex/tests/test_error_reporting.py
--rw-r--r--   0        0        0     2749 2023-05-03 23:39:13.199906 rumex-0.5.0/rumex/tests/test_execution.py
--rw-r--r--   0        0        0     5554 2023-04-24 20:26:14.685112 rumex-0.5.0/rumex/tests/test_no_execution_cases.py
--rw-r--r--   0        0        0     6717 2023-05-03 23:39:13.199906 rumex-0.5.0/rumex/tests/test_simple_execution.py
--rw-r--r--   0        0        0      894 2023-02-16 02:20:09.255404 rumex-0.5.0/rumex/utils.py
--rw-r--r--   0        0        0     1851 1970-01-01 00:00:00.000000 rumex-0.5.0/PKG-INFO
+-rw-r--r--   0        0        0      721 2023-05-05 01:19:14.413580 rumex-0.6.0/LICENSE
+-rw-r--r--   0        0        0     1835 2023-05-05 01:19:14.413580 rumex-0.6.0/README.rst
+-rw-r--r--   0        0        0      916 2023-05-05 01:19:14.417580 rumex-0.6.0/pyproject.toml
+-rw-r--r--   0        0        0      133 2023-05-05 01:19:14.417580 rumex-0.6.0/rumex/__init__.py
+-rw-r--r--   0        0        0        0 2022-10-01 01:54:46.296415 rumex-0.6.0/rumex/parsing/__init__.py
+-rw-r--r--   0        0        0     3493 2023-05-03 23:39:13.199906 rumex-0.6.0/rumex/parsing/builder.py
+-rw-r--r--   0        0        0     1032 2023-05-03 23:39:13.199906 rumex-0.6.0/rumex/parsing/core.py
+-rw-r--r--   0        0        0     8906 2023-05-03 23:39:13.199906 rumex-0.6.0/rumex/parsing/parser.py
+-rw-r--r--   0        0        0      990 2023-05-02 00:37:46.737147 rumex-0.6.0/rumex/parsing/table.py
+-rw-r--r--   0        0        0     2797 2023-05-03 23:39:13.199906 rumex-0.6.0/rumex/parsing/tokenizer.py
+-rw-r--r--   0        0        0    13962 2023-05-05 01:19:14.417580 rumex-0.6.0/rumex/runner.py
+-rw-r--r--   0        0        0     1423 2023-04-23 21:55:25.650645 rumex-0.6.0/rumex/tests/__init__.py
+-rw-r--r--   0        0        0     4206 2023-04-23 21:55:25.650645 rumex-0.6.0/rumex/tests/test_data.py
+-rw-r--r--   0        0        0      810 2023-04-04 00:34:13.843051 rumex-0.6.0/rumex/tests/test_error_reporting.py
+-rw-r--r--   0        0        0     2749 2023-05-03 23:39:13.199906 rumex-0.6.0/rumex/tests/test_execution.py
+-rw-r--r--   0        0        0     5554 2023-04-24 20:26:14.685112 rumex-0.6.0/rumex/tests/test_no_execution_cases.py
+-rw-r--r--   0        0        0     6717 2023-05-03 23:39:13.199906 rumex-0.6.0/rumex/tests/test_simple_execution.py
+-rw-r--r--   0        0        0     2390 2023-05-05 01:19:14.417580 rumex-0.6.0/rumex/utils.py
+-rw-r--r--   0        0        0     2166 1970-01-01 00:00:00.000000 rumex-0.6.0/PKG-INFO
```

### Comparing `rumex-0.5.0/README.rst` & `rumex-0.6.0/README.rst`

 * *Files 18% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 =====
 Rumex
 =====
 
 `Behaviour Driven Development`_ (BDD) testing library.
 
-Rumex is a lightweight library alternative to the `behave`_ framework.
+Rumex is trying to be more of a library rather than a framework.
+This approach aims to increase flexibility and reduce dependency
+on design choices made by designers of alternative frameworks.
 
 
 Basic example
 -------------
 
 .. code:: python
 
@@ -59,24 +61,36 @@
         context_maker=Context,
     )
 
 
 More examples
 ~~~~~~~~~~~~~
 
-See `docs/examples`_
+Perhaps the best way to discover Rumex's fetures is to look at the examples:
+
+`docs/examples`_
 
 
 API
 ---
 
-For complete API documentation see `docs/api`_
+For API documentation see `docs/api`_
+
+
+Some alternatives
+-----------------
+
+- `behave`_
+
+- `pytest-bdd`_
 
 
 .. _`Behaviour Driven Development`:
   https://en.wikipedia.org/wiki/Behavior-driven_development
 
-.. _`behave`: https://github.com/behave/behave
-
 .. _`docs/examples`: docs/examples
 
 .. _`docs/api`: docs/api.rst
+
+.. _`behave`: https://github.com/behave/behave
+
+.. _`pytest-bdd`: https://github.com/pytest-dev/pytest-bdd
```

### Comparing `rumex-0.5.0/pyproject.toml` & `rumex-0.6.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "rumex"
-version = "0.5.0"
+version = "0.6.0"
 
 description = ""
 authors = ["uigctaw <uigctaw@metadata.social>"]
 readme = "README.rst"
 
 
 [tool.poetry.dependencies]
```

### Comparing `rumex-0.5.0/rumex/parsing/builder.py` & `rumex-0.6.0/rumex/parsing/builder.py`

 * *Files identical despite different names*

### Comparing `rumex-0.5.0/rumex/parsing/core.py` & `rumex-0.6.0/rumex/parsing/core.py`

 * *Files identical despite different names*

### Comparing `rumex-0.5.0/rumex/parsing/parser.py` & `rumex-0.6.0/rumex/parsing/parser.py`

 * *Files identical despite different names*

### Comparing `rumex-0.5.0/rumex/parsing/table.py` & `rumex-0.6.0/rumex/parsing/table.py`

 * *Files identical despite different names*

### Comparing `rumex-0.5.0/rumex/parsing/tokenizer.py` & `rumex-0.6.0/rumex/parsing/tokenizer.py`

 * *Files identical despite different names*

### Comparing `rumex-0.5.0/rumex/runner.py` & `rumex-0.6.0/rumex/runner.py`

 * *Files 1% similar despite different names*

```diff
@@ -271,29 +271,39 @@
             name=parsed_file.name,
             description=parsed_file.description,
     )
 
 
 def report(files):
     for file in files:
-        if not file.success:
-            raise AssertionError(file)
+        if file.success:
+            continue
+
+        for scenario in file.scenarios:
+            if scenario.success:
+                continue
+
+            for step_ in scenario.steps:
+                if step_.success:
+                    continue
+
+                raise step_.exception
 
 
 def run(
         *,
         files: Iterable[InputFile],
         steps: StepMapperProto,
         context_maker: Callable[[], Any] | None = None,
         parser: ParserProto = parse,
         executor: ExecutorProto = execute_file,
         reporter=report,
         map_=map,
 ):
-    """Rumex entry point for running tests.
+    """Entry point for running tests.
 
     Params
     ------
     files: Files to be parsed and executed.
 
     steps: See `StepMapper` or `StepMapperProto` for more info.
```

### Comparing `rumex-0.5.0/rumex/tests/__init__.py` & `rumex-0.6.0/rumex/tests/__init__.py`

 * *Files identical despite different names*

### Comparing `rumex-0.5.0/rumex/tests/test_data.py` & `rumex-0.6.0/rumex/tests/test_data.py`

 * *Files identical despite different names*

### Comparing `rumex-0.5.0/rumex/tests/test_error_reporting.py` & `rumex-0.6.0/rumex/tests/test_error_reporting.py`

 * *Files identical despite different names*

### Comparing `rumex-0.5.0/rumex/tests/test_execution.py` & `rumex-0.6.0/rumex/tests/test_execution.py`

 * *Files identical despite different names*

### Comparing `rumex-0.5.0/rumex/tests/test_no_execution_cases.py` & `rumex-0.6.0/rumex/tests/test_no_execution_cases.py`

 * *Files identical despite different names*

### Comparing `rumex-0.5.0/rumex/tests/test_simple_execution.py` & `rumex-0.6.0/rumex/tests/test_simple_execution.py`

 * *Files identical despite different names*

### Comparing `rumex-0.5.0/PKG-INFO` & `rumex-0.6.0/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rumex
-Version: 0.5.0
+Version: 0.6.0
 Summary: 
 Author: uigctaw
 Author-email: uigctaw@metadata.social
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
@@ -12,15 +12,17 @@
 
 =====
 Rumex
 =====
 
 `Behaviour Driven Development`_ (BDD) testing library.
 
-Rumex is a lightweight library alternative to the `behave`_ framework.
+Rumex is trying to be more of a library rather than a framework.
+This approach aims to increase flexibility and reduce dependency
+on design choices made by designers of alternative frameworks.
 
 
 Basic example
 -------------
 
 .. code:: python
 
@@ -71,25 +73,37 @@
         context_maker=Context,
     )
 
 
 More examples
 ~~~~~~~~~~~~~
 
-See `docs/examples`_
+Perhaps the best way to discover Rumex's fetures is to look at the examples:
+
+`docs/examples`_
 
 
 API
 ---
 
-For complete API documentation see `docs/api`_
+For API documentation see `docs/api`_
+
+
+Some alternatives
+-----------------
+
+- `behave`_
+
+- `pytest-bdd`_
 
 
 .. _`Behaviour Driven Development`:
   https://en.wikipedia.org/wiki/Behavior-driven_development
 
-.. _`behave`: https://github.com/behave/behave
-
 .. _`docs/examples`: docs/examples
 
 .. _`docs/api`: docs/api.rst
 
+.. _`behave`: https://github.com/behave/behave
+
+.. _`pytest-bdd`: https://github.com/pytest-dev/pytest-bdd
+
```

