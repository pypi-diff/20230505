# Comparing `tmp/coreftools-0.1.6-py3-none-any.whl.zip` & `tmp/coreftools-0.1.7-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 5367 bytes, number of entries: 6
+Zip file size: 5366 bytes, number of entries: 6
 -rw-r--r--  2.0 unx        0 b- defN 23-May-04 12:56 coreftools/__init__.py
 -rw-r--r--  2.0 unx     6996 b- defN 23-May-05 19:20 coreftools/corefresolvers.py
--rw-r--r--  2.0 unx     3653 b- defN 23-May-05 19:31 coreftools-0.1.6.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-May-05 19:31 coreftools-0.1.6.dist-info/WHEEL
--rw-r--r--  2.0 unx       11 b- defN 23-May-05 19:31 coreftools-0.1.6.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      471 b- defN 23-May-05 19:31 coreftools-0.1.6.dist-info/RECORD
-6 files, 11223 bytes uncompressed, 4509 bytes compressed:  59.8%
+-rw-r--r--  2.0 unx     3653 b- defN 23-May-05 19:42 coreftools-0.1.7.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-May-05 19:42 coreftools-0.1.7.dist-info/WHEEL
+-rw-r--r--  2.0 unx       11 b- defN 23-May-05 19:42 coreftools-0.1.7.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      471 b- defN 23-May-05 19:42 coreftools-0.1.7.dist-info/RECORD
+6 files, 11223 bytes uncompressed, 4508 bytes compressed:  59.8%
```

## zipnote {}

```diff
@@ -1,19 +1,19 @@
 Filename: coreftools/__init__.py
 Comment: 
 
 Filename: coreftools/corefresolvers.py
 Comment: 
 
-Filename: coreftools-0.1.6.dist-info/METADATA
+Filename: coreftools-0.1.7.dist-info/METADATA
 Comment: 
 
-Filename: coreftools-0.1.6.dist-info/WHEEL
+Filename: coreftools-0.1.7.dist-info/WHEEL
 Comment: 
 
-Filename: coreftools-0.1.6.dist-info/top_level.txt
+Filename: coreftools-0.1.7.dist-info/top_level.txt
 Comment: 
 
-Filename: coreftools-0.1.6.dist-info/RECORD
+Filename: coreftools-0.1.7.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `coreftools-0.1.6.dist-info/METADATA` & `coreftools-0.1.7.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: coreftools
-Version: 0.1.6
+Version: 0.1.7
 Summary: Coreference-Resolution library
 Download-URL: https://github.com/explosion/spacy-models/releases/download/en_core_web_sm-2.1.0/en_core_web_sm-2.1.0.tar.gz
 Author: Soumya-Ranjan-Sahoo
 License: MIT
 Description-Content-Type: text/markdown
 Requires-Dist: neuralcoref
 Requires-Dist: spacy (==2.1.0)
```

