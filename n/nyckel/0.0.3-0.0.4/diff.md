# Comparing `tmp/nyckel-0.0.3.tar.gz` & `tmp/nyckel-0.0.4.tar.gz`

## Comparing `nyckel-0.0.3.tar` & `nyckel-0.0.4.tar`

### file list

```diff
@@ -1,11 +1,13 @@
--rw-r--r--   0        0        0       94 2020-02-02 00:00:00.000000 nyckel-0.0.3/requirements.txt
--rw-r--r--   0        0        0      941 2020-02-02 00:00:00.000000 nyckel-0.0.3/.github/workflows/deploy.yml
--rw-r--r--   0        0        0     1058 2020-02-02 00:00:00.000000 nyckel-0.0.3/.github/workflows/test-all.yml
--rw-r--r--   0        0        0      318 2020-02-02 00:00:00.000000 nyckel-0.0.3/.vscode/settings.json
--rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 nyckel-0.0.3/src/nyckel/greeter.py
--rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 nyckel-0.0.3/tests/test_greeter.py
--rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 nyckel-0.0.3/.gitignore
--rw-r--r--   0        0        0     1063 2020-02-02 00:00:00.000000 nyckel-0.0.3/LICENSE
--rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 nyckel-0.0.3/README.md
--rw-r--r--   0        0        0      565 2020-02-02 00:00:00.000000 nyckel-0.0.3/pyproject.toml
--rw-r--r--   0        0        0      478 2020-02-02 00:00:00.000000 nyckel-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0       94 2020-02-02 00:00:00.000000 nyckel-0.0.4/requirements.txt
+-rw-r--r--   0        0        0      950 2020-02-02 00:00:00.000000 nyckel-0.0.4/.github/workflows/deploy.yml
+-rw-r--r--   0        0        0     1068 2020-02-02 00:00:00.000000 nyckel-0.0.4/.github/workflows/test-all.yml
+-rw-r--r--   0        0        0      318 2020-02-02 00:00:00.000000 nyckel-0.0.4/.vscode/settings.json
+-rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 nyckel-0.0.4/src/nyckel/__about__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nyckel-0.0.4/src/nyckel/__init__.py
+-rw-r--r--   0        0        0       65 2020-02-02 00:00:00.000000 nyckel-0.0.4/src/nyckel/greeter.py
+-rw-r--r--   0        0        0      110 2020-02-02 00:00:00.000000 nyckel-0.0.4/tests/test_greeter.py
+-rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 nyckel-0.0.4/.gitignore
+-rw-r--r--   0        0        0     1063 2020-02-02 00:00:00.000000 nyckel-0.0.4/LICENSE
+-rw-r--r--   0        0        0       44 2020-02-02 00:00:00.000000 nyckel-0.0.4/README.md
+-rw-r--r--   0        0        0      565 2020-02-02 00:00:00.000000 nyckel-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0      478 2020-02-02 00:00:00.000000 nyckel-0.0.4/PKG-INFO
```

### Comparing `nyckel-0.0.3/.github/workflows/deploy.yml` & `nyckel-0.0.4/.github/workflows/deploy.yml`

 * *Files 14% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-name: Python package
+name: Test and deploy to PYPI
 
 on: [push]
 
 jobs:
   build:
 
     runs-on: ubuntu-latest
```

### Comparing `nyckel-0.0.3/.github/workflows/test-all.yml` & `nyckel-0.0.4/.github/workflows/test-all.yml`

 * *Files 4% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-name: Python package
+name: Test all python versions
 
 on: [push]
 
 jobs:
   build:
 
     runs-on: ubuntu-latest
```

### Comparing `nyckel-0.0.3/.gitignore` & `nyckel-0.0.4/.gitignore`

 * *Files identical despite different names*

### Comparing `nyckel-0.0.3/LICENSE` & `nyckel-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `nyckel-0.0.3/pyproject.toml` & `nyckel-0.0.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 [tool.hatch.build.targets.wheel]
 packages = ["src/nyckel"]
 
 
 [project]
 name = "nyckel"
-version = "0.0.3"
+version = "0.0.4"
 authors = [
   { name="Oscar Beijbom", email="oscar@nyckel.com" },
 ]
 description = "Python package for the Nyckel API"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

