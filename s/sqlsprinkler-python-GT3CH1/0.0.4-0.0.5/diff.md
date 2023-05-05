# Comparing `tmp/sqlsprinkler-python-GT3CH1-0.0.4.tar.gz` & `tmp/sqlsprinkler-python-GT3CH1-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sqlsprinkler-python-GT3CH1-0.0.4.tar", last modified: Thu May  4 17:51:16 2023, max compression
+gzip compressed data, was "sqlsprinkler-python-GT3CH1-0.0.5.tar", last modified: Fri May  5 14:55:47 2023, max compression
```

## Comparing `sqlsprinkler-python-GT3CH1-0.0.4.tar` & `sqlsprinkler-python-GT3CH1-0.0.5.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 gcpease  (1709703766) 1389146880        0 2023-05-04 17:51:16.889926 sqlsprinkler-python-GT3CH1-0.0.4/
--rw-r--r--   0 gcpease  (1709703766) 1389146880     1068 2023-05-04 14:34:10.000000 sqlsprinkler-python-GT3CH1-0.0.4/LICENSE
--rw-r--r--   0 gcpease  (1709703766) 1389146880      830 2023-05-04 17:51:16.890118 sqlsprinkler-python-GT3CH1-0.0.4/PKG-INFO
--rw-r--r--   0 gcpease  (1709703766) 1389146880      324 2023-05-04 14:34:10.000000 sqlsprinkler-python-GT3CH1-0.0.4/README.md
--rw-r--r--   0 gcpease  (1709703766) 1389146880       84 2023-05-04 14:34:10.000000 sqlsprinkler-python-GT3CH1-0.0.4/pyproject.toml
--rw-r--r--   0 gcpease  (1709703766) 1389146880      641 2023-05-04 17:51:16.892518 sqlsprinkler-python-GT3CH1-0.0.4/setup.cfg
--rw-r--r--   0 gcpease  (1709703766) 1389146880       68 2023-05-04 14:34:10.000000 sqlsprinkler-python-GT3CH1-0.0.4/setup.py
-drwxr-xr-x   0 gcpease  (1709703766) 1389146880        0 2023-05-04 17:51:16.863976 sqlsprinkler-python-GT3CH1-0.0.4/src/
-drwxr-xr-x   0 gcpease  (1709703766) 1389146880        0 2023-05-04 17:51:16.880386 sqlsprinkler-python-GT3CH1-0.0.4/src/sqlsprinkler/
--rw-r--r--   0 gcpease  (1709703766) 1389146880      107 2023-05-04 15:09:35.000000 sqlsprinkler-python-GT3CH1-0.0.4/src/sqlsprinkler/__init__.py
--rw-r--r--   0 gcpease  (1709703766) 1389146880      222 2023-05-04 15:09:35.000000 sqlsprinkler-python-GT3CH1-0.0.4/src/sqlsprinkler/api.py
--rw-r--r--   0 gcpease  (1709703766) 1389146880     5505 2023-05-04 17:50:50.000000 sqlsprinkler-python-GT3CH1-0.0.4/src/sqlsprinkler/system.py
--rw-r--r--   0 gcpease  (1709703766) 1389146880     3087 2023-05-04 17:50:50.000000 sqlsprinkler-python-GT3CH1-0.0.4/src/sqlsprinkler/zone.py
-drwxr-xr-x   0 gcpease  (1709703766) 1389146880        0 2023-05-04 17:51:16.889250 sqlsprinkler-python-GT3CH1-0.0.4/src/sqlsprinkler_python_GT3CH1.egg-info/
--rw-r--r--   0 gcpease  (1709703766) 1389146880      830 2023-05-04 17:51:16.000000 sqlsprinkler-python-GT3CH1-0.0.4/src/sqlsprinkler_python_GT3CH1.egg-info/PKG-INFO
--rw-r--r--   0 gcpease  (1709703766) 1389146880      372 2023-05-04 17:51:16.000000 sqlsprinkler-python-GT3CH1-0.0.4/src/sqlsprinkler_python_GT3CH1.egg-info/SOURCES.txt
--rw-r--r--   0 gcpease  (1709703766) 1389146880        1 2023-05-04 17:51:16.000000 sqlsprinkler-python-GT3CH1-0.0.4/src/sqlsprinkler_python_GT3CH1.egg-info/dependency_links.txt
--rw-r--r--   0 gcpease  (1709703766) 1389146880       13 2023-05-04 17:51:16.000000 sqlsprinkler-python-GT3CH1-0.0.4/src/sqlsprinkler_python_GT3CH1.egg-info/top_level.txt
+drwxrwxrwx   0 gcpease   (1000) gcpease   (1000)        0 2023-05-05 14:55:47.230463 sqlsprinkler-python-GT3CH1-0.0.5/
+-rwxrwxrwx   0 gcpease   (1000) gcpease   (1000)     1089 2022-05-11 15:38:12.000000 sqlsprinkler-python-GT3CH1-0.0.5/LICENSE
+-rwxrwxrwx   0 gcpease   (1000) gcpease   (1000)      830 2023-05-05 14:55:47.230463 sqlsprinkler-python-GT3CH1-0.0.5/PKG-INFO
+-rwxrwxrwx   0 gcpease   (1000) gcpease   (1000)      333 2022-05-11 15:45:59.000000 sqlsprinkler-python-GT3CH1-0.0.5/README.md
+-rwxrwxrwx   0 gcpease   (1000) gcpease   (1000)       86 2022-05-11 15:42:03.000000 sqlsprinkler-python-GT3CH1-0.0.5/pyproject.toml
+-rwxrwxrwx   0 gcpease   (1000) gcpease   (1000)      641 2023-05-05 14:55:47.236377 sqlsprinkler-python-GT3CH1-0.0.5/setup.cfg
+-rwxrwxrwx   0 gcpease   (1000) gcpease   (1000)       71 2022-05-11 15:42:21.000000 sqlsprinkler-python-GT3CH1-0.0.5/setup.py
+drwxrwxrwx   0 gcpease   (1000) gcpease   (1000)        0 2023-05-05 14:55:47.012514 sqlsprinkler-python-GT3CH1-0.0.5/src/
+drwxrwxrwx   0 gcpease   (1000) gcpease   (1000)        0 2023-05-05 14:55:47.137064 sqlsprinkler-python-GT3CH1-0.0.5/src/sqlsprinkler/
+-rwxrwxrwx   0 gcpease   (1000) gcpease   (1000)      110 2023-05-02 15:23:00.000000 sqlsprinkler-python-GT3CH1-0.0.5/src/sqlsprinkler/__init__.py
+-rwxrwxrwx   0 gcpease   (1000) gcpease   (1000)      231 2023-05-04 14:31:15.000000 sqlsprinkler-python-GT3CH1-0.0.5/src/sqlsprinkler/api.py
+-rwxrwxrwx   0 gcpease   (1000) gcpease   (1000)     5759 2023-05-05 14:47:15.000000 sqlsprinkler-python-GT3CH1-0.0.5/src/sqlsprinkler/system.py
+-rwxrwxrwx   0 gcpease   (1000) gcpease   (1000)     3415 2023-05-05 14:47:15.000000 sqlsprinkler-python-GT3CH1-0.0.5/src/sqlsprinkler/zone.py
+drwxrwxrwx   0 gcpease   (1000) gcpease   (1000)        0 2023-05-05 14:55:47.211916 sqlsprinkler-python-GT3CH1-0.0.5/src/sqlsprinkler_python_GT3CH1.egg-info/
+-rwxrwxrwx   0 gcpease   (1000) gcpease   (1000)      830 2023-05-05 14:55:46.000000 sqlsprinkler-python-GT3CH1-0.0.5/src/sqlsprinkler_python_GT3CH1.egg-info/PKG-INFO
+-rwxrwxrwx   0 gcpease   (1000) gcpease   (1000)      372 2023-05-05 14:55:46.000000 sqlsprinkler-python-GT3CH1-0.0.5/src/sqlsprinkler_python_GT3CH1.egg-info/SOURCES.txt
+-rwxrwxrwx   0 gcpease   (1000) gcpease   (1000)        1 2023-05-05 14:55:46.000000 sqlsprinkler-python-GT3CH1-0.0.5/src/sqlsprinkler_python_GT3CH1.egg-info/dependency_links.txt
+-rwxrwxrwx   0 gcpease   (1000) gcpease   (1000)       13 2023-05-05 14:55:46.000000 sqlsprinkler-python-GT3CH1-0.0.5/src/sqlsprinkler_python_GT3CH1.egg-info/top_level.txt
```

### Comparing `sqlsprinkler-python-GT3CH1-0.0.4/LICENSE` & `sqlsprinkler-python-GT3CH1-0.0.5/LICENSE`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-MIT License
-
-Copyright (c) 2022 Gavin Pease
-
-Permission is hereby granted, free of charge, to any person obtaining a copy
-of this software and associated documentation files (the "Software"), to deal
-in the Software without restriction, including without limitation the rights
-to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-copies of the Software, and to permit persons to whom the Software is
-furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all
-copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-SOFTWARE.
+MIT License
+
+Copyright (c) 2022 Gavin Pease
+
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+SOFTWARE.
```

### Comparing `sqlsprinkler-python-GT3CH1-0.0.4/PKG-INFO` & `sqlsprinkler-python-GT3CH1-0.0.5/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sqlsprinkler-python-GT3CH1
-Version: 0.0.4
+Version: 0.0.5
 Summary: A python library to control a SQLSprinkler system
 Home-page: https://github.com/GT3CH1/sqlsprinkler_python
 Author: Gavin Pease
 Author-email: gavinpease@gmail.com
 Project-URL: Bug Tracker, https://github.com/GT3CH1/sqlsprinkler_python/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `sqlsprinkler-python-GT3CH1-0.0.4/setup.cfg` & `sqlsprinkler-python-GT3CH1-0.0.5/setup.cfg`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = sqlsprinkler-python-GT3CH1
-version = 0.0.4
+version = 0.0.5
 author = Gavin Pease
 author_email = gavinpease@gmail.com
 description = A python library to control a SQLSprinkler system
 long_description = file: README.md
 long_description_content_type = text/markdown
 url = https://github.com/GT3CH1/sqlsprinkler_python
 project_urls =
```

### Comparing `sqlsprinkler-python-GT3CH1-0.0.4/src/sqlsprinkler/system.py` & `sqlsprinkler-python-GT3CH1-0.0.5/src/sqlsprinkler/system.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,173 +1,175 @@
-from dataclasses import dataclass, field, asdict
-
-import requests
-from . import API, Zone
-
-
-class System:
-    """ This class represents a SQL Sprinkler system. """
-    zones = []
-    system_state = False
-    hostname = ""
-
-    def __init__(self, hostname: str) -> None:
-        self.hostname = hostname
-        self.zones = self.get_zones()
-        self.system_state = self.get_system_state()
-
-    def __post_init__(self) -> None:
-        """
-        Gets the zones from the hostname.
-        :return: None
-        """
-        print("Host {}".format(self.hostname))
-        self.zones = self.get_zones()
-        self.system_state = self.get_system_state()
-
-    def _fetch_zones(self) -> [Zone]:
-        """
-        Fetches the zones from the hostname.
-        :return: A list of zones.
-        """
-        url = "{}/{}".format(self.hostname, API.ZONE_INFO_URL)
-        print(url)
-        request = requests.get(url)
-        print(request)
-        zone_list = []
-        for zone in request.json():
-            new_zone = Zone()
-            new_zone.host = self.hostname
-            new_zone.name = zone['name']
-            new_zone.gpio = zone['gpio']
-            new_zone.time = zone['time']
-            new_zone.enabled = zone['enabled']
-            new_zone.auto_off = zone['auto_off']
-            new_zone.system_order = zone['system_order']
-            new_zone.state = zone['state']
-            new_zone.id = zone['id']
-            zone_list.append(new_zone)
-        return zone_list
-
-    def get_zones(self) -> [Zone]:
-        """
-        Returns the zones in the system.
-        :return: A list of zones.
-        """
-        self.zones = self._fetch_zones()
-        return self.zones
-
-    def get_system_state(self) -> bool:
-        """
-        Returns the system state.
-        :return: The system state.
-        """
-        self._update_system_state()
-        return self.state
-
-    def update(self):
-        """
-        Updates the system.
-        :return: None
-        """
-        self.zones = self._fetch_zones()
-        self._update_system_state()
-
-    def turn_on(self):
-        self.set_system_state(True)
-
-    def turn_off(self):
-        self.set_system_state(False)
-
-    def set_system_state(self, state: bool) -> None:
-        """
-        Sets the system state.
-        :param state: The state to set.
-        :return: None
-        """
-        url = "{}/{}".format(self.hostname, API.SYSTEM_STATE_URL)
-        request = requests.put(url, json={"system_enabled": state})
-        if request.status_code != 200:
-            raise Exception(f"Failed to set system state {state}")
-        self._update_system_state()
-
-    def _update_system_state(self) -> None:
-        """
-        Fetches the system state from the hostname.
-        """
-        url = "{}/{}".format(self.hostname, API.SYSTEM_STATE_URL)
-        print(url)
-        request = requests.get(url).json()
-        self.state = request["system_enabled"]
-
-    def update_zone_state(self, zone_id: int, state: bool) -> None:
-        """
-        Updates the state of a zone.
-        :param zone_id: The zone ID to update.
-        :param state: The state of the zone, True for on, False for off.
-        :return: None
-        """
-        # Get the zone where the ID matches the one we want to update
-        zone = self.get_zone_by_id(zone_id)
-        if zone is None:
-            raise Exception(f"Zone {zone_id} not found")
-        if state:
-            zone.turn_on()
-        else:
-            zone.turn_off()
-        self._fetch_zones()
-
-    def get_zone_by_id(self, zone_id: int) -> Zone:
-        """ Gets a zone by id."""
-        zone = next(filter(lambda zone: zone.id == zone_id, self.zones), None)
-        return zone
-
-    def add_zone(self, zone: Zone) -> None:
-        """
-        Adds a zone to the system.
-        :param zone: The zone to add.
-        :return: None
-        """
-        zone_to_add = {
-            "Name": zone.name,
-            "GPIO": zone.gpio,
-            "Time": zone.time,
-            "Enabled": zone.enabled,
-            "Autooff": zone.auto_off,
-        }
-        request = requests.post(f"{self.hostname}/{API.ZONE_URL}", json=zone_to_add)
-        if request.status_code != 200:
-            raise Exception(f"Failed to add zone {zone}")
-        self.zones = self.get_zones()
-
-    def delete_zone(self, zone_id: int) -> None:
-        """
-        Deletes a zone from the system.
-        :param zone_id: The zone ID to delete.
-        :return: None
-        """
-        request = requests.delete(f"{self.hostname}/{API.ZONE_URL}", json={"id": zone_id})
-        if request.status_code != 200:
-            raise Exception(f"Failed to delete zone {zone_id}")
-
-    def update_zone(self, zone: Zone) -> None:
-        """
-        Updates a zone in the system.
-        :param zone: The zone to update.
-        :return: None
-        """
-        zone_to_update = self.get_zone_by_id(zone.id)
-        if zone_to_update is None:
-            raise Exception(f"Zone {zone.id} not found")
-        zone.update(zone_to_update)
-        self.zones = self.get_zones()
-
-    def update_zone_order(self, zone_order: [int]) -> None:
-        """
-        Updates the order of the zones.
-        :param: zone_order: The new order of the zones.
-        :return: None
-        """
-        request = requests.put(f"{self.hostname}/{API.ZONE_ORDER_URL}", json={"order": zone_order})
-        if request.status_code != 200:
-            raise Exception(f"Failed to update zone order {zone_order}")
-        self.zones = self.get_zones()
+from dataclasses import dataclass, field, asdict
+
+from typing import List
+
+import requests
+from sqlsprinkler import API, Zone
+
+class System:
+    """ This class represents a SQL Sprinkler system. """
+    zones = []
+    system_state = False
+    hostname = ""
+
+    def __init__(self, hostname: str) -> None:
+        self.hostname = hostname
+        self.zones = self.get_zones()
+        self.system_state = self.get_system_state()
+
+    def __post_init__(self) -> None:
+        """
+        Gets the zones from the hostname.
+        :return: None
+        """
+        print("Host {}".format(self.hostname))
+        self.zones = self.get_zones()
+        self.system_state = self.get_system_state()
+
+    def _fetch_zones(self) -> List[Zone]:
+        """
+        Fetches the zones from the hostname.
+        :return: A list of zones.
+        """
+        url = "{}/{}".format(self.hostname,API.ZONE_INFO_URL)
+        print(url)
+        request = requests.get(url)
+        print(request)
+        zone_list = []
+        for zone in request.json():
+            new_zone = Zone()
+            new_zone.host = self.hostname
+            new_zone.name = zone['name']
+            new_zone.gpio = zone['gpio']
+            new_zone.time = zone['time']
+            new_zone.enabled = zone['enabled']
+            new_zone.auto_off = zone['auto_off']
+            new_zone.system_order = zone['system_order']
+            new_zone.state = zone['state']
+            new_zone.id = zone['id']
+            zone_list.append(new_zone)
+        return zone_list
+
+    def get_zones(self) -> List[Zone]:
+        """
+        Returns the zones in the system.
+        :return: A list of zones.
+        """
+        self.zones = self._fetch_zones()
+        return self.zones
+
+    def get_system_state(self) -> bool:
+        """
+        Returns the system state.
+        :return: The system state.
+        """
+        self._update_system_state()
+        return self.state
+
+    def update(self):
+        """
+        Updates the system.
+        :return: None
+        """
+        self.zones = self._fetch_zones()
+        self._update_system_state()
+
+    def turn_on(self):
+        self.set_system_state(True)
+
+    def turn_off(self):
+        self.set_system_state(False)
+
+    def set_system_state(self, state: bool) -> None:
+        """
+        Sets the system state.
+        :param state: The state to set.
+        :return: None
+        """
+        url = "{}/{}".format(self.hostname,API.SYSTEM_STATE_URL)
+        request = requests.put(url, json={"system_enabled": state})
+        if request.status_code != 200:
+            raise Exception(f"Failed to set system state {state}")
+        self._update_system_state()
+
+    def _update_system_state(self) -> None:
+        """
+        Fetches the system state from the hostname.
+        """
+        url = "{}/{}".format(self.hostname,API.SYSTEM_STATE_URL)
+        print(url)
+        request = requests.get(url).json()
+        self.state = request["system_enabled"]
+
+    def update_zone_state(self, zone_id: int, state: bool) -> None:
+        """
+        Updates the state of a zone.
+        :param zone_id: The zone ID to update.
+        :param state: The state of the zone, True for on, False for off.
+        :return: None
+        """
+        # Get the zone where the ID matches the one we want to update
+        zone = self.get_zone_by_id(zone_id)
+        if zone is None:
+            raise Exception(f"Zone {zone_id} not found")
+        if state:
+            zone.turn_on()
+        else:
+            zone.turn_off()
+        self._fetch_zones()
+
+    def get_zone_by_id(self, zone_id: int) -> Zone:
+        """ Gets a zone by id."""
+        zone = next(filter(lambda zone: zone.id == zone_id, self.zones), None)
+        return zone
+
+    def add_zone(self, zone: Zone) -> None:
+        """
+        Adds a zone to the system.
+        :param zone: The zone to add.
+        :return: None
+        """
+        zone_to_add = {
+                "Name": zone.name,
+                "GPIO": zone.gpio,
+                "Time": zone.time,
+                "Enabled": zone.enabled,
+                "Autooff": zone.auto_off,
+                }
+        request = requests.post(f"{self.hostname}/{API.ZONE_URL}", json=zone_to_add)
+        if request.status_code != 200:
+            raise Exception(f"Failed to add zone {zone}")
+        self.zones = self.get_zones()
+
+    def delete_zone(self, zone_id: int) -> None:
+        """
+        Deletes a zone from the system.
+        :param zone_id: The zone ID to delete.
+        :return: None
+        """
+        request = requests.delete(f"{self.hostname}/{API.ZONE_URL}", json={"id": zone_id})
+        if request.status_code != 200:
+            raise Exception(f"Failed to delete zone {zone_id}")
+
+    def update_zone(self, zone: Zone) -> None:
+        """
+        Updates a zone in the system.
+        :param zone: The zone to update.
+        :return: None
+        """
+        zone_to_update = self.get_zone_by_id(zone.id)
+        if zone_to_update is None:
+            raise Exception(f"Zone {zone.id} not found")
+        zone.update_other(zone_to_update)
+        self.zones = self.get_zones()
+
+    def update_zone_order(self, zone_order: List[int]) -> None:
+        """
+        Updates the order of the zones.
+        :param: zone_order: The new order of the zones.
+        :return: None
+        """
+        request = requests.put(f"{self.hostname}/{API.ZONE_ORDER_URL}", json={"order": zone_order})
+        if request.status_code != 200:
+            raise Exception(f"Failed to update zone order {zone_order}")
+        self.zones = self.get_zones()
+
```

### Comparing `sqlsprinkler-python-GT3CH1-0.0.4/src/sqlsprinkler/zone.py` & `sqlsprinkler-python-GT3CH1-0.0.5/src/sqlsprinkler/zone.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,103 +1,104 @@
-from dataclasses import field, dataclass
-
-import requests
-from . import API
-
-
-@dataclass
-class Zone:
-    """ This class represents a SQL Sprinkler zone. """
-    host = "none"
-    name: str = field(default_factory=str)
-    gpio: int = field(default_factory=int)
-    time: int = field(default_factory=int)
-    enabled: bool = field(default_factory=bool)
-    auto_off: bool = field(default_factory=bool)
-    system_order: int = field(default_factory=int)
-    state: bool = field(default_factory=bool)
-    id: int = field(default_factory=int)
-
-    def turn_on(self) -> None:
-        """
-        Turns the zone on.
-        :return: None
-        """
-        self.state = True
-        # send request to API_ZONE_URL with ID and state
-        url = "{}{}"
-        requests.put(f"{self.host}/{API.ZONE_URL}", json={"id": self.id, "state": self.state})
-
-    def turn_off(self) -> None:
-        """
-        Turns the zone off.
-        :return: None
-        """
-        self.state = False
-        # send request to API_ZONE_URL with ID and state
-        requests.put(f"{self.host}/{API.ZONE_URL}", json={"id": self.id, "state": self.state})
-
-    def enable(self):
-        self.enabled = True
-        self.update(self)
-
-    def disable(self):
-        self.enabled = False
-        self.update(self)
-
-    def set_time(self, time: int) -> None:
-        self.time = time
-        self.update(self)
-
-    def set_gpio(self, gpio: int) -> None:
-        self.gpio = gpio
-        self.update(self)
-
-    def set_name(self, name: str) -> None:
-        self.name = name
-        self.update(self)
-
-    def set_auto_off(self, auto_off: bool) -> None:
-        self.auto_off = auto_off
-        self.update(self)
-
-    def set_system_order(self, system_order: int) -> None:
-        self.system_order = system_order
-        self.update(self)
-
-    def update_other(self, other) -> None:
-        """
-        Updates the state of the zone.
-        :param other: The zone to update with.
-        :return: None
-        """
-        self.name = other.name
-        self.gpio = other.gpio
-        self.time = other.time
-        self.enabled = other.enabled
-        self.auto_off = other.auto_off
-        self.system_order = other.system_order
-
-        # send request to API_ZONE_UPDATE_URL with name, gpio, time, enabled, auto_off, system_order
-        zone_json = {
-            "id": self.id,
-            "name": self.name,
-            "gpio": self.gpio,
-            "time": self.time,
-            "enabled": self.enabled,
-            "auto_off": self.auto_off,
-            "system_order": self.system_order
-        }
-        requests.put(f"{self.host}/{API.ZONE_UPDATE_URL}", json=zone_json)
-
-    def update(self) -> None:
-        url = "{}/{}/{}".format(self.host, API.ZONE_INFO_URL, self.id)
-        print(url)
-        req = requests.get(url).json()
-        print(req)
-        self.name = req['name']
-        self.gpio = req['gpio']
-        self.time = req['time']
-        self.enabled = req['enabled']
-        self.auto_off = req['auto_off']
-        self.system_order = req['system_order']
-        self.state = req['state']
+from dataclasses import field, dataclass
+
+import requests
+from sqlsprinkler import API
+@dataclass
+class Zone:
+    """ This class represents a SQL Sprinkler zone. """
+    host = "none"
+    name: str = field(default_factory=str)
+    gpio: int = field(default_factory=int)
+    time: int = field(default_factory=int)
+    enabled: bool = field(default_factory=bool)
+    auto_off: bool = field(default_factory=bool)
+    system_order: int = field(default_factory=int)
+    state: bool = field(default_factory=bool)
+    id: int = field(default_factory=int)
+
+    def turn_on(self) -> None:
+        """
+        Turns the zone on.
+        :return: None
+        """
+        self.state = True
+        # send request to API_ZONE_URL with ID and state
+        url = "{}{}"
+        requests.put(f"{self.host}/{API.ZONE_URL}", json={"id": self.id, "state": self.state})
+
+    def turn_off(self) -> None:
+        """
+        Turns the zone off.
+        :return: None
+        """
+        self.state = False
+        # send request to API_ZONE_URL with ID and state
+        requests.put(f"{self.host}/{API.ZONE_URL}", json={"id": self.id, "state": self.state})
+
+    def update(self) -> None:
+        """
+        Updates the state of the zone.
+        :return: None
+        """
+        # send request to API_ZONE_INFO_URL with ID
+        url = "{}/{}/{}".format(self.host, API.ZONE_INFO_URL, self.id)
+        request = requests.get(url)
+        self.name = request.json()['name']
+        self.gpio = request.json()['gpio']
+        self.time = request.json()['time']
+        self.enabled = request.json()['enabled']
+        self.auto_off = request.json()['auto_off']
+        self.system_order = request.json()['system_order']
+        self.state = request.json()['state']
+
+    def enable(self):
+        self.enabled = True
+        self.update_other(self)
+
+    def disable(self):
+        self.enabled = False
+        self.update_other(self)
+
+    def set_time(self, time: int) -> None:
+        self.time = time
+        self.update_other(self)
+
+    def set_gpio(self, gpio: int) -> None:
+        self.gpio = gpio
+        self.update_other(self)
+
+    def set_name(self, name: str) -> None:
+        self.name = name
+        self.update_other(self)
+
+    def set_auto_off(self, auto_off: bool) -> None:
+        self.auto_off = auto_off
+        self.update_other(self)
+
+    def set_system_order(self, system_order: int) -> None:
+        self.system_order = system_order
+        self.update_other(self)
+
+    def update_other(self, other) -> None:
+        """
+        Updates the state of the zone.
+        :param other: The zone to update with.
+        :return: None
+        """
+        self.name = other.name
+        self.gpio = other.gpio
+        self.time = other.time
+        self.enabled = other.enabled
+        self.auto_off = other.auto_off
+        self.system_order = other.system_order
+
+        # send request to API_ZONE_UPDATE_URL with name, gpio, time, enabled, auto_off, system_order
+        zone_json = {
+            "id": self.id,
+            "name": self.name,
+            "gpio": self.gpio,
+            "time": self.time,
+            "enabled": self.enabled,
+            "auto_off": self.auto_off,
+            "system_order": self.system_order
+        }
+        requests.put(f"{self.host}/{API.ZONE_UPDATE_URL}", json=zone_json)
```

### Comparing `sqlsprinkler-python-GT3CH1-0.0.4/src/sqlsprinkler_python_GT3CH1.egg-info/PKG-INFO` & `sqlsprinkler-python-GT3CH1-0.0.5/src/sqlsprinkler_python_GT3CH1.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sqlsprinkler-python-GT3CH1
-Version: 0.0.4
+Version: 0.0.5
 Summary: A python library to control a SQLSprinkler system
 Home-page: https://github.com/GT3CH1/sqlsprinkler_python
 Author: Gavin Pease
 Author-email: gavinpease@gmail.com
 Project-URL: Bug Tracker, https://github.com/GT3CH1/sqlsprinkler_python/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

