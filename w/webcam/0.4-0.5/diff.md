# Comparing `tmp/webcam-0.4.tar.gz` & `tmp/webcam-0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "webcam-0.4.tar", last modified: Fri May  5 11:08:59 2023, max compression
+gzip compressed data, was "webcam-0.5.tar", last modified: Fri May  5 11:23:32 2023, max compression
```

## Comparing `webcam-0.4.tar` & `webcam-0.5.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-05-05 11:08:59.202148 webcam-0.4/
--rw-rw-rw-   0        0        0     1089 2023-05-04 16:30:34.000000 webcam-0.4/LICENSE
--rw-rw-rw-   0        0        0     1311 2023-05-05 11:08:59.202148 webcam-0.4/PKG-INFO
--rw-rw-rw-   0        0        0      244 2023-05-05 08:42:27.000000 webcam-0.4/README.md
--rw-rw-rw-   0        0        0       42 2023-05-05 11:08:59.202148 webcam-0.4/setup.cfg
--rw-rw-rw-   0        0        0     1309 2023-05-05 11:08:54.000000 webcam-0.4/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-05 11:08:59.171394 webcam-0.4/webcam/
--rw-rw-rw-   0        0        0       28 2023-05-05 08:42:27.000000 webcam-0.4/webcam/__init__.py
--rw-rw-rw-   0        0        0     2651 2023-05-05 10:53:58.000000 webcam-0.4/webcam/_video_webcam.py
--rw-rw-rw-   0        0        0     1812 2023-05-05 10:19:36.000000 webcam-0.4/webcam/_webcam_background.py
--rw-rw-rw-   0        0        0    11201 2023-05-05 11:08:54.000000 webcam-0.4/webcam/webcam.py
-drwxrwxrwx   0        0        0        0 2023-05-05 11:08:59.202148 webcam-0.4/webcam.egg-info/
--rw-rw-rw-   0        0        0     1311 2023-05-05 11:08:59.000000 webcam-0.4/webcam.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      264 2023-05-05 11:08:59.000000 webcam-0.4/webcam.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-05 11:08:59.000000 webcam-0.4/webcam.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       28 2023-05-05 11:08:59.000000 webcam-0.4/webcam.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-05-05 11:08:59.000000 webcam-0.4/webcam.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-05 11:23:32.577091 webcam-0.5/
+-rw-rw-rw-   0        0        0     1089 2023-05-04 16:30:34.000000 webcam-0.5/LICENSE
+-rw-rw-rw-   0        0        0     1311 2023-05-05 11:23:32.576107 webcam-0.5/PKG-INFO
+-rw-rw-rw-   0        0        0      244 2023-05-05 08:42:27.000000 webcam-0.5/README.md
+-rw-rw-rw-   0        0        0       42 2023-05-05 11:23:32.577091 webcam-0.5/setup.cfg
+-rw-rw-rw-   0        0        0     1309 2023-05-05 11:23:28.000000 webcam-0.5/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-05 11:23:32.527864 webcam-0.5/webcam/
+-rw-rw-rw-   0        0        0       28 2023-05-05 08:42:27.000000 webcam-0.5/webcam/__init__.py
+-rw-rw-rw-   0        0        0     2651 2023-05-05 10:53:58.000000 webcam-0.5/webcam/_video_webcam.py
+-rw-rw-rw-   0        0        0     1812 2023-05-05 10:19:36.000000 webcam-0.5/webcam/_webcam_background.py
+-rw-rw-rw-   0        0        0    10349 2023-05-05 11:22:13.000000 webcam-0.5/webcam/webcam.py
+drwxrwxrwx   0        0        0        0 2023-05-05 11:23:32.571773 webcam-0.5/webcam.egg-info/
+-rw-rw-rw-   0        0        0     1311 2023-05-05 11:23:32.000000 webcam-0.5/webcam.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      264 2023-05-05 11:23:32.000000 webcam-0.5/webcam.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-05 11:23:32.000000 webcam-0.5/webcam.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       28 2023-05-05 11:23:32.000000 webcam-0.5/webcam.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-05-05 11:23:32.000000 webcam-0.5/webcam.egg-info/top_level.txt
```

### Comparing `webcam-0.4/LICENSE` & `webcam-0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `webcam-0.4/PKG-INFO` & `webcam-0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: webcam
-Version: 0.4
+Version: 0.5
 Summary: A simple and convenient library to interact with webcams in Python without having to address Hardware Limitations
 Home-page: https://github.com/Eric-Canas/webcam
 Author: Eric-Canas
 Author-email: eric@ericcanas.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `webcam-0.4/setup.py` & `webcam-0.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name='webcam',
-    version='0.4',
+    version='0.5',
     author='Eric-Canas',
     author_email='eric@ericcanas.com',
     url='https://github.com/Eric-Canas/webcam',
     description='A simple and convenient library to interact with webcams in Python without having to address Hardware Limitations',
 
     long_description=open('README.md', 'r').read(),
     long_description_content_type='text/markdown',
```

### Comparing `webcam-0.4/webcam/_video_webcam.py` & `webcam-0.5/webcam/_video_webcam.py`

 * *Files identical despite different names*

### Comparing `webcam-0.4/webcam/_webcam_background.py` & `webcam-0.5/webcam/_webcam_background.py`

 * *Files identical despite different names*

### Comparing `webcam-0.4/webcam/webcam.py` & `webcam-0.5/webcam/webcam.py`

 * *Files 10% similar despite different names*

```diff
@@ -116,15 +116,15 @@
         :return: The next frame in the video.
         """
         # While webcam is open
         while self.cap.isOpened():
             yield self.read_next_frame()
         raise StopIteration
 
-    def _calculate_and_set_desired_resolution(self, _h: int | None = None, _w: int | None = None) -> tuple[int, int]:
+    def _calculate_and_set_desired_resolution(self, h: int | None = None, w: int | None = None) -> tuple[int, int]:
         """
         Calculate and set the optimal webcam resolution based on the desired width and height.
         The resolution will only change if the new resolution is natively supported by the webcam
         and maintains the maximum available aspect ratio.
 
         :param h: int or None. Desired height of the frames.
         :param w: int or None. Desired width of the frames.
@@ -142,51 +142,28 @@
 
         # Change the resolution if supported (and keeps the maximum aspect ratio if only one dimension was provided)
         if self._is_resolution_natively_supported(h=h, w=w):
             self._set_webcam_resolution(h=h, w=w)
 
         return h, w
 
-    def _set_webcam_resolution(self, _h: int, _w: int) -> Tuple[int, int]:
+    def _set_webcam_resolution(self, h: int, w: int) -> Tuple[int, int]:
         """
         Set the webcam resolution to the specified height and width and return the actual frame size set by the webcam.
 
         :param h: int. Desired height of the frames.
         :param w: int. Desired width of the frames.
         :return: tuple. The final frame size (height, width) after attempting to set the desired resolution.
         """
         self.cap.set(cv2.CAP_PROP_FRAME_WIDTH, w)
         self.cap.set(cv2.CAP_PROP_FRAME_HEIGHT, h)
 
         return self._h, self._w
 
-    def calculate_frame_size_keeping_aspect_ratio(self, _h: int | None, _w: int | None) -> Tuple[int, int]:
-        """
-        Calculate the output frame size based on the desired width and height while keeping the aspect ratio.
-
-        :param h: int or None. Desired height of the frames.
-        :param w: int or None. Desired width of the frames.
-        :return: tuple. The final frame size (height, width) with the aspect ratio preserved.
-        """
-        max_h, max_w = self._max_available_resolution()
-
-        if h is None and w is None:
-            return max_h, max_w
-
-        if h is None:
-            aspect_ratio = max_h / max_w
-            return int(w * aspect_ratio), w
-
-        if w is None:
-            aspect_ratio = max_w / max_h
-            return h, int(h * aspect_ratio)
-
-        return h, w
-
-    def _is_resolution_natively_supported(self, _h: int, _w: int):
+    def _is_resolution_natively_supported(self, h: int, w: int):
         current_h, current_w = self._h, self._w
         supported_h, supported_w = self._set_webcam_resolution(h=h, w=w)
         new_h, new_w = self._set_webcam_resolution(h=current_h, w=current_w)
         assert new_h == current_h and new_w == current_w, f"Webcam resolution could not be restored to {current_h}x{current_w}."
         return supported_h == h and supported_w == w
 
     def _max_available_resolution(self) -> Tuple[int, int]:
@@ -242,15 +219,15 @@
     def release(self):
         self.cap.release()
 
     def isOpened(self):
         return self.cap.isOpened()
 
     # --------------- AUXILIARY METHODS ---------------
-    def calculate_frame_size_keeping_aspect_ratio(self, _h:int | None, _w:int|None) -> tuple[int, int]:
+    def calculate_frame_size_keeping_aspect_ratio(self, h:int | None, w:int|None) -> tuple[int, int]:
         """
         When only one of the frame size dimensions is given, the other one is calculated keeping the
         aspect ratio with the original video.
 
         :param h: int or None. Height of the frame. If None, _w must be provided.
         :param w: int or None. Width of the frame. If None, _h must be provided.
         :return: The height and width of the frame.
```

### Comparing `webcam-0.4/webcam.egg-info/PKG-INFO` & `webcam-0.5/webcam.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: webcam
-Version: 0.4
+Version: 0.5
 Summary: A simple and convenient library to interact with webcams in Python without having to address Hardware Limitations
 Home-page: https://github.com/Eric-Canas/webcam
 Author: Eric-Canas
 Author-email: eric@ericcanas.com
 License: MIT
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
```

