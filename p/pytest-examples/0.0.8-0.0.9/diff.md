# Comparing `tmp/pytest_examples-0.0.8.tar.gz` & `tmp/pytest_examples-0.0.9.tar.gz`

## Comparing `pytest_examples-0.0.8.tar` & `pytest_examples-0.0.9.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0     1237 2020-02-02 00:00:00.000000 pytest_examples-0.0.8/Makefile
--rw-r--r--   0        0        0     1866 2020-02-02 00:00:00.000000 pytest_examples-0.0.8/pytest_examples/__init__.py
--rw-r--r--   0        0        0     3113 2020-02-02 00:00:00.000000 pytest_examples-0.0.8/pytest_examples/config.py
--rw-r--r--   0        0        0     9028 2020-02-02 00:00:00.000000 pytest_examples-0.0.8/pytest_examples/eval_example.py
--rw-r--r--   0        0        0     6211 2020-02-02 00:00:00.000000 pytest_examples-0.0.8/pytest_examples/find_examples.py
--rw-r--r--   0        0        0     3224 2020-02-02 00:00:00.000000 pytest_examples-0.0.8/pytest_examples/lint.py
--rw-r--r--   0        0        0     1899 2020-02-02 00:00:00.000000 pytest_examples-0.0.8/pytest_examples/modify_files.py
--rw-r--r--   0        0        0    11286 2020-02-02 00:00:00.000000 pytest_examples-0.0.8/pytest_examples/run_code.py
--rw-r--r--   0        0        0     3672 2020-02-02 00:00:00.000000 pytest_examples-0.0.8/pytest_examples/traceback.py
--rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 pytest_examples-0.0.8/requirements/all.txt
--rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 pytest_examples-0.0.8/requirements/linting.in
--rw-r--r--   0        0        0      928 2020-02-02 00:00:00.000000 pytest_examples-0.0.8/requirements/linting.txt
--rw-r--r--   0        0        0      685 2020-02-02 00:00:00.000000 pytest_examples-0.0.8/requirements/pyproject.txt
--rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 pytest_examples-0.0.8/requirements/testing.in
--rw-r--r--   0        0        0      741 2020-02-02 00:00:00.000000 pytest_examples-0.0.8/requirements/testing.txt
--rw-r--r--   0        0        0      264 2020-02-02 00:00:00.000000 pytest_examples-0.0.8/.gitignore
--rw-r--r--   0        0        0     1105 2020-02-02 00:00:00.000000 pytest_examples-0.0.8/LICENSE
--rw-r--r--   0        0        0     3124 2020-02-02 00:00:00.000000 pytest_examples-0.0.8/README.md
--rw-r--r--   0        0        0     2346 2020-02-02 00:00:00.000000 pytest_examples-0.0.8/pyproject.toml
--rw-r--r--   0        0        0     4362 2020-02-02 00:00:00.000000 pytest_examples-0.0.8/PKG-INFO
+-rw-r--r--   0        0        0     1237 2020-02-02 00:00:00.000000 pytest_examples-0.0.9/Makefile
+-rw-r--r--   0        0        0     1866 2020-02-02 00:00:00.000000 pytest_examples-0.0.9/pytest_examples/__init__.py
+-rw-r--r--   0        0        0     3113 2020-02-02 00:00:00.000000 pytest_examples-0.0.9/pytest_examples/config.py
+-rw-r--r--   0        0        0     9145 2020-02-02 00:00:00.000000 pytest_examples-0.0.9/pytest_examples/eval_example.py
+-rw-r--r--   0        0        0     6221 2020-02-02 00:00:00.000000 pytest_examples-0.0.9/pytest_examples/find_examples.py
+-rw-r--r--   0        0        0     3224 2020-02-02 00:00:00.000000 pytest_examples-0.0.9/pytest_examples/lint.py
+-rw-r--r--   0        0        0     1899 2020-02-02 00:00:00.000000 pytest_examples-0.0.9/pytest_examples/modify_files.py
+-rw-r--r--   0        0        0    11645 2020-02-02 00:00:00.000000 pytest_examples-0.0.9/pytest_examples/run_code.py
+-rw-r--r--   0        0        0     3672 2020-02-02 00:00:00.000000 pytest_examples-0.0.9/pytest_examples/traceback.py
+-rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 pytest_examples-0.0.9/requirements/all.txt
+-rw-r--r--   0        0        0       63 2020-02-02 00:00:00.000000 pytest_examples-0.0.9/requirements/linting.in
+-rw-r--r--   0        0        0      928 2020-02-02 00:00:00.000000 pytest_examples-0.0.9/requirements/linting.txt
+-rw-r--r--   0        0        0      685 2020-02-02 00:00:00.000000 pytest_examples-0.0.9/requirements/pyproject.txt
+-rw-r--r--   0        0        0       28 2020-02-02 00:00:00.000000 pytest_examples-0.0.9/requirements/testing.in
+-rw-r--r--   0        0        0      741 2020-02-02 00:00:00.000000 pytest_examples-0.0.9/requirements/testing.txt
+-rw-r--r--   0        0        0      264 2020-02-02 00:00:00.000000 pytest_examples-0.0.9/.gitignore
+-rw-r--r--   0        0        0     1105 2020-02-02 00:00:00.000000 pytest_examples-0.0.9/LICENSE
+-rw-r--r--   0        0        0     3124 2020-02-02 00:00:00.000000 pytest_examples-0.0.9/README.md
+-rw-r--r--   0        0        0     2346 2020-02-02 00:00:00.000000 pytest_examples-0.0.9/pyproject.toml
+-rw-r--r--   0        0        0     4362 2020-02-02 00:00:00.000000 pytest_examples-0.0.9/PKG-INFO
```

### Comparing `pytest_examples-0.0.8/Makefile` & `pytest_examples-0.0.9/Makefile`

 * *Files identical despite different names*

### Comparing `pytest_examples-0.0.8/pytest_examples/__init__.py` & `pytest_examples-0.0.9/pytest_examples/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 from pathlib import Path
 
 import pytest
 
 from .eval_example import EvalExample
 from .find_examples import CodeExample, find_examples
 
-__version__ = '0.0.8'
+__version__ = '0.0.9'
 __all__ = 'find_examples', 'CodeExample', 'EvalExample'
 
 
 def pytest_addoption(parser):
     group = parser.getgroup('examples')
     group.addoption(
         '--update-examples',
```

### Comparing `pytest_examples-0.0.8/pytest_examples/config.py` & `pytest_examples-0.0.9/pytest_examples/config.py`

 * *Files identical despite different names*

### Comparing `pytest_examples-0.0.8/pytest_examples/eval_example.py` & `pytest_examples-0.0.9/pytest_examples/eval_example.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from __future__ import annotations as _annotations
 
 from pathlib import Path
-from typing import TYPE_CHECKING, Any
+from typing import TYPE_CHECKING, Any, Callable
 
 import pytest
 from _pytest.assertion.rewrite import AssertionRewritingHook
 from _pytest.outcomes import Failed as PytestFailed
 
 from .config import DEFAULT_LINE_LENGTH, ExamplesConfig
 from .lint import FormatError, black_check, black_format, ruff_check, ruff_format
@@ -26,14 +26,15 @@
 
     def __init__(self, *, tmp_path: Path, pytest_request: pytest.FixtureRequest):
         self.tmp_path = tmp_path
         self._pytest_config = pytest_request.config
         self._test_id = pytest_request.node.nodeid
         self.to_update: list[CodeExample] = []
         self.config: ExamplesConfig = ExamplesConfig()
+        self.print_callback: Callable[[str], str] | None = None
 
     def set_config(
         self,
         *,
         line_length: int = DEFAULT_LINE_LENGTH,
         quotes: Literal['single', 'double', 'either'] = 'either',
         magic_trailing_comma: bool = True,
@@ -155,15 +156,17 @@
             enable_print_mock = True
         elif insert_print_statements == 'update':
             enable_print_mock = True
         else:
             enable_print_mock = False
 
         python_file = self._write_file(example)
-        return run_code(example, python_file, loader, self.config, enable_print_mock, module_globals)
+        return run_code(
+            example, python_file, loader, self.config, enable_print_mock, self.print_callback, module_globals
+        )
 
     def lint(self, example: CodeExample) -> None:
         """
         Lint the example with black and ruff.
 
         :param example: The example to lint.
         """
```

### Comparing `pytest_examples-0.0.8/pytest_examples/find_examples.py` & `pytest_examples-0.0.9/pytest_examples/find_examples.py`

 * *Files 2% similar despite different names*

```diff
@@ -112,15 +112,15 @@
         try:
             path = self.path.relative_to(Path.cwd())
         except ValueError:
             path = self.path
         return f'{path}:{self.start_line}-{self.end_line}'
 
 
-def find_examples(*paths: str, skip: bool = False) -> Iterable[CodeExample]:
+def find_examples(*paths: str | Path, skip: bool = False) -> Iterable[CodeExample]:
     """
     Find Python code examples in markdown files and python file docstrings.
 
     :param paths: Directories or files to search for examples in.
     :param skip: Whether to exit early and not search for examples, useful when running on windows where search fails.
     :return: A generator of `CodeExample` objects.
     """
@@ -136,15 +136,15 @@
         else:
             raise ValueError(f'Not a file or directory: {s!r}')
 
         for path in sub_paths:
             group = uuid4()
             if path.suffix == '.py':
                 code = path.read_text('utf-8')
-                for m_docstring in re.finditer(r'(^ *)(r?"""\n)(.+?)\1"""', code, flags=re.M | re.S):
+                for m_docstring in re.finditer(r'(^ *)(r?""".*?\n)(.+?)\1"""', code, flags=re.M | re.S):
                     start_line = code[: m_docstring.start()].count('\n') + 1
                     docstring = m_docstring.group(3)
                     index_offset = m_docstring.start() + len(m_docstring.group(1)) + len(m_docstring.group(2))
                     yield from _extract_code_chunks(
                         path, docstring, group, line_offset=start_line, index_offset=index_offset
                     )
             elif path.suffix == '.md':
```

### Comparing `pytest_examples-0.0.8/pytest_examples/lint.py` & `pytest_examples-0.0.9/pytest_examples/lint.py`

 * *Files identical despite different names*

### Comparing `pytest_examples-0.0.8/pytest_examples/modify_files.py` & `pytest_examples-0.0.9/pytest_examples/modify_files.py`

 * *Files identical despite different names*

### Comparing `pytest_examples-0.0.8/pytest_examples/run_code.py` & `pytest_examples-0.0.9/pytest_examples/run_code.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 import inspect
 import re
 import sys
 from dataclasses import dataclass
 from importlib.abc import Loader
 from pathlib import Path
 from textwrap import indent
-from typing import TYPE_CHECKING, Any
+from typing import TYPE_CHECKING, Any, Callable
 from unittest.mock import patch
 
 import pytest
 from black import InvalidInput
 
 from .lint import black_format, code_diff
 from .traceback import create_example_traceback
@@ -30,23 +30,24 @@
 
 def run_code(
     example: CodeExample,
     python_file: Path,
     loader: Loader | None,
     config: ExamplesConfig,
     enable_print_mock: bool,
+    print_callback: Callable[[str], str] | None,
     module_globals: dict[str, Any] | None,
 ) -> tuple[InsertPrintStatements, dict[str, Any]]:
     __tracebackhide__ = True
 
     spec = importlib.util.spec_from_file_location('__main__', str(python_file), loader=loader)
     module = importlib.util.module_from_spec(spec)
 
     # does nothing if insert_print_statements is False
-    insert_print = InsertPrintStatements(python_file, config, enable_print_mock)
+    insert_print = InsertPrintStatements(python_file, config, enable_print_mock, print_callback)
 
     if module_globals:
         module.__dict__.update(module_globals)
     try:
         with insert_print:
             spec.loader.exec_module(module)
     except KeyboardInterrupt:
@@ -119,18 +120,21 @@
         if self.file.samefile(frame.filename):
             # -1 to account for the line number being 1-indexed
             s = PrintStatement(frame.lineno, sep, [Arg(arg) for arg in args])
             self.statements.append(s)
 
 
 class InsertPrintStatements:
-    def __init__(self, python_path: Path, config: ExamplesConfig, enable: bool):
+    def __init__(
+        self, python_path: Path, config: ExamplesConfig, enable: bool, print_callback: Callable[[str], str] | None
+    ):
         self.file = python_path
         self.config = config
         self.print_func = MockPrintFunction(python_path) if enable else None
+        self.print_callback = print_callback
         self.patch = None
 
     def __enter__(self) -> None:
         if self.print_func:
             self.patch = patch('builtins.print', side_effect=self.print_func)
             self.patch.start()
 
@@ -172,23 +176,27 @@
 
         return '\n'.join(lines) + '\n'
 
     def _insert_print_args(
         self, lines: list[str], statement: PrintStatement, in_python: bool, line_index: int, col: int
     ) -> None:
         single_line = statement.sep.join(map(str, statement.args))
+        if self.print_callback:
+            single_line = self.print_callback(single_line)
         indent_str = ' ' * col
         max_single_length = self.config.line_length - len(indent_str)
         if '\n' not in single_line and len(single_line) + len(comment_prefix) < max_single_length:
             lines.insert(line_index + 1, f'{indent_str}{comment_prefix}{single_line}')
         else:
             # if the statement is too long to go on one line, print each arg on its own line formatted with black
             sep = f'{statement.sep}\n'
             indent_config = dataclasses.replace(self.config, line_length=max_single_length)
             output = sep.join(arg.format(indent_config).strip('\n') for arg in statement.args)
+            if self.print_callback:
+                output = self.print_callback(output)
             # remove trailing whitespace
             output = re.sub(r' +$', '', output, flags=re.MULTILINE)
             # have to use triple single quotes in python since we're already in a double quotes docstring
             quote = "'''" if in_python else '"""'
             lines.insert(line_index + 1, indent(f'{quote}\n{output}\n{quote}', indent_str))
```

### Comparing `pytest_examples-0.0.8/pytest_examples/traceback.py` & `pytest_examples-0.0.9/pytest_examples/traceback.py`

 * *Files identical despite different names*

### Comparing `pytest_examples-0.0.8/requirements/linting.txt` & `pytest_examples-0.0.9/requirements/linting.txt`

 * *Files identical despite different names*

### Comparing `pytest_examples-0.0.8/requirements/pyproject.txt` & `pytest_examples-0.0.9/requirements/pyproject.txt`

 * *Files identical despite different names*

### Comparing `pytest_examples-0.0.8/requirements/testing.txt` & `pytest_examples-0.0.9/requirements/testing.txt`

 * *Files identical despite different names*

### Comparing `pytest_examples-0.0.8/LICENSE` & `pytest_examples-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `pytest_examples-0.0.8/README.md` & `pytest_examples-0.0.9/README.md`

 * *Files identical despite different names*

### Comparing `pytest_examples-0.0.8/pyproject.toml` & `pytest_examples-0.0.9/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pytest_examples-0.0.8/PKG-INFO` & `pytest_examples-0.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytest-examples
-Version: 0.0.8
+Version: 0.0.9
 Summary: Pytest plugin for testing examples in docstrings and markdown files.
 Project-URL: repository, https://github.com/pydantic/pytest-examples
 Author-email: Samuel Colvin <s@muelcolvin.com>
 License-Expression: MIT
 License-File: LICENSE
 Classifier: Development Status :: 4 - Beta
 Classifier: Environment :: Console
```

