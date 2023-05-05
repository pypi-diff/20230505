# Comparing `tmp/binbinpy-1.0.2.tar.gz` & `tmp/binbinpy-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/Users/sher/Desktop/Sher/python/demopackage/dist/.tmp-c2dfpn1y/binbinpy-1.0.2.tar", last modified: Fri May  5 10:04:10 2023, max compression
+gzip compressed data, was "/Users/sher/Desktop/Sher/python/demopackage/dist/.tmp-muytr0ab/binbinpy-1.0.3.tar", last modified: Fri May  5 10:11:35 2023, max compression
```

## Comparing `binbinpy-1.0.2.tar` & `binbinpy-1.0.3.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 sher       (501) staff       (20)        0 2023-05-05 10:04:10.299306 binbinpy-1.0.2/
--rw-r--r--   0 sher       (501) staff       (20)     1073 2023-05-05 09:02:08.000000 binbinpy-1.0.2/LICENSE
--rw-r--r--   0 sher       (501) staff       (20)      580 2023-05-05 10:04:10.299128 binbinpy-1.0.2/PKG-INFO
--rw-r--r--   0 sher       (501) staff       (20)      172 2023-05-05 09:01:56.000000 binbinpy-1.0.2/README.md
-drwxr-xr-x   0 sher       (501) staff       (20)        0 2023-05-05 10:04:10.298196 binbinpy-1.0.2/binbinpy/
--rw-r--r--   0 sher       (501) staff       (20)       41 2023-05-05 10:02:31.000000 binbinpy-1.0.2/binbinpy/__init__.py
--rw-r--r--   0 sher       (501) staff       (20)      175 2023-05-05 10:01:02.000000 binbinpy-1.0.2/binbinpy/demo.py
-drwxr-xr-x   0 sher       (501) staff       (20)        0 2023-05-05 10:04:10.298955 binbinpy-1.0.2/binbinpy.egg-info/
--rw-r--r--   0 sher       (501) staff       (20)      580 2023-05-05 10:04:10.000000 binbinpy-1.0.2/binbinpy.egg-info/PKG-INFO
--rw-r--r--   0 sher       (501) staff       (20)      207 2023-05-05 10:04:10.000000 binbinpy-1.0.2/binbinpy.egg-info/SOURCES.txt
--rw-r--r--   0 sher       (501) staff       (20)        1 2023-05-05 10:04:10.000000 binbinpy-1.0.2/binbinpy.egg-info/dependency_links.txt
--rw-r--r--   0 sher       (501) staff       (20)       14 2023-05-05 10:04:10.000000 binbinpy-1.0.2/binbinpy.egg-info/top_level.txt
--rw-r--r--   0 sher       (501) staff       (20)      354 2023-05-05 10:03:13.000000 binbinpy-1.0.2/pyproject.toml
--rw-r--r--   0 sher       (501) staff       (20)       38 2023-05-05 10:04:10.299349 binbinpy-1.0.2/setup.cfg
--rw-r--r--   0 sher       (501) staff       (20)      786 2023-05-05 10:03:31.000000 binbinpy-1.0.2/setup.py
+drwxr-xr-x   0 sher       (501) staff       (20)        0 2023-05-05 10:11:35.076992 binbinpy-1.0.3/
+-rw-r--r--   0 sher       (501) staff       (20)     1073 2023-05-05 09:02:08.000000 binbinpy-1.0.3/LICENSE
+-rw-r--r--   0 sher       (501) staff       (20)      580 2023-05-05 10:11:35.076851 binbinpy-1.0.3/PKG-INFO
+-rw-r--r--   0 sher       (501) staff       (20)      172 2023-05-05 09:01:56.000000 binbinpy-1.0.3/README.md
+drwxr-xr-x   0 sher       (501) staff       (20)        0 2023-05-05 10:11:35.075961 binbinpy-1.0.3/binbinpy/
+-rw-r--r--   0 sher       (501) staff       (20)       41 2023-05-05 10:02:31.000000 binbinpy-1.0.3/binbinpy/__init__.py
+-rw-r--r--   0 sher       (501) staff       (20)      175 2023-05-05 10:01:02.000000 binbinpy-1.0.3/binbinpy/demo.py
+drwxr-xr-x   0 sher       (501) staff       (20)        0 2023-05-05 10:11:35.076690 binbinpy-1.0.3/binbinpy.egg-info/
+-rw-r--r--   0 sher       (501) staff       (20)      580 2023-05-05 10:11:35.000000 binbinpy-1.0.3/binbinpy.egg-info/PKG-INFO
+-rw-r--r--   0 sher       (501) staff       (20)      207 2023-05-05 10:11:35.000000 binbinpy-1.0.3/binbinpy.egg-info/SOURCES.txt
+-rw-r--r--   0 sher       (501) staff       (20)        1 2023-05-05 10:11:35.000000 binbinpy-1.0.3/binbinpy.egg-info/dependency_links.txt
+-rw-r--r--   0 sher       (501) staff       (20)       14 2023-05-05 10:11:35.000000 binbinpy-1.0.3/binbinpy.egg-info/top_level.txt
+-rw-r--r--   0 sher       (501) staff       (20)      354 2023-05-05 10:11:26.000000 binbinpy-1.0.3/pyproject.toml
+-rw-r--r--   0 sher       (501) staff       (20)       38 2023-05-05 10:11:35.077031 binbinpy-1.0.3/setup.cfg
+-rw-r--r--   0 sher       (501) staff       (20)      786 2023-05-05 10:03:31.000000 binbinpy-1.0.3/setup.py
```

### Comparing `binbinpy-1.0.2/LICENSE` & `binbinpy-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `binbinpy-1.0.2/PKG-INFO` & `binbinpy-1.0.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: binbinpy
-Version: 1.0.2
+Version: 1.0.3
 Summary: A small example package
 Author: Sophat Chhay
 Author-email: Sophat Chhay <sophat.chhay@gmail.com>
 Keywords: python
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `binbinpy-1.0.2/binbinpy.egg-info/PKG-INFO` & `binbinpy-1.0.3/binbinpy.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: binbinpy
-Version: 1.0.2
+Version: 1.0.3
 Summary: A small example package
 Author: Sophat Chhay
 Author-email: Sophat Chhay <sophat.chhay@gmail.com>
 Keywords: python
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `binbinpy-1.0.2/setup.py` & `binbinpy-1.0.3/setup.py`

 * *Files identical despite different names*

