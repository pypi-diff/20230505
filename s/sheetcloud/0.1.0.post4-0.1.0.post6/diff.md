# Comparing `tmp/sheetcloud-0.1.0.post4.tar.gz` & `tmp/sheetcloud-0.1.0.post6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sheetcloud-0.1.0.post4.tar", last modified: Fri May  5 12:34:55 2023, max compression
+gzip compressed data, was "sheetcloud-0.1.0.post6.tar", last modified: Fri May  5 12:55:34 2023, max compression
```

## Comparing `sheetcloud-0.1.0.post4.tar` & `sheetcloud-0.1.0.post6.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 12:34:55.887761 sheetcloud-0.1.0.post4/
--rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-05-05 12:34:08.000000 sheetcloud-0.1.0.post4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      107 2023-05-05 12:34:08.000000 sheetcloud-0.1.0.post4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4055 2023-05-05 12:34:55.887761 sheetcloud-0.1.0.post4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3165 2023-05-05 12:34:08.000000 sheetcloud-0.1.0.post4/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1481 2023-05-05 12:34:08.000000 sheetcloud-0.1.0.post4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-05-05 12:34:08.000000 sheetcloud-0.1.0.post4/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 12:34:55.883762 sheetcloud-0.1.0.post4/resources/
--rw-r--r--   0 runner    (1001) docker     (123)      193 2023-05-05 12:34:08.000000 sheetcloud-0.1.0.post4/resources/endpoints.v1.json
--rw-r--r--   0 runner    (1001) docker     (123)     3286 2023-05-05 12:34:08.000000 sheetcloud-0.1.0.post4/resources/template_red_sailfish.json
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-05 12:34:55.887761 sheetcloud-0.1.0.post4/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 12:34:55.883762 sheetcloud-0.1.0.post4/sheetcloud/
--rw-r--r--   0 runner    (1001) docker     (123)      343 2023-05-05 12:34:08.000000 sheetcloud-0.1.0.post4/sheetcloud/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5289 2023-05-05 12:34:08.000000 sheetcloud-0.1.0.post4/sheetcloud/conn.py
--rw-r--r--   0 runner    (1001) docker     (123)     1997 2023-05-05 12:34:08.000000 sheetcloud-0.1.0.post4/sheetcloud/drive.py
--rw-r--r--   0 runner    (1001) docker     (123)     1902 2023-05-05 12:34:08.000000 sheetcloud-0.1.0.post4/sheetcloud/env.py
--rw-r--r--   0 runner    (1001) docker     (123)      832 2023-05-05 12:34:08.000000 sheetcloud-0.1.0.post4/sheetcloud/fun.py
--rw-r--r--   0 runner    (1001) docker     (123)     6027 2023-05-05 12:34:08.000000 sheetcloud-0.1.0.post4/sheetcloud/orm.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 12:34:55.887761 sheetcloud-0.1.0.post4/sheetcloud/sheetcloud.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      363 2023-05-05 12:34:55.000000 sheetcloud-0.1.0.post4/sheetcloud/sheetcloud.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)     7254 2023-05-05 12:34:08.000000 sheetcloud-0.1.0.post4/sheetcloud/sheets.py
--rw-r--r--   0 runner    (1001) docker     (123)     3729 2023-05-05 12:34:08.000000 sheetcloud-0.1.0.post4/sheetcloud/templates.py
--rw-r--r--   0 runner    (1001) docker     (123)     1943 2023-05-05 12:34:08.000000 sheetcloud-0.1.0.post4/sheetcloud/user.py
--rw-r--r--   0 runner    (1001) docker     (123)     1712 2023-05-05 12:34:08.000000 sheetcloud-0.1.0.post4/sheetcloud/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 12:34:55.887761 sheetcloud-0.1.0.post4/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      150 2023-05-05 12:34:08.000000 sheetcloud-0.1.0.post4/tests/test_conn.py
--rw-r--r--   0 runner    (1001) docker     (123)     1079 2023-05-05 12:34:08.000000 sheetcloud-0.1.0.post4/tests/test_orm.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 12:55:34.009669 sheetcloud-0.1.0.post6/
+-rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-05-05 12:54:45.000000 sheetcloud-0.1.0.post6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-05-05 12:54:45.000000 sheetcloud-0.1.0.post6/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4114 2023-05-05 12:55:34.009669 sheetcloud-0.1.0.post6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3165 2023-05-05 12:54:45.000000 sheetcloud-0.1.0.post6/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1483 2023-05-05 12:54:45.000000 sheetcloud-0.1.0.post6/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-05-05 12:54:45.000000 sheetcloud-0.1.0.post6/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 12:55:34.009669 sheetcloud-0.1.0.post6/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)      193 2023-05-05 12:54:45.000000 sheetcloud-0.1.0.post6/resources/endpoints.v1.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3286 2023-05-05 12:54:45.000000 sheetcloud-0.1.0.post6/resources/template_red_sailfish.json
+-rw-r--r--   0 runner    (1001) docker     (123)      692 2023-05-05 12:55:34.009669 sheetcloud-0.1.0.post6/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 12:55:34.009669 sheetcloud-0.1.0.post6/sheetcloud/
+-rw-r--r--   0 runner    (1001) docker     (123)      343 2023-05-05 12:54:45.000000 sheetcloud-0.1.0.post6/sheetcloud/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5289 2023-05-05 12:54:45.000000 sheetcloud-0.1.0.post6/sheetcloud/conn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1997 2023-05-05 12:54:45.000000 sheetcloud-0.1.0.post6/sheetcloud/drive.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1902 2023-05-05 12:54:45.000000 sheetcloud-0.1.0.post6/sheetcloud/env.py
+-rw-r--r--   0 runner    (1001) docker     (123)      832 2023-05-05 12:54:45.000000 sheetcloud-0.1.0.post6/sheetcloud/fun.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6027 2023-05-05 12:54:45.000000 sheetcloud-0.1.0.post6/sheetcloud/orm.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 12:55:34.009669 sheetcloud-0.1.0.post6/sheetcloud/sheetcloud.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      373 2023-05-05 12:55:34.000000 sheetcloud-0.1.0.post6/sheetcloud/sheetcloud.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     7254 2023-05-05 12:54:45.000000 sheetcloud-0.1.0.post6/sheetcloud/sheets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3729 2023-05-05 12:54:45.000000 sheetcloud-0.1.0.post6/sheetcloud/templates.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1943 2023-05-05 12:54:45.000000 sheetcloud-0.1.0.post6/sheetcloud/user.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1712 2023-05-05 12:54:45.000000 sheetcloud-0.1.0.post6/sheetcloud/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 12:55:34.009669 sheetcloud-0.1.0.post6/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      150 2023-05-05 12:54:45.000000 sheetcloud-0.1.0.post6/tests/test_conn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1079 2023-05-05 12:54:45.000000 sheetcloud-0.1.0.post6/tests/test_orm.py
```

### Comparing `sheetcloud-0.1.0.post4/LICENSE` & `sheetcloud-0.1.0.post6/LICENSE`

 * *Files identical despite different names*

### Comparing `sheetcloud-0.1.0.post4/PKG-INFO` & `sheetcloud-0.1.0.post6/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,18 +1,20 @@
 Metadata-Version: 2.1
 Name: sheetcloud
-Version: 0.1.0.post4
+Version: 0.1.0.post6
 Summary: Sheetcloud.de | Turn Spreadsheets into a Cloud Database | Account required
-Author-email: "SheetCloud.de" <info@sheetcloud.de>
-Project-URL: Homepage, https://www.sheetcloud.de
+Home-page: https://sheetcloud.org
+Author: sheetcloud.org
+Author-email: "sheetcloud.org" <contact@sheetcloud.org>
+Project-URL: Homepage, https://www.sheetcloud.org
 Project-URL: Tracker, https://github.com/sheetcloud/sheetcloud/issues
 Project-URL: Source, https://github.com/sheetcloud/sheetcloud
 Project-URL: Examples, https://github.com/sheetcloud
 Keywords: Spreadsheets,RAD,Database,Cloud
-Classifier: Development Status :: 2 - Pre-Alpha
+Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Database
 Classifier: Topic :: Office/Business :: Financial :: Spreadsheet
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
```

### Comparing `sheetcloud-0.1.0.post4/README.md` & `sheetcloud-0.1.0.post6/README.md`

 * *Files identical despite different names*

### Comparing `sheetcloud-0.1.0.post4/pyproject.toml` & `sheetcloud-0.1.0.post6/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -4,37 +4,37 @@
 
 [project]
 name = "sheetcloud"
 readme = "README.md"
 keywords = ["Spreadsheets", "RAD", "Database", "Cloud"]
 description = "Sheetcloud.de | Turn Spreadsheets into a Cloud Database | Account required"
 requires-python = ">=3.7"
-authors = [{ name = "SheetCloud.de", email = "info@sheetcloud.de" }]
+authors = [{ name = "sheetcloud.org", email = "contact@sheetcloud.org" }]
 classifiers = [
     # How mature is this project? Common values are
     #   1 - Planning
     #   2 - Pre-Alpha 
     #   3 - Alpha
     #   4 - Beta
     #   5 - Production/Stable
-    "Development Status :: 2 - Pre-Alpha",
+    "Development Status :: 3 - Alpha",
 
     # Indicate who your project is intended for
     "Intended Audience :: Developers",
     "Topic :: Database",
     "Topic :: Office/Business :: Financial :: Spreadsheet",
 
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 dynamic = ["dependencies", "version"]
 
 [project.urls]
-"Homepage" = "https://www.sheetcloud.de"
+"Homepage" = "https://www.sheetcloud.org"
 "Tracker" = "https://github.com/sheetcloud/sheetcloud/issues"
 "Source" = "https://github.com/sheetcloud/sheetcloud"
 "Examples" = "https://github.com/sheetcloud"
 
 [tool.setuptools-git-versioning]
 enabled = true
 template = "{tag}.post{ccount}"
```

### Comparing `sheetcloud-0.1.0.post4/resources/template_red_sailfish.json` & `sheetcloud-0.1.0.post6/resources/template_red_sailfish.json`

 * *Files identical despite different names*

### Comparing `sheetcloud-0.1.0.post4/sheetcloud/conn.py` & `sheetcloud-0.1.0.post6/sheetcloud/conn.py`

 * *Files identical despite different names*

### Comparing `sheetcloud-0.1.0.post4/sheetcloud/drive.py` & `sheetcloud-0.1.0.post6/sheetcloud/drive.py`

 * *Files identical despite different names*

### Comparing `sheetcloud-0.1.0.post4/sheetcloud/env.py` & `sheetcloud-0.1.0.post6/sheetcloud/env.py`

 * *Files identical despite different names*

### Comparing `sheetcloud-0.1.0.post4/sheetcloud/fun.py` & `sheetcloud-0.1.0.post6/sheetcloud/fun.py`

 * *Files identical despite different names*

### Comparing `sheetcloud-0.1.0.post4/sheetcloud/orm.py` & `sheetcloud-0.1.0.post6/sheetcloud/orm.py`

 * *Files identical despite different names*

### Comparing `sheetcloud-0.1.0.post4/sheetcloud/sheets.py` & `sheetcloud-0.1.0.post6/sheetcloud/sheets.py`

 * *Files identical despite different names*

### Comparing `sheetcloud-0.1.0.post4/sheetcloud/templates.py` & `sheetcloud-0.1.0.post6/sheetcloud/templates.py`

 * *Files identical despite different names*

### Comparing `sheetcloud-0.1.0.post4/sheetcloud/user.py` & `sheetcloud-0.1.0.post6/sheetcloud/user.py`

 * *Files identical despite different names*

### Comparing `sheetcloud-0.1.0.post4/sheetcloud/utils.py` & `sheetcloud-0.1.0.post6/sheetcloud/utils.py`

 * *Files identical despite different names*

### Comparing `sheetcloud-0.1.0.post4/tests/test_orm.py` & `sheetcloud-0.1.0.post6/tests/test_orm.py`

 * *Files identical despite different names*

