# Comparing `tmp/arglite-0.5.0-py3-none-any.whl.zip` & `tmp/arglite-0.6.0-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,11 +1,11 @@
-Zip file size: 5552 bytes, number of entries: 9
+Zip file size: 5643 bytes, number of entries: 9
 -rw-r--r--  2.0 unx       43 b- defN 22-Dec-26 21:37 arglite/__init__.py
--rw-r--r--  2.0 unx     4933 b- defN 23-Jan-21 21:11 arglite/arglite.py
+-rw-r--r--  2.0 unx     5198 b- defN 23-May-05 18:59 arglite/arglite.py
 -rw-r--r--  2.0 unx      824 b- defN 22-Dec-26 21:37 arglite/argument.py
 -rw-r--r--  2.0 unx     1037 b- defN 23-Jan-22 15:26 arglite/code.py
--rw-r--r--  2.0 unx     1211 b- defN 23-Jan-22 15:27 arglite-0.5.0.dist-info/LICENSE
--rw-r--r--  2.0 unx      795 b- defN 23-Jan-22 15:27 arglite-0.5.0.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-Jan-22 15:27 arglite-0.5.0.dist-info/WHEEL
--rw-r--r--  2.0 unx        8 b- defN 23-Jan-22 15:27 arglite-0.5.0.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      680 b- defN 23-Jan-22 15:27 arglite-0.5.0.dist-info/RECORD
-9 files, 9623 bytes uncompressed, 4386 bytes compressed:  54.4%
+-rw-r--r--  2.0 unx     1211 b- defN 23-May-05 19:32 arglite-0.6.0.dist-info/LICENSE
+-rw-r--r--  2.0 unx      795 b- defN 23-May-05 19:32 arglite-0.6.0.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-May-05 19:32 arglite-0.6.0.dist-info/WHEEL
+-rw-r--r--  2.0 unx        8 b- defN 23-May-05 19:32 arglite-0.6.0.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      680 b- defN 23-May-05 19:32 arglite-0.6.0.dist-info/RECORD
+9 files, 9888 bytes uncompressed, 4477 bytes compressed:  54.7%
```

## zipnote {}

```diff
@@ -6,23 +6,23 @@
 
 Filename: arglite/argument.py
 Comment: 
 
 Filename: arglite/code.py
 Comment: 
 
-Filename: arglite-0.5.0.dist-info/LICENSE
+Filename: arglite-0.6.0.dist-info/LICENSE
 Comment: 
 
-Filename: arglite-0.5.0.dist-info/METADATA
+Filename: arglite-0.6.0.dist-info/METADATA
 Comment: 
 
-Filename: arglite-0.5.0.dist-info/WHEEL
+Filename: arglite-0.6.0.dist-info/WHEEL
 Comment: 
 
-Filename: arglite-0.5.0.dist-info/top_level.txt
+Filename: arglite-0.6.0.dist-info/top_level.txt
 Comment: 
 
-Filename: arglite-0.5.0.dist-info/RECORD
+Filename: arglite-0.6.0.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## arglite/arglite.py

```diff
@@ -18,15 +18,16 @@
 from .argument import Optional
 from .argument import RequirementError
 
 class Parser:
 
   def __init__(self):
     """ Entry point. """
-    self.file = sys.argv[0]
+    #self.file = sys.argv[0]
+    self.file = self.caller()
     self.h, self.help = None, None
     arg_str = self.flatten(sys.argv[1:])
     self.args = self.pairs(arg_str)
     self.required = Required()
     self.optional = Optional()
     self.set_vars()
     self.get_errors()
@@ -62,14 +63,21 @@
 Usage
 
 - Provide arbitary flags to a program at runtime
 - Interpret flags with the argparse.parser object
     """
     return md
 
+  def caller(self) -> str:
+    stack = inspect.stack()
+    for frame in stack:
+      if frame.function == "<module>":
+        if os.path.dirname(frame.filename) != os.path.dirname(__file__):
+            return frame.filename
+
   def flatten(self, args: list = []) -> str:
     """ Flatten a list into a str """
     return " ".join(args)
 
   def pairs(self, args: str = "") -> list:
     """ Get each pair of args and values, blanks if no value """
     return re.findall(r"-{1,2}([^-][a-z]*(?:\s)?)([^-]*)", args)
@@ -110,18 +118,18 @@
 
   def reflect(self) -> dict:
     """ Gather information about expected, required, and optional variables """
     self.expected = {
       "h": False,
       "help": False
     }
-    file = os.path.abspath(
-      sys.argv[0]
-    )
-    code = Code(file)
+    #file = os.path.abspath(
+    #  sys.argv[0]
+    #)
+    code = Code(self.file)
     exp = f"{code.name}(\.parser)?(\.[a-z0-9_]+)?\.([a-z0-9_]+)"
     regexp = re.compile(exp, re.I)
     for line in code.source:
       while True:
         expected_vars = re.search(regexp, line)
         if not expected_vars: break
         if expected_vars:
```

## Comparing `arglite-0.5.0.dist-info/LICENSE` & `arglite-0.6.0.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `arglite-0.5.0.dist-info/METADATA` & `arglite-0.6.0.dist-info/METADATA`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: arglite
-Version: 0.5.0
+Version: 0.6.0
 Summary: A lightweight, dynamic arg parser for fun, but not profit.
 Home-page: https://github.com/dluman/arglite
 License: UNKNOWN
 Platform: UNKNOWN
 Description-Content-Type: text/x-rst
 Requires-Dist: rich
```

## Comparing `arglite-0.5.0.dist-info/RECORD` & `arglite-0.6.0.dist-info/RECORD`

 * *Files 26% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 arglite/__init__.py,sha256=qYy3XGLguBP5P03kIROVRrkp83p54SyB6mFd-3hMvpE,43
-arglite/arglite.py,sha256=Rej03nkVXXPH6G-ElQ9_i1YGbCb0IY-7DjmnSG5nmSk,4933
+arglite/arglite.py,sha256=pF-dAxHTFL7NrarVR5wrXP4cvhm0HDD5A59_V2f1DB8,5198
 arglite/argument.py,sha256=-tGlU-8eD21NWBOlgfYI4VmFOXXbDT_kbq6D7zXXkTQ,824
 arglite/code.py,sha256=3zYimm_Q4fRIcILrgTfT9gOWAu82pQdFQKO4mWE03kU,1037
-arglite-0.5.0.dist-info/LICENSE,sha256=fhLl30uuEsshWBuhV87SDhmGoFCN0Q0Oikq5pM-U6Fw,1211
-arglite-0.5.0.dist-info/METADATA,sha256=pqc4Lp_JZnWfCD9VY3UKFbIB1xm1_VKwX8Sl2aHt1PU,795
-arglite-0.5.0.dist-info/WHEEL,sha256=g4nMs7d-Xl9-xC9XovUrsDHGXt-FT0E17Yqo92DEfvY,92
-arglite-0.5.0.dist-info/top_level.txt,sha256=arzqHSIoCtyjfK5QmzSD--Cxr2BO3A2zFy50JEko6iA,8
-arglite-0.5.0.dist-info/RECORD,,
+arglite-0.6.0.dist-info/LICENSE,sha256=fhLl30uuEsshWBuhV87SDhmGoFCN0Q0Oikq5pM-U6Fw,1211
+arglite-0.6.0.dist-info/METADATA,sha256=tzg_OHuKzIWaIkiylSnB46J3XCMeq7oBFdihP_rKRy4,795
+arglite-0.6.0.dist-info/WHEEL,sha256=g4nMs7d-Xl9-xC9XovUrsDHGXt-FT0E17Yqo92DEfvY,92
+arglite-0.6.0.dist-info/top_level.txt,sha256=arzqHSIoCtyjfK5QmzSD--Cxr2BO3A2zFy50JEko6iA,8
+arglite-0.6.0.dist-info/RECORD,,
```

