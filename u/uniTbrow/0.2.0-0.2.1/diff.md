# Comparing `tmp/unitbrow-0.2.0.tar.gz` & `tmp/unitbrow-0.2.1.tar.gz`

## Comparing `unitbrow-0.2.0.tar` & `unitbrow-0.2.1.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rwxr-xr-x   0        0        0      155 2020-02-02 00:00:00.000000 unitbrow-0.2.0/.release.sh
--rw-r--r--   0        0        0      216 2020-02-02 00:00:00.000000 unitbrow-0.2.0/tests/unit_tests.py
--rw-r--r--   0        0        0      152 2020-02-02 00:00:00.000000 unitbrow-0.2.0/uniTbrow/__init__.py
--rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 unitbrow-0.2.0/uniTbrow/constants/__init__.py
--rw-r--r--   0        0        0     1107 2020-02-02 00:00:00.000000 unitbrow-0.2.0/uniTbrow/constants/constants.py
--rw-r--r--   0        0        0      135 2020-02-02 00:00:00.000000 unitbrow-0.2.0/uniTbrow/conversions/__init__.py
--rw-r--r--   0        0        0      920 2020-02-02 00:00:00.000000 unitbrow-0.2.0/uniTbrow/conversions/base_unit_systems.py
--rw-r--r--   0        0        0      273 2020-02-02 00:00:00.000000 unitbrow-0.2.0/uniTbrow/conversions/unit_conversions.py
--rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 unitbrow-0.2.0/uniTbrow/dimensions/__init__.py
--rw-r--r--   0        0        0     2190 2020-02-02 00:00:00.000000 unitbrow-0.2.0/uniTbrow/dimensions/dimensions.py
--rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 unitbrow-0.2.0/uniTbrow/parsers/__init__.py
--rw-r--r--   0        0        0      292 2020-02-02 00:00:00.000000 unitbrow-0.2.0/uniTbrow/parsers/unit_parser.py
--rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 unitbrow-0.2.0/uniTbrow/units/__init__.py
--rw-r--r--   0        0        0    18998 2020-02-02 00:00:00.000000 unitbrow-0.2.0/uniTbrow/units/units.py
--rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 unitbrow-0.2.0/.gitignore
--rw-r--r--   0        0        0     9521 2020-02-02 00:00:00.000000 unitbrow-0.2.0/LICENSE
--rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 unitbrow-0.2.0/README.md
--rw-r--r--   0        0        0      608 2020-02-02 00:00:00.000000 unitbrow-0.2.0/pyproject.toml
--rw-r--r--   0        0        0      682 2020-02-02 00:00:00.000000 unitbrow-0.2.0/PKG-INFO
+-rwxr-xr-x   0        0        0      155 2020-02-02 00:00:00.000000 unitbrow-0.2.1/.release.sh
+-rw-r--r--   0        0        0      216 2020-02-02 00:00:00.000000 unitbrow-0.2.1/tests/unit_tests.py
+-rw-r--r--   0        0        0      152 2020-02-02 00:00:00.000000 unitbrow-0.2.1/uniTbrow/__init__.py
+-rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 unitbrow-0.2.1/uniTbrow/constants/__init__.py
+-rw-r--r--   0        0        0     1107 2020-02-02 00:00:00.000000 unitbrow-0.2.1/uniTbrow/constants/constants.py
+-rw-r--r--   0        0        0      135 2020-02-02 00:00:00.000000 unitbrow-0.2.1/uniTbrow/conversions/__init__.py
+-rw-r--r--   0        0        0      920 2020-02-02 00:00:00.000000 unitbrow-0.2.1/uniTbrow/conversions/base_unit_systems.py
+-rw-r--r--   0        0        0      273 2020-02-02 00:00:00.000000 unitbrow-0.2.1/uniTbrow/conversions/unit_conversions.py
+-rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 unitbrow-0.2.1/uniTbrow/dimensions/__init__.py
+-rw-r--r--   0        0        0     2216 2020-02-02 00:00:00.000000 unitbrow-0.2.1/uniTbrow/dimensions/dimensions.py
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 unitbrow-0.2.1/uniTbrow/parsers/__init__.py
+-rw-r--r--   0        0        0      292 2020-02-02 00:00:00.000000 unitbrow-0.2.1/uniTbrow/parsers/unit_parser.py
+-rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 unitbrow-0.2.1/uniTbrow/units/__init__.py
+-rw-r--r--   0        0        0    19024 2020-02-02 00:00:00.000000 unitbrow-0.2.1/uniTbrow/units/units.py
+-rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 unitbrow-0.2.1/.gitignore
+-rw-r--r--   0        0        0     9521 2020-02-02 00:00:00.000000 unitbrow-0.2.1/LICENSE
+-rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 unitbrow-0.2.1/README.md
+-rw-r--r--   0        0        0      608 2020-02-02 00:00:00.000000 unitbrow-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0      682 2020-02-02 00:00:00.000000 unitbrow-0.2.1/PKG-INFO
```

### Comparing `unitbrow-0.2.0/uniTbrow/constants/constants.py` & `unitbrow-0.2.1/uniTbrow/constants/constants.py`

 * *Files identical despite different names*

### Comparing `unitbrow-0.2.0/uniTbrow/conversions/base_unit_systems.py` & `unitbrow-0.2.1/uniTbrow/conversions/base_unit_systems.py`

 * *Files identical despite different names*

### Comparing `unitbrow-0.2.0/uniTbrow/dimensions/dimensions.py` & `unitbrow-0.2.1/uniTbrow/dimensions/dimensions.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 from sympy import symbols as _symbols
 
 
 class Dimension:
     def __init__(self, name, dimension=None):
         if dimension is None:
             self.name = name
-            self.dimension = _symbols(name)
+            self.dimension = _symbols(name, positive=True, real=True)
         else:
             self.name = name
             self.dimension = dimension
 
     def __repr__(self):
         return self.name
```

### Comparing `unitbrow-0.2.0/uniTbrow/units/units.py` & `unitbrow-0.2.1/uniTbrow/units/units.py`

 * *Files 1% similar despite different names*

```diff
@@ -31,15 +31,15 @@
 
 class Unit:
     def __init__(self, dimension: dimensions.Dimension, abbr_symbol: str, alternates=None, base=None, metric=True):
         if alternates is None:
             alternates = []
         assert base is True or (base is not None), "Need to provide a conversion to a base unit"
         self.dimension: dimensions.Dimension = dimension
-        self.symbol = _symbols(abbr_symbol)
+        self.symbol = _symbols(abbr_symbol, positive=True, real=True)
         self.alternates: list = alternates
         self.conversions: dict = dict()
         self.metric: bool = metric
         self.base = base
 
     # add_conversion defines the factor used to convert from other_unit to this unit
     def add_conversion(self, other_unit, expr):
```

### Comparing `unitbrow-0.2.0/LICENSE` & `unitbrow-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `unitbrow-0.2.0/pyproject.toml` & `unitbrow-0.2.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name="uniTbrow"
-version="0.2.0"
+version="0.2.1"
 authors = [
     { name="Matthew Whitaker", email="sub6resources@gmail.com" },
 ]
 dependencies = [
     "sympy",
 ]
 description="Stop raising your brow at unit conversions"
```

### Comparing `unitbrow-0.2.0/PKG-INFO` & `unitbrow-0.2.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: uniTbrow
-Version: 0.2.0
+Version: 0.2.1
 Summary: Stop raising your brow at unit conversions
 Project-URL: Homepage, https://github.com/Sub6Resources/uniTbrow
 Project-URL: Issues, https://github.com/Sub6Resources/uniTbrow/issues
 Author-email: Matthew Whitaker <sub6resources@gmail.com>
 License-File: LICENSE
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
```

