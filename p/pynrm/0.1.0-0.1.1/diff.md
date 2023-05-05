# Comparing `tmp/pynrm-0.1.0.tar.gz` & `tmp/pynrm-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pynrm-0.1.0.tar", last modified: Tue Mar 28 03:38:41 2023, max compression
+gzip compressed data, was "pynrm-0.1.1.tar", last modified: Fri May  5 17:57:57 2023, max compression
```

## Comparing `pynrm-0.1.0.tar` & `pynrm-0.1.1.tar`

### file list

```diff
@@ -1,27 +1,34 @@
-drwxr-xr-x   0 katejeon   (501) staff       (20)        0 2023-03-28 03:38:41.524283 pynrm-0.1.0/
--rw-r--r--   0 katejeon   (501) staff       (20)      294 2023-03-28 03:07:58.000000 pynrm-0.1.0/.bumpversion.cfg
--rw-r--r--   0 katejeon   (501) staff       (20)     1488 2023-03-28 02:34:48.000000 pynrm-0.1.0/CONTRIBUTING.md
--rw-r--r--   0 katejeon   (501) staff       (20)    11357 2023-02-12 21:30:45.000000 pynrm-0.1.0/LICENSE
--rw-r--r--   0 katejeon   (501) staff       (20)      406 2023-03-23 17:44:02.000000 pynrm-0.1.0/MANIFEST.in
--rw-r--r--   0 katejeon   (501) staff       (20)     2251 2023-03-28 03:27:28.000000 pynrm-0.1.0/Makefile
--rw-r--r--   0 katejeon   (501) staff       (20)      179 2023-03-28 03:38:41.523779 pynrm-0.1.0/PKG-INFO
--rw-r--r--   0 katejeon   (501) staff       (20)     1890 2023-03-28 02:34:48.000000 pynrm-0.1.0/README.md
-drwxr-xr-x   0 katejeon   (501) staff       (20)        0 2023-03-28 03:38:41.520783 pynrm-0.1.0/pynrm/
--rw-r--r--   0 katejeon   (501) staff       (20)     1211 2023-03-28 02:34:48.000000 pynrm-0.1.0/pynrm/Pedigree.py
--rw-r--r--   0 katejeon   (501) staff       (20)     5748 2023-03-28 02:34:48.000000 pynrm-0.1.0/pynrm/Simulator.py
--rw-r--r--   0 katejeon   (501) staff       (20)       22 2023-03-28 03:07:58.000000 pynrm-0.1.0/pynrm/__init__.py
--rw-r--r--   0 katejeon   (501) staff       (20)       36 2023-03-28 02:34:48.000000 pynrm-0.1.0/pynrm/__main__.py
--rw-r--r--   0 katejeon   (501) staff       (20)     1800 2023-03-28 02:34:48.000000 pynrm-0.1.0/pynrm/nrm.py
-drwxr-xr-x   0 katejeon   (501) staff       (20)        0 2023-03-28 03:38:41.523204 pynrm-0.1.0/pynrm/tests/
--rw-r--r--   0 katejeon   (501) staff       (20)      825 2023-03-28 02:34:48.000000 pynrm-0.1.0/pynrm/tests/test_nrm.py
--rw-r--r--   0 katejeon   (501) staff       (20)      896 2023-03-28 02:34:48.000000 pynrm-0.1.0/pynrm/tests/test_pedigree.py
--rw-r--r--   0 katejeon   (501) staff       (20)     2326 2023-03-28 02:34:48.000000 pynrm-0.1.0/pynrm/tests/test_simulator.py
-drwxr-xr-x   0 katejeon   (501) staff       (20)        0 2023-03-28 03:38:41.522304 pynrm-0.1.0/pynrm.egg-info/
--rw-r--r--   0 katejeon   (501) staff       (20)      179 2023-03-28 03:38:41.000000 pynrm-0.1.0/pynrm.egg-info/PKG-INFO
--rw-r--r--   0 katejeon   (501) staff       (20)      408 2023-03-28 03:38:41.000000 pynrm-0.1.0/pynrm.egg-info/SOURCES.txt
--rw-r--r--   0 katejeon   (501) staff       (20)        1 2023-03-28 03:38:41.000000 pynrm-0.1.0/pynrm.egg-info/dependency_links.txt
--rw-r--r--   0 katejeon   (501) staff       (20)       13 2023-03-28 03:38:41.000000 pynrm-0.1.0/pynrm.egg-info/requires.txt
--rw-r--r--   0 katejeon   (501) staff       (20)        1 2023-03-28 03:38:41.000000 pynrm-0.1.0/pynrm.egg-info/top_level.txt
--rw-r--r--   0 katejeon   (501) staff       (20)     2169 2023-03-28 03:07:58.000000 pynrm-0.1.0/pyproject.toml
--rw-r--r--   0 katejeon   (501) staff       (20)       38 2023-03-28 03:38:41.524492 pynrm-0.1.0/setup.cfg
--rw-r--r--   0 katejeon   (501) staff       (20)      144 2023-03-28 03:37:29.000000 pynrm-0.1.0/setup.py
+drwxr-xr-x   0 katejeon   (501) staff       (20)        0 2023-05-05 17:57:57.214803 pynrm-0.1.1/
+-rw-r--r--   0 katejeon   (501) staff       (20)      294 2023-05-05 17:28:09.000000 pynrm-0.1.1/.bumpversion.cfg
+-rw-r--r--   0 katejeon   (501) staff       (20)      694 2023-05-02 19:16:19.000000 pynrm-0.1.1/.readthedocs.yaml
+-rw-r--r--   0 katejeon   (501) staff       (20)     1488 2023-04-07 15:59:33.000000 pynrm-0.1.1/CONTRIBUTING.md
+-rw-r--r--   0 katejeon   (501) staff       (20)    11357 2023-04-07 15:59:33.000000 pynrm-0.1.1/LICENSE
+-rw-r--r--   0 katejeon   (501) staff       (20)      540 2023-05-05 17:03:35.000000 pynrm-0.1.1/MANIFEST.in
+-rw-r--r--   0 katejeon   (501) staff       (20)     2251 2023-04-07 15:59:33.000000 pynrm-0.1.1/Makefile
+-rw-r--r--   0 katejeon   (501) staff       (20)    15730 2023-05-05 17:57:57.214312 pynrm-0.1.1/PKG-INFO
+-rw-r--r--   0 katejeon   (501) staff       (20)     1938 2023-05-05 17:03:35.000000 pynrm-0.1.1/README.md
+drwxr-xr-x   0 katejeon   (501) staff       (20)        0 2023-05-05 17:57:57.207034 pynrm-0.1.1/docs/
+-rw-r--r--   0 katejeon   (501) staff       (20)      634 2023-04-06 22:27:41.000000 pynrm-0.1.1/docs/Makefile
+-rw-r--r--   0 katejeon   (501) staff       (20)     2002 2023-04-08 20:20:03.000000 pynrm-0.1.1/docs/conf.py
+-rw-r--r--   0 katejeon   (501) staff       (20)     1595 2023-04-08 20:20:03.000000 pynrm-0.1.1/docs/index.rst
+-rw-r--r--   0 katejeon   (501) staff       (20)      760 2023-04-06 22:27:41.000000 pynrm-0.1.1/docs/make.bat
+-rw-r--r--   0 katejeon   (501) staff       (20)      542 2023-04-08 20:20:03.000000 pynrm-0.1.1/docs/pynrm.rst
+drwxr-xr-x   0 katejeon   (501) staff       (20)        0 2023-05-05 17:57:57.209322 pynrm-0.1.1/pynrm/
+-rw-r--r--   0 katejeon   (501) staff       (20)     2930 2023-05-05 17:03:35.000000 pynrm-0.1.1/pynrm/Pedigree.py
+-rw-r--r--   0 katejeon   (501) staff       (20)     7676 2023-05-05 17:03:35.000000 pynrm-0.1.1/pynrm/Simulator.py
+-rw-r--r--   0 katejeon   (501) staff       (20)       22 2023-05-05 17:28:09.000000 pynrm-0.1.1/pynrm/__init__.py
+-rw-r--r--   0 katejeon   (501) staff       (20)       36 2023-05-05 00:54:10.000000 pynrm-0.1.1/pynrm/__main__.py
+-rw-r--r--   0 katejeon   (501) staff       (20)     2852 2023-05-05 17:03:35.000000 pynrm-0.1.1/pynrm/nrm.py
+drwxr-xr-x   0 katejeon   (501) staff       (20)        0 2023-05-05 17:57:57.213545 pynrm-0.1.1/pynrm/tests/
+-rw-r--r--   0 katejeon   (501) staff       (20)     1278 2023-05-05 17:03:35.000000 pynrm-0.1.1/pynrm/tests/test_nrm.py
+-rw-r--r--   0 katejeon   (501) staff       (20)     1150 2023-05-05 17:03:35.000000 pynrm-0.1.1/pynrm/tests/test_pedigree.py
+-rw-r--r--   0 katejeon   (501) staff       (20)     2433 2023-05-05 17:03:35.000000 pynrm-0.1.1/pynrm/tests/test_simulator.py
+drwxr-xr-x   0 katejeon   (501) staff       (20)        0 2023-05-05 17:57:57.211333 pynrm-0.1.1/pynrm.egg-info/
+-rw-r--r--   0 katejeon   (501) staff       (20)    15730 2023-05-05 17:57:57.000000 pynrm-0.1.1/pynrm.egg-info/PKG-INFO
+-rw-r--r--   0 katejeon   (501) staff       (20)      497 2023-05-05 17:57:57.000000 pynrm-0.1.1/pynrm.egg-info/SOURCES.txt
+-rw-r--r--   0 katejeon   (501) staff       (20)        1 2023-05-05 17:57:57.000000 pynrm-0.1.1/pynrm.egg-info/dependency_links.txt
+-rw-r--r--   0 katejeon   (501) staff       (20)      169 2023-05-05 17:57:57.000000 pynrm-0.1.1/pynrm.egg-info/requires.txt
+-rw-r--r--   0 katejeon   (501) staff       (20)        6 2023-05-05 17:57:57.000000 pynrm-0.1.1/pynrm.egg-info/top_level.txt
+-rw-r--r--   0 katejeon   (501) staff       (20)     2169 2023-05-05 17:28:09.000000 pynrm-0.1.1/pyproject.toml
+-rw-r--r--   0 katejeon   (501) staff       (20)       38 2023-05-05 17:57:57.214927 pynrm-0.1.1/setup.cfg
+-rw-r--r--   0 katejeon   (501) staff       (20)      144 2023-04-06 22:24:45.000000 pynrm-0.1.1/setup.py
```

### Comparing `pynrm-0.1.0/CONTRIBUTING.md` & `pynrm-0.1.1/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `pynrm-0.1.0/LICENSE` & `pynrm-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `pynrm-0.1.0/Makefile` & `pynrm-0.1.1/Makefile`

 * *Files identical despite different names*

### Comparing `pynrm-0.1.0/README.md` & `pynrm-0.1.1/README.md`

 * *Files 21% similar despite different names*

```diff
@@ -1,14 +1,17 @@
 # pynrm
-`pynrm` is a lightweight and extensible animal breeding simulation library for Python.
 
-[![Build Status](https://github.com/katehyerinjeon/pynrm/workflows/Build%20Status/badge.svg?branch=main)](https://github.com/katehyerinjeon/pynrm/actions?query=workflow%3A%22Build+Status%22)
+`pynrm` is a lightweight and extensible Python library for livestock breeding simulation.
+
+![Build Status](https://github.com/katehyerinjeon/pynrm/actions/workflows/build.yml/badge.svg)
+![PyPI](https://img.shields.io/pypi/v/pynrm)
 [![codecov](https://codecov.io/gh/katehyerinjeon/pynrm/branch/main/graph/badge.svg)](https://codecov.io/gh/katehyerinjeon/pynrm)
 ![GitHub](https://img.shields.io/github/license/katehyerinjeon/pynrm)
 ![GitHub issues](https://img.shields.io/github/issues/katehyerinjeon/pynrm)
+[![Docs](https://img.shields.io/readthedocs/pynrm.svg)](https://pynrm.readthedocs.io/)
 
 ## Overview
 The numerator relationship matrix describes additive genetic relationships within a population.
 Numerous evaluation-selection systems have been devised to produce populations with favorable genetic responses while maintaining moderate to low rates of inbreeding.
 `pynrm` provides a simple yet powerful simulation tool to forecast the stochastic impacts of these systems.
 One major bottleneck to running these simulations is that as the number of animals bred increases, the size of the matrix grows exponentially.
 `pynrm` efficiently solves for the numerator relationship matrix values by tracing up the pedigree for only the relevant ancestors, thereby minimizing computational overhead.
@@ -18,25 +21,24 @@
 `pynrm` is available on PyPI:
 
 ```shell
 $ pip install pyrnm
 ```
 
 ### Supported Features
-- Fine-tuned reproduction simulation with user-defined weights
+- Livestock reproduction simulations that provide fine-grained control
 ```python
-from pynrm.Pedigree import Pedigree
-from pynrm.Simulator import Simulator
+from pynrm import Pedigree, Simulator
 
 pedigree = Pedigree()
 simulator = Simulator(pedigree, 10, 100, 0.6, 1)
 
 simulator.reproduce()
 ```
 
 - Data visualization and analysis of simulation results (COMING SOON)
 
 ## Documentation
--- LINK TO OFFICIAL DOC COMING SOON --
+Official documentation is available [here](https://pynrm.readthedocs.io/).
 
 ## Contribution
 Contributions are welcome! There are many ways to contribute to this project. Get started [here](CONTRIBUTING.md).
```

### Comparing `pynrm-0.1.0/pynrm/tests/test_pedigree.py` & `pynrm-0.1.1/pynrm/tests/test_pedigree.py`

 * *Files 10% similar despite different names*

```diff
@@ -16,7 +16,14 @@
 
         self.assertEqual(self.pedigree.data.shape[1], 5, "expected 5 columns")
         self.assertEqual(self.pedigree.data[self.pedigree.data["sex"] == "M"].shape[0], 500, "expected 500 males")
         self.assertEqual(self.pedigree.data[self.pedigree.data["sex"] == "F"].shape[0], 500, "expected 500 females")
         self.assertEqual(self.pedigree.data["gen"][0], 0, "expected generation 0")
         self.assertTrue(pd.isna(self.pedigree.data["sire"][0]), "expected sire NA")
         self.assertTrue(pd.isna(self.pedigree.data["dam"][0]), "expected dam NA")
+
+    def test_get_avg_ebv(self):
+        with self.assertRaises(TypeError):
+            self.pedigree.get_avg_ebv("not int")
+
+        self.pedigree.data["ebv"] = 1.5
+        self.assertEqual(self.pedigree.get_avg_ebv(0), 1.5, "expected average EBV 1.5")
```

### Comparing `pynrm-0.1.0/pynrm/tests/test_simulator.py` & `pynrm-0.1.1/pynrm/tests/test_simulator.py`

 * *Files 4% similar despite different names*

```diff
@@ -34,17 +34,20 @@
         with self.assertRaises(ValueError):
             self.simulator.get_ebv(-1, 0)
         with self.assertRaises(ValueError):
             self.simulator.get_ebv(0, -1)
 
     def test_get_adjusted_ebv(self):
         ebv = round(self.simulator.pedigree.data.iloc[0].ebv, 3)
-        self.assertEqual(self.simulator.get_adjusted_ebv([], 0), ebv, "incorrect adjusted ebv value")
+        self.assertEqual(self.simulator.get_adjusted_ebv(0, []), ebv, "incorrect adjusted ebv value")
 
     def test_get_top_k(self):
+        with self.assertRaises(ValueError):
+            self.simulator.get_top_k([1, 2, 3], [1, 2, 3], 1)
+
         best_ebv = self.simulator.pedigree.data.iloc[[1, 2, 3]][["ebv"]].idxmax()[0]
         self.assertEqual(
             self.simulator.get_top_k([], [1, 2, 3], 0),
             [],
             "not an empty list when k = 0",
         )
         self.assertEqual(
```

### Comparing `pynrm-0.1.0/pyproject.toml` & `pynrm-0.1.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 build-backend="setuptools.build_meta"
 
 [project]
 name = "pynrm"
 authors = [{name = "Kate Jeon", email = "hj2589@columbia.edu"}]
 description="A python library for animal breeding simulation"
 readme = "README.md"
-version = "0.1.0"
+version = "0.1.1"
 requires-python = ">=3.7"
 
 dependencies = ["numpy", "pandas"]
 
 classifiers = [
     "Development Status :: 2 - Pre-Alpha",
     "Programming Language :: Python :: Implementation :: CPython",
```

