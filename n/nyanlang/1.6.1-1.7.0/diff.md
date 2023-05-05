# Comparing `tmp/nyanlang-1.6.1.tar.gz` & `tmp/nyanlang-1.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nyanlang-1.6.1.tar", max compression
+gzip compressed data, was "nyanlang-1.7.0.tar", max compression
```

## Comparing `nyanlang-1.6.1.tar` & `nyanlang-1.7.0.tar`

### file list

```diff
@@ -1,7 +1,8 @@
--rw-r--r--   0        0        0    11342 2023-03-30 11:49:13.955098 nyanlang-1.6.1/LICENSE
--rw-r--r--   0        0        0      529 2023-04-01 06:11:32.522384 nyanlang-1.6.1/README.md
--rw-r--r--   0        0        0     1105 2023-04-12 08:44:48.257994 nyanlang-1.6.1/nyanlang/__init__.py
--rw-r--r--   0        0        0     1216 2023-03-29 08:52:28.005299 nyanlang-1.6.1/nyanlang/helper.py
--rw-r--r--   0        0        0    12610 2023-04-12 09:45:06.941720 nyanlang-1.6.1/nyanlang/nyan.py
--rw-r--r--   0        0        0      338 2023-04-12 09:25:58.503787 nyanlang-1.6.1/pyproject.toml
--rw-r--r--   0        0        0      892 1970-01-01 00:00:00.000000 nyanlang-1.6.1/PKG-INFO
+-rw-r--r--   0        0        0    11342 2023-05-04 03:55:54.976224 nyanlang-1.7.0/LICENSE
+-rw-r--r--   0        0        0      529 2023-05-04 03:55:54.976224 nyanlang-1.7.0/README.md
+-rw-r--r--   0        0        0     1827 2023-05-04 07:50:22.536319 nyanlang-1.7.0/nyanlang/__init__.py
+-rw-r--r--   0        0        0     1228 2023-05-04 13:35:13.126563 nyanlang-1.7.0/nyanlang/helper.py
+-rw-r--r--   0        0        0    22336 2023-05-05 11:54:18.803242 nyanlang-1.7.0/nyanlang/nyan.py
+-rw-r--r--   0        0        0    15218 2023-05-05 11:27:28.853301 nyanlang-1.7.0/nyanlang/nyan.pyi
+-rw-r--r--   0        0        0      338 2023-05-04 07:42:19.842982 nyanlang-1.7.0/pyproject.toml
+-rw-r--r--   0        0        0      892 1970-01-01 00:00:00.000000 nyanlang-1.7.0/PKG-INFO
```

### Comparing `nyanlang-1.6.1/LICENSE` & `nyanlang-1.7.0/LICENSE`

 * *Files identical despite different names*

### Comparing `nyanlang-1.6.1/README.md` & `nyanlang-1.7.0/README.md`

 * *Files identical despite different names*

### Comparing `nyanlang-1.6.1/nyanlang/__init__.py` & `nyanlang-1.7.0/nyanlang/__init__.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,14 +1,13 @@
-from .nyan import NyanInterpreter, NyanEngine
+from .nyan import NyanInterpreter, NyanEngine, NyanBuilder
 
 from .helper import Param, ParamItem
 from .helper import Helper
 
 import sys
-import pathlib
 
 
 def return_(v, e=1):
     print(v)
     exit(e)
 
 
@@ -23,14 +22,19 @@
             ParamItem("run", "Run a file"),
         )
     ),
     "run": helpgen.help(
         "run",
         Param("filename", "", no_desc=True),
         Param("debug", "", no_desc=True, optional=True, kw="d")
+    ),
+    "build": helpgen.help(
+        "build",
+        Param("filename", "", no_desc=True),
+        Param("out", "", no_desc=True, optional=True, kw="o")
     )
 }
 
 
 def main():
     match sys.argv:
         case [_]:
@@ -38,14 +42,26 @@
         case [_, "run"]:
             return_(HELP["run"])
         case [_, "run", f, *options]:
             debug = False
             if "-d" in options or "--debug" in options:
                 debug = True
             NyanEngine(f, debug=debug).run()
+        case [_, "build"]:
+            return_(HELP["build"])
+        case [_, "build", f, *options]:
+            out = None
+            if "-o" in options:
+                if len(options) == options.index("-o")+1:
+                    raise IndexError("'-o' parameter value not specified.")
+                out = options[options.index("-o")+1]
+            elif "--out" in options:
+                if len(options) == options.index("--out")+1:
+                    raise IndexError("'--out' parameter value not specified.")
+            NyanBuilder(f).build(output=out)
         case cmd:
             try:
                 __import__("nyan_ext_"+cmd[1]).run()
             except ModuleNotFoundError:
                 return_(f"Invalid command \"{sys.argv[1]}\"")
```

### Comparing `nyanlang-1.6.1/nyanlang/helper.py` & `nyanlang-1.7.0/nyanlang/helper.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,19 +6,19 @@
 
 class Param:
     def __init__(
             self, command_name: str, description_name: str,
             *items: ParamItem,
             no_desc: bool = False,
             optional: bool = False,
-            kw: str = None
+            kw: str | None = None
     ):
         self.command_name = f"[{command_name}?]" if optional else f"<{command_name}>"
         self.description_name = description_name
-        self.items: tuple[ParamItem] = items
+        self.items: tuple[ParamItem, ...] = items
         self.no = no_desc
         if kw:
             self.command_name = self.command_name[:1] + f"-{kw} | --{self.command_name[1:]}"
 
 
 class Helper:
     def __init__(self, file):
```

### Comparing `nyanlang-1.6.1/PKG-INFO` & `nyanlang-1.7.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nyanlang
-Version: 1.6.1
+Version: 1.7.0
 Summary: A Cutest Programming Language
 Author: sserve-kr
 Author-email: personal@sserve.me
 Requires-Python: >=3.10,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: nyanlang Version: 1.6.1 Summary: A Cutest
+Metadata-Version: 2.1 Name: nyanlang Version: 1.7.0 Summary: A Cutest
 Programming Language Author: sserve-kr Author-email: personal@sserve.me
 Requires-Python: >=3.10,<4.0 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10 Classifier: Programming
 Language :: Python :: 3.11 Description-Content-Type: text/markdown
  [https://user-images.githubusercontent.com/61446372/228822639-f126e6a3-5bcb-
                           4e04-80ed-1cb6325314bf.png]
                              ****** ë¥ë­ ******
```

