# Comparing `tmp/config_joker-0.2.0.tar.gz` & `tmp/config_joker-0.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "config_joker-0.2.0.tar", max compression
+gzip compressed data, was "config_joker-0.3.0.tar", max compression
```

## Comparing `config_joker-0.2.0.tar` & `config_joker-0.3.0.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     1083 2023-04-04 01:35:47.633704 config_joker-0.2.0/LICENSE
--rw-r--r--   0        0        0      730 2023-04-11 01:35:43.700475 config_joker-0.2.0/README.md
--rw-r--r--   0        0        0        0 2023-04-04 02:48:51.887021 config_joker-0.2.0/config_joker/__init__.py
--rw-r--r--   0        0        0     1293 2023-04-05 01:44:05.797405 config_joker-0.2.0/config_joker/config.py
--rw-r--r--   0        0        0        0 2023-04-04 02:48:43.263208 config_joker-0.2.0/config_joker/sources/__init__.py
--rw-r--r--   0        0        0      422 2023-04-04 03:07:58.416142 config_joker-0.2.0/config_joker/sources/environment.py
--rw-r--r--   0        0        0      360 2023-04-11 01:44:37.188523 config_joker-0.2.0/config_joker/sources/source.py
--rw-r--r--   0        0        0      680 2023-04-11 03:34:20.915789 config_joker-0.2.0/config_joker/sources/yamlfile.py
--rw-r--r--   0        0        0        0 2023-04-11 02:22:08.615358 config_joker-0.2.0/config_joker/utils/__init__.py
--rw-r--r--   0        0        0      997 2023-04-11 03:33:33.152316 config_joker-0.2.0/config_joker/utils/parser.py
--rw-r--r--   0        0        0      403 2023-04-11 03:46:30.706740 config_joker-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     1274 1970-01-01 00:00:00.000000 config_joker-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0     1083 2023-04-04 01:35:47.633704 config_joker-0.3.0/LICENSE
+-rw-r--r--   0        0        0      796 2023-05-05 14:26:07.467811 config_joker-0.3.0/README.md
+-rw-r--r--   0        0        0      122 2023-05-05 14:25:37.792222 config_joker-0.3.0/config_joker/__init__.py
+-rw-r--r--   0        0        0     1293 2023-04-05 01:44:05.797405 config_joker-0.3.0/config_joker/config.py
+-rw-r--r--   0        0        0        0 2023-04-04 02:48:43.263208 config_joker-0.3.0/config_joker/sources/__init__.py
+-rw-r--r--   0        0        0      422 2023-04-04 03:07:58.416142 config_joker-0.3.0/config_joker/sources/environment.py
+-rw-r--r--   0        0        0      360 2023-04-11 01:44:37.188523 config_joker-0.3.0/config_joker/sources/source.py
+-rw-r--r--   0        0        0      680 2023-04-11 03:34:20.915789 config_joker-0.3.0/config_joker/sources/yamlfile.py
+-rw-r--r--   0        0        0        0 2023-04-11 02:22:08.615358 config_joker-0.3.0/config_joker/utils/__init__.py
+-rw-r--r--   0        0        0      997 2023-04-11 03:33:33.152316 config_joker-0.3.0/config_joker/utils/parser.py
+-rw-r--r--   0        0        0      724 2023-05-05 15:00:55.393195 config_joker-0.3.0/pyproject.toml
+-rw-r--r--   0        0        0     1340 1970-01-01 00:00:00.000000 config_joker-0.3.0/PKG-INFO
```

### Comparing `config_joker-0.2.0/LICENSE` & `config_joker-0.3.0/LICENSE`

 * *Files identical despite different names*

### Comparing `config_joker-0.2.0/README.md` & `config_joker-0.3.0/README.md`

 * *Files 23% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 # config-joker
 A package to ease usage of different configuration conditions in your projects.
 
 ## How to use in
 
+Obs.: There are some examples in the [examples folder](https://github.com/joaopedromgoulart/config-joker/tree/main/examples)
+
 Import the sources you'll use and the Config class:
 
-    from config_joker.sources.environment import EnvironmentSource
-    from config_joker.config import Config
+    from config_joker Config, EnvironmentSource
 
 Initialize the config class implementing the sources you want to use:
 
     config = Config(
             sources=[
                 EnvironmentSource()
             ]
@@ -18,8 +19,9 @@
 
 Find the configurations you want to use:
 
     import os
     os.environ['env_variable'] = '1'
     number_one_from_env_source_as_int = config.required(key='env_variable', value_type=int)
 
-The value stored in number_one_from_env_source_as_int will be the number one as an integer.
+The value stored in number_one_from_env_source_as_int will be the number one as an integer.
+
```

### Comparing `config_joker-0.2.0/config_joker/config.py` & `config_joker-0.3.0/config_joker/config.py`

 * *Files identical despite different names*

### Comparing `config_joker-0.2.0/config_joker/sources/yamlfile.py` & `config_joker-0.3.0/config_joker/sources/yamlfile.py`

 * *Files identical despite different names*

### Comparing `config_joker-0.2.0/config_joker/utils/parser.py` & `config_joker-0.3.0/config_joker/utils/parser.py`

 * *Files identical despite different names*

### Comparing `config_joker-0.2.0/PKG-INFO` & `config_joker-0.3.0/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: config-joker
-Version: 0.2.0
+Version: 0.3.0
 Summary: A package to ease usage of different configuration conditions in your projects.
 Author: Joao Pedro Mendes Goulart
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
@@ -13,18 +13,19 @@
 Description-Content-Type: text/markdown
 
 # config-joker
 A package to ease usage of different configuration conditions in your projects.
 
 ## How to use in
 
+Obs.: There are some examples in the [examples folder](https://github.com/joaopedromgoulart/config-joker/tree/main/examples)
+
 Import the sources you'll use and the Config class:
 
-    from config_joker.sources.environment import EnvironmentSource
-    from config_joker.config import Config
+    from config_joker Config, EnvironmentSource
 
 Initialize the config class implementing the sources you want to use:
 
     config = Config(
             sources=[
                 EnvironmentSource()
             ]
@@ -33,7 +34,9 @@
 Find the configurations you want to use:
 
     import os
     os.environ['env_variable'] = '1'
     number_one_from_env_source_as_int = config.required(key='env_variable', value_type=int)
 
 The value stored in number_one_from_env_source_as_int will be the number one as an integer.
+
+
```

