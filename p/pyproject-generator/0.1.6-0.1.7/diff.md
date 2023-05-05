# Comparing `tmp/pyproject-generator-0.1.6.tar.gz` & `tmp/pyproject-generator-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyproject-generator-0.1.6.tar", last modified: Fri May  5 02:35:12 2023, max compression
+gzip compressed data, was "pyproject-generator-0.1.7.tar", last modified: Fri May  5 03:28:05 2023, max compression
```

## Comparing `pyproject-generator-0.1.6.tar` & `pyproject-generator-0.1.7.tar`

### file list

```diff
@@ -1,39 +1,39 @@
-drwxr-xr-x   0 cangyuanli   (501) staff       (20)        0 2023-05-05 02:35:12.456054 pyproject-generator-0.1.6/
--rw-r--r--   0 cangyuanli   (501) staff       (20)     1078 2023-05-04 01:48:13.000000 pyproject-generator-0.1.6/LICENSE
--rw-r--r--   0 cangyuanli   (501) staff       (20)     3871 2023-05-05 02:35:12.456309 pyproject-generator-0.1.6/PKG-INFO
--rw-r--r--   0 cangyuanli   (501) staff       (20)     3330 2023-05-04 20:27:10.000000 pyproject-generator-0.1.6/README.md
--rw-r--r--   0 cangyuanli   (501) staff       (20)      264 2023-05-04 02:13:28.000000 pyproject-generator-0.1.6/pyproject.toml
--rw-r--r--   0 cangyuanli   (501) staff       (20)      868 2023-05-05 02:35:12.457296 pyproject-generator-0.1.6/setup.cfg
-drwxr-xr-x   0 cangyuanli   (501) staff       (20)        0 2023-05-05 02:35:12.423911 pyproject-generator-0.1.6/src/
-drwxr-xr-x   0 cangyuanli   (501) staff       (20)        0 2023-05-05 02:35:12.433962 pyproject-generator-0.1.6/src/pyproject/
--rw-r--r--   0 cangyuanli   (501) staff       (20)       51 2023-05-03 20:58:26.000000 pyproject-generator-0.1.6/src/pyproject/__init__.py
--rw-r--r--   0 cangyuanli   (501) staff       (20)       22 2023-05-05 02:34:52.000000 pyproject-generator-0.1.6/src/pyproject/__version__.py
--rw-r--r--   0 cangyuanli   (501) staff       (20)     3991 2023-05-05 02:33:44.000000 pyproject-generator-0.1.6/src/pyproject/cli.py
-drwxr-xr-x   0 cangyuanli   (501) staff       (20)        0 2023-05-05 02:35:12.436285 pyproject-generator-0.1.6/src/pyproject/config/
--rw-r--r--   0 cangyuanli   (501) staff       (20)      237 2023-04-28 18:40:04.000000 pyproject-generator-0.1.6/src/pyproject/config/config.json
--rw-r--r--   0 cangyuanli   (501) staff       (20)      281 2023-05-03 20:05:37.000000 pyproject-generator-0.1.6/src/pyproject/config/default_config.json
--rw-r--r--   0 cangyuanli   (501) staff       (20)     1029 2023-05-04 19:32:40.000000 pyproject-generator-0.1.6/src/pyproject/licenses.py
--rw-r--r--   0 cangyuanli   (501) staff       (20)     1729 2023-05-05 02:24:45.000000 pyproject-generator-0.1.6/src/pyproject/logger.py
--rw-r--r--   0 cangyuanli   (501) staff       (20)    15177 2023-05-05 02:24:58.000000 pyproject-generator-0.1.6/src/pyproject/project_builder.py
--rw-r--r--   0 cangyuanli   (501) staff       (20)     2753 2023-05-04 01:29:47.000000 pyproject-generator-0.1.6/src/pyproject/spinner.py
-drwxr-xr-x   0 cangyuanli   (501) staff       (20)        0 2023-05-05 02:35:12.449102 pyproject-generator-0.1.6/src/pyproject/templates/
--rw-r--r--   0 cangyuanli   (501) staff       (20)     1498 2023-05-03 19:23:49.000000 pyproject-generator-0.1.6/src/pyproject/templates/gitignore.template
--rw-r--r--   0 cangyuanli   (501) staff       (20)      548 2023-04-30 01:20:52.000000 pyproject-generator-0.1.6/src/pyproject/templates/license_apache.template
--rw-r--r--   0 cangyuanli   (501) staff       (20)     1457 2023-05-04 13:35:45.000000 pyproject-generator-0.1.6/src/pyproject/templates/license_bsd3.template
--rw-r--r--   0 cangyuanli   (501) staff       (20)        0 2023-04-30 15:11:38.000000 pyproject-generator-0.1.6/src/pyproject/templates/license_gpl_v3.template
--rw-r--r--   0 cangyuanli   (501) staff       (20)     1074 2023-04-30 01:18:24.000000 pyproject-generator-0.1.6/src/pyproject/templates/license_mit.template
--rw-r--r--   0 cangyuanli   (501) staff       (20)      905 2023-05-03 23:48:11.000000 pyproject-generator-0.1.6/src/pyproject/templates/pre_commit_config.template
--rw-r--r--   0 cangyuanli   (501) staff       (20)      263 2023-05-04 02:15:39.000000 pyproject-generator-0.1.6/src/pyproject/templates/pyproject.template
--rw-r--r--   0 cangyuanli   (501) staff       (20)     1040 2023-05-04 20:10:03.000000 pyproject-generator-0.1.6/src/pyproject/templates/readme.template
--rw-r--r--   0 cangyuanli   (501) staff       (20)      583 2023-04-30 15:11:46.000000 pyproject-generator-0.1.6/src/pyproject/templates/setup.template
--rw-r--r--   0 cangyuanli   (501) staff       (20)      649 2023-04-13 18:27:11.000000 pyproject-generator-0.1.6/src/pyproject/templates/tests.template
--rw-r--r--   0 cangyuanli   (501) staff       (20)      402 2023-04-12 23:45:24.000000 pyproject-generator-0.1.6/src/pyproject/templates/tox.template
-drwxr-xr-x   0 cangyuanli   (501) staff       (20)        0 2023-05-05 02:35:12.454718 pyproject-generator-0.1.6/src/pyproject_generator.egg-info/
--rw-r--r--   0 cangyuanli   (501) staff       (20)     3871 2023-05-05 02:35:12.000000 pyproject-generator-0.1.6/src/pyproject_generator.egg-info/PKG-INFO
--rw-r--r--   0 cangyuanli   (501) staff       (20)     1087 2023-05-05 02:35:12.000000 pyproject-generator-0.1.6/src/pyproject_generator.egg-info/SOURCES.txt
--rw-r--r--   0 cangyuanli   (501) staff       (20)        1 2023-05-05 02:35:12.000000 pyproject-generator-0.1.6/src/pyproject_generator.egg-info/dependency_links.txt
--rw-r--r--   0 cangyuanli   (501) staff       (20)       49 2023-05-05 02:35:12.000000 pyproject-generator-0.1.6/src/pyproject_generator.egg-info/entry_points.txt
--rw-r--r--   0 cangyuanli   (501) staff       (20)       13 2023-05-05 02:35:12.000000 pyproject-generator-0.1.6/src/pyproject_generator.egg-info/requires.txt
--rw-r--r--   0 cangyuanli   (501) staff       (20)       10 2023-05-05 02:35:12.000000 pyproject-generator-0.1.6/src/pyproject_generator.egg-info/top_level.txt
-drwxr-xr-x   0 cangyuanli   (501) staff       (20)        0 2023-05-05 02:35:12.455538 pyproject-generator-0.1.6/tests/
--rw-r--r--   0 cangyuanli   (501) staff       (20)        0 2023-04-19 15:24:26.000000 pyproject-generator-0.1.6/tests/test_pyproject.py
+drwxr-xr-x   0 cangyuanli   (501) staff       (20)        0 2023-05-05 03:28:05.807924 pyproject-generator-0.1.7/
+-rw-r--r--   0 cangyuanli   (501) staff       (20)     1078 2023-05-04 01:48:13.000000 pyproject-generator-0.1.7/LICENSE
+-rw-r--r--   0 cangyuanli   (501) staff       (20)     3871 2023-05-05 03:28:05.808180 pyproject-generator-0.1.7/PKG-INFO
+-rw-r--r--   0 cangyuanli   (501) staff       (20)     3330 2023-05-05 02:42:29.000000 pyproject-generator-0.1.7/README.md
+-rw-r--r--   0 cangyuanli   (501) staff       (20)      264 2023-05-05 02:42:29.000000 pyproject-generator-0.1.7/pyproject.toml
+-rw-r--r--   0 cangyuanli   (501) staff       (20)      868 2023-05-05 03:28:05.810475 pyproject-generator-0.1.7/setup.cfg
+drwxr-xr-x   0 cangyuanli   (501) staff       (20)        0 2023-05-05 03:28:05.769980 pyproject-generator-0.1.7/src/
+drwxr-xr-x   0 cangyuanli   (501) staff       (20)        0 2023-05-05 03:28:05.781134 pyproject-generator-0.1.7/src/pyproject/
+-rw-r--r--   0 cangyuanli   (501) staff       (20)       51 2023-05-05 02:42:30.000000 pyproject-generator-0.1.7/src/pyproject/__init__.py
+-rw-r--r--   0 cangyuanli   (501) staff       (20)       22 2023-05-05 03:27:58.000000 pyproject-generator-0.1.7/src/pyproject/__version__.py
+-rw-r--r--   0 cangyuanli   (501) staff       (20)     3991 2023-05-05 02:42:30.000000 pyproject-generator-0.1.7/src/pyproject/cli.py
+drwxr-xr-x   0 cangyuanli   (501) staff       (20)        0 2023-05-05 03:28:05.782729 pyproject-generator-0.1.7/src/pyproject/config/
+-rw-r--r--   0 cangyuanli   (501) staff       (20)      237 2023-05-05 02:42:30.000000 pyproject-generator-0.1.7/src/pyproject/config/config.json
+-rw-r--r--   0 cangyuanli   (501) staff       (20)      281 2023-05-05 02:42:31.000000 pyproject-generator-0.1.7/src/pyproject/config/default_config.json
+-rw-r--r--   0 cangyuanli   (501) staff       (20)     1029 2023-05-05 02:42:30.000000 pyproject-generator-0.1.7/src/pyproject/licenses.py
+-rw-r--r--   0 cangyuanli   (501) staff       (20)     1729 2023-05-05 02:42:30.000000 pyproject-generator-0.1.7/src/pyproject/logger.py
+-rw-r--r--   0 cangyuanli   (501) staff       (20)    15177 2023-05-05 03:27:26.000000 pyproject-generator-0.1.7/src/pyproject/project_builder.py
+-rw-r--r--   0 cangyuanli   (501) staff       (20)     2753 2023-05-05 02:42:30.000000 pyproject-generator-0.1.7/src/pyproject/spinner.py
+drwxr-xr-x   0 cangyuanli   (501) staff       (20)        0 2023-05-05 03:28:05.799676 pyproject-generator-0.1.7/src/pyproject/templates/
+-rw-r--r--   0 cangyuanli   (501) staff       (20)     1498 2023-05-03 19:23:49.000000 pyproject-generator-0.1.7/src/pyproject/templates/gitignore.template
+-rw-r--r--   0 cangyuanli   (501) staff       (20)      548 2023-04-30 01:20:52.000000 pyproject-generator-0.1.7/src/pyproject/templates/license_apache.template
+-rw-r--r--   0 cangyuanli   (501) staff       (20)     1457 2023-05-04 13:35:45.000000 pyproject-generator-0.1.7/src/pyproject/templates/license_bsd3.template
+-rw-r--r--   0 cangyuanli   (501) staff       (20)        0 2023-04-30 15:11:38.000000 pyproject-generator-0.1.7/src/pyproject/templates/license_gpl_v3.template
+-rw-r--r--   0 cangyuanli   (501) staff       (20)     1074 2023-04-30 01:18:24.000000 pyproject-generator-0.1.7/src/pyproject/templates/license_mit.template
+-rw-r--r--   0 cangyuanli   (501) staff       (20)      905 2023-05-03 23:48:11.000000 pyproject-generator-0.1.7/src/pyproject/templates/pre_commit_config.template
+-rw-r--r--   0 cangyuanli   (501) staff       (20)      263 2023-05-04 02:15:39.000000 pyproject-generator-0.1.7/src/pyproject/templates/pyproject.template
+-rw-r--r--   0 cangyuanli   (501) staff       (20)     1040 2023-05-04 20:10:03.000000 pyproject-generator-0.1.7/src/pyproject/templates/readme.template
+-rw-r--r--   0 cangyuanli   (501) staff       (20)      583 2023-04-30 15:11:46.000000 pyproject-generator-0.1.7/src/pyproject/templates/setup.template
+-rw-r--r--   0 cangyuanli   (501) staff       (20)      649 2023-04-13 18:27:11.000000 pyproject-generator-0.1.7/src/pyproject/templates/tests.template
+-rw-r--r--   0 cangyuanli   (501) staff       (20)      402 2023-04-12 23:45:24.000000 pyproject-generator-0.1.7/src/pyproject/templates/tox.template
+drwxr-xr-x   0 cangyuanli   (501) staff       (20)        0 2023-05-05 03:28:05.806122 pyproject-generator-0.1.7/src/pyproject_generator.egg-info/
+-rw-r--r--   0 cangyuanli   (501) staff       (20)     3871 2023-05-05 03:28:05.000000 pyproject-generator-0.1.7/src/pyproject_generator.egg-info/PKG-INFO
+-rw-r--r--   0 cangyuanli   (501) staff       (20)     1087 2023-05-05 03:28:05.000000 pyproject-generator-0.1.7/src/pyproject_generator.egg-info/SOURCES.txt
+-rw-r--r--   0 cangyuanli   (501) staff       (20)        1 2023-05-05 03:28:05.000000 pyproject-generator-0.1.7/src/pyproject_generator.egg-info/dependency_links.txt
+-rw-r--r--   0 cangyuanli   (501) staff       (20)       49 2023-05-05 03:28:05.000000 pyproject-generator-0.1.7/src/pyproject_generator.egg-info/entry_points.txt
+-rw-r--r--   0 cangyuanli   (501) staff       (20)       13 2023-05-05 03:28:05.000000 pyproject-generator-0.1.7/src/pyproject_generator.egg-info/requires.txt
+-rw-r--r--   0 cangyuanli   (501) staff       (20)       10 2023-05-05 03:28:05.000000 pyproject-generator-0.1.7/src/pyproject_generator.egg-info/top_level.txt
+drwxr-xr-x   0 cangyuanli   (501) staff       (20)        0 2023-05-05 03:28:05.807155 pyproject-generator-0.1.7/tests/
+-rw-r--r--   0 cangyuanli   (501) staff       (20)        0 2023-05-05 02:42:30.000000 pyproject-generator-0.1.7/tests/test_pyproject.py
```

### Comparing `pyproject-generator-0.1.6/LICENSE` & `pyproject-generator-0.1.7/LICENSE`

 * *Files identical despite different names*

### Comparing `pyproject-generator-0.1.6/PKG-INFO` & `pyproject-generator-0.1.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyproject-generator
-Version: 0.1.6
+Version: 0.1.7
 Summary: A command line tool to setup Python packages
 Home-page: https://github.com/CangyuanLi/pyproject
 Author: Cangyuan Li
 Author-email: everest229@gmail.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/CangyuanLi/pyproject/issues
 Classifier: Programming Language :: Python :: 3
```

### Comparing `pyproject-generator-0.1.6/README.md` & `pyproject-generator-0.1.7/README.md`

 * *Files identical despite different names*

### Comparing `pyproject-generator-0.1.6/setup.cfg` & `pyproject-generator-0.1.7/setup.cfg`

 * *Files identical despite different names*

### Comparing `pyproject-generator-0.1.6/src/pyproject/cli.py` & `pyproject-generator-0.1.7/src/pyproject/cli.py`

 * *Files identical despite different names*

### Comparing `pyproject-generator-0.1.6/src/pyproject/licenses.py` & `pyproject-generator-0.1.7/src/pyproject/licenses.py`

 * *Files identical despite different names*

### Comparing `pyproject-generator-0.1.6/src/pyproject/logger.py` & `pyproject-generator-0.1.7/src/pyproject/logger.py`

 * *Files identical despite different names*

### Comparing `pyproject-generator-0.1.6/src/pyproject/project_builder.py` & `pyproject-generator-0.1.7/src/pyproject/project_builder.py`

 * *Files 0% similar despite different names*

```diff
@@ -65,15 +65,15 @@
         c1 = config1.to_dict()
         c2 = config2.to_dict()
         merged_config = {}
         for k, v in c1.items():
             if c2[k] is None:
                 merged_config[k] = v
             else:
-                merged_config[k] = c1[k]
+                merged_config[k] = c2[k]
 
         return Config(**merged_config)
 
     def __or__(self, config2: Config) -> Config:
         dct = self.to_dict() | config2.to_dict()
 
         return Config(**dct)
```

### Comparing `pyproject-generator-0.1.6/src/pyproject/spinner.py` & `pyproject-generator-0.1.7/src/pyproject/spinner.py`

 * *Files identical despite different names*

### Comparing `pyproject-generator-0.1.6/src/pyproject/templates/gitignore.template` & `pyproject-generator-0.1.7/src/pyproject/templates/gitignore.template`

 * *Files identical despite different names*

### Comparing `pyproject-generator-0.1.6/src/pyproject/templates/license_apache.template` & `pyproject-generator-0.1.7/src/pyproject/templates/license_apache.template`

 * *Files identical despite different names*

### Comparing `pyproject-generator-0.1.6/src/pyproject/templates/license_bsd3.template` & `pyproject-generator-0.1.7/src/pyproject/templates/license_bsd3.template`

 * *Files identical despite different names*

### Comparing `pyproject-generator-0.1.6/src/pyproject/templates/license_mit.template` & `pyproject-generator-0.1.7/src/pyproject/templates/license_mit.template`

 * *Files identical despite different names*

### Comparing `pyproject-generator-0.1.6/src/pyproject/templates/pre_commit_config.template` & `pyproject-generator-0.1.7/src/pyproject/templates/pre_commit_config.template`

 * *Files identical despite different names*

### Comparing `pyproject-generator-0.1.6/src/pyproject/templates/readme.template` & `pyproject-generator-0.1.7/src/pyproject/templates/readme.template`

 * *Files identical despite different names*

### Comparing `pyproject-generator-0.1.6/src/pyproject/templates/setup.template` & `pyproject-generator-0.1.7/src/pyproject/templates/setup.template`

 * *Files identical despite different names*

### Comparing `pyproject-generator-0.1.6/src/pyproject/templates/tests.template` & `pyproject-generator-0.1.7/src/pyproject/templates/tests.template`

 * *Files identical despite different names*

### Comparing `pyproject-generator-0.1.6/src/pyproject_generator.egg-info/PKG-INFO` & `pyproject-generator-0.1.7/src/pyproject_generator.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyproject-generator
-Version: 0.1.6
+Version: 0.1.7
 Summary: A command line tool to setup Python packages
 Home-page: https://github.com/CangyuanLi/pyproject
 Author: Cangyuan Li
 Author-email: everest229@gmail.com
 License: MIT
 Project-URL: Bug Tracker, https://github.com/CangyuanLi/pyproject/issues
 Classifier: Programming Language :: Python :: 3
```

### Comparing `pyproject-generator-0.1.6/src/pyproject_generator.egg-info/SOURCES.txt` & `pyproject-generator-0.1.7/src/pyproject_generator.egg-info/SOURCES.txt`

 * *Files identical despite different names*

