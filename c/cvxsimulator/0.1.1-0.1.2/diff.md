# Comparing `tmp/cvxsimulator-0.1.1.tar.gz` & `tmp/cvxsimulator-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cvxsimulator-0.1.1.tar", max compression
+gzip compressed data, was "cvxsimulator-0.1.2.tar", max compression
```

## Comparing `cvxsimulator-0.1.1.tar` & `cvxsimulator-0.1.2.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1102 2023-05-05 00:01:58.403087 cvxsimulator-0.1.1/LICENSE
--rw-r--r--   0        0        0     4115 2023-05-05 00:01:58.403087 cvxsimulator-0.1.1/README.md
--rw-r--r--   0        0        0        0 2023-05-05 00:01:58.431087 cvxsimulator-0.1.1/cvx/simulator/__init__.py
--rw-r--r--   0        0        0     1163 2023-05-05 00:01:58.431087 cvxsimulator-0.1.1/cvx/simulator/metrics.py
--rw-r--r--   0        0        0     4917 2023-05-05 00:01:58.431087 cvxsimulator-0.1.1/cvx/simulator/portfolio.py
--rw-r--r--   0        0        0      464 2023-05-05 00:01:58.431087 cvxsimulator-0.1.1/cvx/simulator/trading_costs.py
--rw-r--r--   0        0        0      491 2023-05-05 00:02:22.358812 cvxsimulator-0.1.1/pyproject.toml
--rw-r--r--   0        0        0     4584 1970-01-01 00:00:00.000000 cvxsimulator-0.1.1/PKG-INFO
+-rw-r--r--   0        0        0     1102 2023-05-05 03:24:23.435125 cvxsimulator-0.1.2/LICENSE
+-rw-r--r--   0        0        0     4115 2023-05-05 03:24:23.435125 cvxsimulator-0.1.2/README.md
+-rw-r--r--   0        0        0        0 2023-05-05 03:24:23.471128 cvxsimulator-0.1.2/cvx/simulator/__init__.py
+-rw-r--r--   0        0        0     1163 2023-05-05 03:24:23.471128 cvxsimulator-0.1.2/cvx/simulator/metrics.py
+-rw-r--r--   0        0        0     4917 2023-05-05 03:24:23.471128 cvxsimulator-0.1.2/cvx/simulator/portfolio.py
+-rw-r--r--   0        0        0      464 2023-05-05 03:24:23.471128 cvxsimulator-0.1.2/cvx/simulator/trading_costs.py
+-rw-r--r--   0        0        0      537 2023-05-05 03:24:43.120525 cvxsimulator-0.1.2/pyproject.toml
+-rw-r--r--   0        0        0     4675 1970-01-01 00:00:00.000000 cvxsimulator-0.1.2/PKG-INFO
```

### Comparing `cvxsimulator-0.1.1/LICENSE` & `cvxsimulator-0.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `cvxsimulator-0.1.1/README.md` & `cvxsimulator-0.1.2/README.md`

 * *Files identical despite different names*

### Comparing `cvxsimulator-0.1.1/cvx/simulator/metrics.py` & `cvxsimulator-0.1.2/cvx/simulator/metrics.py`

 * *Files identical despite different names*

### Comparing `cvxsimulator-0.1.1/cvx/simulator/portfolio.py` & `cvxsimulator-0.1.2/cvx/simulator/portfolio.py`

 * *Files identical despite different names*

### Comparing `cvxsimulator-0.1.1/PKG-INFO` & `cvxsimulator-0.1.2/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,19 +1,21 @@
 Metadata-Version: 2.1
 Name: cvxsimulator
-Version: 0.1.1
+Version: 0.1.2
 Summary: Simple simulator for investors
+Home-page: https://github.com/cvxgrp/simulator
 Author: Thomas Schmelzer
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Requires-Dist: numpy (>=1.24.2,<2.0.0)
-Requires-Dist: pandas (>=2.0.0,<3.0.0)
+Requires-Dist: pandas
+Project-URL: Repository, https://github.com/cvxgrp/simulator
 Description-Content-Type: text/markdown
 
 # [cvxsimulator](http://www.cvxgrp.org/simulator/)
 
 [![binder](https://github.com/cvxgrp/simulator/actions/workflows/binder.yml/badge.svg)](https://github.com/cvxgrp/simulator/actions/workflows/binder.yml)
 [![Book](https://github.com/cvxgrp/simulator/actions/workflows/book.yml/badge.svg)](https://github.com/cvxgrp/simulator/actions/workflows/book.yml)
 [![Test](https://github.com/cvxgrp/simulator/actions/workflows/test.yml/badge.svg)](https://github.com/cvxgrp/simulator/actions/workflows/test.yml)
```

