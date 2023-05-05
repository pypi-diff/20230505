# Comparing `tmp/camerahub_tagger-0.3.2.tar.gz` & `tmp/camerahub_tagger-0.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "camerahub_tagger-0.3.2.tar", max compression
+gzip compressed data, was "camerahub_tagger-0.3.3.tar", max compression
```

## Comparing `camerahub_tagger-0.3.2.tar` & `camerahub_tagger-0.3.3.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     2839 2023-05-05 12:23:20.387669 camerahub_tagger-0.3.2/README.md
--rw-r--r--   0        0        0        0 2023-05-05 12:23:20.387669 camerahub_tagger-0.3.2/camerahub_tagger/__init__.py
--rw-r--r--   0        0        0     2049 2023-05-05 12:23:20.387669 camerahub_tagger-0.3.2/camerahub_tagger/api.py
--rw-r--r--   0        0        0     2037 2023-05-05 12:23:20.387669 camerahub_tagger-0.3.2/camerahub_tagger/config.py
--rw-r--r--   0        0        0     6899 2023-05-05 12:23:20.387669 camerahub_tagger-0.3.2/camerahub_tagger/funcs.py
--rwxr-xr-x   0        0        0     6637 2023-05-05 12:23:20.387669 camerahub_tagger-0.3.2/camerahub_tagger/main.py
--rw-r--r--   0        0        0      670 2023-05-05 12:23:42.328008 camerahub_tagger-0.3.2/pyproject.toml
--rw-r--r--   0        0        0     3607 1970-01-01 00:00:00.000000 camerahub_tagger-0.3.2/PKG-INFO
+-rw-r--r--   0        0        0     2839 2023-05-05 19:40:16.542147 camerahub_tagger-0.3.3/README.md
+-rw-r--r--   0        0        0        0 2023-05-05 19:40:16.542147 camerahub_tagger-0.3.3/camerahub_tagger/__init__.py
+-rw-r--r--   0        0        0     2159 2023-05-05 19:40:16.542147 camerahub_tagger-0.3.3/camerahub_tagger/api.py
+-rw-r--r--   0        0        0     2037 2023-05-05 19:40:16.542147 camerahub_tagger-0.3.3/camerahub_tagger/config.py
+-rw-r--r--   0        0        0     6899 2023-05-05 19:40:16.542147 camerahub_tagger-0.3.3/camerahub_tagger/funcs.py
+-rwxr-xr-x   0        0        0     7043 2023-05-05 19:40:16.542147 camerahub_tagger-0.3.3/camerahub_tagger/main.py
+-rw-r--r--   0        0        0      670 2023-05-05 19:40:33.226040 camerahub_tagger-0.3.3/pyproject.toml
+-rw-r--r--   0        0        0     3607 1970-01-01 00:00:00.000000 camerahub_tagger-0.3.3/PKG-INFO
```

### Comparing `camerahub_tagger-0.3.2/README.md` & `camerahub_tagger-0.3.3/README.md`

 * *Files identical despite different names*

### Comparing `camerahub_tagger-0.3.2/camerahub_tagger/api.py` & `camerahub_tagger-0.3.3/camerahub_tagger/api.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 """
 Functions which interact with the CameraHub API
 """
 
 from datetime import date
+from os.path import basename
 import json
 import requests
 
 def test_credentials(l_server, l_auth):
     """
     Validate a set of credentials
     :param server:
@@ -32,14 +33,17 @@
         "negative": null,
         "print": null,
         "filename": "",
         "date": null
     }
     """
 
+    # Only write the basename of the file
+    l_filename = basename(l_filename)
+
     # Create dict
     data = {
         'negative': l_negative,
         'filename': l_filename,
         'date': date.today()}
     url = l_server+'/scan/'
     response = requests.post(
```

### Comparing `camerahub_tagger-0.3.2/camerahub_tagger/config.py` & `camerahub_tagger-0.3.3/camerahub_tagger/config.py`

 * *Files identical despite different names*

### Comparing `camerahub_tagger-0.3.2/camerahub_tagger/funcs.py` & `camerahub_tagger-0.3.3/camerahub_tagger/funcs.py`

 * *Files identical despite different names*

### Comparing `camerahub_tagger-0.3.2/camerahub_tagger/main.py` & `camerahub_tagger-0.3.3/camerahub_tagger/main.py`

 * *Files 3% similar despite different names*

```diff
@@ -69,14 +69,17 @@
         cprint("No files found", "red")
 
     # set up summary counters
     changed = []
     unchanged = []
     failed = []
 
+    # Disable pyexiv logging to work around issue #37
+    pyexiv2.set_log_level(4)
+
     # foreach found photo:
     # read exif data, check for camerahub scan tag
     for file in files:
         print(f"Processing image {file}")
 
         # Extract exif data from file
         try:
@@ -133,14 +136,19 @@
                 continue
             else:
                 print(f"{file} corresponds to Negative {negative}")
 
             # Create Scan record associated with the Negative
             try:
                 scan = create_scan(negative, file, server, auth)
+
+                # Opportunistically write the new Scan ID to the file in case Tagger runs into problems
+                # later - otherwise the Scan ID would be lost and a new one generated next time
+                with pyexiv2.Image(file) as img:
+                    img.modify_exif({'Exif.Photo.ImageUniqueID': scan})
             except:
                 cprint(f"Couldn't generate Scan ID for Negative {negative}", "red")
                 failed.append(file)
                 continue
             else:
                 print(f"Created new Scan ID {scan}")
```

### Comparing `camerahub_tagger-0.3.2/pyproject.toml` & `camerahub_tagger-0.3.3/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "camerahub-tagger"
-version = "0.3.2"
+version = "0.3.3"
 description = "EXIF tagger for CameraHub"
 authors = ["Jonathan Gazeley <me@jonathangazeley.com>"]
 repository = "https://github.com/camerahub/tagger"
 homepage = "https://camerahub.info/"
 readme = ["README.md"]
 keywords = ["EXIF", "photography", "CameraHub", "metadata"]
```

### Comparing `camerahub_tagger-0.3.2/PKG-INFO` & `camerahub_tagger-0.3.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: camerahub-tagger
-Version: 0.3.2
+Version: 0.3.3
 Summary: EXIF tagger for CameraHub
 Home-page: https://camerahub.info/
 Keywords: EXIF,photography,CameraHub,metadata
 Author: Jonathan Gazeley
 Author-email: me@jonathangazeley.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
```

