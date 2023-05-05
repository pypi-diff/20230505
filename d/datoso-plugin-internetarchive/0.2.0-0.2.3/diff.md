# Comparing `tmp/datoso_plugin_internetarchive-0.2.0.tar.gz` & `tmp/datoso_plugin_internetarchive-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "datoso_plugin_internetarchive-0.2.0.tar", last modified: Sun Apr 30 17:59:19 2023, max compression
+gzip compressed data, was "datoso_plugin_internetarchive-0.2.3.tar", last modified: Fri May  5 04:21:18 2023, max compression
```

## Comparing `datoso_plugin_internetarchive-0.2.0.tar` & `datoso_plugin_internetarchive-0.2.3.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 17:59:19.299252 datoso_plugin_internetarchive-0.2.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-04-30 17:59:05.000000 datoso_plugin_internetarchive-0.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1709 2023-04-30 17:59:19.299252 datoso_plugin_internetarchive-0.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      999 2023-04-30 17:59:05.000000 datoso_plugin_internetarchive-0.2.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1184 2023-04-30 17:59:05.000000 datoso_plugin_internetarchive-0.2.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      180 2023-04-30 17:59:19.299252 datoso_plugin_internetarchive-0.2.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 17:59:19.295252 datoso_plugin_internetarchive-0.2.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 17:59:19.295252 datoso_plugin_internetarchive-0.2.0/src/datoso_plugin_internetarchive/
--rw-r--r--   0 runner    (1001) docker     (123)      221 2023-04-30 17:59:05.000000 datoso_plugin_internetarchive-0.2.0/src/datoso_plugin_internetarchive/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2300 2023-04-30 17:59:05.000000 datoso_plugin_internetarchive-0.2.0/src/datoso_plugin_internetarchive/fetch.py
--rw-r--r--   0 runner    (1001) docker     (123)     1550 2023-04-30 17:59:05.000000 datoso_plugin_internetarchive-0.2.0/src/datoso_plugin_internetarchive/ia.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 17:59:19.299252 datoso_plugin_internetarchive-0.2.0/src/datoso_plugin_internetarchive.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1709 2023-04-30 17:59:19.000000 datoso_plugin_internetarchive-0.2.0/src/datoso_plugin_internetarchive.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      455 2023-04-30 17:59:19.000000 datoso_plugin_internetarchive-0.2.0/src/datoso_plugin_internetarchive.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-30 17:59:19.000000 datoso_plugin_internetarchive-0.2.0/src/datoso_plugin_internetarchive.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-04-30 17:59:19.000000 datoso_plugin_internetarchive-0.2.0/src/datoso_plugin_internetarchive.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-04-30 17:59:19.000000 datoso_plugin_internetarchive-0.2.0/src/datoso_plugin_internetarchive.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 04:21:18.330601 datoso_plugin_internetarchive-0.2.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-05-05 04:21:05.000000 datoso_plugin_internetarchive-0.2.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1689 2023-05-05 04:21:18.330601 datoso_plugin_internetarchive-0.2.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      999 2023-05-05 04:21:05.000000 datoso_plugin_internetarchive-0.2.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1114 2023-05-05 04:21:05.000000 datoso_plugin_internetarchive-0.2.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      180 2023-05-05 04:21:18.330601 datoso_plugin_internetarchive-0.2.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 04:21:18.326601 datoso_plugin_internetarchive-0.2.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 04:21:18.330601 datoso_plugin_internetarchive-0.2.3/src/datoso_plugin_internetarchive/
+-rw-r--r--   0 runner    (1001) docker     (123)      221 2023-05-05 04:21:05.000000 datoso_plugin_internetarchive-0.2.3/src/datoso_plugin_internetarchive/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2300 2023-05-05 04:21:05.000000 datoso_plugin_internetarchive-0.2.3/src/datoso_plugin_internetarchive/fetch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1550 2023-05-05 04:21:05.000000 datoso_plugin_internetarchive-0.2.3/src/datoso_plugin_internetarchive/ia.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 04:21:18.330601 datoso_plugin_internetarchive-0.2.3/src/datoso_plugin_internetarchive.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1689 2023-05-05 04:21:18.000000 datoso_plugin_internetarchive-0.2.3/src/datoso_plugin_internetarchive.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      455 2023-05-05 04:21:18.000000 datoso_plugin_internetarchive-0.2.3/src/datoso_plugin_internetarchive.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 04:21:18.000000 datoso_plugin_internetarchive-0.2.3/src/datoso_plugin_internetarchive.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       37 2023-05-05 04:21:18.000000 datoso_plugin_internetarchive-0.2.3/src/datoso_plugin_internetarchive.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-05-05 04:21:18.000000 datoso_plugin_internetarchive-0.2.3/src/datoso_plugin_internetarchive.egg-info/top_level.txt
```

### Comparing `datoso_plugin_internetarchive-0.2.0/LICENSE` & `datoso_plugin_internetarchive-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `datoso_plugin_internetarchive-0.2.0/PKG-INFO` & `datoso_plugin_internetarchive-0.2.3/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,24 +1,23 @@
 Metadata-Version: 2.1
 Name: datoso_plugin_internetarchive
-Version: 0.2.0
+Version: 0.2.3
 Summary: Python command line tool to download and organize your Rom Dat files.
 Author-email: Lacides Miranda <laromicas@hotmail.com>
 License: MIT License
 Project-URL: Source Code, https://github.com/laromicas/datoso_plugin_internetarchive
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
 
 # Datoso Plugin InternetArchive
 
 Datoso is a WIP Python command line tool to download and organize your Dat Roms.
```

### Comparing `datoso_plugin_internetarchive-0.2.0/README.md` & `datoso_plugin_internetarchive-0.2.3/README.md`

 * *Files identical despite different names*

### Comparing `datoso_plugin_internetarchive-0.2.0/pyproject.toml` & `datoso_plugin_internetarchive-0.2.3/pyproject.toml`

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
+    "datoso>=0.2.3",
     "internetarchive>=3.0.0",
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
 "Source Code"       = "https://github.com/laromicas/datoso_plugin_internetarchive"
 
 [tool.setuptools]
 packages = ["datoso_plugin_internetarchive"]
 license-files = ["LICENSE"]
 include-package-data = true
```

### Comparing `datoso_plugin_internetarchive-0.2.0/src/datoso_plugin_internetarchive/fetch.py` & `datoso_plugin_internetarchive-0.2.3/src/datoso_plugin_internetarchive/fetch.py`

 * *Files identical despite different names*

### Comparing `datoso_plugin_internetarchive-0.2.0/src/datoso_plugin_internetarchive/ia.py` & `datoso_plugin_internetarchive-0.2.3/src/datoso_plugin_internetarchive/ia.py`

 * *Files identical despite different names*

### Comparing `datoso_plugin_internetarchive-0.2.0/src/datoso_plugin_internetarchive.egg-info/PKG-INFO` & `datoso_plugin_internetarchive-0.2.3/src/datoso_plugin_internetarchive.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,24 +1,23 @@
 Metadata-Version: 2.1
 Name: datoso-plugin-internetarchive
-Version: 0.2.0
+Version: 0.2.3
 Summary: Python command line tool to download and organize your Rom Dat files.
 Author-email: Lacides Miranda <laromicas@hotmail.com>
 License: MIT License
 Project-URL: Source Code, https://github.com/laromicas/datoso_plugin_internetarchive
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
 
 # Datoso Plugin InternetArchive
 
 Datoso is a WIP Python command line tool to download and organize your Dat Roms.
```

