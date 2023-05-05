# Comparing `tmp/PyBerries-0.2.6.post1.tar.gz` & `tmp/PyBerries-0.2.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PyBerries-0.2.6.post1.tar", last modified: Fri May  5 09:47:28 2023, max compression
+gzip compressed data, was "PyBerries-0.2.7.tar", last modified: Fri May  5 15:52:40 2023, max compression
```

## Comparing `PyBerries-0.2.6.post1.tar` & `PyBerries-0.2.7.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxrwxrwx   0        0        0        0 2023-05-05 09:47:28.759485 PyBerries-0.2.6.post1/
--rw-rw-rw-   0        0        0    33074 2022-12-22 10:37:47.000000 PyBerries-0.2.6.post1/LICENSE
--rw-rw-rw-   0        0        0    14427 2023-05-05 09:47:28.746485 PyBerries-0.2.6.post1/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-05-05 09:47:28.711430 PyBerries-0.2.6.post1/PyBerries.egg-info/
--rw-rw-rw-   0        0        0    14427 2023-05-05 09:47:28.000000 PyBerries-0.2.6.post1/PyBerries.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      723 2023-05-05 09:47:28.000000 PyBerries-0.2.6.post1/PyBerries.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-05 09:47:28.000000 PyBerries-0.2.6.post1/PyBerries.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       70 2023-05-05 09:47:28.000000 PyBerries-0.2.6.post1/PyBerries.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-05-05 09:47:28.000000 PyBerries-0.2.6.post1/PyBerries.egg-info/top_level.txt
--rw-rw-rw-   0        0        0    14103 2023-05-03 12:45:51.000000 PyBerries-0.2.6.post1/README.md
-drwxrwxrwx   0        0        0        0 2023-05-05 09:47:28.711430 PyBerries-0.2.6.post1/pyberries/
--rw-rw-rw-   0        0        0      118 2023-05-04 14:10:33.000000 PyBerries-0.2.6.post1/pyberries/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-05 09:47:28.724432 PyBerries-0.2.6.post1/pyberries/data/
--rw-rw-rw-   0        0        0    16096 2023-05-04 16:04:58.000000 PyBerries-0.2.6.post1/pyberries/data/DatasetPool.py
--rw-rw-rw-   0        0        0     1886 2023-05-04 10:56:45.000000 PyBerries-0.2.6.post1/pyberries/data/Fitting.py
--rw-rw-rw-   0        0        0       86 2023-05-02 15:00:14.000000 PyBerries-0.2.6.post1/pyberries/data/__init__.py
--rw-rw-rw-   0        0        0     1567 2023-05-02 15:50:42.000000 PyBerries-0.2.6.post1/pyberries/data/util.py
-drwxrwxrwx   0        0        0        0 2023-05-05 09:47:28.733458 PyBerries-0.2.6.post1/pyberries/file_utilities/
--rw-rw-rw-   0        0        0     2877 2023-03-14 14:43:41.000000 PyBerries-0.2.6.post1/pyberries/file_utilities/Filename_utils.py
--rw-rw-rw-   0        0        0     2782 2023-03-14 14:14:07.000000 PyBerries-0.2.6.post1/pyberries/file_utilities/Stack_tiffs.py
--rw-rw-rw-   0        0        0      795 2023-03-14 14:14:07.000000 PyBerries-0.2.6.post1/pyberries/file_utilities/Unpack_omero_folders.py
--rw-rw-rw-   0        0        0      119 2023-03-14 14:14:07.000000 PyBerries-0.2.6.post1/pyberries/file_utilities/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-05 09:47:28.733458 PyBerries-0.2.6.post1/pyberries/metrics/
--rw-rw-rw-   0        0        0     1242 2023-05-02 10:54:16.000000 PyBerries-0.2.6.post1/pyberries/metrics/Metrics.py
--rw-rw-rw-   0        0        0     6475 2023-05-03 12:50:51.000000 PyBerries-0.2.6.post1/pyberries/metrics/Time_metrics.py
--rw-rw-rw-   0        0        0       69 2023-03-10 16:15:28.000000 PyBerries-0.2.6.post1/pyberries/metrics/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-05 09:47:28.746485 PyBerries-0.2.6.post1/pyberries/plots/
--rw-rw-rw-   0        0        0     1037 2023-05-02 16:02:09.000000 PyBerries-0.2.6.post1/pyberries/plots/Fits.py
--rw-rw-rw-   0        0        0     4813 2023-05-04 10:28:45.000000 PyBerries-0.2.6.post1/pyberries/plots/Plot_presets.py
--rw-rw-rw-   0        0        0      353 2023-04-05 10:31:09.000000 PyBerries-0.2.6.post1/pyberries/plots/Plot_utilities.py
--rw-rw-rw-   0        0        0     1372 2023-04-03 13:51:01.000000 PyBerries-0.2.6.post1/pyberries/plots/Plots.py
--rw-rw-rw-   0        0        0      117 2023-05-02 10:54:16.000000 PyBerries-0.2.6.post1/pyberries/plots/__init__.py
--rw-rw-rw-   0        0        0       42 2023-05-05 09:47:28.759485 PyBerries-0.2.6.post1/setup.cfg
--rw-rw-rw-   0        0        0      631 2023-05-05 09:45:04.000000 PyBerries-0.2.6.post1/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-05 15:52:40.351626 PyBerries-0.2.7/
+-rw-rw-rw-   0        0        0    33074 2022-12-22 10:37:47.000000 PyBerries-0.2.7/LICENSE
+-rw-rw-rw-   0        0        0    13971 2023-05-05 15:52:40.351626 PyBerries-0.2.7/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-05-05 15:52:40.319625 PyBerries-0.2.7/PyBerries.egg-info/
+-rw-rw-rw-   0        0        0    13971 2023-05-05 15:52:40.000000 PyBerries-0.2.7/PyBerries.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      723 2023-05-05 15:52:40.000000 PyBerries-0.2.7/PyBerries.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-05 15:52:40.000000 PyBerries-0.2.7/PyBerries.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      135 2023-05-05 15:52:40.000000 PyBerries-0.2.7/PyBerries.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-05-05 15:52:40.000000 PyBerries-0.2.7/PyBerries.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0    13653 2023-05-05 12:20:59.000000 PyBerries-0.2.7/README.md
+drwxrwxrwx   0        0        0        0 2023-05-05 15:52:40.323625 PyBerries-0.2.7/pyberries/
+-rw-rw-rw-   0        0        0      118 2023-05-04 14:10:33.000000 PyBerries-0.2.7/pyberries/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-05 15:52:40.331703 PyBerries-0.2.7/pyberries/data/
+-rw-rw-rw-   0        0        0    16106 2023-05-05 15:50:23.000000 PyBerries-0.2.7/pyberries/data/DatasetPool.py
+-rw-rw-rw-   0        0        0     1886 2023-05-04 10:56:45.000000 PyBerries-0.2.7/pyberries/data/Fitting.py
+-rw-rw-rw-   0        0        0       86 2023-05-02 15:00:14.000000 PyBerries-0.2.7/pyberries/data/__init__.py
+-rw-rw-rw-   0        0        0     1567 2023-05-02 15:50:42.000000 PyBerries-0.2.7/pyberries/data/util.py
+drwxrwxrwx   0        0        0        0 2023-05-05 15:52:40.335624 PyBerries-0.2.7/pyberries/file_utilities/
+-rw-rw-rw-   0        0        0     2877 2023-03-14 14:43:41.000000 PyBerries-0.2.7/pyberries/file_utilities/Filename_utils.py
+-rw-rw-rw-   0        0        0     2782 2023-03-14 14:14:07.000000 PyBerries-0.2.7/pyberries/file_utilities/Stack_tiffs.py
+-rw-rw-rw-   0        0        0      795 2023-03-14 14:14:07.000000 PyBerries-0.2.7/pyberries/file_utilities/Unpack_omero_folders.py
+-rw-rw-rw-   0        0        0      119 2023-03-14 14:14:07.000000 PyBerries-0.2.7/pyberries/file_utilities/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-05 15:52:40.339626 PyBerries-0.2.7/pyberries/metrics/
+-rw-rw-rw-   0        0        0     1242 2023-05-02 10:54:16.000000 PyBerries-0.2.7/pyberries/metrics/Metrics.py
+-rw-rw-rw-   0        0        0     6475 2023-05-03 12:50:51.000000 PyBerries-0.2.7/pyberries/metrics/Time_metrics.py
+-rw-rw-rw-   0        0        0       69 2023-03-10 16:15:28.000000 PyBerries-0.2.7/pyberries/metrics/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-05 15:52:40.347625 PyBerries-0.2.7/pyberries/plots/
+-rw-rw-rw-   0        0        0     1037 2023-05-02 16:02:09.000000 PyBerries-0.2.7/pyberries/plots/Fits.py
+-rw-rw-rw-   0        0        0     4813 2023-05-04 10:28:45.000000 PyBerries-0.2.7/pyberries/plots/Plot_presets.py
+-rw-rw-rw-   0        0        0      353 2023-04-05 10:31:09.000000 PyBerries-0.2.7/pyberries/plots/Plot_utilities.py
+-rw-rw-rw-   0        0        0     1372 2023-04-03 13:51:01.000000 PyBerries-0.2.7/pyberries/plots/Plots.py
+-rw-rw-rw-   0        0        0      117 2023-05-02 10:54:16.000000 PyBerries-0.2.7/pyberries/plots/__init__.py
+-rw-rw-rw-   0        0        0       42 2023-05-05 15:52:40.351626 PyBerries-0.2.7/setup.cfg
+-rw-rw-rw-   0        0        0      690 2023-05-05 15:51:17.000000 PyBerries-0.2.7/setup.py
```

### Comparing `PyBerries-0.2.6.post1/LICENSE` & `PyBerries-0.2.7/LICENSE`

 * *Files identical despite different names*

### Comparing `PyBerries-0.2.6.post1/PKG-INFO` & `PyBerries-0.2.7/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -1,18 +1,7 @@
-Metadata-Version: 2.1
-Name: PyBerries
-Version: 0.2.6.post1
-Summary: Processing of Bacmman measurement tables
-Home-page: https://gitlab.com/MEKlab/pyberries
-Author: Daniel Thedie
-Author-email: daniel.thedie@ed.ac.uk
-Requires-Python: >=3.9
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # PyBerries
 
 PyBerries is a Python package that can be used to import, manipulate and plot data from Bacmman measurement tables.
 
 It relies mainly on Pandas for data handling and Seaborn/Matplotlib for plotting.
 
 [[_TOC_]]
@@ -25,33 +14,25 @@
   <summary markdown="span">Anaconda (recommended)</summary>
 
   Anaconda will install both Python and Jupyter-lab (used to run Python notebooks) easily. Note however that it requires ~5 Gb free disk space.
   For a lighter installation procedure, see the next section "Command line install".
 
   - Download Anaconda from the [official website](https://www.anaconda.com/)
   - Run the installer (leave all options as default)
-  - Check git is installed on your computer
-      - Open a terminal (macOS/Linux) or Powershell (Windows)
-      - Enter the command `git --version`
-      - If an error is shown, download and install git from [here](https://git-scm.com/downloads) (leave all install options as default)
-      - After installing, restart your terminal/powershell; the `git --version` command should display a version number (e.g. 2.40.0)
   - Start "Anaconda Navigator"
   - In Anaconda, launch the "Jupyter Lab" module
 </details>
 
 <details>
   <summary markdown="span">Command line install (advanced users)</summary>
 
   - Open a terminal (macOS/Linux) or Powershell (Windows)
   - Install Python
       - Enter the command `python --version`
-      - If an error or a version < 3.8 is shown, download and install Python from the [official website](https://www.python.org/downloads/)
-  - Install git
-      - Enter the command `git --version`
-      - If an error is shown, download and install git from [here](https://git-scm.com/downloads) (leave all install options as default)
+      - If an error or a version < 3.9 is shown, download and install Python from the [official website](https://www.python.org/downloads/)
   - After installing, restart your terminal/powershell; both of the above commands should display a version number
   - Install Jupyter Lab
       - In a terminal/powershell, run the command `python -m pip install jupyterlab`
       - After the installation completes, Jupyter Lab can be started using the command `jupyter-lab`
 </details>
 
 ## Using existing notebooks
@@ -71,17 +52,21 @@
 
 ## Using the PyBerries package in your own code (advanced users)
 
 To install the package, use the following command in a terminal:
 
 `python -m pip install PyBerries`
 
+You can also install a specific version number (useful e.g. to make sure you code won't be broken by a future update):
+
+`python -m pip install PyBerries==0.2.6.post1`
+
 ### Creating a DatasetPool
 
-ðŸ“– [DatasetPool documentation](./doc/DatasetPool.md)
+📖 [DatasetPool documentation](./doc/DatasetPool.md)
 
 To import Bacmman measurement tables with PyBerries, you must create a "DatasetPool" (an object that will contain one or several Bacmman datasets). The minimum required arguments to create a DatasetPool are:
 - `dsList`: name(s) of the Bacmman datasets to be imported
 - `path`: path to the Bacmman folder containing the datasets
 
 Optional arguments can be added:
 - `groups`: set legend labels for the datasets. If two datasets have the same label, they will be concatenated (and error bars can be shown if supported)
@@ -243,15 +228,15 @@
 plot_args = {'x':'Bacteria_Size',
             'hue':'Group',
             'binwidth':2,
             'stat':'probability',
             'common_norm':False,
             'errorbars':None,
             'title':'',
-            'xlabel':'Cell area (Âµm$^2$)',
+            'xlabel':'Cell area (µm$^2$)',
             'ylabel':'Probability',
             'xlim':(None, None),
             'ylim':(None, None),
             'multiple':'layer',
             'element':'poly',
             'kde':False,
             'palette':'deep',
@@ -279,15 +264,15 @@
 
 plot_args = {'x':'Bacteria_Size',
             'hue':'Group',
             'binwidth':2,
             'stat':'probability',
             'common_norm':False,
             'title':'',
-            'xlabel':'Cell area (Âµm$^2$)',
+            'xlabel':'Cell area (µm$^2$)',
             'ylabel':'Probability',
             'xlim':(None, None),
             'ylim':(None, None),
             'multiple':'layer',
             'element':'poly',
             'kde':False,
             'palette':'deep',
@@ -315,15 +300,15 @@
             'element':'poly',
             'kde':False,
             'palette':'deep',
             }
 
 _,ax = plt.subplots(dpi=130)
 g = sns.histplot(data=data.table['Bacteria'], **plot_args)
-g.set(xlabel='Cell area (Âµm$^2$)', ylabel='Probability', title='Plot title', xlim=(None, None), ylim=(None, None))
+g.set(xlabel='Cell area (µm$^2$)', ylabel='Probability', title='Plot title', xlim=(None, None), ylim=(None, None))
 if not g.get_legend() == None: g.get_legend().set_title("")
 ```
 
 
 
 ## File utilities
 Collection of functions to manipulate:
```

### Comparing `PyBerries-0.2.6.post1/PyBerries.egg-info/PKG-INFO` & `PyBerries-0.2.7/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PyBerries
-Version: 0.2.6.post1
+Version: 0.2.7
 Summary: Processing of Bacmman measurement tables
 Home-page: https://gitlab.com/MEKlab/pyberries
 Author: Daniel Thedie
 Author-email: daniel.thedie@ed.ac.uk
 Requires-Python: >=3.9
 Description-Content-Type: text/markdown
 License-File: LICENSE
@@ -25,33 +25,25 @@
   <summary markdown="span">Anaconda (recommended)</summary>
 
   Anaconda will install both Python and Jupyter-lab (used to run Python notebooks) easily. Note however that it requires ~5 Gb free disk space.
   For a lighter installation procedure, see the next section "Command line install".
 
   - Download Anaconda from the [official website](https://www.anaconda.com/)
   - Run the installer (leave all options as default)
-  - Check git is installed on your computer
-      - Open a terminal (macOS/Linux) or Powershell (Windows)
-      - Enter the command `git --version`
-      - If an error is shown, download and install git from [here](https://git-scm.com/downloads) (leave all install options as default)
-      - After installing, restart your terminal/powershell; the `git --version` command should display a version number (e.g. 2.40.0)
   - Start "Anaconda Navigator"
   - In Anaconda, launch the "Jupyter Lab" module
 </details>
 
 <details>
   <summary markdown="span">Command line install (advanced users)</summary>
 
   - Open a terminal (macOS/Linux) or Powershell (Windows)
   - Install Python
       - Enter the command `python --version`
-      - If an error or a version < 3.8 is shown, download and install Python from the [official website](https://www.python.org/downloads/)
-  - Install git
-      - Enter the command `git --version`
-      - If an error is shown, download and install git from [here](https://git-scm.com/downloads) (leave all install options as default)
+      - If an error or a version < 3.9 is shown, download and install Python from the [official website](https://www.python.org/downloads/)
   - After installing, restart your terminal/powershell; both of the above commands should display a version number
   - Install Jupyter Lab
       - In a terminal/powershell, run the command `python -m pip install jupyterlab`
       - After the installation completes, Jupyter Lab can be started using the command `jupyter-lab`
 </details>
 
 ## Using existing notebooks
@@ -71,14 +63,18 @@
 
 ## Using the PyBerries package in your own code (advanced users)
 
 To install the package, use the following command in a terminal:
 
 `python -m pip install PyBerries`
 
+You can also install a specific version number (useful e.g. to make sure you code won't be broken by a future update):
+
+`python -m pip install PyBerries==0.2.6.post1`
+
 ### Creating a DatasetPool
 
 ðŸ“– [DatasetPool documentation](./doc/DatasetPool.md)
 
 To import Bacmman measurement tables with PyBerries, you must create a "DatasetPool" (an object that will contain one or several Bacmman datasets). The minimum required arguments to create a DatasetPool are:
 - `dsList`: name(s) of the Bacmman datasets to be imported
 - `path`: path to the Bacmman folder containing the datasets
```

### Comparing `PyBerries-0.2.6.post1/PyBerries.egg-info/SOURCES.txt` & `PyBerries-0.2.7/PyBerries.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `PyBerries-0.2.6.post1/README.md` & `PyBerries-0.2.7/PyBerries.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,7 +1,18 @@
+Metadata-Version: 2.1
+Name: PyBerries
+Version: 0.2.7
+Summary: Processing of Bacmman measurement tables
+Home-page: https://gitlab.com/MEKlab/pyberries
+Author: Daniel Thedie
+Author-email: daniel.thedie@ed.ac.uk
+Requires-Python: >=3.9
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # PyBerries
 
 PyBerries is a Python package that can be used to import, manipulate and plot data from Bacmman measurement tables.
 
 It relies mainly on Pandas for data handling and Seaborn/Matplotlib for plotting.
 
 [[_TOC_]]
@@ -14,33 +25,25 @@
   <summary markdown="span">Anaconda (recommended)</summary>
 
   Anaconda will install both Python and Jupyter-lab (used to run Python notebooks) easily. Note however that it requires ~5 Gb free disk space.
   For a lighter installation procedure, see the next section "Command line install".
 
   - Download Anaconda from the [official website](https://www.anaconda.com/)
   - Run the installer (leave all options as default)
-  - Check git is installed on your computer
-      - Open a terminal (macOS/Linux) or Powershell (Windows)
-      - Enter the command `git --version`
-      - If an error is shown, download and install git from [here](https://git-scm.com/downloads) (leave all install options as default)
-      - After installing, restart your terminal/powershell; the `git --version` command should display a version number (e.g. 2.40.0)
   - Start "Anaconda Navigator"
   - In Anaconda, launch the "Jupyter Lab" module
 </details>
 
 <details>
   <summary markdown="span">Command line install (advanced users)</summary>
 
   - Open a terminal (macOS/Linux) or Powershell (Windows)
   - Install Python
       - Enter the command `python --version`
-      - If an error or a version < 3.8 is shown, download and install Python from the [official website](https://www.python.org/downloads/)
-  - Install git
-      - Enter the command `git --version`
-      - If an error is shown, download and install git from [here](https://git-scm.com/downloads) (leave all install options as default)
+      - If an error or a version < 3.9 is shown, download and install Python from the [official website](https://www.python.org/downloads/)
   - After installing, restart your terminal/powershell; both of the above commands should display a version number
   - Install Jupyter Lab
       - In a terminal/powershell, run the command `python -m pip install jupyterlab`
       - After the installation completes, Jupyter Lab can be started using the command `jupyter-lab`
 </details>
 
 ## Using existing notebooks
@@ -60,17 +63,21 @@
 
 ## Using the PyBerries package in your own code (advanced users)
 
 To install the package, use the following command in a terminal:
 
 `python -m pip install PyBerries`
 
+You can also install a specific version number (useful e.g. to make sure you code won't be broken by a future update):
+
+`python -m pip install PyBerries==0.2.6.post1`
+
 ### Creating a DatasetPool
 
-📖 [DatasetPool documentation](./doc/DatasetPool.md)
+ðŸ“– [DatasetPool documentation](./doc/DatasetPool.md)
 
 To import Bacmman measurement tables with PyBerries, you must create a "DatasetPool" (an object that will contain one or several Bacmman datasets). The minimum required arguments to create a DatasetPool are:
 - `dsList`: name(s) of the Bacmman datasets to be imported
 - `path`: path to the Bacmman folder containing the datasets
 
 Optional arguments can be added:
 - `groups`: set legend labels for the datasets. If two datasets have the same label, they will be concatenated (and error bars can be shown if supported)
@@ -232,15 +239,15 @@
 plot_args = {'x':'Bacteria_Size',
             'hue':'Group',
             'binwidth':2,
             'stat':'probability',
             'common_norm':False,
             'errorbars':None,
             'title':'',
-            'xlabel':'Cell area (µm$^2$)',
+            'xlabel':'Cell area (Âµm$^2$)',
             'ylabel':'Probability',
             'xlim':(None, None),
             'ylim':(None, None),
             'multiple':'layer',
             'element':'poly',
             'kde':False,
             'palette':'deep',
@@ -268,15 +275,15 @@
 
 plot_args = {'x':'Bacteria_Size',
             'hue':'Group',
             'binwidth':2,
             'stat':'probability',
             'common_norm':False,
             'title':'',
-            'xlabel':'Cell area (µm$^2$)',
+            'xlabel':'Cell area (Âµm$^2$)',
             'ylabel':'Probability',
             'xlim':(None, None),
             'ylim':(None, None),
             'multiple':'layer',
             'element':'poly',
             'kde':False,
             'palette':'deep',
@@ -304,15 +311,15 @@
             'element':'poly',
             'kde':False,
             'palette':'deep',
             }
 
 _,ax = plt.subplots(dpi=130)
 g = sns.histplot(data=data.table['Bacteria'], **plot_args)
-g.set(xlabel='Cell area (µm$^2$)', ylabel='Probability', title='Plot title', xlim=(None, None), ylim=(None, None))
+g.set(xlabel='Cell area (Âµm$^2$)', ylabel='Probability', title='Plot title', xlim=(None, None), ylim=(None, None))
 if not g.get_legend() == None: g.get_legend().set_title("")
 ```
 
 
 
 ## File utilities
 Collection of functions to manipulate:
```

### Comparing `PyBerries-0.2.6.post1/pyberries/data/DatasetPool.py` & `PyBerries-0.2.7/pyberries/data/DatasetPool.py`

 * *Files 0% similar despite different names*

```diff
@@ -66,15 +66,15 @@
                     if len(preprocessing[obj]) == 1:
                         df_in = df_in.transform(preprocessing[obj][0])
                     elif len(preprocessing[obj]) > 1:
                         assert len(preprocessing[obj]) == len(self.dsList), 'If multiple pre-processings are provided, there should be one per dataset'
                         if preprocessing[obj][i]:
                             df_in = df_in.transform(preprocessing[obj][i])
                 self.table[obj] = df_in if obj not in self.table.keys() else pd.concat([self.table[obj], df_in], axis=0)
-                self.parent[obj] = object_class_names[object_parents[k][0]+1] if object_parents[k] else 'Viewfield'
+                self.parent[obj] = object_class_names[object_parents[k][0]-start_table] if object_parents[k] else 'Viewfield'
                 self.channel[obj] = channel_images[k][0]
                 k+=1
             print(f'Dataset {ds}: loaded objects {object_class_names}')
         self.objects = self.table.keys()
         for data in self.table.values():
             data.reset_index(drop=True, inplace=True)
```

### Comparing `PyBerries-0.2.6.post1/pyberries/data/Fitting.py` & `PyBerries-0.2.7/pyberries/data/Fitting.py`

 * *Files identical despite different names*

### Comparing `PyBerries-0.2.6.post1/pyberries/data/util.py` & `PyBerries-0.2.7/pyberries/data/util.py`

 * *Files identical despite different names*

### Comparing `PyBerries-0.2.6.post1/pyberries/file_utilities/Filename_utils.py` & `PyBerries-0.2.7/pyberries/file_utilities/Filename_utils.py`

 * *Files identical despite different names*

### Comparing `PyBerries-0.2.6.post1/pyberries/file_utilities/Stack_tiffs.py` & `PyBerries-0.2.7/pyberries/file_utilities/Stack_tiffs.py`

 * *Files identical despite different names*

### Comparing `PyBerries-0.2.6.post1/pyberries/file_utilities/Unpack_omero_folders.py` & `PyBerries-0.2.7/pyberries/file_utilities/Unpack_omero_folders.py`

 * *Files identical despite different names*

### Comparing `PyBerries-0.2.6.post1/pyberries/metrics/Metrics.py` & `PyBerries-0.2.7/pyberries/metrics/Metrics.py`

 * *Files identical despite different names*

### Comparing `PyBerries-0.2.6.post1/pyberries/metrics/Time_metrics.py` & `PyBerries-0.2.7/pyberries/metrics/Time_metrics.py`

 * *Files identical despite different names*

### Comparing `PyBerries-0.2.6.post1/pyberries/plots/Fits.py` & `PyBerries-0.2.7/pyberries/plots/Fits.py`

 * *Files identical despite different names*

### Comparing `PyBerries-0.2.6.post1/pyberries/plots/Plot_presets.py` & `PyBerries-0.2.7/pyberries/plots/Plot_presets.py`

 * *Files identical despite different names*

### Comparing `PyBerries-0.2.6.post1/pyberries/plots/Plots.py` & `PyBerries-0.2.7/pyberries/plots/Plots.py`

 * *Files identical despite different names*

### Comparing `PyBerries-0.2.6.post1/setup.py` & `PyBerries-0.2.7/setup.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,18 +1,18 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="PyBerries",
-    version="0.2.6.post1",
+    version="0.2.7",
     author="Daniel Thedie",
     author_email="daniel.thedie@ed.ac.uk",
     description="Processing of Bacmman measurement tables",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://gitlab.com/MEKlab/pyberries",
     packages=setuptools.find_packages(),
     python_requires='>=3.9',
-    install_requires=['numpy', 'scipy', 'pandas', 'matplotlib', 'tifffile', 'h5py','seaborn', 'pybacmman', 'IPython']
+    install_requires=['numpy>=1.24.3', 'scipy>=1.10', 'pandas>=2.0', 'matplotlib>=3.7', 'tifffile>=2023.4.12', 'h5py>=3.8.0','seaborn>=0.12.2', 'pybacmman>=0.5.1', 'IPython>=8.13.2']
 )
```

