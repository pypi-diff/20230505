# Comparing `tmp/better_python_lists-0.1.2.tar.gz` & `tmp/better_python_lists-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "better_python_lists-0.1.2.tar", max compression
+gzip compressed data, was "better_python_lists-0.1.3.tar", max compression
```

## Comparing `better_python_lists-0.1.2.tar` & `better_python_lists-0.1.3.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0    35149 2023-05-04 16:25:45.097915 better_python_lists-0.1.2/LICENSE
--rw-r--r--   0        0        0      981 2023-05-04 18:31:27.446961 better_python_lists-0.1.2/README.md
--rw-r--r--   0        0        0       23 2023-05-04 17:38:53.402760 better_python_lists-0.1.2/better_python_lists/__init__.py
--rw-r--r--   0        0        0      892 2023-05-04 18:12:22.339636 better_python_lists-0.1.2/better_python_lists/list.py
--rw-r--r--   0        0        0      480 2023-05-04 18:31:57.675723 better_python_lists-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     1602 1970-01-01 00:00:00.000000 better_python_lists-0.1.2/setup.py
--rw-r--r--   0        0        0     1424 1970-01-01 00:00:00.000000 better_python_lists-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0    35149 2023-05-04 16:25:45.097915 better_python_lists-0.1.3/LICENSE
+-rw-r--r--   0        0        0     1686 2023-05-05 11:53:08.125467 better_python_lists-0.1.3/README.md
+-rw-r--r--   0        0        0       23 2023-05-04 17:38:53.402760 better_python_lists-0.1.3/better_python_lists/__init__.py
+-rw-r--r--   0        0        0     1713 2023-05-04 20:13:30.847223 better_python_lists-0.1.3/better_python_lists/list.py
+-rw-r--r--   0        0        0      498 2023-05-05 11:49:37.484261 better_python_lists-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0     2333 1970-01-01 00:00:00.000000 better_python_lists-0.1.3/setup.py
+-rw-r--r--   0        0        0     2129 1970-01-01 00:00:00.000000 better_python_lists-0.1.3/PKG-INFO
```

### Comparing `better_python_lists-0.1.2/LICENSE` & `better_python_lists-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `better_python_lists-0.1.2/PKG-INFO` & `better_python_lists-0.1.3/PKG-INFO`

 * *Files 26% similar despite different names*

```diff
@@ -1,43 +1,55 @@
 Metadata-Version: 2.1
 Name: better-python-lists
-Version: 0.1.2
+Version: 0.1.3
 Summary: Adds some useful methods on top of Python lists
 License: GNU GENERAL PUBLIC LICENSE v3
 Author: Bradley Marques
 Author-email: bradleyrcmarques@gmail.com
 Requires-Python: >=3.11,<4.0
 Classifier: License :: Other/Proprietary License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.11
 Description-Content-Type: text/markdown
 
 # Better Python Lists
 
 Makes lists in Python better, by adding some useful methods.
 
++ `List.compact()` - removes all `None` values from the List.
++ `List.flatten()` - flattens an arbitrarily nested List.
+
 ## Installation
 
 `pip install better-python-lists`
 
 ## Basic Usage
 
+```py
+List([1, None, 2, 3, 4, None, None, 5]).compact()
+# => List[(1, 2, 3, 4, 5)]
+
+List([["a"], "b", 5, [6, 7, [8, 9, [10]]]]).flatten()
+# => List(["a", "b", 5, 6, 7, 8, 9, 10])
+```
+
+## Details
+
 ### Compact
 
 The `compact` method is inspired by
 [Ruby's `Array.compact`](https://ruby-doc.org/core-3.0.0/Array.html#method-i-compact).
 It removes all `None` elements from the List, returning a copy of the List.
 
 ```py
 from better_python_lists import List
 
 my_list = List([1, None, 2, 3, 4, None, None, 5])
 compact_list = my_list.compact()
-print(compact_list)
-# => [1, 2, 3, 4, 5]
+print(compact_list) # => [1, 2, 3, 4, 5]
 ```
 
 You can also perform in-place compacting using the `compacted` method:
 
 ```py
 print(my_list)  # => [1, None, 2, 3, 4, None, None, 5]
 my_list.compacted()
@@ -48,7 +60,21 @@
 
 ```py
 another_list = List([1, "None", 2, None, 3, "N/A"])
 another_list.compacted(filter_list=[None, "None", "N/A"])
 print(another_list)  # => [1, 2, 3]
 ```
 
+### Flatten
+
+The methods `flatten` and `flattened` flatten an arbitrarily nested List into a
+single-level one.
+
+```py
+nested_list: List = List([["a"], "b", 5, [6, 7, [8, 9, [10]]]])
+flat_list = nested_list.flatten()
+print(flat_list) # => ["a", "b", 5, 6, 7, 8, 9, 10]
+```
+
+As with `compact/compacted`, `flatten` creates a copy of the List, and `flattened`
+performs in-place replacement.
+
```

