# Comparing `tmp/ghastoolkit-0.2.3.tar.gz` & `tmp/ghastoolkit-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ghastoolkit-0.2.3.tar", last modified: Fri May  5 20:44:34 2023, max compression
+gzip compressed data, was "ghastoolkit-0.2.4.tar", last modified: Fri May  5 21:07:04 2023, max compression
```

## Comparing `ghastoolkit-0.2.3.tar` & `ghastoolkit-0.2.4.tar`

### file list

```diff
@@ -1,48 +1,48 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 20:44:34.481244 ghastoolkit-0.2.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-05-05 20:43:57.000000 ghastoolkit-0.2.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2034 2023-05-05 20:44:34.481244 ghastoolkit-0.2.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1344 2023-05-05 20:43:57.000000 ghastoolkit-0.2.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      929 2023-05-05 20:43:57.000000 ghastoolkit-0.2.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-05 20:44:34.481244 ghastoolkit-0.2.3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 20:44:34.473243 ghastoolkit-0.2.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 20:44:34.473243 ghastoolkit-0.2.3/src/ghastoolkit/
--rw-r--r--   0 runner    (1001) docker     (123)     1456 2023-05-05 20:43:57.000000 ghastoolkit-0.2.3/src/ghastoolkit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2756 2023-05-05 20:43:57.000000 ghastoolkit-0.2.3/src/ghastoolkit/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 20:44:34.477244 ghastoolkit-0.2.3/src/ghastoolkit/codeql/
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-05 20:43:57.000000 ghastoolkit-0.2.3/src/ghastoolkit/codeql/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      268 2023-05-05 20:43:57.000000 ghastoolkit-0.2.3/src/ghastoolkit/codeql/consts.py
--rw-r--r--   0 runner    (1001) docker     (123)     8022 2023-05-05 20:43:57.000000 ghastoolkit-0.2.3/src/ghastoolkit/codeql/databases.py
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-05-05 20:43:57.000000 ghastoolkit-0.2.3/src/ghastoolkit/codeql/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 20:44:34.477244 ghastoolkit-0.2.3/src/ghastoolkit/octokit/
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 20:43:57.000000 ghastoolkit-0.2.3/src/ghastoolkit/octokit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6692 2023-05-05 20:43:57.000000 ghastoolkit-0.2.3/src/ghastoolkit/octokit/codescanning.py
--rw-r--r--   0 runner    (1001) docker     (123)     2098 2023-05-05 20:43:57.000000 ghastoolkit-0.2.3/src/ghastoolkit/octokit/dependabot.py
--rw-r--r--   0 runner    (1001) docker     (123)     4379 2023-05-05 20:43:57.000000 ghastoolkit-0.2.3/src/ghastoolkit/octokit/dependencygraph.py
--rw-r--r--   0 runner    (1001) docker     (123)     7235 2023-05-05 20:43:57.000000 ghastoolkit-0.2.3/src/ghastoolkit/octokit/github.py
--rw-r--r--   0 runner    (1001) docker     (123)    10968 2023-05-05 20:43:57.000000 ghastoolkit-0.2.3/src/ghastoolkit/octokit/octokit.py
--rw-r--r--   0 runner    (1001) docker     (123)     3763 2023-05-05 20:43:57.000000 ghastoolkit-0.2.3/src/ghastoolkit/octokit/secretscanning.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 20:44:34.477244 ghastoolkit-0.2.3/src/ghastoolkit/secretscanning/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 20:43:57.000000 ghastoolkit-0.2.3/src/ghastoolkit/secretscanning/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1145 2023-05-05 20:43:57.000000 ghastoolkit-0.2.3/src/ghastoolkit/secretscanning/secretalerts.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 20:44:34.477244 ghastoolkit-0.2.3/src/ghastoolkit/supplychain/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 20:43:57.000000 ghastoolkit-0.2.3/src/ghastoolkit/supplychain/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      307 2023-05-05 20:43:57.000000 ghastoolkit-0.2.3/src/ghastoolkit/supplychain/advisories.py
--rw-r--r--   0 runner    (1001) docker     (123)     5684 2023-05-05 20:43:57.000000 ghastoolkit-0.2.3/src/ghastoolkit/supplychain/dependencies.py
--rw-r--r--   0 runner    (1001) docker     (123)      805 2023-05-05 20:43:57.000000 ghastoolkit-0.2.3/src/ghastoolkit/supplychain/dependencyalert.py
--rw-r--r--   0 runner    (1001) docker     (123)     4428 2023-05-05 20:43:57.000000 ghastoolkit-0.2.3/src/ghastoolkit/supplychain/licensing.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 20:44:34.477244 ghastoolkit-0.2.3/src/ghastoolkit.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2034 2023-05-05 20:44:34.000000 ghastoolkit-0.2.3/src/ghastoolkit.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1207 2023-05-05 20:44:34.000000 ghastoolkit-0.2.3/src/ghastoolkit.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 20:44:34.000000 ghastoolkit-0.2.3/src/ghastoolkit.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      118 2023-05-05 20:44:34.000000 ghastoolkit-0.2.3/src/ghastoolkit.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-05 20:44:34.000000 ghastoolkit-0.2.3/src/ghastoolkit.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 20:44:34.481244 ghastoolkit-0.2.3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      619 2023-05-05 20:43:57.000000 ghastoolkit-0.2.3/tests/test_codeqldb.py
--rw-r--r--   0 runner    (1001) docker     (123)      686 2023-05-05 20:43:57.000000 ghastoolkit-0.2.3/tests/test_codescanning.py
--rw-r--r--   0 runner    (1001) docker     (123)      646 2023-05-05 20:43:57.000000 ghastoolkit-0.2.3/tests/test_default.py
--rw-r--r--   0 runner    (1001) docker     (123)     2078 2023-05-05 20:43:57.000000 ghastoolkit-0.2.3/tests/test_dependencies.py
--rw-r--r--   0 runner    (1001) docker     (123)     2163 2023-05-05 20:43:57.000000 ghastoolkit-0.2.3/tests/test_depgraph.py
--rw-r--r--   0 runner    (1001) docker     (123)     3551 2023-05-05 20:43:57.000000 ghastoolkit-0.2.3/tests/test_github.py
--rw-r--r--   0 runner    (1001) docker     (123)      900 2023-05-05 20:43:57.000000 ghastoolkit-0.2.3/tests/test_licenses.py
--rw-r--r--   0 runner    (1001) docker     (123)      950 2023-05-05 20:43:57.000000 ghastoolkit-0.2.3/tests/test_octokit.py
--rw-r--r--   0 runner    (1001) docker     (123)     1359 2023-05-05 20:43:57.000000 ghastoolkit-0.2.3/tests/test_secretscanning.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 21:07:04.553689 ghastoolkit-0.2.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-05-05 21:06:35.000000 ghastoolkit-0.2.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2034 2023-05-05 21:07:04.553689 ghastoolkit-0.2.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1344 2023-05-05 21:06:35.000000 ghastoolkit-0.2.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      929 2023-05-05 21:06:35.000000 ghastoolkit-0.2.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-05 21:07:04.553689 ghastoolkit-0.2.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 21:07:04.549689 ghastoolkit-0.2.4/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 21:07:04.549689 ghastoolkit-0.2.4/src/ghastoolkit/
+-rw-r--r--   0 runner    (1001) docker     (123)     1456 2023-05-05 21:06:35.000000 ghastoolkit-0.2.4/src/ghastoolkit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2756 2023-05-05 21:06:35.000000 ghastoolkit-0.2.4/src/ghastoolkit/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 21:07:04.549689 ghastoolkit-0.2.4/src/ghastoolkit/codeql/
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-05 21:06:35.000000 ghastoolkit-0.2.4/src/ghastoolkit/codeql/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      268 2023-05-05 21:06:35.000000 ghastoolkit-0.2.4/src/ghastoolkit/codeql/consts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8022 2023-05-05 21:06:35.000000 ghastoolkit-0.2.4/src/ghastoolkit/codeql/databases.py
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-05-05 21:06:35.000000 ghastoolkit-0.2.4/src/ghastoolkit/codeql/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 21:07:04.549689 ghastoolkit-0.2.4/src/ghastoolkit/octokit/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 21:06:35.000000 ghastoolkit-0.2.4/src/ghastoolkit/octokit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6692 2023-05-05 21:06:35.000000 ghastoolkit-0.2.4/src/ghastoolkit/octokit/codescanning.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2098 2023-05-05 21:06:35.000000 ghastoolkit-0.2.4/src/ghastoolkit/octokit/dependabot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4379 2023-05-05 21:06:35.000000 ghastoolkit-0.2.4/src/ghastoolkit/octokit/dependencygraph.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7235 2023-05-05 21:06:35.000000 ghastoolkit-0.2.4/src/ghastoolkit/octokit/github.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10968 2023-05-05 21:06:35.000000 ghastoolkit-0.2.4/src/ghastoolkit/octokit/octokit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3763 2023-05-05 21:06:35.000000 ghastoolkit-0.2.4/src/ghastoolkit/octokit/secretscanning.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 21:07:04.553689 ghastoolkit-0.2.4/src/ghastoolkit/secretscanning/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 21:06:35.000000 ghastoolkit-0.2.4/src/ghastoolkit/secretscanning/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1145 2023-05-05 21:06:35.000000 ghastoolkit-0.2.4/src/ghastoolkit/secretscanning/secretalerts.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 21:07:04.553689 ghastoolkit-0.2.4/src/ghastoolkit/supplychain/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 21:06:35.000000 ghastoolkit-0.2.4/src/ghastoolkit/supplychain/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      307 2023-05-05 21:06:35.000000 ghastoolkit-0.2.4/src/ghastoolkit/supplychain/advisories.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5684 2023-05-05 21:06:35.000000 ghastoolkit-0.2.4/src/ghastoolkit/supplychain/dependencies.py
+-rw-r--r--   0 runner    (1001) docker     (123)      805 2023-05-05 21:06:35.000000 ghastoolkit-0.2.4/src/ghastoolkit/supplychain/dependencyalert.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4452 2023-05-05 21:06:35.000000 ghastoolkit-0.2.4/src/ghastoolkit/supplychain/licensing.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 21:07:04.549689 ghastoolkit-0.2.4/src/ghastoolkit.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2034 2023-05-05 21:07:04.000000 ghastoolkit-0.2.4/src/ghastoolkit.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1207 2023-05-05 21:07:04.000000 ghastoolkit-0.2.4/src/ghastoolkit.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 21:07:04.000000 ghastoolkit-0.2.4/src/ghastoolkit.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      118 2023-05-05 21:07:04.000000 ghastoolkit-0.2.4/src/ghastoolkit.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-05 21:07:04.000000 ghastoolkit-0.2.4/src/ghastoolkit.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 21:07:04.553689 ghastoolkit-0.2.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      619 2023-05-05 21:06:35.000000 ghastoolkit-0.2.4/tests/test_codeqldb.py
+-rw-r--r--   0 runner    (1001) docker     (123)      686 2023-05-05 21:06:35.000000 ghastoolkit-0.2.4/tests/test_codescanning.py
+-rw-r--r--   0 runner    (1001) docker     (123)      646 2023-05-05 21:06:35.000000 ghastoolkit-0.2.4/tests/test_default.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2078 2023-05-05 21:06:35.000000 ghastoolkit-0.2.4/tests/test_dependencies.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2163 2023-05-05 21:06:35.000000 ghastoolkit-0.2.4/tests/test_depgraph.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3551 2023-05-05 21:06:35.000000 ghastoolkit-0.2.4/tests/test_github.py
+-rw-r--r--   0 runner    (1001) docker     (123)      900 2023-05-05 21:06:35.000000 ghastoolkit-0.2.4/tests/test_licenses.py
+-rw-r--r--   0 runner    (1001) docker     (123)      950 2023-05-05 21:06:35.000000 ghastoolkit-0.2.4/tests/test_octokit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1359 2023-05-05 21:06:35.000000 ghastoolkit-0.2.4/tests/test_secretscanning.py
```

### Comparing `ghastoolkit-0.2.3/LICENSE` & `ghastoolkit-0.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.2.3/PKG-INFO` & `ghastoolkit-0.2.4/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ghastoolkit
-Version: 0.2.3
+Version: 0.2.4
 Summary: GitHub Advanced Security Python Toolkit
 Author: GeekMasher
 Project-URL: Homepage, https://github.com/GeekMasher/ghastoolkit
 Project-URL: Bug Tracker, https://github.com/GeekMasher/ghastoolkit/issues
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `ghastoolkit-0.2.3/README.md` & `ghastoolkit-0.2.4/README.md`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.2.3/pyproject.toml` & `ghastoolkit-0.2.4/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "ghastoolkit"
-version = "0.2.3"
+version = "0.2.4"
 authors = [
   { name="GeekMasher" },
 ]
 description = "GitHub Advanced Security Python Toolkit"
 readme = "README.md"
 requires-python = ">=3.9"
 classifiers = [
```

### Comparing `ghastoolkit-0.2.3/src/ghastoolkit/__init__.py` & `ghastoolkit-0.2.4/src/ghastoolkit/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 __name__ = "ghastoolkit"
 __title__ = "GHAS Toolkit"
 
-__version__ = "0.2.3"
+__version__ = "0.2.4"
 
 __description__ = "GitHub Advanced Security Python Toolkit"
 __summary__ = """\
 GitHub Advanced Security Python Toolkit
 """
 
 __url__ = "https://github.com/GeekMasher/ghastoolkit"
```

### Comparing `ghastoolkit-0.2.3/src/ghastoolkit/__main__.py` & `ghastoolkit-0.2.4/src/ghastoolkit/__main__.py`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.2.3/src/ghastoolkit/codeql/databases.py` & `ghastoolkit-0.2.4/src/ghastoolkit/codeql/databases.py`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.2.3/src/ghastoolkit/octokit/codescanning.py` & `ghastoolkit-0.2.4/src/ghastoolkit/octokit/codescanning.py`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.2.3/src/ghastoolkit/octokit/dependabot.py` & `ghastoolkit-0.2.4/src/ghastoolkit/octokit/dependabot.py`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.2.3/src/ghastoolkit/octokit/dependencygraph.py` & `ghastoolkit-0.2.4/src/ghastoolkit/octokit/dependencygraph.py`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.2.3/src/ghastoolkit/octokit/github.py` & `ghastoolkit-0.2.4/src/ghastoolkit/octokit/github.py`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.2.3/src/ghastoolkit/octokit/octokit.py` & `ghastoolkit-0.2.4/src/ghastoolkit/octokit/octokit.py`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.2.3/src/ghastoolkit/octokit/secretscanning.py` & `ghastoolkit-0.2.4/src/ghastoolkit/octokit/secretscanning.py`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.2.3/src/ghastoolkit/secretscanning/secretalerts.py` & `ghastoolkit-0.2.4/src/ghastoolkit/secretscanning/secretalerts.py`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.2.3/src/ghastoolkit/supplychain/dependencies.py` & `ghastoolkit-0.2.4/src/ghastoolkit/supplychain/dependencies.py`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.2.3/src/ghastoolkit/supplychain/dependencyalert.py` & `ghastoolkit-0.2.4/src/ghastoolkit/supplychain/dependencyalert.py`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.2.3/src/ghastoolkit/supplychain/licensing.py` & `ghastoolkit-0.2.4/src/ghastoolkit/supplychain/licensing.py`

 * *Files 2% similar despite different names*

```diff
@@ -28,16 +28,18 @@
         if not os.path.exists(path):
             raise Exception(f"License path does not exist: {path}")
         if not os.path.isfile(path):
             raise Exception("Path provided needs to be a file")
 
         logger.debug(f"Loading licenseing file :: {path}")
         with open(path, "r") as handle:
+            data = json.load(handle)
             # TODO validate the data before loading?
-            self.data = json.load(handle)
+
+        self.data.update(data)
 
         self.sources.append(path)
         logger.debug(f"Loaded licenses :: {len(self.data)}")
 
     def add(self, purl: str, licenses: str | list):
         """Add license"""
         if self.data.get(purl):
@@ -67,15 +69,15 @@
     def __len__(self) -> int:
         return len(self.data)
 
 
 if __name__ == "__main__":
     import yaml
     import argparse
-    from ghastoolkit.octokit.github import Repository
+    from ghastoolkit import Repository, Dependency
 
     logging.basicConfig(
         level=logging.DEBUG,
         format="%(asctime)s - %(name)s - %(levelname)s - %(message)s",
     )
     parser = argparse.ArgumentParser("ghastoolkit.supplychain.licenses")
     parser.add_argument("-o", "--output", help="Output")
```

### Comparing `ghastoolkit-0.2.3/src/ghastoolkit.egg-info/PKG-INFO` & `ghastoolkit-0.2.4/src/ghastoolkit.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ghastoolkit
-Version: 0.2.3
+Version: 0.2.4
 Summary: GitHub Advanced Security Python Toolkit
 Author: GeekMasher
 Project-URL: Homepage, https://github.com/GeekMasher/ghastoolkit
 Project-URL: Bug Tracker, https://github.com/GeekMasher/ghastoolkit/issues
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `ghastoolkit-0.2.3/src/ghastoolkit.egg-info/SOURCES.txt` & `ghastoolkit-0.2.4/src/ghastoolkit.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.2.3/tests/test_codeqldb.py` & `ghastoolkit-0.2.4/tests/test_codeqldb.py`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.2.3/tests/test_codescanning.py` & `ghastoolkit-0.2.4/tests/test_codescanning.py`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.2.3/tests/test_default.py` & `ghastoolkit-0.2.4/tests/test_default.py`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.2.3/tests/test_dependencies.py` & `ghastoolkit-0.2.4/tests/test_dependencies.py`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.2.3/tests/test_depgraph.py` & `ghastoolkit-0.2.4/tests/test_depgraph.py`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.2.3/tests/test_github.py` & `ghastoolkit-0.2.4/tests/test_github.py`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.2.3/tests/test_licenses.py` & `ghastoolkit-0.2.4/tests/test_licenses.py`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.2.3/tests/test_octokit.py` & `ghastoolkit-0.2.4/tests/test_octokit.py`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.2.3/tests/test_secretscanning.py` & `ghastoolkit-0.2.4/tests/test_secretscanning.py`

 * *Files identical despite different names*

