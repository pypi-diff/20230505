# Comparing `tmp/z3c.insist-1.5.1.tar.gz` & `tmp/z3c.insist-1.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "z3c.insist-1.5.1.tar", last modified: Thu Mar 23 10:52:30 2023, max compression
+gzip compressed data, was "z3c.insist-1.5.2.tar", last modified: Fri May  5 12:49:20 2023, max compression
```

## Comparing `z3c.insist-1.5.1.tar` & `z3c.insist-1.5.2.tar`

### file list

```diff
@@ -1,36 +1,36 @@
-drwxrwxr-x   0 adi       (1000) adi       (1000)        0 2023-03-23 10:52:30.943416 z3c.insist-1.5.1/
--rw-rw-r--   0 adi       (1000) adi       (1000)     2184 2023-03-23 10:52:30.000000 z3c.insist-1.5.1/CHANGES.rst
--rw-rw-r--   0 adi       (1000) adi       (1000)     2070 2023-03-23 10:52:30.000000 z3c.insist-1.5.1/LICENSE
--rw-rw-r--   0 adi       (1000) adi       (1000)      257 2023-03-23 10:52:30.000000 z3c.insist-1.5.1/MANIFEST.in
--rw-rw-r--   0 adi       (1000) adi       (1000)      356 2023-03-23 10:52:30.000000 z3c.insist-1.5.1/Makefile
--rw-rw-r--   0 adi       (1000) adi       (1000)     4025 2023-03-23 10:52:30.943416 z3c.insist-1.5.1/PKG-INFO
--rw-rw-r--   0 adi       (1000) adi       (1000)      942 2023-03-23 10:52:30.000000 z3c.insist-1.5.1/README.rst
--rw-rw-r--   0 adi       (1000) adi       (1000)      145 2023-03-23 10:52:30.943416 z3c.insist-1.5.1/setup.cfg
--rw-rw-r--   0 adi       (1000) adi       (1000)     2199 2023-03-23 10:52:30.000000 z3c.insist-1.5.1/setup.py
-drwxrwxr-x   0 adi       (1000) adi       (1000)        0 2023-03-23 10:52:30.943416 z3c.insist-1.5.1/src/
-drwxrwxr-x   0 adi       (1000) adi       (1000)        0 2023-03-23 10:52:30.943416 z3c.insist-1.5.1/src/z3c/
--rw-rw-r--   0 adi       (1000) adi       (1000)       63 2023-03-23 10:52:30.000000 z3c.insist-1.5.1/src/z3c/__init__.py
-drwxrwxr-x   0 adi       (1000) adi       (1000)        0 2023-03-23 10:52:30.943416 z3c.insist-1.5.1/src/z3c/insist/
--rw-rw-r--   0 adi       (1000) adi       (1000)        0 2023-03-23 10:52:30.000000 z3c.insist-1.5.1/src/z3c/insist/__init__.py
--rw-rw-r--   0 adi       (1000) adi       (1000)      760 2023-03-23 10:52:30.000000 z3c.insist-1.5.1/src/z3c/insist/configure.zcml
--rw-rw-r--   0 adi       (1000) adi       (1000)    17102 2023-03-23 10:52:30.000000 z3c.insist-1.5.1/src/z3c/insist/enforce.py
--rw-rw-r--   0 adi       (1000) adi       (1000)     3133 2023-03-23 10:52:30.000000 z3c.insist-1.5.1/src/z3c/insist/enftest.py
--rw-rw-r--   0 adi       (1000) adi       (1000)    27984 2023-03-23 10:52:30.000000 z3c.insist-1.5.1/src/z3c/insist/insist.py
--rw-rw-r--   0 adi       (1000) adi       (1000)     7914 2023-03-23 10:52:30.000000 z3c.insist-1.5.1/src/z3c/insist/insist.txt
--rw-rw-r--   0 adi       (1000) adi       (1000)     3211 2023-03-23 10:52:30.000000 z3c.insist-1.5.1/src/z3c/insist/interfaces.py
--rw-rw-r--   0 adi       (1000) adi       (1000)     6442 2023-03-23 10:52:30.000000 z3c.insist-1.5.1/src/z3c/insist/perftest.py
--rw-rw-r--   0 adi       (1000) adi       (1000)     1028 2023-03-23 10:52:30.000000 z3c.insist-1.5.1/src/z3c/insist/testing.py
-drwxrwxr-x   0 adi       (1000) adi       (1000)        0 2023-03-23 10:52:30.943416 z3c.insist-1.5.1/src/z3c/insist/tests/
--rw-rw-r--   0 adi       (1000) adi       (1000)       18 2023-03-23 10:52:30.000000 z3c.insist-1.5.1/src/z3c/insist/tests/__init__.py
--rw-rw-r--   0 adi       (1000) adi       (1000)    18262 2023-03-23 10:52:30.000000 z3c.insist-1.5.1/src/z3c/insist/tests/test_enforce.py
--rw-rw-r--   0 adi       (1000) adi       (1000)    39661 2023-03-23 10:52:30.000000 z3c.insist-1.5.1/src/z3c/insist/tests/test_insist.py
-drwxrwxr-x   0 adi       (1000) adi       (1000)        0 2023-03-23 10:52:30.943416 z3c.insist-1.5.1/src/z3c.insist.egg-info/
--rw-rw-r--   0 adi       (1000) adi       (1000)     4025 2023-03-23 10:52:30.000000 z3c.insist-1.5.1/src/z3c.insist.egg-info/PKG-INFO
--rw-rw-r--   0 adi       (1000) adi       (1000)      760 2023-03-23 10:52:30.000000 z3c.insist-1.5.1/src/z3c.insist.egg-info/SOURCES.txt
--rw-rw-r--   0 adi       (1000) adi       (1000)        1 2023-03-23 10:52:30.000000 z3c.insist-1.5.1/src/z3c.insist.egg-info/dependency_links.txt
--rw-rw-r--   0 adi       (1000) adi       (1000)       88 2023-03-23 10:52:30.000000 z3c.insist-1.5.1/src/z3c.insist.egg-info/entry_points.txt
--rw-rw-r--   0 adi       (1000) adi       (1000)        4 2023-03-23 10:52:30.000000 z3c.insist-1.5.1/src/z3c.insist.egg-info/namespace_packages.txt
--rw-rw-r--   0 adi       (1000) adi       (1000)        1 2023-03-23 10:52:30.000000 z3c.insist-1.5.1/src/z3c.insist.egg-info/not-zip-safe
--rw-rw-r--   0 adi       (1000) adi       (1000)      157 2023-03-23 10:52:30.000000 z3c.insist-1.5.1/src/z3c.insist.egg-info/requires.txt
--rw-rw-r--   0 adi       (1000) adi       (1000)        4 2023-03-23 10:52:30.000000 z3c.insist-1.5.1/src/z3c.insist.egg-info/top_level.txt
--rw-rw-r--   0 adi       (1000) adi       (1000)     1188 2023-03-23 10:52:30.000000 z3c.insist-1.5.1/tox.ini
+drwxrwxr-x   0 adi       (1000) adi       (1000)        0 2023-05-05 12:49:20.459462 z3c.insist-1.5.2/
+-rw-rw-r--   0 adi       (1000) adi       (1000)     2330 2023-05-05 12:49:20.000000 z3c.insist-1.5.2/CHANGES.rst
+-rw-rw-r--   0 adi       (1000) adi       (1000)     2070 2023-05-05 12:49:20.000000 z3c.insist-1.5.2/LICENSE
+-rw-rw-r--   0 adi       (1000) adi       (1000)      257 2023-05-05 12:49:20.000000 z3c.insist-1.5.2/MANIFEST.in
+-rw-rw-r--   0 adi       (1000) adi       (1000)      356 2023-05-05 12:49:20.000000 z3c.insist-1.5.2/Makefile
+-rw-rw-r--   0 adi       (1000) adi       (1000)     4171 2023-05-05 12:49:20.459462 z3c.insist-1.5.2/PKG-INFO
+-rw-rw-r--   0 adi       (1000) adi       (1000)      942 2023-05-05 12:49:20.000000 z3c.insist-1.5.2/README.rst
+-rw-rw-r--   0 adi       (1000) adi       (1000)      145 2023-05-05 12:49:20.459462 z3c.insist-1.5.2/setup.cfg
+-rw-rw-r--   0 adi       (1000) adi       (1000)     2207 2023-05-05 12:49:20.000000 z3c.insist-1.5.2/setup.py
+drwxrwxr-x   0 adi       (1000) adi       (1000)        0 2023-05-05 12:49:20.459462 z3c.insist-1.5.2/src/
+drwxrwxr-x   0 adi       (1000) adi       (1000)        0 2023-05-05 12:49:20.459462 z3c.insist-1.5.2/src/z3c/
+-rw-rw-r--   0 adi       (1000) adi       (1000)       63 2023-05-05 12:49:20.000000 z3c.insist-1.5.2/src/z3c/__init__.py
+drwxrwxr-x   0 adi       (1000) adi       (1000)        0 2023-05-05 12:49:20.459462 z3c.insist-1.5.2/src/z3c/insist/
+-rw-rw-r--   0 adi       (1000) adi       (1000)        0 2023-05-05 12:49:20.000000 z3c.insist-1.5.2/src/z3c/insist/__init__.py
+-rw-rw-r--   0 adi       (1000) adi       (1000)      760 2023-05-05 12:49:20.000000 z3c.insist-1.5.2/src/z3c/insist/configure.zcml
+-rw-rw-r--   0 adi       (1000) adi       (1000)    17613 2023-05-05 12:49:20.000000 z3c.insist-1.5.2/src/z3c/insist/enforce.py
+-rw-rw-r--   0 adi       (1000) adi       (1000)     3133 2023-05-05 12:49:20.000000 z3c.insist-1.5.2/src/z3c/insist/enftest.py
+-rw-rw-r--   0 adi       (1000) adi       (1000)    27984 2023-05-05 12:49:20.000000 z3c.insist-1.5.2/src/z3c/insist/insist.py
+-rw-rw-r--   0 adi       (1000) adi       (1000)     7914 2023-05-05 12:49:20.000000 z3c.insist-1.5.2/src/z3c/insist/insist.txt
+-rw-rw-r--   0 adi       (1000) adi       (1000)     3211 2023-05-05 12:49:20.000000 z3c.insist-1.5.2/src/z3c/insist/interfaces.py
+-rw-rw-r--   0 adi       (1000) adi       (1000)     6442 2023-05-05 12:49:20.000000 z3c.insist-1.5.2/src/z3c/insist/perftest.py
+-rw-rw-r--   0 adi       (1000) adi       (1000)     1028 2023-05-05 12:49:20.000000 z3c.insist-1.5.2/src/z3c/insist/testing.py
+drwxrwxr-x   0 adi       (1000) adi       (1000)        0 2023-05-05 12:49:20.459462 z3c.insist-1.5.2/src/z3c/insist/tests/
+-rw-rw-r--   0 adi       (1000) adi       (1000)       18 2023-05-05 12:49:20.000000 z3c.insist-1.5.2/src/z3c/insist/tests/__init__.py
+-rw-rw-r--   0 adi       (1000) adi       (1000)    18262 2023-05-05 12:49:20.000000 z3c.insist-1.5.2/src/z3c/insist/tests/test_enforce.py
+-rw-rw-r--   0 adi       (1000) adi       (1000)    39661 2023-05-05 12:49:20.000000 z3c.insist-1.5.2/src/z3c/insist/tests/test_insist.py
+drwxrwxr-x   0 adi       (1000) adi       (1000)        0 2023-05-05 12:49:20.459462 z3c.insist-1.5.2/src/z3c.insist.egg-info/
+-rw-rw-r--   0 adi       (1000) adi       (1000)     4171 2023-05-05 12:49:20.000000 z3c.insist-1.5.2/src/z3c.insist.egg-info/PKG-INFO
+-rw-rw-r--   0 adi       (1000) adi       (1000)      760 2023-05-05 12:49:20.000000 z3c.insist-1.5.2/src/z3c.insist.egg-info/SOURCES.txt
+-rw-rw-r--   0 adi       (1000) adi       (1000)        1 2023-05-05 12:49:20.000000 z3c.insist-1.5.2/src/z3c.insist.egg-info/dependency_links.txt
+-rw-rw-r--   0 adi       (1000) adi       (1000)       88 2023-05-05 12:49:20.000000 z3c.insist-1.5.2/src/z3c.insist.egg-info/entry_points.txt
+-rw-rw-r--   0 adi       (1000) adi       (1000)        4 2023-05-05 12:49:20.000000 z3c.insist-1.5.2/src/z3c.insist.egg-info/namespace_packages.txt
+-rw-rw-r--   0 adi       (1000) adi       (1000)        1 2023-05-05 12:49:20.000000 z3c.insist-1.5.2/src/z3c.insist.egg-info/not-zip-safe
+-rw-rw-r--   0 adi       (1000) adi       (1000)      164 2023-05-05 12:49:20.000000 z3c.insist-1.5.2/src/z3c.insist.egg-info/requires.txt
+-rw-rw-r--   0 adi       (1000) adi       (1000)        4 2023-05-05 12:49:20.000000 z3c.insist-1.5.2/src/z3c.insist.egg-info/top_level.txt
+-rw-rw-r--   0 adi       (1000) adi       (1000)     1188 2023-05-05 12:49:20.000000 z3c.insist-1.5.2/tox.ini
```

### Comparing `z3c.insist-1.5.1/CHANGES.rst` & `z3c.insist-1.5.2/CHANGES.rst`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,16 @@
 Changelog
 =========
 
+1.5.2 (2023-05-05)
+------------------
+
+- Ignored FileOpenedEvent in dispatch to avoid unnecessary processing of files in IncludingFilesHandler.
+
+
 1.5.1 (2023-03-23)
 ------------------
 
 - Added support for Python 3.10 and 3.11
 
 - Ignored FileOpenedEvent in dispatch to avoid unnecessary processing of files.
```

### Comparing `z3c.insist-1.5.1/LICENSE` & `z3c.insist-1.5.2/LICENSE`

 * *Files identical despite different names*

### Comparing `z3c.insist-1.5.1/PKG-INFO` & `z3c.insist-1.5.2/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: z3c.insist
-Version: 1.5.1
+Version: 1.5.2
 Summary: Persistence to ini Files
 Home-page: http://pypi.python.org/pypi/z3c.insist
 Author: Shoobx, Inc.
 Author-email: dev@shoobx.com
 License: ZPL 2.1
 Keywords: configuration dump serialization
 Classifier: License :: OSI Approved :: Zope Public License
@@ -48,14 +48,20 @@
 
 
 
 
 Changelog
 =========
 
+1.5.2 (2023-05-05)
+------------------
+
+- Ignored FileOpenedEvent in dispatch to avoid unnecessary processing of files in IncludingFilesHandler.
+
+
 1.5.1 (2023-03-23)
 ------------------
 
 - Added support for Python 3.10 and 3.11
 
 - Ignored FileOpenedEvent in dispatch to avoid unnecessary processing of files.
```

### Comparing `z3c.insist-1.5.1/README.rst` & `z3c.insist-1.5.2/README.rst`

 * *Files identical despite different names*

### Comparing `z3c.insist-1.5.1/setup.py` & `z3c.insist-1.5.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -24,15 +24,15 @@
     ]
 
 def read_file(filename):
     return open(os.path.join(os.path.dirname(__file__), filename)).read()
 
 setup(
     name="z3c.insist",
-    version='1.5.1',
+    version='1.5.2',
     author="Shoobx, Inc.",
     author_email="dev@shoobx.com",
     description="Persistence to ini Files",
     long_description=
     read_file('README.rst') +
     '\n\n' +
     read_file('CHANGES.rst'),
@@ -64,15 +64,15 @@
             'coverage',
             'python-subunit',
             'junitxml',
             'mock',
             'pytz',
             ],
         enforce=[
-            'watchdog>=3.0.0',
+            'watchdog>=3.0.0, <4.0.0',
             ],
         ),
     install_requires=INSTALL_REQUIRES,
     entry_points={
         'console_scripts': [
             'perftest = z3c.insist.perftest:main',
             'enftest = z3c.insist.enftest:main',
```

### Comparing `z3c.insist-1.5.1/src/z3c/insist/configure.zcml` & `z3c.insist-1.5.2/src/z3c/insist/configure.zcml`

 * *Files identical despite different names*

### Comparing `z3c.insist-1.5.1/src/z3c/insist/enforce.py` & `z3c.insist-1.5.2/src/z3c/insist/enforce.py`

 * *Files 1% similar despite different names*

```diff
@@ -65,15 +65,15 @@
         return event.store.getSectionFromPath(event.src_path)
 
     def dispatch(self, event):
         if event.event_type == watchdog.events.EVENT_TYPE_OPENED:
             # Do not update configuration for EVENT_TYPE_OPENED. Doing this to avoid
             # unnecessary processing on file open events, need this since watchdog
             # started sending EVENT_TYPE_OPENED events. Eventually refactor dispatch
-            # and event handlers later to do work only on specific events.
+            # and event handlers later to do work and logging only on specific events.
             return False
         ts = time.time()
         store = self.getStoreFromEvent(event)
         if store is None:
             return False
         event.store = store
         event.section = self.getSectionFromEvent(event)
@@ -225,15 +225,19 @@
                 handler.__class__.__name__)
             self.register(handler)
 
     def register(self, handler):
         self.schedule(handler, path=self.watchedDir, recursive=True)
 
     def dispatch_events(self, event_queue):
-        event, watch = event_queue.get(block=True)
+        ev =  event_queue.get(block=True)
+        if not isinstance(ev, tuple):
+            return
+        event, watch = ev
+
 
         with self._lock:
             # Optimization: Ignore all directory modified events, since we
             # cannot really do anything with those. It will also avoid
             # unnecessary transactions due to lock file action.
             if event.is_directory and \
                 event.event_type == watchdog.events.EVENT_TYPE_MODIFIED:
@@ -287,16 +291,21 @@
         ]
     case_sensitive = True
 
     def __init__(self, incObserver):
         self.incObserver = incObserver
 
     def dispatch(self, event):
-        print('-'*78)
-        print(event)
+        if event.event_type == watchdog.events.EVENT_TYPE_OPENED:
+            # Do not update configuration for EVENT_TYPE_OPENED. Doing this to avoid
+            # unnecessary processing on file open events, need this since watchdog
+            # started sending EVENT_TYPE_OPENED events. Eventually refactor dispatch
+            # and event handlers later to do work and logging only on specific events.
+            return
+        logger.info("Handling %s", event)
         if event.is_directory:
             return
 
         if match_any_paths([os.fsdecode(event.src_path)],
                            included_patterns=self.patterns,
                            excluded_patterns=self.ignore_patterns,
                            case_sensitive=self.case_sensitive):
```

### Comparing `z3c.insist-1.5.1/src/z3c/insist/enftest.py` & `z3c.insist-1.5.2/src/z3c/insist/enftest.py`

 * *Files identical despite different names*

### Comparing `z3c.insist-1.5.1/src/z3c/insist/insist.py` & `z3c.insist-1.5.2/src/z3c/insist/insist.py`

 * *Files identical despite different names*

### Comparing `z3c.insist-1.5.1/src/z3c/insist/insist.txt` & `z3c.insist-1.5.2/src/z3c/insist/insist.txt`

 * *Files identical despite different names*

### Comparing `z3c.insist-1.5.1/src/z3c/insist/interfaces.py` & `z3c.insist-1.5.2/src/z3c/insist/interfaces.py`

 * *Files identical despite different names*

### Comparing `z3c.insist-1.5.1/src/z3c/insist/perftest.py` & `z3c.insist-1.5.2/src/z3c/insist/perftest.py`

 * *Files identical despite different names*

### Comparing `z3c.insist-1.5.1/src/z3c/insist/testing.py` & `z3c.insist-1.5.2/src/z3c/insist/testing.py`

 * *Files identical despite different names*

### Comparing `z3c.insist-1.5.1/src/z3c/insist/tests/test_enforce.py` & `z3c.insist-1.5.2/src/z3c/insist/tests/test_enforce.py`

 * *Files identical despite different names*

### Comparing `z3c.insist-1.5.1/src/z3c/insist/tests/test_insist.py` & `z3c.insist-1.5.2/src/z3c/insist/tests/test_insist.py`

 * *Files identical despite different names*

### Comparing `z3c.insist-1.5.1/src/z3c.insist.egg-info/PKG-INFO` & `z3c.insist-1.5.2/src/z3c.insist.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: z3c.insist
-Version: 1.5.1
+Version: 1.5.2
 Summary: Persistence to ini Files
 Home-page: http://pypi.python.org/pypi/z3c.insist
 Author: Shoobx, Inc.
 Author-email: dev@shoobx.com
 License: ZPL 2.1
 Keywords: configuration dump serialization
 Classifier: License :: OSI Approved :: Zope Public License
@@ -48,14 +48,20 @@
 
 
 
 
 Changelog
 =========
 
+1.5.2 (2023-05-05)
+------------------
+
+- Ignored FileOpenedEvent in dispatch to avoid unnecessary processing of files in IncludingFilesHandler.
+
+
 1.5.1 (2023-03-23)
 ------------------
 
 - Added support for Python 3.10 and 3.11
 
 - Ignored FileOpenedEvent in dispatch to avoid unnecessary processing of files.
```

### Comparing `z3c.insist-1.5.1/src/z3c.insist.egg-info/SOURCES.txt` & `z3c.insist-1.5.2/src/z3c.insist.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `z3c.insist-1.5.1/tox.ini` & `z3c.insist-1.5.2/tox.ini`

 * *Files identical despite different names*

