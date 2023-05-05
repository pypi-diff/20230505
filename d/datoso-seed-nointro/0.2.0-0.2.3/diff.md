# Comparing `tmp/datoso_seed_nointro-0.2.0.tar.gz` & `tmp/datoso_seed_nointro-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "datoso_seed_nointro-0.2.0.tar", last modified: Sun Apr 30 18:02:27 2023, max compression
+gzip compressed data, was "datoso_seed_nointro-0.2.3.tar", last modified: Fri May  5 04:12:43 2023, max compression
```

## Comparing `datoso_seed_nointro-0.2.0.tar` & `datoso_seed_nointro-0.2.3.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 18:02:27.610928 datoso_seed_nointro-0.2.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-04-30 18:02:12.000000 datoso_seed_nointro-0.2.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1928 2023-04-30 18:02:27.610928 datoso_seed_nointro-0.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-04-30 18:02:12.000000 datoso_seed_nointro-0.2.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1137 2023-04-30 18:02:12.000000 datoso_seed_nointro-0.2.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      180 2023-04-30 18:02:27.614929 datoso_seed_nointro-0.2.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 18:02:27.610928 datoso_seed_nointro-0.2.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 18:02:27.610928 datoso_seed_nointro-0.2.0/src/datoso_seed_nointro/
--rw-r--r--   0 runner    (1001) docker     (123)      368 2023-04-30 18:02:12.000000 datoso_seed_nointro-0.2.0/src/datoso_seed_nointro/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      427 2023-04-30 18:02:12.000000 datoso_seed_nointro-0.2.0/src/datoso_seed_nointro/actions.py
--rw-r--r--   0 runner    (1001) docker     (123)     3066 2023-04-30 18:02:12.000000 datoso_seed_nointro-0.2.0/src/datoso_seed_nointro/dats.py
--rw-r--r--   0 runner    (1001) docker     (123)     4663 2023-04-30 18:02:12.000000 datoso_seed_nointro-0.2.0/src/datoso_seed_nointro/fetch.py
--rw-r--r--   0 runner    (1001) docker     (123)      526 2023-04-30 18:02:12.000000 datoso_seed_nointro-0.2.0/src/datoso_seed_nointro/rules.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 18:02:27.610928 datoso_seed_nointro-0.2.0/src/datoso_seed_nointro.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1928 2023-04-30 18:02:27.000000 datoso_seed_nointro-0.2.0/src/datoso_seed_nointro.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      445 2023-04-30 18:02:27.000000 datoso_seed_nointro-0.2.0/src/datoso_seed_nointro.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-30 18:02:27.000000 datoso_seed_nointro-0.2.0/src/datoso_seed_nointro.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-04-30 18:02:27.000000 datoso_seed_nointro-0.2.0/src/datoso_seed_nointro.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-04-30 18:02:27.000000 datoso_seed_nointro-0.2.0/src/datoso_seed_nointro.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 04:12:43.017877 datoso_seed_nointro-0.2.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-05-05 04:12:28.000000 datoso_seed_nointro-0.2.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1907 2023-05-05 04:12:43.017877 datoso_seed_nointro-0.2.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1237 2023-05-05 04:12:28.000000 datoso_seed_nointro-0.2.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-05-05 04:12:28.000000 datoso_seed_nointro-0.2.3/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      180 2023-05-05 04:12:43.021877 datoso_seed_nointro-0.2.3/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 04:12:43.013877 datoso_seed_nointro-0.2.3/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 04:12:43.017877 datoso_seed_nointro-0.2.3/src/datoso_seed_nointro/
+-rw-r--r--   0 runner    (1001) docker     (123)      368 2023-05-05 04:12:28.000000 datoso_seed_nointro-0.2.3/src/datoso_seed_nointro/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      427 2023-05-05 04:12:28.000000 datoso_seed_nointro-0.2.3/src/datoso_seed_nointro/actions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3066 2023-05-05 04:12:28.000000 datoso_seed_nointro-0.2.3/src/datoso_seed_nointro/dats.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4663 2023-05-05 04:12:28.000000 datoso_seed_nointro-0.2.3/src/datoso_seed_nointro/fetch.py
+-rw-r--r--   0 runner    (1001) docker     (123)      526 2023-05-05 04:12:28.000000 datoso_seed_nointro-0.2.3/src/datoso_seed_nointro/rules.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 04:12:43.017877 datoso_seed_nointro-0.2.3/src/datoso_seed_nointro.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1907 2023-05-05 04:12:43.000000 datoso_seed_nointro-0.2.3/src/datoso_seed_nointro.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      445 2023-05-05 04:12:43.000000 datoso_seed_nointro-0.2.3/src/datoso_seed_nointro.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 04:12:43.000000 datoso_seed_nointro-0.2.3/src/datoso_seed_nointro.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-05-05 04:12:43.000000 datoso_seed_nointro-0.2.3/src/datoso_seed_nointro.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-05-05 04:12:43.000000 datoso_seed_nointro-0.2.3/src/datoso_seed_nointro.egg-info/top_level.txt
```

### Comparing `datoso_seed_nointro-0.2.0/LICENSE` & `datoso_seed_nointro-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `datoso_seed_nointro-0.2.0/PKG-INFO` & `datoso_seed_nointro-0.2.3/src/datoso_seed_nointro.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,24 +1,23 @@
 Metadata-Version: 2.1
-Name: datoso_seed_nointro
-Version: 0.2.0
+Name: datoso-seed-nointro
+Version: 0.2.3
 Summary: Python command line tool to download and organize your Rom Dat files.
 Author-email: Lacides Miranda <laromicas@hotmail.com>
 License: MIT License
 Project-URL: Source Code, https://github.com/laromicas/datoso_seed_nointro
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
 
 # Datoso Seed No-Intro
 
 Datoso is a WIP Python command line tool to download and organize your Dat Roms.
@@ -32,15 +31,14 @@
 
 Datoso requires python 3.10+.
 
 Install firefox and geckodriver, put geckodriver in your path.
 [Tutorial](https://www.browserstack.com/guide/geckodriver-selenium-python)
 
 Use pip (recommended to use a virtual environment):
-
 If you only need this plugin you can install it directly
 ``` bash
 pip install datoso_seed_nointro
 
 ```
 
 ## Usage
```

### Comparing `datoso_seed_nointro-0.2.0/README.md` & `datoso_seed_nointro-0.2.3/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -13,15 +13,14 @@
 
 Datoso requires python 3.10+.
 
 Install firefox and geckodriver, put geckodriver in your path.
 [Tutorial](https://www.browserstack.com/guide/geckodriver-selenium-python)
 
 Use pip (recommended to use a virtual environment):
-
 If you only need this plugin you can install it directly
 ``` bash
 pip install datoso_seed_nointro
 
 ```
 
 ## Usage
```

### Comparing `datoso_seed_nointro-0.2.0/pyproject.toml` & `datoso_seed_nointro-0.2.3/pyproject.toml`

 * *Files 9% similar despite different names*

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
     "selenium==4.8.3",
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
 "Source Code"       = "https://github.com/laromicas/datoso_seed_nointro"
 
 [tool.setuptools]
 packages = ["datoso_seed_nointro"]
 license-files = ["LICENSE"]
 include-package-data = true
```

### Comparing `datoso_seed_nointro-0.2.0/src/datoso_seed_nointro/dats.py` & `datoso_seed_nointro-0.2.3/src/datoso_seed_nointro/dats.py`

 * *Files identical despite different names*

### Comparing `datoso_seed_nointro-0.2.0/src/datoso_seed_nointro/fetch.py` & `datoso_seed_nointro-0.2.3/src/datoso_seed_nointro/fetch.py`

 * *Files identical despite different names*

### Comparing `datoso_seed_nointro-0.2.0/src/datoso_seed_nointro/rules.py` & `datoso_seed_nointro-0.2.3/src/datoso_seed_nointro/rules.py`

 * *Files identical despite different names*

### Comparing `datoso_seed_nointro-0.2.0/src/datoso_seed_nointro.egg-info/PKG-INFO` & `datoso_seed_nointro-0.2.3/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,24 +1,23 @@
 Metadata-Version: 2.1
-Name: datoso-seed-nointro
-Version: 0.2.0
+Name: datoso_seed_nointro
+Version: 0.2.3
 Summary: Python command line tool to download and organize your Rom Dat files.
 Author-email: Lacides Miranda <laromicas@hotmail.com>
 License: MIT License
 Project-URL: Source Code, https://github.com/laromicas/datoso_seed_nointro
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
 
 # Datoso Seed No-Intro
 
 Datoso is a WIP Python command line tool to download and organize your Dat Roms.
@@ -32,15 +31,14 @@
 
 Datoso requires python 3.10+.
 
 Install firefox and geckodriver, put geckodriver in your path.
 [Tutorial](https://www.browserstack.com/guide/geckodriver-selenium-python)
 
 Use pip (recommended to use a virtual environment):
-
 If you only need this plugin you can install it directly
 ``` bash
 pip install datoso_seed_nointro
 
 ```
 
 ## Usage
```

