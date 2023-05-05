# Comparing `tmp/icloudtogcal-1.0.3-py3-none-any.whl.zip` & `tmp/icloudtogcal-1.0.4-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -10,12 +10,12 @@
 -rw-r--r--  2.0 fat        0 b- defN 80-Jan-01 00:00 iCloudToGCal/processdata/__init__.py
 -rw-r--r--  2.0 fat      283 b- defN 80-Jan-01 00:00 iCloudToGCal/processdata/data.py
 -rw-r--r--  2.0 fat     2123 b- defN 80-Jan-01 00:00 iCloudToGCal/processdata/processAttendence.py
 -rw-r--r--  2.0 fat     9626 b- defN 80-Jan-01 00:00 iCloudToGCal/processdata/processTable.py
 -rw-r--r--  2.0 fat        0 b- defN 80-Jan-01 00:00 iCloudToGCal/selenuimFunctions/__init__.py
 -rw-r--r--  2.0 fat     2320 b- defN 80-Jan-01 00:00 iCloudToGCal/selenuimFunctions/Gform.py
 -rw-r--r--  2.0 fat     3191 b- defN 80-Jan-01 00:00 iCloudToGCal/selenuimFunctions/iCloud.py
--rw-r--r--  2.0 fat       95 b- defN 80-Jan-01 00:00 icloudtogcal-1.0.3.dist-info/entry_points.txt
--rw-r--r--  2.0 fat      893 b- defN 80-Jan-01 00:00 icloudtogcal-1.0.3.dist-info/METADATA
--rw-r--r--  2.0 fat       88 b- defN 80-Jan-01 00:00 icloudtogcal-1.0.3.dist-info/WHEEL
-?rw-r--r--  2.0 fat     1667 b- defN 16-Jan-01 00:00 icloudtogcal-1.0.3.dist-info/RECORD
+-rw-r--r--  2.0 fat       95 b- defN 80-Jan-01 00:00 icloudtogcal-1.0.4.dist-info/entry_points.txt
+-rw-r--r--  2.0 fat      893 b- defN 80-Jan-01 00:00 icloudtogcal-1.0.4.dist-info/METADATA
+-rw-r--r--  2.0 fat       88 b- defN 80-Jan-01 00:00 icloudtogcal-1.0.4.dist-info/WHEEL
+?rw-r--r--  2.0 fat     1667 b- defN 16-Jan-01 00:00 icloudtogcal-1.0.4.dist-info/RECORD
 19 files, 20161883 bytes uncompressed, 9140549 bytes compressed:  54.7%
```

## zipnote {}

```diff
@@ -39,20 +39,20 @@
 
 Filename: iCloudToGCal/selenuimFunctions/Gform.py
 Comment: 
 
 Filename: iCloudToGCal/selenuimFunctions/iCloud.py
 Comment: 
 
-Filename: icloudtogcal-1.0.3.dist-info/entry_points.txt
+Filename: icloudtogcal-1.0.4.dist-info/entry_points.txt
 Comment: 
 
-Filename: icloudtogcal-1.0.3.dist-info/METADATA
+Filename: icloudtogcal-1.0.4.dist-info/METADATA
 Comment: 
 
-Filename: icloudtogcal-1.0.3.dist-info/WHEEL
+Filename: icloudtogcal-1.0.4.dist-info/WHEEL
 Comment: 
 
-Filename: icloudtogcal-1.0.3.dist-info/RECORD
+Filename: icloudtogcal-1.0.4.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `icloudtogcal-1.0.3.dist-info/METADATA` & `icloudtogcal-1.0.4.dist-info/METADATA`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: icloudtogcal
-Version: 1.0.3
+Version: 1.0.4
 Summary: Sync iCloud events to Google Calendar
 Home-page: https://github.com/fjueic/iCloud-to-Google-Calender.git
 Author: Rohit
 Author-email: rohitmalik987789@gmail.com
 Requires-Python: >=3.7,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
```

## Comparing `icloudtogcal-1.0.3.dist-info/RECORD` & `icloudtogcal-1.0.4.dist-info/RECORD`

 * *Files 14% similar despite different names*

```diff
@@ -9,11 +9,11 @@
 iCloudToGCal/processdata/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 iCloudToGCal/processdata/data.py,sha256=efYrdaWtqjfnFWeuw0r3uY7-a5YrSUos4jvk7e2PLu4,283
 iCloudToGCal/processdata/processAttendence.py,sha256=F_E7yt2am4yCWV5c_bdo8C1IkY5KwaXNQxBxfXwa3bk,2123
 iCloudToGCal/processdata/processTable.py,sha256=0U4etX2DrRQfQjxZeEf0AxvgyABrMpMjX9cT3_wlwjk,9626
 iCloudToGCal/selenuimFunctions/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 iCloudToGCal/selenuimFunctions/Gform.py,sha256=p64bS5sLedDJI54f6VT9rbHgG9xNKx-sOH0R3qQ0ue0,2320
 iCloudToGCal/selenuimFunctions/iCloud.py,sha256=hQQ6Xj9Pwn0l71-J_NkMogAbcxLJ4_M6gNGYp0p0GnQ,3191
-icloudtogcal-1.0.3.dist-info/entry_points.txt,sha256=kCuX_JN2KExOH4PT-MNxNZjGldmGeYqkoFEz0kxNDFY,95
-icloudtogcal-1.0.3.dist-info/METADATA,sha256=2Az03t31Q7Lle6hMHCDXPmelWCyqQqilh2bzk8E7cfA,893
-icloudtogcal-1.0.3.dist-info/WHEEL,sha256=7Z8_27uaHI_UZAc4Uox4PpBhQ9Y5_modZXWMxtUi4NU,88
-icloudtogcal-1.0.3.dist-info/RECORD,,
+icloudtogcal-1.0.4.dist-info/entry_points.txt,sha256=kCuX_JN2KExOH4PT-MNxNZjGldmGeYqkoFEz0kxNDFY,95
+icloudtogcal-1.0.4.dist-info/METADATA,sha256=ulERqqDHp_dDkjZRLR1QH5UVp84dJdSfpTUJEeGe_tQ,893
+icloudtogcal-1.0.4.dist-info/WHEEL,sha256=7Z8_27uaHI_UZAc4Uox4PpBhQ9Y5_modZXWMxtUi4NU,88
+icloudtogcal-1.0.4.dist-info/RECORD,,
```

