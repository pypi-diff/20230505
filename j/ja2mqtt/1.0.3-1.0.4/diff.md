# Comparing `tmp/ja2mqtt-1.0.3.tar.gz` & `tmp/ja2mqtt-1.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ja2mqtt-1.0.3.tar", last modified: Sat Apr 22 00:02:10 2023, max compression
+gzip compressed data, was "ja2mqtt-1.0.4.tar", last modified: Fri May  5 20:53:35 2023, max compression
```

## Comparing `ja2mqtt-1.0.3.tar` & `ja2mqtt-1.0.4.tar`

### file list

```diff
@@ -1,45 +1,48 @@
-drwxr-xr-x   0 tomas      (501) staff       (20)        0 2023-04-22 00:02:10.907639 ja2mqtt-1.0.3/
--rw-r--r--   0 tomas      (501) staff       (20)      108 2023-04-18 13:03:48.000000 ja2mqtt-1.0.3/MANIFEST.in
--rw-r--r--   0 tomas      (501) staff       (20)     1995 2023-04-22 00:02:10.907469 ja2mqtt-1.0.3/PKG-INFO
--rw-r--r--   0 tomas      (501) staff       (20)     1650 2023-04-18 13:03:48.000000 ja2mqtt-1.0.3/README-pypi.text
--rw-r--r--   0 tomas      (501) staff       (20)     5128 2023-04-22 00:01:53.000000 ja2mqtt-1.0.3/README.md
-drwxr-xr-x   0 tomas      (501) staff       (20)        0 2023-04-22 00:02:10.903641 ja2mqtt-1.0.3/bin/
--rwxr-xr-x   0 tomas      (501) staff       (20)      345 2023-04-17 22:42:29.000000 ja2mqtt-1.0.3/bin/env.sh
--rwxr-xr-x   0 tomas      (501) staff       (20)       31 2023-04-17 22:42:29.000000 ja2mqtt-1.0.3/bin/ja2mqtt
--rw-r--r--   0 tomas      (501) staff       (20)      107 2023-04-20 19:55:01.000000 ja2mqtt-1.0.3/bin/requirements-dev.txt
--rwxr-xr-x   0 tomas      (501) staff       (20)      700 2023-04-20 19:55:01.000000 ja2mqtt-1.0.3/bin/requirements-setup-py.sh
--rw-r--r--   0 tomas      (501) staff       (20)       70 2023-04-20 19:55:01.000000 ja2mqtt-1.0.3/bin/requirements.txt
-drwxr-xr-x   0 tomas      (501) staff       (20)        0 2023-04-22 00:02:10.904060 ja2mqtt-1.0.3/config/
--rw-r--r--   0 tomas      (501) staff       (20)     3916 2023-04-22 00:01:53.000000 ja2mqtt-1.0.3/config/ja2mqtt.yaml
--rw-r--r--   0 tomas      (501) staff       (20)     2024 2023-04-22 00:01:53.000000 ja2mqtt-1.0.3/config/sample-config.yaml
-drwxr-xr-x   0 tomas      (501) staff       (20)        0 2023-04-22 00:02:10.904456 ja2mqtt-1.0.3/docker/
--rw-r--r--   0 tomas      (501) staff       (20)      975 2023-04-20 19:55:01.000000 ja2mqtt-1.0.3/docker/Dockerfile
--rw-r--r--   0 tomas      (501) staff       (20)      299 2023-04-18 22:48:03.000000 ja2mqtt-1.0.3/docker/docker-compose.yaml
-drwxr-xr-x   0 tomas      (501) staff       (20)        0 2023-04-22 00:02:10.904785 ja2mqtt-1.0.3/docker/mqtt-config/
--rw-r--r--   0 tomas      (501) staff       (20)    40475 2023-04-17 22:42:29.000000 ja2mqtt-1.0.3/docker/mqtt-config/mosquitto.conf
-drwxr-xr-x   0 tomas      (501) staff       (20)        0 2023-04-22 00:02:10.905394 ja2mqtt-1.0.3/ja2mqtt/
--rwxr-xr-x   0 tomas      (501) staff       (20)      167 2023-04-22 00:01:53.000000 ja2mqtt-1.0.3/ja2mqtt/__init__.py
--rw-r--r--   0 tomas      (501) staff       (20)      251 2023-04-22 00:01:53.000000 ja2mqtt-1.0.3/ja2mqtt/__main__.py
-drwxr-xr-x   0 tomas      (501) staff       (20)        0 2023-04-22 00:02:10.906699 ja2mqtt-1.0.3/ja2mqtt/commands/
--rw-r--r--   0 tomas      (501) staff       (20)     1951 2023-04-22 00:01:53.000000 ja2mqtt-1.0.3/ja2mqtt/commands/__init__.py
--rw-r--r--   0 tomas      (501) staff       (20)     1828 2023-04-22 00:01:53.000000 ja2mqtt-1.0.3/ja2mqtt/commands/config.py
--rw-r--r--   0 tomas      (501) staff       (20)     1859 2023-04-22 00:01:53.000000 ja2mqtt-1.0.3/ja2mqtt/commands/ja2mqtt.py
--rw-r--r--   0 tomas      (501) staff       (20)      987 2023-04-22 00:01:53.000000 ja2mqtt-1.0.3/ja2mqtt/commands/run.py
--rw-r--r--   0 tomas      (501) staff       (20)     2552 2023-04-22 00:01:53.000000 ja2mqtt-1.0.3/ja2mqtt/commands/test.py
-drwxr-xr-x   0 tomas      (501) staff       (20)        0 2023-04-22 00:02:10.907257 ja2mqtt-1.0.3/ja2mqtt/components/
--rw-r--r--   0 tomas      (501) staff       (20)      819 2023-04-22 00:01:53.000000 ja2mqtt-1.0.3/ja2mqtt/components/__init__.py
--rw-r--r--   0 tomas      (501) staff       (20)    11210 2023-04-22 00:01:53.000000 ja2mqtt-1.0.3/ja2mqtt/components/bridge.py
--rw-r--r--   0 tomas      (501) staff       (20)     5572 2023-04-22 00:01:53.000000 ja2mqtt-1.0.3/ja2mqtt/components/mqtt.py
--rw-r--r--   0 tomas      (501) staff       (20)     7857 2023-04-22 00:01:53.000000 ja2mqtt-1.0.3/ja2mqtt/components/serial.py
--rw-r--r--   0 tomas      (501) staff       (20)     6477 2023-04-22 00:01:53.000000 ja2mqtt-1.0.3/ja2mqtt/components/simulator.py
--rw-r--r--   0 tomas      (501) staff       (20)    13243 2023-04-22 00:01:53.000000 ja2mqtt-1.0.3/ja2mqtt/config.py
--rw-r--r--   0 tomas      (501) staff       (20)     8079 2023-04-20 19:55:01.000000 ja2mqtt-1.0.3/ja2mqtt/utils.py
-drwxr-xr-x   0 tomas      (501) staff       (20)        0 2023-04-22 00:02:10.906147 ja2mqtt-1.0.3/ja2mqtt.egg-info/
--rw-r--r--   0 tomas      (501) staff       (20)     1995 2023-04-22 00:02:10.000000 ja2mqtt-1.0.3/ja2mqtt.egg-info/PKG-INFO
--rw-r--r--   0 tomas      (501) staff       (20)      814 2023-04-22 00:02:10.000000 ja2mqtt-1.0.3/ja2mqtt.egg-info/SOURCES.txt
--rw-r--r--   0 tomas      (501) staff       (20)        1 2023-04-22 00:02:10.000000 ja2mqtt-1.0.3/ja2mqtt.egg-info/dependency_links.txt
--rw-r--r--   0 tomas      (501) staff       (20)       61 2023-04-22 00:02:10.000000 ja2mqtt-1.0.3/ja2mqtt.egg-info/entry_points.txt
--rw-r--r--   0 tomas      (501) staff       (20)       70 2023-04-22 00:02:10.000000 ja2mqtt-1.0.3/ja2mqtt.egg-info/requires.txt
--rw-r--r--   0 tomas      (501) staff       (20)        8 2023-04-22 00:02:10.000000 ja2mqtt-1.0.3/ja2mqtt.egg-info/top_level.txt
--rw-r--r--   0 tomas      (501) staff       (20)       38 2023-04-22 00:02:10.907680 ja2mqtt-1.0.3/setup.cfg
--rw-r--r--   0 tomas      (501) staff       (20)     1589 2023-04-22 00:01:53.000000 ja2mqtt-1.0.3/setup.py
+drwxr-xr-x   0 tomas      (501) staff       (20)        0 2023-05-05 20:53:35.625080 ja2mqtt-1.0.4/
+-rw-r--r--   0 tomas      (501) staff       (20)     1069 2023-05-03 21:57:45.000000 ja2mqtt-1.0.4/LICENSE
+-rw-r--r--   0 tomas      (501) staff       (20)      143 2023-05-03 21:57:45.000000 ja2mqtt-1.0.4/MANIFEST.in
+-rw-r--r--   0 tomas      (501) staff       (20)     2017 2023-05-05 20:53:35.624939 ja2mqtt-1.0.4/PKG-INFO
+-rw-r--r--   0 tomas      (501) staff       (20)     1650 2023-05-03 21:57:45.000000 ja2mqtt-1.0.4/README-pypi.text
+-rw-r--r--   0 tomas      (501) staff       (20)     4375 2023-05-05 20:48:52.000000 ja2mqtt-1.0.4/README.md
+drwxr-xr-x   0 tomas      (501) staff       (20)        0 2023-05-05 20:53:35.615368 ja2mqtt-1.0.4/bin/
+-rwxr-xr-x   0 tomas      (501) staff       (20)      345 2023-05-05 18:31:56.000000 ja2mqtt-1.0.4/bin/env.sh
+-rwxr-xr-x   0 tomas      (501) staff       (20)       31 2023-05-03 21:57:45.000000 ja2mqtt-1.0.4/bin/ja2mqtt
+-rw-r--r--   0 tomas      (501) staff       (20)      107 2023-05-03 21:57:45.000000 ja2mqtt-1.0.4/bin/requirements-dev.txt
+-rwxr-xr-x   0 tomas      (501) staff       (20)      700 2023-05-03 21:57:45.000000 ja2mqtt-1.0.4/bin/requirements-setup-py.sh
+-rw-r--r--   0 tomas      (501) staff       (20)      118 2023-05-05 20:51:46.000000 ja2mqtt-1.0.4/bin/requirements.txt
+drwxr-xr-x   0 tomas      (501) staff       (20)        0 2023-05-05 20:53:35.615572 ja2mqtt-1.0.4/config/
+-rw-r--r--   0 tomas      (501) staff       (20)     3956 2023-04-30 23:14:11.000000 ja2mqtt-1.0.4/config/ja2mqtt.yaml
+-rw-r--r--   0 tomas      (501) staff       (20)     2024 2023-04-22 00:01:53.000000 ja2mqtt-1.0.4/config/sample-config.yaml
+drwxr-xr-x   0 tomas      (501) staff       (20)        0 2023-05-05 20:53:35.615895 ja2mqtt-1.0.4/docker/
+-rw-r--r--   0 tomas      (501) staff       (20)      975 2023-04-20 19:55:01.000000 ja2mqtt-1.0.4/docker/Dockerfile
+-rw-r--r--   0 tomas      (501) staff       (20)      299 2023-04-18 22:48:03.000000 ja2mqtt-1.0.4/docker/docker-compose.yaml
+drwxr-xr-x   0 tomas      (501) staff       (20)        0 2023-05-05 20:53:35.616028 ja2mqtt-1.0.4/docker/mqtt-config/
+-rw-r--r--   0 tomas      (501) staff       (20)    40475 2023-04-17 22:42:29.000000 ja2mqtt-1.0.4/docker/mqtt-config/mosquitto.conf
+drwxr-xr-x   0 tomas      (501) staff       (20)        0 2023-05-05 20:53:35.616572 ja2mqtt-1.0.4/ja2mqtt/
+-rwxr-xr-x   0 tomas      (501) staff       (20)      167 2023-05-05 20:49:44.000000 ja2mqtt-1.0.4/ja2mqtt/__init__.py
+-rw-r--r--   0 tomas      (501) staff       (20)      251 2023-04-22 00:01:53.000000 ja2mqtt-1.0.4/ja2mqtt/__main__.py
+drwxr-xr-x   0 tomas      (501) staff       (20)        0 2023-05-05 20:53:35.617763 ja2mqtt-1.0.4/ja2mqtt/commands/
+-rw-r--r--   0 tomas      (501) staff       (20)     2192 2023-05-04 21:44:40.000000 ja2mqtt-1.0.4/ja2mqtt/commands/__init__.py
+-rw-r--r--   0 tomas      (501) staff       (20)     2301 2023-05-04 21:45:06.000000 ja2mqtt-1.0.4/ja2mqtt/commands/config.py
+-rw-r--r--   0 tomas      (501) staff       (20)     1859 2023-04-22 00:01:53.000000 ja2mqtt-1.0.4/ja2mqtt/commands/ja2mqtt.py
+-rw-r--r--   0 tomas      (501) staff       (20)     1208 2023-04-30 22:17:24.000000 ja2mqtt-1.0.4/ja2mqtt/commands/run.py
+-rw-r--r--   0 tomas      (501) staff       (20)     2552 2023-04-22 00:01:53.000000 ja2mqtt-1.0.4/ja2mqtt/commands/test.py
+drwxr-xr-x   0 tomas      (501) staff       (20)        0 2023-05-05 20:53:35.624615 ja2mqtt-1.0.4/ja2mqtt/components/
+-rw-r--r--   0 tomas      (501) staff       (20)      819 2023-04-22 00:01:53.000000 ja2mqtt-1.0.4/ja2mqtt/components/__init__.py
+-rw-r--r--   0 tomas      (501) staff       (20)    11210 2023-04-22 00:01:53.000000 ja2mqtt-1.0.4/ja2mqtt/components/bridge.py
+-rw-r--r--   0 tomas      (501) staff       (20)     5572 2023-04-22 00:01:53.000000 ja2mqtt-1.0.4/ja2mqtt/components/mqtt.py
+-rw-r--r--   0 tomas      (501) staff       (20)     7854 2023-04-30 22:20:40.000000 ja2mqtt-1.0.4/ja2mqtt/components/serial.py
+-rw-r--r--   0 tomas      (501) staff       (20)     6477 2023-04-22 00:01:53.000000 ja2mqtt-1.0.4/ja2mqtt/components/simulator.py
+-rw-r--r--   0 tomas      (501) staff       (20)    15442 2023-05-04 21:44:24.000000 ja2mqtt-1.0.4/ja2mqtt/config.py
+drwxr-xr-x   0 tomas      (501) staff       (20)        0 2023-05-05 20:53:35.624745 ja2mqtt-1.0.4/ja2mqtt/schemas/
+-rw-r--r--   0 tomas      (501) staff       (20)     3030 2023-04-30 22:00:50.000000 ja2mqtt-1.0.4/ja2mqtt/schemas/config-schema.yaml
+-rw-r--r--   0 tomas      (501) staff       (20)     8079 2023-04-20 19:55:01.000000 ja2mqtt-1.0.4/ja2mqtt/utils.py
+drwxr-xr-x   0 tomas      (501) staff       (20)        0 2023-05-05 20:53:35.617251 ja2mqtt-1.0.4/ja2mqtt.egg-info/
+-rw-r--r--   0 tomas      (501) staff       (20)     2017 2023-05-05 20:53:35.000000 ja2mqtt-1.0.4/ja2mqtt.egg-info/PKG-INFO
+-rw-r--r--   0 tomas      (501) staff       (20)      857 2023-05-05 20:53:35.000000 ja2mqtt-1.0.4/ja2mqtt.egg-info/SOURCES.txt
+-rw-r--r--   0 tomas      (501) staff       (20)        1 2023-05-05 20:53:35.000000 ja2mqtt-1.0.4/ja2mqtt.egg-info/dependency_links.txt
+-rw-r--r--   0 tomas      (501) staff       (20)       61 2023-05-05 20:53:35.000000 ja2mqtt-1.0.4/ja2mqtt.egg-info/entry_points.txt
+-rw-r--r--   0 tomas      (501) staff       (20)       89 2023-05-05 20:53:35.000000 ja2mqtt-1.0.4/ja2mqtt.egg-info/requires.txt
+-rw-r--r--   0 tomas      (501) staff       (20)        8 2023-05-05 20:53:35.000000 ja2mqtt-1.0.4/ja2mqtt.egg-info/top_level.txt
+-rw-r--r--   0 tomas      (501) staff       (20)       38 2023-05-05 20:53:35.625113 ja2mqtt-1.0.4/setup.cfg
+-rw-r--r--   0 tomas      (501) staff       (20)     1615 2023-05-03 21:58:21.000000 ja2mqtt-1.0.4/setup.py
```

### Comparing `ja2mqtt-1.0.3/PKG-INFO` & `ja2mqtt-1.0.4/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 Metadata-Version: 2.1
 Name: ja2mqtt
-Version: 1.0.3
+Version: 1.0.4
 Summary: Jablotron MQTT bridge
 Author: Tomas Vitvar
 Author-email: tomas@vitvar.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3.7
 Requires-Python: >=3.6.0
+License-File: LICENSE
 
 ja2mqtt is a bridge that connects a Jablotron control unit, extended with the [JA-121T RS-485 bus interface](https://www.jablotron.com/en/produkt/rs-485-bus-interface-426/), to an MQTT broker.
 
 ja2mqtt enables the use of MQTT events to control Jablotron events, allowing for seamless integration with MQTT-based IoT systems and platforms. With this bridge, Jablotron alarms can be integrated into a larger IoT ecosystem, alongside other devices that use industry-standard protocols like ZigBee or MQTT. For example, by using ja2mqtt in conjunction with ZigBee2MQTT, Jablotron alarms and ZigBee devices can be connected in a single network and integrated with other systems such as Alexa, Tahoma, or Google Assistant, providing a unified and interoperable smart home or industrial automation solution.
 
 ja2mqtt reads input from the JA-121T serial interface, converts it into MQTT events, and publishes them to the MQTT broker using defined MQTT topics. It utilizes a ja2mqtt definition file that outlines the implementation of the JA-121T protocol. Additionally, ja2mqtt defines MQTT events that can be converted into input for the JA-121T serial interface, such as changing the state of a section to ARMED or READY. Each MQTT request may contain a correlation ID that is copied to the corresponding generated MQTT event.
```

### Comparing `ja2mqtt-1.0.3/README-pypi.text` & `ja2mqtt-1.0.4/README-pypi.text`

 * *Files identical despite different names*

### Comparing `ja2mqtt-1.0.3/README.md` & `ja2mqtt-1.0.4/README.md`

 * *Files 24% similar despite different names*

```diff
@@ -1,31 +1,68 @@
 # $ ja2mqtt
 
+[![](https://img.shields.io/pypi/v/ja2mqtt.svg)](https://pypi.org/project/ja2mqtt/)
+
+<!-- start elevator-pitch -->
+
 ja2mqtt is a bridge that connects a Jablotron control unit, extended with the [JA-121T RS-485 bus interface](https://www.jablotron.com/en/produkt/rs-485-bus-interface-426/), to an MQTT broker.
 
-ja2mqtt reads input from the JA-121T serial interface, converts it into MQTT events, and publishes them to the MQTT broker using defined MQTT topics. It utilizes a ja2mqtt definition file that outlines the implementation of the JA-121T protocol. Additionally, ja2mqtt defines MQTT events that can be converted into input for the JA-121T serial interface, such as changing the state of a section to ARMED or READY. Each MQTT request may contain a correlation ID that is copied to the corresponding generated MQTT event.
+<p align="center">
+  <img src="https://docs.google.com/drawings/export/svg?id=1GINAM_3vBMGUWAl9Av3RNUfqQ2NBDTurdChcjQiTuOw" />
+</p>
+
+ja2mqtt reads input from the JA-121T serial interface, converts it into MQTT events, and publishes them to the MQTT broker using defined MQTT topics. It utilizes a ja2mqtt definition file that outlines the implementation of the JA-121T protocol. Additionally, ja2mqtt defines MQTT events that can be converted into input for the JA-121T serial interface, such as changing the state of a section to ARMED or READY.
+
+<!-- end elevator-pitch -->
 
 If you do not have access to a JA-121T interface for testing, ja2mqtt offers a simulator that can simulate the interaction with the JA-121T interface. This allows you to test and verify the functionality of ja2mqtt even without the physical JA-121T interface available.
 
+Read the [ja2mqtt documentation](https://ja2mqtt.vitvar.com) for details on how to configure, run and use ja2mqtt.  
+
 ## Features
 
-* Define Jablotron topology in the YAML configuration file, including sections with their codes, names, and peripherals' positions and names.
-* Implement declarative rules in the ja2mqtt.yaml configuration file to support the serial JA-121T protocol.
-* Read events from Jablotron, such as section arming and disarming, peripheral state changes, and convert them to MQTT events.
-* Use MQTT events to query section and peripheral states and correlate request and response MQTT events.
-* Implement automated recovery from serial interface connection failures or MQTT broker connection failures.
-* JA-121T simulator that simulates section state changes, peripheral state changes and heartbeat messages.
+<!-- start features -->
+
+* **Jablotron topology** definition in the YAML configuration file, including sections and their codes, names, and peripherals' positions, types, and names.
+* **Declarative rules** that define how JA-121T serial bus protocol is implemented.
+* Reading events from Jablotron, such as section arming and disarming, peripheral state changes, and converting them to **MQTT events**.
+* MQTT topics that clients can use to **control sections** and **retrieve section and peripheral states**.
+* **Automated recovery** of serial interface and MQTT broker connection failures.
+* **JA-121T simulator** to simulate section state changes, peripheral state changes, and heartbeat messages.
 
-## Testing using Docker
+<!-- end features -->
 
-To test ja2mqtt with the JA-121T simulator, you can utilize the ja2mqtt Docker image that comes with pre-configured settings. The simulator provides a straightforward Jablotron topology with two sections: "House" with code "1" and an initial state of "ARMED", and "Garage" with code "2" and an initial state of "READY". This topology can be used to simulate changing the state or retrieving the status of the sections. The simulator also mimics Jablotron heartbeat messages by generating "OK" messages every 10 seconds.
+## Quickstart
 
-To test ja2mqtt with the simulator, follow the steps below.
+<!-- start quickstart -->
+
+ja2mqtt requires JA-121T bus interface, however, you can test it using the simulator if you do not have one. The Docker image comes with a sample configuration that uses the simulator. The simulator provides a straightforward Jablotron topology with two sections: `House` with code `1` and an initial state of `ARMED`, and `Garage` with code `2` and an initial state of `READY`. This topology can be used to simulate changing the state or retrieving the status of the sections. The simulator also mimics peripheral state changes and Jablotron heartbeat messages by generating "OK" messages every 10 seconds.
+
+In addition, ja2mqtt requires a running instance of [MQTT broker](https://mqtt.org/). The below steps use the [Eclipse Mosquitto MQTT broker](https://mosquitto.org/) with a sample configuration. To test ja2mqtt, follow the steps below.
+
+1. In your working directory, create a sub-directory `mqtt-config` and add the [`mosquitto.conf`](https://github.com/tomvit/ja2mqtt/tree/master/docker/mqtt-config/mosquitto.conf) into it.
+
+1. Add a [`docker-compose.yaml`](https://github.com/tomvit/ja2mqtt/tree/master/docker/docker-compose.yaml) with the following content.
+
+   ```yaml
+   version: '3.0'
+   services:
+     ja2mqtt:
+       container_name: ja2mqtt
+       image: tomvit/ja2mqtt:latest
+       depends_on:
+         - mqtt-broker
+     mqtt-broker:
+       container_name: mqtt-broker
+       volumes:
+         - ./mqtt-config/mosquitto.conf:/mosquitto/config/mosquitto.conf
+       image: eclipse-mosquitto:latest
+   ```
 
-1. Run the `docker-compose.yaml` provided in the [docker](https://github.com/tomvit/ja2mqtt/tree/master/docker) directory.
+1. Run the `docker-compose.yaml`.
 
    ```
    $ docker-compose up -d
    ```
 
 2. Inspect the logs of ja2mqtt by running the following command:
 
@@ -40,33 +77,8 @@
    <-- send: ja2mqtt/section/get: {"pin": "1234", "corrid": "ca8438b82f16"}
    --> recv: ja2mqtt/section/house: {"corrid": "ca8438b82f16", "section_code": 1, "section_name": "house", "state": "ARMED"}
    --> recv: ja2mqtt/section/garage: {"corrid": "ca8438b82f16", "section_code": 2, "section_name": "garage", "state": "READY"}   
    ```
 
 4. Check the log entries in the ja2mqtt log again to see if the events were generated.
 
-## Getting Started
-
-To use ja2mqtt, you will need:
-
-* Jablotron alarms with the control unit and the JA-121T serial interface connected to a serial port on your computer. The device uses RS485 interface, which can be connected to your computer using a [USB to RS485 adapter](https://www.aliexpress.com/w/wholesale-ch340-usb-rs485.html).
-
-* A running instance of an MQTT broker. [Mosquitto](https://mosquitto.org/) is the recommended MQTT broker, but others should also work without issues. You can run the MQTT broker on the same machine as ja2mqtt, on a separate machine, or use an existing instance of MQTT broker if you have one.
-
-* Install ja2mqtt on a computer with access to the serial port where JA-121T is connected.
-
-   ```
-   $ pip install ja2mqtt
-   ```
-
-* Download the sample configuration file and ja2mqtt definition file from the [config directory](https://github.com/tomvit/ja2mqtt/tree/master/config) of the ja2mqtt GitHub repository. In the sample configuration file, you only need to define your Jablotron topology, such as section names and their numbers.
-
-## Usage
-
-ja2mqtt is a CLI that provides the following commands. You can use the `--help` option to get more information on command usage.
-
-* `run` - the main command that reads/writes data from/to the serial interface and sends/receives MQTT events.
-* `pub` - publishes MQTT events and waits for the response. It uses the correlation ID to relate the event request with the event response.
-* `config main` - shows the main configuration in JSON.
-* `config ja2mqtt` - shows the ja2mqtt definition file after Jinja2 templating is processed.
-* `config env` - shows the environment variables used by ja2mqtt. You can define the variables in your system to set defaults for ja2mqtt options.
-* `config topics` - shows publishing and subscribing topics. You can subscribe to publishing topics from your client or send subscribing topics to control the operation of your Jablotron control unit.
+<!-- end quickstart -->
```

### Comparing `ja2mqtt-1.0.3/bin/requirements-setup-py.sh` & `ja2mqtt-1.0.4/bin/requirements-setup-py.sh`

 * *Files identical despite different names*

### Comparing `ja2mqtt-1.0.3/config/ja2mqtt.yaml` & `ja2mqtt-1.0.4/config/ja2mqtt.yaml`

 * *Files 14% similar despite different names*

```diff
@@ -31,21 +31,21 @@
     write:
       heartbeat: !py data
 
     # disable correlation for this rule
     no_correlation: True
 
 # MQTT topics for sections that will be generated when events in serial output occur
-{% for k,v in topology.section.items() %}
-- name: ja2mqtt/section/{{ k }}
+{% for s in topology.section %}
+- name: ja2mqtt/section/{{ s.name }}
   rules:
-  - read: !py pattern('STATE {{ v }} (READY|ARMED_PART|ARMED|SERVICE|BLOCKED|OFF)')
+  - read: !py pattern('STATE {{ s.code }} (READY|ARMED_PART|ARMED|SERVICE|BLOCKED|OFF)')
     write:
-      section_code: {{ v }}
-      section_name: {{ k }}
+      section_code: {{ s.code }}
+      section_name: {{ s.name }}
       state: !py data.match.group(1)
 {% endfor %}
 
 {% for v in topology.peripheral if v.type in ['motion','siren','magnet','smoke'] %}
 - name: ja2mqtt/{{ v.type }}/{{ v.name }}
   rules:
   - read: !py prf_state_change({{ v['pos'] }})
@@ -92,36 +92,36 @@
 
 # get prfstate
 - name: ja2mqtt/prfstate/get
   rules:
     - write: !py write_prf_state(reset=True)
       request_ttl: 128
 
-{% for k,v in topology.section.items() %}
+{% for s in topology.section %}
 # set state to ARMED for a single section
-- name: ja2mqtt/section/{{ k }}/set
+- name: ja2mqtt/section/{{ s.name }}/set
   rules:
     - read:
         pin: !py pattern("^[0-9]{4}$")
-      write: !py format("{pin} SET {{ v }}",pin=data.pin)
+      write: !py format("{pin} SET {{ s.code }}",pin=data.pin)
 
 # set state to ARMED_PART for a single section
-- name: ja2mqtt/section/{{ k }}/setp
+- name: ja2mqtt/section/{{ s.name }}/setp
   rules:
     - read:
         pin: !py pattern("^[0-9]{4}$")
-      write: !py format("{pin} SETP {{ v }}",pin=data.pin)
+      write: !py format("{pin} SETP {{ s.code }}",pin=data.pin)
 
 # unset a single section
-- name: ja2mqtt/section/{{ k }}/unset
+- name: ja2mqtt/section/{{ s.name }}/unset
   rules:
     - read:
         pin: !py pattern("^[0-9]{4}$")
-      write: !py format("{pin} UNSET {{ v }}",pin=data.pin)
+      write: !py format("{pin} UNSET {{ s.code }}",pin=data.pin)
 
 # get state of a single section
-- name: ja2mqtt/section/{{ k }}/get
+- name: ja2mqtt/section/{{ s.name }}/get
   rules:
     - read:
         pin: !py pattern("^[0-9]{4}$")
-      write: !py format("{pin} STATE {{ v }}",pin=data.pin)
+      write: !py format("{pin} STATE {{ s.code }}",pin=data.pin)
 {% endfor %}
```

### Comparing `ja2mqtt-1.0.3/config/sample-config.yaml` & `ja2mqtt-1.0.4/config/sample-config.yaml`

 * *Files identical despite different names*

### Comparing `ja2mqtt-1.0.3/docker/Dockerfile` & `ja2mqtt-1.0.4/docker/Dockerfile`

 * *Files identical despite different names*

### Comparing `ja2mqtt-1.0.3/docker/mqtt-config/mosquitto.conf` & `ja2mqtt-1.0.4/docker/mqtt-config/mosquitto.conf`

 * *Files identical despite different names*

### Comparing `ja2mqtt-1.0.3/ja2mqtt/commands/__init__.py` & `ja2mqtt-1.0.4/ja2mqtt/commands/__init__.py`

 * *Files 8% similar despite different names*

```diff
@@ -40,18 +40,22 @@
     def init_logging(self, config):
         init_logging(
             config.get_dir_path(config.root("logs")),
             "run",
             log_level="DEBUG" if ja2mqtt_config.DEBUG else "INFO",
         )
 
+    def validate_config(self, config):
+        config.validate()
+
     def invoke(self, ctx):
         config_file = ctx.params.pop("config")
         env_file = ctx.params.pop("env")
-        config = Config(config_file, env_file)
+        config = Config(config_file, env_file, schema="config-schema.yaml")
+        self.validate_config(config)
 
         self.init_logging(config)
         log = logging.getLogger(ctx.command.name + "-loop")
         log.info(f"ja2mqtt, Jablotron JA-121 Serial MQTT bridge, version {__version__}")
 
         ctx.params["config"] = config
         ctx.params["log"] = log
@@ -62,7 +66,11 @@
     def init_logging(self, config):
         init_logging(
             config.get_dir_path(config.root("logs")),
             "run",
             log_level="DEBUG" if ja2mqtt_config.DEBUG else "INFO",
             handlers=["file"],
         )
+
+class BaseCommandLogOnlyNoValidate(BaseCommandLogOnly):
+    def validate_config(self, config):
+        pass
```

### Comparing `ja2mqtt-1.0.3/ja2mqtt/commands/config.py` & `ja2mqtt-1.0.4/ja2mqtt/commands/config.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 import os
 
 import click
 
 from ja2mqtt.config import Config, env_variables
 from ja2mqtt.utils import Map
 
-from . import BaseCommandLogOnly
+from . import BaseCommandLogOnly, BaseCommandLogOnlyNoValidate
 
 
 @click.group("config", help="Configuration commands")
 def command_config():
     pass
 
 
@@ -38,25 +38,36 @@
 def config_env():
     print("List of environment variables used by ja2mqtt:")
     print("")
     for e in env_variables:
         print(f"{e}={os.getenv(e)}")
     print("")
 
+
 @click.command("topics", help="Show MQTT topics.", cls=BaseCommandLogOnly)
 def config_topics(config, log):
     ja2mqtt_file = config.get_dir_path(config.root("ja2mqtt"))
     scope = Map(topology=config.root("topology"))
     ja2mqtt = Config(ja2mqtt_file, scope=scope, use_template=True)
 
     print("Publishing:")
     for t in ja2mqtt("serial2mqtt"):
         print(f"- {t['name']}")
     print("Subscribing:")
     for t in ja2mqtt("mqtt2serial"):
         print(f"- {t['name']}")
 
+@click.command("validate", help="Validate configuration.", cls=BaseCommandLogOnlyNoValidate)
+def config_validate(config, log):
+    res, errors = config.validate(throw_ex=False)
+    if not res:
+        click.echo("Validation failed with the following errors:")
+        for e in errors:
+            print(f"- {e.message}, in {e.json_path[2:]}")
+    else:
+        print("The configuration is valid.")
 
 command_config.add_command(config_main)
 command_config.add_command(config_ja2mqtt)
 command_config.add_command(config_env)
 command_config.add_command(config_topics)
+command_config.add_command(config_validate)
```

### Comparing `ja2mqtt-1.0.3/ja2mqtt/commands/ja2mqtt.py` & `ja2mqtt-1.0.4/ja2mqtt/commands/ja2mqtt.py`

 * *Files identical despite different names*

### Comparing `ja2mqtt-1.0.3/ja2mqtt/commands/run.py` & `ja2mqtt-1.0.4/ja2mqtt/commands/run.py`

 * *Files 22% similar despite different names*

```diff
@@ -15,15 +15,21 @@
 
 from . import BaseCommand
 
 
 @click.command("run", help="Run command.", cls=BaseCommand)
 def command_run(config, log):
     bridge = SerialMQTTBridge(config)
-    simulator = Simulator(config.get_part("simulator"), bridge.prfstate_bits)
+
+    simulator = None
+    if config("simulator") is not None:
+        simulator = Simulator(config.get_part("simulator"), bridge.prfstate_bits)
+    elif config("serial.use_simulator", False):
+        log.error("The serial interface is be simulated but the simulator configuration does not exist!")
+
     serial = Serial(config.get_part("serial"), simulator)
     mqtt = MQTT(f"ja2mqtt-client+{randomString(10)}", config.get_part("mqtt-broker"))
 
     bridge.set_mqtt(mqtt)
     bridge.set_serial(serial)
 
     for x in (mqtt, serial, bridge):
```

### Comparing `ja2mqtt-1.0.3/ja2mqtt/commands/test.py` & `ja2mqtt-1.0.4/ja2mqtt/commands/test.py`

 * *Files identical despite different names*

### Comparing `ja2mqtt-1.0.3/ja2mqtt/components/__init__.py` & `ja2mqtt-1.0.4/ja2mqtt/components/__init__.py`

 * *Files identical despite different names*

### Comparing `ja2mqtt-1.0.3/ja2mqtt/components/bridge.py` & `ja2mqtt-1.0.4/ja2mqtt/components/bridge.py`

 * *Files identical despite different names*

### Comparing `ja2mqtt-1.0.3/ja2mqtt/components/mqtt.py` & `ja2mqtt-1.0.4/ja2mqtt/components/mqtt.py`

 * *Files identical despite different names*

### Comparing `ja2mqtt-1.0.3/ja2mqtt/components/serial.py` & `ja2mqtt-1.0.4/ja2mqtt/components/serial.py`

 * *Files 0% similar despite different names*

```diff
@@ -80,26 +80,27 @@
     def __init__(self, config, simulator):
         """
         Initialize the serial object. It reads configuration parameters from the config
         and creates `ser` object that can be either `PySerial` or `Simulator` based on the
         `use_simulator` property in the configuration.
         """
         super().__init__(config, "serial")
+        self.buffer = Queue()
+        self.wait_on_ready = self.config.value_int("wait_on_ready", default=10)
         self.use_simulator = self.config.value_bool("use_simulator", default=False)
         if not self.use_simulator:
             self.ser = None
             self.port = self.config.value_str("port", required=True)
-            self.wait_on_ready = self.config.value_int("wait_on_ready", default=10)
             self.log.info(f"The serial connection configured, the port is {self.port}")
         else:
             self.port = "<simulator>"
             self.ser = simulator
             self.log.info("The serial interface events will be simulated.")
             self.log.debug(f"The simulator object is {self.ser}")
-        self.buffer = Queue()
+
 
     def create_serial(self):
         """
         Create serial object and initialize the parameters from the configuration.
         """
         self.ser = py_serial.serial_for_url(self.port, do_not_open=True)
         self.ser.baudrate = self.config.value_int("baudrate", min=0, default=9600)
```

### Comparing `ja2mqtt-1.0.3/ja2mqtt/components/simulator.py` & `ja2mqtt-1.0.4/ja2mqtt/components/simulator.py`

 * *Files identical despite different names*

### Comparing `ja2mqtt-1.0.3/ja2mqtt/config.py` & `ja2mqtt-1.0.4/ja2mqtt/config.py`

 * *Files 6% similar despite different names*

```diff
@@ -13,14 +13,20 @@
 import warnings
 from threading import Event
 
 import click
 import jinja2
 import yaml
 
+import jsonschema
+from jsonschema import validate
+from jsonschema import Draft7Validator
+
+from jsonschema.validators import extend
+
 warnings.filterwarnings("ignore", category=DeprecationWarning)
 
 import imp
 from functools import reduce
 
 from .utils import (
     Map,
@@ -48,14 +54,17 @@
 env_variables = ["JA2MQTT_DEBUG", "JA2MQTT_NO_ANSI", "JA2MQTT_CONFIG", "JA2MQTT_ENV"]
 
 ENCODING = "ascii"
 
 # global exit event
 exit_event = Event()
 
+# valid schema versions
+SCHEMA_VERSIONS = ["1.0"]
+
 
 class Jinja2TemplateLoader(jinja2.BaseLoader):
     def get_source(self, environment, template):
         if not os.path.exists(template):
             raise jinja2.TemplateNotFound(template)
         with open(template, "r", encoding="utf-8") as f:
             source = f.read()
@@ -87,14 +96,21 @@
             self.seek(0)
         except Exception as e:
             raise Exception(
                 f"Error when processing template {os.path.basename(file)}: {str(e)}"
             )
 
 
+def get_schema_file(name):
+    sfile = os.path.dirname(os.path.realpath(__file__)) + f"/schemas/{name}"
+    if not os.path.exists(sfile):
+        raise Exception(f"The schema {sfile} does not exist!")
+    return sfile
+
+
 def get_dir_path(config_dir, path, base_dir=None, check=False):
     """
     Return the directory for the path specified.
     """
     d = os.path.normpath(
         (
             ((config_dir if base_dir is None else base_dir) + "/")
@@ -194,33 +210,84 @@
         return PythonExpression(replace_env_variable(node.value))
     except Exception as e:
         raise Exception(
             'Cannot create python expression from string "%s". %s'
             % (node.value, str(e))
         )
 
-
 class Config:
     """
     The main confuguration.
     """
 
     def __init__(
-        self, file, env=None, log_level="INFO", scope=None, use_template=False
+        self,
+        file,
+        env=None,
+        schema=None,
+        log_level="INFO",
+        scope=None,
+        use_template=False,
     ):
         """
         Read and parse the configuration from the yaml file and initializes the logging.
         """
+        self.schema = None
         self.log_level = log_level
         if not (os.path.exists(file)):
             raise Exception(f"The configuration file {file} does not exist!")
         self.raw_config, self.config_file, self.config_dir = read_config(
             file, env, use_template=use_template, scope=scope
         )
         self.root = self.get_part(None)
+        if schema:
+            self.schema = read_config(
+                get_schema_file(schema), None, use_template=False
+            )[0]
+
+    def check_dupplicates(self, path):
+        _path = path.split('.')
+        _prop = _path[-1]
+        values = [x[_prop] for x in self('.'.join(_path[:-1]),[],required=False)]
+        dupplicates = list(set([x for x in values if values.count(x) > 1]))
+        if len(dupplicates) > 0:
+            raise Exception(f"There are dupplicate values in '{path}': {dupplicates}")
+
+    def validate(self, throw_ex=True):
+        def __version(c, i):
+            return i in SCHEMA_VERSIONS
+
+        def __time_condition(c, i):
+            return isinstance(i, PythonExpression) or isinstance(i, int)
+
+        def __write_expr(c, i):
+            return isinstance(i, PythonExpression) or isinstance(i, str)
+
+        type_checker = Draft7Validator.TYPE_CHECKER.redefine_many(
+            Map(
+                __version=__version,
+                __time_condition=__time_condition,
+                __write_expr=__write_expr,
+            )
+        )
+        ConfigValidator = extend(Draft7Validator, type_checker=type_checker)
+        validator = ConfigValidator(self.schema)
+        errors = list(validator.iter_errors(self.raw_config))
+
+        if errors:
+            if throw_ex:
+                raise Exception(
+                    f"The configuration file '{self.config_file}' is not valid!"
+                )
+            return False, errors
+        else:
+            self.check_dupplicates('topology.section.code')
+            self.check_dupplicates('topology.peripheral.pos')
+            self.check_dupplicates('simulator.sections.code')
+            return True, None
 
     def get_dir_path(self, path, base_dir=None, check=False):
         """
         Return the full directory of the path with `config_dir` as the base directory.
         """
         return get_dir_path(self.config_dir, path, base_dir, check)
```

### Comparing `ja2mqtt-1.0.3/ja2mqtt/utils.py` & `ja2mqtt-1.0.4/ja2mqtt/utils.py`

 * *Files identical despite different names*

### Comparing `ja2mqtt-1.0.3/ja2mqtt.egg-info/PKG-INFO` & `ja2mqtt-1.0.4/ja2mqtt.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 Metadata-Version: 2.1
 Name: ja2mqtt
-Version: 1.0.3
+Version: 1.0.4
 Summary: Jablotron MQTT bridge
 Author: Tomas Vitvar
 Author-email: tomas@vitvar.com
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3.7
 Requires-Python: >=3.6.0
+License-File: LICENSE
 
 ja2mqtt is a bridge that connects a Jablotron control unit, extended with the [JA-121T RS-485 bus interface](https://www.jablotron.com/en/produkt/rs-485-bus-interface-426/), to an MQTT broker.
 
 ja2mqtt enables the use of MQTT events to control Jablotron events, allowing for seamless integration with MQTT-based IoT systems and platforms. With this bridge, Jablotron alarms can be integrated into a larger IoT ecosystem, alongside other devices that use industry-standard protocols like ZigBee or MQTT. For example, by using ja2mqtt in conjunction with ZigBee2MQTT, Jablotron alarms and ZigBee devices can be connected in a single network and integrated with other systems such as Alexa, Tahoma, or Google Assistant, providing a unified and interoperable smart home or industrial automation solution.
 
 ja2mqtt reads input from the JA-121T serial interface, converts it into MQTT events, and publishes them to the MQTT broker using defined MQTT topics. It utilizes a ja2mqtt definition file that outlines the implementation of the JA-121T protocol. Additionally, ja2mqtt defines MQTT events that can be converted into input for the JA-121T serial interface, such as changing the state of a section to ARMED or READY. Each MQTT request may contain a correlation ID that is copied to the corresponding generated MQTT event.
```

### Comparing `ja2mqtt-1.0.3/ja2mqtt.egg-info/SOURCES.txt` & `ja2mqtt-1.0.4/ja2mqtt.egg-info/SOURCES.txt`

 * *Files 21% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+LICENSE
 MANIFEST.in
 README-pypi.text
 README.md
 setup.py
 bin/env.sh
 bin/ja2mqtt
 bin/requirements-dev.txt
@@ -27,8 +28,9 @@
 ja2mqtt/commands/ja2mqtt.py
 ja2mqtt/commands/run.py
 ja2mqtt/commands/test.py
 ja2mqtt/components/__init__.py
 ja2mqtt/components/bridge.py
 ja2mqtt/components/mqtt.py
 ja2mqtt/components/serial.py
-ja2mqtt/components/simulator.py
+ja2mqtt/components/simulator.py
+ja2mqtt/schemas/config-schema.yaml
```

### Comparing `ja2mqtt-1.0.3/setup.py` & `ja2mqtt-1.0.4/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -29,15 +29,16 @@
 # setup main
 # required modules
 install_requires = [
     'click>=8.0.4',
     'Jinja2>=3.0.3',
     'paho-mqtt>=1.6.1',
     'pyserial>=3.5',
-    'PyYAML>=6.0'
+    'PyYAML>=6.0',
+    'jsonschema>=4.17.3'
 ]
 
 setup(
     name='ja2mqtt',
     version=__version__,
     description='Jablotron MQTT bridge',
     long_description=read('README-pypi.text'),
```

