# Comparing `tmp/regtest-0.3.zip` & `tmp/regtest-0.3.1.zip`

## zipinfo {}

```diff
@@ -1,19 +1,19 @@
-Zip file size: 13258 bytes, number of entries: 17
-drwxr-xr-x  2.0 unx        0 b- stor 21-Nov-21 12:55 regtest-0.3/
-drwxr-xr-x  2.0 unx        0 b- stor 21-Nov-21 12:55 regtest-0.3/regtest.egg-info/
-drwxr-xr-x  2.0 unx        0 b- stor 21-Nov-21 12:55 regtest-0.3/regtest/
--rw-r--r--  2.0 unx     2864 b- defN 21-Nov-21 12:55 regtest-0.3/PKG-INFO
--rw-r--r--  2.0 unx    11357 b- defN 17-Jul-29 12:58 regtest-0.3/LICENSE
--rwxr--r--  2.0 unx       43 b- defN 19-Sep-12 12:23 regtest-0.3/MANIFEST.in
--rw-r--r--  2.0 unx     1685 b- defN 21-Oct-07 10:13 regtest-0.3/setup.py
--rw-r--r--  2.0 unx       38 b- defN 21-Nov-21 12:55 regtest-0.3/setup.cfg
--rw-r--r--  2.0 unx     1865 b- defN 21-Oct-07 11:23 regtest-0.3/README.rst
--rw-r--r--  2.0 unx      424 b- defN 21-Oct-07 11:24 regtest-0.3/CHANGES.rst
--rw-r--r--  2.0 unx     2186 b- defN 21-Nov-21 12:45 regtest-0.3/HOWTO.rst
--rw-r--r--  2.0 unx     2864 b- defN 21-Nov-21 12:55 regtest-0.3/regtest.egg-info/PKG-INFO
--rw-r--r--  2.0 unx      224 b- defN 21-Nov-21 12:55 regtest-0.3/regtest.egg-info/SOURCES.txt
--rw-r--r--  2.0 unx        8 b- defN 21-Nov-21 12:55 regtest-0.3/regtest.egg-info/top_level.txt
--rw-r--r--  2.0 unx        1 b- defN 21-Nov-21 12:55 regtest-0.3/regtest.egg-info/dependency_links.txt
--rw-r--r--  2.0 unx     5985 b- defN 21-Nov-21 12:41 regtest-0.3/regtest/regtest.py
--rw-r--r--  2.0 unx      898 b- defN 21-Nov-21 12:54 regtest-0.3/regtest/__init__.py
-17 files, 30442 bytes uncompressed, 11026 bytes compressed:  63.8%
+Zip file size: 13466 bytes, number of entries: 17
+drwxr-xr-x  2.0 unx        0 b- stor 23-May-05 10:32 regtest-0.3.1/
+drwxr-xr-x  2.0 unx        0 b- stor 23-May-05 10:32 regtest-0.3.1/regtest.egg-info/
+drwxr-xr-x  2.0 unx        0 b- stor 23-May-05 10:32 regtest-0.3.1/regtest/
+-rw-r--r--  2.0 unx     2924 b- defN 23-May-05 10:32 regtest-0.3.1/PKG-INFO
+-rw-r--r--  2.0 unx    11357 b- defN 17-Jul-29 12:58 regtest-0.3.1/LICENSE
+-rwxr--r--  2.0 unx       43 b- defN 19-Sep-12 12:23 regtest-0.3.1/MANIFEST.in
+-rw-r--r--  2.0 unx     1685 b- defN 21-Oct-07 10:13 regtest-0.3.1/setup.py
+-rw-r--r--  2.0 unx       38 b- defN 23-May-05 10:32 regtest-0.3.1/setup.cfg
+-rw-r--r--  2.0 unx     1925 b- defN 23-May-05 09:09 regtest-0.3.1/README.rst
+-rw-r--r--  2.0 unx      713 b- defN 23-May-05 07:45 regtest-0.3.1/CHANGES.rst
+-rw-r--r--  2.0 unx     2186 b- defN 21-Nov-21 12:45 regtest-0.3.1/HOWTO.rst
+-rw-r--r--  2.0 unx     2924 b- defN 23-May-05 10:32 regtest-0.3.1/regtest.egg-info/PKG-INFO
+-rw-r--r--  2.0 unx      224 b- defN 23-May-05 10:32 regtest-0.3.1/regtest.egg-info/SOURCES.txt
+-rw-r--r--  2.0 unx        8 b- defN 23-May-05 10:32 regtest-0.3.1/regtest.egg-info/top_level.txt
+-rw-r--r--  2.0 unx        1 b- defN 23-May-05 10:32 regtest-0.3.1/regtest.egg-info/dependency_links.txt
+-rw-r--r--  2.0 unx     6287 b- defN 23-May-05 08:25 regtest-0.3.1/regtest/regtest.py
+-rw-r--r--  2.0 unx      979 b- defN 23-May-05 08:25 regtest-0.3.1/regtest/__init__.py
+17 files, 31294 bytes uncompressed, 11166 bytes compressed:  64.3%
```

## zipnote {}

```diff
@@ -1,52 +1,52 @@
-Filename: regtest-0.3/
+Filename: regtest-0.3.1/
 Comment: 
 
-Filename: regtest-0.3/regtest.egg-info/
+Filename: regtest-0.3.1/regtest.egg-info/
 Comment: 
 
-Filename: regtest-0.3/regtest/
+Filename: regtest-0.3.1/regtest/
 Comment: 
 
-Filename: regtest-0.3/PKG-INFO
+Filename: regtest-0.3.1/PKG-INFO
 Comment: 
 
-Filename: regtest-0.3/LICENSE
+Filename: regtest-0.3.1/LICENSE
 Comment: 
 
-Filename: regtest-0.3/MANIFEST.in
+Filename: regtest-0.3.1/MANIFEST.in
 Comment: 
 
-Filename: regtest-0.3/setup.py
+Filename: regtest-0.3.1/setup.py
 Comment: 
 
-Filename: regtest-0.3/setup.cfg
+Filename: regtest-0.3.1/setup.cfg
 Comment: 
 
-Filename: regtest-0.3/README.rst
+Filename: regtest-0.3.1/README.rst
 Comment: 
 
-Filename: regtest-0.3/CHANGES.rst
+Filename: regtest-0.3.1/CHANGES.rst
 Comment: 
 
-Filename: regtest-0.3/HOWTO.rst
+Filename: regtest-0.3.1/HOWTO.rst
 Comment: 
 
-Filename: regtest-0.3/regtest.egg-info/PKG-INFO
+Filename: regtest-0.3.1/regtest.egg-info/PKG-INFO
 Comment: 
 
-Filename: regtest-0.3/regtest.egg-info/SOURCES.txt
+Filename: regtest-0.3.1/regtest.egg-info/SOURCES.txt
 Comment: 
 
-Filename: regtest-0.3/regtest.egg-info/top_level.txt
+Filename: regtest-0.3.1/regtest.egg-info/top_level.txt
 Comment: 
 
-Filename: regtest-0.3/regtest.egg-info/dependency_links.txt
+Filename: regtest-0.3.1/regtest.egg-info/dependency_links.txt
 Comment: 
 
-Filename: regtest-0.3/regtest/regtest.py
+Filename: regtest-0.3.1/regtest/regtest.py
 Comment: 
 
-Filename: regtest-0.3/regtest/__init__.py
+Filename: regtest-0.3.1/regtest/__init__.py
 Comment: 
 
 Zip file comment:
```

## Comparing `regtest-0.3/PKG-INFO` & `regtest-0.3.1/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: regtest
-Version: 0.3
+Version: 0.3.1
 Summary: regression test enhancement for the Python unittest framework.
 Home-page: https://github.com/sonntagsgesicht/regtest
 Author: sonntagsgesicht
 Author-email: sonntagsgesicht@icloud.com
 License: Apache License 2.0
 Platform: any
 Classifier: Development Status :: 4 - Beta
@@ -24,17 +24,17 @@
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 
 
 
 Regression test enhancement for the Python *unittest* framework
 
-.. image:: https://img.shields.io/codeship/a5a60730-ba8a-0137-8179-0660bd8c08b8/master.svg
-   :target: https://codeship.com//projects/364831
-   :alt: Codeship
+.. image:: https://github.com/sonntagsgesicht/regtest/actions/workflows/python-package.yml/badge.svg
+    :target: https://github.com/sonntagsgesicht/regtest/actions/workflows/python-package.yml
+    :alt: GitHubWorkflow
 
 .. image:: https://img.shields.io/readthedocs/regtest
    :target: http://regtest.readthedocs.io
    :alt: Read the Docs
 
 .. image:: https://img.shields.io/github/license/sonntagsgesicht/regtest
    :target: https://github.com/sonntagsgesicht/regtest/raw/master/LICENSE
@@ -73,9 +73,7 @@
 The next time (and at any time these routines run) the return values
 will be checked against the stored ones.
 
 To reset a routine simply remove the corresponding file
 (named accordingly) of stored reference data.
 The next time the reference data will be rebuild.
 
-
-
```

## Comparing `regtest-0.3/LICENSE` & `regtest-0.3.1/LICENSE`

 * *Files identical despite different names*

## Comparing `regtest-0.3/setup.py` & `regtest-0.3.1/setup.py`

 * *Files identical despite different names*

## Comparing `regtest-0.3/README.rst` & `regtest-0.3.1/README.rst`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 
 Regression test enhancement for the Python *unittest* framework
 
-.. image:: https://img.shields.io/codeship/a5a60730-ba8a-0137-8179-0660bd8c08b8/master.svg
-   :target: https://codeship.com//projects/364831
-   :alt: Codeship
+.. image:: https://github.com/sonntagsgesicht/regtest/actions/workflows/python-package.yml/badge.svg
+    :target: https://github.com/sonntagsgesicht/regtest/actions/workflows/python-package.yml
+    :alt: GitHubWorkflow
 
 .. image:: https://img.shields.io/readthedocs/regtest
    :target: http://regtest.readthedocs.io
    :alt: Read the Docs
 
 .. image:: https://img.shields.io/github/license/sonntagsgesicht/regtest
    :target: https://github.com/sonntagsgesicht/regtest/raw/master/LICENSE
```

## Comparing `regtest-0.3/HOWTO.rst` & `regtest-0.3.1/HOWTO.rst`

 * *Files identical despite different names*

## Comparing `regtest-0.3/regtest.egg-info/PKG-INFO` & `regtest-0.3.1/regtest.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: regtest
-Version: 0.3
+Version: 0.3.1
 Summary: regression test enhancement for the Python unittest framework.
 Home-page: https://github.com/sonntagsgesicht/regtest
 Author: sonntagsgesicht
 Author-email: sonntagsgesicht@icloud.com
 License: Apache License 2.0
 Platform: any
 Classifier: Development Status :: 4 - Beta
@@ -24,17 +24,17 @@
 Description-Content-Type: text/x-rst
 License-File: LICENSE
 
 
 
 Regression test enhancement for the Python *unittest* framework
 
-.. image:: https://img.shields.io/codeship/a5a60730-ba8a-0137-8179-0660bd8c08b8/master.svg
-   :target: https://codeship.com//projects/364831
-   :alt: Codeship
+.. image:: https://github.com/sonntagsgesicht/regtest/actions/workflows/python-package.yml/badge.svg
+    :target: https://github.com/sonntagsgesicht/regtest/actions/workflows/python-package.yml
+    :alt: GitHubWorkflow
 
 .. image:: https://img.shields.io/readthedocs/regtest
    :target: http://regtest.readthedocs.io
    :alt: Read the Docs
 
 .. image:: https://img.shields.io/github/license/sonntagsgesicht/regtest
    :target: https://github.com/sonntagsgesicht/regtest/raw/master/LICENSE
@@ -73,9 +73,7 @@
 The next time (and at any time these routines run) the return values
 will be checked against the stored ones.
 
 To reset a routine simply remove the corresponding file
 (named accordingly) of stored reference data.
 The next time the reference data will be rebuild.
 
-
-
```

## Comparing `regtest-0.3/regtest/regtest.py` & `regtest-0.3.1/regtest/regtest.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # -*- coding: utf-8 -*-
 
 # regtest
 # -------
 # regression test enhancement for the Python unittest framework.
 #
 # Author:   sonntagsgesicht
-# Version:  0.1, copyright Wednesday, 18 September 2019
+# Version:  0.3.1, copyright Sunday, 21 November 2021
 # Website:  https://github.com/sonntagsgesicht/regtest
 # License:  Apache License 2.0 (see LICENSE file)
 
 
 from inspect import stack
 from json import load, dump
 from logging import getLogger, NullHandler
@@ -48,15 +48,15 @@
 class RegressionTestCase(TestCase):
 
     folder = join('test', 'data')
     silent = False
     compression = True
 
     @property
-    def testmethodnames(self):
+    def alltestmethodnames(self):
         return tuple(m for m in dir(self) if m.startswith('test'))
 
     @property
     def rerun(self):
         return self._get_testmethod() in self._last_results
 
     def __init__(self, *args, **kwargs):
@@ -98,15 +98,15 @@
                 if self.__class__.silent:
                     logger.warning(msg)
                 else:
                     raise LeftoverAssertValueError(msg)
 
     def readResults(self):
         logger.info('read from %s' % (self.folder + sep))
-        for test_method in self.testmethodnames:
+        for test_method in self.alltestmethodnames:
             with self.open(test_method, 'rt') as file:
                 if file:
                     self._last_results[test_method] = load(file)
 
     def writeResults(self):
         msg = 'write to %s' % (self.folder + sep)
         for test_method, data in list(self._new_results.items()):
@@ -115,14 +115,17 @@
                     logger.info(msg)
                     msg = ''
                 with self.open(test_method, 'wt') as file:
                     dump(data, file, indent=2)
 
     def assertAlmostRegressiveEqual(
             self, new, places=7, msg=None, delta=None, key=()):
+        # version 0.3.1, fixing tuple as list issue 'loads(dumps(tuple))=list'
+        if isinstance(new, (tuple, set)):
+            new = list(new)
         self._write_new(new, key)
         last = self._read_last(key)
         if last is _ignore_:
             return
         self._log_assert_call(last, new, places, msg, delta)
         try:
             return super(RegressionTestCase, self).assertAlmostEqual(
@@ -130,14 +133,17 @@
         except AssertionError as e:
             if self.silent:
                 logger.warning(str(e))
             else:
                 raise e
 
     def assertRegressiveEqual(self, new, msg=None, key=()):
+        # version 0.3.1, fixing tuple as list issue 'loads(dumps(tuple))=list'
+        if isinstance(new, (tuple, set)):
+            new = list(new)
         self._write_new(new, key)
         last = self._read_last(key)
         if last is _ignore_:
             return
         self._log_assert_call(last, new, msg)
         try:
             return super(RegressionTestCase, self).assertEqual(last, new, msg)
```

## Comparing `regtest-0.3/regtest/__init__.py` & `regtest-0.3.1/regtest/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,33 +1,37 @@
 # -*- coding: utf-8 -*-
 
 # regtest
 # -------
 # regression test enhancement for the Python unittest framework.
 #
 # Author:   sonntagsgesicht
-# Version:  0.1, copyright Wednesday, 18 September 2019
+# Version:  0.3.1, copyright Sunday, 21 November 2021
 # Website:  https://github.com/sonntagsgesicht/regtest
 # License:  Apache License 2.0 (see LICENSE file)
 
 
 import logging
 
 from unittest import *  # noqa F401 F402
 
 from .regtest import RegressionTestCase # noqa F401
 
 logging.getLogger(__name__).addHandler(logging.NullHandler())
 
 __doc__ = 'regression test enhancement for the Python unittest framework.'
-__version__ = '0.3'
+__version__ = '0.3.1'
 __dev_status__ = '4 - Beta'
-__date__ = 'Sunday, 21 November 2021'
+__date__ = 'Friday, 05 May 2023'
 __author__ = 'sonntagsgesicht'
 __email__ = 'sonntagsgesicht@icloud.com'
 __url__ = 'https://github.com/sonntagsgesicht/' + __name__
 __license__ = 'Apache License 2.0'
 __dependencies__ = ()
 __dependency_links__ = ()
 __data__ = ()
 __scripts__ = ()
 __theme__ = ''
+
+
+# todo
+#  fix tuple value from json are turned into a list, so compare load(dump())
```

