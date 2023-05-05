# Comparing `tmp/abi3info-2023.3.20a1.tar.gz` & `tmp/abi3info-2023.5.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "abi3info-2023.3.20a1.tar", last modified: Tue Mar 21 03:12:49 2023, max compression
+gzip compressed data, was "abi3info-2023.5.4.tar", last modified: Fri May  5 02:06:22 2023, max compression
```

## Comparing `abi3info-2023.3.20a1.tar` & `abi3info-2023.5.4.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1109 2023-03-21 03:12:38.982198 abi3info-2023.3.20a1/LICENSE
--rw-r--r--   0        0        0     1915 2023-03-21 03:12:38.982198 abi3info-2023.3.20a1/README.md
--rw-r--r--   0        0        0     1040 2023-03-21 03:12:38.982198 abi3info-2023.3.20a1/abi3info/__init__.py
--rw-r--r--   0        0        0   189123 2023-03-21 03:12:38.986199 abi3info-2023.3.20a1/abi3info/_internal.py
--rw-r--r--   0        0        0     7791 2023-03-21 03:12:38.986199 abi3info-2023.3.20a1/abi3info/models.py
--rw-r--r--   0        0        0     1885 2023-03-21 03:12:38.986199 abi3info-2023.3.20a1/pyproject.toml
--rw-r--r--   0        0        0     3464 1970-01-01 00:00:00.000000 abi3info-2023.3.20a1/PKG-INFO
+-rw-r--r--   0        0        0     1109 2023-05-05 02:06:06.677518 abi3info-2023.5.4/LICENSE
+-rw-r--r--   0        0        0     1915 2023-05-05 02:06:06.677518 abi3info-2023.5.4/README.md
+-rw-r--r--   0        0        0     1038 2023-05-05 02:06:06.677518 abi3info-2023.5.4/abi3info/__init__.py
+-rw-r--r--   0        0        0   189739 2023-05-05 02:06:06.677518 abi3info-2023.5.4/abi3info/_internal.py
+-rw-r--r--   0        0        0     7791 2023-05-05 02:06:06.677518 abi3info-2023.5.4/abi3info/models.py
+-rw-r--r--   0        0        0     1885 2023-05-05 02:06:06.677518 abi3info-2023.5.4/pyproject.toml
+-rw-r--r--   0        0        0     3461 1970-01-01 00:00:00.000000 abi3info-2023.5.4/PKG-INFO
```

### Comparing `abi3info-2023.3.20a1/LICENSE` & `abi3info-2023.5.4/LICENSE`

 * *Files identical despite different names*

### Comparing `abi3info-2023.3.20a1/README.md` & `abi3info-2023.5.4/README.md`

 * *Files identical despite different names*

### Comparing `abi3info-2023.3.20a1/abi3info/__init__.py` & `abi3info-2023.5.4/abi3info/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -20,15 +20,15 @@
     Function,
     Macro,
     Struct,
     Symbol,
     Typedef,
 )
 
-__version__ = "2023.03.20a1"
+__version__ = "2023.05.04"
 """
 The current version of abi3info.
 """
 
 DATAS: Final[dict[Symbol, Data]] = _DATAS
 """
 Data object members of the limited API and stable ABI.
```

### Comparing `abi3info-2023.3.20a1/abi3info/_internal.py` & `abi3info-2023.5.4/abi3info/_internal.py`

 * *Files 0% similar despite different names*

```diff
@@ -4421,14 +4421,26 @@
     ),
     Symbol(name="PyObject_VectorcallMethod"): Function(
         symbol=Symbol(name="PyObject_VectorcallMethod"),
         added=PyVersion(major=3, minor=12),
         ifdef=None,
         abi_only=False,
     ),
+    Symbol(name="PyObject_GetTypeData"): Function(
+        symbol=Symbol(name="PyObject_GetTypeData"),
+        added=PyVersion(major=3, minor=12),
+        ifdef=None,
+        abi_only=False,
+    ),
+    Symbol(name="PyType_GetTypeDataSize"): Function(
+        symbol=Symbol(name="PyType_GetTypeDataSize"),
+        added=PyVersion(major=3, minor=12),
+        ifdef=None,
+        abi_only=False,
+    ),
 }
 _MACROS: Final[dict[str, Macro]] = {
     "Py_tp_dealloc": Macro(name="Py_tp_dealloc", added=PyVersion(major=3, minor=2)),
     "Py_tp_getattr": Macro(name="Py_tp_getattr", added=PyVersion(major=3, minor=2)),
     "Py_tp_setattr": Macro(name="Py_tp_setattr", added=PyVersion(major=3, minor=2)),
     "Py_tp_repr": Macro(name="Py_tp_repr", added=PyVersion(major=3, minor=2)),
     "Py_tp_hash": Macro(name="Py_tp_hash", added=PyVersion(major=3, minor=2)),
@@ -4571,14 +4583,18 @@
     "Py_T_BOOL": Macro(name="Py_T_BOOL", added=PyVersion(major=3, minor=12)),
     "Py_T_STRING": Macro(name="Py_T_STRING", added=PyVersion(major=3, minor=12)),
     "Py_T_STRING_INPLACE": Macro(name="Py_T_STRING_INPLACE", added=PyVersion(major=3, minor=12)),
     "Py_T_CHAR": Macro(name="Py_T_CHAR", added=PyVersion(major=3, minor=12)),
     "Py_T_OBJECT_EX": Macro(name="Py_T_OBJECT_EX", added=PyVersion(major=3, minor=12)),
     "Py_READONLY": Macro(name="Py_READONLY", added=PyVersion(major=3, minor=12)),
     "Py_AUDIT_READ": Macro(name="Py_AUDIT_READ", added=PyVersion(major=3, minor=12)),
+    "Py_RELATIVE_OFFSET": Macro(name="Py_RELATIVE_OFFSET", added=PyVersion(major=3, minor=12)),
+    "Py_TPFLAGS_ITEMS_AT_END": Macro(
+        name="Py_TPFLAGS_ITEMS_AT_END", added=PyVersion(major=3, minor=12)
+    ),
     "Py_BEGIN_ALLOW_THREADS": Macro(
         name="Py_BEGIN_ALLOW_THREADS", added=PyVersion(major=3, minor=2)
     ),
     "Py_BLOCK_THREADS": Macro(name="Py_BLOCK_THREADS", added=PyVersion(major=3, minor=2)),
     "Py_UNBLOCK_THREADS": Macro(name="Py_UNBLOCK_THREADS", added=PyVersion(major=3, minor=2)),
     "Py_END_ALLOW_THREADS": Macro(name="Py_END_ALLOW_THREADS", added=PyVersion(major=3, minor=2)),
     "PY_VECTORCALL_ARGUMENTS_OFFSET": Macro(
```

### Comparing `abi3info-2023.3.20a1/abi3info/models.py` & `abi3info-2023.5.4/abi3info/models.py`

 * *Files identical despite different names*

### Comparing `abi3info-2023.3.20a1/pyproject.toml` & `abi3info-2023.5.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `abi3info-2023.3.20a1/PKG-INFO` & `abi3info-2023.5.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: abi3info
-Version: 2023.3.20a1
+Version: 2023.5.4
 Summary: A library for abi3 and other CPython API information
 Author-email: William Woodruff <william@yossarian.net>
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3 :: Only
 Classifier: Programming Language :: Python :: 3
```

