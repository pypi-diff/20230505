# Comparing `tmp/pulumi_venafi-1.6.0a1682380572.tar.gz` & `tmp/pulumi_venafi-1.6.0a1683269248.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pulumi_venafi-1.6.0a1682380572.tar", last modified: Tue Apr 25 00:00:13 2023, max compression
+gzip compressed data, was "pulumi_venafi-1.6.0a1683269248.tar", last modified: Fri May  5 06:53:16 2023, max compression
```

## Comparing `pulumi_venafi-1.6.0a1682380572.tar` & `pulumi_venafi-1.6.0a1683269248.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 00:00:13.850467 pulumi_venafi-1.6.0a1682380572/
--rw-r--r--   0 runner    (1001) docker     (123)     3498 2023-04-25 00:00:13.850467 pulumi_venafi-1.6.0a1682380572/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3155 2023-04-25 00:00:13.000000 pulumi_venafi-1.6.0a1682380572/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 00:00:13.850467 pulumi_venafi-1.6.0a1682380572/pulumi_venafi/
--rw-r--r--   0 runner    (1001) docker     (123)     1404 2023-04-25 00:00:13.000000 pulumi_venafi-1.6.0a1682380572/pulumi_venafi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8081 2023-04-25 00:00:13.000000 pulumi_venafi-1.6.0a1682380572/pulumi_venafi/_utilities.py
--rw-r--r--   0 runner    (1001) docker     (123)    47556 2023-04-25 00:00:13.000000 pulumi_venafi-1.6.0a1682380572/pulumi_venafi/certificate.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 00:00:13.850467 pulumi_venafi-1.6.0a1682380572/pulumi_venafi/config/
--rw-r--r--   0 runner    (1001) docker     (123)      285 2023-04-25 00:00:13.000000 pulumi_venafi-1.6.0a1682380572/pulumi_venafi/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2377 2023-04-25 00:00:13.000000 pulumi_venafi-1.6.0a1682380572/pulumi_venafi/config/vars.py
--rw-r--r--   0 runner    (1001) docker     (123)    11703 2023-04-25 00:00:13.000000 pulumi_venafi-1.6.0a1682380572/pulumi_venafi/policy.py
--rw-r--r--   0 runner    (1001) docker     (123)    14951 2023-04-25 00:00:13.000000 pulumi_venafi-1.6.0a1682380572/pulumi_venafi/provider.py
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-04-25 00:00:13.000000 pulumi_venafi-1.6.0a1682380572/pulumi_venafi/pulumi-plugin.json
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-25 00:00:13.000000 pulumi_venafi-1.6.0a1682380572/pulumi_venafi/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    53209 2023-04-25 00:00:13.000000 pulumi_venafi-1.6.0a1682380572/pulumi_venafi/ssh_certificate.py
--rw-r--r--   0 runner    (1001) docker     (123)     8506 2023-04-25 00:00:13.000000 pulumi_venafi-1.6.0a1682380572/pulumi_venafi/ssh_config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-25 00:00:13.850467 pulumi_venafi-1.6.0a1682380572/pulumi_venafi.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3498 2023-04-25 00:00:13.000000 pulumi_venafi-1.6.0a1682380572/pulumi_venafi.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      550 2023-04-25 00:00:13.000000 pulumi_venafi-1.6.0a1682380572/pulumi_venafi.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-25 00:00:13.000000 pulumi_venafi-1.6.0a1682380572/pulumi_venafi.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-25 00:00:13.000000 pulumi_venafi-1.6.0a1682380572/pulumi_venafi.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-04-25 00:00:13.000000 pulumi_venafi-1.6.0a1682380572/pulumi_venafi.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-04-25 00:00:13.000000 pulumi_venafi-1.6.0a1682380572/pulumi_venafi.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-25 00:00:13.850467 pulumi_venafi-1.6.0a1682380572/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2124 2023-04-25 00:00:13.000000 pulumi_venafi-1.6.0a1682380572/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 06:53:16.568911 pulumi_venafi-1.6.0a1683269248/
+-rw-r--r--   0 runner    (1001) docker     (123)     3498 2023-05-05 06:53:16.568911 pulumi_venafi-1.6.0a1683269248/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3155 2023-05-05 06:53:16.000000 pulumi_venafi-1.6.0a1683269248/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 06:53:16.568911 pulumi_venafi-1.6.0a1683269248/pulumi_venafi/
+-rw-r--r--   0 runner    (1001) docker     (123)     1404 2023-05-05 06:53:16.000000 pulumi_venafi-1.6.0a1683269248/pulumi_venafi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8081 2023-05-05 06:53:16.000000 pulumi_venafi-1.6.0a1683269248/pulumi_venafi/_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (123)    47556 2023-05-05 06:53:16.000000 pulumi_venafi-1.6.0a1683269248/pulumi_venafi/certificate.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 06:53:16.568911 pulumi_venafi-1.6.0a1683269248/pulumi_venafi/config/
+-rw-r--r--   0 runner    (1001) docker     (123)      285 2023-05-05 06:53:16.000000 pulumi_venafi-1.6.0a1683269248/pulumi_venafi/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2377 2023-05-05 06:53:16.000000 pulumi_venafi-1.6.0a1683269248/pulumi_venafi/config/vars.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11703 2023-05-05 06:53:16.000000 pulumi_venafi-1.6.0a1683269248/pulumi_venafi/policy.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14951 2023-05-05 06:53:16.000000 pulumi_venafi-1.6.0a1683269248/pulumi_venafi/provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-05-05 06:53:16.000000 pulumi_venafi-1.6.0a1683269248/pulumi_venafi/pulumi-plugin.json
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 06:53:16.000000 pulumi_venafi-1.6.0a1683269248/pulumi_venafi/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    53209 2023-05-05 06:53:16.000000 pulumi_venafi-1.6.0a1683269248/pulumi_venafi/ssh_certificate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8506 2023-05-05 06:53:16.000000 pulumi_venafi-1.6.0a1683269248/pulumi_venafi/ssh_config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 06:53:16.568911 pulumi_venafi-1.6.0a1683269248/pulumi_venafi.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3498 2023-05-05 06:53:16.000000 pulumi_venafi-1.6.0a1683269248/pulumi_venafi.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      550 2023-05-05 06:53:16.000000 pulumi_venafi-1.6.0a1683269248/pulumi_venafi.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 06:53:16.000000 pulumi_venafi-1.6.0a1683269248/pulumi_venafi.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 06:53:16.000000 pulumi_venafi-1.6.0a1683269248/pulumi_venafi.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-05-05 06:53:16.000000 pulumi_venafi-1.6.0a1683269248/pulumi_venafi.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-05 06:53:16.000000 pulumi_venafi-1.6.0a1683269248/pulumi_venafi.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-05 06:53:16.568911 pulumi_venafi-1.6.0a1683269248/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2124 2023-05-05 06:53:16.000000 pulumi_venafi-1.6.0a1683269248/setup.py
```

### Comparing `pulumi_venafi-1.6.0a1682380572/PKG-INFO` & `pulumi_venafi-1.6.0a1683269248/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi_venafi
-Version: 1.6.0a1682380572
+Version: 1.6.0a1683269248
 Summary: A Pulumi package for creating and managing venafi cloud resources.
 Home-page: https://pulumi.io
 License: Apache-2.0
 Project-URL: Repository, https://github.com/pulumi/pulumi-venafi
 Keywords: pulumi venafi
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `pulumi_venafi-1.6.0a1682380572/README.md` & `pulumi_venafi-1.6.0a1683269248/README.md`

 * *Files identical despite different names*

### Comparing `pulumi_venafi-1.6.0a1682380572/pulumi_venafi/__init__.py` & `pulumi_venafi-1.6.0a1683269248/pulumi_venafi/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_venafi-1.6.0a1682380572/pulumi_venafi/_utilities.py` & `pulumi_venafi-1.6.0a1683269248/pulumi_venafi/_utilities.py`

 * *Files identical despite different names*

### Comparing `pulumi_venafi-1.6.0a1682380572/pulumi_venafi/certificate.py` & `pulumi_venafi-1.6.0a1683269248/pulumi_venafi/certificate.py`

 * *Files identical despite different names*

### Comparing `pulumi_venafi-1.6.0a1682380572/pulumi_venafi/config/vars.py` & `pulumi_venafi-1.6.0a1683269248/pulumi_venafi/config/vars.py`

 * *Files identical despite different names*

### Comparing `pulumi_venafi-1.6.0a1682380572/pulumi_venafi/policy.py` & `pulumi_venafi-1.6.0a1683269248/pulumi_venafi/policy.py`

 * *Files identical despite different names*

### Comparing `pulumi_venafi-1.6.0a1682380572/pulumi_venafi/provider.py` & `pulumi_venafi-1.6.0a1683269248/pulumi_venafi/provider.py`

 * *Files identical despite different names*

### Comparing `pulumi_venafi-1.6.0a1682380572/pulumi_venafi/ssh_certificate.py` & `pulumi_venafi-1.6.0a1683269248/pulumi_venafi/ssh_certificate.py`

 * *Files identical despite different names*

### Comparing `pulumi_venafi-1.6.0a1682380572/pulumi_venafi/ssh_config.py` & `pulumi_venafi-1.6.0a1683269248/pulumi_venafi/ssh_config.py`

 * *Files identical despite different names*

### Comparing `pulumi_venafi-1.6.0a1682380572/pulumi_venafi.egg-info/PKG-INFO` & `pulumi_venafi-1.6.0a1683269248/pulumi_venafi.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi-venafi
-Version: 1.6.0a1682380572
+Version: 1.6.0a1683269248
 Summary: A Pulumi package for creating and managing venafi cloud resources.
 Home-page: https://pulumi.io
 License: Apache-2.0
 Project-URL: Repository, https://github.com/pulumi/pulumi-venafi
 Keywords: pulumi venafi
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `pulumi_venafi-1.6.0a1682380572/pulumi_venafi.egg-info/SOURCES.txt` & `pulumi_venafi-1.6.0a1683269248/pulumi_venafi.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pulumi_venafi-1.6.0a1682380572/setup.py` & `pulumi_venafi-1.6.0a1683269248/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,16 +4,16 @@
 
 import errno
 from setuptools import setup, find_packages
 from setuptools.command.install import install
 from subprocess import check_call
 
 
-VERSION = "1.6.0a1682380572"
-PLUGIN_VERSION = "1.6.0-alpha.1682380572+d9ad7543"
+VERSION = "1.6.0a1683269248"
+PLUGIN_VERSION = "1.6.0-alpha.1683269248+78561332"
 
 class InstallPluginCommand(install):
     def run(self):
         install.run(self)
         try:
             check_call(['pulumi', 'plugin', 'install', 'resource', 'venafi', PLUGIN_VERSION])
         except OSError as error:
```

