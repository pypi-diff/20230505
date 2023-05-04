# Comparing `tmp/zoterotex-0.0.1a3.tar.gz` & `tmp/zoterotex-0.0.1a4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zoterotex-0.0.1a3.tar", last modified: Thu May  4 22:31:20 2023, max compression
+gzip compressed data, was "zoterotex-0.0.1a4.tar", last modified: Thu May  4 23:57:16 2023, max compression
```

## Comparing `zoterotex-0.0.1a3.tar` & `zoterotex-0.0.1a4.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 galer    (1959091754) 1971611142        0 2023-05-04 22:31:20.313312 zoterotex-0.0.1a3/
--rw-r--r--   0 galer    (1959091754) 1971611142      193 2023-05-04 22:31:20.313102 zoterotex-0.0.1a3/PKG-INFO
--rw-r--r--   0 galer    (1959091754) 1971611142      408 2023-05-04 22:30:36.000000 zoterotex-0.0.1a3/pyproject.toml
--rw-r--r--   0 galer    (1959091754) 1971611142       38 2023-05-04 22:31:20.313367 zoterotex-0.0.1a3/setup.cfg
-drwxr-xr-x   0 galer    (1959091754) 1971611142        0 2023-05-04 22:31:20.311082 zoterotex-0.0.1a3/zoterotex/
--rw-r--r--   0 galer    (1959091754) 1971611142        0 2023-05-04 21:34:59.000000 zoterotex-0.0.1a3/zoterotex/__init__.py
--rw-r--r--   0 galer    (1959091754) 1971611142     1414 2023-05-04 22:29:25.000000 zoterotex-0.0.1a3/zoterotex/__main__.py
-drwxr-xr-x   0 galer    (1959091754) 1971611142        0 2023-05-04 22:31:20.312818 zoterotex-0.0.1a3/zoterotex.egg-info/
--rw-r--r--   0 galer    (1959091754) 1971611142      193 2023-05-04 22:31:20.000000 zoterotex-0.0.1a3/zoterotex.egg-info/PKG-INFO
--rw-r--r--   0 galer    (1959091754) 1971611142      258 2023-05-04 22:31:20.000000 zoterotex-0.0.1a3/zoterotex.egg-info/SOURCES.txt
--rw-r--r--   0 galer    (1959091754) 1971611142        1 2023-05-04 22:31:20.000000 zoterotex-0.0.1a3/zoterotex.egg-info/dependency_links.txt
--rw-r--r--   0 galer    (1959091754) 1971611142       54 2023-05-04 22:31:20.000000 zoterotex-0.0.1a3/zoterotex.egg-info/entry_points.txt
--rw-r--r--   0 galer    (1959091754) 1971611142       32 2023-05-04 22:31:20.000000 zoterotex-0.0.1a3/zoterotex.egg-info/requires.txt
--rw-r--r--   0 galer    (1959091754) 1971611142       10 2023-05-04 22:31:20.000000 zoterotex-0.0.1a3/zoterotex.egg-info/top_level.txt
+drwxr-xr-x   0 galer    (1959091754) 1971611142        0 2023-05-04 23:57:16.283435 zoterotex-0.0.1a4/
+-rw-r--r--   0 galer    (1959091754) 1971611142      193 2023-05-04 23:57:16.283094 zoterotex-0.0.1a4/PKG-INFO
+-rw-r--r--   0 galer    (1959091754) 1971611142      408 2023-05-04 23:56:49.000000 zoterotex-0.0.1a4/pyproject.toml
+-rw-r--r--   0 galer    (1959091754) 1971611142       38 2023-05-04 23:57:16.283491 zoterotex-0.0.1a4/setup.cfg
+drwxr-xr-x   0 galer    (1959091754) 1971611142        0 2023-05-04 23:57:16.280790 zoterotex-0.0.1a4/zoterotex/
+-rw-r--r--   0 galer    (1959091754) 1971611142        0 2023-05-04 21:34:59.000000 zoterotex-0.0.1a4/zoterotex/__init__.py
+-rw-r--r--   0 galer    (1959091754) 1971611142     2054 2023-05-04 23:56:31.000000 zoterotex-0.0.1a4/zoterotex/__main__.py
+drwxr-xr-x   0 galer    (1959091754) 1971611142        0 2023-05-04 23:57:16.282680 zoterotex-0.0.1a4/zoterotex.egg-info/
+-rw-r--r--   0 galer    (1959091754) 1971611142      193 2023-05-04 23:57:16.000000 zoterotex-0.0.1a4/zoterotex.egg-info/PKG-INFO
+-rw-r--r--   0 galer    (1959091754) 1971611142      258 2023-05-04 23:57:16.000000 zoterotex-0.0.1a4/zoterotex.egg-info/SOURCES.txt
+-rw-r--r--   0 galer    (1959091754) 1971611142        1 2023-05-04 23:57:16.000000 zoterotex-0.0.1a4/zoterotex.egg-info/dependency_links.txt
+-rw-r--r--   0 galer    (1959091754) 1971611142       54 2023-05-04 23:57:16.000000 zoterotex-0.0.1a4/zoterotex.egg-info/entry_points.txt
+-rw-r--r--   0 galer    (1959091754) 1971611142       32 2023-05-04 23:57:16.000000 zoterotex-0.0.1a4/zoterotex.egg-info/requires.txt
+-rw-r--r--   0 galer    (1959091754) 1971611142       10 2023-05-04 23:57:16.000000 zoterotex-0.0.1a4/zoterotex.egg-info/top_level.txt
```

### Comparing `zoterotex-0.0.1a3/zoterotex/__main__.py` & `zoterotex-0.0.1a4/zoterotex/__main__.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,11 +1,11 @@
-# This is a sample Python script.
 import argparse
 import logging
 import os
+import re
 
 import bibtexparser
 from pyzotero.zotero import Zotero
 
 
 def main():
     args = get_args()
@@ -26,22 +26,42 @@
 def sync(action, library_id, out_file, library_type, api_key, log_level):
     logging.basicConfig(level=log_level)
     if not api_key:
         raise ValueError("Must provide Zotero API key with --api-key or environment variable $ZOTERO_API_KEY")
     logging.info(f"Retrieving library...")
     library = Zotero(library_id, library_type, api_key)
     write_bibtex(library, out_file)
-    logging.info(f"Wrote BibTeX library to {out_file}")
 
 
 def write_bibtex(library, out_file):
-    bibtex_database = library.items(format="bibtex")
+    params = {}
+    version = get_file_version(out_file)
+    if version:
+        params["since"] = version
+
+    bibtex_database = library.items(format="bibtex", **params)
+    if not bibtex_database:
+        logging.info(f"No updates since version {version}. Quitting.")
+        return
+
     if "/" in out_file:
         os.makedirs(os.path.dirname(out_file), exist_ok=True)
 
     with open(out_file, "w") as f:
+        print(f"% Version={library.last_modified_version()}", file=f)
+        print(f"% This file was automatically generated. Do not update manually!", file=f)
+        print(f"", file=f)
         bibtexparser.dump(bibtex_database, f)
+        logging.info(f"Wrote BibTeX library to {out_file}")
+
 
+def get_file_version(filename):
+    if os.path.exists(filename):
+        with open(filename) as f:
+            match = re.search(r"% Version=(\d+)", f.readline())
+            if match:
+                return int(match[1])
+    return None
 
 
 if __name__ == '__main__':
     main()
```

