# Comparing `tmp/maoc_support_functions-0.0.2.tar.gz` & `tmp/maoc_support_functions-0.0.3.tar.gz`

## Comparing `maoc_support_functions-0.0.2.tar` & `maoc_support_functions-0.0.3.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 maoc_support_functions-0.0.2/src/maoc_support_functions/__init__.py
--rw-r--r--   0        0        0     6702 2020-02-02 00:00:00.000000 maoc_support_functions-0.0.2/src/maoc_support_functions/representation.py
--rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 maoc_support_functions-0.0.2/src/maoc_support_functions/supporting_functions.py
--rw-r--r--   0        0        0     1087 2020-02-02 00:00:00.000000 maoc_support_functions-0.0.2/LICENSE
--rw-r--r--   0        0        0      275 2020-02-02 00:00:00.000000 maoc_support_functions-0.0.2/README.md
--rw-r--r--   0        0        0      532 2020-02-02 00:00:00.000000 maoc_support_functions-0.0.2/pyproject.toml
--rw-r--r--   0        0        0      738 2020-02-02 00:00:00.000000 maoc_support_functions-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 maoc_support_functions-0.0.3/src/maoc_support_functions/__init__.py
+-rw-r--r--   0        0        0     6702 2020-02-02 00:00:00.000000 maoc_support_functions-0.0.3/src/maoc_support_functions/representation.py
+-rw-r--r--   0        0        0     3092 2020-02-02 00:00:00.000000 maoc_support_functions-0.0.3/src/maoc_support_functions/supporting_functions.py
+-rw-r--r--   0        0        0     1087 2020-02-02 00:00:00.000000 maoc_support_functions-0.0.3/LICENSE
+-rw-r--r--   0        0        0      275 2020-02-02 00:00:00.000000 maoc_support_functions-0.0.3/README.md
+-rw-r--r--   0        0        0      532 2020-02-02 00:00:00.000000 maoc_support_functions-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0      738 2020-02-02 00:00:00.000000 maoc_support_functions-0.0.3/PKG-INFO
```

### Comparing `maoc_support_functions-0.0.2/src/maoc_support_functions/representation.py` & `maoc_support_functions-0.0.3/src/maoc_support_functions/representation.py`

 * *Files identical despite different names*

### Comparing `maoc_support_functions-0.0.2/src/maoc_support_functions/supporting_functions.py` & `maoc_support_functions-0.0.3/src/maoc_support_functions/supporting_functions.py`

 * *Files 5% similar despite different names*

```diff
@@ -28,14 +28,15 @@
 
 
 # In[ ]:
 
 
 def MAOC_atom_extraction(file):
     import pandas as pd
+    import re
     A=open(file).readlines()
     B=A[2:]
     for qaz in B:
         if qaz=='\n':
             B.remove('\n')
     C=[x.split()[0] for x in B]
     my_dict = {i:C.count(i) for i in C}
```

### Comparing `maoc_support_functions-0.0.2/LICENSE` & `maoc_support_functions-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `maoc_support_functions-0.0.2/pyproject.toml` & `maoc_support_functions-0.0.3/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "maoc_support_functions"
-version = "0.0.2"
+version = "0.0.3"
 authors = [
   { name="Stiv Llenga", email="stiv.llenga@h-its.org" },
 ]
 description = "Functions for generating the MAOC representation."
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `maoc_support_functions-0.0.2/PKG-INFO` & `maoc_support_functions-0.0.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: maoc_support_functions
-Version: 0.0.2
+Version: 0.0.3
 Summary: Functions for generating the MAOC representation.
 Project-URL: Homepage, https://github.com/hits-ccc/MAOC
 Author-email: Stiv Llenga <stiv.llenga@h-its.org>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
```

