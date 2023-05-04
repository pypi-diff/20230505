# Comparing `tmp/zoterotex-0.0.1a2.tar.gz` & `tmp/zoterotex-0.0.1a3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zoterotex-0.0.1a2.tar", last modified: Thu May  4 22:16:40 2023, max compression
+gzip compressed data, was "zoterotex-0.0.1a3.tar", last modified: Thu May  4 22:31:20 2023, max compression
```

## Comparing `zoterotex-0.0.1a2.tar` & `zoterotex-0.0.1a3.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 galer    (1959091754) 1971611142        0 2023-05-04 22:16:40.046612 zoterotex-0.0.1a2/
--rw-r--r--   0 galer    (1959091754) 1971611142      193 2023-05-04 22:16:40.046431 zoterotex-0.0.1a2/PKG-INFO
--rw-r--r--   0 galer    (1959091754) 1971611142      408 2023-05-04 21:59:58.000000 zoterotex-0.0.1a2/pyproject.toml
--rw-r--r--   0 galer    (1959091754) 1971611142       38 2023-05-04 22:16:40.046662 zoterotex-0.0.1a2/setup.cfg
-drwxr-xr-x   0 galer    (1959091754) 1971611142        0 2023-05-04 22:16:40.044026 zoterotex-0.0.1a2/zoterotex/
--rw-r--r--   0 galer    (1959091754) 1971611142        0 2023-05-04 21:34:59.000000 zoterotex-0.0.1a2/zoterotex/__init__.py
--rw-r--r--   0 galer    (1959091754) 1971611142     1452 2023-05-04 22:15:58.000000 zoterotex-0.0.1a2/zoterotex/__main__.py
-drwxr-xr-x   0 galer    (1959091754) 1971611142        0 2023-05-04 22:16:40.046173 zoterotex-0.0.1a2/zoterotex.egg-info/
--rw-r--r--   0 galer    (1959091754) 1971611142      193 2023-05-04 22:16:40.000000 zoterotex-0.0.1a2/zoterotex.egg-info/PKG-INFO
--rw-r--r--   0 galer    (1959091754) 1971611142      258 2023-05-04 22:16:40.000000 zoterotex-0.0.1a2/zoterotex.egg-info/SOURCES.txt
--rw-r--r--   0 galer    (1959091754) 1971611142        1 2023-05-04 22:16:40.000000 zoterotex-0.0.1a2/zoterotex.egg-info/dependency_links.txt
--rw-r--r--   0 galer    (1959091754) 1971611142       54 2023-05-04 22:16:40.000000 zoterotex-0.0.1a2/zoterotex.egg-info/entry_points.txt
--rw-r--r--   0 galer    (1959091754) 1971611142       32 2023-05-04 22:16:40.000000 zoterotex-0.0.1a2/zoterotex.egg-info/requires.txt
--rw-r--r--   0 galer    (1959091754) 1971611142       10 2023-05-04 22:16:40.000000 zoterotex-0.0.1a2/zoterotex.egg-info/top_level.txt
+drwxr-xr-x   0 galer    (1959091754) 1971611142        0 2023-05-04 22:31:20.313312 zoterotex-0.0.1a3/
+-rw-r--r--   0 galer    (1959091754) 1971611142      193 2023-05-04 22:31:20.313102 zoterotex-0.0.1a3/PKG-INFO
+-rw-r--r--   0 galer    (1959091754) 1971611142      408 2023-05-04 22:30:36.000000 zoterotex-0.0.1a3/pyproject.toml
+-rw-r--r--   0 galer    (1959091754) 1971611142       38 2023-05-04 22:31:20.313367 zoterotex-0.0.1a3/setup.cfg
+drwxr-xr-x   0 galer    (1959091754) 1971611142        0 2023-05-04 22:31:20.311082 zoterotex-0.0.1a3/zoterotex/
+-rw-r--r--   0 galer    (1959091754) 1971611142        0 2023-05-04 21:34:59.000000 zoterotex-0.0.1a3/zoterotex/__init__.py
+-rw-r--r--   0 galer    (1959091754) 1971611142     1414 2023-05-04 22:29:25.000000 zoterotex-0.0.1a3/zoterotex/__main__.py
+drwxr-xr-x   0 galer    (1959091754) 1971611142        0 2023-05-04 22:31:20.312818 zoterotex-0.0.1a3/zoterotex.egg-info/
+-rw-r--r--   0 galer    (1959091754) 1971611142      193 2023-05-04 22:31:20.000000 zoterotex-0.0.1a3/zoterotex.egg-info/PKG-INFO
+-rw-r--r--   0 galer    (1959091754) 1971611142      258 2023-05-04 22:31:20.000000 zoterotex-0.0.1a3/zoterotex.egg-info/SOURCES.txt
+-rw-r--r--   0 galer    (1959091754) 1971611142        1 2023-05-04 22:31:20.000000 zoterotex-0.0.1a3/zoterotex.egg-info/dependency_links.txt
+-rw-r--r--   0 galer    (1959091754) 1971611142       54 2023-05-04 22:31:20.000000 zoterotex-0.0.1a3/zoterotex.egg-info/entry_points.txt
+-rw-r--r--   0 galer    (1959091754) 1971611142       32 2023-05-04 22:31:20.000000 zoterotex-0.0.1a3/zoterotex.egg-info/requires.txt
+-rw-r--r--   0 galer    (1959091754) 1971611142       10 2023-05-04 22:31:20.000000 zoterotex-0.0.1a3/zoterotex.egg-info/top_level.txt
```

### Comparing `zoterotex-0.0.1a2/zoterotex/__main__.py` & `zoterotex-0.0.1a3/zoterotex/__main__.py`

 * *Files 11% similar despite different names*

```diff
@@ -14,29 +14,27 @@
 
 def get_args():
     parser = argparse.ArgumentParser()
     parser.add_argument("action", choices=("sync",))
     parser.add_argument("library_type", choices=("library", "group"))
     parser.add_argument("library_id")
     parser.add_argument("out_file")
-    parser.add_argument("--api-key",
-                        required=True,
-                        default=os.environ.get("ZOTERO_API_KEY", None),
-                        help="Provide Zotero API key with --api-key or environment variable $ZOTERO_API_KEY",
-    )
+    parser.add_argument("--api-key", default=os.environ.get("ZOTERO_API_KEY", None))
     parser.add_argument("--log-level", choices=("DEBUG", "INFO", "WARNING", "ERROR", "CRITICAL"), default="INFO")
     return parser.parse_args()
 
 
 def sync(action, library_id, out_file, library_type, api_key, log_level):
     logging.basicConfig(level=log_level)
+    if not api_key:
+        raise ValueError("Must provide Zotero API key with --api-key or environment variable $ZOTERO_API_KEY")
     logging.info(f"Retrieving library...")
     library = Zotero(library_id, library_type, api_key)
     write_bibtex(library, out_file)
-    logging.info(f"Wrote file to {out_file}")
+    logging.info(f"Wrote BibTeX library to {out_file}")
 
 
 def write_bibtex(library, out_file):
     bibtex_database = library.items(format="bibtex")
     if "/" in out_file:
         os.makedirs(os.path.dirname(out_file), exist_ok=True)
```

