# Comparing `tmp/py-portfolio-tools-0.0.6.tar.gz` & `tmp/py-portfolio-tools-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py-portfolio-tools-0.0.6.tar", last modified: Fri May  5 17:31:17 2023, max compression
+gzip compressed data, was "py-portfolio-tools-0.0.7.tar", last modified: Fri May  5 17:32:19 2023, max compression
```

## Comparing `py-portfolio-tools-0.0.6.tar` & `py-portfolio-tools-0.0.7.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxrwx   0        0        0        0 2023-05-05 17:31:17.932667 py-portfolio-tools-0.0.6/
--rw-rw-rw-   0        0        0     1075 2023-04-17 11:45:54.000000 py-portfolio-tools-0.0.6/LICENSE.md
--rw-rw-rw-   0        0        0     1198 2023-05-05 17:31:17.932667 py-portfolio-tools-0.0.6/PKG-INFO
--rw-rw-rw-   0        0        0       44 2023-04-17 11:54:14.000000 py-portfolio-tools-0.0.6/README.md
-drwxrwxrwx   0        0        0        0 2023-05-05 17:31:17.917717 py-portfolio-tools-0.0.6/py-portfolio-tools/
--rw-rw-rw-   0        0        0     2545 2023-04-17 18:42:57.000000 py-portfolio-tools-0.0.6/py-portfolio-tools/DataFetch.py
--rw-rw-rw-   0        0        0      703 2023-04-17 13:42:55.000000 py-portfolio-tools-0.0.6/py-portfolio-tools/Logger.py
--rw-rw-rw-   0        0        0     8463 2023-05-05 11:00:54.000000 py-portfolio-tools-0.0.6/py-portfolio-tools/Portfolio.py
--rw-rw-rw-   0        0        0     3232 2023-04-23 17:24:00.000000 py-portfolio-tools-0.0.6/py-portfolio-tools/PortfolioInputWindow.py
--rw-rw-rw-   0        0        0     8397 2023-05-05 11:08:15.000000 py-portfolio-tools-0.0.6/py-portfolio-tools/PortfolioManager.py
--rw-rw-rw-   0        0        0       30 2023-04-17 14:28:58.000000 py-portfolio-tools-0.0.6/py-portfolio-tools/Predictor.py
--rw-rw-rw-   0        0        0     3151 2023-05-05 11:22:09.000000 py-portfolio-tools-0.0.6/py-portfolio-tools/StocksAllocator.py
--rw-rw-rw-   0        0        0     2076 2023-04-23 17:24:05.000000 py-portfolio-tools-0.0.6/py-portfolio-tools/Tickers.py
--rw-rw-rw-   0        0        0     6864 2023-04-22 07:56:08.000000 py-portfolio-tools-0.0.6/py-portfolio-tools/Utils.py
--rw-rw-rw-   0        0        0      243 2023-04-22 07:44:44.000000 py-portfolio-tools-0.0.6/py-portfolio-tools/__init__.py
--rw-rw-rw-   0        0        0     1397 2023-04-21 18:15:14.000000 py-portfolio-tools-0.0.6/py-portfolio-tools/__main__.py
-drwxrwxrwx   0        0        0        0 2023-05-05 17:31:17.931671 py-portfolio-tools-0.0.6/py_portfolio_tools.egg-info/
--rw-rw-rw-   0        0        0     1198 2023-05-05 17:31:17.000000 py-portfolio-tools-0.0.6/py_portfolio_tools.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      603 2023-05-05 17:31:17.000000 py-portfolio-tools-0.0.6/py_portfolio_tools.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-05 17:31:17.000000 py-portfolio-tools-0.0.6/py_portfolio_tools.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       66 2023-05-05 17:31:17.000000 py-portfolio-tools-0.0.6/py_portfolio_tools.egg-info/requires.txt
--rw-rw-rw-   0        0        0       19 2023-05-05 17:31:17.000000 py-portfolio-tools-0.0.6/py_portfolio_tools.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-05 17:31:17.933664 py-portfolio-tools-0.0.6/setup.cfg
--rw-rw-rw-   0        0        0     1633 2023-05-05 17:30:59.000000 py-portfolio-tools-0.0.6/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-05 17:32:19.437162 py-portfolio-tools-0.0.7/
+-rw-rw-rw-   0        0        0     1075 2023-04-17 11:45:54.000000 py-portfolio-tools-0.0.7/LICENSE.md
+-rw-rw-rw-   0        0        0     1198 2023-05-05 17:32:19.437162 py-portfolio-tools-0.0.7/PKG-INFO
+-rw-rw-rw-   0        0        0       44 2023-04-17 11:54:14.000000 py-portfolio-tools-0.0.7/README.md
+drwxrwxrwx   0        0        0        0 2023-05-05 17:32:19.437162 py-portfolio-tools-0.0.7/py-portfolio-tools/
+-rw-rw-rw-   0        0        0     2545 2023-04-17 18:42:57.000000 py-portfolio-tools-0.0.7/py-portfolio-tools/DataFetch.py
+-rw-rw-rw-   0        0        0      703 2023-04-17 13:42:55.000000 py-portfolio-tools-0.0.7/py-portfolio-tools/Logger.py
+-rw-rw-rw-   0        0        0     8330 2023-05-05 17:32:02.000000 py-portfolio-tools-0.0.7/py-portfolio-tools/Portfolio.py
+-rw-rw-rw-   0        0        0     3232 2023-04-23 17:24:00.000000 py-portfolio-tools-0.0.7/py-portfolio-tools/PortfolioInputWindow.py
+-rw-rw-rw-   0        0        0     8397 2023-05-05 11:08:15.000000 py-portfolio-tools-0.0.7/py-portfolio-tools/PortfolioManager.py
+-rw-rw-rw-   0        0        0       30 2023-04-17 14:28:58.000000 py-portfolio-tools-0.0.7/py-portfolio-tools/Predictor.py
+-rw-rw-rw-   0        0        0     3151 2023-05-05 11:22:09.000000 py-portfolio-tools-0.0.7/py-portfolio-tools/StocksAllocator.py
+-rw-rw-rw-   0        0        0     2076 2023-04-23 17:24:05.000000 py-portfolio-tools-0.0.7/py-portfolio-tools/Tickers.py
+-rw-rw-rw-   0        0        0     6864 2023-04-22 07:56:08.000000 py-portfolio-tools-0.0.7/py-portfolio-tools/Utils.py
+-rw-rw-rw-   0        0        0      243 2023-04-22 07:44:44.000000 py-portfolio-tools-0.0.7/py-portfolio-tools/__init__.py
+-rw-rw-rw-   0        0        0     1397 2023-04-21 18:15:14.000000 py-portfolio-tools-0.0.7/py-portfolio-tools/__main__.py
+drwxrwxrwx   0        0        0        0 2023-05-05 17:32:19.437162 py-portfolio-tools-0.0.7/py_portfolio_tools.egg-info/
+-rw-rw-rw-   0        0        0     1198 2023-05-05 17:32:19.000000 py-portfolio-tools-0.0.7/py_portfolio_tools.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      603 2023-05-05 17:32:19.000000 py-portfolio-tools-0.0.7/py_portfolio_tools.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-05 17:32:19.000000 py-portfolio-tools-0.0.7/py_portfolio_tools.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       66 2023-05-05 17:32:19.000000 py-portfolio-tools-0.0.7/py_portfolio_tools.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       19 2023-05-05 17:32:19.000000 py-portfolio-tools-0.0.7/py_portfolio_tools.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-05 17:32:19.437162 py-portfolio-tools-0.0.7/setup.cfg
+-rw-rw-rw-   0        0        0     1633 2023-05-05 17:32:11.000000 py-portfolio-tools-0.0.7/setup.py
```

### Comparing `py-portfolio-tools-0.0.6/LICENSE.md` & `py-portfolio-tools-0.0.7/LICENSE.md`

 * *Files identical despite different names*

### Comparing `py-portfolio-tools-0.0.6/PKG-INFO` & `py-portfolio-tools-0.0.7/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py-portfolio-tools
-Version: 0.0.6
+Version: 0.0.7
 Summary: A Python Library and set of GUI tools for Portfolio Management
 Home-page: https://gitlab.com/Jaysmito101/py-portfolio-tools
 Author: Jaysmito Mukherjee
 Author-email: jaysmito101@gmail.com
 License: MIT
 Project-URL: Documentation, https://gitlab.com/Jaysmito101/py-portfolio-tools/-/wikis/Home
 Project-URL: Issue tracker, https://gitlab.com/Jaysmito101/py-portfolio-tools/-/issues
```

### Comparing `py-portfolio-tools-0.0.6/py-portfolio-tools/DataFetch.py` & `py-portfolio-tools-0.0.7/py-portfolio-tools/DataFetch.py`

 * *Files identical despite different names*

### Comparing `py-portfolio-tools-0.0.6/py-portfolio-tools/Logger.py` & `py-portfolio-tools-0.0.7/py-portfolio-tools/Logger.py`

 * *Files identical despite different names*

### Comparing `py-portfolio-tools-0.0.6/py-portfolio-tools/Portfolio.py` & `py-portfolio-tools-0.0.7/py-portfolio-tools/Portfolio.py`

 * *Files 2% similar despite different names*

```diff
@@ -5,19 +5,14 @@
 import numpy as np
 import json
 import os
 import io
 import imgui
 import matplotlib.pyplot as plt
 
-from pypfopt.efficient_frontier import EfficientFrontier
-from pypfopt import risk_models
-from pypfopt import expected_returns
-
-
 class Portfolio:
     """Portfolio is a class that handles the portfolio"""
 
     def __init__(self, name, stocks, weights = None, predictor = None, dataFetch = DataFetch(), logger = Logger("PPFT")):
         """Initialise the portfolio with the given name, stocks, weights, predictor, dataFetch and logger"""
         self._name = name
         self._stocks = stocks
```

### Comparing `py-portfolio-tools-0.0.6/py-portfolio-tools/PortfolioInputWindow.py` & `py-portfolio-tools-0.0.7/py-portfolio-tools/PortfolioInputWindow.py`

 * *Files identical despite different names*

### Comparing `py-portfolio-tools-0.0.6/py-portfolio-tools/PortfolioManager.py` & `py-portfolio-tools-0.0.7/py-portfolio-tools/PortfolioManager.py`

 * *Files identical despite different names*

### Comparing `py-portfolio-tools-0.0.6/py-portfolio-tools/StocksAllocator.py` & `py-portfolio-tools-0.0.7/py-portfolio-tools/StocksAllocator.py`

 * *Files identical despite different names*

### Comparing `py-portfolio-tools-0.0.6/py-portfolio-tools/Tickers.py` & `py-portfolio-tools-0.0.7/py-portfolio-tools/Tickers.py`

 * *Files identical despite different names*

### Comparing `py-portfolio-tools-0.0.6/py-portfolio-tools/Utils.py` & `py-portfolio-tools-0.0.7/py-portfolio-tools/Utils.py`

 * *Files identical despite different names*

### Comparing `py-portfolio-tools-0.0.6/py-portfolio-tools/__main__.py` & `py-portfolio-tools-0.0.7/py-portfolio-tools/__main__.py`

 * *Files identical despite different names*

### Comparing `py-portfolio-tools-0.0.6/py_portfolio_tools.egg-info/PKG-INFO` & `py-portfolio-tools-0.0.7/py_portfolio_tools.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: py-portfolio-tools
-Version: 0.0.6
+Version: 0.0.7
 Summary: A Python Library and set of GUI tools for Portfolio Management
 Home-page: https://gitlab.com/Jaysmito101/py-portfolio-tools
 Author: Jaysmito Mukherjee
 Author-email: jaysmito101@gmail.com
 License: MIT
 Project-URL: Documentation, https://gitlab.com/Jaysmito101/py-portfolio-tools/-/wikis/Home
 Project-URL: Issue tracker, https://gitlab.com/Jaysmito101/py-portfolio-tools/-/issues
```

### Comparing `py-portfolio-tools-0.0.6/py_portfolio_tools.egg-info/SOURCES.txt` & `py-portfolio-tools-0.0.7/py_portfolio_tools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `py-portfolio-tools-0.0.6/setup.py` & `py-portfolio-tools-0.0.7/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from setuptools import setup, find_packages
 import re
 
 requirements = ['numpy', 'pandas', 'matplotlib', 'yfinance', "PyOpenGL", "glfw", "imgui[glfw]", "Pillow"] 
 
-version = '0.0.6'
+version = '0.0.7'
 
 if not version:
     raise RuntimeError('version is not set')
 
 readme = 'Coming Soon ...'
 
 setup(
```

