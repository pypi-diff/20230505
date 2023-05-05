# Comparing `tmp/bdffont-0.0.4.tar.gz` & `tmp/bdffont-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bdffont-0.0.4.tar", last modified: Fri May  5 14:17:57 2023, max compression
+gzip compressed data, was "bdffont-0.0.5.tar", last modified: Fri May  5 20:05:26 2023, max compression
```

## Comparing `bdffont-0.0.4.tar` & `bdffont-0.0.5.tar`

### file list

```diff
@@ -1,22 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 14:17:57.994434 bdffont-0.0.4/
--rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-05-05 14:17:39.000000 bdffont-0.0.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2508 2023-05-05 14:17:57.994434 bdffont-0.0.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1914 2023-05-05 14:17:39.000000 bdffont-0.0.4/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      670 2023-05-05 14:17:39.000000 bdffont-0.0.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-05 14:17:57.994434 bdffont-0.0.4/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 14:17:57.990434 bdffont-0.0.4/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 14:17:57.994434 bdffont-0.0.4/src/bdffont/
--rw-r--r--   0 runner    (1001) docker     (123)      177 2023-05-05 14:17:39.000000 bdffont-0.0.4/src/bdffont/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      691 2023-05-05 14:17:39.000000 bdffont-0.0.4/src/bdffont/error.py
--rw-r--r--   0 runner    (1001) docker     (123)     6626 2023-05-05 14:17:39.000000 bdffont-0.0.4/src/bdffont/font.py
--rw-r--r--   0 runner    (1001) docker     (123)     5378 2023-05-05 14:17:39.000000 bdffont-0.0.4/src/bdffont/glyph.py
--rw-r--r--   0 runner    (1001) docker     (123)     5928 2023-05-05 14:17:39.000000 bdffont-0.0.4/src/bdffont/parser.py
--rw-r--r--   0 runner    (1001) docker     (123)     3878 2023-05-05 14:17:39.000000 bdffont-0.0.4/src/bdffont/properties.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 14:17:57.994434 bdffont-0.0.4/src/bdffont.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2508 2023-05-05 14:17:57.000000 bdffont-0.0.4/src/bdffont.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      347 2023-05-05 14:17:57.000000 bdffont-0.0.4/src/bdffont.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 14:17:57.000000 bdffont-0.0.4/src/bdffont.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-05 14:17:57.000000 bdffont-0.0.4/src/bdffont.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 14:17:57.994434 bdffont-0.0.4/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1967 2023-05-05 14:17:39.000000 bdffont-0.0.4/tests/test_damaged.py
--rw-r--r--   0 runner    (1001) docker     (123)     3291 2023-05-05 14:17:39.000000 bdffont-0.0.4/tests/test_demo.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 20:05:26.479815 bdffont-0.0.5/
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-05-05 20:05:11.000000 bdffont-0.0.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2508 2023-05-05 20:05:26.479815 bdffont-0.0.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1914 2023-05-05 20:05:11.000000 bdffont-0.0.5/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      670 2023-05-05 20:05:11.000000 bdffont-0.0.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-05 20:05:26.479815 bdffont-0.0.5/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 20:05:26.475815 bdffont-0.0.5/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 20:05:26.475815 bdffont-0.0.5/src/bdffont/
+-rw-r--r--   0 runner    (1001) docker     (123)      177 2023-05-05 20:05:11.000000 bdffont-0.0.5/src/bdffont/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      691 2023-05-05 20:05:11.000000 bdffont-0.0.5/src/bdffont/error.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7112 2023-05-05 20:05:11.000000 bdffont-0.0.5/src/bdffont/font.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5802 2023-05-05 20:05:11.000000 bdffont-0.0.5/src/bdffont/glyph.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6010 2023-05-05 20:05:11.000000 bdffont-0.0.5/src/bdffont/parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3878 2023-05-05 20:05:11.000000 bdffont-0.0.5/src/bdffont/properties.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 20:05:26.479815 bdffont-0.0.5/src/bdffont.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2508 2023-05-05 20:05:26.000000 bdffont-0.0.5/src/bdffont.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      366 2023-05-05 20:05:26.000000 bdffont-0.0.5/src/bdffont.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 20:05:26.000000 bdffont-0.0.5/src/bdffont.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-05 20:05:26.000000 bdffont-0.0.5/src/bdffont.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 20:05:26.479815 bdffont-0.0.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     2015 2023-05-05 20:05:11.000000 bdffont-0.0.5/tests/test_damaged.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3395 2023-05-05 20:05:11.000000 bdffont-0.0.5/tests/test_demo.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4946 2023-05-05 20:05:11.000000 bdffont-0.0.5/tests/test_type.py
```

### Comparing `bdffont-0.0.4/LICENSE` & `bdffont-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `bdffont-0.0.4/PKG-INFO` & `bdffont-0.0.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bdffont
-Version: 0.0.4
+Version: 0.0.5
 Summary: A library for manipulating '.bdf' format fonts.
 Author: TakWolf
 Maintainer: TakWolf
 License: MIT License
 Project-URL: homepage, https://github.com/TakWolf/bdffont
 Project-URL: source, https://github.com/TakWolf/bdffont
 Project-URL: issues, https://github.com/TakWolf/bdffont/issues
```

### Comparing `bdffont-0.0.4/README.md` & `bdffont-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `bdffont-0.0.4/pyproject.toml` & `bdffont-0.0.5/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "bdffont"
-version = "0.0.4"
+version = "0.0.5"
 description = "A library for manipulating '.bdf' format fonts."
 readme = "README.md"
 license = { text = "MIT License" }
 requires-python = ">=3.10"
 authors = [
     { name = "TakWolf" },
 ]
```

### Comparing `bdffont-0.0.4/src/bdffont/error.py` & `bdffont-0.0.5/src/bdffont/error.py`

 * *Files identical despite different names*

### Comparing `bdffont-0.0.4/src/bdffont/font.py` & `bdffont-0.0.5/src/bdffont/font.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+import os
+
 from bdffont.properties import BdfProperties
 from bdffont.glyph import BdfGlyph
 from bdffont.error import BdfGlyphExists
 
 
 class BdfFont:
     # The BDF Specification version.
@@ -10,34 +12,34 @@
     # Either the 'X logical font description' or some private font name.
     # https://en.wikipedia.org/wiki/X_logical_font_description
     # Example: -Adobe-Helvetica-Bold-R-Normal--24-240-75-75-P-65-ISO8859-1
     name: str
 
     # The point size of the characters, the x resolution, and the y resolution of the device for which these characters were intended.
     # Names: point_size, x_dpi, y_dpi
-    size: (int, int, int)
+    size: tuple[int, int, int]
 
     # The width in x, height in y, and the x and y displacement of the lower left corner from the origin of the character.
     # Names: bounding_box_width, bounding_box_height, bounding_box_origin_x, bounding_box_origin_y
-    bounding_box: (int, int, int, int)
+    bounding_box: tuple[int, int, int, int]
 
     # Some optional extended properties.
     properties: BdfProperties
 
     # Glyph objects using code point indexing.
     code_point_to_glyph: dict[int, BdfGlyph]
 
     # Comments.
     comments: list[str]
 
     def __init__(
             self,
             name: str,
-            size: (int, int, int),
-            bounding_box: (int, int, int, int),
+            size: tuple[int, int, int],
+            bounding_box: tuple[int, int, int, int],
             properties: BdfProperties = None,
             glyphs: list[BdfGlyph] = None,
             comments: list[str] = None,
     ):
         self.spec_version = '2.1'
         self.name = name
         self.size = size
@@ -57,103 +59,100 @@
 
     @property
     def point_size(self) -> int:
         return self.size[0]
 
     @point_size.setter
     def point_size(self, value: int):
-        self.size[0] = value
+        self.size = (value, self.size[1], self.size[2])
 
     @property
-    def xy_dpi(self) -> (int, int):
+    def xy_dpi(self) -> tuple[int, int]:
         return self.size[1], self.size[2]
 
     @xy_dpi.setter
-    def xy_dpi(self, value: (int, int)):
-        self.size[1] = value[0]
-        self.size[2] = value[1]
+    def xy_dpi(self, value: tuple[int, int]):
+        self.size = (self.size[0], value[0], value[1])
 
     @property
     def x_dpi(self) -> int:
         return self.size[1]
 
     @x_dpi.setter
     def x_dpi(self, value: int):
-        self.size[1] = value
+        self.size = (self.size[0], value, self.size[2])
 
     @property
     def y_dpi(self) -> int:
         return self.size[2]
 
     @y_dpi.setter
     def y_dpi(self, value: int):
-        self.size[2] = value
+        self.size = (self.size[0], self.size[1], value)
 
     @property
-    def bounding_box_size(self) -> (int, int):
+    def bounding_box_size(self) -> tuple[int, int]:
         return self.bounding_box[0], self.bounding_box[1]
 
     @bounding_box_size.setter
-    def bounding_box_size(self, value: (int, int)):
-        self.bounding_box[0] = value[0]
-        self.bounding_box[1] = value[1]
+    def bounding_box_size(self, value: tuple[int, int]):
+        self.bounding_box = (value[0], value[1], self.bounding_box[2], self.bounding_box[3])
 
     @property
     def bounding_box_width(self) -> int:
         return self.bounding_box[0]
 
     @bounding_box_width.setter
     def bounding_box_width(self, value: int):
-        self.bounding_box[0] = value
+        self.bounding_box = (value, self.bounding_box[1], self.bounding_box[2], self.bounding_box[3])
 
     @property
     def bounding_box_height(self) -> int:
         return self.bounding_box[1]
 
     @bounding_box_height.setter
     def bounding_box_height(self, value: int):
-        self.bounding_box[1] = value
+        self.bounding_box = (self.bounding_box[0], value, self.bounding_box[2], self.bounding_box[3])
 
     @property
-    def bounding_box_origin(self) -> (int, int):
+    def bounding_box_origin(self) -> tuple[int, int]:
         return self.bounding_box[2], self.bounding_box[3]
 
     @bounding_box_origin.setter
-    def bounding_box_origin(self, value: (int, int)):
-        self.bounding_box[2] = value[0]
-        self.bounding_box[3] = value[1]
+    def bounding_box_origin(self, value: tuple[int, int]):
+        self.bounding_box = (self.bounding_box[0], self.bounding_box[1], value[0], value[1])
 
     @property
     def bounding_box_origin_x(self) -> int:
         return self.bounding_box[2]
 
     @bounding_box_origin_x.setter
     def bounding_box_origin_x(self, value: int):
-        self.bounding_box[2] = value
+        self.bounding_box = (self.bounding_box[0], self.bounding_box[1], value, self.bounding_box[3])
 
     @property
     def bounding_box_origin_y(self) -> int:
         return self.bounding_box[3]
 
     @bounding_box_origin_y.setter
     def bounding_box_origin_y(self, value: int):
-        self.bounding_box[3] = value
+        self.bounding_box = (self.bounding_box[0], self.bounding_box[1], self.bounding_box[2], value)
 
-    def get_glyph(self, code_point: int) -> BdfGlyph:
+    def get_glyph(self, code_point: int) -> BdfGlyph | None:
         return self.code_point_to_glyph.get(code_point, None)
 
     def add_glyph(self, glyph: BdfGlyph):
         if glyph.code_point in self.code_point_to_glyph:
             raise BdfGlyphExists(glyph.code_point)
         self.code_point_to_glyph[glyph.code_point] = glyph
 
     def set_glyph(self, glyph: BdfGlyph):
         self.code_point_to_glyph[glyph.code_point] = glyph
 
-    def remove_glyph(self, code_point: int) -> BdfGlyph:
+    def remove_glyph(self, code_point: int) -> BdfGlyph | None:
         return self.code_point_to_glyph.pop(code_point, None)
 
     def encode(self) -> list[str]:
         lines = [
             f'STARTFONT {self.spec_version}',
         ]
         for comment in self.comments:
@@ -191,10 +190,10 @@
         lines.append('ENDFONT')
         lines.append('')
         return lines
 
     def encode_str(self) -> str:
         return '\n'.join(self.encode())
 
-    def save(self, file_path):
+    def save(self, file_path: str | bytes | os.PathLike[str] | os.PathLike[bytes]):
         with open(file_path, 'w', encoding='utf-8') as file:
             file.write(self.encode_str())
```

### Comparing `bdffont-0.0.4/src/bdffont/glyph.py` & `bdffont-0.0.5/src/bdffont/glyph.py`

 * *Files 25% similar despite different names*

```diff
@@ -10,39 +10,39 @@
     # the character. If the size of the character is p points, the width information must be scaled by p/1000
     # to get the width of the character in printer’s points. This width information should be considered as a
     # vector indicating the position of the next character’s origin relative to the origin of this character.
     # To convert the scalable width to the width in device pixels, multiply s_width times p/1000 times r/72,
     # where r is the device resolution in pixels per inch. The result is a real number giving the ideal print
     # width in device pixels. The actual device width must of course be an integral number of device pixels and
     # is given in the next entry. The s_width y value should always be zero for a standard X font.
-    scalable_width: (int, int)
+    scalable_width: tuple[int, int]
 
     # The width in x and y of the character in device units. Like the s_width, this width information is a vector
     # indicating the position of the next character’s origin relative to the origin of this character. Note that
     # the d_width of a given "hand-tuned" WYSIWYG glyph may deviate slightly from its ideal device-independent width
     # given by s_width in order to improve its typographic characteristics on a display. The d_width y value should
     # always be zero for a standard X font.
-    device_width: (int, int)
+    device_width: tuple[int, int]
 
     # The width in x, height in y, and the x and y displacement of the lower left corner from the origin of the character.
-    bounding_box: (int, int, int, int)
+    bounding_box: tuple[int, int, int, int]
 
     # The bitmap object.
     bitmap: list[list[int]]
 
     # Comments.
     comments: list[str]
 
     def __init__(
             self,
             name: str,
             code_point: int,
-            scalable_width: (int, int),
-            device_width: (int, int),
-            bounding_box: (int, int, int, int),
+            scalable_width: tuple[int, int],
+            device_width: tuple[int, int],
+            bounding_box: tuple[int, int, int, int],
             bitmap: list[list[int]] = None,
             comments: list[str] = None,
     ):
         self.name = name
         self.code_point = code_point
         self.scalable_width = scalable_width
         self.device_width = device_width
@@ -58,89 +58,87 @@
 
     @property
     def scalable_width_x(self) -> int:
         return self.scalable_width[0]
 
     @scalable_width_x.setter
     def scalable_width_x(self, value: int):
-        self.scalable_width[0] = value
+        self.scalable_width = (value, self.scalable_width[1])
 
     @property
     def scalable_width_y(self) -> int:
         return self.scalable_width[1]
 
     @scalable_width_y.setter
     def scalable_width_y(self, value: int):
-        self.scalable_width[1] = value
+        self.scalable_width = (self.scalable_width[0], value)
 
     @property
     def device_width_x(self) -> int:
         return self.device_width[0]
 
     @device_width_x.setter
     def device_width_x(self, value: int):
-        self.device_width[0] = value
+        self.device_width = (value, self.device_width[1])
 
     @property
     def device_width_y(self) -> int:
         return self.device_width[1]
 
     @device_width_y.setter
     def device_width_y(self, value: int):
-        self.device_width[1] = value
+        self.device_width = (self.device_width[0], value)
 
     @property
-    def bounding_box_size(self) -> (int, int):
+    def bounding_box_size(self) -> tuple[int, int]:
         return self.bounding_box[0], self.bounding_box[1]
 
     @bounding_box_size.setter
-    def bounding_box_size(self, value: (int, int)):
-        self.bounding_box[0] = value[0]
-        self.bounding_box[1] = value[1]
+    def bounding_box_size(self, value: tuple[int, int]):
+        self.bounding_box = (value[0], value[1], self.bounding_box[2], self.bounding_box[3])
 
     @property
     def bounding_box_width(self) -> int:
         return self.bounding_box[0]
 
     @bounding_box_width.setter
     def bounding_box_width(self, value: int):
-        self.bounding_box[0] = value
+        self.bounding_box = (value, self.bounding_box[1], self.bounding_box[2], self.bounding_box[3])
 
     @property
     def bounding_box_height(self) -> int:
         return self.bounding_box[1]
 
     @bounding_box_height.setter
     def bounding_box_height(self, value: int):
-        self.bounding_box[1] = value
+        self.bounding_box = (self.bounding_box[0], value, self.bounding_box[2], self.bounding_box[3])
 
     @property
-    def bounding_box_origin(self) -> (int, int):
+    def bounding_box_origin(self) -> tuple[int, int]:
         return self.bounding_box[2], self.bounding_box[3]
 
     @bounding_box_origin.setter
-    def bounding_box_origin(self, value: (int, int)):
-        self.bounding_box[2] = value[0]
-        self.bounding_box[3] = value[1]
+    def bounding_box_origin(self, value: tuple[int, int]):
+        self.bounding_box = (self.bounding_box[0], self.bounding_box[1], value[0], value[1])
 
     @property
     def bounding_box_origin_x(self) -> int:
         return self.bounding_box[2]
 
     @bounding_box_origin_x.setter
     def bounding_box_origin_x(self, value: int):
-        self.bounding_box[2] = value
+        self.bounding_box = (self.bounding_box[0], self.bounding_box[1], value, self.bounding_box[3])
 
     @property
     def bounding_box_origin_y(self) -> int:
         return self.bounding_box[3]
 
     @bounding_box_origin_y.setter
     def bounding_box_origin_y(self, value: int):
-        self.bounding_box[3] = value
+        self.bounding_box = (self.bounding_box[0], self.bounding_box[1], self.bounding_box[2], value)
 
     def get_padding_bitmap(self) -> list[list[int]]:
         padding_bitmap = []
         for bitmap_row in self.bitmap:
             padding_bitmap_row = []
             for alpha in bitmap_row:
                 if alpha == 0:
```

### Comparing `bdffont-0.0.4/src/bdffont/parser.py` & `bdffont-0.0.5/src/bdffont/parser.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,17 +1,18 @@
+import os
 import re
 from typing import Iterator
 
 from bdffont.font import BdfFont
 from bdffont.properties import BdfProperties
 from bdffont.glyph import BdfGlyph
 from bdffont.error import BdfGlyphExists, BdfMissingLine, BdfValueIncorrect
 
 
-def _next_word_line(lines: Iterator[str]) -> (str, str):
+def _next_word_line(lines: Iterator[str]) -> tuple[str, str | None] | None:
     while True:
         try:
             line = next(lines)
         except StopIteration:
             return None
         line = line.strip()
         if line == '':
@@ -164,10 +165,10 @@
     raise BdfMissingLine('STARTFONT')
 
 
 def decode_bdf_str(text: str) -> BdfFont:
     return decode_bdf(iter(text.split('\n')))
 
 
-def load_bdf(file_path) -> BdfFont:
+def load_bdf(file_path: str | bytes | os.PathLike[str] | os.PathLike[bytes]) -> BdfFont:
     with open(file_path, 'r', encoding='utf-8') as file:
         return decode_bdf(iter(file.readlines()))
```

### Comparing `bdffont-0.0.4/src/bdffont/properties.py` & `bdffont-0.0.5/src/bdffont/properties.py`

 * *Files identical despite different names*

### Comparing `bdffont-0.0.4/src/bdffont.egg-info/PKG-INFO` & `bdffont-0.0.5/src/bdffont.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bdffont
-Version: 0.0.4
+Version: 0.0.5
 Summary: A library for manipulating '.bdf' format fonts.
 Author: TakWolf
 Maintainer: TakWolf
 License: MIT License
 Project-URL: homepage, https://github.com/TakWolf/bdffont
 Project-URL: source, https://github.com/TakWolf/bdffont
 Project-URL: issues, https://github.com/TakWolf/bdffont/issues
```

### Comparing `bdffont-0.0.4/tests/test_damaged.py` & `bdffont-0.0.5/tests/test_damaged.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,17 @@
-import os.path
+import os
 
 import pytest
 
 import bdffont
 from bdffont.error import BdfMissingLine, BdfValueIncorrect
 from tests import assets_dir
 
 
-def load_damaged_bdf(bdf_file_name):
+def load_damaged_bdf(bdf_file_name: str | bytes | os.PathLike[str] | os.PathLike[bytes]):
     bdf_file_path = os.path.join(assets_dir, 'damaged', bdf_file_name)
     bdffont.load_bdf(bdf_file_path)
 
 
 def test_not_a_bdf():
     with pytest.raises(Exception) as info:
         load_damaged_bdf('not_a_bdf.bdf')
```

### Comparing `bdffont-0.0.4/tests/test_demo.py` & `bdffont-0.0.5/tests/test_demo.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import os
 
 import bdffont
+from bdffont import BdfFont
 from tests import assets_dir, outputs_dir
 
 
-def load_bdf(bdf_file_name):
+def load_bdf(bdf_file_name: str | bytes | os.PathLike[str] | os.PathLike[bytes]) -> tuple[BdfFont, str]:
     bdf_file_path = os.path.join(assets_dir, bdf_file_name)
     with open(bdf_file_path, 'r', encoding='utf-8') as file:
         bdf_text = file.read()
     font = bdffont.decode_bdf_str(bdf_text)
     return font, bdf_text
```

