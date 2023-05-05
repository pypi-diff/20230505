# Comparing `tmp/flytekitplugins-onnxscikitlearn-1.6.0b1.tar.gz` & `tmp/flytekitplugins-onnxscikitlearn-1.6.0b2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flytekitplugins-onnxscikitlearn-1.6.0b1.tar", last modified: Wed May  3 04:48:10 2023, max compression
+gzip compressed data, was "flytekitplugins-onnxscikitlearn-1.6.0b2.tar", last modified: Fri May  5 17:49:48 2023, max compression
```

## Comparing `flytekitplugins-onnxscikitlearn-1.6.0b1.tar` & `flytekitplugins-onnxscikitlearn-1.6.0b2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 04:48:10.856317 flytekitplugins-onnxscikitlearn-1.6.0b1/
--rw-r--r--   0 runner    (1001) docker     (123)      803 2023-05-03 04:48:10.856317 flytekitplugins-onnxscikitlearn-1.6.0b1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      217 2023-05-03 04:47:44.000000 flytekitplugins-onnxscikitlearn-1.6.0b1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 04:48:10.856317 flytekitplugins-onnxscikitlearn-1.6.0b1/flytekitplugins/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 04:48:10.856317 flytekitplugins-onnxscikitlearn-1.6.0b1/flytekitplugins/onnxscikitlearn/
--rw-r--r--   0 runner    (1001) docker     (123)      235 2023-05-03 04:47:44.000000 flytekitplugins-onnxscikitlearn-1.6.0b1/flytekitplugins/onnxscikitlearn/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6321 2023-05-03 04:47:44.000000 flytekitplugins-onnxscikitlearn-1.6.0b1/flytekitplugins/onnxscikitlearn/schema.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 04:48:10.856317 flytekitplugins-onnxscikitlearn-1.6.0b1/flytekitplugins_onnxscikitlearn.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      803 2023-05-03 04:48:10.000000 flytekitplugins-onnxscikitlearn-1.6.0b1/flytekitplugins_onnxscikitlearn.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      442 2023-05-03 04:48:10.000000 flytekitplugins-onnxscikitlearn-1.6.0b1/flytekitplugins_onnxscikitlearn.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-03 04:48:10.000000 flytekitplugins-onnxscikitlearn-1.6.0b1/flytekitplugins_onnxscikitlearn.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-03 04:48:10.000000 flytekitplugins-onnxscikitlearn-1.6.0b1/flytekitplugins_onnxscikitlearn.egg-info/namespace_packages.txt
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-05-03 04:48:10.000000 flytekitplugins-onnxscikitlearn-1.6.0b1/flytekitplugins_onnxscikitlearn.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-03 04:48:10.000000 flytekitplugins-onnxscikitlearn-1.6.0b1/flytekitplugins_onnxscikitlearn.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-03 04:48:10.856317 flytekitplugins-onnxscikitlearn-1.6.0b1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1187 2023-05-03 04:48:03.000000 flytekitplugins-onnxscikitlearn-1.6.0b1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 17:49:47.994189 flytekitplugins-onnxscikitlearn-1.6.0b2/
+-rw-r--r--   0 runner    (1001) docker     (123)      803 2023-05-05 17:49:47.994189 flytekitplugins-onnxscikitlearn-1.6.0b2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      217 2023-05-05 17:49:25.000000 flytekitplugins-onnxscikitlearn-1.6.0b2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 17:49:47.990188 flytekitplugins-onnxscikitlearn-1.6.0b2/flytekitplugins/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 17:49:47.994189 flytekitplugins-onnxscikitlearn-1.6.0b2/flytekitplugins/onnxscikitlearn/
+-rw-r--r--   0 runner    (1001) docker     (123)      235 2023-05-05 17:49:25.000000 flytekitplugins-onnxscikitlearn-1.6.0b2/flytekitplugins/onnxscikitlearn/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6321 2023-05-05 17:49:25.000000 flytekitplugins-onnxscikitlearn-1.6.0b2/flytekitplugins/onnxscikitlearn/schema.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 17:49:47.994189 flytekitplugins-onnxscikitlearn-1.6.0b2/flytekitplugins_onnxscikitlearn.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      803 2023-05-05 17:49:47.000000 flytekitplugins-onnxscikitlearn-1.6.0b2/flytekitplugins_onnxscikitlearn.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      442 2023-05-05 17:49:47.000000 flytekitplugins-onnxscikitlearn-1.6.0b2/flytekitplugins_onnxscikitlearn.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 17:49:47.000000 flytekitplugins-onnxscikitlearn-1.6.0b2/flytekitplugins_onnxscikitlearn.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-05 17:49:47.000000 flytekitplugins-onnxscikitlearn-1.6.0b2/flytekitplugins_onnxscikitlearn.egg-info/namespace_packages.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-05-05 17:49:47.000000 flytekitplugins-onnxscikitlearn-1.6.0b2/flytekitplugins_onnxscikitlearn.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-05 17:49:47.000000 flytekitplugins-onnxscikitlearn-1.6.0b2/flytekitplugins_onnxscikitlearn.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-05 17:49:47.994189 flytekitplugins-onnxscikitlearn-1.6.0b2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1187 2023-05-05 17:49:40.000000 flytekitplugins-onnxscikitlearn-1.6.0b2/setup.py
```

### Comparing `flytekitplugins-onnxscikitlearn-1.6.0b1/PKG-INFO` & `flytekitplugins-onnxscikitlearn-1.6.0b2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flytekitplugins-onnxscikitlearn
-Version: 1.6.0b1
+Version: 1.6.0b2
 Summary: ONNX ScikitLearn Plugin for Flytekit
 Author: flyteorg
 Author-email: admin@flyte.org
 License: apache2
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `flytekitplugins-onnxscikitlearn-1.6.0b1/flytekitplugins/onnxscikitlearn/schema.py` & `flytekitplugins-onnxscikitlearn-1.6.0b2/flytekitplugins/onnxscikitlearn/schema.py`

 * *Files identical despite different names*

### Comparing `flytekitplugins-onnxscikitlearn-1.6.0b1/flytekitplugins_onnxscikitlearn.egg-info/PKG-INFO` & `flytekitplugins-onnxscikitlearn-1.6.0b2/flytekitplugins_onnxscikitlearn.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flytekitplugins-onnxscikitlearn
-Version: 1.6.0b1
+Version: 1.6.0b2
 Summary: ONNX ScikitLearn Plugin for Flytekit
 Author: flyteorg
 Author-email: admin@flyte.org
 License: apache2
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `flytekitplugins-onnxscikitlearn-1.6.0b1/setup.py` & `flytekitplugins-onnxscikitlearn-1.6.0b2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 PLUGIN_NAME = "onnxscikitlearn"
 
 microlib_name = f"flytekitplugins-{PLUGIN_NAME}"
 
 plugin_requires = ["flytekit<1.3.0b2,<2.0.0", "skl2onnx>=1.10.3"]
 
-__version__ = "1.6.0b1"
+__version__ = "1.6.0b2"
 
 setup(
     name=f"flytekitplugins-{PLUGIN_NAME}",
     version=__version__,
     author="flyteorg",
     author_email="admin@flyte.org",
     description="ONNX ScikitLearn Plugin for Flytekit",
```

