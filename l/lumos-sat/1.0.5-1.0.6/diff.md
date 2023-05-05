# Comparing `tmp/lumos-sat-1.0.5.tar.gz` & `tmp/lumos-sat-1.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lumos-sat-1.0.5.tar", last modified: Thu May  4 20:23:55 2023, max compression
+gzip compressed data, was "lumos-sat-1.0.6.tar", last modified: Fri May  5 00:00:20 2023, max compression
```

## Comparing `lumos-sat-1.0.5.tar` & `lumos-sat-1.0.6.tar`

### file list

```diff
@@ -1,28 +1,28 @@
-drwxrwxrwx   0        0        0        0 2023-05-04 20:23:55.536374 lumos-sat-1.0.5/
--rw-rw-rw-   0        0        0     1096 2023-04-06 18:33:06.000000 lumos-sat-1.0.5/LICENSE
--rw-rw-rw-   0        0        0      834 2023-05-04 20:23:55.533381 lumos-sat-1.0.5/PKG-INFO
--rw-rw-rw-   0        0        0      577 2023-04-06 19:37:58.000000 lumos-sat-1.0.5/README.md
-drwxrwxrwx   0        0        0        0 2023-05-04 20:23:55.469553 lumos-sat-1.0.5/lumos/
--rw-rw-rw-   0        0        0        0 2023-04-06 18:42:57.000000 lumos-sat-1.0.5/lumos/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-04 20:23:55.477535 lumos-sat-1.0.5/lumos/brdf/
--rw-rw-rw-   0        0        0        0 2023-04-06 18:51:47.000000 lumos-sat-1.0.5/lumos/brdf/__init__.py
--rw-rw-rw-   0        0        0     6648 2023-05-02 20:42:09.000000 lumos-sat-1.0.5/lumos/brdf/library.py
--rw-rw-rw-   0        0        0     3255 2023-05-03 21:42:13.000000 lumos-sat-1.0.5/lumos/brdf/tools.py
--rw-rw-rw-   0        0        0    14276 2023-05-03 22:10:42.000000 lumos-sat-1.0.5/lumos/calculator.py
--rw-rw-rw-   0        0        0      340 2023-04-09 01:56:39.000000 lumos-sat-1.0.5/lumos/constants.py
-drwxrwxrwx   0        0        0        0 2023-05-04 20:23:55.484512 lumos-sat-1.0.5/lumos/constellation/
--rw-rw-rw-   0        0        0        0 2023-05-02 20:49:52.000000 lumos-sat-1.0.5/lumos/constellation/__init__.py
--rw-rw-rw-   0        0        0     5105 2023-05-03 19:16:32.000000 lumos-sat-1.0.5/lumos/constellation/library.py
--rw-rw-rw-   0        0        0     1088 2023-05-03 19:16:14.000000 lumos-sat-1.0.5/lumos/constellation/tools.py
--rw-rw-rw-   0        0        0     2369 2023-05-01 16:44:37.000000 lumos-sat-1.0.5/lumos/conversions.py
--rw-rw-rw-   0        0        0     3479 2023-04-09 02:37:52.000000 lumos-sat-1.0.5/lumos/functions.py
--rw-rw-rw-   0        0        0     3971 2023-05-01 19:53:20.000000 lumos-sat-1.0.5/lumos/geometry.py
--rw-rw-rw-   0        0        0     9728 2023-05-03 22:36:00.000000 lumos-sat-1.0.5/lumos/plot.py
-drwxrwxrwx   0        0        0        0 2023-05-04 20:23:55.531387 lumos-sat-1.0.5/lumos_sat.egg-info/
--rw-rw-rw-   0        0        0      834 2023-05-04 20:23:55.000000 lumos-sat-1.0.5/lumos_sat.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      482 2023-05-04 20:23:55.000000 lumos-sat-1.0.5/lumos_sat.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-04 20:23:55.000000 lumos-sat-1.0.5/lumos_sat.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      220 2023-05-04 20:23:55.000000 lumos-sat-1.0.5/lumos_sat.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-05-04 20:23:55.000000 lumos-sat-1.0.5/lumos_sat.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      588 2023-05-04 20:22:30.000000 lumos-sat-1.0.5/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-04 20:23:55.536374 lumos-sat-1.0.5/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-05 00:00:20.833053 lumos-sat-1.0.6/
+-rw-rw-rw-   0        0        0     1096 2023-04-06 18:33:06.000000 lumos-sat-1.0.6/LICENSE
+-rw-rw-rw-   0        0        0      834 2023-05-05 00:00:20.830797 lumos-sat-1.0.6/PKG-INFO
+-rw-rw-rw-   0        0        0      577 2023-04-06 19:37:58.000000 lumos-sat-1.0.6/README.md
+drwxrwxrwx   0        0        0        0 2023-05-05 00:00:20.662449 lumos-sat-1.0.6/lumos/
+-rw-rw-rw-   0        0        0        0 2023-04-06 18:42:57.000000 lumos-sat-1.0.6/lumos/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-05 00:00:20.737633 lumos-sat-1.0.6/lumos/brdf/
+-rw-rw-rw-   0        0        0        0 2023-04-06 18:51:47.000000 lumos-sat-1.0.6/lumos/brdf/__init__.py
+-rw-rw-rw-   0        0        0     6648 2023-05-02 20:42:09.000000 lumos-sat-1.0.6/lumos/brdf/library.py
+-rw-rw-rw-   0        0        0     3255 2023-05-03 21:42:13.000000 lumos-sat-1.0.6/lumos/brdf/tools.py
+-rw-rw-rw-   0        0        0    14276 2023-05-03 22:10:42.000000 lumos-sat-1.0.6/lumos/calculator.py
+-rw-rw-rw-   0        0        0      340 2023-04-09 01:56:39.000000 lumos-sat-1.0.6/lumos/constants.py
+drwxrwxrwx   0        0        0        0 2023-05-05 00:00:20.797492 lumos-sat-1.0.6/lumos/constellation/
+-rw-rw-rw-   0        0        0        0 2023-05-02 20:49:52.000000 lumos-sat-1.0.6/lumos/constellation/__init__.py
+-rw-rw-rw-   0        0        0     5105 2023-05-03 19:16:32.000000 lumos-sat-1.0.6/lumos/constellation/library.py
+-rw-rw-rw-   0        0        0     1088 2023-05-03 19:16:14.000000 lumos-sat-1.0.6/lumos/constellation/tools.py
+-rw-rw-rw-   0        0        0     2369 2023-05-01 16:44:37.000000 lumos-sat-1.0.6/lumos/conversions.py
+-rw-rw-rw-   0        0        0     3479 2023-04-09 02:37:52.000000 lumos-sat-1.0.6/lumos/functions.py
+-rw-rw-rw-   0        0        0     3971 2023-05-01 19:53:20.000000 lumos-sat-1.0.6/lumos/geometry.py
+-rw-rw-rw-   0        0        0     9728 2023-05-03 22:36:00.000000 lumos-sat-1.0.6/lumos/plot.py
+drwxrwxrwx   0        0        0        0 2023-05-05 00:00:20.827872 lumos-sat-1.0.6/lumos_sat.egg-info/
+-rw-rw-rw-   0        0        0      834 2023-05-05 00:00:20.000000 lumos-sat-1.0.6/lumos_sat.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      482 2023-05-05 00:00:20.000000 lumos-sat-1.0.6/lumos_sat.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-05 00:00:20.000000 lumos-sat-1.0.6/lumos_sat.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      247 2023-05-05 00:00:20.000000 lumos-sat-1.0.6/lumos_sat.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-05-05 00:00:20.000000 lumos-sat-1.0.6/lumos_sat.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      631 2023-05-04 23:58:50.000000 lumos-sat-1.0.6/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-05 00:00:20.833053 lumos-sat-1.0.6/setup.cfg
```

### Comparing `lumos-sat-1.0.5/LICENSE` & `lumos-sat-1.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `lumos-sat-1.0.5/PKG-INFO` & `lumos-sat-1.0.6/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lumos-sat
-Version: 1.0.5
+Version: 1.0.6
 Summary: Satellite Brightness Calculation Tools
 Author-email: Forrest Fankhauser <fafankhauser@ucdavis.edu>
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # lumos-sat
```

### Comparing `lumos-sat-1.0.5/README.md` & `lumos-sat-1.0.6/README.md`

 * *Files identical despite different names*

### Comparing `lumos-sat-1.0.5/lumos/brdf/library.py` & `lumos-sat-1.0.6/lumos/brdf/library.py`

 * *Files identical despite different names*

### Comparing `lumos-sat-1.0.5/lumos/brdf/tools.py` & `lumos-sat-1.0.6/lumos/brdf/tools.py`

 * *Files identical despite different names*

### Comparing `lumos-sat-1.0.5/lumos/calculator.py` & `lumos-sat-1.0.6/lumos/calculator.py`

 * *Files identical despite different names*

### Comparing `lumos-sat-1.0.5/lumos/constellation/library.py` & `lumos-sat-1.0.6/lumos/constellation/library.py`

 * *Files identical despite different names*

### Comparing `lumos-sat-1.0.5/lumos/constellation/tools.py` & `lumos-sat-1.0.6/lumos/constellation/tools.py`

 * *Files identical despite different names*

### Comparing `lumos-sat-1.0.5/lumos/conversions.py` & `lumos-sat-1.0.6/lumos/conversions.py`

 * *Files identical despite different names*

### Comparing `lumos-sat-1.0.5/lumos/functions.py` & `lumos-sat-1.0.6/lumos/functions.py`

 * *Files identical despite different names*

### Comparing `lumos-sat-1.0.5/lumos/geometry.py` & `lumos-sat-1.0.6/lumos/geometry.py`

 * *Files identical despite different names*

### Comparing `lumos-sat-1.0.5/lumos/plot.py` & `lumos-sat-1.0.6/lumos/plot.py`

 * *Files identical despite different names*

### Comparing `lumos-sat-1.0.5/lumos_sat.egg-info/PKG-INFO` & `lumos-sat-1.0.6/lumos_sat.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lumos-sat
-Version: 1.0.5
+Version: 1.0.6
 Summary: Satellite Brightness Calculation Tools
 Author-email: Forrest Fankhauser <fafankhauser@ucdavis.edu>
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # lumos-sat
```

### Comparing `lumos-sat-1.0.5/pyproject.toml` & `lumos-sat-1.0.6/pyproject.toml`

 * *Files 15% similar despite different names*

```diff
@@ -1,25 +1,27 @@
 [project]
 name = "lumos-sat"
-version = "1.0.5"
+version = "1.0.6"
 description = "Satellite Brightness Calculation Tools"
 authors = [
     {name = "Forrest Fankhauser", email = "fafankhauser@ucdavis.edu"},
 ]
 requires-python = ">=3.10"
 readme = "README.md"
 
 dependencies = [
+    "astropy~=5.2.2",
     "contourpy~=1.0.7",
     "cycler~=0.11.0",
     "fonttools~=4.39.3",
     "kiwisolver~=1.4.4",
     "matplotlib~=3.7.1",
     "numpy~=1.24.2",
     "opencv-python~=4.7.0.72",
     "packaging~=23.0",
     "Pillow~=9.5.0",
     "pyparsing~=3.0.9",
     "python-dateutil~=2.8.2",
     "scipy~=1.10.1",
+    "sgp4~=2.222",
     "six~=1.16.0"
 ]
```

