# Comparing `tmp/pyfanity-0.0.1.tar.gz` & `tmp/pyfanity-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyfanity-0.0.1.tar", last modified: Fri May  5 06:42:52 2023, max compression
+gzip compressed data, was "pyfanity-0.1.0.tar", last modified: Fri May  5 06:46:15 2023, max compression
```

## Comparing `pyfanity-0.0.1.tar` & `pyfanity-0.1.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-05-05 06:42:52.580615 pyfanity-0.0.1/
--rw-rw-rw-   0        0        0        0 2023-05-05 06:26:20.000000 pyfanity-0.0.1/LICENSE
--rw-rw-rw-   0        0        0      844 2023-05-05 06:42:52.580615 pyfanity-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0      174 2023-05-05 06:26:08.000000 pyfanity-0.0.1/README.md
-drwxrwxrwx   0        0        0        0 2023-05-05 06:42:52.566615 pyfanity-0.0.1/pyfanity/
--rw-rw-rw-   0        0        0       83 2023-05-05 04:57:03.000000 pyfanity-0.0.1/pyfanity/__init__.py
--rw-rw-rw-   0        0        0       43 2023-05-05 06:18:12.000000 pyfanity-0.0.1/pyfanity/example.py
-drwxrwxrwx   0        0        0        0 2023-05-05 06:42:52.579613 pyfanity-0.0.1/pyfanity.egg-info/
--rw-rw-rw-   0        0        0      844 2023-05-05 06:42:52.000000 pyfanity-0.0.1/pyfanity.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      210 2023-05-05 06:42:52.000000 pyfanity-0.0.1/pyfanity.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-05 06:42:52.000000 pyfanity-0.0.1/pyfanity.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        9 2023-05-05 06:42:52.000000 pyfanity-0.0.1/pyfanity.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      586 2023-05-05 06:25:43.000000 pyfanity-0.0.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-05 06:42:52.581612 pyfanity-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0     1181 2023-05-05 04:57:03.000000 pyfanity-0.0.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-05 06:46:15.802636 pyfanity-0.1.0/
+-rw-rw-rw-   0        0        0        0 2023-05-05 06:26:20.000000 pyfanity-0.1.0/LICENSE
+-rw-rw-rw-   0        0        0      844 2023-05-05 06:46:15.801637 pyfanity-0.1.0/PKG-INFO
+-rw-rw-rw-   0        0        0      174 2023-05-05 06:26:08.000000 pyfanity-0.1.0/README.md
+drwxrwxrwx   0        0        0        0 2023-05-05 06:46:15.793636 pyfanity-0.1.0/pyfanity/
+-rw-rw-rw-   0        0        0       83 2023-05-05 04:57:03.000000 pyfanity-0.1.0/pyfanity/__init__.py
+-rw-rw-rw-   0        0        0       43 2023-05-05 06:18:12.000000 pyfanity-0.1.0/pyfanity/example.py
+drwxrwxrwx   0        0        0        0 2023-05-05 06:46:15.801637 pyfanity-0.1.0/pyfanity.egg-info/
+-rw-rw-rw-   0        0        0      844 2023-05-05 06:46:15.000000 pyfanity-0.1.0/pyfanity.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      210 2023-05-05 06:46:15.000000 pyfanity-0.1.0/pyfanity.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-05 06:46:15.000000 pyfanity-0.1.0/pyfanity.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        9 2023-05-05 06:46:15.000000 pyfanity-0.1.0/pyfanity.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      586 2023-05-05 06:25:43.000000 pyfanity-0.1.0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-05 06:46:15.802636 pyfanity-0.1.0/setup.cfg
+-rw-rw-rw-   0        0        0     1181 2023-05-05 06:45:45.000000 pyfanity-0.1.0/setup.py
```

### Comparing `pyfanity-0.0.1/PKG-INFO` & `pyfanity-0.1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyfanity
-Version: 0.0.1
+Version: 0.1.0
 Summary: A simple and light weight profanity filter package.
 Home-page: https://github.com/stampixel/pyfanity
 Author: Kevin Tang
 Author-email: stampixel@pm.me
 License: MIT
 Keywords: profanity,profanity blocker,swear,langauge,language-filter
 Platform: UNKNOWN
```

### Comparing `pyfanity-0.0.1/pyfanity.egg-info/PKG-INFO` & `pyfanity-0.1.0/pyfanity.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyfanity
-Version: 0.0.1
+Version: 0.1.0
 Summary: A simple and light weight profanity filter package.
 Home-page: https://github.com/stampixel/pyfanity
 Author: Kevin Tang
 Author-email: stampixel@pm.me
 License: MIT
 Keywords: profanity,profanity blocker,swear,langauge,language-filter
 Platform: UNKNOWN
```

### Comparing `pyfanity-0.0.1/pyproject.toml` & `pyfanity-0.1.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pyfanity-0.0.1/setup.py` & `pyfanity-0.1.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 REQUIREMENTS = [
     ""
 ]
 
 setup(
     name="pyfanity",
-    version="0.0.1",
+    version=VERSION,
     author="Kevin Tang",
     author_email="stampixel@pm.me",
     license="MIT",
     url="https://github.com/stampixel/pyfanity",
     install_requires=REQUIREMENTS,
     keywords=[
         "profanity",
```

