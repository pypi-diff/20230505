# Comparing `tmp/aioca-1.6.tar.gz` & `tmp/aioca-1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/aioca/aioca/dist/tmpk85jzoav/aioca-1.6.tar", last modified: Thu Apr  6 14:27:37 2023, max compression
+gzip compressed data, was "/home/runner/work/aioca/aioca/dist/tmpr346ag9k/aioca-1.7.tar", last modified: Fri May  5 09:45:00 2023, max compression
```

## Comparing `aioca-1.6.tar` & `aioca-1.7.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxr-x   0 runner    (1001) docker     (123)        0 2023-04-06 14:27:37.000000 aioca-1.6/
--rw-rw-r--   0 runner    (1001) docker     (123)     3233 2023-04-06 14:27:37.000000 aioca-1.6/PKG-INFO
--rw-rw-r--   0 runner    (1001) docker     (123)     2069 2023-04-06 14:26:34.000000 aioca-1.6/README.rst
-drwxrwxr-x   0 runner    (1001) docker     (123)        0 2023-04-06 14:27:37.000000 aioca-1.6/aioca/
--rw-rw-r--   0 runner    (1001) docker     (123)     2533 2023-04-06 14:26:34.000000 aioca-1.6/aioca/__init__.py
--rw-rw-r--   0 runner    (1001) docker     (123)    39834 2023-04-06 14:26:34.000000 aioca-1.6/aioca/_catools.py
--rw-rw-r--   0 runner    (1001) docker     (123)     3756 2023-04-06 14:27:37.000000 aioca-1.6/aioca/_version_git.py
--rw-rw-r--   0 runner    (1001) docker     (123)     8396 2023-04-06 14:26:34.000000 aioca-1.6/aioca/types.py
-drwxrwxr-x   0 runner    (1001) docker     (123)        0 2023-04-06 14:27:37.000000 aioca-1.6/aioca.egg-info/
--rw-rw-r--   0 runner    (1001) docker     (123)     3233 2023-04-06 14:27:37.000000 aioca-1.6/aioca.egg-info/PKG-INFO
--rw-rw-r--   0 runner    (1001) docker     (123)      261 2023-04-06 14:27:37.000000 aioca-1.6/aioca.egg-info/SOURCES.txt
--rw-rw-r--   0 runner    (1001) docker     (123)        1 2023-04-06 14:27:37.000000 aioca-1.6/aioca.egg-info/dependency_links.txt
--rw-rw-r--   0 runner    (1001) docker     (123)      216 2023-04-06 14:27:37.000000 aioca-1.6/aioca.egg-info/requires.txt
--rw-rw-r--   0 runner    (1001) docker     (123)        6 2023-04-06 14:27:37.000000 aioca-1.6/aioca.egg-info/top_level.txt
--rw-rw-r--   0 runner    (1001) docker     (123)      173 2023-04-06 14:26:34.000000 aioca-1.6/pyproject.toml
--rw-rw-r--   0 runner    (1001) docker     (123)     1548 2023-04-06 14:27:37.000000 aioca-1.6/setup.cfg
--rw-rw-r--   0 runner    (1001) docker     (123)      386 2023-04-06 14:26:34.000000 aioca-1.6/setup.py
+drwxrwxr-x   0 runner    (1001) docker     (123)        0 2023-05-05 09:45:00.000000 aioca-1.7/
+-rw-rw-r--   0 runner    (1001) docker     (123)     3233 2023-05-05 09:45:00.000000 aioca-1.7/PKG-INFO
+-rw-rw-r--   0 runner    (1001) docker     (123)     2069 2023-05-05 09:43:23.000000 aioca-1.7/README.rst
+drwxrwxr-x   0 runner    (1001) docker     (123)        0 2023-05-05 09:45:00.000000 aioca-1.7/aioca/
+-rw-rw-r--   0 runner    (1001) docker     (123)     2700 2023-05-05 09:43:23.000000 aioca-1.7/aioca/__init__.py
+-rw-rw-r--   0 runner    (1001) docker     (123)    41091 2023-05-05 09:43:23.000000 aioca-1.7/aioca/_catools.py
+-rw-rw-r--   0 runner    (1001) docker     (123)     3756 2023-05-05 09:45:00.000000 aioca-1.7/aioca/_version_git.py
+-rw-rw-r--   0 runner    (1001) docker     (123)     8396 2023-05-05 09:43:23.000000 aioca-1.7/aioca/types.py
+drwxrwxr-x   0 runner    (1001) docker     (123)        0 2023-05-05 09:45:00.000000 aioca-1.7/aioca.egg-info/
+-rw-rw-r--   0 runner    (1001) docker     (123)     3233 2023-05-05 09:45:00.000000 aioca-1.7/aioca.egg-info/PKG-INFO
+-rw-rw-r--   0 runner    (1001) docker     (123)      261 2023-05-05 09:45:00.000000 aioca-1.7/aioca.egg-info/SOURCES.txt
+-rw-rw-r--   0 runner    (1001) docker     (123)        1 2023-05-05 09:45:00.000000 aioca-1.7/aioca.egg-info/dependency_links.txt
+-rw-rw-r--   0 runner    (1001) docker     (123)      216 2023-05-05 09:45:00.000000 aioca-1.7/aioca.egg-info/requires.txt
+-rw-rw-r--   0 runner    (1001) docker     (123)        6 2023-05-05 09:45:00.000000 aioca-1.7/aioca.egg-info/top_level.txt
+-rw-rw-r--   0 runner    (1001) docker     (123)      173 2023-05-05 09:43:23.000000 aioca-1.7/pyproject.toml
+-rw-rw-r--   0 runner    (1001) docker     (123)     1548 2023-05-05 09:45:00.000000 aioca-1.7/setup.cfg
+-rw-rw-r--   0 runner    (1001) docker     (123)      386 2023-05-05 09:43:23.000000 aioca-1.7/setup.py
```

### Comparing `aioca-1.6/PKG-INFO` & `aioca-1.7/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aioca
-Version: 1.6
+Version: 1.7
 Summary: Asynchronous Channel Access client for asyncio and Python using libca via ctypes
 Home-page: https://github.com/dls-controls/aioca
 Author: Tom Cobb
 Author-email: tom.cobb@diamond.ac.uk
 License: Apache License 2.0
 Description: aioca
         =====
```

### Comparing `aioca-1.6/README.rst` & `aioca-1.7/README.rst`

 * *Files identical despite different names*

### Comparing `aioca-1.6/aioca/__init__.py` & `aioca-1.7/aioca/__init__.py`

 * *Files 10% similar despite different names*

```diff
@@ -20,20 +20,22 @@
     FORMAT_TIME,
     ca_extra_fields,
 )
 
 from ._catools import (
     CAInfo,
     CANothing,
+    ChannelInfo,
     Subscription,
     caget,
     cainfo,
     camonitor,
     caput,
     connect,
+    get_channel_infos,
     purge_channel_caches,
     run,
 )
 from ._version_git import __version__
 
 __all__ = [
     # The core functions
@@ -41,14 +43,16 @@
     "caput",  # Write PVs to channel access
     "caget",  # Read PVs from channel access
     "camonitor",  # Monitor PVs over channel access
     "connect",  # Establish PV connection
     "cainfo",  # Returns ca_info describing PV connection
     "CAInfo",  # Ca info object
     "CANothing",  # No value
+    "ChannelInfo",  # Information about a particular channel
+    "get_channel_infos",  # Return information about all channels
     "purge_channel_caches",  # Get rid of old channels
     "run",  # Run one aioca coroutine and clean up
     # The version of aioca
     "__version__",
     # Event type notification codes for camonitor
     "DBE_VALUE",  # Notify normal value changes
     "DBE_LOG",  # Notify archival value changes
```

### Comparing `aioca-1.6/aioca/_catools.py` & `aioca-1.7/aioca/_catools.py`

 * *Files 2% similar despite different names*

```diff
@@ -50,14 +50,17 @@
         self.value: Union[T, Exception] = RuntimeError("No value set")
         self._event = asyncio.Event()
 
     def set(self, value: Union[T, Exception]):
         self._event.set()
         self.value = value
 
+    def is_set(self) -> bool:
+        return self._event.is_set()
+
     def clear(self):
         self._event.clear()
         self.value = RuntimeError("No value set")
 
     async def wait(self) -> T:
         if not self._event.is_set():
             await self._event.wait()
@@ -248,14 +251,22 @@
         notification."""
         self.__subscriptions.add(subscription)
 
     def _remove_subscription(self, subscription):
         """Removes the given subscription from the list of receivers."""
         self.__subscriptions.remove(subscription)
 
+    def count_subscriptions(self) -> int:
+        """Return the number of currently active subscriptions for this Channel"""
+        return len(self.__subscriptions)
+
+    def connected(self) -> bool:
+        """Return whether this Channel is currently connected to a PV"""
+        return self.__connect_event.is_set()
+
     async def wait(self):
         """Waits for the channel to become connected if not already connected."""
         await self.__connect_event.wait()
 
 
 class ChannelCache(object):
     """A cache of all open channels.  If a channel is not present in the
@@ -274,14 +285,17 @@
             return self.__channels[name]
         except KeyError:
             # Have to create a new channel
             channel = Channel(name, self.__loop)
             self.__channels[name] = channel
             return channel
 
+    def get_channels(self) -> List[Channel]:
+        return list(self.__channels.values())
+
     def purge(self):
         """Purges all the channels in the cache: closes them right now.  Will
         cause other channel access to fail, so only to be done on shutdown."""
         for channel in self.__channels.values():
             channel._purge()
         self.__channels.clear()
 
@@ -1077,14 +1091,40 @@
 
 def get_channel(pv: str) -> Channel:
     channel_cache = _Context.get_channel_cache()
     channel = channel_cache.get_channel(pv)
     return channel
 
 
+class ChannelInfo:
+    """Information about a particular Channel
+
+    Attributes:
+        name: Process Variable name the Channel is targeting
+        connected: True if the Channel is currently connected
+        subscriber_count: Number of clients subscribed to this Channel"""
+
+    name: str
+    connected: bool
+    subscriber_count: int
+
+    def __init__(self, name, connected, subscriber_count):
+        self.name = name
+        self.connected = connected
+        self.subscriber_count = subscriber_count
+
+
+def get_channel_infos() -> List[ChannelInfo]:
+    """Return information about all Channels"""
+    return [
+        ChannelInfo(channel.name, channel.connected(), channel.count_subscriptions())
+        for channel in _Context.get_channel_cache().get_channels()
+    ]
+
+
 # Another delicacy arising from relying on asynchronous CA event dispatching is
 # that we need to manually flush IO events such as caget commands.  To ensure
 # that large blocks of channel access activity really are aggregated we used to
 # ensure that ca_flush_io() is only called once in any scheduling cycle, but now
 # we just call it every time
 _flush_io = cadef.ca_flush_io
```

### Comparing `aioca-1.6/aioca/_version_git.py` & `aioca-1.7/aioca/_version_git.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,16 +4,16 @@
 # versiongit-0.6 (https://github.com/dls-controls/versiongit)
 import os
 import re
 import sys
 from subprocess import STDOUT, CalledProcessError, check_output
 
 # These will be filled in if git archive is run or by setup.py cmdclasses
-GIT_REFS = 'tag: 1.6'
-GIT_SHA1 = 'a5500d0'
+GIT_REFS = 'tag: 1.7'
+GIT_SHA1 = '216bcc3'
 
 
 def get_version_from_git(path=None):
     """Try to parse version from git describe, fallback to git archive tags"""
     tag, plus, suffix = "0", "untagged", ""
     if not GIT_SHA1.startswith("$"):
         # git archive or the cmdclasses below have filled in these strings
```

### Comparing `aioca-1.6/aioca/types.py` & `aioca-1.7/aioca/types.py`

 * *Files identical despite different names*

### Comparing `aioca-1.6/aioca.egg-info/PKG-INFO` & `aioca-1.7/aioca.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aioca
-Version: 1.6
+Version: 1.7
 Summary: Asynchronous Channel Access client for asyncio and Python using libca via ctypes
 Home-page: https://github.com/dls-controls/aioca
 Author: Tom Cobb
 Author-email: tom.cobb@diamond.ac.uk
 License: Apache License 2.0
 Description: aioca
         =====
```

### Comparing `aioca-1.6/setup.cfg` & `aioca-1.7/setup.cfg`

 * *Files identical despite different names*

