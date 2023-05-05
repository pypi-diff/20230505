# Comparing `tmp/unitranscode-0.3.2.tar.gz` & `tmp/unitranscode-0.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "unitranscode-0.3.2.tar", last modified: Mon May  1 05:16:24 2023, max compression
+gzip compressed data, was "unitranscode-0.3.3.tar", last modified: Fri May  5 08:31:23 2023, max compression
```

## Comparing `unitranscode-0.3.2.tar` & `unitranscode-0.3.3.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxrwxr-x   0 matthew   (1000) matthew   (1000)        0 2023-05-01 05:16:24.884529 unitranscode-0.3.2/
--rw-rw-r--   0 matthew   (1000) matthew   (1000)     1062 2023-01-01 01:11:48.000000 unitranscode-0.3.2/LICENSE
--rw-rw-r--   0 matthew   (1000) matthew   (1000)      558 2023-05-01 05:16:24.884529 unitranscode-0.3.2/PKG-INFO
--rw-rw-r--   0 matthew   (1000) matthew   (1000)     1399 2023-01-01 03:15:58.000000 unitranscode-0.3.2/README.md
--rw-rw-r--   0 matthew   (1000) matthew   (1000)       38 2023-05-01 05:16:24.884529 unitranscode-0.3.2/setup.cfg
--rw-rw-r--   0 matthew   (1000) matthew   (1000)      717 2023-05-01 05:15:41.000000 unitranscode-0.3.2/setup.py
-drwxrwxr-x   0 matthew   (1000) matthew   (1000)        0 2023-05-01 05:16:24.852530 unitranscode-0.3.2/tests/
--rw-rw-r--   0 matthew   (1000) matthew   (1000)     1138 2023-04-28 03:34:33.000000 unitranscode-0.3.2/tests/test_transcoder.py
-drwxrwxr-x   0 matthew   (1000) matthew   (1000)        0 2023-05-01 05:16:24.884529 unitranscode-0.3.2/unitranscode/
--rw-rw-r--   0 matthew   (1000) matthew   (1000)      411 2023-01-01 01:28:59.000000 unitranscode-0.3.2/unitranscode/__init__.py
--rw-rw-r--   0 matthew   (1000) matthew   (1000)     3661 2023-04-28 03:37:11.000000 unitranscode-0.3.2/unitranscode/custom_types.py
--rw-rw-r--   0 matthew   (1000) matthew   (1000)    25254 2023-05-01 05:15:19.000000 unitranscode-0.3.2/unitranscode/transcoder.py
--rw-rw-r--   0 matthew   (1000) matthew   (1000)      137 2023-05-01 05:12:02.000000 unitranscode-0.3.2/unitranscode/utils.py
-drwxrwxr-x   0 matthew   (1000) matthew   (1000)        0 2023-05-01 05:16:24.884529 unitranscode-0.3.2/unitranscode.egg-info/
--rw-rw-r--   0 matthew   (1000) matthew   (1000)      558 2023-05-01 05:16:24.000000 unitranscode-0.3.2/unitranscode.egg-info/PKG-INFO
--rw-rw-r--   0 matthew   (1000) matthew   (1000)      333 2023-05-01 05:16:24.000000 unitranscode-0.3.2/unitranscode.egg-info/SOURCES.txt
--rw-rw-r--   0 matthew   (1000) matthew   (1000)        1 2023-05-01 05:16:24.000000 unitranscode-0.3.2/unitranscode.egg-info/dependency_links.txt
--rw-rw-r--   0 matthew   (1000) matthew   (1000)        7 2023-05-01 05:16:24.000000 unitranscode-0.3.2/unitranscode.egg-info/requires.txt
--rw-rw-r--   0 matthew   (1000) matthew   (1000)       13 2023-05-01 05:16:24.000000 unitranscode-0.3.2/unitranscode.egg-info/top_level.txt
+drwxrwxr-x   0 matthew   (1000) matthew   (1000)        0 2023-05-05 08:31:23.014281 unitranscode-0.3.3/
+-rw-rw-r--   0 matthew   (1000) matthew   (1000)     1062 2023-01-01 01:11:48.000000 unitranscode-0.3.3/LICENSE
+-rw-rw-r--   0 matthew   (1000) matthew   (1000)      558 2023-05-05 08:31:23.014281 unitranscode-0.3.3/PKG-INFO
+-rw-rw-r--   0 matthew   (1000) matthew   (1000)     1399 2023-01-01 03:15:58.000000 unitranscode-0.3.3/README.md
+-rw-rw-r--   0 matthew   (1000) matthew   (1000)       38 2023-05-05 08:31:23.014281 unitranscode-0.3.3/setup.cfg
+-rw-rw-r--   0 matthew   (1000) matthew   (1000)      717 2023-05-05 08:30:58.000000 unitranscode-0.3.3/setup.py
+drwxrwxr-x   0 matthew   (1000) matthew   (1000)        0 2023-05-05 08:31:23.010281 unitranscode-0.3.3/tests/
+-rw-rw-r--   0 matthew   (1000) matthew   (1000)     1138 2023-04-28 03:34:33.000000 unitranscode-0.3.3/tests/test_transcoder.py
+drwxrwxr-x   0 matthew   (1000) matthew   (1000)        0 2023-05-05 08:31:23.010281 unitranscode-0.3.3/unitranscode/
+-rw-rw-r--   0 matthew   (1000) matthew   (1000)      411 2023-01-01 01:28:59.000000 unitranscode-0.3.3/unitranscode/__init__.py
+-rw-rw-r--   0 matthew   (1000) matthew   (1000)     3661 2023-04-28 03:37:11.000000 unitranscode-0.3.3/unitranscode/custom_types.py
+-rw-rw-r--   0 matthew   (1000) matthew   (1000)    25714 2023-05-05 08:20:48.000000 unitranscode-0.3.3/unitranscode/transcoder.py
+-rw-rw-r--   0 matthew   (1000) matthew   (1000)      137 2023-05-01 05:12:02.000000 unitranscode-0.3.3/unitranscode/utils.py
+drwxrwxr-x   0 matthew   (1000) matthew   (1000)        0 2023-05-05 08:31:23.014281 unitranscode-0.3.3/unitranscode.egg-info/
+-rw-rw-r--   0 matthew   (1000) matthew   (1000)      558 2023-05-05 08:31:22.000000 unitranscode-0.3.3/unitranscode.egg-info/PKG-INFO
+-rw-rw-r--   0 matthew   (1000) matthew   (1000)      333 2023-05-05 08:31:22.000000 unitranscode-0.3.3/unitranscode.egg-info/SOURCES.txt
+-rw-rw-r--   0 matthew   (1000) matthew   (1000)        1 2023-05-05 08:31:22.000000 unitranscode-0.3.3/unitranscode.egg-info/dependency_links.txt
+-rw-rw-r--   0 matthew   (1000) matthew   (1000)        7 2023-05-05 08:31:22.000000 unitranscode-0.3.3/unitranscode.egg-info/requires.txt
+-rw-rw-r--   0 matthew   (1000) matthew   (1000)       13 2023-05-05 08:31:22.000000 unitranscode-0.3.3/unitranscode.egg-info/top_level.txt
```

### Comparing `unitranscode-0.3.2/LICENSE` & `unitranscode-0.3.3/LICENSE`

 * *Files identical despite different names*

### Comparing `unitranscode-0.3.2/PKG-INFO` & `unitranscode-0.3.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: unitranscode
-Version: 0.3.2
+Version: 0.3.3
 Summary: Universal transcoding library
 Home-page: https://github.com/MatthewScholefield/unitranscode
 Author: Matthew D. Scholefield
 Author-email: matthew331199@gmail.com
 Keywords: unitranscode
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

### Comparing `unitranscode-0.3.2/README.md` & `unitranscode-0.3.3/README.md`

 * *Files identical despite different names*

### Comparing `unitranscode-0.3.2/setup.py` & `unitranscode-0.3.3/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup
 
 
 setup(
     name='unitranscode',
-    version='0.3.2',
+    version='0.3.3',
     description='Universal transcoding library',
     url='https://github.com/MatthewScholefield/unitranscode',
     author='Matthew D. Scholefield',
     author_email='matthew331199@gmail.com',
     classifiers=[
         'Development Status :: 3 - Alpha',
         'Intended Audience :: Developers',
```

### Comparing `unitranscode-0.3.2/tests/test_transcoder.py` & `unitranscode-0.3.3/tests/test_transcoder.py`

 * *Files identical despite different names*

### Comparing `unitranscode-0.3.2/unitranscode/custom_types.py` & `unitranscode-0.3.3/unitranscode/custom_types.py`

 * *Files identical despite different names*

### Comparing `unitranscode-0.3.2/unitranscode/transcoder.py` & `unitranscode-0.3.3/unitranscode/transcoder.py`

 * *Files 1% similar despite different names*

```diff
@@ -73,21 +73,31 @@
     def pause_pid(pid: int):
         os.kill(pid, SIGTSTP)
 
     def pause(self, _with_lock=True):
         with self.pause_lock if _with_lock else nullcontext():
             self.is_paused = True
             if self._proc:
-                self.pause_pid(self.proc.pid)
+                try:
+                    self.pause_pid(self.proc.pid)
+                except ProcessLookupError:
+                    assert (
+                        self._proc.poll() is not None
+                    ), 'Error: Process not terminated, but failed to find PID'
 
     def resume(self, _with_lock=True):
         with self.pause_lock if _with_lock else nullcontext():
             self.is_paused = False
             if self._proc:
-                self.resume_pid(self.proc.pid)
+                try:
+                    self.resume_pid(self.proc.pid)
+                except ProcessLookupError:
+                    assert (
+                        self._proc.poll() is not None
+                    ), 'Error: Process not terminated, but failed to find PID'
 
     def cancel(self):
         with self.pause_lock:
             self.cancelled = True
             if self._proc:
                 self._proc.kill()
```

### Comparing `unitranscode-0.3.2/unitranscode.egg-info/PKG-INFO` & `unitranscode-0.3.3/unitranscode.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: unitranscode
-Version: 0.3.2
+Version: 0.3.3
 Summary: Universal transcoding library
 Home-page: https://github.com/MatthewScholefield/unitranscode
 Author: Matthew D. Scholefield
 Author-email: matthew331199@gmail.com
 Keywords: unitranscode
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
```

