# Comparing `tmp/qmenta_anon-1.1.dev323-py3-none-any.whl.zip` & `tmp/qmenta_anon-1.1.dev330-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,11 +1,11 @@
-Zip file size: 9190 bytes, number of entries: 9
+Zip file size: 9251 bytes, number of entries: 9
 -rw-r--r--  2.0 unx       65 b- defN 80-Jan-01 00:00 qmenta/__init__.py
 -rw-r--r--  2.0 unx       65 b- defN 80-Jan-01 00:00 qmenta/anon/__init__.py
 -rw-r--r--  2.0 unx     1753 b- defN 80-Jan-01 00:00 qmenta/anon/auto.py
--rw-r--r--  2.0 unx    19453 b- defN 80-Jan-01 00:00 qmenta/anon/dicom.py
+-rw-r--r--  2.0 unx    19814 b- defN 80-Jan-01 00:00 qmenta/anon/dicom.py
 -rw-r--r--  2.0 unx     1333 b- defN 80-Jan-01 00:00 qmenta/anon/nifti.py
 -rw-r--r--  2.0 unx     3731 b- defN 80-Jan-01 00:00 qmenta/anon/time_utils.py
--rw-r--r--  2.0 unx      776 b- defN 80-Jan-01 00:00 qmenta_anon-1.1.dev323.dist-info/METADATA
--rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 qmenta_anon-1.1.dev323.dist-info/WHEEL
-?rw-r--r--  2.0 unx      696 b- defN 16-Jan-01 00:00 qmenta_anon-1.1.dev323.dist-info/RECORD
-9 files, 27960 bytes uncompressed, 7998 bytes compressed:  71.4%
+-rw-r--r--  2.0 unx      776 b- defN 80-Jan-01 00:00 qmenta_anon-1.1.dev330.dist-info/METADATA
+-rw-r--r--  2.0 unx       88 b- defN 80-Jan-01 00:00 qmenta_anon-1.1.dev330.dist-info/WHEEL
+?rw-r--r--  2.0 unx      696 b- defN 16-Jan-01 00:00 qmenta_anon-1.1.dev330.dist-info/RECORD
+9 files, 28321 bytes uncompressed, 8059 bytes compressed:  71.5%
```

## zipnote {}

```diff
@@ -12,17 +12,17 @@
 
 Filename: qmenta/anon/nifti.py
 Comment: 
 
 Filename: qmenta/anon/time_utils.py
 Comment: 
 
-Filename: qmenta_anon-1.1.dev323.dist-info/METADATA
+Filename: qmenta_anon-1.1.dev330.dist-info/METADATA
 Comment: 
 
-Filename: qmenta_anon-1.1.dev323.dist-info/WHEEL
+Filename: qmenta_anon-1.1.dev330.dist-info/WHEEL
 Comment: 
 
-Filename: qmenta_anon-1.1.dev323.dist-info/RECORD
+Filename: qmenta_anon-1.1.dev330.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## qmenta/anon/dicom.py

```diff
@@ -488,16 +488,27 @@
 
             date_element = header[date_atr.tag]
             time_element = header[time_atr.tag]
 
             assert date_element.VR == "DA"
             assert time_element.VR == "TM"
 
-            in_date = pydicom.valuerep.DA(date_element.value)
-            in_time = pydicom.valuerep.TM(time_element.value)
+            # If date_element not a date string, then set to null to be
+            # anonymized
+            try:
+                in_date = pydicom.valuerep.DA(date_element.value)
+            except ValueError:
+                in_date = None
+
+            # If time_element not a date string, then set to null to be
+            # anonymized
+            try:
+                in_time = pydicom.valuerep.TM(time_element.value)
+            except ValueError:
+                in_time = None
 
             if not (in_date and in_time):
                 # One of the input values was an empty string
                 anonymise_header_attribute(
                     header, time_atr, self._original_actions[time_atr])
                 anonymise_header_attribute(
                     header, date_atr, self._original_actions[date_atr])
```

## Comparing `qmenta_anon-1.1.dev323.dist-info/METADATA` & `qmenta_anon-1.1.dev330.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: qmenta-anon
-Version: 1.1.dev323
+Version: 1.1.dev330
 Summary: The qmenta-anon library is used to anonymize files before transferring them to the QMENTA platform.
 Author: QMENTA
 Author-email: dev@qmenta.com
 Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: License :: Other/Proprietary License
```

## Comparing `qmenta_anon-1.1.dev323.dist-info/RECORD` & `qmenta_anon-1.1.dev330.dist-info/RECORD`

 * *Files 24% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 qmenta/__init__.py,sha256=jv2YF__bseklT3OWEzlqJ5qE24c4aWd5F4r0TTjOrWQ,65
 qmenta/anon/__init__.py,sha256=jv2YF__bseklT3OWEzlqJ5qE24c4aWd5F4r0TTjOrWQ,65
 qmenta/anon/auto.py,sha256=08IERB8Gw4ZSHfXsqkNTJCxMnqgTR0kab-VnaZtwgxQ,1753
-qmenta/anon/dicom.py,sha256=-oceCZE0Z2-t6eRC0PjDjannH4_iwUHlkf8ezI7gaQA,19453
+qmenta/anon/dicom.py,sha256=xlw1g1FwhnWEfMR4TYyTWLFjQZbeILt7YXfO07q03K0,19814
 qmenta/anon/nifti.py,sha256=GF17HD6-ABpL74Ys1pr0M0uLy_9al-eMB5EYaZUQwz4,1333
 qmenta/anon/time_utils.py,sha256=nxrfXsxqWPYHUB-xNwTV1Wpz9RdDKYctHqYQVUXk448,3731
-qmenta_anon-1.1.dev323.dist-info/METADATA,sha256=NqoLliNeNLzUWamhPtrJAEFJY_mlI5MlEPAQ6lUhnO0,776
-qmenta_anon-1.1.dev323.dist-info/WHEEL,sha256=7Z8_27uaHI_UZAc4Uox4PpBhQ9Y5_modZXWMxtUi4NU,88
-qmenta_anon-1.1.dev323.dist-info/RECORD,,
+qmenta_anon-1.1.dev330.dist-info/METADATA,sha256=PhnN2Pv4Zph2Z8KdKD_TVXySGU1ZASJcgRF5KISCeL8,776
+qmenta_anon-1.1.dev330.dist-info/WHEEL,sha256=7Z8_27uaHI_UZAc4Uox4PpBhQ9Y5_modZXWMxtUi4NU,88
+qmenta_anon-1.1.dev330.dist-info/RECORD,,
```

