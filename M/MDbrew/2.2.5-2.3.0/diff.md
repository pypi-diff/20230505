# Comparing `tmp/MDbrew-2.2.5.tar.gz` & `tmp/MDbrew-2.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/MDbrew-2.2.5.tar", last modified: Thu May  4 05:34:49 2023, max compression
+gzip compressed data, was "MDbrew-2.3.0.tar", last modified: Fri May  5 11:52:39 2023, max compression
```

## Comparing `MDbrew-2.2.5.tar` & `MDbrew-2.3.0.tar`

### file list

```diff
@@ -1,38 +1,37 @@
-drwxrwx---   0 minu928   (1216) minu928   (1216)        0 2023-05-04 05:31:31.000000 MDbrew-2.2.5/
--rw-rw----   0 minu928   (1216) minu928   (1216)       24 2023-05-03 12:53:55.000000 MDbrew-2.2.5/MANIFEST.in
-drwxrwx---   0 minu928   (1216) minu928   (1216)        0 2023-05-04 05:31:31.000000 MDbrew-2.2.5/MDbrew.egg-info/
--rw-rw----   0 minu928   (1216) minu928   (1216)      388 2023-05-04 05:31:31.000000 MDbrew-2.2.5/MDbrew.egg-info/PKG-INFO
--rw-rw----   0 minu928   (1216) minu928   (1216)        1 2023-05-04 05:31:31.000000 MDbrew-2.2.5/MDbrew.egg-info/not-zip-safe
--rw-rw----   0 minu928   (1216) minu928   (1216)      706 2023-05-04 05:31:31.000000 MDbrew-2.2.5/MDbrew.egg-info/SOURCES.txt
--rw-rw----   0 minu928   (1216) minu928   (1216)        1 2023-05-04 05:31:31.000000 MDbrew-2.2.5/MDbrew.egg-info/dependency_links.txt
--rw-rw----   0 minu928   (1216) minu928   (1216)        7 2023-05-04 05:31:31.000000 MDbrew-2.2.5/MDbrew.egg-info/top_level.txt
-drwxrwx---   0 minu928   (1216) minu928   (1216)        0 2023-05-04 05:31:31.000000 MDbrew-2.2.5/MDbrew/
-drwxrwx---   0 minu928   (1216) minu928   (1216)        0 2023-05-04 05:31:31.000000 MDbrew-2.2.5/MDbrew/tool/
--rw-rw----   0 minu928   (1216) minu928   (1216)        0 2023-05-04 05:30:46.000000 MDbrew-2.2.5/MDbrew/tool/__init__.py
--rw-rw----   0 minu928   (1216) minu928   (1216)     3545 2023-05-04 05:30:46.000000 MDbrew-2.2.5/MDbrew/tool/colorfont.py
--rw-rw----   0 minu928   (1216) minu928   (1216)      761 2023-05-04 05:30:46.000000 MDbrew-2.2.5/MDbrew/tool/doctor.py
--rw-rw----   0 minu928   (1216) minu928   (1216)      947 2023-05-04 05:30:46.000000 MDbrew-2.2.5/MDbrew/tool/decorator.py
--rw-rw----   0 minu928   (1216) minu928   (1216)      599 2023-05-04 05:30:46.000000 MDbrew-2.2.5/MDbrew/tool/spacer.py
-drwxrwx---   0 minu928   (1216) minu928   (1216)        0 2023-05-04 05:31:31.000000 MDbrew-2.2.5/MDbrew/application/
--rw-rw----   0 minu928   (1216) minu928   (1216)        0 2023-05-04 05:30:46.000000 MDbrew-2.2.5/MDbrew/application/__init__.py
--rw-rw----   0 minu928   (1216) minu928   (1216)     9449 2023-05-04 05:30:46.000000 MDbrew-2.2.5/MDbrew/application/brewcp2k.py
-drwxrwx---   0 minu928   (1216) minu928   (1216)        0 2023-05-04 05:31:31.000000 MDbrew-2.2.5/MDbrew/analysis/
--rw-rw----   0 minu928   (1216) minu928   (1216)     4342 2023-05-04 05:30:46.000000 MDbrew-2.2.5/MDbrew/analysis/msd.py
--rw-rw----   0 minu928   (1216) minu928   (1216)     5475 2023-05-04 05:30:46.000000 MDbrew-2.2.5/MDbrew/analysis/rdf.py
--rw-rw----   0 minu928   (1216) minu928   (1216)        0 2023-05-04 05:30:46.000000 MDbrew-2.2.5/MDbrew/analysis/__init__.py
-drwxrwx---   0 minu928   (1216) minu928   (1216)        0 2023-05-04 05:31:31.000000 MDbrew-2.2.5/MDbrew/main/
--rw-rw----   0 minu928   (1216) minu928   (1216)        0 2023-05-04 05:30:46.000000 MDbrew-2.2.5/MDbrew/main/__init__.py
--rw-rw----   0 minu928   (1216) minu928   (1216)     2605 2023-05-04 05:30:46.000000 MDbrew-2.2.5/MDbrew/main/brewer.py
-drwxrwx---   0 minu928   (1216) minu928   (1216)        0 2023-05-04 05:31:31.000000 MDbrew-2.2.5/MDbrew/main/filetype/
--rw-rw----   0 minu928   (1216) minu928   (1216)      712 2023-05-04 05:30:46.000000 MDbrew-2.2.5/MDbrew/main/filetype/pdb.py
--rw-rw----   0 minu928   (1216) minu928   (1216)     1291 2023-05-04 05:30:46.000000 MDbrew-2.2.5/MDbrew/main/filetype/vasp.py
--rw-rw----   0 minu928   (1216) minu928   (1216)        0 2023-05-04 05:30:46.000000 MDbrew-2.2.5/MDbrew/main/filetype/__init__.py
--rw-rw----   0 minu928   (1216) minu928   (1216)      838 2023-05-04 05:30:46.000000 MDbrew-2.2.5/MDbrew/main/filetype/lmps.py
--rw-rw----   0 minu928   (1216) minu928   (1216)      431 2023-05-04 05:30:46.000000 MDbrew-2.2.5/MDbrew/main/filetype/xyz.py
--rw-rw----   0 minu928   (1216) minu928   (1216)     4183 2023-05-04 05:30:46.000000 MDbrew-2.2.5/MDbrew/main/brewery.py
--rw-rw----   0 minu928   (1216) minu928   (1216)     1960 2023-05-04 05:30:46.000000 MDbrew-2.2.5/MDbrew/main/opener.py
--rw-rw----   0 minu928   (1216) minu928   (1216)      229 2023-05-04 05:30:46.000000 MDbrew-2.2.5/MDbrew/__init__.py
--rw-rw----   0 minu928   (1216) minu928   (1216)      388 2023-05-04 05:31:31.000000 MDbrew-2.2.5/PKG-INFO
--rw-rw----   0 minu928   (1216) minu928   (1216)      631 2023-05-04 05:31:13.000000 MDbrew-2.2.5/setup.py
--rw-rw----   0 minu928   (1216) minu928   (1216)       79 2023-05-04 05:31:31.000000 MDbrew-2.2.5/setup.cfg
--rw-rw----   0 minu928   (1216) minu928   (1216)       58 2023-05-03 12:53:56.000000 MDbrew-2.2.5/requirement.txt
+drwxr-xr-x   0 minu       (501) staff       (20)        0 2023-05-05 11:52:39.305372 MDbrew-2.3.0/
+-rw-r--r--   0 minu       (501) staff       (20)       25 2023-05-05 06:22:51.000000 MDbrew-2.3.0/MANIFEST.in
+drwxr-xr-x   0 minu       (501) staff       (20)        0 2023-05-05 11:52:39.302404 MDbrew-2.3.0/MDbrew/
+-rw-r--r--   0 minu       (501) staff       (20)      238 2023-05-05 11:52:26.000000 MDbrew-2.3.0/MDbrew/__init__.py
+drwxr-xr-x   0 minu       (501) staff       (20)        0 2023-05-05 11:52:39.303470 MDbrew-2.3.0/MDbrew/analysis/
+-rw-r--r--   0 minu       (501) staff       (20)        0 2023-05-05 11:50:38.000000 MDbrew-2.3.0/MDbrew/analysis/__init__.py
+-rw-r--r--   0 minu       (501) staff       (20)     4477 2023-05-05 11:50:38.000000 MDbrew-2.3.0/MDbrew/analysis/msd.py
+-rw-r--r--   0 minu       (501) staff       (20)     5860 2023-05-05 11:50:38.000000 MDbrew-2.3.0/MDbrew/analysis/rdf.py
+drwxr-xr-x   0 minu       (501) staff       (20)        0 2023-05-05 11:52:39.303723 MDbrew-2.3.0/MDbrew/application/
+-rw-r--r--   0 minu       (501) staff       (20)        0 2023-05-05 11:50:38.000000 MDbrew-2.3.0/MDbrew/application/__init__.py
+-rw-r--r--   0 minu       (501) staff       (20)     9705 2023-05-05 11:50:38.000000 MDbrew-2.3.0/MDbrew/application/brewcp2k.py
+drwxr-xr-x   0 minu       (501) staff       (20)        0 2023-05-05 11:52:39.304063 MDbrew-2.3.0/MDbrew/main/
+-rw-r--r--   0 minu       (501) staff       (20)        0 2023-05-05 11:50:38.000000 MDbrew-2.3.0/MDbrew/main/__init__.py
+-rw-r--r--   0 minu       (501) staff       (20)     4770 2023-05-05 11:50:38.000000 MDbrew-2.3.0/MDbrew/main/brewery.py
+drwxr-xr-x   0 minu       (501) staff       (20)        0 2023-05-05 11:52:39.304660 MDbrew-2.3.0/MDbrew/main/filetype/
+-rw-r--r--   0 minu       (501) staff       (20)        0 2023-05-05 11:50:38.000000 MDbrew-2.3.0/MDbrew/main/filetype/__init__.py
+-rw-r--r--   0 minu       (501) staff       (20)      842 2023-05-05 11:50:38.000000 MDbrew-2.3.0/MDbrew/main/filetype/lmps.py
+-rw-r--r--   0 minu       (501) staff       (20)      715 2023-05-05 11:50:38.000000 MDbrew-2.3.0/MDbrew/main/filetype/pdb.py
+-rw-r--r--   0 minu       (501) staff       (20)     1309 2023-05-05 11:50:38.000000 MDbrew-2.3.0/MDbrew/main/filetype/vasp.py
+-rw-r--r--   0 minu       (501) staff       (20)      425 2023-05-05 11:50:38.000000 MDbrew-2.3.0/MDbrew/main/filetype/xyz.py
+-rw-r--r--   0 minu       (501) staff       (20)     1170 2023-05-05 11:50:38.000000 MDbrew-2.3.0/MDbrew/main/opener.py
+drwxr-xr-x   0 minu       (501) staff       (20)        0 2023-05-05 11:52:39.305263 MDbrew-2.3.0/MDbrew/tool/
+-rw-r--r--   0 minu       (501) staff       (20)        0 2023-05-05 11:50:38.000000 MDbrew-2.3.0/MDbrew/tool/__init__.py
+-rw-r--r--   0 minu       (501) staff       (20)     3618 2023-05-05 11:50:38.000000 MDbrew-2.3.0/MDbrew/tool/colorfont.py
+-rw-r--r--   0 minu       (501) staff       (20)     1578 2023-05-05 11:50:38.000000 MDbrew-2.3.0/MDbrew/tool/decorator.py
+-rw-r--r--   0 minu       (501) staff       (20)      752 2023-05-05 11:50:38.000000 MDbrew-2.3.0/MDbrew/tool/doctor.py
+-rw-r--r--   0 minu       (501) staff       (20)      619 2023-05-05 11:50:38.000000 MDbrew-2.3.0/MDbrew/tool/spacer.py
+drwxr-xr-x   0 minu       (501) staff       (20)        0 2023-05-05 11:52:39.303100 MDbrew-2.3.0/MDbrew.egg-info/
+-rw-r--r--   0 minu       (501) staff       (20)      332 2023-05-05 11:52:39.000000 MDbrew-2.3.0/MDbrew.egg-info/PKG-INFO
+-rw-r--r--   0 minu       (501) staff       (20)      684 2023-05-05 11:52:39.000000 MDbrew-2.3.0/MDbrew.egg-info/SOURCES.txt
+-rw-r--r--   0 minu       (501) staff       (20)        1 2023-05-05 11:52:39.000000 MDbrew-2.3.0/MDbrew.egg-info/dependency_links.txt
+-rw-r--r--   0 minu       (501) staff       (20)        1 2023-05-05 11:52:02.000000 MDbrew-2.3.0/MDbrew.egg-info/not-zip-safe
+-rw-r--r--   0 minu       (501) staff       (20)        7 2023-05-05 11:52:39.000000 MDbrew-2.3.0/MDbrew.egg-info/top_level.txt
+-rw-r--r--   0 minu       (501) staff       (20)      332 2023-05-05 11:52:39.305464 MDbrew-2.3.0/PKG-INFO
+-rw-r--r--   0 minu       (501) staff       (20)       62 2023-05-05 06:22:51.000000 MDbrew-2.3.0/requirement.txt
+-rw-r--r--   0 minu       (501) staff       (20)       79 2023-05-05 11:52:39.305722 MDbrew-2.3.0/setup.cfg
+-rw-r--r--   0 minu       (501) staff       (20)      653 2023-05-05 11:51:29.000000 MDbrew-2.3.0/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `MDbrew-2.2.5/MDbrew.egg-info/SOURCES.txt` & `MDbrew-2.3.0/MDbrew.egg-info/SOURCES.txt`

 * *Files 13% similar despite different names*

```diff
@@ -10,15 +10,14 @@
 MDbrew.egg-info/top_level.txt
 MDbrew/analysis/__init__.py
 MDbrew/analysis/msd.py
 MDbrew/analysis/rdf.py
 MDbrew/application/__init__.py
 MDbrew/application/brewcp2k.py
 MDbrew/main/__init__.py
-MDbrew/main/brewer.py
 MDbrew/main/brewery.py
 MDbrew/main/opener.py
 MDbrew/main/filetype/__init__.py
 MDbrew/main/filetype/lmps.py
 MDbrew/main/filetype/pdb.py
 MDbrew/main/filetype/vasp.py
 MDbrew/main/filetype/xyz.py
```

### Comparing `MDbrew-2.2.5/MDbrew/tool/colorfont.py` & `MDbrew-2.3.0/MDbrew/tool/colorfont.py`

 * *Ordering differences only*

 * *Files 6% similar despite different names*

```diff
@@ -1,73 +1,73 @@
-class ColorFont:
-    _color_map = {
-        "black": 30,
-        "red": 31,
-        "green": 32,
-        "yellow": 33,
-        "blue": 34,
-        "magenta": 35,
-        "cyan": 36,
-        "white": 37,
-    }
-
-    def __init__(self) -> None:
-        self.__font_shape__()
-        self.__font_color__()
-        self.__font_bright_color__()
-        self.__background_color__()
-        self.__background_color__()
-
-    def pick_color(self, name, bright: bool = False, bg: str = False):
-        color = self._color_map[name]
-        color = color + 60 if bright else color
-        color = color + 10 if bg else color
-        return f"\033[{color}m"
-
-    def __font_shape__(self):
-        self.reset = "\033[0m"
-        self.bold = "\033[1m"
-        self.itatilc = "\033[3m"
-        self.underline = "\033[4m"
-
-    def __font_color__(self):
-        self.font_black = self.pick_color("black", bright=False, bg=False)
-        self.font_red = self.pick_color("red", bright=False, bg=False)
-        self.font_green = self.pick_color("green", bright=False, bg=False)
-        self.font_yellow = self.pick_color("yellow", bright=False, bg=False)
-        self.font_blue = self.pick_color("blue", bright=False, bg=False)
-        self.font_magenta = self.pick_color("magenta", bright=False, bg=False)
-        self.font_cyan = self.pick_color("cyan", bright=False, bg=False)
-        self.font_white = self.pick_color("white", bright=False, bg=False)
-
-    def __font_bright_color__(self):
-        self.font_bright_black = self.pick_color("black", bright=True, bg=False)
-        self.font_bright_red = self.pick_color("red", bright=True, bg=False)
-        self.font_bright_green = self.pick_color("green", bright=True, bg=False)
-        self.font_bright_yellow = self.pick_color("yellow", bright=True, bg=False)
-        self.font_bright_blue = self.pick_color("blue", bright=True, bg=False)
-        self.font_bright_magenta = self.pick_color("magenta", bright=True, bg=False)
-        self.font_bright_cyan = self.pick_color("cyan", bright=True, bg=False)
-        self.font_bright_white = self.pick_color("white", bright=True, bg=False)
-
-    def __background_color__(self):
-        self.background_black = self.pick_color("black", bright=False, bg=True)
-        self.background_red = self.pick_color("red", bright=False, bg=True)
-        self.background_green = self.pick_color("green", bright=False, bg=True)
-        self.background_yellow = self.pick_color("yellow", bright=False, bg=True)
-        self.background_blue = self.pick_color("blue", bright=False, bg=True)
-        self.background_magenta = self.pick_color("magenta", bright=False, bg=True)
-        self.background_cyan = self.pick_color("cyan", bright=False, bg=True)
-        self.background_white = self.pick_color("white", bright=False, bg=True)
-
-    def __background_bright_color__(self):
-        self.background_bright_black = self.pick_color("black", bright=True, bg=True)
-        self.background_bright_red = self.pick_color("red", bright=True, bg=True)
-        self.background_bright_green = self.pick_color("green", bright=True, bg=True)
-        self.background_bright_yellow = self.pick_color("yellow", bright=True, bg=True)
-        self.background_bright_blue = self.pick_color("blue", bright=True, bg=True)
-        self.background_bright_magenta = self.pick_color("magenta", bright=True, bg=True)
-        self.background_bright_cyan = self.pick_color("cyan", bright=True, bg=True)
-        self.background_bright_white = self.pick_color("white", bright=True, bg=True)
-
-
-color = ColorFont()
+class ColorFont:
+    _color_map = {
+        "black": 30,
+        "red": 31,
+        "green": 32,
+        "yellow": 33,
+        "blue": 34,
+        "magenta": 35,
+        "cyan": 36,
+        "white": 37,
+    }
+
+    def __init__(self) -> None:
+        self.__font_shape__()
+        self.__font_color__()
+        self.__font_bright_color__()
+        self.__background_color__()
+        self.__background_color__()
+
+    def pick_color(self, name, bright: bool = False, bg: str = False):
+        color = self._color_map[name]
+        color = color + 60 if bright else color
+        color = color + 10 if bg else color
+        return f"\033[{color}m"
+
+    def __font_shape__(self):
+        self.reset = "\033[0m"
+        self.bold = "\033[1m"
+        self.itatilc = "\033[3m"
+        self.underline = "\033[4m"
+
+    def __font_color__(self):
+        self.font_black = self.pick_color("black", bright=False, bg=False)
+        self.font_red = self.pick_color("red", bright=False, bg=False)
+        self.font_green = self.pick_color("green", bright=False, bg=False)
+        self.font_yellow = self.pick_color("yellow", bright=False, bg=False)
+        self.font_blue = self.pick_color("blue", bright=False, bg=False)
+        self.font_magenta = self.pick_color("magenta", bright=False, bg=False)
+        self.font_cyan = self.pick_color("cyan", bright=False, bg=False)
+        self.font_white = self.pick_color("white", bright=False, bg=False)
+
+    def __font_bright_color__(self):
+        self.font_bright_black = self.pick_color("black", bright=True, bg=False)
+        self.font_bright_red = self.pick_color("red", bright=True, bg=False)
+        self.font_bright_green = self.pick_color("green", bright=True, bg=False)
+        self.font_bright_yellow = self.pick_color("yellow", bright=True, bg=False)
+        self.font_bright_blue = self.pick_color("blue", bright=True, bg=False)
+        self.font_bright_magenta = self.pick_color("magenta", bright=True, bg=False)
+        self.font_bright_cyan = self.pick_color("cyan", bright=True, bg=False)
+        self.font_bright_white = self.pick_color("white", bright=True, bg=False)
+
+    def __background_color__(self):
+        self.background_black = self.pick_color("black", bright=False, bg=True)
+        self.background_red = self.pick_color("red", bright=False, bg=True)
+        self.background_green = self.pick_color("green", bright=False, bg=True)
+        self.background_yellow = self.pick_color("yellow", bright=False, bg=True)
+        self.background_blue = self.pick_color("blue", bright=False, bg=True)
+        self.background_magenta = self.pick_color("magenta", bright=False, bg=True)
+        self.background_cyan = self.pick_color("cyan", bright=False, bg=True)
+        self.background_white = self.pick_color("white", bright=False, bg=True)
+
+    def __background_bright_color__(self):
+        self.background_bright_black = self.pick_color("black", bright=True, bg=True)
+        self.background_bright_red = self.pick_color("red", bright=True, bg=True)
+        self.background_bright_green = self.pick_color("green", bright=True, bg=True)
+        self.background_bright_yellow = self.pick_color("yellow", bright=True, bg=True)
+        self.background_bright_blue = self.pick_color("blue", bright=True, bg=True)
+        self.background_bright_magenta = self.pick_color("magenta", bright=True, bg=True)
+        self.background_bright_cyan = self.pick_color("cyan", bright=True, bg=True)
+        self.background_bright_white = self.pick_color("white", bright=True, bg=True)
+
+
+color = ColorFont()
```

### Comparing `MDbrew-2.2.5/MDbrew/tool/doctor.py` & `MDbrew-2.3.0/MDbrew/tool/doctor.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,25 +1,25 @@
-from ..analysis.msd import MSD
-from ..analysis.rdf import RDF
-from ..main.brewery import Brewery
-from .colorfont import color
-
-
-def doctor(path):
-    LINE_WIDTH = 60
-    sep_line = "=" * LINE_WIDTH
-    print(sep_line)
-    mb = Brewery(path=path, is_generator=True)
-    coords = mb.coords
-    atom_info = mb.atom_info
-    order1 = mb.order(what="type == 1")
-    order2 = mb.order(what="type == 2")
-    print(sep_line)
-    position = order1.reorder().coords
-    ixiyiz = order1.reorder().brew(cols=["ix", "iy", "iz"])
-    unwrapped_position = [pos + ixyz for pos, ixyz in zip(position, ixiyiz)]
-    rdf = RDF(order1, order2, mb.box_size, max_frame=100).run()
-    rdf.result
-    msd = MSD(unwrapped_position).run()
-    msd.result
-    print(sep_line)
-    print(mb)
+from ..analysis.msd import MSD
+from ..analysis.rdf import RDF
+from ..main.brewery import Brewery
+from .colorfont import color
+
+
+def doctor(path):
+    LINE_WIDTH = 60
+    sep_line = "=" * LINE_WIDTH
+    print(sep_line)
+    mb = Brewery(path=path, fmt="lmps")
+    coords = mb.coords
+    atom_info = mb.atom_info
+    order1 = mb.order(what="type == 1")
+    order2 = mb.order(what="type == 2")
+    print(sep_line)
+    position = order1.coords
+    ixiyiz = order1.brew(cols=["ix", "iy", "iz"])
+    unwrapped_position = [position + ixiyiz for _ in order1.frange()]
+    rdf = RDF(order1, order2, mb.box_size, max_frame=100).run()
+    rdf.result
+    msd = MSD(unwrapped_position).run()
+    msd.result
+    print(sep_line)
+    print(mb)
```

### Comparing `MDbrew-2.2.5/MDbrew/tool/decorator.py` & `MDbrew-2.3.0/MDbrew/tool/decorator.py`

 * *Files 22% similar despite different names*

```diff
@@ -9,21 +9,40 @@
     TAB_SIZE = 8
     str_number = len(name)
     tab_number = str_number // TAB_SIZE
     return 3 - tab_number
 
 
 # Wrapper of count the function execution time
-def color_print(name, verbose: bool = True):
+def color_print(name):
     def deco(func):
         def inner(*args, **kwrgs):
+            print(f"[ {color.font_green}RUNN{color.reset} ] {name}", end="\r")
+            start = time()
+            result = func(*args, **kwrgs)
+            end = time()
+            end_string = f"[ {color.font_red}DONE{color.reset} ] {name}"
+            end_string += "\t" * check_tab(name=name) + f" -> {end - start :5.2f} s \u2705"
+            print(end_string)
+            return result
+
+        return inner
+
+    return deco
+
+
+# Wrapper of count the function execution time
+def color_print_verbose(name):
+    def deco(func):
+        def inner(*args, **kwrgs):
+            verbose = kwrgs.pop("verbose", True)
             if verbose:
                 print(f"[ {color.font_green}RUNN{color.reset} ] {name}", end="\r")
                 start = time()
-            result = func(*args, **kwrgs)
+            result = func(verbose=verbose, *args, **kwrgs)
             if verbose:
                 end = time()
                 end_string = f"[ {color.font_red}DONE{color.reset} ] {name}"
                 end_string += "\t" * check_tab(name=name) + f" -> {end - start :5.2f} s \u2705"
                 print(end_string)
             return result
```

### Comparing `MDbrew-2.2.5/MDbrew/tool/spacer.py` & `MDbrew-2.3.0/MDbrew/tool/spacer.py`

 * *Ordering differences only*

 * *Files 13% similar despite different names*

```diff
@@ -1,20 +1,20 @@
-import numpy as np
-
-__all__ = ["check_dimension", "get_diff_position", "get_distance"]
-
-
-# Dimension checker
-def check_dimension(array, dim: int):
-    new_array = np.asarray(array, dtype=np.float64)
-    assert new_array.ndim == dim, "[DimensionError] Check your dimension "
-    return new_array
-
-
-# get difference of position A & B
-def get_diff_position(a_position, b_position):
-    return np.subtract(a_position, b_position, dtype=np.float64)
-
-
-# get distance from difference position
-def get_distance(diff_position, axis: int = -1):
-    return np.sqrt(np.sum(np.square(diff_position), axis=axis))
+import numpy as np
+
+__all__ = ["check_dimension", "get_diff_position", "get_distance"]
+
+
+# Dimension checker
+def check_dimension(array, dim: int):
+    new_array = np.asarray(array, dtype=np.float64)
+    assert new_array.ndim == dim, "[DimensionError] Check your dimension "
+    return new_array
+
+
+# get difference of position A & B
+def get_diff_position(a_position, b_position):
+    return np.subtract(a_position, b_position, dtype=np.float64)
+
+
+# get distance from difference position
+def get_distance(diff_position, axis: int = -1):
+    return np.sqrt(np.sum(np.square(diff_position), axis=axis))
```

### Comparing `MDbrew-2.2.5/MDbrew/application/brewcp2k.py` & `MDbrew-2.3.0/MDbrew/application/brewcp2k.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,236 +1,236 @@
-#!/usr/bin/env python3
-import os
-import numpy as np
-from tqdm import tqdm
-from scipy import constants
-from ..main.brewery import Brewery
-from ..tool.colorfont import color
-from ..tool.decorator import color_print
-
-
-class BrewCP2K(object):
-    tqmd_option = {"ascii": " #"}
-    printing_option = {
-        "2array": f" #CONVERT  {color.font_yellow}List2Array{color.reset}",
-        "2a.u": f" #CONVERT  {color.font_yellow}Atomic Unit{color.reset}",
-        "save": f" #SAVE  {color.font_yellow}THE DATA{color.reset}",
-        "kind2type": f" #CONVERT  {color.font_yellow}KIND2TYPE{color.reset}",
-    }
-
-    def __init__(self, xyz_file, log_file, type_map: list["str"]) -> None:
-        self._type_map = type_map
-        self._brew_xyzfile(xyz_file=xyz_file)
-        self._brew_logfile(log_file=log_file)
-        self.__error__()
-        self._covert_kind2type()
-        self._change2array()
-        self._convert_unit()
-
-    @property
-    def virials(self):
-        return self._virial_list
-
-    @property
-    def forces(self):
-        return self._force_list
-
-    @property
-    def coords(self):
-        return self._coord_list
-
-    @property
-    def cells(self):
-        return self._cell_list
-
-    @property
-    def energies(self):
-        return self._energy_list
-
-    @property
-    def types(self):
-        return self._type_list
-
-    @property
-    def type_dict(self):
-        return self._type_dict
-
-    def __str__(self) -> str:
-        LINE_WIDTH = 60
-        sep_line = "=" * LINE_WIDTH
-        print("")
-        print(sep_line)
-        print("||" + " " * 22 + " INFO " + " " * 28 + "||")
-        print(sep_line)
-        print(f"\t[  CELL  ] : {self.is_contain_cell} || SHAPE {self.cells.shape}")
-        print(f"\t[ FORCES ] : {self.is_contain_force} || SHAPE {self.forces.shape}")
-        print(f"\t[ VIRIAL ] : {self.is_contain_stress} || SHAPE {self.virials.shape}")
-        print(f"\t[ COORDS ] : {self.is_contain_coord} || SHAPE {self.coords.shape}")
-        print(f"\t[ ENERGY ] : {self.is_contain_energy} || SHAPE {self.energies.shape}")
-        print(f"\t[  TYPE  ] : {self.is_contain_kind} || SHAPE {self.types.shape}")
-        print(sep_line)
-        return f"\t @CopyRight by  {color.font_blue}minu928@snu.ac.kr{color.reset}\n"
-
-    def __error__(self):
-        F_energy = len(self._energy_list)
-        F_stress = len(self._stress_list) / 3
-        F_coords = len(self._coord_list)
-        assert (
-            F_energy == F_stress == F_coords
-        ), f"Frame of Energy {F_energy}, Frame of Stress {F_stress} , Frame of Coords {F_coords}"
-        self._num_frame = F_energy
-        self._num_atom = len(self._force_list) / F_energy
-
-    @color_print(name=printing_option["save"])
-    def save_data(self, folder: str = "./", mode: str = "dpdata"):
-        folder = folder if folder[-1] == "/" else folder + "/"
-        data_path = os.path.join(folder, "set.000")
-        if not os.path.exists(data_path):
-            os.makedirs(data_path)
-        mode_list = ("dpdata", "raw")
-        mode = mode.lower()
-        energy_path = os.path.join(data_path, "energy.npy")
-        box_path = os.path.join(data_path, "box.npy")
-        virial_path = os.path.join(data_path, "virial.npy")
-        force_path = os.path.join(data_path, "force.npy")
-        coord_path = os.path.join(data_path, "coord.npy")
-        assert mode in mode_list, f"[ ERROR ] mode should be dpata, raw || Not {mode}"
-        if mode == "dpdata":
-            np.save(energy_path, self.energies)
-            np.save(box_path, self.cells.reshape(self._num_frame, 9))
-            np.save(virial_path, self.virials.reshape(self._num_frame, 9))
-            np.save(force_path, self.forces.reshape(self._num_frame, int(self._num_atom * 3)))
-            np.save(coord_path, self.coords.reshape(self._num_frame, int(self._num_atom * 3)))
-        elif mode == "raw":
-            np.save(energy_path, self.energies)
-            np.save(box_path, self.cells)
-            np.save(virial_path, self.virials)
-            np.save(force_path, self.forces)
-            np.save(coord_path, self.coords)
-        np.savetxt(folder + "type.raw", self.types, fmt="%d")
-        np.savetxt(folder + "type_map.raw", self._type_map, fmt="%s")
-
-    def _brew_xyzfile(self, xyz_file):
-        database = Brewery(path=xyz_file, fmt="xyz", is_generator=True).coords
-        line_range = tqdm(
-            database,
-            desc=f"[ {color.font_cyan}BREW{color.reset} ]  #{color.font_green}XYZ{color.reset} ",
-            **self.tqmd_option,
-        )
-        self._coord_list = [data for data in line_range]
-        self.is_contain_coord = True
-
-    def _brew_logfile(self, log_file):
-        # BASE for brewing
-        ## CELL
-        cell_keyword = "CELL| Vector "
-        self.is_contain_cell = False
-        self._cell_list = []
-        ## STRESS
-        stress_keyword = "STRESS| Analytical stress"
-        self.is_contain_stress = False
-        self._stress_list = []
-        ## ENERGY
-        energy_keyword = "ENERGY|"
-        self.is_contain_energy = False
-        self._energy_list = []
-        ## FORCE
-        force_keyword = " Atom   Kind "
-        self.is_contain_force = False
-        self._force_list = []
-        force_stop_keyword = "SUM OF ATOMIC FORCES"
-        force_iter_on = False
-        ## KIND
-        kind_keyword = " Atom  Kind "
-        self.is_contain_kind = False
-        self._kind_list = []
-        kind_stop_keyword = "\n"
-        kind_iter_on = False
-        # ITERATION
-        with open(log_file, "r") as f:
-            line_range = enumerate(
-                tqdm(
-                    f,
-                    **self.tqmd_option,
-                    desc=f"[ {color.font_cyan}BREW{color.reset} ]  #{color.font_green}LOG{color.reset} ",
-                )
-            )
-            for idx, line in line_range:
-                # CELL
-                if len(self._cell_list) < 3:
-                    if cell_keyword in line:
-                        self.is_contain_cell = True
-                        self._cell_list.append(line.split()[4:7])
-                        continue
-                # STRESS
-                if stress_keyword in line:
-                    self.is_contain_stress = True
-                    stress_idx = idx
-                if self.is_contain_stress and stress_idx + 5 > idx > stress_idx + 1:
-                    self._stress_list.append(line.split()[2:5])
-                    continue
-                # ENERGY
-                if energy_keyword in line:
-                    self.is_contain_energy = True
-                    self._energy_list.append(line.split()[8])
-                    continue
-                # FORCE
-                if force_keyword in line:
-                    force_idx = idx
-                    self.is_contain_force = True
-                    force_iter_on = True
-                    continue
-                if force_stop_keyword in line:
-                    force_iter_on = False
-                if force_iter_on and idx > force_idx:
-                    self._force_list.append(line.split()[3:6])
-                    continue
-                # TYPE
-                if not self.is_contain_kind:
-                    if kind_keyword in line:
-                        kind_idx = idx
-                        kind_iter_on = True
-                        continue
-                    if kind_iter_on and kind_stop_keyword == line:
-                        kind_iter_on = False
-                        self.is_contain_kind = True
-                    if kind_iter_on and idx > kind_idx:
-                        self._kind_list.append(line.split()[2])
-                        continue
-
-    @color_print(name=printing_option["2array"])
-    def _change2array(self, data_type: str = "float32"):
-        F = int(self._num_frame)
-        N = int(self._num_atom)
-        self._stress_list = np.array(self._stress_list).astype(data_type).reshape(F, 3, 3)
-        self._force_list = np.array(self._force_list).astype(data_type).reshape(F, N, 3)
-        self._cell_list = np.tile(self._cell_list, (self._num_frame, 1)).astype(data_type).reshape(F, 3, 3)
-        self._energy_list = np.array(self._energy_list).astype(data_type)
-        self._coord_list = np.array(self._coord_list).astype(data_type)
-        self._type_list = np.array(self._type_list).astype("int32")
-
-    @color_print(name=printing_option["2a.u"])
-    def _convert_unit(self):
-        ELE_CHG = constants.elementary_charge  # Elementary Charge, in C
-        HARTREE = constants.value("atomic unit of energy")  # Hartree, in Jole
-        BOHR = constants.value("atomic unit of length")  # Bohr, in m
-
-        eV = ELE_CHG  # eV
-        hatree2eV = HARTREE / ELE_CHG  # eV
-        J2eV = 1  # eV
-
-        angstrom = 1  # angstrom
-        m2angstrom = 1e-10 * angstrom  # angstrom
-        bohr2angstrom = BOHR / m2angstrom  # angstrom
-        GPa2eVangstorm = 1e-9 * J2eV / (m2angstrom**3) * eV  # eV / angstrom^3
-
-        self._energy_list *= hatree2eV
-        self._cell_list = self._cell_list
-        self._force_list *= hatree2eV / bohr2angstrom
-        volume = np.linalg.det(self._cell_list[0])
-        self._virial_list = self._stress_list * volume / GPa2eVangstorm
-        self._coord_list = self._coord_list
-
-    @color_print(name=printing_option["kind2type"])
-    def _covert_kind2type(self):
-        self._type_dict = {kind: idx for idx, kind in enumerate(self._type_map)}
-        self._type_list = [self._type_dict[kind] for kind in self._kind_list]
+#!/usr/bin/env python3
+import os
+import numpy as np
+from tqdm import tqdm
+from scipy import constants
+from ..main.brewery import Brewery
+from ..tool.colorfont import color
+from ..tool.decorator import color_print
+
+
+class BrewCP2K(object):
+    tqmd_option = {"ascii": " #"}
+    printing_option = {
+        "2array": f" #CONVERT  {color.font_yellow}List2Array{color.reset}",
+        "2a.u": f" #CONVERT  {color.font_yellow}Atomic Unit{color.reset}",
+        "save": f" #SAVE  {color.font_yellow}THE DATA{color.reset}",
+        "kind2type": f" #CONVERT  {color.font_yellow}KIND2TYPE{color.reset}",
+    }
+
+    def __init__(self, xyz_file, log_file, type_map: list["str"]) -> None:
+        self._type_map = type_map
+        self._brew_xyzfile(xyz_file=xyz_file)
+        self._brew_logfile(log_file=log_file)
+        self.__error__()
+        self._covert_kind2type()
+        self._change2array()
+        self._convert_unit()
+
+    @property
+    def virials(self):
+        return self._virial_list
+
+    @property
+    def forces(self):
+        return self._force_list
+
+    @property
+    def coords(self):
+        return self._coord_list
+
+    @property
+    def cells(self):
+        return self._cell_list
+
+    @property
+    def energies(self):
+        return self._energy_list
+
+    @property
+    def types(self):
+        return self._type_list
+
+    @property
+    def type_dict(self):
+        return self._type_dict
+
+    def __str__(self) -> str:
+        LINE_WIDTH = 60
+        sep_line = "=" * LINE_WIDTH
+        print("")
+        print(sep_line)
+        print("||" + " " * 22 + " INFO " + " " * 28 + "||")
+        print(sep_line)
+        print(f"\t[  CELL  ] : {self.is_contain_cell} || SHAPE {self.cells.shape}")
+        print(f"\t[ FORCES ] : {self.is_contain_force} || SHAPE {self.forces.shape}")
+        print(f"\t[ VIRIAL ] : {self.is_contain_stress} || SHAPE {self.virials.shape}")
+        print(f"\t[ COORDS ] : {self.is_contain_coord} || SHAPE {self.coords.shape}")
+        print(f"\t[ ENERGY ] : {self.is_contain_energy} || SHAPE {self.energies.shape}")
+        print(f"\t[  TYPE  ] : {self.is_contain_kind} || SHAPE {self.types.shape}")
+        print(sep_line)
+        return f"\t @CopyRight by  {color.font_blue}minu928@snu.ac.kr{color.reset}\n"
+
+    def __error__(self):
+        F_energy = len(self._energy_list)
+        F_stress = len(self._stress_list) / 3
+        F_coords = len(self._coord_list)
+        assert (
+            F_energy == F_stress == F_coords
+        ), f"Frame of Energy {F_energy}, Frame of Stress {F_stress} , Frame of Coords {F_coords}"
+        self._num_frame = F_energy
+        self._num_atom = len(self._force_list) / F_energy
+
+    @color_print(name=printing_option["save"])
+    def save_data(self, folder: str = "./", mode: str = "dpdata"):
+        folder = folder if folder[-1] == "/" else folder + "/"
+        data_path = os.path.join(folder, "set.000")
+        if not os.path.exists(data_path):
+            os.makedirs(data_path)
+        mode_list = ("dpdata", "raw")
+        mode = mode.lower()
+        energy_path = os.path.join(data_path, "energy.npy")
+        box_path = os.path.join(data_path, "box.npy")
+        virial_path = os.path.join(data_path, "virial.npy")
+        force_path = os.path.join(data_path, "force.npy")
+        coord_path = os.path.join(data_path, "coord.npy")
+        assert mode in mode_list, f"[ ERROR ] mode should be dpata, raw || Not {mode}"
+        if mode == "dpdata":
+            np.save(energy_path, self.energies)
+            np.save(box_path, self.cells.reshape(self._num_frame, 9))
+            np.save(virial_path, self.virials.reshape(self._num_frame, 9))
+            np.save(force_path, self.forces.reshape(self._num_frame, int(self._num_atom * 3)))
+            np.save(coord_path, self.coords.reshape(self._num_frame, int(self._num_atom * 3)))
+        elif mode == "raw":
+            np.save(energy_path, self.energies)
+            np.save(box_path, self.cells)
+            np.save(virial_path, self.virials)
+            np.save(force_path, self.forces)
+            np.save(coord_path, self.coords)
+        np.savetxt(folder + "type.raw", self.types, fmt="%d")
+        np.savetxt(folder + "type_map.raw", self._type_map, fmt="%s")
+
+    def _brew_xyzfile(self, xyz_file):
+        brewery = Brewery(path=xyz_file, fmt="xyz")
+        line_range = tqdm(
+            brewery.frange(),
+            desc=f"[ {color.font_cyan}BREW{color.reset} ]  #{color.font_green}XYZ{color.reset} ",
+            **self.tqmd_option,
+        )
+        self._coord_list = np.array([brewery.coords for _ in line_range])
+        self.is_contain_coord = True
+
+    def _brew_logfile(self, log_file):
+        # BASE for brewing
+        ## CELL
+        cell_keyword = "CELL| Vector "
+        self.is_contain_cell = False
+        self._cell_list = []
+        ## STRESS
+        stress_keyword = "STRESS| Analytical stress"
+        self.is_contain_stress = False
+        self._stress_list = []
+        ## ENERGY
+        energy_keyword = "ENERGY|"
+        self.is_contain_energy = False
+        self._energy_list = []
+        ## FORCE
+        force_keyword = " Atom   Kind "
+        self.is_contain_force = False
+        self._force_list = []
+        force_stop_keyword = "SUM OF ATOMIC FORCES"
+        force_iter_on = False
+        ## KIND
+        kind_keyword = " Atom  Kind "
+        self.is_contain_kind = False
+        self._kind_list = []
+        kind_stop_keyword = "\n"
+        kind_iter_on = False
+        # ITERATION
+        with open(log_file, "r") as f:
+            line_range = enumerate(
+                tqdm(
+                    f,
+                    **self.tqmd_option,
+                    desc=f"[ {color.font_cyan}BREW{color.reset} ]  #{color.font_green}LOG{color.reset} ",
+                )
+            )
+            for idx, line in line_range:
+                # CELL
+                if len(self._cell_list) < 3:
+                    if cell_keyword in line:
+                        self.is_contain_cell = True
+                        self._cell_list.append(line.split()[4:7])
+                        continue
+                # STRESS
+                if stress_keyword in line:
+                    self.is_contain_stress = True
+                    stress_idx = idx
+                if self.is_contain_stress and stress_idx + 5 > idx > stress_idx + 1:
+                    self._stress_list.append(line.split()[2:5])
+                    continue
+                # ENERGY
+                if energy_keyword in line:
+                    self.is_contain_energy = True
+                    self._energy_list.append(line.split()[8])
+                    continue
+                # FORCE
+                if force_keyword in line:
+                    force_idx = idx
+                    self.is_contain_force = True
+                    force_iter_on = True
+                    continue
+                if force_stop_keyword in line:
+                    force_iter_on = False
+                if force_iter_on and idx > force_idx:
+                    self._force_list.append(line.split()[3:6])
+                    continue
+                # TYPE
+                if not self.is_contain_kind:
+                    if kind_keyword in line:
+                        kind_idx = idx
+                        kind_iter_on = True
+                        continue
+                    if kind_iter_on and kind_stop_keyword == line:
+                        kind_iter_on = False
+                        self.is_contain_kind = True
+                    if kind_iter_on and idx > kind_idx:
+                        self._kind_list.append(line.split()[2])
+                        continue
+
+    @color_print(name=printing_option["2array"])
+    def _change2array(self, data_type: str = "float32"):
+        F = int(self._num_frame)
+        N = int(self._num_atom)
+        self._stress_list = np.array(self._stress_list).astype(data_type).reshape(F, 3, 3)
+        self._force_list = np.array(self._force_list).astype(data_type).reshape(F, N, 3)
+        self._cell_list = np.tile(self._cell_list, (self._num_frame, 1)).astype(data_type).reshape(F, 3, 3)
+        self._energy_list = np.array(self._energy_list).astype(data_type)
+        self._coord_list = np.array(self._coord_list).astype(data_type)
+        self._type_list = np.array(self._type_list).astype("int32")
+
+    @color_print(name=printing_option["2a.u"])
+    def _convert_unit(self, verbose: bool = True):
+        ELE_CHG = constants.elementary_charge  # Elementary Charge, in C
+        HARTREE = constants.value("atomic unit of energy")  # Hartree, in Jole
+        BOHR = constants.value("atomic unit of length")  # Bohr, in m
+
+        eV = ELE_CHG  # eV
+        hatree2eV = HARTREE / ELE_CHG  # eV
+        J2eV = 1  # eV
+
+        angstrom = 1  # angstrom
+        m2angstrom = 1e-10 * angstrom  # angstrom
+        bohr2angstrom = BOHR / m2angstrom  # angstrom
+        GPa2eVangstorm = 1e-9 * J2eV / (m2angstrom**3) * eV  # eV / angstrom^3
+
+        self._energy_list *= hatree2eV
+        self._cell_list = self._cell_list
+        self._force_list *= hatree2eV / bohr2angstrom
+        volume = np.linalg.det(self._cell_list[0])
+        self._virial_list = self._stress_list * volume / GPa2eVangstorm
+        self._coord_list = self._coord_list
+
+    @color_print(name=printing_option["kind2type"])
+    def _covert_kind2type(self):
+        self._type_dict = {kind: idx for idx, kind in enumerate(self._type_map)}
+        self._type_list = [self._type_dict[kind] for kind in self._kind_list]
```

### Comparing `MDbrew-2.2.5/MDbrew/analysis/msd.py` & `MDbrew-2.3.0/MDbrew/analysis/msd.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,130 +1,131 @@
-import numpy as np
-from tqdm import trange, tqdm
-from ..tool import spacer
-from ..main.brewery import Brewery
-from ..tool.colorfont import color
-
-
-# Class of Mean Square Displacement
-class MSD(object):
-    axis_dict = {"frame": 0, "N_particle": 1, "pos": -1}
-    kwrgs_trange = {
-        "desc": f"[ {color.font_cyan}BREW{color.reset} ]  #{color.font_green}MSD{color.reset} ",
-        "ncols": 60,
-        "ascii": True,
-    }
-    kwrgs_pos = {
-        "desc": f"[ {color.font_cyan}BREW{color.reset} ]  #{color.font_green}POS{color.reset} ",
-        "ncols": 60,
-        "ascii": True,
-    }
-
-    def __init__(self, position, fft: bool = True, dtype: str = "float32"):
-        """MSD
-
-        Calculate the msd data and return it with method and fft
-
-        Parameters
-        ------------
-        position
-            Data of Particle's position in each frame
-        fft : bool, optional
-            default = True, if True the calculation in FFT, else  matrix
-
-        ## Result of 'Mean Square Displacement'
-        >>> my_msd      = MSD(position = position, fft = True)
-        >>> msd_result  = my_msd.result
-        """
-        if type(position) == Brewery:
-            self.is_Brewery_type = True
-            self.position = position.reorder().brew(cols=["x", "y", "z"])
-            pos_range = tqdm(self.position, **self.kwrgs_pos)
-            self.position = np.array([data for data in pos_range], dtype=dtype)
-        else:
-            self.position = spacer.check_dimension(position, dim=3)
-        self.frame_number = self.position.shape[0]
-        self.fft = fft
-
-    def run(self):
-        """run
-
-        Return
-        ----------
-        NDArray[np.float64]: result of MSD
-        """
-        if self.fft:
-            self._result = self.__get_msd_fft()
-        else:
-            self._result = self.__get_msd_window()
-        return self
-
-    @property
-    def result(self):
-        return self._result
-
-    # window method with non-FFT
-    def __get_msd_window(self):
-        """MSD - Window Method with non-FFT
-
-        Calculate the MSD list with linear loop with numpy function
-
-        Time complexity : O(N**2)
-
-        Returns
-        ----------
-        NDArray[np.float64]
-            MSD data of each frame
-        """
-        msd_list = np.zeros(self.position.shape[:2])
-        for frame in trange(1, self.frame_number, **self.kwrgs_trange):
-            diff_position = spacer.get_diff_position(self.position[frame:], self.position[:-frame])
-            distance = self.__square_sum_position(diff_position)
-            msd_list[frame, :] = np.mean(distance, axis=self.axis_dict["frame"])
-        return self.__mean_msd_list(msd_list=msd_list)
-
-    # window method with FFT
-    def __get_msd_fft(self):
-        """MSD - Window method wit FFT
-
-        Calculate the MSD list with linear loop with numpy function
-
-        Time complexity : O(N logN)
-
-        Returns
-        ----------
-        NDArray[np.float64]
-            MSD data of each frame
-        """
-        S_1 = self.__get_S_1()
-        S_2 = self.__get_S_2()
-        msd_list = np.subtract(S_1, 2.0 * S_2)
-        return self.__mean_msd_list(msd_list=msd_list)
-
-    def __get_S_1(self):
-        empty_matrix = np.zeros(self.position.shape[:2])
-        D = self.__square_sum_position(self.position)
-        D = np.append(D, empty_matrix, axis=self.axis_dict["frame"])
-        Q = 2.0 * np.sum(D, axis=self.axis_dict["frame"])
-        S_1 = empty_matrix
-        for m in trange(self.frame_number, **self.kwrgs_trange):
-            Q -= D[m - 1, :] + D[self.frame_number - m, :]
-            S_1[m, :] = Q / (self.frame_number - m)
-        return S_1
-
-    # get S2 for FFT
-    def __get_S_2(self):
-        X = np.fft.fft(self.position, n=2 * self.frame_number, axis=self.axis_dict["frame"])
-        dot_X = X * X.conjugate()
-        x = np.fft.ifft(dot_X, axis=self.axis_dict["frame"])
-        x = x[: self.frame_number].real
-        x = x.sum(axis=self.axis_dict["pos"])
-        n = np.arange(self.frame_number, 0, -1)
-        return x / n[:, np.newaxis]
-
-    # do square and sum about position
-    def __square_sum_position(self, position_data):
-        return np.square(position_data).sum(axis=self.axis_dict["pos"])
-
-    # do mean about msd list
-    def __mean_msd_list(self, msd_list):
-        return msd_list.mean(axis=self.axis_dict["N_particle"])
+import numpy as np
+from tqdm import trange, tqdm
+from ..tool import spacer
+from ..main.brewery import Brewery
+from ..tool.colorfont import color
+
+
+# Class of Mean Square Displacement
+class MSD(object):
+    axis_dict = {"frame": 0, "N_particle": 1, "pos": -1}
+    kwrgs_trange = {
+        "desc": f"[ {color.font_cyan}BREW{color.reset} ]  #{color.font_green}MSD{color.reset} ",
+        "ncols": 60,
+        "ascii": True,
+    }
+    kwrgs_pos = {
+        "desc": f"[ {color.font_cyan}BREW{color.reset} ]  #{color.font_green}POS{color.reset} ",
+        "ncols": 60,
+        "ascii": True,
+    }
+
+    def __init__(self, position, fft: bool = True, dtype: str = "float32"):
+        """MSD
+
+        Calculate the msd data and return it with method and fft
+
+        Parameters
+        ------------
+        position
+            Data of Particle's position in each frame
+        fft : bool, optional
+            default = True, if True the calculation in FFT, else  matrix
+
+        ## Result of 'Mean Square Displacement'
+        >>> my_msd      = MSD(position = position, fft = True)
+        >>> msd_result  = my_msd.result
+        """
+        if type(position) == Brewery:
+            self.is_Brewery_type = True
+            pos_range = tqdm(position.frange(), **self.kwrgs_pos)
+            self.position = np.array([position.coords for _ in pos_range], dtype=dtype)
+        else:
+            self.position = spacer.check_dimension(position, dim=3)
+        self.frame_number = self.position.shape[0]
+        self._fft = fft
+
+    def run(self):
+        """run
+
+        Return
+        ----------
+        NDArray[np.float64]: result of MSD
+        """
+        if self._fft:
+            self._result = self.__get_msd_fft()
+        else:
+            self._result = self.__get_msd_window()
+        return self
+
+    @property
+    def result(self):
+        if not hasattr(self, "_result"):
+            self.run()
+        return self._result
+
+    # window method with non-FFT
+    def __get_msd_window(self):
+        """MSD - Window Method with non-FFT
+
+        Calculate the MSD list with linear loop with numpy function
+
+        Time complexity : O(N**2)
+
+        Returns
+        ----------
+        NDArray[np.float64]
+            MSD data of each frame
+        """
+        msd_list = np.zeros(self.position.shape[:2])
+        for frame in trange(1, self.frame_number, **self.kwrgs_trange):
+            diff_position = spacer.get_diff_position(self.position[frame:], self.position[:-frame])
+            distance = self.__square_sum_position(diff_position)
+            msd_list[frame, :] = np.mean(distance, axis=self.axis_dict["frame"])
+        return self.__mean_msd_list(msd_list=msd_list)
+
+    # window method with FFT
+    def __get_msd_fft(self):
+        """MSD - Window method wit FFT
+
+        Calculate the MSD list with linear loop with numpy function
+
+        Time complexity : O(N logN)
+
+        Returns
+        ----------
+        NDArray[np.float64]
+            MSD data of each frame
+        """
+        S_1 = self.__get_S_1()
+        S_2 = self.__get_S_2()
+        msd_list = np.subtract(S_1, 2.0 * S_2)
+        return self.__mean_msd_list(msd_list=msd_list)
+
+    def __get_S_1(self):
+        empty_matrix = np.zeros(self.position.shape[:2])
+        D = self.__square_sum_position(self.position)
+        D = np.append(D, empty_matrix, axis=self.axis_dict["frame"])
+        Q = 2.0 * np.sum(D, axis=self.axis_dict["frame"])
+        S_1 = empty_matrix
+        for m in trange(self.frame_number, **self.kwrgs_trange):
+            Q -= D[m - 1, :] + D[self.frame_number - m, :]
+            S_1[m, :] = Q / (self.frame_number - m)
+        return S_1
+
+    # get S2 for FFT
+    def __get_S_2(self):
+        X = np.fft.fft(self.position, n=2 * self.frame_number, axis=self.axis_dict["frame"])
+        dot_X = X * X.conjugate()
+        x = np.fft.ifft(dot_X, axis=self.axis_dict["frame"])
+        x = x[: self.frame_number].real
+        x = x.sum(axis=self.axis_dict["pos"])
+        n = np.arange(self.frame_number, 0, -1)
+        return x / n[:, np.newaxis]
+
+    # do square and sum about position
+    def __square_sum_position(self, position_data):
+        return np.square(position_data).sum(axis=self.axis_dict["pos"])
+
+    # do mean about msd list
+    def __mean_msd_list(self, msd_list):
+        return msd_list.mean(axis=self.axis_dict["N_particle"])
```

### Comparing `MDbrew-2.2.5/MDbrew/analysis/rdf.py` & `MDbrew-2.3.0/MDbrew/analysis/rdf.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,143 +1,155 @@
-import numpy as np
-from tqdm import trange, tqdm
-from ..main.brewery import Brewery
-from ..tool.spacer import *
-from ..tool.colorfont import color
-
-
-# Calculate and Plot the RDF
-class RDF(object):
-    kwrgs_trange = {
-        "desc": f"[ {color.font_cyan}BREW{color.reset} ]  #{color.font_green}RDF{color.reset} ",
-        "ncols": 60,
-        "ascii": True,
-    }
-
-    def __init__(
-        self, a, b, box_size, layer: int = 0, r_max: float = None, resolution: int = 1000, max_frame: int = None
-    ):
-        if type(a) == Brewery:
-            self.is_Brewery_type = True
-            self.a = a.reorder().brew(cols=["x", "y", "z"])
-            self.b = b.reorder().brew(cols=["x", "y", "z"])
-            self.frame_num = max_frame
-            self.a_number = a.atom_num
-            self.b_number = b.atom_num
-        else:
-            self.is_Brewery_type = False
-            self.a = check_dimension(a, dim=3)
-            self.b = check_dimension(b, dim=3)
-            self.frame_num = self.a.shape[0] if max_frame is None else max_frame
-            self.a_number = self.a.shape[1]
-            self.b_number = self.b.shape[1]
-
-        self.box_size = check_dimension(box_size, dim=1)
-        self.half_box_size = self.box_size * 0.5
-
-        self.layer_depth = layer
-        self.layer = self.__make_layer()
-
-        self.resolution = resolution
-        self.r_max = np.max(self.half_box_size) * (2.0 * self.layer_depth + 1.0) if r_max is None else r_max
-        self.dr = self.r_max / self.resolution
-
-        self.hist_data = None
-        self.radii = np.linspace(0.0, self.r_max, self.resolution)
-
-    def run(self):
-        if self.is_Brewery_type:
-            self._cal_hist_data_with_generator()
-        else:
-            self._cal_hist_data_with_iterator()
-        return self
-
-    @property
-    def result(self):
-        if self.hist_data is None:
-            self.run()
-        return self.__cal_rdf_from_hist_data()
-
-    @property
-    def cn(self):
-        if self.hist_data is None:
-            self.run()
-        return self.__cal_cn_from_hist_data()
-
-    # Function for get hist
-    def _cal_hist_data_with_iterator(self):
-        self.hist_data = np.zeros(self.resolution)
-        _apply_boundary_condition = self.__set_boundary_condition()
-        for frame in trange(self.frame_num, **self.kwrgs_trange):
-            a_unit = self.a[frame, ...]
-            b_unit = self.b[frame, ...]
-            diff_position = get_diff_position(a_unit[:, None, :], b_unit[None, :, :])
-            diff_position = _apply_boundary_condition(diff_position=diff_position)
-            distance = get_distance(diff_position=diff_position, axis=-1)
-            idx_hist = self.__cal_idx_histogram(distance=distance)
-            value, count = np.unique(idx_hist, return_counts=True)
-            self.hist_data[value] += count
-
-    # Function for get hist
-    def _cal_hist_data_with_generator(self):
-        self.hist_data = np.zeros(self.resolution)
-        _apply_boundary_condition = self.__set_boundary_condition()
-        frame_num = 0
-        for a_unit, b_unit in tqdm(zip(self.a, self.b), **self.kwrgs_trange):
-            if self.frame_num is not None and frame_num == self.frame_num:
-                break
-            frame_num += 1
-            diff_position = get_diff_position(a_unit[:, None, :], b_unit[None, :, :])
-            diff_position = _apply_boundary_condition(diff_position=diff_position)
-            distance = get_distance(diff_position=diff_position, axis=-1)
-            idx_hist = self.__cal_idx_histogram(distance=distance)
-            value, count = np.unique(idx_hist, return_counts=True)
-            self.hist_data[value] += count
-        self.frame_num = frame_num
-
-    # select the mode with Boundary Layer
-    def __set_boundary_condition(self):
-        return self.__add_layer if self.layer_depth else self.__check_pbc
-
-    # set the pbc only consider single system
-    def __check_pbc(self, diff_position):
-        diff_position = np.abs(diff_position)
-        return np.where(
-            diff_position > self.half_box_size,
-            self.box_size - diff_position,
-            diff_position,
-        )
-
-    # set the pbc with 27 system
-    def __add_layer(self, diff_position):
-        return diff_position[..., np.newaxis, :] + self.layer
-
-    # Make a 3D layer_idx
-    def __make_layer(self):
-        list_direction = []
-        idx_direction_ = range(-self.layer_depth, self.layer_depth + 1)
-        for i in idx_direction_:
-            for j in idx_direction_:
-                for k in idx_direction_:
-                    list_direction.append([i, j, k])
-        return np.array(list_direction) * self.box_size
-
-    # get idx for histogram
-    def __cal_idx_histogram(self, distance):
-        idx_hist = (distance / self.dr).astype(np.int64)
-        return idx_hist[np.where((0 < idx_hist) & (idx_hist < self.resolution))]
-
-    # Calculate the Density Function
-    def __cal_rdf_from_hist_data(self):
-        r_i = self.radii[1:]
-        g_r = np.append(0.0, self.hist_data[1:] / np.square(r_i))
-        factor = np.array(
-            4.0 * np.pi * self.dr * self.frame_num * self.a_number * self.b_number,
-            dtype=np.float64,
-        )
-        box_volume = np.prod(self.box_size, dtype=np.float64)
-        return g_r * box_volume / factor
-
-    # Function for get coordinate number
-    def __cal_cn_from_hist_data(self):
-        self.n = self.hist_data / (self.frame_num * self.a_number)
-        return np.cumsum(self.n)
+import numpy as np
+from tqdm import trange, tqdm
+from ..main.brewery import Brewery
+from ..tool.spacer import *
+from ..tool.colorfont import color
+
+
+# Calculate and Plot the RDF
+class RDF(object):
+    kwrgs_trange = {
+        "desc": f"[ {color.font_cyan}BREW{color.reset} ]  #{color.font_green}RDF{color.reset} ",
+        "ncols": 60,
+        "ascii": True,
+    }
+
+    def __init__(
+        self,
+        a,
+        b,
+        box_size=None,
+        layer: int = 0,
+        r_max: float = None,
+        resolution: int = 1000,
+        max_frame: int = None,
+        dtype: str = "float32",
+    ):
+        if type(a) == Brewery:
+            self.is_Brewery_type = True
+            self.a = a
+            self.b = b
+            self.frame_num = max_frame
+            self.a_number = a.atom_num
+            self.b_number = b.atom_num
+            self.box_size = a.box_size if box_size is None else box_size
+            assert len(self.box_size), "plz set box_size"
+        else:
+            self.is_Brewery_type = False
+            self.a = check_dimension(a, dim=3)
+            self.b = check_dimension(b, dim=3)
+            self.frame_num = self.a.shape[0] if max_frame is None else max_frame
+            self.a_number = self.a.shape[1]
+            self.b_number = self.b.shape[1]
+
+        self.box_size = np.array(self.box_size, dtype=dtype)
+        self.half_box_size = self.box_size * 0.5
+
+        self.layer_depth = layer
+        self.layer = self.__make_layer()
+
+        self.resolution = resolution
+        self.r_max = np.max(self.half_box_size) * (2.0 * self.layer_depth + 1.0) if r_max is None else r_max
+        self.dr = self.r_max / self.resolution
+
+        self.hist_data = None
+        self.radii = np.linspace(0.0, self.r_max, self.resolution)
+
+    def run(self):
+        if self.is_Brewery_type:
+            self._cal_hist_data_with_generator()
+        else:
+            self._cal_hist_data_with_iterator()
+        return self
+
+    @property
+    def result(self):
+        if self.hist_data is None:
+            self.run()
+        return self.__cal_rdf_from_hist_data()
+
+    @property
+    def cn(self):
+        if self.hist_data is None:
+            self.run()
+        return self.__cal_cn_from_hist_data()
+
+    # Function for get hist
+    def _cal_hist_data_with_iterator(self):
+        self.hist_data = np.zeros(self.resolution)
+        _apply_boundary_condition = self.__set_boundary_condition()
+        for frame in trange(self.frame_num, **self.kwrgs_trange):
+            a_unit = self.a[frame, ...]
+            b_unit = self.b[frame, ...]
+            diff_position = get_diff_position(a_unit[:, None, :], b_unit[None, :, :])
+            diff_position = _apply_boundary_condition(diff_position=diff_position)
+            distance = get_distance(diff_position=diff_position, axis=-1)
+            idx_hist = self.__cal_idx_histogram(distance=distance)
+            value, count = np.unique(idx_hist, return_counts=True)
+            self.hist_data[value] += count
+
+    # Function for get hist
+    def _cal_hist_data_with_generator(self):
+        self.hist_data = np.zeros(self.resolution)
+        _apply_boundary_condition = self.__set_boundary_condition()
+        frame_num = 0
+        for _ in tqdm(zip(self.a.frange(), self.b.frange()), **self.kwrgs_trange):
+            if self.frame_num is not None and frame_num == self.frame_num:
+                break
+            frame_num += 1
+            a_unit = self.a.coords
+            b_unit = self.b.coords
+            diff_position = get_diff_position(a_unit[:, None, :], b_unit[None, :, :])
+            diff_position = _apply_boundary_condition(diff_position=diff_position)
+            distance = get_distance(diff_position=diff_position, axis=-1)
+            idx_hist = self.__cal_idx_histogram(distance=distance)
+            value, count = np.unique(idx_hist, return_counts=True)
+            self.hist_data[value] += count
+        self.frame_num = frame_num
+
+    # select the mode with Boundary Layer
+    def __set_boundary_condition(self):
+        return self.__add_layer if self.layer_depth else self.__check_pbc
+
+    # set the pbc only consider single system
+    def __check_pbc(self, diff_position):
+        diff_position = np.abs(diff_position)
+        return np.where(
+            diff_position > self.half_box_size,
+            self.box_size - diff_position,
+            diff_position,
+        )
+
+    # set the pbc with 27 system
+    def __add_layer(self, diff_position):
+        return diff_position[..., np.newaxis, :] + self.layer
+
+    # Make a 3D layer_idx
+    def __make_layer(self):
+        list_direction = []
+        idx_direction_ = range(-self.layer_depth, self.layer_depth + 1)
+        for i in idx_direction_:
+            for j in idx_direction_:
+                for k in idx_direction_:
+                    list_direction.append([i, j, k])
+        return np.array(list_direction) * self.box_size
+
+    # get idx for histogram
+    def __cal_idx_histogram(self, distance):
+        idx_hist = (distance / self.dr).astype(np.int64)
+        return idx_hist[np.where((0 < idx_hist) & (idx_hist < self.resolution))]
+
+    # Calculate the Density Function
+    def __cal_rdf_from_hist_data(self):
+        r_i = self.radii[1:]
+        g_r = np.append(0.0, self.hist_data[1:] / np.square(r_i))
+        factor = np.array(
+            4.0 * np.pi * self.dr * self.frame_num * self.a_number * self.b_number,
+            dtype=np.float64,
+        )
+        box_volume = np.prod(self.box_size, dtype=np.float64)
+        return g_r * box_volume / factor
+
+    # Function for get coordinate number
+    def __cal_cn_from_hist_data(self):
+        self.n = self.hist_data / (self.frame_num * self.a_number)
+        return np.cumsum(self.n)
```

### Comparing `MDbrew-2.2.5/MDbrew/main/filetype/vasp.py` & `MDbrew-2.3.0/MDbrew/main/filetype/vasp.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,36 +1,37 @@
-from ..opener import Opener
-
-
-class vaspOpener(Opener):
-    def __init__(self, path: str, is_generator: str = False) -> None:
-        super().__init__(path, is_generator)
-        self.skip_head = 7
-        self.column = ["atom", "x", "y", "z"]
-        self._set_box_and_atom(path=path)
-
-    def _make_one_frame_data(self, file, first_loop_line):
-        step = first_loop_line.split()[-1]
-        num_atom = sum(self.atom_kind_num)
-        database = []
-        c_atom_num = 0
-        pointer = 0
-        for _ in range(num_atom):
-            if c_atom_num >= self.atom_kind_num[pointer]:
-                pointer += 1
-                c_atom_num = 0
-            c_atom_num += 1
-            line = [self.atom_kind[pointer]]
-            line.extend(file.readline().split())
-            database.append(line)
-        return database
-
-    def _set_box_and_atom(self, path):
-        with open(path, "r") as raw_file:
-            for i in range(2):
-                raw_file.readline()
-            for i in range(3):
-                line = raw_file.readline().split()
-                box_size = float(line[i])
-                self.box_size.append(box_size)
-            self.atom_kind = raw_file.readline().split()
-            self.atom_kind_num = [int(data) for data in raw_file.readline().split()]
+from ..opener import Opener
+
+
+class vaspOpener(Opener):
+    def __init__(self, path: str) -> None:
+        super().__init__(path)
+        self.skip_head = 7
+        self.column = ["atom", "x", "y", "z"]
+        self._set_box_and_atom(path=path)
+        self.gen_db()
+
+    def _make_one_frame_data(self, file, first_loop_line):
+        step = first_loop_line.split()[-1]
+        num_atom = sum(self.atom_kind_num)
+        database = []
+        c_atom_num = 0
+        pointer = 0
+        for _ in range(num_atom):
+            if c_atom_num >= self.atom_kind_num[pointer]:
+                pointer += 1
+                c_atom_num = 0
+            c_atom_num += 1
+            line = [self.atom_kind[pointer]]
+            line.extend(file.readline().split())
+            database.append(line)
+        return database
+
+    def _set_box_and_atom(self, path):
+        with open(path, "r") as raw_file:
+            for i in range(2):
+                raw_file.readline()
+            for i in range(3):
+                line = raw_file.readline().split()
+                box_size = float(line[i])
+                self.box_size.append(box_size)
+            self.atom_kind = raw_file.readline().split()
+            self.atom_kind_num = [int(data) for data in raw_file.readline().split()]
```

### Comparing `MDbrew-2.2.5/MDbrew/main/filetype/lmps.py` & `MDbrew-2.3.0/MDbrew/main/filetype/lmps.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,22 +1,23 @@
-from ..opener import Opener
-
-
-class lmpsOpener(Opener):
-    def __init__(self, path: str, is_generator: str = False) -> None:
-        super().__init__(path, is_generator)
-        self._atom_keyword = "type"
-
-    def _make_one_frame_data(self, file, first_loop_line):
-        self.skip_line(file=file, num=2)
-        atom_num = int(file.readline().split()[0])
-        self.skip_line(file=file, num=1)
-        self.box_size = [sum([abs(float(box_length)) for box_length in file.readline().split()]) for _ in range(3)]
-        self.column = file.readline().split()[2:]
-        return [self.str2float_list(file.readline().split()) for _ in range(atom_num)]
-
-    def skip_line(self, file, num):
-        for _ in range(num):
-            file.readline()
-
-    def str2float_list(self, str_list):
-        return [float(data) for data in str_list]
+from ..opener import Opener
+
+
+class lmpsOpener(Opener):
+    def __init__(self, path: str) -> None:
+        super().__init__(path)
+        self._atom_keyword = "type"
+        self.gen_db()
+
+    def _make_one_frame_data(self, file, first_loop_line):
+        self.skip_line(file=file, num=2)
+        atom_num = int(file.readline().split()[0])
+        self.skip_line(file=file, num=1)
+        self.box_size = [sum([abs(float(box_length)) for box_length in file.readline().split()]) for _ in range(3)]
+        self.column = file.readline().split()[2:]
+        return [self.str2float_list(file.readline().split()) for _ in range(atom_num)]
+
+    def skip_line(self, file, num):
+        for _ in range(num):
+            file.readline()
+
+    def str2float_list(self, str_list):
+        return [float(data) for data in str_list]
```

