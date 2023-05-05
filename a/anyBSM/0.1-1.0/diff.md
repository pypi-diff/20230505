# Comparing `tmp/anyBSM-0.1.tar.gz` & `tmp/anyBSM-1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "anyBSM-0.1.tar", last modified: Thu Apr 27 01:54:58 2023, max compression
+gzip compressed data, was "anyBSM-1.0.tar", last modified: Fri May  5 01:23:01 2023, max compression
```

## Comparing `anyBSM-0.1.tar` & `anyBSM-1.0.tar`

### file list

```diff
@@ -1,63 +1,63 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 01:54:58.539736 anyBSM-0.1/
--rw-rw-rw-   0 root         (0) root         (0)    35081 2023-04-27 01:54:10.000000 anyBSM-0.1/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)      140 2023-04-27 01:54:10.000000 anyBSM-0.1/MANIFEST.in
--rw-r--r--   0 root         (0) root         (0)      295 2023-04-27 01:54:58.537735 anyBSM-0.1/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)     2651 2023-04-27 01:54:10.000000 anyBSM-0.1/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 01:54:58.516734 anyBSM-0.1/anyBSM/
--rw-rw-rw-   0 root         (0) root         (0)    14861 2023-04-27 01:54:10.000000 anyBSM-0.1/anyBSM/Delta_r_SM.py
--rw-rw-rw-   0 root         (0) root         (0)     1312 2023-04-27 01:54:10.000000 anyBSM-0.1/anyBSM/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1562 2023-04-27 01:54:10.000000 anyBSM-0.1/anyBSM/anyBSM.py
--rw-rw-rw-   0 root         (0) root         (0)     8220 2023-04-27 01:54:10.000000 anyBSM-0.1/anyBSM/anyEWPO.py
--rw-rw-rw-   0 root         (0) root         (0)    21040 2023-04-27 01:54:10.000000 anyBSM-0.1/anyBSM/anyH3.py
--rw-rw-rw-   0 root         (0) root         (0)    59749 2023-04-27 01:54:10.000000 anyBSM-0.1/anyBSM/anyModel.py
--rw-rw-rw-   0 root         (0) root         (0)     2485 2023-04-27 01:54:10.000000 anyBSM-0.1/anyBSM/anyPerturbativeUnitarity.py
--rw-rw-rw-   0 root         (0) root         (0)    23410 2023-04-27 01:54:10.000000 anyBSM-0.1/anyBSM/anyProcess.py
--rw-rw-rw-   0 root         (0) root         (0)     3277 2023-04-27 01:54:10.000000 anyBSM-0.1/anyBSM/config.py
--rw-rw-rw-   0 root         (0) root         (0)    25457 2023-04-27 01:54:10.000000 anyBSM-0.1/anyBSM/diagrams.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 01:54:58.522734 anyBSM-0.1/anyBSM/latex/
--rw-rw-rw-   0 root         (0) root         (0)     4711 2023-04-27 01:54:10.000000 anyBSM-0.1/anyBSM/latex/__init__.py
--rwxrwxrwx   0 root         (0) root         (0)    22703 2023-04-27 01:54:10.000000 anyBSM-0.1/anyBSM/latex/drawer.py
--rw-rw-rw-   0 root         (0) root         (0)     3690 2023-04-27 01:54:10.000000 anyBSM-0.1/anyBSM/latex/printer.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 01:54:58.526734 anyBSM-0.1/anyBSM/latex/tikzfeynman/
--rw-rw-rw-   0 root         (0) root         (0)    52209 2023-04-27 01:54:10.000000 anyBSM-0.1/anyBSM/latex/tikzfeynman/LICENSE
--rw-rw-rw-   0 root         (0) root         (0)    30485 2023-04-27 01:54:10.000000 anyBSM-0.1/anyBSM/latex/tikzfeynman/tikzfeynman.keys.code.tex
--rw-rw-rw-   0 root         (0) root         (0)    31357 2023-04-27 01:54:10.000000 anyBSM-0.1/anyBSM/latex/tikzfeynman/tikzfeynman.patch.3.0.0.lua
--rw-rw-rw-   0 root         (0) root         (0)    32511 2023-04-27 01:54:10.000000 anyBSM-0.1/anyBSM/latex/tikzfeynman/tikzfeynman.patch.3.0.1.lua
--rw-rw-rw-   0 root         (0) root         (0)     1329 2023-04-27 01:54:10.000000 anyBSM-0.1/anyBSM/latex/tikzfeynman/tikzfeynman.sty
--rw-rw-rw-   0 root         (0) root         (0)    11610 2023-04-27 01:54:10.000000 anyBSM-0.1/anyBSM/latex/tikzfeynman/tikzlibraryfeynman.code.tex
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 01:54:58.530735 anyBSM-0.1/anyBSM/logos/
--rw-rw-rw-   0 root         (0) root         (0)    59037 2023-04-27 01:54:10.000000 anyBSM-0.1/anyBSM/logos/anyH3_logo_large.png
--rw-rw-rw-   0 root         (0) root         (0)     3724 2023-04-27 01:54:10.000000 anyBSM-0.1/anyBSM/logos/anyH3_logo_plot.png
--rw-rw-rw-   0 root         (0) root         (0)    15988 2023-04-27 01:54:10.000000 anyBSM-0.1/anyBSM/logos/anyH3_logo_small.png
--rw-rw-rw-   0 root         (0) root         (0)   224085 2023-04-27 01:54:10.000000 anyBSM-0.1/anyBSM/logos/class_structure.png
--rw-rw-rw-   0 root         (0) root         (0)   324099 2023-04-27 01:54:10.000000 anyBSM-0.1/anyBSM/logos/program_structure.png
--rw-rw-rw-   0 root         (0) root         (0)     7296 2023-04-27 01:54:10.000000 anyBSM-0.1/anyBSM/loopfunctions.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 01:54:58.530735 anyBSM-0.1/anyBSM/mathematica_interface/
--rw-rw-rw-   0 root         (0) root         (0)    12715 2023-04-27 01:54:10.000000 anyBSM-0.1/anyBSM/mathematica_interface/anyBSM.m
--rw-rw-rw-   0 root         (0) root         (0)     1826 2023-04-27 01:54:10.000000 anyBSM-0.1/anyBSM/physic_utils.py
--rw-rw-rw-   0 root         (0) root         (0)    12391 2023-04-27 01:54:10.000000 anyBSM-0.1/anyBSM/plotting.py
--rw-rw-rw-   0 root         (0) root         (0)     7752 2023-04-27 01:54:10.000000 anyBSM-0.1/anyBSM/topologies.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 01:54:58.533735 anyBSM-0.1/anyBSM/ufo/
--rw-rw-rw-   0 root         (0) root         (0)     1246 2023-04-27 01:54:10.000000 anyBSM-0.1/anyBSM/ufo/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      730 2023-04-27 01:54:10.000000 anyBSM-0.1/anyBSM/ufo/function_library.py
--rw-rw-rw-   0 root         (0) root         (0)    12774 2023-04-27 01:54:10.000000 anyBSM-0.1/anyBSM/ufo/object_library.py
--rw-rw-rw-   0 root         (0) root         (0)     6200 2023-04-27 01:54:10.000000 anyBSM-0.1/anyBSM/ufo/write_param_card.py
--rw-rw-rw-   0 root         (0) root         (0)     4559 2023-04-27 01:54:10.000000 anyBSM-0.1/anyBSM/utils.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 01:54:58.520734 anyBSM-0.1/anyBSM.egg-info/
--rw-r--r--   0 root         (0) root         (0)      295 2023-04-27 01:54:58.000000 anyBSM-0.1/anyBSM.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     1323 2023-04-27 01:54:58.000000 anyBSM-0.1/anyBSM.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-27 01:54:58.000000 anyBSM-0.1/anyBSM.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      146 2023-04-27 01:54:58.000000 anyBSM-0.1/anyBSM.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)        7 2023-04-27 01:54:58.000000 anyBSM-0.1/anyBSM.egg-info/top_level.txt
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 01:54:58.534735 anyBSM-0.1/bin/
--rwxrwxrwx   0 root         (0) root         (0)    12063 2023-04-27 01:54:10.000000 anyBSM-0.1/bin/anyBSM
--rwxrwxrwx   0 root         (0) root         (0)    25624 2023-04-27 01:54:10.000000 anyBSM-0.1/bin/anyBSM_import
--rw-rw-rw-   0 root         (0) root         (0)      693 2023-04-27 01:54:10.000000 anyBSM-0.1/pyproject.toml
--rw-r--r--   0 root         (0) root         (0)       38 2023-04-27 01:54:58.539736 anyBSM-0.1/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)       88 2023-04-27 01:54:10.000000 anyBSM-0.1/setup.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-27 01:54:58.537735 anyBSM-0.1/tests/
--rw-rw-rw-   0 root         (0) root         (0)    32340 2023-04-27 01:54:10.000000 anyBSM-0.1/tests/test_SM.py
--rw-rw-rw-   0 root         (0) root         (0)    50923 2023-04-27 01:54:10.000000 anyBSM-0.1/tests/test_THDM.py
--rw-rw-rw-   0 root         (0) root         (0)     1007 2023-04-27 01:54:10.000000 anyBSM-0.1/tests/test_caching.py
--rw-rw-rw-   0 root         (0) root         (0)     2583 2023-04-27 01:54:10.000000 anyBSM-0.1/tests/test_loopfunctions.py
--rw-rw-rw-   0 root         (0) root         (0)      598 2023-04-27 01:54:10.000000 anyBSM-0.1/tests/test_unitarity.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 01:23:01.845674 anyBSM-1.0/
+-rw-rw-rw-   0 root         (0) root         (0)    35081 2023-05-05 01:22:24.000000 anyBSM-1.0/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)      140 2023-05-05 01:22:24.000000 anyBSM-1.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)      295 2023-05-05 01:23:01.845674 anyBSM-1.0/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)     2936 2023-05-05 01:22:24.000000 anyBSM-1.0/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 01:23:01.832672 anyBSM-1.0/anyBSM/
+-rw-rw-rw-   0 root         (0) root         (0)    14861 2023-05-05 01:22:24.000000 anyBSM-1.0/anyBSM/Delta_r_SM.py
+-rw-rw-rw-   0 root         (0) root         (0)     1312 2023-05-05 01:22:24.000000 anyBSM-1.0/anyBSM/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1562 2023-05-05 01:22:24.000000 anyBSM-1.0/anyBSM/anyBSM.py
+-rw-rw-rw-   0 root         (0) root         (0)     8220 2023-05-05 01:22:24.000000 anyBSM-1.0/anyBSM/anyEWPO.py
+-rw-rw-rw-   0 root         (0) root         (0)    21040 2023-05-05 01:22:24.000000 anyBSM-1.0/anyBSM/anyH3.py
+-rw-rw-rw-   0 root         (0) root         (0)    59836 2023-05-05 01:22:24.000000 anyBSM-1.0/anyBSM/anyModel.py
+-rw-rw-rw-   0 root         (0) root         (0)     2485 2023-05-05 01:22:24.000000 anyBSM-1.0/anyBSM/anyPerturbativeUnitarity.py
+-rw-rw-rw-   0 root         (0) root         (0)    23410 2023-05-05 01:22:24.000000 anyBSM-1.0/anyBSM/anyProcess.py
+-rw-rw-rw-   0 root         (0) root         (0)     3277 2023-05-05 01:22:24.000000 anyBSM-1.0/anyBSM/config.py
+-rw-rw-rw-   0 root         (0) root         (0)    25457 2023-05-05 01:22:24.000000 anyBSM-1.0/anyBSM/diagrams.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 01:23:01.835672 anyBSM-1.0/anyBSM/latex/
+-rw-rw-rw-   0 root         (0) root         (0)     4711 2023-05-05 01:22:24.000000 anyBSM-1.0/anyBSM/latex/__init__.py
+-rwxrwxrwx   0 root         (0) root         (0)    22804 2023-05-05 01:22:24.000000 anyBSM-1.0/anyBSM/latex/drawer.py
+-rw-rw-rw-   0 root         (0) root         (0)     3690 2023-05-05 01:22:24.000000 anyBSM-1.0/anyBSM/latex/printer.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 01:23:01.837673 anyBSM-1.0/anyBSM/latex/tikzfeynman/
+-rw-rw-rw-   0 root         (0) root         (0)    52209 2023-05-05 01:22:24.000000 anyBSM-1.0/anyBSM/latex/tikzfeynman/LICENSE
+-rw-rw-rw-   0 root         (0) root         (0)    30485 2023-05-05 01:22:24.000000 anyBSM-1.0/anyBSM/latex/tikzfeynman/tikzfeynman.keys.code.tex
+-rw-rw-rw-   0 root         (0) root         (0)    31357 2023-05-05 01:22:24.000000 anyBSM-1.0/anyBSM/latex/tikzfeynman/tikzfeynman.patch.3.0.0.lua
+-rw-rw-rw-   0 root         (0) root         (0)    32511 2023-05-05 01:22:24.000000 anyBSM-1.0/anyBSM/latex/tikzfeynman/tikzfeynman.patch.3.0.1.lua
+-rw-rw-rw-   0 root         (0) root         (0)     1329 2023-05-05 01:22:24.000000 anyBSM-1.0/anyBSM/latex/tikzfeynman/tikzfeynman.sty
+-rw-rw-rw-   0 root         (0) root         (0)    11610 2023-05-05 01:22:24.000000 anyBSM-1.0/anyBSM/latex/tikzfeynman/tikzlibraryfeynman.code.tex
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 01:23:01.839673 anyBSM-1.0/anyBSM/logos/
+-rw-rw-rw-   0 root         (0) root         (0)    59037 2023-05-05 01:22:24.000000 anyBSM-1.0/anyBSM/logos/anyH3_logo_large.png
+-rw-rw-rw-   0 root         (0) root         (0)     3724 2023-05-05 01:22:24.000000 anyBSM-1.0/anyBSM/logos/anyH3_logo_plot.png
+-rw-rw-rw-   0 root         (0) root         (0)    15988 2023-05-05 01:22:24.000000 anyBSM-1.0/anyBSM/logos/anyH3_logo_small.png
+-rw-rw-rw-   0 root         (0) root         (0)   224085 2023-05-05 01:22:24.000000 anyBSM-1.0/anyBSM/logos/class_structure.png
+-rw-rw-rw-   0 root         (0) root         (0)   324099 2023-05-05 01:22:24.000000 anyBSM-1.0/anyBSM/logos/program_structure.png
+-rw-rw-rw-   0 root         (0) root         (0)     7296 2023-05-05 01:22:24.000000 anyBSM-1.0/anyBSM/loopfunctions.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 01:23:01.840673 anyBSM-1.0/anyBSM/mathematica_interface/
+-rw-rw-rw-   0 root         (0) root         (0)    12715 2023-05-05 01:22:24.000000 anyBSM-1.0/anyBSM/mathematica_interface/anyBSM.m
+-rw-rw-rw-   0 root         (0) root         (0)     1826 2023-05-05 01:22:24.000000 anyBSM-1.0/anyBSM/physic_utils.py
+-rw-rw-rw-   0 root         (0) root         (0)    12391 2023-05-05 01:22:24.000000 anyBSM-1.0/anyBSM/plotting.py
+-rw-rw-rw-   0 root         (0) root         (0)     7752 2023-05-05 01:22:24.000000 anyBSM-1.0/anyBSM/topologies.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 01:23:01.842673 anyBSM-1.0/anyBSM/ufo/
+-rw-rw-rw-   0 root         (0) root         (0)     1246 2023-05-05 01:22:24.000000 anyBSM-1.0/anyBSM/ufo/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      730 2023-05-05 01:22:24.000000 anyBSM-1.0/anyBSM/ufo/function_library.py
+-rw-rw-rw-   0 root         (0) root         (0)    12774 2023-05-05 01:22:24.000000 anyBSM-1.0/anyBSM/ufo/object_library.py
+-rw-rw-rw-   0 root         (0) root         (0)     6200 2023-05-05 01:22:24.000000 anyBSM-1.0/anyBSM/ufo/write_param_card.py
+-rw-rw-rw-   0 root         (0) root         (0)     4564 2023-05-05 01:22:24.000000 anyBSM-1.0/anyBSM/utils.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 01:23:01.833672 anyBSM-1.0/anyBSM.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      295 2023-05-05 01:23:01.000000 anyBSM-1.0/anyBSM.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     1323 2023-05-05 01:23:01.000000 anyBSM-1.0/anyBSM.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-05-05 01:23:01.000000 anyBSM-1.0/anyBSM.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      146 2023-05-05 01:23:01.000000 anyBSM-1.0/anyBSM.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)        7 2023-05-05 01:23:01.000000 anyBSM-1.0/anyBSM.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 01:23:01.842673 anyBSM-1.0/bin/
+-rwxrwxrwx   0 root         (0) root         (0)    12063 2023-05-05 01:22:24.000000 anyBSM-1.0/bin/anyBSM
+-rwxrwxrwx   0 root         (0) root         (0)    25624 2023-05-05 01:22:24.000000 anyBSM-1.0/bin/anyBSM_import
+-rw-rw-rw-   0 root         (0) root         (0)      694 2023-05-05 01:22:24.000000 anyBSM-1.0/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)       38 2023-05-05 01:23:01.845674 anyBSM-1.0/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)       88 2023-05-05 01:22:24.000000 anyBSM-1.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-05-05 01:23:01.844673 anyBSM-1.0/tests/
+-rw-rw-rw-   0 root         (0) root         (0)    32340 2023-05-05 01:22:24.000000 anyBSM-1.0/tests/test_SM.py
+-rw-rw-rw-   0 root         (0) root         (0)    50923 2023-05-05 01:22:24.000000 anyBSM-1.0/tests/test_THDM.py
+-rw-rw-rw-   0 root         (0) root         (0)     1007 2023-05-05 01:22:24.000000 anyBSM-1.0/tests/test_caching.py
+-rw-rw-rw-   0 root         (0) root         (0)     2583 2023-05-05 01:22:24.000000 anyBSM-1.0/tests/test_loopfunctions.py
+-rw-rw-rw-   0 root         (0) root         (0)      598 2023-05-05 01:22:24.000000 anyBSM-1.0/tests/test_unitarity.py
```

### Comparing `anyBSM-0.1/LICENSE` & `anyBSM-1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `anyBSM-0.1/README.md` & `anyBSM-1.0/README.md`

 * *Files 17% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 [![pipeline status](https://gitlab.com/anybsm/anybsm/badges/main/pipeline.svg)](https://gitlab.com/anybsm/anybsm/commits/main) 
 [![coverage report](https://gitlab.com/anybsm/anybsm/badges/main/coverage.svg)](https://gitlab.com/anybsm/anybsm/commits/main)
 
 
 <div align="center">
 
-![alt text](anyBSM/logos/anyH3logo_v1.png "anyH3 logo"){width=60% height=60%}
+![alt text](anyBSM/logos/anyH3_logo_large.png "anyH3 logo"){width=40% height=40%}
 
 </div>
 
 ## program purpose
 The idea of this program is to close tha gap regarding $`\kappa_\lambda`$ predictions in the landscape of BSM tool-boxes:
 ```mermaid
 graph LR
@@ -63,14 +63,20 @@
 [pdoc](https://pdoc.dev) is required to generate the documentation locally:
 ```
 pip3 install pdoc
 ./docs/make.py
 # now open /docs/docs/index.html in your browser
 ```
 
+## Journal references
+
+Henning Bahl, Johannes Braathen, Martin Gabelmann, Georg Weiglein
+<br/>*anyH3: precise predictions for the trilinear Higgs coupling in the Standard Model and beyond*  </br>                      
+e-Print: [arXiv:2305.03015](https://arxiv.org/abs/2305.03015)
+
 ## program flow
 
 ### program structure
 
 <div align="center">
 
 ![alt text](anyBSM/logos/program_structure.png "program structure"){width=90% height=90%}
```

### Comparing `anyBSM-0.1/anyBSM/Delta_r_SM.py` & `anyBSM-1.0/anyBSM/Delta_r_SM.py`

 * *Files identical despite different names*

### Comparing `anyBSM-0.1/anyBSM/__init__.py` & `anyBSM-1.0/anyBSM/__init__.py`

 * *Files identical despite different names*

### Comparing `anyBSM-0.1/anyBSM/anyBSM.py` & `anyBSM-1.0/anyBSM/anyBSM.py`

 * *Files identical despite different names*

### Comparing `anyBSM-0.1/anyBSM/anyEWPO.py` & `anyBSM-1.0/anyBSM/anyEWPO.py`

 * *Files identical despite different names*

### Comparing `anyBSM-0.1/anyBSM/anyH3.py` & `anyBSM-1.0/anyBSM/anyH3.py`

 * *Files identical despite different names*

### Comparing `anyBSM-0.1/anyBSM/anyModel.py` & `anyBSM-1.0/anyBSM/anyModel.py`

 * *Files 0% similar despite different names*

```diff
@@ -964,14 +964,15 @@
             self.parameters['SignSinThetaW'].value = 1
         elif abs(sign + 1) == 0:
             self.parameters['SignSinThetaW'].value = -1
         else:
             logger.error(f'Error! Right-handed FFV coupling has unexpected form {coupr}')
             return 'SignSinThetaW'
         self.all_parameters['SignSinThetaW'] = self.parameters['SignSinThetaW'].value
+        self.parameters['SignSinThetaW'].nvalue = self.all_parameters['SignSinThetaW']
         return self.parameters['SignSinThetaW'].value
 
     def load_renormalization_scheme(self, scheme_name: Union[None, str] = None) -> dict:
         """ Load a renormalization scheme from the model directories
         `scheme.yml`-file. The file should look like:
         ```yaml
         # default names for SM fields and parameters
```

### Comparing `anyBSM-0.1/anyBSM/anyPerturbativeUnitarity.py` & `anyBSM-1.0/anyBSM/anyPerturbativeUnitarity.py`

 * *Files identical despite different names*

### Comparing `anyBSM-0.1/anyBSM/anyProcess.py` & `anyBSM-1.0/anyBSM/anyProcess.py`

 * *Files identical despite different names*

### Comparing `anyBSM-0.1/anyBSM/config.py` & `anyBSM-1.0/anyBSM/config.py`

 * *Files identical despite different names*

### Comparing `anyBSM-0.1/anyBSM/diagrams.py` & `anyBSM-1.0/anyBSM/diagrams.py`

 * *Files identical despite different names*

### Comparing `anyBSM-0.1/anyBSM/latex/__init__.py` & `anyBSM-1.0/anyBSM/latex/__init__.py`

 * *Files identical despite different names*

### Comparing `anyBSM-0.1/anyBSM/latex/drawer.py` & `anyBSM-1.0/anyBSM/latex/drawer.py`

 * *Files 1% similar despite different names*

```diff
@@ -42,31 +42,31 @@
 def printparameters(parameters):
     string = ''
     r = 7 # number of digits
     ncol = 5 # number of columns
     colsep = 'l'.join(['' for i in range(ncol+1)])
     nparas = len(parameters)
     string += f'\\begin{{longtable}}{{{colsep}}}\n'
-    for i,p in enumerate(sorted(parameters, key=lambda x: x.name)):
-        if p.name == 'ZERO':
-            continue
+    for i,p in enumerate(sorted(parameters, key=lambda x: x.name.lower())):
         num = p.nvalue
         try:
             if abs(num.imag) > r+2:
                 num = str(round(num.real, r) + round(num.imag, r) * 1j)
             else:
                 num = str(round(num.real, r))
+            num = latex(sympify(num))
         except AttributeError:
+            logger.warning(f'cannot latexify parameter value {p.name}={p.nvalue}')
             num = '\\text{NaN}'
-        num = latex(sympify(num))
-        string += f'${p.texname} = {num}$'
-        if (i+1) % 4 == 0:
-            string += ', \\\\\n'
-        elif (i+1) != nparas:
-            string += ', & '
+        if p.name != 'ZERO':
+            string += f'${p.texname} = {num}$'
+            if (i+1) % ncol == 0:
+                string += ', \\\\\n'
+            elif (i+1) != nparas:
+                string += ', & '
     string += '\\end{longtable}'
     return string
 
 
 class DrawProcess():
     r""" Draw a list of Feynman diagrams along with their results.
     Upon initialization the header of the $\LaTeX$ file is written to the
@@ -94,15 +94,15 @@
         self.extnames = ','.join(particle_name(f) for f in externalfields)
         self.exttype = fieldtypes(externalfields)
         self.simplify = simplify
         self.cutoff = cutoff if cutoff is not True else False
         self.next = len(externalfields)
         self.insertions = defaultdict(dict)
         self.diagrams = defaultdict(dict)
-        options = f'Cut-off set to: {self._unit(cutoff)} (plotting only diagram with |result|>{self._unit(cutoff)}).' if self.cutoff else ''
+        options = f'Cut-off set to: ${self._unit(cutoff)}$ (plotting only diagram with |result|$>{self._unit(cutoff)}$).' if self.cutoff else ''
 
         with open(self.file, 'w') as f:
             f.write(f"""
 % MANUAL COMPILATION:
 % lualatex --halt-on-error {path.basename(self.file)}
 \\documentclass[11pt]{{article}}
 \\usepackage[margin=2.5cm]{{geometry}}
```

### Comparing `anyBSM-0.1/anyBSM/latex/printer.py` & `anyBSM-1.0/anyBSM/latex/printer.py`

 * *Files identical despite different names*

### Comparing `anyBSM-0.1/anyBSM/latex/tikzfeynman/LICENSE` & `anyBSM-1.0/anyBSM/latex/tikzfeynman/LICENSE`

 * *Files identical despite different names*

### Comparing `anyBSM-0.1/anyBSM/latex/tikzfeynman/tikzfeynman.keys.code.tex` & `anyBSM-1.0/anyBSM/latex/tikzfeynman/tikzfeynman.keys.code.tex`

 * *Files identical despite different names*

### Comparing `anyBSM-0.1/anyBSM/latex/tikzfeynman/tikzfeynman.patch.3.0.0.lua` & `anyBSM-1.0/anyBSM/latex/tikzfeynman/tikzfeynman.patch.3.0.0.lua`

 * *Files identical despite different names*

### Comparing `anyBSM-0.1/anyBSM/latex/tikzfeynman/tikzfeynman.patch.3.0.1.lua` & `anyBSM-1.0/anyBSM/latex/tikzfeynman/tikzfeynman.patch.3.0.1.lua`

 * *Files identical despite different names*

### Comparing `anyBSM-0.1/anyBSM/latex/tikzfeynman/tikzfeynman.sty` & `anyBSM-1.0/anyBSM/latex/tikzfeynman/tikzfeynman.sty`

 * *Files identical despite different names*

### Comparing `anyBSM-0.1/anyBSM/latex/tikzfeynman/tikzlibraryfeynman.code.tex` & `anyBSM-1.0/anyBSM/latex/tikzfeynman/tikzlibraryfeynman.code.tex`

 * *Files identical despite different names*

### Comparing `anyBSM-0.1/anyBSM/logos/anyH3_logo_large.png` & `anyBSM-1.0/anyBSM/logos/anyH3_logo_large.png`

 * *Files identical despite different names*

### Comparing `anyBSM-0.1/anyBSM/logos/anyH3_logo_plot.png` & `anyBSM-1.0/anyBSM/logos/anyH3_logo_plot.png`

 * *Files identical despite different names*

### Comparing `anyBSM-0.1/anyBSM/logos/anyH3_logo_small.png` & `anyBSM-1.0/anyBSM/logos/anyH3_logo_small.png`

 * *Files identical despite different names*

### Comparing `anyBSM-0.1/anyBSM/logos/class_structure.png` & `anyBSM-1.0/anyBSM/logos/class_structure.png`

 * *Files identical despite different names*

### Comparing `anyBSM-0.1/anyBSM/logos/program_structure.png` & `anyBSM-1.0/anyBSM/logos/program_structure.png`

 * *Files identical despite different names*

### Comparing `anyBSM-0.1/anyBSM/loopfunctions.py` & `anyBSM-1.0/anyBSM/loopfunctions.py`

 * *Files identical despite different names*

### Comparing `anyBSM-0.1/anyBSM/mathematica_interface/anyBSM.m` & `anyBSM-1.0/anyBSM/mathematica_interface/anyBSM.m`

 * *Files identical despite different names*

### Comparing `anyBSM-0.1/anyBSM/physic_utils.py` & `anyBSM-1.0/anyBSM/physic_utils.py`

 * *Files identical despite different names*

### Comparing `anyBSM-0.1/anyBSM/plotting.py` & `anyBSM-1.0/anyBSM/plotting.py`

 * *Files identical despite different names*

### Comparing `anyBSM-0.1/anyBSM/topologies.py` & `anyBSM-1.0/anyBSM/topologies.py`

 * *Files identical despite different names*

### Comparing `anyBSM-0.1/anyBSM/ufo/__init__.py` & `anyBSM-1.0/anyBSM/ufo/__init__.py`

 * *Files identical despite different names*

### Comparing `anyBSM-0.1/anyBSM/ufo/function_library.py` & `anyBSM-1.0/anyBSM/ufo/function_library.py`

 * *Files identical despite different names*

### Comparing `anyBSM-0.1/anyBSM/ufo/object_library.py` & `anyBSM-1.0/anyBSM/ufo/object_library.py`

 * *Files identical despite different names*

### Comparing `anyBSM-0.1/anyBSM/ufo/write_param_card.py` & `anyBSM-1.0/anyBSM/ufo/write_param_card.py`

 * *Files identical despite different names*

### Comparing `anyBSM-0.1/anyBSM/utils.py` & `anyBSM-1.0/anyBSM/utils.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from collections import Counter
 from os import path
 import sys
-import importlib
+import importlib.util
 import logging
 import pylha
 
 __doc__ = """ # AnyUtility
 A module to store all kinds of useful functions used accross different modules.
 """
```

### Comparing `anyBSM-0.1/anyBSM.egg-info/SOURCES.txt` & `anyBSM-1.0/anyBSM.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `anyBSM-0.1/bin/anyBSM` & `anyBSM-1.0/bin/anyBSM`

 * *Files identical despite different names*

### Comparing `anyBSM-0.1/bin/anyBSM_import` & `anyBSM-1.0/bin/anyBSM_import`

 * *Files identical despite different names*

### Comparing `anyBSM-0.1/pyproject.toml` & `anyBSM-1.0/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = [
   "setuptools>=42",
   "wheel"]
 
 [project]
 name = "anyBSM"
-version = "0.1"
+version = "1.0"
 authors = [
     {name = "Henning Bahl",      email = "hbahl@uchicago.edu"},
     {name = "Johannes Braathen", email = "johannes.braathen@desy.de"},
     {name = "Martin Gabelmann",  email = "martin.gabelmann@desy.de"},
     {name = "Georg Weiglein",    email = "georg.weiglein@desy.de"},
 ]
 requires-python = ">=3.5"
@@ -18,20 +18,20 @@
   "sympy",
   "tqdm",
   "pyyaml>=6.0",
   "pylha",
   "prettytable",
   "jinja2",
   "appdirs",
-  "gitpython"
+  "gitpython",
+  "pyCollier",
 ]
 
 [project.optional-dependencies]
 full = [
-  "pyCollier",
   "matplotlib",
   "numpy",
   "pandas",
   "prettytable",
   "pyyaml",
   "pdoc"
 ]
```

### Comparing `anyBSM-0.1/tests/test_SM.py` & `anyBSM-1.0/tests/test_SM.py`

 * *Files identical despite different names*

### Comparing `anyBSM-0.1/tests/test_THDM.py` & `anyBSM-1.0/tests/test_THDM.py`

 * *Files identical despite different names*

### Comparing `anyBSM-0.1/tests/test_caching.py` & `anyBSM-1.0/tests/test_caching.py`

 * *Files identical despite different names*

### Comparing `anyBSM-0.1/tests/test_loopfunctions.py` & `anyBSM-1.0/tests/test_loopfunctions.py`

 * *Files identical despite different names*

### Comparing `anyBSM-0.1/tests/test_unitarity.py` & `anyBSM-1.0/tests/test_unitarity.py`

 * *Files identical despite different names*

