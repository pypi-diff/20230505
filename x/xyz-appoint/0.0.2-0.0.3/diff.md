# Comparing `tmp/xyz_appoint-0.0.2-py3-none-any.whl.zip` & `tmp/xyz_appoint-0.0.3-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,18 +1,18 @@
-Zip file size: 7614 bytes, number of entries: 16
+Zip file size: 7655 bytes, number of entries: 16
 -rw-r--r--  2.0 unx      134 b- defN 22-May-08 10:07 xyz_appoint/__init__.py
 -rw-r--r--  2.0 unx      616 b- defN 22-May-08 14:46 xyz_appoint/admin.py
 -rw-r--r--  2.0 unx     1666 b- defN 22-May-08 17:35 xyz_appoint/apis.py
 -rw-r--r--  2.0 unx      338 b- defN 22-May-08 09:44 xyz_appoint/apps.py
--rw-r--r--  2.0 unx      483 b- defN 22-May-08 15:43 xyz_appoint/authentications.py
+-rw-r--r--  2.0 unx      577 b- defN 23-Mar-15 06:10 xyz_appoint/authentications.py
 -rw-r--r--  2.0 unx      616 b- defN 22-May-08 12:24 xyz_appoint/helper.py
 -rw-r--r--  2.0 unx      767 b- defN 22-May-08 10:01 xyz_appoint/mixins.py
 -rw-r--r--  2.0 unx     2039 b- defN 22-May-08 15:17 xyz_appoint/models.py
 -rw-r--r--  2.0 unx      862 b- defN 22-May-23 04:12 xyz_appoint/permissions.py
 -rw-r--r--  2.0 unx      602 b- defN 22-May-08 14:43 xyz_appoint/serializers.py
 -rw-r--r--  2.0 unx     3150 b- defN 22-May-08 15:21 xyz_appoint/migrations/0001_initial.py
 -rw-r--r--  2.0 unx        0 b- defN 22-May-08 12:44 xyz_appoint/migrations/__init__.py
--rw-r--r--  2.0 unx      967 b- defN 22-May-23 04:13 xyz_appoint-0.0.2.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 22-May-23 04:13 xyz_appoint-0.0.2.dist-info/WHEEL
--rw-r--r--  2.0 unx       12 b- defN 22-May-23 04:13 xyz_appoint-0.0.2.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx     1284 b- defN 22-May-23 04:13 xyz_appoint-0.0.2.dist-info/RECORD
-16 files, 13628 bytes uncompressed, 5492 bytes compressed:  59.7%
+-rw-r--r--  2.0 unx      967 b- defN 23-May-05 03:18 xyz_appoint-0.0.3.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-May-05 03:18 xyz_appoint-0.0.3.dist-info/WHEEL
+-rw-r--r--  2.0 unx       12 b- defN 23-May-05 03:18 xyz_appoint-0.0.3.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx     1284 b- defN 23-May-05 03:18 xyz_appoint-0.0.3.dist-info/RECORD
+16 files, 13722 bytes uncompressed, 5533 bytes compressed:  59.7%
```

## zipnote {}

```diff
@@ -30,20 +30,20 @@
 
 Filename: xyz_appoint/migrations/0001_initial.py
 Comment: 
 
 Filename: xyz_appoint/migrations/__init__.py
 Comment: 
 
-Filename: xyz_appoint-0.0.2.dist-info/METADATA
+Filename: xyz_appoint-0.0.3.dist-info/METADATA
 Comment: 
 
-Filename: xyz_appoint-0.0.2.dist-info/WHEEL
+Filename: xyz_appoint-0.0.3.dist-info/WHEEL
 Comment: 
 
-Filename: xyz_appoint-0.0.2.dist-info/top_level.txt
+Filename: xyz_appoint-0.0.3.dist-info/top_level.txt
 Comment: 
 
-Filename: xyz_appoint-0.0.2.dist-info/RECORD
+Filename: xyz_appoint-0.0.3.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## xyz_appoint/authentications.py

```diff
@@ -1,14 +1,17 @@
 # -*- coding:utf-8 -*-
-from rest_framework.authentication import   TokenAuthentication
+from rest_framework import exceptions, authentication
 __author__ = 'denishuang'
 
 from .models import Appointment
 
-class AppointAuthentication(TokenAuthentication):
+
+class AppointAuthentication(authentication.TokenAuthentication):
     model = Appointment
 
     def authenticate_credentials(self, key):
         from .helper import check_appoint_token
         context = check_appoint_token(key)
+        if not context:
+            raise exceptions.AuthenticationFailed('not found')
         user, policy = super(AppointAuthentication, self).authenticate_credentials(context['ak'])
-        return user, policy
+        return user, policy
```

## Comparing `xyz_appoint-0.0.2.dist-info/METADATA` & `xyz_appoint-0.0.3.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xyz-appoint
-Version: 0.0.2
+Version: 0.0.3
 Summary: auth appoint api
 Home-page: https://github.com/szuprefix/py-xyz-appoint
 Author: szuprefix
 Author-email: szuprefix@126.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Environment :: Web Environment
```

## Comparing `xyz_appoint-0.0.2.dist-info/RECORD` & `xyz_appoint-0.0.3.dist-info/RECORD`

 * *Files 19% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 xyz_appoint/__init__.py,sha256=LujDnb3B5b3bbSUBApiJhxbmk9hQO9gPCT6uusZIB3g,134
 xyz_appoint/admin.py,sha256=A1W5ah1RNjQ6q0UjFM91ehhEl6f1cT6dRYfn7itpNYQ,616
 xyz_appoint/apis.py,sha256=kL17ABsR1HgeeHx8_mPvDkjpLdrBoyu6VOK0G9TDKLY,1666
 xyz_appoint/apps.py,sha256=au8xkKUK2D8PXo1ORzVGc-WiMcTe3XZTdOmogqdboyo,338
-xyz_appoint/authentications.py,sha256=47mkxsyw7pvaIlXAbvtJBK5b07wvkSnYsOhxgVAszTU,483
+xyz_appoint/authentications.py,sha256=FEKvc099PsOcHrQWibw6VlmG_H4BZfXHQD0yTf6RLJc,577
 xyz_appoint/helper.py,sha256=uxa0_2BZw2YMFZ3bp_ymsYPTsbi0AmLBosHi_ZPVul4,616
 xyz_appoint/mixins.py,sha256=fDptN78fOle5LniSC2DoD-2FKKwoEnDGsIfr0Oy61aI,767
 xyz_appoint/models.py,sha256=dkVemivNaW0w7itoIp1fRlS-7pxqn2EbntSC-mfUB-c,2039
 xyz_appoint/permissions.py,sha256=2mrjP31mWzFPgHpsOOAgEdEMBnbIXPLraboEIWvoV7U,862
 xyz_appoint/serializers.py,sha256=qxuF1hHwSjZXToFZATaxCUOWJe3qBvEmssEx3GPVjUI,602
 xyz_appoint/migrations/0001_initial.py,sha256=1xi73iQU7tiJMW4ZrXg_3WVs8KbDSqRUivfWvF3Bk2c,3150
 xyz_appoint/migrations/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-xyz_appoint-0.0.2.dist-info/METADATA,sha256=_csGnFtiARKFxTSvidXAaIFZsjLj6SaktDUIMU7AP9M,967
-xyz_appoint-0.0.2.dist-info/WHEEL,sha256=g4nMs7d-Xl9-xC9XovUrsDHGXt-FT0E17Yqo92DEfvY,92
-xyz_appoint-0.0.2.dist-info/top_level.txt,sha256=0JThQvtcc6g0nhGdOxNdHOYGr02LORHquZ8vxeZWe_s,12
-xyz_appoint-0.0.2.dist-info/RECORD,,
+xyz_appoint-0.0.3.dist-info/METADATA,sha256=FfpZvVjNaOcxN70FWD553TdupM7GxTPHlpDFuiUtX-w,967
+xyz_appoint-0.0.3.dist-info/WHEEL,sha256=g4nMs7d-Xl9-xC9XovUrsDHGXt-FT0E17Yqo92DEfvY,92
+xyz_appoint-0.0.3.dist-info/top_level.txt,sha256=0JThQvtcc6g0nhGdOxNdHOYGr02LORHquZ8vxeZWe_s,12
+xyz_appoint-0.0.3.dist-info/RECORD,,
```

