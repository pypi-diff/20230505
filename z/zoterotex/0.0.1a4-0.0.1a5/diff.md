# Comparing `tmp/zoterotex-0.0.1a4.tar.gz` & `tmp/zoterotex-0.0.1a5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zoterotex-0.0.1a4.tar", last modified: Thu May  4 23:57:16 2023, max compression
+gzip compressed data, was "zoterotex-0.0.1a5.tar", last modified: Fri May  5 00:09:40 2023, max compression
```

## Comparing `zoterotex-0.0.1a4.tar` & `zoterotex-0.0.1a5.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 galer    (1959091754) 1971611142        0 2023-05-04 23:57:16.283435 zoterotex-0.0.1a4/
--rw-r--r--   0 galer    (1959091754) 1971611142      193 2023-05-04 23:57:16.283094 zoterotex-0.0.1a4/PKG-INFO
--rw-r--r--   0 galer    (1959091754) 1971611142      408 2023-05-04 23:56:49.000000 zoterotex-0.0.1a4/pyproject.toml
--rw-r--r--   0 galer    (1959091754) 1971611142       38 2023-05-04 23:57:16.283491 zoterotex-0.0.1a4/setup.cfg
-drwxr-xr-x   0 galer    (1959091754) 1971611142        0 2023-05-04 23:57:16.280790 zoterotex-0.0.1a4/zoterotex/
--rw-r--r--   0 galer    (1959091754) 1971611142        0 2023-05-04 21:34:59.000000 zoterotex-0.0.1a4/zoterotex/__init__.py
--rw-r--r--   0 galer    (1959091754) 1971611142     2054 2023-05-04 23:56:31.000000 zoterotex-0.0.1a4/zoterotex/__main__.py
-drwxr-xr-x   0 galer    (1959091754) 1971611142        0 2023-05-04 23:57:16.282680 zoterotex-0.0.1a4/zoterotex.egg-info/
--rw-r--r--   0 galer    (1959091754) 1971611142      193 2023-05-04 23:57:16.000000 zoterotex-0.0.1a4/zoterotex.egg-info/PKG-INFO
--rw-r--r--   0 galer    (1959091754) 1971611142      258 2023-05-04 23:57:16.000000 zoterotex-0.0.1a4/zoterotex.egg-info/SOURCES.txt
--rw-r--r--   0 galer    (1959091754) 1971611142        1 2023-05-04 23:57:16.000000 zoterotex-0.0.1a4/zoterotex.egg-info/dependency_links.txt
--rw-r--r--   0 galer    (1959091754) 1971611142       54 2023-05-04 23:57:16.000000 zoterotex-0.0.1a4/zoterotex.egg-info/entry_points.txt
--rw-r--r--   0 galer    (1959091754) 1971611142       32 2023-05-04 23:57:16.000000 zoterotex-0.0.1a4/zoterotex.egg-info/requires.txt
--rw-r--r--   0 galer    (1959091754) 1971611142       10 2023-05-04 23:57:16.000000 zoterotex-0.0.1a4/zoterotex.egg-info/top_level.txt
+drwxr-xr-x   0 galer    (1959091754) 1971611142        0 2023-05-05 00:09:40.285493 zoterotex-0.0.1a5/
+-rw-r--r--   0 galer    (1959091754) 1971611142      193 2023-05-05 00:09:40.285267 zoterotex-0.0.1a5/PKG-INFO
+-rw-r--r--   0 galer    (1959091754) 1971611142      408 2023-05-05 00:09:32.000000 zoterotex-0.0.1a5/pyproject.toml
+-rw-r--r--   0 galer    (1959091754) 1971611142       38 2023-05-05 00:09:40.285540 zoterotex-0.0.1a5/setup.cfg
+drwxr-xr-x   0 galer    (1959091754) 1971611142        0 2023-05-05 00:09:40.282780 zoterotex-0.0.1a5/zoterotex/
+-rw-r--r--   0 galer    (1959091754) 1971611142        0 2023-05-04 21:34:59.000000 zoterotex-0.0.1a5/zoterotex/__init__.py
+-rw-r--r--   0 galer    (1959091754) 1971611142     2190 2023-05-05 00:09:04.000000 zoterotex-0.0.1a5/zoterotex/__main__.py
+drwxr-xr-x   0 galer    (1959091754) 1971611142        0 2023-05-05 00:09:40.284956 zoterotex-0.0.1a5/zoterotex.egg-info/
+-rw-r--r--   0 galer    (1959091754) 1971611142      193 2023-05-05 00:09:40.000000 zoterotex-0.0.1a5/zoterotex.egg-info/PKG-INFO
+-rw-r--r--   0 galer    (1959091754) 1971611142      258 2023-05-05 00:09:40.000000 zoterotex-0.0.1a5/zoterotex.egg-info/SOURCES.txt
+-rw-r--r--   0 galer    (1959091754) 1971611142        1 2023-05-05 00:09:40.000000 zoterotex-0.0.1a5/zoterotex.egg-info/dependency_links.txt
+-rw-r--r--   0 galer    (1959091754) 1971611142       54 2023-05-05 00:09:40.000000 zoterotex-0.0.1a5/zoterotex.egg-info/entry_points.txt
+-rw-r--r--   0 galer    (1959091754) 1971611142       32 2023-05-05 00:09:40.000000 zoterotex-0.0.1a5/zoterotex.egg-info/requires.txt
+-rw-r--r--   0 galer    (1959091754) 1971611142       10 2023-05-05 00:09:40.000000 zoterotex-0.0.1a5/zoterotex.egg-info/top_level.txt
```

### Comparing `zoterotex-0.0.1a4/zoterotex/__main__.py` & `zoterotex-0.0.1a5/zoterotex/__main__.py`

 * *Files 6% similar despite different names*

```diff
@@ -30,38 +30,39 @@
     logging.info(f"Retrieving library...")
     library = Zotero(library_id, library_type, api_key)
     write_bibtex(library, out_file)
 
 
 def write_bibtex(library, out_file):
     params = {}
-    version = get_file_version(out_file)
+    version = get_file_version(out_file, library.library_id)
     if version:
         params["since"] = version
 
     bibtex_database = library.items(format="bibtex", **params)
     if not bibtex_database:
         logging.info(f"No updates since version {version}. Quitting.")
         return
 
     if "/" in out_file:
         os.makedirs(os.path.dirname(out_file), exist_ok=True)
 
     with open(out_file, "w") as f:
-        print(f"% Version={library.last_modified_version()}", file=f)
+        print(f"% Library: {library.library_id}, Version: {library.last_modified_version()}", file=f)
         print(f"% This file was automatically generated. Do not update manually!", file=f)
         print(f"", file=f)
         bibtexparser.dump(bibtex_database, f)
         logging.info(f"Wrote BibTeX library to {out_file}")
 
 
-def get_file_version(filename):
+def get_file_version(filename, library_id):
     if os.path.exists(filename):
         with open(filename) as f:
-            match = re.search(r"% Version=(\d+)", f.readline())
-            if match:
-                return int(match[1])
+            header = f.readline()
+            match = re.search(r"% Library: (.*?), Version: (\d+)", header)
+            if match and match[1] == str(library_id):
+                return match[2]
     return None
 
 
 if __name__ == '__main__':
     main()
```

