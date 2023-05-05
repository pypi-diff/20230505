# Comparing `tmp/bdffont-0.0.3.tar.gz` & `tmp/bdffont-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bdffont-0.0.3.tar", last modified: Fri May  5 12:39:04 2023, max compression
+gzip compressed data, was "bdffont-0.0.4.tar", last modified: Fri May  5 14:17:57 2023, max compression
```

## Comparing `bdffont-0.0.3.tar` & `bdffont-0.0.4.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 takwolf    (502) staff       (20)        0 2023-05-05 12:39:04.693933 bdffont-0.0.3/
--rw-r--r--   0 takwolf    (502) staff       (20)     1064 2023-05-03 16:58:01.000000 bdffont-0.0.3/LICENSE
--rw-r--r--   0 takwolf    (502) staff       (20)     2508 2023-05-05 12:39:04.693792 bdffont-0.0.3/PKG-INFO
--rw-r--r--   0 takwolf    (502) staff       (20)     1914 2023-05-05 12:26:32.000000 bdffont-0.0.3/README.md
--rw-r--r--   0 takwolf    (502) staff       (20)      670 2023-05-05 12:36:51.000000 bdffont-0.0.3/pyproject.toml
--rw-r--r--   0 takwolf    (502) staff       (20)       38 2023-05-05 12:39:04.693980 bdffont-0.0.3/setup.cfg
-drwxr-xr-x   0 takwolf    (502) staff       (20)        0 2023-05-05 12:39:04.689568 bdffont-0.0.3/src/
-drwxr-xr-x   0 takwolf    (502) staff       (20)        0 2023-05-05 12:39:04.692299 bdffont-0.0.3/src/bdffont/
--rw-r--r--   0 takwolf    (502) staff       (20)      177 2023-05-05 04:46:00.000000 bdffont-0.0.3/src/bdffont/__init__.py
--rw-r--r--   0 takwolf    (502) staff       (20)      691 2023-05-05 06:07:54.000000 bdffont-0.0.3/src/bdffont/error.py
--rw-r--r--   0 takwolf    (502) staff       (20)     6626 2023-05-05 12:13:15.000000 bdffont-0.0.3/src/bdffont/font.py
--rw-r--r--   0 takwolf    (502) staff       (20)     5378 2023-05-05 12:06:41.000000 bdffont-0.0.3/src/bdffont/glyph.py
--rw-r--r--   0 takwolf    (502) staff       (20)     5859 2023-05-05 12:15:06.000000 bdffont-0.0.3/src/bdffont/parser.py
--rw-r--r--   0 takwolf    (502) staff       (20)     3878 2023-05-05 11:18:51.000000 bdffont-0.0.3/src/bdffont/properties.py
-drwxr-xr-x   0 takwolf    (502) staff       (20)        0 2023-05-05 12:39:04.693050 bdffont-0.0.3/src/bdffont.egg-info/
--rw-r--r--   0 takwolf    (502) staff       (20)     2508 2023-05-05 12:39:04.000000 bdffont-0.0.3/src/bdffont.egg-info/PKG-INFO
--rw-r--r--   0 takwolf    (502) staff       (20)      347 2023-05-05 12:39:04.000000 bdffont-0.0.3/src/bdffont.egg-info/SOURCES.txt
--rw-r--r--   0 takwolf    (502) staff       (20)        1 2023-05-05 12:39:04.000000 bdffont-0.0.3/src/bdffont.egg-info/dependency_links.txt
--rw-r--r--   0 takwolf    (502) staff       (20)        8 2023-05-05 12:39:04.000000 bdffont-0.0.3/src/bdffont.egg-info/top_level.txt
-drwxr-xr-x   0 takwolf    (502) staff       (20)        0 2023-05-05 12:39:04.693481 bdffont-0.0.3/tests/
--rw-r--r--   0 takwolf    (502) staff       (20)     1967 2023-05-05 06:21:06.000000 bdffont-0.0.3/tests/test_damaged.py
--rw-r--r--   0 takwolf    (502) staff       (20)     3291 2023-05-05 12:32:00.000000 bdffont-0.0.3/tests/test_demo.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 14:17:57.994434 bdffont-0.0.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-05-05 14:17:39.000000 bdffont-0.0.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2508 2023-05-05 14:17:57.994434 bdffont-0.0.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1914 2023-05-05 14:17:39.000000 bdffont-0.0.4/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      670 2023-05-05 14:17:39.000000 bdffont-0.0.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-05 14:17:57.994434 bdffont-0.0.4/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 14:17:57.990434 bdffont-0.0.4/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 14:17:57.994434 bdffont-0.0.4/src/bdffont/
+-rw-r--r--   0 runner    (1001) docker     (123)      177 2023-05-05 14:17:39.000000 bdffont-0.0.4/src/bdffont/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      691 2023-05-05 14:17:39.000000 bdffont-0.0.4/src/bdffont/error.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6626 2023-05-05 14:17:39.000000 bdffont-0.0.4/src/bdffont/font.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5378 2023-05-05 14:17:39.000000 bdffont-0.0.4/src/bdffont/glyph.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5928 2023-05-05 14:17:39.000000 bdffont-0.0.4/src/bdffont/parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3878 2023-05-05 14:17:39.000000 bdffont-0.0.4/src/bdffont/properties.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 14:17:57.994434 bdffont-0.0.4/src/bdffont.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2508 2023-05-05 14:17:57.000000 bdffont-0.0.4/src/bdffont.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      347 2023-05-05 14:17:57.000000 bdffont-0.0.4/src/bdffont.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 14:17:57.000000 bdffont-0.0.4/src/bdffont.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-05 14:17:57.000000 bdffont-0.0.4/src/bdffont.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 14:17:57.994434 bdffont-0.0.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1967 2023-05-05 14:17:39.000000 bdffont-0.0.4/tests/test_damaged.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3291 2023-05-05 14:17:39.000000 bdffont-0.0.4/tests/test_demo.py
```

### Comparing `bdffont-0.0.3/LICENSE` & `bdffont-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `bdffont-0.0.3/PKG-INFO` & `bdffont-0.0.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bdffont
-Version: 0.0.3
+Version: 0.0.4
 Summary: A library for manipulating '.bdf' format fonts.
 Author: TakWolf
 Maintainer: TakWolf
 License: MIT License
 Project-URL: homepage, https://github.com/TakWolf/bdffont
 Project-URL: source, https://github.com/TakWolf/bdffont
 Project-URL: issues, https://github.com/TakWolf/bdffont/issues
```

### Comparing `bdffont-0.0.3/README.md` & `bdffont-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `bdffont-0.0.3/pyproject.toml` & `bdffont-0.0.4/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [project]
 name = "bdffont"
-version = "0.0.3"
+version = "0.0.4"
 description = "A library for manipulating '.bdf' format fonts."
 readme = "README.md"
 license = { text = "MIT License" }
 requires-python = ">=3.10"
 authors = [
     { name = "TakWolf" },
 ]
```

### Comparing `bdffont-0.0.3/src/bdffont/error.py` & `bdffont-0.0.4/src/bdffont/error.py`

 * *Files identical despite different names*

### Comparing `bdffont-0.0.3/src/bdffont/font.py` & `bdffont-0.0.4/src/bdffont/font.py`

 * *Files identical despite different names*

### Comparing `bdffont-0.0.3/src/bdffont/glyph.py` & `bdffont-0.0.4/src/bdffont/glyph.py`

 * *Files identical despite different names*

### Comparing `bdffont-0.0.3/src/bdffont/parser.py` & `bdffont-0.0.4/src/bdffont/parser.py`

 * *Files 2% similar despite different names*

```diff
@@ -31,15 +31,18 @@
     return ints
 
 
 def _convert_tail_to_properties_value(tail: str) -> str | int:
     if tail.startswith('"') and tail.endswith('"'):
         value = tail.removeprefix('"').removesuffix('"')
     else:
-        value = int(tail)
+        try:
+            value = int(tail)
+        except ValueError:
+            value = tail
     return value
 
 
 def _decode_properties_segment(lines: Iterator[str], count: int) -> BdfProperties:
     properties = BdfProperties()
     while line_params := _next_word_line(lines):
         word, tail = line_params
```

### Comparing `bdffont-0.0.3/src/bdffont/properties.py` & `bdffont-0.0.4/src/bdffont/properties.py`

 * *Files identical despite different names*

### Comparing `bdffont-0.0.3/src/bdffont.egg-info/PKG-INFO` & `bdffont-0.0.4/src/bdffont.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: bdffont
-Version: 0.0.3
+Version: 0.0.4
 Summary: A library for manipulating '.bdf' format fonts.
 Author: TakWolf
 Maintainer: TakWolf
 License: MIT License
 Project-URL: homepage, https://github.com/TakWolf/bdffont
 Project-URL: source, https://github.com/TakWolf/bdffont
 Project-URL: issues, https://github.com/TakWolf/bdffont/issues
```

### Comparing `bdffont-0.0.3/tests/test_damaged.py` & `bdffont-0.0.4/tests/test_damaged.py`

 * *Files identical despite different names*

### Comparing `bdffont-0.0.3/tests/test_demo.py` & `bdffont-0.0.4/tests/test_demo.py`

 * *Files identical despite different names*

