# Comparing `tmp/qmenta_anon-1.1.dev320-py3-none-any.whl.zip` & `tmp/qmenta_anon-1.1.dev323-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,11 +1,11 @@
-Zip file size: 9182 bytes, number of entries: 9
+Zip file size: 9190 bytes, number of entries: 9
 -rw-r--r--  2.0 unx       65 b- defN 80-Jan-01 00:00 qmenta/__init__.py
 -rw-r--r--  2.0 unx       65 b- defN 80-Jan-01 00:00 qmenta/anon/__init__.py
 -rw-r--r--  2.0 unx     1753 b- defN 80-Jan-01 00:00 qmenta/anon/auto.py
 -rw-r--r--  2.0 unx    19453 b- defN 80-Jan-01 00:00 qmenta/anon/dicom.py
 -rw-r--r--  2.0 unx     1333 b- defN 80-Jan-01 00:00 qmenta/anon/nifti.py
 -rw-r--r--  2.0 unx     3731 b- defN 80-Jan-01 00:00 qmenta/anon/time_utils.py
-?rw-r--r--  2.0 unx       83 b- defN 16-Jan-01 00:00 qmenta_anon-1.1.dev320.dist-info/WHEEL
-?rw-r--r--  2.0 unx      725 b- defN 16-Jan-01 00:00 qmenta_anon-1.1.dev320.dist-info/METADATA
-?rw-r--r--  2.0 unx      696 b- defN 16-Jan-01 00:00 qmenta_anon-1.1.dev320.dist-info/RECORD
-9 files, 27904 bytes uncompressed, 7990 bytes compressed:  71.4%
+-rw-r--r--  2.0 unx      776 b- defN 80-Jan-01 00:00 qmenta_anon-1.1.dev323.dist-info/METADATA
+-rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 qmenta_anon-1.1.dev323.dist-info/WHEEL
+?rw-r--r--  2.0 unx      696 b- defN 16-Jan-01 00:00 qmenta_anon-1.1.dev323.dist-info/RECORD
+9 files, 27960 bytes uncompressed, 7998 bytes compressed:  71.4%
```

## zipnote {}

```diff
@@ -12,17 +12,17 @@
 
 Filename: qmenta/anon/nifti.py
 Comment: 
 
 Filename: qmenta/anon/time_utils.py
 Comment: 
 
-Filename: qmenta_anon-1.1.dev320.dist-info/WHEEL
+Filename: qmenta_anon-1.1.dev323.dist-info/METADATA
 Comment: 
 
-Filename: qmenta_anon-1.1.dev320.dist-info/METADATA
+Filename: qmenta_anon-1.1.dev323.dist-info/WHEEL
 Comment: 
 
-Filename: qmenta_anon-1.1.dev320.dist-info/RECORD
+Filename: qmenta_anon-1.1.dev323.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `qmenta_anon-1.1.dev320.dist-info/METADATA` & `qmenta_anon-1.1.dev323.dist-info/METADATA`

 * *Files 6% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 Metadata-Version: 2.1
 Name: qmenta-anon
-Version: 1.1.dev320
+Version: 1.1.dev323
 Summary: The qmenta-anon library is used to anonymize files before transferring them to the QMENTA platform.
 Author: QMENTA
 Author-email: dev@qmenta.com
 Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Scientific/Engineering :: Medical Science Apps.
 Requires-Dist: nibabel (>=3.2.2,<4.0.0)
 Requires-Dist: pydicom (>=2.3.0,<3.0.0)
```

