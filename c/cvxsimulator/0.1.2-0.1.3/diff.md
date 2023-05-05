# Comparing `tmp/cvxsimulator-0.1.2.tar.gz` & `tmp/cvxsimulator-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cvxsimulator-0.1.2.tar", max compression
+gzip compressed data, was "cvxsimulator-0.1.3.tar", max compression
```

## Comparing `cvxsimulator-0.1.2.tar` & `cvxsimulator-0.1.3.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1102 2023-05-05 03:24:23.435125 cvxsimulator-0.1.2/LICENSE
--rw-r--r--   0        0        0     4115 2023-05-05 03:24:23.435125 cvxsimulator-0.1.2/README.md
--rw-r--r--   0        0        0        0 2023-05-05 03:24:23.471128 cvxsimulator-0.1.2/cvx/simulator/__init__.py
--rw-r--r--   0        0        0     1163 2023-05-05 03:24:23.471128 cvxsimulator-0.1.2/cvx/simulator/metrics.py
--rw-r--r--   0        0        0     4917 2023-05-05 03:24:23.471128 cvxsimulator-0.1.2/cvx/simulator/portfolio.py
--rw-r--r--   0        0        0      464 2023-05-05 03:24:23.471128 cvxsimulator-0.1.2/cvx/simulator/trading_costs.py
--rw-r--r--   0        0        0      537 2023-05-05 03:24:43.120525 cvxsimulator-0.1.2/pyproject.toml
--rw-r--r--   0        0        0     4675 1970-01-01 00:00:00.000000 cvxsimulator-0.1.2/PKG-INFO
+-rw-r--r--   0        0        0     1102 2023-05-05 04:02:45.893140 cvxsimulator-0.1.3/LICENSE
+-rw-r--r--   0        0        0     4477 2023-05-05 04:02:45.893140 cvxsimulator-0.1.3/README.md
+-rw-r--r--   0        0        0        0 2023-05-05 04:02:45.929141 cvxsimulator-0.1.3/cvx/simulator/__init__.py
+-rw-r--r--   0        0        0     1163 2023-05-05 04:02:45.929141 cvxsimulator-0.1.3/cvx/simulator/metrics.py
+-rw-r--r--   0        0        0     4917 2023-05-05 04:02:45.929141 cvxsimulator-0.1.3/cvx/simulator/portfolio.py
+-rw-r--r--   0        0        0      464 2023-05-05 04:02:45.929141 cvxsimulator-0.1.3/cvx/simulator/trading_costs.py
+-rw-r--r--   0        0        0      537 2023-05-05 04:03:08.787907 cvxsimulator-0.1.3/pyproject.toml
+-rw-r--r--   0        0        0     5037 1970-01-01 00:00:00.000000 cvxsimulator-0.1.3/PKG-INFO
```

### Comparing `cvxsimulator-0.1.2/LICENSE` & `cvxsimulator-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `cvxsimulator-0.1.2/README.md` & `cvxsimulator-0.1.3/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -1,12 +1,15 @@
 # [cvxsimulator](http://www.cvxgrp.org/simulator/)
 
 [![binder](https://github.com/cvxgrp/simulator/actions/workflows/binder.yml/badge.svg)](https://github.com/cvxgrp/simulator/actions/workflows/binder.yml)
 [![Book](https://github.com/cvxgrp/simulator/actions/workflows/book.yml/badge.svg)](https://github.com/cvxgrp/simulator/actions/workflows/book.yml)
 [![Test](https://github.com/cvxgrp/simulator/actions/workflows/test.yml/badge.svg)](https://github.com/cvxgrp/simulator/actions/workflows/test.yml)
+[![PyPI version](https://badge.fury.io/py/cvxsimulator.svg)](https://badge.fury.io/py/cvxsimulator)
+[![Apache 2.0 License](https://img.shields.io/badge/License-APACHEv2-brightgreen.svg)](https://github.com/cvxgrp/simulator/blob/master/LICENSE)
+[![PyPI download month](https://img.shields.io/pypi/dm/cvxsimulator.svg)](https://pypi.python.org/pypi/cvxsimulator/)
 
 Given a universe of $m$ assets we are given prices for each of them at time $t_1, t_2, \ldots t_n$, 
 e.g. we operate using an $n \times m$ matrix where each column corresponds to a particular asset.
 
 In a backtest we iterate in time (e.g. row by row) through the matrix and allocate positions to all or some of the assets.
 This tool shall help to simplify the accounting. It keeps track of the available cash, the profits achieved, etc.
```

### Comparing `cvxsimulator-0.1.2/cvx/simulator/metrics.py` & `cvxsimulator-0.1.3/cvx/simulator/metrics.py`

 * *Files identical despite different names*

### Comparing `cvxsimulator-0.1.2/cvx/simulator/portfolio.py` & `cvxsimulator-0.1.3/cvx/simulator/portfolio.py`

 * *Files identical despite different names*

### Comparing `cvxsimulator-0.1.2/pyproject.toml` & `cvxsimulator-0.1.3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "cvxsimulator"
-version = "v0.1.2"
+version = "v0.1.3"
 description = "Simple simulator for investors"
 authors = ["Thomas Schmelzer"]
 readme = "README.md"
 repository = "https://github.com/cvxgrp/simulator"
 packages = [{include = "cvx"}]
 
 [tool.poetry.dependencies]
```

### Comparing `cvxsimulator-0.1.2/PKG-INFO` & `cvxsimulator-0.1.3/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cvxsimulator
-Version: 0.1.2
+Version: 0.1.3
 Summary: Simple simulator for investors
 Home-page: https://github.com/cvxgrp/simulator
 Author: Thomas Schmelzer
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
@@ -15,14 +15,17 @@
 Description-Content-Type: text/markdown
 
 # [cvxsimulator](http://www.cvxgrp.org/simulator/)
 
 [![binder](https://github.com/cvxgrp/simulator/actions/workflows/binder.yml/badge.svg)](https://github.com/cvxgrp/simulator/actions/workflows/binder.yml)
 [![Book](https://github.com/cvxgrp/simulator/actions/workflows/book.yml/badge.svg)](https://github.com/cvxgrp/simulator/actions/workflows/book.yml)
 [![Test](https://github.com/cvxgrp/simulator/actions/workflows/test.yml/badge.svg)](https://github.com/cvxgrp/simulator/actions/workflows/test.yml)
+[![PyPI version](https://badge.fury.io/py/cvxsimulator.svg)](https://badge.fury.io/py/cvxsimulator)
+[![Apache 2.0 License](https://img.shields.io/badge/License-APACHEv2-brightgreen.svg)](https://github.com/cvxgrp/simulator/blob/master/LICENSE)
+[![PyPI download month](https://img.shields.io/pypi/dm/cvxsimulator.svg)](https://pypi.python.org/pypi/cvxsimulator/)
 
 Given a universe of $m$ assets we are given prices for each of them at time $t_1, t_2, \ldots t_n$, 
 e.g. we operate using an $n \times m$ matrix where each column corresponds to a particular asset.
 
 In a backtest we iterate in time (e.g. row by row) through the matrix and allocate positions to all or some of the assets.
 This tool shall help to simplify the accounting. It keeps track of the available cash, the profits achieved, etc.
```

