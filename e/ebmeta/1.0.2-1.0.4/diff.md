# Comparing `tmp/ebmeta-1.0.2-py3-none-any.whl.zip` & `tmp/ebmeta-1.0.4-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,11 +1,11 @@
-Zip file size: 17428 bytes, number of entries: 9
+Zip file size: 17432 bytes, number of entries: 9
 -rw-r--r--  2.0 unx        0 b- defN 23-May-05 06:36 ebmeta/__init__.py
 -rw-r--r--  2.0 unx     4205 b- defN 23-May-05 06:36 ebmeta/cli.py
 -rw-r--r--  2.0 unx     3748 b- defN 22-Oct-28 03:41 ebmeta/isfdb.py
--rw-r--r--  2.0 unx    35149 b- defN 23-May-05 06:53 ebmeta-1.0.2.dist-info/LICENSE
--rw-r--r--  2.0 unx     3761 b- defN 23-May-05 06:53 ebmeta-1.0.2.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-May-05 06:53 ebmeta-1.0.2.dist-info/WHEEL
--rw-r--r--  2.0 unx       42 b- defN 23-May-05 06:53 ebmeta-1.0.2.dist-info/entry_points.txt
--rw-r--r--  2.0 unx        7 b- defN 23-May-05 06:53 ebmeta-1.0.2.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      689 b- defN 23-May-05 06:53 ebmeta-1.0.2.dist-info/RECORD
-9 files, 47693 bytes uncompressed, 16244 bytes compressed:  65.9%
+-rw-r--r--  2.0 unx    35149 b- defN 23-May-05 07:11 ebmeta-1.0.4.dist-info/LICENSE
+-rw-r--r--  2.0 unx     3769 b- defN 23-May-05 07:11 ebmeta-1.0.4.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-May-05 07:11 ebmeta-1.0.4.dist-info/WHEEL
+-rw-r--r--  2.0 unx       42 b- defN 23-May-05 07:11 ebmeta-1.0.4.dist-info/entry_points.txt
+-rw-r--r--  2.0 unx        7 b- defN 23-May-05 07:11 ebmeta-1.0.4.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      689 b- defN 23-May-05 07:11 ebmeta-1.0.4.dist-info/RECORD
+9 files, 47701 bytes uncompressed, 16248 bytes compressed:  65.9%
```

## zipnote {}

```diff
@@ -3,26 +3,26 @@
 
 Filename: ebmeta/cli.py
 Comment: 
 
 Filename: ebmeta/isfdb.py
 Comment: 
 
-Filename: ebmeta-1.0.2.dist-info/LICENSE
+Filename: ebmeta-1.0.4.dist-info/LICENSE
 Comment: 
 
-Filename: ebmeta-1.0.2.dist-info/METADATA
+Filename: ebmeta-1.0.4.dist-info/METADATA
 Comment: 
 
-Filename: ebmeta-1.0.2.dist-info/WHEEL
+Filename: ebmeta-1.0.4.dist-info/WHEEL
 Comment: 
 
-Filename: ebmeta-1.0.2.dist-info/entry_points.txt
+Filename: ebmeta-1.0.4.dist-info/entry_points.txt
 Comment: 
 
-Filename: ebmeta-1.0.2.dist-info/top_level.txt
+Filename: ebmeta-1.0.4.dist-info/top_level.txt
 Comment: 
 
-Filename: ebmeta-1.0.2.dist-info/RECORD
+Filename: ebmeta-1.0.4.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `ebmeta-1.0.2.dist-info/LICENSE` & `ebmeta-1.0.4.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `ebmeta-1.0.2.dist-info/METADATA` & `ebmeta-1.0.4.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 Metadata-Version: 2.1
 Name: ebmeta
-Version: 1.0.2
-Summary: Ebook Metadata CLI
+Version: 1.0.4
+Summary: Ebook Metadata Munging CLI
 Home-page: http://github.com/pjz/ebmeta
 Author: Paul Jimenez
 Author-email: pj@place.org
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: System Administrators
```

## Comparing `ebmeta-1.0.2.dist-info/RECORD` & `ebmeta-1.0.4.dist-info/RECORD`

 * *Files 22% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 ebmeta/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 ebmeta/cli.py,sha256=UB1KPUC8YfN4rWqLmvp52NjPaeNA1YDwe5-sv1BLdp4,4205
 ebmeta/isfdb.py,sha256=nIaNW2Mo8GTypblagEG__WwEof-AsUQw8fZiQL9aoD0,3748
-ebmeta-1.0.2.dist-info/LICENSE,sha256=OXLcl0T2SZ8Pmy2_dmlvKuetivmyPd5m1q-Gyd-zaYY,35149
-ebmeta-1.0.2.dist-info/METADATA,sha256=BpKTtFPs9FdyDnIXGYWb1poNemCD5HzFf7dtUZPlJag,3761
-ebmeta-1.0.2.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
-ebmeta-1.0.2.dist-info/entry_points.txt,sha256=SqmnFkd8Mq1fTp28PMF2VsCtXgMNKv0jiVKM5Pl38fE,42
-ebmeta-1.0.2.dist-info/top_level.txt,sha256=xFuWv_sTDv3xIEgoU25WD1VvU8d4dbRJFHAfbJUDWsE,7
-ebmeta-1.0.2.dist-info/RECORD,,
+ebmeta-1.0.4.dist-info/LICENSE,sha256=OXLcl0T2SZ8Pmy2_dmlvKuetivmyPd5m1q-Gyd-zaYY,35149
+ebmeta-1.0.4.dist-info/METADATA,sha256=np53tkSuGwFpNADbuFp-8N9-j6yad3j42INXycSjKwo,3769
+ebmeta-1.0.4.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
+ebmeta-1.0.4.dist-info/entry_points.txt,sha256=SqmnFkd8Mq1fTp28PMF2VsCtXgMNKv0jiVKM5Pl38fE,42
+ebmeta-1.0.4.dist-info/top_level.txt,sha256=xFuWv_sTDv3xIEgoU25WD1VvU8d4dbRJFHAfbJUDWsE,7
+ebmeta-1.0.4.dist-info/RECORD,,
```

