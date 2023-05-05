# Comparing `tmp/odoo14_addon_metadata-14.0.0.0.0-py3-none-any.whl.zip` & `tmp/odoo14_addon_metadata-14.0.0.0.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,10 +1,10 @@
-Zip file size: 2617 bytes, number of entries: 8
--rw-r--r--  2.0 unx       21 b- defN 23-May-03 12:56 odoo/addons/metadata/__init__.py
--rw-r--r--  2.0 unx      379 b- defN 23-May-03 12:58 odoo/addons/metadata/__manifest__.py
--rw-r--r--  2.0 unx       28 b- defN 23-May-03 12:56 odoo/addons/metadata/models/__init__.py
--rw-r--r--  2.0 unx      322 b- defN 23-May-03 12:56 odoo/addons/metadata/models/metadata_line.py
--rw-r--r--  2.0 unx      456 b- defN 23-May-03 13:40 odoo14_addon_metadata-14.0.0.0.0.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-May-03 13:40 odoo14_addon_metadata-14.0.0.0.0.dist-info/WHEEL
--rw-r--r--  2.0 unx        5 b- defN 23-May-03 13:40 odoo14_addon_metadata-14.0.0.0.0.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      745 b- defN 23-May-03 13:40 odoo14_addon_metadata-14.0.0.0.0.dist-info/RECORD
-8 files, 2048 bytes uncompressed, 1277 bytes compressed:  37.6%
+Zip file size: 2618 bytes, number of entries: 8
+-rw-r--r--  2.0 unx       21 b- defN 23-May-02 14:44 odoo/addons/metadata/__init__.py
+-rw-r--r--  2.0 unx      379 b- defN 23-May-05 10:33 odoo/addons/metadata/__manifest__.py
+-rw-r--r--  2.0 unx       28 b- defN 23-May-02 14:44 odoo/addons/metadata/models/__init__.py
+-rw-r--r--  2.0 unx      322 b- defN 23-May-02 14:44 odoo/addons/metadata/models/metadata_line.py
+-rw-r--r--  2.0 unx      455 b- defN 23-May-05 10:34 odoo14_addon_metadata-14.0.0.0.1.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-May-05 10:34 odoo14_addon_metadata-14.0.0.0.1.dist-info/WHEEL
+-rw-r--r--  2.0 unx        5 b- defN 23-May-05 10:34 odoo14_addon_metadata-14.0.0.0.1.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      745 b- defN 23-May-05 10:34 odoo14_addon_metadata-14.0.0.0.1.dist-info/RECORD
+8 files, 2047 bytes uncompressed, 1278 bytes compressed:  37.6%
```

## zipnote {}

```diff
@@ -6,20 +6,20 @@
 
 Filename: odoo/addons/metadata/models/__init__.py
 Comment: 
 
 Filename: odoo/addons/metadata/models/metadata_line.py
 Comment: 
 
-Filename: odoo14_addon_metadata-14.0.0.0.0.dist-info/METADATA
+Filename: odoo14_addon_metadata-14.0.0.0.1.dist-info/METADATA
 Comment: 
 
-Filename: odoo14_addon_metadata-14.0.0.0.0.dist-info/WHEEL
+Filename: odoo14_addon_metadata-14.0.0.0.1.dist-info/WHEEL
 Comment: 
 
-Filename: odoo14_addon_metadata-14.0.0.0.0.dist-info/top_level.txt
+Filename: odoo14_addon_metadata-14.0.0.0.1.dist-info/top_level.txt
 Comment: 
 
-Filename: odoo14_addon_metadata-14.0.0.0.0.dist-info/RECORD
+Filename: odoo14_addon_metadata-14.0.0.0.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## odoo/addons/metadata/__manifest__.py

```diff
@@ -5,15 +5,15 @@
     'summary': """
         Save custom metadata on any model""",
 
     'author': "Coopdevs Treball SCCL",
     'website': "",
 
     'category': 'server',
-    'version': '14.0.0.0.0',
+    'version': '14.0.0.0.1',
     "license": "AGPL-3",
 
     # any module necessary for this one to work correctly
     'depends': ['base'],
 
     # always loaded
     'data': [],
```

## Comparing `odoo14_addon_metadata-14.0.0.0.0.dist-info/RECORD` & `odoo14_addon_metadata-14.0.0.0.1.dist-info/RECORD`

 * *Files 22% similar despite different names*

```diff
@@ -1,8 +1,8 @@
 odoo/addons/metadata/__init__.py,sha256=X9EJGOE2GtZbS0G82PtSXmWSZ_R8jEM0rlJTDliQjp4,21
-odoo/addons/metadata/__manifest__.py,sha256=o3CJTwQtOkQuvmUG189sVLPH2iJ7MGeZJLYZVrmJXNQ,379
+odoo/addons/metadata/__manifest__.py,sha256=c6Y1k08idM6gNnfA_sO4iFxx5sYSXZTfNRi1MdnP6to,379
 odoo/addons/metadata/models/__init__.py,sha256=vG7B0tIxGzuSl710Vo4Xv5mrrcfmJpVaAleEZBmvDFs,28
 odoo/addons/metadata/models/metadata_line.py,sha256=127tiwAUtC_hYIyiwGJsRBXCQdfY6TGKk4n0VQr7kC4,322
-odoo14_addon_metadata-14.0.0.0.0.dist-info/METADATA,sha256=gtWT10P8RiJPfrbxYOvzq9LvhwHTWEV0kYngBhMLPVg,456
-odoo14_addon_metadata-14.0.0.0.0.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
-odoo14_addon_metadata-14.0.0.0.0.dist-info/top_level.txt,sha256=qBj40grFkGOfDZ2WDSw3y1RnDlgG0u8rP8pvGNdbz4w,5
-odoo14_addon_metadata-14.0.0.0.0.dist-info/RECORD,,
+odoo14_addon_metadata-14.0.0.0.1.dist-info/METADATA,sha256=pRDthMpRgNvnL2_vSWhCsL0XjqmM194rVI9WlEx9ISE,455
+odoo14_addon_metadata-14.0.0.0.1.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
+odoo14_addon_metadata-14.0.0.0.1.dist-info/top_level.txt,sha256=qBj40grFkGOfDZ2WDSw3y1RnDlgG0u8rP8pvGNdbz4w,5
+odoo14_addon_metadata-14.0.0.0.1.dist-info/RECORD,,
```

