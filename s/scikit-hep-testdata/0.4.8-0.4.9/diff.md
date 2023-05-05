# Comparing `tmp/scikit_hep_testdata-0.4.8.tar.gz` & `tmp/scikit_hep_testdata-0.4.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "scikit_hep_testdata-0.4.8.tar", last modified: Sat Sep 18 02:14:57 2021, max compression
+gzip compressed data, was "scikit_hep_testdata-0.4.9.tar", last modified: Mon Sep 27 16:40:45 2021, max compression
```

## Comparing `scikit_hep_testdata-0.4.8.tar` & `scikit_hep_testdata-0.4.9.tar`

### file list

```diff
@@ -1,45 +1,46 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-18 02:14:57.676972 scikit_hep_testdata-0.4.8/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-18 02:14:57.672972 scikit_hep_testdata-0.4.8/.github/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-18 02:14:57.676972 scikit_hep_testdata-0.4.8/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (121)     2112 2021-09-18 02:14:39.000000 scikit_hep_testdata-0.4.8/.github/workflows/ci.yml
--rw-r--r--   0 runner    (1001) docker     (121)     1308 2021-09-18 02:14:39.000000 scikit_hep_testdata-0.4.8/.gitignore
--rw-r--r--   0 runner    (1001) docker     (121)     1252 2021-09-18 02:14:39.000000 scikit_hep_testdata-0.4.8/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (121)     1511 2021-09-18 02:14:39.000000 scikit_hep_testdata-0.4.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)      185 2021-09-18 02:14:39.000000 scikit_hep_testdata-0.4.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     5223 2021-09-18 02:14:57.676972 scikit_hep_testdata-0.4.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     4084 2021-09-18 02:14:39.000000 scikit_hep_testdata-0.4.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-18 02:14:57.672972 scikit_hep_testdata-0.4.8/dev/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-18 02:14:57.676972 scikit_hep_testdata-0.4.8/dev/make-root/
--rw-r--r--   0 runner    (1001) docker     (121)     5405 2021-09-18 02:14:39.000000 scikit_hep_testdata-0.4.8/dev/make-root/double32_float16.C
--rw-r--r--   0 runner    (1001) docker     (121)     4739 2021-09-18 02:14:39.000000 scikit_hep_testdata-0.4.8/dev/make-root/sample4version.C
--rw-r--r--   0 runner    (1001) docker     (121)    31229 2021-09-18 02:14:39.000000 scikit_hep_testdata-0.4.8/dev/make-root/stl_containers.C
--rw-r--r--   0 runner    (1001) docker     (121)      727 2021-09-18 02:14:39.000000 scikit_hep_testdata-0.4.8/dev/make-root/uproot-issue38c.py
--rw-r--r--   0 runner    (1001) docker     (121)      967 2021-09-18 02:14:39.000000 scikit_hep_testdata-0.4.8/dev/make-root/uproot_issue_407.C
--rw-r--r--   0 runner    (1001) docker     (121)      203 2021-09-18 02:14:39.000000 scikit_hep_testdata-0.4.8/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (121)     2515 2021-09-18 02:14:57.680971 scikit_hep_testdata-0.4.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1046 2021-09-18 02:14:39.000000 scikit_hep_testdata-0.4.8/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-18 02:14:57.672972 scikit_hep_testdata-0.4.8/src/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-18 02:14:57.676972 scikit_hep_testdata-0.4.8/src/scikit_hep_testdata.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     5223 2021-09-18 02:14:55.000000 scikit_hep_testdata-0.4.8/src/scikit_hep_testdata.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     9578 2021-09-18 02:14:57.000000 scikit_hep_testdata-0.4.8/src/scikit_hep_testdata.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-09-18 02:14:55.000000 scikit_hep_testdata-0.4.8/src/scikit_hep_testdata.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)      116 2021-09-18 02:14:55.000000 scikit_hep_testdata-0.4.8/src/scikit_hep_testdata.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)      165 2021-09-18 02:14:55.000000 scikit_hep_testdata-0.4.8/src/scikit_hep_testdata.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       15 2021-09-18 02:14:55.000000 scikit_hep_testdata-0.4.8/src/scikit_hep_testdata.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2021-09-18 02:14:52.000000 scikit_hep_testdata-0.4.8/src/scikit_hep_testdata.egg-info/zip-safe
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-18 02:14:57.676972 scikit_hep_testdata-0.4.8/src/skhep_testdata/
--rw-r--r--   0 runner    (1001) docker     (121)      337 2021-09-18 02:14:39.000000 scikit_hep_testdata-0.4.8/src/skhep_testdata/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1170 2021-09-18 02:14:39.000000 scikit_hep_testdata-0.4.8/src/skhep_testdata/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-18 02:14:57.676972 scikit_hep_testdata-0.4.8/src/skhep_testdata/data/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-09-18 02:14:39.000000 scikit_hep_testdata-0.4.8/src/skhep_testdata/data/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     4412 2021-09-18 02:14:55.000000 scikit_hep_testdata-0.4.8/src/skhep_testdata/data/file_list.txt
--rw-r--r--   0 runner    (1001) docker     (121)     2922 2021-09-18 02:14:41.000000 scikit_hep_testdata-0.4.8/src/skhep_testdata/local_files.py
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-09-18 02:14:41.000000 scikit_hep_testdata-0.4.8/src/skhep_testdata/py.typed
--rw-r--r--   0 runner    (1001) docker     (121)      787 2021-09-18 02:14:41.000000 scikit_hep_testdata-0.4.8/src/skhep_testdata/remote_datasets.yml
--rw-r--r--   0 runner    (1001) docker     (121)     4042 2021-09-18 02:14:41.000000 scikit_hep_testdata-0.4.8/src/skhep_testdata/remote_files.py
--rw-r--r--   0 runner    (1001) docker     (121)      142 2021-09-18 02:14:55.000000 scikit_hep_testdata-0.4.8/src/skhep_testdata/version.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-18 02:14:57.676972 scikit_hep_testdata-0.4.8/tests/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2021-09-18 02:14:41.000000 scikit_hep_testdata-0.4.8/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1129 2021-09-18 02:14:41.000000 scikit_hep_testdata-0.4.8/tests/test_local_files.py
--rw-r--r--   0 runner    (1001) docker     (121)      182 2021-09-18 02:14:41.000000 scikit_hep_testdata-0.4.8/tests/test_remote_datasets.yml
--rw-r--r--   0 runner    (1001) docker     (121)     1401 2021-09-18 02:14:41.000000 scikit_hep_testdata-0.4.8/tests/test_remote_files.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-27 16:40:45.965185 scikit_hep_testdata-0.4.9/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-27 16:40:45.949184 scikit_hep_testdata-0.4.9/.github/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-27 16:40:45.953184 scikit_hep_testdata-0.4.9/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (121)     2112 2021-09-27 16:40:29.000000 scikit_hep_testdata-0.4.9/.github/workflows/ci.yml
+-rw-r--r--   0 runner    (1001) docker     (121)     1308 2021-09-27 16:40:29.000000 scikit_hep_testdata-0.4.9/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (121)     1252 2021-09-27 16:40:29.000000 scikit_hep_testdata-0.4.9/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (121)     1511 2021-09-27 16:40:29.000000 scikit_hep_testdata-0.4.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (121)      185 2021-09-27 16:40:29.000000 scikit_hep_testdata-0.4.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (121)     5223 2021-09-27 16:40:45.965185 scikit_hep_testdata-0.4.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     4084 2021-09-27 16:40:29.000000 scikit_hep_testdata-0.4.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-27 16:40:45.949184 scikit_hep_testdata-0.4.9/dev/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-27 16:40:45.957184 scikit_hep_testdata-0.4.9/dev/make-root/
+-rw-r--r--   0 runner    (1001) docker     (121)     5405 2021-09-27 16:40:29.000000 scikit_hep_testdata-0.4.9/dev/make-root/double32_float16.C
+-rw-r--r--   0 runner    (1001) docker     (121)     1153 2021-09-27 16:40:29.000000 scikit_hep_testdata-0.4.9/dev/make-root/rntuple_int_float.C
+-rw-r--r--   0 runner    (1001) docker     (121)     4739 2021-09-27 16:40:29.000000 scikit_hep_testdata-0.4.9/dev/make-root/sample4version.C
+-rw-r--r--   0 runner    (1001) docker     (121)    31229 2021-09-27 16:40:29.000000 scikit_hep_testdata-0.4.9/dev/make-root/stl_containers.C
+-rw-r--r--   0 runner    (1001) docker     (121)      727 2021-09-27 16:40:29.000000 scikit_hep_testdata-0.4.9/dev/make-root/uproot-issue38c.py
+-rw-r--r--   0 runner    (1001) docker     (121)      967 2021-09-27 16:40:29.000000 scikit_hep_testdata-0.4.9/dev/make-root/uproot_issue_407.C
+-rw-r--r--   0 runner    (1001) docker     (121)      203 2021-09-27 16:40:29.000000 scikit_hep_testdata-0.4.9/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (121)     2515 2021-09-27 16:40:45.969185 scikit_hep_testdata-0.4.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)     1046 2021-09-27 16:40:29.000000 scikit_hep_testdata-0.4.9/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-27 16:40:45.949184 scikit_hep_testdata-0.4.9/src/
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-27 16:40:45.961184 scikit_hep_testdata-0.4.9/src/scikit_hep_testdata.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     5223 2021-09-27 16:40:44.000000 scikit_hep_testdata-0.4.9/src/scikit_hep_testdata.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     9663 2021-09-27 16:40:45.000000 scikit_hep_testdata-0.4.9/src/scikit_hep_testdata.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2021-09-27 16:40:44.000000 scikit_hep_testdata-0.4.9/src/scikit_hep_testdata.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      116 2021-09-27 16:40:44.000000 scikit_hep_testdata-0.4.9/src/scikit_hep_testdata.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      165 2021-09-27 16:40:44.000000 scikit_hep_testdata-0.4.9/src/scikit_hep_testdata.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       15 2021-09-27 16:40:44.000000 scikit_hep_testdata-0.4.9/src/scikit_hep_testdata.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2021-09-27 16:40:41.000000 scikit_hep_testdata-0.4.9/src/scikit_hep_testdata.egg-info/zip-safe
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-27 16:40:45.965185 scikit_hep_testdata-0.4.9/src/skhep_testdata/
+-rw-r--r--   0 runner    (1001) docker     (121)      337 2021-09-27 16:40:29.000000 scikit_hep_testdata-0.4.9/src/skhep_testdata/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1170 2021-09-27 16:40:29.000000 scikit_hep_testdata-0.4.9/src/skhep_testdata/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-27 16:40:45.965185 scikit_hep_testdata-0.4.9/src/skhep_testdata/data/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-09-27 16:40:29.000000 scikit_hep_testdata-0.4.9/src/skhep_testdata/data/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4439 2021-09-27 16:40:43.000000 scikit_hep_testdata-0.4.9/src/skhep_testdata/data/file_list.txt
+-rw-r--r--   0 runner    (1001) docker     (121)     2922 2021-09-27 16:40:31.000000 scikit_hep_testdata-0.4.9/src/skhep_testdata/local_files.py
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-09-27 16:40:31.000000 scikit_hep_testdata-0.4.9/src/skhep_testdata/py.typed
+-rw-r--r--   0 runner    (1001) docker     (121)      787 2021-09-27 16:40:31.000000 scikit_hep_testdata-0.4.9/src/skhep_testdata/remote_datasets.yml
+-rw-r--r--   0 runner    (1001) docker     (121)     4042 2021-09-27 16:40:31.000000 scikit_hep_testdata-0.4.9/src/skhep_testdata/remote_files.py
+-rw-r--r--   0 runner    (1001) docker     (121)      142 2021-09-27 16:40:43.000000 scikit_hep_testdata-0.4.9/src/skhep_testdata/version.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-09-27 16:40:45.965185 scikit_hep_testdata-0.4.9/tests/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2021-09-27 16:40:31.000000 scikit_hep_testdata-0.4.9/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1129 2021-09-27 16:40:31.000000 scikit_hep_testdata-0.4.9/tests/test_local_files.py
+-rw-r--r--   0 runner    (1001) docker     (121)      182 2021-09-27 16:40:31.000000 scikit_hep_testdata-0.4.9/tests/test_remote_datasets.yml
+-rw-r--r--   0 runner    (1001) docker     (121)     1401 2021-09-27 16:40:31.000000 scikit_hep_testdata-0.4.9/tests/test_remote_files.py
```

### Comparing `scikit_hep_testdata-0.4.8/.github/workflows/ci.yml` & `scikit_hep_testdata-0.4.9/.github/workflows/ci.yml`

 * *Files identical despite different names*

### Comparing `scikit_hep_testdata-0.4.8/.gitignore` & `scikit_hep_testdata-0.4.9/.gitignore`

 * *Files identical despite different names*

### Comparing `scikit_hep_testdata-0.4.8/.pre-commit-config.yaml` & `scikit_hep_testdata-0.4.9/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `scikit_hep_testdata-0.4.8/LICENSE` & `scikit_hep_testdata-0.4.9/LICENSE`

 * *Files identical despite different names*

### Comparing `scikit_hep_testdata-0.4.8/PKG-INFO` & `scikit_hep_testdata-0.4.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scikit_hep_testdata
-Version: 0.4.8
+Version: 0.4.9
 Summary: Example HEP files for testing and demonstrating
 Home-page: https://github.com/scikit-hep/scikit-hep-testdata
 Author: Ben Krikler
 Author-email: b.krikler@cern.ch
 Maintainer: The Scikit-HEP admins
 Maintainer-email: scikit-hep-admins@googlegroups.com
 License: BSD-3-Clause
```

### Comparing `scikit_hep_testdata-0.4.8/README.md` & `scikit_hep_testdata-0.4.9/README.md`

 * *Files identical despite different names*

### Comparing `scikit_hep_testdata-0.4.8/dev/make-root/double32_float16.C` & `scikit_hep_testdata-0.4.9/dev/make-root/double32_float16.C`

 * *Files identical despite different names*

### Comparing `scikit_hep_testdata-0.4.8/dev/make-root/sample4version.C` & `scikit_hep_testdata-0.4.9/dev/make-root/sample4version.C`

 * *Files identical despite different names*

### Comparing `scikit_hep_testdata-0.4.8/dev/make-root/stl_containers.C` & `scikit_hep_testdata-0.4.9/dev/make-root/stl_containers.C`

 * *Files identical despite different names*

### Comparing `scikit_hep_testdata-0.4.8/dev/make-root/uproot-issue38c.py` & `scikit_hep_testdata-0.4.9/dev/make-root/uproot-issue38c.py`

 * *Files identical despite different names*

### Comparing `scikit_hep_testdata-0.4.8/dev/make-root/uproot_issue_407.C` & `scikit_hep_testdata-0.4.9/dev/make-root/uproot_issue_407.C`

 * *Files identical despite different names*

### Comparing `scikit_hep_testdata-0.4.8/setup.cfg` & `scikit_hep_testdata-0.4.9/setup.cfg`

 * *Files identical despite different names*

### Comparing `scikit_hep_testdata-0.4.8/setup.py` & `scikit_hep_testdata-0.4.9/setup.py`

 * *Files identical despite different names*

### Comparing `scikit_hep_testdata-0.4.8/src/scikit_hep_testdata.egg-info/PKG-INFO` & `scikit_hep_testdata-0.4.9/src/scikit_hep_testdata.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: scikit-hep-testdata
-Version: 0.4.8
+Version: 0.4.9
 Summary: Example HEP files for testing and demonstrating
 Home-page: https://github.com/scikit-hep/scikit-hep-testdata
 Author: Ben Krikler
 Author-email: b.krikler@cern.ch
 Maintainer: The Scikit-HEP admins
 Maintainer-email: scikit-hep-admins@googlegroups.com
 License: BSD-3-Clause
```

### Comparing `scikit_hep_testdata-0.4.8/src/scikit_hep_testdata.egg-info/SOURCES.txt` & `scikit_hep_testdata-0.4.9/src/scikit_hep_testdata.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -4,14 +4,15 @@
 MANIFEST.in
 README.md
 pyproject.toml
 setup.cfg
 setup.py
 .github/workflows/ci.yml
 dev/make-root/double32_float16.C
+dev/make-root/rntuple_int_float.C
 dev/make-root/sample4version.C
 dev/make-root/stl_containers.C
 dev/make-root/uproot-issue38c.py
 dev/make-root/uproot_issue_407.C
 src/scikit_hep_testdata.egg-info/PKG-INFO
 src/scikit_hep_testdata.egg-info/SOURCES.txt
 src/scikit_hep_testdata.egg-info/dependency_links.txt
@@ -27,14 +28,15 @@
 src/skhep_testdata/remote_files.py
 src/skhep_testdata/version.py
 src/skhep_testdata/data/__init__.py
 src/skhep_testdata/data/file_list.txt
 src/skhep_testdata/data/issue367b.root
 src/skhep_testdata/data/pylhe-drell-yan-ll-lhe.gz
 src/skhep_testdata/data/pylhe-testfile-pr29.lhe
+src/skhep_testdata/data/test_ntuple_int_float.root
 src/skhep_testdata/data/uproot-Event.root
 src/skhep_testdata/data/uproot-FCCDelphesOutput.root
 src/skhep_testdata/data/uproot-HZZ-lz4.root
 src/skhep_testdata/data/uproot-HZZ-lzma.root
 src/skhep_testdata/data/uproot-HZZ-objects.root
 src/skhep_testdata/data/uproot-HZZ-uncompressed.root
 src/skhep_testdata/data/uproot-HZZ-zlib.root
```

### Comparing `scikit_hep_testdata-0.4.8/src/skhep_testdata/__main__.py` & `scikit_hep_testdata-0.4.9/src/skhep_testdata/__main__.py`

 * *Files identical despite different names*

### Comparing `scikit_hep_testdata-0.4.8/src/skhep_testdata/data/file_list.txt` & `scikit_hep_testdata-0.4.9/src/skhep_testdata/data/file_list.txt`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,11 @@
 issue367b.root
 pylhe-drell-yan-ll-lhe.gz
 pylhe-testfile-pr29.lhe
+test_ntuple_int_float.root
 uproot-Event.root
 uproot-FCCDelphesOutput.root
 uproot-HZZ-lz4.root
 uproot-HZZ-lzma.root
 uproot-HZZ-objects.root
 uproot-HZZ-uncompressed.root
 uproot-HZZ-zlib.root
```

### Comparing `scikit_hep_testdata-0.4.8/src/skhep_testdata/local_files.py` & `scikit_hep_testdata-0.4.9/src/skhep_testdata/local_files.py`

 * *Files identical despite different names*

### Comparing `scikit_hep_testdata-0.4.8/src/skhep_testdata/remote_datasets.yml` & `scikit_hep_testdata-0.4.9/src/skhep_testdata/remote_datasets.yml`

 * *Files identical despite different names*

### Comparing `scikit_hep_testdata-0.4.8/src/skhep_testdata/remote_files.py` & `scikit_hep_testdata-0.4.9/src/skhep_testdata/remote_files.py`

 * *Files identical despite different names*

### Comparing `scikit_hep_testdata-0.4.8/tests/test_local_files.py` & `scikit_hep_testdata-0.4.9/tests/test_local_files.py`

 * *Files identical despite different names*

### Comparing `scikit_hep_testdata-0.4.8/tests/test_remote_files.py` & `scikit_hep_testdata-0.4.9/tests/test_remote_files.py`

 * *Files identical despite different names*

