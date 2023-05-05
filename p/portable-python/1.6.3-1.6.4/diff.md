# Comparing `tmp/portable-python-1.6.3.tar.gz` & `tmp/portable-python-1.6.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "portable-python-1.6.3.tar", last modified: Tue Dec 20 01:56:31 2022, max compression
+gzip compressed data, was "portable-python-1.6.4.tar", last modified: Fri May  5 05:30:21 2023, max compression
```

## Comparing `portable-python-1.6.3.tar` & `portable-python-1.6.4.tar`

### file list

```diff
@@ -1,32 +1,43 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-20 01:56:31.842957 portable-python-1.6.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1781 2022-12-20 01:55:50.000000 portable-python-1.6.3/DEVELOP.md
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2022-12-20 01:55:50.000000 portable-python-1.6.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       74 2022-12-20 01:55:50.000000 portable-python-1.6.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     8694 2022-12-20 01:56:31.842957 portable-python-1.6.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7262 2022-12-20 01:55:50.000000 portable-python-1.6.3/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)      289 2022-12-20 01:55:50.000000 portable-python-1.6.3/SECURITY.md
--rw-r--r--   0 runner    (1001) docker     (123)       50 2022-12-20 01:55:50.000000 portable-python-1.6.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2022-12-20 01:56:31.842957 portable-python-1.6.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1556 2022-12-20 01:55:50.000000 portable-python-1.6.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-20 01:56:31.838957 portable-python-1.6.3/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-20 01:56:31.838957 portable-python-1.6.3/src/portable_python/
--rw-r--r--   0 runner    (1001) docker     (123)    26987 2022-12-20 01:55:50.000000 portable-python-1.6.3/src/portable_python/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      149 2022-12-20 01:55:50.000000 portable-python-1.6.3/src/portable_python/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7530 2022-12-20 01:55:50.000000 portable-python-1.6.3/src/portable_python/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)    12776 2022-12-20 01:55:50.000000 portable-python-1.6.3/src/portable_python/config.py
--rw-r--r--   0 runner    (1001) docker     (123)    13816 2022-12-20 01:55:50.000000 portable-python-1.6.3/src/portable_python/cpython.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-20 01:56:31.842957 portable-python-1.6.3/src/portable_python/external/
--rw-r--r--   0 runner    (1001) docker     (123)      725 2022-12-20 01:55:50.000000 portable-python-1.6.3/src/portable_python/external/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3632 2022-12-20 01:55:50.000000 portable-python-1.6.3/src/portable_python/external/_inspect.py
--rw-r--r--   0 runner    (1001) docker     (123)     3446 2022-12-20 01:55:50.000000 portable-python-1.6.3/src/portable_python/external/tkinter.py
--rw-r--r--   0 runner    (1001) docker     (123)    10004 2022-12-20 01:55:50.000000 portable-python-1.6.3/src/portable_python/external/xcpython.py
--rw-r--r--   0 runner    (1001) docker     (123)    21099 2022-12-20 01:55:50.000000 portable-python-1.6.3/src/portable_python/inspector.py
--rw-r--r--   0 runner    (1001) docker     (123)     1981 2022-12-20 01:55:50.000000 portable-python-1.6.3/src/portable_python/tracking.py
--rw-r--r--   0 runner    (1001) docker     (123)     6690 2022-12-20 01:55:50.000000 portable-python-1.6.3/src/portable_python/versions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2022-12-20 01:56:31.838957 portable-python-1.6.3/src/portable_python.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8694 2022-12-20 01:56:31.000000 portable-python-1.6.3/src/portable_python.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      749 2022-12-20 01:56:31.000000 portable-python-1.6.3/src/portable_python.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2022-12-20 01:56:31.000000 portable-python-1.6.3/src/portable_python.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       66 2022-12-20 01:56:31.000000 portable-python-1.6.3/src/portable_python.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       44 2022-12-20 01:56:31.000000 portable-python-1.6.3/src/portable_python.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2022-12-20 01:56:31.000000 portable-python-1.6.3/src/portable_python.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 05:30:21.728153 portable-python-1.6.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1781 2023-05-05 05:29:35.000000 portable-python-1.6.4/DEVELOP.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-05-05 05:29:35.000000 portable-python-1.6.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-05-05 05:29:35.000000 portable-python-1.6.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     8694 2023-05-05 05:30:21.728153 portable-python-1.6.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7262 2023-05-05 05:29:35.000000 portable-python-1.6.4/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      289 2023-05-05 05:29:35.000000 portable-python-1.6.4/SECURITY.md
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-05-05 05:29:35.000000 portable-python-1.6.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-05 05:30:21.728153 portable-python-1.6.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1556 2023-05-05 05:29:35.000000 portable-python-1.6.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 05:30:21.720152 portable-python-1.6.4/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 05:30:21.724153 portable-python-1.6.4/src/portable_python/
+-rw-r--r--   0 runner    (1001) docker     (123)    26987 2023-05-05 05:29:35.000000 portable-python-1.6.4/src/portable_python/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      149 2023-05-05 05:29:35.000000 portable-python-1.6.4/src/portable_python/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7530 2023-05-05 05:29:35.000000 portable-python-1.6.4/src/portable_python/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12776 2023-05-05 05:29:35.000000 portable-python-1.6.4/src/portable_python/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13816 2023-05-05 05:29:35.000000 portable-python-1.6.4/src/portable_python/cpython.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 05:30:21.724153 portable-python-1.6.4/src/portable_python/external/
+-rw-r--r--   0 runner    (1001) docker     (123)      725 2023-05-05 05:29:35.000000 portable-python-1.6.4/src/portable_python/external/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3632 2023-05-05 05:29:35.000000 portable-python-1.6.4/src/portable_python/external/_inspect.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3446 2023-05-05 05:29:35.000000 portable-python-1.6.4/src/portable_python/external/tkinter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10004 2023-05-05 05:29:35.000000 portable-python-1.6.4/src/portable_python/external/xcpython.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21099 2023-05-05 05:29:35.000000 portable-python-1.6.4/src/portable_python/inspector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1981 2023-05-05 05:29:35.000000 portable-python-1.6.4/src/portable_python/tracking.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6690 2023-05-05 05:29:35.000000 portable-python-1.6.4/src/portable_python/versions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 05:30:21.724153 portable-python-1.6.4/src/portable_python.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8694 2023-05-05 05:30:21.000000 portable-python-1.6.4/src/portable_python.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      964 2023-05-05 05:30:21.000000 portable-python-1.6.4/src/portable_python.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 05:30:21.000000 portable-python-1.6.4/src/portable_python.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-05-05 05:30:21.000000 portable-python-1.6.4/src/portable_python.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-05-05 05:30:21.000000 portable-python-1.6.4/src/portable_python.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-05 05:30:21.000000 portable-python-1.6.4/src/portable_python.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 05:30:21.728153 portable-python-1.6.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     3994 2023-05-05 05:29:35.000000 portable-python-1.6.4/tests/test_build.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3289 2023-05-05 05:29:35.000000 portable-python-1.6.4/tests/test_cleanup.py
+-rw-r--r--   0 runner    (1001) docker     (123)      686 2023-05-05 05:29:35.000000 portable-python-1.6.4/tests/test_failed.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8245 2023-05-05 05:29:35.000000 portable-python-1.6.4/tests/test_inspector.py
+-rw-r--r--   0 runner    (1001) docker     (123)      625 2023-05-05 05:29:35.000000 portable-python-1.6.4/tests/test_invoker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1555 2023-05-05 05:29:35.000000 portable-python-1.6.4/tests/test_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)      711 2023-05-05 05:29:35.000000 portable-python-1.6.4/tests/test_prefix.py
+-rw-r--r--   0 runner    (1001) docker     (123)      763 2023-05-05 05:29:35.000000 portable-python-1.6.4/tests/test_recompress.py
+-rw-r--r--   0 runner    (1001) docker     (123)      408 2023-05-05 05:29:35.000000 portable-python-1.6.4/tests/test_report.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2701 2023-05-05 05:29:35.000000 portable-python-1.6.4/tests/test_setup.py
```

### Comparing `portable-python-1.6.3/DEVELOP.md` & `portable-python-1.6.4/DEVELOP.md`

 * *Files identical despite different names*

### Comparing `portable-python-1.6.3/LICENSE` & `portable-python-1.6.4/LICENSE`

 * *Files identical despite different names*

### Comparing `portable-python-1.6.3/PKG-INFO` & `portable-python-1.6.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: portable-python
-Version: 1.6.3
+Version: 1.6.4
 Summary: Portable python binaries
 Home-page: https://github.com/codrsquad/portable-python
 Author: Zoran Simic
 Author-email: zoran@simicweb.com
 License: MIT
 Project-URL: Documentation, https://github.com/codrsquad/portable-python/wiki
 Project-URL: Release notes, https://github.com/codrsquad/portable-python/wiki/Release-notes
```

### Comparing `portable-python-1.6.3/README.rst` & `portable-python-1.6.4/README.rst`

 * *Files identical despite different names*

### Comparing `portable-python-1.6.3/setup.py` & `portable-python-1.6.4/setup.py`

 * *Files identical despite different names*

### Comparing `portable-python-1.6.3/src/portable_python/__init__.py` & `portable-python-1.6.4/src/portable_python/__init__.py`

 * *Files identical despite different names*

### Comparing `portable-python-1.6.3/src/portable_python/cli.py` & `portable-python-1.6.4/src/portable_python/cli.py`

 * *Files identical despite different names*

### Comparing `portable-python-1.6.3/src/portable_python/config.py` & `portable-python-1.6.4/src/portable_python/config.py`

 * *Files identical despite different names*

### Comparing `portable-python-1.6.3/src/portable_python/cpython.py` & `portable-python-1.6.4/src/portable_python/cpython.py`

 * *Files identical despite different names*

### Comparing `portable-python-1.6.3/src/portable_python/external/__init__.py` & `portable-python-1.6.4/src/portable_python/external/__init__.py`

 * *Files identical despite different names*

### Comparing `portable-python-1.6.3/src/portable_python/external/_inspect.py` & `portable-python-1.6.4/src/portable_python/external/_inspect.py`

 * *Files identical despite different names*

### Comparing `portable-python-1.6.3/src/portable_python/external/tkinter.py` & `portable-python-1.6.4/src/portable_python/external/tkinter.py`

 * *Files identical despite different names*

### Comparing `portable-python-1.6.3/src/portable_python/external/xcpython.py` & `portable-python-1.6.4/src/portable_python/external/xcpython.py`

 * *Files 1% similar despite different names*

```diff
@@ -141,15 +141,15 @@
 
     @property
     def url(self):
         return f"https://www.openssl.org/source/openssl-{self.version}.tar.gz"
 
     @property
     def version(self):
-        return self.cfg_version("1.1.1s")
+        return self.cfg_version("1.1.1t")
 
     def c_configure_args(self):
         yield "--openssldir=/etc/ssl"
         yield "no-shared", "no-idea", "no-tests"
 
     def _do_linux_compile(self):
         self.run_configure("./config", "-v", self.c_configure_args())
@@ -253,15 +253,15 @@
 
     @property
     def url(self):
         return f"https://github.com/sqlite/sqlite/archive/refs/tags/version-{self.version}.tar.gz"
 
     @property
     def version(self):
-        return self.cfg_version("3.39.4")
+        return self.cfg_version("3.41.2")
 
     def _do_linux_compile(self):
         self.run_configure(
             "./configure", "--enable-shared=no", "--enable-static=yes", "--disable-tcl", "--disable-readline", "--with-pic=yes"
         )
         self.run_make()
         self.run_make("install")
```

### Comparing `portable-python-1.6.3/src/portable_python/inspector.py` & `portable-python-1.6.4/src/portable_python/inspector.py`

 * *Files identical despite different names*

### Comparing `portable-python-1.6.3/src/portable_python/tracking.py` & `portable-python-1.6.4/src/portable_python/tracking.py`

 * *Files identical despite different names*

### Comparing `portable-python-1.6.3/src/portable_python/versions.py` & `portable-python-1.6.4/src/portable_python/versions.py`

 * *Files identical despite different names*

### Comparing `portable-python-1.6.3/src/portable_python.egg-info/PKG-INFO` & `portable-python-1.6.4/src/portable_python.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: portable-python
-Version: 1.6.3
+Version: 1.6.4
 Summary: Portable python binaries
 Home-page: https://github.com/codrsquad/portable-python
 Author: Zoran Simic
 Author-email: zoran@simicweb.com
 License: MIT
 Project-URL: Documentation, https://github.com/codrsquad/portable-python/wiki
 Project-URL: Release notes, https://github.com/codrsquad/portable-python/wiki/Release-notes
```

