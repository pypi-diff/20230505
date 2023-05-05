# Comparing `tmp/PyBerries-0.2.6.tar.gz` & `tmp/PyBerries-0.2.6.post1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PyBerries-0.2.6.tar", last modified: Fri May  5 09:23:33 2023, max compression
+gzip compressed data, was "PyBerries-0.2.6.post1.tar", last modified: Fri May  5 09:47:28 2023, max compression
```

## Comparing `PyBerries-0.2.6.tar` & `PyBerries-0.2.6.post1.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxrwxrwx   0        0        0        0 2023-05-05 09:23:33.224727 PyBerries-0.2.6/
--rw-rw-rw-   0        0        0    33074 2022-12-22 10:37:47.000000 PyBerries-0.2.6/LICENSE
--rw-rw-rw-   0        0        0    14421 2023-05-05 09:23:33.224727 PyBerries-0.2.6/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-05-05 09:23:33.189114 PyBerries-0.2.6/PyBerries.egg-info/
--rw-rw-rw-   0        0        0    14421 2023-05-05 09:23:33.000000 PyBerries-0.2.6/PyBerries.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1062 2023-05-05 09:23:33.000000 PyBerries-0.2.6/PyBerries.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-05 09:23:33.000000 PyBerries-0.2.6/PyBerries.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       70 2023-05-05 09:23:33.000000 PyBerries-0.2.6/PyBerries.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-05-05 09:23:33.000000 PyBerries-0.2.6/PyBerries.egg-info/top_level.txt
--rw-rw-rw-   0        0        0    14103 2023-05-03 12:45:51.000000 PyBerries-0.2.6/README.md
-drwxrwxrwx   0        0        0        0 2023-05-05 09:23:33.189114 PyBerries-0.2.6/pyberries/
-drwxrwxrwx   0        0        0        0 2023-05-05 09:23:33.201122 PyBerries-0.2.6/pyberries/File_utilities/
--rw-rw-rw-   0        0        0     2877 2023-03-14 14:43:41.000000 PyBerries-0.2.6/pyberries/File_utilities/Filename_utils.py
--rw-rw-rw-   0        0        0     2782 2023-03-14 14:14:07.000000 PyBerries-0.2.6/pyberries/File_utilities/Stack_tiffs.py
--rw-rw-rw-   0        0        0      795 2023-03-14 14:14:07.000000 PyBerries-0.2.6/pyberries/File_utilities/Unpack_omero_folders.py
--rw-rw-rw-   0        0        0      119 2023-03-14 14:14:07.000000 PyBerries-0.2.6/pyberries/File_utilities/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-05 09:23:33.205115 PyBerries-0.2.6/pyberries/Metrics/
--rw-rw-rw-   0        0        0     1242 2023-05-02 10:54:16.000000 PyBerries-0.2.6/pyberries/Metrics/Metrics.py
--rw-rw-rw-   0        0        0     6475 2023-05-03 12:50:51.000000 PyBerries-0.2.6/pyberries/Metrics/Time_metrics.py
--rw-rw-rw-   0        0        0       69 2023-03-10 16:15:28.000000 PyBerries-0.2.6/pyberries/Metrics/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-05 09:23:33.224727 PyBerries-0.2.6/pyberries/Plots/
--rw-rw-rw-   0        0        0     1037 2023-05-02 16:02:09.000000 PyBerries-0.2.6/pyberries/Plots/Fits.py
--rw-rw-rw-   0        0        0     4813 2023-05-04 10:28:45.000000 PyBerries-0.2.6/pyberries/Plots/Plot_presets.py
--rw-rw-rw-   0        0        0      353 2023-04-05 10:31:09.000000 PyBerries-0.2.6/pyberries/Plots/Plot_utilities.py
--rw-rw-rw-   0        0        0     1372 2023-04-03 13:51:01.000000 PyBerries-0.2.6/pyberries/Plots/Plots.py
--rw-rw-rw-   0        0        0      117 2023-05-02 10:54:16.000000 PyBerries-0.2.6/pyberries/Plots/__init__.py
--rw-rw-rw-   0        0        0      118 2023-05-04 14:10:33.000000 PyBerries-0.2.6/pyberries/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-05 09:23:33.216711 PyBerries-0.2.6/pyberries/data/
--rw-rw-rw-   0        0        0    16096 2023-05-04 16:04:58.000000 PyBerries-0.2.6/pyberries/data/DatasetPool.py
--rw-rw-rw-   0        0        0     1886 2023-05-04 10:56:45.000000 PyBerries-0.2.6/pyberries/data/Fitting.py
--rw-rw-rw-   0        0        0       86 2023-05-02 15:00:14.000000 PyBerries-0.2.6/pyberries/data/__init__.py
--rw-rw-rw-   0        0        0     1567 2023-05-02 15:50:42.000000 PyBerries-0.2.6/pyberries/data/util.py
--rw-rw-rw-   0        0        0       42 2023-05-05 09:23:33.224727 PyBerries-0.2.6/setup.cfg
--rw-rw-rw-   0        0        0      625 2023-05-05 09:21:57.000000 PyBerries-0.2.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-05 09:47:28.759485 PyBerries-0.2.6.post1/
+-rw-rw-rw-   0        0        0    33074 2022-12-22 10:37:47.000000 PyBerries-0.2.6.post1/LICENSE
+-rw-rw-rw-   0        0        0    14427 2023-05-05 09:47:28.746485 PyBerries-0.2.6.post1/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-05-05 09:47:28.711430 PyBerries-0.2.6.post1/PyBerries.egg-info/
+-rw-rw-rw-   0        0        0    14427 2023-05-05 09:47:28.000000 PyBerries-0.2.6.post1/PyBerries.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      723 2023-05-05 09:47:28.000000 PyBerries-0.2.6.post1/PyBerries.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-05 09:47:28.000000 PyBerries-0.2.6.post1/PyBerries.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       70 2023-05-05 09:47:28.000000 PyBerries-0.2.6.post1/PyBerries.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-05-05 09:47:28.000000 PyBerries-0.2.6.post1/PyBerries.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0    14103 2023-05-03 12:45:51.000000 PyBerries-0.2.6.post1/README.md
+drwxrwxrwx   0        0        0        0 2023-05-05 09:47:28.711430 PyBerries-0.2.6.post1/pyberries/
+-rw-rw-rw-   0        0        0      118 2023-05-04 14:10:33.000000 PyBerries-0.2.6.post1/pyberries/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-05 09:47:28.724432 PyBerries-0.2.6.post1/pyberries/data/
+-rw-rw-rw-   0        0        0    16096 2023-05-04 16:04:58.000000 PyBerries-0.2.6.post1/pyberries/data/DatasetPool.py
+-rw-rw-rw-   0        0        0     1886 2023-05-04 10:56:45.000000 PyBerries-0.2.6.post1/pyberries/data/Fitting.py
+-rw-rw-rw-   0        0        0       86 2023-05-02 15:00:14.000000 PyBerries-0.2.6.post1/pyberries/data/__init__.py
+-rw-rw-rw-   0        0        0     1567 2023-05-02 15:50:42.000000 PyBerries-0.2.6.post1/pyberries/data/util.py
+drwxrwxrwx   0        0        0        0 2023-05-05 09:47:28.733458 PyBerries-0.2.6.post1/pyberries/file_utilities/
+-rw-rw-rw-   0        0        0     2877 2023-03-14 14:43:41.000000 PyBerries-0.2.6.post1/pyberries/file_utilities/Filename_utils.py
+-rw-rw-rw-   0        0        0     2782 2023-03-14 14:14:07.000000 PyBerries-0.2.6.post1/pyberries/file_utilities/Stack_tiffs.py
+-rw-rw-rw-   0        0        0      795 2023-03-14 14:14:07.000000 PyBerries-0.2.6.post1/pyberries/file_utilities/Unpack_omero_folders.py
+-rw-rw-rw-   0        0        0      119 2023-03-14 14:14:07.000000 PyBerries-0.2.6.post1/pyberries/file_utilities/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-05 09:47:28.733458 PyBerries-0.2.6.post1/pyberries/metrics/
+-rw-rw-rw-   0        0        0     1242 2023-05-02 10:54:16.000000 PyBerries-0.2.6.post1/pyberries/metrics/Metrics.py
+-rw-rw-rw-   0        0        0     6475 2023-05-03 12:50:51.000000 PyBerries-0.2.6.post1/pyberries/metrics/Time_metrics.py
+-rw-rw-rw-   0        0        0       69 2023-03-10 16:15:28.000000 PyBerries-0.2.6.post1/pyberries/metrics/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-05 09:47:28.746485 PyBerries-0.2.6.post1/pyberries/plots/
+-rw-rw-rw-   0        0        0     1037 2023-05-02 16:02:09.000000 PyBerries-0.2.6.post1/pyberries/plots/Fits.py
+-rw-rw-rw-   0        0        0     4813 2023-05-04 10:28:45.000000 PyBerries-0.2.6.post1/pyberries/plots/Plot_presets.py
+-rw-rw-rw-   0        0        0      353 2023-04-05 10:31:09.000000 PyBerries-0.2.6.post1/pyberries/plots/Plot_utilities.py
+-rw-rw-rw-   0        0        0     1372 2023-04-03 13:51:01.000000 PyBerries-0.2.6.post1/pyberries/plots/Plots.py
+-rw-rw-rw-   0        0        0      117 2023-05-02 10:54:16.000000 PyBerries-0.2.6.post1/pyberries/plots/__init__.py
+-rw-rw-rw-   0        0        0       42 2023-05-05 09:47:28.759485 PyBerries-0.2.6.post1/setup.cfg
+-rw-rw-rw-   0        0        0      631 2023-05-05 09:45:04.000000 PyBerries-0.2.6.post1/setup.py
```

### Comparing `PyBerries-0.2.6/LICENSE` & `PyBerries-0.2.6.post1/LICENSE`

 * *Files identical despite different names*

### Comparing `PyBerries-0.2.6/PKG-INFO` & `PyBerries-0.2.6.post1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyBerries
-Version: 0.2.6
+Version: 0.2.6.post1
 Summary: Processing of Bacmman measurement tables
 Home-page: https://gitlab.com/MEKlab/pyberries
 Author: Daniel Thedie
 Author-email: daniel.thedie@ed.ac.uk
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `PyBerries-0.2.6/PyBerries.egg-info/PKG-INFO` & `PyBerries-0.2.6.post1/PyBerries.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyBerries
-Version: 0.2.6
+Version: 0.2.6.post1
 Summary: Processing of Bacmman measurement tables
 Home-page: https://gitlab.com/MEKlab/pyberries
 Author: Daniel Thedie
 Author-email: daniel.thedie@ed.ac.uk
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `PyBerries-0.2.6/PyBerries.egg-info/SOURCES.txt` & `PyBerries-0.2.6.post1/PyBerries.egg-info/SOURCES.txt`

 * *Files 23% similar despite different names*

```diff
@@ -3,24 +3,14 @@
 setup.py
 PyBerries.egg-info/PKG-INFO
 PyBerries.egg-info/SOURCES.txt
 PyBerries.egg-info/dependency_links.txt
 PyBerries.egg-info/requires.txt
 PyBerries.egg-info/top_level.txt
 pyberries/__init__.py
-pyberries/File_utilities/Filename_utils.py
-pyberries/File_utilities/Stack_tiffs.py
-pyberries/File_utilities/Unpack_omero_folders.py
-pyberries/File_utilities/__init__.py
-pyberries/Metrics/Metrics.py
-pyberries/Metrics/Time_metrics.py
-pyberries/Metrics/__init__.py
-pyberries/Plots/Fits.py
-pyberries/Plots/Plots.py
-pyberries/Plots/__init__.py
 pyberries/data/DatasetPool.py
 pyberries/data/Fitting.py
 pyberries/data/__init__.py
 pyberries/data/util.py
 pyberries/file_utilities/Filename_utils.py
 pyberries/file_utilities/Stack_tiffs.py
 pyberries/file_utilities/Unpack_omero_folders.py
```

### Comparing `PyBerries-0.2.6/README.md` & `PyBerries-0.2.6.post1/README.md`

 * *Files identical despite different names*

### Comparing `PyBerries-0.2.6/pyberries/File_utilities/Filename_utils.py` & `PyBerries-0.2.6.post1/pyberries/file_utilities/Filename_utils.py`

 * *Files identical despite different names*

### Comparing `PyBerries-0.2.6/pyberries/File_utilities/Stack_tiffs.py` & `PyBerries-0.2.6.post1/pyberries/file_utilities/Stack_tiffs.py`

 * *Files identical despite different names*

### Comparing `PyBerries-0.2.6/pyberries/File_utilities/Unpack_omero_folders.py` & `PyBerries-0.2.6.post1/pyberries/file_utilities/Unpack_omero_folders.py`

 * *Files identical despite different names*

### Comparing `PyBerries-0.2.6/pyberries/Metrics/Metrics.py` & `PyBerries-0.2.6.post1/pyberries/metrics/Metrics.py`

 * *Files identical despite different names*

### Comparing `PyBerries-0.2.6/pyberries/Metrics/Time_metrics.py` & `PyBerries-0.2.6.post1/pyberries/metrics/Time_metrics.py`

 * *Files identical despite different names*

### Comparing `PyBerries-0.2.6/pyberries/Plots/Fits.py` & `PyBerries-0.2.6.post1/pyberries/plots/Fits.py`

 * *Files identical despite different names*

### Comparing `PyBerries-0.2.6/pyberries/Plots/Plot_presets.py` & `PyBerries-0.2.6.post1/pyberries/plots/Plot_presets.py`

 * *Files identical despite different names*

### Comparing `PyBerries-0.2.6/pyberries/Plots/Plots.py` & `PyBerries-0.2.6.post1/pyberries/plots/Plots.py`

 * *Files identical despite different names*

### Comparing `PyBerries-0.2.6/pyberries/data/DatasetPool.py` & `PyBerries-0.2.6.post1/pyberries/data/DatasetPool.py`

 * *Files identical despite different names*

### Comparing `PyBerries-0.2.6/pyberries/data/Fitting.py` & `PyBerries-0.2.6.post1/pyberries/data/Fitting.py`

 * *Files identical despite different names*

### Comparing `PyBerries-0.2.6/pyberries/data/util.py` & `PyBerries-0.2.6.post1/pyberries/data/util.py`

 * *Files identical despite different names*

### Comparing `PyBerries-0.2.6/setup.py` & `PyBerries-0.2.6.post1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="PyBerries",
-    version="0.2.6",
+    version="0.2.6.post1",
     author="Daniel Thedie",
     author_email="daniel.thedie@ed.ac.uk",
     description="Processing of Bacmman measurement tables",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://gitlab.com/MEKlab/pyberries",
     packages=setuptools.find_packages(),
```

