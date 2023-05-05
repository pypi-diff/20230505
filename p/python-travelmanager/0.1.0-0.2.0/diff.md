# Comparing `tmp/python_travelmanager-0.1.0.tar.gz` & `tmp/python_travelmanager-0.2.0.tar.gz`

## Comparing `python_travelmanager-0.1.0.tar` & `python_travelmanager-0.2.0.tar`

### file list

```diff
@@ -1,6 +1,6 @@
--rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 python_travelmanager-0.1.0/travelmanager/__init__.py
--rw-r--r--   0        0        0     1283 2020-02-02 00:00:00.000000 python_travelmanager-0.1.0/.gitignore
--rw-r--r--   0        0        0     1087 2020-02-02 00:00:00.000000 python_travelmanager-0.1.0/LICENSE
--rw-r--r--   0        0        0      246 2020-02-02 00:00:00.000000 python_travelmanager-0.1.0/README.md
--rw-r--r--   0        0        0      763 2020-02-02 00:00:00.000000 python_travelmanager-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      572 2020-02-02 00:00:00.000000 python_travelmanager-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0       30 2020-02-02 00:00:00.000000 python_travelmanager-0.2.0/travelmanager/__init__.py
+-rw-r--r--   0        0        0     1283 2020-02-02 00:00:00.000000 python_travelmanager-0.2.0/.gitignore
+-rw-r--r--   0        0        0     1087 2020-02-02 00:00:00.000000 python_travelmanager-0.2.0/LICENSE
+-rw-r--r--   0        0        0      246 2020-02-02 00:00:00.000000 python_travelmanager-0.2.0/README.md
+-rw-r--r--   0        0        0      763 2020-02-02 00:00:00.000000 python_travelmanager-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0      572 2020-02-02 00:00:00.000000 python_travelmanager-0.2.0/PKG-INFO
```

### Comparing `python_travelmanager-0.1.0/.gitignore` & `python_travelmanager-0.2.0/.gitignore`

 * *Files identical despite different names*

### Comparing `python_travelmanager-0.1.0/LICENSE` & `python_travelmanager-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `python_travelmanager-0.1.0/pyproject.toml` & `python_travelmanager-0.2.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -12,25 +12,25 @@
 
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "python_travelmanager"
-version = "0.1.0"
+version = "0.2.0"
 authors = [
     { name="Johannes Eimer", email="johannes.eimer@jep-dev.com" },
 ]
 description = "Python TravelManager"
 readme = "README.md"
 requires-python = ">=3.10"
 license = "MIT"
 keywords = ['Python', 'TravelManager']
 dependencies = [
-    "requests~=2.30.0",
+    "requests==2.28.0",
 ]
 
 [tool.hatch.build.targets.sdist]
 include = ["travelmanager"]
 
 [tool.hatch.build.targets.wheel]
 package = ["travelmanager"]
```

### Comparing `python_travelmanager-0.1.0/PKG-INFO` & `python_travelmanager-0.2.0/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,17 +1,17 @@
 Metadata-Version: 2.1
 Name: python_travelmanager
-Version: 0.1.0
+Version: 0.2.0
 Summary: Python TravelManager
 Author-email: Johannes Eimer <johannes.eimer@jep-dev.com>
 License-Expression: MIT
 License-File: LICENSE
 Keywords: Python,TravelManager
 Requires-Python: >=3.10
-Requires-Dist: requests~=2.30.0
+Requires-Dist: requests==2.28.0
 Description-Content-Type: text/markdown
 
 # python_travelmanager
 
 ## install dev
 python -m venv venv
 venv/Scripts/activate
```

