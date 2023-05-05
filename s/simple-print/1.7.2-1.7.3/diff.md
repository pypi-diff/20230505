# Comparing `tmp/simple_print-1.7.2-py3-none-any.whl.zip` & `tmp/simple_print-1.7.3-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,13 +1,13 @@
-Zip file size: 7742 bytes, number of entries: 11
+Zip file size: 7737 bytes, number of entries: 11
 -rw-rw-r--  2.0 unx       51 b- defN 23-Apr-28 06:49 simple_print/__init__.py
 -rw-rw-r--  2.0 unx     4467 b- defN 22-Dec-04 17:59 simple_print/broker.py
--rw-rw-r--  2.0 unx     4392 b- defN 23-May-02 07:17 simple_print/sprint.py
+-rw-rw-r--  2.0 unx     4390 b- defN 23-May-05 05:01 simple_print/sprint.py
 -rw-rw-r--  2.0 unx        0 b- defN 22-Nov-21 11:16 test/__init__.py
 -rw-rw-r--  2.0 unx      220 b- defN 22-Dec-04 18:00 test/test_broker.py
 -rw-rw-r--  2.0 unx     1861 b- defN 23-Feb-27 07:48 test/test_print.py
--rwxr-xr-x  2.0 unx     1094 b- defN 23-May-02 07:18 simple_print-1.7.2.dist-info/LICENSE
--rw-rw-r--  2.0 unx     2605 b- defN 23-May-02 07:18 simple_print-1.7.2.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 23-May-02 07:18 simple_print-1.7.2.dist-info/WHEEL
--rwxr-xr-x  2.0 unx       18 b- defN 23-May-02 07:18 simple_print-1.7.2.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      868 b- defN 23-May-02 07:18 simple_print-1.7.2.dist-info/RECORD
-11 files, 15668 bytes uncompressed, 6274 bytes compressed:  60.0%
+-rwxr-xr-x  2.0 unx     1094 b- defN 23-May-05 05:02 simple_print-1.7.3.dist-info/LICENSE
+-rw-rw-r--  2.0 unx     2605 b- defN 23-May-05 05:02 simple_print-1.7.3.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 23-May-05 05:02 simple_print-1.7.3.dist-info/WHEEL
+-rwxr-xr-x  2.0 unx       18 b- defN 23-May-05 05:02 simple_print-1.7.3.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      868 b- defN 23-May-05 05:02 simple_print-1.7.3.dist-info/RECORD
+11 files, 15666 bytes uncompressed, 6269 bytes compressed:  60.0%
```

## zipnote {}

```diff
@@ -12,23 +12,23 @@
 
 Filename: test/test_broker.py
 Comment: 
 
 Filename: test/test_print.py
 Comment: 
 
-Filename: simple_print-1.7.2.dist-info/LICENSE
+Filename: simple_print-1.7.3.dist-info/LICENSE
 Comment: 
 
-Filename: simple_print-1.7.2.dist-info/METADATA
+Filename: simple_print-1.7.3.dist-info/METADATA
 Comment: 
 
-Filename: simple_print-1.7.2.dist-info/WHEEL
+Filename: simple_print-1.7.3.dist-info/WHEEL
 Comment: 
 
-Filename: simple_print-1.7.2.dist-info/top_level.txt
+Filename: simple_print-1.7.3.dist-info/top_level.txt
 Comment: 
 
-Filename: simple_print-1.7.2.dist-info/RECORD
+Filename: simple_print-1.7.3.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## simple_print/sprint.py

```diff
@@ -34,15 +34,15 @@
     
     if p:       
         cprint(f"{arg_name} | type {type(arg)} | line {lineno} | func {function_name} | file {filename}", color=c, on_color=b, attrs=[a] if a else [])
     else:
         cprint(f"{arg_name} | type {type(arg)} | line {lineno} | func {function_name}", color=c, on_color=b, attrs=[a] if a else [])
 
 
-def sprint(*args, c:Union[None, str]="white", b:Union[None, str]=None, a:Union[None, str]="bold", i:int=0, p:bool=SIMPLE_PRINT_SHOW_PATH_TO_FILE, s:bool=False, f:bool=False, **kwargs) -> Union[None, str]:
+def sprint(*args, c:Union[None, str]="white", b:Union[None, str]=None, a:Union[None, str]=None, i:int=0, p:bool=SIMPLE_PRINT_SHOW_PATH_TO_FILE, s:bool=False, f:bool=False, **kwargs) -> Union[None, str]:
     """     
     с:str ~ colors: ["grey", "red", "green", "yellow", "blue", "magenta", "cyan", "white"]  
     b:str ~ backgrounds: ["on_grey", "on_red", "on_green", "on_yellow", "on_blue", "on_magenta", "on_cyan"]  
     a:str ~ attributes: bold, dark, underline, blink, reverse, concealed   
     i:int ~ indent: 1-40  
     p:bool ~ path: show path to file       
     s:bool ~ string: return as string
```

## Comparing `simple_print-1.7.2.dist-info/LICENSE` & `simple_print-1.7.3.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `simple_print-1.7.2.dist-info/METADATA` & `simple_print-1.7.3.dist-info/METADATA`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: simple-print
-Version: 1.7.2
+Version: 1.7.3
 Summary: Powerful debugging tool for Python.
 Home-page: https://github.com/Sobolev5/simple-print/
 Author: Sobolev Andrey
 Author-email: email.asobolev@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

## Comparing `simple_print-1.7.2.dist-info/RECORD` & `simple_print-1.7.3.dist-info/RECORD`

 * *Files 6% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 simple_print/__init__.py,sha256=5PxZbGPVCHHFBkxb0qDKf-r13G5KKjlFbqNWXDnvWGA,51
 simple_print/broker.py,sha256=p1DDR4UjHBxH0BXqnw_O2dTes-H8rpV8UwzvvVKEh90,4467
-simple_print/sprint.py,sha256=TyPwIC0xskDGFmpzBxvUJEwqqcNWPudNeleO-fUyhLs,4392
+simple_print/sprint.py,sha256=dpVIoBFsQ6tlP8YF0yafkehxwQ-x9xhyNjaGXrBFDzE,4390
 test/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
 test/test_broker.py,sha256=hdDXeNHlO9s2vd_pLlHdqypWgCMQIPa3mz9Ou9Md22c,220
 test/test_print.py,sha256=agnkk5AL5xtnG-4odW0Hr1ahM5iw-Ycv1I9DIwddJ_Y,1861
-simple_print-1.7.2.dist-info/LICENSE,sha256=D2EVTI_UztUmQIzfsNpaXSuKgHLnBVY9Y56G77ZBFv0,1094
-simple_print-1.7.2.dist-info/METADATA,sha256=rM_YcYoG43adVNBtiD4brcDTdBy8Iv8wcNb1qty4lvM,2605
-simple_print-1.7.2.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
-simple_print-1.7.2.dist-info/top_level.txt,sha256=Yhv0h31B2Z5Nu3_Zy3Y27TOagXhPb2VGQBI9Q6CxV3Q,18
-simple_print-1.7.2.dist-info/RECORD,,
+simple_print-1.7.3.dist-info/LICENSE,sha256=D2EVTI_UztUmQIzfsNpaXSuKgHLnBVY9Y56G77ZBFv0,1094
+simple_print-1.7.3.dist-info/METADATA,sha256=a1u9gi0RAzd7M4UXB4AYFVCK86qTNDWOs-OdRg-kInI,2605
+simple_print-1.7.3.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
+simple_print-1.7.3.dist-info/top_level.txt,sha256=Yhv0h31B2Z5Nu3_Zy3Y27TOagXhPb2VGQBI9Q6CxV3Q,18
+simple_print-1.7.3.dist-info/RECORD,,
```

