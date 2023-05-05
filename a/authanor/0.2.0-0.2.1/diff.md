# Comparing `tmp/authanor-0.2.0.tar.gz` & `tmp/authanor-0.2.1.tar.gz`

## Comparing `authanor-0.2.0.tar` & `authanor-0.2.1.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 authanor-0.2.0/authanor/_version.py
--rw-r--r--   0        0        0     3985 2020-02-02 00:00:00.000000 authanor-0.2.0/authanor/database/__init__.py
--rw-r--r--   0        0        0    18062 2020-02-02 00:00:00.000000 authanor-0.2.0/authanor/database/handler.py
--rw-r--r--   0        0        0     5545 2020-02-02 00:00:00.000000 authanor-0.2.0/authanor/database/models.py
--rw-r--r--   0        0        0      572 2020-02-02 00:00:00.000000 authanor-0.2.0/authanor/database/utils.py
--rw-r--r--   0        0        0    10612 2020-02-02 00:00:00.000000 authanor-0.2.0/authanor/test/helpers.py
--rw-r--r--   0        0        0      911 2020-02-02 00:00:00.000000 authanor-0.2.0/.gitignore
--rw-r--r--   0        0        0    35150 2020-02-02 00:00:00.000000 authanor-0.2.0/COPYING
--rw-r--r--   0        0        0      151 2020-02-02 00:00:00.000000 authanor-0.2.0/LICENSE
--rw-r--r--   0        0        0     2166 2020-02-02 00:00:00.000000 authanor-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     3146 2020-02-02 00:00:00.000000 authanor-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 authanor-0.2.1/authanor/_version.py
+-rw-r--r--   0        0        0     3985 2020-02-02 00:00:00.000000 authanor-0.2.1/authanor/database/__init__.py
+-rw-r--r--   0        0        0    18062 2020-02-02 00:00:00.000000 authanor-0.2.1/authanor/database/handler.py
+-rw-r--r--   0        0        0     5545 2020-02-02 00:00:00.000000 authanor-0.2.1/authanor/database/models.py
+-rw-r--r--   0        0        0      572 2020-02-02 00:00:00.000000 authanor-0.2.1/authanor/database/utils.py
+-rw-r--r--   0        0        0    10612 2020-02-02 00:00:00.000000 authanor-0.2.1/authanor/testing/helpers.py
+-rw-r--r--   0        0        0      911 2020-02-02 00:00:00.000000 authanor-0.2.1/.gitignore
+-rw-r--r--   0        0        0    35150 2020-02-02 00:00:00.000000 authanor-0.2.1/COPYING
+-rw-r--r--   0        0        0      151 2020-02-02 00:00:00.000000 authanor-0.2.1/LICENSE
+-rw-r--r--   0        0        0     2172 2020-02-02 00:00:00.000000 authanor-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0     3146 2020-02-02 00:00:00.000000 authanor-0.2.1/PKG-INFO
```

### Comparing `authanor-0.2.0/authanor/database/__init__.py` & `authanor-0.2.1/authanor/database/__init__.py`

 * *Files identical despite different names*

### Comparing `authanor-0.2.0/authanor/database/handler.py` & `authanor-0.2.1/authanor/database/handler.py`

 * *Files identical despite different names*

### Comparing `authanor-0.2.0/authanor/database/models.py` & `authanor-0.2.1/authanor/database/models.py`

 * *Files identical despite different names*

### Comparing `authanor-0.2.0/authanor/database/utils.py` & `authanor-0.2.1/authanor/database/utils.py`

 * *Files identical despite different names*

### Comparing `authanor-0.2.0/authanor/test/helpers.py` & `authanor-0.2.1/authanor/testing/helpers.py`

 * *Files identical despite different names*

### Comparing `authanor-0.2.0/.gitignore` & `authanor-0.2.1/.gitignore`

 * *Files identical despite different names*

### Comparing `authanor-0.2.0/COPYING` & `authanor-0.2.1/COPYING`

 * *Files identical despite different names*

### Comparing `authanor-0.2.0/pyproject.toml` & `authanor-0.2.1/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -31,15 +31,15 @@
 [project.urls]
 Download = 'https://pypi.org/project/authanor'
 Homepage = 'https://github.com/mitchnegus/authanor'
 Repository = 'https://github.com/mitchnegus/authanor'
 Changelog = 'https://github.com/mitchnegus/authanor/blob/main/CHANGELOG.md'
 
 [project.entry-points.pytest11]
-authanor = "authanor.test.helpers"
+authanor = "authanor.testing.helpers"
 
 [tool.hatch.version]
 source = 'vcs'
 
 [tool.hatch.build.targets.sdist]
 include = [
   '/authanor',
@@ -69,15 +69,15 @@
 addopts = [
   '--import-mode=importlib',
 ]
 
 [tool.coverage.run]
 omit = [
   'tests/*',
-  'authanor/test/helpers.py',
+  'authanor/testing/helpers.py',
 ]
 
 [tool.coverage.report]
 exclude_lines = [
   'raise NotImplementedError',
 ]
```

### Comparing `authanor-0.2.0/PKG-INFO` & `authanor-0.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: authanor
-Version: 0.2.0
+Version: 0.2.1
 Summary: A Pythonic SQLALchemy interface to enforce authorization criteria.
 Project-URL: Download, https://pypi.org/project/authanor
 Project-URL: Homepage, https://github.com/mitchnegus/authanor
 Project-URL: Repository, https://github.com/mitchnegus/authanor
 Project-URL: Changelog, https://github.com/mitchnegus/authanor/blob/main/CHANGELOG.md
 Author-email: Mitch Negus <mitchnegus57@gmail.com>
 License: GNU GPLv3
```

