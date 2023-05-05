# Comparing `tmp/MegaFlow2D-0.5.2.tar.gz` & `tmp/MegaFlow2D-0.5.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "MegaFlow2D-0.5.2.tar", last modified: Tue Mar 21 21:14:08 2023, max compression
+gzip compressed data, was "MegaFlow2D-0.5.3.tar", last modified: Fri May  5 17:07:45 2023, max compression
```

## Comparing `MegaFlow2D-0.5.2.tar` & `MegaFlow2D-0.5.3.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0        0        0        0 2023-03-21 21:14:08.304924 MegaFlow2D-0.5.2/
--rw-rw-rw-   0        0        0     1108 2023-01-23 14:53:58.000000 MegaFlow2D-0.5.2/LICENSE
-drwxrwxrwx   0        0        0        0 2023-03-21 21:14:08.285924 MegaFlow2D-0.5.2/MegaFlow2D.egg-info/
--rw-rw-rw-   0        0        0     3867 2023-03-21 21:14:08.000000 MegaFlow2D-0.5.2/MegaFlow2D.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      391 2023-03-21 21:14:08.000000 MegaFlow2D-0.5.2/MegaFlow2D.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-03-21 21:14:08.000000 MegaFlow2D-0.5.2/MegaFlow2D.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      185 2023-03-21 21:14:08.000000 MegaFlow2D-0.5.2/MegaFlow2D.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-03-21 21:14:08.000000 MegaFlow2D-0.5.2/MegaFlow2D.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     3867 2023-03-21 21:14:08.303924 MegaFlow2D-0.5.2/PKG-INFO
--rw-rw-rw-   0        0        0     3261 2023-03-21 18:33:14.000000 MegaFlow2D-0.5.2/README.md
-drwxrwxrwx   0        0        0        0 2023-03-21 21:14:08.286927 MegaFlow2D-0.5.2/megaflow/
--rw-rw-rw-   0        0        0      175 2023-03-21 21:13:12.000000 MegaFlow2D-0.5.2/megaflow/__init__.py
-drwxrwxrwx   0        0        0        0 2023-03-21 21:14:08.300923 MegaFlow2D-0.5.2/megaflow/common/
--rw-rw-rw-   0        0        0        0 2023-01-23 18:34:33.000000 MegaFlow2D-0.5.2/megaflow/common/__init__.py
--rw-rw-rw-   0        0        0      954 2023-01-13 19:03:02.000000 MegaFlow2D-0.5.2/megaflow/common/metrics.py
--rw-rw-rw-   0        0        0     9215 2023-03-21 16:49:03.000000 MegaFlow2D-0.5.2/megaflow/common/utils.py
-drwxrwxrwx   0        0        0        0 2023-03-21 21:14:08.302924 MegaFlow2D-0.5.2/megaflow/dataset/
--rw-rw-rw-   0        0        0     9846 2023-03-21 20:03:54.000000 MegaFlow2D-0.5.2/megaflow/dataset/MegaFlow2D.py
--rw-rw-rw-   0        0        0        0 2023-01-23 16:15:51.000000 MegaFlow2D-0.5.2/megaflow/dataset/__init__.py
--rw-rw-rw-   0        0        0      656 2023-03-21 21:13:12.000000 MegaFlow2D-0.5.2/megaflow/version.py
--rw-rw-rw-   0        0        0       82 2023-01-24 21:15:20.000000 MegaFlow2D-0.5.2/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-03-21 21:14:08.304924 MegaFlow2D-0.5.2/setup.cfg
--rw-rw-rw-   0        0        0     1463 2023-03-20 00:25:16.000000 MegaFlow2D-0.5.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-05 17:07:45.182498 MegaFlow2D-0.5.3/
+-rw-rw-rw-   0        0        0     1108 2023-01-23 14:53:58.000000 MegaFlow2D-0.5.3/LICENSE
+drwxrwxrwx   0        0        0        0 2023-05-05 17:07:45.101865 MegaFlow2D-0.5.3/MegaFlow2D.egg-info/
+-rw-rw-rw-   0        0        0     3867 2023-05-05 17:07:44.000000 MegaFlow2D-0.5.3/MegaFlow2D.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      391 2023-05-05 17:07:44.000000 MegaFlow2D-0.5.3/MegaFlow2D.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-05 17:07:44.000000 MegaFlow2D-0.5.3/MegaFlow2D.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      174 2023-05-05 17:07:44.000000 MegaFlow2D-0.5.3/MegaFlow2D.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-05-05 17:07:44.000000 MegaFlow2D-0.5.3/MegaFlow2D.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     3867 2023-05-05 17:07:45.181497 MegaFlow2D-0.5.3/PKG-INFO
+-rw-rw-rw-   0        0        0     3261 2023-03-21 18:33:14.000000 MegaFlow2D-0.5.3/README.md
+drwxrwxrwx   0        0        0        0 2023-05-05 17:07:45.105864 MegaFlow2D-0.5.3/megaflow/
+-rw-rw-rw-   0        0        0      175 2023-05-05 17:07:15.000000 MegaFlow2D-0.5.3/megaflow/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-05 17:07:45.172183 MegaFlow2D-0.5.3/megaflow/common/
+-rw-rw-rw-   0        0        0        0 2023-01-23 18:34:33.000000 MegaFlow2D-0.5.3/megaflow/common/__init__.py
+-rw-rw-rw-   0        0        0      954 2023-01-13 19:03:02.000000 MegaFlow2D-0.5.3/megaflow/common/metrics.py
+-rw-rw-rw-   0        0        0     9215 2023-03-21 16:49:03.000000 MegaFlow2D-0.5.3/megaflow/common/utils.py
+drwxrwxrwx   0        0        0        0 2023-05-05 17:07:45.180497 MegaFlow2D-0.5.3/megaflow/dataset/
+-rw-rw-rw-   0        0        0    10340 2023-03-27 15:10:46.000000 MegaFlow2D-0.5.3/megaflow/dataset/MegaFlow2D.py
+-rw-rw-rw-   0        0        0        0 2023-01-23 16:15:51.000000 MegaFlow2D-0.5.3/megaflow/dataset/__init__.py
+-rw-rw-rw-   0        0        0      656 2023-05-05 17:07:15.000000 MegaFlow2D-0.5.3/megaflow/version.py
+-rw-rw-rw-   0        0        0       82 2023-01-24 21:15:20.000000 MegaFlow2D-0.5.3/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-05 17:07:45.182498 MegaFlow2D-0.5.3/setup.cfg
+-rw-rw-rw-   0        0        0     1442 2023-05-05 15:21:27.000000 MegaFlow2D-0.5.3/setup.py
```

### Comparing `MegaFlow2D-0.5.2/LICENSE` & `MegaFlow2D-0.5.3/LICENSE`

 * *Files identical despite different names*

### Comparing `MegaFlow2D-0.5.2/MegaFlow2D.egg-info/PKG-INFO` & `MegaFlow2D-0.5.3/MegaFlow2D.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: MegaFlow2D
-Version: 0.5.2
+Version: 0.5.3
 Summary: MegaFlow2D: A Large-Scale Dataset for 2D Flow Simulation
 Home-page: https://github.com/cmudrc/MegaFlow2D
 Author: Wenzhuo Xu, Noelia Grande Gutierrez and Christopher McComb
 Author-email: wxu2@andrew.cmu.edu
 License: MIT
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Intended Audience :: Science/Research
```

### Comparing `MegaFlow2D-0.5.2/PKG-INFO` & `MegaFlow2D-0.5.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: MegaFlow2D
-Version: 0.5.2
+Version: 0.5.3
 Summary: MegaFlow2D: A Large-Scale Dataset for 2D Flow Simulation
 Home-page: https://github.com/cmudrc/MegaFlow2D
 Author: Wenzhuo Xu, Noelia Grande Gutierrez and Christopher McComb
 Author-email: wxu2@andrew.cmu.edu
 License: MIT
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Intended Audience :: Science/Research
```

### Comparing `MegaFlow2D-0.5.2/README.md` & `MegaFlow2D-0.5.3/README.md`

 * *Files identical despite different names*

### Comparing `MegaFlow2D-0.5.2/megaflow/common/metrics.py` & `MegaFlow2D-0.5.3/megaflow/common/metrics.py`

 * *Files identical despite different names*

### Comparing `MegaFlow2D-0.5.2/megaflow/common/utils.py` & `MegaFlow2D-0.5.3/megaflow/common/utils.py`

 * *Files identical despite different names*

### Comparing `MegaFlow2D-0.5.2/megaflow/dataset/MegaFlow2D.py` & `MegaFlow2D-0.5.3/megaflow/dataset/MegaFlow2D.py`

 * *Files 4% similar despite different names*

```diff
@@ -153,21 +153,22 @@
         output_file = os.path.join(self.processed_dir, 'data.h5')
         # output_file_has = os.path.join(self.processed_has_data_dir, 'data.h5')
         merge_hdf5_files(input_files=input_file, output_file=output_file)
         # self.merge_hdf5_files(input_file_has, output_file_has)
         # redo data list
         
     def transform(self, data):
+        (data_l, data_h) = data
         if self.transforms == 'error_estimation':
-            data.y = data.y - data.x
+            data_l.y = data_l.y - data_l.x
         if self.transforms == 'normalize':
             # normalize the data layer-wise via gaussian distribution
-            data.x = (data.x - data.x.mean(dim=0)) / (data.x.std(dim=0) + 1e-8)
-            data.y = (data.y - data.x.mean(dim=0)) / (data.x.std(dim=0) + 1e-8)
-        return data
+            data_l.x = (data_l.x - data_l.x.mean(dim=0)) / (data_l.x.std(dim=0) + 1e-8)
+            data_h.x = (data_h.y - data_l.x.mean(dim=0)) / (data_l.x.std(dim=0) + 1e-8)
+        return (data_l, data_h)
 
     def get(self, idx):
         data_name = self.data_list[idx]
         str1, str2, str3 = data_name.split('_')
         mesh_name = str1 + '_' + str2
         with h5py.File(os.path.join(self.processed_dir, 'data.h5'), 'r') as f:
             grp = f[mesh_name]
@@ -201,22 +202,30 @@
             data_l = data_l if self.transform is None else self.transform(data_l)
             return (data_l, data_h)
 
         else:
             return self.index_select(idx)
 
     def get_eval(self, idx):
-        # same as get, but returns data name as well
-        data = torch.load(os.path.join(self.processed_dir, self.data_list[idx]))
-        str1, str2, str4 = self.data_list[idx].split('_')
-        data_name = str1 + '_' + str2 + '_' + str4
-
-        if self.transform is not None:
-            data = self.transform(data)
-        return data, data_name
+        data_name = self.data_list[idx]
+        str1, str2, str3 = data_name.split('_')
+        mesh_name = str1 + '_' + str2
+        with h5py.File(os.path.join(self.processed_dir, 'data.h5'), 'r') as f:
+            grp = f[mesh_name]
+            grp_time = grp[str3]
+            grp_las = grp_time['las']
+            grp_has = grp_time['has']
+            las_data_dict = {key: torch.tensor(grp_las[key][:]) for key in grp_las.keys()}
+            has_data_dict = {key: torch.tensor(grp_has[key][:]) for key in grp_has.keys()}
+            data_l = Data.from_dict(las_data_dict)
+            data_h = Data.from_dict(has_data_dict)
+        # if self.transforms is not None:
+        #     data_l = self.transform(data_l)
+            
+        return data_name, (data_l, data_h)
 
 
 class MegaFlow2DSubset(MegaFlow2D):
     """
     This subset splits the entire dataset into 40 subsets, which is initialized via indices.
     """
     def __init__(self, root, indices, transform=None):
```

### Comparing `MegaFlow2D-0.5.2/megaflow/version.py` & `MegaFlow2D-0.5.3/megaflow/version.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 import os
 import logging
 from threading import Thread
 
-__version__ = '0.5.2'
+__version__ = '0.5.3'
 
 try:
     os.environ['OUTDATED_IGNORE'] = '1'
     from outdated import check_outdated  # noqa
 except ImportError:
     check_outdated = None
```

### Comparing `MegaFlow2D-0.5.2/setup.py` & `MegaFlow2D-0.5.3/setup.py`

 * *Files 3% similar despite different names*

```diff
@@ -17,31 +17,30 @@
     author="Wenzhuo Xu, Noelia Grande Gutierrez and Christopher McComb",
     author_email="wxu2@andrew.cmu.edu",
     url="https://github.com/cmudrc/MegaFlow2D",
     description="MegaFlow2D: A Large-Scale Dataset for 2D Flow Simulation",
     long_description=long_description,
     long_description_content_type="text/markdown",
     install_requires = [
+        'h5py>=2.10.0',
         'numpy>=1.19.1',
         'ogb>=1.2.6',
         'outdated>=0.2.0',
         'pandas>=1.1.0',
         'pillow>=7.2.0',
-        'ogb>=1.2.6',
         'pytz>=2020.4',
+        'scikit-learn>=0.20.0',
+        'scipy>=1.5.4',
         'torch>=1.7.0',
         'torchvision>=0.8.2',
         'tqdm>=4.53.0',
-        'scikit-learn>=0.20.0',
-        'scipy>=1.5.4',
-        'h5py>=2.10.0',
     ],
     license='MIT',
     packages=setuptools.find_packages(exclude=['examples', 'examples.model']),
     classifiers=[
         'Topic :: Scientific/Engineering :: Artificial Intelligence',
         'Intended Audience :: Science/Research',
         "Programming Language :: Python :: 3",
         "License :: OSI Approved :: MIT License",
     ],
     python_requires='>=3.6',
-)
+)
```

