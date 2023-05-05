# Comparing `tmp/nvcl-kit-1.1.0.tar.gz` & `tmp/nvcl-kit-1.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "nvcl-kit-1.1.0.tar", last modified: Fri May  5 06:33:24 2023, max compression
+gzip compressed data, was "nvcl-kit-1.1.2.tar", last modified: Fri May  5 06:55:16 2023, max compression
```

## Comparing `nvcl-kit-1.1.0.tar` & `nvcl-kit-1.1.2.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0     3915 2023-05-05 06:32:59.261547 nvcl-kit-1.1.0/LICENSE
--rw-r--r--   0        0        0     2823 2023-05-05 06:32:59.261547 nvcl-kit-1.1.0/README.md
--rw-r--r--   0        0        0       14 2023-05-05 06:32:59.406561 nvcl-kit-1.1.0/nvcl_kit/__init__.py
--rw-r--r--   0        0        0     5048 2023-05-05 06:32:59.406561 nvcl-kit-1.1.0/nvcl_kit/constants.py
--rw-r--r--   0        0        0     4386 2023-05-05 06:32:59.406561 nvcl-kit-1.1.0/nvcl_kit/generators.py
--rw-r--r--   0        0        0     5379 2023-05-05 06:32:59.406561 nvcl-kit-1.1.0/nvcl_kit/param_builder.py
--rw-r--r--   0        0        0    40851 2023-05-05 06:32:59.406561 nvcl-kit-1.1.0/nvcl_kit/reader.py
--rw-r--r--   0        0        0    14878 2023-05-05 06:32:59.406561 nvcl-kit-1.1.0/nvcl_kit/svc_interface.py
--rw-r--r--   0        0        0    10805 2023-05-05 06:32:59.406561 nvcl-kit-1.1.0/nvcl_kit/wfs_helpers.py
--rw-r--r--   0        0        0      360 2023-05-05 06:32:59.407561 nvcl-kit-1.1.0/nvcl_kit/xml_helpers.py
--rw-r--r--   0        0        0     1039 2023-05-05 06:32:59.407561 nvcl-kit-1.1.0/pyproject.toml
--rw-r--r--   0        0        0     3584 1970-01-01 00:00:00.000000 nvcl-kit-1.1.0/PKG-INFO
+-rw-r--r--   0        0        0     3915 2023-05-05 06:54:51.969808 nvcl-kit-1.1.2/LICENSE
+-rw-r--r--   0        0        0     2823 2023-05-05 06:54:51.969808 nvcl-kit-1.1.2/README.md
+-rw-r--r--   0        0        0       14 2023-05-05 06:54:51.988810 nvcl-kit-1.1.2/nvcl_kit/__init__.py
+-rw-r--r--   0        0        0     5048 2023-05-05 06:54:51.989810 nvcl-kit-1.1.2/nvcl_kit/constants.py
+-rw-r--r--   0        0        0     4386 2023-05-05 06:54:51.989810 nvcl-kit-1.1.2/nvcl_kit/generators.py
+-rw-r--r--   0        0        0     5379 2023-05-05 06:54:51.989810 nvcl-kit-1.1.2/nvcl_kit/param_builder.py
+-rw-r--r--   0        0        0    40851 2023-05-05 06:54:51.989810 nvcl-kit-1.1.2/nvcl_kit/reader.py
+-rw-r--r--   0        0        0    14878 2023-05-05 06:54:51.989810 nvcl-kit-1.1.2/nvcl_kit/svc_interface.py
+-rw-r--r--   0        0        0    10805 2023-05-05 06:54:51.989810 nvcl-kit-1.1.2/nvcl_kit/wfs_helpers.py
+-rw-r--r--   0        0        0      360 2023-05-05 06:54:51.989810 nvcl-kit-1.1.2/nvcl_kit/xml_helpers.py
+-rw-r--r--   0        0        0     1039 2023-05-05 06:54:51.990810 nvcl-kit-1.1.2/pyproject.toml
+-rw-r--r--   0        0        0     3584 1970-01-01 00:00:00.000000 nvcl-kit-1.1.2/PKG-INFO
```

### Comparing `nvcl-kit-1.1.0/LICENSE` & `nvcl-kit-1.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `nvcl-kit-1.1.0/README.md` & `nvcl-kit-1.1.2/README.md`

 * *Files identical despite different names*

### Comparing `nvcl-kit-1.1.0/nvcl_kit/constants.py` & `nvcl-kit-1.1.2/nvcl_kit/constants.py`

 * *Files identical despite different names*

### Comparing `nvcl-kit-1.1.0/nvcl_kit/generators.py` & `nvcl-kit-1.1.2/nvcl_kit/generators.py`

 * *Files identical despite different names*

### Comparing `nvcl-kit-1.1.0/nvcl_kit/param_builder.py` & `nvcl-kit-1.1.2/nvcl_kit/param_builder.py`

 * *Files identical despite different names*

### Comparing `nvcl-kit-1.1.0/nvcl_kit/reader.py` & `nvcl-kit-1.1.2/nvcl_kit/reader.py`

 * *Files identical despite different names*

### Comparing `nvcl-kit-1.1.0/nvcl_kit/svc_interface.py` & `nvcl-kit-1.1.2/nvcl_kit/svc_interface.py`

 * *Files identical despite different names*

### Comparing `nvcl-kit-1.1.0/nvcl_kit/wfs_helpers.py` & `nvcl-kit-1.1.2/nvcl_kit/wfs_helpers.py`

 * *Files identical despite different names*

### Comparing `nvcl-kit-1.1.0/pyproject.toml` & `nvcl-kit-1.1.2/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 [tool.pdm]
 
 [project]
 name = "nvcl_kit"
-version = "1.1.0"
+version = "1.1.2"
 description = "Downloads Australian NVCL datasets"
 authors = [
     { name = "Vincent Fazio", email = "vincent.fazio@csiro.au" },
 ]
 dependencies = [
     "owslib==0.28.1",
     "shapely~=2.0",
```

### Comparing `nvcl-kit-1.1.0/PKG-INFO` & `nvcl-kit-1.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nvcl_kit
-Version: 1.1.0
+Version: 1.1.2
 Summary: Downloads Australian NVCL datasets
 License: CSIRO BSD/MIT
 Author-email: Vincent Fazio <vincent.fazio@csiro.au>
 Requires-Python: >=3.7
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
```

