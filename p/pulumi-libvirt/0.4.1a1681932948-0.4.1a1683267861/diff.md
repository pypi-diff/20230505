# Comparing `tmp/pulumi_libvirt-0.4.1a1681932948.tar.gz` & `tmp/pulumi_libvirt-0.4.1a1683267861.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pulumi_libvirt-0.4.1a1681932948.tar", last modified: Wed Apr 19 19:51:09 2023, max compression
+gzip compressed data, was "pulumi_libvirt-0.4.1a1683267861.tar", last modified: Fri May  5 06:54:10 2023, max compression
```

## Comparing `pulumi_libvirt-0.4.1a1681932948.tar` & `pulumi_libvirt-0.4.1a1683267861.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 19:51:09.016923 pulumi_libvirt-0.4.1a1681932948/
--rw-r--r--   0 runner    (1001) docker     (123)     2396 2023-04-19 19:51:09.016923 pulumi_libvirt-0.4.1a1681932948/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2049 2023-04-19 19:51:08.000000 pulumi_libvirt-0.4.1a1681932948/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 19:51:09.016923 pulumi_libvirt-0.4.1a1681932948/pulumi_libvirt/
--rw-r--r--   0 runner    (1001) docker     (123)     1893 2023-04-19 19:51:08.000000 pulumi_libvirt-0.4.1a1681932948/pulumi_libvirt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    45336 2023-04-19 19:51:08.000000 pulumi_libvirt-0.4.1a1681932948/pulumi_libvirt/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (123)     8081 2023-04-19 19:51:08.000000 pulumi_libvirt-0.4.1a1681932948/pulumi_libvirt/_utilities.py
--rw-r--r--   0 runner    (1001) docker     (123)    14573 2023-04-19 19:51:08.000000 pulumi_libvirt-0.4.1a1681932948/pulumi_libvirt/cloud_init_disk.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 19:51:09.016923 pulumi_libvirt-0.4.1a1681932948/pulumi_libvirt/config/
--rw-r--r--   0 runner    (1001) docker     (123)      285 2023-04-19 19:51:08.000000 pulumi_libvirt-0.4.1a1681932948/pulumi_libvirt/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      679 2023-04-19 19:51:08.000000 pulumi_libvirt-0.4.1a1681932948/pulumi_libvirt/config/vars.py
--rw-r--r--   0 runner    (1001) docker     (123)    72754 2023-04-19 19:51:08.000000 pulumi_libvirt-0.4.1a1681932948/pulumi_libvirt/domain.py
--rw-r--r--   0 runner    (1001) docker     (123)     3587 2023-04-19 19:51:08.000000 pulumi_libvirt-0.4.1a1681932948/pulumi_libvirt/get_network_dns_host_template.py
--rw-r--r--   0 runner    (1001) docker     (123)     6385 2023-04-19 19:51:08.000000 pulumi_libvirt-0.4.1a1681932948/pulumi_libvirt/get_network_dns_srv_template.py
--rw-r--r--   0 runner    (1001) docker     (123)     3986 2023-04-19 19:51:08.000000 pulumi_libvirt-0.4.1a1681932948/pulumi_libvirt/get_network_dnsmasq_options_template.py
--rw-r--r--   0 runner    (1001) docker     (123)     8813 2023-04-19 19:51:08.000000 pulumi_libvirt-0.4.1a1681932948/pulumi_libvirt/ignition.py
--rw-r--r--   0 runner    (1001) docker     (123)    34091 2023-04-19 19:51:08.000000 pulumi_libvirt-0.4.1a1681932948/pulumi_libvirt/network.py
--rw-r--r--   0 runner    (1001) docker     (123)    38775 2023-04-19 19:51:08.000000 pulumi_libvirt-0.4.1a1681932948/pulumi_libvirt/outputs.py
--rw-r--r--   0 runner    (1001) docker     (123)    16032 2023-04-19 19:51:08.000000 pulumi_libvirt-0.4.1a1681932948/pulumi_libvirt/pool.py
--rw-r--r--   0 runner    (1001) docker     (123)     4666 2023-04-19 19:51:08.000000 pulumi_libvirt-0.4.1a1681932948/pulumi_libvirt/provider.py
--rw-r--r--   0 runner    (1001) docker     (123)       44 2023-04-19 19:51:08.000000 pulumi_libvirt-0.4.1a1681932948/pulumi_libvirt/pulumi-plugin.json
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 19:51:08.000000 pulumi_libvirt-0.4.1a1681932948/pulumi_libvirt/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    22961 2023-04-19 19:51:08.000000 pulumi_libvirt-0.4.1a1681932948/pulumi_libvirt/volume.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 19:51:09.016923 pulumi_libvirt-0.4.1a1681932948/pulumi_libvirt.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2396 2023-04-19 19:51:08.000000 pulumi_libvirt-0.4.1a1681932948/pulumi_libvirt.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      811 2023-04-19 19:51:09.000000 pulumi_libvirt-0.4.1a1681932948/pulumi_libvirt.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-19 19:51:08.000000 pulumi_libvirt-0.4.1a1681932948/pulumi_libvirt.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-19 19:51:08.000000 pulumi_libvirt-0.4.1a1681932948/pulumi_libvirt.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-04-19 19:51:09.000000 pulumi_libvirt-0.4.1a1681932948/pulumi_libvirt.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-04-19 19:51:09.000000 pulumi_libvirt-0.4.1a1681932948/pulumi_libvirt.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-19 19:51:09.016923 pulumi_libvirt-0.4.1a1681932948/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2133 2023-04-19 19:51:08.000000 pulumi_libvirt-0.4.1a1681932948/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 06:54:10.334162 pulumi_libvirt-0.4.1a1683267861/
+-rw-r--r--   0 runner    (1001) docker     (123)     2419 2023-05-05 06:54:10.334162 pulumi_libvirt-0.4.1a1683267861/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2049 2023-05-05 06:54:09.000000 pulumi_libvirt-0.4.1a1683267861/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 06:54:10.334162 pulumi_libvirt-0.4.1a1683267861/pulumi_libvirt/
+-rw-r--r--   0 runner    (1001) docker     (123)     1893 2023-05-05 06:54:09.000000 pulumi_libvirt-0.4.1a1683267861/pulumi_libvirt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    45336 2023-05-05 06:54:09.000000 pulumi_libvirt-0.4.1a1683267861/pulumi_libvirt/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8081 2023-05-05 06:54:09.000000 pulumi_libvirt-0.4.1a1683267861/pulumi_libvirt/_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14573 2023-05-05 06:54:09.000000 pulumi_libvirt-0.4.1a1683267861/pulumi_libvirt/cloud_init_disk.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 06:54:10.334162 pulumi_libvirt-0.4.1a1683267861/pulumi_libvirt/config/
+-rw-r--r--   0 runner    (1001) docker     (123)      285 2023-05-05 06:54:09.000000 pulumi_libvirt-0.4.1a1683267861/pulumi_libvirt/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      679 2023-05-05 06:54:09.000000 pulumi_libvirt-0.4.1a1683267861/pulumi_libvirt/config/vars.py
+-rw-r--r--   0 runner    (1001) docker     (123)    72754 2023-05-05 06:54:09.000000 pulumi_libvirt-0.4.1a1683267861/pulumi_libvirt/domain.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3587 2023-05-05 06:54:09.000000 pulumi_libvirt-0.4.1a1683267861/pulumi_libvirt/get_network_dns_host_template.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6385 2023-05-05 06:54:09.000000 pulumi_libvirt-0.4.1a1683267861/pulumi_libvirt/get_network_dns_srv_template.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3986 2023-05-05 06:54:09.000000 pulumi_libvirt-0.4.1a1683267861/pulumi_libvirt/get_network_dnsmasq_options_template.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8813 2023-05-05 06:54:09.000000 pulumi_libvirt-0.4.1a1683267861/pulumi_libvirt/ignition.py
+-rw-r--r--   0 runner    (1001) docker     (123)    34091 2023-05-05 06:54:09.000000 pulumi_libvirt-0.4.1a1683267861/pulumi_libvirt/network.py
+-rw-r--r--   0 runner    (1001) docker     (123)    38775 2023-05-05 06:54:09.000000 pulumi_libvirt-0.4.1a1683267861/pulumi_libvirt/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16032 2023-05-05 06:54:09.000000 pulumi_libvirt-0.4.1a1683267861/pulumi_libvirt/pool.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4666 2023-05-05 06:54:09.000000 pulumi_libvirt-0.4.1a1683267861/pulumi_libvirt/provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)       44 2023-05-05 06:54:09.000000 pulumi_libvirt-0.4.1a1683267861/pulumi_libvirt/pulumi-plugin.json
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 06:54:09.000000 pulumi_libvirt-0.4.1a1683267861/pulumi_libvirt/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    22961 2023-05-05 06:54:09.000000 pulumi_libvirt-0.4.1a1683267861/pulumi_libvirt/volume.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 06:54:10.334162 pulumi_libvirt-0.4.1a1683267861/pulumi_libvirt.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2419 2023-05-05 06:54:10.000000 pulumi_libvirt-0.4.1a1683267861/pulumi_libvirt.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      811 2023-05-05 06:54:10.000000 pulumi_libvirt-0.4.1a1683267861/pulumi_libvirt.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 06:54:10.000000 pulumi_libvirt-0.4.1a1683267861/pulumi_libvirt.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 06:54:10.000000 pulumi_libvirt-0.4.1a1683267861/pulumi_libvirt.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-05-05 06:54:10.000000 pulumi_libvirt-0.4.1a1683267861/pulumi_libvirt.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-05-05 06:54:10.000000 pulumi_libvirt-0.4.1a1683267861/pulumi_libvirt.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-05 06:54:10.334162 pulumi_libvirt-0.4.1a1683267861/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2164 2023-05-05 06:54:09.000000 pulumi_libvirt-0.4.1a1683267861/setup.py
```

### Comparing `pulumi_libvirt-0.4.1a1681932948/PKG-INFO` & `pulumi_libvirt-0.4.1a1683267861/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 Metadata-Version: 2.1
 Name: pulumi_libvirt
-Version: 0.4.1a1681932948
+Version: 0.4.1a1683267861
 Summary: A Pulumi package for creating and managing libvirt cloud resources.
 Home-page: https://pulumi.io
 License: Apache-2.0
 Project-URL: Repository, https://github.com/pulumi/pulumi-libvirt
 Keywords: pulumi libvirt
 Platform: UNKNOWN
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 
 [![Actions Status](https://github.com/pulumi/pulumi-libvirt/workflows/master/badge.svg)](https://github.com/pulumi/pulumi-libvirt/actions)
 [![Slack](http://www.pulumi.com/images/docs/badges/slack.svg)](https://slack.pulumi.com)
 [![NPM version](https://badge.fury.io/js/%40pulumi%2Flibvirt.svg)](https://www.npmjs.com/package/@pulumi/libvirt)
 [![Python version](https://badge.fury.io/py/pulumi-libvirt.svg)](https://pypi.org/project/pulumi-libvirt)
 [![NuGet version](https://badge.fury.io/nu/pulumi.libvirt.svg)](https://badge.fury.io/nu/pulumi.libvirt)
```

### Comparing `pulumi_libvirt-0.4.1a1681932948/README.md` & `pulumi_libvirt-0.4.1a1683267861/README.md`

 * *Files identical despite different names*

### Comparing `pulumi_libvirt-0.4.1a1681932948/pulumi_libvirt/__init__.py` & `pulumi_libvirt-0.4.1a1683267861/pulumi_libvirt/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_libvirt-0.4.1a1681932948/pulumi_libvirt/_inputs.py` & `pulumi_libvirt-0.4.1a1683267861/pulumi_libvirt/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_libvirt-0.4.1a1681932948/pulumi_libvirt/_utilities.py` & `pulumi_libvirt-0.4.1a1683267861/pulumi_libvirt/_utilities.py`

 * *Files identical despite different names*

### Comparing `pulumi_libvirt-0.4.1a1681932948/pulumi_libvirt/cloud_init_disk.py` & `pulumi_libvirt-0.4.1a1683267861/pulumi_libvirt/cloud_init_disk.py`

 * *Files identical despite different names*

### Comparing `pulumi_libvirt-0.4.1a1681932948/pulumi_libvirt/config/vars.py` & `pulumi_libvirt-0.4.1a1683267861/pulumi_libvirt/config/vars.py`

 * *Files identical despite different names*

### Comparing `pulumi_libvirt-0.4.1a1681932948/pulumi_libvirt/domain.py` & `pulumi_libvirt-0.4.1a1683267861/pulumi_libvirt/domain.py`

 * *Files identical despite different names*

### Comparing `pulumi_libvirt-0.4.1a1681932948/pulumi_libvirt/get_network_dns_host_template.py` & `pulumi_libvirt-0.4.1a1683267861/pulumi_libvirt/get_network_dns_host_template.py`

 * *Files identical despite different names*

### Comparing `pulumi_libvirt-0.4.1a1681932948/pulumi_libvirt/get_network_dns_srv_template.py` & `pulumi_libvirt-0.4.1a1683267861/pulumi_libvirt/get_network_dns_srv_template.py`

 * *Files identical despite different names*

### Comparing `pulumi_libvirt-0.4.1a1681932948/pulumi_libvirt/get_network_dnsmasq_options_template.py` & `pulumi_libvirt-0.4.1a1683267861/pulumi_libvirt/get_network_dnsmasq_options_template.py`

 * *Files identical despite different names*

### Comparing `pulumi_libvirt-0.4.1a1681932948/pulumi_libvirt/ignition.py` & `pulumi_libvirt-0.4.1a1683267861/pulumi_libvirt/ignition.py`

 * *Files identical despite different names*

### Comparing `pulumi_libvirt-0.4.1a1681932948/pulumi_libvirt/network.py` & `pulumi_libvirt-0.4.1a1683267861/pulumi_libvirt/network.py`

 * *Files identical despite different names*

### Comparing `pulumi_libvirt-0.4.1a1681932948/pulumi_libvirt/outputs.py` & `pulumi_libvirt-0.4.1a1683267861/pulumi_libvirt/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_libvirt-0.4.1a1681932948/pulumi_libvirt/pool.py` & `pulumi_libvirt-0.4.1a1683267861/pulumi_libvirt/pool.py`

 * *Files identical despite different names*

### Comparing `pulumi_libvirt-0.4.1a1681932948/pulumi_libvirt/provider.py` & `pulumi_libvirt-0.4.1a1683267861/pulumi_libvirt/provider.py`

 * *Files identical despite different names*

### Comparing `pulumi_libvirt-0.4.1a1681932948/pulumi_libvirt/volume.py` & `pulumi_libvirt-0.4.1a1683267861/pulumi_libvirt/volume.py`

 * *Files identical despite different names*

### Comparing `pulumi_libvirt-0.4.1a1681932948/pulumi_libvirt.egg-info/PKG-INFO` & `pulumi_libvirt-0.4.1a1683267861/pulumi_libvirt.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 Metadata-Version: 2.1
 Name: pulumi-libvirt
-Version: 0.4.1a1681932948
+Version: 0.4.1a1683267861
 Summary: A Pulumi package for creating and managing libvirt cloud resources.
 Home-page: https://pulumi.io
 License: Apache-2.0
 Project-URL: Repository, https://github.com/pulumi/pulumi-libvirt
 Keywords: pulumi libvirt
 Platform: UNKNOWN
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 
 [![Actions Status](https://github.com/pulumi/pulumi-libvirt/workflows/master/badge.svg)](https://github.com/pulumi/pulumi-libvirt/actions)
 [![Slack](http://www.pulumi.com/images/docs/badges/slack.svg)](https://slack.pulumi.com)
 [![NPM version](https://badge.fury.io/js/%40pulumi%2Flibvirt.svg)](https://www.npmjs.com/package/@pulumi/libvirt)
 [![Python version](https://badge.fury.io/py/pulumi-libvirt.svg)](https://pypi.org/project/pulumi-libvirt)
 [![NuGet version](https://badge.fury.io/nu/pulumi.libvirt.svg)](https://badge.fury.io/nu/pulumi.libvirt)
```

### Comparing `pulumi_libvirt-0.4.1a1681932948/pulumi_libvirt.egg-info/SOURCES.txt` & `pulumi_libvirt-0.4.1a1683267861/pulumi_libvirt.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pulumi_libvirt-0.4.1a1681932948/setup.py` & `pulumi_libvirt-0.4.1a1683267861/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -4,16 +4,16 @@
 
 import errno
 from setuptools import setup, find_packages
 from setuptools.command.install import install
 from subprocess import check_call
 
 
-VERSION = "0.4.1a1681932948"
-PLUGIN_VERSION = "0.4.1-alpha.1681932948+5785dbf8"
+VERSION = "0.4.1a1683267861"
+PLUGIN_VERSION = "0.4.1-alpha.1683267861+040c016c"
 
 class InstallPluginCommand(install):
     def run(self):
         install.run(self)
         try:
             check_call(['pulumi', 'plugin', 'install', 'resource', 'libvirt', PLUGIN_VERSION])
         except OSError as error:
@@ -34,14 +34,15 @@
         with open('README.md', encoding='utf-8') as f:
             return f.read()
     except FileNotFoundError:
         return "libvirt Pulumi Package - Development Version"
 
 
 setup(name='pulumi_libvirt',
+      python_requires='>=3.7',
       version=VERSION,
       description="A Pulumi package for creating and managing libvirt cloud resources.",
       long_description=readme(),
       long_description_content_type='text/markdown',
       cmdclass={
           'install': InstallPluginCommand,
       },
```

