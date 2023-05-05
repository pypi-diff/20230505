# Comparing `tmp/nyckel-0.0.4.tar.gz` & `tmp/nyckel-0.0.5.tar.gz`

## Comparing `nyckel-0.0.4.tar` & `nyckel-0.0.5.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0       94 2020-02-02 00:00:00.000000 nyckel-0.0.4/requirements.txt
--rw-r--r--   0        0        0      950 2020-02-02 00:00:00.000000 nyckel-0.0.4/.github/workflows/deploy.yml
--rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 nyckel-0.0.4/.github/workflows/test-all.yml
--rw-r--r--   0        0        0      318 2020-02-02 00:00:00.000000 nyckel-0.0.4/.vscode/settings.json
--rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 nyckel-0.0.4/src/nyckel/__about__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nyckel-0.0.4/src/nyckel/__init__.py
--rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 nyckel-0.0.4/src/nyckel/greeter.py
--rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 nyckel-0.0.4/tests/test_greeter.py
--rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 nyckel-0.0.4/.gitignore
--rw-r--r--   0        0        0     1063 2020-02-02 00:00:00.000000 nyckel-0.0.4/LICENSE
--rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 nyckel-0.0.4/README.md
--rw-r--r--   0        0        0      565 2020-02-02 00:00:00.000000 nyckel-0.0.4/pyproject.toml
--rw-r--r--   0        0        0      478 2020-02-02 00:00:00.000000 nyckel-0.0.4/PKG-INFO
+-rw-r--r--   0        0        0       94 2020-02-02 00:00:00.000000 nyckel-0.0.5/requirements.txt
+-rw-r--r--   0        0        0      981 2020-02-02 00:00:00.000000 nyckel-0.0.5/.github/workflows/deploy.yml
+-rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 nyckel-0.0.5/.github/workflows/test-all.yml
+-rw-r--r--   0        0        0      318 2020-02-02 00:00:00.000000 nyckel-0.0.5/.vscode/settings.json
+-rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 nyckel-0.0.5/src/nyckel/__about__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nyckel-0.0.5/src/nyckel/__init__.py
+-rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 nyckel-0.0.5/src/nyckel/greeter.py
+-rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 nyckel-0.0.5/tests/test_greeter.py
+-rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 nyckel-0.0.5/.gitignore
+-rw-r--r--   0        0        0     1063 2020-02-02 00:00:00.000000 nyckel-0.0.5/LICENSE
+-rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 nyckel-0.0.5/README.md
+-rw-r--r--   0        0        0      565 2020-02-02 00:00:00.000000 nyckel-0.0.5/pyproject.toml
+-rw-r--r--   0        0        0      478 2020-02-02 00:00:00.000000 nyckel-0.0.5/PKG-INFO
```

### Comparing `nyckel-0.0.4/.github/workflows/deploy.yml` & `nyckel-0.0.5/.github/workflows/deploy.yml`

 * *Files 22% similar despite different names*

```diff
@@ -1,10 +1,13 @@
 name: Test and deploy to PYPI
 
-on: [push]
+on: 
+  push:
+    branches:
+      - master
 
 jobs:
   build:
 
     runs-on: ubuntu-latest
     steps:
       - uses: actions/checkout@v3
```

### Comparing `nyckel-0.0.4/.github/workflows/test-all.yml` & `nyckel-0.0.5/.github/workflows/test-all.yml`

 * *Files identical despite different names*

### Comparing `nyckel-0.0.4/.gitignore` & `nyckel-0.0.5/.gitignore`

 * *Files identical despite different names*

### Comparing `nyckel-0.0.4/LICENSE` & `nyckel-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `nyckel-0.0.4/pyproject.toml` & `nyckel-0.0.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 [tool.hatch.build.targets.wheel]
 packages = ["src/nyckel"]
 
 
 [project]
 name = "nyckel"
-version = "0.0.4"
+version = "0.0.5"
 authors = [
   { name="Oscar Beijbom", email="oscar@nyckel.com" },
 ]
 description = "Python package for the Nyckel API"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

