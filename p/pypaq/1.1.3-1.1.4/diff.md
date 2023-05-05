# Comparing `tmp/pypaq-1.1.3.tar.gz` & `tmp/pypaq-1.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pypaq-1.1.3.tar", last modified: Tue Apr 11 18:16:45 2023, max compression
+gzip compressed data, was "dist/pypaq-1.1.4.tar", last modified: Fri May  5 19:19:58 2023, max compression
```

## Comparing `pypaq-1.1.3.tar` & `pypaq-1.1.4.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxrwxr-x   0 pniewinski  (1000) pniewinski  (1000)        0 2023-04-11 18:16:45.000000 pypaq-1.1.3/
--rw-rw-r--   0 pniewinski  (1000) pniewinski  (1000)      200 2023-04-11 18:16:45.000000 pypaq-1.1.3/PKG-INFO
--rw-rw-r--   0 pniewinski  (1000) pniewinski  (1000)      538 2023-03-05 14:20:43.000000 pypaq-1.1.3/README.md
-drwxrwxr-x   0 pniewinski  (1000) pniewinski  (1000)        0 2023-04-11 18:16:45.000000 pypaq-1.1.3/pypaq/
--rw-rw-r--   0 pniewinski  (1000) pniewinski  (1000)        0 2023-02-27 23:13:46.000000 pypaq-1.1.3/pypaq/__init__.py
--rw-rw-r--   0 pniewinski  (1000) pniewinski  (1000)       41 2023-03-09 20:19:41.000000 pypaq-1.1.3/pypaq/exception.py
-drwxrwxr-x   0 pniewinski  (1000) pniewinski  (1000)        0 2023-04-11 18:16:45.000000 pypaq-1.1.3/pypaq/lipytools/
--rw-rw-r--   0 pniewinski  (1000) pniewinski  (1000)        0 2023-02-27 23:13:46.000000 pypaq-1.1.3/pypaq/lipytools/__init__.py
--rwxrwxr-x   0 pniewinski  (1000) pniewinski  (1000)     4111 2023-03-10 11:50:02.000000 pypaq-1.1.3/pypaq/lipytools/decorators.py
--rw-rw-r--   0 pniewinski  (1000) pniewinski  (1000)      826 2023-03-24 23:09:04.000000 pypaq-1.1.3/pypaq/lipytools/double_hinge.py
--rw-rw-r--   0 pniewinski  (1000) pniewinski  (1000)     3559 2023-03-20 19:23:47.000000 pypaq-1.1.3/pypaq/lipytools/files.py
--rw-rw-r--   0 pniewinski  (1000) pniewinski  (1000)     1173 2023-03-09 20:19:41.000000 pypaq-1.1.3/pypaq/lipytools/moving_average.py
--rwxrwxr-x   0 pniewinski  (1000) pniewinski  (1000)     4954 2023-03-20 14:10:43.000000 pypaq-1.1.3/pypaq/lipytools/plots.py
--rwxrwxr-x   0 pniewinski  (1000) pniewinski  (1000)     2995 2023-03-18 14:06:25.000000 pypaq-1.1.3/pypaq/lipytools/printout.py
--rw-rw-r--   0 pniewinski  (1000) pniewinski  (1000)     1750 2023-03-26 12:28:29.000000 pypaq-1.1.3/pypaq/lipytools/pylogger.py
--rw-rw-r--   0 pniewinski  (1000) pniewinski  (1000)       73 2023-02-27 23:13:46.000000 pypaq-1.1.3/pypaq/lipytools/softmax.py
--rwxrwxr-x   0 pniewinski  (1000) pniewinski  (1000)      977 2023-03-26 08:26:06.000000 pypaq-1.1.3/pypaq/lipytools/stats.py
-drwxrwxr-x   0 pniewinski  (1000) pniewinski  (1000)        0 2023-04-11 18:16:45.000000 pypaq-1.1.3/pypaq/mpython/
--rw-rw-r--   0 pniewinski  (1000) pniewinski  (1000)        0 2023-02-27 23:13:46.000000 pypaq-1.1.3/pypaq/mpython/__init__.py
--rw-rw-r--   0 pniewinski  (1000) pniewinski  (1000)     5927 2023-04-11 17:27:08.000000 pypaq-1.1.3/pypaq/mpython/devices.py
--rwxrwxr-x   0 pniewinski  (1000) pniewinski  (1000)     1563 2023-02-28 16:27:57.000000 pypaq-1.1.3/pypaq/mpython/mpdecor.py
--rw-rw-r--   0 pniewinski  (1000) pniewinski  (1000)     5315 2023-03-27 15:53:38.000000 pypaq-1.1.3/pypaq/mpython/mptools.py
-drwxrwxr-x   0 pniewinski  (1000) pniewinski  (1000)        0 2023-04-11 18:16:45.000000 pypaq-1.1.3/pypaq/pms/
--rw-rw-r--   0 pniewinski  (1000) pniewinski  (1000)        0 2023-02-27 23:13:46.000000 pypaq-1.1.3/pypaq/pms/__init__.py
--rw-rw-r--   0 pniewinski  (1000) pniewinski  (1000)     2939 2023-03-20 19:29:23.000000 pypaq-1.1.3/pypaq/pms/base.py
--rw-rw-r--   0 pniewinski  (1000) pniewinski  (1000)     2609 2023-03-11 12:18:25.000000 pypaq-1.1.3/pypaq/pms/config_manager.py
--rwxrwxr-x   0 pniewinski  (1000) pniewinski  (1000)    11938 2023-03-09 20:43:48.000000 pypaq-1.1.3/pypaq/pms/parasave.py
--rwxrwxr-x   0 pniewinski  (1000) pniewinski  (1000)    18475 2023-04-02 18:34:58.000000 pypaq-1.1.3/pypaq/pms/paspa.py
--rw-rw-r--   0 pniewinski  (1000) pniewinski  (1000)     7749 2023-03-24 18:14:54.000000 pypaq-1.1.3/pypaq/pms/subscriptable.py
--rw-rw-r--   0 pniewinski  (1000) pniewinski  (1000)      152 2023-03-31 21:11:22.000000 pypaq-1.1.3/pypaq/pytypes.py
-drwxrwxr-x   0 pniewinski  (1000) pniewinski  (1000)        0 2023-04-11 18:16:45.000000 pypaq-1.1.3/pypaq/textools/
--rw-rw-r--   0 pniewinski  (1000) pniewinski  (1000)        0 2023-02-27 23:13:46.000000 pypaq-1.1.3/pypaq/textools/__init__.py
--rwxrwxr-x   0 pniewinski  (1000) pniewinski  (1000)     1210 2023-02-27 23:13:46.000000 pypaq-1.1.3/pypaq/textools/text_metrics.py
--rw-rw-r--   0 pniewinski  (1000) pniewinski  (1000)      586 2023-02-27 23:13:46.000000 pypaq-1.1.3/pypaq/textools/text_processing.py
-drwxrwxr-x   0 pniewinski  (1000) pniewinski  (1000)        0 2023-04-11 18:16:45.000000 pypaq-1.1.3/pypaq.egg-info/
--rw-rw-r--   0 pniewinski  (1000) pniewinski  (1000)      200 2023-04-11 18:16:45.000000 pypaq-1.1.3/pypaq.egg-info/PKG-INFO
--rw-rw-r--   0 pniewinski  (1000) pniewinski  (1000)      827 2023-04-11 18:16:45.000000 pypaq-1.1.3/pypaq.egg-info/SOURCES.txt
--rw-rw-r--   0 pniewinski  (1000) pniewinski  (1000)        1 2023-04-11 18:16:45.000000 pypaq-1.1.3/pypaq.egg-info/dependency_links.txt
--rw-rw-r--   0 pniewinski  (1000) pniewinski  (1000)       89 2023-04-11 18:16:45.000000 pypaq-1.1.3/pypaq.egg-info/requires.txt
--rw-rw-r--   0 pniewinski  (1000) pniewinski  (1000)        6 2023-04-11 18:16:45.000000 pypaq-1.1.3/pypaq.egg-info/top_level.txt
--rw-rw-r--   0 pniewinski  (1000) pniewinski  (1000)       38 2023-04-11 18:16:45.000000 pypaq-1.1.3/setup.cfg
--rw-rw-r--   0 pniewinski  (1000) pniewinski  (1000)      622 2023-04-11 18:16:12.000000 pypaq-1.1.3/setup.py
+drwxrwxr-x   0 pniewinski  (1000) pniewinski  (1000)        0 2023-05-05 19:19:58.000000 pypaq-1.1.4/
+-rw-rw-r--   0 pniewinski  (1000) pniewinski  (1000)      200 2023-05-05 19:19:58.000000 pypaq-1.1.4/PKG-INFO
+-rw-rw-r--   0 pniewinski  (1000) pniewinski  (1000)      538 2023-03-05 14:20:43.000000 pypaq-1.1.4/README.md
+drwxrwxr-x   0 pniewinski  (1000) pniewinski  (1000)        0 2023-05-05 19:19:58.000000 pypaq-1.1.4/pypaq/
+-rw-rw-r--   0 pniewinski  (1000) pniewinski  (1000)        0 2023-02-27 23:13:46.000000 pypaq-1.1.4/pypaq/__init__.py
+-rw-rw-r--   0 pniewinski  (1000) pniewinski  (1000)       41 2023-03-09 20:19:41.000000 pypaq-1.1.4/pypaq/exception.py
+drwxrwxr-x   0 pniewinski  (1000) pniewinski  (1000)        0 2023-05-05 19:19:58.000000 pypaq-1.1.4/pypaq/lipytools/
+-rw-rw-r--   0 pniewinski  (1000) pniewinski  (1000)        0 2023-02-27 23:13:46.000000 pypaq-1.1.4/pypaq/lipytools/__init__.py
+-rwxrwxr-x   0 pniewinski  (1000) pniewinski  (1000)     4111 2023-03-10 11:50:02.000000 pypaq-1.1.4/pypaq/lipytools/decorators.py
+-rw-rw-r--   0 pniewinski  (1000) pniewinski  (1000)      826 2023-03-24 23:09:04.000000 pypaq-1.1.4/pypaq/lipytools/double_hinge.py
+-rw-rw-r--   0 pniewinski  (1000) pniewinski  (1000)     3559 2023-03-20 19:23:47.000000 pypaq-1.1.4/pypaq/lipytools/files.py
+-rw-rw-r--   0 pniewinski  (1000) pniewinski  (1000)     1173 2023-03-09 20:19:41.000000 pypaq-1.1.4/pypaq/lipytools/moving_average.py
+-rwxrwxr-x   0 pniewinski  (1000) pniewinski  (1000)     4954 2023-03-20 14:10:43.000000 pypaq-1.1.4/pypaq/lipytools/plots.py
+-rwxrwxr-x   0 pniewinski  (1000) pniewinski  (1000)     2995 2023-03-18 14:06:25.000000 pypaq-1.1.4/pypaq/lipytools/printout.py
+-rw-rw-r--   0 pniewinski  (1000) pniewinski  (1000)     1750 2023-03-26 12:28:29.000000 pypaq-1.1.4/pypaq/lipytools/pylogger.py
+-rw-rw-r--   0 pniewinski  (1000) pniewinski  (1000)       73 2023-02-27 23:13:46.000000 pypaq-1.1.4/pypaq/lipytools/softmax.py
+-rwxrwxr-x   0 pniewinski  (1000) pniewinski  (1000)      977 2023-03-26 08:26:06.000000 pypaq-1.1.4/pypaq/lipytools/stats.py
+drwxrwxr-x   0 pniewinski  (1000) pniewinski  (1000)        0 2023-05-05 19:19:58.000000 pypaq-1.1.4/pypaq/mpython/
+-rw-rw-r--   0 pniewinski  (1000) pniewinski  (1000)        0 2023-02-27 23:13:46.000000 pypaq-1.1.4/pypaq/mpython/__init__.py
+-rw-rw-r--   0 pniewinski  (1000) pniewinski  (1000)     5927 2023-04-11 17:27:08.000000 pypaq-1.1.4/pypaq/mpython/devices.py
+-rwxrwxr-x   0 pniewinski  (1000) pniewinski  (1000)     1551 2023-04-24 12:36:21.000000 pypaq-1.1.4/pypaq/mpython/mpdecor.py
+-rw-rw-r--   0 pniewinski  (1000) pniewinski  (1000)     5353 2023-04-12 20:01:16.000000 pypaq-1.1.4/pypaq/mpython/mptools.py
+drwxrwxr-x   0 pniewinski  (1000) pniewinski  (1000)        0 2023-05-05 19:19:58.000000 pypaq-1.1.4/pypaq/pms/
+-rw-rw-r--   0 pniewinski  (1000) pniewinski  (1000)        0 2023-02-27 23:13:46.000000 pypaq-1.1.4/pypaq/pms/__init__.py
+-rw-rw-r--   0 pniewinski  (1000) pniewinski  (1000)     2939 2023-03-20 19:29:23.000000 pypaq-1.1.4/pypaq/pms/base.py
+-rw-rw-r--   0 pniewinski  (1000) pniewinski  (1000)     2566 2023-04-30 09:55:40.000000 pypaq-1.1.4/pypaq/pms/config_manager.py
+-rwxrwxr-x   0 pniewinski  (1000) pniewinski  (1000)    11923 2023-05-02 16:04:06.000000 pypaq-1.1.4/pypaq/pms/parasave.py
+-rwxrwxr-x   0 pniewinski  (1000) pniewinski  (1000)    18475 2023-04-02 18:34:58.000000 pypaq-1.1.4/pypaq/pms/paspa.py
+-rw-rw-r--   0 pniewinski  (1000) pniewinski  (1000)     8550 2023-04-24 18:34:30.000000 pypaq-1.1.4/pypaq/pms/subscriptable.py
+-rw-rw-r--   0 pniewinski  (1000) pniewinski  (1000)      152 2023-03-31 21:11:22.000000 pypaq-1.1.4/pypaq/pytypes.py
+drwxrwxr-x   0 pniewinski  (1000) pniewinski  (1000)        0 2023-05-05 19:19:58.000000 pypaq-1.1.4/pypaq/textools/
+-rw-rw-r--   0 pniewinski  (1000) pniewinski  (1000)        0 2023-02-27 23:13:46.000000 pypaq-1.1.4/pypaq/textools/__init__.py
+-rwxrwxr-x   0 pniewinski  (1000) pniewinski  (1000)     1210 2023-02-27 23:13:46.000000 pypaq-1.1.4/pypaq/textools/text_metrics.py
+-rw-rw-r--   0 pniewinski  (1000) pniewinski  (1000)      586 2023-02-27 23:13:46.000000 pypaq-1.1.4/pypaq/textools/text_processing.py
+drwxrwxr-x   0 pniewinski  (1000) pniewinski  (1000)        0 2023-05-05 19:19:58.000000 pypaq-1.1.4/pypaq.egg-info/
+-rw-rw-r--   0 pniewinski  (1000) pniewinski  (1000)      200 2023-05-05 19:19:58.000000 pypaq-1.1.4/pypaq.egg-info/PKG-INFO
+-rw-rw-r--   0 pniewinski  (1000) pniewinski  (1000)      827 2023-05-05 19:19:58.000000 pypaq-1.1.4/pypaq.egg-info/SOURCES.txt
+-rw-rw-r--   0 pniewinski  (1000) pniewinski  (1000)        1 2023-05-05 19:19:58.000000 pypaq-1.1.4/pypaq.egg-info/dependency_links.txt
+-rw-rw-r--   0 pniewinski  (1000) pniewinski  (1000)       89 2023-05-05 19:19:58.000000 pypaq-1.1.4/pypaq.egg-info/requires.txt
+-rw-rw-r--   0 pniewinski  (1000) pniewinski  (1000)        6 2023-05-05 19:19:58.000000 pypaq-1.1.4/pypaq.egg-info/top_level.txt
+-rw-rw-r--   0 pniewinski  (1000) pniewinski  (1000)       38 2023-05-05 19:19:58.000000 pypaq-1.1.4/setup.cfg
+-rw-rw-r--   0 pniewinski  (1000) pniewinski  (1000)      622 2023-05-05 19:19:17.000000 pypaq-1.1.4/setup.py
```

### Comparing `pypaq-1.1.3/README.md` & `pypaq-1.1.4/README.md`

 * *Files identical despite different names*

### Comparing `pypaq-1.1.3/pypaq/lipytools/decorators.py` & `pypaq-1.1.4/pypaq/lipytools/decorators.py`

 * *Files identical despite different names*

### Comparing `pypaq-1.1.3/pypaq/lipytools/double_hinge.py` & `pypaq-1.1.4/pypaq/lipytools/double_hinge.py`

 * *Files identical despite different names*

### Comparing `pypaq-1.1.3/pypaq/lipytools/files.py` & `pypaq-1.1.4/pypaq/lipytools/files.py`

 * *Files identical despite different names*

### Comparing `pypaq-1.1.3/pypaq/lipytools/moving_average.py` & `pypaq-1.1.4/pypaq/lipytools/moving_average.py`

 * *Files identical despite different names*

### Comparing `pypaq-1.1.3/pypaq/lipytools/plots.py` & `pypaq-1.1.4/pypaq/lipytools/plots.py`

 * *Files identical despite different names*

### Comparing `pypaq-1.1.3/pypaq/lipytools/printout.py` & `pypaq-1.1.4/pypaq/lipytools/printout.py`

 * *Files identical despite different names*

### Comparing `pypaq-1.1.3/pypaq/lipytools/pylogger.py` & `pypaq-1.1.4/pypaq/lipytools/pylogger.py`

 * *Files identical despite different names*

### Comparing `pypaq-1.1.3/pypaq/lipytools/stats.py` & `pypaq-1.1.4/pypaq/lipytools/stats.py`

 * *Files identical despite different names*

### Comparing `pypaq-1.1.3/pypaq/mpython/devices.py` & `pypaq-1.1.4/pypaq/mpython/devices.py`

 * *Files identical despite different names*

### Comparing `pypaq-1.1.3/pypaq/mpython/mpdecor.py` & `pypaq-1.1.4/pypaq/mpython/mpdecor.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 from multiprocessing import Process, Queue
 from functools import partial
-import time
 
 
 # non-blocking process, does not return anything
 def proc(f):
 
     def new_f(*args, **kwargs):
         Process(target=partial(f, *args, **kwargs)).start()
```

### Comparing `pypaq-1.1.3/pypaq/mpython/mptools.py` & `pypaq-1.1.4/pypaq/mpython/mptools.py`

 * *Files 2% similar despite different names*

```diff
@@ -70,16 +70,16 @@
 
 
 # Exception Managed Subprocess - with basic exceptions management
 class ExSubprocess(Process, ABC):
 
     def __init__(
             self,
-            ique: Que,                          # input que
-            oque: Que,                          # output que
+            ique: Optional[Que]=        None,   # input que
+            oque: Optional[Que]=        None,   # output que
             id: Optional[int or str]=   None,   # unique id to identify the subprocess, if not given takes from Process name
             raise_unk_exception=        True,   # raises exception other than KeyboardInterrupt
             logger=                     None,
             loglevel=                   30):
 
         ABC.__init__(self)
         Process.__init__(self, target=self.__run)
@@ -118,15 +118,16 @@
     def subprocess_method(self): pass
 
     # when exception occurs, message with exception data is put on the output que
     def __exception_handle(self, name:str):
         msg = QMessage(
             type=   f'ex_{name}, ExSubprocess id: {self.id}, pid: {self.pid}',
             data=   self.id) # returns ID here to allow process identification
-        self.oque.put(msg)
+        if self.oque is not None:
+            self.oque.put(msg)
         self.logger.warning(f'> ExSubprocess ({self.id}) halted by exception: {name}')
         self.after_exception_handle_run()
 
     # this method may be implemented and will be run after exception occurred
     def after_exception_handle_run(self): pass
 
     def kill(self):
```

### Comparing `pypaq-1.1.3/pypaq/pms/base.py` & `pypaq-1.1.4/pypaq/pms/base.py`

 * *Files identical despite different names*

### Comparing `pypaq-1.1.3/pypaq/pms/parasave.py` & `pypaq-1.1.4/pypaq/pms/parasave.py`

 * *Files 0% similar despite different names*

```diff
@@ -162,15 +162,15 @@
         with open(txt_FN, 'w') as file:
             s = f' *** ParaSave POINT saved: {stamp(year=True, letters=None)} ***\n'
             s += ParaSave.dict_2str(point)
             file.write(s)
 
         self.__log.debug(f'{self.__class__.__name__} {self.name} saved to {self.save_topdir}')
 
-    # loads, next overrides parameters from given kwargs and saves new ParaSave POINT
+    # loads, next overrides parameters from given kwargs and saves POINT
     @classmethod
     def oversave_point(
             cls,
             name: str,
             save_topdir: Optional[str]= None,
             save_fn_pfx: Optional[str]= None,
             **kwargs):
@@ -252,18 +252,20 @@
             save_fn_pfx=    save_fn_pfx,
             logger=         logger,
             loglevel=       loglevel) if name_parent_scnd else None
 
         not_gxable_parents = []
         if not pm['gxable']: not_gxable_parents.append(pm)
         if ps and not ps['gxable']: not_gxable_parents.append(ps)
+
         if not_gxable_parents:
             raise ParaSaveException('not gxable parents, cannot GX!')
+
+        # make pm a child and save
         else:
-            # make pm a child and save
             point_child = SubGX.gx_point(
                 parent_main=    pm,
                 parent_scnd=    ps,
                 name_child=     name_child)
             pm.update(point_child)
             pm['_save_topdir'] = save_topdir_child
             pm.parents = [name_parent_main]
```

### Comparing `pypaq-1.1.3/pypaq/pms/paspa.py` & `pypaq-1.1.4/pypaq/pms/paspa.py`

 * *Files identical despite different names*

### Comparing `pypaq-1.1.3/pypaq/pms/subscriptable.py` & `pypaq-1.1.4/pypaq/pms/subscriptable.py`

 * *Files 14% similar despite different names*

```diff
@@ -2,30 +2,64 @@
 from typing import List, Optional, Union, Dict, Set, Tuple
 
 from pypaq.textools.text_metrics import lev_dist
 from pypaq.pms.base import POINT, PSDD, PMSException
 from pypaq.pms.paspa import PaSpa
 
 
+# returns nice str information about dict differences: db against da
+def dict_diff(da:Dict, db:Dict) -> str:
+
+    nfo = ''
+
+    missing_keys = []
+    for k in da:
+        if k not in db:
+            missing_keys.append(k)
+
+    if missing_keys:
+        nfo += f'missing keys: {missing_keys}\n'
+
+    new_keys = []
+    new_values = []
+    for k in db:
+        if k not in da:
+            new_keys.append(k)
+        else:
+            if da[k] != db[k]:
+                new_values.append(k)
+
+    if new_keys:
+        nfo += f'new keys: {new_keys}\n'
+        for k in new_keys:
+            nfo += f' > {k}: {db[k]}\n'
+
+    if new_values:
+        nfo += f'new values: {new_values}\n'
+        for k in new_values:
+            nfo += f' > {k}: {db[k]}\n'
+
+    if nfo: nfo = nfo[:-1]
+    return nfo
+
+
 # implements dict-like style access to its (self) parameters
 class Subscriptable:
     """
     Subscriptable
         its (object) parameters (POINT) may be accessed in dict-like style [], but are IS NOT a dict type
         protected fields may also be accessed with [], but rather should not
     """
 
     def __getitem__(self, key):
         return getattr(self, key)
 
-
     def __setitem__(self, key, value):
         setattr(self, key, value)
 
-
     def __contains__(self, key):
         return key in vars(self)
 
     # ********************************************************************************************************** getters
 
     # returns list of all object fields
     def get_all_fields(self, protected=False) -> List[str]:
@@ -74,18 +108,19 @@
 
         return found or None
 
 
     def __str__(self):
         s = f'{self.__class__.__name__} (Subscriptable):\n'
         pms = self.get_point()
-        for k in sorted(pms.keys()):
-            p = f'param: {k}'
-            v = f'value: {pms[k]}'
-            s += f'{p:30s} {v:30s}\n'
+        if pms:
+            for k in sorted(pms.keys()):
+                s += f' > {k:30s}: {pms[k]}\n'
+        else:
+            s += f'---empty---\n'
         return s[:-1]
 
 
 # extends Subscriptable with GX on POINT
 class SubGX(Subscriptable):
     """
     SubGX - Subscriptable with GX (genetic crossing algorithm)
```

### Comparing `pypaq-1.1.3/pypaq/textools/text_metrics.py` & `pypaq-1.1.4/pypaq/textools/text_metrics.py`

 * *Files identical despite different names*

### Comparing `pypaq-1.1.3/pypaq/textools/text_processing.py` & `pypaq-1.1.4/pypaq/textools/text_processing.py`

 * *Files identical despite different names*

### Comparing `pypaq-1.1.3/pypaq.egg-info/SOURCES.txt` & `pypaq-1.1.4/pypaq.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pypaq-1.1.3/setup.py` & `pypaq-1.1.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
     with open('requirements.txt') as file:
         lines = [l[:-1] if l[-1]=='\n' else l for l in file.readlines()]
         return lines
 
 
 setup(
     name=               'pypaq',
-    version=            'v1.1.3',
+    version=            'v1.1.4',
     url=                'https://github.com/piteren/pypaq.git',
     author=             'Piotr Niewinski',
     author_email=       'pioniewinski@gmail.com',
     description=        'little python tools',
     packages=           find_packages(),
     install_requires=   get_requirements(),
     license=            'MIT')
```

