# Comparing `tmp/extended_tk-0.12.0-py3-none-any.whl.zip` & `tmp/extended_tk-0.13.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 7174 bytes, number of entries: 7
+Zip file size: 7206 bytes, number of entries: 7
 -rw-rw-rw-  2.0 fat     9452 b- defN 23-Apr-24 19:44 TkPlus/__init__.py
--rw-rw-rw-  2.0 fat     9652 b- defN 23-Apr-25 19:02 extended_tk/__init__.py
--rw-rw-rw-  2.0 fat      243 b- defN 23-Apr-25 19:19 extended_tk-0.12.0.dist-info/LICENSE
--rw-rw-rw-  2.0 fat      810 b- defN 23-Apr-25 19:19 extended_tk-0.12.0.dist-info/METADATA
--rw-rw-rw-  2.0 fat       92 b- defN 23-Apr-25 19:19 extended_tk-0.12.0.dist-info/WHEEL
--rw-rw-rw-  2.0 fat       12 b- defN 23-Apr-25 19:19 extended_tk-0.12.0.dist-info/top_level.txt
--rw-rw-r--  2.0 fat      564 b- defN 23-Apr-25 19:19 extended_tk-0.12.0.dist-info/RECORD
-7 files, 20825 bytes uncompressed, 6170 bytes compressed:  70.4%
+-rw-rw-rw-  2.0 fat     9977 b- defN 23-May-05 10:40 extended_tk/__init__.py
+-rw-rw-rw-  2.0 fat      243 b- defN 23-May-05 11:48 extended_tk-0.13.0.dist-info/LICENSE
+-rw-rw-rw-  2.0 fat      717 b- defN 23-May-05 11:48 extended_tk-0.13.0.dist-info/METADATA
+-rw-rw-rw-  2.0 fat       92 b- defN 23-May-05 11:48 extended_tk-0.13.0.dist-info/WHEEL
+-rw-rw-rw-  2.0 fat       12 b- defN 23-May-05 11:48 extended_tk-0.13.0.dist-info/top_level.txt
+-rw-rw-r--  2.0 fat      564 b- defN 23-May-05 11:48 extended_tk-0.13.0.dist-info/RECORD
+7 files, 21057 bytes uncompressed, 6202 bytes compressed:  70.5%
```

## zipnote {}

```diff
@@ -1,22 +1,22 @@
 Filename: TkPlus/__init__.py
 Comment: 
 
 Filename: extended_tk/__init__.py
 Comment: 
 
-Filename: extended_tk-0.12.0.dist-info/LICENSE
+Filename: extended_tk-0.13.0.dist-info/LICENSE
 Comment: 
 
-Filename: extended_tk-0.12.0.dist-info/METADATA
+Filename: extended_tk-0.13.0.dist-info/METADATA
 Comment: 
 
-Filename: extended_tk-0.12.0.dist-info/WHEEL
+Filename: extended_tk-0.13.0.dist-info/WHEEL
 Comment: 
 
-Filename: extended_tk-0.12.0.dist-info/top_level.txt
+Filename: extended_tk-0.13.0.dist-info/top_level.txt
 Comment: 
 
-Filename: extended_tk-0.12.0.dist-info/RECORD
+Filename: extended_tk-0.13.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## extended_tk/__init__.py

```diff
@@ -218,14 +218,22 @@
     def __updateScrollRegion(self, event):
         self.update_idletasks()
         self.config(scrollregion=self.frame.bbox())
         
     def __on_mousewheel(self, event):
         self.yview_scroll(-1*int(event.delta/120), "units")
         
+    def collect_children(self, *args, **kwargs): #TODO: crear la opción de filtrar los children
+        collected = []
+        for i in self.__dict__['children'].values():
+            for kind in args:
+                if isinstance(i, kind):
+                    collected.append(i)
+        return collected
+        
 class TerminalWindow(Frame):
     '''
     A simplified way to create a scrollable window
     '''
     def __init__(self, master, max_width):
         Frame.__init__(self, master)
```

### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

## Comparing `extended_tk-0.12.0.dist-info/METADATA` & `extended_tk-0.13.0.dist-info/METADATA`

 * *Files 14% similar despite different names*

```diff
@@ -1,24 +1,23 @@
 Metadata-Version: 2.1
 Name: extended-tk
-Version: 0.12.0
+Version: 0.13.0
 Summary: An add on for the tkinter package
 Home-page: UNKNOWN
 Author: Elidas
 License: GNUGPLv3
 Keywords: Tkinter
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Developers
 Classifier: Topic :: Utilities
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 License-File: LICENSE
 
-AmpliaciÃ³n del paquete TkInter con herramientas desarrolladas por necesidad de proyecto.
 This program is free software: you can redistribute it and/or modify it under
 the terms of the GNU General Public License as published by the Free software
 Foundation, either version 3 of the License, or (at your option) any later
 version
```

### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

## Comparing `extended_tk-0.12.0.dist-info/RECORD` & `extended_tk-0.13.0.dist-info/RECORD`

 * *Files 14% similar despite different names*

```diff
@@ -1,7 +1,7 @@
 TkPlus/__init__.py,sha256=fAwcO_zH-AjYKskxRbSUn8TYHsPlVYhs-EybaQDFEw0,9452
-extended_tk/__init__.py,sha256=hBnVgf6-6YS2jsCQlBWwgv-TwoJXteJ-9brF_9hrceQ,9652
-extended_tk-0.12.0.dist-info/LICENSE,sha256=EEAxqxJsjMTyZM0BicuoXjdyUB4VE45rvk83t_jv4uw,243
-extended_tk-0.12.0.dist-info/METADATA,sha256=cKFl3HvBI3azW7EVInA9Pl6uywDlHzuHCgY1U-4ITDI,810
-extended_tk-0.12.0.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
-extended_tk-0.12.0.dist-info/top_level.txt,sha256=A40P8PzvnRpYXa0VqJc51K-aiI4LicWN2h8yzvJfO9Q,12
-extended_tk-0.12.0.dist-info/RECORD,,
+extended_tk/__init__.py,sha256=c1kZ0Y-ebfUnBKNX8ctG4_X32nqrj_TFzx6WMPJhxY8,9977
+extended_tk-0.13.0.dist-info/LICENSE,sha256=EEAxqxJsjMTyZM0BicuoXjdyUB4VE45rvk83t_jv4uw,243
+extended_tk-0.13.0.dist-info/METADATA,sha256=JhGoVwUWoO0kT18GzwsJgBDlkG3SRTQXAQD81ksrpVY,717
+extended_tk-0.13.0.dist-info/WHEEL,sha256=pkctZYzUS4AYVn6dJ-7367OJZivF2e8RA9b_ZBjif18,92
+extended_tk-0.13.0.dist-info/top_level.txt,sha256=A40P8PzvnRpYXa0VqJc51K-aiI4LicWN2h8yzvJfO9Q,12
+extended_tk-0.13.0.dist-info/RECORD,,
```

