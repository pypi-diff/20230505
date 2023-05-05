# Comparing `tmp/webcam-0.6.tar.gz` & `tmp/webcam-0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "webcam-0.6.tar", last modified: Fri May  5 12:15:54 2023, max compression
+gzip compressed data, was "webcam-0.7.tar", last modified: Fri May  5 14:27:17 2023, max compression
```

## Comparing `webcam-0.6.tar` & `webcam-0.7.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-05-05 12:15:54.528339 webcam-0.6/
--rw-rw-rw-   0        0        0     1089 2023-05-04 16:30:34.000000 webcam-0.6/LICENSE
--rw-rw-rw-   0        0        0     1311 2023-05-05 12:15:54.522307 webcam-0.6/PKG-INFO
--rw-rw-rw-   0        0        0      244 2023-05-05 08:42:27.000000 webcam-0.6/README.md
--rw-rw-rw-   0        0        0       42 2023-05-05 12:15:54.528339 webcam-0.6/setup.cfg
--rw-rw-rw-   0        0        0     1309 2023-05-05 12:15:52.000000 webcam-0.6/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-05 12:15:54.496805 webcam-0.6/webcam/
--rw-rw-rw-   0        0        0       28 2023-05-05 08:42:27.000000 webcam-0.6/webcam/__init__.py
--rw-rw-rw-   0        0        0     2687 2023-05-05 12:14:40.000000 webcam-0.6/webcam/_video_webcam.py
--rw-rw-rw-   0        0        0     1812 2023-05-05 10:19:36.000000 webcam-0.6/webcam/_webcam_background.py
--rw-rw-rw-   0        0        0    10350 2023-05-05 12:11:12.000000 webcam-0.6/webcam/webcam.py
-drwxrwxrwx   0        0        0        0 2023-05-05 12:15:54.522307 webcam-0.6/webcam.egg-info/
--rw-rw-rw-   0        0        0     1311 2023-05-05 12:15:54.000000 webcam-0.6/webcam.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      264 2023-05-05 12:15:54.000000 webcam-0.6/webcam.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-05 12:15:54.000000 webcam-0.6/webcam.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       28 2023-05-05 12:15:54.000000 webcam-0.6/webcam.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-05-05 12:15:54.000000 webcam-0.6/webcam.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-05 14:27:17.386033 webcam-0.7/
+-rw-rw-rw-   0        0        0     1089 2023-05-04 16:30:34.000000 webcam-0.7/LICENSE
+-rw-rw-rw-   0        0        0     1311 2023-05-05 14:27:17.386033 webcam-0.7/PKG-INFO
+-rw-rw-rw-   0        0        0      244 2023-05-05 08:42:27.000000 webcam-0.7/README.md
+-rw-rw-rw-   0        0        0       42 2023-05-05 14:27:17.386033 webcam-0.7/setup.cfg
+-rw-rw-rw-   0        0        0     1309 2023-05-05 14:27:01.000000 webcam-0.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-05 14:27:17.354786 webcam-0.7/webcam/
+-rw-rw-rw-   0        0        0       28 2023-05-05 08:42:27.000000 webcam-0.7/webcam/__init__.py
+-rw-rw-rw-   0        0        0     2687 2023-05-05 12:14:40.000000 webcam-0.7/webcam/_video_webcam.py
+-rw-rw-rw-   0        0        0     1812 2023-05-05 10:19:36.000000 webcam-0.7/webcam/_webcam_background.py
+-rw-rw-rw-   0        0        0    12714 2023-05-05 13:05:54.000000 webcam-0.7/webcam/webcam.py
+drwxrwxrwx   0        0        0        0 2023-05-05 14:27:17.386033 webcam-0.7/webcam.egg-info/
+-rw-rw-rw-   0        0        0     1311 2023-05-05 14:27:16.000000 webcam-0.7/webcam.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      264 2023-05-05 14:27:17.000000 webcam-0.7/webcam.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-05 14:27:16.000000 webcam-0.7/webcam.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       28 2023-05-05 14:27:17.000000 webcam-0.7/webcam.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-05-05 14:27:17.000000 webcam-0.7/webcam.egg-info/top_level.txt
```

### Comparing `webcam-0.6/LICENSE` & `webcam-0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `webcam-0.6/PKG-INFO` & `webcam-0.7/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: webcam
-Version: 0.6
+Version: 0.7
 Summary: A simple and convenient library to interact with webcams in Python without having to address Hardware Limitations
 Home-page: https://github.com/Eric-Canas/webcam
 Author: Eric-Canas
 Author-email: eric@ericcanas.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `webcam-0.6/setup.py` & `webcam-0.7/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='webcam',
-    version='0.6',
+    version='0.7',
     author='Eric-Canas',
     author_email='eric@ericcanas.com',
     url='https://github.com/Eric-Canas/webcam',
     description='A simple and convenient library to interact with webcams in Python without having to address Hardware Limitations',
 
     long_description=open('README.md', 'r').read(),
     long_description_content_type='text/markdown',
```

### Comparing `webcam-0.6/webcam/_video_webcam.py` & `webcam-0.7/webcam/_video_webcam.py`

 * *Files identical despite different names*

### Comparing `webcam-0.6/webcam/_webcam_background.py` & `webcam-0.7/webcam/_webcam_background.py`

 * *Files identical despite different names*

### Comparing `webcam-0.6/webcam/webcam.py` & `webcam-0.7/webcam/webcam.py`

 * *Files 26% similar despite different names*

```diff
@@ -17,38 +17,43 @@
 from typing import Tuple
 
 import os
 
 from webcam._video_webcam import _VideoWebcam
 from webcam._webcam_background import _WebcamBackground
 
+CROP, RESIZE = 'crop', 'resize'
 
 class Webcam:
     def __init__(
         self,
         webcam_src: int | str = 0,
         h: int | None = None,
         w: int | None = None,
         as_bgr: bool = False,
         batch_size: int | None = None,
         run_in_background: bool = False,
         max_frame_rate: int | None = 60,
+        on_aspect_ratio_lost: str = CROP,
     ):
         """
         Initialize the WebcamReader.
 
         :param webcam_src: int or str. The index of the webcam or its path.
         :param h: int or None. Desired height of the frames. If None and `_w` is provided, the aspect ratio will be preserved.
         :param w: int or None. Desired width of the frames. If None and `_h` is provided, the aspect ratio will be preserved.
         :param as_bgr: bool. If True, the frames will be returned in BGR format, otherwise in RGB format.
         :param batch_size: int or None. If not None, the iterator will yield batches of frames (B, H, W, C). If None, the iterator will yield single frames (H, W, C).
         :param run_in_background: bool. If True, the frames will be read in a background thread (speeding up the reading).
         :param max_frame_rate: int or None. The maximum frame rate to read the frames at. If None, there will be no limitations on frame rating.
         """
+        assert on_aspect_ratio_lost in (CROP, RESIZE), f"Invalid value for `on_aspect_ratio_lost`: {on_aspect_ratio_lost}." \
+                                                       f" Valid values are: {CROP}, {RESIZE}"
         self._background = run_in_background
+        self.on_aspect_ratio_lost = on_aspect_ratio_lost
         if run_in_background:
             raise NotImplementedError("Background reading is not implemented yet.")
             #self.cap = _WebcamBackground(src=webcam_src).start()
         elif isinstance(webcam_src, str):
             #TODO: Improve the check for video file
             assert os.path.isfile(webcam_src), f"Video file not found: {webcam_src}"
             self.cap = _VideoWebcam(video_path=webcam_src)
@@ -179,14 +184,59 @@
         max_h, max_w = self._set_webcam_resolution(h=1e6, w=1e6)
 
         # Restore the original resolution
         self._set_webcam_resolution(h=current_h, w=current_w)
 
         return max_h, max_w
 
+    def _adjust_image_shape(self, frame: np.ndarray, h: int, w: int) -> np.ndarray:
+        """
+        Adjust the shape of the frame according to the on_aspect_ratio_lost parameter.
+
+        :param frame: np.ndarray. The input frame.
+        :param h: int. Desired height of the frame.
+        :param w: int. Desired width of the frame.
+        :return: np.ndarray. The adjusted frame.
+        """
+        if self.on_aspect_ratio_lost == RESIZE:
+            return cv2.resize(src=frame, dsize=(w, h))
+        elif self.on_aspect_ratio_lost == CROP:
+            return self._resize_and_center_crop(frame=frame, h=h, w=w)
+        else:
+            raise ValueError(f"Invalid value for 'on_aspect_ratio_lost' parameter: {self.on_aspect_ratio_lost}. "
+                                f"Valid values are: {RESIZE}, {CROP}.")
+
+    def _resize_and_center_crop(self, frame: np.ndarray, h: int, w: int) -> np.ndarray:
+        """
+        Resize and center crop the input frame to the desired dimensions, while preserving the original aspect ratio.
+
+        :param frame: np.ndarray. The input frame to be resized and cropped.
+        :param h: int. The desired height of the output frame.
+        :param w: int. The desired width of the output frame.
+        :return: np.ndarray. The resized and center-cropped frame.
+        """
+        current_h, current_w = frame.shape[:2]
+        aspect_ratio = current_w / current_h
+
+        # Calculate the new dimensions such that the aspect ratio is preserved
+        if float(h) / w > aspect_ratio:
+            new_h, new_w = h, int(h * aspect_ratio)
+        else:
+            new_w, new_h = w, int(w / aspect_ratio)
+
+        # Resize the frame to the new dimensions
+        frame = cv2.resize(src=frame, dsize=(new_w, new_h))
+
+        # Calculate the position of the center crop
+        y1, x1 = (new_h - h) // 2, (new_w - w) // 2
+        y2, x2 = y1 + h, x1 + w
+
+        # Crop the frame
+        return frame[y1:y2, x1:x2]
+
     def read(self) -> tuple[bool, np.ndarray|None]:
         """
         Read a frame from the webcam.
 
         If the webcam's returned frame size is different from the user-set size, the frame is automatically resized.
 
         :return: tuple. A boolean indicating whether the frame was read successfully, and the frame itself.
@@ -194,16 +244,16 @@
         ret, frame = self.cap.read()
 
         if ret:
             # Extract the height and width of the frame
             h, w = frame.shape[:2]
 
             # Resize the frame if the webcam's returned frame size is different from the user-set size
-            if (h, w) != self.frame_size_hw:
-                frame = cv2.resize(src=frame, dsize=self.frame_size_hw[::-1])
+            if (h, w) != (self.h, self.w):
+                frame = self._adjust_image_shape(frame=frame, h=self.h, w=self.w)
 
             # Convert the frame from BGR to RGB format if necessary
             if not self.as_bgr:
                 cv2.cvtColor(src=frame, code=cv2.COLOR_BGR2RGB, dst=frame)
 
         return ret, frame
```

### Comparing `webcam-0.6/webcam.egg-info/PKG-INFO` & `webcam-0.7/webcam.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: webcam
-Version: 0.6
+Version: 0.7
 Summary: A simple and convenient library to interact with webcams in Python without having to address Hardware Limitations
 Home-page: https://github.com/Eric-Canas/webcam
 Author: Eric-Canas
 Author-email: eric@ericcanas.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
```

