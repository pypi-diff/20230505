# Comparing `tmp/userfs-0.1.0.tar.gz` & `tmp/userfs-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "userfs-0.1.0.tar", last modified: Thu May  4 06:15:14 2023, max compression
+gzip compressed data, was "userfs-0.2.0.tar", last modified: Fri May  5 08:36:45 2023, max compression
```

## Comparing `userfs-0.1.0.tar` & `userfs-0.2.0.tar`

### file list

```diff
@@ -1,28 +1,52 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 06:15:14.929886 userfs-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-05-04 06:14:13.000000 userfs-0.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2988 2023-05-04 06:15:14.929886 userfs-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2098 2023-05-04 06:14:13.000000 userfs-0.1.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1116 2023-05-04 06:14:13.000000 userfs-0.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-04 06:15:14.929886 userfs-0.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      820 2023-05-04 06:14:13.000000 userfs-0.1.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 06:15:14.929886 userfs-0.1.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      640 2023-05-04 06:14:13.000000 userfs-0.1.0/tests/test_entry.py
--rw-r--r--   0 runner    (1001) docker     (123)      268 2023-05-04 06:14:13.000000 userfs-0.1.0/tests/test_resources.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 06:15:14.929886 userfs-0.1.0/userfs/
--rw-r--r--   0 runner    (1001) docker     (123)      322 2023-05-04 06:14:13.000000 userfs-0.1.0/userfs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      326 2023-05-04 06:14:13.000000 userfs-0.1.0/userfs/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)      810 2023-05-04 06:14:13.000000 userfs-0.1.0/userfs/app.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 06:15:14.929886 userfs-0.1.0/userfs/commands/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 06:14:13.000000 userfs-0.1.0/userfs/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      398 2023-05-04 06:14:13.000000 userfs-0.1.0/userfs/commands/all.py
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-05-04 06:14:13.000000 userfs-0.1.0/userfs/dev_requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2004 2023-05-04 06:14:13.000000 userfs-0.1.0/userfs/entry.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 06:14:13.000000 userfs-0.1.0/userfs/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-04 06:14:13.000000 userfs-0.1.0/userfs/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 06:15:14.929886 userfs-0.1.0/userfs.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2988 2023-05-04 06:15:14.000000 userfs-0.1.0/userfs.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      454 2023-05-04 06:15:14.000000 userfs-0.1.0/userfs.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-04 06:15:14.000000 userfs-0.1.0/userfs.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-05-04 06:15:14.000000 userfs-0.1.0/userfs.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       98 2023-05-04 06:15:14.000000 userfs-0.1.0/userfs.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-04 06:15:14.000000 userfs-0.1.0/userfs.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 08:36:45.198417 userfs-0.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-05-05 08:35:34.000000 userfs-0.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3252 2023-05-05 08:36:45.198417 userfs-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2311 2023-05-05 08:35:34.000000 userfs-0.2.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1160 2023-05-05 08:35:34.000000 userfs-0.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-05 08:36:45.198417 userfs-0.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      836 2023-05-05 08:35:34.000000 userfs-0.2.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 08:36:45.194416 userfs-0.2.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      640 2023-05-05 08:35:34.000000 userfs-0.2.0/tests/test_entry.py
+-rw-r--r--   0 runner    (1001) docker     (123)      268 2023-05-05 08:35:34.000000 userfs-0.2.0/tests/test_resources.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 08:36:45.198417 userfs-0.2.0/userfs/
+-rw-r--r--   0 runner    (1001) docker     (123)      322 2023-05-05 08:35:34.000000 userfs-0.2.0/userfs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      326 2023-05-05 08:35:34.000000 userfs-0.2.0/userfs/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      967 2023-05-05 08:35:34.000000 userfs-0.2.0/userfs/app.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 08:36:45.198417 userfs-0.2.0/userfs/build/
+-rw-r--r--   0 runner    (1001) docker     (123)     1048 2023-05-05 08:35:34.000000 userfs-0.2.0/userfs/build/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 08:36:45.198417 userfs-0.2.0/userfs/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 08:35:34.000000 userfs-0.2.0/userfs/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      934 2023-05-05 08:35:34.000000 userfs-0.2.0/userfs/commands/all.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1085 2023-05-05 08:35:34.000000 userfs-0.2.0/userfs/commands/build.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1518 2023-05-05 08:35:34.000000 userfs-0.2.0/userfs/commands/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1026 2023-05-05 08:35:34.000000 userfs-0.2.0/userfs/commands/fetch.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 08:36:45.198417 userfs-0.2.0/userfs/config/
+-rw-r--r--   0 runner    (1001) docker     (123)     2773 2023-05-05 08:35:34.000000 userfs-0.2.0/userfs/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2243 2023-05-05 08:35:34.000000 userfs-0.2.0/userfs/config/project.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-05-05 08:35:34.000000 userfs-0.2.0/userfs/config/source.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 08:36:45.198417 userfs-0.2.0/userfs/data/
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-05-05 08:35:34.000000 userfs-0.2.0/userfs/data/config.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 08:36:45.198417 userfs-0.2.0/userfs/data/schemas/
+-rw-r--r--   0 runner    (1001) docker     (123)      453 2023-05-05 08:35:34.000000 userfs-0.2.0/userfs/data/schemas/Config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      776 2023-05-05 08:35:34.000000 userfs-0.2.0/userfs/data/schemas/ProjectSpecification.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      472 2023-05-05 08:35:34.000000 userfs-0.2.0/userfs/data/schemas/SourceSpecification.yaml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 08:36:45.198417 userfs-0.2.0/userfs/deploy/
+-rw-r--r--   0 runner    (1001) docker     (123)      364 2023-05-05 08:35:34.000000 userfs-0.2.0/userfs/deploy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-05-05 08:35:34.000000 userfs-0.2.0/userfs/dev_requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2004 2023-05-05 08:35:34.000000 userfs-0.2.0/userfs/entry.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 08:36:45.198417 userfs-0.2.0/userfs/fetch/
+-rw-r--r--   0 runner    (1001) docker     (123)      774 2023-05-05 08:35:34.000000 userfs-0.2.0/userfs/fetch/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 08:36:45.198417 userfs-0.2.0/userfs/project/
+-rw-r--r--   0 runner    (1001) docker     (123)     1910 2023-05-05 08:35:34.000000 userfs-0.2.0/userfs/project/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 08:35:34.000000 userfs-0.2.0/userfs/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-05-05 08:35:34.000000 userfs-0.2.0/userfs/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      583 2023-05-05 08:35:34.000000 userfs-0.2.0/userfs/schemas.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 08:36:45.198417 userfs-0.2.0/userfs/update/
+-rw-r--r--   0 runner    (1001) docker     (123)      558 2023-05-05 08:35:34.000000 userfs-0.2.0/userfs/update/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 08:36:45.198417 userfs-0.2.0/userfs.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3252 2023-05-05 08:36:45.000000 userfs-0.2.0/userfs.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      899 2023-05-05 08:36:45.000000 userfs-0.2.0/userfs.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 08:36:45.000000 userfs-0.2.0/userfs.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-05-05 08:36:45.000000 userfs-0.2.0/userfs.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-05-05 08:36:45.000000 userfs-0.2.0/userfs.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-05 08:36:45.000000 userfs-0.2.0/userfs.egg-info/top_level.txt
```

### Comparing `userfs-0.1.0/LICENSE` & `userfs-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `userfs-0.1.0/PKG-INFO` & `userfs-0.2.0/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 Metadata-Version: 2.1
 Name: userfs
-Version: 0.1.0
+Version: 0.2.0
 Summary: A system-bootstrapping automation and introspection tool.
 Home-page: https://github.com/vkottler/userfs
 Author: Vaughn Kottler
 Author-email: Vaughn Kottler <vaughnkottler@gmail.com>
 Maintainer-email: Vaughn Kottler <vaughnkottler@gmail.com>
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: MacOS
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Operating System :: Unix
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.7
@@ -21,19 +22,19 @@
 Provides-Extra: test
 License-File: LICENSE
 
 <!--
     =====================================
     generator=datazen
     version=3.1.2
-    hash=605284d3174ef737937a73768df6f028
+    hash=035acc9a20df17a172151cf57e984c39
     =====================================
 -->
 
-# userfs ([0.1.0](https://pypi.org/project/userfs/))
+# userfs ([0.2.0](https://pypi.org/project/userfs/))
 
 [![python](https://img.shields.io/pypi/pyversions/userfs.svg)](https://pypi.org/project/userfs/)
 ![Build Status](https://github.com/vkottler/userfs/workflows/Python%20Package/badge.svg)
 [![codecov](https://codecov.io/gh/vkottler/userfs/branch/master/graphs/badge.svg?branch=master)](https://codecov.io/github/vkottler/userfs)
 ![PyPI - Status](https://img.shields.io/pypi/status/userfs)
 ![Dependents (via libraries.io)](https://img.shields.io/librariesio/dependents/pypi/userfs)
 
@@ -46,14 +47,15 @@
 
 This package is tested with the following Python minor versions:
 
 * [`python3.7`](https://docs.python.org/3.7/)
 * [`python3.8`](https://docs.python.org/3.8/)
 * [`python3.9`](https://docs.python.org/3.9/)
 * [`python3.10`](https://docs.python.org/3.10/)
+* [`python3.11`](https://docs.python.org/3.11/)
 
 ## Platform Support
 
 This package is tested on the following platforms:
 
 * `ubuntu-latest`
 * `macos-latest`
@@ -62,27 +64,29 @@
 # Introduction
 
 # Command-line Options
 
 ```
 $ ./venv3.11/bin/ufs -h
 
-usage: ufs [-h] [--version] [-v] [-C DIR] {noop} ...
+usage: ufs [-h] [--version] [-v] [-C DIR] {build,fetch,noop} ...
 
 A system-bootstrapping automation and introspection tool.
 
 options:
-  -h, --help         show this help message and exit
-  --version          show program's version number and exit
-  -v, --verbose      set to increase logging verbosity
-  -C DIR, --dir DIR  execute from a specific directory
+  -h, --help          show this help message and exit
+  --version           show program's version number and exit
+  -v, --verbose       set to increase logging verbosity
+  -C DIR, --dir DIR   execute from a specific directory
 
 commands:
-  {noop}             set of available commands
-    noop             command stub (does nothing)
+  {build,fetch,noop}  set of available commands
+    build             attempt to build a software project from its sources
+    fetch             attempt to obtain some software from the internet
+    noop              command stub (does nothing)
 
 ```
 
 # Internal Dependency Graph
 
 A coarse view of the internal structure and scale of
 `userfs`'s source.
```

### Comparing `userfs-0.1.0/README.md` & `userfs-0.2.0/README.md`

 * *Files 25% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 <!--
     =====================================
     generator=datazen
     version=3.1.2
-    hash=605284d3174ef737937a73768df6f028
+    hash=035acc9a20df17a172151cf57e984c39
     =====================================
 -->
 
-# userfs ([0.1.0](https://pypi.org/project/userfs/))
+# userfs ([0.2.0](https://pypi.org/project/userfs/))
 
 [![python](https://img.shields.io/pypi/pyversions/userfs.svg)](https://pypi.org/project/userfs/)
 ![Build Status](https://github.com/vkottler/userfs/workflows/Python%20Package/badge.svg)
 [![codecov](https://codecov.io/gh/vkottler/userfs/branch/master/graphs/badge.svg?branch=master)](https://codecov.io/github/vkottler/userfs)
 ![PyPI - Status](https://img.shields.io/pypi/status/userfs)
 ![Dependents (via libraries.io)](https://img.shields.io/librariesio/dependents/pypi/userfs)
 
@@ -23,14 +23,15 @@
 
 This package is tested with the following Python minor versions:
 
 * [`python3.7`](https://docs.python.org/3.7/)
 * [`python3.8`](https://docs.python.org/3.8/)
 * [`python3.9`](https://docs.python.org/3.9/)
 * [`python3.10`](https://docs.python.org/3.10/)
+* [`python3.11`](https://docs.python.org/3.11/)
 
 ## Platform Support
 
 This package is tested on the following platforms:
 
 * `ubuntu-latest`
 * `macos-latest`
@@ -39,27 +40,29 @@
 # Introduction
 
 # Command-line Options
 
 ```
 $ ./venv3.11/bin/ufs -h
 
-usage: ufs [-h] [--version] [-v] [-C DIR] {noop} ...
+usage: ufs [-h] [--version] [-v] [-C DIR] {build,fetch,noop} ...
 
 A system-bootstrapping automation and introspection tool.
 
 options:
-  -h, --help         show this help message and exit
-  --version          show program's version number and exit
-  -v, --verbose      set to increase logging verbosity
-  -C DIR, --dir DIR  execute from a specific directory
+  -h, --help          show this help message and exit
+  --version           show program's version number and exit
+  -v, --verbose       set to increase logging verbosity
+  -C DIR, --dir DIR   execute from a specific directory
 
 commands:
-  {noop}             set of available commands
-    noop             command stub (does nothing)
+  {build,fetch,noop}  set of available commands
+    build             attempt to build a software project from its sources
+    fetch             attempt to obtain some software from the internet
+    noop              command stub (does nothing)
 
 ```
 
 # Internal Dependency Graph
 
 A coarse view of the internal structure and scale of
 `userfs`'s source.
```

### Comparing `userfs-0.1.0/pyproject.toml` & `userfs-0.2.0/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -1,28 +1,29 @@
 [build-system]
 requires = ["setuptools-wrapper", "trove-classifiers"]
 build-backend = "setuptools.build_meta:__legacy__"
 
 [project]
 name = "userfs"
-version = "0.1.0"
+version = "0.2.0"
 description = "A system-bootstrapping automation and introspection tool."
 readme = "README.md"
 requires-python = ">=3.7"
 authors = [
   {name = "Vaughn Kottler", email = "vaughnkottler@gmail.com"}
 ]
 maintainers = [
   {name = "Vaughn Kottler", email = "vaughnkottler@gmail.com"}
 ]
 classifiers = [
   "Programming Language :: Python :: 3.7",
   "Programming Language :: Python :: 3.8",
   "Programming Language :: Python :: 3.9",
   "Programming Language :: Python :: 3.10",
+  "Programming Language :: Python :: 3.11",
   "Operating System :: Microsoft :: Windows",
   "Operating System :: MacOS",
   "Operating System :: POSIX :: Linux",
   "Operating System :: Unix",
   "Development Status :: 5 - Production/Stable",
   "License :: OSI Approved :: MIT License"
 ]
```

### Comparing `userfs-0.1.0/setup.py` & `userfs-0.2.0/setup.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 # =====================================
 # generator=datazen
 # version=3.1.2
-# hash=5517809d127fa7fa4a57439c1f26b2ae
+# hash=adbd3386d75866f59abf0027f730de43
 # =====================================
 
 """
 userfs - Package definition for distribution.
 """
 
 # third-party
@@ -28,13 +28,14 @@
     "version": VERSION,
     "description": DESCRIPTION,
     "versions": [
         "3.7",
         "3.8",
         "3.9",
         "3.10",
+        "3.11",
     ],
 }
 setup(
     pkg_info,
     author_info,
 )
```

### Comparing `userfs-0.1.0/tests/test_entry.py` & `userfs-0.2.0/tests/test_entry.py`

 * *Files identical despite different names*

### Comparing `userfs-0.1.0/userfs/app.py` & `userfs-0.2.0/userfs/app.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,7 +1,13 @@
+# =====================================
+# generator=datazen
+# version=3.1.2
+# hash=6b8d7773adb61a955438889b00b5cf7c
+# =====================================
+
 """
 This package's command-line entry-point application.
 """
 
 # built-in
 from argparse import ArgumentParser as _ArgumentParser
 from argparse import Namespace as _Namespace
```

### Comparing `userfs-0.1.0/userfs/entry.py` & `userfs-0.2.0/userfs/entry.py`

 * *Files identical despite different names*

### Comparing `userfs-0.1.0/userfs.egg-info/PKG-INFO` & `userfs-0.2.0/userfs.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 Metadata-Version: 2.1
 Name: userfs
-Version: 0.1.0
+Version: 0.2.0
 Summary: A system-bootstrapping automation and introspection tool.
 Home-page: https://github.com/vkottler/userfs
 Author: Vaughn Kottler
 Author-email: Vaughn Kottler <vaughnkottler@gmail.com>
 Maintainer-email: Vaughn Kottler <vaughnkottler@gmail.com>
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: MacOS
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Operating System :: Unix
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: MIT License
 Requires-Python: >=3.7
@@ -21,19 +22,19 @@
 Provides-Extra: test
 License-File: LICENSE
 
 <!--
     =====================================
     generator=datazen
     version=3.1.2
-    hash=605284d3174ef737937a73768df6f028
+    hash=035acc9a20df17a172151cf57e984c39
     =====================================
 -->
 
-# userfs ([0.1.0](https://pypi.org/project/userfs/))
+# userfs ([0.2.0](https://pypi.org/project/userfs/))
 
 [![python](https://img.shields.io/pypi/pyversions/userfs.svg)](https://pypi.org/project/userfs/)
 ![Build Status](https://github.com/vkottler/userfs/workflows/Python%20Package/badge.svg)
 [![codecov](https://codecov.io/gh/vkottler/userfs/branch/master/graphs/badge.svg?branch=master)](https://codecov.io/github/vkottler/userfs)
 ![PyPI - Status](https://img.shields.io/pypi/status/userfs)
 ![Dependents (via libraries.io)](https://img.shields.io/librariesio/dependents/pypi/userfs)
 
@@ -46,14 +47,15 @@
 
 This package is tested with the following Python minor versions:
 
 * [`python3.7`](https://docs.python.org/3.7/)
 * [`python3.8`](https://docs.python.org/3.8/)
 * [`python3.9`](https://docs.python.org/3.9/)
 * [`python3.10`](https://docs.python.org/3.10/)
+* [`python3.11`](https://docs.python.org/3.11/)
 
 ## Platform Support
 
 This package is tested on the following platforms:
 
 * `ubuntu-latest`
 * `macos-latest`
@@ -62,27 +64,29 @@
 # Introduction
 
 # Command-line Options
 
 ```
 $ ./venv3.11/bin/ufs -h
 
-usage: ufs [-h] [--version] [-v] [-C DIR] {noop} ...
+usage: ufs [-h] [--version] [-v] [-C DIR] {build,fetch,noop} ...
 
 A system-bootstrapping automation and introspection tool.
 
 options:
-  -h, --help         show this help message and exit
-  --version          show program's version number and exit
-  -v, --verbose      set to increase logging verbosity
-  -C DIR, --dir DIR  execute from a specific directory
+  -h, --help          show this help message and exit
+  --version           show program's version number and exit
+  -v, --verbose       set to increase logging verbosity
+  -C DIR, --dir DIR   execute from a specific directory
 
 commands:
-  {noop}             set of available commands
-    noop             command stub (does nothing)
+  {build,fetch,noop}  set of available commands
+    build             attempt to build a software project from its sources
+    fetch             attempt to obtain some software from the internet
+    noop              command stub (does nothing)
 
 ```
 
 # Internal Dependency Graph
 
 A coarse view of the internal structure and scale of
 `userfs`'s source.
```

