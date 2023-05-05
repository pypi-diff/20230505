# Comparing `tmp/overlab-0.2.4-py3-none-any.whl.zip` & `tmp/overlab-0.2.5-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 15693 bytes, number of entries: 7
--rwxrwxrwx  2.0 unx       36 b- defN 23-Jan-31 23:06 overlab/__init__.py
--rwxrwxrwx  2.0 unx     5224 b- defN 23-Jan-31 23:06 overlab/overlab.py
--rwxrwxrwx  2.0 unx    34523 b- defN 23-Feb-02 09:38 overlab-0.2.4.dist-info/LICENSE.txt
--rwxrwxrwx  2.0 unx     2107 b- defN 23-Feb-02 09:38 overlab-0.2.4.dist-info/METADATA
--rwxrwxrwx  2.0 unx       92 b- defN 23-Feb-02 09:38 overlab-0.2.4.dist-info/WHEEL
--rwxrwxrwx  2.0 unx        8 b- defN 23-Feb-02 09:38 overlab-0.2.4.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      539 b- defN 23-Feb-02 09:38 overlab-0.2.4.dist-info/RECORD
-7 files, 42529 bytes uncompressed, 14739 bytes compressed:  65.3%
+Zip file size: 15695 bytes, number of entries: 7
+-rwxrwxrwx  2.0 unx       30 b- defN 23-May-05 11:01 overlab/__init__.py
+-rwxrwxrwx  2.0 unx     5225 b- defN 23-May-05 11:02 overlab/overlab.py
+-rwxrwxrwx  2.0 unx    34523 b- defN 23-May-05 11:03 overlab-0.2.5.dist-info/LICENSE.txt
+-rwxrwxrwx  2.0 unx     2107 b- defN 23-May-05 11:03 overlab-0.2.5.dist-info/METADATA
+-rwxrwxrwx  2.0 unx       92 b- defN 23-May-05 11:03 overlab-0.2.5.dist-info/WHEEL
+-rwxrwxrwx  2.0 unx        8 b- defN 23-May-05 11:03 overlab-0.2.5.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      539 b- defN 23-May-05 11:03 overlab-0.2.5.dist-info/RECORD
+7 files, 42524 bytes uncompressed, 14741 bytes compressed:  65.3%
```

## zipnote {}

```diff
@@ -1,22 +1,22 @@
 Filename: overlab/__init__.py
 Comment: 
 
 Filename: overlab/overlab.py
 Comment: 
 
-Filename: overlab-0.2.4.dist-info/LICENSE.txt
+Filename: overlab-0.2.5.dist-info/LICENSE.txt
 Comment: 
 
-Filename: overlab-0.2.4.dist-info/METADATA
+Filename: overlab-0.2.5.dist-info/METADATA
 Comment: 
 
-Filename: overlab-0.2.4.dist-info/WHEEL
+Filename: overlab-0.2.5.dist-info/WHEEL
 Comment: 
 
-Filename: overlab-0.2.4.dist-info/top_level.txt
+Filename: overlab-0.2.5.dist-info/top_level.txt
 Comment: 
 
-Filename: overlab-0.2.4.dist-info/RECORD
+Filename: overlab-0.2.5.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## overlab/__init__.py

```diff
@@ -1 +1 @@
-from overlab.overlab import overlab
+from .overlab import annotate
```

## overlab/overlab.py

```diff
@@ -1,12 +1,12 @@
 import matplotlib
 import numpy as np
 
 
-def overlab(x,y,list_of_annotations,ax,verbose=False,**kwargs):
+def annotate(x,y,list_of_annotations,ax,verbose=False,**kwargs):
     
     class Point:
         def __init__(self, x, y):
             self.x = x
             self.y = y
```

## Comparing `overlab-0.2.4.dist-info/LICENSE.txt` & `overlab-0.2.5.dist-info/LICENSE.txt`

 * *Files identical despite different names*

## Comparing `overlab-0.2.4.dist-info/METADATA` & `overlab-0.2.5.dist-info/METADATA`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: overlab
-Version: 0.2.4
+Version: 0.2.5
 Author: Francesco Gualdi
 License: GPL
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
 
 # overlab
```

