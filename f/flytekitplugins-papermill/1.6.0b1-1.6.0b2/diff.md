# Comparing `tmp/flytekitplugins-papermill-1.6.0b1.tar.gz` & `tmp/flytekitplugins-papermill-1.6.0b2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flytekitplugins-papermill-1.6.0b1.tar", last modified: Wed May  3 04:48:11 2023, max compression
+gzip compressed data, was "flytekitplugins-papermill-1.6.0b2.tar", last modified: Fri May  5 17:49:48 2023, max compression
```

## Comparing `flytekitplugins-papermill-1.6.0b1.tar` & `flytekitplugins-papermill-1.6.0b2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 04:48:11.568319 flytekitplugins-papermill-1.6.0b1/
--rw-r--r--   0 runner    (1001) docker     (123)      798 2023-05-03 04:48:11.568319 flytekitplugins-papermill-1.6.0b1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      789 2023-05-03 04:47:44.000000 flytekitplugins-papermill-1.6.0b1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 04:48:11.564319 flytekitplugins-papermill-1.6.0b1/flytekitplugins/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 04:48:11.564319 flytekitplugins-papermill-1.6.0b1/flytekitplugins/papermill/
--rw-r--r--   0 runner    (1001) docker     (123)      274 2023-05-03 04:47:44.000000 flytekitplugins-papermill-1.6.0b1/flytekitplugins/papermill/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12932 2023-05-03 04:47:44.000000 flytekitplugins-papermill-1.6.0b1/flytekitplugins/papermill/task.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 04:48:11.564319 flytekitplugins-papermill-1.6.0b1/flytekitplugins_papermill.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      798 2023-05-03 04:48:11.000000 flytekitplugins-papermill-1.6.0b1/flytekitplugins_papermill.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      392 2023-05-03 04:48:11.000000 flytekitplugins-papermill-1.6.0b1/flytekitplugins_papermill.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-03 04:48:11.000000 flytekitplugins-papermill-1.6.0b1/flytekitplugins_papermill.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-03 04:48:11.000000 flytekitplugins-papermill-1.6.0b1/flytekitplugins_papermill.egg-info/namespace_packages.txt
--rw-r--r--   0 runner    (1001) docker     (123)       76 2023-05-03 04:48:11.000000 flytekitplugins-papermill-1.6.0b1/flytekitplugins_papermill.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-03 04:48:11.000000 flytekitplugins-papermill-1.6.0b1/flytekitplugins_papermill.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-03 04:48:11.568319 flytekitplugins-papermill-1.6.0b1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1223 2023-05-03 04:48:03.000000 flytekitplugins-papermill-1.6.0b1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 17:49:48.730198 flytekitplugins-papermill-1.6.0b2/
+-rw-r--r--   0 runner    (1001) docker     (123)      798 2023-05-05 17:49:48.730198 flytekitplugins-papermill-1.6.0b2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      789 2023-05-05 17:49:25.000000 flytekitplugins-papermill-1.6.0b2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 17:49:48.730198 flytekitplugins-papermill-1.6.0b2/flytekitplugins/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 17:49:48.730198 flytekitplugins-papermill-1.6.0b2/flytekitplugins/papermill/
+-rw-r--r--   0 runner    (1001) docker     (123)      274 2023-05-05 17:49:25.000000 flytekitplugins-papermill-1.6.0b2/flytekitplugins/papermill/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12932 2023-05-05 17:49:25.000000 flytekitplugins-papermill-1.6.0b2/flytekitplugins/papermill/task.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 17:49:48.730198 flytekitplugins-papermill-1.6.0b2/flytekitplugins_papermill.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      798 2023-05-05 17:49:48.000000 flytekitplugins-papermill-1.6.0b2/flytekitplugins_papermill.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      392 2023-05-05 17:49:48.000000 flytekitplugins-papermill-1.6.0b2/flytekitplugins_papermill.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 17:49:48.000000 flytekitplugins-papermill-1.6.0b2/flytekitplugins_papermill.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-05 17:49:48.000000 flytekitplugins-papermill-1.6.0b2/flytekitplugins_papermill.egg-info/namespace_packages.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       76 2023-05-05 17:49:48.000000 flytekitplugins-papermill-1.6.0b2/flytekitplugins_papermill.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-05 17:49:48.000000 flytekitplugins-papermill-1.6.0b2/flytekitplugins_papermill.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-05 17:49:48.730198 flytekitplugins-papermill-1.6.0b2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1223 2023-05-05 17:49:40.000000 flytekitplugins-papermill-1.6.0b2/setup.py
```

### Comparing `flytekitplugins-papermill-1.6.0b1/PKG-INFO` & `flytekitplugins-papermill-1.6.0b2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flytekitplugins-papermill
-Version: 1.6.0b1
+Version: 1.6.0b2
 Summary: This is the flytekit papermill plugin
 Author: flyteorg
 Author-email: admin@flyte.org
 License: apache2
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `flytekitplugins-papermill-1.6.0b1/README.md` & `flytekitplugins-papermill-1.6.0b2/README.md`

 * *Files identical despite different names*

### Comparing `flytekitplugins-papermill-1.6.0b1/flytekitplugins/papermill/task.py` & `flytekitplugins-papermill-1.6.0b2/flytekitplugins/papermill/task.py`

 * *Files identical despite different names*

### Comparing `flytekitplugins-papermill-1.6.0b1/flytekitplugins_papermill.egg-info/PKG-INFO` & `flytekitplugins-papermill-1.6.0b2/flytekitplugins_papermill.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flytekitplugins-papermill
-Version: 1.6.0b1
+Version: 1.6.0b2
 Summary: This is the flytekit papermill plugin
 Author: flyteorg
 Author-email: admin@flyte.org
 License: apache2
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `flytekitplugins-papermill-1.6.0b1/setup.py` & `flytekitplugins-papermill-1.6.0b2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 plugin_requires = [
     "flytekit>=1.3.0b2,<2.0.0",
     "papermill>=1.2.0",
     "nbconvert>=6.0.7",
     "ipykernel>=5.0.0",
 ]
 
-__version__ = "1.6.0b1"
+__version__ = "1.6.0b2"
 
 setup(
     name=microlib_name,
     version=__version__,
     author="flyteorg",
     author_email="admin@flyte.org",
     description="This is the flytekit papermill plugin",
```

