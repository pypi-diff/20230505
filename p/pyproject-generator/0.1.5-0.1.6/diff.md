# Comparing `tmp/pyproject-generator-0.1.5.tar.gz` & `tmp/pyproject-generator-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyproject-generator-0.1.5.tar", last modified: Thu May  4 18:16:42 2023, max compression
+gzip compressed data, was "pyproject-generator-0.1.6.tar", last modified: Fri May  5 02:35:12 2023, max compression
```

## Comparing `pyproject-generator-0.1.5.tar` & `pyproject-generator-0.1.6.tar`

### file list

```diff
@@ -1,38 +1,39 @@
-drwxr-xr-x   0 cangyuanli   (501) staff       (20)        0 2023-05-04 18:16:42.780785 pyproject-generator-0.1.5/
--rw-r--r--   0 cangyuanli   (501) staff       (20)     1078 2023-05-04 01:48:13.000000 pyproject-generator-0.1.5/LICENSE
--rw-r--r--   0 cangyuanli   (501) staff       (20)     3564 2023-05-04 18:16:42.780945 pyproject-generator-0.1.5/PKG-INFO
--rw-r--r--   0 cangyuanli   (501) staff       (20)     3023 2023-05-04 18:03:16.000000 pyproject-generator-0.1.5/README.md
--rw-r--r--   0 cangyuanli   (501) staff       (20)      264 2023-05-04 02:13:28.000000 pyproject-generator-0.1.5/pyproject.toml
--rw-r--r--   0 cangyuanli   (501) staff       (20)      868 2023-05-04 18:16:42.785353 pyproject-generator-0.1.5/setup.cfg
-drwxr-xr-x   0 cangyuanli   (501) staff       (20)        0 2023-05-04 18:16:42.737608 pyproject-generator-0.1.5/src/
-drwxr-xr-x   0 cangyuanli   (501) staff       (20)        0 2023-05-04 18:16:42.746989 pyproject-generator-0.1.5/src/pyproject/
--rw-r--r--   0 cangyuanli   (501) staff       (20)       51 2023-05-03 20:58:26.000000 pyproject-generator-0.1.5/src/pyproject/__init__.py
--rw-r--r--   0 cangyuanli   (501) staff       (20)       22 2023-05-04 18:16:36.000000 pyproject-generator-0.1.5/src/pyproject/__version__.py
--rw-r--r--   0 cangyuanli   (501) staff       (20)     3530 2023-05-04 13:38:47.000000 pyproject-generator-0.1.5/src/pyproject/cli.py
-drwxr-xr-x   0 cangyuanli   (501) staff       (20)        0 2023-05-04 18:16:42.749914 pyproject-generator-0.1.5/src/pyproject/config/
--rw-r--r--   0 cangyuanli   (501) staff       (20)      237 2023-04-28 18:40:04.000000 pyproject-generator-0.1.5/src/pyproject/config/config.json
--rw-r--r--   0 cangyuanli   (501) staff       (20)      281 2023-05-03 20:05:37.000000 pyproject-generator-0.1.5/src/pyproject/config/default_config.json
--rw-r--r--   0 cangyuanli   (501) staff       (20)     1314 2023-05-04 13:50:03.000000 pyproject-generator-0.1.5/src/pyproject/logger.py
--rw-r--r--   0 cangyuanli   (501) staff       (20)    15640 2023-05-04 13:37:51.000000 pyproject-generator-0.1.5/src/pyproject/project_builder.py
--rw-r--r--   0 cangyuanli   (501) staff       (20)     2753 2023-05-04 01:29:47.000000 pyproject-generator-0.1.5/src/pyproject/spinner.py
-drwxr-xr-x   0 cangyuanli   (501) staff       (20)        0 2023-05-04 18:16:42.769211 pyproject-generator-0.1.5/src/pyproject/templates/
--rw-r--r--   0 cangyuanli   (501) staff       (20)     1498 2023-05-03 19:23:49.000000 pyproject-generator-0.1.5/src/pyproject/templates/gitignore.template
--rw-r--r--   0 cangyuanli   (501) staff       (20)      548 2023-04-30 01:20:52.000000 pyproject-generator-0.1.5/src/pyproject/templates/license_apache.template
--rw-r--r--   0 cangyuanli   (501) staff       (20)     1457 2023-05-04 13:35:45.000000 pyproject-generator-0.1.5/src/pyproject/templates/license_bsd3.template
--rw-r--r--   0 cangyuanli   (501) staff       (20)        0 2023-04-30 15:11:38.000000 pyproject-generator-0.1.5/src/pyproject/templates/license_gpl_v3.template
--rw-r--r--   0 cangyuanli   (501) staff       (20)     1074 2023-04-30 01:18:24.000000 pyproject-generator-0.1.5/src/pyproject/templates/license_mit.template
--rw-r--r--   0 cangyuanli   (501) staff       (20)      905 2023-05-03 23:48:11.000000 pyproject-generator-0.1.5/src/pyproject/templates/pre_commit_config.template
--rw-r--r--   0 cangyuanli   (501) staff       (20)      263 2023-05-04 02:15:39.000000 pyproject-generator-0.1.5/src/pyproject/templates/pyproject.template
--rw-r--r--   0 cangyuanli   (501) staff       (20)      986 2023-05-04 02:20:31.000000 pyproject-generator-0.1.5/src/pyproject/templates/readme.template
--rw-r--r--   0 cangyuanli   (501) staff       (20)      583 2023-04-30 15:11:46.000000 pyproject-generator-0.1.5/src/pyproject/templates/setup.template
--rw-r--r--   0 cangyuanli   (501) staff       (20)      649 2023-04-13 18:27:11.000000 pyproject-generator-0.1.5/src/pyproject/templates/tests.template
--rw-r--r--   0 cangyuanli   (501) staff       (20)      402 2023-04-12 23:45:24.000000 pyproject-generator-0.1.5/src/pyproject/templates/tox.template
-drwxr-xr-x   0 cangyuanli   (501) staff       (20)        0 2023-05-04 18:16:42.779674 pyproject-generator-0.1.5/src/pyproject_generator.egg-info/
--rw-r--r--   0 cangyuanli   (501) staff       (20)     3564 2023-05-04 18:16:42.000000 pyproject-generator-0.1.5/src/pyproject_generator.egg-info/PKG-INFO
--rw-r--r--   0 cangyuanli   (501) staff       (20)     1061 2023-05-04 18:16:42.000000 pyproject-generator-0.1.5/src/pyproject_generator.egg-info/SOURCES.txt
--rw-r--r--   0 cangyuanli   (501) staff       (20)        1 2023-05-04 18:16:42.000000 pyproject-generator-0.1.5/src/pyproject_generator.egg-info/dependency_links.txt
--rw-r--r--   0 cangyuanli   (501) staff       (20)       49 2023-05-04 18:16:42.000000 pyproject-generator-0.1.5/src/pyproject_generator.egg-info/entry_points.txt
--rw-r--r--   0 cangyuanli   (501) staff       (20)       13 2023-05-04 18:16:42.000000 pyproject-generator-0.1.5/src/pyproject_generator.egg-info/requires.txt
--rw-r--r--   0 cangyuanli   (501) staff       (20)       10 2023-05-04 18:16:42.000000 pyproject-generator-0.1.5/src/pyproject_generator.egg-info/top_level.txt
-drwxr-xr-x   0 cangyuanli   (501) staff       (20)        0 2023-05-04 18:16:42.780513 pyproject-generator-0.1.5/tests/
--rw-r--r--   0 cangyuanli   (501) staff       (20)        0 2023-04-19 15:24:26.000000 pyproject-generator-0.1.5/tests/test_pyproject.py
+drwxr-xr-x   0 cangyuanli   (501) staff       (20)        0 2023-05-05 02:35:12.456054 pyproject-generator-0.1.6/
+-rw-r--r--   0 cangyuanli   (501) staff       (20)     1078 2023-05-04 01:48:13.000000 pyproject-generator-0.1.6/LICENSE
+-rw-r--r--   0 cangyuanli   (501) staff       (20)     3871 2023-05-05 02:35:12.456309 pyproject-generator-0.1.6/PKG-INFO
+-rw-r--r--   0 cangyuanli   (501) staff       (20)     3330 2023-05-04 20:27:10.000000 pyproject-generator-0.1.6/README.md
+-rw-r--r--   0 cangyuanli   (501) staff       (20)      264 2023-05-04 02:13:28.000000 pyproject-generator-0.1.6/pyproject.toml
+-rw-r--r--   0 cangyuanli   (501) staff       (20)      868 2023-05-05 02:35:12.457296 pyproject-generator-0.1.6/setup.cfg
+drwxr-xr-x   0 cangyuanli   (501) staff       (20)        0 2023-05-05 02:35:12.423911 pyproject-generator-0.1.6/src/
+drwxr-xr-x   0 cangyuanli   (501) staff       (20)        0 2023-05-05 02:35:12.433962 pyproject-generator-0.1.6/src/pyproject/
+-rw-r--r--   0 cangyuanli   (501) staff       (20)       51 2023-05-03 20:58:26.000000 pyproject-generator-0.1.6/src/pyproject/__init__.py
+-rw-r--r--   0 cangyuanli   (501) staff       (20)       22 2023-05-05 02:34:52.000000 pyproject-generator-0.1.6/src/pyproject/__version__.py
+-rw-r--r--   0 cangyuanli   (501) staff       (20)     3991 2023-05-05 02:33:44.000000 pyproject-generator-0.1.6/src/pyproject/cli.py
+drwxr-xr-x   0 cangyuanli   (501) staff       (20)        0 2023-05-05 02:35:12.436285 pyproject-generator-0.1.6/src/pyproject/config/
+-rw-r--r--   0 cangyuanli   (501) staff       (20)      237 2023-04-28 18:40:04.000000 pyproject-generator-0.1.6/src/pyproject/config/config.json
+-rw-r--r--   0 cangyuanli   (501) staff       (20)      281 2023-05-03 20:05:37.000000 pyproject-generator-0.1.6/src/pyproject/config/default_config.json
+-rw-r--r--   0 cangyuanli   (501) staff       (20)     1029 2023-05-04 19:32:40.000000 pyproject-generator-0.1.6/src/pyproject/licenses.py
+-rw-r--r--   0 cangyuanli   (501) staff       (20)     1729 2023-05-05 02:24:45.000000 pyproject-generator-0.1.6/src/pyproject/logger.py
+-rw-r--r--   0 cangyuanli   (501) staff       (20)    15177 2023-05-05 02:24:58.000000 pyproject-generator-0.1.6/src/pyproject/project_builder.py
+-rw-r--r--   0 cangyuanli   (501) staff       (20)     2753 2023-05-04 01:29:47.000000 pyproject-generator-0.1.6/src/pyproject/spinner.py
+drwxr-xr-x   0 cangyuanli   (501) staff       (20)        0 2023-05-05 02:35:12.449102 pyproject-generator-0.1.6/src/pyproject/templates/
+-rw-r--r--   0 cangyuanli   (501) staff       (20)     1498 2023-05-03 19:23:49.000000 pyproject-generator-0.1.6/src/pyproject/templates/gitignore.template
+-rw-r--r--   0 cangyuanli   (501) staff       (20)      548 2023-04-30 01:20:52.000000 pyproject-generator-0.1.6/src/pyproject/templates/license_apache.template
+-rw-r--r--   0 cangyuanli   (501) staff       (20)     1457 2023-05-04 13:35:45.000000 pyproject-generator-0.1.6/src/pyproject/templates/license_bsd3.template
+-rw-r--r--   0 cangyuanli   (501) staff       (20)        0 2023-04-30 15:11:38.000000 pyproject-generator-0.1.6/src/pyproject/templates/license_gpl_v3.template
+-rw-r--r--   0 cangyuanli   (501) staff       (20)     1074 2023-04-30 01:18:24.000000 pyproject-generator-0.1.6/src/pyproject/templates/license_mit.template
+-rw-r--r--   0 cangyuanli   (501) staff       (20)      905 2023-05-03 23:48:11.000000 pyproject-generator-0.1.6/src/pyproject/templates/pre_commit_config.template
+-rw-r--r--   0 cangyuanli   (501) staff       (20)      263 2023-05-04 02:15:39.000000 pyproject-generator-0.1.6/src/pyproject/templates/pyproject.template
+-rw-r--r--   0 cangyuanli   (501) staff       (20)     1040 2023-05-04 20:10:03.000000 pyproject-generator-0.1.6/src/pyproject/templates/readme.template
+-rw-r--r--   0 cangyuanli   (501) staff       (20)      583 2023-04-30 15:11:46.000000 pyproject-generator-0.1.6/src/pyproject/templates/setup.template
+-rw-r--r--   0 cangyuanli   (501) staff       (20)      649 2023-04-13 18:27:11.000000 pyproject-generator-0.1.6/src/pyproject/templates/tests.template
+-rw-r--r--   0 cangyuanli   (501) staff       (20)      402 2023-04-12 23:45:24.000000 pyproject-generator-0.1.6/src/pyproject/templates/tox.template
+drwxr-xr-x   0 cangyuanli   (501) staff       (20)        0 2023-05-05 02:35:12.454718 pyproject-generator-0.1.6/src/pyproject_generator.egg-info/
+-rw-r--r--   0 cangyuanli   (501) staff       (20)     3871 2023-05-05 02:35:12.000000 pyproject-generator-0.1.6/src/pyproject_generator.egg-info/PKG-INFO
+-rw-r--r--   0 cangyuanli   (501) staff       (20)     1087 2023-05-05 02:35:12.000000 pyproject-generator-0.1.6/src/pyproject_generator.egg-info/SOURCES.txt
+-rw-r--r--   0 cangyuanli   (501) staff       (20)        1 2023-05-05 02:35:12.000000 pyproject-generator-0.1.6/src/pyproject_generator.egg-info/dependency_links.txt
+-rw-r--r--   0 cangyuanli   (501) staff       (20)       49 2023-05-05 02:35:12.000000 pyproject-generator-0.1.6/src/pyproject_generator.egg-info/entry_points.txt
+-rw-r--r--   0 cangyuanli   (501) staff       (20)       13 2023-05-05 02:35:12.000000 pyproject-generator-0.1.6/src/pyproject_generator.egg-info/requires.txt
+-rw-r--r--   0 cangyuanli   (501) staff       (20)       10 2023-05-05 02:35:12.000000 pyproject-generator-0.1.6/src/pyproject_generator.egg-info/top_level.txt
+drwxr-xr-x   0 cangyuanli   (501) staff       (20)        0 2023-05-05 02:35:12.455538 pyproject-generator-0.1.6/tests/
+-rw-r--r--   0 cangyuanli   (501) staff       (20)        0 2023-04-19 15:24:26.000000 pyproject-generator-0.1.6/tests/test_pyproject.py
```

### Comparing `pyproject-generator-0.1.5/LICENSE` & `pyproject-generator-0.1.6/LICENSE`

 * *Files identical despite different names*

### Comparing `pyproject-generator-0.1.5/PKG-INFO` & `pyproject-generator-0.1.6/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyproject-generator
-Version: 0.1.5
+Version: 0.1.6
 Summary: A command line tool to setup Python packages
 Home-page: https://github.com/CangyuanLi/pyproject
 Author: Cangyuan Li
 Author-email: everest229@gmail.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/CangyuanLi/pyproject/issues
 Classifier: Programming Language :: Python :: 3
@@ -41,15 +41,15 @@
 
 ```sh
 pip install pyproject-generator
 ```
 
 Afterwards, a pyproject command will be exposed on your system.
 
-## Running
+## Initializing a Project
 
 Simply run
 ```sh
 pyproject init {project_name}
 ```
 
 to create your project folder. It will automatically setup a package structure, virtual
@@ -76,44 +76,52 @@
 │       ├── __init__.py
 │       └── py.typed
 ├── tests
 │   └── test_myproject.py
 └── tox.ini
 ```
 
+## Configuring pyproject-generator
+
 **pyproject** also allows you to configure your author name, email, Github URL,
 PyPI username and password, and a list of default dependencies that you want to install.
 Please note that your credentials are simply stored locally as plaintext.
 If you do not wish to store them, you can simply pass them in manually
 via the --pypi_username and --pypi_password flags, or run without any flags and type
 them in as required. To configure, run
 
 ```sh
 pyproject config --author="" --email="" --github_url="" --pypi_username="" --pypi_password=""
 ```
 
-You may set dependencies one of three ways. In all cases, pass in a comma-delimited string.
+You may set dependencies one of three ways. In all cases, pass in a comma-delimited
+string (for multiple dependencies) or a string (for one dependency).
 You can set the dependencies, which overrides the default settings.
 
 ```sh
-pyproject config --set_dependencies
+pyproject config --set_dependencies="white,ruff,mypy"
 ```
 
 You may add dependencies:
 
 ```sh
-pyproject config --add_dependencies
+pyproject config --add_dependencies="django"
 ```
 
 And you may remove dependencies:
 
 ```sh
-pyproject config --remove_dependencies
+pyproject config --remove_dependencies="pre-commit"
 ```
 
+Note that these flags also work with the `init` action. `config` merely does the work
+of saving them locally to be re-used later.
+
+## Uploading a Project
+
 **pyproject** also supplies an upload function. Run
 
 ```sh
 pyproject upload
 ```
 
 to build and upload your package to PyPI.
```

### Comparing `pyproject-generator-0.1.5/README.md` & `pyproject-generator-0.1.6/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -25,15 +25,15 @@
 
 ```sh
 pip install pyproject-generator
 ```
 
 Afterwards, a pyproject command will be exposed on your system.
 
-## Running
+## Initializing a Project
 
 Simply run
 ```sh
 pyproject init {project_name}
 ```
 
 to create your project folder. It will automatically setup a package structure, virtual
@@ -60,44 +60,52 @@
 │       ├── __init__.py
 │       └── py.typed
 ├── tests
 │   └── test_myproject.py
 └── tox.ini
 ```
 
+## Configuring pyproject-generator
+
 **pyproject** also allows you to configure your author name, email, Github URL,
 PyPI username and password, and a list of default dependencies that you want to install.
 Please note that your credentials are simply stored locally as plaintext.
 If you do not wish to store them, you can simply pass them in manually
 via the --pypi_username and --pypi_password flags, or run without any flags and type
 them in as required. To configure, run
 
 ```sh
 pyproject config --author="" --email="" --github_url="" --pypi_username="" --pypi_password=""
 ```
 
-You may set dependencies one of three ways. In all cases, pass in a comma-delimited string.
+You may set dependencies one of three ways. In all cases, pass in a comma-delimited
+string (for multiple dependencies) or a string (for one dependency).
 You can set the dependencies, which overrides the default settings.
 
 ```sh
-pyproject config --set_dependencies
+pyproject config --set_dependencies="white,ruff,mypy"
 ```
 
 You may add dependencies:
 
 ```sh
-pyproject config --add_dependencies
+pyproject config --add_dependencies="django"
 ```
 
 And you may remove dependencies:
 
 ```sh
-pyproject config --remove_dependencies
+pyproject config --remove_dependencies="pre-commit"
 ```
 
+Note that these flags also work with the `init` action. `config` merely does the work
+of saving them locally to be re-used later.
+
+## Uploading a Project
+
 **pyproject** also supplies an upload function. Run
 
 ```sh
 pyproject upload
 ```
 
 to build and upload your package to PyPI.
```

### Comparing `pyproject-generator-0.1.5/setup.cfg` & `pyproject-generator-0.1.6/setup.cfg`

 * *Files identical despite different names*

### Comparing `pyproject-generator-0.1.5/src/pyproject/cli.py` & `pyproject-generator-0.1.6/src/pyproject/cli.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,16 +1,18 @@
 import argparse
 import typing
 from typing import Optional
 
 from .__version__ import __version__
-from .project_builder import LICENSE_NAME_MAPPER, Action, ProjectBuilder
+from .licenses import LICENSES
+from .logger import Level, Logger
+from .project_builder import Action, ProjectBuilder
 
-ACTIONS = list(typing.get_args(Action))
-LICENSES = list(LICENSE_NAME_MAPPER.keys())
+ACTIONS = typing.get_args(Action)
+ALLOWED_LICENSES = tuple(LICENSES.keys())
 
 
 def _parse_arg_to_set(string: Optional[str], sep: str = ",") -> set[str]:
     """Expects a delimited string of arguments, e.g. `a,b,c,d`. Transforms string
     into a set.
 
     Args:
@@ -25,15 +27,15 @@
 
     return set(word.strip() for word in string.split(sep))
 
 
 def get_parser():
     parser = argparse.ArgumentParser(description="Generate python project")
 
-    parser.add_argument("action", type=str, choices=ACTIONS, help="Action")
+    parser.add_argument("action", type=str, help="Action")
     parser.add_argument(
         "project_name", type=str, nargs="?", default=None, help="Name of the project"
     )
 
     parser.add_argument(
         "--reset_config",
         required=False,
@@ -41,15 +43,15 @@
         help="Reset configuration to default settings.",
     )
     parser.add_argument("--pypi_username", type=str, help="Set PyPI username")
     parser.add_argument("--pypi_password", type=str, help="Set PyPI password")
     parser.add_argument("--github_url", type=str, help="Set Github URL")
     parser.add_argument("--author", type=str, help="Set author name")
     parser.add_argument("--email", type=str, help="Set author email")
-    parser.add_argument("--license", type=str, choices=LICENSES, help="Set license")
+    parser.add_argument("--license", type=str, help="Set license")
     parser.add_argument(
         "--set_dependencies",
         type=str,
         help=(
             "Set dependencies to always download. Overwrites saved config. Pass in a"
             " comma delimited string"
         ),
@@ -82,18 +84,30 @@
     return parser
 
 
 def main():
     parser = get_parser()
     args = parser.parse_args()
 
+    options = {"quiet": args.quiet}
+
+    # set up the console for logging
+    logging_level = Level.INFO
+    if options["quiet"]:
+        logging_level = Level.ERROR
+    logger = Logger(logging_level)
+
+    if args.action not in ACTIONS:
+        logger.error(f"Invalid choice `{args.action}`, choose from {ACTIONS}")
+
     if args.action == "init" and args.project_name is None:
-        parser.error("init requires project name")
+        logger.error("Action `init` requires project name")
 
-    options = {"quiet": args.quiet}
+    if args.license not in LICENSES and args.license is not None:
+        logger.error(f"Invalid choice `{args.license}`, choose from {ALLOWED_LICENSES}")
 
     config = {
         "pypi_username": args.pypi_username,
         "pypi_password": args.pypi_password,
         "github_url": args.github_url,
         "author": args.author,
         "email": args.email,
@@ -101,13 +115,13 @@
         "set_dependencies": _parse_arg_to_set(args.set_dependencies),
         "add_dependencies": _parse_arg_to_set(args.add_dependencies),
         "remove_dependencies": _parse_arg_to_set(args.remove_dependencies),
         "reset_config": args.reset_config,
         "show": args.show,
     }
 
-    builder = ProjectBuilder(config=config, options=options)
+    builder = ProjectBuilder(config=config, options=options, logger=logger)
     builder.dispatch(action=args.action, project_name=args.project_name)
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `pyproject-generator-0.1.5/src/pyproject/logger.py` & `pyproject-generator-0.1.6/src/pyproject/logger.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,54 +1,70 @@
 from __future__ import annotations
 
 import enum
+import sys
 from typing import Callable, Optional
 
 import rich.pretty
 from rich.console import Console
 
 from .spinner import Spinner
 
 
 class Level(enum.Enum):
     ERROR = 1
-    INFO = 2
+    WARNING = 2
+    INFO = 3
 
     def __lt__(self, other: Level) -> bool:
         if isinstance(other, Level):
             return self.value < other.value
 
         return NotImplemented
 
 
-class CustomConsole(Console):
+class Logger:
     def __init__(self, logging_level: Level):
-        super().__init__()
+        self._console = Console()
+        self._err_console = Console(stderr=True)
         self._level = logging_level
 
     def pprint(self, *args, **kwargs):
-        rich.pretty.pprint(*args, **kwargs, console=self)
+        rich.pretty.pprint(*args, **kwargs, console=self._console)
 
     def info(self, *args, **kwargs):
         if Level.INFO > self._level:
             return None
 
-        self.print(*args, **kwargs)
+        self._console.print(*args, **kwargs)
+
+    def warning(self, warning: str, **kwargs):
+        if Level.WARNING > self._level:
+            return None
+
+        self._err_console.print(
+            f"[bold yellow]Warning[/bold yellow]: [yellow]{warning}[/yellow]", **kwargs
+        )
 
     def error(self, error_message: str, **kwargs):
-        self.print(f"[bold red]Error[/bold red]: [red]{error_message}[/red]", **kwargs)
+        self._err_console.print(
+            f"[bold red]Error[/bold red]: [red]{error_message}[/red]", **kwargs
+        )
+        sys.exit(1)
 
     def spinner(
         self,
         func: Callable,
         text: str,
         delay: float = 0.1,
         prefix: str = "    ",
         suffix: str = " ",
         clear: bool = False,
         min_show_duration: Optional[float] = None,
     ):
         if Level.INFO > self._level:
             return func()
 
-        with Spinner(self, text, delay, prefix, suffix, clear, min_show_duration):
+        with Spinner(
+            self._console, text, delay, prefix, suffix, clear, min_show_duration
+        ):
             return func()
```

### Comparing `pyproject-generator-0.1.5/src/pyproject/project_builder.py` & `pyproject-generator-0.1.6/src/pyproject/project_builder.py`

 * *Files 4% similar despite different names*

```diff
@@ -6,69 +6,52 @@
 import datetime
 import json
 import os
 import re
 import shutil
 import string
 import subprocess
-import sys
 import venv
 from pathlib import Path
 from types import SimpleNamespace
 from typing import Literal, Optional, Union
 
 import platformdirs
 from rich.panel import Panel
 
-from .logger import CustomConsole, Level
+from .licenses import LICENSES, License
+from .logger import Logger
 
 # Globals
 
 BASE_PATH = Path(__file__).resolve().parents[0]
 TEMPLATE_PATH = BASE_PATH / "templates"
 USER_CONFIG_PATH = platformdirs.user_config_dir(
     appname="pyproject-generator", appauthor="cangyuanli"
 )
 
-LICENSE_NAME_MAPPER = {
-    "mit": "MIT",
-    "apache": "Apache",
-    "gpl_v3": "GPL v3",
-    "bsd3": "BSD 3-Clause",
-}
-
 # Types
 
 Action = Literal["init", "upload", "config"]
 PathLike = Union[Path, str]
 
 
 @dataclasses.dataclass
-class License:
-    short_name: str
-    proper_name: Optional[str] = None
-
-    def __post_init__(self):
-        if self.proper_name is None:
-            self.proper_name = LICENSE_NAME_MAPPER[self.short_name]
-
-
-@dataclasses.dataclass
 class Config:
     pypi_username: str
     pypi_password: str
     github_url: str
     author: str
     email: str
     license: License
     dependencies: set[str]
 
     def __post_init__(self):
         if isinstance(self.license, str):
-            self.license = License(self.license)
+            self.license = LICENSES[self.license]
         self.dependencies = set(self.dependencies)
 
     def to_json_representable(self) -> dict:
         _dict = self.to_dict()
         _dict["license"] = self.license.short_name
         _dict["dependencies"] = sorted(list(self.dependencies))
 
@@ -156,26 +139,22 @@
 
 
 class ProjectBuilder:
     def __init__(
         self,
         config: dict,
         options: dict,
+        logger: Logger,
         template_path: PathLike = TEMPLATE_PATH,
         user_config_dir: PathLike = USER_CONFIG_PATH,
     ) -> None:
         self.proj_path = Path().cwd()
 
         self._template_path = Path(template_path)
-
-        # set up the console for logging
-        self._logging_level = Level.INFO
-        if options["quiet"]:
-            self._logging_level = Level.ERROR
-        self._console = CustomConsole(self._logging_level)
+        self._logger = logger
 
         self._user_config_dir = Path(user_config_dir)
         self._create_config_dir()
         self._config = self._set_config(config)
 
     @staticmethod
     def _validate_project_name(project_name: str) -> None:
@@ -224,14 +203,16 @@
             "PYPI_USERNAME": config.pypi_username,
             "PYPI_PASSWORD": config.pypi_password,
             "GITHUB_URL": config.github_url,
             "AUTHOR": config.author,
             "EMAIL": config.email,
             "YEAR": datetime.datetime.now().year,
             "LICENSE": config.license.proper_name,
+            "LICENSE_BADGE": config.license.badge_url,
+            "LICENSE_LINK": config.license.link,
         }
 
         filled_in_templates = {}
         for file in self._template_path.glob("*.template"):
             with open(file, "r") as f:
                 src = string.Template(f.read())
                 result = src.substitute(d)
@@ -288,127 +269,125 @@
             project_name (str): User-supplied name of project
         """
 
         # Create the project directory
         try:
             self._validate_project_name(project_name)
         except ValueError as e:
-            self._console.error(str(e))
-            sys.exit(1)
+            self._logger.error(str(e))
 
         proj_path = self.proj_path / project_name
 
         try:
             proj_path.mkdir()
         except FileExistsError:
-            self._console.error(f"{proj_path} already exists")
-            sys.exit(1)
+            self._logger.error(f"{proj_path} already exists")
 
-        self._console.info(Panel("Creating project files..."), justify="left")
+        self._logger.info(Panel("Creating project files..."), justify="left")
 
         # Fill in templates
-        templates = self._console.spinner(
+        templates = self._logger.spinner(
             lambda: self._fill_in_templates(project_name),
             "Filling in templates",
             clear=True,
             min_show_duration=0.2,
         )
 
         # src
-        self._console.spinner(
+        self._logger.spinner(
             lambda: self._init_source_directory(proj_path, project_name),
             "Creating source directory",
             clear=True,
             min_show_duration=0.2,
         )
 
         # tests
-        self._console.spinner(
+        self._logger.spinner(
             lambda: self._init_tests(proj_path, project_name),
             "Creating tests",
             clear=True,
             min_show_duration=0.2,
         )
 
         # benchmarks
-        self._console.spinner(
+        self._logger.spinner(
             lambda: self._init_benchmarks(proj_path),
             "Creating benchmarks",
             clear=True,
             min_show_duration=0.2,
         )
 
         # github actions
-        self._console.spinner(
+        self._logger.spinner(
             lambda: self._init_github_actions(proj_path, templates),
             "Setting up Github Actions",
             clear=True,
             min_show_duration=0.2,
         )
 
         # misc setup
-        self._console.spinner(
+        self._logger.spinner(
             lambda: self._init_config_files(proj_path, templates),
             "Setting up configuration files",
             clear=True,
             min_show_duration=0.2,
         )
 
-        self._console.info("Building project skeleton completed with no errors.")
+        self._logger.info("Building project skeleton completed with no errors.")
 
         # Setup the virtual environment
-        self._console.info(
+        self._logger.info(
             Panel("Setting up the virtual environment..."), justify="left"
         )
 
         venv_builder = Env(with_pip=True)
         venv_builder.venv_create(proj_path / "venv")
 
         # Install developer dependencies
 
-        self._console.spinner(
+        self._logger.spinner(
             lambda: venv_builder.run_bin(
                 ["python", "-m", "pip", "install", "-U", "pip"],
                 stdout=subprocess.DEVNULL,
             ),
             text="pip",
         )
 
         for dep in sorted(list(self._config.dependencies)):
-            self._console.spinner(
+            self._logger.spinner(
                 lambda: venv_builder.run_bin(
                     ["pip", "install", dep], stdout=subprocess.DEVNULL
                 ),
                 text=dep,
             )
 
-        self._console.info(Panel("Finalizing project..."), justify="left")
+        self._logger.info(Panel("Finalizing project..."), justify="left")
 
         # Create requirements_dev file
         def _create_req_file():
             reqs = venv_builder.run_bin(["pip", "freeze"], capture_output=True)
             (proj_path / "requirements_dev.txt").write_bytes(reqs.stdout)
 
-        self._console.spinner(
+        self._logger.spinner(
             _create_req_file,
             "Creating requirements_dev.txt",
             clear=True,
             min_show_duration=0.2,
         )
 
         # Ensure pre-commit is up to date
-        self._console.spinner(
+        self._logger.spinner(
             lambda: venv_builder.run_bin(
                 ["pre-commit", "autoupdate"], stdout=subprocess.DEVNULL
             ),
             "Ensuring pre-commit config is up to date",
             clear=True,
         )
 
-        self._console.info(f"Done setting up {project_name}!", style="green")
+        self._logger.info(f"Done setting up {project_name}!", style="green")
 
     def _parse_config_file(self, filename: PathLike) -> Config:
         if filename == "default_config.json":
             path = BASE_PATH / "config/default_config.json"
         elif filename == "config.json":
             path = self._user_config_dir / filename
         else:
@@ -445,15 +424,15 @@
             config["dependencies"] = config["set_dependencies"]
 
         _config = CLIConfig(**config)
 
         merged_config = Config.merge(saved_config, _config)
 
         if _config.show:
-            self._console.pprint(merged_config.to_json_representable())
+            self._logger.pprint(merged_config.to_json_representable())
 
         return merged_config
 
     def _write_config_file(self, config: Config):
         with open(self._user_config_dir / "config.json", "w") as f:
             json.dump(config.to_json_representable(), f, indent=4)
```

### Comparing `pyproject-generator-0.1.5/src/pyproject/spinner.py` & `pyproject-generator-0.1.6/src/pyproject/spinner.py`

 * *Files identical despite different names*

### Comparing `pyproject-generator-0.1.5/src/pyproject/templates/gitignore.template` & `pyproject-generator-0.1.6/src/pyproject/templates/gitignore.template`

 * *Files identical despite different names*

### Comparing `pyproject-generator-0.1.5/src/pyproject/templates/license_apache.template` & `pyproject-generator-0.1.6/src/pyproject/templates/license_apache.template`

 * *Files identical despite different names*

### Comparing `pyproject-generator-0.1.5/src/pyproject/templates/license_bsd3.template` & `pyproject-generator-0.1.6/src/pyproject/templates/license_bsd3.template`

 * *Files identical despite different names*

### Comparing `pyproject-generator-0.1.5/src/pyproject/templates/license_mit.template` & `pyproject-generator-0.1.6/src/pyproject/templates/license_mit.template`

 * *Files identical despite different names*

### Comparing `pyproject-generator-0.1.5/src/pyproject/templates/pre_commit_config.template` & `pyproject-generator-0.1.6/src/pyproject/templates/pre_commit_config.template`

 * *Files identical despite different names*

### Comparing `pyproject-generator-0.1.5/src/pyproject/templates/readme.template` & `pyproject-generator-0.1.6/src/pyproject/templates/readme.template`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 # $PACKAGE:
 [![PyPI version](https://badge.fury.io/py/$PACKAGE.svg)](https://badge.fury.io/py/$PACKAGE)
 ![PyPI - Downloads](https://img.shields.io/pypi/dm/$PACKAGE)
+[![License: $LICENSE]($LICENSE_BADGE)]($LICENSE_LINK)
 ![Tests]($GITHUB_URL/$PACKAGE/actions/workflows/tests.yml/badge.svg)
 [![pre-commit](https://img.shields.io/badge/pre--commit-enabled-brightgreen?logo=pre-commit&logoColor=white)](https://github.com/pre-commit/pre-commit)
 [![Checked with mypy](http://www.mypy-lang.org/static/mypy_badge.svg)](http://mypy-lang.org/)
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 [![Imports: isort](https://img.shields.io/badge/%20imports-isort-%231674b1?style=flat&labelColor=ef8336)](https://pycqa.github.io/isort/)
 
 ## What is it?
```

### Comparing `pyproject-generator-0.1.5/src/pyproject/templates/setup.template` & `pyproject-generator-0.1.6/src/pyproject/templates/setup.template`

 * *Files identical despite different names*

### Comparing `pyproject-generator-0.1.5/src/pyproject/templates/tests.template` & `pyproject-generator-0.1.6/src/pyproject/templates/tests.template`

 * *Files identical despite different names*

### Comparing `pyproject-generator-0.1.5/src/pyproject_generator.egg-info/PKG-INFO` & `pyproject-generator-0.1.6/src/pyproject_generator.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyproject-generator
-Version: 0.1.5
+Version: 0.1.6
 Summary: A command line tool to setup Python packages
 Home-page: https://github.com/CangyuanLi/pyproject
 Author: Cangyuan Li
 Author-email: everest229@gmail.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/CangyuanLi/pyproject/issues
 Classifier: Programming Language :: Python :: 3
@@ -41,15 +41,15 @@
 
 ```sh
 pip install pyproject-generator
 ```
 
 Afterwards, a pyproject command will be exposed on your system.
 
-## Running
+## Initializing a Project
 
 Simply run
 ```sh
 pyproject init {project_name}
 ```
 
 to create your project folder. It will automatically setup a package structure, virtual
@@ -76,44 +76,52 @@
 │       ├── __init__.py
 │       └── py.typed
 ├── tests
 │   └── test_myproject.py
 └── tox.ini
 ```
 
+## Configuring pyproject-generator
+
 **pyproject** also allows you to configure your author name, email, Github URL,
 PyPI username and password, and a list of default dependencies that you want to install.
 Please note that your credentials are simply stored locally as plaintext.
 If you do not wish to store them, you can simply pass them in manually
 via the --pypi_username and --pypi_password flags, or run without any flags and type
 them in as required. To configure, run
 
 ```sh
 pyproject config --author="" --email="" --github_url="" --pypi_username="" --pypi_password=""
 ```
 
-You may set dependencies one of three ways. In all cases, pass in a comma-delimited string.
+You may set dependencies one of three ways. In all cases, pass in a comma-delimited
+string (for multiple dependencies) or a string (for one dependency).
 You can set the dependencies, which overrides the default settings.
 
 ```sh
-pyproject config --set_dependencies
+pyproject config --set_dependencies="white,ruff,mypy"
 ```
 
 You may add dependencies:
 
 ```sh
-pyproject config --add_dependencies
+pyproject config --add_dependencies="django"
 ```
 
 And you may remove dependencies:
 
 ```sh
-pyproject config --remove_dependencies
+pyproject config --remove_dependencies="pre-commit"
 ```
 
+Note that these flags also work with the `init` action. `config` merely does the work
+of saving them locally to be re-used later.
+
+## Uploading a Project
+
 **pyproject** also supplies an upload function. Run
 
 ```sh
 pyproject upload
 ```
 
 to build and upload your package to PyPI.
```

### Comparing `pyproject-generator-0.1.5/src/pyproject_generator.egg-info/SOURCES.txt` & `pyproject-generator-0.1.6/src/pyproject_generator.egg-info/SOURCES.txt`

 * *Files 8% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 LICENSE
 README.md
 pyproject.toml
 setup.cfg
 src/pyproject/__init__.py
 src/pyproject/__version__.py
 src/pyproject/cli.py
+src/pyproject/licenses.py
 src/pyproject/logger.py
 src/pyproject/project_builder.py
 src/pyproject/spinner.py
 src/pyproject/config/config.json
 src/pyproject/config/default_config.json
 src/pyproject/templates/gitignore.template
 src/pyproject/templates/license_apache.template
```

