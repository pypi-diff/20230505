# Comparing `tmp/tcolorpy-0.1.2.tar.gz` & `tmp/tcolorpy-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tcolorpy-0.1.2.tar", last modified: Sat Feb 26 15:33:56 2022, max compression
+gzip compressed data, was "tcolorpy-0.1.3.tar", last modified: Fri May  5 08:49:54 2023, max compression
```

## Comparing `tcolorpy-0.1.2.tar` & `tcolorpy-0.1.3.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2022-02-26 15:33:56.701723 tcolorpy-0.1.2/
--rw-r--r--   0 toor      (1000) toor      (1000)     1074 2022-02-26 15:33:35.000000 tcolorpy-0.1.2/LICENSE
--rw-r--r--   0 toor      (1000) toor      (1000)      203 2022-02-26 15:33:35.000000 tcolorpy-0.1.2/MANIFEST.in
--rw-r--r--   0 toor      (1000) toor      (1000)     5887 2022-02-26 15:33:56.701723 tcolorpy-0.1.2/PKG-INFO
--rw-r--r--   0 toor      (1000) toor      (1000)     4435 2022-02-26 15:33:35.000000 tcolorpy-0.1.2/README.rst
--rw-r--r--   0 toor      (1000) toor      (1000)     1144 2022-02-26 15:33:35.000000 tcolorpy-0.1.2/pyproject.toml
-drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2022-02-26 15:33:56.701723 tcolorpy-0.1.2/requirements/
--rw-r--r--   0 toor      (1000) toor      (1000)        0 2022-02-26 15:33:35.000000 tcolorpy-0.1.2/requirements/requirements.txt
--rw-r--r--   0 toor      (1000) toor      (1000)       29 2022-02-26 15:33:35.000000 tcolorpy-0.1.2/requirements/test_requirements.txt
--rw-r--r--   0 toor      (1000) toor      (1000)       38 2022-02-26 15:33:56.701723 tcolorpy-0.1.2/setup.cfg
--rw-r--r--   0 toor      (1000) toor      (1000)     2457 2022-02-26 15:33:35.000000 tcolorpy-0.1.2/setup.py
-drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2022-02-26 15:33:56.701723 tcolorpy-0.1.2/tcolorpy/
--rw-r--r--   0 toor      (1000) toor      (1000)      705 2022-02-26 15:33:35.000000 tcolorpy-0.1.2/tcolorpy/__init__.py
--rw-r--r--   0 toor      (1000) toor      (1000)     1702 2022-02-26 15:33:35.000000 tcolorpy-0.1.2/tcolorpy/__main__.py
--rw-r--r--   0 toor      (1000) toor      (1000)      201 2022-02-26 15:33:35.000000 tcolorpy-0.1.2/tcolorpy/__version__.py
--rw-r--r--   0 toor      (1000) toor      (1000)     1080 2022-02-26 15:33:35.000000 tcolorpy-0.1.2/tcolorpy/_const.py
--rw-r--r--   0 toor      (1000) toor      (1000)     7324 2022-02-26 15:33:35.000000 tcolorpy-0.1.2/tcolorpy/_truecolor.py
--rw-r--r--   0 toor      (1000) toor      (1000)        0 2022-02-26 15:33:35.000000 tcolorpy-0.1.2/tcolorpy/py.typed
-drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2022-02-26 15:33:56.701723 tcolorpy-0.1.2/tcolorpy.egg-info/
--rw-r--r--   0 toor      (1000) toor      (1000)     5887 2022-02-26 15:33:56.000000 tcolorpy-0.1.2/tcolorpy.egg-info/PKG-INFO
--rw-r--r--   0 toor      (1000) toor      (1000)      485 2022-02-26 15:33:56.000000 tcolorpy-0.1.2/tcolorpy.egg-info/SOURCES.txt
--rw-r--r--   0 toor      (1000) toor      (1000)        1 2022-02-26 15:33:56.000000 tcolorpy-0.1.2/tcolorpy.egg-info/dependency_links.txt
--rw-r--r--   0 toor      (1000) toor      (1000)        1 2022-02-26 15:33:35.000000 tcolorpy-0.1.2/tcolorpy.egg-info/not-zip-safe
--rw-r--r--   0 toor      (1000) toor      (1000)       37 2022-02-26 15:33:56.000000 tcolorpy-0.1.2/tcolorpy.egg-info/requires.txt
--rw-r--r--   0 toor      (1000) toor      (1000)        9 2022-02-26 15:33:56.000000 tcolorpy-0.1.2/tcolorpy.egg-info/top_level.txt
-drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2022-02-26 15:33:56.701723 tcolorpy-0.1.2/test/
--rw-r--r--   0 toor      (1000) toor      (1000)     2784 2022-02-26 15:33:35.000000 tcolorpy-0.1.2/test/test_color.py
--rw-r--r--   0 toor      (1000) toor      (1000)     3432 2022-02-26 15:33:35.000000 tcolorpy-0.1.2/test/test_truecolor.py
--rw-r--r--   0 toor      (1000) toor      (1000)     1029 2022-02-26 15:33:35.000000 tcolorpy-0.1.2/tox.ini
+drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2023-05-05 08:49:54.913649 tcolorpy-0.1.3/
+-rw-r--r--   0 toor      (1000) toor      (1000)     1074 2023-05-05 08:49:37.000000 tcolorpy-0.1.3/LICENSE
+-rw-r--r--   0 toor      (1000) toor      (1000)      203 2023-05-05 08:49:37.000000 tcolorpy-0.1.3/MANIFEST.in
+-rw-r--r--   0 toor      (1000) toor      (1000)     5610 2023-05-05 08:49:54.913649 tcolorpy-0.1.3/PKG-INFO
+-rw-r--r--   0 toor      (1000) toor      (1000)     4177 2023-05-05 08:49:37.000000 tcolorpy-0.1.3/README.rst
+-rw-r--r--   0 toor      (1000) toor      (1000)     1145 2023-05-05 08:49:37.000000 tcolorpy-0.1.3/pyproject.toml
+drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2023-05-05 08:49:54.903649 tcolorpy-0.1.3/requirements/
+-rw-r--r--   0 toor      (1000) toor      (1000)        0 2023-05-05 08:49:37.000000 tcolorpy-0.1.3/requirements/requirements.txt
+-rw-r--r--   0 toor      (1000) toor      (1000)       29 2023-05-05 08:49:37.000000 tcolorpy-0.1.3/requirements/test_requirements.txt
+-rw-r--r--   0 toor      (1000) toor      (1000)       38 2023-05-05 08:49:54.913649 tcolorpy-0.1.3/setup.cfg
+-rw-r--r--   0 toor      (1000) toor      (1000)     2470 2023-05-05 08:49:37.000000 tcolorpy-0.1.3/setup.py
+drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2023-05-05 08:49:54.903649 tcolorpy-0.1.3/tcolorpy/
+-rw-r--r--   0 toor      (1000) toor      (1000)      705 2023-05-05 08:49:37.000000 tcolorpy-0.1.3/tcolorpy/__init__.py
+-rw-r--r--   0 toor      (1000) toor      (1000)     1701 2023-05-05 08:49:37.000000 tcolorpy-0.1.3/tcolorpy/__main__.py
+-rw-r--r--   0 toor      (1000) toor      (1000)      201 2023-05-05 08:49:37.000000 tcolorpy-0.1.3/tcolorpy/__version__.py
+-rw-r--r--   0 toor      (1000) toor      (1000)     1080 2023-05-05 08:49:37.000000 tcolorpy-0.1.3/tcolorpy/_const.py
+-rw-r--r--   0 toor      (1000) toor      (1000)     7324 2023-05-05 08:49:37.000000 tcolorpy-0.1.3/tcolorpy/_truecolor.py
+-rw-r--r--   0 toor      (1000) toor      (1000)        0 2023-05-05 08:49:37.000000 tcolorpy-0.1.3/tcolorpy/py.typed
+drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2023-05-05 08:49:54.903649 tcolorpy-0.1.3/tcolorpy.egg-info/
+-rw-r--r--   0 toor      (1000) toor      (1000)     5610 2023-05-05 08:49:54.000000 tcolorpy-0.1.3/tcolorpy.egg-info/PKG-INFO
+-rw-r--r--   0 toor      (1000) toor      (1000)      485 2023-05-05 08:49:54.000000 tcolorpy-0.1.3/tcolorpy.egg-info/SOURCES.txt
+-rw-r--r--   0 toor      (1000) toor      (1000)        1 2023-05-05 08:49:54.000000 tcolorpy-0.1.3/tcolorpy.egg-info/dependency_links.txt
+-rw-r--r--   0 toor      (1000) toor      (1000)        1 2023-05-05 08:49:47.000000 tcolorpy-0.1.3/tcolorpy.egg-info/not-zip-safe
+-rw-r--r--   0 toor      (1000) toor      (1000)       37 2023-05-05 08:49:54.000000 tcolorpy-0.1.3/tcolorpy.egg-info/requires.txt
+-rw-r--r--   0 toor      (1000) toor      (1000)        9 2023-05-05 08:49:54.000000 tcolorpy-0.1.3/tcolorpy.egg-info/top_level.txt
+drwxr-xr-x   0 toor      (1000) toor      (1000)        0 2023-05-05 08:49:54.903649 tcolorpy-0.1.3/test/
+-rw-r--r--   0 toor      (1000) toor      (1000)     2784 2023-05-05 08:49:37.000000 tcolorpy-0.1.3/test/test_color.py
+-rw-r--r--   0 toor      (1000) toor      (1000)     3432 2023-05-05 08:49:37.000000 tcolorpy-0.1.3/test/test_truecolor.py
+-rw-r--r--   0 toor      (1000) toor      (1000)      966 2023-05-05 08:49:37.000000 tcolorpy-0.1.3/tox.ini
```

### Comparing `tcolorpy-0.1.2/LICENSE` & `tcolorpy-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `tcolorpy-0.1.2/PKG-INFO` & `tcolorpy-0.1.3/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,37 +1,36 @@
 Metadata-Version: 2.1
 Name: tcolorpy
-Version: 0.1.2
+Version: 0.1.3
 Summary: tcolopy is a Python library to apply true color for terminal text.
 Home-page: https://github.com/thombashi/tcolorpy
 Author: Tsuyoshi Hombashi
 Author-email: tsuyoshi.hombashi@gmail.com
 License: MIT License
 Project-URL: Source, https://github.com/thombashi/tcolorpy
 Project-URL: Tracker, https://github.com/thombashi/tcolorpy/issues
 Keywords: ANSI escape,terminal color,truecolor
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Information Technology
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Terminals
 Classifier: Topic :: Text Processing
-Requires-Python: >=3.6
+Requires-Python: >=3.7
 Description-Content-Type: text/x-rst
 Provides-Extra: test
 License-File: LICENSE
 
 .. contents:: **tcolorpy**
    :backlinks: top
    :depth: 2
@@ -99,30 +98,30 @@
     .. figure:: https://cdn.jsdelivr.net/gh/thombashi/tcolorpy@master/ss/oneline.png
         :scale: 60%
         :alt: https://github.com/thombashi/tcolorpy/blob/master/ss/oneline.png
 
 You can set the following ``tcolor`` arguments:
 
 - ``color``/``bg_color``
-    - color names (``"red"``, ``"red"``, etc.) or color code (``"#RRGGBB"``)
+    - color names (``"red"``, ``"green"``, etc.) or color code (``"#RRGGBB"``)
 - ``styles``
     - ``"bold"``, ``"italic"``, etc.
 
 
 Other examples
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 Apply true color and styles to text:
 
 .. figure:: https://cdn.jsdelivr.net/gh/thombashi/tcolorpy@master/ss/styles.png
     :scale: 60%
     :alt: https://github.com/thombashi/tcolorpy/blob/master/ss/styles.png
 
     `example source code <https://github.com/thombashi/tcolorpy/blob/master/examples/ansi_styles.py>`__
 
-You can also specify colors by names:
+You can also specify colors by name:
 
 .. figure:: https://cdn.jsdelivr.net/gh/thombashi/tcolorpy@master/ss/ansi_colors.png
     :scale: 60%
     :alt: https://github.com/thombashi/tcolorpy/blob/master/ss/ansi_colors.png
 
     `example source code <https://github.com/thombashi/tcolorpy/blob/master/examples/ansi_colors.py>`__
 
@@ -135,38 +134,27 @@
 
     $ python3 -m tcolorpy "tcolopy example" -c "#ee1177" -s bold,italic,underline
 
 Command help
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 ::
 
-    usage: __main__.py [-h] [-c COLOR] [-b BG_COLOR] [-s STYLES] [--encode ENCODE]
-                       string
+    usage: __main__.py [-h] [-c COLOR] [-b BG_COLOR] [-s STYLES] [--encode ENCODE] string
 
     positional arguments:
       string                string to apply styles.
 
-    optional arguments:
+    options:
       -h, --help            show this help message and exit
       -c COLOR, --color COLOR
-                            specify a color code (#XXXXXX) or a name. valid names
-                            are: black, red, green, yellow, blue, magenta, cyan,
-                            white, lightblack, lightred, lightgreen, lightyellow,
-                            lightblue, lightmagenta, lightcyan, lightwhite
+                            specify a color code (#XXXXXX) or a name. valid names are: black, red, green, yellow, blue, magenta, cyan, white, lightblack, lightred, lightgreen, lightyellow, lightblue, lightmagenta, lightcyan, lightwhite
       -b BG_COLOR, --bg-color BG_COLOR
-                            specify a background color code (#XXXXXX) or a name.
-                            valid names are: black, red, green, yellow, blue,
-                            magenta, cyan, white, lightblack, lightred,
-                            lightgreen, lightyellow, lightblue, lightmagenta,
-                            lightcyan, lightwhite
+                            specify a background color code (#XXXXXX) or a name. valid names are: black, red, green, yellow, blue, magenta, cyan, white, lightblack, lightred, lightgreen, lightyellow, lightblue, lightmagenta, lightcyan, lightwhite
       -s STYLES, --styles STYLES
-                            specify a comma separated styles. valid values are:
-                            bold, dim, italic, underline, blink, invert, strike
+                            specify a comma-separated style. valid values are: bold, dim, italic, underline, blink, invert, strike
       --encode ENCODE       output a text encoded with the specified encoding
 
 
 Dependencies
 ============================================
-Python 3.6+
+Python 3.7+
 no external dependencies.
-
-
```

### Comparing `tcolorpy-0.1.2/README.rst` & `tcolorpy-0.1.3/README.rst`

 * *Files 3% similar despite different names*

```diff
@@ -65,30 +65,30 @@
     .. figure:: https://cdn.jsdelivr.net/gh/thombashi/tcolorpy@master/ss/oneline.png
         :scale: 60%
         :alt: https://github.com/thombashi/tcolorpy/blob/master/ss/oneline.png
 
 You can set the following ``tcolor`` arguments:
 
 - ``color``/``bg_color``
-    - color names (``"red"``, ``"red"``, etc.) or color code (``"#RRGGBB"``)
+    - color names (``"red"``, ``"green"``, etc.) or color code (``"#RRGGBB"``)
 - ``styles``
     - ``"bold"``, ``"italic"``, etc.
 
 
 Other examples
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 Apply true color and styles to text:
 
 .. figure:: https://cdn.jsdelivr.net/gh/thombashi/tcolorpy@master/ss/styles.png
     :scale: 60%
     :alt: https://github.com/thombashi/tcolorpy/blob/master/ss/styles.png
 
     `example source code <https://github.com/thombashi/tcolorpy/blob/master/examples/ansi_styles.py>`__
 
-You can also specify colors by names:
+You can also specify colors by name:
 
 .. figure:: https://cdn.jsdelivr.net/gh/thombashi/tcolorpy@master/ss/ansi_colors.png
     :scale: 60%
     :alt: https://github.com/thombashi/tcolorpy/blob/master/ss/ansi_colors.png
 
     `example source code <https://github.com/thombashi/tcolorpy/blob/master/examples/ansi_colors.py>`__
 
@@ -101,36 +101,27 @@
 
     $ python3 -m tcolorpy "tcolopy example" -c "#ee1177" -s bold,italic,underline
 
 Command help
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 ::
 
-    usage: __main__.py [-h] [-c COLOR] [-b BG_COLOR] [-s STYLES] [--encode ENCODE]
-                       string
+    usage: __main__.py [-h] [-c COLOR] [-b BG_COLOR] [-s STYLES] [--encode ENCODE] string
 
     positional arguments:
       string                string to apply styles.
 
-    optional arguments:
+    options:
       -h, --help            show this help message and exit
       -c COLOR, --color COLOR
-                            specify a color code (#XXXXXX) or a name. valid names
-                            are: black, red, green, yellow, blue, magenta, cyan,
-                            white, lightblack, lightred, lightgreen, lightyellow,
-                            lightblue, lightmagenta, lightcyan, lightwhite
+                            specify a color code (#XXXXXX) or a name. valid names are: black, red, green, yellow, blue, magenta, cyan, white, lightblack, lightred, lightgreen, lightyellow, lightblue, lightmagenta, lightcyan, lightwhite
       -b BG_COLOR, --bg-color BG_COLOR
-                            specify a background color code (#XXXXXX) or a name.
-                            valid names are: black, red, green, yellow, blue,
-                            magenta, cyan, white, lightblack, lightred,
-                            lightgreen, lightyellow, lightblue, lightmagenta,
-                            lightcyan, lightwhite
+                            specify a background color code (#XXXXXX) or a name. valid names are: black, red, green, yellow, blue, magenta, cyan, white, lightblack, lightred, lightgreen, lightyellow, lightblue, lightmagenta, lightcyan, lightwhite
       -s STYLES, --styles STYLES
-                            specify a comma separated styles. valid values are:
-                            bold, dim, italic, underline, blink, invert, strike
+                            specify a comma-separated style. valid values are: bold, dim, italic, underline, blink, invert, strike
       --encode ENCODE       output a text encoded with the specified encoding
 
 
 Dependencies
 ============================================
-Python 3.6+
+Python 3.7+
 no external dependencies.
```

### Comparing `tcolorpy-0.1.2/pyproject.toml` & `tcolorpy-0.1.3/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -14,15 +14,15 @@
     | _build
     | buck-out
     | build
     | dist
 )/
 | docs/conf.py
 '''
-target-version = ['py36', 'py37', 'py38', 'py39', 'py310']
+target-version = ['py37', 'py38', 'py39', 'py310', 'py311']
 
 [tool.coverage.run]
 source = ['tcolorpy']
 branch = true
 
 [tool.coverage.report]
 show_missing = true
@@ -50,15 +50,15 @@
     '*/.eggs/*',
     '*/.pytype/*',
     '*/.tox/*',
 ]
 
 [tool.mypy]
 ignore_missing_imports = true
-python_version = 3.6
+python_version = 3.7
 
 pretty = true
 show_error_codes = true
 show_error_context = true
 warn_unreachable = true
 warn_unused_configs = true
```

### Comparing `tcolorpy-0.1.2/setup.py` & `tcolorpy-0.1.3/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 import os.path
-from typing import Dict
+from typing import Dict, Type
 
 import setuptools
 
 
 MODULE_NAME = "tcolorpy"
 REPOSITORY_URL = f"https://github.com/thombashi/{MODULE_NAME:s}"
 REQUIREMENT_DIR = "requirements"
 
 pkg_info: Dict[str, str] = {}
 
 
-def get_release_command_class() -> Dict[str, setuptools.Command]:
+def get_release_command_class() -> Dict[str, Type[setuptools.Command]]:
     try:
         from releasecmd import ReleaseCommand
     except ImportError:
         return {}
 
     return {"release": ReleaseCommand}
 
@@ -43,27 +43,27 @@
     long_description_content_type="text/x-rst",
     packages=setuptools.find_packages(exclude=["test*"]),
     package_data={MODULE_NAME: ["py.typed"]},
     project_urls={
         "Source": REPOSITORY_URL,
         "Tracker": f"{REPOSITORY_URL:s}/issues",
     },
-    python_requires=">=3.6",
+    python_requires=">=3.7",
     extras_require={"test": TESTS_REQUIRES},
     classifiers=[
         "Development Status :: 4 - Beta",
         "Intended Audience :: Information Technology",
         "License :: OSI Approved :: MIT License",
         "Operating System :: OS Independent",
         "Programming Language :: Python :: 3",
-        "Programming Language :: Python :: 3.6",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
         "Programming Language :: Python :: 3 :: Only",
         "Programming Language :: Python :: Implementation :: CPython",
         "Programming Language :: Python :: Implementation :: PyPy",
         "Topic :: Software Development :: Libraries",
         "Topic :: Software Development :: Libraries :: Python Modules",
         "Topic :: Terminals",
         "Topic :: Text Processing",
```

### Comparing `tcolorpy-0.1.2/tcolorpy/__init__.py` & `tcolorpy-0.1.3/tcolorpy/__init__.py`

 * *Files identical despite different names*

### Comparing `tcolorpy-0.1.2/tcolorpy/__main__.py` & `tcolorpy-0.1.3/tcolorpy/__main__.py`

 * *Files 2% similar despite different names*

```diff
@@ -22,15 +22,15 @@
         help="specify a background color code (#XXXXXX) or a name. valid names are: {}".format(
             ", ".join([style.name.lower() for style in list(AnsiBGColor)])
         ),
     )
     parser.add_argument(
         "-s",
         "--styles",
-        help="specify a comma separated styles. valid values are: {}".format(
+        help="specify a comma-separated style. valid values are: {}".format(
             ", ".join([style.name.lower() for style in list(AnsiStyle)])
         ),
     )
     parser.add_argument(
         "--encode",
         help="output a text encoded with the specified encoding",
     )
```

### Comparing `tcolorpy-0.1.2/tcolorpy/_const.py` & `tcolorpy-0.1.3/tcolorpy/_const.py`

 * *Files identical despite different names*

### Comparing `tcolorpy-0.1.2/tcolorpy/_truecolor.py` & `tcolorpy-0.1.3/tcolorpy/_truecolor.py`

 * *Files identical despite different names*

### Comparing `tcolorpy-0.1.2/tcolorpy.egg-info/PKG-INFO` & `tcolorpy-0.1.3/tcolorpy.egg-info/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,37 +1,36 @@
 Metadata-Version: 2.1
 Name: tcolorpy
-Version: 0.1.2
+Version: 0.1.3
 Summary: tcolopy is a Python library to apply true color for terminal text.
 Home-page: https://github.com/thombashi/tcolorpy
 Author: Tsuyoshi Hombashi
 Author-email: tsuyoshi.hombashi@gmail.com
 License: MIT License
 Project-URL: Source, https://github.com/thombashi/tcolorpy
 Project-URL: Tracker, https://github.com/thombashi/tcolorpy/issues
 Keywords: ANSI escape,terminal color,truecolor
-Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: Information Technology
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Terminals
 Classifier: Topic :: Text Processing
-Requires-Python: >=3.6
+Requires-Python: >=3.7
 Description-Content-Type: text/x-rst
 Provides-Extra: test
 License-File: LICENSE
 
 .. contents:: **tcolorpy**
    :backlinks: top
    :depth: 2
@@ -99,30 +98,30 @@
     .. figure:: https://cdn.jsdelivr.net/gh/thombashi/tcolorpy@master/ss/oneline.png
         :scale: 60%
         :alt: https://github.com/thombashi/tcolorpy/blob/master/ss/oneline.png
 
 You can set the following ``tcolor`` arguments:
 
 - ``color``/``bg_color``
-    - color names (``"red"``, ``"red"``, etc.) or color code (``"#RRGGBB"``)
+    - color names (``"red"``, ``"green"``, etc.) or color code (``"#RRGGBB"``)
 - ``styles``
     - ``"bold"``, ``"italic"``, etc.
 
 
 Other examples
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 Apply true color and styles to text:
 
 .. figure:: https://cdn.jsdelivr.net/gh/thombashi/tcolorpy@master/ss/styles.png
     :scale: 60%
     :alt: https://github.com/thombashi/tcolorpy/blob/master/ss/styles.png
 
     `example source code <https://github.com/thombashi/tcolorpy/blob/master/examples/ansi_styles.py>`__
 
-You can also specify colors by names:
+You can also specify colors by name:
 
 .. figure:: https://cdn.jsdelivr.net/gh/thombashi/tcolorpy@master/ss/ansi_colors.png
     :scale: 60%
     :alt: https://github.com/thombashi/tcolorpy/blob/master/ss/ansi_colors.png
 
     `example source code <https://github.com/thombashi/tcolorpy/blob/master/examples/ansi_colors.py>`__
 
@@ -135,38 +134,27 @@
 
     $ python3 -m tcolorpy "tcolopy example" -c "#ee1177" -s bold,italic,underline
 
 Command help
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 ::
 
-    usage: __main__.py [-h] [-c COLOR] [-b BG_COLOR] [-s STYLES] [--encode ENCODE]
-                       string
+    usage: __main__.py [-h] [-c COLOR] [-b BG_COLOR] [-s STYLES] [--encode ENCODE] string
 
     positional arguments:
       string                string to apply styles.
 
-    optional arguments:
+    options:
       -h, --help            show this help message and exit
       -c COLOR, --color COLOR
-                            specify a color code (#XXXXXX) or a name. valid names
-                            are: black, red, green, yellow, blue, magenta, cyan,
-                            white, lightblack, lightred, lightgreen, lightyellow,
-                            lightblue, lightmagenta, lightcyan, lightwhite
+                            specify a color code (#XXXXXX) or a name. valid names are: black, red, green, yellow, blue, magenta, cyan, white, lightblack, lightred, lightgreen, lightyellow, lightblue, lightmagenta, lightcyan, lightwhite
       -b BG_COLOR, --bg-color BG_COLOR
-                            specify a background color code (#XXXXXX) or a name.
-                            valid names are: black, red, green, yellow, blue,
-                            magenta, cyan, white, lightblack, lightred,
-                            lightgreen, lightyellow, lightblue, lightmagenta,
-                            lightcyan, lightwhite
+                            specify a background color code (#XXXXXX) or a name. valid names are: black, red, green, yellow, blue, magenta, cyan, white, lightblack, lightred, lightgreen, lightyellow, lightblue, lightmagenta, lightcyan, lightwhite
       -s STYLES, --styles STYLES
-                            specify a comma separated styles. valid values are:
-                            bold, dim, italic, underline, blink, invert, strike
+                            specify a comma-separated style. valid values are: bold, dim, italic, underline, blink, invert, strike
       --encode ENCODE       output a text encoded with the specified encoding
 
 
 Dependencies
 ============================================
-Python 3.6+
+Python 3.7+
 no external dependencies.
-
-
```

### Comparing `tcolorpy-0.1.2/test/test_color.py` & `tcolorpy-0.1.3/test/test_color.py`

 * *Files identical despite different names*

### Comparing `tcolorpy-0.1.2/test/test_truecolor.py` & `tcolorpy-0.1.3/test/test_truecolor.py`

 * *Files identical despite different names*

