# Comparing `tmp/avclass-malicialab-2.8.0.tar.gz` & `tmp/avclass-malicialab-2.8.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "avclass-malicialab-2.8.0.tar", last modified: Mon Apr 10 14:58:13 2023, max compression
+gzip compressed data, was "avclass-malicialab-2.8.1.tar", last modified: Fri May  5 14:58:44 2023, max compression
```

## Comparing `avclass-malicialab-2.8.0.tar` & `avclass-malicialab-2.8.1.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxrwxr-x   0 juanca    (1000) juanca    (1000)        0 2023-04-10 14:58:13.194088 avclass-malicialab-2.8.0/
--rw-rw-r--   0 juanca    (1000) juanca    (1000)     1100 2020-09-01 17:16:19.000000 avclass-malicialab-2.8.0/LICENSE
--rw-rw-r--   0 juanca    (1000) juanca    (1000)       23 2023-02-23 10:39:34.000000 avclass-malicialab-2.8.0/MANIFEST.in
--rw-rw-r--   0 juanca    (1000) juanca    (1000)    17117 2023-04-10 14:58:13.194088 avclass-malicialab-2.8.0/PKG-INFO
--rw-rw-r--   0 juanca    (1000) juanca    (1000)    15317 2023-04-10 14:11:52.000000 avclass-malicialab-2.8.0/README.md
-drwxrwxr-x   0 juanca    (1000) juanca    (1000)        0 2023-04-10 14:58:13.194088 avclass-malicialab-2.8.0/avclass/
--rw-rw-r--   0 juanca    (1000) juanca    (1000)      401 2023-02-23 10:09:56.000000 avclass-malicialab-2.8.0/avclass/__init__.py
--rw-rw-r--   0 juanca    (1000) juanca    (1000)    20210 2023-03-23 08:28:38.000000 avclass-malicialab-2.8.0/avclass/common.py
-drwxrwxr-x   0 juanca    (1000) juanca    (1000)        0 2023-04-10 14:58:13.194088 avclass-malicialab-2.8.0/avclass/data/
--rw-rw-r--   0 juanca    (1000) juanca    (1000)     6823 2023-02-23 10:09:56.000000 avclass-malicialab-2.8.0/avclass/data/andropup.expansion
--rw-rw-r--   0 juanca    (1000) juanca    (1000)      308 2023-04-10 14:08:05.000000 avclass-malicialab-2.8.0/avclass/data/default.expansion
--rw-rw-r--   0 juanca    (1000) juanca    (1000)    56429 2023-04-10 14:08:05.000000 avclass-malicialab-2.8.0/avclass/data/default.tagging
--rw-rw-r--   0 juanca    (1000) juanca    (1000)    41254 2023-04-10 14:08:05.000000 avclass-malicialab-2.8.0/avclass/data/default.taxonomy
--rwxrwxr-x   0 juanca    (1000) juanca    (1000)     4202 2023-02-26 07:44:35.000000 avclass-malicialab-2.8.0/avclass/evaluate.py
--rwxrwxr-x   0 juanca    (1000) juanca    (1000)    23606 2023-02-27 10:51:54.000000 avclass-malicialab-2.8.0/avclass/labeler.py
--rwxrwxr-x   0 juanca    (1000) juanca    (1000)     3996 2023-03-04 13:05:26.000000 avclass-malicialab-2.8.0/avclass/misp.py
--rwxrwxr-x   0 juanca    (1000) juanca    (1000)     1704 2023-02-26 07:00:49.000000 avclass-malicialab-2.8.0/avclass/normalize.py
--rwxrwxr-x   0 juanca    (1000) juanca    (1000)    17636 2023-02-23 10:26:36.000000 avclass-malicialab-2.8.0/avclass/update.py
-drwxrwxr-x   0 juanca    (1000) juanca    (1000)        0 2023-04-10 14:58:13.194088 avclass-malicialab-2.8.0/avclass_malicialab.egg-info/
--rw-rw-r--   0 juanca    (1000) juanca    (1000)    17117 2023-04-10 14:58:13.000000 avclass-malicialab-2.8.0/avclass_malicialab.egg-info/PKG-INFO
--rw-rw-r--   0 juanca    (1000) juanca    (1000)      511 2023-04-10 14:58:13.000000 avclass-malicialab-2.8.0/avclass_malicialab.egg-info/SOURCES.txt
--rw-rw-r--   0 juanca    (1000) juanca    (1000)        1 2023-04-10 14:58:13.000000 avclass-malicialab-2.8.0/avclass_malicialab.egg-info/dependency_links.txt
--rw-rw-r--   0 juanca    (1000) juanca    (1000)      162 2023-04-10 14:58:13.000000 avclass-malicialab-2.8.0/avclass_malicialab.egg-info/entry_points.txt
--rw-rw-r--   0 juanca    (1000) juanca    (1000)        8 2023-04-10 14:58:13.000000 avclass-malicialab-2.8.0/avclass_malicialab.egg-info/top_level.txt
--rw-rw-r--   0 juanca    (1000) juanca    (1000)      831 2023-04-10 14:09:05.000000 avclass-malicialab-2.8.0/pyproject.toml
--rw-rw-r--   0 juanca    (1000) juanca    (1000)       38 2023-04-10 14:58:13.194088 avclass-malicialab-2.8.0/setup.cfg
+drwxrwxr-x   0 juanca    (1000) juanca    (1000)        0 2023-05-05 14:58:44.534130 avclass-malicialab-2.8.1/
+-rw-rw-r--   0 juanca    (1000) juanca    (1000)     1100 2020-09-01 17:16:19.000000 avclass-malicialab-2.8.1/LICENSE
+-rw-rw-r--   0 juanca    (1000) juanca    (1000)       23 2023-02-23 10:39:34.000000 avclass-malicialab-2.8.1/MANIFEST.in
+-rw-rw-r--   0 juanca    (1000) juanca    (1000)    17117 2023-05-05 14:58:44.534130 avclass-malicialab-2.8.1/PKG-INFO
+-rw-rw-r--   0 juanca    (1000) juanca    (1000)    15317 2023-04-10 14:11:52.000000 avclass-malicialab-2.8.1/README.md
+drwxrwxr-x   0 juanca    (1000) juanca    (1000)        0 2023-05-05 14:58:44.530130 avclass-malicialab-2.8.1/avclass/
+-rw-rw-r--   0 juanca    (1000) juanca    (1000)      401 2023-02-23 10:09:56.000000 avclass-malicialab-2.8.1/avclass/__init__.py
+-rw-rw-r--   0 juanca    (1000) juanca    (1000)    20578 2023-05-05 14:49:38.000000 avclass-malicialab-2.8.1/avclass/common.py
+drwxrwxr-x   0 juanca    (1000) juanca    (1000)        0 2023-05-05 14:58:44.534130 avclass-malicialab-2.8.1/avclass/data/
+-rw-rw-r--   0 juanca    (1000) juanca    (1000)     6823 2023-02-23 10:09:56.000000 avclass-malicialab-2.8.1/avclass/data/andropup.expansion
+-rw-rw-r--   0 juanca    (1000) juanca    (1000)      308 2023-04-10 14:08:05.000000 avclass-malicialab-2.8.1/avclass/data/default.expansion
+-rw-rw-r--   0 juanca    (1000) juanca    (1000)    56429 2023-04-10 14:08:05.000000 avclass-malicialab-2.8.1/avclass/data/default.tagging
+-rw-rw-r--   0 juanca    (1000) juanca    (1000)    41254 2023-04-10 14:08:05.000000 avclass-malicialab-2.8.1/avclass/data/default.taxonomy
+-rwxrwxr-x   0 juanca    (1000) juanca    (1000)     4202 2023-02-26 07:44:35.000000 avclass-malicialab-2.8.1/avclass/evaluate.py
+-rwxrwxr-x   0 juanca    (1000) juanca    (1000)    23606 2023-02-27 10:51:54.000000 avclass-malicialab-2.8.1/avclass/labeler.py
+-rwxrwxr-x   0 juanca    (1000) juanca    (1000)     3996 2023-03-04 13:05:26.000000 avclass-malicialab-2.8.1/avclass/misp.py
+-rwxrwxr-x   0 juanca    (1000) juanca    (1000)     1704 2023-02-26 07:00:49.000000 avclass-malicialab-2.8.1/avclass/normalize.py
+-rwxrwxr-x   0 juanca    (1000) juanca    (1000)    17636 2023-02-23 10:26:36.000000 avclass-malicialab-2.8.1/avclass/update.py
+drwxrwxr-x   0 juanca    (1000) juanca    (1000)        0 2023-05-05 14:58:44.534130 avclass-malicialab-2.8.1/avclass_malicialab.egg-info/
+-rw-rw-r--   0 juanca    (1000) juanca    (1000)    17117 2023-05-05 14:58:44.000000 avclass-malicialab-2.8.1/avclass_malicialab.egg-info/PKG-INFO
+-rw-rw-r--   0 juanca    (1000) juanca    (1000)      511 2023-05-05 14:58:44.000000 avclass-malicialab-2.8.1/avclass_malicialab.egg-info/SOURCES.txt
+-rw-rw-r--   0 juanca    (1000) juanca    (1000)        1 2023-05-05 14:58:44.000000 avclass-malicialab-2.8.1/avclass_malicialab.egg-info/dependency_links.txt
+-rw-rw-r--   0 juanca    (1000) juanca    (1000)      162 2023-05-05 14:58:44.000000 avclass-malicialab-2.8.1/avclass_malicialab.egg-info/entry_points.txt
+-rw-rw-r--   0 juanca    (1000) juanca    (1000)        8 2023-05-05 14:58:44.000000 avclass-malicialab-2.8.1/avclass_malicialab.egg-info/top_level.txt
+-rw-rw-r--   0 juanca    (1000) juanca    (1000)      831 2023-05-05 14:56:52.000000 avclass-malicialab-2.8.1/pyproject.toml
+-rw-rw-r--   0 juanca    (1000) juanca    (1000)       38 2023-05-05 14:58:44.534130 avclass-malicialab-2.8.1/setup.cfg
```

### Comparing `avclass-malicialab-2.8.0/LICENSE` & `avclass-malicialab-2.8.1/LICENSE`

 * *Files identical despite different names*

### Comparing `avclass-malicialab-2.8.0/PKG-INFO` & `avclass-malicialab-2.8.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: avclass-malicialab
-Version: 2.8.0
+Version: 2.8.1
 Summary: AVClass is a Python package and command line tool to tag / label malware samples.
 Author: MaliciaLab
 License: MIT License
         
         Copyright (c) 2016-2020 MaliciaLab @ IMDEA Software Institute
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `avclass-malicialab-2.8.0/README.md` & `avclass-malicialab-2.8.1/README.md`

 * *Files identical despite different names*

### Comparing `avclass-malicialab-2.8.0/avclass/common.py` & `avclass-malicialab-2.8.1/avclass/common.py`

 * *Files 2% similar despite different names*

```diff
@@ -622,7 +622,18 @@
         else:
             cnt = 0
             for (av_name, label) in sample_info.labels:
                 if av_name in self.avs:
                     cnt += 1
             return cnt
 
+    def get_family_from_label(self, label):
+        """Return family from given label, or None if no family found"""
+        fam = None
+        tags = self.get_label_tags(label, [])
+        for t in tags:
+            cat = self.taxonomy.get_category(t)
+            if (cat == "UNK") or (cat == "FAM"):
+                fam = t
+                break
+        return fam
+
```

### Comparing `avclass-malicialab-2.8.0/avclass/data/andropup.expansion` & `avclass-malicialab-2.8.1/avclass/data/andropup.expansion`

 * *Files identical despite different names*

### Comparing `avclass-malicialab-2.8.0/avclass/data/default.tagging` & `avclass-malicialab-2.8.1/avclass/data/default.tagging`

 * *Files identical despite different names*

### Comparing `avclass-malicialab-2.8.0/avclass/data/default.taxonomy` & `avclass-malicialab-2.8.1/avclass/data/default.taxonomy`

 * *Files identical despite different names*

### Comparing `avclass-malicialab-2.8.0/avclass/evaluate.py` & `avclass-malicialab-2.8.1/avclass/evaluate.py`

 * *Files identical despite different names*

### Comparing `avclass-malicialab-2.8.0/avclass/labeler.py` & `avclass-malicialab-2.8.1/avclass/labeler.py`

 * *Files identical despite different names*

### Comparing `avclass-malicialab-2.8.0/avclass/misp.py` & `avclass-malicialab-2.8.1/avclass/misp.py`

 * *Files identical despite different names*

### Comparing `avclass-malicialab-2.8.0/avclass/normalize.py` & `avclass-malicialab-2.8.1/avclass/normalize.py`

 * *Files identical despite different names*

### Comparing `avclass-malicialab-2.8.0/avclass/update.py` & `avclass-malicialab-2.8.1/avclass/update.py`

 * *Files identical despite different names*

### Comparing `avclass-malicialab-2.8.0/avclass_malicialab.egg-info/PKG-INFO` & `avclass-malicialab-2.8.1/avclass_malicialab.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: avclass-malicialab
-Version: 2.8.0
+Version: 2.8.1
 Summary: AVClass is a Python package and command line tool to tag / label malware samples.
 Author: MaliciaLab
 License: MIT License
         
         Copyright (c) 2016-2020 MaliciaLab @ IMDEA Software Institute
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `avclass-malicialab-2.8.0/pyproject.toml` & `avclass-malicialab-2.8.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires      = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "avclass-malicialab"
-version = "2.8.0"
+version = "2.8.1"
 description = "AVClass is a Python package and command line tool to tag / label malware samples."
 readme = "README.md"
 authors = [{ name = "MaliciaLab" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
```

