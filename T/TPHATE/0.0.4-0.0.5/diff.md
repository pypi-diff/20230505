# Comparing `tmp/TPHATE-0.0.4.tar.gz` & `tmp/TPHATE-0.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/Users/elb/Library/CloudStorage/GoogleDrive-erica.busch@yale.edu/My Drive/DriveLocal/Projects/NTB/poetry/TPHATE/dist/.tmp-d7vwj", last modified: Wed May  3 18:01:52 2023, max compression
+gzip compressed data, was "/Users/elb/Library/CloudStorage/GoogleDrive-erica.busch@yale.edu/My Drive/DriveLocal/Projects/NTB/poetry/TPHATE/dist/.tmp-7lore", last modified: Fri May  5 18:12:09 2023, max compression
```

## Comparing `TPHATE-0.0.4.tar` & `TPHATE-0.0.5.tar`

### file list

```diff
@@ -1,25 +1,16 @@
-drwxr-xr-x   0 elb        (501) staff       (20)        0 2023-05-03 18:01:52.984699 TPHATE-0.0.4/
--rw-r--r--   0 elb        (501) staff       (20)    35149 2023-04-25 23:34:37.000000 TPHATE-0.0.4/LICENSE
--rw-r--r--   0 elb        (501) staff       (20)     1785 2023-05-03 18:01:52.984367 TPHATE-0.0.4/PKG-INFO
--rw-r--r--   0 elb        (501) staff       (20)     1153 2023-05-03 17:57:42.000000 TPHATE-0.0.4/README.md
--rw-r--r--   0 elb        (501) staff       (20)      952 2023-05-03 18:01:21.000000 TPHATE-0.0.4/pyproject.toml
--rw-r--r--   0 elb        (501) staff       (20)       38 2023-05-03 18:01:52.984802 TPHATE-0.0.4/setup.cfg
-drwxr-xr-x   0 elb        (501) staff       (20)        0 2023-05-03 18:01:52.970800 TPHATE-0.0.4/src/
-drwxr-xr-x   0 elb        (501) staff       (20)        0 2023-05-03 18:01:52.974988 TPHATE-0.0.4/src/TPHATE.egg-info/
--rw-r--r--   0 elb        (501) staff       (20)     1785 2023-05-03 18:01:52.000000 TPHATE-0.0.4/src/TPHATE.egg-info/PKG-INFO
--rw-r--r--   0 elb        (501) staff       (20)      390 2023-05-03 18:01:52.000000 TPHATE-0.0.4/src/TPHATE.egg-info/SOURCES.txt
--rw-r--r--   0 elb        (501) staff       (20)        1 2023-05-03 18:01:52.000000 TPHATE-0.0.4/src/TPHATE.egg-info/dependency_links.txt
--rw-r--r--   0 elb        (501) staff       (20)        7 2023-05-03 18:01:52.000000 TPHATE-0.0.4/src/TPHATE.egg-info/top_level.txt
-drwxr-xr-x   0 elb        (501) staff       (20)        0 2023-05-03 18:01:52.982926 TPHATE-0.0.4/src/tphate/
--rw-r--r--   0 elb        (501) staff       (20)       59 2023-04-26 18:31:46.000000 TPHATE-0.0.4/src/tphate/__init__.py
--rw-r--r--   0 elb        (501) staff       (20)    11774 2023-04-25 23:34:38.000000 TPHATE-0.0.4/src/tphate/api.py
--rw-r--r--   0 elb        (501) staff       (20)    41142 2023-04-25 23:34:38.000000 TPHATE-0.0.4/src/tphate/base.py
--rw-r--r--   0 elb        (501) staff       (20)    54724 2023-04-25 23:34:38.000000 TPHATE-0.0.4/src/tphate/graphs.py
--rw-r--r--   0 elb        (501) staff       (20)     2090 2023-04-25 23:34:38.000000 TPHATE-0.0.4/src/tphate/matrix.py
--rw-r--r--   0 elb        (501) staff       (20)     7430 2023-04-25 23:34:38.000000 TPHATE-0.0.4/src/tphate/mds.py
--rw-r--r--   0 elb        (501) staff       (20)    37913 2023-04-25 23:34:38.000000 TPHATE-0.0.4/src/tphate/tphate.py
--rw-r--r--   0 elb        (501) staff       (20)     9569 2023-04-25 23:34:38.000000 TPHATE-0.0.4/src/tphate/utils.py
--rw-r--r--   0 elb        (501) staff       (20)       21 2023-04-26 18:29:27.000000 TPHATE-0.0.4/src/tphate/version.py
--rw-r--r--   0 elb        (501) staff       (20)     3966 2023-04-25 23:34:38.000000 TPHATE-0.0.4/src/tphate/vne.py
-drwxr-xr-x   0 elb        (501) staff       (20)        0 2023-05-03 18:01:52.983384 TPHATE-0.0.4/tests/
--rw-r--r--   0 elb        (501) staff       (20)       83 2023-04-25 23:37:03.000000 TPHATE-0.0.4/tests/test_tphate.py
+drwxr-xr-x   0 elb        (501) staff       (20)        0 2023-05-05 18:12:09.120682 TPHATE-0.0.5/
+-rw-r--r--   0 elb        (501) staff       (20)    35149 2023-04-25 23:34:37.000000 TPHATE-0.0.5/LICENSE
+-rw-r--r--   0 elb        (501) staff       (20)     1785 2023-05-05 18:12:09.120890 TPHATE-0.0.5/PKG-INFO
+-rw-r--r--   0 elb        (501) staff       (20)     1153 2023-05-03 17:57:42.000000 TPHATE-0.0.5/README.md
+drwxr-xr-x   0 elb        (501) staff       (20)        0 2023-05-05 18:12:09.119418 TPHATE-0.0.5/TPHATE.egg-info/
+-rw-r--r--   0 elb        (501) staff       (20)     1785 2023-05-05 18:12:09.000000 TPHATE-0.0.5/TPHATE.egg-info/PKG-INFO
+-rw-r--r--   0 elb        (501) staff       (20)      239 2023-05-05 18:12:09.000000 TPHATE-0.0.5/TPHATE.egg-info/SOURCES.txt
+-rw-r--r--   0 elb        (501) staff       (20)        1 2023-05-05 18:12:09.000000 TPHATE-0.0.5/TPHATE.egg-info/dependency_links.txt
+-rw-r--r--   0 elb        (501) staff       (20)      198 2023-05-05 18:12:09.000000 TPHATE-0.0.5/TPHATE.egg-info/requires.txt
+-rw-r--r--   0 elb        (501) staff       (20)        6 2023-05-05 18:12:09.000000 TPHATE-0.0.5/TPHATE.egg-info/top_level.txt
+-rw-r--r--   0 elb        (501) staff       (20)     1283 2023-05-05 18:11:09.000000 TPHATE-0.0.5/pyproject.toml
+-rw-r--r--   0 elb        (501) staff       (20)      272 2023-05-05 18:12:09.121441 TPHATE-0.0.5/setup.cfg
+-rw-r--r--   0 elb        (501) staff       (20)     2354 2023-05-05 18:07:51.000000 TPHATE-0.0.5/setup.py
+drwxr-xr-x   0 elb        (501) staff       (20)        0 2023-05-05 18:12:09.120344 TPHATE-0.0.5/tests/
+-rw-r--r--   0 elb        (501) staff       (20)        0 2023-04-25 23:37:03.000000 TPHATE-0.0.5/tests/__init__.py
+-rw-r--r--   0 elb        (501) staff       (20)       83 2023-04-25 23:37:03.000000 TPHATE-0.0.5/tests/test_tphate.py
```

### Comparing `TPHATE-0.0.4/LICENSE` & `TPHATE-0.0.5/LICENSE`

 * *Files identical despite different names*

### Comparing `TPHATE-0.0.4/PKG-INFO` & `TPHATE-0.0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: TPHATE
-Version: 0.0.4
+Version: 0.0.5
 Summary: Temporal PHATE (TPHATE) is a python package for learning robust manifold representations of timeseries data with high temporal autocorrelation.
 Author-email: Erica Busch <ericalindseybusch@gmail.com>
 Project-URL: Homepage, https://github.com/KrishnaswamyLab/TPHATE/
 Project-URL: Bug Tracker, https://github.com/KrishnaswamyLab/TPHATE/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `TPHATE-0.0.4/README.md` & `TPHATE-0.0.5/README.md`

 * *Files identical despite different names*

### Comparing `TPHATE-0.0.4/src/TPHATE.egg-info/PKG-INFO` & `TPHATE-0.0.5/TPHATE.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: TPHATE
-Version: 0.0.4
+Version: 0.0.5
 Summary: Temporal PHATE (TPHATE) is a python package for learning robust manifold representations of timeseries data with high temporal autocorrelation.
 Author-email: Erica Busch <ericalindseybusch@gmail.com>
 Project-URL: Homepage, https://github.com/KrishnaswamyLab/TPHATE/
 Project-URL: Bug Tracker, https://github.com/KrishnaswamyLab/TPHATE/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

