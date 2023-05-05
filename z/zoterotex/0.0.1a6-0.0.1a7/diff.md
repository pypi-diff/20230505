# Comparing `tmp/zoterotex-0.0.1a6.tar.gz` & `tmp/zoterotex-0.0.1a7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zoterotex-0.0.1a6.tar", last modified: Fri May  5 00:16:16 2023, max compression
+gzip compressed data, was "zoterotex-0.0.1a7.tar", last modified: Fri May  5 00:29:54 2023, max compression
```

## Comparing `zoterotex-0.0.1a6.tar` & `zoterotex-0.0.1a7.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 galer    (1959091754) 1971611142        0 2023-05-05 00:16:16.499682 zoterotex-0.0.1a6/
--rw-r--r--   0 galer    (1959091754) 1971611142      193 2023-05-05 00:16:16.499450 zoterotex-0.0.1a6/PKG-INFO
--rw-r--r--   0 galer    (1959091754) 1971611142      408 2023-05-05 00:15:55.000000 zoterotex-0.0.1a6/pyproject.toml
--rw-r--r--   0 galer    (1959091754) 1971611142       38 2023-05-05 00:16:16.499730 zoterotex-0.0.1a6/setup.cfg
-drwxr-xr-x   0 galer    (1959091754) 1971611142        0 2023-05-05 00:16:16.497160 zoterotex-0.0.1a6/zoterotex/
--rw-r--r--   0 galer    (1959091754) 1971611142        0 2023-05-04 21:34:59.000000 zoterotex-0.0.1a6/zoterotex/__init__.py
--rw-r--r--   0 galer    (1959091754) 1971611142     2190 2023-05-05 00:09:04.000000 zoterotex-0.0.1a6/zoterotex/__main__.py
-drwxr-xr-x   0 galer    (1959091754) 1971611142        0 2023-05-05 00:16:16.499158 zoterotex-0.0.1a6/zoterotex.egg-info/
--rw-r--r--   0 galer    (1959091754) 1971611142      193 2023-05-05 00:16:16.000000 zoterotex-0.0.1a6/zoterotex.egg-info/PKG-INFO
--rw-r--r--   0 galer    (1959091754) 1971611142      258 2023-05-05 00:16:16.000000 zoterotex-0.0.1a6/zoterotex.egg-info/SOURCES.txt
--rw-r--r--   0 galer    (1959091754) 1971611142        1 2023-05-05 00:16:16.000000 zoterotex-0.0.1a6/zoterotex.egg-info/dependency_links.txt
--rw-r--r--   0 galer    (1959091754) 1971611142       54 2023-05-05 00:16:16.000000 zoterotex-0.0.1a6/zoterotex.egg-info/entry_points.txt
--rw-r--r--   0 galer    (1959091754) 1971611142       32 2023-05-05 00:16:16.000000 zoterotex-0.0.1a6/zoterotex.egg-info/requires.txt
--rw-r--r--   0 galer    (1959091754) 1971611142       10 2023-05-05 00:16:16.000000 zoterotex-0.0.1a6/zoterotex.egg-info/top_level.txt
+drwxr-xr-x   0 galer    (1959091754) 1971611142        0 2023-05-05 00:29:54.967843 zoterotex-0.0.1a7/
+-rw-r--r--   0 galer    (1959091754) 1971611142      193 2023-05-05 00:29:54.967598 zoterotex-0.0.1a7/PKG-INFO
+-rw-r--r--   0 galer    (1959091754) 1971611142      408 2023-05-05 00:18:06.000000 zoterotex-0.0.1a7/pyproject.toml
+-rw-r--r--   0 galer    (1959091754) 1971611142       38 2023-05-05 00:29:54.967888 zoterotex-0.0.1a7/setup.cfg
+drwxr-xr-x   0 galer    (1959091754) 1971611142        0 2023-05-05 00:29:54.964851 zoterotex-0.0.1a7/zoterotex/
+-rw-r--r--   0 galer    (1959091754) 1971611142        0 2023-05-04 21:34:59.000000 zoterotex-0.0.1a7/zoterotex/__init__.py
+-rw-r--r--   0 galer    (1959091754) 1971611142     2154 2023-05-05 00:29:26.000000 zoterotex-0.0.1a7/zoterotex/__main__.py
+drwxr-xr-x   0 galer    (1959091754) 1971611142        0 2023-05-05 00:29:54.967286 zoterotex-0.0.1a7/zoterotex.egg-info/
+-rw-r--r--   0 galer    (1959091754) 1971611142      193 2023-05-05 00:29:54.000000 zoterotex-0.0.1a7/zoterotex.egg-info/PKG-INFO
+-rw-r--r--   0 galer    (1959091754) 1971611142      258 2023-05-05 00:29:54.000000 zoterotex-0.0.1a7/zoterotex.egg-info/SOURCES.txt
+-rw-r--r--   0 galer    (1959091754) 1971611142        1 2023-05-05 00:29:54.000000 zoterotex-0.0.1a7/zoterotex.egg-info/dependency_links.txt
+-rw-r--r--   0 galer    (1959091754) 1971611142       54 2023-05-05 00:29:54.000000 zoterotex-0.0.1a7/zoterotex.egg-info/entry_points.txt
+-rw-r--r--   0 galer    (1959091754) 1971611142       32 2023-05-05 00:29:54.000000 zoterotex-0.0.1a7/zoterotex.egg-info/requires.txt
+-rw-r--r--   0 galer    (1959091754) 1971611142       10 2023-05-05 00:29:54.000000 zoterotex-0.0.1a7/zoterotex.egg-info/top_level.txt
```

### Comparing `zoterotex-0.0.1a6/zoterotex/__main__.py` & `zoterotex-0.0.1a7/zoterotex/__main__.py`

 * *Files 4% similar despite different names*

```diff
@@ -29,24 +29,21 @@
         raise ValueError("Must provide Zotero API key with --api-key or environment variable $ZOTERO_API_KEY")
     logging.info(f"Retrieving library...")
     library = Zotero(library_id, library_type, api_key)
     write_bibtex(library, out_file)
 
 
 def write_bibtex(library, out_file):
-    params = {}
     version = get_file_version(out_file, library.library_id)
-    if version:
-        params["since"] = version
-
-    bibtex_database = library.items(format="bibtex", **params)
-    if not bibtex_database:
+    if version and version == library.last_modified_version():
         logging.info(f"No updates since version {version}. Quitting.")
         return
 
+    bibtex_database = library.items(format="bibtex")
+
     if "/" in out_file:
         os.makedirs(os.path.dirname(out_file), exist_ok=True)
 
     with open(out_file, "w") as f:
         print(f"% Library: {library.library_id}, Version: {library.last_modified_version()}", file=f)
         print(f"% This file was automatically generated. Do not update manually!", file=f)
         print(f"", file=f)
@@ -56,13 +53,13 @@
 
 def get_file_version(filename, library_id):
     if os.path.exists(filename):
         with open(filename) as f:
             header = f.readline()
             match = re.search(r"% Library: (.*?), Version: (\d+)", header)
             if match and match[1] == str(library_id):
-                return match[2]
+                return int(match[2])
     return None
 
 
 if __name__ == '__main__':
     main()
```

