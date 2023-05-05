# Comparing `tmp/flytekitplugins-envd-1.6.0b1.tar.gz` & `tmp/flytekitplugins-envd-1.6.0b2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flytekitplugins-envd-1.6.0b1.tar", last modified: Wed May  3 04:48:06 2023, max compression
+gzip compressed data, was "flytekitplugins-envd-1.6.0b2.tar", last modified: Fri May  5 17:49:44 2023, max compression
```

## Comparing `flytekitplugins-envd-1.6.0b1.tar` & `flytekitplugins-envd-1.6.0b2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 04:48:06.956297 flytekitplugins-envd-1.6.0b1/
--rw-r--r--   0 runner    (1001) docker     (123)      888 2023-05-03 04:48:06.956297 flytekitplugins-envd-1.6.0b1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      797 2023-05-03 04:47:44.000000 flytekitplugins-envd-1.6.0b1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 04:48:06.956297 flytekitplugins-envd-1.6.0b1/flytekitplugins/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 04:48:06.956297 flytekitplugins-envd-1.6.0b1/flytekitplugins/envd/
--rw-r--r--   0 runner    (1001) docker     (123)      255 2023-05-03 04:47:44.000000 flytekitplugins-envd-1.6.0b1/flytekitplugins/envd/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2610 2023-05-03 04:47:44.000000 flytekitplugins-envd-1.6.0b1/flytekitplugins/envd/image_builder.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 04:48:06.956297 flytekitplugins-envd-1.6.0b1/flytekitplugins_envd.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      888 2023-05-03 04:48:06.000000 flytekitplugins-envd-1.6.0b1/flytekitplugins_envd.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      408 2023-05-03 04:48:06.000000 flytekitplugins-envd-1.6.0b1/flytekitplugins_envd.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-03 04:48:06.000000 flytekitplugins-envd-1.6.0b1/flytekitplugins_envd.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-05-03 04:48:06.000000 flytekitplugins-envd-1.6.0b1/flytekitplugins_envd.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-03 04:48:06.000000 flytekitplugins-envd-1.6.0b1/flytekitplugins_envd.egg-info/namespace_packages.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-03 04:48:06.000000 flytekitplugins-envd-1.6.0b1/flytekitplugins_envd.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-03 04:48:06.000000 flytekitplugins-envd-1.6.0b1/flytekitplugins_envd.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-03 04:48:06.956297 flytekitplugins-envd-1.6.0b1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1314 2023-05-03 04:48:03.000000 flytekitplugins-envd-1.6.0b1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 17:49:44.038134 flytekitplugins-envd-1.6.0b2/
+-rw-r--r--   0 runner    (1001) docker     (123)      888 2023-05-05 17:49:44.038134 flytekitplugins-envd-1.6.0b2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      797 2023-05-05 17:49:25.000000 flytekitplugins-envd-1.6.0b2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 17:49:44.034134 flytekitplugins-envd-1.6.0b2/flytekitplugins/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 17:49:44.038134 flytekitplugins-envd-1.6.0b2/flytekitplugins/envd/
+-rw-r--r--   0 runner    (1001) docker     (123)      255 2023-05-05 17:49:25.000000 flytekitplugins-envd-1.6.0b2/flytekitplugins/envd/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2757 2023-05-05 17:49:25.000000 flytekitplugins-envd-1.6.0b2/flytekitplugins/envd/image_builder.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 17:49:44.038134 flytekitplugins-envd-1.6.0b2/flytekitplugins_envd.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      888 2023-05-05 17:49:44.000000 flytekitplugins-envd-1.6.0b2/flytekitplugins_envd.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      408 2023-05-05 17:49:44.000000 flytekitplugins-envd-1.6.0b2/flytekitplugins_envd.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 17:49:44.000000 flytekitplugins-envd-1.6.0b2/flytekitplugins_envd.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-05-05 17:49:44.000000 flytekitplugins-envd-1.6.0b2/flytekitplugins_envd.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-05 17:49:44.000000 flytekitplugins-envd-1.6.0b2/flytekitplugins_envd.egg-info/namespace_packages.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-05 17:49:44.000000 flytekitplugins-envd-1.6.0b2/flytekitplugins_envd.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-05 17:49:44.000000 flytekitplugins-envd-1.6.0b2/flytekitplugins_envd.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-05 17:49:44.038134 flytekitplugins-envd-1.6.0b2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1314 2023-05-05 17:49:40.000000 flytekitplugins-envd-1.6.0b2/setup.py
```

### Comparing `flytekitplugins-envd-1.6.0b1/PKG-INFO` & `flytekitplugins-envd-1.6.0b2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flytekitplugins-envd
-Version: 1.6.0b1
+Version: 1.6.0b2
 Summary: This package enables users to easily build a Docker image for tasks or workflows.
 Author: flyteorg
 Author-email: admin@flyte.org
 License: apache2
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `flytekitplugins-envd-1.6.0b1/README.md` & `flytekitplugins-envd-1.6.0b2/README.md`

 * *Files identical despite different names*

### Comparing `flytekitplugins-envd-1.6.0b1/flytekitplugins/envd/image_builder.py` & `flytekitplugins-envd-1.6.0b2/flytekitplugins/envd/image_builder.py`

 * *Files 4% similar despite different names*

```diff
@@ -44,24 +44,28 @@
 
     envd_config = f"""# syntax=v1
 
 def build():
     base(image="{base_image}", dev=False)
     install.python_packages(name = [{', '.join(map(str, map(lambda x: f'"{x}"', packages)))}])
     install.apt_packages(name = [{', '.join(map(str, map(lambda x: f'"{x}"', apt_packages)))}])
-    install.python(version="{image_spec.python_version}")
     runtime.environ(env={env})
 """
 
+    if image_spec.python_version:
+        # Indentation is required by envd
+        envd_config += f'    install.python(version="{image_spec.python_version}")\n'
+
     ctx = context_manager.FlyteContextManager.current_context()
     cfg_path = ctx.file_access.get_random_local_path("build.envd")
     pathlib.Path(cfg_path).parent.mkdir(parents=True, exist_ok=True)
 
     if image_spec.source_root:
         shutil.copytree(image_spec.source_root, pathlib.Path(cfg_path).parent, dirs_exist_ok=True)
+        # Indentation is required by envd
         envd_config += '    io.copy(host_path="./", envd_path="/root")'
 
     with open(cfg_path, "w+") as f:
         f.write(envd_config)
 
     return cfg_path
```

### Comparing `flytekitplugins-envd-1.6.0b1/flytekitplugins_envd.egg-info/PKG-INFO` & `flytekitplugins-envd-1.6.0b2/flytekitplugins_envd.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: flytekitplugins-envd
-Version: 1.6.0b1
+Version: 1.6.0b2
 Summary: This package enables users to easily build a Docker image for tasks or workflows.
 Author: flyteorg
 Author-email: admin@flyte.org
 License: apache2
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: Apache Software License
```

### Comparing `flytekitplugins-envd-1.6.0b1/setup.py` & `flytekitplugins-envd-1.6.0b2/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 PLUGIN_NAME = "envd"
 
 microlib_name = f"flytekitplugins-{PLUGIN_NAME}"
 
 plugin_requires = ["flytekit", "envd"]
 
-__version__ = "1.6.0b1"
+__version__ = "1.6.0b2"
 
 setup(
     name=microlib_name,
     version=__version__,
     author="flyteorg",
     author_email="admin@flyte.org",
     description="This package enables users to easily build a Docker image for tasks or workflows.",
```

