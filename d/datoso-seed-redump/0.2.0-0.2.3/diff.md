# Comparing `tmp/datoso_seed_redump-0.2.0.tar.gz` & `tmp/datoso_seed_redump-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "datoso_seed_redump-0.2.0.tar", last modified: Sun Apr 30 18:19:33 2023, max compression
+gzip compressed data, was "datoso_seed_redump-0.2.3.tar", last modified: Fri May  5 04:16:44 2023, max compression
```

## Comparing `datoso_seed_redump-0.2.0.tar` & `datoso_seed_redump-0.2.3.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 18:19:33.435958 datoso_seed_redump-0.2.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-04-30 18:19:18.000000 datoso_seed_redump-0.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1856 2023-04-30 18:19:33.435958 datoso_seed_redump-0.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1168 2023-04-30 18:19:18.000000 datoso_seed_redump-0.2.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1110 2023-04-30 18:19:18.000000 datoso_seed_redump-0.2.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      180 2023-04-30 18:19:33.435958 datoso_seed_redump-0.2.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 18:19:33.431958 datoso_seed_redump-0.2.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 18:19:33.431958 datoso_seed_redump-0.2.0/src/datoso_seed_redump/
--rw-r--r--   0 runner    (1001) docker     (123)      366 2023-04-30 18:19:18.000000 datoso_seed_redump-0.2.0/src/datoso_seed_redump/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1006 2023-04-30 18:19:18.000000 datoso_seed_redump-0.2.0/src/datoso_seed_redump/actions.py
--rw-r--r--   0 runner    (1001) docker     (123)     3192 2023-04-30 18:19:18.000000 datoso_seed_redump-0.2.0/src/datoso_seed_redump/dats.py
--rw-r--r--   0 runner    (1001) docker     (123)     2876 2023-04-30 18:19:18.000000 datoso_seed_redump-0.2.0/src/datoso_seed_redump/fetch.py
--rw-r--r--   0 runner    (1001) docker     (123)     1197 2023-04-30 18:19:18.000000 datoso_seed_redump-0.2.0/src/datoso_seed_redump/rules.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 18:19:33.435958 datoso_seed_redump-0.2.0/src/datoso_seed_redump.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1856 2023-04-30 18:19:33.000000 datoso_seed_redump-0.2.0/src/datoso_seed_redump.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      435 2023-04-30 18:19:33.000000 datoso_seed_redump-0.2.0/src/datoso_seed_redump.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-30 18:19:33.000000 datoso_seed_redump-0.2.0/src/datoso_seed_redump.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-04-30 18:19:33.000000 datoso_seed_redump-0.2.0/src/datoso_seed_redump.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-04-30 18:19:33.000000 datoso_seed_redump-0.2.0/src/datoso_seed_redump.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 04:16:44.893979 datoso_seed_redump-0.2.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-05-05 04:16:21.000000 datoso_seed_redump-0.2.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1836 2023-05-05 04:16:44.893979 datoso_seed_redump-0.2.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1168 2023-05-05 04:16:21.000000 datoso_seed_redump-0.2.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1040 2023-05-05 04:16:21.000000 datoso_seed_redump-0.2.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      180 2023-05-05 04:16:44.897979 datoso_seed_redump-0.2.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 04:16:44.889979 datoso_seed_redump-0.2.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 04:16:44.893979 datoso_seed_redump-0.2.3/src/datoso_seed_redump/
+-rw-r--r--   0 runner    (1001) docker     (123)      366 2023-05-05 04:16:21.000000 datoso_seed_redump-0.2.3/src/datoso_seed_redump/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1006 2023-05-05 04:16:21.000000 datoso_seed_redump-0.2.3/src/datoso_seed_redump/actions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3192 2023-05-05 04:16:21.000000 datoso_seed_redump-0.2.3/src/datoso_seed_redump/dats.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2876 2023-05-05 04:16:21.000000 datoso_seed_redump-0.2.3/src/datoso_seed_redump/fetch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1197 2023-05-05 04:16:21.000000 datoso_seed_redump-0.2.3/src/datoso_seed_redump/rules.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 04:16:44.893979 datoso_seed_redump-0.2.3/src/datoso_seed_redump.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1836 2023-05-05 04:16:44.000000 datoso_seed_redump-0.2.3/src/datoso_seed_redump.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      435 2023-05-05 04:16:44.000000 datoso_seed_redump-0.2.3/src/datoso_seed_redump.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 04:16:44.000000 datoso_seed_redump-0.2.3/src/datoso_seed_redump.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-05 04:16:44.000000 datoso_seed_redump-0.2.3/src/datoso_seed_redump.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-05-05 04:16:44.000000 datoso_seed_redump-0.2.3/src/datoso_seed_redump.egg-info/top_level.txt
```

### Comparing `datoso_seed_redump-0.2.0/LICENSE` & `datoso_seed_redump-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `datoso_seed_redump-0.2.0/PKG-INFO` & `datoso_seed_redump-0.2.3/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,24 +1,23 @@
 Metadata-Version: 2.1
 Name: datoso_seed_redump
-Version: 0.2.0
+Version: 0.2.3
 Summary: Python command line tool to download and organize your Rom Dat files.
 Author-email: Lacides Miranda <laromicas@hotmail.com>
 License: MIT License
 Project-URL: Source Code, https://github.com/laromicas/datoso_seed_redump
 Keywords: emulators,roms
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: System :: Emulators
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
-Provides-Extra: dev
 License-File: LICENSE
 
 ![Datoso](https://github.com/laromicas/datoso/blob/master/bearlogo.png)
 
 # Datoso Seed Redump
 
 Datoso is a WIP Python command line tool to download and organize your Dat Roms.
```

### Comparing `datoso_seed_redump-0.2.0/README.md` & `datoso_seed_redump-0.2.3/README.md`

 * *Files identical despite different names*

### Comparing `datoso_seed_redump-0.2.0/pyproject.toml` & `datoso_seed_redump-0.2.3/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -18,25 +18,18 @@
     "Environment :: Console",
     'License :: OSI Approved :: MIT License',
     "Operating System :: POSIX :: Linux",
     'Programming Language :: Python :: 3',
     'Topic :: System :: Emulators',
 ]
 dependencies = [
-    "datoso>=0.2.0",
+    "datoso>=0.2.3",
 ]
 dynamic = ["version"]
 
-
-[project.optional-dependencies]
-
-dev = [
-    "ruff>=0.0.261",
-    ]
-
 [project.urls]
 "Source Code"       = "https://github.com/laromicas/datoso_seed_redump"
 
 [tool.setuptools]
 packages = ["datoso_seed_redump"]
 license-files = ["LICENSE"]
 include-package-data = true
```

### Comparing `datoso_seed_redump-0.2.0/src/datoso_seed_redump/actions.py` & `datoso_seed_redump-0.2.3/src/datoso_seed_redump/actions.py`

 * *Files identical despite different names*

### Comparing `datoso_seed_redump-0.2.0/src/datoso_seed_redump/dats.py` & `datoso_seed_redump-0.2.3/src/datoso_seed_redump/dats.py`

 * *Files identical despite different names*

### Comparing `datoso_seed_redump-0.2.0/src/datoso_seed_redump/fetch.py` & `datoso_seed_redump-0.2.3/src/datoso_seed_redump/fetch.py`

 * *Files identical despite different names*

### Comparing `datoso_seed_redump-0.2.0/src/datoso_seed_redump/rules.py` & `datoso_seed_redump-0.2.3/src/datoso_seed_redump/rules.py`

 * *Files identical despite different names*

### Comparing `datoso_seed_redump-0.2.0/src/datoso_seed_redump.egg-info/PKG-INFO` & `datoso_seed_redump-0.2.3/src/datoso_seed_redump.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,24 +1,23 @@
 Metadata-Version: 2.1
 Name: datoso-seed-redump
-Version: 0.2.0
+Version: 0.2.3
 Summary: Python command line tool to download and organize your Rom Dat files.
 Author-email: Lacides Miranda <laromicas@hotmail.com>
 License: MIT License
 Project-URL: Source Code, https://github.com/laromicas/datoso_seed_redump
 Keywords: emulators,roms
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: System :: Emulators
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
-Provides-Extra: dev
 License-File: LICENSE
 
 ![Datoso](https://github.com/laromicas/datoso/blob/master/bearlogo.png)
 
 # Datoso Seed Redump
 
 Datoso is a WIP Python command line tool to download and organize your Dat Roms.
```

