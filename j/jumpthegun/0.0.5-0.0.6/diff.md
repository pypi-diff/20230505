# Comparing `tmp/jumpthegun-0.0.5.tar.gz` & `tmp/jumpthegun-0.0.6.tar.gz`

## Comparing `jumpthegun-0.0.5.tar` & `jumpthegun-0.0.6.tar`

### file list

```diff
@@ -1,37 +1,37 @@
--rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 jumpthegun-0.0.5/.flake8
--rw-r--r--   0        0        0      469 2020-02-02 00:00:00.000000 jumpthegun-0.0.5/.pre-commit-config.yaml
--rw-r--r--   0        0        0       35 2020-02-02 00:00:00.000000 jumpthegun-0.0.5/test_requirements.txt
--rw-r--r--   0        0        0      454 2020-02-02 00:00:00.000000 jumpthegun-0.0.5/tox.ini
--rwxr-xr-x   0        0        0     5064 2020-02-02 00:00:00.000000 jumpthegun-0.0.5/src/jumpthegun.sh
--rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 jumpthegun-0.0.5/src/jumpthegun/__init__.py
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 jumpthegun-0.0.5/src/jumpthegun/__version__.py
--rw-r--r--   0        0        0    12726 2020-02-02 00:00:00.000000 jumpthegun-0.0.5/src/jumpthegun/jumpthegunctl.py
--rw-r--r--   0        0        0     3900 2020-02-02 00:00:00.000000 jumpthegun-0.0.5/src/jumpthegun/output_redirect.py
--rw-r--r--   0        0        0      475 2020-02-02 00:00:00.000000 jumpthegun-0.0.5/src/jumpthegun/testutils.py
--rw-r--r--   0        0        0     1891 2020-02-02 00:00:00.000000 jumpthegun-0.0.5/src/jumpthegun/tools.py
--rw-r--r--   0        0        0      547 2020-02-02 00:00:00.000000 jumpthegun-0.0.5/src/jumpthegun/utils.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jumpthegun-0.0.5/src/jumpthegun/_vendor/__init__.py
--rw-r--r--   0        0        0     1210 2020-02-02 00:00:00.000000 jumpthegun-0.0.5/src/jumpthegun/_vendor/filelock/LICENSE
--rw-r--r--   0        0        0      860 2020-02-02 00:00:00.000000 jumpthegun-0.0.5/src/jumpthegun/_vendor/filelock/README.md
--rw-r--r--   0        0        0        6 2020-02-02 00:00:00.000000 jumpthegun-0.0.5/src/jumpthegun/_vendor/filelock/VERSION
--rw-r--r--   0        0        0     1315 2020-02-02 00:00:00.000000 jumpthegun-0.0.5/src/jumpthegun/_vendor/filelock/__init__.py
--rw-r--r--   0        0        0     8896 2020-02-02 00:00:00.000000 jumpthegun-0.0.5/src/jumpthegun/_vendor/filelock/_api.py
--rw-r--r--   0        0        0      399 2020-02-02 00:00:00.000000 jumpthegun-0.0.5/src/jumpthegun/_vendor/filelock/_error.py
--rw-r--r--   0        0        0     1650 2020-02-02 00:00:00.000000 jumpthegun-0.0.5/src/jumpthegun/_vendor/filelock/_soft.py
--rw-r--r--   0        0        0     1578 2020-02-02 00:00:00.000000 jumpthegun-0.0.5/src/jumpthegun/_vendor/filelock/_unix.py
--rw-r--r--   0        0        0      594 2020-02-02 00:00:00.000000 jumpthegun-0.0.5/src/jumpthegun/_vendor/filelock/_util.py
--rw-r--r--   0        0        0     1890 2020-02-02 00:00:00.000000 jumpthegun-0.0.5/src/jumpthegun/_vendor/filelock/_windows.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jumpthegun-0.0.5/src/jumpthegun/_vendor/filelock/py.typed
--rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 jumpthegun-0.0.5/src/jumpthegun/_vendor/filelock/version.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jumpthegun-0.0.5/tests/__init__.py
--rw-r--r--   0        0        0     7516 2020-02-02 00:00:00.000000 jumpthegun-0.0.5/tests/test_jumpthegun.py
--rw-r--r--   0        0        0      436 2020-02-02 00:00:00.000000 jumpthegun-0.0.5/tests/test_tools.py
--rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 jumpthegun-0.0.5/tests/testproj/.flake8
--rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 jumpthegun-0.0.5/tests/testproj/bad.py
--rw-r--r--   0        0        0       94 2020-02-02 00:00:00.000000 jumpthegun-0.0.5/tests/testproj/good.py
--rw-r--r--   0        0        0      280 2020-02-02 00:00:00.000000 jumpthegun-0.0.5/tests/testproj/pyproject.toml
--rw-r--r--   0        0        0     1860 2020-02-02 00:00:00.000000 jumpthegun-0.0.5/.gitignore
--rw-r--r--   0        0        0    11357 2020-02-02 00:00:00.000000 jumpthegun-0.0.5/LICENSE
--rw-r--r--   0        0        0     2296 2020-02-02 00:00:00.000000 jumpthegun-0.0.5/README.md
--rw-r--r--   0        0        0     1984 2020-02-02 00:00:00.000000 jumpthegun-0.0.5/pyproject.toml
--rw-r--r--   0        0        0     3456 2020-02-02 00:00:00.000000 jumpthegun-0.0.5/PKG-INFO
+-rw-r--r--   0        0        0      125 2020-02-02 00:00:00.000000 jumpthegun-0.0.6/.flake8
+-rw-r--r--   0        0        0      469 2020-02-02 00:00:00.000000 jumpthegun-0.0.6/.pre-commit-config.yaml
+-rw-r--r--   0        0        0       35 2020-02-02 00:00:00.000000 jumpthegun-0.0.6/test_requirements.txt
+-rw-r--r--   0        0        0      561 2020-02-02 00:00:00.000000 jumpthegun-0.0.6/tox.ini
+-rwxr-xr-x   0        0        0     5064 2020-02-02 00:00:00.000000 jumpthegun-0.0.6/src/jumpthegun.sh
+-rw-r--r--   0        0        0       51 2020-02-02 00:00:00.000000 jumpthegun-0.0.6/src/jumpthegun/__init__.py
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 jumpthegun-0.0.6/src/jumpthegun/__version__.py
+-rw-r--r--   0        0        0    12726 2020-02-02 00:00:00.000000 jumpthegun-0.0.6/src/jumpthegun/jumpthegunctl.py
+-rw-r--r--   0        0        0     3900 2020-02-02 00:00:00.000000 jumpthegun-0.0.6/src/jumpthegun/output_redirect.py
+-rw-r--r--   0        0        0      475 2020-02-02 00:00:00.000000 jumpthegun-0.0.6/src/jumpthegun/testutils.py
+-rw-r--r--   0        0        0     2081 2020-02-02 00:00:00.000000 jumpthegun-0.0.6/src/jumpthegun/tools.py
+-rw-r--r--   0        0        0      547 2020-02-02 00:00:00.000000 jumpthegun-0.0.6/src/jumpthegun/utils.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jumpthegun-0.0.6/src/jumpthegun/_vendor/__init__.py
+-rw-r--r--   0        0        0     1210 2020-02-02 00:00:00.000000 jumpthegun-0.0.6/src/jumpthegun/_vendor/filelock/LICENSE
+-rw-r--r--   0        0        0      860 2020-02-02 00:00:00.000000 jumpthegun-0.0.6/src/jumpthegun/_vendor/filelock/README.md
+-rw-r--r--   0        0        0        6 2020-02-02 00:00:00.000000 jumpthegun-0.0.6/src/jumpthegun/_vendor/filelock/VERSION
+-rw-r--r--   0        0        0     1315 2020-02-02 00:00:00.000000 jumpthegun-0.0.6/src/jumpthegun/_vendor/filelock/__init__.py
+-rw-r--r--   0        0        0     8896 2020-02-02 00:00:00.000000 jumpthegun-0.0.6/src/jumpthegun/_vendor/filelock/_api.py
+-rw-r--r--   0        0        0      399 2020-02-02 00:00:00.000000 jumpthegun-0.0.6/src/jumpthegun/_vendor/filelock/_error.py
+-rw-r--r--   0        0        0     1650 2020-02-02 00:00:00.000000 jumpthegun-0.0.6/src/jumpthegun/_vendor/filelock/_soft.py
+-rw-r--r--   0        0        0     1578 2020-02-02 00:00:00.000000 jumpthegun-0.0.6/src/jumpthegun/_vendor/filelock/_unix.py
+-rw-r--r--   0        0        0      594 2020-02-02 00:00:00.000000 jumpthegun-0.0.6/src/jumpthegun/_vendor/filelock/_util.py
+-rw-r--r--   0        0        0     1890 2020-02-02 00:00:00.000000 jumpthegun-0.0.6/src/jumpthegun/_vendor/filelock/_windows.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jumpthegun-0.0.6/src/jumpthegun/_vendor/filelock/py.typed
+-rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 jumpthegun-0.0.6/src/jumpthegun/_vendor/filelock/version.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 jumpthegun-0.0.6/tests/__init__.py
+-rw-r--r--   0        0        0     7516 2020-02-02 00:00:00.000000 jumpthegun-0.0.6/tests/test_jumpthegun.py
+-rw-r--r--   0        0        0      436 2020-02-02 00:00:00.000000 jumpthegun-0.0.6/tests/test_tools.py
+-rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 jumpthegun-0.0.6/tests/testproj/.flake8
+-rw-r--r--   0        0        0       59 2020-02-02 00:00:00.000000 jumpthegun-0.0.6/tests/testproj/bad.py
+-rw-r--r--   0        0        0       94 2020-02-02 00:00:00.000000 jumpthegun-0.0.6/tests/testproj/good.py
+-rw-r--r--   0        0        0      280 2020-02-02 00:00:00.000000 jumpthegun-0.0.6/tests/testproj/pyproject.toml
+-rw-r--r--   0        0        0     1860 2020-02-02 00:00:00.000000 jumpthegun-0.0.6/.gitignore
+-rw-r--r--   0        0        0     1081 2020-02-02 00:00:00.000000 jumpthegun-0.0.6/LICENSE
+-rw-r--r--   0        0        0     4789 2020-02-02 00:00:00.000000 jumpthegun-0.0.6/README.md
+-rw-r--r--   0        0        0     1984 2020-02-02 00:00:00.000000 jumpthegun-0.0.6/pyproject.toml
+-rw-r--r--   0        0        0     5949 2020-02-02 00:00:00.000000 jumpthegun-0.0.6/PKG-INFO
```

### Comparing `jumpthegun-0.0.5/src/jumpthegun.sh` & `jumpthegun-0.0.6/src/jumpthegun.sh`

 * *Files identical despite different names*

### Comparing `jumpthegun-0.0.5/src/jumpthegun/jumpthegunctl.py` & `jumpthegun-0.0.6/src/jumpthegun/jumpthegunctl.py`

 * *Files identical despite different names*

### Comparing `jumpthegun-0.0.5/src/jumpthegun/output_redirect.py` & `jumpthegun-0.0.6/src/jumpthegun/output_redirect.py`

 * *Files identical despite different names*

### Comparing `jumpthegun-0.0.5/src/jumpthegun/tools.py` & `jumpthegun-0.0.6/src/jumpthegun/tools.py`

 * *Files 6% similar despite different names*

```diff
@@ -14,14 +14,20 @@
 ]
 
 
 testing_tools: Dict[str, str] = {
     "__test_sleep_and_exit_on_signal": "jumpthegun.testutils:sleep_and_exit_on_signal",
 }
 
+well_known_tools: Dict[str, str] = {
+    "aws": "awscli.clidriver:main",
+}
+
+all_known_tools = {**well_known_tools, **testing_tools}
+
 
 class ToolExceptionBase(Exception):
     """Exception raised for CLI tool-related exceptions."""
 
     tool_name: str
 
     def __init__(self, tool_name) -> None:
@@ -41,18 +47,19 @@
 
     def __str__(self) -> str:
         return f"Multiple console entrypoints: {self.tool_name}"
 
 
 def get_tool_entrypoint(tool_name: str) -> EntryPoint:
     """Get an entrypoint function for a CLI tool."""
-    if tool_name in testing_tools:
+    tool_entrypoint_str = all_known_tools.get(tool_name)
+    if tool_entrypoint_str is not None:
         entrypoint = EntryPoint(
             name=tool_name,
-            value=testing_tools[tool_name],
+            value=tool_entrypoint_str,
             group="console_scripts",
         )
         return entrypoint
 
     all_entrypoints = entry_points()
     if hasattr(all_entrypoints, "select"):
         entrypoints = all_entrypoints.select(name=tool_name, group="console_scripts")
```

### Comparing `jumpthegun-0.0.5/src/jumpthegun/utils.py` & `jumpthegun-0.0.6/src/jumpthegun/utils.py`

 * *Files identical despite different names*

### Comparing `jumpthegun-0.0.5/src/jumpthegun/_vendor/filelock/LICENSE` & `jumpthegun-0.0.6/src/jumpthegun/_vendor/filelock/LICENSE`

 * *Files identical despite different names*

### Comparing `jumpthegun-0.0.5/src/jumpthegun/_vendor/filelock/README.md` & `jumpthegun-0.0.6/src/jumpthegun/_vendor/filelock/README.md`

 * *Files identical despite different names*

### Comparing `jumpthegun-0.0.5/src/jumpthegun/_vendor/filelock/__init__.py` & `jumpthegun-0.0.6/src/jumpthegun/_vendor/filelock/__init__.py`

 * *Files identical despite different names*

### Comparing `jumpthegun-0.0.5/src/jumpthegun/_vendor/filelock/_api.py` & `jumpthegun-0.0.6/src/jumpthegun/_vendor/filelock/_api.py`

 * *Files identical despite different names*

### Comparing `jumpthegun-0.0.5/src/jumpthegun/_vendor/filelock/_soft.py` & `jumpthegun-0.0.6/src/jumpthegun/_vendor/filelock/_soft.py`

 * *Files identical despite different names*

### Comparing `jumpthegun-0.0.5/src/jumpthegun/_vendor/filelock/_unix.py` & `jumpthegun-0.0.6/src/jumpthegun/_vendor/filelock/_unix.py`

 * *Files identical despite different names*

### Comparing `jumpthegun-0.0.5/src/jumpthegun/_vendor/filelock/_util.py` & `jumpthegun-0.0.6/src/jumpthegun/_vendor/filelock/_util.py`

 * *Files identical despite different names*

### Comparing `jumpthegun-0.0.5/src/jumpthegun/_vendor/filelock/_windows.py` & `jumpthegun-0.0.6/src/jumpthegun/_vendor/filelock/_windows.py`

 * *Files identical despite different names*

### Comparing `jumpthegun-0.0.5/tests/test_jumpthegun.py` & `jumpthegun-0.0.6/tests/test_jumpthegun.py`

 * *Files 1% similar despite different names*

```diff
@@ -171,15 +171,15 @@
             ["jumpthegun", "run", "--no-autorun", *subcmd],
             proj_path=testproj,
             background=True,
         )
         assert proc.stdout.readline() == b"Sleeping...\n"
         assert proc.poll() is None
         proc.send_signal(signum)
-        proc.wait(2)
+        proc.wait(5)
         assert b"Received signal" in proc.stdout.read()
     finally:
         run(["jumpthegun", "stop", subcmd[0]], proj_path=testproj, check=True)
 
 
 def run(
     cmd: List[str], proj_path: Path, background: bool = False, check: bool = False
```

### Comparing `jumpthegun-0.0.5/.gitignore` & `jumpthegun-0.0.6/.gitignore`

 * *Files identical despite different names*

### Comparing `jumpthegun-0.0.5/pyproject.toml` & `jumpthegun-0.0.6/pyproject.toml`

 * *Files identical despite different names*

