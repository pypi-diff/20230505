# Comparing `tmp/regtest-0.3.1.zip` & `tmp/regtest-0.3.2.zip`

## zipinfo {}

```diff
@@ -1,19 +1,19 @@
-Zip file size: 13466 bytes, number of entries: 17
-drwxr-xr-x  2.0 unx        0 b- stor 23-May-05 10:32 regtest-0.3.1/
-drwxr-xr-x  2.0 unx        0 b- stor 23-May-05 10:32 regtest-0.3.1/regtest.egg-info/
-drwxr-xr-x  2.0 unx        0 b- stor 23-May-05 10:32 regtest-0.3.1/regtest/
--rw-r--r--  2.0 unx     2924 b- defN 23-May-05 10:32 regtest-0.3.1/PKG-INFO
--rw-r--r--  2.0 unx    11357 b- defN 17-Jul-29 12:58 regtest-0.3.1/LICENSE
--rwxr--r--  2.0 unx       43 b- defN 19-Sep-12 12:23 regtest-0.3.1/MANIFEST.in
--rw-r--r--  2.0 unx     1685 b- defN 21-Oct-07 10:13 regtest-0.3.1/setup.py
--rw-r--r--  2.0 unx       38 b- defN 23-May-05 10:32 regtest-0.3.1/setup.cfg
--rw-r--r--  2.0 unx     1925 b- defN 23-May-05 09:09 regtest-0.3.1/README.rst
--rw-r--r--  2.0 unx      713 b- defN 23-May-05 07:45 regtest-0.3.1/CHANGES.rst
--rw-r--r--  2.0 unx     2186 b- defN 21-Nov-21 12:45 regtest-0.3.1/HOWTO.rst
--rw-r--r--  2.0 unx     2924 b- defN 23-May-05 10:32 regtest-0.3.1/regtest.egg-info/PKG-INFO
--rw-r--r--  2.0 unx      224 b- defN 23-May-05 10:32 regtest-0.3.1/regtest.egg-info/SOURCES.txt
--rw-r--r--  2.0 unx        8 b- defN 23-May-05 10:32 regtest-0.3.1/regtest.egg-info/top_level.txt
--rw-r--r--  2.0 unx        1 b- defN 23-May-05 10:32 regtest-0.3.1/regtest.egg-info/dependency_links.txt
--rw-r--r--  2.0 unx     6287 b- defN 23-May-05 08:25 regtest-0.3.1/regtest/regtest.py
--rw-r--r--  2.0 unx      979 b- defN 23-May-05 08:25 regtest-0.3.1/regtest/__init__.py
-17 files, 31294 bytes uncompressed, 11166 bytes compressed:  64.3%
+Zip file size: 13506 bytes, number of entries: 17
+drwxr-xr-x  2.0 unx        0 b- stor 23-May-05 10:51 regtest-0.3.2/
+drwxr-xr-x  2.0 unx        0 b- stor 23-May-05 10:51 regtest-0.3.2/regtest.egg-info/
+drwxr-xr-x  2.0 unx        0 b- stor 23-May-05 10:51 regtest-0.3.2/regtest/
+-rw-r--r--  2.0 unx     2924 b- defN 23-May-05 10:51 regtest-0.3.2/PKG-INFO
+-rw-r--r--  2.0 unx    11357 b- defN 17-Jul-29 12:58 regtest-0.3.2/LICENSE
+-rwxr--r--  2.0 unx       43 b- defN 19-Sep-12 12:23 regtest-0.3.2/MANIFEST.in
+-rw-r--r--  2.0 unx     1685 b- defN 21-Oct-07 10:13 regtest-0.3.2/setup.py
+-rw-r--r--  2.0 unx       38 b- defN 23-May-05 10:51 regtest-0.3.2/setup.cfg
+-rw-r--r--  2.0 unx     1925 b- defN 23-May-05 09:09 regtest-0.3.2/README.rst
+-rw-r--r--  2.0 unx      833 b- defN 23-May-05 10:48 regtest-0.3.2/CHANGES.rst
+-rw-r--r--  2.0 unx     2186 b- defN 21-Nov-21 12:45 regtest-0.3.2/HOWTO.rst
+-rw-r--r--  2.0 unx     2924 b- defN 23-May-05 10:51 regtest-0.3.2/regtest.egg-info/PKG-INFO
+-rw-r--r--  2.0 unx      224 b- defN 23-May-05 10:51 regtest-0.3.2/regtest.egg-info/SOURCES.txt
+-rw-r--r--  2.0 unx        8 b- defN 23-May-05 10:51 regtest-0.3.2/regtest.egg-info/top_level.txt
+-rw-r--r--  2.0 unx        1 b- defN 23-May-05 10:51 regtest-0.3.2/regtest.egg-info/dependency_links.txt
+-rw-r--r--  2.0 unx     6329 b- defN 23-May-05 10:46 regtest-0.3.2/regtest/regtest.py
+-rw-r--r--  2.0 unx      979 b- defN 23-May-05 10:47 regtest-0.3.2/regtest/__init__.py
+17 files, 31456 bytes uncompressed, 11206 bytes compressed:  64.4%
```

## zipnote {}

```diff
@@ -1,52 +1,52 @@
-Filename: regtest-0.3.1/
+Filename: regtest-0.3.2/
 Comment: 
 
-Filename: regtest-0.3.1/regtest.egg-info/
+Filename: regtest-0.3.2/regtest.egg-info/
 Comment: 
 
-Filename: regtest-0.3.1/regtest/
+Filename: regtest-0.3.2/regtest/
 Comment: 
 
-Filename: regtest-0.3.1/PKG-INFO
+Filename: regtest-0.3.2/PKG-INFO
 Comment: 
 
-Filename: regtest-0.3.1/LICENSE
+Filename: regtest-0.3.2/LICENSE
 Comment: 
 
-Filename: regtest-0.3.1/MANIFEST.in
+Filename: regtest-0.3.2/MANIFEST.in
 Comment: 
 
-Filename: regtest-0.3.1/setup.py
+Filename: regtest-0.3.2/setup.py
 Comment: 
 
-Filename: regtest-0.3.1/setup.cfg
+Filename: regtest-0.3.2/setup.cfg
 Comment: 
 
-Filename: regtest-0.3.1/README.rst
+Filename: regtest-0.3.2/README.rst
 Comment: 
 
-Filename: regtest-0.3.1/CHANGES.rst
+Filename: regtest-0.3.2/CHANGES.rst
 Comment: 
 
-Filename: regtest-0.3.1/HOWTO.rst
+Filename: regtest-0.3.2/HOWTO.rst
 Comment: 
 
-Filename: regtest-0.3.1/regtest.egg-info/PKG-INFO
+Filename: regtest-0.3.2/regtest.egg-info/PKG-INFO
 Comment: 
 
-Filename: regtest-0.3.1/regtest.egg-info/SOURCES.txt
+Filename: regtest-0.3.2/regtest.egg-info/SOURCES.txt
 Comment: 
 
-Filename: regtest-0.3.1/regtest.egg-info/top_level.txt
+Filename: regtest-0.3.2/regtest.egg-info/top_level.txt
 Comment: 
 
-Filename: regtest-0.3.1/regtest.egg-info/dependency_links.txt
+Filename: regtest-0.3.2/regtest.egg-info/dependency_links.txt
 Comment: 
 
-Filename: regtest-0.3.1/regtest/regtest.py
+Filename: regtest-0.3.2/regtest/regtest.py
 Comment: 
 
-Filename: regtest-0.3.1/regtest/__init__.py
+Filename: regtest-0.3.2/regtest/__init__.py
 Comment: 
 
 Zip file comment:
```

## Comparing `regtest-0.3.1/PKG-INFO` & `regtest-0.3.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: regtest
-Version: 0.3.1
+Version: 0.3.2
 Summary: regression test enhancement for the Python unittest framework.
 Home-page: https://github.com/sonntagsgesicht/regtest
 Author: sonntagsgesicht
 Author-email: sonntagsgesicht@icloud.com
 License: Apache License 2.0
 Platform: any
 Classifier: Development Status :: 4 - Beta
```

## Comparing `regtest-0.3.1/LICENSE` & `regtest-0.3.2/LICENSE`

 * *Files identical despite different names*

## Comparing `regtest-0.3.1/setup.py` & `regtest-0.3.2/setup.py`

 * *Files identical despite different names*

## Comparing `regtest-0.3.1/README.rst` & `regtest-0.3.2/README.rst`

 * *Files identical despite different names*

## Comparing `regtest-0.3.1/CHANGES.rst` & `regtest-0.3.2/CHANGES.rst`

 * *Files 9% similar despite different names*

```diff
@@ -1,15 +1,22 @@
 
 These changes are listed in decreasing version number order.
 
+Release 0.3.2
+-------------
+
+Release date was |today|
+
+* fixing `tuple` as `list` issue for nested tuples.
+
 
 Release 0.3.1
 -------------
 
-Release date was |today|
+Release date was Friday, 05 May 2023
 
 * fixing `tuple` as `list` issue by `loads(dumps((1, 2)))==[1, 2]`.
   Now every `tuple` or `set` is asserted as a `list`.
 
 
 Release 0.3
 -----------
```

## Comparing `regtest-0.3.1/HOWTO.rst` & `regtest-0.3.2/HOWTO.rst`

 * *Files identical despite different names*

## Comparing `regtest-0.3.1/regtest.egg-info/PKG-INFO` & `regtest-0.3.2/regtest.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: regtest
-Version: 0.3.1
+Version: 0.3.2
 Summary: regression test enhancement for the Python unittest framework.
 Home-page: https://github.com/sonntagsgesicht/regtest
 Author: sonntagsgesicht
 Author-email: sonntagsgesicht@icloud.com
 License: Apache License 2.0
 Platform: any
 Classifier: Development Status :: 4 - Beta
```

## Comparing `regtest-0.3.1/regtest/regtest.py` & `regtest-0.3.2/regtest/regtest.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 # Author:   sonntagsgesicht
 # Version:  0.3.1, copyright Sunday, 21 November 2021
 # Website:  https://github.com/sonntagsgesicht/regtest
 # License:  Apache License 2.0 (see LICENSE file)
 
 
 from inspect import stack
-from json import load, dump
+from json import load, dump, loads, dumps
 from logging import getLogger, NullHandler
 from os.path import exists, sep, join
 from os import makedirs
 from unittest import TestCase
 from gzip import open as zip
 
 OPEN = zip
@@ -117,15 +117,15 @@
                 with self.open(test_method, 'wt') as file:
                     dump(data, file, indent=2)
 
     def assertAlmostRegressiveEqual(
             self, new, places=7, msg=None, delta=None, key=()):
         # version 0.3.1, fixing tuple as list issue 'loads(dumps(tuple))=list'
         if isinstance(new, (tuple, set)):
-            new = list(new)
+            new = loads(dumps(list(new)))
         self._write_new(new, key)
         last = self._read_last(key)
         if last is _ignore_:
             return
         self._log_assert_call(last, new, places, msg, delta)
         try:
             return super(RegressionTestCase, self).assertAlmostEqual(
@@ -135,15 +135,15 @@
                 logger.warning(str(e))
             else:
                 raise e
 
     def assertRegressiveEqual(self, new, msg=None, key=()):
         # version 0.3.1, fixing tuple as list issue 'loads(dumps(tuple))=list'
         if isinstance(new, (tuple, set)):
-            new = list(new)
+            new = loads(dumps(list(new)))
         self._write_new(new, key)
         last = self._read_last(key)
         if last is _ignore_:
             return
         self._log_assert_call(last, new, msg)
         try:
             return super(RegressionTestCase, self).assertEqual(last, new, msg)
```

## Comparing `regtest-0.3.1/regtest/__init__.py` & `regtest-0.3.2/regtest/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -15,15 +15,15 @@
 from unittest import *  # noqa F401 F402
 
 from .regtest import RegressionTestCase # noqa F401
 
 logging.getLogger(__name__).addHandler(logging.NullHandler())
 
 __doc__ = 'regression test enhancement for the Python unittest framework.'
-__version__ = '0.3.1'
+__version__ = '0.3.2'
 __dev_status__ = '4 - Beta'
 __date__ = 'Friday, 05 May 2023'
 __author__ = 'sonntagsgesicht'
 __email__ = 'sonntagsgesicht@icloud.com'
 __url__ = 'https://github.com/sonntagsgesicht/' + __name__
 __license__ = 'Apache License 2.0'
 __dependencies__ = ()
```

