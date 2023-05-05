# Comparing `tmp/venv-modulefile-0.0.2.tar.gz` & `tmp/venv-modulefile-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/volatile/catA/rl222169/softs/custom_venv/extend_python_venv_with_environment_modules/dist/tmp3h54xkcm/venv-modulefile-0.0.2.ta", last modified: Wed Apr 19 17:39:53 2023, max compression
+gzip compressed data, was "/volatile/catA/rl222169/softs/custom_venv/extend_python_venv_with_environment_modules/dist/tmp3w1inqb9/venv-modulefile-0.0.8.ta", last modified: Fri May  5 07:36:30 2023, max compression
```

## Comparing `venv-modulefile-0.0.2.tar` & `venv-modulefile-0.0.8.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxrwx---   0 rl222169 (222169) dm2s-user-cat-a (470572)        0 2023-04-19 17:39:53.000000 venv-modulefile-0.0.2/
--rw-rw----   0 rl222169 (222169) dm2s-user-cat-a (470572)     1188 2023-04-19 17:39:53.000000 venv-modulefile-0.0.2/PKG-INFO
--rw-rw----   0 rl222169 (222169) dm2s-user-cat-a (470572)       81 2023-04-19 16:42:52.000000 venv-modulefile-0.0.2/pyproject.toml
--rw-rw----   0 rl222169 (222169) dm2s-user-cat-a (470572)       38 2023-04-19 17:39:53.000000 venv-modulefile-0.0.2/setup.cfg
--rw-rw----   0 rl222169 (222169) dm2s-user-cat-a (470572)       22 2023-04-19 16:42:18.000000 venv-modulefile-0.0.2/MANIFEST.in
--rw-rw----   0 rl222169 (222169) dm2s-user-cat-a (470572)      909 2023-04-18 14:24:37.000000 venv-modulefile-0.0.2/README.md
--rw-rw----   0 rl222169 (222169) dm2s-user-cat-a (470572)     9590 2023-04-19 17:34:33.000000 venv-modulefile-0.0.2/setup.py
-drwxrwx---   0 rl222169 (222169) dm2s-user-cat-a (470572)        0 2023-04-19 17:39:53.000000 venv-modulefile-0.0.2/src/
-drwxrwx---   0 rl222169 (222169) dm2s-user-cat-a (470572)        0 2023-04-19 17:39:53.000000 venv-modulefile-0.0.2/src/venvmod/
--rw-rw----   0 rl222169 (222169) dm2s-user-cat-a (470572)        6 2023-04-19 17:38:08.000000 venv-modulefile-0.0.2/src/venvmod/VERSION
--rw-rw----   0 rl222169 (222169) dm2s-user-cat-a (470572)       45 2023-04-19 16:36:02.000000 venv-modulefile-0.0.2/src/venvmod/__init__.py
--rw-rw----   0 rl222169 (222169) dm2s-user-cat-a (470572)     1666 2023-04-19 15:36:05.000000 venv-modulefile-0.0.2/src/venvmod/tools.py
-drwxrwx---   0 rl222169 (222169) dm2s-user-cat-a (470572)        0 2023-04-19 17:39:53.000000 venv-modulefile-0.0.2/src/venvmod/commands/
--rw-rw----   0 rl222169 (222169) dm2s-user-cat-a (470572)     1336 2023-04-19 17:34:50.000000 venv-modulefile-0.0.2/src/venvmod/commands/test_imports.py
--rw-rw----   0 rl222169 (222169) dm2s-user-cat-a (470572)     1236 2023-04-19 11:41:45.000000 venv-modulefile-0.0.2/src/venvmod/commands/__init__.py
--rw-rw----   0 rl222169 (222169) dm2s-user-cat-a (470572)     2894 2023-04-19 16:35:42.000000 venv-modulefile-0.0.2/src/venvmod/commands/create_module.py
--rw-rw----   0 rl222169 (222169) dm2s-user-cat-a (470572)     4578 2023-04-19 17:36:07.000000 venv-modulefile-0.0.2/src/venvmod/commands/append_module.py
--rw-rw----   0 rl222169 (222169) dm2s-user-cat-a (470572)    10971 2023-04-19 15:26:15.000000 venv-modulefile-0.0.2/src/venvmod/modulefile.py
--rw-rw----   0 rl222169 (222169) dm2s-user-cat-a (470572)       47 2023-04-19 09:35:41.000000 venv-modulefile-0.0.2/src/README.md
-drwxrwx---   0 rl222169 (222169) dm2s-user-cat-a (470572)        0 2023-04-19 17:39:53.000000 venv-modulefile-0.0.2/src/venv_modulefile.egg-info/
--rw-rw----   0 rl222169 (222169) dm2s-user-cat-a (470572)      809 2023-04-19 17:39:53.000000 venv-modulefile-0.0.2/src/venv_modulefile.egg-info/entry_points.txt
--rw-rw----   0 rl222169 (222169) dm2s-user-cat-a (470572)        8 2023-04-19 17:39:53.000000 venv-modulefile-0.0.2/src/venv_modulefile.egg-info/top_level.txt
--rw-rw----   0 rl222169 (222169) dm2s-user-cat-a (470572)      567 2023-04-19 17:39:53.000000 venv-modulefile-0.0.2/src/venv_modulefile.egg-info/SOURCES.txt
--rw-rw----   0 rl222169 (222169) dm2s-user-cat-a (470572)     1188 2023-04-19 17:39:53.000000 venv-modulefile-0.0.2/src/venv_modulefile.egg-info/PKG-INFO
--rw-rw----   0 rl222169 (222169) dm2s-user-cat-a (470572)        1 2023-04-19 17:39:53.000000 venv-modulefile-0.0.2/src/venv_modulefile.egg-info/dependency_links.txt
--rw-rw----   0 rl222169 (222169) dm2s-user-cat-a (470572)      229 2023-04-19 17:39:53.000000 venv-modulefile-0.0.2/src/venv_modulefile.egg-info/requires.txt
--rw-rw----   0 rl222169 (222169) dm2s-user-cat-a (470572)     1302 2023-04-18 14:24:37.000000 venv-modulefile-0.0.2/LICENSE.md
+drwxrwx---   0 rl222169 (222169) dm2s-user-cat-a (470572)        0 2023-05-05 07:36:30.000000 venv-modulefile-0.0.8/
+-rw-rw----   0 rl222169 (222169) dm2s-user-cat-a (470572)     2042 2023-05-05 07:36:30.000000 venv-modulefile-0.0.8/PKG-INFO
+-rw-rw----   0 rl222169 (222169) dm2s-user-cat-a (470572)       81 2023-05-04 08:19:39.000000 venv-modulefile-0.0.8/pyproject.toml
+-rw-rw----   0 rl222169 (222169) dm2s-user-cat-a (470572)       38 2023-05-05 07:36:30.000000 venv-modulefile-0.0.8/setup.cfg
+-rw-rw----   0 rl222169 (222169) dm2s-user-cat-a (470572)       22 2023-04-19 16:42:18.000000 venv-modulefile-0.0.8/MANIFEST.in
+-rw-rw----   0 rl222169 (222169) dm2s-user-cat-a (470572)      898 2023-05-04 08:19:39.000000 venv-modulefile-0.0.8/README.md
+-rw-rw----   0 rl222169 (222169) dm2s-user-cat-a (470572)     9593 2023-05-04 08:46:54.000000 venv-modulefile-0.0.8/setup.py
+drwxrwx---   0 rl222169 (222169) dm2s-user-cat-a (470572)        0 2023-05-05 07:36:30.000000 venv-modulefile-0.0.8/src/
+drwxrwx---   0 rl222169 (222169) dm2s-user-cat-a (470572)        0 2023-05-05 07:36:30.000000 venv-modulefile-0.0.8/src/venvmod/
+-rw-rw----   0 rl222169 (222169) dm2s-user-cat-a (470572)        6 2023-05-05 07:35:53.000000 venv-modulefile-0.0.8/src/venvmod/VERSION
+-rw-rw----   0 rl222169 (222169) dm2s-user-cat-a (470572)      232 2023-05-04 08:26:00.000000 venv-modulefile-0.0.8/src/venvmod/__init__.py
+-rw-rw----   0 rl222169 (222169) dm2s-user-cat-a (470572)     2840 2023-05-04 10:36:26.000000 venv-modulefile-0.0.8/src/venvmod/tools.py
+drwxrwx---   0 rl222169 (222169) dm2s-user-cat-a (470572)        0 2023-05-05 07:36:30.000000 venv-modulefile-0.0.8/src/venvmod/commands/
+-rw-rw----   0 rl222169 (222169) dm2s-user-cat-a (470572)     1539 2023-05-04 09:25:04.000000 venv-modulefile-0.0.8/src/venvmod/commands/test_imports.py
+-rw-rw----   0 rl222169 (222169) dm2s-user-cat-a (470572)     2098 2023-05-04 09:28:22.000000 venv-modulefile-0.0.8/src/venvmod/commands/__init__.py
+-rw-rw----   0 rl222169 (222169) dm2s-user-cat-a (470572)     3897 2023-05-04 10:38:57.000000 venv-modulefile-0.0.8/src/venvmod/commands/create_module.py
+-rw-rw----   0 rl222169 (222169) dm2s-user-cat-a (470572)     8304 2023-05-04 10:38:37.000000 venv-modulefile-0.0.8/src/venvmod/commands/append_module.py
+-rw-rw----   0 rl222169 (222169) dm2s-user-cat-a (470572)    12262 2023-05-04 09:42:38.000000 venv-modulefile-0.0.8/src/venvmod/modulefile.py
+-rw-rw----   0 rl222169 (222169) dm2s-user-cat-a (470572)      898 2023-05-04 08:19:39.000000 venv-modulefile-0.0.8/src/README.md
+drwxrwx---   0 rl222169 (222169) dm2s-user-cat-a (470572)        0 2023-05-05 07:36:30.000000 venv-modulefile-0.0.8/src/venv_modulefile.egg-info/
+-rw-rw----   0 rl222169 (222169) dm2s-user-cat-a (470572)      809 2023-05-05 07:36:30.000000 venv-modulefile-0.0.8/src/venv_modulefile.egg-info/entry_points.txt
+-rw-rw----   0 rl222169 (222169) dm2s-user-cat-a (470572)        8 2023-05-05 07:36:30.000000 venv-modulefile-0.0.8/src/venv_modulefile.egg-info/top_level.txt
+-rw-rw----   0 rl222169 (222169) dm2s-user-cat-a (470572)      567 2023-05-05 07:36:30.000000 venv-modulefile-0.0.8/src/venv_modulefile.egg-info/SOURCES.txt
+-rw-rw----   0 rl222169 (222169) dm2s-user-cat-a (470572)     2042 2023-05-05 07:36:30.000000 venv-modulefile-0.0.8/src/venv_modulefile.egg-info/PKG-INFO
+-rw-rw----   0 rl222169 (222169) dm2s-user-cat-a (470572)        1 2023-05-05 07:36:30.000000 venv-modulefile-0.0.8/src/venv_modulefile.egg-info/dependency_links.txt
+-rw-rw----   0 rl222169 (222169) dm2s-user-cat-a (470572)      229 2023-05-05 07:36:30.000000 venv-modulefile-0.0.8/src/venv_modulefile.egg-info/requires.txt
+-rw-rw----   0 rl222169 (222169) dm2s-user-cat-a (470572)     1302 2023-05-04 08:19:39.000000 venv-modulefile-0.0.8/LICENSE.md
```

### Comparing `venv-modulefile-0.0.2/README.md` & `venv-modulefile-0.0.8/README.md`

 * *Files 23% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 # venv-modulefile
 
 [<img src="https://www.python.org/static/community_logos/python-logo-master-v3-TM.png" height="30"/>](Python)
 [<img src="https://raw.githubusercontent.com/cea-hpc/modules/v5.2.0/doc/img/modules_red.svg" height="30" style="background-color: white"/>](Environment_Module)
 
-- [Venvironment Modules](#venvironment-modules)
+- [venv-modulefile](#venv-modulefile)
   - [Description](#description)
   - [Quick start](#quick-start)
 
-
 ## Description
 
 Tool to create Python complient environment from non-pythonic tools in a Python virtual
 environment.
 
 It is based on [Environment Module](https://modules.readthedocs.io/en/latest/) to
 modify the virtual environment.
```

### Comparing `venv-modulefile-0.0.2/setup.py` & `venv-modulefile-0.0.8/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -192,11 +192,11 @@
     #
     # Examples listed include a pattern for specifying where the package tracks
     # issues, where the source is hosted, where to say thanks to the package
     # maintainers, and where to support the project financially. The key is
     # what's used to render the link text on PyPI.
     project_urls={  # Optional
         "Bug Reports": "https://github.com/roland-lenain/venv-modulefile/issues",
-        "Doc": "https://icoco-python.readthedocs.io/en/latest/index.html",
+        "Doc": "https://venv-modulefile.readthedocs.io/en/latest/index.html",
         "Source": "https://github.com/roland-lenain/venv-modulefile",
     },
 )
```

### Comparing `venv-modulefile-0.0.2/src/venvmod/tools.py` & `venv-modulefile-0.0.8/src/venvmod/tools.py`

 * *Files 18% similar despite different names*

```diff
@@ -8,35 +8,99 @@
 from typing import List
 
 from . import __name__ as PACKAGE_NAME
 
 logger = logging.getLogger(__name__)
 
 def check_raise(condition: bool, exception_type: Exception, message: str):
+    """Chack if a condition is True to raise
+
+    Parameters
+    ----------
+    condition : bool
+        Condition to be True to raise
+    exception_type : Exception
+        Exception to raise
+    message : str
+        Message for the exception
+
+    Raises
+    ------
+    exception_type
+        _description_
+    """
     if condition:
         logger.error(message)
         raise exception_type(message)
 
 
-def get_shell_name_command():
+def get_shell_name_command() -> str:
+    """Gets command to get shell name..
+
+    Returns
+    -------
+    str
+        Command as str.
+    """
     return '"import os; print(os.path.basename(os.readlink(os.path.join(os.sep, \'proc\', str(os.getppid()), \'exe\'))))"'
     # return '"import os; print(os.path.basename(os.environ[\'SHELL\']))"'
 
-def get_shell_name():
+def get_shell_name() -> str:
+    """Gets current shell name.
+
+    Returns
+    -------
+    str
+        shell name
+    """
     return os.path.basename(os.environ["SHELL"])
     return os.path.basename(os.readlink(os.path.join(os.sep, "proc", str(os.getppid()), "exe")))
 
 
 def get_process_result(command: str, capture_output: bool, cwd: str or Path = None) -> CompletedProcess:
+    """Run procces and get results
+
+    Parameters
+    ----------
+    command : str
+        command to run
+    capture_output : bool
+        True to capture output
+    cwd : str or Path, optional
+        execution directory, by default None
+
+    Returns
+    -------
+    CompletedProcess
+        Process result
+    """
 
     pipe = PIPE if capture_output else None
     return _run_process([get_shell_name(), '-c', command], stderr=pipe, stdout=pipe, cwd=cwd)
 
 
 def run_process(command: str, verbose: bool, do_raise: bool, cwd: str or Path = None) -> int:
+    """Run process
+
+    Parameters
+    ----------
+    command : str
+        command to run
+    verbose : bool
+        to enable verbosity
+    do_raise : bool
+        If True, raise if fails
+    cwd : str or Path, optional
+        execution directory, by default None
+
+    Returns
+    -------
+    int
+        return code
+    """
 
     result = get_process_result(command=command, capture_output=not verbose, cwd=cwd)
     if do_raise:
         result.check_returncode
 
     return result.returncode
```

### Comparing `venv-modulefile-0.0.2/src/venvmod/commands/__init__.py` & `venv-modulefile-0.0.8/src/venvmod/commands/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -5,14 +5,34 @@
 from ..modulefile import get_module_file_directory
 
 def get_parser(description: str,
                help_arguments: str = None,
                with_appli: bool = False,
                with_verbose: bool = False,
                args: List = None) -> argparse.Namespace:
+    """Create a parser for entry-points.
+
+    Parameters
+    ----------
+    description : str
+        Description of the command
+    help_arguments : str, optional
+        Help for the arguments, by default None
+    with_appli : bool, optional
+        True to enable '--appli' option, by default False
+    with_verbose : bool, optional
+        True to enable '--verbise' option, by default False
+    args : List, optional
+        list of arguments if not given throug cli, by default None
+
+    Returns
+    -------
+    argparse.Namespace
+        parsed arguments
+    """
 
     parser = argparse.ArgumentParser(description=description)
 
     parser.add_argument("virtual_env",
                         help="Path to the virtual env to modify")
     if with_verbose:
         parser.add_argument('--verbose', action='store_true', help='To display the result.')
@@ -22,11 +42,25 @@
                         help='Name of the appli modulefile (case insensitive)')
     if help_arguments:
         parser.add_argument('arguments', nargs='+', default=[], help=help_arguments)
 
     return parser.parse_args(args)
 
 def get_module_filename(virtual_env_name: str, appli_name: str = None) -> str:
+    """_summary_
+
+    Parameters
+    ----------
+    virtual_env_name : str
+        name or path to the virtual env
+    appli_name : str, optional
+        name of the application, by default None
+
+    Returns
+    -------
+    str
+        name of the module file associated to the appli
+    """
     virtual_env = Path(virtual_env_name).absolute()
     name = (appli_name if appli_name else virtual_env.name).lower()
     virtual_env = virtual_env / get_module_file_directory(virtual_env)
     return str(virtual_env / name)
```

### Comparing `venv-modulefile-0.0.2/src/venvmod/modulefile.py` & `venv-modulefile-0.0.8/src/venvmod/modulefile.py`

 * *Files 6% similar despite different names*

```diff
@@ -10,30 +10,70 @@
 
 import requests
 
 from .tools import (get_process_result, run_process, check_raise,
                     get_shell_name, get_shell_name_command, PACKAGE_NAME, logger)
 
 def get_module_file_directory(venv_name: str or Path) -> Path:
+    """Gets the modulefile directory
+
+    Parameters
+    ----------
+    venv_name : str or Path
+        Path to virtual env
+
+    Returns
+    -------
+    Path
+        Path prepend by venv_name
+    """
     return Path(venv_name) / "etc" / "modulefiles"
 
 def add_command(filename: Path, line: str):
+    """Appends a command to a modulefile
+
+    Parameters
+    ----------
+    filename : Path
+        File to modify
+    line : str
+        Line to append
+    """
     with open(filename, mode='a', encoding='utf-8') as modulefile:
         modulefile.write(line + "\n")
 
 
 def get_version() -> str:
+    """Gets modulefile version
+
+    Returns
+    -------
+    str
+        version as 'x.y.z', '0.0.0' if not found
+    """
     result = get_process_result(command="module --version", capture_output=True)
     if 'VERSION=' in result.stderr.decode().split()[0]: # version < 4.0
         return result.stderr.decode().split()[0].split("=")[1]
     if 'Modules' == result.stderr.decode().split()[0]:
         return result.stderr.decode().split()[2]
     return "0.0.0"
 
-def get_version_list(index: int = 0) -> List[int]:
+def get_version_list(index: int = 0) -> List[int] or int:
+    """Gets version as list
+
+    Parameters
+    ----------
+    index : int, optional
+        index in version, by default 0
+
+    Returns
+    -------
+    List[int] or int
+        version numbers or version number if index > 0
+    """
     version = get_version()
     version = [int(id) for id in version.split(".")]
     return version[index-1] if index else version
 
 
 class ModuleInstaller:
     """Class to install Environment Module.
@@ -44,15 +84,29 @@
                  install_prefix: str or Path,
                  cache_directory: str or Path) -> None:
 
         self._version_or_path: str = version_or_path
         self._install_prefix: Path = Path(install_prefix)
         self._cache_directory: Path = Path(cache_directory)
 
-    def run(self, verbose: bool = False, do_raise: bool = True):
+    def run(self, verbose: bool = False, do_raise: bool = True) -> int:
+        """run installer
+
+        Parameters
+        ----------
+        verbose : bool, optional
+            True to enable verbosity, by default False
+        do_raise : bool, optional
+            True to raise if fails, by default True
+
+        Returns
+        -------
+        int
+            return code
+        """
 
         self._cache_directory.mkdir(parents=True, exist_ok=True)
         if Path(self._version_or_path).exists():
             src_directory = Path(self._version_or_path)
             build_directory = self._cache_directory / src_directory.name
         else:
             check_raise(condition=version.parse(self._version_or_path) < version.parse("4.6"),
@@ -85,15 +139,29 @@
             return code
 
         return run_process(command="make clean && make && make install",
                            verbose=verbose,
                            cwd=build_directory,
                            do_raise=do_raise)
 
-def upgrade_modulefile(virtual_env: Path, module_prefix: Path):
+def upgrade_modulefile(virtual_env: Path, module_prefix: Path) -> int:
+    """Upgrade modulefile in venv
+
+    Parameters
+    ----------
+    virtual_env : Path
+        Path to virtual env
+    module_prefix : Path
+        Modulefile install prefix
+
+    Returns
+    -------
+    int
+        return code
+    """
 
     activate_src = virtual_env / "bin" / "activate"
     check_raise(not activate_src.is_file(), AssertionError,
                 f'"activate" file {activate_src} not found.')
 
     with open(activate_src, "r") as src_file:
         src_lines = src_file.readlines()
```

### Comparing `venv-modulefile-0.0.2/src/venv_modulefile.egg-info/entry_points.txt` & `venv-modulefile-0.0.8/src/venv_modulefile.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `venv-modulefile-0.0.2/src/venv_modulefile.egg-info/SOURCES.txt` & `venv-modulefile-0.0.8/src/venv_modulefile.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `venv-modulefile-0.0.2/LICENSE.md` & `venv-modulefile-0.0.8/LICENSE.md`

 * *Files identical despite different names*

