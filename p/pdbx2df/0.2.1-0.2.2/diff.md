# Comparing `tmp/pdbx2df-0.2.1.tar.gz` & `tmp/pdbx2df-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pdbx2df-0.2.1.tar", last modified: Fri Jan 27 00:19:27 2023, max compression
+gzip compressed data, was "pdbx2df-0.2.2.tar", last modified: Fri May  5 15:44:05 2023, max compression
```

## Comparing `pdbx2df-0.2.1.tar` & `pdbx2df-0.2.2.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 rliu      (2718) Shen      (2001)        0 2023-01-27 00:19:27.161432 pdbx2df-0.2.1/
--rw-r--r--   0 rliu      (2718) Shen      (2001)     1542 2023-01-06 18:27:27.000000 pdbx2df-0.2.1/.pre-commit-config.yaml
--rw-r--r--   0 rliu      (2718) Shen      (2001)      174 2023-01-04 17:52:02.000000 pdbx2df-0.2.1/.readthedocs.yaml
--rw-r--r--   0 rliu      (2718) Shen      (2001)     1067 2023-01-04 17:51:08.000000 pdbx2df-0.2.1/LICENSE
--rw-r--r--   0 rliu      (2718) Shen      (2001)      348 2023-01-04 18:04:18.000000 pdbx2df-0.2.1/MANIFEST.in
--rw-r--r--   0 rliu      (2718) Shen      (2001)     2332 2023-01-27 00:19:27.161432 pdbx2df-0.2.1/PKG-INFO
--rw-r--r--   0 rliu      (2718) Shen      (2001)     1780 2023-01-06 19:34:13.000000 pdbx2df-0.2.1/README.md
-drwxr-xr-x   0 rliu      (2718) Shen      (2001)        0 2023-01-27 00:19:27.145432 pdbx2df-0.2.1/pdbx2df/
--rw-r--r--   0 rliu      (2718) Shen      (2001)      258 2023-01-06 14:31:26.000000 pdbx2df-0.2.1/pdbx2df/__init__.py
--rw-r--r--   0 rliu      (2718) Shen      (2001)        0 2023-01-05 03:15:10.000000 pdbx2df-0.2.1/pdbx2df/py.typed
--rw-r--r--   0 rliu      (2718) Shen      (2001)     5756 2023-01-27 00:18:48.000000 pdbx2df-0.2.1/pdbx2df/read_pdbx.py
--rw-r--r--   0 rliu      (2718) Shen      (2001)     2212 2023-01-06 19:10:17.000000 pdbx2df-0.2.1/pdbx2df/split_line.py
--rw-r--r--   0 rliu      (2718) Shen      (2001)       22 2023-01-27 00:18:48.000000 pdbx2df-0.2.1/pdbx2df/version.py
-drwxr-xr-x   0 rliu      (2718) Shen      (2001)        0 2023-01-27 00:19:27.145432 pdbx2df-0.2.1/pdbx2df.egg-info/
--rw-r--r--   0 rliu      (2718) Shen      (2001)     2332 2023-01-27 00:19:26.000000 pdbx2df-0.2.1/pdbx2df.egg-info/PKG-INFO
--rw-r--r--   0 rliu      (2718) Shen      (2001)      489 2023-01-27 00:19:26.000000 pdbx2df-0.2.1/pdbx2df.egg-info/SOURCES.txt
--rw-r--r--   0 rliu      (2718) Shen      (2001)        1 2023-01-27 00:19:26.000000 pdbx2df-0.2.1/pdbx2df.egg-info/dependency_links.txt
--rw-r--r--   0 rliu      (2718) Shen      (2001)       61 2023-01-27 00:19:26.000000 pdbx2df-0.2.1/pdbx2df.egg-info/requires.txt
--rw-r--r--   0 rliu      (2718) Shen      (2001)       14 2023-01-27 00:19:26.000000 pdbx2df-0.2.1/pdbx2df.egg-info/top_level.txt
--rw-r--r--   0 rliu      (2718) Shen      (2001)      327 2023-01-06 14:11:27.000000 pdbx2df-0.2.1/pyproject.toml
--rw-r--r--   0 rliu      (2718) Shen      (2001)       12 2023-01-04 18:02:53.000000 pdbx2df-0.2.1/requirements.txt
--rw-r--r--   0 rliu      (2718) Shen      (2001)       38 2023-01-04 17:52:29.000000 pdbx2df-0.2.1/requirements_dev.txt
--rw-r--r--   0 rliu      (2718) Shen      (2001)      240 2023-01-27 00:19:27.161432 pdbx2df-0.2.1/setup.cfg
--rw-r--r--   0 rliu      (2718) Shen      (2001)     1202 2023-01-06 19:37:41.000000 pdbx2df-0.2.1/setup.py
-drwxr-xr-x   0 rliu      (2718) Shen      (2001)        0 2023-01-27 00:19:27.157432 pdbx2df-0.2.1/tests/
--rw-r--r--   0 rliu      (2718) Shen      (2001)        0 2023-01-05 20:19:15.000000 pdbx2df-0.2.1/tests/__init__.py
--rw-r--r--   0 rliu      (2718) Shen      (2001)      304 2023-01-05 20:19:46.000000 pdbx2df-0.2.1/tests/conftest.py
--rw-r--r--   0 rliu      (2718) Shen      (2001)     2038 2023-01-06 19:28:03.000000 pdbx2df-0.2.1/tests/test_read_pdbx.py
--rw-r--r--   0 rliu      (2718) Shen      (2001)     1999 2023-01-06 14:17:27.000000 pdbx2df-0.2.1/tests/test_split_line.py
--rw-r--r--   0 rliu      (2718) Shen      (2001)      306 2023-01-06 18:37:06.000000 pdbx2df-0.2.1/tox.ini
+drwxr-xr-x   0 rliu      (2718) Shen      (2001)        0 2023-05-05 15:44:05.243265 pdbx2df-0.2.2/
+-rw-r--r--   0 rliu      (2718) Shen      (2001)     1542 2023-01-06 18:27:27.000000 pdbx2df-0.2.2/.pre-commit-config.yaml
+-rw-r--r--   0 rliu      (2718) Shen      (2001)      174 2023-01-04 17:52:02.000000 pdbx2df-0.2.2/.readthedocs.yaml
+-rw-r--r--   0 rliu      (2718) Shen      (2001)     1067 2023-01-04 17:51:08.000000 pdbx2df-0.2.2/LICENSE
+-rw-r--r--   0 rliu      (2718) Shen      (2001)      348 2023-01-04 18:04:18.000000 pdbx2df-0.2.2/MANIFEST.in
+-rw-r--r--   0 rliu      (2718) Shen      (2001)     2332 2023-05-05 15:44:05.243265 pdbx2df-0.2.2/PKG-INFO
+-rw-r--r--   0 rliu      (2718) Shen      (2001)     1780 2023-01-06 19:34:13.000000 pdbx2df-0.2.2/README.md
+drwxr-xr-x   0 rliu      (2718) Shen      (2001)        0 2023-05-05 15:44:05.227265 pdbx2df-0.2.2/pdbx2df/
+-rw-r--r--   0 rliu      (2718) Shen      (2001)      258 2023-01-06 14:31:26.000000 pdbx2df-0.2.2/pdbx2df/__init__.py
+-rw-r--r--   0 rliu      (2718) Shen      (2001)        0 2023-01-05 03:15:10.000000 pdbx2df-0.2.2/pdbx2df/py.typed
+-rw-r--r--   0 rliu      (2718) Shen      (2001)     5782 2023-05-05 15:43:14.000000 pdbx2df-0.2.2/pdbx2df/read_pdbx.py
+-rw-r--r--   0 rliu      (2718) Shen      (2001)     2212 2023-01-06 19:10:17.000000 pdbx2df-0.2.2/pdbx2df/split_line.py
+-rw-r--r--   0 rliu      (2718) Shen      (2001)       22 2023-05-05 15:43:14.000000 pdbx2df-0.2.2/pdbx2df/version.py
+drwxr-xr-x   0 rliu      (2718) Shen      (2001)        0 2023-05-05 15:44:05.227265 pdbx2df-0.2.2/pdbx2df.egg-info/
+-rw-r--r--   0 rliu      (2718) Shen      (2001)     2332 2023-05-05 15:44:05.000000 pdbx2df-0.2.2/pdbx2df.egg-info/PKG-INFO
+-rw-r--r--   0 rliu      (2718) Shen      (2001)      489 2023-05-05 15:44:05.000000 pdbx2df-0.2.2/pdbx2df.egg-info/SOURCES.txt
+-rw-r--r--   0 rliu      (2718) Shen      (2001)        1 2023-05-05 15:44:05.000000 pdbx2df-0.2.2/pdbx2df.egg-info/dependency_links.txt
+-rw-r--r--   0 rliu      (2718) Shen      (2001)       61 2023-05-05 15:44:05.000000 pdbx2df-0.2.2/pdbx2df.egg-info/requires.txt
+-rw-r--r--   0 rliu      (2718) Shen      (2001)       14 2023-05-05 15:44:05.000000 pdbx2df-0.2.2/pdbx2df.egg-info/top_level.txt
+-rw-r--r--   0 rliu      (2718) Shen      (2001)      327 2023-01-06 14:11:27.000000 pdbx2df-0.2.2/pyproject.toml
+-rw-r--r--   0 rliu      (2718) Shen      (2001)       12 2023-01-04 18:02:53.000000 pdbx2df-0.2.2/requirements.txt
+-rw-r--r--   0 rliu      (2718) Shen      (2001)       38 2023-01-04 17:52:29.000000 pdbx2df-0.2.2/requirements_dev.txt
+-rw-r--r--   0 rliu      (2718) Shen      (2001)      240 2023-05-05 15:44:05.243265 pdbx2df-0.2.2/setup.cfg
+-rw-r--r--   0 rliu      (2718) Shen      (2001)     1202 2023-01-06 19:37:41.000000 pdbx2df-0.2.2/setup.py
+drwxr-xr-x   0 rliu      (2718) Shen      (2001)        0 2023-05-05 15:44:05.239265 pdbx2df-0.2.2/tests/
+-rw-r--r--   0 rliu      (2718) Shen      (2001)        0 2023-01-05 20:19:15.000000 pdbx2df-0.2.2/tests/__init__.py
+-rw-r--r--   0 rliu      (2718) Shen      (2001)      304 2023-01-05 20:19:46.000000 pdbx2df-0.2.2/tests/conftest.py
+-rw-r--r--   0 rliu      (2718) Shen      (2001)     2038 2023-01-06 19:28:03.000000 pdbx2df-0.2.2/tests/test_read_pdbx.py
+-rw-r--r--   0 rliu      (2718) Shen      (2001)     1999 2023-01-06 14:17:27.000000 pdbx2df-0.2.2/tests/test_split_line.py
+-rw-r--r--   0 rliu      (2718) Shen      (2001)      306 2023-01-06 18:37:06.000000 pdbx2df-0.2.2/tox.ini
```

### Comparing `pdbx2df-0.2.1/.pre-commit-config.yaml` & `pdbx2df-0.2.2/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `pdbx2df-0.2.1/LICENSE` & `pdbx2df-0.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `pdbx2df-0.2.1/PKG-INFO` & `pdbx2df-0.2.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pdbx2df
-Version: 0.2.1
+Version: 0.2.2
 Summary: A python package to parse PDBx file into Pandas DataFrames.
 Home-page: https://github.com/Ruibin-Liu/pdbx2df
 Author: Ruibin Liu
 Author-email: ruibinliuphd@gmail.com
 Project-URL: Bug Tracker, https://github.com/Ruibin-Liu/pdbx2df/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `pdbx2df-0.2.1/README.md` & `pdbx2df-0.2.2/README.md`

 * *Files identical despite different names*

### Comparing `pdbx2df-0.2.1/pdbx2df/read_pdbx.py` & `pdbx2df-0.2.2/pdbx2df/read_pdbx.py`

 * *Files 2% similar despite different names*

```diff
@@ -35,15 +35,15 @@
                     break
                 if line == "loop_\n":
                     loop_category = True
                     line = pf.readline()
                 in_multiple_line = (
                     False  # lines quoted by ';', they need to be specially treated
                 )
-                while line[0] != "#":
+                while line.strip() not in ["#", "#   #", "##"]:
                     if line[0] == "_" and not in_multiple_line:
                         category_name, category_nth_col = (
                             line.strip().split(" ")[0].split(".")
                         )
                         category_cols.append(category_nth_col)
                     if (
                         category_name in category_names or "all" in category_names
```

### Comparing `pdbx2df-0.2.1/pdbx2df/split_line.py` & `pdbx2df-0.2.2/pdbx2df/split_line.py`

 * *Files identical despite different names*

### Comparing `pdbx2df-0.2.1/pdbx2df.egg-info/PKG-INFO` & `pdbx2df-0.2.2/pdbx2df.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pdbx2df
-Version: 0.2.1
+Version: 0.2.2
 Summary: A python package to parse PDBx file into Pandas DataFrames.
 Home-page: https://github.com/Ruibin-Liu/pdbx2df
 Author: Ruibin Liu
 Author-email: ruibinliuphd@gmail.com
 Project-URL: Bug Tracker, https://github.com/Ruibin-Liu/pdbx2df/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `pdbx2df-0.2.1/setup.py` & `pdbx2df-0.2.2/setup.py`

 * *Files identical despite different names*

### Comparing `pdbx2df-0.2.1/tests/test_read_pdbx.py` & `pdbx2df-0.2.2/tests/test_read_pdbx.py`

 * *Files identical despite different names*

### Comparing `pdbx2df-0.2.1/tests/test_split_line.py` & `pdbx2df-0.2.2/tests/test_split_line.py`

 * *Files identical despite different names*

