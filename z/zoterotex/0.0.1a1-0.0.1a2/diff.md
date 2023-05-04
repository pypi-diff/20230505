# Comparing `tmp/zoterotex-0.0.1a1.tar.gz` & `tmp/zoterotex-0.0.1a2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zoterotex-0.0.1a1.tar", last modified: Thu May  4 21:56:50 2023, max compression
+gzip compressed data, was "zoterotex-0.0.1a2.tar", last modified: Thu May  4 22:16:40 2023, max compression
```

## Comparing `zoterotex-0.0.1a1.tar` & `zoterotex-0.0.1a2.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 galer    (1959091754) 1971611142        0 2023-05-04 21:56:50.367889 zoterotex-0.0.1a1/
--rw-r--r--   0 galer    (1959091754) 1971611142      193 2023-05-04 21:56:50.367630 zoterotex-0.0.1a1/PKG-INFO
--rw-r--r--   0 galer    (1959091754) 1971611142      408 2023-05-04 21:54:16.000000 zoterotex-0.0.1a1/pyproject.toml
--rw-r--r--   0 galer    (1959091754) 1971611142       38 2023-05-04 21:56:50.367948 zoterotex-0.0.1a1/setup.cfg
-drwxr-xr-x   0 galer    (1959091754) 1971611142        0 2023-05-04 21:56:50.365149 zoterotex-0.0.1a1/zoterotex/
--rw-r--r--   0 galer    (1959091754) 1971611142        0 2023-05-04 21:34:59.000000 zoterotex-0.0.1a1/zoterotex/__init__.py
--rw-r--r--   0 galer    (1959091754) 1971611142     1395 2023-05-04 21:52:20.000000 zoterotex-0.0.1a1/zoterotex/__main__.py
-drwxr-xr-x   0 galer    (1959091754) 1971611142        0 2023-05-04 21:56:50.367326 zoterotex-0.0.1a1/zoterotex.egg-info/
--rw-r--r--   0 galer    (1959091754) 1971611142      193 2023-05-04 21:56:50.000000 zoterotex-0.0.1a1/zoterotex.egg-info/PKG-INFO
--rw-r--r--   0 galer    (1959091754) 1971611142      258 2023-05-04 21:56:50.000000 zoterotex-0.0.1a1/zoterotex.egg-info/SOURCES.txt
--rw-r--r--   0 galer    (1959091754) 1971611142        1 2023-05-04 21:56:50.000000 zoterotex-0.0.1a1/zoterotex.egg-info/dependency_links.txt
--rw-r--r--   0 galer    (1959091754) 1971611142       54 2023-05-04 21:56:50.000000 zoterotex-0.0.1a1/zoterotex.egg-info/entry_points.txt
--rw-r--r--   0 galer    (1959091754) 1971611142       32 2023-05-04 21:56:50.000000 zoterotex-0.0.1a1/zoterotex.egg-info/requires.txt
--rw-r--r--   0 galer    (1959091754) 1971611142       10 2023-05-04 21:56:50.000000 zoterotex-0.0.1a1/zoterotex.egg-info/top_level.txt
+drwxr-xr-x   0 galer    (1959091754) 1971611142        0 2023-05-04 22:16:40.046612 zoterotex-0.0.1a2/
+-rw-r--r--   0 galer    (1959091754) 1971611142      193 2023-05-04 22:16:40.046431 zoterotex-0.0.1a2/PKG-INFO
+-rw-r--r--   0 galer    (1959091754) 1971611142      408 2023-05-04 21:59:58.000000 zoterotex-0.0.1a2/pyproject.toml
+-rw-r--r--   0 galer    (1959091754) 1971611142       38 2023-05-04 22:16:40.046662 zoterotex-0.0.1a2/setup.cfg
+drwxr-xr-x   0 galer    (1959091754) 1971611142        0 2023-05-04 22:16:40.044026 zoterotex-0.0.1a2/zoterotex/
+-rw-r--r--   0 galer    (1959091754) 1971611142        0 2023-05-04 21:34:59.000000 zoterotex-0.0.1a2/zoterotex/__init__.py
+-rw-r--r--   0 galer    (1959091754) 1971611142     1452 2023-05-04 22:15:58.000000 zoterotex-0.0.1a2/zoterotex/__main__.py
+drwxr-xr-x   0 galer    (1959091754) 1971611142        0 2023-05-04 22:16:40.046173 zoterotex-0.0.1a2/zoterotex.egg-info/
+-rw-r--r--   0 galer    (1959091754) 1971611142      193 2023-05-04 22:16:40.000000 zoterotex-0.0.1a2/zoterotex.egg-info/PKG-INFO
+-rw-r--r--   0 galer    (1959091754) 1971611142      258 2023-05-04 22:16:40.000000 zoterotex-0.0.1a2/zoterotex.egg-info/SOURCES.txt
+-rw-r--r--   0 galer    (1959091754) 1971611142        1 2023-05-04 22:16:40.000000 zoterotex-0.0.1a2/zoterotex.egg-info/dependency_links.txt
+-rw-r--r--   0 galer    (1959091754) 1971611142       54 2023-05-04 22:16:40.000000 zoterotex-0.0.1a2/zoterotex.egg-info/entry_points.txt
+-rw-r--r--   0 galer    (1959091754) 1971611142       32 2023-05-04 22:16:40.000000 zoterotex-0.0.1a2/zoterotex.egg-info/requires.txt
+-rw-r--r--   0 galer    (1959091754) 1971611142       10 2023-05-04 22:16:40.000000 zoterotex-0.0.1a2/zoterotex.egg-info/top_level.txt
```

### Comparing `zoterotex-0.0.1a1/zoterotex/__main__.py` & `zoterotex-0.0.1a2/zoterotex/__main__.py`

 * *Files 20% similar despite different names*

```diff
@@ -14,33 +14,31 @@
 
 def get_args():
     parser = argparse.ArgumentParser()
     parser.add_argument("action", choices=("sync",))
     parser.add_argument("library_type", choices=("library", "group"))
     parser.add_argument("library_id")
     parser.add_argument("out_file")
-    parser.add_argument("--api-key-file", default="key.txt")
+    parser.add_argument("--api-key",
+                        required=True,
+                        default=os.environ.get("ZOTERO_API_KEY", None),
+                        help="Provide Zotero API key with --api-key or environment variable $ZOTERO_API_KEY",
+    )
     parser.add_argument("--log-level", choices=("DEBUG", "INFO", "WARNING", "ERROR", "CRITICAL"), default="INFO")
     return parser.parse_args()
 
 
-def sync(action, library_id, out_file, library_type, api_key_file, log_level):
+def sync(action, library_id, out_file, library_type, api_key, log_level):
     logging.basicConfig(level=log_level)
-    api_key = load_api_key(api_key_file)
     logging.info(f"Retrieving library...")
     library = Zotero(library_id, library_type, api_key)
     write_bibtex(library, out_file)
     logging.info(f"Wrote file to {out_file}")
 
 
-def load_api_key(api_key_file):
-    with open(api_key_file) as f:
-        return f.read().strip()
-
-
 def write_bibtex(library, out_file):
     bibtex_database = library.items(format="bibtex")
     if "/" in out_file:
         os.makedirs(os.path.dirname(out_file), exist_ok=True)
 
     with open(out_file, "w") as f:
         bibtexparser.dump(bibtex_database, f)
```

