# Comparing `tmp/locura_iotlab_bridge-0.1.6.tar.gz` & `tmp/locura_iotlab_bridge-0.1.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/locura_iotlab_bridge-0.1.6.tar", last modified: Thu Apr 27 15:12:55 2023, max compression
+gzip compressed data, was "dist/locura_iotlab_bridge-0.1.7.tar", last modified: Fri May  5 10:22:25 2023, max compression
```

## Comparing `locura_iotlab_bridge-0.1.6.tar` & `locura_iotlab_bridge-0.1.7.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 quentin   (1000) quentin   (1000)        0 2023-04-27 15:12:55.000000 locura_iotlab_bridge-0.1.6/
--rw-r--r--   0 quentin   (1000) quentin   (1000)      503 2023-04-27 15:12:55.000000 locura_iotlab_bridge-0.1.6/PKG-INFO
--rw-r--r--   0 quentin   (1000) quentin   (1000)      718 2023-04-27 15:12:53.000000 locura_iotlab_bridge-0.1.6/setup.py
-drwxr-xr-x   0 quentin   (1000) quentin   (1000)        0 2023-04-27 15:12:55.000000 locura_iotlab_bridge-0.1.6/locura_iotlab_bridge/
--rwxr-xr-x   0 quentin   (1000) quentin   (1000)     6786 2023-04-27 15:11:34.000000 locura_iotlab_bridge-0.1.6/locura_iotlab_bridge/locura_iotlab_bridge.py
--rw-r--r--   0 quentin   (1000) quentin   (1000)     1156 2023-04-27 14:49:52.000000 locura_iotlab_bridge-0.1.6/locura_iotlab_bridge/helpers.py
--rw-r--r--   0 quentin   (1000) quentin   (1000)       49 2022-12-12 15:29:01.000000 locura_iotlab_bridge-0.1.6/locura_iotlab_bridge/__init__.py
--rw-r--r--   0 quentin   (1000) quentin   (1000)       38 2023-04-27 15:12:55.000000 locura_iotlab_bridge-0.1.6/setup.cfg
--rw-r--r--   0 quentin   (1000) quentin   (1000)    21783 2022-12-12 13:41:17.000000 locura_iotlab_bridge-0.1.6/LICENSE
-drwxr-xr-x   0 quentin   (1000) quentin   (1000)        0 2023-04-27 15:12:55.000000 locura_iotlab_bridge-0.1.6/locura_iotlab_bridge.egg-info/
--rw-r--r--   0 quentin   (1000) quentin   (1000)      503 2023-04-27 15:12:55.000000 locura_iotlab_bridge-0.1.6/locura_iotlab_bridge.egg-info/PKG-INFO
--rw-r--r--   0 quentin   (1000) quentin   (1000)      345 2023-04-27 15:12:55.000000 locura_iotlab_bridge-0.1.6/locura_iotlab_bridge.egg-info/SOURCES.txt
--rw-r--r--   0 quentin   (1000) quentin   (1000)       21 2023-04-27 15:12:55.000000 locura_iotlab_bridge-0.1.6/locura_iotlab_bridge.egg-info/top_level.txt
--rw-r--r--   0 quentin   (1000) quentin   (1000)        1 2023-04-27 15:12:55.000000 locura_iotlab_bridge-0.1.6/locura_iotlab_bridge.egg-info/dependency_links.txt
--rw-r--r--   0 quentin   (1000) quentin   (1000)       27 2023-04-27 15:12:55.000000 locura_iotlab_bridge-0.1.6/locura_iotlab_bridge.egg-info/requires.txt
+drwxr-xr-x   0 quentin   (1000) quentin   (1000)        0 2023-05-05 10:22:25.000000 locura_iotlab_bridge-0.1.7/
+-rw-r--r--   0 quentin   (1000) quentin   (1000)      503 2023-05-05 10:22:25.000000 locura_iotlab_bridge-0.1.7/PKG-INFO
+-rw-r--r--   0 quentin   (1000) quentin   (1000)      718 2023-05-05 10:22:07.000000 locura_iotlab_bridge-0.1.7/setup.py
+drwxr-xr-x   0 quentin   (1000) quentin   (1000)        0 2023-05-05 10:22:25.000000 locura_iotlab_bridge-0.1.7/locura_iotlab_bridge/
+-rwxr-xr-x   0 quentin   (1000) quentin   (1000)     6848 2023-05-05 10:21:12.000000 locura_iotlab_bridge-0.1.7/locura_iotlab_bridge/locura_iotlab_bridge.py
+-rw-r--r--   0 quentin   (1000) quentin   (1000)     1156 2023-04-27 14:49:52.000000 locura_iotlab_bridge-0.1.7/locura_iotlab_bridge/helpers.py
+-rw-r--r--   0 quentin   (1000) quentin   (1000)       49 2022-12-12 15:29:01.000000 locura_iotlab_bridge-0.1.7/locura_iotlab_bridge/__init__.py
+-rw-r--r--   0 quentin   (1000) quentin   (1000)       38 2023-05-05 10:22:25.000000 locura_iotlab_bridge-0.1.7/setup.cfg
+-rw-r--r--   0 quentin   (1000) quentin   (1000)    21783 2022-12-12 13:41:17.000000 locura_iotlab_bridge-0.1.7/LICENSE
+drwxr-xr-x   0 quentin   (1000) quentin   (1000)        0 2023-05-05 10:22:25.000000 locura_iotlab_bridge-0.1.7/locura_iotlab_bridge.egg-info/
+-rw-r--r--   0 quentin   (1000) quentin   (1000)      503 2023-05-05 10:22:25.000000 locura_iotlab_bridge-0.1.7/locura_iotlab_bridge.egg-info/PKG-INFO
+-rw-r--r--   0 quentin   (1000) quentin   (1000)      345 2023-05-05 10:22:25.000000 locura_iotlab_bridge-0.1.7/locura_iotlab_bridge.egg-info/SOURCES.txt
+-rw-r--r--   0 quentin   (1000) quentin   (1000)       21 2023-05-05 10:22:25.000000 locura_iotlab_bridge-0.1.7/locura_iotlab_bridge.egg-info/top_level.txt
+-rw-r--r--   0 quentin   (1000) quentin   (1000)        1 2023-05-05 10:22:25.000000 locura_iotlab_bridge-0.1.7/locura_iotlab_bridge.egg-info/dependency_links.txt
+-rw-r--r--   0 quentin   (1000) quentin   (1000)       27 2023-05-05 10:22:25.000000 locura_iotlab_bridge-0.1.7/locura_iotlab_bridge.egg-info/requires.txt
```

### Comparing `locura_iotlab_bridge-0.1.6/setup.py` & `locura_iotlab_bridge-0.1.7/setup.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup
 
 setup(
     name='locura_iotlab_bridge',
-    version='0.1.6',    
+    version='0.1.7',    
     description='Bridge to connect LocURa MQTT ecosystem to IOT-LAB',
     url='https://gitlab.irit.fr/rmess/locura/infra/locura_iotlab_bridge',
     author='Quentin Vey',
     author_email='quentin.vey@irit.fr',
     license='CeCILL 2.1',
     packages=['locura_iotlab_bridge'],
     install_requires=['iotlabcli>=3.3.0',
```

### Comparing `locura_iotlab_bridge-0.1.6/locura_iotlab_bridge/locura_iotlab_bridge.py` & `locura_iotlab_bridge-0.1.7/locura_iotlab_bridge/locura_iotlab_bridge.py`

 * *Files 2% similar despite different names*

```diff
@@ -129,15 +129,15 @@
         mapping = None
 
     # Let's exploit automatic things from serialaggregator
     # We don't care about allowing the user to supply their username/password
     # because this script is only ever to be used directly on 
     # (dev)toulouse.iot-lab.info SSH frontend, where these are supplied as
     # environment variables
-    opts = SerialAggregator.parser.parse_args("")
+    opts = SerialAggregator.parser.parse_args(['--id', os.environ['EXP_ID']] if 'EXP_ID' in os.environ else '')
     nodes_list = SerialAggregator.select_nodes(opts)
     
 
     bridge = mqttSerialBridge(nodes_list, args.broker, username=args.username, password=args.password, IDMap=mapping, port=args.port, verbose = args.verbose, topicRoot=args.topic_root)
     bridge.loop_forever()
```

### Comparing `locura_iotlab_bridge-0.1.6/locura_iotlab_bridge/helpers.py` & `locura_iotlab_bridge-0.1.7/locura_iotlab_bridge/helpers.py`

 * *Files identical despite different names*

### Comparing `locura_iotlab_bridge-0.1.6/LICENSE` & `locura_iotlab_bridge-0.1.7/LICENSE`

 * *Files identical despite different names*

