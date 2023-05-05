# Comparing `tmp/ghastoolkit-0.2.1.tar.gz` & `tmp/ghastoolkit-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ghastoolkit-0.2.1.tar", last modified: Thu May  4 14:16:07 2023, max compression
+gzip compressed data, was "ghastoolkit-0.2.2.tar", last modified: Fri May  5 17:06:18 2023, max compression
```

## Comparing `ghastoolkit-0.2.1.tar` & `ghastoolkit-0.2.2.tar`

### file list

```diff
@@ -1,46 +1,46 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 14:16:07.204547 ghastoolkit-0.2.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-05-04 14:15:38.000000 ghastoolkit-0.2.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2034 2023-05-04 14:16:07.204547 ghastoolkit-0.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1344 2023-05-04 14:15:38.000000 ghastoolkit-0.2.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      929 2023-05-04 14:15:38.000000 ghastoolkit-0.2.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-04 14:16:07.204547 ghastoolkit-0.2.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 14:16:07.200547 ghastoolkit-0.2.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 14:16:07.200547 ghastoolkit-0.2.1/src/ghastoolkit/
--rw-r--r--   0 runner    (1001) docker     (123)     1456 2023-05-04 14:15:38.000000 ghastoolkit-0.2.1/src/ghastoolkit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2756 2023-05-04 14:15:38.000000 ghastoolkit-0.2.1/src/ghastoolkit/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 14:16:07.204547 ghastoolkit-0.2.1/src/ghastoolkit/codeql/
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-04 14:15:38.000000 ghastoolkit-0.2.1/src/ghastoolkit/codeql/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      268 2023-05-04 14:15:38.000000 ghastoolkit-0.2.1/src/ghastoolkit/codeql/consts.py
--rw-r--r--   0 runner    (1001) docker     (123)     8022 2023-05-04 14:15:38.000000 ghastoolkit-0.2.1/src/ghastoolkit/codeql/databases.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 14:16:07.204547 ghastoolkit-0.2.1/src/ghastoolkit/octokit/
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-04 14:15:38.000000 ghastoolkit-0.2.1/src/ghastoolkit/octokit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6692 2023-05-04 14:15:38.000000 ghastoolkit-0.2.1/src/ghastoolkit/octokit/codescanning.py
--rw-r--r--   0 runner    (1001) docker     (123)     2132 2023-05-04 14:15:38.000000 ghastoolkit-0.2.1/src/ghastoolkit/octokit/dependabot.py
--rw-r--r--   0 runner    (1001) docker     (123)     4135 2023-05-04 14:15:38.000000 ghastoolkit-0.2.1/src/ghastoolkit/octokit/dependencygraph.py
--rw-r--r--   0 runner    (1001) docker     (123)     7235 2023-05-04 14:15:38.000000 ghastoolkit-0.2.1/src/ghastoolkit/octokit/github.py
--rw-r--r--   0 runner    (1001) docker     (123)    10920 2023-05-04 14:15:38.000000 ghastoolkit-0.2.1/src/ghastoolkit/octokit/octokit.py
--rw-r--r--   0 runner    (1001) docker     (123)     3763 2023-05-04 14:15:38.000000 ghastoolkit-0.2.1/src/ghastoolkit/octokit/secretscanning.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 14:16:07.204547 ghastoolkit-0.2.1/src/ghastoolkit/secretscanning/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 14:15:38.000000 ghastoolkit-0.2.1/src/ghastoolkit/secretscanning/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1145 2023-05-04 14:15:38.000000 ghastoolkit-0.2.1/src/ghastoolkit/secretscanning/secretalerts.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 14:16:07.204547 ghastoolkit-0.2.1/src/ghastoolkit/supplychain/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 14:15:38.000000 ghastoolkit-0.2.1/src/ghastoolkit/supplychain/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      307 2023-05-04 14:15:38.000000 ghastoolkit-0.2.1/src/ghastoolkit/supplychain/advisories.py
--rw-r--r--   0 runner    (1001) docker     (123)     5553 2023-05-04 14:15:38.000000 ghastoolkit-0.2.1/src/ghastoolkit/supplychain/dependencies.py
--rw-r--r--   0 runner    (1001) docker     (123)      805 2023-05-04 14:15:38.000000 ghastoolkit-0.2.1/src/ghastoolkit/supplychain/dependencyalert.py
--rw-r--r--   0 runner    (1001) docker     (123)     3419 2023-05-04 14:15:38.000000 ghastoolkit-0.2.1/src/ghastoolkit/supplychain/licensing.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 14:16:07.200547 ghastoolkit-0.2.1/src/ghastoolkit.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2034 2023-05-04 14:16:07.000000 ghastoolkit-0.2.1/src/ghastoolkit.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1148 2023-05-04 14:16:07.000000 ghastoolkit-0.2.1/src/ghastoolkit.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-04 14:16:07.000000 ghastoolkit-0.2.1/src/ghastoolkit.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      118 2023-05-04 14:16:07.000000 ghastoolkit-0.2.1/src/ghastoolkit.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-04 14:16:07.000000 ghastoolkit-0.2.1/src/ghastoolkit.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 14:16:07.204547 ghastoolkit-0.2.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      619 2023-05-04 14:15:38.000000 ghastoolkit-0.2.1/tests/test_codeqldb.py
--rw-r--r--   0 runner    (1001) docker     (123)      686 2023-05-04 14:15:38.000000 ghastoolkit-0.2.1/tests/test_codescanning.py
--rw-r--r--   0 runner    (1001) docker     (123)      646 2023-05-04 14:15:38.000000 ghastoolkit-0.2.1/tests/test_default.py
--rw-r--r--   0 runner    (1001) docker     (123)     3563 2023-05-04 14:15:38.000000 ghastoolkit-0.2.1/tests/test_depgraph.py
--rw-r--r--   0 runner    (1001) docker     (123)     3551 2023-05-04 14:15:38.000000 ghastoolkit-0.2.1/tests/test_github.py
--rw-r--r--   0 runner    (1001) docker     (123)      900 2023-05-04 14:15:38.000000 ghastoolkit-0.2.1/tests/test_licenses.py
--rw-r--r--   0 runner    (1001) docker     (123)      950 2023-05-04 14:15:38.000000 ghastoolkit-0.2.1/tests/test_octokit.py
--rw-r--r--   0 runner    (1001) docker     (123)     1359 2023-05-04 14:15:38.000000 ghastoolkit-0.2.1/tests/test_secretscanning.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 17:06:18.938242 ghastoolkit-0.2.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-05-05 17:05:50.000000 ghastoolkit-0.2.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2034 2023-05-05 17:06:18.938242 ghastoolkit-0.2.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1344 2023-05-05 17:05:50.000000 ghastoolkit-0.2.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      929 2023-05-05 17:05:50.000000 ghastoolkit-0.2.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-05 17:06:18.938242 ghastoolkit-0.2.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 17:06:18.934242 ghastoolkit-0.2.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 17:06:18.934242 ghastoolkit-0.2.2/src/ghastoolkit/
+-rw-r--r--   0 runner    (1001) docker     (123)     1456 2023-05-05 17:05:50.000000 ghastoolkit-0.2.2/src/ghastoolkit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2756 2023-05-05 17:05:50.000000 ghastoolkit-0.2.2/src/ghastoolkit/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 17:06:18.938242 ghastoolkit-0.2.2/src/ghastoolkit/codeql/
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-05 17:05:50.000000 ghastoolkit-0.2.2/src/ghastoolkit/codeql/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      268 2023-05-05 17:05:50.000000 ghastoolkit-0.2.2/src/ghastoolkit/codeql/consts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8022 2023-05-05 17:05:50.000000 ghastoolkit-0.2.2/src/ghastoolkit/codeql/databases.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 17:06:18.938242 ghastoolkit-0.2.2/src/ghastoolkit/octokit/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 17:05:50.000000 ghastoolkit-0.2.2/src/ghastoolkit/octokit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6692 2023-05-05 17:05:50.000000 ghastoolkit-0.2.2/src/ghastoolkit/octokit/codescanning.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2132 2023-05-05 17:05:50.000000 ghastoolkit-0.2.2/src/ghastoolkit/octokit/dependabot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4379 2023-05-05 17:05:50.000000 ghastoolkit-0.2.2/src/ghastoolkit/octokit/dependencygraph.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7235 2023-05-05 17:05:50.000000 ghastoolkit-0.2.2/src/ghastoolkit/octokit/github.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10920 2023-05-05 17:05:50.000000 ghastoolkit-0.2.2/src/ghastoolkit/octokit/octokit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3763 2023-05-05 17:05:50.000000 ghastoolkit-0.2.2/src/ghastoolkit/octokit/secretscanning.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 17:06:18.938242 ghastoolkit-0.2.2/src/ghastoolkit/secretscanning/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 17:05:50.000000 ghastoolkit-0.2.2/src/ghastoolkit/secretscanning/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1145 2023-05-05 17:05:50.000000 ghastoolkit-0.2.2/src/ghastoolkit/secretscanning/secretalerts.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 17:06:18.938242 ghastoolkit-0.2.2/src/ghastoolkit/supplychain/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 17:05:50.000000 ghastoolkit-0.2.2/src/ghastoolkit/supplychain/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      307 2023-05-05 17:05:50.000000 ghastoolkit-0.2.2/src/ghastoolkit/supplychain/advisories.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5553 2023-05-05 17:05:50.000000 ghastoolkit-0.2.2/src/ghastoolkit/supplychain/dependencies.py
+-rw-r--r--   0 runner    (1001) docker     (123)      805 2023-05-05 17:05:50.000000 ghastoolkit-0.2.2/src/ghastoolkit/supplychain/dependencyalert.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3419 2023-05-05 17:05:50.000000 ghastoolkit-0.2.2/src/ghastoolkit/supplychain/licensing.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 17:06:18.934242 ghastoolkit-0.2.2/src/ghastoolkit.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2034 2023-05-05 17:06:18.000000 ghastoolkit-0.2.2/src/ghastoolkit.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1148 2023-05-05 17:06:18.000000 ghastoolkit-0.2.2/src/ghastoolkit.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 17:06:18.000000 ghastoolkit-0.2.2/src/ghastoolkit.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      118 2023-05-05 17:06:18.000000 ghastoolkit-0.2.2/src/ghastoolkit.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-05 17:06:18.000000 ghastoolkit-0.2.2/src/ghastoolkit.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 17:06:18.938242 ghastoolkit-0.2.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      619 2023-05-05 17:05:50.000000 ghastoolkit-0.2.2/tests/test_codeqldb.py
+-rw-r--r--   0 runner    (1001) docker     (123)      686 2023-05-05 17:05:50.000000 ghastoolkit-0.2.2/tests/test_codescanning.py
+-rw-r--r--   0 runner    (1001) docker     (123)      646 2023-05-05 17:05:50.000000 ghastoolkit-0.2.2/tests/test_default.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3563 2023-05-05 17:05:50.000000 ghastoolkit-0.2.2/tests/test_depgraph.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3551 2023-05-05 17:05:50.000000 ghastoolkit-0.2.2/tests/test_github.py
+-rw-r--r--   0 runner    (1001) docker     (123)      900 2023-05-05 17:05:50.000000 ghastoolkit-0.2.2/tests/test_licenses.py
+-rw-r--r--   0 runner    (1001) docker     (123)      950 2023-05-05 17:05:50.000000 ghastoolkit-0.2.2/tests/test_octokit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1359 2023-05-05 17:05:50.000000 ghastoolkit-0.2.2/tests/test_secretscanning.py
```

### Comparing `ghastoolkit-0.2.1/LICENSE` & `ghastoolkit-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.2.1/PKG-INFO` & `ghastoolkit-0.2.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ghastoolkit
-Version: 0.2.1
+Version: 0.2.2
 Summary: GitHub Advanced Security Python Toolkit
 Author: GeekMasher
 Project-URL: Homepage, https://github.com/GeekMasher/ghastoolkit
 Project-URL: Bug Tracker, https://github.com/GeekMasher/ghastoolkit/issues
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `ghastoolkit-0.2.1/README.md` & `ghastoolkit-0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.2.1/pyproject.toml` & `ghastoolkit-0.2.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "ghastoolkit"
-version = "0.2.1"
+version = "0.2.2"
 authors = [
   { name="GeekMasher" },
 ]
 description = "GitHub Advanced Security Python Toolkit"
 readme = "README.md"
 requires-python = ">=3.9"
 classifiers = [
```

### Comparing `ghastoolkit-0.2.1/src/ghastoolkit/__init__.py` & `ghastoolkit-0.2.2/src/ghastoolkit/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 __name__ = "ghastoolkit"
 __title__ = "GHAS Toolkit"
 
-__version__ = "0.2.1"
+__version__ = "0.2.2"
 
 __description__ = "GitHub Advanced Security Python Toolkit"
 __summary__ = """\
 GitHub Advanced Security Python Toolkit
 """
 
 __url__ = "https://github.com/GeekMasher/ghastoolkit"
```

### Comparing `ghastoolkit-0.2.1/src/ghastoolkit/__main__.py` & `ghastoolkit-0.2.2/src/ghastoolkit/__main__.py`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.2.1/src/ghastoolkit/codeql/databases.py` & `ghastoolkit-0.2.2/src/ghastoolkit/codeql/databases.py`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.2.1/src/ghastoolkit/octokit/codescanning.py` & `ghastoolkit-0.2.2/src/ghastoolkit/octokit/codescanning.py`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.2.1/src/ghastoolkit/octokit/dependabot.py` & `ghastoolkit-0.2.2/src/ghastoolkit/octokit/dependabot.py`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.2.1/src/ghastoolkit/octokit/dependencygraph.py` & `ghastoolkit-0.2.2/src/ghastoolkit/octokit/dependencygraph.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 import logging
 from dataclasses import dataclass, field
 from datetime import datetime
 import re
+from typing import Any
 import urllib.parse
 
 from ghastoolkit.octokit.github import GitHub, Repository
 from ghastoolkit.supplychain.advisories import Advisory
 from ghastoolkit.supplychain.dependencyalert import DependencyAlert
 from ghastoolkit.supplychain.dependencies import Dependencies, Dependency
 from ghastoolkit.octokit.octokit import GraphQLRequest, Optional, RestRequest
@@ -109,7 +110,15 @@
         https://docs.github.com/en/rest/dependency-graph/dependency-submission?apiVersion=2022-11-28#create-a-snapshot-of-dependencies-for-a-repository
         """
         self.rest.postJson(
             "/repos/{owner}/{repo}/dependency-graph/snapshots",
             dependencies.exportBOM(tool, path, sha, ref, version, url),
             expected=201,
         )
+
+    def submitSbom(self, sbom: dict[Any, Any]):
+        """Submit SBOM"""
+        self.rest.postJson(
+            "/repos/{owner}/{repo}/dependency-graph/snapshots",
+            sbom,
+            expected=201,
+        )
```

### Comparing `ghastoolkit-0.2.1/src/ghastoolkit/octokit/github.py` & `ghastoolkit-0.2.2/src/ghastoolkit/octokit/github.py`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.2.1/src/ghastoolkit/octokit/octokit.py` & `ghastoolkit-0.2.2/src/ghastoolkit/octokit/octokit.py`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.2.1/src/ghastoolkit/octokit/secretscanning.py` & `ghastoolkit-0.2.2/src/ghastoolkit/octokit/secretscanning.py`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.2.1/src/ghastoolkit/secretscanning/secretalerts.py` & `ghastoolkit-0.2.2/src/ghastoolkit/secretscanning/secretalerts.py`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.2.1/src/ghastoolkit/supplychain/dependencies.py` & `ghastoolkit-0.2.2/src/ghastoolkit/supplychain/dependencies.py`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.2.1/src/ghastoolkit/supplychain/dependencyalert.py` & `ghastoolkit-0.2.2/src/ghastoolkit/supplychain/dependencyalert.py`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.2.1/src/ghastoolkit/supplychain/licensing.py` & `ghastoolkit-0.2.2/src/ghastoolkit/supplychain/licensing.py`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.2.1/src/ghastoolkit.egg-info/PKG-INFO` & `ghastoolkit-0.2.2/src/ghastoolkit.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ghastoolkit
-Version: 0.2.1
+Version: 0.2.2
 Summary: GitHub Advanced Security Python Toolkit
 Author: GeekMasher
 Project-URL: Homepage, https://github.com/GeekMasher/ghastoolkit
 Project-URL: Bug Tracker, https://github.com/GeekMasher/ghastoolkit/issues
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `ghastoolkit-0.2.1/src/ghastoolkit.egg-info/SOURCES.txt` & `ghastoolkit-0.2.2/src/ghastoolkit.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.2.1/tests/test_codeqldb.py` & `ghastoolkit-0.2.2/tests/test_codeqldb.py`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.2.1/tests/test_codescanning.py` & `ghastoolkit-0.2.2/tests/test_codescanning.py`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.2.1/tests/test_default.py` & `ghastoolkit-0.2.2/tests/test_default.py`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.2.1/tests/test_depgraph.py` & `ghastoolkit-0.2.2/tests/test_depgraph.py`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.2.1/tests/test_github.py` & `ghastoolkit-0.2.2/tests/test_github.py`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.2.1/tests/test_licenses.py` & `ghastoolkit-0.2.2/tests/test_licenses.py`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.2.1/tests/test_octokit.py` & `ghastoolkit-0.2.2/tests/test_octokit.py`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.2.1/tests/test_secretscanning.py` & `ghastoolkit-0.2.2/tests/test_secretscanning.py`

 * *Files identical despite different names*

