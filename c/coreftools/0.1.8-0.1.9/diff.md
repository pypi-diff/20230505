# Comparing `tmp/coreftools-0.1.8-py3-none-any.whl.zip` & `tmp/coreftools-0.1.9-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 5369 bytes, number of entries: 6
+Zip file size: 5371 bytes, number of entries: 6
 -rw-r--r--  2.0 unx        0 b- defN 23-May-04 12:56 coreftools/__init__.py
 -rw-r--r--  2.0 unx     6996 b- defN 23-May-05 19:20 coreftools/corefresolvers.py
--rw-r--r--  2.0 unx     3676 b- defN 23-May-05 19:52 coreftools-0.1.8.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-May-05 19:52 coreftools-0.1.8.dist-info/WHEEL
--rw-r--r--  2.0 unx       11 b- defN 23-May-05 19:52 coreftools-0.1.8.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      471 b- defN 23-May-05 19:52 coreftools-0.1.8.dist-info/RECORD
-6 files, 11246 bytes uncompressed, 4511 bytes compressed:  59.9%
+-rw-r--r--  2.0 unx     3676 b- defN 23-May-05 19:57 coreftools-0.1.9.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-May-05 19:57 coreftools-0.1.9.dist-info/WHEEL
+-rw-r--r--  2.0 unx       11 b- defN 23-May-05 19:57 coreftools-0.1.9.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      471 b- defN 23-May-05 19:57 coreftools-0.1.9.dist-info/RECORD
+6 files, 11246 bytes uncompressed, 4513 bytes compressed:  59.9%
```

## zipnote {}

```diff
@@ -1,19 +1,19 @@
 Filename: coreftools/__init__.py
 Comment: 
 
 Filename: coreftools/corefresolvers.py
 Comment: 
 
-Filename: coreftools-0.1.8.dist-info/METADATA
+Filename: coreftools-0.1.9.dist-info/METADATA
 Comment: 
 
-Filename: coreftools-0.1.8.dist-info/WHEEL
+Filename: coreftools-0.1.9.dist-info/WHEEL
 Comment: 
 
-Filename: coreftools-0.1.8.dist-info/top_level.txt
+Filename: coreftools-0.1.9.dist-info/top_level.txt
 Comment: 
 
-Filename: coreftools-0.1.8.dist-info/RECORD
+Filename: coreftools-0.1.9.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `coreftools-0.1.8.dist-info/METADATA` & `coreftools-0.1.9.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: coreftools
-Version: 0.1.8
+Version: 0.1.9
 Summary: Coreference-Resolution library
 Download-URL: https://github.com/explosion/spacy-models/releases/download/en_core_web_sm-2.1.0/en_core_web_sm-2.1.0.tar.gz
 Author: Soumya-Ranjan-Sahoo
 License: MIT
 Description-Content-Type: text/markdown
 Requires-Dist: neuralcoref
 Requires-Dist: spacy (==2.1.0)
```

