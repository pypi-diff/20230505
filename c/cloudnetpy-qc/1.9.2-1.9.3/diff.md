# Comparing `tmp/cloudnetpy_qc-1.9.2.tar.gz` & `tmp/cloudnetpy_qc-1.9.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cloudnetpy_qc-1.9.2.tar", last modified: Thu May  4 14:53:04 2023, max compression
+gzip compressed data, was "cloudnetpy_qc-1.9.3.tar", last modified: Fri May  5 09:51:39 2023, max compression
```

## Comparing `cloudnetpy_qc-1.9.2.tar` & `cloudnetpy_qc-1.9.3.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 14:53:04.550412 cloudnetpy_qc-1.9.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1094 2023-05-04 14:52:53.000000 cloudnetpy_qc-1.9.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-05-04 14:52:53.000000 cloudnetpy_qc-1.9.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2044 2023-05-04 14:53:04.550412 cloudnetpy_qc-1.9.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1368 2023-05-04 14:52:53.000000 cloudnetpy_qc-1.9.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 14:53:04.542412 cloudnetpy_qc-1.9.2/cloudnetpy_qc/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 14:52:53.000000 cloudnetpy_qc-1.9.2/cloudnetpy_qc/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 14:53:04.546412 cloudnetpy_qc-1.9.2/cloudnetpy_qc/data/
--rw-r--r--   0 runner    (1001) docker     (123)    14435 2023-05-04 14:52:53.000000 cloudnetpy_qc-1.9.2/cloudnetpy_qc/data/area-type-table.xml
--rw-r--r--   0 runner    (1001) docker     (123)  4094783 2023-05-04 14:52:53.000000 cloudnetpy_qc-1.9.2/cloudnetpy_qc/data/cf-standard-name-table.xml
--rw-r--r--   0 runner    (1001) docker     (123)     1118 2023-05-04 14:52:53.000000 cloudnetpy_qc-1.9.2/cloudnetpy_qc/data/data_quality_config.ini
--rw-r--r--   0 runner    (1001) docker     (123)      169 2023-05-04 14:52:53.000000 cloudnetpy_qc-1.9.2/cloudnetpy_qc/data/metadata_config.ini
--rw-r--r--   0 runner    (1001) docker     (123)     6274 2023-05-04 14:52:53.000000 cloudnetpy_qc-1.9.2/cloudnetpy_qc/data/standardized-region-list.xml
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 14:52:53.000000 cloudnetpy_qc-1.9.2/cloudnetpy_qc/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    15829 2023-05-04 14:52:53.000000 cloudnetpy_qc-1.9.2/cloudnetpy_qc/quality.py
--rw-r--r--   0 runner    (1001) docker     (123)     1195 2023-05-04 14:52:53.000000 cloudnetpy_qc-1.9.2/cloudnetpy_qc/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    30074 2023-05-04 14:52:53.000000 cloudnetpy_qc-1.9.2/cloudnetpy_qc/variables.py
--rw-r--r--   0 runner    (1001) docker     (123)      100 2023-05-04 14:52:53.000000 cloudnetpy_qc-1.9.2/cloudnetpy_qc/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 14:53:04.542412 cloudnetpy_qc-1.9.2/cloudnetpy_qc.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2044 2023-05-04 14:53:04.000000 cloudnetpy_qc-1.9.2/cloudnetpy_qc.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      586 2023-05-04 14:53:04.000000 cloudnetpy_qc-1.9.2/cloudnetpy_qc.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-04 14:53:04.000000 cloudnetpy_qc-1.9.2/cloudnetpy_qc.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-05-04 14:53:04.000000 cloudnetpy_qc-1.9.2/cloudnetpy_qc.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-04 14:53:04.000000 cloudnetpy_qc-1.9.2/cloudnetpy_qc.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-04 14:53:04.550412 cloudnetpy_qc-1.9.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1347 2023-05-04 14:52:53.000000 cloudnetpy_qc-1.9.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 09:51:39.739992 cloudnetpy_qc-1.9.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1094 2023-05-05 09:51:21.000000 cloudnetpy_qc-1.9.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-05-05 09:51:21.000000 cloudnetpy_qc-1.9.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2044 2023-05-05 09:51:39.739992 cloudnetpy_qc-1.9.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1368 2023-05-05 09:51:21.000000 cloudnetpy_qc-1.9.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 09:51:39.731991 cloudnetpy_qc-1.9.3/cloudnetpy_qc/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 09:51:21.000000 cloudnetpy_qc-1.9.3/cloudnetpy_qc/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 09:51:39.739992 cloudnetpy_qc-1.9.3/cloudnetpy_qc/data/
+-rw-r--r--   0 runner    (1001) docker     (123)    14435 2023-05-05 09:51:21.000000 cloudnetpy_qc-1.9.3/cloudnetpy_qc/data/area-type-table.xml
+-rw-r--r--   0 runner    (1001) docker     (123)  4094783 2023-05-05 09:51:21.000000 cloudnetpy_qc-1.9.3/cloudnetpy_qc/data/cf-standard-name-table.xml
+-rw-r--r--   0 runner    (1001) docker     (123)     1118 2023-05-05 09:51:21.000000 cloudnetpy_qc-1.9.3/cloudnetpy_qc/data/data_quality_config.ini
+-rw-r--r--   0 runner    (1001) docker     (123)      169 2023-05-05 09:51:21.000000 cloudnetpy_qc-1.9.3/cloudnetpy_qc/data/metadata_config.ini
+-rw-r--r--   0 runner    (1001) docker     (123)     6274 2023-05-05 09:51:21.000000 cloudnetpy_qc-1.9.3/cloudnetpy_qc/data/standardized-region-list.xml
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 09:51:21.000000 cloudnetpy_qc-1.9.3/cloudnetpy_qc/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    15829 2023-05-05 09:51:21.000000 cloudnetpy_qc-1.9.3/cloudnetpy_qc/quality.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1195 2023-05-05 09:51:21.000000 cloudnetpy_qc-1.9.3/cloudnetpy_qc/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30120 2023-05-05 09:51:21.000000 cloudnetpy_qc-1.9.3/cloudnetpy_qc/variables.py
+-rw-r--r--   0 runner    (1001) docker     (123)      100 2023-05-05 09:51:21.000000 cloudnetpy_qc-1.9.3/cloudnetpy_qc/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 09:51:39.731991 cloudnetpy_qc-1.9.3/cloudnetpy_qc.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2044 2023-05-05 09:51:39.000000 cloudnetpy_qc-1.9.3/cloudnetpy_qc.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      586 2023-05-05 09:51:39.000000 cloudnetpy_qc-1.9.3/cloudnetpy_qc.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 09:51:39.000000 cloudnetpy_qc-1.9.3/cloudnetpy_qc.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-05-05 09:51:39.000000 cloudnetpy_qc-1.9.3/cloudnetpy_qc.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-05-05 09:51:39.000000 cloudnetpy_qc-1.9.3/cloudnetpy_qc.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-05 09:51:39.739992 cloudnetpy_qc-1.9.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1347 2023-05-05 09:51:21.000000 cloudnetpy_qc-1.9.3/setup.py
```

### Comparing `cloudnetpy_qc-1.9.2/LICENSE` & `cloudnetpy_qc-1.9.3/LICENSE`

 * *Files identical despite different names*

### Comparing `cloudnetpy_qc-1.9.2/PKG-INFO` & `cloudnetpy_qc-1.9.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cloudnetpy_qc
-Version: 1.9.2
+Version: 1.9.3
 Summary: Quality control routines for CloudnetPy products
 Home-page: https://github.com/actris-cloudnet/cloudnetpy-qc
 Author: Finnish Meteorological Institute
 Author-email: actris-cloudnet@fmi.fi
 License: MIT License
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

### Comparing `cloudnetpy_qc-1.9.2/README.md` & `cloudnetpy_qc-1.9.3/README.md`

 * *Files identical despite different names*

### Comparing `cloudnetpy_qc-1.9.2/cloudnetpy_qc/data/area-type-table.xml` & `cloudnetpy_qc-1.9.3/cloudnetpy_qc/data/area-type-table.xml`

 * *Files identical despite different names*

### Comparing `cloudnetpy_qc-1.9.2/cloudnetpy_qc/data/cf-standard-name-table.xml` & `cloudnetpy_qc-1.9.3/cloudnetpy_qc/data/cf-standard-name-table.xml`

 * *Files identical despite different names*

### Comparing `cloudnetpy_qc-1.9.2/cloudnetpy_qc/data/data_quality_config.ini` & `cloudnetpy_qc-1.9.3/cloudnetpy_qc/data/data_quality_config.ini`

 * *Files identical despite different names*

### Comparing `cloudnetpy_qc-1.9.2/cloudnetpy_qc/data/standardized-region-list.xml` & `cloudnetpy_qc-1.9.3/cloudnetpy_qc/data/standardized-region-list.xml`

 * *Files identical despite different names*

### Comparing `cloudnetpy_qc-1.9.2/cloudnetpy_qc/quality.py` & `cloudnetpy_qc-1.9.3/cloudnetpy_qc/quality.py`

 * *Files identical despite different names*

### Comparing `cloudnetpy_qc-1.9.2/cloudnetpy_qc/utils.py` & `cloudnetpy_qc-1.9.3/cloudnetpy_qc/utils.py`

 * *Files identical despite different names*

### Comparing `cloudnetpy_qc-1.9.2/cloudnetpy_qc/variables.py` & `cloudnetpy_qc-1.9.3/cloudnetpy_qc/variables.py`

 * *Files 0% similar despite different names*

```diff
@@ -475,14 +475,16 @@
     ),
     "number_concentration": Variable(
         long_name="Number of particles per diameter class", units="m-3 mm-1"
     ),
     "fall_velocity": Variable(long_name="Average velocity of each diameter class", units="m s-1"),
     "data_raw": Variable(
         long_name="Raw data as a function of particle diameter and velocity",
+        units="1",
+        dtype=Dtype.SHORT,
     ),
     "phi_cx": Variable(
         long_name="Co-cross-channel differential phase",
         units="rad",
     ),
     "rho_cx": Variable(
         long_name="Co-cross-channel correlation coefficient",
```

### Comparing `cloudnetpy_qc-1.9.2/cloudnetpy_qc.egg-info/PKG-INFO` & `cloudnetpy_qc-1.9.3/cloudnetpy_qc.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cloudnetpy-qc
-Version: 1.9.2
+Version: 1.9.3
 Summary: Quality control routines for CloudnetPy products
 Home-page: https://github.com/actris-cloudnet/cloudnetpy-qc
 Author: Finnish Meteorological Institute
 Author-email: actris-cloudnet@fmi.fi
 License: MIT License
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

### Comparing `cloudnetpy_qc-1.9.2/cloudnetpy_qc.egg-info/SOURCES.txt` & `cloudnetpy_qc-1.9.3/cloudnetpy_qc.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cloudnetpy_qc-1.9.2/setup.py` & `cloudnetpy_qc-1.9.3/setup.py`

 * *Files identical despite different names*

