# Comparing `tmp/Slpapy-0.2.7.tar.gz` & `tmp/Slpapy-0.2.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Slpapy-0.2.7.tar", last modified: Fri May  5 07:57:47 2023, max compression
+gzip compressed data, was "Slpapy-0.2.8.tar", last modified: Fri May  5 07:59:05 2023, max compression
```

## Comparing `Slpapy-0.2.7.tar` & `Slpapy-0.2.8.tar`

### file list

```diff
@@ -1,29 +1,29 @@
-drwxrwxrwx   0        0        0        0 2023-05-05 07:57:47.850681 Slpapy-0.2.7/
--rw-rw-rw-   0        0        0      159 2023-05-05 07:57:47.849681 Slpapy-0.2.7/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-05-05 07:57:47.814681 Slpapy-0.2.7/Slpapy/
--rw-rw-rw-   0        0        0     3120 2023-05-05 07:57:07.000000 Slpapy-0.2.7/Slpapy/Data_reconstruction.py
--rw-rw-rw-   0        0        0     1015 2023-04-10 03:52:28.000000 Slpapy-0.2.7/Slpapy/MZ_ppm_match.py
-drwxrwxrwx   0        0        0        0 2023-05-05 07:57:47.847681 Slpapy-0.2.7/Slpapy/Spatial_map/
--rw-rw-rw-   0        0        0      293 2023-04-18 09:32:26.000000 Slpapy-0.2.7/Slpapy/Spatial_map/Spatial_map.py
--rw-rw-rw-   0        0        0       62 2023-04-18 08:17:33.000000 Slpapy-0.2.7/Slpapy/Spatial_map/__init__.py
--rw-rw-rw-   0        0        0      936 2023-03-31 06:05:23.000000 Slpapy-0.2.7/Slpapy/Spatial_map/_compat.py
--rw-rw-rw-   0        0        0    13507 2023-03-31 06:05:23.000000 Slpapy-0.2.7/Slpapy/Spatial_map/_docs.py
--rw-rw-rw-   0        0        0     1935 2023-03-31 06:05:23.000000 Slpapy-0.2.7/Slpapy/Spatial_map/_rcmod.py
--rw-rw-rw-   0        0        0    15781 2023-04-18 09:43:06.000000 Slpapy-0.2.7/Slpapy/Spatial_map/_settings.py
--rw-rw-rw-   0        0        0    38840 2023-04-18 09:54:49.000000 Slpapy-0.2.7/Slpapy/Spatial_map/_utils.py
--rw-rw-rw-   0        0        0    26068 2023-04-18 09:48:59.000000 Slpapy-0.2.7/Slpapy/Spatial_map/beats.py
--rw-rw-rw-   0        0        0     2817 2023-03-31 06:05:23.000000 Slpapy-0.2.7/Slpapy/Spatial_map/is_constant.py
--rw-rw-rw-   0        0        0     8160 2023-04-18 09:54:49.000000 Slpapy-0.2.7/Slpapy/Spatial_map/logging.py
--rw-rw-rw-   0        0        0     4615 2023-03-31 06:05:23.000000 Slpapy-0.2.7/Slpapy/Spatial_map/palettes.py
--rw-rw-rw-   0        0        0    34738 2023-04-18 09:54:49.000000 Slpapy-0.2.7/Slpapy/Spatial_map/readwrite.py
--rw-rw-rw-   0        0        0    43073 2023-04-18 09:56:24.000000 Slpapy-0.2.7/Slpapy/Spatial_map/scatterplots.py
--rw-rw-rw-   0        0        0      269 2023-04-18 10:11:49.000000 Slpapy-0.2.7/Slpapy/__init__.py
--rw-rw-rw-   0        0        0     5262 2023-05-03 07:08:38.000000 Slpapy-0.2.7/Slpapy/processing_analyze.py
-drwxrwxrwx   0        0        0        0 2023-05-05 07:57:47.823681 Slpapy-0.2.7/Slpapy.egg-info/
--rw-rw-rw-   0        0        0      159 2023-05-05 07:57:47.000000 Slpapy-0.2.7/Slpapy.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      661 2023-05-05 07:57:47.000000 Slpapy-0.2.7/Slpapy.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-05 07:57:47.000000 Slpapy-0.2.7/Slpapy.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      110 2023-05-05 07:57:47.000000 Slpapy-0.2.7/Slpapy.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-05-05 07:57:47.000000 Slpapy-0.2.7/Slpapy.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-05 07:57:47.850681 Slpapy-0.2.7/setup.cfg
--rw-rw-rw-   0        0        0      486 2023-05-05 07:57:16.000000 Slpapy-0.2.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-05 07:59:05.082957 Slpapy-0.2.8/
+-rw-rw-rw-   0        0        0      159 2023-05-05 07:59:05.081956 Slpapy-0.2.8/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-05-05 07:59:05.046957 Slpapy-0.2.8/Slpapy/
+-rw-rw-rw-   0        0        0     3120 2023-05-05 07:57:07.000000 Slpapy-0.2.8/Slpapy/Data_reconstruction.py
+-rw-rw-rw-   0        0        0     1015 2023-04-10 03:52:28.000000 Slpapy-0.2.8/Slpapy/MZ_ppm_match.py
+drwxrwxrwx   0        0        0        0 2023-05-05 07:59:05.079957 Slpapy-0.2.8/Slpapy/Spatial_map/
+-rw-rw-rw-   0        0        0      293 2023-04-18 09:32:26.000000 Slpapy-0.2.8/Slpapy/Spatial_map/Spatial_map.py
+-rw-rw-rw-   0        0        0       62 2023-04-18 08:17:33.000000 Slpapy-0.2.8/Slpapy/Spatial_map/__init__.py
+-rw-rw-rw-   0        0        0      936 2023-03-31 06:05:23.000000 Slpapy-0.2.8/Slpapy/Spatial_map/_compat.py
+-rw-rw-rw-   0        0        0    13507 2023-03-31 06:05:23.000000 Slpapy-0.2.8/Slpapy/Spatial_map/_docs.py
+-rw-rw-rw-   0        0        0     1935 2023-03-31 06:05:23.000000 Slpapy-0.2.8/Slpapy/Spatial_map/_rcmod.py
+-rw-rw-rw-   0        0        0    15781 2023-04-18 09:43:06.000000 Slpapy-0.2.8/Slpapy/Spatial_map/_settings.py
+-rw-rw-rw-   0        0        0    38840 2023-04-18 09:54:49.000000 Slpapy-0.2.8/Slpapy/Spatial_map/_utils.py
+-rw-rw-rw-   0        0        0    26068 2023-04-18 09:48:59.000000 Slpapy-0.2.8/Slpapy/Spatial_map/beats.py
+-rw-rw-rw-   0        0        0     2817 2023-03-31 06:05:23.000000 Slpapy-0.2.8/Slpapy/Spatial_map/is_constant.py
+-rw-rw-rw-   0        0        0     8160 2023-04-18 09:54:49.000000 Slpapy-0.2.8/Slpapy/Spatial_map/logging.py
+-rw-rw-rw-   0        0        0     4615 2023-03-31 06:05:23.000000 Slpapy-0.2.8/Slpapy/Spatial_map/palettes.py
+-rw-rw-rw-   0        0        0    34738 2023-04-18 09:54:49.000000 Slpapy-0.2.8/Slpapy/Spatial_map/readwrite.py
+-rw-rw-rw-   0        0        0    43073 2023-04-18 09:56:24.000000 Slpapy-0.2.8/Slpapy/Spatial_map/scatterplots.py
+-rw-rw-rw-   0        0        0      269 2023-04-18 10:11:49.000000 Slpapy-0.2.8/Slpapy/__init__.py
+-rw-rw-rw-   0        0        0     5262 2023-05-03 07:08:38.000000 Slpapy-0.2.8/Slpapy/processing_analyze.py
+drwxrwxrwx   0        0        0        0 2023-05-05 07:59:05.055987 Slpapy-0.2.8/Slpapy.egg-info/
+-rw-rw-rw-   0        0        0      159 2023-05-05 07:59:04.000000 Slpapy-0.2.8/Slpapy.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      661 2023-05-05 07:59:04.000000 Slpapy-0.2.8/Slpapy.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-05 07:59:04.000000 Slpapy-0.2.8/Slpapy.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      110 2023-05-05 07:59:04.000000 Slpapy-0.2.8/Slpapy.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-05-05 07:59:04.000000 Slpapy-0.2.8/Slpapy.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-05 07:59:05.082957 Slpapy-0.2.8/setup.cfg
+-rw-rw-rw-   0        0        0      486 2023-05-05 07:58:15.000000 Slpapy-0.2.8/setup.py
```

### Comparing `Slpapy-0.2.7/Slpapy/Data_reconstruction.py` & `Slpapy-0.2.8/Slpapy/Data_reconstruction.py`

 * *Files identical despite different names*

### Comparing `Slpapy-0.2.7/Slpapy/MZ_ppm_match.py` & `Slpapy-0.2.8/Slpapy/MZ_ppm_match.py`

 * *Files identical despite different names*

### Comparing `Slpapy-0.2.7/Slpapy/Spatial_map/_compat.py` & `Slpapy-0.2.8/Slpapy/Spatial_map/_compat.py`

 * *Files identical despite different names*

### Comparing `Slpapy-0.2.7/Slpapy/Spatial_map/_docs.py` & `Slpapy-0.2.8/Slpapy/Spatial_map/_docs.py`

 * *Files identical despite different names*

### Comparing `Slpapy-0.2.7/Slpapy/Spatial_map/_rcmod.py` & `Slpapy-0.2.8/Slpapy/Spatial_map/_rcmod.py`

 * *Files identical despite different names*

### Comparing `Slpapy-0.2.7/Slpapy/Spatial_map/_settings.py` & `Slpapy-0.2.8/Slpapy/Spatial_map/_settings.py`

 * *Files identical despite different names*

### Comparing `Slpapy-0.2.7/Slpapy/Spatial_map/_utils.py` & `Slpapy-0.2.8/Slpapy/Spatial_map/_utils.py`

 * *Files identical despite different names*

### Comparing `Slpapy-0.2.7/Slpapy/Spatial_map/beats.py` & `Slpapy-0.2.8/Slpapy/Spatial_map/beats.py`

 * *Files identical despite different names*

### Comparing `Slpapy-0.2.7/Slpapy/Spatial_map/is_constant.py` & `Slpapy-0.2.8/Slpapy/Spatial_map/is_constant.py`

 * *Files identical despite different names*

### Comparing `Slpapy-0.2.7/Slpapy/Spatial_map/logging.py` & `Slpapy-0.2.8/Slpapy/Spatial_map/logging.py`

 * *Files identical despite different names*

### Comparing `Slpapy-0.2.7/Slpapy/Spatial_map/palettes.py` & `Slpapy-0.2.8/Slpapy/Spatial_map/palettes.py`

 * *Files identical despite different names*

### Comparing `Slpapy-0.2.7/Slpapy/Spatial_map/readwrite.py` & `Slpapy-0.2.8/Slpapy/Spatial_map/readwrite.py`

 * *Files identical despite different names*

### Comparing `Slpapy-0.2.7/Slpapy/Spatial_map/scatterplots.py` & `Slpapy-0.2.8/Slpapy/Spatial_map/scatterplots.py`

 * *Files identical despite different names*

### Comparing `Slpapy-0.2.7/Slpapy/processing_analyze.py` & `Slpapy-0.2.8/Slpapy/processing_analyze.py`

 * *Files identical despite different names*

### Comparing `Slpapy-0.2.7/Slpapy.egg-info/SOURCES.txt` & `Slpapy-0.2.8/Slpapy.egg-info/SOURCES.txt`

 * *Files identical despite different names*

