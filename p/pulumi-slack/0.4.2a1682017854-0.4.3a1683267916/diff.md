# Comparing `tmp/pulumi_slack-0.4.2a1682017854.tar.gz` & `tmp/pulumi_slack-0.4.3a1683267916.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pulumi_slack-0.4.2a1682017854.tar", last modified: Thu Apr 20 19:15:34 2023, max compression
+gzip compressed data, was "pulumi_slack-0.4.3a1683267916.tar", last modified: Fri May  5 06:31:03 2023, max compression
```

## Comparing `pulumi_slack-0.4.2a1682017854.tar` & `pulumi_slack-0.4.3a1683267916.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 19:15:34.534107 pulumi_slack-0.4.2a1682017854/
--rw-r--r--   0 runner    (1001) docker     (123)     1408 2023-04-20 19:15:34.534107 pulumi_slack-0.4.2a1682017854/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1042 2023-04-20 19:15:34.000000 pulumi_slack-0.4.2a1682017854/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 19:15:34.530107 pulumi_slack-0.4.2a1682017854/pulumi_slack/
--rw-r--r--   0 runner    (1001) docker     (123)     1121 2023-04-20 19:15:34.000000 pulumi_slack-0.4.2a1682017854/pulumi_slack/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     8081 2023-04-20 19:15:34.000000 pulumi_slack-0.4.2a1682017854/pulumi_slack/_utilities.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 19:15:34.534107 pulumi_slack-0.4.2a1682017854/pulumi_slack/config/
--rw-r--r--   0 runner    (1001) docker     (123)      285 2023-04-20 19:15:34.000000 pulumi_slack-0.4.2a1682017854/pulumi_slack/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      580 2023-04-20 19:15:34.000000 pulumi_slack-0.4.2a1682017854/pulumi_slack/config/vars.py
--rw-r--r--   0 runner    (1001) docker     (123)    37057 2023-04-20 19:15:34.000000 pulumi_slack-0.4.2a1682017854/pulumi_slack/conversation.py
--rw-r--r--   0 runner    (1001) docker     (123)    10370 2023-04-20 19:15:34.000000 pulumi_slack-0.4.2a1682017854/pulumi_slack/get_conversation.py
--rw-r--r--   0 runner    (1001) docker     (123)     4475 2023-04-20 19:15:34.000000 pulumi_slack-0.4.2a1682017854/pulumi_slack/get_user.py
--rw-r--r--   0 runner    (1001) docker     (123)     6428 2023-04-20 19:15:34.000000 pulumi_slack-0.4.2a1682017854/pulumi_slack/get_usergroup.py
--rw-r--r--   0 runner    (1001) docker     (123)     4312 2023-04-20 19:15:34.000000 pulumi_slack-0.4.2a1682017854/pulumi_slack/provider.py
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-04-20 19:15:34.000000 pulumi_slack-0.4.2a1682017854/pulumi_slack/pulumi-plugin.json
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 19:15:34.000000 pulumi_slack-0.4.2a1682017854/pulumi_slack/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    17988 2023-04-20 19:15:34.000000 pulumi_slack-0.4.2a1682017854/pulumi_slack/usergroup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 19:15:34.534107 pulumi_slack-0.4.2a1682017854/pulumi_slack.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1408 2023-04-20 19:15:34.000000 pulumi_slack-0.4.2a1682017854/pulumi_slack.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      566 2023-04-20 19:15:34.000000 pulumi_slack-0.4.2a1682017854/pulumi_slack.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-20 19:15:34.000000 pulumi_slack-0.4.2a1682017854/pulumi_slack.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-20 19:15:34.000000 pulumi_slack-0.4.2a1682017854/pulumi_slack.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-04-20 19:15:34.000000 pulumi_slack-0.4.2a1682017854/pulumi_slack.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-04-20 19:15:34.000000 pulumi_slack-0.4.2a1682017854/pulumi_slack.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-20 19:15:34.534107 pulumi_slack-0.4.2a1682017854/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2150 2023-04-20 19:15:34.000000 pulumi_slack-0.4.2a1682017854/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 06:31:03.879872 pulumi_slack-0.4.3a1683267916/
+-rw-r--r--   0 runner    (1001) docker     (123)     1408 2023-05-05 06:31:03.879872 pulumi_slack-0.4.3a1683267916/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1042 2023-05-05 06:31:03.000000 pulumi_slack-0.4.3a1683267916/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 06:31:03.879872 pulumi_slack-0.4.3a1683267916/pulumi_slack/
+-rw-r--r--   0 runner    (1001) docker     (123)     1121 2023-05-05 06:31:03.000000 pulumi_slack-0.4.3a1683267916/pulumi_slack/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8081 2023-05-05 06:31:03.000000 pulumi_slack-0.4.3a1683267916/pulumi_slack/_utilities.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 06:31:03.879872 pulumi_slack-0.4.3a1683267916/pulumi_slack/config/
+-rw-r--r--   0 runner    (1001) docker     (123)      285 2023-05-05 06:31:03.000000 pulumi_slack-0.4.3a1683267916/pulumi_slack/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      580 2023-05-05 06:31:03.000000 pulumi_slack-0.4.3a1683267916/pulumi_slack/config/vars.py
+-rw-r--r--   0 runner    (1001) docker     (123)    37057 2023-05-05 06:31:03.000000 pulumi_slack-0.4.3a1683267916/pulumi_slack/conversation.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10370 2023-05-05 06:31:03.000000 pulumi_slack-0.4.3a1683267916/pulumi_slack/get_conversation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4475 2023-05-05 06:31:03.000000 pulumi_slack-0.4.3a1683267916/pulumi_slack/get_user.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6428 2023-05-05 06:31:03.000000 pulumi_slack-0.4.3a1683267916/pulumi_slack/get_usergroup.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4312 2023-05-05 06:31:03.000000 pulumi_slack-0.4.3a1683267916/pulumi_slack/provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-05-05 06:31:03.000000 pulumi_slack-0.4.3a1683267916/pulumi_slack/pulumi-plugin.json
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 06:31:03.000000 pulumi_slack-0.4.3a1683267916/pulumi_slack/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    17988 2023-05-05 06:31:03.000000 pulumi_slack-0.4.3a1683267916/pulumi_slack/usergroup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 06:31:03.879872 pulumi_slack-0.4.3a1683267916/pulumi_slack.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1408 2023-05-05 06:31:03.000000 pulumi_slack-0.4.3a1683267916/pulumi_slack.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      566 2023-05-05 06:31:03.000000 pulumi_slack-0.4.3a1683267916/pulumi_slack.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 06:31:03.000000 pulumi_slack-0.4.3a1683267916/pulumi_slack.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 06:31:03.000000 pulumi_slack-0.4.3a1683267916/pulumi_slack.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-05-05 06:31:03.000000 pulumi_slack-0.4.3a1683267916/pulumi_slack.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-05 06:31:03.000000 pulumi_slack-0.4.3a1683267916/pulumi_slack.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-05 06:31:03.879872 pulumi_slack-0.4.3a1683267916/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2150 2023-05-05 06:31:03.000000 pulumi_slack-0.4.3a1683267916/setup.py
```

### Comparing `pulumi_slack-0.4.2a1682017854/PKG-INFO` & `pulumi_slack-0.4.3a1683267916/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi_slack
-Version: 0.4.2a1682017854
+Version: 0.4.3a1683267916
 Summary: A Pulumi package for managing Slack workspaces.
 Home-page: https://www.pulumi.com
 License: Apache-2.0
 Project-URL: Repository, https://github.com/pulumi/pulumi-slack
 Keywords: pulumi slack category/utility
 Platform: UNKNOWN
 Requires-Python: >=3.7
```

### Comparing `pulumi_slack-0.4.2a1682017854/README.md` & `pulumi_slack-0.4.3a1683267916/README.md`

 * *Files identical despite different names*

### Comparing `pulumi_slack-0.4.2a1682017854/pulumi_slack/__init__.py` & `pulumi_slack-0.4.3a1683267916/pulumi_slack/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_slack-0.4.2a1682017854/pulumi_slack/_utilities.py` & `pulumi_slack-0.4.3a1683267916/pulumi_slack/_utilities.py`

 * *Files identical despite different names*

### Comparing `pulumi_slack-0.4.2a1682017854/pulumi_slack/config/vars.py` & `pulumi_slack-0.4.3a1683267916/pulumi_slack/config/vars.py`

 * *Files identical despite different names*

### Comparing `pulumi_slack-0.4.2a1682017854/pulumi_slack/conversation.py` & `pulumi_slack-0.4.3a1683267916/pulumi_slack/conversation.py`

 * *Files identical despite different names*

### Comparing `pulumi_slack-0.4.2a1682017854/pulumi_slack/get_conversation.py` & `pulumi_slack-0.4.3a1683267916/pulumi_slack/get_conversation.py`

 * *Files identical despite different names*

### Comparing `pulumi_slack-0.4.2a1682017854/pulumi_slack/get_user.py` & `pulumi_slack-0.4.3a1683267916/pulumi_slack/get_user.py`

 * *Files identical despite different names*

### Comparing `pulumi_slack-0.4.2a1682017854/pulumi_slack/get_usergroup.py` & `pulumi_slack-0.4.3a1683267916/pulumi_slack/get_usergroup.py`

 * *Files identical despite different names*

### Comparing `pulumi_slack-0.4.2a1682017854/pulumi_slack/provider.py` & `pulumi_slack-0.4.3a1683267916/pulumi_slack/provider.py`

 * *Files identical despite different names*

### Comparing `pulumi_slack-0.4.2a1682017854/pulumi_slack/usergroup.py` & `pulumi_slack-0.4.3a1683267916/pulumi_slack/usergroup.py`

 * *Files identical despite different names*

### Comparing `pulumi_slack-0.4.2a1682017854/pulumi_slack.egg-info/PKG-INFO` & `pulumi_slack-0.4.3a1683267916/pulumi_slack.egg-info/PKG-INFO`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi-slack
-Version: 0.4.2a1682017854
+Version: 0.4.3a1683267916
 Summary: A Pulumi package for managing Slack workspaces.
 Home-page: https://www.pulumi.com
 License: Apache-2.0
 Project-URL: Repository, https://github.com/pulumi/pulumi-slack
 Keywords: pulumi slack category/utility
 Platform: UNKNOWN
 Requires-Python: >=3.7
```

### Comparing `pulumi_slack-0.4.2a1682017854/pulumi_slack.egg-info/SOURCES.txt` & `pulumi_slack-0.4.3a1683267916/pulumi_slack.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pulumi_slack-0.4.2a1682017854/setup.py` & `pulumi_slack-0.4.3a1683267916/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,16 +4,16 @@
 
 import errno
 from setuptools import setup, find_packages
 from setuptools.command.install import install
 from subprocess import check_call
 
 
-VERSION = "0.4.2a1682017854"
-PLUGIN_VERSION = "0.4.2-alpha.1682017854+5c7b6a6e"
+VERSION = "0.4.3a1683267916"
+PLUGIN_VERSION = "0.4.3-alpha.1683267916+50bf5427"
 
 class InstallPluginCommand(install):
     def run(self):
         install.run(self)
         try:
             check_call(['pulumi', 'plugin', 'install', 'resource', 'slack', PLUGIN_VERSION])
         except OSError as error:
```

