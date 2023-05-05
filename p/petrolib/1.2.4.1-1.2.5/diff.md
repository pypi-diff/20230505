# Comparing `tmp/petrolib-1.2.4.1.tar.gz` & `tmp/petrolib-1.2.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "petrolib-1.2.4.1.tar", last modified: Mon May  1 18:01:58 2023, max compression
+gzip compressed data, was "petrolib-1.2.5.tar", last modified: Fri May  5 04:32:54 2023, max compression
```

## Comparing `petrolib-1.2.4.1.tar` & `petrolib-1.2.5.tar`

### file list

```diff
@@ -1,24 +1,25 @@
-drwxrwxr-x   0 mayorofgeology  (1000) mayorofgeology  (1000)        0 2023-05-01 18:01:58.661255 petrolib-1.2.4.1/
--rw-rw-r--   0 mayorofgeology  (1000) mayorofgeology  (1000)     1093 2023-03-26 20:57:50.000000 petrolib-1.2.4.1/LICENSE
--rw-rw-r--   0 mayorofgeology  (1000) mayorofgeology  (1000)       40 2023-05-01 16:09:25.000000 petrolib-1.2.4.1/MANIFEST.in
--rw-rw-r--   0 mayorofgeology  (1000) mayorofgeology  (1000)     3691 2023-05-01 18:01:58.661255 petrolib-1.2.4.1/PKG-INFO
--rw-rw-r--   0 mayorofgeology  (1000) mayorofgeology  (1000)     3146 2023-05-01 17:54:18.000000 petrolib-1.2.4.1/README.md
--rw-rw-r--   0 mayorofgeology  (1000) mayorofgeology  (1000)      853 2023-05-01 17:55:01.000000 petrolib-1.2.4.1/pyproject.toml
--rw-rw-r--   0 mayorofgeology  (1000) mayorofgeology  (1000)       38 2023-05-01 18:01:58.661255 petrolib-1.2.4.1/setup.cfg
-drwxrwxr-x   0 mayorofgeology  (1000) mayorofgeology  (1000)        0 2023-05-01 18:01:58.625255 petrolib-1.2.4.1/src/
-drwxrwxr-x   0 mayorofgeology  (1000) mayorofgeology  (1000)        0 2023-05-01 18:01:58.633255 petrolib-1.2.4.1/src/petrolib/
--rwxrwxrwx   0 mayorofgeology  (1000) mayorofgeology  (1000)      278 2023-05-01 17:59:23.000000 petrolib-1.2.4.1/src/petrolib/__init__.py
-drwxrwxr-x   0 mayorofgeology  (1000) mayorofgeology  (1000)        0 2023-05-01 18:01:58.633255 petrolib-1.2.4.1/src/petrolib/data/
--rwxrwxrwx   0 mayorofgeology  (1000) mayorofgeology  (1000)      286 2023-02-13 04:26:20.000000 petrolib-1.2.4.1/src/petrolib/data/litho_info.csv
--rwxrwxrwx   0 mayorofgeology  (1000) mayorofgeology  (1000)     4893 2023-05-01 15:44:07.000000 petrolib-1.2.4.1/src/petrolib/file_reader.py
--rwxrwxrwx   0 mayorofgeology  (1000) mayorofgeology  (1000)     8001 2023-04-12 22:16:51.000000 petrolib-1.2.4.1/src/petrolib/interp.py
--rwxrwxrwx   0 mayorofgeology  (1000) mayorofgeology  (1000)    58756 2023-05-01 16:14:23.000000 petrolib-1.2.4.1/src/petrolib/plots.py
--rwxrwxrwx   0 mayorofgeology  (1000) mayorofgeology  (1000)     6786 2023-04-12 22:19:13.000000 petrolib-1.2.4.1/src/petrolib/procs.py
--rwxrwxrwx   0 mayorofgeology  (1000) mayorofgeology  (1000)     5394 2023-03-26 17:12:05.000000 petrolib-1.2.4.1/src/petrolib/stats.py
--rw-rw-r--   0 mayorofgeology  (1000) mayorofgeology  (1000)      236 2023-05-01 15:40:48.000000 petrolib-1.2.4.1/src/petrolib/utils.py
--rwxrwxrwx   0 mayorofgeology  (1000) mayorofgeology  (1000)    57715 2023-03-26 20:12:21.000000 petrolib-1.2.4.1/src/petrolib/workflow.py
-drwxrwxr-x   0 mayorofgeology  (1000) mayorofgeology  (1000)        0 2023-05-01 18:01:58.633255 petrolib-1.2.4.1/src/petrolib.egg-info/
--rw-rw-r--   0 mayorofgeology  (1000) mayorofgeology  (1000)     3691 2023-05-01 18:01:58.000000 petrolib-1.2.4.1/src/petrolib.egg-info/PKG-INFO
--rw-rw-r--   0 mayorofgeology  (1000) mayorofgeology  (1000)      410 2023-05-01 18:01:58.000000 petrolib-1.2.4.1/src/petrolib.egg-info/SOURCES.txt
--rw-rw-r--   0 mayorofgeology  (1000) mayorofgeology  (1000)        1 2023-05-01 18:01:58.000000 petrolib-1.2.4.1/src/petrolib.egg-info/dependency_links.txt
--rw-rw-r--   0 mayorofgeology  (1000) mayorofgeology  (1000)        9 2023-05-01 18:01:58.000000 petrolib-1.2.4.1/src/petrolib.egg-info/top_level.txt
+drwxrwxr-x   0 mayorofgeology  (1000) mayorofgeology  (1000)        0 2023-05-05 04:32:54.856857 petrolib-1.2.5/
+-rw-rw-r--   0 mayorofgeology  (1000) mayorofgeology  (1000)     1093 2023-03-26 20:57:50.000000 petrolib-1.2.5/LICENSE
+-rw-rw-r--   0 mayorofgeology  (1000) mayorofgeology  (1000)       40 2023-05-01 16:09:25.000000 petrolib-1.2.5/MANIFEST.in
+-rw-rw-r--   0 mayorofgeology  (1000) mayorofgeology  (1000)     3731 2023-05-05 04:32:54.856857 petrolib-1.2.5/PKG-INFO
+-rw-rw-r--   0 mayorofgeology  (1000) mayorofgeology  (1000)     3190 2023-05-05 04:14:13.000000 petrolib-1.2.5/README.md
+-rw-rw-r--   0 mayorofgeology  (1000) mayorofgeology  (1000)      957 2023-05-05 04:30:11.000000 petrolib-1.2.5/pyproject.toml
+-rw-rw-r--   0 mayorofgeology  (1000) mayorofgeology  (1000)       38 2023-05-05 04:32:54.856857 petrolib-1.2.5/setup.cfg
+drwxrwxr-x   0 mayorofgeology  (1000) mayorofgeology  (1000)        0 2023-05-05 04:32:54.804855 petrolib-1.2.5/src/
+drwxrwxr-x   0 mayorofgeology  (1000) mayorofgeology  (1000)        0 2023-05-05 04:32:54.828856 petrolib-1.2.5/src/petrolib/
+-rwxrwxrwx   0 mayorofgeology  (1000) mayorofgeology  (1000)      276 2023-05-05 04:26:54.000000 petrolib-1.2.5/src/petrolib/__init__.py
+drwxrwxr-x   0 mayorofgeology  (1000) mayorofgeology  (1000)        0 2023-05-05 04:32:54.832856 petrolib-1.2.5/src/petrolib/data/
+-rwxrwxrwx   0 mayorofgeology  (1000) mayorofgeology  (1000)      286 2023-02-13 04:26:20.000000 petrolib-1.2.5/src/petrolib/data/litho_info.csv
+-rwxrwxrwx   0 mayorofgeology  (1000) mayorofgeology  (1000)     4877 2023-05-05 04:21:04.000000 petrolib-1.2.5/src/petrolib/file_reader.py
+-rwxrwxrwx   0 mayorofgeology  (1000) mayorofgeology  (1000)     8035 2023-05-05 04:09:44.000000 petrolib-1.2.5/src/petrolib/interp.py
+-rwxrwxrwx   0 mayorofgeology  (1000) mayorofgeology  (1000)    59141 2023-05-05 04:07:20.000000 petrolib-1.2.5/src/petrolib/plots.py
+-rwxrwxrwx   0 mayorofgeology  (1000) mayorofgeology  (1000)     6822 2023-05-05 04:09:53.000000 petrolib-1.2.5/src/petrolib/procs.py
+-rwxrwxrwx   0 mayorofgeology  (1000) mayorofgeology  (1000)     5430 2023-05-05 04:10:09.000000 petrolib-1.2.5/src/petrolib/stats.py
+-rw-rw-r--   0 mayorofgeology  (1000) mayorofgeology  (1000)      202 2023-05-04 03:45:42.000000 petrolib-1.2.5/src/petrolib/utils.py
+-rwxrwxrwx   0 mayorofgeology  (1000) mayorofgeology  (1000)    57715 2023-05-05 04:12:11.000000 petrolib-1.2.5/src/petrolib/workflow.py
+drwxrwxr-x   0 mayorofgeology  (1000) mayorofgeology  (1000)        0 2023-05-05 04:32:54.832856 petrolib-1.2.5/src/petrolib.egg-info/
+-rw-rw-r--   0 mayorofgeology  (1000) mayorofgeology  (1000)     3731 2023-05-05 04:32:54.000000 petrolib-1.2.5/src/petrolib.egg-info/PKG-INFO
+-rw-rw-r--   0 mayorofgeology  (1000) mayorofgeology  (1000)      445 2023-05-05 04:32:54.000000 petrolib-1.2.5/src/petrolib.egg-info/SOURCES.txt
+-rw-rw-r--   0 mayorofgeology  (1000) mayorofgeology  (1000)        1 2023-05-05 04:32:54.000000 petrolib-1.2.5/src/petrolib.egg-info/dependency_links.txt
+-rw-rw-r--   0 mayorofgeology  (1000) mayorofgeology  (1000)       65 2023-05-05 04:32:54.000000 petrolib-1.2.5/src/petrolib.egg-info/requires.txt
+-rw-rw-r--   0 mayorofgeology  (1000) mayorofgeology  (1000)        9 2023-05-05 04:32:54.000000 petrolib-1.2.5/src/petrolib.egg-info/top_level.txt
```

### Comparing `petrolib-1.2.4.1/LICENSE` & `petrolib-1.2.5/LICENSE`

 * *Files identical despite different names*

### Comparing `petrolib-1.2.4.1/PKG-INFO` & `petrolib-1.2.5/README.md`

 * *Files 11% similar despite different names*

```diff
@@ -1,21 +1,7 @@
-Metadata-Version: 2.1
-Name: petrolib
-Version: 1.2.4.1
-Summary: A Python Package for Petrophysical Evaluation
-Author-email: Joshua Atolagbe <atolagbejoshua2@gmail.com>
-Project-URL: Homepage, https://github.com/mayor-of-geology/petrolib
-Project-URL: Bug Tracker, https://github.com/mayor-of-geology/petrolib/issues
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.5
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # Petrophysical Evaluation Package
 
 This is a python package designed to help users perform petrophysical analysis by estimating petrophysical parameters such as:
 ```
 * Volume of Shale using various methods like Clavier, Stieber and Larionov methods
 * Porosity - Effective and Total porosities using the density and Wyllie's sonic methods.
 * Water Saturation - using both archie and simmandoux methods
@@ -43,14 +29,21 @@
 * Well log visualisation 
 * Plot well locations on an actual map
 * Facilitates the loading of well tops.
 * Plot log curves along with zonation tracks
 * Neutron-density cross plot
 * Pickett Plot
 
+### Installation
+
+```
+pip install petrolib
+```
+
+
 ### Quick tutorial
 ```
 #import necessaries
 from pathlib import Path
 from petrolib import procs
 from petrolib import file_reader as fr
 from petrolib.workflow import Quanti
@@ -88,9 +81,9 @@
 
 ps = pp.paySummary(name='15-9_F1A')
 
 #save results to excel
 pp.save(file_name='Pay Summary')
 ```
 
-Tutorial [link](https://github.com/mayor-of-geology/tutorials/petrolib)
+Tutorial repo [link](https://github.com/joshua-atolagbe/tutorials)
```

### Comparing `petrolib-1.2.4.1/src/petrolib/file_reader.py` & `petrolib-1.2.5/src/petrolib/file_reader.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 A Python module for handling th importation of files into code environment
 
 Functions
 ---------
 load_las
 load_table
 '''
-
+from __future__ import annotations
 from pathlib import Path
 from warnings import filterwarnings
 filterwarnings('ignore')
 import lasio
 import pandas as pd
 from .utils import MnemonicError
 
@@ -55,15 +55,14 @@
 
             assert file.exists(), 'File does not exists'      
 
     except:
 
         raise FileNotFoundError(f'{file} path does not exists.')
 
-        # raise TypeError(f'{file} is not a LAS file')
 
     las = lasio.read(str(file))
 
     assert type(las) == lasio.las.LASFile, 'Fucntion can only read a LAS file'
 
     if return_csv == True:
 
@@ -75,15 +74,15 @@
             
                 for i in curves:
                     
                     assert i in df.columns, f"'{i}' not found in log data."
                     
             except:
                 
-                raise MnemonicError('Check data. Log curve mnemonic not passed correctly.')
+                raise MnemonicError('Check data. A log curve mnemonic was not passed correctly.')
         
             df = df.filter(curves, axis=1)
             
             return df, las
     
         elif curves == None:
```

### Comparing `petrolib-1.2.4.1/src/petrolib/interp.py` & `petrolib-1.2.5/src/petrolib/interp.py`

 * *Files 5% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 Python module for reservoir interpretation from plots
 
 Function
 --------
 crossPlot
 picketPlot
 '''
-
+from __future__ import annotations
 import seaborn as sns
 import numpy as np
 import pandas as pd
 from itertools import cycle
 from random import choice
 from matplotlib import pyplot as plt
 from matplotlib.ticker import FormatStrFormatter
```

### Comparing `petrolib-1.2.4.1/src/petrolib/plots.py` & `petrolib-1.2.5/src/petrolib/plots.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,14 +10,15 @@
 plotLoc
 tripleCombo
 plotLog
 plotZoneCombo
 plotLogFacies
 plotLogs
 '''
+from __future__ import annotations
 
 
 import numpy as np
 import lasio
 import csv
 import pandas as pd
 import contextily as ctx
@@ -500,18 +501,18 @@
         color = [choice(next(cycol)) for i in range(len(logs))]
         np.random.shuffle(color)
 
         for i in range(len(logs)):
             
             if logs[i] == 'RT' or logs[i] == 'ILD':
                 # for resistivity, semilog plot
-                ax[i].semilogx(self._df[logs[i]], self._df[depth], color=color[i])
+                ax[i].semilogx(self._df[logs[i]], self._df[depth], color=color[i], linewidth=1.)
             else:
                 # for non-resistivity, normal plot
-                ax[i].plot(self._df[logs[i]], self._df[depth], color=color[i])
+                ax[i].plot(self._df[logs[i]], self._df[depth], color=color[i], linewidth=1.)
 
             if logs[i] == 'NPHI':
                 ax[i].invert_xaxis()
 
             ax[i].set_title(logs[i], pad=15)
             ax[i].minorticks_on()
             ax[i].set_ylim(top, bottom); ax[i].invert_yaxis()
@@ -599,18 +600,18 @@
         np.random.shuffle(color)
 
         if len(logs) > 1:
             for i in range(len(logs)):
                 np.random.shuffle(color)
                 if logs[i] == 'RT' or logs[i] == 'ILD':
                     # for resistivity, semilog plot
-                    ax[i].semilogx(df[logs[i]], df[depth], color=color[i])
+                    ax[i].semilogx(df[logs[i]], df[depth], color=color[i], linewidth=1.)
                 else:
                     # for non-resistivity, normal plot
-                    ax[i].plot(df[logs[i]], df[depth], color=color[i])
+                    ax[i].plot(df[logs[i]], df[depth], color=color[i], linewidth=1.)
 
                 if logs[i] == 'NPHI' or logs[i] == 'PHIE':
                     ax[i].invert_xaxis()
 
                 ax[i].set_title(logs[i], pad=15)
                 ax[i].minorticks_on()
                 ax[i].set_ylim(top, bottom); ax[i].invert_yaxis()
@@ -624,18 +625,18 @@
         
         elif len(logs) == 1:
             
             for i in logs:
                 np.random.shuffle(color)
                 if i == 'RT' or i == 'ILD':
                     # for resistivity, semilog plot
-                    plt.semilogx(df[i], df[depth], color=next(cycol))
+                    plt.semilogx(df[i], df[depth], color=next(cycol), linewidth=1.)
                 else:
                         # for non-resistivity, normal plot
-                    plt.plot(df[i], df[depth], color=next(cycol))
+                    plt.plot(df[i], df[depth], color=next(cycol), linewidth=1.)
 
                 if i == 'NPHI' or i == 'PHIE':
                     plt.xlim(df[i].max(), df[i].min())
                     
                 plt.title(i, pad=15)
                 plt.minorticks_on()
                 plt.ylim(bottom, top);
@@ -985,24 +986,24 @@
             if isinstance(j, list):
 
                 assert len(j) > 1, 'Error. list of lists of curves must be greater than 1.'
                 np.random.shuffle(color)
                 for ii in range(len(j)):
                     if logs[i][ii] == 'RT' or logs[i][ii] == 'ILD':
                         # for resistivity, semilog plot
-                        ax[i].semilogx(df[logs[i][ii]], df[depth], color=color[-i])
+                        ax[i].semilogx(df[logs[i][ii]], df[depth], color=color[-i], linewidth=1.)
 
                     if ii == 0:# and logs[i][ii] != 'RT':
                         # for non-resistivity, normal plot
-                        ax[i].plot(df[logs[i][ii]], df[depth], color=color[ii])
+                        ax[i].plot(df[logs[i][ii]], df[depth], color=color[ii], linewidth=1.)
                         
                         # ax[ii].set_xticklabels([]);  ax[ii].set_xticks([])
                         ax[i].set_xticklabels([]);  ax[i].set_xticks([])
                     if ii >= 1:# or logs[i][ii] != 'RT':
-                        ax[i].twiny().plot(df[logs[i][ii]], df[depth], color=color[ii])    
+                        ax[i].twiny().plot(df[logs[i][ii]], df[depth], color=color[ii], linewidth=1.)    
                         ax[i].set_xticklabels([]);  ax[i].set_xticks([])                    
                     
                     
                     ax[i].yaxis.grid(which='major', linestyle='-', linewidth=1, color='darkgrey')
                     ax[i].yaxis.grid(which='minor', linestyle='-', linewidth=0.5, color='lightgrey')
                     
                 tracks = []
@@ -1035,19 +1036,19 @@
                     axes.invert_yaxis()
                     additive += 0.06
   
             else:
                 np.random.shuffle(color)
                 if logs[i] == 'RT' or logs[i] == 'ILD':
                     # for resistivity, semilog plot
-                    ax[i].semilogx(df[logs[i]], df[depth], color=color[i])
+                    ax[i].semilogx(df[logs[i]], df[depth], color=color[i], linewidth=1.)
                     
                 else:
                     # for non-resistivity, normal plot
-                    ax[i].plot(df[logs[i]], df[depth], color=color[i])
+                    ax[i].plot(df[logs[i]], df[depth], color=color[i], linewidth=1.)
 
                 if logs[i] == 'NPHI' or logs[i] == 'PHIE':
                     ax[i].invert_xaxis()
 
                 ax[i].set_title(logs[i], pad=15)
                 ax[i].minorticks_on()
                 ax[i].set_ylim(top, bottom); ax[i].invert_yaxis()
@@ -1064,18 +1065,18 @@
     elif len(logs) == 1 and facies == None:
             
         for idxi, i in enumerate(logs):
             if not isinstance(i, list):
                 np.random.shuffle(color)
                 if i == 'RT' or i == 'ILD':
                     # for resistivity, semilog plot
-                    plt.semilogx(df[i], df[depth], color=color[idxi])
+                    plt.semilogx(df[i], df[depth], color=color[idxi], linewidth=1.)
                 else:
                         # for non-resistivity, normal plot
-                    plt.plot(df[i], df[depth], color=color[idxi])
+                    plt.plot(df[i], df[depth], color=color[idxi], linewidth=1.)
 
                 if i == 'NPHI' or i == 'PHIE':
                     plt.xlim(df[i].max(), df[i].min())
 
                 plt.title(i, pad=15)
                 plt.minorticks_on()
                 plt.ylim(bottom, top);
@@ -1097,15 +1098,15 @@
                         # ax.set_xticklabels([]);ax.set_xticks([])
                     if idxii == 0:
                         # for non-resistivity, normal plot
                         ax.plot(df[logs[idxi][idxii]], df[depth], color=color[idxii], linewidth=1.)
                         ax.set_xticklabels([]); ax.set_xticks([])
 
                     if idxii >= 1:
-                        ax.twiny().plot(df[logs[idxi][idxii]], df[depth], color=color[idxii])    
+                        ax.twiny().plot(df[logs[idxi][idxii]], df[depth], color=color[idxii], linewidth=1.)    
                         ax.set_xticklabels([]);  ax.set_xticks([])
 
                     ax.yaxis.grid(which='major', linestyle='-', linewidth=1, color='darkgrey')
                     ax.yaxis.grid(which='minor', linestyle='-', linewidth=0.5, color='lightgrey')
 
                              
                 tracks = []
@@ -1143,18 +1144,18 @@
 
     elif len(logs) == 1 and facies != None:            
         for idxi, i in enumerate(logs):
             if not isinstance(i, list):
                 np.random.shuffle(color)
                 if i == 'RT' or i == 'ILD':
                     # for resistivity, semilog plot
-                    ax[idxi].semilogx(df[i], df[depth], color=color[idxi])
+                    ax[idxi].semilogx(df[i], df[depth], color=color[idxi], linewidth=1.)
                 else:
                         # for non-resistivity, normal plot
-                    ax[idxi].plot(df[i], df[depth], color=color[idxi])
+                    ax[idxi].plot(df[i], df[depth], color=color[idxi], linewidth=1.)
 
                 if i == 'NPHI' or i == 'PHIE':
                     ax[idxi].xlim(df[i].max(), df[i].min())
 
                 ax[idxi].set_title(i, pad=15)
                 ax[idxi].minorticks_on()
                 ax[idxi].set_ylim(bottom, top);
@@ -1174,15 +1175,15 @@
                         ax[idxi].semilogx(df[logs[idxi][idxii]], df[depth], color=color[idxii], linewidth=1.)
                         # ax[idxi].set_xticklabels([]);ax[idxi].set_xticks([])
                     if idxii == 0:
                         # for non-resistivity, normal plot
                         ax[idxi].plot(df[logs[idxi][idxii]], df[depth], color=color[idxii], linewidth=1.)
                         ax[idxi].set_xticklabels([]); ax[idxi].set_xticks([])
                     if idxii >= 1:
-                        ax[idxi].twiny().plot(df[logs[idxi][idxii]], df[depth], color=color[idxii])  
+                        ax[idxi].twiny().plot(df[logs[idxi][idxii]], df[depth], color=color[idxii], linewidth=1.)  
                         ax[idxii].twiny().set_xticklabels([]);  ax[idxii].twiny().set_xticks([])  
 
                     ax[idxi].yaxis.grid(which='major', linestyle='-', linewidth=1, color='darkgrey')
                     ax[idxi].yaxis.grid(which='minor', linestyle='-', linewidth=0.5, color='lightgrey')
 
                 tracks = []
 
@@ -1310,24 +1311,24 @@
             if isinstance(j, list):
 
                 assert len(j) > 1, 'Error. list of lists of curves must be greater than 1.'
                 np.random.shuffle(color)
                 for ii in range(len(j)):
                     if logs[i][ii] == 'RT' or logs[i][ii] == 'ILD':
                         # for resistivity, semilog plot
-                        ax[i].semilogx(df[logs[i][ii]], df[depth], color=color[-i])
+                        ax[i].semilogx(df[logs[i][ii]], df[depth], color=color[-i], linewidth=1.)
 
                     if ii == 0:# and logs[i][ii] != 'RT':
                         # for non-resistivity, normal plot
-                        ax[i].plot(df[logs[i][ii]], df[depth], color=color[ii])
+                        ax[i].plot(df[logs[i][ii]], df[depth], color=color[ii], linewidth=1.)
                         
                         # ax[ii].set_xticklabels([]);  ax[ii].set_xticks([])
                         ax[i].set_xticklabels([]);  ax[i].set_xticks([])
                     if ii >= 1:# or logs[i][ii] != 'RT':
-                        ax[i].twiny().plot(df[logs[i][ii]], df[depth], color=color[ii])    
+                        ax[i].twiny().plot(df[logs[i][ii]], df[depth], color=color[ii], linewidth=1.)    
                         ax[i].set_xticklabels([]);  ax[i].set_xticks([])        
                     
                     
                     ax[i].yaxis.grid(which='major', linestyle='-', linewidth=1, color='darkgrey')
                     ax[i].yaxis.grid(which='minor', linestyle='-', linewidth=0.5, color='lightgrey')
                     
                 tracks = []
@@ -1360,19 +1361,19 @@
                     axes.invert_yaxis()
                     additive += 0.06
   
             else:
                 np.random.shuffle(color)
                 if logs[i] == 'RT' or logs[i] == 'ILD':
                     # for resistivity, semilog plot
-                    ax[i].semilogx(df[logs[i]], df[depth], color=color[i])
+                    ax[i].semilogx(df[logs[i]], df[depth], color=color[i], linewidth=1.)
                     
                 else:
                     # for non-resistivity, normal plot
-                    ax[i].plot(df[logs[i]], df[depth], color=color[i])
+                    ax[i].plot(df[logs[i]], df[depth], color=color[i], linewidth=1.)
 
                 if logs[i] == 'NPHI' or logs[i] == 'PHIE':
                     ax[i].invert_xaxis()
 
                 ax[i].set_title(logs[i], pad=15)
                 ax[i].minorticks_on()
                 ax[i].set_ylim(top, bottom); ax[i].invert_yaxis()
@@ -1389,18 +1390,18 @@
     elif len(logs) == 1:
             
         for idxi, i in enumerate(logs):
             if not isinstance(i, list):
                 np.random.shuffle(color)
                 if i == 'RT' or i == 'ILD':
                     # for resistivity, semilog plot
-                    plt.semilogx(df[i], df[depth], color=color[idxi])
+                    plt.semilogx(df[i], df[depth], color=color[idxi], linewidth=1.)
                 else:
                         # for non-resistivity, normal plot
-                    plt.plot(df[i], df[depth], color=color[idxi])
+                    plt.plot(df[i], df[depth], color=color[idxi], linewidth=1.)
 
                 if i == 'NPHI' or i == 'PHIE':
                     plt.xlim(df[i].max(), df[i].min())
 
                 plt.title(i, pad=15)
                 plt.minorticks_on()
                 plt.ylim(bottom, top);
@@ -1423,15 +1424,15 @@
                         # ax.set_xticklabels([]);ax.set_xticks([])
                     if idxii == 0:
                         # for non-resistivity, normal plot
                         ax.plot(df[logs[idxi][idxii]], df[depth], color=color[idxii], linewidth=1.)
                         ax.set_xticklabels([]); ax.set_xticks([])
 
                     if idxii >= 1:
-                        ax.twiny().plot(df[logs[idxi][idxii]], df[depth], color=color[idxii])    
+                        ax.twiny().plot(df[logs[idxi][idxii]], df[depth], color=color[idxii], linewidth=1.)    
                         ax.set_xticklabels([]);  ax.set_xticks([])
 
                     ax.yaxis.grid(which='major', linestyle='-', linewidth=1, color='darkgrey')
                     ax.yaxis.grid(which='minor', linestyle='-', linewidth=0.5, color='lightgrey')
 
                              
                 tracks = []
```

### Comparing `petrolib-1.2.4.1/src/petrolib/procs.py` & `petrolib-1.2.5/src/petrolib/procs.py`

 * *Files 1% similar despite different names*

```diff
@@ -6,14 +6,15 @@
 ---------
 set_alias
 process_data
 trim
 model_facies
 
 '''
+from __future__ import annotations
 
 from warnings import filterwarnings
 filterwarnings('ignore')
 import pandas as pd
 import numpy as np
 from typing import Optional
```

### Comparing `petrolib-1.2.4.1/src/petrolib/stats.py` & `petrolib-1.2.5/src/petrolib/stats.py`

 * *Files 1% similar despite different names*

```diff
@@ -7,14 +7,15 @@
 
 Function
 --------
 displayFreq
 
 '''
 
+from __future__ import annotations
 
 from warnings import filterwarnings
 filterwarnings('ignore')
 import seaborn as sns
 import pandas as pd
 import numpy as np
 from scipy.stats.stats import pearsonr
```

### Comparing `petrolib-1.2.4.1/src/petrolib/workflow.py` & `petrolib-1.2.5/src/petrolib/workflow.py`

 * *Files 1% similar despite different names*

```diff
@@ -189,15 +189,15 @@
 
         self._results = pd.DataFrame.from_records(df)
 
         #return result
 
         return self._results, data
 
-    def vshale(self, method:str='linear', show_plot:bool=False, palette_op:str=None, figsize:slice=None):
+    def vshale(self, method:str='linear', show_plot:bool=False, palette_op:str=None, figsize:tuple=None):
         
         '''
 
         Computes the Volume of Shale
 
         Parameters
         ----------
@@ -210,15 +210,15 @@
 
         show_plot : bool default False
             Display plot if True.. Plots GR, VSH and Zone track
 
         palette_op: str default None
             Palette option for to color code vshale plot. Check https://matplotlib.org/stable/tutorials/colors/colormaps.html
 
-        figsize: slice default None
+        figsize: tuple default None
             Size of plot
 
         Returns
         ------
         Either/Both Dataframe containing the VSH and the plot if show_plot=True  
        
 
@@ -353,15 +353,15 @@
         elif show_plot==False:
             
 #             assert palette_op == None and figsize == None, f'show_plot is set to {show_plot}. Set palette_op and figsize as None'
 
             return new_data
 
     def porosity(self, method:str='density', rhob_shale:float=2.4, rhob_fluid:float=1.,
-                     rhob_matrix:float=2.65, fzs:float=None, show_plot:bool=False, figsize:slice=None):
+                     rhob_matrix:float=2.65, fzs:float=None, show_plot:bool=False, figsize:tuple=None):
 
         '''
         Computes the effective and total porosities using the 'density' and Wyllie's 'sonic' method. 
         To use, must have called the `vshale` method 
 
         Parameters
         ----------
@@ -379,15 +379,15 @@
 
         fzs: float default None
             Flushed zone saturation for PHIE. If None, it is calculated from rhob_fluid, rhob_shale and rhob_matrix
 
         show_plot : bool default False
             Display plot if True.. Plots RHOB, VSH, PHIE/PHIT and Zone track
 
-        figsize: slice default None
+        figsize: tuple default None
             Size of plot
 
         Returns
         -------
         Either/Both Dataframe containing the PHIE/PHIT and the plot if show_plot=True  
        
 
@@ -547,15 +547,15 @@
         elif show_plot==False:
             
 #             assert figsize == None, f'show_plot is set to {show_plot}. Set figsize as None'
 
             return new_data
 
     def water_saturation(self, method:str='archie', rw:float=0.03, a:float=1., m:float=2., n:float=2.,
-                                 show_plot:bool=False, figsize:slice=None):
+                                 show_plot:bool=False, figsize:tuple=None):
 
                 
         '''
 
         Computes water and hydrocarbon saturation
         To use, must have called both `vshale` and `porosity` methods
 
@@ -575,15 +575,15 @@
 
         n : float default 2.
             Saturation exponent
 
         show_plot : bool default False
             Display plot if True.. Plots RT, SW, PHIE/PHIT and Zone track
 
-        figsize: slice default None
+        figsize: tuple default None
             Size of plot
 
         Returns
         ------
         Either/Both Dataframe containing the SW, SH and the plot if show_plot=True  
        
 
@@ -744,27 +744,27 @@
         elif show_plot==False:
             
             
 #             assert figsize == None, f'show_plot is set to {show_plot}. Set figsize as None'
 
             return new_data
 
-    def permeability(self, show_plot:bool=False, figsize:slice=None):
+    def permeability(self, show_plot:bool=False, figsize:tuple=None):
 
         '''
 
         Computes the permeability
         To use, must have called `vshale` and `porosity` and `water_saturation` methods
 
         Parameters
         ----------
         show_plot : bool default False
             Display plot if True.. Plots PHIE, Permeability and Zone track
 
-        figsize: slice default None
+        figsize: tuple default None
             Size of plot
 
         Returns
         ------
         Either/Both Dataframe containing the Perm and the plot if show_plot=True  
        
 
@@ -867,15 +867,15 @@
             
             
 #             assert figsize == None, f'show_plot is set to {show_plot}. Set figsize as None'
 
             return new_data
 
     def flags(self, vsh_cutoff:float, por_cutoff:float, sw_cutoff:float, 
-                        ref_unit:str='m', show_plot:bool=False, palette_op:str=None, figsize:slice=None):
+                        ref_unit:str='m', show_plot:bool=False, palette_op:str=None, figsize:tuple=None):
 
         '''
 
         Create the {ROCK, RES, PAY} flags
 
         To use, must have called `vshale`, `porosity`, `water_saturation` and `permeability` methods
 
@@ -897,15 +897,15 @@
         
         show_plot : bool default False
             Display plot if True.. Plots GR, RT, VSH, SW, Perm, NPHI/RHOB, PHIE/PHIT, ['ROCK', 'RES', 'PAY] flags and Zonation track
 
         palette_op : str default None
              palette option for VSH coloring. Check https://matplotlib.org/stable/tutorials/colors/colormaps.html for availabel palette options
 
-        figsize: slice default None
+        figsize: tuple default None
             Size of plot
 
         Returns
         ------
         Either/Both Dataframe containing the flags and the plot if show_plot=True
```

### Comparing `petrolib-1.2.4.1/src/petrolib.egg-info/PKG-INFO` & `petrolib-1.2.5/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 Metadata-Version: 2.1
 Name: petrolib
-Version: 1.2.4.1
+Version: 1.2.5
 Summary: A Python Package for Petrophysical Evaluation
 Author-email: Joshua Atolagbe <atolagbejoshua2@gmail.com>
-Project-URL: Homepage, https://github.com/mayor-of-geology/petrolib
-Project-URL: Bug Tracker, https://github.com/mayor-of-geology/petrolib/issues
+Project-URL: Homepage, https://github.com/joshua-atolagbe/petrolib
+Project-URL: Bug Tracker, https://github.com/joshua-atolagbe/petrolib/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.5
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Petrophysical Evaluation Package
 
 This is a python package designed to help users perform petrophysical analysis by estimating petrophysical parameters such as:
 ```
@@ -43,14 +43,21 @@
 * Well log visualisation 
 * Plot well locations on an actual map
 * Facilitates the loading of well tops.
 * Plot log curves along with zonation tracks
 * Neutron-density cross plot
 * Pickett Plot
 
+### Installation
+
+```
+pip install petrolib
+```
+
+
 ### Quick tutorial
 ```
 #import necessaries
 from pathlib import Path
 from petrolib import procs
 from petrolib import file_reader as fr
 from petrolib.workflow import Quanti
@@ -88,9 +95,9 @@
 
 ps = pp.paySummary(name='15-9_F1A')
 
 #save results to excel
 pp.save(file_name='Pay Summary')
 ```
 
-Tutorial [link](https://github.com/mayor-of-geology/tutorials/petrolib)
+Tutorial repo [link](https://github.com/joshua-atolagbe/tutorials)
```

