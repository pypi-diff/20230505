# Comparing `tmp/zope.mkzeoinstance-5.1.tar.gz` & `tmp/zope.mkzeoinstance-5.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "zope.mkzeoinstance-5.1.tar", last modified: Fri Apr 28 05:57:35 2023, max compression
+gzip compressed data, was "zope.mkzeoinstance-5.1.1.tar", last modified: Fri May  5 06:29:41 2023, max compression
```

## Comparing `zope.mkzeoinstance-5.1.tar` & `zope.mkzeoinstance-5.1.1.tar`

### file list

```diff
@@ -1,27 +1,27 @@
-drwxr-xr-x   0 m.howitz   (502) staff       (20)        0 2023-04-28 05:57:35.793563 zope.mkzeoinstance-5.1/
--rw-r--r--   0 m.howitz   (502) staff       (20)     1849 2023-04-28 05:57:35.000000 zope.mkzeoinstance-5.1/CHANGES.rst
--rw-r--r--   0 m.howitz   (502) staff       (20)      804 2023-04-28 05:57:35.000000 zope.mkzeoinstance-5.1/CONTRIBUTING.md
--rw-r--r--   0 m.howitz   (502) staff       (20)      196 2023-04-28 05:57:35.000000 zope.mkzeoinstance-5.1/MANIFEST.in
--rw-r--r--   0 m.howitz   (502) staff       (20)     2973 2023-04-28 05:57:35.793629 zope.mkzeoinstance-5.1/PKG-INFO
--rw-r--r--   0 m.howitz   (502) staff       (20)      153 2023-04-28 05:57:35.000000 zope.mkzeoinstance-5.1/README.rst
--rw-r--r--   0 m.howitz   (502) staff       (20)      100 2023-04-28 05:57:35.000000 zope.mkzeoinstance-5.1/buildout.cfg
--rw-r--r--   0 m.howitz   (502) staff       (20)      423 2023-04-28 05:57:35.793931 zope.mkzeoinstance-5.1/setup.cfg
--rw-r--r--   0 m.howitz   (502) staff       (20)     2389 2023-04-28 05:57:35.000000 zope.mkzeoinstance-5.1/setup.py
-drwxr-xr-x   0 m.howitz   (502) staff       (20)        0 2023-04-28 05:57:35.790099 zope.mkzeoinstance-5.1/src/
-drwxr-xr-x   0 m.howitz   (502) staff       (20)        0 2023-04-28 05:57:35.791707 zope.mkzeoinstance-5.1/src/zope/
--rw-r--r--   0 m.howitz   (502) staff       (20)       56 2023-04-28 05:57:35.000000 zope.mkzeoinstance-5.1/src/zope/__init__.py
-drwxr-xr-x   0 m.howitz   (502) staff       (20)        0 2023-04-28 05:57:35.793127 zope.mkzeoinstance-5.1/src/zope/mkzeoinstance/
--rw-r--r--   0 m.howitz   (502) staff       (20)     7887 2023-04-28 05:57:35.000000 zope.mkzeoinstance-5.1/src/zope/mkzeoinstance/__init__.py
-drwxr-xr-x   0 m.howitz   (502) staff       (20)        0 2023-04-28 05:57:35.793403 zope.mkzeoinstance-5.1/src/zope/mkzeoinstance/tests/
--rw-r--r--   0 m.howitz   (502) staff       (20)        0 2023-04-28 05:57:35.000000 zope.mkzeoinstance-5.1/src/zope/mkzeoinstance/tests/__init__.py
--rw-r--r--   0 m.howitz   (502) staff       (20)    24486 2023-04-28 05:57:35.000000 zope.mkzeoinstance-5.1/src/zope/mkzeoinstance/tests/test_unix.py
-drwxr-xr-x   0 m.howitz   (502) staff       (20)        0 2023-04-28 05:57:35.792976 zope.mkzeoinstance-5.1/src/zope.mkzeoinstance.egg-info/
--rw-r--r--   0 m.howitz   (502) staff       (20)     2973 2023-04-28 05:57:35.000000 zope.mkzeoinstance-5.1/src/zope.mkzeoinstance.egg-info/PKG-INFO
--rw-r--r--   0 m.howitz   (502) staff       (20)      607 2023-04-28 05:57:35.000000 zope.mkzeoinstance-5.1/src/zope.mkzeoinstance.egg-info/SOURCES.txt
--rw-r--r--   0 m.howitz   (502) staff       (20)        1 2023-04-28 05:57:35.000000 zope.mkzeoinstance-5.1/src/zope.mkzeoinstance.egg-info/dependency_links.txt
--rw-r--r--   0 m.howitz   (502) staff       (20)       58 2023-04-28 05:57:35.000000 zope.mkzeoinstance-5.1/src/zope.mkzeoinstance.egg-info/entry_points.txt
--rw-r--r--   0 m.howitz   (502) staff       (20)        5 2023-04-28 05:57:35.000000 zope.mkzeoinstance-5.1/src/zope.mkzeoinstance.egg-info/namespace_packages.txt
--rw-r--r--   0 m.howitz   (502) staff       (20)        1 2023-04-28 05:57:35.000000 zope.mkzeoinstance-5.1/src/zope.mkzeoinstance.egg-info/not-zip-safe
--rw-r--r--   0 m.howitz   (502) staff       (20)       52 2023-04-28 05:57:35.000000 zope.mkzeoinstance-5.1/src/zope.mkzeoinstance.egg-info/requires.txt
--rw-r--r--   0 m.howitz   (502) staff       (20)        5 2023-04-28 05:57:35.000000 zope.mkzeoinstance-5.1/src/zope.mkzeoinstance.egg-info/top_level.txt
--rw-r--r--   0 m.howitz   (502) staff       (20)     1387 2023-04-28 05:57:35.000000 zope.mkzeoinstance-5.1/tox.ini
+drwxr-xr-x   0 mac        (513) staff       (20)        0 2023-05-05 06:29:41.484249 zope.mkzeoinstance-5.1.1/
+-rw-r--r--   0 mac        (513) staff       (20)     2017 2023-05-05 06:29:40.000000 zope.mkzeoinstance-5.1.1/CHANGES.rst
+-rw-r--r--   0 mac        (513) staff       (20)      804 2023-05-05 06:29:40.000000 zope.mkzeoinstance-5.1.1/CONTRIBUTING.md
+-rw-r--r--   0 mac        (513) staff       (20)      196 2023-05-05 06:29:40.000000 zope.mkzeoinstance-5.1.1/MANIFEST.in
+-rw-r--r--   0 mac        (513) staff       (20)     3143 2023-05-05 06:29:41.484373 zope.mkzeoinstance-5.1.1/PKG-INFO
+-rw-r--r--   0 mac        (513) staff       (20)      153 2023-05-05 06:29:40.000000 zope.mkzeoinstance-5.1.1/README.rst
+-rw-r--r--   0 mac        (513) staff       (20)      100 2023-05-05 06:29:40.000000 zope.mkzeoinstance-5.1.1/buildout.cfg
+-rw-r--r--   0 mac        (513) staff       (20)      423 2023-05-05 06:29:41.484920 zope.mkzeoinstance-5.1.1/setup.cfg
+-rw-r--r--   0 mac        (513) staff       (20)     2391 2023-05-05 06:29:40.000000 zope.mkzeoinstance-5.1.1/setup.py
+drwxr-xr-x   0 mac        (513) staff       (20)        0 2023-05-05 06:29:41.476912 zope.mkzeoinstance-5.1.1/src/
+drwxr-xr-x   0 mac        (513) staff       (20)        0 2023-05-05 06:29:41.480240 zope.mkzeoinstance-5.1.1/src/zope/
+-rw-r--r--   0 mac        (513) staff       (20)       56 2023-05-05 06:29:40.000000 zope.mkzeoinstance-5.1.1/src/zope/__init__.py
+drwxr-xr-x   0 mac        (513) staff       (20)        0 2023-05-05 06:29:41.483323 zope.mkzeoinstance-5.1.1/src/zope/mkzeoinstance/
+-rw-r--r--   0 mac        (513) staff       (20)     7894 2023-05-05 06:29:40.000000 zope.mkzeoinstance-5.1.1/src/zope/mkzeoinstance/__init__.py
+drwxr-xr-x   0 mac        (513) staff       (20)        0 2023-05-05 06:29:41.483920 zope.mkzeoinstance-5.1.1/src/zope/mkzeoinstance/tests/
+-rw-r--r--   0 mac        (513) staff       (20)        0 2023-05-05 06:29:40.000000 zope.mkzeoinstance-5.1.1/src/zope/mkzeoinstance/tests/__init__.py
+-rw-r--r--   0 mac        (513) staff       (20)    26627 2023-05-05 06:29:40.000000 zope.mkzeoinstance-5.1.1/src/zope/mkzeoinstance/tests/test_unix.py
+drwxr-xr-x   0 mac        (513) staff       (20)        0 2023-05-05 06:29:41.482979 zope.mkzeoinstance-5.1.1/src/zope.mkzeoinstance.egg-info/
+-rw-r--r--   0 mac        (513) staff       (20)     3143 2023-05-05 06:29:41.000000 zope.mkzeoinstance-5.1.1/src/zope.mkzeoinstance.egg-info/PKG-INFO
+-rw-r--r--   0 mac        (513) staff       (20)      607 2023-05-05 06:29:41.000000 zope.mkzeoinstance-5.1.1/src/zope.mkzeoinstance.egg-info/SOURCES.txt
+-rw-r--r--   0 mac        (513) staff       (20)        1 2023-05-05 06:29:41.000000 zope.mkzeoinstance-5.1.1/src/zope.mkzeoinstance.egg-info/dependency_links.txt
+-rw-r--r--   0 mac        (513) staff       (20)       58 2023-05-05 06:29:41.000000 zope.mkzeoinstance-5.1.1/src/zope.mkzeoinstance.egg-info/entry_points.txt
+-rw-r--r--   0 mac        (513) staff       (20)        5 2023-05-05 06:29:41.000000 zope.mkzeoinstance-5.1.1/src/zope.mkzeoinstance.egg-info/namespace_packages.txt
+-rw-r--r--   0 mac        (513) staff       (20)        1 2023-05-05 06:29:41.000000 zope.mkzeoinstance-5.1.1/src/zope.mkzeoinstance.egg-info/not-zip-safe
+-rw-r--r--   0 mac        (513) staff       (20)       52 2023-05-05 06:29:41.000000 zope.mkzeoinstance-5.1.1/src/zope.mkzeoinstance.egg-info/requires.txt
+-rw-r--r--   0 mac        (513) staff       (20)        5 2023-05-05 06:29:41.000000 zope.mkzeoinstance-5.1.1/src/zope.mkzeoinstance.egg-info/top_level.txt
+-rw-r--r--   0 mac        (513) staff       (20)     1387 2023-05-05 06:29:40.000000 zope.mkzeoinstance-5.1.1/tox.ini
```

### Comparing `zope.mkzeoinstance-5.1/CHANGES.rst` & `zope.mkzeoinstance-5.1.1/CHANGES.rst`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,17 @@
 Changelog
 =========
 
+5.1.1 (2023-05-05)
+------------------
+
+- Make ``blob_dir`` parameter added in 5.1 optional.
+  (`#18 <https://github.com/zopefoundation/zope.mkzeoinstance/pull/18>`_)
+
+
 5.1 (2023-04-28)
 ----------------
 
 - Add configuration option ``-b`` resp. ``--blobs`` for passing blob directory
   path. (`#16 <https://github.com/zopefoundation/zope.mkzeoinstance/pull/16>`_)
```

### Comparing `zope.mkzeoinstance-5.1/CONTRIBUTING.md` & `zope.mkzeoinstance-5.1.1/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `zope.mkzeoinstance-5.1/PKG-INFO` & `zope.mkzeoinstance-5.1.1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zope.mkzeoinstance
-Version: 5.1
+Version: 5.1.1
 Summary: Make standalone ZEO database server instances
 Home-page: https://github.com/zopefoundation/zope.mkzeoinstance
 Author: Zope Foundation and Contributors
 Author-email: zope-dev@zope.dev
 License: ZPL 2.1
 Keywords: ZEO ZODB instance script
 Classifier: Development Status :: 5 - Production/Stable
@@ -27,14 +27,21 @@
 
 This package provides a single script, ``mkzeoinstance``, which creates
 a standalone ZEO server instance.
 
 Changelog
 =========
 
+5.1.1 (2023-05-05)
+------------------
+
+- Make ``blob_dir`` parameter added in 5.1 optional.
+  (`#18 <https://github.com/zopefoundation/zope.mkzeoinstance/pull/18>`_)
+
+
 5.1 (2023-04-28)
 ----------------
 
 - Add configuration option ``-b`` resp. ``--blobs`` for passing blob directory
   path. (`#16 <https://github.com/zopefoundation/zope.mkzeoinstance/pull/16>`_)
```

### Comparing `zope.mkzeoinstance-5.1/setup.py` & `zope.mkzeoinstance-5.1.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 
 from setuptools import find_packages
 from setuptools import setup
 
 
 setup(
     name='zope.mkzeoinstance',
-    version='5.1',
+    version='5.1.1',
     url='https://github.com/zopefoundation/zope.mkzeoinstance',
     license='ZPL 2.1',
     description='Make standalone ZEO database server instances',
     author='Zope Foundation and Contributors',
     author_email='zope-dev@zope.dev',
     long_description=(open('README.rst').read() + "\n" +
                       open('CHANGES.rst').read()),
```

### Comparing `zope.mkzeoinstance-5.1/src/zope/mkzeoinstance/__init__.py` & `zope.mkzeoinstance-5.1.1/src/zope/mkzeoinstance/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -178,15 +178,15 @@
         makedir(home)
         makedir(home, "etc")
         makedir(home, "var")
         makedir(home, "log")
         makedir(home, "bin")
 
         # Create dir only when default is selected
-        if ZEO_DEFAULT_BLOB_DIR in params.get('blob_dir', ''):
+        if ZEO_DEFAULT_BLOB_DIR in params.setdefault('blob_dir', ''):
             makedir(home, "var/blobs")
 
         makefile(ZEO_CONF_TEMPLATE, home, "etc", "zeo.conf", **params)
         makexfile(ZEOCTL_TEMPLATE, home, "bin", "zeoctl", **params)
         makexfile(RUNZEO_TEMPLATE, home, "bin", "runzeo", **params)
 
     def run(self, argv,
```

### Comparing `zope.mkzeoinstance-5.1/src/zope/mkzeoinstance/tests/test_unix.py` & `zope.mkzeoinstance-5.1.1/src/zope/mkzeoinstance/tests/test_unix.py`

 * *Files 2% similar despite different names*

```diff
@@ -419,14 +419,79 @@
 
         with TempStdout():
             builder.create(instance_home, params)
 
         with open(zeo_conf_path) as f:
             self.assertEqual(f.read(), expected_out)
 
+    def test_zeo_conf_content_w_missing_blob_param(self):
+        import os
+
+        builder = self._makeOne()
+        params = self._makeParams()
+
+        # there may be packages out there
+        # which do not provide the new parameter "blob_dir".
+        del params["blob_dir"]
+
+        instance_home = params['instance_home']
+        zeo_conf_path = os.path.join(instance_home, 'etc', 'zeo.conf')
+        expected_out = "\n".join([
+            "# ZEO configuration file",
+            "",
+            "%%define INSTANCE %(instance_home)s",
+            "",
+            "<zeo>",
+            "  address 99999",
+            "  read-only false",
+            "  invalidation-queue-size 100",
+            "  # pid-filename $INSTANCE/var/ZEO.pid",
+            "  # monitor-address PORT",
+            "  # transaction-timeout SECONDS",
+            "</zeo>",
+            "",
+            "<filestorage 1>",
+            "  path $INSTANCE/var/Data.fs",
+            "  ",
+            "</filestorage>",
+            "",
+            "<eventlog>",
+            "  level info",
+            "  <logfile>",
+            "    path $INSTANCE/log/zeo.log",
+            "  </logfile>",
+            "</eventlog>",
+            "",
+            "<runner>",
+            "  program $INSTANCE/bin/runzeo",
+            "  socket-name $INSTANCE/var/zeo.zdsock",
+            "  daemon true",
+            "  forever false",
+            "  backoff-limit 10",
+            "  exit-codes 0, 2",
+            "  directory $INSTANCE",
+            "  default-to-interactive true",
+            "  # user zope",
+            "  python %(executable)s",
+            "  zdrun %(zdaemon_home)s/zdaemon/zdrun.py",
+            "",
+            "  # This logfile should match the one in the zeo.conf file.",
+            ("  # It is used by zdctl's logtail command, "
+             "zdrun/zdctl doesn't write it."),
+            "  logfile $INSTANCE/log/zeo.log",
+            "</runner>",
+            '',
+        ]) % params
+
+        with TempStdout():
+            builder.create(instance_home, params)
+
+        with open(zeo_conf_path) as f:
+            self.assertEqual(f.read(), expected_out)
+
     def test_zeoctl_content(self):
         import os
         params = self._makeParams()
         instance_home = params['instance_home']
         zeoctl_path = os.path.join(instance_home, 'bin', 'zeoctl')
 
         expected_out = "\n".join([
```

### Comparing `zope.mkzeoinstance-5.1/src/zope.mkzeoinstance.egg-info/PKG-INFO` & `zope.mkzeoinstance-5.1.1/src/zope.mkzeoinstance.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: zope.mkzeoinstance
-Version: 5.1
+Version: 5.1.1
 Summary: Make standalone ZEO database server instances
 Home-page: https://github.com/zopefoundation/zope.mkzeoinstance
 Author: Zope Foundation and Contributors
 Author-email: zope-dev@zope.dev
 License: ZPL 2.1
 Keywords: ZEO ZODB instance script
 Classifier: Development Status :: 5 - Production/Stable
@@ -27,14 +27,21 @@
 
 This package provides a single script, ``mkzeoinstance``, which creates
 a standalone ZEO server instance.
 
 Changelog
 =========
 
+5.1.1 (2023-05-05)
+------------------
+
+- Make ``blob_dir`` parameter added in 5.1 optional.
+  (`#18 <https://github.com/zopefoundation/zope.mkzeoinstance/pull/18>`_)
+
+
 5.1 (2023-04-28)
 ----------------
 
 - Add configuration option ``-b`` resp. ``--blobs`` for passing blob directory
   path. (`#16 <https://github.com/zopefoundation/zope.mkzeoinstance/pull/16>`_)
```

### Comparing `zope.mkzeoinstance-5.1/src/zope.mkzeoinstance.egg-info/SOURCES.txt` & `zope.mkzeoinstance-5.1.1/src/zope.mkzeoinstance.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `zope.mkzeoinstance-5.1/tox.ini` & `zope.mkzeoinstance-5.1.1/tox.ini`

 * *Files identical despite different names*

