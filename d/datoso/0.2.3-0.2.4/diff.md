# Comparing `tmp/datoso-0.2.3.tar.gz` & `tmp/datoso-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "datoso-0.2.3.tar", last modified: Fri May  5 03:28:37 2023, max compression
+gzip compressed data, was "datoso-0.2.4.tar", last modified: Fri May  5 04:45:00 2023, max compression
```

## Comparing `datoso-0.2.3.tar` & `datoso-0.2.4.tar`

### file list

```diff
@@ -1,54 +1,54 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 03:28:37.368187 datoso-0.2.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-05-05 03:28:21.000000 datoso-0.2.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      110 2023-05-05 03:28:21.000000 datoso-0.2.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     5600 2023-05-05 03:28:37.368187 datoso-0.2.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4665 2023-05-05 03:28:21.000000 datoso-0.2.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     2691 2023-05-05 03:28:21.000000 datoso-0.2.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      180 2023-05-05 03:28:37.368187 datoso-0.2.3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 03:28:37.364187 datoso-0.2.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 03:28:37.364187 datoso-0.2.3/src/datoso/
--rw-r--r--   0 runner    (1001) docker     (123)      166 2023-05-05 03:28:21.000000 datoso-0.2.3/src/datoso/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18019 2023-05-05 03:28:21.000000 datoso-0.2.3/src/datoso/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 03:28:37.364187 datoso-0.2.3/src/datoso/actions/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 03:28:21.000000 datoso-0.2.3/src/datoso/actions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5316 2023-05-05 03:28:21.000000 datoso-0.2.3/src/datoso/actions/processor.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 03:28:37.368187 datoso-0.2.3/src/datoso/commands/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 03:28:21.000000 datoso-0.2.3/src/datoso/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2355 2023-05-05 03:28:21.000000 datoso-0.2.3/src/datoso/commands/doctor.py
--rw-r--r--   0 runner    (1001) docker     (123)     3848 2023-05-05 03:28:21.000000 datoso-0.2.3/src/datoso/commands/seed.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 03:28:37.368187 datoso-0.2.3/src/datoso/configuration/
--rw-r--r--   0 runner    (1001) docker     (123)      209 2023-05-05 03:28:21.000000 datoso-0.2.3/src/datoso/configuration/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      465 2023-05-05 03:28:21.000000 datoso-0.2.3/src/datoso/configuration/configuration.py
--rw-r--r--   0 runner    (1001) docker     (123)      997 2023-05-05 03:28:21.000000 datoso-0.2.3/src/datoso/configuration/folder_helper.py
--rw-r--r--   0 runner    (1001) docker     (123)     3896 2023-05-05 03:28:21.000000 datoso-0.2.3/src/datoso/configuration/logger.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 03:28:37.368187 datoso-0.2.3/src/datoso/database/
--rw-r--r--   0 runner    (1001) docker     (123)     1220 2023-05-05 03:28:21.000000 datoso-0.2.3/src/datoso/database/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 03:28:37.368187 datoso-0.2.3/src/datoso/database/models/
--rw-r--r--   0 runner    (1001) docker     (123)      202 2023-05-05 03:28:21.000000 datoso-0.2.3/src/datoso/database/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2771 2023-05-05 03:28:21.000000 datoso-0.2.3/src/datoso/database/models/datfile.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 03:28:37.368187 datoso-0.2.3/src/datoso/database/seeds/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 03:28:21.000000 datoso-0.2.3/src/datoso/database/seeds/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1467 2023-05-05 03:28:21.000000 datoso-0.2.3/src/datoso/database/seeds/dat_repos.py
--rw-r--r--   0 runner    (1001) docker     (123)     2052 2023-05-05 03:28:21.000000 datoso-0.2.3/src/datoso/database/seeds/dat_rules.py
--rw-r--r--   0 runner    (1001) docker     (123)     1533 2023-05-05 03:28:21.000000 datoso-0.2.3/src/datoso/datoso.ini
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 03:28:37.368187 datoso-0.2.3/src/datoso/helpers/
--rw-r--r--   0 runner    (1001) docker     (123)     3347 2023-05-05 03:28:21.000000 datoso-0.2.3/src/datoso/helpers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1276 2023-05-05 03:28:21.000000 datoso-0.2.3/src/datoso/helpers/executor.py
--rw-r--r--   0 runner    (1001) docker     (123)     1287 2023-05-05 03:28:21.000000 datoso-0.2.3/src/datoso/helpers/plugins.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 03:28:37.368187 datoso-0.2.3/src/datoso/repositories/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 03:28:21.000000 datoso-0.2.3/src/datoso/repositories/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13001 2023-05-05 03:28:21.000000 datoso-0.2.3/src/datoso/repositories/dat.py
--rw-r--r--   0 runner    (1001) docker     (123)     1970 2023-05-05 03:28:21.000000 datoso-0.2.3/src/datoso/repositories/dedupe.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 03:28:37.368187 datoso-0.2.3/src/datoso/seeds/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 03:28:21.000000 datoso-0.2.3/src/datoso/seeds/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      486 2023-05-05 03:28:21.000000 datoso-0.2.3/src/datoso/seeds/rules.py
--rw-r--r--   0 runner    (1001) docker     (123)     4005 2023-05-05 03:28:21.000000 datoso-0.2.3/src/datoso/seeds/unknown_seed.py
--rw-r--r--   0 runner    (1001) docker     (123)      553 2023-05-05 03:28:21.000000 datoso-0.2.3/src/datoso/seeds.txt
--rw-r--r--   0 runner    (1001) docker     (123)    42230 2023-05-05 03:28:21.000000 datoso-0.2.3/src/datoso/systems.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 03:28:37.364187 datoso-0.2.3/src/datoso.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5600 2023-05-05 03:28:37.000000 datoso-0.2.3/src/datoso.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1188 2023-05-05 03:28:37.000000 datoso-0.2.3/src/datoso.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 03:28:37.000000 datoso-0.2.3/src/datoso.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-05-05 03:28:37.000000 datoso-0.2.3/src/datoso.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      827 2023-05-05 03:28:37.000000 datoso-0.2.3/src/datoso.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-05 03:28:37.000000 datoso-0.2.3/src/datoso.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 04:45:00.862411 datoso-0.2.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-05-05 04:44:44.000000 datoso-0.2.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-05-05 04:44:44.000000 datoso-0.2.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     5600 2023-05-05 04:45:00.862411 datoso-0.2.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4665 2023-05-05 04:44:44.000000 datoso-0.2.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     2691 2023-05-05 04:44:44.000000 datoso-0.2.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      180 2023-05-05 04:45:00.866411 datoso-0.2.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 04:45:00.850410 datoso-0.2.4/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 04:45:00.854411 datoso-0.2.4/src/datoso/
+-rw-r--r--   0 runner    (1001) docker     (123)      166 2023-05-05 04:44:44.000000 datoso-0.2.4/src/datoso/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18019 2023-05-05 04:44:44.000000 datoso-0.2.4/src/datoso/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 04:45:00.858411 datoso-0.2.4/src/datoso/actions/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 04:44:44.000000 datoso-0.2.4/src/datoso/actions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5316 2023-05-05 04:44:44.000000 datoso-0.2.4/src/datoso/actions/processor.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 04:45:00.858411 datoso-0.2.4/src/datoso/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 04:44:44.000000 datoso-0.2.4/src/datoso/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2355 2023-05-05 04:44:44.000000 datoso-0.2.4/src/datoso/commands/doctor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3848 2023-05-05 04:44:44.000000 datoso-0.2.4/src/datoso/commands/seed.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 04:45:00.858411 datoso-0.2.4/src/datoso/configuration/
+-rw-r--r--   0 runner    (1001) docker     (123)      209 2023-05-05 04:44:44.000000 datoso-0.2.4/src/datoso/configuration/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      465 2023-05-05 04:44:44.000000 datoso-0.2.4/src/datoso/configuration/configuration.py
+-rw-r--r--   0 runner    (1001) docker     (123)      997 2023-05-05 04:44:44.000000 datoso-0.2.4/src/datoso/configuration/folder_helper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3896 2023-05-05 04:44:44.000000 datoso-0.2.4/src/datoso/configuration/logger.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 04:45:00.858411 datoso-0.2.4/src/datoso/database/
+-rw-r--r--   0 runner    (1001) docker     (123)     1220 2023-05-05 04:44:44.000000 datoso-0.2.4/src/datoso/database/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 04:45:00.858411 datoso-0.2.4/src/datoso/database/models/
+-rw-r--r--   0 runner    (1001) docker     (123)      202 2023-05-05 04:44:44.000000 datoso-0.2.4/src/datoso/database/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2771 2023-05-05 04:44:44.000000 datoso-0.2.4/src/datoso/database/models/datfile.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 04:45:00.862411 datoso-0.2.4/src/datoso/database/seeds/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 04:44:44.000000 datoso-0.2.4/src/datoso/database/seeds/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1467 2023-05-05 04:44:44.000000 datoso-0.2.4/src/datoso/database/seeds/dat_repos.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2052 2023-05-05 04:44:44.000000 datoso-0.2.4/src/datoso/database/seeds/dat_rules.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1533 2023-05-05 04:44:44.000000 datoso-0.2.4/src/datoso/datoso.ini
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 04:45:00.862411 datoso-0.2.4/src/datoso/helpers/
+-rw-r--r--   0 runner    (1001) docker     (123)     3347 2023-05-05 04:44:44.000000 datoso-0.2.4/src/datoso/helpers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1276 2023-05-05 04:44:44.000000 datoso-0.2.4/src/datoso/helpers/executor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1322 2023-05-05 04:44:44.000000 datoso-0.2.4/src/datoso/helpers/plugins.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 04:45:00.862411 datoso-0.2.4/src/datoso/repositories/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 04:44:44.000000 datoso-0.2.4/src/datoso/repositories/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13001 2023-05-05 04:44:44.000000 datoso-0.2.4/src/datoso/repositories/dat.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1970 2023-05-05 04:44:44.000000 datoso-0.2.4/src/datoso/repositories/dedupe.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 04:45:00.862411 datoso-0.2.4/src/datoso/seeds/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 04:44:44.000000 datoso-0.2.4/src/datoso/seeds/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      486 2023-05-05 04:44:44.000000 datoso-0.2.4/src/datoso/seeds/rules.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4005 2023-05-05 04:44:44.000000 datoso-0.2.4/src/datoso/seeds/unknown_seed.py
+-rw-r--r--   0 runner    (1001) docker     (123)      553 2023-05-05 04:44:44.000000 datoso-0.2.4/src/datoso/seeds.txt
+-rw-r--r--   0 runner    (1001) docker     (123)    42230 2023-05-05 04:44:44.000000 datoso-0.2.4/src/datoso/systems.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 04:45:00.858411 datoso-0.2.4/src/datoso.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5600 2023-05-05 04:45:00.000000 datoso-0.2.4/src/datoso.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1188 2023-05-05 04:45:00.000000 datoso-0.2.4/src/datoso.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 04:45:00.000000 datoso-0.2.4/src/datoso.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-05-05 04:45:00.000000 datoso-0.2.4/src/datoso.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      827 2023-05-05 04:45:00.000000 datoso-0.2.4/src/datoso.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-05 04:45:00.000000 datoso-0.2.4/src/datoso.egg-info/top_level.txt
```

### Comparing `datoso-0.2.3/LICENSE` & `datoso-0.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `datoso-0.2.3/PKG-INFO` & `datoso-0.2.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datoso
-Version: 0.2.3
+Version: 0.2.4
 Summary: Python command line tool to download and organize your Rom Dat files.
 Author-email: Lacides Miranda <laromicas@hotmail.com>
 License: MIT License
 Project-URL: Source Code, https://github.com/laromicas/datoso
 Keywords: emulators,roms
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
```

### Comparing `datoso-0.2.3/README.md` & `datoso-0.2.4/README.md`

 * *Files identical despite different names*

### Comparing `datoso-0.2.3/pyproject.toml` & `datoso-0.2.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `datoso-0.2.3/src/datoso/__main__.py` & `datoso-0.2.4/src/datoso/__main__.py`

 * *Files identical despite different names*

### Comparing `datoso-0.2.3/src/datoso/actions/processor.py` & `datoso-0.2.4/src/datoso/actions/processor.py`

 * *Files identical despite different names*

### Comparing `datoso-0.2.3/src/datoso/commands/doctor.py` & `datoso-0.2.4/src/datoso/commands/doctor.py`

 * *Files identical despite different names*

### Comparing `datoso-0.2.3/src/datoso/commands/seed.py` & `datoso-0.2.4/src/datoso/commands/seed.py`

 * *Files identical despite different names*

### Comparing `datoso-0.2.3/src/datoso/configuration/folder_helper.py` & `datoso-0.2.4/src/datoso/configuration/folder_helper.py`

 * *Files identical despite different names*

### Comparing `datoso-0.2.3/src/datoso/configuration/logger.py` & `datoso-0.2.4/src/datoso/configuration/logger.py`

 * *Files identical despite different names*

### Comparing `datoso-0.2.3/src/datoso/database/__init__.py` & `datoso-0.2.4/src/datoso/database/__init__.py`

 * *Files identical despite different names*

### Comparing `datoso-0.2.3/src/datoso/database/models/datfile.py` & `datoso-0.2.4/src/datoso/database/models/datfile.py`

 * *Files identical despite different names*

### Comparing `datoso-0.2.3/src/datoso/database/seeds/dat_repos.py` & `datoso-0.2.4/src/datoso/database/seeds/dat_repos.py`

 * *Files identical despite different names*

### Comparing `datoso-0.2.3/src/datoso/database/seeds/dat_rules.py` & `datoso-0.2.4/src/datoso/database/seeds/dat_rules.py`

 * *Files identical despite different names*

### Comparing `datoso-0.2.3/src/datoso/datoso.ini` & `datoso-0.2.4/src/datoso/datoso.ini`

 * *Files identical despite different names*

### Comparing `datoso-0.2.3/src/datoso/helpers/__init__.py` & `datoso-0.2.4/src/datoso/helpers/__init__.py`

 * *Files identical despite different names*

### Comparing `datoso-0.2.3/src/datoso/helpers/executor.py` & `datoso-0.2.4/src/datoso/helpers/executor.py`

 * *Files identical despite different names*

### Comparing `datoso-0.2.3/src/datoso/helpers/plugins.py` & `datoso-0.2.4/src/datoso/helpers/plugins.py`

 * *Files 6% similar despite different names*

```diff
@@ -12,36 +12,35 @@
     if module:
         return locate(f'{__app_name__}_{plugin_type}_{plugin}.{module}')
     return locate(f'{__app_name__}_{plugin_type}_{plugin}')
 
 def installed(plugin_type):
     import importlib
     import pkgutil
-
     return {
         name: importlib.import_module(name)
         for finder, name, ispkg
         in pkgutil.iter_modules()
         if name.startswith(f'{__app_name__}_{plugin_type}_')
     }
 
 def description(plugin, plugin_type):
     plugin = plugin if isinstance(plugin, ModuleType) else locate(f'{__app_name__}_{plugin_type}_{plugin}')
     return plugin.__description__
 
 def get_seed(seed, module=None):
-    return get(seed, module, PluginType.SEED)
+    return get(seed, module, PluginType.SEED.value)
 
 def installed_seeds():
-    return installed(PluginType.SEED)
+    return installed(PluginType.SEED.value)
 
 def seed_description(seed):
-    return description(seed, PluginType.SEED)
+    return description(seed, PluginType.SEED.value)
 
 def get_plugin(plugin, module=None):
-    return get(plugin, module, PluginType.PLUGIN)
+    return get(plugin, module, PluginType.PLUGIN.value)
 
 def installed_plugins():
-    return installed(PluginType.PLUGIN)
+    return installed(PluginType.PLUGIN.value)
 
 def plugin_description(plugin):
-    return description(plugin, PluginType.PLUGIN)
+    return description(plugin, PluginType.PLUGIN.value)
```

### Comparing `datoso-0.2.3/src/datoso/repositories/dat.py` & `datoso-0.2.4/src/datoso/repositories/dat.py`

 * *Files identical despite different names*

### Comparing `datoso-0.2.3/src/datoso/repositories/dedupe.py` & `datoso-0.2.4/src/datoso/repositories/dedupe.py`

 * *Files identical despite different names*

### Comparing `datoso-0.2.3/src/datoso/seeds/unknown_seed.py` & `datoso-0.2.4/src/datoso/seeds/unknown_seed.py`

 * *Files identical despite different names*

### Comparing `datoso-0.2.3/src/datoso/seeds.txt` & `datoso-0.2.4/src/datoso/seeds.txt`

 * *Files identical despite different names*

### Comparing `datoso-0.2.3/src/datoso/systems.json` & `datoso-0.2.4/src/datoso/systems.json`

 * *Files identical despite different names*

### Comparing `datoso-0.2.3/src/datoso.egg-info/PKG-INFO` & `datoso-0.2.4/src/datoso.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datoso
-Version: 0.2.3
+Version: 0.2.4
 Summary: Python command line tool to download and organize your Rom Dat files.
 Author-email: Lacides Miranda <laromicas@hotmail.com>
 License: MIT License
 Project-URL: Source Code, https://github.com/laromicas/datoso
 Keywords: emulators,roms
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
```

### Comparing `datoso-0.2.3/src/datoso.egg-info/SOURCES.txt` & `datoso-0.2.4/src/datoso.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `datoso-0.2.3/src/datoso.egg-info/requires.txt` & `datoso-0.2.4/src/datoso.egg-info/requires.txt`

 * *Files identical despite different names*

