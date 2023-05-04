# Comparing `tmp/cfgpie-2.3.7.tar.gz` & `tmp/cfgpie-2.3.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cfgpie-2.3.7.tar", last modified: Mon Dec  5 19:26:36 2022, max compression
+gzip compressed data, was "cfgpie-2.3.9.tar", last modified: Thu Dec 29 12:42:45 2022, max compression
```

## Comparing `cfgpie-2.3.7.tar` & `cfgpie-2.3.9.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxrwxrwx   0        0        0        0 2022-12-05 19:26:36.207733 cfgpie-2.3.7/
--rw-rw-rw-   0        0        0     1090 2022-09-04 11:44:11.000000 cfgpie-2.3.7/LICENSE
--rw-rw-rw-   0        0        0       14 2022-10-24 07:53:37.000000 cfgpie-2.3.7/MANIFEST.in
--rw-rw-rw-   0        0        0     6208 2022-12-05 19:26:36.207733 cfgpie-2.3.7/PKG-INFO
--rw-rw-rw-   0        0        0     5251 2022-10-24 19:21:20.000000 cfgpie-2.3.7/README.md
--rw-rw-rw-   0        0        0       93 2022-08-10 18:07:14.000000 cfgpie-2.3.7/pyproject.toml
--rw-rw-rw-   0        0        0     1084 2022-12-05 19:26:36.207733 cfgpie-2.3.7/setup.cfg
-drwxrwxrwx   0        0        0        0 2022-12-05 19:26:36.187304 cfgpie-2.3.7/src/
-drwxrwxrwx   0        0        0        0 2022-12-05 19:26:36.196328 cfgpie-2.3.7/src/cfgpie/
--rw-rw-rw-   0        0        0      385 2022-10-24 19:10:52.000000 cfgpie-2.3.7/src/cfgpie/__init__.py
--rw-rw-rw-   0        0        0      546 2022-10-04 17:04:28.000000 cfgpie-2.3.7/src/cfgpie/constants.py
--rw-rw-rw-   0        0        0      225 2022-10-02 15:56:49.000000 cfgpie-2.3.7/src/cfgpie/exceptions.py
--rw-rw-rw-   0        0        0     5839 2022-11-09 17:00:16.000000 cfgpie-2.3.7/src/cfgpie/handlers.py
--rw-rw-rw-   0        0        0      946 2022-12-01 16:27:10.000000 cfgpie-2.3.7/src/cfgpie/utils.py
-drwxrwxrwx   0        0        0        0 2022-12-05 19:26:36.196328 cfgpie-2.3.7/src/cfgpie.egg-info/
--rw-rw-rw-   0        0        0     6208 2022-12-05 19:26:36.000000 cfgpie-2.3.7/src/cfgpie.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      338 2022-12-05 19:26:36.000000 cfgpie-2.3.7/src/cfgpie.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-12-05 19:26:36.000000 cfgpie-2.3.7/src/cfgpie.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2022-09-04 16:13:39.000000 cfgpie-2.3.7/src/cfgpie.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0        7 2022-12-05 19:26:36.000000 cfgpie-2.3.7/src/cfgpie.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2022-12-29 12:42:45.958235 cfgpie-2.3.9/
+-rw-rw-rw-   0        0        0     1090 2022-09-04 11:44:11.000000 cfgpie-2.3.9/LICENSE
+-rw-rw-rw-   0        0        0       14 2022-10-24 07:53:37.000000 cfgpie-2.3.9/MANIFEST.in
+-rw-rw-rw-   0        0        0     6191 2022-12-29 12:42:45.958235 cfgpie-2.3.9/PKG-INFO
+-rw-rw-rw-   0        0        0     5234 2022-12-29 12:36:33.000000 cfgpie-2.3.9/README.md
+-rw-rw-rw-   0        0        0       93 2022-08-10 18:07:14.000000 cfgpie-2.3.9/pyproject.toml
+-rw-rw-rw-   0        0        0     1084 2022-12-29 12:42:45.958235 cfgpie-2.3.9/setup.cfg
+drwxrwxrwx   0        0        0        0 2022-12-29 12:42:45.938493 cfgpie-2.3.9/src/
+drwxrwxrwx   0        0        0        0 2022-12-29 12:42:45.947256 cfgpie-2.3.9/src/cfgpie/
+-rw-rw-rw-   0        0        0      384 2022-12-29 12:07:25.000000 cfgpie-2.3.9/src/cfgpie/__init__.py
+-rw-rw-rw-   0        0        0      546 2022-10-04 17:04:28.000000 cfgpie-2.3.9/src/cfgpie/constants.py
+-rw-rw-rw-   0        0        0      225 2022-10-02 15:56:49.000000 cfgpie-2.3.9/src/cfgpie/exceptions.py
+-rw-rw-rw-   0        0        0     5850 2022-12-29 12:11:38.000000 cfgpie-2.3.9/src/cfgpie/handlers.py
+-rw-rw-rw-   0        0        0      946 2022-12-01 16:27:10.000000 cfgpie-2.3.9/src/cfgpie/utils.py
+drwxrwxrwx   0        0        0        0 2022-12-29 12:42:45.947256 cfgpie-2.3.9/src/cfgpie.egg-info/
+-rw-rw-rw-   0        0        0     6191 2022-12-29 12:42:45.000000 cfgpie-2.3.9/src/cfgpie.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      338 2022-12-29 12:42:45.000000 cfgpie-2.3.9/src/cfgpie.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2022-12-29 12:42:45.000000 cfgpie-2.3.9/src/cfgpie.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2022-09-04 16:13:39.000000 cfgpie-2.3.9/src/cfgpie.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0        7 2022-12-29 12:42:45.000000 cfgpie-2.3.9/src/cfgpie.egg-info/top_level.txt
```

### Comparing `cfgpie-2.3.7/LICENSE` & `cfgpie-2.3.9/LICENSE`

 * *Files identical despite different names*

### Comparing `cfgpie-2.3.7/PKG-INFO` & `cfgpie-2.3.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cfgpie
-Version: 2.3.7
+Version: 2.3.9
 Summary: Simplified `ConfigParser` setup.
 Home-page: https://github.com/ClaudiuDrug/cfgpie
 Author: Claudiu DRUG
 Author-email: claudiu.drug@outlook.com
 License: MIT License
 Project-URL: Bug Tracker, https://github.com/ClaudiuDrug/cfgpie/issues
 Classifier: Programming Language :: Python :: 3.7
@@ -42,15 +42,15 @@
 #### Usage:
 
 After installation, simply import the method `get_config` from `cfgpie` module:
 ```python
 from cfgpie import CfgParser, get_config
 ```
 
-By passing a name with the `instance` param we can have multiple instances:
+By passing a name with the `name` param we can have multiple instances:
 ```python
 # mymodule.py
 
 from cfgpie import CfgParser, get_config
 
 cfg: CfgParser = get_config(name="main")
 cfg2: CfgParser = get_config(name="main")
@@ -173,15 +173,15 @@
 #### Defaults:
 
 If not provided, by default, `CfgParser` will set:
 
 * `defaults` parameter as dict with section `DEFAULT` and option `directory` to the root folder of the `__main__` module.
 
 
-* `instance` parameter to the name `default`;
+* `name` parameter to: `cfgpie`;
 
 
 * `interpolation` parameter to [ExtendedInterpolation](https://docs.python.org/3.7/library/configparser.html#configparser.ExtendedInterpolation);
 
 
 * `converters` parameter to evaluate:
```

### Comparing `cfgpie-2.3.7/README.md` & `cfgpie-2.3.9/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -18,15 +18,15 @@
 #### Usage:
 
 After installation, simply import the method `get_config` from `cfgpie` module:
 ```python
 from cfgpie import CfgParser, get_config
 ```
 
-By passing a name with the `instance` param we can have multiple instances:
+By passing a name with the `name` param we can have multiple instances:
 ```python
 # mymodule.py
 
 from cfgpie import CfgParser, get_config
 
 cfg: CfgParser = get_config(name="main")
 cfg2: CfgParser = get_config(name="main")
@@ -149,15 +149,15 @@
 #### Defaults:
 
 If not provided, by default, `CfgParser` will set:
 
 * `defaults` parameter as dict with section `DEFAULT` and option `directory` to the root folder of the `__main__` module.
 
 
-* `instance` parameter to the name `default`;
+* `name` parameter to: `cfgpie`;
 
 
 * `interpolation` parameter to [ExtendedInterpolation](https://docs.python.org/3.7/library/configparser.html#configparser.ExtendedInterpolation);
 
 
 * `converters` parameter to evaluate:
```

### Comparing `cfgpie-2.3.7/setup.cfg` & `cfgpie-2.3.9/setup.cfg`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2063 6667 7069 650d 0a76 6572 7369   = cfgpie..versi
-00000020: 6f6e 203d 2032 2e33 2e37 0d0a 6175 7468  on = 2.3.7..auth
+00000020: 6f6e 203d 2032 2e33 2e39 0d0a 6175 7468  on = 2.3.9..auth
 00000030: 6f72 203d 2043 6c61 7564 6975 2044 5255  or = Claudiu DRU
 00000040: 470d 0a61 7574 686f 725f 656d 6169 6c20  G..author_email 
 00000050: 3d20 636c 6175 6469 752e 6472 7567 406f  = claudiu.drug@o
 00000060: 7574 6c6f 6f6b 2e63 6f6d 0d0a 6c69 6365  utlook.com..lice
 00000070: 6e73 6520 3d20 4d49 5420 4c69 6365 6e73  nse = MIT Licens
 00000080: 650d 0a64 6573 6372 6970 7469 6f6e 203d  e..description =
 00000090: 2053 696d 706c 6966 6965 6420 6043 6f6e   Simplified `Con
```

### Comparing `cfgpie-2.3.7/src/cfgpie/constants.py` & `cfgpie-2.3.9/src/cfgpie/constants.py`

 * *Files identical despite different names*

### Comparing `cfgpie-2.3.7/src/cfgpie/handlers.py` & `cfgpie-2.3.9/src/cfgpie/handlers.py`

 * *Files 1% similar despite different names*

```diff
@@ -84,15 +84,15 @@
 
         return mapping
 
     @staticmethod
     def _exists(item: str) -> bool:
         return exists(item) and isfile(item)
 
-    def __init__(self, name: str, **kwargs):
+    def __init__(self, name: str = "cfgpie", **kwargs):
 
         self._name = name
         self._thread_lock: RLock = self._dispatch(self._name)
 
         super(CfgParser, self).__init__(**self._default_params(kwargs))
 
     @property
```

### Comparing `cfgpie-2.3.7/src/cfgpie/utils.py` & `cfgpie-2.3.9/src/cfgpie/utils.py`

 * *Files identical despite different names*

### Comparing `cfgpie-2.3.7/src/cfgpie.egg-info/PKG-INFO` & `cfgpie-2.3.9/src/cfgpie.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cfgpie
-Version: 2.3.7
+Version: 2.3.9
 Summary: Simplified `ConfigParser` setup.
 Home-page: https://github.com/ClaudiuDrug/cfgpie
 Author: Claudiu DRUG
 Author-email: claudiu.drug@outlook.com
 License: MIT License
 Project-URL: Bug Tracker, https://github.com/ClaudiuDrug/cfgpie/issues
 Classifier: Programming Language :: Python :: 3.7
@@ -42,15 +42,15 @@
 #### Usage:
 
 After installation, simply import the method `get_config` from `cfgpie` module:
 ```python
 from cfgpie import CfgParser, get_config
 ```
 
-By passing a name with the `instance` param we can have multiple instances:
+By passing a name with the `name` param we can have multiple instances:
 ```python
 # mymodule.py
 
 from cfgpie import CfgParser, get_config
 
 cfg: CfgParser = get_config(name="main")
 cfg2: CfgParser = get_config(name="main")
@@ -173,15 +173,15 @@
 #### Defaults:
 
 If not provided, by default, `CfgParser` will set:
 
 * `defaults` parameter as dict with section `DEFAULT` and option `directory` to the root folder of the `__main__` module.
 
 
-* `instance` parameter to the name `default`;
+* `name` parameter to: `cfgpie`;
 
 
 * `interpolation` parameter to [ExtendedInterpolation](https://docs.python.org/3.7/library/configparser.html#configparser.ExtendedInterpolation);
 
 
 * `converters` parameter to evaluate:
```

