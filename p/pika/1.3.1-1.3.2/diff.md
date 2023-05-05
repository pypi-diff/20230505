# Comparing `tmp/pika-1.3.1.tar.gz` & `tmp/pika-1.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pika-1.3.1.tar", last modified: Tue Oct 18 23:16:13 2022, max compression
+gzip compressed data, was "pika-1.3.2.tar", last modified: Fri May  5 14:25:29 2023, max compression
```

## Comparing `pika-1.3.1.tar` & `pika-1.3.2.tar`

### file list

```diff
@@ -1,47 +1,47 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-18 23:16:13.346786 pika-1.3.1/
--rw-r--r--   0 runner    (1001) docker     (121)     1552 2022-10-18 23:15:57.000000 pika-1.3.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)       34 2022-10-18 23:15:57.000000 pika-1.3.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)    13019 2022-10-18 23:16:13.346786 pika-1.3.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)    11476 2022-10-18 23:15:57.000000 pika-1.3.1/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-18 23:16:13.342786 pika-1.3.1/pika/
--rw-r--r--   0 runner    (1001) docker     (121)      693 2022-10-18 23:15:57.000000 pika-1.3.1/pika/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-18 23:16:13.346786 pika-1.3.1/pika/adapters/
--rw-r--r--   0 runner    (1001) docker     (121)      994 2022-10-18 23:15:57.000000 pika-1.3.1/pika/adapters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     9234 2022-10-18 23:15:57.000000 pika-1.3.1/pika/adapters/asyncio_connection.py
--rw-r--r--   0 runner    (1001) docker     (121)    20525 2022-10-18 23:15:57.000000 pika-1.3.1/pika/adapters/base_connection.py
--rw-r--r--   0 runner    (1001) docker     (121)   110260 2022-10-18 23:15:57.000000 pika-1.3.1/pika/adapters/blocking_connection.py
--rw-r--r--   0 runner    (1001) docker     (121)    16734 2022-10-18 23:15:57.000000 pika-1.3.1/pika/adapters/gevent_connection.py
--rw-r--r--   0 runner    (1001) docker     (121)    45161 2022-10-18 23:15:57.000000 pika-1.3.1/pika/adapters/select_connection.py
--rw-r--r--   0 runner    (1001) docker     (121)     3558 2022-10-18 23:15:57.000000 pika-1.3.1/pika/adapters/tornado_connection.py
--rw-r--r--   0 runner    (1001) docker     (121)    50292 2022-10-18 23:15:57.000000 pika-1.3.1/pika/adapters/twisted_connection.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-18 23:16:13.346786 pika-1.3.1/pika/adapters/utils/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-18 23:15:57.000000 pika-1.3.1/pika/adapters/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    33845 2022-10-18 23:15:57.000000 pika-1.3.1/pika/adapters/utils/connection_workflow.py
--rwxr-xr-x   0 runner    (1001) docker     (121)    53574 2022-10-18 23:15:57.000000 pika-1.3.1/pika/adapters/utils/io_services_utils.py
--rw-r--r--   0 runner    (1001) docker     (121)    17217 2022-10-18 23:15:57.000000 pika-1.3.1/pika/adapters/utils/nbio_interface.py
--rwxr-xr-x   0 runner    (1001) docker     (121)    19955 2022-10-18 23:15:57.000000 pika-1.3.1/pika/adapters/utils/selector_ioloop_adapter.py
--rw-r--r--   0 runner    (1001) docker     (121)     1830 2022-10-18 23:15:57.000000 pika-1.3.1/pika/amqp_object.py
--rw-r--r--   0 runner    (1001) docker     (121)    14743 2022-10-18 23:15:57.000000 pika-1.3.1/pika/callback.py
--rw-r--r--   0 runner    (1001) docker     (121)    63124 2022-10-18 23:15:57.000000 pika-1.3.1/pika/channel.py
--rw-r--r--   0 runner    (1001) docker     (121)     7221 2022-10-18 23:15:57.000000 pika-1.3.1/pika/compat.py
--rw-r--r--   0 runner    (1001) docker     (121)    87633 2022-10-18 23:15:57.000000 pika-1.3.1/pika/connection.py
--rw-r--r--   0 runner    (1001) docker     (121)     4646 2022-10-18 23:15:57.000000 pika-1.3.1/pika/credentials.py
--rw-r--r--   0 runner    (1001) docker     (121)     9956 2022-10-18 23:15:57.000000 pika-1.3.1/pika/data.py
--rw-r--r--   0 runner    (1001) docker     (121)       87 2022-10-18 23:15:57.000000 pika-1.3.1/pika/delivery_mode.py
--rw-r--r--   0 runner    (1001) docker     (121)     1759 2022-10-18 23:15:57.000000 pika-1.3.1/pika/diagnostic_utils.py
--rw-r--r--   0 runner    (1001) docker     (121)    10117 2022-10-18 23:15:57.000000 pika-1.3.1/pika/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (121)      139 2022-10-18 23:15:57.000000 pika-1.3.1/pika/exchange_type.py
--rw-r--r--   0 runner    (1001) docker     (121)     7744 2022-10-18 23:15:57.000000 pika-1.3.1/pika/frame.py
--rw-r--r--   0 runner    (1001) docker     (121)     8170 2022-10-18 23:15:57.000000 pika-1.3.1/pika/heartbeat.py
--rw-r--r--   0 runner    (1001) docker     (121)    80449 2022-10-18 23:15:57.000000 pika-1.3.1/pika/spec.py
--rw-r--r--   0 runner    (1001) docker     (121)     1513 2022-10-18 23:15:57.000000 pika-1.3.1/pika/tcp_socket_opts.py
--rw-r--r--   0 runner    (1001) docker     (121)     1419 2022-10-18 23:15:57.000000 pika-1.3.1/pika/validators.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-18 23:16:13.346786 pika-1.3.1/pika.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)    13019 2022-10-18 23:16:13.000000 pika-1.3.1/pika.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      995 2022-10-18 23:16:13.000000 pika-1.3.1/pika.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-10-18 23:16:13.000000 pika-1.3.1/pika.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       55 2022-10-18 23:16:13.000000 pika-1.3.1/pika.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        5 2022-10-18 23:16:13.000000 pika-1.3.1/pika.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-10-18 23:16:13.000000 pika-1.3.1/pika.egg-info/zip-safe
--rw-r--r--   0 runner    (1001) docker     (121)     1840 2022-10-18 23:15:57.000000 pika-1.3.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-10-18 23:16:13.346786 pika-1.3.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 14:25:29.788974 pika-1.3.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1552 2023-05-05 14:25:12.000000 pika-1.3.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-05-05 14:25:12.000000 pika-1.3.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    12922 2023-05-05 14:25:29.788974 pika-1.3.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    11478 2023-05-05 14:25:12.000000 pika-1.3.2/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 14:25:29.784974 pika-1.3.2/pika/
+-rw-r--r--   0 runner    (1001) docker     (123)      693 2023-05-05 14:25:12.000000 pika-1.3.2/pika/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 14:25:29.784974 pika-1.3.2/pika/adapters/
+-rw-r--r--   0 runner    (1001) docker     (123)      994 2023-05-05 14:25:12.000000 pika-1.3.2/pika/adapters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9235 2023-05-05 14:25:12.000000 pika-1.3.2/pika/adapters/asyncio_connection.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20525 2023-05-05 14:25:12.000000 pika-1.3.2/pika/adapters/base_connection.py
+-rw-r--r--   0 runner    (1001) docker     (123)   110248 2023-05-05 14:25:12.000000 pika-1.3.2/pika/adapters/blocking_connection.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16735 2023-05-05 14:25:12.000000 pika-1.3.2/pika/adapters/gevent_connection.py
+-rw-r--r--   0 runner    (1001) docker     (123)    45162 2023-05-05 14:25:12.000000 pika-1.3.2/pika/adapters/select_connection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3559 2023-05-05 14:25:12.000000 pika-1.3.2/pika/adapters/tornado_connection.py
+-rw-r--r--   0 runner    (1001) docker     (123)    50294 2023-05-05 14:25:12.000000 pika-1.3.2/pika/adapters/twisted_connection.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 14:25:29.788974 pika-1.3.2/pika/adapters/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 14:25:12.000000 pika-1.3.2/pika/adapters/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    33845 2023-05-05 14:25:12.000000 pika-1.3.2/pika/adapters/utils/connection_workflow.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    53574 2023-05-05 14:25:12.000000 pika-1.3.2/pika/adapters/utils/io_services_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17217 2023-05-05 14:25:12.000000 pika-1.3.2/pika/adapters/utils/nbio_interface.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    19955 2023-05-05 14:25:12.000000 pika-1.3.2/pika/adapters/utils/selector_ioloop_adapter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1830 2023-05-05 14:25:12.000000 pika-1.3.2/pika/amqp_object.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14743 2023-05-05 14:25:12.000000 pika-1.3.2/pika/callback.py
+-rw-r--r--   0 runner    (1001) docker     (123)    63112 2023-05-05 14:25:12.000000 pika-1.3.2/pika/channel.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7221 2023-05-05 14:25:12.000000 pika-1.3.2/pika/compat.py
+-rw-r--r--   0 runner    (1001) docker     (123)    87627 2023-05-05 14:25:12.000000 pika-1.3.2/pika/connection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4646 2023-05-05 14:25:12.000000 pika-1.3.2/pika/credentials.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9956 2023-05-05 14:25:12.000000 pika-1.3.2/pika/data.py
+-rw-r--r--   0 runner    (1001) docker     (123)       87 2023-05-05 14:25:12.000000 pika-1.3.2/pika/delivery_mode.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1759 2023-05-05 14:25:12.000000 pika-1.3.2/pika/diagnostic_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10117 2023-05-05 14:25:12.000000 pika-1.3.2/pika/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      390 2023-05-05 14:25:12.000000 pika-1.3.2/pika/exchange_type.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7744 2023-05-05 14:25:12.000000 pika-1.3.2/pika/frame.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8170 2023-05-05 14:25:12.000000 pika-1.3.2/pika/heartbeat.py
+-rw-r--r--   0 runner    (1001) docker     (123)    80448 2023-05-05 14:25:12.000000 pika-1.3.2/pika/spec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1513 2023-05-05 14:25:12.000000 pika-1.3.2/pika/tcp_socket_opts.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1419 2023-05-05 14:25:12.000000 pika-1.3.2/pika/validators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 14:25:29.784974 pika-1.3.2/pika.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    12922 2023-05-05 14:25:29.000000 pika-1.3.2/pika.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      995 2023-05-05 14:25:29.000000 pika-1.3.2/pika.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 14:25:29.000000 pika-1.3.2/pika.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-05 14:25:29.000000 pika-1.3.2/pika.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-05-05 14:25:29.000000 pika-1.3.2/pika.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 14:25:29.000000 pika-1.3.2/pika.egg-info/zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)     1767 2023-05-05 14:25:12.000000 pika-1.3.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-05 14:25:29.788974 pika-1.3.2/setup.cfg
```

### Comparing `pika-1.3.1/LICENSE` & `pika-1.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pika-1.3.1/PKG-INFO` & `pika-1.3.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,37 +1,35 @@
 Metadata-Version: 2.1
 Name: pika
-Version: 1.3.1
+Version: 1.3.2
 Summary: Pika Python AMQP Client Library
 Maintainer-email: "Gavin M. Roy" <gavinmroy@gmail.com>, Luke Bakken <lukerbakken@gmail.com>
 License: BSD-3-Clause
 Project-URL: Homepage, https://pika.readthedocs.io
 Project-URL: Source, https://github.com/pika/pika
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.4
-Classifier: Programming Language :: Python :: 3.5
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: Jython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Topic :: Communications
 Classifier: Topic :: Internet
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: System :: Networking
-Requires-Python: >=3.4
+Requires-Python: >=3.7
 Description-Content-Type: text/x-rst
 Provides-Extra: gevent
 Provides-Extra: tornado
 Provides-Extra: twisted
 License-File: LICENSE
 
 Pika
@@ -41,15 +39,15 @@
 |Version| |Python versions| |Actions Status| |Coverage| |License| |Docs|
 
 Introduction
 ------------
 Pika is a pure-Python implementation of the AMQP 0-9-1 protocol including
 RabbitMQ's extensions.
 
-- Supports Python 3.4+ (`1.1.0` was the last version to support 2.7)
+- Supports Python 3.7+ (`1.1.0` was the last version to support 2.7)
 - Since threads aren't appropriate to every situation, it doesn't require
   threads. Pika core takes care not to forbid them, either. The same goes for
   greenlets, callbacks, continuations, and generators. An instance of Pika's
   built-in connection adapters isn't thread-safe, however.
 - People may be using direct sockets, plain old ``select()``, or any of the
   wide variety of ways of getting network events to and from a Python
   application. Pika tries to stay compatible with all of these, and to make
@@ -195,15 +193,15 @@
 publishing of messages, etc., from a background thread to the connection
 adapter's thread.
 
 Connection recovery
 -------------------
 
 Some RabbitMQ clients (Bunny, Java, .NET, Objective-C, Swift) provide a way to
-automatically recover connection, its channels and topology (e.g. queues,
+automatically recover a connection, its channels and topology (e.g. queues,
 bindings and consumers) after a network failure. Others require connection
 recovery to be performed by the application code and strive to make it a
 straightforward process. Pika falls into the second category.
 
 Pika supports multiple connection adapters. They take different approaches to
 connection recovery.
```

### Comparing `pika-1.3.1/README.rst` & `pika-1.3.2/README.rst`

 * *Files 0% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 |Version| |Python versions| |Actions Status| |Coverage| |License| |Docs|
 
 Introduction
 ------------
 Pika is a pure-Python implementation of the AMQP 0-9-1 protocol including
 RabbitMQ's extensions.
 
-- Supports Python 3.4+ (`1.1.0` was the last version to support 2.7)
+- Supports Python 3.7+ (`1.1.0` was the last version to support 2.7)
 - Since threads aren't appropriate to every situation, it doesn't require
   threads. Pika core takes care not to forbid them, either. The same goes for
   greenlets, callbacks, continuations, and generators. An instance of Pika's
   built-in connection adapters isn't thread-safe, however.
 - People may be using direct sockets, plain old ``select()``, or any of the
   wide variety of ways of getting network events to and from a Python
   application. Pika tries to stay compatible with all of these, and to make
@@ -159,15 +159,15 @@
 publishing of messages, etc., from a background thread to the connection
 adapter's thread.
 
 Connection recovery
 -------------------
 
 Some RabbitMQ clients (Bunny, Java, .NET, Objective-C, Swift) provide a way to
-automatically recover connection, its channels and topology (e.g. queues,
+automatically recover a connection, its channels and topology (e.g. queues,
 bindings and consumers) after a network failure. Others require connection
 recovery to be performed by the application code and strive to make it a
 straightforward process. Pika falls into the second category.
 
 Pika supports multiple connection adapters. They take different approaches to
 connection recovery.
```

### Comparing `pika-1.3.1/pika/__init__.py` & `pika-1.3.2/pika/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-__version__ = '1.3.1'
+__version__ = '1.3.2'
 
 import logging
 
 # Add NullHandler before importing Pika modules to prevent logging warnings
 logging.getLogger(__name__).addHandler(logging.NullHandler())
 
 # pylint: disable=C0413
```

### Comparing `pika-1.3.1/pika/adapters/__init__.py` & `pika-1.3.2/pika/adapters/__init__.py`

 * *Files identical despite different names*

### Comparing `pika-1.3.1/pika/adapters/asyncio_connection.py` & `pika-1.3.2/pika/adapters/asyncio_connection.py`

 * *Files 0% similar despite different names*

```diff
@@ -65,15 +65,15 @@
     @classmethod
     def create_connection(cls,
                           connection_configs,
                           on_done,
                           custom_ioloop=None,
                           workflow=None):
         """Implement
-        :py:classmethod:`pika.adapters.BaseConnection.create_connection()`.
+        :py:classmethod::`pika.adapters.BaseConnection.create_connection()`.
 
         """
         nbio = _AsyncioIOServicesAdapter(custom_ioloop)
 
         def connection_factory(params):
             """Connection factory."""
             if params is None:
```

### Comparing `pika-1.3.1/pika/adapters/base_connection.py` & `pika-1.3.2/pika/adapters/base_connection.py`

 * *Files identical despite different names*

### Comparing `pika-1.3.1/pika/adapters/blocking_connection.py` & `pika-1.3.2/pika/adapters/blocking_connection.py`

 * *Files 0% similar despite different names*

```diff
@@ -666,15 +666,15 @@
         """RabbitMQ AMQP extension - Add a callback to be notified when the
         connection gets unblocked (`Connection.Unblocked` frame is received from
         RabbitMQ) letting publishers know it's ok to start publishing again.
 
         :param callable callback: Callback to call on Connection.Unblocked`,
             having the signature `callback(connection, pika.frame.Method)`,
             where connection is the `BlockingConnection` instance and the method
-             frame's `method` member is of type `pika.spec.Connection.Unblocked`
+            frame's `method` member is of type `pika.spec.Connection.Unblocked`
 
         """
         self._impl.add_on_connection_unblocked_callback(
             functools.partial(self._on_connection_unblocked,
                               functools.partial(callback, self)))
 
     def call_later(self, delay, callback):
@@ -1582,18 +1582,18 @@
 
     def add_on_return_callback(self, callback):
         """Pass a callback function that will be called when a published
         message is rejected and returned by the server via `Basic.Return`.
 
         :param callable callback: The method to call on callback with the
             signature callback(channel, method, properties, body), where
-             - channel: pika.Channel
-             - method: pika.spec.Basic.Return
-             - properties: pika.spec.BasicProperties
-             - body: bytes
+            - channel: pika.Channel
+            - method: pika.spec.Basic.Return
+            - properties: pika.spec.BasicProperties
+            - body: bytes
 
         """
         self._impl.add_on_return_callback(
             lambda _channel, method, properties, body: (
                 self._add_pending_event(
                     _ReturnedMessageEvt(
                         callback, self, method, properties, body))))
@@ -1618,18 +1618,18 @@
         For more information about Basic.Consume, see:
         http://www.rabbitmq.com/amqp-0-9-1-reference.html#basic.consume
 
         :param str queue: The queue from which to consume
         :param callable on_message_callback: Required function for dispatching messages
             to user, having the signature:
             on_message_callback(channel, method, properties, body)
-             - channel: BlockingChannel
-             - method: spec.Basic.Deliver
-             - properties: spec.BasicProperties
-             - body: bytes
+            - channel: BlockingChannel
+            - method: spec.Basic.Deliver
+            - properties: spec.BasicProperties
+            - body: bytes
         :param bool auto_ack: if set to True, automatic acknowledgement mode will be used
                               (see http://www.rabbitmq.com/confirms.html). This corresponds
                               with the 'no_ack' parameter in the basic.consume AMQP 0.9.1
                               method
         :param bool exclusive: Don't allow other consumers on the queue
         :param str consumer_tag: You may specify your own consumer tag; if left
           empty, a consumer tag will be generated automatically
@@ -1746,18 +1746,18 @@
             undefined (bad things will happen)
         :returns: (NEW IN pika 0.10.0) empty sequence for a auto_ack=False
             consumer; for a auto_ack=True consumer, returns a (possibly empty)
             sequence of pending messages that arrived before broker confirmed
             the cancellation (this is done instead of via consumer's callback in
             order to prevent reentrancy/recursion. Each message is four-tuple:
             (channel, method, properties, body)
-             - channel: BlockingChannel
-             - method: spec.Basic.Deliver
-             - properties: spec.BasicProperties
-             - body: bytes
+            - channel: BlockingChannel
+            - method: spec.Basic.Deliver
+            - properties: spec.BasicProperties
+            - body: bytes
         :rtype: list
         """
         try:
             consumer_info = self._consumer_infos[consumer_tag]
         except KeyError:
             LOGGER.warning(
                 "User is attempting to cancel an unknown consumer=%s; "
@@ -1906,15 +1906,15 @@
         properties, and body. The active generator iterator terminates when the
         consumer is cancelled by client via `BlockingChannel.cancel()` or by
         broker.
 
         Example:
         ::
             for method, properties, body in channel.consume('queue'):
-                print body
+                print(body)
                 channel.basic_ack(method.delivery_tag)
 
         You should call `BlockingChannel.cancel()` when you escape out of the
         generator loop.
 
         If you don't cancel this consumer, then next call on the same channel
         to `consume()` with the exact same (queue, auto_ack, exclusive) parameters
```

### Comparing `pika-1.3.1/pika/adapters/gevent_connection.py` & `pika-1.3.2/pika/adapters/gevent_connection.py`

 * *Files 0% similar despite different names*

```diff
@@ -88,15 +88,15 @@
     @classmethod
     def create_connection(cls,
                           connection_configs,
                           on_done,
                           custom_ioloop=None,
                           workflow=None):
         """Implement
-        :py:classmethod:`pika.adapters.BaseConnection.create_connection()`.
+        :py:classmethod::`pika.adapters.BaseConnection.create_connection()`.
         """
         custom_ioloop = (custom_ioloop or
                          _GeventSelectorIOLoop(gevent.get_hub()))
 
         nbio = _GeventSelectorIOServicesAdapter(custom_ioloop)
 
         def connection_factory(params):
```

### Comparing `pika-1.3.1/pika/adapters/select_connection.py` & `pika-1.3.2/pika/adapters/select_connection.py`

 * *Files 0% similar despite different names*

```diff
@@ -109,15 +109,15 @@
     @classmethod
     def create_connection(cls,
                           connection_configs,
                           on_done,
                           custom_ioloop=None,
                           workflow=None):
         """Implement
-        :py:classmethod:`pika.adapters.BaseConnection.create_connection()`.
+        :py:classmethod::`pika.adapters.BaseConnection.create_connection()`.
 
         """
         nbio = SelectorIOServicesAdapter(custom_ioloop or IOLoop())
 
         def connection_factory(params):
             """Connection factory."""
             if params is None:
```

### Comparing `pika-1.3.1/pika/adapters/tornado_connection.py` & `pika-1.3.2/pika/adapters/tornado_connection.py`

 * *Files 0% similar despite different names*

```diff
@@ -62,15 +62,15 @@
     @classmethod
     def create_connection(cls,
                           connection_configs,
                           on_done,
                           custom_ioloop=None,
                           workflow=None):
         """Implement
-        :py:classmethod:`pika.adapters.BaseConnection.create_connection()`.
+        :py:classmethod::`pika.adapters.BaseConnection.create_connection()`.
 
         """
         nbio = selector_ioloop_adapter.SelectorIOServicesAdapter(
             custom_ioloop or ioloop.IOLoop.instance())
 
         def connection_factory(params):
             """Connection factory."""
```

### Comparing `pika-1.3.1/pika/adapters/twisted_connection.py` & `pika-1.3.2/pika/adapters/twisted_connection.py`

 * *Files 0% similar despite different names*

```diff
@@ -299,20 +299,19 @@
 
     def add_on_return_callback(self, callback):
         """Pass a callback function that will be called when a published
         message is rejected and returned by the server via `Basic.Return`.
 
         :param callable callback: The method to call on callback with the
             message as only argument. The message is a named tuple with
-            the following attributes:
-            channel: this TwistedChannel
-            method: pika.spec.Basic.Return
-            properties: pika.spec.BasicProperties
-            body: bytes
-
+            the following attributes
+            - channel: this TwistedChannel
+            - method: pika.spec.Basic.Return
+            - properties: pika.spec.BasicProperties
+            - body: bytes
         """
         self._channel.add_on_return_callback(
             lambda _channel, method, properties, body: callback(
                 ReceivedMessage(
                     channel=self,
                     method=method,
                     properties=properties,
@@ -398,18 +397,18 @@
             ``(queue_object, consumer_tag)``. The Deferred will errback with an
             instance of :class:`exceptions.ChannelClosed` if the call fails.
             The queue object is an instance of :class:`ClosableDeferredQueue`,
             where data received from the queue will be stored. Clients should
             use its :meth:`get() <ClosableDeferredQueue.get>` method to fetch
             an individual message, which will return a Deferred firing with a
             namedtuple whose attributes are:
-             - channel: this TwistedChannel
-             - method: pika.spec.Basic.Deliver
-             - properties: pika.spec.BasicProperties
-             - body: bytes
+            - channel: this TwistedChannel
+            - method: pika.spec.Basic.Deliver
+            - properties: pika.spec.BasicProperties
+            - body: bytes
         :rtype: Deferred
 
         """
         if self._closed:
             return defer.fail(self._closed)
 
         queue_obj = ClosableDeferredQueue()
```

### Comparing `pika-1.3.1/pika/adapters/utils/connection_workflow.py` & `pika-1.3.2/pika/adapters/utils/connection_workflow.py`

 * *Files identical despite different names*

### Comparing `pika-1.3.1/pika/adapters/utils/io_services_utils.py` & `pika-1.3.2/pika/adapters/utils/io_services_utils.py`

 * *Files identical despite different names*

### Comparing `pika-1.3.1/pika/adapters/utils/nbio_interface.py` & `pika-1.3.2/pika/adapters/utils/nbio_interface.py`

 * *Files identical despite different names*

### Comparing `pika-1.3.1/pika/adapters/utils/selector_ioloop_adapter.py` & `pika-1.3.2/pika/adapters/utils/selector_ioloop_adapter.py`

 * *Files identical despite different names*

### Comparing `pika-1.3.1/pika/amqp_object.py` & `pika-1.3.2/pika/amqp_object.py`

 * *Files identical despite different names*

### Comparing `pika-1.3.1/pika/callback.py` & `pika-1.3.2/pika/callback.py`

 * *Files identical despite different names*

### Comparing `pika-1.3.1/pika/channel.py` & `pika-1.3.2/pika/channel.py`

 * *Files 0% similar despite different names*

```diff
@@ -170,18 +170,18 @@
     def add_on_return_callback(self, callback):
         """Pass a callback function that will be called when basic_publish is
         sent a message that has been rejected and returned by the server.
 
         :param callable callback: The function to call, having the signature
                                 callback(channel, method, properties, body)
                                 where
-                                 - channel: pika.channel.Channel
-                                 - method: pika.spec.Basic.Return
-                                 - properties: pika.spec.BasicProperties
-                                 - body: bytes
+                                - channel: pika.channel.Channel
+                                - method: pika.spec.Basic.Return
+                                - properties: pika.spec.BasicProperties
+                                - body: bytes
 
         """
         self.callbacks.add(self.channel_number, '_on_return', callback, False)
 
     def basic_ack(self, delivery_tag=0, multiple=False):
         """Acknowledge one or more messages. When sent by the client, this
         method acknowledges one or more messages delivered via the Deliver or
@@ -280,18 +280,18 @@
         http://www.rabbitmq.com/amqp-0-9-1-reference.html#basic.consume
 
         :param str queue: The queue to consume from. Use the empty string to
             specify the most recent server-named queue for this channel
         :param callable on_message_callback: The function to call when
             consuming with the signature
             on_message_callback(channel, method, properties, body), where
-             - channel: pika.channel.Channel
-             - method: pika.spec.Basic.Deliver
-             - properties: pika.spec.BasicProperties
-             - body: bytes
+            - channel: pika.channel.Channel
+            - method: pika.spec.Basic.Deliver
+            - properties: pika.spec.BasicProperties
+            - body: bytes
         :param bool auto_ack: if set to True, automatic acknowledgement mode
             will be used (see http://www.rabbitmq.com/confirms.html).
             This corresponds with the 'no_ack' parameter in the basic.consume
             AMQP 0.9.1 method
         :param bool exclusive: Don't allow other consumers on the queue
         :param str consumer_tag: Specify your own consumer tag
         :param dict arguments: Custom key/value pair arguments for the consumer
@@ -355,18 +355,18 @@
         http://www.rabbitmq.com/amqp-0-9-1-reference.html#basic.get
 
         :param str queue: The queue from which to get a message. Use the empty
             string to specify the most recent server-named queue for this
             channel
         :param callable callback: The callback to call with a message that has
             the signature callback(channel, method, properties, body), where:
-             - channel: pika.channel.Channel
-             - method: pika.spec.Basic.GetOk
-             - properties: pika.spec.BasicProperties
-             - body: bytes
+            - channel: pika.channel.Channel
+            - method: pika.spec.Basic.GetOk
+            - properties: pika.spec.BasicProperties
+            - body: bytes
         :param bool auto_ack: Tell the broker to not expect a reply
         :raises ValueError:
 
         """
         validators.require_string(queue, 'queue')
         validators.require_callback(callback)
         if self._on_getok_callback is not None:
```

### Comparing `pika-1.3.1/pika/compat.py` & `pika-1.3.2/pika/compat.py`

 * *Files identical despite different names*

### Comparing `pika-1.3.1/pika/connection.py` & `pika-1.3.2/pika/connection.py`

 * *Files 0% similar despite different names*

```diff
@@ -529,17 +529,15 @@
             raise TypeError(
                 'tcp_options must be a dict or None, but got %r' % (value,))
         self._tcp_options = value
 
 
 class ConnectionParameters(Parameters):
     """Connection parameters object that is passed into the connection adapter
-    upon construction.
-
-    """
+    upon construction."""
 
     # Protect against accidental assignment of an invalid attribute
     __slots__ = ()
 
     class _DEFAULT(object):
         """Designates default parameter value; internal use"""
 
@@ -887,16 +885,16 @@
         """Deserialize and apply the corresponding query string arg
 
         """
         opts = ast.literal_eval(value)
         if opts is None:
             if self.ssl_options is not None:
                 raise ValueError(
-                    'Specified ssl_options=None URL arg is inconsistent with '
-                    'the specified https URL scheme.')
+                    'Specified ssl_options=None URI arg is inconsistent with '
+                    'the specified amqps URI scheme.')
         else:
             # Older versions of Pika would take the opts dict and pass it
             # directly as kwargs to the deprecated ssl.wrap_socket method.
             # Here, we take the valid options and translate them into args
             # for various SSLContext methods.
             #
             # https://docs.python.org/3/library/ssl.html#ssl.wrap_socket
```

### Comparing `pika-1.3.1/pika/credentials.py` & `pika-1.3.2/pika/credentials.py`

 * *Files identical despite different names*

### Comparing `pika-1.3.1/pika/data.py` & `pika-1.3.2/pika/data.py`

 * *Files identical despite different names*

### Comparing `pika-1.3.1/pika/diagnostic_utils.py` & `pika-1.3.2/pika/diagnostic_utils.py`

 * *Files identical despite different names*

### Comparing `pika-1.3.1/pika/exceptions.py` & `pika-1.3.2/pika/exceptions.py`

 * *Files identical despite different names*

### Comparing `pika-1.3.1/pika/frame.py` & `pika-1.3.2/pika/frame.py`

 * *Files identical despite different names*

### Comparing `pika-1.3.1/pika/heartbeat.py` & `pika-1.3.2/pika/heartbeat.py`

 * *Files identical despite different names*

### Comparing `pika-1.3.1/pika/spec.py` & `pika-1.3.2/pika/spec.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,13 @@
 """
 AMQP Specification
 ==================
 This module implements the constants and classes that comprise AMQP protocol
 level constructs. It should rarely be directly referenced outside of Pika's
 own internal use.
-
 .. note:: Auto-generated code by codegen.py, do not edit directly. Pull
 requests to this file without accompanying ``utils/codegen.py`` changes will be
 rejected.
 
 """
 
 import struct
```

### Comparing `pika-1.3.1/pika/tcp_socket_opts.py` & `pika-1.3.2/pika/tcp_socket_opts.py`

 * *Files identical despite different names*

### Comparing `pika-1.3.1/pika/validators.py` & `pika-1.3.2/pika/validators.py`

 * *Files identical despite different names*

### Comparing `pika-1.3.1/pika.egg-info/PKG-INFO` & `pika-1.3.2/pika.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,37 +1,35 @@
 Metadata-Version: 2.1
 Name: pika
-Version: 1.3.1
+Version: 1.3.2
 Summary: Pika Python AMQP Client Library
 Maintainer-email: "Gavin M. Roy" <gavinmroy@gmail.com>, Luke Bakken <lukerbakken@gmail.com>
 License: BSD-3-Clause
 Project-URL: Homepage, https://pika.readthedocs.io
 Project-URL: Source, https://github.com/pika/pika
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Natural Language :: English
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.4
-Classifier: Programming Language :: Python :: 3.5
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: Jython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Topic :: Communications
 Classifier: Topic :: Internet
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: System :: Networking
-Requires-Python: >=3.4
+Requires-Python: >=3.7
 Description-Content-Type: text/x-rst
 Provides-Extra: gevent
 Provides-Extra: tornado
 Provides-Extra: twisted
 License-File: LICENSE
 
 Pika
@@ -41,15 +39,15 @@
 |Version| |Python versions| |Actions Status| |Coverage| |License| |Docs|
 
 Introduction
 ------------
 Pika is a pure-Python implementation of the AMQP 0-9-1 protocol including
 RabbitMQ's extensions.
 
-- Supports Python 3.4+ (`1.1.0` was the last version to support 2.7)
+- Supports Python 3.7+ (`1.1.0` was the last version to support 2.7)
 - Since threads aren't appropriate to every situation, it doesn't require
   threads. Pika core takes care not to forbid them, either. The same goes for
   greenlets, callbacks, continuations, and generators. An instance of Pika's
   built-in connection adapters isn't thread-safe, however.
 - People may be using direct sockets, plain old ``select()``, or any of the
   wide variety of ways of getting network events to and from a Python
   application. Pika tries to stay compatible with all of these, and to make
@@ -195,15 +193,15 @@
 publishing of messages, etc., from a background thread to the connection
 adapter's thread.
 
 Connection recovery
 -------------------
 
 Some RabbitMQ clients (Bunny, Java, .NET, Objective-C, Swift) provide a way to
-automatically recover connection, its channels and topology (e.g. queues,
+automatically recover a connection, its channels and topology (e.g. queues,
 bindings and consumers) after a network failure. Others require connection
 recovery to be performed by the application code and strive to make it a
 straightforward process. Pika falls into the second category.
 
 Pika supports multiple connection adapters. They take different approaches to
 connection recovery.
```

### Comparing `pika-1.3.1/pika.egg-info/SOURCES.txt` & `pika-1.3.2/pika.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pika-1.3.1/pyproject.toml` & `pika-1.3.2/pyproject.toml`

 * *Files 5% similar despite different names*

```diff
@@ -1,59 +1,59 @@
 [build-system]
 requires = ["setuptools>=61.2"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "pika"
-version = "1.3.1"
+version = "1.3.2"
 maintainers = [
     {name = "Gavin M. Roy", email = "gavinmroy@gmail.com"},
     {name = "Luke Bakken", email = "lukerbakken@gmail.com"}
 ]
 license = {text = "BSD-3-Clause"}
 description = "Pika Python AMQP Client Library"
 classifiers = [
     "Development Status :: 5 - Production/Stable",
     "Intended Audience :: Developers",
     "License :: OSI Approved :: BSD License",
     "Natural Language :: English",
     "Operating System :: OS Independent",
     "Programming Language :: Python :: 3",
-    "Programming Language :: Python :: 3.4",
-    "Programming Language :: Python :: 3.5",
-    "Programming Language :: Python :: 3.6",
     "Programming Language :: Python :: 3.7",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
     "Programming Language :: Python :: 3.10",
+    "Programming Language :: Python :: 3.11",
     "Programming Language :: Python :: Implementation :: CPython",
     "Programming Language :: Python :: Implementation :: Jython",
     "Programming Language :: Python :: Implementation :: PyPy",
     "Topic :: Communications",
     "Topic :: Internet",
     "Topic :: Software Development :: Libraries",
     "Topic :: Software Development :: Libraries :: Python Modules",
     "Topic :: System :: Networking",
 ]
 dependencies = []
-requires-python = ">=3.4"
+requires-python = ">=3.7"
 
 [project.readme]
 file = "README.rst"
 content-type = "text/x-rst"
 
 [project.urls]
 Homepage = "https://pika.readthedocs.io"
 Source = "https://github.com/pika/pika"
 
 [project.optional-dependencies]
 gevent = ["gevent"]
 tornado = ["tornado"]
 twisted = ["twisted"]
 
+[tool.pyright]
+
 [tool.setuptools]
 zip-safe = true
 include-package-data = false
 packages = ["pika", "pika.adapters", "pika.adapters.utils"]
 
 [tool.setuptools.package-data]
 "*" = ["LICENSE", "README.rst"]
```

