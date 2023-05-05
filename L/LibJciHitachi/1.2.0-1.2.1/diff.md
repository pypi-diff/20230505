# Comparing `tmp/LibJciHitachi-1.2.0.tar.gz` & `tmp/LibJciHitachi-1.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "LibJciHitachi-1.2.0.tar", last modified: Tue May  2 14:49:10 2023, max compression
+gzip compressed data, was "LibJciHitachi-1.2.1.tar", last modified: Fri May  5 07:22:10 2023, max compression
```

## Comparing `LibJciHitachi-1.2.0.tar` & `LibJciHitachi-1.2.1.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 14:49:10.580887 LibJciHitachi-1.2.0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 14:49:10.576887 LibJciHitachi-1.2.0/JciHitachi/
--rw-r--r--   0 runner    (1001) docker     (123)       46 2023-05-02 14:48:53.000000 LibJciHitachi-1.2.0/JciHitachi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    40925 2023-05-02 14:48:53.000000 LibJciHitachi-1.2.0/JciHitachi/api.py
--rw-r--r--   0 runner    (1001) docker     (123)    35735 2023-05-02 14:48:53.000000 LibJciHitachi-1.2.0/JciHitachi/aws_connection.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 14:49:10.576887 LibJciHitachi-1.2.0/JciHitachi/cert/
--rw-r--r--   0 runner    (1001) docker     (123)     1188 2023-05-02 14:48:53.000000 LibJciHitachi-1.2.0/JciHitachi/cert/AmazonRootCA1.pem
--rw-r--r--   0 runner    (1001) docker     (123)     2116 2023-05-02 14:48:53.000000 LibJciHitachi-1.2.0/JciHitachi/cert/api-jci-hitachi-smarthome-com-chain.pem
--rw-r--r--   0 runner    (1001) docker     (123)     2124 2023-05-02 14:48:53.000000 LibJciHitachi-1.2.0/JciHitachi/cert/mqtt-jci-hitachi-smarthome-com-chain.pem
--rw-r--r--   0 runner    (1001) docker     (123)    11973 2023-05-02 14:48:53.000000 LibJciHitachi-1.2.0/JciHitachi/connection.py
--rw-r--r--   0 runner    (1001) docker     (123)    56244 2023-05-02 14:48:53.000000 LibJciHitachi-1.2.0/JciHitachi/model.py
--rw-r--r--   0 runner    (1001) docker     (123)     4309 2023-05-02 14:48:53.000000 LibJciHitachi-1.2.0/JciHitachi/mqtt_connection.py
--rw-r--r--   0 runner    (1001) docker     (123)     8418 2023-05-02 14:48:53.000000 LibJciHitachi-1.2.0/JciHitachi/status.py
--rw-r--r--   0 runner    (1001) docker     (123)     2906 2023-05-02 14:48:53.000000 LibJciHitachi-1.2.0/JciHitachi/utility.py
--rw-r--r--   0 runner    (1001) docker     (123)    11337 2023-05-02 14:48:53.000000 LibJciHitachi-1.2.0/LICENSE
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 14:49:10.576887 LibJciHitachi-1.2.0/LibJciHitachi.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3966 2023-05-02 14:49:10.000000 LibJciHitachi-1.2.0/LibJciHitachi.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      680 2023-05-02 14:49:10.000000 LibJciHitachi-1.2.0/LibJciHitachi.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-02 14:49:10.000000 LibJciHitachi-1.2.0/LibJciHitachi.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       34 2023-05-02 14:49:10.000000 LibJciHitachi-1.2.0/LibJciHitachi.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-02 14:49:10.000000 LibJciHitachi-1.2.0/LibJciHitachi.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3966 2023-05-02 14:49:10.580887 LibJciHitachi-1.2.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3203 2023-05-02 14:48:53.000000 LibJciHitachi-1.2.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-02 14:49:10.580887 LibJciHitachi-1.2.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1530 2023-05-02 14:48:53.000000 LibJciHitachi-1.2.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 14:49:10.580887 LibJciHitachi-1.2.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)    17566 2023-05-02 14:48:53.000000 LibJciHitachi-1.2.0/tests/test_api.py
--rw-r--r--   0 runner    (1001) docker     (123)    18884 2023-05-02 14:48:53.000000 LibJciHitachi-1.2.0/tests/test_aws_connection.py
--rw-r--r--   0 runner    (1001) docker     (123)     6364 2023-05-02 14:48:53.000000 LibJciHitachi-1.2.0/tests/test_integration.py
--rw-r--r--   0 runner    (1001) docker     (123)     9204 2023-05-02 14:48:53.000000 LibJciHitachi-1.2.0/tests/test_model.py
--rw-r--r--   0 runner    (1001) docker     (123)     1121 2023-05-02 14:48:53.000000 LibJciHitachi-1.2.0/tests/test_sanity.py
--rw-r--r--   0 runner    (1001) docker     (123)     6949 2023-05-02 14:48:53.000000 LibJciHitachi-1.2.0/tests/test_status.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 07:22:10.159077 LibJciHitachi-1.2.1/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 07:22:10.159077 LibJciHitachi-1.2.1/JciHitachi/
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-05-05 07:21:58.000000 LibJciHitachi-1.2.1/JciHitachi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40925 2023-05-05 07:21:58.000000 LibJciHitachi-1.2.1/JciHitachi/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    35711 2023-05-05 07:21:58.000000 LibJciHitachi-1.2.1/JciHitachi/aws_connection.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 07:22:10.159077 LibJciHitachi-1.2.1/JciHitachi/cert/
+-rw-r--r--   0 runner    (1001) docker     (123)     1188 2023-05-05 07:21:58.000000 LibJciHitachi-1.2.1/JciHitachi/cert/AmazonRootCA1.pem
+-rw-r--r--   0 runner    (1001) docker     (123)     2116 2023-05-05 07:21:58.000000 LibJciHitachi-1.2.1/JciHitachi/cert/api-jci-hitachi-smarthome-com-chain.pem
+-rw-r--r--   0 runner    (1001) docker     (123)     2124 2023-05-05 07:21:58.000000 LibJciHitachi-1.2.1/JciHitachi/cert/mqtt-jci-hitachi-smarthome-com-chain.pem
+-rw-r--r--   0 runner    (1001) docker     (123)    11973 2023-05-05 07:21:58.000000 LibJciHitachi-1.2.1/JciHitachi/connection.py
+-rw-r--r--   0 runner    (1001) docker     (123)    56244 2023-05-05 07:21:58.000000 LibJciHitachi-1.2.1/JciHitachi/model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4309 2023-05-05 07:21:58.000000 LibJciHitachi-1.2.1/JciHitachi/mqtt_connection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8418 2023-05-05 07:21:58.000000 LibJciHitachi-1.2.1/JciHitachi/status.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3802 2023-05-05 07:21:58.000000 LibJciHitachi-1.2.1/JciHitachi/utility.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11337 2023-05-05 07:21:58.000000 LibJciHitachi-1.2.1/LICENSE
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 07:22:10.159077 LibJciHitachi-1.2.1/LibJciHitachi.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3966 2023-05-05 07:22:10.000000 LibJciHitachi-1.2.1/LibJciHitachi.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      680 2023-05-05 07:22:10.000000 LibJciHitachi-1.2.1/LibJciHitachi.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 07:22:10.000000 LibJciHitachi-1.2.1/LibJciHitachi.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       34 2023-05-05 07:22:10.000000 LibJciHitachi-1.2.1/LibJciHitachi.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-05 07:22:10.000000 LibJciHitachi-1.2.1/LibJciHitachi.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3966 2023-05-05 07:22:10.159077 LibJciHitachi-1.2.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3203 2023-05-05 07:21:58.000000 LibJciHitachi-1.2.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-05 07:22:10.159077 LibJciHitachi-1.2.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1530 2023-05-05 07:21:58.000000 LibJciHitachi-1.2.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 07:22:10.159077 LibJciHitachi-1.2.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)    17566 2023-05-05 07:21:58.000000 LibJciHitachi-1.2.1/tests/test_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18884 2023-05-05 07:21:58.000000 LibJciHitachi-1.2.1/tests/test_aws_connection.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6364 2023-05-05 07:21:58.000000 LibJciHitachi-1.2.1/tests/test_integration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9204 2023-05-05 07:21:58.000000 LibJciHitachi-1.2.1/tests/test_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1121 2023-05-05 07:21:58.000000 LibJciHitachi-1.2.1/tests/test_sanity.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6949 2023-05-05 07:21:58.000000 LibJciHitachi-1.2.1/tests/test_status.py
```

### Comparing `LibJciHitachi-1.2.0/JciHitachi/api.py` & `LibJciHitachi-1.2.1/JciHitachi/api.py`

 * *Files identical despite different names*

### Comparing `LibJciHitachi-1.2.0/JciHitachi/aws_connection.py` & `LibJciHitachi-1.2.1/JciHitachi/aws_connection.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 from typing import Callable, Optional, Union
 
 import awscrt
 import httpx
 from awsiot import iotshadow, mqtt_connection_builder
 
 from .model import JciHitachiAWSStatus, JciHitachiAWSStatusSupport
+from .utility import to_thread
 
 AWS_REGION = "ap-northeast-1"
 AWS_COGNITO_IDP_ENDPOINT = f"cognito-idp.{AWS_REGION}.amazonaws.com"
 AWS_COGNITO_ENDPOINT = f"cognito-identity.{AWS_REGION}.amazonaws.com"
 AWS_COGNITO_CLIENT_ID = "7kfnjsb66ei1qt5s5gjv6j1lp6"
 AWS_COGNITO_USERPOOL_ID = f"{AWS_REGION}_aTZeaievK"
 
@@ -621,15 +622,15 @@
 
             resubscribe_future.add_done_callback(on_resubscribe_complete)
             _LOGGER.info("Resubscribed successfully.")
         return
     
     async def _wrap_async(self, identifier: str, fn: Callable, timeout: float) -> str:
         await asyncio.sleep(random() / 2)  # randomly wait 0~0.5 seconds to prevent messages flooding to the broker.
-        await asyncio.wait_for(fn(), timeout)
+        await asyncio.wait_for(to_thread(fn), timeout)
         return identifier
 
     def disconnect(self) -> None:
         """Disconnect from the MQTT broker.
         """
 
         if self._mqttc is not None:
@@ -755,42 +756,42 @@
         if publish_type == "support":
             support_topic = f"{host_identity_id}/{thing_name}/registration/request"
             if thing_name in self._mqtt_events.device_support_event:
                 self._mqtt_events.device_support_event[thing_name].clear()
             else:
                 self._mqtt_events.device_support_event[thing_name] = threading.Event()
                 
-            async def wrapper():
+            def fn():
                 publish_future, _ = self._mqttc.publish(support_topic, json.dumps(default_payload), QOS)
                 publish_future.result()
                 self._mqtt_events.device_support_event[thing_name].wait()
             
-            self._execution_pools.support_execution_pool.append(self._wrap_async(thing_name, wrapper, timeout))
+            self._execution_pools.support_execution_pool.append(self._wrap_async(thing_name, fn, timeout))
         elif publish_type == "status":
             status_topic = f"{host_identity_id}/{thing_name}/status/request"
             if thing_name in self._mqtt_events.device_status_event:
                 self._mqtt_events.device_status_event[thing_name].clear()
             else:
                 self._mqtt_events.device_status_event[thing_name] = threading.Event()
-            async def wrapper():
+            def fn():
                 publish_future, _ = self._mqttc.publish(status_topic, json.dumps(default_payload), QOS)
                 publish_future.result()
                 self._mqtt_events.device_status_event[thing_name].wait()
-            self._execution_pools.status_execution_pool.append(self._wrap_async(thing_name, wrapper, timeout))
+            self._execution_pools.status_execution_pool.append(self._wrap_async(thing_name, fn, timeout))
         elif publish_type == "control":
             control_topic = f"{host_identity_id}/{thing_name}/control/request"
             if thing_name in self._mqtt_events.device_control_event:
                 self._mqtt_events.device_control_event[thing_name].clear()
             else:
                 self._mqtt_events.device_control_event[thing_name] = threading.Event()
-            async def wrapper():
+            def fn():
                 publish_future, _ = self._mqttc.publish(control_topic, json.dumps(payload), QOS)
                 publish_future.result()
                 self._mqtt_events.device_control_event[thing_name].wait()
-            self._execution_pools.control_execution_pool.append(self._wrap_async(thing_name, wrapper, timeout))
+            self._execution_pools.control_execution_pool.append(self._wrap_async(thing_name, fn, timeout))
 
         else:
             raise ValueError(f"Invalid publish_type: {publish_type}")
 
     def publish_shadow(
         self,
         thing_name: str,
@@ -823,15 +824,15 @@
         self._client_tokens.update({client_token: thing_name})
         if thing_name in self._mqtt_events.device_shadow_event:
             self._mqtt_events.device_shadow_event[thing_name].clear()
         else:
             self._mqtt_events.device_shadow_event[thing_name] = threading.Event()
         
 
-        async def wrapper():
+        def fn():
             if shadow_name is None:
                 if command_name == "get":
                     publish_future = self._shadow_mqttc.publish_get_shadow(
                         iotshadow.GetShadowRequest(
                             client_token=client_token,
                             thing_name=thing_name
                         ),
@@ -882,15 +883,15 @@
                             shadow_name=shadow_name, 
                             thing_name=thing_name
                         ),
                         qos=QOS
                     )
             publish_future.result()
             self._mqtt_events.device_shadow_event[thing_name].wait()
-        self._execution_pools.shadow_execution_pool.append(self._wrap_async(thing_name, wrapper, timeout))
+        self._execution_pools.shadow_execution_pool.append(self._wrap_async(thing_name, fn, timeout))
     
     def execute(self) -> list[list[Union[str, BaseException]], list[Union[str, BaseException]], list[Union[str, BaseException]], list[Union[str, BaseException]]]:
         """Execute publish commands in the execution pools.
         
         Returns
         -------
         list
```

### Comparing `LibJciHitachi-1.2.0/JciHitachi/cert/AmazonRootCA1.pem` & `LibJciHitachi-1.2.1/JciHitachi/cert/AmazonRootCA1.pem`

 * *Files identical despite different names*

### Comparing `LibJciHitachi-1.2.0/JciHitachi/cert/api-jci-hitachi-smarthome-com-chain.pem` & `LibJciHitachi-1.2.1/JciHitachi/cert/api-jci-hitachi-smarthome-com-chain.pem`

 * *Files identical despite different names*

### Comparing `LibJciHitachi-1.2.0/JciHitachi/cert/mqtt-jci-hitachi-smarthome-com-chain.pem` & `LibJciHitachi-1.2.1/JciHitachi/cert/mqtt-jci-hitachi-smarthome-com-chain.pem`

 * *Files identical despite different names*

### Comparing `LibJciHitachi-1.2.0/JciHitachi/connection.py` & `LibJciHitachi-1.2.1/JciHitachi/connection.py`

 * *Files identical despite different names*

### Comparing `LibJciHitachi-1.2.0/JciHitachi/model.py` & `LibJciHitachi-1.2.1/JciHitachi/model.py`

 * *Files identical despite different names*

### Comparing `LibJciHitachi-1.2.0/JciHitachi/mqtt_connection.py` & `LibJciHitachi-1.2.1/JciHitachi/mqtt_connection.py`

 * *Files identical despite different names*

### Comparing `LibJciHitachi-1.2.0/JciHitachi/status.py` & `LibJciHitachi-1.2.1/JciHitachi/status.py`

 * *Files identical despite different names*

### Comparing `LibJciHitachi-1.2.0/LICENSE` & `LibJciHitachi-1.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `LibJciHitachi-1.2.0/LibJciHitachi.egg-info/PKG-INFO` & `LibJciHitachi-1.2.1/LibJciHitachi.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: LibJciHitachi
-Version: 1.2.0
+Version: 1.2.1
 Summary: A library for controlling Jci Hitachi devices.
 Home-page: https://github.com/qqaatw/LibJciHitachi
 Author: Allan Lin
 Author-email: qqaatw@gmail.com
 Project-URL: Issue Tracker, https://github.com/qqaatw/LibJciHitachi/issues
 Project-URL: Documentation, https://libjcihitachi.readthedocs.io/en/latest/
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `LibJciHitachi-1.2.0/LibJciHitachi.egg-info/SOURCES.txt` & `LibJciHitachi-1.2.1/LibJciHitachi.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `LibJciHitachi-1.2.0/PKG-INFO` & `LibJciHitachi-1.2.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: LibJciHitachi
-Version: 1.2.0
+Version: 1.2.1
 Summary: A library for controlling Jci Hitachi devices.
 Home-page: https://github.com/qqaatw/LibJciHitachi
 Author: Allan Lin
 Author-email: qqaatw@gmail.com
 Project-URL: Issue Tracker, https://github.com/qqaatw/LibJciHitachi/issues
 Project-URL: Documentation, https://libjcihitachi.readthedocs.io/en/latest/
 Classifier: Programming Language :: Python :: 3.8
```

### Comparing `LibJciHitachi-1.2.0/README.md` & `LibJciHitachi-1.2.1/README.md`

 * *Files identical despite different names*

### Comparing `LibJciHitachi-1.2.0/setup.py` & `LibJciHitachi-1.2.1/setup.py`

 * *Files identical despite different names*

### Comparing `LibJciHitachi-1.2.0/tests/test_api.py` & `LibJciHitachi-1.2.1/tests/test_api.py`

 * *Files identical despite different names*

### Comparing `LibJciHitachi-1.2.0/tests/test_aws_connection.py` & `LibJciHitachi-1.2.1/tests/test_aws_connection.py`

 * *Files identical despite different names*

### Comparing `LibJciHitachi-1.2.0/tests/test_integration.py` & `LibJciHitachi-1.2.1/tests/test_integration.py`

 * *Files identical despite different names*

### Comparing `LibJciHitachi-1.2.0/tests/test_model.py` & `LibJciHitachi-1.2.1/tests/test_model.py`

 * *Files identical despite different names*

### Comparing `LibJciHitachi-1.2.0/tests/test_sanity.py` & `LibJciHitachi-1.2.1/tests/test_sanity.py`

 * *Files identical despite different names*

### Comparing `LibJciHitachi-1.2.0/tests/test_status.py` & `LibJciHitachi-1.2.1/tests/test_status.py`

 * *Files identical despite different names*

