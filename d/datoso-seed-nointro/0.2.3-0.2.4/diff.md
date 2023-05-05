# Comparing `tmp/datoso_seed_nointro-0.2.3.tar.gz` & `tmp/datoso_seed_nointro-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "datoso_seed_nointro-0.2.3.tar", last modified: Fri May  5 04:12:43 2023, max compression
+gzip compressed data, was "datoso_seed_nointro-0.2.4.tar", last modified: Fri May  5 05:01:42 2023, max compression
```

## Comparing `datoso_seed_nointro-0.2.3.tar` & `datoso_seed_nointro-0.2.4.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 04:12:43.017877 datoso_seed_nointro-0.2.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-05-05 04:12:28.000000 datoso_seed_nointro-0.2.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     1907 2023-05-05 04:12:43.017877 datoso_seed_nointro-0.2.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1237 2023-05-05 04:12:28.000000 datoso_seed_nointro-0.2.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-05-05 04:12:28.000000 datoso_seed_nointro-0.2.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      180 2023-05-05 04:12:43.021877 datoso_seed_nointro-0.2.3/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 04:12:43.013877 datoso_seed_nointro-0.2.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 04:12:43.017877 datoso_seed_nointro-0.2.3/src/datoso_seed_nointro/
--rw-r--r--   0 runner    (1001) docker     (123)      368 2023-05-05 04:12:28.000000 datoso_seed_nointro-0.2.3/src/datoso_seed_nointro/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      427 2023-05-05 04:12:28.000000 datoso_seed_nointro-0.2.3/src/datoso_seed_nointro/actions.py
--rw-r--r--   0 runner    (1001) docker     (123)     3066 2023-05-05 04:12:28.000000 datoso_seed_nointro-0.2.3/src/datoso_seed_nointro/dats.py
--rw-r--r--   0 runner    (1001) docker     (123)     4663 2023-05-05 04:12:28.000000 datoso_seed_nointro-0.2.3/src/datoso_seed_nointro/fetch.py
--rw-r--r--   0 runner    (1001) docker     (123)      526 2023-05-05 04:12:28.000000 datoso_seed_nointro-0.2.3/src/datoso_seed_nointro/rules.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 04:12:43.017877 datoso_seed_nointro-0.2.3/src/datoso_seed_nointro.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1907 2023-05-05 04:12:43.000000 datoso_seed_nointro-0.2.3/src/datoso_seed_nointro.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      445 2023-05-05 04:12:43.000000 datoso_seed_nointro-0.2.3/src/datoso_seed_nointro.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 04:12:43.000000 datoso_seed_nointro-0.2.3/src/datoso_seed_nointro.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-05-05 04:12:43.000000 datoso_seed_nointro-0.2.3/src/datoso_seed_nointro.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-05-05 04:12:43.000000 datoso_seed_nointro-0.2.3/src/datoso_seed_nointro.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 05:01:42.564749 datoso_seed_nointro-0.2.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-05-05 05:01:22.000000 datoso_seed_nointro-0.2.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     1907 2023-05-05 05:01:42.564749 datoso_seed_nointro-0.2.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1237 2023-05-05 05:01:22.000000 datoso_seed_nointro-0.2.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-05-05 05:01:22.000000 datoso_seed_nointro-0.2.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      180 2023-05-05 05:01:42.564749 datoso_seed_nointro-0.2.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 05:01:42.564749 datoso_seed_nointro-0.2.4/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 05:01:42.564749 datoso_seed_nointro-0.2.4/src/datoso_seed_nointro/
+-rw-r--r--   0 runner    (1001) docker     (123)      368 2023-05-05 05:01:22.000000 datoso_seed_nointro-0.2.4/src/datoso_seed_nointro/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      427 2023-05-05 05:01:22.000000 datoso_seed_nointro-0.2.4/src/datoso_seed_nointro/actions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3066 2023-05-05 05:01:22.000000 datoso_seed_nointro-0.2.4/src/datoso_seed_nointro/dats.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4689 2023-05-05 05:01:22.000000 datoso_seed_nointro-0.2.4/src/datoso_seed_nointro/fetch.py
+-rw-r--r--   0 runner    (1001) docker     (123)      526 2023-05-05 05:01:22.000000 datoso_seed_nointro-0.2.4/src/datoso_seed_nointro/rules.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 05:01:42.564749 datoso_seed_nointro-0.2.4/src/datoso_seed_nointro.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1907 2023-05-05 05:01:42.000000 datoso_seed_nointro-0.2.4/src/datoso_seed_nointro.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      445 2023-05-05 05:01:42.000000 datoso_seed_nointro-0.2.4/src/datoso_seed_nointro.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 05:01:42.000000 datoso_seed_nointro-0.2.4/src/datoso_seed_nointro.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-05-05 05:01:42.000000 datoso_seed_nointro-0.2.4/src/datoso_seed_nointro.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-05-05 05:01:42.000000 datoso_seed_nointro-0.2.4/src/datoso_seed_nointro.egg-info/top_level.txt
```

### Comparing `datoso_seed_nointro-0.2.3/LICENSE` & `datoso_seed_nointro-0.2.4/LICENSE`

 * *Files identical despite different names*

### Comparing `datoso_seed_nointro-0.2.3/PKG-INFO` & `datoso_seed_nointro-0.2.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datoso_seed_nointro
-Version: 0.2.3
+Version: 0.2.4
 Summary: Python command line tool to download and organize your Rom Dat files.
 Author-email: Lacides Miranda <laromicas@hotmail.com>
 License: MIT License
 Project-URL: Source Code, https://github.com/laromicas/datoso_seed_nointro
 Keywords: emulators,roms
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
```

### Comparing `datoso_seed_nointro-0.2.3/README.md` & `datoso_seed_nointro-0.2.4/README.md`

 * *Files identical despite different names*

### Comparing `datoso_seed_nointro-0.2.3/pyproject.toml` & `datoso_seed_nointro-0.2.4/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -18,15 +18,15 @@
     "Environment :: Console",
     'License :: OSI Approved :: MIT License',
     "Operating System :: POSIX :: Linux",
     'Programming Language :: Python :: 3',
     'Topic :: System :: Emulators',
 ]
 dependencies = [
-    "datoso>=0.2.3",
+    "datoso>=0.2.5",
     "selenium==4.8.3",
 ]
 dynamic = ["version"]
 
 [project.urls]
 "Source Code"       = "https://github.com/laromicas/datoso_seed_nointro"
```

### Comparing `datoso_seed_nointro-0.2.3/src/datoso_seed_nointro/dats.py` & `datoso_seed_nointro-0.2.4/src/datoso_seed_nointro/dats.py`

 * *Files identical despite different names*

### Comparing `datoso_seed_nointro-0.2.3/src/datoso_seed_nointro/fetch.py` & `datoso_seed_nointro-0.2.4/src/datoso_seed_nointro/fetch.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 from pathlib import Path
-import shutil
 import sys
 import time
 import random
 import zipfile
 
 from selenium import webdriver
 from selenium.webdriver import FirefoxOptions
 from selenium.webdriver.common.by import By
+from datoso.helpers import FileUtils
+from datoso.configuration.folder_helper import Folders
 
 from datoso_seed_nointro import __preffix__
-from datoso.configuration.folder_helper import Folders
 
 
 def execute_with_retry(method, max_attempts):
     """Executes a method with several times until it fails all or is executed fine."""
     exc = None
     for _ in range(0, max_attempts):
         try:
@@ -133,15 +133,15 @@
 
 
 def download_dats(folder_helper: Folders):
     download_daily(folder_helper)
     downloaded_file = get_downloaded_file(folder_helper)
     print('Extracting dats')
     extract_dats(downloaded_file, folder_helper)
-    shutil.move(downloaded_file, folder_helper.backup)
+    FileUtils.move(downloaded_file, folder_helper.backup)
 
 
 def fetch():
     folder_helper = Folders(seed=__preffix__)
     folder_helper.clean_dats()
     folder_helper.create_all()
     download_dats(folder_helper)
```

### Comparing `datoso_seed_nointro-0.2.3/src/datoso_seed_nointro/rules.py` & `datoso_seed_nointro-0.2.4/src/datoso_seed_nointro/rules.py`

 * *Files identical despite different names*

### Comparing `datoso_seed_nointro-0.2.3/src/datoso_seed_nointro.egg-info/PKG-INFO` & `datoso_seed_nointro-0.2.4/src/datoso_seed_nointro.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: datoso-seed-nointro
-Version: 0.2.3
+Version: 0.2.4
 Summary: Python command line tool to download and organize your Rom Dat files.
 Author-email: Lacides Miranda <laromicas@hotmail.com>
 License: MIT License
 Project-URL: Source Code, https://github.com/laromicas/datoso_seed_nointro
 Keywords: emulators,roms
 Classifier: Development Status :: 3 - Alpha
 Classifier: Environment :: Console
```

