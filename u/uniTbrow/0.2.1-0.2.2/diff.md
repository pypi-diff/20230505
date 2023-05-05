# Comparing `tmp/unitbrow-0.2.1.tar.gz` & `tmp/unitbrow-0.2.2.tar.gz`

## Comparing `unitbrow-0.2.1.tar` & `unitbrow-0.2.2.tar`

### file list

```diff
@@ -1,19 +1,19 @@
--rwxr-xr-x   0        0        0      155 2020-02-02 00:00:00.000000 unitbrow-0.2.1/.release.sh
--rw-r--r--   0        0        0      216 2020-02-02 00:00:00.000000 unitbrow-0.2.1/tests/unit_tests.py
--rw-r--r--   0        0        0      152 2020-02-02 00:00:00.000000 unitbrow-0.2.1/uniTbrow/__init__.py
--rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 unitbrow-0.2.1/uniTbrow/constants/__init__.py
--rw-r--r--   0        0        0     1107 2020-02-02 00:00:00.000000 unitbrow-0.2.1/uniTbrow/constants/constants.py
--rw-r--r--   0        0        0      135 2020-02-02 00:00:00.000000 unitbrow-0.2.1/uniTbrow/conversions/__init__.py
--rw-r--r--   0        0        0      920 2020-02-02 00:00:00.000000 unitbrow-0.2.1/uniTbrow/conversions/base_unit_systems.py
--rw-r--r--   0        0        0      273 2020-02-02 00:00:00.000000 unitbrow-0.2.1/uniTbrow/conversions/unit_conversions.py
--rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 unitbrow-0.2.1/uniTbrow/dimensions/__init__.py
--rw-r--r--   0        0        0     2216 2020-02-02 00:00:00.000000 unitbrow-0.2.1/uniTbrow/dimensions/dimensions.py
--rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 unitbrow-0.2.1/uniTbrow/parsers/__init__.py
--rw-r--r--   0        0        0      292 2020-02-02 00:00:00.000000 unitbrow-0.2.1/uniTbrow/parsers/unit_parser.py
--rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 unitbrow-0.2.1/uniTbrow/units/__init__.py
--rw-r--r--   0        0        0    19024 2020-02-02 00:00:00.000000 unitbrow-0.2.1/uniTbrow/units/units.py
--rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 unitbrow-0.2.1/.gitignore
--rw-r--r--   0        0        0     9521 2020-02-02 00:00:00.000000 unitbrow-0.2.1/LICENSE
--rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 unitbrow-0.2.1/README.md
--rw-r--r--   0        0        0      608 2020-02-02 00:00:00.000000 unitbrow-0.2.1/pyproject.toml
--rw-r--r--   0        0        0      682 2020-02-02 00:00:00.000000 unitbrow-0.2.1/PKG-INFO
+-rwxr-xr-x   0        0        0      155 2020-02-02 00:00:00.000000 unitbrow-0.2.2/.release.sh
+-rw-r--r--   0        0        0      216 2020-02-02 00:00:00.000000 unitbrow-0.2.2/tests/unit_tests.py
+-rw-r--r--   0        0        0      152 2020-02-02 00:00:00.000000 unitbrow-0.2.2/uniTbrow/__init__.py
+-rw-r--r--   0        0        0      100 2020-02-02 00:00:00.000000 unitbrow-0.2.2/uniTbrow/constants/__init__.py
+-rw-r--r--   0        0        0     2079 2020-02-02 00:00:00.000000 unitbrow-0.2.2/uniTbrow/constants/constants.py
+-rw-r--r--   0        0        0      135 2020-02-02 00:00:00.000000 unitbrow-0.2.2/uniTbrow/conversions/__init__.py
+-rw-r--r--   0        0        0      920 2020-02-02 00:00:00.000000 unitbrow-0.2.2/uniTbrow/conversions/base_unit_systems.py
+-rw-r--r--   0        0        0      273 2020-02-02 00:00:00.000000 unitbrow-0.2.2/uniTbrow/conversions/unit_conversions.py
+-rw-r--r--   0        0        0       26 2020-02-02 00:00:00.000000 unitbrow-0.2.2/uniTbrow/dimensions/__init__.py
+-rw-r--r--   0        0        0     2216 2020-02-02 00:00:00.000000 unitbrow-0.2.2/uniTbrow/dimensions/dimensions.py
+-rw-r--r--   0        0        0       37 2020-02-02 00:00:00.000000 unitbrow-0.2.2/uniTbrow/parsers/__init__.py
+-rw-r--r--   0        0        0      292 2020-02-02 00:00:00.000000 unitbrow-0.2.2/uniTbrow/parsers/unit_parser.py
+-rw-r--r--   0        0        0       21 2020-02-02 00:00:00.000000 unitbrow-0.2.2/uniTbrow/units/__init__.py
+-rw-r--r--   0        0        0    19024 2020-02-02 00:00:00.000000 unitbrow-0.2.2/uniTbrow/units/units.py
+-rw-r--r--   0        0        0       40 2020-02-02 00:00:00.000000 unitbrow-0.2.2/.gitignore
+-rw-r--r--   0        0        0     9521 2020-02-02 00:00:00.000000 unitbrow-0.2.2/LICENSE
+-rw-r--r--   0        0        0      140 2020-02-02 00:00:00.000000 unitbrow-0.2.2/README.md
+-rw-r--r--   0        0        0      608 2020-02-02 00:00:00.000000 unitbrow-0.2.2/pyproject.toml
+-rw-r--r--   0        0        0      682 2020-02-02 00:00:00.000000 unitbrow-0.2.2/PKG-INFO
```

### Comparing `unitbrow-0.2.1/uniTbrow/conversions/base_unit_systems.py` & `unitbrow-0.2.2/uniTbrow/conversions/base_unit_systems.py`

 * *Files identical despite different names*

### Comparing `unitbrow-0.2.1/uniTbrow/dimensions/dimensions.py` & `unitbrow-0.2.2/uniTbrow/dimensions/dimensions.py`

 * *Files identical despite different names*

### Comparing `unitbrow-0.2.1/uniTbrow/units/units.py` & `unitbrow-0.2.2/uniTbrow/units/units.py`

 * *Files identical despite different names*

### Comparing `unitbrow-0.2.1/LICENSE` & `unitbrow-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `unitbrow-0.2.1/pyproject.toml` & `unitbrow-0.2.2/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name="uniTbrow"
-version="0.2.1"
+version="0.2.2"
 authors = [
     { name="Matthew Whitaker", email="sub6resources@gmail.com" },
 ]
 dependencies = [
     "sympy",
 ]
 description="Stop raising your brow at unit conversions"
```

### Comparing `unitbrow-0.2.1/PKG-INFO` & `unitbrow-0.2.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: uniTbrow
-Version: 0.2.1
+Version: 0.2.2
 Summary: Stop raising your brow at unit conversions
 Project-URL: Homepage, https://github.com/Sub6Resources/uniTbrow
 Project-URL: Issues, https://github.com/Sub6Resources/uniTbrow/issues
 Author-email: Matthew Whitaker <sub6resources@gmail.com>
 License-File: LICENSE
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
```

