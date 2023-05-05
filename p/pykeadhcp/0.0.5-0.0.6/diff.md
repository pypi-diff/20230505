# Comparing `tmp/pykeadhcp-0.0.5.tar.gz` & `tmp/pykeadhcp-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pykeadhcp-0.0.5.tar", last modified: Sun Mar 12 02:06:19 2023, max compression
+gzip compressed data, was "pykeadhcp-0.0.6.tar", last modified: Fri May  5 21:10:21 2023, max compression
```

## Comparing `pykeadhcp-0.0.5.tar` & `pykeadhcp-0.0.6.tar`

### file list

```diff
@@ -1,20 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-12 02:06:19.589863 pykeadhcp-0.0.5/
--rw-r--r--   0 runner    (1001) docker     (123)    11073 2023-03-12 02:06:19.589863 pykeadhcp-0.0.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    10734 2023-03-12 02:06:02.000000 pykeadhcp-0.0.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-12 02:06:19.585863 pykeadhcp-0.0.5/pykeadhcp/
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-03-12 02:06:02.000000 pykeadhcp-0.0.5/pykeadhcp/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-12 02:06:19.589863 pykeadhcp-0.0.5/pykeadhcp/daemons/
--rw-r--r--   0 runner    (1001) docker     (123)      174 2023-03-12 02:06:02.000000 pykeadhcp-0.0.5/pykeadhcp/daemons/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3860 2023-03-12 02:06:02.000000 pykeadhcp-0.0.5/pykeadhcp/daemons/ctrlagent.py
--rw-r--r--   0 runner    (1001) docker     (123)     3615 2023-03-12 02:06:02.000000 pykeadhcp-0.0.5/pykeadhcp/daemons/ddns.py
--rw-r--r--   0 runner    (1001) docker     (123)    19979 2023-03-12 02:06:02.000000 pykeadhcp-0.0.5/pykeadhcp/daemons/dhcp4.py
--rw-r--r--   0 runner    (1001) docker     (123)     3617 2023-03-12 02:06:02.000000 pykeadhcp-0.0.5/pykeadhcp/daemons/dhcp6.py
--rw-r--r--   0 runner    (1001) docker     (123)     3007 2023-03-12 02:06:02.000000 pykeadhcp-0.0.5/pykeadhcp/kea.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-12 02:06:19.585863 pykeadhcp-0.0.5/pykeadhcp.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    11073 2023-03-12 02:06:19.000000 pykeadhcp-0.0.5/pykeadhcp.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      362 2023-03-12 02:06:19.000000 pykeadhcp-0.0.5/pykeadhcp.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-12 02:06:19.000000 pykeadhcp-0.0.5/pykeadhcp.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-03-12 02:06:19.000000 pykeadhcp-0.0.5/pykeadhcp.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-03-12 02:06:19.000000 pykeadhcp-0.0.5/pykeadhcp.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-12 02:06:19.589863 pykeadhcp-0.0.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      571 2023-03-12 02:06:02.000000 pykeadhcp-0.0.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 21:10:21.774371 pykeadhcp-0.0.6/
+-rw-r--r--   0 runner    (1001) docker     (123)    11356 2023-05-05 21:10:08.000000 pykeadhcp-0.0.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    11095 2023-05-05 21:10:21.774371 pykeadhcp-0.0.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    10734 2023-05-05 21:10:08.000000 pykeadhcp-0.0.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 21:10:21.774371 pykeadhcp-0.0.6/pykeadhcp/
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-05-05 21:10:08.000000 pykeadhcp-0.0.6/pykeadhcp/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 21:10:21.774371 pykeadhcp-0.0.6/pykeadhcp/daemons/
+-rw-r--r--   0 runner    (1001) docker     (123)      174 2023-05-05 21:10:08.000000 pykeadhcp-0.0.6/pykeadhcp/daemons/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3860 2023-05-05 21:10:08.000000 pykeadhcp-0.0.6/pykeadhcp/daemons/ctrlagent.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3615 2023-05-05 21:10:08.000000 pykeadhcp-0.0.6/pykeadhcp/daemons/ddns.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19979 2023-05-05 21:10:08.000000 pykeadhcp-0.0.6/pykeadhcp/daemons/dhcp4.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3617 2023-05-05 21:10:08.000000 pykeadhcp-0.0.6/pykeadhcp/daemons/dhcp6.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3007 2023-05-05 21:10:08.000000 pykeadhcp-0.0.6/pykeadhcp/kea.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 21:10:21.774371 pykeadhcp-0.0.6/pykeadhcp.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    11095 2023-05-05 21:10:21.000000 pykeadhcp-0.0.6/pykeadhcp.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      370 2023-05-05 21:10:21.000000 pykeadhcp-0.0.6/pykeadhcp.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 21:10:21.000000 pykeadhcp-0.0.6/pykeadhcp.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-05-05 21:10:21.000000 pykeadhcp-0.0.6/pykeadhcp.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-05 21:10:21.000000 pykeadhcp-0.0.6/pykeadhcp.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-05 21:10:21.774371 pykeadhcp-0.0.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      571 2023-05-05 21:10:08.000000 pykeadhcp-0.0.6/setup.py
```

### Comparing `pykeadhcp-0.0.5/PKG-INFO` & `pykeadhcp-0.0.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 Metadata-Version: 2.1
 Name: pykeadhcp
-Version: 0.0.5
+Version: 0.0.6
 Summary: Wrapper around requests module to query ISC Kea DHCP API Daemons (ctrlagent, dhcp4, dhcp6, ddns)
 Home-page: https://github.com/BSpendlove/pykeadhcp
 Author: Brandon Spendlove
 Author-email: brandonspendlove@gmail.com
 Description-Content-Type: text/markdown
 Provides-Extra: dev
+License-File: LICENSE
 
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 
 # pykeadhcp
 A python module used to interact the the Kea DHCP API daemons (dhcp4, dhcp6, ctrl-agent and ddns)
 
 ## How to use
```

### Comparing `pykeadhcp-0.0.5/README.md` & `pykeadhcp-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `pykeadhcp-0.0.5/pykeadhcp/daemons/ctrlagent.py` & `pykeadhcp-0.0.6/pykeadhcp/daemons/ctrlagent.py`

 * *Files identical despite different names*

### Comparing `pykeadhcp-0.0.5/pykeadhcp/daemons/ddns.py` & `pykeadhcp-0.0.6/pykeadhcp/daemons/ddns.py`

 * *Files identical despite different names*

### Comparing `pykeadhcp-0.0.5/pykeadhcp/daemons/dhcp4.py` & `pykeadhcp-0.0.6/pykeadhcp/daemons/dhcp4.py`

 * *Files identical despite different names*

### Comparing `pykeadhcp-0.0.5/pykeadhcp/daemons/dhcp6.py` & `pykeadhcp-0.0.6/pykeadhcp/daemons/dhcp6.py`

 * *Files identical despite different names*

### Comparing `pykeadhcp-0.0.5/pykeadhcp/kea.py` & `pykeadhcp-0.0.6/pykeadhcp/kea.py`

 * *Files identical despite different names*

### Comparing `pykeadhcp-0.0.5/pykeadhcp.egg-info/PKG-INFO` & `pykeadhcp-0.0.6/pykeadhcp.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 Metadata-Version: 2.1
 Name: pykeadhcp
-Version: 0.0.5
+Version: 0.0.6
 Summary: Wrapper around requests module to query ISC Kea DHCP API Daemons (ctrlagent, dhcp4, dhcp6, ddns)
 Home-page: https://github.com/BSpendlove/pykeadhcp
 Author: Brandon Spendlove
 Author-email: brandonspendlove@gmail.com
 Description-Content-Type: text/markdown
 Provides-Extra: dev
+License-File: LICENSE
 
 [![Code style: black](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
 
 # pykeadhcp
 A python module used to interact the the Kea DHCP API daemons (dhcp4, dhcp6, ctrl-agent and ddns)
 
 ## How to use
```

### Comparing `pykeadhcp-0.0.5/setup.py` & `pykeadhcp-0.0.6/setup.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="pykeadhcp",
-    version="0.0.5",
+    version="0.0.6",
     description="Wrapper around requests module to query ISC Kea DHCP API Daemons (ctrlagent, dhcp4, dhcp6, ddns)",
     long_description=open("README.md").read(),
     long_description_content_type="text/markdown",
     url="https://github.com/BSpendlove/pykeadhcp",
     author="Brandon Spendlove",
     author_email="brandonspendlove@gmail.com",
     install_requires=["requests>=2.28.2"],
```

