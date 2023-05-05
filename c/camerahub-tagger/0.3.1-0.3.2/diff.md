# Comparing `tmp/camerahub_tagger-0.3.1.tar.gz` & `tmp/camerahub_tagger-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "camerahub_tagger-0.3.1.tar", max compression
+gzip compressed data, was "camerahub_tagger-0.3.2.tar", max compression
```

## Comparing `camerahub_tagger-0.3.1.tar` & `camerahub_tagger-0.3.2.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     2839 2023-04-28 09:55:07.337266 camerahub_tagger-0.3.1/README.md
--rw-r--r--   0        0        0        0 2023-04-28 09:55:07.337266 camerahub_tagger-0.3.1/camerahub_tagger/__init__.py
--rw-r--r--   0        0        0     2049 2023-04-28 09:55:07.337266 camerahub_tagger-0.3.1/camerahub_tagger/api.py
--rw-r--r--   0        0        0     2037 2023-04-28 09:55:07.337266 camerahub_tagger-0.3.1/camerahub_tagger/config.py
--rw-r--r--   0        0        0     6899 2023-04-28 09:55:07.337266 camerahub_tagger-0.3.1/camerahub_tagger/funcs.py
--rwxr-xr-x   0        0        0     6296 2023-04-28 09:55:07.337266 camerahub_tagger-0.3.1/camerahub_tagger/main.py
--rw-r--r--   0        0        0      670 2023-04-28 09:55:31.321518 camerahub_tagger-0.3.1/pyproject.toml
--rw-r--r--   0        0        0     3607 1970-01-01 00:00:00.000000 camerahub_tagger-0.3.1/PKG-INFO
+-rw-r--r--   0        0        0     2839 2023-05-05 12:23:20.387669 camerahub_tagger-0.3.2/README.md
+-rw-r--r--   0        0        0        0 2023-05-05 12:23:20.387669 camerahub_tagger-0.3.2/camerahub_tagger/__init__.py
+-rw-r--r--   0        0        0     2049 2023-05-05 12:23:20.387669 camerahub_tagger-0.3.2/camerahub_tagger/api.py
+-rw-r--r--   0        0        0     2037 2023-05-05 12:23:20.387669 camerahub_tagger-0.3.2/camerahub_tagger/config.py
+-rw-r--r--   0        0        0     6899 2023-05-05 12:23:20.387669 camerahub_tagger-0.3.2/camerahub_tagger/funcs.py
+-rwxr-xr-x   0        0        0     6637 2023-05-05 12:23:20.387669 camerahub_tagger-0.3.2/camerahub_tagger/main.py
+-rw-r--r--   0        0        0      670 2023-05-05 12:23:42.328008 camerahub_tagger-0.3.2/pyproject.toml
+-rw-r--r--   0        0        0     3607 1970-01-01 00:00:00.000000 camerahub_tagger-0.3.2/PKG-INFO
```

### Comparing `camerahub_tagger-0.3.1/README.md` & `camerahub_tagger-0.3.2/README.md`

 * *Files identical despite different names*

### Comparing `camerahub_tagger-0.3.1/camerahub_tagger/api.py` & `camerahub_tagger-0.3.2/camerahub_tagger/api.py`

 * *Files identical despite different names*

### Comparing `camerahub_tagger-0.3.1/camerahub_tagger/config.py` & `camerahub_tagger-0.3.2/camerahub_tagger/config.py`

 * *Files identical despite different names*

### Comparing `camerahub_tagger-0.3.1/camerahub_tagger/funcs.py` & `camerahub_tagger-0.3.2/camerahub_tagger/funcs.py`

 * *Files identical despite different names*

### Comparing `camerahub_tagger-0.3.1/camerahub_tagger/main.py` & `camerahub_tagger-0.3.2/camerahub_tagger/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -75,16 +75,29 @@
 
     # foreach found photo:
     # read exif data, check for camerahub scan tag
     for file in files:
         print(f"Processing image {file}")
 
         # Extract exif data from file
-        with pyexiv2.Image(file) as img:
+        try:
+            img = pyexiv2.Image(file)
+        except RuntimeError as err:
+            cprint(f"{err} when reading {file}", "red")
+            failed.append(file)
+            continue
+
+        try:
             existing = img.read_exif()
+        except UnicodeDecodeError as err:
+            cprint(f"{err} when reading {file}", "red")
+            failed.append(file)
+            continue
+
+        img.close()
 
         # Example format
         # existing = {'Exif.Image.DateTime': '2019:06:23 19:45:17', 'Exif.Image.Artist': 'TEST', 'Exif.Image.Rating': '4', ...}
 
         if existing is not None and 'Exif.Photo.ImageUniqueID' in existing and is_valid_uuid(existing['Exif.Photo.ImageUniqueID']):
             # check for presence of custom exif tag for camerahub
             # already has a uuid scan id
```

### Comparing `camerahub_tagger-0.3.1/pyproject.toml` & `camerahub_tagger-0.3.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "camerahub-tagger"
-version = "0.3.1"
+version = "0.3.2"
 description = "EXIF tagger for CameraHub"
 authors = ["Jonathan Gazeley <me@jonathangazeley.com>"]
 repository = "https://github.com/camerahub/tagger"
 homepage = "https://camerahub.info/"
 readme = ["README.md"]
 keywords = ["EXIF", "photography", "CameraHub", "metadata"]
```

### Comparing `camerahub_tagger-0.3.1/PKG-INFO` & `camerahub_tagger-0.3.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: camerahub-tagger
-Version: 0.3.1
+Version: 0.3.2
 Summary: EXIF tagger for CameraHub
 Home-page: https://camerahub.info/
 Keywords: EXIF,photography,CameraHub,metadata
 Author: Jonathan Gazeley
 Author-email: me@jonathangazeley.com
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
```

