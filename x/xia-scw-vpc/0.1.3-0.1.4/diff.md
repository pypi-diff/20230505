# Comparing `tmp/xia_scw_vpc-0.1.3-cp39-none-win_amd64.whl.zip` & `tmp/xia_scw_vpc-0.1.4-cp39-none-macosx_11_0_x86_64.whl.zip`

## zipinfo {}

```diff
@@ -1,13 +1,13 @@
-Zip file size: 111629 bytes, number of entries: 11
--rw-r--r--  2.0 unx       87 b- defN 23-May-04 17:01 xia_scw_vpc/__init__.py
--rw-r--r--  2.0 unx   264192 b- defN 23-May-04 17:09 xia_scw_vpc/vpc.cp39-win_amd64.pyd
--rw-rw-rw-  2.0 unx     1210 b- defN 23-May-02 08:44 xia_scw_vpc/templates/ScwVpc/main.tf
--rw-rw-rw-  2.0 unx     1077 b- defN 23-May-04 16:55 xia_scw_vpc/templates/ScwVpc/output.tf
--rw-rw-rw-  2.0 unx      343 b- defN 23-Apr-21 13:39 xia_scw_vpc/templates/ScwVpc/provider.tf
--rw-rw-rw-  2.0 unx     2295 b- defN 23-May-02 08:44 xia_scw_vpc/templates/ScwVpc/variables.tf
--rw-rw-rw-  2.0 unx      150 b- defN 23-May-04 17:09 xia_scw_vpc-0.1.3.dist-info/LICENSE.txt
--rw-r--r--  2.0 unx      672 b- defN 23-May-04 17:09 xia_scw_vpc-0.1.3.dist-info/METADATA
--rw-r--r--  2.0 unx       99 b- defN 23-May-04 17:09 xia_scw_vpc-0.1.3.dist-info/WHEEL
--rw-r--r--  2.0 unx       12 b- defN 23-May-04 17:09 xia_scw_vpc-0.1.3.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      961 b- defN 23-May-04 17:09 xia_scw_vpc-0.1.3.dist-info/RECORD
-11 files, 271098 bytes uncompressed, 109981 bytes compressed:  59.4%
+Zip file size: 95548 bytes, number of entries: 11
+-rw-r--r--  2.0 unx       87 b- defN 23-May-05 14:59 xia_scw_vpc/__init__.py
+-rw-r--r--  2.0 unx   252424 b- defN 23-May-05 14:59 xia_scw_vpc/vpc.cpython-310-darwin.so
+-rw-r--r--  2.0 unx     1210 b- defN 23-May-02 08:46 xia_scw_vpc/templates/ScwVpc/main.tf
+-rw-r--r--  2.0 unx     1077 b- defN 23-May-04 17:07 xia_scw_vpc/templates/ScwVpc/output.tf
+-rw-r--r--  2.0 unx      343 b- defN 23-Apr-21 16:02 xia_scw_vpc/templates/ScwVpc/provider.tf
+-rw-r--r--  2.0 unx     2295 b- defN 23-May-02 08:46 xia_scw_vpc/templates/ScwVpc/variables.tf
+-rw-r--r--  2.0 unx      150 b- defN 23-May-05 14:59 xia_scw_vpc-0.1.4.dist-info/LICENSE.txt
+-rw-r--r--  2.0 unx      635 b- defN 23-May-05 14:59 xia_scw_vpc-0.1.4.dist-info/METADATA
+-rw-r--r--  2.0 unx      108 b- defN 23-May-05 14:59 xia_scw_vpc-0.1.4.dist-info/WHEEL
+-rw-r--r--  2.0 unx       12 b- defN 23-May-05 14:59 xia_scw_vpc-0.1.4.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      965 b- defN 23-May-05 14:59 xia_scw_vpc-0.1.4.dist-info/RECORD
+11 files, 259306 bytes uncompressed, 93894 bytes compressed:  63.8%
```

## zipnote {}

```diff
@@ -1,34 +1,34 @@
 Filename: xia_scw_vpc/__init__.py
 Comment: 
 
-Filename: xia_scw_vpc/vpc.cp39-win_amd64.pyd
+Filename: xia_scw_vpc/vpc.cpython-310-darwin.so
 Comment: 
 
 Filename: xia_scw_vpc/templates/ScwVpc/main.tf
 Comment: 
 
 Filename: xia_scw_vpc/templates/ScwVpc/output.tf
 Comment: 
 
 Filename: xia_scw_vpc/templates/ScwVpc/provider.tf
 Comment: 
 
 Filename: xia_scw_vpc/templates/ScwVpc/variables.tf
 Comment: 
 
-Filename: xia_scw_vpc-0.1.3.dist-info/LICENSE.txt
+Filename: xia_scw_vpc-0.1.4.dist-info/LICENSE.txt
 Comment: 
 
-Filename: xia_scw_vpc-0.1.3.dist-info/METADATA
+Filename: xia_scw_vpc-0.1.4.dist-info/METADATA
 Comment: 
 
-Filename: xia_scw_vpc-0.1.3.dist-info/WHEEL
+Filename: xia_scw_vpc-0.1.4.dist-info/WHEEL
 Comment: 
 
-Filename: xia_scw_vpc-0.1.3.dist-info/top_level.txt
+Filename: xia_scw_vpc-0.1.4.dist-info/top_level.txt
 Comment: 
 
-Filename: xia_scw_vpc-0.1.3.dist-info/RECORD
+Filename: xia_scw_vpc-0.1.4.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## xia_scw_vpc/__init__.py

```diff
@@ -1,8 +1,8 @@
 from xia_scw_vpc.vpc import ScwVpc
 
 
 __all__ = [
     "ScwVpc"
 ]
 
-__version__ = "0.1.3"
+__version__ = "0.1.4"
```

## Comparing `xia_scw_vpc-0.1.3.dist-info/RECORD` & `xia_scw_vpc-0.1.4.dist-info/RECORD`

 * *Files 24% similar despite different names*

```diff
@@ -1,11 +1,11 @@
-xia_scw_vpc/__init__.py,sha256=jrgxomwI7fyERF7QCYA4aYFJV_A_29v_tdE7j1UIifw,87
-xia_scw_vpc/vpc.cp39-win_amd64.pyd,sha256=J8QwhKbYw5KbR9xH4rmEaToVBxCrjUnr24XR8Bc-Zgc,264192
+xia_scw_vpc/__init__.py,sha256=Jl3hFUzXrf1Ipl1URHyvev9YkgwgjN7fuE3ubHTK3i8,87
+xia_scw_vpc/vpc.cpython-310-darwin.so,sha256=xnuPm9dHI5M073uGeffYT5DFB9RsNjcKUjBDp7k5vKs,252424
 xia_scw_vpc/templates/ScwVpc/main.tf,sha256=_VCRRiquB39fg7rzlQdta2E5N62DBESugd5r5igNt9M,1210
 xia_scw_vpc/templates/ScwVpc/output.tf,sha256=1AoWU7gDnPFjkXg0VMcgmbQLy7O9VNKpOEnvO_EbgT0,1077
 xia_scw_vpc/templates/ScwVpc/provider.tf,sha256=h_zFGas7QtYJPGvufLGuPHtgDhoZa28Qa5t--1dpheI,343
 xia_scw_vpc/templates/ScwVpc/variables.tf,sha256=-qYxcGlWOGcmTQIhkM6HFRnxhd-yMFZ7wG5GtSHoFpE,2295
-xia_scw_vpc-0.1.3.dist-info/LICENSE.txt,sha256=2HzK8y__YhkYAEzI5V38DGwiVGnADL74BLH_dyBEs7I,150
-xia_scw_vpc-0.1.3.dist-info/METADATA,sha256=AJJl1y9BIs-mte7TJWN34q9JBhQe7Y81JycdIPC4918,672
-xia_scw_vpc-0.1.3.dist-info/WHEEL,sha256=T8VPDjot1YI5-NaRzS6kIMlJNVl0SSGa_dm-8Fprszg,99
-xia_scw_vpc-0.1.3.dist-info/top_level.txt,sha256=jNt0Wv07qq3bYLKNdao2gLQ4e_U6VYrOuw3Wehup0ts,12
-xia_scw_vpc-0.1.3.dist-info/RECORD,,
+xia_scw_vpc-0.1.4.dist-info/LICENSE.txt,sha256=2HzK8y__YhkYAEzI5V38DGwiVGnADL74BLH_dyBEs7I,150
+xia_scw_vpc-0.1.4.dist-info/METADATA,sha256=lHJWKzgRhPerW82nVPKK9kXpH7NK4CCRo-xoljrKWkM,635
+xia_scw_vpc-0.1.4.dist-info/WHEEL,sha256=NsapCMY7EanMRKZsZABtoiyq2rs4aXJ4FKsV_kV91NE,108
+xia_scw_vpc-0.1.4.dist-info/top_level.txt,sha256=jNt0Wv07qq3bYLKNdao2gLQ4e_U6VYrOuw3Wehup0ts,12
+xia_scw_vpc-0.1.4.dist-info/RECORD,,
```

