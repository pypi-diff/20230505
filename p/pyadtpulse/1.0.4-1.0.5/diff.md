# Comparing `tmp/pyadtpulse-1.0.4-py3-none-any.whl.zip` & `tmp/pyadtpulse-1.0.5-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,13 +1,13 @@
-Zip file size: 21418 bytes, number of entries: 11
+Zip file size: 22431 bytes, number of entries: 11
 -rw-r--r--  2.0 unx    34446 b- defN 23-Apr-29 06:07 pyadtpulse/__init__.py
 -rw-r--r--  2.0 unx     1609 b- defN 23-Mar-28 16:07 pyadtpulse/const.py
 -rw-r--r--  2.0 unx    24957 b- defN 23-Apr-29 06:07 pyadtpulse/site.py
--rw-r--r--  2.0 unx     4803 b- defN 23-Mar-28 16:07 pyadtpulse/util.py
+-rw-r--r--  2.0 unx     5877 b- defN 23-May-05 03:34 pyadtpulse/util.py
 -rw-r--r--  2.0 unx     5847 b- defN 23-Apr-29 06:07 pyadtpulse/zones.py
--rw-r--r--  2.0 unx      581 b- defN 23-May-02 07:01 pyadtpulse-1.0.4.dist-info/LICENSE.md
--rw-r--r--  2.0 unx     3680 b- defN 23-May-02 07:01 pyadtpulse-1.0.4.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-May-02 07:01 pyadtpulse-1.0.4.dist-info/WHEEL
--rw-r--r--  2.0 unx       11 b- defN 23-May-02 07:01 pyadtpulse-1.0.4.dist-info/top_level.txt
--rw-r--r--  2.0 unx        1 b- defN 23-Apr-18 03:34 pyadtpulse-1.0.4.dist-info/zip-safe
--rw-rw-r--  2.0 unx      875 b- defN 23-May-02 07:01 pyadtpulse-1.0.4.dist-info/RECORD
-11 files, 76902 bytes uncompressed, 19944 bytes compressed:  74.1%
+-rw-r--r--  2.0 unx      581 b- defN 23-May-05 03:34 pyadtpulse-1.0.5.dist-info/LICENSE.md
+-rw-r--r--  2.0 unx     5206 b- defN 23-May-05 03:34 pyadtpulse-1.0.5.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-May-05 03:34 pyadtpulse-1.0.5.dist-info/WHEEL
+-rw-r--r--  2.0 unx       11 b- defN 23-May-05 03:34 pyadtpulse-1.0.5.dist-info/top_level.txt
+-rw-r--r--  2.0 unx        1 b- defN 23-Apr-18 03:34 pyadtpulse-1.0.5.dist-info/zip-safe
+-rw-rw-r--  2.0 unx      875 b- defN 23-May-05 03:34 pyadtpulse-1.0.5.dist-info/RECORD
+11 files, 79502 bytes uncompressed, 20957 bytes compressed:  73.6%
```

## zipnote {}

```diff
@@ -9,26 +9,26 @@
 
 Filename: pyadtpulse/util.py
 Comment: 
 
 Filename: pyadtpulse/zones.py
 Comment: 
 
-Filename: pyadtpulse-1.0.4.dist-info/LICENSE.md
+Filename: pyadtpulse-1.0.5.dist-info/LICENSE.md
 Comment: 
 
-Filename: pyadtpulse-1.0.4.dist-info/METADATA
+Filename: pyadtpulse-1.0.5.dist-info/METADATA
 Comment: 
 
-Filename: pyadtpulse-1.0.4.dist-info/WHEEL
+Filename: pyadtpulse-1.0.5.dist-info/WHEEL
 Comment: 
 
-Filename: pyadtpulse-1.0.4.dist-info/top_level.txt
+Filename: pyadtpulse-1.0.5.dist-info/top_level.txt
 Comment: 
 
-Filename: pyadtpulse-1.0.4.dist-info/zip-safe
+Filename: pyadtpulse-1.0.5.dist-info/zip-safe
 Comment: 
 
-Filename: pyadtpulse-1.0.4.dist-info/RECORD
+Filename: pyadtpulse-1.0.5.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## pyadtpulse/util.py

```diff
@@ -1,10 +1,14 @@
 """Utility functions for pyadtpulse."""
 import logging
+import string
 import sys
+from base64 import urlsafe_b64encode
+from pathlib import Path
+from random import randint
 from threading import RLock, current_thread
 from typing import Optional
 
 from aiohttp import ClientResponse
 from bs4 import BeautifulSoup
 
 LOG = logging.getLogger(__name__)
@@ -67,14 +71,48 @@
     if response is None:  # shut up type checker
         return None
     body_text = await response.text()
     response.close()
     return BeautifulSoup(body_text, "html.parser")
 
 
+FINGERPRINT_LENGTH = 2292
+ALLOWABLE_CHARACTERS = list(string.ascii_letters + string.digits)
+FINGERPRINT_RANGE_LEN = len(ALLOWABLE_CHARACTERS)
+
+
+def generate_random_fingerprint() -> str:
+    """Generate a random browser fingerprint string.
+
+    Returns:
+        str: a fingerprint string
+    """
+    fingerprint = [
+        ALLOWABLE_CHARACTERS[(randint(0, FINGERPRINT_RANGE_LEN - 1))]
+        for i in range(FINGERPRINT_LENGTH)
+    ]
+    return "".join(fingerprint)
+
+
+def generate_fingerprint_from_browser_json(filename: str) -> str:
+    """Generate a browser fingerprint from a JSON file.
+
+    Args:
+        filename (str): JSON file containing fingerprint information
+
+    Returns:
+        str: the fingerprint
+    """
+    data = Path(filename).read_text()
+    # Pulse just calls JSON.Stringify() and btoa() in javascript, so we need to
+    # do this to emulate that
+    data2 = "".join(data.split())
+    return str(urlsafe_b64encode(data2.encode("utf-8")), "utf-8")
+
+
 class DebugRLock:
     """Provides a debug lock logging caller who acquired/released."""
 
     def __init__(self, name: str):
         """Create the lock."""
         self._Rlock = RLock()
         self._lock_name = name
```

## Comparing `pyadtpulse-1.0.4.dist-info/LICENSE.md` & `pyadtpulse-1.0.5.dist-info/LICENSE.md`

 * *Files identical despite different names*

## Comparing `pyadtpulse-1.0.4.dist-info/METADATA` & `pyadtpulse-1.0.5.dist-info/METADATA`

 * *Files 25% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyadtpulse
-Version: 1.0.4
+Version: 1.0.5
 Summary: Python interface for ADT Pulse security systems
 Home-page: https://github.com/rsnodgrass/pyadtpulse
 Author: 
 Author-email: 
 License: Apache Software License
 Keywords: security system,adt,home automation,security alarm
 Classifier: Programming Language :: Python :: 3
@@ -26,15 +26,15 @@
 ## UNSUPPORTED
 
 **This is an unsupported interface provided only as a basis for others to explore integrating
 their ADT system wtih their own tools.**
 
 While two or three Python clients to ADT Pulse existed, they generally only provided
 arm/disarm support and none provided support for ADT Pulse when multiple sites existed
-under a single account. This attempts to provide APIs to both all the zones (motion 
+under a single account. This attempts to provide APIs to both all the zones (motion
 sensors, door sensors, etc) as well as arming and disarming individual sites.
 
 NOTE: Since this interacts with the unofficial ADT Pulse AJAX web service, the
 behavior is subject to change by ADT without notice.
 
 ## Developer Note
 
@@ -59,40 +59,76 @@
 Additionally, since pyadtpulse currently does not support multiple sites (premises/locations), a
 simple approach is to create a separate username/password for each site and configured such that
 the username only has access to ONE site. This ensures that clients are always interacting with
 that one site (and not accidentally with another site location).
 
 #### Notes
 
-* any changes to the name/count of sites are not automatically updated for existing site objects 
+- any changes to the name/count of sites are not automatically updated for existing site objects
 
 ## Examples
 
 ```python
-adt = PyADTPulse(username, password)
+adt = PyADTPulse(username, password, fingerprint)
 
 for site in adt.sites:
     site.status
     site.zones
 
     site.disarm()
     site.arm_away()
+    site.arm_away(force=True)
+```
+
+Async version (preferred for new integrations):
+
+```python
+adt = PyADTPulse(username, password, fingerprint, do_login=false)
+
+await adt.async_login()
+
+for site in adt.sites:
+    site.status
+    site.zones
+
+    await site.async_disarm()
+    await site.async_arm_away()
+    await site.async_arm_away(force=True)
 ```
 
 See [example-client.py](example-client.py) for a working example.
 
+## Browser Fingerprinting
+
+ADT Pulse requires 2 factor authentication to log into their site. When you perform the 2 factor authentication, you will see an option to save the browser to not have to re-authenticate through it.
+
+Internally, ADT uses some Javascript code to create a browser fingerprint. This (very long) string is used to check that the browser has been saved upon subsequent logins. It is the "fingerprint" parameter required to be passed in to the PyADTPulse object constructor.
+
+### Note:
+
+The browser fingerprint will change with a browser/OS upgrade. For this reason, it is recommended to create a separate username in ADT Pulse just for monitoring.
+
+There are 2 ways to determine this fingerprint:
+
+1. Visit [this link](https://rawcdn.githack.com/rlippmann/pyadtpulse/b3a0e7097e22446623d170f0a971726fbedb6a2d/doc/browser_fingerprint.html) using the same browser you used to authenticate with ADT Pulse. This should determine the correct browser fingerprint
+
+2. Follow the instructions [here](https://github.com/mrjackyliang/homebridge-adt-pulse#configure-2-factor-authentication)
+
 ## See Also
 
-* [ADT Pulse Portal](https://portal.adtpulse.com/)
-* [Home Assistant ADT Pulse integration](https://github.com/rsnodgrass/hass-adtpulse/)
-* [adt-pulse-mqtt](https://github.com/haruny/adt-pulse-mqtt) – MQTT integration with ADT Pulse alarm panels
+- [ADT Pulse Portal](https://portal.adtpulse.com/)
+- [Home Assistant ADT Pulse integration](https://github.com/rsnodgrass/hass-adtpulse/)
+- [adt-pulse-mqtt](https://github.com/haruny/adt-pulse-mqtt) – MQTT integration with ADT Pulse alarm panels
 
 ## Future Enhancements
 
-Feature ideas, but no plans to implement:
+Feature ideas:
 
-* support OFFLINE status checking
-* support multiple sites (premises/locations) under a single ADT account
-* implement lightweight status pings to check if cache needs to be invalidated (every 5 seconds) (https://portal.adtpulse.com/myhome/16.0.0-131/Ajax/SyncCheckServ?t=1568950496392)
-* alarm history (/ajax/alarmHistory.jsp)
+- 2 factor authenciation
+- Cameras (via Janus)
 
+Feature ideas, but no plans to implement:
 
+- support OFFLINE status checking
+- support multiple sites (premises/locations) under a single ADT account
+  ~~- implement lightweight status pings to check if cache needs to be invalidated (every 5 seconds) (https://portal.adtpulse.com/myhome/16.0.0-131/Ajax/SyncCheckServ?t=1568950496392)~~
+- alarm history (/ajax/alarmHistory.jsp)
```

