# Comparing `tmp/maoc_support_functions-0.0.4.tar.gz` & `tmp/maoc_support_functions-0.0.5.tar.gz`

## Comparing `maoc_support_functions-0.0.4.tar` & `maoc_support_functions-0.0.5.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 maoc_support_functions-0.0.4/src/maoc_support_functions/__init__.py
--rw-r--r--   0        0        0     6764 2020-02-02 00:00:00.000000 maoc_support_functions-0.0.4/src/maoc_support_functions/representation.py
--rw-r--r--   0        0        0     3092 2020-02-02 00:00:00.000000 maoc_support_functions-0.0.4/src/maoc_support_functions/supporting_functions.py
--rw-r--r--   0        0        0     1087 2020-02-02 00:00:00.000000 maoc_support_functions-0.0.4/LICENSE
--rw-r--r--   0        0        0      275 2020-02-02 00:00:00.000000 maoc_support_functions-0.0.4/README.md
--rw-r--r--   0        0        0      532 2020-02-02 00:00:00.000000 maoc_support_functions-0.0.4/pyproject.toml
--rw-r--r--   0        0        0      738 2020-02-02 00:00:00.000000 maoc_support_functions-0.0.4/PKG-INFO
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 maoc_support_functions-0.0.5/src/maoc_support_functions/__init__.py
+-rw-r--r--   0        0        0     7023 2020-02-02 00:00:00.000000 maoc_support_functions-0.0.5/src/maoc_support_functions/representation.py
+-rw-r--r--   0        0        0     3092 2020-02-02 00:00:00.000000 maoc_support_functions-0.0.5/src/maoc_support_functions/supporting_functions.py
+-rw-r--r--   0        0        0     1087 2020-02-02 00:00:00.000000 maoc_support_functions-0.0.5/LICENSE
+-rw-r--r--   0        0        0      275 2020-02-02 00:00:00.000000 maoc_support_functions-0.0.5/README.md
+-rw-r--r--   0        0        0      532 2020-02-02 00:00:00.000000 maoc_support_functions-0.0.5/pyproject.toml
+-rw-r--r--   0        0        0      738 2020-02-02 00:00:00.000000 maoc_support_functions-0.0.5/PKG-INFO
```

### Comparing `maoc_support_functions-0.0.4/src/maoc_support_functions/representation.py` & `maoc_support_functions-0.0.5/src/maoc_support_functions/representation.py`

 * *Files 7% similar despite different names*

```diff
@@ -6,15 +6,18 @@
 
 #The code that generates the MAOC representation
 def MAOC(PATH=None, basis_set='sto-3g',charge=0,nr_pca=None,spin=None,pre_orth_AO='ANO',pca_explanation=True):
     from pyscf import scf,gto,lo
     import glob
     import pandas as pd
     import numpy as np
-    from maoc_support_functions.supporting_functions import *
+    from maoc_support_functions.supporting_functions import MAOC_atom_extraction
+    from maoc_support_functions.supporting_functions import MAOC_min_ch_max_ch
+    from maoc_support_functions.supporting_functions import MAOC_partial_charges
+    from maoc_support_functions.supporting_functions import MAOC_periodic_table
     from natsort import natsorted
     from sklearn.decomposition import PCA
     from openbabel import openbabel as ob
     
     maoc_pca=[] # A list used to store PCX-MAOC arrays. Users can simply transform the [1,X] array into [N,X/N] and use the non-flattened representation. 
     
     maoc=[] # A list having the MAOC array. If the flattened version is used, each element is represented by a [1, M] array, whereas the extent of the array for the non-flatten version is [sqr(M),sqr(M)].
```

### Comparing `maoc_support_functions-0.0.4/src/maoc_support_functions/supporting_functions.py` & `maoc_support_functions-0.0.5/src/maoc_support_functions/supporting_functions.py`

 * *Files identical despite different names*

### Comparing `maoc_support_functions-0.0.4/LICENSE` & `maoc_support_functions-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `maoc_support_functions-0.0.4/pyproject.toml` & `maoc_support_functions-0.0.5/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "maoc_support_functions"
-version = "0.0.4"
+version = "0.0.5"
 authors = [
   { name="Stiv Llenga", email="stiv.llenga@h-its.org" },
 ]
 description = "Functions for generating the MAOC representation."
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `maoc_support_functions-0.0.4/PKG-INFO` & `maoc_support_functions-0.0.5/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: maoc_support_functions
-Version: 0.0.4
+Version: 0.0.5
 Summary: Functions for generating the MAOC representation.
 Project-URL: Homepage, https://github.com/hits-ccc/MAOC
 Author-email: Stiv Llenga <stiv.llenga@h-its.org>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
```

