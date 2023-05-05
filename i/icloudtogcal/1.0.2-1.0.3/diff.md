# Comparing `tmp/icloudtogcal-1.0.2-py3-none-any.whl.zip` & `tmp/icloudtogcal-1.0.3-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,21 +1,21 @@
-Zip file size: 9143335 bytes, number of entries: 19
+Zip file size: 9143327 bytes, number of entries: 19
 -rw-r--r--  2.0 fat     1128 b- defN 80-Jan-01 00:00 iCloudToGCal/__init__.py
 -rw-r--r--  2.0 fat        0 b- defN 80-Jan-01 00:00 iCloudToGCal/__main__.py
 -rw-r--r--  2.0 fat      367 b- defN 80-Jan-01 00:00 iCloudToGCal/__version__.py
 -rw-r--r--  2.0 fat        0 b- defN 80-Jan-01 00:00 iCloudToGCal/chromedriver/__init__.py
--rw-r--r--  2.0 fat     4189 b- defN 80-Jan-01 00:00 iCloudToGCal/chromedriver/installDriver.py
+-rw-r--r--  2.0 fat     4180 b- defN 80-Jan-01 00:00 iCloudToGCal/chromedriver/installDriver.py
 -rw-r--r--  2.0 fat        0 b- defN 80-Jan-01 00:00 iCloudToGCal/GUI/__init__.py
 -rw-r--r--  2.0 fat 20131386 b- defN 80-Jan-01 00:00 iCloudToGCal/GUI/create.py
--rw-r--r--  2.0 fat     4565 b- defN 80-Jan-01 00:00 iCloudToGCal/GUI/GUI.py
+-rw-r--r--  2.0 fat     4536 b- defN 80-Jan-01 00:00 iCloudToGCal/GUI/GUI.py
 -rw-r--r--  2.0 fat        0 b- defN 80-Jan-01 00:00 iCloudToGCal/processdata/__init__.py
 -rw-r--r--  2.0 fat      283 b- defN 80-Jan-01 00:00 iCloudToGCal/processdata/data.py
 -rw-r--r--  2.0 fat     2123 b- defN 80-Jan-01 00:00 iCloudToGCal/processdata/processAttendence.py
 -rw-r--r--  2.0 fat     9626 b- defN 80-Jan-01 00:00 iCloudToGCal/processdata/processTable.py
 -rw-r--r--  2.0 fat        0 b- defN 80-Jan-01 00:00 iCloudToGCal/selenuimFunctions/__init__.py
 -rw-r--r--  2.0 fat     2320 b- defN 80-Jan-01 00:00 iCloudToGCal/selenuimFunctions/Gform.py
 -rw-r--r--  2.0 fat     3191 b- defN 80-Jan-01 00:00 iCloudToGCal/selenuimFunctions/iCloud.py
--rw-r--r--  2.0 fat       95 b- defN 80-Jan-01 00:00 icloudtogcal-1.0.2.dist-info/entry_points.txt
--rw-r--r--  2.0 fat      893 b- defN 80-Jan-01 00:00 icloudtogcal-1.0.2.dist-info/METADATA
--rw-r--r--  2.0 fat       88 b- defN 80-Jan-01 00:00 icloudtogcal-1.0.2.dist-info/WHEEL
-?rw-r--r--  2.0 fat     1667 b- defN 16-Jan-01 00:00 icloudtogcal-1.0.2.dist-info/RECORD
-19 files, 20161921 bytes uncompressed, 9140557 bytes compressed:  54.7%
+-rw-r--r--  2.0 fat       95 b- defN 80-Jan-01 00:00 icloudtogcal-1.0.3.dist-info/entry_points.txt
+-rw-r--r--  2.0 fat      893 b- defN 80-Jan-01 00:00 icloudtogcal-1.0.3.dist-info/METADATA
+-rw-r--r--  2.0 fat       88 b- defN 80-Jan-01 00:00 icloudtogcal-1.0.3.dist-info/WHEEL
+?rw-r--r--  2.0 fat     1667 b- defN 16-Jan-01 00:00 icloudtogcal-1.0.3.dist-info/RECORD
+19 files, 20161883 bytes uncompressed, 9140549 bytes compressed:  54.7%
```

## zipnote {}

```diff
@@ -39,20 +39,20 @@
 
 Filename: iCloudToGCal/selenuimFunctions/Gform.py
 Comment: 
 
 Filename: iCloudToGCal/selenuimFunctions/iCloud.py
 Comment: 
 
-Filename: icloudtogcal-1.0.2.dist-info/entry_points.txt
+Filename: icloudtogcal-1.0.3.dist-info/entry_points.txt
 Comment: 
 
-Filename: icloudtogcal-1.0.2.dist-info/METADATA
+Filename: icloudtogcal-1.0.3.dist-info/METADATA
 Comment: 
 
-Filename: icloudtogcal-1.0.2.dist-info/WHEEL
+Filename: icloudtogcal-1.0.3.dist-info/WHEEL
 Comment: 
 
-Filename: icloudtogcal-1.0.2.dist-info/RECORD
+Filename: icloudtogcal-1.0.3.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## iCloudToGCal/chromedriver/installDriver.py

```diff
@@ -1,9 +1,9 @@
 import os
-
+from ..GUI.create import create_desktop_icon
 
 def add_to_path(path):
     """
     Adds a path to the PATH environment variable
     """
     import winreg
     key = winreg.OpenKey(
@@ -72,15 +72,14 @@
 
 def check_for_resources():
     """
     Checks if the resources folder exists
     if it does not exist it creates it
     """
     if not os.path.exists("C:\\icloud_resources"):
-        from .GUI.create import create_desktop_icon
         create_desktop_icon()
         os.makedirs("C:\\icloud_resources")
     if not os.path.exists("C:\\icloud_resources\\record.json"):
         with open("C:\\icloud_resources\\record.json", "w") as f:
             f.write("{}")
     if not os.path.exists("C:\\icloud_resources\\cerdential.txt"):
         with open("C:\\icloud_resources\\cerdential.txt", "w") as f:
```

## iCloudToGCal/GUI/GUI.py

```diff
@@ -1,9 +1,9 @@
 from iCloudToGCal.selenuimFunctions.iCloud import openiCloud
-from iCloudToGCal.chromedriver.installDriver import install_driver
+from iCloudToGCal.chromedriver.installDriver import install_driver,create_desktop_icon
 from time import sleep
 def check_if_ID_pass_is_correct(username, password, app, finishLabel, button1):
 
     finishLabel.configure(text="Verifying...")
     button1.configure(state="disabled")
     driver = openiCloud(username=username,password=password)
     if driver.current_url == "https://gu.icloudems.com/corecampus/index.php":
@@ -83,15 +83,14 @@
     entry2.pack(pady=12, padx=10)
 
     entry3 = customtkinter.CTkEntry(master=frame, placeholder_text="Form Link")
     entry3.pack(pady=12, padx=10)
 
     button1 = customtkinter.CTkButton(master=frame, text="Submit", command=submit)
     button1.pack(pady=12, padx=10)
-    from .GUI.create import create_desktop_icon
     button2 = customtkinter.CTkButton(master=frame, text="Add Icon", command=create_desktop_icon)
     button2.pack(pady=12, padx=10)
 
     finishLabel = customtkinter.CTkLabel(frame, text=s)
     finishLabel.pack(pady=20)
 
     # about_text_outer = customtkinter.CTkLabel(master=frame, text="")
```

## Comparing `icloudtogcal-1.0.2.dist-info/METADATA` & `icloudtogcal-1.0.3.dist-info/METADATA`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: icloudtogcal
-Version: 1.0.2
+Version: 1.0.3
 Summary: Sync iCloud events to Google Calendar
 Home-page: https://github.com/fjueic/iCloud-to-Google-Calender.git
 Author: Rohit
 Author-email: rohitmalik987789@gmail.com
 Requires-Python: >=3.7,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.7
```

## Comparing `icloudtogcal-1.0.2.dist-info/RECORD` & `icloudtogcal-1.0.3.dist-info/RECORD`

 * *Files 9% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 iCloudToGCal/__init__.py,sha256=jpP_Pa6dJw9AfVBIquq6WzP5e54nFNIlRgcOnxIoZV0,1128
 iCloudToGCal/__main__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 iCloudToGCal/__version__.py,sha256=XHymZfMIvtCL5DF_Xt-13bcGUNY6MSSi1z_smm7hwNY,367
 iCloudToGCal/chromedriver/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-iCloudToGCal/chromedriver/installDriver.py,sha256=YK6pewGKAjQR7p8d_eyrlbZqcc5RaOYyqdRXzhA0IRQ,4189
+iCloudToGCal/chromedriver/installDriver.py,sha256=g-vqxOpUNk6grudaxnyrb-T1u0BuiTEk1IuNJNeuGr4,4180
 iCloudToGCal/GUI/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 iCloudToGCal/GUI/create.py,sha256=bUCn14GCky5_zXqaSqRIXE0E_0IMtj3W4S1XdZz_qS8,20131386
-iCloudToGCal/GUI/GUI.py,sha256=HYBo11A5AqMIUjqpzs1FNnZkhWcRdrm-j4AVFfTJ_rk,4565
+iCloudToGCal/GUI/GUI.py,sha256=m2OK3V-hChfZJCRI3s7L3vmOimu-L4Xad9yNDl5E05k,4536
 iCloudToGCal/processdata/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 iCloudToGCal/processdata/data.py,sha256=efYrdaWtqjfnFWeuw0r3uY7-a5YrSUos4jvk7e2PLu4,283
 iCloudToGCal/processdata/processAttendence.py,sha256=F_E7yt2am4yCWV5c_bdo8C1IkY5KwaXNQxBxfXwa3bk,2123
 iCloudToGCal/processdata/processTable.py,sha256=0U4etX2DrRQfQjxZeEf0AxvgyABrMpMjX9cT3_wlwjk,9626
 iCloudToGCal/selenuimFunctions/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 iCloudToGCal/selenuimFunctions/Gform.py,sha256=p64bS5sLedDJI54f6VT9rbHgG9xNKx-sOH0R3qQ0ue0,2320
 iCloudToGCal/selenuimFunctions/iCloud.py,sha256=hQQ6Xj9Pwn0l71-J_NkMogAbcxLJ4_M6gNGYp0p0GnQ,3191
-icloudtogcal-1.0.2.dist-info/entry_points.txt,sha256=kCuX_JN2KExOH4PT-MNxNZjGldmGeYqkoFEz0kxNDFY,95
-icloudtogcal-1.0.2.dist-info/METADATA,sha256=4ViHVC8RSgn5h3Qo_CDgCIxV1gUNZTf9OPLtX8yL0e8,893
-icloudtogcal-1.0.2.dist-info/WHEEL,sha256=7Z8_27uaHI_UZAc4Uox4PpBhQ9Y5_modZXWMxtUi4NU,88
-icloudtogcal-1.0.2.dist-info/RECORD,,
+icloudtogcal-1.0.3.dist-info/entry_points.txt,sha256=kCuX_JN2KExOH4PT-MNxNZjGldmGeYqkoFEz0kxNDFY,95
+icloudtogcal-1.0.3.dist-info/METADATA,sha256=2Az03t31Q7Lle6hMHCDXPmelWCyqQqilh2bzk8E7cfA,893
+icloudtogcal-1.0.3.dist-info/WHEEL,sha256=7Z8_27uaHI_UZAc4Uox4PpBhQ9Y5_modZXWMxtUi4NU,88
+icloudtogcal-1.0.3.dist-info/RECORD,,
```

