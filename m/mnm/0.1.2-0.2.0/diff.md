# Comparing `tmp/mnm-0.1.2.tar.gz` & `tmp/mnm-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mnm-0.1.2.tar", last modified: Tue May  2 00:29:31 2023, max compression
+gzip compressed data, was "mnm-0.2.0.tar", last modified: Fri May  5 06:24:20 2023, max compression
```

## Comparing `mnm-0.1.2.tar` & `mnm-0.2.0.tar`

### file list

```diff
@@ -1,16 +1,25 @@
-drwxr-xr-x   0 ohk990102  (1000) ohk990102  (1000)        0 2023-05-02 00:29:31.962648 mnm-0.1.2/
--rw-r--r--   0 ohk990102  (1000) ohk990102  (1000)     1067 2023-05-01 04:28:16.000000 mnm-0.1.2/LICENSE
--rw-r--r--   0 ohk990102  (1000) ohk990102  (1000)      926 2023-05-02 00:29:31.962648 mnm-0.1.2/PKG-INFO
--rw-r--r--   0 ohk990102  (1000) ohk990102  (1000)      403 2023-05-01 12:59:53.000000 mnm-0.1.2/README.md
--rw-r--r--   0 ohk990102  (1000) ohk990102  (1000)      636 2023-05-02 00:29:28.000000 mnm-0.1.2/pyproject.toml
--rw-r--r--   0 ohk990102  (1000) ohk990102  (1000)       38 2023-05-02 00:29:31.962648 mnm-0.1.2/setup.cfg
-drwxr-xr-x   0 ohk990102  (1000) ohk990102  (1000)        0 2023-05-02 00:29:31.962648 mnm-0.1.2/src/
-drwxr-xr-x   0 ohk990102  (1000) ohk990102  (1000)        0 2023-05-02 00:29:31.962648 mnm-0.1.2/src/mnm/
--rw-r--r--   0 ohk990102  (1000) ohk990102  (1000)     4267 2023-05-02 00:26:30.000000 mnm-0.1.2/src/mnm/__init__.py
--rw-r--r--   0 ohk990102  (1000) ohk990102  (1000)      183 2023-05-01 13:05:36.000000 mnm-0.1.2/src/mnm/example.py
-drwxr-xr-x   0 ohk990102  (1000) ohk990102  (1000)        0 2023-05-02 00:29:31.962648 mnm-0.1.2/src/mnm.egg-info/
--rw-r--r--   0 ohk990102  (1000) ohk990102  (1000)      926 2023-05-02 00:29:31.000000 mnm-0.1.2/src/mnm.egg-info/PKG-INFO
--rw-r--r--   0 ohk990102  (1000) ohk990102  (1000)      225 2023-05-02 00:29:31.000000 mnm-0.1.2/src/mnm.egg-info/SOURCES.txt
--rw-r--r--   0 ohk990102  (1000) ohk990102  (1000)        1 2023-05-02 00:29:31.000000 mnm-0.1.2/src/mnm.egg-info/dependency_links.txt
--rw-r--r--   0 ohk990102  (1000) ohk990102  (1000)       29 2023-05-02 00:29:31.000000 mnm-0.1.2/src/mnm.egg-info/requires.txt
--rw-r--r--   0 ohk990102  (1000) ohk990102  (1000)        4 2023-05-02 00:29:31.000000 mnm-0.1.2/src/mnm.egg-info/top_level.txt
+drwxr-xr-x   0 ohk990102  (1000) ohk990102  (1000)        0 2023-05-05 06:24:20.509023 mnm-0.2.0/
+-rw-r--r--   0 ohk990102  (1000) ohk990102  (1000)     1067 2023-05-01 04:28:16.000000 mnm-0.2.0/LICENSE
+-rw-r--r--   0 ohk990102  (1000) ohk990102  (1000)      901 2023-05-05 06:24:20.499023 mnm-0.2.0/PKG-INFO
+-rw-r--r--   0 ohk990102  (1000) ohk990102  (1000)      403 2023-05-01 12:59:53.000000 mnm-0.2.0/README.md
+-rw-r--r--   0 ohk990102  (1000) ohk990102  (1000)      604 2023-05-05 06:20:10.000000 mnm-0.2.0/pyproject.toml
+-rw-r--r--   0 ohk990102  (1000) ohk990102  (1000)       38 2023-05-05 06:24:20.509023 mnm-0.2.0/setup.cfg
+drwxr-xr-x   0 ohk990102  (1000) ohk990102  (1000)        0 2023-05-05 06:24:20.499023 mnm-0.2.0/src/
+drwxr-xr-x   0 ohk990102  (1000) ohk990102  (1000)        0 2023-05-05 06:24:20.499023 mnm-0.2.0/src/mnm/
+-rw-r--r--   0 ohk990102  (1000) ohk990102  (1000)      256 2023-05-05 05:43:08.000000 mnm-0.2.0/src/mnm/__init__.py
+-rw-r--r--   0 ohk990102  (1000) ohk990102  (1000)      655 2023-05-05 05:37:33.000000 mnm-0.2.0/src/mnm/_internal_utils.py
+drwxr-xr-x   0 ohk990102  (1000) ohk990102  (1000)        0 2023-05-05 06:24:20.499023 mnm-0.2.0/src/mnm/examples/
+-rw-r--r--   0 ohk990102  (1000) ohk990102  (1000)      427 2023-05-05 06:14:01.000000 mnm-0.2.0/src/mnm/examples/mixed_options.py
+-rw-r--r--   0 ohk990102  (1000) ohk990102  (1000)      382 2023-05-05 06:13:22.000000 mnm-0.2.0/src/mnm/examples/mixed_simple.py
+-rw-r--r--   0 ohk990102  (1000) ohk990102  (1000)      445 2023-05-05 06:17:27.000000 mnm-0.2.0/src/mnm/examples/with_pattern.py
+-rw-r--r--   0 ohk990102  (1000) ohk990102  (1000)      723 2023-05-05 06:16:06.000000 mnm-0.2.0/src/mnm/global_functions.py
+-rw-r--r--   0 ohk990102  (1000) ohk990102  (1000)     1795 2023-05-05 06:16:10.000000 mnm-0.2.0/src/mnm/header_mocking.py
+-rw-r--r--   0 ohk990102  (1000) ohk990102  (1000)      638 2023-05-05 06:16:15.000000 mnm-0.2.0/src/mnm/mixed.py
+-rw-r--r--   0 ohk990102  (1000) ohk990102  (1000)     2074 2023-05-05 06:16:19.000000 mnm-0.2.0/src/mnm/socket_fragmentation.py
+-rw-r--r--   0 ohk990102  (1000) ohk990102  (1000)      353 2023-05-05 06:16:22.000000 mnm-0.2.0/src/mnm/wrapper.py
+drwxr-xr-x   0 ohk990102  (1000) ohk990102  (1000)        0 2023-05-05 06:24:20.499023 mnm-0.2.0/src/mnm.egg-info/
+-rw-r--r--   0 ohk990102  (1000) ohk990102  (1000)      901 2023-05-05 06:24:20.000000 mnm-0.2.0/src/mnm.egg-info/PKG-INFO
+-rw-r--r--   0 ohk990102  (1000) ohk990102  (1000)      455 2023-05-05 06:24:20.000000 mnm-0.2.0/src/mnm.egg-info/SOURCES.txt
+-rw-r--r--   0 ohk990102  (1000) ohk990102  (1000)        1 2023-05-05 06:24:20.000000 mnm-0.2.0/src/mnm.egg-info/dependency_links.txt
+-rw-r--r--   0 ohk990102  (1000) ohk990102  (1000)       17 2023-05-05 06:24:20.000000 mnm-0.2.0/src/mnm.egg-info/requires.txt
+-rw-r--r--   0 ohk990102  (1000) ohk990102  (1000)        4 2023-05-05 06:24:20.000000 mnm-0.2.0/src/mnm.egg-info/top_level.txt
```

### Comparing `mnm-0.1.2/LICENSE` & `mnm-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `mnm-0.1.2/PKG-INFO` & `mnm-0.2.0/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 Metadata-Version: 2.1
 Name: mnm
-Version: 0.1.2
+Version: 0.2.0
 Summary: A simple python library for pentesting firewall protected webapp
 Author-email: ohk990102 <ohk990102@gmail.com>
 Project-URL: Homepage, https://github.com/ohk990102/mnm
 Project-URL: Bug Tracker, https://github.com/ohk990102/mnm/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: POSIX :: Linux
 Description-Content-Type: text/markdown
-Provides-Extra: requests
 License-File: LICENSE
 
 # mnm
 
 This is a simple python library for pentesting firewall protected webapp.
 
 ## Installation
```

### Comparing `mnm-0.1.2/pyproject.toml` & `mnm-0.2.0/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "mnm"
-version = "0.1.2"
+version = "0.2.0"
 authors = [
   { name="ohk990102", email="ohk990102@gmail.com" },
 ]
 description = "A simple python library for pentesting firewall protected webapp"
 readme = "README.md"
 classifiers = [
-    "Programming Language :: Python :: 3",
-    "License :: OSI Approved :: MIT License",
-    "Operating System :: POSIX :: Linux",
+  "Programming Language :: Python :: 3",
+  "License :: OSI Approved :: MIT License",
+  "Operating System :: POSIX :: Linux",
+]
+dependencies = [
+  "requests>=2.26.0",
 ]
 
 [project.urls]
 "Homepage" = "https://github.com/ohk990102/mnm"
 "Bug Tracker" = "https://github.com/ohk990102/mnm/issues"
-
-[project.optional-dependencies]
-"requests" = ["requests>=2.26.0"]
```

### Comparing `mnm-0.1.2/src/mnm.egg-info/PKG-INFO` & `mnm-0.2.0/src/mnm.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,19 +1,18 @@
 Metadata-Version: 2.1
 Name: mnm
-Version: 0.1.2
+Version: 0.2.0
 Summary: A simple python library for pentesting firewall protected webapp
 Author-email: ohk990102 <ohk990102@gmail.com>
 Project-URL: Homepage, https://github.com/ohk990102/mnm
 Project-URL: Bug Tracker, https://github.com/ohk990102/mnm/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: POSIX :: Linux
 Description-Content-Type: text/markdown
-Provides-Extra: requests
 License-File: LICENSE
 
 # mnm
 
 This is a simple python library for pentesting firewall protected webapp.
 
 ## Installation
```

