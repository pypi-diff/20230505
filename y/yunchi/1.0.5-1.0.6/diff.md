# Comparing `tmp/yunchi-1.0.5-cp38-cp38-win_amd64.whl.zip` & `tmp/yunchi-1.0.6-cp38-cp38-manylinux_2_5_x86_64.manylinux1_x86_64.whl.zip`

## zipinfo {}

```diff
@@ -1,21 +1,24 @@
-Zip file size: 454023 bytes, number of entries: 19
--rw-rw-rw-  2.0 fat      188 b- defN 23-Apr-14 03:05 yunchi/__init__.py
--rw-rw-rw-  2.0 fat      150 b- defN 23-Apr-14 03:00 yunchi/api.py
--rw-rw-rw-  2.0 fat   270336 b- defN 23-Apr-21 08:29 yunchi/data.cp38-win_amd64.pyd
--rw-rw-rw-  2.0 fat     9403 b- defN 23-Mar-31 07:27 yunchi/model.py
--rw-rw-rw-  2.0 fat   176640 b- defN 23-Apr-21 08:29 yunchi/quote.cp38-win_amd64.pyd
--rw-rw-rw-  2.0 fat   176640 b- defN 23-Apr-21 08:29 yunchi/sdk.cp38-win_amd64.pyd
--rw-rw-rw-  2.0 fat   107008 b- defN 23-Apr-21 08:29 yunchi/strategy.cp38-win_amd64.pyd
--rw-rw-rw-  2.0 fat   254464 b- defN 23-Apr-21 08:29 yunchi/trade.cp38-win_amd64.pyd
--rw-rw-rw-  2.0 fat     9745 b- defN 23-Apr-06 07:48 yunchi/pb/Quotation.proto
--rw-rw-rw-  2.0 fat   102268 b- defN 23-Mar-10 07:41 yunchi/pb/Quotation_pb2.py
--rw-rw-rw-  2.0 fat      104 b- defN 23-Apr-14 01:57 yunchi/pb/__init__.py
--rw-rw-rw-  2.0 fat   352070 b- defN 23-Apr-14 01:58 yunchi/pb/api_pb2.py
--rw-rw-rw-  2.0 fat    35275 b- defN 23-Jan-10 06:21 yunchi/pb/dtp.api.proto
--rw-rw-rw-  2.0 fat    10950 b- defN 23-Jan-10 06:21 yunchi/pb/dtp.type.proto
--rw-rw-rw-  2.0 fat    49067 b- defN 23-Apr-14 01:57 yunchi/pb/type_pb2.py
--rw-rw-rw-  2.0 fat      466 b- defN 23-Apr-21 08:29 yunchi-1.0.5.dist-info/METADATA
--rw-rw-rw-  2.0 fat      100 b- defN 23-Apr-21 08:29 yunchi-1.0.5.dist-info/WHEEL
--rw-rw-rw-  2.0 fat        7 b- defN 23-Apr-21 08:29 yunchi-1.0.5.dist-info/top_level.txt
-?rw-rw-r--  2.0 fat     1523 b- defN 23-Apr-21 08:29 yunchi-1.0.5.dist-info/RECORD
-19 files, 1556404 bytes uncompressed, 451587 bytes compressed:  71.0%
+Zip file size: 2407538 bytes, number of entries: 22
+drwxr-xr-x  2.0 unx        0 b- stor 23-May-05 09:12 yunchi.libs/
+drwxr-xr-x  2.0 unx        0 b- stor 23-May-05 09:12 yunchi/
+drwxr-xr-x  2.0 unx        0 b- stor 23-May-05 09:12 yunchi-1.0.6.dist-info/
+drwxr-xr-x  2.0 unx        0 b- stor 23-May-05 09:12 yunchi/pb/
+-rwxr-xr-x  2.0 unx  2246347 b- defN 23-May-05 09:12 yunchi/quote.cpython-38-x86_64-linux-gnu.so
+-rw-r--r--  2.0 unx      150 b- defN 23-May-05 09:12 yunchi/api.py
+-rwxr-xr-x  2.0 unx  6091160 b- defN 23-May-05 09:12 yunchi/data.cpython-38-x86_64-linux-gnu.so
+-rwxr-xr-x  2.0 unx  3753684 b- defN 23-May-05 09:12 yunchi/trade.cpython-38-x86_64-linux-gnu.so
+-rwxr-xr-x  2.0 unx  1228926 b- defN 23-May-05 09:12 yunchi/strategy.cpython-38-x86_64-linux-gnu.so
+-rw-r--r--  2.0 unx     9397 b- defN 23-May-05 09:12 yunchi/model.py
+-rw-r--r--  2.0 unx      188 b- defN 23-May-05 09:12 yunchi/__init__.py
+-rw-r--r--  2.0 unx   352070 b- defN 23-May-05 09:12 yunchi/pb/api_pb2.py
+-rwxrwxrwx  2.0 unx     9745 b- defN 23-May-05 09:12 yunchi/pb/Quotation.proto
+-rwxrwxrwx  2.0 unx    35275 b- defN 23-May-05 09:12 yunchi/pb/dtp.api.proto
+-rw-r--r--  2.0 unx   102268 b- defN 23-May-05 09:12 yunchi/pb/Quotation_pb2.py
+-rwxrwxrwx  2.0 unx    10950 b- defN 23-May-05 09:12 yunchi/pb/dtp.type.proto
+-rw-r--r--  2.0 unx    49067 b- defN 23-May-05 09:12 yunchi/pb/type_pb2.py
+-rw-r--r--  2.0 unx      104 b- defN 23-May-05 09:12 yunchi/pb/__init__.py
+-rw-rw-r--  2.0 unx     1505 b- defN 23-May-05 09:12 yunchi-1.0.6.dist-info/RECORD
+-rw-r--r--  2.0 unx      450 b- defN 23-May-05 09:12 yunchi-1.0.6.dist-info/METADATA
+-rw-r--r--  2.0 unx      144 b- defN 23-May-05 09:12 yunchi-1.0.6.dist-info/WHEEL
+-rwxrwxrwx  2.0 unx        7 b- defN 23-May-05 09:12 yunchi-1.0.6.dist-info/top_level.txt
+22 files, 13891437 bytes uncompressed, 2404732 bytes compressed:  82.7%
```

## zipnote {}

```diff
@@ -1,58 +1,67 @@
-Filename: yunchi/__init__.py
+Filename: yunchi.libs/
 Comment: 
 
-Filename: yunchi/api.py
+Filename: yunchi/
 Comment: 
 
-Filename: yunchi/data.cp38-win_amd64.pyd
+Filename: yunchi-1.0.6.dist-info/
 Comment: 
 
-Filename: yunchi/model.py
+Filename: yunchi/pb/
 Comment: 
 
-Filename: yunchi/quote.cp38-win_amd64.pyd
+Filename: yunchi/quote.cpython-38-x86_64-linux-gnu.so
 Comment: 
 
-Filename: yunchi/sdk.cp38-win_amd64.pyd
+Filename: yunchi/api.py
 Comment: 
 
-Filename: yunchi/strategy.cp38-win_amd64.pyd
+Filename: yunchi/data.cpython-38-x86_64-linux-gnu.so
 Comment: 
 
-Filename: yunchi/trade.cp38-win_amd64.pyd
+Filename: yunchi/trade.cpython-38-x86_64-linux-gnu.so
 Comment: 
 
-Filename: yunchi/pb/Quotation.proto
+Filename: yunchi/strategy.cpython-38-x86_64-linux-gnu.so
 Comment: 
 
-Filename: yunchi/pb/Quotation_pb2.py
+Filename: yunchi/model.py
 Comment: 
 
-Filename: yunchi/pb/__init__.py
+Filename: yunchi/__init__.py
 Comment: 
 
 Filename: yunchi/pb/api_pb2.py
 Comment: 
 
+Filename: yunchi/pb/Quotation.proto
+Comment: 
+
 Filename: yunchi/pb/dtp.api.proto
 Comment: 
 
+Filename: yunchi/pb/Quotation_pb2.py
+Comment: 
+
 Filename: yunchi/pb/dtp.type.proto
 Comment: 
 
 Filename: yunchi/pb/type_pb2.py
 Comment: 
 
-Filename: yunchi-1.0.5.dist-info/METADATA
+Filename: yunchi/pb/__init__.py
+Comment: 
+
+Filename: yunchi-1.0.6.dist-info/RECORD
 Comment: 
 
-Filename: yunchi-1.0.5.dist-info/WHEEL
+Filename: yunchi-1.0.6.dist-info/METADATA
 Comment: 
 
-Filename: yunchi-1.0.5.dist-info/top_level.txt
+Filename: yunchi-1.0.6.dist-info/WHEEL
 Comment: 
 
-Filename: yunchi-1.0.5.dist-info/RECORD
+Filename: yunchi-1.0.6.dist-info/top_level.txt
 Comment: 
 
 Zip file comment:
```

## filetype from file(1)

```diff
@@ -1 +1 @@
-Zip archive data, at least v2.0 to extract, compression method=deflate
+Zip archive data, at least v2.0 to extract, compression method=store
```

## yunchi/model.py

```diff
@@ -108,15 +108,15 @@
         int64 nLowLimited = 62;  //跌停价
         int32 nLocalTime = 67;
     """
 
 
 class BarData(dict):
     """
-        分钟Bar定义
+        Bar定义
     """
 
     @property
     def code(self):
         """
         证券代码
         :return:
```

