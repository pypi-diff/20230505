# Comparing `tmp/yang-vlp-0.2.14.tar.gz` & `tmp/yang-vlp-0.2.15.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "D:\SoftwareData\VSCode\Python\python_study\yang-vlp0.2\dist\.tmp-bcaia9du\yang-vlp-0.2.14.tar", last modified: Thu Apr 27 11:25:58 2023, max compression
+gzip compressed data, was "D:\SoftwareData\VSCode\Python\python_study\yang-vlp0.2\dist\.tmp-45krm8_0\yang-vlp-0.2.15.tar", last modified: Fri May  5 07:56:18 2023, max compression
```

## Comparing `yang-vlp-0.2.14.tar` & `yang-vlp-0.2.15.tar`

### file list

```diff
@@ -1,64 +1,64 @@
-drwxrwxrwx   0        0        0        0 2023-04-27 11:25:58.782108 yang-vlp-0.2.14/
--rw-rw-rw-   0        0        0     1091 2022-09-12 09:03:59.000000 yang-vlp-0.2.14/LICENSE
--rw-rw-rw-   0        0        0      294 2023-04-18 03:27:59.000000 yang-vlp-0.2.14/MANIFEST.in
--rw-rw-rw-   0        0        0     2687 2023-04-27 11:25:58.780085 yang-vlp-0.2.14/PKG-INFO
--rw-rw-rw-   0        0        0      848 2023-04-27 01:00:56.000000 yang-vlp-0.2.14/README.md
--rw-rw-rw-   0        0        0      639 2023-04-27 11:25:38.000000 yang-vlp-0.2.14/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-04-27 11:25:58.783083 yang-vlp-0.2.14/setup.cfg
--rw-rw-rw-   0        0        0      932 2023-04-27 11:25:43.000000 yang-vlp-0.2.14/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-27 11:25:58.603831 yang-vlp-0.2.14/vlppy/
-drwxrwxrwx   0        0        0        0 2023-04-27 11:25:58.605884 yang-vlp-0.2.14/vlppy/.vscode/
--rw-rw-rw-   0        0        0      478 2022-11-24 08:46:45.000000 yang-vlp-0.2.14/vlppy/.vscode/settings.json
--rw-rw-rw-   0        0        0     1093 2022-09-23 02:30:35.000000 yang-vlp-0.2.14/vlppy/LICENSE.txt
--rw-rw-rw-   0        0        0      271 2023-04-18 03:27:13.000000 yang-vlp-0.2.14/vlppy/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-27 11:25:58.621847 yang-vlp-0.2.14/vlppy/demo/
--rw-rw-rw-   0        0        0      348 2023-04-20 03:12:41.000000 yang-vlp-0.2.14/vlppy/demo/README.md
--rw-rw-rw-   0        0        0       88 2023-01-09 07:00:52.000000 yang-vlp-0.2.14/vlppy/demo/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-27 11:25:58.630843 yang-vlp-0.2.14/vlppy/demo/__pycache__/
--rw-rw-rw-   0        0        0      234 2022-09-15 01:51:51.000000 yang-vlp-0.2.14/vlppy/demo/__pycache__/__init__.cpython-39.pyc
--rw-rw-rw-   0        0        0     1938 2022-09-15 01:51:51.000000 yang-vlp-0.2.14/vlppy/demo/__pycache__/demo_main.cpython-39.pyc
--rw-rw-rw-   0        0        0     2913 2022-09-15 01:51:51.000000 yang-vlp-0.2.14/vlppy/demo/__pycache__/vlp_model.cpython-39.pyc
--rw-rw-rw-   0        0        0     1342 2023-04-27 10:40:52.000000 yang-vlp-0.2.14/vlppy/demo/demo_filter.py
--rw-rw-rw-   0        0        0     2607 2023-04-19 03:46:42.000000 yang-vlp-0.2.14/vlppy/demo/demo_main.py
--rw-rw-rw-   0        0        0     3315 2023-04-24 05:29:31.000000 yang-vlp-0.2.14/vlppy/demo/vlp_model.py
-drwxrwxrwx   0        0        0        0 2023-04-27 11:25:58.638851 yang-vlp-0.2.14/vlppy/error/
--rw-rw-rw-   0        0        0       26 2022-11-08 07:31:14.000000 yang-vlp-0.2.14/vlppy/error/__init__.py
--rw-rw-rw-   0        0        0     1619 2023-04-20 05:53:48.000000 yang-vlp-0.2.14/vlppy/error/error.py
--rw-rw-rw-   0        0        0      110 2023-04-27 11:25:32.000000 yang-vlp-0.2.14/vlppy/info.py
-drwxrwxrwx   0        0        0        0 2023-04-27 11:25:58.645848 yang-vlp-0.2.14/vlppy/io/
--rw-rw-rw-   0        0        0       26 2022-09-02 10:32:14.000000 yang-vlp-0.2.14/vlppy/io/__init__.py
--rw-rw-rw-   0        0        0     5346 2023-04-20 06:14:59.000000 yang-vlp-0.2.14/vlppy/io/io.py
-drwxrwxrwx   0        0        0        0 2023-04-27 11:25:58.658913 yang-vlp-0.2.14/vlppy/model/
--rw-rw-rw-   0        0        0       66 2022-09-19 01:30:24.000000 yang-vlp-0.2.14/vlppy/model/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-27 11:25:58.706848 yang-vlp-0.2.14/vlppy/model/__pycache__/
--rw-rw-rw-   0        0        0      282 2022-09-15 01:51:49.000000 yang-vlp-0.2.14/vlppy/model/__pycache__/__init__.cpython-39.pyc
--rw-rw-rw-   0        0        0    11287 2022-09-15 01:51:49.000000 yang-vlp-0.2.14/vlppy/model/__pycache__/filter.cpython-39.pyc
--rw-rw-rw-   0        0        0     4494 2022-09-15 01:51:50.000000 yang-vlp-0.2.14/vlppy/model/__pycache__/led.cpython-39.pyc
--rw-rw-rw-   0        0        0     9730 2022-09-15 01:51:50.000000 yang-vlp-0.2.14/vlppy/model/__pycache__/pd.cpython-39.pyc
--rw-rw-rw-   0        0        0     9684 2022-09-15 01:51:50.000000 yang-vlp-0.2.14/vlppy/model/__pycache__/room.cpython-39.pyc
--rw-rw-rw-   0        0        0     6151 2023-04-27 07:56:52.000000 yang-vlp-0.2.14/vlppy/model/led.py
--rw-rw-rw-   0        0        0    18271 2023-04-27 11:24:31.000000 yang-vlp-0.2.14/vlppy/model/pd.py
--rw-rw-rw-   0        0        0    17040 2023-04-27 01:50:02.000000 yang-vlp-0.2.14/vlppy/model/room.py
-drwxrwxrwx   0        0        0        0 2023-04-27 11:25:58.726847 yang-vlp-0.2.14/vlppy/setting/
--rw-rw-rw-   0        0        0       40 2022-05-31 05:29:34.000000 yang-vlp-0.2.14/vlppy/setting/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-27 11:25:58.734853 yang-vlp-0.2.14/vlppy/setting/__pycache__/
--rw-rw-rw-   0        0        0      196 2022-05-31 05:35:37.000000 yang-vlp-0.2.14/vlppy/setting/__pycache__/__init__.cpython-39.pyc
--rw-rw-rw-   0        0        0     2526 2022-09-15 01:51:51.000000 yang-vlp-0.2.14/vlppy/setting/__pycache__/json_setting.cpython-39.pyc
--rw-rw-rw-   0        0        0     2903 2023-04-20 06:15:26.000000 yang-vlp-0.2.14/vlppy/setting/json_setting.py
--rw-rw-rw-   0        0        0     2208 2022-12-08 07:54:09.000000 yang-vlp-0.2.14/vlppy/setting/settings.json
-drwxrwxrwx   0        0        0        0 2023-04-27 11:25:58.748228 yang-vlp-0.2.14/vlppy/signal/
--rw-rw-rw-   0        0        0       48 2023-01-09 06:55:15.000000 yang-vlp-0.2.14/vlppy/signal/__init__.py
--rw-rw-rw-   0        0        0    10010 2023-04-20 06:24:52.000000 yang-vlp-0.2.14/vlppy/signal/filter.py
--rw-rw-rw-   0        0        0     3719 2023-04-27 10:42:14.000000 yang-vlp-0.2.14/vlppy/signal/plot.py
-drwxrwxrwx   0        0        0        0 2023-04-27 11:25:58.755239 yang-vlp-0.2.14/vlppy/tools/
--rw-rw-rw-   0        0        0       26 2023-04-18 03:21:34.000000 yang-vlp-0.2.14/vlppy/tools/__init__.py
--rw-rw-rw-   0        0        0      273 2023-04-18 03:22:02.000000 yang-vlp-0.2.14/vlppy/tools/decorator.py
-drwxrwxrwx   0        0        0        0 2023-04-27 11:25:58.761242 yang-vlp-0.2.14/vlppy/vis/
--rw-rw-rw-   0        0        0       26 2022-06-07 05:02:10.000000 yang-vlp-0.2.14/vlppy/vis/__init__.py
--rw-rw-rw-   0        0        0     3653 2023-04-19 02:52:08.000000 yang-vlp-0.2.14/vlppy/vis/vis.py
-drwxrwxrwx   0        0        0        0 2023-04-27 11:25:58.778085 yang-vlp-0.2.14/yang_vlp.egg-info/
--rw-rw-rw-   0        0        0     2687 2023-04-27 11:25:58.000000 yang-vlp-0.2.14/yang_vlp.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1281 2023-04-27 11:25:58.000000 yang-vlp-0.2.14/yang_vlp.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-27 11:25:58.000000 yang-vlp-0.2.14/yang_vlp.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       59 2023-04-27 11:25:58.000000 yang-vlp-0.2.14/yang_vlp.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-04-27 11:25:58.000000 yang-vlp-0.2.14/yang_vlp.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-05 07:56:18.390613 yang-vlp-0.2.15/
+-rw-rw-rw-   0        0        0     1091 2022-09-12 09:03:59.000000 yang-vlp-0.2.15/LICENSE
+-rw-rw-rw-   0        0        0      294 2023-04-18 03:27:59.000000 yang-vlp-0.2.15/MANIFEST.in
+-rw-rw-rw-   0        0        0     2687 2023-05-05 07:56:18.388587 yang-vlp-0.2.15/PKG-INFO
+-rw-rw-rw-   0        0        0      848 2023-04-27 01:00:56.000000 yang-vlp-0.2.15/README.md
+-rw-rw-rw-   0        0        0      639 2023-05-05 07:26:56.000000 yang-vlp-0.2.15/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-05 07:56:18.391591 yang-vlp-0.2.15/setup.cfg
+-rw-rw-rw-   0        0        0      932 2023-05-05 07:27:01.000000 yang-vlp-0.2.15/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-05 07:56:18.170583 yang-vlp-0.2.15/vlppy/
+drwxrwxrwx   0        0        0        0 2023-05-05 07:56:18.175588 yang-vlp-0.2.15/vlppy/.vscode/
+-rw-rw-rw-   0        0        0      478 2022-11-24 08:46:45.000000 yang-vlp-0.2.15/vlppy/.vscode/settings.json
+-rw-rw-rw-   0        0        0     1093 2022-09-23 02:30:35.000000 yang-vlp-0.2.15/vlppy/LICENSE.txt
+-rw-rw-rw-   0        0        0      271 2023-04-18 03:27:13.000000 yang-vlp-0.2.15/vlppy/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-05 07:56:18.192587 yang-vlp-0.2.15/vlppy/demo/
+-rw-rw-rw-   0        0        0      348 2023-04-20 03:12:41.000000 yang-vlp-0.2.15/vlppy/demo/README.md
+-rw-rw-rw-   0        0        0       88 2023-01-09 07:00:52.000000 yang-vlp-0.2.15/vlppy/demo/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-05 07:56:18.208582 yang-vlp-0.2.15/vlppy/demo/__pycache__/
+-rw-rw-rw-   0        0        0      234 2022-09-15 01:51:51.000000 yang-vlp-0.2.15/vlppy/demo/__pycache__/__init__.cpython-39.pyc
+-rw-rw-rw-   0        0        0     1938 2022-09-15 01:51:51.000000 yang-vlp-0.2.15/vlppy/demo/__pycache__/demo_main.cpython-39.pyc
+-rw-rw-rw-   0        0        0     2913 2022-09-15 01:51:51.000000 yang-vlp-0.2.15/vlppy/demo/__pycache__/vlp_model.cpython-39.pyc
+-rw-rw-rw-   0        0        0     1342 2023-04-27 10:40:52.000000 yang-vlp-0.2.15/vlppy/demo/demo_filter.py
+-rw-rw-rw-   0        0        0     2607 2023-04-19 03:46:42.000000 yang-vlp-0.2.15/vlppy/demo/demo_main.py
+-rw-rw-rw-   0        0        0     3188 2023-05-05 07:55:54.000000 yang-vlp-0.2.15/vlppy/demo/vlp_model.py
+drwxrwxrwx   0        0        0        0 2023-05-05 07:56:18.226582 yang-vlp-0.2.15/vlppy/error/
+-rw-rw-rw-   0        0        0       26 2022-11-08 07:31:14.000000 yang-vlp-0.2.15/vlppy/error/__init__.py
+-rw-rw-rw-   0        0        0     1619 2023-04-20 05:53:48.000000 yang-vlp-0.2.15/vlppy/error/error.py
+-rw-rw-rw-   0        0        0      110 2023-05-05 07:27:09.000000 yang-vlp-0.2.15/vlppy/info.py
+drwxrwxrwx   0        0        0        0 2023-05-05 07:56:18.231585 yang-vlp-0.2.15/vlppy/io/
+-rw-rw-rw-   0        0        0       26 2022-09-02 10:32:14.000000 yang-vlp-0.2.15/vlppy/io/__init__.py
+-rw-rw-rw-   0        0        0     5346 2023-04-20 06:14:59.000000 yang-vlp-0.2.15/vlppy/io/io.py
+drwxrwxrwx   0        0        0        0 2023-05-05 07:56:18.243619 yang-vlp-0.2.15/vlppy/model/
+-rw-rw-rw-   0        0        0       66 2022-09-19 01:30:24.000000 yang-vlp-0.2.15/vlppy/model/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-05 07:56:18.285583 yang-vlp-0.2.15/vlppy/model/__pycache__/
+-rw-rw-rw-   0        0        0      282 2022-09-15 01:51:49.000000 yang-vlp-0.2.15/vlppy/model/__pycache__/__init__.cpython-39.pyc
+-rw-rw-rw-   0        0        0    11287 2022-09-15 01:51:49.000000 yang-vlp-0.2.15/vlppy/model/__pycache__/filter.cpython-39.pyc
+-rw-rw-rw-   0        0        0     4494 2022-09-15 01:51:50.000000 yang-vlp-0.2.15/vlppy/model/__pycache__/led.cpython-39.pyc
+-rw-rw-rw-   0        0        0     9730 2022-09-15 01:51:50.000000 yang-vlp-0.2.15/vlppy/model/__pycache__/pd.cpython-39.pyc
+-rw-rw-rw-   0        0        0     9684 2022-09-15 01:51:50.000000 yang-vlp-0.2.15/vlppy/model/__pycache__/room.cpython-39.pyc
+-rw-rw-rw-   0        0        0     6154 2023-05-05 07:26:43.000000 yang-vlp-0.2.15/vlppy/model/led.py
+-rw-rw-rw-   0        0        0    17952 2023-05-05 07:54:41.000000 yang-vlp-0.2.15/vlppy/model/pd.py
+-rw-rw-rw-   0        0        0    17803 2023-05-05 07:23:46.000000 yang-vlp-0.2.15/vlppy/model/room.py
+drwxrwxrwx   0        0        0        0 2023-05-05 07:56:18.305587 yang-vlp-0.2.15/vlppy/setting/
+-rw-rw-rw-   0        0        0       40 2022-05-31 05:29:34.000000 yang-vlp-0.2.15/vlppy/setting/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-05 07:56:18.319585 yang-vlp-0.2.15/vlppy/setting/__pycache__/
+-rw-rw-rw-   0        0        0      196 2022-05-31 05:35:37.000000 yang-vlp-0.2.15/vlppy/setting/__pycache__/__init__.cpython-39.pyc
+-rw-rw-rw-   0        0        0     2526 2022-09-15 01:51:51.000000 yang-vlp-0.2.15/vlppy/setting/__pycache__/json_setting.cpython-39.pyc
+-rw-rw-rw-   0        0        0     2903 2023-04-20 06:15:26.000000 yang-vlp-0.2.15/vlppy/setting/json_setting.py
+-rw-rw-rw-   0        0        0     2208 2022-12-08 07:54:09.000000 yang-vlp-0.2.15/vlppy/setting/settings.json
+drwxrwxrwx   0        0        0        0 2023-05-05 07:56:18.357618 yang-vlp-0.2.15/vlppy/signal/
+-rw-rw-rw-   0        0        0       48 2023-01-09 06:55:15.000000 yang-vlp-0.2.15/vlppy/signal/__init__.py
+-rw-rw-rw-   0        0        0    10010 2023-04-20 06:24:52.000000 yang-vlp-0.2.15/vlppy/signal/filter.py
+-rw-rw-rw-   0        0        0     3719 2023-04-27 10:42:14.000000 yang-vlp-0.2.15/vlppy/signal/plot.py
+drwxrwxrwx   0        0        0        0 2023-05-05 07:56:18.362586 yang-vlp-0.2.15/vlppy/tools/
+-rw-rw-rw-   0        0        0       26 2023-04-18 03:21:34.000000 yang-vlp-0.2.15/vlppy/tools/__init__.py
+-rw-rw-rw-   0        0        0      273 2023-04-18 03:22:02.000000 yang-vlp-0.2.15/vlppy/tools/decorator.py
+drwxrwxrwx   0        0        0        0 2023-05-05 07:56:18.368592 yang-vlp-0.2.15/vlppy/vis/
+-rw-rw-rw-   0        0        0       26 2022-06-07 05:02:10.000000 yang-vlp-0.2.15/vlppy/vis/__init__.py
+-rw-rw-rw-   0        0        0     3653 2023-04-19 02:52:08.000000 yang-vlp-0.2.15/vlppy/vis/vis.py
+drwxrwxrwx   0        0        0        0 2023-05-05 07:56:18.385586 yang-vlp-0.2.15/yang_vlp.egg-info/
+-rw-rw-rw-   0        0        0     2687 2023-05-05 07:56:18.000000 yang-vlp-0.2.15/yang_vlp.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1281 2023-05-05 07:56:18.000000 yang-vlp-0.2.15/yang_vlp.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-05 07:56:18.000000 yang-vlp-0.2.15/yang_vlp.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       59 2023-05-05 07:56:18.000000 yang-vlp-0.2.15/yang_vlp.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-05-05 07:56:18.000000 yang-vlp-0.2.15/yang_vlp.egg-info/top_level.txt
```

### Comparing `yang-vlp-0.2.14/LICENSE` & `yang-vlp-0.2.15/LICENSE`

 * *Files identical despite different names*

### Comparing `yang-vlp-0.2.14/PKG-INFO` & `yang-vlp-0.2.15/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yang-vlp
-Version: 0.2.14
+Version: 0.2.15
 Summary: Construction of visible light positioning model
 Home-page: https://gitee.com/yangwuju/yang_vlp
 Author: yangwuju
 Author-email: yangwuju <1424134319@qq.com>
 License: Copyright (c) 2018 The Python Packaging Authority
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `yang-vlp-0.2.14/README.md` & `yang-vlp-0.2.15/README.md`

 * *Files identical despite different names*

### Comparing `yang-vlp-0.2.14/pyproject.toml` & `yang-vlp-0.2.15/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "yang-vlp"
-version = "0.2.14"
+version = "0.2.15"
 authors = [
   { name="yangwuju", email="1424134319@qq.com" },
 ]
 description = "Construction of visible light positioning model"
 readme = "README.md"
 license = { file="LICENSE" }
 requires-python = ">=3.5"
```

### Comparing `yang-vlp-0.2.14/setup.py` & `yang-vlp-0.2.15/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 path = os.path.join(CUR_PATH, 'build')
 if os.path.isdir(path):
     print('INFO del dir ', path) 
     shutil.rmtree(path)
 
 setup(
     name = 'yang-vlp', #应用名
-    version = '0.2.14',  #版本号
+    version = '0.2.15',  #版本号
     description = 'Construction of visible light positioning model', 
     packages = find_packages(),  #包括在安装包内的Python包
     include_package_data = True, #启用清单文件MANIFEST.in,包含数据文件
     # exclude_package_data = {'docs':['1.txt']},  #排除文件
     install_requires = [#自动安装依赖
         'numpy>=1.19.0',
         'matplotlib>=3.5.0',
```

### Comparing `yang-vlp-0.2.14/vlppy/LICENSE.txt` & `yang-vlp-0.2.15/vlppy/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `yang-vlp-0.2.14/vlppy/demo/__pycache__/demo_main.cpython-39.pyc` & `yang-vlp-0.2.15/vlppy/demo/__pycache__/demo_main.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `yang-vlp-0.2.14/vlppy/demo/__pycache__/vlp_model.cpython-39.pyc` & `yang-vlp-0.2.15/vlppy/demo/__pycache__/vlp_model.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `yang-vlp-0.2.14/vlppy/demo/demo_filter.py` & `yang-vlp-0.2.15/vlppy/demo/demo_filter.py`

 * *Files identical despite different names*

### Comparing `yang-vlp-0.2.14/vlppy/demo/demo_main.py` & `yang-vlp-0.2.15/vlppy/demo/demo_main.py`

 * *Files identical despite different names*

### Comparing `yang-vlp-0.2.14/vlppy/demo/vlp_model.py` & `yang-vlp-0.2.15/vlppy/demo/vlp_model.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import matplotlib.pyplot as plt
+import numpy as np
 from ..model import LED
 from ..model import PD
 from ..model import Room
 
 class VLP_Model:
     def __init__(self,**kwargs):
         # 房间
@@ -12,18 +13,18 @@
         # PD
         pd = kwargs["PD_Info"] 
         pd1 = pd["PD1"]   
         pd2 = pd["PD2"]   
         pd3 = pd["PD3"]   
         pd4 = pd["PD4"]   
         
-        pd1_pos, (alpha1,beta1) = PD.recv_frame_model(l=pd["l"], alpha=pd1["alpha"], beta=pd1["beta"], center_tp_pos=self.room.tp_grid_pos)  # PD位置和倾斜角
-        pd2_pos, (alpha2,beta2) = PD.recv_frame_model(l=pd["l"], alpha=pd2["alpha"], beta=pd2["beta"], center_tp_pos=self.room.tp_grid_pos) 
-        pd3_pos, (alpha3,beta3) = PD.recv_frame_model(l=pd["l"], alpha=pd3["alpha"], beta=pd3["beta"], center_tp_pos=self.room.tp_grid_pos)  
-        pd4_pos, (alpha4,beta4) = PD.recv_frame_model(l=pd["l"], alpha=pd4["alpha"], beta=pd4["beta"], center_tp_pos=self.room.tp_grid_pos) 
+        pd1_pos, (alpha1,beta1) = PD.recv_frame_model(l=pd["l"], alpha=pd1["alpha"], beta=pd1["beta"], center_tp_pos=self.room.tp_pos)  # PD位置和倾斜角
+        pd2_pos, (alpha2,beta2) = PD.recv_frame_model(l=pd["l"], alpha=pd2["alpha"], beta=pd2["beta"], center_tp_pos=self.room.tp_pos) 
+        pd3_pos, (alpha3,beta3) = PD.recv_frame_model(l=pd["l"], alpha=pd3["alpha"], beta=pd3["beta"], center_tp_pos=self.room.tp_pos)  
+        pd4_pos, (alpha4,beta4) = PD.recv_frame_model(l=pd["l"], alpha=pd4["alpha"], beta=pd4["beta"], center_tp_pos=self.room.tp_pos) 
         
         self.pd1 = PD(n=pd["n"], fov=pd["fov"], Ar=pd["Ar"], Ts=pd["Ts"], pos=pd1_pos, alpha=alpha1, beta=beta1) 
         self.pd2 = PD(n=pd["n"], fov=pd["fov"], Ar=pd["Ar"], Ts=pd["Ts"], pos=pd2_pos, alpha=alpha2, beta=beta2)
         self.pd3 = PD(n=pd["n"], fov=pd["fov"], Ar=pd["Ar"], Ts=pd["Ts"], pos=pd3_pos, alpha=alpha3, beta=beta3) 
         self.pd4 = PD(n=pd["n"], fov=pd["fov"], Ar=pd["Ar"], Ts=pd["Ts"], pos=pd4_pos, alpha=alpha4, beta=beta4) 
         
         # LED
@@ -35,38 +36,30 @@
         led1 = led["LED1"]
         self.led1 = LED(theta=led["theta"], signal=led["signal"], **led1, t=self.t)
 
     def get_data(self):
         """计算PD接收LED功率
         outshape: 输出数据形状,默认shape=(n,)(为None不改变形状)
         """
-        # PD接收各LED的信号 (l,w,h)
-        PD1_LED1 = self.pd1.recv_led_signal(led=self.led1, room=self.room) 
-        PD2_LED1 = self.pd2.recv_led_signal(led=self.led1, room=self.room)
-        PD3_LED1 = self.pd3.recv_led_signal(led=self.led1, room=self.room) 
-        PD4_LED1 = self.pd4.recv_led_signal(led=self.led1, room=self.room) 
+        # PD接收各LED的信号 (l*w*h)
+        P_PD1 = self.pd1.recv_led_signal(led=self.led1, room=self.room) 
+        P_PD2 = self.pd2.recv_led_signal(led=self.led1, room=self.room)
+        P_PD3 = self.pd3.recv_led_signal(led=self.led1, room=self.room) 
+        P_PD4 = self.pd4.recv_led_signal(led=self.led1, room=self.room) 
 
-        P_PD1 = PD1_LED1.reshape(-1)  # (l,w,h) ->(l*w*h)
-        P_PD2 = PD2_LED1.reshape(-1)
-        P_PD3 = PD3_LED1.reshape(-1)
-        P_PD4 = PD4_LED1.reshape(-1)
-
-        xr,yr,zr = self.room.tp_grid_pos
-        Xr = xr.reshape(-1)  #（l*w*h）
-        Yr = yr.reshape(-1)  
-        Zr = zr.reshape(-1)  
+        xr, yr, zr = np.split(self.room.tp_pos, indices_or_sections=3, axis=-1) # 在最后一个维度上进行分割操作#（l*w*h,3） -> 3*（l*w*h,1)
+        Xr, Yr, Zr = xr.flatten(), yr.flatten(), zr.flatten()  #（l*w*h）
         return (P_PD1,P_PD2,P_PD3,P_PD4,Xr,Yr,Zr)  
       
     def show(self,z,savepath=...,showfig=True):
         """绘图
         z: 第三维度数据
         """
-        xr,yr,_ = self.room.tp_grid_pos
-        assert xr.ndim == 2
-        z = z.reshape(xr.shape)  
+        xr, yr, _ = self.room.tp_grid
+        z = np.reshape(z, xr.shape)  
         ax = plt.axes(projection='3d')
         ax.plot_surface(xr, yr, z, cmap='viridis', edgecolor='none')
         ax.set_xlabel('X')
         ax.set_ylabel('Y')
         ax.set_zlabel('Z')
         if savepath != ...:
             plt.savefig(savepath)
```

### Comparing `yang-vlp-0.2.14/vlppy/error/error.py` & `yang-vlp-0.2.15/vlppy/error/error.py`

 * *Files identical despite different names*

### Comparing `yang-vlp-0.2.14/vlppy/io/io.py` & `yang-vlp-0.2.15/vlppy/io/io.py`

 * *Files identical despite different names*

### Comparing `yang-vlp-0.2.14/vlppy/model/__pycache__/filter.cpython-39.pyc` & `yang-vlp-0.2.15/vlppy/model/__pycache__/filter.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `yang-vlp-0.2.14/vlppy/model/__pycache__/led.cpython-39.pyc` & `yang-vlp-0.2.15/vlppy/model/__pycache__/led.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `yang-vlp-0.2.14/vlppy/model/__pycache__/pd.cpython-39.pyc` & `yang-vlp-0.2.15/vlppy/model/__pycache__/pd.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `yang-vlp-0.2.14/vlppy/model/__pycache__/room.cpython-39.pyc` & `yang-vlp-0.2.15/vlppy/model/__pycache__/room.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `yang-vlp-0.2.14/vlppy/model/led.py` & `yang-vlp-0.2.15/vlppy/model/led.py`

 * *Files 3% similar despite different names*

```diff
@@ -135,23 +135,23 @@
             raise VLPSequenceLenError(o, 3)
         self._origin = tuple(o)
 
     @property
     def pos(self) -> tuple:
         """获取相对位置(参考位置相对与原点的相对位置)
         """
-        return tuple(i+j for i,j in zip(self._pos,self.origin))
+        return self._pos + self.origin
     
     @pos.setter
     def pos(self, pos:tuple):
         """设置参考位置
         """
-        if not len(pos) == 3:
-            raise VLPSequenceLenError(pos,3)
-        self._pos = tuple(pos)
+        if not np.shape(pos)[-1] == 3:
+            raise VLPSequenceLenError(np.shape(pos)[-1],3)
+        self._pos = np.asarray(pos)
         
     @property
     def Nv(self):  
         """获取LED单位法向量  
         """  
         return self._Nv/np.linalg.norm(self._Nv)
```

### Comparing `yang-vlp-0.2.14/vlppy/model/pd.py` & `yang-vlp-0.2.15/vlppy/model/pd.py`

 * *Files 26% similar despite different names*

```diff
@@ -43,225 +43,216 @@
         """接收机模型:PD支架模型(倾斜PD和中心参考点位置关系)
         Params
             l: 倾斜PD到中心水平PD(参考点)的长度(单位:米)
             alpha: PD倾斜面的方位角(单位:度)
             beta: PD倾斜面倾斜角(单位:度)
             center_tp_pos: 水平中心测试点位置
         Return
-            (xr,yr,zr): 倾斜PD位置
+            pos: 倾斜PD位置
             (alpha,beta): 倾斜PD的方位角和倾斜角(单位:度)
         """
-        [x0, y0, z0] = np.asarray(center_tp_pos, dtype=np.float)  #水平中心测试点位置
+        x0, y0, z0 = np.split(center_tp_pos, indices_or_sections=3, axis=-1)
+        x0, y0, z0 = x0.flatten(), y0.flatten(), z0.flatten()
+
         # 倾斜PD的方位角和倾斜角,角度制转弧度制
         alpha_rad, beta_rad = np.radians([alpha, beta])
 
         xr = x0 + l * np.cos(alpha_rad) * np.cos(beta_rad) 
         yr = y0 + l * np.sin(alpha_rad) * np.cos(beta_rad)
         zr = z0 + l * np.sin(beta_rad)
+        pos = np.stack([xr,yr,zr], axis=-1) # 在最后一维度上堆叠
         
         # PD的方位角和PD倾斜面的方位角反向
         # PD的倾斜角和PD倾斜面的倾斜角相等
         pd_alpha = alpha+180  
         pd_alpha = pd_alpha-360 if pd_alpha > 360 else pd_alpha if pd_alpha >= 0 else pd_alpha+360 # 转到区间 [0,360)
-        return (xr,yr,zr), (alpha,beta) 
+        
+        return pos, (alpha,beta)
 
     @staticmethod
     def recv_surface_model(r:Union[Number,tuple], alpha, beta, center_tp_pos:tuple):
         """接收机模型:安全帽椭球面(倾斜PD和中心参考点位置关系)
         Params
             r: 曲球面半径(单位:米)
             alpha:倾斜PD方位角(单位:度)
             beta:  倾斜PD倾斜角(单位:度)
             center_tp_pos: 椭球面顶部中心测试点位置
         Return
-            (xr,yr,zr): 倾斜PD位置
+            pos: 倾斜PD位置
             (alpha,beta): 倾斜PD的方位角和倾斜角(单位:度)
         """
-        r=tuple(r)
         r = np.asarray(r)
         assert r.size in (1,3)
         a, b, c = np.full(shape=(3), fill_value=r) if r.size == 1 else r
 
         # 倾斜PD的方位角和倾斜角
         alpha_rad, beta_rad = np.radians([alpha,beta]) # 角度制转弧度制
 
         if not 0 <= beta_rad <= 90: # 限定
             raise VLPValueRangeError(beta, 0, 90)
         
-        [x0, y0, z0] = np.asarray(center_tp_pos, dtype=np.float) #测试点位置
+        x0, y0, z0 = np.split(center_tp_pos, indices_or_sections=3, axis=-1)
+        x0, y0, z0 = x0.flatten(), y0.flatten(), z0.flatten()
 
         # 倾斜PD位置
         xr = x0 + a * np.cos(alpha_rad) * np.sin(beta_rad)
         yr = y0 + b * np.sin(alpha_rad) * np.sin(beta_rad)
         zr = z0 - c * (1 - np.cos(beta_rad))
+        pos = np.stack([xr,yr,zr], axis=-1) # 在最后一维度上堆叠
 
         # PD的方位角和PD倾斜面的方位角相等
         # PD的倾斜角和PD倾斜面的倾斜角相等
-        return (xr,yr,zr), (alpha, beta)
+        return pos, (alpha,beta)
 
     @staticmethod
     def recv_hemisphere_model(r, l, alpha, center_tp_pos:tuple):
         """接收机模型:半球面模型(倾斜PD和中心参考点位置关系)
         Params
             r: 曲球面半径(单位:米)
             l: 倾斜PD到顶部中心(参考点)的弧长(单位:米)   
             alpha:倾斜PD方位角(单位:度) 
             center_tp_pos: 测试点位置 
         Return
-            (xr,yr,zr): 倾斜PD位置
+            pos: 倾斜PD位置
             (alpha,beta): 倾斜PD的方位角和倾斜角(单位:度)
         """
         # 倾斜PD的方位角和倾斜角
         beta_rad = l/r   # PD倾斜角
         beta = np.degrees(beta_rad) # 弧度制转角度制
         return PD.recv_surface_model(r, alpha, beta, center_tp_pos)
 
     def recv_led_radiation_intensity(self, led:LED):
         """计算LED辐射强度(LOS链路):
         Parameters
             led: LED实例化
         Return 
             LOS链路LED辐射强度
         """
-        # 坐标shape转换,使其可以进行矩阵乘法运算
-        led_pos = np.stack(led.pos, axis=-1)  # (3,..) -> (..,3)
-        pd_pos = np.stack(self.pos, axis=-1)  # PD位置 (3,l,w,h) -> (.l,w,h,3)
-
-        Vt_r = pd_pos - led_pos               # LED到PD的方向向量 (l,w,h,3)
-        d = np.linalg.norm(Vt_r,axis=-1)      # LED到PD的方向向量的模 (l,w,h)
-        cos_led_t_angle_rad_rad = np.sum(Vt_r*led.Nv, axis=-1) / d # LED发射角的余弦值 (l,w,h)
+        Vt_r = self.pos - led.pos               # LED到PD的方向向量 (l*w*h,3)
+        d = np.linalg.norm(Vt_r,axis=-1)      # LED到PD的方向向量的模 (l*w*h)
+        cos_led_t_angle_rad_rad = np.sum(Vt_r*led.Nv, axis=-1) / d # LED发射角的余弦值 (l*w*h)
 
-        R0 = ((led.m + 1)  / (2 * np.pi)) * cos_led_t_angle_rad_rad**led.m  # 辐射强度模型 (l,w,h)
+        R0 = ((led.m + 1)  / (2 * np.pi)) * cos_led_t_angle_rad_rad**led.m  # 辐射强度模型 (l*w*h)
 
         """
         H0 = H0.flatten() #打平 (l,w) -> (l*w,)
         return np.array([np.convolve(h,led.send_signal) for h in H0])  #卷积 (l*w,npt)
               <=> np.array([h * led.send_signal for h in H0])          #相乘 (l*w,npt) 
         """
-        R0 = np.expand_dims(R0,-1) # 在最后一维扩充一个维度 (l,w,h) -> (l,w,h,1)  <=> H0.reshape(l,w,h,1) <=> H0[...,np.newaxis]
-        radiation_intensity = R0 * led.signal # LED辐射强度[广播机制 (l,w,h,1) * (npt) -> (l,w,h,npt) * (l,w,h,npt) = (l,w,h,npt)]
-        return np.squeeze(radiation_intensity)  # (l,w,h,npt).如果npt==1,则返回形状为(l,w,h)
+        R0 = np.expand_dims(R0,-1) # 在最后一维扩充一个维度 (l*w*h) -> (l*w*h,1)  <=> H0.reshape(l*w*h,1) <=> H0[...,np.newaxis]
+        radiation_intensity = R0 * led.signal # LED辐射强度[广播机制 (l*w*h,1) * (npt) -> (l*w*h,npt) * (l*w*h,npt) = (l*w*h,npt)]
+        return np.squeeze(radiation_intensity)  # (l*w*h,npt).如果npt==1,则返回形状为(l*w*h)
 
     def recv_los_led_signal(self, led:LED):
         """计算PD接收LED信号(LOS链路):
         Parameters
             led: LED实例化
         Return 
             LOS链路中PD探测器接收LED信号
         """
-        # 坐标shape转换,使其可以进行矩阵乘法运算
-        led_pos = np.stack(led.pos, axis=-1)  # (3,..) -> (..,3)
-        pd_pos = np.stack(self.pos, axis=-1)  # (3,l,w,h) -> (l,w,h,3)
-
         # LED发射端
-        Vt_r = pd_pos - led_pos                     # LED到PD的方向向量 (l,w,h,3)
-        d = np.linalg.norm(Vt_r,axis=-1)            # 求模:LED到PD的方向向量的模 (l,w,h)
-        cos_led_t_angle_rad_rad = np.sum(Vt_r*led.Nv, axis=-1) / d # LED发射角的余弦值 (l,w,h)
+        Vt_r = self.pos - led.pos                     # LED到PD的方向向量 (l*w*h,3)
+        d = np.linalg.norm(Vt_r,axis=-1)            # 求模:LED到PD的方向向量的模 (l*w*h)
+        cos_led_t_angle_rad_rad = np.sum(Vt_r*led.Nv, axis=-1) / d # LED发射角的余弦值 (l*w*h)
 
         # PD接收端
-        Vr_t = -Vt_r # PD到LED的方向向量 (l,w,h，3)
-        cos_pd_r_angle_rad = np.sum(Vr_t*self.Nv, axis=-1) / d     # PD接收角的余弦值 (l,w,h) 
+        Vr_t = -Vt_r # PD到LED的方向向量 (l*w*h,3)
+        cos_pd_r_angle_rad = np.sum(Vr_t*self.Nv, axis=-1) / d     # PD接收角的余弦值 (l*w*h) 
 
         # PD入射角
-        pd_r_angle_rad = np.arccos(cos_pd_r_angle_rad) # PD接收器入射角的大小(弧度制) (l,w,h)
-        pd_r_angle = np.degrees(pd_r_angle_rad)        # 弧度制转为角度制 (l,w,h)
+        pd_r_angle_rad = np.arccos(cos_pd_r_angle_rad) # PD接收器入射角的大小(弧度制) (l*w*h)
+        pd_r_angle = np.degrees(pd_r_angle_rad)        # 弧度制转为角度制 (l*w*h)
 
         # 计算信道增益
-        H0 = (((led.m + 1) * self.Ar) / (2 * np.pi * d**2)) * cos_led_t_angle_rad_rad**led.m * cos_pd_r_angle_rad * self.Ts * self.G_Con # 信道增益 (l,w,h)
-        H0 = np.where((pd_r_angle>=0) & (pd_r_angle<=self.fov), H0, 0)  # 视场内信道增益 (l,w,h) <=> np.place(H0,(phi>=0)&(phi<=pd.fov),0)
+        H0 = (((led.m + 1) * self.Ar) / (2 * np.pi * d**2)) * cos_led_t_angle_rad_rad**led.m * cos_pd_r_angle_rad * self.Ts * self.G_Con # 信道增益 (l*w*h)
+        H0 = np.where((pd_r_angle>=0) & (pd_r_angle<=self.fov), H0, 0)  # 视场内信道增益 (l*w*h) <=> np.place(H0,(phi>=0)&(phi<=pd.fov),0)
 
         # 以下是为了兼容交直流信号
         """
         H0 = H0.flatten() #打平 (l,w) -> (l*w,)
         return np.array([np.convolve(h,led.send_signal) for h in H0])  #卷积 (l*w,npt)
               <=> np.array([h * led.send_signal for h in H0])          #相乘 (l*w,npt) 
         """
-        H0 = np.expand_dims(H0,-1) # 在最后一维扩充一个维度 (l,w,h) -> (l,w,h,1)  <=> H0.reshape(l,w,h,1) <=> H0[...,np.newaxis]
-        recv_signal = H0 * led.signal # PD接收信号 [广播机制 (l,w,h,1) * (npt) -> (l,w,h,npt) * (l,w,h,npt) = (l,w,h,npt)]
+        H0 = np.expand_dims(H0,-1) # 在最后一维扩充一个维度 (l*w*h) -> (l*w*h,1)  <=> H0.reshape(l*w*h,1) <=> H0[...,np.newaxis]
+        recv_signal = H0 * led.signal # PD接收信号 [广播机制 (l*w*h,1) * (npt) -> (l*w*h,npt) * (l*w*h,npt) = (l*w*h,npt)]
         return np.squeeze(recv_signal) # (l,w,h,npt).如果npt==1,则返回形状为(l,w,h)
       
     def recv_nlos_led_signal(self, led:LED, room:Room):
         """计算PD接收LED一次反射信号(NLOS链路):
         Params
             led: LED实例化
             room: Room实例化
         Return 
             NLOS链路中PD探测器接收LED一次反射信号
         """
-        pd_pos = np.asarray(self.pos)
-        # 对PD坐标张量扩充两个维度,以便使用广播
-        pd_pos = pd_pos[..., np.newaxis, np.newaxis]  # (l,w,h,1,1) 
-
-        # 坐标shape转换,使其可以进行矩阵乘法运算
-        led_pos = np.stack(led.pos, axis=-1) # (3,..) -> (..,3)
-        pd_pos = np.stack(pd_pos, axis=-1)  # (3,l,w,h,1,1) -> (l,w,h,1,1,3)
+        # 对PD坐标张量扩充维度,以便使用广播
+        pd_pos = np.expand_dims(self.pos,axis=-2)  # (l*w*h,3) -> (l*w*h,1,3) 
+        # print(f"{pd_pos.shape=}")
 
         H0 = 0  #反射（LOS）链路信道增益
-        # 遍历每一面反射墙壁参数:((l1,w1),(l1,w1),(l1,w1)), ((l1,w1),(l1,w1))
-        for i, ((xw, yw, zw), (w_alpha, w_beta)) in enumerate(room.get_reflect_wall_args()):
-            # 坐标shape转换,使其可以进行矩阵乘法运算
-            wall_pos = np.stack([xw, yw, zw], axis=-1)  # (3,l1,w1) -> (l1,w1,3)
-
+        # 遍历每一面反射墙壁参数:(l1*w1,3),(l1*w1,2)
+        for i, (wall_pos, angle) in enumerate(room.get_reflect_wall_args()):
+            w_alpha, w_beta = np.split(angle,indices_or_sections=2, axis=-1) # (l1*w1,2) -> (l1*w1,1) + (l1*w1,1)
+            w_alpha, w_beta = w_alpha.flatten(), w_beta.flatten() # (l1*w1,1) -> (l1*w1)
             # 墙壁反射单元的方向角和倾斜角,角度制转弧度制
-            w_alpha_rad , w_beta_rad = np.radians([w_alpha, w_beta])
+            w_alpha_rad, w_beta_rad = np.radians([w_alpha, w_beta]) # (l1*w1)
 
             # 墙壁反射单元法向量
             Nx = np.cos(w_alpha_rad) * np.sin(w_beta_rad)
             Ny = np.sin(w_alpha_rad) * np.sin(w_beta_rad)
             Nz = np.cos(w_beta_rad)
-            Nw = np.stack([Nx,Ny,Nz], axis=-1)  # 墙壁法向量 (l1,w1,3)
-            Nw = Nw/np.linalg.norm(Nw)  # 墙壁单位法向量 (l1,w1,3)
+            Nw = np.stack([Nx,Ny,Nz], axis=-1)  # 墙壁反射点法向量 (l1*w1,3)
+            Nw = Nw/np.linalg.norm(Nw)  # 墙壁反射点的单位法向量 (l1*w1,3)
 
             # LED -> 墙壁反射单元
             # 发射端
-            Vt_w = wall_pos - led_pos  # LED灯到墙壁反射单元的方向向量 (l1,w1,3)
-            d1 = np.linalg.norm(Vt_w, axis=-1) # 求模:LED灯到墙壁反射单元的距离 (l1,w1)
-
-            mark1 = np.all(Vt_w==0, axis=-1) # 异常点处理:判断墙壁反射单元和LED是否重合(方向向量是否为零向量) (l1,w1)
-            d1 = np.where(mark1, 1, d1)      # 异常点处理:为使cos_led_t_angle_rad分母不为0,让墙壁反射单元和LED重合时的距离不为0 (l1,w1)
-
-            cos_led_t_angle_rad = np.sum(Vt_w*led.Nv, axis=-1) / d1  # LED发射角的余弦值 (l1,w1)
+            Vt_w = wall_pos - led.pos  # LED灯到墙壁反射单元的方向向量 (l1*w1,3)
+            d1 = np.linalg.norm(Vt_w, axis=-1) # 求模:LED灯到墙壁反射单元的距离 (l1*w1)
+            mark1 = np.all(Vt_w==0, axis=-1) # 异常点处理:判断墙壁反射单元和LED是否重合(方向向量是否为零向量) (l1*w1)
+            d1 = np.where(mark1, 1, d1)      # 异常点处理:为使cos_led_t_angle_rad分母不为0,让墙壁反射单元和LED重合时的距离不为0 (l1*w1)
+            
+            cos_led_t_angle_rad = np.sum(Vt_w*led.Nv, axis=-1) / d1  # LED发射角的余弦值 (l1*w1)
 
             # 接收端
             Vw_t = -Vt_w  # 墙壁反射单元到LED灯的方向向量 (l1,w1,3)
-            cos_wall_r_angle_rad = np.sum(Vw_t*Nw, axis=-1) / d1 # 墙壁反射单元入射角 (l1,w1)
+            cos_wall_r_angle_rad = np.sum(Vw_t*Nw, axis=-1) / d1 # 墙壁反射单元入射角 (l1*w1)
 
             # 墙壁反射单元 -> PD
             # 发射端
-            Vw_r = pd_pos - wall_pos # 墙壁反射单元到PD的方向向量   (l,w,h,l1,w1,3)
-            d2 = np.linalg.norm(Vw_r, axis=-1) # 求模:墙壁反射单元到PD之间的距离 (l,w,h,l1,w1)
+            Vw_r = pd_pos - wall_pos # 墙壁反射单元到PD的方向向量  (l*w*h,1,3)-(l1*w1,3) (l*w*h,l1*w1,3)
+            d2 = np.linalg.norm(Vw_r, axis=-1) # 求模:墙壁反射单元到PD之间的距离 (l*w*h,l1*w1)
 
-            mark2 = np.all(Vw_r==0, axis=-1) # 异常点处理:判断墙壁反射单元和参考点是否重合(方向向量是否为零向量) (l,w,h,l1,w1)
+            mark2 = np.all(Vw_r==0, axis=-1) # 异常点处理:判断墙壁反射单元和参考点是否重合(方向向量是否为零向量) (l*w*h,l1*w1)
             d2 = np.where(mark2, 1, d2)      # 异常点处理:为使cos_wall_t_angle_rad分母不为0,让墙壁反射单元和参考点重合时的距离不为0
 
-            cos_wall_t_angle_rad = np.sum(Vw_r*Nw, axis=-1) / d2 # 墙壁反射单元发射角  (l,w,h,l1,w1)
-            cos_wall_t_angle_rad = np.where(cos_wall_t_angle_rad>0, cos_wall_t_angle_rad, 0) # 满足墙壁反射入射条件
-
+            cos_wall_t_angle_rad = np.sum(Vw_r*Nw, axis=-1) / d2 # 墙壁反射单元发射角  (l*w*h,l1*w1)
+            cos_wall_t_angle_rad = np.where(cos_wall_t_angle_rad>0, cos_wall_t_angle_rad, 0) # 满足墙壁反射入射条件 (l*w*h,l1*w1)
+      
             # 接收端
-            Vr_w = -Vw_r  # PD到墙壁反射单元的方向向量   (l,w,h,l1,w1,3)
-            cos_pd_r_angle_rad = np.sum(Vr_w*self.Nv, axis=-1) / d2 # PD接收角的余弦值   (l,w,h,l1,w1)
+            Vr_w = -Vw_r  # PD到墙壁反射单元的方向向量   (l*w*h,l1*w1,3)
+            cos_pd_r_angle_rad = np.sum(Vr_w*self.Nv, axis=-1) / d2 # PD接收角的余弦值   (l*w*h,l1*w1)
             cos_pd_r_angle_rad = np.where(cos_pd_r_angle_rad>0, cos_pd_r_angle_rad, 0) # 满足墙壁反射发射条件
 
             # PD入射角
-            pd_r_angle_rad = np.arccos(cos_pd_r_angle_rad) # PD接收器入射角(弧度制) (l,w,h,l1,w1)
-            pd_r_angle = np.degrees(pd_r_angle_rad) # 弧度制转为角度制 (l,w,h,l1,w1)
+            pd_r_angle_rad = np.arccos(cos_pd_r_angle_rad) # PD接收器入射角(弧度制) (l*w*h,l1*w1)
+            pd_r_angle = np.degrees(pd_r_angle_rad) # 弧度制转为角度制 (l*w*h,l1*w1)
 
             rho = room.rho[i]   #墙壁反射率
             Aw = room.Aw[i]     #墙壁反射单元面积
 
             # 反射(NLOS)子链路信道增益 (l,w,h,l1,w1)
             Hw = (((led.m + 1) * self.Ar) / (2 * np.pi**2 * d1**2 * d2**2)) * rho * Aw * cos_led_t_angle_rad**led.m * cos_wall_r_angle_rad * cos_wall_t_angle_rad *  cos_pd_r_angle_rad * self.Ts * self.G_Con  # 信道增益 
-            Hw = np.where((pd_r_angle>=0) & (pd_r_angle<=self.fov), Hw, 0)  # 视场内信道增益 (l,w,h,l1,w1)
+            Hw = np.where((pd_r_angle>=0) & (pd_r_angle<=self.fov), Hw, 0)  # 视场内信道增益 (l*w*h,l1*w1)
 
-            Hw = np.sum(np.sum(Hw, axis=-1), axis=-1)   # 反射(NLOS)链路信道增益 (l,w,h)
-            H0 += Hw  # 墙壁反射(NLOS)链路信道增益(l,w,h)
+            Hw = np.sum(Hw, axis=-1)   # 反射(NLOS)链路信道增益求和 (l*w*h)
+            H0 += Hw  # 墙壁反射(NLOS)链路信道增益(l*w*h)
         
-        H0 = np.expand_dims(H0,-1) # 在最后一维扩充一个维度 (l,w,h) -> (l,w,h,1)  <=> H0.reshape(l,w,h,1) <=> H0[...,np.newaxis]
-        recv_signal = H0 * led.signal # PD接收信号[广播机制 (l,w,h,1) * (npt) -> (l,w,h,npt) * (l,w,h,npt) = (l,w,h,npt)]
-        return np.squeeze(recv_signal)
+        H0 = np.expand_dims(H0,-1) # 在最后一维扩充一个维度 (l*w*h) -> (l*w*h,1)  <=> H0.reshape(l*w*h,1) <=> H0[...,np.newaxis]
+        recv_signal = H0 * led.signal # PD接收信号[广播机制 (l*w*h,1) * (npt) -> (l*w*h,npt) * (l*w*h,npt) = (l*w*h,npt)]
+        return np.squeeze(recv_signal) # 去除维度为1的维数
     
     def recv_led_signal(self, led:LED, room:Room):
         """计算PD接收LED信号(LOS+NLOS链路):
         Params
             led: LED实例化
             room: Room实例化
         Return 
@@ -324,26 +315,26 @@
         """获取原点位置
         """
         if not len(o) == 3:
             raise VLPSequenceLenError(o,3)
         self._origin = tuple(o) 
 
     @property
-    def pos(self) -> tuple:
+    def pos(self):
         """获取相对位置(参考位置相对与原点的相对位置)
         """
-        return tuple(i+j for i,j in zip(self._pos,self.origin))
+        return self._pos + self.origin
     
     @pos.setter
     def pos(self, pos:tuple):
         """设置参考位置
         """
-        if not len(pos) == 3:
-            raise VLPSequenceLenError(pos,3)
-        self._pos = tuple(pos)
+        if not np.shape(pos)[-1] == 3:
+            raise VLPSequenceLenError(np.shape(pos)[-1],3)
+        self._pos = np.asarray(pos)
 
     @property
     def Nv(self):  
         """获取PD单位法向量  
         """  
         # PD方位角和倾斜角,角度制转弧度制
         alpha_rad, beta_rad = np.radians([self.alpha, self.beta])
```

### Comparing `yang-vlp-0.2.14/vlppy/model/room.py` & `yang-vlp-0.2.15/vlppy/model/room.py`

 * *Files 6% similar despite different names*

```diff
@@ -44,73 +44,77 @@
         self.rho = rho #墙壁反射率
         
         self.rp_height = [0, height]   # 前后左右反射墙壁高度范围
 
         self.origin = (0,0,0) #原点位置
         self.wall_args_path = f"wall_args.xlsx" # 默认墙壁参数地址
 
-    def _get_reflect_wall_grid(self, gap, wall):
-        """得到反射墙壁反射面的网格矩阵
+    def _get_reflect_wall_pos(self, gap, wall):
+        """得到反射点坐标
         Params
             gap: 墙壁划分网格的间隔
             wall: 第几面墙(0=地板、1-4=前右后左、5=天花板)
         Return
-            (Xw, Yw, Zw): 墙壁面划分的网格矩阵
+            reflect_pos: 反射点坐标(列表元素个数等于反射单元的个数)
         """
         if wall not in (0,1,2,3,4,5):
             raise VLPValueError(wall,0,1,2,3,4,5)
         (xo, yo, zo) = self.origin # 原点
         gx, gy, gz = gap # 墙壁网格划分的间隔
 
+        # 不取靠近墙壁的点（符合实际环境）
         if wall in (0,5):    # 地板或天花板
             x = np.arange(gx, self.length-gx+1e-3, gx) 
             y = np.arange(gy, self.width-gy+1e-3, gy) 
-            z = 0 if wall == 0 else self.height
+            z = 0 if wall == 0 else self.height 
             Xw, Yw, Zw = np.meshgrid(xo+x, yo+y, zo+z, indexing='ij') # 地板和天花板平面建立二维网格矩阵 
         elif wall in (1,3): #前后墙  
             x = np.arange(gx, self.length-gx+1e-3, gx) 
             y = 0 if wall == 1 else self.width 
             z = np.arange(gz+self.rp_height[0], self.rp_height[1]-gz+1e-3, gz) 
             Xw, Yw, Zw = np.meshgrid(xo+x, yo+y, zo+z, indexing='ij') # 前后墙面建立二维网格矩阵 
         else:  #左右墙
             x = self.length if wall == 2 else 0
             y = np.arange(gy, self.width-gy+1e-3, gy) 
             z = np.arange(gz+self.rp_height[0], self.rp_height[1]-gz+1e-3, gz) 
             Xw, Yw, Zw = np.meshgrid(xo+x, yo+y, zo+z, indexing='ij') # 左右墙面建立二维网格矩阵  
-        Xw, Yw, Zw = np.squeeze(Xw), np.squeeze(Yw), np.squeeze(Zw) # 去除维数为1的维度
-        return (Xw, Yw, Zw)
+        Xw, Yw, Zw = Xw.flatten(), Yw.flatten(), Zw.flatten() # 打平
+        reflect_pos = np.stack([Xw, Yw, Zw], axis=-1)
+        return reflect_pos
 
-    def _get_reflect_wall_angle(self, grid_shape):
+    def _get_reflect_wall_angle(self, shape):
         """获取反射墙壁反射单元(法向量)的方位角和倾斜角
         Return 
-            alpha: 方位角(单位:度) (min,max) = (0°,360°)
-            beta: 倾斜角(单位:度)  (min,max) = (-90°,90°)
-        """
-        alpha = np.random.uniform(low=0, high=360, size=grid_shape)
-        beta = np.random.uniform(low=-90, high=90, size=grid_shape)
-        return alpha, beta
+            angles = [[alpha0,beta0],[alpha1,beta1],...] (列表元素个数等于反射单元的个数)
+                alpha: 方位角(单位:度) (min,max) = (0°,360°)
+                beta: 倾斜角(单位:度)  (min,max) = (-90°,90°)
+        """
+        print(f"{shape=}")
+        alpha = np.random.uniform(low=0, high=360, size=shape)
+        beta = np.random.uniform(low=-90, high=90, size=shape)
+        angles = np.stack([alpha, beta], axis=-1)
+        print(f"{alpha.shape=}")
+        print(f"{angles.shape=}")
+        return angles
 
-    def _save_reflect_wall_args(self, fp:str, reflect_pos:tuple, angle):
+    def _save_reflect_wall_args(self, fp:str, reflect_pos, angles):
         """保存反射墙壁参数(方位角和倾斜角)到excell
         Params 
             fp: 保存路径
             reflect_pos: 墙壁反射单元所在位置
-            angle: 获取墙壁反射单元的方位角和倾斜角(单位:度)
+            angle: 获取墙壁反射单元角度(方位角和倾斜角)(单位:度)
         """
-        if not len(reflect_pos) == 3:
+        if not np.shape(reflect_pos)[-1] == 3:
             raise VLPSequenceLenError(reflect_pos,3)
-        if not len(angle) == 2:
-            raise VLPSequenceLenError(angle,2)
-        xw, yw, zw = reflect_pos 
-        alpha, beta = angle
-        xw = np.array(xw).reshape(-1)
-        yw = np.array(yw).reshape(-1)
-        zw = np.array(zw).reshape(-1)
-        alpha = np.array(alpha).reshape(-1)
-        beta = np.array(beta).reshape(-1)
+        if not np.shape(angles)[-1] == 2:
+            raise VLPSequenceLenError(angles,2)
+        xw, yw, zw = np.split(reflect_pos, indices_or_sections=3, axis=-1)  # 分割操作
+        alpha, beta = np.split(angles, indices_or_sections=2, axis=-1) # 分割操作
+        xw, yw, zw = xw.flatten(), yw.flatten(), zw.flatten() # 打平
+        alpha, beta = alpha.flatten(), beta.flatten() # 打平
         wall_args = pd.DataFrame({
             "xw": xw,
             "yw": yw,
             "zw": zw,
             "alpha": alpha,
             "beta": beta
         })
@@ -119,80 +123,87 @@
         # np.savez(fp, alpha=alpha, beta=beta, xw=xw, yw=yw, zw=zw)
     
     def _load_reflect_wall_args(self, fp:str):
         """加载墙壁参数(方位角和倾斜角)到excell
         Params 
             fp: 文件路径
         Return
-            (xw, yw, zw), (alpha, beta): 反射墙壁网格矩阵和反射单元方向角和倾斜角(单位:度)
+            reflect_pos,angles 反射单元坐标和反射单元角度(方向角和倾斜角)(单位:度)
         """
         wall_args = pd.read_excel(fp).to_numpy()
-        xw,yw,zw,alpha,beta = np.split(wall_args,indices_or_sections=5,axis=-1)
+        xw, yw, zw, alpha, beta = np.split(wall_args,indices_or_sections=5,axis=-1)
         # 加载npz文件
         # with np.load(fp) as f:
         #     xw,yw,zw,alpha,beta = f['xw'],f['yw'],f['zw'],f['alpha'],f['beta']
-        return (xw, yw, zw), (alpha, beta)
+        # xw, yw, zw = xw.flatten(), yw.flatten(), zw.flatten() # 打平操作
+        # alpha, beta = alpha.flatten(), beta.flatten()
+        reflect_pos = np.stack([xw, yw, zw], axis=-1)
+        angles = np.stack([alpha, beta], axis=-1)
+        return reflect_pos, angles
 
     def set_regular_wall(self):
         """设置为规制墙壁 (更新墙壁参数)
         """
         # 如果前后左右墙反射单元距离地面最小高度不为0,则无需考虑地面反射
         if self.rp_height[0] > 0 and 0 in self.reflect_wall:
             self.reflect_wall.remove(0)
         # 如果前后左右墙反射单元与天花板最小距离不为0,则无需考虑天花板反射
         if self.rp_height[1] < self.height and 5 in self.reflect_wall:
             self.reflect_wall.remove(5)
 
         for wall in self.reflect_wall:
-            (Xw, Yw, Zw) = self._get_reflect_wall_grid(self.wall_gap, wall) #得到反射面的网格矩阵
-            grid_shape = Xw.shape # 获取矩阵形状
+            reflect_pos = self._get_reflect_wall_pos(self.wall_gap, wall) #得到反射点位置
+            xw, _, _ = np.split(reflect_pos,indices_or_sections=3,axis=-1)
+            shape = xw.flatten().shape # 打平后获取形状
             fpath = self.wall_args_path.format(wall) #默认路径
-            alpha, beta = np.zeros(shape=grid_shape), np.zeros(shape=grid_shape)#获取墙壁参数(倾斜角和方向角)
-            self._save_reflect_wall_args(fpath, (Xw, Yw, Zw), (alpha, beta)) #保存墙壁参数
+            alpha, beta = np.zeros(shape=shape), np.zeros(shape=shape)#获取墙壁参数(倾斜角和方向角)
+            angles = np.stack([alpha, beta], axis=-1)
+            self._save_reflect_wall_args(fpath, reflect_pos, angles) #保存墙壁参数
 
     def get_reflect_wall_args(self) -> list:
         """获取墙壁参数
         params
             无
         Return
-            [((Xw, Yw, Zw), (alpha, beta)),...]: 
-                    反射墙壁网格坐标矩阵和反射单元方向角和倾斜角(列表元素个数等于反射墙壁的个数)
+            [(reflect_pos, angles),...]: 
+                    反射墙壁网格坐标矩阵和反射单元角度(方向角和倾斜角) (列表元素个数等于反射墙壁的个数)
         """
         # 如果前后左右墙反射单元距离地面最小高度不为0,则无需考虑地面反射
         if self.rp_height[0] > 0 and 0 in self.reflect_wall:
             self.reflect_wall.remove(0)
             self.Aw.remove(self.reflect_wall.index(0))
         # 如果前后左右墙反射单元与天花板最小距离不为0,则无需考虑天花板反射
         if self.rp_height[1] < self.height and 5 in self.reflect_wall:
             self.reflect_wall.remove(5)
             self.Aw.remove(self.reflect_wall.index(5))
 
-        reflect_wall_args = []  # 反射墙壁网格坐标矩阵和反射单元方向角和倾斜角
+        reflect_wall_args = []  # 反射墙壁网格坐标和反射单元角度
         for wall in self.reflect_wall:
-            (Xw, Yw, Zw) = self._get_reflect_wall_grid(self.wall_gap, wall) #得到反射面的网格矩阵
-            grid_shape = Xw.shape # 获取矩阵形状
+            reflect_pos = self._get_reflect_wall_pos(self.wall_gap, wall) #得到反射点位置
+            pos_shape = np.shape(reflect_pos)
+
             fpath = self.wall_args_path.format(wall) #默认路径
-            # 检查路径是否存在
-            if os.path.exists(fpath):
-                try:
-                    _,(alpha, beta) = self._load_reflect_wall_args(fpath) #加载墙壁参数
-                    alpha, beta = alpha.reshape(grid_shape), beta.reshape(grid_shape) # excell读取的数据shape=（-1）->grid_shape
-                except:
-                    print("房间尺寸或墙壁划分间隔发生变化!") # 会导致reshape失败
-                    print(f"重新生成反射墙壁{wall}参数文件!")
-                    alpha, beta = self._get_reflect_wall_angle(grid_shape=grid_shape) #获取墙壁参数(倾斜角和方向角)
-                    self._save_reflect_wall_args(fpath, (Xw, Yw, Zw), (alpha, beta)) #保存墙壁参数
-                finally:
-                    print(f"反射墙壁{wall}参数文件加载成功!")
-            else:
+            angles = None
+            try:
+                _,angles = self._load_reflect_wall_args(fpath) #加载墙壁参数
+                assert pos_shape[0] == np.shape(angles)[0]  # 验证房间尺寸或墙壁划分间隔发生变化
+            except FileNotFoundError as e:
                 print(f"未发现反射墙壁{wall}参数文件!")
                 print(f"随机生成反射墙壁{wall}参数保存到文件!")
-                alpha, beta = self._get_reflect_wall_angle(grid_shape=grid_shape) #获取墙壁参数(倾斜角和方向角)
-                self._save_reflect_wall_args(fpath, (Xw, Yw, Zw), (alpha, beta)) #保存墙壁参数
-            reflect_wall_args.append(((Xw, Yw, Zw), (alpha, beta)))
+                angles = self._get_reflect_wall_angle(shape=pos_shape[0]) #获取墙壁参数(倾斜角和方向角)
+                self._save_reflect_wall_args(fpath, reflect_pos, angles) # 保存参数
+            except AssertionError as e:
+                print("房间尺寸或墙壁划分间隔发生变化!") # 会导致reshape失败
+                print(f"重新生成反射墙壁{wall}参数文件!")
+                angles = self._get_reflect_wall_angle(shape=pos_shape[0]) #获取墙壁参数(倾斜角和方向角)
+                self._save_reflect_wall_args(fpath, reflect_pos, angles) # 保存参数
+            else:
+                print(f"反射墙壁{wall}参数文件加载成功!")
+            finally:
+                reflect_wall_args.append((reflect_pos, angles))
         return reflect_wall_args
 
     @property
     def length(self):
         """获取房间长度
         """
         return self._length
@@ -295,27 +306,35 @@
         if not np.all((gap>0) & (gap<self.size)):
             raise VLPValueRangeError(gap, 0, self.size) # The gap setting is not reasonable!
         if gap.size == 1:
             gap = np.full(shape=(3), fill_value=gap) # 填充
         self._tp_gap = gap
 
     @property
-    def tp_grid_pos(self) -> tuple:
+    def tp_grid(self) -> tuple:
         """获取测试点位置的网格矩阵(所有测试点的相对位置)
         """
         (xo, yo, zo) = self._origin #原点位置
 
         gx, gy, gz = self.tp_gap # 测试区域划分网格的间隔
         tp_h1, tp_h2 = self.tp_height # 测试区域高度
         x = np.arange(0, self.length+1e-3, gx) # 房间长度等间隔划分的数组
         y = np.arange(0, self.width+1e-3, gy)  # 房间宽度等间隔划分的数组
         z = np.arange(tp_h1, tp_h2+1e-3, gz)   # 测试平面高度等间隔划分的数组
         xr, yr, zr = np.meshgrid(xo+x, yo+y, zo+z, indexing='ij') # 返回二维网格矩阵（测试点的相对位置）
-        return (np.squeeze(xr), np.squeeze(yr), np.squeeze(zr))  # 去除维数为1的维度
-    
+        return xr.squeeze(), yr.squeeze(), zr.squeeze() 
+
+    @property
+    def tp_pos(self) -> tuple:
+        """获取测试点位置
+        """
+        xr, yr, zr = self.tp_grid
+        pos = np.stack([xr,yr,zr], axis=-1)
+        return pos
+
     @property
     def wall_gap(self):
         """获取墙壁划分网格的间隔 
         """
         return self._wall_gap
     
     @wall_gap.setter
```

### Comparing `yang-vlp-0.2.14/vlppy/setting/__pycache__/json_setting.cpython-39.pyc` & `yang-vlp-0.2.15/vlppy/setting/__pycache__/json_setting.cpython-39.pyc`

 * *Files identical despite different names*

### Comparing `yang-vlp-0.2.14/vlppy/setting/json_setting.py` & `yang-vlp-0.2.15/vlppy/setting/json_setting.py`

 * *Files identical despite different names*

### Comparing `yang-vlp-0.2.14/vlppy/setting/settings.json` & `yang-vlp-0.2.15/vlppy/setting/settings.json`

 * *Files identical despite different names*

### Comparing `yang-vlp-0.2.14/vlppy/signal/filter.py` & `yang-vlp-0.2.15/vlppy/signal/filter.py`

 * *Files identical despite different names*

### Comparing `yang-vlp-0.2.14/vlppy/signal/plot.py` & `yang-vlp-0.2.15/vlppy/signal/plot.py`

 * *Files identical despite different names*

### Comparing `yang-vlp-0.2.14/vlppy/vis/vis.py` & `yang-vlp-0.2.15/vlppy/vis/vis.py`

 * *Files identical despite different names*

### Comparing `yang-vlp-0.2.14/yang_vlp.egg-info/PKG-INFO` & `yang-vlp-0.2.15/yang_vlp.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: yang-vlp
-Version: 0.2.14
+Version: 0.2.15
 Summary: Construction of visible light positioning model
 Home-page: https://gitee.com/yangwuju/yang_vlp
 Author: yangwuju
 Author-email: yangwuju <1424134319@qq.com>
 License: Copyright (c) 2018 The Python Packaging Authority
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `yang-vlp-0.2.14/yang_vlp.egg-info/SOURCES.txt` & `yang-vlp-0.2.15/yang_vlp.egg-info/SOURCES.txt`

 * *Files identical despite different names*

