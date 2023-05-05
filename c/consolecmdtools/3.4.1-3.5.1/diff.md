# Comparing `tmp/consolecmdtools-3.4.1.tar.gz` & `tmp/consolecmdtools-3.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "consolecmdtools-3.4.1.tar", last modified: Thu Dec 15 11:33:54 2022, max compression
+gzip compressed data, was "consolecmdtools-3.5.1.tar", last modified: Fri May  5 03:42:19 2023, max compression
```

## Comparing `consolecmdtools-3.4.1.tar` & `consolecmdtools-3.5.1.tar`

### file list

```diff
@@ -1,15 +1,18 @@
-drwxrwxrwx   0        0        0        0 2022-12-15 11:33:54.316894 consolecmdtools-3.4.1/
--rw-rw-rw-   0        0        0     1082 2022-12-15 10:24:01.000000 consolecmdtools-3.4.1/LICENSE
--rw-rw-rw-   0        0        0     5919 2022-12-15 11:33:54.316894 consolecmdtools-3.4.1/PKG-INFO
--rw-rw-rw-   0        0        0     5044 2022-12-15 11:23:24.000000 consolecmdtools-3.4.1/README.md
-drwxrwxrwx   0        0        0        0 2022-12-15 11:33:54.291803 consolecmdtools-3.4.1/consolecmdtools/
--rw-rw-rw-   0        0        0    14469 2022-12-15 11:31:49.000000 consolecmdtools-3.4.1/consolecmdtools/__init__.py
--rw-rw-rw-   0        0        0     2088 2022-12-15 11:28:48.000000 consolecmdtools-3.4.1/consolecmdtools/__main__.py
-drwxrwxrwx   0        0        0        0 2022-12-15 11:33:54.315451 consolecmdtools-3.4.1/consolecmdtools.egg-info/
--rw-rw-rw-   0        0        0     5919 2022-12-15 11:33:54.000000 consolecmdtools-3.4.1/consolecmdtools.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      282 2022-12-15 11:33:54.000000 consolecmdtools-3.4.1/consolecmdtools.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-12-15 11:33:54.000000 consolecmdtools-3.4.1/consolecmdtools.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       60 2022-12-15 11:33:54.000000 consolecmdtools-3.4.1/consolecmdtools.egg-info/requires.txt
--rw-rw-rw-   0        0        0       21 2022-12-15 11:33:54.000000 consolecmdtools-3.4.1/consolecmdtools.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1273 2022-12-15 11:02:11.000000 consolecmdtools-3.4.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2022-12-15 11:33:54.316894 consolecmdtools-3.4.1/setup.cfg
+drwxr-xr-x   0 kyan001    (501) staff       (20)        0 2023-05-05 03:42:19.133686 consolecmdtools-3.5.1/
+-rw-r--r--   0 kyan001    (501) staff       (20)     1061 2020-11-09 08:36:27.000000 consolecmdtools-3.5.1/LICENSE
+-rw-r--r--   0 kyan001    (501) staff       (20)     7368 2023-05-05 03:42:19.133023 consolecmdtools-3.5.1/PKG-INFO
+-rw-r--r--   0 kyan001    (501) staff       (20)     5293 2023-05-05 03:39:04.000000 consolecmdtools-3.5.1/README.md
+drwxr-xr-x   0 kyan001    (501) staff       (20)        0 2023-05-05 03:42:19.123893 consolecmdtools-3.5.1/consolecmdtools/
+-rw-r--r--   0 kyan001    (501) staff       (20)    15613 2023-05-05 03:39:04.000000 consolecmdtools-3.5.1/consolecmdtools/__init__.py
+-rw-r--r--   0 kyan001    (501) staff       (20)     2037 2022-12-25 10:04:52.000000 consolecmdtools-3.5.1/consolecmdtools/__main__.py
+drwxr-xr-x   0 kyan001    (501) staff       (20)        0 2023-05-05 03:42:19.128894 consolecmdtools-3.5.1/consolecmdtools.egg-info/
+-rw-r--r--   0 kyan001    (501) staff       (20)     7368 2023-05-05 03:42:19.000000 consolecmdtools-3.5.1/consolecmdtools.egg-info/PKG-INFO
+-rw-r--r--   0 kyan001    (501) staff       (20)      332 2023-05-05 03:42:19.000000 consolecmdtools-3.5.1/consolecmdtools.egg-info/SOURCES.txt
+-rw-r--r--   0 kyan001    (501) staff       (20)        1 2023-05-05 03:42:19.000000 consolecmdtools-3.5.1/consolecmdtools.egg-info/dependency_links.txt
+-rw-r--r--   0 kyan001    (501) staff       (20)       60 2023-05-05 03:42:19.000000 consolecmdtools-3.5.1/consolecmdtools.egg-info/requires.txt
+-rw-r--r--   0 kyan001    (501) staff       (20)       21 2023-05-05 03:42:19.000000 consolecmdtools-3.5.1/consolecmdtools.egg-info/top_level.txt
+-rw-r--r--   0 kyan001    (501) staff       (20)     1230 2022-12-25 10:04:52.000000 consolecmdtools-3.5.1/pyproject.toml
+-rw-r--r--   0 kyan001    (501) staff       (20)       38 2023-05-05 03:42:19.133893 consolecmdtools-3.5.1/setup.cfg
+drwxr-xr-x   0 kyan001    (501) staff       (20)        0 2023-05-05 03:42:19.131688 consolecmdtools-3.5.1/tests/
+-rw-r--r--   0 kyan001    (501) staff       (20)    12262 2023-05-05 03:39:04.000000 consolecmdtools-3.5.1/tests/test_consolecmdtools.py
+-rw-r--r--   0 kyan001    (501) staff       (20)      363 2021-03-01 08:05:34.000000 consolecmdtools-3.5.1/tests/test_runas.py
```

### Comparing `consolecmdtools-3.4.1/LICENSE` & `consolecmdtools-3.5.1/LICENSE`

 * *Ordering differences only*

 * *Files 18% similar despite different names*

```diff
@@ -1,21 +1,21 @@
-MIT License
-
-Copyright (c) 2020 Kyan
-
-Permission is hereby granted, free of charge, to any person obtaining a copy
-of this software and associated documentation files (the "Software"), to deal
-in the Software without restriction, including without limitation the rights
-to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
-copies of the Software, and to permit persons to whom the Software is
-furnished to do so, subject to the following conditions:
-
-The above copyright notice and this permission notice shall be included in all
-copies or substantial portions of the Software.
-
-THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
-IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
-FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
-AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
-LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
-OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
-SOFTWARE.
+MIT License
+
+Copyright (c) 2020 Kyan
+
+Permission is hereby granted, free of charge, to any person obtaining a copy
+of this software and associated documentation files (the "Software"), to deal
+in the Software without restriction, including without limitation the rights
+to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+copies of the Software, and to permit persons to whom the Software is
+furnished to do so, subject to the following conditions:
+
+The above copyright notice and this permission notice shall be included in all
+copies or substantial portions of the Software.
+
+THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+SOFTWARE.
```

### Comparing `consolecmdtools-3.4.1/PKG-INFO` & `consolecmdtools-3.5.1/README.md`

 * *Files 20% similar despite different names*

```diff
@@ -1,186 +1,172 @@
-Metadata-Version: 2.1
-Name: consolecmdtools
-Version: 3.4.1
-Summary: Console command tools in Python
-Author-email: Kyan <kai@kyan001.com>
-License: LICENSE
-Project-URL: Homepage, https://github.com/kyan001/PyConsoleCMDTools
-Project-URL: Issue Tracker, https://github.com/kyan001/PyConsoleCMDTools/issues
-Project-URL: Source Code, https://github.com/kyan001/PyConsoleCMDTools
-Keywords: python,console,command,tool
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Intended Audience :: Developers
-Classifier: Topic :: Software Development :: User Interfaces
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3 :: Only
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-Provides-Extra: opt
-Provides-Extra: dev
-License-File: LICENSE
-
-# PyConsoleCMDTools
-![PyPI - Downloads](https://img.shields.io/pypi/dm/consolecmdtools)
-![GitHub release](https://img.shields.io/github/v/release/kyan001/PyConsoleCMDTools)
-[![GitHub license](https://img.shields.io/github/license/kyan001/PyConsoleCMDTools.svg)](https://github.com/kyan001/PyConsoleCMDTools/blob/master/LICENSE)
-
-## Installation
-
-```sh
-pip install consolecmdtools  # install
-pip install --upgrade consolecmdtools  # update
-python -m consolecmdtools  # examples
-```
-
-## Get Started
-
-```python
-import consolecmdtools as cct
-print(cct.__version__)
-```
-
-## Functions
-
-```python
->>> cct.banner("hello, world!")  # Generate banner for text
-#######################
-#    hello, world!    #
-#######################
-
->>> cct.md5("blah blah blah")  # Return md5 hash for text.
-'55e562bfee2bde4f9e71b8885eb5e303'
-
->>> cct.md5(42)  # Return md5 hash for number.
-'a1d0c6e83f027327d8461063f4ac58a6'
-
->>> cct.md5('file.txt')  # Return md5 hash for file.
-'d07aa6ddab4d6d2d2891aa9f3625a5db'
-
->>> cct.md5('file.txt', force_text=True)  # Force to return the md5 has for text, even the file exists.
-'3d8e577bddb17db339eae0b3d9bcf180'
-
->>> cct.crc32("blah blah blah")  # Return crc32 hash for text.
-753353432
-
->>> cct.crc32(42)  # Return crc32 hash for number.
-841265288
-
->>> cct.crc32('file.txt')  # Return crc32 hash for file.
-1030388931
-
->>> cct.crc32('file.txt', force_text=True)  # Force to return the md5 has for text, even the file exists.
-3774289445
-
->>> cct.main_color('image.jpg')  # Get theme color of image.
-(152, 156, 69)  # RGB value
-
->>> cct.main_color('http://image-url/image', is_url=True)  # Get theme color of web image.
-(152, 156, 69)  # RGB value
-
->>> cct.main_color('image.jpg', scale=500)  # Cost more time to generate a preciser color. default scale is 200.
-(152, 156, 69)
-
->>> cct.main_color('image.jpg', triplet='hex')  # Return color in hex triplet format. default mode is 'rgb'.
-'#989C45'
-
->>> cct.clear_screen()  # Clear the console.
-
->>> cct.get_py_cmd()  # Get python running command for different OS.
-'python3'
-
->>> cct.run_cmd("echo hello")  # Run console command. If the command failed, a warning message echoed. Returns bool.
-*
-| __RUN COMMAND__________________________
-| (Command) echo hello
-hello
-`
-
->>> cct.read_cmd("echo hello")  # Run a command and return the output.
-'hello\n'
-
->>> cct.is_cmd_exist("ls")  # Test if a command is exist.
-True
-
->>> cct.get_dir("./file")  # Get the parent folder path of the file.
-'/path/to/dir'  # '/path/to/dir/file' for example
-
->>> cct.get_dir("./file", mode="file")  # Get the file absolute path.
-'/path/to/dir/file'
-
->>> cct.get_dir("./file", mode="basename")  # Get the parent folder name of the file.
-'dir'
-
->>> cct.select_path()  # Show file dialog to get file path. Additional args pass to tkinter.filedialog.askopenfilename()
-'/path/to/dir/file'
-
->>> cct.select_path(multiple=True)  # Show file dialog to get multiple file paths.
-['/path/1', '/path/2']
-
->>> cct.select_path(folder=True)  # Show file dialog to get folder path.
-'/path/to/dir'
-
->>> cct.show_in_folder("/path/to/file")  # Show file in Explorer/Finder/Folder.
-
->>> cct.show_in_folder("/path/to/file", ask=True)  # Ask before show.
-
->>> cct.diff("str1", "str2")  # Compare 2 strings, return the list of diffs.
-[  # you can use `"\n".join(diff)` to print the diff.
-    "-str1",
-    "+str2"
-]
-
->>> cct.diff("str1", "str2", meta=True)  # show meta data in the first 3 lines.
-[
-    "--- <class 'str'>",
-    "+++ <class 'str'>",
-    "@@ -1 +1 @@",
-    "-str1",
-    "+str2"
-]
-
-
->>> cct.diff(["a", "b"], ["a", "b", "c"])  # Compare 2 lists and print diffs.
-[
-    "+c"
-]
-
->>> cct.diff(["a", "b"], ["a", "b", "c"], context=2)  # Show diffs with 2 extra context lines.
-[
-    " a",  # context line
-    " b",  # context line
-    "+c"  # diff
-]
-
->>> cct.diff("/path/to/file1", "/path/to/file2")  # Compare between 2 files.
-
->>> cct.diff("/path/to/file1", "str")  # Compare between file and str/list.
-
->>> cct.diff('str', 'str')  # If no diff, return [].
-[]
-
->>> cct.update_file('file', 'http://file-url')  # Update file if the file is not as same as url content.
-False  # if already up-to-date.
-
->>> cct.read_file('file')  # Read file using different encoding automatically.
-"file content"
-
->>> cct.ajax('http://ajax-url')  # Start a AJAX request.
-{'result': 'data'}  # As python dict.
-
->>> cct.ajax('http://ajax-url', {'data': 'value'})  # AJAX request with param.
-{'result': 'data'}
-
->>> cct.ajax('http://ajax-url', method='post')  # AJAX request using post. default is 'get'.
-{'result': 'data'}
-
->>> if not cct.is_admin():  # Check does the script has admin privileges.
-...     cct.runas_admin(__file__)  # run the script with admin privileges.
-... else:
-...     # your code here
-```
-
-## Updates
-* 2021-01-29 v3.0.0:
-    * Deprecated `image_to_color()`, add `main_color()`.
-        * use `main_color(..., is_url=True)` instead of `image_to_color(...)`
+# PyConsoleCMDTools
+![PyPI - Downloads](https://img.shields.io/pypi/dm/consolecmdtools)
+![GitHub release](https://img.shields.io/github/v/release/kyan001/PyConsoleCMDTools)
+[![GitHub license](https://img.shields.io/github/license/kyan001/PyConsoleCMDTools.svg)](https://github.com/kyan001/PyConsoleCMDTools/blob/master/LICENSE)
+
+## Installation
+
+```sh
+pip install consolecmdtools  # install
+pip install --upgrade consolecmdtools  # update
+python -m consolecmdtools  # examples
+```
+
+## Get Started
+
+```python
+import consolecmdtools as cct
+print(cct.__version__)
+```
+
+## Functions
+
+```python
+>>> cct.banner("hello, world!")  # Generate banner for text
+#######################
+#    hello, world!    #
+#######################
+
+>>> cct.md5("blah blah blah")  # Return md5 hash for text.
+'55e562bfee2bde4f9e71b8885eb5e303'
+
+>>> cct.md5(42)  # Return md5 hash for number.
+'a1d0c6e83f027327d8461063f4ac58a6'
+
+>>> cct.md5('file.txt')  # Return md5 hash for file.
+'d07aa6ddab4d6d2d2891aa9f3625a5db'
+
+>>> cct.md5('file.txt', force_text=True)  # Force to return the md5 has for text, even the file exists.
+'3d8e577bddb17db339eae0b3d9bcf180'
+
+>>> cct.crc32("blah blah blah")  # Return crc32 hash for text.
+753353432
+
+>>> cct.crc32(42)  # Return crc32 hash for number.
+841265288
+
+>>> cct.crc32('file.txt')  # Return crc32 hash for file.
+1030388931
+
+>>> cct.crc32('file.txt', force_text=True)  # Force to return the md5 has for text, even the file exists.
+3774289445
+
+>>> cct.main_color('image.jpg')  # Get theme color of image.
+(152, 156, 69)  # RGB value
+
+>>> cct.main_color('http://image-url/image', is_url=True)  # Get theme color of web image.
+(152, 156, 69)  # RGB value
+
+>>> cct.main_color('image.jpg', scale=500)  # Cost more time to generate a preciser color. default scale is 200.
+(152, 156, 69)
+
+>>> cct.main_color('image.jpg', triplet='hex')  # Return color in hex triplet format. default mode is 'rgb'.
+'#989C45'
+
+>>> cct.clear_screen()  # Clear the console.
+
+>>> cct.get_py_cmd()  # Get python running command for different OS.
+'python3'
+
+>>> cct.run_cmd("echo hello")  # Run console command. If the command failed, a warning message echoed. Returns bool.
+*
+| __RUN COMMAND__________________________
+| (Command) echo hello
+hello
+`
+
+>>> cct.read_cmd("echo hello")  # Run a command and return the output.
+'hello\n'
+
+>>> cct.is_cmd_exist("ls")  # Test if a command is exist.
+True
+
+>>> cct.get_dir("./file")  # Get the parent folder path of the file.
+'/path/to/dir'  # '/path/to/dir/file' for example
+
+>>> cct.get_dir("./file", mode="file")  # Get the file absolute path.
+'/path/to/dir/file'
+
+>>> cct.get_dir("./file", mode="basename")  # Get the parent folder name of the file.
+'dir'
+
+>>> cct.select_path()  # Show file dialog to get file path. Additional args pass to tkinter.filedialog.askopenfilename()
+'/path/to/dir/file'
+
+>>> cct.select_path(multiple=True)  # Show file dialog to get multiple file paths.
+['/path/1', '/path/2']
+
+>>> cct.select_path(folder=True)  # Show file dialog to get folder path.
+'/path/to/dir'
+
+>>> cct.show_in_folder("/path/to/file")  # Show file in Explorer/Finder/Folder.
+
+>>> cct.show_in_folder("/path/to/file", ask=True)  # Ask before show.
+
+>>> cct.diff("str1", "str2")  # Compare 2 strings, return the list of diffs.
+[  # you can use `"\n".join(diff)` to print the diff.
+    "-str1",
+    "+str2"
+]
+
+>>> cct.diff("str1", "str2", meta=True)  # show meta data in the first 3 lines.
+[
+    "--- <class 'str'>",
+    "+++ <class 'str'>",
+    "@@ -1 +1 @@",
+    "-str1",
+    "+str2"
+]
+
+
+>>> cct.diff(["a", "b"], ["a", "b", "c"])  # Compare 2 lists and print diffs.
+[
+    "+c"
+]
+
+>>> cct.diff(["a", "b"], ["a", "b", "c"], context=2)  # Show diffs with 2 extra context lines.
+[
+    " a",  # context line
+    " b",  # context line
+    "+c"  # diff
+]
+
+>>> cct.diff("/path/to/file1", "/path/to/file2")  # Compare between 2 files.
+
+>>> cct.diff("/path/to/file1", "str")  # Compare between file and str/list.
+
+>>> cct.diff('str', 'str')  # If no diff, return [].
+[]
+
+>>> cct.update_file('file', 'http://file-url')  # Update file if the file is not as same as url content.
+False  # if already up-to-date.
+
+>>> cct.read_file('file')  # Read file using different encoding automatically.
+"file content"
+
+>>> cct.move_file("/path/to/src", "/path/to/dst")  # Move file from src to dst, overwrite if dst already exists.
+
+>>> cct.move_file("/path/to/src", "/path/to/dst", copy=True)  # Copy file from src to dst.
+
+>>> cct.move_file("/path/to/src", "/path/to/dst", backup=True)  # Backup dst file before move or copy.
+
+>>> cct.move_file("/path/to/src", "/path/to/dst", msgout=print)  # Use `print` to handle output logs.
+
+>>> cct.ajax('http://ajax-url')  # Start a AJAX request.
+{'result': 'data'}  # As python dict.
+
+>>> cct.ajax('http://ajax-url', {'data': 'value'})  # AJAX request with param.
+{'result': 'data'}
+
+>>> cct.ajax('http://ajax-url', method='post')  # AJAX request using post. default is 'get'.
+{'result': 'data'}
+
+>>> if not cct.is_admin():  # Check does the script has admin privileges.
+...     cct.runas_admin(__file__)  # run the script with admin privileges.
+... else:
+...     # your code here
+```
+
+## Updates
+* 2021-01-29 v3.0.0:
+    * Deprecated `image_to_color()`, add `main_color()`.
+        * use `main_color(..., is_url=True)` instead of `image_to_color(...)`
```

### Comparing `consolecmdtools-3.4.1/consolecmdtools/__init__.py` & `consolecmdtools-3.5.1/consolecmdtools/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -1,413 +1,452 @@
-# -*- coding: utf-8 -*-
-import os
-import sys
-import urllib.request
-import json
-import io
-# !! some imports are lazy-loaded
-
-import consoleiotools as cit
-
-__version__ = '3.4.1'
-
-
-def banner(text: str) -> str:
-    """Generate a banner of 3 lines"""
-    FILLER = "#"
-    text = text.strip()
-    middle_line = FILLER + text.center(int(len(text) / 0.618)) + FILLER
-    top_line = bottom_line = FILLER * len(middle_line)
-    return "\n".join([top_line, middle_line, bottom_line])
-
-
-def md5(target, force_text=False) -> str:
-    """Generate MD5 hash for bytes, string, int, file, etc."""
-    import hashlib
-
-    if not target:
-        return None
-    if not force_text and os.path.isfile(target):  # if target is a file
-        with open(target, 'rb') as f:
-            content = f.read().replace(os.linesep.encode(), b"\n")  # universal newline
-            return hashlib.md5(content).hexdigest()
-    if type(target) != bytes:  # the input of hashlib.md5() should be type of bytes
-        target = str(target).encode()
-    return hashlib.md5(target).hexdigest()
-
-
-def crc32(target, force_text=False) -> int:
-    """Generate CRC32 hash for bytes, string, int, file, etc."""
-    import binascii
-
-    if not target:
-        return 0
-    if not force_text and os.path.isfile(target):  # if target is a file
-        with open(target, 'rb') as f:
-            content = f.read().replace(os.linesep.encode(), b"\n")  # universal newline
-            return binascii.crc32(content)
-    if type(target) != bytes:  # if target is str/int/float, the input of binascii.crc32() should be type of bytes
-        target = str(target).encode()
-    return binascii.crc32(target)
-
-
-def main_color(source: str, scale: int = 200, triplet: str = "rgb", is_url: bool = False) -> tuple:
-    """Get a representative color from the source-pointed image
-
-    Imports:
-        colorsys: shipped with python.
-        PIL: use `pip install pillow` or install by package manager (apt, apk, etc).
-
-    Args:
-        source: str. The URL of the image, or the filepath.
-        scale: int. The size of generated image thumbnail.
-        triplet: str. The return value format. `rgb` for RGB triplet: (255, 255, 255), and `hex` for HEX triplet: '#FFFFFF'.
-        is_url: The source should be downloaded or not.
-
-    Returns:
-        The main color of the source image in RGB or HEX format.
-    """
-    import colorsys
-    try:
-        from PIL import Image
-    except ModuleNotFoundError as e:
-        raise ModuleNotFoundError("Install pillow (`pip install pillow`) to use PIL.") from e
-
-    if not source:
-        return None
-    if is_url:
-        img_buffer = io.BytesIO(read_url(source))
-        img = Image.open(img_buffer).convert("RGBA")
-    else:  # source is an image file
-        img = Image.open(source).convert("RGBA")
-    img.thumbnail((scale, scale))
-    statistics = {
-        "r": 0,
-        "g": 0,
-        "b": 0,
-        "coef": 0
-    }
-    for count, (r, g, b, a) in img.getcolors(img.size[0] * img.size[1]):  # get each color used in image with its count, maxcolors = the size of the image.
-        h, s, v = colorsys.rgb_to_hsv(r / 255, g / 255, b / 255)
-        saturation = s * 255  # extend the range from 0~1 to 0~255
-        coefficient = (saturation * count * a) or 0.01  # get how important this color is. Should not be 0.
-        statistics["r"] += coefficient * r  # raise the importance of red of this image.
-        statistics["g"] += coefficient * g
-        statistics["b"] += coefficient * b
-        statistics["coef"] += coefficient
-    color = (
-        int(statistics["r"] / statistics["coef"]),  # normalize to 0~255
-        int(statistics["g"] / statistics["coef"]),
-        int(statistics["b"] / statistics["coef"])
-    )
-    if triplet.lower() == "hex":
-        return "#%0.2X%0.2X%0.2X" % color
-    else:
-        return color
-
-
-def clear_screen():
-    """Clear the console screen"""
-    if sys.platform.startswith("win"):  # Windows
-        os.system("cls")
-    elif os.name == "posix":  # Linux and Unix
-        os.system("clear")
-    elif sys.platform == "darwin":  # macOS
-        os.system("clear")
-    else:
-        cit.err("No clearScreen for " + sys.platform)
-
-
-def get_py_cmd() -> str:
-    """Get OS's python command"""
-    if sys.platform.startswith("win"):
-        return "py"
-    elif os.name == "posix":
-        return "python3"
-    elif sys.platform == "darwin":
-        return "python3"
-    else:
-        return sys.executable
-
-
-def run_cmd(cmd: str) -> bool:
-    """Run command and show if success or failed
-
-    Args:
-        cmd: string
-    Returns:
-        bool: Does this command run successfully
-    """
-    SUCCESS_CODE = 0
-    cit.echo(cmd, pre="command")
-    is_success = (os.system(cmd) == SUCCESS_CODE)
-    if not is_success:
-        cit.warn("Command Failed")
-
-
-def read_cmd(cmd: str) -> str:
-    """Run command and return command's output
-
-    Args:
-        cmd: string
-    Returns:
-        str: What the command's output to stdout
-    """
-    import shlex
-    import subprocess
-
-    cit.echo(cmd, pre="command")
-    args = shlex.split(cmd)
-    proc = subprocess.Popen(args, stdout=subprocess.PIPE)
-    (proc_stdout, proc_stderr) = proc.communicate(input=None)  # proc_stdin
-    return proc_stdout.decode()  # Decode stdout and stderr bytes to str
-
-
-def is_cmd_exist(cmd: str) -> bool:
-    """Test if command is available for execution
-
-    Args:
-        cmd: string
-    Returns:
-        bool: if the command is exist
-    """
-    if sys.platform.startswith('win'):  # Windows
-        result = os.system("where {} >nul 2>&1".format(cmd))
-        return (result == 0)
-    else:  # Linux, Unix, macOS
-        proc = os.popen("command -v {}".format(cmd))
-        result = proc.read()
-        proc.close()
-        return (result != "")
-
-
-def get_dir(filename: str, mode: str = 'dir') -> str:
-    """Get file dir's name and dir's basename.
-
-    If file located at /path/to/dir/file, then the dirname is "/path/to/dir", and basename is "dir"
-
-    Args:
-        filename: str. Local filename, normally it's __file__.
-        mode: str. `file` return the file path, `dir` return the dir path, `basename` return dir basename.
-
-    Returns:
-        str: file path or dir path or dir basename based on mode.
-    """
-    file_path = os.path.abspath(filename)
-    dir_path = os.path.dirname(file_path)
-    dir_basename = os.path.basename(dir_path)
-    if mode == 'file':
-        return os.path.abspath(filename)
-    elif mode == 'dir':
-        return dir_path
-    elif mode == 'basename':
-        return dir_basename
-    else:
-        return dir_path
-
-
-def select_path(multiple: bool = False, folder: bool = False, *args, **kwargs):
-    """Open a file dialog to get file or folder path.
-
-    Args:
-        multiple: bool. The file dialog select multiple files, and return list.
-        folder: bool. The file dialog select folder not file.
-        *: Any additional args will considered as filedialog args.
-
-    Returns:
-        str: The path of selected file or folder.
-        list: The path list of selected files.
-    """
-    import tkinter
-    import tkinter.filedialog
-    tkapp = tkinter.Tk()
-    tkapp.withdraw()
-    tkapp.update()
-    if folder:
-        path = tkinter.filedialog.askdirectory(*args, **kwargs)
-    elif multiple:
-        path = tkinter.filedialog.askopenfilenames(*args, **kwargs)
-    else:
-        path = tkinter.filedialog.askopenfilename(*args, **kwargs)
-    tkapp.destroy()
-    return path
-
-
-def show_in_folder(path: str, ask: bool = False):
-    """Show file in Explorer/Finder/Folder"""
-    import subprocess
-    import platform
-    if ask:
-        cit.ask("Show in folder?")
-        if cit.get_choice(('Yes', 'No')) == 'No':
-            return False
-    if sys.platform.startswith("win"):
-        os.startfile(path)
-    elif platform.system() == "Darwin":
-        subprocess.Popen(["open", path])
-    else:
-        subprocess.Popen(["xdg-open", path])
-
-
-def diff(a, b, meta: bool = False, force_str: bool = False, context: int = 0) -> list:
-    """Compare two strings, lists or files and return their differences as list.
-
-    Args:
-        a: str/list/file. The source of comparison.
-        b: str/list/file. The target of comparison.
-        meta: bool. Show the meta data in the first 3 lines.
-        force_str: bool. Set to `True` if you wanna force to compare `a` and `b` as string. Default is False.
-        context: int. Number of context lines returns with diffs. Default is 0, no context lines shows.
-
-    Returns:
-        list: Diffs where the dst is not same as src. Only lines with diffs in the result. The first 2 lines are the header of diffs.
-    """
-    import difflib
-
-    src, dst = {'raw': a}, {'raw': b}
-    for d in (src, dst):
-        if isinstance(d['raw'], str):
-            if (not force_str) and os.path.isfile(d['raw']):
-                d['label'] = os.path.basename(d['raw'])  # filename will show in header of diffs
-                with open(d['raw'], encoding='utf-8') as f:
-                    d['content'] = f.readlines()
-            else:
-                d['label'] = str(str)
-                d['content'] = d['raw'].split('\n')  # convert str to list for comparison. Ex. ['str',]
-        else:
-            d['label'] = str(type(d['raw']))
-            d['content'] = d['raw']
-    diffs = difflib.unified_diff(src['content'], dst['content'], n=context, fromfile=src['label'], tofile=dst['label'])
-    diffs = [ln.strip('\n') for ln in diffs]  # Ensure no \n returns
-    return diffs if meta else diffs[3:]
-
-
-def update_file(filename: str, url: str) -> bool:
-    """Check and update file compares with remote_url
-
-    Args:
-        filename: str. Local filename, normally it's `__file__`
-        url: str or urllib.request.Request object. Remote url of raw file content. Use urllib.request.Request object for headers.
-    Returns:
-        bool: file updated or not
-    """
-    def compare(s1, s2):
-        return s1 == s2, len(s2) - len(s1)
-
-    if not url or not filename:
-        return False
-    try:
-        raw_codes = read_url(url)
-        with open(filename, "rb") as f:
-            current_codes = f.read().replace(b"\r", b"")
-        is_same, diff = compare(current_codes, raw_codes)
-        if is_same:
-            cit.info("{} is already up-to-date.".format(filename))
-            return False
-        else:
-            cit.ask("A new version is available. Update? (Diff: {})".format(diff))
-            if cit.get_choice(["Yes", "No"]) == "Yes":
-                with open(filename, "wb") as f:
-                    f.write(raw_codes)
-                cit.info("Update Success.")
-                return True
-            else:
-                cit.warn("Update Canceled")
-                return False
-    except Exception as e:
-        cit.err("{f} update failed: {e}".format(f=filename, e=e))
-        return False
-
-
-def read_file(filepath, *args, **kwargs) -> str:
-    """Try different encoding to open a file in readonly mode."""
-    for mode in ("utf-8", "gbk", "cp1252", "windows-1252", "latin-1", "ascii"):
-        try:
-            with open(filepath, *args, encoding=mode, **kwargs) as f:
-                content = f.read()
-                cit.info("File is read in {} mode.".format(mode))
-                return content
-        except UnicodeDecodeError:
-            cit.warn("File cannot be opened in {} mode".format(mode))
-    with open(filepath, *args, encoding='ascii', errors='surrogateescape', **kwargs) as f:
-        content = f.read()
-        cit.info("File is read in ASCII surrogate escape mode.")
-        return content
-
-
-def read_url(source) -> bytes:
-    """Try to get file content from the url
-
-    Args:
-        source: str or Request. The target url.
-
-    Returns:
-        bytes: The content of the request's response.
-    """
-    response = urllib.request.urlopen(source)
-    return response.read() if response else None
-
-
-def ajax(url: str, param: dict = {}, method: str = "get"):
-    """Get response using AJAX.
-
-    Args:
-        url: string. The requesting url.
-        param: dict. The parameters in the request payload.
-        method: str. The method of request, "get" or "post".
-    Returns:
-        dict: The responsed json decoded into a dict.
-    """
-    if method.lower() == "get":
-        if param:
-            param = urllib.parse.urlencode(param)
-            url += "?" + param
-        req = urllib.request.Request(url)
-    elif method.lower() == "post":
-        param = json.dumps(param).encode("utf-8")
-        req = urllib.request.Request(url, data=param)
-    else:
-        raise Exception("invalid method '{}' (GET/POST)".format(method))
-    rsp_bytes = read_url(req)
-    if rsp_bytes:
-        rsp_str = rsp_bytes.decode("utf-8")
-        try:
-            return json.loads(rsp_str)
-        except json.decoder.JSONDecodeError as e:
-            return rsp_str
-    return None
-
-
-def is_python3() -> bool:
-    """Check does the script is running in python3"""
-    return sys.version_info[0] == 3
-
-
-def is_admin() -> bool:
-    """Check does the script has admin privileges."""
-    import ctypes
-    try:
-        return ctypes.windll.shell32.IsUserAnAdmin()
-    except AttributeError:  # Windows only
-        return None
-
-
-def runas_admin(py_file: str) -> bool:
-    """Execute a python script with admin privileges.
-
-    Links:
-        Syntax of ShellExecuteW: https://docs.microsoft.com/en-us/windows/win32/api/shellapi/nf-shellapi-shellexecutew
-
-    Args:
-        py_file: string. The command line arguments passed to python. It should be the script path, such as `__file__`.
-    """
-    import ctypes
-    parent_window_handle = None  # no UI
-    operation = "runas"  # run as admin
-    executor = sys.executable  # python.exe
-    parameter = py_file
-    directory = None  # using current working directory.
-    SHOWNORMAL = 1  # SW_SHOWNORMAL
-    if not os.path.isfile(parameter):
-        raise FileNotFoundError(parameter)
-    return_code = ctypes.windll.shell32.ShellExecuteW(parent_window_handle, operation, executor, parameter, directory, SHOWNORMAL)
-    return return_code > 32  # should be greater than 32 if execute success
+# -*- coding: utf-8 -*-
+import os
+import sys
+import urllib.request
+import json
+import io
+# !! some imports are lazy-loaded
+
+import consoleiotools as cit
+
+__version__ = '3.5.1'
+
+
+def banner(text: str) -> str:
+    """Generate a banner of 3 lines"""
+    FILLER = "#"
+    text = text.strip()
+    middle_line = FILLER + text.center(int(len(text) / 0.618)) + FILLER
+    top_line = bottom_line = FILLER * len(middle_line)
+    return "\n".join([top_line, middle_line, bottom_line])
+
+
+def md5(target, force_text=False) -> str:
+    """Generate MD5 hash for bytes, str, int, file, etc."""
+    import hashlib
+
+    if not target:
+        return None
+    if not force_text and os.path.isfile(target):  # if target is a file
+        with open(target, 'rb') as f:
+            content = f.read().replace(os.linesep.encode(), b"\n")  # universal newline
+            return hashlib.md5(content).hexdigest()
+    if type(target) != bytes:  # the input of hashlib.md5() should be type of bytes
+        target = str(target).encode()
+    return hashlib.md5(target).hexdigest()
+
+
+def crc32(target, force_text=False) -> int:
+    """Generate CRC32 hash for bytes, str, int, file, etc."""
+    import binascii
+
+    if not target:
+        return 0
+    if not force_text and os.path.isfile(target):  # if target is a file
+        with open(target, 'rb') as f:
+            content = f.read().replace(os.linesep.encode(), b"\n")  # universal newline
+            return binascii.crc32(content)
+    if type(target) != bytes:  # if target is str/int/float, the input of binascii.crc32() should be type of bytes
+        target = str(target).encode()
+    return binascii.crc32(target)
+
+
+def main_color(source: str, scale: int = 200, triplet: str = "rgb", is_url: bool = False) -> str:
+    """Get a representative color from the source-pointed image
+
+    Imports:
+        colorsys: Shipped with python.
+        PIL: Use `pip install pillow` or install by package manager (apt, apk, etc).
+
+    Args:
+        source (str): The URL of the image, or the filepath.
+        scale (int): The size of generated image thumbnail.
+        triplet (str): The return value format. `rgb` for RGB triplet: (255, 255, 255), and `hex` for HEX triplet: '#FFFFFF'.
+        is_url (bool): The source should be downloaded or not.
+
+    Returns:
+        str: The main color of the source image in RGB or HEX format.
+    """
+    import colorsys
+    try:
+        from PIL import Image
+    except ModuleNotFoundError as e:
+        raise ModuleNotFoundError("Install pillow (`pip install pillow`) to use PIL.") from e
+
+    if not source:
+        return None
+    if is_url:
+        img_buffer = io.BytesIO(read_url(source))
+        img = Image.open(img_buffer).convert("RGBA")
+    else:  # source is an image file
+        img = Image.open(source).convert("RGBA")
+    img.thumbnail((scale, scale))
+    statistics = {
+        "r": 0,
+        "g": 0,
+        "b": 0,
+        "coef": 0
+    }
+    for count, (r, g, b, a) in img.getcolors(img.size[0] * img.size[1]):  # get each color used in image with its count, maxcolors = the size of the image.
+        h, s, v = colorsys.rgb_to_hsv(r / 255, g / 255, b / 255)
+        saturation = s * 255  # extend the range from 0~1 to 0~255
+        coefficient = (saturation * count * a) or 0.01  # get how important this color is. Should not be 0.
+        statistics["r"] += coefficient * r  # raise the importance of red of this image.
+        statistics["g"] += coefficient * g
+        statistics["b"] += coefficient * b
+        statistics["coef"] += coefficient
+    color = (
+        int(statistics["r"] / statistics["coef"]),  # normalize to 0~255
+        int(statistics["g"] / statistics["coef"]),
+        int(statistics["b"] / statistics["coef"])
+    )
+    if triplet.lower() == "hex":
+        return "#%0.2X%0.2X%0.2X" % color
+    else:
+        return color
+
+
+def clear_screen():
+    """Clear the console screen"""
+    if sys.platform.startswith("win"):  # Windows
+        os.system("cls")
+    elif os.name == "posix":  # Linux and Unix
+        os.system("clear")
+    elif sys.platform == "darwin":  # macOS
+        os.system("clear")
+    else:
+        cit.err("No clearScreen for " + sys.platform)
+
+
+def get_py_cmd() -> str:
+    """Get OS's python command"""
+    if sys.platform.startswith("win"):
+        return "py"
+    elif os.name == "posix":
+        return "python3"
+    elif sys.platform == "darwin":
+        return "python3"
+    else:
+        return sys.executable
+
+
+def run_cmd(cmd: str) -> bool:
+    """Run command and show if success or failed
+
+    Args:
+        cmd (str): The command.
+    Returns:
+        bool: Does this command run successfully
+    """
+    SUCCESS_CODE = 0
+    cit.echo(cmd, pre="command")
+    is_success = (os.system(cmd) == SUCCESS_CODE)
+    if not is_success:
+        cit.warn("Command Failed")
+
+
+def read_cmd(cmd: str) -> str:
+    """Run command and return command's output
+
+    Args:
+        cmd (str): The command.
+    Returns:
+        str: What the command's output to stdout
+    """
+    import shlex
+    import subprocess
+
+    cit.echo(cmd, pre="command")
+    args = shlex.split(cmd)
+    proc = subprocess.Popen(args, stdout=subprocess.PIPE)
+    (proc_stdout, proc_stderr) = proc.communicate(input=None)  # proc_stdin
+    return proc_stdout.decode()  # Decode stdout and stderr bytes to str
+
+
+def is_cmd_exist(cmd: str) -> bool:
+    """Test if command is available for execution
+
+    Args:
+        cmd (str): The command.
+    Returns:
+        bool: if the command is exist
+    """
+    if sys.platform.startswith('win'):  # Windows
+        result = os.system("where {} >nul 2>&1".format(cmd))
+        return (result == 0)
+    else:  # Linux, Unix, macOS
+        proc = os.popen("command -v {}".format(cmd))
+        result = proc.read()
+        proc.close()
+        return (result != "")
+
+
+def get_dir(filename: str, mode: str = 'dir') -> str:
+    """Get file dir's name and dir's basename.
+
+    If file located at /path/to/dir/file, then the dirname is "/path/to/dir", and basename is "dir"
+
+    Args:
+        filename (str): Local filename, normally it's __file__.
+        mode (str): `file` return the file path, `dir` return the dir path, `basename` return dir basename.
+
+    Returns:
+        str: file path or dir path or dir basename based on mode.
+    """
+    file_path = os.path.abspath(filename)
+    dir_path = os.path.dirname(file_path)
+    dir_basename = os.path.basename(dir_path)
+    if mode == 'file':
+        return os.path.abspath(filename)
+    elif mode == 'dir':
+        return dir_path
+    elif mode == 'basename':
+        return dir_basename
+    else:
+        return dir_path
+
+
+def select_path(multiple: bool = False, folder: bool = False, *args, **kwargs):
+    """Open a file dialog to get file or folder path.
+
+    Args:
+        multiple (bool): The file dialog select multiple files, and return list.
+        folder (bool): The file dialog select folder not file.
+        *: Any additional args will considered as filedialog args.
+
+    Returns:
+        str: The path of selected file or folder.
+        list: The path list of selected files.
+    """
+    import tkinter
+    import tkinter.filedialog
+    tkapp = tkinter.Tk()
+    tkapp.withdraw()
+    tkapp.update()
+    if folder:
+        path = tkinter.filedialog.askdirectory(*args, **kwargs)
+    elif multiple:
+        path = tkinter.filedialog.askopenfilenames(*args, **kwargs)
+    else:
+        path = tkinter.filedialog.askopenfilename(*args, **kwargs)
+    tkapp.destroy()
+    return path
+
+
+def show_in_folder(path: str, ask: bool = False):
+    """Show file in Explorer/Finder/Folder"""
+    import subprocess
+    import platform
+    if ask:
+        cit.ask("Show in folder?")
+        if cit.get_choice(('Yes', 'No')) == 'No':
+            return False
+    if sys.platform.startswith("win"):
+        os.startfile(path)
+    elif platform.system() == "Darwin":
+        subprocess.Popen(["open", path])
+    else:
+        subprocess.Popen(["xdg-open", path])
+
+
+def diff(a, b, meta: bool = False, force_str: bool = False, context: int = 0) -> list:
+    """Compare two strings, lists or files and return their differences as list.
+
+    Args:
+        a (str|list|file): The source of comparison.
+        b (str|list|file): The target of comparison.
+        meta (bool): Show the meta data in the first 3 lines.
+        force_str (bool): Set to `True` if you wanna force to compare `a` and `b` as string. Default is False.
+        context (int): Number of context lines returns with diffs. Default is 0, no context lines shows.
+
+    Returns:
+        list: Diffs where the dst is not same as src. Only lines with diffs in the result. The first 2 lines are the header of diffs.
+    """
+    import difflib
+
+    src, dst = {'raw': a}, {'raw': b}
+    for d in (src, dst):
+        if isinstance(d['raw'], str):
+            if (not force_str) and os.path.isfile(d['raw']):
+                d['label'] = os.path.basename(d['raw'])  # filename will show in header of diffs
+                with open(d['raw'], encoding='utf-8') as f:
+                    d['content'] = f.readlines()
+            else:
+                d['label'] = str(str)
+                d['content'] = d['raw'].split('\n')  # convert str to list for comparison. Ex. ['str',]
+        else:
+            d['label'] = str(type(d['raw']))
+            d['content'] = d['raw']
+    diffs = difflib.unified_diff(src['content'], dst['content'], n=context, fromfile=src['label'], tofile=dst['label'])
+    diffs = [ln.strip('\n') for ln in diffs]  # Ensure no \n returns
+    return diffs if meta else diffs[3:]
+
+
+def update_file(filename: str, url: str) -> bool:
+    """Check and update file compares with remote_url
+
+    Args:
+        filename (str): Local filename, normally it's `__file__`
+        url (str|urllib.request.Request): Remote url of raw file content. Use urllib.request.Request object for headers.
+    Returns:
+        bool: File updated or not
+    """
+    def compare(s1, s2):
+        return s1 == s2, len(s2) - len(s1)
+
+    if not url or not filename:
+        return False
+    try:
+        raw_codes = read_url(url)
+        with open(filename, "rb") as f:
+            current_codes = f.read().replace(b"\r", b"")
+        is_same, diff = compare(current_codes, raw_codes)
+        if is_same:
+            cit.info("{} is already up-to-date.".format(filename))
+            return False
+        else:
+            cit.ask("A new version is available. Update? (Diff: {})".format(diff))
+            if cit.get_choice(["Yes", "No"]) == "Yes":
+                with open(filename, "wb") as f:
+                    f.write(raw_codes)
+                cit.info("Update Success.")
+                return True
+            else:
+                cit.warn("Update Canceled")
+                return False
+    except Exception as e:
+        cit.err("{f} update failed: {e}".format(f=filename, e=e))
+        return False
+
+
+def read_file(filepath, *args, **kwargs) -> str:
+    """Try different encoding to open a file in readonly mode."""
+    for mode in ("utf-8", "gbk", "cp1252", "windows-1252", "latin-1", "ascii"):
+        try:
+            with open(filepath, *args, encoding=mode, **kwargs) as f:
+                content = f.read()
+                cit.info("File is read in {} mode.".format(mode))
+                return content
+        except UnicodeDecodeError:
+            cit.warn("File cannot be opened in {} mode".format(mode))
+    with open(filepath, *args, encoding='ascii', errors='surrogateescape', **kwargs) as f:
+        content = f.read()
+        cit.info("File is read in ASCII surrogate escape mode.")
+        return content
+
+
+def read_url(source) -> bytes:
+    """Try to get file content from the url
+
+    Args:
+        source (str|Request): The target url.
+
+    Returns:
+        bytes: The content of the request's response.
+    """
+    response = urllib.request.urlopen(source)
+    return response.read() if response else None
+
+
+def move_file(src: str, dst: str, copy: bool = False, backup: bool = False, msgout: callable = None):
+    """Move or copy file from one place to another.
+
+    Args:
+        src (str): Source file path.
+        dst (str): Destination file path.
+        copy (bool): Copy or move source file to destination.
+        backup (bool): Backup destination file or not. `True` means try to backup destination file, pass if destination file does not exist.
+        msgout (callable): Output function to handle the outputs. `None` means no outputs.
+    """
+    import time
+    import shutil
+
+    def _msg(message):
+        if msgout:
+            msgout(message)
+    _msg(f"From{' (+Copy)' if copy else ''}: {src}")
+    _msg(f"To{' (+Backup)' if backup else ''}: {dst}")
+    if not os.path.exists(src):
+        raise FileNotFoundError(f"Source file {src} does not exist.")
+    if os.path.exists(dst):
+        if backup:
+            dst_backup = f"{dst}.backup.{time.strftime('%Y%m%d%H%M%S')}"
+            shutil.copy2(dst, dst_backup)
+            _msg(f"Destination file {dst} backuped up to {dst_backup}.")
+        else:
+            _msg(f"Warning: Destination file {dst} already exists and will be overwritten.")
+    else:
+        if backup:
+            _msg(f"Warning: Destination file {dst} does not exist, backup skipped.")
+    if copy:
+        shutil.copy2(src, dst)
+    else:
+        shutil.move(src, dst)
+    _msg(f"File {src} {'copied' if copy else 'moved'} to {dst}.")
+
+
+def ajax(url: str, param: dict = {}, method: str = "get"):
+    """Get response using AJAX.
+
+    Args:
+        url (str): The requesting url.
+        param (dict): The parameters in the request payload.
+        method (str): The method of request, "get" or "post".
+    Returns:
+        dict: The responsed json decoded into a dict.
+    """
+    if method.lower() == "get":
+        if param:
+            param = urllib.parse.urlencode(param)
+            url += "?" + param
+        req = urllib.request.Request(url)
+    elif method.lower() == "post":
+        param = json.dumps(param).encode("utf-8")
+        req = urllib.request.Request(url, data=param)
+    else:
+        raise Exception("invalid method '{}' (GET/POST)".format(method))
+    rsp_bytes = read_url(req)
+    if rsp_bytes:
+        rsp_str = rsp_bytes.decode("utf-8")
+        try:
+            return json.loads(rsp_str)
+        except json.decoder.JSONDecodeError as e:
+            return rsp_str
+    return None
+
+
+def is_python3() -> bool:
+    """Check does the script is running in python3"""
+    return sys.version_info[0] == 3
+
+
+def is_admin() -> bool:
+    """Check does the script has admin privileges."""
+    import ctypes
+    try:
+        return ctypes.windll.shell32.IsUserAnAdmin()
+    except AttributeError:  # Windows only
+        return None
+
+
+def runas_admin(py_file: str) -> bool:
+    """Execute a python script with admin privileges.
+
+    Links:
+        Syntax of ShellExecuteW: https://docs.microsoft.com/en-us/windows/win32/api/shellapi/nf-shellapi-shellexecutew
+
+    Args:
+        py_file (str): The command line arguments passed to python. It should be the script path, such as `__file__`.
+    Returns:
+        bool: Command run success.
+    """
+    import ctypes
+    parent_window_handle = None  # no UI
+    operation = "runas"  # run as admin
+    executor = sys.executable  # python.exe
+    parameter = py_file
+    directory = None  # using current working directory.
+    SHOWNORMAL = 1  # SW_SHOWNORMAL
+    if not os.path.isfile(parameter):
+        raise FileNotFoundError(parameter)
+    return_code = ctypes.windll.shell32.ShellExecuteW(parent_window_handle, operation, executor, parameter, directory, SHOWNORMAL)
+    return return_code > 32  # should be greater than 32 if execute success
```

### Comparing `consolecmdtools-3.4.1/consolecmdtools/__main__.py` & `consolecmdtools-3.5.1/consolecmdtools/__main__.py`

 * *Ordering differences only*

 * *Files 20% similar despite different names*

```diff
@@ -1,51 +1,51 @@
-import consoleiotools as cit
-import consolecmdtools as cct
-
-
-def inspect(func_name, *args, **kwargs):
-    cit.br()
-    args_txt = ""
-    if args:
-        args_txt += ", ".join(f"{('`' + a + '`') if isinstance(a, str) else str(a)}" for a in args)
-    if kwargs:
-        args_txt += ", " + ", ".join(f"{k}=" + f"{('`' + v + '`') if isinstance(v, str) else str(v)}" for k, v in kwargs.items())
-    cit.print(f"[dim bright_white]# {func_name}({args_txt})")
-    return getattr(cct, func_name)(*args, **kwargs)
-
-
-def examples():
-    inspect("clear_screen")
-    cit.print(inspect("banner", "This is a banner"))
-    cit.print(inspect("md5", "blah blah blah"))
-    cit.print(inspect("md5", 42))
-    cit.print(inspect("md5", "README.md"))
-    cit.print(inspect("md5", "README.md", force_text=True))
-    cit.print(inspect("crc32", "blah blah blah"))
-    cit.print(inspect("crc32", 42))
-    cit.print(inspect("crc32", "README.md"))
-    cit.print(inspect("crc32", "README.md", force_text=True))
-    cit.print(inspect("get_py_cmd"))
-    inspect("run_cmd", "echo hello")
-    cit.print(inspect("read_cmd", "echo hello"))
-    cit.print(inspect("is_cmd_exist", "ls"))
-    cit.print(inspect("get_dir", "README.md"))
-    cit.print(inspect("get_dir", "README.md", mode="file"))
-    cit.print(inspect("get_dir", "README.md", mode="basename"))
-    for line in inspect("diff", "str 1", "str 2"):
-        cit.print(line)
-    for line in inspect("diff", "str 1", "str 2", meta=True):
-        cit.print(line)
-    for line in inspect("diff", ["a", "b"], ["a", "b", "c"]):
-        cit.print(line)
-    for line in inspect("diff", ["a", "b"], ["a", "b", "c"], context=2):
-        cit.print(line)
-    resp = inspect("ajax", "https://yesno.wtf/api", method="get")
-    cit.print(resp)
-    cit.print(inspect("main_color", resp["image"], is_url=True))
-    cit.print(inspect("read_file", "README.md")[:19])
-    cit.print(inspect("is_admin"))
-
-
-if __name__ == "__main__":
-    cit.panel(f"cct.__version__ = {cct.__version__}", title="ConsoleCMDTools Features")
-    examples()
+import consoleiotools as cit
+import consolecmdtools as cct
+
+
+def inspect(func_name, *args, **kwargs):
+    cit.br()
+    args_txt = ""
+    if args:
+        args_txt += ", ".join(f"{('`' + a + '`') if isinstance(a, str) else str(a)}" for a in args)
+    if kwargs:
+        args_txt += ", " + ", ".join(f"{k}=" + f"{('`' + v + '`') if isinstance(v, str) else str(v)}" for k, v in kwargs.items())
+    cit.print(f"[dim bright_white]# {func_name}({args_txt})")
+    return getattr(cct, func_name)(*args, **kwargs)
+
+
+def examples():
+    inspect("clear_screen")
+    cit.print(inspect("banner", "This is a banner"))
+    cit.print(inspect("md5", "blah blah blah"))
+    cit.print(inspect("md5", 42))
+    cit.print(inspect("md5", "README.md"))
+    cit.print(inspect("md5", "README.md", force_text=True))
+    cit.print(inspect("crc32", "blah blah blah"))
+    cit.print(inspect("crc32", 42))
+    cit.print(inspect("crc32", "README.md"))
+    cit.print(inspect("crc32", "README.md", force_text=True))
+    cit.print(inspect("get_py_cmd"))
+    inspect("run_cmd", "echo hello")
+    cit.print(inspect("read_cmd", "echo hello"))
+    cit.print(inspect("is_cmd_exist", "ls"))
+    cit.print(inspect("get_dir", "README.md"))
+    cit.print(inspect("get_dir", "README.md", mode="file"))
+    cit.print(inspect("get_dir", "README.md", mode="basename"))
+    for line in inspect("diff", "str 1", "str 2"):
+        cit.print(line)
+    for line in inspect("diff", "str 1", "str 2", meta=True):
+        cit.print(line)
+    for line in inspect("diff", ["a", "b"], ["a", "b", "c"]):
+        cit.print(line)
+    for line in inspect("diff", ["a", "b"], ["a", "b", "c"], context=2):
+        cit.print(line)
+    resp = inspect("ajax", "https://yesno.wtf/api", method="get")
+    cit.print(resp)
+    cit.print(inspect("main_color", resp["image"], is_url=True))
+    cit.print(inspect("read_file", "README.md")[:19])
+    cit.print(inspect("is_admin"))
+
+
+if __name__ == "__main__":
+    cit.panel(f"cct.__version__ = {cct.__version__}", title="ConsoleCMDTools Features")
+    examples()
```

### Comparing `consolecmdtools-3.4.1/consolecmdtools.egg-info/PKG-INFO` & `consolecmdtools-3.5.1/PKG-INFO`

 * *Files 22% similar despite different names*

```diff
@@ -1,186 +1,215 @@
-Metadata-Version: 2.1
-Name: consolecmdtools
-Version: 3.4.1
-Summary: Console command tools in Python
-Author-email: Kyan <kai@kyan001.com>
-License: LICENSE
-Project-URL: Homepage, https://github.com/kyan001/PyConsoleCMDTools
-Project-URL: Issue Tracker, https://github.com/kyan001/PyConsoleCMDTools/issues
-Project-URL: Source Code, https://github.com/kyan001/PyConsoleCMDTools
-Keywords: python,console,command,tool
-Classifier: Development Status :: 5 - Production/Stable
-Classifier: Intended Audience :: Developers
-Classifier: Topic :: Software Development :: User Interfaces
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3 :: Only
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-Provides-Extra: opt
-Provides-Extra: dev
-License-File: LICENSE
-
-# PyConsoleCMDTools
-![PyPI - Downloads](https://img.shields.io/pypi/dm/consolecmdtools)
-![GitHub release](https://img.shields.io/github/v/release/kyan001/PyConsoleCMDTools)
-[![GitHub license](https://img.shields.io/github/license/kyan001/PyConsoleCMDTools.svg)](https://github.com/kyan001/PyConsoleCMDTools/blob/master/LICENSE)
-
-## Installation
-
-```sh
-pip install consolecmdtools  # install
-pip install --upgrade consolecmdtools  # update
-python -m consolecmdtools  # examples
-```
-
-## Get Started
-
-```python
-import consolecmdtools as cct
-print(cct.__version__)
-```
-
-## Functions
-
-```python
->>> cct.banner("hello, world!")  # Generate banner for text
-#######################
-#    hello, world!    #
-#######################
-
->>> cct.md5("blah blah blah")  # Return md5 hash for text.
-'55e562bfee2bde4f9e71b8885eb5e303'
-
->>> cct.md5(42)  # Return md5 hash for number.
-'a1d0c6e83f027327d8461063f4ac58a6'
-
->>> cct.md5('file.txt')  # Return md5 hash for file.
-'d07aa6ddab4d6d2d2891aa9f3625a5db'
-
->>> cct.md5('file.txt', force_text=True)  # Force to return the md5 has for text, even the file exists.
-'3d8e577bddb17db339eae0b3d9bcf180'
-
->>> cct.crc32("blah blah blah")  # Return crc32 hash for text.
-753353432
-
->>> cct.crc32(42)  # Return crc32 hash for number.
-841265288
-
->>> cct.crc32('file.txt')  # Return crc32 hash for file.
-1030388931
-
->>> cct.crc32('file.txt', force_text=True)  # Force to return the md5 has for text, even the file exists.
-3774289445
-
->>> cct.main_color('image.jpg')  # Get theme color of image.
-(152, 156, 69)  # RGB value
-
->>> cct.main_color('http://image-url/image', is_url=True)  # Get theme color of web image.
-(152, 156, 69)  # RGB value
-
->>> cct.main_color('image.jpg', scale=500)  # Cost more time to generate a preciser color. default scale is 200.
-(152, 156, 69)
-
->>> cct.main_color('image.jpg', triplet='hex')  # Return color in hex triplet format. default mode is 'rgb'.
-'#989C45'
-
->>> cct.clear_screen()  # Clear the console.
-
->>> cct.get_py_cmd()  # Get python running command for different OS.
-'python3'
-
->>> cct.run_cmd("echo hello")  # Run console command. If the command failed, a warning message echoed. Returns bool.
-*
-| __RUN COMMAND__________________________
-| (Command) echo hello
-hello
-`
-
->>> cct.read_cmd("echo hello")  # Run a command and return the output.
-'hello\n'
-
->>> cct.is_cmd_exist("ls")  # Test if a command is exist.
-True
-
->>> cct.get_dir("./file")  # Get the parent folder path of the file.
-'/path/to/dir'  # '/path/to/dir/file' for example
-
->>> cct.get_dir("./file", mode="file")  # Get the file absolute path.
-'/path/to/dir/file'
-
->>> cct.get_dir("./file", mode="basename")  # Get the parent folder name of the file.
-'dir'
-
->>> cct.select_path()  # Show file dialog to get file path. Additional args pass to tkinter.filedialog.askopenfilename()
-'/path/to/dir/file'
-
->>> cct.select_path(multiple=True)  # Show file dialog to get multiple file paths.
-['/path/1', '/path/2']
-
->>> cct.select_path(folder=True)  # Show file dialog to get folder path.
-'/path/to/dir'
-
->>> cct.show_in_folder("/path/to/file")  # Show file in Explorer/Finder/Folder.
-
->>> cct.show_in_folder("/path/to/file", ask=True)  # Ask before show.
-
->>> cct.diff("str1", "str2")  # Compare 2 strings, return the list of diffs.
-[  # you can use `"\n".join(diff)` to print the diff.
-    "-str1",
-    "+str2"
-]
-
->>> cct.diff("str1", "str2", meta=True)  # show meta data in the first 3 lines.
-[
-    "--- <class 'str'>",
-    "+++ <class 'str'>",
-    "@@ -1 +1 @@",
-    "-str1",
-    "+str2"
-]
-
-
->>> cct.diff(["a", "b"], ["a", "b", "c"])  # Compare 2 lists and print diffs.
-[
-    "+c"
-]
-
->>> cct.diff(["a", "b"], ["a", "b", "c"], context=2)  # Show diffs with 2 extra context lines.
-[
-    " a",  # context line
-    " b",  # context line
-    "+c"  # diff
-]
-
->>> cct.diff("/path/to/file1", "/path/to/file2")  # Compare between 2 files.
-
->>> cct.diff("/path/to/file1", "str")  # Compare between file and str/list.
-
->>> cct.diff('str', 'str')  # If no diff, return [].
-[]
-
->>> cct.update_file('file', 'http://file-url')  # Update file if the file is not as same as url content.
-False  # if already up-to-date.
-
->>> cct.read_file('file')  # Read file using different encoding automatically.
-"file content"
-
->>> cct.ajax('http://ajax-url')  # Start a AJAX request.
-{'result': 'data'}  # As python dict.
-
->>> cct.ajax('http://ajax-url', {'data': 'value'})  # AJAX request with param.
-{'result': 'data'}
-
->>> cct.ajax('http://ajax-url', method='post')  # AJAX request using post. default is 'get'.
-{'result': 'data'}
-
->>> if not cct.is_admin():  # Check does the script has admin privileges.
-...     cct.runas_admin(__file__)  # run the script with admin privileges.
-... else:
-...     # your code here
-```
-
-## Updates
-* 2021-01-29 v3.0.0:
-    * Deprecated `image_to_color()`, add `main_color()`.
-        * use `main_color(..., is_url=True)` instead of `image_to_color(...)`
+Metadata-Version: 2.1
+Name: consolecmdtools
+Version: 3.5.1
+Summary: Console command tools in Python
+Author-email: Kyan <kai@kyan001.com>
+License: MIT License
+        
+        Copyright (c) 2020 Kyan
+        
+        Permission is hereby granted, free of charge, to any person obtaining a copy
+        of this software and associated documentation files (the "Software"), to deal
+        in the Software without restriction, including without limitation the rights
+        to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
+        copies of the Software, and to permit persons to whom the Software is
+        furnished to do so, subject to the following conditions:
+        
+        The above copyright notice and this permission notice shall be included in all
+        copies or substantial portions of the Software.
+        
+        THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
+        IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
+        FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
+        AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
+        LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
+        OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
+        SOFTWARE.
+        
+Project-URL: Homepage, https://github.com/kyan001/PyConsoleCMDTools
+Project-URL: Issue Tracker, https://github.com/kyan001/PyConsoleCMDTools/issues
+Project-URL: Source Code, https://github.com/kyan001/PyConsoleCMDTools
+Keywords: python,console,command,tool
+Classifier: Development Status :: 5 - Production/Stable
+Classifier: Intended Audience :: Developers
+Classifier: Topic :: Software Development :: User Interfaces
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3 :: Only
+Requires-Python: >=3.6
+Description-Content-Type: text/markdown
+Provides-Extra: opt
+Provides-Extra: dev
+License-File: LICENSE
+
+# PyConsoleCMDTools
+![PyPI - Downloads](https://img.shields.io/pypi/dm/consolecmdtools)
+![GitHub release](https://img.shields.io/github/v/release/kyan001/PyConsoleCMDTools)
+[![GitHub license](https://img.shields.io/github/license/kyan001/PyConsoleCMDTools.svg)](https://github.com/kyan001/PyConsoleCMDTools/blob/master/LICENSE)
+
+## Installation
+
+```sh
+pip install consolecmdtools  # install
+pip install --upgrade consolecmdtools  # update
+python -m consolecmdtools  # examples
+```
+
+## Get Started
+
+```python
+import consolecmdtools as cct
+print(cct.__version__)
+```
+
+## Functions
+
+```python
+>>> cct.banner("hello, world!")  # Generate banner for text
+#######################
+#    hello, world!    #
+#######################
+
+>>> cct.md5("blah blah blah")  # Return md5 hash for text.
+'55e562bfee2bde4f9e71b8885eb5e303'
+
+>>> cct.md5(42)  # Return md5 hash for number.
+'a1d0c6e83f027327d8461063f4ac58a6'
+
+>>> cct.md5('file.txt')  # Return md5 hash for file.
+'d07aa6ddab4d6d2d2891aa9f3625a5db'
+
+>>> cct.md5('file.txt', force_text=True)  # Force to return the md5 has for text, even the file exists.
+'3d8e577bddb17db339eae0b3d9bcf180'
+
+>>> cct.crc32("blah blah blah")  # Return crc32 hash for text.
+753353432
+
+>>> cct.crc32(42)  # Return crc32 hash for number.
+841265288
+
+>>> cct.crc32('file.txt')  # Return crc32 hash for file.
+1030388931
+
+>>> cct.crc32('file.txt', force_text=True)  # Force to return the md5 has for text, even the file exists.
+3774289445
+
+>>> cct.main_color('image.jpg')  # Get theme color of image.
+(152, 156, 69)  # RGB value
+
+>>> cct.main_color('http://image-url/image', is_url=True)  # Get theme color of web image.
+(152, 156, 69)  # RGB value
+
+>>> cct.main_color('image.jpg', scale=500)  # Cost more time to generate a preciser color. default scale is 200.
+(152, 156, 69)
+
+>>> cct.main_color('image.jpg', triplet='hex')  # Return color in hex triplet format. default mode is 'rgb'.
+'#989C45'
+
+>>> cct.clear_screen()  # Clear the console.
+
+>>> cct.get_py_cmd()  # Get python running command for different OS.
+'python3'
+
+>>> cct.run_cmd("echo hello")  # Run console command. If the command failed, a warning message echoed. Returns bool.
+*
+| __RUN COMMAND__________________________
+| (Command) echo hello
+hello
+`
+
+>>> cct.read_cmd("echo hello")  # Run a command and return the output.
+'hello\n'
+
+>>> cct.is_cmd_exist("ls")  # Test if a command is exist.
+True
+
+>>> cct.get_dir("./file")  # Get the parent folder path of the file.
+'/path/to/dir'  # '/path/to/dir/file' for example
+
+>>> cct.get_dir("./file", mode="file")  # Get the file absolute path.
+'/path/to/dir/file'
+
+>>> cct.get_dir("./file", mode="basename")  # Get the parent folder name of the file.
+'dir'
+
+>>> cct.select_path()  # Show file dialog to get file path. Additional args pass to tkinter.filedialog.askopenfilename()
+'/path/to/dir/file'
+
+>>> cct.select_path(multiple=True)  # Show file dialog to get multiple file paths.
+['/path/1', '/path/2']
+
+>>> cct.select_path(folder=True)  # Show file dialog to get folder path.
+'/path/to/dir'
+
+>>> cct.show_in_folder("/path/to/file")  # Show file in Explorer/Finder/Folder.
+
+>>> cct.show_in_folder("/path/to/file", ask=True)  # Ask before show.
+
+>>> cct.diff("str1", "str2")  # Compare 2 strings, return the list of diffs.
+[  # you can use `"\n".join(diff)` to print the diff.
+    "-str1",
+    "+str2"
+]
+
+>>> cct.diff("str1", "str2", meta=True)  # show meta data in the first 3 lines.
+[
+    "--- <class 'str'>",
+    "+++ <class 'str'>",
+    "@@ -1 +1 @@",
+    "-str1",
+    "+str2"
+]
+
+
+>>> cct.diff(["a", "b"], ["a", "b", "c"])  # Compare 2 lists and print diffs.
+[
+    "+c"
+]
+
+>>> cct.diff(["a", "b"], ["a", "b", "c"], context=2)  # Show diffs with 2 extra context lines.
+[
+    " a",  # context line
+    " b",  # context line
+    "+c"  # diff
+]
+
+>>> cct.diff("/path/to/file1", "/path/to/file2")  # Compare between 2 files.
+
+>>> cct.diff("/path/to/file1", "str")  # Compare between file and str/list.
+
+>>> cct.diff('str', 'str')  # If no diff, return [].
+[]
+
+>>> cct.update_file('file', 'http://file-url')  # Update file if the file is not as same as url content.
+False  # if already up-to-date.
+
+>>> cct.read_file('file')  # Read file using different encoding automatically.
+"file content"
+
+>>> cct.move_file("/path/to/src", "/path/to/dst")  # Move file from src to dst, overwrite if dst already exists.
+
+>>> cct.move_file("/path/to/src", "/path/to/dst", copy=True)  # Copy file from src to dst.
+
+>>> cct.move_file("/path/to/src", "/path/to/dst", backup=True)  # Backup dst file before move or copy.
+
+>>> cct.move_file("/path/to/src", "/path/to/dst", msgout=print)  # Use `print` to handle output logs.
+
+>>> cct.ajax('http://ajax-url')  # Start a AJAX request.
+{'result': 'data'}  # As python dict.
+
+>>> cct.ajax('http://ajax-url', {'data': 'value'})  # AJAX request with param.
+{'result': 'data'}
+
+>>> cct.ajax('http://ajax-url', method='post')  # AJAX request using post. default is 'get'.
+{'result': 'data'}
+
+>>> if not cct.is_admin():  # Check does the script has admin privileges.
+...     cct.runas_admin(__file__)  # run the script with admin privileges.
+... else:
+...     # your code here
+```
+
+## Updates
+* 2021-01-29 v3.0.0:
+    * Deprecated `image_to_color()`, add `main_color()`.
+        * use `main_color(..., is_url=True)` instead of `image_to_color(...)`
```

### Comparing `consolecmdtools-3.4.1/pyproject.toml` & `consolecmdtools-3.5.1/pyproject.toml`

 * *Files 17% similar despite different names*

```diff
@@ -1,43 +1,43 @@
-[build-system]
-requires = ["setuptools>=61.0.0", "wheel"]
-build-backend = "setuptools.build_meta"
-
-[project]
-name = "consolecmdtools"
-description = "Console command tools in Python"
-requires-python = ">=3.6"
-readme = "README.md"
-keywords = ["python", "console", "command", "tool"]
-license = {text = "LICENSE"}
-classifiers = [
-    "Development Status :: 5 - Production/Stable",
-    "Intended Audience :: Developers",
-    "Topic :: Software Development :: User Interfaces",
-    "License :: OSI Approved :: MIT License",
-    "Programming Language :: Python :: 3",
-    "Programming Language :: Python :: 3 :: Only",
-]
-dependencies = ["consoleiotools"]
-dynamic = ["version"]
-
-[[project.authors]]
-name = "Kyan"
-email = "kai@kyan001.com"
-
-[project.optional-dependencies]
-opt = ["pillow"]
-dev = ["build", "wheel", "pycodestyle"]
-
-[project.urls]
-Homepage = "https://github.com/kyan001/PyConsoleCMDTools"
-"Issue Tracker" = "https://github.com/kyan001/PyConsoleCMDTools/issues"
-"Source Code" = "https://github.com/kyan001/PyConsoleCMDTools"
-
-[tool.setuptools]
-py-modules = ["consolecmdtools"]
-
-[tool.setuptools.dynamic]
-version = {attr = "consolecmdtools.__version__"}
-
-[tool.setuptools.packages.find]
-exclude = ["contrib", "docs", "tests"]
+[build-system]
+requires = ["setuptools>=61.0.0", "wheel"]
+build-backend = "setuptools.build_meta"
+
+[project]
+name = "consolecmdtools"
+description = "Console command tools in Python"
+requires-python = ">=3.6"
+readme = "README.md"
+keywords = ["python", "console", "command", "tool"]
+license = {file = "LICENSE"}
+classifiers = [
+    "Development Status :: 5 - Production/Stable",
+    "Intended Audience :: Developers",
+    "Topic :: Software Development :: User Interfaces",
+    "License :: OSI Approved :: MIT License",
+    "Programming Language :: Python :: 3",
+    "Programming Language :: Python :: 3 :: Only",
+]
+dependencies = ["consoleiotools"]
+dynamic = ["version"]
+
+[[project.authors]]
+name = "Kyan"
+email = "kai@kyan001.com"
+
+[project.optional-dependencies]
+opt = ["pillow"]
+dev = ["build", "wheel", "pycodestyle"]
+
+[project.urls]
+Homepage = "https://github.com/kyan001/PyConsoleCMDTools"
+"Issue Tracker" = "https://github.com/kyan001/PyConsoleCMDTools/issues"
+"Source Code" = "https://github.com/kyan001/PyConsoleCMDTools"
+
+[tool.setuptools]
+py-modules = ["consolecmdtools"]
+
+[tool.setuptools.dynamic]
+version = {attr = "consolecmdtools.__version__"}
+
+[tool.setuptools.packages.find]
+exclude = ["contrib", "docs", "tests"]
```

