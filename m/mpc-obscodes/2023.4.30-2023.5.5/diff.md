# Comparing `tmp/mpc_obscodes-2023.4.30.tar.gz` & `tmp/mpc_obscodes-2023.5.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mpc_obscodes-2023.4.30.tar", last modified: Sun Apr 30 18:02:28 2023, max compression
+gzip compressed data, was "mpc_obscodes-2023.5.5.tar", last modified: Fri May  5 02:26:46 2023, max compression
```

## Comparing `mpc_obscodes-2023.4.30.tar` & `mpc_obscodes-2023.5.5.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 18:02:28.016862 mpc_obscodes-2023.4.30/
--rw-r--r--   0 runner    (1001) docker     (123)       86 2023-04-30 18:02:05.000000 mpc_obscodes-2023.4.30/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2405 2023-04-30 18:02:28.016862 mpc_obscodes-2023.4.30/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2148 2023-04-30 18:02:05.000000 mpc_obscodes-2023.4.30/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 18:02:28.012863 mpc_obscodes-2023.4.30/mpc_obscodes/
--rw-r--r--   0 runner    (1001) docker     (123)      187 2023-04-30 18:02:05.000000 mpc_obscodes-2023.4.30/mpc_obscodes/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1329 2023-04-30 18:02:05.000000 mpc_obscodes-2023.4.30/mpc_obscodes/compare.py
--rw-r--r--   0 runner    (1001) docker     (123)     3446 2023-04-30 18:02:05.000000 mpc_obscodes-2023.4.30/mpc_obscodes/fetch.py
--rw-r--r--   0 runner    (1001) docker     (123)   245280 2023-04-30 18:02:12.000000 mpc_obscodes-2023.4.30/mpc_obscodes/obscodes_extended.json
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-04-30 18:02:12.000000 mpc_obscodes-2023.4.30/mpc_obscodes/obscodes_extended.md5
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 18:02:28.016862 mpc_obscodes-2023.4.30/mpc_obscodes/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-30 18:02:05.000000 mpc_obscodes-2023.4.30/mpc_obscodes/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1164 2023-04-30 18:02:05.000000 mpc_obscodes-2023.4.30/mpc_obscodes/tests/test_compare.py
--rw-r--r--   0 runner    (1001) docker     (123)      649 2023-04-30 18:02:05.000000 mpc_obscodes-2023.4.30/mpc_obscodes/tests/test_fetch.py
--rw-r--r--   0 runner    (1001) docker     (123)      653 2023-04-30 18:02:05.000000 mpc_obscodes-2023.4.30/mpc_obscodes/tests/test_mpc_obscodes.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 18:02:28.012863 mpc_obscodes-2023.4.30/mpc_obscodes.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2405 2023-04-30 18:02:28.000000 mpc_obscodes-2023.4.30/mpc_obscodes.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      496 2023-04-30 18:02:28.000000 mpc_obscodes-2023.4.30/mpc_obscodes.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-30 18:02:28.000000 mpc_obscodes-2023.4.30/mpc_obscodes.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-04-30 18:02:28.000000 mpc_obscodes-2023.4.30/mpc_obscodes.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-04-30 18:02:28.000000 mpc_obscodes-2023.4.30/mpc_obscodes.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      571 2023-04-30 18:02:12.000000 mpc_obscodes-2023.4.30/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-30 18:02:28.016862 mpc_obscodes-2023.4.30/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 02:26:46.726957 mpc_obscodes-2023.5.5/
+-rw-r--r--   0 runner    (1001) docker     (123)       86 2023-05-05 02:26:32.000000 mpc_obscodes-2023.5.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2404 2023-05-05 02:26:46.726957 mpc_obscodes-2023.5.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2148 2023-05-05 02:26:32.000000 mpc_obscodes-2023.5.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 02:26:46.726957 mpc_obscodes-2023.5.5/mpc_obscodes/
+-rw-r--r--   0 runner    (1001) docker     (123)      187 2023-05-05 02:26:32.000000 mpc_obscodes-2023.5.5/mpc_obscodes/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1329 2023-05-05 02:26:32.000000 mpc_obscodes-2023.5.5/mpc_obscodes/compare.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3446 2023-05-05 02:26:32.000000 mpc_obscodes-2023.5.5/mpc_obscodes/fetch.py
+-rw-r--r--   0 runner    (1001) docker     (123)   245386 2023-05-05 02:26:35.000000 mpc_obscodes-2023.5.5/mpc_obscodes/obscodes_extended.json
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-05-05 02:26:35.000000 mpc_obscodes-2023.5.5/mpc_obscodes/obscodes_extended.md5
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 02:26:46.726957 mpc_obscodes-2023.5.5/mpc_obscodes/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 02:26:32.000000 mpc_obscodes-2023.5.5/mpc_obscodes/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1164 2023-05-05 02:26:32.000000 mpc_obscodes-2023.5.5/mpc_obscodes/tests/test_compare.py
+-rw-r--r--   0 runner    (1001) docker     (123)      649 2023-05-05 02:26:32.000000 mpc_obscodes-2023.5.5/mpc_obscodes/tests/test_fetch.py
+-rw-r--r--   0 runner    (1001) docker     (123)      653 2023-05-05 02:26:32.000000 mpc_obscodes-2023.5.5/mpc_obscodes/tests/test_mpc_obscodes.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 02:26:46.726957 mpc_obscodes-2023.5.5/mpc_obscodes.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2404 2023-05-05 02:26:46.000000 mpc_obscodes-2023.5.5/mpc_obscodes.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      496 2023-05-05 02:26:46.000000 mpc_obscodes-2023.5.5/mpc_obscodes.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 02:26:46.000000 mpc_obscodes-2023.5.5/mpc_obscodes.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-05 02:26:46.000000 mpc_obscodes-2023.5.5/mpc_obscodes.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-05 02:26:46.000000 mpc_obscodes-2023.5.5/mpc_obscodes.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      571 2023-05-05 02:26:35.000000 mpc_obscodes-2023.5.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-05 02:26:46.726957 mpc_obscodes-2023.5.5/setup.cfg
```

### Comparing `mpc_obscodes-2023.4.30/PKG-INFO` & `mpc_obscodes-2023.5.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mpc_obscodes
-Version: 2023.4.30
+Version: 2023.5.5
 Summary: Minor Planet Center Observatory Codes
 Author-email: B612 Asteroid Institute <info@b612foundation.org>
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: tests
 
 # mpc_obscodes: Minor Planet Center Observatory Codes File
```

### Comparing `mpc_obscodes-2023.4.30/README.md` & `mpc_obscodes-2023.5.5/README.md`

 * *Files identical despite different names*

### Comparing `mpc_obscodes-2023.4.30/mpc_obscodes/compare.py` & `mpc_obscodes-2023.5.5/mpc_obscodes/compare.py`

 * *Files identical despite different names*

### Comparing `mpc_obscodes-2023.4.30/mpc_obscodes/fetch.py` & `mpc_obscodes-2023.5.5/mpc_obscodes/fetch.py`

 * *Files identical despite different names*

### Comparing `mpc_obscodes-2023.4.30/mpc_obscodes/obscodes_extended.json` & `mpc_obscodes-2023.5.5/mpc_obscodes/obscodes_extended.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9995886466474702%*

 * *Differences: {"'M54'": "OrderedDict([('Longitude', 7.07781), ('cos', 0.72514), ('sin', 0.686335), ('Name', "*

 * *          "'Observatoire Albireo de Biot')])"}*

```diff
@@ -12079,14 +12079,20 @@
     },
     "M53": {
         "Longitude": 10.28219,
         "Name": "CAS Observatory, Preetz",
         "cos": 0.585977,
         "sin": 0.807623
     },
+    "M54": {
+        "Longitude": 7.07781,
+        "Name": "Observatoire Albireo de Biot",
+        "cos": 0.72514,
+        "sin": 0.686335
+    },
     "M90": {
         "Longitude": 65.4286,
         "Name": "Chervishevo",
         "cos": 0.54672,
         "sin": 0.83452
     },
     "N27": {
```

### Comparing `mpc_obscodes-2023.4.30/mpc_obscodes/tests/test_compare.py` & `mpc_obscodes-2023.5.5/mpc_obscodes/tests/test_compare.py`

 * *Files identical despite different names*

### Comparing `mpc_obscodes-2023.4.30/mpc_obscodes/tests/test_fetch.py` & `mpc_obscodes-2023.5.5/mpc_obscodes/tests/test_fetch.py`

 * *Files identical despite different names*

### Comparing `mpc_obscodes-2023.4.30/mpc_obscodes/tests/test_mpc_obscodes.py` & `mpc_obscodes-2023.5.5/mpc_obscodes/tests/test_mpc_obscodes.py`

 * *Files identical despite different names*

### Comparing `mpc_obscodes-2023.4.30/mpc_obscodes.egg-info/PKG-INFO` & `mpc_obscodes-2023.5.5/mpc_obscodes.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mpc-obscodes
-Version: 2023.4.30
+Version: 2023.5.5
 Summary: Minor Planet Center Observatory Codes
 Author-email: B612 Asteroid Institute <info@b612foundation.org>
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: tests
 
 # mpc_obscodes: Minor Planet Center Observatory Codes File
```

### Comparing `mpc_obscodes-2023.4.30/pyproject.toml` & `mpc_obscodes-2023.5.5/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires =  ["setuptools>=45", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "mpc_obscodes"
-version = "2023.04.30"
+version = "2023.05.05"
 authors = [
     {name = "B612 Asteroid Institute", email = "info@b612foundation.org"},
 ]
 description = "Minor Planet Center Observatory Codes"
 readme = "README.md"
 requires-python = ">=3.7"
```

