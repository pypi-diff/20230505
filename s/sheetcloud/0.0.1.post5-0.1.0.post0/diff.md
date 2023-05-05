# Comparing `tmp/sheetcloud-0.0.1.post5.tar.gz` & `tmp/sheetcloud-0.1.0.post0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sheetcloud-0.0.1.post5.tar", last modified: Mon Mar  6 14:16:35 2023, max compression
+gzip compressed data, was "sheetcloud-0.1.0.post0.tar", last modified: Fri May  5 11:16:24 2023, max compression
```

## Comparing `sheetcloud-0.0.1.post5.tar` & `sheetcloud-0.1.0.post0.tar`

### file list

```diff
@@ -1,18 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 14:16:35.152116 sheetcloud-0.0.1.post5/
--rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-03-06 14:15:59.000000 sheetcloud-0.0.1.post5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      107 2023-03-06 14:15:59.000000 sheetcloud-0.0.1.post5/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1368 2023-03-06 14:16:35.152116 sheetcloud-0.0.1.post5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      478 2023-03-06 14:15:59.000000 sheetcloud-0.0.1.post5/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1481 2023-03-06 14:15:59.000000 sheetcloud-0.0.1.post5/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-03-06 14:15:59.000000 sheetcloud-0.0.1.post5/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 14:16:35.152116 sheetcloud-0.0.1.post5/resources/
--rw-r--r--   0 runner    (1001) docker     (123)      193 2023-03-06 14:15:59.000000 sheetcloud-0.0.1.post5/resources/endpoints.v1.json
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-06 14:16:35.152116 sheetcloud-0.0.1.post5/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 14:16:35.152116 sheetcloud-0.0.1.post5/sheetcloud/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-06 14:15:59.000000 sheetcloud-0.0.1.post5/sheetcloud/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7613 2023-03-06 14:15:59.000000 sheetcloud-0.0.1.post5/sheetcloud/conn.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 14:16:35.152116 sheetcloud-0.0.1.post5/sheetcloud/sheetcloud.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      170 2023-03-06 14:16:35.000000 sheetcloud-0.0.1.post5/sheetcloud/sheetcloud.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)      298 2023-03-06 14:15:59.000000 sheetcloud-0.0.1.post5/sheetcloud/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-06 14:16:35.152116 sheetcloud-0.0.1.post5/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-03-06 14:15:59.000000 sheetcloud-0.0.1.post5/tests/test_conn.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 11:16:24.370425 sheetcloud-0.1.0.post0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-05-05 11:14:51.000000 sheetcloud-0.1.0.post0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      107 2023-05-05 11:14:51.000000 sheetcloud-0.1.0.post0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4055 2023-05-05 11:16:24.366425 sheetcloud-0.1.0.post0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3165 2023-05-05 11:14:51.000000 sheetcloud-0.1.0.post0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1481 2023-05-05 11:14:51.000000 sheetcloud-0.1.0.post0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-05-05 11:14:51.000000 sheetcloud-0.1.0.post0/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 11:16:24.366425 sheetcloud-0.1.0.post0/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)      193 2023-05-05 11:14:51.000000 sheetcloud-0.1.0.post0/resources/endpoints.v1.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3286 2023-05-05 11:14:51.000000 sheetcloud-0.1.0.post0/resources/template_red_sailfish.json
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-05 11:16:24.370425 sheetcloud-0.1.0.post0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 11:16:24.366425 sheetcloud-0.1.0.post0/sheetcloud/
+-rw-r--r--   0 runner    (1001) docker     (123)      198 2023-05-05 11:14:51.000000 sheetcloud-0.1.0.post0/sheetcloud/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5254 2023-05-05 11:14:51.000000 sheetcloud-0.1.0.post0/sheetcloud/conn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1997 2023-05-05 11:14:51.000000 sheetcloud-0.1.0.post0/sheetcloud/drive.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1902 2023-05-05 11:14:51.000000 sheetcloud-0.1.0.post0/sheetcloud/env.py
+-rw-r--r--   0 runner    (1001) docker     (123)      832 2023-05-05 11:14:51.000000 sheetcloud-0.1.0.post0/sheetcloud/fun.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6027 2023-05-05 11:14:51.000000 sheetcloud-0.1.0.post0/sheetcloud/orm.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 11:16:24.366425 sheetcloud-0.1.0.post0/sheetcloud/sheetcloud.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      363 2023-05-05 11:16:24.000000 sheetcloud-0.1.0.post0/sheetcloud/sheetcloud.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     7153 2023-05-05 11:14:51.000000 sheetcloud-0.1.0.post0/sheetcloud/sheets.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3729 2023-05-05 11:14:51.000000 sheetcloud-0.1.0.post0/sheetcloud/templates.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1943 2023-05-05 11:14:51.000000 sheetcloud-0.1.0.post0/sheetcloud/user.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1712 2023-05-05 11:14:51.000000 sheetcloud-0.1.0.post0/sheetcloud/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 11:16:24.366425 sheetcloud-0.1.0.post0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      103 2023-05-05 11:14:51.000000 sheetcloud-0.1.0.post0/tests/test_conn.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-05-05 11:14:51.000000 sheetcloud-0.1.0.post0/tests/test_orm.py
```

### Comparing `sheetcloud-0.0.1.post5/LICENSE` & `sheetcloud-0.1.0.post0/LICENSE`

 * *Files identical despite different names*

### Comparing `sheetcloud-0.0.1.post5/pyproject.toml` & `sheetcloud-0.1.0.post0/pyproject.toml`

 * *Files identical despite different names*

