# Comparing `tmp/regtest-0.3.2.zip` & `tmp/regtest-0.3.3.zip`

## zipinfo {}

```diff
@@ -1,19 +1,19 @@
-Zip file size: 13506 bytes, number of entries: 17
-drwxr-xr-x  2.0 unx        0 b- stor 23-May-05 10:51 regtest-0.3.2/
-drwxr-xr-x  2.0 unx        0 b- stor 23-May-05 10:51 regtest-0.3.2/regtest.egg-info/
-drwxr-xr-x  2.0 unx        0 b- stor 23-May-05 10:51 regtest-0.3.2/regtest/
--rw-r--r--  2.0 unx     2924 b- defN 23-May-05 10:51 regtest-0.3.2/PKG-INFO
--rw-r--r--  2.0 unx    11357 b- defN 17-Jul-29 12:58 regtest-0.3.2/LICENSE
--rwxr--r--  2.0 unx       43 b- defN 19-Sep-12 12:23 regtest-0.3.2/MANIFEST.in
--rw-r--r--  2.0 unx     1685 b- defN 21-Oct-07 10:13 regtest-0.3.2/setup.py
--rw-r--r--  2.0 unx       38 b- defN 23-May-05 10:51 regtest-0.3.2/setup.cfg
--rw-r--r--  2.0 unx     1925 b- defN 23-May-05 09:09 regtest-0.3.2/README.rst
--rw-r--r--  2.0 unx      833 b- defN 23-May-05 10:48 regtest-0.3.2/CHANGES.rst
--rw-r--r--  2.0 unx     2186 b- defN 21-Nov-21 12:45 regtest-0.3.2/HOWTO.rst
--rw-r--r--  2.0 unx     2924 b- defN 23-May-05 10:51 regtest-0.3.2/regtest.egg-info/PKG-INFO
--rw-r--r--  2.0 unx      224 b- defN 23-May-05 10:51 regtest-0.3.2/regtest.egg-info/SOURCES.txt
--rw-r--r--  2.0 unx        8 b- defN 23-May-05 10:51 regtest-0.3.2/regtest.egg-info/top_level.txt
--rw-r--r--  2.0 unx        1 b- defN 23-May-05 10:51 regtest-0.3.2/regtest.egg-info/dependency_links.txt
--rw-r--r--  2.0 unx     6329 b- defN 23-May-05 10:46 regtest-0.3.2/regtest/regtest.py
--rw-r--r--  2.0 unx      979 b- defN 23-May-05 10:47 regtest-0.3.2/regtest/__init__.py
-17 files, 31456 bytes uncompressed, 11206 bytes compressed:  64.4%
+Zip file size: 13508 bytes, number of entries: 17
+drwxr-xr-x  2.0 unx        0 b- stor 23-May-05 10:59 regtest-0.3.3/
+drwxr-xr-x  2.0 unx        0 b- stor 23-May-05 10:59 regtest-0.3.3/regtest.egg-info/
+drwxr-xr-x  2.0 unx        0 b- stor 23-May-05 10:59 regtest-0.3.3/regtest/
+-rw-r--r--  2.0 unx     2924 b- defN 23-May-05 10:59 regtest-0.3.3/PKG-INFO
+-rw-r--r--  2.0 unx    11357 b- defN 17-Jul-29 12:58 regtest-0.3.3/LICENSE
+-rwxr--r--  2.0 unx       43 b- defN 19-Sep-12 12:23 regtest-0.3.3/MANIFEST.in
+-rw-r--r--  2.0 unx     1685 b- defN 21-Oct-07 10:13 regtest-0.3.3/setup.py
+-rw-r--r--  2.0 unx       38 b- defN 23-May-05 10:59 regtest-0.3.3/setup.cfg
+-rw-r--r--  2.0 unx     1925 b- defN 23-May-05 09:09 regtest-0.3.3/README.rst
+-rw-r--r--  2.0 unx      962 b- defN 23-May-05 10:55 regtest-0.3.3/CHANGES.rst
+-rw-r--r--  2.0 unx     2186 b- defN 21-Nov-21 12:45 regtest-0.3.3/HOWTO.rst
+-rw-r--r--  2.0 unx     2924 b- defN 23-May-05 10:59 regtest-0.3.3/regtest.egg-info/PKG-INFO
+-rw-r--r--  2.0 unx      224 b- defN 23-May-05 10:59 regtest-0.3.3/regtest.egg-info/SOURCES.txt
+-rw-r--r--  2.0 unx        8 b- defN 23-May-05 10:59 regtest-0.3.3/regtest.egg-info/top_level.txt
+-rw-r--r--  2.0 unx        1 b- defN 23-May-05 10:59 regtest-0.3.3/regtest.egg-info/dependency_links.txt
+-rw-r--r--  2.0 unx     6336 b- defN 23-May-05 10:57 regtest-0.3.3/regtest/regtest.py
+-rw-r--r--  2.0 unx      974 b- defN 23-May-05 10:57 regtest-0.3.3/regtest/__init__.py
+17 files, 31587 bytes uncompressed, 11208 bytes compressed:  64.5%
```

## zipnote {}

```diff
@@ -1,52 +1,52 @@
-Filename: regtest-0.3.2/
+Filename: regtest-0.3.3/
 Comment: 
 
-Filename: regtest-0.3.2/regtest.egg-info/
+Filename: regtest-0.3.3/regtest.egg-info/
 Comment: 
 
-Filename: regtest-0.3.2/regtest/
+Filename: regtest-0.3.3/regtest/
 Comment: 
 
-Filename: regtest-0.3.2/PKG-INFO
+Filename: regtest-0.3.3/PKG-INFO
 Comment: 
 
-Filename: regtest-0.3.2/LICENSE
+Filename: regtest-0.3.3/LICENSE
 Comment: 
 
-Filename: regtest-0.3.2/MANIFEST.in
+Filename: regtest-0.3.3/MANIFEST.in
 Comment: 
 
-Filename: regtest-0.3.2/setup.py
+Filename: regtest-0.3.3/setup.py
 Comment: 
 
-Filename: regtest-0.3.2/setup.cfg
+Filename: regtest-0.3.3/setup.cfg
 Comment: 
 
-Filename: regtest-0.3.2/README.rst
+Filename: regtest-0.3.3/README.rst
 Comment: 
 
-Filename: regtest-0.3.2/CHANGES.rst
+Filename: regtest-0.3.3/CHANGES.rst
 Comment: 
 
-Filename: regtest-0.3.2/HOWTO.rst
+Filename: regtest-0.3.3/HOWTO.rst
 Comment: 
 
-Filename: regtest-0.3.2/regtest.egg-info/PKG-INFO
+Filename: regtest-0.3.3/regtest.egg-info/PKG-INFO
 Comment: 
 
-Filename: regtest-0.3.2/regtest.egg-info/SOURCES.txt
+Filename: regtest-0.3.3/regtest.egg-info/SOURCES.txt
 Comment: 
 
-Filename: regtest-0.3.2/regtest.egg-info/top_level.txt
+Filename: regtest-0.3.3/regtest.egg-info/top_level.txt
 Comment: 
 
-Filename: regtest-0.3.2/regtest.egg-info/dependency_links.txt
+Filename: regtest-0.3.3/regtest.egg-info/dependency_links.txt
 Comment: 
 
-Filename: regtest-0.3.2/regtest/regtest.py
+Filename: regtest-0.3.3/regtest/regtest.py
 Comment: 
 
-Filename: regtest-0.3.2/regtest/__init__.py
+Filename: regtest-0.3.3/regtest/__init__.py
 Comment: 
 
 Zip file comment:
```

## Comparing `regtest-0.3.2/PKG-INFO` & `regtest-0.3.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: regtest
-Version: 0.3.2
+Version: 0.3.3
 Summary: regression test enhancement for the Python unittest framework.
 Home-page: https://github.com/sonntagsgesicht/regtest
 Author: sonntagsgesicht
 Author-email: sonntagsgesicht@icloud.com
 License: Apache License 2.0
 Platform: any
 Classifier: Development Status :: 4 - Beta
```

## Comparing `regtest-0.3.2/LICENSE` & `regtest-0.3.3/LICENSE`

 * *Files identical despite different names*

## Comparing `regtest-0.3.2/setup.py` & `regtest-0.3.3/setup.py`

 * *Files identical despite different names*

## Comparing `regtest-0.3.2/README.rst` & `regtest-0.3.3/README.rst`

 * *Files identical despite different names*

## Comparing `regtest-0.3.2/HOWTO.rst` & `regtest-0.3.3/HOWTO.rst`

 * *Files identical despite different names*

## Comparing `regtest-0.3.2/regtest.egg-info/PKG-INFO` & `regtest-0.3.3/regtest.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: regtest
-Version: 0.3.2
+Version: 0.3.3
 Summary: regression test enhancement for the Python unittest framework.
 Home-page: https://github.com/sonntagsgesicht/regtest
 Author: sonntagsgesicht
 Author-email: sonntagsgesicht@icloud.com
 License: Apache License 2.0
 Platform: any
 Classifier: Development Status :: 4 - Beta
```

## Comparing `regtest-0.3.2/regtest/regtest.py` & `regtest-0.3.3/regtest/regtest.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # -*- coding: utf-8 -*-
 
 # regtest
 # -------
 # regression test enhancement for the Python unittest framework.
 #
 # Author:   sonntagsgesicht
-# Version:  0.3.1, copyright Sunday, 21 November 2021
+# Version:  0.3.3, copyright Friday, 05 May 2023
 # Website:  https://github.com/sonntagsgesicht/regtest
 # License:  Apache License 2.0 (see LICENSE file)
 
 
 from inspect import stack
 from json import load, dump, loads, dumps
 from logging import getLogger, NullHandler
@@ -116,15 +116,15 @@
                     msg = ''
                 with self.open(test_method, 'wt') as file:
                     dump(data, file, indent=2)
 
     def assertAlmostRegressiveEqual(
             self, new, places=7, msg=None, delta=None, key=()):
         # version 0.3.1, fixing tuple as list issue 'loads(dumps(tuple))=list'
-        if isinstance(new, (tuple, set)):
+        if isinstance(new, (tuple, set, list)):
             new = loads(dumps(list(new)))
         self._write_new(new, key)
         last = self._read_last(key)
         if last is _ignore_:
             return
         self._log_assert_call(last, new, places, msg, delta)
         try:
@@ -134,15 +134,15 @@
             if self.silent:
                 logger.warning(str(e))
             else:
                 raise e
 
     def assertRegressiveEqual(self, new, msg=None, key=()):
         # version 0.3.1, fixing tuple as list issue 'loads(dumps(tuple))=list'
-        if isinstance(new, (tuple, set)):
+        if isinstance(new, (tuple, set, list)):
             new = loads(dumps(list(new)))
         self._write_new(new, key)
         last = self._read_last(key)
         if last is _ignore_:
             return
         self._log_assert_call(last, new, msg)
         try:
```

## Comparing `regtest-0.3.2/regtest/__init__.py` & `regtest-0.3.3/regtest/__init__.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,29 +1,29 @@
 # -*- coding: utf-8 -*-
 
 # regtest
 # -------
 # regression test enhancement for the Python unittest framework.
 #
 # Author:   sonntagsgesicht
-# Version:  0.3.1, copyright Sunday, 21 November 2021
+# Version:  0.3.3, copyright Friday, 05 May 2023
 # Website:  https://github.com/sonntagsgesicht/regtest
 # License:  Apache License 2.0 (see LICENSE file)
 
 
 import logging
 
 from unittest import *  # noqa F401 F402
 
 from .regtest import RegressionTestCase # noqa F401
 
 logging.getLogger(__name__).addHandler(logging.NullHandler())
 
 __doc__ = 'regression test enhancement for the Python unittest framework.'
-__version__ = '0.3.2'
+__version__ = '0.3.3'
 __dev_status__ = '4 - Beta'
 __date__ = 'Friday, 05 May 2023'
 __author__ = 'sonntagsgesicht'
 __email__ = 'sonntagsgesicht@icloud.com'
 __url__ = 'https://github.com/sonntagsgesicht/' + __name__
 __license__ = 'Apache License 2.0'
 __dependencies__ = ()
```

