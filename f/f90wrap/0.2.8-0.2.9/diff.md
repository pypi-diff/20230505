# Comparing `tmp/f90wrap-0.2.8.tar.gz` & `tmp/f90wrap-0.2.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "f90wrap-0.2.8.tar", last modified: Wed Sep 14 15:49:01 2022, max compression
+gzip compressed data, was "f90wrap-0.2.9.tar", last modified: Thu Oct 13 10:57:21 2022, max compression
```

## Comparing `f90wrap-0.2.8.tar` & `f90wrap-0.2.9.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-14 15:49:01.208202 f90wrap-0.2.8/
--rw-r--r--   0 runner    (1001) docker     (121)     7651 2022-09-14 15:42:36.000000 f90wrap-0.2.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)    13637 2022-09-14 15:49:01.208202 f90wrap-0.2.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)    13230 2022-09-14 15:42:36.000000 f90wrap-0.2.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-14 15:49:01.204202 f90wrap-0.2.8/f90wrap/
--rw-r--r--   0 runner    (1001) docker     (121)     2027 2022-09-14 15:42:36.000000 f90wrap-0.2.8/f90wrap/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1386 2022-09-14 15:42:36.000000 f90wrap-0.2.8/f90wrap/__main__.py
--rw-r--r--   0 runner    (1001) docker     (121)     5632 2022-09-14 15:42:36.000000 f90wrap-0.2.8/f90wrap/arraydatamodule.c
--rw-r--r--   0 runner    (1001) docker     (121)     4833 2022-09-14 15:42:36.000000 f90wrap-0.2.8/f90wrap/codegen.py
--rw-r--r--   0 runner    (1001) docker     (121)    35273 2022-09-14 15:42:36.000000 f90wrap-0.2.8/f90wrap/f90wrapgen.py
--rw-r--r--   0 runner    (1001) docker     (121)    32522 2022-09-14 15:42:36.000000 f90wrap-0.2.8/f90wrap/fortran.py
--rw-r--r--   0 runner    (1001) docker     (121)     4135 2022-09-14 15:42:36.000000 f90wrap-0.2.8/f90wrap/fortrantype.py
--rw-r--r--   0 runner    (1001) docker     (121)    31846 2022-09-14 15:42:36.000000 f90wrap-0.2.8/f90wrap/latex.py
--rw-r--r--   0 runner    (1001) docker     (121)    46940 2022-09-14 15:42:36.000000 f90wrap-0.2.8/f90wrap/parser.py
--rw-r--r--   0 runner    (1001) docker     (121)    32185 2022-09-14 15:42:36.000000 f90wrap-0.2.8/f90wrap/pywrapgen.py
--rw-r--r--   0 runner    (1001) docker     (121)     1974 2022-09-14 15:42:36.000000 f90wrap-0.2.8/f90wrap/runtime.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-14 15:49:01.208202 f90wrap-0.2.8/f90wrap/scripts/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-14 15:42:36.000000 f90wrap-0.2.8/f90wrap/scripts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     7964 2022-09-14 15:42:36.000000 f90wrap-0.2.8/f90wrap/scripts/f2py_f90wrap.py
--rw-r--r--   0 runner    (1001) docker     (121)     3619 2022-09-14 15:42:36.000000 f90wrap-0.2.8/f90wrap/scripts/f90doc.py
--rw-r--r--   0 runner    (1001) docker     (121)    17363 2022-09-14 15:42:36.000000 f90wrap-0.2.8/f90wrap/scripts/main.py
--rw-r--r--   0 runner    (1001) docker     (121)    31087 2022-09-14 15:42:36.000000 f90wrap-0.2.8/f90wrap/six.py
--rw-r--r--   0 runner    (1001) docker     (121)      282 2022-09-14 15:42:36.000000 f90wrap-0.2.8/f90wrap/sizeoffortran.f90
--rw-r--r--   0 runner    (1001) docker     (121)    61616 2022-09-14 15:42:36.000000 f90wrap-0.2.8/f90wrap/transform.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-14 15:49:01.208202 f90wrap-0.2.8/f90wrap.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)    13637 2022-09-14 15:49:01.000000 f90wrap-0.2.8/f90wrap.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      854 2022-09-14 15:49:01.000000 f90wrap-0.2.8/f90wrap.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-09-14 15:49:01.000000 f90wrap-0.2.8/f90wrap.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       12 2022-09-14 15:49:01.000000 f90wrap-0.2.8/f90wrap.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       24 2022-09-14 15:49:01.000000 f90wrap-0.2.8/f90wrap.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)      172 2022-09-14 15:42:36.000000 f90wrap-0.2.8/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-14 15:49:01.208202 f90wrap-0.2.8/scripts/
--rw-r--r--   0 runner    (1001) docker     (121)      129 2022-09-14 15:42:36.000000 f90wrap-0.2.8/scripts/f2py-f90wrap
--rw-r--r--   0 runner    (1001) docker     (121)      123 2022-09-14 15:42:36.000000 f90wrap-0.2.8/scripts/f90doc
--rw-r--r--   0 runner    (1001) docker     (121)      121 2022-09-14 15:42:36.000000 f90wrap-0.2.8/scripts/f90wrap
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-09-14 15:49:01.208202 f90wrap-0.2.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     2528 2022-09-14 15:42:36.000000 f90wrap-0.2.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-14 15:49:01.208202 f90wrap-0.2.8/test/
--rw-r--r--   0 runner    (1001) docker     (121)     1109 2022-09-14 15:42:36.000000 f90wrap-0.2.8/test/test_parser.py
--rw-r--r--   0 runner    (1001) docker     (121)     3241 2022-09-14 15:42:36.000000 f90wrap-0.2.8/test/test_transform.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-13 10:57:21.136614 f90wrap-0.2.9/
+-rw-r--r--   0 runner    (1001) docker     (121)     7651 2022-10-13 10:30:29.000000 f90wrap-0.2.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (121)    14534 2022-10-13 10:57:21.136614 f90wrap-0.2.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)    14127 2022-10-13 10:30:29.000000 f90wrap-0.2.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-13 10:57:21.132614 f90wrap-0.2.9/f90wrap/
+-rw-r--r--   0 runner    (1001) docker     (121)     2027 2022-10-13 10:30:29.000000 f90wrap-0.2.9/f90wrap/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1386 2022-10-13 10:30:29.000000 f90wrap-0.2.9/f90wrap/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     5632 2022-10-13 10:30:29.000000 f90wrap-0.2.9/f90wrap/arraydatamodule.c
+-rw-r--r--   0 runner    (1001) docker     (121)     4833 2022-10-13 10:30:29.000000 f90wrap-0.2.9/f90wrap/codegen.py
+-rw-r--r--   0 runner    (1001) docker     (121)    35273 2022-10-13 10:30:29.000000 f90wrap-0.2.9/f90wrap/f90wrapgen.py
+-rw-r--r--   0 runner    (1001) docker     (121)    32522 2022-10-13 10:30:29.000000 f90wrap-0.2.9/f90wrap/fortran.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4135 2022-10-13 10:30:29.000000 f90wrap-0.2.9/f90wrap/fortrantype.py
+-rw-r--r--   0 runner    (1001) docker     (121)    31846 2022-10-13 10:30:29.000000 f90wrap-0.2.9/f90wrap/latex.py
+-rw-r--r--   0 runner    (1001) docker     (121)    46940 2022-10-13 10:30:29.000000 f90wrap-0.2.9/f90wrap/parser.py
+-rw-r--r--   0 runner    (1001) docker     (121)    32185 2022-10-13 10:30:29.000000 f90wrap-0.2.9/f90wrap/pywrapgen.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1974 2022-10-13 10:30:29.000000 f90wrap-0.2.9/f90wrap/runtime.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-13 10:57:21.136614 f90wrap-0.2.9/f90wrap/scripts/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-10-13 10:30:29.000000 f90wrap-0.2.9/f90wrap/scripts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     7964 2022-10-13 10:30:29.000000 f90wrap-0.2.9/f90wrap/scripts/f2py_f90wrap.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3619 2022-10-13 10:30:29.000000 f90wrap-0.2.9/f90wrap/scripts/f90doc.py
+-rw-r--r--   0 runner    (1001) docker     (121)    17363 2022-10-13 10:30:29.000000 f90wrap-0.2.9/f90wrap/scripts/main.py
+-rw-r--r--   0 runner    (1001) docker     (121)    31087 2022-10-13 10:30:29.000000 f90wrap-0.2.9/f90wrap/six.py
+-rw-r--r--   0 runner    (1001) docker     (121)      282 2022-10-13 10:30:29.000000 f90wrap-0.2.9/f90wrap/sizeoffortran.f90
+-rw-r--r--   0 runner    (1001) docker     (121)    61616 2022-10-13 10:30:29.000000 f90wrap-0.2.9/f90wrap/transform.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-13 10:57:21.136614 f90wrap-0.2.9/f90wrap.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)    14534 2022-10-13 10:57:21.000000 f90wrap-0.2.9/f90wrap.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      854 2022-10-13 10:57:21.000000 f90wrap-0.2.9/f90wrap.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-10-13 10:57:21.000000 f90wrap-0.2.9/f90wrap.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       12 2022-10-13 10:57:21.000000 f90wrap-0.2.9/f90wrap.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       24 2022-10-13 10:57:21.000000 f90wrap-0.2.9/f90wrap.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      172 2022-10-13 10:30:29.000000 f90wrap-0.2.9/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-13 10:57:21.136614 f90wrap-0.2.9/scripts/
+-rw-r--r--   0 runner    (1001) docker     (121)      129 2022-10-13 10:30:29.000000 f90wrap-0.2.9/scripts/f2py-f90wrap
+-rw-r--r--   0 runner    (1001) docker     (121)      123 2022-10-13 10:30:29.000000 f90wrap-0.2.9/scripts/f90doc
+-rw-r--r--   0 runner    (1001) docker     (121)      121 2022-10-13 10:30:29.000000 f90wrap-0.2.9/scripts/f90wrap
+-rw-r--r--   0 runner    (1001) docker     (121)       38 2022-10-13 10:57:21.136614 f90wrap-0.2.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)     2528 2022-10-13 10:30:29.000000 f90wrap-0.2.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-10-13 10:57:21.136614 f90wrap-0.2.9/test/
+-rw-r--r--   0 runner    (1001) docker     (121)     1109 2022-10-13 10:30:29.000000 f90wrap-0.2.9/test/test_parser.py
+-rw-r--r--   0 runner    (1001) docker     (121)     3241 2022-10-13 10:30:29.000000 f90wrap-0.2.9/test/test_transform.py
```

### Comparing `f90wrap-0.2.8/LICENSE` & `f90wrap-0.2.9/LICENSE`

 * *Files identical despite different names*

### Comparing `f90wrap-0.2.8/PKG-INFO` & `f90wrap-0.2.9/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: f90wrap
-Version: 0.2.8
+Version: 0.2.9
 Summary: Fortran to Python interface generator with derived type support
 Home-page: https://github.com/jameskermode/f90wrap
-Download-URL: https://github.com/jameskermode/f90wrap/archive/refs/tags/v0.2.8.tar.gz
+Download-URL: https://github.com/jameskermode/f90wrap/archive/refs/tags/v0.2.9.tar.gz
 Author: James Kermode
 Author-email: james.kermode@gmail.com
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 f90wrap: Fortran to Python interface generator with derived type support
@@ -108,15 +108,16 @@
 Case studies
 ------------
 
 f90wrap has been used to wrap the following large-scale scientific
 applications:
 
  - [QUIP](http://libatoms.github.io/QUIP/) - molecular dynamics code
- - [CASTEP](http://www.castep.org) - electronic structure code
+ - [CASTEP](http://www.castep.org) - CasPyTep wrappers for electronic structure code
+ - [QEpy](http://qepy.rutgers.edu/index.html) - Python wrapper for Quantum Espresso electronic structure code
 
 See this [Jupyter notebook](https://github.com/jameskermode/f90wrap/blob/master/docs/tutorials/f90wrap-demo.ipynb) 
 from a recent seminar for more details.
 
 Usage
 -----
 
@@ -301,7 +302,34 @@
 - Greg Corbett  [gregcorbett](https://github.com/gregcorbett)
 - Bob Fischer [citibob](https://github.com/citibob)
 - David Verelst [davidovitch](https://github.com/davidovitch)
 - James Orr [jamesorr](https://github.com/jamesorr)
 - [yvesch](https://github.com/yvesch)
 - [Matthias Cuntz](https://github.com/mcuntz)
 - Balthasar Reuter [reuterbal](https://github.com/reuterbal)
+
+
+Developer Notes
+---------------
+
+### Triggering the wheel build
+
+Wheels are built on push and pull requests to `master` using cibuildwheel
+with [this workflow](.github/workflows/build-wheels.yml).
+
+To make a release candidate create a tag with a suffix such as `-rc1` for the first attempt, 
+push to trigger the build:
+
+```bash
+git commit -m 'release v0.x.z.rc1'
+git tag v0.x.y.rc1
+git push --tags
+```
+
+If all goes well, the `.whl` files will show up as assets within a new GitHub
+release. The installation process can now be tested locally.
+
+### Release wheels to PyPI
+
+Once everything works correctly, make a full release (i.e. create a tag named
+just `v0.x.y` without the `-rc1` suffix). This will trigger the upload of wheels
+and source distribution to PyPI.
```

### Comparing `f90wrap-0.2.8/README.md` & `f90wrap-0.2.9/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -96,15 +96,16 @@
 Case studies
 ------------
 
 f90wrap has been used to wrap the following large-scale scientific
 applications:
 
  - [QUIP](http://libatoms.github.io/QUIP/) - molecular dynamics code
- - [CASTEP](http://www.castep.org) - electronic structure code
+ - [CASTEP](http://www.castep.org) - CasPyTep wrappers for electronic structure code
+ - [QEpy](http://qepy.rutgers.edu/index.html) - Python wrapper for Quantum Espresso electronic structure code
 
 See this [Jupyter notebook](https://github.com/jameskermode/f90wrap/blob/master/docs/tutorials/f90wrap-demo.ipynb) 
 from a recent seminar for more details.
 
 Usage
 -----
 
@@ -289,7 +290,34 @@
 - Greg Corbett  [gregcorbett](https://github.com/gregcorbett)
 - Bob Fischer [citibob](https://github.com/citibob)
 - David Verelst [davidovitch](https://github.com/davidovitch)
 - James Orr [jamesorr](https://github.com/jamesorr)
 - [yvesch](https://github.com/yvesch)
 - [Matthias Cuntz](https://github.com/mcuntz)
 - Balthasar Reuter [reuterbal](https://github.com/reuterbal)
+
+
+Developer Notes
+---------------
+
+### Triggering the wheel build
+
+Wheels are built on push and pull requests to `master` using cibuildwheel
+with [this workflow](.github/workflows/build-wheels.yml).
+
+To make a release candidate create a tag with a suffix such as `-rc1` for the first attempt, 
+push to trigger the build:
+
+```bash
+git commit -m 'release v0.x.z.rc1'
+git tag v0.x.y.rc1
+git push --tags
+```
+
+If all goes well, the `.whl` files will show up as assets within a new GitHub
+release. The installation process can now be tested locally.
+
+### Release wheels to PyPI
+
+Once everything works correctly, make a full release (i.e. create a tag named
+just `v0.x.y` without the `-rc1` suffix). This will trigger the upload of wheels
+and source distribution to PyPI.
```

### Comparing `f90wrap-0.2.8/f90wrap/__init__.py` & `f90wrap-0.2.9/f90wrap/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -43,8 +43,8 @@
 """f90wrap package
 
 Add support for Fortran derived types and interfaces to f2py by
 wrapping Fortran code with a simple f90 interface layer.
 
 (c) James Kermode 2011-2021 <james.kermode@gmail.com>"""
 
-__version__ = '0.2.8'
+__version__ = '0.2.9'
```

### Comparing `f90wrap-0.2.8/f90wrap/__main__.py` & `f90wrap-0.2.9/f90wrap/__main__.py`

 * *Files identical despite different names*

### Comparing `f90wrap-0.2.8/f90wrap/arraydatamodule.c` & `f90wrap-0.2.9/f90wrap/arraydatamodule.c`

 * *Files identical despite different names*

### Comparing `f90wrap-0.2.8/f90wrap/codegen.py` & `f90wrap-0.2.9/f90wrap/codegen.py`

 * *Files identical despite different names*

### Comparing `f90wrap-0.2.8/f90wrap/f90wrapgen.py` & `f90wrap-0.2.9/f90wrap/f90wrapgen.py`

 * *Files identical despite different names*

### Comparing `f90wrap-0.2.8/f90wrap/fortran.py` & `f90wrap-0.2.9/f90wrap/fortran.py`

 * *Files identical despite different names*

### Comparing `f90wrap-0.2.8/f90wrap/fortrantype.py` & `f90wrap-0.2.9/f90wrap/fortrantype.py`

 * *Files identical despite different names*

### Comparing `f90wrap-0.2.8/f90wrap/latex.py` & `f90wrap-0.2.9/f90wrap/latex.py`

 * *Files identical despite different names*

### Comparing `f90wrap-0.2.8/f90wrap/parser.py` & `f90wrap-0.2.9/f90wrap/parser.py`

 * *Files identical despite different names*

### Comparing `f90wrap-0.2.8/f90wrap/pywrapgen.py` & `f90wrap-0.2.9/f90wrap/pywrapgen.py`

 * *Files identical despite different names*

### Comparing `f90wrap-0.2.8/f90wrap/runtime.py` & `f90wrap-0.2.9/f90wrap/runtime.py`

 * *Files identical despite different names*

### Comparing `f90wrap-0.2.8/f90wrap/scripts/f2py_f90wrap.py` & `f90wrap-0.2.9/f90wrap/scripts/f2py_f90wrap.py`

 * *Files identical despite different names*

### Comparing `f90wrap-0.2.8/f90wrap/scripts/f90doc.py` & `f90wrap-0.2.9/f90wrap/scripts/f90doc.py`

 * *Files identical despite different names*

### Comparing `f90wrap-0.2.8/f90wrap/scripts/main.py` & `f90wrap-0.2.9/f90wrap/scripts/main.py`

 * *Files identical despite different names*

### Comparing `f90wrap-0.2.8/f90wrap/six.py` & `f90wrap-0.2.9/f90wrap/six.py`

 * *Files identical despite different names*

### Comparing `f90wrap-0.2.8/f90wrap/transform.py` & `f90wrap-0.2.9/f90wrap/transform.py`

 * *Files identical despite different names*

### Comparing `f90wrap-0.2.8/f90wrap.egg-info/PKG-INFO` & `f90wrap-0.2.9/f90wrap.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: f90wrap
-Version: 0.2.8
+Version: 0.2.9
 Summary: Fortran to Python interface generator with derived type support
 Home-page: https://github.com/jameskermode/f90wrap
-Download-URL: https://github.com/jameskermode/f90wrap/archive/refs/tags/v0.2.8.tar.gz
+Download-URL: https://github.com/jameskermode/f90wrap/archive/refs/tags/v0.2.9.tar.gz
 Author: James Kermode
 Author-email: james.kermode@gmail.com
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 f90wrap: Fortran to Python interface generator with derived type support
@@ -108,15 +108,16 @@
 Case studies
 ------------
 
 f90wrap has been used to wrap the following large-scale scientific
 applications:
 
  - [QUIP](http://libatoms.github.io/QUIP/) - molecular dynamics code
- - [CASTEP](http://www.castep.org) - electronic structure code
+ - [CASTEP](http://www.castep.org) - CasPyTep wrappers for electronic structure code
+ - [QEpy](http://qepy.rutgers.edu/index.html) - Python wrapper for Quantum Espresso electronic structure code
 
 See this [Jupyter notebook](https://github.com/jameskermode/f90wrap/blob/master/docs/tutorials/f90wrap-demo.ipynb) 
 from a recent seminar for more details.
 
 Usage
 -----
 
@@ -301,7 +302,34 @@
 - Greg Corbett  [gregcorbett](https://github.com/gregcorbett)
 - Bob Fischer [citibob](https://github.com/citibob)
 - David Verelst [davidovitch](https://github.com/davidovitch)
 - James Orr [jamesorr](https://github.com/jamesorr)
 - [yvesch](https://github.com/yvesch)
 - [Matthias Cuntz](https://github.com/mcuntz)
 - Balthasar Reuter [reuterbal](https://github.com/reuterbal)
+
+
+Developer Notes
+---------------
+
+### Triggering the wheel build
+
+Wheels are built on push and pull requests to `master` using cibuildwheel
+with [this workflow](.github/workflows/build-wheels.yml).
+
+To make a release candidate create a tag with a suffix such as `-rc1` for the first attempt, 
+push to trigger the build:
+
+```bash
+git commit -m 'release v0.x.z.rc1'
+git tag v0.x.y.rc1
+git push --tags
+```
+
+If all goes well, the `.whl` files will show up as assets within a new GitHub
+release. The installation process can now be tested locally.
+
+### Release wheels to PyPI
+
+Once everything works correctly, make a full release (i.e. create a tag named
+just `v0.x.y` without the `-rc1` suffix). This will trigger the upload of wheels
+and source distribution to PyPI.
```

### Comparing `f90wrap-0.2.8/f90wrap.egg-info/SOURCES.txt` & `f90wrap-0.2.9/f90wrap.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 LICENSE
 README.md
 pyproject.toml
 setup.py
-/tmp/build-env-ol4tsk4w/lib/python3.10/site-packages/numpy/f2py/src/fortranobject.c
-/tmp/build-env-ol4tsk4w/lib/python3.10/site-packages/numpy/f2py/src/fortranobject.h
+/tmp/build-env-afx9jcub/lib/python3.10/site-packages/numpy/f2py/src/fortranobject.c
+/tmp/build-env-afx9jcub/lib/python3.10/site-packages/numpy/f2py/src/fortranobject.h
 f90wrap/__init__.py
 f90wrap/__main__.py
 f90wrap/arraydatamodule.c
 f90wrap/codegen.py
 f90wrap/f90wrapgen.py
 f90wrap/fortran.py
 f90wrap/fortrantype.py
```

### Comparing `f90wrap-0.2.8/setup.py` & `f90wrap-0.2.9/setup.py`

 * *Files identical despite different names*

### Comparing `f90wrap-0.2.8/test/test_parser.py` & `f90wrap-0.2.9/test/test_parser.py`

 * *Files identical despite different names*

### Comparing `f90wrap-0.2.8/test/test_transform.py` & `f90wrap-0.2.9/test/test_transform.py`

 * *Files identical despite different names*

