# Comparing `tmp/simauth-0.0.8.tar.gz` & `tmp/simauth-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/simauth-0.0.8.tar", last modified: Mon Apr 17 12:12:34 2023, max compression
+gzip compressed data, was "dist/simauth-0.0.9.tar", last modified: Fri May  5 03:40:01 2023, max compression
```

## Comparing `simauth-0.0.8.tar` & `simauth-0.0.9.tar`

### file list

```diff
@@ -1,12 +1,12 @@
-drwxrwxr-x   0 gaoang    (1001) gaoang    (1001)        0 2023-04-17 12:12:34.122870 simauth-0.0.8/
--rw-rw-r--   0 gaoang    (1001) gaoang    (1001)      299 2023-04-17 12:12:34.122870 simauth-0.0.8/PKG-INFO
--rw-r--r--   0 gaoang    (1001) gaoang    (1001)        5 2022-11-24 14:14:06.000000 simauth-0.0.8/README.md
--rw-rw-r--   0 gaoang    (1001) gaoang    (1001)       38 2023-04-17 12:12:34.122870 simauth-0.0.8/setup.cfg
--rw-r--r--   0 gaoang    (1001) gaoang    (1001)      546 2023-04-17 12:12:32.000000 simauth-0.0.8/setup.py
-drwxrwxr-x   0 gaoang    (1001) gaoang    (1001)        0 2023-04-17 12:12:34.122870 simauth-0.0.8/simauth/
--rw-r--r--   0 gaoang    (1001) gaoang    (1001)     2056 2023-01-18 01:57:29.000000 simauth-0.0.8/simauth/__init__.py
-drwxrwxr-x   0 gaoang    (1001) gaoang    (1001)        0 2023-04-17 12:12:34.122870 simauth-0.0.8/simauth.egg-info/
--rw-rw-r--   0 gaoang    (1001) gaoang    (1001)      299 2023-04-17 12:12:34.000000 simauth-0.0.8/simauth.egg-info/PKG-INFO
--rw-rw-r--   0 gaoang    (1001) gaoang    (1001)      162 2023-04-17 12:12:34.000000 simauth-0.0.8/simauth.egg-info/SOURCES.txt
--rw-rw-r--   0 gaoang    (1001) gaoang    (1001)        1 2023-04-17 12:12:34.000000 simauth-0.0.8/simauth.egg-info/dependency_links.txt
--rw-rw-r--   0 gaoang    (1001) gaoang    (1001)        8 2023-04-17 12:12:34.000000 simauth-0.0.8/simauth.egg-info/top_level.txt
+drwxrwxr-x   0 gaoang    (1001) gaoang    (1001)        0 2023-05-05 03:40:01.293974 simauth-0.0.9/
+-rw-rw-r--   0 gaoang    (1001) gaoang    (1001)      299 2023-05-05 03:40:01.293974 simauth-0.0.9/PKG-INFO
+-rw-r--r--   0 gaoang    (1001) gaoang    (1001)        5 2022-11-24 14:14:06.000000 simauth-0.0.9/README.md
+-rw-rw-r--   0 gaoang    (1001) gaoang    (1001)       38 2023-05-05 03:40:01.293974 simauth-0.0.9/setup.cfg
+-rw-r--r--   0 gaoang    (1001) gaoang    (1001)      526 2023-05-05 03:39:43.000000 simauth-0.0.9/setup.py
+drwxrwxr-x   0 gaoang    (1001) gaoang    (1001)        0 2023-05-05 03:40:01.293974 simauth-0.0.9/simauth/
+-rw-r--r--   0 gaoang    (1001) gaoang    (1001)     2260 2023-05-05 03:39:04.000000 simauth-0.0.9/simauth/__init__.py
+drwxrwxr-x   0 gaoang    (1001) gaoang    (1001)        0 2023-05-05 03:40:01.293974 simauth-0.0.9/simauth.egg-info/
+-rw-rw-r--   0 gaoang    (1001) gaoang    (1001)      299 2023-05-05 03:40:01.000000 simauth-0.0.9/simauth.egg-info/PKG-INFO
+-rw-rw-r--   0 gaoang    (1001) gaoang    (1001)      162 2023-05-05 03:40:01.000000 simauth-0.0.9/simauth.egg-info/SOURCES.txt
+-rw-rw-r--   0 gaoang    (1001) gaoang    (1001)        1 2023-05-05 03:40:01.000000 simauth-0.0.9/simauth.egg-info/dependency_links.txt
+-rw-rw-r--   0 gaoang    (1001) gaoang    (1001)        8 2023-05-05 03:40:01.000000 simauth-0.0.9/simauth.egg-info/top_level.txt
```

### Comparing `simauth-0.0.8/setup.py` & `simauth-0.0.9/setup.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="simauth",
-    version="0.0.8",  # Latest version .
+    version="0.0.9",
     author="none",
     author_email="google@gmail.com",
     description="ok",
     long_description=long_description,
     long_description_content_type="text/markdown",
     packages=setuptools.find_packages(),
     classifiers=[
```

### Comparing `simauth-0.0.8/simauth/__init__.py` & `simauth-0.0.9/simauth/__init__.py`

 * *Files 16% similar despite different names*

```diff
@@ -9,18 +9,24 @@
 class Accounts(object):
 
     def __init__(self, accounts: dict, paths: list) -> None:
         self.accounts = accounts
         self.paths = paths
 
     def get_key(self) -> str:
-        for p in self.paths:
+        def complete_path(p):
             if p.startswith('~'):
-                p = os.path.expanduser(p)
-                return open(p).read().strip().encode()
+                return os.path.expanduser(p)
+            return p
+        pathes = [complete_path(p) for p in self.paths]
+        for p in pathes:
+            if os.path.exists(p):
+                content=open(p).read().strip().encode()
+                if content:
+                    return content
         raise Exception('Fernet key not found')
 
     def initialize(self) -> None:
 
         class Attrs(object):
 
             def __getitem__(self, key: str):
```

