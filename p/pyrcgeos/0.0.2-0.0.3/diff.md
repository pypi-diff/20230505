# Comparing `tmp/pyrcgeos-0.0.2.tar.gz` & `tmp/pyrcgeos-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyrcgeos-0.0.2.tar", last modified: Mon Mar 20 15:50:03 2023, max compression
+gzip compressed data, was "pyrcgeos-0.0.3.tar", last modified: Fri May  5 14:43:41 2023, max compression
```

## Comparing `pyrcgeos-0.0.2.tar` & `pyrcgeos-0.0.3.tar`

### file list

```diff
@@ -1,17 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-20 15:50:03.796321 pyrcgeos-0.0.2/
--rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-03-20 15:49:54.000000 pyrcgeos-0.0.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      122 2023-03-20 15:49:54.000000 pyrcgeos-0.0.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1328 2023-03-20 15:50:03.796321 pyrcgeos-0.0.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      567 2023-03-20 15:49:54.000000 pyrcgeos-0.0.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-20 15:50:03.796321 pyrcgeos-0.0.2/pyrcgeos/
--rw-r--r--   0 runner    (1001) docker     (123)      126 2023-03-20 15:49:54.000000 pyrcgeos-0.0.2/pyrcgeos/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-03-20 15:49:54.000000 pyrcgeos-0.0.2/pyrcgeos/pyrcgeos.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-20 15:50:03.796321 pyrcgeos-0.0.2/pyrcgeos.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1328 2023-03-20 15:50:03.000000 pyrcgeos-0.0.2/pyrcgeos.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      266 2023-03-20 15:50:03.000000 pyrcgeos-0.0.2/pyrcgeos.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-20 15:50:03.000000 pyrcgeos-0.0.2/pyrcgeos.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-20 15:50:03.000000 pyrcgeos-0.0.2/pyrcgeos.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-03-20 15:50:03.000000 pyrcgeos-0.0.2/pyrcgeos.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-20 15:49:54.000000 pyrcgeos-0.0.2/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      391 2023-03-20 15:50:03.796321 pyrcgeos-0.0.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1741 2023-03-20 15:49:54.000000 pyrcgeos-0.0.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 14:43:41.895940 pyrcgeos-0.0.3/
+-rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-05-05 14:43:25.000000 pyrcgeos-0.0.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      122 2023-05-05 14:43:25.000000 pyrcgeos-0.0.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1328 2023-05-05 14:43:41.895940 pyrcgeos-0.0.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      567 2023-05-05 14:43:25.000000 pyrcgeos-0.0.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 14:43:41.891940 pyrcgeos-0.0.3/pyrcgeos/
+-rw-r--r--   0 runner    (1001) docker     (123)      150 2023-05-05 14:43:25.000000 pyrcgeos-0.0.3/pyrcgeos/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      139 2023-05-05 14:43:25.000000 pyrcgeos-0.0.3/pyrcgeos/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2840 2023-05-05 14:43:25.000000 pyrcgeos-0.0.3/pyrcgeos/foliumap.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10830 2023-05-05 14:43:25.000000 pyrcgeos-0.0.3/pyrcgeos/pyrcgeos.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 14:43:41.895940 pyrcgeos-0.0.3/pyrcgeos.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1328 2023-05-05 14:43:41.000000 pyrcgeos-0.0.3/pyrcgeos.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      337 2023-05-05 14:43:41.000000 pyrcgeos-0.0.3/pyrcgeos.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-05-05 14:43:41.000000 pyrcgeos-0.0.3/pyrcgeos.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 14:43:41.000000 pyrcgeos-0.0.3/pyrcgeos.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-05-05 14:43:41.000000 pyrcgeos-0.0.3/pyrcgeos.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-05-05 14:43:41.000000 pyrcgeos-0.0.3/pyrcgeos.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       72 2023-05-05 14:43:25.000000 pyrcgeos-0.0.3/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      391 2023-05-05 14:43:41.895940 pyrcgeos-0.0.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1741 2023-05-05 14:43:25.000000 pyrcgeos-0.0.3/setup.py
```

### Comparing `pyrcgeos-0.0.2/LICENSE` & `pyrcgeos-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pyrcgeos-0.0.2/PKG-INFO` & `pyrcgeos-0.0.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyrcgeos
-Version: 0.0.2
+Version: 0.0.3
 Summary: A python package for interactive mapping.
 Home-page: https://github.com/rcgeos/pyrcgeos
 Author: rcgeos
 Author-email: renato.cumani4@gmail.com
 License: MIT license
 Keywords: pyrcgeos
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `pyrcgeos-0.0.2/README.md` & `pyrcgeos-0.0.3/README.md`

 * *Files identical despite different names*

### Comparing `pyrcgeos-0.0.2/pyrcgeos.egg-info/PKG-INFO` & `pyrcgeos-0.0.3/pyrcgeos.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyrcgeos
-Version: 0.0.2
+Version: 0.0.3
 Summary: A python package for interactive mapping.
 Home-page: https://github.com/rcgeos/pyrcgeos
 Author: rcgeos
 Author-email: renato.cumani4@gmail.com
 License: MIT license
 Keywords: pyrcgeos
 Classifier: Development Status :: 2 - Pre-Alpha
```

### Comparing `pyrcgeos-0.0.2/setup.py` & `pyrcgeos-0.0.3/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -49,10 +49,10 @@
     keywords='pyrcgeos',
     name='pyrcgeos',
     packages=find_packages(include=['pyrcgeos', 'pyrcgeos.*']),
     setup_requires=setup_requirements,
     test_suite='tests',
     tests_require=test_requirements,
     url='https://github.com/rcgeos/pyrcgeos',
-    version='0.0.2',
+    version='0.0.3',
     zip_safe=False,
 )
```

