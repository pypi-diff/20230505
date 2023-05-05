# Comparing `tmp/fps_jupyterlab-0.1.5.tar.gz` & `tmp/fps_jupyterlab-0.1.6.tar.gz`

## Comparing `fps_jupyterlab-0.1.5.tar` & `fps_jupyterlab-0.1.6.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 fps_jupyterlab-0.1.5/MANIFEST.in
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 fps_jupyterlab-0.1.5/fps_jupyterlab/__init__.py
--rw-r--r--   0        0        0     1069 2020-02-02 00:00:00.000000 fps_jupyterlab-0.1.5/fps_jupyterlab/index.py
--rw-r--r--   0        0        0      965 2020-02-02 00:00:00.000000 fps_jupyterlab-0.1.5/fps_jupyterlab/main.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fps_jupyterlab-0.1.5/fps_jupyterlab/py.typed
--rw-r--r--   0        0        0     6212 2020-02-02 00:00:00.000000 fps_jupyterlab-0.1.5/fps_jupyterlab/routes.py
--rw-r--r--   0        0        0     6359 2020-02-02 00:00:00.000000 fps_jupyterlab-0.1.5/.gitignore
--rw-r--r--   0        0        0     2833 2020-02-02 00:00:00.000000 fps_jupyterlab-0.1.5/COPYING.md
--rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 fps_jupyterlab-0.1.5/README.md
--rw-r--r--   0        0        0      941 2020-02-02 00:00:00.000000 fps_jupyterlab-0.1.5/pyproject.toml
--rw-r--r--   0        0        0      506 2020-02-02 00:00:00.000000 fps_jupyterlab-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 fps_jupyterlab-0.1.6/MANIFEST.in
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 fps_jupyterlab-0.1.6/fps_jupyterlab/__init__.py
+-rw-r--r--   0        0        0     1069 2020-02-02 00:00:00.000000 fps_jupyterlab-0.1.6/fps_jupyterlab/index.py
+-rw-r--r--   0        0        0      965 2020-02-02 00:00:00.000000 fps_jupyterlab-0.1.6/fps_jupyterlab/main.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fps_jupyterlab-0.1.6/fps_jupyterlab/py.typed
+-rw-r--r--   0        0        0     6212 2020-02-02 00:00:00.000000 fps_jupyterlab-0.1.6/fps_jupyterlab/routes.py
+-rw-r--r--   0        0        0     6359 2020-02-02 00:00:00.000000 fps_jupyterlab-0.1.6/.gitignore
+-rw-r--r--   0        0        0     2833 2020-02-02 00:00:00.000000 fps_jupyterlab-0.1.6/COPYING.md
+-rw-r--r--   0        0        0       56 2020-02-02 00:00:00.000000 fps_jupyterlab-0.1.6/README.md
+-rw-r--r--   0        0        0      942 2020-02-02 00:00:00.000000 fps_jupyterlab-0.1.6/pyproject.toml
+-rw-r--r--   0        0        0      507 2020-02-02 00:00:00.000000 fps_jupyterlab-0.1.6/PKG-INFO
```

### Comparing `fps_jupyterlab-0.1.5/fps_jupyterlab/index.py` & `fps_jupyterlab-0.1.6/fps_jupyterlab/index.py`

 * *Files identical despite different names*

### Comparing `fps_jupyterlab-0.1.5/fps_jupyterlab/main.py` & `fps_jupyterlab-0.1.6/fps_jupyterlab/main.py`

 * *Files identical despite different names*

### Comparing `fps_jupyterlab-0.1.5/fps_jupyterlab/routes.py` & `fps_jupyterlab-0.1.6/fps_jupyterlab/routes.py`

 * *Files identical despite different names*

### Comparing `fps_jupyterlab-0.1.5/.gitignore` & `fps_jupyterlab-0.1.6/.gitignore`

 * *Files identical despite different names*

### Comparing `fps_jupyterlab-0.1.5/COPYING.md` & `fps_jupyterlab-0.1.6/COPYING.md`

 * *Files identical despite different names*

### Comparing `fps_jupyterlab-0.1.5/pyproject.toml` & `fps_jupyterlab-0.1.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 [project]
 name = "fps_jupyterlab"
 description = "An FPS plugin for the JupyterLab API"
 keywords = [ "jupyter", "server", "fastapi", "plugins" ]
 requires-python = ">=3.8"
 dependencies = [
-  "jupyterlab >=4.0.0b0,<5",
+  "jupyterlab >=4.0.0rc0,<5",
   "jupyverse-api >=0.1.2,<1",
 ]
 dynamic = [ "version",]
 [[project.authors]]
 name = "Jupyter Development Team"
 email = "jupyter@googlegroups.com"
```

