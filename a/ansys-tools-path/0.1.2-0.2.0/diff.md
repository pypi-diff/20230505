# Comparing `tmp/ansys-tools-path-0.1.2.tar.gz` & `tmp/ansys-tools-path-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ansys-tools-path-0.1.2.tar", last modified: Fri Apr 14 12:51:30 2023, max compression
+gzip compressed data, was "ansys-tools-path-0.2.0.tar", last modified: Fri May  5 11:29:55 2023, max compression
```

## Comparing `ansys-tools-path-0.1.2.tar` & `ansys-tools-path-0.2.0.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1089 2023-04-14 12:51:14.205697 ansys-tools-path-0.1.2/LICENSE
--rw-r--r--   0        0        0     4701 2023-04-14 12:51:14.205697 ansys-tools-path-0.1.2/README.rst
--rw-r--r--   0        0        0     1849 2023-04-14 12:51:14.205697 ansys-tools-path-0.1.2/pyproject.toml
--rw-r--r--   0        0        0      404 2023-04-14 12:51:14.205697 ansys-tools-path-0.1.2/src/ansys/tools/path/__init__.py
--rw-r--r--   0        0        0      194 2023-04-14 12:51:14.205697 ansys-tools-path-0.1.2/src/ansys/tools/path/misc.py
--rw-r--r--   0        0        0    13647 2023-04-14 12:51:14.205697 ansys-tools-path-0.1.2/src/ansys/tools/path/path.py
--rw-r--r--   0        0        0     6192 1970-01-01 00:00:00.000000 ansys-tools-path-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     1089 2023-05-05 11:29:42.712175 ansys-tools-path-0.2.0/LICENSE
+-rw-r--r--   0        0        0     4701 2023-05-05 11:29:42.712175 ansys-tools-path-0.2.0/README.rst
+-rw-r--r--   0        0        0     1849 2023-05-05 11:29:42.716175 ansys-tools-path-0.2.0/pyproject.toml
+-rw-r--r--   0        0        0      919 2023-05-05 11:29:42.716175 ansys-tools-path-0.2.0/src/ansys/tools/path/__init__.py
+-rw-r--r--   0        0        0      648 2023-05-05 11:29:42.716175 ansys-tools-path-0.2.0/src/ansys/tools/path/misc.py
+-rw-r--r--   0        0        0    25880 2023-05-05 11:29:42.716175 ansys-tools-path-0.2.0/src/ansys/tools/path/path.py
+-rw-r--r--   0        0        0     6192 1970-01-01 00:00:00.000000 ansys-tools-path-0.2.0/PKG-INFO
```

### Comparing `ansys-tools-path-0.1.2/LICENSE` & `ansys-tools-path-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ansys-tools-path-0.1.2/README.rst` & `ansys-tools-path-0.2.0/README.rst`

 * *Files identical despite different names*

### Comparing `ansys-tools-path-0.1.2/pyproject.toml` & `ansys-tools-path-0.2.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["flit_core >=3.2,<4"]
 build-backend = "flit_core.buildapi"
 
 [project]
 # Check https://flit.readthedocs.io/en/latest/pyproject_toml.html for all available sections
 name = "ansys-tools-path"
-version = "0.1.2"
+version = "0.2.0"
 description = "Library to locate Ansys products in a local machine."
 readme = "README.rst"
 requires-python = ">=3.7"
 license = {file = "LICENSE"}
 authors = [
     {name = "ANSYS, Inc.", email = "pyansys.core@ansys.com"},
 ]
@@ -31,23 +31,23 @@
     "importlib-metadata >=4.0",
     "appdirs>=1.4.0",
 ]
 
 
 [project.optional-dependencies]
 test = [
-    "pytest==7.3.0",
+    "pytest==7.3.1",
     "pytest-cov==4.0.0",
 ]
 
 doc = [
-    "Sphinx==5.3.0",
+    "Sphinx==7.0.0",
     "numpydoc==1.5.0",
-    "ansys-sphinx-theme==0.9.7",
-    "sphinx-copybutton==0.5.1",
+    "ansys-sphinx-theme==0.9.8",
+    "sphinx-copybutton==0.5.2",
 ]
 
 build = [
     "build==0.10.0",
     "twine==4.0.2",
 ]
```

### Comparing `ansys-tools-path-0.1.2/PKG-INFO` & `ansys-tools-path-0.2.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ansys-tools-path
-Version: 0.1.2
+Version: 0.2.0
 Summary: Library to locate Ansys products in a local machine.
 Author-email: "ANSYS, Inc." <pyansys.core@ansys.com>
 Maintainer-email: "ANSYS, Inc." <pyansys.core@ansys.com>
 Requires-Python: >=3.7
 Description-Content-Type: text/x-rst
 Classifier: Development Status :: 4 - Beta
 Classifier: Programming Language :: Python :: 3.7
@@ -14,19 +14,19 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Dist: importlib-metadata >=4.0
 Requires-Dist: appdirs>=1.4.0
 Requires-Dist: build==0.10.0 ; extra == "build"
 Requires-Dist: twine==4.0.2 ; extra == "build"
-Requires-Dist: Sphinx==5.3.0 ; extra == "doc"
+Requires-Dist: Sphinx==7.0.0 ; extra == "doc"
 Requires-Dist: numpydoc==1.5.0 ; extra == "doc"
-Requires-Dist: ansys-sphinx-theme==0.9.7 ; extra == "doc"
-Requires-Dist: sphinx-copybutton==0.5.1 ; extra == "doc"
-Requires-Dist: pytest==7.3.0 ; extra == "test"
+Requires-Dist: ansys-sphinx-theme==0.9.8 ; extra == "doc"
+Requires-Dist: sphinx-copybutton==0.5.2 ; extra == "doc"
+Requires-Dist: pytest==7.3.1 ; extra == "test"
 Requires-Dist: pytest-cov==4.0.0 ; extra == "test"
 Project-URL: Documentation, https://path.tools.docs.pyansys.com
 Project-URL: Homepage, https://github.com/pyansys/ansys-tools-path
 Project-URL: Source, https://github.com/pyansys/ansys-tools-path
 Project-URL: Tracker, https://github.com/pyansys/ansys-tools-path/issues
 Provides-Extra: build
 Provides-Extra: doc
```

