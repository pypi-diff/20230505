# Comparing `tmp/cvxsimulator-0.1.0.tar.gz` & `tmp/cvxsimulator-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cvxsimulator-0.1.0.tar", max compression
+gzip compressed data, was "cvxsimulator-0.1.1.tar", max compression
```

## Comparing `cvxsimulator-0.1.0.tar` & `cvxsimulator-0.1.1.tar`

### file list

```diff
@@ -1,8 +1,8 @@
--rw-r--r--   0        0        0     1102 2023-05-04 23:34:01.985417 cvxsimulator-0.1.0/LICENSE
--rw-r--r--   0        0        0     4115 2023-05-04 23:34:01.985417 cvxsimulator-0.1.0/README.md
--rw-r--r--   0        0        0        0 2023-05-04 23:34:02.017417 cvxsimulator-0.1.0/cvx/simulator/__init__.py
--rw-r--r--   0        0        0     1163 2023-05-04 23:34:02.017417 cvxsimulator-0.1.0/cvx/simulator/metrics.py
--rw-r--r--   0        0        0     4917 2023-05-04 23:34:02.017417 cvxsimulator-0.1.0/cvx/simulator/portfolio.py
--rw-r--r--   0        0        0      464 2023-05-04 23:34:02.017417 cvxsimulator-0.1.0/cvx/simulator/trading_costs.py
--rw-r--r--   0        0        0      491 2023-05-04 23:34:25.285842 cvxsimulator-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     4584 1970-01-01 00:00:00.000000 cvxsimulator-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1102 2023-05-05 00:01:58.403087 cvxsimulator-0.1.1/LICENSE
+-rw-r--r--   0        0        0     4115 2023-05-05 00:01:58.403087 cvxsimulator-0.1.1/README.md
+-rw-r--r--   0        0        0        0 2023-05-05 00:01:58.431087 cvxsimulator-0.1.1/cvx/simulator/__init__.py
+-rw-r--r--   0        0        0     1163 2023-05-05 00:01:58.431087 cvxsimulator-0.1.1/cvx/simulator/metrics.py
+-rw-r--r--   0        0        0     4917 2023-05-05 00:01:58.431087 cvxsimulator-0.1.1/cvx/simulator/portfolio.py
+-rw-r--r--   0        0        0      464 2023-05-05 00:01:58.431087 cvxsimulator-0.1.1/cvx/simulator/trading_costs.py
+-rw-r--r--   0        0        0      491 2023-05-05 00:02:22.358812 cvxsimulator-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     4584 1970-01-01 00:00:00.000000 cvxsimulator-0.1.1/PKG-INFO
```

### Comparing `cvxsimulator-0.1.0/LICENSE` & `cvxsimulator-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `cvxsimulator-0.1.0/README.md` & `cvxsimulator-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `cvxsimulator-0.1.0/cvx/simulator/metrics.py` & `cvxsimulator-0.1.1/cvx/simulator/metrics.py`

 * *Files identical despite different names*

### Comparing `cvxsimulator-0.1.0/cvx/simulator/portfolio.py` & `cvxsimulator-0.1.1/cvx/simulator/portfolio.py`

 * *Files identical despite different names*

### Comparing `cvxsimulator-0.1.0/PKG-INFO` & `cvxsimulator-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cvxsimulator
-Version: 0.1.0
+Version: 0.1.1
 Summary: Simple simulator for investors
 Author: Thomas Schmelzer
 Requires-Python: >=3.9,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
```

