# Comparing `tmp/ghastoolkit-0.2.2.tar.gz` & `tmp/ghastoolkit-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ghastoolkit-0.2.2.tar", last modified: Fri May  5 17:06:18 2023, max compression
+gzip compressed data, was "ghastoolkit-0.2.3.tar", last modified: Fri May  5 20:44:34 2023, max compression
```

## Comparing `ghastoolkit-0.2.2.tar` & `ghastoolkit-0.2.3.tar`

### file list

```diff
@@ -1,46 +1,48 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 17:06:18.938242 ghastoolkit-0.2.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-05-05 17:05:50.000000 ghastoolkit-0.2.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2034 2023-05-05 17:06:18.938242 ghastoolkit-0.2.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1344 2023-05-05 17:05:50.000000 ghastoolkit-0.2.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      929 2023-05-05 17:05:50.000000 ghastoolkit-0.2.2/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-05 17:06:18.938242 ghastoolkit-0.2.2/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 17:06:18.934242 ghastoolkit-0.2.2/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 17:06:18.934242 ghastoolkit-0.2.2/src/ghastoolkit/
--rw-r--r--   0 runner    (1001) docker     (123)     1456 2023-05-05 17:05:50.000000 ghastoolkit-0.2.2/src/ghastoolkit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2756 2023-05-05 17:05:50.000000 ghastoolkit-0.2.2/src/ghastoolkit/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 17:06:18.938242 ghastoolkit-0.2.2/src/ghastoolkit/codeql/
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-05 17:05:50.000000 ghastoolkit-0.2.2/src/ghastoolkit/codeql/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      268 2023-05-05 17:05:50.000000 ghastoolkit-0.2.2/src/ghastoolkit/codeql/consts.py
--rw-r--r--   0 runner    (1001) docker     (123)     8022 2023-05-05 17:05:50.000000 ghastoolkit-0.2.2/src/ghastoolkit/codeql/databases.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 17:06:18.938242 ghastoolkit-0.2.2/src/ghastoolkit/octokit/
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 17:05:50.000000 ghastoolkit-0.2.2/src/ghastoolkit/octokit/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6692 2023-05-05 17:05:50.000000 ghastoolkit-0.2.2/src/ghastoolkit/octokit/codescanning.py
--rw-r--r--   0 runner    (1001) docker     (123)     2132 2023-05-05 17:05:50.000000 ghastoolkit-0.2.2/src/ghastoolkit/octokit/dependabot.py
--rw-r--r--   0 runner    (1001) docker     (123)     4379 2023-05-05 17:05:50.000000 ghastoolkit-0.2.2/src/ghastoolkit/octokit/dependencygraph.py
--rw-r--r--   0 runner    (1001) docker     (123)     7235 2023-05-05 17:05:50.000000 ghastoolkit-0.2.2/src/ghastoolkit/octokit/github.py
--rw-r--r--   0 runner    (1001) docker     (123)    10920 2023-05-05 17:05:50.000000 ghastoolkit-0.2.2/src/ghastoolkit/octokit/octokit.py
--rw-r--r--   0 runner    (1001) docker     (123)     3763 2023-05-05 17:05:50.000000 ghastoolkit-0.2.2/src/ghastoolkit/octokit/secretscanning.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 17:06:18.938242 ghastoolkit-0.2.2/src/ghastoolkit/secretscanning/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 17:05:50.000000 ghastoolkit-0.2.2/src/ghastoolkit/secretscanning/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1145 2023-05-05 17:05:50.000000 ghastoolkit-0.2.2/src/ghastoolkit/secretscanning/secretalerts.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 17:06:18.938242 ghastoolkit-0.2.2/src/ghastoolkit/supplychain/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 17:05:50.000000 ghastoolkit-0.2.2/src/ghastoolkit/supplychain/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      307 2023-05-05 17:05:50.000000 ghastoolkit-0.2.2/src/ghastoolkit/supplychain/advisories.py
--rw-r--r--   0 runner    (1001) docker     (123)     5553 2023-05-05 17:05:50.000000 ghastoolkit-0.2.2/src/ghastoolkit/supplychain/dependencies.py
--rw-r--r--   0 runner    (1001) docker     (123)      805 2023-05-05 17:05:50.000000 ghastoolkit-0.2.2/src/ghastoolkit/supplychain/dependencyalert.py
--rw-r--r--   0 runner    (1001) docker     (123)     3419 2023-05-05 17:05:50.000000 ghastoolkit-0.2.2/src/ghastoolkit/supplychain/licensing.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 17:06:18.934242 ghastoolkit-0.2.2/src/ghastoolkit.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2034 2023-05-05 17:06:18.000000 ghastoolkit-0.2.2/src/ghastoolkit.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1148 2023-05-05 17:06:18.000000 ghastoolkit-0.2.2/src/ghastoolkit.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 17:06:18.000000 ghastoolkit-0.2.2/src/ghastoolkit.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      118 2023-05-05 17:06:18.000000 ghastoolkit-0.2.2/src/ghastoolkit.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-05 17:06:18.000000 ghastoolkit-0.2.2/src/ghastoolkit.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 17:06:18.938242 ghastoolkit-0.2.2/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      619 2023-05-05 17:05:50.000000 ghastoolkit-0.2.2/tests/test_codeqldb.py
--rw-r--r--   0 runner    (1001) docker     (123)      686 2023-05-05 17:05:50.000000 ghastoolkit-0.2.2/tests/test_codescanning.py
--rw-r--r--   0 runner    (1001) docker     (123)      646 2023-05-05 17:05:50.000000 ghastoolkit-0.2.2/tests/test_default.py
--rw-r--r--   0 runner    (1001) docker     (123)     3563 2023-05-05 17:05:50.000000 ghastoolkit-0.2.2/tests/test_depgraph.py
--rw-r--r--   0 runner    (1001) docker     (123)     3551 2023-05-05 17:05:50.000000 ghastoolkit-0.2.2/tests/test_github.py
--rw-r--r--   0 runner    (1001) docker     (123)      900 2023-05-05 17:05:50.000000 ghastoolkit-0.2.2/tests/test_licenses.py
--rw-r--r--   0 runner    (1001) docker     (123)      950 2023-05-05 17:05:50.000000 ghastoolkit-0.2.2/tests/test_octokit.py
--rw-r--r--   0 runner    (1001) docker     (123)     1359 2023-05-05 17:05:50.000000 ghastoolkit-0.2.2/tests/test_secretscanning.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 20:44:34.481244 ghastoolkit-0.2.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-05-05 20:43:57.000000 ghastoolkit-0.2.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2034 2023-05-05 20:44:34.481244 ghastoolkit-0.2.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1344 2023-05-05 20:43:57.000000 ghastoolkit-0.2.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      929 2023-05-05 20:43:57.000000 ghastoolkit-0.2.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-05 20:44:34.481244 ghastoolkit-0.2.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 20:44:34.473243 ghastoolkit-0.2.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 20:44:34.473243 ghastoolkit-0.2.3/src/ghastoolkit/
+-rw-r--r--   0 runner    (1001) docker     (123)     1456 2023-05-05 20:43:57.000000 ghastoolkit-0.2.3/src/ghastoolkit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2756 2023-05-05 20:43:57.000000 ghastoolkit-0.2.3/src/ghastoolkit/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 20:44:34.477244 ghastoolkit-0.2.3/src/ghastoolkit/codeql/
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-05 20:43:57.000000 ghastoolkit-0.2.3/src/ghastoolkit/codeql/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      268 2023-05-05 20:43:57.000000 ghastoolkit-0.2.3/src/ghastoolkit/codeql/consts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8022 2023-05-05 20:43:57.000000 ghastoolkit-0.2.3/src/ghastoolkit/codeql/databases.py
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-05-05 20:43:57.000000 ghastoolkit-0.2.3/src/ghastoolkit/codeql/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 20:44:34.477244 ghastoolkit-0.2.3/src/ghastoolkit/octokit/
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 20:43:57.000000 ghastoolkit-0.2.3/src/ghastoolkit/octokit/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6692 2023-05-05 20:43:57.000000 ghastoolkit-0.2.3/src/ghastoolkit/octokit/codescanning.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2098 2023-05-05 20:43:57.000000 ghastoolkit-0.2.3/src/ghastoolkit/octokit/dependabot.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4379 2023-05-05 20:43:57.000000 ghastoolkit-0.2.3/src/ghastoolkit/octokit/dependencygraph.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7235 2023-05-05 20:43:57.000000 ghastoolkit-0.2.3/src/ghastoolkit/octokit/github.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10968 2023-05-05 20:43:57.000000 ghastoolkit-0.2.3/src/ghastoolkit/octokit/octokit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3763 2023-05-05 20:43:57.000000 ghastoolkit-0.2.3/src/ghastoolkit/octokit/secretscanning.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 20:44:34.477244 ghastoolkit-0.2.3/src/ghastoolkit/secretscanning/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 20:43:57.000000 ghastoolkit-0.2.3/src/ghastoolkit/secretscanning/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1145 2023-05-05 20:43:57.000000 ghastoolkit-0.2.3/src/ghastoolkit/secretscanning/secretalerts.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 20:44:34.477244 ghastoolkit-0.2.3/src/ghastoolkit/supplychain/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 20:43:57.000000 ghastoolkit-0.2.3/src/ghastoolkit/supplychain/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      307 2023-05-05 20:43:57.000000 ghastoolkit-0.2.3/src/ghastoolkit/supplychain/advisories.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5684 2023-05-05 20:43:57.000000 ghastoolkit-0.2.3/src/ghastoolkit/supplychain/dependencies.py
+-rw-r--r--   0 runner    (1001) docker     (123)      805 2023-05-05 20:43:57.000000 ghastoolkit-0.2.3/src/ghastoolkit/supplychain/dependencyalert.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4428 2023-05-05 20:43:57.000000 ghastoolkit-0.2.3/src/ghastoolkit/supplychain/licensing.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 20:44:34.477244 ghastoolkit-0.2.3/src/ghastoolkit.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2034 2023-05-05 20:44:34.000000 ghastoolkit-0.2.3/src/ghastoolkit.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1207 2023-05-05 20:44:34.000000 ghastoolkit-0.2.3/src/ghastoolkit.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 20:44:34.000000 ghastoolkit-0.2.3/src/ghastoolkit.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      118 2023-05-05 20:44:34.000000 ghastoolkit-0.2.3/src/ghastoolkit.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-05 20:44:34.000000 ghastoolkit-0.2.3/src/ghastoolkit.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 20:44:34.481244 ghastoolkit-0.2.3/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      619 2023-05-05 20:43:57.000000 ghastoolkit-0.2.3/tests/test_codeqldb.py
+-rw-r--r--   0 runner    (1001) docker     (123)      686 2023-05-05 20:43:57.000000 ghastoolkit-0.2.3/tests/test_codescanning.py
+-rw-r--r--   0 runner    (1001) docker     (123)      646 2023-05-05 20:43:57.000000 ghastoolkit-0.2.3/tests/test_default.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2078 2023-05-05 20:43:57.000000 ghastoolkit-0.2.3/tests/test_dependencies.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2163 2023-05-05 20:43:57.000000 ghastoolkit-0.2.3/tests/test_depgraph.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3551 2023-05-05 20:43:57.000000 ghastoolkit-0.2.3/tests/test_github.py
+-rw-r--r--   0 runner    (1001) docker     (123)      900 2023-05-05 20:43:57.000000 ghastoolkit-0.2.3/tests/test_licenses.py
+-rw-r--r--   0 runner    (1001) docker     (123)      950 2023-05-05 20:43:57.000000 ghastoolkit-0.2.3/tests/test_octokit.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1359 2023-05-05 20:43:57.000000 ghastoolkit-0.2.3/tests/test_secretscanning.py
```

### Comparing `ghastoolkit-0.2.2/LICENSE` & `ghastoolkit-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.2.2/PKG-INFO` & `ghastoolkit-0.2.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ghastoolkit
-Version: 0.2.2
+Version: 0.2.3
 Summary: GitHub Advanced Security Python Toolkit
 Author: GeekMasher
 Project-URL: Homepage, https://github.com/GeekMasher/ghastoolkit
 Project-URL: Bug Tracker, https://github.com/GeekMasher/ghastoolkit/issues
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `ghastoolkit-0.2.2/README.md` & `ghastoolkit-0.2.3/README.md`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.2.2/pyproject.toml` & `ghastoolkit-0.2.3/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "ghastoolkit"
-version = "0.2.2"
+version = "0.2.3"
 authors = [
   { name="GeekMasher" },
 ]
 description = "GitHub Advanced Security Python Toolkit"
 readme = "README.md"
 requires-python = ">=3.9"
 classifiers = [
```

### Comparing `ghastoolkit-0.2.2/src/ghastoolkit/__init__.py` & `ghastoolkit-0.2.3/src/ghastoolkit/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 __name__ = "ghastoolkit"
 __title__ = "GHAS Toolkit"
 
-__version__ = "0.2.2"
+__version__ = "0.2.3"
 
 __description__ = "GitHub Advanced Security Python Toolkit"
 __summary__ = """\
 GitHub Advanced Security Python Toolkit
 """
 
 __url__ = "https://github.com/GeekMasher/ghastoolkit"
```

### Comparing `ghastoolkit-0.2.2/src/ghastoolkit/__main__.py` & `ghastoolkit-0.2.3/src/ghastoolkit/__main__.py`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.2.2/src/ghastoolkit/codeql/databases.py` & `ghastoolkit-0.2.3/src/ghastoolkit/codeql/databases.py`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.2.2/src/ghastoolkit/octokit/codescanning.py` & `ghastoolkit-0.2.3/src/ghastoolkit/octokit/codescanning.py`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.2.2/src/ghastoolkit/octokit/dependabot.py` & `ghastoolkit-0.2.3/src/ghastoolkit/octokit/dependabot.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,7 @@
-from dataclasses import dataclass
 import logging
 from typing import Optional
 
 from ghastoolkit.octokit.github import GitHub, Repository
 from ghastoolkit.octokit.octokit import GraphQLRequest
 from ghastoolkit.supplychain.advisories import Advisory
 from ghastoolkit.supplychain.dependencyalert import DependencyAlert
```

### Comparing `ghastoolkit-0.2.2/src/ghastoolkit/octokit/dependencygraph.py` & `ghastoolkit-0.2.3/src/ghastoolkit/octokit/dependencygraph.py`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.2.2/src/ghastoolkit/octokit/github.py` & `ghastoolkit-0.2.3/src/ghastoolkit/octokit/github.py`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.2.2/src/ghastoolkit/octokit/octokit.py` & `ghastoolkit-0.2.3/src/ghastoolkit/octokit/octokit.py`

 * *Files 2% similar despite different names*

```diff
@@ -235,14 +235,15 @@
         url = Octokit.route(path, repo, rtype="rest")
         logger.debug(f"Posting content from URL :: {url}")
 
         response = self.session.post(url, json=data)
 
         if response.status_code != expected:
             logger.error(f"Error code from server :: {response.status_code}")
+            logger.error(f"{response.content}")
             known_error = __OCTOKIT_ERRORS__.get(response.status_code)
             if known_error:
                 raise Exception(known_error)
             raise Exception(f"Failed to post data")
 
         return response.json()
```

### Comparing `ghastoolkit-0.2.2/src/ghastoolkit/octokit/secretscanning.py` & `ghastoolkit-0.2.3/src/ghastoolkit/octokit/secretscanning.py`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.2.2/src/ghastoolkit/secretscanning/secretalerts.py` & `ghastoolkit-0.2.3/src/ghastoolkit/secretscanning/secretalerts.py`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.2.2/src/ghastoolkit/supplychain/dependencies.py` & `ghastoolkit-0.2.3/src/ghastoolkit/supplychain/dependencies.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import logging
 from dataclasses import dataclass, field
 from datetime import datetime
 import re
 from typing import Optional
 
 from ghastoolkit.supplychain.dependencyalert import DependencyAlert
-from ghastoolkit.supplychain.licensing import Licenses
+from ghastoolkit.supplychain.licensing import NO_LICENSES, Licenses
 
 logger = logging.getLogger("ghastoolkit.supplychain.dependencies")
 
 
 @dataclass
 class Dependency:
     name: str
@@ -131,21 +131,22 @@
                 if any(regex.search(dep.licence or "NA") for regex in regex_list)
             ]
         )
 
     def findUnknownLicenses(
         self, licenses: Optional[list[str]] = None
     ) -> "Dependencies":
-        licenses = licenses or ["NA", "NOASSERTION"]
+        """Find all the dependencies with no license"""
+        licenses = licenses or NO_LICENSES
         return self.findLicenses(licenses)
 
     def applyLicenses(self, licenses: Licenses):
-        """Apply Linceses"""
+        """Given a list of licenses (Licenses) apply a license"""
         for i, dep in enumerate(self):
-            if dep.licence:
+            if dep.licence and dep.licence not in NO_LICENSES:
                 continue
             purl = dep.getPurl(version=False)
             dblicense = licenses.find(purl)
             if dblicense:
                 dep.licence = " OR ".join(dblicense)
                 self[i] = dep
```

### Comparing `ghastoolkit-0.2.2/src/ghastoolkit/supplychain/dependencyalert.py` & `ghastoolkit-0.2.3/src/ghastoolkit/supplychain/dependencyalert.py`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.2.2/src/ghastoolkit.egg-info/PKG-INFO` & `ghastoolkit-0.2.3/src/ghastoolkit.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ghastoolkit
-Version: 0.2.2
+Version: 0.2.3
 Summary: GitHub Advanced Security Python Toolkit
 Author: GeekMasher
 Project-URL: Homepage, https://github.com/GeekMasher/ghastoolkit
 Project-URL: Bug Tracker, https://github.com/GeekMasher/ghastoolkit/issues
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

### Comparing `ghastoolkit-0.2.2/src/ghastoolkit.egg-info/SOURCES.txt` & `ghastoolkit-0.2.3/src/ghastoolkit.egg-info/SOURCES.txt`

 * *Files 6% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 src/ghastoolkit.egg-info/SOURCES.txt
 src/ghastoolkit.egg-info/dependency_links.txt
 src/ghastoolkit.egg-info/requires.txt
 src/ghastoolkit.egg-info/top_level.txt
 src/ghastoolkit/codeql/__init__.py
 src/ghastoolkit/codeql/consts.py
 src/ghastoolkit/codeql/databases.py
+src/ghastoolkit/codeql/utils.py
 src/ghastoolkit/octokit/__init__.py
 src/ghastoolkit/octokit/codescanning.py
 src/ghastoolkit/octokit/dependabot.py
 src/ghastoolkit/octokit/dependencygraph.py
 src/ghastoolkit/octokit/github.py
 src/ghastoolkit/octokit/octokit.py
 src/ghastoolkit/octokit/secretscanning.py
@@ -24,12 +25,13 @@
 src/ghastoolkit/supplychain/advisories.py
 src/ghastoolkit/supplychain/dependencies.py
 src/ghastoolkit/supplychain/dependencyalert.py
 src/ghastoolkit/supplychain/licensing.py
 tests/test_codeqldb.py
 tests/test_codescanning.py
 tests/test_default.py
+tests/test_dependencies.py
 tests/test_depgraph.py
 tests/test_github.py
 tests/test_licenses.py
 tests/test_octokit.py
 tests/test_secretscanning.py
```

### Comparing `ghastoolkit-0.2.2/tests/test_codeqldb.py` & `ghastoolkit-0.2.3/tests/test_codeqldb.py`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.2.2/tests/test_codescanning.py` & `ghastoolkit-0.2.3/tests/test_codescanning.py`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.2.2/tests/test_default.py` & `ghastoolkit-0.2.3/tests/test_default.py`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.2.2/tests/test_depgraph.py` & `ghastoolkit-0.2.3/tests/test_dependencies.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,74 +1,21 @@
-import unittest
-
-from ghastoolkit.octokit.dependencygraph import Dependency, Dependencies
 
+import unittest
 
-class TestDepGraph(unittest.TestCase):
-    def test_dependency(self):
-        dep = Dependency("django", version="1.11.1", manager="pypi")
-
-        self.assertEqual(dep.name, "django")
-        self.assertEqual(dep.manager, "pypi")
-        self.assertEqual(dep.version, "1.11.1")
-
-    def test_fullname_maven(self):
-        dep = Dependency("express", manager="npm")
-        self.assertEqual(dep.fullname, "express")
-
-        dep = Dependency(
-            "spring-boot-starter-web", "org.springframework.boot", manager="maven"
-        )
-        self.assertEqual(
-            dep.fullname, "org.springframework.boot:spring-boot-starter-web"
-        )
-
-    def test_purl(self):
-        # python
-        dep = Dependency("django", version="1.11.1", manager="pypi")
-        self.assertEqual(dep.getPurl(), "pkg:pypi/django@1.11.1")
-
-        # go
-        dep = Dependency("genproto", "google.golang.org", manager="golang")
-        self.assertEqual(dep.getPurl(), "pkg:golang/google.golang.org/genproto")
-
-    def test_purl_from(self):
-        # GitHub Actions
-        dep = Dependency.fromPurl("pkg:githubactions/actions/setup-python@3")
-        self.assertEqual(dep.name, "setup-python")
-        self.assertEqual(dep.namespace, "actions")
-        self.assertEqual(dep.manager, "githubactions")
-        self.assertEqual(dep.version, "3")
-
-        dep = Dependency.fromPurl("pkg:githubactions/github/codeql-action/analyze@2")
-        self.assertEqual(dep.name, "codeql-action/analyze")
-        self.assertEqual(dep.namespace, "github")
-        self.assertEqual(dep.manager, "githubactions")
-        self.assertEqual(dep.version, "2")
-
-        # PyPi
-        dep = Dependency.fromPurl("pkg:pypi/requests@2.28.2")
-        self.assertEqual(dep.name, "requests")
-        self.assertEqual(dep.manager, "pypi")
-        self.assertEqual(dep.version, "2.28.2")
-
-    def test_purl_from_basic(self):
-        dep = Dependency.fromPurl("npm/ini")
-        self.assertEqual(dep.name, "ini")
-        self.assertEqual(dep.manager, "npm")
+from ghastoolkit import Dependencies, Dependency, Licenses
 
 
 class TestDependencies(unittest.TestCase):
     def setUp(self) -> None:
         self.deps = Dependencies()
-        self.deps.append(Dependency("urllib3", licence="MIT"))
-        self.deps.append(Dependency("rich", licence="NOASSERTION"))
-        self.deps.append(Dependency("pyyaml", licence="GPL-3.0"))
-        self.deps.append(Dependency("pyproject-hooks", licence="Apache-2.0"))
-        self.deps.append(Dependency("requests", licence="GPL-2.0"))
+        self.deps.append(Dependency("urllib3", manager="pypi", licence="MIT"))
+        self.deps.append(Dependency("rich", manager="pypi", licence="NOASSERTION"))
+        self.deps.append(Dependency("pyyaml", manager="pypi", licence="GPL-3.0"))
+        self.deps.append(Dependency("pyproject-hooks", manager="pypi", licence="Apache-2.0"))
+        self.deps.append(Dependency("requests", manager="pypi", licence="GPL-2.0"))
         return super().setUp()
 
     def test_license(self):
         mit = self.deps.findLicenses(["MIT"])
         self.assertEqual(len(mit), 1)
         self.assertEqual(mit[0].name, "urllib3")
 
@@ -90,7 +37,25 @@
         self.assertEqual(pys[1].name, "pyproject-hooks")
 
     def test_find(self):
         dep = self.deps.find("pyyaml")
         self.assertIsNotNone(dep)
         assert dep is not None
         self.assertEqual(dep.name, "pyyaml")
+
+    def test_apply_license(self):
+        deps = self.deps.findUnknownLicenses()
+        self.assertEqual(len(deps), 1)
+
+        licenses = Licenses()
+        licenses.add("pkg:pypi/rich", ["MIT"])
+
+        self.deps.applyLicenses(licenses)
+        
+        deps = self.deps.findUnknownLicenses()
+        self.assertEqual(len(deps), 0)
+
+        dep = self.deps.find("rich")
+        self.assertEqual(dep.name, "rich")
+        self.assertEqual(dep.licence, "MIT")
+
+
```

### Comparing `ghastoolkit-0.2.2/tests/test_github.py` & `ghastoolkit-0.2.3/tests/test_github.py`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.2.2/tests/test_licenses.py` & `ghastoolkit-0.2.3/tests/test_licenses.py`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.2.2/tests/test_octokit.py` & `ghastoolkit-0.2.3/tests/test_octokit.py`

 * *Files identical despite different names*

### Comparing `ghastoolkit-0.2.2/tests/test_secretscanning.py` & `ghastoolkit-0.2.3/tests/test_secretscanning.py`

 * *Files identical despite different names*

