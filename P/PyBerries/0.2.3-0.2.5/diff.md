# Comparing `tmp/PyBerries-0.2.3.tar.gz` & `tmp/PyBerries-0.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PyBerries-0.2.3.tar", last modified: Thu May  4 12:43:29 2023, max compression
+gzip compressed data, was "PyBerries-0.2.5.tar", last modified: Thu May  4 16:19:05 2023, max compression
```

## Comparing `PyBerries-0.2.3.tar` & `PyBerries-0.2.5.tar`

### file list

```diff
@@ -1,34 +1,33 @@
-drwxrwxrwx   0        0        0        0 2023-05-04 12:43:29.310075 PyBerries-0.2.3/
--rw-rw-rw-   0        0        0    33074 2022-12-22 10:37:47.000000 PyBerries-0.2.3/LICENSE
--rw-rw-rw-   0        0        0    14421 2023-05-04 12:43:29.308076 PyBerries-0.2.3/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-05-04 12:43:29.275576 PyBerries-0.2.3/PyBerries.egg-info/
--rw-rw-rw-   0        0        0    14421 2023-05-04 12:43:29.000000 PyBerries-0.2.3/PyBerries.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1062 2023-05-04 12:43:29.000000 PyBerries-0.2.3/PyBerries.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-04 12:43:29.000000 PyBerries-0.2.3/PyBerries.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       70 2023-05-04 12:43:29.000000 PyBerries-0.2.3/PyBerries.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-05-04 12:43:29.000000 PyBerries-0.2.3/PyBerries.egg-info/top_level.txt
--rw-rw-rw-   0        0        0    14103 2023-05-03 12:45:51.000000 PyBerries-0.2.3/README.md
-drwxrwxrwx   0        0        0        0 2023-05-04 12:43:29.276576 PyBerries-0.2.3/pyberries/
-drwxrwxrwx   0        0        0        0 2023-05-04 12:43:29.284576 PyBerries-0.2.3/pyberries/File_utilities/
--rw-rw-rw-   0        0        0     2877 2023-03-14 14:43:41.000000 PyBerries-0.2.3/pyberries/File_utilities/Filename_utils.py
--rw-rw-rw-   0        0        0     2782 2023-03-14 14:14:07.000000 PyBerries-0.2.3/pyberries/File_utilities/Stack_tiffs.py
--rw-rw-rw-   0        0        0      795 2023-03-14 14:14:07.000000 PyBerries-0.2.3/pyberries/File_utilities/Unpack_omero_folders.py
--rw-rw-rw-   0        0        0      119 2023-03-14 14:14:07.000000 PyBerries-0.2.3/pyberries/File_utilities/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-04 12:43:29.288576 PyBerries-0.2.3/pyberries/Metrics/
--rw-rw-rw-   0        0        0     1242 2023-05-02 10:54:16.000000 PyBerries-0.2.3/pyberries/Metrics/Metrics.py
--rw-rw-rw-   0        0        0     6475 2023-05-03 12:50:51.000000 PyBerries-0.2.3/pyberries/Metrics/Time_metrics.py
--rw-rw-rw-   0        0        0       69 2023-03-10 16:15:28.000000 PyBerries-0.2.3/pyberries/Metrics/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-04 12:43:29.307079 PyBerries-0.2.3/pyberries/Plots/
--rw-rw-rw-   0        0        0     1037 2023-05-02 16:02:09.000000 PyBerries-0.2.3/pyberries/Plots/Fits.py
--rw-rw-rw-   0        0        0     4813 2023-05-04 10:28:45.000000 PyBerries-0.2.3/pyberries/Plots/Plot_presets.py
--rw-rw-rw-   0        0        0      353 2023-04-05 10:31:09.000000 PyBerries-0.2.3/pyberries/Plots/Plot_utilities.py
--rw-rw-rw-   0        0        0     1372 2023-04-03 13:51:01.000000 PyBerries-0.2.3/pyberries/Plots/Plots.py
--rw-rw-rw-   0        0        0      117 2023-05-02 10:54:16.000000 PyBerries-0.2.3/pyberries/Plots/__init__.py
--rw-rw-rw-   0        0        0      118 2023-05-02 10:54:16.000000 PyBerries-0.2.3/pyberries/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-04 12:43:29.299579 PyBerries-0.2.3/pyberries/data/
--rw-rw-rw-   0        0        0    16099 2023-05-04 10:24:24.000000 PyBerries-0.2.3/pyberries/data/DatasetPool.py
--rw-rw-rw-   0        0        0     1886 2023-05-04 10:56:45.000000 PyBerries-0.2.3/pyberries/data/Fitting.py
--rw-rw-rw-   0        0        0       86 2023-05-02 15:00:14.000000 PyBerries-0.2.3/pyberries/data/__init__.py
--rw-rw-rw-   0        0        0     1567 2023-05-02 15:50:42.000000 PyBerries-0.2.3/pyberries/data/util.py
--rw-rw-rw-   0        0        0       42 2023-05-04 12:43:29.310075 PyBerries-0.2.3/setup.cfg
--rw-rw-rw-   0        0        0      625 2023-05-04 12:40:58.000000 PyBerries-0.2.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-04 16:19:05.164798 PyBerries-0.2.5/
+-rw-rw-rw-   0        0        0    33074 2022-12-22 10:37:47.000000 PyBerries-0.2.5/LICENSE
+-rw-rw-rw-   0        0        0    14421 2023-05-04 16:19:05.163794 PyBerries-0.2.5/PKG-INFO
+-rw-rw-rw-   0        0        0    14103 2023-05-03 12:45:51.000000 PyBerries-0.2.5/README.md
+drwxrwxrwx   0        0        0        0 2023-05-04 16:19:05.116791 PyBerries-0.2.5/pyberries/
+drwxrwxrwx   0        0        0        0 2023-05-04 16:19:05.132793 PyBerries-0.2.5/pyberries/PyBerries.egg-info/
+-rw-rw-rw-   0        0        0    14421 2023-05-04 16:19:05.000000 PyBerries-0.2.5/pyberries/PyBerries.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      751 2023-05-04 16:19:05.000000 PyBerries-0.2.5/pyberries/PyBerries.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-04 16:19:05.000000 PyBerries-0.2.5/pyberries/PyBerries.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       70 2023-05-04 16:19:05.000000 PyBerries-0.2.5/pyberries/PyBerries.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       34 2023-05-04 16:19:05.000000 PyBerries-0.2.5/pyberries/PyBerries.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-04 16:19:05.139799 PyBerries-0.2.5/pyberries/data/
+-rw-rw-rw-   0        0        0    16096 2023-05-04 16:04:58.000000 PyBerries-0.2.5/pyberries/data/DatasetPool.py
+-rw-rw-rw-   0        0        0     1886 2023-05-04 10:56:45.000000 PyBerries-0.2.5/pyberries/data/Fitting.py
+-rw-rw-rw-   0        0        0       86 2023-05-02 15:00:14.000000 PyBerries-0.2.5/pyberries/data/__init__.py
+-rw-rw-rw-   0        0        0     1567 2023-05-02 15:50:42.000000 PyBerries-0.2.5/pyberries/data/util.py
+drwxrwxrwx   0        0        0        0 2023-05-04 16:19:05.147799 PyBerries-0.2.5/pyberries/file_utilities/
+-rw-rw-rw-   0        0        0     2877 2023-03-14 14:43:41.000000 PyBerries-0.2.5/pyberries/file_utilities/Filename_utils.py
+-rw-rw-rw-   0        0        0     2782 2023-03-14 14:14:07.000000 PyBerries-0.2.5/pyberries/file_utilities/Stack_tiffs.py
+-rw-rw-rw-   0        0        0      795 2023-03-14 14:14:07.000000 PyBerries-0.2.5/pyberries/file_utilities/Unpack_omero_folders.py
+-rw-rw-rw-   0        0        0      119 2023-03-14 14:14:07.000000 PyBerries-0.2.5/pyberries/file_utilities/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-04 16:19:05.151791 PyBerries-0.2.5/pyberries/metrics/
+-rw-rw-rw-   0        0        0     1242 2023-05-02 10:54:16.000000 PyBerries-0.2.5/pyberries/metrics/Metrics.py
+-rw-rw-rw-   0        0        0     6475 2023-05-03 12:50:51.000000 PyBerries-0.2.5/pyberries/metrics/Time_metrics.py
+-rw-rw-rw-   0        0        0       69 2023-03-10 16:15:28.000000 PyBerries-0.2.5/pyberries/metrics/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-04 16:19:05.161795 PyBerries-0.2.5/pyberries/plots/
+-rw-rw-rw-   0        0        0     1037 2023-05-02 16:02:09.000000 PyBerries-0.2.5/pyberries/plots/Fits.py
+-rw-rw-rw-   0        0        0     4813 2023-05-04 10:28:45.000000 PyBerries-0.2.5/pyberries/plots/Plot_presets.py
+-rw-rw-rw-   0        0        0      353 2023-04-05 10:31:09.000000 PyBerries-0.2.5/pyberries/plots/Plot_utilities.py
+-rw-rw-rw-   0        0        0     1372 2023-04-03 13:51:01.000000 PyBerries-0.2.5/pyberries/plots/Plots.py
+-rw-rw-rw-   0        0        0      117 2023-05-02 10:54:16.000000 PyBerries-0.2.5/pyberries/plots/__init__.py
+-rw-rw-rw-   0        0        0       42 2023-05-04 16:19:05.165792 PyBerries-0.2.5/setup.cfg
+-rw-rw-rw-   0        0        0      678 2023-05-04 16:18:50.000000 PyBerries-0.2.5/setup.py
```

### Comparing `PyBerries-0.2.3/LICENSE` & `PyBerries-0.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `PyBerries-0.2.3/PKG-INFO` & `PyBerries-0.2.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyBerries
-Version: 0.2.3
+Version: 0.2.5
 Summary: Processing of Bacmman measurement tables
 Home-page: https://gitlab.com/MEKlab/pyberries
 Author: Daniel Thedie
 Author-email: daniel.thedie@ed.ac.uk
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `PyBerries-0.2.3/PyBerries.egg-info/PKG-INFO` & `PyBerries-0.2.5/pyberries/PyBerries.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyBerries
-Version: 0.2.3
+Version: 0.2.5
 Summary: Processing of Bacmman measurement tables
 Home-page: https://gitlab.com/MEKlab/pyberries
 Author: Daniel Thedie
 Author-email: daniel.thedie@ed.ac.uk
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 License-File: LICENSE
```

### Comparing `PyBerries-0.2.3/README.md` & `PyBerries-0.2.5/README.md`

 * *Files identical despite different names*

### Comparing `PyBerries-0.2.3/pyberries/File_utilities/Filename_utils.py` & `PyBerries-0.2.5/pyberries/file_utilities/Filename_utils.py`

 * *Files identical despite different names*

### Comparing `PyBerries-0.2.3/pyberries/File_utilities/Stack_tiffs.py` & `PyBerries-0.2.5/pyberries/file_utilities/Stack_tiffs.py`

 * *Files identical despite different names*

### Comparing `PyBerries-0.2.3/pyberries/File_utilities/Unpack_omero_folders.py` & `PyBerries-0.2.5/pyberries/file_utilities/Unpack_omero_folders.py`

 * *Files identical despite different names*

### Comparing `PyBerries-0.2.3/pyberries/Metrics/Metrics.py` & `PyBerries-0.2.5/pyberries/metrics/Metrics.py`

 * *Files identical despite different names*

### Comparing `PyBerries-0.2.3/pyberries/Metrics/Time_metrics.py` & `PyBerries-0.2.5/pyberries/metrics/Time_metrics.py`

 * *Files identical despite different names*

### Comparing `PyBerries-0.2.3/pyberries/Plots/Fits.py` & `PyBerries-0.2.5/pyberries/plots/Fits.py`

 * *Files identical despite different names*

### Comparing `PyBerries-0.2.3/pyberries/Plots/Plot_presets.py` & `PyBerries-0.2.5/pyberries/plots/Plot_presets.py`

 * *Files identical despite different names*

### Comparing `PyBerries-0.2.3/pyberries/Plots/Plots.py` & `PyBerries-0.2.5/pyberries/plots/Plots.py`

 * *Files identical despite different names*

### Comparing `PyBerries-0.2.3/pyberries/data/DatasetPool.py` & `PyBerries-0.2.5/pyberries/data/DatasetPool.py`

 * *Files 0% similar despite different names*

```diff
@@ -118,15 +118,15 @@
                     if var == 'DateTime':
                         df['TimeDelta'] = 0
                         df['Time_min'] = 0
                     for i, ds in enumerate(self.dsList):
                         ds_path = self.path[0] if len(self.path) == 1 else self.path[i]
                         for pos in df.loc[df['Dataset'] == ds].Position.unique():
                             # Open metadata file
-                            with open(join(ds_path, ds, 'SourceImageMetadata', f'{pos}_c{channel}_t0.txt')) as f:
+                            with open(join(ds_path, ds, 'SourceImageMetadata', f'{pos}_c{channel}.txt')) as f:
                                 value = next((line for line in f if var in line), None)
                                 # Add metadata value to the current dataset and position
                                 df.loc[(df['Position'] == pos) & (df['Dataset'] == ds), var.replace(' ', '_')] = value.split('=')[-1][:-1] # Remove line break (last character)
                         if 'DateTime' in df.columns:
                             df.loc[df['Dataset'] == ds] = (df.loc[df['Dataset'] == ds]
                                                             .assign(DateTime = lambda df: pd.to_datetime(df.DateTime, format='%Y%m%d %H:%M:%S.%f'),
                                                                     TimeDelta = lambda df: df.DateTime - df.DateTime.iloc[0],
```

### Comparing `PyBerries-0.2.3/pyberries/data/Fitting.py` & `PyBerries-0.2.5/pyberries/data/Fitting.py`

 * *Files identical despite different names*

### Comparing `PyBerries-0.2.3/pyberries/data/util.py` & `PyBerries-0.2.5/pyberries/data/util.py`

 * *Files identical despite different names*

### Comparing `PyBerries-0.2.3/setup.py` & `PyBerries-0.2.5/setup.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="PyBerries",
-    version="0.2.3",
+    version="0.2.5",
     author="Daniel Thedie",
     author_email="daniel.thedie@ed.ac.uk",
     description="Processing of Bacmman measurement tables",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://gitlab.com/MEKlab/pyberries",
-    packages=setuptools.find_packages(),
+    packages=setuptools.find_packages(where='pyberries'),
+    package_dir={"": "pyberries"},
     python_requires='>=3.8',
     install_requires=['numpy', 'scipy', 'pandas', 'matplotlib', 'tifffile', 'h5py','seaborn', 'pybacmman', 'IPython']
 )
```

