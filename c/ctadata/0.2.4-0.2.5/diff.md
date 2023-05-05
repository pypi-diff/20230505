# Comparing `tmp/ctadata-0.2.4.tar.gz` & `tmp/ctadata-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ctadata-0.2.4.tar", max compression
+gzip compressed data, was "ctadata-0.2.5.tar", max compression
```

## Comparing `ctadata-0.2.4.tar` & `ctadata-0.2.5.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     2868 2023-04-13 13:02:07.443168 ctadata-0.2.4/README.md
--rw-r--r--   0        0        0      828 2023-04-13 12:10:14.442525 ctadata-0.2.4/ctadata/__init__.py
--rw-r--r--   0        0        0     4125 2023-04-13 14:55:57.598706 ctadata-0.2.4/ctadata/api.py
--rw-r--r--   0        0        0     1052 2023-04-13 12:54:26.214867 ctadata-0.2.4/ctadata/cli.py
--rw-r--r--   0        0        0      199 2023-04-13 09:18:00.949088 ctadata-0.2.4/ctadata/util.py
--rw-r--r--   0        0        0      369 2023-04-13 14:56:39.307201 ctadata-0.2.4/pyproject.toml
--rw-r--r--   0        0        0     3310 1970-01-01 00:00:00.000000 ctadata-0.2.4/PKG-INFO
+-rw-r--r--   0        0        0     2868 2023-05-05 16:42:21.505294 ctadata-0.2.5/README.md
+-rw-r--r--   0        0        0      828 2023-05-05 16:42:21.505294 ctadata-0.2.5/ctadata/__init__.py
+-rw-r--r--   0        0        0     4498 2023-05-05 16:42:21.505294 ctadata-0.2.5/ctadata/api.py
+-rw-r--r--   0        0        0     1355 2023-05-05 16:42:21.505294 ctadata-0.2.5/ctadata/cli.py
+-rw-r--r--   0        0        0      199 2023-05-05 16:42:21.505294 ctadata-0.2.5/ctadata/util.py
+-rw-r--r--   0        0        0      369 2023-05-05 16:43:08.137786 ctadata-0.2.5/pyproject.toml
+-rw-r--r--   0        0        0     3360 1970-01-01 00:00:00.000000 ctadata-0.2.5/PKG-INFO
```

### Comparing `ctadata-0.2.4/README.md` & `ctadata-0.2.5/README.md`

 * *Files identical despite different names*

### Comparing `ctadata-0.2.4/ctadata/__init__.py` & `ctadata-0.2.5/ctadata/__init__.py`

 * *Files identical despite different names*

### Comparing `ctadata-0.2.4/ctadata/api.py` & `ctadata-0.2.5/ctadata/api.py`

 * *Files 10% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 logger = logging.getLogger(__name__)
 
 class StorageException(Exception):
     pass
 
 # TODO: move to bravado and rest
 class APIClient:
-    __export_functions__ = ['list_dir', 'fetch_and_save_file', 'upload_file']
+    __export_functions__ = ['list_dir', 'fetch_and_save_file', 'upload_file', 'upload_dir']
     __class_args__ = ['token', 'downloadservice', 'data_root', 'optional_url_parts', 'chunk_size']
 
     downloadservice = os.getenv("CTADS_URL", "http://hub:5000/services/downloadservice/")
     optional_url_parts = ["services/downloadservice/"]
     
     chunk_size = 10 * 1024 * 1024
 
@@ -115,16 +115,24 @@
             def generate(stats):
                 while r := f.read(self.chunk_size):
                     stats['total_size'] += len(r)
                     logger.info("uploaded %s Mb", stats['total_size']/1024/1024)
                     yield r
 
             r = requests.post(url, data=generate(stats), params={'token': self.token, 'ctadata_version': __version__}, stream=True)
-            logger.info("upload result: %s %s", r, r.json())
-
+            
         if r.status_code != 200:
             logger.error("error: %s", r.text)
             raise StorageException(r.text)
 
+        logger.info("upload result: %s %s", r, r.json())
         return r.json()
+    
+    def upload_dir(self, local_dir, path):
+        logger.info("uploading dir %s to %s", local_dir, path)
+        for (dirpath, dirnames, filenames) in os.walk(local_dir):
+            for name in filenames:
+                fn = os.path.join(dirpath, name)
+                self.upload_file(fn, os.path.join(path, dirpath[len(local_dir):], name))
+
 
 api_client = APIClient()
```

### Comparing `ctadata-0.2.4/ctadata/cli.py` & `ctadata-0.2.5/ctadata/cli.py`

 * *Files 21% similar despite different names*

```diff
@@ -34,15 +34,22 @@
 @click.argument("path", type=str)
 def get_path(ctx, path):
     ctx.obj['api'].fetch_and_save_file(path)
 
 
 @cli.command("put")
 @click.pass_context
-@click.argument("file", type=click.Path(exists=True))
+@click.argument("local_path", type=click.Path(exists=True))
 @click.argument("path", type=str)
-def put_path(ctx, file, path):
-    ctx.obj['api'].upload_file(file, path)
+@click.option("--recursive", "-r", is_flag=True)
+def put_path(ctx, local_path, path, recursive):
+    if os.path.isfile(local_path):        
+        ctx.obj['api'].upload_file(local_path, path)
+    else:
+        if recursive:
+            ctx.obj['api'].upload_dir(local_path, path)
+        else:
+            logger.error("can't upload directory without --recursive flag")
 
 
 def main():
     cli(obj={})
```

### Comparing `ctadata-0.2.4/PKG-INFO` & `ctadata-0.2.5/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,16 @@
 Metadata-Version: 2.1
 Name: ctadata
-Version: 0.2.4
+Version: 0.2.5
 Summary: 
 Author: Volodymyr Savchenko
 Author-email: contact@volodymyrsavchenko.com
-Requires-Python: >=3.9,<4.0
+Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: click (>=8.1.3,<9.0.0)
 Description-Content-Type: text/markdown
 
 # Client for CTA Data Download Service at Swiss CTA DC
```

