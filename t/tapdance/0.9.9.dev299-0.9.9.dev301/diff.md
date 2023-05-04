# Comparing `tmp/tapdance-0.9.9.dev299.tar.gz` & `tmp/tapdance-0.9.9.dev301.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tapdance-0.9.9.dev299.tar", max compression
+gzip compressed data, was "tapdance-0.9.9.dev301.tar", max compression
```

## Comparing `tapdance-0.9.9.dev299.tar` & `tapdance-0.9.9.dev301.tar`

### file list

```diff
@@ -1,11 +1,11 @@
--rw-r--r--   0        0        0     1069 2023-04-05 17:47:07.778496 tapdance-0.9.9.dev299/LICENSE
--rw-r--r--   0        0        0     1040 2023-04-05 17:47:24.506782 tapdance-0.9.9.dev299/pyproject.toml
--rw-r--r--   0        0        0      288 2023-04-05 17:47:07.782496 tapdance-0.9.9.dev299/tapdance/__init__.py
--rw-r--r--   0        0        0      696 2023-04-05 17:47:07.782496 tapdance-0.9.9.dev299/tapdance/cli.py
--rw-r--r--   0        0        0    14857 2023-04-05 17:47:07.782496 tapdance-0.9.9.dev299/tapdance/config.py
--rw-r--r--   0        0        0    13532 2023-04-05 17:47:07.782496 tapdance-0.9.9.dev299/tapdance/docker.py
--rw-r--r--   0        0        0     1606 2023-04-05 17:47:07.782496 tapdance-0.9.9.dev299/tapdance/install_helper.py
--rw-r--r--   0        0        0    37111 2023-04-05 17:47:07.782496 tapdance-0.9.9.dev299/tapdance/plans.py
--rw-r--r--   0        0        0     2432 2023-04-05 17:47:07.782496 tapdance-0.9.9.dev299/tapdance/states.py
--rw-r--r--   0        0        0    10919 2023-04-05 17:47:07.782496 tapdance-0.9.9.dev299/tapdance/syncs.py
--rw-r--r--   0        0        0     1209 1970-01-01 00:00:00.000000 tapdance-0.9.9.dev299/PKG-INFO
+-rw-r--r--   0        0        0     1069 2023-05-04 18:59:29.349139 tapdance-0.9.9.dev301/LICENSE
+-rw-r--r--   0        0        0     1040 2023-05-04 18:59:51.857309 tapdance-0.9.9.dev301/pyproject.toml
+-rw-r--r--   0        0        0      288 2023-05-04 18:59:29.353139 tapdance-0.9.9.dev301/tapdance/__init__.py
+-rw-r--r--   0        0        0      696 2023-05-04 18:59:29.353139 tapdance-0.9.9.dev301/tapdance/cli.py
+-rw-r--r--   0        0        0    14857 2023-05-04 18:59:29.353139 tapdance-0.9.9.dev301/tapdance/config.py
+-rw-r--r--   0        0        0    13532 2023-05-04 18:59:29.353139 tapdance-0.9.9.dev301/tapdance/docker.py
+-rw-r--r--   0        0        0     1606 2023-05-04 18:59:29.353139 tapdance-0.9.9.dev301/tapdance/install_helper.py
+-rw-r--r--   0        0        0    37111 2023-05-04 18:59:29.353139 tapdance-0.9.9.dev301/tapdance/plans.py
+-rw-r--r--   0        0        0     2432 2023-05-04 18:59:29.353139 tapdance-0.9.9.dev301/tapdance/states.py
+-rw-r--r--   0        0        0    10919 2023-05-04 18:59:29.353139 tapdance-0.9.9.dev301/tapdance/syncs.py
+-rw-r--r--   0        0        0     1209 1970-01-01 00:00:00.000000 tapdance-0.9.9.dev301/PKG-INFO
```

### Comparing `tapdance-0.9.9.dev299/LICENSE` & `tapdance-0.9.9.dev301/LICENSE`

 * *Files identical despite different names*

### Comparing `tapdance-0.9.9.dev299/pyproject.toml` & `tapdance-0.9.9.dev301/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "tapdance"
-version = "0.9.9-dev.299"
+version = "0.9.9-dev.301"
 description = "Tapdance is an orchestration layer for the open source Singer tap platform."
 authors = ["AJ Steers <aj.steers@slalom.com>"]
 license = "MIT"
 
 [tool.poetry.dependencies]
 python = "^3.7"
 docker = "^4.4.1"
```

### Comparing `tapdance-0.9.9.dev299/tapdance/cli.py` & `tapdance-0.9.9.dev301/tapdance/cli.py`

 * *Files identical despite different names*

### Comparing `tapdance-0.9.9.dev299/tapdance/config.py` & `tapdance-0.9.9.dev301/tapdance/config.py`

 * *Files identical despite different names*

### Comparing `tapdance-0.9.9.dev299/tapdance/docker.py` & `tapdance-0.9.9.dev301/tapdance/docker.py`

 * *Files identical despite different names*

### Comparing `tapdance-0.9.9.dev299/tapdance/install_helper.py` & `tapdance-0.9.9.dev301/tapdance/install_helper.py`

 * *Files identical despite different names*

### Comparing `tapdance-0.9.9.dev299/tapdance/plans.py` & `tapdance-0.9.9.dev301/tapdance/plans.py`

 * *Files identical despite different names*

### Comparing `tapdance-0.9.9.dev299/tapdance/states.py` & `tapdance-0.9.9.dev301/tapdance/states.py`

 * *Files identical despite different names*

### Comparing `tapdance-0.9.9.dev299/tapdance/syncs.py` & `tapdance-0.9.9.dev301/tapdance/syncs.py`

 * *Files identical despite different names*

### Comparing `tapdance-0.9.9.dev299/PKG-INFO` & `tapdance-0.9.9.dev301/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tapdance
-Version: 0.9.9.dev299
+Version: 0.9.9.dev301
 Summary: Tapdance is an orchestration layer for the open source Singer tap platform.
 License: MIT
 Author: AJ Steers
 Author-email: aj.steers@slalom.com
 Requires-Python: >=3.7,<4.0
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
```

