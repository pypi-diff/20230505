# Comparing `tmp/localstack-plugin-persistence-1.0.2.tar.gz` & `tmp/localstack-plugin-persistence-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "localstack-plugin-persistence-1.0.2.tar", last modified: Tue May  2 18:27:27 2023, max compression
+gzip compressed data, was "localstack-plugin-persistence-1.0.3.tar", last modified: Fri May  5 13:09:20 2023, max compression
```

## Comparing `localstack-plugin-persistence-1.0.2.tar` & `localstack-plugin-persistence-1.0.3.tar`

### file list

```diff
@@ -1,48 +1,49 @@
-drwxr-xr-x   0 giograno   (501) staff       (20)        0 2023-05-02 18:27:27.845333 localstack-plugin-persistence-1.0.2/
--rw-r--r--   0 giograno   (501) staff       (20)      331 2023-05-02 18:27:27.845409 localstack-plugin-persistence-1.0.2/PKG-INFO
-drwxr-xr-x   0 giograno   (501) staff       (20)        0 2023-05-02 18:27:27.840312 localstack-plugin-persistence-1.0.2/localstack_persistence/
--rw-r--r--   0 giograno   (501) staff       (20)        0 2023-05-02 18:27:27.000000 localstack-plugin-persistence-1.0.2/localstack_persistence/__init__.py
--rw-r--r--   0 giograno   (501) staff       (20)      175 2023-05-02 18:27:27.000000 localstack-plugin-persistence-1.0.2/localstack_persistence/constants.py
-drwxr-xr-x   0 giograno   (501) staff       (20)        0 2023-05-02 18:27:27.840585 localstack-plugin-persistence-1.0.2/localstack_persistence/pickling/
--rw-r--r--   0 giograno   (501) staff       (20)        0 2023-05-02 18:27:27.000000 localstack-plugin-persistence-1.0.2/localstack_persistence/pickling/__init__.py
--rw-r--r--   0 giograno   (501) staff       (20)      372 2023-05-02 18:27:27.000000 localstack-plugin-persistence-1.0.2/localstack_persistence/pickling/__plugins__.py
-drwxr-xr-x   0 giograno   (501) staff       (20)        0 2023-05-02 18:27:27.841040 localstack-plugin-persistence-1.0.2/localstack_persistence/pickling/reducers/
--rw-r--r--   0 giograno   (501) staff       (20)      533 2023-05-02 18:27:27.000000 localstack-plugin-persistence-1.0.2/localstack_persistence/pickling/reducers/__init__.py
--rw-r--r--   0 giograno   (501) staff       (20)     1514 2023-05-02 18:27:27.000000 localstack-plugin-persistence-1.0.2/localstack_persistence/pickling/reducers/cryptography.py
-drwxr-xr-x   0 giograno   (501) staff       (20)        0 2023-05-02 18:27:27.841333 localstack-plugin-persistence-1.0.2/localstack_persistence/pickling/reducers/services/
--rw-r--r--   0 giograno   (501) staff       (20)        0 2023-05-02 18:27:27.000000 localstack-plugin-persistence-1.0.2/localstack_persistence/pickling/reducers/services/__init__.py
--rw-r--r--   0 giograno   (501) staff       (20)      391 2023-05-02 18:27:27.000000 localstack-plugin-persistence-1.0.2/localstack_persistence/pickling/reducers/services/acm.py
--rw-r--r--   0 giograno   (501) staff       (20)     1710 2023-05-02 18:27:27.000000 localstack-plugin-persistence-1.0.2/localstack_persistence/pickling/reducers/stdlib.py
-drwxr-xr-x   0 giograno   (501) staff       (20)        0 2023-05-02 18:27:27.842185 localstack-plugin-persistence-1.0.2/localstack_persistence/pods/
--rw-r--r--   0 giograno   (501) staff       (20)        0 2023-05-02 18:27:27.000000 localstack-plugin-persistence-1.0.2/localstack_persistence/pods/__init__.py
--rw-r--r--   0 giograno   (501) staff       (20)      333 2023-05-02 18:27:27.000000 localstack-plugin-persistence-1.0.2/localstack_persistence/pods/__plugins__.py
--rw-r--r--   0 giograno   (501) staff       (20)     1754 2023-05-02 18:27:27.000000 localstack-plugin-persistence-1.0.2/localstack_persistence/pods/endpoints.py
--rw-r--r--   0 giograno   (501) staff       (20)     3155 2023-05-02 18:27:27.000000 localstack-plugin-persistence-1.0.2/localstack_persistence/pods/load.py
--rw-r--r--   0 giograno   (501) staff       (20)     2038 2023-05-02 18:27:27.000000 localstack-plugin-persistence-1.0.2/localstack_persistence/pods/manager.py
--rw-r--r--   0 giograno   (501) staff       (20)     1638 2023-05-02 18:27:27.000000 localstack-plugin-persistence-1.0.2/localstack_persistence/pods/save.py
-drwxr-xr-x   0 giograno   (501) staff       (20)        0 2023-05-02 18:27:27.842731 localstack-plugin-persistence-1.0.2/localstack_persistence/reset/
--rw-r--r--   0 giograno   (501) staff       (20)        0 2023-05-02 18:27:27.000000 localstack-plugin-persistence-1.0.2/localstack_persistence/reset/__init__.py
--rw-r--r--   0 giograno   (501) staff       (20)      337 2023-05-02 18:27:27.000000 localstack-plugin-persistence-1.0.2/localstack_persistence/reset/__plugins__.py
--rw-r--r--   0 giograno   (501) staff       (20)      766 2023-05-02 18:27:27.000000 localstack-plugin-persistence-1.0.2/localstack_persistence/reset/endpoints.py
--rw-r--r--   0 giograno   (501) staff       (20)     2478 2023-05-02 18:27:27.000000 localstack-plugin-persistence-1.0.2/localstack_persistence/reset/reset.py
-drwxr-xr-x   0 giograno   (501) staff       (20)        0 2023-05-02 18:27:27.843751 localstack-plugin-persistence-1.0.2/localstack_persistence/snapshot/
--rw-r--r--   0 giograno   (501) staff       (20)        0 2023-05-02 18:27:27.000000 localstack-plugin-persistence-1.0.2/localstack_persistence/snapshot/__init__.py
--rw-r--r--   0 giograno   (501) staff       (20)     3410 2023-05-02 18:27:27.000000 localstack-plugin-persistence-1.0.2/localstack_persistence/snapshot/__plugins__.py
--rw-r--r--   0 giograno   (501) staff       (20)     1030 2023-05-02 18:27:27.000000 localstack-plugin-persistence-1.0.2/localstack_persistence/snapshot/api.py
--rw-r--r--   0 giograno   (501) staff       (20)      580 2023-05-02 18:27:27.000000 localstack-plugin-persistence-1.0.2/localstack_persistence/snapshot/endpoints.py
--rw-r--r--   0 giograno   (501) staff       (20)     1640 2023-05-02 18:27:27.000000 localstack-plugin-persistence-1.0.2/localstack_persistence/snapshot/load.py
--rw-r--r--   0 giograno   (501) staff       (20)     6973 2023-05-02 18:27:27.000000 localstack-plugin-persistence-1.0.2/localstack_persistence/snapshot/manager.py
--rw-r--r--   0 giograno   (501) staff       (20)     1361 2023-05-02 18:27:27.000000 localstack-plugin-persistence-1.0.2/localstack_persistence/snapshot/save.py
--rw-r--r--   0 giograno   (501) staff       (20)      584 2023-05-02 18:27:27.000000 localstack-plugin-persistence-1.0.2/localstack_persistence/utils.py
-drwxr-xr-x   0 giograno   (501) staff       (20)        0 2023-05-02 18:27:27.845191 localstack-plugin-persistence-1.0.2/localstack_plugin_persistence.egg-info/
--rw-r--r--   0 giograno   (501) staff       (20)      331 2023-05-02 18:27:27.000000 localstack-plugin-persistence-1.0.2/localstack_plugin_persistence.egg-info/PKG-INFO
--rw-r--r--   0 giograno   (501) staff       (20)     1626 2023-05-02 18:27:27.000000 localstack-plugin-persistence-1.0.2/localstack_plugin_persistence.egg-info/SOURCES.txt
--rw-r--r--   0 giograno   (501) staff       (20)        1 2023-05-02 18:27:27.000000 localstack-plugin-persistence-1.0.2/localstack_plugin_persistence.egg-info/dependency_links.txt
--rw-r--r--   0 giograno   (501) staff       (20)      925 2023-05-02 18:27:27.000000 localstack-plugin-persistence-1.0.2/localstack_plugin_persistence.egg-info/entry_points.txt
--rw-r--r--   0 giograno   (501) staff       (20)        1 2023-05-02 18:27:27.000000 localstack-plugin-persistence-1.0.2/localstack_plugin_persistence.egg-info/not-zip-safe
--rw-r--r--   0 giograno   (501) staff       (20)      940 2023-05-02 18:27:27.000000 localstack-plugin-persistence-1.0.2/localstack_plugin_persistence.egg-info/plux.json
--rw-r--r--   0 giograno   (501) staff       (20)      277 2023-05-02 18:27:27.000000 localstack-plugin-persistence-1.0.2/localstack_plugin_persistence.egg-info/requires.txt
--rw-r--r--   0 giograno   (501) staff       (20)       23 2023-05-02 18:27:27.000000 localstack-plugin-persistence-1.0.2/localstack_plugin_persistence.egg-info/top_level.txt
--rw-r--r--   0 giograno   (501) staff       (20)      571 2023-05-02 18:27:27.000000 localstack-plugin-persistence-1.0.2/pyproject.toml
--rw-r--r--   0 giograno   (501) staff       (20)      843 2023-05-02 18:27:27.845747 localstack-plugin-persistence-1.0.2/setup.cfg
--rwxr-xr-x   0 giograno   (501) staff       (20)       60 2023-05-02 18:27:27.000000 localstack-plugin-persistence-1.0.2/setup.py
+drwxr-xr-x   0 giograno   (501) staff       (20)        0 2023-05-05 13:09:20.610731 localstack-plugin-persistence-1.0.3/
+-rw-r--r--   0 giograno   (501) staff       (20)      331 2023-05-05 13:09:20.610791 localstack-plugin-persistence-1.0.3/PKG-INFO
+drwxr-xr-x   0 giograno   (501) staff       (20)        0 2023-05-05 13:09:20.605920 localstack-plugin-persistence-1.0.3/localstack_persistence/
+-rw-r--r--   0 giograno   (501) staff       (20)        0 2023-05-05 13:09:20.000000 localstack-plugin-persistence-1.0.3/localstack_persistence/__init__.py
+-rw-r--r--   0 giograno   (501) staff       (20)      175 2023-05-05 13:09:20.000000 localstack-plugin-persistence-1.0.3/localstack_persistence/constants.py
+drwxr-xr-x   0 giograno   (501) staff       (20)        0 2023-05-05 13:09:20.606194 localstack-plugin-persistence-1.0.3/localstack_persistence/pickling/
+-rw-r--r--   0 giograno   (501) staff       (20)        0 2023-05-05 13:09:20.000000 localstack-plugin-persistence-1.0.3/localstack_persistence/pickling/__init__.py
+-rw-r--r--   0 giograno   (501) staff       (20)      372 2023-05-05 13:09:20.000000 localstack-plugin-persistence-1.0.3/localstack_persistence/pickling/__plugins__.py
+drwxr-xr-x   0 giograno   (501) staff       (20)        0 2023-05-05 13:09:20.606788 localstack-plugin-persistence-1.0.3/localstack_persistence/pickling/reducers/
+-rw-r--r--   0 giograno   (501) staff       (20)      533 2023-05-05 13:09:20.000000 localstack-plugin-persistence-1.0.3/localstack_persistence/pickling/reducers/__init__.py
+-rw-r--r--   0 giograno   (501) staff       (20)      259 2023-05-05 13:09:20.000000 localstack-plugin-persistence-1.0.3/localstack_persistence/pickling/reducers/botocore.py
+-rw-r--r--   0 giograno   (501) staff       (20)     1514 2023-05-05 13:09:20.000000 localstack-plugin-persistence-1.0.3/localstack_persistence/pickling/reducers/cryptography.py
+drwxr-xr-x   0 giograno   (501) staff       (20)        0 2023-05-05 13:09:20.607062 localstack-plugin-persistence-1.0.3/localstack_persistence/pickling/reducers/services/
+-rw-r--r--   0 giograno   (501) staff       (20)        0 2023-05-05 13:09:20.000000 localstack-plugin-persistence-1.0.3/localstack_persistence/pickling/reducers/services/__init__.py
+-rw-r--r--   0 giograno   (501) staff       (20)      391 2023-05-05 13:09:20.000000 localstack-plugin-persistence-1.0.3/localstack_persistence/pickling/reducers/services/acm.py
+-rw-r--r--   0 giograno   (501) staff       (20)     1710 2023-05-05 13:09:20.000000 localstack-plugin-persistence-1.0.3/localstack_persistence/pickling/reducers/stdlib.py
+drwxr-xr-x   0 giograno   (501) staff       (20)        0 2023-05-05 13:09:20.607905 localstack-plugin-persistence-1.0.3/localstack_persistence/pods/
+-rw-r--r--   0 giograno   (501) staff       (20)        0 2023-05-05 13:09:20.000000 localstack-plugin-persistence-1.0.3/localstack_persistence/pods/__init__.py
+-rw-r--r--   0 giograno   (501) staff       (20)      333 2023-05-05 13:09:20.000000 localstack-plugin-persistence-1.0.3/localstack_persistence/pods/__plugins__.py
+-rw-r--r--   0 giograno   (501) staff       (20)     1754 2023-05-05 13:09:20.000000 localstack-plugin-persistence-1.0.3/localstack_persistence/pods/endpoints.py
+-rw-r--r--   0 giograno   (501) staff       (20)     3155 2023-05-05 13:09:20.000000 localstack-plugin-persistence-1.0.3/localstack_persistence/pods/load.py
+-rw-r--r--   0 giograno   (501) staff       (20)     2038 2023-05-05 13:09:20.000000 localstack-plugin-persistence-1.0.3/localstack_persistence/pods/manager.py
+-rw-r--r--   0 giograno   (501) staff       (20)     1638 2023-05-05 13:09:20.000000 localstack-plugin-persistence-1.0.3/localstack_persistence/pods/save.py
+drwxr-xr-x   0 giograno   (501) staff       (20)        0 2023-05-05 13:09:20.608449 localstack-plugin-persistence-1.0.3/localstack_persistence/reset/
+-rw-r--r--   0 giograno   (501) staff       (20)        0 2023-05-05 13:09:20.000000 localstack-plugin-persistence-1.0.3/localstack_persistence/reset/__init__.py
+-rw-r--r--   0 giograno   (501) staff       (20)      337 2023-05-05 13:09:20.000000 localstack-plugin-persistence-1.0.3/localstack_persistence/reset/__plugins__.py
+-rw-r--r--   0 giograno   (501) staff       (20)      766 2023-05-05 13:09:20.000000 localstack-plugin-persistence-1.0.3/localstack_persistence/reset/endpoints.py
+-rw-r--r--   0 giograno   (501) staff       (20)     2478 2023-05-05 13:09:20.000000 localstack-plugin-persistence-1.0.3/localstack_persistence/reset/reset.py
+drwxr-xr-x   0 giograno   (501) staff       (20)        0 2023-05-05 13:09:20.609426 localstack-plugin-persistence-1.0.3/localstack_persistence/snapshot/
+-rw-r--r--   0 giograno   (501) staff       (20)        0 2023-05-05 13:09:20.000000 localstack-plugin-persistence-1.0.3/localstack_persistence/snapshot/__init__.py
+-rw-r--r--   0 giograno   (501) staff       (20)     3410 2023-05-05 13:09:20.000000 localstack-plugin-persistence-1.0.3/localstack_persistence/snapshot/__plugins__.py
+-rw-r--r--   0 giograno   (501) staff       (20)     1030 2023-05-05 13:09:20.000000 localstack-plugin-persistence-1.0.3/localstack_persistence/snapshot/api.py
+-rw-r--r--   0 giograno   (501) staff       (20)      580 2023-05-05 13:09:20.000000 localstack-plugin-persistence-1.0.3/localstack_persistence/snapshot/endpoints.py
+-rw-r--r--   0 giograno   (501) staff       (20)     1640 2023-05-05 13:09:20.000000 localstack-plugin-persistence-1.0.3/localstack_persistence/snapshot/load.py
+-rw-r--r--   0 giograno   (501) staff       (20)     6973 2023-05-05 13:09:20.000000 localstack-plugin-persistence-1.0.3/localstack_persistence/snapshot/manager.py
+-rw-r--r--   0 giograno   (501) staff       (20)     1361 2023-05-05 13:09:20.000000 localstack-plugin-persistence-1.0.3/localstack_persistence/snapshot/save.py
+-rw-r--r--   0 giograno   (501) staff       (20)      584 2023-05-05 13:09:20.000000 localstack-plugin-persistence-1.0.3/localstack_persistence/utils.py
+drwxr-xr-x   0 giograno   (501) staff       (20)        0 2023-05-05 13:09:20.610597 localstack-plugin-persistence-1.0.3/localstack_plugin_persistence.egg-info/
+-rw-r--r--   0 giograno   (501) staff       (20)      331 2023-05-05 13:09:20.000000 localstack-plugin-persistence-1.0.3/localstack_plugin_persistence.egg-info/PKG-INFO
+-rw-r--r--   0 giograno   (501) staff       (20)     1679 2023-05-05 13:09:20.000000 localstack-plugin-persistence-1.0.3/localstack_plugin_persistence.egg-info/SOURCES.txt
+-rw-r--r--   0 giograno   (501) staff       (20)        1 2023-05-05 13:09:20.000000 localstack-plugin-persistence-1.0.3/localstack_plugin_persistence.egg-info/dependency_links.txt
+-rw-r--r--   0 giograno   (501) staff       (20)      925 2023-05-05 13:09:20.000000 localstack-plugin-persistence-1.0.3/localstack_plugin_persistence.egg-info/entry_points.txt
+-rw-r--r--   0 giograno   (501) staff       (20)        1 2023-05-05 13:09:20.000000 localstack-plugin-persistence-1.0.3/localstack_plugin_persistence.egg-info/not-zip-safe
+-rw-r--r--   0 giograno   (501) staff       (20)      940 2023-05-05 13:09:20.000000 localstack-plugin-persistence-1.0.3/localstack_plugin_persistence.egg-info/plux.json
+-rw-r--r--   0 giograno   (501) staff       (20)      277 2023-05-05 13:09:20.000000 localstack-plugin-persistence-1.0.3/localstack_plugin_persistence.egg-info/requires.txt
+-rw-r--r--   0 giograno   (501) staff       (20)       23 2023-05-05 13:09:20.000000 localstack-plugin-persistence-1.0.3/localstack_plugin_persistence.egg-info/top_level.txt
+-rw-r--r--   0 giograno   (501) staff       (20)      571 2023-05-05 13:09:20.000000 localstack-plugin-persistence-1.0.3/pyproject.toml
+-rw-r--r--   0 giograno   (501) staff       (20)      843 2023-05-05 13:09:20.611100 localstack-plugin-persistence-1.0.3/setup.cfg
+-rwxr-xr-x   0 giograno   (501) staff       (20)       60 2023-05-05 13:09:20.000000 localstack-plugin-persistence-1.0.3/setup.py
```

### Comparing `localstack-plugin-persistence-1.0.2/localstack_persistence/pickling/reducers/__init__.py` & `localstack-plugin-persistence-1.0.3/localstack_persistence/pickling/reducers/__init__.py`

 * *Files identical despite different names*

### Comparing `localstack-plugin-persistence-1.0.2/localstack_persistence/pickling/reducers/cryptography.py` & `localstack-plugin-persistence-1.0.3/localstack_persistence/pickling/reducers/cryptography.py`

 * *Files identical despite different names*

### Comparing `localstack-plugin-persistence-1.0.2/localstack_persistence/pickling/reducers/stdlib.py` & `localstack-plugin-persistence-1.0.3/localstack_persistence/pickling/reducers/stdlib.py`

 * *Files identical despite different names*

### Comparing `localstack-plugin-persistence-1.0.2/localstack_persistence/pods/endpoints.py` & `localstack-plugin-persistence-1.0.3/localstack_persistence/pods/endpoints.py`

 * *Files identical despite different names*

### Comparing `localstack-plugin-persistence-1.0.2/localstack_persistence/pods/load.py` & `localstack-plugin-persistence-1.0.3/localstack_persistence/pods/load.py`

 * *Files identical despite different names*

### Comparing `localstack-plugin-persistence-1.0.2/localstack_persistence/pods/manager.py` & `localstack-plugin-persistence-1.0.3/localstack_persistence/pods/manager.py`

 * *Files identical despite different names*

### Comparing `localstack-plugin-persistence-1.0.2/localstack_persistence/pods/save.py` & `localstack-plugin-persistence-1.0.3/localstack_persistence/pods/save.py`

 * *Files identical despite different names*

### Comparing `localstack-plugin-persistence-1.0.2/localstack_persistence/reset/endpoints.py` & `localstack-plugin-persistence-1.0.3/localstack_persistence/reset/endpoints.py`

 * *Files identical despite different names*

### Comparing `localstack-plugin-persistence-1.0.2/localstack_persistence/reset/reset.py` & `localstack-plugin-persistence-1.0.3/localstack_persistence/reset/reset.py`

 * *Files identical despite different names*

### Comparing `localstack-plugin-persistence-1.0.2/localstack_persistence/snapshot/__plugins__.py` & `localstack-plugin-persistence-1.0.3/localstack_persistence/snapshot/__plugins__.py`

 * *Files identical despite different names*

### Comparing `localstack-plugin-persistence-1.0.2/localstack_persistence/snapshot/api.py` & `localstack-plugin-persistence-1.0.3/localstack_persistence/snapshot/api.py`

 * *Files identical despite different names*

### Comparing `localstack-plugin-persistence-1.0.2/localstack_persistence/snapshot/endpoints.py` & `localstack-plugin-persistence-1.0.3/localstack_persistence/snapshot/endpoints.py`

 * *Files identical despite different names*

### Comparing `localstack-plugin-persistence-1.0.2/localstack_persistence/snapshot/load.py` & `localstack-plugin-persistence-1.0.3/localstack_persistence/snapshot/load.py`

 * *Files identical despite different names*

### Comparing `localstack-plugin-persistence-1.0.2/localstack_persistence/snapshot/manager.py` & `localstack-plugin-persistence-1.0.3/localstack_persistence/snapshot/manager.py`

 * *Files identical despite different names*

### Comparing `localstack-plugin-persistence-1.0.2/localstack_persistence/snapshot/save.py` & `localstack-plugin-persistence-1.0.3/localstack_persistence/snapshot/save.py`

 * *Files identical despite different names*

### Comparing `localstack-plugin-persistence-1.0.2/localstack_persistence/utils.py` & `localstack-plugin-persistence-1.0.3/localstack_persistence/utils.py`

 * *Files identical despite different names*

### Comparing `localstack-plugin-persistence-1.0.2/localstack_plugin_persistence.egg-info/SOURCES.txt` & `localstack-plugin-persistence-1.0.3/localstack_plugin_persistence.egg-info/SOURCES.txt`

 * *Files 9% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 setup.py
 localstack_persistence/__init__.py
 localstack_persistence/constants.py
 localstack_persistence/utils.py
 localstack_persistence/pickling/__init__.py
 localstack_persistence/pickling/__plugins__.py
 localstack_persistence/pickling/reducers/__init__.py
+localstack_persistence/pickling/reducers/botocore.py
 localstack_persistence/pickling/reducers/cryptography.py
 localstack_persistence/pickling/reducers/stdlib.py
 localstack_persistence/pickling/reducers/services/__init__.py
 localstack_persistence/pickling/reducers/services/acm.py
 localstack_persistence/pods/__init__.py
 localstack_persistence/pods/__plugins__.py
 localstack_persistence/pods/endpoints.py
```

### Comparing `localstack-plugin-persistence-1.0.2/localstack_plugin_persistence.egg-info/entry_points.txt` & `localstack-plugin-persistence-1.0.3/localstack_plugin_persistence.egg-info/entry_points.txt`

 * *Files identical despite different names*

### Comparing `localstack-plugin-persistence-1.0.2/localstack_plugin_persistence.egg-info/plux.json` & `localstack-plugin-persistence-1.0.3/localstack_plugin_persistence.egg-info/plux.json`

 * *Files 0% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.9523809523809524%*

 * *Differences: {"'localstack.hooks.on_infra_start'": '{insert: [(1, '*

 * *                                      "'register_pickle_patches_runtime=localstack_persistence.pickling.__plugins__:register_pickle_patches_runtime')], "*

 * *                                      'delete: [0]}'}*

```diff
@@ -1,14 +1,14 @@
 {
     "localstack.hooks.on_infra_ready": [
         "do_run_state_load_all=localstack_persistence.snapshot.__plugins__:do_run_state_load_all"
     ],
     "localstack.hooks.on_infra_start": [
-        "register_pickle_patches_runtime=localstack_persistence.pickling.__plugins__:register_pickle_patches_runtime",
         "register_public_cloudpods_endpoints=localstack_persistence.pods.__plugins__:register_public_cloudpods_endpoints",
+        "register_pickle_patches_runtime=localstack_persistence.pickling.__plugins__:register_pickle_patches_runtime",
         "register_reset_state_resource=localstack_persistence.reset.__plugins__:register_reset_state_resource",
         "register_state_load_strategy=localstack_persistence.snapshot.__plugins__:register_state_load_strategy",
         "register_state_resource=localstack_persistence.snapshot.__plugins__:register_state_resource",
         "register_state_save_strategy=localstack_persistence.snapshot.__plugins__:register_state_save_strategy"
     ],
     "localstack.hooks.prepare_host": [
         "register_pickle_patches_host=localstack_persistence.pickling.__plugins__:register_pickle_patches_host"
```

### Comparing `localstack-plugin-persistence-1.0.2/pyproject.toml` & `localstack-plugin-persistence-1.0.3/pyproject.toml`

 * *Files identical despite different names*

### Comparing `localstack-plugin-persistence-1.0.2/setup.cfg` & `localstack-plugin-persistence-1.0.3/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = localstack-plugin-persistence
-version = 1.0.2
+version = 1.0.3
 url = https://github.com/localstack/localstack-plugin-persistence
 author = LocalStack Contributors
 author_email = info@localstack.cloud
 description = plugin containing persistence code
 long_description = file: README.md
 long_description_content_type = text/markdown; charset=UTF-8
```

