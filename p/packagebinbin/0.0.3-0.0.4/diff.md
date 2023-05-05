# Comparing `tmp/packagebinbin-0.0.3.tar.gz` & `tmp/packagebinbin-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/packagebinbin-0.0.3.tar", last modified: Fri May  5 08:39:35 2023, max compression
+gzip compressed data, was "dist/packagebinbin-0.0.4.tar", last modified: Fri May  5 08:41:31 2023, max compression
```

## Comparing `packagebinbin-0.0.3.tar` & `packagebinbin-0.0.4.tar`

### file list

```diff
@@ -1,9 +1,9 @@
-drwxr-xr-x   0 sher       (501) staff       (20)        0 2023-05-05 08:39:35.633092 packagebinbin-0.0.3/
--rw-r--r--   0 sher       (501) staff       (20)      581 2023-05-05 08:39:35.632966 packagebinbin-0.0.3/PKG-INFO
-drwxr-xr-x   0 sher       (501) staff       (20)        0 2023-05-05 08:39:35.632793 packagebinbin-0.0.3/packagebinbin.egg-info/
--rw-r--r--   0 sher       (501) staff       (20)      581 2023-05-05 08:39:35.000000 packagebinbin-0.0.3/packagebinbin.egg-info/PKG-INFO
--rw-r--r--   0 sher       (501) staff       (20)      156 2023-05-05 08:39:35.000000 packagebinbin-0.0.3/packagebinbin.egg-info/SOURCES.txt
--rw-r--r--   0 sher       (501) staff       (20)        1 2023-05-05 08:39:35.000000 packagebinbin-0.0.3/packagebinbin.egg-info/dependency_links.txt
--rw-r--r--   0 sher       (501) staff       (20)        1 2023-05-05 08:39:35.000000 packagebinbin-0.0.3/packagebinbin.egg-info/top_level.txt
--rw-r--r--   0 sher       (501) staff       (20)       38 2023-05-05 08:39:35.633138 packagebinbin-0.0.3/setup.cfg
--rw-r--r--   0 sher       (501) staff       (20)      766 2023-05-05 08:39:31.000000 packagebinbin-0.0.3/setup.py
+drwxr-xr-x   0 sher       (501) staff       (20)        0 2023-05-05 08:41:31.959061 packagebinbin-0.0.4/
+-rw-r--r--   0 sher       (501) staff       (20)      581 2023-05-05 08:41:31.958897 packagebinbin-0.0.4/PKG-INFO
+drwxr-xr-x   0 sher       (501) staff       (20)        0 2023-05-05 08:41:31.958698 packagebinbin-0.0.4/packagebinbin.egg-info/
+-rw-r--r--   0 sher       (501) staff       (20)      581 2023-05-05 08:41:31.000000 packagebinbin-0.0.4/packagebinbin.egg-info/PKG-INFO
+-rw-r--r--   0 sher       (501) staff       (20)      156 2023-05-05 08:41:31.000000 packagebinbin-0.0.4/packagebinbin.egg-info/SOURCES.txt
+-rw-r--r--   0 sher       (501) staff       (20)        1 2023-05-05 08:41:31.000000 packagebinbin-0.0.4/packagebinbin.egg-info/dependency_links.txt
+-rw-r--r--   0 sher       (501) staff       (20)        1 2023-05-05 08:41:31.000000 packagebinbin-0.0.4/packagebinbin.egg-info/top_level.txt
+-rw-r--r--   0 sher       (501) staff       (20)       38 2023-05-05 08:41:31.959106 packagebinbin-0.0.4/setup.cfg
+-rw-r--r--   0 sher       (501) staff       (20)      766 2023-05-05 08:41:28.000000 packagebinbin-0.0.4/setup.py
```

### Comparing `packagebinbin-0.0.3/PKG-INFO` & `packagebinbin-0.0.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: packagebinbin
-Version: 0.0.3
+Version: 0.0.4
 Summary: My demo package with my daughter name
 Author: Sophat Chhay
 Author-email: <sophat.chhay@gmail.com>
 Keywords: python
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `packagebinbin-0.0.3/packagebinbin.egg-info/PKG-INFO` & `packagebinbin-0.0.4/packagebinbin.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: packagebinbin
-Version: 0.0.3
+Version: 0.0.4
 Summary: My demo package with my daughter name
 Author: Sophat Chhay
 Author-email: <sophat.chhay@gmail.com>
 Keywords: python
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

