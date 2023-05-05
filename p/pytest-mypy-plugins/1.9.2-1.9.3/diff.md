# Comparing `tmp/pytest-mypy-plugins-1.9.2.tar.gz` & `tmp/pytest-mypy-plugins-1.9.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pytest-mypy-plugins-1.9.2.tar", last modified: Tue Oct 19 10:00:56 2021, max compression
+gzip compressed data, was "pytest-mypy-plugins-1.9.3.tar", last modified: Tue Jan 11 12:44:07 2022, max compression
```

## Comparing `pytest-mypy-plugins-1.9.2.tar` & `pytest-mypy-plugins-1.9.3.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 sobolev    (501) staff       (20)        0 2021-10-19 10:00:56.554225 pytest-mypy-plugins-1.9.2/
--rw-r--r--   0 sobolev    (501) staff       (20)     1054 2020-04-08 22:59:41.000000 pytest-mypy-plugins-1.9.2/LICENSE
--rw-r--r--   0 sobolev    (501) staff       (20)     8228 2021-10-19 10:00:56.554468 pytest-mypy-plugins-1.9.2/PKG-INFO
--rw-r--r--   0 sobolev    (501) staff       (20)     7489 2021-10-19 09:32:51.000000 pytest-mypy-plugins-1.9.2/README.md
--rw-r--r--   0 sobolev    (501) staff       (20)       31 2020-04-16 22:12:59.000000 pytest-mypy-plugins-1.9.2/pyproject.toml
-drwxr-xr-x   0 sobolev    (501) staff       (20)        0 2021-10-19 10:00:56.525892 pytest-mypy-plugins-1.9.2/pytest_mypy_plugins/
--rw-r--r--   0 sobolev    (501) staff       (20)        0 2020-04-08 22:59:41.000000 pytest-mypy-plugins-1.9.2/pytest_mypy_plugins/__init__.py
--rw-r--r--   0 sobolev    (501) staff       (20)     6601 2021-10-19 09:40:34.000000 pytest-mypy-plugins-1.9.2/pytest_mypy_plugins/collect.py
--rw-r--r--   0 sobolev    (501) staff       (20)    15163 2021-10-19 09:40:34.000000 pytest-mypy-plugins-1.9.2/pytest_mypy_plugins/item.py
--rw-r--r--   0 sobolev    (501) staff       (20)        0 2021-10-19 09:32:51.000000 pytest-mypy-plugins-1.9.2/pytest_mypy_plugins/py.typed
--rw-r--r--   0 sobolev    (501) staff       (20)    12431 2021-10-19 09:40:34.000000 pytest-mypy-plugins-1.9.2/pytest_mypy_plugins/utils.py
-drwxr-xr-x   0 sobolev    (501) staff       (20)        0 2021-10-19 10:00:56.544037 pytest-mypy-plugins-1.9.2/pytest_mypy_plugins.egg-info/
--rw-r--r--   0 sobolev    (501) staff       (20)     8228 2021-10-19 10:00:56.000000 pytest-mypy-plugins-1.9.2/pytest_mypy_plugins.egg-info/PKG-INFO
--rw-r--r--   0 sobolev    (501) staff       (20)      460 2021-10-19 10:00:56.000000 pytest-mypy-plugins-1.9.2/pytest_mypy_plugins.egg-info/SOURCES.txt
--rw-r--r--   0 sobolev    (501) staff       (20)        1 2021-10-19 10:00:56.000000 pytest-mypy-plugins-1.9.2/pytest_mypy_plugins.egg-info/dependency_links.txt
--rw-r--r--   0 sobolev    (501) staff       (20)       62 2021-10-19 10:00:56.000000 pytest-mypy-plugins-1.9.2/pytest_mypy_plugins.egg-info/entry_points.txt
--rw-r--r--   0 sobolev    (501) staff       (20)       96 2021-10-19 10:00:56.000000 pytest-mypy-plugins-1.9.2/pytest_mypy_plugins.egg-info/requires.txt
--rw-r--r--   0 sobolev    (501) staff       (20)       20 2021-10-19 10:00:56.000000 pytest-mypy-plugins-1.9.2/pytest_mypy_plugins.egg-info/top_level.txt
--rw-r--r--   0 sobolev    (501) staff       (20)       99 2021-10-19 10:00:56.556536 pytest-mypy-plugins-1.9.2/setup.cfg
--rw-r--r--   0 sobolev    (501) staff       (20)     1319 2021-10-19 09:46:14.000000 pytest-mypy-plugins-1.9.2/setup.py
+drwxr-xr-x   0 sobolev    (501) staff       (20)        0 2022-01-11 12:44:07.602709 pytest-mypy-plugins-1.9.3/
+-rw-r--r--   0 sobolev    (501) staff       (20)     1054 2020-04-08 22:59:41.000000 pytest-mypy-plugins-1.9.3/LICENSE
+-rw-r--r--   0 sobolev    (501) staff       (20)     8228 2022-01-11 12:44:07.602046 pytest-mypy-plugins-1.9.3/PKG-INFO
+-rw-r--r--   0 sobolev    (501) staff       (20)     7489 2021-10-19 09:32:51.000000 pytest-mypy-plugins-1.9.3/README.md
+-rw-r--r--   0 sobolev    (501) staff       (20)      115 2021-12-25 08:11:40.000000 pytest-mypy-plugins-1.9.3/pyproject.toml
+drwxr-xr-x   0 sobolev    (501) staff       (20)        0 2022-01-11 12:44:07.595543 pytest-mypy-plugins-1.9.3/pytest_mypy_plugins/
+-rw-r--r--   0 sobolev    (501) staff       (20)        0 2020-04-08 22:59:41.000000 pytest-mypy-plugins-1.9.3/pytest_mypy_plugins/__init__.py
+-rw-r--r--   0 sobolev    (501) staff       (20)     7182 2021-12-25 08:11:40.000000 pytest-mypy-plugins-1.9.3/pytest_mypy_plugins/collect.py
+-rw-r--r--   0 sobolev    (501) staff       (20)    14746 2022-01-11 12:36:28.000000 pytest-mypy-plugins-1.9.3/pytest_mypy_plugins/item.py
+-rw-r--r--   0 sobolev    (501) staff       (20)        0 2021-10-19 09:32:51.000000 pytest-mypy-plugins-1.9.3/pytest_mypy_plugins/py.typed
+-rw-r--r--   0 sobolev    (501) staff       (20)    12431 2021-10-19 09:40:34.000000 pytest-mypy-plugins-1.9.3/pytest_mypy_plugins/utils.py
+drwxr-xr-x   0 sobolev    (501) staff       (20)        0 2022-01-11 12:44:07.601156 pytest-mypy-plugins-1.9.3/pytest_mypy_plugins.egg-info/
+-rw-r--r--   0 sobolev    (501) staff       (20)     8228 2022-01-11 12:44:07.000000 pytest-mypy-plugins-1.9.3/pytest_mypy_plugins.egg-info/PKG-INFO
+-rw-r--r--   0 sobolev    (501) staff       (20)      450 2022-01-11 12:44:07.000000 pytest-mypy-plugins-1.9.3/pytest_mypy_plugins.egg-info/SOURCES.txt
+-rw-r--r--   0 sobolev    (501) staff       (20)        1 2022-01-11 12:44:07.000000 pytest-mypy-plugins-1.9.3/pytest_mypy_plugins.egg-info/dependency_links.txt
+-rw-r--r--   0 sobolev    (501) staff       (20)       62 2022-01-11 12:44:07.000000 pytest-mypy-plugins-1.9.3/pytest_mypy_plugins.egg-info/entry_points.txt
+-rw-r--r--   0 sobolev    (501) staff       (20)       96 2022-01-11 12:44:07.000000 pytest-mypy-plugins-1.9.3/pytest_mypy_plugins.egg-info/requires.txt
+-rw-r--r--   0 sobolev    (501) staff       (20)       20 2022-01-11 12:44:07.000000 pytest-mypy-plugins-1.9.3/pytest_mypy_plugins.egg-info/top_level.txt
+-rw-r--r--   0 sobolev    (501) staff       (20)       38 2022-01-11 12:44:07.602907 pytest-mypy-plugins-1.9.3/setup.cfg
+-rw-r--r--   0 sobolev    (501) staff       (20)     1319 2022-01-11 12:37:14.000000 pytest-mypy-plugins-1.9.3/setup.py
```

### Comparing `pytest-mypy-plugins-1.9.2/LICENSE` & `pytest-mypy-plugins-1.9.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pytest-mypy-plugins-1.9.2/PKG-INFO` & `pytest-mypy-plugins-1.9.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytest-mypy-plugins
-Version: 1.9.2
+Version: 1.9.3
 Summary: pytest plugin for writing tests for mypy plugins
 Home-page: https://github.com/TypedDjango/pytest-mypy-plugins
 Author: Maksim Kurnikov
 Author-email: maxim.kurnikov@gmail.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `pytest-mypy-plugins-1.9.2/README.md` & `pytest-mypy-plugins-1.9.3/README.md`

 * *Files identical despite different names*

### Comparing `pytest-mypy-plugins-1.9.2/pytest_mypy_plugins/collect.py` & `pytest-mypy-plugins-1.9.3/pytest_mypy_plugins/collect.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 import os
+import pathlib
 import platform
 import sys
 import tempfile
 from typing import TYPE_CHECKING, Any, Dict, Iterator, List, Mapping, Optional, Set
 
+import pkg_resources
 import pytest
 import yaml
 from _pytest.config.argparsing import Parser
 from _pytest.nodes import Node
 from py._path.local import LocalPath
 
 from pytest_mypy_plugins import utils
@@ -72,15 +74,17 @@
         return mapping
 
 
 class YamlTestFile(pytest.File):
     def collect(self) -> Iterator["YamlTestItem"]:
         from pytest_mypy_plugins.item import YamlTestItem
 
-        parsed_file = yaml.load(stream=self.fspath.read_text("utf8"), Loader=SafeLineLoader)
+        # To support both Pytest 6.x and 7.x
+        path = getattr(self, "path", None) or getattr(self, "fspath")
+        parsed_file = yaml.load(stream=path.read_text("utf8"), Loader=SafeLineLoader)
         if parsed_file is None:
             return
 
         if not isinstance(parsed_file, list):
             raise ValueError(f"Test file has to be YAML list, got {type(parsed_file)!r}.")
 
         for raw_test in parsed_file:
@@ -134,18 +138,27 @@
                         expect_fail=expect_fail,
                     )
 
     def _eval_skip(self, skip_if: str) -> bool:
         return eval(skip_if, {"sys": sys, "os": os, "pytest": pytest, "platform": platform})
 
 
-def pytest_collect_file(path: LocalPath, parent: Node) -> Optional[YamlTestFile]:
-    if path.ext in {".yaml", ".yml"} and path.basename.startswith(("test-", "test_")):
-        return YamlTestFile.from_parent(parent, fspath=path)
-    return None
+if pkg_resources.parse_version(pytest.__version__) >= pkg_resources.parse_version("7.0.0rc1"):
+
+    def pytest_collect_file(file_path: pathlib.Path, parent: Node) -> Optional[YamlTestFile]:
+        if file_path.suffix in {".yaml", ".yml"} and file_path.name.startswith(("test-", "test_")):
+            return YamlTestFile.from_parent(parent, path=file_path, fspath=None)
+        return None
+
+else:
+
+    def pytest_collect_file(path: LocalPath, parent: Node) -> Optional[YamlTestFile]:  # type: ignore[misc]
+        if path.ext in {".yaml", ".yml"} and path.basename.startswith(("test-", "test_")):
+            return YamlTestFile.from_parent(parent, fspath=path)
+        return None
 
 
 def pytest_addoption(parser: Parser) -> None:
     group = parser.getgroup("mypy-tests")
     group.addoption(
         "--mypy-testing-base", type=str, default=tempfile.gettempdir(), help="Base directory for tests to use"
     )
```

### Comparing `pytest-mypy-plugins-1.9.2/pytest_mypy_plugins/item.py` & `pytest-mypy-plugins-1.9.3/pytest_mypy_plugins/item.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,25 @@
 import importlib
 import os
 import subprocess
 import sys
 import tempfile
 from configparser import ConfigParser
 from pathlib import Path
-from typing import TYPE_CHECKING, Any, Callable, Dict, List, Optional, Tuple, Union
+from typing import (
+    TYPE_CHECKING,
+    Any,
+    Callable,
+    Dict,
+    List,
+    Optional,
+    Tuple,
+    Union,
+    no_type_check,
+)
 
 import py
 import pytest
 from _pytest._code import ExceptionInfo
 from _pytest._code.code import ReprEntry, ReprFileLocation, TerminalRepr
 from _pytest._io import TerminalWriter
 from _pytest.config import Config
@@ -170,24 +180,14 @@
             if (
                 parent_dir.exists()
                 and len(list(parent_dir.iterdir())) == 0
                 and str(self.incremental_cache_dir) in str(parent_dir)
             ):
                 parent_dir.rmdir()
 
-    def find_dependent_paths(self, path: Path) -> List[Path]:
-        py_module = ".".join(path.with_suffix("").parts)
-        dependants = []
-        for dirpath, _, filenames in os.walk(self.incremental_cache_dir):
-            for filename in filenames:
-                path = Path(dirpath) / filename
-                if f'"{py_module}"' in path.read_text():
-                    dependants.append(path.with_suffix("").with_suffix(""))
-        return dependants
-
     def typecheck_in_new_subprocess(
         self, execution_path: Path, mypy_cmd_options: List[Any]
     ) -> Tuple[int, Tuple[str, str]]:
         import shutil
 
         mypy_executable = shutil.which("mypy")
         assert mypy_executable is not None, "mypy executable is not found"
@@ -236,16 +236,22 @@
         extension_hook = getattr(module, func_name)
         extension_hook(self)
 
     def runtest(self) -> None:
         try:
             temp_dir = tempfile.TemporaryDirectory(prefix="pytest-mypy-", dir=self.root_directory)
 
+        except (FileNotFoundError, PermissionError, NotADirectoryError) as e:
+
+            raise TypecheckAssertionError(
+                error_message=f"Testing base directory {self.root_directory} must exist and be writable"
+            ) from e
+
+        try:
             execution_path = Path(temp_dir.name)
-            assert execution_path.exists()
 
             with utils.cd(execution_path):
                 # extension point for derived packages
                 if (
                     hasattr(self.config.option, "mypy_extension_hook")
                     and self.config.option.mypy_extension_hook is not None
                 ):
@@ -280,41 +286,34 @@
                         raise e
                 else:
                     if self.expect_fail:
                         raise TypecheckAssertionError("Expected failure, but test passed")
 
         finally:
             temp_dir.cleanup()
-            # remove created modules and all their dependants from cache
+            # remove created modules
             if not self.disable_cache:
                 for file in self.files:
                     path = Path(file.path)
                     self.remove_cache_files(path.with_suffix(""))
 
-                    dependants = self.find_dependent_paths(path)
-                    for dependant in dependants:
-                        self.remove_cache_files(dependant)
-
         assert not os.path.exists(temp_dir.name)
 
     def prepare_mypy_cmd_options(self, execution_path: Path) -> List[str]:
         mypy_cmd_options = [
             "--show-traceback",
             "--no-error-summary",
             "--no-pretty",
             "--hide-error-context",
         ]
         if not self.test_only_local_stub:
             mypy_cmd_options.append("--no-silence-site-packages")
         if not self.disable_cache:
             mypy_cmd_options.extend(["--cache-dir", self.incremental_cache_dir])
 
-        python_version = ".".join([str(part) for part in sys.version_info[:2]])
-        mypy_cmd_options.append(f"--python-version={python_version}")
-
         # Merge `self.base_ini_fpath` and `self.additional_mypy_config`
         # into one file and copy to the typechecking folder:
         mypy_ini_config = ConfigParser()
         if self.base_ini_fpath:
             mypy_ini_config.read(self.base_ini_fpath)
         if self.additional_mypy_config:
             additional_config = self.additional_mypy_config
@@ -350,16 +349,19 @@
                 exception_repr.reprtraceback.reprentries[-1].lines[1:], None, None, repr_file_location, "short"
             )
             exception_repr.reprtraceback.reprentries = [repr_tb_entry]
             return exception_repr
         else:
             return super().repr_failure(excinfo, style="native")
 
-    def reportinfo(self) -> Tuple[Union[py.path.local, str], Optional[int], str]:
-        return self.fspath, None, self.name
+    @no_type_check
+    def reportinfo(self) -> Tuple[Union[py.path.local, Path, str], Optional[int], str]:
+        # To support both Pytest 6.x and 7.x
+        path = getattr(self, "path", None) or getattr(self, "fspath")
+        return path, None, self.name
 
     def _collect_python_path(
         self,
         rootdir: Optional[Path],
         execution_path: Path,
     ) -> None:
         python_path_parts = []
```

### Comparing `pytest-mypy-plugins-1.9.2/pytest_mypy_plugins/utils.py` & `pytest-mypy-plugins-1.9.3/pytest_mypy_plugins/utils.py`

 * *Files identical despite different names*

### Comparing `pytest-mypy-plugins-1.9.2/pytest_mypy_plugins.egg-info/PKG-INFO` & `pytest-mypy-plugins-1.9.3/pytest_mypy_plugins.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pytest-mypy-plugins
-Version: 1.9.2
+Version: 1.9.3
 Summary: pytest plugin for writing tests for mypy plugins
 Home-page: https://github.com/TypedDjango/pytest-mypy-plugins
 Author: Maksim Kurnikov
 Author-email: maxim.kurnikov@gmail.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `pytest-mypy-plugins-1.9.2/setup.py` & `pytest-mypy-plugins-1.9.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -11,15 +11,15 @@
     "chevron",
     "regex",
     "dataclasses ; python_version<'3.7'",
 ]
 
 setup(
     name="pytest-mypy-plugins",
-    version="1.9.2",
+    version="1.9.3",
     description="pytest plugin for writing tests for mypy plugins",
     long_description=readme,
     long_description_content_type="text/markdown",
     license="MIT",
     url="https://github.com/TypedDjango/pytest-mypy-plugins",
     author="Maksim Kurnikov",
     author_email="maxim.kurnikov@gmail.com",
```

