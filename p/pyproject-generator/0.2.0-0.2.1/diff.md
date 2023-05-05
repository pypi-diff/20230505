# Comparing `tmp/pyproject-generator-0.2.0.tar.gz` & `tmp/pyproject-generator-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyproject-generator-0.2.0.tar", last modified: Fri May  5 04:32:49 2023, max compression
+gzip compressed data, was "pyproject-generator-0.2.1.tar", last modified: Fri May  5 12:42:47 2023, max compression
```

## Comparing `pyproject-generator-0.2.0.tar` & `pyproject-generator-0.2.1.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxr-xr-x   0 cangyuanli   (501) staff       (20)        0 2023-05-05 04:32:49.585652 pyproject-generator-0.2.0/
--rw-r--r--   0 cangyuanli   (501) staff       (20)     1078 2023-05-04 01:48:13.000000 pyproject-generator-0.2.0/LICENSE
--rw-r--r--   0 cangyuanli   (501) staff       (20)     3871 2023-05-05 04:32:49.585873 pyproject-generator-0.2.0/PKG-INFO
--rw-r--r--   0 cangyuanli   (501) staff       (20)     3330 2023-05-05 02:42:29.000000 pyproject-generator-0.2.0/README.md
--rw-r--r--   0 cangyuanli   (501) staff       (20)      264 2023-05-05 02:42:29.000000 pyproject-generator-0.2.0/pyproject.toml
--rw-r--r--   0 cangyuanli   (501) staff       (20)      868 2023-05-05 04:32:49.586674 pyproject-generator-0.2.0/setup.cfg
-drwxr-xr-x   0 cangyuanli   (501) staff       (20)        0 2023-05-05 04:32:49.565105 pyproject-generator-0.2.0/src/
-drwxr-xr-x   0 cangyuanli   (501) staff       (20)        0 2023-05-05 04:32:49.573691 pyproject-generator-0.2.0/src/pyproject/
--rw-r--r--   0 cangyuanli   (501) staff       (20)       51 2023-05-05 02:42:30.000000 pyproject-generator-0.2.0/src/pyproject/__init__.py
--rw-r--r--   0 cangyuanli   (501) staff       (20)       22 2023-05-05 04:32:39.000000 pyproject-generator-0.2.0/src/pyproject/__version__.py
--rw-r--r--   0 cangyuanli   (501) staff       (20)     3991 2023-05-05 02:42:30.000000 pyproject-generator-0.2.0/src/pyproject/cli.py
-drwxr-xr-x   0 cangyuanli   (501) staff       (20)        0 2023-05-05 04:32:49.574339 pyproject-generator-0.2.0/src/pyproject/config/
--rw-r--r--   0 cangyuanli   (501) staff       (20)      315 2023-05-05 03:34:04.000000 pyproject-generator-0.2.0/src/pyproject/config/default_config.json
--rw-r--r--   0 cangyuanli   (501) staff       (20)     1029 2023-05-05 02:42:30.000000 pyproject-generator-0.2.0/src/pyproject/licenses.py
--rw-r--r--   0 cangyuanli   (501) staff       (20)     1729 2023-05-05 02:42:30.000000 pyproject-generator-0.2.0/src/pyproject/logger.py
--rw-r--r--   0 cangyuanli   (501) staff       (20)    15536 2023-05-05 04:31:05.000000 pyproject-generator-0.2.0/src/pyproject/project_builder.py
--rw-r--r--   0 cangyuanli   (501) staff       (20)     2753 2023-05-05 02:42:30.000000 pyproject-generator-0.2.0/src/pyproject/spinner.py
-drwxr-xr-x   0 cangyuanli   (501) staff       (20)        0 2023-05-05 04:32:49.580705 pyproject-generator-0.2.0/src/pyproject/templates/
--rw-r--r--   0 cangyuanli   (501) staff       (20)     1498 2023-05-03 19:23:49.000000 pyproject-generator-0.2.0/src/pyproject/templates/gitignore.template
--rw-r--r--   0 cangyuanli   (501) staff       (20)      548 2023-04-30 01:20:52.000000 pyproject-generator-0.2.0/src/pyproject/templates/license_apache.template
--rw-r--r--   0 cangyuanli   (501) staff       (20)     1457 2023-05-04 13:35:45.000000 pyproject-generator-0.2.0/src/pyproject/templates/license_bsd3.template
--rw-r--r--   0 cangyuanli   (501) staff       (20)        0 2023-04-30 15:11:38.000000 pyproject-generator-0.2.0/src/pyproject/templates/license_gpl_v3.template
--rw-r--r--   0 cangyuanli   (501) staff       (20)     1074 2023-04-30 01:18:24.000000 pyproject-generator-0.2.0/src/pyproject/templates/license_mit.template
--rw-r--r--   0 cangyuanli   (501) staff       (20)      905 2023-05-03 23:48:11.000000 pyproject-generator-0.2.0/src/pyproject/templates/pre_commit_config.template
--rw-r--r--   0 cangyuanli   (501) staff       (20)      263 2023-05-04 02:15:39.000000 pyproject-generator-0.2.0/src/pyproject/templates/pyproject.template
--rw-r--r--   0 cangyuanli   (501) staff       (20)     1040 2023-05-04 20:10:03.000000 pyproject-generator-0.2.0/src/pyproject/templates/readme.template
--rw-r--r--   0 cangyuanli   (501) staff       (20)      583 2023-04-30 15:11:46.000000 pyproject-generator-0.2.0/src/pyproject/templates/setup.template
--rw-r--r--   0 cangyuanli   (501) staff       (20)      649 2023-04-13 18:27:11.000000 pyproject-generator-0.2.0/src/pyproject/templates/tests.template
--rw-r--r--   0 cangyuanli   (501) staff       (20)      402 2023-04-12 23:45:24.000000 pyproject-generator-0.2.0/src/pyproject/templates/tox.template
-drwxr-xr-x   0 cangyuanli   (501) staff       (20)        0 2023-05-05 04:32:49.584796 pyproject-generator-0.2.0/src/pyproject_generator.egg-info/
--rw-r--r--   0 cangyuanli   (501) staff       (20)     3871 2023-05-05 04:32:49.000000 pyproject-generator-0.2.0/src/pyproject_generator.egg-info/PKG-INFO
--rw-r--r--   0 cangyuanli   (501) staff       (20)     1054 2023-05-05 04:32:49.000000 pyproject-generator-0.2.0/src/pyproject_generator.egg-info/SOURCES.txt
--rw-r--r--   0 cangyuanli   (501) staff       (20)        1 2023-05-05 04:32:49.000000 pyproject-generator-0.2.0/src/pyproject_generator.egg-info/dependency_links.txt
--rw-r--r--   0 cangyuanli   (501) staff       (20)       49 2023-05-05 04:32:49.000000 pyproject-generator-0.2.0/src/pyproject_generator.egg-info/entry_points.txt
--rw-r--r--   0 cangyuanli   (501) staff       (20)       13 2023-05-05 04:32:49.000000 pyproject-generator-0.2.0/src/pyproject_generator.egg-info/requires.txt
--rw-r--r--   0 cangyuanli   (501) staff       (20)       10 2023-05-05 04:32:49.000000 pyproject-generator-0.2.0/src/pyproject_generator.egg-info/top_level.txt
-drwxr-xr-x   0 cangyuanli   (501) staff       (20)        0 2023-05-05 04:32:49.585332 pyproject-generator-0.2.0/tests/
--rw-r--r--   0 cangyuanli   (501) staff       (20)        0 2023-05-05 02:42:30.000000 pyproject-generator-0.2.0/tests/test_pyproject.py
+drwxr-xr-x   0 cangyuanli   (501) staff       (20)        0 2023-05-05 12:42:47.266066 pyproject-generator-0.2.1/
+-rw-r--r--   0 cangyuanli   (501) staff       (20)     1078 2023-05-04 01:48:13.000000 pyproject-generator-0.2.1/LICENSE
+-rw-r--r--   0 cangyuanli   (501) staff       (20)     3871 2023-05-05 12:42:47.266288 pyproject-generator-0.2.1/PKG-INFO
+-rw-r--r--   0 cangyuanli   (501) staff       (20)     3330 2023-05-05 02:42:29.000000 pyproject-generator-0.2.1/README.md
+-rw-r--r--   0 cangyuanli   (501) staff       (20)      264 2023-05-05 02:42:29.000000 pyproject-generator-0.2.1/pyproject.toml
+-rw-r--r--   0 cangyuanli   (501) staff       (20)      868 2023-05-05 12:42:47.267219 pyproject-generator-0.2.1/setup.cfg
+drwxr-xr-x   0 cangyuanli   (501) staff       (20)        0 2023-05-05 12:42:47.237201 pyproject-generator-0.2.1/src/
+drwxr-xr-x   0 cangyuanli   (501) staff       (20)        0 2023-05-05 12:42:47.246336 pyproject-generator-0.2.1/src/pyproject/
+-rw-r--r--   0 cangyuanli   (501) staff       (20)       51 2023-05-05 02:42:30.000000 pyproject-generator-0.2.1/src/pyproject/__init__.py
+-rw-r--r--   0 cangyuanli   (501) staff       (20)       22 2023-05-05 12:42:33.000000 pyproject-generator-0.2.1/src/pyproject/__version__.py
+-rw-r--r--   0 cangyuanli   (501) staff       (20)     3991 2023-05-05 02:42:30.000000 pyproject-generator-0.2.1/src/pyproject/cli.py
+drwxr-xr-x   0 cangyuanli   (501) staff       (20)        0 2023-05-05 12:42:47.247036 pyproject-generator-0.2.1/src/pyproject/config/
+-rw-r--r--   0 cangyuanli   (501) staff       (20)      315 2023-05-05 03:34:04.000000 pyproject-generator-0.2.1/src/pyproject/config/default_config.json
+-rw-r--r--   0 cangyuanli   (501) staff       (20)     1029 2023-05-05 02:42:30.000000 pyproject-generator-0.2.1/src/pyproject/licenses.py
+-rw-r--r--   0 cangyuanli   (501) staff       (20)     1727 2023-05-05 12:40:42.000000 pyproject-generator-0.2.1/src/pyproject/logger.py
+-rw-r--r--   0 cangyuanli   (501) staff       (20)    15133 2023-05-05 12:41:28.000000 pyproject-generator-0.2.1/src/pyproject/project_builder.py
+-rw-r--r--   0 cangyuanli   (501) staff       (20)     2753 2023-05-05 02:42:30.000000 pyproject-generator-0.2.1/src/pyproject/spinner.py
+drwxr-xr-x   0 cangyuanli   (501) staff       (20)        0 2023-05-05 12:42:47.258769 pyproject-generator-0.2.1/src/pyproject/templates/
+-rw-r--r--   0 cangyuanli   (501) staff       (20)     1498 2023-05-03 19:23:49.000000 pyproject-generator-0.2.1/src/pyproject/templates/gitignore.template
+-rw-r--r--   0 cangyuanli   (501) staff       (20)      548 2023-04-30 01:20:52.000000 pyproject-generator-0.2.1/src/pyproject/templates/license_apache.template
+-rw-r--r--   0 cangyuanli   (501) staff       (20)     1457 2023-05-04 13:35:45.000000 pyproject-generator-0.2.1/src/pyproject/templates/license_bsd3.template
+-rw-r--r--   0 cangyuanli   (501) staff       (20)        0 2023-04-30 15:11:38.000000 pyproject-generator-0.2.1/src/pyproject/templates/license_gpl_v3.template
+-rw-r--r--   0 cangyuanli   (501) staff       (20)     1074 2023-04-30 01:18:24.000000 pyproject-generator-0.2.1/src/pyproject/templates/license_mit.template
+-rw-r--r--   0 cangyuanli   (501) staff       (20)      905 2023-05-03 23:48:11.000000 pyproject-generator-0.2.1/src/pyproject/templates/pre_commit_config.template
+-rw-r--r--   0 cangyuanli   (501) staff       (20)      263 2023-05-04 02:15:39.000000 pyproject-generator-0.2.1/src/pyproject/templates/pyproject.template
+-rw-r--r--   0 cangyuanli   (501) staff       (20)     1040 2023-05-04 20:10:03.000000 pyproject-generator-0.2.1/src/pyproject/templates/readme.template
+-rw-r--r--   0 cangyuanli   (501) staff       (20)      583 2023-04-30 15:11:46.000000 pyproject-generator-0.2.1/src/pyproject/templates/setup.template
+-rw-r--r--   0 cangyuanli   (501) staff       (20)      649 2023-04-13 18:27:11.000000 pyproject-generator-0.2.1/src/pyproject/templates/tests.template
+-rw-r--r--   0 cangyuanli   (501) staff       (20)      402 2023-04-12 23:45:24.000000 pyproject-generator-0.2.1/src/pyproject/templates/tox.template
+drwxr-xr-x   0 cangyuanli   (501) staff       (20)        0 2023-05-05 12:42:47.265030 pyproject-generator-0.2.1/src/pyproject_generator.egg-info/
+-rw-r--r--   0 cangyuanli   (501) staff       (20)     3871 2023-05-05 12:42:47.000000 pyproject-generator-0.2.1/src/pyproject_generator.egg-info/PKG-INFO
+-rw-r--r--   0 cangyuanli   (501) staff       (20)     1054 2023-05-05 12:42:47.000000 pyproject-generator-0.2.1/src/pyproject_generator.egg-info/SOURCES.txt
+-rw-r--r--   0 cangyuanli   (501) staff       (20)        1 2023-05-05 12:42:47.000000 pyproject-generator-0.2.1/src/pyproject_generator.egg-info/dependency_links.txt
+-rw-r--r--   0 cangyuanli   (501) staff       (20)       49 2023-05-05 12:42:47.000000 pyproject-generator-0.2.1/src/pyproject_generator.egg-info/entry_points.txt
+-rw-r--r--   0 cangyuanli   (501) staff       (20)       13 2023-05-05 12:42:47.000000 pyproject-generator-0.2.1/src/pyproject_generator.egg-info/requires.txt
+-rw-r--r--   0 cangyuanli   (501) staff       (20)       10 2023-05-05 12:42:47.000000 pyproject-generator-0.2.1/src/pyproject_generator.egg-info/top_level.txt
+drwxr-xr-x   0 cangyuanli   (501) staff       (20)        0 2023-05-05 12:42:47.265615 pyproject-generator-0.2.1/tests/
+-rw-r--r--   0 cangyuanli   (501) staff       (20)        0 2023-05-05 02:42:30.000000 pyproject-generator-0.2.1/tests/test_pyproject.py
```

### Comparing `pyproject-generator-0.2.0/LICENSE` & `pyproject-generator-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pyproject-generator-0.2.0/PKG-INFO` & `pyproject-generator-0.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyproject-generator
-Version: 0.2.0
+Version: 0.2.1
 Summary: A command line tool to setup Python packages
 Home-page: https://github.com/CangyuanLi/pyproject
 Author: Cangyuan Li
 Author-email: everest229@gmail.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/CangyuanLi/pyproject/issues
 Classifier: Programming Language :: Python :: 3
```

### Comparing `pyproject-generator-0.2.0/README.md` & `pyproject-generator-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `pyproject-generator-0.2.0/setup.cfg` & `pyproject-generator-0.2.1/setup.cfg`

 * *Files identical despite different names*

### Comparing `pyproject-generator-0.2.0/src/pyproject/cli.py` & `pyproject-generator-0.2.1/src/pyproject/cli.py`

 * *Files identical despite different names*

### Comparing `pyproject-generator-0.2.0/src/pyproject/licenses.py` & `pyproject-generator-0.2.1/src/pyproject/licenses.py`

 * *Files identical despite different names*

### Comparing `pyproject-generator-0.2.0/src/pyproject/logger.py` & `pyproject-generator-0.2.1/src/pyproject/logger.py`

 * *Files 14% similar despite different names*

```diff
@@ -54,16 +54,16 @@
     def spinner(
         self,
         func: Callable,
         text: str,
         delay: float = 0.1,
         prefix: str = "    ",
         suffix: str = " ",
-        clear: bool = False,
-        min_show_duration: Optional[float] = None,
+        clear: bool = True,
+        min_show_duration: Optional[float] = 0.2,
     ):
         if Level.INFO > self._level:
             return func()
 
         with Spinner(
             self._console, text, delay, prefix, suffix, clear, min_show_duration
         ):
```

### Comparing `pyproject-generator-0.2.0/src/pyproject/project_builder.py` & `pyproject-generator-0.2.1/src/pyproject/project_builder.py`

 * *Files 9% similar despite different names*

```diff
@@ -288,64 +288,50 @@
 
         self._logger.info(Panel("Creating project files..."), justify="left")
 
         # Fill in templates
         templates = self._logger.spinner(
             lambda: self._fill_in_templates(project_name),
             "Filling in templates",
-            clear=True,
-            min_show_duration=0.2,
         )
 
         # initialize git repo
         self._logger.spinner(
             lambda: self._init_git(proj_path),
             "Initializing git repository",
-            clear=True,
-            min_show_duration=0.2,
         )
 
         # src
         self._logger.spinner(
             lambda: self._init_source_directory(proj_path, project_name),
             "Creating source directory",
-            clear=True,
-            min_show_duration=0.2,
         )
 
         # tests
         self._logger.spinner(
             lambda: self._init_tests(proj_path, project_name),
             "Creating tests",
-            clear=True,
-            min_show_duration=0.2,
         )
 
         # benchmarks
         self._logger.spinner(
             lambda: self._init_benchmarks(proj_path),
             "Creating benchmarks",
-            clear=True,
-            min_show_duration=0.2,
         )
 
         # github actions
         self._logger.spinner(
             lambda: self._init_github_actions(proj_path, templates),
             "Setting up Github Actions",
-            clear=True,
-            min_show_duration=0.2,
         )
 
         # misc setup
         self._logger.spinner(
             lambda: self._init_config_files(proj_path, templates),
             "Setting up configuration files",
-            clear=True,
-            min_show_duration=0.2,
         )
 
         self._logger.info("Building project skeleton completed with no errors.")
 
         # Setup the virtual environment
         self._logger.info(
             Panel("Setting up the virtual environment..."), justify="left"
@@ -358,42 +344,42 @@
 
         self._logger.spinner(
             lambda: venv_builder.run_bin(
                 ["python", "-m", "pip", "install", "-U", "pip"],
                 stdout=subprocess.DEVNULL,
             ),
             text="pip",
+            clear=False,
         )
 
         for dep in sorted(list(self._config.dependencies)):
             self._logger.spinner(
                 lambda: venv_builder.run_bin(
                     ["pip", "install", dep], stdout=subprocess.DEVNULL
                 ),
                 text=dep,
+                clear=False,
             )
 
         self._logger.info(Panel("Finalizing project..."), justify="left")
 
         # Create requirements_dev file
         def _create_req_file():
             reqs = venv_builder.run_bin(["pip", "freeze"], capture_output=True)
             (proj_path / "requirements_dev.txt").write_bytes(reqs.stdout)
 
         self._logger.spinner(
             _create_req_file,
             "Creating requirements_dev.txt",
-            clear=True,
-            min_show_duration=0.2,
         )
 
         # Ensure pre-commit is up to date
         self._logger.spinner(
             lambda: venv_builder.run_bin(
-                ["pre-commit", "autoupdate"], stdout=subprocess.DEVNULL
+                ["pre-commit", "autoupdate"], cwd=proj_path, stdout=subprocess.DEVNULL
             ),
             "Ensuring pre-commit config is up to date",
             clear=True,
         )
 
         self._logger.info(f"Done setting up {project_name}!", style="green")
```

### Comparing `pyproject-generator-0.2.0/src/pyproject/spinner.py` & `pyproject-generator-0.2.1/src/pyproject/spinner.py`

 * *Files identical despite different names*

### Comparing `pyproject-generator-0.2.0/src/pyproject/templates/gitignore.template` & `pyproject-generator-0.2.1/src/pyproject/templates/gitignore.template`

 * *Files identical despite different names*

### Comparing `pyproject-generator-0.2.0/src/pyproject/templates/license_apache.template` & `pyproject-generator-0.2.1/src/pyproject/templates/license_apache.template`

 * *Files identical despite different names*

### Comparing `pyproject-generator-0.2.0/src/pyproject/templates/license_bsd3.template` & `pyproject-generator-0.2.1/src/pyproject/templates/license_bsd3.template`

 * *Files identical despite different names*

### Comparing `pyproject-generator-0.2.0/src/pyproject/templates/license_mit.template` & `pyproject-generator-0.2.1/src/pyproject/templates/license_mit.template`

 * *Files identical despite different names*

### Comparing `pyproject-generator-0.2.0/src/pyproject/templates/pre_commit_config.template` & `pyproject-generator-0.2.1/src/pyproject/templates/pre_commit_config.template`

 * *Files identical despite different names*

### Comparing `pyproject-generator-0.2.0/src/pyproject/templates/readme.template` & `pyproject-generator-0.2.1/src/pyproject/templates/readme.template`

 * *Files identical despite different names*

### Comparing `pyproject-generator-0.2.0/src/pyproject/templates/setup.template` & `pyproject-generator-0.2.1/src/pyproject/templates/setup.template`

 * *Files identical despite different names*

### Comparing `pyproject-generator-0.2.0/src/pyproject/templates/tests.template` & `pyproject-generator-0.2.1/src/pyproject/templates/tests.template`

 * *Files identical despite different names*

### Comparing `pyproject-generator-0.2.0/src/pyproject_generator.egg-info/PKG-INFO` & `pyproject-generator-0.2.1/src/pyproject_generator.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyproject-generator
-Version: 0.2.0
+Version: 0.2.1
 Summary: A command line tool to setup Python packages
 Home-page: https://github.com/CangyuanLi/pyproject
 Author: Cangyuan Li
 Author-email: everest229@gmail.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/CangyuanLi/pyproject/issues
 Classifier: Programming Language :: Python :: 3
```

### Comparing `pyproject-generator-0.2.0/src/pyproject_generator.egg-info/SOURCES.txt` & `pyproject-generator-0.2.1/src/pyproject_generator.egg-info/SOURCES.txt`

 * *Files identical despite different names*

