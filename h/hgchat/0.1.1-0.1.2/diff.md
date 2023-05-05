# Comparing `tmp/hgchat-0.1.1.tar.gz` & `tmp/hgchat-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hgchat-0.1.1.tar", max compression
+gzip compressed data, was "hgchat-0.1.2.tar", max compression
```

## Comparing `hgchat-0.1.1.tar` & `hgchat-0.1.2.tar`

### file list

```diff
@@ -1,4 +1,4 @@
--rw-r--r--   0        0        0      683 2023-04-30 10:09:45.807393 hgchat-0.1.1/README.md
--rw-r--r--   0        0        0     2684 2023-05-04 23:28:08.663907 hgchat-0.1.1/hgchat/__init__.py
--rw-r--r--   0        0        0      409 2023-05-04 23:27:42.726826 hgchat-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     1052 1970-01-01 00:00:00.000000 hgchat-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0      683 2023-04-30 10:09:45.807393 hgchat-0.1.2/README.md
+-rw-r--r--   0        0        0     4031 2023-05-05 20:06:48.846991 hgchat-0.1.2/hgchat/__init__.py
+-rw-r--r--   0        0        0      438 2023-05-05 20:06:55.649969 hgchat-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     1102 1970-01-01 00:00:00.000000 hgchat-0.1.2/PKG-INFO
```

### Comparing `hgchat-0.1.1/README.md` & `hgchat-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `hgchat-0.1.1/PKG-INFO` & `hgchat-0.1.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 Metadata-Version: 2.1
 Name: hgchat
-Version: 0.1.1
+Version: 0.1.2
 Summary: 
 Author: 0xMRTT
 Author-email: 0xMRTT@proton.me
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: requests (>=2.29.0,<3.0.0)
+Requires-Dist: requests-toolbelt (>=1.0.0,<2.0.0)
 Description-Content-Type: text/markdown
 
 # Hugging Chat Python
 
 ## Installation
 
 ### As library
```

