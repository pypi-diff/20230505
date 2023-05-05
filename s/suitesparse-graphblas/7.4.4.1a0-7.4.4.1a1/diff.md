# Comparing `tmp/suitesparse-graphblas-7.4.4.1a0.tar.gz` & `tmp/suitesparse-graphblas-7.4.4.1a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "suitesparse-graphblas-7.4.4.1a0.tar", last modified: Wed May  3 19:51:53 2023, max compression
+gzip compressed data, was "suitesparse-graphblas-7.4.4.1a1.tar", last modified: Fri May  5 02:04:24 2023, max compression
```

## Comparing `suitesparse-graphblas-7.4.4.1a0.tar` & `suitesparse-graphblas-7.4.4.1a1.tar`

### file list

```diff
@@ -1,42 +1,42 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 19:51:53.126165 suitesparse-graphblas-7.4.4.1a0/
--rw-r--r--   0 runner    (1001) docker     (123)    11372 2023-05-03 19:51:34.000000 suitesparse-graphblas-7.4.4.1a0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      223 2023-05-03 19:51:34.000000 suitesparse-graphblas-7.4.4.1a0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    16883 2023-05-03 19:51:53.126165 suitesparse-graphblas-7.4.4.1a0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2032 2023-05-03 19:51:34.000000 suitesparse-graphblas-7.4.4.1a0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     3014 2023-05-03 19:51:34.000000 suitesparse-graphblas-7.4.4.1a0/build_graphblas_cffi.py
--rw-r--r--   0 runner    (1001) docker     (123)     3343 2023-05-03 19:51:34.000000 suitesparse-graphblas-7.4.4.1a0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-03 19:51:53.126165 suitesparse-graphblas-7.4.4.1a0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2388 2023-05-03 19:51:34.000000 suitesparse-graphblas-7.4.4.1a0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 19:51:53.122166 suitesparse-graphblas-7.4.4.1a0/suitesparse_graphblas/
--rw-r--r--   0 runner    (1001) docker     (123)     9276 2023-05-03 19:51:34.000000 suitesparse-graphblas-7.4.4.1a0/suitesparse_graphblas/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    28334 2023-05-03 19:51:34.000000 suitesparse-graphblas-7.4.4.1a0/suitesparse_graphblas/create_headers.py
--rw-r--r--   0 runner    (1001) docker     (123)      832 2023-05-03 19:51:34.000000 suitesparse-graphblas-7.4.4.1a0/suitesparse_graphblas/exceptions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 19:51:53.126165 suitesparse-graphblas-7.4.4.1a0/suitesparse_graphblas/io/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 19:51:34.000000 suitesparse-graphblas-7.4.4.1a0/suitesparse_graphblas/io/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    16442 2023-05-03 19:51:34.000000 suitesparse-graphblas-7.4.4.1a0/suitesparse_graphblas/io/binary.py
--rw-r--r--   0 runner    (1001) docker     (123)     5008 2023-05-03 19:51:34.000000 suitesparse-graphblas-7.4.4.1a0/suitesparse_graphblas/io/serialize.py
--rw-r--r--   0 runner    (1001) docker     (123)     5244 2023-05-03 19:51:34.000000 suitesparse-graphblas-7.4.4.1a0/suitesparse_graphblas/matrix.py
--rw-r--r--   0 runner    (1001) docker     (123)     1456 2023-05-03 19:51:34.000000 suitesparse-graphblas-7.4.4.1a0/suitesparse_graphblas/scalar.py
--rw-r--r--   0 runner    (1001) docker     (123)      402 2023-05-03 19:51:34.000000 suitesparse-graphblas-7.4.4.1a0/suitesparse_graphblas/source.c
--rw-r--r--   0 runner    (1001) docker     (123)   199175 2023-05-03 19:51:34.000000 suitesparse-graphblas-7.4.4.1a0/suitesparse_graphblas/suitesparse_graphblas.h
--rw-r--r--   0 runner    (1001) docker     (123)   199175 2023-05-03 19:51:34.000000 suitesparse-graphblas-7.4.4.1a0/suitesparse_graphblas/suitesparse_graphblas_arm64.h
--rw-r--r--   0 runner    (1001) docker     (123)   184310 2023-05-03 19:51:34.000000 suitesparse-graphblas-7.4.4.1a0/suitesparse_graphblas/suitesparse_graphblas_no_complex.h
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 19:51:53.126165 suitesparse-graphblas-7.4.4.1a0/suitesparse_graphblas/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-03 19:51:34.000000 suitesparse-graphblas-7.4.4.1a0/suitesparse_graphblas/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      165 2023-05-03 19:51:34.000000 suitesparse-graphblas-7.4.4.1a0/suitesparse_graphblas/tests/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)      259 2023-05-03 19:51:34.000000 suitesparse-graphblas-7.4.4.1a0/suitesparse_graphblas/tests/test_doctest.py
--rw-r--r--   0 runner    (1001) docker     (123)      370 2023-05-03 19:51:34.000000 suitesparse-graphblas-7.4.4.1a0/suitesparse_graphblas/tests/test_exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)      299 2023-05-03 19:51:34.000000 suitesparse-graphblas-7.4.4.1a0/suitesparse_graphblas/tests/test_initialize.py
--rw-r--r--   0 runner    (1001) docker     (123)     6307 2023-05-03 19:51:34.000000 suitesparse-graphblas-7.4.4.1a0/suitesparse_graphblas/tests/test_io.py
--rw-r--r--   0 runner    (1001) docker     (123)      238 2023-05-03 19:51:34.000000 suitesparse-graphblas-7.4.4.1a0/suitesparse_graphblas/tests/test_package.py
--rw-r--r--   0 runner    (1001) docker     (123)      385 2023-05-03 19:51:34.000000 suitesparse-graphblas-7.4.4.1a0/suitesparse_graphblas/tests/test_scalar.py
--rw-r--r--   0 runner    (1001) docker     (123)   334342 2023-05-03 19:51:50.000000 suitesparse-graphblas-7.4.4.1a0/suitesparse_graphblas/utils.c
--rw-r--r--   0 runner    (1001) docker     (123)     1408 2023-05-03 19:51:34.000000 suitesparse-graphblas-7.4.4.1a0/suitesparse_graphblas/utils.pxd
--rw-r--r--   0 runner    (1001) docker     (123)     2898 2023-05-03 19:51:34.000000 suitesparse-graphblas-7.4.4.1a0/suitesparse_graphblas/utils.pyx
--rw-r--r--   0 runner    (1001) docker     (123)     2288 2023-05-03 19:51:34.000000 suitesparse-graphblas-7.4.4.1a0/suitesparse_graphblas/vector.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-03 19:51:53.126165 suitesparse-graphblas-7.4.4.1a0/suitesparse_graphblas.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    16883 2023-05-03 19:51:53.000000 suitesparse-graphblas-7.4.4.1a0/suitesparse_graphblas.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1241 2023-05-03 19:51:53.000000 suitesparse-graphblas-7.4.4.1a0/suitesparse_graphblas.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-03 19:51:53.000000 suitesparse-graphblas-7.4.4.1a0/suitesparse_graphblas.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-03 19:51:53.000000 suitesparse-graphblas-7.4.4.1a0/suitesparse_graphblas.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-03 19:51:53.000000 suitesparse-graphblas-7.4.4.1a0/suitesparse_graphblas.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 02:04:24.017196 suitesparse-graphblas-7.4.4.1a1/
+-rw-r--r--   0 runner    (1001) docker     (123)    11372 2023-05-05 02:03:52.000000 suitesparse-graphblas-7.4.4.1a1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      223 2023-05-05 02:03:52.000000 suitesparse-graphblas-7.4.4.1a1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    16883 2023-05-05 02:04:24.013196 suitesparse-graphblas-7.4.4.1a1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2032 2023-05-05 02:03:52.000000 suitesparse-graphblas-7.4.4.1a1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     3014 2023-05-05 02:03:52.000000 suitesparse-graphblas-7.4.4.1a1/build_graphblas_cffi.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3343 2023-05-05 02:03:52.000000 suitesparse-graphblas-7.4.4.1a1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-05 02:04:24.017196 suitesparse-graphblas-7.4.4.1a1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2388 2023-05-05 02:03:52.000000 suitesparse-graphblas-7.4.4.1a1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 02:04:24.013196 suitesparse-graphblas-7.4.4.1a1/suitesparse_graphblas/
+-rw-r--r--   0 runner    (1001) docker     (123)     9276 2023-05-05 02:03:52.000000 suitesparse-graphblas-7.4.4.1a1/suitesparse_graphblas/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    28334 2023-05-05 02:03:52.000000 suitesparse-graphblas-7.4.4.1a1/suitesparse_graphblas/create_headers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      832 2023-05-05 02:03:52.000000 suitesparse-graphblas-7.4.4.1a1/suitesparse_graphblas/exceptions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 02:04:24.013196 suitesparse-graphblas-7.4.4.1a1/suitesparse_graphblas/io/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 02:03:52.000000 suitesparse-graphblas-7.4.4.1a1/suitesparse_graphblas/io/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16442 2023-05-05 02:03:52.000000 suitesparse-graphblas-7.4.4.1a1/suitesparse_graphblas/io/binary.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5008 2023-05-05 02:03:52.000000 suitesparse-graphblas-7.4.4.1a1/suitesparse_graphblas/io/serialize.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5244 2023-05-05 02:03:52.000000 suitesparse-graphblas-7.4.4.1a1/suitesparse_graphblas/matrix.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1456 2023-05-05 02:03:52.000000 suitesparse-graphblas-7.4.4.1a1/suitesparse_graphblas/scalar.py
+-rw-r--r--   0 runner    (1001) docker     (123)      402 2023-05-05 02:03:52.000000 suitesparse-graphblas-7.4.4.1a1/suitesparse_graphblas/source.c
+-rw-r--r--   0 runner    (1001) docker     (123)   199175 2023-05-05 02:03:52.000000 suitesparse-graphblas-7.4.4.1a1/suitesparse_graphblas/suitesparse_graphblas.h
+-rw-r--r--   0 runner    (1001) docker     (123)   199175 2023-05-05 02:03:52.000000 suitesparse-graphblas-7.4.4.1a1/suitesparse_graphblas/suitesparse_graphblas_arm64.h
+-rw-r--r--   0 runner    (1001) docker     (123)   184310 2023-05-05 02:03:52.000000 suitesparse-graphblas-7.4.4.1a1/suitesparse_graphblas/suitesparse_graphblas_no_complex.h
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 02:04:24.013196 suitesparse-graphblas-7.4.4.1a1/suitesparse_graphblas/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 02:03:52.000000 suitesparse-graphblas-7.4.4.1a1/suitesparse_graphblas/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      165 2023-05-05 02:03:52.000000 suitesparse-graphblas-7.4.4.1a1/suitesparse_graphblas/tests/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      259 2023-05-05 02:03:52.000000 suitesparse-graphblas-7.4.4.1a1/suitesparse_graphblas/tests/test_doctest.py
+-rw-r--r--   0 runner    (1001) docker     (123)      370 2023-05-05 02:03:52.000000 suitesparse-graphblas-7.4.4.1a1/suitesparse_graphblas/tests/test_exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      299 2023-05-05 02:03:52.000000 suitesparse-graphblas-7.4.4.1a1/suitesparse_graphblas/tests/test_initialize.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6307 2023-05-05 02:03:52.000000 suitesparse-graphblas-7.4.4.1a1/suitesparse_graphblas/tests/test_io.py
+-rw-r--r--   0 runner    (1001) docker     (123)      238 2023-05-05 02:03:52.000000 suitesparse-graphblas-7.4.4.1a1/suitesparse_graphblas/tests/test_package.py
+-rw-r--r--   0 runner    (1001) docker     (123)      385 2023-05-05 02:03:52.000000 suitesparse-graphblas-7.4.4.1a1/suitesparse_graphblas/tests/test_scalar.py
+-rw-r--r--   0 runner    (1001) docker     (123)   334342 2023-05-05 02:04:21.000000 suitesparse-graphblas-7.4.4.1a1/suitesparse_graphblas/utils.c
+-rw-r--r--   0 runner    (1001) docker     (123)     1408 2023-05-05 02:03:52.000000 suitesparse-graphblas-7.4.4.1a1/suitesparse_graphblas/utils.pxd
+-rw-r--r--   0 runner    (1001) docker     (123)     2898 2023-05-05 02:03:52.000000 suitesparse-graphblas-7.4.4.1a1/suitesparse_graphblas/utils.pyx
+-rw-r--r--   0 runner    (1001) docker     (123)     2288 2023-05-05 02:03:52.000000 suitesparse-graphblas-7.4.4.1a1/suitesparse_graphblas/vector.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 02:04:24.013196 suitesparse-graphblas-7.4.4.1a1/suitesparse_graphblas.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    16883 2023-05-05 02:04:24.000000 suitesparse-graphblas-7.4.4.1a1/suitesparse_graphblas.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1241 2023-05-05 02:04:24.000000 suitesparse-graphblas-7.4.4.1a1/suitesparse_graphblas.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 02:04:24.000000 suitesparse-graphblas-7.4.4.1a1/suitesparse_graphblas.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-05 02:04:24.000000 suitesparse-graphblas-7.4.4.1a1/suitesparse_graphblas.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-05 02:04:24.000000 suitesparse-graphblas-7.4.4.1a1/suitesparse_graphblas.egg-info/top_level.txt
```

### Comparing `suitesparse-graphblas-7.4.4.1a0/LICENSE` & `suitesparse-graphblas-7.4.4.1a1/LICENSE`

 * *Files identical despite different names*

### Comparing `suitesparse-graphblas-7.4.4.1a0/PKG-INFO` & `suitesparse-graphblas-7.4.4.1a1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: suitesparse-graphblas
-Version: 7.4.4.1a0
+Version: 7.4.4.1a1
 Summary: SuiteSparse:GraphBLAS Python bindings.
 Author: Jim Kitchen, Michel Pelletier, suitesparse-graphblas contributors
 Author-email: Erik Welch <erik.n.welch@gmail.com>
 Maintainer-email: Erik Welch <erik.n.welch@gmail.com>, Jim Kitchen <jim22k@gmail.com>, Michel Pelletier <michel@graphegon.com>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
```

### Comparing `suitesparse-graphblas-7.4.4.1a0/README.md` & `suitesparse-graphblas-7.4.4.1a1/README.md`

 * *Files identical despite different names*

### Comparing `suitesparse-graphblas-7.4.4.1a0/build_graphblas_cffi.py` & `suitesparse-graphblas-7.4.4.1a1/build_graphblas_cffi.py`

 * *Files identical despite different names*

### Comparing `suitesparse-graphblas-7.4.4.1a0/pyproject.toml` & `suitesparse-graphblas-7.4.4.1a1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `suitesparse-graphblas-7.4.4.1a0/setup.py` & `suitesparse-graphblas-7.4.4.1a1/setup.py`

 * *Files identical despite different names*

### Comparing `suitesparse-graphblas-7.4.4.1a0/suitesparse_graphblas/__init__.py` & `suitesparse-graphblas-7.4.4.1a1/suitesparse_graphblas/__init__.py`

 * *Files identical despite different names*

### Comparing `suitesparse-graphblas-7.4.4.1a0/suitesparse_graphblas/create_headers.py` & `suitesparse-graphblas-7.4.4.1a1/suitesparse_graphblas/create_headers.py`

 * *Files identical despite different names*

### Comparing `suitesparse-graphblas-7.4.4.1a0/suitesparse_graphblas/exceptions.py` & `suitesparse-graphblas-7.4.4.1a1/suitesparse_graphblas/exceptions.py`

 * *Files identical despite different names*

### Comparing `suitesparse-graphblas-7.4.4.1a0/suitesparse_graphblas/io/binary.py` & `suitesparse-graphblas-7.4.4.1a1/suitesparse_graphblas/io/binary.py`

 * *Files identical despite different names*

### Comparing `suitesparse-graphblas-7.4.4.1a0/suitesparse_graphblas/io/serialize.py` & `suitesparse-graphblas-7.4.4.1a1/suitesparse_graphblas/io/serialize.py`

 * *Files identical despite different names*

### Comparing `suitesparse-graphblas-7.4.4.1a0/suitesparse_graphblas/matrix.py` & `suitesparse-graphblas-7.4.4.1a1/suitesparse_graphblas/matrix.py`

 * *Files identical despite different names*

### Comparing `suitesparse-graphblas-7.4.4.1a0/suitesparse_graphblas/scalar.py` & `suitesparse-graphblas-7.4.4.1a1/suitesparse_graphblas/scalar.py`

 * *Files identical despite different names*

### Comparing `suitesparse-graphblas-7.4.4.1a0/suitesparse_graphblas/suitesparse_graphblas.h` & `suitesparse-graphblas-7.4.4.1a1/suitesparse_graphblas/suitesparse_graphblas.h`

 * *Files identical despite different names*

### Comparing `suitesparse-graphblas-7.4.4.1a0/suitesparse_graphblas/suitesparse_graphblas_arm64.h` & `suitesparse-graphblas-7.4.4.1a1/suitesparse_graphblas/suitesparse_graphblas_arm64.h`

 * *Files identical despite different names*

### Comparing `suitesparse-graphblas-7.4.4.1a0/suitesparse_graphblas/suitesparse_graphblas_no_complex.h` & `suitesparse-graphblas-7.4.4.1a1/suitesparse_graphblas/suitesparse_graphblas_no_complex.h`

 * *Files identical despite different names*

### Comparing `suitesparse-graphblas-7.4.4.1a0/suitesparse_graphblas/tests/test_io.py` & `suitesparse-graphblas-7.4.4.1a1/suitesparse_graphblas/tests/test_io.py`

 * *Files identical despite different names*

### Comparing `suitesparse-graphblas-7.4.4.1a0/suitesparse_graphblas/utils.c` & `suitesparse-graphblas-7.4.4.1a1/suitesparse_graphblas/utils.c`

 * *Files 0% similar despite different names*

```diff
@@ -6,23 +6,23 @@
         "define_macros": [
             [
                 "NPY_NO_DEPRECATED_API",
                 "NPY_1_7_API_VERSION"
             ]
         ],
         "depends": [
-            "/tmp/build-env-nn5jlqfo/lib/python3.10/site-packages/numpy/core/include/numpy/arrayobject.h",
-            "/tmp/build-env-nn5jlqfo/lib/python3.10/site-packages/numpy/core/include/numpy/arrayscalars.h",
-            "/tmp/build-env-nn5jlqfo/lib/python3.10/site-packages/numpy/core/include/numpy/ndarrayobject.h",
-            "/tmp/build-env-nn5jlqfo/lib/python3.10/site-packages/numpy/core/include/numpy/ndarraytypes.h",
-            "/tmp/build-env-nn5jlqfo/lib/python3.10/site-packages/numpy/core/include/numpy/ufuncobject.h"
+            "/tmp/build-env-z2vjckqo/lib/python3.10/site-packages/numpy/core/include/numpy/arrayobject.h",
+            "/tmp/build-env-z2vjckqo/lib/python3.10/site-packages/numpy/core/include/numpy/arrayscalars.h",
+            "/tmp/build-env-z2vjckqo/lib/python3.10/site-packages/numpy/core/include/numpy/ndarrayobject.h",
+            "/tmp/build-env-z2vjckqo/lib/python3.10/site-packages/numpy/core/include/numpy/ndarraytypes.h",
+            "/tmp/build-env-z2vjckqo/lib/python3.10/site-packages/numpy/core/include/numpy/ufuncobject.h"
         ],
         "include_dirs": [
-            "/tmp/build-env-nn5jlqfo/lib/python3.10/site-packages/numpy/core/include",
-            "/tmp/build-env-nn5jlqfo/include"
+            "/tmp/build-env-z2vjckqo/lib/python3.10/site-packages/numpy/core/include",
+            "/tmp/build-env-z2vjckqo/include"
         ],
         "name": "suitesparse_graphblas.utils",
         "sources": [
             "suitesparse_graphblas/utils.pyx"
         ]
     },
     "module_name": "suitesparse_graphblas.utils"
@@ -1013,195 +1013,195 @@
 
 static const char *__pyx_f[] = {
   "suitesparse_graphblas/utils.pyx",
   "__init__.pxd",
   "type.pxd",
 };
 
-/* "../../../../../tmp/build-env-nn5jlqfo/lib/python3.10/site-packages/numpy/__init__.pxd":690
+/* "../../../../../tmp/build-env-z2vjckqo/lib/python3.10/site-packages/numpy/__init__.pxd":690
  * # in Cython to enable them only on the right systems.
  * 
  * ctypedef npy_int8       int8_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t
  */
 typedef npy_int8 __pyx_t_5numpy_int8_t;
 
-/* "../../../../../tmp/build-env-nn5jlqfo/lib/python3.10/site-packages/numpy/__init__.pxd":691
+/* "../../../../../tmp/build-env-z2vjckqo/lib/python3.10/site-packages/numpy/__init__.pxd":691
  * 
  * ctypedef npy_int8       int8_t
  * ctypedef npy_int16      int16_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int32      int32_t
  * ctypedef npy_int64      int64_t
  */
 typedef npy_int16 __pyx_t_5numpy_int16_t;
 
-/* "../../../../../tmp/build-env-nn5jlqfo/lib/python3.10/site-packages/numpy/__init__.pxd":692
+/* "../../../../../tmp/build-env-z2vjckqo/lib/python3.10/site-packages/numpy/__init__.pxd":692
  * ctypedef npy_int8       int8_t
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_int64      int64_t
  * #ctypedef npy_int96      int96_t
  */
 typedef npy_int32 __pyx_t_5numpy_int32_t;
 
-/* "../../../../../tmp/build-env-nn5jlqfo/lib/python3.10/site-packages/numpy/__init__.pxd":693
+/* "../../../../../tmp/build-env-z2vjckqo/lib/python3.10/site-packages/numpy/__init__.pxd":693
  * ctypedef npy_int16      int16_t
  * ctypedef npy_int32      int32_t
  * ctypedef npy_int64      int64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_int96      int96_t
  * #ctypedef npy_int128     int128_t
  */
 typedef npy_int64 __pyx_t_5numpy_int64_t;
 
-/* "../../../../../tmp/build-env-nn5jlqfo/lib/python3.10/site-packages/numpy/__init__.pxd":697
+/* "../../../../../tmp/build-env-z2vjckqo/lib/python3.10/site-packages/numpy/__init__.pxd":697
  * #ctypedef npy_int128     int128_t
  * 
  * ctypedef npy_uint8      uint8_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t
  */
 typedef npy_uint8 __pyx_t_5numpy_uint8_t;
 
-/* "../../../../../tmp/build-env-nn5jlqfo/lib/python3.10/site-packages/numpy/__init__.pxd":698
+/* "../../../../../tmp/build-env-z2vjckqo/lib/python3.10/site-packages/numpy/__init__.pxd":698
  * 
  * ctypedef npy_uint8      uint8_t
  * ctypedef npy_uint16     uint16_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint32     uint32_t
  * ctypedef npy_uint64     uint64_t
  */
 typedef npy_uint16 __pyx_t_5numpy_uint16_t;
 
-/* "../../../../../tmp/build-env-nn5jlqfo/lib/python3.10/site-packages/numpy/__init__.pxd":699
+/* "../../../../../tmp/build-env-z2vjckqo/lib/python3.10/site-packages/numpy/__init__.pxd":699
  * ctypedef npy_uint8      uint8_t
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uint64     uint64_t
  * #ctypedef npy_uint96     uint96_t
  */
 typedef npy_uint32 __pyx_t_5numpy_uint32_t;
 
-/* "../../../../../tmp/build-env-nn5jlqfo/lib/python3.10/site-packages/numpy/__init__.pxd":700
+/* "../../../../../tmp/build-env-z2vjckqo/lib/python3.10/site-packages/numpy/__init__.pxd":700
  * ctypedef npy_uint16     uint16_t
  * ctypedef npy_uint32     uint32_t
  * ctypedef npy_uint64     uint64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_uint96     uint96_t
  * #ctypedef npy_uint128    uint128_t
  */
 typedef npy_uint64 __pyx_t_5numpy_uint64_t;
 
-/* "../../../../../tmp/build-env-nn5jlqfo/lib/python3.10/site-packages/numpy/__init__.pxd":704
+/* "../../../../../tmp/build-env-z2vjckqo/lib/python3.10/site-packages/numpy/__init__.pxd":704
  * #ctypedef npy_uint128    uint128_t
  * 
  * ctypedef npy_float32    float32_t             # <<<<<<<<<<<<<<
  * ctypedef npy_float64    float64_t
  * #ctypedef npy_float80    float80_t
  */
 typedef npy_float32 __pyx_t_5numpy_float32_t;
 
-/* "../../../../../tmp/build-env-nn5jlqfo/lib/python3.10/site-packages/numpy/__init__.pxd":705
+/* "../../../../../tmp/build-env-z2vjckqo/lib/python3.10/site-packages/numpy/__init__.pxd":705
  * 
  * ctypedef npy_float32    float32_t
  * ctypedef npy_float64    float64_t             # <<<<<<<<<<<<<<
  * #ctypedef npy_float80    float80_t
  * #ctypedef npy_float128   float128_t
  */
 typedef npy_float64 __pyx_t_5numpy_float64_t;
 
-/* "../../../../../tmp/build-env-nn5jlqfo/lib/python3.10/site-packages/numpy/__init__.pxd":714
+/* "../../../../../tmp/build-env-z2vjckqo/lib/python3.10/site-packages/numpy/__init__.pxd":714
  * # The int types are mapped a bit surprising --
  * # numpy.int corresponds to 'l' and numpy.long to 'q'
  * ctypedef npy_long       int_t             # <<<<<<<<<<<<<<
  * ctypedef npy_longlong   long_t
  * ctypedef npy_longlong   longlong_t
  */
 typedef npy_long __pyx_t_5numpy_int_t;
 
-/* "../../../../../tmp/build-env-nn5jlqfo/lib/python3.10/site-packages/numpy/__init__.pxd":715
+/* "../../../../../tmp/build-env-z2vjckqo/lib/python3.10/site-packages/numpy/__init__.pxd":715
  * # numpy.int corresponds to 'l' and numpy.long to 'q'
  * ctypedef npy_long       int_t
  * ctypedef npy_longlong   long_t             # <<<<<<<<<<<<<<
  * ctypedef npy_longlong   longlong_t
  * 
  */
 typedef npy_longlong __pyx_t_5numpy_long_t;
 
-/* "../../../../../tmp/build-env-nn5jlqfo/lib/python3.10/site-packages/numpy/__init__.pxd":716
+/* "../../../../../tmp/build-env-z2vjckqo/lib/python3.10/site-packages/numpy/__init__.pxd":716
  * ctypedef npy_long       int_t
  * ctypedef npy_longlong   long_t
  * ctypedef npy_longlong   longlong_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_ulong      uint_t
  */
 typedef npy_longlong __pyx_t_5numpy_longlong_t;
 
-/* "../../../../../tmp/build-env-nn5jlqfo/lib/python3.10/site-packages/numpy/__init__.pxd":718
+/* "../../../../../tmp/build-env-z2vjckqo/lib/python3.10/site-packages/numpy/__init__.pxd":718
  * ctypedef npy_longlong   longlong_t
  * 
  * ctypedef npy_ulong      uint_t             # <<<<<<<<<<<<<<
  * ctypedef npy_ulonglong  ulong_t
  * ctypedef npy_ulonglong  ulonglong_t
  */
 typedef npy_ulong __pyx_t_5numpy_uint_t;
 
-/* "../../../../../tmp/build-env-nn5jlqfo/lib/python3.10/site-packages/numpy/__init__.pxd":719
+/* "../../../../../tmp/build-env-z2vjckqo/lib/python3.10/site-packages/numpy/__init__.pxd":719
  * 
  * ctypedef npy_ulong      uint_t
  * ctypedef npy_ulonglong  ulong_t             # <<<<<<<<<<<<<<
  * ctypedef npy_ulonglong  ulonglong_t
  * 
  */
 typedef npy_ulonglong __pyx_t_5numpy_ulong_t;
 
-/* "../../../../../tmp/build-env-nn5jlqfo/lib/python3.10/site-packages/numpy/__init__.pxd":720
+/* "../../../../../tmp/build-env-z2vjckqo/lib/python3.10/site-packages/numpy/__init__.pxd":720
  * ctypedef npy_ulong      uint_t
  * ctypedef npy_ulonglong  ulong_t
  * ctypedef npy_ulonglong  ulonglong_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_intp       intp_t
  */
 typedef npy_ulonglong __pyx_t_5numpy_ulonglong_t;
 
-/* "../../../../../tmp/build-env-nn5jlqfo/lib/python3.10/site-packages/numpy/__init__.pxd":722
+/* "../../../../../tmp/build-env-z2vjckqo/lib/python3.10/site-packages/numpy/__init__.pxd":722
  * ctypedef npy_ulonglong  ulonglong_t
  * 
  * ctypedef npy_intp       intp_t             # <<<<<<<<<<<<<<
  * ctypedef npy_uintp      uintp_t
  * 
  */
 typedef npy_intp __pyx_t_5numpy_intp_t;
 
-/* "../../../../../tmp/build-env-nn5jlqfo/lib/python3.10/site-packages/numpy/__init__.pxd":723
+/* "../../../../../tmp/build-env-z2vjckqo/lib/python3.10/site-packages/numpy/__init__.pxd":723
  * 
  * ctypedef npy_intp       intp_t
  * ctypedef npy_uintp      uintp_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_double     float_t
  */
 typedef npy_uintp __pyx_t_5numpy_uintp_t;
 
-/* "../../../../../tmp/build-env-nn5jlqfo/lib/python3.10/site-packages/numpy/__init__.pxd":725
+/* "../../../../../tmp/build-env-z2vjckqo/lib/python3.10/site-packages/numpy/__init__.pxd":725
  * ctypedef npy_uintp      uintp_t
  * 
  * ctypedef npy_double     float_t             # <<<<<<<<<<<<<<
  * ctypedef npy_double     double_t
  * ctypedef npy_longdouble longdouble_t
  */
 typedef npy_double __pyx_t_5numpy_float_t;
 
-/* "../../../../../tmp/build-env-nn5jlqfo/lib/python3.10/site-packages/numpy/__init__.pxd":726
+/* "../../../../../tmp/build-env-z2vjckqo/lib/python3.10/site-packages/numpy/__init__.pxd":726
  * 
  * ctypedef npy_double     float_t
  * ctypedef npy_double     double_t             # <<<<<<<<<<<<<<
  * ctypedef npy_longdouble longdouble_t
  * 
  */
 typedef npy_double __pyx_t_5numpy_double_t;
 
-/* "../../../../../tmp/build-env-nn5jlqfo/lib/python3.10/site-packages/numpy/__init__.pxd":727
+/* "../../../../../tmp/build-env-z2vjckqo/lib/python3.10/site-packages/numpy/__init__.pxd":727
  * ctypedef npy_double     float_t
  * ctypedef npy_double     double_t
  * ctypedef npy_longdouble longdouble_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_cfloat      cfloat_t
  */
 typedef npy_longdouble __pyx_t_5numpy_longdouble_t;
@@ -1228,42 +1228,42 @@
     typedef struct { double real, imag; } __pyx_t_double_complex;
 #endif
 static CYTHON_INLINE __pyx_t_double_complex __pyx_t_double_complex_from_parts(double, double);
 
 
 /*--- Type declarations ---*/
 
-/* "../../../../../tmp/build-env-nn5jlqfo/lib/python3.10/site-packages/numpy/__init__.pxd":729
+/* "../../../../../tmp/build-env-z2vjckqo/lib/python3.10/site-packages/numpy/__init__.pxd":729
  * ctypedef npy_longdouble longdouble_t
  * 
  * ctypedef npy_cfloat      cfloat_t             # <<<<<<<<<<<<<<
  * ctypedef npy_cdouble     cdouble_t
  * ctypedef npy_clongdouble clongdouble_t
  */
 typedef npy_cfloat __pyx_t_5numpy_cfloat_t;
 
-/* "../../../../../tmp/build-env-nn5jlqfo/lib/python3.10/site-packages/numpy/__init__.pxd":730
+/* "../../../../../tmp/build-env-z2vjckqo/lib/python3.10/site-packages/numpy/__init__.pxd":730
  * 
  * ctypedef npy_cfloat      cfloat_t
  * ctypedef npy_cdouble     cdouble_t             # <<<<<<<<<<<<<<
  * ctypedef npy_clongdouble clongdouble_t
  * 
  */
 typedef npy_cdouble __pyx_t_5numpy_cdouble_t;
 
-/* "../../../../../tmp/build-env-nn5jlqfo/lib/python3.10/site-packages/numpy/__init__.pxd":731
+/* "../../../../../tmp/build-env-z2vjckqo/lib/python3.10/site-packages/numpy/__init__.pxd":731
  * ctypedef npy_cfloat      cfloat_t
  * ctypedef npy_cdouble     cdouble_t
  * ctypedef npy_clongdouble clongdouble_t             # <<<<<<<<<<<<<<
  * 
  * ctypedef npy_cdouble     complex_t
  */
 typedef npy_clongdouble __pyx_t_5numpy_clongdouble_t;
 
-/* "../../../../../tmp/build-env-nn5jlqfo/lib/python3.10/site-packages/numpy/__init__.pxd":733
+/* "../../../../../tmp/build-env-z2vjckqo/lib/python3.10/site-packages/numpy/__init__.pxd":733
  * ctypedef npy_clongdouble clongdouble_t
  * 
  * ctypedef npy_cdouble     complex_t             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew1(a):
  */
 typedef npy_cdouble __pyx_t_5numpy_complex_t;
@@ -3224,15 +3224,15 @@
   __pyx_r = NULL;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-nn5jlqfo/lib/python3.10/site-packages/numpy/__init__.pxd":735
+/* "../../../../../tmp/build-env-z2vjckqo/lib/python3.10/site-packages/numpy/__init__.pxd":735
  * ctypedef npy_cdouble     complex_t
  * 
  * cdef inline object PyArray_MultiIterNew1(a):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  */
 
@@ -3241,29 +3241,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew1", 0);
 
-  /* "../../../../../tmp/build-env-nn5jlqfo/lib/python3.10/site-packages/numpy/__init__.pxd":736
+  /* "../../../../../tmp/build-env-z2vjckqo/lib/python3.10/site-packages/numpy/__init__.pxd":736
  * 
  * cdef inline object PyArray_MultiIterNew1(a):
  *     return PyArray_MultiIterNew(1, <void*>a)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(1, ((void *)__pyx_v_a)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 736, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-nn5jlqfo/lib/python3.10/site-packages/numpy/__init__.pxd":735
+  /* "../../../../../tmp/build-env-z2vjckqo/lib/python3.10/site-packages/numpy/__init__.pxd":735
  * ctypedef npy_cdouble     complex_t
  * 
  * cdef inline object PyArray_MultiIterNew1(a):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  */
 
@@ -3274,15 +3274,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-nn5jlqfo/lib/python3.10/site-packages/numpy/__init__.pxd":738
+/* "../../../../../tmp/build-env-z2vjckqo/lib/python3.10/site-packages/numpy/__init__.pxd":738
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  */
 
@@ -3291,29 +3291,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew2", 0);
 
-  /* "../../../../../tmp/build-env-nn5jlqfo/lib/python3.10/site-packages/numpy/__init__.pxd":739
+  /* "../../../../../tmp/build-env-z2vjckqo/lib/python3.10/site-packages/numpy/__init__.pxd":739
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(2, ((void *)__pyx_v_a), ((void *)__pyx_v_b)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 739, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-nn5jlqfo/lib/python3.10/site-packages/numpy/__init__.pxd":738
+  /* "../../../../../tmp/build-env-z2vjckqo/lib/python3.10/site-packages/numpy/__init__.pxd":738
  *     return PyArray_MultiIterNew(1, <void*>a)
  * 
  * cdef inline object PyArray_MultiIterNew2(a, b):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  */
 
@@ -3324,15 +3324,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-nn5jlqfo/lib/python3.10/site-packages/numpy/__init__.pxd":741
+/* "../../../../../tmp/build-env-z2vjckqo/lib/python3.10/site-packages/numpy/__init__.pxd":741
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  */
 
@@ -3341,29 +3341,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew3", 0);
 
-  /* "../../../../../tmp/build-env-nn5jlqfo/lib/python3.10/site-packages/numpy/__init__.pxd":742
+  /* "../../../../../tmp/build-env-z2vjckqo/lib/python3.10/site-packages/numpy/__init__.pxd":742
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(3, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 742, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-nn5jlqfo/lib/python3.10/site-packages/numpy/__init__.pxd":741
+  /* "../../../../../tmp/build-env-z2vjckqo/lib/python3.10/site-packages/numpy/__init__.pxd":741
  *     return PyArray_MultiIterNew(2, <void*>a, <void*>b)
  * 
  * cdef inline object PyArray_MultiIterNew3(a, b, c):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  */
 
@@ -3374,15 +3374,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-nn5jlqfo/lib/python3.10/site-packages/numpy/__init__.pxd":744
+/* "../../../../../tmp/build-env-z2vjckqo/lib/python3.10/site-packages/numpy/__init__.pxd":744
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  */
 
@@ -3391,29 +3391,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew4", 0);
 
-  /* "../../../../../tmp/build-env-nn5jlqfo/lib/python3.10/site-packages/numpy/__init__.pxd":745
+  /* "../../../../../tmp/build-env-z2vjckqo/lib/python3.10/site-packages/numpy/__init__.pxd":745
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(4, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c), ((void *)__pyx_v_d)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 745, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-nn5jlqfo/lib/python3.10/site-packages/numpy/__init__.pxd":744
+  /* "../../../../../tmp/build-env-z2vjckqo/lib/python3.10/site-packages/numpy/__init__.pxd":744
  *     return PyArray_MultiIterNew(3, <void*>a, <void*>b, <void*> c)
  * 
  * cdef inline object PyArray_MultiIterNew4(a, b, c, d):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  */
 
@@ -3424,15 +3424,15 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-nn5jlqfo/lib/python3.10/site-packages/numpy/__init__.pxd":747
+/* "../../../../../tmp/build-env-z2vjckqo/lib/python3.10/site-packages/numpy/__init__.pxd":747
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  */
 
@@ -3441,29 +3441,29 @@
   __Pyx_RefNannyDeclarations
   PyObject *__pyx_t_1 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("PyArray_MultiIterNew5", 0);
 
-  /* "../../../../../tmp/build-env-nn5jlqfo/lib/python3.10/site-packages/numpy/__init__.pxd":748
+  /* "../../../../../tmp/build-env-z2vjckqo/lib/python3.10/site-packages/numpy/__init__.pxd":748
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)             # <<<<<<<<<<<<<<
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  */
   __Pyx_XDECREF(__pyx_r);
   __pyx_t_1 = PyArray_MultiIterNew(5, ((void *)__pyx_v_a), ((void *)__pyx_v_b), ((void *)__pyx_v_c), ((void *)__pyx_v_d), ((void *)__pyx_v_e)); if (unlikely(!__pyx_t_1)) __PYX_ERR(1, 748, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   __pyx_r = __pyx_t_1;
   __pyx_t_1 = 0;
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-nn5jlqfo/lib/python3.10/site-packages/numpy/__init__.pxd":747
+  /* "../../../../../tmp/build-env-z2vjckqo/lib/python3.10/site-packages/numpy/__init__.pxd":747
  *     return PyArray_MultiIterNew(4, <void*>a, <void*>b, <void*>c, <void*> d)
  * 
  * cdef inline object PyArray_MultiIterNew5(a, b, c, d, e):             # <<<<<<<<<<<<<<
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  */
 
@@ -3474,212 +3474,212 @@
   __pyx_r = 0;
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-nn5jlqfo/lib/python3.10/site-packages/numpy/__init__.pxd":750
+/* "../../../../../tmp/build-env-z2vjckqo/lib/python3.10/site-packages/numpy/__init__.pxd":750
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):             # <<<<<<<<<<<<<<
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape
  */
 
 static CYTHON_INLINE PyObject *__pyx_f_5numpy_PyDataType_SHAPE(PyArray_Descr *__pyx_v_d) {
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   __Pyx_RefNannySetupContext("PyDataType_SHAPE", 0);
 
-  /* "../../../../../tmp/build-env-nn5jlqfo/lib/python3.10/site-packages/numpy/__init__.pxd":751
+  /* "../../../../../tmp/build-env-z2vjckqo/lib/python3.10/site-packages/numpy/__init__.pxd":751
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):             # <<<<<<<<<<<<<<
  *         return <tuple>d.subarray.shape
  *     else:
  */
   __pyx_t_1 = (PyDataType_HASSUBARRAY(__pyx_v_d) != 0);
   if (__pyx_t_1) {
 
-    /* "../../../../../tmp/build-env-nn5jlqfo/lib/python3.10/site-packages/numpy/__init__.pxd":752
+    /* "../../../../../tmp/build-env-z2vjckqo/lib/python3.10/site-packages/numpy/__init__.pxd":752
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape             # <<<<<<<<<<<<<<
  *     else:
  *         return ()
  */
     __Pyx_XDECREF(__pyx_r);
     __Pyx_INCREF(((PyObject*)__pyx_v_d->subarray->shape));
     __pyx_r = ((PyObject*)__pyx_v_d->subarray->shape);
     goto __pyx_L0;
 
-    /* "../../../../../tmp/build-env-nn5jlqfo/lib/python3.10/site-packages/numpy/__init__.pxd":751
+    /* "../../../../../tmp/build-env-z2vjckqo/lib/python3.10/site-packages/numpy/__init__.pxd":751
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):
  *     if PyDataType_HASSUBARRAY(d):             # <<<<<<<<<<<<<<
  *         return <tuple>d.subarray.shape
  *     else:
  */
   }
 
-  /* "../../../../../tmp/build-env-nn5jlqfo/lib/python3.10/site-packages/numpy/__init__.pxd":754
+  /* "../../../../../tmp/build-env-z2vjckqo/lib/python3.10/site-packages/numpy/__init__.pxd":754
  *         return <tuple>d.subarray.shape
  *     else:
  *         return ()             # <<<<<<<<<<<<<<
  * 
  * 
  */
   /*else*/ {
     __Pyx_XDECREF(__pyx_r);
     __Pyx_INCREF(__pyx_empty_tuple);
     __pyx_r = __pyx_empty_tuple;
     goto __pyx_L0;
   }
 
-  /* "../../../../../tmp/build-env-nn5jlqfo/lib/python3.10/site-packages/numpy/__init__.pxd":750
+  /* "../../../../../tmp/build-env-z2vjckqo/lib/python3.10/site-packages/numpy/__init__.pxd":750
  *     return PyArray_MultiIterNew(5, <void*>a, <void*>b, <void*>c, <void*> d, <void*> e)
  * 
  * cdef inline tuple PyDataType_SHAPE(dtype d):             # <<<<<<<<<<<<<<
  *     if PyDataType_HASSUBARRAY(d):
  *         return <tuple>d.subarray.shape
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-nn5jlqfo/lib/python3.10/site-packages/numpy/__init__.pxd":929
+/* "../../../../../tmp/build-env-z2vjckqo/lib/python3.10/site-packages/numpy/__init__.pxd":929
  *     int _import_umath() except -1
  * 
  * cdef inline void set_array_base(ndarray arr, object base):             # <<<<<<<<<<<<<<
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)
  */
 
 static CYTHON_INLINE void __pyx_f_5numpy_set_array_base(PyArrayObject *__pyx_v_arr, PyObject *__pyx_v_base) {
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("set_array_base", 0);
 
-  /* "../../../../../tmp/build-env-nn5jlqfo/lib/python3.10/site-packages/numpy/__init__.pxd":930
+  /* "../../../../../tmp/build-env-z2vjckqo/lib/python3.10/site-packages/numpy/__init__.pxd":930
  * 
  * cdef inline void set_array_base(ndarray arr, object base):
  *     Py_INCREF(base) # important to do this before stealing the reference below!             # <<<<<<<<<<<<<<
  *     PyArray_SetBaseObject(arr, base)
  * 
  */
   Py_INCREF(__pyx_v_base);
 
-  /* "../../../../../tmp/build-env-nn5jlqfo/lib/python3.10/site-packages/numpy/__init__.pxd":931
+  /* "../../../../../tmp/build-env-z2vjckqo/lib/python3.10/site-packages/numpy/__init__.pxd":931
  * cdef inline void set_array_base(ndarray arr, object base):
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)             # <<<<<<<<<<<<<<
  * 
  * cdef inline object get_array_base(ndarray arr):
  */
   (void)(PyArray_SetBaseObject(__pyx_v_arr, __pyx_v_base));
 
-  /* "../../../../../tmp/build-env-nn5jlqfo/lib/python3.10/site-packages/numpy/__init__.pxd":929
+  /* "../../../../../tmp/build-env-z2vjckqo/lib/python3.10/site-packages/numpy/__init__.pxd":929
  *     int _import_umath() except -1
  * 
  * cdef inline void set_array_base(ndarray arr, object base):             # <<<<<<<<<<<<<<
  *     Py_INCREF(base) # important to do this before stealing the reference below!
  *     PyArray_SetBaseObject(arr, base)
  */
 
   /* function exit code */
   __Pyx_RefNannyFinishContext();
 }
 
-/* "../../../../../tmp/build-env-nn5jlqfo/lib/python3.10/site-packages/numpy/__init__.pxd":933
+/* "../../../../../tmp/build-env-z2vjckqo/lib/python3.10/site-packages/numpy/__init__.pxd":933
  *     PyArray_SetBaseObject(arr, base)
  * 
  * cdef inline object get_array_base(ndarray arr):             # <<<<<<<<<<<<<<
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  */
 
 static CYTHON_INLINE PyObject *__pyx_f_5numpy_get_array_base(PyArrayObject *__pyx_v_arr) {
   PyObject *__pyx_v_base;
   PyObject *__pyx_r = NULL;
   __Pyx_RefNannyDeclarations
   int __pyx_t_1;
   __Pyx_RefNannySetupContext("get_array_base", 0);
 
-  /* "../../../../../tmp/build-env-nn5jlqfo/lib/python3.10/site-packages/numpy/__init__.pxd":934
+  /* "../../../../../tmp/build-env-z2vjckqo/lib/python3.10/site-packages/numpy/__init__.pxd":934
  * 
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)             # <<<<<<<<<<<<<<
  *     if base is NULL:
  *         return None
  */
   __pyx_v_base = PyArray_BASE(__pyx_v_arr);
 
-  /* "../../../../../tmp/build-env-nn5jlqfo/lib/python3.10/site-packages/numpy/__init__.pxd":935
+  /* "../../../../../tmp/build-env-z2vjckqo/lib/python3.10/site-packages/numpy/__init__.pxd":935
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)
  *     if base is NULL:             # <<<<<<<<<<<<<<
  *         return None
  *     return <object>base
  */
   __pyx_t_1 = ((__pyx_v_base == NULL) != 0);
   if (__pyx_t_1) {
 
-    /* "../../../../../tmp/build-env-nn5jlqfo/lib/python3.10/site-packages/numpy/__init__.pxd":936
+    /* "../../../../../tmp/build-env-z2vjckqo/lib/python3.10/site-packages/numpy/__init__.pxd":936
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  *         return None             # <<<<<<<<<<<<<<
  *     return <object>base
  * 
  */
     __Pyx_XDECREF(__pyx_r);
     __pyx_r = Py_None; __Pyx_INCREF(Py_None);
     goto __pyx_L0;
 
-    /* "../../../../../tmp/build-env-nn5jlqfo/lib/python3.10/site-packages/numpy/__init__.pxd":935
+    /* "../../../../../tmp/build-env-z2vjckqo/lib/python3.10/site-packages/numpy/__init__.pxd":935
  * cdef inline object get_array_base(ndarray arr):
  *     base = PyArray_BASE(arr)
  *     if base is NULL:             # <<<<<<<<<<<<<<
  *         return None
  *     return <object>base
  */
   }
 
-  /* "../../../../../tmp/build-env-nn5jlqfo/lib/python3.10/site-packages/numpy/__init__.pxd":937
+  /* "../../../../../tmp/build-env-z2vjckqo/lib/python3.10/site-packages/numpy/__init__.pxd":937
  *     if base is NULL:
  *         return None
  *     return <object>base             # <<<<<<<<<<<<<<
  * 
  * # Versions of the import_* functions which are more suitable for
  */
   __Pyx_XDECREF(__pyx_r);
   __Pyx_INCREF(((PyObject *)__pyx_v_base));
   __pyx_r = ((PyObject *)__pyx_v_base);
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-nn5jlqfo/lib/python3.10/site-packages/numpy/__init__.pxd":933
+  /* "../../../../../tmp/build-env-z2vjckqo/lib/python3.10/site-packages/numpy/__init__.pxd":933
  *     PyArray_SetBaseObject(arr, base)
  * 
  * cdef inline object get_array_base(ndarray arr):             # <<<<<<<<<<<<<<
  *     base = PyArray_BASE(arr)
  *     if base is NULL:
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_XGIVEREF(__pyx_r);
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-nn5jlqfo/lib/python3.10/site-packages/numpy/__init__.pxd":941
+/* "../../../../../tmp/build-env-z2vjckqo/lib/python3.10/site-packages/numpy/__init__.pxd":941
  * # Versions of the import_* functions which are more suitable for
  * # Cython code.
  * cdef inline int import_array() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         __pyx_import_array()
  */
 
@@ -3695,15 +3695,15 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_array", 0);
 
-  /* "../../../../../tmp/build-env-nn5jlqfo/lib/python3.10/site-packages/numpy/__init__.pxd":942
+  /* "../../../../../tmp/build-env-z2vjckqo/lib/python3.10/site-packages/numpy/__init__.pxd":942
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
   {
@@ -3711,53 +3711,53 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "../../../../../tmp/build-env-nn5jlqfo/lib/python3.10/site-packages/numpy/__init__.pxd":943
+      /* "../../../../../tmp/build-env-z2vjckqo/lib/python3.10/site-packages/numpy/__init__.pxd":943
  * cdef inline int import_array() except -1:
  *     try:
  *         __pyx_import_array()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")
  */
       __pyx_t_4 = _import_array(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(1, 943, __pyx_L3_error)
 
-      /* "../../../../../tmp/build-env-nn5jlqfo/lib/python3.10/site-packages/numpy/__init__.pxd":942
+      /* "../../../../../tmp/build-env-z2vjckqo/lib/python3.10/site-packages/numpy/__init__.pxd":942
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "../../../../../tmp/build-env-nn5jlqfo/lib/python3.10/site-packages/numpy/__init__.pxd":944
+    /* "../../../../../tmp/build-env-z2vjckqo/lib/python3.10/site-packages/numpy/__init__.pxd":944
  *     try:
  *         __pyx_import_array()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_array", __pyx_clineno, __pyx_lineno, __pyx_filename);
       if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(1, 944, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_5);
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_GOTREF(__pyx_t_7);
 
-      /* "../../../../../tmp/build-env-nn5jlqfo/lib/python3.10/site-packages/numpy/__init__.pxd":945
+      /* "../../../../../tmp/build-env-z2vjckqo/lib/python3.10/site-packages/numpy/__init__.pxd":945
  *         __pyx_import_array()
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_umath() except -1:
  */
       __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__2, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(1, 945, __pyx_L5_except_error)
@@ -3765,30 +3765,30 @@
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
       __PYX_ERR(1, 945, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
     __pyx_L5_except_error:;
 
-    /* "../../../../../tmp/build-env-nn5jlqfo/lib/python3.10/site-packages/numpy/__init__.pxd":942
+    /* "../../../../../tmp/build-env-z2vjckqo/lib/python3.10/site-packages/numpy/__init__.pxd":942
  * # Cython code.
  * cdef inline int import_array() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         __pyx_import_array()
  *     except Exception:
  */
     __Pyx_XGIVEREF(__pyx_t_1);
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "../../../../../tmp/build-env-nn5jlqfo/lib/python3.10/site-packages/numpy/__init__.pxd":941
+  /* "../../../../../tmp/build-env-z2vjckqo/lib/python3.10/site-packages/numpy/__init__.pxd":941
  * # Versions of the import_* functions which are more suitable for
  * # Cython code.
  * cdef inline int import_array() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         __pyx_import_array()
  */
 
@@ -3803,15 +3803,15 @@
   __Pyx_AddTraceback("numpy.import_array", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-nn5jlqfo/lib/python3.10/site-packages/numpy/__init__.pxd":947
+/* "../../../../../tmp/build-env-z2vjckqo/lib/python3.10/site-packages/numpy/__init__.pxd":947
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  * cdef inline int import_umath() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -3827,15 +3827,15 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_umath", 0);
 
-  /* "../../../../../tmp/build-env-nn5jlqfo/lib/python3.10/site-packages/numpy/__init__.pxd":948
+  /* "../../../../../tmp/build-env-z2vjckqo/lib/python3.10/site-packages/numpy/__init__.pxd":948
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
   {
@@ -3843,53 +3843,53 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "../../../../../tmp/build-env-nn5jlqfo/lib/python3.10/site-packages/numpy/__init__.pxd":949
+      /* "../../../../../tmp/build-env-z2vjckqo/lib/python3.10/site-packages/numpy/__init__.pxd":949
  * cdef inline int import_umath() except -1:
  *     try:
  *         _import_umath()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")
  */
       __pyx_t_4 = _import_umath(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(1, 949, __pyx_L3_error)
 
-      /* "../../../../../tmp/build-env-nn5jlqfo/lib/python3.10/site-packages/numpy/__init__.pxd":948
+      /* "../../../../../tmp/build-env-z2vjckqo/lib/python3.10/site-packages/numpy/__init__.pxd":948
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "../../../../../tmp/build-env-nn5jlqfo/lib/python3.10/site-packages/numpy/__init__.pxd":950
+    /* "../../../../../tmp/build-env-z2vjckqo/lib/python3.10/site-packages/numpy/__init__.pxd":950
  *     try:
  *         _import_umath()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_umath", __pyx_clineno, __pyx_lineno, __pyx_filename);
       if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(1, 950, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_5);
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_GOTREF(__pyx_t_7);
 
-      /* "../../../../../tmp/build-env-nn5jlqfo/lib/python3.10/site-packages/numpy/__init__.pxd":951
+      /* "../../../../../tmp/build-env-z2vjckqo/lib/python3.10/site-packages/numpy/__init__.pxd":951
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_ufunc() except -1:
  */
       __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__3, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(1, 951, __pyx_L5_except_error)
@@ -3897,30 +3897,30 @@
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
       __PYX_ERR(1, 951, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
     __pyx_L5_except_error:;
 
-    /* "../../../../../tmp/build-env-nn5jlqfo/lib/python3.10/site-packages/numpy/__init__.pxd":948
+    /* "../../../../../tmp/build-env-z2vjckqo/lib/python3.10/site-packages/numpy/__init__.pxd":948
  * 
  * cdef inline int import_umath() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     __Pyx_XGIVEREF(__pyx_t_1);
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "../../../../../tmp/build-env-nn5jlqfo/lib/python3.10/site-packages/numpy/__init__.pxd":947
+  /* "../../../../../tmp/build-env-z2vjckqo/lib/python3.10/site-packages/numpy/__init__.pxd":947
  *         raise ImportError("numpy.core.multiarray failed to import")
  * 
  * cdef inline int import_umath() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -3935,15 +3935,15 @@
   __Pyx_AddTraceback("numpy.import_umath", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-nn5jlqfo/lib/python3.10/site-packages/numpy/__init__.pxd":953
+/* "../../../../../tmp/build-env-z2vjckqo/lib/python3.10/site-packages/numpy/__init__.pxd":953
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  * cdef inline int import_ufunc() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -3959,15 +3959,15 @@
   PyObject *__pyx_t_7 = NULL;
   PyObject *__pyx_t_8 = NULL;
   int __pyx_lineno = 0;
   const char *__pyx_filename = NULL;
   int __pyx_clineno = 0;
   __Pyx_RefNannySetupContext("import_ufunc", 0);
 
-  /* "../../../../../tmp/build-env-nn5jlqfo/lib/python3.10/site-packages/numpy/__init__.pxd":954
+  /* "../../../../../tmp/build-env-z2vjckqo/lib/python3.10/site-packages/numpy/__init__.pxd":954
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
   {
@@ -3975,53 +3975,53 @@
     __Pyx_PyThreadState_assign
     __Pyx_ExceptionSave(&__pyx_t_1, &__pyx_t_2, &__pyx_t_3);
     __Pyx_XGOTREF(__pyx_t_1);
     __Pyx_XGOTREF(__pyx_t_2);
     __Pyx_XGOTREF(__pyx_t_3);
     /*try:*/ {
 
-      /* "../../../../../tmp/build-env-nn5jlqfo/lib/python3.10/site-packages/numpy/__init__.pxd":955
+      /* "../../../../../tmp/build-env-z2vjckqo/lib/python3.10/site-packages/numpy/__init__.pxd":955
  * cdef inline int import_ufunc() except -1:
  *     try:
  *         _import_umath()             # <<<<<<<<<<<<<<
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")
  */
       __pyx_t_4 = _import_umath(); if (unlikely(__pyx_t_4 == ((int)-1))) __PYX_ERR(1, 955, __pyx_L3_error)
 
-      /* "../../../../../tmp/build-env-nn5jlqfo/lib/python3.10/site-packages/numpy/__init__.pxd":954
+      /* "../../../../../tmp/build-env-z2vjckqo/lib/python3.10/site-packages/numpy/__init__.pxd":954
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     }
     __Pyx_XDECREF(__pyx_t_1); __pyx_t_1 = 0;
     __Pyx_XDECREF(__pyx_t_2); __pyx_t_2 = 0;
     __Pyx_XDECREF(__pyx_t_3); __pyx_t_3 = 0;
     goto __pyx_L8_try_end;
     __pyx_L3_error:;
 
-    /* "../../../../../tmp/build-env-nn5jlqfo/lib/python3.10/site-packages/numpy/__init__.pxd":956
+    /* "../../../../../tmp/build-env-z2vjckqo/lib/python3.10/site-packages/numpy/__init__.pxd":956
  *     try:
  *         _import_umath()
  *     except Exception:             # <<<<<<<<<<<<<<
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  */
     __pyx_t_4 = __Pyx_PyErr_ExceptionMatches(((PyObject *)(&((PyTypeObject*)PyExc_Exception)[0])));
     if (__pyx_t_4) {
       __Pyx_AddTraceback("numpy.import_ufunc", __pyx_clineno, __pyx_lineno, __pyx_filename);
       if (__Pyx_GetException(&__pyx_t_5, &__pyx_t_6, &__pyx_t_7) < 0) __PYX_ERR(1, 956, __pyx_L5_except_error)
       __Pyx_GOTREF(__pyx_t_5);
       __Pyx_GOTREF(__pyx_t_6);
       __Pyx_GOTREF(__pyx_t_7);
 
-      /* "../../../../../tmp/build-env-nn5jlqfo/lib/python3.10/site-packages/numpy/__init__.pxd":957
+      /* "../../../../../tmp/build-env-z2vjckqo/lib/python3.10/site-packages/numpy/__init__.pxd":957
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef extern from *:
  */
       __pyx_t_8 = __Pyx_PyObject_Call(__pyx_builtin_ImportError, __pyx_tuple__3, NULL); if (unlikely(!__pyx_t_8)) __PYX_ERR(1, 957, __pyx_L5_except_error)
@@ -4029,30 +4029,30 @@
       __Pyx_Raise(__pyx_t_8, 0, 0, 0);
       __Pyx_DECREF(__pyx_t_8); __pyx_t_8 = 0;
       __PYX_ERR(1, 957, __pyx_L5_except_error)
     }
     goto __pyx_L5_except_error;
     __pyx_L5_except_error:;
 
-    /* "../../../../../tmp/build-env-nn5jlqfo/lib/python3.10/site-packages/numpy/__init__.pxd":954
+    /* "../../../../../tmp/build-env-z2vjckqo/lib/python3.10/site-packages/numpy/__init__.pxd":954
  * 
  * cdef inline int import_ufunc() except -1:
  *     try:             # <<<<<<<<<<<<<<
  *         _import_umath()
  *     except Exception:
  */
     __Pyx_XGIVEREF(__pyx_t_1);
     __Pyx_XGIVEREF(__pyx_t_2);
     __Pyx_XGIVEREF(__pyx_t_3);
     __Pyx_ExceptionReset(__pyx_t_1, __pyx_t_2, __pyx_t_3);
     goto __pyx_L1_error;
     __pyx_L8_try_end:;
   }
 
-  /* "../../../../../tmp/build-env-nn5jlqfo/lib/python3.10/site-packages/numpy/__init__.pxd":953
+  /* "../../../../../tmp/build-env-z2vjckqo/lib/python3.10/site-packages/numpy/__init__.pxd":953
  *         raise ImportError("numpy.core.umath failed to import")
  * 
  * cdef inline int import_ufunc() except -1:             # <<<<<<<<<<<<<<
  *     try:
  *         _import_umath()
  */
 
@@ -4067,176 +4067,176 @@
   __Pyx_AddTraceback("numpy.import_ufunc", __pyx_clineno, __pyx_lineno, __pyx_filename);
   __pyx_r = -1;
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-nn5jlqfo/lib/python3.10/site-packages/numpy/__init__.pxd":967
+/* "../../../../../tmp/build-env-z2vjckqo/lib/python3.10/site-packages/numpy/__init__.pxd":967
  * 
  * 
  * cdef inline bint is_timedelta64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.timedelta64)`
  */
 
 static CYTHON_INLINE int __pyx_f_5numpy_is_timedelta64_object(PyObject *__pyx_v_obj) {
   int __pyx_r;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("is_timedelta64_object", 0);
 
-  /* "../../../../../tmp/build-env-nn5jlqfo/lib/python3.10/site-packages/numpy/__init__.pxd":979
+  /* "../../../../../tmp/build-env-z2vjckqo/lib/python3.10/site-packages/numpy/__init__.pxd":979
  *     bool
  *     """
  *     return PyObject_TypeCheck(obj, &PyTimedeltaArrType_Type)             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = PyObject_TypeCheck(__pyx_v_obj, (&PyTimedeltaArrType_Type));
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-nn5jlqfo/lib/python3.10/site-packages/numpy/__init__.pxd":967
+  /* "../../../../../tmp/build-env-z2vjckqo/lib/python3.10/site-packages/numpy/__init__.pxd":967
  * 
  * 
  * cdef inline bint is_timedelta64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.timedelta64)`
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-nn5jlqfo/lib/python3.10/site-packages/numpy/__init__.pxd":982
+/* "../../../../../tmp/build-env-z2vjckqo/lib/python3.10/site-packages/numpy/__init__.pxd":982
  * 
  * 
  * cdef inline bint is_datetime64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.datetime64)`
  */
 
 static CYTHON_INLINE int __pyx_f_5numpy_is_datetime64_object(PyObject *__pyx_v_obj) {
   int __pyx_r;
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("is_datetime64_object", 0);
 
-  /* "../../../../../tmp/build-env-nn5jlqfo/lib/python3.10/site-packages/numpy/__init__.pxd":994
+  /* "../../../../../tmp/build-env-z2vjckqo/lib/python3.10/site-packages/numpy/__init__.pxd":994
  *     bool
  *     """
  *     return PyObject_TypeCheck(obj, &PyDatetimeArrType_Type)             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = PyObject_TypeCheck(__pyx_v_obj, (&PyDatetimeArrType_Type));
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-nn5jlqfo/lib/python3.10/site-packages/numpy/__init__.pxd":982
+  /* "../../../../../tmp/build-env-z2vjckqo/lib/python3.10/site-packages/numpy/__init__.pxd":982
  * 
  * 
  * cdef inline bint is_datetime64_object(object obj):             # <<<<<<<<<<<<<<
  *     """
  *     Cython equivalent of `isinstance(obj, np.datetime64)`
  */
 
   /* function exit code */
   __pyx_L0:;
   __Pyx_RefNannyFinishContext();
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-nn5jlqfo/lib/python3.10/site-packages/numpy/__init__.pxd":997
+/* "../../../../../tmp/build-env-z2vjckqo/lib/python3.10/site-packages/numpy/__init__.pxd":997
  * 
  * 
  * cdef inline npy_datetime get_datetime64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy datetime64 object
  */
 
 static CYTHON_INLINE npy_datetime __pyx_f_5numpy_get_datetime64_value(PyObject *__pyx_v_obj) {
   npy_datetime __pyx_r;
 
-  /* "../../../../../tmp/build-env-nn5jlqfo/lib/python3.10/site-packages/numpy/__init__.pxd":1004
+  /* "../../../../../tmp/build-env-z2vjckqo/lib/python3.10/site-packages/numpy/__init__.pxd":1004
  *     also needed.  That can be found using `get_datetime64_unit`.
  *     """
  *     return (<PyDatetimeScalarObject*>obj).obval             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = ((PyDatetimeScalarObject *)__pyx_v_obj)->obval;
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-nn5jlqfo/lib/python3.10/site-packages/numpy/__init__.pxd":997
+  /* "../../../../../tmp/build-env-z2vjckqo/lib/python3.10/site-packages/numpy/__init__.pxd":997
  * 
  * 
  * cdef inline npy_datetime get_datetime64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy datetime64 object
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-nn5jlqfo/lib/python3.10/site-packages/numpy/__init__.pxd":1007
+/* "../../../../../tmp/build-env-z2vjckqo/lib/python3.10/site-packages/numpy/__init__.pxd":1007
  * 
  * 
  * cdef inline npy_timedelta get_timedelta64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy timedelta64 object
  */
 
 static CYTHON_INLINE npy_timedelta __pyx_f_5numpy_get_timedelta64_value(PyObject *__pyx_v_obj) {
   npy_timedelta __pyx_r;
 
-  /* "../../../../../tmp/build-env-nn5jlqfo/lib/python3.10/site-packages/numpy/__init__.pxd":1011
+  /* "../../../../../tmp/build-env-z2vjckqo/lib/python3.10/site-packages/numpy/__init__.pxd":1011
  *     returns the int64 value underlying scalar numpy timedelta64 object
  *     """
  *     return (<PyTimedeltaScalarObject*>obj).obval             # <<<<<<<<<<<<<<
  * 
  * 
  */
   __pyx_r = ((PyTimedeltaScalarObject *)__pyx_v_obj)->obval;
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-nn5jlqfo/lib/python3.10/site-packages/numpy/__init__.pxd":1007
+  /* "../../../../../tmp/build-env-z2vjckqo/lib/python3.10/site-packages/numpy/__init__.pxd":1007
  * 
  * 
  * cdef inline npy_timedelta get_timedelta64_value(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the int64 value underlying scalar numpy timedelta64 object
  */
 
   /* function exit code */
   __pyx_L0:;
   return __pyx_r;
 }
 
-/* "../../../../../tmp/build-env-nn5jlqfo/lib/python3.10/site-packages/numpy/__init__.pxd":1014
+/* "../../../../../tmp/build-env-z2vjckqo/lib/python3.10/site-packages/numpy/__init__.pxd":1014
  * 
  * 
  * cdef inline NPY_DATETIMEUNIT get_datetime64_unit(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the unit part of the dtype for a numpy datetime64 object.
  */
 
 static CYTHON_INLINE NPY_DATETIMEUNIT __pyx_f_5numpy_get_datetime64_unit(PyObject *__pyx_v_obj) {
   NPY_DATETIMEUNIT __pyx_r;
 
-  /* "../../../../../tmp/build-env-nn5jlqfo/lib/python3.10/site-packages/numpy/__init__.pxd":1018
+  /* "../../../../../tmp/build-env-z2vjckqo/lib/python3.10/site-packages/numpy/__init__.pxd":1018
  *     returns the unit part of the dtype for a numpy datetime64 object.
  *     """
  *     return <NPY_DATETIMEUNIT>(<PyDatetimeScalarObject*>obj).obmeta.base             # <<<<<<<<<<<<<<
  */
   __pyx_r = ((NPY_DATETIMEUNIT)((PyDatetimeScalarObject *)__pyx_v_obj)->obmeta.base);
   goto __pyx_L0;
 
-  /* "../../../../../tmp/build-env-nn5jlqfo/lib/python3.10/site-packages/numpy/__init__.pxd":1014
+  /* "../../../../../tmp/build-env-z2vjckqo/lib/python3.10/site-packages/numpy/__init__.pxd":1014
  * 
  * 
  * cdef inline NPY_DATETIMEUNIT get_datetime64_unit(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the unit part of the dtype for a numpy datetime64 object.
  */
 
@@ -4339,26 +4339,26 @@
   return -1;
 }
 
 static CYTHON_SMALL_CODE int __Pyx_InitCachedConstants(void) {
   __Pyx_RefNannyDeclarations
   __Pyx_RefNannySetupContext("__Pyx_InitCachedConstants", 0);
 
-  /* "../../../../../tmp/build-env-nn5jlqfo/lib/python3.10/site-packages/numpy/__init__.pxd":945
+  /* "../../../../../tmp/build-env-z2vjckqo/lib/python3.10/site-packages/numpy/__init__.pxd":945
  *         __pyx_import_array()
  *     except Exception:
  *         raise ImportError("numpy.core.multiarray failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_umath() except -1:
  */
   __pyx_tuple__2 = PyTuple_Pack(1, __pyx_kp_u_numpy_core_multiarray_failed_to); if (unlikely(!__pyx_tuple__2)) __PYX_ERR(1, 945, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_tuple__2);
   __Pyx_GIVEREF(__pyx_tuple__2);
 
-  /* "../../../../../tmp/build-env-nn5jlqfo/lib/python3.10/site-packages/numpy/__init__.pxd":951
+  /* "../../../../../tmp/build-env-z2vjckqo/lib/python3.10/site-packages/numpy/__init__.pxd":951
  *         _import_umath()
  *     except Exception:
  *         raise ImportError("numpy.core.umath failed to import")             # <<<<<<<<<<<<<<
  * 
  * cdef inline int import_ufunc() except -1:
  */
   __pyx_tuple__3 = PyTuple_Pack(1, __pyx_kp_u_numpy_core_umath_failed_to_impor); if (unlikely(!__pyx_tuple__3)) __PYX_ERR(1, 951, __pyx_L1_error)
@@ -4839,15 +4839,15 @@
  * from libc.stdint cimport uintptr_t
  */
   __pyx_t_1 = __Pyx_PyDict_NewPresized(0); if (unlikely(!__pyx_t_1)) __PYX_ERR(0, 1, __pyx_L1_error)
   __Pyx_GOTREF(__pyx_t_1);
   if (PyDict_SetItem(__pyx_d, __pyx_n_s_test, __pyx_t_1) < 0) __PYX_ERR(0, 1, __pyx_L1_error)
   __Pyx_DECREF(__pyx_t_1); __pyx_t_1 = 0;
 
-  /* "../../../../../tmp/build-env-nn5jlqfo/lib/python3.10/site-packages/numpy/__init__.pxd":1014
+  /* "../../../../../tmp/build-env-z2vjckqo/lib/python3.10/site-packages/numpy/__init__.pxd":1014
  * 
  * 
  * cdef inline NPY_DATETIMEUNIT get_datetime64_unit(object obj) nogil:             # <<<<<<<<<<<<<<
  *     """
  *     returns the unit part of the dtype for a numpy datetime64 object.
  */
```

### Comparing `suitesparse-graphblas-7.4.4.1a0/suitesparse_graphblas/utils.pxd` & `suitesparse-graphblas-7.4.4.1a1/suitesparse_graphblas/utils.pxd`

 * *Files identical despite different names*

### Comparing `suitesparse-graphblas-7.4.4.1a0/suitesparse_graphblas/utils.pyx` & `suitesparse-graphblas-7.4.4.1a1/suitesparse_graphblas/utils.pyx`

 * *Files identical despite different names*

### Comparing `suitesparse-graphblas-7.4.4.1a0/suitesparse_graphblas/vector.py` & `suitesparse-graphblas-7.4.4.1a1/suitesparse_graphblas/vector.py`

 * *Files identical despite different names*

### Comparing `suitesparse-graphblas-7.4.4.1a0/suitesparse_graphblas.egg-info/PKG-INFO` & `suitesparse-graphblas-7.4.4.1a1/suitesparse_graphblas.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: suitesparse-graphblas
-Version: 7.4.4.1a0
+Version: 7.4.4.1a1
 Summary: SuiteSparse:GraphBLAS Python bindings.
 Author: Jim Kitchen, Michel Pelletier, suitesparse-graphblas contributors
 Author-email: Erik Welch <erik.n.welch@gmail.com>
 Maintainer-email: Erik Welch <erik.n.welch@gmail.com>, Jim Kitchen <jim22k@gmail.com>, Michel Pelletier <michel@graphegon.com>
 License:                                  Apache License
                                    Version 2.0, January 2004
                                 http://www.apache.org/licenses/
```

### Comparing `suitesparse-graphblas-7.4.4.1a0/suitesparse_graphblas.egg-info/SOURCES.txt` & `suitesparse-graphblas-7.4.4.1a1/suitesparse_graphblas.egg-info/SOURCES.txt`

 * *Files identical despite different names*

