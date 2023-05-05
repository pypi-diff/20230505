# Comparing `tmp/HumanCursor-0.0.3.tar.gz` & `tmp/HumanCursor-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "HumanCursor-0.0.3.tar", last modified: Wed Apr 26 15:32:20 2023, max compression
+gzip compressed data, was "HumanCursor-0.0.4.tar", last modified: Fri May  5 15:17:21 2023, max compression
```

## Comparing `HumanCursor-0.0.3.tar` & `HumanCursor-0.0.4.tar`

### file list

```diff
@@ -1,20 +1,28 @@
-drwxrwxrwx   0        0        0        0 2023-04-26 15:32:20.430572 HumanCursor-0.0.3/
-drwxrwxrwx   0        0        0        0 2023-04-26 15:32:20.413518 HumanCursor-0.0.3/HumanCursor.egg-info/
--rw-rw-rw-   0        0        0     5040 2023-04-26 15:32:20.000000 HumanCursor-0.0.3/HumanCursor.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      404 2023-04-26 15:32:20.000000 HumanCursor-0.0.3/HumanCursor.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-26 15:32:20.000000 HumanCursor-0.0.3/HumanCursor.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       34 2023-04-26 15:32:20.000000 HumanCursor-0.0.3/HumanCursor.egg-info/requires.txt
--rw-rw-rw-   0        0        0       12 2023-04-26 15:32:20.000000 HumanCursor-0.0.3/HumanCursor.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1089 2023-04-25 17:10:16.000000 HumanCursor-0.0.3/LICENSE
--rw-rw-rw-   0        0        0     5040 2023-04-26 15:32:20.430572 HumanCursor-0.0.3/PKG-INFO
--rw-rw-rw-   0        0        0     4559 2023-04-26 15:15:26.000000 HumanCursor-0.0.3/README.md
-drwxrwxrwx   0        0        0        0 2023-04-26 15:32:20.422080 HumanCursor-0.0.3/humancursor/
--rw-rw-rw-   0        0        0       98 2023-04-26 15:30:38.000000 HumanCursor-0.0.3/humancursor/__init__.py
--rw-rw-rw-   0        0        0     1118 2023-04-26 15:30:38.000000 HumanCursor-0.0.3/humancursor/system_cursor.py
-drwxrwxrwx   0        0        0        0 2023-04-26 15:32:20.428037 HumanCursor-0.0.3/humancursor/utilities/
--rw-rw-rw-   0        0        0        0 2023-04-25 15:16:36.000000 HumanCursor-0.0.3/humancursor/utilities/__init__.py
--rw-rw-rw-   0        0        0     7848 2023-04-25 15:13:53.000000 HumanCursor-0.0.3/humancursor/utilities/human_curve_generator.py
--rw-rw-rw-   0        0        0     8531 2023-04-26 15:30:38.000000 HumanCursor-0.0.3/humancursor/utilities/web_adjuster.py
--rw-rw-rw-   0        0        0     6923 2023-04-26 15:30:38.000000 HumanCursor-0.0.3/humancursor/web_cursor.py
--rw-rw-rw-   0        0        0      643 2023-04-26 15:31:53.000000 HumanCursor-0.0.3/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-04-26 15:32:20.430572 HumanCursor-0.0.3/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-05 15:17:21.040648 HumanCursor-0.0.4/
+drwxrwxrwx   0        0        0        0 2023-05-05 15:17:21.004715 HumanCursor-0.0.4/HumanCursor.egg-info/
+-rw-rw-rw-   0        0        0     5040 2023-05-05 15:17:20.000000 HumanCursor-0.0.4/HumanCursor.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      556 2023-05-05 15:17:20.000000 HumanCursor-0.0.4/HumanCursor.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-05 15:17:20.000000 HumanCursor-0.0.4/HumanCursor.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       34 2023-05-05 15:17:20.000000 HumanCursor-0.0.4/HumanCursor.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       12 2023-05-05 15:17:20.000000 HumanCursor-0.0.4/HumanCursor.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1089 2023-04-25 17:10:16.000000 HumanCursor-0.0.4/LICENSE
+-rw-rw-rw-   0        0        0     5040 2023-05-05 15:17:21.040648 HumanCursor-0.0.4/PKG-INFO
+-rw-rw-rw-   0        0        0     4559 2023-04-26 15:15:26.000000 HumanCursor-0.0.4/README.md
+drwxrwxrwx   0        0        0        0 2023-05-05 15:17:21.017508 HumanCursor-0.0.4/humancursor/
+-rw-rw-rw-   0        0        0       98 2023-04-26 15:30:38.000000 HumanCursor-0.0.4/humancursor/__init__.py
+-rw-rw-rw-   0        0        0     2027 2023-05-05 14:49:34.000000 HumanCursor-0.0.4/humancursor/system_cursor.py
+drwxrwxrwx   0        0        0        0 2023-05-05 15:17:21.024793 HumanCursor-0.0.4/humancursor/test/
+-rw-rw-rw-   0        0        0        0 2023-05-05 14:50:29.000000 HumanCursor-0.0.4/humancursor/test/__init__.py
+-rw-rw-rw-   0        0        0      266 2023-05-05 15:01:17.000000 HumanCursor-0.0.4/humancursor/test/system.py
+-rw-rw-rw-   0        0        0     1110 2023-05-05 15:01:16.000000 HumanCursor-0.0.4/humancursor/test/web.py
+drwxrwxrwx   0        0        0        0 2023-05-05 15:17:21.034147 HumanCursor-0.0.4/humancursor/utilities/
+-rw-rw-rw-   0        0        0        0 2023-04-25 15:16:36.000000 HumanCursor-0.0.4/humancursor/utilities/__init__.py
+-rw-rw-rw-   0        0        0     3318 2023-05-05 14:44:20.000000 HumanCursor-0.0.4/humancursor/utilities/calc.py
+-rw-rw-rw-   0        0        0     7876 2023-05-05 14:39:43.000000 HumanCursor-0.0.4/humancursor/utilities/human_curve_generator.py
+-rw-rw-rw-   0        0        0     5346 2023-05-05 14:46:47.000000 HumanCursor-0.0.4/humancursor/utilities/web_adjuster.py
+drwxrwxrwx   0        0        0        0 2023-05-05 15:17:20.971877 HumanCursor-0.0.4/humancursor/venv/
+drwxrwxrwx   0        0        0        0 2023-05-05 15:17:21.037093 HumanCursor-0.0.4/humancursor/venv/Scripts/
+-rw-rw-rw-   0        0        0     1169 2023-05-05 13:35:16.000000 HumanCursor-0.0.4/humancursor/venv/Scripts/activate_this.py
+-rw-rw-rw-   0        0        0     6923 2023-04-26 15:30:38.000000 HumanCursor-0.0.4/humancursor/web_cursor.py
+-rw-rw-rw-   0        0        0      643 2023-05-05 15:14:19.000000 HumanCursor-0.0.4/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-05 15:17:21.042437 HumanCursor-0.0.4/setup.cfg
```

### Comparing `HumanCursor-0.0.3/HumanCursor.egg-info/PKG-INFO` & `HumanCursor-0.0.4/HumanCursor.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: HumanCursor
-Version: 0.0.3
+Version: 0.0.4
 Summary: Simulate Human Cursor Movement for Automated Scripts
 Author-email: Flori Batusha <floribatusha0@gmail.com>
 Project-URL: Homepage, https://github.com/riflosnake/HumanCursor
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
```

### Comparing `HumanCursor-0.0.3/LICENSE` & `HumanCursor-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `HumanCursor-0.0.3/PKG-INFO` & `HumanCursor-0.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: HumanCursor
-Version: 0.0.3
+Version: 0.0.4
 Summary: Simulate Human Cursor Movement for Automated Scripts
 Author-email: Flori Batusha <floribatusha0@gmail.com>
 Project-URL: Homepage, https://github.com/riflosnake/HumanCursor
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.7
```

### Comparing `HumanCursor-0.0.3/README.md` & `HumanCursor-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `HumanCursor-0.0.3/humancursor/system_cursor.py` & `HumanCursor-0.0.4/humancursor/system_cursor.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,26 +1,51 @@
 from time import sleep
 import random
 import pyautogui
 
 from humancursor.utilities.human_curve_generator import HumanizeMouseTrajectory
+from humancursor.utilities.calc import generate_random_curve_parameters
 
 
 class SystemCursor:
     def __init__(self):
         pyautogui.MINIMUM_DURATION = 0
         pyautogui.MINIMUM_SLEEP = 0
         pyautogui.PAUSE = 0.015
 
     @staticmethod
     def move_to(point: list, duration: int = None, human_curve=None):
         """Moves to certain coordinates of screen"""
         from_point = pyautogui.position()
+
         if not human_curve:
-            human_curve = HumanizeMouseTrajectory(from_point, point)
+            (
+                offset_boundary_x,
+                offset_boundary_y,
+                knots_count,
+                distortion_mean,
+                distortion_st_dev,
+                distortion_frequency,
+                tween,
+                target_points,
+            ) = generate_random_curve_parameters(
+                pyautogui, from_point, point
+            )
+            human_curve = HumanizeMouseTrajectory(
+                from_point,
+                point,
+                offset_boundary_x=offset_boundary_x,
+                offset_boundary_y=offset_boundary_y,
+                knots_count=knots_count,
+                distortion_mean=distortion_mean,
+                distortion_st_dev=distortion_st_dev,
+                distortion_frequency=distortion_frequency,
+                tween=tween,
+                target_points=target_points,
+            )
 
         if duration is None:
             duration = random.uniform(0.5, 2.0)
         pyautogui.PAUSE = duration / len(human_curve.points)
         for pnt in human_curve.points:
             pyautogui.moveTo(pnt)
         pyautogui.moveTo(point)
```

### Comparing `HumanCursor-0.0.3/humancursor/utilities/human_curve_generator.py` & `HumanCursor-0.0.4/humancursor/utilities/human_curve_generator.py`

 * *Files 1% similar despite different names*

```diff
@@ -65,16 +65,16 @@
                 "left_boundary must be less than or equal to right_boundary"
             )
         if d_boundary > u_boundary:
             raise ValueError(
                 "down_boundary must be less than or equal to upper_boundary"
             )
         try:
-            knotsX = np.random.choice(range(l_boundary, r_boundary), size=knots_count)
-            knotsY = np.random.choice(range(d_boundary, u_boundary), size=knots_count)
+            knotsX = np.random.choice(range(l_boundary, r_boundary) or l_boundary, size=knots_count)
+            knotsY = np.random.choice(range(d_boundary, u_boundary) or d_boundary, size=knots_count)
         except TypeError:
             knotsX = np.random.choice(
                 range(int(l_boundary), int(r_boundary)), size=knots_count
             )
             knotsY = np.random.choice(
                 range(int(d_boundary), int(u_boundary)), size=knots_count
             )
```

### Comparing `HumanCursor-0.0.3/humancursor/web_cursor.py` & `HumanCursor-0.0.4/humancursor/web_cursor.py`

 * *Files identical despite different names*

### Comparing `HumanCursor-0.0.3/pyproject.toml` & `HumanCursor-0.0.4/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "HumanCursor"
-version = "0.0.3"
+version = "0.0.4"
 authors = [
   { name="Flori Batusha", email="floribatusha0@gmail.com" },
 ]
 description = "Simulate Human Cursor Movement for Automated Scripts"
 readme = "README.md"
 requires-python = ">=3.7"
 dependencies = [
```

