# Comparing `tmp/xmodel-0.4.0.tar.gz` & `tmp/xmodel-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "xmodel-0.4.0.tar", max compression
+gzip compressed data, was "xmodel-0.4.1.tar", max compression
```

## Comparing `xmodel-0.4.0.tar` & `xmodel-0.4.1.tar`

### file list

```diff
@@ -1,33 +1,33 @@
--rw-r--r--   0        0        0     1211 2023-05-02 19:24:12.630477 xmodel-0.4.0/LICENSE
--rw-r--r--   0        0        0     1046 2023-05-02 19:24:12.630477 xmodel-0.4.0/README.md
--rw-r--r--   0        0        0     2072 2023-05-02 19:24:12.630477 xmodel-0.4.0/pyproject.toml
--rw-r--r--   0        0        0    20732 2023-05-02 19:24:12.630477 xmodel-0.4.0/xmodel/__init__.py
--rw-r--r--   0        0        0       18 2023-05-02 19:24:12.630477 xmodel-0.4.0/xmodel/_private/__init__.py
--rw-r--r--   0        0        0       33 2023-05-02 19:24:12.630477 xmodel-0.4.0/xmodel/_private/api/__init__.py
--rw-r--r--   0        0        0     7007 2023-05-02 19:24:12.630477 xmodel-0.4.0/xmodel/_private/api/state.py
--rw-r--r--   0        0        0      828 2023-05-02 19:24:12.630477 xmodel-0.4.0/xmodel/_private/api/utils.py
--rw-r--r--   0        0        0      191 2023-05-02 19:24:12.630477 xmodel-0.4.0/xmodel/base/__init__.py
--rw-r--r--   0        0        0    48893 2023-05-02 19:24:12.634477 xmodel-0.4.0/xmodel/base/api.py
--rw-r--r--   0        0        0    35396 2023-05-02 19:24:12.634477 xmodel-0.4.0/xmodel/base/fields.py
--rw-r--r--   0        0        0    31842 2023-05-02 19:24:12.634477 xmodel-0.4.0/xmodel/base/model.py
--rw-r--r--   0        0        0    21759 2023-05-02 19:24:12.634477 xmodel-0.4.0/xmodel/base/structure.py
--rw-r--r--   0        0        0        1 2023-05-02 19:24:12.634477 xmodel-0.4.0/xmodel/common/__init__.py
--rw-r--r--   0        0        0    13348 2023-05-02 19:24:12.634477 xmodel-0.4.0/xmodel/common/children.py
--rw-r--r--   0        0        0     1943 2023-05-02 19:24:12.634477 xmodel-0.4.0/xmodel/common/lazy.py
--rw-r--r--   0        0        0      963 2023-05-02 19:24:12.634477 xmodel-0.4.0/xmodel/common/types.py
--rw-r--r--   0        0        0     1635 2023-05-02 19:24:12.634477 xmodel-0.4.0/xmodel/common/unwrap.py
--rw-r--r--   0        0        0     2555 2023-05-02 19:24:12.634477 xmodel-0.4.0/xmodel/common/utils.py
--rw-r--r--   0        0        0     7716 2023-05-02 19:24:12.634477 xmodel-0.4.0/xmodel/converters.py
--rw-r--r--   0        0        0       89 2023-05-02 19:24:12.634477 xmodel-0.4.0/xmodel/errors.py
--rw-r--r--   0        0        0      801 2023-05-02 19:24:12.634477 xmodel-0.4.0/xmodel/json.py
--rw-r--r--   0        0        0      273 2023-05-02 19:24:12.634477 xmodel-0.4.0/xmodel/remote/__init__.py
--rw-r--r--   0        0        0    30590 2023-05-02 19:24:12.634477 xmodel-0.4.0/xmodel/remote/api.py
--rw-r--r--   0        0        0     7789 2023-05-02 19:24:12.634477 xmodel-0.4.0/xmodel/remote/client.py
--rw-r--r--   0        0        0      301 2023-05-02 19:24:12.634477 xmodel-0.4.0/xmodel/remote/errors.py
--rw-r--r--   0        0        0     2242 2023-05-02 19:24:12.634477 xmodel-0.4.0/xmodel/remote/model.py
--rw-r--r--   0        0        0     3112 2023-05-02 19:24:12.634477 xmodel-0.4.0/xmodel/remote/options.py
--rw-r--r--   0        0        0    12775 2023-05-02 19:24:12.634477 xmodel-0.4.0/xmodel/remote/response_state.py
--rw-r--r--   0        0        0     6709 2023-05-02 19:24:12.634477 xmodel-0.4.0/xmodel/remote/structure.py
--rw-r--r--   0        0        0     7935 2023-05-02 19:24:12.634477 xmodel-0.4.0/xmodel/remote/weak_cache_pool.py
--rw-r--r--   0        0        0      240 2023-05-02 19:24:12.634477 xmodel-0.4.0/xmodel/util.py
--rw-r--r--   0        0        0     2048 1970-01-01 00:00:00.000000 xmodel-0.4.0/PKG-INFO
+-rw-r--r--   0        0        0     1211 2023-05-04 23:48:12.067873 xmodel-0.4.1/LICENSE
+-rw-r--r--   0        0        0     1046 2023-05-04 23:48:12.067873 xmodel-0.4.1/README.md
+-rw-r--r--   0        0        0     2072 2023-05-04 23:48:12.067873 xmodel-0.4.1/pyproject.toml
+-rw-r--r--   0        0        0    20732 2023-05-04 23:48:12.067873 xmodel-0.4.1/xmodel/__init__.py
+-rw-r--r--   0        0        0       18 2023-05-04 23:48:12.067873 xmodel-0.4.1/xmodel/_private/__init__.py
+-rw-r--r--   0        0        0       33 2023-05-04 23:48:12.067873 xmodel-0.4.1/xmodel/_private/api/__init__.py
+-rw-r--r--   0        0        0     7007 2023-05-04 23:48:12.067873 xmodel-0.4.1/xmodel/_private/api/state.py
+-rw-r--r--   0        0        0      828 2023-05-04 23:48:12.067873 xmodel-0.4.1/xmodel/_private/api/utils.py
+-rw-r--r--   0        0        0      191 2023-05-04 23:48:12.067873 xmodel-0.4.1/xmodel/base/__init__.py
+-rw-r--r--   0        0        0    48954 2023-05-04 23:48:12.067873 xmodel-0.4.1/xmodel/base/api.py
+-rw-r--r--   0        0        0    35396 2023-05-04 23:48:12.067873 xmodel-0.4.1/xmodel/base/fields.py
+-rw-r--r--   0        0        0    31842 2023-05-04 23:48:12.067873 xmodel-0.4.1/xmodel/base/model.py
+-rw-r--r--   0        0        0    21759 2023-05-04 23:48:12.067873 xmodel-0.4.1/xmodel/base/structure.py
+-rw-r--r--   0        0        0        1 2023-05-04 23:48:12.067873 xmodel-0.4.1/xmodel/common/__init__.py
+-rw-r--r--   0        0        0    13348 2023-05-04 23:48:12.067873 xmodel-0.4.1/xmodel/common/children.py
+-rw-r--r--   0        0        0     1943 2023-05-04 23:48:12.067873 xmodel-0.4.1/xmodel/common/lazy.py
+-rw-r--r--   0        0        0      963 2023-05-04 23:48:12.067873 xmodel-0.4.1/xmodel/common/types.py
+-rw-r--r--   0        0        0     1635 2023-05-04 23:48:12.067873 xmodel-0.4.1/xmodel/common/unwrap.py
+-rw-r--r--   0        0        0     2555 2023-05-04 23:48:12.071873 xmodel-0.4.1/xmodel/common/utils.py
+-rw-r--r--   0        0        0     7716 2023-05-04 23:48:12.071873 xmodel-0.4.1/xmodel/converters.py
+-rw-r--r--   0        0        0       89 2023-05-04 23:48:12.071873 xmodel-0.4.1/xmodel/errors.py
+-rw-r--r--   0        0        0      801 2023-05-04 23:48:12.071873 xmodel-0.4.1/xmodel/json.py
+-rw-r--r--   0        0        0      273 2023-05-04 23:48:12.071873 xmodel-0.4.1/xmodel/remote/__init__.py
+-rw-r--r--   0        0        0    30590 2023-05-04 23:48:12.071873 xmodel-0.4.1/xmodel/remote/api.py
+-rw-r--r--   0        0        0     7789 2023-05-04 23:48:12.071873 xmodel-0.4.1/xmodel/remote/client.py
+-rw-r--r--   0        0        0      301 2023-05-04 23:48:12.071873 xmodel-0.4.1/xmodel/remote/errors.py
+-rw-r--r--   0        0        0     2242 2023-05-04 23:48:12.071873 xmodel-0.4.1/xmodel/remote/model.py
+-rw-r--r--   0        0        0     3112 2023-05-04 23:48:12.071873 xmodel-0.4.1/xmodel/remote/options.py
+-rw-r--r--   0        0        0    12775 2023-05-04 23:48:12.071873 xmodel-0.4.1/xmodel/remote/response_state.py
+-rw-r--r--   0        0        0     6709 2023-05-04 23:48:12.071873 xmodel-0.4.1/xmodel/remote/structure.py
+-rw-r--r--   0        0        0     7935 2023-05-04 23:48:12.071873 xmodel-0.4.1/xmodel/remote/weak_cache_pool.py
+-rw-r--r--   0        0        0      240 2023-05-04 23:48:12.071873 xmodel-0.4.1/xmodel/util.py
+-rw-r--r--   0        0        0     2048 1970-01-01 00:00:00.000000 xmodel-0.4.1/PKG-INFO
```

### Comparing `xmodel-0.4.0/LICENSE` & `xmodel-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `xmodel-0.4.0/README.md` & `xmodel-0.4.1/README.md`

 * *Files identical despite different names*

### Comparing `xmodel-0.4.0/pyproject.toml` & `xmodel-0.4.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "xmodel"
-version = "0.4.0"
+version = "0.4.1"
 description = "Models for working with JSON, ie: JsonModel"
 authors = ["Josh Orr <josh@orr.blue>"]
 packages = [{include = "xmodel"}]
 readme = "README.md"
 repository = "https://github.com/xyngular/py-xmodel"
 classifiers = [
     "Topic :: Software Development :: Libraries :: Python Modules",
```

### Comparing `xmodel-0.4.0/xmodel/__init__.py` & `xmodel-0.4.1/xmodel/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -496,8 +496,8 @@
     'BaseStructure',
     'Field',
     'Converter',
     'XModelError',
     'JsonModel'
 ]
 
-__version__ = '0.4.0'
+__version__ = '0.4.1'
```

### Comparing `xmodel-0.4.0/xmodel/_private/api/state.py` & `xmodel-0.4.1/xmodel/_private/api/state.py`

 * *Files identical despite different names*

### Comparing `xmodel-0.4.0/xmodel/_private/api/utils.py` & `xmodel-0.4.1/xmodel/_private/api/utils.py`

 * *Files identical despite different names*

### Comparing `xmodel-0.4.0/xmodel/base/api.py` & `xmodel-0.4.1/xmodel/base/api.py`

 * *Files 0% similar despite different names*

```diff
@@ -376,14 +376,15 @@
 
         if not api:
             assert not model, "You can't pass in a model without an associated api/model obj."
 
         if model:
             # If we have a model, the structure should be exactly the same as it's BaseModel type.
             self._structure = api.structure
+            self.default_converters = api.default_converters
             self._api_state = PrivateApiState(model=model)
             return
 
         # If We don't have a BaseModel, then we need to copy the structure, it could change
         # because we are being allocated for a new BaseModel type at the class/type level;
         # this means we are not associated with a specific BaseModel instance, only a BaseModel
         # type.
```

### Comparing `xmodel-0.4.0/xmodel/base/fields.py` & `xmodel-0.4.1/xmodel/base/fields.py`

 * *Files identical despite different names*

### Comparing `xmodel-0.4.0/xmodel/base/model.py` & `xmodel-0.4.1/xmodel/base/model.py`

 * *Files identical despite different names*

### Comparing `xmodel-0.4.0/xmodel/base/structure.py` & `xmodel-0.4.1/xmodel/base/structure.py`

 * *Files identical despite different names*

### Comparing `xmodel-0.4.0/xmodel/common/children.py` & `xmodel-0.4.1/xmodel/common/children.py`

 * *Files identical despite different names*

### Comparing `xmodel-0.4.0/xmodel/common/lazy.py` & `xmodel-0.4.1/xmodel/common/lazy.py`

 * *Files identical despite different names*

### Comparing `xmodel-0.4.0/xmodel/common/types.py` & `xmodel-0.4.1/xmodel/common/types.py`

 * *Files identical despite different names*

### Comparing `xmodel-0.4.0/xmodel/common/unwrap.py` & `xmodel-0.4.1/xmodel/common/unwrap.py`

 * *Files identical despite different names*

### Comparing `xmodel-0.4.0/xmodel/common/utils.py` & `xmodel-0.4.1/xmodel/common/utils.py`

 * *Files identical despite different names*

### Comparing `xmodel-0.4.0/xmodel/converters.py` & `xmodel-0.4.1/xmodel/converters.py`

 * *Files identical despite different names*

### Comparing `xmodel-0.4.0/xmodel/json.py` & `xmodel-0.4.1/xmodel/json.py`

 * *Files identical despite different names*

### Comparing `xmodel-0.4.0/xmodel/remote/api.py` & `xmodel-0.4.1/xmodel/remote/api.py`

 * *Files identical despite different names*

### Comparing `xmodel-0.4.0/xmodel/remote/client.py` & `xmodel-0.4.1/xmodel/remote/client.py`

 * *Files identical despite different names*

### Comparing `xmodel-0.4.0/xmodel/remote/model.py` & `xmodel-0.4.1/xmodel/remote/model.py`

 * *Files identical despite different names*

### Comparing `xmodel-0.4.0/xmodel/remote/options.py` & `xmodel-0.4.1/xmodel/remote/options.py`

 * *Files identical despite different names*

### Comparing `xmodel-0.4.0/xmodel/remote/response_state.py` & `xmodel-0.4.1/xmodel/remote/response_state.py`

 * *Files identical despite different names*

### Comparing `xmodel-0.4.0/xmodel/remote/structure.py` & `xmodel-0.4.1/xmodel/remote/structure.py`

 * *Files identical despite different names*

### Comparing `xmodel-0.4.0/xmodel/remote/weak_cache_pool.py` & `xmodel-0.4.1/xmodel/remote/weak_cache_pool.py`

 * *Files identical despite different names*

### Comparing `xmodel-0.4.0/PKG-INFO` & `xmodel-0.4.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: xmodel
-Version: 0.4.0
+Version: 0.4.1
 Summary: Models for working with JSON, ie: JsonModel
 Home-page: https://github.com/xyngular/py-xmodel
 Author: Josh Orr
 Author-email: josh@orr.blue
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: The Unlicense (Unlicense)
 Classifier: Programming Language :: Python :: 3
```

