# Comparing `tmp/sbioapputils-1.0.8.tar.gz` & `tmp/sbioapputils-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sbioapputils-1.0.8.tar", last modified: Thu May  4 17:22:15 2023, max compression
+gzip compressed data, was "sbioapputils-1.0.9.tar", last modified: Fri May  5 12:37:00 2023, max compression
```

## Comparing `sbioapputils-1.0.8.tar` & `sbioapputils-1.0.9.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-05-04 17:22:15.314647 sbioapputils-1.0.8/
--rw-rw-rw-   0        0        0    35823 2023-05-03 10:08:17.000000 sbioapputils-1.0.8/LICENSE
--rw-rw-rw-   0        0        0      783 2023-05-04 17:22:15.313647 sbioapputils-1.0.8/PKG-INFO
--rw-rw-rw-   0        0        0       53 2023-05-03 10:08:17.000000 sbioapputils-1.0.8/README.md
--rw-rw-rw-   0        0        0      837 2023-05-04 17:22:09.000000 sbioapputils-1.0.8/pyproject.toml
-drwxrwxrwx   0        0        0        0 2023-05-04 17:22:15.299851 sbioapputils-1.0.8/sbioapputils/
--rw-rw-rw-   0        0        0        0 2023-05-04 17:17:59.000000 sbioapputils-1.0.8/sbioapputils/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-04 17:22:15.311648 sbioapputils-1.0.8/sbioapputils.egg-info/
--rw-rw-rw-   0        0        0      783 2023-05-04 17:22:15.000000 sbioapputils-1.0.8/sbioapputils.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      245 2023-05-04 17:22:15.000000 sbioapputils-1.0.8/sbioapputils.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-04 17:22:15.000000 sbioapputils-1.0.8/sbioapputils.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       87 2023-05-04 17:22:15.000000 sbioapputils-1.0.8/sbioapputils.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-05-04 17:22:15.000000 sbioapputils-1.0.8/sbioapputils.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-04 17:22:15.314647 sbioapputils-1.0.8/setup.cfg
--rw-rw-rw-   0        0        0      405 2023-05-04 16:31:23.000000 sbioapputils-1.0.8/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-05 12:37:00.371984 sbioapputils-1.0.9/
+-rw-rw-rw-   0        0        0    35823 2023-05-03 10:08:17.000000 sbioapputils-1.0.9/LICENSE
+-rw-rw-rw-   0        0        0      783 2023-05-05 12:37:00.370983 sbioapputils-1.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0       53 2023-05-03 10:08:17.000000 sbioapputils-1.0.9/README.md
+-rw-rw-rw-   0        0        0      837 2023-05-05 12:36:55.000000 sbioapputils-1.0.9/pyproject.toml
+drwxrwxrwx   0        0        0        0 2023-05-05 12:37:00.143600 sbioapputils-1.0.9/sbioapputils/
+-rw-rw-rw-   0        0        0       54 2023-05-05 12:26:04.000000 sbioapputils-1.0.9/sbioapputils/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-05 12:37:00.157050 sbioapputils-1.0.9/sbioapputils.egg-info/
+-rw-rw-rw-   0        0        0      783 2023-05-05 12:36:59.000000 sbioapputils-1.0.9/sbioapputils.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      245 2023-05-05 12:37:00.000000 sbioapputils-1.0.9/sbioapputils.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-05 12:36:59.000000 sbioapputils-1.0.9/sbioapputils.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       87 2023-05-05 12:36:59.000000 sbioapputils-1.0.9/sbioapputils.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-05-05 12:36:59.000000 sbioapputils-1.0.9/sbioapputils.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-05 12:37:00.371984 sbioapputils-1.0.9/setup.cfg
+-rw-rw-rw-   0        0        0      405 2023-05-04 16:31:23.000000 sbioapputils-1.0.9/setup.py
```

### Comparing `sbioapputils-1.0.8/LICENSE` & `sbioapputils-1.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `sbioapputils-1.0.8/PKG-INFO` & `sbioapputils-1.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sbioapputils
-Version: 1.0.8
+Version: 1.0.9
 Summary: Utilities for developing apps with Superbio
 Home-page: https://github.com/Superbio-ai/app-sbioutils
 Author: Superbio AI
 Author-email: Superbio AI <smorgan@superbio.ai>
 Project-URL: Homepage, https://github.com/Superbio-ai/app-sbioutils
 Project-URL: Bug Tracker, https://github.com/Superbio-ai/app-sbioutils/issues
 Classifier: Programming Language :: Python :: 3
```

### Comparing `sbioapputils-1.0.8/pyproject.toml` & `sbioapputils-1.0.9/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 [build-system]
 requires = ["setuptools>=65"]
 build-backend = "setuptools.build_meta"
 [project]
 name = "sbioapputils"
-version = "1.0.8"
+version = "1.0.9"
 authors = [
   { name="Superbio AI", email="smorgan@superbio.ai" },
 ]
 description = "Utilities for developing apps with Superbio"
 readme = "README.md"
 requires-python = ">=3.0"
 classifiers = [
```

### Comparing `sbioapputils-1.0.8/sbioapputils.egg-info/PKG-INFO` & `sbioapputils-1.0.9/sbioapputils.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sbioapputils
-Version: 1.0.8
+Version: 1.0.9
 Summary: Utilities for developing apps with Superbio
 Home-page: https://github.com/Superbio-ai/app-sbioutils
 Author: Superbio AI
 Author-email: Superbio AI <smorgan@superbio.ai>
 Project-URL: Homepage, https://github.com/Superbio-ai/app-sbioutils
 Project-URL: Bug Tracker, https://github.com/Superbio-ai/app-sbioutils/issues
 Classifier: Programming Language :: Python :: 3
```

