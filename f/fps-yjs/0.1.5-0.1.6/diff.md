# Comparing `tmp/fps_yjs-0.1.5.tar.gz` & `tmp/fps_yjs-0.1.6.tar.gz`

## Comparing `fps_yjs-0.1.5.tar` & `fps_yjs-0.1.6.tar`

### file list

```diff
@@ -1,10 +1,10 @@
--rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 fps_yjs-0.1.5/MANIFEST.in
--rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 fps_yjs-0.1.5/fps_yjs/__init__.py
--rw-r--r--   0        0        0      996 2020-02-02 00:00:00.000000 fps_yjs-0.1.5/fps_yjs/main.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fps_yjs-0.1.5/fps_yjs/py.typed
--rw-r--r--   0        0        0    13858 2020-02-02 00:00:00.000000 fps_yjs-0.1.5/fps_yjs/routes.py
--rw-r--r--   0        0        0     6359 2020-02-02 00:00:00.000000 fps_yjs-0.1.5/.gitignore
--rw-r--r--   0        0        0     2833 2020-02-02 00:00:00.000000 fps_yjs-0.1.5/COPYING.md
--rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 fps_yjs-0.1.5/README.md
--rw-r--r--   0        0        0      945 2020-02-02 00:00:00.000000 fps_yjs-0.1.5/pyproject.toml
--rw-r--r--   0        0        0      555 2020-02-02 00:00:00.000000 fps_yjs-0.1.5/PKG-INFO
+-rw-r--r--   0        0        0       13 2020-02-02 00:00:00.000000 fps_yjs-0.1.6/MANIFEST.in
+-rw-r--r--   0        0        0       22 2020-02-02 00:00:00.000000 fps_yjs-0.1.6/fps_yjs/__init__.py
+-rw-r--r--   0        0        0      996 2020-02-02 00:00:00.000000 fps_yjs-0.1.6/fps_yjs/main.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 fps_yjs-0.1.6/fps_yjs/py.typed
+-rw-r--r--   0        0        0    13858 2020-02-02 00:00:00.000000 fps_yjs-0.1.6/fps_yjs/routes.py
+-rw-r--r--   0        0        0     6359 2020-02-02 00:00:00.000000 fps_yjs-0.1.6/.gitignore
+-rw-r--r--   0        0        0     2833 2020-02-02 00:00:00.000000 fps_yjs-0.1.6/COPYING.md
+-rw-r--r--   0        0        0       42 2020-02-02 00:00:00.000000 fps_yjs-0.1.6/README.md
+-rw-r--r--   0        0        0      937 2020-02-02 00:00:00.000000 fps_yjs-0.1.6/pyproject.toml
+-rw-r--r--   0        0        0      547 2020-02-02 00:00:00.000000 fps_yjs-0.1.6/PKG-INFO
```

### Comparing `fps_yjs-0.1.5/fps_yjs/main.py` & `fps_yjs-0.1.6/fps_yjs/main.py`

 * *Files identical despite different names*

### Comparing `fps_yjs-0.1.5/fps_yjs/routes.py` & `fps_yjs-0.1.6/fps_yjs/routes.py`

 * *Files identical despite different names*

### Comparing `fps_yjs-0.1.5/.gitignore` & `fps_yjs-0.1.6/.gitignore`

 * *Files identical despite different names*

### Comparing `fps_yjs-0.1.5/COPYING.md` & `fps_yjs-0.1.6/COPYING.md`

 * *Files identical despite different names*

### Comparing `fps_yjs-0.1.5/pyproject.toml` & `fps_yjs-0.1.6/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 [project]
 name = "fps_yjs"
 description = "An FPS plugin for the Yjs API"
 keywords = [ "jupyter", "server", "fastapi", "plugins" ]
 requires-python = ">=3.8"
 dependencies = [
-    "jupyter_ydoc >=0.3.4,<0.4.0",
+    "jupyter_ydoc >=1,<2",
     "ypy-websocket >=0.8.2,<1",
     "y-py >=0.6.0,<0.7.0",
     "jupyverse-api >=0.1.2,<1",
 ]
 dynamic = [ "version",]
 [[project.authors]]
 name = "Jupyter Development Team"
```

### Comparing `fps_yjs-0.1.5/PKG-INFO` & `fps_yjs-0.1.6/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: fps_yjs
-Version: 0.1.5
+Version: 0.1.6
 Summary: An FPS plugin for the Yjs API
 Project-URL: Homepage, https://jupyter.org
 Author-email: Jupyter Development Team <jupyter@googlegroups.com>
 License: BSD 3-Clause License
 License-File: COPYING.md
 Keywords: fastapi,jupyter,plugins,server
 Requires-Python: >=3.8
-Requires-Dist: jupyter-ydoc<0.4.0,>=0.3.4
+Requires-Dist: jupyter-ydoc<2,>=1
 Requires-Dist: jupyverse-api<1,>=0.1.2
 Requires-Dist: y-py<0.7.0,>=0.6.0
 Requires-Dist: ypy-websocket<1,>=0.8.2
 Description-Content-Type: text/markdown
 
 # fps-yjs
```

