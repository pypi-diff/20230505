# Comparing `tmp/prettynumbers-0.1.3.tar.gz` & `tmp/prettynumbers-0.1.3b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "prettynumbers-0.1.3.tar", last modified: Fri May  5 16:18:52 2023, max compression
+gzip compressed data, was "prettynumbers-0.1.3b0.tar", last modified: Fri May  5 16:12:24 2023, max compression
```

## Comparing `prettynumbers-0.1.3.tar` & `prettynumbers-0.1.3b0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-05 16:18:52.185101 prettynumbers-0.1.3/
--rw-r--r--   0 circleci  (1001) circleci  (1002)    14849 2023-05-05 16:18:21.000000 prettynumbers-0.1.3/LICENSE.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)       65 2023-05-05 16:18:21.000000 prettynumbers-0.1.3/MANIFEST.in
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1049 2023-05-05 16:18:52.185101 prettynumbers-0.1.3/PKG-INFO
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1199 2023-05-05 16:18:21.000000 prettynumbers-0.1.3/README.md
--rw-r--r--   0 circleci  (1001) circleci  (1002)      500 2023-05-05 16:18:21.000000 prettynumbers-0.1.3/README.rst
--rwxr-xr-x   0 circleci  (1001) circleci  (1002)     1991 2023-05-05 16:18:21.000000 prettynumbers-0.1.3/pretty_numbers.py
-drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-05 16:18:52.185101 prettynumbers-0.1.3/prettynumbers.egg-info/
--rw-r--r--   0 circleci  (1001) circleci  (1002)     1049 2023-05-05 16:18:52.000000 prettynumbers-0.1.3/prettynumbers.egg-info/PKG-INFO
--rw-r--r--   0 circleci  (1001) circleci  (1002)      244 2023-05-05 16:18:52.000000 prettynumbers-0.1.3/prettynumbers.egg-info/SOURCES.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2023-05-05 16:18:52.000000 prettynumbers-0.1.3/prettynumbers.egg-info/dependency_links.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)       15 2023-05-05 16:18:52.000000 prettynumbers-0.1.3/prettynumbers.egg-info/top_level.txt
--rw-r--r--   0 circleci  (1001) circleci  (1002)      488 2023-05-05 16:18:21.000000 prettynumbers-0.1.3/pyproject.toml
--rw-r--r--   0 circleci  (1001) circleci  (1002)       67 2023-05-05 16:18:52.185101 prettynumbers-0.1.3/setup.cfg
--rw-r--r--   0 circleci  (1001) circleci  (1002)      930 2023-05-05 16:18:21.000000 prettynumbers-0.1.3/setup.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-05 16:12:24.888012 prettynumbers-0.1.3b0/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)    14849 2023-05-05 16:12:20.000000 prettynumbers-0.1.3b0/LICENSE.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       65 2023-05-05 16:12:20.000000 prettynumbers-0.1.3b0/MANIFEST.in
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1052 2023-05-05 16:12:24.888012 prettynumbers-0.1.3b0/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1199 2023-05-05 16:12:20.000000 prettynumbers-0.1.3b0/README.md
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      500 2023-05-05 16:12:20.000000 prettynumbers-0.1.3b0/README.rst
+-rwxr-xr-x   0 circleci  (1001) circleci  (1002)     1991 2023-05-05 16:12:20.000000 prettynumbers-0.1.3b0/pretty_numbers.py
+drwxr-xr-x   0 circleci  (1001) circleci  (1002)        0 2023-05-05 16:12:24.888012 prettynumbers-0.1.3b0/prettynumbers.egg-info/
+-rw-r--r--   0 circleci  (1001) circleci  (1002)     1052 2023-05-05 16:12:24.000000 prettynumbers-0.1.3b0/prettynumbers.egg-info/PKG-INFO
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      244 2023-05-05 16:12:24.000000 prettynumbers-0.1.3b0/prettynumbers.egg-info/SOURCES.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)        1 2023-05-05 16:12:24.000000 prettynumbers-0.1.3b0/prettynumbers.egg-info/dependency_links.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       15 2023-05-05 16:12:24.000000 prettynumbers-0.1.3b0/prettynumbers.egg-info/top_level.txt
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      488 2023-05-05 16:12:20.000000 prettynumbers-0.1.3b0/pyproject.toml
+-rw-r--r--   0 circleci  (1001) circleci  (1002)       67 2023-05-05 16:12:24.892012 prettynumbers-0.1.3b0/setup.cfg
+-rw-r--r--   0 circleci  (1001) circleci  (1002)      931 2023-05-05 16:12:20.000000 prettynumbers-0.1.3b0/setup.py
```

### Comparing `prettynumbers-0.1.3/LICENSE.txt` & `prettynumbers-0.1.3b0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `prettynumbers-0.1.3/PKG-INFO` & `prettynumbers-0.1.3b0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: prettynumbers
-Version: 0.1.3
+Version: 0.1.3b0
 Summary: Display a range of numbers in a human readable way
 Home-page: https://github.com/vfxGer/pretty-numbers
 Author: Gerard Keating
 Author-email: gerardk@gmail.com
 License: GNU GENERAL PUBLIC LICENSE
-Download-URL: https://pypi.python.org/packages/source/d/pretty_numbers-0.1.3.tar.gz?raw=true
+Download-URL: https://pypi.python.org/packages/source/d/pretty_numbers-0.1.3b.tar.gz?raw=true
 Description: |Build Status| |codecov.io| |Code Climate|
         
         .. |Build Status| image:: https://travis-ci.org/vfxGer/pretty-numbers.svg?branch=master
            :target: https://travis-ci.org/vfxGer/pretty-numbers
         .. |codecov.io| image:: https://codecov.io/gh/vfxGer/pretty-numbers/coverage.svg?branch=master
            :target: https://codecov.io/gh/vfxGer/pretty-numbers
         .. |Code Climate| image:: https://codeclimate.com/github/vfxGer/pretty-numbers/badges/gpa.svg
```

### Comparing `prettynumbers-0.1.3/README.md` & `prettynumbers-0.1.3b0/README.md`

 * *Files identical despite different names*

### Comparing `prettynumbers-0.1.3/pretty_numbers.py` & `prettynumbers-0.1.3b0/pretty_numbers.py`

 * *Files identical despite different names*

### Comparing `prettynumbers-0.1.3/prettynumbers.egg-info/PKG-INFO` & `prettynumbers-0.1.3b0/prettynumbers.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: prettynumbers
-Version: 0.1.3
+Version: 0.1.3b0
 Summary: Display a range of numbers in a human readable way
 Home-page: https://github.com/vfxGer/pretty-numbers
 Author: Gerard Keating
 Author-email: gerardk@gmail.com
 License: GNU GENERAL PUBLIC LICENSE
-Download-URL: https://pypi.python.org/packages/source/d/pretty_numbers-0.1.3.tar.gz?raw=true
+Download-URL: https://pypi.python.org/packages/source/d/pretty_numbers-0.1.3b.tar.gz?raw=true
 Description: |Build Status| |codecov.io| |Code Climate|
         
         .. |Build Status| image:: https://travis-ci.org/vfxGer/pretty-numbers.svg?branch=master
            :target: https://travis-ci.org/vfxGer/pretty-numbers
         .. |codecov.io| image:: https://codecov.io/gh/vfxGer/pretty-numbers/coverage.svg?branch=master
            :target: https://codecov.io/gh/vfxGer/pretty-numbers
         .. |Code Climate| image:: https://codeclimate.com/github/vfxGer/pretty-numbers/badges/gpa.svg
```

### Comparing `prettynumbers-0.1.3/setup.py` & `prettynumbers-0.1.3b0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # based on https://github.com/pypa/sampleproject/blob/master/setup.py
 from setuptools import setup
 from os import path
 
 here = path.abspath(path.dirname(__file__))
 
-version = "0.1.3"
+version = "0.1.3b"
 
 # Get the long description from the README file
 with open(path.join(here, "README.rst")) as f:
     long_description = f.read()
 
 setup(
     name="prettynumbers",
```

