# Comparing `tmp/jmspack-0.1.1.tar.gz` & `tmp/jmspack-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "jmspack-0.1.1.tar", last modified: Sat Dec 11 17:22:44 2021, max compression
+gzip compressed data, was "jmspack-0.1.2.tar", last modified: Fri May  5 14:33:55 2023, max compression
```

## Comparing `jmspack-0.1.1.tar` & `jmspack-0.1.2.tar`

### file list

```diff
@@ -1,19 +1,21 @@
-drwxr-xr-x   0 jamestwose   (501) staff       (20)        0 2021-12-11 17:22:44.997387 jmspack-0.1.1/
--rw-r--r--   0 jamestwose   (501) staff       (20)     1519 2021-03-13 13:16:25.000000 jmspack-0.1.1/LICENSE
--rw-r--r--   0 jamestwose   (501) staff       (20)     1648 2021-12-11 17:22:44.997177 jmspack-0.1.1/PKG-INFO
--rw-r--r--   0 jamestwose   (501) staff       (20)     1347 2021-12-11 17:08:29.000000 jmspack-0.1.1/README.md
-drwxr-xr-x   0 jamestwose   (501) staff       (20)        0 2021-12-11 17:22:44.995593 jmspack-0.1.1/jmspack/
--rw-r--r--   0 jamestwose   (501) staff       (20)    26914 2021-11-13 21:55:38.000000 jmspack-0.1.1/jmspack/NLTSA.py
--rw-r--r--   0 jamestwose   (501) staff       (20)       22 2021-12-11 17:09:41.000000 jmspack-0.1.1/jmspack/__init__.py
--rw-r--r--   0 jamestwose   (501) staff       (20)    29116 2021-12-11 17:08:29.000000 jmspack-0.1.1/jmspack/frequentist_statistics.py
--rw-r--r--   0 jamestwose   (501) staff       (20)    10725 2021-11-13 21:55:38.000000 jmspack-0.1.1/jmspack/internal_utils.py
--rw-r--r--   0 jamestwose   (501) staff       (20)    30399 2021-12-11 17:08:29.000000 jmspack-0.1.1/jmspack/ml_utils.py
--rw-r--r--   0 jamestwose   (501) staff       (20)     5054 2021-12-11 17:08:29.000000 jmspack-0.1.1/jmspack/utils.py
-drwxr-xr-x   0 jamestwose   (501) staff       (20)        0 2021-12-11 17:22:44.996849 jmspack-0.1.1/jmspack.egg-info/
--rw-r--r--   0 jamestwose   (501) staff       (20)     1648 2021-12-11 17:22:44.000000 jmspack-0.1.1/jmspack.egg-info/PKG-INFO
--rw-r--r--   0 jamestwose   (501) staff       (20)      314 2021-12-11 17:22:44.000000 jmspack-0.1.1/jmspack.egg-info/SOURCES.txt
--rw-r--r--   0 jamestwose   (501) staff       (20)        1 2021-12-11 17:22:44.000000 jmspack-0.1.1/jmspack.egg-info/dependency_links.txt
--rw-r--r--   0 jamestwose   (501) staff       (20)       74 2021-12-11 17:22:44.000000 jmspack-0.1.1/jmspack.egg-info/requires.txt
--rw-r--r--   0 jamestwose   (501) staff       (20)        8 2021-12-11 17:22:44.000000 jmspack-0.1.1/jmspack.egg-info/top_level.txt
--rw-r--r--   0 jamestwose   (501) staff       (20)       38 2021-12-11 17:22:44.997454 jmspack-0.1.1/setup.cfg
--rw-r--r--   0 jamestwose   (501) staff       (20)     1588 2021-12-11 17:08:29.000000 jmspack-0.1.1/setup.py
+drwxr-xr-x   0 jamestwose   (501) staff       (20)        0 2023-05-05 14:33:55.763434 jmspack-0.1.2/
+-rw-r--r--   0 jamestwose   (501) staff       (20)     1519 2023-05-05 13:37:00.000000 jmspack-0.1.2/LICENSE
+-rw-r--r--   0 jamestwose   (501) staff       (20)     2441 2023-05-05 14:33:55.763188 jmspack-0.1.2/PKG-INFO
+-rw-r--r--   0 jamestwose   (501) staff       (20)     2160 2023-05-05 13:37:00.000000 jmspack-0.1.2/README.md
+drwxr-xr-x   0 jamestwose   (501) staff       (20)        0 2023-05-05 14:33:55.761456 jmspack-0.1.2/jmspack/
+-rw-r--r--   0 jamestwose   (501) staff       (20)    28089 2023-05-05 13:37:02.000000 jmspack-0.1.2/jmspack/NLTSA.py
+-rw-r--r--   0 jamestwose   (501) staff       (20)       22 2023-05-05 13:37:02.000000 jmspack-0.1.2/jmspack/__init__.py
+-rw-r--r--   0 jamestwose   (501) staff       (20)    30962 2023-05-05 13:37:02.000000 jmspack-0.1.2/jmspack/frequentist_statistics.py
+-rw-r--r--   0 jamestwose   (501) staff       (20)     4330 2023-05-05 13:37:02.000000 jmspack-0.1.2/jmspack/imputation_utils.py
+-rw-r--r--   0 jamestwose   (501) staff       (20)    10761 2023-05-05 13:37:02.000000 jmspack-0.1.2/jmspack/internal_utils.py
+-rw-r--r--   0 jamestwose   (501) staff       (20)    36945 2023-05-05 13:37:02.000000 jmspack-0.1.2/jmspack/ml_utils.py
+-rw-r--r--   0 jamestwose   (501) staff       (20)     5090 2023-05-05 13:37:02.000000 jmspack-0.1.2/jmspack/networks.py
+-rw-r--r--   0 jamestwose   (501) staff       (20)     5675 2023-05-05 13:37:02.000000 jmspack-0.1.2/jmspack/utils.py
+drwxr-xr-x   0 jamestwose   (501) staff       (20)        0 2023-05-05 14:33:55.762861 jmspack-0.1.2/jmspack.egg-info/
+-rw-r--r--   0 jamestwose   (501) staff       (20)     2441 2023-05-05 14:33:55.000000 jmspack-0.1.2/jmspack.egg-info/PKG-INFO
+-rw-r--r--   0 jamestwose   (501) staff       (20)      362 2023-05-05 14:33:55.000000 jmspack-0.1.2/jmspack.egg-info/SOURCES.txt
+-rw-r--r--   0 jamestwose   (501) staff       (20)        1 2023-05-05 14:33:55.000000 jmspack-0.1.2/jmspack.egg-info/dependency_links.txt
+-rw-r--r--   0 jamestwose   (501) staff       (20)       74 2023-05-05 14:33:55.000000 jmspack-0.1.2/jmspack.egg-info/requires.txt
+-rw-r--r--   0 jamestwose   (501) staff       (20)        8 2023-05-05 14:33:55.000000 jmspack-0.1.2/jmspack.egg-info/top_level.txt
+-rw-r--r--   0 jamestwose   (501) staff       (20)       38 2023-05-05 14:33:55.763503 jmspack-0.1.2/setup.cfg
+-rw-r--r--   0 jamestwose   (501) staff       (20)     1588 2023-05-05 13:37:02.000000 jmspack-0.1.2/setup.py
```

### Comparing `jmspack-0.1.1/LICENSE` & `jmspack-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `jmspack-0.1.1/PKG-INFO` & `jmspack-0.1.2/README.md`

 * *Files 19% similar despite different names*

```diff
@@ -1,23 +1,20 @@
-Metadata-Version: 2.1
-Name: jmspack
-Version: 0.1.1
-Summary: James Data Science package
-Home-page: https://github.com/jameshtwose/jmspack
-Author: James Twose
-Author-email: contact@jamestwose.com
-License: BSD (3-clause)
-Platform: UNKNOWN
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # jmspack
 
+<p align="center">
+<img src="https://raw.githubusercontent.com/jameshtwose/jmspack/main/docs/source/_static/jmspack_logo.png" alt="drawing" width="150"/>
+</p>
+
 ## Python package of functions that James finds useful
 
+[![codecov](https://img.shields.io/codecov/c/github/jameshtwose/jmspack)](https://app.codecov.io/gh/jameshtwose/jmspack)
+[![Code Style](https://img.shields.io/badge/code%20style-black-000000.svg)](https://github.com/psf/black)
+[![Actions Passing](https://img.shields.io/badge/python-3.8%20%7C%203.9-blue)](https://github.com/Neurocast/data-science-core/actions)
+
+
 The documentation for the package can be found [here](https://docs.jms.rocks).
 [![Netlify Status](https://api.netlify.com/api/v1/badges/4de4fdcb-e2f0-4178-8f3f-cff4ecbeea3d/deploy-status)](https://app.netlify.com/sites/romantic-franklin-818651/deploys)
 
 The package can be installed via [conda](https://anaconda.org/james.twose/jmspack) using the following code: <br>
 `conda install -c james.twose jmspack`
 
 [![Anaconda-Server Badge](https://anaconda.org/james.twose/jmspack/badges/version.svg)](https://anaconda.org/james.twose/jmspack)
@@ -27,8 +24,16 @@
 
 The package can be installed via [pip](https://pypi.org/project/jmspack/) using the following code: <br>
 `pip install jmspack`
 
 [![PyPI version](https://badge.fury.io/py/jmspack.svg)](https://badge.fury.io/py/jmspack)
 [![PyPI download month](https://img.shields.io/pypi/dm/jmspack.svg)](https://pypi.python.org/pypi/jmspack/)
 
-
+### Installation from github
+- Clone the repository
+- `git clone git@github.com:jameshtwose/jmspack.git`
+- Create a virtual environment
+- `python3 -m venv venv`
+- Activate the virtual environment
+- `source venv/bin/activate`
+- Install the requirements
+- `pip install -r requirements.txt`
```

### Comparing `jmspack-0.1.1/jmspack/NLTSA.py` & `jmspack-0.1.2/jmspack/NLTSA.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,17 +1,25 @@
-r"""Submodule NLTSA.py includes the following functions: <br>
-- **fluctuation_intensity():** run fluctuation intensity on a time series to detect non linear change <br>
-- **distribution_uniformity():** run distribution uniformity on a time series to detect non linear change <br>
-- **complexity_resonance():** the product of fluctuation_intensity and distribution_uniformity <br>
-- **complexity_resonance_diagram():** plots a heatmap of the complexity_resonance <br>
-- **ts_levels():** defines distinct levels in a time series based on decision tree regressor <br>
-- **cmaps_options[]:** a list of possible colour maps that may be used when plotting <br>
-- **cumulative_complexity_peaks():** a function which will calculate the significant peaks in the dynamic
-complexity of a set of time series (these peaks are known as cumulative complexity peaks; CCPs) <br>
-- **cumulative_complexity_peaks_plot():** plots a heatmap of the cumulative_complexity_peaks <br>
+r"""Submodule NLTSA.py includes the following functions:
+
+- **fluctuation_intensity():** run fluctuation intensity on a time series to detect non linear change.
+
+- **distribution_uniformity():** run distribution uniformity on a time series to detect non linear change.
+
+- **complexity_resonance():** the product of fluctuation_intensity and distribution_uniformity.
+
+- **complexity_resonance_diagram():** plots a heatmap of the complexity_resonance.
+
+- **ts_levels():** defines distinct levels in a time series based on decision tree regressor.
+
+- **cmaps_options[]:** a list of possible colour maps that may be used when plotting.
+
+- **cumulative_complexity_peaks():** a function which will calculate the significant peaks in the dynamic complexity of a set of time series (these peaks are known as cumulative complexity peaks; CCPs).
+
+- **cumulative_complexity_peaks_plot():** plots a heatmap of the cumulative_complexity_peaks.
+
 """
 import matplotlib.patheffects as pe
 import matplotlib.pyplot as plt
 import numpy as np
 import pandas as pd
 import seaborn as sns
 from scipy.stats import norm
@@ -41,35 +49,36 @@
     "gist_ncar",
 ]
 
 
 def ts_levels(
     ts,
     ts_x=None,
-    criterion="mse",
+    criterion="squared_error",
     max_depth=2,
     min_samples_leaf=1,
     min_samples_split=2,
     max_leaf_nodes=30,
     plot=True,
     equal_spaced=True,
     n_x_ticks=10,
     figsize=(20, 5),
 ):
-    r"""Use recursive partitioning (DecisionTreeRegressor) to perform a 'classification' of relatively stable levels in a timeseries.
+    """Use recursive partitioning (DecisionTreeRegressor) to perform a 'classification' of relatively stable levels in a timeseries.
+
     Parameters
-    ---------
-    ts: pandas DataFrame (column)
+    ----------
+    ts: pd.DataFrame (column)
         A dataframe column containing a univariate time series from 1 person.
         Rows should indicate time, column should indicate the time series variable.
-    ts_x: pandas DataFrame (column; Default=None)
+    ts_x: pd.DataFrame (column; Default=None)
         A dataframe column containing the corresponding timestamps to the aforementioned time series.
         If None is passed, the index of the time series will be used (Default = None).
-    criterion: str (Default="mse")
-        The function to measure the quality of a split. Supported criteria are “mse” for the mean squared error, which
+    criterion: str (Default="squared_error")
+        The function to measure the quality of a split. Supported criteria are squared_error for the mean squared error, which
         is equal to variance reduction as feature selection criterion and minimizes the L2 loss using the mean of each
         terminal node, “friedman_mse”, which uses mean squared error with Friedman’s improvement score for potential
         splits, and “mae” for the mean absolute error, which minimizes the L1 loss using the median of each terminal node.
     max_depth: int or None, optional (default=2)
         The maximum depth of the tree. If None, then nodes are expanded until all leaves are pure or until all leaves
         contain less than min_samples_split samples.
     min_samples_leaf: int, float, optional (default=1)
@@ -93,22 +102,31 @@
         A boolean to define whether or not the time series is continuously measured or not. If False this will be taken
         into account when plotting the X-axis of the plot.
     n_x_ticks: int (Default=10)
         The amount of x-ticks you wish to show when plotting.
     figsize: tuple (Default=(20,5))
         The tuple used to specify the size of the plot if plot = True.
 
+    Returns
+    -------
+    df_result: pd.DataFrame
+        A dataframe containing the time steps, original time series and time series levels.
+    plt.figure.Figure
+        The matplotlib figure object.
+    plt.axes.Axes
+        The matplotlib axes object.
+
     Examples
-    ---------
-    Demonstration of the function using time series data
+    --------
     >>> from jmspack.NLTSA import ts_levels
     >>> ts_df = pd.read_csv("time_series_dataset.csv", index_col=0)
     >>> ts = ts_df["lorenz"]
-    >>> ts_levels_df, fig, ax = ts_levels(ts, ts_x=None, criterion="mse", max_depth=10, min_samples_leaf=1,
-    >>>                          min_samples_split=2, max_leaf_nodes=30, plot=True, equal_spaced=True, n_x_ticks=10)
+    >>> ts_levels_df, fig, ax = ts_levels(ts, ts_x=None, criterion="squared_error", max_depth=10, min_samples_leaf=1,
+    ...                          min_samples_split=2, max_leaf_nodes=30, plot=True, equal_spaced=True, n_x_ticks=10)
+
     """
     # Change ts to a numpy array
     if not isinstance(ts, np.ndarray):
         ts = ts.to_numpy()
     # Check whether ts has only one dimension
     if len(ts.shape) != 1:
         raise ValueError("ts is not one-dimensional")
@@ -203,18 +221,19 @@
     if ts_x is not None:
         df_result["ts_x"] = ts_x
 
     return df_result, fig, ax
 
 
 def distribution_uniformity(df, win, xmin, xmax, col_first, col_last):
-    r"""Run distribution uniformity on a time series to detect non linear change
+    """Run distribution uniformity on a time series to detect non linear change
+
     Parameters
-    ---------
-    df: pandas DataFrame
+    ----------
+    df: pd.DataFrame
         A dataframe containing multivariate time series data from 1 person.
         Rows should indicate time, columns should indicate the time series variables.
         All time series in df should be on the same scale. Otherwise the comparisons across
         time series will make no sense.
     win: int
         Size of sliding window in which to calculate distribution uniformity
         (amount of data considered in each evaluation of change).
@@ -223,22 +242,27 @@
     xmax: int
         The theoretical maximum that the values in the time series can take (scaling?)
     col_first: int
         The first column index you wish to be included in the calculation (index starts at 1!)
     col_last: int
         The last column index you wish to be included in the calculation (index starts at 1!)
 
+    Returns
+    -------
+    distribution_uniformity_df: pd.DataFrame
+        A dataframe containing the distribution uniformity values from multivariate time series data from 1 person.
+
     Examples
-    ---------
-    Demonstration of the function using time series data
+    --------
     >>> ts_df = pd.read_csv("time_series_dataset.csv", index_col=0)
     >>> scaler = MinMaxScaler()
     >>> scaled_ts_df = pd.DataFrame(scaler.fit_transform(ts_df), columns=ts_df.columns.tolist())
     >>> distribution_uniformity_df = pd.DataFrame(distribution_uniformity(scaled_ts_df, win=7, xmin=0, xmax=1, col_first=1, col_last=7))
     >>> distribution_uniformity_df.columns=scaled_ts_df.columns.tolist()
+
     """
 
     col_first = int(col_first)
     col_last = int(col_last)
     win = int(win)
     xmin = int(xmin)
     xmax = int(xmax)
@@ -276,18 +300,19 @@
         distribution_uniformity_df.columns = df.columns.tolist()
         distribution_uniformity_df.index = df.index.tolist()
 
     return distribution_uniformity_df
 
 
 def fluctuation_intensity(df, win, xmin, xmax, col_first, col_last):
-    r"""Run fluctuation intensity on a time series to detect non linear change
+    """Run fluctuation intensity on a time series to detect non linear change
+
     Parameters
-    ---------
-    df: pandas DataFrame
+    ----------
+    df: pd.DataFrame
         A dataframe containing multivariate time series data from 1 person.
         Rows should indicate time, columns should indicate the time series variables.
         All time series in df should be on the same scale. Otherwise the comparisons across
         time series will make no sense.
     win: int
         Size of sliding window in which to calculate fluctuation intensity
         (amount of data considered in each evaluation of change).
@@ -296,22 +321,27 @@
     xmax: int
         The theoretical maximum that the values in the time series can take (scaling?)
     col_first: int
         The first column index you wish to be included in the calculation (index starts at 1!)
     col_last: int
         The last column index you wish to be included in the calculation (index starts at 1!)
 
+    Returns
+    -------
+    fluctuation_intensity_df: pd.DataFrame
+        A dataframe containing the fluctuation intensity values from multivariate time series data from 1 person.
+
     Examples
-    ---------
-    Demonstration of the function using time series data
+    --------
     >>> ts_df = pd.read_csv("time_series_dataset.csv", index_col=0)
     >>> scaler = MinMaxScaler()
     >>> scaled_ts_df = pd.DataFrame(scaler.fit_transform(ts_df), columns=ts_df.columns.tolist())
     >>> fluctuation_intensity_df = pd.DataFrame(fluctuation_intensity(scaled_ts_df, win=7, xmin=0, xmax=1, col_first=1, col_last=7))
     >>> fluctuation_intensity_df.columns=scaled_ts_df.columns.tolist()
+
     """
 
     col_first = int(col_first)
     col_last = int(col_last)
     win = int(win)
     xmin = int(xmin)
     xmax = int(xmax)
@@ -321,16 +351,16 @@
 
     ew_data_F = np.zeros((nrow, ncol))
     ew_data_F = pd.DataFrame(ew_data_F)
 
     newrows = df.iloc[0:1, :].copy()
     newrows.iloc[:, col_first - 1 : col_last] = 0.0
 
-    data = df.append(newrows)
-    data = data.append(newrows)
+    data = pd.concat([df, newrows])
+    data = pd.concat([data, newrows])
     data.reset_index(inplace=True, drop=True)
 
     s = xmax - xmin
     length_ts = len(data)
 
     for column in range(col_first - 1, col_last):
         distance = 1
@@ -381,50 +411,58 @@
         fluctuation_intensity_df.columns = df.columns.tolist()
         fluctuation_intensity_df.index = df.index.tolist()
 
     return fluctuation_intensity_df
 
 
 def complexity_resonance(distribution_uniformity_df, fluctuation_intensity_df):
-    r"""Create a complexity resonance data frame based on the product of the distribution uniformity and the fluctuation intensity
+    """Create a complexity resonance data frame based on the product of the distribution uniformity and the fluctuation intensity
+
     Parameters
-    ---------
+    ----------
     distribution_uniformity_df: pandas DataFrame
         A dataframe containing distribution uniformity values from multivariate time series data from 1 person.
         Rows should indicate time, columns should indicate the distribution uniformity.
     fluctuation_intensity_df: pandas DataFrame
         A dataframe containing fluctuation intensity values from multivariate time series data from 1 person.
         Rows should indicate time, columns should indicate the fluctuation intensity.
 
+    Returns
+    -------
+    complexity_resonance_df: pandas DataFrame
+        A dataframe containing the complexity resonance values from multivariate time series data from 1 person.
+
     Examples
-    ---------
-    Demonstration of the function using time series data
+    --------
     >>> ts_df = pd.read_csv("time_series_dataset.csv", index_col=0)
     >>> scaler = MinMaxScaler()
     >>> scaled_ts_df = pd.DataFrame(scaler.fit_transform(ts_df), columns=ts_df.columns.tolist())
     >>> distribution_uniformity_df = pd.DataFrame(distribution_uniformity(scaled_ts_df, win=7, xmin=0, xmax=1, col_first=1, col_last=7))
     >>> distribution_uniformity_df.columns=scaled_ts_df.columns.tolist()
     >>> fluctuation_intensity_df = pd.DataFrame(fluctuation_intensity(scaled_ts_df, win=7, xmin=0, xmax=1, col_first=1, col_last=7))
     >>> fluctuation_intensity_df.columns=scaled_ts_df.columns.tolist()
     >>> complexity_resonance_df = complexity_resonance(distribution_uniformity_df, fluctuation_intensity_df)
+
     """
+
     complexity_resonance_df = distribution_uniformity_df * fluctuation_intensity_df
     return complexity_resonance_df
 
 
 def complexity_resonance_diagram(
     df,
     cmap_n: int = 12,
     plot_title="Complexity Resonance Diagram",
     labels_n=10,
     figsize=(20, 7),
 ):
-    r"""Create a complexity resonance data frame based on the product of the distribution uniformity and the fluctuation intensity
+    """Create a complexity resonance data frame based on the product of the distribution uniformity and the fluctuation intensity
+
     Parameters
-    ---------
+    ----------
     df: pandas DataFrame
         A dataframe containing complexity resonance values from multivariate time series data from 1 person.
         Rows should indicate time, columns should indicate the complexity resonance.
     cmap_n: int (Default=12)
         An integer indicating which colour map to use when plotting the heatmap. These values correspond to the index
         of the cmaps_options list (['flag', 'prism', 'ocean', 'gist_earth', 'terrain', 'gist_stern',
         'gnuplot', 'gnuplot2', 'CMRmap', 'cubehelix', 'brg', 'gist_rainbow', 'rainbow', 'jet', 'nipy_spectral',
@@ -432,26 +470,33 @@
     plot_title: str
         A string indicating the title to be used at the top of the plot
     labels_n: int (Default=10)
         An integer indicating the nth value to be taken for the x-axis of the plot. So if the x-axis consists of
         1, 2, 3, 4, 5, 6, 7, 8, 9, 10, and the labels_n value is set to 2, then 2, 4, 6, 8, 10, will be shown on the
         x-axis of the plot.
 
+    Returns
+    -------
+    plt.figure.Figure
+        The matplotlib figure object.
+    plt.axes.Axes
+        The matplotlib axes object.
+
     Examples
-    ---------
-    Demonstration of the function using time series data
+    --------
     >>> ts_df = pd.read_csv("time_series_dataset.csv", index_col=0)
     >>> scaler = MinMaxScaler()
     >>> scaled_ts_df = pd.DataFrame(scaler.fit_transform(ts_df), columns=ts_df.columns.tolist())
     >>> distribution_uniformity_df = pd.DataFrame(distribution_uniformity(scaled_ts_df, win=7, xmin=0, xmax=1, col_first=1, col_last=7))
     >>> distribution_uniformity_df.columns=scaled_ts_df.columns.tolist()
     >>> fluctuation_intensity_df = pd.DataFrame(fluctuation_intensity(scaled_ts_df, win=7, xmin=0, xmax=1, col_first=1, col_last=7))
     >>> fluctuation_intensity_df.columns=scaled_ts_df.columns.tolist()
     >>> complexity_resonance_df = complexity_resonance(distribution_uniformity_df, fluctuation_intensity_df)
     >>> complexity_resonance_diagram(complexity_resonance_df, cmap_n=12, labels_n=30)
+
     """
 
     df_for_plot = df.copy()
     # df_for_plot.insert(loc=0, column="", value=np.nan)
 
     # plot the complexity resonance diagram
     fig, ax = plt.subplots(figsize=figsize)
@@ -478,49 +523,58 @@
         l.set_visible(False)
         for (i, l) in enumerate(ax.xaxis.get_ticklabels())
         if i % labels_n != 0
     ]
 
     # set the axis title
     ax.set_title(plot_title)
-    # plt.show()
 
-    return ax
+    return fig, ax
 
 
 def cumulative_complexity_peaks(
     df: pd.DataFrame,
     significant_level_item: float = 0.05,
     significant_level_time: float = 0.05,
 ):
-    r"""Create a complexity resonance data frame based on the product of the distribution uniformity and the fluctuation intensity
+    """Create a complexity resonance data frame based on the product of the distribution uniformity and the fluctuation intensity
+
     Parameters
-    ---------
-    df: pandas DataFrame
+    ----------
+    df: pd.DataFrame
         A dataframe containing complexity resonance values from multivariate time series data from 1 person.
         Rows should indicate time, columns should indicate the complexity resonance.
     significant_level_item: float (Default=0.05)
         A float indicating the cutoff of when a point in time is significantly different than the rest on an individual item level (i.e.
         is this time point different than all the other time points for this item/ feature).
     significant_level_time: float (Default=0.05)
         A float indicating the cutoff of when a point in time is significantly different than the rest on a timepoint level
         (i.e. is this day different than all the other days).
 
+    Returns
+    -------
+    ccp_df: pd.DataFrame
+        A dataframe containing the cumulative complexity peaks values from multivariate time series data from 1 person.
+        Rows indicate time, columns indicate the cumulative complexity peaks.
+    sig_peaks_df: pd.DataFrame
+        A dataframe containing one column of significant complexity peaks values from multivariate time series data from 1 person.
+        Rows indicate time, columns indicate the significant cumulative complexity peaks.
+
     Examples
-    ---------
-    Demonstration of the function using time series data
+    --------
     >>> ts_df = pd.read_csv("time_series_dataset.csv", index_col=0)
     >>> scaler = MinMaxScaler()
     >>> scaled_ts_df = pd.DataFrame(scaler.fit_transform(ts_df), columns=ts_df.columns.tolist())
     >>> distribution_uniformity_df = pd.DataFrame(distribution_uniformity(scaled_ts_df, win=7, xmin=0, xmax=1, col_first=1, col_last=7))
     >>> distribution_uniformity_df.columns=scaled_ts_df.columns.tolist()
     >>> fluctuation_intensity_df = pd.DataFrame(fluctuation_intensity(scaled_ts_df, win=7, xmin=0, xmax=1, col_first=1, col_last=7))
     >>> fluctuation_intensity_df.columns=scaled_ts_df.columns.tolist()
     >>> complexity_resonance_df = complexity_resonance(distribution_uniformity_df, fluctuation_intensity_df)
     >>> cumulative_complexity_peaks_df, significant_peaks_df = cumulative_complexity_peaks(df=complexity_resonance_df)
+
     """
 
     ## Creating CCP data frame
     z_scale_cr_df = pd.DataFrame(
         StandardScaler().fit_transform(df), columns=df.columns.tolist()
     )
     ccp_df = z_scale_cr_df.mask(
@@ -548,47 +602,55 @@
     cumulative_complexity_peaks_df: pd.DataFrame,
     significant_peaks_df: pd.DataFrame,
     plot_title: str = "Cumulative Complexity Peaks Plot",
     figsize: tuple = (20, 5),
     height_ratios: list = [1, 3],
     labels_n: int = 10,
 ):
-    r"""Create a cumulative complexity peaks plot based on the cumulative_complexity_peaks_df and the significant_peaks_df
+    """Create a cumulative complexity peaks plot based on the cumulative_complexity_peaks_df and the significant_peaks_df
+
     Parameters
-    ---------
-    cumulative_complexity_peaks_df: pandas DataFrame
+    ----------
+    cumulative_complexity_peaks_df: pdDataFrame
         A dataframe containing cumulative complexity peaks values from multivariate time series data from 1 person.
         Rows should indicate time, columns should indicate the cumulative complexity peaks.
-    significant_peaks_df: pandas DataFrame
+    significant_peaks_df: pd.DataFrame
         A dataframe containing one column of significant complexity peaks values from multivariate time series data from 1 person.
         Rows should indicate time, columns should indicate the significant cumulative complexity peaks.
     plot_title: str
         A string indicating the title to be used at the top of the plot
     figsize: tuple (Default=(20,5))
         The tuple used to specify the size of the plot.
     height_ratios: list (Default=[1,3])
         The tuple used to specify the size of the plot.
     labels_n: int (Default=10)
         An integer indicating the nth value to be taken for the x-axis of the plot. So if the x-axis consists of
         1, 2, 3, 4, 5, 6, 7, 8, 9, 10, and the labels_n value is set to 2, then 2, 4, 6, 8, 10, will be shown on the
         x-axis of the plot.
 
+    Returns
+    -------
+    plt.figure.Figure
+        The matplotlib figure object.
+    plt.axes.Axes
+        The matplotlib axes object.
+
     Examples
-    ---------
-    Demonstration of the function using time series data
+    --------
     >>> ts_df = pd.read_csv("datasets/time_series_dataset.csv", index_col=0)
     >>> scaler = MinMaxScaler()
     >>> scaled_ts_df = pd.DataFrame(scaler.fit_transform(ts_df), columns=ts_df.columns.tolist())
     >>> distribution_uniformity_df = pd.DataFrame(distribution_uniformity(scaled_ts_df, win=7, xmin=0, xmax=1, col_first=1, col_last=7))
     >>> distribution_uniformity_df.columns=scaled_ts_df.columns.tolist()
     >>> fluctuation_intensity_df = pd.DataFrame(fluctuation_intensity(scaled_ts_df, win=7, xmin=0, xmax=1, col_first=1, col_last=7))
     >>> fluctuation_intensity_df.columns=scaled_ts_df.columns.tolist()
     >>> complexity_resonance_df = complexity_resonance(distribution_uniformity_df, fluctuation_intensity_df)
     >>> cumulative_complexity_peaks_df, significant_peaks_df = cumulative_complexity_peaks(df=complexity_resonance_df)
     >>> _ = cumulative_complexity_peaks_plot(cumulative_complexity_peaks_df=cumulative_complexity_peaks_df, significant_peaks_df=significant_peaks_df)
+
     """
     custom_cmap = sns.color_palette(["#FFFFFF", "#000000"])
 
     fig, axes = plt.subplots(
         2, 1, figsize=figsize, gridspec_kw={"height_ratios": height_ratios}
     )
```

### Comparing `jmspack-0.1.1/jmspack/frequentist_statistics.py` & `jmspack-0.1.2/jmspack/frequentist_statistics.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,53 +1,65 @@
-r"""Submodule frequentist_statistics.py includes the following functions: <br>
-- **normal_check():** compare the distribution of numeric variables to a normal distribution using the
-    Kolmogrov-Smirnov test <br>
-- **correlation_analysis():** Run correlations for numerical features and return output in different formats <br>
-- **correlations_as_sample_increases():** Run correlations for subparts of the data to check robustness <br>
-- **multiple_univariate_OLSs():** Tmp <br>
-- **potential_for_change_index():** Calculate the potential for change index based on either variants of the r-squared
-    (from linear regression) or the r-value (pearson correlation) <br>
-- **correct_pvalues():** function to correct for multiple testing <br>
-- **partial_correlation():** function to calculate the partial correlations whilst correcting for other variables <br>
+r"""Submodule frequentist_statistics.py includes the following functions:
+
+- **normal_check():** compare the distribution of numeric variables to a normal distribution using the Kolmogrov-Smirnov test.
+
+- **correlation_analysis():** Run correlations for numerical features and return output in different formats.
+
+- **correlations_as_sample_increases():** Run correlations for subparts of the data to check robustness.
+
+- **multiple_univariate_OLSs():** A function used to compute multiple univariate ordinary least squares regression (i.e. not a multivariate OLS).
+
+- **potential_for_change_index():** Calculate the potential for change index based on either variants of the r-squared (from linear regression) or the r-value (pearson correlation).
+
+- **correct_pvalues():** function to correct for multiple testing.
+
+- **partial_correlation():** function to calculate the partial correlations whilst correcting for other variables.
+
 """
 from itertools import combinations
 from itertools import product
+from typing import Any
 from typing import Tuple
 from typing import Union
 
 import matplotlib.pyplot as plt
 import numpy as np
 import pandas as pd
+import pingouin as pg
 import seaborn as sns
 import statsmodels.api as sm
 from matplotlib.lines import Line2D
 from scipy import stats
 from sklearn.linear_model import LinearRegression
 from statsmodels.stats.multitest import multipletests
 
 from .utils import apply_scaling
 
 
-def normal_check(data: pd.DataFrame) -> pd.DataFrame:
+def normal_check(data: pd.DataFrame):
     r"""Compare the distribution of numeric variables to a normal distribution using the Kolmogrov-Smirnov test
     Wrapper for `scipy.stats.kstest`: the empircal data is compared to a normally distributed variable with the
     same mean and standard deviation. A significant result (p < 0.05) in the goodness of fit test means that the
     data is not normally distributed.
+
     Parameters
     ----------
-    data: pandas.DataFrame
+    data: pd.DataFrame
         Dataframe including the columns of interest
+
     Returns
-    ----------
+    -------
     df_normality_check: pd.DataFrame
         Dataframe with column names, p-values and an indication of normality
+
     Examples
-    ----------
+    --------
     >>> tips = sns.load_dataset("tips")
     >>> df_normality_check = normal_check(tips)
+
     """
     # Select numeric columns only
     num_features = data.select_dtypes(include="number").columns.tolist()
     # Compare distribution of each feature to a normal distribution with given mean and std
     df_normality_check = data[num_features].apply(
         lambda x: stats.kstest(
             x.dropna(), stats.norm.cdf, args=(np.nanmean(x), np.nanstd(x)), N=len(x)
@@ -61,28 +73,31 @@
     df_normality_check["normality"] = df_normality_check["p-value"] >= 0.05
 
     return df_normality_check
 
 
 def permute_test(a, test_type, test, **kwargs):
     r"""Helper function to run tests for permutations
+
     Parameters
     ----------
     a : np.array
     test_type: str {'correlation', 'independent_t_test'}
         Type of the test to be used
     test:
         e.g. `scipy.stats.pearsonr` or `statsmodels.stats.weightstats.ttest_ind`
     **kwargs:
         Additional keywords to be added to `test`
         - `a2` for the second feature if test_type = 'correlation'
+
     Returns
-    ----------
+    -------
     float:
         p value for permutation
+
     """
     if test_type == "correlation":
         a2 = kwargs["a2"]
         _, p = test(a, a2)
 
     else:
         raise ValueError("Unknown test_type provided")
@@ -92,23 +107,22 @@
     data: pd.DataFrame,
     col_list=None,
     row_list=None,
     check_norm=False,
     method: str = "pearson",
     dropna: str = "pairwise",
     permutation_test: bool = False,
-    n_permutations: int = 1000,
-    random_state=None,
 ):
-    r"""Run correlations for numerical features and return output in different formats
+    """Run correlations for numerical features and return output in different formats
     Different methods to compute correlations and to handle missing values are implemented.
     Inspired by `researchpy.corr_case` and `researchpy.corr_pair`.
+
     Parameters
     ----------
-    data : pandas.DataFrame
+    data : pd.DataFrame
         Dataframe with variables in columns, cases in rows
     row_list: list or None (default: None)
         List with names of columns in `data` that should be in the rows of the correlogram.
         If None, all columns are used but only every unique combination.
     col_list: list or None (default: None)
         List with names of columns in `data` that should be in the columns of the correlogram.
         If None, all columns are used and only every unique combination.
@@ -129,46 +143,50 @@
         Number of permutations in the permutation test
     random_state: None or int (default: None)
         Random state for permutation_test. If not None, random_state will be updated for every permutation
     plot_permutation: bool (default: False)
         Whether to plot the results of the permutation test
     figsize: tuple (default: (11.7, 8.27))
         Width and height of the figure in inches
+
     Returns
-    ----------
+    -------
     result_dict: dict
         Dictionary containing with the following keys:
-        info : pandas.DataFrame
+        info: pd.DataFrame
             Description of correlation method, missing values handling and number of observations
-        r-values : pandas.DataFrame
+        r-values: pd.DataFrame
             Dataframe with correlation coefficients. Indices and columns are column names from `data`. Only lower
             triangle is filled.
-        p-values : pandas.DataFrame
+        p-values: pd.DataFrame
             Dataframe with p-values. Indices and columns are column names from `data`. Only lower triangle is filled.
-        N        : pandas.DataFrame
+        N: pd.DataFrame
             Dataframe with numbers of observations. Indices and columns are column names from `data`. Only lower
             triangle is filled. If dropna ='listwise', every correlation will have the same number of observations.
-        summary : pandas.DataFrame
+        summary: pd.DataFrame
             Dataframe with columns ['analysis', 'feature1', 'feature2', 'r-value', 'p-value', 'N', 'stat-sign']
             which indicate the type of test used for the correlation, the pair of columns, the correlation coefficient,
             the p-value, the number of observations for each combination of columns in `data` and whether the r-value is
             statistically significant.
     plotted_permuations: Figure
+
     Examples
-    ----------
+    --------
     >>> from jmspack.frequentist_statistics import correlation_analysis
     >>> import seaborn as sns
     >>> iris = sns.load_dataset('iris')
     >>> dict_results = correlation_analysis(iris, method='pearson', dropna='listwise', permutation_test=True,
-    >>>                                        n_permutations=100, check_norm=True)
+    ...                                        n_permutations=100, check_norm=True)
     >>> dict_results['summary']
+
     References
     ----------
     Bryant, C (2018). researchpy's documentation [Revision 9ae5ed63]. Retrieved from
     https://researchpy.readthedocs.io/en/latest/
+
     """
 
     # Settings test
     if method == "pearson":
         test, test_name = stats.pearsonr, "Pearson"
     elif method == "spearman":
         test, test_name = stats.spearmanr, "Spearman Rank"
@@ -194,31 +212,41 @@
         p_vals = pd.DataFrame(columns=data.columns, index=data.columns)
         n_vals = pd.DataFrame(columns=data.columns, index=data.columns)
         iterator = combinations(data.columns, 2)
     else:
         r_vals = pd.DataFrame(columns=col_list, index=row_list)
         p_vals = pd.DataFrame(columns=col_list, index=row_list)
         n_vals = pd.DataFrame(columns=col_list, index=row_list)
-        iterator = product(col_list, row_list)
+        iterator = product(col_list, row_list)  # type: ignore
 
     if dropna == "listwise":
         # Remove rows with missing values
         data = data.dropna(how="any", axis="index")
-        info = info.append(
-            {
-                f"{test_name} correlation test using {dropna} deletion": f"Total observations used = {len(data)}"
-            },
-            ignore_index=True,
+        info = pd.concat(
+            [
+                info,
+                pd.DataFrame(
+                    {
+                        f"{test_name} correlation test using {dropna} deletion": f"Total observations used = {len(data)}"
+                    },
+                    index=[0],
+                ),
+            ]
         )
     elif dropna == "pairwise":
-        info = info.append(
-            {
-                f"{test_name} correlation test using {dropna} deletion": f"Observations in the data = {len(data)}"
-            },
-            ignore_index=True,
+        info = pd.concat(
+            [
+                info,
+                pd.DataFrame(
+                    {
+                        f"{test_name} correlation test using {dropna} deletion": f"Observations in the data = {len(data)}"
+                    },
+                    index=[0],
+                ),
+            ]
         )
     else:
         raise ValueError("dropna not in {'listwise', 'pairwise'}")
 
     if check_norm:
         # Check normality of all columns in the data
         df_normality = normal_check(data)
@@ -263,40 +291,14 @@
             "stat-sign": (p_value < 0.05),
             "N": n_value,
         }
 
         if permutation_test:
             raise ValueError("permutation_test has yet to be implemented")
 
-            # # Copy the complete data
-            # col2_shuffle = np.array(test_data.loc[:, col2])
-            # col2_shuffle = np.repeat(
-            #     col2_shuffle[:, np.newaxis], n_permutations, axis=1
-            # )
-            # # Shuffle within the columns
-            # np.random.seed(random_state)
-            # ix_i = np.random.sample(col2_shuffle.shape).argsort(axis=0)
-            # ix_j = np.tile(np.arange(col2_shuffle.shape[1]), (col2_shuffle.shape[0], 1))
-            # col2_shuffle = col2_shuffle[ix_i, ix_j]
-            # permutations = np.apply_along_axis(
-            #     permute_test,
-            #     axis=0,
-            #     arr=col2_shuffle,
-            #     test_type="correlation",
-            #     test=test,
-            #     a2=np.array(test_data.loc[:, col1]),
-            # )
-            #
-            # extreme_permutation = np.where(permutations < p_value, 1, 0)
-            # p_permutation = extreme_permutation.sum() / len(permutations)
-            # dict_summary["permutation-p-value"] = p_permutation
-            #
-            # # Reset random seed numpy
-            # np.random.seed(None)
-
         summary = pd.concat(
             [summary, pd.DataFrame(data=dict_summary, index=[0])],
             axis=0,
             ignore_index=True,
             sort=False,
         )
 
@@ -325,17 +327,18 @@
     plot: bool = True,
     addition_to_title: str = "",
     figsize: Tuple[float, float] = (9.0, 4.0),
     alpha: float = 0.05,
 ):
     r"""Plot changes in r-value and p-value from correlation between two features when sample size increases.
     Different methods to compute correlations are implemented. Data is shuffled first, to prevent any order effects.
+
     Parameters
     ----------
-    data : pandas.DataFrame
+    data : pd.DataFrame
         Dataframe with variables in columns, cases in rows
     feature1: str
         Name of column with first feature to be included in correlation
     feature2: str
         Name of column with second feature to be included in correlation
     starting_N: int (default: 10)
         Number of cases that should be used for first correlation
@@ -354,28 +357,31 @@
     plot: bool (default: True)
         Whether to plot the results
     addition_to_title: str (default: '')
         The title of the plot will be "The absolute r-value between {feature1} and {feature2} as N increases" and
         followed by the addition (e.g. to describe a dataset).
     alpha: float (default: 0.05)
         Threshold for p-value that should be shown in the plot
+
     Returns
-    ----------
+    -------
     cor_results: pd.DataFrame
         Dataframe with the results for all ran analyses
     fig: Figure
         Figure will be returned if plot=True, otherwise None. This allows you to change properties of the figure
         afterwards, e.g. fig.axes[0].set_title('This is my new title')
+
     Examples
-    ----------
+    --------
     >>> import seaborn as sns
     >>> from jmspack.frequentist_statistics import correlations_as_sample_increases
     >>> iris = sns.load_dataset('iris')
     >>> summary,  fig = correlations_as_sample_increases(data=iris,feature1='petal_width',feature2='sepal_length',
-    >>> starting_N=20)
+    ... starting_N=20)
+
     """
 
     data = (
         data[[feature1, feature2]].copy()
         # Remove rows with np.nans
         .dropna()
         # Randomize order of the data
@@ -443,14 +449,40 @@
 
 
 def multiple_univariate_OLSs(
     X: pd.DataFrame,
     y: pd.Series,
     features_list: list,
 ):
+    """Calculate multiple univariate ordinary least squares regression (i.e. not a multivariate OLS).
+
+    Parameters
+    ----------
+    X: pd.DataFrame
+        Dataframe with features
+    y: pd.Series
+        Series with target
+    features_list: list
+        List with features to be used in each of the OLS regressions
+
+    Returns
+    -------
+    all_coefs_df: pd.DataFrame
+        Dataframe with coefficients, p-values, r-squared and r-squared adjusted for each of the OLS regressions
+
+    Examples
+    --------
+    >>> from jmspack.frequentist_statistics import multiple_univariate_OLSs
+    >>> import seaborn as sns
+    >>> iris = sns.load_dataset('iris')
+    >>> multiple_univariate_OLSs(X=iris[['sepal_length', 'sepal_width', 'petal_length']], y=iris['petal_width'],
+    ... features_list=['sepal_length', 'sepal_width', 'petal_length'])
+
+    """
+
     all_coefs_df = pd.DataFrame()
     for feature in features_list:
         mod = sm.OLS(endog=y, exog=sm.add_constant(X[[feature]]))
         res = mod.fit()
         coef_df = pd.read_html(
             res.summary().tables[1].as_html(), header=0, index_col=0
         )[0].drop("const")
@@ -469,16 +501,66 @@
     centrality_measure: str = "mean",
     maximum_measure: str = "max",
     weight_measure: str = "rsquared_adj",
     scale_data: bool = True,
     pci_heatmap: bool = True,
     pci_heatmap_figsize: Tuple[float, float] = (1.0, 4.0),
 ):
+    """Calculate the potential for change index based on either variants of the r-squared (from linear regression) or
+
+    Parameters
+    ----------
+    data: pd.DataFrame
+        Dataframe with features and target
+    features_list: list
+        List with features to be used in each of potential for change index calculations
+    target: str
+        Name of the target variable
+    minimum_measure: str (default: 'min')
+        Measure to be used for the minimum value of the feature
+    centrality_measure: str (default: 'mean')
+        Measure to be used for the centrality of the feature
+    maximum_measure: str (default: 'max')
+        Measure to be used for the maximum value of the feature
+    weight_measure: str (default: 'rsquared_adj')
+        Measure to be used for the weight of the feature
+    scale_data: bool (default: True)
+        Whether to scale the data before calculating the potential for change index
+    pci_heatmap: bool (default: True)
+        Whether to plot the heatmap of the potential for change index
+    pci_heatmap_figsize: tuple (default: (1.0, 4.0))
+        Width and height of the figure in inches
+
+    Returns
+    -------
+    pci_df: pd.DataFrame
+        Dataframe with the potential for change index for each feature
+
+    Examples
+    --------
+    >>> from jmspack.frequentist_statistics import potential_for_change_index
+    >>> import seaborn as sns
+    >>> iris = sns.load_dataset('iris')
+    >>> potential_for_change_index(
+    ...     data=iris,
+    ...     features_list=["sepal_length", "sepal_width", "petal_length"],
+    ...     target="petal_width",
+    ...     minimum_measure="min",
+    ...     centrality_measure="mean",
+    ...     maximum_measure="max",
+    ...     weight_measure="rsquared_adj",
+    ...     scale_data=True,
+    ...     pci_heatmap=True,
+    ...     pci_heatmap_figsize=(1.0, 4.0),
+    ... )
+
+    """
+
     if scale_data:
-        data = data.pipe(apply_scaling)
+        data = data[features_list + [target]].pipe(apply_scaling)
 
     if weight_measure == "rsquared_adj" or weight_measure == "rsquared":
         tmp_X = data[features_list]
         tmp_y = data[target]
         weight_df = multiple_univariate_OLSs(
             X=tmp_X, y=tmp_y, features_list=features_list
         )
@@ -489,23 +571,19 @@
         output_dict = correlation_analysis(
             data=data,
             col_list=features_list,
             row_list=[target],
             method="pearson",
             check_norm=False,
             dropna="pairwise",
-            permutation_test=False,
-            n_permutations=10,
-            random_state=69420,
         )
         weight_df = output_dict["summary"].set_index("feature1")
         negative_list = weight_df[weight_df["r-value"] < 0].index.tolist()
 
     if len(negative_list) < 0:
-
         pci_df = (
             # room for improvement calculation (series)
             (
                 data[features_list].agg(centrality_measure)
                 - (data[features_list].agg(maximum_measure))
             ).abs()
             * weight_df[weight_measure]  # weight (based on weight_measure series)
@@ -571,40 +649,64 @@
     alpha: float = 0.05,
     method: str = "fdr_bh",
     plot: bool = False,
     labels=None,
     title: str = "",
     figsize: tuple = (10, 5),
 ):
-    r"""
-    Correct an array-like with pvalues using `method`, wrapper for `statsmodels.stats.multitest.multipletests`
+    r"""Correct an array-like with pvalues using `method`, wrapper for `statsmodels.stats.multitest.multipletests`
+
     Parameters
     ----------
-    pvals: array-like, 1d
+    pvals: array-like
         uncorrected pvalues
     alpha: float
         FWER, family-wise error rate
-    method: str, one of {'bonferroni', 'sidak', 'holm-sidak', 'holm', 'simes-hochberg', 'hommel', 'fdr_bh',
-    'fdr_by', 'fdr_tsbh', 'fdr_tsbky'}
+    method: str
+        one of {'bonferroni', 'sidak', 'holm-sidak', 'holm', 'simes-hochberg', 'hommel', 'fdr_bh',
+        'fdr_by', 'fdr_tsbh', 'fdr_tsbky'}
     plot: bool
         whether to plot the results
     title: str
         title to show above the plot
-    labels: array-like, 1d
+    labels: array-like
         labels for the uncorrected pvalues
     figsize: tuple
         size for the Figure
+
     Returns
-    ----------
+    -------
     reject: numpy.array, bool
         true for hypothesis that can be rejected for given alpha
     corrected_p: numpy.array
         p-values corrected for multiple tests
     pvalues_plot: matplotlib.figure.Figure (optional)
         Figure if plot == True, else None
+
+    Examples
+    --------
+    >>> from jmspack.frequentist_statistics import correct_pvalues, correlation_analysis
+    >>> import seaborn as sns
+    >>> iris = sns.load_dataset('iris')
+    >>> output_dict = correlation_analysis(
+    ...     iris,
+    ...     method="pearson",
+    ...     dropna="listwise",
+    ...     permutation_test=False,
+    ...     n_permutations=100,
+    ...     check_norm=True,
+    ... )
+    >>> rejected_array, corrected_p_array, fig = correct_pvalues(
+    ...     pvals=output_dict["summary"]["p-value"],
+    ...     alpha=0.05,
+    ...     method="fdr_bh",
+    ...     plot=True,
+    ...     title="Corrected p-values",
+    ... )
+
     """
 
     if isinstance(pvals, pd.Series):
         pvals = pvals.values
 
     if labels is not None:
         if len(pvals) != len(labels):
@@ -708,54 +810,52 @@
 
         if labels is not None:
             _ = plt.xticks(plt.xticks()[0], labels)
 
     return reject, corrected_p, pvalues_plot
 
 
-def partial_correlation(df: pd.DataFrame):
-    """
-    Returns the sample linear partial correlation coefficients between pairs of variables,
+def partial_correlation(df: pd.DataFrame, feature_list: list):
+    """Returns the sample linear partial correlation coefficients between pairs of variables,
     controlling for all other remaining variables
+
     Parameters
     ----------
-    df : array-like, shape (n, p)
-        Array with the different variables. Each column is taken as a variable.
+    df: pd.DataFrame
+        Dataframe with features
+    feature_list: list
+        List with features to be used in each of partial correlation calculations
+
     Returns
     -------
-    P : array-like, shape (p, p)
-        P[i, j] contains the partial correlation of input_df[:, i] and input_df[:, j]
-        controlling for all other remaining variables.
+    partial_cor_df: pd.DataFrame
+        Dataframe with the partial correlation coefficients for each pair of features
+
+    Examples
+    --------
+    >>> from jmspack.frequentist_statistics import partial_correlation
+    >>> import seaborn as sns
+    >>> iris = sns.load_dataset('iris')
+    >>> summary_df = partial_correlation(df=iris, feature_list=['sepal_length', 'sepal_width', 'petal_length'])
+
     """
-    partial_corr_matrix_rvals = np.zeros((df.shape[1], df.shape[1]))
-    partial_corr_matrix_pvals = np.zeros((df.shape[1], df.shape[1]))
+    feature_tuple_list = list(combinations(feature_list, 2))
 
-    for i, column1 in enumerate(df):
-        for j, column2 in enumerate(df):
-            control_variables = np.delete(np.arange(df.shape[1]), [i, j])
-            if i == j:
-                partial_corr_matrix_rvals[i, j] = 1
-                partial_corr_matrix_pvals[i, j] = 1
-                continue
-            data_control_variable = df.iloc[:, control_variables]
-            data_column1 = df[column1].values
-            data_column2 = df[column2].values
-            fit1 = LinearRegression(fit_intercept=True)
-            fit2 = LinearRegression(fit_intercept=True)
-            fit1.fit(data_control_variable, data_column1)
-            fit2.fit(data_control_variable, data_column2)
-            residual1 = data_column1 - (
-                np.dot(data_control_variable, fit1.coef_) + fit1.intercept_
-            )
-            residual2 = data_column2 - (
-                np.dot(data_control_variable, fit2.coef_) + fit2.intercept_
-            )
-            partial_corr_matrix_rvals[i, j] = stats.pearsonr(residual1, residual2)[0]
-            partial_corr_matrix_pvals[i, j] = stats.pearsonr(residual1, residual2)[1]
-            partial_corr_matrix_rvals_df = pd.DataFrame(
-                partial_corr_matrix_rvals, columns=df.columns, index=df.columns
-            )
-            partial_corr_matrix_pvals_df = pd.DataFrame(
-                partial_corr_matrix_pvals, columns=df.columns, index=df.columns
-            )
+    partial_cor_df = pd.DataFrame()
+    for feature_tuple in feature_tuple_list:
+        covariate_list = list(set(feature_list) - set(feature_tuple))
+        partial_cor_df = pd.concat(
+            [
+                partial_cor_df,
+                pg.partial_corr(
+                    data=df,
+                    x=feature_tuple[0],
+                    y=feature_tuple[1],
+                    covar=covariate_list,
+                    method="pearson",
+                ).assign(
+                    **{"feature1": feature_tuple[0], "feature2": feature_tuple[1]}
+                ),
+            ]
+        )
 
-    return partial_corr_matrix_rvals_df, partial_corr_matrix_pvals_df
+    return partial_cor_df.rename(columns={"r": "r-value", "p-val": "p-value"}).round(3)
```

### Comparing `jmspack-0.1.1/jmspack/internal_utils.py` & `jmspack-0.1.2/jmspack/internal_utils.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,19 @@
-r"""Submodule internal_utils.py includes the following functions: <br>
-- **postgresql_data_extraction():** importing data from a table of a postgresql database. <br>
-- **postgresql_table_names_list():** extract the table names from a specified postgresql database. <br>
-- **create_postgresql_table_based_on_df():** create a new table in a specified postgresql database based on the columns of a pandas data frame. <br>
-- **add_data_to_postgresql_table():** add new data to an existing table in a specified postgresql database. <br>
-- **delete_postgresql_table():** delete a table from a postgresql database. <br>
+r"""Submodule internal_utils.py includes the following functions:
+
+- **postgresql_data_extraction():** importing data from a table of a postgresql database.
+
+- **postgresql_table_names_list():** extract the table names from a specified postgresql database.
+
+- **create_postgresql_table_based_on_df():** create a new table in a specified postgresql database based on the columns of a pandas data frame.
+
+- **add_data_to_postgresql_table():** add new data to an existing table in a specified postgresql database.
+
+- **delete_postgresql_table():** delete a table from a postgresql database.
+
 """
 import os
 
 import pandas as pd
 import psycopg2
 
 # INFO: for all of postgresql based functions, you will need to specify your
@@ -17,41 +23,43 @@
 
 
 def postgresql_data_extraction(
     table_name: str = "suggested_energy_intake",
     database_name: str = "tracker",
     user: str = "tracker",
 ):
-    r"""
-    Load data from a specified postgresql database.
+    """Load data from a specified postgresql database.
 
     Parameters
     ----------
     table_name: str
         The name of the table to extract from the postgresql database.
     database_name: str
         The name of the postgresql database.
     user: str
         The name of the user.
 
     Returns
     -------
-    pd.DataFrame
+    df: pd.DataFrame
+        pandas dataframe object containing the data from the specified table.
 
     Examples
-    ---------
+    --------
     >>> from dotenv import load_dotenv, find_dotenv
     >>> from jmspack.internal_utils import postgresql_data_extraction
     >>> # Make sure you have a .env file somewhere with your postgresql credentials
     >>> # labelled as postgresql_host="BLA", and postgresql_password="BLA2"
     >>> load_dotenv(find_dotenv())
     >>> df = postgresql_data_extraction(table_name = 'iris_test',
-                                database_name = 'tracker',
-                                user='tracker')
+    ...                            database_name = 'tracker',
+    ...                            user='tracker')
+
     """
+
     df = pd.DataFrame()
     try:
         conn = psycopg2.connect(
             host=os.getenv("postgresql_host"),
             database=database_name,
             user=user,
             password=os.getenv("postgresql_password"),
@@ -65,37 +73,38 @@
     return df
 
 
 def postgresql_table_names_list(
     database_name: str = "tracker",
     user="tracker",
 ):
-    r"""
-    Extract the table names from a specified postgresql database.
+    """Extract the table names from a specified postgresql database.
 
     Parameters
     ----------
     database_name: str
         The name of the postgresql database.
     user: str
         The name of the user.
 
     Returns
     -------
     list
 
     Examples
-    ---------
+    --------
     >>> from dotenv import load_dotenv, find_dotenv
     >>> from jmspack.internal_utils import postgresql_table_names_list
     >>> # Make sure you have a .env file somewhere with your postgresql credentials
     >>> # labelled as postgresql_host="BLA", and postgresql_password="BLA2"
     >>> load_dotenv(find_dotenv())
     >>> table_names = postgresql_table_names_list()
+
     """
+
     table_list = False
     try:
         conn = psycopg2.connect(
             host=os.getenv("postgresql_host"),
             database=database_name,
             user=user,
             password=os.getenv("postgresql_password"),
@@ -115,16 +124,15 @@
 def create_postgresql_table_based_on_df(
     df: pd.DataFrame,
     database_name: str,
     user: str,
     table_name: str,
 ):
 
-    r"""
-    Create a new table in a specified postgresql database based on the columns of a pandas data frame.
+    """Create a new table in a specified postgresql database based on the columns of a pandas data frame.
 
     Parameters
     ----------
     df: pd.DataFrame
         The pandas dataframe object you wish to use the columns and data types
         to create the table from in postgresql
     database_name: str
@@ -135,27 +143,28 @@
         A string specifying the name of the newly created table.
 
     Returns
     -------
     str
 
     Examples
-    ---------
+    --------
     >>> import seaborn as sns
     >>> from dotenv import load_dotenv, find_dotenv
     >>> from jmspack.internal_utils import add_data_to_postgresql_table
     >>> # Make sure you have a .env file somewhere with your postgresql credentials
     >>> # labelled as postgresql_host="BLA", and postgresql_password="BLA2"
     >>> load_dotenv(find_dotenv())
     >>> iris_df = sns.load_dataset("iris")
     >>> _ = create_postgresql_table_based_on_df(df=iris_df,
     ...                                         database_name="tracker",
     ...                                         user="tracker",
     ...                                         table_name="iris_test",
     ...                                         )
+
     """
 
     python_to_sql_dtypes_dict = {
         "object": "text",
         "float64": "float",
         "float32": "float",
         "int8": "int",
@@ -193,16 +202,15 @@
 def add_data_to_postgresql_table(
     df: pd.DataFrame,
     database_name: str,
     user: str,
     table_name: str,
 ):
 
-    r"""
-    Add new data to an existing table in a specified postgresql database.
+    """Add new data to an existing table in a specified postgresql database.
 
     Parameters
     ----------
     df: pd.DataFrame
         The pandas dataframe object you wish to use the columns and data types
         to create the table from in postgresql
     database_name: str
@@ -213,15 +221,15 @@
         A string specifying the name of the newly created table.
 
     Returns
     -------
     str
 
     Examples
-    ---------
+    --------
     >>> import seaborn as sns
     >>> from dotenv import load_dotenv, find_dotenv
     >>> from jmspack.internal_utils import add_data_to_postgresql_table
     >>> # Make sure you have a .env file somewhere with your postgresql credentials
     >>> # labelled as postgresql_host="BLA", and postgresql_password="BLA2"
     >>> load_dotenv(find_dotenv())
     >>> iris_df = sns.load_dataset("iris")
@@ -231,14 +239,15 @@
     ...                                         table_name="iris_test",
     ...                                         )
     >>> _ = add_data_to_postgresql_table(df=iris_df,
     ...                                 database_name="tracker",
     ...                                 user="tracker",
     ...                                 table_name="iris_test",
     ...                                 )
+
     """
 
     columns_string = ", ".join(df.columns.tolist())
     value_placeholder_string = ", ".join(["%s" for x in range(0, df.shape[1])])
     insert_string = f"""INSERT INTO {table_name} ({columns_string}) VALUES ({value_placeholder_string})"""
     try:
         conn = psycopg2.connect(
@@ -266,16 +275,15 @@
 
 def delete_postgresql_table(
     database_name: str,
     user: str,
     table_name: str,
 ):
 
-    r"""
-    Delete a table from a postgresql database.
+    """Delete a table from a postgresql database.
 
     Parameters
     ----------
     database_name: str
         The name of the postgresql database.
     user: str
         The name of the user.
@@ -283,15 +291,15 @@
         A string specifying the name of the newly created table.
 
     Returns
     -------
     str
 
     Examples
-    ---------
+    --------
     >>> import seaborn as sns
     >>> from dotenv import load_dotenv, find_dotenv
     >>> from jmspack.internal_utils import add_data_to_postgresql_table
     >>> # Make sure you have a .env file somewhere with your postgresql credentials
     >>> # labelled as postgresql_host="BLA", and postgresql_password="BLA2"
     >>> load_dotenv(find_dotenv())
     >>> iris_df = sns.load_dataset("iris")
@@ -305,14 +313,15 @@
     ...                                 user="tracker",
     ...                                 table_name="iris_test",
     ...                                 )
     >>> _ = delete_postgresql_table(database_name="tracker",
     ...                             user="tracker",
     ...                             table_name="iris_test"
     ...                             )
+
     """
 
     try:
         conn = psycopg2.connect(
             host=os.getenv("postgresql_host"),
             database=database_name,
             user=user,
```

### Comparing `jmspack-0.1.1/jmspack/ml_utils.py` & `jmspack-0.1.2/jmspack/ml_utils.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,17 +1,26 @@
 r"""Submodule ml_utils.py includes the following functions:
 
-  - plot_decision_boundary(): Generate a simple plot of the decision boundary of a classifier. <br>
-  - plot_cv_indices(): tmp <br>
-  - plot_learning_curve(): tmp <br>
-  - dict_of_models: tmp <br>
-  - multi_roc_auc_plot(): tmp <br>
-  - RFE_opt_rf(): tmp <br>
-  - make_confusion_matrix(): tmp <br>
-  - summary_performance_metrics_classification(): tmp <br>
+- plot_decision_boundary(): Generate a simple plot of the decision boundary of a classifier.
+
+- plot_cv_indices(): Visualise the inputted cross validation method in chunks.
+
+- plot_learning_curve(): Plot the learning curve of an estimator as samples increase to evaluate overfitting.
+
+- dict_of_models: A dictionary of useful models.
+
+- multi_roc_auc_plot(): A utility to plot the ROC curves of multiple classifiers (suggested to use in conjunction with the dict_of_models).
+
+- optimize_model(): A utility to run gridsearch and Recursive Feature Elimination on a classifier to return a model with the best parameters.
+
+- plot_confusion_matrix(): Visualise a confusion matrix.
+
+- summary_performance_metrics_classification(): A utility to return a selection of regularly used classification performance metrics.
+
+- RMSE(): Root Mean Squared Error.
 
 """
 import warnings
 from typing import Union
 
 import matplotlib.pyplot as plt
 import numpy as np
@@ -27,14 +36,15 @@
 from sklearn.ensemble import AdaBoostClassifier
 from sklearn.ensemble import GradientBoostingClassifier
 from sklearn.ensemble import RandomForestClassifier
 from sklearn.feature_selection import RFE
 from sklearn.gaussian_process import GaussianProcessClassifier
 from sklearn.gaussian_process.kernels import RBF
 from sklearn.linear_model import LogisticRegression
+from sklearn.metrics import mean_squared_error
 from sklearn.model_selection import GridSearchCV
 from sklearn.model_selection import learning_curve
 from sklearn.model_selection import train_test_split
 from sklearn.naive_bayes import GaussianNB
 from sklearn.neighbors import KNeighborsClassifier
 from sklearn.neural_network import MLPClassifier
 from sklearn.preprocessing import StandardScaler
@@ -49,16 +59,16 @@
     y: pd.Series,
     clf: ClassifierMixin = sklearn.linear_model.LogisticRegression(),
     title: str = "Decision Boundary Logistic Regression",
     legend_title: str = "Legend",
     h: float = 0.05,
     figsize: tuple = (11.7, 8.27),
 ):
-    r"""
-    Generate a simple plot of the decision boundary of a classifier.
+    """Generate a simple plot of the decision boundary of a classifier.
+
     Parameters
     ----------
     X : array-like, shape (n_samples, n_features)
         Classifier vector, where n_samples is the number of samples and
         n_features is the number of features.
     y : array-like, shape (n_samples)
         Target relative to X for classification. Datatype should be integers.
@@ -68,31 +78,33 @@
         Step size in the mesh
     title : string
         Title for the plot.
     legend_title : string
         Legend title for the plot.
     figsize: tuple (default: (11.7, 8.27))
         Width and height of the figure in inches
+
     Returns
-    ----------
+    -------
     boundaries: Figure
         Properties of the figure can be changed later, e.g. use `boundaries.axes[0].set_ylim(0,100)` to change ylim
     ax: Axes
         The axes associated with the boundaries Figure.
+
     Examples
-    ----------
+    --------
     >>> import seaborn as sns
     >>> from sklearn.svm import SVC
     >>> data = sns.load_dataset("iris")
     >>> # convert the target from string to category to numeric as sklearn cannot handle strings as target
     >>> y = data["species"]
     >>> X = data[["sepal_length", "sepal_width"]]
     >>> clf = SVC(kernel="rbf", gamma=2, C=1, probability=True)
     >>> _ = plot_decision_boundary(X=X, y=y, clf=clf, title = 'Decision Boundary', legend_title = "Species")
-    >>> # plt.show()
+
     """
 
     if X.shape[1] != 2:
         raise ValueError("X must contains only two features.")
 
     if not (
         pd.api.types.is_integer_dtype(y)
@@ -138,15 +150,15 @@
     Z_max = Z_proba.max(axis=1)  # Take the class with highest probability
     Z_max = Z_max.reshape(xx.shape)
 
     # Put the result into a color plot
     boundaries, ax = plt.subplots(figsize=figsize)
     _ = ax.contour(xx, yy, Z, cmap=cmap_bold)
     _ = ax.scatter(
-        xx, yy, s=(Z_max ** 2 / h), c=Z, cmap=cmap_bold, alpha=1, edgecolors="none"
+        xx, yy, s=(Z_max**2 / h), c=Z, cmap=cmap_bold, alpha=1, edgecolors="none"
     )
 
     # Plot also the training points
     training = ax.scatter(X[:, 0], X[:, 1], c=y, cmap=cmap_bold, edgecolors="black")
     _ = plt.xlim(xx.min(), xx.max())
     _ = plt.ylim(yy.min(), yy.max())
     _ = plt.title(title)
@@ -163,18 +175,18 @@
         bbox_to_anchor=(1, 0.5),
         handlelength=2,
         handletextpad=1,
         title=legend_title,
     )
 
     # Add legend sizes
-    l1 = plt.scatter([], [], c="black", s=0.4 ** 2 / h, edgecolors="none")
-    l2 = plt.scatter([], [], c="black", s=0.6 ** 2 / h, edgecolors="none")
-    l3 = plt.scatter([], [], c="black", s=0.8 ** 2 / h, edgecolors="none")
-    l4 = plt.scatter([], [], c="black", s=1 ** 2 / h, edgecolors="none")
+    l1 = plt.scatter([], [], c="black", s=0.4**2 / h, edgecolors="none")
+    l2 = plt.scatter([], [], c="black", s=0.6**2 / h, edgecolors="none")
+    l3 = plt.scatter([], [], c="black", s=0.8**2 / h, edgecolors="none")
+    l4 = plt.scatter([], [], c="black", s=1**2 / h, edgecolors="none")
 
     labels = ["0.4", "0.6", "0.8", "1"]
     _ = plt.legend(
         [l1, l2, l3, l4],
         labels,
         frameon=False,
         fontsize=12,
@@ -187,15 +199,55 @@
     )
     _ = plt.gca().add_artist(leg1)
 
     return boundaries, ax
 
 
 def plot_cv_indices(cv, X, y, group, n_splits, lw=10, figsize=(6, 3)):
-    """Create a sample plot for indices of a cross-validation object."""
+    """Create an example plot for indices of a cross-validation object.
+
+    Parameters
+    ----------
+    cv : cross-validation generator
+        A scikit-learn cross-validation object with a split method.
+    X : array-like
+        Training vector, where n_samples is the number of samples and
+        n_features is the number of features.
+    y : array-like
+        Target relative to X for classification or regression.
+    group : array-like
+        Group relative to X for classification or regression.
+    n_splits : int
+        Number of splits in the cross-validation object.
+    lw : int
+        Line width for the plots.
+    figsize : tuple
+        Width and height of the figure in inches
+
+    Returns
+    -------
+    fig: matplotlib.figure.Figure
+        Properties of the figure can be changed later, e.g. use `fig.axes[0].set_ylim(0,100)` to change ylim
+    ax: matplotlib.axes._subplots.AxesSubplot
+        The axes associated with the fig Figure.
+
+    Examples
+    --------
+    >>> import numpy as np
+    >>> from sklearn.model_selection import GroupKFold
+    >>> import matplotlib.pyplot as plt
+    >>> from jmspack.ml_utils import plot_cv_indices
+    >>> X = np.array([[1, 2], [3, 4], [5, 6], [7, 8]])
+    >>> y = np.array([1, 2, 1, 2])
+    >>> groups = np.array([0, 0, 2, 2])
+    >>> group_kfold = GroupKFold(n_splits=2)
+    >>> _ = plot_cv_indices(cv=group_kfold, X=X, y=y, group=groups, n_splits=2, lw=10, figsize=(6, 3))
+    >>> _ = plt.show()
+
+    """
 
     # set plotting options
     cmap_data = plt.cm.Paired
     cmap_cv = plt.cm.coolwarm
 
     fig, ax = plt.subplots(figsize=figsize)
 
@@ -262,35 +314,32 @@
     scoring: str = "accuracy",
     ylim: Union[None, tuple] = None,
     cv: Union[None, int] = None,
     n_jobs: int = -1,
     train_sizes: np.array = np.linspace(0.1, 1.0, 40),
     figsize: tuple = (10, 5),
 ):
-    """
-    Generate a simple plot of the test and training learning curve.
+    """Generate a simple plot of the test and training learning curve.
+
     Parameters
     ----------
     estimator : object type that implements the "fit" and "predict" methods
         An object of that type which is cloned for each validation.
     title : string
         Title for the chart.
     X : array-like, shape (n_samples, n_features)
         Training vector, where n_samples is the number of samples and
         n_features is the number of features.
     y : array-like, shape (n_samples) or (n_samples, n_features), optional
         Target relative to X for classification or regression;
         None for unsupervised learning.
-
     cross_color : string
         Signifies the color of the cross validation in the plot
-
     test_color : string
         Signifies the color of the test set in the plot
-
     scoring : string
         Signifies a scoring to evaluate the cross validation
     ylim : tuple, shape (ymin, ymax), optional
         Defines minimum and maximum yvalues plotted.
     cv : int, cross-validation generator or an iterable, optional
         Determines the cross-validation splitting strategy.
         Possible inputs for cv are:
@@ -314,21 +363,23 @@
         generate the learning curve. If the dtype is float, it is regarded as a
         fraction of the maximum size of the training set (that is determined
         by the selected validation method), i.e. it has to be within (0, 1].
         Otherwise it is interpreted as absolute sizes of the training sets.
         Note that for classification the number of samples usually have to
         be big enough to contain at least one sample from each class.
         (default: np.linspace(0.1, 1.0, 5))
+
     """
+
     fig, ax = plt.subplots(figsize=figsize)
-    plt.title(title)
+    _ = plt.title(title)
     if ylim is not None:
         plt.ylim(*ylim)
-    plt.xlabel("Training examples")
-    plt.ylabel(scoring)
+    _ = plt.xlabel("Training examples")
+    _ = plt.ylabel(scoring)
     train_sizes, train_scores, test_scores = learning_curve(
         estimator,
         X,
         y,
         groups=groups,
         cv=cv,
         scoring=scoring,
@@ -427,14 +478,50 @@
 def multi_roc_auc_plot(
     X: pd.DataFrame,
     y: pd.Series,
     models: list = dict_of_models,
     figsize: tuple = (7, 7),
 ):
 
+    """Plot the ROC curves of multiple classifiers.
+
+    Parameters
+    ----------
+    X : array-like, shape (n_samples, n_features)
+        Classifier vector, where n_samples is the number of samples and
+        n_features is the number of features.
+    y : array-like, shape (n_samples)
+        Target relative to X for classification. Datatype should be integers.
+    models : list
+        A list of dictionaries containing the model and the label to be used in the plot.
+    figsize: tuple (default: (7, 7))
+        Width and height of the figure in inches
+
+    Returns
+    -------
+    fig: matplotlib.figure.Figure
+        Properties of the figure can be changed later, e.g. use `fig.axes[0].set_ylim(0,100)` to change ylim
+    ax: matplotlib.axes._subplots.AxesSubplot
+        The axes associated with the fig Figure.
+
+    Examples
+    --------
+    >>> import seaborn as sns
+    >>> from jmspack.ml_utils import multi_roc_auc_plot, dict_of_models
+    >>> data = (
+    ...     sns.load_dataset("iris")
+    ...     .loc[lambda df: df["species"].isin(["setosa", "virginica"])]
+    ...     .replace({"virginica": 0, "setosa": 1})
+    ... )
+    >>> y = data["species"]
+    >>> X = data[["sepal_length", "sepal_width"]]
+    >>> _ = multi_roc_auc_plot(X=X, y=y, models=dict_of_models, figsize=(7, 7))
+
+    """
+
     # scale the data and create training and test sets of the data
     X = StandardScaler().fit_transform(X)
     X_train, X_test, y_train, y_test = train_test_split(
         X, y, test_size=0.3, random_state=42
     )
     fig, ax = plt.subplots(figsize=figsize)
     # Below for loop iterates through your models list
@@ -467,24 +554,81 @@
 def optimize_model(
     X: pd.DataFrame,
     y: pd.Series,
     estimator: BaseEstimator = sklearn.ensemble.RandomForestClassifier(),
     grid_params_dict: dict = {
         "max_depth": [1, 2, 3, 4, 5, 10],
         "n_estimators": [10, 20, 30, 40, 50],
-        "max_features": ["log2", "auto", "sqrt"],
+        "max_features": ["log2", "sqrt"],
         "criterion": ["gini", "entropy"],
     },
     gridsearch_kwargs: dict = {"scoring": "roc_auc", "cv": 3, "n_jobs": -2},
     rfe_kwargs: dict = {"n_features_to_select": 2, "verbose": 1},
 ):
 
+    """A utility to run gridsearch and Recursive Feature Elimination on a classifier to return a model with the best parameters.
+
+    Parameters
+    ----------
+    X : array-like, shape (n_samples, n_features)
+        Classifier vector, where n_samples is the number of samples and
+        n_features is the number of features.
+    y : array-like, shape (n_samples)
+        Target relative to X for classification. Datatype should be integers.
+    estimator : object type that implements the "fit" and "predict" methods
+        An object of that type which is cloned for each validation.
+    grid_params_dict : dict
+        A dictionary of parameters to be used in the gridsearch.
+    gridsearch_kwargs : dict
+        A dictionary of parameters to be used in the gridsearch.
+    rfe_kwargs : dict
+        A dictionary of parameters to be used in the Recursive Feature Elimination.
+
+    Returns
+    -------
+    optimized_estimator: sklearn estimator
+        The optimized estimator.
+    feature_ranking: pandas DataFrame
+        A dataframe with features ranking (high = dropped early on).
+    feature_selected: list
+        A list of features selected.
+    feature_importance: pandas DataFrame
+        A dataframe with importances per feature.
+    optimal_parameters: pandas DataFrame
+        A dataframe with the optimal parameters.
+
+    Examples
+    --------
+    >>> import seaborn as sns
+    >>> from sklearn.ensemble import RandomForestClassifier
+    >>> from jmspack.ml_utils import optimize_model
+    >>> data = (
+    ...     sns.load_dataset("iris")
+    ...     .loc[lambda df: df["species"].isin(["setosa", "virginica"])]
+    ...     .replace({"virginica": 0, "setosa": 1})
+    ... )
+    >>> y = data["species"]
+    >>> X = data[["sepal_length", "sepal_width"]]
+    >>> model = RandomForestClassifier()
+    >>> (
+    ...    optimized_estimator,
+    ...    feature_ranking,
+    ...    feature_selected,
+    ...    feature_importance,
+    ...    optimal_parameters,
+    ... ) = optimize_model(X=X, y=y, estimator=model)
+
+    """
     # Perform a 75% training and 25% test data split
     X_train, X_test, y_train, y_test = train_test_split(
-        X, y, test_size=0.3, stratify=y, random_state=42
+        X,
+        y,
+        test_size=0.3,
+        # stratify=y,
+        random_state=42,
     )
 
     # Instantiate grid_dt
     grid_dt = GridSearchCV(
         estimator=estimator, param_grid=grid_params_dict, **gridsearch_kwargs
     )
 
@@ -511,28 +655,28 @@
 
     # create dataframe with importances per feature
     feature_importance = pd.Series(
         dict(zip(X.columns, optimized_estimator.feature_importances_.round(2)))
     )
 
     # Calculates the test set accuracy
-    acc = metrics.accuracy_score(y_test, rfe.predict(X_test))
+    # acc = metrics.accuracy_score(y_test, rfe.predict(X_test))
 
     print("\n- Sizes :")
     print(f"- X shape = {X.shape}")
     print(f"- y shape = {y.shape}")
     print(f"- X_train shape = {X_train.shape}")
     print(f"- X_test shape = {X_test.shape}")
     print(f"- y_train shape = {y_train.shape}")
     print(f"- y_test shape = {y_test.shape}")
 
     print("\n- Model info :")
     print(f"- Optimal Parameters = {optimized_estimator.get_params()}")
     print(f"- Selected feature list = {feature_selected}")
-    print("- Accuracy score on test set = {0:.1%}".format(acc))
+    # print("- Accuracy score on test set = {0:.1%}".format(acc))
 
     return (
         optimized_estimator,
         feature_ranking,
         feature_selected,
         feature_importance,
         pd.DataFrame(optimized_estimator.get_params(), index=["optimal_parameters"]),
@@ -549,33 +693,61 @@
     xyticks=True,
     xyplotlabels=True,
     sum_stats=True,
     figsize: tuple = (7, 5),
     cmap="Blues",
     title=None,
 ):
-    """
-    This function will make a pretty plot of an sklearn Confusion Matrix cm using a Seaborn heatmap visualization.
-    Arguments
-    ---------
-    cf:            confusion matrix to be passed in
-    group_names:   List of strings that represent the labels row by row to be shown in each square.
-    categories:    List of strings containing the categories to be displayed on the x,y axis. Default is 'auto'
-    count:         If True, show the raw number in the confusion matrix. Default is True.
-    normalize:     If True, show the proportions for each category. Default is True.
-    cbar:          If True, show the color bar. The cbar values are based off the values in the confusion matrix.
-                   Default is True.
-    xyticks:       If True, show x and y ticks. Default is True.
-    xyplotlabels:  If True, show 'True Label' and 'Predicted Label' on the figure. Default is True.
-    sum_stats:     If True, display summary statistics below the figure. Default is True.
-    figsize:       Tuple representing the figure size. Default will be the matplotlib rcParams value.
-    cmap:          Colormap of the values displayed from matplotlib.pyplot.cm. Default is 'Blues'
-                   See http://matplotlib.org/examples/color/colormaps_reference.html
+    """This function will make a pretty plot of an sklearn Confusion Matrix cm using a Seaborn heatmap visualization.
+
+    Parameters
+    ----------
+    cf:
+        confusion matrix to be passed in
+    group_names:
+        List of strings that represent the labels row by row to be shown in each square.
+    categories:
+        List of strings containing the categories to be displayed on the x,y axis. Default is 'auto'
+    count:
+        If True, show the raw number in the confusion matrix. Default is True.
+    normalize:
+        If True, show the proportions for each category. Default is True.
+    cbar:
+        If True, show the color bar. The cbar values are based off the values in the confusion matrix. Default is True.
+    xyticks:
+        If True, show x and y ticks. Default is True.
+    xyplotlabels:
+        If True, show 'True Label' and 'Predicted Label' on the figure. Default is True.
+    sum_stats:
+        If True, display summary statistics below the figure. Default is True.
+    figsize:
+        Tuple representing the figure size. Default will be the matplotlib rcParams value.
+    cmap:
+        Colormap of the values displayed from matplotlib.pyplot.cm. Default is 'Blues'
+        See http://matplotlib.org/examples/color/colormaps_reference.html
+    title:
+        Title for the heatmap. Default is None.
+
+    Returns
+    -------
+    fig: matplotlib.figure.Figure
+        Properties of the figure can be changed later, e.g. use `fig.axes[0].set_ylim(0,100)` to change ylim
+    ax: matplotlib.axes._subplots.AxesSubplot
+        The axes associated with the fig Figure.
+
+    Examples
+    --------
+    >>> import seaborn as sns
+    >>> from sklearn.metrics import confusion_matrix
+    >>> from jmspack.ml_utils import plot_confusion_matrix
+    >>> y_true = ["cat", "dog", "cat", "cat", "dog", "bird"]
+    >>> y_pred = ["cat", "cat", "cat", "dog", "bird", "bird"]
+    >>> cf = confusion_matrix(y_true, y_pred, labels=["cat", "dog", "bird"])
+    >>> _ = plot_confusion_matrix(cf, figsize=(7, 5))
 
-    title:         Title for the heatmap. Default is None.
     """
 
     fig, ax = plt.subplots(figsize=figsize)
 
     # CODE TO GENERATE TEXT INSIDE EACH SQUARE
     blanks = ["" for i in range(cf.size)]
 
@@ -649,31 +821,34 @@
 
 
 def _bootstrap_auc(
     model, X_test, y_true, use_probabilities, bootstraps, fold_size, random_state
 ):
     """Internal function to bootstrap auc.
     Originates from the AI in healthcare specialization of coursera. https://www.coursera.org/specializations/ai-healthcare
+
     Parameters
     ----------
     model:
         The fitted sklearn model.
     X_test: pd.Series
         The predictors used to match to y_true.
     y_true: pd.Series
         The actual binary targets.
     classes: list(str)
         List with the name of the classes in string format.
     bootstraps: int
         The number of bootstraps.
     fold_size: int
         The number of folds.
+
     Returns
     -------
     list
+
     """
 
     if use_probabilities:
         y_pred_proba = model.predict_proba(X_test)[:, 1]
         df = pd.DataFrame({"y": y_true, "pred": y_pred_proba})
     else:
         y_pred = model.predict(X_test)
@@ -715,59 +890,64 @@
     return [f"{mean:.3f} (95% CI {min_:.3f}-{max_:.3f})"]
 
 
 def summary_performance_metrics_classification(
     model, X_test, y_true, bootstraps=100, fold_size=1000, random_state=69420
 ):
     """Summary of different evaluation metrics specific to a single class classification learning problem.
-    Notes
-    -----
-    The function returns the following metrics:
-    - true positive (TP): The model classifies the example as positive, and the actual label also positive.
-    - false positive (FP): The model classifies the example as positive, but the actual label is negative.
-    - true negative (TN): The model classifies the example as negative, and the actual label is also negative.
-    - false negative (FN): The model classifies the example as negative, but the label is actually positive.
-    - accuracy: The fractions of predictions the model got right.
-    - prevalance: The proportion of positive examples. Where y=1.
-    - sensitivity: The probability that our test outputs positive given that the case is actually positive.
-    - specificity: The probability that the test outputs negative given that the case is actually negative.
-    - positive predictive value: The proportion of positive predictions that are true positives.
-    - negative predictive value: The proportion of negative predictions that are true negatives.
-    - auc: A measure of goodness of fit.
-    - bootstrapped auc: The bootstrap estimates the uncertainty by resampling the dataset with replacement.
-    - F1: The harmonic mean of the precision and recall, where an F1 score reaches its best value at 1 (perfect precision and recall) and worst at 0.
-    Examples
-    --------
-    >>> from sklearn import datasets
-    >>> from sklearn.model_selection import train_test_split
-    >>> from sklearn.neighbors import KNeighborsClassifier
-    >>> import pandas as pd
-    >>> data = datasets.load_breast_cancer()
-    >>> df = pd.DataFrame(data.data, columns=data.feature_names)
-    >>> df['target'] = data.target
-    >>> X = data.data
-    >>> y = data.target
-    >>> X_train, X_test, y_train, y_test = train_test_split(X, y)
-    >>> clf = KNeighborsClassifier(n_neighbors=6)
-    >>> clf.fit(X_train, y_train)
-    >>> y_pred = clf.predict(X_test)
-    >>> summary_performance_metrics_classification(y_true=y_test, y_pred=y_pred)
+
     Parameters
     ----------
     model: sklearn.model
         A fitted sklearn model with predict() and predict_proba() methods.
     X_test: pd.DataFrame
         A data frame used to run predict the target values (y_pred).
     y_true: pd.Series or np.arrays
         Binary true values.
     bootstraps: int
     fold_size: int
+
     Returns
     -------
-    pd.DataFrame
+    summary_df: pd.DataFrame
+        A dataframe with the summary of the metrics.
+
+    Notes
+    -----
+    The function returns the following metrics:
+        - true positive (TP): The model classifies the example as positive, and the actual label also positive.
+        - false positive (FP): The model classifies the example as positive, but the actual label is negative.
+        - true negative (TN): The model classifies the example as negative, and the actual label is also negative.
+        - false negative (FN): The model classifies the example as negative, but the label is actually positive.
+        - accuracy: The fractions of predictions the model got right.
+        - prevalance: The proportion of positive examples. Where y=1.
+        - sensitivity: The probability that our test outputs positive given that the case is actually positive.
+        - specificity: The probability that the test outputs negative given that the case is actually negative.
+        - positive predictive value: The proportion of positive predictions that are true positives.
+        - negative predictive value: The proportion of negative predictions that are true negatives.
+        - auc: A measure of goodness of fit.
+        - bootstrapped auc: The bootstrap estimates the uncertainty by resampling the dataset with replacement.
+        - F1: The harmonic mean of the precision and recall, where an F1 score reaches its best value at 1 (perfect precision and recall) and worst at 0.
+
+    Examples
+    --------
+    >>> import seaborn as sns
+    >>> from sklearn.ensemble import RandomForestClassifier
+    >>> from jmspack.ml_utils import summary_performance_metrics_classification
+    >>> data = (
+    ...     sns.load_dataset("iris")
+    ...    .loc[lambda df: df["species"].isin(["setosa", "virginica"])]
+    ...    .replace({"virginica": 0, "setosa": 1})
+    ... )
+    >>> y = data["species"]
+    >>> X = data[["sepal_length", "sepal_width"]]
+    >>> model = RandomForestClassifier()
+    >>> model.fit(X=X, y=y)
+    >>> summary_df = summary_performance_metrics_classification(model=model, X_test=X, y_true=y)
+
     """
 
     y_pred = model.predict(X_test)
 
     # check if the fitted model has the "predict_proba" attribute
     if "predict_proba" in dir(model):
         # check that the fitted model has the "probability" attribute
@@ -864,7 +1044,33 @@
             "Mean AUC (CI 5%-95%)": bootstrap_auc_metric,
             "F1": f1,
         },
         index=["scores"],
     )
 
     return df_metrics.round(3)
+
+
+def RMSE(true, pred):
+    """Root Mean Squared Error.
+
+    Parameters
+    ----------
+    true: pd.Series
+        The actual values.
+    pred: pd.Series
+        The predicted values.
+
+    Returns
+    -------
+    float
+
+    Examples
+    --------
+    >>> import pandas as pd
+    >>> from jmspack.ml_utils import RMSE
+    >>> true = pd.Series([1, 2, 5, 4, 5])
+    >>> pred = pd.Series([1, 2, 3, 4, 5])
+    >>> RMSE(true, pred)
+
+    """
+    return np.sqrt(mean_squared_error(y_true=true, y_pred=pred))
```

### Comparing `jmspack-0.1.1/jmspack/utils.py` & `jmspack-0.1.2/jmspack/utils.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,15 +1,16 @@
-r"""Submodule utils.py includes the following functions and classes: <br>
+r"""Submodule utils.py includes the following functions and classes:
 
-    - **silence_stdout():** tmp <br>
-    - **JmsColors:** a class containing useful colours according to Jms and functions to show these colors in various forms.
-        <br>
-    - **apply_scaling():** a utility function to be used in conjunction with pandas pipe() to scale columns of a data frame
-        seperately. <br>
-    - **flatten():** a utility function used to flatten a list of lists to a single list. <br>
+- **silence_stdout():** A utility function used to stop other functions from printing to console (use with `with()`).
+
+- **JmsColors:** a class containing useful colours according to Jms and functions to show these colors in various forms.
+
+- **apply_scaling():** a utility function to be used in conjunction with pandas pipe() to scale columns of a data frame seperately.
+
+- **flatten():** a utility function used to flatten a list of lists to a single list.
 
 """
 import os
 import sys
 from contextlib import (
     contextmanager,
 )  # these three are needed to create the silence output function
@@ -20,45 +21,63 @@
 
 import matplotlib.pyplot as plt
 import pandas as pd
 from sklearn.preprocessing import MinMaxScaler
 from sklearn.preprocessing import StandardScaler
 
 
-# Create a function which will silence printing when called
 @contextmanager
 def silence_stdout():
+    """A utility function used to stop other functions from printing to console (use with `with()`).
+
+    Parameters
+    ----------
+    None
+
+    Returns
+    -------
+    None
+
+    Examples
+    --------
+    >>> with silence_stdout():
+    ...    print("This will not print to console")
+    >>> print("This will print to console")
+
+    """
+
     new_target = open(os.devnull, "w")
     old_target = sys.stdout
     sys.stdout = new_target
     try:
         yield new_target
     finally:
         sys.stdout = old_target
 
 
 class JmsColors:
-    r"""Utility class for James Twose's color codes.
-    Available Functions
-    --------
-    get_names(): returns a list of the color names e.g. [PURPLE, DARKBLUE, etc.]
-    to_dict(): returns a dictionary of format {color name: hexcode}
-    to_list(): returns a list of hexcodes
-    plot_colors(): returns a lineplot of all the available colours (like a color swatch)
+    """Utility class for James Twose's color codes.
+
+    Functions
+    ---------
+    - get_names(): returns a list of the color names e.g. [PURPLE, DARKBLUE, etc.]
+    - to_dict(): returns a dictionary of format {color name: hexcode}
+    - to_list(): returns a list of hexcodes
+    - plot_colors(): returns a lineplot of all the available colours (like a color swatch)
 
     Examples
     --------
     >>> import numpy as np
     >>> import matplotlib.pyplot as plt
     >>> from jmspack.utils import JmsColors
     >>> x = np.linspace(0, 10, 100)
     >>> fig = plt.figure()
-    >>> _ = plt.plot(x, np.sin(x), color=JmsColors.ORANGE)
-    >>> _ = plt.plot(x, np.cos(x), color=JmsColors.LIGHTBLUE)
-    >>> # plt.show()
+    >>> _ = plt.plot(x, np.sin(x), color=JmsColors.YELLOW)
+    >>> _ = plt.plot(x, np.cos(x), color=JmsColors.DARKBLUE)
+
     """
 
     PURPLE = "#8f0fd4"
     DARKBLUE = "#0072e8"
     BLUEGREEN = "#009cdc"
     GREENBLUE = "#00c7b1"
     GREENYELLOW = "#71db5c"
@@ -67,49 +86,52 @@
     DARKGREY = "#282d32"
     MEDIUMGREY = "#808080"
     LIGHTGREY = "#b1b1b1"
     OFFWHITE = "#d5d5d5"
 
     @staticmethod
     def get_names():
+        """Returns a list of the color names e.g. [PURPLE, DARKBLUE, etc.]"""
         return [
             k
             for k in JmsColors.__dict__.keys()
             if not k.startswith("__") and not callable(getattr(JmsColors, k))
         ]
 
     @staticmethod
     def to_dict():
+        """Returns a dictionary of format {color name: hexcode}"""
         return {
             k: v
             for k, v in JmsColors.__dict__.items()
             if not k.startswith("__") and not callable(getattr(JmsColors, k))
         }
 
     @staticmethod
     def to_list():
+        """Returns a list of hexcodes"""
         return [
             v
             for k, v in JmsColors.__dict__.items()
             if not k.startswith("__") and not callable(getattr(JmsColors, k))
         ]
 
     @staticmethod
     def plot_colors():
+        """Returns a lineplot of all the available colours (like a color swatch)"""
         for i, c in enumerate(JmsColors.to_list()):
             _ = plt.title("Available Jms Colors")
             _ = plt.plot([1, 5], [i, i], color=c, linewidth=5)
 
 
 def apply_scaling(
     df: pd.DataFrame,
     method: Union[str, Optional[Callable]] = "MinMax",
     kwargs: Dict = {},
 ):
-
     r"""Utility function to be used in conjunction with pandas pipe()
     to scale columns of a data frame seperately.
 
     Parameters
     ----------
     df: pd.DataFrame
         The data frame you want to scale.
@@ -118,25 +140,27 @@
         "Standard"], or an Sklearn transformer,
         see: https://scikit-learn.org/stable/modules/preprocessing.html
     kwargs: Dict
         Dictionary containing additional keywords to be added to the Scaler.
 
     Returns
     -------
-    pd.DataFrame
+    scal_df: pd.DataFrame
+        The scaled data frame.
 
     Examples
     --------
     >>> import seaborn as sns
     >>> import pandas as pd
     >>> df = sns.load_dataset("iris")
     >>> scaled_df = (df
     ...             .select_dtypes("number")
     ...             .pipe(apply_scaling)
     ...             )
+
     """
 
     if method == "MinMax":
         scal_df = pd.DataFrame(
             MinMaxScaler(**kwargs).fit_transform(df),
             index=df.index,
             columns=df.columns,
@@ -160,16 +184,16 @@
     Parameters
     ----------
     l: list
         A list of lists.
 
     Returns
     -------
-    pd.DataFrame
-
+    list
+        The flattened list.
 
     Examples
     --------
     >>> from jmspack.utils import flatten
     >>> list_of_lists = [[f"p_{x}" for x in range(10)],
     ...                 [f"p_{x}" for x in range(10, 20)],
     ...                 [f"p_{x}" for x in range(20, 30)]]
```

### Comparing `jmspack-0.1.1/setup.py` & `jmspack-0.1.2/setup.py`

 * *Files identical despite different names*

