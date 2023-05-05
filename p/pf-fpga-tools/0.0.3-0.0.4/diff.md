# Comparing `tmp/pf_fpga_tools-0.0.3.tar.gz` & `tmp/pf_fpga_tools-0.0.4.tar.gz`

## Comparing `pf_fpga_tools-0.0.3.tar` & `pf_fpga_tools-0.0.4.tar`

### file list

```diff
@@ -1,20 +1,20 @@
--rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 pf_fpga_tools-0.0.3/.flake8
--rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 pf_fpga_tools-0.0.3/pffpgatools/__about__.py
--rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 pf_fpga_tools-0.0.3/pffpgatools/__init__.py
--rw-r--r--   0        0        0      331 2020-02-02 00:00:00.000000 pf_fpga_tools-0.0.3/pffpgatools/exceptions.py
--rw-r--r--   0        0        0     1621 2020-02-02 00:00:00.000000 pf_fpga_tools-0.0.3/pffpgatools/utils.py
--rwxr-xr-x   0        0        0      916 2020-02-02 00:00:00.000000 pf_fpga_tools-0.0.3/pffpgatools/pfBuildCore/__main__.py
--rw-r--r--   0        0        0    14660 2020-02-02 00:00:00.000000 pf_fpga_tools-0.0.3/pffpgatools/pfBuildCore/pfBuildCore.py
--rwxr-xr-x   0        0        0      940 2020-02-02 00:00:00.000000 pf_fpga_tools-0.0.3/pffpgatools/pfCloneCoreTemplate/__main__.py
--rw-r--r--   0        0        0     3135 2020-02-02 00:00:00.000000 pf_fpga_tools-0.0.3/pffpgatools/pfCloneCoreTemplate/pfCloneCoreTemplate.py
--rwxr-xr-x   0        0        0      925 2020-02-02 00:00:00.000000 pf_fpga_tools-0.0.3/pffpgatools/pfConvertImage/__main__.py
--rw-r--r--   0        0        0     4479 2020-02-02 00:00:00.000000 pf_fpga_tools-0.0.3/pffpgatools/pfConvertImage/pfConvertImage.py
--rwxr-xr-x   0        0        0      922 2020-02-02 00:00:00.000000 pf_fpga_tools-0.0.3/pffpgatools/pfInstallCore/__main__.py
--rw-r--r--   0        0        0     4909 2020-02-02 00:00:00.000000 pf_fpga_tools-0.0.3/pffpgatools/pfInstallCore/pfInstallCore.py
--rwxr-xr-x   0        0        0      937 2020-02-02 00:00:00.000000 pf_fpga_tools-0.0.3/pffpgatools/pfReverseBitstream/__main__.py
--rw-r--r--   0        0        0     3316 2020-02-02 00:00:00.000000 pf_fpga_tools-0.0.3/pffpgatools/pfReverseBitstream/pfReverseBitstream.py
--rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 pf_fpga_tools-0.0.3/.gitignore
--rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 pf_fpga_tools-0.0.3/LICENSE
--rw-r--r--   0        0        0     2040 2020-02-02 00:00:00.000000 pf_fpga_tools-0.0.3/README.md
--rw-r--r--   0        0        0     1755 2020-02-02 00:00:00.000000 pf_fpga_tools-0.0.3/pyproject.toml
--rw-r--r--   0        0        0     3191 2020-02-02 00:00:00.000000 pf_fpga_tools-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0       73 2020-02-02 00:00:00.000000 pf_fpga_tools-0.0.4/.flake8
+-rw-r--r--   0        0        0      148 2020-02-02 00:00:00.000000 pf_fpga_tools-0.0.4/pffpgatools/__about__.py
+-rw-r--r--   0        0        0      102 2020-02-02 00:00:00.000000 pf_fpga_tools-0.0.4/pffpgatools/__init__.py
+-rw-r--r--   0        0        0      331 2020-02-02 00:00:00.000000 pf_fpga_tools-0.0.4/pffpgatools/exceptions.py
+-rw-r--r--   0        0        0     1621 2020-02-02 00:00:00.000000 pf_fpga_tools-0.0.4/pffpgatools/utils.py
+-rwxr-xr-x   0        0        0      916 2020-02-02 00:00:00.000000 pf_fpga_tools-0.0.4/pffpgatools/pfBuildCore/__main__.py
+-rw-r--r--   0        0        0    14660 2020-02-02 00:00:00.000000 pf_fpga_tools-0.0.4/pffpgatools/pfBuildCore/pfBuildCore.py
+-rwxr-xr-x   0        0        0      940 2020-02-02 00:00:00.000000 pf_fpga_tools-0.0.4/pffpgatools/pfCloneCoreTemplate/__main__.py
+-rw-r--r--   0        0        0     3732 2020-02-02 00:00:00.000000 pf_fpga_tools-0.0.4/pffpgatools/pfCloneCoreTemplate/pfCloneCoreTemplate.py
+-rwxr-xr-x   0        0        0      925 2020-02-02 00:00:00.000000 pf_fpga_tools-0.0.4/pffpgatools/pfConvertImage/__main__.py
+-rw-r--r--   0        0        0     4479 2020-02-02 00:00:00.000000 pf_fpga_tools-0.0.4/pffpgatools/pfConvertImage/pfConvertImage.py
+-rwxr-xr-x   0        0        0      922 2020-02-02 00:00:00.000000 pf_fpga_tools-0.0.4/pffpgatools/pfInstallCore/__main__.py
+-rw-r--r--   0        0        0     4909 2020-02-02 00:00:00.000000 pf_fpga_tools-0.0.4/pffpgatools/pfInstallCore/pfInstallCore.py
+-rwxr-xr-x   0        0        0      937 2020-02-02 00:00:00.000000 pf_fpga_tools-0.0.4/pffpgatools/pfReverseBitstream/__main__.py
+-rw-r--r--   0        0        0     3316 2020-02-02 00:00:00.000000 pf_fpga_tools-0.0.4/pffpgatools/pfReverseBitstream/pfReverseBitstream.py
+-rw-r--r--   0        0        0       60 2020-02-02 00:00:00.000000 pf_fpga_tools-0.0.4/.gitignore
+-rw-r--r--   0        0        0    35149 2020-02-02 00:00:00.000000 pf_fpga_tools-0.0.4/LICENSE
+-rw-r--r--   0        0        0     2040 2020-02-02 00:00:00.000000 pf_fpga_tools-0.0.4/README.md
+-rw-r--r--   0        0        0     1755 2020-02-02 00:00:00.000000 pf_fpga_tools-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0     3191 2020-02-02 00:00:00.000000 pf_fpga_tools-0.0.4/PKG-INFO
```

### Comparing `pf_fpga_tools-0.0.3/pffpgatools/utils.py` & `pf_fpga_tools-0.0.4/pffpgatools/utils.py`

 * *Files identical despite different names*

### Comparing `pf_fpga_tools-0.0.3/pffpgatools/pfBuildCore/__main__.py` & `pf_fpga_tools-0.0.4/pffpgatools/pfBuildCore/__main__.py`

 * *Files identical despite different names*

### Comparing `pf_fpga_tools-0.0.3/pffpgatools/pfBuildCore/pfBuildCore.py` & `pf_fpga_tools-0.0.4/pffpgatools/pfBuildCore/pfBuildCore.py`

 * *Files identical despite different names*

### Comparing `pf_fpga_tools-0.0.3/pffpgatools/pfCloneCoreTemplate/__main__.py` & `pf_fpga_tools-0.0.4/pffpgatools/pfCloneCoreTemplate/__main__.py`

 * *Files identical despite different names*

### Comparing `pf_fpga_tools-0.0.3/pffpgatools/pfCloneCoreTemplate/pfCloneCoreTemplate.py` & `pf_fpga_tools-0.0.4/pffpgatools/pfCloneCoreTemplate/pfCloneCoreTemplate.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,48 +1,56 @@
 # SPDX-FileCopyrightText: 2023-present Didier Malenfant
 #
 # SPDX-License-Identifier: GPL-3.0-or-later
 
 import os
 import sys
 import getopt
-import zipfile
-import tempfile
 import shutil
 
 from pffpgatools.__about__ import __version__
 from pffpgatools.utils import Utils
+from pffpgatools.exceptions import ArgumentError
 
 
 # -- Classes
 class pfCloneCoreTemplate:
     """A tool to clone the Github core template."""
 
     def __init__(self, args):
         """Constructor based on command line arguments."""
 
         try:
             self.branch_name = None
+            self.tag_name = None
 
             # -- Gather the arguments
-            opts, arguments = getopt.getopt(args, 'hvb:', ['help', 'version', 'branch='])
+            opts, arguments = getopt.getopt(args, 'hvb:t:', ['help', 'version', 'branch=', 'tag='])
 
             for o, a in opts:
                 if o in ('-h', '--help'):
                     pfCloneCoreTemplate.printUsage()
                     sys.exit(0)
                 elif o in ('-v', '--version'):
                     pfCloneCoreTemplate.printVersion()
                     sys.exit(0)
                 elif o in ('-b', '--branch'):
+                    if self.tag_name is not None:
+                        raise ArgumentError('Cannot specificy both a branch and a tag on the command line.')
+
                     self.branch_name = a
+                elif o in ('-t', '--tag'):
+                    if self.branch_name is not None:
+                        raise ArgumentError('Cannot specificy both a branch and a tag on the command line.')
+
+                    self.tag_name = a
 
             nb_of_arguments: int = len(arguments)
             if nb_of_arguments != 1:
-                raise RuntimeError('Invalid arguments. Maybe start with `pfCloneCoreTemplate --help?')
+                raise ArgumentError('Invalid arguments. Maybe start with `pfCloneCoreTemplate --help?')
 
             self.destination_folder: str = arguments[0]
 
         except getopt.GetoptError:
             print('Unknown option or argument. Maybe start with `pfCloneCoreTemplate --help?')
             sys.exit(0)
 
@@ -57,14 +65,17 @@
         print('Cloning core template in \'' + repo_folder + '\'.')
 
         command_line = ['git', 'clone', '--depth', '1']
 
         if self.branch_name is not None:
             command_line.append('--branch')
             command_line.append(self.branch_name)
+        elif self.tag_name is not None:
+            command_line.append('--branch')
+            command_line.append(self.tag_name)
 
         command_line.append('https://github.com/DidierMalenfant/pf-core-template.git')
 
         Utils.shellCommand(command_line, from_dir=self.destination_folder, silent_mode=True)
 
     @classmethod
     def printUsage(cls) -> None:
```

### Comparing `pf_fpga_tools-0.0.3/pffpgatools/pfConvertImage/__main__.py` & `pf_fpga_tools-0.0.4/pffpgatools/pfConvertImage/__main__.py`

 * *Files identical despite different names*

### Comparing `pf_fpga_tools-0.0.3/pffpgatools/pfConvertImage/pfConvertImage.py` & `pf_fpga_tools-0.0.4/pffpgatools/pfConvertImage/pfConvertImage.py`

 * *Files identical despite different names*

### Comparing `pf_fpga_tools-0.0.3/pffpgatools/pfInstallCore/__main__.py` & `pf_fpga_tools-0.0.4/pffpgatools/pfInstallCore/__main__.py`

 * *Files identical despite different names*

### Comparing `pf_fpga_tools-0.0.3/pffpgatools/pfInstallCore/pfInstallCore.py` & `pf_fpga_tools-0.0.4/pffpgatools/pfInstallCore/pfInstallCore.py`

 * *Files identical despite different names*

### Comparing `pf_fpga_tools-0.0.3/pffpgatools/pfReverseBitstream/__main__.py` & `pf_fpga_tools-0.0.4/pffpgatools/pfReverseBitstream/__main__.py`

 * *Files identical despite different names*

### Comparing `pf_fpga_tools-0.0.3/pffpgatools/pfReverseBitstream/pfReverseBitstream.py` & `pf_fpga_tools-0.0.4/pffpgatools/pfReverseBitstream/pfReverseBitstream.py`

 * *Files identical despite different names*

### Comparing `pf_fpga_tools-0.0.3/LICENSE` & `pf_fpga_tools-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `pf_fpga_tools-0.0.3/README.md` & `pf_fpga_tools-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `pf_fpga_tools-0.0.3/pyproject.toml` & `pf_fpga_tools-0.0.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `pf_fpga_tools-0.0.3/PKG-INFO` & `pf_fpga_tools-0.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pf-fpga-tools
-Version: 0.0.3
+Version: 0.0.4
 Summary: A collection of tools for openFPGA projects
 Project-URL: Homepage, https://didier.malenfant.net/ProjectFreedom/
 Project-URL: Documentation, https://github.com/DidierMalenfant/pf-fpga-tools#readme
 Project-URL: Bug Tracker, https://github.com/DidierMalenfant/pf-fpga-tools/issues
 Project-URL: Source Code, https://github.com/DidierMalenfant/pf-fpga-tools
 Author-email: Didier Malenfant <coding@malenfant.net>
 License-Expression: GPL-3.0-or-later
```

