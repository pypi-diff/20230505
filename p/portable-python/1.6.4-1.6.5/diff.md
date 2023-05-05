# Comparing `tmp/portable-python-1.6.4.tar.gz` & `tmp/portable-python-1.6.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "portable-python-1.6.4.tar", last modified: Fri May  5 05:30:21 2023, max compression
+gzip compressed data, was "portable-python-1.6.5.tar", last modified: Fri May  5 19:48:31 2023, max compression
```

## Comparing `portable-python-1.6.4.tar` & `portable-python-1.6.5.tar`

### file list

```diff
@@ -1,43 +1,43 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 05:30:21.728153 portable-python-1.6.4/
--rw-r--r--   0 runner    (1001) docker     (123)     1781 2023-05-05 05:29:35.000000 portable-python-1.6.4/DEVELOP.md
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-05-05 05:29:35.000000 portable-python-1.6.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-05-05 05:29:35.000000 portable-python-1.6.4/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     8694 2023-05-05 05:30:21.728153 portable-python-1.6.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7262 2023-05-05 05:29:35.000000 portable-python-1.6.4/README.rst
--rw-r--r--   0 runner    (1001) docker     (123)      289 2023-05-05 05:29:35.000000 portable-python-1.6.4/SECURITY.md
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-05-05 05:29:35.000000 portable-python-1.6.4/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-05 05:30:21.728153 portable-python-1.6.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1556 2023-05-05 05:29:35.000000 portable-python-1.6.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 05:30:21.720152 portable-python-1.6.4/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 05:30:21.724153 portable-python-1.6.4/src/portable_python/
--rw-r--r--   0 runner    (1001) docker     (123)    26987 2023-05-05 05:29:35.000000 portable-python-1.6.4/src/portable_python/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      149 2023-05-05 05:29:35.000000 portable-python-1.6.4/src/portable_python/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7530 2023-05-05 05:29:35.000000 portable-python-1.6.4/src/portable_python/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)    12776 2023-05-05 05:29:35.000000 portable-python-1.6.4/src/portable_python/config.py
--rw-r--r--   0 runner    (1001) docker     (123)    13816 2023-05-05 05:29:35.000000 portable-python-1.6.4/src/portable_python/cpython.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 05:30:21.724153 portable-python-1.6.4/src/portable_python/external/
--rw-r--r--   0 runner    (1001) docker     (123)      725 2023-05-05 05:29:35.000000 portable-python-1.6.4/src/portable_python/external/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3632 2023-05-05 05:29:35.000000 portable-python-1.6.4/src/portable_python/external/_inspect.py
--rw-r--r--   0 runner    (1001) docker     (123)     3446 2023-05-05 05:29:35.000000 portable-python-1.6.4/src/portable_python/external/tkinter.py
--rw-r--r--   0 runner    (1001) docker     (123)    10004 2023-05-05 05:29:35.000000 portable-python-1.6.4/src/portable_python/external/xcpython.py
--rw-r--r--   0 runner    (1001) docker     (123)    21099 2023-05-05 05:29:35.000000 portable-python-1.6.4/src/portable_python/inspector.py
--rw-r--r--   0 runner    (1001) docker     (123)     1981 2023-05-05 05:29:35.000000 portable-python-1.6.4/src/portable_python/tracking.py
--rw-r--r--   0 runner    (1001) docker     (123)     6690 2023-05-05 05:29:35.000000 portable-python-1.6.4/src/portable_python/versions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 05:30:21.724153 portable-python-1.6.4/src/portable_python.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8694 2023-05-05 05:30:21.000000 portable-python-1.6.4/src/portable_python.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      964 2023-05-05 05:30:21.000000 portable-python-1.6.4/src/portable_python.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 05:30:21.000000 portable-python-1.6.4/src/portable_python.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-05-05 05:30:21.000000 portable-python-1.6.4/src/portable_python.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-05-05 05:30:21.000000 portable-python-1.6.4/src/portable_python.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-05 05:30:21.000000 portable-python-1.6.4/src/portable_python.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 05:30:21.728153 portable-python-1.6.4/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     3994 2023-05-05 05:29:35.000000 portable-python-1.6.4/tests/test_build.py
--rw-r--r--   0 runner    (1001) docker     (123)     3289 2023-05-05 05:29:35.000000 portable-python-1.6.4/tests/test_cleanup.py
--rw-r--r--   0 runner    (1001) docker     (123)      686 2023-05-05 05:29:35.000000 portable-python-1.6.4/tests/test_failed.py
--rw-r--r--   0 runner    (1001) docker     (123)     8245 2023-05-05 05:29:35.000000 portable-python-1.6.4/tests/test_inspector.py
--rw-r--r--   0 runner    (1001) docker     (123)      625 2023-05-05 05:29:35.000000 portable-python-1.6.4/tests/test_invoker.py
--rw-r--r--   0 runner    (1001) docker     (123)     1555 2023-05-05 05:29:35.000000 portable-python-1.6.4/tests/test_list.py
--rw-r--r--   0 runner    (1001) docker     (123)      711 2023-05-05 05:29:35.000000 portable-python-1.6.4/tests/test_prefix.py
--rw-r--r--   0 runner    (1001) docker     (123)      763 2023-05-05 05:29:35.000000 portable-python-1.6.4/tests/test_recompress.py
--rw-r--r--   0 runner    (1001) docker     (123)      408 2023-05-05 05:29:35.000000 portable-python-1.6.4/tests/test_report.py
--rw-r--r--   0 runner    (1001) docker     (123)     2701 2023-05-05 05:29:35.000000 portable-python-1.6.4/tests/test_setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 19:48:31.788893 portable-python-1.6.5/
+-rw-r--r--   0 runner    (1001) docker     (123)     1781 2023-05-05 19:47:50.000000 portable-python-1.6.5/DEVELOP.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-05-05 19:47:50.000000 portable-python-1.6.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-05-05 19:47:50.000000 portable-python-1.6.5/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     8694 2023-05-05 19:48:31.788893 portable-python-1.6.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7262 2023-05-05 19:47:50.000000 portable-python-1.6.5/README.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      289 2023-05-05 19:47:50.000000 portable-python-1.6.5/SECURITY.md
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-05-05 19:47:50.000000 portable-python-1.6.5/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-05 19:48:31.788893 portable-python-1.6.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1556 2023-05-05 19:47:50.000000 portable-python-1.6.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 19:48:31.780893 portable-python-1.6.5/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 19:48:31.784893 portable-python-1.6.5/src/portable_python/
+-rw-r--r--   0 runner    (1001) docker     (123)    26987 2023-05-05 19:47:50.000000 portable-python-1.6.5/src/portable_python/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      149 2023-05-05 19:47:50.000000 portable-python-1.6.5/src/portable_python/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7634 2023-05-05 19:47:50.000000 portable-python-1.6.5/src/portable_python/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12776 2023-05-05 19:47:50.000000 portable-python-1.6.5/src/portable_python/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13816 2023-05-05 19:47:50.000000 portable-python-1.6.5/src/portable_python/cpython.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 19:48:31.788893 portable-python-1.6.5/src/portable_python/external/
+-rw-r--r--   0 runner    (1001) docker     (123)      725 2023-05-05 19:47:50.000000 portable-python-1.6.5/src/portable_python/external/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3632 2023-05-05 19:47:50.000000 portable-python-1.6.5/src/portable_python/external/_inspect.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3446 2023-05-05 19:47:50.000000 portable-python-1.6.5/src/portable_python/external/tkinter.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10004 2023-05-05 19:47:50.000000 portable-python-1.6.5/src/portable_python/external/xcpython.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21099 2023-05-05 19:47:50.000000 portable-python-1.6.5/src/portable_python/inspector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1981 2023-05-05 19:47:50.000000 portable-python-1.6.5/src/portable_python/tracking.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6690 2023-05-05 19:47:50.000000 portable-python-1.6.5/src/portable_python/versions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 19:48:31.788893 portable-python-1.6.5/src/portable_python.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8694 2023-05-05 19:48:31.000000 portable-python-1.6.5/src/portable_python.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      964 2023-05-05 19:48:31.000000 portable-python-1.6.5/src/portable_python.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 19:48:31.000000 portable-python-1.6.5/src/portable_python.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-05-05 19:48:31.000000 portable-python-1.6.5/src/portable_python.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-05-05 19:48:31.000000 portable-python-1.6.5/src/portable_python.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-05-05 19:48:31.000000 portable-python-1.6.5/src/portable_python.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 19:48:31.788893 portable-python-1.6.5/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     3994 2023-05-05 19:47:50.000000 portable-python-1.6.5/tests/test_build.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3289 2023-05-05 19:47:50.000000 portable-python-1.6.5/tests/test_cleanup.py
+-rw-r--r--   0 runner    (1001) docker     (123)      686 2023-05-05 19:47:50.000000 portable-python-1.6.5/tests/test_failed.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8245 2023-05-05 19:47:50.000000 portable-python-1.6.5/tests/test_inspector.py
+-rw-r--r--   0 runner    (1001) docker     (123)      625 2023-05-05 19:47:50.000000 portable-python-1.6.5/tests/test_invoker.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1555 2023-05-05 19:47:50.000000 portable-python-1.6.5/tests/test_list.py
+-rw-r--r--   0 runner    (1001) docker     (123)      711 2023-05-05 19:47:50.000000 portable-python-1.6.5/tests/test_prefix.py
+-rw-r--r--   0 runner    (1001) docker     (123)      763 2023-05-05 19:47:50.000000 portable-python-1.6.5/tests/test_recompress.py
+-rw-r--r--   0 runner    (1001) docker     (123)      408 2023-05-05 19:47:50.000000 portable-python-1.6.5/tests/test_report.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2701 2023-05-05 19:47:50.000000 portable-python-1.6.5/tests/test_setup.py
```

### Comparing `portable-python-1.6.4/DEVELOP.md` & `portable-python-1.6.5/DEVELOP.md`

 * *Files identical despite different names*

### Comparing `portable-python-1.6.4/LICENSE` & `portable-python-1.6.5/LICENSE`

 * *Files identical despite different names*

### Comparing `portable-python-1.6.4/PKG-INFO` & `portable-python-1.6.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: portable-python
-Version: 1.6.4
+Version: 1.6.5
 Summary: Portable python binaries
 Home-page: https://github.com/codrsquad/portable-python
 Author: Zoran Simic
 Author-email: zoran@simicweb.com
 License: MIT
 Project-URL: Documentation, https://github.com/codrsquad/portable-python/wiki
 Project-URL: Release notes, https://github.com/codrsquad/portable-python/wiki/Release-notes
```

### Comparing `portable-python-1.6.4/README.rst` & `portable-python-1.6.5/README.rst`

 * *Files identical despite different names*

### Comparing `portable-python-1.6.4/setup.py` & `portable-python-1.6.5/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 setup(
     name="portable-python",
     setup_requires="setupmeta",
     versioning="dev",
     author="Zoran Simic zoran@simicweb.com",
     keywords="python, portable, binary",
     url="https://github.com/codrsquad/portable-python",
-    python_requires='>=3.6',
+    python_requires=">=3.6",
     entry_points={
         "console_scripts": [
             "portable-python = portable_python.__main__:main",
         ],
     },
     classifiers=[
         "Development Status :: 5 - Production/Stable",
```

### Comparing `portable-python-1.6.4/src/portable_python/__init__.py` & `portable-python-1.6.5/src/portable_python/__init__.py`

 * *Files identical despite different names*

### Comparing `portable-python-1.6.4/src/portable_python/cli.py` & `portable-python-1.6.5/src/portable_python/cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -71,25 +71,26 @@
         print(PrettyTable.two_column_diagnostics(_diagnostics(), depot.representation(), config))
 
 
 @main.command()
 @click.option("--modules", "-m", help="Modules to inspect")
 @click.option("--verbose", "-v", is_flag=True, help="Show full so report")
 @click.option("--prefix", "-p", is_flag=True, help="Build was done with --prefix (not portable)")
+@click.option("--skip-so", "-s", is_flag=True, help="Don't check all .so-s")
 @click.argument("path")
-def inspect(modules, verbose, prefix, path):
+def inspect(modules, verbose, prefix, skip_so, path):
     """Inspect a python installation for non-portable dynamic lib usage"""
     if path != "invoker":
         path = runez.resolved_path(path)
 
     inspector = PythonInspector(path, modules=modules)
     runez.abort_if(inspector.python.problem, "%s: %s" % (runez.red(path), inspector.python.problem))
     print(runez.blue(inspector.python))
     print(inspector.represented(verbose=verbose))
-    if not modules or modules == "all":
+    if not skip_so and (not modules or modules == "all"):
         problem = inspector.full_so_report.get_problem(portable=not prefix)
         runez.abort_if(problem)
 
 
 @main.command(name="list")
 @click.option("--json", is_flag=True, help="Json output")
 @click.argument("family", default="cpython")
```

### Comparing `portable-python-1.6.4/src/portable_python/config.py` & `portable-python-1.6.5/src/portable_python/config.py`

 * *Files identical despite different names*

### Comparing `portable-python-1.6.4/src/portable_python/cpython.py` & `portable-python-1.6.5/src/portable_python/cpython.py`

 * *Files identical despite different names*

### Comparing `portable-python-1.6.4/src/portable_python/external/__init__.py` & `portable-python-1.6.5/src/portable_python/external/__init__.py`

 * *Files identical despite different names*

### Comparing `portable-python-1.6.4/src/portable_python/external/_inspect.py` & `portable-python-1.6.5/src/portable_python/external/_inspect.py`

 * *Files identical despite different names*

### Comparing `portable-python-1.6.4/src/portable_python/external/tkinter.py` & `portable-python-1.6.5/src/portable_python/external/tkinter.py`

 * *Files identical despite different names*

### Comparing `portable-python-1.6.4/src/portable_python/external/xcpython.py` & `portable-python-1.6.5/src/portable_python/external/xcpython.py`

 * *Files identical despite different names*

### Comparing `portable-python-1.6.4/src/portable_python/inspector.py` & `portable-python-1.6.5/src/portable_python/inspector.py`

 * *Files identical despite different names*

### Comparing `portable-python-1.6.4/src/portable_python/tracking.py` & `portable-python-1.6.5/src/portable_python/tracking.py`

 * *Files identical despite different names*

### Comparing `portable-python-1.6.4/src/portable_python/versions.py` & `portable-python-1.6.5/src/portable_python/versions.py`

 * *Files identical despite different names*

### Comparing `portable-python-1.6.4/src/portable_python.egg-info/PKG-INFO` & `portable-python-1.6.5/src/portable_python.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: portable-python
-Version: 1.6.4
+Version: 1.6.5
 Summary: Portable python binaries
 Home-page: https://github.com/codrsquad/portable-python
 Author: Zoran Simic
 Author-email: zoran@simicweb.com
 License: MIT
 Project-URL: Documentation, https://github.com/codrsquad/portable-python/wiki
 Project-URL: Release notes, https://github.com/codrsquad/portable-python/wiki/Release-notes
```

### Comparing `portable-python-1.6.4/src/portable_python.egg-info/SOURCES.txt` & `portable-python-1.6.5/src/portable_python.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `portable-python-1.6.4/tests/test_build.py` & `portable-python-1.6.5/tests/test_build.py`

 * *Files identical despite different names*

### Comparing `portable-python-1.6.4/tests/test_cleanup.py` & `portable-python-1.6.5/tests/test_cleanup.py`

 * *Files identical despite different names*

### Comparing `portable-python-1.6.4/tests/test_failed.py` & `portable-python-1.6.5/tests/test_failed.py`

 * *Files identical despite different names*

### Comparing `portable-python-1.6.4/tests/test_inspector.py` & `portable-python-1.6.5/tests/test_inspector.py`

 * *Files identical despite different names*

### Comparing `portable-python-1.6.4/tests/test_invoker.py` & `portable-python-1.6.5/tests/test_invoker.py`

 * *Files identical despite different names*

### Comparing `portable-python-1.6.4/tests/test_list.py` & `portable-python-1.6.5/tests/test_list.py`

 * *Files identical despite different names*

### Comparing `portable-python-1.6.4/tests/test_prefix.py` & `portable-python-1.6.5/tests/test_prefix.py`

 * *Files identical despite different names*

### Comparing `portable-python-1.6.4/tests/test_recompress.py` & `portable-python-1.6.5/tests/test_recompress.py`

 * *Files identical despite different names*

### Comparing `portable-python-1.6.4/tests/test_setup.py` & `portable-python-1.6.5/tests/test_setup.py`

 * *Files identical despite different names*

