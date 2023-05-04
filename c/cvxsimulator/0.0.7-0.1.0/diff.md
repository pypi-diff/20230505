# Comparing `tmp/cvxsimulator-0.0.7.tar.gz` & `tmp/cvxsimulator-0.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cvxsimulator-0.0.7.tar", max compression
+gzip compressed data, was "cvxsimulator-0.1.0.tar", max compression
```

## Comparing `cvxsimulator-0.0.7.tar` & `cvxsimulator-0.1.0.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1102 2023-05-04 22:53:08.605310 cvxsimulator-0.0.7/LICENSE
--rw-r--r--   0        0        0     4118 2023-05-04 22:53:08.605310 cvxsimulator-0.0.7/README.md
--rw-r--r--   0        0        0        0 2023-05-04 22:53:08.641310 cvxsimulator-0.0.7/cvx/simulator/__init__.py
--rw-r--r--   0        0        0     1163 2023-05-04 22:53:08.641310 cvxsimulator-0.0.7/cvx/simulator/metrics.py
--rw-r--r--   0        0        0     4917 2023-05-04 22:53:08.641310 cvxsimulator-0.0.7/cvx/simulator/portfolio.py
--rw-r--r--   0        0        0      464 2023-05-04 22:53:08.641310 cvxsimulator-0.0.7/cvx/simulator/trading_costs.py
--rw-r--r--   0        0        0      491 2023-05-04 22:53:32.253863 cvxsimulator-0.0.7/pyproject.toml
--rw-r--r--   0        0        0     4587 1970-01-01 00:00:00.000000 cvxsimulator-0.0.7/PKG-INFO
+-rw-r--r--   0        0        0     1102 2023-05-04 23:34:01.985417 cvxsimulator-0.1.0/LICENSE
+-rw-r--r--   0        0        0     4115 2023-05-04 23:34:01.985417 cvxsimulator-0.1.0/README.md
+-rw-r--r--   0        0        0        0 2023-05-04 23:34:02.017417 cvxsimulator-0.1.0/cvx/simulator/__init__.py
+-rw-r--r--   0        0        0     1163 2023-05-04 23:34:02.017417 cvxsimulator-0.1.0/cvx/simulator/metrics.py
+-rw-r--r--   0        0        0     4917 2023-05-04 23:34:02.017417 cvxsimulator-0.1.0/cvx/simulator/portfolio.py
+-rw-r--r--   0        0        0      464 2023-05-04 23:34:02.017417 cvxsimulator-0.1.0/cvx/simulator/trading_costs.py
+-rw-r--r--   0        0        0      491 2023-05-04 23:34:25.285842 cvxsimulator-0.1.0/pyproject.toml
+-rw-r--r--   0        0        0     4584 1970-01-01 00:00:00.000000 cvxsimulator-0.1.0/PKG-INFO
```

### Comparing `cvxsimulator-0.0.7/LICENSE` & `cvxsimulator-0.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `cvxsimulator-0.0.7/README.md` & `cvxsimulator-0.1.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# [cvx.simulator](http://www.cvxgrp.org/simulator/)
+# [cvxsimulator](http://www.cvxgrp.org/simulator/)
 
 [![binder](https://github.com/cvxgrp/simulator/actions/workflows/binder.yml/badge.svg)](https://github.com/cvxgrp/simulator/actions/workflows/binder.yml)
 [![Book](https://github.com/cvxgrp/simulator/actions/workflows/book.yml/badge.svg)](https://github.com/cvxgrp/simulator/actions/workflows/book.yml)
 [![Test](https://github.com/cvxgrp/simulator/actions/workflows/test.yml/badge.svg)](https://github.com/cvxgrp/simulator/actions/workflows/test.yml)
 
 Given a universe of $m$ assets we are given prices for each of them at time $t_1, t_2, \ldots t_n$, 
 e.g. we operate using an $n \times m$ matrix where each column corresponds to a particular asset.
@@ -89,15 +89,15 @@
 
 We assume you share already the love for [Poetry](https://python-poetry.org). Once you have installed poetry you can perform
 
 ```bash
 poetry install
 ```
 
-to replicate the virtual environment we have defined in pyproject.toml.  
+to replicate the virtual environment we have defined in pyproject.toml.
 
 ## Kernel
 
 We install [JupyterLab](https://jupyter.org) within your new virtual environment. Executing
 
 ```bash
 ./create_kernel.sh
```

### Comparing `cvxsimulator-0.0.7/cvx/simulator/metrics.py` & `cvxsimulator-0.1.0/cvx/simulator/metrics.py`

 * *Files identical despite different names*

### Comparing `cvxsimulator-0.0.7/cvx/simulator/portfolio.py` & `cvxsimulator-0.1.0/cvx/simulator/portfolio.py`

 * *Files identical despite different names*

### Comparing `cvxsimulator-0.0.7/PKG-INFO` & `cvxsimulator-0.1.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 Metadata-Version: 2.1
 Name: cvxsimulator
-Version: 0.0.7
+Version: 0.1.0
 Summary: Simple simulator for investors
 Author: Thomas Schmelzer
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: numpy (>=1.24.2,<2.0.0)
 Requires-Dist: pandas (>=2.0.0,<3.0.0)
 Description-Content-Type: text/markdown
 
-# [cvx.simulator](http://www.cvxgrp.org/simulator/)
+# [cvxsimulator](http://www.cvxgrp.org/simulator/)
 
 [![binder](https://github.com/cvxgrp/simulator/actions/workflows/binder.yml/badge.svg)](https://github.com/cvxgrp/simulator/actions/workflows/binder.yml)
 [![Book](https://github.com/cvxgrp/simulator/actions/workflows/book.yml/badge.svg)](https://github.com/cvxgrp/simulator/actions/workflows/book.yml)
 [![Test](https://github.com/cvxgrp/simulator/actions/workflows/test.yml/badge.svg)](https://github.com/cvxgrp/simulator/actions/workflows/test.yml)
 
 Given a universe of $m$ assets we are given prices for each of them at time $t_1, t_2, \ldots t_n$, 
 e.g. we operate using an $n \times m$ matrix where each column corresponds to a particular asset.
@@ -103,15 +103,15 @@
 
 We assume you share already the love for [Poetry](https://python-poetry.org). Once you have installed poetry you can perform
 
 ```bash
 poetry install
 ```
 
-to replicate the virtual environment we have defined in pyproject.toml.  
+to replicate the virtual environment we have defined in pyproject.toml.
 
 ## Kernel
 
 We install [JupyterLab](https://jupyter.org) within your new virtual environment. Executing
 
 ```bash
 ./create_kernel.sh
```

