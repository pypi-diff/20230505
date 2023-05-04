# Comparing `tmp/airflow-kdb-provider-0.1.2.tar.gz` & `tmp/airflow-kdb-provider-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/airflow-kdb-provider-0.1.2.tar", last modified: Wed May  3 06:53:14 2023, max compression
+gzip compressed data, was "dist/airflow-kdb-provider-0.1.3.tar", last modified: Thu May  4 17:47:53 2023, max compression
```

## Comparing `airflow-kdb-provider-0.1.2.tar` & `airflow-kdb-provider-0.1.3.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxr-xr-x   0 kabir      (501) staff       (20)        0 2023-05-03 06:53:14.474964 airflow-kdb-provider-0.1.2/
--rw-r--r--   0 kabir      (501) staff       (20)    11358 2023-05-03 00:16:45.000000 airflow-kdb-provider-0.1.2/LICENSE
--rw-r--r--   0 kabir      (501) staff       (20)     2437 2023-05-03 06:53:14.474774 airflow-kdb-provider-0.1.2/PKG-INFO
--rw-r--r--   0 kabir      (501) staff       (20)     1634 2023-05-03 06:52:57.000000 airflow-kdb-provider-0.1.2/README.md
-drwxr-xr-x   0 kabir      (501) staff       (20)        0 2023-05-03 06:53:14.472732 airflow-kdb-provider-0.1.2/airflow_kdb_provider/
--rw-r--r--   0 kabir      (501) staff       (20)        0 2023-05-03 00:07:52.000000 airflow-kdb-provider-0.1.2/airflow_kdb_provider/__init__.py
-drwxr-xr-x   0 kabir      (501) staff       (20)        0 2023-05-03 06:53:14.474185 airflow-kdb-provider-0.1.2/airflow_kdb_provider/operators/
--rw-r--r--   0 kabir      (501) staff       (20)        0 2023-05-03 00:08:28.000000 airflow-kdb-provider-0.1.2/airflow_kdb_provider/operators/__init__.py
--rw-r--r--   0 kabir      (501) staff       (20)      869 2023-05-03 00:10:53.000000 airflow-kdb-provider-0.1.2/airflow_kdb_provider/operators/kdb_operator.py
-drwxr-xr-x   0 kabir      (501) staff       (20)        0 2023-05-03 06:53:14.473813 airflow-kdb-provider-0.1.2/airflow_kdb_provider.egg-info/
--rw-r--r--   0 kabir      (501) staff       (20)     2437 2023-05-03 06:53:14.000000 airflow-kdb-provider-0.1.2/airflow_kdb_provider.egg-info/PKG-INFO
--rw-r--r--   0 kabir      (501) staff       (20)      368 2023-05-03 06:53:14.000000 airflow-kdb-provider-0.1.2/airflow_kdb_provider.egg-info/SOURCES.txt
--rw-r--r--   0 kabir      (501) staff       (20)        1 2023-05-03 06:53:14.000000 airflow-kdb-provider-0.1.2/airflow_kdb_provider.egg-info/dependency_links.txt
--rw-r--r--   0 kabir      (501) staff       (20)       22 2023-05-03 06:53:14.000000 airflow-kdb-provider-0.1.2/airflow_kdb_provider.egg-info/requires.txt
--rw-r--r--   0 kabir      (501) staff       (20)       21 2023-05-03 06:53:14.000000 airflow-kdb-provider-0.1.2/airflow_kdb_provider.egg-info/top_level.txt
--rw-r--r--   0 kabir      (501) staff       (20)       38 2023-05-03 06:53:14.475026 airflow-kdb-provider-0.1.2/setup.cfg
--rw-r--r--   0 kabir      (501) staff       (20)      800 2023-05-03 06:53:08.000000 airflow-kdb-provider-0.1.2/setup.py
+drwxr-xr-x   0 kabir      (501) staff       (20)        0 2023-05-04 17:47:53.307213 airflow-kdb-provider-0.1.3/
+-rw-r--r--   0 kabir      (501) staff       (20)    11358 2023-05-03 00:16:45.000000 airflow-kdb-provider-0.1.3/LICENSE
+-rw-r--r--   0 kabir      (501) staff       (20)     2437 2023-05-04 17:47:53.306801 airflow-kdb-provider-0.1.3/PKG-INFO
+-rw-r--r--   0 kabir      (501) staff       (20)     1634 2023-05-03 06:52:57.000000 airflow-kdb-provider-0.1.3/README.md
+drwxr-xr-x   0 kabir      (501) staff       (20)        0 2023-05-04 17:47:53.304378 airflow-kdb-provider-0.1.3/airflow_kdb_provider/
+-rw-r--r--   0 kabir      (501) staff       (20)        0 2023-05-03 00:07:52.000000 airflow-kdb-provider-0.1.3/airflow_kdb_provider/__init__.py
+drwxr-xr-x   0 kabir      (501) staff       (20)        0 2023-05-04 17:47:53.306223 airflow-kdb-provider-0.1.3/airflow_kdb_provider/operators/
+-rw-r--r--   0 kabir      (501) staff       (20)        0 2023-05-03 00:08:28.000000 airflow-kdb-provider-0.1.3/airflow_kdb_provider/operators/__init__.py
+-rw-r--r--   0 kabir      (501) staff       (20)     1611 2023-05-03 20:01:22.000000 airflow-kdb-provider-0.1.3/airflow_kdb_provider/operators/kdb_operator.py
+drwxr-xr-x   0 kabir      (501) staff       (20)        0 2023-05-04 17:47:53.305803 airflow-kdb-provider-0.1.3/airflow_kdb_provider.egg-info/
+-rw-r--r--   0 kabir      (501) staff       (20)     2437 2023-05-04 17:47:53.000000 airflow-kdb-provider-0.1.3/airflow_kdb_provider.egg-info/PKG-INFO
+-rw-r--r--   0 kabir      (501) staff       (20)      368 2023-05-04 17:47:53.000000 airflow-kdb-provider-0.1.3/airflow_kdb_provider.egg-info/SOURCES.txt
+-rw-r--r--   0 kabir      (501) staff       (20)        1 2023-05-04 17:47:53.000000 airflow-kdb-provider-0.1.3/airflow_kdb_provider.egg-info/dependency_links.txt
+-rw-r--r--   0 kabir      (501) staff       (20)       22 2023-05-04 17:47:53.000000 airflow-kdb-provider-0.1.3/airflow_kdb_provider.egg-info/requires.txt
+-rw-r--r--   0 kabir      (501) staff       (20)       21 2023-05-04 17:47:53.000000 airflow-kdb-provider-0.1.3/airflow_kdb_provider.egg-info/top_level.txt
+-rw-r--r--   0 kabir      (501) staff       (20)       38 2023-05-04 17:47:53.307293 airflow-kdb-provider-0.1.3/setup.cfg
+-rw-r--r--   0 kabir      (501) staff       (20)      800 2023-05-04 17:41:17.000000 airflow-kdb-provider-0.1.3/setup.py
```

### Comparing `airflow-kdb-provider-0.1.2/LICENSE` & `airflow-kdb-provider-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `airflow-kdb-provider-0.1.2/PKG-INFO` & `airflow-kdb-provider-0.1.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: airflow-kdb-provider
-Version: 0.1.2
+Version: 0.1.3
 Summary: Apache Airflow provider for KDBAirflowOperator
 Home-page: UNKNOWN
 Author: Kabir Jaiswal
 Author-email: kabirjaiswal30@gmail.com
 License: Apache License 2.0
 Description: # Airflow KDB Provider
```

### Comparing `airflow-kdb-provider-0.1.2/README.md` & `airflow-kdb-provider-0.1.3/README.md`

 * *Files identical despite different names*

### Comparing `airflow-kdb-provider-0.1.2/airflow_kdb_provider.egg-info/PKG-INFO` & `airflow-kdb-provider-0.1.3/airflow_kdb_provider.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: airflow-kdb-provider
-Version: 0.1.2
+Version: 0.1.3
 Summary: Apache Airflow provider for KDBAirflowOperator
 Home-page: UNKNOWN
 Author: Kabir Jaiswal
 Author-email: kabirjaiswal30@gmail.com
 License: Apache License 2.0
 Description: # Airflow KDB Provider
```

### Comparing `airflow-kdb-provider-0.1.2/setup.py` & `airflow-kdb-provider-0.1.3/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 # Read the README.md content
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name='airflow-kdb-provider',
-    version='0.1.2',
+    version='0.1.3',
     description='Apache Airflow provider for KDBAirflowOperator',
     long_description=long_description,
     long_description_content_type="text/markdown",
     author='Kabir Jaiswal',
     author_email='kabirjaiswal30@gmail.com',
     license='Apache License 2.0',
     packages=find_packages(),
```

