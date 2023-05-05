# Comparing `tmp/HATasmota-0.6.4.tar.gz` & `tmp/HATasmota-0.6.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "HATasmota-0.6.4.tar", last modified: Tue Feb 21 20:07:35 2023, max compression
+gzip compressed data, was "HATasmota-0.6.5.tar", last modified: Fri May  5 09:17:26 2023, max compression
```

## Comparing `HATasmota-0.6.4.tar` & `HATasmota-0.6.5.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 20:07:35.369687 HATasmota-0.6.4/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 20:07:35.365687 HATasmota-0.6.4/HATasmota.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      634 2023-02-21 20:07:35.000000 HATasmota-0.6.4/HATasmota.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      644 2023-02-21 20:07:35.000000 HATasmota-0.6.4/HATasmota.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-21 20:07:35.000000 HATasmota-0.6.4/HATasmota.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-21 20:07:35.000000 HATasmota-0.6.4/HATasmota.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-02-21 20:07:35.000000 HATasmota-0.6.4/HATasmota.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-02-21 20:07:35.000000 HATasmota-0.6.4/HATasmota.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-02-21 20:07:18.000000 HATasmota-0.6.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-02-21 20:07:18.000000 HATasmota-0.6.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      634 2023-02-21 20:07:35.369687 HATasmota-0.6.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-02-21 20:07:18.000000 HATasmota-0.6.4/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-21 20:07:35.369687 HATasmota-0.6.4/hatasmota/
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-02-21 20:07:18.000000 HATasmota-0.6.4/hatasmota/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5590 2023-02-21 20:07:18.000000 HATasmota-0.6.4/hatasmota/button.py
--rw-r--r--   0 runner    (1001) docker     (123)     1100 2023-02-21 20:07:18.000000 HATasmota-0.6.4/hatasmota/config_validation.py
--rw-r--r--   0 runner    (1001) docker     (123)     8755 2023-02-21 20:07:18.000000 HATasmota-0.6.4/hatasmota/const.py
--rw-r--r--   0 runner    (1001) docker     (123)     5934 2023-02-21 20:07:18.000000 HATasmota-0.6.4/hatasmota/device_status.py
--rw-r--r--   0 runner    (1001) docker     (123)    19768 2023-02-21 20:07:18.000000 HATasmota-0.6.4/hatasmota/discovery.py
--rw-r--r--   0 runner    (1001) docker     (123)     3934 2023-02-21 20:07:18.000000 HATasmota-0.6.4/hatasmota/entity.py
--rw-r--r--   0 runner    (1001) docker     (123)     3624 2023-02-21 20:07:18.000000 HATasmota-0.6.4/hatasmota/fan.py
--rw-r--r--   0 runner    (1001) docker     (123)    17261 2023-02-21 20:07:18.000000 HATasmota-0.6.4/hatasmota/light.py
--rw-r--r--   0 runner    (1001) docker     (123)      753 2023-02-21 20:07:18.000000 HATasmota-0.6.4/hatasmota/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     3469 2023-02-21 20:07:18.000000 HATasmota-0.6.4/hatasmota/mqtt.py
--rw-r--r--   0 runner    (1001) docker     (123)     4003 2023-02-21 20:07:18.000000 HATasmota-0.6.4/hatasmota/relay.py
--rw-r--r--   0 runner    (1001) docker     (123)    17528 2023-02-21 20:07:18.000000 HATasmota-0.6.4/hatasmota/sensor.py
--rw-r--r--   0 runner    (1001) docker     (123)     8189 2023-02-21 20:07:18.000000 HATasmota-0.6.4/hatasmota/shutter.py
--rw-r--r--   0 runner    (1001) docker     (123)    10019 2023-02-21 20:07:18.000000 HATasmota-0.6.4/hatasmota/status_sensor.py
--rw-r--r--   0 runner    (1001) docker     (123)    13813 2023-02-21 20:07:18.000000 HATasmota-0.6.4/hatasmota/switch.py
--rw-r--r--   0 runner    (1001) docker     (123)     2615 2023-02-21 20:07:18.000000 HATasmota-0.6.4/hatasmota/trigger.py
--rw-r--r--   0 runner    (1001) docker     (123)     7063 2023-02-21 20:07:18.000000 HATasmota-0.6.4/hatasmota/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-02-21 20:07:18.000000 HATasmota-0.6.4/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      129 2023-02-21 20:07:35.369687 HATasmota-0.6.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      956 2023-02-21 20:07:18.000000 HATasmota-0.6.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 09:17:26.971653 HATasmota-0.6.5/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 09:17:26.963653 HATasmota-0.6.5/HATasmota.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      634 2023-05-05 09:17:26.000000 HATasmota-0.6.5/HATasmota.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      644 2023-05-05 09:17:26.000000 HATasmota-0.6.5/HATasmota.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 09:17:26.000000 HATasmota-0.6.5/HATasmota.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 09:17:26.000000 HATasmota-0.6.5/HATasmota.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-05-05 09:17:26.000000 HATasmota-0.6.5/HATasmota.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-05 09:17:26.000000 HATasmota-0.6.5/HATasmota.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1072 2023-05-05 09:17:15.000000 HATasmota-0.6.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-05-05 09:17:15.000000 HATasmota-0.6.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      634 2023-05-05 09:17:26.971653 HATasmota-0.6.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-05-05 09:17:15.000000 HATasmota-0.6.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 09:17:26.971653 HATasmota-0.6.5/hatasmota/
+-rw-r--r--   0 runner    (1001) docker     (123)       17 2023-05-05 09:17:15.000000 HATasmota-0.6.5/hatasmota/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5590 2023-05-05 09:17:15.000000 HATasmota-0.6.5/hatasmota/button.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1100 2023-05-05 09:17:15.000000 HATasmota-0.6.5/hatasmota/config_validation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8755 2023-05-05 09:17:15.000000 HATasmota-0.6.5/hatasmota/const.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5932 2023-05-05 09:17:15.000000 HATasmota-0.6.5/hatasmota/device_status.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19752 2023-05-05 09:17:15.000000 HATasmota-0.6.5/hatasmota/discovery.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3934 2023-05-05 09:17:15.000000 HATasmota-0.6.5/hatasmota/entity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3624 2023-05-05 09:17:15.000000 HATasmota-0.6.5/hatasmota/fan.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17260 2023-05-05 09:17:15.000000 HATasmota-0.6.5/hatasmota/light.py
+-rw-r--r--   0 runner    (1001) docker     (123)      753 2023-05-05 09:17:15.000000 HATasmota-0.6.5/hatasmota/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3469 2023-05-05 09:17:15.000000 HATasmota-0.6.5/hatasmota/mqtt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4003 2023-05-05 09:17:15.000000 HATasmota-0.6.5/hatasmota/relay.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17521 2023-05-05 09:17:15.000000 HATasmota-0.6.5/hatasmota/sensor.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8189 2023-05-05 09:17:15.000000 HATasmota-0.6.5/hatasmota/shutter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10017 2023-05-05 09:17:15.000000 HATasmota-0.6.5/hatasmota/status_sensor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13813 2023-05-05 09:17:15.000000 HATasmota-0.6.5/hatasmota/switch.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2615 2023-05-05 09:17:15.000000 HATasmota-0.6.5/hatasmota/trigger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7063 2023-05-05 09:17:15.000000 HATasmota-0.6.5/hatasmota/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-05-05 09:17:15.000000 HATasmota-0.6.5/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      129 2023-05-05 09:17:26.971653 HATasmota-0.6.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      956 2023-05-05 09:17:15.000000 HATasmota-0.6.5/setup.py
```

### Comparing `HATasmota-0.6.4/HATasmota.egg-info/PKG-INFO` & `HATasmota-0.6.5/HATasmota.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: HATasmota
-Version: 0.6.4
+Version: 0.6.5
 Summary: Python module to help parse and construct Tasmota MQTT messages.
 Home-page: https://github.com/emontnemery/hatasmota
 Author: 
 Author-email: 
 License: MIT
 Platform: any
 Classifier: Intended Audience :: Developers
```

### Comparing `HATasmota-0.6.4/HATasmota.egg-info/SOURCES.txt` & `HATasmota-0.6.5/HATasmota.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `HATasmota-0.6.4/LICENSE` & `HATasmota-0.6.5/LICENSE`

 * *Files identical despite different names*

### Comparing `HATasmota-0.6.4/PKG-INFO` & `HATasmota-0.6.5/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: HATasmota
-Version: 0.6.4
+Version: 0.6.5
 Summary: Python module to help parse and construct Tasmota MQTT messages.
 Home-page: https://github.com/emontnemery/hatasmota
 Author: 
 Author-email: 
 License: MIT
 Platform: any
 Classifier: Intended Audience :: Developers
```

### Comparing `HATasmota-0.6.4/hatasmota/button.py` & `HATasmota-0.6.5/hatasmota/button.py`

 * *Files identical despite different names*

### Comparing `HATasmota-0.6.4/hatasmota/config_validation.py` & `HATasmota-0.6.5/hatasmota/config_validation.py`

 * *Files identical despite different names*

### Comparing `HATasmota-0.6.4/hatasmota/const.py` & `HATasmota-0.6.5/hatasmota/const.py`

 * *Files identical despite different names*

### Comparing `HATasmota-0.6.4/hatasmota/device_status.py` & `HATasmota-0.6.5/hatasmota/device_status.py`

 * *Files 1% similar despite different names*

```diff
@@ -121,15 +121,15 @@
         def state_message_received(msg: ReceiveMessage) -> None:
             """Handle new MQTT state messages."""
             if not self._on_state_callback:
                 return
 
             try:
                 payload = json.loads(msg.payload)
-            except (json.decoder.JSONDecodeError):
+            except json.decoder.JSONDecodeError:
                 return
 
             attributes = {}
             for attribute in ATTRIBUTES:
                 state = None
                 if msg.topic == self._cfg.state_topic and attribute in STATE_PATHS:
                     state = get_value_by_path(payload, STATE_PATHS[attribute])
```

### Comparing `HATasmota-0.6.4/hatasmota/discovery.py` & `HATasmota-0.6.5/hatasmota/discovery.py`

 * *Files 2% similar despite different names*

```diff
@@ -312,15 +312,15 @@
 
 
 def get_binary_sensor_entities(
     discovery_msg: dict,
 ) -> list[tuple[TasmotaSwitchConfig | None, DiscoveryHashType]]:
     """Generate binary sensor configuration."""
     entities: list[tuple[TasmotaSwitchConfig | None, DiscoveryHashType]] = []
-    for (idx, value) in enumerate(discovery_msg[CONF_SWITCH]):
+    for idx, value in enumerate(discovery_msg[CONF_SWITCH]):
         entity = None
         discovery_hash = (discovery_msg[CONF_MAC], "binary_sensor", "switch", idx)
         if value:
             entity = TasmotaSwitchConfig.from_discovery_message(
                 discovery_msg, idx, "binary_sensor"
             )
         entities.append((entity, discovery_hash))
@@ -333,15 +333,15 @@
 ) -> list[tuple[TasmotaShutterConfig | None, DiscoveryHashType]]:
     """Generate cover configuration."""
     relays = discovery_msg[CONF_RELAY]
     shutter_entities: list[tuple[TasmotaShutterConfig | None, DiscoveryHashType]] = []
     shutter_indices = []
 
     # Tasmota supports up to 4 shutters, each shutter is assigned two consecutive relays
-    for (idx, value) in enumerate(chain(relays, [-1])):
+    for idx, value in enumerate(chain(relays, [-1])):
         if idx - 1 in shutter_indices:
             # This is the 2nd half of a pair, skip
             continue
 
         if value == RL_SHUTTER:
             if relays[idx + 1] == RL_SHUTTER:
                 shutter_indices.append(idx)
@@ -355,15 +355,15 @@
                 )
                 shutter_indices = []
                 break
 
     # pad / truncate the shutter index list to 4
     shutter_indices = shutter_indices[:4] + [-1] * (4 - len(shutter_indices))
 
-    for (idx, relay_idx) in enumerate(shutter_indices):
+    for idx, relay_idx in enumerate(shutter_indices):
         entity = None
         discovery_hash = (discovery_msg[CONF_MAC], "cover", "shutter", idx)
         if relay_idx != -1:
             entity = TasmotaShutterConfig.from_discovery_message(
                 discovery_msg, idx, "cover"
             )
         shutter_entities.append((entity, discovery_hash))
@@ -388,15 +388,15 @@
 
 def get_switch_entities(
     discovery_msg: dict,
 ) -> list[tuple[TasmotaRelayConfig | None, DiscoveryHashType]]:
     """Generate switch configuration."""
     force_light = discovery_msg[CONF_OPTIONS][OPTION_HASS_LIGHT] == 1
     switch_entities: list[tuple[TasmotaRelayConfig | None, DiscoveryHashType]] = []
-    for (idx, value) in enumerate(discovery_msg[CONF_RELAY]):
+    for idx, value in enumerate(discovery_msg[CONF_RELAY]):
         entity = None
         discovery_hash = (discovery_msg[CONF_MAC], "switch", "relay", idx)
         if value == RL_RELAY and not force_light:
             entity = TasmotaRelayConfig.from_discovery_message(
                 discovery_msg, idx, "switch"
             )
         switch_entities.append((entity, discovery_hash))
@@ -415,23 +415,23 @@
     ] = []
     relays = list(discovery_msg[CONF_RELAY])
 
     if discovery_msg[CONF_IFAN] and relays[0] == RL_LIGHT:
         # Special case for iFan: Single, non dimmable light
         relays[0] = RL_RELAY
 
-    for (idx, value) in enumerate(relays):
+    for idx, value in enumerate(relays):
         entity = None
         discovery_hash = (discovery_msg[CONF_MAC], "light", "light", idx)
         if value == RL_LIGHT:
             entity = TasmotaLightConfig.from_discovery_message(
                 discovery_msg, idx, "light"
             )
         light_entities.append((entity, discovery_hash))
-    for (idx, value) in enumerate(relays):
+    for idx, value in enumerate(relays):
         entity = None
         discovery_hash = (discovery_msg[CONF_MAC], "light", "relay", idx)
         if value == RL_RELAY:
             if force_light or (discovery_msg[CONF_IFAN] and idx == 0):
                 entity = TasmotaRelayConfig.from_discovery_message(
                     discovery_msg, idx, "light"
                 )
@@ -510,25 +510,25 @@
         return TasmotaRelay(config=config, mqtt_client=mqtt_client)
     return None
 
 
 def get_button_triggers(discovery_msg: dict) -> list[TasmotaButtonTriggerConfig]:
     """Generate binary sensor configuration."""
     triggers = []
-    for (idx, _) in enumerate(discovery_msg[CONF_BUTTON]):
+    for idx, _ in enumerate(discovery_msg[CONF_BUTTON]):
         trigger = TasmotaButtonTriggerConfig.from_discovery_message(discovery_msg, idx)
         triggers.extend(trigger)
 
     return triggers
 
 
 def get_switch_triggers(discovery_msg: dict) -> list[TasmotaSwitchTriggerConfig]:
     """Generate binary sensor configuration."""
     triggers = []
-    for (idx, _) in enumerate(discovery_msg[CONF_SWITCH]):
+    for idx, _ in enumerate(discovery_msg[CONF_SWITCH]):
         trigger = TasmotaSwitchTriggerConfig.from_discovery_message(discovery_msg, idx)
         triggers.extend(trigger)
 
     return triggers
 
 
 def get_triggers(discovery_msg: dict) -> list[TasmotaTriggerConfig]:
```

### Comparing `HATasmota-0.6.4/hatasmota/entity.py` & `HATasmota-0.6.5/hatasmota/entity.py`

 * *Files identical despite different names*

### Comparing `HATasmota-0.6.4/hatasmota/fan.py` & `HATasmota-0.6.5/hatasmota/fan.py`

 * *Files identical despite different names*

### Comparing `HATasmota-0.6.4/hatasmota/light.py` & `HATasmota-0.6.5/hatasmota/light.py`

 * *Files 0% similar despite different names*

```diff
@@ -198,15 +198,14 @@
                 return
 
             attributes = {}
             idx = self._cfg.idx
 
             if self._cfg.endpoint == "light":
                 if self._cfg.light_type != LIGHT_TYPE_NONE:
-
                     brightness = get_value_by_path(
                         msg.payload, [self._cfg.dimmer_state]
                     )
                     if brightness is not None:
                         self._brightness = brightness
                         attributes["brightness"] = brightness
```

### Comparing `HATasmota-0.6.4/hatasmota/models.py` & `HATasmota-0.6.5/hatasmota/models.py`

 * *Files identical despite different names*

### Comparing `HATasmota-0.6.4/hatasmota/mqtt.py` & `HATasmota-0.6.5/hatasmota/mqtt.py`

 * *Files identical despite different names*

### Comparing `HATasmota-0.6.4/hatasmota/relay.py` & `HATasmota-0.6.5/hatasmota/relay.py`

 * *Files identical despite different names*

### Comparing `HATasmota-0.6.4/hatasmota/sensor.py` & `HATasmota-0.6.5/hatasmota/sensor.py`

 * *Files 0% similar despite different names*

```diff
@@ -243,15 +243,15 @@
         platform: str,
         sensor_name: str,
         value_path: list[str | int],
         parent_path: list[str | int],
         quantity: str,
     ) -> TasmotaSensorConfig:
         """Instantiate from discovery message."""
-        unit = SENSOR_UNIT_MAP.get(quantity, " ")
+        unit = SENSOR_UNIT_MAP.get(quantity)
         if quantity in SENSOR_DYNAMIC_UNIT_MAP:
             key, supported_units = SENSOR_DYNAMIC_UNIT_MAP[quantity]
             unit = sensor_config[CONF_SENSOR].get(key)
             if unit not in supported_units:
                 _LOGGER.warning("Unknown unit %s for %s", unit, quantity)
 
         if last_reset_key := LAST_RESET_SENSOR_MAP.get(quantity):
@@ -454,15 +454,15 @@
                             subsubsensorpath,
                             subsubsensorpath,
                             quantity,
                         )
                     )
             elif isinstance(subsensor, list):
                 # Array sensor
-                for (idx, _) in enumerate(subsensor):
+                for idx, _ in enumerate(subsensor):
                     subsubsensorpath = list(subsensorpath)
                     subsubsensorpath.append(idx)
                     sensor_configs.append(
                         _get_sensor_entity(
                             sensor_discovery_message,
                             device_discovery_msg,
                             subsubsensorpath,
```

### Comparing `HATasmota-0.6.4/hatasmota/shutter.py` & `HATasmota-0.6.5/hatasmota/shutter.py`

 * *Files identical despite different names*

### Comparing `HATasmota-0.6.4/hatasmota/status_sensor.py` & `HATasmota-0.6.5/hatasmota/status_sensor.py`

 * *Files 1% similar despite different names*

```diff
@@ -210,15 +210,15 @@
         def state_message_received(msg: ReceiveMessage) -> None:
             """Handle new MQTT state messages."""
             if not self._on_state_callback:
                 return
 
             try:
                 payload = json.loads(msg.payload)
-            except (json.decoder.JSONDecodeError):
+            except json.decoder.JSONDecodeError:
                 return
 
             state = None
             if msg.topic == self._cfg.state_topic:
                 state = get_value_by_path(payload, STATE_PATHS[self._cfg.sensor])
             else:
                 state = get_value_by_path(payload, STATUS_PATHS[self._cfg.sensor])
```

### Comparing `HATasmota-0.6.4/hatasmota/switch.py` & `HATasmota-0.6.5/hatasmota/switch.py`

 * *Files identical despite different names*

### Comparing `HATasmota-0.6.4/hatasmota/trigger.py` & `HATasmota-0.6.5/hatasmota/trigger.py`

 * *Files identical despite different names*

### Comparing `HATasmota-0.6.4/hatasmota/utils.py` & `HATasmota-0.6.5/hatasmota/utils.py`

 * *Files identical despite different names*

### Comparing `HATasmota-0.6.4/setup.py` & `HATasmota-0.6.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from setuptools import setup, find_packages
 
 
 long_description = open("README.md").read()
 
 setup(
     name="HATasmota",
-    version="0.6.4",
+    version="0.6.5",
     license="MIT",
     url="https://github.com/emontnemery/hatasmota",
     author="",
     author_email="",
     description="Python module to help parse and construct Tasmota MQTT messages.",
     long_description=long_description,
     long_description_content_type="text/markdown",
```

