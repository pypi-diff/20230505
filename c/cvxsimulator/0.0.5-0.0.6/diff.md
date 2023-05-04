# Comparing `tmp/cvxsimulator-0.0.5.tar.gz` & `tmp/cvxsimulator-0.0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cvxsimulator-0.0.5.tar", max compression
+gzip compressed data, was "cvxsimulator-0.0.6.tar", max compression
```

## Comparing `cvxsimulator-0.0.5.tar` & `cvxsimulator-0.0.6.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1102 2023-05-04 22:41:05.232216 cvxsimulator-0.0.5/LICENSE
--rw-r--r--   0        0        0     4118 2023-05-04 22:41:05.232216 cvxsimulator-0.0.5/README.md
--rw-r--r--   0        0        0        0 2023-05-04 22:41:05.264216 cvxsimulator-0.0.5/cvx/simulator/__init__.py
--rw-r--r--   0        0        0     1163 2023-05-04 22:41:05.264216 cvxsimulator-0.0.5/cvx/simulator/metrics.py
--rw-r--r--   0        0        0     4917 2023-05-04 22:41:05.264216 cvxsimulator-0.0.5/cvx/simulator/portfolio.py
--rw-r--r--   0        0        0      464 2023-05-04 22:41:05.264216 cvxsimulator-0.0.5/cvx/simulator/trading_costs.py
--rw-r--r--   0        0        0      509 2023-05-04 22:41:28.732349 cvxsimulator-0.0.5/pyproject.toml
--rw-r--r--   0        0        0     4605 1970-01-01 00:00:00.000000 cvxsimulator-0.0.5/PKG-INFO
+-rw-r--r--   0        0        0     1102 2023-05-04 22:46:34.909043 cvxsimulator-0.0.6/LICENSE
+-rw-r--r--   0        0        0     4118 2023-05-04 22:46:34.909043 cvxsimulator-0.0.6/README.md
+-rw-r--r--   0        0        0        0 2023-05-04 22:46:34.941043 cvxsimulator-0.0.6/cvx/simulator/__init__.py
+-rw-r--r--   0        0        0     1163 2023-05-04 22:46:34.941043 cvxsimulator-0.0.6/cvx/simulator/metrics.py
+-rw-r--r--   0        0        0     4917 2023-05-04 22:46:34.941043 cvxsimulator-0.0.6/cvx/simulator/portfolio.py
+-rw-r--r--   0        0        0      464 2023-05-04 22:46:34.941043 cvxsimulator-0.0.6/cvx/simulator/trading_costs.py
+-rw-r--r--   0        0        0      508 2023-05-04 22:47:01.949200 cvxsimulator-0.0.6/pyproject.toml
+-rw-r--r--   0        0        0     4605 1970-01-01 00:00:00.000000 cvxsimulator-0.0.6/PKG-INFO
```

### Comparing `cvxsimulator-0.0.5/LICENSE` & `cvxsimulator-0.0.6/LICENSE`

 * *Files identical despite different names*

### Comparing `cvxsimulator-0.0.5/README.md` & `cvxsimulator-0.0.6/README.md`

 * *Files identical despite different names*

### Comparing `cvxsimulator-0.0.5/cvx/simulator/metrics.py` & `cvxsimulator-0.0.6/cvx/simulator/metrics.py`

 * *Files identical despite different names*

### Comparing `cvxsimulator-0.0.5/cvx/simulator/portfolio.py` & `cvxsimulator-0.0.6/cvx/simulator/portfolio.py`

 * *Files identical despite different names*

### Comparing `cvxsimulator-0.0.5/PKG-INFO` & `cvxsimulator-0.0.6/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cvxsimulator
-Version: 0.0.5
+Version: 0.0.6
 Summary: Simple simulator for investors
 Author: Thomas Schmelzer, and Stephen Boyd
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

