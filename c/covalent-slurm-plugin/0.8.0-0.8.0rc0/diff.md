# Comparing `tmp/covalent-slurm-plugin-0.8.0.tar.gz` & `tmp/covalent-slurm-plugin-0.8.0rc0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "covalent-slurm-plugin-0.8.0.tar", last modified: Sat Nov 19 01:00:20 2022, max compression
+gzip compressed data, was "covalent-slurm-plugin-0.8.0rc0.tar", last modified: Sat Nov 19 00:51:33 2022, max compression
```

## Comparing `covalent-slurm-plugin-0.8.0.tar` & `covalent-slurm-plugin-0.8.0rc0.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-19 01:00:20.102491 covalent-slurm-plugin-0.8.0/
--rw-r--r--   0 runner    (1001) docker     (121)    34523 2022-11-19 01:00:11.000000 covalent-slurm-plugin-0.8.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)       41 2022-11-19 01:00:11.000000 covalent-slurm-plugin-0.8.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     5856 2022-11-19 01:00:20.102491 covalent-slurm-plugin-0.8.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     3782 2022-11-19 01:00:11.000000 covalent-slurm-plugin-0.8.0/README.md
--rw-r--r--   0 runner    (1001) docker     (121)        6 2022-11-19 01:00:11.000000 covalent-slurm-plugin-0.8.0/VERSION
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-19 01:00:20.102491 covalent-slurm-plugin-0.8.0/covalent_slurm_plugin/
--rw-r--r--   0 runner    (1001) docker     (121)      869 2022-11-19 01:00:11.000000 covalent-slurm-plugin-0.8.0/covalent_slurm_plugin/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    18056 2022-11-19 01:00:11.000000 covalent-slurm-plugin-0.8.0/covalent_slurm_plugin/slurm.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-19 01:00:20.102491 covalent-slurm-plugin-0.8.0/covalent_slurm_plugin.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     5856 2022-11-19 01:00:20.000000 covalent-slurm-plugin-0.8.0/covalent_slurm_plugin.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      453 2022-11-19 01:00:20.000000 covalent-slurm-plugin-0.8.0/covalent_slurm_plugin.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-19 01:00:20.000000 covalent-slurm-plugin-0.8.0/covalent_slurm_plugin.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       74 2022-11-19 01:00:20.000000 covalent-slurm-plugin-0.8.0/covalent_slurm_plugin.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)       54 2022-11-19 01:00:20.000000 covalent-slurm-plugin-0.8.0/covalent_slurm_plugin.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       28 2022-11-19 01:00:20.000000 covalent-slurm-plugin-0.8.0/covalent_slurm_plugin.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1106 2022-11-19 01:00:11.000000 covalent-slurm-plugin-0.8.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)       54 2022-11-19 01:00:11.000000 covalent-slurm-plugin-0.8.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-11-19 01:00:20.102491 covalent-slurm-plugin-0.8.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     2823 2022-11-19 01:00:11.000000 covalent-slurm-plugin-0.8.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-19 01:00:20.102491 covalent-slurm-plugin-0.8.0/tests/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-19 01:00:11.000000 covalent-slurm-plugin-0.8.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     8295 2022-11-19 01:00:11.000000 covalent-slurm-plugin-0.8.0/tests/slurm_test.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-19 00:51:33.898447 covalent-slurm-plugin-0.8.0rc0/
+-rw-r--r--   0 runner    (1001) docker     (121)    34523 2022-11-19 00:51:25.000000 covalent-slurm-plugin-0.8.0rc0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (121)       41 2022-11-19 00:51:25.000000 covalent-slurm-plugin-0.8.0rc0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (121)     5859 2022-11-19 00:51:33.898447 covalent-slurm-plugin-0.8.0rc0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     3782 2022-11-19 00:51:25.000000 covalent-slurm-plugin-0.8.0rc0/README.md
+-rw-r--r--   0 runner    (1001) docker     (121)        6 2022-11-19 00:51:25.000000 covalent-slurm-plugin-0.8.0rc0/VERSION
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-19 00:51:33.894447 covalent-slurm-plugin-0.8.0rc0/covalent_slurm_plugin/
+-rw-r--r--   0 runner    (1001) docker     (121)      869 2022-11-19 00:51:25.000000 covalent-slurm-plugin-0.8.0rc0/covalent_slurm_plugin/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)    18056 2022-11-19 00:51:25.000000 covalent-slurm-plugin-0.8.0rc0/covalent_slurm_plugin/slurm.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-19 00:51:33.898447 covalent-slurm-plugin-0.8.0rc0/covalent_slurm_plugin.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     5859 2022-11-19 00:51:33.000000 covalent-slurm-plugin-0.8.0rc0/covalent_slurm_plugin.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      453 2022-11-19 00:51:33.000000 covalent-slurm-plugin-0.8.0rc0/covalent_slurm_plugin.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-11-19 00:51:33.000000 covalent-slurm-plugin-0.8.0rc0/covalent_slurm_plugin.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       74 2022-11-19 00:51:33.000000 covalent-slurm-plugin-0.8.0rc0/covalent_slurm_plugin.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       54 2022-11-19 00:51:33.000000 covalent-slurm-plugin-0.8.0rc0/covalent_slurm_plugin.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       28 2022-11-19 00:51:33.000000 covalent-slurm-plugin-0.8.0rc0/covalent_slurm_plugin.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     1106 2022-11-19 00:51:25.000000 covalent-slurm-plugin-0.8.0rc0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (121)       54 2022-11-19 00:51:25.000000 covalent-slurm-plugin-0.8.0rc0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       41 2022-11-19 00:51:33.898447 covalent-slurm-plugin-0.8.0rc0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)     2823 2022-11-19 00:51:25.000000 covalent-slurm-plugin-0.8.0rc0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-11-19 00:51:33.898447 covalent-slurm-plugin-0.8.0rc0/tests/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-11-19 00:51:25.000000 covalent-slurm-plugin-0.8.0rc0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     8295 2022-11-19 00:51:25.000000 covalent-slurm-plugin-0.8.0rc0/tests/slurm_test.py
```

### Comparing `covalent-slurm-plugin-0.8.0/LICENSE` & `covalent-slurm-plugin-0.8.0rc0/LICENSE`

 * *Files identical despite different names*

### Comparing `covalent-slurm-plugin-0.8.0/PKG-INFO` & `covalent-slurm-plugin-0.8.0rc0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: covalent-slurm-plugin
-Version: 0.8.0
+Version: 0.8.0rc0
 Summary: Covalent Slurm Plugin
 Home-page: https://github.com/AgnostiqHQ/covalent-slurm-plugin
 Author: Agnostiq
 Author-email: support@agnostiq.ai
 Maintainer: Agnostiq
 License: GNU Affero GPL v3.0
 Download-URL: https://github.com/AgnostiqHQ/covalent-slurm-plugin/archive/v0.8.0.tar.gz
```

### Comparing `covalent-slurm-plugin-0.8.0/README.md` & `covalent-slurm-plugin-0.8.0rc0/README.md`

 * *Files identical despite different names*

### Comparing `covalent-slurm-plugin-0.8.0/covalent_slurm_plugin/__init__.py` & `covalent-slurm-plugin-0.8.0rc0/covalent_slurm_plugin/__init__.py`

 * *Files identical despite different names*

### Comparing `covalent-slurm-plugin-0.8.0/covalent_slurm_plugin/slurm.py` & `covalent-slurm-plugin-0.8.0rc0/covalent_slurm_plugin/slurm.py`

 * *Files identical despite different names*

### Comparing `covalent-slurm-plugin-0.8.0/covalent_slurm_plugin.egg-info/PKG-INFO` & `covalent-slurm-plugin-0.8.0rc0/covalent_slurm_plugin.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: covalent-slurm-plugin
-Version: 0.8.0
+Version: 0.8.0rc0
 Summary: Covalent Slurm Plugin
 Home-page: https://github.com/AgnostiqHQ/covalent-slurm-plugin
 Author: Agnostiq
 Author-email: support@agnostiq.ai
 Maintainer: Agnostiq
 License: GNU Affero GPL v3.0
 Download-URL: https://github.com/AgnostiqHQ/covalent-slurm-plugin/archive/v0.8.0.tar.gz
```

### Comparing `covalent-slurm-plugin-0.8.0/pyproject.toml` & `covalent-slurm-plugin-0.8.0rc0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `covalent-slurm-plugin-0.8.0/setup.py` & `covalent-slurm-plugin-0.8.0rc0/setup.py`

 * *Files identical despite different names*

### Comparing `covalent-slurm-plugin-0.8.0/tests/slurm_test.py` & `covalent-slurm-plugin-0.8.0rc0/tests/slurm_test.py`

 * *Files identical despite different names*

