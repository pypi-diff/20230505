# Comparing `tmp/pants_py_deploy-0.0.15rc6-py3-none-any.whl.zip` & `tmp/pants_py_deploy-0.0.15rc7-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,14 +1,14 @@
-Zip file size: 10918 bytes, number of entries: 12
--rw-r--r--  2.0 unx        0 b- defN 23-May-05 09:20 pants_py_deploy/__init__.py
--rw-r--r--  2.0 unx     4618 b- defN 23-May-05 09:20 pants_py_deploy/compose_file.py
--rw-r--r--  2.0 unx     7083 b- defN 23-May-05 09:20 pants_py_deploy/export_env.py
--rw-r--r--  2.0 unx      606 b- defN 23-May-05 09:20 pants_py_deploy/fields.py
--rw-r--r--  2.0 unx     3534 b- defN 23-May-05 09:20 pants_py_deploy/models.py
--rw-r--r--  2.0 unx    10014 b- defN 23-May-05 09:20 pants_py_deploy/plugin.py
--rw-r--r--  2.0 unx      482 b- defN 23-May-05 09:20 pants_py_deploy/register.py
--rw-r--r--  2.0 unx     2256 b- defN 23-May-05 09:20 pants_py_deploy-0.0.15rc6.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-May-05 09:20 pants_py_deploy-0.0.15rc6.dist-info/WHEEL
--rw-r--r--  2.0 unx        1 b- defN 23-May-05 09:20 pants_py_deploy-0.0.15rc6.dist-info/namespace_packages.txt
--rw-r--r--  2.0 unx       16 b- defN 23-May-05 09:20 pants_py_deploy-0.0.15rc6.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     1042 b- defN 23-May-05 09:20 pants_py_deploy-0.0.15rc6.dist-info/RECORD
-12 files, 29744 bytes uncompressed, 9138 bytes compressed:  69.3%
+Zip file size: 10919 bytes, number of entries: 12
+-rw-r--r--  2.0 unx        0 b- defN 23-May-05 10:10 pants_py_deploy/__init__.py
+-rw-r--r--  2.0 unx     4618 b- defN 23-May-05 10:10 pants_py_deploy/compose_file.py
+-rw-r--r--  2.0 unx     7083 b- defN 23-May-05 10:10 pants_py_deploy/export_env.py
+-rw-r--r--  2.0 unx      606 b- defN 23-May-05 10:10 pants_py_deploy/fields.py
+-rw-r--r--  2.0 unx     3534 b- defN 23-May-05 10:10 pants_py_deploy/models.py
+-rw-r--r--  2.0 unx    10014 b- defN 23-May-05 10:10 pants_py_deploy/plugin.py
+-rw-r--r--  2.0 unx      482 b- defN 23-May-05 10:10 pants_py_deploy/register.py
+-rw-r--r--  2.0 unx     2256 b- defN 23-May-05 10:10 pants_py_deploy-0.0.15rc7.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-May-05 10:10 pants_py_deploy-0.0.15rc7.dist-info/WHEEL
+-rw-r--r--  2.0 unx        1 b- defN 23-May-05 10:10 pants_py_deploy-0.0.15rc7.dist-info/namespace_packages.txt
+-rw-r--r--  2.0 unx       16 b- defN 23-May-05 10:10 pants_py_deploy-0.0.15rc7.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     1042 b- defN 23-May-05 10:10 pants_py_deploy-0.0.15rc7.dist-info/RECORD
+12 files, 29744 bytes uncompressed, 9139 bytes compressed:  69.3%
```

## zipnote {}

```diff
@@ -15,23 +15,23 @@
 
 Filename: pants_py_deploy/plugin.py
 Comment: 
 
 Filename: pants_py_deploy/register.py
 Comment: 
 
-Filename: pants_py_deploy-0.0.15rc6.dist-info/METADATA
+Filename: pants_py_deploy-0.0.15rc7.dist-info/METADATA
 Comment: 
 
-Filename: pants_py_deploy-0.0.15rc6.dist-info/WHEEL
+Filename: pants_py_deploy-0.0.15rc7.dist-info/WHEEL
 Comment: 
 
-Filename: pants_py_deploy-0.0.15rc6.dist-info/namespace_packages.txt
+Filename: pants_py_deploy-0.0.15rc7.dist-info/namespace_packages.txt
 Comment: 
 
-Filename: pants_py_deploy-0.0.15rc6.dist-info/top_level.txt
+Filename: pants_py_deploy-0.0.15rc7.dist-info/top_level.txt
 Comment: 
 
-Filename: pants_py_deploy-0.0.15rc6.dist-info/RECORD
+Filename: pants_py_deploy-0.0.15rc7.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `pants_py_deploy-0.0.15rc6.dist-info/METADATA` & `pants_py_deploy-0.0.15rc7.dist-info/METADATA`

 * *Files 4% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: pants-py-deploy
-Version: 0.0.15rc6
+Version: 0.0.15rc7
 Summary: Make it easy to maintain docker-compose files and helm-charts across projects with pants-py-deploy
 Home-page: https://github.com/EspenAlbert/py-libs
 Author: Espen Albert
 License: MIT
 Classifier: Programming Language :: Python :: 3.9
 Requires-Python: <3.10,>=3.9
 Description-Content-Type: text/markdown
-Requires-Dist: compose-chart-export (==0.0.15rc2)
+Requires-Dist: compose-chart-export (==0.0.15rc4)
 Requires-Dist: docker-compose-parser (==0.0.15)
 Requires-Dist: model-lib (==0.0.15)
 Requires-Dist: pantsbuild.pants (<2.17,>=2.16.0a0)
 Requires-Dist: zero-3rdparty (==0.0.15)
 
 # Pants py_deploy plugin
 - Purpose: Make it easy to maintain docker-compose files and helm-charts across projects
```

## Comparing `pants_py_deploy-0.0.15rc6.dist-info/RECORD` & `pants_py_deploy-0.0.15rc7.dist-info/RECORD`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 pants_py_deploy/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 pants_py_deploy/compose_file.py,sha256=kl6m34S_tdU1SxirGM5FEasPeqqjb_jUndwA2AQBO4c,4618
 pants_py_deploy/export_env.py,sha256=z0a7Sa2Lc4_7cFf9oH7rdoHjUqHgU-e6oshAQ9bm1Yg,7083
 pants_py_deploy/fields.py,sha256=entMoIWLwKiEwOBBr54Mi9CDX6HdqLDdo8RZ-aDIJP4,606
 pants_py_deploy/models.py,sha256=96cqQqW1w3z-tZhthlOyGozL4YwR93H_FVEkipH0qsA,3534
 pants_py_deploy/plugin.py,sha256=64GE89jQMSjK7VFEH43O7r-v1XadT74jJx5UXCManYo,10014
 pants_py_deploy/register.py,sha256=DdsyxfuCEzkruWOItCsoYMpTN75iBkQ1df25Si46KZk,482
-pants_py_deploy-0.0.15rc6.dist-info/METADATA,sha256=QFe7ipQXj9RS5N1IW211mvm9WVPO6z_Eqdbyf7epm00,2256
-pants_py_deploy-0.0.15rc6.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
-pants_py_deploy-0.0.15rc6.dist-info/namespace_packages.txt,sha256=AbpHGcgLb-kRsJGnwFEktk7uzpZOCcBY74-YBdrKVGs,1
-pants_py_deploy-0.0.15rc6.dist-info/top_level.txt,sha256=6ImFjHnejcc1tZDfj2IB6KwifldxnUrXnYfA5rSHSmc,16
-pants_py_deploy-0.0.15rc6.dist-info/RECORD,,
+pants_py_deploy-0.0.15rc7.dist-info/METADATA,sha256=GUYgzJ-2Jwm6SO-15OsClq04B41eJmd9wg-Gx5LMx-k,2256
+pants_py_deploy-0.0.15rc7.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
+pants_py_deploy-0.0.15rc7.dist-info/namespace_packages.txt,sha256=AbpHGcgLb-kRsJGnwFEktk7uzpZOCcBY74-YBdrKVGs,1
+pants_py_deploy-0.0.15rc7.dist-info/top_level.txt,sha256=6ImFjHnejcc1tZDfj2IB6KwifldxnUrXnYfA5rSHSmc,16
+pants_py_deploy-0.0.15rc7.dist-info/RECORD,,
```

