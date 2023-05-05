# Comparing `tmp/multimetricprog-0.0.4.tar.gz` & `tmp/multimetricprog-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "multimetricprog-0.0.4.tar", last modified: Fri May  5 02:26:15 2023, max compression
+gzip compressed data, was "multimetricprog-0.0.5.tar", last modified: Fri May  5 03:28:08 2023, max compression
```

## Comparing `multimetricprog-0.0.4.tar` & `multimetricprog-0.0.5.tar`

### file list

```diff
@@ -1,51 +1,51 @@
-drwxrwxrwx   0        0        0        0 2023-05-05 02:26:15.887447 multimetricprog-0.0.4/
--rw-rw-rw-   0        0        0     1350 2023-05-04 16:59:00.000000 multimetricprog-0.0.4/LICENSE
--rw-rw-rw-   0        0        0       62 2023-05-04 16:59:00.000000 multimetricprog-0.0.4/MANIFEST.in
--rw-rw-rw-   0        0        0     8357 2023-05-05 02:26:15.886447 multimetricprog-0.0.4/PKG-INFO
--rw-rw-rw-   0        0        0     7634 2023-05-04 16:59:00.000000 multimetricprog-0.0.4/README.md
-drwxrwxrwx   0        0        0        0 2023-05-05 02:26:15.846449 multimetricprog-0.0.4/multimetricprog/
--rw-rw-rw-   0        0        0       19 2023-05-04 16:59:00.000000 multimetricprog-0.0.4/multimetricprog/__init__.py
--rw-rw-rw-   0        0        0     3412 2023-05-05 01:33:18.000000 multimetricprog-0.0.4/multimetricprog/calculator.py
-drwxrwxrwx   0        0        0        0 2023-05-05 02:26:15.867448 multimetricprog-0.0.4/multimetricprog/cls/
--rw-rw-rw-   0        0        0        0 2023-05-04 16:59:00.000000 multimetricprog-0.0.4/multimetricprog/cls/__init__.py
--rw-rw-rw-   0        0        0      745 2023-05-04 16:59:00.000000 multimetricprog-0.0.4/multimetricprog/cls/base.py
--rw-rw-rw-   0        0        0      289 2023-05-04 16:59:00.000000 multimetricprog-0.0.4/multimetricprog/cls/base_calc.py
--rw-rw-rw-   0        0        0      294 2023-05-04 16:59:00.000000 multimetricprog-0.0.4/multimetricprog/cls/base_stats.py
-drwxrwxrwx   0        0        0        0 2023-05-05 02:26:15.871447 multimetricprog-0.0.4/multimetricprog/cls/calc/
--rw-rw-rw-   0        0        0        0 2023-05-04 16:59:00.000000 multimetricprog-0.0.4/multimetricprog/cls/calc/__init__.py
--rw-rw-rw-   0        0        0     3560 2023-05-04 16:59:00.000000 multimetricprog-0.0.4/multimetricprog/cls/calc/halstead.py
--rw-rw-rw-   0        0        0     2020 2023-05-04 16:59:00.000000 multimetricprog-0.0.4/multimetricprog/cls/calc/maintenance.py
--rw-rw-rw-   0        0        0     2254 2023-05-04 16:59:00.000000 multimetricprog-0.0.4/multimetricprog/cls/calc/pylint.py
--rw-rw-rw-   0        0        0     4870 2023-05-04 16:59:00.000000 multimetricprog-0.0.4/multimetricprog/cls/calc/tiobe.py
-drwxrwxrwx   0        0        0        0 2023-05-05 02:26:15.875446 multimetricprog-0.0.4/multimetricprog/cls/importer/
--rw-rw-rw-   0        0        0        0 2023-05-04 16:59:00.000000 multimetricprog-0.0.4/multimetricprog/cls/importer/__init__.py
--rw-rw-rw-   0        0        0     1098 2023-05-04 16:59:00.000000 multimetricprog-0.0.4/multimetricprog/cls/importer/base.py
--rw-rw-rw-   0        0        0      385 2023-05-04 16:59:00.000000 multimetricprog-0.0.4/multimetricprog/cls/importer/filtered.py
-drwxrwxrwx   0        0        0        0 2023-05-05 02:26:15.878446 multimetricprog-0.0.4/multimetricprog/cls/importer/mods/
--rw-rw-rw-   0        0        0        0 2023-05-04 16:59:00.000000 multimetricprog-0.0.4/multimetricprog/cls/importer/mods/__init__.py
--rw-rw-rw-   0        0        0      558 2023-05-04 16:59:00.000000 multimetricprog-0.0.4/multimetricprog/cls/importer/mods/csv.py
--rw-rw-rw-   0        0        0      739 2023-05-04 16:59:00.000000 multimetricprog-0.0.4/multimetricprog/cls/importer/mods/json.py
--rw-rw-rw-   0        0        0      583 2023-05-04 16:59:00.000000 multimetricprog-0.0.4/multimetricprog/cls/importer/pick.py
-drwxrwxrwx   0        0        0        0 2023-05-05 02:26:15.883447 multimetricprog-0.0.4/multimetricprog/cls/metric/
--rw-rw-rw-   0        0        0        0 2023-05-04 16:59:00.000000 multimetricprog-0.0.4/multimetricprog/cls/metric/__init__.py
--rw-rw-rw-   0        0        0     1786 2023-05-04 16:59:00.000000 multimetricprog-0.0.4/multimetricprog/cls/metric/comments.py
--rw-rw-rw-   0        0        0     1743 2023-05-04 16:59:00.000000 multimetricprog-0.0.4/multimetricprog/cls/metric/cyclomatic.py
--rw-rw-rw-   0        0        0     4403 2023-05-04 16:59:00.000000 multimetricprog-0.0.4/multimetricprog/cls/metric/fanout.py
--rw-rw-rw-   0        0        0      991 2023-05-04 16:59:00.000000 multimetricprog-0.0.4/multimetricprog/cls/metric/loc.py
--rw-rw-rw-   0        0        0     2516 2023-05-04 16:59:00.000000 multimetricprog-0.0.4/multimetricprog/cls/metric/operands.py
--rw-rw-rw-   0        0        0     1680 2023-05-04 16:59:00.000000 multimetricprog-0.0.4/multimetricprog/cls/metric/operators.py
--rw-rw-rw-   0        0        0     2201 2023-05-04 16:59:00.000000 multimetricprog-0.0.4/multimetricprog/cls/modules.py
-drwxrwxrwx   0        0        0        0 2023-05-05 02:26:15.885446 multimetricprog-0.0.4/multimetricprog/cls/stats/
--rw-rw-rw-   0        0        0        0 2023-05-04 16:59:00.000000 multimetricprog-0.0.4/multimetricprog/cls/stats/__init__.py
--rw-rw-rw-   0        0        0     1398 2023-05-04 16:59:00.000000 multimetricprog-0.0.4/multimetricprog/cls/stats/stats.py
--rw-rw-rw-   0        0        0     1739 2023-05-04 16:59:00.000000 multimetricprog-0.0.4/multimetricprog/fp.py
-drwxrwxrwx   0        0        0        0 2023-05-05 02:26:15.863446 multimetricprog-0.0.4/multimetricprog.egg-info/
--rw-rw-rw-   0        0        0     8357 2023-05-05 02:26:15.000000 multimetricprog-0.0.4/multimetricprog.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1312 2023-05-05 02:26:15.000000 multimetricprog-0.0.4/multimetricprog.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-05 02:26:15.000000 multimetricprog-0.0.4/multimetricprog.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       32 2023-05-05 02:26:15.000000 multimetricprog-0.0.4/multimetricprog.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2023-05-05 02:26:15.000000 multimetricprog-0.0.4/multimetricprog.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      730 2023-05-05 02:26:02.000000 multimetricprog-0.0.4/pyproject.toml
--rw-rw-rw-   0        0        0      254 2023-05-05 01:39:57.000000 multimetricprog-0.0.4/requirements.txt
--rw-rw-rw-   0        0        0       42 2023-05-05 02:26:15.887447 multimetricprog-0.0.4/setup.cfg
--rw-rw-rw-   0        0        0     1776 2023-05-05 02:25:47.000000 multimetricprog-0.0.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-05 03:28:08.567393 multimetricprog-0.0.5/
+-rw-rw-rw-   0        0        0     1350 2023-05-04 16:59:00.000000 multimetricprog-0.0.5/LICENSE
+-rw-rw-rw-   0        0        0       62 2023-05-04 16:59:00.000000 multimetricprog-0.0.5/MANIFEST.in
+-rw-rw-rw-   0        0        0     8357 2023-05-05 03:28:08.566393 multimetricprog-0.0.5/PKG-INFO
+-rw-rw-rw-   0        0        0     7634 2023-05-04 16:59:00.000000 multimetricprog-0.0.5/README.md
+drwxrwxrwx   0        0        0        0 2023-05-05 03:28:08.532393 multimetricprog-0.0.5/multimetricprog/
+-rw-rw-rw-   0        0        0       19 2023-05-04 16:59:00.000000 multimetricprog-0.0.5/multimetricprog/__init__.py
+-rw-rw-rw-   0        0        0     3239 2023-05-05 03:25:20.000000 multimetricprog-0.0.5/multimetricprog/calculator.py
+drwxrwxrwx   0        0        0        0 2023-05-05 03:28:08.548395 multimetricprog-0.0.5/multimetricprog/cls/
+-rw-rw-rw-   0        0        0        0 2023-05-04 16:59:00.000000 multimetricprog-0.0.5/multimetricprog/cls/__init__.py
+-rw-rw-rw-   0        0        0      745 2023-05-04 16:59:00.000000 multimetricprog-0.0.5/multimetricprog/cls/base.py
+-rw-rw-rw-   0        0        0      289 2023-05-04 16:59:00.000000 multimetricprog-0.0.5/multimetricprog/cls/base_calc.py
+-rw-rw-rw-   0        0        0      294 2023-05-04 16:59:00.000000 multimetricprog-0.0.5/multimetricprog/cls/base_stats.py
+drwxrwxrwx   0        0        0        0 2023-05-05 03:28:08.552393 multimetricprog-0.0.5/multimetricprog/cls/calc/
+-rw-rw-rw-   0        0        0        0 2023-05-04 16:59:00.000000 multimetricprog-0.0.5/multimetricprog/cls/calc/__init__.py
+-rw-rw-rw-   0        0        0     3560 2023-05-04 16:59:00.000000 multimetricprog-0.0.5/multimetricprog/cls/calc/halstead.py
+-rw-rw-rw-   0        0        0     2020 2023-05-04 16:59:00.000000 multimetricprog-0.0.5/multimetricprog/cls/calc/maintenance.py
+-rw-rw-rw-   0        0        0     2254 2023-05-04 16:59:00.000000 multimetricprog-0.0.5/multimetricprog/cls/calc/pylint.py
+-rw-rw-rw-   0        0        0     4870 2023-05-04 16:59:00.000000 multimetricprog-0.0.5/multimetricprog/cls/calc/tiobe.py
+drwxrwxrwx   0        0        0        0 2023-05-05 03:28:08.555393 multimetricprog-0.0.5/multimetricprog/cls/importer/
+-rw-rw-rw-   0        0        0        0 2023-05-04 16:59:00.000000 multimetricprog-0.0.5/multimetricprog/cls/importer/__init__.py
+-rw-rw-rw-   0        0        0     1098 2023-05-04 16:59:00.000000 multimetricprog-0.0.5/multimetricprog/cls/importer/base.py
+-rw-rw-rw-   0        0        0      385 2023-05-04 16:59:00.000000 multimetricprog-0.0.5/multimetricprog/cls/importer/filtered.py
+drwxrwxrwx   0        0        0        0 2023-05-05 03:28:08.558393 multimetricprog-0.0.5/multimetricprog/cls/importer/mods/
+-rw-rw-rw-   0        0        0        0 2023-05-04 16:59:00.000000 multimetricprog-0.0.5/multimetricprog/cls/importer/mods/__init__.py
+-rw-rw-rw-   0        0        0      558 2023-05-04 16:59:00.000000 multimetricprog-0.0.5/multimetricprog/cls/importer/mods/csv.py
+-rw-rw-rw-   0        0        0      739 2023-05-04 16:59:00.000000 multimetricprog-0.0.5/multimetricprog/cls/importer/mods/json.py
+-rw-rw-rw-   0        0        0      583 2023-05-04 16:59:00.000000 multimetricprog-0.0.5/multimetricprog/cls/importer/pick.py
+drwxrwxrwx   0        0        0        0 2023-05-05 03:28:08.564393 multimetricprog-0.0.5/multimetricprog/cls/metric/
+-rw-rw-rw-   0        0        0        0 2023-05-04 16:59:00.000000 multimetricprog-0.0.5/multimetricprog/cls/metric/__init__.py
+-rw-rw-rw-   0        0        0     1786 2023-05-04 16:59:00.000000 multimetricprog-0.0.5/multimetricprog/cls/metric/comments.py
+-rw-rw-rw-   0        0        0     1743 2023-05-04 16:59:00.000000 multimetricprog-0.0.5/multimetricprog/cls/metric/cyclomatic.py
+-rw-rw-rw-   0        0        0     4403 2023-05-04 16:59:00.000000 multimetricprog-0.0.5/multimetricprog/cls/metric/fanout.py
+-rw-rw-rw-   0        0        0      991 2023-05-04 16:59:00.000000 multimetricprog-0.0.5/multimetricprog/cls/metric/loc.py
+-rw-rw-rw-   0        0        0     2516 2023-05-04 16:59:00.000000 multimetricprog-0.0.5/multimetricprog/cls/metric/operands.py
+-rw-rw-rw-   0        0        0     1680 2023-05-04 16:59:00.000000 multimetricprog-0.0.5/multimetricprog/cls/metric/operators.py
+-rw-rw-rw-   0        0        0     2201 2023-05-04 16:59:00.000000 multimetricprog-0.0.5/multimetricprog/cls/modules.py
+drwxrwxrwx   0        0        0        0 2023-05-05 03:28:08.565393 multimetricprog-0.0.5/multimetricprog/cls/stats/
+-rw-rw-rw-   0        0        0        0 2023-05-04 16:59:00.000000 multimetricprog-0.0.5/multimetricprog/cls/stats/__init__.py
+-rw-rw-rw-   0        0        0     1398 2023-05-04 16:59:00.000000 multimetricprog-0.0.5/multimetricprog/cls/stats/stats.py
+-rw-rw-rw-   0        0        0     1739 2023-05-04 16:59:00.000000 multimetricprog-0.0.5/multimetricprog/fp.py
+drwxrwxrwx   0        0        0        0 2023-05-05 03:28:08.544394 multimetricprog-0.0.5/multimetricprog.egg-info/
+-rw-rw-rw-   0        0        0     8357 2023-05-05 03:28:08.000000 multimetricprog-0.0.5/multimetricprog.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1312 2023-05-05 03:28:08.000000 multimetricprog-0.0.5/multimetricprog.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-05 03:28:08.000000 multimetricprog-0.0.5/multimetricprog.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       32 2023-05-05 03:28:08.000000 multimetricprog-0.0.5/multimetricprog.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2023-05-05 03:28:08.000000 multimetricprog-0.0.5/multimetricprog.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      730 2023-05-05 03:27:56.000000 multimetricprog-0.0.5/pyproject.toml
+-rw-rw-rw-   0        0        0      254 2023-05-05 01:39:57.000000 multimetricprog-0.0.5/requirements.txt
+-rw-rw-rw-   0        0        0       42 2023-05-05 03:28:08.567393 multimetricprog-0.0.5/setup.cfg
+-rw-rw-rw-   0        0        0     1776 2023-05-05 02:25:47.000000 multimetricprog-0.0.5/setup.py
```

### Comparing `multimetricprog-0.0.4/LICENSE` & `multimetricprog-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `multimetricprog-0.0.4/PKG-INFO` & `multimetricprog-0.0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: multimetricprog
-Version: 0.0.4
+Version: 0.0.5
 Summary: Calculate code metrics in various languages
 Home-page: https://github.com/VadokDev/multimetric-programmatically
 Author: Konrad Weihmann
 Author-email: Gonzalo Fernández <gonzalo.fdez06@gmail.com>, Konrad Weihmann <kweihmann@outlook.com>
 Project-URL: Homepage, https://github.com/VadokDev/multimetric-programmatically
 Project-URL: Bug Tracker, https://github.com/VadokDev/multimetric-programmatically/issues
 Classifier: Programming Language :: Python :: 3
```

### Comparing `multimetricprog-0.0.4/README.md` & `multimetricprog-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `multimetricprog-0.0.4/multimetricprog/calculator.py` & `multimetricprog-0.0.5/multimetricprog/calculator.py`

 * *Files 10% similar despite different names*

```diff
@@ -63,27 +63,24 @@
     try:
         _cnt = bytes(code, "utf-8")
         _enc = chardet.detect(_cnt)
         _cnt = _cnt.decode(_enc["encoding"]).encode("utf-8")
         _localImporter = {k: FilteredImporter(
             v, _file) for k, v in _importer.items()}
         tokens = list(_lexer.get_tokens(_cnt))
-        if _args.dump:
-            for x in tokens:
-                print("{}: {} -> {}".format(_file, x[0], str(x[1])))
-        else:
-            _localMetrics = get_modules_metrics(_args, **_localImporter)
-            _localCalc = get_modules_calculated(_args, **_localImporter)
-            for x in _localMetrics:
-                x.parse_tokens(_lexer.name, tokens)
-                res.update(x.get_results())
-                store.update(x.get_internal_store())
-            for x in _localCalc:
-                res.update(x.get_results(res))
-                store.update(x.get_internal_store())
+
+        _localMetrics = get_modules_metrics(_args, **_localImporter)
+        _localCalc = get_modules_calculated(_args, **_localImporter)
+        for x in _localMetrics:
+            x.parse_tokens(_lexer.name, tokens)
+            res.update(x.get_results())
+            store.update(x.get_internal_store())
+        for x in _localCalc:
+            res.update(x.get_results(res))
+            store.update(x.get_internal_store())
     except Exception:
         tokens = []
 
     results = [(res, _file, _lexer.name, tokens, store)]
 
     for x in results:
         _result["files"][x[1]] = x[0]
```

### Comparing `multimetricprog-0.0.4/multimetricprog/cls/base.py` & `multimetricprog-0.0.5/multimetricprog/cls/base.py`

 * *Files identical despite different names*

### Comparing `multimetricprog-0.0.4/multimetricprog/cls/calc/halstead.py` & `multimetricprog-0.0.5/multimetricprog/cls/calc/halstead.py`

 * *Files identical despite different names*

### Comparing `multimetricprog-0.0.4/multimetricprog/cls/calc/maintenance.py` & `multimetricprog-0.0.5/multimetricprog/cls/calc/maintenance.py`

 * *Files identical despite different names*

### Comparing `multimetricprog-0.0.4/multimetricprog/cls/calc/pylint.py` & `multimetricprog-0.0.5/multimetricprog/cls/calc/pylint.py`

 * *Files identical despite different names*

### Comparing `multimetricprog-0.0.4/multimetricprog/cls/calc/tiobe.py` & `multimetricprog-0.0.5/multimetricprog/cls/calc/tiobe.py`

 * *Files identical despite different names*

### Comparing `multimetricprog-0.0.4/multimetricprog/cls/importer/base.py` & `multimetricprog-0.0.5/multimetricprog/cls/importer/base.py`

 * *Files identical despite different names*

### Comparing `multimetricprog-0.0.4/multimetricprog/cls/importer/mods/csv.py` & `multimetricprog-0.0.5/multimetricprog/cls/importer/mods/csv.py`

 * *Files identical despite different names*

### Comparing `multimetricprog-0.0.4/multimetricprog/cls/importer/mods/json.py` & `multimetricprog-0.0.5/multimetricprog/cls/importer/mods/json.py`

 * *Files identical despite different names*

### Comparing `multimetricprog-0.0.4/multimetricprog/cls/importer/pick.py` & `multimetricprog-0.0.5/multimetricprog/cls/importer/pick.py`

 * *Files identical despite different names*

### Comparing `multimetricprog-0.0.4/multimetricprog/cls/metric/comments.py` & `multimetricprog-0.0.5/multimetricprog/cls/metric/comments.py`

 * *Files identical despite different names*

### Comparing `multimetricprog-0.0.4/multimetricprog/cls/metric/cyclomatic.py` & `multimetricprog-0.0.5/multimetricprog/cls/metric/cyclomatic.py`

 * *Files identical despite different names*

### Comparing `multimetricprog-0.0.4/multimetricprog/cls/metric/fanout.py` & `multimetricprog-0.0.5/multimetricprog/cls/metric/fanout.py`

 * *Files identical despite different names*

### Comparing `multimetricprog-0.0.4/multimetricprog/cls/metric/loc.py` & `multimetricprog-0.0.5/multimetricprog/cls/metric/loc.py`

 * *Files identical despite different names*

### Comparing `multimetricprog-0.0.4/multimetricprog/cls/metric/operands.py` & `multimetricprog-0.0.5/multimetricprog/cls/metric/operands.py`

 * *Files identical despite different names*

### Comparing `multimetricprog-0.0.4/multimetricprog/cls/metric/operators.py` & `multimetricprog-0.0.5/multimetricprog/cls/metric/operators.py`

 * *Files identical despite different names*

### Comparing `multimetricprog-0.0.4/multimetricprog/cls/modules.py` & `multimetricprog-0.0.5/multimetricprog/cls/modules.py`

 * *Files identical despite different names*

### Comparing `multimetricprog-0.0.4/multimetricprog/cls/stats/stats.py` & `multimetricprog-0.0.5/multimetricprog/cls/stats/stats.py`

 * *Files identical despite different names*

### Comparing `multimetricprog-0.0.4/multimetricprog/fp.py` & `multimetricprog-0.0.5/multimetricprog/fp.py`

 * *Files identical despite different names*

### Comparing `multimetricprog-0.0.4/multimetricprog.egg-info/PKG-INFO` & `multimetricprog-0.0.5/multimetricprog.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: multimetricprog
-Version: 0.0.4
+Version: 0.0.5
 Summary: Calculate code metrics in various languages
 Home-page: https://github.com/VadokDev/multimetric-programmatically
 Author: Konrad Weihmann
 Author-email: Gonzalo Fernández <gonzalo.fdez06@gmail.com>, Konrad Weihmann <kweihmann@outlook.com>
 Project-URL: Homepage, https://github.com/VadokDev/multimetric-programmatically
 Project-URL: Bug Tracker, https://github.com/VadokDev/multimetric-programmatically/issues
 Classifier: Programming Language :: Python :: 3
```

### Comparing `multimetricprog-0.0.4/multimetricprog.egg-info/SOURCES.txt` & `multimetricprog-0.0.5/multimetricprog.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `multimetricprog-0.0.4/pyproject.toml` & `multimetricprog-0.0.5/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=40.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "multimetricprog"
-version = "0.0.4"
+version = "0.0.5"
 authors = [
   { name="Gonzalo Fernández", email="gonzalo.fdez06@gmail.com" },
   { name="Konrad Weihmann", email="kweihmann@outlook.com" },
 ]
 description = "Calculate code metrics in various languages"
 readme = "README.md"
 requires-python = ">=3.7"
```

### Comparing `multimetricprog-0.0.4/setup.py` & `multimetricprog-0.0.5/setup.py`

 * *Files identical despite different names*

