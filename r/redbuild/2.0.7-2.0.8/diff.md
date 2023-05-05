# Comparing `tmp/redbuild-2.0.7.tar.gz` & `tmp/redbuild-2.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "redbuild-2.0.7.tar", max compression
+gzip compressed data, was "redbuild-2.0.8.tar", max compression
```

## Comparing `redbuild-2.0.7.tar` & `redbuild-2.0.8.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     1066 2023-04-15 16:57:41.337879 redbuild-2.0.7/LICENSE
--rw-r--r--   0        0        0     2475 2023-04-17 07:13:34.753986 redbuild-2.0.7/README.md
--rw-r--r--   0        0        0      604 2023-04-17 01:56:51.840957 redbuild-2.0.7/pyproject.toml
--rw-r--r--   0        0        0      162 2023-04-17 00:47:12.554903 redbuild-2.0.7/redbuild/__init__.py
--rw-r--r--   0        0        0       60 2023-04-07 18:52:09.664386 redbuild-2.0.7/redbuild/__main__.py
--rw-r--r--   0        0        0    10678 2023-04-17 01:56:34.767608 redbuild-2.0.7/redbuild/cli.py
--rw-r--r--   0        0        0     1445 2023-04-17 01:41:29.902707 redbuild-2.0.7/redbuild/composer.py
--rw-r--r--   0        0        0      675 2023-04-15 17:10:40.965361 redbuild-2.0.7/redbuild/engine.py
--rw-r--r--   0        0        0      366 2023-04-17 01:15:37.329254 redbuild-2.0.7/redbuild/res.py
--rw-r--r--   0        0        0      836 2023-04-17 00:40:30.278667 redbuild-2.0.7/redbuild/util.py
--rw-r--r--   0        0        0     3208 1970-01-01 00:00:00.000000 redbuild-2.0.7/PKG-INFO
+-rw-r--r--   0        0        0     1066 2023-04-15 16:57:41.337879 redbuild-2.0.8/LICENSE
+-rw-r--r--   0        0        0     2475 2023-04-17 07:13:34.753986 redbuild-2.0.8/README.md
+-rw-r--r--   0        0        0      604 2023-05-05 00:03:01.111520 redbuild-2.0.8/pyproject.toml
+-rw-r--r--   0        0        0      162 2023-04-17 00:47:12.554903 redbuild-2.0.8/redbuild/__init__.py
+-rw-r--r--   0        0        0       60 2023-04-07 18:52:09.664386 redbuild-2.0.8/redbuild/__main__.py
+-rw-r--r--   0        0        0    10678 2023-04-17 01:56:34.767608 redbuild-2.0.8/redbuild/cli.py
+-rw-r--r--   0        0        0     1445 2023-04-17 01:41:29.902707 redbuild-2.0.8/redbuild/composer.py
+-rw-r--r--   0        0        0      856 2023-05-05 00:02:51.112733 redbuild-2.0.8/redbuild/engine.py
+-rw-r--r--   0        0        0      366 2023-04-17 01:15:37.329254 redbuild-2.0.8/redbuild/res.py
+-rw-r--r--   0        0        0      836 2023-04-17 00:40:30.278667 redbuild-2.0.8/redbuild/util.py
+-rw-r--r--   0        0        0     3208 1970-01-01 00:00:00.000000 redbuild-2.0.8/PKG-INFO
```

### Comparing `redbuild-2.0.7/LICENSE` & `redbuild-2.0.8/LICENSE`

 * *Files identical despite different names*

### Comparing `redbuild-2.0.7/README.md` & `redbuild-2.0.8/README.md`

 * *Files identical despite different names*

### Comparing `redbuild-2.0.7/pyproject.toml` & `redbuild-2.0.8/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "redbuild"
-version = "2.0.7"
+version = "2.0.8"
 description = "magic containerized builds"
 authors = ["redthing1 <redthing1@alt.icu>"]
 readme = "README.md"
 
 [tool.poetry.dependencies]
 python = ">=3.9,<4.0"
 typer = {extras = ["rich"], version = "^0.7.0"}
```

### Comparing `redbuild-2.0.7/redbuild/cli.py` & `redbuild-2.0.8/redbuild/cli.py`

 * *Files identical despite different names*

### Comparing `redbuild-2.0.7/redbuild/composer.py` & `redbuild-2.0.8/redbuild/composer.py`

 * *Files identical despite different names*

### Comparing `redbuild-2.0.7/redbuild/engine.py` & `redbuild-2.0.8/redbuild/engine.py`

 * *Files 21% similar despite different names*

```diff
@@ -5,22 +5,28 @@
 class ContainerEngine(Enum):
     podman = "podman"
     docker = "docker"
 
     def __str__(self):
         return self.value
 
+def is_program_available(program_name: str):
+    try:
+        sh.which(program_name)
+        return True
+    except sh.ErrorReturnCode:
+        return False
 
 def detect_container_engine():
     # get container engine
     # we prefer podman to docker, but we'll use docker if podman is not available
 
-    if sh.which("podman"):
+    if is_program_available("podman"):
         return ContainerEngine.podman
-    elif sh.which("docker"):
+    elif is_program_available("docker"):
         return ContainerEngine.docker
     else:
         raise Exception(
             "No usable container engine found. Please install podman or docker."
         )
```

### Comparing `redbuild-2.0.7/redbuild/util.py` & `redbuild-2.0.8/redbuild/util.py`

 * *Files identical despite different names*

### Comparing `redbuild-2.0.7/PKG-INFO` & `redbuild-2.0.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: redbuild
-Version: 2.0.7
+Version: 2.0.8
 Summary: magic containerized builds
 Author: redthing1
 Author-email: redthing1@alt.icu
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
```

