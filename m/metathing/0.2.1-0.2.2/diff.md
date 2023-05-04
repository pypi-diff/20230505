# Comparing `tmp/metathing-0.2.1.tar.gz` & `tmp/metathing-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "metathing-0.2.1.tar", last modified: Thu May  4 13:59:40 2023, max compression
+gzip compressed data, was "metathing-0.2.2.tar", last modified: Thu May  4 23:27:20 2023, max compression
```

## Comparing `metathing-0.2.1.tar` & `metathing-0.2.2.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 13:59:40.185782 metathing-0.2.1/
--rw-r--r--   0 root         (0) root         (0)       93 2023-05-04 13:59:40.182449 metathing-0.2.1/PKG-INFO
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 13:59:40.172449 metathing-0.2.1/metathing/
--rw-r--r--   0 root         (0) root         (0)        0 2023-02-25 13:42:49.000000 metathing-0.2.1/metathing/__init__.py
--rw-r--r--   0 root         (0) root         (0)     2210 2023-03-31 12:28:23.000000 metathing-0.2.1/metathing/alarmer.py
--rw-r--r--   0 root         (0) root         (0)     9007 2023-05-04 13:48:06.000000 metathing-0.2.1/metathing/application.py
--rw-r--r--   0 root         (0) root         (0)      290 2023-02-25 13:42:49.000000 metathing-0.2.1/metathing/config.py
--rw-r--r--   0 root         (0) root         (0)    20090 2023-04-22 14:51:16.000000 metathing-0.2.1/metathing/device.py
--rw-r--r--   0 root         (0) root         (0)    16266 2023-03-31 01:10:23.000000 metathing-0.2.1/metathing/http.py
--rw-r--r--   0 root         (0) root         (0)     1117 2023-04-11 23:36:40.000000 metathing-0.2.1/metathing/logger.py
--rw-r--r--   0 root         (0) root         (0)     3931 2023-05-04 13:56:53.000000 metathing-0.2.1/metathing/metathing.py
--rw-r--r--   0 root         (0) root         (0)     6853 2023-04-13 16:58:53.000000 metathing-0.2.1/metathing/mqtt.py
--rw-r--r--   0 root         (0) root         (0)     3844 2023-03-28 12:54:26.000000 metathing-0.2.1/metathing/service.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 13:59:40.182449 metathing-0.2.1/metathing.egg-info/
--rw-r--r--   0 root         (0) root         (0)       93 2023-05-04 13:59:39.000000 metathing-0.2.1/metathing.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)      348 2023-05-04 13:59:39.000000 metathing-0.2.1/metathing.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-05-04 13:59:39.000000 metathing-0.2.1/metathing.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)       10 2023-05-04 13:59:39.000000 metathing-0.2.1/metathing.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-05-04 13:59:40.185782 metathing-0.2.1/setup.cfg
--rw-r--r--   0 root         (0) root         (0)      243 2023-05-04 13:59:19.000000 metathing-0.2.1/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 23:27:20.200119 metathing-0.2.2/
+-rw-r--r--   0 root         (0) root         (0)       93 2023-05-04 23:27:20.196786 metathing-0.2.2/PKG-INFO
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 23:27:20.186786 metathing-0.2.2/metathing/
+-rw-r--r--   0 root         (0) root         (0)        0 2023-02-25 13:42:49.000000 metathing-0.2.2/metathing/__init__.py
+-rw-r--r--   0 root         (0) root         (0)     2210 2023-03-31 12:28:23.000000 metathing-0.2.2/metathing/alarmer.py
+-rw-r--r--   0 root         (0) root         (0)     9007 2023-05-04 13:48:06.000000 metathing-0.2.2/metathing/application.py
+-rw-r--r--   0 root         (0) root         (0)      290 2023-02-25 13:42:49.000000 metathing-0.2.2/metathing/config.py
+-rw-r--r--   0 root         (0) root         (0)    20090 2023-04-22 14:51:16.000000 metathing-0.2.2/metathing/device.py
+-rw-r--r--   0 root         (0) root         (0)    16266 2023-03-31 01:10:23.000000 metathing-0.2.2/metathing/http.py
+-rw-r--r--   0 root         (0) root         (0)     1117 2023-04-11 23:36:40.000000 metathing-0.2.2/metathing/logger.py
+-rw-r--r--   0 root         (0) root         (0)     3953 2023-05-04 23:26:41.000000 metathing-0.2.2/metathing/metathing.py
+-rw-r--r--   0 root         (0) root         (0)     6853 2023-04-13 16:58:53.000000 metathing-0.2.2/metathing/mqtt.py
+-rw-r--r--   0 root         (0) root         (0)     3844 2023-03-28 12:54:26.000000 metathing-0.2.2/metathing/service.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-04 23:27:20.196786 metathing-0.2.2/metathing.egg-info/
+-rw-r--r--   0 root         (0) root         (0)       93 2023-05-04 23:27:19.000000 metathing-0.2.2/metathing.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)      348 2023-05-04 23:27:19.000000 metathing-0.2.2/metathing.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-04 23:27:19.000000 metathing-0.2.2/metathing.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)       10 2023-05-04 23:27:19.000000 metathing-0.2.2/metathing.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-05-04 23:27:20.203452 metathing-0.2.2/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)      243 2023-05-04 23:26:49.000000 metathing-0.2.2/setup.py
```

### Comparing `metathing-0.2.1/metathing/alarmer.py` & `metathing-0.2.2/metathing/alarmer.py`

 * *Files identical despite different names*

### Comparing `metathing-0.2.1/metathing/application.py` & `metathing-0.2.2/metathing/application.py`

 * *Files identical despite different names*

### Comparing `metathing-0.2.1/metathing/device.py` & `metathing-0.2.2/metathing/device.py`

 * *Files identical despite different names*

### Comparing `metathing-0.2.1/metathing/http.py` & `metathing-0.2.2/metathing/http.py`

 * *Files identical despite different names*

### Comparing `metathing-0.2.1/metathing/logger.py` & `metathing-0.2.2/metathing/logger.py`

 * *Files identical despite different names*

### Comparing `metathing-0.2.1/metathing/metathing.py` & `metathing-0.2.2/metathing/metathing.py`

 * *Files 1% similar despite different names*

```diff
@@ -38,14 +38,15 @@
                 pid = conn.pid
                 psutil.Process(pid).kill()
                 logger.warning(f"Killed conflicted process with pid {pid}")
         
     @staticmethod
     def MTNodeIPRequest():
         req_msg = 'MTNode_IP_REQUEST'
+        time.sleep(5)
         
         # Check connection
         sock = socket.socket(socket.AF_INET, socket.SOCK_DGRAM, socket.IPPROTO_UDP)
         sock.setsockopt(socket.IPPROTO_IP, socket.IP_MULTICAST_TTL, 2)
         sock_recv = socket.socket(socket.AF_INET, socket.SOCK_DGRAM, socket.IPPROTO_UDP)
         sock_recv.setsockopt(socket.SOL_SOCKET, socket.SO_REUSEADDR, 1)
         sock_recv.bind(('', RECV_MCAST_PORT))
```

### Comparing `metathing-0.2.1/metathing/mqtt.py` & `metathing-0.2.2/metathing/mqtt.py`

 * *Files identical despite different names*

### Comparing `metathing-0.2.1/metathing/service.py` & `metathing-0.2.2/metathing/service.py`

 * *Files identical despite different names*

