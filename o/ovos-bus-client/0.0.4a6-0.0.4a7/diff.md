# Comparing `tmp/ovos-bus-client-0.0.4a6.tar.gz` & `tmp/ovos-bus-client-0.0.4a7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ovos-bus-client-0.0.4a6.tar", last modified: Sun Apr 30 23:24:31 2023, max compression
+gzip compressed data, was "ovos-bus-client-0.0.4a7.tar", last modified: Fri May  5 20:13:04 2023, max compression
```

## Comparing `ovos-bus-client-0.0.4a6.tar` & `ovos-bus-client-0.0.4a7.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 23:24:31.598416 ovos-bus-client-0.0.4a6/
--rw-r--r--   0 runner    (1001) docker     (123)    11733 2023-04-30 23:24:31.000000 ovos-bus-client-0.0.4a6/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-04-30 23:24:31.000000 ovos-bus-client-0.0.4a6/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      628 2023-04-30 23:24:31.598416 ovos-bus-client-0.0.4a6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      273 2023-04-30 23:24:31.000000 ovos-bus-client-0.0.4a6/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 23:24:31.598416 ovos-bus-client-0.0.4a6/ovos_bus_client/
--rw-r--r--   0 runner    (1001) docker     (123)     1254 2023-04-30 23:24:31.000000 ovos-bus-client-0.0.4a6/ovos_bus_client/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 23:24:31.598416 ovos-bus-client-0.0.4a6/ovos_bus_client/client/
--rw-r--r--   0 runner    (1001) docker     (123)      648 2023-04-30 23:24:31.000000 ovos-bus-client-0.0.4a6/ovos_bus_client/client/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    15330 2023-04-30 23:24:31.000000 ovos-bus-client-0.0.4a6/ovos_bus_client/client/client.py
--rw-r--r--   0 runner    (1001) docker     (123)     6720 2023-04-30 23:24:31.000000 ovos-bus-client-0.0.4a6/ovos_bus_client/client/collector.py
--rw-r--r--   0 runner    (1001) docker     (123)     2459 2023-04-30 23:24:31.000000 ovos-bus-client-0.0.4a6/ovos_bus_client/client/waiter.py
--rw-r--r--   0 runner    (1001) docker     (123)     3463 2023-04-30 23:24:31.000000 ovos-bus-client-0.0.4a6/ovos_bus_client/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)    16171 2023-04-30 23:24:31.000000 ovos-bus-client-0.0.4a6/ovos_bus_client/message.py
--rw-r--r--   0 runner    (1001) docker     (123)     1305 2023-04-30 23:24:31.000000 ovos-bus-client-0.0.4a6/ovos_bus_client/scripts.py
--rw-r--r--   0 runner    (1001) docker     (123)      950 2023-04-30 23:24:31.000000 ovos-bus-client-0.0.4a6/ovos_bus_client/send_func.py
--rw-r--r--   0 runner    (1001) docker     (123)    15471 2023-04-30 23:24:31.000000 ovos-bus-client-0.0.4a6/ovos_bus_client/session.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 23:24:31.598416 ovos-bus-client-0.0.4a6/ovos_bus_client/util/
--rw-r--r--   0 runner    (1001) docker     (123)     1292 2023-04-30 23:24:31.000000 ovos-bus-client-0.0.4a6/ovos_bus_client/util/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    22884 2023-04-30 23:24:31.000000 ovos-bus-client-0.0.4a6/ovos_bus_client/util/scheduler.py
--rw-r--r--   0 runner    (1001) docker     (123)     1441 2023-04-30 23:24:31.000000 ovos-bus-client-0.0.4a6/ovos_bus_client/util/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      114 2023-04-30 23:24:31.000000 ovos-bus-client-0.0.4a6/ovos_bus_client/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-30 23:24:31.598416 ovos-bus-client-0.0.4a6/ovos_bus_client.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      628 2023-04-30 23:24:31.000000 ovos-bus-client-0.0.4a6/ovos_bus_client.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      717 2023-04-30 23:24:31.000000 ovos-bus-client-0.0.4a6/ovos_bus_client.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-30 23:24:31.000000 ovos-bus-client-0.0.4a6/ovos_bus_client.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      167 2023-04-30 23:24:31.000000 ovos-bus-client-0.0.4a6/ovos_bus_client.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-04-30 23:24:31.000000 ovos-bus-client-0.0.4a6/ovos_bus_client.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-04-30 23:24:31.000000 ovos-bus-client-0.0.4a6/ovos_bus_client.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-04-30 23:24:31.000000 ovos-bus-client-0.0.4a6/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-30 23:24:31.598416 ovos-bus-client-0.0.4a6/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2677 2023-04-30 23:24:31.000000 ovos-bus-client-0.0.4a6/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 20:13:04.392304 ovos-bus-client-0.0.4a7/
+-rw-r--r--   0 runner    (1001) docker     (123)    11733 2023-05-05 20:13:03.000000 ovos-bus-client-0.0.4a7/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-05-05 20:13:03.000000 ovos-bus-client-0.0.4a7/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      628 2023-05-05 20:13:04.392304 ovos-bus-client-0.0.4a7/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      273 2023-05-05 20:13:03.000000 ovos-bus-client-0.0.4a7/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 20:13:04.388304 ovos-bus-client-0.0.4a7/ovos_bus_client/
+-rw-r--r--   0 runner    (1001) docker     (123)     1254 2023-05-05 20:13:03.000000 ovos-bus-client-0.0.4a7/ovos_bus_client/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 20:13:04.392304 ovos-bus-client-0.0.4a7/ovos_bus_client/client/
+-rw-r--r--   0 runner    (1001) docker     (123)      648 2023-05-05 20:13:03.000000 ovos-bus-client-0.0.4a7/ovos_bus_client/client/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15330 2023-05-05 20:13:03.000000 ovos-bus-client-0.0.4a7/ovos_bus_client/client/client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6720 2023-05-05 20:13:03.000000 ovos-bus-client-0.0.4a7/ovos_bus_client/client/collector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2459 2023-05-05 20:13:03.000000 ovos-bus-client-0.0.4a7/ovos_bus_client/client/waiter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3463 2023-05-05 20:13:03.000000 ovos-bus-client-0.0.4a7/ovos_bus_client/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16253 2023-05-05 20:13:03.000000 ovos-bus-client-0.0.4a7/ovos_bus_client/message.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1305 2023-05-05 20:13:03.000000 ovos-bus-client-0.0.4a7/ovos_bus_client/scripts.py
+-rw-r--r--   0 runner    (1001) docker     (123)      950 2023-05-05 20:13:03.000000 ovos-bus-client-0.0.4a7/ovos_bus_client/send_func.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15538 2023-05-05 20:13:03.000000 ovos-bus-client-0.0.4a7/ovos_bus_client/session.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 20:13:04.392304 ovos-bus-client-0.0.4a7/ovos_bus_client/util/
+-rw-r--r--   0 runner    (1001) docker     (123)     1292 2023-05-05 20:13:03.000000 ovos-bus-client-0.0.4a7/ovos_bus_client/util/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22884 2023-05-05 20:13:03.000000 ovos-bus-client-0.0.4a7/ovos_bus_client/util/scheduler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1441 2023-05-05 20:13:03.000000 ovos-bus-client-0.0.4a7/ovos_bus_client/util/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-05-05 20:13:03.000000 ovos-bus-client-0.0.4a7/ovos_bus_client/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 20:13:04.388304 ovos-bus-client-0.0.4a7/ovos_bus_client.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      628 2023-05-05 20:13:04.000000 ovos-bus-client-0.0.4a7/ovos_bus_client.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      717 2023-05-05 20:13:04.000000 ovos-bus-client-0.0.4a7/ovos_bus_client.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 20:13:04.000000 ovos-bus-client-0.0.4a7/ovos_bus_client.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      167 2023-05-05 20:13:04.000000 ovos-bus-client-0.0.4a7/ovos_bus_client.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-05 20:13:04.000000 ovos-bus-client-0.0.4a7/ovos_bus_client.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-05 20:13:04.000000 ovos-bus-client-0.0.4a7/ovos_bus_client.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      106 2023-05-05 20:13:03.000000 ovos-bus-client-0.0.4a7/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-05 20:13:04.392304 ovos-bus-client-0.0.4a7/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2677 2023-05-05 20:13:03.000000 ovos-bus-client-0.0.4a7/setup.py
```

### Comparing `ovos-bus-client-0.0.4a6/LICENSE.md` & `ovos-bus-client-0.0.4a7/LICENSE.md`

 * *Files identical despite different names*

### Comparing `ovos-bus-client-0.0.4a6/PKG-INFO` & `ovos-bus-client-0.0.4a7/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ovos-bus-client
-Version: 0.0.4a6
+Version: 0.0.4a7
 Summary: OVOS Messagebus Client
 Home-page: https://github.com/OpenVoiceOS/ovos-bus-client
 Author: JarbasAI
 Author-email: jarbasai@mailfence.com
 License: Apache-2.0
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
```

### Comparing `ovos-bus-client-0.0.4a6/ovos_bus_client/__init__.py` & `ovos-bus-client-0.0.4a7/ovos_bus_client/__init__.py`

 * *Files identical despite different names*

### Comparing `ovos-bus-client-0.0.4a6/ovos_bus_client/client/__init__.py` & `ovos-bus-client-0.0.4a7/ovos_bus_client/client/__init__.py`

 * *Files identical despite different names*

### Comparing `ovos-bus-client-0.0.4a6/ovos_bus_client/client/client.py` & `ovos-bus-client-0.0.4a7/ovos_bus_client/client/client.py`

 * *Files identical despite different names*

### Comparing `ovos-bus-client-0.0.4a6/ovos_bus_client/client/collector.py` & `ovos-bus-client-0.0.4a7/ovos_bus_client/client/collector.py`

 * *Files identical despite different names*

### Comparing `ovos-bus-client-0.0.4a6/ovos_bus_client/client/waiter.py` & `ovos-bus-client-0.0.4a7/ovos_bus_client/client/waiter.py`

 * *Files identical despite different names*

### Comparing `ovos-bus-client-0.0.4a6/ovos_bus_client/conf.py` & `ovos-bus-client-0.0.4a7/ovos_bus_client/conf.py`

 * *Files identical despite different names*

### Comparing `ovos-bus-client-0.0.4a6/ovos_bus_client/message.py` & `ovos-bus-client-0.0.4a7/ovos_bus_client/message.py`

 * *Files 1% similar despite different names*

```diff
@@ -121,14 +121,18 @@
 
         msg = json.dumps({'type': self.msg_type, 'data': data, 'context': ctxt})
         if self._secret_key:
             payload = encrypt_as_dict(msg)
             return json.dumps(payload)
         return msg
 
+    @property
+    def as_dict(self):
+        return json.loads(self.serialize())
+
     @staticmethod
     def _json_dump(value):
         def serialize_item(x):
             try:
                 if hasattr(x, "serialize"):
                     return x.serialize()
             except:
```

### Comparing `ovos-bus-client-0.0.4a6/ovos_bus_client/scripts.py` & `ovos-bus-client-0.0.4a7/ovos_bus_client/scripts.py`

 * *Files identical despite different names*

### Comparing `ovos-bus-client-0.0.4a6/ovos_bus_client/send_func.py` & `ovos-bus-client-0.0.4a7/ovos_bus_client/send_func.py`

 * *Files identical despite different names*

### Comparing `ovos-bus-client-0.0.4a6/ovos_bus_client/session.py` & `ovos-bus-client-0.0.4a7/ovos_bus_client/session.py`

 * *Files 0% similar despite different names*

```diff
@@ -107,15 +107,17 @@
             "lang": self.lang,
             "context": self.context.serialize()
         }
 
     def update_history(self, message=None):
         message = message or dig_for_message()
         if message:
-            self.history.append((message.serialize(), time.time()))
+            m = message.as_dict
+            m["context"] = {}  # clear personal data
+            self.history.append((m, time.time()))
         self._prune_history()
 
     @staticmethod
     def deserialize(data):
         uid = data.get("session_id")
         active = data.get("active_skills") or []
         history = data.get("history") or []
```

### Comparing `ovos-bus-client-0.0.4a6/ovos_bus_client/util/__init__.py` & `ovos-bus-client-0.0.4a7/ovos_bus_client/util/__init__.py`

 * *Files identical despite different names*

### Comparing `ovos-bus-client-0.0.4a6/ovos_bus_client/util/scheduler.py` & `ovos-bus-client-0.0.4a7/ovos_bus_client/util/scheduler.py`

 * *Files identical despite different names*

### Comparing `ovos-bus-client-0.0.4a6/ovos_bus_client/util/utils.py` & `ovos-bus-client-0.0.4a7/ovos_bus_client/util/utils.py`

 * *Files identical despite different names*

### Comparing `ovos-bus-client-0.0.4a6/ovos_bus_client.egg-info/PKG-INFO` & `ovos-bus-client-0.0.4a7/ovos_bus_client.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ovos-bus-client
-Version: 0.0.4a6
+Version: 0.0.4a7
 Summary: OVOS Messagebus Client
 Home-page: https://github.com/OpenVoiceOS/ovos-bus-client
 Author: JarbasAI
 Author-email: jarbasai@mailfence.com
 License: Apache-2.0
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
```

### Comparing `ovos-bus-client-0.0.4a6/ovos_bus_client.egg-info/SOURCES.txt` & `ovos-bus-client-0.0.4a7/ovos_bus_client.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ovos-bus-client-0.0.4a6/setup.py` & `ovos-bus-client-0.0.4a7/setup.py`

 * *Files identical despite different names*

