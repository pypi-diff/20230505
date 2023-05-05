# Comparing `tmp/kingspan_connect_sensor-2.1.0.tar.gz` & `tmp/kingspan_connect_sensor-2.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kingspan_connect_sensor-2.1.0.tar", max compression
+gzip compressed data, was "kingspan_connect_sensor-2.1.1.tar", max compression
```

## Comparing `kingspan_connect_sensor-2.1.0.tar` & `kingspan_connect_sensor-2.1.1.tar`

### file list

```diff
@@ -1,13 +1,12 @@
--rw-r--r--   0        0        0     1078 2022-11-19 09:25:30.276140 kingspan_connect_sensor-2.1.0/LICENSE
--rw-r--r--   0        0        0     3604 2022-11-26 11:07:29.414711 kingspan_connect_sensor-2.1.0/README.md
--rw-r--r--   0        0        0     2289 2023-02-26 17:41:54.246946 kingspan_connect_sensor-2.1.0/pyproject.toml
--rw-r--r--   0        0        0      190 2022-11-24 19:10:40.355078 kingspan_connect_sensor-2.1.0/src/connectsensor/__init__.py
--rw-r--r--   0        0        0     3542 2022-11-26 08:54:31.150331 kingspan_connect_sensor-2.1.0/src/connectsensor/_kingspan_export.py
--rw-r--r--   0        0        0     5722 2022-11-26 10:59:27.697337 kingspan_connect_sensor-2.1.0/src/connectsensor/_kingspan_notifier.py
--rw-r--r--   0        0        0     1816 2023-02-26 17:41:22.129396 kingspan_connect_sensor-2.1.0/src/connectsensor/_kingspan_status.py
--rw-r--r--   0        0        0     4488 2022-11-24 19:48:32.745484 kingspan_connect_sensor-2.1.0/src/connectsensor/client.py
--rw-r--r--   0        0        0      545 2021-01-30 15:44:34.000000 kingspan_connect_sensor-2.1.0/src/connectsensor/debug.py
--rw-r--r--   0        0        0      200 2022-11-24 13:07:58.577473 kingspan_connect_sensor-2.1.0/src/connectsensor/exceptions.py
--rw-r--r--   0        0        0     3551 2022-12-11 15:27:42.709954 kingspan_connect_sensor-2.1.0/src/connectsensor/tank.py
--rw-r--r--   0        0        0     4956 1970-01-01 00:00:00.000000 kingspan_connect_sensor-2.1.0/setup.py
--rw-r--r--   0        0        0     4889 1970-01-01 00:00:00.000000 kingspan_connect_sensor-2.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1078 2022-11-19 09:25:30.276140 kingspan_connect_sensor-2.1.1/LICENSE
+-rw-r--r--   0        0        0     3604 2022-11-26 11:07:29.414711 kingspan_connect_sensor-2.1.1/README.md
+-rw-r--r--   0        0        0     2285 2023-05-05 08:22:02.083484 kingspan_connect_sensor-2.1.1/pyproject.toml
+-rw-r--r--   0        0        0      190 2022-11-24 19:10:40.355078 kingspan_connect_sensor-2.1.1/src/connectsensor/__init__.py
+-rw-r--r--   0        0        0     3542 2022-11-26 08:54:31.150331 kingspan_connect_sensor-2.1.1/src/connectsensor/_kingspan_export.py
+-rw-r--r--   0        0        0     5722 2022-11-26 10:59:27.697337 kingspan_connect_sensor-2.1.1/src/connectsensor/_kingspan_notifier.py
+-rw-r--r--   0        0        0     1816 2023-02-26 17:41:22.129396 kingspan_connect_sensor-2.1.1/src/connectsensor/_kingspan_status.py
+-rw-r--r--   0        0        0     4488 2022-11-24 19:48:32.745484 kingspan_connect_sensor-2.1.1/src/connectsensor/client.py
+-rw-r--r--   0        0        0      545 2021-01-30 15:44:34.000000 kingspan_connect_sensor-2.1.1/src/connectsensor/debug.py
+-rw-r--r--   0        0        0      200 2022-11-24 13:07:58.577473 kingspan_connect_sensor-2.1.1/src/connectsensor/exceptions.py
+-rw-r--r--   0        0        0     3551 2022-12-11 15:27:42.709954 kingspan_connect_sensor-2.1.1/src/connectsensor/tank.py
+-rw-r--r--   0        0        0     4885 1970-01-01 00:00:00.000000 kingspan_connect_sensor-2.1.1/PKG-INFO
```

### Comparing `kingspan_connect_sensor-2.1.0/LICENSE` & `kingspan_connect_sensor-2.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `kingspan_connect_sensor-2.1.0/README.md` & `kingspan_connect_sensor-2.1.1/README.md`

 * *Files identical despite different names*

### Comparing `kingspan_connect_sensor-2.1.0/pyproject.toml` & `kingspan_connect_sensor-2.1.1/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -11,22 +11,22 @@
 description = "API to get oil tank from Kingspan SENSiT sensors"
 documentation = "https://github.com/masaccio/kingspan-connect-sensor/blob/main/README.md"
 license = "MIT"
 name = "kingspan-connect-sensor"
 packages = [{include = "connectsensor", from = "src"}]
 readme = "README.md"
 repository = "https://github.com/masaccio/kingspan-connect-sensor"
-version = "2.1.0"
+version = "2.1.1"
 
 [tool.poetry.dependencies]
 async-property = "^0.2.1"
 asyncio = "^3.4.3"
 datetime = "^4.7"
-# homeassistant has a constraint on httpx==0.23.1
-httpx = "^0.23.0"
+# homeassistant has a constraint on httpx==0.24
+httpx = "^0.24"
 # homeassistant has a constraint on pandas==1.4.3
 pandas = "^1.4.3"
 python = "^3.9"
 requests = "^2.28.1"
 zeep = "^4.2.0"
 
 [tool.poetry.group.dev.dependencies]
```

### Comparing `kingspan_connect_sensor-2.1.0/src/connectsensor/_kingspan_export.py` & `kingspan_connect_sensor-2.1.1/src/connectsensor/_kingspan_export.py`

 * *Files identical despite different names*

### Comparing `kingspan_connect_sensor-2.1.0/src/connectsensor/_kingspan_notifier.py` & `kingspan_connect_sensor-2.1.1/src/connectsensor/_kingspan_notifier.py`

 * *Files identical despite different names*

### Comparing `kingspan_connect_sensor-2.1.0/src/connectsensor/_kingspan_status.py` & `kingspan_connect_sensor-2.1.1/src/connectsensor/_kingspan_status.py`

 * *Files identical despite different names*

### Comparing `kingspan_connect_sensor-2.1.0/src/connectsensor/client.py` & `kingspan_connect_sensor-2.1.1/src/connectsensor/client.py`

 * *Files identical despite different names*

### Comparing `kingspan_connect_sensor-2.1.0/src/connectsensor/debug.py` & `kingspan_connect_sensor-2.1.1/src/connectsensor/debug.py`

 * *Files identical despite different names*

### Comparing `kingspan_connect_sensor-2.1.0/src/connectsensor/tank.py` & `kingspan_connect_sensor-2.1.1/src/connectsensor/tank.py`

 * *Files identical despite different names*

### Comparing `kingspan_connect_sensor-2.1.0/PKG-INFO` & `kingspan_connect_sensor-2.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kingspan-connect-sensor
-Version: 2.1.0
+Version: 2.1.1
 Summary: API to get oil tank from Kingspan SENSiT sensors
 Home-page: https://github.com/masaccio/kingspan-connect-sensor
 License: MIT
 Author: Jon Connell
 Author-email: python@figsandfudge.com
 Requires-Python: >=3.9,<4.0
 Classifier: Development Status :: 5 - Production/Stable
@@ -16,15 +16,15 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3
 Requires-Dist: async-property (>=0.2.1,<0.3.0)
 Requires-Dist: asyncio (>=3.4.3,<4.0.0)
 Requires-Dist: datetime (>=4.7,<5.0)
-Requires-Dist: httpx (>=0.23.0,<0.24.0)
+Requires-Dist: httpx (>=0.24,<0.25)
 Requires-Dist: pandas (>=1.4.3,<2.0.0)
 Requires-Dist: requests (>=2.28.1,<3.0.0)
 Requires-Dist: zeep (>=4.2.0,<5.0.0)
 Project-URL: Documentation, https://github.com/masaccio/kingspan-connect-sensor/blob/main/README.md
 Project-URL: Repository, https://github.com/masaccio/kingspan-connect-sensor
 Description-Content-Type: text/markdown
```

