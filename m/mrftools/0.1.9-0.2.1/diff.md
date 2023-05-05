# Comparing `tmp/mrftools-0.1.9.tar.gz` & `tmp/mrftools-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mrftools-0.1.9.tar", last modified: Thu Oct  6 13:33:14 2022, max compression
+gzip compressed data, was "mrftools-0.2.1.tar", last modified: Mon Mar 20 14:03:44 2023, max compression
```

## Comparing `mrftools-0.1.9.tar` & `mrftools-0.2.1.tar`

### file list

```diff
@@ -1,25 +1,67 @@
-drwxr-sr-x   0 jovyan    (1000) users      (100)        0 2022-10-06 13:33:14.040215 mrftools-0.1.9/
--rw-r--r--   0 jovyan    (1000) users      (100)    35148 2022-10-06 11:24:25.000000 mrftools-0.1.9/LICENSE
--rw-r--r--   0 jovyan    (1000) users      (100)     1991 2022-10-06 13:33:14.040215 mrftools-0.1.9/PKG-INFO
--rw-r--r--   0 jovyan    (1000) users      (100)     1568 2022-10-06 11:24:25.000000 mrftools-0.1.9/README.md
--rw-r--r--   0 jovyan    (1000) users      (100)       38 2022-10-06 13:33:14.040215 mrftools-0.1.9/setup.cfg
--rw-r--r--   0 jovyan    (1000) users      (100)      833 2022-10-06 13:32:54.000000 mrftools-0.1.9/setup.py
-drwxr-sr-x   0 jovyan    (1000) users      (100)        0 2022-10-06 13:33:14.036215 mrftools-0.1.9/src/
-drwxr-sr-x   0 jovyan    (1000) users      (100)        0 2022-10-06 13:33:14.040215 mrftools-0.1.9/src/mrftools/
--rw-r--r--   0 jovyan    (1000) users      (100)      346 2022-10-06 11:50:28.000000 mrftools-0.1.9/src/mrftools/__init__.py
--rw-r--r--   0 jovyan    (1000) users      (100)     4615 2022-10-06 12:37:33.000000 mrftools-0.1.9/src/mrftools/datasets.py
--rw-r--r--   0 jovyan    (1000) users      (100)     7349 2022-10-06 11:24:25.000000 mrftools-0.1.9/src/mrftools/dictionaryParameters.py
--rw-r--r--   0 jovyan    (1000) users      (100)     8073 2022-10-06 11:24:25.000000 mrftools-0.1.9/src/mrftools/phantomGenerators.py
--rw-r--r--   0 jovyan    (1000) users      (100)     2204 2022-10-06 11:24:25.000000 mrftools-0.1.9/src/mrftools/sequenceGenerators.py
--rw-r--r--   0 jovyan    (1000) users      (100)     4510 2022-10-06 11:24:25.000000 mrftools-0.1.9/src/mrftools/sequenceParameters.py
--rw-r--r--   0 jovyan    (1000) users      (100)    12809 2022-10-06 11:24:25.000000 mrftools-0.1.9/src/mrftools/simulation.py
--rw-r--r--   0 jovyan    (1000) users      (100)     3612 2022-10-06 13:21:29.000000 mrftools-0.1.9/src/mrftools/synthetics.py
--rw-r--r--   0 jovyan    (1000) users      (100)     1379 2022-10-06 11:24:25.000000 mrftools-0.1.9/src/mrftools/testing.py
--rw-r--r--   0 jovyan    (1000) users      (100)   348639 2022-10-06 11:41:18.000000 mrftools-0.1.9/src/mrftools/types.py
-drwxr-sr-x   0 jovyan    (1000) users      (100)        0 2022-10-06 13:33:14.040215 mrftools-0.1.9/src/mrftools.egg-info/
--rw-r--r--   0 jovyan    (1000) users      (100)     1991 2022-10-06 13:33:14.000000 mrftools-0.1.9/src/mrftools.egg-info/PKG-INFO
--rw-r--r--   0 jovyan    (1000) users      (100)      531 2022-10-06 13:33:14.000000 mrftools-0.1.9/src/mrftools.egg-info/SOURCES.txt
--rw-r--r--   0 jovyan    (1000) users      (100)        1 2022-10-06 13:33:14.000000 mrftools-0.1.9/src/mrftools.egg-info/dependency_links.txt
--rw-r--r--   0 jovyan    (1000) users      (100)        1 2022-10-06 11:51:06.000000 mrftools-0.1.9/src/mrftools.egg-info/not-zip-safe
--rw-r--r--   0 jovyan    (1000) users      (100)       28 2022-10-06 13:33:14.000000 mrftools-0.1.9/src/mrftools.egg-info/requires.txt
--rw-r--r--   0 jovyan    (1000) users      (100)        9 2022-10-06 13:33:14.000000 mrftools-0.1.9/src/mrftools.egg-info/top_level.txt
+drwxrwxr-x   0 andrew    (1000) andrew    (1000)        0 2023-03-20 14:03:44.488076 mrftools-0.2.1/
+drwxrwxr-x   0 andrew    (1000) andrew    (1000)        0 2023-03-20 14:03:44.436076 mrftools-0.2.1/.devcontainer/
+-rw-rw-r--   0 andrew    (1000) andrew    (1000)      637 2022-10-19 13:19:53.000000 mrftools-0.2.1/.devcontainer/Dockerfile
+-rw-rw-r--   0 andrew    (1000) andrew    (1000)      429 2022-10-19 13:45:59.000000 mrftools-0.2.1/.devcontainer/devcontainer.json
+-rw-rw-r--   0 andrew    (1000) andrew    (1000)     3078 2022-09-27 09:37:53.000000 mrftools-0.2.1/.gitignore
+-rw-rw-r--   0 andrew    (1000) andrew    (1000)    35148 2022-09-27 09:37:53.000000 mrftools-0.2.1/LICENSE
+-rw-rw-r--   0 andrew    (1000) andrew    (1000)     1955 2023-03-20 14:03:44.488076 mrftools-0.2.1/PKG-INFO
+-rw-rw-r--   0 andrew    (1000) andrew    (1000)     1568 2022-09-27 09:37:53.000000 mrftools-0.2.1/README.md
+drwxrwxr-x   0 andrew    (1000) andrew    (1000)        0 2023-03-20 14:03:44.452076 mrftools-0.2.1/examples/
+-rw-rw-r--   0 andrew    (1000) andrew    (1000)    55040 2022-12-14 21:13:35.000000 mrftools-0.2.1/examples/Experimental.ipynb
+-rw-rw-r--   0 andrew    (1000) andrew    (1000)    16406 2023-02-27 19:00:03.000000 mrftools-0.2.1/examples/JsonTests.ipynb
+-rw-rw-r--   0 andrew    (1000) andrew    (1000)  1178964 2022-12-14 21:13:35.000000 mrftools-0.2.1/examples/NIFTIDatasets.ipynb
+-rw-rw-r--   0 andrew    (1000) andrew    (1000)     2583 2022-09-27 09:37:53.000000 mrftools-0.2.1/examples/PatternMatching.ipynb
+-rw-rw-r--   0 andrew    (1000) andrew    (1000)   198573 2022-09-27 09:37:53.000000 mrftools-0.2.1/examples/PhantomGeneration.ipynb
+-rw-rw-r--   0 andrew    (1000) andrew    (1000)  1266078 2023-02-24 21:37:04.000000 mrftools-0.2.1/examples/Samples.ipynb
+-rw-rw-r--   0 andrew    (1000) andrew    (1000)   246929 2023-02-28 18:37:45.000000 mrftools-0.2.1/examples/YongMyelinWaterFraction_dev.sequence
+-rw-rw-r--   0 andrew    (1000) andrew    (1000)   308108 2023-03-01 18:22:46.000000 mrftools-0.2.1/examples/YongSequenceTests.ipynb
+-rw-rw-r--   0 andrew    (1000) andrew    (1000)   249182 2023-02-28 18:41:27.000000 mrftools-0.2.1/examples/YongSequenceTests.pdf
+-rw-rw-r--   0 andrew    (1000) andrew    (1000)   124106 2023-03-20 13:43:44.000000 mrftools-0.2.1/examples/YuranMRFTest_dev.sequence
+-rw-rw-r--   0 andrew    (1000) andrew    (1000)   705005 2023-03-20 13:43:41.000000 mrftools-0.2.1/examples/YuranTestSequence.ipynb
+-rw-rw-r--   0 andrew    (1000) andrew    (1000)   524483 2023-03-20 13:43:40.000000 mrftools-0.2.1/examples/YuranTestSequence.pdf
+drwxrwxr-x   0 andrew    (1000) andrew    (1000)        0 2023-03-20 14:03:44.452076 mrftools-0.2.1/examples/fisp/
+-rw-rw-r--   0 andrew    (1000) andrew    (1000)    20369 2023-02-20 14:36:35.000000 mrftools-0.2.1/examples/fisp/FAs.txt
+-rw-rw-r--   0 andrew    (1000) andrew    (1000)       31 2023-02-20 14:36:35.000000 mrftools-0.2.1/examples/fisp/PrepIDs.txt
+-rw-rw-r--   0 andrew    (1000) andrew    (1000)       94 2023-02-20 14:36:35.000000 mrftools-0.2.1/examples/fisp/PrepTimes.txt
+-rw-rw-r--   0 andrew    (1000) andrew    (1000)      287 2023-02-20 14:36:35.000000 mrftools-0.2.1/examples/fisp/RRTimes.txt
+-rw-rw-r--   0 andrew    (1000) andrew    (1000)    30719 2023-02-20 14:36:35.000000 mrftools-0.2.1/examples/fisp/TEs.txt
+-rw-rw-r--   0 andrew    (1000) andrew    (1000)    23039 2023-02-20 14:36:35.000000 mrftools-0.2.1/examples/fisp/TRs.txt
+-rw-rw-r--   0 andrew    (1000) andrew    (1000)      140 2023-02-20 14:36:35.000000 mrftools-0.2.1/examples/fisp/TenPctDict_B1s.txt
+-rw-rw-r--   0 andrew    (1000) andrew    (1000)    17346 2023-02-20 14:36:35.000000 mrftools-0.2.1/examples/fisp/TenPctDict_T1s.txt
+-rw-rw-r--   0 andrew    (1000) andrew    (1000)    16464 2023-02-20 14:36:35.000000 mrftools-0.2.1/examples/fisp/TenPctDict_T2s.txt
+drwxrwxr-x   0 andrew    (1000) andrew    (1000)        0 2023-03-20 14:03:44.452076 mrftools-0.2.1/examples/testdata/
+-rw-rw-r--   0 andrew    (1000) andrew    (1000)  5814644 2022-09-27 09:37:53.000000 mrftools-0.2.1/examples/testdata/test.mrf
+drwxrwxr-x   0 andrew    (1000) andrew    (1000)        0 2023-03-20 14:03:44.480076 mrftools-0.2.1/examples/testdata/txt/
+-rw-rw-r--   0 andrew    (1000) andrew    (1000)     5320 2022-09-27 09:37:53.000000 mrftools-0.2.1/examples/testdata/txt/testDict_T1s.txt
+-rw-rw-r--   0 andrew    (1000) andrew    (1000)     5320 2022-09-27 09:37:53.000000 mrftools-0.2.1/examples/testdata/txt/testDict_T2s.txt
+-rw-rw-r--   0 andrew    (1000) andrew    (1000)     4266 2022-09-27 09:37:53.000000 mrftools-0.2.1/examples/testdata/txt/testSeq_FAs.txt
+-rw-rw-r--   0 andrew    (1000) andrew    (1000)     4000 2022-09-27 09:37:53.000000 mrftools-0.2.1/examples/testdata/txt/testSeq_TEs.txt
+-rw-rw-r--   0 andrew    (1000) andrew    (1000)     4000 2022-09-27 09:37:53.000000 mrftools-0.2.1/examples/testdata/txt/testSeq_TRs.txt
+-rw-rw-r--   0 andrew    (1000) andrew    (1000)      154 2022-12-14 20:23:59.000000 mrftools-0.2.1/requirements.txt
+-rw-rw-r--   0 andrew    (1000) andrew    (1000)       38 2023-03-20 14:03:44.488076 mrftools-0.2.1/setup.cfg
+-rw-rw-r--   0 andrew    (1000) andrew    (1000)      990 2023-02-27 16:58:30.000000 mrftools-0.2.1/setup.py
+drwxrwxr-x   0 andrew    (1000) andrew    (1000)        0 2023-03-20 14:03:44.436076 mrftools-0.2.1/src/
+drwxrwxr-x   0 andrew    (1000) andrew    (1000)        0 2023-03-20 14:03:44.484076 mrftools-0.2.1/src/mrftools/
+-rw-rw-r--   0 andrew    (1000) andrew    (1000)      571 2023-02-27 16:58:18.000000 mrftools-0.2.1/src/mrftools/__init__.py
+-rw-rw-r--   0 andrew    (1000) andrew    (1000)      827 2022-12-14 21:13:35.000000 mrftools-0.2.1/src/mrftools/clustering.py
+-rw-rw-r--   0 andrew    (1000) andrew    (1000)     7939 2022-12-13 19:24:41.000000 mrftools-0.2.1/src/mrftools/coilCombination.py
+-rw-rw-r--   0 andrew    (1000) andrew    (1000)     8542 2022-12-14 20:27:50.000000 mrftools-0.2.1/src/mrftools/datasets.py
+-rw-rw-r--   0 andrew    (1000) andrew    (1000)     7773 2023-02-27 16:27:59.000000 mrftools-0.2.1/src/mrftools/dictionaryParameters.py
+-rw-rw-r--   0 andrew    (1000) andrew    (1000)     4656 2022-12-13 14:45:39.000000 mrftools-0.2.1/src/mrftools/ismrmrdQuaternionHelper.py
+-rw-rw-r--   0 andrew    (1000) andrew    (1000)     4502 2022-12-14 21:24:13.000000 mrftools-0.2.1/src/mrftools/kmeans.py
+-rw-rw-r--   0 andrew    (1000) andrew    (1000)     8073 2023-02-27 16:27:56.000000 mrftools-0.2.1/src/mrftools/phantomGenerators.py
+-rw-rw-r--   0 andrew    (1000) andrew    (1000)    19607 2023-02-27 16:22:25.000000 mrftools-0.2.1/src/mrftools/reconstruction.py
+-rw-rw-r--   0 andrew    (1000) andrew    (1000)     2371 2022-10-13 12:07:44.000000 mrftools-0.2.1/src/mrftools/registration.py
+-rw-rw-r--   0 andrew    (1000) andrew    (1000)     5007 2023-02-27 22:17:24.000000 mrftools-0.2.1/src/mrftools/sequenceGenerators.py
+-rw-rw-r--   0 andrew    (1000) andrew    (1000)    45923 2023-03-20 13:39:34.000000 mrftools-0.2.1/src/mrftools/sequenceParameters.py
+-rw-rw-r--   0 andrew    (1000) andrew    (1000)    11459 2023-03-01 17:43:59.000000 mrftools-0.2.1/src/mrftools/simulation.py
+-rw-rw-r--   0 andrew    (1000) andrew    (1000)    11774 2023-02-20 14:36:35.000000 mrftools-0.2.1/src/mrftools/synthetics.py
+-rw-rw-r--   0 andrew    (1000) andrew    (1000)     1379 2022-09-27 09:37:53.000000 mrftools-0.2.1/src/mrftools/testing.py
+-rw-rw-r--   0 andrew    (1000) andrew    (1000)   353789 2023-02-28 18:33:15.000000 mrftools-0.2.1/src/mrftools/types.py
+drwxrwxr-x   0 andrew    (1000) andrew    (1000)        0 2023-03-20 14:03:44.488076 mrftools-0.2.1/src/mrftools.egg-info/
+-rw-rw-r--   0 andrew    (1000) andrew    (1000)     1955 2023-03-20 14:03:43.000000 mrftools-0.2.1/src/mrftools.egg-info/PKG-INFO
+-rw-rw-r--   0 andrew    (1000) andrew    (1000)     1640 2023-03-20 14:03:44.000000 mrftools-0.2.1/src/mrftools.egg-info/SOURCES.txt
+-rw-rw-r--   0 andrew    (1000) andrew    (1000)        1 2023-03-20 14:03:43.000000 mrftools-0.2.1/src/mrftools.egg-info/dependency_links.txt
+-rw-rw-r--   0 andrew    (1000) andrew    (1000)        1 2022-10-13 12:47:21.000000 mrftools-0.2.1/src/mrftools.egg-info/not-zip-safe
+-rw-rw-r--   0 andrew    (1000) andrew    (1000)      104 2023-03-20 14:03:43.000000 mrftools-0.2.1/src/mrftools.egg-info/requires.txt
+-rw-rw-r--   0 andrew    (1000) andrew    (1000)        9 2023-03-20 14:03:44.000000 mrftools-0.2.1/src/mrftools.egg-info/top_level.txt
```

### Comparing `mrftools-0.1.9/LICENSE` & `mrftools-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `mrftools-0.1.9/PKG-INFO` & `mrftools-0.2.1/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 Metadata-Version: 2.1
 Name: mrftools
-Version: 0.1.9
+Version: 0.2.1
 Summary: Tools for Magnetic Resonance Fingerprinting
 Home-page: https://gitlab.casemri.com/common-resources/mrftools
 Author: Andrew Dupuis
 Author-email: andrew.dupuis@case.edu
-License: UNKNOWN
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # mrftools
 
@@ -41,8 +39,7 @@
 1. git clone https://gitlab.casemri.com/common-resources/mrftools
 2. cd mrftools
 3. pip install .
 
 ## Building and Publishing pip Package
 1. python3 setup.py sdist bdist_wheel
 2. twine upload dist/* 
-
```

### Comparing `mrftools-0.1.9/README.md` & `mrftools-0.2.1/README.md`

 * *Files identical despite different names*

### Comparing `mrftools-0.1.9/setup.py` & `mrftools-0.2.1/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,28 +1,35 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="mrftools",
-    version="0.1.9",
+    version="0.2.1",
     author="Andrew Dupuis",
     author_email="andrew.dupuis@case.edu",
     description="Tools for Magnetic Resonance Fingerprinting",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://gitlab.casemri.com/common-resources/mrftools",
     package_dir = {'': 'src'}, # Our packages live under src but src is not a package itself
     packages=setuptools.find_packages("src"), exclude=["test"],
     classifiers=[
         "Programming Language :: Python :: 3",
         "Operating System :: OS Independent",
     ],
     install_requires=[
-        'numba',
         'scipy',
         'h5py', 
-        'matplotlib'
+        'matplotlib',
+        'nibabel',
+        'SimpleITK', 
+        'azure-storage-blob',
+        'tensorflow',
+        'torch', 
+        'torchkbnufft',
+        'kornia', 
+        'ismrmrd'
     ],
     zip_safe=False
-)
+)
```

### Comparing `mrftools-0.1.9/src/mrftools/dictionaryParameters.py` & `mrftools-0.2.1/src/mrftools/dictionaryParameters.py`

 * *Files 6% similar despite different names*

```diff
@@ -12,22 +12,29 @@
         self.name = name
         self.entries = entries
 
     def __str__(self):
         return "(" + str(len(self.entries)) + ")"
 
     def Initialize(self, T1s, T2s, B1s=[1]):
-        self.entries = np.empty(len(T1s)*len(B1s), dtype=DictionaryEntry)
         if (len(T1s)!=len(T2s)):
-            print("Import Failed: T1/T2 files must have identical number of entries")
+            print("Import Failed: T1/T2 lists must have identical number of entries")
             return 
-        for b1Index in range(len(B1s)):
+        if (len(B1s) != len(T1s)):
+            # B1 lists has different number of entries - tiling T1/T2 across B1
+            self.entries = np.empty(len(T1s)*len(B1s), dtype=DictionaryEntry)
+            for b1Index in range(len(B1s)):
+                for t1Index in range(len(T1s)):
+                    index = b1Index*len(T1s) + t1Index
+                    self.entries[index] = (T1s[t1Index], T2s[t1Index], B1s[b1Index])
+        else:
+            # T1/T2/B1 lists have same number of entries - reading entries 1:1
+            self.entries = np.empty(len(T1s), dtype=DictionaryEntry)
             for t1Index in range(len(T1s)):
-                index = b1Index*len(T1s) + t1Index
-                self.entries[index] = (T1s[t1Index], T2s[t1Index], B1s[b1Index])
+                self.entries[t1Index] = (T1s[t1Index], T2s[t1Index], B1s[t1Index])
         print("Dictionary Parameter set '"+ self.name + "' initialized with " + str(len(self.entries)) + " entries")
     
     def Export(self, filename, force=False):
         if ".mrf" in filename:
             outfile = h5py.File(filename, "a")
             try:
                 outfile.create_group("dictionaryParameters")
```

### Comparing `mrftools-0.1.9/src/mrftools/phantomGenerators.py` & `mrftools-0.2.1/src/mrftools/phantomGenerators.py`

 * *Files identical despite different names*

### Comparing `mrftools-0.1.9/src/mrftools/simulation.py` & `mrftools-0.2.1/src/mrftools/simulation.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,163 +1,107 @@
 import numpy as np
-import numba
-from numba import jit
 import h5py
 from matplotlib import pyplot as plt
+import torch
+from tqdm import tqdm
 
 from mrftools import DictionaryParameters, SequenceParameters
 
 class Simulation: 
-    def __init__(self,sequenceParameters, dictionaryParameters, name="", numTimepoints = -1, phaseRange=(-2*np.pi, 2*np.pi), numSpins=1, results=[], truncationMatrix=[], truncatedResults=[]):
+    def __init__(self,sequenceParameters, dictionaryParameters, name="", numSpins=1, times=[], timeDomainResults=[], results=[], truncationMatrix=[], truncatedResults=[], singularValues=[]):
         self.sequenceParameters = sequenceParameters
         self.dictionaryParameters = dictionaryParameters
-        if numTimepoints == -1:
-            numTimepoints = len(sequenceParameters.timepoints)
-        self.numTimepoints = numTimepoints
-        self.phaseRange = phaseRange
         self.numSpins = numSpins
+        self.times = times
+        self.timeDomainResults = timeDomainResults
         self.results = results
         self.truncationMatrix = truncationMatrix
         self.truncatedResults = truncatedResults
+        self.singularValues = singularValues
         if not name:
-            self.name = sequenceParameters.name + "_" + dictionaryParameters.name + "_" + str(numSpins) # Doesn't account for phase range
+            self.name = sequenceParameters.name + "_" + dictionaryParameters.name + "_" + str(numSpins)
         else:
             self.name = name
 
-    @staticmethod
-    @jit(parallel=True, nopython=True)
-    def ExecuteNumbaSimulation(numTimepoints,T1s,T2s,B1s,TRs,TEs,FAs,phaseValues):
-
-        numberOfExperiments = np.int32(numTimepoints)         
-        numberOfDictionaryEntries = len(T1s)
-        numberOfSpins = len(phaseValues)
-        FAs = np.radians(FAs)
-        Mx0 = np.zeros((numTimepoints,numberOfDictionaryEntries,numberOfSpins))
-        My0 = np.zeros((numberOfExperiments,numberOfDictionaryEntries,numberOfSpins))
-        Mz0 = np.zeros((numberOfExperiments,numberOfDictionaryEntries,numberOfSpins))
-        phaseValueCosines = np.cos(phaseValues)
-        phaseValueSines = np.sin(phaseValues)
-                            
-        for dictionaryEntryNumber in numba.prange(0,numberOfDictionaryEntries):
-            
-            T1 = T1s[dictionaryEntryNumber]
-            T2 = T2s[dictionaryEntryNumber]
-            B1 = B1s[dictionaryEntryNumber]
-            
-            Mx = np.zeros(numberOfSpins)
-            My = np.zeros(numberOfSpins)
-            Mz = np.zeros(numberOfSpins)
-            Mz[:] = -0.95
-            
-            for iTimepoint in range(numTimepoints):
-                fa = FAs[iTimepoint] * B1
-                tr = TRs[iTimepoint]
-                te = TEs[iTimepoint]
-                tre = tr-te
-                
-                At2te = np.exp(-1*te/T2)
-                At1te = np.exp(-1*te/T1)
-                Bt1te = 1-At1te
-                
-                At2tr = np.exp(-1*tre/T2)
-                At1tr = np.exp(-1*tre/T1)
-                Bt1tr = 1-At1tr
-            
-                crf = np.cos(fa)
-                srf = np.sin(fa)
-
-                # Applying flip angle 
-                Myi = My
-                Mzi = Mz
-                My = np.multiply(crf,Myi)-np.multiply(srf,Mzi)
-                Mz = np.multiply(srf,Myi)+np.multiply(crf,Mzi)
-
-                # Relaxation over TE
-                Mx = np.multiply(Mx,At2te)
-                My = np.multiply(My,At2te)
-                Mz = np.multiply(Mz,At1te)+Bt1te
-
-                # Reading value after TE and before TRE
-                Mx0[iTimepoint,dictionaryEntryNumber,:]=Mx[:]
-                My0[iTimepoint,dictionaryEntryNumber,:]=My[:]
-                Mz0[iTimepoint,dictionaryEntryNumber,:]=Mz[:]
-
-                # Relaxation over TRE (TR-TE) 
-                Mx = Mx*At2tr
-                My = My*At2tr
-                Mz = Mz*At1tr+Bt1tr
-
-                # Applying off-resonance to spins
-                Mxi = Mx
-                Myi = My
-                Mx = np.multiply(phaseValueCosines,Mxi) - np.multiply(phaseValueSines,Myi)
-                My = np.multiply(phaseValueSines,Mxi) + np.multiply(phaseValueCosines,Myi)
-
-        return Mx0,My0,Mz0
-        
-    @staticmethod
-    @jit(parallel=True, nopython=True)
-    def ParallizedMeans(Mx0,My0,Mz0):
-        MeansXo = np.zeros((np.shape(Mx0)[0],np.shape(Mx0)[1]))
-        MeansYo = np.zeros((np.shape(Mx0)[0],np.shape(Mx0)[1]))
-        MeansZo = np.zeros((np.shape(Mx0)[0],np.shape(Mx0)[1]))
-
-        for n in numba.prange(np.shape(Mx0)[1]):
-            for timepoint in range(np.shape(Mx0)[0]):
-                MeansXo[timepoint,n] = np.mean(Mx0[timepoint,n,:])
-                MeansYo[timepoint,n] = np.mean(My0[timepoint,n,:])
-                MeansZo[timepoint,n] = np.mean(Mz0[timepoint,n,:])
-        return MeansXo, MeansYo, MeansZo
-
-    def Execute(self, numBatches = 1):
-        TRs = []
-        TEs = []
-        FAs = []
-        T1s= []
-        T2s = []
-        B1s = []
-
-        for timepoint in self.sequenceParameters.timepoints:
-            TRs.append(timepoint['TR'])
-            TEs.append(timepoint['TE'])
-            FAs.append(timepoint['FA'])
-
-        phaseValues = np.linspace(self.phaseRange[0], self.phaseRange[1], self.numSpins)
+    def Execute(self, numBatches=1, device=None):
+        if(device==None):
+            if torch.cuda.is_available():
+                device = torch.device("cuda")
+            else:
+                device = torch.device("cpu")
         dictEntriesPerBatch = int(len(self.dictionaryParameters.entries)/numBatches)
         print("Simulating " + str(numBatches) + " batch(s) of ~" + str(dictEntriesPerBatch) + " dictionary entries")
+        singleResult = self.sequenceParameters.Simulate(self.dictionaryParameters.entries[0], 1)
+        self.numTimepoints = np.shape(singleResult[1][0])[0]
+        self.numReadoutPoints = np.shape(singleResult[2][0])[0]
         Mxy = np.zeros((self.numTimepoints, len(self.dictionaryParameters.entries)), np.complex128)
-        for i in range(numBatches):
-            firstDictEntry = i*dictEntriesPerBatch
-            if i == (numBatches-1):
-                lastDictEntry = len(self.dictionaryParameters.entries)
-            else:
-                lastDictEntry = firstDictEntry+dictEntriesPerBatch
-            print("Starting Batch: " + str(i) + " (Entries " + str(firstDictEntry) + "->" + str(lastDictEntry)+ ")")
-            T1s.clear();T2s.clear();B1s.clear()
-            for dictionaryEntry in self.dictionaryParameters.entries[firstDictEntry:lastDictEntry]:
-                T1s.append(dictionaryEntry['T1'])
-                T2s.append(dictionaryEntry['T2'])
-                B1s.append(dictionaryEntry['B1'])
-            Mx0,My0,Mz0 = self.ExecuteNumbaSimulation(self.numTimepoints, np.asarray(T1s),np.asarray(T2s),np.asarray(B1s),np.asarray(TRs),np.asarray(TEs),np.asarray(FAs),phaseValues)
-            Mx,My,Mz = self.ParallizedMeans(Mx0,My0,Mz0)
-            Mxy[:,firstDictEntry:lastDictEntry] = Mx+(My*1j)
-        self.results = Mxy
+        ReadoutMxy = np.zeros((self.numReadoutPoints, len(self.dictionaryParameters.entries)), np.complex128)
+        with tqdm(total=numBatches) as pbar:
+            for i in range(numBatches):
+                firstDictEntry = i*dictEntriesPerBatch
+                if i == (numBatches-1):
+                    lastDictEntry = len(self.dictionaryParameters.entries)
+                else:
+                    lastDictEntry = firstDictEntry+dictEntriesPerBatch
+                batchDictionaryEntries = self.dictionaryParameters.entries[firstDictEntry:lastDictEntry]
+                allResults = self.sequenceParameters.Simulate(batchDictionaryEntries, self.numSpins, device=device)
+                Mx = torch.mean(allResults[1][0], axis=1)
+                My = torch.mean(allResults[1][1], axis=1)
+                Mxy[:,firstDictEntry:lastDictEntry] = Mx+(My*1j) 
+                ReadoutMx = torch.mean(allResults[2][0], axis=1)
+                ReadoutMy = torch.mean(allResults[2][1], axis=1)
+                ReadoutMxy[:,firstDictEntry:lastDictEntry] = ReadoutMx+(ReadoutMy*1j)
+                pbar.update(1)
+        self.times = allResults[0]
+        self.timeDomainResults = Mxy
+        self.results = ReadoutMxy
         return self.results
+    
+    @staticmethod
+    def GetInnerProducts(querySignals, dictionarySignals):  
+        querySignalsTransposed = querySignals.transpose()
+        normalizedQuerySignals = querySignalsTransposed / np.linalg.norm(querySignalsTransposed, axis=1)[:,None]
+        simulationResultsTransposed = dictionarySignals.transpose()
+        normalizedSimulationResultsTransposed = simulationResultsTransposed / np.linalg.norm(simulationResultsTransposed, axis=1)[:,None]
+        innerProducts = np.inner(normalizedQuerySignals, normalizedSimulationResultsTransposed)
+        return innerProducts
 
-    def CalculateSVD(self, truncationNumber):
+    def CalculateSVD(self, desiredSVDPower=0.99, truncationNumberOverride=None):
         dictionary = self.results.transpose()
         dictionaryNorm = np.sqrt(np.sum(np.power(np.abs(dictionary[:,:]),2),1))
         dictionaryShape = np.shape(dictionary)
         normalizedDictionary = np.zeros_like(dictionary)
         for i in range(dictionaryShape[0]):
             normalizedDictionary[i,:] = dictionary[i,:]/dictionaryNorm[i]
         (u,s,v) = np.linalg.svd(normalizedDictionary, full_matrices=False)
+        self.singularValues = s
+        if truncationNumberOverride == None:
+            (truncationNumber, totalSVDPower) = self.GetTruncationNumberFromDesiredPower(desiredSVDPower)
+        else:
+            truncationNumber = truncationNumberOverride
+            totalSVDPower = self.GetPowerFromDesiredTruncationNumber(truncationNumber)
         vt = np.transpose(v)
         self.truncationMatrix = vt[:,0:truncationNumber]
         self.truncatedResults = np.matmul(normalizedDictionary,self.truncationMatrix).transpose()
+        return (truncationNumber, totalSVDPower)
+
+    def GetTruncationNumberFromDesiredPower(self, desiredSVDPower):
+        singularVectorPowers = self.singularValues/np.sum(self.singularValues)
+        totalSVDPower=0; numSVDComponents=0
+        for singularVectorPower in singularVectorPowers:
+            totalSVDPower += singularVectorPower
+            numSVDComponents += 1
+            if totalSVDPower > desiredSVDPower:
+                break
+        return numSVDComponents, totalSVDPower
+
+    def GetPowerFromDesiredTruncationNumber(self, desiredTruncationNumber):
+        singularVectorPowers = self.singularValues/np.sum(self.singularValues)
+        totalSVDPower=np.sum(singularVectorPowers[0:desiredTruncationNumber])
+        return totalSVDPower
 
     def Export(self, filename, force=False, includeFullResults=True, includeSVDResults=True):
         if ".mrf" in filename:
             outfile = h5py.File(filename, "a")
             try:
                 outfile.create_group("simulations")
             except:
@@ -189,26 +133,28 @@
                     simulation["truncationMatrix"] = []
                     simulation["truncatedResults"] = []
 
                 outfile.close()
         else:
             print("Input is not a .mrf file")
 
-    def Plot(self, numTimepoints=-1, dictionaryEntryNumbers=[], plotTruncated=False):
-        if numTimepoints == -1:
-            numTimepoints = len(self.sequenceParameters.timepoints)
+    def Plot(self, dictionaryEntryNumbers=[], plotTruncated=False, plotTimeDomain=False):
         if dictionaryEntryNumbers == []:
             dictionaryEntryNumbers = [int(len(self.dictionaryParameters.entries)/2)]
         ax = plt.subplot(1,1,1)
-        if not plotTruncated:
-            for entry in dictionaryEntryNumbers:
-                plt.plot(abs(self.results[:,entry]), label=str(self.dictionaryParameters.entries[entry]))
+        if not plotTimeDomain:
+            if not plotTruncated:
+                for entry in dictionaryEntryNumbers:
+                    plt.plot(abs(self.results[:,entry]), label=str(self.dictionaryParameters.entries[entry]))
+            else:
+                for entry in dictionaryEntryNumbers:
+                    plt.plot(abs(self.truncatedResults[:,entry]), label=str(self.dictionaryParameters.entries[entry]))
         else:
             for entry in dictionaryEntryNumbers:
-                plt.plot(abs(self.truncatedResults[:,entry]), label=str(self.dictionaryParameters.entries[entry]))
+                plt.plot(self.times, abs(self.timeDomainResults[:,entry]), label=str(self.dictionaryParameters.entries[entry]))
         ax.legend()
 
     def GetAverageResult(self, indices):
         return np.average(self.results[:,indices], 1)
 
     def FindPatternMatches(self, querySignals, useSVD=False, truncationNumber=25):
         if querySignals.ndim == 1:
```

### Comparing `mrftools-0.1.9/src/mrftools/testing.py` & `mrftools-0.2.1/src/mrftools/testing.py`

 * *Files identical despite different names*

### Comparing `mrftools-0.1.9/src/mrftools/types.py` & `mrftools-0.2.1/src/mrftools/types.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,25 +1,189 @@
 from enum import Enum
 from matplotlib.colors  import ListedColormap
 import numpy as np
 
+class Units(Enum):
+    SECONDS = 0
+    MILLISECONDS = 1
+    MICROSECONDS = 2
+    DEGREES = 3
+    CENTIDEGREES = 4
+    RADIANS = 5
+    CENTIRADIANS = 6
+
+    @staticmethod
+    def Convert(input, inputUnits, outputUnits):
+        if(inputUnits == Units.SECONDS):
+            if(outputUnits == Units.SECONDS):
+                return input
+            if(outputUnits == Units.MILLISECONDS):
+                return input*1000
+            if(outputUnits == Units.MICROSECONDS):
+                return input*(1000*1000)
+            else:
+                print("Cannot convert", inputUnits, "to", outputUnits)
+                return None
+        if(inputUnits == Units.MILLISECONDS):
+            if(outputUnits == Units.SECONDS):
+                return input/1000
+            if(outputUnits == Units.MILLISECONDS):
+                return input
+            if(outputUnits == Units.MICROSECONDS):
+                return input*1000
+            else:
+                print("Cannot convert", inputUnits, "to", outputUnits)
+                return None
+        if(inputUnits == Units.MICROSECONDS):
+            if(outputUnits == Units.SECONDS):
+                return input/(1000*1000)
+            if(outputUnits == Units.MILLISECONDS):
+                return input/1000
+            if(outputUnits == Units.MICROSECONDS):
+                return input
+            else:
+                print("Cannot convert", inputUnits, "to", outputUnits)
+                return None
+        if(inputUnits == Units.DEGREES):
+            if(outputUnits == Units.DEGREES):
+                return input
+            if(outputUnits == Units.CENTIDEGREES):
+                return input*100
+            if(outputUnits == Units.RADIANS):
+                return (input/180)*np.pi
+            if(outputUnits == Units.CENTIRADIANS):
+                return (input/180)*np.pi * 100
+            else:
+                print("Cannot convert", inputUnits, "to", outputUnits)
+                return None
+        if(inputUnits == Units.CENTIDEGREES):
+            if(outputUnits == Units.DEGREES):
+                return input/100
+            if(outputUnits == Units.CENTIDEGREES):
+                return input
+            if(outputUnits == Units.RADIANS):
+                return (input/100/180)*np.pi
+            if(outputUnits == Units.CENTIRADIANS):
+                return (input/180)*np.pi
+            else:
+                print("Cannot convert", inputUnits, "to", outputUnits)
+                return None
+        if(inputUnits == Units.RADIANS):
+            if(outputUnits == Units.DEGREES):
+                return (input/np.pi)*180
+            if(outputUnits == Units.CENTIDEGREES):
+                return (input/np.pi)*180*100
+            if(outputUnits == Units.RADIANS):
+                return input
+            if(outputUnits == Units.CENTIRADIANS):
+                return input*100
+            else:
+                print("Cannot convert", inputUnits, "to", outputUnits)
+                return None
+        if(inputUnits == Units.CENTIRADIANS):
+            if(outputUnits == Units.DEGREES):
+                return (input/100/np.pi)*180
+            if(outputUnits == Units.CENTIDEGREES):
+                return (input/np.pi)*180
+            if(outputUnits == Units.RADIANS):
+                return input/100
+            if(outputUnits == Units.CENTIRADIANS):
+                return input
+            else:
+                print("Cannot convert", inputUnits, "to", outputUnits)
+                return None
+        else:
+            print("Cannot convert", inputUnits, "to", outputUnits)
+            return None 
+
+class SequenceUnits:
+    def __init__(self, time:Units, angle:Units):
+        self.time = time
+        self.angle = angle
+    
+    def __dict__(self):
+        unitsDict = {
+            "time":self.time.name,
+            "angle":self.angle.name
+        }
+        return unitsDict
+    
+    def __str__(self):
+        return "Time: " + str(self.time) + " Angle: " + str(self.angle)
+
+    @staticmethod
+    def FromJson(jsonInput):  
+        timeJson = jsonInput.get("time")
+        angleJson = jsonInput.get("angle")
+
+        if timeJson != None and angleJson != None:
+            return SequenceUnits(Units[timeJson], Units[angleJson])
+        else:
+            print("SequenceUnits requires totalDuration")
+
+    
 class SequenceGeneratorType(Enum):
     PERLIN = 0
     DAN_MA_PERLIN = 1
     SINUSOID = 2
+    BITREVERSE = 3
 
-class SequenceType(Enum):
+class ModuleType(Enum):
+    PREPARATION = 0
+    ACQUISITION = 1
+    RECOVERY = 2
+
+class PreparationType(Enum):
+    RF = 0
+    GRADIENT = 1
+
+class AcquisitionType(Enum):
     FISP = 0
     TRUEFISP = 1
-    
+
+class RecoveryType(Enum):
+    DEADTIME = 0
+    RF = 1
+    GRADIENT = 2
+
+class RFType(Enum):
+    EXCITATION = 0
+    ADIABATIC_EXCITATION = 1
+    INVERSION = 2
+    ADIABATIC_INVERSION = 3
+    REFOCUSING = 4
+    ADIABATIC_REFOCUSING = 5
+    COMPOSITE = 6
+    MAGNETIZATION_TRANSFER = 7
+    SPECTRALLY_SELECTIVE = 8
+    MULTIDIMENSIONAL = 9
+    RAMP = 10
+    SPATIAL_SATURATION = 11
+    SPATIAL_SPECTRAL = 12
+    TAGGING = 13
+
+class GradientType(Enum):
+    DIFFUSION_WEIGHTING = 0
+    FLOW_ENCODING = 1
+    CONCOMITANT_FIELD_CORRECTION = 2
+    CRUSHER = 3
+    EDDY_CURRENT_COMPENSATION = 4
+    GRADIENT_MOMENT_NULLING = 5
+    SPOILER = 6
+    TWISTER = 7
+
 class SyntheticSequenceType(Enum):
     FSE = 0
     IR = 1
     DIR = 2
 
+class KMeansModes(Enum):
+    EUCLIDEAN = 0
+    COSINE = 1
+
 T1_COLORMAP_MIN = 0
 T1_COLORMAP_MAX = 3.000
 
 T2_COLORMAP_MIN = 0
 T2_COLORMAP_MAX = 0.300
 
 B0_COLORMAP_MIN = 0.600
```

### Comparing `mrftools-0.1.9/src/mrftools.egg-info/PKG-INFO` & `mrftools-0.2.1/src/mrftools.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,14 @@
 Metadata-Version: 2.1
 Name: mrftools
-Version: 0.1.9
+Version: 0.2.1
 Summary: Tools for Magnetic Resonance Fingerprinting
 Home-page: https://gitlab.casemri.com/common-resources/mrftools
 Author: Andrew Dupuis
 Author-email: andrew.dupuis@case.edu
-License: UNKNOWN
-Platform: UNKNOWN
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # mrftools
 
@@ -41,8 +39,7 @@
 1. git clone https://gitlab.casemri.com/common-resources/mrftools
 2. cd mrftools
 3. pip install .
 
 ## Building and Publishing pip Package
 1. python3 setup.py sdist bdist_wheel
 2. twine upload dist/* 
-
```

