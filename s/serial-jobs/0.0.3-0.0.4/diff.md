# Comparing `tmp/serial-jobs-0.0.3.tar.gz` & `tmp/serial-jobs-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "serial-jobs-0.0.3.tar", last modified: Wed Apr 12 14:45:26 2023, max compression
+gzip compressed data, was "serial-jobs-0.0.4.tar", last modified: Fri May  5 11:11:39 2023, max compression
```

## Comparing `serial-jobs-0.0.3.tar` & `serial-jobs-0.0.4.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 peter      (501) staff       (20)        0 2023-04-12 14:45:26.292306 serial-jobs-0.0.3/
--rw-r--r--   0 peter      (501) staff       (20)     1071 2022-05-08 11:19:26.000000 serial-jobs-0.0.3/LICENSE
--rw-r--r--   0 peter      (501) staff       (20)    30579 2023-04-12 14:45:26.292356 serial-jobs-0.0.3/PKG-INFO
--rw-r--r--   0 peter      (501) staff       (20)    30203 2023-04-12 14:44:50.000000 serial-jobs-0.0.3/README.rst
--rw-r--r--   0 peter      (501) staff       (20)      373 2022-05-18 00:29:13.000000 serial-jobs-0.0.3/pyproject.toml
--rw-r--r--   0 peter      (501) staff       (20)      827 2023-04-12 14:45:26.292636 serial-jobs-0.0.3/setup.cfg
-drwxr-xr-x   0 peter      (501) staff       (20)        0 2023-04-12 14:45:26.287250 serial-jobs-0.0.3/src/
-drwxr-xr-x   0 peter      (501) staff       (20)        0 2023-04-12 14:45:26.290502 serial-jobs-0.0.3/src/serial_jobs/
--rw-r--r--   0 peter      (501) staff       (20)      333 2023-04-12 14:44:50.000000 serial-jobs-0.0.3/src/serial_jobs/__init__.py
--rw-r--r--   0 peter      (501) staff       (20)     3479 2023-04-07 09:18:03.000000 serial-jobs-0.0.3/src/serial_jobs/config.py
--rw-r--r--   0 peter      (501) staff       (20)     7372 2022-07-24 13:43:17.000000 serial-jobs-0.0.3/src/serial_jobs/data.py
-drwxr-xr-x   0 peter      (501) staff       (20)        0 2023-04-12 14:45:26.291694 serial-jobs-0.0.3/src/serial_jobs/device/
--rw-r--r--   0 peter      (501) staff       (20)      127 2022-05-18 00:29:13.000000 serial-jobs-0.0.3/src/serial_jobs/device/__init__.py
--rw-r--r--   0 peter      (501) staff       (20)    11125 2022-05-18 00:29:13.000000 serial-jobs-0.0.3/src/serial_jobs/device/base.py
--rw-r--r--   0 peter      (501) staff       (20)     3407 2022-05-18 00:29:13.000000 serial-jobs-0.0.3/src/serial_jobs/device/bms.py
--rw-r--r--   0 peter      (501) staff       (20)     8104 2022-05-18 00:29:13.000000 serial-jobs-0.0.3/src/serial_jobs/device/modbus.py
--rw-r--r--   0 peter      (501) staff       (20)     2622 2022-05-18 00:29:13.000000 serial-jobs-0.0.3/src/serial_jobs/handler.py
--rw-r--r--   0 peter      (501) staff       (20)     5855 2022-05-18 00:29:13.000000 serial-jobs-0.0.3/src/serial_jobs/job.py
--rw-r--r--   0 peter      (501) staff       (20)     2341 2022-05-18 00:29:13.000000 serial-jobs-0.0.3/src/serial_jobs/main.py
--rw-r--r--   0 peter      (501) staff       (20)     3182 2022-05-18 00:29:13.000000 serial-jobs-0.0.3/src/serial_jobs/mqtt.py
--rw-r--r--   0 peter      (501) staff       (20)     4971 2023-04-07 09:18:03.000000 serial-jobs-0.0.3/src/serial_jobs/schema.py
-drwxr-xr-x   0 peter      (501) staff       (20)        0 2023-04-12 14:45:26.292176 serial-jobs-0.0.3/src/serial_jobs/scripts/
--rw-r--r--   0 peter      (501) staff       (20)        0 2022-05-18 00:29:13.000000 serial-jobs-0.0.3/src/serial_jobs/scripts/__init__.py
--rwxr-xr-x   0 peter      (501) staff       (20)     1445 2022-05-18 00:29:13.000000 serial-jobs-0.0.3/src/serial_jobs/scripts/convert_config.py
--rwxr-xr-x   0 peter      (501) staff       (20)     1924 2022-05-18 00:29:13.000000 serial-jobs-0.0.3/src/serial_jobs/scripts/merge_config.py
--rwxr-xr-x   0 peter      (501) staff       (20)     1804 2022-05-18 00:29:13.000000 serial-jobs-0.0.3/src/serial_jobs/scripts/run.py
--rw-r--r--   0 peter      (501) staff       (20)     5291 2022-05-18 00:29:13.000000 serial-jobs-0.0.3/src/serial_jobs/service.py
--rw-r--r--   0 peter      (501) staff       (20)     1362 2022-05-08 13:39:42.000000 serial-jobs-0.0.3/src/serial_jobs/specification.py
--rw-r--r--   0 peter      (501) staff       (20)     2437 2022-05-18 00:29:13.000000 serial-jobs-0.0.3/src/serial_jobs/task.py
--rw-r--r--   0 peter      (501) staff       (20)     4463 2022-05-18 00:29:13.000000 serial-jobs-0.0.3/src/serial_jobs/value.py
-drwxr-xr-x   0 peter      (501) staff       (20)        0 2023-04-12 14:45:26.291205 serial-jobs-0.0.3/src/serial_jobs.egg-info/
--rw-r--r--   0 peter      (501) staff       (20)    30579 2023-04-12 14:45:26.000000 serial-jobs-0.0.3/src/serial_jobs.egg-info/PKG-INFO
--rw-r--r--   0 peter      (501) staff       (20)      868 2023-04-12 14:45:26.000000 serial-jobs-0.0.3/src/serial_jobs.egg-info/SOURCES.txt
--rw-r--r--   0 peter      (501) staff       (20)        1 2023-04-12 14:45:26.000000 serial-jobs-0.0.3/src/serial_jobs.egg-info/dependency_links.txt
--rw-r--r--   0 peter      (501) staff       (20)      199 2023-04-12 14:45:26.000000 serial-jobs-0.0.3/src/serial_jobs.egg-info/entry_points.txt
--rw-r--r--   0 peter      (501) staff       (20)       65 2023-04-12 14:45:26.000000 serial-jobs-0.0.3/src/serial_jobs.egg-info/requires.txt
--rw-r--r--   0 peter      (501) staff       (20)       12 2023-04-12 14:45:26.000000 serial-jobs-0.0.3/src/serial_jobs.egg-info/top_level.txt
+drwxr-xr-x   0 peter     (1000) peter     (1000)        0 2023-05-05 11:11:39.254968 serial-jobs-0.0.4/
+-rw-r--r--   0 peter     (1000) peter     (1000)     1071 2022-05-01 11:21:32.000000 serial-jobs-0.0.4/LICENSE
+-rw-r--r--   0 peter     (1000) peter     (1000)    31140 2023-05-05 11:11:39.254968 serial-jobs-0.0.4/PKG-INFO
+-rw-r--r--   0 peter     (1000) peter     (1000)    30629 2023-05-05 08:50:58.000000 serial-jobs-0.0.4/README.rst
+-rw-r--r--   0 peter     (1000) peter     (1000)      373 2022-05-15 09:42:17.000000 serial-jobs-0.0.4/pyproject.toml
+-rw-r--r--   0 peter     (1000) peter     (1000)      993 2023-05-05 11:11:39.254968 serial-jobs-0.0.4/setup.cfg
+drwxr-xr-x   0 peter     (1000) peter     (1000)        0 2023-05-05 11:11:39.251634 serial-jobs-0.0.4/src/
+drwxr-xr-x   0 peter     (1000) peter     (1000)        0 2023-05-05 11:11:39.251634 serial-jobs-0.0.4/src/serial_jobs/
+-rw-r--r--   0 peter     (1000) peter     (1000)      333 2023-05-05 11:03:26.000000 serial-jobs-0.0.4/src/serial_jobs/__init__.py
+-rw-r--r--   0 peter     (1000) peter     (1000)     3479 2023-05-04 19:01:30.000000 serial-jobs-0.0.4/src/serial_jobs/config.py
+-rw-r--r--   0 peter     (1000) peter     (1000)     7429 2023-05-04 22:56:27.000000 serial-jobs-0.0.4/src/serial_jobs/data.py
+drwxr-xr-x   0 peter     (1000) peter     (1000)        0 2023-05-05 11:11:39.254968 serial-jobs-0.0.4/src/serial_jobs/device/
+-rw-r--r--   0 peter     (1000) peter     (1000)      127 2022-05-14 20:06:35.000000 serial-jobs-0.0.4/src/serial_jobs/device/__init__.py
+-rw-r--r--   0 peter     (1000) peter     (1000)    11133 2023-05-04 19:01:30.000000 serial-jobs-0.0.4/src/serial_jobs/device/base.py
+-rw-r--r--   0 peter     (1000) peter     (1000)     3501 2023-05-04 19:01:30.000000 serial-jobs-0.0.4/src/serial_jobs/device/bms.py
+-rw-r--r--   0 peter     (1000) peter     (1000)     8116 2023-05-04 19:01:30.000000 serial-jobs-0.0.4/src/serial_jobs/device/modbus.py
+-rw-r--r--   0 peter     (1000) peter     (1000)     2622 2022-05-15 09:00:47.000000 serial-jobs-0.0.4/src/serial_jobs/handler.py
+-rw-r--r--   0 peter     (1000) peter     (1000)     5855 2022-05-14 02:57:27.000000 serial-jobs-0.0.4/src/serial_jobs/job.py
+-rw-r--r--   0 peter     (1000) peter     (1000)     2407 2023-05-04 19:01:30.000000 serial-jobs-0.0.4/src/serial_jobs/main.py
+-rw-r--r--   0 peter     (1000) peter     (1000)     3182 2022-05-14 17:33:59.000000 serial-jobs-0.0.4/src/serial_jobs/mqtt.py
+-rw-r--r--   0 peter     (1000) peter     (1000)     5019 2023-05-04 19:01:30.000000 serial-jobs-0.0.4/src/serial_jobs/schema.py
+drwxr-xr-x   0 peter     (1000) peter     (1000)        0 2023-05-05 11:11:39.254968 serial-jobs-0.0.4/src/serial_jobs/scripts/
+-rw-r--r--   0 peter     (1000) peter     (1000)        0 2022-05-15 09:09:58.000000 serial-jobs-0.0.4/src/serial_jobs/scripts/__init__.py
+-rwxr-xr-x   0 peter     (1000) peter     (1000)     1445 2022-05-15 09:00:47.000000 serial-jobs-0.0.4/src/serial_jobs/scripts/convert_config.py
+-rwxr-xr-x   0 peter     (1000) peter     (1000)     1924 2022-05-15 09:00:47.000000 serial-jobs-0.0.4/src/serial_jobs/scripts/merge_config.py
+-rwxr-xr-x   0 peter     (1000) peter     (1000)     1804 2022-05-14 18:30:21.000000 serial-jobs-0.0.4/src/serial_jobs/scripts/run.py
+-rw-r--r--   0 peter     (1000) peter     (1000)     5291 2022-05-14 18:35:31.000000 serial-jobs-0.0.4/src/serial_jobs/service.py
+-rw-r--r--   0 peter     (1000) peter     (1000)     1362 2022-05-08 13:19:30.000000 serial-jobs-0.0.4/src/serial_jobs/specification.py
+-rw-r--r--   0 peter     (1000) peter     (1000)     2437 2022-05-14 02:57:04.000000 serial-jobs-0.0.4/src/serial_jobs/task.py
+-rw-r--r--   0 peter     (1000) peter     (1000)     4463 2022-05-14 19:27:00.000000 serial-jobs-0.0.4/src/serial_jobs/value.py
+drwxr-xr-x   0 peter     (1000) peter     (1000)        0 2023-05-05 11:11:39.254968 serial-jobs-0.0.4/src/serial_jobs.egg-info/
+-rw-r--r--   0 peter     (1000) peter     (1000)    31140 2023-05-05 11:11:39.000000 serial-jobs-0.0.4/src/serial_jobs.egg-info/PKG-INFO
+-rw-r--r--   0 peter     (1000) peter     (1000)      868 2023-05-05 11:11:39.000000 serial-jobs-0.0.4/src/serial_jobs.egg-info/SOURCES.txt
+-rw-r--r--   0 peter     (1000) peter     (1000)        1 2023-05-05 11:11:39.000000 serial-jobs-0.0.4/src/serial_jobs.egg-info/dependency_links.txt
+-rw-r--r--   0 peter     (1000) peter     (1000)      199 2023-05-05 11:11:39.000000 serial-jobs-0.0.4/src/serial_jobs.egg-info/entry_points.txt
+-rw-r--r--   0 peter     (1000) peter     (1000)       65 2023-05-05 11:11:39.000000 serial-jobs-0.0.4/src/serial_jobs.egg-info/requires.txt
+-rw-r--r--   0 peter     (1000) peter     (1000)       12 2023-05-05 11:11:39.000000 serial-jobs-0.0.4/src/serial_jobs.egg-info/top_level.txt
```

### Comparing `serial-jobs-0.0.3/LICENSE` & `serial-jobs-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `serial-jobs-0.0.3/PKG-INFO` & `serial-jobs-0.0.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,15 @@
 Metadata-Version: 2.1
 Name: serial-jobs
-Version: 0.0.3
+Version: 0.0.4
+Summary: A tool for bidirectional communication between serial devices and MQTT brokers.
 Home-page: https://github.com/pbasista/serial-jobs/
 Author: Peter Bašista
+Author-email: pbasista@gmail.com
+License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Home Automation
 Classifier: Topic :: Utilities
 Description-Content-Type: text/x-rst
 Provides-Extra: dev
 License-File: LICENSE
@@ -673,15 +676,15 @@
 
 ``value`` (when used within `handlers`_ as MQTT input value)
     A part of configuration which specifies
     how to extract value from an incoming MQTT message
     and how to write it to a particular serial `device <devices_>`_.
 
     It consists of an object which specifies how to obtain the value
-    for sending to the configured MQTT broker from the configured serial device.
+    for writing to the configured serial device from the incoming MQTT messages.
 
     It might contain fields defined below.
 
     :mapping: *(optional)* An object containing string-to-string mapping
         applied to the obtained MQTT message content
         *before* converting it to the final value type.
 
@@ -699,14 +702,26 @@
         which will then be written to the configured serial device.
 
         Available values are:
         `float`_, `int`_,
         `str`_,
         `date`_, `datetime`_ and `time`_.
 
+        .. note::
+
+            Parsing of MQTT message payload
+            into the `date`_, `datetime`_ and `time`_ types
+            is implemented via their respective `fromisoformat`_ methods.
+
+            The parsed date or datetime or time value is then split
+            into tuples of the individual numeric fields
+            which can be written to the desired device registers.
+
+        .. _fromisoformat: https://docs.python.org/3/library/datetime.html#datetime.datetime.fromisoformat
+
     :data: A *sequence* of data part `specifications <data_>`_.
         They specify how to convert the obtained Python value to data parts
         which could be written to the configured serial device.
 
     **Example:**
 
     .. code-block:: yaml
@@ -755,16 +770,16 @@
 
     :register_type: *(optional)* Type of the register to read from.
         Defaults to ``default``.
 
         Available values are:
 
         * ``default``: The device-specific default register type.
-          Some device types like ``ModbusDevice`` do not have the default register type.
-          For those it is necessary to explicitly specify a register type other than ``default``.
+          For devices of type ``ModbusDevice`` the default register type
+          is the ``input`` register type.
 
         * ``coil``: A readable and writable register type which holds one bit of data.
           Available only for devices of type ``ModbusDevice``.
 
         * ``discrete``: A read-only register type which holds one bit of data.
           Available only for devices of type ``ModbusDevice``.
```

### Comparing `serial-jobs-0.0.3/README.rst` & `serial-jobs-0.0.4/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -660,15 +660,15 @@
 
 ``value`` (when used within `handlers`_ as MQTT input value)
     A part of configuration which specifies
     how to extract value from an incoming MQTT message
     and how to write it to a particular serial `device <devices_>`_.
 
     It consists of an object which specifies how to obtain the value
-    for sending to the configured MQTT broker from the configured serial device.
+    for writing to the configured serial device from the incoming MQTT messages.
 
     It might contain fields defined below.
 
     :mapping: *(optional)* An object containing string-to-string mapping
         applied to the obtained MQTT message content
         *before* converting it to the final value type.
 
@@ -686,14 +686,26 @@
         which will then be written to the configured serial device.
 
         Available values are:
         `float`_, `int`_,
         `str`_,
         `date`_, `datetime`_ and `time`_.
 
+        .. note::
+
+            Parsing of MQTT message payload
+            into the `date`_, `datetime`_ and `time`_ types
+            is implemented via their respective `fromisoformat`_ methods.
+
+            The parsed date or datetime or time value is then split
+            into tuples of the individual numeric fields
+            which can be written to the desired device registers.
+
+        .. _fromisoformat: https://docs.python.org/3/library/datetime.html#datetime.datetime.fromisoformat
+
     :data: A *sequence* of data part `specifications <data_>`_.
         They specify how to convert the obtained Python value to data parts
         which could be written to the configured serial device.
 
     **Example:**
 
     .. code-block:: yaml
@@ -742,16 +754,16 @@
 
     :register_type: *(optional)* Type of the register to read from.
         Defaults to ``default``.
 
         Available values are:
 
         * ``default``: The device-specific default register type.
-          Some device types like ``ModbusDevice`` do not have the default register type.
-          For those it is necessary to explicitly specify a register type other than ``default``.
+          For devices of type ``ModbusDevice`` the default register type
+          is the ``input`` register type.
 
         * ``coil``: A readable and writable register type which holds one bit of data.
           Available only for devices of type ``ModbusDevice``.
 
         * ``discrete``: A read-only register type which holds one bit of data.
           Available only for devices of type ``ModbusDevice``.
```

### Comparing `serial-jobs-0.0.3/setup.cfg` & `serial-jobs-0.0.4/setup.cfg`

 * *Files 26% similar despite different names*

```diff
@@ -1,17 +1,21 @@
 [metadata]
 name = serial-jobs
 version = attr: serial_jobs.__version__
 url = https://github.com/pbasista/serial-jobs/
 author = Peter Bašista
+author_email = pbasista@gmail.com
+license = MIT
+license_files = LICENSE
 classifiers = 
 	License :: OSI Approved :: MIT License
 	Operating System :: OS Independent
 	Topic :: Home Automation
 	Topic :: Utilities
+description = A tool for bidirectional communication between serial devices and MQTT brokers.
 long_description = file: README.rst
 long_description_content_type = text/x-rst
 
 [options]
 package_dir = 
 	= src
 packages = find:
```

### Comparing `serial-jobs-0.0.3/src/serial_jobs/config.py` & `serial-jobs-0.0.4/src/serial_jobs/config.py`

 * *Files identical despite different names*

### Comparing `serial-jobs-0.0.3/src/serial_jobs/data.py` & `serial-jobs-0.0.4/src/serial_jobs/data.py`

 * *Files 1% similar despite different names*

```diff
@@ -178,16 +178,17 @@
             register_data = int(register_data)
             if self.bitshift:
                 if self.bitshift > 0:
                     register_data <<= self.bitshift
                 elif self.bitshift < 0:
                     register_data >>= self.bitshift
             if self.bitmask:
-                inverse_bitmask = (1 << 8 * expected_size) - 1
-                register_data |= current_data ^ inverse_bitmask
+                binary_ones = (1 << 8 * expected_size) - 1
+                inverse_bitmask = self.bitmask ^ binary_ones
+                register_data |= current_data & inverse_bitmask
 
         changed_bytes = self.pack(register_data)
 
         if self.byte_count:
             register_bytes[self.byte_offset : self.byte_count] = changed_bytes
         else:
             register_bytes[self.byte_offset :] = changed_bytes
```

### Comparing `serial-jobs-0.0.3/src/serial_jobs/device/base.py` & `serial-jobs-0.0.4/src/serial_jobs/device/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -137,15 +137,15 @@
 
         Return the number of bytes read.
         """
         if register_type == RegisterType.DEFAULT:
             register_type = self.default_register_type
 
         LOGGER.debug(
-            "device %s: reading from %s register addresses %d-%d",
+            "device %s: reading from %s register addresses 0x%X-0x%X",
             self.spec_id,
             register_type.name,
             start_address,
             stop_address,
         )
 
         bytes_read = 0
@@ -175,15 +175,15 @@
 
         Return the number of bytes written.
         """
         if register_type == RegisterType.DEFAULT:
             register_type = self.default_register_type
 
         LOGGER.debug(
-            "device %s: writing to %s register addresses %d-%d",
+            "device %s: writing to %s register addresses 0x%X-0x%X",
             self.spec_id,
             register_type.name,
             start_address,
             stop_address,
         )
 
         bytes_written = 0
```

### Comparing `serial-jobs-0.0.3/src/serial_jobs/device/bms.py` & `serial-jobs-0.0.4/src/serial_jobs/device/bms.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 """Functionality related to communication with BMS devices."""
 from __future__ import annotations
 
 from dataclasses import dataclass
 from logging import getLogger
 from struct import pack
+from time import sleep
 
 from serial import Serial
 
 from .base import Device, RegisterType
 
 LOGGER = getLogger(__name__)
 
@@ -62,15 +63,18 @@
         # * 1 byte of data length
         # * "data length" bytes of content
         # * 2 bytes of checksum
         # * 0x77
         response = bytearray()
 
         attempts = 0
+        response.extend(self.serial.read(4))
+
         while len(response) < 4 and attempts < 3:
+            sleep(0.5)
             response.extend(self.serial.read(4))
             attempts += 1
 
         if len(response) < 4:
             raise RuntimeError(f"only {len(response)} bytes received from the device")
 
         length = response[3]
@@ -86,15 +90,15 @@
 
         LOGGER.debug("device %s: received data %s", self.spec_id, response.hex(" "))
 
         return response
 
     def _read_register(self, address: int, register_type: RegisterType) -> int:
         LOGGER.debug(
-            "device %s: reading from %s BMS register address %d",
+            "device %s: reading from %s BMS register address 0x%X",
             self.spec_id,
             register_type.name,
             address,
         )
 
         if register_type == RegisterType.DEFAULT:
             input_values = [0xDD, 0xA5, address, 0]
```

### Comparing `serial-jobs-0.0.3/src/serial_jobs/device/modbus.py` & `serial-jobs-0.0.4/src/serial_jobs/device/modbus.py`

 * *Files 2% similar despite different names*

```diff
@@ -75,15 +75,15 @@
         if self.instrument is None:
             raise RuntimeError("instrument is unavailable")
 
         if register_type == register_type.DEFAULT:
             register_type = self.default_register_type
 
         LOGGER.debug(
-            "device %s: reading from %s Modbus register address %d",
+            "device %s: reading from %s Modbus register address 0x%X",
             self.spec_id,
             register_type.name,
             address,
         )
 
         if register_type in (RegisterType.COIL, RegisterType.DISCRETE):
             int_value = self.instrument.read_bit(
@@ -110,15 +110,15 @@
         if self.instrument is None:
             raise RuntimeError("instrument is unavailable")
 
         if register_type == register_type.DEFAULT:
             register_type = self.default_register_type
 
         LOGGER.debug(
-            "device %s: reading from %s Modbus register address range %d-%d",
+            "device %s: reading from %s Modbus register address range 0x%X-0x%X",
             self.spec_id,
             register_type.name,
             start_address,
             stop_address,
         )
 
         number_of_registers = stop_address - start_address
@@ -153,15 +153,15 @@
         if self.instrument is None:
             raise RuntimeError("instrument is unavailable")
 
         if register_type == register_type.DEFAULT:
             register_type = self.default_register_type
 
         LOGGER.debug(
-            "device %s: writing to %s Modbus register address %d",
+            "device %s: writing to %s Modbus register address 0x%X",
             self.spec_id,
             register_type.name,
             address,
         )
 
         bytes_value = self.registers[register_type][address]
 
@@ -182,15 +182,15 @@
         if self.instrument is None:
             raise RuntimeError("instrument is unavailable")
 
         if register_type == register_type.DEFAULT:
             register_type = self.default_register_type
 
         LOGGER.debug(
-            "device %s: writing to %s Modbus register address range %d-%d",
+            "device %s: writing to %s Modbus register address range 0x%X-0x%X",
             self.spec_id,
             register_type.name,
             start_address,
             stop_address,
         )
 
         bytes_values = [
```

### Comparing `serial-jobs-0.0.3/src/serial_jobs/handler.py` & `serial-jobs-0.0.4/src/serial_jobs/handler.py`

 * *Files identical despite different names*

### Comparing `serial-jobs-0.0.3/src/serial_jobs/job.py` & `serial-jobs-0.0.4/src/serial_jobs/job.py`

 * *Files identical despite different names*

### Comparing `serial-jobs-0.0.3/src/serial_jobs/main.py` & `serial-jobs-0.0.4/src/serial_jobs/main.py`

 * *Files 9% similar despite different names*

```diff
@@ -51,16 +51,18 @@
     config = load_configuration(configuration_path)
 
     logger.debug("loading specifications")
     MQTTBroker.load_specifications(config["mqtt_brokers"])
     Device.load_specifications(config["devices"])
     Task.load_specifications(config["tasks"])
     Job.load_specifications(config["jobs"])
-    Handler.load_specifications(config["handlers"])
-    Service.load_specifications(config["services"])
+    if "handlers" in config:
+        Handler.load_specifications(config["handlers"])
+    if "services" in config:
+        Service.load_specifications(config["services"])
     logger.debug("specifications loaded")
 
     awaitable_jobs = [
         job.carry_out(keep_going, send_initial_messages, send_task_messages)
         for job in Job.from_all_specs()
     ]
     awaitable_services = [
```

### Comparing `serial-jobs-0.0.3/src/serial_jobs/mqtt.py` & `serial-jobs-0.0.4/src/serial_jobs/mqtt.py`

 * *Files identical despite different names*

### Comparing `serial-jobs-0.0.3/src/serial_jobs/schema.py` & `serial-jobs-0.0.4/src/serial_jobs/schema.py`

 * *Files 1% similar despite different names*

```diff
@@ -155,16 +155,16 @@
     }
 )
 
 jobs_schema = Seq(job_schema)
 
 input_value_schema = Map(
     {
+        Optional("type"): Enum(("float", "int", "str", "date", "datetime", "time")),
         Optional("mapping"): MapPattern(Str(), Str()),
-        Optional("type"): Enum(("float", "int", "str")),
         "data": data_schema,
     }
 )
 
 handler_schema = Map(
     {
         "id": Str(),
@@ -203,11 +203,11 @@
 
 configuration_schema = Map(
     {
         "mqtt_brokers": mqtt_brokers_schema,
         "devices": devices_schema,
         "tasks": tasks_schema,
         "jobs": jobs_schema,
-        "handlers": handlers_schema,
-        "services": services_schema,
+        Optional("handlers"): handlers_schema,
+        Optional("services"): services_schema,
     }
 )
```

### Comparing `serial-jobs-0.0.3/src/serial_jobs/scripts/convert_config.py` & `serial-jobs-0.0.4/src/serial_jobs/scripts/convert_config.py`

 * *Files identical despite different names*

### Comparing `serial-jobs-0.0.3/src/serial_jobs/scripts/merge_config.py` & `serial-jobs-0.0.4/src/serial_jobs/scripts/merge_config.py`

 * *Files identical despite different names*

### Comparing `serial-jobs-0.0.3/src/serial_jobs/scripts/run.py` & `serial-jobs-0.0.4/src/serial_jobs/scripts/run.py`

 * *Files identical despite different names*

### Comparing `serial-jobs-0.0.3/src/serial_jobs/service.py` & `serial-jobs-0.0.4/src/serial_jobs/service.py`

 * *Files identical despite different names*

### Comparing `serial-jobs-0.0.3/src/serial_jobs/specification.py` & `serial-jobs-0.0.4/src/serial_jobs/specification.py`

 * *Files identical despite different names*

### Comparing `serial-jobs-0.0.3/src/serial_jobs/task.py` & `serial-jobs-0.0.4/src/serial_jobs/task.py`

 * *Files identical despite different names*

### Comparing `serial-jobs-0.0.3/src/serial_jobs/value.py` & `serial-jobs-0.0.4/src/serial_jobs/value.py`

 * *Files identical despite different names*

### Comparing `serial-jobs-0.0.3/src/serial_jobs.egg-info/PKG-INFO` & `serial-jobs-0.0.4/src/serial_jobs.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,15 @@
 Metadata-Version: 2.1
 Name: serial-jobs
-Version: 0.0.3
+Version: 0.0.4
+Summary: A tool for bidirectional communication between serial devices and MQTT brokers.
 Home-page: https://github.com/pbasista/serial-jobs/
 Author: Peter Bašista
+Author-email: pbasista@gmail.com
+License: MIT
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Home Automation
 Classifier: Topic :: Utilities
 Description-Content-Type: text/x-rst
 Provides-Extra: dev
 License-File: LICENSE
@@ -673,15 +676,15 @@
 
 ``value`` (when used within `handlers`_ as MQTT input value)
     A part of configuration which specifies
     how to extract value from an incoming MQTT message
     and how to write it to a particular serial `device <devices_>`_.
 
     It consists of an object which specifies how to obtain the value
-    for sending to the configured MQTT broker from the configured serial device.
+    for writing to the configured serial device from the incoming MQTT messages.
 
     It might contain fields defined below.
 
     :mapping: *(optional)* An object containing string-to-string mapping
         applied to the obtained MQTT message content
         *before* converting it to the final value type.
 
@@ -699,14 +702,26 @@
         which will then be written to the configured serial device.
 
         Available values are:
         `float`_, `int`_,
         `str`_,
         `date`_, `datetime`_ and `time`_.
 
+        .. note::
+
+            Parsing of MQTT message payload
+            into the `date`_, `datetime`_ and `time`_ types
+            is implemented via their respective `fromisoformat`_ methods.
+
+            The parsed date or datetime or time value is then split
+            into tuples of the individual numeric fields
+            which can be written to the desired device registers.
+
+        .. _fromisoformat: https://docs.python.org/3/library/datetime.html#datetime.datetime.fromisoformat
+
     :data: A *sequence* of data part `specifications <data_>`_.
         They specify how to convert the obtained Python value to data parts
         which could be written to the configured serial device.
 
     **Example:**
 
     .. code-block:: yaml
@@ -755,16 +770,16 @@
 
     :register_type: *(optional)* Type of the register to read from.
         Defaults to ``default``.
 
         Available values are:
 
         * ``default``: The device-specific default register type.
-          Some device types like ``ModbusDevice`` do not have the default register type.
-          For those it is necessary to explicitly specify a register type other than ``default``.
+          For devices of type ``ModbusDevice`` the default register type
+          is the ``input`` register type.
 
         * ``coil``: A readable and writable register type which holds one bit of data.
           Available only for devices of type ``ModbusDevice``.
 
         * ``discrete``: A read-only register type which holds one bit of data.
           Available only for devices of type ``ModbusDevice``.
```

### Comparing `serial-jobs-0.0.3/src/serial_jobs.egg-info/SOURCES.txt` & `serial-jobs-0.0.4/src/serial_jobs.egg-info/SOURCES.txt`

 * *Files identical despite different names*

