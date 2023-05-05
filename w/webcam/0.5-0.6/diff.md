# Comparing `tmp/webcam-0.5.tar.gz` & `tmp/webcam-0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "webcam-0.5.tar", last modified: Fri May  5 11:23:32 2023, max compression
+gzip compressed data, was "webcam-0.6.tar", last modified: Fri May  5 12:15:54 2023, max compression
```

## Comparing `webcam-0.5.tar` & `webcam-0.6.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-05-05 11:23:32.577091 webcam-0.5/
--rw-rw-rw-   0        0        0     1089 2023-05-04 16:30:34.000000 webcam-0.5/LICENSE
--rw-rw-rw-   0        0        0     1311 2023-05-05 11:23:32.576107 webcam-0.5/PKG-INFO
--rw-rw-rw-   0        0        0      244 2023-05-05 08:42:27.000000 webcam-0.5/README.md
--rw-rw-rw-   0        0        0       42 2023-05-05 11:23:32.577091 webcam-0.5/setup.cfg
--rw-rw-rw-   0        0        0     1309 2023-05-05 11:23:28.000000 webcam-0.5/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-05 11:23:32.527864 webcam-0.5/webcam/
--rw-rw-rw-   0        0        0       28 2023-05-05 08:42:27.000000 webcam-0.5/webcam/__init__.py
--rw-rw-rw-   0        0        0     2651 2023-05-05 10:53:58.000000 webcam-0.5/webcam/_video_webcam.py
--rw-rw-rw-   0        0        0     1812 2023-05-05 10:19:36.000000 webcam-0.5/webcam/_webcam_background.py
--rw-rw-rw-   0        0        0    10349 2023-05-05 11:22:13.000000 webcam-0.5/webcam/webcam.py
-drwxrwxrwx   0        0        0        0 2023-05-05 11:23:32.571773 webcam-0.5/webcam.egg-info/
--rw-rw-rw-   0        0        0     1311 2023-05-05 11:23:32.000000 webcam-0.5/webcam.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      264 2023-05-05 11:23:32.000000 webcam-0.5/webcam.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-05 11:23:32.000000 webcam-0.5/webcam.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       28 2023-05-05 11:23:32.000000 webcam-0.5/webcam.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-05-05 11:23:32.000000 webcam-0.5/webcam.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-05 12:15:54.528339 webcam-0.6/
+-rw-rw-rw-   0        0        0     1089 2023-05-04 16:30:34.000000 webcam-0.6/LICENSE
+-rw-rw-rw-   0        0        0     1311 2023-05-05 12:15:54.522307 webcam-0.6/PKG-INFO
+-rw-rw-rw-   0        0        0      244 2023-05-05 08:42:27.000000 webcam-0.6/README.md
+-rw-rw-rw-   0        0        0       42 2023-05-05 12:15:54.528339 webcam-0.6/setup.cfg
+-rw-rw-rw-   0        0        0     1309 2023-05-05 12:15:52.000000 webcam-0.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-05 12:15:54.496805 webcam-0.6/webcam/
+-rw-rw-rw-   0        0        0       28 2023-05-05 08:42:27.000000 webcam-0.6/webcam/__init__.py
+-rw-rw-rw-   0        0        0     2687 2023-05-05 12:14:40.000000 webcam-0.6/webcam/_video_webcam.py
+-rw-rw-rw-   0        0        0     1812 2023-05-05 10:19:36.000000 webcam-0.6/webcam/_webcam_background.py
+-rw-rw-rw-   0        0        0    10350 2023-05-05 12:11:12.000000 webcam-0.6/webcam/webcam.py
+drwxrwxrwx   0        0        0        0 2023-05-05 12:15:54.522307 webcam-0.6/webcam.egg-info/
+-rw-rw-rw-   0        0        0     1311 2023-05-05 12:15:54.000000 webcam-0.6/webcam.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      264 2023-05-05 12:15:54.000000 webcam-0.6/webcam.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-05 12:15:54.000000 webcam-0.6/webcam.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       28 2023-05-05 12:15:54.000000 webcam-0.6/webcam.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-05-05 12:15:54.000000 webcam-0.6/webcam.egg-info/top_level.txt
```

### Comparing `webcam-0.5/LICENSE` & `webcam-0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `webcam-0.5/PKG-INFO` & `webcam-0.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: webcam
-Version: 0.5
+Version: 0.6
 Summary: A simple and convenient library to interact with webcams in Python without having to address Hardware Limitations
 Home-page: https://github.com/Eric-Canas/webcam
 Author: Eric-Canas
 Author-email: eric@ericcanas.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `webcam-0.5/setup.py` & `webcam-0.6/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='webcam',
-    version='0.5',
+    version='0.6',
     author='Eric-Canas',
     author_email='eric@ericcanas.com',
     url='https://github.com/Eric-Canas/webcam',
     description='A simple and convenient library to interact with webcams in Python without having to address Hardware Limitations',
 
     long_description=open('README.md', 'r').read(),
     long_description_content_type='text/markdown',
```

### Comparing `webcam-0.5/webcam/_video_webcam.py` & `webcam-0.6/webcam/_video_webcam.py`

 * *Files 26% similar despite different names*

```diff
@@ -5,18 +5,22 @@
 can be used as a drop-in replacement for the cv2.VideoCapture class when working with video files.
 
 Author: Eric Canas
 Github: https://github.com/Eric-Canas
 Email: eric@ericcanas.com
 Date: 05-05-2023
 """
+from __future__ import annotations
 
 import os
 import cv2
 import time
+from warnings import warn
+
+import numpy as np
 
 
 class _VideoWebcam:
     def __init__(self, video_path: str):
         """
         Initialize the _VideoWebcam.
 
@@ -30,35 +34,33 @@
         self.start_timestamp = time.time()
         # Just read the first frame to make sure the video is valid
         ret, frame = self.cap.read()
         assert ret, f'Video file at {video_path} is invalid'
 
     def read(self):
         current_frame = int((time.time() - self.start_timestamp) * self.fps) % self.video_length
-        return self.get_required_frame(current_frame)
+        return self.get_required_frame(target_frame=current_frame)
 
-    def get_required_frame(self, target_frame):
+    def get_required_frame(self, target_frame: int) -> tuple[bool, None | np.ndarray]:
         last_frame = int(self.cap.get(cv2.CAP_PROP_POS_FRAMES))
 
         # Calculate the number of frames to skip
         skip_frames = target_frame - last_frame
-        if skip_frames < 0:
-            skip_frames += self.video_length
+        if skip_frames < -1:
+            warn(f'Frame {target_frame} has already been read. Cannot read frame {target_frame} again.')
+            return False, None
+
 
-        # Use set method if more than 50 frames need to be skipped
-        if skip_frames > 50:
-            self.cap.set(cv2.CAP_PROP_POS_FRAMES, target_frame)
-            ret, frame = self.cap.read()
-        else:
-            # Use grab method to quickly skip the unnecessary frames
-            for _ in range(skip_frames - 1):
-                self.cap.grab()
+        # Use grab method to quickly skip the unnecessary frames
+        for _ in range(skip_frames - 1):
+            if not self.cap.grab():
+                return False, None
 
-            # Retrieve the required frame
-            ret, frame = self.cap.retrieve()
+        # Retrieve the required frame
+        ret, frame = self.cap.retrieve()
 
         return ret, frame
 
     def stop(self):
         pass
 
     def get(self, propId):
```

### Comparing `webcam-0.5/webcam/_webcam_background.py` & `webcam-0.6/webcam/_webcam_background.py`

 * *Files identical despite different names*

### Comparing `webcam-0.5/webcam/webcam.py` & `webcam-0.6/webcam/webcam.py`

 * *Files 0% similar despite different names*

```diff
@@ -24,15 +24,15 @@
 
 class Webcam:
     def __init__(
         self,
         webcam_src: int | str = 0,
         h: int | None = None,
         w: int | None = None,
-        as_bgr: bool = True,
+        as_bgr: bool = False,
         batch_size: int | None = None,
         run_in_background: bool = False,
         max_frame_rate: int | None = 60,
     ):
         """
         Initialize the WebcamReader.
```

### Comparing `webcam-0.5/webcam.egg-info/PKG-INFO` & `webcam-0.6/webcam.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: webcam
-Version: 0.5
+Version: 0.6
 Summary: A simple and convenient library to interact with webcams in Python without having to address Hardware Limitations
 Home-page: https://github.com/Eric-Canas/webcam
 Author: Eric-Canas
 Author-email: eric@ericcanas.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
```

