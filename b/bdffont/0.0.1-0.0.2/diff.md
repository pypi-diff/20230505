# Comparing `tmp/bdffont-0.0.1.tar.gz` & `tmp/bdffont-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bdffont-0.0.1.tar", last modified: Thu May  4 16:05:52 2023, max compression
+gzip compressed data, was "bdffont-0.0.2.tar", last modified: Fri May  5 07:48:30 2023, max compression
```

## Comparing `bdffont-0.0.1.tar` & `bdffont-0.0.2.tar`

### file list

```diff
@@ -1,21 +1,22 @@
-drwxr-xr-x   0 takwolf    (501) staff       (20)        0 2023-05-04 16:05:52.822732 bdffont-0.0.1/
--rw-r--r--   0 takwolf    (501) staff       (20)     1064 2023-05-01 03:55:41.000000 bdffont-0.0.1/LICENSE
--rw-r--r--   0 takwolf    (501) staff       (20)     1053 2023-05-04 16:05:52.822324 bdffont-0.0.1/PKG-INFO
--rw-r--r--   0 takwolf    (501) staff       (20)      459 2023-05-03 10:38:16.000000 bdffont-0.0.1/README.md
--rw-r--r--   0 takwolf    (501) staff       (20)      670 2023-05-04 16:01:25.000000 bdffont-0.0.1/pyproject.toml
--rw-r--r--   0 takwolf    (501) staff       (20)       38 2023-05-04 16:05:52.822847 bdffont-0.0.1/setup.cfg
-drwxr-xr-x   0 takwolf    (501) staff       (20)        0 2023-05-04 16:05:52.811186 bdffont-0.0.1/src/
-drwxr-xr-x   0 takwolf    (501) staff       (20)        0 2023-05-04 16:05:52.818605 bdffont-0.0.1/src/bdffont/
--rw-r--r--   0 takwolf    (501) staff       (20)      161 2023-05-04 13:19:43.000000 bdffont-0.0.1/src/bdffont/__init__.py
--rw-r--r--   0 takwolf    (501) staff       (20)      873 2023-05-04 13:19:43.000000 bdffont-0.0.1/src/bdffont/common.py
--rw-r--r--   0 takwolf    (501) staff       (20)     6525 2023-05-04 14:52:07.000000 bdffont-0.0.1/src/bdffont/font.py
--rw-r--r--   0 takwolf    (501) staff       (20)     2575 2023-05-04 14:37:36.000000 bdffont-0.0.1/src/bdffont/glyph.py
--rw-r--r--   0 takwolf    (501) staff       (20)     5703 2023-05-04 14:49:35.000000 bdffont-0.0.1/src/bdffont/parser.py
--rw-r--r--   0 takwolf    (501) staff       (20)     2953 2023-05-04 14:49:35.000000 bdffont-0.0.1/src/bdffont/properties.py
-drwxr-xr-x   0 takwolf    (501) staff       (20)        0 2023-05-04 16:05:52.820933 bdffont-0.0.1/src/bdffont.egg-info/
--rw-r--r--   0 takwolf    (501) staff       (20)     1053 2023-05-04 16:05:52.000000 bdffont-0.0.1/src/bdffont.egg-info/PKG-INFO
--rw-r--r--   0 takwolf    (501) staff       (20)      326 2023-05-04 16:05:52.000000 bdffont-0.0.1/src/bdffont.egg-info/SOURCES.txt
--rw-r--r--   0 takwolf    (501) staff       (20)        1 2023-05-04 16:05:52.000000 bdffont-0.0.1/src/bdffont.egg-info/dependency_links.txt
--rw-r--r--   0 takwolf    (501) staff       (20)        8 2023-05-04 16:05:52.000000 bdffont-0.0.1/src/bdffont.egg-info/top_level.txt
-drwxr-xr-x   0 takwolf    (501) staff       (20)        0 2023-05-04 16:05:52.821461 bdffont-0.0.1/tests/
--rw-r--r--   0 takwolf    (501) staff       (20)      716 2023-05-04 15:39:47.000000 bdffont-0.0.1/tests/test_spec.py
+drwxr-xr-x   0 takwolf    (502) staff       (20)        0 2023-05-05 07:48:30.077327 bdffont-0.0.2/
+-rw-r--r--   0 takwolf    (502) staff       (20)     1064 2023-05-03 16:58:01.000000 bdffont-0.0.2/LICENSE
+-rw-r--r--   0 takwolf    (502) staff       (20)     2502 2023-05-05 07:48:30.077146 bdffont-0.0.2/PKG-INFO
+-rw-r--r--   0 takwolf    (502) staff       (20)     1908 2023-05-05 06:55:00.000000 bdffont-0.0.2/README.md
+-rw-r--r--   0 takwolf    (502) staff       (20)      670 2023-05-05 07:43:52.000000 bdffont-0.0.2/pyproject.toml
+-rw-r--r--   0 takwolf    (502) staff       (20)       38 2023-05-05 07:48:30.077382 bdffont-0.0.2/setup.cfg
+drwxr-xr-x   0 takwolf    (502) staff       (20)        0 2023-05-05 07:48:30.072027 bdffont-0.0.2/src/
+drwxr-xr-x   0 takwolf    (502) staff       (20)        0 2023-05-05 07:48:30.074859 bdffont-0.0.2/src/bdffont/
+-rw-r--r--   0 takwolf    (502) staff       (20)      177 2023-05-05 04:46:00.000000 bdffont-0.0.2/src/bdffont/__init__.py
+-rw-r--r--   0 takwolf    (502) staff       (20)      691 2023-05-05 06:07:54.000000 bdffont-0.0.2/src/bdffont/error.py
+-rw-r--r--   0 takwolf    (502) staff       (20)     6132 2023-05-05 07:26:02.000000 bdffont-0.0.2/src/bdffont/font.py
+-rw-r--r--   0 takwolf    (502) staff       (20)     3144 2023-05-05 07:26:02.000000 bdffont-0.0.2/src/bdffont/glyph.py
+-rw-r--r--   0 takwolf    (502) staff       (20)     5775 2023-05-05 07:26:02.000000 bdffont-0.0.2/src/bdffont/parser.py
+-rw-r--r--   0 takwolf    (502) staff       (20)     3394 2023-05-05 05:41:07.000000 bdffont-0.0.2/src/bdffont/properties.py
+drwxr-xr-x   0 takwolf    (502) staff       (20)        0 2023-05-05 07:48:30.076046 bdffont-0.0.2/src/bdffont.egg-info/
+-rw-r--r--   0 takwolf    (502) staff       (20)     2502 2023-05-05 07:48:30.000000 bdffont-0.0.2/src/bdffont.egg-info/PKG-INFO
+-rw-r--r--   0 takwolf    (502) staff       (20)      347 2023-05-05 07:48:30.000000 bdffont-0.0.2/src/bdffont.egg-info/SOURCES.txt
+-rw-r--r--   0 takwolf    (502) staff       (20)        1 2023-05-05 07:48:30.000000 bdffont-0.0.2/src/bdffont.egg-info/dependency_links.txt
+-rw-r--r--   0 takwolf    (502) staff       (20)        8 2023-05-05 07:48:30.000000 bdffont-0.0.2/src/bdffont.egg-info/top_level.txt
+drwxr-xr-x   0 takwolf    (502) staff       (20)        0 2023-05-05 07:48:30.076774 bdffont-0.0.2/tests/
+-rw-r--r--   0 takwolf    (502) staff       (20)     1967 2023-05-05 06:21:06.000000 bdffont-0.0.2/tests/test_damaged.py
+-rw-r--r--   0 takwolf    (502) staff       (20)     1463 2023-05-05 06:56:12.000000 bdffont-0.0.2/tests/test_demo.py
```

### Comparing `bdffont-0.0.1/LICENSE` & `bdffont-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `bdffont-0.0.1/pyproject.toml` & `bdffont-0.0.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "bdffont"
-version = "0.0.1"
+version = "0.0.2"
 description = "A library for manipulating '.bdf' format fonts."
 readme = "README.md"
 license = { text = "MIT License" }
 requires-python = ">=3.10"
 authors = [
     { name = "TakWolf" },
 ]
```

### Comparing `bdffont-0.0.1/src/bdffont/font.py` & `bdffont-0.0.2/src/bdffont/font.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
-from bdffont import common
 from bdffont.properties import BdfProperties
 from bdffont.glyph import BdfGlyph
+from bdffont.error import BdfGlyphExists
 
 
 class BdfFont:
     # The BDF Specification version.
     spec_version: str
 
     # Either the 'X logical font description' or some private font name.
@@ -121,70 +121,62 @@
         self.size[3] = y
 
     def get_glyph(self, code_point: int) -> BdfGlyph:
         return self.code_point_to_glyph.get(code_point, None)
 
     def add_glyph(self, glyph: BdfGlyph):
         if glyph.code_point in self.code_point_to_glyph:
-            common.raise_glyph_already_exists_exception(glyph.code_point)
+            raise BdfGlyphExists(glyph.code_point)
         self.code_point_to_glyph[glyph.code_point] = glyph
 
     def set_glyph(self, glyph: BdfGlyph):
         self.code_point_to_glyph[glyph.code_point] = glyph
 
     def remove_glyph(self, code_point: int) -> BdfGlyph:
         return self.code_point_to_glyph.pop(code_point, None)
 
-    def encode(self) -> str:
-        lines = []
-        lines.append(f'STARTFONT {self.spec_version}')
+    def encode(self) -> list[str]:
+        lines = [
+            f'STARTFONT {self.spec_version}',
+        ]
         for comment in self.comments:
             lines.append(f'COMMENT {comment}')
         lines.append(f'FONT {self.name}')
         lines.append(f'SIZE {self.size[0]} {self.size[1]} {self.size[2]}')
         lines.append(f'FONTBOUNDINGBOX {self.bounding_box[0]} {self.bounding_box[1]} {self.bounding_box[2]} {self.bounding_box[3]}')
 
         lines.append(f'STARTPROPERTIES {len(self.properties)}')
         for comment in self.properties.comments:
             lines.append(f'COMMENT {comment}')
         for word, value in self.properties.items():
             if isinstance(value, str):
-                lines.append(f'{word} "{value}"')
-            else:
-                lines.append(f'{word} {value}')
+                value = f'"{value}"'
+            lines.append(f'{word} {value}')
         lines.append('ENDPROPERTIES')
 
-        alphabet = list(self.code_point_to_glyph.keys())
+        alphabet = list(self.code_point_to_glyph.items())
         alphabet.sort()
         lines.append(f'CHARS {len(alphabet)}')
-        for code_point in alphabet:
-            glyph = self.code_point_to_glyph[code_point]
+        for code_point, glyph in alphabet:
             lines.append(f'STARTCHAR {glyph.name}')
             for comment in glyph.comments:
                 lines.append(f'COMMENT {comment}')
             lines.append(f'ENCODING {code_point}')
             lines.append(f'SWIDTH {glyph.s_width[0]} {glyph.s_width[1]}')
             lines.append(f'DWIDTH {glyph.d_width[0]} {glyph.d_width[1]}')
             lines.append(f'BBX {glyph.bbx[0]} {glyph.bbx[1]} {glyph.bbx[2]} {glyph.bbx[3]}')
             lines.append('BITMAP')
-            for bitmap_row in glyph.bitmap:
-                binary_text = ''
-                for alpha in bitmap_row:
-                    if alpha == 0:
-                        binary_text += '0'
-                    else:
-                        binary_text += '1'
-                remainder = len(binary_text) % 8
-                if remainder > 0:
-                    for _ in range(8 - remainder):
-                        binary_text += '0'
-                format_string = '{:0' + str(len(binary_text) // 4) + 'X}'
-                lines.append(format_string.format(int(binary_text, 2)))
+            for bitmap_row in glyph.get_padding_bitmap():
+                hex_format = '{:0' + str(len(bitmap_row) // 4) + 'X}'
+                lines.append(hex_format.format(int(''.join(map(str, bitmap_row)), 2)))
             lines.append('ENDCHAR')
 
         lines.append('ENDFONT')
         lines.append('')
-        return '\n'.join(lines)
+        return lines
+
+    def encode_str(self) -> str:
+        return '\n'.join(self.encode())
 
     def save(self, file_path):
         with open(file_path, 'w', encoding='utf-8') as file:
-            file.write(self.encode())
+            file.write(self.encode_str())
```

### Comparing `bdffont-0.0.1/src/bdffont/glyph.py` & `bdffont-0.0.2/src/bdffont/glyph.py`

 * *Files 13% similar despite different names*

```diff
@@ -4,38 +4,33 @@
     # Example: quoteright
     name: str
 
     # Code point in Unicode.
     # Example: 39
     code_point: int
 
-    # The scalable width in x and y of character.
-    # Scalable widths are in units of 1/1000th of the size of the character.
-    # If the size of the character is p points, the width information must be scaled by p/1000 to get
-    # the width of the character in printer’s points.
-    # This width information should be considered as a vector indicating the position of the next
-    # character’s origin relative to the origin of this character.
+    # The scalable width in x and y of character. Scalable widths are in units of 1/1000th of the size of
+    # the character. If the size of the character is p points, the width information must be scaled by p/1000
+    # to get the width of the character in printer’s points. This width information should be considered as a
+    # vector indicating the position of the next character’s origin relative to the origin of this character.
     # To convert the scalable width to the width in device pixels, multiply s_width times p/1000 times r/72,
-    # where r is the device resolution in pixels per inch.
-    # The result is a real number giving the ideal print width in device pixels.
-    # The actual device width must of course be an integral number of device pixels and is given in the next entry.
-    # The s_width y value should always be zero for a standard X font.
+    # where r is the device resolution in pixels per inch. The result is a real number giving the ideal print
+    # width in device pixels. The actual device width must of course be an integral number of device pixels and
+    # is given in the next entry. The s_width y value should always be zero for a standard X font.
     s_width: (int, int)
 
-    # The width in x and y of the character in device units.
-    # Like the s_width, this width information is a vector indicating the position of the next character’s origin
-    # relative to the origin of this character.
-    # Note that the d_width of a given "hand-tuned" WYSIWYG glyph may deviate slightly from its ideal
-    # device-independent width given by s_width in order to improve its typographic characteristics
-    # on a display.
-    # The d_width y value should always be zero for a standard X font.
+    # The width in x and y of the character in device units. Like the s_width, this width information is a vector
+    # indicating the position of the next character’s origin relative to the origin of this character. Note that
+    # the d_width of a given "hand-tuned" WYSIWYG glyph may deviate slightly from its ideal device-independent width
+    # given by s_width in order to improve its typographic characteristics on a display. The d_width y value should
+    # always be zero for a standard X font.
     d_width: (int, int)
 
-    # The width in x (BBw), height in y (BBh), and x and y displacement (BBox, BBoy) of the lower left corner
-    # from the origin of the character.
+    # The width in x (BBw), height in y (BBh), and x and y displacement (BBox, BBoy) of the lower left corner from
+    # the origin of the character.
     bbx: (int, int, int, int)
 
     # The bitmap object.
     bitmap: list[list[int]]
 
     # Comments.
     comments: list[str]
@@ -59,7 +54,23 @@
             self.bitmap = []
         else:
             self.bitmap = bitmap
         if comments is None:
             self.comments = []
         else:
             self.comments = comments
+
+    def get_padding_bitmap(self) -> list[list[int]]:
+        padding_bitmap = []
+        for bitmap_row in self.bitmap:
+            padding_bitmap_row = []
+            for alpha in bitmap_row:
+                if alpha == 0:
+                    padding_bitmap_row.append(0)
+                else:
+                    padding_bitmap_row.append(1)
+            remainder = len(bitmap_row) % 8
+            if remainder > 0:
+                for _ in range(8 - remainder):
+                    padding_bitmap_row.append(0)
+            padding_bitmap.append(padding_bitmap_row)
+        return padding_bitmap
```

