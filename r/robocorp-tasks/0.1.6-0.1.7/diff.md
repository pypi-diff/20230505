# Comparing `tmp/robocorp_tasks-0.1.6.tar.gz` & `tmp/robocorp_tasks-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "robocorp_tasks-0.1.6.tar", max compression
+gzip compressed data, was "robocorp_tasks-0.1.7.tar", max compression
```

## Comparing `robocorp_tasks-0.1.6.tar` & `robocorp_tasks-0.1.7.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0     4799 2023-04-27 17:49:20.287384 robocorp_tasks-0.1.6/README.md
--rw-r--r--   0        0        0     1214 2023-04-27 17:49:20.287384 robocorp_tasks-0.1.6/pyproject.toml
--rw-r--r--   0        0        0      721 2023-04-27 17:49:20.291384 robocorp_tasks-0.1.6/src/robocorp/tasks/__init__.py
--rw-r--r--   0        0        0       79 2023-04-27 17:49:20.291384 robocorp_tasks-0.1.6/src/robocorp/tasks/__main__.py
--rw-r--r--   0        0        0     3371 2023-04-27 17:49:20.291384 robocorp_tasks-0.1.6/src/robocorp/tasks/_argdispatch.py
--rw-r--r--   0        0        0     1230 2023-04-27 17:49:20.291384 robocorp_tasks-0.1.6/src/robocorp/tasks/_callback.py
--rw-r--r--   0        0        0     5048 2023-04-27 17:49:20.291384 robocorp_tasks-0.1.6/src/robocorp/tasks/_collect_tasks.py
--rw-r--r--   0        0        0     5284 2023-04-27 17:49:20.291384 robocorp_tasks-0.1.6/src/robocorp/tasks/_commands.py
--rw-r--r--   0        0        0      638 2023-04-27 17:49:20.291384 robocorp_tasks-0.1.6/src/robocorp/tasks/_decorators.py
--rw-r--r--   0        0        0      182 2023-04-27 17:49:20.291384 robocorp_tasks-0.1.6/src/robocorp/tasks/_exceptions.py
--rw-r--r--   0        0        0      599 2023-04-27 17:49:20.291384 robocorp_tasks-0.1.6/src/robocorp/tasks/_hooks.py
--rw-r--r--   0        0        0     4940 2023-04-27 17:49:20.291384 robocorp_tasks-0.1.6/src/robocorp/tasks/_log_auto_setup.py
--rw-r--r--   0        0        0     2335 2023-04-27 17:49:20.291384 robocorp_tasks-0.1.6/src/robocorp/tasks/_log_output_setup.py
--rw-r--r--   0        0        0     1699 2023-04-27 17:49:20.291384 robocorp_tasks-0.1.6/src/robocorp/tasks/_protocols.py
--rw-r--r--   0        0        0      933 2023-04-27 17:49:20.291384 robocorp_tasks-0.1.6/src/robocorp/tasks/_task.py
--rw-r--r--   0        0        0      809 2023-04-27 17:49:20.291384 robocorp_tasks-0.1.6/src/robocorp/tasks/cli.py
--rw-r--r--   0        0        0     5544 1970-01-01 00:00:00.000000 robocorp_tasks-0.1.6/PKG-INFO
+-rw-r--r--   0        0        0     4922 2023-05-05 11:49:59.127328 robocorp_tasks-0.1.7/README.md
+-rw-r--r--   0        0        0     1266 2023-05-05 11:49:59.127328 robocorp_tasks-0.1.7/pyproject.toml
+-rw-r--r--   0        0        0      721 2023-05-05 11:49:59.127328 robocorp_tasks-0.1.7/src/robocorp/tasks/__init__.py
+-rw-r--r--   0        0        0       79 2023-05-05 11:49:59.127328 robocorp_tasks-0.1.7/src/robocorp/tasks/__main__.py
+-rw-r--r--   0        0        0     4237 2023-05-05 11:49:59.127328 robocorp_tasks-0.1.7/src/robocorp/tasks/_argdispatch.py
+-rw-r--r--   0        0        0     1230 2023-05-05 11:49:59.127328 robocorp_tasks-0.1.7/src/robocorp/tasks/_callback.py
+-rw-r--r--   0        0        0     5048 2023-05-05 11:49:59.127328 robocorp_tasks-0.1.7/src/robocorp/tasks/_collect_tasks.py
+-rw-r--r--   0        0        0     5908 2023-05-05 11:49:59.127328 robocorp_tasks-0.1.7/src/robocorp/tasks/_commands.py
+-rw-r--r--   0        0        0      638 2023-05-05 11:49:59.127328 robocorp_tasks-0.1.7/src/robocorp/tasks/_decorators.py
+-rw-r--r--   0        0        0      182 2023-05-05 11:49:59.127328 robocorp_tasks-0.1.7/src/robocorp/tasks/_exceptions.py
+-rw-r--r--   0        0        0      599 2023-05-05 11:49:59.127328 robocorp_tasks-0.1.7/src/robocorp/tasks/_hooks.py
+-rw-r--r--   0        0        0     4985 2023-05-05 11:49:59.127328 robocorp_tasks-0.1.7/src/robocorp/tasks/_log_auto_setup.py
+-rw-r--r--   0        0        0      461 2023-05-05 11:49:59.127328 robocorp_tasks-0.1.7/src/robocorp/tasks/_log_output_setup.py
+-rw-r--r--   0        0        0     1790 2023-05-05 11:49:59.127328 robocorp_tasks-0.1.7/src/robocorp/tasks/_protocols.py
+-rw-r--r--   0        0        0     5053 2023-05-05 11:49:59.127328 robocorp_tasks-0.1.7/src/robocorp/tasks/_task.py
+-rw-r--r--   0        0        0      809 2023-05-05 11:49:59.131328 robocorp_tasks-0.1.7/src/robocorp/tasks/cli.py
+-rw-r--r--   0        0        0     5667 1970-01-01 00:00:00.000000 robocorp_tasks-0.1.7/PKG-INFO
```

### Comparing `robocorp_tasks-0.1.6/README.md` & `robocorp_tasks-0.1.7/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,25 +1,26 @@
 # robocorp-tasks
 
-`robocorp-tasks` is a Python framework to simplify RPA development in Python.
+`robocorp-tasks` is a Python framework designed to simplify the development 
+of Python automations.
 
 > Note: The current version is still alpha but its public API is already meant
 > to be stable and new releases should keep backward compatibility.
 
 ## Why
 
-While Python is widely used in the RPA world, many solutions end up being ad-hoc, 
-making it difficult to navigate different projects or achieve comprehensible 
-logging out of the box.
+While Python is widely used in the automation world, many solutions end up being 
+ad-hoc, making it difficult to navigate different projects and keep up with the
+features required for analysing the results of such automations afterwards.
 
 ## How
 
-`robocorp-tasks` provides a runner for RPA tasks that offers logging 
-out of the box by leveraging `robocorp-log`, as well as the necessary 
-lifecycle management for running such tasks.
+`robocorp-tasks` provides a runner for running tasks that offers logging 
+out of the box for Python code (showing method calls, arguments, assigns, etc)
+by leveraging `robocorp-log`, and managing the lifecycle for running such tasks.
  
 ### Installation
 
 To install `robocorp-tasks`, use the following command:
 
 `pip install robocorp-tasks`
```

### Comparing `robocorp_tasks-0.1.6/pyproject.toml` & `robocorp_tasks-0.1.7/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "robocorp-tasks"
-version = "0.1.6"
+version = "0.1.7"
 description = "The automation framework for Python"
 authors = [
 	"Fabio Zadrozny <fabio@robocorp.com>",
 ]
 readme = "README.md"
 packages = [{include = "robocorp/tasks", from = "src"}]
 classifiers = [
@@ -13,15 +13,16 @@
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
     "Programming Language :: Python :: 3.11",
 ]
 
 [tool.poetry.dependencies]
 python = "^3.9"
-robocorp-log = "0.0.13"
+robocorp-log = "0.0.15"
+# robocorp-log = {path = "../log/", develop = true}
 
 [tool.mypy]
 mypy_path = "src:tests"
 
 [[tool.mypy.overrides]]
 module = "setuptools.*"
 ignore_missing_imports = true
```

### Comparing `robocorp_tasks-0.1.6/src/robocorp/tasks/__init__.py` & `robocorp_tasks-0.1.7/src/robocorp/tasks/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -26,9 +26,9 @@
 Note: Using the `cli.main(args)` is possible to run tasks programmatically, but
 clients using this approach MUST make sure that any code which must be
 automatically logged is not imported prior the the `cli.main` call.
 """
 
 from ._decorators import task
 
-__version__ = "0.1.6"
+__version__ = "0.1.7"
 version_info = [int(x) for x in __version__.split(".")]
```

### Comparing `robocorp_tasks-0.1.6/src/robocorp/tasks/_argdispatch.py` & `robocorp_tasks-0.1.7/src/robocorp/tasks/_argdispatch.py`

 * *Files 16% similar despite different names*

```diff
@@ -75,22 +75,45 @@
         run_parser.add_argument(
             "--max-log-file-size",
             dest="max_log_file_size",
             help="The maximum size for the log files (i.e.: 1MB, 500kb).",
             default="1MB",
         )
 
+        run_parser.add_argument(
+            "--console-colors",
+            help="""Define how the console messages shown should be color encoded.
+
+"auto" (default) will color either using the windows API or the ansi color codes.
+"plain" will disable console coloring.
+"ansi" will force the console coloring to use ansi color codes.
+""",
+            dest="console_colors",
+            type=str,
+            choices=["auto", "plain", "ansi"],
+            default="auto",
+        )
+
+        run_parser.add_argument(
+            "--log-output-to-stdout",
+            help="Can be used so that log messages are also sent to the 'stdout' (if not specified the RC_LOG_OUTPUT_STDOUT is also queried).",
+            dest="log_output_to_stdout",
+            type=str,
+            choices=["no", "json"],
+            default="",
+        )
+
         # List tasks
         list_parser = subparsers.add_parser(
             "list",
             help="Provides output to stdout with json contents of the tasks available.",
         )
         list_parser.add_argument(
             dest="path",
-            help="The directory or file from where the tasks should be listed.",
+            help="The directory or file from where the tasks should be listed (default is the current directory).",
             nargs="?",
             default=".",
         )
 
         return parser
 
     def process_args(self, args: List[str]) -> int:
```

### Comparing `robocorp_tasks-0.1.6/src/robocorp/tasks/_callback.py` & `robocorp_tasks-0.1.7/src/robocorp/tasks/_callback.py`

 * *Files identical despite different names*

### Comparing `robocorp_tasks-0.1.6/src/robocorp/tasks/_collect_tasks.py` & `robocorp_tasks-0.1.7/src/robocorp/tasks/_collect_tasks.py`

 * *Files identical despite different names*

### Comparing `robocorp_tasks-0.1.6/src/robocorp/tasks/_commands.py` & `robocorp_tasks-0.1.7/src/robocorp/tasks/_commands.py`

 * *Files 7% similar despite different names*

```diff
@@ -60,25 +60,35 @@
 @_arg_dispatch.register()
 def run(
     output_dir: str,
     path: str,
     task_name: str,
     max_log_files: int = 5,
     max_log_file_size: str = "1MB",
+    console_colors: str = "auto",
+    log_output_to_stdout: str = "",
 ) -> int:
     """
     Runs a task.
 
     Args:
         output_dir: The directory where output should be put.
         path: The path (file or directory where the tasks should be collected from.
         task_name: The name of the task to run.
         max_log_files: The maximum number of log files to be created (if more would
             be needed the oldest one is deleted).
         max_log_file_size: The maximum size for the created log files.
+        console_colors:
+            "auto": uses the default console
+            "plain": disables colors
+            "ansi": forces ansi color mode
+        log_output_to_stdout:
+            "": query the RC_LOG_OUTPUT_STDOUT value.
+            "no": don't provide log output to the stdout.
+            "json": provide json output to the stdout.
 
     Returns:
         0 if everything went well.
         1 if there was some error running the task.
     """
     from ._collect_tasks import collect_tasks
     from ._hooks import before_task_run, after_task_run
@@ -86,15 +96,19 @@
     from ._task import Context
     from ._protocols import Status
     from ._exceptions import RobocorpTasksCollectError
     from ._log_auto_setup import (
         setup_cli_auto_logging,
         read_filters_from_pyproject_toml,
     )
-    from ._log_output_setup import setup_log_output, setup_stdout_logging
+    from ._log_output_setup import setup_log_output
+    from robocorp.log import redirect
+    from robocorp.log import console
+
+    console.set_mode(console_colors)
 
     # Don't show internal machinery on tracebacks:
     # setting __tracebackhide__ will make it so that robocorp-log
     # won't show this frame onwards in the logging.
     __tracebackhide__ = 1
 
     p = Path(path).absolute()
@@ -107,19 +121,19 @@
 
     config = read_filters_from_pyproject_toml(context, p)
 
     with setup_cli_auto_logging(
         # Note: we can't customize what's a "project" file or a "library" file, right now
         # the customizations are all based on module names.
         config
-    ), setup_stdout_logging(), setup_log_output(
+    ), redirect.setup_stdout_logging(log_output_to_stdout), setup_log_output(
         output_dir=Path(output_dir),
         max_files=max_log_files,
         max_file_size=max_log_file_size,
-    ):
+    ), context.register_lifecycle_prints():
         run_status = "PASS"
         setup_message = ""
 
         run_name = f"{os.path.basename(path)} - {task_name}"
         log.start_run(run_name)
 
         try:
@@ -161,13 +175,14 @@
                 try:
                     task.run()
                     run_status = task.status = Status.PASS
                 except Exception as e:
                     run_status = task.status = Status.ERROR
                     returncode = 1
                     task.message = str(e)
+                    task.exc_info = sys.exc_info()
                 finally:
                     after_task_run(task)
 
             return returncode
         finally:
             log.end_run(run_name, run_status)
```

### Comparing `robocorp_tasks-0.1.6/src/robocorp/tasks/_decorators.py` & `robocorp_tasks-0.1.7/src/robocorp/tasks/_decorators.py`

 * *Files identical despite different names*

### Comparing `robocorp_tasks-0.1.6/src/robocorp/tasks/_hooks.py` & `robocorp_tasks-0.1.7/src/robocorp/tasks/_hooks.py`

 * *Files identical despite different names*

### Comparing `robocorp_tasks-0.1.6/src/robocorp/tasks/_log_auto_setup.py` & `robocorp_tasks-0.1.7/src/robocorp/tasks/_log_auto_setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -122,14 +122,15 @@
 
 def _log_before_task_run(task: ITask):
     log.start_task(
         task.name,
         task.module_name,
         task.filename,
         task.method.__code__.co_firstlineno,
+        getattr(task.method, "__doc__", ""),
     )
 
 
 def _log_after_task_run(task: ITask):
     status = task.status
     log.end_task(task.name, task.module_name, status, task.message)
```

### Comparing `robocorp_tasks-0.1.6/src/robocorp/tasks/_protocols.py` & `robocorp_tasks-0.1.7/src/robocorp/tasks/_protocols.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 from pathlib import Path
-from typing import TypeVar
+from typing import TypeVar, Optional
 import typing
+from robocorp.log.protocols import OptExcInfo
 
 
 T = TypeVar("T")
 Y = TypeVar("Y", covariant=True)
 
 
 def check_implements(x: T) -> T:
@@ -36,14 +37,15 @@
 class ITask(typing.Protocol):
     module_name: str
     filename: str
     method: typing.Callable
 
     status: str
     message: str
+    exc_info: Optional[OptExcInfo]
 
     @property
     def name(self) -> str:
         pass
 
     @property
     def lineno(self) -> int:
```

### Comparing `robocorp_tasks-0.1.6/src/robocorp/tasks/cli.py` & `robocorp_tasks-0.1.7/src/robocorp/tasks/cli.py`

 * *Files identical despite different names*

### Comparing `robocorp_tasks-0.1.6/PKG-INFO` & `robocorp_tasks-0.1.7/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,44 +1,45 @@
 Metadata-Version: 2.1
 Name: robocorp-tasks
-Version: 0.1.6
+Version: 0.1.7
 Summary: The automation framework for Python
 Author: Fabio Zadrozny
 Author-email: fabio@robocorp.com
 Requires-Python: >=3.9,<4.0
 Classifier: Development Status :: 3 - Alpha
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Software Development :: Libraries :: Application Frameworks
-Requires-Dist: robocorp-log (==0.0.13)
+Requires-Dist: robocorp-log (==0.0.15)
 Description-Content-Type: text/markdown
 
 # robocorp-tasks
 
-`robocorp-tasks` is a Python framework to simplify RPA development in Python.
+`robocorp-tasks` is a Python framework designed to simplify the development 
+of Python automations.
 
 > Note: The current version is still alpha but its public API is already meant
 > to be stable and new releases should keep backward compatibility.
 
 ## Why
 
-While Python is widely used in the RPA world, many solutions end up being ad-hoc, 
-making it difficult to navigate different projects or achieve comprehensible 
-logging out of the box.
+While Python is widely used in the automation world, many solutions end up being 
+ad-hoc, making it difficult to navigate different projects and keep up with the
+features required for analysing the results of such automations afterwards.
 
 ## How
 
-`robocorp-tasks` provides a runner for RPA tasks that offers logging 
-out of the box by leveraging `robocorp-log`, as well as the necessary 
-lifecycle management for running such tasks.
+`robocorp-tasks` provides a runner for running tasks that offers logging 
+out of the box for Python code (showing method calls, arguments, assigns, etc)
+by leveraging `robocorp-log`, and managing the lifecycle for running such tasks.
  
 ### Installation
 
 To install `robocorp-tasks`, use the following command:
 
 `pip install robocorp-tasks`
```

