# Comparing `tmp/jiggybase-0.0.23.tar.gz` & `tmp/jiggybase-0.0.24.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jiggybase-0.0.23.tar", last modified: Fri May  5 00:39:31 2023, max compression
+gzip compressed data, was "jiggybase-0.0.24.tar", last modified: Fri May  5 00:50:52 2023, max compression
```

## Comparing `jiggybase-0.0.23.tar` & `jiggybase-0.0.24.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxr-xr-x   0 wsk        (501) staff       (20)        0 2023-05-05 00:39:31.290938 jiggybase-0.0.23/
--rw-r--r--   0 wsk        (501) staff       (20)    11357 2023-04-10 04:07:02.000000 jiggybase-0.0.23/LICENSE
--rw-r--r--   0 wsk        (501) staff       (20)     5826 2023-05-05 00:39:31.290518 jiggybase-0.0.23/PKG-INFO
--rw-r--r--   0 wsk        (501) staff       (20)     5292 2023-05-01 15:45:10.000000 jiggybase-0.0.23/README.md
-drwxr-xr-x   0 wsk        (501) staff       (20)        0 2023-05-05 00:39:31.282317 jiggybase-0.0.23/jiggybase/
--rw-r--r--   0 wsk        (501) staff       (20)       30 2023-04-28 15:28:30.000000 jiggybase-0.0.23/jiggybase/__init__.py
--rw-r--r--   0 wsk        (501) staff       (20)     2044 2023-05-01 01:40:42.000000 jiggybase-0.0.23/jiggybase/client.py
--rw-r--r--   0 wsk        (501) staff       (20)     8508 2023-04-30 00:50:55.000000 jiggybase-0.0.23/jiggybase/collection.py
-drwxr-xr-x   0 wsk        (501) staff       (20)        0 2023-05-05 00:39:31.284701 jiggybase-0.0.23/jiggybase/examples/
--rwxr-xr-x   0 wsk        (501) staff       (20)     2233 2023-05-04 23:46:16.000000 jiggybase-0.0.23/jiggybase/examples/jiggybase_upload.py
--rw-r--r--   0 wsk        (501) staff       (20)     1361 2023-05-03 07:37:11.000000 jiggybase-0.0.23/jiggybase/examples/upload_email_example.py
--rw-r--r--   0 wsk        (501) staff       (20)     4531 2023-04-29 04:12:14.000000 jiggybase-0.0.23/jiggybase/jiggybase_session.py
--rw-r--r--   0 wsk        (501) staff       (20)     1187 2023-03-30 18:09:13.000000 jiggybase-0.0.23/jiggybase/login.py
-drwxr-xr-x   0 wsk        (501) staff       (20)        0 2023-05-05 00:39:31.289683 jiggybase-0.0.23/jiggybase/models/
--rw-r--r--   0 wsk        (501) staff       (20)      273 2023-04-26 01:37:49.000000 jiggybase-0.0.23/jiggybase/models/__init__.py
--rw-r--r--   0 wsk        (501) staff       (20)     1236 2023-04-10 05:17:32.000000 jiggybase-0.0.23/jiggybase/models/auth.py
--rw-r--r--   0 wsk        (501) staff       (20)     1007 2023-04-23 16:10:39.000000 jiggybase-0.0.23/jiggybase/models/chat.py
--rw-r--r--   0 wsk        (501) staff       (20)      188 2023-04-23 04:17:06.000000 jiggybase-0.0.23/jiggybase/models/chatmodel.py
--rw-r--r--   0 wsk        (501) staff       (20)     1322 2023-04-10 16:54:34.000000 jiggybase-0.0.23/jiggybase/models/chunk.py
--rw-r--r--   0 wsk        (501) staff       (20)     4240 2023-04-20 21:45:37.000000 jiggybase-0.0.23/jiggybase/models/collection.py
--rw-r--r--   0 wsk        (501) staff       (20)      454 2023-04-23 05:06:00.000000 jiggybase-0.0.23/jiggybase/models/embedding.py
--rw-r--r--   0 wsk        (501) staff       (20)      696 2023-04-10 04:48:20.000000 jiggybase-0.0.23/jiggybase/models/metadata.py
--rw-r--r--   0 wsk        (501) staff       (20)     2214 2023-04-10 04:58:39.000000 jiggybase-0.0.23/jiggybase/models/org.py
--rw-r--r--   0 wsk        (501) staff       (20)     2777 2023-04-29 00:07:44.000000 jiggybase-0.0.23/jiggybase/models/plugin.py
--rw-r--r--   0 wsk        (501) staff       (20)     3415 2023-05-04 23:56:42.000000 jiggybase-0.0.23/jiggybase/models/plugin_config.py
--rw-r--r--   0 wsk        (501) staff       (20)     2834 2023-04-22 23:44:02.000000 jiggybase-0.0.23/jiggybase/models/prompt.py
--rw-r--r--   0 wsk        (501) staff       (20)     3012 2023-04-11 17:29:49.000000 jiggybase-0.0.23/jiggybase/models/providers.py
--rw-r--r--   0 wsk        (501) staff       (20)     1820 2023-04-17 16:14:19.000000 jiggybase-0.0.23/jiggybase/models/user.py
--rw-r--r--   0 wsk        (501) staff       (20)     4600 2023-04-29 15:22:54.000000 jiggybase-0.0.23/jiggybase/org.py
-drwxr-xr-x   0 wsk        (501) staff       (20)        0 2023-05-05 00:39:31.284090 jiggybase-0.0.23/jiggybase.egg-info/
--rw-r--r--   0 wsk        (501) staff       (20)     5826 2023-05-05 00:39:31.000000 jiggybase-0.0.23/jiggybase.egg-info/PKG-INFO
--rw-r--r--   0 wsk        (501) staff       (20)      852 2023-05-05 00:39:31.000000 jiggybase-0.0.23/jiggybase.egg-info/SOURCES.txt
--rw-r--r--   0 wsk        (501) staff       (20)        1 2023-05-05 00:39:31.000000 jiggybase-0.0.23/jiggybase.egg-info/dependency_links.txt
--rw-r--r--   0 wsk        (501) staff       (20)       78 2023-05-05 00:39:31.000000 jiggybase-0.0.23/jiggybase.egg-info/entry_points.txt
--rw-r--r--   0 wsk        (501) staff       (20)       32 2023-05-05 00:39:31.000000 jiggybase-0.0.23/jiggybase.egg-info/requires.txt
--rw-r--r--   0 wsk        (501) staff       (20)       10 2023-05-05 00:39:31.000000 jiggybase-0.0.23/jiggybase.egg-info/top_level.txt
--rw-r--r--   0 wsk        (501) staff       (20)      752 2023-05-05 00:38:32.000000 jiggybase-0.0.23/pyproject.toml
--rw-r--r--   0 wsk        (501) staff       (20)       38 2023-05-05 00:39:31.291055 jiggybase-0.0.23/setup.cfg
-drwxr-xr-x   0 wsk        (501) staff       (20)        0 2023-05-05 00:39:31.290027 jiggybase-0.0.23/test/
--rw-r--r--   0 wsk        (501) staff       (20)      830 2023-04-28 15:38:35.000000 jiggybase-0.0.23/test/test.py
+drwxr-xr-x   0 wsk        (501) staff       (20)        0 2023-05-05 00:50:52.187026 jiggybase-0.0.24/
+-rw-r--r--   0 wsk        (501) staff       (20)    11357 2023-04-10 04:07:02.000000 jiggybase-0.0.24/LICENSE
+-rw-r--r--   0 wsk        (501) staff       (20)     5826 2023-05-05 00:50:52.186771 jiggybase-0.0.24/PKG-INFO
+-rw-r--r--   0 wsk        (501) staff       (20)     5292 2023-05-01 15:45:10.000000 jiggybase-0.0.24/README.md
+drwxr-xr-x   0 wsk        (501) staff       (20)        0 2023-05-05 00:50:52.180362 jiggybase-0.0.24/jiggybase/
+-rw-r--r--   0 wsk        (501) staff       (20)       30 2023-04-28 15:28:30.000000 jiggybase-0.0.24/jiggybase/__init__.py
+-rw-r--r--   0 wsk        (501) staff       (20)     2044 2023-05-01 01:40:42.000000 jiggybase-0.0.24/jiggybase/client.py
+-rw-r--r--   0 wsk        (501) staff       (20)     8508 2023-04-30 00:50:55.000000 jiggybase-0.0.24/jiggybase/collection.py
+drwxr-xr-x   0 wsk        (501) staff       (20)        0 2023-05-05 00:50:52.182520 jiggybase-0.0.24/jiggybase/examples/
+-rwxr-xr-x   0 wsk        (501) staff       (20)     2225 2023-05-05 00:50:28.000000 jiggybase-0.0.24/jiggybase/examples/jiggybase_upload.py
+-rw-r--r--   0 wsk        (501) staff       (20)     1361 2023-05-03 07:37:11.000000 jiggybase-0.0.24/jiggybase/examples/upload_email_example.py
+-rw-r--r--   0 wsk        (501) staff       (20)     4531 2023-04-29 04:12:14.000000 jiggybase-0.0.24/jiggybase/jiggybase_session.py
+-rw-r--r--   0 wsk        (501) staff       (20)     1187 2023-03-30 18:09:13.000000 jiggybase-0.0.24/jiggybase/login.py
+drwxr-xr-x   0 wsk        (501) staff       (20)        0 2023-05-05 00:50:52.186206 jiggybase-0.0.24/jiggybase/models/
+-rw-r--r--   0 wsk        (501) staff       (20)      273 2023-04-26 01:37:49.000000 jiggybase-0.0.24/jiggybase/models/__init__.py
+-rw-r--r--   0 wsk        (501) staff       (20)     1236 2023-04-10 05:17:32.000000 jiggybase-0.0.24/jiggybase/models/auth.py
+-rw-r--r--   0 wsk        (501) staff       (20)     1007 2023-04-23 16:10:39.000000 jiggybase-0.0.24/jiggybase/models/chat.py
+-rw-r--r--   0 wsk        (501) staff       (20)      188 2023-04-23 04:17:06.000000 jiggybase-0.0.24/jiggybase/models/chatmodel.py
+-rw-r--r--   0 wsk        (501) staff       (20)     1322 2023-04-10 16:54:34.000000 jiggybase-0.0.24/jiggybase/models/chunk.py
+-rw-r--r--   0 wsk        (501) staff       (20)     4240 2023-04-20 21:45:37.000000 jiggybase-0.0.24/jiggybase/models/collection.py
+-rw-r--r--   0 wsk        (501) staff       (20)      454 2023-04-23 05:06:00.000000 jiggybase-0.0.24/jiggybase/models/embedding.py
+-rw-r--r--   0 wsk        (501) staff       (20)      696 2023-04-10 04:48:20.000000 jiggybase-0.0.24/jiggybase/models/metadata.py
+-rw-r--r--   0 wsk        (501) staff       (20)     2214 2023-04-10 04:58:39.000000 jiggybase-0.0.24/jiggybase/models/org.py
+-rw-r--r--   0 wsk        (501) staff       (20)     2777 2023-04-29 00:07:44.000000 jiggybase-0.0.24/jiggybase/models/plugin.py
+-rw-r--r--   0 wsk        (501) staff       (20)     3415 2023-05-04 23:56:42.000000 jiggybase-0.0.24/jiggybase/models/plugin_config.py
+-rw-r--r--   0 wsk        (501) staff       (20)     2834 2023-04-22 23:44:02.000000 jiggybase-0.0.24/jiggybase/models/prompt.py
+-rw-r--r--   0 wsk        (501) staff       (20)     3012 2023-04-11 17:29:49.000000 jiggybase-0.0.24/jiggybase/models/providers.py
+-rw-r--r--   0 wsk        (501) staff       (20)     1820 2023-04-17 16:14:19.000000 jiggybase-0.0.24/jiggybase/models/user.py
+-rw-r--r--   0 wsk        (501) staff       (20)     4600 2023-04-29 15:22:54.000000 jiggybase-0.0.24/jiggybase/org.py
+drwxr-xr-x   0 wsk        (501) staff       (20)        0 2023-05-05 00:50:52.181979 jiggybase-0.0.24/jiggybase.egg-info/
+-rw-r--r--   0 wsk        (501) staff       (20)     5826 2023-05-05 00:50:52.000000 jiggybase-0.0.24/jiggybase.egg-info/PKG-INFO
+-rw-r--r--   0 wsk        (501) staff       (20)      852 2023-05-05 00:50:52.000000 jiggybase-0.0.24/jiggybase.egg-info/SOURCES.txt
+-rw-r--r--   0 wsk        (501) staff       (20)        1 2023-05-05 00:50:52.000000 jiggybase-0.0.24/jiggybase.egg-info/dependency_links.txt
+-rw-r--r--   0 wsk        (501) staff       (20)       78 2023-05-05 00:50:52.000000 jiggybase-0.0.24/jiggybase.egg-info/entry_points.txt
+-rw-r--r--   0 wsk        (501) staff       (20)       32 2023-05-05 00:50:52.000000 jiggybase-0.0.24/jiggybase.egg-info/requires.txt
+-rw-r--r--   0 wsk        (501) staff       (20)       10 2023-05-05 00:50:52.000000 jiggybase-0.0.24/jiggybase.egg-info/top_level.txt
+-rw-r--r--   0 wsk        (501) staff       (20)      752 2023-05-05 00:49:54.000000 jiggybase-0.0.24/pyproject.toml
+-rw-r--r--   0 wsk        (501) staff       (20)       38 2023-05-05 00:50:52.187095 jiggybase-0.0.24/setup.cfg
+drwxr-xr-x   0 wsk        (501) staff       (20)        0 2023-05-05 00:50:52.186462 jiggybase-0.0.24/test/
+-rw-r--r--   0 wsk        (501) staff       (20)      830 2023-04-28 15:38:35.000000 jiggybase-0.0.24/test/test.py
```

### Comparing `jiggybase-0.0.23/LICENSE` & `jiggybase-0.0.24/LICENSE`

 * *Files identical despite different names*

### Comparing `jiggybase-0.0.23/PKG-INFO` & `jiggybase-0.0.24/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jiggybase
-Version: 0.0.23
+Version: 0.0.24
 Summary: Client for Jiggy AI JiggyBase, including ChatGPT Retriever Plugins
 Author-email: Bill Kish <bk@jiggy.ai>
 Project-URL: Homepage, https://github.com/jiggy-ai/jiggybase
 Project-URL: Bug Tracker, https://github.com/jiggy-ai/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

### Comparing `jiggybase-0.0.23/README.md` & `jiggybase-0.0.24/README.md`

 * *Files identical despite different names*

### Comparing `jiggybase-0.0.23/jiggybase/client.py` & `jiggybase-0.0.24/jiggybase/client.py`

 * *Files identical despite different names*

### Comparing `jiggybase-0.0.23/jiggybase/collection.py` & `jiggybase-0.0.24/jiggybase/collection.py`

 * *Files identical despite different names*

### Comparing `jiggybase-0.0.23/jiggybase/examples/jiggybase_upload.py` & `jiggybase-0.0.24/jiggybase/examples/jiggybase_upload.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,25 +22,25 @@
             continue
         doc_id = upsert_rsp.ids[0]
         dcl =  collection.get_doc(doc_id)
         text_len = len(" ".join([dc.text for dc in dcl]))
         print(f'uploaded {fn} as {doc_id}: chunk count {len(dcl)} text length {text_len} metadata {dcl[0].metadata}')
 
 
-def main(args):
+def main():
     parser = argparse.ArgumentParser(description="Upload a directory to a JiggyBase collection")
     parser.add_argument("--org", type=str, help="The name of your JiggyBase organization")
     parser.add_argument("--collection", type=str, help="The name of your JiggyBase collection")
     parser.add_argument("--dir", type=str, help="The directory you want to upload")
 
     if len(sys.argv) == 1:
         parser.print_help(sys.stderr)
         sys.exit(1)
 
-    parsed_args = parser.parse_args(args)
+    parsed_args = parser.parse_args(sys.argv[1:])
 
     if not parsed_args.org:
         orgs = jb.orgs()
         if len(orgs) > 1:
             print("Please provide an organization name using the --org option")
             sys.exit(1)
         elif JIGGYBASE_ORG:
@@ -62,8 +62,8 @@
     else:
         collection = org.collection(parsed_args.collection)
 
     upload_directory(collection, parsed_args.dir)
 
 
 if __name__ == "__main__":
-    main(sys.argv[1:])
+    main()
```

### Comparing `jiggybase-0.0.23/jiggybase/examples/upload_email_example.py` & `jiggybase-0.0.24/jiggybase/examples/upload_email_example.py`

 * *Files identical despite different names*

### Comparing `jiggybase-0.0.23/jiggybase/jiggybase_session.py` & `jiggybase-0.0.24/jiggybase/jiggybase_session.py`

 * *Files identical despite different names*

### Comparing `jiggybase-0.0.23/jiggybase/login.py` & `jiggybase-0.0.24/jiggybase/login.py`

 * *Files identical despite different names*

### Comparing `jiggybase-0.0.23/jiggybase/models/auth.py` & `jiggybase-0.0.24/jiggybase/models/auth.py`

 * *Files identical despite different names*

### Comparing `jiggybase-0.0.23/jiggybase/models/chat.py` & `jiggybase-0.0.24/jiggybase/models/chat.py`

 * *Files identical despite different names*

### Comparing `jiggybase-0.0.23/jiggybase/models/chunk.py` & `jiggybase-0.0.24/jiggybase/models/chunk.py`

 * *Files identical despite different names*

### Comparing `jiggybase-0.0.23/jiggybase/models/collection.py` & `jiggybase-0.0.24/jiggybase/models/collection.py`

 * *Files identical despite different names*

### Comparing `jiggybase-0.0.23/jiggybase/models/metadata.py` & `jiggybase-0.0.24/jiggybase/models/metadata.py`

 * *Files identical despite different names*

### Comparing `jiggybase-0.0.23/jiggybase/models/org.py` & `jiggybase-0.0.24/jiggybase/models/org.py`

 * *Files identical despite different names*

### Comparing `jiggybase-0.0.23/jiggybase/models/plugin.py` & `jiggybase-0.0.24/jiggybase/models/plugin.py`

 * *Files identical despite different names*

### Comparing `jiggybase-0.0.23/jiggybase/models/plugin_config.py` & `jiggybase-0.0.24/jiggybase/models/plugin_config.py`

 * *Files identical despite different names*

### Comparing `jiggybase-0.0.23/jiggybase/models/prompt.py` & `jiggybase-0.0.24/jiggybase/models/prompt.py`

 * *Files identical despite different names*

### Comparing `jiggybase-0.0.23/jiggybase/models/providers.py` & `jiggybase-0.0.24/jiggybase/models/providers.py`

 * *Files identical despite different names*

### Comparing `jiggybase-0.0.23/jiggybase/models/user.py` & `jiggybase-0.0.24/jiggybase/models/user.py`

 * *Files identical despite different names*

### Comparing `jiggybase-0.0.23/jiggybase/org.py` & `jiggybase-0.0.24/jiggybase/org.py`

 * *Files identical despite different names*

### Comparing `jiggybase-0.0.23/jiggybase.egg-info/PKG-INFO` & `jiggybase-0.0.24/jiggybase.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: jiggybase
-Version: 0.0.23
+Version: 0.0.24
 Summary: Client for Jiggy AI JiggyBase, including ChatGPT Retriever Plugins
 Author-email: Bill Kish <bk@jiggy.ai>
 Project-URL: Homepage, https://github.com/jiggy-ai/jiggybase
 Project-URL: Bug Tracker, https://github.com/jiggy-ai/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: OS Independent
```

### Comparing `jiggybase-0.0.23/jiggybase.egg-info/SOURCES.txt` & `jiggybase-0.0.24/jiggybase.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `jiggybase-0.0.23/pyproject.toml` & `jiggybase-0.0.24/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "jiggybase"
-version = "0.0.23"
+version = "0.0.24"
 authors = [
   { name="Bill Kish", email="bk@jiggy.ai" },
 ]
 dependencies=['loguru', 'pydantic[email]', 'requests']
 description = "Client for Jiggy AI JiggyBase, including ChatGPT Retriever Plugins"
 readme = "README.md"
 requires-python = ">=3.9"
```

### Comparing `jiggybase-0.0.23/test/test.py` & `jiggybase-0.0.24/test/test.py`

 * *Files identical despite different names*

