# Comparing `tmp/maoc_support_functions-0.0.1.tar.gz` & `tmp/maoc_support_functions-0.0.2.tar.gz`

## Comparing `maoc_support_functions-0.0.1.tar` & `maoc_support_functions-0.0.2.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 maoc_support_functions-0.0.1/src/maoc_support_functions/__init__.py
--rw-r--r--   0        0        0     6702 2020-02-02 00:00:00.000000 maoc_support_functions-0.0.1/src/maoc_support_functions/representation.py
--rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 maoc_support_functions-0.0.1/src/maoc_support_functions/supporting_functions.py
--rw-r--r--   0        0        0     1087 2020-02-02 00:00:00.000000 maoc_support_functions-0.0.1/LICENSE
--rw-r--r--   0        0        0      289 2020-02-02 00:00:00.000000 maoc_support_functions-0.0.1/README.md
--rw-r--r--   0        0        0      532 2020-02-02 00:00:00.000000 maoc_support_functions-0.0.1/pyproject.toml
--rw-r--r--   0        0        0      752 2020-02-02 00:00:00.000000 maoc_support_functions-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 maoc_support_functions-0.0.2/src/maoc_support_functions/__init__.py
+-rw-r--r--   0        0        0     6702 2020-02-02 00:00:00.000000 maoc_support_functions-0.0.2/src/maoc_support_functions/representation.py
+-rw-r--r--   0        0        0     3078 2020-02-02 00:00:00.000000 maoc_support_functions-0.0.2/src/maoc_support_functions/supporting_functions.py
+-rw-r--r--   0        0        0     1087 2020-02-02 00:00:00.000000 maoc_support_functions-0.0.2/LICENSE
+-rw-r--r--   0        0        0      275 2020-02-02 00:00:00.000000 maoc_support_functions-0.0.2/README.md
+-rw-r--r--   0        0        0      532 2020-02-02 00:00:00.000000 maoc_support_functions-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0      738 2020-02-02 00:00:00.000000 maoc_support_functions-0.0.2/PKG-INFO
```

### Comparing `maoc_support_functions-0.0.1/src/maoc_support_functions/representation.py` & `maoc_support_functions-0.0.2/src/maoc_support_functions/representation.py`

 * *Files identical despite different names*

### Comparing `maoc_support_functions-0.0.1/src/maoc_support_functions/supporting_functions.py` & `maoc_support_functions-0.0.2/src/maoc_support_functions/supporting_functions.py`

 * *Files identical despite different names*

### Comparing `maoc_support_functions-0.0.1/LICENSE` & `maoc_support_functions-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `maoc_support_functions-0.0.1/pyproject.toml` & `maoc_support_functions-0.0.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "maoc_support_functions"
-version = "0.0.1"
+version = "0.0.2"
 authors = [
   { name="Stiv Llenga", email="stiv.llenga@h-its.org" },
 ]
 description = "Functions for generating the MAOC representation."
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `maoc_support_functions-0.0.1/PKG-INFO` & `maoc_support_functions-0.0.2/PKG-INFO`

 * *Files 23% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 2.1
 Name: maoc_support_functions
-Version: 0.0.1
+Version: 0.0.2
 Summary: Functions for generating the MAOC representation.
 Project-URL: Homepage, https://github.com/hits-ccc/MAOC
 Author-email: Stiv Llenga <stiv.llenga@h-its.org>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 
 The matrix of orthogonal atomic orbital coefficients (https://chemrxiv.org/engage/chemrxiv/article-details/64160d85aad2a62ca1f937f6) was generated with the help of these several different functions.
 For more info please check: 
-[Github-flavored Markdown](https://github.com/hits-ccc/MAOC)
+[CCC GITHUB](https://github.com/hits-ccc/MAOC)
```

