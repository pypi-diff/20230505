# Comparing `tmp/pymee-1.6.0.tar.gz` & `tmp/pymee-1.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pymee-1.6.0.tar", last modified: Mon Feb 20 09:41:19 2023, max compression
+gzip compressed data, was "pymee-1.7.0.tar", last modified: Fri May  5 07:03:39 2023, max compression
```

## Comparing `pymee-1.6.0.tar` & `pymee-1.7.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-20 09:41:19.531473 pymee-1.6.0/
--rw-r--r--   0 root         (0) root         (0)     1069 2023-02-20 09:41:16.000000 pymee-1.6.0/LICENSE
--rw-r--r--   0 root         (0) root         (0)     6037 2023-02-20 09:41:19.531473 pymee-1.6.0/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     5627 2023-02-20 09:41:16.000000 pymee-1.6.0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-20 09:41:19.527473 pymee-1.6.0/pymee/
--rw-r--r--   0 root         (0) root         (0)    16323 2023-02-20 09:41:16.000000 pymee-1.6.0/pymee/__init__.py
--rw-r--r--   0 root         (0) root         (0)    26751 2023-02-20 09:41:16.000000 pymee-1.6.0/pymee/const.py
--rw-r--r--   0 root         (0) root         (0)    10984 2023-02-20 09:41:16.000000 pymee-1.6.0/pymee/model.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-02-20 09:41:19.531473 pymee-1.6.0/pymee.egg-info/
--rw-r--r--   0 root         (0) root         (0)     6037 2023-02-20 09:41:19.000000 pymee-1.6.0/pymee.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      200 2023-02-20 09:41:19.000000 pymee-1.6.0/pymee.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-02-20 09:41:19.000000 pymee-1.6.0/pymee.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)        6 2023-02-20 09:41:19.000000 pymee-1.6.0/pymee.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       98 2023-02-20 09:41:19.531473 pymee-1.6.0/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      647 2023-02-20 09:41:16.000000 pymee-1.6.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 07:03:39.354405 pymee-1.7.0/
+-rw-r--r--   0 root         (0) root         (0)     1069 2023-05-05 07:03:36.000000 pymee-1.7.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)     6037 2023-05-05 07:03:39.354405 pymee-1.7.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     5627 2023-05-05 07:03:36.000000 pymee-1.7.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 07:03:39.354405 pymee-1.7.0/pymee/
+-rw-r--r--   0 root         (0) root         (0)    16359 2023-05-05 07:03:36.000000 pymee-1.7.0/pymee/__init__.py
+-rw-r--r--   0 root         (0) root         (0)    26751 2023-05-05 07:03:36.000000 pymee-1.7.0/pymee/const.py
+-rw-r--r--   0 root         (0) root         (0)    10984 2023-05-05 07:03:36.000000 pymee-1.7.0/pymee/model.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 07:03:39.354405 pymee-1.7.0/pymee.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     6037 2023-05-05 07:03:39.000000 pymee-1.7.0/pymee.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      200 2023-05-05 07:03:39.000000 pymee-1.7.0/pymee.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-05 07:03:39.000000 pymee-1.7.0/pymee.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)        6 2023-05-05 07:03:39.000000 pymee-1.7.0/pymee.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       98 2023-05-05 07:03:39.354405 pymee-1.7.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      647 2023-05-05 07:03:37.000000 pymee-1.7.0/setup.py
```

### Comparing `pymee-1.6.0/LICENSE` & `pymee-1.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `pymee-1.6.0/PKG-INFO` & `pymee-1.7.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pymee
-Version: 1.6.0
+Version: 1.7.0
 Summary: a python library to interact with homee
 Home-page: https://github.com/FreshlyBrewedCode/pymee
 Author: FreshlyBrewedCode
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
```

### Comparing `pymee-1.6.0/README.md` & `pymee-1.7.0/README.md`

 * *Files identical despite different names*

### Comparing `pymee-1.6.0/pymee/__init__.py` & `pymee-1.7.0/pymee/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -13,29 +13,30 @@
     HomeeNode,
     HomeeRelationship,
     HomeeSettings,
 )
 import re
 import logging
 
+_LOGGER = logging.getLogger(__name__)
+
 
 class Homee:
     def __init__(
         self,
         host: str,
         user: str,
         password: str,
         device: str = "pymee",
         pingInterval: int = 30,
         reconnectInterval: int = 5,
         reconnect: bool = True,
         maxRetries: int = 5,
         loop: asyncio.AbstractEventLoop = None,
     ) -> None:
-
         self.host = host
         self.user = user
         self.password = password
 
         self.device = device
         self.pingInterval = pingInterval
         self.shouldReconnect = reconnect
@@ -138,15 +139,15 @@
     def start(self):
         """Wraps run() with asyncio.create_task() and returns the resulting task."""
         return asyncio.create_task(self.run())
 
     async def open_ws(self):
         """Opens the websocket connection assuming an access token was already received. Runs until connection is closed again."""
 
-        self._log("Opening websocket...")
+        _LOGGER.info("Opening websocket...")
 
         if self.retries > 0:
             await self.on_reconnect()
 
         try:
             async with websockets.connect(
                 uri=f"{self.ws_url}/connection?access_token={self.token}",
@@ -212,21 +213,21 @@
 
     async def _ws_ping_handler(self, ws: websockets.WebSocketClientProtocol):
         if self.pingInterval <= 0:
             return
 
         while self.connected and not self.shouldClose and ws.open:
             await ws.ping()
-            self._log("PING!")
+            _LOGGER.debug("PING!")
             await asyncio.sleep(self.pingInterval)
 
     async def _ws_on_open(self):
         """Websocket on_open callback."""
 
-        self._log("Connection to websocket successfull")
+        _LOGGER.info("Connection to websocket successfull")
 
         self.connected = True
 
         await self.on_connected()
         self.retries = 0
 
         await self.send("GET:all")
@@ -244,29 +245,29 @@
         self._disconnected_event.set()
 
         await self.on_disconnected()
 
     async def _ws_on_error(self, error):
         """Websocket on_error callback."""
 
-        self._log(f"An error occurred: {error}")
+        _LOGGER.error(f"An error occurred: {error}")
         await self.on_error(error)
 
     async def send(self, msg: str):
         """Send a raw string message to homee."""
 
         if not self.connected or self.shouldClose:
             return
 
         await self._message_queue.put(msg)
 
     async def reconnect(self):
         """Start a reconnection attempt."""
 
-        self._log(
+        _LOGGER.info(
             f"Attempting to reconnect in {self.reconnectInterval * self.retries} seconds..."
         )
 
         await asyncio.sleep(self.reconnectInterval * self.retries)
         await self.run()
 
     def disconnect(self):
@@ -278,19 +279,19 @@
         """Internal handleing of incoming homee messages."""
 
         msgType = None
 
         try:
             msgType = list(msg)[0]
         except:
-            self._log(f"Invalid message: {msg}")
+            _LOGGER.warn(f"Invalid message: {msg}")
             await self.on_error()
             return
 
-        self._log(msg)
+        _LOGGER.debug(msg)
 
         if msgType == "all":
             self.settings = HomeeSettings(msg["all"]["settings"])
 
             # Create / Update nodes
             if len(self.nodes) <= 0:
                 self.nodes = list(map(lambda n: HomeeNode(n), msg["all"]["nodes"]))
@@ -324,22 +325,22 @@
             self._update_or_create_relationships(msg["relationships"])
             self._remap_relationships()
         elif msgType == "group":
             self._update_or_create_group(msg["group"])
         elif msgType == "relationship":
             self._update_or_create_relationship(msg["relationship"])
         else:
-            self._log(f"Unknown/Unsupported message type: {msgType}")
+            _LOGGER.info(f"Unknown/Unsupported message type: {msgType}")
 
         await self.on_message(msg)
 
     async def _handle_attribute_change(self, attribute_data: dict):
         """Internal handleling of an attribute changed message."""
 
-        self._log(f"Updating attribute {attribute_data['id']}")
+        _LOGGER.info(f"Updating attribute {attribute_data['id']}")
 
         # try:
         attrNodeId = attribute_data["node_id"]
         node = self.get_node_by_id(attrNodeId)
         if node != None:
             node._update_attribute(attribute_data)
             await self.on_attribute_updated(attribute_data, node)
@@ -417,15 +418,17 @@
         """Returns the group with the given id or `None` if no group with the given id exists."""
         index = self.get_group_index(groupId)
         return self.groups[index] if index != -1 else None
 
     async def set_value(self, deviceId: int, attributeId: int, value: float):
         """Set the target value of an attribute of a device."""
 
-        self._log(f"Set value: Device: {deviceId} Attribute: {attributeId} To: {value}")
+        _LOGGER.info(
+            f"Set value: Device: {deviceId} Attribute: {attributeId} To: {value}"
+        )
         await self.send(
             f"PUT:/nodes/{deviceId}/attributes/{attributeId}?target_value={value}"
         )
 
     async def play_homeegram(self, homeegramId: int):
         """Invoke a homeegram."""
 
@@ -440,15 +443,15 @@
     @property
     def ws_url(self):
         """Local homee websocket url."""
 
         return f"ws://{self.host}:7681"
 
     def wait_until_connected(self):
-        """"Returns a coroutine that runs until a connection has been established and the initial data has been received."""
+        """ "Returns a coroutine that runs until a connection has been established and the initial data has been received."""
         return self._connected_event.wait()
 
     def wait_until_disconnected(self):
         """Returns a coroutine that runs until the connection has been closed."""
         return self._disconnected_event.wait()
 
     async def on_reconnect(self):
@@ -468,17 +471,14 @@
 
     async def on_message(self, msg: dict):
         """Called when the websocket receives a message. The message is automatically parsed from json into a dictionary."""
 
     async def on_attribute_updated(self, attribute_data: dict, node: HomeeNode):
         """Called when an 'attribute' message was received and an attribute was updated. Contains the parsed json attribute data and the corresponding node instance."""
 
-    def _log(self, msg: str):
-        logging.debug(msg)
-
 
 class HomeeException(Exception):
     """Base class for all errors thrown by this library"""
 
 
 class AuthenticationFailedException(HomeeException):
     """Raised if no valid access token could be acquired."""
```

### Comparing `pymee-1.6.0/pymee/const.py` & `pymee-1.7.0/pymee/const.py`

 * *Files identical despite different names*

### Comparing `pymee-1.6.0/pymee/model.py` & `pymee-1.7.0/pymee/model.py`

 * *Files identical despite different names*

### Comparing `pymee-1.6.0/pymee.egg-info/PKG-INFO` & `pymee-1.7.0/pymee.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pymee
-Version: 1.6.0
+Version: 1.7.0
 Summary: a python library to interact with homee
 Home-page: https://github.com/FreshlyBrewedCode/pymee
 Author: FreshlyBrewedCode
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.6
```

### Comparing `pymee-1.6.0/setup.py` & `pymee-1.7.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 import setuptools
 
-__version__ = "1.6.0"
+__version__ = "1.7.0"
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="pymee",
     version=__version__,
```

