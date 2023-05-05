# Comparing `tmp/miniflask-5.1.1.tar.gz` & `tmp/miniflask-5.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "miniflask-5.1.1.tar", last modified: Tue Feb 28 14:45:16 2023, max compression
+gzip compressed data, was "miniflask-5.1.2.tar", last modified: Fri May  5 12:55:00 2023, max compression
```

## Comparing `miniflask-5.1.1.tar` & `miniflask-5.1.2.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 14:45:16.047315 miniflask-5.1.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-02-28 14:45:10.000000 miniflask-5.1.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     3730 2023-02-28 14:45:16.047315 miniflask-5.1.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2550 2023-02-28 14:45:10.000000 miniflask-5.1.1/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-28 14:45:16.047315 miniflask-5.1.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2276 2023-02-28 14:45:10.000000 miniflask-5.1.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 14:45:16.043315 miniflask-5.1.1/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 14:45:16.047315 miniflask-5.1.1/src/miniflask/
--rw-r--r--   0 runner    (1001) docker     (123)      659 2023-02-28 14:45:10.000000 miniflask-5.1.1/src/miniflask/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 14:45:16.047315 miniflask-5.1.1/src/miniflask/definitions/
--rw-r--r--   0 runner    (1001) docker     (123)      132 2023-02-28 14:45:10.000000 miniflask-5.1.1/src/miniflask/definitions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1086 2023-02-28 14:45:10.000000 miniflask-5.1.1/src/miniflask/dummy.py
--rw-r--r--   0 runner    (1001) docker     (123)    23080 2023-02-28 14:45:10.000000 miniflask-5.1.1/src/miniflask/event.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 14:45:16.047315 miniflask-5.1.1/src/miniflask/events/
--rw-r--r--   0 runner    (1001) docker     (123)     6222 2023-02-28 14:45:10.000000 miniflask-5.1.1/src/miniflask/events/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2971 2023-02-28 14:45:10.000000 miniflask-5.1.1/src/miniflask/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 14:45:16.047315 miniflask-5.1.1/src/miniflask/info/
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-02-28 14:45:10.000000 miniflask-5.1.1/src/miniflask/info/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    86785 2023-02-28 14:45:10.000000 miniflask-5.1.1/src/miniflask/miniflask.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 14:45:16.047315 miniflask-5.1.1/src/miniflask/modules/
--rw-r--r--   0 runner    (1001) docker     (123)      230 2023-02-28 14:45:10.000000 miniflask-5.1.1/src/miniflask/modules/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 14:45:16.047315 miniflask-5.1.1/src/miniflask/settings/
--rw-r--r--   0 runner    (1001) docker     (123)     4922 2023-02-28 14:45:10.000000 miniflask-5.1.1/src/miniflask/settings/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    21899 2023-02-28 14:45:10.000000 miniflask-5.1.1/src/miniflask/state.py
--rw-r--r--   0 runner    (1001) docker     (123)     9844 2023-02-28 14:45:10.000000 miniflask-5.1.1/src/miniflask/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-28 14:45:16.047315 miniflask-5.1.1/src/miniflask.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3730 2023-02-28 14:45:16.000000 miniflask-5.1.1/src/miniflask.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      553 2023-02-28 14:45:16.000000 miniflask-5.1.1/src/miniflask.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-28 14:45:16.000000 miniflask-5.1.1/src/miniflask.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-02-28 14:45:16.000000 miniflask-5.1.1/src/miniflask.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-02-28 14:45:16.000000 miniflask-5.1.1/src/miniflask.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 12:55:00.103622 miniflask-5.1.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-05-05 12:54:54.000000 miniflask-5.1.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     3730 2023-05-05 12:55:00.103622 miniflask-5.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2550 2023-05-05 12:54:54.000000 miniflask-5.1.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-05 12:55:00.103622 miniflask-5.1.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2276 2023-05-05 12:54:54.000000 miniflask-5.1.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 12:55:00.099622 miniflask-5.1.2/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 12:55:00.103622 miniflask-5.1.2/src/miniflask/
+-rw-r--r--   0 runner    (1001) docker     (123)      659 2023-05-05 12:54:54.000000 miniflask-5.1.2/src/miniflask/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 12:55:00.103622 miniflask-5.1.2/src/miniflask/definitions/
+-rw-r--r--   0 runner    (1001) docker     (123)      132 2023-05-05 12:54:54.000000 miniflask-5.1.2/src/miniflask/definitions/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1086 2023-05-05 12:54:54.000000 miniflask-5.1.2/src/miniflask/dummy.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23080 2023-05-05 12:54:54.000000 miniflask-5.1.2/src/miniflask/event.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 12:55:00.103622 miniflask-5.1.2/src/miniflask/events/
+-rw-r--r--   0 runner    (1001) docker     (123)     6222 2023-05-05 12:54:54.000000 miniflask-5.1.2/src/miniflask/events/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2971 2023-05-05 12:54:54.000000 miniflask-5.1.2/src/miniflask/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 12:55:00.103622 miniflask-5.1.2/src/miniflask/info/
+-rw-r--r--   0 runner    (1001) docker     (123)       85 2023-05-05 12:54:54.000000 miniflask-5.1.2/src/miniflask/info/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    86785 2023-05-05 12:54:54.000000 miniflask-5.1.2/src/miniflask/miniflask.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 12:55:00.103622 miniflask-5.1.2/src/miniflask/modules/
+-rw-r--r--   0 runner    (1001) docker     (123)      230 2023-05-05 12:54:54.000000 miniflask-5.1.2/src/miniflask/modules/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 12:55:00.103622 miniflask-5.1.2/src/miniflask/settings/
+-rw-r--r--   0 runner    (1001) docker     (123)     4922 2023-05-05 12:54:54.000000 miniflask-5.1.2/src/miniflask/settings/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21933 2023-05-05 12:54:54.000000 miniflask-5.1.2/src/miniflask/state.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9844 2023-05-05 12:54:54.000000 miniflask-5.1.2/src/miniflask/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 12:55:00.103622 miniflask-5.1.2/src/miniflask.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3730 2023-05-05 12:55:00.000000 miniflask-5.1.2/src/miniflask.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      553 2023-05-05 12:55:00.000000 miniflask-5.1.2/src/miniflask.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 12:55:00.000000 miniflask-5.1.2/src/miniflask.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-05 12:55:00.000000 miniflask-5.1.2/src/miniflask.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-05-05 12:55:00.000000 miniflask-5.1.2/src/miniflask.egg-info/top_level.txt
```

### Comparing `miniflask-5.1.1/LICENSE` & `miniflask-5.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `miniflask-5.1.1/PKG-INFO` & `miniflask-5.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: miniflask
-Version: 5.1.1
+Version: 5.1.2
 Summary: Small research-oriented hook-based plugin engine.
 Home-page: https://github.com/da-h/miniflask
 Author: David Hartmann
 Maintainer: David Hartmann
 License: MIT License
 Keywords: miniflask,plugin-engine,plugin-system
 Classifier: Development Status :: 4 - Beta
```

### Comparing `miniflask-5.1.1/README.md` & `miniflask-5.1.2/README.md`

 * *Files identical despite different names*

### Comparing `miniflask-5.1.1/setup.py` & `miniflask-5.1.2/setup.py`

 * *Files identical despite different names*

### Comparing `miniflask-5.1.1/src/miniflask/__init__.py` & `miniflask-5.1.2/src/miniflask/__init__.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from .miniflask import miniflask as init, print_info, get_default_args
 from .event import outervar
 from .state import optional
 
 # meta
-__version__       = "5.1.1"
+__version__       = "5.1.2"
 __title__         = "miniflask"
 __description__   = "Small research-oriented hook-based plugin engine."
 __url__           = "https://github.com/da-h/miniflask"
 __uri__           = __url__
 __doc__           = __description__ + " <" + __uri__ + ">"
 __documentation__ = 'https://da-h.github.io/miniflask'
 __source__        = __url__
```

### Comparing `miniflask-5.1.1/src/miniflask/dummy.py` & `miniflask-5.1.2/src/miniflask/dummy.py`

 * *Files identical despite different names*

### Comparing `miniflask-5.1.1/src/miniflask/event.py` & `miniflask-5.1.2/src/miniflask/event.py`

 * *Files identical despite different names*

### Comparing `miniflask-5.1.1/src/miniflask/events/__init__.py` & `miniflask-5.1.2/src/miniflask/events/__init__.py`

 * *Files identical despite different names*

### Comparing `miniflask-5.1.1/src/miniflask/exceptions.py` & `miniflask-5.1.2/src/miniflask/exceptions.py`

 * *Files identical despite different names*

### Comparing `miniflask-5.1.1/src/miniflask/miniflask.py` & `miniflask-5.1.2/src/miniflask/miniflask.py`

 * *Files identical despite different names*

### Comparing `miniflask-5.1.1/src/miniflask/settings/__init__.py` & `miniflask-5.1.2/src/miniflask/settings/__init__.py`

 * *Files identical despite different names*

### Comparing `miniflask-5.1.1/src/miniflask/state.py` & `miniflask-5.1.2/src/miniflask/state.py`

 * *Files 2% similar despite different names*

```diff
@@ -371,15 +371,16 @@
 
     def __call__(self, state, event):  # pylint: disable=redefined-outer-name
         return self.type
 
     def str(self, asciicodes=True, color_attr=attr):
         if not asciicodes:
             color_attr = lambda x: ''  # noqa: E731 no-lambda
-        return color_attr('dim') + "'" + str(self.type) + "' or '" + "None" + "' ⟶   " + color_attr('reset') + str(self.dependencies)
+        alt = "None" if isinstance(self.type, list) else "[]"
+        return color_attr('dim') + "'" + str(self.type) + "' or '" + alt + "' ⟶   " + color_attr('reset')
 
     def __str__(self):
         return self.str()
 
 
 class state_node:
```

### Comparing `miniflask-5.1.1/src/miniflask/util.py` & `miniflask-5.1.2/src/miniflask/util.py`

 * *Files identical despite different names*

### Comparing `miniflask-5.1.1/src/miniflask.egg-info/PKG-INFO` & `miniflask-5.1.2/src/miniflask.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: miniflask
-Version: 5.1.1
+Version: 5.1.2
 Summary: Small research-oriented hook-based plugin engine.
 Home-page: https://github.com/da-h/miniflask
 Author: David Hartmann
 Maintainer: David Hartmann
 License: MIT License
 Keywords: miniflask,plugin-engine,plugin-system
 Classifier: Development Status :: 4 - Beta
```

### Comparing `miniflask-5.1.1/src/miniflask.egg-info/SOURCES.txt` & `miniflask-5.1.2/src/miniflask.egg-info/SOURCES.txt`

 * *Files identical despite different names*

