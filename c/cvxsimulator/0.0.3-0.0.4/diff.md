# Comparing `tmp/cvxsimulator-0.0.3.tar.gz` & `tmp/cvxsimulator-0.0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cvxsimulator-0.0.3.tar", max compression
+gzip compressed data, was "cvxsimulator-0.0.4.tar", max compression
```

## Comparing `cvxsimulator-0.0.3.tar` & `cvxsimulator-0.0.4.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1102 2023-05-04 22:19:56.729473 cvxsimulator-0.0.3/LICENSE
--rw-r--r--   0        0        0     4118 2023-05-04 22:19:56.729473 cvxsimulator-0.0.3/README.md
--rw-r--r--   0        0        0        0 2023-05-04 22:19:56.765477 cvxsimulator-0.0.3/cvx/simulator/__init__.py
--rw-r--r--   0        0        0     1163 2023-05-04 22:19:56.765477 cvxsimulator-0.0.3/cvx/simulator/metrics.py
--rw-r--r--   0        0        0     4917 2023-05-04 22:19:56.765477 cvxsimulator-0.0.3/cvx/simulator/portfolio.py
--rw-r--r--   0        0        0      464 2023-05-04 22:19:56.765477 cvxsimulator-0.0.3/cvx/simulator/trading_costs.py
--rw-r--r--   0        0        0      508 2023-05-04 22:20:21.819419 cvxsimulator-0.0.3/pyproject.toml
--rw-r--r--   0        0        0     4605 1970-01-01 00:00:00.000000 cvxsimulator-0.0.3/PKG-INFO
+-rw-r--r--   0        0        0     1102 2023-05-04 22:22:04.824048 cvxsimulator-0.0.4/LICENSE
+-rw-r--r--   0        0        0     4118 2023-05-04 22:22:04.824048 cvxsimulator-0.0.4/README.md
+-rw-r--r--   0        0        0        0 2023-05-04 22:22:04.856049 cvxsimulator-0.0.4/cvx/simulator/__init__.py
+-rw-r--r--   0        0        0     1163 2023-05-04 22:22:04.856049 cvxsimulator-0.0.4/cvx/simulator/metrics.py
+-rw-r--r--   0        0        0     4917 2023-05-04 22:22:04.856049 cvxsimulator-0.0.4/cvx/simulator/portfolio.py
+-rw-r--r--   0        0        0      464 2023-05-04 22:22:04.856049 cvxsimulator-0.0.4/cvx/simulator/trading_costs.py
+-rw-r--r--   0        0        0      508 2023-05-04 22:22:27.000490 cvxsimulator-0.0.4/pyproject.toml
+-rw-r--r--   0        0        0     4605 1970-01-01 00:00:00.000000 cvxsimulator-0.0.4/PKG-INFO
```

### Comparing `cvxsimulator-0.0.3/LICENSE` & `cvxsimulator-0.0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `cvxsimulator-0.0.3/README.md` & `cvxsimulator-0.0.4/README.md`

 * *Files identical despite different names*

### Comparing `cvxsimulator-0.0.3/cvx/simulator/metrics.py` & `cvxsimulator-0.0.4/cvx/simulator/metrics.py`

 * *Files identical despite different names*

### Comparing `cvxsimulator-0.0.3/cvx/simulator/portfolio.py` & `cvxsimulator-0.0.4/cvx/simulator/portfolio.py`

 * *Files identical despite different names*

### Comparing `cvxsimulator-0.0.3/PKG-INFO` & `cvxsimulator-0.0.4/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cvxsimulator
-Version: 0.0.3
+Version: 0.0.4
 Summary: Simple simulator for investors
 Author: Thomas Schmelzer, and Stephen Boyd
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

