# Comparing `tmp/webcam-0.3.tar.gz` & `tmp/webcam-0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "webcam-0.3.tar", last modified: Fri May  5 10:57:33 2023, max compression
+gzip compressed data, was "webcam-0.4.tar", last modified: Fri May  5 11:08:59 2023, max compression
```

## Comparing `webcam-0.3.tar` & `webcam-0.4.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-05-05 10:57:33.606796 webcam-0.3/
--rw-rw-rw-   0        0        0     1089 2023-05-04 16:30:34.000000 webcam-0.3/LICENSE
--rw-rw-rw-   0        0        0     1311 2023-05-05 10:57:33.605920 webcam-0.3/PKG-INFO
--rw-rw-rw-   0        0        0      244 2023-05-05 08:42:27.000000 webcam-0.3/README.md
--rw-rw-rw-   0        0        0       42 2023-05-05 10:57:33.606796 webcam-0.3/setup.cfg
--rw-rw-rw-   0        0        0     1309 2023-05-05 10:57:21.000000 webcam-0.3/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-05 10:57:33.570007 webcam-0.3/webcam/
--rw-rw-rw-   0        0        0       28 2023-05-05 08:42:27.000000 webcam-0.3/webcam/__init__.py
--rw-rw-rw-   0        0        0     2651 2023-05-05 10:53:58.000000 webcam-0.3/webcam/_video_webcam.py
--rw-rw-rw-   0        0        0     1812 2023-05-05 10:19:36.000000 webcam-0.3/webcam/_webcam_background.py
--rw-rw-rw-   0        0        0    11009 2023-05-05 10:10:40.000000 webcam-0.3/webcam/webcam.py
-drwxrwxrwx   0        0        0        0 2023-05-05 10:57:33.603464 webcam-0.3/webcam.egg-info/
--rw-rw-rw-   0        0        0     1311 2023-05-05 10:57:33.000000 webcam-0.3/webcam.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      264 2023-05-05 10:57:33.000000 webcam-0.3/webcam.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-05 10:57:33.000000 webcam-0.3/webcam.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       28 2023-05-05 10:57:33.000000 webcam-0.3/webcam.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-05-05 10:57:33.000000 webcam-0.3/webcam.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-05 11:08:59.202148 webcam-0.4/
+-rw-rw-rw-   0        0        0     1089 2023-05-04 16:30:34.000000 webcam-0.4/LICENSE
+-rw-rw-rw-   0        0        0     1311 2023-05-05 11:08:59.202148 webcam-0.4/PKG-INFO
+-rw-rw-rw-   0        0        0      244 2023-05-05 08:42:27.000000 webcam-0.4/README.md
+-rw-rw-rw-   0        0        0       42 2023-05-05 11:08:59.202148 webcam-0.4/setup.cfg
+-rw-rw-rw-   0        0        0     1309 2023-05-05 11:08:54.000000 webcam-0.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-05 11:08:59.171394 webcam-0.4/webcam/
+-rw-rw-rw-   0        0        0       28 2023-05-05 08:42:27.000000 webcam-0.4/webcam/__init__.py
+-rw-rw-rw-   0        0        0     2651 2023-05-05 10:53:58.000000 webcam-0.4/webcam/_video_webcam.py
+-rw-rw-rw-   0        0        0     1812 2023-05-05 10:19:36.000000 webcam-0.4/webcam/_webcam_background.py
+-rw-rw-rw-   0        0        0    11201 2023-05-05 11:08:54.000000 webcam-0.4/webcam/webcam.py
+drwxrwxrwx   0        0        0        0 2023-05-05 11:08:59.202148 webcam-0.4/webcam.egg-info/
+-rw-rw-rw-   0        0        0     1311 2023-05-05 11:08:59.000000 webcam-0.4/webcam.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      264 2023-05-05 11:08:59.000000 webcam-0.4/webcam.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-05 11:08:59.000000 webcam-0.4/webcam.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       28 2023-05-05 11:08:59.000000 webcam-0.4/webcam.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-05-05 11:08:59.000000 webcam-0.4/webcam.egg-info/top_level.txt
```

### Comparing `webcam-0.3/LICENSE` & `webcam-0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `webcam-0.3/PKG-INFO` & `webcam-0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: webcam
-Version: 0.3
+Version: 0.4
 Summary: A simple and convenient library to interact with webcams in Python without having to address Hardware Limitations
 Home-page: https://github.com/Eric-Canas/webcam
 Author: Eric-Canas
 Author-email: eric@ericcanas.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `webcam-0.3/setup.py` & `webcam-0.4/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='webcam',
-    version='0.3',
+    version='0.4',
     author='Eric-Canas',
     author_email='eric@ericcanas.com',
     url='https://github.com/Eric-Canas/webcam',
     description='A simple and convenient library to interact with webcams in Python without having to address Hardware Limitations',
 
     long_description=open('README.md', 'r').read(),
     long_description_content_type='text/markdown',
```

### Comparing `webcam-0.3/webcam/_video_webcam.py` & `webcam-0.4/webcam/_video_webcam.py`

 * *Files identical despite different names*

### Comparing `webcam-0.3/webcam/_webcam_background.py` & `webcam-0.4/webcam/_webcam_background.py`

 * *Files identical despite different names*

### Comparing `webcam-0.3/webcam/webcam.py` & `webcam-0.4/webcam/webcam.py`

 * *Files 2% similar despite different names*

```diff
@@ -33,16 +33,16 @@
         run_in_background: bool = False,
         max_frame_rate: int | None = 60,
     ):
         """
         Initialize the WebcamReader.
 
         :param webcam_src: int or str. The index of the webcam or its path.
-        :param h: int or None. Desired height of the frames. If None and `w` is provided, the aspect ratio will be preserved.
-        :param w: int or None. Desired width of the frames. If None and `h` is provided, the aspect ratio will be preserved.
+        :param h: int or None. Desired height of the frames. If None and `_w` is provided, the aspect ratio will be preserved.
+        :param w: int or None. Desired width of the frames. If None and `_h` is provided, the aspect ratio will be preserved.
         :param as_bgr: bool. If True, the frames will be returned in BGR format, otherwise in RGB format.
         :param batch_size: int or None. If not None, the iterator will yield batches of frames (B, H, W, C). If None, the iterator will yield single frames (H, W, C).
         :param run_in_background: bool. If True, the frames will be read in a background thread (speeding up the reading).
         :param max_frame_rate: int or None. The maximum frame rate to read the frames at. If None, there will be no limitations on frame rating.
         """
         self._background = run_in_background
         if run_in_background:
@@ -62,22 +62,30 @@
         # Set batch size and frame rate attributes
         self.batch_size = batch_size
         self.start_timestamp = time.time()
         self.max_frame_rate = max_frame_rate
         self.last_frame_timestamp = self.start_timestamp
 
     @property
-    def h(self) -> int:
+    def _h(self) -> int:
         return int(self.cap.get(cv2.CAP_PROP_FRAME_HEIGHT))
 
     @property
-    def w(self) -> int:
+    def _w(self) -> int:
         return int(self.cap.get(cv2.CAP_PROP_FRAME_WIDTH))
 
     @property
+    def h(self) -> int:
+        return self.frame_size_hw[0]
+
+    @property
+    def w(self) -> int:
+        return self.frame_size_hw[1]
+
+    @property
     def current_timestamp_seconds(self):
         return time.time() - self.start_timestamp
 
     def read_next_frame(self) -> np.ndarray:
         """
         Read the next frame from the video. (Skipping the frames_offset if it is greater than one.)
         """
@@ -108,15 +116,15 @@
         :return: The next frame in the video.
         """
         # While webcam is open
         while self.cap.isOpened():
             yield self.read_next_frame()
         raise StopIteration
 
-    def _calculate_and_set_desired_resolution(self, h: int | None = None, w: int | None = None) -> tuple[int, int]:
+    def _calculate_and_set_desired_resolution(self, _h: int | None = None, _w: int | None = None) -> tuple[int, int]:
         """
         Calculate and set the optimal webcam resolution based on the desired width and height.
         The resolution will only change if the new resolution is natively supported by the webcam
         and maintains the maximum available aspect ratio.
 
         :param h: int or None. Desired height of the frames.
         :param w: int or None. Desired width of the frames.
@@ -134,28 +142,28 @@
 
         # Change the resolution if supported (and keeps the maximum aspect ratio if only one dimension was provided)
         if self._is_resolution_natively_supported(h=h, w=w):
             self._set_webcam_resolution(h=h, w=w)
 
         return h, w
 
-    def _set_webcam_resolution(self, h: int, w: int) -> Tuple[int, int]:
+    def _set_webcam_resolution(self, _h: int, _w: int) -> Tuple[int, int]:
         """
         Set the webcam resolution to the specified height and width and return the actual frame size set by the webcam.
 
         :param h: int. Desired height of the frames.
         :param w: int. Desired width of the frames.
         :return: tuple. The final frame size (height, width) after attempting to set the desired resolution.
         """
         self.cap.set(cv2.CAP_PROP_FRAME_WIDTH, w)
         self.cap.set(cv2.CAP_PROP_FRAME_HEIGHT, h)
 
-        return self.h, self.w
+        return self._h, self._w
 
-    def calculate_frame_size_keeping_aspect_ratio(self, h: int | None, w: int | None) -> Tuple[int, int]:
+    def calculate_frame_size_keeping_aspect_ratio(self, _h: int | None, _w: int | None) -> Tuple[int, int]:
         """
         Calculate the output frame size based on the desired width and height while keeping the aspect ratio.
 
         :param h: int or None. Desired height of the frames.
         :param w: int or None. Desired width of the frames.
         :return: tuple. The final frame size (height, width) with the aspect ratio preserved.
         """
@@ -170,29 +178,29 @@
 
         if w is None:
             aspect_ratio = max_w / max_h
             return h, int(h * aspect_ratio)
 
         return h, w
 
-    def _is_resolution_natively_supported(self, h: int, w: int):
-        current_h, current_w = self.h, self.w
+    def _is_resolution_natively_supported(self, _h: int, _w: int):
+        current_h, current_w = self._h, self._w
         supported_h, supported_w = self._set_webcam_resolution(h=h, w=w)
         new_h, new_w = self._set_webcam_resolution(h=current_h, w=current_w)
         assert new_h == current_h and new_w == current_w, f"Webcam resolution could not be restored to {current_h}x{current_w}."
         return supported_h == h and supported_w == w
 
     def _max_available_resolution(self) -> Tuple[int, int]:
         """
         Get the maximum allowed webcam resolution without changing the current resolution.
 
         :return: tuple. The maximum allowed webcam resolution (height, width).
         """
         # Store the current resolution
-        current_h, current_w = self.h, self.w
+        current_h, current_w = self._h, self._w
 
         # Set the webcam resolution to an extremely high value and get the resulting maximum allowed resolution
         max_h, max_w = self._set_webcam_resolution(h=1e6, w=1e6)
 
         # Restore the original resolution
         self._set_webcam_resolution(h=current_h, w=current_w)
 
@@ -234,33 +242,33 @@
     def release(self):
         self.cap.release()
 
     def isOpened(self):
         return self.cap.isOpened()
 
     # --------------- AUXILIARY METHODS ---------------
-    def calculate_frame_size_keeping_aspect_ratio(self, h:int | None, w:int|None) -> tuple[int, int]:
+    def calculate_frame_size_keeping_aspect_ratio(self, _h:int | None, _w:int|None) -> tuple[int, int]:
         """
         When only one of the frame size dimensions is given, the other one is calculated keeping the
         aspect ratio with the original video.
 
-        :param h: int or None. Height of the frame. If None, w must be provided.
-        :param w: int or None. Width of the frame. If None, h must be provided.
+        :param h: int or None. Height of the frame. If None, _w must be provided.
+        :param w: int or None. Width of the frame. If None, _h must be provided.
         :return: The height and width of the frame.
         """
 
 
         if h is None and w is not None:
-            h = int(round(self.h * w / self.w))
+            h = int(round(self._h * w / self._w))
         elif h is not None and w is None:
-            w = int(round(self.w * h / self.h))
+            w = int(round(self._w * h / self._h))
         else:
             raise ValueError(f'Only one of the frame size dimensions must be provided.'
-                             f' Got h={h} and w={w}.')
-        assert h is not None and w is not None, f'Both h and w should have been calculated. Got h={h} and w={w}.'
+                             f' Got _h={h} and _w={w}.')
+        assert h is not None and w is not None, f'Both _h and _w should have been calculated. Got _h={h} and _w={w}.'
         return h, w
 
     def __iter__(self):
         return self
 
     def __next__(self):
         return self.read_next_frame()
```

### Comparing `webcam-0.3/webcam.egg-info/PKG-INFO` & `webcam-0.4/webcam.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: webcam
-Version: 0.3
+Version: 0.4
 Summary: A simple and convenient library to interact with webcams in Python without having to address Hardware Limitations
 Home-page: https://github.com/Eric-Canas/webcam
 Author: Eric-Canas
 Author-email: eric@ericcanas.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
```

