# Comparing `tmp/fabricauthenticator-1.1rc9.tar.gz` & `tmp/fabricauthenticator-1.2rc0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "fabricauthenticator-1.1rc9.tar", last modified: Wed May 11 19:46:51 2022, max compression
+gzip compressed data, was "fabricauthenticator-1.2rc0.tar", last modified: Fri May  5 18:07:31 2023, max compression
```

## Comparing `fabricauthenticator-1.1rc9.tar` & `fabricauthenticator-1.2rc0.tar`

### file list

```diff
@@ -1,14 +1,7 @@
-drwxr-xr-x   0 kthare10   (503) staff       (20)        0 2022-05-11 19:46:51.203759 fabricauthenticator-1.1rc9/
--rw-r--r--   0 kthare10   (503) staff       (20)     1072 2021-07-23 17:00:43.000000 fabricauthenticator-1.1rc9/LICENSE
--rw-r--r--   0 kthare10   (503) staff       (20)     1864 2022-05-11 19:46:51.203365 fabricauthenticator-1.1rc9/PKG-INFO
--rw-r--r--   0 kthare10   (503) staff       (20)     1374 2021-07-23 17:00:43.000000 fabricauthenticator-1.1rc9/README.md
-drwxr-xr-x   0 kthare10   (503) staff       (20)        0 2022-05-11 19:46:51.201396 fabricauthenticator-1.1rc9/fabricauthenticator/
--rw-r--r--   0 kthare10   (503) staff       (20)       35 2022-02-02 20:21:50.000000 fabricauthenticator-1.1rc9/fabricauthenticator/__init__.py
--rw-r--r--   0 kthare10   (503) staff       (20)     4826 2022-05-11 19:46:17.000000 fabricauthenticator-1.1rc9/fabricauthenticator/fabricauthenticator.py
-drwxr-xr-x   0 kthare10   (503) staff       (20)        0 2022-05-11 19:46:51.202946 fabricauthenticator-1.1rc9/fabricauthenticator.egg-info/
--rw-r--r--   0 kthare10   (503) staff       (20)     1864 2022-05-11 19:46:50.000000 fabricauthenticator-1.1rc9/fabricauthenticator.egg-info/PKG-INFO
--rw-r--r--   0 kthare10   (503) staff       (20)      273 2022-05-11 19:46:51.000000 fabricauthenticator-1.1rc9/fabricauthenticator.egg-info/SOURCES.txt
--rw-r--r--   0 kthare10   (503) staff       (20)        1 2022-05-11 19:46:50.000000 fabricauthenticator-1.1rc9/fabricauthenticator.egg-info/dependency_links.txt
--rw-r--r--   0 kthare10   (503) staff       (20)       20 2022-05-11 19:46:51.000000 fabricauthenticator-1.1rc9/fabricauthenticator.egg-info/top_level.txt
--rw-r--r--   0 kthare10   (503) staff       (20)       38 2022-05-11 19:46:51.203879 fabricauthenticator-1.1rc9/setup.cfg
--rw-r--r--   0 kthare10   (503) staff       (20)      732 2022-05-11 19:46:30.000000 fabricauthenticator-1.1rc9/setup.py
+-rw-r--r--   0        0        0     1806 2023-05-05 18:03:14.733463 fabricauthenticator-1.2rc0/.gitignore
+-rw-r--r--   0        0        0     1072 2023-05-03 18:37:04.862085 fabricauthenticator-1.2rc0/LICENSE
+-rw-r--r--   0        0        0     1164 2023-05-03 18:37:04.862450 fabricauthenticator-1.2rc0/README.md
+-rw-r--r--   0        0        0       23 2023-05-05 18:00:19.782657 fabricauthenticator-1.2rc0/fabricauthenticator/__init__.py
+-rw-r--r--   0        0        0     6269 2023-05-05 15:56:19.372834 fabricauthenticator-1.2rc0/fabricauthenticator/fabricauthenticator.py
+-rw-r--r--   0        0        0      798 2023-05-05 17:59:47.733357 fabricauthenticator-1.2rc0/pyproject.toml
+-rw-r--r--   0        0        0     1774 1970-01-01 00:00:00.000000 fabricauthenticator-1.2rc0/PKG-INFO
```

### Comparing `fabricauthenticator-1.1rc9/LICENSE` & `fabricauthenticator-1.2rc0/LICENSE`

 * *Files identical despite different names*

### Comparing `fabricauthenticator-1.1rc9/PKG-INFO` & `fabricauthenticator-1.2rc0/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 Metadata-Version: 2.1
 Name: fabricauthenticator
-Version: 1.1rc9
-Summary: Fabric Authenticator for Jupyterhub
-Home-page: https://github.com/fabric-testbed/fabricauthenticator
-Author: Erica Fu, Komal Thareja
-Author-email: ericafu@renci.org, kthare10@renci.org
+Version: 1.2rc0
+Summary: Fabric OAuth Authenticator
+Keywords: Swagger,Fabric OAuth Authenticator
+Author-email: Komal Thareja <kthare10@renci.org>
+Requires-Python: >=3.9
+Description-Content-Type: text/markdown
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.7
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-[![Requirements Status](https://requires.io/github/fabric-testbed/fabricauthenticator/requirements.svg?branch=vouch)](https://requires.io/github/fabric-testbed/fabricauthenticator/requirements/?branch=master)
+Requires-Dist: jupyterhub>=1.0
+Requires-Dist: oauthenticator
+Requires-Dist: ldap3
+Project-URL: Home, https://fabric-testbed.net/
+Project-URL: Sources, https://github.com/fabric-testbed/fabricauthenticator
 
 [![PyPI](https://img.shields.io/pypi/v/fabricauthenticator?style=plastic)](https://pypi.org/project/fabricauthenticator/)
 
 # Fabric Authenticator for Jupyterhub
 
 The authenticator for Fabric Testbed Jupyterhub
 Based on CILogon authentication, in addition it checks if user belongs to Fabric JUPYTERHUB COU group
@@ -50,7 +51,8 @@
       c.CILogonOAuthenticator.client_secret = ""
       c.CILogonOAuthenticator.oauth_callback_url = "<host>/hub/oauth_callback"
 auth:
   type: custom
   custom:
       className: fabricauthenticator.FabricAuthenticator
 ```
+
```

### Comparing `fabricauthenticator-1.1rc9/README.md` & `fabricauthenticator-1.2rc0/README.md`

 * *Files 19% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-[![Requirements Status](https://requires.io/github/fabric-testbed/fabricauthenticator/requirements.svg?branch=vouch)](https://requires.io/github/fabric-testbed/fabricauthenticator/requirements/?branch=master)
-
 [![PyPI](https://img.shields.io/pypi/v/fabricauthenticator?style=plastic)](https://pypi.org/project/fabricauthenticator/)
 
 # Fabric Authenticator for Jupyterhub
 
 The authenticator for Fabric Testbed Jupyterhub
 Based on CILogon authentication, in addition it checks if user belongs to Fabric JUPYTERHUB COU group
```

