# Comparing `tmp/open_geodata-22.6.8.tar.gz` & `tmp/open_geodata-22.6.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "open_geodata-22.6.8.tar", last modified: Wed Sep 14 19:54:59 2022, max compression
+gzip compressed data, was "open_geodata-22.6.9.tar", last modified: Wed Sep 14 20:00:48 2022, max compression
```

## Comparing `open_geodata-22.6.8.tar` & `open_geodata-22.6.9.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-14 19:54:59.370855 open_geodata-22.6.8/
--rw-r--r--   0 runner    (1001) docker     (121)     1069 2022-09-14 19:54:44.000000 open_geodata-22.6.8/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)      642 2022-09-14 19:54:44.000000 open_geodata-22.6.8/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     2464 2022-09-14 19:54:59.370855 open_geodata-22.6.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     1898 2022-09-14 19:54:44.000000 open_geodata-22.6.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-14 19:54:59.370855 open_geodata-22.6.8/open_geodata/
--rw-r--r--   0 runner    (1001) docker     (121)      302 2022-09-14 19:54:44.000000 open_geodata-22.6.8/open_geodata/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)      275 2022-09-14 19:54:51.000000 open_geodata-22.6.8/open_geodata/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-14 19:54:59.370855 open_geodata-22.6.8/open_geodata/converts/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-14 19:54:44.000000 open_geodata-22.6.8/open_geodata/converts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     4845 2022-09-14 19:54:44.000000 open_geodata-22.6.8/open_geodata/converts/converts.py
--rw-r--r--   0 runner    (1001) docker     (121)     1296 2022-09-14 19:54:44.000000 open_geodata-22.6.8/open_geodata/converts/others.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-14 19:54:59.370855 open_geodata-22.6.8/open_geodata/folium_plus/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-14 19:54:44.000000 open_geodata-22.6.8/open_geodata/folium_plus/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     4872 2022-09-14 19:54:44.000000 open_geodata-22.6.8/open_geodata/folium_plus/adds.py
--rw-r--r--   0 runner    (1001) docker     (121)     1471 2022-09-14 19:54:44.000000 open_geodata-22.6.8/open_geodata/functions.py
--rw-r--r--   0 runner    (1001) docker     (121)     4500 2022-09-14 19:54:44.000000 open_geodata-22.6.8/open_geodata/geo.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-14 19:54:59.370855 open_geodata-22.6.8/open_geodata/lyr/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-14 19:54:44.000000 open_geodata-22.6.8/open_geodata/lyr/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     2646 2022-09-14 19:54:44.000000 open_geodata-22.6.8/open_geodata/lyr/base.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-14 19:54:59.370855 open_geodata-22.6.8/open_geodata/sidra/
--rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-14 19:54:44.000000 open_geodata-22.6.8/open_geodata/sidra/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)     1168 2022-09-14 19:54:44.000000 open_geodata-22.6.8/open_geodata/sidra/ibge.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-14 19:54:59.370855 open_geodata-22.6.8/open_geodata.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     2464 2022-09-14 19:54:59.000000 open_geodata-22.6.8/open_geodata.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      612 2022-09-14 19:54:59.000000 open_geodata-22.6.8/open_geodata.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-09-14 19:54:59.000000 open_geodata-22.6.8/open_geodata.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)      157 2022-09-14 19:54:59.000000 open_geodata-22.6.8/open_geodata.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)       13 2022-09-14 19:54:59.000000 open_geodata-22.6.8/open_geodata.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)      157 2022-09-14 19:54:44.000000 open_geodata-22.6.8/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-09-14 19:54:59.370855 open_geodata-22.6.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1707 2022-09-14 19:54:44.000000 open_geodata-22.6.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-14 20:00:48.094684 open_geodata-22.6.9/
+-rw-r--r--   0 runner    (1001) docker     (121)     1069 2022-09-14 20:00:30.000000 open_geodata-22.6.9/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (121)      642 2022-09-14 20:00:30.000000 open_geodata-22.6.9/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (121)     2464 2022-09-14 20:00:48.094684 open_geodata-22.6.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     1898 2022-09-14 20:00:30.000000 open_geodata-22.6.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-14 20:00:48.090684 open_geodata-22.6.9/open_geodata/
+-rw-r--r--   0 runner    (1001) docker     (121)      302 2022-09-14 20:00:30.000000 open_geodata-22.6.9/open_geodata/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      275 2022-09-14 20:00:38.000000 open_geodata-22.6.9/open_geodata/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-14 20:00:48.094684 open_geodata-22.6.9/open_geodata/converts/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-14 20:00:30.000000 open_geodata-22.6.9/open_geodata/converts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4845 2022-09-14 20:00:30.000000 open_geodata-22.6.9/open_geodata/converts/converts.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1296 2022-09-14 20:00:30.000000 open_geodata-22.6.9/open_geodata/converts/others.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-14 20:00:48.094684 open_geodata-22.6.9/open_geodata/folium_plus/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-14 20:00:30.000000 open_geodata-22.6.9/open_geodata/folium_plus/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4872 2022-09-14 20:00:30.000000 open_geodata-22.6.9/open_geodata/folium_plus/adds.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1471 2022-09-14 20:00:30.000000 open_geodata-22.6.9/open_geodata/functions.py
+-rw-r--r--   0 runner    (1001) docker     (121)     4500 2022-09-14 20:00:30.000000 open_geodata-22.6.9/open_geodata/geo.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-14 20:00:48.094684 open_geodata-22.6.9/open_geodata/lyr/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-14 20:00:30.000000 open_geodata-22.6.9/open_geodata/lyr/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     2646 2022-09-14 20:00:30.000000 open_geodata-22.6.9/open_geodata/lyr/base.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-14 20:00:48.094684 open_geodata-22.6.9/open_geodata/sidra/
+-rw-r--r--   0 runner    (1001) docker     (121)        0 2022-09-14 20:00:30.000000 open_geodata-22.6.9/open_geodata/sidra/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1168 2022-09-14 20:00:30.000000 open_geodata-22.6.9/open_geodata/sidra/ibge.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-14 20:00:48.094684 open_geodata-22.6.9/open_geodata.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     2464 2022-09-14 20:00:48.000000 open_geodata-22.6.9/open_geodata.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      612 2022-09-14 20:00:48.000000 open_geodata-22.6.9/open_geodata.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2022-09-14 20:00:48.000000 open_geodata-22.6.9/open_geodata.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      157 2022-09-14 20:00:48.000000 open_geodata-22.6.9/open_geodata.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       13 2022-09-14 20:00:48.000000 open_geodata-22.6.9/open_geodata.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      157 2022-09-14 20:00:30.000000 open_geodata-22.6.9/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       38 2022-09-14 20:00:48.094684 open_geodata-22.6.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)     1707 2022-09-14 20:00:30.000000 open_geodata-22.6.9/setup.py
```

### Comparing `open_geodata-22.6.8/LICENSE` & `open_geodata-22.6.9/LICENSE`

 * *Files identical despite different names*

### Comparing `open_geodata-22.6.8/MANIFEST.in` & `open_geodata-22.6.9/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `open_geodata-22.6.8/PKG-INFO` & `open_geodata-22.6.9/open_geodata.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: open_geodata
-Version: 22.6.8
+Name: open-geodata
+Version: 22.6.9
 Summary: Dados Espaciais do Brasil
 Home-page: https://github.com/open-geodata/open-geodata
 Author: Michel Metran
 Author-email: michelmetran@gmail.com
 Keywords: python,geodata,geoprocessamento
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `open_geodata-22.6.8/README.md` & `open_geodata-22.6.9/README.md`

 * *Files identical despite different names*

### Comparing `open_geodata-22.6.8/open_geodata/converts/converts.py` & `open_geodata-22.6.9/open_geodata/converts/converts.py`

 * *Files identical despite different names*

### Comparing `open_geodata-22.6.8/open_geodata/converts/others.py` & `open_geodata-22.6.9/open_geodata/converts/others.py`

 * *Files identical despite different names*

### Comparing `open_geodata-22.6.8/open_geodata/folium_plus/adds.py` & `open_geodata-22.6.9/open_geodata/folium_plus/adds.py`

 * *Files identical despite different names*

### Comparing `open_geodata-22.6.8/open_geodata/functions.py` & `open_geodata-22.6.9/open_geodata/functions.py`

 * *Files identical despite different names*

### Comparing `open_geodata-22.6.8/open_geodata/geo.py` & `open_geodata-22.6.9/open_geodata/geo.py`

 * *Files identical despite different names*

### Comparing `open_geodata-22.6.8/open_geodata/lyr/base.py` & `open_geodata-22.6.9/open_geodata/lyr/base.py`

 * *Files identical despite different names*

### Comparing `open_geodata-22.6.8/open_geodata/sidra/ibge.py` & `open_geodata-22.6.9/open_geodata/sidra/ibge.py`

 * *Files identical despite different names*

### Comparing `open_geodata-22.6.8/open_geodata.egg-info/PKG-INFO` & `open_geodata-22.6.9/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
-Name: open-geodata
-Version: 22.6.8
+Name: open_geodata
+Version: 22.6.9
 Summary: Dados Espaciais do Brasil
 Home-page: https://github.com/open-geodata/open-geodata
 Author: Michel Metran
 Author-email: michelmetran@gmail.com
 Keywords: python,geodata,geoprocessamento
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `open_geodata-22.6.8/open_geodata.egg-info/SOURCES.txt` & `open_geodata-22.6.9/open_geodata.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `open_geodata-22.6.8/setup.py` & `open_geodata-22.6.9/setup.py`

 * *Files identical despite different names*

