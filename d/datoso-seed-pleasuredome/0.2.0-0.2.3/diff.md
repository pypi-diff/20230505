# Comparing `tmp/datoso_seed_pleasuredome-0.2.0.tar.gz` & `tmp/datoso_seed_pleasuredome-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "datoso_seed_pleasuredome-0.2.0.tar", last modified: Sun Apr 30 18:01:40 2023, max compression
+gzip compressed data, was "datoso_seed_pleasuredome-0.2.3.tar", last modified: Fri May  5 04:16:01 2023, max compression
```

## Comparing `datoso_seed_pleasuredome-0.2.0.tar` & `datoso_seed_pleasuredome-0.2.3.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 18:01:40.262170 datoso_seed_pleasuredome-0.2.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-04-30 18:01:28.000000 datoso_seed_pleasuredome-0.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1767 2023-04-30 18:01:40.262170 datoso_seed_pleasuredome-0.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-04-30 18:01:28.000000 datoso_seed_pleasuredome-0.2.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1191 2023-04-30 18:01:28.000000 datoso_seed_pleasuredome-0.2.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      180 2023-04-30 18:01:40.262170 datoso_seed_pleasuredome-0.2.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 18:01:40.258170 datoso_seed_pleasuredome-0.2.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 18:01:40.258170 datoso_seed_pleasuredome-0.2.0/src/datoso_seed_pleasuredome/
--rw-r--r--   0 runner    (1001) docker     (123)      259 2023-04-30 18:01:28.000000 datoso_seed_pleasuredome-0.2.0/src/datoso_seed_pleasuredome/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      446 2023-04-30 18:01:28.000000 datoso_seed_pleasuredome-0.2.0/src/datoso_seed_pleasuredome/actions.py
--rw-r--r--   0 runner    (1001) docker     (123)     3916 2023-04-30 18:01:28.000000 datoso_seed_pleasuredome-0.2.0/src/datoso_seed_pleasuredome/dats.py
--rw-r--r--   0 runner    (1001) docker     (123)     4278 2023-04-30 18:01:28.000000 datoso_seed_pleasuredome-0.2.0/src/datoso_seed_pleasuredome/fetch.py
--rw-r--r--   0 runner    (1001) docker     (123)     1657 2023-04-30 18:01:28.000000 datoso_seed_pleasuredome-0.2.0/src/datoso_seed_pleasuredome/rules.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 18:01:40.262170 datoso_seed_pleasuredome-0.2.0/src/datoso_seed_pleasuredome.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1767 2023-04-30 18:01:40.000000 datoso_seed_pleasuredome-0.2.0/src/datoso_seed_pleasuredome.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      495 2023-04-30 18:01:40.000000 datoso_seed_pleasuredome-0.2.0/src/datoso_seed_pleasuredome.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-30 18:01:40.000000 datoso_seed_pleasuredome-0.2.0/src/datoso_seed_pleasuredome.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       35 2023-04-30 18:01:40.000000 datoso_seed_pleasuredome-0.2.0/src/datoso_seed_pleasuredome.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-04-30 18:01:40.000000 datoso_seed_pleasuredome-0.2.0/src/datoso_seed_pleasuredome.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 04:16:01.946121 datoso_seed_pleasuredome-0.2.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-05-05 04:15:42.000000 datoso_seed_pleasuredome-0.2.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1747 2023-05-05 04:16:01.946121 datoso_seed_pleasuredome-0.2.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-05-05 04:15:42.000000 datoso_seed_pleasuredome-0.2.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-05-05 04:15:42.000000 datoso_seed_pleasuredome-0.2.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      180 2023-05-05 04:16:01.946121 datoso_seed_pleasuredome-0.2.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 04:16:01.942121 datoso_seed_pleasuredome-0.2.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 04:16:01.942121 datoso_seed_pleasuredome-0.2.3/src/datoso_seed_pleasuredome/
+-rw-r--r--   0 runner    (1001) docker     (123)      259 2023-05-05 04:15:42.000000 datoso_seed_pleasuredome-0.2.3/src/datoso_seed_pleasuredome/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1549 2023-05-05 04:15:42.000000 datoso_seed_pleasuredome-0.2.3/src/datoso_seed_pleasuredome/actions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3916 2023-05-05 04:15:42.000000 datoso_seed_pleasuredome-0.2.3/src/datoso_seed_pleasuredome/dats.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4278 2023-05-05 04:15:42.000000 datoso_seed_pleasuredome-0.2.3/src/datoso_seed_pleasuredome/fetch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1657 2023-05-05 04:15:42.000000 datoso_seed_pleasuredome-0.2.3/src/datoso_seed_pleasuredome/rules.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 04:16:01.946121 datoso_seed_pleasuredome-0.2.3/src/datoso_seed_pleasuredome.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1747 2023-05-05 04:16:01.000000 datoso_seed_pleasuredome-0.2.3/src/datoso_seed_pleasuredome.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      495 2023-05-05 04:16:01.000000 datoso_seed_pleasuredome-0.2.3/src/datoso_seed_pleasuredome.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 04:16:01.000000 datoso_seed_pleasuredome-0.2.3/src/datoso_seed_pleasuredome.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-05 04:16:01.000000 datoso_seed_pleasuredome-0.2.3/src/datoso_seed_pleasuredome.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-05-05 04:16:01.000000 datoso_seed_pleasuredome-0.2.3/src/datoso_seed_pleasuredome.egg-info/top_level.txt
```

### Comparing `datoso_seed_pleasuredome-0.2.0/LICENSE` & `datoso_seed_pleasuredome-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `datoso_seed_pleasuredome-0.2.0/PKG-INFO` & `datoso_seed_pleasuredome-0.2.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,23 @@
 Metadata-Version: 2.1
 Name: datoso_seed_pleasuredome
-Version: 0.2.0
+Version: 0.2.3
 Summary: Python command line tool to download and organize your Rom Dat files.
 Author-email: Lacides Miranda <laromicas@hotmail.com>
 License: MIT License
 Project-URL: Source Code, https://github.com/laromicas/datoso_seed_pleasuredome
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
 
 # Datoso Seed Pleasuredome
 
 Datoso is a WIP Python command line tool to download and organize your Dat Roms.
```

### Comparing `datoso_seed_pleasuredome-0.2.0/README.md` & `datoso_seed_pleasuredome-0.2.3/README.md`

 * *Files identical despite different names*

### Comparing `datoso_seed_pleasuredome-0.2.0/pyproject.toml` & `datoso_seed_pleasuredome-0.2.3/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -18,26 +18,18 @@
     "Environment :: Console",
     'License :: OSI Approved :: MIT License',
     "Operating System :: POSIX :: Linux",
     'Programming Language :: Python :: 3',
     'Topic :: System :: Emulators',
 ]
 dependencies = [
-    "datoso>=0.2.0",
-    # "beautifulsoup4>=4.12.1",
-    # "requests>=2.28.2",
+    "datoso>=0.2.3",
 ]
 dynamic = ["version"]
 
-
-[project.optional-dependencies]
-dev = [
-    "ruff>=0.0.261",
-    ]
-
 [project.urls]
 "Source Code"       = "https://github.com/laromicas/datoso_seed_pleasuredome"
 
 [tool.setuptools]
 packages = ["datoso_seed_pleasuredome"]
 license-files = ["LICENSE"]
 include-package-data = true
```

### Comparing `datoso_seed_pleasuredome-0.2.0/src/datoso_seed_pleasuredome/dats.py` & `datoso_seed_pleasuredome-0.2.3/src/datoso_seed_pleasuredome/dats.py`

 * *Files identical despite different names*

### Comparing `datoso_seed_pleasuredome-0.2.0/src/datoso_seed_pleasuredome/fetch.py` & `datoso_seed_pleasuredome-0.2.3/src/datoso_seed_pleasuredome/fetch.py`

 * *Files identical despite different names*

### Comparing `datoso_seed_pleasuredome-0.2.0/src/datoso_seed_pleasuredome/rules.py` & `datoso_seed_pleasuredome-0.2.3/src/datoso_seed_pleasuredome/rules.py`

 * *Files identical despite different names*

### Comparing `datoso_seed_pleasuredome-0.2.0/src/datoso_seed_pleasuredome.egg-info/PKG-INFO` & `datoso_seed_pleasuredome-0.2.3/src/datoso_seed_pleasuredome.egg-info/PKG-INFO`

 * *Files 5% similar despite different names*

```diff
@@ -1,24 +1,23 @@
 Metadata-Version: 2.1
 Name: datoso-seed-pleasuredome
-Version: 0.2.0
+Version: 0.2.3
 Summary: Python command line tool to download and organize your Rom Dat files.
 Author-email: Lacides Miranda <laromicas@hotmail.com>
 License: MIT License
 Project-URL: Source Code, https://github.com/laromicas/datoso_seed_pleasuredome
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
 
 # Datoso Seed Pleasuredome
 
 Datoso is a WIP Python command line tool to download and organize your Dat Roms.
```

