# Comparing `tmp/durin-0.0.75.tar.gz` & `tmp/durin-0.0.76.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "durin-0.0.75.tar", last modified: Thu Apr  6 15:36:30 2023, max compression
+gzip compressed data, was "durin-0.0.76.tar", last modified: Fri May  5 09:17:32 2023, max compression
```

## Comparing `durin-0.0.75.tar` & `durin-0.0.76.tar`

### file list

```diff
@@ -1,51 +1,51 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 15:36:30.303285 durin-0.0.75/
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-04-06 15:36:21.000000 durin-0.0.75/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2929 2023-04-06 15:36:30.303285 durin-0.0.75/PKG-INFO
--rwxr-xr-x   0 runner    (1001) docker     (123)     2683 2023-04-06 15:36:21.000000 durin-0.0.75/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 15:36:30.299285 durin-0.0.75/bin/
--rwxr-xr-x   0 runner    (1001) docker     (123)       34 2023-04-06 15:36:21.000000 durin-0.0.75/bin/durin
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 15:36:30.299285 durin-0.0.75/durin/
--rw-r--r--   0 runner    (1001) docker     (123)      368 2023-04-06 15:36:21.000000 durin-0.0.75/durin/Profiler.py
--rw-r--r--   0 runner    (1001) docker     (123)      290 2023-04-06 15:36:21.000000 durin-0.0.75/durin/Read_profilers.py
--rwxr-xr-x   0 runner    (1001) docker     (123)       80 2023-04-06 15:36:21.000000 durin-0.0.75/durin/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      475 2023-04-06 15:36:21.000000 durin-0.0.75/durin/__main__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      766 2023-04-06 15:36:21.000000 durin-0.0.75/durin/actuator.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4148 2023-04-06 15:36:21.000000 durin-0.0.75/durin/cli.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 15:36:30.299285 durin-0.0.75/durin/controller/
--rwxr-xr-x   0 runner    (1001) docker     (123)       40 2023-04-06 15:36:21.000000 durin-0.0.75/durin/controller/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      344 2023-04-06 15:36:21.000000 durin-0.0.75/durin/controller/dvs.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4307 2023-04-06 15:36:21.000000 durin-0.0.75/durin/controller/server.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 15:36:30.303285 durin-0.0.75/durin/controller/test/
--rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 15:36:21.000000 durin-0.0.75/durin/controller/test/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      947 2023-04-06 15:36:21.000000 durin-0.0.75/durin/controller/test/test_stream.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4694 2023-04-06 15:36:21.000000 durin-0.0.75/durin/durin.py
--rwxr-xr-x   0 runner    (1001) docker     (123)   181742 2023-04-06 15:36:21.000000 durin-0.0.75/durin/durin_birdseye.jpg
--rwxr-xr-x   0 runner    (1001) docker     (123)      504 2023-04-06 15:36:21.000000 durin-0.0.75/durin/dvs.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 15:36:30.303285 durin-0.0.75/durin/examples/
--rw-r--r--   0 runner    (1001) docker     (123)      193 2023-04-06 15:36:21.000000 durin-0.0.75/durin/examples/CPU_test.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-06 15:36:21.000000 durin-0.0.75/durin/examples/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2281 2023-04-06 15:36:21.000000 durin-0.0.75/durin/examples/braitenberg.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     2631 2023-04-06 15:36:21.000000 durin-0.0.75/durin/examples/commands.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1459 2023-04-06 15:36:21.000000 durin-0.0.75/durin/examples/dashboard.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      923 2023-04-06 15:36:21.000000 durin-0.0.75/durin/examples/main.py
--rw-r--r--   0 runner    (1001) docker     (123)     1232 2023-04-06 15:36:21.000000 durin-0.0.75/durin/examples/plot.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      589 2023-04-06 15:36:21.000000 durin-0.0.75/durin/examples/record.py
--rw-r--r--   0 runner    (1001) docker     (123)     2865 2023-04-06 15:36:21.000000 durin-0.0.75/durin/examples/stats.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 15:36:30.303285 durin-0.0.75/durin/io/
--rwxr-xr-x   0 runner    (1001) docker     (123)      673 2023-04-06 15:36:21.000000 durin-0.0.75/durin/io/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5073 2023-04-06 15:36:21.000000 durin-0.0.75/durin/io/command.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1442 2023-04-06 15:36:21.000000 durin-0.0.75/durin/io/gamepad.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     6181 2023-04-06 15:36:21.000000 durin-0.0.75/durin/io/network.py
--rwxr-xr-x   0 runner    (1001) docker     (123)      525 2023-04-06 15:36:21.000000 durin-0.0.75/durin/io/ringbuffer.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     1824 2023-04-06 15:36:21.000000 durin-0.0.75/durin/io/runnable.py
--rw-r--r--   0 runner    (1001) docker     (123)     9042 2023-04-06 15:36:21.000000 durin-0.0.75/durin/io/schema.capnp
--rwxr-xr-x   0 runner    (1001) docker     (123)     7102 2023-04-06 15:36:21.000000 durin-0.0.75/durin/sensor.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    13631 2023-04-06 15:36:21.000000 durin-0.0.75/durin/ui.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-06 15:36:30.299285 durin-0.0.75/durin.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2929 2023-04-06 15:36:30.000000 durin-0.0.75/durin.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      906 2023-04-06 15:36:30.000000 durin-0.0.75/durin.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-06 15:36:30.000000 durin-0.0.75/durin.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       55 2023-04-06 15:36:30.000000 durin-0.0.75/durin.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-06 15:36:30.000000 durin-0.0.75/durin.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-06 15:36:30.303285 durin-0.0.75/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)      663 2023-04-06 15:36:21.000000 durin-0.0.75/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 09:17:32.362083 durin-0.0.76/
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-05-05 09:17:23.000000 durin-0.0.76/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2929 2023-05-05 09:17:32.362083 durin-0.0.76/PKG-INFO
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2683 2023-05-05 09:17:23.000000 durin-0.0.76/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 09:17:32.358083 durin-0.0.76/bin/
+-rwxr-xr-x   0 runner    (1001) docker     (123)       34 2023-05-05 09:17:23.000000 durin-0.0.76/bin/durin
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 09:17:32.358083 durin-0.0.76/durin/
+-rw-r--r--   0 runner    (1001) docker     (123)      368 2023-05-05 09:17:23.000000 durin-0.0.76/durin/Profiler.py
+-rw-r--r--   0 runner    (1001) docker     (123)      290 2023-05-05 09:17:23.000000 durin-0.0.76/durin/Read_profilers.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)       80 2023-05-05 09:17:23.000000 durin-0.0.76/durin/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      475 2023-05-05 09:17:23.000000 durin-0.0.76/durin/__main__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      766 2023-05-05 09:17:23.000000 durin-0.0.76/durin/actuator.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4148 2023-05-05 09:17:23.000000 durin-0.0.76/durin/cli.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 09:17:32.362083 durin-0.0.76/durin/controller/
+-rwxr-xr-x   0 runner    (1001) docker     (123)       40 2023-05-05 09:17:23.000000 durin-0.0.76/durin/controller/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      344 2023-05-05 09:17:23.000000 durin-0.0.76/durin/controller/dvs.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4307 2023-05-05 09:17:23.000000 durin-0.0.76/durin/controller/server.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 09:17:32.362083 durin-0.0.76/durin/controller/test/
+-rwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 09:17:23.000000 durin-0.0.76/durin/controller/test/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      947 2023-05-05 09:17:23.000000 durin-0.0.76/durin/controller/test/test_stream.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4694 2023-05-05 09:17:23.000000 durin-0.0.76/durin/durin.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)   181742 2023-05-05 09:17:23.000000 durin-0.0.76/durin/durin_birdseye.jpg
+-rwxr-xr-x   0 runner    (1001) docker     (123)      504 2023-05-05 09:17:23.000000 durin-0.0.76/durin/dvs.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 09:17:32.362083 durin-0.0.76/durin/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)      193 2023-05-05 09:17:23.000000 durin-0.0.76/durin/examples/CPU_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 09:17:23.000000 durin-0.0.76/durin/examples/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2281 2023-05-05 09:17:23.000000 durin-0.0.76/durin/examples/braitenberg.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     2631 2023-05-05 09:17:23.000000 durin-0.0.76/durin/examples/commands.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1459 2023-05-05 09:17:23.000000 durin-0.0.76/durin/examples/dashboard.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      923 2023-05-05 09:17:23.000000 durin-0.0.76/durin/examples/main.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1232 2023-05-05 09:17:23.000000 durin-0.0.76/durin/examples/plot.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      589 2023-05-05 09:17:23.000000 durin-0.0.76/durin/examples/record.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2865 2023-05-05 09:17:23.000000 durin-0.0.76/durin/examples/stats.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 09:17:32.362083 durin-0.0.76/durin/io/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      673 2023-05-05 09:17:23.000000 durin-0.0.76/durin/io/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5073 2023-05-05 09:17:23.000000 durin-0.0.76/durin/io/command.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1442 2023-05-05 09:17:23.000000 durin-0.0.76/durin/io/gamepad.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     6181 2023-05-05 09:17:23.000000 durin-0.0.76/durin/io/network.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)      525 2023-05-05 09:17:23.000000 durin-0.0.76/durin/io/ringbuffer.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     1824 2023-05-05 09:17:23.000000 durin-0.0.76/durin/io/runnable.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9042 2023-05-05 09:17:23.000000 durin-0.0.76/durin/io/schema.capnp
+-rwxr-xr-x   0 runner    (1001) docker     (123)     7102 2023-05-05 09:17:23.000000 durin-0.0.76/durin/sensor.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    14526 2023-05-05 09:17:23.000000 durin-0.0.76/durin/ui.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 09:17:32.358083 durin-0.0.76/durin.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2929 2023-05-05 09:17:32.000000 durin-0.0.76/durin.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      906 2023-05-05 09:17:32.000000 durin-0.0.76/durin.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 09:17:32.000000 durin-0.0.76/durin.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       55 2023-05-05 09:17:32.000000 durin-0.0.76/durin.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-05 09:17:32.000000 durin-0.0.76/durin.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-05 09:17:32.362083 durin-0.0.76/setup.cfg
+-rwxr-xr-x   0 runner    (1001) docker     (123)      663 2023-05-05 09:17:23.000000 durin-0.0.76/setup.py
```

### Comparing `durin-0.0.75/PKG-INFO` & `durin-0.0.76/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: durin
-Version: 0.0.75
+Version: 0.0.76
 Summary: Python control interface for the Durin robot
 Maintainer: Jens E. Pedersen
 Maintainer-email: jeped@kth.se
 License: LGPLv3
 Description-Content-Type: text/markdown
 Provides-Extra: aestream
```

### Comparing `durin-0.0.75/README.md` & `durin-0.0.76/README.md`

 * *Files identical despite different names*

### Comparing `durin-0.0.75/durin/actuator.py` & `durin-0.0.76/durin/actuator.py`

 * *Files identical despite different names*

### Comparing `durin-0.0.75/durin/cli.py` & `durin-0.0.76/durin/cli.py`

 * *Files identical despite different names*

### Comparing `durin-0.0.75/durin/controller/server.py` & `durin-0.0.76/durin/controller/server.py`

 * *Files identical despite different names*

### Comparing `durin-0.0.75/durin/controller/test/test_stream.py` & `durin-0.0.76/durin/controller/test/test_stream.py`

 * *Files identical despite different names*

### Comparing `durin-0.0.75/durin/durin.py` & `durin-0.0.76/durin/durin.py`

 * *Files identical despite different names*

### Comparing `durin-0.0.75/durin/durin_birdseye.jpg` & `durin-0.0.76/durin/durin_birdseye.jpg`

 * *Files identical despite different names*

### Comparing `durin-0.0.75/durin/examples/braitenberg.py` & `durin-0.0.76/durin/examples/braitenberg.py`

 * *Files identical despite different names*

### Comparing `durin-0.0.75/durin/examples/commands.py` & `durin-0.0.76/durin/examples/commands.py`

 * *Files identical despite different names*

### Comparing `durin-0.0.75/durin/examples/dashboard.py` & `durin-0.0.76/durin/examples/dashboard.py`

 * *Files identical despite different names*

### Comparing `durin-0.0.75/durin/examples/main.py` & `durin-0.0.76/durin/examples/main.py`

 * *Files identical despite different names*

### Comparing `durin-0.0.75/durin/examples/plot.py` & `durin-0.0.76/durin/examples/plot.py`

 * *Files identical despite different names*

### Comparing `durin-0.0.75/durin/examples/record.py` & `durin-0.0.76/durin/examples/record.py`

 * *Files identical despite different names*

### Comparing `durin-0.0.75/durin/examples/stats.py` & `durin-0.0.76/durin/examples/stats.py`

 * *Files identical despite different names*

### Comparing `durin-0.0.75/durin/io/__init__.py` & `durin-0.0.76/durin/io/__init__.py`

 * *Files identical despite different names*

### Comparing `durin-0.0.75/durin/io/command.py` & `durin-0.0.76/durin/io/command.py`

 * *Files identical despite different names*

### Comparing `durin-0.0.75/durin/io/gamepad.py` & `durin-0.0.76/durin/io/gamepad.py`

 * *Files identical despite different names*

### Comparing `durin-0.0.75/durin/io/network.py` & `durin-0.0.76/durin/io/network.py`

 * *Files identical despite different names*

### Comparing `durin-0.0.75/durin/io/ringbuffer.py` & `durin-0.0.76/durin/io/ringbuffer.py`

 * *Files identical despite different names*

### Comparing `durin-0.0.75/durin/io/runnable.py` & `durin-0.0.76/durin/io/runnable.py`

 * *Files identical despite different names*

### Comparing `durin-0.0.75/durin/io/schema.capnp` & `durin-0.0.76/durin/io/schema.capnp`

 * *Files identical despite different names*

### Comparing `durin-0.0.75/durin/sensor.py` & `durin-0.0.76/durin/sensor.py`

 * *Files identical despite different names*

### Comparing `durin-0.0.75/durin/ui.py` & `durin-0.0.76/durin/ui.py`

 * *Files 8% similar despite different names*

```diff
@@ -11,26 +11,26 @@
 
 from durin.durin import Durin
 from durin.io.gamepad import Gamepad
 from durin import SetSensorPeriod, GetSystemInfo, EnableTofStatus
 
 
 # Constants
-surface_width = 200
+surface_width = 300
 surface_height = 200
 sleep_interval = 0.02
 
 SENSOR_PLACEMENTS = [
     (0.25, 0.01),
     (0.02, 0.03),
     (0.02, 0.4),
     (0.02, 0.7),
-    (0.25, 0.78),
+    (0.25, 0.76),
     (0.41, 0.7),
-    (0.47, 0.4),
+    (0.45, 0.4),
     (0.41, 0.02),
 ]
 
 SENSOR_ROTATIONS = [0 - 90, 45 - 90, 90 - 90, 135 - 90, 180 - 90, 225 - 90, 270 - 90, 315 - 90]
 
 # A distance (in % of screen size) constant related to the layout.
 d= 0.02
@@ -186,33 +186,42 @@
         tofs = (np.tanh((obs.tof / 1000)) * 255).astype(np.int32)
 
         # Rotated surfaces
         rotated_surfaces = []
 
         for o in range(len(self.surfaces)):
             surface = self.surfaces[o]
-
-            square_size = surface_width//8
+            square_size = math.ceil(min(surface_width, surface_height) / 8)
             for i in range(8):
                 for j in range(8):
-
                     left = i * square_size
                     top = j * square_size
                     square_rect = pygame.Rect(left, top, square_size, square_size)
-
                     color_value = tofs[o][i][j]
                     color = (color_value, color_value, color_value)
                     pygame.draw.rect(surface, color, square_rect)
 
+                    status_left = i * square_size // 2 + surface_height
+                    status_top = j * square_size // 2 + surface_height / 4
+                    status_rect = pygame.Rect(status_left, status_top, math.ceil(square_size / 2), math.ceil(square_size / 2))
+                    status_color = (0, 0, 0)
+                    if obs.tof_status[o][i][j] == 0: # all good
+                        status_color = (0, 255, 0)
+                    elif obs.tof_status[o][i][j] == 1: # 50% error
+                        status_color = (255, 255, 0)
+                    elif obs.tof_status[o][i][j] == 2: # 100% error
+                        status_color = (255, 0, 0)
+                    elif obs.tof_status[o][i][j] == 3: # not updated
+                        status_color = (0, 0, 255)
+                    pygame.draw.rect(surface, status_color, status_rect)
 
             rotation_angle = SENSOR_ROTATIONS[o]
             rotated_surface = pygame.transform.rotate(surface, rotation_angle)
             rotated_surfaces.append(rotated_surface)
 
-
         for i in range(8):
             self.screen.blit(rotated_surfaces[i], (SENSOR_PLACEMENTS[i][0]*self.screen_width,SENSOR_PLACEMENTS[i][1]*self.screen_height))
 
         # Update UWB ######################
 
         uwb = obs.uwb
         #self.render_text("Becon ID\t\t\tDistance (mm)", UWB_PLACEMENT[0])
```

### Comparing `durin-0.0.75/durin.egg-info/PKG-INFO` & `durin-0.0.76/durin.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: durin
-Version: 0.0.75
+Version: 0.0.76
 Summary: Python control interface for the Durin robot
 Maintainer: Jens E. Pedersen
 Maintainer-email: jeped@kth.se
 License: LGPLv3
 Description-Content-Type: text/markdown
 Provides-Extra: aestream
```

### Comparing `durin-0.0.75/durin.egg-info/SOURCES.txt` & `durin-0.0.76/durin.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `durin-0.0.75/setup.py` & `durin-0.0.76/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     requirements = fp.read().split("\n")
 
 with open("README.md", "r") as fp:
     long_description = fp.read()
 
 setup(
     name="durin",
-    version="0.0.75",
+    version="0.0.76",
     install_requires=requirements,
     packages=find_packages(),
     license="LGPLv3",
     maintainer="Jens E. Pedersen",
     maintainer_email="jeped@kth.se",
     extras_require={"aestream": ["aestream"]},
     scripts=["bin/durin"],
```

