# Comparing `tmp/easymp-0.1.7.tar.gz` & `tmp/easymp-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "easymp-0.1.7.tar", last modified: Fri May  5 14:18:00 2023, max compression
+gzip compressed data, was "easymp-0.1.8.tar", last modified: Fri May  5 14:49:19 2023, max compression
```

## Comparing `easymp-0.1.7.tar` & `easymp-0.1.8.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-05-05 14:18:00.982059 easymp-0.1.7/
--rw-r--r--   0 user      (1000) user      (1000)      666 2023-05-05 14:14:53.000000 easymp-0.1.7/LICENSE.txt
--rw-r--r--   0 user      (1000) user      (1000)      899 2023-05-05 14:18:00.982059 easymp-0.1.7/PKG-INFO
--rw-r--r--   0 user      (1000) user      (1000)      582 2023-05-05 14:14:53.000000 easymp-0.1.7/README.md
--rw-r--r--   0 user      (1000) user      (1000)      107 2023-05-05 14:18:00.982059 easymp-0.1.7/setup.cfg
--rw-r--r--   0 user      (1000) user      (1000)      634 2023-05-05 14:17:14.000000 easymp-0.1.7/setup.py
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-05-05 14:18:00.982059 easymp-0.1.7/src/
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-05-05 14:18:00.982059 easymp-0.1.7/src/easymp/
--rw-r--r--   0 user      (1000) user      (1000)       50 2023-05-05 14:14:53.000000 easymp-0.1.7/src/easymp/__init__.py
--rw-r--r--   0 user      (1000) user      (1000)     4049 2023-05-05 14:15:13.000000 easymp-0.1.7/src/easymp/easymp.py
-drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-05-05 14:18:00.982059 easymp-0.1.7/src/easymp.egg-info/
--rw-r--r--   0 user      (1000) user      (1000)      899 2023-05-05 14:18:00.000000 easymp-0.1.7/src/easymp.egg-info/PKG-INFO
--rw-r--r--   0 user      (1000) user      (1000)      220 2023-05-05 14:18:00.000000 easymp-0.1.7/src/easymp.egg-info/SOURCES.txt
--rw-r--r--   0 user      (1000) user      (1000)        1 2023-05-05 14:18:00.000000 easymp-0.1.7/src/easymp.egg-info/dependency_links.txt
--rw-r--r--   0 user      (1000) user      (1000)        7 2023-05-05 14:18:00.000000 easymp-0.1.7/src/easymp.egg-info/top_level.txt
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-05-05 14:49:19.848415 easymp-0.1.8/
+-rw-r--r--   0 user      (1000) user      (1000)      666 2023-05-05 14:14:53.000000 easymp-0.1.8/LICENSE.txt
+-rw-r--r--   0 user      (1000) user      (1000)      899 2023-05-05 14:49:19.848415 easymp-0.1.8/PKG-INFO
+-rw-r--r--   0 user      (1000) user      (1000)      582 2023-05-05 14:14:53.000000 easymp-0.1.8/README.md
+-rw-r--r--   0 user      (1000) user      (1000)      107 2023-05-05 14:49:19.848415 easymp-0.1.8/setup.cfg
+-rw-r--r--   0 user      (1000) user      (1000)      634 2023-05-05 14:48:47.000000 easymp-0.1.8/setup.py
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-05-05 14:49:19.848415 easymp-0.1.8/src/
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-05-05 14:49:19.848415 easymp-0.1.8/src/easymp/
+-rw-r--r--   0 user      (1000) user      (1000)       50 2023-05-05 14:14:53.000000 easymp-0.1.8/src/easymp/__init__.py
+-rw-r--r--   0 user      (1000) user      (1000)     3847 2023-05-05 14:48:21.000000 easymp-0.1.8/src/easymp/easymp.py
+drwxr-xr-x   0 user      (1000) user      (1000)        0 2023-05-05 14:49:19.848415 easymp-0.1.8/src/easymp.egg-info/
+-rw-r--r--   0 user      (1000) user      (1000)      899 2023-05-05 14:49:19.000000 easymp-0.1.8/src/easymp.egg-info/PKG-INFO
+-rw-r--r--   0 user      (1000) user      (1000)      220 2023-05-05 14:49:19.000000 easymp-0.1.8/src/easymp.egg-info/SOURCES.txt
+-rw-r--r--   0 user      (1000) user      (1000)        1 2023-05-05 14:49:19.000000 easymp-0.1.8/src/easymp.egg-info/dependency_links.txt
+-rw-r--r--   0 user      (1000) user      (1000)        7 2023-05-05 14:49:19.000000 easymp-0.1.8/src/easymp.egg-info/top_level.txt
```

### Comparing `easymp-0.1.7/LICENSE.txt` & `easymp-0.1.8/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `easymp-0.1.7/PKG-INFO` & `easymp-0.1.8/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: easymp
-Version: 0.1.7
+Version: 0.1.8
 Summary: Python utility for easy multiprocessing + logging.
 Home-page: https://github.com/MNayer/easymp
 Author: MNayer
 Author-email: marie.nayer@web.de
 License: 0BSD
 Keywords: multiprocessing logging
 Description-Content-Type: text/markdown
```

### Comparing `easymp-0.1.7/README.md` & `easymp-0.1.8/README.md`

 * *Files identical despite different names*

### Comparing `easymp-0.1.7/setup.py` & `easymp-0.1.8/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from pathlib import Path
 
 this_directory = Path(__file__).parent
 long_description = (this_directory / "README.md").read_text()
 
 setup(
     name="easymp",
-    version="0.1.7",
+    version="0.1.8",
     description="Python utility for easy multiprocessing + logging.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     license="0BSD",
     author="MNayer",
     author_email="marie.nayer@web.de",
     packages=find_packages("src"),
```

### Comparing `easymp-0.1.7/src/easymp/easymp.py` & `easymp-0.1.8/src/easymp/easymp.py`

 * *Files 3% similar despite different names*

```diff
@@ -101,24 +101,18 @@
     listener = mp.Process(target=listener_process, args=(queue, listener_configurer))
     listener.start()
     with mp.Pool(nprocs, initializer=worker_init, initargs=(queue, worker_configurer)) as p:
         try:
             res = p.imap_unordered(function, it, chunksize=chunksize)
             if progress:
                 for el in tqdm(res, total=total, file=progress_file):
-                    if yield_results:
-                        yield el
-                    else:
-                        pass
+                    pass
             else:
                 for el in res:
-                    if yield_results:
-                        yield el
-                    else:
-                        pass
+                    pass
             p.close()
             p.join()
             queue.put_nowait(None)
             listener.join()
         except KeyboardInterrupt:
             print("Caught KeyboardInterrupt, terminating workers.")
             p.terminate()
```

### Comparing `easymp-0.1.7/src/easymp.egg-info/PKG-INFO` & `easymp-0.1.8/src/easymp.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: easymp
-Version: 0.1.7
+Version: 0.1.8
 Summary: Python utility for easy multiprocessing + logging.
 Home-page: https://github.com/MNayer/easymp
 Author: MNayer
 Author-email: marie.nayer@web.de
 License: 0BSD
 Keywords: multiprocessing logging
 Description-Content-Type: text/markdown
```

