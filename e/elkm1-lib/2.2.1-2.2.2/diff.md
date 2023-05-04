# Comparing `tmp/elkm1_lib-2.2.1.tar.gz` & `tmp/elkm1_lib-2.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "elkm1_lib-2.2.1.tar", max compression
+gzip compressed data, was "elkm1_lib-2.2.2.tar", max compression
```

## Comparing `elkm1_lib-2.2.1.tar` & `elkm1_lib-2.2.2.tar`

### file list

```diff
@@ -1,31 +1,30 @@
--rw-r--r--   0        0        0     9610 2022-12-01 01:19:25.910593 elkm1_lib-2.2.1/CHANGELOG.md
--rw-r--r--   0        0        0     9289 2022-12-01 01:19:25.910593 elkm1_lib-2.2.1/README.md
--rw-r--r--   0        0        0    12509 2022-12-01 01:19:25.910593 elkm1_lib-2.2.1/bin/cmdr.py
--rwxr-xr-x   0        0        0     3088 2022-12-01 01:19:25.910593 elkm1_lib-2.2.1/bin/elk
--rwxr-xr-x   0        0        0     2165 2022-12-01 01:19:25.914593 elkm1_lib-2.2.1/bin/mkdoc
--rwxr-xr-x   0        0        0     1259 2022-12-01 01:19:25.914593 elkm1_lib-2.2.1/bin/simple
--rwxr-xr-x   0        0        0     2117 2022-12-01 01:19:25.914593 elkm1_lib-2.2.1/bin/test-serial
--rw-r--r--   0        0        0       41 2022-12-01 01:19:25.914593 elkm1_lib-2.2.1/elkm1_lib/__init__.py
--rw-r--r--   0        0        0     5127 2022-12-01 01:19:25.914593 elkm1_lib-2.2.1/elkm1_lib/areas.py
--rw-r--r--   0        0        0     7032 2022-12-01 01:19:25.914593 elkm1_lib-2.2.1/elkm1_lib/connection.py
--rw-r--r--   0        0        0    10373 2022-12-01 01:19:25.914593 elkm1_lib-2.2.1/elkm1_lib/const.py
--rw-r--r--   0        0        0     1424 2022-12-01 01:19:25.914593 elkm1_lib-2.2.1/elkm1_lib/counters.py
--rw-r--r--   0        0        0     5827 2022-12-01 01:19:25.914593 elkm1_lib-2.2.1/elkm1_lib/discovery.py
--rw-r--r--   0        0        0     5119 2022-12-01 01:19:25.914593 elkm1_lib-2.2.1/elkm1_lib/elements.py
--rw-r--r--   0        0        0     5183 2022-12-01 01:19:25.914593 elkm1_lib-2.2.1/elkm1_lib/elk.py
--rw-r--r--   0        0        0     3586 2022-12-01 01:19:25.914593 elkm1_lib-2.2.1/elkm1_lib/keypads.py
--rw-r--r--   0        0        0     1835 2022-12-01 01:19:25.914593 elkm1_lib-2.2.1/elkm1_lib/lights.py
--rw-r--r--   0        0        0    18619 2022-12-01 01:19:25.914593 elkm1_lib-2.2.1/elkm1_lib/message.py
--rw-r--r--   0        0        0     1478 2022-12-01 01:19:25.914593 elkm1_lib-2.2.1/elkm1_lib/notify.py
--rw-r--r--   0        0        0     1691 2022-12-01 01:19:25.914593 elkm1_lib-2.2.1/elkm1_lib/outputs.py
--rw-r--r--   0        0        0     4437 2022-12-01 01:19:25.914593 elkm1_lib-2.2.1/elkm1_lib/panel.py
--rw-r--r--   0        0        0        0 2022-12-01 01:19:25.914593 elkm1_lib-2.2.1/elkm1_lib/py.typed
--rw-r--r--   0        0        0     1848 2022-12-01 01:19:25.914593 elkm1_lib-2.2.1/elkm1_lib/settings.py
--rw-r--r--   0        0        0     1096 2022-12-01 01:19:25.914593 elkm1_lib-2.2.1/elkm1_lib/tasks.py
--rw-r--r--   0        0        0     3196 2022-12-01 01:19:25.914593 elkm1_lib-2.2.1/elkm1_lib/thermostats.py
--rw-r--r--   0        0        0      974 2022-12-01 01:19:25.914593 elkm1_lib-2.2.1/elkm1_lib/users.py
--rw-r--r--   0        0        0     2034 2022-12-01 01:19:25.914593 elkm1_lib-2.2.1/elkm1_lib/util.py
--rw-r--r--   0        0        0     4933 2022-12-01 01:19:25.914593 elkm1_lib-2.2.1/elkm1_lib/zones.py
--rw-r--r--   0        0        0     1943 2022-12-01 01:19:25.914593 elkm1_lib-2.2.1/pyproject.toml
--rw-r--r--   0        0        0    10257 1970-01-01 00:00:00.000000 elkm1_lib-2.2.1/setup.py
--rw-r--r--   0        0        0    10027 1970-01-01 00:00:00.000000 elkm1_lib-2.2.1/PKG-INFO
+-rw-r--r--   0        0        0     9610 2023-05-04 22:03:28.971976 elkm1_lib-2.2.2/CHANGELOG.md
+-rw-r--r--   0        0        0     9289 2023-05-04 22:03:28.971976 elkm1_lib-2.2.2/README.md
+-rw-r--r--   0        0        0    12509 2023-05-04 22:03:28.971976 elkm1_lib-2.2.2/bin/cmdr.py
+-rwxr-xr-x   0        0        0     3088 2023-05-04 22:03:28.971976 elkm1_lib-2.2.2/bin/elk
+-rwxr-xr-x   0        0        0     2165 2023-05-04 22:03:28.971976 elkm1_lib-2.2.2/bin/mkdoc
+-rwxr-xr-x   0        0        0     1259 2023-05-04 22:03:28.971976 elkm1_lib-2.2.2/bin/simple
+-rwxr-xr-x   0        0        0     2117 2023-05-04 22:03:28.971976 elkm1_lib-2.2.2/bin/test-serial
+-rw-r--r--   0        0        0       41 2023-05-04 22:03:28.971976 elkm1_lib-2.2.2/elkm1_lib/__init__.py
+-rw-r--r--   0        0        0     5127 2023-05-04 22:03:28.971976 elkm1_lib-2.2.2/elkm1_lib/areas.py
+-rw-r--r--   0        0        0     7032 2023-05-04 22:03:28.971976 elkm1_lib-2.2.2/elkm1_lib/connection.py
+-rw-r--r--   0        0        0    10373 2023-05-04 22:03:28.971976 elkm1_lib-2.2.2/elkm1_lib/const.py
+-rw-r--r--   0        0        0     1424 2023-05-04 22:03:28.971976 elkm1_lib-2.2.2/elkm1_lib/counters.py
+-rw-r--r--   0        0        0     5827 2023-05-04 22:03:28.971976 elkm1_lib-2.2.2/elkm1_lib/discovery.py
+-rw-r--r--   0        0        0     5119 2023-05-04 22:03:28.975976 elkm1_lib-2.2.2/elkm1_lib/elements.py
+-rw-r--r--   0        0        0     5183 2023-05-04 22:03:28.975976 elkm1_lib-2.2.2/elkm1_lib/elk.py
+-rw-r--r--   0        0        0     3586 2023-05-04 22:03:28.975976 elkm1_lib-2.2.2/elkm1_lib/keypads.py
+-rw-r--r--   0        0        0     1835 2023-05-04 22:03:28.975976 elkm1_lib-2.2.2/elkm1_lib/lights.py
+-rw-r--r--   0        0        0    18619 2023-05-04 22:03:28.975976 elkm1_lib-2.2.2/elkm1_lib/message.py
+-rw-r--r--   0        0        0     1478 2023-05-04 22:03:28.975976 elkm1_lib-2.2.2/elkm1_lib/notify.py
+-rw-r--r--   0        0        0     1691 2023-05-04 22:03:28.975976 elkm1_lib-2.2.2/elkm1_lib/outputs.py
+-rw-r--r--   0        0        0     4437 2023-05-04 22:03:28.975976 elkm1_lib-2.2.2/elkm1_lib/panel.py
+-rw-r--r--   0        0        0        0 2023-05-04 22:03:28.975976 elkm1_lib-2.2.2/elkm1_lib/py.typed
+-rw-r--r--   0        0        0     1848 2023-05-04 22:03:28.975976 elkm1_lib-2.2.2/elkm1_lib/settings.py
+-rw-r--r--   0        0        0     1096 2023-05-04 22:03:28.975976 elkm1_lib-2.2.2/elkm1_lib/tasks.py
+-rw-r--r--   0        0        0     3196 2023-05-04 22:03:28.975976 elkm1_lib-2.2.2/elkm1_lib/thermostats.py
+-rw-r--r--   0        0        0      974 2023-05-04 22:03:28.975976 elkm1_lib-2.2.2/elkm1_lib/users.py
+-rw-r--r--   0        0        0     2490 2023-05-04 22:03:28.975976 elkm1_lib-2.2.2/elkm1_lib/util.py
+-rw-r--r--   0        0        0     4933 2023-05-04 22:03:28.975976 elkm1_lib-2.2.2/elkm1_lib/zones.py
+-rw-r--r--   0        0        0     1943 2023-05-04 22:03:28.975976 elkm1_lib-2.2.2/pyproject.toml
+-rw-r--r--   0        0        0    10027 1970-01-01 00:00:00.000000 elkm1_lib-2.2.2/PKG-INFO
```

### Comparing `elkm1_lib-2.2.1/CHANGELOG.md` & `elkm1_lib-2.2.2/CHANGELOG.md`

 * *Files identical despite different names*

### Comparing `elkm1_lib-2.2.1/README.md` & `elkm1_lib-2.2.2/README.md`

 * *Files identical despite different names*

### Comparing `elkm1_lib-2.2.1/bin/cmdr.py` & `elkm1_lib-2.2.2/bin/cmdr.py`

 * *Files identical despite different names*

### Comparing `elkm1_lib-2.2.1/bin/elk` & `elkm1_lib-2.2.2/bin/elk`

 * *Files identical despite different names*

### Comparing `elkm1_lib-2.2.1/bin/mkdoc` & `elkm1_lib-2.2.2/bin/mkdoc`

 * *Files identical despite different names*

### Comparing `elkm1_lib-2.2.1/bin/simple` & `elkm1_lib-2.2.2/bin/simple`

 * *Files identical despite different names*

### Comparing `elkm1_lib-2.2.1/bin/test-serial` & `elkm1_lib-2.2.2/bin/test-serial`

 * *Files identical despite different names*

### Comparing `elkm1_lib-2.2.1/elkm1_lib/areas.py` & `elkm1_lib-2.2.2/elkm1_lib/areas.py`

 * *Files identical despite different names*

### Comparing `elkm1_lib-2.2.1/elkm1_lib/connection.py` & `elkm1_lib-2.2.2/elkm1_lib/connection.py`

 * *Files identical despite different names*

### Comparing `elkm1_lib-2.2.1/elkm1_lib/const.py` & `elkm1_lib-2.2.2/elkm1_lib/const.py`

 * *Files identical despite different names*

### Comparing `elkm1_lib-2.2.1/elkm1_lib/counters.py` & `elkm1_lib-2.2.2/elkm1_lib/counters.py`

 * *Files identical despite different names*

### Comparing `elkm1_lib-2.2.1/elkm1_lib/discovery.py` & `elkm1_lib-2.2.2/elkm1_lib/discovery.py`

 * *Files identical despite different names*

### Comparing `elkm1_lib-2.2.1/elkm1_lib/elements.py` & `elkm1_lib-2.2.2/elkm1_lib/elements.py`

 * *Files identical despite different names*

### Comparing `elkm1_lib-2.2.1/elkm1_lib/elk.py` & `elkm1_lib-2.2.2/elkm1_lib/elk.py`

 * *Files identical despite different names*

### Comparing `elkm1_lib-2.2.1/elkm1_lib/keypads.py` & `elkm1_lib-2.2.2/elkm1_lib/keypads.py`

 * *Files identical despite different names*

### Comparing `elkm1_lib-2.2.1/elkm1_lib/lights.py` & `elkm1_lib-2.2.2/elkm1_lib/lights.py`

 * *Files identical despite different names*

### Comparing `elkm1_lib-2.2.1/elkm1_lib/message.py` & `elkm1_lib-2.2.2/elkm1_lib/message.py`

 * *Files identical despite different names*

### Comparing `elkm1_lib-2.2.1/elkm1_lib/notify.py` & `elkm1_lib-2.2.2/elkm1_lib/notify.py`

 * *Files identical despite different names*

### Comparing `elkm1_lib-2.2.1/elkm1_lib/outputs.py` & `elkm1_lib-2.2.2/elkm1_lib/outputs.py`

 * *Files identical despite different names*

### Comparing `elkm1_lib-2.2.1/elkm1_lib/panel.py` & `elkm1_lib-2.2.2/elkm1_lib/panel.py`

 * *Files identical despite different names*

### Comparing `elkm1_lib-2.2.1/elkm1_lib/settings.py` & `elkm1_lib-2.2.2/elkm1_lib/settings.py`

 * *Files identical despite different names*

### Comparing `elkm1_lib-2.2.1/elkm1_lib/tasks.py` & `elkm1_lib-2.2.2/elkm1_lib/tasks.py`

 * *Files identical despite different names*

### Comparing `elkm1_lib-2.2.1/elkm1_lib/thermostats.py` & `elkm1_lib-2.2.2/elkm1_lib/thermostats.py`

 * *Files identical despite different names*

### Comparing `elkm1_lib-2.2.1/elkm1_lib/users.py` & `elkm1_lib-2.2.2/elkm1_lib/users.py`

 * *Files identical despite different names*

### Comparing `elkm1_lib-2.2.1/elkm1_lib/util.py` & `elkm1_lib-2.2.2/elkm1_lib/util.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 """Utility functions"""
 
 from __future__ import annotations
 
 import ssl
+from functools import cache
 
 TLS_VERSIONS = {
     # Unfortunately M1XEP does not support auto-negotiation for TLS
     # protocol; the user code must figure out the version to use. The
     # simplest way is to configure using the connection URL (smarter would
     # be to try to connect using each of the version, except SSL lib does
     # not report TLS error, it just closes the connection, so no easy way to
@@ -20,31 +21,44 @@
 
 def url_scheme_is_secure(url: str) -> bool:
     """Check if the URL is one that requires SSL/TLS."""
     scheme, _dest = url.split("://")
     return scheme.startswith("elks")
 
 
+@cache
+def ssl_context_for_scheme(scheme: str) -> ssl.SSLContext:
+    """Create an SSL context for the given scheme.
+
+    Since ssl context is expensive to create, cache it
+    for future use since we only have a few schemes.
+    """
+    ssl_context = ssl.SSLContext(ssl.PROTOCOL_TLS)
+    if tls := TLS_VERSIONS.get(scheme):
+        ssl_context.minimum_version = tls
+        ssl_context.maximum_version = tls
+
+    ssl_context.set_ciphers(
+        "DEFAULT:!aNULL:!eNULL:!MD5:!3DES:!DES:!RC4:!IDEA:!SEED:!aDSS:!SRP:!PSK"
+    )
+    # ssl.OP_LEGACY_SERVER_CONNECT is only available in Python 3.12a4+
+    ssl_context.options |= getattr(ssl, "OP_LEGACY_SERVER_CONNECT", 0x4)
+    return ssl_context
+
+
 def parse_url(url: str) -> tuple[str, str, int, ssl.SSLContext | None]:
     """Parse a Elk connection string"""
     scheme, dest = url.split("://")
     host = None
     ssl_context = None
     if scheme == "elk":
         host, port = dest.split(":") if ":" in dest else (dest, "2101")
     elif TLS_VERSIONS.get(scheme):
         host, port = dest.split(":") if ":" in dest else (dest, "2601")
-        ssl_context = ssl.SSLContext(ssl.PROTOCOL_TLS)
-        if tls := TLS_VERSIONS.get(scheme):
-            ssl_context.minimum_version = tls
-            ssl_context.maximum_version = tls
-
-        ssl_context.set_ciphers(
-            "DEFAULT:!aNULL:!eNULL:!MD5:!3DES:!DES:!RC4:!IDEA:!SEED:!aDSS:!SRP:!PSK"
-        )
+        ssl_context = ssl_context_for_scheme(scheme)
         scheme = "elks"
     elif scheme == "serial":
         host, port = dest.split(":") if ":" in dest else (dest, "115200")
     else:
         raise ValueError(f"Invalid scheme '{scheme}'")
     return (scheme, host, int(port), ssl_context)
```

### Comparing `elkm1_lib-2.2.1/elkm1_lib/zones.py` & `elkm1_lib-2.2.2/elkm1_lib/zones.py`

 * *Files identical despite different names*

### Comparing `elkm1_lib-2.2.1/pyproject.toml` & `elkm1_lib-2.2.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "elkm1-lib"
-version = "2.2.1"
+version = "2.2.2"
 description = "Library for interacting with ElkM1 alarm/automation panel."
 homepage = "https://github.com/gwww/elkm1"
 authors = ["Glenn Waters <gwwaters+elkm1@gmail.com>"]
 readme = "README.md"
 license = "MIT"
 classifiers = [
   'Development Status :: 5 - Production/Stable',
```

### Comparing `elkm1_lib-2.2.1/setup.py` & `elkm1_lib-2.2.2/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,30 +1,256 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: elkm1-lib
+Version: 2.2.2
+Summary: Library for interacting with ElkM1 alarm/automation panel.
+Home-page: https://github.com/gwww/elkm1
+License: MIT
+Author: Glenn Waters
+Author-email: gwwaters+elkm1@gmail.com
+Requires-Python: >=3.9,<4.0
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Intended Audience :: Developers
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: async-timeout (>=4.0,<5.0)
+Requires-Dist: pyserial-asyncio (>=0.5)
+Description-Content-Type: text/markdown
 
-packages = \
-['elkm1_lib']
+# Python ElkM1 library
 
-package_data = \
-{'': ['*']}
+[![PyPI version](https://badge.fury.io/py/elkm1-lib.svg)](https://badge.fury.io/py/elkm1-lib)
+[![CI](https://github.com/gwww/elkm1/actions/workflows/code-quality.yml/badge.svg)](https://github.com/gwww/elkm1/actions/workflows/code-quality.yml)
+[![Downloads](https://pepy.tech/badge/elkm1-lib)](https://pepy.tech/project/elkm1-lib)
+[![License](https://img.shields.io/github/license/mashape/apistatus.svg)](https://pypi.org/project/elkm1_lib/)
 
-install_requires = \
-['async-timeout>=4.0,<5.0', 'pyserial-asyncio>=0.5']
-
-setup_kwargs = {
-    'name': 'elkm1-lib',
-    'version': '2.2.1',
-    'description': 'Library for interacting with ElkM1 alarm/automation panel.',
-    'long_description': '# Python ElkM1 library\n\n[![PyPI version](https://badge.fury.io/py/elkm1-lib.svg)](https://badge.fury.io/py/elkm1-lib)\n[![CI](https://github.com/gwww/elkm1/actions/workflows/code-quality.yml/badge.svg)](https://github.com/gwww/elkm1/actions/workflows/code-quality.yml)\n[![Downloads](https://pepy.tech/badge/elkm1-lib)](https://pepy.tech/project/elkm1-lib)\n[![License](https://img.shields.io/github/license/mashape/apistatus.svg)](https://pypi.org/project/elkm1_lib/)\n\nLibrary for interacting with ElkM1 alarm/automation panel.\n\nhttps://github.com/gwww/elkm1\n\n## Requirements\n\n- Python 3.9 (or higher)\n\n## Description\n\nThis package is created as a library to interact with an ElkM1 alarm/automation\npattern. The motivation to write this was to use with the Home Assistant\nautomation platform. The library can be used for writing other ElkM1 integration\napplications. The IO with the panel is asynchronous over TCP or over the\nserial port.\n\n## Installation\n\n```bash\n    $ pip install elkm1_lib\n```\n\n## Overview\n\nBasic connection to the Elk panel:\n\n```python\n    from elkm1_lib import Elk\n    import logging\n\n    # Print to STDOUT\n    LOG = logging.getLogger(__name__)\n    logging.basicConfig(level=logging.DEBUG, format=\'%(message)s\')\n\n    # Connect to elk\n    elk = Elk({\'url\': \'elk://192.168.1.100\'})\n    elk.connect()\n    elk.run()\n```\n\nThe above will connect to the Elk panel at IP address 192.168.1.100. the `elk://`\nprefix specifies that the connect is plaintext. Alternatively, `elks://` will\nconnect over TLS. In this case a userid and password must be specified\nand the call to `Elk` changes to:\n\n```python\n    elk = Elk(\n        {\'url\': \'elks://192.168.1.100\', \'userid\': \'test\', \'password\': \'pass\'}\n    )\n```\n\nThe following ElkM1 connection protocols are supported:\n- serial:// - Serial port;\n- elk:// - Elk M1XEP Ethernet, non-secure\n- elks:// - Elk M1XEP Ethernet, secure, TLS 1.0\n- elksv1_0:// - Elk M1XEP Ethernet, secure, TLS 1.0, supported on M1XEP version < 2.0.46\n- elksv1_2:// - Elk M1XEP Ethernet, secure, TLS 1.2, supported on M1XEP version = 2.0.46\n- elksv1_3:// - Elk M1XEP Ethernet, secure, TLS 1.2, not yet supported on M1XEP, reserved for future\n\nA username and password are required for any of the secure modes.\n\nTo see working example code take a look at the script `bin/simple`.\n\nThe `Elk` object supports the concept of `Elements`. An `Element`\nis the base class representation of `Zones`, `Lights`, etc. So, for\nexample there is a list of zones: `elk.zones` and each zone can be\naccessed by `elk.zones[index]`. Each element has a `__str__`\nrepresentation so that it is easy to print its contents.\n\nAll `Elements` are referenced starting at 0. Even though the Elk panel\nrefers to, for example, zones 1-208, the library references them\nas zones 0-207. All translation from base 0 to 1 and vice-versa is\nhandled internally in the `elkm1_lib.message` module.\n\nAfter creating the `Elk` object and connecting to the panel the\nlibrary code will synchronize all the elements to the data from the Elk panel.\n\nMany Elk messages are handled by the library, caching their contents. When a\nmessage causes a change to an attribute of an `Element`, registered\ncallbacks are called so that user use of the library can be notified\nof changing elements. The following user code shows registering a callback:\n\n```python\n    def call_me(element, changeset):\n       print(changeset)\n\n    for zone_number in range(Max.ZONES.value):\n      elk.zones[zone_number].add_callback(call_me)\n```\n\nThe library encodes, decodes, and processes messages to/from the\nElk panel. All the encoding and decoding is done in `elkm1_lib.message` module.\n\nMessages received are handled with callbacks. The library\ninternally registers callbacks so that decoded messages\ncan be used to update an `Element`. The user of the\nlibrary may also register callbacks. Any particular message\nmay have multiple callbacks.\n\nWhen the message is received it is decoded\nand some validation is done. The message handler is called\nwith the fields of from the decoded message. Each type of\nmessage has parameters that match the message type. All handler parameters\nare named parameters.\n\nHere is an example of a message handler being registered and how it is called:\n\n```python\n    def zone_status_change_handler(zone_number, zone_status):\n      print(zone_number, zone_status)\n\n    elk.add_handler(\'ZC\', zone_status_change_handler)\n```\n\nThe above code registers a callback for \'ZC\' (Elk zone status change)\nmessages. When a ZC message is received the handler functions are called\nwith the zone_number and zone_status.\n\nThere are a number of pseudo-handlers that act like the handlers. These are\ncalled when events happen. The pseudo-handlers are:\n\n- `connect`: When a successful connection to the ElkM1 is completed.\n- `disconnect`: When a connection to a panel is disconnected.\n- `login`: When a login is made to the panel (using `elks://` connection mode.\n  A single boolean parameter is passed `succeeded`.\n- `sync_complete`: When the panel has completed synchonizing all its elements.\n- `timeout`: When a send of a message to the ElkM1 times out (fails to send).\n- `unknown`: When a message from the ElkM1 is received and the library does\n  not have a method to decode the message. The message is passed to this handler\n  and can be decoded outside of the library.\n\n## Utilities\n\nThe `bin` directory of the library has one utility program and\na couple of example uses of the library.\n\n### `mkdoc`\n\nThe utility `mkdoc` creates a Markdown table of the list of Elk\nmessages with a check mark for those messages have encoders/decoders\nand an X for those messages are not planned to be implemented.\nThere are no parameters to `mkdoc`. It outputs to stdout.\nThe data for the report comes from the ElkM1 library code mostly.\nA couple of things are hard coded in the mkdoc script, notably\nthe "no plans to implement" list.\n\n### `simple`\n\nThe `simple` Python script is a trivial use of the ElkM1 library.\nIt connects to the panel, syncs to internal memory, and continues\nlistening for any messages from the panel. The URL of the ElkM1 to\nconnect to is retrieved from an environment variable named `ELKM1_URL`.\n\n### `elk`\n\nThe `elk` Python script is a bit of a command interpretor. It can run in\ntwo modes. Non-interactive mode is the default. Just run the `elk` command.\nThe non-interactive mode is similar to `simple` except there are a\ncouple of message handlers (`timeout` and `unknown` handlers).\n\nThe `elk` can also be run in interactive mode by invoking it by\n`elk -i`. In this mode is uses curses (full screen use of the terminal)\nthat has a command line and an output window. `TAB` switches between\nthe command line and output windows. In the output window the arrow keys\nand scrollwheel scroll the contents of the window.\n\nIn the command line when running `elk -i` there are a\nnumber of commands. Start with `help`. Then `help <command>` for\ndetails on each command. In general there are commands to dump the internal\nstate of elements and to invoke any of the encoders to send a message\nto the Elk panel.\n\nFor example, `light <4, 8, 12-14` would invoke the `__str__` method\nfor the light element to print the cached info for lights 0-3, 8, and 12-14.\n\nAnother example would be `pf 3` which issues the pf (Turn light off)\ncommand for light number 3 (light 4 on the panel -- remember 0\nversus 1 base).\n\nAll of the commands that send messages to the panel are automatically\ndiscovered and are all the XX_encode functions in the ``elkm1_lib.message``\nmodule. The docstring and the XX_encode\'s parameters are shown as part\nof the help.\n\n## Development\n\nThis project uses [poetry](https://poetry.eustace.io/) for development dependencies. Installation instructions are on their website.\n\nTo get started developing:\n\n```\ngit clone https://github.com/gwww/elkm1.git\ncd elkm1\npoetry install\npoetry shell # Or activate the created virtual environment\nmake test # to ensure everything installed properly\n```\n\nThere is a `Makefile` in the root directory as well. The `make` command\nfollowed by one of the targets in the `Makefile` can be used. If you don\'t\nhave or wish to use `make` the `Makefile` serves as examples of common\ncommands that can be run.\n\n## Reporting a Bug\n\nNo problem ;) — report the bugs! But, logs are most often required. If you\nare using Home Assistant, which is about the only use I\'m aware of for\nthis library, then add the following to your `configuration.yaml`:\n```\nlogger:\n  default: info\n  logs:\n    custom_components.elkm1: debug\n    elkm1_lib: debug\n```\n\nDo everything in your power to trim to logs down to their smallest. One way is\nto reproduce your problem quickly so that few other logs are not generated in\nbetween. Another recommendation is to use the simplest configuration that you\ncan think of to reproduce the problem.\n\nCan you reproduce the problem in other ways? If this is a problem that is\nbeing experienced while using Home Assistant try using the `Services` in `Developer Tools`.\n\nSometime logs may have sensitive information in them. You may want to\nscan your logs for that info and "X" it out. In addition, you can send logs\ndirectly to me. Support email is in the `pyproject.toml` file. You may also\nsend a link to somewhere you\'ve stored/shared the file (DropBox for example).\n',
-    'author': 'Glenn Waters',
-    'author_email': 'gwwaters+elkm1@gmail.com',
-    'maintainer': 'None',
-    'maintainer_email': 'None',
-    'url': 'https://github.com/gwww/elkm1',
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'python_requires': '>=3.9,<4.0',
-}
+Library for interacting with ElkM1 alarm/automation panel.
 
+https://github.com/gwww/elkm1
+
+## Requirements
+
+- Python 3.9 (or higher)
+
+## Description
+
+This package is created as a library to interact with an ElkM1 alarm/automation
+pattern. The motivation to write this was to use with the Home Assistant
+automation platform. The library can be used for writing other ElkM1 integration
+applications. The IO with the panel is asynchronous over TCP or over the
+serial port.
+
+## Installation
+
+```bash
+    $ pip install elkm1_lib
+```
+
+## Overview
+
+Basic connection to the Elk panel:
+
+```python
+    from elkm1_lib import Elk
+    import logging
+
+    # Print to STDOUT
+    LOG = logging.getLogger(__name__)
+    logging.basicConfig(level=logging.DEBUG, format='%(message)s')
+
+    # Connect to elk
+    elk = Elk({'url': 'elk://192.168.1.100'})
+    elk.connect()
+    elk.run()
+```
+
+The above will connect to the Elk panel at IP address 192.168.1.100. the `elk://`
+prefix specifies that the connect is plaintext. Alternatively, `elks://` will
+connect over TLS. In this case a userid and password must be specified
+and the call to `Elk` changes to:
+
+```python
+    elk = Elk(
+        {'url': 'elks://192.168.1.100', 'userid': 'test', 'password': 'pass'}
+    )
+```
+
+The following ElkM1 connection protocols are supported:
+- serial:// - Serial port;
+- elk:// - Elk M1XEP Ethernet, non-secure
+- elks:// - Elk M1XEP Ethernet, secure, TLS 1.0
+- elksv1_0:// - Elk M1XEP Ethernet, secure, TLS 1.0, supported on M1XEP version < 2.0.46
+- elksv1_2:// - Elk M1XEP Ethernet, secure, TLS 1.2, supported on M1XEP version = 2.0.46
+- elksv1_3:// - Elk M1XEP Ethernet, secure, TLS 1.2, not yet supported on M1XEP, reserved for future
+
+A username and password are required for any of the secure modes.
+
+To see working example code take a look at the script `bin/simple`.
+
+The `Elk` object supports the concept of `Elements`. An `Element`
+is the base class representation of `Zones`, `Lights`, etc. So, for
+example there is a list of zones: `elk.zones` and each zone can be
+accessed by `elk.zones[index]`. Each element has a `__str__`
+representation so that it is easy to print its contents.
+
+All `Elements` are referenced starting at 0. Even though the Elk panel
+refers to, for example, zones 1-208, the library references them
+as zones 0-207. All translation from base 0 to 1 and vice-versa is
+handled internally in the `elkm1_lib.message` module.
+
+After creating the `Elk` object and connecting to the panel the
+library code will synchronize all the elements to the data from the Elk panel.
+
+Many Elk messages are handled by the library, caching their contents. When a
+message causes a change to an attribute of an `Element`, registered
+callbacks are called so that user use of the library can be notified
+of changing elements. The following user code shows registering a callback:
+
+```python
+    def call_me(element, changeset):
+       print(changeset)
+
+    for zone_number in range(Max.ZONES.value):
+      elk.zones[zone_number].add_callback(call_me)
+```
+
+The library encodes, decodes, and processes messages to/from the
+Elk panel. All the encoding and decoding is done in `elkm1_lib.message` module.
+
+Messages received are handled with callbacks. The library
+internally registers callbacks so that decoded messages
+can be used to update an `Element`. The user of the
+library may also register callbacks. Any particular message
+may have multiple callbacks.
+
+When the message is received it is decoded
+and some validation is done. The message handler is called
+with the fields of from the decoded message. Each type of
+message has parameters that match the message type. All handler parameters
+are named parameters.
+
+Here is an example of a message handler being registered and how it is called:
+
+```python
+    def zone_status_change_handler(zone_number, zone_status):
+      print(zone_number, zone_status)
+
+    elk.add_handler('ZC', zone_status_change_handler)
+```
+
+The above code registers a callback for 'ZC' (Elk zone status change)
+messages. When a ZC message is received the handler functions are called
+with the zone_number and zone_status.
+
+There are a number of pseudo-handlers that act like the handlers. These are
+called when events happen. The pseudo-handlers are:
+
+- `connect`: When a successful connection to the ElkM1 is completed.
+- `disconnect`: When a connection to a panel is disconnected.
+- `login`: When a login is made to the panel (using `elks://` connection mode.
+  A single boolean parameter is passed `succeeded`.
+- `sync_complete`: When the panel has completed synchonizing all its elements.
+- `timeout`: When a send of a message to the ElkM1 times out (fails to send).
+- `unknown`: When a message from the ElkM1 is received and the library does
+  not have a method to decode the message. The message is passed to this handler
+  and can be decoded outside of the library.
+
+## Utilities
+
+The `bin` directory of the library has one utility program and
+a couple of example uses of the library.
+
+### `mkdoc`
+
+The utility `mkdoc` creates a Markdown table of the list of Elk
+messages with a check mark for those messages have encoders/decoders
+and an X for those messages are not planned to be implemented.
+There are no parameters to `mkdoc`. It outputs to stdout.
+The data for the report comes from the ElkM1 library code mostly.
+A couple of things are hard coded in the mkdoc script, notably
+the "no plans to implement" list.
+
+### `simple`
+
+The `simple` Python script is a trivial use of the ElkM1 library.
+It connects to the panel, syncs to internal memory, and continues
+listening for any messages from the panel. The URL of the ElkM1 to
+connect to is retrieved from an environment variable named `ELKM1_URL`.
+
+### `elk`
+
+The `elk` Python script is a bit of a command interpretor. It can run in
+two modes. Non-interactive mode is the default. Just run the `elk` command.
+The non-interactive mode is similar to `simple` except there are a
+couple of message handlers (`timeout` and `unknown` handlers).
+
+The `elk` can also be run in interactive mode by invoking it by
+`elk -i`. In this mode is uses curses (full screen use of the terminal)
+that has a command line and an output window. `TAB` switches between
+the command line and output windows. In the output window the arrow keys
+and scrollwheel scroll the contents of the window.
+
+In the command line when running `elk -i` there are a
+number of commands. Start with `help`. Then `help <command>` for
+details on each command. In general there are commands to dump the internal
+state of elements and to invoke any of the encoders to send a message
+to the Elk panel.
+
+For example, `light <4, 8, 12-14` would invoke the `__str__` method
+for the light element to print the cached info for lights 0-3, 8, and 12-14.
+
+Another example would be `pf 3` which issues the pf (Turn light off)
+command for light number 3 (light 4 on the panel -- remember 0
+versus 1 base).
+
+All of the commands that send messages to the panel are automatically
+discovered and are all the XX_encode functions in the ``elkm1_lib.message``
+module. The docstring and the XX_encode's parameters are shown as part
+of the help.
+
+## Development
+
+This project uses [poetry](https://poetry.eustace.io/) for development dependencies. Installation instructions are on their website.
+
+To get started developing:
+
+```
+git clone https://github.com/gwww/elkm1.git
+cd elkm1
+poetry install
+poetry shell # Or activate the created virtual environment
+make test # to ensure everything installed properly
+```
+
+There is a `Makefile` in the root directory as well. The `make` command
+followed by one of the targets in the `Makefile` can be used. If you don't
+have or wish to use `make` the `Makefile` serves as examples of common
+commands that can be run.
+
+## Reporting a Bug
+
+No problem ;) — report the bugs! But, logs are most often required. If you
+are using Home Assistant, which is about the only use I'm aware of for
+this library, then add the following to your `configuration.yaml`:
+```
+logger:
+  default: info
+  logs:
+    custom_components.elkm1: debug
+    elkm1_lib: debug
+```
+
+Do everything in your power to trim to logs down to their smallest. One way is
+to reproduce your problem quickly so that few other logs are not generated in
+between. Another recommendation is to use the simplest configuration that you
+can think of to reproduce the problem.
+
+Can you reproduce the problem in other ways? If this is a problem that is
+being experienced while using Home Assistant try using the `Services` in `Developer Tools`.
+
+Sometime logs may have sensitive information in them. You may want to
+scan your logs for that info and "X" it out. In addition, you can send logs
+directly to me. Support email is in the `pyproject.toml` file. You may also
+send a link to somewhere you've stored/shared the file (DropBox for example).
 
-setup(**setup_kwargs)
```

