# Comparing `tmp/lariat_python_sdk-0.1.2.tar.gz` & `tmp/lariat_python_sdk-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lariat_python_sdk-0.1.2.tar", last modified: Fri May  5 03:23:15 2023, max compression
+gzip compressed data, was "lariat_python_sdk-0.1.3.tar", last modified: Fri May  5 04:25:20 2023, max compression
```

## Comparing `lariat_python_sdk-0.1.2.tar` & `lariat_python_sdk-0.1.3.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 vikas      (501) staff       (20)        0 2023-05-05 03:23:15.554549 lariat_python_sdk-0.1.2/
--rw-r--r--   0 vikas      (501) staff       (20)     1498 2023-04-25 19:17:29.000000 lariat_python_sdk-0.1.2/LICENSE
--rw-r--r--   0 vikas      (501) staff       (20)     2327 2023-05-05 03:23:15.554376 lariat_python_sdk-0.1.2/PKG-INFO
--rw-r--r--   0 vikas      (501) staff       (20)     1427 2023-05-04 03:31:42.000000 lariat_python_sdk-0.1.2/README.md
-drwxr-xr-x   0 vikas      (501) staff       (20)        0 2023-05-05 03:23:15.551867 lariat_python_sdk-0.1.2/lariat_client/
--rw-r--r--   0 vikas      (501) staff       (20)      332 2023-04-25 19:25:48.000000 lariat_python_sdk-0.1.2/lariat_client/__init__.py
--rw-r--r--   0 vikas      (501) staff       (20)    19981 2023-05-04 11:38:36.000000 lariat_python_sdk-0.1.2/lariat_client/lariat_client.py
-drwxr-xr-x   0 vikas      (501) staff       (20)        0 2023-05-05 03:23:15.552942 lariat_python_sdk-0.1.2/lariat_python_sdk.egg-info/
--rw-r--r--   0 vikas      (501) staff       (20)     2327 2023-05-05 03:23:15.000000 lariat_python_sdk-0.1.2/lariat_python_sdk.egg-info/PKG-INFO
--rw-r--r--   0 vikas      (501) staff       (20)      321 2023-05-05 03:23:15.000000 lariat_python_sdk-0.1.2/lariat_python_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 vikas      (501) staff       (20)        1 2023-05-05 03:23:15.000000 lariat_python_sdk-0.1.2/lariat_python_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 vikas      (501) staff       (20)       43 2023-05-05 03:23:15.000000 lariat_python_sdk-0.1.2/lariat_python_sdk.egg-info/requires.txt
--rw-r--r--   0 vikas      (501) staff       (20)       14 2023-05-05 03:23:15.000000 lariat_python_sdk-0.1.2/lariat_python_sdk.egg-info/top_level.txt
--rw-r--r--   0 vikas      (501) staff       (20)     1032 2023-05-05 03:22:31.000000 lariat_python_sdk-0.1.2/pyproject.toml
--rw-r--r--   0 vikas      (501) staff       (20)       38 2023-05-05 03:23:15.554600 lariat_python_sdk-0.1.2/setup.cfg
-drwxr-xr-x   0 vikas      (501) staff       (20)        0 2023-05-05 03:23:15.553087 lariat_python_sdk-0.1.2/tests/
--rw-r--r--   0 vikas      (501) staff       (20)     6746 2023-04-25 19:32:13.000000 lariat_python_sdk-0.1.2/tests/test_lariat_client.py
+drwxr-xr-x   0 vikas      (501) staff       (20)        0 2023-05-05 04:25:20.558365 lariat_python_sdk-0.1.3/
+-rw-r--r--   0 vikas      (501) staff       (20)     1498 2023-05-05 03:34:47.000000 lariat_python_sdk-0.1.3/LICENSE
+-rw-r--r--   0 vikas      (501) staff       (20)     2407 2023-05-05 04:25:20.558208 lariat_python_sdk-0.1.3/PKG-INFO
+-rw-r--r--   0 vikas      (501) staff       (20)     1427 2023-05-05 03:34:47.000000 lariat_python_sdk-0.1.3/README.md
+drwxr-xr-x   0 vikas      (501) staff       (20)        0 2023-05-05 04:25:20.556843 lariat_python_sdk-0.1.3/lariat_client/
+-rw-r--r--   0 vikas      (501) staff       (20)      332 2023-05-05 03:34:47.000000 lariat_python_sdk-0.1.3/lariat_client/__init__.py
+-rw-r--r--   0 vikas      (501) staff       (20)    19981 2023-05-05 03:34:47.000000 lariat_python_sdk-0.1.3/lariat_client/lariat_client.py
+drwxr-xr-x   0 vikas      (501) staff       (20)        0 2023-05-05 04:25:20.557809 lariat_python_sdk-0.1.3/lariat_python_sdk.egg-info/
+-rw-r--r--   0 vikas      (501) staff       (20)     2407 2023-05-05 04:25:20.000000 lariat_python_sdk-0.1.3/lariat_python_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 vikas      (501) staff       (20)      321 2023-05-05 04:25:20.000000 lariat_python_sdk-0.1.3/lariat_python_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 vikas      (501) staff       (20)        1 2023-05-05 04:25:20.000000 lariat_python_sdk-0.1.3/lariat_python_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 vikas      (501) staff       (20)       43 2023-05-05 04:25:20.000000 lariat_python_sdk-0.1.3/lariat_python_sdk.egg-info/requires.txt
+-rw-r--r--   0 vikas      (501) staff       (20)       14 2023-05-05 04:25:20.000000 lariat_python_sdk-0.1.3/lariat_python_sdk.egg-info/top_level.txt
+-rw-r--r--   0 vikas      (501) staff       (20)     1102 2023-05-05 04:25:11.000000 lariat_python_sdk-0.1.3/pyproject.toml
+-rw-r--r--   0 vikas      (501) staff       (20)       38 2023-05-05 04:25:20.558411 lariat_python_sdk-0.1.3/setup.cfg
+drwxr-xr-x   0 vikas      (501) staff       (20)        0 2023-05-05 04:25:20.557965 lariat_python_sdk-0.1.3/tests/
+-rw-r--r--   0 vikas      (501) staff       (20)     6746 2023-05-05 03:34:47.000000 lariat_python_sdk-0.1.3/tests/test_lariat_client.py
```

### Comparing `lariat_python_sdk-0.1.2/LICENSE` & `lariat_python_sdk-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `lariat_python_sdk-0.1.2/PKG-INFO` & `lariat_python_sdk-0.1.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 Metadata-Version: 2.1
 Name: lariat_python_sdk
-Version: 0.1.2
+Version: 0.1.3
 Summary: A Python module to interact with Lariat API to access data quality metrics and diagnostics
 Author-email: Lariat Data Team <info@lariatdata.com>
 License: BSD-3-Clause
 Project-URL: homepage, https://www.lariatdata.com
+Project-URL: documentation, https://lariat-python-sdk.readthedocs.io/en/latest/
 Project-URL: repository, https://github.com/lariat-data/lariat-python-sdk
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
```

### Comparing `lariat_python_sdk-0.1.2/README.md` & `lariat_python_sdk-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `lariat_python_sdk-0.1.2/lariat_client/lariat_client.py` & `lariat_python_sdk-0.1.3/lariat_client/lariat_client.py`

 * *Files identical despite different names*

### Comparing `lariat_python_sdk-0.1.2/lariat_python_sdk.egg-info/PKG-INFO` & `lariat_python_sdk-0.1.3/lariat_python_sdk.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 Metadata-Version: 2.1
 Name: lariat-python-sdk
-Version: 0.1.2
+Version: 0.1.3
 Summary: A Python module to interact with Lariat API to access data quality metrics and diagnostics
 Author-email: Lariat Data Team <info@lariatdata.com>
 License: BSD-3-Clause
 Project-URL: homepage, https://www.lariatdata.com
+Project-URL: documentation, https://lariat-python-sdk.readthedocs.io/en/latest/
 Project-URL: repository, https://github.com/lariat-data/lariat-python-sdk
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
```

### Comparing `lariat_python_sdk-0.1.2/pyproject.toml` & `lariat_python_sdk-0.1.3/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ["setuptools"]
 build-backend = "setuptools.build_meta"
 
 
 [project]
 name = "lariat_python_sdk"
-version = "0.1.2"
+version = "0.1.3"
 description = "A Python module to interact with Lariat API to access data quality metrics and diagnostics"
 readme = "README.md"
 authors = [
     { name = "Lariat Data Team", email = "info@lariatdata.com"}
 ]
 license = {text = "BSD-3-Clause"}
 dependencies = [
@@ -29,9 +29,10 @@
     "Programming Language :: Python :: 3.7",
     "Programming Language :: Python :: 3.8",
     "Programming Language :: Python :: 3.9",
 ]
 
 [project.urls]
 homepage = 'https://www.lariatdata.com'
+documentation = 'https://lariat-python-sdk.readthedocs.io/en/latest/'
 repository = 'https://github.com/lariat-data/lariat-python-sdk'
```

### Comparing `lariat_python_sdk-0.1.2/tests/test_lariat_client.py` & `lariat_python_sdk-0.1.3/tests/test_lariat_client.py`

 * *Files identical despite different names*

