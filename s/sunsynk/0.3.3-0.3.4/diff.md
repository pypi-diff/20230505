# Comparing `tmp/sunsynk-0.3.3.tar.gz` & `tmp/sunsynk-0.3.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sunsynk-0.3.3.tar", last modified: Sat Apr 22 20:28:34 2023, max compression
+gzip compressed data, was "sunsynk-0.3.4.tar", last modified: Fri May  5 11:04:19 2023, max compression
```

## Comparing `sunsynk-0.3.3.tar` & `sunsynk-0.3.4.tar`

### file list

```diff
@@ -1,47 +1,48 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 20:28:34.037470 sunsynk-0.3.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-04-22 20:28:24.000000 sunsynk-0.3.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       81 2023-04-22 20:28:24.000000 sunsynk-0.3.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2713 2023-04-22 20:28:34.037470 sunsynk-0.3.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1948 2023-04-22 20:28:24.000000 sunsynk-0.3.3/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1377 2023-04-22 20:28:34.037470 sunsynk-0.3.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      120 2023-04-22 20:28:24.000000 sunsynk-0.3.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 20:28:34.033470 sunsynk-0.3.3/sunsynk/
--rw-r--r--   0 runner    (1001) docker     (123)      303 2023-04-22 20:28:24.000000 sunsynk-0.3.3/sunsynk/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    12614 2023-04-22 20:28:24.000000 sunsynk-0.3.3/sunsynk/definitions.py
--rw-r--r--   0 runner    (1001) docker     (123)    12157 2023-04-22 20:28:24.000000 sunsynk-0.3.3/sunsynk/definitions3ph.py
--rw-r--r--   0 runner    (1001) docker     (123)     2885 2023-04-22 20:28:24.000000 sunsynk-0.3.3/sunsynk/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     2665 2023-04-22 20:28:24.000000 sunsynk-0.3.3/sunsynk/pysunsynk.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     8050 2023-04-22 20:28:24.000000 sunsynk-0.3.3/sunsynk/rwsensors.py
--rw-r--r--   0 runner    (1001) docker     (123)     5777 2023-04-22 20:28:24.000000 sunsynk-0.3.3/sunsynk/sensors.py
--rw-r--r--   0 runner    (1001) docker     (123)     3219 2023-04-22 20:28:24.000000 sunsynk-0.3.3/sunsynk/state.py
--rw-r--r--   0 runner    (1001) docker     (123)     4053 2023-04-22 20:28:24.000000 sunsynk-0.3.3/sunsynk/sunsynk.py
--rw-r--r--   0 runner    (1001) docker     (123)     2066 2023-04-22 20:28:24.000000 sunsynk-0.3.3/sunsynk/usunsynk.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 20:28:34.033470 sunsynk-0.3.3/sunsynk.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2713 2023-04-22 20:28:34.000000 sunsynk-0.3.3/sunsynk.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1046 2023-04-22 20:28:34.000000 sunsynk-0.3.3/sunsynk.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-22 20:28:34.000000 sunsynk-0.3.3/sunsynk.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      250 2023-04-22 20:28:34.000000 sunsynk-0.3.3/sunsynk.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-04-22 20:28:34.000000 sunsynk-0.3.3/sunsynk.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-22 20:28:33.000000 sunsynk-0.3.3/sunsynk.egg-info/zip-safe
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 20:28:34.033470 sunsynk-0.3.3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)       61 2023-04-22 20:28:24.000000 sunsynk-0.3.3/tests/README.md
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-22 20:28:24.000000 sunsynk-0.3.3/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1179 2023-04-22 20:28:24.000000 sunsynk-0.3.3/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     4426 2023-04-22 20:28:24.000000 sunsynk-0.3.3/tests/hass-addon-sunsynk-dev.zip
--rw-r--r--   0 runner    (1001) docker     (123)    14052 2023-04-22 20:28:24.000000 sunsynk-0.3.3/tests/hass-addon-sunsynk.zip
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 20:28:34.037470 sunsynk-0.3.3/tests/hass_addon_sunsynk_multi/
--rw-r--r--   0 runner    (1001) docker     (123)      273 2023-04-22 20:28:24.000000 sunsynk-0.3.3/tests/hass_addon_sunsynk_multi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      303 2023-04-22 20:28:24.000000 sunsynk-0.3.3/tests/hass_addon_sunsynk_multi/test_definitions3ph.py
--rw-r--r--   0 runner    (1001) docker     (123)     4475 2023-04-22 20:28:24.000000 sunsynk-0.3.3/tests/hass_addon_sunsynk_multi/test_filter.py
--rw-r--r--   0 runner    (1001) docker     (123)     1367 2023-04-22 20:28:24.000000 sunsynk-0.3.3/tests/hass_addon_sunsynk_multi/test_run.py
--rw-r--r--   0 runner    (1001) docker     (123)     1687 2023-04-22 20:28:24.000000 sunsynk-0.3.3/tests/hass_addon_sunsynk_multi/test_state.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-22 20:28:34.037470 sunsynk-0.3.3/tests/sunsynk/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-22 20:28:24.000000 sunsynk-0.3.3/tests/sunsynk/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      210 2023-04-22 20:28:24.000000 sunsynk-0.3.3/tests/sunsynk/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     2031 2023-04-22 20:28:24.000000 sunsynk-0.3.3/tests/sunsynk/test_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)     3485 2023-04-22 20:28:24.000000 sunsynk-0.3.3/tests/sunsynk/test_pysunsynk.py
--rw-r--r--   0 runner    (1001) docker     (123)      999 2023-04-22 20:28:24.000000 sunsynk-0.3.3/tests/sunsynk/test_register.py
--rw-r--r--   0 runner    (1001) docker     (123)     4658 2023-04-22 20:28:24.000000 sunsynk-0.3.3/tests/sunsynk/test_rwsensors.py
--rw-r--r--   0 runner    (1001) docker     (123)     4779 2023-04-22 20:28:24.000000 sunsynk-0.3.3/tests/sunsynk/test_sensors.py
--rw-r--r--   0 runner    (1001) docker     (123)     2864 2023-04-22 20:28:24.000000 sunsynk-0.3.3/tests/sunsynk/test_sunsynk.py
--rw-r--r--   0 runner    (1001) docker     (123)     1320 2023-04-22 20:28:24.000000 sunsynk-0.3.3/tests/sunsynk/test_usunsynk.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 11:04:19.860590 sunsynk-0.3.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1073 2023-05-05 11:04:11.000000 sunsynk-0.3.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       81 2023-05-05 11:04:11.000000 sunsynk-0.3.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2712 2023-05-05 11:04:19.860590 sunsynk-0.3.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1947 2023-05-05 11:04:11.000000 sunsynk-0.3.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1377 2023-05-05 11:04:19.860590 sunsynk-0.3.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      120 2023-05-05 11:04:11.000000 sunsynk-0.3.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 11:04:19.856590 sunsynk-0.3.4/sunsynk/
+-rw-r--r--   0 runner    (1001) docker     (123)      303 2023-05-05 11:04:11.000000 sunsynk-0.3.4/sunsynk/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    12100 2023-05-05 11:04:11.000000 sunsynk-0.3.4/sunsynk/definitions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12157 2023-05-05 11:04:11.000000 sunsynk-0.3.4/sunsynk/definitions3ph.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4333 2023-05-05 11:04:11.000000 sunsynk-0.3.4/sunsynk/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2665 2023-05-05 11:04:11.000000 sunsynk-0.3.4/sunsynk/pysunsynk.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     8030 2023-05-05 11:04:11.000000 sunsynk-0.3.4/sunsynk/rwsensors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5795 2023-05-05 11:04:11.000000 sunsynk-0.3.4/sunsynk/sensors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3219 2023-05-05 11:04:11.000000 sunsynk-0.3.4/sunsynk/state.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4053 2023-05-05 11:04:11.000000 sunsynk-0.3.4/sunsynk/sunsynk.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2066 2023-05-05 11:04:11.000000 sunsynk-0.3.4/sunsynk/usunsynk.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 11:04:19.856590 sunsynk-0.3.4/sunsynk.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2712 2023-05-05 11:04:19.000000 sunsynk-0.3.4/sunsynk.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1093 2023-05-05 11:04:19.000000 sunsynk-0.3.4/sunsynk.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 11:04:19.000000 sunsynk-0.3.4/sunsynk.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      250 2023-05-05 11:04:19.000000 sunsynk-0.3.4/sunsynk.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-05 11:04:19.000000 sunsynk-0.3.4/sunsynk.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 11:04:19.000000 sunsynk-0.3.4/sunsynk.egg-info/zip-safe
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 11:04:19.856590 sunsynk-0.3.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)       61 2023-05-05 11:04:11.000000 sunsynk-0.3.4/tests/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 11:04:11.000000 sunsynk-0.3.4/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1179 2023-05-05 11:04:11.000000 sunsynk-0.3.4/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4426 2023-05-05 11:04:11.000000 sunsynk-0.3.4/tests/hass-addon-sunsynk-dev.zip
+-rw-r--r--   0 runner    (1001) docker     (123)    14052 2023-05-05 11:04:11.000000 sunsynk-0.3.4/tests/hass-addon-sunsynk.zip
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 11:04:19.860590 sunsynk-0.3.4/tests/hass_addon_sunsynk_multi/
+-rw-r--r--   0 runner    (1001) docker     (123)      320 2023-05-05 11:04:11.000000 sunsynk-0.3.4/tests/hass_addon_sunsynk_multi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      303 2023-05-05 11:04:11.000000 sunsynk-0.3.4/tests/hass_addon_sunsynk_multi/test_definitions3ph.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4475 2023-05-05 11:04:11.000000 sunsynk-0.3.4/tests/hass_addon_sunsynk_multi/test_filter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1333 2023-05-05 11:04:11.000000 sunsynk-0.3.4/tests/hass_addon_sunsynk_multi/test_run.py
+-rw-r--r--   0 runner    (1001) docker     (123)      832 2023-05-05 11:04:11.000000 sunsynk-0.3.4/tests/hass_addon_sunsynk_multi/test_sensors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1963 2023-05-05 11:04:11.000000 sunsynk-0.3.4/tests/hass_addon_sunsynk_multi/test_state.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 11:04:19.860590 sunsynk-0.3.4/tests/sunsynk/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 11:04:11.000000 sunsynk-0.3.4/tests/sunsynk/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      210 2023-05-05 11:04:11.000000 sunsynk-0.3.4/tests/sunsynk/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2503 2023-05-05 11:04:11.000000 sunsynk-0.3.4/tests/sunsynk/test_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3497 2023-05-05 11:04:11.000000 sunsynk-0.3.4/tests/sunsynk/test_pysunsynk.py
+-rw-r--r--   0 runner    (1001) docker     (123)      999 2023-05-05 11:04:11.000000 sunsynk-0.3.4/tests/sunsynk/test_register.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4936 2023-05-05 11:04:11.000000 sunsynk-0.3.4/tests/sunsynk/test_rwsensors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4779 2023-05-05 11:04:11.000000 sunsynk-0.3.4/tests/sunsynk/test_sensors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2864 2023-05-05 11:04:11.000000 sunsynk-0.3.4/tests/sunsynk/test_sunsynk.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1320 2023-05-05 11:04:11.000000 sunsynk-0.3.4/tests/sunsynk/test_usunsynk.py
```

### Comparing `sunsynk-0.3.3/LICENSE` & `sunsynk-0.3.4/LICENSE`

 * *Files identical despite different names*

### Comparing `sunsynk-0.3.3/PKG-INFO` & `sunsynk-0.3.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sunsynk
-Version: 0.3.3
+Version: 0.3.4
 Summary: Library to interface Deye/Sunsynk Hybrid Inverters
 Home-page: https://kellerza.github.io/sunsynk/
 Author: Johann Kellerman
 Author-email: kellerza@gmail.com
 License: MIT
 Keywords: sunsynk,deye,inverter,modbus,asyncio
 Classifier: Development Status :: 4 - Beta
@@ -51,12 +51,11 @@
 
 
 Below an example of the HomeAssistant Energy management dashboard using sensors from the Sunsynk.
 
 ![HASS Energy management](https://github.com/kellerza/sunsynk/raw/main/images/energy.png)
 
 ## Sunsynk Python Library
-
 [![PyPI version](https://badge.fury.io/py/sunsynk.svg)](https://pypi.org/project/sunsynk/)
 [![codecov](https://codecov.io/gh/kellerza/sunsynk/branch/main/graph/badge.svg?token=ILKRC5UTXI)](https://codecov.io/gh/kellerza/sunsynk)
 
 The Python library is available through pip: `pip install sunsynk`
```

### Comparing `sunsynk-0.3.3/README.md` & `sunsynk-0.3.4/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -28,12 +28,11 @@
 
 
 Below an example of the HomeAssistant Energy management dashboard using sensors from the Sunsynk.
 
 ![HASS Energy management](https://github.com/kellerza/sunsynk/raw/main/images/energy.png)
 
 ## Sunsynk Python Library
-
 [![PyPI version](https://badge.fury.io/py/sunsynk.svg)](https://pypi.org/project/sunsynk/)
 [![codecov](https://codecov.io/gh/kellerza/sunsynk/branch/main/graph/badge.svg?token=ILKRC5UTXI)](https://codecov.io/gh/kellerza/sunsynk)
 
 The Python library is available through pip: `pip install sunsynk`
```

### Comparing `sunsynk-0.3.3/setup.cfg` & `sunsynk-0.3.4/setup.cfg`

 * *Files identical despite different names*

### Comparing `sunsynk-0.3.3/sunsynk/definitions.py` & `sunsynk-0.3.4/sunsynk/definitions3ph.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,13 +1,14 @@
-"""Sunsynk 5kW&8kW hybrid inverter sensor definitions."""
+"""Sunsynk 5kW&8kW hybrid 3-phase inverter sensor definitions."""
+# pylint: disable=duplicate-code
 from sunsynk import AMPS, CELSIUS, KWH, VOLT, WATT
 from sunsynk.rwsensors import (
     NumberRWSensor,
     SelectRWSensor,
-    SystemTimeRWSensor,
+    SwitchRWSensor,
     TimeRWSensor,
 )
 from sunsynk.sensors import (
     FaultSensor,
     InverterStateSensor,
     MathSensor,
     SDStatusSensor,
@@ -19,178 +20,215 @@
 
 SENSORS = SensorDefinitions()
 
 ##########
 # Battery
 ##########
 SENSORS += (
-    TempSensor(182, "Battery temperature", CELSIUS, 0.1),
-    Sensor(183, "Battery voltage", VOLT, 0.01),
-    Sensor(184, "Battery SOC", "%"),
-    Sensor(190, "Battery power", WATT, -1),
-    Sensor(191, "Battery current", AMPS, -0.01),
+    TempSensor(586, "Battery temperature", CELSIUS, 0.1),
+    Sensor(587, "Battery voltage", VOLT, 0.01),
+    Sensor(588, "Battery SOC", "%"),
+    Sensor(590, "Battery power", WATT, -1),
+    Sensor(591, "Battery current", AMPS, -0.01),
 )
 
 #################
 # Inverter Power
 #################
 SENSORS += (
-    Sensor(175, "Inverter power", WATT, -1),
-    Sensor(154, "Inverter voltage", VOLT, 0.1),
-    Sensor(193, "Inverter frequency", "Hz", 0.01),
+    Sensor(636, "Inverter power", WATT, -1),
+    Sensor(633, "Inverter L1 power", WATT, -1),
+    Sensor(634, "Inverter L2 power", WATT, -1),
+    Sensor(635, "Inverter L3 power", WATT, -1),
+    Sensor(627, "Inverter voltage", VOLT, 0.1),
+    Sensor(638, "Inverter frequency", "Hz", 0.01),
 )
 
 #############
 # Grid Power
 #############
 SENSORS += (
-    Sensor(79, "Grid frequency", "Hz", 0.01),
-    Sensor(169, "Grid power", WATT, -1),  # L1(167) + L2(168)
-    Sensor(167, "Grid LD power", WATT, -1),  # L1 seems to be LD
-    Sensor(168, "Grid L2 power", WATT, -1),
-    Sensor(150, "Grid voltage", VOLT, 0.1),
-    MathSensor((160, 161), "Grid current", AMPS, factors=(0.01, 0.01)),
-    Sensor(172, "Grid CT power", WATT, -1),
+    Sensor(609, "Grid frequency", "Hz", 0.01),
+    Sensor(625, "Grid power", WATT, -1),  # gridTotalPac
+    Sensor(622, "Grid L1 power", WATT, -1),  # aPower
+    Sensor(623, "Grid L2 power", WATT, -1),  # bPower
+    Sensor(624, "Grid L3 power", WATT, -1),  # cPower
+    Sensor(600, "Grid voltage", VOLT, 0.1),  # aLineVolt
+    MathSensor(
+        (610, 611, 612), "Grid current", AMPS, factors=(0.01, 0.01, 0.01)
+    ),  # iac1,iac2,iac3
+    Sensor(619, "Grid CT power", WATT, -1),  # gridOutsideTotalPac (unsure ??)
 )
-# LD power?
 
 #############
 # Load Power
 #############
 SENSORS += (
-    Sensor(178, "Load power", WATT, -1),  # L1(176) + L2(177)
-    Sensor(176, "Load L1 power", WATT, -1),
-    Sensor(177, "Load L2 power", WATT, -1),
+    Sensor(653, "Load power", WATT, -1),
+    Sensor(650, "Load L1 power", WATT, -1),
+    Sensor(651, "Load L2 power", WATT, -1),
+    Sensor(652, "Load L3 power", WATT, -1),
 )
 
 ################
 # Solar Power 1
 ################
 SENSORS += (
-    Sensor(186, "PV1 power", WATT, -1),
-    Sensor(109, "PV1 voltage", VOLT, 0.1),
-    Sensor(110, "PV1 current", AMPS, 0.1),
+    Sensor(672, "PV1 power", WATT, -1),
+    Sensor(676, "PV1 voltage", VOLT, 0.1),
+    Sensor(677, "PV1 current", AMPS, 0.1),
 )
 
 ################
 # Solar Power 2
 ################
 SENSORS += (
-    Sensor(187, "PV2 power", WATT, -1),
-    Sensor(111, "PV2 voltage", VOLT, 0.1),
-    Sensor(112, "PV2 current", AMPS, 0.1),
+    Sensor(673, "PV2 power", WATT, -1),
+    Sensor(678, "PV2 voltage", VOLT, 0.1),
+    Sensor(679, "PV2 current", AMPS, 0.1),
+)
+
+################
+# Solar Power 3 (?? deye 3 Phase  only has 2 MPPT)
+################
+SENSORS += (
+    Sensor(674, "PV3 power", WATT, -1),
+    Sensor(680, "PV3 voltage", VOLT, 0.1),
+    Sensor(681, "PV3 current", AMPS, 0.1),
+)
+
+################
+# Solar Power 4 (?? deye 3 Phase  only has 2 MPPT)
+################
+SENSORS += (
+    Sensor(675, "PV4 power", WATT, -1),
+    Sensor(682, "PV4 voltage", VOLT, 0.1),
+    Sensor(683, "PV4 current", AMPS, 0.1),
 )
 
+
 ###################
-# Power on Outputs
+# Power on Outputs (aka GEN - which has multiple modes on the deye 3 Phase )
 ###################
 SENSORS += (
-    Sensor(166, "AUX power", WATT, -1),
-    # https://github.com/kellerza/sunsynk/issues/75
-    #  https://powerforum.co.za/topic/8646-my-sunsynk-8kw-data-collection-setup/?do=findComment&comment=147591
-    MathSensor(
-        (175, 169, 166), "Essential power", WATT, factors=(1, 1, -1), absolute=True
-    ),
-    # MathSensor((175, 167, 166), "Essential power", WATT, factors=(1, 1, -1)),
-    MathSensor(
-        (172, 167), "Non-Essential power", WATT, factors=(1, -1), no_negative=True
-    ),
+    Sensor(667, "Gen power", WATT, -1),
+    Sensor(664, "Gen L1 power", WATT, -1),
+    Sensor(665, "Gen L2 power", WATT, -1),
+    Sensor(666, "Gen L3 power", WATT, -1),
 )
 
 ###################
 # Energy
 ###################
 SENSORS += (
-    Sensor(60, "Day Active Energy", KWH, -0.1),
-    Sensor(70, "Day Battery Charge", KWH, 0.1),
-    Sensor(71, "Day Battery discharge", KWH, 0.1),
-    Sensor(77, "Day Grid Export", KWH, 0.1),
-    Sensor(76, "Day Grid Import", KWH, 0.1),
-    # Sensor(200, "Day Load Power", KWH, 0.01),
-    Sensor(84, "Day Load Energy", KWH, 0.1),
-    Sensor(108, "Day PV Energy", KWH, 0.1),
-    Sensor(61, "Day Reactive Energy", "kVarh", -0.1),
-    # Sensor((201, 202), "History Load Power", KWH, 0.1),
-    Sensor(67, "Month Grid Energy", KWH, 0.1),
-    Sensor(66, "Month Load Energy", KWH, 0.1),
-    Sensor(65, "Month PV Energy", KWH, 0.1),
-    Sensor((63, 64), "Total Active Energy", KWH, 0.1),  # signed?
-    Sensor((72, 73), "Total Battery Charge", KWH, 0.1),
-    Sensor((74, 75), "Total Battery Discharge", KWH, 0.1),
-    Sensor((81, 82), "Total Grid Export", KWH, 0.1),
-    Sensor((78, 80), "Total Grid Import", KWH, 0.1),
-    Sensor((85, 86), "Total Load Energy", KWH, 0.1),
-    Sensor((96, 97), "Total PV Energy", KWH, 0.1),
-    Sensor((98, 99), "Year Grid Export", KWH, 0.1),
-    Sensor((87, 88), "Year Load Energy", KWH, 0.1),
-    Sensor((68, 69), "Year PV Energy", KWH, 0.1),
+    Sensor(502, "Day Active Energy", KWH, -0.1),
+    Sensor(514, "Day Battery Charge", KWH, 0.1),
+    Sensor(515, "Day Battery discharge", KWH, 0.1),
+    Sensor(521, "Day Grid Export", KWH, 0.1),
+    Sensor(520, "Day Grid Import", KWH, 0.1),
+    Sensor(536, "Day Gen Energy", KWH, 0.1),
+    Sensor(526, "Day Load Energy", KWH, 0.1),  # I guess "used" = load?
+    Sensor(529, "Day PV Energy", KWH, 0.1),
+    Sensor((506, 507), "Total Active Energy", KWH, 0.1),  # signed?
+    Sensor((516, 517), "Total Battery Charge", KWH, 0.1),
+    Sensor((518, 519), "Total Battery Discharge", KWH, 0.1),
+    Sensor((524, 525), "Total Grid Export", KWH, 0.1),
+    Sensor((522, 523), "Total Grid Import", KWH, 0.1),
+    Sensor((527, 528), "Total Load Energy", KWH, 0.1),
+    Sensor((534, 535), "Total PV Energy", KWH, 0.1),
 )
 
 ##########
 # General
 ##########
-RATED_POWER = Sensor((16, 17), "Rated power", WATT, 0.1)
+RATED_POWER = Sensor((20, 21), "Rated power", WATT, 0.1)
+SENSORS += RATED_POWER
+
 SENSORS += (
-    RATED_POWER,
+    Sensor(
+        0, "Device Type"
+    ),  # {2: "Inverter", 3: "Hybrid Inverter", 4: "Micro Inverter", 5: "3 Phase Hybrid Inverter" }),
+    FaultSensor((555, 556, 557, 558), "Fault"),
+    InverterStateSensor(500, "Overall state"),
+    SDStatusSensor(0, "SD Status", ""),  # type: ignore        # 3 Phase does not have SD Card but crashes when removed
     SerialSensor((3, 4, 5, 6, 7), "Serial"),
-    Sensor(0, "Device Type"),
-    FaultSensor((103, 104, 105, 106), "Fault"),
-    InverterStateSensor(59, "Overall state"),
-    SDStatusSensor(92, "SD Status", ""),  # type: ignore
-    TempSensor(90, "DC transformer temperature", CELSIUS, 0.1),
-    TempSensor(95, "Environment temperature", CELSIUS, 0.1),
-    TempSensor(91, "Radiator temperature", CELSIUS, 0.1),
-    Sensor(194, "Grid Connected Status"),
-    SystemTimeRWSensor((22, 23, 24), "Date Time", unit=""),
+    TempSensor(540, "DC transformer temperature", CELSIUS, 0.1),
+    TempSensor(541, "Radiator temperature", CELSIUS, 0.1),
+    Sensor(
+        552, "Grid Connected Status"
+    ),  # Bit 0 = INV Relay, 1 = Undef, 2 = Grid relay, 3 = Gen relay, 4 = Grid give, 5, Dry contact
 )
+
+
 ###########
 # Settings
 ###########
 SENSORS += (
-    Sensor(200, "Control Mode"),
-    Sensor(232, "Grid Charge enabled", "", -1),
-    Sensor(312, "Battery charging voltage", VOLT, 0.01),
-    Sensor(603, "Bat1 SOC", "%"),
-    Sensor(611, "Bat1 Cycle"),
+    NumberRWSensor(128, "Grid Charge Battery current", AMPS, max=210),
+    SwitchRWSensor(130, "Grid Charge enabled"),
+    SwitchRWSensor(146, "Use Timer", on=255),
+    SwitchRWSensor(145, "Solar Export"),
+    NumberRWSensor(143, "Export Limit power", WATT, max=RATED_POWER),
+    NumberRWSensor(108, "Battery Max Charge current", AMPS, max=210),
+    NumberRWSensor(109, "Battery Max Discharge current", AMPS, max=210),
+    NumberRWSensor(102, "Battery Capacity current", AMPS, max=2000),
+)
+
+# Additional optional sensors
+SENSORS += (
+    NumberRWSensor(
+        103, "Battery low voltage", VOLT, -0.1
+    ),  # interesting perhaps not available in menu. default 4500 (45V)
+    SelectRWSensor(
+        133,
+        "Generator Port Usage",
+        options={0: "Generator", 1: "Smartload", 2: "Micro Inverter"},
+    ),
+    SelectRWSensor(129, "Generator Charge enabled", options={0: "Off", 1: "On"}),
+    SelectRWSensor(112, "Battery Activate", options={0: "Off", 1: "On"}),
+    NumberRWSensor(113, "Battery Resistance", "mΩ", max=6000),
+    NumberRWSensor(104, "System Zero Export power", WATT, -1),
+    NumberRWSensor(105, "Battery Equalization Days", "days", -1),
+    NumberRWSensor(106, "Battery Equalization Hours", "h", -1),  # 1 = 0.5 hours
 )
 
 # Absolute min and max voltage based on Deye inverter
 MIN_VOLTAGE = 41
 MAX_VOLTAGE = 60
 
 BATTERY_EQUALIZATION_VOLTAGE = NumberRWSensor(
-    201, "Battery Equalization voltage", VOLT, 0.01, min=MIN_VOLTAGE, max=MAX_VOLTAGE
+    99, "Battery Equalization voltage", VOLT, 0.01, min=MIN_VOLTAGE, max=MAX_VOLTAGE
 )
 BATTERY_ABSORPTION_VOLTAGE = NumberRWSensor(
-    202, "Battery Absorption voltage", VOLT, 0.01, min=MIN_VOLTAGE, max=MAX_VOLTAGE
+    100, "Battery Absorption voltage", VOLT, 0.01, min=MIN_VOLTAGE, max=MAX_VOLTAGE
 )
 BATTERY_FLOAT_VOLTAGE = NumberRWSensor(
-    203, "Battery Float voltage", VOLT, 0.01, min=MIN_VOLTAGE, max=MAX_VOLTAGE
+    101, "Battery Float voltage", VOLT, 0.01, min=MIN_VOLTAGE, max=MAX_VOLTAGE
 )
 
-BATTERY_SHUTDOWN_CAPACITY = NumberRWSensor(217, "Battery Shutdown Capacity", "%")
-BATTERY_RESTART_CAPACITY = NumberRWSensor(218, "Battery Restart Capacity", "%")
+BATTERY_SHUTDOWN_CAPACITY = NumberRWSensor(115, "Battery Shutdown Capacity", "%")
+BATTERY_RESTART_CAPACITY = NumberRWSensor(116, "Battery Restart Capacity", "%")
 BATTERY_LOW_CAPACITY = NumberRWSensor(
-    219,
+    117,
     "Battery Low Capacity",
     "%",
     min=BATTERY_SHUTDOWN_CAPACITY,
     max=BATTERY_RESTART_CAPACITY,
 )
 BATTERY_SHUTDOWN_CAPACITY.max = BATTERY_LOW_CAPACITY
 BATTERY_RESTART_CAPACITY.min = BATTERY_LOW_CAPACITY
 
 BATTERY_SHUTDOWN_VOLTAGE = NumberRWSensor(
-    220, "Battery Shutdown voltage", VOLT, 0.01, min=MIN_VOLTAGE
+    118, "Battery Shutdown voltage", VOLT, 0.01, min=MIN_VOLTAGE
 )
 BATTERY_RESTART_VOLTAGE = NumberRWSensor(
-    221, "Battery Restart voltage", VOLT, 0.01, max=MAX_VOLTAGE
+    119, "Battery Restart voltage", VOLT, 0.01, max=MAX_VOLTAGE
 )
 BATTERY_LOW_VOLTAGE = NumberRWSensor(
-    222,
+    120,
     "Battery Low voltage",
     VOLT,
     0.01,
     min=BATTERY_SHUTDOWN_VOLTAGE,
     max=BATTERY_RESTART_VOLTAGE,
 )
 BATTERY_SHUTDOWN_VOLTAGE.max = BATTERY_LOW_VOLTAGE
@@ -207,175 +245,140 @@
     BATTERY_RESTART_VOLTAGE,
     BATTERY_LOW_VOLTAGE,
 )
 
 #################
 # System program
 #################
+
 SENSORS += SelectRWSensor(
-    243, "Priority Mode", options={0: "Battery first", 1: "Load first"}
+    141, "Priority Mode", options={0: "Battery first", 1: "Load first"}
 )
 
 SENSORS += SelectRWSensor(
-    244,
+    142,
     "Load Limit",
     options={0: "Allow Export", 1: "Essentials", 2: "Zero Export"},
 )
 
-PROG1_TIME = TimeRWSensor(250, "Prog1 Time")
-PROG2_TIME = TimeRWSensor(251, "Prog2 Time", min=PROG1_TIME)
-PROG3_TIME = TimeRWSensor(252, "Prog3 Time", min=PROG2_TIME)
-PROG4_TIME = TimeRWSensor(253, "Prog4 Time", min=PROG3_TIME)
-PROG5_TIME = TimeRWSensor(254, "Prog5 Time", min=PROG4_TIME)
-PROG6_TIME = TimeRWSensor(255, "Prog6 Time", min=PROG5_TIME)
+PROG1_TIME = TimeRWSensor(148, "Prog1 Time")
+PROG2_TIME = TimeRWSensor(149, "Prog2 Time", min=PROG1_TIME)
+PROG3_TIME = TimeRWSensor(150, "Prog3 Time", min=PROG2_TIME)
+PROG4_TIME = TimeRWSensor(151, "Prog4 Time", min=PROG3_TIME)
+PROG5_TIME = TimeRWSensor(152, "Prog5 Time", min=PROG4_TIME)
+PROG6_TIME = TimeRWSensor(153, "Prog6 Time", min=PROG5_TIME)
 PROG1_TIME.min = PROG6_TIME
 PROG1_TIME.max = PROG2_TIME
 PROG2_TIME.max = PROG3_TIME
 PROG3_TIME.max = PROG4_TIME
 PROG4_TIME.max = PROG5_TIME
 PROG5_TIME.max = PROG6_TIME
 PROG6_TIME.max = PROG1_TIME
 
 PROG_CHARGE_OPTIONS = {
-    0: "No Grid or Gen",
-    1: "Allow Grid",
-    2: "Allow Gen",
-    3: "Allow Grid & Gen",
-}
-PROG_MODE_OPTIONS = {
-    0: "None",
-    4: "General",
-    8: "Backup",
-    16: "Charge",
+    0: "Off",
+    1: "On",
 }
 
+# PROG_CHARGE_OPTIONS = {
+#     0: "No Grid or Gen",
+#     1: "Allow Grid",
+#     2: "Allow Gen",
+#     3: "Allow Grid & Gen",
+# }
+# PROG_MODE_OPTIONS = {
+#     0: "None",
+#     4: "General",
+#     8: "Backup",
+#     16: "Charge",
+# }
+
 SENSORS += (
     PROG1_TIME,
     PROG2_TIME,
     PROG3_TIME,
     PROG4_TIME,
     PROG5_TIME,
     PROG6_TIME,
-    NumberRWSensor(256, "Prog1 power", WATT, max=RATED_POWER),
-    NumberRWSensor(257, "Prog2 power", WATT, max=RATED_POWER),
-    NumberRWSensor(258, "Prog3 power", WATT, max=RATED_POWER),
-    NumberRWSensor(259, "Prog4 power", WATT, max=RATED_POWER),
-    NumberRWSensor(260, "Prog5 power", WATT, max=RATED_POWER),
-    NumberRWSensor(261, "Prog6 power", WATT, max=RATED_POWER),
-    NumberRWSensor(268, "Prog1 Capacity", "%", min=BATTERY_LOW_CAPACITY),
-    NumberRWSensor(269, "Prog2 Capacity", "%", min=BATTERY_LOW_CAPACITY),
-    NumberRWSensor(270, "Prog3 Capacity", "%", min=BATTERY_LOW_CAPACITY),
-    NumberRWSensor(271, "Prog4 Capacity", "%", min=BATTERY_LOW_CAPACITY),
-    NumberRWSensor(272, "Prog5 Capacity", "%", min=BATTERY_LOW_CAPACITY),
-    NumberRWSensor(273, "Prog6 Capacity", "%", min=BATTERY_LOW_CAPACITY),
-    SelectRWSensor(274, "Prog1 charge", options=PROG_CHARGE_OPTIONS, bitmask=0x03),
-    SelectRWSensor(275, "Prog2 charge", options=PROG_CHARGE_OPTIONS, bitmask=0x03),
-    SelectRWSensor(276, "Prog3 charge", options=PROG_CHARGE_OPTIONS, bitmask=0x03),
-    SelectRWSensor(277, "Prog4 charge", options=PROG_CHARGE_OPTIONS, bitmask=0x03),
-    SelectRWSensor(278, "Prog5 charge", options=PROG_CHARGE_OPTIONS, bitmask=0x03),
-    SelectRWSensor(279, "Prog6 charge", options=PROG_CHARGE_OPTIONS, bitmask=0x03),
-    SelectRWSensor(274, "Prog1 mode", options=PROG_MODE_OPTIONS, bitmask=0x1C),
-    SelectRWSensor(275, "Prog2 mode", options=PROG_MODE_OPTIONS, bitmask=0x1C),
-    SelectRWSensor(276, "Prog3 mode", options=PROG_MODE_OPTIONS, bitmask=0x1C),
-    SelectRWSensor(277, "Prog4 mode", options=PROG_MODE_OPTIONS, bitmask=0x1C),
-    SelectRWSensor(278, "Prog5 mode", options=PROG_MODE_OPTIONS, bitmask=0x1C),
-    SelectRWSensor(279, "Prog6 mode", options=PROG_MODE_OPTIONS, bitmask=0x1C),
+    NumberRWSensor(154, "Prog1 power", WATT, max=RATED_POWER),
+    NumberRWSensor(155, "Prog2 power", WATT, max=RATED_POWER),
+    NumberRWSensor(156, "Prog3 power", WATT, max=RATED_POWER),
+    NumberRWSensor(157, "Prog4 power", WATT, max=RATED_POWER),
+    NumberRWSensor(158, "Prog5 power", WATT, max=RATED_POWER),
+    NumberRWSensor(159, "Prog6 power", WATT, max=RATED_POWER),
+    NumberRWSensor(166, "Prog1 Capacity", "%", min=BATTERY_LOW_CAPACITY),
+    NumberRWSensor(167, "Prog2 Capacity", "%", min=BATTERY_LOW_CAPACITY),
+    NumberRWSensor(168, "Prog3 Capacity", "%", min=BATTERY_LOW_CAPACITY),
+    NumberRWSensor(169, "Prog4 Capacity", "%", min=BATTERY_LOW_CAPACITY),
+    NumberRWSensor(170, "Prog5 Capacity", "%", min=BATTERY_LOW_CAPACITY),
+    NumberRWSensor(171, "Prog6 Capacity", "%", min=BATTERY_LOW_CAPACITY),
+    SelectRWSensor(172, "Prog1 charge", options=PROG_CHARGE_OPTIONS),
+    SelectRWSensor(173, "Prog2 charge", options=PROG_CHARGE_OPTIONS),
+    SelectRWSensor(174, "Prog3 charge", options=PROG_CHARGE_OPTIONS),
+    SelectRWSensor(175, "Prog4 charge", options=PROG_CHARGE_OPTIONS),
+    SelectRWSensor(176, "Prog5 charge", options=PROG_CHARGE_OPTIONS),
+    SelectRWSensor(177, "Prog6 charge", options=PROG_CHARGE_OPTIONS),
+    # SelectRWSensor(172, "Prog1 charge", options=PROG_CHARGE_OPTIONS, bitmask=0x03),
+    # SelectRWSensor(173, "Prog2 charge", options=PROG_CHARGE_OPTIONS, bitmask=0x03),
+    # SelectRWSensor(174, "Prog3 charge", options=PROG_CHARGE_OPTIONS, bitmask=0x03),
+    # SelectRWSensor(175, "Prog4 charge", options=PROG_CHARGE_OPTIONS, bitmask=0x03),
+    # SelectRWSensor(176, "Prog5 charge", options=PROG_CHARGE_OPTIONS, bitmask=0x03),
+    # SelectRWSensor(177, "Prog6 charge", options=PROG_CHARGE_OPTIONS, bitmask=0x03),
+    # SelectRWSensor(172, "Prog1 mode", options=PROG_MODE_OPTIONS, bitmask=0x1C),
+    # SelectRWSensor(173, "Prog2 mode", options=PROG_MODE_OPTIONS, bitmask=0x1C),
+    # SelectRWSensor(174, "Prog3 mode", options=PROG_MODE_OPTIONS, bitmask=0x1C),
+    # SelectRWSensor(175, "Prog4 mode", options=PROG_MODE_OPTIONS, bitmask=0x1C),
+    # SelectRWSensor(176, "Prog5 mode", options=PROG_MODE_OPTIONS, bitmask=0x1C),
+    # SelectRWSensor(177, "Prog6 mode", options=PROG_MODE_OPTIONS, bitmask=0x1C),
 )
+
+
 SENSORS += (
     NumberRWSensor(
-        262,
+        160,
         "Prog1 voltage",
         VOLT,
         0.01,
         min=BATTERY_LOW_VOLTAGE,
         max=BATTERY_FLOAT_VOLTAGE,
     ),
     NumberRWSensor(
-        263,
+        161,
         "Prog2 voltage",
         VOLT,
         0.01,
         min=BATTERY_LOW_VOLTAGE,
         max=BATTERY_FLOAT_VOLTAGE,
     ),
     NumberRWSensor(
-        264,
+        162,
         "Prog3 voltage",
         VOLT,
         0.01,
         min=BATTERY_LOW_VOLTAGE,
         max=BATTERY_FLOAT_VOLTAGE,
     ),
     NumberRWSensor(
-        265,
+        163,
         "Prog4 voltage",
         VOLT,
         0.01,
         min=BATTERY_LOW_VOLTAGE,
         max=BATTERY_FLOAT_VOLTAGE,
     ),
     NumberRWSensor(
-        266,
+        164,
         "Prog5 voltage",
         VOLT,
         0.01,
         min=BATTERY_LOW_VOLTAGE,
         max=BATTERY_FLOAT_VOLTAGE,
     ),
     NumberRWSensor(
-        267,
+        165,
         "Prog6 voltage",
         VOLT,
         0.01,
         min=BATTERY_LOW_VOLTAGE,
         max=BATTERY_FLOAT_VOLTAGE,
     ),
 )
-
-#############
-# Inverter settings
-#############
-SENSORS += NumberRWSensor(230, "Grid Charge Battery current", AMPS, min=0, max=185)
-SENSORS += NumberRWSensor(210, "Battery Max Charge current", AMPS, min=0, max=185)
-SENSORS += NumberRWSensor(211, "Battery Max Discharge current", AMPS, min=0, max=185)
-
-#############
-# Deprecated
-#############
-
-
-def _deprecated() -> None:
-    """Populate the deprecated sensors."""
-    dep_map: dict[str, Sensor] = {
-        "aux_power": Sensor(166, "AUX load", WATT, -1),
-        "battery_temperature": TempSensor(182, "Temp Battery", CELSIUS, 0.1),
-        "dc_transformer_temperature": TempSensor(
-            90, "Temp DC transformer", CELSIUS, 0.1
-        ),
-        "environment_temperature": TempSensor(95, "Temp Environment", CELSIUS, 0.1),
-        "grid_charge_battery_current": Sensor(230, "Battery Grid Charge", AMPS, -1),
-        "grid_ct_power": Sensor(172, "Grid CT load", WATT, -1),
-        "grid_l2_power": Sensor(168, "Grid L2 load", WATT, -1),
-        "grid_ld_power": Sensor(167, "Grid L1 load", WATT, -1),
-        "grid_power": Sensor(169, "Grid load", WATT, -1),
-        "inverter_power": Sensor(175, "Inverter Output", WATT, -1),
-        "radiator_temperature": TempSensor(91, "Temp Radiator", CELSIUS, 0.1),
-        "day_active_energy": Sensor(60, "Day Active Power", KWH, -0.1),
-        "day_reactive_energy": Sensor(61, "Day Reactive Power", "kVarh", -0.1),
-        "total_active_energy": Sensor((63, 64), "Total Active Power", KWH, 0.1),
-        "month_pv_energy": Sensor(65, "Month PV Power", KWH),
-        "month_load_energy": Sensor(66, "Month Load Power", KWH),
-        "month_grid_energy": Sensor(67, "Month Grid Power", KWH),
-        "year_pv_energy": Sensor((68, 69), "Year PV Power", KWH, 0.1),
-        "day_load_energy": Sensor(84, "Day Load Power", KWH, 0.1),
-        "total_load_energy": Sensor((85, 86), "Total Load Power", KWH, 0.1),
-        "year_load_energy": Sensor((87, 88), "Year Load Power", KWH, 0.1),
-        "total_pv_energy": Sensor((96, 97), "Total PV Power", KWH, 0.1),
-        "battery_equalization_voltage": Sensor(201, "Equalization voltage", VOLT, 0.01),
-        "battery_absorption_voltage": Sensor(202, "Absorption voltage", VOLT, 0.01),
-    }
-
-    for newname, sen in dep_map.items():
-        SENSORS.deprecated[sen.id] = SENSORS.all[newname]
-
-
-_deprecated()
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `sunsynk-0.3.3/sunsynk/definitions3ph.py` & `sunsynk-0.3.4/sunsynk/definitions.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,14 +1,13 @@
-"""Sunsynk 5kW&8kW hybrid 3-phase inverter sensor definitions."""
-# pylint: disable=duplicate-code
+"""Sunsynk 5kW&8kW hybrid inverter sensor definitions."""
 from sunsynk import AMPS, CELSIUS, KWH, VOLT, WATT
 from sunsynk.rwsensors import (
     NumberRWSensor,
     SelectRWSensor,
-    SwitchRWSensor,
+    SystemTimeRWSensor,
     TimeRWSensor,
 )
 from sunsynk.sensors import (
     FaultSensor,
     InverterStateSensor,
     MathSensor,
     SDStatusSensor,
@@ -20,365 +19,325 @@
 
 SENSORS = SensorDefinitions()
 
 ##########
 # Battery
 ##########
 SENSORS += (
-    TempSensor(586, "Battery temperature", CELSIUS, 0.1),
-    Sensor(587, "Battery voltage", VOLT, 0.01),
-    Sensor(588, "Battery SOC", "%"),
-    Sensor(590, "Battery power", WATT, -1),
-    Sensor(591, "Battery current", AMPS, -0.01),
+    TempSensor(182, "Battery temperature", CELSIUS, 0.1),
+    Sensor(183, "Battery voltage", VOLT, 0.01),
+    Sensor(184, "Battery SOC", "%"),
+    Sensor(190, "Battery power", WATT, -1),
+    Sensor(191, "Battery current", AMPS, -0.01),
 )
 
 #################
 # Inverter Power
 #################
 SENSORS += (
-    Sensor(636, "Inverter power", WATT, -1),
-    Sensor(633, "Inverter L1 power", WATT, -1),
-    Sensor(634, "Inverter L2 power", WATT, -1),
-    Sensor(635, "Inverter L3 power", WATT, -1),
-    Sensor(627, "Inverter voltage", VOLT, 0.1),
-    Sensor(638, "Inverter frequency", "Hz", 0.01),
+    Sensor(175, "Inverter power", WATT, -1),
+    Sensor(154, "Inverter voltage", VOLT, 0.1),
+    Sensor(193, "Inverter frequency", "Hz", 0.01),
 )
 
 #############
 # Grid Power
 #############
 SENSORS += (
-    Sensor(609, "Grid frequency", "Hz", 0.01),
-    Sensor(625, "Grid power", WATT, -1),  # gridTotalPac
-    Sensor(622, "Grid L1 power", WATT, -1),  # aPower
-    Sensor(623, "Grid L2 power", WATT, -1),  # bPower
-    Sensor(624, "Grid L3 power", WATT, -1),  # cPower
-    Sensor(600, "Grid voltage", VOLT, 0.1),  # aLineVolt
-    MathSensor(
-        (610, 611, 612), "Grid current", AMPS, factors=(0.01, 0.01, 0.01)
-    ),  # iac1,iac2,iac3
-    Sensor(619, "Grid CT power", WATT, -1),  # gridOutsideTotalPac (unsure ??)
+    Sensor(79, "Grid frequency", "Hz", 0.01),
+    Sensor(169, "Grid power", WATT, -1),  # L1(167) + L2(168)
+    Sensor(167, "Grid LD power", WATT, -1),  # L1 seems to be LD
+    Sensor(168, "Grid L2 power", WATT, -1),
+    Sensor(150, "Grid voltage", VOLT, 0.1),
+    MathSensor((160, 161), "Grid current", AMPS, factors=(0.01, 0.01)),
+    Sensor(172, "Grid CT power", WATT, -1),
 )
+# LD power?
 
 #############
 # Load Power
 #############
 SENSORS += (
-    Sensor(653, "Load power", WATT, -1),
-    Sensor(650, "Load L1 power", WATT, -1),
-    Sensor(651, "Load L2 power", WATT, -1),
-    Sensor(652, "Load L3 power", WATT, -1),
+    Sensor(178, "Load power", WATT, -1),  # L1(176) + L2(177)
+    Sensor(176, "Load L1 power", WATT, -1),
+    Sensor(177, "Load L2 power", WATT, -1),
 )
 
 ################
 # Solar Power 1
 ################
 SENSORS += (
-    Sensor(672, "PV1 power", WATT, -1),
-    Sensor(676, "PV1 voltage", VOLT, 0.1),
-    Sensor(677, "PV1 current", AMPS, 0.1),
+    Sensor(186, "PV1 power", WATT, -1),
+    Sensor(109, "PV1 voltage", VOLT, 0.1),
+    Sensor(110, "PV1 current", AMPS, 0.1),
 )
 
 ################
 # Solar Power 2
 ################
 SENSORS += (
-    Sensor(673, "PV2 power", WATT, -1),
-    Sensor(678, "PV2 voltage", VOLT, 0.1),
-    Sensor(679, "PV2 current", AMPS, 0.1),
-)
-
-################
-# Solar Power 3 (?? deye 3 Phase  only has 2 MPPT)
-################
-SENSORS += (
-    Sensor(674, "PV3 power", WATT, -1),
-    Sensor(680, "PV3 voltage", VOLT, 0.1),
-    Sensor(681, "PV3 current", AMPS, 0.1),
+    Sensor(187, "PV2 power", WATT, -1),
+    Sensor(111, "PV2 voltage", VOLT, 0.1),
+    Sensor(112, "PV2 current", AMPS, 0.1),
 )
 
-################
-# Solar Power 4 (?? deye 3 Phase  only has 2 MPPT)
-################
-SENSORS += (
-    Sensor(675, "PV4 power", WATT, -1),
-    Sensor(682, "PV4 voltage", VOLT, 0.1),
-    Sensor(683, "PV4 current", AMPS, 0.1),
-)
-
-
 ###################
-# Power on Outputs (aka GEN - which has multiple modes on the deye 3 Phase )
+# Power on Outputs
 ###################
 SENSORS += (
-    Sensor(667, "Gen power", WATT, -1),
-    Sensor(664, "Gen L1 power", WATT, -1),
-    Sensor(665, "Gen L2 power", WATT, -1),
-    Sensor(666, "Gen L3 power", WATT, -1),
+    Sensor(166, "AUX power", WATT, -1),
+    # https://github.com/kellerza/sunsynk/issues/75
+    #  https://powerforum.co.za/topic/8646-my-sunsynk-8kw-data-collection-setup/?do=findComment&comment=147591
+    MathSensor(
+        (175, 169, 166), "Essential power", WATT, factors=(1, 1, -1), absolute=True
+    ),
+    # MathSensor((175, 167, 166), "Essential power", WATT, factors=(1, 1, -1)),
+    MathSensor(
+        (172, 167), "Non-Essential power", WATT, factors=(1, -1), no_negative=True
+    ),
 )
 
 ###################
 # Energy
 ###################
 SENSORS += (
-    Sensor(502, "Day Active Energy", KWH, -0.1),
-    Sensor(514, "Day Battery Charge", KWH, 0.1),
-    Sensor(515, "Day Battery discharge", KWH, 0.1),
-    Sensor(521, "Day Grid Export", KWH, 0.1),
-    Sensor(520, "Day Grid Import", KWH, 0.1),
-    Sensor(536, "Day Gen Energy", KWH, 0.1),
-    Sensor(526, "Day Load Energy", KWH, 0.1),  # I guess "used" = load?
-    Sensor(529, "Day PV Energy", KWH, 0.1),
-    Sensor((506, 507), "Total Active Energy", KWH, 0.1),  # signed?
-    Sensor((516, 517), "Total Battery Charge", KWH, 0.1),
-    Sensor((518, 519), "Total Battery Discharge", KWH, 0.1),
-    Sensor((524, 525), "Total Grid Export", KWH, 0.1),
-    Sensor((522, 523), "Total Grid Import", KWH, 0.1),
-    Sensor((527, 528), "Total Load Energy", KWH, 0.1),
-    Sensor((534, 535), "Total PV Energy", KWH, 0.1),
+    Sensor(60, "Day Active Energy", KWH, -0.1),
+    Sensor(70, "Day Battery Charge", KWH, 0.1),
+    Sensor(71, "Day Battery Discharge", KWH, 0.1),
+    Sensor(77, "Day Grid Export", KWH, 0.1),
+    Sensor(76, "Day Grid Import", KWH, 0.1),
+    # Sensor(200, "Day Load Power", KWH, 0.01),
+    Sensor(84, "Day Load Energy", KWH, 0.1),
+    Sensor(108, "Day PV Energy", KWH, 0.1),
+    Sensor(61, "Day Reactive Energy", "kVarh", -0.1),
+    # Sensor((201, 202), "History Load Power", KWH, 0.1),
+    Sensor(67, "Month Grid Energy", KWH, 0.1),
+    Sensor(66, "Month Load Energy", KWH, 0.1),
+    Sensor(65, "Month PV Energy", KWH, 0.1),
+    Sensor((63, 64), "Total Active Energy", KWH, 0.1),  # signed?
+    Sensor((72, 73), "Total Battery Charge", KWH, 0.1),
+    Sensor((74, 75), "Total Battery Discharge", KWH, 0.1),
+    Sensor((81, 82), "Total Grid Export", KWH, 0.1),
+    Sensor((78, 80), "Total Grid Import", KWH, 0.1),
+    Sensor((85, 86), "Total Load Energy", KWH, 0.1),
+    Sensor((96, 97), "Total PV Energy", KWH, 0.1),
+    Sensor((98, 99), "Year Grid Export", KWH, 0.1),
+    Sensor((87, 88), "Year Load Energy", KWH, 0.1),
+    Sensor((68, 69), "Year PV Energy", KWH, 0.1),
 )
 
 ##########
 # General
 ##########
-RATED_POWER = Sensor((20, 21), "Rated power", WATT, 0.1)
-SENSORS += RATED_POWER
-
+RATED_POWER = Sensor((16, 17), "Rated power", WATT, 0.1)
 SENSORS += (
-    Sensor(
-        0, "Device Type"
-    ),  # {2: "Inverter", 3: "Hybrid Inverter", 4: "Micro Inverter", 5: "3 Phase Hybrid Inverter" }),
-    FaultSensor((555, 556, 557, 558), "Fault"),
-    InverterStateSensor(500, "Overall state"),
-    SDStatusSensor(0, "SD Status", ""),  # type: ignore        # 3 Phase does not have SD Card but crashes when removed
+    RATED_POWER,
     SerialSensor((3, 4, 5, 6, 7), "Serial"),
-    TempSensor(540, "DC transformer temperature", CELSIUS, 0.1),
-    TempSensor(541, "Radiator temperature", CELSIUS, 0.1),
-    Sensor(
-        552, "Grid Connected Status"
-    ),  # Bit 0 = INV Relay, 1 = Undef, 2 = Grid relay, 3 = Gen relay, 4 = Grid give, 5, Dry contact
+    Sensor(0, "Device Type"),
+    FaultSensor((103, 104, 105, 106), "Fault"),
+    InverterStateSensor(59, "Overall state"),
+    SDStatusSensor(92, "SD Status", ""),  # type: ignore
+    TempSensor(90, "DC transformer temperature", CELSIUS, 0.1),
+    TempSensor(95, "Environment temperature", CELSIUS, 0.1),
+    TempSensor(91, "Radiator temperature", CELSIUS, 0.1),
+    Sensor(194, "Grid Connected Status"),
+    SystemTimeRWSensor((22, 23, 24), "Date Time", unit=""),
 )
-
-
 ###########
 # Settings
 ###########
 SENSORS += (
-    NumberRWSensor(128, "Grid Charge Battery current", AMPS, max=210),
-    SwitchRWSensor(130, "Grid Charge enabled"),
-    SwitchRWSensor(146, "Use Timer", on=255),
-    SwitchRWSensor(145, "Solar Export"),
-    NumberRWSensor(143, "Export Limit power", WATT, max=RATED_POWER),
-    NumberRWSensor(108, "Battery Max Charge current", AMPS, max=210),
-    NumberRWSensor(109, "Battery Max Discharge current", AMPS, max=210),
-    NumberRWSensor(102, "Battery Capacity current", AMPS, max=2000),
+    Sensor(200, "Control Mode"),
+    Sensor(232, "Grid Charge enabled", "", -1),
+    Sensor(312, "Battery charging voltage", VOLT, 0.01),
+    Sensor(603, "Bat1 SOC", "%"),
+    Sensor(611, "Bat1 Cycle"),
 )
 
-# Additional optional sensors
-SENSORS += (
-    NumberRWSensor(
-        103, "Battery low voltage", VOLT, -0.1
-    ),  # interesting perhaps not available in menu. default 4500 (45V)
-    SelectRWSensor(
-        133,
-        "Generator Port Usage",
-        options={0: "Generator", 1: "Smartload", 2: "Micro Inverter"},
-    ),
-    SelectRWSensor(129, "Generator Charge enabled", options={0: "Off", 1: "On"}),
-    SelectRWSensor(112, "Battery Activate", options={0: "Off", 1: "On"}),
-    NumberRWSensor(113, "Battery Resistance", "mΩ", max=6000),
-    NumberRWSensor(104, "System Zero Export power", WATT, -1),
-    NumberRWSensor(105, "Battery Equalization Days", "days", -1),
-    NumberRWSensor(106, "Battery Equalization Hours", "h", -1),  # 1 = 0.5 hours
+# Battery capacity (if managed by BMS)
+BATTERY_LOW_CAP = NumberRWSensor(219, "Battery Low Capacity", "%", max=50)
+BATTERY_SHUTDOWN_CAP = NumberRWSensor(
+    217, "Battery Shutdown Capacity", "%", max=BATTERY_LOW_CAP
+)
+BATTERY_LOW_CAP.min = BATTERY_SHUTDOWN_CAP
+BATTERY_RESTART_CAP = NumberRWSensor(
+    218, "Battery Restart Capacity", "%", min=BATTERY_SHUTDOWN_CAP
 )
 
 # Absolute min and max voltage based on Deye inverter
-MIN_VOLTAGE = 41
-MAX_VOLTAGE = 60
+MIN_VOLT = 41
+MAX_VOLT = 60
 
-BATTERY_EQUALIZATION_VOLTAGE = NumberRWSensor(
-    99, "Battery Equalization voltage", VOLT, 0.01, min=MIN_VOLTAGE, max=MAX_VOLTAGE
+# Battery voltage (if managed by voltage only)
+BATTERY_SHUTDOWN_VOLT = NumberRWSensor(
+    220, "Battery Shutdown voltage", VOLT, 0.01, min=MIN_VOLT
 )
-BATTERY_ABSORPTION_VOLTAGE = NumberRWSensor(
-    100, "Battery Absorption voltage", VOLT, 0.01, min=MIN_VOLTAGE, max=MAX_VOLTAGE
+BATTERY_LOW_VOLT = NumberRWSensor(
+    222, "Battery Low voltage", VOLT, 0.01, min=BATTERY_SHUTDOWN_VOLT, max=MAX_VOLT
 )
-BATTERY_FLOAT_VOLTAGE = NumberRWSensor(
-    101, "Battery Float voltage", VOLT, 0.01, min=MIN_VOLTAGE, max=MAX_VOLTAGE
-)
-
-BATTERY_SHUTDOWN_CAPACITY = NumberRWSensor(115, "Battery Shutdown Capacity", "%")
-BATTERY_RESTART_CAPACITY = NumberRWSensor(116, "Battery Restart Capacity", "%")
-BATTERY_LOW_CAPACITY = NumberRWSensor(
-    117,
-    "Battery Low Capacity",
-    "%",
-    min=BATTERY_SHUTDOWN_CAPACITY,
-    max=BATTERY_RESTART_CAPACITY,
-)
-BATTERY_SHUTDOWN_CAPACITY.max = BATTERY_LOW_CAPACITY
-BATTERY_RESTART_CAPACITY.min = BATTERY_LOW_CAPACITY
-
-BATTERY_SHUTDOWN_VOLTAGE = NumberRWSensor(
-    118, "Battery Shutdown voltage", VOLT, 0.01, min=MIN_VOLTAGE
-)
-BATTERY_RESTART_VOLTAGE = NumberRWSensor(
-    119, "Battery Restart voltage", VOLT, 0.01, max=MAX_VOLTAGE
-)
-BATTERY_LOW_VOLTAGE = NumberRWSensor(
-    120,
-    "Battery Low voltage",
-    VOLT,
-    0.01,
-    min=BATTERY_SHUTDOWN_VOLTAGE,
-    max=BATTERY_RESTART_VOLTAGE,
-)
-BATTERY_SHUTDOWN_VOLTAGE.max = BATTERY_LOW_VOLTAGE
-BATTERY_RESTART_VOLTAGE.min = BATTERY_LOW_VOLTAGE
-
-SENSORS += (
-    BATTERY_EQUALIZATION_VOLTAGE,
-    BATTERY_ABSORPTION_VOLTAGE,
-    BATTERY_FLOAT_VOLTAGE,
-    BATTERY_SHUTDOWN_CAPACITY,
-    BATTERY_RESTART_CAPACITY,
-    BATTERY_LOW_CAPACITY,
-    BATTERY_SHUTDOWN_VOLTAGE,
-    BATTERY_RESTART_VOLTAGE,
-    BATTERY_LOW_VOLTAGE,
+BATTERY_RESTART_VOLT = NumberRWSensor(
+    221, "Battery Restart voltage", VOLT, 0.01, max=MAX_VOLT, min=BATTERY_SHUTDOWN_VOLT
+)
+
+
+BATTERY_EQUALIZATION_VOLT = NumberRWSensor(
+    201, "Battery Equalization voltage", VOLT, 0.01, min=MIN_VOLT, max=MAX_VOLT
+)
+BATTERY_ABSORPTION_VOLT = NumberRWSensor(
+    202, "Battery Absorption voltage", VOLT, 0.01, min=MIN_VOLT, max=MAX_VOLT
+)
+BATTERY_FLOAT_VOLT = NumberRWSensor(
+    203, "Battery Float voltage", VOLT, 0.01, min=MIN_VOLT, max=MAX_VOLT
+)
+
+SENSORS += (
+    BATTERY_EQUALIZATION_VOLT,
+    BATTERY_ABSORPTION_VOLT,
+    BATTERY_FLOAT_VOLT,
+    BATTERY_SHUTDOWN_CAP,
+    BATTERY_RESTART_CAP,
+    BATTERY_LOW_CAP,
+    BATTERY_SHUTDOWN_VOLT,
+    BATTERY_RESTART_VOLT,
+    BATTERY_LOW_VOLT,
 )
 
 #################
 # System program
 #################
-
 SENSORS += SelectRWSensor(
-    141, "Priority Mode", options={0: "Battery first", 1: "Load first"}
+    243, "Priority Mode", options={0: "Battery first", 1: "Load first"}
 )
 
 SENSORS += SelectRWSensor(
-    142,
+    244,
     "Load Limit",
     options={0: "Allow Export", 1: "Essentials", 2: "Zero Export"},
 )
 
-PROG1_TIME = TimeRWSensor(148, "Prog1 Time")
-PROG2_TIME = TimeRWSensor(149, "Prog2 Time", min=PROG1_TIME)
-PROG3_TIME = TimeRWSensor(150, "Prog3 Time", min=PROG2_TIME)
-PROG4_TIME = TimeRWSensor(151, "Prog4 Time", min=PROG3_TIME)
-PROG5_TIME = TimeRWSensor(152, "Prog5 Time", min=PROG4_TIME)
-PROG6_TIME = TimeRWSensor(153, "Prog6 Time", min=PROG5_TIME)
+PROG1_TIME = TimeRWSensor(250, "Prog1 Time")
+PROG2_TIME = TimeRWSensor(251, "Prog2 Time", min=PROG1_TIME)
+PROG3_TIME = TimeRWSensor(252, "Prog3 Time", min=PROG2_TIME)
+PROG4_TIME = TimeRWSensor(253, "Prog4 Time", min=PROG3_TIME)
+PROG5_TIME = TimeRWSensor(254, "Prog5 Time", min=PROG4_TIME)
+PROG6_TIME = TimeRWSensor(255, "Prog6 Time", min=PROG5_TIME)
 PROG1_TIME.min = PROG6_TIME
 PROG1_TIME.max = PROG2_TIME
 PROG2_TIME.max = PROG3_TIME
 PROG3_TIME.max = PROG4_TIME
 PROG4_TIME.max = PROG5_TIME
 PROG5_TIME.max = PROG6_TIME
 PROG6_TIME.max = PROG1_TIME
 
 PROG_CHARGE_OPTIONS = {
-    0: "Off",
-    1: "On",
+    0: "No Grid or Gen",
+    1: "Allow Grid",
+    2: "Allow Gen",
+    3: "Allow Grid & Gen",
+}
+PROG_MODE_OPTIONS = {
+    0: "None",
+    4: "General",
+    8: "Backup",
+    16: "Charge",
 }
-
-# PROG_CHARGE_OPTIONS = {
-#     0: "No Grid or Gen",
-#     1: "Allow Grid",
-#     2: "Allow Gen",
-#     3: "Allow Grid & Gen",
-# }
-# PROG_MODE_OPTIONS = {
-#     0: "None",
-#     4: "General",
-#     8: "Backup",
-#     16: "Charge",
-# }
 
 SENSORS += (
     PROG1_TIME,
     PROG2_TIME,
     PROG3_TIME,
     PROG4_TIME,
     PROG5_TIME,
     PROG6_TIME,
-    NumberRWSensor(154, "Prog1 power", WATT, max=RATED_POWER),
-    NumberRWSensor(155, "Prog2 power", WATT, max=RATED_POWER),
-    NumberRWSensor(156, "Prog3 power", WATT, max=RATED_POWER),
-    NumberRWSensor(157, "Prog4 power", WATT, max=RATED_POWER),
-    NumberRWSensor(158, "Prog5 power", WATT, max=RATED_POWER),
-    NumberRWSensor(159, "Prog6 power", WATT, max=RATED_POWER),
-    NumberRWSensor(166, "Prog1 Capacity", "%", min=BATTERY_LOW_CAPACITY),
-    NumberRWSensor(167, "Prog2 Capacity", "%", min=BATTERY_LOW_CAPACITY),
-    NumberRWSensor(168, "Prog3 Capacity", "%", min=BATTERY_LOW_CAPACITY),
-    NumberRWSensor(169, "Prog4 Capacity", "%", min=BATTERY_LOW_CAPACITY),
-    NumberRWSensor(170, "Prog5 Capacity", "%", min=BATTERY_LOW_CAPACITY),
-    NumberRWSensor(171, "Prog6 Capacity", "%", min=BATTERY_LOW_CAPACITY),
-    SelectRWSensor(172, "Prog1 charge", options=PROG_CHARGE_OPTIONS),
-    SelectRWSensor(173, "Prog2 charge", options=PROG_CHARGE_OPTIONS),
-    SelectRWSensor(174, "Prog3 charge", options=PROG_CHARGE_OPTIONS),
-    SelectRWSensor(175, "Prog4 charge", options=PROG_CHARGE_OPTIONS),
-    SelectRWSensor(176, "Prog5 charge", options=PROG_CHARGE_OPTIONS),
-    SelectRWSensor(177, "Prog6 charge", options=PROG_CHARGE_OPTIONS),
-    # SelectRWSensor(172, "Prog1 charge", options=PROG_CHARGE_OPTIONS, bitmask=0x03),
-    # SelectRWSensor(173, "Prog2 charge", options=PROG_CHARGE_OPTIONS, bitmask=0x03),
-    # SelectRWSensor(174, "Prog3 charge", options=PROG_CHARGE_OPTIONS, bitmask=0x03),
-    # SelectRWSensor(175, "Prog4 charge", options=PROG_CHARGE_OPTIONS, bitmask=0x03),
-    # SelectRWSensor(176, "Prog5 charge", options=PROG_CHARGE_OPTIONS, bitmask=0x03),
-    # SelectRWSensor(177, "Prog6 charge", options=PROG_CHARGE_OPTIONS, bitmask=0x03),
-    # SelectRWSensor(172, "Prog1 mode", options=PROG_MODE_OPTIONS, bitmask=0x1C),
-    # SelectRWSensor(173, "Prog2 mode", options=PROG_MODE_OPTIONS, bitmask=0x1C),
-    # SelectRWSensor(174, "Prog3 mode", options=PROG_MODE_OPTIONS, bitmask=0x1C),
-    # SelectRWSensor(175, "Prog4 mode", options=PROG_MODE_OPTIONS, bitmask=0x1C),
-    # SelectRWSensor(176, "Prog5 mode", options=PROG_MODE_OPTIONS, bitmask=0x1C),
-    # SelectRWSensor(177, "Prog6 mode", options=PROG_MODE_OPTIONS, bitmask=0x1C),
+    NumberRWSensor(256, "Prog1 power", WATT, max=RATED_POWER),
+    NumberRWSensor(257, "Prog2 power", WATT, max=RATED_POWER),
+    NumberRWSensor(258, "Prog3 power", WATT, max=RATED_POWER),
+    NumberRWSensor(259, "Prog4 power", WATT, max=RATED_POWER),
+    NumberRWSensor(260, "Prog5 power", WATT, max=RATED_POWER),
+    NumberRWSensor(261, "Prog6 power", WATT, max=RATED_POWER),
+    NumberRWSensor(268, "Prog1 Capacity", "%", min=BATTERY_LOW_CAP),
+    NumberRWSensor(269, "Prog2 Capacity", "%", min=BATTERY_LOW_CAP),
+    NumberRWSensor(270, "Prog3 Capacity", "%", min=BATTERY_LOW_CAP),
+    NumberRWSensor(271, "Prog4 Capacity", "%", min=BATTERY_LOW_CAP),
+    NumberRWSensor(272, "Prog5 Capacity", "%", min=BATTERY_LOW_CAP),
+    NumberRWSensor(273, "Prog6 Capacity", "%", min=BATTERY_LOW_CAP),
+    SelectRWSensor(274, "Prog1 charge", options=PROG_CHARGE_OPTIONS, bitmask=0x03),
+    SelectRWSensor(275, "Prog2 charge", options=PROG_CHARGE_OPTIONS, bitmask=0x03),
+    SelectRWSensor(276, "Prog3 charge", options=PROG_CHARGE_OPTIONS, bitmask=0x03),
+    SelectRWSensor(277, "Prog4 charge", options=PROG_CHARGE_OPTIONS, bitmask=0x03),
+    SelectRWSensor(278, "Prog5 charge", options=PROG_CHARGE_OPTIONS, bitmask=0x03),
+    SelectRWSensor(279, "Prog6 charge", options=PROG_CHARGE_OPTIONS, bitmask=0x03),
+    SelectRWSensor(274, "Prog1 mode", options=PROG_MODE_OPTIONS, bitmask=0x1C),
+    SelectRWSensor(275, "Prog2 mode", options=PROG_MODE_OPTIONS, bitmask=0x1C),
+    SelectRWSensor(276, "Prog3 mode", options=PROG_MODE_OPTIONS, bitmask=0x1C),
+    SelectRWSensor(277, "Prog4 mode", options=PROG_MODE_OPTIONS, bitmask=0x1C),
+    SelectRWSensor(278, "Prog5 mode", options=PROG_MODE_OPTIONS, bitmask=0x1C),
+    SelectRWSensor(279, "Prog6 mode", options=PROG_MODE_OPTIONS, bitmask=0x1C),
 )
-
-
 SENSORS += (
     NumberRWSensor(
-        160,
-        "Prog1 voltage",
-        VOLT,
-        0.01,
-        min=BATTERY_LOW_VOLTAGE,
-        max=BATTERY_FLOAT_VOLTAGE,
+        262, "Prog1 voltage", VOLT, 0.01, min=BATTERY_LOW_VOLT, max=BATTERY_FLOAT_VOLT
     ),
     NumberRWSensor(
-        161,
-        "Prog2 voltage",
-        VOLT,
-        0.01,
-        min=BATTERY_LOW_VOLTAGE,
-        max=BATTERY_FLOAT_VOLTAGE,
+        263, "Prog2 voltage", VOLT, 0.01, min=BATTERY_LOW_VOLT, max=BATTERY_FLOAT_VOLT
     ),
     NumberRWSensor(
-        162,
-        "Prog3 voltage",
-        VOLT,
-        0.01,
-        min=BATTERY_LOW_VOLTAGE,
-        max=BATTERY_FLOAT_VOLTAGE,
+        264, "Prog3 voltage", VOLT, 0.01, min=BATTERY_LOW_VOLT, max=BATTERY_FLOAT_VOLT
     ),
     NumberRWSensor(
-        163,
-        "Prog4 voltage",
-        VOLT,
-        0.01,
-        min=BATTERY_LOW_VOLTAGE,
-        max=BATTERY_FLOAT_VOLTAGE,
+        265, "Prog4 voltage", VOLT, 0.01, min=BATTERY_LOW_VOLT, max=BATTERY_FLOAT_VOLT
     ),
     NumberRWSensor(
-        164,
-        "Prog5 voltage",
-        VOLT,
-        0.01,
-        min=BATTERY_LOW_VOLTAGE,
-        max=BATTERY_FLOAT_VOLTAGE,
+        266, "Prog5 voltage", VOLT, 0.01, min=BATTERY_LOW_VOLT, max=BATTERY_FLOAT_VOLT
     ),
     NumberRWSensor(
-        165,
-        "Prog6 voltage",
-        VOLT,
-        0.01,
-        min=BATTERY_LOW_VOLTAGE,
-        max=BATTERY_FLOAT_VOLTAGE,
+        267, "Prog6 voltage", VOLT, 0.01, min=BATTERY_LOW_VOLT, max=BATTERY_FLOAT_VOLT
     ),
 )
+
+#############
+# Inverter settings
+#############
+SENSORS += NumberRWSensor(230, "Grid Charge Battery current", AMPS, min=0, max=185)
+SENSORS += NumberRWSensor(210, "Battery Max Charge current", AMPS, min=0, max=185)
+SENSORS += NumberRWSensor(211, "Battery Max Discharge current", AMPS, min=0, max=185)
+
+
+#############
+# Deprecated
+#############
+def _deprecated() -> None:
+    """Populate the deprecated sensors."""
+    dep_map: dict[str, Sensor] = {
+        "aux_power": Sensor(166, "AUX load", WATT, -1),
+        "battery_temperature": TempSensor(182, "Temp Battery", CELSIUS, 0.1),
+        "dc_transformer_temperature": TempSensor(
+            90, "Temp DC transformer", CELSIUS, 0.1
+        ),
+        "environment_temperature": TempSensor(95, "Temp Environment", CELSIUS, 0.1),
+        "grid_charge_battery_current": Sensor(230, "Battery Grid Charge", AMPS, -1),
+        "grid_ct_power": Sensor(172, "Grid CT load", WATT, -1),
+        "grid_l2_power": Sensor(168, "Grid L2 load", WATT, -1),
+        "grid_ld_power": Sensor(167, "Grid L1 load", WATT, -1),
+        "grid_power": Sensor(169, "Grid load", WATT, -1),
+        "inverter_power": Sensor(175, "Inverter Output", WATT, -1),
+        "radiator_temperature": TempSensor(91, "Temp Radiator", CELSIUS, 0.1),
+        "day_active_energy": Sensor(60, "Day Active Power", KWH, -0.1),
+        "day_reactive_energy": Sensor(61, "Day Reactive Power", "kVarh", -0.1),
+        "total_active_energy": Sensor((63, 64), "Total Active Power", KWH, 0.1),
+        "month_pv_energy": Sensor(65, "Month PV Power", KWH),
+        "month_load_energy": Sensor(66, "Month Load Power", KWH),
+        "month_grid_energy": Sensor(67, "Month Grid Power", KWH),
+        "year_pv_energy": Sensor((68, 69), "Year PV Power", KWH, 0.1),
+        "day_load_energy": Sensor(84, "Day Load Power", KWH, 0.1),
+        "total_load_energy": Sensor((85, 86), "Total Load Power", KWH, 0.1),
+        "year_load_energy": Sensor((87, 88), "Year Load Power", KWH, 0.1),
+        "total_pv_energy": Sensor((96, 97), "Total PV Power", KWH, 0.1),
+        "battery_equalization_voltage": Sensor(201, "Equalization voltage", VOLT, 0.01),
+        "battery_absorption_voltage": Sensor(202, "Absorption voltage", VOLT, 0.01),
+    }
+
+    for newname, sen in dep_map.items():
+        SENSORS.deprecated[sen.id] = SENSORS.all[newname]
+
+
+_deprecated()
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `sunsynk-0.3.3/sunsynk/pysunsynk.py` & `sunsynk-0.3.4/sunsynk/pysunsynk.py`

 * *Files identical despite different names*

### Comparing `sunsynk-0.3.3/sunsynk/rwsensors.py` & `sunsynk-0.3.4/sunsynk/rwsensors.py`

 * *Files 0% similar despite different names*

```diff
@@ -129,16 +129,14 @@
         self.options = {self.off: "OFF", self.on: "ON"}
 
 
 @attrs.define(slots=True, eq=False)
 class SystemTimeRWSensor(RWSensor):
     """Read & write time sensor."""
 
-    _path = "text"
-
     def value_to_reg(self, value: ValType, resolve: ResolveType) -> RegType:
         """Get the reg value from a display value."""
         # pylint: disable=invalid-name
         redt = re.compile(r"(2\d{3})-(\d{2})-(\d{2}) (\d{2}):(\d{2}):(\d{2})")
         match = redt.fullmatch(str(value).strip())
         if not match:
             raise ValueError("Invalid datetime {value}")
```

### Comparing `sunsynk-0.3.3/sunsynk/sensors.py` & `sunsynk-0.3.4/sunsynk/sensors.py`

 * *Files 1% similar despite different names*

```diff
@@ -56,15 +56,15 @@
     def __hash__(self) -> int:
         """Hash the sensor id."""
         return hash(self.id)
 
     def __eq__(self, other: object) -> bool:
         """Sensor equality is based on the ID only."""
         if not isinstance(other, Sensor):
-            raise TypeError
+            raise TypeError(str(type(other)))
         return self.id == other.id
 
 
 @attrs.define(slots=True)
 class SensorDefinitions:
     """Definitions."""
```

### Comparing `sunsynk-0.3.3/sunsynk/state.py` & `sunsynk-0.3.4/sunsynk/state.py`

 * *Files identical despite different names*

### Comparing `sunsynk-0.3.3/sunsynk/sunsynk.py` & `sunsynk-0.3.4/sunsynk/sunsynk.py`

 * *Files identical despite different names*

### Comparing `sunsynk-0.3.3/sunsynk/usunsynk.py` & `sunsynk-0.3.4/sunsynk/usunsynk.py`

 * *Files identical despite different names*

### Comparing `sunsynk-0.3.3/sunsynk.egg-info/PKG-INFO` & `sunsynk-0.3.4/sunsynk.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sunsynk
-Version: 0.3.3
+Version: 0.3.4
 Summary: Library to interface Deye/Sunsynk Hybrid Inverters
 Home-page: https://kellerza.github.io/sunsynk/
 Author: Johann Kellerman
 Author-email: kellerza@gmail.com
 License: MIT
 Keywords: sunsynk,deye,inverter,modbus,asyncio
 Classifier: Development Status :: 4 - Beta
@@ -51,12 +51,11 @@
 
 
 Below an example of the HomeAssistant Energy management dashboard using sensors from the Sunsynk.
 
 ![HASS Energy management](https://github.com/kellerza/sunsynk/raw/main/images/energy.png)
 
 ## Sunsynk Python Library
-
 [![PyPI version](https://badge.fury.io/py/sunsynk.svg)](https://pypi.org/project/sunsynk/)
 [![codecov](https://codecov.io/gh/kellerza/sunsynk/branch/main/graph/badge.svg?token=ILKRC5UTXI)](https://codecov.io/gh/kellerza/sunsynk)
 
 The Python library is available through pip: `pip install sunsynk`
```

### Comparing `sunsynk-0.3.3/sunsynk.egg-info/SOURCES.txt` & `sunsynk-0.3.4/sunsynk.egg-info/SOURCES.txt`

 * *Files 3% similar despite different names*

```diff
@@ -24,14 +24,15 @@
 tests/conftest.py
 tests/hass-addon-sunsynk-dev.zip
 tests/hass-addon-sunsynk.zip
 tests/hass_addon_sunsynk_multi/__init__.py
 tests/hass_addon_sunsynk_multi/test_definitions3ph.py
 tests/hass_addon_sunsynk_multi/test_filter.py
 tests/hass_addon_sunsynk_multi/test_run.py
+tests/hass_addon_sunsynk_multi/test_sensors.py
 tests/hass_addon_sunsynk_multi/test_state.py
 tests/sunsynk/__init__.py
 tests/sunsynk/conftest.py
 tests/sunsynk/test_helpers.py
 tests/sunsynk/test_pysunsynk.py
 tests/sunsynk/test_register.py
 tests/sunsynk/test_rwsensors.py
```

### Comparing `sunsynk-0.3.3/tests/conftest.py` & `sunsynk-0.3.4/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `sunsynk-0.3.3/tests/hass-addon-sunsynk-dev.zip` & `sunsynk-0.3.4/tests/hass-addon-sunsynk-dev.zip`

 * *Files identical despite different names*

### Comparing `sunsynk-0.3.3/tests/hass-addon-sunsynk.zip` & `sunsynk-0.3.4/tests/hass-addon-sunsynk.zip`

 * *Files identical despite different names*

### Comparing `sunsynk-0.3.3/tests/hass_addon_sunsynk_multi/test_filter.py` & `sunsynk-0.3.4/tests/hass_addon_sunsynk_multi/test_filter.py`

 * *Files identical despite different names*

### Comparing `sunsynk-0.3.3/tests/hass_addon_sunsynk_multi/test_run.py` & `sunsynk-0.3.4/tests/hass_addon_sunsynk_multi/test_run.py`

 * *Files 25% similar despite different names*

```diff
@@ -16,16 +16,15 @@
 def run() -> ModuleType:
     """Import the module."""
     return import_module("run", MOD_FOLDER)
 
 
 def test_run(run):
     """Test Run."""
-    assert not run.STATES
-    assert not run.OPT.mqtt_host
+    assert not run.STATE
 
 
 def test_versions(run):
     """Test versions.
 
     config.json - contains the HASS addon version
     Dockerfile  - installs the specific sunsynk library from pypi
```

### Comparing `sunsynk-0.3.3/tests/sunsynk/test_helpers.py` & `sunsynk-0.3.4/tests/sunsynk/test_helpers.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,9 +1,16 @@
 """Test helpers."""
-from sunsynk.helpers import SSTime, ensure_tuple, int_round, patch_bitmask, signed
+from sunsynk.helpers import (
+    SSTime,
+    ensure_tuple,
+    int_round,
+    patch_bitmask,
+    signed,
+    simple_eval,
+)
 from sunsynk.sensors import Sensor
 
 
 def test_int_round() -> None:
     res1 = int_round(1.0)
     assert isinstance(res1, int)
     assert res1 == 1
@@ -67,7 +74,25 @@
 def test_patch_bitmask() -> None:
     assert patch_bitmask(2, 1, 1) == 3
     assert patch_bitmask(1, 2, 2) == 3
 
     assert patch_bitmask(0xFFF, 0, 1) == 0xFFE
     assert patch_bitmask(0xFFFF, 0, 1) == 0xFFFE
     assert patch_bitmask(0xFFF, 0, 2) == 0xFFD
+
+
+def test_math() -> None:
+    for expr, res in (
+        ("2^4", 6),
+        ("2**4", 16),
+        ("1 + 2*3**(4^5) / (6 + -7)", -5.0),
+        ("7 + 9 * (2 << 2)", 79),
+        ("6 // 2 + 0.0", 3.0),
+        ("2+3", 5),
+        ("6+4/2*2", 10.0),
+        ("3+2.45/8", 3.30625),
+        ("3**3*3/3+3", 30.0),
+        ("abs(-1)", 1),
+        ("pow(2,0)", 1),
+    ):
+        result = simple_eval(expr)
+        assert result == res
```

### Comparing `sunsynk-0.3.3/tests/sunsynk/test_pysunsynk.py` & `sunsynk-0.3.4/tests/sunsynk/test_pysunsynk.py`

 * *Files 1% similar despite different names*

```diff
@@ -109,17 +109,17 @@
     wrr.function_code = 0x100
     res = await ss.write_register(address=1, value=1)
     assert res is False
 
 
 @pytest.mark.asyncio
 @patch("sunsynk.pysunsynk.AsyncModbusSerialClient", async_connected=PropertyMock)
-async def test_ss_serial(ser: MagicMock, state: InverterState):
+async def test_ss_serial(serialc: MagicMock, state: InverterState):
     ss = pySunsynk(port="/dev/tty0")
     ss.state = state
 
-    ser.side_effect = TypeError
+    serialc.side_effect = TypeError
     with pytest.raises(TypeError):
         await ss.connect()
 
-    ser.side_effect = None
+    serialc.side_effect = None
     await ss.connect()
```

### Comparing `sunsynk-0.3.3/tests/sunsynk/test_register.py` & `sunsynk-0.3.4/tests/sunsynk/test_register.py`

 * *Files identical despite different names*

### Comparing `sunsynk-0.3.3/tests/sunsynk/test_rwsensors.py` & `sunsynk-0.3.4/tests/sunsynk/test_rwsensors.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,14 +5,15 @@
 
 from sunsynk.rwsensors import (
     NumberRWSensor,
     RWSensor,
     SelectRWSensor,
     Sensor,
     SwitchRWSensor,
+    SystemTimeRWSensor,
     TimeRWSensor,
 )
 
 _LOGGER = logging.getLogger(__name__)
 
 
 def test_bitmask(caplog, state) -> None:
@@ -120,14 +121,24 @@
     assert s.available_values() == ["one", "two"]
 
     assert s.value_to_reg("five", state.get) == (2,)
     assert caplog.records[-1].message == "Unknown five"
     assert caplog.records[-1].levelname == "WARNING"
 
 
+def test_systemtime_rw(state) -> None:
+    s = SystemTimeRWSensor((1, 2, 3), "Time")
+    state.track(s)
+
+    tim = "2023-03-01 12:34:56"
+    res = s.value_to_reg(tim, state.get)
+    assert res == (5891, 268, 8760)
+    assert s.reg_to_value(res) == tim
+
+
 def test_time_rw(state) -> None:
     s = TimeRWSensor(60, "two", factor=0.1)
     state.track(s)
 
     state.update(
         {
             60: 300,
```

### Comparing `sunsynk-0.3.3/tests/sunsynk/test_sensors.py` & `sunsynk-0.3.4/tests/sunsynk/test_sensors.py`

 * *Files identical despite different names*

### Comparing `sunsynk-0.3.3/tests/sunsynk/test_sunsynk.py` & `sunsynk-0.3.4/tests/sunsynk/test_sunsynk.py`

 * *Files identical despite different names*

### Comparing `sunsynk-0.3.3/tests/sunsynk/test_usunsynk.py` & `sunsynk-0.3.4/tests/sunsynk/test_usunsynk.py`

 * *Files identical despite different names*

