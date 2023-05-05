# Comparing `tmp/fastspell-0.9.0.tar.gz` & `tmp/fastspell-0.9.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fastspell-0.9.0.tar", last modified: Fri Apr 14 15:42:06 2023, max compression
+gzip compressed data, was "fastspell-0.9.1.tar", last modified: Fri May  5 12:58:58 2023, max compression
```

## Comparing `fastspell-0.9.0.tar` & `fastspell-0.9.1.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 15:42:06.664455 fastspell-0.9.0/
--rw-r--r--   0 runner    (1001) docker     (123)    10192 2023-04-14 15:42:06.664455 fastspell-0.9.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     8908 2023-04-14 15:41:56.000000 fastspell-0.9.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1719 2023-04-14 15:41:56.000000 fastspell-0.9.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-14 15:42:06.664455 fastspell-0.9.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 15:42:06.660455 fastspell-0.9.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 15:42:06.664455 fastspell-0.9.0/src/fastspell/
--rw-r--r--   0 runner    (1001) docker     (123)      141 2023-04-14 15:41:56.000000 fastspell-0.9.0/src/fastspell/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 15:42:06.664455 fastspell-0.9.0/src/fastspell/config/
--rw-r--r--   0 runner    (1001) docker     (123)      578 2023-04-14 15:41:56.000000 fastspell-0.9.0/src/fastspell/config/hunspell.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      514 2023-04-14 15:41:56.000000 fastspell-0.9.0/src/fastspell/config/similar.yaml
--rw-r--r--   0 runner    (1001) docker     (123)    12844 2023-04-14 15:41:56.000000 fastspell-0.9.0/src/fastspell/fastspell.py
--rw-r--r--   0 runner    (1001) docker     (123)     4250 2023-04-14 15:41:56.000000 fastspell-0.9.0/src/fastspell/fastspell_download.py
--rw-r--r--   0 runner    (1001) docker     (123)     4351 2023-04-14 15:41:56.000000 fastspell-0.9.0/src/fastspell/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 15:42:06.664455 fastspell-0.9.0/src/fastspell.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    10192 2023-04-14 15:42:06.000000 fastspell-0.9.0/src/fastspell.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      452 2023-04-14 15:42:06.000000 fastspell-0.9.0/src/fastspell.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-14 15:42:06.000000 fastspell-0.9.0/src/fastspell.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      110 2023-04-14 15:42:06.000000 fastspell-0.9.0/src/fastspell.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-04-14 15:42:06.000000 fastspell-0.9.0/src/fastspell.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-14 15:42:06.000000 fastspell-0.9.0/src/fastspell.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 15:42:06.664455 fastspell-0.9.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      842 2023-04-14 15:41:56.000000 fastspell-0.9.0/tests/test_fastspell.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 12:58:58.447302 fastspell-0.9.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    10192 2023-05-05 12:58:58.447302 fastspell-0.9.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8908 2023-05-05 12:58:47.000000 fastspell-0.9.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1725 2023-05-05 12:58:47.000000 fastspell-0.9.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-05 12:58:58.447302 fastspell-0.9.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 12:58:58.447302 fastspell-0.9.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 12:58:58.447302 fastspell-0.9.1/src/fastspell/
+-rw-r--r--   0 runner    (1001) docker     (123)      141 2023-05-05 12:58:47.000000 fastspell-0.9.1/src/fastspell/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 12:58:58.447302 fastspell-0.9.1/src/fastspell/config/
+-rw-r--r--   0 runner    (1001) docker     (123)      578 2023-05-05 12:58:47.000000 fastspell-0.9.1/src/fastspell/config/hunspell.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      514 2023-05-05 12:58:47.000000 fastspell-0.9.1/src/fastspell/config/similar.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)    12844 2023-05-05 12:58:47.000000 fastspell-0.9.1/src/fastspell/fastspell.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4250 2023-05-05 12:58:47.000000 fastspell-0.9.1/src/fastspell/fastspell_download.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4351 2023-05-05 12:58:47.000000 fastspell-0.9.1/src/fastspell/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 12:58:58.447302 fastspell-0.9.1/src/fastspell.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    10192 2023-05-05 12:58:58.000000 fastspell-0.9.1/src/fastspell.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      452 2023-05-05 12:58:58.000000 fastspell-0.9.1/src/fastspell.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 12:58:58.000000 fastspell-0.9.1/src/fastspell.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      110 2023-05-05 12:58:58.000000 fastspell-0.9.1/src/fastspell.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       91 2023-05-05 12:58:58.000000 fastspell-0.9.1/src/fastspell.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-05 12:58:58.000000 fastspell-0.9.1/src/fastspell.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 12:58:58.447302 fastspell-0.9.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      842 2023-05-05 12:58:47.000000 fastspell-0.9.1/tests/test_fastspell.py
```

### Comparing `fastspell-0.9.0/PKG-INFO` & `fastspell-0.9.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fastspell
-Version: 0.9.0
+Version: 0.9.1
 Summary: Targetted language identifier, based on FastText and Hunspell.
 Author-email: Prompsit Language Engineering <info@prompsit.com>
 Maintainer-email: Marta Bañon <mbanon@prompsit.com>, Jaume Zaragoza <jzaragoza@prompsit.com>
 Project-URL: Homepage, https://github.com/mbanon/fastspell
 Project-URL: FastSpell on GitHub, https://github.com/mbanon/fastspell
 Project-URL: Prompsit Language Engineering, http://www.prompsit.com
 Project-URL: Paracrawl, https://paracrawl.eu/
```

### Comparing `fastspell-0.9.0/README.md` & `fastspell-0.9.1/README.md`

 * *Files identical despite different names*

### Comparing `fastspell-0.9.0/pyproject.toml` & `fastspell-0.9.1/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 [project]
 name = "fastspell"
-version = "0.9.0"
+version = "0.9.1"
 license = {file = "LICENSE"}
 readme = "README.md"
 description = "Targetted language identifier, based on FastText and Hunspell."
 requires-python = ">=3.8"
 dependencies = [
     "cyhunspell>=2.0.2, <=2.0.3",
     "fastspell-dictionaries==3.0",
-    "fasttext==0.9.2",
+    "fasttext-wheel==0.9.2",
     "urllib3",
     "PyYAML",
 ]
 classifiers = [
     "Environment :: Console",
     "Intended Audience :: Science/Research",
     "Programming Language :: Python :: 3.8",
```

### Comparing `fastspell-0.9.0/src/fastspell/config/hunspell.yaml` & `fastspell-0.9.1/src/fastspell/config/hunspell.yaml`

 * *Files identical despite different names*

### Comparing `fastspell-0.9.0/src/fastspell/config/similar.yaml` & `fastspell-0.9.1/src/fastspell/config/similar.yaml`

 * *Files identical despite different names*

### Comparing `fastspell-0.9.0/src/fastspell/fastspell.py` & `fastspell-0.9.1/src/fastspell/fastspell.py`

 * *Files identical despite different names*

### Comparing `fastspell-0.9.0/src/fastspell/fastspell_download.py` & `fastspell-0.9.1/src/fastspell/fastspell_download.py`

 * *Files identical despite different names*

### Comparing `fastspell-0.9.0/src/fastspell/util.py` & `fastspell-0.9.1/src/fastspell/util.py`

 * *Files identical despite different names*

### Comparing `fastspell-0.9.0/src/fastspell.egg-info/PKG-INFO` & `fastspell-0.9.1/src/fastspell.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: fastspell
-Version: 0.9.0
+Version: 0.9.1
 Summary: Targetted language identifier, based on FastText and Hunspell.
 Author-email: Prompsit Language Engineering <info@prompsit.com>
 Maintainer-email: Marta Bañon <mbanon@prompsit.com>, Jaume Zaragoza <jzaragoza@prompsit.com>
 Project-URL: Homepage, https://github.com/mbanon/fastspell
 Project-URL: FastSpell on GitHub, https://github.com/mbanon/fastspell
 Project-URL: Prompsit Language Engineering, http://www.prompsit.com
 Project-URL: Paracrawl, https://paracrawl.eu/
```

### Comparing `fastspell-0.9.0/tests/test_fastspell.py` & `fastspell-0.9.1/tests/test_fastspell.py`

 * *Files identical despite different names*

