# Comparing `tmp/packagebinbin-0.0.4.tar.gz` & `tmp/packagebinbin-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/packagebinbin-0.0.4.tar", last modified: Fri May  5 08:41:31 2023, max compression
+gzip compressed data, was "dist/packagebinbin-0.0.5.tar", last modified: Fri May  5 08:47:58 2023, max compression
```

## Comparing `packagebinbin-0.0.4.tar` & `packagebinbin-0.0.5.tar`

### file list

```diff
@@ -1,9 +1,10 @@
-drwxr-xr-x   0 sher       (501) staff       (20)        0 2023-05-05 08:41:31.959061 packagebinbin-0.0.4/
--rw-r--r--   0 sher       (501) staff       (20)      581 2023-05-05 08:41:31.958897 packagebinbin-0.0.4/PKG-INFO
-drwxr-xr-x   0 sher       (501) staff       (20)        0 2023-05-05 08:41:31.958698 packagebinbin-0.0.4/packagebinbin.egg-info/
--rw-r--r--   0 sher       (501) staff       (20)      581 2023-05-05 08:41:31.000000 packagebinbin-0.0.4/packagebinbin.egg-info/PKG-INFO
--rw-r--r--   0 sher       (501) staff       (20)      156 2023-05-05 08:41:31.000000 packagebinbin-0.0.4/packagebinbin.egg-info/SOURCES.txt
--rw-r--r--   0 sher       (501) staff       (20)        1 2023-05-05 08:41:31.000000 packagebinbin-0.0.4/packagebinbin.egg-info/dependency_links.txt
--rw-r--r--   0 sher       (501) staff       (20)        1 2023-05-05 08:41:31.000000 packagebinbin-0.0.4/packagebinbin.egg-info/top_level.txt
--rw-r--r--   0 sher       (501) staff       (20)       38 2023-05-05 08:41:31.959106 packagebinbin-0.0.4/setup.cfg
--rw-r--r--   0 sher       (501) staff       (20)      766 2023-05-05 08:41:28.000000 packagebinbin-0.0.4/setup.py
+drwxr-xr-x   0 sher       (501) staff       (20)        0 2023-05-05 08:47:58.536355 packagebinbin-0.0.5/
+-rw-r--r--   0 sher       (501) staff       (20)      581 2023-05-05 08:47:58.536218 packagebinbin-0.0.5/PKG-INFO
+-rw-r--r--   0 sher       (501) staff       (20)       85 2023-05-05 07:14:00.000000 packagebinbin-0.0.5/demo.py
+drwxr-xr-x   0 sher       (501) staff       (20)        0 2023-05-05 08:47:58.536050 packagebinbin-0.0.5/packagebinbin.egg-info/
+-rw-r--r--   0 sher       (501) staff       (20)      581 2023-05-05 08:47:58.000000 packagebinbin-0.0.5/packagebinbin.egg-info/PKG-INFO
+-rw-r--r--   0 sher       (501) staff       (20)      164 2023-05-05 08:47:58.000000 packagebinbin-0.0.5/packagebinbin.egg-info/SOURCES.txt
+-rw-r--r--   0 sher       (501) staff       (20)        1 2023-05-05 08:47:58.000000 packagebinbin-0.0.5/packagebinbin.egg-info/dependency_links.txt
+-rw-r--r--   0 sher       (501) staff       (20)        5 2023-05-05 08:47:58.000000 packagebinbin-0.0.5/packagebinbin.egg-info/top_level.txt
+-rw-r--r--   0 sher       (501) staff       (20)       38 2023-05-05 08:47:58.536395 packagebinbin-0.0.5/setup.cfg
+-rw-r--r--   0 sher       (501) staff       (20)      791 2023-05-05 08:47:56.000000 packagebinbin-0.0.5/setup.py
```

### Comparing `packagebinbin-0.0.4/PKG-INFO` & `packagebinbin-0.0.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: packagebinbin
-Version: 0.0.4
+Version: 0.0.5
 Summary: My demo package with my daughter name
 Author: Sophat Chhay
 Author-email: <sophat.chhay@gmail.com>
 Keywords: python
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `packagebinbin-0.0.4/packagebinbin.egg-info/PKG-INFO` & `packagebinbin-0.0.5/packagebinbin.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: packagebinbin
-Version: 0.0.4
+Version: 0.0.5
 Summary: My demo package with my daughter name
 Author: Sophat Chhay
 Author-email: <sophat.chhay@gmail.com>
 Keywords: python
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `packagebinbin-0.0.4/setup.py` & `packagebinbin-0.0.5/setup.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,16 +1,17 @@
 from setuptools import setup, find_packages
 
 setup(
     name="packagebinbin",
-    version="0.0.4",
+    version="0.0.5",
     author="Sophat Chhay",
     author_email="<sophat.chhay@gmail.com>",
     description="My demo package with my daughter name",
     packages=find_packages(),
+    py_modules=['demo'],
     install_requires=[],
     keywords=['python'],
     long_description= "Testing",
     long_description_content_type="text/markdown",
     python_requires='>=3.6',
     classifiers=[
         "Development Status :: 1 - Planning",
```

