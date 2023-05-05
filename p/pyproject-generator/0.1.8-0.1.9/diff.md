# Comparing `tmp/pyproject-generator-0.1.8.tar.gz` & `tmp/pyproject-generator-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyproject-generator-0.1.8.tar", last modified: Fri May  5 03:34:52 2023, max compression
+gzip compressed data, was "pyproject-generator-0.1.9.tar", last modified: Fri May  5 04:26:47 2023, max compression
```

## Comparing `pyproject-generator-0.1.8.tar` & `pyproject-generator-0.1.9.tar`

### file list

```diff
@@ -1,39 +1,38 @@
-drwxr-xr-x   0 cangyuanli   (501) staff       (20)        0 2023-05-05 03:34:52.685142 pyproject-generator-0.1.8/
--rw-r--r--   0 cangyuanli   (501) staff       (20)     1078 2023-05-04 01:48:13.000000 pyproject-generator-0.1.8/LICENSE
--rw-r--r--   0 cangyuanli   (501) staff       (20)     3871 2023-05-05 03:34:52.685416 pyproject-generator-0.1.8/PKG-INFO
--rw-r--r--   0 cangyuanli   (501) staff       (20)     3330 2023-05-05 02:42:29.000000 pyproject-generator-0.1.8/README.md
--rw-r--r--   0 cangyuanli   (501) staff       (20)      264 2023-05-05 02:42:29.000000 pyproject-generator-0.1.8/pyproject.toml
--rw-r--r--   0 cangyuanli   (501) staff       (20)      868 2023-05-05 03:34:52.686684 pyproject-generator-0.1.8/setup.cfg
-drwxr-xr-x   0 cangyuanli   (501) staff       (20)        0 2023-05-05 03:34:52.655619 pyproject-generator-0.1.8/src/
-drwxr-xr-x   0 cangyuanli   (501) staff       (20)        0 2023-05-05 03:34:52.665422 pyproject-generator-0.1.8/src/pyproject/
--rw-r--r--   0 cangyuanli   (501) staff       (20)       51 2023-05-05 02:42:30.000000 pyproject-generator-0.1.8/src/pyproject/__init__.py
--rw-r--r--   0 cangyuanli   (501) staff       (20)       22 2023-05-05 03:34:36.000000 pyproject-generator-0.1.8/src/pyproject/__version__.py
--rw-r--r--   0 cangyuanli   (501) staff       (20)     3991 2023-05-05 02:42:30.000000 pyproject-generator-0.1.8/src/pyproject/cli.py
-drwxr-xr-x   0 cangyuanli   (501) staff       (20)        0 2023-05-05 03:34:52.667240 pyproject-generator-0.1.8/src/pyproject/config/
--rw-r--r--   0 cangyuanli   (501) staff       (20)      237 2023-05-05 02:42:30.000000 pyproject-generator-0.1.8/src/pyproject/config/config.json
--rw-r--r--   0 cangyuanli   (501) staff       (20)      315 2023-05-05 03:34:04.000000 pyproject-generator-0.1.8/src/pyproject/config/default_config.json
--rw-r--r--   0 cangyuanli   (501) staff       (20)     1029 2023-05-05 02:42:30.000000 pyproject-generator-0.1.8/src/pyproject/licenses.py
--rw-r--r--   0 cangyuanli   (501) staff       (20)     1729 2023-05-05 02:42:30.000000 pyproject-generator-0.1.8/src/pyproject/logger.py
--rw-r--r--   0 cangyuanli   (501) staff       (20)    15179 2023-05-05 03:32:08.000000 pyproject-generator-0.1.8/src/pyproject/project_builder.py
--rw-r--r--   0 cangyuanli   (501) staff       (20)     2753 2023-05-05 02:42:30.000000 pyproject-generator-0.1.8/src/pyproject/spinner.py
-drwxr-xr-x   0 cangyuanli   (501) staff       (20)        0 2023-05-05 03:34:52.679134 pyproject-generator-0.1.8/src/pyproject/templates/
--rw-r--r--   0 cangyuanli   (501) staff       (20)     1498 2023-05-03 19:23:49.000000 pyproject-generator-0.1.8/src/pyproject/templates/gitignore.template
--rw-r--r--   0 cangyuanli   (501) staff       (20)      548 2023-04-30 01:20:52.000000 pyproject-generator-0.1.8/src/pyproject/templates/license_apache.template
--rw-r--r--   0 cangyuanli   (501) staff       (20)     1457 2023-05-04 13:35:45.000000 pyproject-generator-0.1.8/src/pyproject/templates/license_bsd3.template
--rw-r--r--   0 cangyuanli   (501) staff       (20)        0 2023-04-30 15:11:38.000000 pyproject-generator-0.1.8/src/pyproject/templates/license_gpl_v3.template
--rw-r--r--   0 cangyuanli   (501) staff       (20)     1074 2023-04-30 01:18:24.000000 pyproject-generator-0.1.8/src/pyproject/templates/license_mit.template
--rw-r--r--   0 cangyuanli   (501) staff       (20)      905 2023-05-03 23:48:11.000000 pyproject-generator-0.1.8/src/pyproject/templates/pre_commit_config.template
--rw-r--r--   0 cangyuanli   (501) staff       (20)      263 2023-05-04 02:15:39.000000 pyproject-generator-0.1.8/src/pyproject/templates/pyproject.template
--rw-r--r--   0 cangyuanli   (501) staff       (20)     1040 2023-05-04 20:10:03.000000 pyproject-generator-0.1.8/src/pyproject/templates/readme.template
--rw-r--r--   0 cangyuanli   (501) staff       (20)      583 2023-04-30 15:11:46.000000 pyproject-generator-0.1.8/src/pyproject/templates/setup.template
--rw-r--r--   0 cangyuanli   (501) staff       (20)      649 2023-04-13 18:27:11.000000 pyproject-generator-0.1.8/src/pyproject/templates/tests.template
--rw-r--r--   0 cangyuanli   (501) staff       (20)      402 2023-04-12 23:45:24.000000 pyproject-generator-0.1.8/src/pyproject/templates/tox.template
-drwxr-xr-x   0 cangyuanli   (501) staff       (20)        0 2023-05-05 03:34:52.683868 pyproject-generator-0.1.8/src/pyproject_generator.egg-info/
--rw-r--r--   0 cangyuanli   (501) staff       (20)     3871 2023-05-05 03:34:52.000000 pyproject-generator-0.1.8/src/pyproject_generator.egg-info/PKG-INFO
--rw-r--r--   0 cangyuanli   (501) staff       (20)     1087 2023-05-05 03:34:52.000000 pyproject-generator-0.1.8/src/pyproject_generator.egg-info/SOURCES.txt
--rw-r--r--   0 cangyuanli   (501) staff       (20)        1 2023-05-05 03:34:52.000000 pyproject-generator-0.1.8/src/pyproject_generator.egg-info/dependency_links.txt
--rw-r--r--   0 cangyuanli   (501) staff       (20)       49 2023-05-05 03:34:52.000000 pyproject-generator-0.1.8/src/pyproject_generator.egg-info/entry_points.txt
--rw-r--r--   0 cangyuanli   (501) staff       (20)       13 2023-05-05 03:34:52.000000 pyproject-generator-0.1.8/src/pyproject_generator.egg-info/requires.txt
--rw-r--r--   0 cangyuanli   (501) staff       (20)       10 2023-05-05 03:34:52.000000 pyproject-generator-0.1.8/src/pyproject_generator.egg-info/top_level.txt
-drwxr-xr-x   0 cangyuanli   (501) staff       (20)        0 2023-05-05 03:34:52.684682 pyproject-generator-0.1.8/tests/
--rw-r--r--   0 cangyuanli   (501) staff       (20)        0 2023-05-05 02:42:30.000000 pyproject-generator-0.1.8/tests/test_pyproject.py
+drwxr-xr-x   0 cangyuanli   (501) staff       (20)        0 2023-05-05 04:26:47.859681 pyproject-generator-0.1.9/
+-rw-r--r--   0 cangyuanli   (501) staff       (20)     1078 2023-05-04 01:48:13.000000 pyproject-generator-0.1.9/LICENSE
+-rw-r--r--   0 cangyuanli   (501) staff       (20)     3871 2023-05-05 04:26:47.859983 pyproject-generator-0.1.9/PKG-INFO
+-rw-r--r--   0 cangyuanli   (501) staff       (20)     3330 2023-05-05 02:42:29.000000 pyproject-generator-0.1.9/README.md
+-rw-r--r--   0 cangyuanli   (501) staff       (20)      264 2023-05-05 02:42:29.000000 pyproject-generator-0.1.9/pyproject.toml
+-rw-r--r--   0 cangyuanli   (501) staff       (20)      868 2023-05-05 04:26:47.861633 pyproject-generator-0.1.9/setup.cfg
+drwxr-xr-x   0 cangyuanli   (501) staff       (20)        0 2023-05-05 04:26:47.832239 pyproject-generator-0.1.9/src/
+drwxr-xr-x   0 cangyuanli   (501) staff       (20)        0 2023-05-05 04:26:47.841188 pyproject-generator-0.1.9/src/pyproject/
+-rw-r--r--   0 cangyuanli   (501) staff       (20)       51 2023-05-05 02:42:30.000000 pyproject-generator-0.1.9/src/pyproject/__init__.py
+-rw-r--r--   0 cangyuanli   (501) staff       (20)       22 2023-05-05 04:26:40.000000 pyproject-generator-0.1.9/src/pyproject/__version__.py
+-rw-r--r--   0 cangyuanli   (501) staff       (20)     3991 2023-05-05 02:42:30.000000 pyproject-generator-0.1.9/src/pyproject/cli.py
+drwxr-xr-x   0 cangyuanli   (501) staff       (20)        0 2023-05-05 04:26:47.841980 pyproject-generator-0.1.9/src/pyproject/config/
+-rw-r--r--   0 cangyuanli   (501) staff       (20)      315 2023-05-05 03:34:04.000000 pyproject-generator-0.1.9/src/pyproject/config/default_config.json
+-rw-r--r--   0 cangyuanli   (501) staff       (20)     1029 2023-05-05 02:42:30.000000 pyproject-generator-0.1.9/src/pyproject/licenses.py
+-rw-r--r--   0 cangyuanli   (501) staff       (20)     1729 2023-05-05 02:42:30.000000 pyproject-generator-0.1.9/src/pyproject/logger.py
+-rw-r--r--   0 cangyuanli   (501) staff       (20)    15487 2023-05-05 04:25:49.000000 pyproject-generator-0.1.9/src/pyproject/project_builder.py
+-rw-r--r--   0 cangyuanli   (501) staff       (20)     2753 2023-05-05 02:42:30.000000 pyproject-generator-0.1.9/src/pyproject/spinner.py
+drwxr-xr-x   0 cangyuanli   (501) staff       (20)        0 2023-05-05 04:26:47.852623 pyproject-generator-0.1.9/src/pyproject/templates/
+-rw-r--r--   0 cangyuanli   (501) staff       (20)     1498 2023-05-03 19:23:49.000000 pyproject-generator-0.1.9/src/pyproject/templates/gitignore.template
+-rw-r--r--   0 cangyuanli   (501) staff       (20)      548 2023-04-30 01:20:52.000000 pyproject-generator-0.1.9/src/pyproject/templates/license_apache.template
+-rw-r--r--   0 cangyuanli   (501) staff       (20)     1457 2023-05-04 13:35:45.000000 pyproject-generator-0.1.9/src/pyproject/templates/license_bsd3.template
+-rw-r--r--   0 cangyuanli   (501) staff       (20)        0 2023-04-30 15:11:38.000000 pyproject-generator-0.1.9/src/pyproject/templates/license_gpl_v3.template
+-rw-r--r--   0 cangyuanli   (501) staff       (20)     1074 2023-04-30 01:18:24.000000 pyproject-generator-0.1.9/src/pyproject/templates/license_mit.template
+-rw-r--r--   0 cangyuanli   (501) staff       (20)      905 2023-05-03 23:48:11.000000 pyproject-generator-0.1.9/src/pyproject/templates/pre_commit_config.template
+-rw-r--r--   0 cangyuanli   (501) staff       (20)      263 2023-05-04 02:15:39.000000 pyproject-generator-0.1.9/src/pyproject/templates/pyproject.template
+-rw-r--r--   0 cangyuanli   (501) staff       (20)     1040 2023-05-04 20:10:03.000000 pyproject-generator-0.1.9/src/pyproject/templates/readme.template
+-rw-r--r--   0 cangyuanli   (501) staff       (20)      583 2023-04-30 15:11:46.000000 pyproject-generator-0.1.9/src/pyproject/templates/setup.template
+-rw-r--r--   0 cangyuanli   (501) staff       (20)      649 2023-04-13 18:27:11.000000 pyproject-generator-0.1.9/src/pyproject/templates/tests.template
+-rw-r--r--   0 cangyuanli   (501) staff       (20)      402 2023-04-12 23:45:24.000000 pyproject-generator-0.1.9/src/pyproject/templates/tox.template
+drwxr-xr-x   0 cangyuanli   (501) staff       (20)        0 2023-05-05 04:26:47.858053 pyproject-generator-0.1.9/src/pyproject_generator.egg-info/
+-rw-r--r--   0 cangyuanli   (501) staff       (20)     3871 2023-05-05 04:26:47.000000 pyproject-generator-0.1.9/src/pyproject_generator.egg-info/PKG-INFO
+-rw-r--r--   0 cangyuanli   (501) staff       (20)     1054 2023-05-05 04:26:47.000000 pyproject-generator-0.1.9/src/pyproject_generator.egg-info/SOURCES.txt
+-rw-r--r--   0 cangyuanli   (501) staff       (20)        1 2023-05-05 04:26:47.000000 pyproject-generator-0.1.9/src/pyproject_generator.egg-info/dependency_links.txt
+-rw-r--r--   0 cangyuanli   (501) staff       (20)       49 2023-05-05 04:26:47.000000 pyproject-generator-0.1.9/src/pyproject_generator.egg-info/entry_points.txt
+-rw-r--r--   0 cangyuanli   (501) staff       (20)       13 2023-05-05 04:26:47.000000 pyproject-generator-0.1.9/src/pyproject_generator.egg-info/requires.txt
+-rw-r--r--   0 cangyuanli   (501) staff       (20)       10 2023-05-05 04:26:47.000000 pyproject-generator-0.1.9/src/pyproject_generator.egg-info/top_level.txt
+drwxr-xr-x   0 cangyuanli   (501) staff       (20)        0 2023-05-05 04:26:47.859089 pyproject-generator-0.1.9/tests/
+-rw-r--r--   0 cangyuanli   (501) staff       (20)        0 2023-05-05 02:42:30.000000 pyproject-generator-0.1.9/tests/test_pyproject.py
```

### Comparing `pyproject-generator-0.1.8/LICENSE` & `pyproject-generator-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `pyproject-generator-0.1.8/PKG-INFO` & `pyproject-generator-0.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyproject-generator
-Version: 0.1.8
+Version: 0.1.9
 Summary: A command line tool to setup Python packages
 Home-page: https://github.com/CangyuanLi/pyproject
 Author: Cangyuan Li
 Author-email: everest229@gmail.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/CangyuanLi/pyproject/issues
 Classifier: Programming Language :: Python :: 3
```

### Comparing `pyproject-generator-0.1.8/README.md` & `pyproject-generator-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `pyproject-generator-0.1.8/setup.cfg` & `pyproject-generator-0.1.9/setup.cfg`

 * *Files identical despite different names*

### Comparing `pyproject-generator-0.1.8/src/pyproject/cli.py` & `pyproject-generator-0.1.9/src/pyproject/cli.py`

 * *Files identical despite different names*

### Comparing `pyproject-generator-0.1.8/src/pyproject/licenses.py` & `pyproject-generator-0.1.9/src/pyproject/licenses.py`

 * *Files identical despite different names*

### Comparing `pyproject-generator-0.1.8/src/pyproject/logger.py` & `pyproject-generator-0.1.9/src/pyproject/logger.py`

 * *Files identical despite different names*

### Comparing `pyproject-generator-0.1.8/src/pyproject/project_builder.py` & `pyproject-generator-0.1.9/src/pyproject/project_builder.py`

 * *Files 2% similar despite different names*

```diff
@@ -218,14 +218,18 @@
                 result = src.substitute(d)
 
                 filled_in_templates[file.stem] = result
 
         return filled_in_templates
 
     @staticmethod
+    def _init_git():
+        subprocess.run(["git", "init"], stdout=subprocess.DEVNULL)
+
+    @staticmethod
     def _init_source_directory(proj_path: Path, project_name: str):
         src_path = proj_path / "src"
         src_path.mkdir()
 
         src_proj_path = src_path / project_name
         src_proj_path.mkdir()
         (src_proj_path / "__init__.py").touch()
@@ -288,14 +292,22 @@
         templates = self._logger.spinner(
             lambda: self._fill_in_templates(project_name),
             "Filling in templates",
             clear=True,
             min_show_duration=0.2,
         )
 
+        # initialize git repo
+        self._logger.spinner(
+            self._init_git,
+            "Initializing git repository",
+            clear=True,
+            min_show_duration=0.2,
+        )
+
         # src
         self._logger.spinner(
             lambda: self._init_source_directory(proj_path, project_name),
             "Creating source directory",
             clear=True,
             min_show_duration=0.2,
         )
```

### Comparing `pyproject-generator-0.1.8/src/pyproject/spinner.py` & `pyproject-generator-0.1.9/src/pyproject/spinner.py`

 * *Files identical despite different names*

### Comparing `pyproject-generator-0.1.8/src/pyproject/templates/gitignore.template` & `pyproject-generator-0.1.9/src/pyproject/templates/gitignore.template`

 * *Files identical despite different names*

### Comparing `pyproject-generator-0.1.8/src/pyproject/templates/license_apache.template` & `pyproject-generator-0.1.9/src/pyproject/templates/license_apache.template`

 * *Files identical despite different names*

### Comparing `pyproject-generator-0.1.8/src/pyproject/templates/license_bsd3.template` & `pyproject-generator-0.1.9/src/pyproject/templates/license_bsd3.template`

 * *Files identical despite different names*

### Comparing `pyproject-generator-0.1.8/src/pyproject/templates/license_mit.template` & `pyproject-generator-0.1.9/src/pyproject/templates/license_mit.template`

 * *Files identical despite different names*

### Comparing `pyproject-generator-0.1.8/src/pyproject/templates/pre_commit_config.template` & `pyproject-generator-0.1.9/src/pyproject/templates/pre_commit_config.template`

 * *Files identical despite different names*

### Comparing `pyproject-generator-0.1.8/src/pyproject/templates/readme.template` & `pyproject-generator-0.1.9/src/pyproject/templates/readme.template`

 * *Files identical despite different names*

### Comparing `pyproject-generator-0.1.8/src/pyproject/templates/setup.template` & `pyproject-generator-0.1.9/src/pyproject/templates/setup.template`

 * *Files identical despite different names*

### Comparing `pyproject-generator-0.1.8/src/pyproject/templates/tests.template` & `pyproject-generator-0.1.9/src/pyproject/templates/tests.template`

 * *Files identical despite different names*

### Comparing `pyproject-generator-0.1.8/src/pyproject_generator.egg-info/PKG-INFO` & `pyproject-generator-0.1.9/src/pyproject_generator.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyproject-generator
-Version: 0.1.8
+Version: 0.1.9
 Summary: A command line tool to setup Python packages
 Home-page: https://github.com/CangyuanLi/pyproject
 Author: Cangyuan Li
 Author-email: everest229@gmail.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/CangyuanLi/pyproject/issues
 Classifier: Programming Language :: Python :: 3
```

### Comparing `pyproject-generator-0.1.8/src/pyproject_generator.egg-info/SOURCES.txt` & `pyproject-generator-0.1.9/src/pyproject_generator.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -5,15 +5,14 @@
 src/pyproject/__init__.py
 src/pyproject/__version__.py
 src/pyproject/cli.py
 src/pyproject/licenses.py
 src/pyproject/logger.py
 src/pyproject/project_builder.py
 src/pyproject/spinner.py
-src/pyproject/config/config.json
 src/pyproject/config/default_config.json
 src/pyproject/templates/gitignore.template
 src/pyproject/templates/license_apache.template
 src/pyproject/templates/license_bsd3.template
 src/pyproject/templates/license_gpl_v3.template
 src/pyproject/templates/license_mit.template
 src/pyproject/templates/pre_commit_config.template
```

