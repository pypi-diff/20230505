# Comparing `tmp/webcam-0.2.tar.gz` & `tmp/webcam-0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "webcam-0.2.tar", last modified: Fri May  5 08:51:00 2023, max compression
+gzip compressed data, was "webcam-0.3.tar", last modified: Fri May  5 10:57:33 2023, max compression
```

## Comparing `webcam-0.2.tar` & `webcam-0.3.tar`

### file list

```diff
@@ -1,16 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-05-05 08:51:00.386967 webcam-0.2/
--rw-rw-rw-   0        0        0     1089 2023-05-04 16:30:34.000000 webcam-0.2/LICENSE
--rw-rw-rw-   0        0        0     1311 2023-05-05 08:51:00.386967 webcam-0.2/PKG-INFO
--rw-rw-rw-   0        0        0      244 2023-05-05 08:42:27.000000 webcam-0.2/README.md
--rw-rw-rw-   0        0        0       42 2023-05-05 08:51:00.386967 webcam-0.2/setup.cfg
--rw-rw-rw-   0        0        0     1309 2023-05-05 08:50:48.000000 webcam-0.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-05 08:51:00.362988 webcam-0.2/webcam/
--rw-rw-rw-   0        0        0       28 2023-05-05 08:42:27.000000 webcam-0.2/webcam/__init__.py
--rw-rw-rw-   0        0        0     1522 2023-05-05 08:42:27.000000 webcam-0.2/webcam/_webcam_background.py
--rw-rw-rw-   0        0        0    10572 2023-05-05 08:42:27.000000 webcam-0.2/webcam/webcam.py
-drwxrwxrwx   0        0        0        0 2023-05-05 08:51:00.386967 webcam-0.2/webcam.egg-info/
--rw-rw-rw-   0        0        0     1311 2023-05-05 08:51:00.000000 webcam-0.2/webcam.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      240 2023-05-05 08:51:00.000000 webcam-0.2/webcam.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-05 08:51:00.000000 webcam-0.2/webcam.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       28 2023-05-05 08:51:00.000000 webcam-0.2/webcam.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-05-05 08:51:00.000000 webcam-0.2/webcam.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-05 10:57:33.606796 webcam-0.3/
+-rw-rw-rw-   0        0        0     1089 2023-05-04 16:30:34.000000 webcam-0.3/LICENSE
+-rw-rw-rw-   0        0        0     1311 2023-05-05 10:57:33.605920 webcam-0.3/PKG-INFO
+-rw-rw-rw-   0        0        0      244 2023-05-05 08:42:27.000000 webcam-0.3/README.md
+-rw-rw-rw-   0        0        0       42 2023-05-05 10:57:33.606796 webcam-0.3/setup.cfg
+-rw-rw-rw-   0        0        0     1309 2023-05-05 10:57:21.000000 webcam-0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-05 10:57:33.570007 webcam-0.3/webcam/
+-rw-rw-rw-   0        0        0       28 2023-05-05 08:42:27.000000 webcam-0.3/webcam/__init__.py
+-rw-rw-rw-   0        0        0     2651 2023-05-05 10:53:58.000000 webcam-0.3/webcam/_video_webcam.py
+-rw-rw-rw-   0        0        0     1812 2023-05-05 10:19:36.000000 webcam-0.3/webcam/_webcam_background.py
+-rw-rw-rw-   0        0        0    11009 2023-05-05 10:10:40.000000 webcam-0.3/webcam/webcam.py
+drwxrwxrwx   0        0        0        0 2023-05-05 10:57:33.603464 webcam-0.3/webcam.egg-info/
+-rw-rw-rw-   0        0        0     1311 2023-05-05 10:57:33.000000 webcam-0.3/webcam.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      264 2023-05-05 10:57:33.000000 webcam-0.3/webcam.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-05 10:57:33.000000 webcam-0.3/webcam.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       28 2023-05-05 10:57:33.000000 webcam-0.3/webcam.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-05-05 10:57:33.000000 webcam-0.3/webcam.egg-info/top_level.txt
```

### Comparing `webcam-0.2/LICENSE` & `webcam-0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `webcam-0.2/PKG-INFO` & `webcam-0.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: webcam
-Version: 0.2
+Version: 0.3
 Summary: A simple and convenient library to interact with webcams in Python without having to address Hardware Limitations
 Home-page: https://github.com/Eric-Canas/webcam
 Author: Eric-Canas
 Author-email: eric@ericcanas.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `webcam-0.2/setup.py` & `webcam-0.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='webcam',
-    version='0.2',
+    version='0.3',
     author='Eric-Canas',
     author_email='eric@ericcanas.com',
     url='https://github.com/Eric-Canas/webcam',
     description='A simple and convenient library to interact with webcams in Python without having to address Hardware Limitations',
 
     long_description=open('README.md', 'r').read(),
     long_description_content_type='text/markdown',
```

### Comparing `webcam-0.2/webcam/_webcam_background.py` & `webcam-0.3/webcam/_webcam_background.py`

 * *Files 11% similar despite different names*

```diff
@@ -5,22 +5,30 @@
 cv2.VideoCapture class, so it can be used as a drop-in replacement for the cv2.VideoCapture class.
 
 Author: Eric Canas
 Github: https://github.com/Eric-Canas
 Email: eric@ericcanas.com
 Date: 05-05-2023
 """
-
 from __future__ import annotations
 from imutils.video import WebcamVideoStream
+import time
 
 
 class _WebcamBackground(WebcamVideoStream):
     def __init__(self, src=0, name="WebcamVideoStream"):
         super().__init__(src=src, name=name)
+        time.sleep(0.25)  # Added delay
+
+    def update(self):
+        while True:
+            if self.stopped:
+                return
+            if self.stream.isOpened():  # Check if the stream is opened
+                (self.grabbed, self.frame) = self.stream.read()
 
     def read(self):
         frame = super().read()
         return self.grabbed, frame
 
     def stop(self):
         super().stop()
```

### Comparing `webcam-0.2/webcam/webcam.py` & `webcam-0.3/webcam/webcam.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,41 +12,52 @@
 
 from __future__ import annotations
 import cv2
 import numpy as np
 import time
 from typing import Tuple
 
+import os
+
+from webcam._video_webcam import _VideoWebcam
 from webcam._webcam_background import _WebcamBackground
 
 
 class Webcam:
     def __init__(
         self,
         webcam_src: int | str = 0,
         h: int | None = None,
         w: int | None = None,
         as_bgr: bool = True,
         batch_size: int | None = None,
-        run_in_background: bool = True,
+        run_in_background: bool = False,
         max_frame_rate: int | None = 60,
     ):
         """
         Initialize the WebcamReader.
 
         :param webcam_src: int or str. The index of the webcam or its path.
         :param h: int or None. Desired height of the frames. If None and `w` is provided, the aspect ratio will be preserved.
         :param w: int or None. Desired width of the frames. If None and `h` is provided, the aspect ratio will be preserved.
         :param as_bgr: bool. If True, the frames will be returned in BGR format, otherwise in RGB format.
         :param batch_size: int or None. If not None, the iterator will yield batches of frames (B, H, W, C). If None, the iterator will yield single frames (H, W, C).
         :param run_in_background: bool. If True, the frames will be read in a background thread (speeding up the reading).
         :param max_frame_rate: int or None. The maximum frame rate to read the frames at. If None, there will be no limitations on frame rating.
         """
         self._background = run_in_background
-        self.cap = _WebcamBackground(src=webcam_src).start() if run_in_background else cv2.VideoCapture(webcam_src)
+        if run_in_background:
+            raise NotImplementedError("Background reading is not implemented yet.")
+            #self.cap = _WebcamBackground(src=webcam_src).start()
+        elif isinstance(webcam_src, str):
+            #TODO: Improve the check for video file
+            assert os.path.isfile(webcam_src), f"Video file not found: {webcam_src}"
+            self.cap = _VideoWebcam(video_path=webcam_src)
+        else:
+            self.cap = cv2.VideoCapture(webcam_src)
         self.as_bgr = as_bgr
 
         # Calculate and set output frame size
         self.frame_size_hw = self._calculate_and_set_desired_resolution(h, w)
 
         # Set batch size and frame rate attributes
         self.batch_size = batch_size
```

### Comparing `webcam-0.2/webcam.egg-info/PKG-INFO` & `webcam-0.3/webcam.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: webcam
-Version: 0.2
+Version: 0.3
 Summary: A simple and convenient library to interact with webcams in Python without having to address Hardware Limitations
 Home-page: https://github.com/Eric-Canas/webcam
 Author: Eric-Canas
 Author-email: eric@ericcanas.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
```

