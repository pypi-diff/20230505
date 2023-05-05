# Comparing `tmp/pip-compile-multi-2.6.2.tar.gz` & `tmp/pip-compile-multi-2.6.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pip-compile-multi-2.6.2.tar", last modified: Fri Feb 17 19:37:21 2023, max compression
+gzip compressed data, was "pip-compile-multi-2.6.3.tar", last modified: Fri May  5 20:22:14 2023, max compression
```

## Comparing `pip-compile-multi-2.6.2.tar` & `pip-compile-multi-2.6.3.tar`

### file list

```diff
@@ -1,57 +1,57 @@
-drwxr-xr-x   0 peter.demin   (501) staff       (20)        0 2023-02-17 19:37:21.003917 pip-compile-multi-2.6.2/
--rw-r--r--   0 peter.demin   (501) staff       (20)      156 2022-06-30 03:25:41.000000 pip-compile-multi-2.6.2/AUTHORS.rst
--rw-r--r--   0 peter.demin   (501) staff       (20)     3246 2022-06-30 03:25:41.000000 pip-compile-multi-2.6.2/CONTRIBUTING.rst
--rw-r--r--   0 peter.demin   (501) staff       (20)     8055 2023-02-17 19:32:18.000000 pip-compile-multi-2.6.2/HISTORY.rst
--rw-r--r--   0 peter.demin   (501) staff       (20)     1069 2022-06-30 03:25:41.000000 pip-compile-multi-2.6.2/LICENSE.txt
--rw-r--r--   0 peter.demin   (501) staff       (20)      110 2022-06-30 03:25:41.000000 pip-compile-multi-2.6.2/MANIFEST.in
--rw-r--r--   0 peter.demin   (501) staff       (20)     9596 2023-02-17 19:37:21.004054 pip-compile-multi-2.6.2/PKG-INFO
--rw-r--r--   0 peter.demin   (501) staff       (20)     1982 2022-11-04 14:30:40.000000 pip-compile-multi-2.6.2/README.rst
-drwxr-xr-x   0 peter.demin   (501) staff       (20)        0 2023-02-17 19:37:20.988192 pip-compile-multi-2.6.2/pip_compile_multi.egg-info/
--rw-r--r--   0 peter.demin   (501) staff       (20)     9596 2023-02-17 19:37:20.000000 pip-compile-multi-2.6.2/pip_compile_multi.egg-info/PKG-INFO
--rw-r--r--   0 peter.demin   (501) staff       (20)     1655 2023-02-17 19:37:20.000000 pip-compile-multi-2.6.2/pip_compile_multi.egg-info/SOURCES.txt
--rw-r--r--   0 peter.demin   (501) staff       (20)        1 2023-02-17 19:37:20.000000 pip-compile-multi-2.6.2/pip_compile_multi.egg-info/dependency_links.txt
--rw-r--r--   0 peter.demin   (501) staff       (20)       66 2023-02-17 19:37:20.000000 pip-compile-multi-2.6.2/pip_compile_multi.egg-info/entry_points.txt
--rw-r--r--   0 peter.demin   (501) staff       (20)        1 2022-07-15 18:26:11.000000 pip-compile-multi-2.6.2/pip_compile_multi.egg-info/not-zip-safe
--rw-r--r--   0 peter.demin   (501) staff       (20)       32 2023-02-17 19:37:20.000000 pip-compile-multi-2.6.2/pip_compile_multi.egg-info/requires.txt
--rw-r--r--   0 peter.demin   (501) staff       (20)       16 2023-02-17 19:37:20.000000 pip-compile-multi-2.6.2/pip_compile_multi.egg-info/top_level.txt
-drwxr-xr-x   0 peter.demin   (501) staff       (20)        0 2023-02-17 19:37:20.993527 pip-compile-multi-2.6.2/pipcompilemulti/
--rw-r--r--   0 peter.demin   (501) staff       (20)      126 2023-02-17 19:36:23.000000 pip-compile-multi-2.6.2/pipcompilemulti/__init__.py
--rw-r--r--   0 peter.demin   (501) staff       (20)     1424 2022-06-30 03:25:41.000000 pip-compile-multi-2.6.2/pipcompilemulti/actions.py
--rw-r--r--   0 peter.demin   (501) staff       (20)     1586 2022-06-30 03:25:41.000000 pip-compile-multi-2.6.2/pipcompilemulti/cli_v1.py
--rw-r--r--   0 peter.demin   (501) staff       (20)     2457 2022-06-30 03:25:41.000000 pip-compile-multi-2.6.2/pipcompilemulti/cli_v2.py
--rw-r--r--   0 peter.demin   (501) staff       (20)     1925 2022-06-30 03:25:41.000000 pip-compile-multi-2.6.2/pipcompilemulti/config.py
--rw-r--r--   0 peter.demin   (501) staff       (20)     1997 2023-02-17 19:30:39.000000 pip-compile-multi-2.6.2/pipcompilemulti/deduplicate.py
--rw-r--r--   0 peter.demin   (501) staff       (20)     6218 2022-07-15 20:25:06.000000 pip-compile-multi-2.6.2/pipcompilemulti/dependency.py
--rw-r--r--   0 peter.demin   (501) staff       (20)     2210 2022-06-30 03:25:41.000000 pip-compile-multi-2.6.2/pipcompilemulti/discover.py
--rw-r--r--   0 peter.demin   (501) staff       (20)     9566 2022-06-30 03:25:41.000000 pip-compile-multi-2.6.2/pipcompilemulti/environment.py
-drwxr-xr-x   0 peter.demin   (501) staff       (20)        0 2023-02-17 19:37:21.003275 pip-compile-multi-2.6.2/pipcompilemulti/features/
--rw-r--r--   0 peter.demin   (501) staff       (20)      105 2022-06-30 03:25:41.000000 pip-compile-multi-2.6.2/pipcompilemulti/features/__init__.py
--rw-r--r--   0 peter.demin   (501) staff       (20)     3101 2022-06-30 03:25:41.000000 pip-compile-multi-2.6.2/pipcompilemulti/features/add_hashes.py
--rw-r--r--   0 peter.demin   (501) staff       (20)     1360 2022-11-03 13:49:25.000000 pip-compile-multi-2.6.2/pipcompilemulti/features/annotate_index.py
--rw-r--r--   0 peter.demin   (501) staff       (20)     3247 2022-06-30 03:25:41.000000 pip-compile-multi-2.6.2/pipcompilemulti/features/autoresolve.py
--rw-r--r--   0 peter.demin   (501) staff       (20)     1249 2022-11-23 20:57:10.000000 pip-compile-multi-2.6.2/pipcompilemulti/features/backtracking.py
--rw-r--r--   0 peter.demin   (501) staff       (20)     2604 2023-02-01 16:02:44.000000 pip-compile-multi-2.6.2/pipcompilemulti/features/base.py
--rw-r--r--   0 peter.demin   (501) staff       (20)     1167 2022-06-30 03:25:41.000000 pip-compile-multi-2.6.2/pipcompilemulti/features/base_dir.py
--rw-r--r--   0 peter.demin   (501) staff       (20)     1144 2022-06-30 03:25:41.000000 pip-compile-multi-2.6.2/pipcompilemulti/features/build_isolation.py
--rw-r--r--   0 peter.demin   (501) staff       (20)     1844 2022-06-30 03:25:41.000000 pip-compile-multi-2.6.2/pipcompilemulti/features/compatible.py
--rw-r--r--   0 peter.demin   (501) staff       (20)     6848 2022-11-23 20:57:10.000000 pip-compile-multi-2.6.2/pipcompilemulti/features/controller.py
--rw-r--r--   0 peter.demin   (501) staff       (20)     1425 2022-11-03 13:57:23.000000 pip-compile-multi-2.6.2/pipcompilemulti/features/emit_trusted_host.py
--rw-r--r--   0 peter.demin   (501) staff       (20)     2192 2022-06-30 03:25:41.000000 pip-compile-multi-2.6.2/pipcompilemulti/features/extra_index_url.py
--rw-r--r--   0 peter.demin   (501) staff       (20)     1544 2022-06-30 03:25:41.000000 pip-compile-multi-2.6.2/pipcompilemulti/features/file_extensions.py
--rw-r--r--   0 peter.demin   (501) staff       (20)     1666 2022-06-30 03:25:41.000000 pip-compile-multi-2.6.2/pipcompilemulti/features/forbid_post.py
--rw-r--r--   0 peter.demin   (501) staff       (20)      608 2022-06-30 03:25:41.000000 pip-compile-multi-2.6.2/pipcompilemulti/features/forward.py
--rw-r--r--   0 peter.demin   (501) staff       (20)     1228 2022-06-30 03:25:41.000000 pip-compile-multi-2.6.2/pipcompilemulti/features/header.py
--rw-r--r--   0 peter.demin   (501) staff       (20)     1760 2022-06-30 03:25:41.000000 pip-compile-multi-2.6.2/pipcompilemulti/features/limit_envs.py
--rw-r--r--   0 peter.demin   (501) staff       (20)     2602 2022-06-30 03:25:41.000000 pip-compile-multi-2.6.2/pipcompilemulti/features/limit_in_paths.py
--rw-r--r--   0 peter.demin   (501) staff       (20)      911 2022-06-30 03:25:41.000000 pip-compile-multi-2.6.2/pipcompilemulti/features/live_output.py
--rw-r--r--   0 peter.demin   (501) staff       (20)     2977 2022-06-30 03:25:41.000000 pip-compile-multi-2.6.2/pipcompilemulti/features/skip_constraint_comments.py
--rw-r--r--   0 peter.demin   (501) staff       (20)     1291 2022-06-30 03:25:41.000000 pip-compile-multi-2.6.2/pipcompilemulti/features/unsafe.py
--rw-r--r--   0 peter.demin   (501) staff       (20)     3975 2022-06-30 03:25:41.000000 pip-compile-multi-2.6.2/pipcompilemulti/features/upgrade.py
--rw-r--r--   0 peter.demin   (501) staff       (20)     1176 2022-06-30 03:25:41.000000 pip-compile-multi-2.6.2/pipcompilemulti/features/use_cache.py
--rw-r--r--   0 peter.demin   (501) staff       (20)      198 2022-06-30 03:25:41.000000 pip-compile-multi-2.6.2/pipcompilemulti/options.py
--rw-r--r--   0 peter.demin   (501) staff       (20)     3403 2022-06-30 03:25:41.000000 pip-compile-multi-2.6.2/pipcompilemulti/utils.py
--rw-r--r--   0 peter.demin   (501) staff       (20)     4183 2022-06-30 03:25:41.000000 pip-compile-multi-2.6.2/pipcompilemulti/verify.py
-drwxr-xr-x   0 peter.demin   (501) staff       (20)        0 2023-02-17 19:37:21.003634 pip-compile-multi-2.6.2/requirements/
--rw-r--r--   0 peter.demin   (501) staff       (20)       32 2022-11-23 20:57:10.000000 pip-compile-multi-2.6.2/requirements/base.in
--rw-r--r--   0 peter.demin   (501) staff       (20)      630 2023-02-17 19:37:21.004582 pip-compile-multi-2.6.2/setup.cfg
--rw-r--r--   0 peter.demin   (501) staff       (20)     2370 2023-02-17 19:36:23.000000 pip-compile-multi-2.6.2/setup.py
+drwxr-xr-x   0 peter.demin   (501) staff       (20)        0 2023-05-05 20:22:14.134042 pip-compile-multi-2.6.3/
+-rw-r--r--   0 peter.demin   (501) staff       (20)      156 2022-06-30 03:25:41.000000 pip-compile-multi-2.6.3/AUTHORS.rst
+-rw-r--r--   0 peter.demin   (501) staff       (20)     3246 2022-06-30 03:25:41.000000 pip-compile-multi-2.6.3/CONTRIBUTING.rst
+-rw-r--r--   0 peter.demin   (501) staff       (20)     8397 2023-05-05 20:20:44.000000 pip-compile-multi-2.6.3/HISTORY.rst
+-rw-r--r--   0 peter.demin   (501) staff       (20)     1069 2022-06-30 03:25:41.000000 pip-compile-multi-2.6.3/LICENSE.txt
+-rw-r--r--   0 peter.demin   (501) staff       (20)      110 2022-06-30 03:25:41.000000 pip-compile-multi-2.6.3/MANIFEST.in
+-rw-r--r--   0 peter.demin   (501) staff       (20)     9938 2023-05-05 20:22:14.134164 pip-compile-multi-2.6.3/PKG-INFO
+-rw-r--r--   0 peter.demin   (501) staff       (20)     1982 2022-11-04 14:30:40.000000 pip-compile-multi-2.6.3/README.rst
+drwxr-xr-x   0 peter.demin   (501) staff       (20)        0 2023-05-05 20:22:14.117922 pip-compile-multi-2.6.3/pip_compile_multi.egg-info/
+-rw-r--r--   0 peter.demin   (501) staff       (20)     9938 2023-05-05 20:22:14.000000 pip-compile-multi-2.6.3/pip_compile_multi.egg-info/PKG-INFO
+-rw-r--r--   0 peter.demin   (501) staff       (20)     1655 2023-05-05 20:22:14.000000 pip-compile-multi-2.6.3/pip_compile_multi.egg-info/SOURCES.txt
+-rw-r--r--   0 peter.demin   (501) staff       (20)        1 2023-05-05 20:22:14.000000 pip-compile-multi-2.6.3/pip_compile_multi.egg-info/dependency_links.txt
+-rw-r--r--   0 peter.demin   (501) staff       (20)       66 2023-05-05 20:22:14.000000 pip-compile-multi-2.6.3/pip_compile_multi.egg-info/entry_points.txt
+-rw-r--r--   0 peter.demin   (501) staff       (20)        1 2022-07-15 18:26:11.000000 pip-compile-multi-2.6.3/pip_compile_multi.egg-info/not-zip-safe
+-rw-r--r--   0 peter.demin   (501) staff       (20)       32 2023-05-05 20:22:14.000000 pip-compile-multi-2.6.3/pip_compile_multi.egg-info/requires.txt
+-rw-r--r--   0 peter.demin   (501) staff       (20)       16 2023-05-05 20:22:14.000000 pip-compile-multi-2.6.3/pip_compile_multi.egg-info/top_level.txt
+drwxr-xr-x   0 peter.demin   (501) staff       (20)        0 2023-05-05 20:22:14.123139 pip-compile-multi-2.6.3/pipcompilemulti/
+-rw-r--r--   0 peter.demin   (501) staff       (20)      126 2023-05-05 20:21:01.000000 pip-compile-multi-2.6.3/pipcompilemulti/__init__.py
+-rw-r--r--   0 peter.demin   (501) staff       (20)     1424 2022-06-30 03:25:41.000000 pip-compile-multi-2.6.3/pipcompilemulti/actions.py
+-rw-r--r--   0 peter.demin   (501) staff       (20)     1586 2022-06-30 03:25:41.000000 pip-compile-multi-2.6.3/pipcompilemulti/cli_v1.py
+-rw-r--r--   0 peter.demin   (501) staff       (20)     2457 2022-06-30 03:25:41.000000 pip-compile-multi-2.6.3/pipcompilemulti/cli_v2.py
+-rw-r--r--   0 peter.demin   (501) staff       (20)     1925 2022-06-30 03:25:41.000000 pip-compile-multi-2.6.3/pipcompilemulti/config.py
+-rw-r--r--   0 peter.demin   (501) staff       (20)     1997 2023-02-17 19:30:39.000000 pip-compile-multi-2.6.3/pipcompilemulti/deduplicate.py
+-rw-r--r--   0 peter.demin   (501) staff       (20)     6218 2022-07-15 20:25:06.000000 pip-compile-multi-2.6.3/pipcompilemulti/dependency.py
+-rw-r--r--   0 peter.demin   (501) staff       (20)     2210 2022-06-30 03:25:41.000000 pip-compile-multi-2.6.3/pipcompilemulti/discover.py
+-rw-r--r--   0 peter.demin   (501) staff       (20)     9566 2022-06-30 03:25:41.000000 pip-compile-multi-2.6.3/pipcompilemulti/environment.py
+drwxr-xr-x   0 peter.demin   (501) staff       (20)        0 2023-05-05 20:22:14.133434 pip-compile-multi-2.6.3/pipcompilemulti/features/
+-rw-r--r--   0 peter.demin   (501) staff       (20)      105 2022-06-30 03:25:41.000000 pip-compile-multi-2.6.3/pipcompilemulti/features/__init__.py
+-rw-r--r--   0 peter.demin   (501) staff       (20)     3101 2022-06-30 03:25:41.000000 pip-compile-multi-2.6.3/pipcompilemulti/features/add_hashes.py
+-rw-r--r--   0 peter.demin   (501) staff       (20)     1360 2022-11-03 13:49:25.000000 pip-compile-multi-2.6.3/pipcompilemulti/features/annotate_index.py
+-rw-r--r--   0 peter.demin   (501) staff       (20)     3247 2022-06-30 03:25:41.000000 pip-compile-multi-2.6.3/pipcompilemulti/features/autoresolve.py
+-rw-r--r--   0 peter.demin   (501) staff       (20)     1249 2022-11-23 20:57:10.000000 pip-compile-multi-2.6.3/pipcompilemulti/features/backtracking.py
+-rw-r--r--   0 peter.demin   (501) staff       (20)     2604 2023-02-01 16:02:44.000000 pip-compile-multi-2.6.3/pipcompilemulti/features/base.py
+-rw-r--r--   0 peter.demin   (501) staff       (20)     1167 2022-06-30 03:25:41.000000 pip-compile-multi-2.6.3/pipcompilemulti/features/base_dir.py
+-rw-r--r--   0 peter.demin   (501) staff       (20)     1144 2022-06-30 03:25:41.000000 pip-compile-multi-2.6.3/pipcompilemulti/features/build_isolation.py
+-rw-r--r--   0 peter.demin   (501) staff       (20)     1844 2022-06-30 03:25:41.000000 pip-compile-multi-2.6.3/pipcompilemulti/features/compatible.py
+-rw-r--r--   0 peter.demin   (501) staff       (20)     6848 2022-11-23 20:57:10.000000 pip-compile-multi-2.6.3/pipcompilemulti/features/controller.py
+-rw-r--r--   0 peter.demin   (501) staff       (20)     1425 2022-11-03 13:57:23.000000 pip-compile-multi-2.6.3/pipcompilemulti/features/emit_trusted_host.py
+-rw-r--r--   0 peter.demin   (501) staff       (20)     2192 2022-06-30 03:25:41.000000 pip-compile-multi-2.6.3/pipcompilemulti/features/extra_index_url.py
+-rw-r--r--   0 peter.demin   (501) staff       (20)     1544 2022-06-30 03:25:41.000000 pip-compile-multi-2.6.3/pipcompilemulti/features/file_extensions.py
+-rw-r--r--   0 peter.demin   (501) staff       (20)     1666 2022-06-30 03:25:41.000000 pip-compile-multi-2.6.3/pipcompilemulti/features/forbid_post.py
+-rw-r--r--   0 peter.demin   (501) staff       (20)      608 2022-06-30 03:25:41.000000 pip-compile-multi-2.6.3/pipcompilemulti/features/forward.py
+-rw-r--r--   0 peter.demin   (501) staff       (20)     1228 2022-06-30 03:25:41.000000 pip-compile-multi-2.6.3/pipcompilemulti/features/header.py
+-rw-r--r--   0 peter.demin   (501) staff       (20)     1760 2022-06-30 03:25:41.000000 pip-compile-multi-2.6.3/pipcompilemulti/features/limit_envs.py
+-rw-r--r--   0 peter.demin   (501) staff       (20)     2602 2022-06-30 03:25:41.000000 pip-compile-multi-2.6.3/pipcompilemulti/features/limit_in_paths.py
+-rw-r--r--   0 peter.demin   (501) staff       (20)      911 2022-06-30 03:25:41.000000 pip-compile-multi-2.6.3/pipcompilemulti/features/live_output.py
+-rw-r--r--   0 peter.demin   (501) staff       (20)     2977 2022-06-30 03:25:41.000000 pip-compile-multi-2.6.3/pipcompilemulti/features/skip_constraint_comments.py
+-rw-r--r--   0 peter.demin   (501) staff       (20)     1291 2022-06-30 03:25:41.000000 pip-compile-multi-2.6.3/pipcompilemulti/features/unsafe.py
+-rw-r--r--   0 peter.demin   (501) staff       (20)     4504 2023-05-05 20:20:42.000000 pip-compile-multi-2.6.3/pipcompilemulti/features/upgrade.py
+-rw-r--r--   0 peter.demin   (501) staff       (20)     1176 2022-06-30 03:25:41.000000 pip-compile-multi-2.6.3/pipcompilemulti/features/use_cache.py
+-rw-r--r--   0 peter.demin   (501) staff       (20)      198 2022-06-30 03:25:41.000000 pip-compile-multi-2.6.3/pipcompilemulti/options.py
+-rw-r--r--   0 peter.demin   (501) staff       (20)     3403 2022-06-30 03:25:41.000000 pip-compile-multi-2.6.3/pipcompilemulti/utils.py
+-rw-r--r--   0 peter.demin   (501) staff       (20)     4183 2022-06-30 03:25:41.000000 pip-compile-multi-2.6.3/pipcompilemulti/verify.py
+drwxr-xr-x   0 peter.demin   (501) staff       (20)        0 2023-05-05 20:22:14.133749 pip-compile-multi-2.6.3/requirements/
+-rw-r--r--   0 peter.demin   (501) staff       (20)       32 2022-11-23 20:57:10.000000 pip-compile-multi-2.6.3/requirements/base.in
+-rw-r--r--   0 peter.demin   (501) staff       (20)      630 2023-05-05 20:22:14.134706 pip-compile-multi-2.6.3/setup.cfg
+-rw-r--r--   0 peter.demin   (501) staff       (20)     2370 2023-05-05 20:21:01.000000 pip-compile-multi-2.6.3/setup.py
```

### Comparing `pip-compile-multi-2.6.2/CONTRIBUTING.rst` & `pip-compile-multi-2.6.3/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `pip-compile-multi-2.6.2/HISTORY.rst` & `pip-compile-multi-2.6.3/HISTORY.rst`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,20 @@
 History
 =======
 
+2.6.3 (2023-05-05)
+------------------
+
+* Allow version constraints in ``--upgrade-package`` parameters.
+  (Issue `#392`_, PR `#394`_, thanks to `Peter Law`_.)
+
+.. _#392: https://github.com/peterdemin/pip-compile-multi/issues/392
+.. _#394: https://github.com/peterdemin/pip-compile-multi/pull/394
+.. _Peter Law: https://github.com/PeterJCLaw
+
 2.6.2 (2023-02-23)
 ------------------
 
 * Fix package name normalization for names with delimiters (``urltemplate`` != ``url-template``).
 
 
 2.6.1 (2022-11-23)
```

### Comparing `pip-compile-multi-2.6.2/LICENSE.txt` & `pip-compile-multi-2.6.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pip-compile-multi-2.6.2/PKG-INFO` & `pip-compile-multi-2.6.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pip-compile-multi
-Version: 2.6.2
+Version: 2.6.3
 Summary: Compile multiple requirements files to lock dependency versions
 Home-page: https://github.com/peterdemin/pip-compile-multi
 Author: Peter Demin
 Author-email: peterdemin@gmail.com
 License: MIT
 Keywords: pip-compile-multi
 Platform: UNKNOWN
@@ -55,14 +55,24 @@
 * Issue tracker: https://github.com/peterdemin/pip-compile-multi/issues
 
 
 
 History
 =======
 
+2.6.3 (2023-05-05)
+------------------
+
+* Allow version constraints in ``--upgrade-package`` parameters.
+  (Issue `#392`_, PR `#394`_, thanks to `Peter Law`_.)
+
+.. _#392: https://github.com/peterdemin/pip-compile-multi/issues/392
+.. _#394: https://github.com/peterdemin/pip-compile-multi/pull/394
+.. _Peter Law: https://github.com/PeterJCLaw
+
 2.6.2 (2023-02-23)
 ------------------
 
 * Fix package name normalization for names with delimiters (``urltemplate`` != ``url-template``).
 
 
 2.6.1 (2022-11-23)
```

### Comparing `pip-compile-multi-2.6.2/README.rst` & `pip-compile-multi-2.6.3/README.rst`

 * *Files identical despite different names*

### Comparing `pip-compile-multi-2.6.2/pip_compile_multi.egg-info/PKG-INFO` & `pip-compile-multi-2.6.3/pip_compile_multi.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pip-compile-multi
-Version: 2.6.2
+Version: 2.6.3
 Summary: Compile multiple requirements files to lock dependency versions
 Home-page: https://github.com/peterdemin/pip-compile-multi
 Author: Peter Demin
 Author-email: peterdemin@gmail.com
 License: MIT
 Keywords: pip-compile-multi
 Platform: UNKNOWN
@@ -55,14 +55,24 @@
 * Issue tracker: https://github.com/peterdemin/pip-compile-multi/issues
 
 
 
 History
 =======
 
+2.6.3 (2023-05-05)
+------------------
+
+* Allow version constraints in ``--upgrade-package`` parameters.
+  (Issue `#392`_, PR `#394`_, thanks to `Peter Law`_.)
+
+.. _#392: https://github.com/peterdemin/pip-compile-multi/issues/392
+.. _#394: https://github.com/peterdemin/pip-compile-multi/pull/394
+.. _Peter Law: https://github.com/PeterJCLaw
+
 2.6.2 (2023-02-23)
 ------------------
 
 * Fix package name normalization for names with delimiters (``urltemplate`` != ``url-template``).
 
 
 2.6.1 (2022-11-23)
```

### Comparing `pip-compile-multi-2.6.2/pip_compile_multi.egg-info/SOURCES.txt` & `pip-compile-multi-2.6.3/pip_compile_multi.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pip-compile-multi-2.6.2/pipcompilemulti/actions.py` & `pip-compile-multi-2.6.3/pipcompilemulti/actions.py`

 * *Files identical despite different names*

### Comparing `pip-compile-multi-2.6.2/pipcompilemulti/cli_v1.py` & `pip-compile-multi-2.6.3/pipcompilemulti/cli_v1.py`

 * *Files identical despite different names*

### Comparing `pip-compile-multi-2.6.2/pipcompilemulti/cli_v2.py` & `pip-compile-multi-2.6.3/pipcompilemulti/cli_v2.py`

 * *Files identical despite different names*

### Comparing `pip-compile-multi-2.6.2/pipcompilemulti/config.py` & `pip-compile-multi-2.6.3/pipcompilemulti/config.py`

 * *Files identical despite different names*

### Comparing `pip-compile-multi-2.6.2/pipcompilemulti/deduplicate.py` & `pip-compile-multi-2.6.3/pipcompilemulti/deduplicate.py`

 * *Files identical despite different names*

### Comparing `pip-compile-multi-2.6.2/pipcompilemulti/dependency.py` & `pip-compile-multi-2.6.3/pipcompilemulti/dependency.py`

 * *Files identical despite different names*

### Comparing `pip-compile-multi-2.6.2/pipcompilemulti/discover.py` & `pip-compile-multi-2.6.3/pipcompilemulti/discover.py`

 * *Files identical despite different names*

### Comparing `pip-compile-multi-2.6.2/pipcompilemulti/environment.py` & `pip-compile-multi-2.6.3/pipcompilemulti/environment.py`

 * *Files identical despite different names*

### Comparing `pip-compile-multi-2.6.2/pipcompilemulti/features/add_hashes.py` & `pip-compile-multi-2.6.3/pipcompilemulti/features/add_hashes.py`

 * *Files identical despite different names*

### Comparing `pip-compile-multi-2.6.2/pipcompilemulti/features/annotate_index.py` & `pip-compile-multi-2.6.3/pipcompilemulti/features/annotate_index.py`

 * *Files identical despite different names*

### Comparing `pip-compile-multi-2.6.2/pipcompilemulti/features/autoresolve.py` & `pip-compile-multi-2.6.3/pipcompilemulti/features/autoresolve.py`

 * *Files identical despite different names*

### Comparing `pip-compile-multi-2.6.2/pipcompilemulti/features/backtracking.py` & `pip-compile-multi-2.6.3/pipcompilemulti/features/backtracking.py`

 * *Files identical despite different names*

### Comparing `pip-compile-multi-2.6.2/pipcompilemulti/features/base.py` & `pip-compile-multi-2.6.3/pipcompilemulti/features/base.py`

 * *Files identical despite different names*

### Comparing `pip-compile-multi-2.6.2/pipcompilemulti/features/base_dir.py` & `pip-compile-multi-2.6.3/pipcompilemulti/features/base_dir.py`

 * *Files identical despite different names*

### Comparing `pip-compile-multi-2.6.2/pipcompilemulti/features/build_isolation.py` & `pip-compile-multi-2.6.3/pipcompilemulti/features/build_isolation.py`

 * *Files identical despite different names*

### Comparing `pip-compile-multi-2.6.2/pipcompilemulti/features/compatible.py` & `pip-compile-multi-2.6.3/pipcompilemulti/features/compatible.py`

 * *Files identical despite different names*

### Comparing `pip-compile-multi-2.6.2/pipcompilemulti/features/controller.py` & `pip-compile-multi-2.6.3/pipcompilemulti/features/controller.py`

 * *Files identical despite different names*

### Comparing `pip-compile-multi-2.6.2/pipcompilemulti/features/emit_trusted_host.py` & `pip-compile-multi-2.6.3/pipcompilemulti/features/emit_trusted_host.py`

 * *Files identical despite different names*

### Comparing `pip-compile-multi-2.6.2/pipcompilemulti/features/extra_index_url.py` & `pip-compile-multi-2.6.3/pipcompilemulti/features/extra_index_url.py`

 * *Files identical despite different names*

### Comparing `pip-compile-multi-2.6.2/pipcompilemulti/features/file_extensions.py` & `pip-compile-multi-2.6.3/pipcompilemulti/features/file_extensions.py`

 * *Files identical despite different names*

### Comparing `pip-compile-multi-2.6.2/pipcompilemulti/features/forbid_post.py` & `pip-compile-multi-2.6.3/pipcompilemulti/features/forbid_post.py`

 * *Files identical despite different names*

### Comparing `pip-compile-multi-2.6.2/pipcompilemulti/features/forward.py` & `pip-compile-multi-2.6.3/pipcompilemulti/features/forward.py`

 * *Files identical despite different names*

### Comparing `pip-compile-multi-2.6.2/pipcompilemulti/features/header.py` & `pip-compile-multi-2.6.3/pipcompilemulti/features/header.py`

 * *Files identical despite different names*

### Comparing `pip-compile-multi-2.6.2/pipcompilemulti/features/limit_envs.py` & `pip-compile-multi-2.6.3/pipcompilemulti/features/limit_envs.py`

 * *Files identical despite different names*

### Comparing `pip-compile-multi-2.6.2/pipcompilemulti/features/limit_in_paths.py` & `pip-compile-multi-2.6.3/pipcompilemulti/features/limit_in_paths.py`

 * *Files identical despite different names*

### Comparing `pip-compile-multi-2.6.2/pipcompilemulti/features/live_output.py` & `pip-compile-multi-2.6.3/pipcompilemulti/features/live_output.py`

 * *Files identical despite different names*

### Comparing `pip-compile-multi-2.6.2/pipcompilemulti/features/skip_constraint_comments.py` & `pip-compile-multi-2.6.3/pipcompilemulti/features/skip_constraint_comments.py`

 * *Files identical despite different names*

### Comparing `pip-compile-multi-2.6.2/pipcompilemulti/features/unsafe.py` & `pip-compile-multi-2.6.3/pipcompilemulti/features/unsafe.py`

 * *Files identical despite different names*

### Comparing `pip-compile-multi-2.6.2/pipcompilemulti/features/upgrade.py` & `pip-compile-multi-2.6.3/pipcompilemulti/features/upgrade.py`

 * *Files 6% similar despite different names*

```diff
@@ -29,14 +29,16 @@
 
 Thanks to `Jonathan Rogers <https://github.com/JonathanRRogers>`_.
 
 .. _`the same option of pip-compile`: \
         https://github.com/jazzband/pip-tools#updating-requirements
 """
 
+import re
+
 from .base import BaseFeature, ClickOption
 from .forward import ForwardOption
 
 
 class UpgradeAll(ForwardOption):
     """Upgrade all packages in all environments."""
 
@@ -66,37 +68,53 @@
         long_option='--upgrade-package',
         short_option='-P',
         multiple=True,
         help_text='Only upgrade named package. '
                   'Can be supplied multiple times.',
     )
 
+    RE_PACKAGE_NAME = re.compile(
+        r'(?iu)(?P<package>[a-z0-9-_.]+)',
+    )
+
     def __init__(self, controller):
         self._controller = controller
         self.reset()
 
     def reset(self):
         """Clear cached packages."""
         self._env_packages_cache = {}
 
     @property
+    def package_specs(self):
+        """List of package specs to upgrade."""
+        return self.value or []
+
+    @property
     def package_names(self):
         """List of package names to upgrade."""
-        return self.value or []
+        def name_from_spec(name):
+            match = self.RE_PACKAGE_NAME.match(name)
+            if match is None:
+                raise ValueError(
+                    f"{name!r} does not appear to be a valid package spec",
+                )
+            return match.group(0)
+        return [name_from_spec(x) for x in self.package_specs]
 
     @property
     def active(self):
         """Whether selective upgrade is active."""
         return bool(self.package_names)
 
     def pin_options(self):
         """Pin command options for upgrading specific packages."""
         return [
             '--upgrade-package=' + package
-            for package in self.package_names
+            for package in self.package_specs
         ]
 
     def has_package(self, in_path, package_name):
         """Whether specified package name is already in the outfile."""
         return package_name.lower() in self._get_packages(in_path)
 
     def _get_packages(self, in_path):
```

### Comparing `pip-compile-multi-2.6.2/pipcompilemulti/features/use_cache.py` & `pip-compile-multi-2.6.3/pipcompilemulti/features/use_cache.py`

 * *Files identical despite different names*

### Comparing `pip-compile-multi-2.6.2/pipcompilemulti/utils.py` & `pip-compile-multi-2.6.3/pipcompilemulti/utils.py`

 * *Files identical despite different names*

### Comparing `pip-compile-multi-2.6.2/pipcompilemulti/verify.py` & `pip-compile-multi-2.6.3/pipcompilemulti/verify.py`

 * *Files identical despite different names*

### Comparing `pip-compile-multi-2.6.2/setup.cfg` & `pip-compile-multi-2.6.3/setup.cfg`

 * *Files 14% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [bumpversion]
-current_version = 2.6.2
+current_version = 2.6.3
 commit = True
 tag = True
 
 [wheel]
 universal = 1
 
 [bdist_wheel]
```

### Comparing `pip-compile-multi-2.6.2/setup.py` & `pip-compile-multi-2.6.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 """Package configuration"""
 
 import os
 from setuptools import setup, find_packages
 
 
-VERSION = "2.6.2"
+VERSION = "2.6.3"
 
 
 README = """
 pip-compile-multi
 =================
 
 Compile multiple requirements files to lock dependency versions.
```

