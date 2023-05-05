# Comparing `tmp/pyytlounge-1.4.3.tar.gz` & `tmp/pyytlounge-1.5.0.tar.gz`

## Comparing `pyytlounge-1.4.3.tar` & `pyytlounge-1.5.0.tar`

### file list

```diff
@@ -1,13 +1,23 @@
--rw-r--r--   0        0        0      182 2020-02-02 00:00:00.000000 pyytlounge-1.4.3/requirements.txt
--rw-r--r--   0        0        0     1719 2020-02-02 00:00:00.000000 pyytlounge-1.4.3/test.py
--rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 pyytlounge-1.4.3/variables_example.py
--rw-r--r--   0        0        0      495 2020-02-02 00:00:00.000000 pyytlounge-1.4.3/.vscode/launch.json
--rw-r--r--   0        0        0       74 2020-02-02 00:00:00.000000 pyytlounge-1.4.3/src/pyytlounge/__init__.py
--rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 pyytlounge-1.4.3/src/pyytlounge/api.py
--rwxr-xr-x   0        0        0      802 2020-02-02 00:00:00.000000 pyytlounge-1.4.3/src/pyytlounge/manual_pairing.py
--rw-r--r--   0        0        0    16678 2020-02-02 00:00:00.000000 pyytlounge-1.4.3/src/pyytlounge/wrapper.py
--rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 pyytlounge-1.4.3/.gitignore
--rw-r--r--   0        0        0    35148 2020-02-02 00:00:00.000000 pyytlounge-1.4.3/LICENSE
--rw-r--r--   0        0        0      649 2020-02-02 00:00:00.000000 pyytlounge-1.4.3/README.md
--rw-r--r--   0        0        0      556 2020-02-02 00:00:00.000000 pyytlounge-1.4.3/pyproject.toml
--rw-r--r--   0        0        0     1145 2020-02-02 00:00:00.000000 pyytlounge-1.4.3/PKG-INFO
+-rw-r--r--   0        0        0      153 2020-02-02 00:00:00.000000 pyytlounge-1.5.0/CHANGELOG.md
+-rw-r--r--   0        0        0     1432 2020-02-02 00:00:00.000000 pyytlounge-1.5.0/test.py
+-rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 pyytlounge-1.5.0/variables_example.py
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 pyytlounge-1.5.0/.pytest_cache/.gitignore
+-rw-r--r--   0        0        0      191 2020-02-02 00:00:00.000000 pyytlounge-1.5.0/.pytest_cache/CACHEDIR.TAG
+-rw-r--r--   0        0        0      302 2020-02-02 00:00:00.000000 pyytlounge-1.5.0/.pytest_cache/README.md
+-rw-r--r--   0        0        0      155 2020-02-02 00:00:00.000000 pyytlounge-1.5.0/.pytest_cache/v/cache/lastfailed
+-rw-r--r--   0        0        0      278 2020-02-02 00:00:00.000000 pyytlounge-1.5.0/.pytest_cache/v/cache/nodeids
+-rw-r--r--   0        0        0        2 2020-02-02 00:00:00.000000 pyytlounge-1.5.0/.pytest_cache/v/cache/stepwise
+-rw-r--r--   0        0        0      495 2020-02-02 00:00:00.000000 pyytlounge-1.5.0/.vscode/launch.json
+-rw-r--r--   0        0        0       74 2020-02-02 00:00:00.000000 pyytlounge-1.5.0/src/pyytlounge/__init__.py
+-rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 pyytlounge-1.5.0/src/pyytlounge/api.py
+-rwxr-xr-x   0        0        0      802 2020-02-02 00:00:00.000000 pyytlounge-1.5.0/src/pyytlounge/manual_pairing.py
+-rw-r--r--   0        0        0    16630 2020-02-02 00:00:00.000000 pyytlounge-1.5.0/src/pyytlounge/wrapper.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 pyytlounge-1.5.0/tests/__init__.py
+-rw-r--r--   0        0        0      219 2020-02-02 00:00:00.000000 pyytlounge-1.5.0/tests/conftest.py
+-rw-r--r--   0        0        0     4096 2020-02-02 00:00:00.000000 pyytlounge-1.5.0/tests/devices.py
+-rw-r--r--   0        0        0      446 2020-02-02 00:00:00.000000 pyytlounge-1.5.0/tests/test_process_event.py
+-rw-r--r--   0        0        0       48 2020-02-02 00:00:00.000000 pyytlounge-1.5.0/.gitignore
+-rw-r--r--   0        0        0    35148 2020-02-02 00:00:00.000000 pyytlounge-1.5.0/LICENSE
+-rw-r--r--   0        0        0      649 2020-02-02 00:00:00.000000 pyytlounge-1.5.0/README.md
+-rw-r--r--   0        0        0      693 2020-02-02 00:00:00.000000 pyytlounge-1.5.0/pyproject.toml
+-rw-r--r--   0        0        0     1316 2020-02-02 00:00:00.000000 pyytlounge-1.5.0/PKG-INFO
```

### Comparing `pyytlounge-1.4.3/test.py` & `pyytlounge-1.5.0/test.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,28 +1,25 @@
 import asyncio
-from src.pyytlounge.wrapper import YtLoungeApi
+from src.pyytlounge.wrapper import YtLoungeApi, PlaybackState, State
 from ast import literal_eval
 import os
 
-from src.pyytlounge.wrapper import PlaybackState
-
 AUTH_STATE_FILE = "auth_state"
 
 
 async def go():
     api = YtLoungeApi("Test")
     if os.path.exists(AUTH_STATE_FILE):
         with open(AUTH_STATE_FILE, "r") as f:
             content = f.read()
             api.load_auth_state(literal_eval(content))
-            api.auth.lounge_id_token = "AGdO5p_6vEjSUu6aPm_E_Cqem9d2g6uDsYQrOsKYPCLMjCP746xnxBeoOS8IskNwn7pAwNpPE1S-NISvBvXVw7WYrauy-vLHUM3QrCc_A-sx1P-iae7ILRI"
             print("Loaded from file")
     else:
-        pairing_code = int(input("Enter pairing code: "))
-        print("Pairing...")
+        pairing_code = input("Enter pairing code: ")
+        print(f"Pairing with code {pairing_code}...")
         paired = await api.pair(pairing_code)
         print(paired and "success" or "failed")
         if not paired:
             exit()
         auth_state = api.auth.serialize()
         with open(AUTH_STATE_FILE, "w") as f:
             f.write(str(auth_state))
@@ -30,26 +27,23 @@
     is_available = await api.is_available()
     print(f"Screen availability: {is_available}")
 
     print("Connecting...")
     connected = await api.connect()
     print(connected and "success" or "failed")
     if not connected:
-        authed = await api.refresh_auth()
-        if not authed or not await api.connect():
-            exit()
-        else:
-            print("Reauth success")
+        exit()
 
     print(f"Screen: {api.screen_name}")
     print(f"Device: {api.screen_device_name}")
 
-    print(api.auth.serialize())
-
     async def receive_state(state: PlaybackState):
         print(f"New state: {state}")
-        print(f"Image should be at: https://img.youtube.com/vi/{state.videoId}/0.jpg")
+        if state.videoId:
+            print(
+                f"Image should be at: https://img.youtube.com/vi/{state.videoId}/0.jpg"
+            )
 
     await api.subscribe(receive_state)
 
 
 asyncio.run(go())
```

### Comparing `pyytlounge-1.4.3/src/pyytlounge/manual_pairing.py` & `pyytlounge-1.5.0/src/pyytlounge/manual_pairing.py`

 * *Files identical despite different names*

### Comparing `pyytlounge-1.4.3/src/pyytlounge/wrapper.py` & `pyytlounge-1.5.0/src/pyytlounge/wrapper.py`

 * *Files 3% similar despite different names*

```diff
@@ -36,15 +36,15 @@
     duration: float
     videoId: str
     state: State
 
     def __init__(
         self, logger: logging.Logger, state: Union[NowPlayingData, None] = None
     ):
-        self.__logger = logger
+        self._logger = logger
 
         if not state or "state" not in state:
             self.currentTime = 0.0
             self.duration = 0.0
             self.videoId = ""
             self.state = State.Stopped
             return
@@ -54,15 +54,15 @@
 
     def apply_state(self, state: PlaybackStateData):
         self.currentTime = float(state["currentTime"])
         self.duration = float(state["duration"])
         try:
             self.state = State(int(state["state"]))
         except ValueError:
-            self.__logger.warning(
+            self._logger.warning(
                 "Unknown state %s %s. Assuming stopped state.", state["state"], state
             )
             self.state = State.Stopped
 
     def __eq__(self, other):
         return vars(self) == vars(other)
 
@@ -144,17 +144,17 @@
         self.auth = AuthState()
         self._sid = None
         self._gsession = None
         self._last_event_id = None
         self.state = PlaybackState(logger)
         self.state_update = 0
         self._command_offset = 1
-        self.__screen_name: str = None
-        self.__device_info: __DeviceInfo = None
-        self.__logger = logger or logging.Logger(__package__, logging.DEBUG)
+        self._screen_name: str = None
+        self._device_info: __DeviceInfo = None
+        self._logger = logger or logging.Logger(__package__, logging.DEBUG)
 
     def paired(self) -> bool:
         """Returns true if screen id and lounge id token are known."""
         return self.auth.screen_id is not None
 
     def linked(self) -> bool:
         """Returns true if paired and lounge id token is known."""
@@ -174,41 +174,41 @@
 
     @property
     def screen_name(self) -> str:
         """Returns screen name as returned by YouTube"""
         if not self.linked():
             raise Exception("Not linked")
 
-        return self.__screen_name
+        return self._screen_name
 
     @property
     def screen_device_name(self) -> str:
         """Returns device name built from device info returned by YouTube"""
         if not self.connected():
             raise Exception("Not connected")
-        brand = self.__device_info["brand"]
-        model = self.__device_info["model"]
+        brand = self._device_info["brand"]
+        model = self._device_info["model"]
         return f"{brand} {model}"
 
     async def pair(self, pairing_code) -> bool:
         """Pair with a device using a manual input pairing code"""
 
         async with aiohttp.ClientSession() as session:
             pair_url = f"{api_base}/pairing/get_screen"
             pair_data = {"pairing_code": pairing_code}
             async with session.post(url=pair_url, data=pair_data) as resp:
                 try:
                     screens = await resp.json()
                     screen = screens["screen"]
-                    self.__screen_name = screen["name"]
+                    self._screen_name = screen["name"]
                     self.auth.screen_id = screen["screenId"]
                     self.auth.lounge_id_token = screen["loungeToken"]
                     return self.linked()
                 except Exception as ex:
-                    self.__logger.exception(ex)
+                    self._logger.exception(ex)
                     return False
 
     async def refresh_auth(self) -> bool:
         """Refresh lounge token using stored refresh token."""
         if not self.paired():
             raise Exception("Must be paired")
 
@@ -218,21 +218,21 @@
             async with session.post(url=refresh_url, data=refresh_data) as resp:
                 try:
                     screens = await resp.json()
                     screen = screens["screens"][0]
                     self.auth.screen_id = screen["screenId"]
                     self.auth.lounge_id_token = screen["loungeToken"]
 
-                    self.__logger.info(
+                    self._logger.info(
                         "Refreshed auth, lounge id token %s", self.auth.lounge_id_token
                     )
 
                     return self.linked()
                 except Exception as ex:
-                    self.__logger.exception(ex)
+                    self._logger.exception(ex)
                     return False
 
     def store_auth_state(self) -> dict:
         """Return auth parameters as dict which can be serialized for later use"""
         return {
             "screenId": self.auth.screen_id,
             "lounge_id_token": self.auth.lounge_id_token,
@@ -240,62 +240,62 @@
         }
 
     def load_auth_state(self, data: dict):
         """Use deserialized auth parameters"""
         self.auth = AuthState()
         self.auth.deserialize(data)
 
-    def __update_state(self):
+    def _update_state(self):
         self.state_update = self.state_update + 1
 
-    def __connection_lost(self):
+    def _connection_lost(self):
         self._sid = None
         self._gsession = None
         self._last_event_id = None
 
-    def __process_event(self, event_id: int, event_type: str, args):
+    def _process_event(self, event_id: int, event_type: str, args):
         if event_type == "onStateChange":
             data = args[0]
             self.state.apply_state(data)
-            self.__update_state()
+            self._update_state()
         elif event_type == "nowPlaying":
             data = args[0]
-            self.state = PlaybackState(self.__logger, data)
-            self.__update_state()
+            self.state = PlaybackState(self._logger, data)
+            self._update_state()
         elif event_type == "loungeStatus":
             data: __LoungeStatus = args[0]
             devices: List[__Device] = json.loads(data["devices"])
             for device in devices:
                 if device["type"] == "LOUNGE_SCREEN":
-                    self.__screen_name = device["name"]
-                    self.__device_info = json.loads(device["deviceInfo"])
+                    self._screen_name = device["name"]
+                    self._device_info = json.loads(device["deviceInfo"])
                     break
         elif event_type == "loungeScreenDisconnected":
-            self.state = PlaybackState(self.__logger)
-            self.__update_state()
-            self.__connection_lost()
+            self.state = PlaybackState(self._logger)
+            self._update_state()
+            self._connection_lost()
         elif event_type == "noop":
             pass  # no-op
         else:
-            self.__logger.debug("Unprocessed event %s %s", event_type, args)
+            self._logger.debug("Unprocessed event %s %s", event_type, args)
 
-    def __process_events(self, events):
+    def _process_events(self, events):
         for event in events:
             event_id, (event_type, *args) = event
             if event_type == "c":
                 self._sid = args[0]
             elif event_type == "S":
                 self._gsession = args[0]
             else:
-                self.__process_event(event_id, event_type, args)
+                self._process_event(event_id, event_type, args)
 
         last_id = events[-1][0]
         self._last_event_id = last_id
 
-    async def __parse_event_chunks(self, lines: AsyncIterator[str]):
+    async def _parse_event_chunks(self, lines: AsyncIterator[str]):
         chunk_remaining = 0
         current_chunk = ""
         async for line in lines:
             if chunk_remaining <= 0:
                 chunk_remaining = int(line)
                 current_chunk = ""
             else:
@@ -360,33 +360,33 @@
                 try:
                     text = await resp.text()
                     if resp.status == 401:
                         self.auth.lounge_id_token = None
                         return False
 
                     if resp.status != 200:
-                        self.__logger.warning(
+                        self._logger.warning(
                             "Unknown reply to connect %i %s", resp.status, resp.reason
                         )
                         return False
                     lines = text.splitlines()
-                    async for events in self.__parse_event_chunks(desync(lines)):
-                        self.__process_events(events)
+                    async for events in self._parse_event_chunks(desync(lines)):
+                        self._process_events(events)
                     self._command_offset = 1
                     return self.connected()
                 except Exception as ex:
-                    self.__logger.exception(ex)
+                    self._logger.exception(ex)
                     return False
 
-    def __handle_session_result(self, status_code: int, reason: str) -> bool:
+    def _handle_session_result(self, status_code: int, reason: str) -> bool:
         if status_code == 400 and "Unknown SID" in reason:
-            self.__connection_lost()
+            self._connection_lost()
             return False
         if status_code == 410 and "Gone" in reason:
-            self.__connection_lost()
+            self._connection_lost()
             return False
         return True
 
     async def subscribe(self, callback: Callable[[PlaybackState], Any]) -> None:
         """Start listening for events"""
         if not self.connected():
             raise Exception("Not connected")
@@ -403,38 +403,38 @@
             "CI": "0",
             "AID": self._last_event_id,
             "gsessionid": self._gsession,
             "TYPE": "xmlhttp",
         }
         req = PreparedRequest()
         req.prepare_url(f"{api_base}/bc/bind", params)
-        self.__logger.info("Subscribing to lounge id %s", self.auth.lounge_id_token)
+        self._logger.info("Subscribing to lounge id %s", self.auth.lounge_id_token)
         try:
             async with aiohttp.ClientSession(timeout=ClientTimeout()) as session:
                 async with session.get(req.url) as resp:
-                    if not self.__handle_session_result(resp.status, resp.reason):
+                    if not self._handle_session_result(resp.status, resp.reason):
                         return
 
-                    async for events in self.__parse_event_chunks(
+                    async for events in self._parse_event_chunks(
                         iter_response_lines(resp.content)
                     ):
                         pre_state_update = self.state_update
-                        self.__process_events(events)
+                        self._process_events(events)
                         if pre_state_update != self.state_update:
                             await callback(self.state)
                         if not self.connected():
                             break
-                    self.__logger.info(
+                    self._logger.info(
                         "Subscribe completed, status %i %s", resp.status, resp.reason
                     )
 
         except Exception as ex:
-            self.__logger.exception(ex)
+            self._logger.exception(ex)
 
-    async def __command(self, command: str, command_parameters: dict = None) -> bool:
+    async def _command(self, command: str, command_parameters: dict = None) -> bool:
         if not self.connected():
             raise Exception("Not connected")
 
         command_body = {"count": 1, "ofs": self._command_offset, "req0__sc": command}
         if command_parameters:
             for cmd_param in command_parameters:
                 value = command_parameters[cmd_param]
@@ -455,34 +455,34 @@
         }
         req = PreparedRequest()
         req.prepare_url(f"{api_base}/bc/bind", params)
         async with aiohttp.ClientSession() as session:
             async with session.post(url=req.url, data=command_body) as resp:
                 try:
                     response_text = await resp.text()
-                    if not self.__handle_session_result(resp.status, response_text):
+                    if not self._handle_session_result(resp.status, response_text):
                         return False
                     resp.raise_for_status()
                     return True
                 except Exception as ex:
-                    self.__logger.exception(ex)
+                    self._logger.exception(ex)
                     return False
 
     async def play(self) -> bool:
         """Sends play command to screen"""
-        return await self.__command("play")
+        return await self._command("play")
 
     async def pause(self) -> bool:
         """Sends pause command to screen"""
-        return await self.__command("pause")
+        return await self._command("pause")
 
     async def previous(self) -> bool:
         """Sends previous command to screen"""
-        return await self.__command("previous")
+        return await self._command("previous")
 
     async def next(self) -> bool:
         """Sends next command to screen"""
-        return await self.__command("next")
+        return await self._command("next")
 
     async def seek_to(self, time: float) -> bool:
         """Seek to given time (seconds)"""
-        return await self.__command("seekTo", {"newTime": time})
+        return await self._command("seekTo", {"newTime": time})
```

### Comparing `pyytlounge-1.4.3/LICENSE` & `pyytlounge-1.5.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pyytlounge-1.4.3/README.md` & `pyytlounge-1.5.0/README.md`

 * *Files identical despite different names*

### Comparing `pyytlounge-1.4.3/PKG-INFO` & `pyytlounge-1.5.0/PKG-INFO`

 * *Files 15% similar despite different names*

```diff
@@ -1,19 +1,24 @@
 Metadata-Version: 2.1
 Name: pyytlounge
-Version: 1.4.3
+Version: 1.5.0
 Summary: YouTube Lounge API wrapper
-Project-URL: Homepage, https://github.com/pypa/sampleproject
-Project-URL: Bug Tracker, https://github.com/pypa/sampleproject/issues
+Project-URL: Homepage, https://github.com/FabioGNR/pyytlounge
+Project-URL: Bug Tracker, https://github.com/FabioGNR/pyytlounge/issues
 Author-email: Fabio <example@example.com>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
+Requires-Dist: aiohttp==3.8.1
+Requires-Dist: requests==2.28.1
+Provides-Extra: tests
+Requires-Dist: pytest; extra == 'tests'
+Requires-Dist: pytest-mock; extra == 'tests'
 Description-Content-Type: text/markdown
 
 # YouTube Lounge API wrapper written in Python (WIP)
 
 ## Setup
 
 Activate virtual environment:
```

