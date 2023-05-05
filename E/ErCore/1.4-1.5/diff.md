# Comparing `tmp/ErCore-1.4.tar.gz` & `tmp/ErCore-1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ErCore-1.4.tar", last modified: Thu May  4 11:43:25 2023, max compression
+gzip compressed data, was "ErCore-1.5.tar", last modified: Fri May  5 12:53:21 2023, max compression
```

## Comparing `ErCore-1.4.tar` & `ErCore-1.5.tar`

### file list

```diff
@@ -1,18 +1,19 @@
-drwxrwxrwx   0        0        0        0 2023-05-04 11:43:25.089462 ErCore-1.4/
-drwxrwxrwx   0        0        0        0 2023-05-04 11:43:25.060463 ErCore-1.4/ErCore/
--rw-rw-rw-   0        0        0     2065 2023-05-04 11:42:03.000000 ErCore-1.4/ErCore/Core.py
--rw-rw-rw-   0        0        0       33 2023-05-04 11:39:44.000000 ErCore-1.4/ErCore/__init__.py
--rw-rw-rw-   0        0        0     3172 2023-05-04 11:40:35.000000 ErCore-1.4/ErCore/cli.py
-drwxrwxrwx   0        0        0        0 2023-05-04 11:43:25.084462 ErCore-1.4/ErCore/std/
--rw-rw-rw-   0        0        0     1666 2023-05-04 10:21:42.000000 ErCore-1.4/ErCore/std/Base.py
-drwxrwxrwx   0        0        0        0 2023-05-04 11:43:25.082472 ErCore-1.4/ErCore.egg-info/
--rw-rw-rw-   0        0        0      588 2023-05-04 11:43:24.000000 ErCore-1.4/ErCore.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      246 2023-05-04 11:43:24.000000 ErCore-1.4/ErCore.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-04 11:43:24.000000 ErCore-1.4/ErCore.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       98 2023-05-04 11:43:24.000000 ErCore-1.4/ErCore.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        7 2023-05-04 11:43:24.000000 ErCore-1.4/ErCore.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1086 2023-04-21 12:30:11.000000 ErCore-1.4/LICENSE
--rw-rw-rw-   0        0        0      588 2023-05-04 11:43:25.088462 ErCore-1.4/PKG-INFO
--rw-rw-rw-   0        0        0      233 2023-05-04 11:41:57.000000 ErCore-1.4/README.md
--rw-rw-rw-   0        0        0       42 2023-05-04 11:43:25.090463 ErCore-1.4/setup.cfg
--rw-rw-rw-   0        0        0      679 2023-05-04 11:41:52.000000 ErCore-1.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-05 12:53:21.602856 ErCore-1.5/
+drwxrwxrwx   0        0        0        0 2023-05-05 12:53:21.378509 ErCore-1.5/ErCore/
+-rw-rw-rw-   0        0        0     2065 2023-05-05 12:53:02.000000 ErCore-1.5/ErCore/Core.py
+-rw-rw-rw-   0        0        0       52 2023-05-05 12:48:37.000000 ErCore-1.5/ErCore/__init__.py
+-rw-rw-rw-   0        0        0     3172 2023-05-04 11:40:35.000000 ErCore-1.5/ErCore/cli.py
+drwxrwxrwx   0        0        0        0 2023-05-05 12:53:21.535817 ErCore-1.5/ErCore/std/
+-rw-rw-rw-   0        0        0     1666 2023-05-04 10:21:42.000000 ErCore-1.5/ErCore/std/Base.py
+-rw-rw-rw-   0        0        0       20 2023-05-05 12:49:09.000000 ErCore-1.5/ErCore/std/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-05 12:53:21.473912 ErCore-1.5/ErCore.egg-info/
+-rw-rw-rw-   0        0        0      625 2023-05-05 12:53:20.000000 ErCore-1.5/ErCore.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      269 2023-05-05 12:53:20.000000 ErCore-1.5/ErCore.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-05 12:53:20.000000 ErCore-1.5/ErCore.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       98 2023-05-05 12:53:20.000000 ErCore-1.5/ErCore.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        7 2023-05-05 12:53:20.000000 ErCore-1.5/ErCore.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1086 2023-04-21 12:30:11.000000 ErCore-1.5/LICENSE
+-rw-rw-rw-   0        0        0      625 2023-05-05 12:53:21.570848 ErCore-1.5/PKG-INFO
+-rw-rw-rw-   0        0        0      270 2023-05-05 12:52:52.000000 ErCore-1.5/README.md
+-rw-rw-rw-   0        0        0       42 2023-05-05 12:53:21.602856 ErCore-1.5/setup.cfg
+-rw-rw-rw-   0        0        0      679 2023-05-05 12:49:51.000000 ErCore-1.5/setup.py
```

### Comparing `ErCore-1.4/ErCore/Core.py` & `ErCore-1.5/ErCore/Core.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 import platform
 
 from std.Base import *
 
 
 class ECore:
     def __init__(self):
-        self.version = 1.4
+        self.version = 1.5
         self.IS_WINDOWS = (platform.system() == 'Windows')
         self.IS_LINUX = (platform.system() == 'Linux')
         self.IS_MAC = (platform.system() == 'Darwin')
 
     def info(self):
         try:
             print(f'Autor: Eragod\nProject: ErCore\nVersion: {self.version}')
```

### Comparing `ErCore-1.4/ErCore/cli.py` & `ErCore-1.5/ErCore/cli.py`

 * *Files identical despite different names*

### Comparing `ErCore-1.4/ErCore/std/Base.py` & `ErCore-1.5/ErCore/std/Base.py`

 * *Files identical despite different names*

### Comparing `ErCore-1.4/LICENSE` & `ErCore-1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `ErCore-1.4/setup.py` & `ErCore-1.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='ErCore',
-    version='1.4',
+    version='1.5',
     packages=find_packages(),
     author='Eragod',
     description='Core for projects',
     url="https://github.com/Eragod/ErCore",
     long_description=open('README.md', 'r').read(),
     long_description_content_type="text/markdown",
     entry_points={'console_scripts': ['ErCore-project = ErCore.cli:make_project',
```

