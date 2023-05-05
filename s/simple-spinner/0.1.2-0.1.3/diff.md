# Comparing `tmp/simple_spinner-0.1.2-py3-none-any.whl.zip` & `tmp/simple_spinner-0.1.3-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 2716 bytes, number of entries: 6
--rw-r--r--  2.0 unx       21 b- defN 23-May-05 02:53 simple_spinner/__init__.py
+Zip file size: 2717 bytes, number of entries: 6
+-rw-r--r--  2.0 unx       28 b- defN 23-May-05 03:04 simple_spinner/__init__.py
 -rw-r--r--  2.0 unx     2022 b- defN 23-May-04 12:37 simple_spinner/spinner.py
--rw-r--r--  2.0 unx     1283 b- defN 23-May-05 02:55 simple_spinner-0.1.2.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-May-05 02:55 simple_spinner-0.1.2.dist-info/WHEEL
--rw-r--r--  2.0 unx       15 b- defN 23-May-05 02:55 simple_spinner-0.1.2.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      489 b- defN 23-May-05 02:55 simple_spinner-0.1.2.dist-info/RECORD
-6 files, 3922 bytes uncompressed, 1824 bytes compressed:  53.5%
+-rw-r--r--  2.0 unx     1283 b- defN 23-May-05 03:05 simple_spinner-0.1.3.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-May-05 03:05 simple_spinner-0.1.3.dist-info/WHEEL
+-rw-r--r--  2.0 unx       15 b- defN 23-May-05 03:05 simple_spinner-0.1.3.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      489 b- defN 23-May-05 03:05 simple_spinner-0.1.3.dist-info/RECORD
+6 files, 3929 bytes uncompressed, 1825 bytes compressed:  53.6%
```

## zipnote {}

```diff
@@ -1,19 +1,19 @@
 Filename: simple_spinner/__init__.py
 Comment: 
 
 Filename: simple_spinner/spinner.py
 Comment: 
 
-Filename: simple_spinner-0.1.2.dist-info/METADATA
+Filename: simple_spinner-0.1.3.dist-info/METADATA
 Comment: 
 
-Filename: simple_spinner-0.1.2.dist-info/WHEEL
+Filename: simple_spinner-0.1.3.dist-info/WHEEL
 Comment: 
 
-Filename: simple_spinner-0.1.2.dist-info/top_level.txt
+Filename: simple_spinner-0.1.3.dist-info/top_level.txt
 Comment: 
 
-Filename: simple_spinner-0.1.2.dist-info/RECORD
+Filename: simple_spinner-0.1.3.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## simple_spinner/__init__.py

```diff
@@ -1 +1 @@
-from . import spinner
+from .spinner import Spinner
```

## Comparing `simple_spinner-0.1.2.dist-info/METADATA` & `simple_spinner-0.1.3.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: simple-spinner
-Version: 0.1.2
+Version: 0.1.3
 Summary: Simple Spinner in python
 Home-page: https://github.com/wooy0ng/simple_spinner
 Author: wooy0ng
 Author-email: yygg9800@naver.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: simple-spinner Version: 0.1.2 Summary: Simple
+Metadata-Version: 2.1 Name: simple-spinner Version: 0.1.3 Summary: Simple
 Spinner in python Home-page: https://github.com/wooy0ng/simple_spinner Author:
 wooy0ng Author-email: yygg9800@naver.com License: UNKNOWN Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3 Classifier: License :: OSI
 Approved :: MIT License Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8 Description-Content-Type: text/markdown
                          ****** Simple Spinner ******
  [https://user-images.githubusercontent.com/37149278/236219276-9553b362-3232-
```

