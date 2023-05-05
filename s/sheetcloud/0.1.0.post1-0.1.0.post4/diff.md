# Comparing `tmp/sheetcloud-0.1.0.post1.tar.gz` & `tmp/sheetcloud-0.1.0.post4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sheetcloud-0.1.0.post1.tar", last modified: Fri May  5 12:22:57 2023, max compression
+gzip compressed data, was "sheetcloud-0.1.0.post4.tar", last modified: Fri May  5 12:34:55 2023, max compression
```

## Comparing `sheetcloud-0.1.0.post1.tar` & `sheetcloud-0.1.0.post4.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 12:22:57.300330 sheetcloud-0.1.0.post1/
--rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-05-05 12:21:37.000000 sheetcloud-0.1.0.post1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      107 2023-05-05 12:21:37.000000 sheetcloud-0.1.0.post1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4055 2023-05-05 12:22:57.300330 sheetcloud-0.1.0.post1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3165 2023-05-05 12:21:37.000000 sheetcloud-0.1.0.post1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1481 2023-05-05 12:21:37.000000 sheetcloud-0.1.0.post1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-05-05 12:21:37.000000 sheetcloud-0.1.0.post1/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 12:22:57.296330 sheetcloud-0.1.0.post1/resources/
--rw-r--r--   0 runner    (1001) docker     (123)      193 2023-05-05 12:21:37.000000 sheetcloud-0.1.0.post1/resources/endpoints.v1.json
--rw-r--r--   0 runner    (1001) docker     (123)     3286 2023-05-05 12:21:37.000000 sheetcloud-0.1.0.post1/resources/template_red_sailfish.json
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-05 12:22:57.300330 sheetcloud-0.1.0.post1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 12:22:57.300330 sheetcloud-0.1.0.post1/sheetcloud/
--rw-r--r--   0 runner    (1001) docker     (123)      331 2023-05-05 12:21:37.000000 sheetcloud-0.1.0.post1/sheetcloud/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5254 2023-05-05 12:21:37.000000 sheetcloud-0.1.0.post1/sheetcloud/conn.py
--rw-r--r--   0 runner    (1001) docker     (123)     1997 2023-05-05 12:21:37.000000 sheetcloud-0.1.0.post1/sheetcloud/drive.py
--rw-r--r--   0 runner    (1001) docker     (123)     1902 2023-05-05 12:21:37.000000 sheetcloud-0.1.0.post1/sheetcloud/env.py
--rw-r--r--   0 runner    (1001) docker     (123)      832 2023-05-05 12:21:37.000000 sheetcloud-0.1.0.post1/sheetcloud/fun.py
--rw-r--r--   0 runner    (1001) docker     (123)     6027 2023-05-05 12:21:37.000000 sheetcloud-0.1.0.post1/sheetcloud/orm.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 12:22:57.300330 sheetcloud-0.1.0.post1/sheetcloud/sheetcloud.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      363 2023-05-05 12:22:57.000000 sheetcloud-0.1.0.post1/sheetcloud/sheetcloud.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)     7153 2023-05-05 12:21:37.000000 sheetcloud-0.1.0.post1/sheetcloud/sheets.py
--rw-r--r--   0 runner    (1001) docker     (123)     3729 2023-05-05 12:21:37.000000 sheetcloud-0.1.0.post1/sheetcloud/templates.py
--rw-r--r--   0 runner    (1001) docker     (123)     1943 2023-05-05 12:21:37.000000 sheetcloud-0.1.0.post1/sheetcloud/user.py
--rw-r--r--   0 runner    (1001) docker     (123)     1712 2023-05-05 12:21:37.000000 sheetcloud-0.1.0.post1/sheetcloud/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 12:22:57.300330 sheetcloud-0.1.0.post1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      103 2023-05-05 12:21:37.000000 sheetcloud-0.1.0.post1/tests/test_conn.py
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-05-05 12:21:37.000000 sheetcloud-0.1.0.post1/tests/test_orm.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 12:34:55.887761 sheetcloud-0.1.0.post4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-05-05 12:34:08.000000 sheetcloud-0.1.0.post4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-05-05 12:34:08.000000 sheetcloud-0.1.0.post4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4055 2023-05-05 12:34:55.887761 sheetcloud-0.1.0.post4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3165 2023-05-05 12:34:08.000000 sheetcloud-0.1.0.post4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1481 2023-05-05 12:34:08.000000 sheetcloud-0.1.0.post4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-05-05 12:34:08.000000 sheetcloud-0.1.0.post4/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 12:34:55.883762 sheetcloud-0.1.0.post4/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)      193 2023-05-05 12:34:08.000000 sheetcloud-0.1.0.post4/resources/endpoints.v1.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3286 2023-05-05 12:34:08.000000 sheetcloud-0.1.0.post4/resources/template_red_sailfish.json
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-05 12:34:55.887761 sheetcloud-0.1.0.post4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 12:34:55.883762 sheetcloud-0.1.0.post4/sheetcloud/
+-rw-r--r--   0 runner    (1001) docker     (123)      343 2023-05-05 12:34:08.000000 sheetcloud-0.1.0.post4/sheetcloud/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5289 2023-05-05 12:34:08.000000 sheetcloud-0.1.0.post4/sheetcloud/conn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1997 2023-05-05 12:34:08.000000 sheetcloud-0.1.0.post4/sheetcloud/drive.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1902 2023-05-05 12:34:08.000000 sheetcloud-0.1.0.post4/sheetcloud/env.py
+-rw-r--r--   0 runner    (1001) docker     (123)      832 2023-05-05 12:34:08.000000 sheetcloud-0.1.0.post4/sheetcloud/fun.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6027 2023-05-05 12:34:08.000000 sheetcloud-0.1.0.post4/sheetcloud/orm.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 12:34:55.887761 sheetcloud-0.1.0.post4/sheetcloud/sheetcloud.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      363 2023-05-05 12:34:55.000000 sheetcloud-0.1.0.post4/sheetcloud/sheetcloud.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     7254 2023-05-05 12:34:08.000000 sheetcloud-0.1.0.post4/sheetcloud/sheets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3729 2023-05-05 12:34:08.000000 sheetcloud-0.1.0.post4/sheetcloud/templates.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1943 2023-05-05 12:34:08.000000 sheetcloud-0.1.0.post4/sheetcloud/user.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1712 2023-05-05 12:34:08.000000 sheetcloud-0.1.0.post4/sheetcloud/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 12:34:55.887761 sheetcloud-0.1.0.post4/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      150 2023-05-05 12:34:08.000000 sheetcloud-0.1.0.post4/tests/test_conn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1079 2023-05-05 12:34:08.000000 sheetcloud-0.1.0.post4/tests/test_orm.py
```

### Comparing `sheetcloud-0.1.0.post1/LICENSE` & `sheetcloud-0.1.0.post4/LICENSE`

 * *Files identical despite different names*

### Comparing `sheetcloud-0.1.0.post1/PKG-INFO` & `sheetcloud-0.1.0.post4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sheetcloud
-Version: 0.1.0.post1
+Version: 0.1.0.post4
 Summary: Sheetcloud.de | Turn Spreadsheets into a Cloud Database | Account required
 Author-email: "SheetCloud.de" <info@sheetcloud.de>
 Project-URL: Homepage, https://www.sheetcloud.de
 Project-URL: Tracker, https://github.com/sheetcloud/sheetcloud/issues
 Project-URL: Source, https://github.com/sheetcloud/sheetcloud
 Project-URL: Examples, https://github.com/sheetcloud
 Keywords: Spreadsheets,RAD,Database,Cloud
```

### Comparing `sheetcloud-0.1.0.post1/README.md` & `sheetcloud-0.1.0.post4/README.md`

 * *Files identical despite different names*

### Comparing `sheetcloud-0.1.0.post1/pyproject.toml` & `sheetcloud-0.1.0.post4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `sheetcloud-0.1.0.post1/resources/template_red_sailfish.json` & `sheetcloud-0.1.0.post4/resources/template_red_sailfish.json`

 * *Files identical despite different names*

### Comparing `sheetcloud-0.1.0.post1/sheetcloud/conn.py` & `sheetcloud-0.1.0.post4/sheetcloud/conn.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,15 +5,16 @@
 import os
 import json
 import time
 import requests
 
 from typing import *
 
-from sheetcloud.utils import pw_obfuscator
+# from sheetcloud.utils import pw_obfuscator
+from .utils import pw_obfuscator
 
 
 ENV_SHEETCLOUD_USERNAME = os.environ.get('SHEETCLOUD_USERNAME', 'missing')
 ENV_SHEETCLOUD_PASSWORD = os.environ.get('SHEETCLOUD_PASSWORD', 'missing')
 ENV_SHEETCLOUD_LICENSE = os.environ.get('SHEETCLOUD_LICENSE', 'missing')
```

### Comparing `sheetcloud-0.1.0.post1/sheetcloud/drive.py` & `sheetcloud-0.1.0.post4/sheetcloud/drive.py`

 * *Files identical despite different names*

### Comparing `sheetcloud-0.1.0.post1/sheetcloud/env.py` & `sheetcloud-0.1.0.post4/sheetcloud/env.py`

 * *Files identical despite different names*

### Comparing `sheetcloud-0.1.0.post1/sheetcloud/fun.py` & `sheetcloud-0.1.0.post4/sheetcloud/fun.py`

 * *Files identical despite different names*

### Comparing `sheetcloud-0.1.0.post1/sheetcloud/orm.py` & `sheetcloud-0.1.0.post4/sheetcloud/orm.py`

 * *Files identical despite different names*

### Comparing `sheetcloud-0.1.0.post1/sheetcloud/sheets.py` & `sheetcloud-0.1.0.post4/sheetcloud/sheets.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,17 +4,21 @@
 
 import io
 import pandas as pd
 
 from datetime import datetime, timezone
 from typing import *
 
-from sheetcloud.conn import service
-from sheetcloud.utils import get_modification_datetime_from_file, create_dir
-from sheetcloud.templates import load_template
+# from sheetcloud.conn import service
+# from sheetcloud.utils import get_modification_datetime_from_file, create_dir
+# from sheetcloud.templates import load_template
+
+from .conn import service
+from .utils import get_modification_datetime_from_file, create_dir
+
 
 SHEETCLOUD_CACHE_PATH = '.tmp'
 
 
 def list_spreadsheets() -> List[Dict]:
     res = service('/sheets/list', method='post')
     if 'sheets' in res:
```

### Comparing `sheetcloud-0.1.0.post1/sheetcloud/templates.py` & `sheetcloud-0.1.0.post4/sheetcloud/templates.py`

 * *Files identical despite different names*

### Comparing `sheetcloud-0.1.0.post1/sheetcloud/user.py` & `sheetcloud-0.1.0.post4/sheetcloud/user.py`

 * *Files identical despite different names*

### Comparing `sheetcloud-0.1.0.post1/sheetcloud/utils.py` & `sheetcloud-0.1.0.post4/sheetcloud/utils.py`

 * *Files identical despite different names*

### Comparing `sheetcloud-0.1.0.post1/tests/test_orm.py` & `sheetcloud-0.1.0.post4/tests/test_orm.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from dataclasses import dataclass, field
 from typing import Optional, List, Dict, Any
 
 import pytest
-import sheetcloud as sc
+# import sheetcloud as sc
 
 
 @dataclass
 class MySubSubDC:
     name: str = 'myname'
 
 
@@ -36,11 +36,11 @@
 
 @pytest.fixture
 def my_classes():
     yield [MyDC, MySubDC, MySubSubDC]
 
 
 
-def test_orm(my_dc_list, my_classes):
-    sc.orm.write('sheetcloud-test', my_dc_list, 'ORM_TEST')
-    objs = sc.orm.read('sheetcloud-test', 'ORM_TEST', my_classes)
-    print(objs)
+# def test_orm(my_dc_list, my_classes):
+#     sc.orm.write('sheetcloud-test', my_dc_list, 'ORM_TEST')
+#     objs = sc.orm.read('sheetcloud-test', 'ORM_TEST', my_classes)
+#     print(objs)
```

