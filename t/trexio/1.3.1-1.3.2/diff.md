# Comparing `tmp/trexio-1.3.1.tar.gz` & `tmp/trexio-1.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "trexio-1.3.1.tar", last modified: Wed Apr 26 08:25:43 2023, max compression
+gzip compressed data, was "trexio-1.3.2.tar", last modified: Fri May  5 15:09:27 2023, max compression
```

## Comparing `trexio-1.3.1.tar` & `trexio-1.3.2.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-26 08:25:43.967239 trexio-1.3.1/
--rw-r--r--   0 runner    (1001) docker     (122)       39 2023-04-26 08:24:16.000000 trexio-1.3.1/AUTHORS
--rw-r--r--   0 runner    (1001) docker     (122)     1533 2023-04-26 08:24:16.000000 trexio-1.3.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (122)      267 2023-04-26 08:21:35.000000 trexio-1.3.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (122)     5521 2023-04-26 08:25:43.967239 trexio-1.3.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)     4573 2023-04-26 08:21:35.000000 trexio-1.3.1/README.md
--rw-r--r--   0 runner    (1001) docker     (122)     1931 2023-04-26 08:21:35.000000 trexio-1.3.1/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-26 08:25:43.959238 trexio-1.3.1/pytrexio/
--rw-r--r--   0 runner    (1001) docker     (122)       35 2023-04-26 08:21:35.000000 trexio-1.3.1/pytrexio/__init__.py
--rw-r--r--   0 runner    (1001) docker     (122)       22 2023-04-26 08:21:35.000000 trexio-1.3.1/pytrexio/_version.py
--rw-r--r--   0 runner    (1001) docker     (122)   264868 2023-04-26 08:24:16.000000 trexio-1.3.1/pytrexio/pytrexio.py
--rw-r--r--   0 runner    (1001) docker     (122)       52 2023-04-26 08:21:35.000000 trexio-1.3.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (122)      264 2023-04-26 08:25:43.967239 trexio-1.3.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (122)     4838 2023-04-26 08:21:35.000000 trexio-1.3.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-26 08:25:43.967239 trexio-1.3.1/src/
--rw-r--r--   0 runner    (1001) docker     (122)  2216321 2023-04-26 08:24:16.000000 trexio-1.3.1/src/pytrexio_wrap.c
--rw-r--r--   0 runner    (1001) docker     (122)  1344758 2023-04-26 08:24:16.000000 trexio-1.3.1/src/trexio.c
--rw-r--r--   0 runner    (1001) docker     (122)   163581 2023-04-26 08:24:16.000000 trexio-1.3.1/src/trexio.h
--rw-r--r--   0 runner    (1001) docker     (122)   658349 2023-04-26 08:24:16.000000 trexio-1.3.1/src/trexio_hdf5.c
--rw-r--r--   0 runner    (1001) docker     (122)    62512 2023-04-26 08:24:16.000000 trexio-1.3.1/src/trexio_hdf5.h
--rw-r--r--   0 runner    (1001) docker     (122)     1822 2023-04-26 08:24:16.000000 trexio-1.3.1/src/trexio_private.h
--rw-r--r--   0 runner    (1001) docker     (122)      668 2023-04-26 08:24:16.000000 trexio-1.3.1/src/trexio_s.h
--rw-r--r--   0 runner    (1001) docker     (122)   841272 2023-04-26 08:24:16.000000 trexio-1.3.1/src/trexio_text.c
--rw-r--r--   0 runner    (1001) docker     (122)    79312 2023-04-26 08:24:16.000000 trexio-1.3.1/src/trexio_text.h
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-26 08:25:43.967239 trexio-1.3.1/test/
--rw-r--r--   0 runner    (1001) docker     (122)     1466 2023-04-26 08:21:35.000000 trexio-1.3.1/test/benzene_data.py
--rw-r--r--   0 runner    (1001) docker     (122)    12197 2023-04-26 08:21:35.000000 trexio-1.3.1/test/test_api.py
--rw-r--r--   0 runner    (1001) docker     (122)     7652 2023-04-26 08:21:35.000000 trexio-1.3.1/test/test_pytrexio.py
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-26 08:25:43.967239 trexio-1.3.1/tools/
--rwxr-xr-x   0 runner    (1001) docker     (122)      106 2023-04-26 08:21:35.000000 trexio-1.3.1/tools/set_NUMPY_INCLUDEDIR.sh
-drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-26 08:25:43.967239 trexio-1.3.1/trexio.egg-info/
--rw-r--r--   0 runner    (1001) docker     (122)     5521 2023-04-26 08:25:43.000000 trexio-1.3.1/trexio.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (122)      808 2023-04-26 08:25:43.000000 trexio-1.3.1/trexio.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-04-26 08:25:43.000000 trexio-1.3.1/trexio.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (122)        1 2023-04-26 08:25:43.000000 trexio-1.3.1/trexio.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (122)       14 2023-04-26 08:25:43.000000 trexio-1.3.1/trexio.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (122)       16 2023-04-26 08:25:43.000000 trexio-1.3.1/trexio.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (122)   750503 2023-04-26 08:24:16.000000 trexio-1.3.1/trexio.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-05 15:09:27.193608 trexio-1.3.2/
+-rw-r--r--   0 runner    (1001) docker     (122)       39 2023-05-05 15:08:06.000000 trexio-1.3.2/AUTHORS
+-rw-r--r--   0 runner    (1001) docker     (122)     1533 2023-05-05 15:08:06.000000 trexio-1.3.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)      267 2023-05-05 15:06:36.000000 trexio-1.3.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)     5521 2023-05-05 15:09:27.193608 trexio-1.3.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     4573 2023-05-05 15:06:36.000000 trexio-1.3.2/README.md
+-rw-r--r--   0 runner    (1001) docker     (122)     1931 2023-05-05 15:06:36.000000 trexio-1.3.2/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-05 15:09:27.177608 trexio-1.3.2/pytrexio/
+-rw-r--r--   0 runner    (1001) docker     (122)       35 2023-05-05 15:06:36.000000 trexio-1.3.2/pytrexio/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)       22 2023-05-05 15:06:36.000000 trexio-1.3.2/pytrexio/_version.py
+-rw-r--r--   0 runner    (1001) docker     (122)   264868 2023-05-05 15:08:06.000000 trexio-1.3.2/pytrexio/pytrexio.py
+-rw-r--r--   0 runner    (1001) docker     (122)       52 2023-05-05 15:06:36.000000 trexio-1.3.2/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (122)      264 2023-05-05 15:09:27.193608 trexio-1.3.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     4838 2023-05-05 15:06:36.000000 trexio-1.3.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-05 15:09:27.189608 trexio-1.3.2/src/
+-rw-r--r--   0 runner    (1001) docker     (122)  2216365 2023-05-05 15:08:06.000000 trexio-1.3.2/src/pytrexio_wrap.c
+-rw-r--r--   0 runner    (1001) docker     (122)  1344758 2023-05-05 15:08:06.000000 trexio-1.3.2/src/trexio.c
+-rw-r--r--   0 runner    (1001) docker     (122)   163581 2023-05-05 15:08:06.000000 trexio-1.3.2/src/trexio.h
+-rw-r--r--   0 runner    (1001) docker     (122)   658349 2023-05-05 15:08:06.000000 trexio-1.3.2/src/trexio_hdf5.c
+-rw-r--r--   0 runner    (1001) docker     (122)    62512 2023-05-05 15:08:06.000000 trexio-1.3.2/src/trexio_hdf5.h
+-rw-r--r--   0 runner    (1001) docker     (122)     1822 2023-05-05 15:08:06.000000 trexio-1.3.2/src/trexio_private.h
+-rw-r--r--   0 runner    (1001) docker     (122)      668 2023-05-05 15:08:06.000000 trexio-1.3.2/src/trexio_s.h
+-rw-r--r--   0 runner    (1001) docker     (122)   841272 2023-05-05 15:08:06.000000 trexio-1.3.2/src/trexio_text.c
+-rw-r--r--   0 runner    (1001) docker     (122)    79312 2023-05-05 15:08:06.000000 trexio-1.3.2/src/trexio_text.h
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-05 15:09:27.189608 trexio-1.3.2/test/
+-rw-r--r--   0 runner    (1001) docker     (122)     1466 2023-05-05 15:06:36.000000 trexio-1.3.2/test/benzene_data.py
+-rw-r--r--   0 runner    (1001) docker     (122)    12197 2023-05-05 15:06:36.000000 trexio-1.3.2/test/test_api.py
+-rw-r--r--   0 runner    (1001) docker     (122)     7652 2023-05-05 15:06:36.000000 trexio-1.3.2/test/test_pytrexio.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-05 15:09:27.189608 trexio-1.3.2/tools/
+-rwxr-xr-x   0 runner    (1001) docker     (122)      106 2023-05-05 15:06:36.000000 trexio-1.3.2/tools/set_NUMPY_INCLUDEDIR.sh
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-05-05 15:09:27.193608 trexio-1.3.2/trexio.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     5521 2023-05-05 15:09:27.000000 trexio-1.3.2/trexio.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      808 2023-05-05 15:09:27.000000 trexio-1.3.2/trexio.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-05 15:09:27.000000 trexio-1.3.2/trexio.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-05-05 15:09:26.000000 trexio-1.3.2/trexio.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (122)       14 2023-05-05 15:09:27.000000 trexio-1.3.2/trexio.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       16 2023-05-05 15:09:27.000000 trexio-1.3.2/trexio.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)   750503 2023-05-05 15:08:06.000000 trexio-1.3.2/trexio.py
```

### Comparing `trexio-1.3.1/LICENSE` & `trexio-1.3.2/LICENSE`

 * *Files identical despite different names*

### Comparing `trexio-1.3.1/PKG-INFO` & `trexio-1.3.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trexio
-Version: 1.3.1
+Version: 1.3.2
 Summary: Python API of the TREXIO library
 Home-page: https://github.com/TREX-CoE/trexio
 Author: TREX-CoE
 Author-email: posenitskiy@irsamc.ups-tlse.fr
 License: BSD
 Project-URL: Bug Tracker, https://github.com/TREX-CoE/trexio/issues
 Classifier: Intended Audience :: Science/Research
```

### Comparing `trexio-1.3.1/README.md` & `trexio-1.3.2/README.md`

 * *Files identical despite different names*

### Comparing `trexio-1.3.1/pyproject.toml` & `trexio-1.3.2/pyproject.toml`

 * *Files identical despite different names*

### Comparing `trexio-1.3.1/pytrexio/pytrexio.py` & `trexio-1.3.2/pytrexio/pytrexio.py`

 * *Files identical despite different names*

### Comparing `trexio-1.3.1/setup.py` & `trexio-1.3.2/setup.py`

 * *Files identical despite different names*

### Comparing `trexio-1.3.1/src/pytrexio_wrap.c` & `trexio-1.3.2/src/pytrexio_wrap.c`

 * *Files 0% similar despite different names*

```diff
@@ -5781,15 +5781,15 @@
   if (!SWIG_IsOK(res1)) {
     SWIG_exception_fail(SWIG_ArgError(res1), "in method '" "trexio_read_metadata_code_num_64" "', argument " "1"" of type '" "trexio_t *const""'"); 
   }
   arg1 = (trexio_t *)(argp1);
   result = (trexio_exit_code)trexio_read_metadata_code_num_64(arg1,arg2);
   resultobj = SWIG_From_int((int)(result));
   if (SWIG_IsTmpObj(res2)) {
-    resultobj = SWIG_Python_AppendOutput(resultobj, SWIG_From_int((*arg2)));
+    resultobj = SWIG_Python_AppendOutput(resultobj, SWIG_From_long((*arg2)));
   } else {
     int new_flags = SWIG_IsNewObj(res2) ? (SWIG_POINTER_OWN |  0 ) :  0 ;
     resultobj = SWIG_Python_AppendOutput(resultobj, SWIG_NewPointerObj((void*)(arg2), SWIGTYPE_p_long, new_flags));
   }
   return resultobj;
 fail:
   return NULL;
@@ -5993,15 +5993,15 @@
   if (!SWIG_IsOK(res1)) {
     SWIG_exception_fail(SWIG_ArgError(res1), "in method '" "trexio_read_metadata_author_num_64" "', argument " "1"" of type '" "trexio_t *const""'"); 
   }
   arg1 = (trexio_t *)(argp1);
   result = (trexio_exit_code)trexio_read_metadata_author_num_64(arg1,arg2);
   resultobj = SWIG_From_int((int)(result));
   if (SWIG_IsTmpObj(res2)) {
-    resultobj = SWIG_Python_AppendOutput(resultobj, SWIG_From_int((*arg2)));
+    resultobj = SWIG_Python_AppendOutput(resultobj, SWIG_From_long((*arg2)));
   } else {
     int new_flags = SWIG_IsNewObj(res2) ? (SWIG_POINTER_OWN |  0 ) :  0 ;
     resultobj = SWIG_Python_AppendOutput(resultobj, SWIG_NewPointerObj((void*)(arg2), SWIGTYPE_p_long, new_flags));
   }
   return resultobj;
 fail:
   return NULL;
@@ -6205,15 +6205,15 @@
   if (!SWIG_IsOK(res1)) {
     SWIG_exception_fail(SWIG_ArgError(res1), "in method '" "trexio_read_metadata_unsafe_64" "', argument " "1"" of type '" "trexio_t *const""'"); 
   }
   arg1 = (trexio_t *)(argp1);
   result = (trexio_exit_code)trexio_read_metadata_unsafe_64(arg1,arg2);
   resultobj = SWIG_From_int((int)(result));
   if (SWIG_IsTmpObj(res2)) {
-    resultobj = SWIG_Python_AppendOutput(resultobj, SWIG_From_int((*arg2)));
+    resultobj = SWIG_Python_AppendOutput(resultobj, SWIG_From_long((*arg2)));
   } else {
     int new_flags = SWIG_IsNewObj(res2) ? (SWIG_POINTER_OWN |  0 ) :  0 ;
     resultobj = SWIG_Python_AppendOutput(resultobj, SWIG_NewPointerObj((void*)(arg2), SWIGTYPE_p_long, new_flags));
   }
   return resultobj;
 fail:
   return NULL;
@@ -6417,15 +6417,15 @@
   if (!SWIG_IsOK(res1)) {
     SWIG_exception_fail(SWIG_ArgError(res1), "in method '" "trexio_read_nucleus_num_64" "', argument " "1"" of type '" "trexio_t *const""'"); 
   }
   arg1 = (trexio_t *)(argp1);
   result = (trexio_exit_code)trexio_read_nucleus_num_64(arg1,arg2);
   resultobj = SWIG_From_int((int)(result));
   if (SWIG_IsTmpObj(res2)) {
-    resultobj = SWIG_Python_AppendOutput(resultobj, SWIG_From_int((*arg2)));
+    resultobj = SWIG_Python_AppendOutput(resultobj, SWIG_From_long((*arg2)));
   } else {
     int new_flags = SWIG_IsNewObj(res2) ? (SWIG_POINTER_OWN |  0 ) :  0 ;
     resultobj = SWIG_Python_AppendOutput(resultobj, SWIG_NewPointerObj((void*)(arg2), SWIGTYPE_p_long, new_flags));
   }
   return resultobj;
 fail:
   return NULL;
@@ -6503,15 +6503,15 @@
   if (!SWIG_IsOK(res1)) {
     SWIG_exception_fail(SWIG_ArgError(res1), "in method '" "trexio_read_nucleus_repulsion" "', argument " "1"" of type '" "trexio_t *const""'"); 
   }
   arg1 = (trexio_t *)(argp1);
   result = (trexio_exit_code)trexio_read_nucleus_repulsion(arg1,arg2);
   resultobj = SWIG_From_int((int)(result));
   if (SWIG_IsTmpObj(res2)) {
-    resultobj = SWIG_Python_AppendOutput(resultobj, SWIG_From_float((*arg2)));
+    resultobj = SWIG_Python_AppendOutput(resultobj, SWIG_From_double((*arg2)));
   } else {
     int new_flags = SWIG_IsNewObj(res2) ? (SWIG_POINTER_OWN |  0 ) :  0 ;
     resultobj = SWIG_Python_AppendOutput(resultobj, SWIG_NewPointerObj((void*)(arg2), SWIGTYPE_p_double, new_flags));
   }
   return resultobj;
 fail:
   return NULL;
@@ -6629,15 +6629,15 @@
   if (!SWIG_IsOK(res1)) {
     SWIG_exception_fail(SWIG_ArgError(res1), "in method '" "trexio_read_nucleus_repulsion_64" "', argument " "1"" of type '" "trexio_t *const""'"); 
   }
   arg1 = (trexio_t *)(argp1);
   result = (trexio_exit_code)trexio_read_nucleus_repulsion_64(arg1,arg2);
   resultobj = SWIG_From_int((int)(result));
   if (SWIG_IsTmpObj(res2)) {
-    resultobj = SWIG_Python_AppendOutput(resultobj, SWIG_From_float((*arg2)));
+    resultobj = SWIG_Python_AppendOutput(resultobj, SWIG_From_double((*arg2)));
   } else {
     int new_flags = SWIG_IsNewObj(res2) ? (SWIG_POINTER_OWN |  0 ) :  0 ;
     resultobj = SWIG_Python_AppendOutput(resultobj, SWIG_NewPointerObj((void*)(arg2), SWIGTYPE_p_double, new_flags));
   }
   return resultobj;
 fail:
   return NULL;
@@ -6841,15 +6841,15 @@
   if (!SWIG_IsOK(res1)) {
     SWIG_exception_fail(SWIG_ArgError(res1), "in method '" "trexio_read_cell_two_pi_64" "', argument " "1"" of type '" "trexio_t *const""'"); 
   }
   arg1 = (trexio_t *)(argp1);
   result = (trexio_exit_code)trexio_read_cell_two_pi_64(arg1,arg2);
   resultobj = SWIG_From_int((int)(result));
   if (SWIG_IsTmpObj(res2)) {
-    resultobj = SWIG_Python_AppendOutput(resultobj, SWIG_From_int((*arg2)));
+    resultobj = SWIG_Python_AppendOutput(resultobj, SWIG_From_long((*arg2)));
   } else {
     int new_flags = SWIG_IsNewObj(res2) ? (SWIG_POINTER_OWN |  0 ) :  0 ;
     resultobj = SWIG_Python_AppendOutput(resultobj, SWIG_NewPointerObj((void*)(arg2), SWIGTYPE_p_long, new_flags));
   }
   return resultobj;
 fail:
   return NULL;
@@ -7053,15 +7053,15 @@
   if (!SWIG_IsOK(res1)) {
     SWIG_exception_fail(SWIG_ArgError(res1), "in method '" "trexio_read_pbc_periodic_64" "', argument " "1"" of type '" "trexio_t *const""'"); 
   }
   arg1 = (trexio_t *)(argp1);
   result = (trexio_exit_code)trexio_read_pbc_periodic_64(arg1,arg2);
   resultobj = SWIG_From_int((int)(result));
   if (SWIG_IsTmpObj(res2)) {
-    resultobj = SWIG_Python_AppendOutput(resultobj, SWIG_From_int((*arg2)));
+    resultobj = SWIG_Python_AppendOutput(resultobj, SWIG_From_long((*arg2)));
   } else {
     int new_flags = SWIG_IsNewObj(res2) ? (SWIG_POINTER_OWN |  0 ) :  0 ;
     resultobj = SWIG_Python_AppendOutput(resultobj, SWIG_NewPointerObj((void*)(arg2), SWIGTYPE_p_long, new_flags));
   }
   return resultobj;
 fail:
   return NULL;
@@ -7265,15 +7265,15 @@
   if (!SWIG_IsOK(res1)) {
     SWIG_exception_fail(SWIG_ArgError(res1), "in method '" "trexio_read_electron_num_64" "', argument " "1"" of type '" "trexio_t *const""'"); 
   }
   arg1 = (trexio_t *)(argp1);
   result = (trexio_exit_code)trexio_read_electron_num_64(arg1,arg2);
   resultobj = SWIG_From_int((int)(result));
   if (SWIG_IsTmpObj(res2)) {
-    resultobj = SWIG_Python_AppendOutput(resultobj, SWIG_From_int((*arg2)));
+    resultobj = SWIG_Python_AppendOutput(resultobj, SWIG_From_long((*arg2)));
   } else {
     int new_flags = SWIG_IsNewObj(res2) ? (SWIG_POINTER_OWN |  0 ) :  0 ;
     resultobj = SWIG_Python_AppendOutput(resultobj, SWIG_NewPointerObj((void*)(arg2), SWIGTYPE_p_long, new_flags));
   }
   return resultobj;
 fail:
   return NULL;
@@ -7477,15 +7477,15 @@
   if (!SWIG_IsOK(res1)) {
     SWIG_exception_fail(SWIG_ArgError(res1), "in method '" "trexio_read_electron_up_num_64" "', argument " "1"" of type '" "trexio_t *const""'"); 
   }
   arg1 = (trexio_t *)(argp1);
   result = (trexio_exit_code)trexio_read_electron_up_num_64(arg1,arg2);
   resultobj = SWIG_From_int((int)(result));
   if (SWIG_IsTmpObj(res2)) {
-    resultobj = SWIG_Python_AppendOutput(resultobj, SWIG_From_int((*arg2)));
+    resultobj = SWIG_Python_AppendOutput(resultobj, SWIG_From_long((*arg2)));
   } else {
     int new_flags = SWIG_IsNewObj(res2) ? (SWIG_POINTER_OWN |  0 ) :  0 ;
     resultobj = SWIG_Python_AppendOutput(resultobj, SWIG_NewPointerObj((void*)(arg2), SWIGTYPE_p_long, new_flags));
   }
   return resultobj;
 fail:
   return NULL;
@@ -7689,15 +7689,15 @@
   if (!SWIG_IsOK(res1)) {
     SWIG_exception_fail(SWIG_ArgError(res1), "in method '" "trexio_read_electron_dn_num_64" "', argument " "1"" of type '" "trexio_t *const""'"); 
   }
   arg1 = (trexio_t *)(argp1);
   result = (trexio_exit_code)trexio_read_electron_dn_num_64(arg1,arg2);
   resultobj = SWIG_From_int((int)(result));
   if (SWIG_IsTmpObj(res2)) {
-    resultobj = SWIG_Python_AppendOutput(resultobj, SWIG_From_int((*arg2)));
+    resultobj = SWIG_Python_AppendOutput(resultobj, SWIG_From_long((*arg2)));
   } else {
     int new_flags = SWIG_IsNewObj(res2) ? (SWIG_POINTER_OWN |  0 ) :  0 ;
     resultobj = SWIG_Python_AppendOutput(resultobj, SWIG_NewPointerObj((void*)(arg2), SWIGTYPE_p_long, new_flags));
   }
   return resultobj;
 fail:
   return NULL;
@@ -7901,15 +7901,15 @@
   if (!SWIG_IsOK(res1)) {
     SWIG_exception_fail(SWIG_ArgError(res1), "in method '" "trexio_read_state_num_64" "', argument " "1"" of type '" "trexio_t *const""'"); 
   }
   arg1 = (trexio_t *)(argp1);
   result = (trexio_exit_code)trexio_read_state_num_64(arg1,arg2);
   resultobj = SWIG_From_int((int)(result));
   if (SWIG_IsTmpObj(res2)) {
-    resultobj = SWIG_Python_AppendOutput(resultobj, SWIG_From_int((*arg2)));
+    resultobj = SWIG_Python_AppendOutput(resultobj, SWIG_From_long((*arg2)));
   } else {
     int new_flags = SWIG_IsNewObj(res2) ? (SWIG_POINTER_OWN |  0 ) :  0 ;
     resultobj = SWIG_Python_AppendOutput(resultobj, SWIG_NewPointerObj((void*)(arg2), SWIGTYPE_p_long, new_flags));
   }
   return resultobj;
 fail:
   return NULL;
@@ -8113,15 +8113,15 @@
   if (!SWIG_IsOK(res1)) {
     SWIG_exception_fail(SWIG_ArgError(res1), "in method '" "trexio_read_state_id_64" "', argument " "1"" of type '" "trexio_t *const""'"); 
   }
   arg1 = (trexio_t *)(argp1);
   result = (trexio_exit_code)trexio_read_state_id_64(arg1,arg2);
   resultobj = SWIG_From_int((int)(result));
   if (SWIG_IsTmpObj(res2)) {
-    resultobj = SWIG_Python_AppendOutput(resultobj, SWIG_From_int((*arg2)));
+    resultobj = SWIG_Python_AppendOutput(resultobj, SWIG_From_long((*arg2)));
   } else {
     int new_flags = SWIG_IsNewObj(res2) ? (SWIG_POINTER_OWN |  0 ) :  0 ;
     resultobj = SWIG_Python_AppendOutput(resultobj, SWIG_NewPointerObj((void*)(arg2), SWIGTYPE_p_long, new_flags));
   }
   return resultobj;
 fail:
   return NULL;
@@ -8325,15 +8325,15 @@
   if (!SWIG_IsOK(res1)) {
     SWIG_exception_fail(SWIG_ArgError(res1), "in method '" "trexio_read_basis_prim_num_64" "', argument " "1"" of type '" "trexio_t *const""'"); 
   }
   arg1 = (trexio_t *)(argp1);
   result = (trexio_exit_code)trexio_read_basis_prim_num_64(arg1,arg2);
   resultobj = SWIG_From_int((int)(result));
   if (SWIG_IsTmpObj(res2)) {
-    resultobj = SWIG_Python_AppendOutput(resultobj, SWIG_From_int((*arg2)));
+    resultobj = SWIG_Python_AppendOutput(resultobj, SWIG_From_long((*arg2)));
   } else {
     int new_flags = SWIG_IsNewObj(res2) ? (SWIG_POINTER_OWN |  0 ) :  0 ;
     resultobj = SWIG_Python_AppendOutput(resultobj, SWIG_NewPointerObj((void*)(arg2), SWIGTYPE_p_long, new_flags));
   }
   return resultobj;
 fail:
   return NULL;
@@ -8537,15 +8537,15 @@
   if (!SWIG_IsOK(res1)) {
     SWIG_exception_fail(SWIG_ArgError(res1), "in method '" "trexio_read_basis_shell_num_64" "', argument " "1"" of type '" "trexio_t *const""'"); 
   }
   arg1 = (trexio_t *)(argp1);
   result = (trexio_exit_code)trexio_read_basis_shell_num_64(arg1,arg2);
   resultobj = SWIG_From_int((int)(result));
   if (SWIG_IsTmpObj(res2)) {
-    resultobj = SWIG_Python_AppendOutput(resultobj, SWIG_From_int((*arg2)));
+    resultobj = SWIG_Python_AppendOutput(resultobj, SWIG_From_long((*arg2)));
   } else {
     int new_flags = SWIG_IsNewObj(res2) ? (SWIG_POINTER_OWN |  0 ) :  0 ;
     resultobj = SWIG_Python_AppendOutput(resultobj, SWIG_NewPointerObj((void*)(arg2), SWIGTYPE_p_long, new_flags));
   }
   return resultobj;
 fail:
   return NULL;
@@ -8623,15 +8623,15 @@
   if (!SWIG_IsOK(res1)) {
     SWIG_exception_fail(SWIG_ArgError(res1), "in method '" "trexio_read_basis_e_cut" "', argument " "1"" of type '" "trexio_t *const""'"); 
   }
   arg1 = (trexio_t *)(argp1);
   result = (trexio_exit_code)trexio_read_basis_e_cut(arg1,arg2);
   resultobj = SWIG_From_int((int)(result));
   if (SWIG_IsTmpObj(res2)) {
-    resultobj = SWIG_Python_AppendOutput(resultobj, SWIG_From_float((*arg2)));
+    resultobj = SWIG_Python_AppendOutput(resultobj, SWIG_From_double((*arg2)));
   } else {
     int new_flags = SWIG_IsNewObj(res2) ? (SWIG_POINTER_OWN |  0 ) :  0 ;
     resultobj = SWIG_Python_AppendOutput(resultobj, SWIG_NewPointerObj((void*)(arg2), SWIGTYPE_p_double, new_flags));
   }
   return resultobj;
 fail:
   return NULL;
@@ -8749,15 +8749,15 @@
   if (!SWIG_IsOK(res1)) {
     SWIG_exception_fail(SWIG_ArgError(res1), "in method '" "trexio_read_basis_e_cut_64" "', argument " "1"" of type '" "trexio_t *const""'"); 
   }
   arg1 = (trexio_t *)(argp1);
   result = (trexio_exit_code)trexio_read_basis_e_cut_64(arg1,arg2);
   resultobj = SWIG_From_int((int)(result));
   if (SWIG_IsTmpObj(res2)) {
-    resultobj = SWIG_Python_AppendOutput(resultobj, SWIG_From_float((*arg2)));
+    resultobj = SWIG_Python_AppendOutput(resultobj, SWIG_From_double((*arg2)));
   } else {
     int new_flags = SWIG_IsNewObj(res2) ? (SWIG_POINTER_OWN |  0 ) :  0 ;
     resultobj = SWIG_Python_AppendOutput(resultobj, SWIG_NewPointerObj((void*)(arg2), SWIGTYPE_p_double, new_flags));
   }
   return resultobj;
 fail:
   return NULL;
@@ -8961,15 +8961,15 @@
   if (!SWIG_IsOK(res1)) {
     SWIG_exception_fail(SWIG_ArgError(res1), "in method '" "trexio_read_ecp_num_64" "', argument " "1"" of type '" "trexio_t *const""'"); 
   }
   arg1 = (trexio_t *)(argp1);
   result = (trexio_exit_code)trexio_read_ecp_num_64(arg1,arg2);
   resultobj = SWIG_From_int((int)(result));
   if (SWIG_IsTmpObj(res2)) {
-    resultobj = SWIG_Python_AppendOutput(resultobj, SWIG_From_int((*arg2)));
+    resultobj = SWIG_Python_AppendOutput(resultobj, SWIG_From_long((*arg2)));
   } else {
     int new_flags = SWIG_IsNewObj(res2) ? (SWIG_POINTER_OWN |  0 ) :  0 ;
     resultobj = SWIG_Python_AppendOutput(resultobj, SWIG_NewPointerObj((void*)(arg2), SWIGTYPE_p_long, new_flags));
   }
   return resultobj;
 fail:
   return NULL;
@@ -9047,15 +9047,15 @@
   if (!SWIG_IsOK(res1)) {
     SWIG_exception_fail(SWIG_ArgError(res1), "in method '" "trexio_read_grid_rad_precision" "', argument " "1"" of type '" "trexio_t *const""'"); 
   }
   arg1 = (trexio_t *)(argp1);
   result = (trexio_exit_code)trexio_read_grid_rad_precision(arg1,arg2);
   resultobj = SWIG_From_int((int)(result));
   if (SWIG_IsTmpObj(res2)) {
-    resultobj = SWIG_Python_AppendOutput(resultobj, SWIG_From_float((*arg2)));
+    resultobj = SWIG_Python_AppendOutput(resultobj, SWIG_From_double((*arg2)));
   } else {
     int new_flags = SWIG_IsNewObj(res2) ? (SWIG_POINTER_OWN |  0 ) :  0 ;
     resultobj = SWIG_Python_AppendOutput(resultobj, SWIG_NewPointerObj((void*)(arg2), SWIGTYPE_p_double, new_flags));
   }
   return resultobj;
 fail:
   return NULL;
@@ -9173,15 +9173,15 @@
   if (!SWIG_IsOK(res1)) {
     SWIG_exception_fail(SWIG_ArgError(res1), "in method '" "trexio_read_grid_rad_precision_64" "', argument " "1"" of type '" "trexio_t *const""'"); 
   }
   arg1 = (trexio_t *)(argp1);
   result = (trexio_exit_code)trexio_read_grid_rad_precision_64(arg1,arg2);
   resultobj = SWIG_From_int((int)(result));
   if (SWIG_IsTmpObj(res2)) {
-    resultobj = SWIG_Python_AppendOutput(resultobj, SWIG_From_float((*arg2)));
+    resultobj = SWIG_Python_AppendOutput(resultobj, SWIG_From_double((*arg2)));
   } else {
     int new_flags = SWIG_IsNewObj(res2) ? (SWIG_POINTER_OWN |  0 ) :  0 ;
     resultobj = SWIG_Python_AppendOutput(resultobj, SWIG_NewPointerObj((void*)(arg2), SWIGTYPE_p_double, new_flags));
   }
   return resultobj;
 fail:
   return NULL;
@@ -9385,15 +9385,15 @@
   if (!SWIG_IsOK(res1)) {
     SWIG_exception_fail(SWIG_ArgError(res1), "in method '" "trexio_read_grid_num_64" "', argument " "1"" of type '" "trexio_t *const""'"); 
   }
   arg1 = (trexio_t *)(argp1);
   result = (trexio_exit_code)trexio_read_grid_num_64(arg1,arg2);
   resultobj = SWIG_From_int((int)(result));
   if (SWIG_IsTmpObj(res2)) {
-    resultobj = SWIG_Python_AppendOutput(resultobj, SWIG_From_int((*arg2)));
+    resultobj = SWIG_Python_AppendOutput(resultobj, SWIG_From_long((*arg2)));
   } else {
     int new_flags = SWIG_IsNewObj(res2) ? (SWIG_POINTER_OWN |  0 ) :  0 ;
     resultobj = SWIG_Python_AppendOutput(resultobj, SWIG_NewPointerObj((void*)(arg2), SWIGTYPE_p_long, new_flags));
   }
   return resultobj;
 fail:
   return NULL;
@@ -9597,15 +9597,15 @@
   if (!SWIG_IsOK(res1)) {
     SWIG_exception_fail(SWIG_ArgError(res1), "in method '" "trexio_read_grid_max_ang_num_64" "', argument " "1"" of type '" "trexio_t *const""'"); 
   }
   arg1 = (trexio_t *)(argp1);
   result = (trexio_exit_code)trexio_read_grid_max_ang_num_64(arg1,arg2);
   resultobj = SWIG_From_int((int)(result));
   if (SWIG_IsTmpObj(res2)) {
-    resultobj = SWIG_Python_AppendOutput(resultobj, SWIG_From_int((*arg2)));
+    resultobj = SWIG_Python_AppendOutput(resultobj, SWIG_From_long((*arg2)));
   } else {
     int new_flags = SWIG_IsNewObj(res2) ? (SWIG_POINTER_OWN |  0 ) :  0 ;
     resultobj = SWIG_Python_AppendOutput(resultobj, SWIG_NewPointerObj((void*)(arg2), SWIGTYPE_p_long, new_flags));
   }
   return resultobj;
 fail:
   return NULL;
@@ -9809,15 +9809,15 @@
   if (!SWIG_IsOK(res1)) {
     SWIG_exception_fail(SWIG_ArgError(res1), "in method '" "trexio_read_grid_min_ang_num_64" "', argument " "1"" of type '" "trexio_t *const""'"); 
   }
   arg1 = (trexio_t *)(argp1);
   result = (trexio_exit_code)trexio_read_grid_min_ang_num_64(arg1,arg2);
   resultobj = SWIG_From_int((int)(result));
   if (SWIG_IsTmpObj(res2)) {
-    resultobj = SWIG_Python_AppendOutput(resultobj, SWIG_From_int((*arg2)));
+    resultobj = SWIG_Python_AppendOutput(resultobj, SWIG_From_long((*arg2)));
   } else {
     int new_flags = SWIG_IsNewObj(res2) ? (SWIG_POINTER_OWN |  0 ) :  0 ;
     resultobj = SWIG_Python_AppendOutput(resultobj, SWIG_NewPointerObj((void*)(arg2), SWIGTYPE_p_long, new_flags));
   }
   return resultobj;
 fail:
   return NULL;
@@ -10021,15 +10021,15 @@
   if (!SWIG_IsOK(res1)) {
     SWIG_exception_fail(SWIG_ArgError(res1), "in method '" "trexio_read_grid_ang_num_64" "', argument " "1"" of type '" "trexio_t *const""'"); 
   }
   arg1 = (trexio_t *)(argp1);
   result = (trexio_exit_code)trexio_read_grid_ang_num_64(arg1,arg2);
   resultobj = SWIG_From_int((int)(result));
   if (SWIG_IsTmpObj(res2)) {
-    resultobj = SWIG_Python_AppendOutput(resultobj, SWIG_From_int((*arg2)));
+    resultobj = SWIG_Python_AppendOutput(resultobj, SWIG_From_long((*arg2)));
   } else {
     int new_flags = SWIG_IsNewObj(res2) ? (SWIG_POINTER_OWN |  0 ) :  0 ;
     resultobj = SWIG_Python_AppendOutput(resultobj, SWIG_NewPointerObj((void*)(arg2), SWIGTYPE_p_long, new_flags));
   }
   return resultobj;
 fail:
   return NULL;
@@ -10233,15 +10233,15 @@
   if (!SWIG_IsOK(res1)) {
     SWIG_exception_fail(SWIG_ArgError(res1), "in method '" "trexio_read_grid_rad_num_64" "', argument " "1"" of type '" "trexio_t *const""'"); 
   }
   arg1 = (trexio_t *)(argp1);
   result = (trexio_exit_code)trexio_read_grid_rad_num_64(arg1,arg2);
   resultobj = SWIG_From_int((int)(result));
   if (SWIG_IsTmpObj(res2)) {
-    resultobj = SWIG_Python_AppendOutput(resultobj, SWIG_From_int((*arg2)));
+    resultobj = SWIG_Python_AppendOutput(resultobj, SWIG_From_long((*arg2)));
   } else {
     int new_flags = SWIG_IsNewObj(res2) ? (SWIG_POINTER_OWN |  0 ) :  0 ;
     resultobj = SWIG_Python_AppendOutput(resultobj, SWIG_NewPointerObj((void*)(arg2), SWIGTYPE_p_long, new_flags));
   }
   return resultobj;
 fail:
   return NULL;
@@ -10445,15 +10445,15 @@
   if (!SWIG_IsOK(res1)) {
     SWIG_exception_fail(SWIG_ArgError(res1), "in method '" "trexio_read_ao_cartesian_64" "', argument " "1"" of type '" "trexio_t *const""'"); 
   }
   arg1 = (trexio_t *)(argp1);
   result = (trexio_exit_code)trexio_read_ao_cartesian_64(arg1,arg2);
   resultobj = SWIG_From_int((int)(result));
   if (SWIG_IsTmpObj(res2)) {
-    resultobj = SWIG_Python_AppendOutput(resultobj, SWIG_From_int((*arg2)));
+    resultobj = SWIG_Python_AppendOutput(resultobj, SWIG_From_long((*arg2)));
   } else {
     int new_flags = SWIG_IsNewObj(res2) ? (SWIG_POINTER_OWN |  0 ) :  0 ;
     resultobj = SWIG_Python_AppendOutput(resultobj, SWIG_NewPointerObj((void*)(arg2), SWIGTYPE_p_long, new_flags));
   }
   return resultobj;
 fail:
   return NULL;
@@ -10657,15 +10657,15 @@
   if (!SWIG_IsOK(res1)) {
     SWIG_exception_fail(SWIG_ArgError(res1), "in method '" "trexio_read_ao_num_64" "', argument " "1"" of type '" "trexio_t *const""'"); 
   }
   arg1 = (trexio_t *)(argp1);
   result = (trexio_exit_code)trexio_read_ao_num_64(arg1,arg2);
   resultobj = SWIG_From_int((int)(result));
   if (SWIG_IsTmpObj(res2)) {
-    resultobj = SWIG_Python_AppendOutput(resultobj, SWIG_From_int((*arg2)));
+    resultobj = SWIG_Python_AppendOutput(resultobj, SWIG_From_long((*arg2)));
   } else {
     int new_flags = SWIG_IsNewObj(res2) ? (SWIG_POINTER_OWN |  0 ) :  0 ;
     resultobj = SWIG_Python_AppendOutput(resultobj, SWIG_NewPointerObj((void*)(arg2), SWIGTYPE_p_long, new_flags));
   }
   return resultobj;
 fail:
   return NULL;
@@ -10869,15 +10869,15 @@
   if (!SWIG_IsOK(res1)) {
     SWIG_exception_fail(SWIG_ArgError(res1), "in method '" "trexio_read_ao_2e_int_eri_cholesky_num_64" "', argument " "1"" of type '" "trexio_t *const""'"); 
   }
   arg1 = (trexio_t *)(argp1);
   result = (trexio_exit_code)trexio_read_ao_2e_int_eri_cholesky_num_64(arg1,arg2);
   resultobj = SWIG_From_int((int)(result));
   if (SWIG_IsTmpObj(res2)) {
-    resultobj = SWIG_Python_AppendOutput(resultobj, SWIG_From_int((*arg2)));
+    resultobj = SWIG_Python_AppendOutput(resultobj, SWIG_From_long((*arg2)));
   } else {
     int new_flags = SWIG_IsNewObj(res2) ? (SWIG_POINTER_OWN |  0 ) :  0 ;
     resultobj = SWIG_Python_AppendOutput(resultobj, SWIG_NewPointerObj((void*)(arg2), SWIGTYPE_p_long, new_flags));
   }
   return resultobj;
 fail:
   return NULL;
@@ -11081,15 +11081,15 @@
   if (!SWIG_IsOK(res1)) {
     SWIG_exception_fail(SWIG_ArgError(res1), "in method '" "trexio_read_ao_2e_int_eri_lr_cholesky_num_64" "', argument " "1"" of type '" "trexio_t *const""'"); 
   }
   arg1 = (trexio_t *)(argp1);
   result = (trexio_exit_code)trexio_read_ao_2e_int_eri_lr_cholesky_num_64(arg1,arg2);
   resultobj = SWIG_From_int((int)(result));
   if (SWIG_IsTmpObj(res2)) {
-    resultobj = SWIG_Python_AppendOutput(resultobj, SWIG_From_int((*arg2)));
+    resultobj = SWIG_Python_AppendOutput(resultobj, SWIG_From_long((*arg2)));
   } else {
     int new_flags = SWIG_IsNewObj(res2) ? (SWIG_POINTER_OWN |  0 ) :  0 ;
     resultobj = SWIG_Python_AppendOutput(resultobj, SWIG_NewPointerObj((void*)(arg2), SWIGTYPE_p_long, new_flags));
   }
   return resultobj;
 fail:
   return NULL;
@@ -11293,15 +11293,15 @@
   if (!SWIG_IsOK(res1)) {
     SWIG_exception_fail(SWIG_ArgError(res1), "in method '" "trexio_read_mo_num_64" "', argument " "1"" of type '" "trexio_t *const""'"); 
   }
   arg1 = (trexio_t *)(argp1);
   result = (trexio_exit_code)trexio_read_mo_num_64(arg1,arg2);
   resultobj = SWIG_From_int((int)(result));
   if (SWIG_IsTmpObj(res2)) {
-    resultobj = SWIG_Python_AppendOutput(resultobj, SWIG_From_int((*arg2)));
+    resultobj = SWIG_Python_AppendOutput(resultobj, SWIG_From_long((*arg2)));
   } else {
     int new_flags = SWIG_IsNewObj(res2) ? (SWIG_POINTER_OWN |  0 ) :  0 ;
     resultobj = SWIG_Python_AppendOutput(resultobj, SWIG_NewPointerObj((void*)(arg2), SWIGTYPE_p_long, new_flags));
   }
   return resultobj;
 fail:
   return NULL;
@@ -11505,15 +11505,15 @@
   if (!SWIG_IsOK(res1)) {
     SWIG_exception_fail(SWIG_ArgError(res1), "in method '" "trexio_read_mo_2e_int_eri_cholesky_num_64" "', argument " "1"" of type '" "trexio_t *const""'"); 
   }
   arg1 = (trexio_t *)(argp1);
   result = (trexio_exit_code)trexio_read_mo_2e_int_eri_cholesky_num_64(arg1,arg2);
   resultobj = SWIG_From_int((int)(result));
   if (SWIG_IsTmpObj(res2)) {
-    resultobj = SWIG_Python_AppendOutput(resultobj, SWIG_From_int((*arg2)));
+    resultobj = SWIG_Python_AppendOutput(resultobj, SWIG_From_long((*arg2)));
   } else {
     int new_flags = SWIG_IsNewObj(res2) ? (SWIG_POINTER_OWN |  0 ) :  0 ;
     resultobj = SWIG_Python_AppendOutput(resultobj, SWIG_NewPointerObj((void*)(arg2), SWIGTYPE_p_long, new_flags));
   }
   return resultobj;
 fail:
   return NULL;
@@ -11717,15 +11717,15 @@
   if (!SWIG_IsOK(res1)) {
     SWIG_exception_fail(SWIG_ArgError(res1), "in method '" "trexio_read_mo_2e_int_eri_lr_cholesky_num_64" "', argument " "1"" of type '" "trexio_t *const""'"); 
   }
   arg1 = (trexio_t *)(argp1);
   result = (trexio_exit_code)trexio_read_mo_2e_int_eri_lr_cholesky_num_64(arg1,arg2);
   resultobj = SWIG_From_int((int)(result));
   if (SWIG_IsTmpObj(res2)) {
-    resultobj = SWIG_Python_AppendOutput(resultobj, SWIG_From_int((*arg2)));
+    resultobj = SWIG_Python_AppendOutput(resultobj, SWIG_From_long((*arg2)));
   } else {
     int new_flags = SWIG_IsNewObj(res2) ? (SWIG_POINTER_OWN |  0 ) :  0 ;
     resultobj = SWIG_Python_AppendOutput(resultobj, SWIG_NewPointerObj((void*)(arg2), SWIGTYPE_p_long, new_flags));
   }
   return resultobj;
 fail:
   return NULL;
@@ -11869,15 +11869,15 @@
   if (!SWIG_IsOK(res1)) {
     SWIG_exception_fail(SWIG_ArgError(res1), "in method '" "trexio_read_determinant_num_64" "', argument " "1"" of type '" "trexio_t *const""'"); 
   }
   arg1 = (trexio_t *)(argp1);
   result = (trexio_exit_code)trexio_read_determinant_num_64(arg1,arg2);
   resultobj = SWIG_From_int((int)(result));
   if (SWIG_IsTmpObj(res2)) {
-    resultobj = SWIG_Python_AppendOutput(resultobj, SWIG_From_int((*arg2)));
+    resultobj = SWIG_Python_AppendOutput(resultobj, SWIG_From_long((*arg2)));
   } else {
     int new_flags = SWIG_IsNewObj(res2) ? (SWIG_POINTER_OWN |  0 ) :  0 ;
     resultobj = SWIG_Python_AppendOutput(resultobj, SWIG_NewPointerObj((void*)(arg2), SWIGTYPE_p_long, new_flags));
   }
   return resultobj;
 fail:
   return NULL;
@@ -11991,15 +11991,15 @@
   if (!SWIG_IsOK(res1)) {
     SWIG_exception_fail(SWIG_ArgError(res1), "in method '" "trexio_read_csf_num_64" "', argument " "1"" of type '" "trexio_t *const""'"); 
   }
   arg1 = (trexio_t *)(argp1);
   result = (trexio_exit_code)trexio_read_csf_num_64(arg1,arg2);
   resultobj = SWIG_From_int((int)(result));
   if (SWIG_IsTmpObj(res2)) {
-    resultobj = SWIG_Python_AppendOutput(resultobj, SWIG_From_int((*arg2)));
+    resultobj = SWIG_Python_AppendOutput(resultobj, SWIG_From_long((*arg2)));
   } else {
     int new_flags = SWIG_IsNewObj(res2) ? (SWIG_POINTER_OWN |  0 ) :  0 ;
     resultobj = SWIG_Python_AppendOutput(resultobj, SWIG_NewPointerObj((void*)(arg2), SWIGTYPE_p_long, new_flags));
   }
   return resultobj;
 fail:
   return NULL;
@@ -12173,15 +12173,15 @@
   if (!SWIG_IsOK(res1)) {
     SWIG_exception_fail(SWIG_ArgError(res1), "in method '" "trexio_read_rdm_2e_cholesky_num_64" "', argument " "1"" of type '" "trexio_t *const""'"); 
   }
   arg1 = (trexio_t *)(argp1);
   result = (trexio_exit_code)trexio_read_rdm_2e_cholesky_num_64(arg1,arg2);
   resultobj = SWIG_From_int((int)(result));
   if (SWIG_IsTmpObj(res2)) {
-    resultobj = SWIG_Python_AppendOutput(resultobj, SWIG_From_int((*arg2)));
+    resultobj = SWIG_Python_AppendOutput(resultobj, SWIG_From_long((*arg2)));
   } else {
     int new_flags = SWIG_IsNewObj(res2) ? (SWIG_POINTER_OWN |  0 ) :  0 ;
     resultobj = SWIG_Python_AppendOutput(resultobj, SWIG_NewPointerObj((void*)(arg2), SWIGTYPE_p_long, new_flags));
   }
   return resultobj;
 fail:
   return NULL;
@@ -12385,15 +12385,15 @@
   if (!SWIG_IsOK(res1)) {
     SWIG_exception_fail(SWIG_ArgError(res1), "in method '" "trexio_read_rdm_2e_upup_cholesky_num_64" "', argument " "1"" of type '" "trexio_t *const""'"); 
   }
   arg1 = (trexio_t *)(argp1);
   result = (trexio_exit_code)trexio_read_rdm_2e_upup_cholesky_num_64(arg1,arg2);
   resultobj = SWIG_From_int((int)(result));
   if (SWIG_IsTmpObj(res2)) {
-    resultobj = SWIG_Python_AppendOutput(resultobj, SWIG_From_int((*arg2)));
+    resultobj = SWIG_Python_AppendOutput(resultobj, SWIG_From_long((*arg2)));
   } else {
     int new_flags = SWIG_IsNewObj(res2) ? (SWIG_POINTER_OWN |  0 ) :  0 ;
     resultobj = SWIG_Python_AppendOutput(resultobj, SWIG_NewPointerObj((void*)(arg2), SWIGTYPE_p_long, new_flags));
   }
   return resultobj;
 fail:
   return NULL;
@@ -12597,15 +12597,15 @@
   if (!SWIG_IsOK(res1)) {
     SWIG_exception_fail(SWIG_ArgError(res1), "in method '" "trexio_read_rdm_2e_dndn_cholesky_num_64" "', argument " "1"" of type '" "trexio_t *const""'"); 
   }
   arg1 = (trexio_t *)(argp1);
   result = (trexio_exit_code)trexio_read_rdm_2e_dndn_cholesky_num_64(arg1,arg2);
   resultobj = SWIG_From_int((int)(result));
   if (SWIG_IsTmpObj(res2)) {
-    resultobj = SWIG_Python_AppendOutput(resultobj, SWIG_From_int((*arg2)));
+    resultobj = SWIG_Python_AppendOutput(resultobj, SWIG_From_long((*arg2)));
   } else {
     int new_flags = SWIG_IsNewObj(res2) ? (SWIG_POINTER_OWN |  0 ) :  0 ;
     resultobj = SWIG_Python_AppendOutput(resultobj, SWIG_NewPointerObj((void*)(arg2), SWIGTYPE_p_long, new_flags));
   }
   return resultobj;
 fail:
   return NULL;
@@ -12809,15 +12809,15 @@
   if (!SWIG_IsOK(res1)) {
     SWIG_exception_fail(SWIG_ArgError(res1), "in method '" "trexio_read_rdm_2e_updn_cholesky_num_64" "', argument " "1"" of type '" "trexio_t *const""'"); 
   }
   arg1 = (trexio_t *)(argp1);
   result = (trexio_exit_code)trexio_read_rdm_2e_updn_cholesky_num_64(arg1,arg2);
   resultobj = SWIG_From_int((int)(result));
   if (SWIG_IsTmpObj(res2)) {
-    resultobj = SWIG_Python_AppendOutput(resultobj, SWIG_From_int((*arg2)));
+    resultobj = SWIG_Python_AppendOutput(resultobj, SWIG_From_long((*arg2)));
   } else {
     int new_flags = SWIG_IsNewObj(res2) ? (SWIG_POINTER_OWN |  0 ) :  0 ;
     resultobj = SWIG_Python_AppendOutput(resultobj, SWIG_NewPointerObj((void*)(arg2), SWIGTYPE_p_long, new_flags));
   }
   return resultobj;
 fail:
   return NULL;
@@ -13021,15 +13021,15 @@
   if (!SWIG_IsOK(res1)) {
     SWIG_exception_fail(SWIG_ArgError(res1), "in method '" "trexio_read_jastrow_en_num_64" "', argument " "1"" of type '" "trexio_t *const""'"); 
   }
   arg1 = (trexio_t *)(argp1);
   result = (trexio_exit_code)trexio_read_jastrow_en_num_64(arg1,arg2);
   resultobj = SWIG_From_int((int)(result));
   if (SWIG_IsTmpObj(res2)) {
-    resultobj = SWIG_Python_AppendOutput(resultobj, SWIG_From_int((*arg2)));
+    resultobj = SWIG_Python_AppendOutput(resultobj, SWIG_From_long((*arg2)));
   } else {
     int new_flags = SWIG_IsNewObj(res2) ? (SWIG_POINTER_OWN |  0 ) :  0 ;
     resultobj = SWIG_Python_AppendOutput(resultobj, SWIG_NewPointerObj((void*)(arg2), SWIGTYPE_p_long, new_flags));
   }
   return resultobj;
 fail:
   return NULL;
@@ -13233,15 +13233,15 @@
   if (!SWIG_IsOK(res1)) {
     SWIG_exception_fail(SWIG_ArgError(res1), "in method '" "trexio_read_jastrow_ee_num_64" "', argument " "1"" of type '" "trexio_t *const""'"); 
   }
   arg1 = (trexio_t *)(argp1);
   result = (trexio_exit_code)trexio_read_jastrow_ee_num_64(arg1,arg2);
   resultobj = SWIG_From_int((int)(result));
   if (SWIG_IsTmpObj(res2)) {
-    resultobj = SWIG_Python_AppendOutput(resultobj, SWIG_From_int((*arg2)));
+    resultobj = SWIG_Python_AppendOutput(resultobj, SWIG_From_long((*arg2)));
   } else {
     int new_flags = SWIG_IsNewObj(res2) ? (SWIG_POINTER_OWN |  0 ) :  0 ;
     resultobj = SWIG_Python_AppendOutput(resultobj, SWIG_NewPointerObj((void*)(arg2), SWIGTYPE_p_long, new_flags));
   }
   return resultobj;
 fail:
   return NULL;
@@ -13445,15 +13445,15 @@
   if (!SWIG_IsOK(res1)) {
     SWIG_exception_fail(SWIG_ArgError(res1), "in method '" "trexio_read_jastrow_een_num_64" "', argument " "1"" of type '" "trexio_t *const""'"); 
   }
   arg1 = (trexio_t *)(argp1);
   result = (trexio_exit_code)trexio_read_jastrow_een_num_64(arg1,arg2);
   resultobj = SWIG_From_int((int)(result));
   if (SWIG_IsTmpObj(res2)) {
-    resultobj = SWIG_Python_AppendOutput(resultobj, SWIG_From_int((*arg2)));
+    resultobj = SWIG_Python_AppendOutput(resultobj, SWIG_From_long((*arg2)));
   } else {
     int new_flags = SWIG_IsNewObj(res2) ? (SWIG_POINTER_OWN |  0 ) :  0 ;
     resultobj = SWIG_Python_AppendOutput(resultobj, SWIG_NewPointerObj((void*)(arg2), SWIGTYPE_p_long, new_flags));
   }
   return resultobj;
 fail:
   return NULL;
@@ -13531,15 +13531,15 @@
   if (!SWIG_IsOK(res1)) {
     SWIG_exception_fail(SWIG_ArgError(res1), "in method '" "trexio_read_jastrow_ee_scaling" "', argument " "1"" of type '" "trexio_t *const""'"); 
   }
   arg1 = (trexio_t *)(argp1);
   result = (trexio_exit_code)trexio_read_jastrow_ee_scaling(arg1,arg2);
   resultobj = SWIG_From_int((int)(result));
   if (SWIG_IsTmpObj(res2)) {
-    resultobj = SWIG_Python_AppendOutput(resultobj, SWIG_From_float((*arg2)));
+    resultobj = SWIG_Python_AppendOutput(resultobj, SWIG_From_double((*arg2)));
   } else {
     int new_flags = SWIG_IsNewObj(res2) ? (SWIG_POINTER_OWN |  0 ) :  0 ;
     resultobj = SWIG_Python_AppendOutput(resultobj, SWIG_NewPointerObj((void*)(arg2), SWIGTYPE_p_double, new_flags));
   }
   return resultobj;
 fail:
   return NULL;
@@ -13657,15 +13657,15 @@
   if (!SWIG_IsOK(res1)) {
     SWIG_exception_fail(SWIG_ArgError(res1), "in method '" "trexio_read_jastrow_ee_scaling_64" "', argument " "1"" of type '" "trexio_t *const""'"); 
   }
   arg1 = (trexio_t *)(argp1);
   result = (trexio_exit_code)trexio_read_jastrow_ee_scaling_64(arg1,arg2);
   resultobj = SWIG_From_int((int)(result));
   if (SWIG_IsTmpObj(res2)) {
-    resultobj = SWIG_Python_AppendOutput(resultobj, SWIG_From_float((*arg2)));
+    resultobj = SWIG_Python_AppendOutput(resultobj, SWIG_From_double((*arg2)));
   } else {
     int new_flags = SWIG_IsNewObj(res2) ? (SWIG_POINTER_OWN |  0 ) :  0 ;
     resultobj = SWIG_Python_AppendOutput(resultobj, SWIG_NewPointerObj((void*)(arg2), SWIGTYPE_p_double, new_flags));
   }
   return resultobj;
 fail:
   return NULL;
@@ -13869,15 +13869,15 @@
   if (!SWIG_IsOK(res1)) {
     SWIG_exception_fail(SWIG_ArgError(res1), "in method '" "trexio_read_qmc_num_64" "', argument " "1"" of type '" "trexio_t *const""'"); 
   }
   arg1 = (trexio_t *)(argp1);
   result = (trexio_exit_code)trexio_read_qmc_num_64(arg1,arg2);
   resultobj = SWIG_From_int((int)(result));
   if (SWIG_IsTmpObj(res2)) {
-    resultobj = SWIG_Python_AppendOutput(resultobj, SWIG_From_int((*arg2)));
+    resultobj = SWIG_Python_AppendOutput(resultobj, SWIG_From_long((*arg2)));
   } else {
     int new_flags = SWIG_IsNewObj(res2) ? (SWIG_POINTER_OWN |  0 ) :  0 ;
     resultobj = SWIG_Python_AppendOutput(resultobj, SWIG_NewPointerObj((void*)(arg2), SWIGTYPE_p_long, new_flags));
   }
   return resultobj;
 fail:
   return NULL;
@@ -61964,15 +61964,15 @@
   SWIG_Python_SetConstant(d, "TREXIO_DELIM",SWIG_FromCharPtr("\n"));
   SWIG_Python_SetConstant(d, "TREXIO_ORBITAL_SHIFT",SWIG_From_int((int)(1)));
   SWIG_Python_SetConstant(d, "TREXIO_INT_SIZE",SWIG_From_int((int)(64)));
   SWIG_Python_SetConstant(d, "TREXIO_PACKAGE_VERSION",SWIG_FromCharPtr("2.3.1"));
   SWIG_Python_SetConstant(d, "TREXIO_VERSION_MAJOR",SWIG_From_int((int)(2)));
   SWIG_Python_SetConstant(d, "TREXIO_VERSION_MINOR",SWIG_From_int((int)(3)));
   SWIG_Python_SetConstant(d, "TREXIO_VERSION_PATCH",SWIG_From_int((int)(1)));
-  SWIG_Python_SetConstant(d, "TREXIO_GIT_HASH",SWIG_FromCharPtr("13567fceb89aaafff9e38952bd2bd486611243b8"));
+  SWIG_Python_SetConstant(d, "TREXIO_GIT_HASH",SWIG_FromCharPtr("0df3a70bbee200b60f735c7284884f8656c708a5"));
 #if PY_VERSION_HEX >= 0x03000000
   return m;
 #else
   return;
 #endif
 }
```

### Comparing `trexio-1.3.1/src/trexio.c` & `trexio-1.3.2/src/trexio.c`

 * *Files 0% similar despite different names*

```diff
@@ -24517,16 +24517,16 @@
 
   /* To be set by generator : number of unique dimensions
      (e.g. 1 for ERI in AO basis because only ao_num is present in the list of dimensions) */
 #define unique_rank 2
   int64_t unique_dims[2];
 
   // Below part is populated by the generator when unique_rank > 1
-  rc = trexio_read_determinant_num_64(file, &unique_dims[0]); if (rc != TREXIO_SUCCESS) return rc;
-  rc = trexio_read_csf_num_64(file, &unique_dims[1]); if (rc != TREXIO_SUCCESS) return rc;
+  rc = trexio_read_csf_num_64(file, &unique_dims[0]); if (rc != TREXIO_SUCCESS) return rc;
+  rc = trexio_read_determinant_num_64(file, &unique_dims[1]); if (rc != TREXIO_SUCCESS) return rc;
 
   /* Find the maximal value along all dimensions to define the compression technique in the back end */
   int64_t max_dim = unique_dims[0];
 #if (unique_rank != 1) 
   for (uint32_t i = 1; i < unique_rank; i++) {
     if (unique_dims[i] > max_dim) max_dim = unique_dims[i];
   }
@@ -25863,16 +25863,16 @@
 
   /* To be set by generator : number of unique dimensions
      (e.g. 1 for ERI in AO basis because only ao_num is present in the list of dimensions) */
 #define unique_rank 2
   int64_t unique_dims[2];
 
   // Below part is populated by the generator when unique_rank > 1
-  rc = trexio_read_rdm_2e_upup_cholesky_num_64(file, &unique_dims[0]); if (rc != TREXIO_SUCCESS) return rc;
-  rc = trexio_read_mo_num_64(file, &unique_dims[1]); if (rc != TREXIO_SUCCESS) return rc;
+  rc = trexio_read_mo_num_64(file, &unique_dims[0]); if (rc != TREXIO_SUCCESS) return rc;
+  rc = trexio_read_rdm_2e_upup_cholesky_num_64(file, &unique_dims[1]); if (rc != TREXIO_SUCCESS) return rc;
 
   /* Find the maximal value along all dimensions to define the compression technique in the back end */
   int64_t max_dim = unique_dims[0];
 #if (unique_rank != 1) 
   for (uint32_t i = 1; i < unique_rank; i++) {
     if (unique_dims[i] > max_dim) max_dim = unique_dims[i];
   }
@@ -47784,16 +47784,16 @@
 
   /* To be set by generator : number of unique dimensions
      (e.g. 1 for ERI in AO basis because only ao_num is present in the list of dimensions) */
 #define unique_rank 2
   int64_t unique_dims[2];
 
   // Below part is populated by the generator when unique_rank > 1
-  rc = trexio_read_determinant_num_64(file, &unique_dims[0]); if (rc != TREXIO_SUCCESS) return rc;
-  rc = trexio_read_csf_num_64(file, &unique_dims[1]); if (rc != TREXIO_SUCCESS) return rc;
+  rc = trexio_read_csf_num_64(file, &unique_dims[0]); if (rc != TREXIO_SUCCESS) return rc;
+  rc = trexio_read_determinant_num_64(file, &unique_dims[1]); if (rc != TREXIO_SUCCESS) return rc;
 
   /* Find the maximal value along all dimensions to define the compression technique in the back end */
   int64_t max_dim = unique_dims[0];
 #if (unique_rank != 1) 
   for (uint32_t i = 1; i < unique_rank; i++) {
     if (unique_dims[i] > max_dim) max_dim = unique_dims[i];
   }
@@ -49578,16 +49578,16 @@
 
   /* To be set by generator : number of unique dimensions
      (e.g. 1 for ERI in AO basis because only ao_num is present in the list of dimensions) */
 #define unique_rank 2
   int64_t unique_dims[2];
 
   // Below part is populated by the generator when unique_rank > 1
-  rc = trexio_read_rdm_2e_upup_cholesky_num_64(file, &unique_dims[0]); if (rc != TREXIO_SUCCESS) return rc;
-  rc = trexio_read_mo_num_64(file, &unique_dims[1]); if (rc != TREXIO_SUCCESS) return rc;
+  rc = trexio_read_mo_num_64(file, &unique_dims[0]); if (rc != TREXIO_SUCCESS) return rc;
+  rc = trexio_read_rdm_2e_upup_cholesky_num_64(file, &unique_dims[1]); if (rc != TREXIO_SUCCESS) return rc;
 
   /* Find the maximal value along all dimensions to define the compression technique in the back end */
   int64_t max_dim = unique_dims[0];
 #if (unique_rank != 1) 
   for (uint32_t i = 1; i < unique_rank; i++) {
     if (unique_dims[i] > max_dim) max_dim = unique_dims[i];
   }
```

### Comparing `trexio-1.3.1/src/trexio.h` & `trexio-1.3.2/src/trexio.h`

 * *Files 0% similar despite different names*

```diff
@@ -106,15 +106,15 @@
 trexio_exit_code trexio_safe_to_orbital_list_up_dn (const int32_t N_int, const bitfield_t* dset_in, const int64_t dim_in, int32_t* const dset_up_out, const int64_t dim_up_out, int32_t* const dset_dn_out, const int64_t dim_dn_out, int32_t* const num_up, int32_t* const num_dn);
 trexio_exit_code trexio_to_bitfield_list (const int32_t* orb_list, const int32_t occupied_num, bitfield_t* const bit_list, const int32_t N_int);
 
 #define TREXIO_PACKAGE_VERSION "2.3.1"
 #define TREXIO_VERSION_MAJOR 2
 #define TREXIO_VERSION_MINOR 3
 #define TREXIO_VERSION_PATCH 1
-#define TREXIO_GIT_HASH "13567fceb89aaafff9e38952bd2bd486611243b8"
+#define TREXIO_GIT_HASH "0df3a70bbee200b60f735c7284884f8656c708a5"
 
 trexio_exit_code trexio_delete_metadata(trexio_t* const file);
 
 trexio_exit_code trexio_delete_nucleus(trexio_t* const file);
 
 trexio_exit_code trexio_delete_cell(trexio_t* const file);
```

### Comparing `trexio-1.3.1/src/trexio_hdf5.c` & `trexio-1.3.2/src/trexio_hdf5.c`

 * *Files identical despite different names*

### Comparing `trexio-1.3.1/src/trexio_hdf5.h` & `trexio-1.3.2/src/trexio_hdf5.h`

 * *Files identical despite different names*

### Comparing `trexio-1.3.1/src/trexio_private.h` & `trexio-1.3.2/src/trexio_private.h`

 * *Files identical despite different names*

### Comparing `trexio-1.3.1/src/trexio_s.h` & `trexio-1.3.2/src/trexio_s.h`

 * *Files identical despite different names*

### Comparing `trexio-1.3.1/src/trexio_text.c` & `trexio-1.3.2/src/trexio_text.c`

 * *Files identical despite different names*

### Comparing `trexio-1.3.1/src/trexio_text.h` & `trexio-1.3.2/src/trexio_text.h`

 * *Files identical despite different names*

### Comparing `trexio-1.3.1/test/benzene_data.py` & `trexio-1.3.2/test/benzene_data.py`

 * *Files identical despite different names*

### Comparing `trexio-1.3.1/test/test_api.py` & `trexio-1.3.2/test/test_api.py`

 * *Files identical despite different names*

### Comparing `trexio-1.3.1/test/test_pytrexio.py` & `trexio-1.3.2/test/test_pytrexio.py`

 * *Files identical despite different names*

### Comparing `trexio-1.3.1/trexio.egg-info/PKG-INFO` & `trexio-1.3.2/trexio.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: trexio
-Version: 1.3.1
+Version: 1.3.2
 Summary: Python API of the TREXIO library
 Home-page: https://github.com/TREX-CoE/trexio
 Author: TREX-CoE
 Author-email: posenitskiy@irsamc.ups-tlse.fr
 License: BSD
 Project-URL: Bug Tracker, https://github.com/TREX-CoE/trexio/issues
 Classifier: Intended Audience :: Science/Research
```

### Comparing `trexio-1.3.1/trexio.egg-info/SOURCES.txt` & `trexio-1.3.2/trexio.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `trexio-1.3.1/trexio.py` & `trexio-1.3.2/trexio.py`

 * *Files identical despite different names*

