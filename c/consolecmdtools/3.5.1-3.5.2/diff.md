# Comparing `tmp/consolecmdtools-3.5.1.tar.gz` & `tmp/consolecmdtools-3.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "consolecmdtools-3.5.1.tar", last modified: Fri May  5 03:42:19 2023, max compression
+gzip compressed data, was "consolecmdtools-3.5.2.tar", last modified: Fri May  5 04:11:02 2023, max compression
```

## Comparing `consolecmdtools-3.5.1.tar` & `consolecmdtools-3.5.2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 kyan001    (501) staff       (20)        0 2023-05-05 03:42:19.133686 consolecmdtools-3.5.1/
--rw-r--r--   0 kyan001    (501) staff       (20)     1061 2020-11-09 08:36:27.000000 consolecmdtools-3.5.1/LICENSE
--rw-r--r--   0 kyan001    (501) staff       (20)     7368 2023-05-05 03:42:19.133023 consolecmdtools-3.5.1/PKG-INFO
--rw-r--r--   0 kyan001    (501) staff       (20)     5293 2023-05-05 03:39:04.000000 consolecmdtools-3.5.1/README.md
-drwxr-xr-x   0 kyan001    (501) staff       (20)        0 2023-05-05 03:42:19.123893 consolecmdtools-3.5.1/consolecmdtools/
--rw-r--r--   0 kyan001    (501) staff       (20)    15613 2023-05-05 03:39:04.000000 consolecmdtools-3.5.1/consolecmdtools/__init__.py
--rw-r--r--   0 kyan001    (501) staff       (20)     2037 2022-12-25 10:04:52.000000 consolecmdtools-3.5.1/consolecmdtools/__main__.py
-drwxr-xr-x   0 kyan001    (501) staff       (20)        0 2023-05-05 03:42:19.128894 consolecmdtools-3.5.1/consolecmdtools.egg-info/
--rw-r--r--   0 kyan001    (501) staff       (20)     7368 2023-05-05 03:42:19.000000 consolecmdtools-3.5.1/consolecmdtools.egg-info/PKG-INFO
--rw-r--r--   0 kyan001    (501) staff       (20)      332 2023-05-05 03:42:19.000000 consolecmdtools-3.5.1/consolecmdtools.egg-info/SOURCES.txt
--rw-r--r--   0 kyan001    (501) staff       (20)        1 2023-05-05 03:42:19.000000 consolecmdtools-3.5.1/consolecmdtools.egg-info/dependency_links.txt
--rw-r--r--   0 kyan001    (501) staff       (20)       60 2023-05-05 03:42:19.000000 consolecmdtools-3.5.1/consolecmdtools.egg-info/requires.txt
--rw-r--r--   0 kyan001    (501) staff       (20)       21 2023-05-05 03:42:19.000000 consolecmdtools-3.5.1/consolecmdtools.egg-info/top_level.txt
--rw-r--r--   0 kyan001    (501) staff       (20)     1230 2022-12-25 10:04:52.000000 consolecmdtools-3.5.1/pyproject.toml
--rw-r--r--   0 kyan001    (501) staff       (20)       38 2023-05-05 03:42:19.133893 consolecmdtools-3.5.1/setup.cfg
-drwxr-xr-x   0 kyan001    (501) staff       (20)        0 2023-05-05 03:42:19.131688 consolecmdtools-3.5.1/tests/
--rw-r--r--   0 kyan001    (501) staff       (20)    12262 2023-05-05 03:39:04.000000 consolecmdtools-3.5.1/tests/test_consolecmdtools.py
--rw-r--r--   0 kyan001    (501) staff       (20)      363 2021-03-01 08:05:34.000000 consolecmdtools-3.5.1/tests/test_runas.py
+drwxr-xr-x   0 kyan001    (501) staff       (20)        0 2023-05-05 04:11:02.294607 consolecmdtools-3.5.2/
+-rw-r--r--   0 kyan001    (501) staff       (20)     1061 2020-11-09 08:36:27.000000 consolecmdtools-3.5.2/LICENSE
+-rw-r--r--   0 kyan001    (501) staff       (20)     7368 2023-05-05 04:11:02.293642 consolecmdtools-3.5.2/PKG-INFO
+-rw-r--r--   0 kyan001    (501) staff       (20)     5293 2023-05-05 03:39:04.000000 consolecmdtools-3.5.2/README.md
+drwxr-xr-x   0 kyan001    (501) staff       (20)        0 2023-05-05 04:11:02.285771 consolecmdtools-3.5.2/consolecmdtools/
+-rw-r--r--   0 kyan001    (501) staff       (20)    15641 2023-05-05 04:07:35.000000 consolecmdtools-3.5.2/consolecmdtools/__init__.py
+-rw-r--r--   0 kyan001    (501) staff       (20)     2037 2022-12-25 10:04:52.000000 consolecmdtools-3.5.2/consolecmdtools/__main__.py
+drwxr-xr-x   0 kyan001    (501) staff       (20)        0 2023-05-05 04:11:02.289895 consolecmdtools-3.5.2/consolecmdtools.egg-info/
+-rw-r--r--   0 kyan001    (501) staff       (20)     7368 2023-05-05 04:11:02.000000 consolecmdtools-3.5.2/consolecmdtools.egg-info/PKG-INFO
+-rw-r--r--   0 kyan001    (501) staff       (20)      332 2023-05-05 04:11:02.000000 consolecmdtools-3.5.2/consolecmdtools.egg-info/SOURCES.txt
+-rw-r--r--   0 kyan001    (501) staff       (20)        1 2023-05-05 04:11:02.000000 consolecmdtools-3.5.2/consolecmdtools.egg-info/dependency_links.txt
+-rw-r--r--   0 kyan001    (501) staff       (20)       60 2023-05-05 04:11:02.000000 consolecmdtools-3.5.2/consolecmdtools.egg-info/requires.txt
+-rw-r--r--   0 kyan001    (501) staff       (20)       21 2023-05-05 04:11:02.000000 consolecmdtools-3.5.2/consolecmdtools.egg-info/top_level.txt
+-rw-r--r--   0 kyan001    (501) staff       (20)     1230 2022-12-25 10:04:52.000000 consolecmdtools-3.5.2/pyproject.toml
+-rw-r--r--   0 kyan001    (501) staff       (20)       38 2023-05-05 04:11:02.294797 consolecmdtools-3.5.2/setup.cfg
+drwxr-xr-x   0 kyan001    (501) staff       (20)        0 2023-05-05 04:11:02.291796 consolecmdtools-3.5.2/tests/
+-rw-r--r--   0 kyan001    (501) staff       (20)    12262 2023-05-05 03:39:04.000000 consolecmdtools-3.5.2/tests/test_consolecmdtools.py
+-rw-r--r--   0 kyan001    (501) staff       (20)      363 2021-03-01 08:05:34.000000 consolecmdtools-3.5.2/tests/test_runas.py
```

### Comparing `consolecmdtools-3.5.1/LICENSE` & `consolecmdtools-3.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `consolecmdtools-3.5.1/PKG-INFO` & `consolecmdtools-3.5.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: consolecmdtools
-Version: 3.5.1
+Version: 3.5.2
 Summary: Console command tools in Python
 Author-email: Kyan <kai@kyan001.com>
 License: MIT License
         
         Copyright (c) 2020 Kyan
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `consolecmdtools-3.5.1/README.md` & `consolecmdtools-3.5.2/README.md`

 * *Files identical despite different names*

### Comparing `consolecmdtools-3.5.1/consolecmdtools/__init__.py` & `consolecmdtools-3.5.2/consolecmdtools/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 import urllib.request
 import json
 import io
 # !! some imports are lazy-loaded
 
 import consoleiotools as cit
 
-__version__ = '3.5.1'
+__version__ = '3.5.2'
 
 
 def banner(text: str) -> str:
     """Generate a banner of 3 lines"""
     FILLER = "#"
     text = text.strip()
     middle_line = FILLER + text.center(int(len(text) / 0.618)) + FILLER
@@ -359,28 +359,32 @@
     """
     import time
     import shutil
 
     def _msg(message):
         if msgout:
             msgout(message)
-    _msg(f"From{' (+Copy)' if copy else ''}: {src}")
-    _msg(f"To{' (+Backup)' if backup else ''}: {dst}")
+    _msg(f"Source File: {src}")
+    _msg(f"Destination File: {dst}")
+    if copy:
+        _msg("Copy Enabled.")
+    if backup:
+        _msg("Backup Enabled.")
     if not os.path.exists(src):
-        raise FileNotFoundError(f"Source file {src} does not exist.")
+        raise FileNotFoundError(f"Source file does not exist.")
     if os.path.exists(dst):
         if backup:
-            dst_backup = f"{dst}.backup.{time.strftime('%Y%m%d%H%M%S')}"
+            dst_backup = f"{ dst}.backup.{time.strftime('%Y%m%d%H%M%S')}"
             shutil.copy2(dst, dst_backup)
-            _msg(f"Destination file {dst} backuped up to {dst_backup}.")
+            _msg(f"Destination file backuped up to `{dst_backup}`.")
         else:
-            _msg(f"Warning: Destination file {dst} already exists and will be overwritten.")
+            _msg("Warning: Destination file already exists and will be overwritten.")
     else:
         if backup:
-            _msg(f"Warning: Destination file {dst} does not exist, backup skipped.")
+            _msg("Warning: Destination file does not exist, backup skipped.")
     if copy:
         shutil.copy2(src, dst)
     else:
         shutil.move(src, dst)
     _msg(f"File {src} {'copied' if copy else 'moved'} to {dst}.")
```

### Comparing `consolecmdtools-3.5.1/consolecmdtools/__main__.py` & `consolecmdtools-3.5.2/consolecmdtools/__main__.py`

 * *Files identical despite different names*

### Comparing `consolecmdtools-3.5.1/consolecmdtools.egg-info/PKG-INFO` & `consolecmdtools-3.5.2/consolecmdtools.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: consolecmdtools
-Version: 3.5.1
+Version: 3.5.2
 Summary: Console command tools in Python
 Author-email: Kyan <kai@kyan001.com>
 License: MIT License
         
         Copyright (c) 2020 Kyan
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `consolecmdtools-3.5.1/pyproject.toml` & `consolecmdtools-3.5.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `consolecmdtools-3.5.1/tests/test_consolecmdtools.py` & `consolecmdtools-3.5.2/tests/test_consolecmdtools.py`

 * *Files identical despite different names*

