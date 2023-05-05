# Comparing `tmp/commandline_parsable-0.1.1.tar.gz` & `tmp/commandline_parsable-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/commandline_parsable-0.1.1.tar", last modified: Thu Jun 28 13:56:50 2018, max compression
+gzip compressed data, was "commandline_parsable-0.2.0.tar", last modified: Fri May  5 20:31:32 2023, max compression
```

## Comparing `commandline_parsable-0.1.1.tar` & `commandline_parsable-0.2.0.tar`

### file list

```diff
@@ -1,11 +1,12 @@
-drwxr-xr-x   0 thiel     (5095) tbi       (1000)        0 2018-06-28 13:56:50.000000 commandline_parsable-0.1.1/
-drwxr-xr-x   0 thiel     (5095) tbi       (1000)        0 2018-06-28 13:56:50.000000 commandline_parsable-0.1.1/commandline_parsable.egg-info/
--rw-r--r--   0 thiel     (5095) tbi       (1000)      330 2018-06-28 13:56:50.000000 commandline_parsable-0.1.1/commandline_parsable.egg-info/PKG-INFO
--rw-r--r--   0 thiel     (5095) tbi       (1000)      251 2018-06-28 13:56:50.000000 commandline_parsable-0.1.1/commandline_parsable.egg-info/SOURCES.txt
--rw-r--r--   0 thiel     (5095) tbi       (1000)        1 2018-06-28 13:56:50.000000 commandline_parsable-0.1.1/commandline_parsable.egg-info/dependency_links.txt
--rw-r--r--   0 thiel     (5095) tbi       (1000)        6 2018-06-28 13:56:50.000000 commandline_parsable-0.1.1/commandline_parsable.egg-info/requires.txt
--rw-r--r--   0 thiel     (5095) tbi       (1000)       21 2018-06-28 13:56:50.000000 commandline_parsable-0.1.1/commandline_parsable.egg-info/top_level.txt
--rw-r--r--   0 thiel     (5095) tbi       (1000)    11025 2018-05-18 11:46:48.000000 commandline_parsable-0.1.1/commandline_parsable.py
--rw-r--r--   0 thiel     (5095) tbi       (1000)      387 2018-06-28 13:56:25.000000 commandline_parsable-0.1.1/setup.py
--rw-r--r--   0 thiel     (5095) tbi       (1000)      330 2018-06-28 13:56:50.000000 commandline_parsable-0.1.1/PKG-INFO
--rw-r--r--   0 thiel     (5095) tbi       (1000)       38 2018-06-28 13:56:50.000000 commandline_parsable-0.1.1/setup.cfg
+drwxr-xr-x   0 thiel     (1000) thiel     (1000)        0 2023-05-05 20:31:32.606533 commandline_parsable-0.2.0/
+-rw-r--r--   0 thiel     (1000) thiel     (1000)     1071 2017-11-15 12:11:43.000000 commandline_parsable-0.2.0/LICENSE
+-rw-r--r--   0 thiel     (1000) thiel     (1000)      262 2023-05-05 20:31:32.606533 commandline_parsable-0.2.0/PKG-INFO
+drwxr-xr-x   0 thiel     (1000) thiel     (1000)        0 2023-05-05 20:31:32.606533 commandline_parsable-0.2.0/commandline_parsable.egg-info/
+-rw-r--r--   0 thiel     (1000) thiel     (1000)      262 2023-05-05 20:31:32.000000 commandline_parsable-0.2.0/commandline_parsable.egg-info/PKG-INFO
+-rw-r--r--   0 thiel     (1000) thiel     (1000)      259 2023-05-05 20:31:32.000000 commandline_parsable-0.2.0/commandline_parsable.egg-info/SOURCES.txt
+-rw-r--r--   0 thiel     (1000) thiel     (1000)        1 2023-05-05 20:31:32.000000 commandline_parsable-0.2.0/commandline_parsable.egg-info/dependency_links.txt
+-rw-r--r--   0 thiel     (1000) thiel     (1000)        6 2023-05-05 20:31:32.000000 commandline_parsable-0.2.0/commandline_parsable.egg-info/requires.txt
+-rw-r--r--   0 thiel     (1000) thiel     (1000)       21 2023-05-05 20:31:32.000000 commandline_parsable-0.2.0/commandline_parsable.egg-info/top_level.txt
+-rw-r--r--   0 thiel     (1000) thiel     (1000)    12142 2020-01-07 14:50:53.000000 commandline_parsable-0.2.0/commandline_parsable.py
+-rw-r--r--   0 thiel     (1000) thiel     (1000)       38 2023-05-05 20:31:32.606533 commandline_parsable-0.2.0/setup.cfg
+-rw-r--r--   0 thiel     (1000) thiel     (1000)      387 2023-05-05 20:29:46.000000 commandline_parsable-0.2.0/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `commandline_parsable-0.1.1/commandline_parsable.py` & `commandline_parsable-0.2.0/commandline_parsable.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,19 @@
 import inspect
 import logging
 import regex as re
 import traceback
 import sys
 
+if sys.version_info[0] >2:
+    PY3K=True
+else:
+    PY3K=False
+    import six
+
 from collections import OrderedDict
 log=logging.getLogger(__name__)
 
 
 def _get_all_subclasses(cls, include_base = False):
     """
     Get all subclasses of a given class, unless they are abstract.
@@ -49,19 +55,16 @@
 
     If __annotations__ is not present (py2k) or empty, do not perform any conversion.
 
     This tries to perform the conversion by calling the type (works for int,str).
     If calling the type results in an error, no conversion is performed.
     """
     args = list(args)
-    try:
+    if PY3K:
         argspec = inspect.getfullargspec(function)
-    except AttributeError:
-        pass # Py2K
-    else:
         annot = argspec.annotations
         log.debug("Function's annotations are: %s", annot)
         for i, arg in enumerate(argspec.args):
             i=i-1 # cls/ self does not count
             if arg in annot:
                 log.debug("For arg %s: i=%s, args=%s", arg, i, args)
                 if i<len(args):
@@ -76,33 +79,59 @@
 
 def call(function, *args, **kwargs):
     try:
         return _convert_and_call(function, *args, **kwargs)
     except TypeError as e:
         if "argument" not in str(e):
             raise
-        if hasattr(function, "__init__"):
-            argspec = inspect.getargspec(function.__init__)
-            target_args = argspec.args[1:]
-        else:
+        t, v, tb = sys.exc_info()
+        log.error("Error calling %s", function.__name__)
+        log.exception("The following exception occured and will be reraised with a potentially different message:")
+        log.error(" ")
+        try:
+            log.debug("Getting rgspec of function")
             argspec = inspect.getargspec(function)
             target_args = argspec.args
-        target_kwargs = target_args[len(args):]
+        except TypeError:
+            try:
+                log.debug("getting argspec of init")
+                argspec = inspect.getargspec(function.__init__)
+            except TypeError as e2:
+                log.debug("Cannot get argspec: %s", e2)
+                if PY3K:
+                    raise e #from None
+                else:
+                    # Reraise original error
+                    six.reraise(t, v, tb)
+            target_args = argspec.args[1:]
+
+        target_kwargs = target_args[len(args)+1:]
         missing_args = set(target_kwargs) - set(kwargs.keys())
         tb = traceback.extract_tb(sys.exc_info()[2])
         signature = ", ".join(argspec.args)
         if argspec.varargs:
-            singature+=", *{}".format(argspec.varargs)
+            signature+=", *{}".format(argspec.varargs)
         if argspec.keywords:
-            singature+=", **{}".format(argspec.keywords)
-        used_sig = ", ".join(args)+", "*(bool(args) and bool(kwargs))+", ".join("{}={}".format(k,v) for k,v in kwargs.items())
+            signature+=", **{}".format(argspec.keywords)
+        used_sig = ", ".join(map(repr,args))+", "*(bool(args) and bool(kwargs))+", ".join("{}={}".format(k,v) for k,v in kwargs.items())
         if tb[-1][2] == "_convert_and_call":
+            try:
+               fname = function.__qualname__
+            except AttributeError:
+               try:
+                  if function.im_self is not None: # bound method
+                      fname = function.im_self.__name__ + "." + function.__name__
+                  else:
+                      fname = function.im_class.__name__ + "." + function.__name__
+               except Exception as ex2:
+                  # py 3.0-3.2
+                  fname = function.__name__
             msg = (str(e) + "\nTried to call {fun} with signature ({target_sig}) (from module"
                            " {module}) as {fun}({used_sig}) "
-                           "".format(fun=function.__name__,
+                           "".format(fun=fname,
                                      target_sig = signature,
                                      module=function.__module__,
                                      used_sig=used_sig
                                     ))
             if missing_args:
                 msg+=("The following arguments are "
                       "missing: {}".format(list(missing_args)))
```

