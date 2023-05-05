# Comparing `tmp/django_watch-0.4.2-py3-none-any.whl.zip` & `tmp/django_watch-0.5-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 3870 bytes, number of entries: 7
--rw-rw-r--  2.0 unx        0 b- defN 20-Jan-27 13:04 django_watch/__init__.py
--rw-rw-r--  2.0 unx     3656 b- defN 22-Sep-16 15:09 django_watch/middleware.py
--rw-r--r--  2.0 unx     1094 b- defN 22-Sep-16 15:12 django_watch-0.4.2.dist-info/LICENSE
--rw-rw-r--  2.0 unx     1421 b- defN 22-Sep-16 15:12 django_watch-0.4.2.dist-info/METADATA
--rw-rw-r--  2.0 unx       92 b- defN 22-Sep-16 15:12 django_watch-0.4.2.dist-info/WHEEL
--rw-rw-r--  2.0 unx       13 b- defN 22-Sep-16 15:12 django_watch-0.4.2.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      572 b- defN 22-Sep-16 15:12 django_watch-0.4.2.dist-info/RECORD
-7 files, 6848 bytes uncompressed, 2848 bytes compressed:  58.4%
+Zip file size: 3954 bytes, number of entries: 7
+-rwxr-xr-x  2.0 unx        0 b- defN 20-Jan-27 13:04 django_watch/__init__.py
+-rw-rw-r--  2.0 unx     3121 b- defN 23-May-05 04:56 django_watch/middleware.py
+-rwxr-xr-x  2.0 unx     1094 b- defN 23-May-05 05:00 django_watch-0.5.dist-info/LICENSE
+-rw-rw-r--  2.0 unx     1898 b- defN 23-May-05 05:00 django_watch-0.5.dist-info/METADATA
+-rw-rw-r--  2.0 unx       92 b- defN 23-May-05 05:00 django_watch-0.5.dist-info/WHEEL
+-rwxr-xr-x  2.0 unx       13 b- defN 23-May-05 05:00 django_watch-0.5.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      562 b- defN 23-May-05 05:00 django_watch-0.5.dist-info/RECORD
+7 files, 6780 bytes uncompressed, 2952 bytes compressed:  56.5%
```

## zipnote {}

```diff
@@ -1,22 +1,22 @@
 Filename: django_watch/__init__.py
 Comment: 
 
 Filename: django_watch/middleware.py
 Comment: 
 
-Filename: django_watch-0.4.2.dist-info/LICENSE
+Filename: django_watch-0.5.dist-info/LICENSE
 Comment: 
 
-Filename: django_watch-0.4.2.dist-info/METADATA
+Filename: django_watch-0.5.dist-info/METADATA
 Comment: 
 
-Filename: django_watch-0.4.2.dist-info/WHEEL
+Filename: django_watch-0.5.dist-info/WHEEL
 Comment: 
 
-Filename: django_watch-0.4.2.dist-info/top_level.txt
+Filename: django_watch-0.5.dist-info/top_level.txt
 Comment: 
 
-Filename: django_watch-0.4.2.dist-info/RECORD
+Filename: django_watch-0.5.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## django_watch/middleware.py

```diff
@@ -1,9 +1,10 @@
 import time
 import logging
+import traceback
 
 
 def unwrap(func):
     while hasattr(func, "__wrapped__"):
         func = func.__wrapped__
     return func
 
@@ -34,50 +35,41 @@
         self.BLINK = "\033[5m"
         self.NEGATIVE = "\033[7m"
         self.CROSSED = "\033[9m"
         self.END = "\033[0m"
 
     def __call__(self, request):
         response = None
-        time_start = time.monotonic()     
+        time_start = time.monotonic()    
         response = self.get_response(request)
-        if hasattr(response, "status_code") and response.status_code in [200, 201] and hasattr(request, "process_stdout_end") and request.process_stdout_end:
+
+        if hasattr(response, "status_code") and hasattr(request, "process_stdout_end") and request.process_stdout_end:
             process_stdout_end = request.process_stdout_end            
-            process_stdout_end += f"{self.YELLOW} • Total time • {round((time.monotonic() - time_start), 2)}s{self.END}"        
-            print(process_stdout_end)      
+            process_stdout_end += f"{self.YELLOW} • STATUS {response.status_code} • Total time • {round((time.monotonic() - time_start), 2)}s{self.END}"        
+   
         return response
 
     def process_view(self, request, func, args, kwargs):                 
         func = unwrap(func)   
         if hasattr(func, "__code__"):
-            process_stdout_start = f"\n{self.GREEN}START {func.__code__.co_filename} • {self.END}{self.RED}{self.BOLD}{func.__name__}{self.END}{self.END} {self.GREEN}•{self.END} {self.LIGHT_BLUE}Line number {func.__code__.co_firstlineno}{self.END}"
-            request.process_stdout_end = f"\n{self.YELLOW}{self.BOLD}END {func.__code__.co_filename} • {self.END}{self.RED}{self.BOLD}{func.__name__}{self.END}{self.END}"
+            process_stdout_start = f"\n| {self.GREEN}START {request.method} {func.__code__.co_filename} {self.END}| • {self.GREEN}{self.BOLD}{func.__name__}{self.END}{self.END} {self.GREEN}•{self.END} {self.GREEN}Line number {func.__code__.co_firstlineno}{self.END}"
+            request.process_stdout_end = f"\n| {self.YELLOW}{self.BOLD}END {request.method} {func.__code__.co_filename} {self.END}| • {self.YELLOW}{self.BOLD}{func.__name__}{self.END}{self.END}"
             
-            print_part = None
+            print(process_stdout_start)
             if args: 
-                print_part = f"args: {args}"
+                print(f"| args: {args}"[:200])
             if kwargs: 
-                print_part = f"kwargs: {kwargs}"
+                print(f"| kwargs: {kwargs}"[:200])
             if request.GET:
-                print_part = f"request.GET: {request.GET}"                
+                print(f"| request.GET: {request.GET}"[:200])                
             if request.POST: 
-                print_part = f"request.POST: {request.POST}"
+                print(f"| request.POST: {request.POST}"[:200])
                 
             try:
                 if not request.POST and request.body:
-                    print_part = f"request.body: {request.body}"
+                    print(f"| request.body: {request.body}"[:200])
             except Exception as e:
-                logging.exception(e)
+                pass
             
-            if print_part:         
-                if len(print_part) > 200:
-                    process_stdout_start += f"\n{self.PURPLE}%s ...{self.END}" % print_part[:200]
-                else:
-                    process_stdout_start += f"\n{self.PURPLE}%s{self.END}" % print_part                                                        
-            print(process_stdout_start) 
-
     def process_exception(self, request, exception):
-        if hasattr(request, "process_stdout_end") and request.process_stdout_end: 
-            exception_stdout = request.process_stdout_end.replace(self.YELLOW, self.RED)  
-            exception_stdout = f"{self.RED}{self.BOLD} {exception_stdout}{self.END}{self.END} {self.RED}{self.BOLD}• Exception {exception}{self.END}{self.END}"
-            print(exception_stdout)
- 
+        print(f"{self.RED}{self.BOLD}| Exception{self.END}{self.END}")
+        print( "| TRACEBACK:\n{}".format( "".join(traceback.format_exception(type(exception), exception, exception.__traceback__))))
```

## Comparing `django_watch-0.4.2.dist-info/LICENSE` & `django_watch-0.5.dist-info/LICENSE`

 * *Files identical despite different names*

