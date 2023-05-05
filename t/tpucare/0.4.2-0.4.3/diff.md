# Comparing `tmp/tpucare-0.4.2.tar.gz` & `tmp/tpucare-0.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tpucare-0.4.2.tar", last modified: Wed May  3 14:23:41 2023, max compression
+gzip compressed data, was "tpucare-0.4.3.tar", last modified: Fri May  5 11:57:56 2023, max compression
```

## Comparing `tpucare-0.4.2.tar` & `tpucare-0.4.3.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxr-x   0 lucas     (1000) lucas     (1000)        0 2023-05-03 14:23:41.226373 tpucare-0.4.2/
--rw-rw-r--   0 lucas     (1000) lucas     (1000)     1323 2023-05-02 17:44:22.000000 tpucare-0.4.2/LICENSE
--rw-rw-r--   0 lucas     (1000) lucas     (1000)     8366 2023-05-03 14:23:41.226373 tpucare-0.4.2/PKG-INFO
--rw-rw-r--   0 lucas     (1000) lucas     (1000)     7570 2023-05-02 17:44:22.000000 tpucare-0.4.2/README.md
--rw-rw-r--   0 lucas     (1000) lucas     (1000)       38 2023-05-03 14:23:41.226373 tpucare-0.4.2/setup.cfg
--rw-rw-r--   0 lucas     (1000) lucas     (1000)     1106 2023-05-03 14:23:19.000000 tpucare-0.4.2/setup.py
-drwxrwxr-x   0 lucas     (1000) lucas     (1000)        0 2023-05-03 14:23:41.226373 tpucare-0.4.2/tpucare/
--rw-rw-r--   0 lucas     (1000) lucas     (1000)    11095 2023-05-03 13:35:37.000000 tpucare-0.4.2/tpucare/__init__.py
-drwxrwxr-x   0 lucas     (1000) lucas     (1000)        0 2023-05-03 14:23:41.226373 tpucare-0.4.2/tpucare.egg-info/
--rw-rw-r--   0 lucas     (1000) lucas     (1000)     8366 2023-05-03 14:23:41.000000 tpucare-0.4.2/tpucare.egg-info/PKG-INFO
--rw-rw-r--   0 lucas     (1000) lucas     (1000)      170 2023-05-03 14:23:41.000000 tpucare-0.4.2/tpucare.egg-info/SOURCES.txt
--rw-rw-r--   0 lucas     (1000) lucas     (1000)        1 2023-05-03 14:23:41.000000 tpucare-0.4.2/tpucare.egg-info/dependency_links.txt
--rw-rw-r--   0 lucas     (1000) lucas     (1000)        8 2023-05-03 14:23:41.000000 tpucare-0.4.2/tpucare.egg-info/top_level.txt
+drwxrwxr-x   0 lucas     (1000) lucas     (1000)        0 2023-05-05 11:57:56.356714 tpucare-0.4.3/
+-rw-rw-r--   0 lucas     (1000) lucas     (1000)     1323 2023-05-02 17:44:22.000000 tpucare-0.4.3/LICENSE
+-rw-rw-r--   0 lucas     (1000) lucas     (1000)     8366 2023-05-05 11:57:56.356714 tpucare-0.4.3/PKG-INFO
+-rw-rw-r--   0 lucas     (1000) lucas     (1000)     7570 2023-05-02 17:44:22.000000 tpucare-0.4.3/README.md
+-rw-rw-r--   0 lucas     (1000) lucas     (1000)       38 2023-05-05 11:57:56.356714 tpucare-0.4.3/setup.cfg
+-rw-rw-r--   0 lucas     (1000) lucas     (1000)     1106 2023-05-05 11:57:42.000000 tpucare-0.4.3/setup.py
+drwxrwxr-x   0 lucas     (1000) lucas     (1000)        0 2023-05-05 11:57:56.356714 tpucare-0.4.3/tpucare/
+-rw-rw-r--   0 lucas     (1000) lucas     (1000)    11123 2023-05-05 11:57:30.000000 tpucare-0.4.3/tpucare/__init__.py
+drwxrwxr-x   0 lucas     (1000) lucas     (1000)        0 2023-05-05 11:57:56.356714 tpucare-0.4.3/tpucare.egg-info/
+-rw-rw-r--   0 lucas     (1000) lucas     (1000)     8366 2023-05-05 11:57:56.000000 tpucare-0.4.3/tpucare.egg-info/PKG-INFO
+-rw-rw-r--   0 lucas     (1000) lucas     (1000)      170 2023-05-05 11:57:56.000000 tpucare-0.4.3/tpucare.egg-info/SOURCES.txt
+-rw-rw-r--   0 lucas     (1000) lucas     (1000)        1 2023-05-05 11:57:56.000000 tpucare-0.4.3/tpucare.egg-info/dependency_links.txt
+-rw-rw-r--   0 lucas     (1000) lucas     (1000)        8 2023-05-05 11:57:56.000000 tpucare-0.4.3/tpucare.egg-info/top_level.txt
```

### Comparing `tpucare-0.4.2/LICENSE` & `tpucare-0.4.3/LICENSE`

 * *Files identical despite different names*

### Comparing `tpucare-0.4.2/PKG-INFO` & `tpucare-0.4.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tpucare
-Version: 0.4.2
+Version: 0.4.3
 Summary: Automatically take good care of your preemptible TPUs
 Home-page: https://github.com/clashluke/tpucare
 Author: Lucas Nestler
 Author-email: github.tpucare@nestler.sh
 License: BSD
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: BSD License
```

### Comparing `tpucare-0.4.2/README.md` & `tpucare-0.4.3/README.md`

 * *Files identical despite different names*

### Comparing `tpucare-0.4.2/setup.py` & `tpucare-0.4.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 setuptools.setup(
     author="Lucas Nestler",
     author_email="github.tpucare@nestler.sh",
     name='tpucare',
     license='BSD',
     description='Automatically take good care of your preemptible TPUs',
-    version='0.4.2',
+    version='0.4.3',
     long_description=README,
     url='https://github.com/clashluke/tpucare',
     packages=setuptools.find_packages(),
     python_requires=">=3.7",
     long_description_content_type="text/markdown",
     install_requires=[],
     classifiers=[
```

### Comparing `tpucare-0.4.2/tpucare/__init__.py` & `tpucare-0.4.3/tpucare/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -198,22 +198,24 @@
         return get_name(type(fn), base)
     return base
 
 
 def start_single(host: str, tpu_version: int, zone: str, preemptible: bool, service_account: str, slices: int,
                  start_fn: typing.Callable[[Context, SliceIndex], None],
                  creation_callback: typing.Callable[[str, typing.Optional[Context]], Context],
-                 creation_semaphore: typing.Optional[typing.ContextManager] = None, all_workers: bool = False):
+                 creation_semaphore: typing.Optional[typing.ContextManager] = None, all_workers: bool = False,
+                 unhealthy_timeout_seconds=3600):
     if creation_semaphore is None:
         creation_semaphore = nullcontext()
 
     ctx = None
 
     creation_callback_name = get_name(creation_callback, "creation_callback")
     start_fn_name = get_name(start_fn, "start_fn")
+    unhealthy_timeout_seconds /= CACHE_TIME
 
     while True:
         try:
             log("Recreating TPU", log_level=logging.INFO)
             recreate(host, zone, tpu_version, preemptible, service_account, slices, creation_semaphore)
             log(f"TPU Created. Calling {creation_callback_name}.", log_level=logging.INFO)
             ctx = creation_callback(host, ctx)
@@ -221,25 +223,24 @@
             if all_workers:
                 threads = [multiprocessing.Process(target=start_fn, args=(ctx, "all"), daemon=True)]
             else:
                 threads = [multiprocessing.Process(target=start_fn, args=(ctx, i), daemon=True) for i in range(slices)]
             for t in threads:
                 t.start()
             log("Started start_fn. Babysitting TPU..", log_level=logging.INFO)
-            unhealthy_timeout = 600 / CACHE_TIME  # sometimes "unhealthy" resolves itself. Let's wait up to 10 minutes
+            retries = unhealthy_timeout_seconds  # sometimes "unhealthy" resolves itself. Let's wait
             while host in tpu_names(zone, preempted=False, unhealthy=True):
-                if unhealthy_timeout <= 0:
+                if retries <= 0:
                     break
                 time.sleep(CACHE_TIME)
                 if host in tpu_names(zone, preempted=False, unhealthy=False):
-                    unhealthy_timeout = 600 / CACHE_TIME
+                    retries = unhealthy_timeout_seconds
                 else:
-                    unhealthy_timeout -= 1
-            log(f"TPU is {'unhealthy' if unhealthy_timeout <= 0 else 'preempted'}. Recreating it now.",
-                log_level=logging.INFO)
+                    retries -= 1
+            log(f"TPU is {'unhealthy' if retries <= 0 else 'preempted'}. Recreating it now.", log_level=logging.INFO)
             while any(t.is_alive() for t in threads):
                 for t in threads:
                     if t.is_alive():
                         os.kill(t.pid, signal.SIGINT)
                 time.sleep(0.1)
             log("Sent SIGINT to all workers", log_level=logging.INFO)
         except KeyboardInterrupt:
```

### Comparing `tpucare-0.4.2/tpucare.egg-info/PKG-INFO` & `tpucare-0.4.3/tpucare.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tpucare
-Version: 0.4.2
+Version: 0.4.3
 Summary: Automatically take good care of your preemptible TPUs
 Home-page: https://github.com/clashluke/tpucare
 Author: Lucas Nestler
 Author-email: github.tpucare@nestler.sh
 License: BSD
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: License :: OSI Approved :: BSD License
```

