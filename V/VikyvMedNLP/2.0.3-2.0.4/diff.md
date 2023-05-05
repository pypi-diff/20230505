# Comparing `tmp/VikyvMedNLP-2.0.3-py38-none-any.whl.zip` & `tmp/VikyvMedNLP-2.0.4-py38-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 11161 bytes, number of entries: 6
--rw-------  2.0 unx      143 b- defN 23-May-04 15:36 VikyvMedNLP/__init__.pyc
--rw-------  2.0 unx    18830 b- defN 23-May-04 15:36 VikyvMedNLP/medToolkit.pyc
--rw-------  2.0 unx     8784 b- defN 23-May-04 15:36 VikyvMedNLP-2.0.3.dist-info/METADATA
--rw-------  2.0 unx       82 b- defN 23-May-04 15:36 VikyvMedNLP-2.0.3.dist-info/WHEEL
--rw-------  2.0 unx       12 b- defN 23-May-04 15:36 VikyvMedNLP-2.0.3.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      478 b- defN 23-May-04 15:36 VikyvMedNLP-2.0.3.dist-info/RECORD
-6 files, 28329 bytes uncompressed, 10295 bytes compressed:  63.7%
+Zip file size: 11199 bytes, number of entries: 6
+-rw-------  2.0 unx      143 b- defN 23-May-05 05:36 VikyvMedNLP/__init__.pyc
+-rw-------  2.0 unx    18830 b- defN 23-May-05 05:36 VikyvMedNLP/medToolkit.pyc
+-rw-------  2.0 unx     8837 b- defN 23-May-05 05:36 VikyvMedNLP-2.0.4.dist-info/METADATA
+-rw-------  2.0 unx       82 b- defN 23-May-05 05:36 VikyvMedNLP-2.0.4.dist-info/WHEEL
+-rw-------  2.0 unx       12 b- defN 23-May-05 05:36 VikyvMedNLP-2.0.4.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      478 b- defN 23-May-05 05:36 VikyvMedNLP-2.0.4.dist-info/RECORD
+6 files, 28382 bytes uncompressed, 10333 bytes compressed:  63.6%
```

## zipnote {}

```diff
@@ -1,19 +1,19 @@
 Filename: VikyvMedNLP/__init__.pyc
 Comment: 
 
 Filename: VikyvMedNLP/medToolkit.pyc
 Comment: 
 
-Filename: VikyvMedNLP-2.0.3.dist-info/METADATA
+Filename: VikyvMedNLP-2.0.4.dist-info/METADATA
 Comment: 
 
-Filename: VikyvMedNLP-2.0.3.dist-info/WHEEL
+Filename: VikyvMedNLP-2.0.4.dist-info/WHEEL
 Comment: 
 
-Filename: VikyvMedNLP-2.0.3.dist-info/top_level.txt
+Filename: VikyvMedNLP-2.0.4.dist-info/top_level.txt
 Comment: 
 
-Filename: VikyvMedNLP-2.0.3.dist-info/RECORD
+Filename: VikyvMedNLP-2.0.4.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## VikyvMedNLP/medToolkit.pyc

 * *Format-specific differences are supported for Python .pyc files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: Byte-compiled Python module for CPython 3.8, timestamp-based, .py timestamp: Thu May  4 13:45:34 2023 UTC, .py size: 26897 bytes*

 * *Could not decompile bytecode: bad marshal data (unknown type code)*

```diff
@@ -1101,15 +1101,15 @@
 000044c0: 656e 7473 729a 0000 005a 0867 6574 5f74  entsr....Z.get_t
 000044d0: 6578 74da 0772 6570 6c61 6365 7230 0000  ext..replacer0..
 000044e0: 00da 046b 6579 735a 0a73 6561 7263 685f  ...keysZ.search_
 000044f0: 666f 725a 1061 6464 5f72 6564 6163 745f  forZ.add_redact_
 00004500: 616e 6e6f 745a 1061 7070 6c79 5f72 6564  annotZ.apply_red
 00004510: 6163 7469 6f6e 73da 0473 6176 6572 1500  actions..saver..
 00004520: 0000 290a 7282 0000 0072 9d00 0000 7258  ..).r....r....rX
-00004530: 0000 00da 0470 6167 655a 0973 656e 7369  .....pageZ.sensi
+00004530: 0000 005a 0470 6167 655a 0973 656e 7369  ...Z.pageZ.sensi
 00004540: 7469 7665 7227 0000 0072 3b00 0000 da04  tiver'...r;.....
 00004550: 6461 7461 5a05 6172 6561 735a 0461 7265  dataZ.areasZ.are
 00004560: 6172 1700 0000 72a2 0000 0072 1800 0000  ar....r....r....
 00004570: 729b 0000 007c 0200 0073 1e00 0000 0002  r....|...s......
 00004580: 0801 0601 0801 1802 1601 0c01 0e02 0801  ................
 00004590: 0a01 0801 1201 0a02 0a01 0801 7a1b 4465  ............z.De
 000045a0: 6964 656e 7469 6669 6361 7469 6f6e 2e72  identification.r
```

## Comparing `VikyvMedNLP-2.0.3.dist-info/METADATA` & `VikyvMedNLP-2.0.4.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 Metadata-Version: 2.1
 Name: VikyvMedNLP
-Version: 2.0.3
+Version: 2.0.4
 Summary: Medical NLP Toolkit
+Download-URL: https://sample-videos.com/zip/10mb.zip
 Author: vLife|Virtusa
 Author-email: vlife@virtusa.com
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
```

