# Comparing `tmp/crdb-0.6.0.tar.gz` & `tmp/crdb-0.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "crdb-0.6.0.tar", last modified: Thu May  4 19:31:48 2023, max compression
+gzip compressed data, was "crdb-0.6.1.tar", last modified: Fri May  5 09:38:57 2023, max compression
```

## Comparing `crdb-0.6.0.tar` & `crdb-0.6.1.tar`

### file list

```diff
@@ -1,49 +1,49 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 19:31:48.391471 crdb-0.6.0/
--rw-r--r--   0 runner    (1001) docker     (123)      172 2023-05-04 19:31:40.000000 crdb-0.6.0/.coveragerc
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 19:31:48.387471 crdb-0.6.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 19:31:48.387471 crdb-0.6.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1123 2023-05-04 19:31:40.000000 crdb-0.6.0/.github/workflows/publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-05-04 19:31:40.000000 crdb-0.6.0/.github/workflows/test.yml
--rw-r--r--   0 runner    (1001) docker     (123)      666 2023-05-04 19:31:40.000000 crdb-0.6.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      637 2023-05-04 19:31:40.000000 crdb-0.6.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      231 2023-05-04 19:31:40.000000 crdb-0.6.0/.readthedocs.yml
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-05-04 19:31:40.000000 crdb-0.6.0/AUTHORS.rst
--rw-r--r--   0 runner    (1001) docker     (123)       94 2023-05-04 19:31:40.000000 crdb-0.6.0/CHANGELOG.rst
--rw-r--r--   0 runner    (1001) docker     (123)     2203 2023-05-04 19:31:40.000000 crdb-0.6.0/CONTRIBUTING.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1103 2023-05-04 19:31:40.000000 crdb-0.6.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      321 2023-05-04 19:31:40.000000 crdb-0.6.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3644 2023-05-04 19:31:48.391471 crdb-0.6.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2504 2023-05-04 19:31:40.000000 crdb-0.6.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 19:31:48.387471 crdb-0.6.0/docs/
--rw-r--r--   0 runner    (1001) docker     (123)       28 2023-05-04 19:31:40.000000 crdb-0.6.0/docs/authors.rst
--rw-r--r--   0 runner    (1001) docker     (123)      253 2023-05-04 19:31:40.000000 crdb-0.6.0/docs/build.py
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-05-04 19:31:40.000000 crdb-0.6.0/docs/changelog.rst
--rw-r--r--   0 runner    (1001) docker     (123)     1199 2023-05-04 19:31:40.000000 crdb-0.6.0/docs/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)       33 2023-05-04 19:31:40.000000 crdb-0.6.0/docs/contributing.rst
--rw-r--r--   0 runner    (1001) docker     (123)      123 2023-05-04 19:31:40.000000 crdb-0.6.0/docs/index.rst
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-04 19:31:40.000000 crdb-0.6.0/docs/reference.rst
--rw-r--r--   0 runner    (1001) docker     (123)      109 2023-05-04 19:31:40.000000 crdb-0.6.0/docs/spelling_wordlist.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2247 2023-05-04 19:31:40.000000 crdb-0.6.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      298 2023-05-04 19:31:48.391471 crdb-0.6.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 19:31:48.387471 crdb-0.6.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 19:31:48.391471 crdb-0.6.0/src/crdb/
--rw-r--r--   0 runner    (1001) docker     (123)      637 2023-05-04 19:31:40.000000 crdb-0.6.0/src/crdb/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      355 2023-05-04 19:31:40.000000 crdb-0.6.0/src/crdb/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)    21214 2023-05-04 19:31:40.000000 crdb-0.6.0/src/crdb/_lib.py
--rw-r--r--   0 runner    (1001) docker     (123)     1891 2023-05-04 19:31:40.000000 crdb-0.6.0/src/crdb/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)    14332 2023-05-04 19:31:40.000000 crdb-0.6.0/src/crdb/crdb_logo.png
--rw-r--r--   0 runner    (1001) docker     (123)     3162 2023-05-04 19:31:40.000000 crdb-0.6.0/src/crdb/experimental.py
--rw-r--r--   0 runner    (1001) docker     (123)     2926 2023-05-04 19:31:40.000000 crdb-0.6.0/src/crdb/mpl.py
--rw-r--r--   0 runner    (1001) docker     (123)     9328 2023-05-04 19:31:40.000000 crdb-0.6.0/src/crdb/solarsystem_abundances2003.dat
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 19:31:48.391471 crdb-0.6.0/src/crdb.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3644 2023-05-04 19:31:48.000000 crdb-0.6.0/src/crdb.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      819 2023-05-04 19:31:48.000000 crdb-0.6.0/src/crdb.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-04 19:31:48.000000 crdb-0.6.0/src/crdb.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       39 2023-05-04 19:31:48.000000 crdb-0.6.0/src/crdb.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       89 2023-05-04 19:31:48.000000 crdb-0.6.0/src/crdb.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-05-04 19:31:48.000000 crdb-0.6.0/src/crdb.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 19:31:48.391471 crdb-0.6.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      253 2023-05-04 19:31:40.000000 crdb-0.6.0/tests/test_cli.py
--rw-r--r--   0 runner    (1001) docker     (123)      636 2023-05-04 19:31:40.000000 crdb-0.6.0/tests/test_experimental.py
--rw-r--r--   0 runner    (1001) docker     (123)     1264 2023-05-04 19:31:40.000000 crdb-0.6.0/tests/test_lib.py
--rw-r--r--   0 runner    (1001) docker     (123)      325 2023-05-04 19:31:40.000000 crdb-0.6.0/tests/test_mpl.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 09:38:57.976195 crdb-0.6.1/
+-rw-r--r--   0 runner    (1001) docker     (123)      172 2023-05-05 09:38:49.000000 crdb-0.6.1/.coveragerc
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 09:38:57.972195 crdb-0.6.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 09:38:57.972195 crdb-0.6.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1123 2023-05-05 09:38:49.000000 crdb-0.6.1/.github/workflows/publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1077 2023-05-05 09:38:49.000000 crdb-0.6.1/.github/workflows/test.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      666 2023-05-05 09:38:49.000000 crdb-0.6.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      637 2023-05-05 09:38:49.000000 crdb-0.6.1/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      231 2023-05-05 09:38:49.000000 crdb-0.6.1/.readthedocs.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-05-05 09:38:49.000000 crdb-0.6.1/AUTHORS.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       94 2023-05-05 09:38:49.000000 crdb-0.6.1/CHANGELOG.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     2203 2023-05-05 09:38:49.000000 crdb-0.6.1/CONTRIBUTING.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1103 2023-05-05 09:38:49.000000 crdb-0.6.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      321 2023-05-05 09:38:49.000000 crdb-0.6.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3644 2023-05-05 09:38:57.976195 crdb-0.6.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2504 2023-05-05 09:38:49.000000 crdb-0.6.1/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 09:38:57.976195 crdb-0.6.1/docs/
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-05-05 09:38:49.000000 crdb-0.6.1/docs/authors.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      253 2023-05-05 09:38:49.000000 crdb-0.6.1/docs/build.py
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-05-05 09:38:49.000000 crdb-0.6.1/docs/changelog.rst
+-rw-r--r--   0 runner    (1001) docker     (123)     1199 2023-05-05 09:38:49.000000 crdb-0.6.1/docs/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-05-05 09:38:49.000000 crdb-0.6.1/docs/contributing.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-05-05 09:38:49.000000 crdb-0.6.1/docs/index.rst
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-05-05 09:38:49.000000 crdb-0.6.1/docs/reference.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      109 2023-05-05 09:38:49.000000 crdb-0.6.1/docs/spelling_wordlist.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     2247 2023-05-05 09:38:49.000000 crdb-0.6.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      298 2023-05-05 09:38:57.976195 crdb-0.6.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 09:38:57.972195 crdb-0.6.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 09:38:57.976195 crdb-0.6.1/src/crdb/
+-rw-r--r--   0 runner    (1001) docker     (123)      637 2023-05-05 09:38:49.000000 crdb-0.6.1/src/crdb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      355 2023-05-05 09:38:49.000000 crdb-0.6.1/src/crdb/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21293 2023-05-05 09:38:49.000000 crdb-0.6.1/src/crdb/_lib.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1891 2023-05-05 09:38:49.000000 crdb-0.6.1/src/crdb/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14332 2023-05-05 09:38:49.000000 crdb-0.6.1/src/crdb/crdb_logo.png
+-rw-r--r--   0 runner    (1001) docker     (123)     3162 2023-05-05 09:38:49.000000 crdb-0.6.1/src/crdb/experimental.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2926 2023-05-05 09:38:49.000000 crdb-0.6.1/src/crdb/mpl.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9328 2023-05-05 09:38:49.000000 crdb-0.6.1/src/crdb/solarsystem_abundances2003.dat
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 09:38:57.976195 crdb-0.6.1/src/crdb.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3644 2023-05-05 09:38:57.000000 crdb-0.6.1/src/crdb.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      819 2023-05-05 09:38:57.000000 crdb-0.6.1/src/crdb.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 09:38:57.000000 crdb-0.6.1/src/crdb.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       39 2023-05-05 09:38:57.000000 crdb-0.6.1/src/crdb.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-05-05 09:38:57.000000 crdb-0.6.1/src/crdb.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-05-05 09:38:57.000000 crdb-0.6.1/src/crdb.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 09:38:57.976195 crdb-0.6.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      253 2023-05-05 09:38:49.000000 crdb-0.6.1/tests/test_cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)      636 2023-05-05 09:38:49.000000 crdb-0.6.1/tests/test_experimental.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1264 2023-05-05 09:38:49.000000 crdb-0.6.1/tests/test_lib.py
+-rw-r--r--   0 runner    (1001) docker     (123)      325 2023-05-05 09:38:49.000000 crdb-0.6.1/tests/test_mpl.py
```

### Comparing `crdb-0.6.0/.github/workflows/publish.yml` & `crdb-0.6.1/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `crdb-0.6.0/.github/workflows/test.yml` & `crdb-0.6.1/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `crdb-0.6.0/.gitignore` & `crdb-0.6.1/.gitignore`

 * *Files identical despite different names*

### Comparing `crdb-0.6.0/.pre-commit-config.yaml` & `crdb-0.6.1/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `crdb-0.6.0/CONTRIBUTING.rst` & `crdb-0.6.1/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `crdb-0.6.0/LICENSE` & `crdb-0.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `crdb-0.6.0/PKG-INFO` & `crdb-0.6.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: crdb
-Version: 0.6.0
+Version: 0.6.1
 Summary: CRDB Python frontend
 Maintainer: Hans Dembinski
 Maintainer-email: hans.dembinski@gmail.com
 License: MIT
 Project-URL: repository, https://github.com/crdb-project/crdb
 Project-URL: documentation, https://lpsc.in2p3.fr/crdb
 Classifier: Development Status :: 4 - Beta
```

### Comparing `crdb-0.6.0/README.rst` & `crdb-0.6.1/README.rst`

 * *Files identical despite different names*

### Comparing `crdb-0.6.0/docs/conf.py` & `crdb-0.6.1/docs/conf.py`

 * *Files identical despite different names*

### Comparing `crdb-0.6.0/pyproject.toml` & `crdb-0.6.1/pyproject.toml`

 * *Files identical despite different names*

### Comparing `crdb-0.6.0/src/crdb/__init__.py` & `crdb-0.6.1/src/crdb/__init__.py`

 * *Files identical despite different names*

### Comparing `crdb-0.6.0/src/crdb/_lib.py` & `crdb-0.6.1/src/crdb/_lib.py`

 * *Files 1% similar despite different names*

```diff
@@ -682,14 +682,16 @@
         for val, key in zip(row, mapping):
             if key is None:
                 continue
             if isinstance(key, tuple):
                 key, pos = key
                 table[idx][key][pos] = val
             else:
+                if key == "is_upper_limit":
+                    val = int(val)
                 table[idx][key] = val
 
     # workaround: replace &amp; in sub_exp strings
     sub_exps = np.unique(table["sub_exp"])
     code = "&amp;"
     for sub_exp in sub_exps:
         if code not in sub_exp:
```

### Comparing `crdb-0.6.0/src/crdb/cli.py` & `crdb-0.6.1/src/crdb/cli.py`

 * *Files identical despite different names*

### Comparing `crdb-0.6.0/src/crdb/crdb_logo.png` & `crdb-0.6.1/src/crdb/crdb_logo.png`

 * *Files identical despite different names*

### Comparing `crdb-0.6.0/src/crdb/experimental.py` & `crdb-0.6.1/src/crdb/experimental.py`

 * *Files identical despite different names*

### Comparing `crdb-0.6.0/src/crdb/mpl.py` & `crdb-0.6.1/src/crdb/mpl.py`

 * *Files identical despite different names*

### Comparing `crdb-0.6.0/src/crdb/solarsystem_abundances2003.dat` & `crdb-0.6.1/src/crdb/solarsystem_abundances2003.dat`

 * *Files identical despite different names*

### Comparing `crdb-0.6.0/src/crdb.egg-info/PKG-INFO` & `crdb-0.6.1/src/crdb.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: crdb
-Version: 0.6.0
+Version: 0.6.1
 Summary: CRDB Python frontend
 Maintainer: Hans Dembinski
 Maintainer-email: hans.dembinski@gmail.com
 License: MIT
 Project-URL: repository, https://github.com/crdb-project/crdb
 Project-URL: documentation, https://lpsc.in2p3.fr/crdb
 Classifier: Development Status :: 4 - Beta
```

### Comparing `crdb-0.6.0/src/crdb.egg-info/SOURCES.txt` & `crdb-0.6.1/src/crdb.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `crdb-0.6.0/tests/test_experimental.py` & `crdb-0.6.1/tests/test_experimental.py`

 * *Files identical despite different names*

### Comparing `crdb-0.6.0/tests/test_lib.py` & `crdb-0.6.1/tests/test_lib.py`

 * *Files identical despite different names*

