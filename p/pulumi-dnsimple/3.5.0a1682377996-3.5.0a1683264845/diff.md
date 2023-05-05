# Comparing `tmp/pulumi_dnsimple-3.5.0a1682377996.tar.gz` & `tmp/pulumi_dnsimple-3.5.0a1683264845.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pulumi_dnsimple-3.5.0a1682377996.tar", last modified: Mon Apr 24 23:23:12 2023, max compression
+gzip compressed data, was "pulumi_dnsimple-3.5.0a1683264845.tar", last modified: Fri May  5 05:42:09 2023, max compression
```

## Comparing `pulumi_dnsimple-3.5.0a1682377996.tar` & `pulumi_dnsimple-3.5.0a1683264845.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 23:23:12.115560 pulumi_dnsimple-3.5.0a1682377996/
--rw-r--r--   0 runner    (1001) docker     (123)     2753 2023-04-24 23:23:12.115560 pulumi_dnsimple-3.5.0a1682377996/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2402 2023-04-24 23:23:11.000000 pulumi_dnsimple-3.5.0a1682377996/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 23:23:12.111560 pulumi_dnsimple-3.5.0a1682377996/pulumi_dnsimple/
--rw-r--r--   0 runner    (1001) docker     (123)     1711 2023-04-24 23:23:11.000000 pulumi_dnsimple-3.5.0a1682377996/pulumi_dnsimple/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8081 2023-04-24 23:23:11.000000 pulumi_dnsimple-3.5.0a1682377996/pulumi_dnsimple/_utilities.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 23:23:12.111560 pulumi_dnsimple-3.5.0a1682377996/pulumi_dnsimple/config/
--rw-r--r--   0 runner    (1001) docker     (123)      285 2023-04-24 23:23:11.000000 pulumi_dnsimple-3.5.0a1682377996/pulumi_dnsimple/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1329 2023-04-24 23:23:11.000000 pulumi_dnsimple-3.5.0a1682377996/pulumi_dnsimple/config/vars.py
--rw-r--r--   0 runner    (1001) docker     (123)     9408 2023-04-24 23:23:11.000000 pulumi_dnsimple-3.5.0a1682377996/pulumi_dnsimple/domain.py
--rw-r--r--   0 runner    (1001) docker     (123)     8785 2023-04-24 23:23:11.000000 pulumi_dnsimple-3.5.0a1682377996/pulumi_dnsimple/email_forward.py
--rw-r--r--   0 runner    (1001) docker     (123)     5082 2023-04-24 23:23:11.000000 pulumi_dnsimple-3.5.0a1682377996/pulumi_dnsimple/get_certificate.py
--rw-r--r--   0 runner    (1001) docker     (123)     2976 2023-04-24 23:23:11.000000 pulumi_dnsimple-3.5.0a1682377996/pulumi_dnsimple/get_zone.py
--rw-r--r--   0 runner    (1001) docker     (123)    15442 2023-04-24 23:23:11.000000 pulumi_dnsimple-3.5.0a1682377996/pulumi_dnsimple/lets_encrypt_certificate.py
--rw-r--r--   0 runner    (1001) docker     (123)     8730 2023-04-24 23:23:11.000000 pulumi_dnsimple-3.5.0a1682377996/pulumi_dnsimple/provider.py
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-04-24 23:23:11.000000 pulumi_dnsimple-3.5.0a1682377996/pulumi_dnsimple/pulumi-plugin.json
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-24 23:23:11.000000 pulumi_dnsimple-3.5.0a1682377996/pulumi_dnsimple/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    12185 2023-04-24 23:23:11.000000 pulumi_dnsimple-3.5.0a1682377996/pulumi_dnsimple/record.py
--rw-r--r--   0 runner    (1001) docker     (123)    12508 2023-04-24 23:23:11.000000 pulumi_dnsimple-3.5.0a1682377996/pulumi_dnsimple/zone_record.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-24 23:23:12.111560 pulumi_dnsimple-3.5.0a1682377996/pulumi_dnsimple.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2753 2023-04-24 23:23:12.000000 pulumi_dnsimple-3.5.0a1682377996/pulumi_dnsimple.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      685 2023-04-24 23:23:12.000000 pulumi_dnsimple-3.5.0a1682377996/pulumi_dnsimple.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-24 23:23:12.000000 pulumi_dnsimple-3.5.0a1682377996/pulumi_dnsimple.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-24 23:23:12.000000 pulumi_dnsimple-3.5.0a1682377996/pulumi_dnsimple.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-04-24 23:23:12.000000 pulumi_dnsimple-3.5.0a1682377996/pulumi_dnsimple.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-04-24 23:23:12.000000 pulumi_dnsimple-3.5.0a1682377996/pulumi_dnsimple.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-24 23:23:12.115560 pulumi_dnsimple-3.5.0a1682377996/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2142 2023-04-24 23:23:11.000000 pulumi_dnsimple-3.5.0a1682377996/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 05:42:09.566138 pulumi_dnsimple-3.5.0a1683264845/
+-rw-r--r--   0 runner    (1001) docker     (123)     2753 2023-05-05 05:42:09.566138 pulumi_dnsimple-3.5.0a1683264845/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2402 2023-05-05 05:42:09.000000 pulumi_dnsimple-3.5.0a1683264845/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 05:42:09.566138 pulumi_dnsimple-3.5.0a1683264845/pulumi_dnsimple/
+-rw-r--r--   0 runner    (1001) docker     (123)     1711 2023-05-05 05:42:09.000000 pulumi_dnsimple-3.5.0a1683264845/pulumi_dnsimple/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8081 2023-05-05 05:42:09.000000 pulumi_dnsimple-3.5.0a1683264845/pulumi_dnsimple/_utilities.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 05:42:09.566138 pulumi_dnsimple-3.5.0a1683264845/pulumi_dnsimple/config/
+-rw-r--r--   0 runner    (1001) docker     (123)      285 2023-05-05 05:42:09.000000 pulumi_dnsimple-3.5.0a1683264845/pulumi_dnsimple/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1329 2023-05-05 05:42:09.000000 pulumi_dnsimple-3.5.0a1683264845/pulumi_dnsimple/config/vars.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9408 2023-05-05 05:42:09.000000 pulumi_dnsimple-3.5.0a1683264845/pulumi_dnsimple/domain.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8785 2023-05-05 05:42:09.000000 pulumi_dnsimple-3.5.0a1683264845/pulumi_dnsimple/email_forward.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5082 2023-05-05 05:42:09.000000 pulumi_dnsimple-3.5.0a1683264845/pulumi_dnsimple/get_certificate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2976 2023-05-05 05:42:09.000000 pulumi_dnsimple-3.5.0a1683264845/pulumi_dnsimple/get_zone.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15442 2023-05-05 05:42:09.000000 pulumi_dnsimple-3.5.0a1683264845/pulumi_dnsimple/lets_encrypt_certificate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8730 2023-05-05 05:42:09.000000 pulumi_dnsimple-3.5.0a1683264845/pulumi_dnsimple/provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-05-05 05:42:09.000000 pulumi_dnsimple-3.5.0a1683264845/pulumi_dnsimple/pulumi-plugin.json
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 05:42:09.000000 pulumi_dnsimple-3.5.0a1683264845/pulumi_dnsimple/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    12185 2023-05-05 05:42:09.000000 pulumi_dnsimple-3.5.0a1683264845/pulumi_dnsimple/record.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12508 2023-05-05 05:42:09.000000 pulumi_dnsimple-3.5.0a1683264845/pulumi_dnsimple/zone_record.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 05:42:09.566138 pulumi_dnsimple-3.5.0a1683264845/pulumi_dnsimple.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2753 2023-05-05 05:42:09.000000 pulumi_dnsimple-3.5.0a1683264845/pulumi_dnsimple.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      685 2023-05-05 05:42:09.000000 pulumi_dnsimple-3.5.0a1683264845/pulumi_dnsimple.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 05:42:09.000000 pulumi_dnsimple-3.5.0a1683264845/pulumi_dnsimple.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 05:42:09.000000 pulumi_dnsimple-3.5.0a1683264845/pulumi_dnsimple.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-05-05 05:42:09.000000 pulumi_dnsimple-3.5.0a1683264845/pulumi_dnsimple.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-05 05:42:09.000000 pulumi_dnsimple-3.5.0a1683264845/pulumi_dnsimple.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-05 05:42:09.566138 pulumi_dnsimple-3.5.0a1683264845/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2142 2023-05-05 05:42:09.000000 pulumi_dnsimple-3.5.0a1683264845/setup.py
```

### Comparing `pulumi_dnsimple-3.5.0a1682377996/PKG-INFO` & `pulumi_dnsimple-3.5.0a1683264845/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi_dnsimple
-Version: 3.5.0a1682377996
+Version: 3.5.0a1683264845
 Summary: A Pulumi package for creating and managing dnsimple cloud resources.
 Home-page: https://pulumi.io
 License: Apache-2.0
 Project-URL: Repository, https://github.com/pulumi/pulumi-dnsimple
 Keywords: pulumi dnsimple
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `pulumi_dnsimple-3.5.0a1682377996/README.md` & `pulumi_dnsimple-3.5.0a1683264845/README.md`

 * *Files identical despite different names*

### Comparing `pulumi_dnsimple-3.5.0a1682377996/pulumi_dnsimple/__init__.py` & `pulumi_dnsimple-3.5.0a1683264845/pulumi_dnsimple/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_dnsimple-3.5.0a1682377996/pulumi_dnsimple/_utilities.py` & `pulumi_dnsimple-3.5.0a1683264845/pulumi_dnsimple/_utilities.py`

 * *Files identical despite different names*

### Comparing `pulumi_dnsimple-3.5.0a1682377996/pulumi_dnsimple/config/vars.py` & `pulumi_dnsimple-3.5.0a1683264845/pulumi_dnsimple/config/vars.py`

 * *Files identical despite different names*

### Comparing `pulumi_dnsimple-3.5.0a1682377996/pulumi_dnsimple/domain.py` & `pulumi_dnsimple-3.5.0a1683264845/pulumi_dnsimple/domain.py`

 * *Files identical despite different names*

### Comparing `pulumi_dnsimple-3.5.0a1682377996/pulumi_dnsimple/email_forward.py` & `pulumi_dnsimple-3.5.0a1683264845/pulumi_dnsimple/email_forward.py`

 * *Files identical despite different names*

### Comparing `pulumi_dnsimple-3.5.0a1682377996/pulumi_dnsimple/get_certificate.py` & `pulumi_dnsimple-3.5.0a1683264845/pulumi_dnsimple/get_certificate.py`

 * *Files identical despite different names*

### Comparing `pulumi_dnsimple-3.5.0a1682377996/pulumi_dnsimple/get_zone.py` & `pulumi_dnsimple-3.5.0a1683264845/pulumi_dnsimple/get_zone.py`

 * *Files identical despite different names*

### Comparing `pulumi_dnsimple-3.5.0a1682377996/pulumi_dnsimple/lets_encrypt_certificate.py` & `pulumi_dnsimple-3.5.0a1683264845/pulumi_dnsimple/lets_encrypt_certificate.py`

 * *Files identical despite different names*

### Comparing `pulumi_dnsimple-3.5.0a1682377996/pulumi_dnsimple/provider.py` & `pulumi_dnsimple-3.5.0a1683264845/pulumi_dnsimple/provider.py`

 * *Files identical despite different names*

### Comparing `pulumi_dnsimple-3.5.0a1682377996/pulumi_dnsimple/record.py` & `pulumi_dnsimple-3.5.0a1683264845/pulumi_dnsimple/record.py`

 * *Files identical despite different names*

### Comparing `pulumi_dnsimple-3.5.0a1682377996/pulumi_dnsimple/zone_record.py` & `pulumi_dnsimple-3.5.0a1683264845/pulumi_dnsimple/zone_record.py`

 * *Files identical despite different names*

### Comparing `pulumi_dnsimple-3.5.0a1682377996/pulumi_dnsimple.egg-info/PKG-INFO` & `pulumi_dnsimple-3.5.0a1683264845/pulumi_dnsimple.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi-dnsimple
-Version: 3.5.0a1682377996
+Version: 3.5.0a1683264845
 Summary: A Pulumi package for creating and managing dnsimple cloud resources.
 Home-page: https://pulumi.io
 License: Apache-2.0
 Project-URL: Repository, https://github.com/pulumi/pulumi-dnsimple
 Keywords: pulumi dnsimple
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `pulumi_dnsimple-3.5.0a1682377996/pulumi_dnsimple.egg-info/SOURCES.txt` & `pulumi_dnsimple-3.5.0a1683264845/pulumi_dnsimple.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pulumi_dnsimple-3.5.0a1682377996/setup.py` & `pulumi_dnsimple-3.5.0a1683264845/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -4,16 +4,16 @@
 
 import errno
 from setuptools import setup, find_packages
 from setuptools.command.install import install
 from subprocess import check_call
 
 
-VERSION = "3.5.0a1682377996"
-PLUGIN_VERSION = "3.5.0-alpha.1682377996+723983f9"
+VERSION = "3.5.0a1683264845"
+PLUGIN_VERSION = "3.5.0-alpha.1683264845+88e43f70"
 
 class InstallPluginCommand(install):
     def run(self):
         install.run(self)
         try:
             check_call(['pulumi', 'plugin', 'install', 'resource', 'dnsimple', PLUGIN_VERSION])
         except OSError as error:
```

