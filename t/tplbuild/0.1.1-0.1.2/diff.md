# Comparing `tmp/tplbuild-0.1.1.tar.gz` & `tmp/tplbuild-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tplbuild-0.1.1.tar", last modified: Sun Nov  6 07:28:02 2022, max compression
+gzip compressed data, was "tplbuild-0.1.2.tar", last modified: Fri May  5 02:29:25 2023, max compression
```

## Comparing `tplbuild-0.1.1.tar` & `tplbuild-0.1.2.tar`

### file list

```diff
@@ -1,49 +1,56 @@
-drwxrwxr-x   0 msg       (1000) msg       (1000)        0 2022-11-06 07:28:02.738947 tplbuild-0.1.1/
--rw-rw-r--   0 msg       (1000) msg       (1000)     1493 2022-01-02 20:30:49.000000 tplbuild-0.1.1/LICENSE
--rw-rw-r--   0 msg       (1000) msg       (1000)     1620 2022-11-06 07:28:02.738947 tplbuild-0.1.1/PKG-INFO
--rw-rw-r--   0 msg       (1000) msg       (1000)     1005 2022-10-19 05:38:05.000000 tplbuild-0.1.1/README.md
--rw-rw-r--   0 msg       (1000) msg       (1000)     1168 2022-08-15 01:35:07.000000 tplbuild-0.1.1/pyproject.toml
--rw-rw-r--   0 msg       (1000) msg       (1000)      935 2022-11-06 07:28:02.738947 tplbuild-0.1.1/setup.cfg
--rwxrwxr-x   0 msg       (1000) msg       (1000)       61 2022-03-19 20:59:54.000000 tplbuild-0.1.1/setup.py
-drwxrwxr-x   0 msg       (1000) msg       (1000)        0 2022-11-06 07:28:02.738947 tplbuild-0.1.1/tplbuild/
--rw-rw-r--   0 msg       (1000) msg       (1000)        0 2022-01-02 20:30:49.000000 tplbuild-0.1.1/tplbuild/__init__.py
--rwxrwxr-x   0 msg       (1000) msg       (1000)       57 2022-03-19 21:22:14.000000 tplbuild-0.1.1/tplbuild/__main__.py
--rw-rw-r--   0 msg       (1000) msg       (1000)       22 2022-11-06 07:24:40.000000 tplbuild-0.1.1/tplbuild/_version.py
--rw-rw-r--   0 msg       (1000) msg       (1000)     2207 2022-02-06 08:59:54.000000 tplbuild-0.1.1/tplbuild/arch.py
--rw-rw-r--   0 msg       (1000) msg       (1000)     1901 2022-05-23 06:47:33.000000 tplbuild-0.1.1/tplbuild/builtin_clients.yml
-drwxrwxr-x   0 msg       (1000) msg       (1000)        0 2022-11-06 07:28:02.738947 tplbuild-0.1.1/tplbuild/cmd/
--rw-rw-r--   0 msg       (1000) msg       (1000)        0 2022-01-17 03:22:17.000000 tplbuild-0.1.1/tplbuild/cmd/__init__.py
--rw-rw-r--   0 msg       (1000) msg       (1000)     3868 2022-08-17 08:01:29.000000 tplbuild-0.1.1/tplbuild/cmd/base_build.py
--rw-rw-r--   0 msg       (1000) msg       (1000)     1737 2022-07-11 03:57:00.000000 tplbuild-0.1.1/tplbuild/cmd/base_lookup.py
--rw-rw-r--   0 msg       (1000) msg       (1000)     4821 2022-07-11 03:55:19.000000 tplbuild-0.1.1/tplbuild/cmd/base_prune.py
--rw-rw-r--   0 msg       (1000) msg       (1000)     4092 2022-08-17 08:01:29.000000 tplbuild-0.1.1/tplbuild/cmd/build.py
--rw-rw-r--   0 msg       (1000) msg       (1000)      785 2022-08-17 09:31:38.000000 tplbuild-0.1.1/tplbuild/cmd/common.py
--rw-rw-r--   0 msg       (1000) msg       (1000)     9424 2022-10-24 00:59:10.000000 tplbuild-0.1.1/tplbuild/cmd/main.py
--rw-rw-r--   0 msg       (1000) msg       (1000)     5635 2022-08-17 08:01:29.000000 tplbuild-0.1.1/tplbuild/cmd/publish.py
--rw-rw-r--   0 msg       (1000) msg       (1000)     1664 2022-07-11 03:50:41.000000 tplbuild-0.1.1/tplbuild/cmd/source_lookup.py
--rw-rw-r--   0 msg       (1000) msg       (1000)     4428 2022-10-24 02:13:51.000000 tplbuild-0.1.1/tplbuild/cmd/source_update.py
--rw-rw-r--   0 msg       (1000) msg       (1000)      628 2022-07-15 04:02:38.000000 tplbuild-0.1.1/tplbuild/cmd/utility.py
--rw-rw-r--   0 msg       (1000) msg       (1000)      536 2022-10-24 01:19:28.000000 tplbuild-0.1.1/tplbuild/cmd/version.py
--rw-rw-r--   0 msg       (1000) msg       (1000)    18200 2022-10-24 02:22:30.000000 tplbuild-0.1.1/tplbuild/config.py
--rw-rw-r--   0 msg       (1000) msg       (1000)    14880 2022-07-16 18:21:12.000000 tplbuild-0.1.1/tplbuild/context.py
--rw-rw-r--   0 msg       (1000) msg       (1000)     1865 2022-08-15 06:45:34.000000 tplbuild-0.1.1/tplbuild/exceptions.py
--rw-rw-r--   0 msg       (1000) msg       (1000)    25961 2022-09-12 06:15:23.000000 tplbuild-0.1.1/tplbuild/executor.py
--rw-rw-r--   0 msg       (1000) msg       (1000)     2795 2022-09-12 05:48:57.000000 tplbuild-0.1.1/tplbuild/exit_context.py
--rw-rw-r--   0 msg       (1000) msg       (1000)     4359 2022-08-15 01:00:06.000000 tplbuild-0.1.1/tplbuild/graph.py
--rw-rw-r--   0 msg       (1000) msg       (1000)      864 2022-01-02 20:30:49.000000 tplbuild-0.1.1/tplbuild/hashing.py
--rw-rw-r--   0 msg       (1000) msg       (1000)     7526 2022-08-17 07:02:10.000000 tplbuild-0.1.1/tplbuild/images.py
--rw-rw-r--   0 msg       (1000) msg       (1000)     3479 2022-11-06 07:21:23.000000 tplbuild-0.1.1/tplbuild/jinja_source_mapper.py
--rw-rw-r--   0 msg       (1000) msg       (1000)     2682 2022-03-07 09:27:00.000000 tplbuild-0.1.1/tplbuild/output.py
--rw-rw-r--   0 msg       (1000) msg       (1000)     8119 2022-05-23 08:20:57.000000 tplbuild-0.1.1/tplbuild/plan.py
--rw-rw-r--   0 msg       (1000) msg       (1000)        0 2022-01-02 20:30:49.000000 tplbuild-0.1.1/tplbuild/py.typed
--rw-rw-r--   0 msg       (1000) msg       (1000)    11053 2022-08-26 04:03:41.000000 tplbuild-0.1.1/tplbuild/render.py
--rw-rw-r--   0 msg       (1000) msg       (1000)     3837 2022-07-16 18:21:11.000000 tplbuild-0.1.1/tplbuild/sync_to_async_pipe.py
--rw-rw-r--   0 msg       (1000) msg       (1000)    28989 2022-11-06 06:49:53.000000 tplbuild-0.1.1/tplbuild/tplbuild.py
--rw-rw-r--   0 msg       (1000) msg       (1000)     7873 2022-08-17 09:42:57.000000 tplbuild-0.1.1/tplbuild/utils.py
-drwxrwxr-x   0 msg       (1000) msg       (1000)        0 2022-11-06 07:28:02.738947 tplbuild-0.1.1/tplbuild.egg-info/
--rw-rw-r--   0 msg       (1000) msg       (1000)     1620 2022-11-06 07:28:02.000000 tplbuild-0.1.1/tplbuild.egg-info/PKG-INFO
--rw-rw-r--   0 msg       (1000) msg       (1000)      999 2022-11-06 07:28:02.000000 tplbuild-0.1.1/tplbuild.egg-info/SOURCES.txt
--rw-rw-r--   0 msg       (1000) msg       (1000)        1 2022-11-06 07:28:02.000000 tplbuild-0.1.1/tplbuild.egg-info/dependency_links.txt
--rw-rw-r--   0 msg       (1000) msg       (1000)       52 2022-11-06 07:28:02.000000 tplbuild-0.1.1/tplbuild.egg-info/entry_points.txt
--rw-rw-r--   0 msg       (1000) msg       (1000)       57 2022-11-06 07:28:02.000000 tplbuild-0.1.1/tplbuild.egg-info/requires.txt
--rw-rw-r--   0 msg       (1000) msg       (1000)        9 2022-11-06 07:28:02.000000 tplbuild-0.1.1/tplbuild.egg-info/top_level.txt
+drwxrwxr-x   0 msg       (1000) msg       (1000)        0 2023-05-05 02:29:25.623012 tplbuild-0.1.2/
+-rw-rw-r--   0 msg       (1000) msg       (1000)     1493 2022-01-02 20:30:49.000000 tplbuild-0.1.2/LICENSE
+-rw-rw-r--   0 msg       (1000) msg       (1000)     1745 2023-05-05 02:29:25.623012 tplbuild-0.1.2/PKG-INFO
+-rw-rw-r--   0 msg       (1000) msg       (1000)     1130 2022-11-06 07:35:08.000000 tplbuild-0.1.2/README.md
+-rw-rw-r--   0 msg       (1000) msg       (1000)     1265 2023-05-05 02:25:24.000000 tplbuild-0.1.2/pyproject.toml
+-rw-rw-r--   0 msg       (1000) msg       (1000)      935 2023-05-05 02:29:25.623012 tplbuild-0.1.2/setup.cfg
+-rwxrwxr-x   0 msg       (1000) msg       (1000)       61 2022-03-19 20:59:54.000000 tplbuild-0.1.2/setup.py
+drwxrwxr-x   0 msg       (1000) msg       (1000)        0 2023-05-05 02:29:25.619012 tplbuild-0.1.2/tests/
+-rw-rw-r--   0 msg       (1000) msg       (1000)     4109 2022-08-17 08:02:37.000000 tplbuild-0.1.2/tests/test_builds.py
+-rw-rw-r--   0 msg       (1000) msg       (1000)    10998 2022-05-10 03:15:44.000000 tplbuild-0.1.2/tests/test_context.py
+-rw-rw-r--   0 msg       (1000) msg       (1000)     4384 2022-04-17 03:55:49.000000 tplbuild-0.1.2/tests/test_exit_context.py
+-rw-rw-r--   0 msg       (1000) msg       (1000)     4947 2022-07-16 18:21:12.000000 tplbuild-0.1.2/tests/test_graph.py
+-rw-rw-r--   0 msg       (1000) msg       (1000)     1902 2022-07-16 18:21:11.000000 tplbuild-0.1.2/tests/test_sync_to_async_pipe.py
+-rw-rw-r--   0 msg       (1000) msg       (1000)     6203 2022-08-17 09:45:01.000000 tplbuild-0.1.2/tests/test_utils.py
+drwxrwxr-x   0 msg       (1000) msg       (1000)        0 2023-05-05 02:29:25.623012 tplbuild-0.1.2/tplbuild/
+-rw-rw-r--   0 msg       (1000) msg       (1000)        0 2022-01-02 20:30:49.000000 tplbuild-0.1.2/tplbuild/__init__.py
+-rwxrwxr-x   0 msg       (1000) msg       (1000)       57 2022-03-19 21:22:14.000000 tplbuild-0.1.2/tplbuild/__main__.py
+-rw-rw-r--   0 msg       (1000) msg       (1000)       22 2023-05-05 02:19:25.000000 tplbuild-0.1.2/tplbuild/_version.py
+-rw-rw-r--   0 msg       (1000) msg       (1000)     2207 2022-02-06 08:59:54.000000 tplbuild-0.1.2/tplbuild/arch.py
+-rw-rw-r--   0 msg       (1000) msg       (1000)     1901 2022-05-23 06:47:33.000000 tplbuild-0.1.2/tplbuild/builtin_clients.yml
+drwxrwxr-x   0 msg       (1000) msg       (1000)        0 2023-05-05 02:29:25.623012 tplbuild-0.1.2/tplbuild/cmd/
+-rw-rw-r--   0 msg       (1000) msg       (1000)        0 2022-01-17 03:22:17.000000 tplbuild-0.1.2/tplbuild/cmd/__init__.py
+-rw-rw-r--   0 msg       (1000) msg       (1000)     3905 2023-05-05 02:19:25.000000 tplbuild-0.1.2/tplbuild/cmd/base_build.py
+-rw-rw-r--   0 msg       (1000) msg       (1000)     1737 2022-07-11 03:57:00.000000 tplbuild-0.1.2/tplbuild/cmd/base_lookup.py
+-rw-rw-r--   0 msg       (1000) msg       (1000)     4821 2022-07-11 03:55:19.000000 tplbuild-0.1.2/tplbuild/cmd/base_prune.py
+-rw-rw-r--   0 msg       (1000) msg       (1000)     4092 2022-08-17 08:01:29.000000 tplbuild-0.1.2/tplbuild/cmd/build.py
+-rw-rw-r--   0 msg       (1000) msg       (1000)      785 2022-08-17 09:31:38.000000 tplbuild-0.1.2/tplbuild/cmd/common.py
+-rw-rw-r--   0 msg       (1000) msg       (1000)     9459 2023-05-05 02:19:25.000000 tplbuild-0.1.2/tplbuild/cmd/main.py
+-rw-rw-r--   0 msg       (1000) msg       (1000)     5635 2022-08-17 08:01:29.000000 tplbuild-0.1.2/tplbuild/cmd/publish.py
+-rw-rw-r--   0 msg       (1000) msg       (1000)     1664 2022-07-11 03:50:41.000000 tplbuild-0.1.2/tplbuild/cmd/source_lookup.py
+-rw-rw-r--   0 msg       (1000) msg       (1000)     4428 2022-10-24 02:13:51.000000 tplbuild-0.1.2/tplbuild/cmd/source_update.py
+-rw-rw-r--   0 msg       (1000) msg       (1000)      628 2022-07-15 04:02:38.000000 tplbuild-0.1.2/tplbuild/cmd/utility.py
+-rw-rw-r--   0 msg       (1000) msg       (1000)      536 2022-10-24 01:19:28.000000 tplbuild-0.1.2/tplbuild/cmd/version.py
+-rw-rw-r--   0 msg       (1000) msg       (1000)    18200 2022-10-24 02:22:30.000000 tplbuild-0.1.2/tplbuild/config.py
+-rw-rw-r--   0 msg       (1000) msg       (1000)    14890 2023-05-05 02:19:25.000000 tplbuild-0.1.2/tplbuild/context.py
+-rw-rw-r--   0 msg       (1000) msg       (1000)     1865 2022-08-15 06:45:34.000000 tplbuild-0.1.2/tplbuild/exceptions.py
+-rw-rw-r--   0 msg       (1000) msg       (1000)    25961 2022-09-12 06:15:23.000000 tplbuild-0.1.2/tplbuild/executor.py
+-rw-rw-r--   0 msg       (1000) msg       (1000)     2795 2022-09-12 05:48:57.000000 tplbuild-0.1.2/tplbuild/exit_context.py
+-rw-rw-r--   0 msg       (1000) msg       (1000)     4359 2022-08-15 01:00:06.000000 tplbuild-0.1.2/tplbuild/graph.py
+-rw-rw-r--   0 msg       (1000) msg       (1000)      864 2022-01-02 20:30:49.000000 tplbuild-0.1.2/tplbuild/hashing.py
+-rw-rw-r--   0 msg       (1000) msg       (1000)     7526 2022-08-17 07:02:10.000000 tplbuild-0.1.2/tplbuild/images.py
+-rw-rw-r--   0 msg       (1000) msg       (1000)     3479 2022-11-06 07:21:23.000000 tplbuild-0.1.2/tplbuild/jinja_source_mapper.py
+-rw-rw-r--   0 msg       (1000) msg       (1000)     2682 2022-03-07 09:27:00.000000 tplbuild-0.1.2/tplbuild/output.py
+-rw-rw-r--   0 msg       (1000) msg       (1000)     8119 2022-05-23 08:20:57.000000 tplbuild-0.1.2/tplbuild/plan.py
+-rw-rw-r--   0 msg       (1000) msg       (1000)        0 2022-01-02 20:30:49.000000 tplbuild-0.1.2/tplbuild/py.typed
+-rw-rw-r--   0 msg       (1000) msg       (1000)    11053 2022-08-26 04:03:41.000000 tplbuild-0.1.2/tplbuild/render.py
+-rw-rw-r--   0 msg       (1000) msg       (1000)     3837 2022-07-16 18:21:11.000000 tplbuild-0.1.2/tplbuild/sync_to_async_pipe.py
+-rw-rw-r--   0 msg       (1000) msg       (1000)    28989 2022-11-06 06:49:53.000000 tplbuild-0.1.2/tplbuild/tplbuild.py
+-rw-rw-r--   0 msg       (1000) msg       (1000)     7873 2022-08-17 09:42:57.000000 tplbuild-0.1.2/tplbuild/utils.py
+drwxrwxr-x   0 msg       (1000) msg       (1000)        0 2023-05-05 02:29:25.623012 tplbuild-0.1.2/tplbuild.egg-info/
+-rw-rw-r--   0 msg       (1000) msg       (1000)     1745 2023-05-05 02:29:25.000000 tplbuild-0.1.2/tplbuild.egg-info/PKG-INFO
+-rw-rw-r--   0 msg       (1000) msg       (1000)     1142 2023-05-05 02:29:25.000000 tplbuild-0.1.2/tplbuild.egg-info/SOURCES.txt
+-rw-rw-r--   0 msg       (1000) msg       (1000)        1 2023-05-05 02:29:25.000000 tplbuild-0.1.2/tplbuild.egg-info/dependency_links.txt
+-rw-rw-r--   0 msg       (1000) msg       (1000)       52 2023-05-05 02:29:25.000000 tplbuild-0.1.2/tplbuild.egg-info/entry_points.txt
+-rw-rw-r--   0 msg       (1000) msg       (1000)       57 2023-05-05 02:29:25.000000 tplbuild-0.1.2/tplbuild.egg-info/requires.txt
+-rw-rw-r--   0 msg       (1000) msg       (1000)        9 2023-05-05 02:29:25.000000 tplbuild-0.1.2/tplbuild.egg-info/top_level.txt
```

### Comparing `tplbuild-0.1.1/LICENSE` & `tplbuild-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `tplbuild-0.1.1/PKG-INFO` & `tplbuild-0.1.2/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tplbuild
-Version: 0.1.1
+Version: 0.1.2
 Summary: Templated container build tool
 Home-page: http://github.com/msg555/tplbuild/
 Author: Mark Gordon
 Author-email: msg555@gmail.com
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
@@ -39,14 +39,19 @@
 
 
 ## Documentation
 
 Documentation for *tplbuild* can be found
 [here](https://tplbuild.readthedocs.io/)
 
+### Examples
+
+Check out the [examples](examples/) folder in this repo for some example of
+what can be done with `tplbuild`.
+
 ### Demo Video
 
 Additionally, you can find a quick tutorial highlighting key features
 [here](https://youtu.be/HDiyABr8Adw)
 
 [![Tplbuild Demo
 Video](https://img.youtube.com/vi/HDiyABr8Adw/0.jpg)](https://www.youtube.com/watch?v=HDiyABr8Adw "Tplbuild Demo")
```

### Comparing `tplbuild-0.1.1/README.md` & `tplbuild-0.1.2/README.md`

 * *Files 8% similar despite different names*

```diff
@@ -21,14 +21,19 @@
 
 
 ## Documentation
 
 Documentation for *tplbuild* can be found
 [here](https://tplbuild.readthedocs.io/)
 
+### Examples
+
+Check out the [examples](examples/) folder in this repo for some example of
+what can be done with `tplbuild`.
+
 ### Demo Video
 
 Additionally, you can find a quick tutorial highlighting key features
 [here](https://youtu.be/HDiyABr8Adw)
 
 [![Tplbuild Demo
 Video](https://img.youtube.com/vi/HDiyABr8Adw/0.jpg)](https://www.youtube.com/watch?v=HDiyABr8Adw "Tplbuild Demo")
```

### Comparing `tplbuild-0.1.1/pyproject.toml` & `tplbuild-0.1.2/pyproject.toml`

 * *Files 4% similar despite different names*

```diff
@@ -27,18 +27,22 @@
     "too-many-locals",
     "too-many-statements",
     "too-many-nested-blocks",
     "too-many-return-statements",
     "too-many-instance-attributes",
     "too-many-arguments",
     "consider-using-assignment-expr",
+    "use-dict-literal",
     # handled by black
     "format",
     "missing-module-docstring",
     "fixme",
+
+    "deprecated-typing-alias",
+    "consider-alternative-union-syntax",
 ]
 
 [tool.pylint.MASTER]
 load-plugins = [
     "pylint.extensions.check_elif",
     "pylint.extensions.bad_builtin",
     "pylint.extensions.code_style",
```

### Comparing `tplbuild-0.1.1/setup.cfg` & `tplbuild-0.1.2/setup.cfg`

 * *Files identical despite different names*

### Comparing `tplbuild-0.1.1/tplbuild/arch.py` & `tplbuild-0.1.2/tplbuild/arch.py`

 * *Files identical despite different names*

### Comparing `tplbuild-0.1.1/tplbuild/builtin_clients.yml` & `tplbuild-0.1.2/tplbuild/builtin_clients.yml`

 * *Files identical despite different names*

### Comparing `tplbuild-0.1.1/tplbuild/cmd/base_build.py` & `tplbuild-0.1.2/tplbuild/cmd/base_build.py`

 * *Files 2% similar despite different names*

```diff
@@ -92,17 +92,18 @@
 
         # Replace BaseImage nodes in the build graph with their underlying
         # build definition.
         await tplbld.resolve_base_images(stages_to_build, dereference=True)
 
         # Create a plan of build operations to execute the requested build.
         build_ops = tplbld.plan(stages_to_build)
+        if not build_ops:
+            print("Base images up to date!")
+            return 0
         if args.check:
-            if not build_ops:
-                return 0
             print(f"Needed {len(build_ops)} build operations")
             return 1
 
         # Execute the build operations.
         if args.debug:
             debug_build_operations(tplbld, build_ops)
         else:
```

### Comparing `tplbuild-0.1.1/tplbuild/cmd/base_lookup.py` & `tplbuild-0.1.2/tplbuild/cmd/base_lookup.py`

 * *Files identical despite different names*

### Comparing `tplbuild-0.1.1/tplbuild/cmd/base_prune.py` & `tplbuild-0.1.2/tplbuild/cmd/base_prune.py`

 * *Files identical despite different names*

### Comparing `tplbuild-0.1.1/tplbuild/cmd/build.py` & `tplbuild-0.1.2/tplbuild/cmd/build.py`

 * *Files identical despite different names*

### Comparing `tplbuild-0.1.1/tplbuild/cmd/common.py` & `tplbuild-0.1.2/tplbuild/cmd/common.py`

 * *Files identical despite different names*

### Comparing `tplbuild-0.1.1/tplbuild/cmd/main.py` & `tplbuild-0.1.2/tplbuild/cmd/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -130,20 +130,22 @@
         default=SUPPRESS,
         help="Load system default certs always",
     )
     parser.add_argument(
         "--build-jobs",
         required=False,
         default=SUPPRESS,
+        type=int,
         help="Set max concurrent build jobs",
     )
     parser.add_argument(
         "--push-jobs",
         required=False,
         default=SUPPRESS,
+        type=int,
         help="Set max concurrent push or pull jobs",
     )
     return parser
 
 
 def setup_logging(verbose: int) -> None:
     """Setup tplbuild default logging based on the verbosity level"""
@@ -209,15 +211,15 @@
         user_config.ssl_context.load_default_certs = True
     if args.build_jobs is not None:
         if args.build_jobs <= 0:
             user_config.build_jobs = os.cpu_count() or 4
         else:
             user_config.build_jobs = args.build_jobs
     if args.push_jobs is not None:
-        if args.build_jobs <= 0:
+        if args.push_jobs <= 0:
             user_config.push_jobs = os.cpu_count() or 4
         else:
             user_config.push_jobs = args.push_jobs
     return user_config
 
 
 def create_registry_client(user_config: UserConfig) -> AsyncRegistryClient:
```

### Comparing `tplbuild-0.1.1/tplbuild/cmd/publish.py` & `tplbuild-0.1.2/tplbuild/cmd/publish.py`

 * *Files identical despite different names*

### Comparing `tplbuild-0.1.1/tplbuild/cmd/source_lookup.py` & `tplbuild-0.1.2/tplbuild/cmd/source_lookup.py`

 * *Files identical despite different names*

### Comparing `tplbuild-0.1.1/tplbuild/cmd/source_update.py` & `tplbuild-0.1.2/tplbuild/cmd/source_update.py`

 * *Files identical despite different names*

### Comparing `tplbuild-0.1.1/tplbuild/cmd/utility.py` & `tplbuild-0.1.2/tplbuild/cmd/utility.py`

 * *Files identical despite different names*

### Comparing `tplbuild-0.1.1/tplbuild/cmd/version.py` & `tplbuild-0.1.2/tplbuild/cmd/version.py`

 * *Files identical despite different names*

### Comparing `tplbuild-0.1.1/tplbuild/config.py` & `tplbuild-0.1.2/tplbuild/config.py`

 * *Files identical despite different names*

### Comparing `tplbuild-0.1.1/tplbuild/context.py` & `tplbuild-0.1.2/tplbuild/context.py`

 * *Files 0% similar despite different names*

```diff
@@ -286,15 +286,15 @@
                 ignored = pattern.ignoring
         return ignored
 
     def walk_context(
         self,
         *,
         extra_files: Optional[Dict[str, Tuple[int, bytes]]] = None,
-        ignore_func: Callable[[str], bool] = None,
+        ignore_func: Optional[Callable[[str], bool]] = None,
     ) -> Iterable[tarfile.TarInfo]:
         """
         Generator that yields TarInfo objects for each not-ignored object
         in the context. Objects are yielded in a deterministic order based on the
         names.
         """
```

### Comparing `tplbuild-0.1.1/tplbuild/exceptions.py` & `tplbuild-0.1.2/tplbuild/exceptions.py`

 * *Files identical despite different names*

### Comparing `tplbuild-0.1.1/tplbuild/executor.py` & `tplbuild-0.1.2/tplbuild/executor.py`

 * *Files identical despite different names*

### Comparing `tplbuild-0.1.1/tplbuild/exit_context.py` & `tplbuild-0.1.2/tplbuild/exit_context.py`

 * *Files identical despite different names*

### Comparing `tplbuild-0.1.1/tplbuild/graph.py` & `tplbuild-0.1.2/tplbuild/graph.py`

 * *Files identical despite different names*

### Comparing `tplbuild-0.1.1/tplbuild/hashing.py` & `tplbuild-0.1.2/tplbuild/hashing.py`

 * *Files identical despite different names*

### Comparing `tplbuild-0.1.1/tplbuild/images.py` & `tplbuild-0.1.2/tplbuild/images.py`

 * *Files identical despite different names*

### Comparing `tplbuild-0.1.1/tplbuild/jinja_source_mapper.py` & `tplbuild-0.1.2/tplbuild/jinja_source_mapper.py`

 * *Files identical despite different names*

### Comparing `tplbuild-0.1.1/tplbuild/output.py` & `tplbuild-0.1.2/tplbuild/output.py`

 * *Files identical despite different names*

### Comparing `tplbuild-0.1.1/tplbuild/plan.py` & `tplbuild-0.1.2/tplbuild/plan.py`

 * *Files identical despite different names*

### Comparing `tplbuild-0.1.1/tplbuild/render.py` & `tplbuild-0.1.2/tplbuild/render.py`

 * *Files identical despite different names*

### Comparing `tplbuild-0.1.1/tplbuild/sync_to_async_pipe.py` & `tplbuild-0.1.2/tplbuild/sync_to_async_pipe.py`

 * *Files identical despite different names*

### Comparing `tplbuild-0.1.1/tplbuild/tplbuild.py` & `tplbuild-0.1.2/tplbuild/tplbuild.py`

 * *Files identical despite different names*

### Comparing `tplbuild-0.1.1/tplbuild/utils.py` & `tplbuild-0.1.2/tplbuild/utils.py`

 * *Files identical despite different names*

### Comparing `tplbuild-0.1.1/tplbuild.egg-info/PKG-INFO` & `tplbuild-0.1.2/tplbuild.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tplbuild
-Version: 0.1.1
+Version: 0.1.2
 Summary: Templated container build tool
 Home-page: http://github.com/msg555/tplbuild/
 Author: Mark Gordon
 Author-email: msg555@gmail.com
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
@@ -39,14 +39,19 @@
 
 
 ## Documentation
 
 Documentation for *tplbuild* can be found
 [here](https://tplbuild.readthedocs.io/)
 
+### Examples
+
+Check out the [examples](examples/) folder in this repo for some example of
+what can be done with `tplbuild`.
+
 ### Demo Video
 
 Additionally, you can find a quick tutorial highlighting key features
 [here](https://youtu.be/HDiyABr8Adw)
 
 [![Tplbuild Demo
 Video](https://img.youtube.com/vi/HDiyABr8Adw/0.jpg)](https://www.youtube.com/watch?v=HDiyABr8Adw "Tplbuild Demo")
```

### Comparing `tplbuild-0.1.1/tplbuild.egg-info/SOURCES.txt` & `tplbuild-0.1.2/tplbuild.egg-info/SOURCES.txt`

 * *Files 12% similar despite different names*

```diff
@@ -1,12 +1,18 @@
 LICENSE
 README.md
 pyproject.toml
 setup.cfg
 setup.py
+tests/test_builds.py
+tests/test_context.py
+tests/test_exit_context.py
+tests/test_graph.py
+tests/test_sync_to_async_pipe.py
+tests/test_utils.py
 tplbuild/__init__.py
 tplbuild/__main__.py
 tplbuild/_version.py
 tplbuild/arch.py
 tplbuild/builtin_clients.yml
 tplbuild/config.py
 tplbuild/context.py
```

