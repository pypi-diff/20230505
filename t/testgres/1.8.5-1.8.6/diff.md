# Comparing `tmp/testgres-1.8.5.tar.gz` & `tmp/testgres-1.8.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "testgres-1.8.5.tar", last modified: Tue May 24 14:50:03 2022, max compression
+gzip compressed data, was "testgres-1.8.6.tar", last modified: Fri May  5 11:15:28 2023, max compression
```

## Comparing `testgres-1.8.5.tar` & `testgres-1.8.6.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxrwxr-x   0 vbif      (1000) vbif      (1000)        0 2022-05-24 14:50:03.034646 testgres-1.8.5/
--rw-rw-r--   0 vbif      (1000) vbif      (1000)     1106 2022-04-11 10:37:10.000000 testgres-1.8.5/LICENSE
--rw-rw-r--   0 vbif      (1000) vbif      (1000)      136 2022-04-11 10:37:10.000000 testgres-1.8.5/MANIFEST.in
--rw-rw-r--   0 vbif      (1000) vbif      (1000)     5713 2022-05-24 14:50:03.034646 testgres-1.8.5/PKG-INFO
--rw-rw-r--   0 vbif      (1000) vbif      (1000)     5379 2022-04-11 10:37:10.000000 testgres-1.8.5/README.md
--rw-rw-r--   0 vbif      (1000) vbif      (1000)      160 2022-05-24 14:50:03.034646 testgres-1.8.5/setup.cfg
--rwxrwxr-x   0 vbif      (1000) vbif      (1000)      975 2022-05-24 14:21:13.000000 testgres-1.8.5/setup.py
-drwxrwxr-x   0 vbif      (1000) vbif      (1000)        0 2022-05-24 14:50:03.030646 testgres-1.8.5/testgres/
--rw-rw-r--   0 vbif      (1000) vbif      (1000)      588 2022-04-11 10:37:10.000000 testgres-1.8.5/testgres/__init__.py
--rw-rw-r--   0 vbif      (1000) vbif      (1000)     1524 2022-04-11 10:37:10.000000 testgres-1.8.5/testgres/api.py
--rw-rw-r--   0 vbif      (1000) vbif      (1000)     5187 2022-04-11 16:26:54.000000 testgres-1.8.5/testgres/backup.py
--rw-rw-r--   0 vbif      (1000) vbif      (1000)     2195 2022-04-11 16:26:54.000000 testgres-1.8.5/testgres/cache.py
--rw-rw-r--   0 vbif      (1000) vbif      (1000)     4781 2022-04-11 16:26:54.000000 testgres-1.8.5/testgres/config.py
--rw-rw-r--   0 vbif      (1000) vbif      (1000)     3080 2022-04-11 16:26:54.000000 testgres-1.8.5/testgres/connection.py
--rw-rw-r--   0 vbif      (1000) vbif      (1000)      819 2022-04-11 10:37:10.000000 testgres-1.8.5/testgres/consts.py
--rw-rw-r--   0 vbif      (1000) vbif      (1000)     1749 2022-04-11 16:26:54.000000 testgres-1.8.5/testgres/decorators.py
--rw-rw-r--   0 vbif      (1000) vbif      (1000)      932 2022-04-11 10:37:10.000000 testgres-1.8.5/testgres/defaults.py
--rw-rw-r--   0 vbif      (1000) vbif      (1000)     2303 2022-04-11 10:37:10.000000 testgres-1.8.5/testgres/enums.py
--rw-rw-r--   0 vbif      (1000) vbif      (1000)     1988 2022-04-11 10:37:10.000000 testgres-1.8.5/testgres/exceptions.py
--rw-rw-r--   0 vbif      (1000) vbif      (1000)     1428 2022-04-11 16:26:54.000000 testgres-1.8.5/testgres/logger.py
--rw-rw-r--   0 vbif      (1000) vbif      (1000)    41720 2022-05-24 14:20:05.000000 testgres-1.8.5/testgres/node.py
--rw-rw-r--   0 vbif      (1000) vbif      (1000)     8225 2022-04-11 16:26:54.000000 testgres-1.8.5/testgres/pubsub.py
--rw-rw-r--   0 vbif      (1000) vbif      (1000)     1547 2022-04-11 16:26:54.000000 testgres-1.8.5/testgres/standby.py
--rw-rw-r--   0 vbif      (1000) vbif      (1000)     6293 2022-04-11 16:26:54.000000 testgres-1.8.5/testgres/utils.py
-drwxrwxr-x   0 vbif      (1000) vbif      (1000)        0 2022-05-24 14:50:03.030646 testgres-1.8.5/testgres.egg-info/
--rw-rw-r--   0 vbif      (1000) vbif      (1000)     5713 2022-05-24 14:50:02.000000 testgres-1.8.5/testgres.egg-info/PKG-INFO
--rw-rw-r--   0 vbif      (1000) vbif      (1000)      541 2022-05-24 14:50:03.000000 testgres-1.8.5/testgres.egg-info/SOURCES.txt
--rw-rw-r--   0 vbif      (1000) vbif      (1000)        1 2022-05-24 14:50:02.000000 testgres-1.8.5/testgres.egg-info/dependency_links.txt
--rw-rw-r--   0 vbif      (1000) vbif      (1000)       39 2022-05-24 14:50:02.000000 testgres-1.8.5/testgres.egg-info/requires.txt
--rw-rw-r--   0 vbif      (1000) vbif      (1000)        9 2022-05-24 14:50:02.000000 testgres-1.8.5/testgres.egg-info/top_level.txt
-drwxrwxr-x   0 vbif      (1000) vbif      (1000)        0 2022-05-24 14:50:03.030646 testgres-1.8.5/tests/
--rwxrwxr-x   0 vbif      (1000) vbif      (1000)    33775 2022-04-11 16:26:54.000000 testgres-1.8.5/tests/test_simple.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 11:15:27.997087 testgres-1.8.6/
+-rw-rw-r--   0 root         (0) root         (0)     1106 2022-02-22 09:57:57.000000 testgres-1.8.6/LICENSE
+-rw-rw-r--   0 root         (0) root         (0)      136 2022-02-22 09:57:57.000000 testgres-1.8.6/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     5753 2023-05-05 11:15:27.997087 testgres-1.8.6/PKG-INFO
+-rw-rw-r--   0 root         (0) root         (0)     5399 2023-05-05 04:23:08.000000 testgres-1.8.6/README.md
+-rw-rw-r--   0 root         (0) root         (0)      160 2023-05-05 11:15:28.001087 testgres-1.8.6/setup.cfg
+-rwxrwxr-x   0 root         (0) root         (0)      975 2023-05-05 04:23:08.000000 testgres-1.8.6/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 11:15:27.997087 testgres-1.8.6/testgres/
+-rw-rw-r--   0 root         (0) root         (0)     1519 2023-05-05 04:23:08.000000 testgres-1.8.6/testgres/__init__.py
+-rw-rw-r--   0 root         (0) root         (0)     1524 2022-02-22 09:57:57.000000 testgres-1.8.6/testgres/api.py
+-rw-rw-r--   0 root         (0) root         (0)     5187 2022-05-06 11:01:56.000000 testgres-1.8.6/testgres/backup.py
+-rw-rw-r--   0 root         (0) root         (0)     2195 2022-05-06 11:01:56.000000 testgres-1.8.6/testgres/cache.py
+-rw-rw-r--   0 root         (0) root         (0)     4781 2022-05-06 11:01:56.000000 testgres-1.8.6/testgres/config.py
+-rw-rw-r--   0 root         (0) root         (0)     3080 2022-05-06 11:01:56.000000 testgres-1.8.6/testgres/connection.py
+-rw-rw-r--   0 root         (0) root         (0)      819 2022-02-22 09:57:57.000000 testgres-1.8.6/testgres/consts.py
+-rw-rw-r--   0 root         (0) root         (0)     1749 2022-05-06 11:01:56.000000 testgres-1.8.6/testgres/decorators.py
+-rw-rw-r--   0 root         (0) root         (0)      932 2022-02-22 09:57:57.000000 testgres-1.8.6/testgres/defaults.py
+-rw-rw-r--   0 root         (0) root         (0)     2451 2023-05-05 04:23:08.000000 testgres-1.8.6/testgres/enums.py
+-rw-rw-r--   0 root         (0) root         (0)     1988 2022-02-22 09:57:57.000000 testgres-1.8.6/testgres/exceptions.py
+-rw-rw-r--   0 root         (0) root         (0)     1428 2022-05-06 11:01:56.000000 testgres-1.8.6/testgres/logger.py
+-rw-rw-r--   0 root         (0) root         (0)    51631 2023-05-05 10:42:56.000000 testgres-1.8.6/testgres/node.py
+-rw-rw-r--   0 root         (0) root         (0)     8225 2022-05-06 11:01:56.000000 testgres-1.8.6/testgres/pubsub.py
+-rw-rw-r--   0 root         (0) root         (0)     1547 2022-05-06 11:01:56.000000 testgres-1.8.6/testgres/standby.py
+-rw-rw-r--   0 root         (0) root         (0)     6283 2022-11-09 15:43:39.000000 testgres-1.8.6/testgres/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 11:15:27.997087 testgres-1.8.6/testgres.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     5753 2023-05-05 11:15:27.000000 testgres-1.8.6/testgres.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      541 2023-05-05 11:15:27.000000 testgres-1.8.6/testgres.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-05 11:15:27.000000 testgres-1.8.6/testgres.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       39 2023-05-05 11:15:27.000000 testgres-1.8.6/testgres.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        9 2023-05-05 11:15:27.000000 testgres-1.8.6/testgres.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 11:15:27.997087 testgres-1.8.6/tests/
+-rwxrwxr-x   0 root         (0) root         (0)    34618 2023-05-05 04:23:08.000000 testgres-1.8.6/tests/test_simple.py
```

### Comparing `testgres-1.8.5/LICENSE` & `testgres-1.8.6/LICENSE`

 * *Files identical despite different names*

### Comparing `testgres-1.8.5/PKG-INFO` & `testgres-1.8.6/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 Metadata-Version: 2.1
 Name: testgres
-Version: 1.8.5
+Version: 1.8.6
 Summary: Testing utility for PostgreSQL and its extensions
 Home-page: https://github.com/postgrespro/testgres
 Author: Ildar Musin
 Author-email: zildermann@gmail.com
 License: PostgreSQL
 Keywords: test,testing,postgresql
+Platform: UNKNOWN
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-[![Build Status](https://travis-ci.org/postgrespro/testgres.svg?branch=master)](https://travis-ci.org/postgrespro/testgres)
+[![Build Status](https://travis-ci.com/postgrespro/testgres.svg?branch=master)](https://app.travis-ci.com/github/postgrespro/testgres/branches)
 [![codecov](https://codecov.io/gh/postgrespro/testgres/branch/master/graph/badge.svg)](https://codecov.io/gh/postgrespro/testgres)
 [![PyPI version](https://badge.fury.io/py/testgres.svg)](https://badge.fury.io/py/testgres)
 
 [Documentation](https://postgrespro.github.io/testgres/)
 
 # testgres
 
@@ -188,7 +189,9 @@
 
 ## Authors
 
 [Ildar Musin](https://github.com/zilder)  
 [Dmitry Ivanov](https://github.com/funbringer)  
 [Ildus Kurbangaliev](https://github.com/ildus)  
 [Yury Zhuravlev](https://github.com/stalkerg)  
+
+
```

### Comparing `testgres-1.8.5/README.md` & `testgres-1.8.6/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-[![Build Status](https://travis-ci.org/postgrespro/testgres.svg?branch=master)](https://travis-ci.org/postgrespro/testgres)
+[![Build Status](https://travis-ci.com/postgrespro/testgres.svg?branch=master)](https://app.travis-ci.com/github/postgrespro/testgres/branches)
 [![codecov](https://codecov.io/gh/postgrespro/testgres/branch/master/graph/badge.svg)](https://codecov.io/gh/postgrespro/testgres)
 [![PyPI version](https://badge.fury.io/py/testgres.svg)](https://badge.fury.io/py/testgres)
 
 [Documentation](https://postgrespro.github.io/testgres/)
 
 # testgres
```

### Comparing `testgres-1.8.5/setup.py` & `testgres-1.8.6/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -17,15 +17,15 @@
     install_requires.append("ipaddress")
 
 # Get contents of README file
 with open('README.md', 'r') as f:
     readme = f.read()
 
 setup(
-    version='1.8.5',
+    version='1.8.6',
     name='testgres',
     packages=['testgres'],
     description='Testing utility for PostgreSQL and its extensions',
     url='https://github.com/postgrespro/testgres',
     long_description=readme,
     long_description_content_type='text/markdown',
     license='PostgreSQL',
```

### Comparing `testgres-1.8.5/testgres/api.py` & `testgres-1.8.6/testgres/api.py`

 * *Files identical despite different names*

### Comparing `testgres-1.8.5/testgres/backup.py` & `testgres-1.8.6/testgres/backup.py`

 * *Files identical despite different names*

### Comparing `testgres-1.8.5/testgres/cache.py` & `testgres-1.8.6/testgres/cache.py`

 * *Files identical despite different names*

### Comparing `testgres-1.8.5/testgres/config.py` & `testgres-1.8.6/testgres/config.py`

 * *Files identical despite different names*

### Comparing `testgres-1.8.5/testgres/connection.py` & `testgres-1.8.6/testgres/connection.py`

 * *Files identical despite different names*

### Comparing `testgres-1.8.5/testgres/consts.py` & `testgres-1.8.6/testgres/consts.py`

 * *Files identical despite different names*

### Comparing `testgres-1.8.5/testgres/decorators.py` & `testgres-1.8.6/testgres/decorators.py`

 * *Files identical despite different names*

### Comparing `testgres-1.8.5/testgres/defaults.py` & `testgres-1.8.6/testgres/defaults.py`

 * *Files identical despite different names*

### Comparing `testgres-1.8.5/testgres/enums.py` & `testgres-1.8.6/testgres/enums.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from enum import Enum, IntEnum
 from six import iteritems
+from psutil import NoSuchProcess
 
 
 class XLogMethod(Enum):
     """
     Available WAL methods for :class:`.NodeBackup`
     """
 
@@ -64,19 +65,23 @@
                 'logical replication worker'
             ],
             ProcessType.BackgroundWriter: [
                 'writer'
             ],
         }  # yapf: disable
 
+        try:
+            cmdline = ''.join(process.cmdline())
+        except (FileNotFoundError, ProcessLookupError, NoSuchProcess):
+            return ProcessType.Unknown
+
         # we deliberately cut special words and spaces
-        cmdline = ''.join(process.cmdline()) \
-                    .replace('postgres:', '', 1) \
-                    .replace('bgworker:', '', 1) \
-                    .replace(' ', '')
+        cmdline = cmdline.replace('postgres:', '', 1) \
+            .replace('bgworker:', '', 1) \
+            .replace(' ', '')
 
         for ptype in ProcessType:
             if cmdline.startswith(ptype.value.replace(' ', '')):
                 return ptype
 
         for ptype, names in iteritems(alternative_names):
             for name in names:
```

### Comparing `testgres-1.8.5/testgres/exceptions.py` & `testgres-1.8.6/testgres/exceptions.py`

 * *Files identical despite different names*

### Comparing `testgres-1.8.5/testgres/logger.py` & `testgres-1.8.6/testgres/logger.py`

 * *Files identical despite different names*

### Comparing `testgres-1.8.5/testgres/node.py` & `testgres-1.8.6/testgres/node.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,20 +1,36 @@
 # coding: utf-8
 
 import io
 import os
+import random
+import shutil
+import signal
+import threading
+from queue import Queue
+
 import psutil
 import subprocess
 import time
 
+
 try:
     from collections.abc import Iterable
 except ImportError:
     from collections import Iterable
 
+# we support both pg8000 and psycopg2
+try:
+    import psycopg2 as pglib
+except ImportError:
+    try:
+        import pg8000 as pglib
+    except ImportError:
+        raise ImportError("You must have psycopg2 or pg8000 modules installed")
+
 from shutil import rmtree
 from six import raise_from, iteritems, text_type
 from tempfile import mkstemp, mkdtemp
 
 from .enums import \
     NodeStatus, \
     ProcessType, \
@@ -82,23 +98,28 @@
     release_port, \
     execute_utility, \
     options_string, \
     clean_on_error
 
 from .backup import NodeBackup
 
+InternalError = pglib.InternalError
+ProgrammingError = pglib.ProgrammingError
+OperationalError = pglib.OperationalError
+
 
 class ProcessProxy(object):
     """
     Wrapper for psutil.Process
 
     Attributes:
         process: wrapped psutill.Process object
         ptype: instance of ProcessType
     """
+
     def __init__(self, process, ptype=None):
         self.process = process
         self.ptype = ptype or ProcessType.from_process(process)
 
     def __getattr__(self, name):
         return getattr(self.process, name)
 
@@ -136,14 +157,17 @@
         self.cleanup_on_bad_exit = testgres_config.node_cleanup_on_bad_exit
         self.shutdown_max_attempts = 3
 
         # NOTE: for compatibility
         self.utils_log_name = self.utils_log_file
         self.pg_log_name = self.pg_log_file
 
+        # Node state
+        self.is_started = False
+
     def __enter__(self):
         return self
 
     def __exit__(self, type, value, traceback):
         self.free_port()
 
         # NOTE: Ctrl+C does not count!
@@ -335,15 +359,15 @@
         except ValueError:
             conninfo["host"] = master.host
 
         line = (
             "primary_conninfo='{}'\n"
         ).format(options_string(**conninfo))  # yapf: disable
         # Since 12 recovery.conf had disappeared
-        if self.version >= '12':
+        if self.version >= PgVer('12'):
             signal_name = os.path.join(self.data_dir, "standby.signal")
             # cross-python touch(). It is vulnerable to races, but who cares?
             with open(signal_name, 'a'):
                 os.utime(signal_name, None)
         else:
             line += "standby_mode=on\n"
 
@@ -367,15 +391,15 @@
                 con.execute(
                     """
                     select pg_catalog.pg_create_physical_replication_slot(%s)
                     """, slot)
 
             line += "primary_slot_name={}\n".format(slot)
 
-        if self.version >= '12':
+        if self.version >= PgVer('12'):
             self.append_conf(line=line)
         else:
             self.append_conf(filename=RECOVERY_CONF_FILE, line=line)
 
     def _maybe_start_logger(self):
         if testgres_config.use_python_logging:
             # spawn new logger if it doesn't exist or is stopped
@@ -513,28 +537,28 @@
         if allow_streaming or allow_logical:
             self.append_conf(max_replication_slots=MAX_REPLICATION_SLOTS,
                              max_wal_senders=MAX_WAL_SENDERS)  # yapf: disable
 
         # binary replication
         if allow_streaming:
             # select a proper wal_level for PostgreSQL
-            wal_level = 'replica' if self._pg_version >= '9.6' else 'hot_standby'
+            wal_level = 'replica' if self._pg_version >= PgVer('9.6') else 'hot_standby'
 
-            if self._pg_version < '13':
+            if self._pg_version < PgVer('13'):
                 self.append_conf(hot_standby=True,
                                  wal_keep_segments=WAL_KEEP_SEGMENTS,
                                  wal_level=wal_level)  # yapf: disable
             else:
                 self.append_conf(hot_standby=True,
                                  wal_keep_size=WAL_KEEP_SIZE,
                                  wal_level=wal_level)  # yapf: disable
 
         # logical replication
         if allow_logical:
-            if self._pg_version < '10':
+            if self._pg_version < PgVer('10'):
                 raise InitNodeException("Logical replication is only "
                                         "available on PostgreSQL 10 and newer")
 
             self.append_conf(
                 max_logical_replication_workers=MAX_LOGICAL_REPLICATION_WORKERS,
                 wal_level='logical')
 
@@ -612,38 +636,70 @@
     def get_control_data(self):
         """
         Return contents of pg_control file.
         """
 
         # this one is tricky (blame PG 9.4)
         _params = [get_bin_path("pg_controldata")]
-        _params += ["-D"] if self._pg_version >= '9.5' else []
+        _params += ["-D"] if self._pg_version >= PgVer('9.5') else []
         _params += [self.data_dir]
 
         data = execute_utility(_params, self.utils_log_file)
 
         out_dict = {}
 
         for line in data.splitlines():
             key, _, value = line.partition(':')
             out_dict[key.strip()] = value.strip()
 
         return out_dict
 
+    def slow_start(self, replica=False, dbname='template1', username=default_username()):
+        """
+        Starts the PostgreSQL instance and then polls the instance
+        until it reaches the expected state (primary or replica). The state is checked
+        using the pg_is_in_recovery() function.
+
+        Args:
+               dbname:
+               username:
+               replica: If True, waits for the instance to be in recovery (i.e., replica mode).
+                        If False, waits for the instance to be in primary mode. Default is False.
+        """
+        self.start()
+
+        if replica:
+            query = 'SELECT pg_is_in_recovery()'
+        else:
+            query = 'SELECT not pg_is_in_recovery()'
+        # Call poll_query_until until the expected value is returned
+        self.poll_query_until(query=query,
+                              dbname=dbname,
+                              username=username,
+                              suppress={InternalError,
+                                        QueryException,
+                                        ProgrammingError,
+                                        OperationalError})
+
     def start(self, params=[], wait=True):
         """
-        Start this node using pg_ctl.
+        Starts the PostgreSQL node using pg_ctl if node has not been started.
+        By default, it waits for the operation to complete before returning.
+        Optionally, it can return immediately without waiting for the start operation
+        to complete by setting the `wait` parameter to False.
 
         Args:
             params: additional arguments for pg_ctl.
             wait: wait until operation completes.
 
         Returns:
             This instance of :class:`.PostgresNode`.
         """
+        if self.is_started:
+            return self
 
         _params = [
             get_bin_path("pg_ctl"),
             "-D", self.data_dir,
             "-l", self.pg_log_file,
             "-w" if wait else '-W',  # --wait or --no-wait
             "start"
@@ -653,42 +709,60 @@
             execute_utility(_params, self.utils_log_file)
         except ExecUtilException as e:
             msg = 'Cannot start node'
             files = self._collect_special_files()
             raise_from(StartNodeException(msg, files), e)
 
         self._maybe_start_logger()
-
+        self.is_started = True
         return self
 
     def stop(self, params=[], wait=True):
         """
-        Stop this node using pg_ctl.
+        Stops the PostgreSQL node using pg_ctl if the node has been started.
 
         Args:
-            params: additional arguments for pg_ctl.
-            wait: wait until operation completes.
+            params: A list of additional arguments for pg_ctl. Defaults to None.
+            wait: If True, waits until the operation is complete. Defaults to True.
 
         Returns:
             This instance of :class:`.PostgresNode`.
         """
+        if not self.is_started:
+            return self
 
         _params = [
             get_bin_path("pg_ctl"),
             "-D", self.data_dir,
             "-w" if wait else '-W',  # --wait or --no-wait
             "stop"
         ] + params  # yapf: disable
 
         execute_utility(_params, self.utils_log_file)
 
         self._maybe_stop_logger()
-
+        self.is_started = False
         return self
 
+    def kill(self, someone=None):
+        """
+            Kills the PostgreSQL node or a specified auxiliary process if the node is running.
+
+            Args:
+                someone: A key to the auxiliary process in the auxiliary_pids dictionary.
+                         If None, the main PostgreSQL node process will be killed. Defaults to None.
+            """
+        if self.is_started:
+            sig = signal.SIGKILL if os.name != 'nt' else signal.SIGBREAK
+            if someone is None:
+                os.kill(self.pid, sig)
+            else:
+                os.kill(self.auxiliary_pids[someone][0], sig)
+            self.is_started = False
+
     def restart(self, params=[]):
         """
         Restart this node using pg_ctl.
 
         Args:
             params: additional arguments for pg_ctl.
 
@@ -754,15 +828,15 @@
             "promote"
         ]  # yapf: disable
 
         execute_utility(_params, self.utils_log_file)
 
         # for versions below 10 `promote` is asynchronous so we need to wait
         # until it actually becomes writable
-        if self._pg_version < '10':
+        if self._pg_version < PgVer('10'):
             check_query = "SELECT pg_is_in_recovery()"
 
             self.poll_query_until(query=check_query,
                                   expected=False,
                                   dbname=dbname,
                                   username=username,
                                   max_attempts=0)    # infinite
@@ -890,37 +964,44 @@
                                    stderr=subprocess.PIPE)
 
         # wait until it finishes and get stdout and stderr
         out, err = process.communicate(input=input)
         return process.returncode, out, err
 
     @method_decorator(positional_args_hack(['dbname', 'query']))
-    def safe_psql(self, query=None, **kwargs):
+    def safe_psql(self, query=None, expect_error=False, **kwargs):
         """
         Execute a query using psql.
 
         Args:
             query: query to be executed.
             filename: file with a query.
             dbname: database name to connect to.
             username: database user name.
             input: raw input to be passed.
+            expect_error: if True - fail if we didn't get ret
+                          if False - fail if we got ret
 
             **kwargs are passed to psql().
 
         Returns:
             psql's output as str.
         """
 
         # force this setting
         kwargs['ON_ERROR_STOP'] = 1
 
         ret, out, err = self.psql(query=query, **kwargs)
         if ret:
-            raise QueryException((err or b'').decode('utf-8'), query)
+            if expect_error:
+                out = (err or b'').decode('utf-8')
+            else:
+                raise QueryException((err or b'').decode('utf-8'), query)
+        elif expect_error:
+            assert False, f"Exception was expected, but query finished successfully: `{query}` "
 
         return out
 
     def dump(self,
              filename=None,
              dbname=None,
              username=None,
@@ -1154,15 +1235,15 @@
             master = get_new_node().init().start()
             with master.replicate().start() as standby:
                 master.append_conf("synchronous_commit = remote_apply")
                 master.set_synchronous_standbys(First(1, [standby]))
                 master.restart()
 
         """
-        if self._pg_version >= '9.6':
+        if self._pg_version >= PgVer('9.6'):
             if isinstance(standbys, Iterable):
                 standbys = First(1, standbys)
         else:
             if isinstance(standbys, Iterable):
                 standbys = u", ".join(u"\"{}\"".format(r.name)
                                       for r in standbys)
             else:
@@ -1175,15 +1256,15 @@
         """
         Wait until async replica catches up with its master.
         """
 
         if not self.master:
             raise TestgresException("Node doesn't have a master")
 
-        if self._pg_version >= '10':
+        if self._pg_version >= PgVer('10'):
             poll_lsn = "select pg_catalog.pg_current_wal_lsn()::text"
             wait_lsn = "select pg_catalog.pg_last_wal_replay_lsn() >= '{}'::pg_lsn"
         else:
             poll_lsn = "select pg_catalog.pg_current_xlog_location()::text"
             wait_lsn = "select pg_catalog.pg_last_xlog_replay_location() >= '{}'::pg_lsn"
 
         try:
@@ -1355,7 +1436,215 @@
         """
 
         return NodeConnection(node=self,
                               dbname=dbname,
                               username=username,
                               password=password,
                               autocommit=autocommit)  # yapf: disable
+
+    def table_checksum(self, table, dbname="postgres"):
+        con = self.connect(dbname=dbname)
+
+        curname = "cur_" + str(random.randint(0, 2 ** 48))
+
+        con.execute("""
+            DECLARE %s NO SCROLL CURSOR FOR
+            SELECT t::text FROM %s as t
+        """ % (curname, table))
+
+        que = Queue(maxsize=50)
+        sum = 0
+
+        rows = con.execute("FETCH FORWARD 2000 FROM %s" % curname)
+        if not rows:
+            return 0
+        que.put(rows)
+
+        th = None
+        if len(rows) == 2000:
+            def querier():
+                try:
+                    while True:
+                        rows = con.execute("FETCH FORWARD 2000 FROM %s" % curname)
+                        if not rows:
+                            break
+                        que.put(rows)
+                except Exception as e:
+                    que.put(e)
+                else:
+                    que.put(None)
+
+            th = threading.Thread(target=querier)
+            th.start()
+        else:
+            que.put(None)
+
+        while True:
+            rows = que.get()
+            if rows is None:
+                break
+            if isinstance(rows, Exception):
+                raise rows
+            # hash uses SipHash since Python3.4, therefore it is good enough
+            for row in rows:
+                sum += hash(row[0])
+
+        if th is not None:
+            th.join()
+
+        con.execute("CLOSE %s; ROLLBACK;" % curname)
+
+        con.close()
+        return sum
+
+    def pgbench_table_checksums(self, dbname="postgres",
+                                pgbench_tables=('pgbench_branches',
+                                                'pgbench_tellers',
+                                                'pgbench_accounts',
+                                                'pgbench_history')
+                                ):
+        return {(table, self.table_checksum(table, dbname))
+                for table in pgbench_tables}
+
+    def set_auto_conf(self, options, config='postgresql.auto.conf', rm_options={}):
+        """
+        Update or remove configuration options in the specified configuration file,
+        updates the options specified in the options dictionary, removes any options
+        specified in the rm_options set, and writes the updated configuration back to
+        the file.
+
+        Args:
+            options (dict): A dictionary containing the options to update or add,
+                            with the option names as keys and their values as values.
+            config (str, optional): The name of the configuration file to update.
+                                     Defaults to 'postgresql.auto.conf'.
+            rm_options (set, optional): A set containing the names of the options to remove.
+                                         Defaults to an empty set.
+        """
+        # parse postgresql.auto.conf
+        path = os.path.join(self.data_dir, config)
+
+        with open(path, 'r') as f:
+            raw_content = f.read()
+
+        current_options = {}
+        current_directives = []
+        for line in raw_content.splitlines():
+
+            # ignore comments
+            if line.startswith('#'):
+                continue
+
+            if line == '':
+                continue
+
+            if line.startswith('include'):
+                current_directives.append(line)
+                continue
+
+            name, var = line.partition('=')[::2]
+            name = name.strip()
+            var = var.strip()
+            var = var.strip('"')
+            var = var.strip("'")
+
+            # remove options specified in rm_options list
+            if name in rm_options:
+                continue
+
+            current_options[name] = var
+
+        for option in options:
+            current_options[option] = options[option]
+
+        auto_conf = ''
+        for option in current_options:
+            auto_conf += "{0} = '{1}'\n".format(
+                option, current_options[option])
+
+        for directive in current_directives:
+            auto_conf += directive + "\n"
+
+        with open(path, 'wt') as f:
+            f.write(auto_conf)
+
+
+class NodeApp:
+
+    def __init__(self, test_path, nodes_to_cleanup):
+        self.test_path = test_path
+        self.nodes_to_cleanup = nodes_to_cleanup
+
+    def make_empty(
+            self,
+            base_dir=None):
+        real_base_dir = os.path.join(self.test_path, base_dir)
+        shutil.rmtree(real_base_dir, ignore_errors=True)
+        os.makedirs(real_base_dir)
+
+        node = PostgresNode(base_dir=real_base_dir)
+        node.should_rm_dirs = True
+        self.nodes_to_cleanup.append(node)
+
+        return node
+
+    def make_simple(
+            self,
+            base_dir=None,
+            set_replication=False,
+            ptrack_enable=False,
+            initdb_params=[],
+            pg_options={}):
+
+        node = self.make_empty(base_dir)
+        node.init(
+            initdb_params=initdb_params, allow_streaming=set_replication)
+
+        # set major version
+        with open(os.path.join(node.data_dir, 'PG_VERSION')) as f:
+            node.major_version_str = str(f.read().rstrip())
+            node.major_version = float(node.major_version_str)
+
+        # Sane default parameters
+        options = {}
+        options['max_connections'] = 100
+        options['shared_buffers'] = '10MB'
+        options['fsync'] = 'off'
+
+        options['wal_level'] = 'logical'
+        options['hot_standby'] = 'off'
+
+        options['log_line_prefix'] = '%t [%p]: [%l-1] '
+        options['log_statement'] = 'none'
+        options['log_duration'] = 'on'
+        options['log_min_duration_statement'] = 0
+        options['log_connections'] = 'on'
+        options['log_disconnections'] = 'on'
+        options['restart_after_crash'] = 'off'
+        options['autovacuum'] = 'off'
+
+        # Allow replication in pg_hba.conf
+        if set_replication:
+            options['max_wal_senders'] = 10
+
+        if ptrack_enable:
+            options['ptrack.map_size'] = '1'
+            options['shared_preload_libraries'] = 'ptrack'
+
+        if node.major_version >= 13:
+            options['wal_keep_size'] = '200MB'
+        else:
+            options['wal_keep_segments'] = '12'
+
+        # set default values
+        node.set_auto_conf(options)
+
+        # Apply given parameters
+        node.set_auto_conf(pg_options)
+
+        # kludge for testgres
+        # https://github.com/postgrespro/testgres/issues/54
+        # for PG >= 13 remove 'wal_keep_segments' parameter
+        if node.major_version >= 13:
+            node.set_auto_conf({}, 'postgresql.conf', ['wal_keep_segments'])
+
+        return node
```

### Comparing `testgres-1.8.5/testgres/pubsub.py` & `testgres-1.8.6/testgres/pubsub.py`

 * *Files identical despite different names*

### Comparing `testgres-1.8.5/testgres/standby.py` & `testgres-1.8.6/testgres/standby.py`

 * *Files identical despite different names*

### Comparing `testgres-1.8.5/testgres/utils.py` & `testgres-1.8.6/testgres/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,29 +7,29 @@
 import os
 import port_for
 import subprocess
 import sys
 import tempfile
 
 from contextlib import contextmanager
-from distutils.version import LooseVersion
+from packaging.version import Version
 from distutils.spawn import find_executable
 from six import iteritems
 
 from .config import testgres_config
 from .exceptions import ExecUtilException
 
 # rows returned by PG_CONFIG
 _pg_config_data = {}
 
 # ports used by nodes
 bound_ports = set()
 
 # re-export version type
-PgVer = LooseVersion
+PgVer = Version
 
 
 def reserve_port():
     """
     Generate a new port and add it to 'bound_ports'.
     """
```

### Comparing `testgres-1.8.5/testgres.egg-info/PKG-INFO` & `testgres-1.8.6/testgres.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 Metadata-Version: 2.1
 Name: testgres
-Version: 1.8.5
+Version: 1.8.6
 Summary: Testing utility for PostgreSQL and its extensions
 Home-page: https://github.com/postgrespro/testgres
 Author: Ildar Musin
 Author-email: zildermann@gmail.com
 License: PostgreSQL
 Keywords: test,testing,postgresql
+Platform: UNKNOWN
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-[![Build Status](https://travis-ci.org/postgrespro/testgres.svg?branch=master)](https://travis-ci.org/postgrespro/testgres)
+[![Build Status](https://travis-ci.com/postgrespro/testgres.svg?branch=master)](https://app.travis-ci.com/github/postgrespro/testgres/branches)
 [![codecov](https://codecov.io/gh/postgrespro/testgres/branch/master/graph/badge.svg)](https://codecov.io/gh/postgrespro/testgres)
 [![PyPI version](https://badge.fury.io/py/testgres.svg)](https://badge.fury.io/py/testgres)
 
 [Documentation](https://postgrespro.github.io/testgres/)
 
 # testgres
 
@@ -188,7 +189,9 @@
 
 ## Authors
 
 [Ildar Musin](https://github.com/zilder)  
 [Dmitry Ivanov](https://github.com/funbringer)  
 [Ildus Kurbangaliev](https://github.com/ildus)  
 [Yury Zhuravlev](https://github.com/stalkerg)  
+
+
```

### Comparing `testgres-1.8.5/testgres.egg-info/SOURCES.txt` & `testgres-1.8.6/testgres.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `testgres-1.8.5/tests/test_simple.py` & `testgres-1.8.6/tests/test_simple.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 import re
 import subprocess
 import tempfile
 import testgres
 import time
 import six
 import unittest
+import psutil
 
 import logging.config
 
 from contextlib import contextmanager
 from shutil import rmtree
 
 from testgres import \
@@ -44,14 +45,15 @@
 from testgres import \
     First, \
     Any
 
 # NOTE: those are ugly imports
 from testgres import bound_ports
 from testgres.utils import PgVer
+from testgres.node import ProcessProxy
 
 
 def pg_version_ge(version):
     cur_ver = PgVer(get_pg_version())
     min_ver = PgVer(version)
     return cur_ver >= min_ver
 
@@ -165,16 +167,16 @@
 
         # should have been removed by default
         self.assertFalse(os.path.exists(base_dir))
 
     def test_double_start(self):
         with get_new_node().init().start() as node:
             # can't start node more than once
-            with self.assertRaises(StartNodeException):
-                node.start()
+            node.start()
+            self.assertTrue(node.is_started)
 
     def test_uninitialized_start(self):
         with get_new_node() as node:
             # node is not initialized yet
             with self.assertRaises(StartNodeException):
                 node.start()
 
@@ -892,24 +894,30 @@
         str(ExecUtilException('msg', 'cmd', 1, 'out'))
         str(QueryException('msg', 'query'))
 
     def test_version_management(self):
         a = PgVer('10.0')
         b = PgVer('10')
         c = PgVer('9.6.5')
+        d = PgVer('15.0')
+        e = PgVer('15rc1')
+        f = PgVer('15beta4')
 
-        self.assertTrue(a > b)
+        self.assertTrue(a == b)
         self.assertTrue(b > c)
         self.assertTrue(a > c)
+        self.assertTrue(d > e)
+        self.assertTrue(e > f)
+        self.assertTrue(d > f)
 
         version = get_pg_version()
         with get_new_node() as node:
             self.assertTrue(isinstance(version, six.string_types))
             self.assertTrue(isinstance(node.version, PgVer))
-            self.assertEqual(node.version, str(version))
+            self.assertEqual(node.version, PgVer(version))
 
     def test_child_pids(self):
         master_processes = [
             ProcessType.AutovacuumLauncher,
             ProcessType.BackgroundWriter,
             ProcessType.Checkpointer,
             ProcessType.StatsCollector,
@@ -955,14 +963,26 @@
 
                 replica.stop()
 
                 # there should be no walsender after we've stopped replica
                 with self.assertRaises(TestgresException):
                     replica.source_walsender
 
+    def test_child_process_dies(self):
+        # test for FileNotFound exception during child_processes() function
+        with subprocess.Popen(["sleep", "60"]) as process:
+            self.assertEqual(process.poll(), None)
+            # collect list of processes currently running
+            children = psutil.Process(os.getpid()).children()
+            # kill a process, so received children dictionary becomes invalid
+            process.kill()
+            process.wait()
+            # try to handle children list -- missing processes will have ptype "ProcessType.Unknown"
+            [ProcessProxy(p) for p in children]
+
 
 if __name__ == '__main__':
     if os.environ.get('ALT_CONFIG'):
         suite = unittest.TestSuite()
 
         # Small subset of tests for alternative configs (PG_BIN or PG_CONFIG)
         suite.addTest(TestgresTests('test_pg_config'))
```

