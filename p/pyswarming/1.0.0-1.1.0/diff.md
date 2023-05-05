# Comparing `tmp/pyswarming-1.0.0.tar.gz` & `tmp/pyswarming-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/pyswarming-1.0.0.tar", last modified: Thu Sep 22 17:40:22 2022, max compression
+gzip compressed data, was "/Users/macbookpro/Documents/GitHub/pyswarming/dist/.tmp-ttexk_cz/pyswarming-1.1.0.tar", last modified: Fri May  5 02:11:18 2023, max compression
```

## Comparing `pyswarming-1.0.0.tar` & `pyswarming-1.1.0.tar`

### file list

```diff
@@ -1,61 +1,20 @@
-drwxr-xr-x   0 mrsonandrade   (503) staff       (20)        0 2022-09-22 17:40:22.000000 pyswarming-1.0.0/
--rw-r--r--   0 mrsonandrade   (503) staff       (20)       66 2022-09-09 13:09:52.000000 pyswarming-1.0.0/.gitattributes
-drwxr-xr-x   0 mrsonandrade   (503) staff       (20)        0 2022-09-22 17:40:20.000000 pyswarming-1.0.0/.github/
-drwxr-xr-x   0 mrsonandrade   (503) staff       (20)        0 2022-09-22 17:40:21.000000 pyswarming-1.0.0/.github/workflows/
--rw-r--r--   0 mrsonandrade   (503) staff       (20)      670 2022-09-21 17:57:30.000000 pyswarming-1.0.0/.github/workflows/draft-pdf.yml
--rw-r--r--   0 mrsonandrade   (503) staff       (20)     1201 2022-09-13 01:24:50.000000 pyswarming-1.0.0/.github/workflows/tests_package.yml
--rwxr-xr-x   0 mrsonandrade   (503) staff       (20)      117 2022-09-13 01:25:33.000000 pyswarming-1.0.0/.gitignore
-drwxr-xr-x   0 mrsonandrade   (503) staff       (20)        0 2022-09-22 17:40:21.000000 pyswarming-1.0.0/Examples/
--rwxr-xr-x   0 mrsonandrade   (503) staff       (20)    17854 2022-09-19 01:31:35.000000 pyswarming-1.0.0/Examples/01_Getting_Started.ipynb
-drwxr-xr-x   0 mrsonandrade   (503) staff       (20)        0 2022-09-22 17:40:21.000000 pyswarming-1.0.0/Examples/pics/
--rw-r--r--   0 mrsonandrade   (503) staff       (20)   778383 2022-09-09 17:55:40.000000 pyswarming-1.0.0/Examples/pics/Aggregation.gif
--rw-r--r--   0 mrsonandrade   (503) staff       (20)   566169 2022-09-09 18:00:22.000000 pyswarming-1.0.0/Examples/pics/AggregationRepulsion.gif
--rw-r--r--   0 mrsonandrade   (503) staff       (20)   371035 2022-09-10 00:57:22.000000 pyswarming-1.0.0/Examples/pics/AreaCoverage.gif
--rw-r--r--   0 mrsonandrade   (503) staff       (20)  1016225 2022-09-10 00:36:51.000000 pyswarming-1.0.0/Examples/pics/CollectiveNavigation.gif
--rw-r--r--   0 mrsonandrade   (503) staff       (20)   581136 2022-09-09 17:57:50.000000 pyswarming-1.0.0/Examples/pics/Repulsion.gif
--rw-r--r--   0 mrsonandrade   (503) staff       (20)   589487 2022-09-09 17:53:56.000000 pyswarming-1.0.0/Examples/pics/Target.gif
--rwxr-xr-x   0 mrsonandrade   (503) staff       (20)     1529 2022-09-01 17:38:39.000000 pyswarming-1.0.0/LICENSE.md
--rw-r--r--   0 mrsonandrade   (503) staff       (20)     9001 2022-09-22 17:40:22.000000 pyswarming-1.0.0/PKG-INFO
--rwxr-xr-x   0 mrsonandrade   (503) staff       (20)     6849 2022-09-22 00:42:08.000000 pyswarming-1.0.0/README.md
-drwxr-xr-x   0 mrsonandrade   (503) staff       (20)        0 2022-09-22 17:40:21.000000 pyswarming-1.0.0/docs/
--rwxr-xr-x   0 mrsonandrade   (503) staff       (20)      638 2022-08-23 05:09:44.000000 pyswarming-1.0.0/docs/Makefile
--rwxr-xr-x   0 mrsonandrade   (503) staff       (20)      799 2022-08-23 05:09:44.000000 pyswarming-1.0.0/docs/make.bat
-drwxr-xr-x   0 mrsonandrade   (503) staff       (20)        0 2022-09-22 17:40:21.000000 pyswarming-1.0.0/docs/readme_pics/
--rw-r--r--   0 mrsonandrade   (503) staff       (20)   778383 2022-09-09 17:55:40.000000 pyswarming-1.0.0/docs/readme_pics/Aggregation.gif
--rw-r--r--   0 mrsonandrade   (503) staff       (20)   566169 2022-09-09 18:00:22.000000 pyswarming-1.0.0/docs/readme_pics/AggregationRepulsion.gif
--rw-r--r--   0 mrsonandrade   (503) staff       (20)   371035 2022-09-10 00:57:22.000000 pyswarming-1.0.0/docs/readme_pics/AreaCoverage.gif
--rw-r--r--   0 mrsonandrade   (503) staff       (20)  1016225 2022-09-10 00:36:51.000000 pyswarming-1.0.0/docs/readme_pics/CollectiveNavigation.gif
--rw-r--r--   0 mrsonandrade   (503) staff       (20)   581136 2022-09-09 17:57:50.000000 pyswarming-1.0.0/docs/readme_pics/Repulsion.gif
--rw-r--r--   0 mrsonandrade   (503) staff       (20)   589487 2022-09-09 17:53:56.000000 pyswarming-1.0.0/docs/readme_pics/Target.gif
--rw-r--r--   0 mrsonandrade   (503) staff       (20)    58836 2022-09-06 13:09:21.000000 pyswarming-1.0.0/docs/readme_pics/logo.png
--rwxr-xr-x   0 mrsonandrade   (503) staff       (20)       52 2022-09-22 17:36:00.000000 pyswarming-1.0.0/docs/requirements.txt
-drwxr-xr-x   0 mrsonandrade   (503) staff       (20)        0 2022-09-22 17:40:21.000000 pyswarming-1.0.0/docs/source/
--rwxr-xr-x   0 mrsonandrade   (503) staff       (20)      450 2022-09-19 00:29:52.000000 pyswarming-1.0.0/docs/source/Acknowledgements.rst
--rwxr-xr-x   0 mrsonandrade   (503) staff       (20)     3925 2022-09-19 00:40:45.000000 pyswarming-1.0.0/docs/source/Contribution.rst
--rwxr-xr-x   0 mrsonandrade   (503) staff       (20)      139 2022-09-19 00:41:08.000000 pyswarming-1.0.0/docs/source/Examples.rst
--rwxr-xr-x   0 mrsonandrade   (503) staff       (20)     2103 2022-09-19 00:26:07.000000 pyswarming-1.0.0/docs/source/conf.py
-drwxr-xr-x   0 mrsonandrade   (503) staff       (20)        0 2022-09-22 17:40:21.000000 pyswarming-1.0.0/docs/source/example_notebooks/
--rwxr-xr-x   0 mrsonandrade   (503) staff       (20)    17854 2022-09-19 01:31:35.000000 pyswarming-1.0.0/docs/source/example_notebooks/01_Getting_Started.ipynb
--rwxr-xr-x   0 mrsonandrade   (503) staff       (20)       48 2022-08-23 05:09:44.000000 pyswarming-1.0.0/docs/source/functions.rst
--rwxr-xr-x   0 mrsonandrade   (503) staff       (20)     6020 2022-09-21 00:05:42.000000 pyswarming-1.0.0/docs/source/index.rst
--rwxr-xr-x   0 mrsonandrade   (503) staff       (20)      186 2022-09-19 00:44:28.000000 pyswarming-1.0.0/docs/source/pyswarming.rst
-drwxr-xr-x   0 mrsonandrade   (503) staff       (20)        0 2022-09-22 17:40:21.000000 pyswarming-1.0.0/paper/
--rwxr-xr-x   0 mrsonandrade   (503) staff       (20)    27041 2022-09-22 03:37:20.000000 pyswarming-1.0.0/paper/fig1.png
--rwxr-xr-x   0 mrsonandrade   (503) staff       (20)    32186 2022-09-22 03:23:23.000000 pyswarming-1.0.0/paper/fig2.png
--rwxr-xr-x   0 mrsonandrade   (503) staff       (20)     4093 2022-09-22 03:51:27.000000 pyswarming-1.0.0/paper/paper.bib
--rwxr-xr-x   0 mrsonandrade   (503) staff       (20)     6534 2022-09-22 03:51:29.000000 pyswarming-1.0.0/paper/paper.md
-drwxr-xr-x   0 mrsonandrade   (503) staff       (20)        0 2022-09-22 17:40:21.000000 pyswarming-1.0.0/pyswarming/
--rwxr-xr-x   0 mrsonandrade   (503) staff       (20)      735 2022-09-09 00:03:11.000000 pyswarming-1.0.0/pyswarming/__init__.py
--rw-r--r--   0 mrsonandrade   (503) staff       (20)    14252 2022-09-07 14:02:37.000000 pyswarming-1.0.0/pyswarming/auto_differentiation.py
--rwxr-xr-x   0 mrsonandrade   (503) staff       (20)    15044 2022-09-22 00:40:53.000000 pyswarming-1.0.0/pyswarming/behaviors.py
-drwxr-xr-x   0 mrsonandrade   (503) staff       (20)        0 2022-09-22 17:40:22.000000 pyswarming-1.0.0/pyswarming.egg-info/
--rw-r--r--   0 mrsonandrade   (503) staff       (20)     9001 2022-09-22 17:40:19.000000 pyswarming-1.0.0/pyswarming.egg-info/PKG-INFO
--rw-r--r--   0 mrsonandrade   (503) staff       (20)     1236 2022-09-22 17:40:20.000000 pyswarming-1.0.0/pyswarming.egg-info/SOURCES.txt
--rw-r--r--   0 mrsonandrade   (503) staff       (20)        1 2022-09-22 17:40:19.000000 pyswarming-1.0.0/pyswarming.egg-info/dependency_links.txt
--rw-r--r--   0 mrsonandrade   (503) staff       (20)        6 2022-09-22 17:40:19.000000 pyswarming-1.0.0/pyswarming.egg-info/requires.txt
--rw-r--r--   0 mrsonandrade   (503) staff       (20)       17 2022-09-22 17:40:19.000000 pyswarming-1.0.0/pyswarming.egg-info/top_level.txt
--rw-r--r--   0 mrsonandrade   (503) staff       (20)      106 2022-09-22 17:40:22.000000 pyswarming-1.0.0/setup.cfg
--rwxr-xr-x   0 mrsonandrade   (503) staff       (20)     1067 2022-09-09 12:52:29.000000 pyswarming-1.0.0/setup.py
-drwxr-xr-x   0 mrsonandrade   (503) staff       (20)        0 2022-09-22 17:40:22.000000 pyswarming-1.0.0/tests/
--rwxr-xr-x   0 mrsonandrade   (503) staff       (20)        0 2022-08-23 05:09:44.000000 pyswarming-1.0.0/tests/__init__.py
--rwxr-xr-x   0 mrsonandrade   (503) staff       (20)     7094 2022-09-21 18:45:38.000000 pyswarming-1.0.0/tests/test_behaviors.py
+drwxr-xr-x   0 macbookpro   (501) staff       (20)        0 2023-05-05 02:11:18.000000 pyswarming-1.1.0/
+-rwxr-xr-x   0 macbookpro   (501) staff       (20)     1529 2023-04-24 23:27:31.000000 pyswarming-1.1.0/LICENSE.md
+-rw-r--r--   0 macbookpro   (501) staff       (20)    11816 2023-05-05 02:11:18.000000 pyswarming-1.1.0/PKG-INFO
+-rwxr-xr-x   0 macbookpro   (501) staff       (20)    11049 2023-05-04 23:15:51.000000 pyswarming-1.1.0/README.md
+drwxr-xr-x   0 macbookpro   (501) staff       (20)        0 2023-05-05 02:11:18.000000 pyswarming-1.1.0/pyswarming/
+-rwxr-xr-x   0 macbookpro   (501) staff       (20)      899 2023-05-04 18:36:20.000000 pyswarming-1.1.0/pyswarming/__init__.py
+-rw-r--r--   0 macbookpro   (501) staff       (20)    14252 2023-03-29 00:19:04.000000 pyswarming-1.1.0/pyswarming/auto_differentiation.py
+-rwxr-xr-x   0 macbookpro   (501) staff       (20)    25881 2023-05-04 23:32:13.000000 pyswarming-1.1.0/pyswarming/behaviors.py
+-rw-r--r--   0 macbookpro   (501) staff       (20)     8710 2023-05-05 00:54:30.000000 pyswarming-1.1.0/pyswarming/swarm.py
+drwxr-xr-x   0 macbookpro   (501) staff       (20)        0 2023-05-05 02:11:18.000000 pyswarming-1.1.0/pyswarming.egg-info/
+-rw-r--r--   0 macbookpro   (501) staff       (20)    11816 2023-05-05 02:11:18.000000 pyswarming-1.1.0/pyswarming.egg-info/PKG-INFO
+-rw-r--r--   0 macbookpro   (501) staff       (20)      352 2023-05-05 02:11:18.000000 pyswarming-1.1.0/pyswarming.egg-info/SOURCES.txt
+-rw-r--r--   0 macbookpro   (501) staff       (20)        1 2023-05-05 02:11:18.000000 pyswarming-1.1.0/pyswarming.egg-info/dependency_links.txt
+-rw-r--r--   0 macbookpro   (501) staff       (20)       17 2023-05-05 02:11:18.000000 pyswarming-1.1.0/pyswarming.egg-info/requires.txt
+-rw-r--r--   0 macbookpro   (501) staff       (20)       17 2023-05-05 02:11:18.000000 pyswarming-1.1.0/pyswarming.egg-info/top_level.txt
+-rw-r--r--   0 macbookpro   (501) staff       (20)      106 2023-05-05 02:11:18.000000 pyswarming-1.1.0/setup.cfg
+-rwxr-xr-x   0 macbookpro   (501) staff       (20)     1146 2023-04-24 23:22:58.000000 pyswarming-1.1.0/setup.py
+drwxr-xr-x   0 macbookpro   (501) staff       (20)        0 2023-05-05 02:11:18.000000 pyswarming-1.1.0/tests/
+-rwxr-xr-x   0 macbookpro   (501) staff       (20)        0 2023-03-29 00:19:04.000000 pyswarming-1.1.0/tests/__init__.py
+-rwxr-xr-x   0 macbookpro   (501) staff       (20)    16957 2023-05-05 00:54:12.000000 pyswarming-1.1.0/tests/test_behaviors.py
```

### Comparing `pyswarming-1.0.0/LICENSE.md` & `pyswarming-1.1.0/LICENSE.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 BSD 3-Clause License
 
-Copyright (c) 2022, pyswarming Developers
+Copyright (c) 2023, pyswarming Developers
 All rights reserved.
 
 Redistribution and use in source and binary forms, with or without
 modification, are permitted provided that the following conditions are met:
 
 1. Redistributions of source code must retain the above copyright notice, this
    list of conditions and the following disclaimer.
```

### Comparing `pyswarming-1.0.0/pyswarming/__init__.py` & `pyswarming-1.1.0/pyswarming/__init__.py`

 * *Files 11% similar despite different names*

```diff
@@ -11,24 +11,29 @@
 with the code, and a loose standing reference guide, available from
 `the PySwarming homepage <https://github.com/mrsonandrade/pyswarming>`_.
 
 Available subpackages
 ---------------------
 
 behaviors
-    Collection of swarming behaviors.
+    Collection of swarming behaviors based on different research articles.
+
+swarm
+    Allow the creation of simple virtual swarms.
 """
 
 import os
 import sys
 
 sys.path.append(os.path.dirname(os.path.realpath(__file__)))
 
 # To get sub-modules
 from . import behaviors
+from . import swarm
 
 __all__ = behaviors.__all__.copy()
+__all__ = swarm.__all__.copy()
 
 name = "pyswarming"
-__version__ = "1.0.0"
-__author__ = "Emerson de Andrade, Antonio Fernandes and Joel Sales Jr"
+__version__ = "1.1.0"
+__author__ = "Emerson Martins de Andrade, Antonio Carlos Fernandes and Joel Sena Sales Jr"
 __author_email__ = "mrson@oceanica.ufrj.br"
```

### Comparing `pyswarming-1.0.0/pyswarming/auto_differentiation.py` & `pyswarming-1.1.0/pyswarming/auto_differentiation.py`

 * *Files identical despite different names*

### Comparing `pyswarming-1.0.0/setup.py` & `pyswarming-1.1.0/setup.py`

 * *Files 7% similar despite different names*

```diff
@@ -2,31 +2,33 @@
 
 with open("README.md", "r", encoding="utf8", errors="ignore") as fh:
     LONG_DESCRIPTION = fh.read()
 
 # Packages that pyswarming uses explicitly:
 INSTALL_REQUIRES = [
     "numpy",
+    "matplotlib",
 ]
 
 setuptools.setup(
     name="pyswarming",
-    version="1.0.0",
-    author="Emerson Andrade",
+    version="1.1.0",
+    author="Emerson Martins de Andrade",
     author_email="mrson@oceanica.ufrj.br",
     description="A research toolkit for Swarm Robotics",
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     url="https://github.com/mrsonandrade/pyswarming",
     packages=setuptools.find_packages(),
     classifiers=[
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
+        "Programming Language :: Python :: 3.11",
         "License :: OSI Approved :: BSD License",
         "Intended Audience :: Science/Research",
         "Operating System :: OS Independent",
         "Topic :: Scientific/Engineering :: GIS",
     ],
     python_requires=">=3.7",
     install_requires=INSTALL_REQUIRES,
```

