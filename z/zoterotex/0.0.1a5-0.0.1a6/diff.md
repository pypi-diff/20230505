# Comparing `tmp/zoterotex-0.0.1a5.tar.gz` & `tmp/zoterotex-0.0.1a6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zoterotex-0.0.1a5.tar", last modified: Fri May  5 00:09:40 2023, max compression
+gzip compressed data, was "zoterotex-0.0.1a6.tar", last modified: Fri May  5 00:16:16 2023, max compression
```

## Comparing `zoterotex-0.0.1a5.tar` & `zoterotex-0.0.1a6.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 galer    (1959091754) 1971611142        0 2023-05-05 00:09:40.285493 zoterotex-0.0.1a5/
--rw-r--r--   0 galer    (1959091754) 1971611142      193 2023-05-05 00:09:40.285267 zoterotex-0.0.1a5/PKG-INFO
--rw-r--r--   0 galer    (1959091754) 1971611142      408 2023-05-05 00:09:32.000000 zoterotex-0.0.1a5/pyproject.toml
--rw-r--r--   0 galer    (1959091754) 1971611142       38 2023-05-05 00:09:40.285540 zoterotex-0.0.1a5/setup.cfg
-drwxr-xr-x   0 galer    (1959091754) 1971611142        0 2023-05-05 00:09:40.282780 zoterotex-0.0.1a5/zoterotex/
--rw-r--r--   0 galer    (1959091754) 1971611142        0 2023-05-04 21:34:59.000000 zoterotex-0.0.1a5/zoterotex/__init__.py
--rw-r--r--   0 galer    (1959091754) 1971611142     2190 2023-05-05 00:09:04.000000 zoterotex-0.0.1a5/zoterotex/__main__.py
-drwxr-xr-x   0 galer    (1959091754) 1971611142        0 2023-05-05 00:09:40.284956 zoterotex-0.0.1a5/zoterotex.egg-info/
--rw-r--r--   0 galer    (1959091754) 1971611142      193 2023-05-05 00:09:40.000000 zoterotex-0.0.1a5/zoterotex.egg-info/PKG-INFO
--rw-r--r--   0 galer    (1959091754) 1971611142      258 2023-05-05 00:09:40.000000 zoterotex-0.0.1a5/zoterotex.egg-info/SOURCES.txt
--rw-r--r--   0 galer    (1959091754) 1971611142        1 2023-05-05 00:09:40.000000 zoterotex-0.0.1a5/zoterotex.egg-info/dependency_links.txt
--rw-r--r--   0 galer    (1959091754) 1971611142       54 2023-05-05 00:09:40.000000 zoterotex-0.0.1a5/zoterotex.egg-info/entry_points.txt
--rw-r--r--   0 galer    (1959091754) 1971611142       32 2023-05-05 00:09:40.000000 zoterotex-0.0.1a5/zoterotex.egg-info/requires.txt
--rw-r--r--   0 galer    (1959091754) 1971611142       10 2023-05-05 00:09:40.000000 zoterotex-0.0.1a5/zoterotex.egg-info/top_level.txt
+drwxr-xr-x   0 galer    (1959091754) 1971611142        0 2023-05-05 00:16:16.499682 zoterotex-0.0.1a6/
+-rw-r--r--   0 galer    (1959091754) 1971611142      193 2023-05-05 00:16:16.499450 zoterotex-0.0.1a6/PKG-INFO
+-rw-r--r--   0 galer    (1959091754) 1971611142      408 2023-05-05 00:15:55.000000 zoterotex-0.0.1a6/pyproject.toml
+-rw-r--r--   0 galer    (1959091754) 1971611142       38 2023-05-05 00:16:16.499730 zoterotex-0.0.1a6/setup.cfg
+drwxr-xr-x   0 galer    (1959091754) 1971611142        0 2023-05-05 00:16:16.497160 zoterotex-0.0.1a6/zoterotex/
+-rw-r--r--   0 galer    (1959091754) 1971611142        0 2023-05-04 21:34:59.000000 zoterotex-0.0.1a6/zoterotex/__init__.py
+-rw-r--r--   0 galer    (1959091754) 1971611142     2190 2023-05-05 00:09:04.000000 zoterotex-0.0.1a6/zoterotex/__main__.py
+drwxr-xr-x   0 galer    (1959091754) 1971611142        0 2023-05-05 00:16:16.499158 zoterotex-0.0.1a6/zoterotex.egg-info/
+-rw-r--r--   0 galer    (1959091754) 1971611142      193 2023-05-05 00:16:16.000000 zoterotex-0.0.1a6/zoterotex.egg-info/PKG-INFO
+-rw-r--r--   0 galer    (1959091754) 1971611142      258 2023-05-05 00:16:16.000000 zoterotex-0.0.1a6/zoterotex.egg-info/SOURCES.txt
+-rw-r--r--   0 galer    (1959091754) 1971611142        1 2023-05-05 00:16:16.000000 zoterotex-0.0.1a6/zoterotex.egg-info/dependency_links.txt
+-rw-r--r--   0 galer    (1959091754) 1971611142       54 2023-05-05 00:16:16.000000 zoterotex-0.0.1a6/zoterotex.egg-info/entry_points.txt
+-rw-r--r--   0 galer    (1959091754) 1971611142       32 2023-05-05 00:16:16.000000 zoterotex-0.0.1a6/zoterotex.egg-info/requires.txt
+-rw-r--r--   0 galer    (1959091754) 1971611142       10 2023-05-05 00:16:16.000000 zoterotex-0.0.1a6/zoterotex.egg-info/top_level.txt
```

### Comparing `zoterotex-0.0.1a5/zoterotex/__main__.py` & `zoterotex-0.0.1a6/zoterotex/__main__.py`

 * *Files identical despite different names*

