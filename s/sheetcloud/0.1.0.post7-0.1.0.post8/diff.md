# Comparing `tmp/sheetcloud-0.1.0.post7.tar.gz` & `tmp/sheetcloud-0.1.0.post8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sheetcloud-0.1.0.post7.tar", last modified: Fri May  5 13:19:37 2023, max compression
+gzip compressed data, was "sheetcloud-0.1.0.post8.tar", last modified: Fri May  5 13:28:32 2023, max compression
```

## Comparing `sheetcloud-0.1.0.post7.tar` & `sheetcloud-0.1.0.post8.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 13:19:37.617426 sheetcloud-0.1.0.post7/
--rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-05-05 13:18:37.000000 sheetcloud-0.1.0.post7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      107 2023-05-05 13:18:37.000000 sheetcloud-0.1.0.post7/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4057 2023-05-05 13:19:37.613426 sheetcloud-0.1.0.post7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3165 2023-05-05 13:18:37.000000 sheetcloud-0.1.0.post7/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1474 2023-05-05 13:18:37.000000 sheetcloud-0.1.0.post7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-05-05 13:18:37.000000 sheetcloud-0.1.0.post7/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 13:19:37.613426 sheetcloud-0.1.0.post7/resources/
--rw-r--r--   0 runner    (1001) docker     (123)      193 2023-05-05 13:18:37.000000 sheetcloud-0.1.0.post7/resources/endpoints.v1.json
--rw-r--r--   0 runner    (1001) docker     (123)     3286 2023-05-05 13:18:37.000000 sheetcloud-0.1.0.post7/resources/template_red_sailfish.json
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-05 13:19:37.617426 sheetcloud-0.1.0.post7/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 13:19:37.613426 sheetcloud-0.1.0.post7/sheetcloud/
--rw-r--r--   0 runner    (1001) docker     (123)      343 2023-05-05 13:18:37.000000 sheetcloud-0.1.0.post7/sheetcloud/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5289 2023-05-05 13:18:37.000000 sheetcloud-0.1.0.post7/sheetcloud/conn.py
--rw-r--r--   0 runner    (1001) docker     (123)     1997 2023-05-05 13:18:37.000000 sheetcloud-0.1.0.post7/sheetcloud/drive.py
--rw-r--r--   0 runner    (1001) docker     (123)     1902 2023-05-05 13:18:37.000000 sheetcloud-0.1.0.post7/sheetcloud/env.py
--rw-r--r--   0 runner    (1001) docker     (123)      832 2023-05-05 13:18:37.000000 sheetcloud-0.1.0.post7/sheetcloud/fun.py
--rw-r--r--   0 runner    (1001) docker     (123)     6027 2023-05-05 13:18:37.000000 sheetcloud-0.1.0.post7/sheetcloud/orm.py
--rw-r--r--   0 runner    (1001) docker     (123)     7254 2023-05-05 13:18:37.000000 sheetcloud-0.1.0.post7/sheetcloud/sheets.py
--rw-r--r--   0 runner    (1001) docker     (123)     3729 2023-05-05 13:18:37.000000 sheetcloud-0.1.0.post7/sheetcloud/templates.py
--rw-r--r--   0 runner    (1001) docker     (123)     1943 2023-05-05 13:18:37.000000 sheetcloud-0.1.0.post7/sheetcloud/user.py
--rw-r--r--   0 runner    (1001) docker     (123)     1712 2023-05-05 13:18:37.000000 sheetcloud-0.1.0.post7/sheetcloud/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 13:19:37.613426 sheetcloud-0.1.0.post7/sheetcloud.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4057 2023-05-05 13:19:37.000000 sheetcloud-0.1.0.post7/sheetcloud.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      532 2023-05-05 13:19:37.000000 sheetcloud-0.1.0.post7/sheetcloud.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 13:19:37.000000 sheetcloud-0.1.0.post7/sheetcloud.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-05-05 13:19:37.000000 sheetcloud-0.1.0.post7/sheetcloud.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-05-05 13:19:37.000000 sheetcloud-0.1.0.post7/sheetcloud.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 13:19:37.613426 sheetcloud-0.1.0.post7/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      150 2023-05-05 13:18:37.000000 sheetcloud-0.1.0.post7/tests/test_conn.py
--rw-r--r--   0 runner    (1001) docker     (123)     1079 2023-05-05 13:18:37.000000 sheetcloud-0.1.0.post7/tests/test_orm.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 13:28:32.402811 sheetcloud-0.1.0.post8/
+-rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-05-05 13:26:52.000000 sheetcloud-0.1.0.post8/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-05-05 13:26:52.000000 sheetcloud-0.1.0.post8/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4057 2023-05-05 13:28:32.398810 sheetcloud-0.1.0.post8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3165 2023-05-05 13:26:52.000000 sheetcloud-0.1.0.post8/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1474 2023-05-05 13:26:52.000000 sheetcloud-0.1.0.post8/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-05-05 13:26:52.000000 sheetcloud-0.1.0.post8/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 13:28:32.394811 sheetcloud-0.1.0.post8/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)      193 2023-05-05 13:26:52.000000 sheetcloud-0.1.0.post8/resources/endpoints.v1.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3286 2023-05-05 13:26:52.000000 sheetcloud-0.1.0.post8/resources/template_red_sailfish.json
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-05 13:28:32.402811 sheetcloud-0.1.0.post8/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 13:28:32.398810 sheetcloud-0.1.0.post8/sheetcloud/
+-rw-r--r--   0 runner    (1001) docker     (123)      120 2023-05-05 13:26:52.000000 sheetcloud-0.1.0.post8/sheetcloud/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5254 2023-05-05 13:26:52.000000 sheetcloud-0.1.0.post8/sheetcloud/conn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1997 2023-05-05 13:26:52.000000 sheetcloud-0.1.0.post8/sheetcloud/drive.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1902 2023-05-05 13:26:52.000000 sheetcloud-0.1.0.post8/sheetcloud/env.py
+-rw-r--r--   0 runner    (1001) docker     (123)      832 2023-05-05 13:26:52.000000 sheetcloud-0.1.0.post8/sheetcloud/fun.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6027 2023-05-05 13:26:52.000000 sheetcloud-0.1.0.post8/sheetcloud/orm.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7154 2023-05-05 13:26:52.000000 sheetcloud-0.1.0.post8/sheetcloud/sheets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3729 2023-05-05 13:26:52.000000 sheetcloud-0.1.0.post8/sheetcloud/templates.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1943 2023-05-05 13:26:52.000000 sheetcloud-0.1.0.post8/sheetcloud/user.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1712 2023-05-05 13:26:52.000000 sheetcloud-0.1.0.post8/sheetcloud/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 13:28:32.398810 sheetcloud-0.1.0.post8/sheetcloud.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4057 2023-05-05 13:28:32.000000 sheetcloud-0.1.0.post8/sheetcloud.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      532 2023-05-05 13:28:32.000000 sheetcloud-0.1.0.post8/sheetcloud.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 13:28:32.000000 sheetcloud-0.1.0.post8/sheetcloud.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-05-05 13:28:32.000000 sheetcloud-0.1.0.post8/sheetcloud.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-05-05 13:28:32.000000 sheetcloud-0.1.0.post8/sheetcloud.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 13:28:32.398810 sheetcloud-0.1.0.post8/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      140 2023-05-05 13:26:52.000000 sheetcloud-0.1.0.post8/tests/test_conn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-05-05 13:26:52.000000 sheetcloud-0.1.0.post8/tests/test_orm.py
```

### Comparing `sheetcloud-0.1.0.post7/LICENSE` & `sheetcloud-0.1.0.post8/LICENSE`

 * *Files identical despite different names*

### Comparing `sheetcloud-0.1.0.post7/PKG-INFO` & `sheetcloud-0.1.0.post8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sheetcloud
-Version: 0.1.0.post7
+Version: 0.1.0.post8
 Summary: Sheetcloud.de | Turn Spreadsheets into a Cloud Database | Account required
 Author-email: "sheetcloud.org" <contact@sheetcloud.org>
 Project-URL: Homepage, https://www.sheetcloud.org
 Project-URL: Tracker, https://github.com/sheetcloud/sheetcloud/issues
 Project-URL: Source, https://github.com/sheetcloud/sheetcloud
 Project-URL: Examples, https://github.com/sheetcloud
 Keywords: Spreadsheets,RAD,Database,Cloud
```

### Comparing `sheetcloud-0.1.0.post7/README.md` & `sheetcloud-0.1.0.post8/README.md`

 * *Files identical despite different names*

### Comparing `sheetcloud-0.1.0.post7/pyproject.toml` & `sheetcloud-0.1.0.post8/pyproject.toml`

 * *Files identical despite different names*

### Comparing `sheetcloud-0.1.0.post7/resources/template_red_sailfish.json` & `sheetcloud-0.1.0.post8/resources/template_red_sailfish.json`

 * *Files identical despite different names*

### Comparing `sheetcloud-0.1.0.post7/sheetcloud/conn.py` & `sheetcloud-0.1.0.post8/sheetcloud/conn.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,16 +5,15 @@
 import os
 import json
 import time
 import requests
 
 from typing import *
 
-# from sheetcloud.utils import pw_obfuscator
-from .utils import pw_obfuscator
+from sheetcloud.utils import pw_obfuscator
 
 
 ENV_SHEETCLOUD_USERNAME = os.environ.get('SHEETCLOUD_USERNAME', 'missing')
 ENV_SHEETCLOUD_PASSWORD = os.environ.get('SHEETCLOUD_PASSWORD', 'missing')
 ENV_SHEETCLOUD_LICENSE = os.environ.get('SHEETCLOUD_LICENSE', 'missing')
```

### Comparing `sheetcloud-0.1.0.post7/sheetcloud/drive.py` & `sheetcloud-0.1.0.post8/sheetcloud/drive.py`

 * *Files identical despite different names*

### Comparing `sheetcloud-0.1.0.post7/sheetcloud/env.py` & `sheetcloud-0.1.0.post8/sheetcloud/env.py`

 * *Files identical despite different names*

### Comparing `sheetcloud-0.1.0.post7/sheetcloud/fun.py` & `sheetcloud-0.1.0.post8/sheetcloud/fun.py`

 * *Files identical despite different names*

### Comparing `sheetcloud-0.1.0.post7/sheetcloud/orm.py` & `sheetcloud-0.1.0.post8/sheetcloud/orm.py`

 * *Files identical despite different names*

### Comparing `sheetcloud-0.1.0.post7/sheetcloud/sheets.py` & `sheetcloud-0.1.0.post8/sheetcloud/sheets.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,20 +4,17 @@
 
 import io
 import pandas as pd
 
 from datetime import datetime, timezone
 from typing import *
 
-# from sheetcloud.conn import service
-# from sheetcloud.utils import get_modification_datetime_from_file, create_dir
-# from sheetcloud.templates import load_template
-
-from .conn import service
-from .utils import get_modification_datetime_from_file, create_dir
+from sheetcloud.conn import service
+from sheetcloud.utils import get_modification_datetime_from_file, create_dir
+from sheetcloud.templates import load_template
 
 
 SHEETCLOUD_CACHE_PATH = '.tmp'
 
 
 def list_spreadsheets() -> List[Dict]:
     res = service('/sheets/list', method='post')
```

### Comparing `sheetcloud-0.1.0.post7/sheetcloud/templates.py` & `sheetcloud-0.1.0.post8/sheetcloud/templates.py`

 * *Files identical despite different names*

### Comparing `sheetcloud-0.1.0.post7/sheetcloud/user.py` & `sheetcloud-0.1.0.post8/sheetcloud/user.py`

 * *Files identical despite different names*

### Comparing `sheetcloud-0.1.0.post7/sheetcloud/utils.py` & `sheetcloud-0.1.0.post8/sheetcloud/utils.py`

 * *Files identical despite different names*

### Comparing `sheetcloud-0.1.0.post7/sheetcloud.egg-info/PKG-INFO` & `sheetcloud-0.1.0.post8/sheetcloud.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sheetcloud
-Version: 0.1.0.post7
+Version: 0.1.0.post8
 Summary: Sheetcloud.de | Turn Spreadsheets into a Cloud Database | Account required
 Author-email: "sheetcloud.org" <contact@sheetcloud.org>
 Project-URL: Homepage, https://www.sheetcloud.org
 Project-URL: Tracker, https://github.com/sheetcloud/sheetcloud/issues
 Project-URL: Source, https://github.com/sheetcloud/sheetcloud
 Project-URL: Examples, https://github.com/sheetcloud
 Keywords: Spreadsheets,RAD,Database,Cloud
```

### Comparing `sheetcloud-0.1.0.post7/sheetcloud.egg-info/SOURCES.txt` & `sheetcloud-0.1.0.post8/sheetcloud.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `sheetcloud-0.1.0.post7/tests/test_orm.py` & `sheetcloud-0.1.0.post8/tests/test_orm.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from dataclasses import dataclass, field
 from typing import Optional, List, Dict, Any
 
 import pytest
-# import sheetcloud as sc
+import sheetcloud as sc
 
 
 @dataclass
 class MySubSubDC:
     name: str = 'myname'
 
 
@@ -36,11 +36,11 @@
 
 @pytest.fixture
 def my_classes():
     yield [MyDC, MySubDC, MySubSubDC]
 
 
 
-# def test_orm(my_dc_list, my_classes):
-#     sc.orm.write('sheetcloud-test', my_dc_list, 'ORM_TEST')
-#     objs = sc.orm.read('sheetcloud-test', 'ORM_TEST', my_classes)
-#     print(objs)
+def test_orm(my_dc_list, my_classes):
+    sc.orm.write('sheetcloud-test', my_dc_list, 'ORM_TEST')
+    objs = sc.orm.read('sheetcloud-test', 'ORM_TEST', my_classes)
+    print(objs)
```

