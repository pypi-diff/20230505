# Comparing `tmp/artemis_utils-1.0.8.tar.gz` & `tmp/artemis_utils-1.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/artemis_utils-1.0.8.tar", last modified: Fri Jan  8 09:31:34 2021, max compression
+gzip compressed data, was "dist/artemis_utils-1.0.9.tar", last modified: Thu Feb 18 12:57:01 2021, max compression
```

## Comparing `artemis_utils-1.0.8.tar` & `artemis_utils-1.0.9.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxr-x   0 vkotronis  (1000) vkotronis  (1000)        0 2021-01-08 09:31:34.879563 artemis_utils-1.0.8/
--rw-rw-r--   0 vkotronis  (1000) vkotronis  (1000)     1104 2021-01-08 09:31:34.879563 artemis_utils-1.0.8/PKG-INFO
--rw-rw-r--   0 vkotronis  (1000) vkotronis  (1000)      486 2020-11-06 12:06:37.000000 artemis_utils-1.0.8/README.md
-drwxrwxr-x   0 vkotronis  (1000) vkotronis  (1000)        0 2021-01-08 09:31:34.879563 artemis_utils-1.0.8/artemis_utils/
--rw-rw-r--   0 vkotronis  (1000) vkotronis  (1000)     3381 2020-12-23 15:01:52.000000 artemis_utils-1.0.8/artemis_utils/__init__.py
--rw-rw-r--   0 vkotronis  (1000) vkotronis  (1000)     6538 2020-12-23 15:01:52.000000 artemis_utils-1.0.8/artemis_utils/conf_lib.py
--rw-rw-r--   0 vkotronis  (1000) vkotronis  (1000)     1148 2020-12-23 15:01:52.000000 artemis_utils-1.0.8/artemis_utils/constants.py
--rw-rw-r--   0 vkotronis  (1000) vkotronis  (1000)     6039 2020-12-23 15:01:52.000000 artemis_utils-1.0.8/artemis_utils/db.py
--rw-rw-r--   0 vkotronis  (1000) vkotronis  (1000)     2247 2020-12-23 15:01:52.000000 artemis_utils-1.0.8/artemis_utils/envvars.py
--rw-rw-r--   0 vkotronis  (1000) vkotronis  (1000)     3302 2020-12-23 15:01:52.000000 artemis_utils-1.0.8/artemis_utils/logaux.py
--rw-rw-r--   0 vkotronis  (1000) vkotronis  (1000)      784 2020-12-23 15:01:52.000000 artemis_utils-1.0.8/artemis_utils/rabbitmq.py
--rw-rw-r--   0 vkotronis  (1000) vkotronis  (1000)     3753 2021-01-08 09:30:26.000000 artemis_utils-1.0.8/artemis_utils/redis.py
--rw-rw-r--   0 vkotronis  (1000) vkotronis  (1000)      540 2020-12-23 15:01:52.000000 artemis_utils-1.0.8/artemis_utils/rpki.py
--rw-rw-r--   0 vkotronis  (1000) vkotronis  (1000)     3151 2020-12-23 15:01:52.000000 artemis_utils-1.0.8/artemis_utils/service.py
--rw-rw-r--   0 vkotronis  (1000) vkotronis  (1000)     7675 2020-12-23 15:01:52.000000 artemis_utils-1.0.8/artemis_utils/translations.py
--rw-rw-r--   0 vkotronis  (1000) vkotronis  (1000)     6548 2020-12-23 15:01:52.000000 artemis_utils-1.0.8/artemis_utils/updates.py
-drwxrwxr-x   0 vkotronis  (1000) vkotronis  (1000)        0 2021-01-08 09:31:34.879563 artemis_utils-1.0.8/artemis_utils.egg-info/
--rw-rw-r--   0 vkotronis  (1000) vkotronis  (1000)     1104 2021-01-08 09:31:34.000000 artemis_utils-1.0.8/artemis_utils.egg-info/PKG-INFO
--rw-rw-r--   0 vkotronis  (1000) vkotronis  (1000)      501 2021-01-08 09:31:34.000000 artemis_utils-1.0.8/artemis_utils.egg-info/SOURCES.txt
--rw-rw-r--   0 vkotronis  (1000) vkotronis  (1000)        1 2021-01-08 09:31:34.000000 artemis_utils-1.0.8/artemis_utils.egg-info/dependency_links.txt
--rw-rw-r--   0 vkotronis  (1000) vkotronis  (1000)      117 2021-01-08 09:31:34.000000 artemis_utils-1.0.8/artemis_utils.egg-info/requires.txt
--rw-rw-r--   0 vkotronis  (1000) vkotronis  (1000)       14 2021-01-08 09:31:34.000000 artemis_utils-1.0.8/artemis_utils.egg-info/top_level.txt
--rw-rw-r--   0 vkotronis  (1000) vkotronis  (1000)       38 2021-01-08 09:31:34.879563 artemis_utils-1.0.8/setup.cfg
--rw-rw-r--   0 vkotronis  (1000) vkotronis  (1000)     1052 2021-01-08 09:30:26.000000 artemis_utils-1.0.8/setup.py
+drwxrwxr-x   0 vkotronis  (1000) vkotronis  (1000)        0 2021-02-18 12:57:01.711732 artemis_utils-1.0.9/
+-rw-rw-r--   0 vkotronis  (1000) vkotronis  (1000)     1104 2021-02-18 12:57:01.711732 artemis_utils-1.0.9/PKG-INFO
+-rw-rw-r--   0 vkotronis  (1000) vkotronis  (1000)      486 2021-02-12 11:45:48.000000 artemis_utils-1.0.9/README.md
+drwxrwxr-x   0 vkotronis  (1000) vkotronis  (1000)        0 2021-02-18 12:57:01.711732 artemis_utils-1.0.9/artemis_utils/
+-rw-rw-r--   0 vkotronis  (1000) vkotronis  (1000)     3381 2021-02-12 11:45:48.000000 artemis_utils-1.0.9/artemis_utils/__init__.py
+-rw-rw-r--   0 vkotronis  (1000) vkotronis  (1000)     6538 2021-02-12 11:45:48.000000 artemis_utils-1.0.9/artemis_utils/conf_lib.py
+-rw-rw-r--   0 vkotronis  (1000) vkotronis  (1000)     1148 2021-02-12 11:45:48.000000 artemis_utils-1.0.9/artemis_utils/constants.py
+-rw-rw-r--   0 vkotronis  (1000) vkotronis  (1000)     6039 2021-02-12 11:45:48.000000 artemis_utils-1.0.9/artemis_utils/db.py
+-rw-rw-r--   0 vkotronis  (1000) vkotronis  (1000)     2247 2021-02-12 11:45:48.000000 artemis_utils-1.0.9/artemis_utils/envvars.py
+-rw-rw-r--   0 vkotronis  (1000) vkotronis  (1000)     3302 2021-02-12 11:45:48.000000 artemis_utils-1.0.9/artemis_utils/logaux.py
+-rw-rw-r--   0 vkotronis  (1000) vkotronis  (1000)      784 2021-02-12 11:45:48.000000 artemis_utils-1.0.9/artemis_utils/rabbitmq.py
+-rw-rw-r--   0 vkotronis  (1000) vkotronis  (1000)     3800 2021-02-12 11:45:48.000000 artemis_utils-1.0.9/artemis_utils/redis.py
+-rw-rw-r--   0 vkotronis  (1000) vkotronis  (1000)      540 2021-02-12 11:45:48.000000 artemis_utils-1.0.9/artemis_utils/rpki.py
+-rw-rw-r--   0 vkotronis  (1000) vkotronis  (1000)     3151 2021-02-12 11:45:48.000000 artemis_utils-1.0.9/artemis_utils/service.py
+-rw-rw-r--   0 vkotronis  (1000) vkotronis  (1000)     7675 2021-02-12 11:45:48.000000 artemis_utils-1.0.9/artemis_utils/translations.py
+-rw-rw-r--   0 vkotronis  (1000) vkotronis  (1000)     6548 2021-02-12 11:45:48.000000 artemis_utils-1.0.9/artemis_utils/updates.py
+drwxrwxr-x   0 vkotronis  (1000) vkotronis  (1000)        0 2021-02-18 12:57:01.711732 artemis_utils-1.0.9/artemis_utils.egg-info/
+-rw-rw-r--   0 vkotronis  (1000) vkotronis  (1000)     1104 2021-02-18 12:57:01.000000 artemis_utils-1.0.9/artemis_utils.egg-info/PKG-INFO
+-rw-rw-r--   0 vkotronis  (1000) vkotronis  (1000)      501 2021-02-18 12:57:01.000000 artemis_utils-1.0.9/artemis_utils.egg-info/SOURCES.txt
+-rw-rw-r--   0 vkotronis  (1000) vkotronis  (1000)        1 2021-02-18 12:57:01.000000 artemis_utils-1.0.9/artemis_utils.egg-info/dependency_links.txt
+-rw-rw-r--   0 vkotronis  (1000) vkotronis  (1000)      144 2021-02-18 12:57:01.000000 artemis_utils-1.0.9/artemis_utils.egg-info/requires.txt
+-rw-rw-r--   0 vkotronis  (1000) vkotronis  (1000)       14 2021-02-18 12:57:01.000000 artemis_utils-1.0.9/artemis_utils.egg-info/top_level.txt
+-rw-rw-r--   0 vkotronis  (1000) vkotronis  (1000)       38 2021-02-18 12:57:01.711732 artemis_utils-1.0.9/setup.cfg
+-rw-rw-r--   0 vkotronis  (1000) vkotronis  (1000)     1090 2021-02-18 12:56:07.000000 artemis_utils-1.0.9/setup.py
```

### Comparing `artemis_utils-1.0.8/PKG-INFO` & `artemis_utils-1.0.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: artemis_utils
-Version: 1.0.8
+Version: 1.0.9
 Summary: ARTEMIS utility modules
 Home-page: https://github.com/FORTH-ICS-INSPIRE/artemis
 Author: Dimitrios Mavrommatis, Vassileios Kotronis
 Author-email: jim.mavrommatis@gmail.com, biece89@gmail.com
 License: UNKNOWN
 Description: ARTEMIS is an open-source tool, that implements a defense approach against BGP prefix hijacking attacks.
```

### Comparing `artemis_utils-1.0.8/artemis_utils/__init__.py` & `artemis_utils-1.0.9/artemis_utils/__init__.py`

 * *Files identical despite different names*

### Comparing `artemis_utils-1.0.8/artemis_utils/conf_lib.py` & `artemis_utils-1.0.9/artemis_utils/conf_lib.py`

 * *Files identical despite different names*

### Comparing `artemis_utils-1.0.8/artemis_utils/constants.py` & `artemis_utils-1.0.9/artemis_utils/constants.py`

 * *Files identical despite different names*

### Comparing `artemis_utils-1.0.8/artemis_utils/db.py` & `artemis_utils-1.0.9/artemis_utils/db.py`

 * *Files identical despite different names*

### Comparing `artemis_utils-1.0.8/artemis_utils/envvars.py` & `artemis_utils-1.0.9/artemis_utils/envvars.py`

 * *Files identical despite different names*

### Comparing `artemis_utils-1.0.8/artemis_utils/logaux.py` & `artemis_utils-1.0.9/artemis_utils/logaux.py`

 * *Files identical despite different names*

### Comparing `artemis_utils-1.0.8/artemis_utils/rabbitmq.py` & `artemis_utils-1.0.9/artemis_utils/rabbitmq.py`

 * *Files identical despite different names*

### Comparing `artemis_utils-1.0.8/artemis_utils/redis.py` & `artemis_utils-1.0.9/artemis_utils/redis.py`

 * *Files 5% similar despite different names*

```diff
@@ -59,15 +59,21 @@
 
 
 class RedisExpiryChecker:
     """
     Checker for redis expiry events (stops data worker and allows it to restart automatically)
     """
 
-    def __init__(self, redis=None, shared_memory_manager_dict=None, monitor=None, stop_data_worker_fun=None):
+    def __init__(
+        self,
+        redis=None,
+        shared_memory_manager_dict=None,
+        monitor=None,
+        stop_data_worker_fun=None,
+    ):
         self.redis = redis
         self.shared_memory_manager_dict = shared_memory_manager_dict
         self.redis_pubsub = self.redis.pubsub()
         self.redis_pubsub_mon_channel = "__keyspace@0__:{}_seen_bgp_update".format(
             monitor
         )
         self.redis_listener_thread = None
```

### Comparing `artemis_utils-1.0.8/artemis_utils/rpki.py` & `artemis_utils-1.0.9/artemis_utils/rpki.py`

 * *Files identical despite different names*

### Comparing `artemis_utils-1.0.8/artemis_utils/service.py` & `artemis_utils-1.0.9/artemis_utils/service.py`

 * *Files identical despite different names*

### Comparing `artemis_utils-1.0.8/artemis_utils/translations.py` & `artemis_utils-1.0.9/artemis_utils/translations.py`

 * *Files identical despite different names*

### Comparing `artemis_utils-1.0.8/artemis_utils/updates.py` & `artemis_utils-1.0.9/artemis_utils/updates.py`

 * *Files identical despite different names*

### Comparing `artemis_utils-1.0.8/artemis_utils.egg-info/PKG-INFO` & `artemis_utils-1.0.9/artemis_utils.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: artemis-utils
-Version: 1.0.8
+Version: 1.0.9
 Summary: ARTEMIS utility modules
 Home-page: https://github.com/FORTH-ICS-INSPIRE/artemis
 Author: Dimitrios Mavrommatis, Vassileios Kotronis
 Author-email: jim.mavrommatis@gmail.com, biece89@gmail.com
 License: UNKNOWN
 Description: ARTEMIS is an open-source tool, that implements a defense approach against BGP prefix hijacking attacks.
```

### Comparing `artemis_utils-1.0.8/setup.py` & `artemis_utils-1.0.9/setup.py`

 * *Files 12% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 this_directory = path.abspath(path.dirname(__file__))
 with open(path.join(this_directory, "README.md"), encoding="utf-8") as f:
     long_description = f.read()
 
 setuptools.setup(
     name="artemis_utils",
-    version="1.0.8",
+    version="1.0.9",
     author="Dimitrios Mavrommatis, Vassileios Kotronis",
     author_email="jim.mavrommatis@gmail.com, biece89@gmail.com",
     description="ARTEMIS utility modules",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/FORTH-ICS-INSPIRE/artemis",
     packages=setuptools.find_packages(),
@@ -26,10 +26,11 @@
         "kombu==4.6.7",
         "ruamel.yaml==0.16.5",
         "ujson==1.35",
         "PyYAML==5.3",
         "gql==0.4.0",
         "ipaddress==1.0.23",
         "psycopg2==2.8.4",
+        "slacker-log-handler==1.7.1",
         "tornado==6.0.4",
     ],
 )
```

