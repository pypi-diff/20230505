# Comparing `tmp/auditd-python-parser-0.0.8.tar.gz` & `tmp/auditd-python-parser-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "auditd-python-parser-0.0.8.tar", last modified: Fri Mar 31 08:03:28 2023, max compression
+gzip compressed data, was "auditd-python-parser-0.0.9.tar", last modified: Fri May  5 07:28:21 2023, max compression
```

## Comparing `auditd-python-parser-0.0.8.tar` & `auditd-python-parser-0.0.9.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxrwxrwx   0        0        0        0 2023-03-31 08:03:28.640742 auditd-python-parser-0.0.8/
--rw-rw-rw-   0        0        0    35823 2023-03-30 15:22:12.000000 auditd-python-parser-0.0.8/LICENSE
--rw-rw-rw-   0        0        0    37201 2023-03-31 08:03:28.641739 auditd-python-parser-0.0.8/PKG-INFO
--rw-rw-rw-   0        0        0      979 2023-03-30 16:55:54.000000 auditd-python-parser-0.0.8/README.rst
--rw-rw-rw-   0        0        0      747 2023-03-31 07:14:35.000000 auditd-python-parser-0.0.8/README_pypi.md
-drwxrwxrwx   0        0        0        0 2023-03-31 08:03:28.634758 auditd-python-parser-0.0.8/auditd_python_parser.egg-info/
--rw-rw-rw-   0        0        0    37201 2023-03-31 08:03:28.000000 auditd-python-parser-0.0.8/auditd_python_parser.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      343 2023-03-31 08:03:28.000000 auditd-python-parser-0.0.8/auditd_python_parser.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-31 08:03:28.000000 auditd-python-parser-0.0.8/auditd_python_parser.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       14 2023-03-31 08:03:28.000000 auditd-python-parser-0.0.8/auditd_python_parser.egg-info/requires.txt
--rw-rw-rw-   0        0        0       19 2023-03-31 08:03:28.000000 auditd-python-parser-0.0.8/auditd_python_parser.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-03-31 08:03:28.638747 auditd-python-parser-0.0.8/auditdpythonparser/
--rw-rw-rw-   0        0        0       35 2023-03-31 07:33:51.000000 auditd-python-parser-0.0.8/auditdpythonparser/__init__.py
--rw-rw-rw-   0        0        0    20410 2023-03-30 16:38:06.000000 auditd-python-parser-0.0.8/auditdpythonparser/auditdparser.py
--rw-rw-rw-   0        0        0      101 2023-03-31 07:58:28.000000 auditd-python-parser-0.0.8/pyproject.toml
--rw-rw-rw-   0        0        0      774 2023-03-31 08:03:28.643734 auditd-python-parser-0.0.8/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-05 07:28:21.311965 auditd-python-parser-0.0.9/
+-rw-rw-rw-   0        0        0    35823 2023-03-30 15:22:12.000000 auditd-python-parser-0.0.9/LICENSE
+-rw-rw-rw-   0        0        0    37511 2023-05-05 07:28:21.312963 auditd-python-parser-0.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0     1808 2023-05-05 07:27:10.000000 auditd-python-parser-0.0.9/README.rst
+-rw-rw-rw-   0        0        0     1057 2023-05-05 07:27:22.000000 auditd-python-parser-0.0.9/README_pypi.md
+drwxrwxrwx   0        0        0        0 2023-05-05 07:28:21.301993 auditd-python-parser-0.0.9/auditd_python_parser.egg-info/
+-rw-rw-rw-   0        0        0    37511 2023-05-05 07:28:21.000000 auditd-python-parser-0.0.9/auditd_python_parser.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      343 2023-05-05 07:28:21.000000 auditd-python-parser-0.0.9/auditd_python_parser.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-05 07:28:21.000000 auditd-python-parser-0.0.9/auditd_python_parser.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       14 2023-05-05 07:28:21.000000 auditd-python-parser-0.0.9/auditd_python_parser.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       19 2023-05-05 07:28:21.000000 auditd-python-parser-0.0.9/auditd_python_parser.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-05 07:28:21.310969 auditd-python-parser-0.0.9/auditdpythonparser/
+-rw-rw-rw-   0        0        0       35 2023-03-31 07:33:51.000000 auditd-python-parser-0.0.9/auditdpythonparser/__init__.py
+-rw-rw-rw-   0        0        0    30661 2023-05-05 07:14:56.000000 auditd-python-parser-0.0.9/auditdpythonparser/auditdparser.py
+-rw-rw-rw-   0        0        0      101 2023-03-31 07:58:28.000000 auditd-python-parser-0.0.9/pyproject.toml
+-rw-rw-rw-   0        0        0      774 2023-05-05 07:28:21.314958 auditd-python-parser-0.0.9/setup.cfg
```

### Comparing `auditd-python-parser-0.0.8/LICENSE` & `auditd-python-parser-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `auditd-python-parser-0.0.8/PKG-INFO` & `auditd-python-parser-0.0.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,38 @@
 Metadata-Version: 2.1
 Name: auditd-python-parser
-Version: 0.0.8
+Version: 0.0.9
 Summary: A python package to parse & process raw auditd.log files
 Home-page: https://github.com/exeronn/auditd-python-parser
 Author: exeron
 Project-URL: Bug Tracker, https://github.com/exeronn/auditd-python-parser/issues
 Project-URL: repository, https://github.com/exeronn/auditd-python-parser
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-An in development python library to parse raw auditd events generated on a linux system. This is done only using the auditd.log* files and doesn't require the use of ausearch or similar. The logs can also be parsed on a Windows system.
+An in development python library to parse raw auditd events generated on a linux system. This is done only using the audit.log* files and doesn't require the use of ausearch or similar. The logs can also be parsed on a Windows system.
 
 The library tries to keep to the key fields for each event type and generates additional fields to enable process ancestry (process GUIDs) and event linkage similar to how SysmonForLinux does. Some events are enriched where possible such as the network events by adding the process commandline to the network connection where possible.
 
-To use you call parsedata(data) from it which will return the values. Currently it returns dfprocessevents, dfnetworkevents. See the Github project for example code.
-
+To use you call parsedata(data) from it which will return the values. Currently it returns process, network, filecreate & file open. See the Github project for example code.
 
+import auditdpythonparser 
+f = open("audit.log", "r")
+rawdata = f.read()
+f.close()   
+results = auditdpythonparser.parsedata(rawdata)
+
+dfprocessevents = results["process"]
+dfnetworkevents = results["network"]
+dffilecreateevents = results["filecreate"]
+dffileopenatevents = results["fileopenat"]
                     GNU GENERAL PUBLIC LICENSE
                        Version 3, 29 June 2007
 
  Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
  Everyone is permitted to copy and distribute verbatim copies
  of this license document, but changing it is not allowed.
```

### Comparing `auditd-python-parser-0.0.8/README.rst` & `auditd-python-parser-0.0.9/README_pypi.md`

 * *Files 19% similar despite different names*

```diff
@@ -1,16 +1,16 @@
-auditd-python-parser
-========
-
-An in development python library to parse raw auditd events generated on a linux system. This is done only using the auditd.log* files and doesn't require the use of ausearch or similar. The logs can also be parsed on a Windows system.
+An in development python library to parse raw auditd events generated on a linux system. This is done only using the audit.log* files and doesn't require the use of ausearch or similar. The logs can also be parsed on a Windows system.
 
 The library tries to keep to the key fields for each event type and generates additional fields to enable process ancestry (process GUIDs) and event linkage similar to how SysmonForLinux does. Some events are enriched where possible such as the network events by adding the process commandline to the network connection where possible.
 
-To use you import the library in the src folder and then call parsedata(data) from it which will return the values. Currently it returns dfprocessevents, dfnetworkevents.
+To use you call parsedata(data) from it which will return the values. Currently it returns process, network, filecreate & file open. See the Github project for example code.
 
-.. code:: python
+import auditdpythonparser 
+f = open("audit.log", "r")
+rawdata = f.read()
+f.close()   
+results = auditdpythonparser.parsedata(rawdata)
 
-    import auditdparser 
-    f = open("auditd.log", "r")
-    rawdata = f.read()
-    f.close()   
-    dfprocessevents, dfnetworkevents = auditdparser.parsedata(rawdata)
+dfprocessevents = results["process"]
+dfnetworkevents = results["network"]
+dffilecreateevents = results["filecreate"]
+dffileopenatevents = results["fileopenat"]
```

### Comparing `auditd-python-parser-0.0.8/auditd_python_parser.egg-info/PKG-INFO` & `auditd-python-parser-0.0.9/auditd_python_parser.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,29 +1,38 @@
 Metadata-Version: 2.1
 Name: auditd-python-parser
-Version: 0.0.8
+Version: 0.0.9
 Summary: A python package to parse & process raw auditd.log files
 Home-page: https://github.com/exeronn/auditd-python-parser
 Author: exeron
 Project-URL: Bug Tracker, https://github.com/exeronn/auditd-python-parser/issues
 Project-URL: repository, https://github.com/exeronn/auditd-python-parser
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
-An in development python library to parse raw auditd events generated on a linux system. This is done only using the auditd.log* files and doesn't require the use of ausearch or similar. The logs can also be parsed on a Windows system.
+An in development python library to parse raw auditd events generated on a linux system. This is done only using the audit.log* files and doesn't require the use of ausearch or similar. The logs can also be parsed on a Windows system.
 
 The library tries to keep to the key fields for each event type and generates additional fields to enable process ancestry (process GUIDs) and event linkage similar to how SysmonForLinux does. Some events are enriched where possible such as the network events by adding the process commandline to the network connection where possible.
 
-To use you call parsedata(data) from it which will return the values. Currently it returns dfprocessevents, dfnetworkevents. See the Github project for example code.
-
+To use you call parsedata(data) from it which will return the values. Currently it returns process, network, filecreate & file open. See the Github project for example code.
 
+import auditdpythonparser 
+f = open("audit.log", "r")
+rawdata = f.read()
+f.close()   
+results = auditdpythonparser.parsedata(rawdata)
+
+dfprocessevents = results["process"]
+dfnetworkevents = results["network"]
+dffilecreateevents = results["filecreate"]
+dffileopenatevents = results["fileopenat"]
                     GNU GENERAL PUBLIC LICENSE
                        Version 3, 29 June 2007
 
  Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
  Everyone is permitted to copy and distribute verbatim copies
  of this license document, but changing it is not allowed.
```

### Comparing `auditd-python-parser-0.0.8/setup.cfg` & `auditd-python-parser-0.0.9/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2061 7564 6974 642d 7079 7468 6f6e   = auditd-python
 00000020: 2d70 6172 7365 720d 0a76 6572 7369 6f6e  -parser..version
-00000030: 203d 2030 2e30 2e38 0d0a 6175 7468 6f72   = 0.0.8..author
+00000030: 203d 2030 2e30 2e39 0d0a 6175 7468 6f72   = 0.0.9..author
 00000040: 203d 2065 7865 726f 6e0d 0a64 6573 6372   = exeron..descr
 00000050: 6970 7469 6f6e 203d 2041 2070 7974 686f  iption = A pytho
 00000060: 6e20 7061 636b 6167 6520 746f 2070 6172  n package to par
 00000070: 7365 2026 2070 726f 6365 7373 2072 6177  se & process raw
 00000080: 2061 7564 6974 642e 6c6f 6720 6669 6c65   auditd.log file
 00000090: 730d 0a6c 6f6e 675f 6465 7363 7269 7074  s..long_descript
 000000a0: 696f 6e20 3d20 6669 6c65 3a20 5245 4144  ion = file: READ
```

