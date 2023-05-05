# Comparing `tmp/prettynumbers-0.1.0.tar.gz` & `tmp/prettynumbers-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/prettynumbers-0.1.0.tar", last modified: Fri Nov 26 11:42:30 2021, max compression
+gzip compressed data, was "prettynumbers-0.1.1.tar", last modified: Fri May  5 15:07:48 2023, max compression
```

## Comparing `prettynumbers-0.1.0.tar` & `prettynumbers-0.1.1.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 gerardkeating   (501) staff       (20)        0 2021-11-26 11:42:30.484497 prettynumbers-0.1.0/
--rw-r--r--   0 gerardkeating   (501) staff       (20)    14849 2021-10-22 10:26:22.000000 prettynumbers-0.1.0/LICENSE.txt
--rw-r--r--   0 gerardkeating   (501) staff       (20)       65 2021-10-22 10:26:22.000000 prettynumbers-0.1.0/MANIFEST.in
--rw-r--r--   0 gerardkeating   (501) staff       (20)      992 2021-11-26 11:42:30.484620 prettynumbers-0.1.0/PKG-INFO
--rw-r--r--   0 gerardkeating   (501) staff       (20)     1199 2021-10-22 10:26:22.000000 prettynumbers-0.1.0/README.md
--rw-r--r--   0 gerardkeating   (501) staff       (20)      500 2021-10-22 10:26:22.000000 prettynumbers-0.1.0/README.rst
--rwxr-xr-x   0 gerardkeating   (501) staff       (20)     1991 2021-11-26 11:17:29.000000 prettynumbers-0.1.0/pretty_numbers.py
-drwxr-xr-x   0 gerardkeating   (501) staff       (20)        0 2021-11-26 11:42:30.484245 prettynumbers-0.1.0/prettynumbers.egg-info/
--rw-r--r--   0 gerardkeating   (501) staff       (20)      992 2021-11-26 11:42:30.000000 prettynumbers-0.1.0/prettynumbers.egg-info/PKG-INFO
--rw-r--r--   0 gerardkeating   (501) staff       (20)      244 2021-11-26 11:42:30.000000 prettynumbers-0.1.0/prettynumbers.egg-info/SOURCES.txt
--rw-r--r--   0 gerardkeating   (501) staff       (20)        1 2021-11-26 11:42:30.000000 prettynumbers-0.1.0/prettynumbers.egg-info/dependency_links.txt
--rw-r--r--   0 gerardkeating   (501) staff       (20)       15 2021-11-26 11:42:30.000000 prettynumbers-0.1.0/prettynumbers.egg-info/top_level.txt
--rw-r--r--   0 gerardkeating   (501) staff       (20)      404 2021-11-26 11:22:38.000000 prettynumbers-0.1.0/pyproject.toml
--rw-r--r--   0 gerardkeating   (501) staff       (20)       67 2021-11-26 11:42:30.485718 prettynumbers-0.1.0/setup.cfg
--rw-r--r--   0 gerardkeating   (501) staff       (20)      930 2021-11-26 11:41:42.000000 prettynumbers-0.1.0/setup.py
+drwxr-xr-x   0 gerardk    (501) staff       (20)        0 2023-05-05 15:07:48.718307 prettynumbers-0.1.1/
+-rw-r--r--   0 gerardk    (501) staff       (20)    14849 2016-07-14 20:10:07.000000 prettynumbers-0.1.1/LICENSE.txt
+-rw-r--r--   0 gerardk    (501) staff       (20)       65 2016-09-02 20:23:13.000000 prettynumbers-0.1.1/MANIFEST.in
+-rw-r--r--   0 gerardk    (501) staff       (20)      990 2023-05-05 15:07:48.719258 prettynumbers-0.1.1/PKG-INFO
+-rw-r--r--   0 gerardk    (501) staff       (20)     1199 2023-05-05 08:09:26.000000 prettynumbers-0.1.1/README.md
+-rw-r--r--   0 gerardk    (501) staff       (20)      500 2016-09-04 11:25:13.000000 prettynumbers-0.1.1/README.rst
+-rwxr-xr-x   0 gerardk    (501) staff       (20)     1991 2023-05-05 08:09:26.000000 prettynumbers-0.1.1/pretty_numbers.py
+drwxr-xr-x   0 gerardk    (501) staff       (20)        0 2023-05-05 15:07:48.715740 prettynumbers-0.1.1/prettynumbers.egg-info/
+-rw-r--r--   0 gerardk    (501) staff       (20)      990 2023-05-05 15:07:48.000000 prettynumbers-0.1.1/prettynumbers.egg-info/PKG-INFO
+-rw-r--r--   0 gerardk    (501) staff       (20)      244 2023-05-05 15:07:48.000000 prettynumbers-0.1.1/prettynumbers.egg-info/SOURCES.txt
+-rw-r--r--   0 gerardk    (501) staff       (20)        1 2023-05-05 15:07:48.000000 prettynumbers-0.1.1/prettynumbers.egg-info/dependency_links.txt
+-rw-r--r--   0 gerardk    (501) staff       (20)       15 2023-05-05 15:07:48.000000 prettynumbers-0.1.1/prettynumbers.egg-info/top_level.txt
+-rw-r--r--   0 gerardk    (501) staff       (20)      488 2023-05-05 14:55:22.000000 prettynumbers-0.1.1/pyproject.toml
+-rw-r--r--   0 gerardk    (501) staff       (20)       67 2023-05-05 15:07:48.720541 prettynumbers-0.1.1/setup.cfg
+-rw-r--r--   0 gerardk    (501) staff       (20)      930 2023-05-05 14:51:35.000000 prettynumbers-0.1.1/setup.py
```

### Comparing `prettynumbers-0.1.0/LICENSE.txt` & `prettynumbers-0.1.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `prettynumbers-0.1.0/PKG-INFO` & `prettynumbers-0.1.1/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,25 +1,23 @@
 Metadata-Version: 2.1
 Name: prettynumbers
-Version: 0.1.0
+Version: 0.1.1
 Summary: Display a range of numbers in a human readable way
 Home-page: https://github.com/vfxGer/pretty-numbers
+Download-URL: https://pypi.python.org/packages/source/d/pretty_numbers-0.1.1.tar.gz?raw=true
 Author: Gerard Keating
 Author-email: gerardk@gmail.com
 License: GNU GENERAL PUBLIC LICENSE
-Download-URL: https://pypi.python.org/packages/source/d/pretty_numbers-0.1.0.tar.gz?raw=true
 Platform: Cross-platform
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/x-rst
 License-File: LICENSE.txt
 
 |Build Status| |codecov.io| |Code Climate|
 
 .. |Build Status| image:: https://travis-ci.org/vfxGer/pretty-numbers.svg?branch=master
    :target: https://travis-ci.org/vfxGer/pretty-numbers
 .. |codecov.io| image:: https://codecov.io/gh/vfxGer/pretty-numbers/coverage.svg?branch=master
    :target: https://codecov.io/gh/vfxGer/pretty-numbers
 .. |Code Climate| image:: https://codeclimate.com/github/vfxGer/pretty-numbers/badges/gpa.svg
    :target: https://codeclimate.com/github/vfxGer/pretty-numbers
  
-
-
```

### Comparing `prettynumbers-0.1.0/README.md` & `prettynumbers-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `prettynumbers-0.1.0/pretty_numbers.py` & `prettynumbers-0.1.1/pretty_numbers.py`

 * *Files identical despite different names*

### Comparing `prettynumbers-0.1.0/prettynumbers.egg-info/PKG-INFO` & `prettynumbers-0.1.1/prettynumbers.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,25 +1,23 @@
 Metadata-Version: 2.1
 Name: prettynumbers
-Version: 0.1.0
+Version: 0.1.1
 Summary: Display a range of numbers in a human readable way
 Home-page: https://github.com/vfxGer/pretty-numbers
+Download-URL: https://pypi.python.org/packages/source/d/pretty_numbers-0.1.1.tar.gz?raw=true
 Author: Gerard Keating
 Author-email: gerardk@gmail.com
 License: GNU GENERAL PUBLIC LICENSE
-Download-URL: https://pypi.python.org/packages/source/d/pretty_numbers-0.1.0.tar.gz?raw=true
 Platform: Cross-platform
 Classifier: Programming Language :: Python :: 3
 Description-Content-Type: text/x-rst
 License-File: LICENSE.txt
 
 |Build Status| |codecov.io| |Code Climate|
 
 .. |Build Status| image:: https://travis-ci.org/vfxGer/pretty-numbers.svg?branch=master
    :target: https://travis-ci.org/vfxGer/pretty-numbers
 .. |codecov.io| image:: https://codecov.io/gh/vfxGer/pretty-numbers/coverage.svg?branch=master
    :target: https://codecov.io/gh/vfxGer/pretty-numbers
 .. |Code Climate| image:: https://codeclimate.com/github/vfxGer/pretty-numbers/badges/gpa.svg
    :target: https://codeclimate.com/github/vfxGer/pretty-numbers
  
-
-
```

### Comparing `prettynumbers-0.1.0/setup.py` & `prettynumbers-0.1.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # based on https://github.com/pypa/sampleproject/blob/master/setup.py
 from setuptools import setup
 from os import path
 
 here = path.abspath(path.dirname(__file__))
 
-version = "0.1.0"
+version = "0.1.1"
 
 # Get the long description from the README file
 with open(path.join(here, "README.rst")) as f:
     long_description = f.read()
 
 setup(
     name="prettynumbers",
```

