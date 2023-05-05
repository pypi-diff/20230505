# Comparing `tmp/packagebinbin-0.0.2.tar.gz` & `tmp/packagebinbin-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/packagebinbin-0.0.2.tar", last modified: Fri May  5 08:37:57 2023, max compression
+gzip compressed data, was "dist/packagebinbin-0.0.3.tar", last modified: Fri May  5 08:39:35 2023, max compression
```

## Comparing `packagebinbin-0.0.2.tar` & `packagebinbin-0.0.3.tar`

### file list

```diff
@@ -1,9 +1,9 @@
-drwxr-xr-x   0 sher       (501) staff       (20)        0 2023-05-05 08:37:57.094955 packagebinbin-0.0.2/
--rw-r--r--   0 sher       (501) staff       (20)      508 2023-05-05 08:37:57.094815 packagebinbin-0.0.2/PKG-INFO
-drwxr-xr-x   0 sher       (501) staff       (20)        0 2023-05-05 08:37:57.094637 packagebinbin-0.0.2/packagebinbin.egg-info/
--rw-r--r--   0 sher       (501) staff       (20)      508 2023-05-05 08:37:57.000000 packagebinbin-0.0.2/packagebinbin.egg-info/PKG-INFO
--rw-r--r--   0 sher       (501) staff       (20)      156 2023-05-05 08:37:57.000000 packagebinbin-0.0.2/packagebinbin.egg-info/SOURCES.txt
--rw-r--r--   0 sher       (501) staff       (20)        1 2023-05-05 08:37:57.000000 packagebinbin-0.0.2/packagebinbin.egg-info/dependency_links.txt
--rw-r--r--   0 sher       (501) staff       (20)        1 2023-05-05 08:37:57.000000 packagebinbin-0.0.2/packagebinbin.egg-info/top_level.txt
--rw-r--r--   0 sher       (501) staff       (20)       38 2023-05-05 08:37:57.094995 packagebinbin-0.0.2/setup.cfg
--rw-r--r--   0 sher       (501) staff       (20)      689 2023-05-05 08:37:53.000000 packagebinbin-0.0.2/setup.py
+drwxr-xr-x   0 sher       (501) staff       (20)        0 2023-05-05 08:39:35.633092 packagebinbin-0.0.3/
+-rw-r--r--   0 sher       (501) staff       (20)      581 2023-05-05 08:39:35.632966 packagebinbin-0.0.3/PKG-INFO
+drwxr-xr-x   0 sher       (501) staff       (20)        0 2023-05-05 08:39:35.632793 packagebinbin-0.0.3/packagebinbin.egg-info/
+-rw-r--r--   0 sher       (501) staff       (20)      581 2023-05-05 08:39:35.000000 packagebinbin-0.0.3/packagebinbin.egg-info/PKG-INFO
+-rw-r--r--   0 sher       (501) staff       (20)      156 2023-05-05 08:39:35.000000 packagebinbin-0.0.3/packagebinbin.egg-info/SOURCES.txt
+-rw-r--r--   0 sher       (501) staff       (20)        1 2023-05-05 08:39:35.000000 packagebinbin-0.0.3/packagebinbin.egg-info/dependency_links.txt
+-rw-r--r--   0 sher       (501) staff       (20)        1 2023-05-05 08:39:35.000000 packagebinbin-0.0.3/packagebinbin.egg-info/top_level.txt
+-rw-r--r--   0 sher       (501) staff       (20)       38 2023-05-05 08:39:35.633138 packagebinbin-0.0.3/setup.cfg
+-rw-r--r--   0 sher       (501) staff       (20)      766 2023-05-05 08:39:31.000000 packagebinbin-0.0.3/setup.py
```

### Comparing `packagebinbin-0.0.2/setup.py` & `packagebinbin-0.0.3/setup.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,22 +1,24 @@
 from setuptools import setup, find_packages
 
 setup(
     name="packagebinbin",
-    version="0.0.2",
+    version="0.0.3",
     author="Sophat Chhay",
     author_email="<sophat.chhay@gmail.com>",
     description="My demo package with my daughter name",
     packages=find_packages(),
     install_requires=[],
     keywords=['python'],
     long_description= "Testing",
     long_description_content_type="text/markdown",
+    python_requires='>=3.6',
     classifiers=[
         "Development Status :: 1 - Planning",
         "Intended Audience :: Developers",
         "Programming Language :: Python :: 3",
         "Operating System :: Unix",
         "Operating System :: MacOS :: MacOS X",
         "Operating System :: Microsoft :: Windows",
+        "Programming Language :: Python :: 3.9"
     ]
 )
```

