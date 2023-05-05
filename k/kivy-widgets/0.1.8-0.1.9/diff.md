# Comparing `tmp/kivy_widgets-0.1.8.tar.gz` & `tmp/kivy_widgets-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "kivy_widgets-0.1.8.tar", max compression
+gzip compressed data, was "kivy_widgets-0.1.9.tar", max compression
```

## Comparing `kivy_widgets-0.1.8.tar` & `kivy_widgets-0.1.9.tar`

### file list

```diff
@@ -1,13 +1,13 @@
--rw-r--r--   0        0        0     1068 2023-03-22 04:32:53.454823 kivy_widgets-0.1.8/LICENSE
--rw-r--r--   0        0        0     1098 2023-03-29 09:24:10.945782 kivy_widgets-0.1.8/README.md
--rw-r--r--   0        0        0        0 2023-03-24 03:41:57.270003 kivy_widgets-0.1.8/kivy_widgets/__init__.py
--rw-r--r--   0        0        0     4014 2023-05-02 13:09:47.427325 kivy_widgets-0.1.8/kivy_widgets/buttons.py
--rw-r--r--   0        0        0     7716 2023-04-27 06:16:20.787339 kivy_widgets-0.1.8/kivy_widgets/color_definitions.py
--rw-r--r--   0        0        0    10884 2023-05-02 13:57:34.878412 kivy_widgets-0.1.8/kivy_widgets/dropdown.py
--rw-r--r--   0        0        0  1261792 2023-03-29 09:08:00.604752 kivy_widgets-0.1.8/kivy_widgets/fonts/materialdesignicons-webfont.ttf
--rw-r--r--   0        0        0   266864 2023-03-29 09:08:00.605752 kivy_widgets-0.1.8/kivy_widgets/icon_definitions.py
--rw-r--r--   0        0        0     6794 2023-04-05 03:45:49.650130 kivy_widgets-0.1.8/kivy_widgets/icons.py
--rw-r--r--   0        0        0        0 2023-04-01 03:59:53.455098 kivy_widgets-0.1.8/kivy_widgets/inspector.py
--rw-r--r--   0        0        0       62 2023-04-27 06:16:14.173339 kivy_widgets-0.1.8/kivy_widgets/test.py
--rw-r--r--   0        0        0      994 2023-05-05 06:25:28.557128 kivy_widgets-0.1.8/pyproject.toml
--rw-r--r--   0        0        0     1583 1970-01-01 00:00:00.000000 kivy_widgets-0.1.8/PKG-INFO
+-rw-r--r--   0        0        0     1068 2023-03-22 04:32:53.454823 kivy_widgets-0.1.9/LICENSE
+-rw-r--r--   0        0        0     1098 2023-03-29 09:24:10.945782 kivy_widgets-0.1.9/README.md
+-rw-r--r--   0        0        0        0 2023-03-24 03:41:57.270003 kivy_widgets-0.1.9/kivy_widgets/__init__.py
+-rw-r--r--   0        0        0     4014 2023-05-02 13:09:47.427325 kivy_widgets-0.1.9/kivy_widgets/buttons.py
+-rw-r--r--   0        0        0     7716 2023-04-27 06:16:20.787339 kivy_widgets-0.1.9/kivy_widgets/color_definitions.py
+-rw-r--r--   0        0        0    10883 2023-05-05 07:51:08.030284 kivy_widgets-0.1.9/kivy_widgets/dropdown.py
+-rw-r--r--   0        0        0  1261792 2023-03-29 09:08:00.604752 kivy_widgets-0.1.9/kivy_widgets/fonts/materialdesignicons-webfont.ttf
+-rw-r--r--   0        0        0   266864 2023-03-29 09:08:00.605752 kivy_widgets-0.1.9/kivy_widgets/icon_definitions.py
+-rw-r--r--   0        0        0     6794 2023-04-05 03:45:49.650130 kivy_widgets-0.1.9/kivy_widgets/icons.py
+-rw-r--r--   0        0        0        0 2023-04-01 03:59:53.455098 kivy_widgets-0.1.9/kivy_widgets/inspector.py
+-rw-r--r--   0        0        0       62 2023-04-27 06:16:14.173339 kivy_widgets-0.1.9/kivy_widgets/test.py
+-rw-r--r--   0        0        0      994 2023-05-05 07:52:32.560287 kivy_widgets-0.1.9/pyproject.toml
+-rw-r--r--   0        0        0     1583 1970-01-01 00:00:00.000000 kivy_widgets-0.1.9/PKG-INFO
```

### Comparing `kivy_widgets-0.1.8/LICENSE` & `kivy_widgets-0.1.9/LICENSE`

 * *Files identical despite different names*

### Comparing `kivy_widgets-0.1.8/README.md` & `kivy_widgets-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `kivy_widgets-0.1.8/kivy_widgets/buttons.py` & `kivy_widgets-0.1.9/kivy_widgets/buttons.py`

 * *Files identical despite different names*

### Comparing `kivy_widgets-0.1.8/kivy_widgets/color_definitions.py` & `kivy_widgets-0.1.9/kivy_widgets/color_definitions.py`

 * *Files identical despite different names*

### Comparing `kivy_widgets-0.1.8/kivy_widgets/dropdown.py` & `kivy_widgets-0.1.9/kivy_widgets/dropdown.py`

 * *Files 0% similar despite different names*

```diff
@@ -232,15 +232,15 @@
             self._dropdown.dismiss()
             self._dropdown = None
         cls = self.dropdown_cls
         if isinstance(cls, str):
             cls = Factory.get(cls)
 
         if not self.container_width:
-            self._dropdown = cls(auto_width=False)
+            self._dropdown = cls(auto_width=True)
         else:
             self._dropdown = cls()
         self._dropdown.bind(on_select=self._on_dropdown_select)
         self._dropdown.bind(on_dismiss=self._close_dropdown)
         self._update_dropdown()
 
     def _update_dropdown(self, *largs):
```

### Comparing `kivy_widgets-0.1.8/kivy_widgets/fonts/materialdesignicons-webfont.ttf` & `kivy_widgets-0.1.9/kivy_widgets/fonts/materialdesignicons-webfont.ttf`

 * *Files identical despite different names*

### Comparing `kivy_widgets-0.1.8/kivy_widgets/icon_definitions.py` & `kivy_widgets-0.1.9/kivy_widgets/icon_definitions.py`

 * *Files identical despite different names*

### Comparing `kivy_widgets-0.1.8/kivy_widgets/icons.py` & `kivy_widgets-0.1.9/kivy_widgets/icons.py`

 * *Files identical despite different names*

### Comparing `kivy_widgets-0.1.8/pyproject.toml` & `kivy_widgets-0.1.9/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "kivy-widgets"
-version = "0.1.8"
+version = "0.1.9"
 description = ""
 authors = ["filipemarch <filipe.marchesini@gmail.com>", "ShootingStarDragon <rppapamaths@gmail.com>"]
 readme = "README.md"
 packages = [{include = "kivy_widgets"}]
 
 [tool.poetry.dependencies]
 python = "^3.8"
```

### Comparing `kivy_widgets-0.1.8/PKG-INFO` & `kivy_widgets-0.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: kivy-widgets
-Version: 0.1.8
+Version: 0.1.9
 Summary: 
 Author: filipemarch
 Author-email: filipe.marchesini@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

