# Comparing `tmp/PythonToolsKit-1.2.4.tar.gz` & `tmp/PythonToolsKit-1.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PythonToolsKit-1.2.4.tar", last modified: Sat Apr 29 07:51:18 2023, max compression
+gzip compressed data, was "PythonToolsKit-1.2.5.tar", last modified: Fri May  5 10:40:51 2023, max compression
```

## Comparing `PythonToolsKit-1.2.4.tar` & `PythonToolsKit-1.2.5.tar`

### file list

```diff
@@ -1,47 +1,47 @@
-drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2023-04-29 07:51:18.403137 PythonToolsKit-1.2.4/
--rw-r--r--   0 kali      (1000) kali      (1000)    35149 2023-04-09 21:21:10.000000 PythonToolsKit-1.2.4/LICENSE.txt
--rw-r--r--   0 kali      (1000) kali      (1000)       27 2023-04-09 21:21:10.000000 PythonToolsKit-1.2.4/MANIFEST.in
--rw-r--r--   0 kali      (1000) kali      (1000)    15504 2023-04-29 07:51:18.403137 PythonToolsKit-1.2.4/PKG-INFO
-drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2023-04-29 07:51:18.403137 PythonToolsKit-1.2.4/PythonToolsKit/
--rw-r--r--   0 kali      (1000) kali      (1000)    14031 2023-04-29 13:44:50.000000 PythonToolsKit-1.2.4/PythonToolsKit/Arguments.py
--rw-r--r--   0 kali      (1000) kali      (1000)     8577 2023-04-29 13:44:50.000000 PythonToolsKit-1.2.4/PythonToolsKit/Characters.py
--rw-r--r--   0 kali      (1000) kali      (1000)    27267 2023-04-29 13:44:50.000000 PythonToolsKit-1.2.4/PythonToolsKit/Colors.py
--rw-r--r--   0 kali      (1000) kali      (1000)    42937 2023-04-29 13:44:50.000000 PythonToolsKit-1.2.4/PythonToolsKit/DataAnalysis.py
--rw-r--r--   0 kali      (1000) kali      (1000)    19183 2023-04-29 13:44:50.000000 PythonToolsKit-1.2.4/PythonToolsKit/DebugEncoding.py
--rw-r--r--   0 kali      (1000) kali      (1000)     5837 2023-04-29 13:44:50.000000 PythonToolsKit-1.2.4/PythonToolsKit/Dict.py
--rw-r--r--   0 kali      (1000) kali      (1000)     4452 2023-04-29 13:44:50.000000 PythonToolsKit-1.2.4/PythonToolsKit/DictObject.py
--rw-r--r--   0 kali      (1000) kali      (1000)    11277 2023-04-29 13:44:50.000000 PythonToolsKit-1.2.4/PythonToolsKit/Encodings.py
--rw-r--r--   0 kali      (1000) kali      (1000)     2661 2023-04-29 13:44:50.000000 PythonToolsKit-1.2.4/PythonToolsKit/Function.py
--rw-r--r--   0 kali      (1000) kali      (1000)     3701 2023-04-29 13:44:50.000000 PythonToolsKit-1.2.4/PythonToolsKit/GetFile.py
--rw-r--r--   0 kali      (1000) kali      (1000)     3810 2023-04-29 13:44:50.000000 PythonToolsKit-1.2.4/PythonToolsKit/GetPass.py
--rw-r--r--   0 kali      (1000) kali      (1000)    19618 2023-04-29 13:44:50.000000 PythonToolsKit-1.2.4/PythonToolsKit/GetType.py
--rw-r--r--   0 kali      (1000) kali      (1000)     2400 2023-04-29 13:44:50.000000 PythonToolsKit-1.2.4/PythonToolsKit/Import.py
--rw-r--r--   0 kali      (1000) kali      (1000)     5260 2023-04-29 13:44:50.000000 PythonToolsKit-1.2.4/PythonToolsKit/Json.py
--rw-r--r--   0 kali      (1000) kali      (1000)     3225 2023-04-29 13:44:50.000000 PythonToolsKit-1.2.4/PythonToolsKit/List.py
--rw-r--r--   0 kali      (1000) kali      (1000)     8574 2023-04-29 13:44:50.000000 PythonToolsKit-1.2.4/PythonToolsKit/Logs.py
--rw-r--r--   0 kali      (1000) kali      (1000)    16523 2023-04-29 13:44:50.000000 PythonToolsKit-1.2.4/PythonToolsKit/OrdDict.py
--rw-r--r--   0 kali      (1000) kali      (1000)     5351 2023-04-29 13:44:50.000000 PythonToolsKit-1.2.4/PythonToolsKit/PrintF.py
--rw-r--r--   0 kali      (1000) kali      (1000)     3392 2023-04-29 13:44:50.000000 PythonToolsKit-1.2.4/PythonToolsKit/Process.py
--rw-r--r--   0 kali      (1000) kali      (1000)     6189 2023-04-29 13:44:50.000000 PythonToolsKit-1.2.4/PythonToolsKit/Random.py
--rw-r--r--   0 kali      (1000) kali      (1000)     2488 2023-04-29 13:44:50.000000 PythonToolsKit-1.2.4/PythonToolsKit/RecursionDebug.py
--rw-r--r--   0 kali      (1000) kali      (1000)    18306 2023-04-29 13:44:50.000000 PythonToolsKit-1.2.4/PythonToolsKit/Report.py
--rw-r--r--   0 kali      (1000) kali      (1000)     9654 2023-04-29 13:44:50.000000 PythonToolsKit-1.2.4/PythonToolsKit/ScapyTools.py
--rw-r--r--   0 kali      (1000) kali      (1000)     7131 2023-04-29 13:44:50.000000 PythonToolsKit-1.2.4/PythonToolsKit/StringF.py
--rw-r--r--   0 kali      (1000) kali      (1000)    15457 2023-04-29 13:44:50.000000 PythonToolsKit-1.2.4/PythonToolsKit/Terminal.py
--rw-r--r--   0 kali      (1000) kali      (1000)     1106 2023-04-09 21:21:10.000000 PythonToolsKit-1.2.4/PythonToolsKit/TestArguments.py
--rw-r--r--   0 kali      (1000) kali      (1000)     4710 2023-04-29 13:44:50.000000 PythonToolsKit-1.2.4/PythonToolsKit/TestTimeout.py
--rw-r--r--   0 kali      (1000) kali      (1000)     3092 2023-04-29 13:44:50.000000 PythonToolsKit-1.2.4/PythonToolsKit/Thread.py
--rw-r--r--   0 kali      (1000) kali      (1000)     7854 2023-04-29 13:44:50.000000 PythonToolsKit-1.2.4/PythonToolsKit/Timeout.py
--rw-r--r--   0 kali      (1000) kali      (1000)     3252 2023-04-29 13:44:50.000000 PythonToolsKit-1.2.4/PythonToolsKit/Tuple.py
--rw-r--r--   0 kali      (1000) kali      (1000)    10004 2023-04-29 13:44:50.000000 PythonToolsKit-1.2.4/PythonToolsKit/WindowsTerminal.py
--rw-r--r--   0 kali      (1000) kali      (1000)     1641 2023-04-29 13:21:36.000000 PythonToolsKit-1.2.4/PythonToolsKit/__init__.py
--rw-r--r--   0 kali      (1000) kali      (1000)     5935 2023-04-29 13:44:50.000000 PythonToolsKit-1.2.4/PythonToolsKit/urlopen.py
-drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2023-04-29 07:51:18.403137 PythonToolsKit-1.2.4/PythonToolsKit.egg-info/
--rw-r--r--   0 kali      (1000) kali      (1000)    15504 2023-04-29 07:51:18.000000 PythonToolsKit-1.2.4/PythonToolsKit.egg-info/PKG-INFO
--rw-r--r--   0 kali      (1000) kali      (1000)     1135 2023-04-29 07:51:18.000000 PythonToolsKit-1.2.4/PythonToolsKit.egg-info/SOURCES.txt
--rw-r--r--   0 kali      (1000) kali      (1000)        1 2023-04-29 07:51:18.000000 PythonToolsKit-1.2.4/PythonToolsKit.egg-info/dependency_links.txt
--rw-r--r--   0 kali      (1000) kali      (1000)      112 2023-04-29 07:51:18.000000 PythonToolsKit-1.2.4/PythonToolsKit.egg-info/entry_points.txt
--rw-r--r--   0 kali      (1000) kali      (1000)       15 2023-04-29 07:51:18.000000 PythonToolsKit-1.2.4/PythonToolsKit.egg-info/top_level.txt
--rw-r--r--   0 kali      (1000) kali      (1000)    10968 2023-04-09 21:21:10.000000 PythonToolsKit-1.2.4/README.md
--rw-r--r--   0 kali      (1000) kali      (1000)       38 2023-04-29 07:51:18.403137 PythonToolsKit-1.2.4/setup.cfg
--rw-r--r--   0 kali      (1000) kali      (1000)     6693 2023-04-09 21:21:10.000000 PythonToolsKit-1.2.4/setup.py
+drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2023-05-05 10:40:51.434679 PythonToolsKit-1.2.5/
+-rw-r--r--   0 kali      (1000) kali      (1000)    35149 2023-05-05 14:37:14.000000 PythonToolsKit-1.2.5/LICENSE.txt
+-rw-r--r--   0 kali      (1000) kali      (1000)       27 2023-05-05 14:37:14.000000 PythonToolsKit-1.2.5/MANIFEST.in
+-rw-r--r--   0 kali      (1000) kali      (1000)    15504 2023-05-05 10:40:51.434679 PythonToolsKit-1.2.5/PKG-INFO
+drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2023-05-05 10:40:51.434679 PythonToolsKit-1.2.5/PythonToolsKit/
+-rw-r--r--   0 kali      (1000) kali      (1000)    14031 2023-05-05 14:37:14.000000 PythonToolsKit-1.2.5/PythonToolsKit/Arguments.py
+-rw-r--r--   0 kali      (1000) kali      (1000)     8577 2023-05-05 14:37:14.000000 PythonToolsKit-1.2.5/PythonToolsKit/Characters.py
+-rw-r--r--   0 kali      (1000) kali      (1000)    27267 2023-05-05 14:37:14.000000 PythonToolsKit-1.2.5/PythonToolsKit/Colors.py
+-rw-r--r--   0 kali      (1000) kali      (1000)    42959 2023-05-05 14:44:46.000000 PythonToolsKit-1.2.5/PythonToolsKit/DataAnalysis.py
+-rw-r--r--   0 kali      (1000) kali      (1000)    19183 2023-05-05 14:37:14.000000 PythonToolsKit-1.2.5/PythonToolsKit/DebugEncoding.py
+-rw-r--r--   0 kali      (1000) kali      (1000)     5837 2023-05-05 14:37:14.000000 PythonToolsKit-1.2.5/PythonToolsKit/Dict.py
+-rw-r--r--   0 kali      (1000) kali      (1000)     4452 2023-05-05 14:37:14.000000 PythonToolsKit-1.2.5/PythonToolsKit/DictObject.py
+-rw-r--r--   0 kali      (1000) kali      (1000)    11277 2023-05-05 14:37:14.000000 PythonToolsKit-1.2.5/PythonToolsKit/Encodings.py
+-rw-r--r--   0 kali      (1000) kali      (1000)     2661 2023-05-05 14:37:14.000000 PythonToolsKit-1.2.5/PythonToolsKit/Function.py
+-rw-r--r--   0 kali      (1000) kali      (1000)     3701 2023-05-05 14:37:14.000000 PythonToolsKit-1.2.5/PythonToolsKit/GetFile.py
+-rw-r--r--   0 kali      (1000) kali      (1000)     3810 2023-05-05 14:37:14.000000 PythonToolsKit-1.2.5/PythonToolsKit/GetPass.py
+-rw-r--r--   0 kali      (1000) kali      (1000)    19618 2023-05-05 14:37:14.000000 PythonToolsKit-1.2.5/PythonToolsKit/GetType.py
+-rw-r--r--   0 kali      (1000) kali      (1000)     2400 2023-05-05 14:37:14.000000 PythonToolsKit-1.2.5/PythonToolsKit/Import.py
+-rw-r--r--   0 kali      (1000) kali      (1000)     5260 2023-05-05 14:37:14.000000 PythonToolsKit-1.2.5/PythonToolsKit/Json.py
+-rw-r--r--   0 kali      (1000) kali      (1000)     3225 2023-05-05 14:37:14.000000 PythonToolsKit-1.2.5/PythonToolsKit/List.py
+-rw-r--r--   0 kali      (1000) kali      (1000)     8574 2023-05-05 14:37:14.000000 PythonToolsKit-1.2.5/PythonToolsKit/Logs.py
+-rw-r--r--   0 kali      (1000) kali      (1000)    16523 2023-05-05 14:37:14.000000 PythonToolsKit-1.2.5/PythonToolsKit/OrdDict.py
+-rw-r--r--   0 kali      (1000) kali      (1000)     5351 2023-05-05 14:37:14.000000 PythonToolsKit-1.2.5/PythonToolsKit/PrintF.py
+-rw-r--r--   0 kali      (1000) kali      (1000)     3392 2023-05-05 14:37:14.000000 PythonToolsKit-1.2.5/PythonToolsKit/Process.py
+-rw-r--r--   0 kali      (1000) kali      (1000)     6189 2023-05-05 14:37:14.000000 PythonToolsKit-1.2.5/PythonToolsKit/Random.py
+-rw-r--r--   0 kali      (1000) kali      (1000)     2488 2023-05-05 14:37:14.000000 PythonToolsKit-1.2.5/PythonToolsKit/RecursionDebug.py
+-rw-r--r--   0 kali      (1000) kali      (1000)    18306 2023-05-05 14:37:14.000000 PythonToolsKit-1.2.5/PythonToolsKit/Report.py
+-rw-r--r--   0 kali      (1000) kali      (1000)     9654 2023-05-05 14:37:14.000000 PythonToolsKit-1.2.5/PythonToolsKit/ScapyTools.py
+-rw-r--r--   0 kali      (1000) kali      (1000)     7131 2023-05-05 14:37:14.000000 PythonToolsKit-1.2.5/PythonToolsKit/StringF.py
+-rw-r--r--   0 kali      (1000) kali      (1000)    15457 2023-05-05 14:37:14.000000 PythonToolsKit-1.2.5/PythonToolsKit/Terminal.py
+-rw-r--r--   0 kali      (1000) kali      (1000)     1106 2023-05-05 14:37:14.000000 PythonToolsKit-1.2.5/PythonToolsKit/TestArguments.py
+-rw-r--r--   0 kali      (1000) kali      (1000)     4710 2023-05-05 14:37:14.000000 PythonToolsKit-1.2.5/PythonToolsKit/TestTimeout.py
+-rw-r--r--   0 kali      (1000) kali      (1000)     3092 2023-05-05 14:37:14.000000 PythonToolsKit-1.2.5/PythonToolsKit/Thread.py
+-rw-r--r--   0 kali      (1000) kali      (1000)     7854 2023-05-05 14:37:14.000000 PythonToolsKit-1.2.5/PythonToolsKit/Timeout.py
+-rw-r--r--   0 kali      (1000) kali      (1000)     3252 2023-05-05 14:37:14.000000 PythonToolsKit-1.2.5/PythonToolsKit/Tuple.py
+-rw-r--r--   0 kali      (1000) kali      (1000)    10004 2023-05-05 14:37:14.000000 PythonToolsKit-1.2.5/PythonToolsKit/WindowsTerminal.py
+-rw-r--r--   0 kali      (1000) kali      (1000)     1641 2023-05-05 14:44:58.000000 PythonToolsKit-1.2.5/PythonToolsKit/__init__.py
+-rw-r--r--   0 kali      (1000) kali      (1000)     5935 2023-05-05 14:37:14.000000 PythonToolsKit-1.2.5/PythonToolsKit/urlopen.py
+drwxr-xr-x   0 kali      (1000) kali      (1000)        0 2023-05-05 10:40:51.434679 PythonToolsKit-1.2.5/PythonToolsKit.egg-info/
+-rw-r--r--   0 kali      (1000) kali      (1000)    15504 2023-05-05 10:40:51.000000 PythonToolsKit-1.2.5/PythonToolsKit.egg-info/PKG-INFO
+-rw-r--r--   0 kali      (1000) kali      (1000)     1135 2023-05-05 10:40:51.000000 PythonToolsKit-1.2.5/PythonToolsKit.egg-info/SOURCES.txt
+-rw-r--r--   0 kali      (1000) kali      (1000)        1 2023-05-05 10:40:51.000000 PythonToolsKit-1.2.5/PythonToolsKit.egg-info/dependency_links.txt
+-rw-r--r--   0 kali      (1000) kali      (1000)      112 2023-05-05 10:40:51.000000 PythonToolsKit-1.2.5/PythonToolsKit.egg-info/entry_points.txt
+-rw-r--r--   0 kali      (1000) kali      (1000)       15 2023-05-05 10:40:51.000000 PythonToolsKit-1.2.5/PythonToolsKit.egg-info/top_level.txt
+-rw-r--r--   0 kali      (1000) kali      (1000)    10968 2023-05-05 14:37:14.000000 PythonToolsKit-1.2.5/README.md
+-rw-r--r--   0 kali      (1000) kali      (1000)       38 2023-05-05 10:40:51.434679 PythonToolsKit-1.2.5/setup.cfg
+-rw-r--r--   0 kali      (1000) kali      (1000)     6693 2023-05-05 14:37:14.000000 PythonToolsKit-1.2.5/setup.py
```

### Comparing `PythonToolsKit-1.2.4/LICENSE.txt` & `PythonToolsKit-1.2.5/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `PythonToolsKit-1.2.4/PKG-INFO` & `PythonToolsKit-1.2.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PythonToolsKit
-Version: 1.2.4
+Version: 1.2.5
 Summary: This package implements tools to build python package and tools.
 Home-page: https://github.com/mauricelambert/PythonToolsKit
 Author: Maurice Lambert
 Author-email: mauricelambert434@gmail.com
 Maintainer: Maurice Lambert
 Maintainer-email: mauricelambert434@gmail.com
 License: GPL-3.0 License
```

### Comparing `PythonToolsKit-1.2.4/PythonToolsKit/Arguments.py` & `PythonToolsKit-1.2.5/PythonToolsKit/Arguments.py`

 * *Files identical despite different names*

### Comparing `PythonToolsKit-1.2.4/PythonToolsKit/Characters.py` & `PythonToolsKit-1.2.5/PythonToolsKit/Characters.py`

 * *Files identical despite different names*

### Comparing `PythonToolsKit-1.2.4/PythonToolsKit/Colors.py` & `PythonToolsKit-1.2.5/PythonToolsKit/Colors.py`

 * *Files identical despite different names*

### Comparing `PythonToolsKit-1.2.4/PythonToolsKit/DataAnalysis.py` & `PythonToolsKit-1.2.5/PythonToolsKit/DataAnalysis.py`

 * *Files 0% similar despite different names*

```diff
@@ -355,15 +355,15 @@
 -------------------------------------
 DataAnalysis.py     290      0   100%
 -------------------------------------
 TOTAL               290      0   100%
 ~#
 """
 
-__version__ = "0.0.1"
+__version__ = "0.0.2"
 __author__ = "Maurice Lambert"
 __author_email__ = "mauricelambert434@gmail.com"
 __maintainer__ = "Maurice Lambert"
 __maintainer_email__ = "mauricelambert434@gmail.com"
 __description__ = """
 This package implements tools to build python package and tools.
 """
@@ -384,14 +384,15 @@
 from typing import Dict, TypeVar, List, Tuple, Union, Any
 from collections.abc import Hashable, Iterable, Callable
 from collections import defaultdict, namedtuple, Counter
 from statistics import fmean, median, pstdev, variance
 from functools import partial
 from datetime import datetime
 from operator import gt, lt
+from sys import argv
 
 try:
     from matplotlib.pyplot import bar, show, title
 except ImportError:
     PYPLOT = False
 else:
     PYPLOT = True
```

### Comparing `PythonToolsKit-1.2.4/PythonToolsKit/DebugEncoding.py` & `PythonToolsKit-1.2.5/PythonToolsKit/DebugEncoding.py`

 * *Files identical despite different names*

### Comparing `PythonToolsKit-1.2.4/PythonToolsKit/Dict.py` & `PythonToolsKit-1.2.5/PythonToolsKit/Dict.py`

 * *Files identical despite different names*

### Comparing `PythonToolsKit-1.2.4/PythonToolsKit/DictObject.py` & `PythonToolsKit-1.2.5/PythonToolsKit/DictObject.py`

 * *Files identical despite different names*

### Comparing `PythonToolsKit-1.2.4/PythonToolsKit/Encodings.py` & `PythonToolsKit-1.2.5/PythonToolsKit/Encodings.py`

 * *Files identical despite different names*

### Comparing `PythonToolsKit-1.2.4/PythonToolsKit/Function.py` & `PythonToolsKit-1.2.5/PythonToolsKit/Function.py`

 * *Files identical despite different names*

### Comparing `PythonToolsKit-1.2.4/PythonToolsKit/GetFile.py` & `PythonToolsKit-1.2.5/PythonToolsKit/GetFile.py`

 * *Files identical despite different names*

### Comparing `PythonToolsKit-1.2.4/PythonToolsKit/GetPass.py` & `PythonToolsKit-1.2.5/PythonToolsKit/GetPass.py`

 * *Files identical despite different names*

### Comparing `PythonToolsKit-1.2.4/PythonToolsKit/GetType.py` & `PythonToolsKit-1.2.5/PythonToolsKit/GetType.py`

 * *Files identical despite different names*

### Comparing `PythonToolsKit-1.2.4/PythonToolsKit/Import.py` & `PythonToolsKit-1.2.5/PythonToolsKit/Import.py`

 * *Files identical despite different names*

### Comparing `PythonToolsKit-1.2.4/PythonToolsKit/Json.py` & `PythonToolsKit-1.2.5/PythonToolsKit/Json.py`

 * *Files identical despite different names*

### Comparing `PythonToolsKit-1.2.4/PythonToolsKit/List.py` & `PythonToolsKit-1.2.5/PythonToolsKit/List.py`

 * *Files identical despite different names*

### Comparing `PythonToolsKit-1.2.4/PythonToolsKit/Logs.py` & `PythonToolsKit-1.2.5/PythonToolsKit/Logs.py`

 * *Files identical despite different names*

### Comparing `PythonToolsKit-1.2.4/PythonToolsKit/OrdDict.py` & `PythonToolsKit-1.2.5/PythonToolsKit/OrdDict.py`

 * *Files identical despite different names*

### Comparing `PythonToolsKit-1.2.4/PythonToolsKit/PrintF.py` & `PythonToolsKit-1.2.5/PythonToolsKit/PrintF.py`

 * *Files identical despite different names*

### Comparing `PythonToolsKit-1.2.4/PythonToolsKit/Process.py` & `PythonToolsKit-1.2.5/PythonToolsKit/Process.py`

 * *Files identical despite different names*

### Comparing `PythonToolsKit-1.2.4/PythonToolsKit/Random.py` & `PythonToolsKit-1.2.5/PythonToolsKit/Random.py`

 * *Files identical despite different names*

### Comparing `PythonToolsKit-1.2.4/PythonToolsKit/RecursionDebug.py` & `PythonToolsKit-1.2.5/PythonToolsKit/RecursionDebug.py`

 * *Files identical despite different names*

### Comparing `PythonToolsKit-1.2.4/PythonToolsKit/Report.py` & `PythonToolsKit-1.2.5/PythonToolsKit/Report.py`

 * *Files identical despite different names*

### Comparing `PythonToolsKit-1.2.4/PythonToolsKit/ScapyTools.py` & `PythonToolsKit-1.2.5/PythonToolsKit/ScapyTools.py`

 * *Files identical despite different names*

### Comparing `PythonToolsKit-1.2.4/PythonToolsKit/StringF.py` & `PythonToolsKit-1.2.5/PythonToolsKit/StringF.py`

 * *Files identical despite different names*

### Comparing `PythonToolsKit-1.2.4/PythonToolsKit/Terminal.py` & `PythonToolsKit-1.2.5/PythonToolsKit/Terminal.py`

 * *Files identical despite different names*

### Comparing `PythonToolsKit-1.2.4/PythonToolsKit/TestArguments.py` & `PythonToolsKit-1.2.5/PythonToolsKit/TestArguments.py`

 * *Files identical despite different names*

### Comparing `PythonToolsKit-1.2.4/PythonToolsKit/TestTimeout.py` & `PythonToolsKit-1.2.5/PythonToolsKit/TestTimeout.py`

 * *Files identical despite different names*

### Comparing `PythonToolsKit-1.2.4/PythonToolsKit/Thread.py` & `PythonToolsKit-1.2.5/PythonToolsKit/Thread.py`

 * *Files identical despite different names*

### Comparing `PythonToolsKit-1.2.4/PythonToolsKit/Timeout.py` & `PythonToolsKit-1.2.5/PythonToolsKit/Timeout.py`

 * *Files identical despite different names*

### Comparing `PythonToolsKit-1.2.4/PythonToolsKit/Tuple.py` & `PythonToolsKit-1.2.5/PythonToolsKit/Tuple.py`

 * *Files identical despite different names*

### Comparing `PythonToolsKit-1.2.4/PythonToolsKit/WindowsTerminal.py` & `PythonToolsKit-1.2.5/PythonToolsKit/WindowsTerminal.py`

 * *Files identical despite different names*

### Comparing `PythonToolsKit-1.2.4/PythonToolsKit/__init__.py` & `PythonToolsKit-1.2.5/PythonToolsKit/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 #    along with this program.  If not, see <https://www.gnu.org/licenses/>.
 ###################
 
 """
 This package implements tools to build python package and tools.
 """
 
-__version__ = "1.2.4"
+__version__ = "1.2.5"
 __author__ = "Maurice Lambert"
 __author_email__ = "mauricelambert434@gmail.com"
 __maintainer__ = "Maurice Lambert"
 __maintainer_email__ = "mauricelambert434@gmail.com"
 __description__ = """
 This package implements tools to build python package and tools.
 """
```

### Comparing `PythonToolsKit-1.2.4/PythonToolsKit/urlopen.py` & `PythonToolsKit-1.2.5/PythonToolsKit/urlopen.py`

 * *Files identical despite different names*

### Comparing `PythonToolsKit-1.2.4/PythonToolsKit.egg-info/PKG-INFO` & `PythonToolsKit-1.2.5/PythonToolsKit.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PythonToolsKit
-Version: 1.2.4
+Version: 1.2.5
 Summary: This package implements tools to build python package and tools.
 Home-page: https://github.com/mauricelambert/PythonToolsKit
 Author: Maurice Lambert
 Author-email: mauricelambert434@gmail.com
 Maintainer: Maurice Lambert
 Maintainer-email: mauricelambert434@gmail.com
 License: GPL-3.0 License
```

### Comparing `PythonToolsKit-1.2.4/PythonToolsKit.egg-info/SOURCES.txt` & `PythonToolsKit-1.2.5/PythonToolsKit.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `PythonToolsKit-1.2.4/README.md` & `PythonToolsKit-1.2.5/README.md`

 * *Files identical despite different names*

### Comparing `PythonToolsKit-1.2.4/setup.py` & `PythonToolsKit-1.2.5/setup.py`

 * *Files identical despite different names*

