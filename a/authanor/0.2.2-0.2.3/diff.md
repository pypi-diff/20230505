# Comparing `tmp/authanor-0.2.2.tar.gz` & `tmp/authanor-0.2.3.tar.gz`

## Comparing `authanor-0.2.2.tar` & `authanor-0.2.3.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 authanor-0.2.2/authanor/_version.py
--rw-r--r--   0        0        0     3985 2020-02-02 00:00:00.000000 authanor-0.2.2/authanor/database/__init__.py
--rw-r--r--   0        0        0    18062 2020-02-02 00:00:00.000000 authanor-0.2.2/authanor/database/handler.py
--rw-r--r--   0        0        0     5545 2020-02-02 00:00:00.000000 authanor-0.2.2/authanor/database/models.py
--rw-r--r--   0        0        0      572 2020-02-02 00:00:00.000000 authanor-0.2.2/authanor/database/utils.py
--rw-r--r--   0        0        0    10612 2020-02-02 00:00:00.000000 authanor-0.2.2/authanor/testing/helpers.py
--rw-r--r--   0        0        0      911 2020-02-02 00:00:00.000000 authanor-0.2.2/.gitignore
--rw-r--r--   0        0        0    35150 2020-02-02 00:00:00.000000 authanor-0.2.2/COPYING
--rw-r--r--   0        0        0      151 2020-02-02 00:00:00.000000 authanor-0.2.2/LICENSE
--rw-r--r--   0        0        0     2195 2020-02-02 00:00:00.000000 authanor-0.2.2/pyproject.toml
--rw-r--r--   0        0        0     3146 2020-02-02 00:00:00.000000 authanor-0.2.2/PKG-INFO
+-rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 authanor-0.2.3/authanor/_version.py
+-rw-r--r--   0        0        0     3985 2020-02-02 00:00:00.000000 authanor-0.2.3/authanor/database/__init__.py
+-rw-r--r--   0        0        0    18062 2020-02-02 00:00:00.000000 authanor-0.2.3/authanor/database/handler.py
+-rw-r--r--   0        0        0     5545 2020-02-02 00:00:00.000000 authanor-0.2.3/authanor/database/models.py
+-rw-r--r--   0        0        0      572 2020-02-02 00:00:00.000000 authanor-0.2.3/authanor/database/utils.py
+-rw-r--r--   0        0        0    10612 2020-02-02 00:00:00.000000 authanor-0.2.3/authanor/testing/helpers.py
+-rw-r--r--   0        0        0      911 2020-02-02 00:00:00.000000 authanor-0.2.3/.gitignore
+-rw-r--r--   0        0        0    35150 2020-02-02 00:00:00.000000 authanor-0.2.3/COPYING
+-rw-r--r--   0        0        0      151 2020-02-02 00:00:00.000000 authanor-0.2.3/LICENSE
+-rw-r--r--   0        0        0     2133 2020-02-02 00:00:00.000000 authanor-0.2.3/pyproject.toml
+-rw-r--r--   0        0        0     3146 2020-02-02 00:00:00.000000 authanor-0.2.3/PKG-INFO
```

### Comparing `authanor-0.2.2/authanor/database/__init__.py` & `authanor-0.2.3/authanor/database/__init__.py`

 * *Files identical despite different names*

### Comparing `authanor-0.2.2/authanor/database/handler.py` & `authanor-0.2.3/authanor/database/handler.py`

 * *Files identical despite different names*

### Comparing `authanor-0.2.2/authanor/database/models.py` & `authanor-0.2.3/authanor/database/models.py`

 * *Files identical despite different names*

### Comparing `authanor-0.2.2/authanor/database/utils.py` & `authanor-0.2.3/authanor/database/utils.py`

 * *Files identical despite different names*

### Comparing `authanor-0.2.2/authanor/testing/helpers.py` & `authanor-0.2.3/authanor/testing/helpers.py`

 * *Files identical despite different names*

### Comparing `authanor-0.2.2/.gitignore` & `authanor-0.2.3/.gitignore`

 * *Files identical despite different names*

### Comparing `authanor-0.2.2/COPYING` & `authanor-0.2.3/COPYING`

 * *Files identical despite different names*

### Comparing `authanor-0.2.2/pyproject.toml` & `authanor-0.2.3/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -36,21 +36,17 @@
 
 [project.entry-points.pytest11]
 authanor = "authanor.testing.helpers"
 
 [tool.hatch.version]
 source = 'vcs'
 
-[tool.hatch.build.targets.sdist]
+[tool.hatch.build]
 include = [
   '/authanor',
-  '/authanor/testing',
-]
-exclude = [
-  '*.pyc',
 ]
 
 [tool.hatch.build.hooks.vcs]
 version-file = 'authanor/_version.py'
 
 [tool.hatch.metadata.hooks.fancy-pypi-readme]
 content-type = 'text/markdown'
```

### Comparing `authanor-0.2.2/PKG-INFO` & `authanor-0.2.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: authanor
-Version: 0.2.2
+Version: 0.2.3
 Summary: A Pythonic SQLALchemy interface to enforce authorization criteria.
 Project-URL: Download, https://pypi.org/project/authanor
 Project-URL: Homepage, https://github.com/mitchnegus/authanor
 Project-URL: Repository, https://github.com/mitchnegus/authanor
 Project-URL: Changelog, https://github.com/mitchnegus/authanor/blob/main/CHANGELOG.md
 Author-email: Mitch Negus <mitchnegus57@gmail.com>
 License: GNU GPLv3
```

