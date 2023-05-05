# Comparing `tmp/boschshcpy-0.2.8.dev5.tar.gz` & `tmp/boschshcpy-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/boschshcpy-0.2.8.dev5.tar", last modified: Sun Feb 28 12:08:44 2021, max compression
+gzip compressed data, was "dist/boschshcpy-0.2.9.tar", last modified: Sun Mar  7 20:06:49 2021, max compression
```

## Comparing `boschshcpy-0.2.8.dev5.tar` & `boschshcpy-0.2.9.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 schamm     (501) staff       (20)        0 2021-02-28 12:08:44.460712 boschshcpy-0.2.8.dev5/
--rw-r--r--   0 schamm     (501) staff       (20)       35 2021-02-28 12:07:35.000000 boschshcpy-0.2.8.dev5/MANIFEST.in
--rw-r--r--   0 schamm     (501) staff       (20)     3771 2021-02-28 12:08:44.460310 boschshcpy-0.2.8.dev5/PKG-INFO
--rw-r--r--   0 schamm     (501) staff       (20)     2491 2021-01-10 11:03:10.000000 boschshcpy-0.2.8.dev5/README.md
-drwxr-xr-x   0 schamm     (501) staff       (20)        0 2021-02-28 12:08:44.456734 boschshcpy-0.2.8.dev5/boschshcpy/
--rw-r--r--   0 schamm     (501) staff       (20)      649 2021-02-28 00:55:09.000000 boschshcpy-0.2.8.dev5/boschshcpy/__init__.py
--rw-r--r--   0 schamm     (501) staff       (20)     7481 2021-02-28 00:55:09.000000 boschshcpy-0.2.8.dev5/boschshcpy/api.py
--rw-r--r--   0 schamm     (501) staff       (20)     4493 2021-02-27 22:44:02.000000 boschshcpy-0.2.8.dev5/boschshcpy/device.py
--rw-r--r--   0 schamm     (501) staff       (20)     4586 2021-02-28 00:55:09.000000 boschshcpy-0.2.8.dev5/boschshcpy/device_helper.py
--rw-r--r--   0 schamm     (501) staff       (20)     2036 2021-02-27 22:44:02.000000 boschshcpy-0.2.8.dev5/boschshcpy/device_service.py
--rw-r--r--   0 schamm     (501) staff       (20)     5064 2021-02-27 22:44:02.000000 boschshcpy-0.2.8.dev5/boschshcpy/domain_impl.py
--rw-r--r--   0 schamm     (501) staff       (20)      951 2021-02-28 00:55:09.000000 boschshcpy-0.2.8.dev5/boschshcpy/exceptions.py
--rw-r--r--   0 schamm     (501) staff       (20)     1402 2021-02-28 00:55:09.000000 boschshcpy-0.2.8.dev5/boschshcpy/generate_cert.py
--rw-r--r--   0 schamm     (501) staff       (20)     5432 2021-02-28 00:53:30.000000 boschshcpy-0.2.8.dev5/boschshcpy/information.py
--rw-r--r--   0 schamm     (501) staff       (20)    22635 2021-02-28 00:55:09.000000 boschshcpy-0.2.8.dev5/boschshcpy/models_impl.py
--rw-r--r--   0 schamm     (501) staff       (20)     4029 2021-02-28 00:55:09.000000 boschshcpy-0.2.8.dev5/boschshcpy/register_client.py
--rw-r--r--   0 schamm     (501) staff       (20)      475 2021-02-27 22:44:02.000000 boschshcpy-0.2.8.dev5/boschshcpy/room.py
--rw-r--r--   0 schamm     (501) staff       (20)      689 2021-02-27 22:44:02.000000 boschshcpy-0.2.8.dev5/boschshcpy/scenario.py
--rw-r--r--   0 schamm     (501) staff       (20)    19177 2021-02-27 22:48:32.000000 boschshcpy-0.2.8.dev5/boschshcpy/services_impl.py
--rw-r--r--   0 schamm     (501) staff       (20)    10158 2021-02-28 00:55:09.000000 boschshcpy-0.2.8.dev5/boschshcpy/session.py
--rw-r--r--   0 schamm     (501) staff       (20)     3924 2021-02-28 00:55:09.000000 boschshcpy-0.2.8.dev5/boschshcpy/tls_ca_chain.pem
-drwxr-xr-x   0 schamm     (501) staff       (20)        0 2021-02-28 12:08:44.459506 boschshcpy-0.2.8.dev5/boschshcpy.egg-info/
--rw-r--r--   0 schamm     (501) staff       (20)     3771 2021-02-28 12:08:44.000000 boschshcpy-0.2.8.dev5/boschshcpy.egg-info/PKG-INFO
--rw-r--r--   0 schamm     (501) staff       (20)      599 2021-02-28 12:08:44.000000 boschshcpy-0.2.8.dev5/boschshcpy.egg-info/SOURCES.txt
--rw-r--r--   0 schamm     (501) staff       (20)        1 2021-02-28 12:08:44.000000 boschshcpy-0.2.8.dev5/boschshcpy.egg-info/dependency_links.txt
--rw-r--r--   0 schamm     (501) staff       (20)       46 2021-02-28 12:08:44.000000 boschshcpy-0.2.8.dev5/boschshcpy.egg-info/requires.txt
--rw-r--r--   0 schamm     (501) staff       (20)       11 2021-02-28 12:08:44.000000 boschshcpy-0.2.8.dev5/boschshcpy.egg-info/top_level.txt
--rw-r--r--   0 schamm     (501) staff       (20)       38 2021-02-28 12:08:44.460914 boschshcpy-0.2.8.dev5/setup.cfg
--rw-r--r--   0 schamm     (501) staff       (20)      899 2021-02-28 12:08:16.000000 boschshcpy-0.2.8.dev5/setup.py
+drwxr-xr-x   0 schamm     (501) staff       (20)        0 2021-03-07 20:06:49.599314 boschshcpy-0.2.9/
+-rw-r--r--   0 schamm     (501) staff       (20)       35 2021-02-28 12:07:35.000000 boschshcpy-0.2.9/MANIFEST.in
+-rw-r--r--   0 schamm     (501) staff       (20)     3799 2021-03-07 20:06:49.598774 boschshcpy-0.2.9/PKG-INFO
+-rw-r--r--   0 schamm     (501) staff       (20)     2516 2021-03-07 20:02:09.000000 boschshcpy-0.2.9/README.md
+drwxr-xr-x   0 schamm     (501) staff       (20)        0 2021-03-07 20:06:49.594227 boschshcpy-0.2.9/boschshcpy/
+-rw-r--r--   0 schamm     (501) staff       (20)      674 2021-03-07 20:05:12.000000 boschshcpy-0.2.9/boschshcpy/__init__.py
+-rw-r--r--   0 schamm     (501) staff       (20)     7481 2021-03-07 20:05:20.000000 boschshcpy-0.2.9/boschshcpy/api.py
+-rw-r--r--   0 schamm     (501) staff       (20)     4493 2021-03-07 20:02:35.000000 boschshcpy-0.2.9/boschshcpy/device.py
+-rw-r--r--   0 schamm     (501) staff       (20)     4843 2021-03-07 20:05:29.000000 boschshcpy-0.2.9/boschshcpy/device_helper.py
+-rw-r--r--   0 schamm     (501) staff       (20)     2036 2021-03-07 20:02:35.000000 boschshcpy-0.2.9/boschshcpy/device_service.py
+-rw-r--r--   0 schamm     (501) staff       (20)     5064 2021-03-07 20:02:35.000000 boschshcpy-0.2.9/boschshcpy/domain_impl.py
+-rw-r--r--   0 schamm     (501) staff       (20)      951 2021-03-07 20:05:35.000000 boschshcpy-0.2.9/boschshcpy/exceptions.py
+-rw-r--r--   0 schamm     (501) staff       (20)     1402 2021-03-01 19:59:37.000000 boschshcpy-0.2.9/boschshcpy/generate_cert.py
+-rw-r--r--   0 schamm     (501) staff       (20)     5432 2021-03-07 20:02:35.000000 boschshcpy-0.2.9/boschshcpy/information.py
+-rw-r--r--   0 schamm     (501) staff       (20)    24256 2021-03-07 20:05:52.000000 boschshcpy-0.2.9/boschshcpy/models_impl.py
+-rw-r--r--   0 schamm     (501) staff       (20)     4029 2021-03-07 20:05:58.000000 boschshcpy-0.2.9/boschshcpy/register_client.py
+-rw-r--r--   0 schamm     (501) staff       (20)      475 2021-03-07 20:02:35.000000 boschshcpy-0.2.9/boschshcpy/room.py
+-rw-r--r--   0 schamm     (501) staff       (20)      689 2021-03-07 20:02:35.000000 boschshcpy-0.2.9/boschshcpy/scenario.py
+-rw-r--r--   0 schamm     (501) staff       (20)    19177 2021-03-07 20:02:35.000000 boschshcpy-0.2.9/boschshcpy/services_impl.py
+-rw-r--r--   0 schamm     (501) staff       (20)    10158 2021-03-07 20:06:09.000000 boschshcpy-0.2.9/boschshcpy/session.py
+-rw-r--r--   0 schamm     (501) staff       (20)     3924 2021-03-01 19:59:37.000000 boschshcpy-0.2.9/boschshcpy/tls_ca_chain.pem
+drwxr-xr-x   0 schamm     (501) staff       (20)        0 2021-03-07 20:06:49.597790 boschshcpy-0.2.9/boschshcpy.egg-info/
+-rw-r--r--   0 schamm     (501) staff       (20)     3799 2021-03-07 20:06:49.000000 boschshcpy-0.2.9/boschshcpy.egg-info/PKG-INFO
+-rw-r--r--   0 schamm     (501) staff       (20)      599 2021-03-07 20:06:49.000000 boschshcpy-0.2.9/boschshcpy.egg-info/SOURCES.txt
+-rw-r--r--   0 schamm     (501) staff       (20)        1 2021-03-07 20:06:49.000000 boschshcpy-0.2.9/boschshcpy.egg-info/dependency_links.txt
+-rw-r--r--   0 schamm     (501) staff       (20)       46 2021-03-07 20:06:49.000000 boschshcpy-0.2.9/boschshcpy.egg-info/requires.txt
+-rw-r--r--   0 schamm     (501) staff       (20)       11 2021-03-07 20:06:49.000000 boschshcpy-0.2.9/boschshcpy.egg-info/top_level.txt
+-rw-r--r--   0 schamm     (501) staff       (20)       38 2021-03-07 20:06:49.599506 boschshcpy-0.2.9/setup.cfg
+-rw-r--r--   0 schamm     (501) staff       (20)      894 2021-03-07 20:06:30.000000 boschshcpy-0.2.9/setup.py
```

### Comparing `boschshcpy-0.2.8.dev5/PKG-INFO` & `boschshcpy-0.2.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: boschshcpy
-Version: 0.2.8.dev5
+Version: 0.2.9
 Summary: Bosch Smart Home Controller API Python Library
 Home-page: https://github.com/tschamm/boschshcpy
 Author: Clemens-Alexander Brust, Thomas Schamm
 Author-email: cabrust@pm.me, thomas@tschamm.de
 License: bsd-3-clause
 Description: # Bosch Smart Home Controller API Python Library
         
@@ -39,14 +39,15 @@
         * ```WaterLeakageSensorTilt```
         
         The following device models are implemented, using the above services:
         
         * ```ShutterContact```
         * ```ShutterControl```
         * ```SmartPlug```
+        * ```SmartPlugCompact```
         * ```LightControl```
         * ```SmokeDetector```
         * ```CameraEyes```
         * ```IntrusionDetectionSystem```
         * ```RoomClimateControl```
         * ```Thermostat```
         * ```WallThermostat```
```

### Comparing `boschshcpy-0.2.8.dev5/README.md` & `boschshcpy-0.2.9/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -31,14 +31,15 @@
 * ```WaterLeakageSensorTilt```
 
 The following device models are implemented, using the above services:
 
 * ```ShutterContact```
 * ```ShutterControl```
 * ```SmartPlug```
+* ```SmartPlugCompact```
 * ```LightControl```
 * ```SmokeDetector```
 * ```CameraEyes```
 * ```IntrusionDetectionSystem```
 * ```RoomClimateControl```
 * ```Thermostat```
 * ```WallThermostat```
```

### Comparing `boschshcpy-0.2.8.dev5/boschshcpy/__init__.py` & `boschshcpy-0.2.9/boschshcpy/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -6,14 +6,15 @@
     SHCClimateControl,
     SHCDeviceHelper,
     SHCLight,
     SHCMotionDetector,
     SHCShutterContact,
     SHCShutterControl,
     SHCSmartPlug,
+    SHCSmartPlugCompact,
     SHCSmokeDetector,
     SHCThermostat,
     SHCTwinguard,
     SHCUniversalSwitch,
     SHCWallThermostat,
 )
 from .domain_impl import SHCIntrusionSystem
```

### Comparing `boschshcpy-0.2.8.dev5/boschshcpy/api.py` & `boschshcpy-0.2.9/boschshcpy/api.py`

 * *Files identical despite different names*

### Comparing `boschshcpy-0.2.8.dev5/boschshcpy/device.py` & `boschshcpy-0.2.9/boschshcpy/device.py`

 * *Files identical despite different names*

### Comparing `boschshcpy-0.2.8.dev5/boschshcpy/device_helper.py` & `boschshcpy-0.2.9/boschshcpy/device_helper.py`

 * *Files 11% similar despite different names*

```diff
@@ -9,14 +9,15 @@
     SHCCameraEyes,
     SHCClimateControl,
     SHCLight,
     SHCMotionDetector,
     SHCShutterContact,
     SHCShutterControl,
     SHCSmartPlug,
+    SHCSmartPlugCompact,
     SHCSmokeDetector,
     SHCThermostat,
     SHCTwinguard,
     SHCUniversalSwitch,
     SHCWallThermostat,
     SHCWaterLeakageSensor,
     build,
@@ -62,14 +63,20 @@
         if "PSM" in SUPPORTED_MODELS:
             devices.extend(self._devices_by_model["PSM"].values())
         if "BSM" in SUPPORTED_MODELS:
             devices.extend(self._devices_by_model["BSM"].values())
         return devices
 
     @property
+    def smart_plugs_compact(self) -> typing.Sequence[SHCSmartPlugCompact]:
+        if "PLUG_COMPACT" not in SUPPORTED_MODELS:
+            return []
+        return list(self._devices_by_model['PLUG_COMPACT'].values())
+
+    @property
     def smoke_detectors(self) -> typing.Sequence[SHCSmokeDetector]:
         if "SD" not in SUPPORTED_MODELS:
             return []
         return list(self._devices_by_model["SD"].values())
 
     @property
     def climate_controls(self) -> typing.Sequence[SHCClimateControl]:
```

### Comparing `boschshcpy-0.2.8.dev5/boschshcpy/device_service.py` & `boschshcpy-0.2.9/boschshcpy/device_service.py`

 * *Files identical despite different names*

### Comparing `boschshcpy-0.2.8.dev5/boschshcpy/domain_impl.py` & `boschshcpy-0.2.9/boschshcpy/domain_impl.py`

 * *Files identical despite different names*

### Comparing `boschshcpy-0.2.8.dev5/boschshcpy/exceptions.py` & `boschshcpy-0.2.9/boschshcpy/exceptions.py`

 * *Files identical despite different names*

### Comparing `boschshcpy-0.2.8.dev5/boschshcpy/generate_cert.py` & `boschshcpy-0.2.9/boschshcpy/generate_cert.py`

 * *Files identical despite different names*

### Comparing `boschshcpy-0.2.8.dev5/boschshcpy/information.py` & `boschshcpy-0.2.9/boschshcpy/information.py`

 * *Files identical despite different names*

### Comparing `boschshcpy-0.2.8.dev5/boschshcpy/models_impl.py` & `boschshcpy-0.2.9/boschshcpy/models_impl.py`

 * *Files 2% similar despite different names*

```diff
@@ -113,14 +113,63 @@
         self._powermeter_service.short_poll()
 
     def summary(self):
         print(f"PSM/BSM SmartPlug:")
         super().summary()
 
 
+class SHCSmartPlugCompact(SHCDevice):
+    from .services_impl import (
+        PowerMeterService,
+        PowerSwitchProgramService,
+        PowerSwitchService,
+        CommunicationQualityService
+    )
+
+    def __init__(self, api, raw_device):
+        super().__init__(api, raw_device)
+
+        self._powerswitch_service = self.device_service("PowerSwitch")
+        self._powerswitchprogram_service = self.device_service("PowerSwitchProgram")
+        self._powermeter_service = self.device_service("PowerMeter")
+        self._communicationquality_service = self.device_service("CommunicationQuality")
+
+    @property
+    def state(self) -> PowerSwitchService.State:
+        return self._powerswitch_service.value
+
+    @state.setter
+    def state(self, state: bool):
+        self._powerswitch_service.put_state_element(
+            "switchState", "ON" if state else "OFF"
+        )
+
+    @property
+    def energyconsumption(self) -> float:
+        return self._powermeter_service.energyconsumption
+
+    @property
+    def powerconsumption(self) -> float:
+        return self._powermeter_service.powerconsumption
+
+    @property
+    def communicationquality(self) -> CommunicationQualityService.State:
+        return self._communicationquality_service.value
+
+    def update(self):
+        self._powerswitch_service.short_poll()
+        self._powerswitchprogram_service.short_poll()
+        self._powermeter_service.short_poll()
+        self._communicationquality_service.short_poll()
+
+    def summary(self):
+        print(f"PLUG_COMPACT SmartPlugCompact:")
+        super().summary()
+
+
 class SHCShutterControl(SHCDevice):
     from .services_impl import ShutterControlService
 
     def __init__(self, api, raw_device):
         super().__init__(api, raw_device=raw_device)
         self._service = self.device_service("ShutterControl")
 
@@ -699,14 +748,15 @@
 
 
 MODEL_MAPPING = {
     "SWD": SHCShutterContact,
     "BBL": SHCShutterControl,
     "PSM": SHCSmartPlug,
     "BSM": SHCSmartPlug,  # uses same impl as PSM
+    "PLUG_COMPACT": SHCSmartPlugCompact,
     "SD": SHCSmokeDetector,
     "CAMERA_EYES": SHCCameraEyes,
     "CAMERA_360": SHCCamera360,
     "ROOM_CLIMATE_CONTROL": SHCClimateControl,
     "TRV": SHCThermostat,
     "THB": SHCWallThermostat,
     "BWTH": SHCWallThermostat,  # uses same impl as THB
```

### Comparing `boschshcpy-0.2.8.dev5/boschshcpy/register_client.py` & `boschshcpy-0.2.9/boschshcpy/register_client.py`

 * *Files identical despite different names*

### Comparing `boschshcpy-0.2.8.dev5/boschshcpy/scenario.py` & `boschshcpy-0.2.9/boschshcpy/scenario.py`

 * *Files identical despite different names*

### Comparing `boschshcpy-0.2.8.dev5/boschshcpy/services_impl.py` & `boschshcpy-0.2.9/boschshcpy/services_impl.py`

 * *Files identical despite different names*

### Comparing `boschshcpy-0.2.8.dev5/boschshcpy/session.py` & `boschshcpy-0.2.9/boschshcpy/session.py`

 * *Files identical despite different names*

### Comparing `boschshcpy-0.2.8.dev5/boschshcpy/tls_ca_chain.pem` & `boschshcpy-0.2.9/boschshcpy/tls_ca_chain.pem`

 * *Files identical despite different names*

### Comparing `boschshcpy-0.2.8.dev5/boschshcpy.egg-info/PKG-INFO` & `boschshcpy-0.2.9/boschshcpy.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: boschshcpy
-Version: 0.2.8.dev5
+Version: 0.2.9
 Summary: Bosch Smart Home Controller API Python Library
 Home-page: https://github.com/tschamm/boschshcpy
 Author: Clemens-Alexander Brust, Thomas Schamm
 Author-email: cabrust@pm.me, thomas@tschamm.de
 License: bsd-3-clause
 Description: # Bosch Smart Home Controller API Python Library
         
@@ -39,14 +39,15 @@
         * ```WaterLeakageSensorTilt```
         
         The following device models are implemented, using the above services:
         
         * ```ShutterContact```
         * ```ShutterControl```
         * ```SmartPlug```
+        * ```SmartPlugCompact```
         * ```LightControl```
         * ```SmokeDetector```
         * ```CameraEyes```
         * ```IntrusionDetectionSystem```
         * ```RoomClimateControl```
         * ```Thermostat```
         * ```WallThermostat```
```

### Comparing `boschshcpy-0.2.8.dev5/boschshcpy.egg-info/SOURCES.txt` & `boschshcpy-0.2.9/boschshcpy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `boschshcpy-0.2.8.dev5/setup.py` & `boschshcpy-0.2.9/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import find_packages, setup
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setup(
     name="boschshcpy",
-    version="0.2.8.dev5",
+    version="0.2.9",
     url="https://github.com/tschamm/boschshcpy",
     author="Clemens-Alexander Brust, Thomas Schamm",
     author_email="cabrust@pm.me, thomas@tschamm.de",
     description="Bosch Smart Home Controller API Python Library",
     license='bsd-3-clause',
     long_description=long_description,
     long_description_content_type="text/markdown",
```

