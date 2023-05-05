# Comparing `tmp/kivy_widgets-0.1.7.tar.gz` & `tmp/kivy_widgets-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kivy_widgets-0.1.7.tar", max compression
+gzip compressed data, was "kivy_widgets-0.1.8.tar", max compression
```

## Comparing `kivy_widgets-0.1.7.tar` & `kivy_widgets-0.1.8.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0     1068 2023-03-22 04:32:53.454823 kivy_widgets-0.1.7/LICENSE
--rw-r--r--   0        0        0     1098 2023-03-29 09:24:10.945782 kivy_widgets-0.1.7/README.md
--rw-r--r--   0        0        0        0 2023-03-24 03:41:57.270003 kivy_widgets-0.1.7/kivy_widgets/__init__.py
--rw-r--r--   0        0        0     3686 2023-05-01 20:55:55.093542 kivy_widgets-0.1.7/kivy_widgets/buttons.py
--rw-r--r--   0        0        0     7716 2023-04-27 06:16:20.787339 kivy_widgets-0.1.7/kivy_widgets/color_definitions.py
--rw-r--r--   0        0        0     4854 2023-05-01 20:55:55.096542 kivy_widgets-0.1.7/kivy_widgets/dropdown.py
--rw-r--r--   0        0        0  1261792 2023-03-29 09:08:00.604752 kivy_widgets-0.1.7/kivy_widgets/fonts/materialdesignicons-webfont.ttf
--rw-r--r--   0        0        0   266864 2023-03-29 09:08:00.605752 kivy_widgets-0.1.7/kivy_widgets/icon_definitions.py
--rw-r--r--   0        0        0     6794 2023-04-05 03:45:49.650130 kivy_widgets-0.1.7/kivy_widgets/icons.py
--rw-r--r--   0        0        0        0 2023-04-01 03:59:53.455098 kivy_widgets-0.1.7/kivy_widgets/inspector.py
--rw-r--r--   0        0        0       62 2023-04-27 06:16:14.173339 kivy_widgets-0.1.7/kivy_widgets/test.py
--rw-r--r--   0        0        0      994 2023-05-01 21:12:00.279571 kivy_widgets-0.1.7/pyproject.toml
--rw-r--r--   0        0        0     1583 1970-01-01 00:00:00.000000 kivy_widgets-0.1.7/PKG-INFO
+-rw-r--r--   0        0        0     1068 2023-03-22 04:32:53.454823 kivy_widgets-0.1.8/LICENSE
+-rw-r--r--   0        0        0     1098 2023-03-29 09:24:10.945782 kivy_widgets-0.1.8/README.md
+-rw-r--r--   0        0        0        0 2023-03-24 03:41:57.270003 kivy_widgets-0.1.8/kivy_widgets/__init__.py
+-rw-r--r--   0        0        0     4014 2023-05-02 13:09:47.427325 kivy_widgets-0.1.8/kivy_widgets/buttons.py
+-rw-r--r--   0        0        0     7716 2023-04-27 06:16:20.787339 kivy_widgets-0.1.8/kivy_widgets/color_definitions.py
+-rw-r--r--   0        0        0    10884 2023-05-02 13:57:34.878412 kivy_widgets-0.1.8/kivy_widgets/dropdown.py
+-rw-r--r--   0        0        0  1261792 2023-03-29 09:08:00.604752 kivy_widgets-0.1.8/kivy_widgets/fonts/materialdesignicons-webfont.ttf
+-rw-r--r--   0        0        0   266864 2023-03-29 09:08:00.605752 kivy_widgets-0.1.8/kivy_widgets/icon_definitions.py
+-rw-r--r--   0        0        0     6794 2023-04-05 03:45:49.650130 kivy_widgets-0.1.8/kivy_widgets/icons.py
+-rw-r--r--   0        0        0        0 2023-04-01 03:59:53.455098 kivy_widgets-0.1.8/kivy_widgets/inspector.py
+-rw-r--r--   0        0        0       62 2023-04-27 06:16:14.173339 kivy_widgets-0.1.8/kivy_widgets/test.py
+-rw-r--r--   0        0        0      994 2023-05-05 06:25:28.557128 kivy_widgets-0.1.8/pyproject.toml
+-rw-r--r--   0        0        0     1583 1970-01-01 00:00:00.000000 kivy_widgets-0.1.8/PKG-INFO
```

### Comparing `kivy_widgets-0.1.7/LICENSE` & `kivy_widgets-0.1.8/LICENSE`

 * *Files identical despite different names*

### Comparing `kivy_widgets-0.1.7/README.md` & `kivy_widgets-0.1.8/README.md`

 * *Files identical despite different names*

### Comparing `kivy_widgets-0.1.7/kivy_widgets/buttons.py` & `kivy_widgets-0.1.8/kivy_widgets/buttons.py`

 * *Files 10% similar despite different names*

```diff
@@ -18,18 +18,20 @@
     Custom button with icon and text
     """
 
     text = StringProperty()
     font_size = NumericProperty(sp(18))
     icon = StringProperty()
     bg_color = ColorProperty([1, 1, 1, 1])
-    color = ColorProperty([0, 0, 0, 1])
+    font_color = ColorProperty([0, 0, 0, 1])
     icon_color = ColorProperty([0, 0, 0, 1])
     radius = ListProperty([dp(5)])
     icon_size = NumericProperty(dp(24))
+    border_color = ColorProperty([1, 1, 1, 1])
+    border_width = NumericProperty(1)
     # icon_position = OptionProperty("left", options=["left", "right"])
     # text_pos = OptionProperty("left", options=["left", "center"])
 
     def get_current_color(self):
         if self.state == "normal":
             return self.bg_color
         else:
@@ -92,14 +94,19 @@
     canvas.before:
         Color:
             rgba: root.current_color
         RoundedRectangle:
             size: self.size
             pos: self.pos
             radius: root.radius
+        Color:
+            rgba: root.border_color if root.border_width else (0,0,0,0)
+        SmoothLine:
+            width: root.border_width
+            rounded_rectangle: (self.x, self.y, self.width, self.height, root.radius[0])
 
     Label:
         id: icon
         text: u"{}".format(unicode[root.icon]) if root.icon in unicode else "blank"
         icon: root.icon
         font_name: icon_font
         size_hint: (None, None)
@@ -117,11 +124,11 @@
 
     Label:
         id: label
         text: root.text
         font_size: root.font_size
         size_hint: None, None
         size: self.texture_size
-        color: root.color
+        color: root.font_color
         pos_hint: {'center_y': .5}
 """)
 # fmt: on
```

### Comparing `kivy_widgets-0.1.7/kivy_widgets/color_definitions.py` & `kivy_widgets-0.1.8/kivy_widgets/color_definitions.py`

 * *Files identical despite different names*

### Comparing `kivy_widgets-0.1.7/kivy_widgets/fonts/materialdesignicons-webfont.ttf` & `kivy_widgets-0.1.8/kivy_widgets/fonts/materialdesignicons-webfont.ttf`

 * *Files identical despite different names*

### Comparing `kivy_widgets-0.1.7/kivy_widgets/icon_definitions.py` & `kivy_widgets-0.1.8/kivy_widgets/icon_definitions.py`

 * *Files identical despite different names*

### Comparing `kivy_widgets-0.1.7/kivy_widgets/icons.py` & `kivy_widgets-0.1.8/kivy_widgets/icons.py`

 * *Files identical despite different names*

### Comparing `kivy_widgets-0.1.7/pyproject.toml` & `kivy_widgets-0.1.8/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "kivy-widgets"
-version = "0.1.7"
+version = "0.1.8"
 description = ""
 authors = ["filipemarch <filipe.marchesini@gmail.com>", "ShootingStarDragon <rppapamaths@gmail.com>"]
 readme = "README.md"
 packages = [{include = "kivy_widgets"}]
 
 [tool.poetry.dependencies]
 python = "^3.8"
```

### Comparing `kivy_widgets-0.1.7/PKG-INFO` & `kivy_widgets-0.1.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kivy-widgets
-Version: 0.1.7
+Version: 0.1.8
 Summary: 
 Author: filipemarch
 Author-email: filipe.marchesini@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

