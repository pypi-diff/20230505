# Comparing `tmp/jiggybase-0.0.24.tar.gz` & `tmp/jiggybase-0.0.25.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jiggybase-0.0.24.tar", last modified: Fri May  5 00:50:52 2023, max compression
+gzip compressed data, was "jiggybase-0.0.25.tar", last modified: Fri May  5 02:03:04 2023, max compression
```

## Comparing `jiggybase-0.0.24.tar` & `jiggybase-0.0.25.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxr-xr-x   0 wsk        (501) staff       (20)        0 2023-05-05 00:50:52.187026 jiggybase-0.0.24/
--rw-r--r--   0 wsk        (501) staff       (20)    11357 2023-04-10 04:07:02.000000 jiggybase-0.0.24/LICENSE
--rw-r--r--   0 wsk        (501) staff       (20)     5826 2023-05-05 00:50:52.186771 jiggybase-0.0.24/PKG-INFO
--rw-r--r--   0 wsk        (501) staff       (20)     5292 2023-05-01 15:45:10.000000 jiggybase-0.0.24/README.md
-drwxr-xr-x   0 wsk        (501) staff       (20)        0 2023-05-05 00:50:52.180362 jiggybase-0.0.24/jiggybase/
--rw-r--r--   0 wsk        (501) staff       (20)       30 2023-04-28 15:28:30.000000 jiggybase-0.0.24/jiggybase/__init__.py
--rw-r--r--   0 wsk        (501) staff       (20)     2044 2023-05-01 01:40:42.000000 jiggybase-0.0.24/jiggybase/client.py
--rw-r--r--   0 wsk        (501) staff       (20)     8508 2023-04-30 00:50:55.000000 jiggybase-0.0.24/jiggybase/collection.py
-drwxr-xr-x   0 wsk        (501) staff       (20)        0 2023-05-05 00:50:52.182520 jiggybase-0.0.24/jiggybase/examples/
--rwxr-xr-x   0 wsk        (501) staff       (20)     2225 2023-05-05 00:50:28.000000 jiggybase-0.0.24/jiggybase/examples/jiggybase_upload.py
--rw-r--r--   0 wsk        (501) staff       (20)     1361 2023-05-03 07:37:11.000000 jiggybase-0.0.24/jiggybase/examples/upload_email_example.py
--rw-r--r--   0 wsk        (501) staff       (20)     4531 2023-04-29 04:12:14.000000 jiggybase-0.0.24/jiggybase/jiggybase_session.py
--rw-r--r--   0 wsk        (501) staff       (20)     1187 2023-03-30 18:09:13.000000 jiggybase-0.0.24/jiggybase/login.py
-drwxr-xr-x   0 wsk        (501) staff       (20)        0 2023-05-05 00:50:52.186206 jiggybase-0.0.24/jiggybase/models/
--rw-r--r--   0 wsk        (501) staff       (20)      273 2023-04-26 01:37:49.000000 jiggybase-0.0.24/jiggybase/models/__init__.py
--rw-r--r--   0 wsk        (501) staff       (20)     1236 2023-04-10 05:17:32.000000 jiggybase-0.0.24/jiggybase/models/auth.py
--rw-r--r--   0 wsk        (501) staff       (20)     1007 2023-04-23 16:10:39.000000 jiggybase-0.0.24/jiggybase/models/chat.py
--rw-r--r--   0 wsk        (501) staff       (20)      188 2023-04-23 04:17:06.000000 jiggybase-0.0.24/jiggybase/models/chatmodel.py
--rw-r--r--   0 wsk        (501) staff       (20)     1322 2023-04-10 16:54:34.000000 jiggybase-0.0.24/jiggybase/models/chunk.py
--rw-r--r--   0 wsk        (501) staff       (20)     4240 2023-04-20 21:45:37.000000 jiggybase-0.0.24/jiggybase/models/collection.py
--rw-r--r--   0 wsk        (501) staff       (20)      454 2023-04-23 05:06:00.000000 jiggybase-0.0.24/jiggybase/models/embedding.py
--rw-r--r--   0 wsk        (501) staff       (20)      696 2023-04-10 04:48:20.000000 jiggybase-0.0.24/jiggybase/models/metadata.py
--rw-r--r--   0 wsk        (501) staff       (20)     2214 2023-04-10 04:58:39.000000 jiggybase-0.0.24/jiggybase/models/org.py
--rw-r--r--   0 wsk        (501) staff       (20)     2777 2023-04-29 00:07:44.000000 jiggybase-0.0.24/jiggybase/models/plugin.py
--rw-r--r--   0 wsk        (501) staff       (20)     3415 2023-05-04 23:56:42.000000 jiggybase-0.0.24/jiggybase/models/plugin_config.py
--rw-r--r--   0 wsk        (501) staff       (20)     2834 2023-04-22 23:44:02.000000 jiggybase-0.0.24/jiggybase/models/prompt.py
--rw-r--r--   0 wsk        (501) staff       (20)     3012 2023-04-11 17:29:49.000000 jiggybase-0.0.24/jiggybase/models/providers.py
--rw-r--r--   0 wsk        (501) staff       (20)     1820 2023-04-17 16:14:19.000000 jiggybase-0.0.24/jiggybase/models/user.py
--rw-r--r--   0 wsk        (501) staff       (20)     4600 2023-04-29 15:22:54.000000 jiggybase-0.0.24/jiggybase/org.py
-drwxr-xr-x   0 wsk        (501) staff       (20)        0 2023-05-05 00:50:52.181979 jiggybase-0.0.24/jiggybase.egg-info/
--rw-r--r--   0 wsk        (501) staff       (20)     5826 2023-05-05 00:50:52.000000 jiggybase-0.0.24/jiggybase.egg-info/PKG-INFO
--rw-r--r--   0 wsk        (501) staff       (20)      852 2023-05-05 00:50:52.000000 jiggybase-0.0.24/jiggybase.egg-info/SOURCES.txt
--rw-r--r--   0 wsk        (501) staff       (20)        1 2023-05-05 00:50:52.000000 jiggybase-0.0.24/jiggybase.egg-info/dependency_links.txt
--rw-r--r--   0 wsk        (501) staff       (20)       78 2023-05-05 00:50:52.000000 jiggybase-0.0.24/jiggybase.egg-info/entry_points.txt
--rw-r--r--   0 wsk        (501) staff       (20)       32 2023-05-05 00:50:52.000000 jiggybase-0.0.24/jiggybase.egg-info/requires.txt
--rw-r--r--   0 wsk        (501) staff       (20)       10 2023-05-05 00:50:52.000000 jiggybase-0.0.24/jiggybase.egg-info/top_level.txt
--rw-r--r--   0 wsk        (501) staff       (20)      752 2023-05-05 00:49:54.000000 jiggybase-0.0.24/pyproject.toml
--rw-r--r--   0 wsk        (501) staff       (20)       38 2023-05-05 00:50:52.187095 jiggybase-0.0.24/setup.cfg
-drwxr-xr-x   0 wsk        (501) staff       (20)        0 2023-05-05 00:50:52.186462 jiggybase-0.0.24/test/
--rw-r--r--   0 wsk        (501) staff       (20)      830 2023-04-28 15:38:35.000000 jiggybase-0.0.24/test/test.py
+drwxr-xr-x   0 wsk        (501) staff       (20)        0 2023-05-05 02:03:04.494290 jiggybase-0.0.25/
+-rw-r--r--   0 wsk        (501) staff       (20)    11357 2023-04-10 04:07:02.000000 jiggybase-0.0.25/LICENSE
+-rw-r--r--   0 wsk        (501) staff       (20)     5826 2023-05-05 02:03:04.493904 jiggybase-0.0.25/PKG-INFO
+-rw-r--r--   0 wsk        (501) staff       (20)     5292 2023-05-01 15:45:10.000000 jiggybase-0.0.25/README.md
+drwxr-xr-x   0 wsk        (501) staff       (20)        0 2023-05-05 02:03:04.484206 jiggybase-0.0.25/jiggybase/
+-rw-r--r--   0 wsk        (501) staff       (20)       30 2023-04-28 15:28:30.000000 jiggybase-0.0.25/jiggybase/__init__.py
+-rw-r--r--   0 wsk        (501) staff       (20)     2044 2023-05-01 01:40:42.000000 jiggybase-0.0.25/jiggybase/client.py
+-rw-r--r--   0 wsk        (501) staff       (20)     8508 2023-04-30 00:50:55.000000 jiggybase-0.0.25/jiggybase/collection.py
+drwxr-xr-x   0 wsk        (501) staff       (20)        0 2023-05-05 02:03:04.487116 jiggybase-0.0.25/jiggybase/examples/
+-rwxr-xr-x   0 wsk        (501) staff       (20)     3383 2023-05-05 01:59:33.000000 jiggybase-0.0.25/jiggybase/examples/jiggybase_upload.py
+-rw-r--r--   0 wsk        (501) staff       (20)     1361 2023-05-03 07:37:11.000000 jiggybase-0.0.25/jiggybase/examples/upload_email_example.py
+-rw-r--r--   0 wsk        (501) staff       (20)     4531 2023-04-29 04:12:14.000000 jiggybase-0.0.25/jiggybase/jiggybase_session.py
+-rw-r--r--   0 wsk        (501) staff       (20)     1187 2023-03-30 18:09:13.000000 jiggybase-0.0.25/jiggybase/login.py
+drwxr-xr-x   0 wsk        (501) staff       (20)        0 2023-05-05 02:03:04.492954 jiggybase-0.0.25/jiggybase/models/
+-rw-r--r--   0 wsk        (501) staff       (20)      273 2023-04-26 01:37:49.000000 jiggybase-0.0.25/jiggybase/models/__init__.py
+-rw-r--r--   0 wsk        (501) staff       (20)     1236 2023-04-10 05:17:32.000000 jiggybase-0.0.25/jiggybase/models/auth.py
+-rw-r--r--   0 wsk        (501) staff       (20)     1007 2023-04-23 16:10:39.000000 jiggybase-0.0.25/jiggybase/models/chat.py
+-rw-r--r--   0 wsk        (501) staff       (20)      188 2023-04-23 04:17:06.000000 jiggybase-0.0.25/jiggybase/models/chatmodel.py
+-rw-r--r--   0 wsk        (501) staff       (20)     1322 2023-04-10 16:54:34.000000 jiggybase-0.0.25/jiggybase/models/chunk.py
+-rw-r--r--   0 wsk        (501) staff       (20)     4240 2023-04-20 21:45:37.000000 jiggybase-0.0.25/jiggybase/models/collection.py
+-rw-r--r--   0 wsk        (501) staff       (20)      454 2023-04-23 05:06:00.000000 jiggybase-0.0.25/jiggybase/models/embedding.py
+-rw-r--r--   0 wsk        (501) staff       (20)      696 2023-04-10 04:48:20.000000 jiggybase-0.0.25/jiggybase/models/metadata.py
+-rw-r--r--   0 wsk        (501) staff       (20)     2214 2023-04-10 04:58:39.000000 jiggybase-0.0.25/jiggybase/models/org.py
+-rw-r--r--   0 wsk        (501) staff       (20)     2777 2023-04-29 00:07:44.000000 jiggybase-0.0.25/jiggybase/models/plugin.py
+-rw-r--r--   0 wsk        (501) staff       (20)     3415 2023-05-04 23:56:42.000000 jiggybase-0.0.25/jiggybase/models/plugin_config.py
+-rw-r--r--   0 wsk        (501) staff       (20)     2834 2023-04-22 23:44:02.000000 jiggybase-0.0.25/jiggybase/models/prompt.py
+-rw-r--r--   0 wsk        (501) staff       (20)     3012 2023-04-11 17:29:49.000000 jiggybase-0.0.25/jiggybase/models/providers.py
+-rw-r--r--   0 wsk        (501) staff       (20)     1820 2023-04-17 16:14:19.000000 jiggybase-0.0.25/jiggybase/models/user.py
+-rw-r--r--   0 wsk        (501) staff       (20)     4600 2023-04-29 15:22:54.000000 jiggybase-0.0.25/jiggybase/org.py
+drwxr-xr-x   0 wsk        (501) staff       (20)        0 2023-05-05 02:03:04.486263 jiggybase-0.0.25/jiggybase.egg-info/
+-rw-r--r--   0 wsk        (501) staff       (20)     5826 2023-05-05 02:03:04.000000 jiggybase-0.0.25/jiggybase.egg-info/PKG-INFO
+-rw-r--r--   0 wsk        (501) staff       (20)      852 2023-05-05 02:03:04.000000 jiggybase-0.0.25/jiggybase.egg-info/SOURCES.txt
+-rw-r--r--   0 wsk        (501) staff       (20)        1 2023-05-05 02:03:04.000000 jiggybase-0.0.25/jiggybase.egg-info/dependency_links.txt
+-rw-r--r--   0 wsk        (501) staff       (20)       78 2023-05-05 02:03:04.000000 jiggybase-0.0.25/jiggybase.egg-info/entry_points.txt
+-rw-r--r--   0 wsk        (501) staff       (20)       32 2023-05-05 02:03:04.000000 jiggybase-0.0.25/jiggybase.egg-info/requires.txt
+-rw-r--r--   0 wsk        (501) staff       (20)       10 2023-05-05 02:03:04.000000 jiggybase-0.0.25/jiggybase.egg-info/top_level.txt
+-rw-r--r--   0 wsk        (501) staff       (20)      752 2023-05-05 01:22:51.000000 jiggybase-0.0.25/pyproject.toml
+-rw-r--r--   0 wsk        (501) staff       (20)       38 2023-05-05 02:03:04.494400 jiggybase-0.0.25/setup.cfg
+drwxr-xr-x   0 wsk        (501) staff       (20)        0 2023-05-05 02:03:04.493383 jiggybase-0.0.25/test/
+-rw-r--r--   0 wsk        (501) staff       (20)      830 2023-04-28 15:38:35.000000 jiggybase-0.0.25/test/test.py
```

### Comparing `jiggybase-0.0.24/LICENSE` & `jiggybase-0.0.25/LICENSE`

 * *Files identical despite different names*

### Comparing `jiggybase-0.0.24/PKG-INFO` & `jiggybase-0.0.25/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jiggybase
-Version: 0.0.24
+Version: 0.0.25
 Summary: Client for Jiggy AI JiggyBase, including ChatGPT Retriever Plugins
 Author-email: Bill Kish <bk@jiggy.ai>
 Project-URL: Homepage, https://github.com/jiggy-ai/jiggybase
 Project-URL: Bug Tracker, https://github.com/jiggy-ai/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

### Comparing `jiggybase-0.0.24/README.md` & `jiggybase-0.0.25/README.md`

 * *Files identical despite different names*

### Comparing `jiggybase-0.0.24/jiggybase/client.py` & `jiggybase-0.0.25/jiggybase/client.py`

 * *Files identical despite different names*

### Comparing `jiggybase-0.0.24/jiggybase/collection.py` & `jiggybase-0.0.25/jiggybase/collection.py`

 * *Files identical despite different names*

### Comparing `jiggybase-0.0.24/jiggybase/examples/jiggybase_upload.py` & `jiggybase-0.0.25/jiggybase/examples/jiggybase_upload.py`

 * *Files 23% similar despite different names*

```diff
@@ -7,41 +7,49 @@
 
 jb = jiggybase.JiggyBase()
 
 JIGGYBASE_ORG = os.environ.get("JIGGYBASE_ORG")
 JIGGYBASE_COLLECTION = os.environ.get("JIGGYBASE_COLLECTION")
 
 
+def upload_file(collection : jiggybase.models.Collection, filename : str):
+    print(f'Uploading {filename}')
+    try:
+        upsert_rsp = collection.upsert_file(filename)
+    except Exception as e:            
+        print(f'error on {filename}: {e}')
+        return
+    doc_id = upsert_rsp.ids[0]
+    dcl =  collection.get_doc(doc_id)
+    text_len = len(" ".join([dc.text for dc in dcl]))
+    title = dcl[0].metadata.title if dcl[0].metadata.title else "Unnown Title"
+    print(f'Processed {filename}: "{title}"  {text_len//1024} KB text ({len(dcl)} chunks)')
+    
+
 def upload_directory(collection : jiggybase.models.Collection, dirname : str):
     for fn in os.listdir(dirname):
         fn = os.path.join(dirname, fn)
-        print(f'uploading {fn}')
-        try:
-            upsert_rsp = collection.upsert_file(fn)
-        except Exception as e:            
-            print(f'error on {fn}: {e}')
-            continue
-        doc_id = upsert_rsp.ids[0]
-        dcl =  collection.get_doc(doc_id)
-        text_len = len(" ".join([dc.text for dc in dcl]))
-        print(f'uploaded {fn} as {doc_id}: chunk count {len(dcl)} text length {text_len} metadata {dcl[0].metadata}')
+        upload_file(collection, fn)
+
+
+epilog = "If neither '--file' nor '--dir' options are provided, the script will automatically process the last argument as a file or directory"
 
 
 def main():
-    parser = argparse.ArgumentParser(description="Upload a directory to a JiggyBase collection")
-    parser.add_argument("--org", type=str, help="The name of your JiggyBase organization")
-    parser.add_argument("--collection", type=str, help="The name of your JiggyBase collection")
-    parser.add_argument("--dir", type=str, help="The directory you want to upload")
+    parser = argparse.ArgumentParser(description="Upload a file or directory to a JiggyBase collection",  epilog=epilog )    
+    parser.add_argument("--org", type=str, help="The name of your JiggyBase organization.  Alternatively, set JIGGYBASE_ORG environment variable or be a member of a single Org.")
+    parser.add_argument("--collection", type=str, help="The name of your JiggyBase collection. Alternatively, set JIGGYBASE_COLLECTION environment variable or have a single collection in your org.")
+    parser.add_argument("--dir", type=str, help="The directory you want to upload.")
+    parser.add_argument("--file", type=str, help="The file you want to upload")
 
     if len(sys.argv) == 1:
         parser.print_help(sys.stderr)
         sys.exit(1)
 
-    parsed_args = parser.parse_args(sys.argv[1:])
-
+    parsed_args, unknown_args = parser.parse_known_args(sys.argv[1:])
     if not parsed_args.org:
         orgs = jb.orgs()
         if len(orgs) > 1:
             print("Please provide an organization name using the --org option")
             sys.exit(1)
         elif JIGGYBASE_ORG:
             org = jb.get_org(JIGGYBASE_ORG)
@@ -58,12 +66,27 @@
         elif JIGGYBASE_COLLECTION:
             collection = org.collection(JIGGYBASE_COLLECTION)
         else:
             collection = collections[0]
     else:
         collection = org.collection(parsed_args.collection)
 
-    upload_directory(collection, parsed_args.dir)
+    if parsed_args.dir:
+        upload_directory(collection, parsed_args.dir)
+    elif parsed_args.file:
+        upload_file(collection, parsed_args.file)
+    elif unknown_args:
+        for arg in unknown_args:
+            if os.path.isfile(arg):
+                upload_file(collection, arg)
+            elif os.path.isdir(arg):
+                upload_directory(collection, arg)
+            else:
+                print(f"Skipping unknown argument: {arg}")
+    else:
+        print("Please provide a valid file or directory to upload")
+        parser.print_help(sys.stderr)
+        sys.exit(1)
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `jiggybase-0.0.24/jiggybase/examples/upload_email_example.py` & `jiggybase-0.0.25/jiggybase/examples/upload_email_example.py`

 * *Files identical despite different names*

### Comparing `jiggybase-0.0.24/jiggybase/jiggybase_session.py` & `jiggybase-0.0.25/jiggybase/jiggybase_session.py`

 * *Files identical despite different names*

### Comparing `jiggybase-0.0.24/jiggybase/login.py` & `jiggybase-0.0.25/jiggybase/login.py`

 * *Files identical despite different names*

### Comparing `jiggybase-0.0.24/jiggybase/models/auth.py` & `jiggybase-0.0.25/jiggybase/models/auth.py`

 * *Files identical despite different names*

### Comparing `jiggybase-0.0.24/jiggybase/models/chat.py` & `jiggybase-0.0.25/jiggybase/models/chat.py`

 * *Files identical despite different names*

### Comparing `jiggybase-0.0.24/jiggybase/models/chunk.py` & `jiggybase-0.0.25/jiggybase/models/chunk.py`

 * *Files identical despite different names*

### Comparing `jiggybase-0.0.24/jiggybase/models/collection.py` & `jiggybase-0.0.25/jiggybase/models/collection.py`

 * *Files identical despite different names*

### Comparing `jiggybase-0.0.24/jiggybase/models/metadata.py` & `jiggybase-0.0.25/jiggybase/models/metadata.py`

 * *Files identical despite different names*

### Comparing `jiggybase-0.0.24/jiggybase/models/org.py` & `jiggybase-0.0.25/jiggybase/models/org.py`

 * *Files identical despite different names*

### Comparing `jiggybase-0.0.24/jiggybase/models/plugin.py` & `jiggybase-0.0.25/jiggybase/models/plugin.py`

 * *Files identical despite different names*

### Comparing `jiggybase-0.0.24/jiggybase/models/plugin_config.py` & `jiggybase-0.0.25/jiggybase/models/plugin_config.py`

 * *Files identical despite different names*

### Comparing `jiggybase-0.0.24/jiggybase/models/prompt.py` & `jiggybase-0.0.25/jiggybase/models/prompt.py`

 * *Files identical despite different names*

### Comparing `jiggybase-0.0.24/jiggybase/models/providers.py` & `jiggybase-0.0.25/jiggybase/models/providers.py`

 * *Files identical despite different names*

### Comparing `jiggybase-0.0.24/jiggybase/models/user.py` & `jiggybase-0.0.25/jiggybase/models/user.py`

 * *Files identical despite different names*

### Comparing `jiggybase-0.0.24/jiggybase/org.py` & `jiggybase-0.0.25/jiggybase/org.py`

 * *Files identical despite different names*

### Comparing `jiggybase-0.0.24/jiggybase.egg-info/PKG-INFO` & `jiggybase-0.0.25/jiggybase.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jiggybase
-Version: 0.0.24
+Version: 0.0.25
 Summary: Client for Jiggy AI JiggyBase, including ChatGPT Retriever Plugins
 Author-email: Bill Kish <bk@jiggy.ai>
 Project-URL: Homepage, https://github.com/jiggy-ai/jiggybase
 Project-URL: Bug Tracker, https://github.com/jiggy-ai/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

### Comparing `jiggybase-0.0.24/jiggybase.egg-info/SOURCES.txt` & `jiggybase-0.0.25/jiggybase.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `jiggybase-0.0.24/pyproject.toml` & `jiggybase-0.0.25/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "jiggybase"
-version = "0.0.24"
+version = "0.0.25"
 authors = [
   { name="Bill Kish", email="bk@jiggy.ai" },
 ]
 dependencies=['loguru', 'pydantic[email]', 'requests']
 description = "Client for Jiggy AI JiggyBase, including ChatGPT Retriever Plugins"
 readme = "README.md"
 requires-python = ">=3.9"
```

### Comparing `jiggybase-0.0.24/test/test.py` & `jiggybase-0.0.25/test/test.py`

 * *Files identical despite different names*

