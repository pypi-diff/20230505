# Comparing `tmp/packagebinbin-0.0.9.tar.gz` & `tmp/packagebinbin-1.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/Users/sher/Desktop/Sher/python/demopackage/dist/.tmp-mxpetbmu/packagebinbin-0.0.9.tar", last modified: Fri May  5 09:44:40 2023, max compression
+gzip compressed data, was "/Users/sher/Desktop/Sher/python/demopackage/dist/.tmp-ut02iwb4/packagebinbin-1.0.0.tar", last modified: Fri May  5 09:49:43 2023, max compression
```

## Comparing `packagebinbin-0.0.9.tar` & `packagebinbin-1.0.0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 sher       (501) staff       (20)        0 2023-05-05 09:44:40.086960 packagebinbin-0.0.9/
--rw-r--r--   0 sher       (501) staff       (20)     1073 2023-05-05 09:02:08.000000 packagebinbin-0.0.9/LICENSE
--rw-r--r--   0 sher       (501) staff       (20)      585 2023-05-05 09:44:40.086808 packagebinbin-0.0.9/PKG-INFO
--rw-r--r--   0 sher       (501) staff       (20)      172 2023-05-05 09:01:56.000000 packagebinbin-0.0.9/README.md
-drwxr-xr-x   0 sher       (501) staff       (20)        0 2023-05-05 09:44:40.085758 packagebinbin-0.0.9/packagebinbin.egg-info/
--rw-r--r--   0 sher       (501) staff       (20)      585 2023-05-05 09:44:40.000000 packagebinbin-0.0.9/packagebinbin.egg-info/PKG-INFO
--rw-r--r--   0 sher       (501) staff       (20)      261 2023-05-05 09:44:40.000000 packagebinbin-0.0.9/packagebinbin.egg-info/SOURCES.txt
--rw-r--r--   0 sher       (501) staff       (20)        1 2023-05-05 09:44:40.000000 packagebinbin-0.0.9/packagebinbin.egg-info/dependency_links.txt
--rw-r--r--   0 sher       (501) staff       (20)        9 2023-05-05 09:44:40.000000 packagebinbin-0.0.9/packagebinbin.egg-info/top_level.txt
--rw-r--r--   0 sher       (501) staff       (20)      359 2023-05-05 09:31:09.000000 packagebinbin-0.0.9/pyproject.toml
--rw-r--r--   0 sher       (501) staff       (20)       38 2023-05-05 09:44:40.086999 packagebinbin-0.0.9/setup.cfg
--rw-r--r--   0 sher       (501) staff       (20)      791 2023-05-05 08:54:45.000000 packagebinbin-0.0.9/setup.py
-drwxr-xr-x   0 sher       (501) staff       (20)        0 2023-05-05 09:44:40.085894 packagebinbin-0.0.9/src/
--rw-r--r--   0 sher       (501) staff       (20)       40 2023-05-05 09:06:36.000000 packagebinbin-0.0.9/src/__init__.py
-drwxr-xr-x   0 sher       (501) staff       (20)        0 2023-05-05 09:44:40.086466 packagebinbin-0.0.9/src/packagebinbin/
--rw-r--r--   0 sher       (501) staff       (20)       21 2023-05-05 09:06:36.000000 packagebinbin-0.0.9/src/packagebinbin/__init__.py
--rw-r--r--   0 sher       (501) staff       (20)      136 2023-05-05 08:59:11.000000 packagebinbin-0.0.9/src/packagebinbin/demo.py
+drwxr-xr-x   0 sher       (501) staff       (20)        0 2023-05-05 09:49:43.300480 packagebinbin-1.0.0/
+-rw-r--r--   0 sher       (501) staff       (20)     1073 2023-05-05 09:02:08.000000 packagebinbin-1.0.0/LICENSE
+-rw-r--r--   0 sher       (501) staff       (20)      585 2023-05-05 09:49:43.300327 packagebinbin-1.0.0/PKG-INFO
+-rw-r--r--   0 sher       (501) staff       (20)      172 2023-05-05 09:01:56.000000 packagebinbin-1.0.0/README.md
+drwxr-xr-x   0 sher       (501) staff       (20)        0 2023-05-05 09:49:43.299426 packagebinbin-1.0.0/packagebinbin.egg-info/
+-rw-r--r--   0 sher       (501) staff       (20)      585 2023-05-05 09:49:43.000000 packagebinbin-1.0.0/packagebinbin.egg-info/PKG-INFO
+-rw-r--r--   0 sher       (501) staff       (20)      261 2023-05-05 09:49:43.000000 packagebinbin-1.0.0/packagebinbin.egg-info/SOURCES.txt
+-rw-r--r--   0 sher       (501) staff       (20)        1 2023-05-05 09:49:43.000000 packagebinbin-1.0.0/packagebinbin.egg-info/dependency_links.txt
+-rw-r--r--   0 sher       (501) staff       (20)        9 2023-05-05 09:49:43.000000 packagebinbin-1.0.0/packagebinbin.egg-info/top_level.txt
+-rw-r--r--   0 sher       (501) staff       (20)      359 2023-05-05 09:49:07.000000 packagebinbin-1.0.0/pyproject.toml
+-rw-r--r--   0 sher       (501) staff       (20)       38 2023-05-05 09:49:43.300523 packagebinbin-1.0.0/setup.cfg
+-rw-r--r--   0 sher       (501) staff       (20)      791 2023-05-05 08:54:45.000000 packagebinbin-1.0.0/setup.py
+drwxr-xr-x   0 sher       (501) staff       (20)        0 2023-05-05 09:49:43.299560 packagebinbin-1.0.0/src/
+-rw-r--r--   0 sher       (501) staff       (20)       28 2023-05-05 09:48:04.000000 packagebinbin-1.0.0/src/__init__.py
+drwxr-xr-x   0 sher       (501) staff       (20)        0 2023-05-05 09:49:43.300029 packagebinbin-1.0.0/src/packagebinbin/
+-rw-r--r--   0 sher       (501) staff       (20)       21 2023-05-05 09:06:36.000000 packagebinbin-1.0.0/src/packagebinbin/__init__.py
+-rw-r--r--   0 sher       (501) staff       (20)      136 2023-05-05 08:59:11.000000 packagebinbin-1.0.0/src/packagebinbin/demo.py
```

### Comparing `packagebinbin-0.0.9/LICENSE` & `packagebinbin-1.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `packagebinbin-0.0.9/PKG-INFO` & `packagebinbin-1.0.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: packagebinbin
-Version: 0.0.9
+Version: 1.0.0
 Summary: A small example package
 Author: Sophat Chhay
 Author-email: Sophat Chhay <sophat.chhay@gmail.com>
 Keywords: python
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `packagebinbin-0.0.9/packagebinbin.egg-info/PKG-INFO` & `packagebinbin-1.0.0/packagebinbin.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: packagebinbin
-Version: 0.0.9
+Version: 1.0.0
 Summary: A small example package
 Author: Sophat Chhay
 Author-email: Sophat Chhay <sophat.chhay@gmail.com>
 Keywords: python
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `packagebinbin-0.0.9/setup.py` & `packagebinbin-1.0.0/setup.py`

 * *Files identical despite different names*

