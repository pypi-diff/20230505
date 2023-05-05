# Comparing `tmp/datoso_seed_translatedenglish-0.0.1.tar.gz` & `tmp/datoso_seed_translatedenglish-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "datoso_seed_translatedenglish-0.0.1.tar", last modified: Sun Apr 30 18:17:54 2023, max compression
+gzip compressed data, was "datoso_seed_translatedenglish-0.2.3.tar", last modified: Fri May  5 04:25:10 2023, max compression
```

## Comparing `datoso_seed_translatedenglish-0.0.1.tar` & `datoso_seed_translatedenglish-0.2.3.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 18:17:54.482803 datoso_seed_translatedenglish-0.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-04-30 18:17:42.000000 datoso_seed_translatedenglish-0.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1787 2023-04-30 18:17:54.482803 datoso_seed_translatedenglish-0.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-04-30 18:17:42.000000 datoso_seed_translatedenglish-0.0.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1198 2023-04-30 18:17:42.000000 datoso_seed_translatedenglish-0.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      180 2023-04-30 18:17:54.482803 datoso_seed_translatedenglish-0.0.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 18:17:54.482803 datoso_seed_translatedenglish-0.0.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 18:17:54.482803 datoso_seed_translatedenglish-0.0.1/src/datoso_seed_translatedenglish/
--rw-r--r--   0 runner    (1001) docker     (123)      250 2023-04-30 18:17:42.000000 datoso_seed_translatedenglish-0.0.1/src/datoso_seed_translatedenglish/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      457 2023-04-30 18:17:42.000000 datoso_seed_translatedenglish-0.0.1/src/datoso_seed_translatedenglish/actions.py
--rw-r--r--   0 runner    (1001) docker     (123)     1166 2023-04-30 18:17:42.000000 datoso_seed_translatedenglish-0.0.1/src/datoso_seed_translatedenglish/dats.py
--rw-r--r--   0 runner    (1001) docker     (123)      490 2023-04-30 18:17:42.000000 datoso_seed_translatedenglish-0.0.1/src/datoso_seed_translatedenglish/fetch.py
--rw-r--r--   0 runner    (1001) docker     (123)      419 2023-04-30 18:17:42.000000 datoso_seed_translatedenglish-0.0.1/src/datoso_seed_translatedenglish/rules.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 18:17:54.482803 datoso_seed_translatedenglish-0.0.1/src/datoso_seed_translatedenglish.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1787 2023-04-30 18:17:54.000000 datoso_seed_translatedenglish-0.0.1/src/datoso_seed_translatedenglish.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      545 2023-04-30 18:17:54.000000 datoso_seed_translatedenglish-0.0.1/src/datoso_seed_translatedenglish.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-30 18:17:54.000000 datoso_seed_translatedenglish-0.0.1/src/datoso_seed_translatedenglish.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       72 2023-04-30 18:17:54.000000 datoso_seed_translatedenglish-0.0.1/src/datoso_seed_translatedenglish.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-04-30 18:17:54.000000 datoso_seed_translatedenglish-0.0.1/src/datoso_seed_translatedenglish.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 04:25:10.382086 datoso_seed_translatedenglish-0.2.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-05-05 04:24:48.000000 datoso_seed_translatedenglish-0.2.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1767 2023-05-05 04:25:10.382086 datoso_seed_translatedenglish-0.2.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-05-05 04:24:48.000000 datoso_seed_translatedenglish-0.2.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1128 2023-05-05 04:24:48.000000 datoso_seed_translatedenglish-0.2.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      180 2023-05-05 04:25:10.386086 datoso_seed_translatedenglish-0.2.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 04:25:10.382086 datoso_seed_translatedenglish-0.2.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 04:25:10.382086 datoso_seed_translatedenglish-0.2.3/src/datoso_seed_translatedenglish/
+-rw-r--r--   0 runner    (1001) docker     (123)      250 2023-05-05 04:24:48.000000 datoso_seed_translatedenglish-0.2.3/src/datoso_seed_translatedenglish/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      457 2023-05-05 04:24:48.000000 datoso_seed_translatedenglish-0.2.3/src/datoso_seed_translatedenglish/actions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1166 2023-05-05 04:24:48.000000 datoso_seed_translatedenglish-0.2.3/src/datoso_seed_translatedenglish/dats.py
+-rw-r--r--   0 runner    (1001) docker     (123)      456 2023-05-05 04:24:48.000000 datoso_seed_translatedenglish-0.2.3/src/datoso_seed_translatedenglish/fetch.py
+-rw-r--r--   0 runner    (1001) docker     (123)      419 2023-05-05 04:24:48.000000 datoso_seed_translatedenglish-0.2.3/src/datoso_seed_translatedenglish/rules.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 04:25:10.382086 datoso_seed_translatedenglish-0.2.3/src/datoso_seed_translatedenglish.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1767 2023-05-05 04:25:10.000000 datoso_seed_translatedenglish-0.2.3/src/datoso_seed_translatedenglish.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      545 2023-05-05 04:25:10.000000 datoso_seed_translatedenglish-0.2.3/src/datoso_seed_translatedenglish.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 04:25:10.000000 datoso_seed_translatedenglish-0.2.3/src/datoso_seed_translatedenglish.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-05-05 04:25:10.000000 datoso_seed_translatedenglish-0.2.3/src/datoso_seed_translatedenglish.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-05-05 04:25:10.000000 datoso_seed_translatedenglish-0.2.3/src/datoso_seed_translatedenglish.egg-info/top_level.txt
```

### Comparing `datoso_seed_translatedenglish-0.0.1/LICENSE` & `datoso_seed_translatedenglish-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `datoso_seed_translatedenglish-0.0.1/PKG-INFO` & `datoso_seed_translatedenglish-0.2.3/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,24 +1,23 @@
 Metadata-Version: 2.1
 Name: datoso_seed_translatedenglish
-Version: 0.0.1
+Version: 0.2.3
 Summary: Python command line tool to download and organize your Rom Dat files.
 Author-email: Lacides Miranda <laromicas@hotmail.com>
 License: MIT License
 Project-URL: Source Code, https://github.com/laromicas/datoso_seed_translatedenglish
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
 
 # Datoso Seed Translated English
 
 Datoso is a WIP Python command line tool to download and organize your Dat Roms.
```

### Comparing `datoso_seed_translatedenglish-0.0.1/README.md` & `datoso_seed_translatedenglish-0.2.3/README.md`

 * *Files identical despite different names*

### Comparing `datoso_seed_translatedenglish-0.0.1/pyproject.toml` & `datoso_seed_translatedenglish-0.2.3/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -18,26 +18,19 @@
     "Environment :: Console",
     'License :: OSI Approved :: MIT License',
     "Operating System :: POSIX :: Linux",
     'Programming Language :: Python :: 3',
     'Topic :: System :: Emulators',
 ]
 dependencies = [
-    "datoso>=0.2.0",
-    "datoso-plugin-internetarchive>=0.0.1",
+    "datoso>=0.2.3",
+    "datoso-plugin-internetarchive>=0.2.3",
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
 "Source Code"       = "https://github.com/laromicas/datoso_seed_translatedenglish"
 
 [tool.setuptools]
 packages = ["datoso_seed_translatedenglish"]
 license-files = ["LICENSE"]
 include-package-data = true
```

### Comparing `datoso_seed_translatedenglish-0.0.1/src/datoso_seed_translatedenglish/dats.py` & `datoso_seed_translatedenglish-0.2.3/src/datoso_seed_translatedenglish/dats.py`

 * *Files identical despite different names*

### Comparing `datoso_seed_translatedenglish-0.0.1/src/datoso_seed_translatedenglish.egg-info/PKG-INFO` & `datoso_seed_translatedenglish-0.2.3/src/datoso_seed_translatedenglish.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,24 +1,23 @@
 Metadata-Version: 2.1
 Name: datoso-seed-translatedenglish
-Version: 0.0.1
+Version: 0.2.3
 Summary: Python command line tool to download and organize your Rom Dat files.
 Author-email: Lacides Miranda <laromicas@hotmail.com>
 License: MIT License
 Project-URL: Source Code, https://github.com/laromicas/datoso_seed_translatedenglish
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
 
 # Datoso Seed Translated English
 
 Datoso is a WIP Python command line tool to download and organize your Dat Roms.
```

### Comparing `datoso_seed_translatedenglish-0.0.1/src/datoso_seed_translatedenglish.egg-info/SOURCES.txt` & `datoso_seed_translatedenglish-0.2.3/src/datoso_seed_translatedenglish.egg-info/SOURCES.txt`

 * *Files identical despite different names*

