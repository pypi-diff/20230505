# Comparing `tmp/BindingGP-0.0.36.tar.gz` & `tmp/BindingGP-0.0.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "BindingGP-0.0.36.tar", last modified: Fri May  5 12:50:32 2023, max compression
+gzip compressed data, was "dist\BindingGP-0.0.9.tar", last modified: Sat Sep 26 02:35:38 2020, max compression
```

## Comparing `BindingGP-0.0.36.tar` & `BindingGP-0.0.9.tar`

### file list

```diff
@@ -1,53 +1,46 @@
-drwxrwxrwx   0        0        0        0 2023-05-05 12:50:32.230016 BindingGP-0.0.36/
-drwxrwxrwx   0        0        0        0 2023-05-05 12:50:32.192791 BindingGP-0.0.36/BindingGP.egg-info/
--rw-rw-rw-   0        0        0     2351 2023-05-05 12:50:31.000000 BindingGP-0.0.36/BindingGP.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      951 2023-05-05 12:50:32.000000 BindingGP-0.0.36/BindingGP.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-05 12:50:31.000000 BindingGP-0.0.36/BindingGP.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       88 2023-05-05 12:50:31.000000 BindingGP-0.0.36/BindingGP.egg-info/requires.txt
--rw-rw-rw-   0        0        0        4 2023-05-05 12:50:32.000000 BindingGP-0.0.36/BindingGP.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     7797 2021-12-19 09:04:13.000000 BindingGP-0.0.36/LICENSE
--rw-rw-rw-   0        0        0       62 2021-12-19 09:04:13.000000 BindingGP-0.0.36/MANIFEST.in
--rw-rw-rw-   0        0        0     2351 2023-05-05 12:50:32.230016 BindingGP-0.0.36/PKG-INFO
--rw-rw-rw-   0        0        0     1314 2022-03-06 11:54:57.000000 BindingGP-0.0.36/README.md
-drwxrwxrwx   0        0        0        0 2023-05-05 12:50:32.200745 BindingGP-0.0.36/bgp/
--rw-rw-rw-   0        0        0      114 2021-12-19 09:04:13.000000 BindingGP-0.0.36/bgp/__init__.py
--rw-rw-rw-   0        0        0    59873 2022-09-28 13:42:27.000000 BindingGP-0.0.36/bgp/base.py
-drwxrwxrwx   0        0        0        0 2023-05-05 12:50:32.205801 BindingGP-0.0.36/bgp/calculation/
--rw-rw-rw-   0        0        0       52 2021-12-19 09:04:13.000000 BindingGP-0.0.36/bgp/calculation/__init__.py
--rw-rw-rw-   0        0        0    20718 2022-03-06 11:54:57.000000 BindingGP-0.0.36/bgp/calculation/coefficient.py
--rw-rw-rw-   0        0        0    20816 2023-04-26 10:53:33.000000 BindingGP-0.0.36/bgp/calculation/scores.py
--rw-rw-rw-   0        0        0     9504 2021-12-19 09:04:13.000000 BindingGP-0.0.36/bgp/calculation/translate.py
--rw-rw-rw-   0        0        0    26868 2023-04-26 13:18:35.000000 BindingGP-0.0.36/bgp/flow.py
-drwxrwxrwx   0        0        0        0 2023-05-05 12:50:32.212129 BindingGP-0.0.36/bgp/functions/
--rw-rw-rw-   0        0        0      519 2021-12-19 09:04:13.000000 BindingGP-0.0.36/bgp/functions/__init__.py
--rw-rw-rw-   0        0        0    17247 2022-08-13 08:39:55.000000 BindingGP-0.0.36/bgp/functions/dimfunc.py
--rw-rw-rw-   0        0        0     7247 2021-12-19 09:04:13.000000 BindingGP-0.0.36/bgp/functions/gsymfunc.py
--rw-rw-rw-   0        0        0     5024 2021-12-19 09:04:13.000000 BindingGP-0.0.36/bgp/functions/newfunc.py
--rw-rw-rw-   0        0        0     1705 2021-12-19 09:04:13.000000 BindingGP-0.0.36/bgp/functions/npfunc.py
--rw-rw-rw-   0        0        0     1562 2021-12-19 09:04:13.000000 BindingGP-0.0.36/bgp/functions/symfunc.py
--rw-rw-rw-   0        0        0    24106 2022-08-24 14:23:25.000000 BindingGP-0.0.36/bgp/gp.py
-drwxrwxrwx   0        0        0        0 2023-05-05 12:50:32.215310 BindingGP-0.0.36/bgp/iteration/
--rw-rw-rw-   0        0        0       40 2021-12-19 09:04:13.000000 BindingGP-0.0.36/bgp/iteration/__init__.py
--rw-rw-rw-   0        0        0     2563 2021-12-19 09:04:13.000000 BindingGP-0.0.36/bgp/iteration/newpoints.py
--rw-rw-rw-   0        0        0      159 2021-12-19 09:04:13.000000 BindingGP-0.0.36/bgp/iteration/nonewpoints.py
--rw-rw-rw-   0        0        0    17778 2023-05-05 12:47:47.000000 BindingGP-0.0.36/bgp/postprocess.py
--rw-rw-rw-   0        0        0     5267 2021-12-19 09:04:13.000000 BindingGP-0.0.36/bgp/preprocess.py
-drwxrwxrwx   0        0        0        0 2023-05-05 12:50:32.216311 BindingGP-0.0.36/bgp/probability/
--rw-rw-rw-   0        0        0       26 2021-12-19 09:04:13.000000 BindingGP-0.0.36/bgp/probability/__init__.py
--rw-rw-rw-   0        0        0    12258 2022-08-13 08:12:58.000000 BindingGP-0.0.36/bgp/probability/preference.py
--rw-rw-rw-   0        0        0    14307 2023-04-28 05:02:28.000000 BindingGP-0.0.36/bgp/skflow.py
--rw-rw-rw-   0        0        0      377 2021-12-19 09:04:13.000000 BindingGP-0.0.36/requirements.txt
--rw-rw-rw-   0        0        0       42 2023-05-05 12:50:32.230016 BindingGP-0.0.36/setup.cfg
--rw-rw-rw-   0        0        0     1906 2023-05-05 12:49:29.000000 BindingGP-0.0.36/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-05 12:50:32.227963 BindingGP-0.0.36/test/
--rw-rw-rw-   0        0        0     2186 2023-04-26 13:39:56.000000 BindingGP-0.0.36/test/test2.py
--rw-rw-rw-   0        0        0     3712 2022-08-13 07:57:08.000000 BindingGP-0.0.36/test/test_der.py
--rw-rw-rw-   0        0        0    11183 2021-12-19 09:04:13.000000 BindingGP-0.0.36/test/test_dim.py
--rw-rw-rw-   0        0        0     5561 2021-12-19 09:04:13.000000 BindingGP-0.0.36/test/test_function.py
--rw-rw-rw-   0        0        0     2575 2022-08-13 08:36:17.000000 BindingGP-0.0.36/test/test_one_sample.py
--rw-rw-rw-   0        0        0      547 2021-12-19 09:04:13.000000 BindingGP-0.0.36/test/test_preference.py
--rw-rw-rw-   0        0        0     2948 2022-08-13 08:44:54.000000 BindingGP-0.0.36/test/test_score.py
--rw-rw-rw-   0        0        0     1318 2022-08-13 08:12:58.000000 BindingGP-0.0.36/test/test_simp.py
--rw-rw-rw-   0        0        0     3107 2022-08-13 08:12:59.000000 BindingGP-0.0.36/test/test_symbol_base.py
--rw-rw-rw-   0        0        0     3822 2022-08-13 08:12:59.000000 BindingGP-0.0.36/test/test_symbol_gp.py
--rw-rw-rw-   0        0        0     2529 2022-08-13 08:46:11.000000 BindingGP-0.0.36/test/test_translate.py
+drwxrwxrwx   0        0        0        0 2020-09-26 02:35:38.000000 BindingGP-0.0.9/
+drwxrwxrwx   0        0        0        0 2020-09-26 02:35:38.000000 BindingGP-0.0.9/BGP/
+-rw-rw-rw-   0        0        0      108 2020-09-09 06:38:03.000000 BindingGP-0.0.9/BGP/__init__.py
+-rw-rw-rw-   0        0        0    50393 2020-09-26 02:22:00.000000 BindingGP-0.0.9/BGP/base.py
+drwxrwxrwx   0        0        0        0 2020-09-26 02:35:38.000000 BindingGP-0.0.9/BGP/calculation/
+-rw-rw-rw-   0        0        0       52 2020-09-09 06:15:05.000000 BindingGP-0.0.9/BGP/calculation/__init__.py
+-rw-rw-rw-   0        0        0    16380 2020-09-09 06:15:05.000000 BindingGP-0.0.9/BGP/calculation/coefficient.py
+-rw-rw-rw-   0        0        0    14474 2020-09-26 01:52:38.000000 BindingGP-0.0.9/BGP/calculation/scores.py
+-rw-rw-rw-   0        0        0     9367 2020-09-26 01:52:38.000000 BindingGP-0.0.9/BGP/calculation/translate.py
+-rw-rw-rw-   0        0        0    20247 2020-09-26 01:52:38.000000 BindingGP-0.0.9/BGP/flow.py
+drwxrwxrwx   0        0        0        0 2020-09-26 02:35:38.000000 BindingGP-0.0.9/BGP/functions/
+-rw-rw-rw-   0        0        0      519 2020-09-09 06:15:05.000000 BindingGP-0.0.9/BGP/functions/__init__.py
+-rw-rw-rw-   0        0        0    17226 2020-09-09 06:15:05.000000 BindingGP-0.0.9/BGP/functions/dimfunc.py
+-rw-rw-rw-   0        0        0     6291 2020-09-09 06:15:05.000000 BindingGP-0.0.9/BGP/functions/gsymfunc.py
+-rw-rw-rw-   0        0        0     5056 2020-09-26 01:52:38.000000 BindingGP-0.0.9/BGP/functions/newfunc.py
+-rw-rw-rw-   0        0        0     1548 2020-09-09 06:15:05.000000 BindingGP-0.0.9/BGP/functions/npfunc.py
+-rw-rw-rw-   0        0        0     1521 2020-09-09 06:15:05.000000 BindingGP-0.0.9/BGP/functions/symfunc.py
+-rw-rw-rw-   0        0        0     6366 2020-09-26 01:52:38.000000 BindingGP-0.0.9/BGP/gjj.py
+-rw-rw-rw-   0        0        0    23103 2020-09-26 01:52:38.000000 BindingGP-0.0.9/BGP/gp.py
+-rw-rw-rw-   0        0        0     5292 2020-09-09 06:15:05.000000 BindingGP-0.0.9/BGP/preprocess.py
+drwxrwxrwx   0        0        0        0 2020-09-26 02:35:38.000000 BindingGP-0.0.9/BGP/probability/
+-rw-rw-rw-   0        0        0       26 2020-09-09 06:15:05.000000 BindingGP-0.0.9/BGP/probability/__init__.py
+-rw-rw-rw-   0        0        0    12171 2020-09-26 02:22:00.000000 BindingGP-0.0.9/BGP/probability/preference.py
+-rw-rw-rw-   0        0        0    11173 2020-09-26 02:22:01.000000 BindingGP-0.0.9/BGP/skflow.py
+drwxrwxrwx   0        0        0        0 2020-09-26 02:35:38.000000 BindingGP-0.0.9/BindingGP.egg-info/
+-rw-rw-rw-   0        0        0     2672 2020-09-26 02:35:38.000000 BindingGP-0.0.9/BindingGP.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      806 2020-09-26 02:35:38.000000 BindingGP-0.0.9/BindingGP.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2020-09-26 02:35:38.000000 BindingGP-0.0.9/BindingGP.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      108 2020-09-26 02:35:38.000000 BindingGP-0.0.9/BindingGP.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        4 2020-09-26 02:35:38.000000 BindingGP-0.0.9/BindingGP.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     7797 2020-09-09 06:15:04.000000 BindingGP-0.0.9/LICENSE
+-rw-rw-rw-   0        0        0       62 2020-09-09 06:41:53.000000 BindingGP-0.0.9/MANIFEST.in
+-rw-rw-rw-   0        0        0     2672 2020-09-26 02:35:38.000000 BindingGP-0.0.9/PKG-INFO
+-rw-rw-rw-   0        0        0     1349 2020-09-26 02:34:10.000000 BindingGP-0.0.9/README.md
+-rw-rw-rw-   0        0        0      241 2020-09-09 06:45:18.000000 BindingGP-0.0.9/requirements.txt
+-rw-rw-rw-   0        0        0       42 2020-09-26 02:35:38.000000 BindingGP-0.0.9/setup.cfg
+-rw-rw-rw-   0        0        0     1871 2020-09-26 02:33:18.000000 BindingGP-0.0.9/setup.py
+drwxrwxrwx   0        0        0        0 2020-09-26 02:35:38.000000 BindingGP-0.0.9/test/
+-rw-rw-rw-   0        0        0    11183 2020-09-26 01:52:38.000000 BindingGP-0.0.9/test/test_dim.py
+-rw-rw-rw-   0        0        0     5561 2020-09-26 01:52:38.000000 BindingGP-0.0.9/test/test_function.py
+-rw-rw-rw-   0        0        0      547 2020-09-26 01:52:38.000000 BindingGP-0.0.9/test/test_preference.py
+-rw-rw-rw-   0        0        0     2917 2020-09-26 01:52:38.000000 BindingGP-0.0.9/test/test_score.py
+-rw-rw-rw-   0        0        0     1280 2020-09-26 01:52:38.000000 BindingGP-0.0.9/test/test_simp.py
+-rw-rw-rw-   0        0        0     3069 2020-09-26 01:52:38.000000 BindingGP-0.0.9/test/test_symbol_base.py
+-rw-rw-rw-   0        0        0     3784 2020-09-26 01:52:38.000000 BindingGP-0.0.9/test/test_symbol_gp.py
+-rw-rw-rw-   0        0        0     2493 2020-09-26 01:52:38.000000 BindingGP-0.0.9/test/test_translate.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive
+POSIX tar archive (GNU)
```

### Comparing `BindingGP-0.0.36/LICENSE` & `BindingGP-0.0.9/LICENSE`

 * *Files identical despite different names*

### Comparing `BindingGP-0.0.36/README.md` & `BindingGP-0.0.9/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,45 +1,43 @@
 <div align="center">
-  <img alt="BGP" src="https://github.com/MGEdata/bgp/blob/master/img.jpg?raw=true">
+  <img alt="BGP" src="https://github.com/MGEdata/BGP/blob/master/img.jpg?raw=true">
 </div>
 
-[![Python Versions](https://img.shields.io/pypi/pyversions/bindinggp.svg)](https://pypi.org/project/bindinggp/)
-[![Version](https://img.shields.io/github/tag/MGEdata/bgp.svg)](https://github.com/MGEdata/bgp/releases/latest)
-![pypi Versions](https://badge.fury.io/py/BindingGP.svg)
+[![Python Versions](https://img.shields.io/pypi/pyversions/bgp.svg)](https://pypi.org/project/bgp/)
+[![Version](https://img.shields.io/github/tag/MGEdata/BGP.svg)](https://github.com/MGEdata/BGP/releases/latest)
+![pypi Versions](https://badge.fury.io/py/bgp.svg)
 
 
 BGP
 ----------------------
 Welcome to BGP.
 
-BGP (Binding Genetic Programming) is an open python library that implements a comprehensive set of symbolic regression
-tools for materials informatics.
+BGP (Binding Genetic Programming) is a open python library that implements a comprehensive set of symbolic regression tools for materials informatics.
 
-This tool contains a symbol regression tool with dimension calculation, which is aimed at establish expressions with
-physical limitation.
+This tool contains a symbol regression tool with dimension calculation,
+which is aimed at establish expressions with physical limitation.
 
 BGP inspired by:
 
-[XenonPy](https://github.com/yoshida-lab/XenonPy),
-[matminer](https://hackingmaterials.github.io/matminer/ ),
-[deap](https://github.com/DEAP/deap),
-[sympy](https://www.sympy.org/en/index.html)
+  [XenonPy](https://github.com/yoshida-lab/XenonPy),
+  [matminer](https://hackingmaterials.github.io/matminer/ ),
+  [deap](https://github.com/DEAP/deap),
+  [sympy](https://www.sympy.org/en/index.html)
 
 Quick Install
 ----------------------
-
 ```bash
 pip install BindingGP
 ```
 
-Document
+[Document](https://boliqq07.github.io/BGPdocument/)
 ----------------------
-The usage of this package and **install** deatils are collected in BGP document.
+The **usage** of this package and **install** deatils are collected in BGP document.
 
-Turn to [BGP document](https://bgp.readthedocs.io/en/latest/) for more details.
+Turn to [BGP document](https://boliqq07.github.io/BGPdocument/) for more details.
 
 License
 ----------------------
 GNU LGPL-3.0 License
```

### Comparing `BindingGP-0.0.36/bgp/base.py` & `BindingGP-0.0.9/BGP/base.py`

 * *Files 7% similar despite different names*

```diff
@@ -3,77 +3,67 @@
 
 # @Time    : 2019/11/12 15:13
 # @Email   : 986798607@qq.com
 # @Software: PyCharm
 # @License: GNU Lesser General Public License v3.0
 
 """
-Base objects for symbolic regression.
-
-Contains:
-  - Class: ``SymbolSet``
-
-  - Class: ``CalculatePrecisionSet``
-
-  - Class: ``SymbolTree``
-
-  - others
+Notes:
+    this part is a customization from deap.
 """
 
 import copy
 import functools
 from collections.abc import Iterable
 
 import numpy as np
 import sympy
-from mgetool.tool import parallelize, batch_parallelize
+from BGP.calculation.scores import calcualte_dim_score, \
+    calculate_collect, compile_context, calculate_cv_score, score_collection
+from BGP.calculation.translate import group_str
+from BGP.functions.dimfunc import dim_map, Dim, dnan, dless
+from BGP.functions.gsymfunc import gsym_map, NewArray
+from BGP.functions.npfunc import np_map
+from BGP.functions.symfunc import sym_vector_map, sym_dispose_map
+from BGP.gp import genGrow, genFull, depart
+from BGP.probability.preference import PreMap
+from mgetool.tool import parallelize
 from sklearn.metrics import r2_score
 from sklearn.utils import check_X_y, check_array
 
-from bgp.calculation.coefficient import try_add_coef_times
-from bgp.calculation.scores import calcualte_dim_score, compile_context, calculate_cv_score, score_collection, \
-    calculate_collect_
-from bgp.calculation.translate import group_str
-from bgp.functions.dimfunc import dim_map, Dim, dnan, dless
-from bgp.functions.gsymfunc import gsym_map, NewArray
-from bgp.functions.npfunc import np_map
-from bgp.functions.symfunc import sym_vector_map, sym_dispose_map
-from bgp.gp import genGrow, genFull, depart
-from bgp.probability.preference import PreMap
-
 
 class SymbolTerminal:
-    """General feature type, do not use directly.\n
+    """General feature type.\n
     The name for show (str) and calculation (repr) are set to different string for
     avoiding repeated calculations.
     """
 
     def __init__(self, name, init_name=None):
         """
 
         Parameters
         ----------
         name: str
             Represent name. Default "xi".
         init_name: str
             Just for show, rather than calculate.\n
-            Examples:
-                init_name=[x1, x2] , if is compact features, need[].\n
-                init_name=(x1*x4-x3), if is expr, need ().
+            Examples:\n
+            init_name=[x1,x2] , if is compact features, need[]\n
+            init_name=(x1*x4-x3), if is expr, need ()
         """
         self.name = str(name)
         self.conv_fct = str
         self.arity = 0
         if init_name is None:
             self.init_name = None
         else:
             self.init_name = str(init_name)
 
     def format_repr(self):
-        # short, repr
+        # short,repr
         """representing name"""
         return self.conv_fct(self.name)
 
     def format_str(self):
         # long.str
         """represented name"""
         if self.init_name:
@@ -107,29 +97,29 @@
 
     def __init__(self, values, name, dim=None, prob=None, init_sym=None, init_name=None):
         """
 
         Parameters
         ----------
         values: None, number or np.ndarray
-            xi value, the shape can be (n, ) or (n_x, n), 
+            xi value, the shape can be (n,) or (n_x,n),
             n is number of samples, n_x is numbers of feature.
         name: str
             Represent name. Default "xi"
-        dim: bgp.dim.Dim or None
-            None.
+        dim: BGP.dim.Dim or None
+            None
         prob: float or None
-            None.
+            None
         init_sym: list, sympy.Expr
-            list.
+            list
         init_name: str or None 
             Just for show, rather than calculate.\n
-            Examples:
-                init_name="[x1, x2]" , if is compact features, need[].\n
-                init_name="(x1*x4-x3)", if is expr, need ().
+            Examples:\n
+            init_name="[x1,x2]" , if is compact features, need[]\n
+            init_name="(x1*x4-x3)", if is expr, need ()
         """
         super(SymbolTerminalDetail, self).__init__(name, init_name)
         if prob is None:
             prob = 1
         if dim is None:
             dim = dless
         self.value = values
@@ -138,23 +128,23 @@
         self.dim = dim
         self.prob = prob
 
     def capsule(self):
         return SymbolTerminal(self.name, self.init_name)
 
 
-def _tsum(*ters, name="gx0"):
+def tsum(*ters, name="gx0"):
     """
 
     Parameters
     ----------
     ters: tuple of SymbolTerminalDetail
         SymbolTerminalDetail
     name: str
-        specific the name of results.
+        sepcific the name of results.
 
     Returns
     -------
     SymbolTerminalDetail
     """
 
     for i in ters:
@@ -167,28 +157,24 @@
     prob = sum([i.prob for i in ters]) / len(ters)
     res = SymbolTerminalDetail(values, name, dim=dim, prob=prob,
                                init_sym=sym, init_name=str(list(sym)))
     return res
 
 
 class SymbolPrimitive:
-    """General operator type, do not use directly,
-    but use SymbolPrimitiveDetail."""
+    """General operation type"""
 
     def __init__(self, name, arity):
         """
-
         Parameters
         ----------
         name: str
-            function name.
+            function name
         arity: int
-            input parameters numbers of function.
-            such as ``+`` with 2, ``ln`` with 1.
-
+            function input numbers
         """
         self.name = str(name)
         self.arity = arity
         self.args = list(range(arity))
 
         args = ", ".join(map("{{{0}}}".format, list(range(self.arity))))
         self.seq = "{name}({args})".format(name=self.name, args=args)
@@ -207,63 +193,51 @@
     def __str__(self):
         return self.name
 
     __repr__ = __str__  # for function the format for machine and user is the same.
 
 
 class SymbolPrimitiveDetail(SymbolPrimitive):
-    """
-    General operator type with more details.
-    """
-
     def __init__(self, name, arity, func, prob, np_func=None, dim_func=None, sym_func=None):
         """
         Parameters
         ----------
-
         func: Callable
-            function. better using sympy.Function Type.\n
+            function. Better for sympy.Function Type.\n
             For Maintainer:
-                If self function and can not be simplified to sympy.Function or elementary function, 
-                the function for function.np_map() and dim.dim_map() should be defined.
+            If self function and can not be simplified to sympy.Function or elementary function,
+            the function for function.np_map() and dim.dim_map() should be defined.
         name: str
-            function name.
+            function name
         arity: int
-            function input numbers.
+            function input numbers
         prob: float
-            default 1.
+            default 1
         """
         super(SymbolPrimitiveDetail, self).__init__(name, arity)
 
         if prob is None:
             prob = 1
         self.func = func
         self.prob = prob
         self.np_func = np_func
         self.dim_func = dim_func
         self.sym_func = sym_func
 
     def capsule(self):
-        """return short one."""
         return SymbolPrimitive(self.name, self.arity)
 
 
 class SymbolSet(object):
     """
-    Definite the preparation set of operations, features, and fixed constants.
+    Definite the operations, features, and fixed constants.
     """
 
     def __init__(self, name="PSet"):
-        """
-
-        Parameters
-        ----------
-        name: str
-            name.
-        """
+        """Definite the preparation set of operations, features, and fixed constants."""
         self.arguments = []  # for translate
         self.name = name
         self.y = None  # data y
         self.y_dim = dless  # dim y
 
         self.data_x_dict = {}  # data x
 
@@ -289,20 +263,20 @@
         self.ter_con_dict = {}  # term and const
         self.dim_ter_con = {}  # Dim of and features and constants
         self.prob_ter_con = {}  # probability of and features and constants
 
         self.gro_ter_con = {}  # for group size calculation and simple
 
         self.terminals_init_map = {}  # for Tree show
-        # terminals representing name "gx0" to represented name "[x1, x2]", 
-        # or "newx0" to represented name "Add(Mul(x2, x4)+[x1, x2])".
+        # terminals representing name "gx0" to represented name "[x1,x2]",
+        # or "newx0" to represented name "Add(Mul(x2,x4)+[x1,x2])".
 
         self.terminals_symbol_map = {}  # for Tree show
-        # terminals representing name "gx0" to represented name "[x1, x2]", 
-        # or "newx0" to represented name "Add(Mul(x2, x4)+[x1, x2])".
+        # terminals representing name "gx0" to represented name "[x1,x2]",
+        # or "newx0" to represented name "Add(Mul(x2,x4)+[x1,x2])".
 
         self.expr_init_map = {}  # for expr show
         # terminals representing name "newx0" to represented name "(x2*x4+gx0)"
         self.terminals_fea_map = {}  # for terminals Latex feature name show.
 
         self.premap = PreMap.from_shape(3)
         self.x_group = [[]]
@@ -318,15 +292,15 @@
         """
         Parameters
         ----------
         name: str
             function name
         func: Callable
             function. Better for sympy.Function Type.
-            If self function and can not be simplified to sympy.Function or elementary function, 
+            If self function and can not be simplified to sympy.Function or elementary function,
             the function for np_func and dim_func should be defined.
         arity: int
             function input numbers
         prob: float
             default 1
         np_func: Callable
             numpy function or function constructed by numpy function
@@ -355,15 +329,15 @@
         """
         Parameters
         ----------
         name: str
             function name
         func: Callable
             function. Better for sympy.Function Type.
-            If self function and can not be simplified to sympy.Function or elementary function, 
+            If self function and can not be simplified to sympy.Function or elementary function,
             the function for np_func and dim_func should be defined.
         arity: 1
             function input numbers, must be 1
         prob: float
             default 1/n, n is structure function number.
         np_func: Callable
             numpy function or function constructed by numpy function
@@ -386,22 +360,22 @@
 
     def _add_terminal(self, value, name, dim=None, prob=None, init_sym=None, init_name=None):
         """
         Parameters
         ----------
         name: str
             function name
-        value: numpy.ndarray, ndarray
+        value: numpy.ndarray
             xi value
         prob: float
             default 1
         init_name: str
             True name can be found of input. Just for show, rather than calculate.
             Examples:
-            init_name="[x1, x2]" , if is compact features, need[]
+            init_name="[x1,x2]" , if is compact features, need[]
             init_name="(x1*x4-x3)", if is expr, need ()
         dim: Dim
             xi Dim
         """
 
         if prob is None:
             prob = 1
@@ -411,23 +385,23 @@
         self.ter_con_dict[name] = SymbolTerminalDetail(value, name, dim=dim, prob=prob,
                                                        init_sym=init_sym,
                                                        init_name=init_name)
         self.terms_count += 1
 
     def register(self, primitives_dict="all", dispose_dict="all", ter_con_dict="all"):
         """
-        Register and capsule for simplify.
+        Register and capsule for simpify.
         
         Parameters
         ----------
-        primitives_dict:None, str, dict
+        primitives_dict:None,str,dict
         
-        dispose_dict:None, str, dict
+        dispose_dict:None,str,dict
         
-        ter_con_dict:None, str, dict
+        ter_con_dict:None,str,dict
 
         """
         if primitives_dict == "all":
             primitives_dict = self.primitives_dict
         if dispose_dict == "all":
             dispose_dict = self.dispose_dict
         if ter_con_dict == "all":
@@ -455,54 +429,56 @@
                     self.dim_map[p.name] = p.dim_func
                 self.prob_dispose[p.name] = p.prob
                 self.context[p.name] = p.func
                 self.dispose_dict[p.name] = self.dispose_dict[p.name].capsule()
 
         if ter_con_dict is not None:
             for t in ter_con_dict.values():
-
-                if t.dim.ndim == 1:
-                    ng = 1
-                elif t.dim.ndim == 2:
-                    ng = t.dim.shape[0]
+                if t.name in self.data_x_dict:
+                    pass
                 else:
-                    ng = 1
-
-                self.gro_ter_con[t.name] = ng
-                self.dim_ter_con[t.name] = t.dim
-                self.prob_ter_con[t.name] = t.prob
-                self.data_x_dict[t.name] = t.value
-
-                self.context[t.name] = sympy.Symbol(t.name)
-
-                if t.init_name:
-                    self.terminals_init_map[t.name] = t.init_name
-                    if isinstance(t.init_sym, (np.ndarray, NewArray)):
-                        self.terminals_symbol_map[t.name] = t.init_sym
+                    if t.dim.ndim == 1:
+                        ng = 1
+                    elif t.dim.ndim == 2:
+                        ng = t.dim.shape[0]
                     else:
-                        self.expr_init_map[t.name] = t.init_sym
-                self.ter_con_dict[t.name] = self.ter_con_dict[t.name]
+                        ng = 1
+
+                    self.gro_ter_con[t.name] = ng
+                    self.dim_ter_con[t.name] = t.dim
+                    self.prob_ter_con[t.name] = t.prob
+                    self.data_x_dict[t.name] = t.value
+
+                    self.context[t.name] = sympy.Symbol(t.name)
+
+                    if t.init_name:
+                        self.terminals_init_map[t.name] = t.init_name
+                        if isinstance(t.init_sym, (np.ndarray, NewArray)):
+                            self.terminals_symbol_map[t.name] = t.init_sym
+                        else:
+                            self.expr_init_map[t.name] = t.init_sym
+                    self.ter_con_dict[t.name] = self.ter_con_dict[t.name].capsule()
 
     def _group(self, x_group=None):
         if not x_group:
             x_group = self.x_group
         if isinstance(x_group, int):
-            assert self.terms_count > x_group > 1, "the len of group should in (2, x.shape[1]]"
+            assert self.terms_count > x_group > 1, "the len of group should in (2,x.shape[1]]"
             indexes = [_ for _ in range(self.terms_count)]
             x_group = [indexes[i:i + x_group] for i in range(0, len(indexes), x_group)]
 
         x_group = [x_groupi for x_groupi in x_group if len(x_groupi) >= 2]
 
         for i, gi in enumerate(x_group):
             len_gi = len(gi)
             if len_gi > 0:
                 init_ter_name = ["x%s" % j for j in gi]
                 init_ter = [self.ter_con_dict.pop(i) for i in init_ter_name]
                 name = "gx%s" % i
-                ter = _tsum(*init_ter, name=name)
+                ter = tsum(*init_ter, name=name)
                 self.ter_con_dict[name] = ter
 
                 self.terms_count -= (len(init_ter) - 1)
 
     def _add_constant(self, value, name=None, dim=None, prob=None):
         """
         Parameters
@@ -532,62 +508,55 @@
     def add_operations(self, power_categories=None, categories=None, self_categories=None,
                        power_categories_prob="balance", categories_prob="balance", special_prob=None):
         """
         Add operations with probability.
 
         Parameters
         ----------
-        power_categories: Sized, tuple, None
-            Examples:
-                (0.5, 2, 3)
+
+        power_categories: Sized,tuple, None
+            Examples:(0.5,2,3)
         categories: tuple of str
             map table:
-                {'Add': sympy.Add, 'Sub': Sub, 'Mul': sympy.Mul, 'Div': Div}
-                {"sin": sympy.sin, 'cos': sympy.cos, 'exp': sympy.exp, 'ln': sympy.ln, }
-                {'Abs': sympy.Abs, "Neg": functools.partial(sympy.Mul, -1.0), }
-                "Rec": functools.partial(sympy.Pow, e=-1.0)}
-
-                Others:  \n
-                "Rem":  f(x)=1-x, if x true \n
-                "Self":  f(x)=x, if x true \n
-        categories_prob: "balance", float
-            probability of categories, except (+, -*, /), in (0, 1].
-            "balance" is 1/n_categories.
-            The (+, -*, /) are set as 1 to be a standard.
-        special_prob: None, dict
-            prob for special name.\n
-            Examples:{"Mul":0.6, "Add":0.4, "exp":0.1}
-        power_categories_prob: "balance", float
-            float in (0, 1].
-            probability of power categories, "balance" is 1/power_categories_prob.
-        self_categories:list of dict, None
-            the dict can be generate from newfuncV or definition self.\n
-            the function at least containing:
-            {"func": func, "name": name, "arity":2, "np_func": npf, "dim_func": dimf, "sym_func": gsymf}
-
-            1.func:sympy.Function(name) object
-
-            2.name:name
+                    {"Add": sympy.Add, 'Sub': Sub, 'Mul': sympy.Mul, 'Div': Div}
 
-            3.arity:int, the number of parameter
+                    {"sin": sympy.sin, 'cos': sympy.cos, 'exp': sympy.exp, 'ln': sympy.ln,
 
-            4.np_func:numpy function
+                    {'Abs': sympy.Abs, "Neg": functools.partial(sympy.Mul, -1.0),
+                    
+                    "Rec": functools.partial(sympy.Pow, e=-1.0)}
 
-            5.dim_func:dimension function
+                    Others:  \n
+                    "Rem":  f(x)=1-x,if x true \n
+                    "Self":  f(x)=x,if x true \n
 
-            6.sym_func:NewArray function. (unpack the group, used just for shown)
-
-            See Also bgp.newfunc.newfuncV
+        power_categories_prob:"balance", float
+            float in (0,1]
+            probability of power categories, "balance" is 1/n_power_cat
+        categories_prob: "balance", float
+            float in (0,1]
+            probabilityty of categories, except (+,-*,/), "balance" is 1/n_categories.\n
+            Notes: the  (+,-*,/) are set as 1 to be a standard.
+        special_prob: None or dict
+            Examples: {"Mul":0.6,"Add":0.4,"exp":0.1}
+        self_categories:list of dict,None
+            the dict can be generate from newfuncV or defination self.
+            the function at least containing:
+            {"func": func, "name": name, "arity":2,"np_func": npf, "dim_func": dimf, "sym_func": gsymf}
+            func:sympy.Function(name) object
+            name:name
+            arity:int,the number of parameter
+            np_func:numpy function
+            dim_func:dimension function
+            sym_func:NewArray function. (unpack the group,used just for shown)
+            See Also BGP.newfunc.newfuncV
+        Returns
+        -------
+        SymbolSet
         """
-
-        """        
-
-
-
-"""
         if categories is None:
             categories = ("Add", "Mul", "Self", "exp")
 
         def change(n, p):
             if isinstance(special_prob, dict):
                 if n in special_prob:
                     p = special_prob[n]
@@ -599,15 +568,15 @@
         functions1, functions2 = sym_vector_map()
         if power_categories:
             if power_categories_prob == "balance":
                 prob = 1 / len(power_categories)
             elif isinstance(power_categories_prob, float):
                 prob = power_categories_prob
             else:
-                raise TypeError("power_categories_prob accept float from (0, 1] or 'balance'.")
+                raise TypeError("power_categories_prob accept float from (0,1] or 'balance'.")
             for j, i in enumerate(power_categories):
                 name = 'pow%s' % j
                 prob = change(name, prob)
                 self._add_primitive(functools.partial(sympy.Pow, e=i),
                                     arity=1, name='pow%s' % j, prob=prob)
 
         for i in categories:
@@ -616,71 +585,60 @@
                 if len(ca_new) >= 1:
                     prob1 = 1 / len(ca_new)
                 else:
                     prob1 = 1
             elif isinstance(categories_prob, float):
                 prob1 = categories_prob
             else:
-                raise TypeError("categories_prob accept float from (0, 1] or 'balance'.")
+                raise TypeError("categories_prob accept float from (0,1] or 'balance'.")
             if i in functions1:
                 prob1 = change(i, prob1)
                 self._add_primitive(functions1[i], arity=1, name=i, prob=prob1)
             if i in functions2:
                 prob2 = change(i, 1)
                 self._add_primitive(functions2[i], arity=2, name=i, prob=prob2)
 
         if self_categories:
             for i in self_categories:
                 prob = change(i, 0.2)
                 i["prob"] = prob
                 i["arity"] = 1
-                self._add_primitive(**i)
+                self._add_dispose(*i)
         self.register(primitives_dict="all", dispose_dict=None, ter_con_dict=None)
         return self
 
     def add_accumulative_operation(self, categories=None, categories_prob="balance",
                                    self_categories=None, special_prob=None):
         """
-        add accumulative operation.
 
         Parameters
         ----------
         categories: tuple of str
-            categories=("Self", "MAdd", "MSub", "MMul", "MDiv")
+            categories=("Self","MAdd","MSub", "MMul","MDiv")
         categories_prob: None, "balance" or float.
-            probility of categories in (0, 1], except ("Self", "MAdd", "MSub", "MMul", "MDiv"),
-
+            probility of categories  (0,1], except ("Self","MAdd", "MSub", "MMul", "MDiv"),
             "balance" is 1/n_categories.
-
-            "MSub", "MMul", "MDiv" are only worked on the size of group is 2, else work like "Self".
-
-            Notes:
-                the  ("Self", "MAdd", "MSub", "MMul", "MDiv") are set as 1 to be a standard.
-        self_categories:list of dict, None
-            the dict can generate from newfuncD or defination self.
-
+            "MSub", "MMul", "MDiv" only work on the size of group is 2, else work like "Self".
+            Notes: the  ("Self","MAdd","MSub", "MMul", "MDiv") are set as 1 and 0.1 to be a standard.
+        self_categories:list of dict,None
+            the dict can be generate from newfuncD or defination self.
             the function at least containing:
-
             {"func": func, "name": name, "np_func": npf, "dim_func": dimf, "sym_func": gsymf}
-
-            1.func:sympy.Function(name) object, which need add attributes: is_jump, keep.
-
-            2.name:name
-
-            3.np_func:numpy function
-
-            4.dim_func:dimension function
-
-            5.sym_func:NewArray function. (unpack the group, used just for shown)
-
-            See Also bgp.newfunc.newfuncV
-
+            func:sympy.Function(name) object,which need add attributes: is_jump,keep.
+            name:name
+            np_func:numpy function
+            dim_func:dimension function
+            sym_func:NewArray function. (unpack the group,used just for shown)
+            See Also BGP.newfunc.newfuncV
         special_prob: None or dict
-            Examples:
-                {"MAdd":0.5, "Self":0.5}
+            Examples: {"MAdd":0.5,"Self":0.5}
+
+        Returns
+        -------
+        SymbolSet
         """
 
         def change(n, pp):
             if isinstance(special_prob, dict):
                 if n in special_prob:
                     pp = special_prob[n]
             return pp
@@ -703,15 +661,15 @@
             if len(ca_new) >= 1:
                 prob1 = 1.0 / len(ca_new)
             else:
                 prob1 = 1.0
         elif isinstance(categories_prob, float):
             prob1 = categories_prob
         else:
-            raise TypeError("categories_prob accept float from (0, 1] or 'balance'.")
+            raise TypeError("categories_prob accept float from (0,1] or 'balance'.")
 
         for i in categories:
 
             if i == "Self":
                 p = change(i, 0.5)
                 self._add_dispose(sym_dispose_map()[i], arity=1, name=i, prob=p)
             elif i in ("MAdd", "MSub", "MMul", "MDiv"):
@@ -733,23 +691,27 @@
                 self._add_dispose(*i)
         self.register(primitives_dict=None, dispose_dict="all", ter_con_dict=None)
         return self
 
     def add_tree_to_features(self, Tree, prob=0.3):
         """
         Add the individual as a new feature to initial features.
-        not sure add success, because the value and name should be check and
+        not sure add seccess,because the value and name should be check and
         different to exist.
 
         Parameters
         ----------
         Tree: SymbolTree
             individual or expression
         prob: int
             probability of this individual
+
+        Returns
+        -------
+        SymbolSet
         """
         try:
             value = Tree.pre_y
             check_array(value, ensure_2d=False)
 
             eq = any([np.all(np.equal(value, i)) for i in self.data_x_dict.values()])
             if eq:
@@ -772,15 +734,15 @@
 
             # self.expr are not passed
             t_map_va = list(self.expr_init_map.keys())
             t_map_va.reverse()
             for i in t_map_va:
                 init_name1 = init_name1.subs(sympy.Symbol(i), self.expr_init_map[i])
 
-        except(AssertionError, NameError, ValueError, TypeError):
+        except(AssertionError, NameError, ValueError):
             pass
         else:
             name = "new%s" % self.new_num
             Tree.p_name = name
             self._add_terminal(value, name, dim=dim, prob=prob,
                                init_sym=init_name1, init_name=init_name0)
             self.premap = self.premap.add_new()
@@ -793,42 +755,44 @@
 
         """
         Add features with dimension and probability.
 
         Parameters
         ----------
         X: np.ndarray
-            2D data.
+            2D data
         y: np.ndarray
-            1D data.
+            1D data
         feature_name: None, list of str
-            the same size wih x.shape[1].
+            the same size wih x.shape[1]
         x_dim: 1 or list of Dim
-            the same size wih x.shape[1], default 1 is dless for all x.
-        y_dim: 1, Dim
-            dim of y.
-        x_prob: None, list of float
-            the same size wih x.shape[1].
+            the same size wih x.shape[1], default 1 is dless for all x
+        y_dim: 1,Dim
+            dim of y
+        x_prob: None,list of float
+            the same size wih x.shape[1]
         x_group: None or list of list, int
-            features group.
+            features group
 
+        Returns
+        -------
+        SymbolSet
         """
         X = X.astype(np.float32)
         y = y.astype(np.float32)
         X, y = check_X_y(X, y)
 
         # define terminal
         n = X.shape[1]
         self.y = y.ravel()
-
-        if y_dim == 1:
+        if y_dim is 1:
             y_dim = dless
         self.y_dim = y_dim
 
-        if x_dim == 1:
+        if x_dim is 1:
             x_dim = [dless for _ in range(n)]
 
         if x_prob is None:
             x_prob = [1.0 for _ in range(n)]
         elif isinstance(x_prob, (float, int)):
             x_prob = [float(x_prob) for _ in range(n)]
         if isinstance(feature_name, list):
@@ -847,70 +811,53 @@
         self.x_group = x_group
         self._group(x_group)
 
         self.register(primitives_dict=None, dispose_dict=None, ter_con_dict="all")
         self.premap = PreMap.from_shape(len(self.ter_con_dict))
         return self
 
-    def replace(self, X, y=None, tree_X=None):
-        X = X.astype(np.float32)
-        if y is not None:
-            y = y.astype(np.float32)
-            X, y = check_X_y(X, y)
-
-        self.y = y.ravel()
-
+    def replace(self, X):
         old = self.terms_count
         self.terms_count = 0
         # self.ter_con_dict={}
         n = X.shape[1]
         for i in range(n):
             self._add_terminal(np.array(X.T[i]), name="x%s" % i)
 
         self._group(self.x_group)
 
-        if isinstance(tree_X, np.ndarray):
-            tree_X = tree_X.astype(np.float32)
-            n = tree_X.shape[1]
-            for i in range(n):
-                self._add_terminal(np.array(tree_X.T[i]), name="new%s" % i)
-
-        elif isinstance(tree_X, dict):
-            for k, v in tree_X.items():
-                v = v.astype(np.float32)
-                self._add_terminal(np.array(v), name=v)
-
-        assert old == self.terms_count, "the new X (test, predict) should be with the " \
-                                        "same shape[1] with old X (fit, train). when use re_tree, " \
-                                        "the tree_X should be offered"
+        assert old == self.terms_count, "the new X (test,predict) should be with the " \
+                                        "same shape[1] with old X (fit,train)"
 
         self.register(primitives_dict=None, dispose_dict=None, ter_con_dict="all")
-        if y is not None:
-            self.y = y
         return self
 
     def add_constants(self, c, c_dim=1, c_prob=None):
         """
         Add features with dimension and probability.
 
         Parameters
         ----------
         c_dim: 1, list of Dim
-            the same size wih c.
-        c: float, list
-            list of float.
+            the same size wih c
+        c: float,list
+            list of float
         c_prob: None, float, list of float
-            the same size with c.
+            the same size wih c
+
+        Returns
+        -------
+        SymbolSet
         """
         if isinstance(c, float):
             c = [c, ]
 
         n = len(c)
 
-        if c_dim == 1:
+        if c_dim is 1:
             c_dim = [dless for _ in range(n)]
 
         if c_prob is None:
             c_prob = [0.1 for _ in range(n)]
         elif isinstance(c_prob, (float, int)):
             c_prob = [c_prob for _ in range(n)]
 
@@ -922,48 +869,47 @@
         self.register(primitives_dict=None, dispose_dict=None, ter_con_dict="all")
         self.premap = PreMap.from_shape(len(self.ter_con_dict))
         # re-generate each time.
         return self
 
     def add_features_and_constants(self, X, y, c=None, x_dim=1, y_dim=1, c_dim=1, x_prob=None,
                                    c_prob=None, x_group=None, feature_name=None):
-        """combination of add_constant and add_features."""
         self.add_features(X, y, x_dim=x_dim, y_dim=y_dim, x_prob=x_prob, x_group=x_group,
                           feature_name=feature_name, )
         if c is not None:
             self.add_constants(c, c_dim=c_dim, c_prob=c_prob)
 
     def set_personal_maps(self, pers):
         """
-        personal preference add to permap. more control can be found by pset.premap.***\n
+        Personal preference add to permap. more control can be found by pset.premap.***\n
         Just set couples of points and don't chang others.
 
         Parameters
         ----------
         pers : list of list
             Examples:
-                [[index1, index2, prob]],
-                the prob in [0, 1).
+                [[index1,index2,prob]]
+                the prob in [0,1).
         """
         for i in pers:
             self.premap.set_sigle_point(*i)
 
     def bonding_personal_maps(self, pers):
         """
-        Personal preference add to permap more control can be found by pset.premap\n
+        Personal preference add to permap. more control can be found by pset.premap.***\n
         Bond the points with ratio. the others would be penalty.\n
-        For example set the [1, 2, 0.9], 
-        the others bond such as (1, 2), (1, 3), (1, 4),...,(2, 3), (2, 4)...would be with small prob.
+        For example set the [1,2,0.9],
+        the others bond such as (1,2),(1,3),(1,4)...(2,3),(2,4)...would be with small prob.
 
         Parameters
         ----------
         pers : list of list
             Examples:
-                [[index1, index2, prob][...]]
-                the prob is [0, 1), 1 means the force binding.
+                [[index1,index2,prob][...]]
+                the prob is [0,1), 1 means the force binding.
         """
         for i in pers:
             self.premap.down_other_point(*i)
 
     @property
     def terminalRatio(self):
         """Return the ratio of the number of terminals on the number of all
@@ -995,15 +941,14 @@
 
     @property
     def dim_ter_con_list(self):
         return self.get_values(self.dim_ter_con, mean=False)
 
     @property
     def primitives(self):
-        """operators"""
         return self.get_values(self.primitives_dict, mean=False)
 
     @property
     def types(self):
         if self.gro_ter_con:
             ln = list(self.gro_ter_con.values())
             ln.append(1)
@@ -1019,20 +964,18 @@
         else:
             raise NotImplementedError("the question type are defined by 'group' "
                                       "parameters in .add_features"
                                       "please add features before add operations.")
 
     @property
     def dispose(self):
-        """accumulate operators"""
         return self.get_values(self.dispose_dict, mean=False)
 
     @property
     def terminals_and_constants(self):
-        """terminals_and_constants"""
         return self.get_values(self.ter_con_dict, mean=False)
 
     @property
     def terminals_and_constants_repr(self):
         return [sympy.Symbol(repr(i)) for i in self.terminals_and_constants]
 
     @property
@@ -1064,14 +1007,15 @@
         return terminals
 
 
 class _ExprTree(list):
     """
     Tree of expression
     """
+    hasher = repr
 
     def __init__(self, content):
         list.__init__(self, content)
 
     def __deepcopy__(self, memo=None):
         new = self.__class__(self)
         new.__dict__.update(copy.deepcopy(self.__dict__))
@@ -1092,15 +1036,15 @@
             for node in val[1:]:
                 total += node.arity - 1
             if total != 0:
                 raise ValueError("Invalid slice assignation : insertion of"
                                  " an incomplete subtree is not allowed in PrimitiveTree."
                                  " A tree is defined as incomplete when some nodes cannot"
                                  " be mapped to any position in the tree, considering the"
-                                 " primitives' arity. For instance, the tree [sub, 4, 5, "
+                                 " primitives' arity. For instance, the tree [sub, 4, 5,"
                                  " 6] is incomplete if the arity of sub is 2, because it"
                                  " would produce an orphan node (the 6).")
         elif val.arity != self[key].arity:
             raise ValueError("Invalid node replacement with a node of a"
                              " different arity.")
 
         list.__setitem__(self, key, val)
@@ -1154,22 +1098,14 @@
         for elem in self:
             depth = stack.pop()
             max_depth = max(max_depth, depth)
             stack.extend([depth + 1] * elem.arity)
         return max_depth
 
     @property
-    def length(self):
-        return self.__len__()
-
-    @property
-    def h_bgp(self):
-        return (self.height - 1) / 2
-
-    @property
     def root(self):
         """Root of the tree, the element 0 of the list.
         """
         return self[0]
 
     def searchSubtree(self, begin):
         """Return a slice object that corresponds to the
@@ -1179,33 +1115,31 @@
         end = begin + 1
         total = self[begin].arity
         while total > 0:
             total += self[end].arity - 1
             end += 1
         return slice(begin, end)
 
+    def __hash__(self):
+        return hash(repr(self))
+
+    def __eq__(self, other):
+        return hash(self) == hash(other)
+
     def top(self):
         """accumulative operation"""
-        return self[::2]
+        return self[1::2]
 
     def bot(self):
         """operation and terminals"""
-        return self[1::2]
-
-    def cut(self, index=2):
-        slice_ = self.searchSubtree(index)
-        new_inds = self[slice_]
-        self.clear()
-        self.extend(new_inds)
+        return self[::2]
 
 
 class SymbolTree(_ExprTree):
-    """ Individual Tree, each tree is one expression.
-    The SymbolTree is only generated by method: ``genGrow`` and ``genFull``.
-    """
+    """ Individual Tree, each tree is one expression"""
 
     def __init__(self, *arg, **kwargs):
         super(SymbolTree, self).__init__(*arg, **kwargs)
         self.p_name = None
         self.y_dim = dnan
         self.pre_y = None
         self.expr = None
@@ -1226,59 +1160,50 @@
             return _ExprTree.__repr__(self)
 
     def __str__(self):
 
         return _ExprTree.__str__(self)
 
     def __hash__(self):
-        return hash(tuple(self))
-
-    def __eq__(self, other):
-        return repr(self) == repr(other)
+        return hash(self.hasher(self))
 
     def compress(self):
-        """drop unnecessary attributes"""
 
         [_ExprTree.__delattr__(self, i) for i in ("coef_expr", "coef_pre_y",
                                                   "coef_score", "pure_expr", "pure_pre_y")
          if hasattr(self, i)]
 
     def terminals(self):
         """Return terminals that occur in the expression tree."""
         return [primitive for primitive in self if primitive.arity == 0]
 
     def ter_site(self):
-        """site for feature and constants node"""
         return [i for i, primitive in enumerate(self) if primitive.arity == 0]
 
     def depart(self):
-        """take part the expression"""
         return depart(self)
 
     @property
     def capsule(self):
-        """return the short one"""
         return ShortStr(self)
 
     @classmethod
     def genGrow(cls, pset, min_, max_, per=False, ):
         """details in genGrow function"""
         return cls(genGrow(pset, min_, max_, per))
 
     @classmethod
     def genFull(cls, pset, min_, max_, per=False, ):
         """details in genGrow function"""
         return cls(genFull(pset, min_, max_, per, ))
 
     def to_expr(self, pset):
-        """transformed to sympy.Expr"""
         return compile_context(self, pset.context, pset.gro_ter_con)
 
     def ppprint(self, pset, feature_name=False):
-        """get a user friendly version"""
         return group_str(self, pset, feature_name=feature_name)
 
 
 class ShortStr:
     """short version of tree, just left name to simplify the store and transmit."""
 
     def __init__(self, st):
@@ -1294,76 +1219,66 @@
     def __hash__(self):
         return hash(self.__repr__())
 
 
 class CalculatePrecisionSet(SymbolSet):
     """
     Add score method to SymbolSet.
-    The object can get from a worked ``SymbolSet`` object.
+    The object can get from a worked symbolset object.
     """
     hasher = str
 
     def __hash__(self):
         return hash(self.hasher(self))
 
     def __init__(self, pset, scoring=None, score_pen=(1,), filter_warning=True, cv=1,
                  cal_dim=True, dim_type=None, fuzzy=False, add_coef=True, inter_add=True,
                  inner_add=False, vector_add=False, out_add=False, flat_add=False, n_jobs=1, batch_size=20,
-                 tq=True, details=False, classification=False, score_object="y", batch_para=False):
+                 tq=True):
         """
 
         Parameters
         ----------
+        fuzzy : bool
+            fuzzy or not
+        dim_type : object
+            if None, use the y_dim
         pset:SymbolSet
-            SymbolSet.
-        scoring: Callbale, default is sklearn.metrics.r2_score.
-            See Also sklearn.metrics.
+            SymbolSet
+        scoring: Callbale, default is sklearn.metrics.r2_score
+            See Also sklearn.metrics
+        score_pen: tuple, default is sklearn.metrics.r2_score
+            See Also sklearn.metrics
         filter_warning:bool
-            bool.
-        score_pen: tuple of float
-            1 : best is positive, worse -np.inf. \n
-            -1 : best is negative, worse np.inf. \n
-            0 : best is positive , worst is 0. \n
+            bool
+        score_pen: tuple of 1 or -1
+            1 : best is positive, worse -np.inf \n
+            -1 : best is negative, worse np.inf \n
+            0 : best is positive , worse 0 \n
         cal_dim: bool
-            calculate dim or not, if not return dless.
+            calculate dim or not, if not return dimless
         add_coef: bool
-            bool.
+            bool
         inter_add: bool
-            bool.
+            bool
         inner_add: bool
-            bool.
-        fuzzy : bool
-            fuzzy or not.
-        dim_type : object
-            if None, use the y_dim.
+            bool
         n_jobs:int
-            running core.
+            running core
         batch_size:int
-            batch size, advice batch_size*n_jobs = inds.
+            batch size, advice batch_size*n_jobs = inds/n
         tq:bool
-            bool.
-        cv:sklearn.model_selection._split._BaseKFold, int
-            the shuffler must be False!
-
-            use cv spilt for score, return the mean_test_score.
-
-            use cv spilt for predict, return the cv_predict_y.(not be used)
-
+            bool
+        cv:sklearn.model_selection._split._BaseKFold,int
+            the shuffler must be False
+            use cv spilt for score,return the mean_test_score.
+            use cv spilt for predict,return the cv_predict_y.(not be used)
             Notes:
-                if cv and refit, all the data is refit to determination the coefficients.\n
-                Thus the expression is not compact with the this scores, when re-calculated by this expression
-
-        details:bool
-            return the expr and predict y cor not.
-
-        classification: bool
-            classification or not.
-
-        score_object:
-            score by y or delta y (for implicit function).
+            if cv and refit, all the data is refit to determination the coefficients.
+            Thus the expression is not compact with the this scores, when re-calculated by this expression
 
         """
         super(CalculatePrecisionSet, self).__init__()
         self.__dict__.update(copy.deepcopy(pset.__dict__))
         self.name = "CPSet"
         self.cal_dim = cal_dim
         self.score_pen = score_pen
@@ -1373,295 +1288,148 @@
         self.inter_add = inter_add
         self.inner_add = inner_add
         self.vector_add = vector_add
         self.out_add = out_add
         self.flat_add = flat_add
         self.n_jobs = n_jobs
         self.batch_size = batch_size
-        self.batch_para = batch_para
         self.tq = tq
         self.fuzzy = fuzzy
         self.dim_type = dim_type if dim_type is not None else self.y_dim
         self.refit = True
         self.cv = cv
-        self.details = details
-        self.classification = classification
-        self.score_object = score_object
 
         if not scoring:
             scoring = [r2_score, ]
         if not isinstance(scoring, (tuple, list)):
             scoring = [scoring, ]
 
         scoring = [score_collection[i] if isinstance(i, str) else i for i in scoring]
 
         self.scoring = scoring
 
-    def update(self, pset):
-        """updata self by input pset."""
-        self.__dict__.update(copy.deepcopy(pset.__dict__))
-
-    def update_with_X_y(self, X, y):
-        """replace x, y data."""
-        if self.expr_init_map:
-            tree_x = []
-            n = len(self.expr_init_map)
-            self.replace(X, y=y, tree_X=np.zeros((2, n)))
-
-            for k, v in self.expr_init_map.items():
-                v = self.calculate_expr(v)
-                pre_y = v["pre_y"]
-                tree_x.append(pre_y)
-            lens = len(tree_x)
-            tree_x = np.array(tree_x).T
-            tree_x = tree_x.reshape(-1, lens)
-            self.replace(X, y=y, tree_X=tree_x)
-
-        else:
-            self.replace(X, y=y)
-
-    def compile_context(self, ind):
-        """transform SymbolTree to sympy.Expr."""
-        if isinstance(ind, SymbolTree):
-            expr = compile_context(ind.capsule, self.context, self.gro_ter_con)
-        else:
-            expr = compile_context(ind, self.context, self.gro_ter_con)
-        return expr
-
     def calculate_cv_score(self, ind):
-        """just used for calculating single one or check."""
         if isinstance(ind, SymbolTree):
             expr = compile_context(ind.capsule, self.context, self.gro_ter_con)
         elif isinstance(ind, sympy.Expr):
             expr = ind
         else:
             raise TypeError("must be SymbolTree or sympy.Expr")
         score, expr01, pre_y = calculate_cv_score(expr, self.data_x, self.y,
                                                   self.terminals_and_constants_repr,
                                                   cv=self.cv, refit=self.refit,
                                                   add_coef=self.add_coef, inter_add=self.inter_add,
                                                   inner_add=self.inner_add, vector_add=self.vector_add,
                                                   out_add=self.out_add, flat_add=self.flat_add,
                                                   scoring=self.scoring, score_pen=self.score_pen,
                                                   filter_warning=self.filter_warning,
-                                                  np_maps=self.np_map, classification=self.classification,
-                                                  score_object=self.score_object, details=True)
+                                                  np_maps=self.np_map)
         return score, expr01, pre_y
 
     def calculate_score(self, ind):
-        """
-        just used for calculating single one or check with cv=1.
-
-        Parameters
-        ----------
-        ind:SymbolTree
-        """
         self.cv = 1
         return self.calculate_cv_score(ind)
 
     def calculate_detail(self, ind):
         """
-        just used for calculated final best one result for showing.
-
-        calculate the best expression.
 
         Parameters
         ----------
         ind: SymbolTree
-            best expression.
+
+        Returns
+        -------
+        SymbolTree
         """
         ind = self.calculate_simple(ind)
 
         score, expr01, pre_y = calculate_cv_score(ind.expr, self.data_x, self.y,
                                                   self.terminals_and_constants_repr,
                                                   cv=self.cv, refit=self.refit,
                                                   add_coef=self.add_coef, inter_add=self.inter_add,
                                                   inner_add=self.inner_add, vector_add=self.vector_add,
                                                   out_add=self.out_add, flat_add=self.flat_add,
                                                   scoring=self.scoring, score_pen=self.score_pen,
                                                   filter_warning=self.filter_warning,
-                                                  np_maps=self.np_map, classification=self.classification,
-                                                  score_object=self.score_object, details=True)
+                                                  np_maps=self.np_map)
 
         # this group should be get onetime and get all.
         ind.coef_expr = expr01
         ind.coef_pre_y = pre_y
         ind.coef_score = score
 
         ind.pure_expr = ind.expr
         ind.pure_pre_y = ind.pre_y
 
         return ind
 
     def calculate_simple(self, ind):
         """
-        just used for re_Tree, and showing.
-
-        calculate the best expression.
 
         Parameters
         ----------
         ind:SymbolTree
+
+        Returns
+        -------
+        SymbolTree
         """
         if isinstance(ind, SymbolTree):
             expr = compile_context(ind.capsule, self.context, self.gro_ter_con)
         elif isinstance(ind, sympy.Expr):
             expr = ind
         else:
             raise TypeError("must be SymbolTree or sympy.Expr")
-
-        if self.cal_dim:
-            dim, dim_score = calcualte_dim_score(expr, self.terminals_and_constants_repr,
-                                                 self.dim_ter_con_list, self.dim_type,
-                                                 self.fuzzy, self.dim_map)
-        else:
-            dim, dim_score = dless, 1
-
         score, expr01, pre_y = calculate_cv_score(expr, self.data_x, self.y,
                                                   self.terminals_and_constants_repr,
                                                   cv=self.cv, refit=self.refit,
                                                   add_coef=False, inter_add=False,
                                                   inner_add=False, vector_add=False, out_add=False, flat_add=False,
                                                   scoring=self.scoring, score_pen=self.score_pen,
                                                   filter_warning=self.filter_warning,
-                                                  np_maps=self.np_map, classification=self.classification,
-                                                  score_object=self.score_object, details=True)
-
-        ind.y_dim = dim
-        ind.expr = expr01
-        ind.pre_y = pre_y
-        ind.dim_score = dim_score
-
-        return ind
-
-    def calculate_expr(self, expr):
-        """
-        just used for calculated final result for showing.
-
-        Parameters
-        ----------
-        ind:sympy.Expr
-
-        """
-
-        if isinstance(expr, sympy.Expr):
-            pass
-        else:
-            raise TypeError("must be sympy.Expr")
-
+                                                  np_maps=self.np_map)
         if self.cal_dim:
             dim, dim_score = calcualte_dim_score(expr, self.terminals_and_constants_repr,
                                                  self.dim_ter_con_list, self.dim_type,
                                                  self.fuzzy, self.dim_map)
         else:
             dim, dim_score = dless, 1
 
-        score, expr01, pre_y = calculate_cv_score(expr, self.data_x, self.y,
-                                                  self.terminals_and_constants_repr,
-                                                  cv=self.cv, refit=self.refit,
-                                                  add_coef=False, inter_add=False,
-                                                  inner_add=False, vector_add=False, out_add=False, flat_add=False,
-                                                  scoring=self.scoring, score_pen=self.score_pen,
-                                                  filter_warning=self.filter_warning,
-                                                  np_maps=self.np_map, classification=self.classification,
-                                                  score_object=self.score_object, details=True)
-
-        result = {"score": score, "expr": expr01, "pre_y": pre_y, "dim": dim, "dim_score": dim_score}
-
-        return result
-
-    def parallelize_calculate_expr(self, exprs):
-        """just used for final results, calculate exprs."""
-
-        calls = functools.partial(calculate_cv_score, x=self.data_x, y=self.y,
-                                  terminals_and_constants_repr=self.terminals_and_constants_repr,
-                                  cv=self.cv, refit=self.refit,
-                                  add_coef=False, inter_add=False,
-                                  inner_add=False, vector_add=False, out_add=False, flat_add=False,
-                                  scoring=self.scoring, score_pen=self.score_pen,
-                                  filter_warning=self.filter_warning,
-                                  np_maps=self.np_map, classification=self.classification,
-                                  score_object=self.score_object, details=self.details)
-
-        score_dim_list = parallelize(func=calls, iterable=exprs, n_jobs=self.n_jobs,
-                                     respective=False,
-                                     tq=self.tq, batch_size=self.batch_size)
-        # (sc_all, expr01, pre_y)
-        return score_dim_list
-
-    def try_add_coef_times(self, expr, grid_x=None):
-        """just used for best result, try add coefficient to expr."""
-
-        pre_y_all_expr01 = try_add_coef_times(expr, self.data_x, self.y, self.terminals_and_constants_repr, grid_x,
-                                              filter_warning=self.filter_warning, inter_add=self.inter_add,
-                                              inner_add=self.inner_add, vector_add=self.vector_add,
-                                              out_add=self.out_add,
-                                              flat_add=self.flat_add,
-                                              np_maps=self.np_map, classification=self.classification,
-                                              random_state=0,
-                                              return_expr=False
-                                              )
-
-        return pre_y_all_expr01
-
-    def parallelize_try_add_coef_times(self, exprs, grid_x=None, resample_number=500):
-        """to be continued"""
-        if isinstance(grid_x, np.ndarray):
-            grid_x = list(grid_x.T)
-        calls = functools.partial(try_add_coef_times, x=self.data_x, y=self.y,
-                                  terminals=self.terminals_and_constants_repr,
-                                  grid_x=grid_x,
-                                  filter_warning=self.filter_warning, inter_add=self.inter_add,
-                                  inner_add=self.inner_add, vector_add=self.vector_add,
-                                  out_add=self.out_add,
-                                  flat_add=self.flat_add,
-                                  np_maps=self.np_map, classification=self.classification,
-                                  random_state=0,
-                                  return_expr=False,
-                                  resample_number=resample_number,
-                                  )
-
-        pre_y_all_list = parallelize(func=calls, iterable=exprs, n_jobs=1, respective=False,
-                                     tq=self.tq)
+        ind.y_dim = dim
+        ind.expr = expr01
+        ind.pre_y = pre_y
+        ind.dim_score = dim_score
 
-        return pre_y_all_list
+        return ind
 
     def parallelize_score(self, inds):
         """
-        The main score in each generation of GP!
 
         Parameters
         ----------
         inds:list of SymbolTree
-            list of expressions
 
+        Returns
+        -------
+        list of (score,dim,dim_score)
         """
 
         indss = [i.capsule for i in inds]
 
-        calculate_collect_use = calculate_collect_
-
-        calls = functools.partial(calculate_collect_use, context=self.context, x=self.data_x, y=self.y,
+        calls = functools.partial(calculate_collect, context=self.context, x=self.data_x, y=self.y,
                                   terminals_and_constants_repr=self.terminals_and_constants_repr,
                                   gro_ter_con=self.gro_ter_con, cv=self.cv, refit=self.refit,
                                   dim_ter_con_list=self.dim_ter_con_list, dim_type=self.dim_type,
                                   fuzzy=self.fuzzy,
                                   scoring=self.scoring, score_pen=self.score_pen,
                                   vector_add=self.vector_add,
                                   add_coef=self.add_coef, inter_add=self.inter_add,
                                   out_add=self.out_add, flat_add=self.flat_add,
-                                  inner_add=self.inner_add, np_maps=self.np_map, classification=self.classification,
+                                  inner_add=self.inner_add, np_maps=self.np_map,
                                   filter_warning=self.filter_warning,
-                                  dim_maps=self.dim_map, cal_dim=self.cal_dim, score_object=self.score_object,
-                                  details=self.details
-                                  )
-
-        if isinstance(self.batch_size, int) and self.batch_para:
-            score_dim_list = batch_parallelize(func=calls, iterable=indss, n_jobs=self.n_jobs,
-                                               respective=False,
-                                               tq=self.tq, batch_size=self.batch_size)
-        else:
-            score_dim_list = parallelize(func=calls, iterable=indss, n_jobs=self.n_jobs,
-                                         respective=False,
-                                         tq=self.tq, batch_size=self.batch_size)
+                                  dim_maps=self.dim_map, cal_dim=self.cal_dim)
+
+        score_dim_list = parallelize(func=calls, iterable=indss, n_jobs=self.n_jobs,
+                                     respective=False,
+                                     tq=self.tq, batch_size=self.batch_size)
 
         return score_dim_list
```

### Comparing `BindingGP-0.0.36/bgp/calculation/coefficient.py` & `BindingGP-0.0.9/BGP/calculation/coefficient.py`

 * *Files 11% similar despite different names*

```diff
@@ -4,22 +4,22 @@
 import copy
 import warnings
 from collections import Counter
 
 import numpy as np
 import sympy
 from scipy import optimize
-from sklearn.utils import resample
+from sympy import Function
+from sympy.core.function import UndefinedFunction
 from sympy.core.numbers import NegativeOne
-from sympy.core.function import UndefinedFunction, Function
 
 
 class Coef(UndefinedFunction):
     """
-    generate metaclass, the type of identity is .arr,.tp ,rather isinstance.
+    generate metaclass, the type of identity is .arr,.tp ,rather isinstance
     """
 
     def __new__(mcs, name, arr):
 
         def lfun(x):
             if isinstance(x, np.ndarray):
                 return arr * x
@@ -339,19 +339,19 @@
         cof_list.append(A)
 
     return expr01
 
 
 def add_coefficient(expr01, inter_add=True, inner_add=False, vector_add=False, out_add=False, flat_add=False):
     """
-    Try add the placeholder coefficient to sympy expression.
-    1. Add Wi,A,B normal coefficients to expression.
-    2. Add V, Vi vector coefficients to expression, for this type of coefficient ,
-    there should be with expr01.conu for Function("MAdd"), Function("MSub").
-    more details can be found in ..translate.simple
+    try add placeholder coefficient to sympy expression.
+    add to Wi,A,B normal coefficient to expression.
+    add V, Vi vecotr coefficient to expression, for this type of coefficent ,
+    there should be expr01.conu for Function("MAdd"), Function("MSub").
+    more detial can be found in ..translate.simple
 
     Parameters
     ----------
     expr01: Expr
         sympy expressions
     inter_add: bool
         bool
@@ -420,74 +420,68 @@
         return len(self.name)
 
     @property
     def ind(self):
         lsa = list(range(len(self.cof_list)))
         n = len(lsa)
         for k in self.cof_dict_values:
-            lsi = np.arange(k) + n
+            lsi = list(range(k))
+            lsi = [lsii + n for lsii in lsi]
             lsa.append(lsi)
             n = lsi[-1] + 1
 
         return lsa
 
     def group(self, p, decimals=False):
         """change the p to grpup"""
         p = np.array(p)
-
-        ls = [p[i] if isinstance(i, int) else p[i].reshape((-1, 1)) for i in self.ind]
+        ls = []
+        for i in self.ind:
+            if isinstance(i, int):
+                ls.append(p[i])
+            else:
+                ps = p[i].reshape((-1, 1))
+                ls.append(ps)
 
         if decimals:
             return self.dec(ls)
         else:
             return ls
-        # return ls
 
     def dec(self, ls):
         cof_ = []
         for a_listi, cofi in zip(self.name, ls):
 
             if not isinstance(cofi, np.ndarray):
                 cof_.append(float("%.3e" % cofi))
             else:
                 cof_.append(np.array([float("%.3e" % i) for i in cofi]).reshape((-1, 1)))
         return cof_
 
 
-def cla(pre_y, cl=True):
-    pre_y = 1.0 / (1.0 + np.exp(-pre_y))
-    if cl:
-        pre_y[np.where(pre_y >= 0.5)] = 1
-        pre_y[np.where(pre_y < 0.5)] = 0
-    return pre_y
-
-
-def try_add_coef(expr01, x, y, terminals, grid_x=None,
+def try_add_coef(expr01, x, y, terminals,
                  filter_warning=True, inter_add=True, inner_add=False, vector_add=False, out_add=False, flat_add=False,
-                 np_maps=None, classification=False):
+                 np_maps=None):
     """
-    Try calculate predict y by sympy expression with coefficients.
-    if except error return expr itself.
-
+    try calculate predict y by sympy expression with coef.
+    if except error return expr self.
     Parameters
     ----------
     flat_add:bool
-        add flat coefficient or not
+        add flat coefficent or not
     out_add:
-        add outcoefficientt or not
+        add out coefficent or not
     vector_add: bool
-        add vectorcoefficientt or not
+        add vector coefficent or not
     expr01: sympy.Expr
         sympy expressions
     x: list of np.ndarray
         list of xi
     y: np.ndarray
         y value
-    grid_x:
-        new x to predict
     terminals: list of sympy.Symbol
         features and constants
     filter_warning: bool
         bool
     inter_add: bool
         bool
     inner_add: bool
@@ -501,15 +495,15 @@
         np.array or None
     expr01: Expr
         New expr.
     """
     if filter_warning:
         warnings.filterwarnings("ignore")
 
-    expr00 = copy.copy(expr01)
+    expr00 = copy.deepcopy(expr01)
 
     expr01, a_list, a_dict = add_coefficient(expr01, inter_add=inter_add, inner_add=inner_add, vector_add=vector_add,
                                              out_add=out_add, flat_add=flat_add)
 
     cc = CheckCoef(a_list, a_dict)
 
     ter = []
@@ -518,52 +512,32 @@
 
     try:
 
         func0 = sympy.utilities.lambdify(ter, expr01, modules=[np_maps, "numpy", "math"])
 
         def func(x_, p):
             """"""
-            # num_list = []
-            # num_list.extend(x_)
-            if vector_add:
-                p = cc.group(p)
-            # num_list.extend(p)
+            num_list = []
+            num_list.extend(x_)
+            p = cc.group(p)
+            num_list.extend(p)
 
-            return func0(*x_, *p)
+            return func0(*num_list)
 
         def res(p, x_, y_):
             """"""
-            return y_ - func(x_, p)
-
-        def res2(p, x_, y_):
-            """"""
-            pre_y = func(x_, p)
-            ress = y_ - cla(pre_y, cl=False)
-
+            ress = y_ - func(x_, p)
             return ress
 
-        if not classification:
-            result = optimize.least_squares(res, x0=[1.0] * cc.num, args=(x, y), xtol=1e-4, ftol=1e-5, gtol=1e-5,
-                                            # long
-                                            jac='3-point', loss='linear')
-        else:
-            result = optimize.least_squares(res2, x0=[1.0] * cc.num, args=(x, y), xtol=1e-4, ftol=1e-5, gtol=1e-5,
-                                            # long
-                                            jac='3-point', loss='linear')
+        result = optimize.least_squares(res, x0=[1.0] * cc.num, args=(x, y), xtol=1e-4, ftol=1e-5, gtol=1e-5,  # long
+                                        jac='3-point', loss='linear')
         cof = result.x
 
         cof = cc.group(cof)
-
-        if grid_x is None:
-            grid_x = x
-
-        pre_y = func0(*grid_x, *cof)
-        if classification:
-            pre_y = cla(pre_y, cl=True)
-
+        pre_y = func0(*x + cof)
         cof = cc.dec(cof)
 
         for ai, choi in zip(cc.name, cof):
             if ai in cc.cof_dict_keys:
 
                 fun = Coef(ai.name, choi)
                 # replace the Vi to Vi()
@@ -572,123 +546,13 @@
                     raise KeyError("0*wi is 0,and make the placeholder fade out")
                 olds = [old for old in olds0 if old is not ai]
                 olds = sympy.Mul(*olds)
                 expr01 = expr01.xreplace({sympy.Mul(ai, olds): fun(olds)})
             else:
                 expr01 = expr01.xreplace({ai: choi})
 
-    except (ValueError, KeyError, NameError, TypeError, ZeroDivisionError, IndexError):
+    except (ValueError, KeyError, NameError, TypeError, ZeroDivisionError):
 
         expr01 = expr00
         pre_y = None
 
     return pre_y, expr01
-
-
-def try_add_coef_times(expr01, x, y, terminals, grid_x=None,
-                       filter_warning=True, inter_add=True, inner_add=False, vector_add=False, out_add=False,
-                       flat_add=False,
-                       np_maps=None, classification=False, random_state=0, return_expr=False, resample_number=500):
-    if filter_warning:
-        warnings.filterwarnings("ignore")
-
-    if grid_x is None:
-        grid_x = x
-
-    expr01, a_list, a_dict = add_coefficient(expr01, inter_add=inter_add, inner_add=inner_add, vector_add=vector_add,
-                                             out_add=out_add, flat_add=flat_add)
-
-    cc = CheckCoef(a_list, a_dict)
-
-    ter = []
-    ter.extend(terminals)
-    ter.extend(cc.name)
-
-    func0 = sympy.utilities.lambdify(ter, expr01, modules=[np_maps, "numpy", "math"])
-
-    def func(x_, p):
-        """"""
-        num_list = []
-        num_list.extend(x_)
-
-        p = cc.group(p)
-        num_list.extend(p)
-
-        return func0(*num_list)
-
-    def res(p, x_, y_):
-        """"""
-        ress = y_ - func(x_, p)
-        return ress
-
-    def res2(p, x_, y_):
-        """"""
-        pre_y = func(x_, p)
-        pre_y = cla(pre_y, cl=False)
-        ress = y_ - pre_y
-
-        return ress
-
-    pre_y_all = []
-    expr_all = []
-    for times in range(resample_number):
-        *x, y = resample(*x, y, replace=True, random_state=times)
-
-        if not classification:
-            result = optimize.least_squares(res, x0=[1.0] * cc.num, args=(x, y), xtol=1e-4, ftol=1e-4, gtol=1e-4,
-                                            # max_nfev=200,
-                                            jac='3-point', loss='linear')
-        else:
-            result = optimize.least_squares(res2, x0=[1.0] * cc.num, args=(x, y), xtol=1e-4, ftol=1e-4, gtol=1e-4,
-                                            # max_nfev=200,
-                                            jac='3-point', loss='linear')
-        cof = result.x
-        cof = cc.group(cof)
-
-        try:
-
-            pre_y = func0(*grid_x + cof)
-
-            if classification:
-                pre_y = cla(pre_y, cl=True)
-
-                expr00 = expr01
-            if return_expr:
-
-                expr00 = copy.deepcopy(expr01)
-
-                cof = cc.dec(cof)
-                for ai, choi in zip(cc.name, cof):
-                    if ai in cc.cof_dict_keys:
-
-                        fun = Coef(ai.name, choi)
-                        # replace the Vi to Vi()
-                        olds0 = find_args(expr00, ai)
-                        if olds0 is None:
-                            raise KeyError("0*wi is 0,and make the placeholder fade out")
-                        olds = [old for old in olds0 if old is not ai]
-                        olds = sympy.Mul(*olds)
-                        expr00 = expr00.xreplace({sympy.Mul(ai, olds): fun(olds)})
-                    else:
-                        expr00 = expr00.xreplace({ai: choi})
-            else:
-                pass
-
-        except (ValueError, KeyError, NameError, TypeError, ZeroDivisionError):
-
-            pre_y = None
-
-        if isinstance(pre_y, np.ndarray):
-
-            if np.all(np.isfinite(pre_y)):
-                pre_y_all.append(pre_y)
-
-                if return_expr:
-                    expr_all.append(expr00)
-
-    pre_y_all = np.array(pre_y_all)
-
-    if return_expr:
-        return pre_y_all, expr_all
-    else:
-
-        return pre_y_all
```

### Comparing `BindingGP-0.0.36/bgp/calculation/scores.py` & `BindingGP-0.0.9/BGP/calculation/scores.py`

 * *Files 20% similar despite different names*

```diff
@@ -8,101 +8,87 @@
 # @License: GNU Lesser General Public License v3.0
 """
 Notes:
     score method.
 """
 
 import copy
-import itertools
 import warnings
 
 import numpy as np
-# import sympy
+import sympy
+from BGP.calculation.coefficient import try_add_coef
+from BGP.calculation.translate import compile_context
+from BGP.functions.dimfunc import dim_map, dless, dnan, Dim
 from sklearn import metrics
 from sklearn.exceptions import DataConversionWarning
 from sklearn.metrics import r2_score
 from sklearn.model_selection import KFold
 from sklearn.utils import check_array
-from sympy import utilities, Expr, diff
-from sympy.core import Function
-
-from bgp.calculation.coefficient import try_add_coef, cla
-from bgp.calculation.translate import compile_context
-from bgp.functions.dimfunc import dim_map, dless, dnan, Dim
-from bgp.functions.gsymfunc import NewArray
 
 
 def calculate_y(expr01, x, y, terminals, add_coef=True, x_test=None, y_test=None,
                 filter_warning=True, inter_add=True, inner_add=False, vector_add=False, out_add=False, flat_add=False,
-                np_maps=None, classification=False):
+                np_maps=None):
     if filter_warning:
         warnings.filterwarnings("ignore")
     try:
         if add_coef:
             pre_y, expr01 = try_add_coef(expr01, x, y, terminals,
                                          filter_warning=filter_warning,
                                          inter_add=inter_add, inner_add=inner_add,
-                                         vector_add=vector_add, out_add=out_add, flat_add=flat_add,
-                                         np_maps=np_maps, classification=classification)
+                                         vector_add=vector_add, out_add=out_add, flat_add=flat_add, np_maps=np_maps)
         else:
-            func0 = utilities.lambdify(terminals, expr01, modules=[np_maps, "numpy"])
+            func0 = sympy.utilities.lambdify(terminals, expr01, modules=[np_maps, "numpy"])
             pre_y = func0(*x)
-            if classification:
-                pre_y = cla(pre_y)
 
         if x_test is not None and y_test is not None:
-            func0 = utilities.lambdify(terminals, expr01, modules=[np_maps, "numpy"])
+            func0 = sympy.utilities.lambdify(terminals, expr01, modules=[np_maps, "numpy"])
             pre_y = func0(*x_test)
-            if classification:
-                pre_y = cla(pre_y)
-
             pre_y = pre_y.ravel()
             assert y_test.shape == pre_y.shape
             pre_y = check_array(pre_y, ensure_2d=False)
         else:
             pre_y = pre_y.ravel()
             assert y.shape == pre_y.shape
             pre_y = check_array(pre_y, ensure_2d=False)
 
-    except (DataConversionWarning, TypeError, AssertionError, ValueError, AttributeError, KeyError, ZeroDivisionError):
+    except (DataConversionWarning, AssertionError, ValueError, AttributeError, KeyError, ZeroDivisionError):
         pre_y = None
 
     return pre_y, expr01
 
 
-def calculate_y_unpack(expr01, x, terminals, classification=False):
+def calculate_y_unpack(expr01, x, terminals):
     try:
-        func0 = utilities.lambdify(terminals, expr01)
+        func0 = sympy.utilities.lambdify(terminals, expr01)
         pre_y = func0(*x)
-        if classification:
-            pre_y = cla(pre_y)
         pre_y = pre_y.ravel()
         pre_y = check_array(pre_y, ensure_2d=False)
 
     except (DataConversionWarning, AssertionError, ValueError, AttributeError, KeyError, ZeroDivisionError):
         pre_y = None
     return pre_y
 
 
 def uniform_score(score_pen=1):
-    """return the worst score"""
+    """return the worse score"""
     if score_pen >= 0:
         return -np.inf
     elif score_pen <= 0:
         return np.inf
     elif score_pen == 0:
         return 0
     else:
         return score_pen
 
 
 def calculate_score(expr01, x, y, terminals, scoring=None, score_pen=(1,),
                     add_coef=True, filter_warning=True, inter_add=True,
-                    inner_add=False, vector_add=False, out_add=False, flat_add=False, np_maps=None,
-                    classification=False, score_object="y", details=False):
+                    inner_add=False, vector_add=False, out_add=False, flat_add=False, np_maps=None):
     """
 
     Parameters
     ----------
     vector_add
     expr01: Expr
         sympy expression.
@@ -115,15 +101,15 @@
     scoring: list of Callbale, default is [sklearn.metrics.r2_score,]
         See Also sklearn.metrics
     score_pen: tuple of  1 or -1
         1 : best is positive, worse -np.inf
         -1 : best is negative, worse np.inf
         0 : best is positive , worse 0
     add_coef: bool
-        bool.
+        bool
     filter_warning: bool
         bool
     inter_add: bool
         bool
     inner_add: bool
         bool
     np_maps: Callable
@@ -132,15 +118,15 @@
     Returns
     -------
     score:float
         score
     expr01: Expr
         New expr.
     pre_y: np.ndarray or float
-        np.ndarray or None
+        np.array or None
     """
     if filter_warning:
         warnings.filterwarnings("ignore")
     if not scoring:
         scoring = [r2_score, ]
     if not isinstance(scoring, (tuple, list)):
         scoring = [scoring, ]
@@ -148,162 +134,43 @@
         score_pen = [score_pen, ]
 
     assert len(scoring) == len(score_pen), "the scoring and score_pen with same size"
 
     pre_y, expr01 = calculate_y(expr01, x, y, terminals, add_coef=add_coef,
                                 filter_warning=filter_warning, inter_add=inter_add, inner_add=inner_add,
                                 vector_add=vector_add, out_add=out_add, flat_add=flat_add,
-                                np_maps=np_maps, classification=classification)
-
-    if score_object == "y" or classification is True:
-        try:
-            sc_all = []
-            for si, sp in zip(scoring, score_pen):
-                sc = si(y, pre_y)
-                if np.isnan(sc):
-                    sc = uniform_score(score_pen=sp)
-                sc_all.append(sc)
-
-        except (ValueError, RuntimeWarning, TypeError):
-
-            sc_all = [uniform_score(score_pen=i) for i in score_pen]
-
-    else:
-
-        ######dy under test########
-        pre_dy, dy = calculate_derivative_y(expr01, x, terminals, np_maps=np_maps)
-        if pre_dy is None:
-            sc_all = [uniform_score(score_pen=i) for i in score_pen]
-        else:
-            try:
-                sc_all = []
-                for si, sp in zip(scoring, score_pen):
-                    sc = []
-                    for i, j in zip(dy, pre_dy):
-                        index = np.isfinite(i) * np.isfinite(j)
-                        sci = si(i[index], j[index])
-                        sc.append(sci)
-                    sc = [uniform_score(score_pen=sp) if np.isnan(i) or i is None else i for i in sc]
-                    sc = sum(sc) / len(sc)
-                    sc_all.append(sc)
-
-            except (ValueError, RuntimeWarning, TypeError):
-
-                sc_all = [uniform_score(score_pen=i) for i in score_pen]
-    if details:
-        return sc_all, expr01, pre_y
-    else:
-        return sc_all, str(expr01), 0
-
-
-def calculate_derivative_y(expr01, x, terminals, np_maps=None):
-    """
-    Something error for reference:
-
-    M. Schmidt, H. Lipson, Distilling free-form natural laws from experimental data, Science, 324 (2009),
-    81–85.
-
-    Parameters
-    ----------
-    expr01: Expr
-        sympy expression.
-    x: list of np.ndarray
-        list of xi
-    terminals: list of sympy.Symbol
-        features and constants
-    np_maps: Callable
-        user np.ndarray function
-
-    Returns
-    -------
-    pre_dy_all:np.ndarray or float
-        pre-dy
-    dy_all: np.ndarray or float
-        dy
-    """
-    warnings.filterwarnings("ignore")
-    if not isinstance(expr01, (Expr, NewArray)):
-        return None, None
-    if len(expr01.free_symbols) < 2:
-        return None, None
-
-    free_symbols = list(expr01.free_symbols)[:4] if len(expr01.free_symbols) > 4 else list(expr01.free_symbols)
-
-    free_symbols.sort(key=lambda x: x.name)
-    par = list(itertools.combinations(free_symbols, 2))
-
-    # free_symbols = [] # no dependence
-    free_symbols = par  # all denpendence
-    # free_symbols = [par[0]]
-    # free_symbols = par[-1:]
-    # free_symbols = par[1:]
+                                np_maps=np_maps)
 
     try:
-        pre_dy_all = []
-        dy_all = []
-        for pari in par:
-            pari = list(pari)
-            pari.sort(key=lambda x: x.name)
-            i, j = pari
-            subbb = {}
-            subbb1 = {k: Function("{}f".format(k.name))(v) for k, v in free_symbols if k is not i and v is i}
-            subbb2 = {k: Function("{}f".format(k.name))(v) for v, k in free_symbols if k is not i and v is i}
-            subbb.update(subbb1)
-            subbb.update(subbb2)
-            subb_re = dict(zip(subbb.values(), subbb.keys()))
-
-            fdv1 = diff(expr01.subs(subbb), i, evaluate=True)
-            fdv1 = fdv1.subs(subb_re)
-            subbb = {}
-            subbb3 = {k: Function("{}f".format(k.name))(v) for k, v in free_symbols if k is not j and v is j}
-            subbb4 = {k: Function("{}f".format(k.name))(v) for v, k in free_symbols if k is not j and v is j}
-            subbb.update(subbb3)
-            subbb.update(subbb4)
-            subb_re = dict(zip(subbb.values(), subbb.keys()))
-            fdv2 = diff(expr01.subs(subbb), j, evaluate=True).subs(subb_re)
-            fdv = fdv2 / fdv1
-
-            func0 = utilities.lambdify(terminals, fdv, modules=[np_maps, "numpy"])
-            pre_dy = func0(*x)
-
-            ff = diff(i, j, evaluate=False)
-            func0 = utilities.lambdify(terminals, ff, modules=[np_maps, "numpy"])
-            dy = func0(*x)
-
-            pre_dy_all.append(pre_dy)
-            dy_all.append(dy)
+        sc_all = []
+        for si, sp in zip(scoring, score_pen):
+            sc = si(y, pre_y)
+            if np.isnan(sc):
+                sc = uniform_score(score_pen=sp)
+            sc_all.append(sc)
 
-        pre_dy_all = np.array(pre_dy_all)
-        dy_all = np.array(dy_all)
+    except (ValueError, RuntimeWarning):
 
-    except (ValueError, RuntimeWarning, TypeError):
-        pre_dy_all, dy_all = None, None
+        sc_all = [uniform_score(score_pen=i) for i in score_pen]
 
-    return pre_dy_all, dy_all
+    return sc_all, expr01, pre_y
 
 
 def calculate_cv_score(expr01, x, y, terminals, scoring=None, score_pen=(1,), cv=5, refit=True,
                        add_coef=True, filter_warning=True, inter_add=True,
-                       inner_add=False, vector_add=False, out_add=False, flat_add=False, np_maps=None,
-                       classification=False, score_object="y", details=False):
+                       inner_add=False, vector_add=False, out_add=False, flat_add=False, np_maps=None):
     """
-    Use cv spilt for score, return the mean_test_score.
-    Use cv spilt for predict, return the cv_predict_y.(have not be used)
-
+    use cv spilt for score,return the mean_test_score.
+    use cv spilt for predict,return the cv_predict_y.(not be used)
     Notes:
-        if cv and refit, all the data is refit to determine the coefficients.
-        Thus, the expression is not compact with the this scores, when re-calculated by this expression.
-
+        if cv and refit, all the data is refit to determination the coefficients.
+        Thus the expression is not compact with the this scores, when re-calculated by this expression
     Parameters
     ----------
 
-    score_object:
-        score by y or delta y
-    classification:
-        classification or not
     refit: True:
         use forced, refit the coefficient use all data.
     cv:sklearn.model_selection._split._BaseKFold,int
         the shuffler must be False
     vector_add
     expr01: Expr
         sympy expression.
@@ -346,107 +213,90 @@
     if filter_warning:
         warnings.filterwarnings("ignore")
 
     if cv == 1:
         sc_all, expr01, pre_y = calculate_score(expr01, x, y, terminals, scoring=scoring, score_pen=score_pen,
                                                 add_coef=add_coef, filter_warning=filter_warning, inter_add=inter_add,
                                                 inner_add=inner_add, vector_add=vector_add, out_add=out_add,
-                                                flat_add=flat_add, np_maps=np_maps, classification=classification,
-                                                score_object=score_object, details=details)
+                                                flat_add=flat_add, np_maps=np_maps)
         return sc_all, expr01, pre_y
 
-    else:
-        if score_object != "y":
-            raise TypeError('cv>1 and score_object !="y" are not compatible')
+    if isinstance(cv, int):
+        cv = KFold(cv, shuffle=False)
 
-        if isinstance(cv, int):
-            cv = KFold(cv, shuffle=False)
+    cv_sc_all = []
+    cv_expr01 = []
+    cv_pre_y = []
+    xx = [xi for xi in x if isinstance(xi, np.ndarray)]
+    c = [xi for xi in x if not isinstance(xi, np.ndarray)]
+    xx = [xi.reshape((-1, 1)) if xi.ndim == 1 else xi.T for xi in xx]
+
+    for train_index, test_index in cv.split(xx[0], y):
+
+        X_train = [xi[train_index] for xi in xx]
+        X_test = [xi[test_index] for xi in xx]
+        y_train, y_test = y[train_index], y[test_index]
+
+        X_train.reverse()
+        X_test.reverse()
+        nc = copy.deepcopy(c)
+        nc.reverse()
+        X_train = [X_train.pop() if isinstance(xi, np.ndarray) else nc.pop() for index, xi in enumerate(x)]
+        nc = copy.deepcopy(c)
+        nc.reverse()
+        X_test = [X_test.pop() if isinstance(xi, np.ndarray) else nc.pop() for index, xi in enumerate(x)]
+
+        pre_y, expr01 = calculate_y(expr01, X_train, y_train, terminals,
+                                    x_test=X_test, y_test=y_test,
+                                    add_coef=add_coef,
+                                    filter_warning=filter_warning, inter_add=inter_add,
+                                    inner_add=inner_add,
+                                    vector_add=vector_add, out_add=out_add, flat_add=flat_add,
+                                    np_maps=np_maps)
 
-        if True:
-            _, expr01, _ = calculate_score(expr01, x, y, terminals, scoring=scoring, score_pen=score_pen,
-                                           add_coef=add_coef, filter_warning=filter_warning,
-                                           inter_add=inter_add,
-                                           inner_add=inner_add, vector_add=vector_add, out_add=out_add,
-                                           flat_add=flat_add, np_maps=np_maps, classification=classification,
-                                           score_object=score_object, details=details)
-
-        cv_sc_all = []
-        # cv_expr01 = []
-        cv_pre_y = []
-        xx = [xi for xi in x if isinstance(xi, np.ndarray)]
-        c = [xi for xi in x if not isinstance(xi, np.ndarray)]
-        xx = [xi.reshape((-1, 1)) if xi.ndim == 1 else xi.T for xi in xx]
-
-        for train_index, test_index in cv.split(xx[0], y):
-
-            X_train = [xi[train_index] for xi in xx]
-            X_test = [xi[test_index] for xi in xx]
-            y_train, y_test = y[train_index], y[test_index]
-
-            X_train.reverse()
-            X_test.reverse()
-            nc = copy.deepcopy(c)
-            nc.reverse()
-            X_train = [X_train.pop() if isinstance(xi, np.ndarray) else nc.pop() for index, xi in enumerate(x)]
-            nc = copy.deepcopy(c)
-            nc.reverse()
-            X_test = [X_test.pop() if isinstance(xi, np.ndarray) else nc.pop() for index, xi in enumerate(x)]
-
-            pre_y, expr01 = calculate_y(expr01, X_train, y_train, terminals,
-                                        x_test=X_test, y_test=y_test,
-                                        add_coef=False,
-                                        filter_warning=filter_warning, inter_add=inter_add,
-                                        inner_add=inner_add,
-                                        vector_add=vector_add, out_add=out_add, flat_add=flat_add,
-                                        np_maps=np_maps, classification=classification)
-
-            try:
-                sc_all = []
-                for si, sp in zip(scoring, score_pen):
-                    sc = si(y_test, pre_y)
-                    if np.isnan(sc):
-                        sc = uniform_score(score_pen=sp)
-                    sc_all.append(sc)
-
-            except (ValueError, RuntimeWarning, TypeError):
-
-                sc_all = [uniform_score(score_pen=i) for i in score_pen]
-
-            cv_sc_all.append(sc_all)
-            # cv_expr01.append(expr01)
-            cv_pre_y.append(pre_y)
-
-        sc_all = list(np.mean(np.array(cv_sc_all), axis=0))
         try:
-            pre_y = np.concatenate(cv_pre_y)
-        except ValueError:
-            pre_y = None
-
-        if refit is True:
-            "the refit only use for see the detial of calcualtion after loop"
-            sc_all0, expr01, pre_y0 = calculate_score(expr01, x, y, terminals, scoring=scoring, score_pen=score_pen,
-                                                      add_coef=add_coef, filter_warning=filter_warning,
-                                                      inter_add=inter_add,
-                                                      inner_add=inner_add, vector_add=vector_add, out_add=out_add,
-                                                      flat_add=flat_add, np_maps=np_maps, classification=classification,
-                                                      score_object=score_object, details=details)
+            sc_all = []
+            for si, sp in zip(scoring, score_pen):
+                sc = si(y_test, pre_y)
+                if np.isnan(sc):
+                    sc = uniform_score(score_pen=sp)
+                sc_all.append(sc)
 
-        return sc_all, expr01, pre_y
+        except (ValueError, RuntimeWarning):
+
+            sc_all = [uniform_score(score_pen=i) for i in score_pen]
+
+        cv_sc_all.append(sc_all)
+        cv_expr01.append(expr01)
+        cv_pre_y.append(pre_y)
+
+    sc_all = list(np.mean(np.array(cv_sc_all), axis=0))
+    try:
+        pre_y = np.concatenate(cv_pre_y)
+    except ValueError:
+        pre_y = None
+
+    if refit is True:
+        "the refit only use for see the detial of calcualtion after loop"
+        sc_all0, expr01, pre_y0 = calculate_score(expr01, x, y, terminals, scoring=scoring, score_pen=score_pen,
+                                                  add_coef=add_coef, filter_warning=filter_warning, inter_add=inter_add,
+                                                  inner_add=inner_add, vector_add=vector_add, out_add=out_add,
+                                                  flat_add=flat_add, np_maps=np_maps)
+
+    return sc_all, expr01, pre_y
 
 
 def score_dim(dim_, dim_type, fuzzy=False):
     if dim_type is None:
         return 1
     elif isinstance(dim_type, str):
         if dim_type == 'integer':
             return 1 if dim_.isinteger() else 0
         elif dim_type == 'coef':
             return 1 if not dim_.anyisnan() else 0
-        elif dim_type == 'ignore':
-            return 1
         else:
             raise TypeError("dim_type should be None,'coef', 'integer', special Dim or list of Dim")
     elif isinstance(dim_type, list):
         return 1 if dim_ in dim_type else 0
     elif isinstance(dim_type, Dim):
         if fuzzy:
             return 1 if dim_.is_same_base(dim_type) else 0
@@ -478,15 +328,15 @@
         dimension
     dim_score
         is target dim or not
     """
     terminals = [str(i) for i in terminals]
     if not dim_maps:
         dim_maps = dim_map()
-    func0 = utilities.lambdify(terminals, expr01, modules=[dim_maps])
+    func0 = sympy.utilities.lambdify(terminals, expr01, modules=[dim_maps])
     try:
         dim_ = func0(*dim_list)
     except (ValueError, TypeError, ZeroDivisionError, NameError):
         dim_ = dnan
     if isinstance(dim_, (float, int)):
         dim_ = dless
     if not isinstance(dim_, Dim):
@@ -522,42 +372,39 @@
     """
     dim_ = calcualte_dim(expr01, terminals, dim_list, dim_maps=dim_maps)
 
     dim_score = score_dim(dim_, dim_type, fuzzy)
     return dim_, dim_score
 
 
-def calculate_collect_(ind, context, x, y, terminals_and_constants_repr, gro_ter_con,
-                       dim_ter_con_list, dim_type, fuzzy, cv=1, refit=True,
-                       scoring=None, score_pen=(1,),
-                       add_coef=True, filter_warning=True, inter_add=True, inner_add=False,
-                       vector_add=False, out_add=False, flat_add=False,
-                       np_maps=None, classification=False, dim_maps=None, cal_dim=True, score_object="y",
-                       details=False):
+def calculate_collect(ind, context, x, y, terminals_and_constants_repr, gro_ter_con,
+                      dim_ter_con_list, dim_type, fuzzy, cv=1, refit=True,
+                      scoring=None, score_pen=(1,),
+                      add_coef=True, filter_warning=True, inter_add=True, inner_add=False,
+                      vector_add=False, out_add=False, flat_add=False,
+                      np_maps=None, dim_maps=None, cal_dim=True):
     expr01 = compile_context(ind, context, gro_ter_con)
 
-    if cal_dim:
-        dim, dim_score = calcualte_dim_score(expr01, terminals_and_constants_repr,
-                                             dim_ter_con_list, dim_type, fuzzy,
-                                             dim_maps=dim_maps)
-    else:
-        dim, dim_score = dless, 1
-
     score, expr01, pre_y = calculate_cv_score(expr01, x, y, terminals_and_constants_repr,
                                               cv=cv, refit=refit,
                                               add_coef=add_coef, inter_add=inter_add,
                                               inner_add=inner_add, vector_add=vector_add, out_add=out_add,
                                               flat_add=flat_add,
                                               scoring=scoring, score_pen=score_pen,
                                               filter_warning=filter_warning,
-                                              np_maps=np_maps, classification=classification, score_object=score_object,
-                                              details=details
-                                              )
+                                              np_maps=np_maps)
+
+    if cal_dim:
+        dim, dim_score = calcualte_dim_score(expr01, terminals_and_constants_repr,
+                                             dim_ter_con_list, dim_type, fuzzy,
+                                             dim_maps=dim_maps)
+    else:
+        dim, dim_score = dless, 1
 
-    return score, dim, dim_score, expr01, pre_y
+    return score, dim, dim_score
 
 
 score_collection = {'explained_variance': metrics.explained_variance_score,
                     'max_error': metrics.max_error,
                     'neg_mean_absolute_error': metrics.mean_absolute_error,
                     'neg_mean_squared_error': metrics.mean_squared_error,
                     'neg_root_mean_squared_error': metrics.mean_squared_error,
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `BindingGP-0.0.36/bgp/calculation/translate.py` & `BindingGP-0.0.9/BGP/calculation/translate.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,16 @@
 import copy
 import sys
 
 import numpy as np
 import sympy
+from BGP.calculation.coefficient import get_args
 from sympy import Number, Expr
 from sympy.core.numbers import ComplexInfinity, NumberSymbol
 
-from bgp.calculation.coefficient import get_args
-
 """lambidfy"""
 
 
 def general_expr_dict(self, expr_init_map, free_symbol, gsym_map, simplifying=False):
     """gen expr"""
 
     init_sub = expr_init_map.items()
@@ -47,15 +46,14 @@
 
     return res
 
 
 def group_str(self, pset, feature_name=False):
     """
     return expr just build by input feature name.
-
     Parameters
     ----------
     self:sympy.Expr or SymbolTree
     pset:SymbolSet
     feature_name:Bool
 
     Returns
@@ -127,39 +125,33 @@
         else:
             print("Don not assign the feature_name to pset when pest.add_features")
     print(name_subd)
     return name_subd
 
 
 def simple(expr01, groups):
-    """
-    str to sympy.Expr function.
+    """str to sympy.Expr function.
     add conv to MMdd and MMul.
-    the calcualte conv need conform with np_func()!!
-    
-    is_jump: jump the calculate >= 3 (group_size).
-    keep: the calculate is return then input group_size or 1.
+    !!!!!!! the calcualte conv need conform with np_func().
+        is_jump: jump the calculate >= 3 (group_size).
+        keep: the calculate is return then input group_size or 1.
     """
 
     def max_method(expr):
 
         new = [calculate_number(i) for i in expr.args]
-        try:
-            exprarg_new = list(zip(*new))[0]
-            n = list(list(zip(*new))[1])
-            expr = expr.func(*exprarg_new)
-            n.append(1)
-            le = len(set(n))
-            if le >= 3:
-                return expr, np.nan
-            else:
-                return expr, max(n)
-        except IndexError:
-            print(expr)
+        exprarg_new = list(zip(*new))[0]
+        n = list(list(zip(*new))[1])
+        expr = expr.func(*exprarg_new)
+        n.append(1)
+        le = len(set(n))
+        if le >= 3:
             return expr, np.nan
+        else:
+            return expr, max(n)
 
     def calculate_number(expr):
 
         if isinstance(expr, sympy.Symbol):
             return expr, groups[expr.name]
         elif isinstance(expr, (Number, ComplexInfinity)):
             return expr, 1
```

### Comparing `BindingGP-0.0.36/bgp/flow.py` & `BindingGP-0.0.9/BGP/flow.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,349 +1,262 @@
 # #!/usr/bin/python
 # # -*- coding: utf-8 -*-
 #
 # # @Time    : 2019/11/12 15:13
 # # @Email   : 986798607@qq.com
 # # @Software: PyCharm
 # # @License: GNU Lesser General Public License v3.0
-"""
-Some definition loop for genetic algorithm.
-All the loop is with same run method.
 
-Contains:
-
--Class: ``BaseLoop``
-
-    one node mate and one tree mutate.
-
--Class: ``MultiMutateLoop``
-
-    one node mate and (one tree mutate, one node Replacement mutate, shrink mutate, difference mutate).
-
--Class: ``OnePointMutateLoop``
-
-    one node Replacement mutate: (keep height of tree)
-
--Class: ``DimForceLoop``
-
-    Select with dimension : (keep dimension of tree)
-
-"""
 import copy
 import operator
 import os
 import time
 
+import sympy
 from deap.base import Fitness
 from deap.tools import HallOfFame, Logbook
+from BGP.base import CalculatePrecisionSet
+from BGP.base import SymbolSet
+from BGP.base import SymbolTree
+from BGP.calculation.translate import compile_context, general_expr
+from BGP.functions.dimfunc import Dim, dless
+from BGP.gp import cxOnePoint, varAnd, genGrow, staticLimit, selKbestDim, \
+    selTournament, Statis_func, mutUniform, mutShrink, varAndfus, \
+    mutDifferentReplacementVerbose, mutNodeReplacementVerbose, selBest, genFull
 from mgetool import newclass
 from mgetool.exports import Store
 from mgetool.packbox import Toolbox
 from numpy import random
-
+from sklearn.datasets import load_boston
 from sklearn.metrics import r2_score
 
-from bgp.base import CalculatePrecisionSet
-from bgp.base import SymbolSet
-from bgp.base import SymbolTree
-from bgp.functions.dimfunc import Dim, dless
-from bgp.gp import cxOnePoint, varAnd, genGrow, staticLimit, selKbestDim, \
-    selTournament, Statis_func, mutUniform, mutShrink, varAndfus, \
-    mutDifferentReplacementVerbose, mutNodeReplacementVerbose, selBest, genFull
-
 
 class BaseLoop(Toolbox):
-    """
-    Base loop for BGP.
-
-    Examples::
-
-        if __name__ == "__main__":
-            pset = SymbolSet()
-            stop = lambda ind: ind.fitness.values[0] >= 0.880963
-
-            bl = BaseLoop(pset=pset, gen=10, pop=1000, hall=1, batch_size=40, re_hall=3, \n
-            n_jobs=12, mate_prob=0.9, max_value=5, initial_min=1, initial_max=2, \n
-            mutate_prob=0.8, tq=True, dim_type="coef", stop_condition=stop,\n
-            re_Tree=0, store=False, random_state=1, verbose=True,\n
-            stats={"fitness_dim_max": ["max"], "dim_is_target": ["sum"]},\n
-            add_coef=True, inter_add=True, inner_add=False, cal_dim=True, vector_add=False,\n
-            personal_map=False)
+    """Base loop"""
 
-            bl.run()
-
-    """
-
-    def __init__(self, pset, pop=500, gen=20, mutate_prob=0.5, mate_prob=0.8, hall=1, re_hall=1,
+    def __init__(self, pset, pop=500, gen=20, mutate_prob=0.5, mate_prob=0.8, hall=1, re_hall=None,
                  re_Tree=None, initial_min=None, initial_max=3, max_value=5,
                  scoring=(r2_score,), score_pen=(1,), filter_warning=True, cv=1,
                  add_coef=True, inter_add=True, inner_add=False, vector_add=False, out_add=False, flat_add=False,
                  cal_dim=False, dim_type=None, fuzzy=False, n_jobs=1, batch_size=40,
                  random_state=None, stats=None, verbose=True, migrate_prob=0,
-                 tq=True, store=False, personal_map=False, stop_condition=None, details=False, classification=False,
-                 score_object="y", sub_mu_max=1, limit_type="h_bgp", batch_para=False):
+                 tq=True, store=False, personal_map=False, stop_condition=None):
         """
 
         Parameters
         ----------
         pset:SymbolSet
-            the feature x and target y and others should have been added.
-        pop: int
-            number of population.
-        gen: int
-            number of generation.
+            the feature x and traget y and others should have been added.
+        pop:int
+            number of popolation
+        gen:int
+            number of generation
         mutate_prob:float
-            probability of mutate.
+            probability of mutate
         mate_prob:float
-            probability of mate(crossover).
+            probability of mate(crossover)
         initial_max:int
             max initial size of expression when first producing.
         initial_min : None,int
-            min initial size of expression when first producing.
+            max initial size of expression when first producing.
         max_value:int
-            max size of expression.
-        limit_type: "height" or "length",","h_bgp"
-            limitation type for max_value, but don't affect initial_max, initial_min.
+            max size of expression
         hall:int,>=1
-            number of HallOfFame (elite) to maintain.
+            number of HallOfFame(elite) to maintain
         re_hall:None or int>=2
-            Notes: only valid when hall
+            Notes: only vaild when hall
             number of HallOfFame to add to next generation.
         re_Tree: int
             number of new features to add to next generation.
             0 is false to add.
         personal_map:bool or "auto"
-            "auto" is using 'premap' and with auto refresh the 'premap' with individual.\n
-            True is just using constant 'premap'.\n
+            "auto" is using premap and with auto refresh the premap with individual.\n
+            True is just using constant premap.\n
             False is just use the prob of terminals.
-        scoring: list of Callable, default is [sklearn.metrics.r2_score,]
-            See Also ``sklearn.metrics``
+        scoring: list of Callbale, default is [sklearn.metrics.r2_score,]
+            See Also sklearn.metrics
         score_pen: tuple of  1, -1 or float but 0.
-            >0 : max problem, best is positive, worse -np.inf.
-            <0 : min problem, best is negative, worse np.inf.
-
+            >0 : max problem, best is positive, worse -np.inf
+            <0 : min problem, best is negative, worse np.inf
             Notes:
-                if multiply score method, the scores must be turn to same dimension in prepossessing
-                or weight by score_pen. Because the all the selection are stand on the mean(w_i*score_i)
-
-            Examples::
-
-                scoring = [r2_score,]
-                score_pen= [1,]
-
-        cv:sklearn.model_selection._split._BaseKFold,int
-            the shuffler must be False,
-            default=1 means no cv.
+            if multiply score method, the scores must be turn to same dimension in preprocessing
+            or weight by score_pen. Because the all the selection are stand on the mean(w_i*score_i)
+            Examples: [r2_score] is [1],
+        cv=int,sklearn.model_selection._split._BaseKFold
+            default =1, means not cv
         filter_warning:bool
-            filter warning or not.
+            filter warning or not
         add_coef:bool
             add coef in expression or not.
         inter_add：bool
-            add intercept constant or not.
+            add intercept constant or not
         inner_add:bool
-            add inner coefficients or not.
+            add inner coeffcients or not
         out_add:bool
-            add out coefficients or not.
+            add out coeffcients or not
         flat_add:bool
-            add flat coefficients or not.
+            add flat coeffcients or not
         n_jobs:int
-            default 1, advise 6.
+            default 1, advise 6
         batch_size:int
-            default 40, depend of machine.
+            default 40, depend of machine
         random_state:int
-            None,int.
+            None,int
         cal_dim:bool
-            escape the dim calculation.
+            excape the dim calculation
         dim_type:Dim or None or list of Dim
-            "coef": af(x)+b. a,b have dimension,f(x)'s dimension is not dnan. \n
-            "integer": af(x)+b. f(x) is with integer dimension. \n
-            [Dim1,Dim2]: f(x)'s dimension in list. \n
+            "coef": af(x)+b. a,b have dimension,f(x) is not dnan. \n
+            "integer": af(x)+b. f(x) is interger dimension. \n
+            [Dim1,Dim2]: f(x) in list. \n
             Dim: f(x) ~= Dim. (see fuzzy) \n
             Dim: f(x) == Dim. \n
             None: f(x) == pset.y_dim
         fuzzy:bool
-            choose the dim with same base with dim_type, such as m,m^2,m^3.
+            choose the dim with same base with dim_type,such as m,m^2,m^3.
         stats:dict
             details of logbook to show. \n
             Map:\n
-            values
+            values 
                 = {"max": np.max, "mean": np.mean, "min": np.mean, "std": np.std, "sum": np.sum}
             keys
                 = {\n
                    "fitness": just see fitness[0], \n
                    "fitness_dim_max": max problem, see fitness with demand dim,\n
                    "fitness_dim_min": min problem, see fitness with demand dim,\n
                    "dim_is_target": demand dim,\n
-                   "coef":  dim is True, coef have dim, \n
+                   "coef":  dim is true, coef have dim, \n
                    "integer":  dim is integer, \n
                    ...
                    }
-
-            if stats is None, default is:
-
-            for cal_dim=True:
-                stats = {"fitness_dim_max": ("max",), "dim_is_target": ("sum",)}
-
-            for cal_dim=False
-                stats = {"fitness": ("max",)}
-
-            if self-definition, the key is func to get attribute of each ind.
-
-            Examples::
-
-                def func(ind):
+            if stats is None, default is :\n
+                stats = {"fitness_dim_max": ("max",), "dim_is_target": ("sum",)}   for cal_dim=True
+                stats = {"fitness": ("max",)}                                      for cal_dim=False
+            if self-definition, the key is func to get attribute of each ind./n
+            Examples:
+                def func(ind):\n
                     return ind.fitness[0]
                 stats = {func: ("mean",), "dim_is_target": ("sum",)}
-
         verbose:bool
-            print verbose logbook or not.
+            print verbose logbook or not
         tq:bool
-            print progress bar or not.
+            print progress bar or not
         store:bool or path
-            bool or path.
+            bool or path
         stop_condition:callable
             stop condition on the best ind of hall, which return bool,the true means stop loop.
-
-            Examples::
-
-                def func(ind):
+            Examples:
+                def func(ind):\n
                     c = ind.fitness.values[0]>=0.90
                     return c
-
-        details:bool
-            return expr and predict_y or not.
-
-        classification: bool
-            classification or not.
-
-        score_object:
-            score by y or delta y (for implicit function).
         """
         super(BaseLoop, self).__init__()
-
         assert initial_max <= max_value, "the initial size of expression should less than max_value limitation"
         if cal_dim:
             assert all(
                 [isinstance(i, Dim) for i in pset.dim_ter_con.values()]), \
                 "all import dim of pset should be Dim object."
 
-        self.details = details
+        random.seed(random_state)
+
         self.max_value = max_value
         self.pop = pop
         self.gen = gen
         self.mutate_prob = mutate_prob
         self.mate_prob = mate_prob
         self.migrate_prob = migrate_prob
         self.verbose = verbose
         self.cal_dim = cal_dim
         self.re_hall = re_hall
         self.re_Tree = re_Tree
         self.store = store
-        self.limit_type = limit_type
         self.data_all = []
         self.personal_map = personal_map
         self.stop_condition = stop_condition
-        self.population = []
-        self.rand_state = None
-        self.random_state = random_state
-        self.sub_mu_max = sub_mu_max
-        self.population_next = []
 
         self.cpset = CalculatePrecisionSet(pset, scoring=scoring, score_pen=score_pen,
                                            filter_warning=filter_warning, cal_dim=cal_dim,
                                            add_coef=add_coef, inter_add=inter_add, inner_add=inner_add,
                                            vector_add=vector_add, out_add=out_add, flat_add=flat_add, cv=cv,
                                            n_jobs=n_jobs, batch_size=batch_size, tq=tq,
-                                           fuzzy=fuzzy, dim_type=dim_type, details=details,
-                                           classification=classification, score_object=score_object,
-                                           batch_para=batch_para
+                                           fuzzy=fuzzy, dim_type=dim_type,
                                            )
 
         Fitness_ = newclass.create("Fitness_", Fitness, weights=score_pen)
         self.PTree = newclass.create("PTrees", SymbolTree, fitness=Fitness_)
         # def produce
         if initial_min is None:
             initial_min = 2
         self.register("genGrow", genGrow, pset=self.cpset, min_=initial_min, max_=initial_max + 1,
                       personal_map=self.personal_map)
         self.register("genFull", genFull, pset=self.cpset, min_=initial_min, max_=initial_max + 1,
                       personal_map=self.personal_map)
-        self.register("genHalf", genGrow, pset=self.cpset, min_=initial_min, max_=initial_max + 1,
-                      personal_map=self.personal_map)
-        self.register("gen_mu", genGrow, min_=1, max_=self.sub_mu_max + 1, personal_map=self.personal_map)
+        self.register("gen_mu", genGrow, min_=1, max_=1 + 1, personal_map=self.personal_map)
         # def selection
 
         self.register("select", selTournament, tournsize=2)
 
         self.register("selKbestDim", selKbestDim,
                       dim_type=self.cpset.dim_type, fuzzy=self.cpset.fuzzy)
         self.register("selBest", selBest)
 
         self.register("mate", cxOnePoint)
         # def mutate
 
         self.register("mutate", mutUniform, expr=self.gen_mu, pset=self.cpset)
 
-        self.decorate("mate", staticLimit(key=operator.attrgetter(limit_type), max_value=self.max_value))
-        self.decorate("mutate", staticLimit(key=operator.attrgetter(limit_type), max_value=self.max_value))
+        self.decorate("mate", staticLimit(key=operator.attrgetter("height"), max_value=2 * (max_value + 1)))
+        self.decorate("mutate", staticLimit(key=operator.attrgetter("height"), max_value=2 * (max_value + 1)))
 
         if stats is None:
             if cal_dim:
-                if score_pen[0] > 0:
-                    stats = {"fitness_dim_max": ("max",), "dim_is_target": ("sum",)}
-                else:
-                    stats = {"fitness_dim_min": ("min",), "dim_is_target": ("sum",)}
+                stats = {"fitness_dim_max": ("max",), "dim_is_target": ("sum",)}
             else:
-                if score_pen[0] > 0:
-                    stats = {"fitness": ("max",)}
-                else:
-                    stats = {"fitness": ("min",)}
+                stats = {"fitness": ("max",)}
 
         self.stats = Statis_func(stats=stats)
         logbook = Logbook()
         logbook.header = ['gen'] + (self.stats.fields if self.stats else [])
         self.logbook = logbook
 
         if hall is None:
             hall = 1
         self.hall = HallOfFame(hall)
 
         if re_hall is None:
             self.re_hall = None
         else:
-            if re_hall == 1 or re_hall == 0:
+            if re_hall is 1 or re_hall is 0:
                 print("re_hall should more than 1")
                 re_hall = 2
             assert re_hall >= hall, "re_hall should more than hall"
             self.re_hall = HallOfFame(re_hall)
 
     def varAnd(self, *arg, **kwargs):
         return varAnd(*arg, **kwargs)
 
     def to_csv(self, data_all):
-        """store to csv"""
         if self.store:
             if isinstance(self.store, str):
                 path = self.store
             else:
                 path = os.getcwd()
             file_new_name = "_".join((str(self.pop), str(self.gen),
                                       str(self.mutate_prob), str(self.mate_prob),
                                       str(time.time())))
             try:
                 st = Store(path)
-                st.to_csv(data_all, file_new_name, transposition=True)
+                st.to_csv(data_all, file_new_name)
                 print("store data to ", path, file_new_name)
             except (IOError, PermissionError):
                 st = Store(os.getcwd())
-                st.to_csv(data_all, file_new_name, transposition=True)
+                st.to_csv(data_all, file_new_name)
                 print("store data to ", os.getcwd(), file_new_name)
 
     def maintain_halls(self, population):
-        """maintain the best p expression"""
+
         if self.re_hall is not None:
             maxsize = max(self.hall.maxsize, self.re_hall.maxsize)
 
             if self.cal_dim:
                 inds_dim = self.selKbestDim(population, maxsize)
             else:
                 inds_dim = self.selBest(population, maxsize)
@@ -362,251 +275,136 @@
             self.hall.update(inds_dim)
             inds_dim = []
 
         inds_dim = copy.deepcopy(inds_dim)
         return inds_dim
 
     def re_add(self):
-        """add the expression as a feature"""
         if self.hall.items and self.re_Tree:
             it = self.hall.items
             indo = it[random.choice(len(it))]
             ind = copy.deepcopy(indo)
             inds = ind.depart()
             if not inds:
                 pass
             else:
                 inds = [self.cpset.calculate_detail(indi) for indi in inds]
                 le = min(self.re_Tree, len(inds))
                 indi = inds[random.choice(le)]
                 self.cpset.add_tree_to_features(indi)
 
     def re_fresh_by_name(self, *arr):
-        re_name = ["mutate", "genGrow", "genFull", "genHalf"]
+        re_name = ["mutate", "genGrow", "genFull"]
         if len(arr) > 0:
             re_name.extend(arr)
         self.refresh(re_name, pset=self.cpset)
-        # for i in re_name + ["mate"]:  # don‘t del this
-        #     self.decorate(i, staticLimit(key=operator.attrgetter("height"), max_value=2 * (self.max_value + 1)))
-
-    def top_n(self, n=10, gen=-1, key="value", filter_dim=True, ascending=False):
-        """
-        Return the best n results.
-
-        Note:
-            Only valid in ``store=True``.
-
-        Parameters
-        ----------
-        n:int
-            n.
-        gen:
-            the generation, default is -1.
-        key: str
-            sort keys, default is "values".
-        filter_dim:
-            filter no-dim expressions or not.
-        ascending:
-            reverse.
-
-        Returns
-        -------
-        top n results.
-        pd.DataFrame
-
-        """
-        if self.store is False:
-            raise TypeError("Only valid with parameter: store=True")
-
-        import pandas as pd
-        data = self.data_all
-
-        data = pd.DataFrame(data)
-        if gen == -1:
-            gen = max(data["gen"])
-
-        data = data[data["gen"] == gen]
-
-        if filter_dim:
-            data = data[data["dim_score"] == 1]
-
-        data = data.drop_duplicates(['expr'], keep="first")
 
-        if key is not None:
-            data[key] = data[key].str.replace("(", "")
-            data[key] = data[key].str.replace(")", "")
-            data[key] = data[key].str.replace(",", "")
-            try:
-                data[key] = data[key].astype(float)
-            except ValueError:
-                raise TypeError("check this key column can be translated into float")
-
-            data = data.sort_values(by='value', ascending=ascending).iloc[:n, :]
-
-        return data
-
-    def check_height_length(self, pop, site=""):
-        old = len(pop)
-        if self.limit_type == 'height':
-            pop = [i for i in pop if i.height <= self.max_value]
-        elif self.limit_type == 'length':
-            pop = [i for i in pop if i.length <= self.max_value]
-        else:
-            pop = [i for i in pop if i.h_bgp <= self.max_value]
-        new = len(pop)
-        if old == new:
-            pass
-        else:
-            if site != "":
-                print(site)
-            # raise TypeError
-            index = random.randint(0, new, old - new)
-            pop.extend([pop[i] for i in index])
-        return pop
-
-    def run(self, warm_start=False, new_gen=None):
-        """
-
-        Parameters
-        ----------
-        warm_start:bool
-            warm_start from last result.
-        new_gen:
-            new generations for warm_startm, default is the initial generations.
-
-        """
+    def run(self):
         # 1.generate###################################################################
-        if warm_start is False:
-            random.seed(self.random_state)
-            population = [self.PTree(self.genHalf()) for _ in range(self.pop)]
-            gen_i = 0
-            gen = self.gen
-        else:
-            assert self.population_next != []
-            random.set_state(self.rand_state)
-            population = self.population_next
-            gen_i = self.gen_i
-            self.re_fresh_by_name()
-            if new_gen:
-                gen = gen_i + new_gen
-            else:
-                gen = gen_i + self.gen
+        population = [self.PTree(self.genFull()) for _ in range(self.pop)]
 
-        for gen_i in range(gen_i + 1, gen + 1):
+        for gen_i in range(1, self.gen + 1):
 
             population_old = copy.deepcopy(population)
 
             # 2.evaluate###############################################################
-
             invalid_ind_score = self.cpset.parallelize_score(population_old)
 
             for ind, score in zip(population_old, invalid_ind_score):
                 ind.fitness.values = tuple(score[0])
                 ind.y_dim = score[1]
                 ind.dim_score = score[2]
-                ind.coef_expr = score[3]
-                ind.coef_pre_y = score[4]
+
             population = population_old
+
             # 3.log###################################################################
             # 3.1.log-print##############################
 
             record = self.stats.compile(population) if self.stats else {}
             self.logbook.record(gen=gen_i, **record)
             if self.verbose:
                 print(self.logbook.stream)
+
             # 3.2.log-store##############################
             if self.store:
-                datas = [{"gen": gen_i, "name": str(pop_i), "expr": pop_i.coef_expr,
-                          "value": str(pop_i.fitness.values),
-                          "dimension": str(pop_i.y_dim),
-                          "dim_score": pop_i.dim_score} for pop_i in population]
+                datas = [{"gen": gen_i, "name": str(gen_i), "value": str(gen_i.fitness.values),
+                          "dimension": str(gen_i.y_dim),
+                          "dim_score": str(gen_i.dim_score)} for gen_i in population]
                 self.data_all.extend(datas)
 
-            self.population = copy.deepcopy(population)
-
             # 3.3.log-hall###############################
             inds_dim = self.maintain_halls(population)
 
             # 4.refresh################################################################
             # 4.1.re_update the premap ##################
             if self.personal_map == "auto":
                 [self.cpset.premap.update(indi, self.cpset) for indi in inds_dim]
 
             # 4.2.re_add_tree and refresh pset###########
             if self.re_Tree:
                 self.re_add()
 
             self.re_fresh_by_name()
 
-            # 6.next generation ！！！！#######################################################
+            # 5.break#######################################################
+            if self.stop_condition is not None:
+                if self.stop_condition(self.hall.items[0]):
+                    break
+            # 6.next generation#######################################################
             # selection and mutate,mate,migration
             population = self.select(population, int((1 - self.migrate_prob) * len(population)) - len(inds_dim))
 
             offspring = self.varAnd(population, self, self.mate_prob, self.mutate_prob)
+
             offspring.extend(inds_dim)
             migrate_pop = [self.PTree(self.genFull()) for _ in range(int(self.migrate_prob * len(population)))]
             population[:] = offspring + migrate_pop
 
-            population = self.check_height_length(population)
-
-            # 5.break#######################################################
-            if self.stop_condition is not None:
-                if self.stop_condition(self.hall.items[0]):
-                    break
-
-            # 7 freeze ###################################################
-
-            self.rand_state = random.get_state()
-            self.population_next = population
-            self.gen_i = gen_i
-
-        # final.store#####################################################################
+        # 7.store#####################################################################
 
         if self.store:
             self.to_csv(self.data_all)
         self.hall.items = [self.cpset.calculate_detail(indi) for indi in self.hall.items]
 
         return self.hall
 
 
-class MultiMutateLoop(BaseLoop):
+class MutilMutateLoop(BaseLoop):
     """
     multiply mutate method.
     """
 
     def __init__(self, *args, **kwargs):
         """See also BaseLoop"""
-        super(MultiMutateLoop, self).__init__(*args, **kwargs)
+        super(MutilMutateLoop, self).__init__(*args, **kwargs)
 
         self.register("mutate0", mutNodeReplacementVerbose, pset=self.cpset, personal_map=self.personal_map)
 
         self.register("mutate1", mutUniform, expr=self.gen_mu, pset=self.cpset)
-        self.decorate("mutate1", staticLimit(key=operator.attrgetter("height"), max_value=2 * (self.max_value + 1)))
+        self.decorate("mutate1", staticLimit(key=operator.attrgetter("height"), max_value=2 * self.max_value))
 
         self.register("mutate2", mutShrink, pset=self.cpset)
 
         self.register("mutate3", mutDifferentReplacementVerbose, pset=self.cpset, personal_map=self.personal_map)
 
-        self.mutpb_list = [0.1, 0.5, 0.2, 0.2]
-
     def varAnd(self, population, toolbox, cxpb, mutpb):
         names = self.__dict__.keys()
         import re
         patt = r'mutate[0-9]'
         pattern = re.compile(patt)
         result = [pattern.findall(i) for i in names]
         att_name = []
         for i in result:
             att_name.extend(i)
 
         self.re_fresh_by_name(*att_name)
 
         fus = [getattr(self, i) for i in att_name]
 
-        off = varAndfus(population, toolbox, cxpb, mutpb, fus, self.mutpb_list)
+        off = varAndfus(population, toolbox, cxpb, mutpb, fus)
 
         return off
 
 
 class OnePointMutateLoop(BaseLoop):
     """
     limitation height of population, just use mutNodeReplacementVerbose method.
@@ -635,32 +433,31 @@
         fus = [getattr(self, i) for i in att_name]
 
         off = varAndfus(population, toolbox, cxpb, mutpb, fus)
 
         return off
 
 
-class DimForceLoop(MultiMutateLoop):
+class DimForceLoop(MutilMutateLoop):
     """Force select the individual with target dim for next generation"""
 
     def __init__(self, *args, **kwargs):
         """See also BaseLoop"""
         super(DimForceLoop, self).__init__(*args, **kwargs)
         assert self.cal_dim == True, "For DimForceLoop type, the 'cal_dim' must be True"
 
         self.register("select", selKbestDim,
                       dim_type=self.cpset.dim_type, fuzzy=self.cpset.fuzzy, force_number=True)
 
 
 if __name__ == "__main__":
     # data
-    from sklearn.datasets import fetch_california_housing
-    data = fetch_california_housing()
-    x = data["data"][:100]
-    y = data["target"][:100]
+    data = load_boston()
+    x = data["data"]
+    y = data["target"]
     c = [6, 3, 4]
     # unit
     from sympy.physics.units import kg
 
     x_u = [kg] * 13
     y_u = kg
     c_u = [dless, dless, dless]
@@ -675,44 +472,41 @@
     pset0 = SymbolSet()
     pset0.add_features(x, y, x_dim=x_dim, y_dim=y_dim, x_group=[[1, 2], [3, 4], [5, 6]])
     pset0.add_constants(c, c_dim=c_dim, c_prob=None)
     pset0.add_operations(power_categories=(2, 3, 0.5),
                          categories=("Add", "Mul", "Sub", "Div", "exp", "Abs"))
 
     # a = time.time()
-
-    bl = MultiMutateLoop(pset=pset0, gen=20, pop=2000, hall=2, batch_size=60, re_hall=2,
-                         n_jobs=1, mate_prob=1, max_value=3, initial_max=1, initial_min=1,
+    bl = MutilMutateLoop(pset=pset0, gen=4, pop=10, hall=2, batch_size=40, re_hall=2,
+                         n_jobs=1, mate_prob=1, max_value=10, initial_max=3,
                          mutate_prob=0.8, tq=True, dim_type="coef",
-                         re_Tree=None, store=False, random_state=2,
-                         stats={"fitness_dim_max": ["max"], "dim_is_target": ["sum"], "h_bgp": ["max"]},
-                         add_coef=True, cal_dim=False, inner_add=False, vector_add=True, personal_map=False)
+                         re_Tree=2, store=False, random_state=1,
+                         stats={"fitness_dim_max": ["max"], "dim_is_target": ["sum"], "height": ["mean"]},
+                         add_coef=True, cal_dim=True, inner_add=False, vector_add=True, personal_map=False)
     # b = time.time()
     bl.run()
-    bl.run(warm_start=True)
-
-    # population = [bl.PTree(bl.genFull()) for _ in range(30)]
-    # pset = bl.cpset
-    # for i in population:
-    #     # i.ppprint(bl.cpset)
-    #     # i = "exp(gx0/gx1)"
-    #
-    #     i = compile_context(i, pset.context, pset.gro_ter_con, simplify=False)
-    #     # print(i)
-    #     # print(i)
-    #     # fun = Coef("V", np.array([1.4,1.3]))
-    #     # i = fun(i)
-    #     # f = Function("MAdd")
-    #     # i = f(i)
-    #     try:
-    #         # group_str(i,pset)
-    #         # i=general_expr(i, pset, simplifying=True)
-    #         i = general_expr(i, pset, simplifying=False)
-    #         # print(i)
-    #         # print(i)
-    #         # pprint(i)
-    #     except NotImplementedError as e:
-    #         print(e)
-    # # c = time.time()
-    # # print(c - b, b - a, a - z)
-    # a, b, c = sympy.Symbol("a"), sympy.Symbol("b"), sympy.Symbol("c")
-    # print(sympy.simplify((a + (b + 1)) * c) == sympy.simplify(a * c + b * c + c))
+    population = [bl.PTree(bl.genFull()) for _ in range(30)]
+    pset = bl.cpset
+    for i in population:
+        # i.ppprint(bl.cpset)
+        # i = "exp(gx0/gx1)"
+
+        i = compile_context(i, pset.context, pset.gro_ter_con, simplify=False)
+        # print(i)
+        # print(i)
+        # fun = Coef("V", np.array([1.4,1.3]))
+        # i = fun(i)
+        # f = Function("MAdd")
+        # i = f(i)
+        try:
+            # group_str(i,pset)
+            # i=general_expr(i, pset, simplifying=True)
+            i = general_expr(i, pset, simplifying=False)
+            # print(i)
+            # print(i)
+            # pprint(i)
+        except NotImplementedError as e:
+            print(e)
+    # c = time.time()
+    # print(c - b, b - a, a - z)
+    a, b, c = sympy.Symbol("a"), sympy.Symbol("b"), sympy.Symbol("c")
+    print(sympy.simplify((a + (b + 1)) * c) == sympy.simplify(a * c + b * c + c))
```

### Comparing `BindingGP-0.0.36/bgp/functions/__init__.py` & `BindingGP-0.0.9/BGP/functions/__init__.py`

 * *Files identical despite different names*

### Comparing `BindingGP-0.0.36/bgp/functions/dimfunc.py` & `BindingGP-0.0.9/BGP/functions/dimfunc.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,30 +4,28 @@
 # @Time    : 2019/11/12 15:13
 # @Email   : 986798607@qq.com
 # @Software: PyCharm
 # @License: GNU Lesser General Public License v3.0
 
 """
 Notes:
-    These are some of parts coped from sympy.
+    this some of this part are a copy from sympy
 """
 
 from __future__ import division
 
 import numbers
-from functools import reduce
-from typing import Iterable
 
 import numpy as np
 import numpy.core.numeric as numeric
 import sympy
 from numpy.linalg import matrix_rank
 from sklearn.utils import check_array
 from sympy import Add, Mul, Pow, Tuple, sympify
-
+from sympy.core.compatibility import reduce, Iterable
 from sympy.physics.units import Dimension
 from sympy.physics.units.quantities import Quantity
 
 
 def dim_map():
     """expr to dim function """
 
@@ -101,50 +99,36 @@
             if dim == dless:
                 return dless.get_n(dim)
             else:
                 return dnan.get_n(dim)
         else:
             return dim
 
-    def my_der(dim1, dim2):
-
-        if isinstance(dim1, Dim):
-            return dim1.__div__(dim2)
-        elif isinstance(dim2, Dim):
-            return dim2.__rdiv__(dim1)
-
     my_log = my_ln = my_cos = my_sin = my_exp
 
-    my_funcs = {"Abs": my_abs, "exp": my_exp, "ln": my_ln, 'cos': my_cos, 'sin': my_sin, "log": my_log, "Der": my_der,
+    my_funcs = {"Abs": my_abs, "exp": my_exp, "ln": my_ln, 'cos': my_cos, 'sin': my_sin, "log": my_log,
                 'sqrt': my_sqrt, "MAdd": my_flat, "MMul": my_comp, "MSub": my_diff,
                 "MDiv": my_quot, "Self": my_self, "Conv": my_conv}
     return my_funcs
 
 
 class Dim(numeric.ndarray):
     """Redefine the Dimension of sympy, the default dimension SI system with 7 number.\n
     1.can be constructed by list of number.\n
     2.can be translated from a sympy.physics.unit. \n
-
-    Examples::
-
-        from sympy.physics.units import N
-        scale,dim = Dim.convert_to_Dim(N)
-
-    Examples::
-
-        dim=[1,0,1,0,1,0,0]
-        dim = Dim(dim)
-
-    Notes:
-        self.unit = [str(i) for i in SI._base_units]\n
-        self.unit_map = {'meter': "m", 'kilogram': "kg", 'second': "s",
-        'ampere': "A", 'mole': "mol", 'candela': "cd", 'kelvin': "K"}\n
-        self.dim = ['length', 'mass', 'time', 'current', 'amount_of_substance',
-        'luminous_intensity', 'temperature']
+        # >>>from sympy.physics.units import N
+        # >>>scale,dim = Dim.convert_to_Dim(N)
+        #inverse back
+    """
+    """
+    #     self.unit = [str(i) for i in SI._base_units]\n
+    #     self.unit_map = {'meter': "m", 'kilogram': "kg", 'second': "s",
+    #     'ampere': "A", 'mole': "mol", 'candela': "cd", 'kelvin': "K"}\n
+    #     self.dim = ['length', 'mass', 'time', 'current', 'amount_of_substance',
+    #     'luminous_intensity', 'temperature']
     """
 
     def __new__(cls, data):
 
         assert isinstance(data, (numeric.ndarray, (list, tuple)))
         dtype = np.float16
 
@@ -366,63 +350,68 @@
         d.unit = target_units
         return expr_scale_factor, d
 
     @classmethod
     def convert_to_Dim(cls, u, target_units=None, unit_system="SI"):
         """
         depend on sympy 1.5-1.6!!!
-
         Parameters
         ----------
-        u: sympy.physics.unit, Expr of sympy.physics.unit
+        u: sympy.physics.unit or Expr of sympy.physics.unit
             unit.
-        target_units: None, list of sympy.physics.unit
+        target_units: None or list of sympy.physics.unit
             if None, the target_units is 7 SI units
         unit_system: str
             default is unit_system="SI"
+            
+        Returns
+        -------
+        Expr
         """
         if isinstance(u, Dim):
             return 1, u
         else:
             expr_scale_factor, d = cls.convert_to(u, target_units=target_units, unit_system=unit_system)
             return expr_scale_factor, d
 
     @classmethod
     def convert_xi(cls, xi, ui, target_units=None, unit_system="SI"):
         """
         depend on sympy 1.5-1.6!!!
         Quick method. translate xi and ui to standard system.
-
         Parameters
+        
         ----------
         xi: np.ndarray
             xi
         ui: sympy.physics.unit or Expr of sympy.physics.unit
             unit
         target_units: None or list of sympy.physics.unit
             if None, the target_units is 7 SI units
         unit_system: str
             default is unit_system="SI"
 
         Returns
         -------
-        xi: np.ndarray
-
-        expr: Expr
+        xi: 
+            np.ndarray
+        
+        expr: 
+            Expr
         """
         expr_scale_factor, d = cls.convert_to_Dim(ui, target_units=target_units, unit_system=unit_system)
         xi = expr_scale_factor * xi
         if isinstance(xi, np.ndarray):
             xi = xi.astype(np.float32)
         return xi, d
 
     @classmethod
     def convert_x(cls, x, u, target_units=None, unit_system="SI"):
         """
-         depend on sympy 1.5-1.6!!!
+        depend on sympy 1.5-1.6!!!
          Quick method. translate x and u to standard system.
          
          Parameters
          ----------
          x: np.ndarray or list of ndarray,list of float,list of int
              x
          u: list of sympy.physics.unit or Expr of sympy.physics.unit
@@ -430,16 +419,19 @@
          target_units: None or list of sympy.physics.unit
              if None, the target_units is 7 SI units
          unit_system: str
              default is unit_system="SI"
 
          Returns
          -------
-         x: np.ndarray
-         expr: Expr
+         x: 
+             np.ndarray
+         
+         expr: 
+             Expr
          
          """
         if isinstance(x, list):
             pass
         elif isinstance(x, np.ndarray):
             x = x.T
         else:
@@ -450,31 +442,33 @@
         return x, x_dim
 
     @classmethod
     def inverse_convert(cls, dim, scale=1, target_units=None, unit_system="SI"):
         """
         depend on sympy 1.5-1.6!!!
         Quick method. Translate ui to other unit.
-
         Parameters
+        
         ----------
         dim: Dim
             dim
         scale: float
             scale generated before.
         target_units: None or list of sympy.physics.unit
             if None, the target_units is 7 SI units
         unit_system: str
             default is unit_system="SI"
 
         Returns
         -------
-        scale:float
-
-        expr: Expr
+        scale: 
+            float
+        
+        expr: 
+            Expr
         """
         from sympy.physics.units import UnitSystem
         unit_system = UnitSystem.get_unit_system(unit_system)
         if not target_units:
             target_units = unit_system._base_units
 
         if not isinstance(target_units, (Iterable, Tuple)):
@@ -497,33 +491,34 @@
         return sc, scale * tar * bas
 
     @classmethod
     def inverse_convert_xi(cls, xi, dim, scale=1, target_units=None, unit_system="SI"):
         """
         depend on sympy 1.5-1.6!!!
         Quick method. Translate xi, dim to other unit.
-
         Parameters
+        
         ----------
         xi:np.ndarray
             xi
         dim: Dim
             dim
         scale: float
             if xi is have been scaled, the scale is 1.
         target_units: None or list of sympy.physics.unit
             if None, the target_units is 7 SI units
         unit_system: str
             default is unit_system="SI"
 
         Returns
         -------
-        scale: float
-
-        expr: Expr
+        scale: 
+            float
+        expr: 
+            Expr
         """
         expr_scale_factor, d = cls.inverse_convert(dim, scale=scale, target_units=target_units, unit_system=unit_system)
         xi = expr_scale_factor * xi
         if isinstance(xi, np.ndarray):
             xi = xi.astype(np.float32)
         return expr_scale_factor * xi, d
```

### Comparing `BindingGP-0.0.36/bgp/functions/gsymfunc.py` & `BindingGP-0.0.9/BGP/functions/gsymfunc.py`

 * *Files 4% similar despite different names*

```diff
@@ -189,30 +189,12 @@
 
         if isinstance(x, (np.ndarray, NewArray)):
             result_list = [sympy.cos(i) for i in Flatten(x)]
             return NewArray(result_list, x.shape)
         else:
             return sympy.cos(x)
 
-    def my_der(self, other):
-        if isinstance(self, (np.ndarray, NewArray)):
-            if isinstance(other, (np.ndarray, NewArray)):
-                if self.shape != other.shape:
-                    raise ValueError("array shape mismatch")
-                else:
-                    result_list = [sympy.diff(i, j, evaluate=False) for i, j in zip(Flatten(self), Flatten(other))]
-                    return type(self)(result_list, self.shape)
-            else:
-                result_list = [sympy.diff(i, other, evaluate=False) for i in Flatten(self)]
-                return type(self)(result_list, self.shape)
-        else:
-            if isinstance(other, (np.ndarray, NewArray)):
-                result_list = [sympy.diff(self, i, evaluate=False) for i in Flatten(other)]
-                return type(self)(result_list, other.shape)
-            else:
-                return sympy.diff(self, other, evaluate=False)
-
     return {"MAdd": Flat, "MMul": Comp, "MSub": Diff, "MDiv": Quot, "Conv": Conv,
             "Self": lambda x_: x_,
-            "Abs": my_abs, "exp": my_exp, "ln": my_ln, 'cos': my_cos, 'sin': my_sin, "log": my_log, "Der": my_der,
+            "Abs": my_abs, "exp": my_exp, "ln": my_ln, 'cos': my_cos, 'sin': my_sin, "log": my_log,
             'sqrt': my_sqrt,
             }
```

### Comparing `BindingGP-0.0.36/bgp/functions/newfunc.py` & `BindingGP-0.0.9/BGP/functions/newfunc.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,26 +1,28 @@
 import numpy as np
 import sympy
+from BGP.functions.dimfunc import Dim
+from BGP.functions.gsymfunc import NewArray
 from sympy import Function
 
-from bgp.functions.dimfunc import Dim
-from bgp.functions.gsymfunc import NewArray
-
 
 def newfuncV(operation, arity=1, name="Fc"):
     """
 
     Parameters
     ----------
     operation:callable
-        the detail of operation only accept +,-,*,/,abs,-(negative),x^n.
+        the detail of opearation only accept +,-,*,/,abs,-(negative),x^n
     arity: int
-        the arity of operation.
+        the arity of opeaation
     name:str
-        name.
+        name
+    Returns
+    -------
+    dict
     """
     func = Function(name)
 
     def npf(*x):
         return operation(*x)
 
     def gsymf(*x):
```

### Comparing `BindingGP-0.0.36/bgp/functions/symfunc.py` & `BindingGP-0.0.9/BGP/functions/symfunc.py`

 * *Files 6% similar despite different names*

```diff
@@ -20,21 +20,19 @@
 
     def Sub(left, right):
         return left - right
 
     def rem(ax):
         return 1 - ax
 
-    der = Function("Der")
-
     functions1 = {"sin": sympy.sin, 'cos': sympy.cos, 'exp': sympy.exp, 'ln': sympy.ln, "log": sympy.ln,
                   'Abs': sympy.Abs, "Neg": functools.partial(sympy.Mul, -1.0),
                   "Rec": functools.partial(sympy.Pow, e=-1.0), "Self": lambda x: x,
                   "Rem": rem}
-    functions2 = {"Add": sympy.Add, 'Sub': Sub, 'Mul': sympy.Mul, 'Div': Div, "Der": der}
+    functions2 = {"Add": sympy.Add, 'Sub': Sub, 'Mul': sympy.Mul, 'Div': Div}
 
     return functions1, functions2
 
 
 def sym_dispose_map():
     """user's str to sympy.expr function"""
     Flat = Function("MAdd")
```

### Comparing `BindingGP-0.0.36/bgp/gp.py` & `BindingGP-0.0.9/BGP/gp.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,47 +4,46 @@
 # @Time    : 2019/11/12 15:13
 # @Email   : 986798607@qq.com
 # @Software: PyCharm
 # @License: GNU Lesser General Public License v3.0
 
 """
 Notes:
-    This part are one copy from deap,
-    change the random to numpy.random.
+    this part are one copy from deap,
+    change the random to numpy.random
 """
 
 import copy
 import operator
 import sys
 from collections import Counter
 from functools import wraps
 from inspect import isclass
 from operator import attrgetter
 
 import numpy as np
 from deap.tools import Statistics, MultiStatistics
+from BGP.calculation.scores import score_dim
 from numpy import random
 
-from bgp.calculation.scores import score_dim
-
 
 ######################################
 # Generate                         #
 ######################################
 
 
 def checkss(func):
     @wraps(func)
     def wrapper(*args, **kwargs):
         result = func(*args, **kwargs)
 
         pset = kwargs["pset"]
-        for i in result[0].top():
-            assert i in pset.dispose
         for i in result[0].bot():
+            assert i in pset.dispose
+        for i in result[0].top():
             assert i in pset.primitives + pset.terminals_and_constants
 
         return result
 
     return wrapper
 
 
@@ -64,15 +63,14 @@
         return result
 
     return wrapper
 
 
 def generate(pset, min_, max_, condition, personal_map=False, *kwargs):
     """
-    generate expression.
 
     Parameters
     ----------
     pset: SymbolSet
         pset
     min_: int
         Minimum height of the produced trees.
@@ -83,14 +81,17 @@
         the height of the tree to build and the current
         depth in the tree.
     kwargs: None
         placeholder for future
     personal_map:bool
         premap
 
+    Returns
+    -------
+
     """
     _ = kwargs
     type_ = object
     expr = []
     height = random.randint(min_, max_)
     stack = [(0, type_)]
     while len(stack) != 0:
@@ -166,15 +167,14 @@
         """
         return depth == height or (depth >= min_ and random.random() < pset.terminalRatio)
 
     return generate(pset, min_, max_, condition, personal_map=personal_map)
 
 
 def depart(individual):
-    """take part expression."""
     if len(individual) <= 10 or individual.height <= 8:
         return [individual, ]
     else:
         inds = []
         for index in np.arange(2, len(individual) - 4, step=2):
             slice_ = individual.searchSubtree(index)
             ind_new = individual.__class__(individual[slice_])
@@ -201,22 +201,14 @@
     def condition(height, depth):
         """Expression generation stops when the depth is equal to height."""
         return depth == height
 
     return generate(pset, min_, max_, condition, personal_map=personal_map)
 
 
-def genHalf(pset, min_, max_, personal_map=False):
-    a = random.rand()
-    if a > 0.5:
-        return genFull(pset, min_, max_, personal_map=personal_map)
-    else:
-        return genGrow(pset, min_, max_, personal_map=personal_map)
-
-
 ######################################
 # crossover                        #
 ######################################
 def cxOnePoint(ind10, ind20):
     """Randomly select crossover point in each individual and exchange each
     subtree with the point as root between each individual.
 
@@ -252,16 +244,19 @@
         @wraps(func)
         def wrapper(*args, **kwargs):
 
             keep_inds = [copy.deepcopy(ind) for ind in args]
             new_inds = list(func(*args, **kwargs))
             for i, ind in enumerate(new_inds):
 
-                if key(ind) > max_value:
+                if key(ind) == key(keep_inds[i]):
+                    pass
+                elif key(ind) > max_value:
                     new_inds[i] = keep_inds[random.choice(len(keep_inds))]
+
             return new_inds
 
         return wrapper
 
     return decorator
 
 
@@ -278,23 +273,20 @@
     :param individual: The tree to be mutated.
     :param expr: A function object that can generate an expression when
                  called.
     :param pset: SymbolSet
     :returns: A tuple of one tree.
 
     """
-    individual = copy.copy(individual)
-
     index = random.choice(len(individual))
     if index % 2 == 1:
         index -= 1
     slice_ = individual.searchSubtree(index)
 
     individual[slice_] = expr(pset=pset)
-
     return individual,
 
 
 # @logg
 # @checkss
 def mutShrink(individual, pset=None):
     """This operator shrinks the *individual* by choosing randomly a branch and
@@ -302,53 +294,52 @@
 
     :param individual: The tree to be shrinked.
     :param pset: SymbolSet.
     :returns: A tuple of one tree.
     """
     _ = pset
     # We don't want to "shrink" the root
-    if len(individual) < 4 or individual.height < 4:
+    if len(individual) < 4 or individual.height <= 4:
         return individual,
 
-    individual = copy.copy(individual)
     index = random.randint(0, len(individual))
 
     if index % 2 == 1:
         index -= 1
     slice_ = individual.searchSubtree(index)
 
     ter = [i for i in individual[slice_] if i.arity == 0]
     left = random.choice(ter)
     hat = random.choice(pset.dispose, p=pset.prob_dispose_list)
 
     del individual[slice_]
     individual.insert(index, left)
     individual.insert(index, hat)
+
     return individual,
 
 
 # @logg
 # @checkss
 def mutNodeReplacementVerbose(individual, pset, personal_map=False):
     """
-    choice terminals_and_constants verbose
+    # choice terminals_and_constants verbose
     Replaces a randomly chosen primitive from *individual* by a randomly
     chosen primitive with the same number of arguments from the :attr:`pset`
     attribute of the individual.
 
     :param individual: The normal or typed tree to be mutated.
     :param pset: SymbolSet
     :param personal_map: bool
     :returns: A tuple of one tree.
     """
 
     if len(individual) < 4:
         return individual,
 
-    individual = copy.copy(individual)
     if pset.types > 1:
         if random.random() <= 0.8:
             index = random.choice(np.arange(1, len(individual), step=2))
         else:
             index = random.choice(np.arange(0, len(individual), step=2))
     else:
         index = random.choice(np.arange(0, len(individual), step=2))
@@ -388,49 +379,46 @@
     return individual,
 
 
 # @logg
 # @checkss
 def mutDifferentReplacementVerbose(individual, pset, personal_map=False):
     """
-    choice terminals_and_constants verbose
+    # choice terminals_and_constants verbose
     Replaces a randomly chosen primitive from *individual* by a randomly
     chosen primitive with the same number of arguments from the :attr:`pset`
     attribute of the individual.
     decrease the probability of same terminals.
 
     :param individual: The normal or typed tree to be mutated.
     :param pset: SymbolSet
     :param personal_map: bool
 
     :returns: A tuple of one tree.
     """
-
     if len(individual) < 4:
         return individual,
-
-    individual = copy.copy(individual)
     ters = [repr(i) for i in individual.terminals()]
     pset_ters = [repr(i) for i in pset.terminals_and_constants]
     cou = Counter(ters)
-    cou_multil = {i: j for i, j in cou.items() if j >= 2}
-    ks = list(cou_multil.keys())
+    cou_mutil = {i: j for i, j in cou.items() if j >= 2}
+    ks = list(cou_mutil.keys())
     nks = list(set(pset_ters) - (set(ks)))
     if len(nks) <= 1:
         return individual,
 
     nks.sort()  # very import for random
 
     p_nks = np.array([pset.prob_ter_con[i] for i in nks])
     p_nks = p_nks.astype(float)
     p_nks /= np.sum(p_nks)
 
-    if cou_multil:
+    if cou_mutil:
         indexs = []
-        for k, v in cou_multil.items():
+        for k, v in cou_mutil.items():
             indi = []
             for i in np.arange(1, len(individual), 2):
                 if repr(individual[i]) == k:
                     indi.append(i)
             if indi:
                 indexs.append(random.choice(indi))
 
@@ -508,29 +496,31 @@
     return chosen
 
 
 @checks_number
 def selKbestDim(pop, K_best=10, dim_type=None, fuzzy=False, fit_attr="fitness", force_number=False):
     """
     Select the individual with dim limitation.
-
     Parameters
+    
     ----------
     pop: SymbolTree
         A list of individuals to select from.
     K_best:int
         The number of individuals to select.
     dim_type:Dim
     fuzzy:bool
         the dim or the dim with same base. such as m,m^2,m^3
     fit_attr:str
-        The attribute of individuals to use as selection criterion, default attr is "fitness".
-    force_number:False
-        return the number the same with K.
-
+        The attribute of individuals to use as selection criterion
+    force_number:
+        return the number the same with K
+    .. note::
+        default attr is "fitness"
+        
     Returns
     -------
     A list of selected individuals.
     """
     chosen = sorted(pop, key=operator.attrgetter(fit_attr))
     chosen.reverse()
 
@@ -570,17 +560,17 @@
         "dim_is_target": lambda ind: 1 if ind.dim_score else 0,
         # special
         "coef": lambda ind: score_dim(ind.y_dim, "coef", fuzzy=False),
         "integer": lambda ind: score_dim(ind.y_dim, "integer", fuzzy=False),
 
         "length": lambda ind: len(ind),
         "height": lambda ind: ind.height,
-        "h_bgp": lambda ind: ind.h_bgp,
+        "h_BGP": lambda ind: (ind.height - 1) / 2,
 
-        # multil-target
+        # mutil-target
         "weight_fitness": lambda ind: ind.fitness.wvalues,
         "weight_fitness_dim": lambda ind: ind.fitness.wvalues if ind.dim_score else -np.inf,
         # weight have mul the "-"
     }
 
     sa_all = {}
 
@@ -607,15 +597,15 @@
     return stats
 
 
 ######################################
 # shown                      #
 ######################################
 
-def _graph(expr):
+def graph(expr):
     """Construct the graph of a tree expression. The tree expression must be
     valid. It returns in order a node list, an edge list, and a dictionary of
     the per node labels. The node are represented by numbers, the edges are
     tuples connecting two nodes (number), and the labels are values of a
     dictionary for which keys are the node numbers.
 
     :param expr: A tree expression to convert into a graph.
@@ -698,57 +688,27 @@
         if random.random() < mutpb:
             offspring[i], = toolbox.mutate(offspring[i])
             del offspring[i].fitness.values
 
     return offspring
 
 
-def varAndfus(population, toolbox, cxpb, mutpb, fus, mutpb_list=1.0):
-    """
-
-    Parameters
-    ----------
-    population
-    toolbox
-    cxpb
-    mutpb
-    fus
-    mutpb_list:float,list,None
-
-    Returns
-    -------
-
-    """
+def varAndfus(population, toolbox, cxpb, mutpb, fus):
     offspring = copy.deepcopy(population)
 
     # Apply crossover and mutation on the offspring
     for i in range(1, len(offspring), 2):
         if random.random() < cxpb:
             offspring[i - 1], offspring[i] = toolbox.mate(offspring[i - 1],
                                                           offspring[i])
             del offspring[i - 1].fitness.values, offspring[i].fitness.values
 
-    if isinstance(mutpb_list, float) or mutpb_list is None:
-
-        mutpb /= len(fus)
-        for j in fus:
-            for i in range(len(offspring)):
-                if random.random() < mutpb:
-                    # print(random.random(), i)
-                    offspring[i], = j(offspring[i])
-                    del offspring[i].fitness.values
-    else:
-        assert len(fus) == len(mutpb_list)
-        mutpb_list = [i * mutpb for i in mutpb_list]
-
-        for j, m in zip(fus, mutpb_list):
-            for n, i in enumerate(offspring):
-
-                if random.random() < m:
-                    k, = j(i)
-                else:
-                    k = i
+    mutpb /= len(fus)
 
-                del k.fitness.values
-                offspring[n] = k
+    for j in fus:
+        for i in range(len(offspring)):
+            if random.random() < mutpb:
+                # print(random.random(), i)
+                offspring[i], = j(offspring[i])
+                del offspring[i].fitness.values
 
     return offspring
```

### Comparing `BindingGP-0.0.36/bgp/preprocess.py` & `BindingGP-0.0.9/BGP/preprocess.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import numpy as np
 from sklearn.base import TransformerMixin, BaseEstimator
 from sklearn.utils import check_array
 
 
-def _ger_magnitude(a):
+def ger_magnitude(a):
     c = 0
     if abs(a) > 1:
         while a >= 1:
             a /= 10
             c += 1
     elif 1 >= abs(a) > 0:
         while a <= 1:
@@ -15,15 +15,15 @@
             c += 1
         c = -c
 
     return c
 
 
 def _scale(a):
-    return 10 ** _ger_magnitude(a)
+    return 10 ** ger_magnitude(a)
 
 
 class MagnitudeTransformer(TransformerMixin, BaseEstimator):
     """
     Transform x, y or c to near to 1, and store the transform Magnitude.
     """
 
@@ -36,23 +36,22 @@
 
     def fit(self, X, y=None, group=2, apply=None, keep=None):
         """
 
         Parameters
         ----------
         X: np.ndarray
-
         y: np.ndarray
-
-        group: group index of x
-
+        group:group index of x
         apply: specific which index of x to transform
-
         keep: specific which index of x to not transform
 
+        Returns
+        -------
+
         """
 
         X = X.astype(np.float32)
         X = check_array(X, ensure_2d=True)
         n = X.shape[1]
         assert isinstance(X, np.ndarray)
         means = np.mean(X, axis=0)
```

### Comparing `BindingGP-0.0.36/bgp/probability/preference.py` & `BindingGP-0.0.9/BGP/probability/preference.py`

 * *Files 3% similar despite different names*

```diff
@@ -11,15 +11,14 @@
 
 import numpy as np
 from numpy import random
 from numpy.core import numeric
 
 
 class PreMap(numeric.ndarray):
-    """2D probability map"""
 
     def __new__(cls, data):
 
         assert isinstance(data, numeric.ndarray)
         dtype = np.float32
         arr = numeric.array(data, dtype=dtype, copy=True)
         shape = arr.shape
@@ -27,20 +26,19 @@
                                       buffer=arr,
                                       order='c')
         return ret
 
     @classmethod
     def from_shape(cls, shape):
         """
-        Generation.
 
         Parameters
         ----------
         shape:int
-            shape of premap.
+            shape of premap
 
         Returns
         -------
         PreMap
         """
         shape = (shape, shape)
         ret = numeric.ndarray.__new__(cls, shape, dtype=np.float16)
@@ -50,15 +48,15 @@
             ret[i, i] = 0.01 / shape[0]
         return cls(ret)
 
     def down_other_point(self, *sv):
 
         """
         Use for binding.rate the others and add the subbed value to the [index1,index2]
-        the rate are [0,1).
+        the rate are [0,1)
             
         Parameters
         ----------
         sv:[index1,index2,rate]
             site to set value
 
         """
@@ -108,19 +106,19 @@
         self[a, b] = c
         self[b, a] = c
 
     def set_ratio(self, *sv):
         """
         Rate the [index1,index2] to sum and add the subbed value to the others.
         under check.
-
         Parameters
+        
         ----------
         sv:[index1,index2,rate]
-            rate in [0,n), if [0,1) down, if [1,n) up.
+            rate in [0,n), if [0,1) down, if [1,n) up
         """
 
         a = sv[0]
         b = sv[1]
         c = sv[2]
         if c == 1:
             c -= 0.001
@@ -140,21 +138,21 @@
         self[a, b] = st
         self[b, a] = st
 
     def set_ratio_point(self, *sv):
         """
         Rate the [index1,index2] to self and add the subbed value to the others.
         under check.
-
         Parameters
+        
         ----------
-        sv:[index1,index2,rate]\n
-            in [0,n)\n
-            [0,1) down,\n
-            [1,n) up\n
+        sv:[index1,index2,rate]
+            [0,n)
+            [0,1) down,
+            [1,n) up
         """
 
         a = sv[0]
         b = sv[1]
         c = sv[2]
         if c == 1:
             c -= 0.00001
@@ -356,27 +354,27 @@
             prob = self.get_indexes_value(indexes, weight=weight)
         else:
             prob = None
         return prob
 
 # if __name__ == "__main__":
 #    # import copy
-#    # from bgp.gp import mutNodeReplacementVerbose, mutDifferentReplacementVerbose
+#    # from BGP.gp import mutNodeReplacementVerbose, mutDifferentReplacementVerbose
 #    # from numpy import random
-#    # from sklearn.datasets import fetch_california_housing
+#    # from sklearn.datasets import load_boston
 #    #
-#    # from bgp.base import SymbolSet
-#    # from bgp.base import SymbolTree
-#    # from bgp.dim import dless, Dim
+#    # from BGP.base import SymbolSet
+#    # from BGP.base import SymbolTree
+#    # from BGP.dim import dless, Dim
 #    #
 #    # random.seed(3)
 #    # # data
-#    # data = fetch_california_housing()
-#    # x = data["data"][:100]
-#    # y = data["target"][:100]
+#    # data = load_boston()
+#    # x = data["data"]
+#    # y = data["target"]
 #    # c = [6, 3, 4]
 #    # # unit
 #    # from sympy.physics.units import kg
 #    #
 #    # x_u = [kg] * 13
 #    # y_u = kg
 #    # c_u = [dless, dless, dless]
```

### Comparing `BindingGP-0.0.36/bgp/skflow.py` & `BindingGP-0.0.9/BGP/skflow.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,312 +1,225 @@
+from BGP import flow
+from BGP.base import SymbolSet
+from BGP.calculation.scores import calculate_y_unpack
+from BGP.calculation.translate import general_expr
+from BGP.flow import MutilMutateLoop
 from sklearn.base import BaseEstimator, TransformerMixin, MultiOutputMixin
 from sklearn.metrics import check_scoring
 
-from bgp import flow
-from bgp.base import SymbolSet
-from bgp.calculation.scores import calculate_y_unpack
-from bgp.calculation.translate import general_expr
-from bgp.flow import MultiMutateLoop
-
 
 class SymbolLearning(BaseEstimator, MultiOutputMixin, TransformerMixin):
-    """
-    One simplify Guide for flow.
-
-    1. The SymbolLearning is time-costing and not suit for ``GridSearchCV``,
-    the cross_validate are embedded.
-
-    2. For the classification problems, please using ``classification`` =True,
-    and set the suit classification metrics for ``scoring`` and ``score_pen`` carefully.
-
-    `Web of Symbolic Learning <https://bgp.readthedocs.io/en/latest/src/bgp.html#bgp.skflow.SymbolLearning>`_ .
-
-    See Also:
-        :class:`bgp.flow.BaseLoop`
-
-    """
+    """One simplify API for flow.\n
+    The detailed functions should turn to the loop of BGP.flow.\n
+    The SymbolLearning is time costing and are not suit for GridSearchCV, the cross_validate are builtin """
 
     def __str__(self):
         return str(self.loop)
 
     def __init__(self, loop, *args, **kwargs):
         """
-
         Parameters
         ----------
-        loop: str, None
-            bgp.flow.BaseLoop or ['BaseLoop', 'MultiMutateLoop', 'OnePointMutateLoop', 'DimForceLoop' ...].
-        pop: int
-            number of population.
-        gen: int
-            number of generation.
+        pset:SymbolSet
+            the feature x and traget y and others should have been added.
+        loop: str,None
+            BGP.flow.BaseLoop
+            [“BaseLoop”,”MutilMutateLoop“,“OnePointMutateLoop”, ”DimForceLoop“...]
+        pop:int
+            number of popolation
+        gen:int
+            number of generation
         mutate_prob:float
-            probability of mutate.
+            probability of mutate
         mate_prob:float
-            probability of mate(crossover).
+            probability of mate(crossover)
         initial_max:int
             max initial size of expression when first producing.
         initial_min : None,int
-            min initial size of expression when first producing.
+            max initial size of expression when first producing.
         max_value:int
-            max size of expression.
+            max size of expression
         hall:int,>=1
-            number of HallOfFame (elite) to maintain.
+            number of HallOfFame(elite) to maintain
         re_hall:None or int>=2
-            Notes: only valid when hall
+            Notes: only vaild when hall
             number of HallOfFame to add to next generation.
         re_Tree: int
             number of new features to add to next generation.
             0 is false to add.
         personal_map:bool or "auto"
-            "auto" is using 'premap' and with auto refresh the 'premap' with individual.\n
-            True is just using constant 'premap'.\n
+            "auto" is using premap and with auto refresh the premap with individual.\n
+            True is just using constant premap.\n
             False is just use the prob of terminals.
-        scoring: list of Callable, default is [sklearn.metrics.r2_score,]
-            See Also ``sklearn.metrics``
-            See Also ``bgp.calculation.scores.score_collection``.
+        scoring: list of Callbale, default is [sklearn.metrics.r2_score,]
+            See Also sklearn.metrics
         score_pen: tuple of  1, -1 or float but 0.
-            >0 : max problem, best is positive, worst is -np.inf.
-            <0 : min problem, best is negative, worst is np.inf.
-
+            >0 : max problem, best is positive, worse -np.inf
+            <0 : min problem, best is negative, worse np.inf
             Notes:
-            if multiply score method, the scores must turn to same dimension in prepossessing,
+            if multiply score method, the scores must be turn to same dimension in preprocessing
             or weight by score_pen. Because the all the selection are stand on the mean(w_i*score_i)
-
-            Examples::
-
-                scoring = [r2_score,]
-                score_pen= [1,]
-
+            Examples: [r2_score] is [1],
         cv:sklearn.model_selection._split._BaseKFold,int
-            default=1 means no cv. (the shuffler must be False)
+            the shuffler must be False,
+            default=1 means no cv
         filter_warning:bool
-            filter warning or not.
+            filter warning or not
         add_coef:bool
             add coef in expression or not.
         inter_add：bool
-            add intercept constant or not.
+            add intercept constant or not
         inner_add:bool
-            add inner coefficients or not.
+            add inner coeffcients or not
         out_add:bool
-            add out coefficients or not.
+            add out coeffcients or not
         flat_add:bool
-            add flat coefficients or not.
+            add flat coeffcients or not
         n_jobs:int
-            default 1, advise 6.
+            default 1, advise 6
         batch_size:int
-            default 40, depend on machine.
+            default 40, depend of machine
         random_state:int
-            None,int.
+            None,int
         cal_dim:bool
-            escape the dim calculation.
+            excape the dim calculation
         dim_type:Dim or None or list of Dim
-            "coef": af(x)+b. a,b have dimension,f(x)'s dimension is not dnan. \n
-            "integer": af(x)+b. f(x) is with integer dimension. \n
-            [Dim1,Dim2]: f(x)'s dimension in list. \n
+            "coef": af(x)+b. a,b have dimension,f(x) is not dnan. \n
+            "integer": af(x)+b. f(x) is interger dimension. \n
+            [Dim1,Dim2]: f(x) in list. \n
             Dim: f(x) ~= Dim. (see fuzzy) \n
             Dim: f(x) == Dim. \n
             None: f(x) == pset.y_dim
         fuzzy:bool
-            choose the dim with same base with dim_type, such as m,m^2,m^3.
+            choose the dim with same base with dim_type,such as m,m^2,m^3.
         stats:dict
             details of logbook to show. \n
             Map:\n
             values
                 = {"max": np.max, "mean": np.mean, "min": np.mean, "std": np.std, "sum": np.sum}
             keys
                 = {\n
                    "fitness": just see fitness[0], \n
                    "fitness_dim_max": max problem, see fitness with demand dim,\n
                    "fitness_dim_min": min problem, see fitness with demand dim,\n
                    "dim_is_target": demand dim,\n
-                   "coef":  dim is True, coef have dim, \n
+                   "coef":  dim is true, coef have dim, \n
                    "integer":  dim is integer, \n
                    ...
                    }
-
-            if stats is None, default is :
-
-            for cal_dim=True:
-                stats = {"fitness_dim_max": ("max",), "dim_is_target": ("sum",)}
-
-            for cal_dim=False:
-                stats = {"fitness": ("max",)}
-
-            if self-definition, the key is func to get attribute of each ind.
-
-            Examples::
-
-                def func(ind):
+            if stats is None, default is :\n
+                stats = {"fitness_dim_max": ("max",), "dim_is_target": ("sum",)}   for cal_dim=True
+                stats = {"fitness": ("max",)}                                      for cal_dim=False
+            if self-definition, the key is func to get attribute of each ind./n
+            Examples:
+                def func(ind):\n
                     return ind.fitness[0]
-                stats = { func: ("mean",), "dim_is_target":("sum",)}
-
+                stats = {func: ("mean",), "dim_is_target": ("sum",)}
         verbose:bool
-            print verbose logbook or not.
+            print verbose logbook or not
         tq:bool
-            print progress bar or not.
+            print progress bar or not
         store:bool or path
-            bool or path.
-        stop_condition:callable, float
-            stop condition on the best individual of hall, which return bool,the true means stop loop.
-
-            Examples::
-
-                def func(ind):
+            bool or path
+        stop_condition:callable
+            stop condition on the best ind of hall, which return bool,the true means stop loop.
+            Examples:
+                def func(ind):\n
                     c = ind.fitness.values[0]>=0.90
                     return c
-
-        pset:SymbolSet
-            the feature x and target y and others should have been added.
-        details:bool
-            return expr and predict_y or not.
-        classification: bool
-            classification or not.
         """
-
         self.args = args
         self.kwargs = kwargs
         if loop is None:
-            loop = MultiMutateLoop
+            loop = MutilMutateLoop
         if isinstance(loop, str):
             loop = getattr(flow, loop)
 
         self.loop = loop
 
     def fit(self, X=None, y=None, c=None, x_group=None, x_dim=1, y_dim=1, c_dim=1, x_prob=None,
-            c_prob=None, pset=None, power_categories=(2, 3, 0.5),
-            categories=("Add", "Mul", "Sub", "Div"),
-            warm_start=False, new_gen=None):
+            c_prob=None, pset=None, power_categories=(2, 3, 0.5), categories=("Add", "Mul", "Sub", "Div")):
         """
-        Method 1. fit with x, y.
 
-        Examples::
-
-            sl = SymbolLearning()
-            sl.fit(x,y,...)
-
-        Method 2. fit with customized pset. If you need more self-definition, use one defined SymbolSet object to ``pset``.
-
-        Examples::
-
-            pset = SymbolSet()
-            pset.add_features_and_constants(...)
-            pset.add_operations(...)
-            ...
-            sl = SymbolLearning()
-            sl.fit(pset=pset)
+        If need more self-definition, use one defined SymbolSet object to pset.\n
+        Examples:
+            pset = SymbolSet()\n
+            pset.add_features_and_constants(...)\n
+            pset.add_operations(...)\n
+            ...\n
+            ...SymbolLearning().fit(pset=pset)\n
 
         Parameters
         ----------
         X:np.ndarray
-            data.
+
         y:np.ndarray
-            y.
+
         c:list of float, None
-            constants.
+
         x_dim: 1 or list of Dim
-            the same size wih x.shape[1], default 1 is dless for all x.
-        y_dim: 1, Dim
-            Dim of y.
+            the same size wih x.shape[1], default 1 is dless for all x
+        y_dim: 1,Dim
+            dim of y
         c_dim: 1,list of Dim
-            the same size wih c.shape, default 1 is dless for all c.
+            the same size wih c.shape, default 1 is dless for all c
 
         x_prob: None,list of float
-            the same size wih x.shape[1].
+            the same size wih x.shape[1]
         c_prob: None,list of float
-            the same size wih c.
+            the same size wih c
         x_group:list of list
-            Group of x.
-
-            Examples:
-
-                x_group=[[1,2],]
-                or
-                x_group=2
-
-            See Also :py:func:`bgp.base.SymbolSet.add_features`
-
+            Group of x.\n
+            See Also pset.add_features_and_constants
         power_categories: Sized,tuple, None
             Examples:(0.5,2,3)
         categories: tuple of str
             map table:
                     {"Add": sympy.Add, 'Sub': Sub, 'Mul': sympy.Mul, 'Div': Div}
+
                     {"sin": sympy.sin, 'cos': sympy.cos, 'exp': sympy.exp, 'ln': sympy.ln,
+
                     {'Abs': sympy.Abs, "Neg": functools.partial(sympy.Mul, -1.0),
+
                     "Rec": functools.partial(sympy.Pow, e=-1.0)}
 
                     Others:  \n
                     "Rem":  f(x)=1-x,if x true \n
                     "Self":  f(x)=x,if x true \n
 
         pset:SymbolSet
-            See Also SymbolSet.
-        warm_start: bool
-            warm start or not.
-
-            Note:
-                If you offer pset in advance by user, please check carefully the feature numbers,especially when use ``re_Tree``.
-                because the new features are add.
-            Reference:
-                CalculatePrecisionSet.update_with_X_y.
-        new_gen: None,int
-            warm_start generation.
+            See Also SymbolSet
 
-        """
 
+        """
         # try to find pest form args,kwargs
         psets = [i for i in self.args if isinstance(i, SymbolSet)]
         if len(psets) > 0:
             self.args.remove(psets[0])
         if "pset" in self.kwargs:
             psets.append(self.kwargs["pset"])
             del self.kwargs["pset"]
 
         if pset is None:
             if len(psets) > 0:
                 pset = psets[0]
 
         if pset is None:
             # one simple pset are generate with no dimension calculation, But just with x_group.\n
-
             if X is not None and y is not None:
                 pset = SymbolSet()
                 pset.add_features_and_constants(X, y, c, x_dim=x_dim, y_dim=y_dim, c_dim=c_dim, x_prob=x_prob,
                                                 c_prob=c_prob, x_group=x_group, feature_name=None)
                 pset.add_operations(power_categories=power_categories,
                                     categories=categories)
-
-            elif hasattr(self.loop, "gen"):
-                pass
-            else:
-                raise ValueError("The pset should be defined or the X and Y should be offered.")
-        ####################################
-
-        if warm_start:
-            assert hasattr(self.loop, "gen"), "Before the warm_start, Need fit at least one time"
-            if X is not None and y is not None:
-                self.loop.cpset.update_with_X_y(X, y)
-            elif pset:
-                # the warm_start are not compacting with "re_Tree"
-                self.loop.cpset.update(pset)
             else:
                 raise ValueError("The pset should be defined or the X and Y should be offered.")
 
-            self.loop.re_fresh_by_name()
-
-            hall = self.loop.run(warm_start=True, new_gen=new_gen)
-        else:
-            if hasattr(self.loop, "gen"):
-                loops = self.loop.__class__
-                self.loop = loops(pset, *self.args, **self.kwargs)
-            else:
-                self.loop = self.loop(pset, *self.args, **self.kwargs)
-
-            hall = self.loop.run()
-
+        self.loop = self.loop(pset, *self.args, **self.kwargs)
+        hall = self.loop.run()
         self.best_one = hall.items[0]
         try:
             expr = general_expr(self.best_one.coef_expr, self.loop.cpset)
             self.expr_type = "single"
         except (RecursionError, RuntimeWarning):
             expr = self.best_one.coef_expr
             self.expr_type = "group"
@@ -336,85 +249,52 @@
         se = cpset_new.replace(X)
 
         res = se.calculate_score(self.expr)
         score, expr01, pre_y = res
         return pre_y
 
     def predict(self, X):
-        """
-        predict y from X.
-
-        Parameters
-        ----------
-        X: np.ndarray
-            data.
-
-        """
         if self.expr_type == "group":
             return self._predict_by_group(X)
         else:
             return self._predict_by_single(X)
 
     def score(self, X, y, scoring):
-        """
-        score
-
-        Parameters
-        ----------
-        X: np.ndarray
-            data.
-        y: np.ndarray
-            true y.
-        scoring: str
-            scoring method,default is "r2"
 
-        """
         scoring = check_scoring(self, scoring=scoring)
 
         if not isinstance(scoring, (list, tuple)):
             scoring = [scoring, ]
         try:
             sc_all = []
             for si in scoring:
                 sc = si(self, X, y)
                 sc_all.append(sc)
 
-        # except (ValueError, RuntimeWarning):
-        except RuntimeWarning:
+        except (ValueError, RuntimeWarning):
 
             sc_all = None
 
         return sc_all
 
-    def cv_result(self, refit=False):
-        """
-        return the cv_result best expression.
-        Only valid when ``cv`` !=1.
-
-        Parameters
-        ----------
-        refit: bool
-            re-fit the data or not. If true, use all the data on the best expression.
-        """
-
+    def cv_result(self, refit=True):
         if self.loop.cpset.cv != 1:
             self.loop.cpset.refit = refit
             return self.loop.cpset.calculate_cv_score(self.best_one.expr)
         else:
             return None
 
 
 if __name__ == "__main__":
     # data
-    from sklearn.datasets import fetch_california_housing
+    from sklearn.datasets import load_boston
 
-    data = fetch_california_housing()
-    x = data["data"][:100]
-    y = data["target"][:100]
+    data = load_boston()
+    x = data["data"]
+    y = data["target"]
     c = [6, 3, 4]
 
-    sl = SymbolLearning(loop=None, pop=50, gen=3, cal_dim=False, re_hall=2, add_coef=True, cv=1, random_state=2,
-                        re_Tree=0, details=True, store=r"/data/home/wangchangxin")
-    sl.fit(x, y, c=c)
-    # sl.fit(x, y, c=c, x_group=[[1, 3], [0, 2], [4, 7]], warm_start=True)
-    # score = sl.score(x, y, "r2")
-    # print(sl.expr)
+    sl = SymbolLearning(loop=None, pop=50, gen=3, cal_dim=True, re_hall=2, add_coef=True, cv=2, random_state=1,store = r"/data/home/wangchangxin"
+                        )
+    sl.fit(x, y, c=c, x_group=[[1, 3], [0, 2], [4, 7]])
+    score = sl.score(x, y, "r2")
+    print(sl.expr)
```

### Comparing `BindingGP-0.0.36/setup.py` & `BindingGP-0.0.9/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,26 +13,26 @@
 this_directory = path.abspath(path.dirname(__file__))
 with open(path.join(this_directory, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
 
     name='BindingGP',
-    version='0.0.36',
+    version='0.0.09',
     keywords=['symbolic regression'],
     description='This is for symbolic regression.'
                 'Some of code are non-originality, just copy for use. All the referenced code are marked,'
                 'details can be shown in their sources',
     install_requires=['pandas', 'numpy', 'sympy>=1.5.1', 'scipy', 'scikit-learn', 'joblib',
-                      'requests', 'tqdm', 'six', 'deap>=1.2', "mgetool"],
+                      'requests', 'tqdm', 'six', 'deap>=1.2', "mgetool", "featurebox>=0.0.850"],
     include_package_data=True,
     author='wangchangxin',
     author_email='986798607@qq.com',
     python_requires='>=3.6',
-    url='https://github.com/boliqq07/bgp',
+    url='https://github.com/boliqq07/gvp',
     maintainer='wangchangxin',
     platforms=[
         "Windows",
         "Unix",
     ],
     classifiers=[
         "Development Status :: 4 - Beta",
@@ -40,15 +40,14 @@
         "License :: OSI Approved :: GNU General Public License v3 (GPLv3)",
         "Natural Language :: English",
         "Operating System :: Microsoft :: Windows",
         "Operating System :: Unix",
         "Programming Language :: Python :: 3.6",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
-        "Programming Language :: Python :: 3.9",
     ],
 
     packages=find_packages(
-        exclude=["*.tests", "*.tests.*", "tests.*", "tests", "tests", 'deprecated', "SUM", "Instances", "docs"], ),
+        exclude=["*.tests", "*.tests.*", "tests.*", "tests", "tests", 'deprecated', "SUM", "Instances"], ),
     long_description=long_description,
     long_description_content_type='text/markdown'
 )
```

### Comparing `BindingGP-0.0.36/test/test2.py` & `BindingGP-0.0.9/test/test_score.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,71 +1,81 @@
-# -*- coding: utf-8 -*-
-import sympy
+import time
 
-from bgp.postprocess import pprint
-# @Time    : 2020/12/17 17:29
-# @Email   : 986798607@qq.com
-# @Software: PyCharm
-# @License: BSD 3-Clause
-from mgetool.tool import tt
+from numpy import random
+from sklearn.datasets import load_boston
+
+from BGP.base import SymbolSet, SymbolTree, CalculatePrecisionSet
+from BGP.calculation.scores import calculate_y
+from BGP.calculation.translate import compile_context
+from BGP.functions.dimfunc import dless, Dim
+from BGP.functions.npfunc import np_map
 
 if __name__ == "__main__":
-    from sklearn.datasets import load_iris, fetch_california_housing
-    from bgp.skflow import SymbolLearning
-    from sklearn import metrics
-    from sklearn.utils import shuffle
-
-    # data = load_iris()
-    data = fetch_california_housing()
-    x = data["data"][:100]
-    y = data["target"][:100]
-    c = [1, 2, 3]
-
-    #    data = pd.read_csv(r"..data/a.csv")
-    #    y = data[:,0]
-    #    x = data[:,1:]
-
-    sl = SymbolLearning(loop="MultiMutateLoop", pop=500,
-                        re_hall=3,
-                        gen=5, random_state=1,
-                        # classification=True,
-                        classification=False,
-                        # scoring=[metrics.accuracy_score, ], score_pen=[1, ],
-                        # store=False,
-                        store=True,
-                        n_jobs=4,
-
-                        batch_size=10,
-                        batch_para=False,
-
-                        # add_coef=False,
-                        # out_add =True,
-                        # vector_add=True,
-                        )
-    tt.t
-    sl.fit(x, y, c=c,categories=("Mul", "Sub", "exp", "ln")
-           # x_group=[[0, 1], [2, 3]]
-           )
-    tt.t
-    tt.p
-    # score = sl.score(x, y, "r2")
-    top_n = sl.loop.top_n(10)
-    pprint(top_n["expr"].values[4])
-
-    # print(sl.expr)
-
-    # top_n.to_csv(r"./re.csv")
-
-# if __name__ == "__main__":
-#     from sklearn.datasets import fetch_california_housing
-#     from bgp.skflow import SymbolLearning
-#
-#     data = fetch_california_housing()
-#     x = data["data"][:100]
-#     y = data["target"][:100]
-#     c = [1, 2, 3]
-#
-#     sl = SymbolLearning(loop="MultiMutateLoop", pop=500, gen=3, cal_dim=True, re_hall=2, add_coef=True, cv=1, random_state=1
-#                 )
-#     sl.fit(x, y, c=c,x_group=[[1, 3], [0, 2], [4, 7]])
-#     score = sl.score(x, y, "r2")
-#     print(sl.expr)
+    # data
+    data = load_boston()
+    x = data["data"]
+    y = data["target"]
+    c = [6, 3, 4]
+    # unit
+    from sympy.physics.units import kg
+
+    x_u = [kg] * 13
+    y_u = kg
+    c_u = [dless, dless, dless]
+
+    x, x_dim = Dim.convert_x(x, x_u, target_units=None, unit_system="SI")
+    y, y_dim = Dim.convert_xi(y, y_u)
+    c, c_dim = Dim.convert_x(c, c_u)
+
+    t = time.time()
+
+    # symbolset
+    pset0 = SymbolSet()
+    pset0.add_features(x, y, x_dim=x_dim, y_dim=y_dim, x_group=[[1, 2], [3, 4, 5], [6, 7]],
+                       feature_name=["Ss%i" % i for i in range(13)])
+    pset0.add_constants(c, c_dim=c_dim, c_prob=None)
+    pset0.add_operations(power_categories=(2, 3, 0.5),
+                         categories=("Add", "Mul", "Sub", "Div", "ln"),
+                         self_categories=None)
+
+    random.seed(2)
+    z = time.time()
+    sl = [SymbolTree.genGrow(pset0, 3, 4) for _ in range(500)]
+    a = time.time()
+    # sli =" MAdd(Sub(Add(Mul(x0, gx1), exp(x10)), Mul(Conv(Add(x0, gx0)), Mul(x6, MAdd(x10)))))"
+    # sl =["MAdd(gx1 * x11 * (-x0 + x11) * MAdd(gx1))"]
+
+    # sl = [compile_context(sli, pset0.context, pset0.gro_ter_con) for sli in sl]
+    # sl = [simple(sli.args[0], pset0.gro_ter_con) for sli in sl if len(sli.args)>0]
+    c = 1
+    a = time.time()
+    pset0 = CalculatePrecisionSet(pset0, scoring=None, score_pen=(1,), filter_warning=True, cal_dim=False,
+                                  dim_type=None,
+                                  fuzzy=False, add_coef=False, inter_add=True,
+                                  inner_add=False, n_jobs=1, batch_size=20,
+                                  tq=True)
+    from sys import getsizeof
+
+    T100 = getsizeof(sl)
+    psize = getsizeof(pset0)
+    # print(T100,psize)
+    for i in sl:
+        b = time.time()
+        i0 = compile_context(i, pset0.context, pset0.gro_ter_con)
+        r2 = time.time()
+        # pprint(i0,pset0)
+        calculate_y(i0, pset0.data_x, pset0.y, pset0.terminals_and_constants_repr, add_coef=True,
+                    filter_warning=True, inter_add=True, inner_add=True, np_maps=np_map())
+        # i = pset0.calculate_detail(i)
+        # j = simple(i.coef_expr, pset0.gro_ter_con)
+        # print(i)
+        # print(repr(i))
+        # print(i0)
+        # ppprint(i, pset0, feature_name=True)
+        if y[0] is None:
+            c = c + 1
+
+        r3 = time.time()
+    #     print(r2 - b, "com")
+    #     print(r3-r2,"cal")
+    # e = time.time()
+    # print(e-a)
```

### Comparing `BindingGP-0.0.36/test/test_dim.py` & `BindingGP-0.0.9/test/test_dim.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import unittest
 
 import numpy as np
 
-from bgp.functions.dimfunc import Dim, dless, dnan, dim_map
+from BGP.functions.dimfunc import Dim, dless, dnan, dim_map
 
 
 class MyTestCase(unittest.TestCase):
     def setUp(self):
         self.a = Dim([1, 2, 3, 4, 5, 6, 7])
         self.b = Dim([2, 2, 3, 4, 5, 6, 7])
```

### Comparing `BindingGP-0.0.36/test/test_function.py` & `BindingGP-0.0.9/test/test_function.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import unittest
 
 import sympy
 from sympy.core.numbers import nan
 from sympy.core.numbers import oo as Inf
 
-from bgp.functions.gsymfunc import NewArray
-from bgp.functions.gsymfunc import gsym_map as sym_map
+from BGP.functions.gsymfunc import NewArray
+from BGP.functions.gsymfunc import gsym_map as sym_map
 
 
 class MyTestCase(unittest.TestCase):
     def setUp(self):
         self.a = sympy.Symbol("a") * sympy.Symbol("a")
         self.nan = nan
         self.n = NewArray([1.0, 1, Inf])
```

### Comparing `BindingGP-0.0.36/test/test_preference.py` & `BindingGP-0.0.9/test/test_preference.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import unittest
 
 import numpy as np
 
-from bgp.probability.preference import PreMap
+from BGP.probability.preference import PreMap
 
 
 class MyTestCase(unittest.TestCase):
     def setUp(self):
         self.premap = PreMap.from_shape(14)
 
     def test_down_self(self):
```

### Comparing `BindingGP-0.0.36/test/test_score.py` & `BindingGP-0.0.9/test/test_translate.py`

 * *Files 21% similar despite different names*

```diff
@@ -1,81 +1,58 @@
 import time
 
-from numpy import random
-from sklearn.datasets import fetch_california_housing
+from sklearn import preprocessing
+from sklearn.datasets import load_boston
 
-from bgp.base import SymbolSet, SymbolTree, CalculatePrecisionSet
-from bgp.calculation.scores import calculate_y
-from bgp.calculation.translate import compile_context
-from bgp.functions.dimfunc import dless, Dim
-from bgp.functions.npfunc import np_map
+from BGP.base import SymbolSet, SymbolTree, CalculatePrecisionSet
+from BGP.calculation.coefficient import try_add_coef
+from BGP.calculation.translate import general_expr, compile_context
+from BGP.functions.dimfunc import dless, Dim
+from BGP.functions.npfunc import np_map
 
 if __name__ == "__main__":
     # data
-    data = fetch_california_housing()
-    x = data["data"][:100,:8]
-    y = data["target"][:100]
+    data = load_boston()
+    x = data["data"]
+    y = data["target"]
     c = [6, 3, 4]
     # unit
     from sympy.physics.units import kg
 
     x_u = [kg] * 13
     y_u = kg
     c_u = [dless, dless, dless]
 
     x, x_dim = Dim.convert_x(x, x_u, target_units=None, unit_system="SI")
     y, y_dim = Dim.convert_xi(y, y_u)
     c, c_dim = Dim.convert_x(c, c_u)
 
+    sc = preprocessing.MinMaxScaler((1, 2))
+    x = sc.fit_transform(x)
     t = time.time()
 
     # symbolset
     pset0 = SymbolSet()
-    pset0.add_features(x, y, x_dim=x_dim, y_dim=y_dim, x_group=[[1, 2], [3, 4, 5], [6, 7]],
-                       feature_name=["Ss%i" % i for i in range(8)])
+    pset0.add_features(x, y, x_dim=x_dim, y_dim=y_dim, x_group=2,
+                       feature_name=["Ss%i" % i for i in range(13)])
     pset0.add_constants(c, c_dim=c_dim, c_prob=None)
-    pset0.add_operations(power_categories=(2, 3, 0.5),
-                         categories=("Add", "Mul", "Sub", "Div", "ln"),
+    pset0.add_operations(power_categories=(2, 3, 4),
+                         categories=("Add", "Mul", "Sub", "Div", "ln", "exp"),
                          self_categories=None)
 
-    random.seed(2)
-    z = time.time()
-    sl = [SymbolTree.genGrow(pset0, 3, 4) for _ in range(50)]
-    a = time.time()
-    # sli =" MAdd(Sub(Add(Mul(x0, gx1), exp(x10)), Mul(Conv(Add(x0, gx0)), Mul(x6, MAdd(x10)))))"
-    # sl =["MAdd(gx1 * x11 * (-x0 + x11) * MAdd(gx1))"]
-
-    # sl = [compile_context(sli, pset0.context, pset0.gro_ter_con) for sli in sl]
-    # sl = [simple(sli.args[0], pset0.gro_ter_con) for sli in sl if len(sli.args)>0]
-    c = 1
-    a = time.time()
     pset0 = CalculatePrecisionSet(pset0, scoring=None, score_pen=(1,), filter_warning=True, cal_dim=False,
                                   dim_type=None,
                                   fuzzy=False, add_coef=False, inter_add=True,
                                   inner_add=False, n_jobs=1, batch_size=20,
                                   tq=True)
-    from sys import getsizeof
+    sl = [SymbolTree.genGrow(pset0, 3, 4) for _ in range(50)]
+    sll = [compile_context(o, pset0.context, pset0.gro_ter_con, simplify=True) for o in sl]
 
-    T100 = getsizeof(sl)
-    psize = getsizeof(pset0)
-    # print(T100,psize)
-    for i in sl:
-        b = time.time()
-        i0 = compile_context(i, pset0.context, pset0.gro_ter_con)
-        r2 = time.time()
-        # pprint(i0,pset0)
-        calculate_y(i0, pset0.data_x, pset0.y, pset0.terminals_and_constants_repr, add_coef=True,
-                    filter_warning=True, inter_add=True, inner_add=True, np_maps=np_map())
-        # i = pset0.calculate_detail(i)
-        # j = simple(i.coef_expr, pset0.gro_ter_con)
-        # print(i)
-        # print(repr(i))
-        # print(i0)
-        # ppprint(i, pset0, feature_name=True)
-        if y[0] is None:
-            c = c + 1
-
-        r3 = time.time()
-        print(r2 - b, "com")
-        print(r3-r2,"cal")
-    e = time.time()
-    print(e-a)
+    slll = [try_add_coef(i, pset0.data_x, pset0.y, pset0.terminals_and_constants_repr,
+                         filter_warning=True, inter_add=True, inner_add=False, vector_add=True, np_maps=np_map())[1]
+            for i in sll]
+    sllll = [general_expr(o, pset0, simplifying=False) for o in slll]
+    # tree="MSub(exp(gx5))"
+    # sll = compile_context(tree, pset0.context, pset0.gro_ter_con, simplify=True)
+    # slll = try_add_coef(sll, pset0.data_x, pset0.y, pset0.terminals_and_constants_repr,
+    #               filter_warning=True, inter_add=False, inner_add=False, vector_add=True, np_maps=np_map())[1]
+    # sllll=general_expr(slll, pset0, simplifying=False)
```

### Comparing `BindingGP-0.0.36/test/test_simp.py` & `BindingGP-0.0.9/test/test_simp.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 import time
 
 from numpy import random
-from sklearn.datasets import fetch_california_housing
+from sklearn.datasets import load_boston
 
-from bgp.base import SymbolSet, SymbolTree
-from bgp.calculation.translate import compile_context
-from bgp.functions.dimfunc import dless, Dim
+from BGP.base import SymbolSet, SymbolTree
+from BGP.calculation.translate import compile_context
+from BGP.functions.dimfunc import dless, Dim
 
 if __name__ == "__main__":
     # data
-    data = fetch_california_housing()
-    x = data["data"][:100]
-    y = data["target"][:100]
+    data = load_boston()
+    x = data["data"]
+    y = data["target"]
     c = [6, 3, 4]
     # unit
     from sympy.physics.units import kg
 
     x_u = [kg] * 13
     y_u = kg
     c_u = [dless, dless, dless]
```

### Comparing `BindingGP-0.0.36/test/test_symbol_base.py` & `BindingGP-0.0.9/test/test_symbol_base.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 import unittest
 
 import numpy
 
-from bgp.base import CalculatePrecisionSet
-from bgp.base import SymbolSet
-from bgp.base import SymbolTree
-from bgp.functions.dimfunc import dless
+from BGP.base import CalculatePrecisionSet
+from BGP.base import SymbolSet
+from BGP.base import SymbolTree
+from BGP.functions.dimfunc import dless
 
 
 class MyTestbase(unittest.TestCase):
 
     def setUp(self):
         self.SymbolTree = SymbolTree
         self.pset = SymbolSet()
 
-        from sklearn.datasets import fetch_california_housing
+        from sklearn.datasets import load_boston
 
-        data = fetch_california_housing()
-        x = data["data"][:100]
-        y = data["target"][:100]
+        data = load_boston()
+        x = data["data"]
+        y = data["target"]
         # No = Normalizer()
         # y=y/max(y)
         # x = No.fit_transform(x)
         self.x = x
         self.y = y
         # self.pset.add_features(x, y, )
         self.pset.add_features(x, y, x_group=[[1, 2], [4, 5]])
```

### Comparing `BindingGP-0.0.36/test/test_symbol_gp.py` & `BindingGP-0.0.9/test/test_symbol_gp.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,31 +1,31 @@
 import operator
 import unittest
 
 from mgetool import newclass
 from mgetool.packbox import Toolbox
 
-from bgp.base import CalculatePrecisionSet
-from bgp.base import SymbolSet
-from bgp.base import SymbolTree
-from bgp.functions.dimfunc import dless
-from bgp.gp import cxOnePoint, varAnd, genGrow, staticLimit, mutShrink, selKbestDim
+from BGP.base import CalculatePrecisionSet
+from BGP.base import SymbolSet
+from BGP.base import SymbolTree
+from BGP.functions.dimfunc import dless
+from BGP.gp import cxOnePoint, varAnd, genGrow, staticLimit, mutShrink, selKbestDim
 
 
 class MyTestgp(unittest.TestCase):
 
     def setUp(self):
         self.SymbolTree = SymbolTree
         self.pset = SymbolSet()
 
-        from sklearn.datasets import fetch_california_housing
+        from sklearn.datasets import load_boston
 
-        data = fetch_california_housing()
-        x = data["data"][:100]
-        y = data["target"][:100]
+        data = load_boston()
+        x = data["data"]
+        y = data["target"]
 
         self.x = x
         self.y = y
         # self.pset.add_features(x, y, )
         self.pset.add_features(x, y, x_group=[[1, 2], [4, 5]])
         self.pset.add_constants([6, 3, 4], c_dim=[dless, dless, dless], c_prob=None)
         self.pset.add_operations(power_categories=(2, 3, 0.5),
```

