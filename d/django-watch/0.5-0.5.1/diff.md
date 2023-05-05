# Comparing `tmp/django_watch-0.5-py3-none-any.whl.zip` & `tmp/django_watch-0.5.1-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 3954 bytes, number of entries: 7
+Zip file size: 3976 bytes, number of entries: 7
 -rwxr-xr-x  2.0 unx        0 b- defN 20-Jan-27 13:04 django_watch/__init__.py
--rw-rw-r--  2.0 unx     3121 b- defN 23-May-05 04:56 django_watch/middleware.py
--rwxr-xr-x  2.0 unx     1094 b- defN 23-May-05 05:00 django_watch-0.5.dist-info/LICENSE
--rw-rw-r--  2.0 unx     1898 b- defN 23-May-05 05:00 django_watch-0.5.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 23-May-05 05:00 django_watch-0.5.dist-info/WHEEL
--rwxr-xr-x  2.0 unx       13 b- defN 23-May-05 05:00 django_watch-0.5.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      562 b- defN 23-May-05 05:00 django_watch-0.5.dist-info/RECORD
-7 files, 6780 bytes uncompressed, 2952 bytes compressed:  56.5%
+-rw-rw-r--  2.0 unx     3154 b- defN 23-May-05 05:20 django_watch/middleware.py
+-rwxr-xr-x  2.0 unx     1094 b- defN 23-May-05 05:21 django_watch-0.5.1.dist-info/LICENSE
+-rw-rw-r--  2.0 unx     1900 b- defN 23-May-05 05:21 django_watch-0.5.1.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 23-May-05 05:21 django_watch-0.5.1.dist-info/WHEEL
+-rwxr-xr-x  2.0 unx       13 b- defN 23-May-05 05:21 django_watch-0.5.1.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      572 b- defN 23-May-05 05:21 django_watch-0.5.1.dist-info/RECORD
+7 files, 6825 bytes uncompressed, 2954 bytes compressed:  56.7%
```

## zipnote {}

```diff
@@ -1,22 +1,22 @@
 Filename: django_watch/__init__.py
 Comment: 
 
 Filename: django_watch/middleware.py
 Comment: 
 
-Filename: django_watch-0.5.dist-info/LICENSE
+Filename: django_watch-0.5.1.dist-info/LICENSE
 Comment: 
 
-Filename: django_watch-0.5.dist-info/METADATA
+Filename: django_watch-0.5.1.dist-info/METADATA
 Comment: 
 
-Filename: django_watch-0.5.dist-info/WHEEL
+Filename: django_watch-0.5.1.dist-info/WHEEL
 Comment: 
 
-Filename: django_watch-0.5.dist-info/top_level.txt
+Filename: django_watch-0.5.1.dist-info/top_level.txt
 Comment: 
 
-Filename: django_watch-0.5.dist-info/RECORD
+Filename: django_watch-0.5.1.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## django_watch/middleware.py

```diff
@@ -37,19 +37,18 @@
         self.CROSSED = "\033[9m"
         self.END = "\033[0m"
 
     def __call__(self, request):
         response = None
         time_start = time.monotonic()    
         response = self.get_response(request)
-
         if hasattr(response, "status_code") and hasattr(request, "process_stdout_end") and request.process_stdout_end:
             process_stdout_end = request.process_stdout_end            
             process_stdout_end += f"{self.YELLOW} • STATUS {response.status_code} • Total time • {round((time.monotonic() - time_start), 2)}s{self.END}"        
-   
+            print(process_stdout_end)
         return response
 
     def process_view(self, request, func, args, kwargs):                 
         func = unwrap(func)   
         if hasattr(func, "__code__"):
             process_stdout_start = f"\n| {self.GREEN}START {request.method} {func.__code__.co_filename} {self.END}| • {self.GREEN}{self.BOLD}{func.__name__}{self.END}{self.END} {self.GREEN}•{self.END} {self.GREEN}Line number {func.__code__.co_firstlineno}{self.END}"
             request.process_stdout_end = f"\n| {self.YELLOW}{self.BOLD}END {request.method} {func.__code__.co_filename} {self.END}| • {self.YELLOW}{self.BOLD}{func.__name__}{self.END}{self.END}"
```

## Comparing `django_watch-0.5.dist-info/LICENSE` & `django_watch-0.5.1.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `django_watch-0.5.dist-info/METADATA` & `django_watch-0.5.1.dist-info/METADATA`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-watch
-Version: 0.5
+Version: 0.5.1
 Summary: Simple and useful django middleware for real-time logging.
 Home-page: https://github.com/Sobolev5/django-watch/
 Author: Sobolev Andrey
 Author-email: email.asobolev@gmail.com
 License: UNKNOWN
 Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
```

## Comparing `django_watch-0.5.dist-info/RECORD` & `django_watch-0.5.1.dist-info/RECORD`

 * *Files 14% similar despite different names*

```diff
@@ -1,7 +1,7 @@
 django_watch/__init__.py,sha256=47DEQpj8HBSa-_TImW-5JCeuQeRkm5NMpJWZG3hSuFU,0
-django_watch/middleware.py,sha256=r0ih4X4oCtNzh98gDo6e1JdumehQGp1I3PNUmnOq68U,3121
-django_watch-0.5.dist-info/LICENSE,sha256=BvmWh0aXPp8jrD0GS25NwyJ321UbcQ7KIui9wAmwVD0,1094
-django_watch-0.5.dist-info/METADATA,sha256=FE8YvJuq_cBSR-i2EDKu__ZiOvMst8ENEJ9GXJfo0-k,1898
-django_watch-0.5.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
-django_watch-0.5.dist-info/top_level.txt,sha256=Q6Y_7H4paLM2YTKdPpC2LHZ4a2zUoWHBxkv9GmX9SOg,13
-django_watch-0.5.dist-info/RECORD,,
+django_watch/middleware.py,sha256=94qIr_lVqGChqIPjlihsoZh-dMyLY1jorT8Mj5RxQYE,3154
+django_watch-0.5.1.dist-info/LICENSE,sha256=BvmWh0aXPp8jrD0GS25NwyJ321UbcQ7KIui9wAmwVD0,1094
+django_watch-0.5.1.dist-info/METADATA,sha256=SVG-gxBTkfvyao_oFyLB-veT8IFsPjK9rF4Ew_9aPUY,1900
+django_watch-0.5.1.dist-info/WHEEL,sha256=G16H4A3IeoQmnOrYV4ueZGKSjhipXx8zc8nu9FGlvMA,92
+django_watch-0.5.1.dist-info/top_level.txt,sha256=Q6Y_7H4paLM2YTKdPpC2LHZ4a2zUoWHBxkv9GmX9SOg,13
+django_watch-0.5.1.dist-info/RECORD,,
```

