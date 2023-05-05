# Comparing `tmp/Office_helper_functions-0.1.12.tar.gz` & `tmp/Office_helper_functions-0.1.13.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Office_helper_functions-0.1.12.tar", last modified: Fri May  5 19:49:52 2023, max compression
+gzip compressed data, was "Office_helper_functions-0.1.13.tar", last modified: Fri May  5 19:58:28 2023, max compression
```

## Comparing `Office_helper_functions-0.1.12.tar` & `Office_helper_functions-0.1.13.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxrwx   0        0        0        0 2023-05-05 19:49:52.488957 Office_helper_functions-0.1.12/
-drwxrwxrwx   0        0        0        0 2023-05-05 19:49:52.452784 Office_helper_functions-0.1.12/Office_helper_functions/
--rw-rw-rw-   0        0        0     3175 2023-05-04 20:51:57.000000 Office_helper_functions-0.1.12/Office_helper_functions/Dates.py
-drwxrwxrwx   0        0        0        0 2023-05-05 19:49:52.481677 Office_helper_functions-0.1.12/Office_helper_functions/Image/
--rw-rw-rw-   0        0        0     1418 2023-05-04 20:40:27.000000 Office_helper_functions-0.1.12/Office_helper_functions/Image/Image_operations.py
--rw-rw-rw-   0        0        0        0 2023-05-04 20:41:09.000000 Office_helper_functions-0.1.12/Office_helper_functions/Image/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-05 19:49:52.486340 Office_helper_functions-0.1.12/Office_helper_functions/Word/
--rw-rw-rw-   0        0        0     2477 2023-05-05 19:33:25.000000 Office_helper_functions-0.1.12/Office_helper_functions/Word/Word_Image.py
--rw-rw-rw-   0        0        0        0 2023-05-04 20:52:17.000000 Office_helper_functions-0.1.12/Office_helper_functions/Word/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-05 19:49:52.488957 Office_helper_functions-0.1.12/Office_helper_functions/Word/checkbox/
--rw-rw-rw-   0        0        0        0 2023-05-04 19:59:26.000000 Office_helper_functions-0.1.12/Office_helper_functions/Word/checkbox/__init__.py
--rw-rw-rw-   0        0        0     3121 2023-05-05 19:47:04.000000 Office_helper_functions-0.1.12/Office_helper_functions/Word/form_field.py
--rw-rw-rw-   0        0        0        0 2023-05-04 19:59:16.000000 Office_helper_functions-0.1.12/Office_helper_functions/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-05 19:49:52.474743 Office_helper_functions-0.1.12/Office_helper_functions.egg-info/
--rw-rw-rw-   0        0        0      202 2023-05-05 19:49:52.000000 Office_helper_functions-0.1.12/Office_helper_functions.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      534 2023-05-05 19:49:52.000000 Office_helper_functions-0.1.12/Office_helper_functions.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-05 19:49:52.000000 Office_helper_functions-0.1.12/Office_helper_functions.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       24 2023-05-05 19:49:52.000000 Office_helper_functions-0.1.12/Office_helper_functions.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      202 2023-05-05 19:49:52.488957 Office_helper_functions-0.1.12/PKG-INFO
--rw-rw-rw-   0        0        0       42 2023-05-05 19:49:52.491703 Office_helper_functions-0.1.12/setup.cfg
--rw-rw-rw-   0        0        0      354 2023-05-05 19:49:44.000000 Office_helper_functions-0.1.12/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-05 19:58:28.910556 Office_helper_functions-0.1.13/
+drwxrwxrwx   0        0        0        0 2023-05-05 19:58:28.861563 Office_helper_functions-0.1.13/Office_helper_functions/
+-rw-rw-rw-   0        0        0     3175 2023-05-04 20:51:57.000000 Office_helper_functions-0.1.13/Office_helper_functions/Dates.py
+drwxrwxrwx   0        0        0        0 2023-05-05 19:58:28.897244 Office_helper_functions-0.1.13/Office_helper_functions/Image/
+-rw-rw-rw-   0        0        0     1418 2023-05-04 20:40:27.000000 Office_helper_functions-0.1.13/Office_helper_functions/Image/Image_operations.py
+-rw-rw-rw-   0        0        0        0 2023-05-04 20:41:09.000000 Office_helper_functions-0.1.13/Office_helper_functions/Image/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-05 19:58:28.902265 Office_helper_functions-0.1.13/Office_helper_functions/Word/
+-rw-rw-rw-   0        0        0     2477 2023-05-05 19:33:25.000000 Office_helper_functions-0.1.13/Office_helper_functions/Word/Word_Image.py
+-rw-rw-rw-   0        0        0        0 2023-05-04 20:52:17.000000 Office_helper_functions-0.1.13/Office_helper_functions/Word/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-05 19:58:28.902265 Office_helper_functions-0.1.13/Office_helper_functions/Word/checkbox/
+-rw-rw-rw-   0        0        0        0 2023-05-04 19:59:26.000000 Office_helper_functions-0.1.13/Office_helper_functions/Word/checkbox/__init__.py
+-rw-rw-rw-   0        0        0     3138 2023-05-05 19:57:26.000000 Office_helper_functions-0.1.13/Office_helper_functions/Word/form_field.py
+-rw-rw-rw-   0        0        0        0 2023-05-04 19:59:16.000000 Office_helper_functions-0.1.13/Office_helper_functions/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-05 19:58:28.891016 Office_helper_functions-0.1.13/Office_helper_functions.egg-info/
+-rw-rw-rw-   0        0        0      202 2023-05-05 19:58:28.000000 Office_helper_functions-0.1.13/Office_helper_functions.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      534 2023-05-05 19:58:28.000000 Office_helper_functions-0.1.13/Office_helper_functions.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-05 19:58:28.000000 Office_helper_functions-0.1.13/Office_helper_functions.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       24 2023-05-05 19:58:28.000000 Office_helper_functions-0.1.13/Office_helper_functions.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      202 2023-05-05 19:58:28.910556 Office_helper_functions-0.1.13/PKG-INFO
+-rw-rw-rw-   0        0        0       42 2023-05-05 19:58:28.910556 Office_helper_functions-0.1.13/setup.cfg
+-rw-rw-rw-   0        0        0      354 2023-05-05 19:58:13.000000 Office_helper_functions-0.1.13/setup.py
```

### Comparing `Office_helper_functions-0.1.12/Office_helper_functions/Dates.py` & `Office_helper_functions-0.1.13/Office_helper_functions/Dates.py`

 * *Files identical despite different names*

### Comparing `Office_helper_functions-0.1.12/Office_helper_functions/Image/Image_operations.py` & `Office_helper_functions-0.1.13/Office_helper_functions/Image/Image_operations.py`

 * *Files identical despite different names*

### Comparing `Office_helper_functions-0.1.12/Office_helper_functions/Word/Word_Image.py` & `Office_helper_functions-0.1.13/Office_helper_functions/Word/Word_Image.py`

 * *Files identical despite different names*

### Comparing `Office_helper_functions-0.1.12/Office_helper_functions/Word/form_field.py` & `Office_helper_functions-0.1.13/Office_helper_functions/Word/form_field.py`

 * *Files 2% similar despite different names*

```diff
@@ -55,15 +55,15 @@
     """
     with zipfile.ZipFile(io.BytesIO(word_file), mode='r') as zf:
 
         files = {x: zf.read(x) for x in zf.namelist()}
 
     # Create a new in-memory ZipFile object
     new_word_file = io.BytesIO()
-    with zipfile.ZipFile(new_word_file, mode='w', compression=zipfile.ZIP_DEFLATED) as zkf:
+    with zipfile.ZipFile(new_word_file, mode='w', compression=zipfile.ZIP_DEFLATED, compresslevel=9) as zkf:
         for name, file in files.items():
             # Add each file to the new zipfile
             zkf.writestr(name, file)
 
     # Reset the output_zip's file pointer to the beginning
     new_word_file.seek(0)
     return new_word_file
```

### Comparing `Office_helper_functions-0.1.12/Office_helper_functions.egg-info/SOURCES.txt` & `Office_helper_functions-0.1.13/Office_helper_functions.egg-info/SOURCES.txt`

 * *Files identical despite different names*

