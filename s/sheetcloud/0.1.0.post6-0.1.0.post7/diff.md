# Comparing `tmp/sheetcloud-0.1.0.post6.tar.gz` & `tmp/sheetcloud-0.1.0.post7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sheetcloud-0.1.0.post6.tar", last modified: Fri May  5 12:55:34 2023, max compression
+gzip compressed data, was "sheetcloud-0.1.0.post7.tar", last modified: Fri May  5 13:19:37 2023, max compression
```

## Comparing `sheetcloud-0.1.0.post6.tar` & `sheetcloud-0.1.0.post7.tar`

### file list

```diff
@@ -1,27 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 12:55:34.009669 sheetcloud-0.1.0.post6/
--rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-05-05 12:54:45.000000 sheetcloud-0.1.0.post6/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      107 2023-05-05 12:54:45.000000 sheetcloud-0.1.0.post6/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4114 2023-05-05 12:55:34.009669 sheetcloud-0.1.0.post6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3165 2023-05-05 12:54:45.000000 sheetcloud-0.1.0.post6/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1483 2023-05-05 12:54:45.000000 sheetcloud-0.1.0.post6/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-05-05 12:54:45.000000 sheetcloud-0.1.0.post6/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 12:55:34.009669 sheetcloud-0.1.0.post6/resources/
--rw-r--r--   0 runner    (1001) docker     (123)      193 2023-05-05 12:54:45.000000 sheetcloud-0.1.0.post6/resources/endpoints.v1.json
--rw-r--r--   0 runner    (1001) docker     (123)     3286 2023-05-05 12:54:45.000000 sheetcloud-0.1.0.post6/resources/template_red_sailfish.json
--rw-r--r--   0 runner    (1001) docker     (123)      692 2023-05-05 12:55:34.009669 sheetcloud-0.1.0.post6/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 12:55:34.009669 sheetcloud-0.1.0.post6/sheetcloud/
--rw-r--r--   0 runner    (1001) docker     (123)      343 2023-05-05 12:54:45.000000 sheetcloud-0.1.0.post6/sheetcloud/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5289 2023-05-05 12:54:45.000000 sheetcloud-0.1.0.post6/sheetcloud/conn.py
--rw-r--r--   0 runner    (1001) docker     (123)     1997 2023-05-05 12:54:45.000000 sheetcloud-0.1.0.post6/sheetcloud/drive.py
--rw-r--r--   0 runner    (1001) docker     (123)     1902 2023-05-05 12:54:45.000000 sheetcloud-0.1.0.post6/sheetcloud/env.py
--rw-r--r--   0 runner    (1001) docker     (123)      832 2023-05-05 12:54:45.000000 sheetcloud-0.1.0.post6/sheetcloud/fun.py
--rw-r--r--   0 runner    (1001) docker     (123)     6027 2023-05-05 12:54:45.000000 sheetcloud-0.1.0.post6/sheetcloud/orm.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 12:55:34.009669 sheetcloud-0.1.0.post6/sheetcloud/sheetcloud.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      373 2023-05-05 12:55:34.000000 sheetcloud-0.1.0.post6/sheetcloud/sheetcloud.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)     7254 2023-05-05 12:54:45.000000 sheetcloud-0.1.0.post6/sheetcloud/sheets.py
--rw-r--r--   0 runner    (1001) docker     (123)     3729 2023-05-05 12:54:45.000000 sheetcloud-0.1.0.post6/sheetcloud/templates.py
--rw-r--r--   0 runner    (1001) docker     (123)     1943 2023-05-05 12:54:45.000000 sheetcloud-0.1.0.post6/sheetcloud/user.py
--rw-r--r--   0 runner    (1001) docker     (123)     1712 2023-05-05 12:54:45.000000 sheetcloud-0.1.0.post6/sheetcloud/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 12:55:34.009669 sheetcloud-0.1.0.post6/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      150 2023-05-05 12:54:45.000000 sheetcloud-0.1.0.post6/tests/test_conn.py
--rw-r--r--   0 runner    (1001) docker     (123)     1079 2023-05-05 12:54:45.000000 sheetcloud-0.1.0.post6/tests/test_orm.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 13:19:37.617426 sheetcloud-0.1.0.post7/
+-rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-05-05 13:18:37.000000 sheetcloud-0.1.0.post7/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-05-05 13:18:37.000000 sheetcloud-0.1.0.post7/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4057 2023-05-05 13:19:37.613426 sheetcloud-0.1.0.post7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3165 2023-05-05 13:18:37.000000 sheetcloud-0.1.0.post7/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1474 2023-05-05 13:18:37.000000 sheetcloud-0.1.0.post7/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-05-05 13:18:37.000000 sheetcloud-0.1.0.post7/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 13:19:37.613426 sheetcloud-0.1.0.post7/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)      193 2023-05-05 13:18:37.000000 sheetcloud-0.1.0.post7/resources/endpoints.v1.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3286 2023-05-05 13:18:37.000000 sheetcloud-0.1.0.post7/resources/template_red_sailfish.json
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-05 13:19:37.617426 sheetcloud-0.1.0.post7/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 13:19:37.613426 sheetcloud-0.1.0.post7/sheetcloud/
+-rw-r--r--   0 runner    (1001) docker     (123)      343 2023-05-05 13:18:37.000000 sheetcloud-0.1.0.post7/sheetcloud/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5289 2023-05-05 13:18:37.000000 sheetcloud-0.1.0.post7/sheetcloud/conn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1997 2023-05-05 13:18:37.000000 sheetcloud-0.1.0.post7/sheetcloud/drive.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1902 2023-05-05 13:18:37.000000 sheetcloud-0.1.0.post7/sheetcloud/env.py
+-rw-r--r--   0 runner    (1001) docker     (123)      832 2023-05-05 13:18:37.000000 sheetcloud-0.1.0.post7/sheetcloud/fun.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6027 2023-05-05 13:18:37.000000 sheetcloud-0.1.0.post7/sheetcloud/orm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7254 2023-05-05 13:18:37.000000 sheetcloud-0.1.0.post7/sheetcloud/sheets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3729 2023-05-05 13:18:37.000000 sheetcloud-0.1.0.post7/sheetcloud/templates.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1943 2023-05-05 13:18:37.000000 sheetcloud-0.1.0.post7/sheetcloud/user.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1712 2023-05-05 13:18:37.000000 sheetcloud-0.1.0.post7/sheetcloud/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 13:19:37.613426 sheetcloud-0.1.0.post7/sheetcloud.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4057 2023-05-05 13:19:37.000000 sheetcloud-0.1.0.post7/sheetcloud.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      532 2023-05-05 13:19:37.000000 sheetcloud-0.1.0.post7/sheetcloud.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 13:19:37.000000 sheetcloud-0.1.0.post7/sheetcloud.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-05-05 13:19:37.000000 sheetcloud-0.1.0.post7/sheetcloud.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-05-05 13:19:37.000000 sheetcloud-0.1.0.post7/sheetcloud.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 13:19:37.613426 sheetcloud-0.1.0.post7/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      150 2023-05-05 13:18:37.000000 sheetcloud-0.1.0.post7/tests/test_conn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1079 2023-05-05 13:18:37.000000 sheetcloud-0.1.0.post7/tests/test_orm.py
```

### Comparing `sheetcloud-0.1.0.post6/LICENSE` & `sheetcloud-0.1.0.post7/LICENSE`

 * *Files identical despite different names*

### Comparing `sheetcloud-0.1.0.post6/PKG-INFO` & `sheetcloud-0.1.0.post7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,11 @@
 Metadata-Version: 2.1
 Name: sheetcloud
-Version: 0.1.0.post6
+Version: 0.1.0.post7
 Summary: Sheetcloud.de | Turn Spreadsheets into a Cloud Database | Account required
-Home-page: https://sheetcloud.org
-Author: sheetcloud.org
 Author-email: "sheetcloud.org" <contact@sheetcloud.org>
 Project-URL: Homepage, https://www.sheetcloud.org
 Project-URL: Tracker, https://github.com/sheetcloud/sheetcloud/issues
 Project-URL: Source, https://github.com/sheetcloud/sheetcloud
 Project-URL: Examples, https://github.com/sheetcloud
 Keywords: Spreadsheets,RAD,Database,Cloud
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `sheetcloud-0.1.0.post6/README.md` & `sheetcloud-0.1.0.post7/README.md`

 * *Files identical despite different names*

### Comparing `sheetcloud-0.1.0.post6/pyproject.toml` & `sheetcloud-0.1.0.post7/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -43,8 +43,8 @@
 [tool.setuptools.dynamic]
 dependencies = { file = ["requirements.txt"] }
 
 [tool.setuptools]
 include-package-data = true
 
 [tool.setuptools.packages.find]
-where = ["sheetcloud"]
+where = ["."]
```

### Comparing `sheetcloud-0.1.0.post6/resources/template_red_sailfish.json` & `sheetcloud-0.1.0.post7/resources/template_red_sailfish.json`

 * *Files identical despite different names*

### Comparing `sheetcloud-0.1.0.post6/sheetcloud/conn.py` & `sheetcloud-0.1.0.post7/sheetcloud/conn.py`

 * *Files identical despite different names*

### Comparing `sheetcloud-0.1.0.post6/sheetcloud/drive.py` & `sheetcloud-0.1.0.post7/sheetcloud/drive.py`

 * *Files identical despite different names*

### Comparing `sheetcloud-0.1.0.post6/sheetcloud/env.py` & `sheetcloud-0.1.0.post7/sheetcloud/env.py`

 * *Files identical despite different names*

### Comparing `sheetcloud-0.1.0.post6/sheetcloud/fun.py` & `sheetcloud-0.1.0.post7/sheetcloud/fun.py`

 * *Files identical despite different names*

### Comparing `sheetcloud-0.1.0.post6/sheetcloud/orm.py` & `sheetcloud-0.1.0.post7/sheetcloud/orm.py`

 * *Files identical despite different names*

### Comparing `sheetcloud-0.1.0.post6/sheetcloud/sheets.py` & `sheetcloud-0.1.0.post7/sheetcloud/sheets.py`

 * *Files identical despite different names*

### Comparing `sheetcloud-0.1.0.post6/sheetcloud/templates.py` & `sheetcloud-0.1.0.post7/sheetcloud/templates.py`

 * *Files identical despite different names*

### Comparing `sheetcloud-0.1.0.post6/sheetcloud/user.py` & `sheetcloud-0.1.0.post7/sheetcloud/user.py`

 * *Files identical despite different names*

### Comparing `sheetcloud-0.1.0.post6/sheetcloud/utils.py` & `sheetcloud-0.1.0.post7/sheetcloud/utils.py`

 * *Files identical despite different names*

### Comparing `sheetcloud-0.1.0.post6/tests/test_orm.py` & `sheetcloud-0.1.0.post7/tests/test_orm.py`

 * *Files identical despite different names*

