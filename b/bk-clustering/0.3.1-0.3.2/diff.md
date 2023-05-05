# Comparing `tmp/bk_clustering-0.3.1.tar.gz` & `tmp/bk_clustering-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "bk_clustering-0.3.1.tar", max compression
+gzip compressed data, was "bk_clustering-0.3.2.tar", max compression
```

## Comparing `bk_clustering-0.3.1.tar` & `bk_clustering-0.3.2.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0     3589 2023-04-27 10:56:15.518241 bk_clustering-0.3.1/README.md
--rw-r--r--   0        0        0       40 2023-04-08 23:59:03.211844 bk_clustering-0.3.1/bk_clustering/__init__.py
--rw-r--r--   0        0        0    33769 2023-03-25 12:39:17.568753 bk_clustering-0.3.1/bk_clustering/_hierarchy.pyx
--rw-r--r--   0        0        0     9283 2023-04-25 19:13:21.122903 bk_clustering-0.3.1/bk_clustering/main.py
--rw-r--r--   0        0        0     3776 2023-04-27 10:39:46.156891 bk_clustering-0.3.1/bk_clustering/run_batch.py
--rw-r--r--   0        0        0        1 2023-04-24 00:00:09.354511 bk_clustering-0.3.1/bk_clustering/utilities/__init__.py
--rw-r--r--   0        0        0     2012 2023-04-08 23:21:19.153823 bk_clustering-0.3.1/bk_clustering/utilities/calculation_utilities.py
--rw-r--r--   0        0        0     5155 2023-04-27 10:47:08.290038 bk_clustering-0.3.1/bk_clustering/utilities/cluster_calculations.py
--rw-r--r--   0        0        0     6955 2023-03-30 17:31:18.984431 bk_clustering-0.3.1/bk_clustering/utilities/density_peak.py
--rw-r--r--   0        0        0     3843 2023-04-25 19:11:53.211146 bk_clustering-0.3.1/bk_clustering/utilities/load_save.py
--rw-r--r--   0        0        0    24666 2023-04-25 19:11:53.211146 bk_clustering-0.3.1/bk_clustering/utilities/method_comparison.py
--rw-r--r--   0        0        0     8278 2023-04-24 00:00:09.354511 bk_clustering-0.3.1/bk_clustering/utilities/metrics.py
--rw-r--r--   0        0        0     4511 2023-04-25 19:11:53.211146 bk_clustering-0.3.1/bk_clustering/utilities/plot_utilities.py
--rw-r--r--   0        0        0      527 2023-04-25 19:11:53.211146 bk_clustering-0.3.1/bk_clustering/utilities/postprocessing.py
--rw-r--r--   0        0        0     2607 2023-04-24 00:00:09.354511 bk_clustering-0.3.1/bk_clustering/utilities/preprocessing.py
--rw-r--r--   0        0        0    13106 2023-04-25 19:02:17.088220 bk_clustering-0.3.1/bk_clustering/utilities/tree_traversal.py
--rw-r--r--   0        0        0      472 2023-04-27 10:59:16.883400 bk_clustering-0.3.1/pyproject.toml
--rw-r--r--   0        0        0     4161 1970-01-01 00:00:00.000000 bk_clustering-0.3.1/PKG-INFO
+-rw-r--r--   0        0        0     3589 2023-04-27 11:12:01.555363 bk_clustering-0.3.2/README.md
+-rw-r--r--   0        0        0       40 2023-04-08 23:59:03.211844 bk_clustering-0.3.2/bk_clustering/__init__.py
+-rw-r--r--   0        0        0    33769 2023-03-25 12:39:17.568753 bk_clustering-0.3.2/bk_clustering/_hierarchy.pyx
+-rw-r--r--   0        0        0     9283 2023-04-25 19:13:21.122903 bk_clustering-0.3.2/bk_clustering/main.py
+-rw-r--r--   0        0        0     3776 2023-04-27 10:39:46.156891 bk_clustering-0.3.2/bk_clustering/run_batch.py
+-rw-r--r--   0        0        0        1 2023-04-24 00:00:09.354511 bk_clustering-0.3.2/bk_clustering/utilities/__init__.py
+-rw-r--r--   0        0        0     2012 2023-04-08 23:21:19.153823 bk_clustering-0.3.2/bk_clustering/utilities/calculation_utilities.py
+-rw-r--r--   0        0        0     5155 2023-04-27 10:47:08.290038 bk_clustering-0.3.2/bk_clustering/utilities/cluster_calculations.py
+-rw-r--r--   0        0        0     6955 2023-03-30 17:31:18.984431 bk_clustering-0.3.2/bk_clustering/utilities/density_peak.py
+-rw-r--r--   0        0        0     3843 2023-04-25 19:11:53.211146 bk_clustering-0.3.2/bk_clustering/utilities/load_save.py
+-rw-r--r--   0        0        0    24666 2023-04-25 19:11:53.211146 bk_clustering-0.3.2/bk_clustering/utilities/method_comparison.py
+-rw-r--r--   0        0        0     8278 2023-04-24 00:00:09.354511 bk_clustering-0.3.2/bk_clustering/utilities/metrics.py
+-rw-r--r--   0        0        0     4511 2023-04-25 19:11:53.211146 bk_clustering-0.3.2/bk_clustering/utilities/plot_utilities.py
+-rw-r--r--   0        0        0      527 2023-04-25 19:11:53.211146 bk_clustering-0.3.2/bk_clustering/utilities/postprocessing.py
+-rw-r--r--   0        0        0     2607 2023-04-24 00:00:09.354511 bk_clustering-0.3.2/bk_clustering/utilities/preprocessing.py
+-rw-r--r--   0        0        0    13106 2023-04-25 19:02:17.088220 bk_clustering-0.3.2/bk_clustering/utilities/tree_traversal.py
+-rw-r--r--   0        0        0      491 2023-05-05 21:10:26.682753 bk_clustering-0.3.2/pyproject.toml
+-rw-r--r--   0        0        0     4201 1970-01-01 00:00:00.000000 bk_clustering-0.3.2/PKG-INFO
```

### Comparing `bk_clustering-0.3.1/README.md` & `bk_clustering-0.3.2/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-![Logo](https://github.com/IvanReznikov/bk_clustering/blob/main/docs/images/logo_white.png?raw=true)
+![Logo](https://github.com/IvanReznikov/bk_clustering/blob/main/docs/images/logo_black.png?raw=true)
 # Burj Khalifa Clustering
 The `bk_clustering` package is a Python realization of the Burj Khalifa clustering method.
 The Burj Khalifa method can be considered as Agglomerative clustering on steroids: great quality with no parameters required!
 
 The idea is to automatically detect solid clusters, based on the dendrogram. Read more in the publication section.
 
 ## Installation
```

### Comparing `bk_clustering-0.3.1/bk_clustering/_hierarchy.pyx` & `bk_clustering-0.3.2/bk_clustering/_hierarchy.pyx`

 * *Files identical despite different names*

### Comparing `bk_clustering-0.3.1/bk_clustering/main.py` & `bk_clustering-0.3.2/bk_clustering/main.py`

 * *Files identical despite different names*

### Comparing `bk_clustering-0.3.1/bk_clustering/run_batch.py` & `bk_clustering-0.3.2/bk_clustering/run_batch.py`

 * *Files identical despite different names*

### Comparing `bk_clustering-0.3.1/bk_clustering/utilities/calculation_utilities.py` & `bk_clustering-0.3.2/bk_clustering/utilities/calculation_utilities.py`

 * *Files identical despite different names*

### Comparing `bk_clustering-0.3.1/bk_clustering/utilities/cluster_calculations.py` & `bk_clustering-0.3.2/bk_clustering/utilities/cluster_calculations.py`

 * *Files identical despite different names*

### Comparing `bk_clustering-0.3.1/bk_clustering/utilities/density_peak.py` & `bk_clustering-0.3.2/bk_clustering/utilities/density_peak.py`

 * *Files identical despite different names*

### Comparing `bk_clustering-0.3.1/bk_clustering/utilities/load_save.py` & `bk_clustering-0.3.2/bk_clustering/utilities/load_save.py`

 * *Files identical despite different names*

### Comparing `bk_clustering-0.3.1/bk_clustering/utilities/method_comparison.py` & `bk_clustering-0.3.2/bk_clustering/utilities/method_comparison.py`

 * *Files identical despite different names*

### Comparing `bk_clustering-0.3.1/bk_clustering/utilities/metrics.py` & `bk_clustering-0.3.2/bk_clustering/utilities/metrics.py`

 * *Files identical despite different names*

### Comparing `bk_clustering-0.3.1/bk_clustering/utilities/plot_utilities.py` & `bk_clustering-0.3.2/bk_clustering/utilities/plot_utilities.py`

 * *Files identical despite different names*

### Comparing `bk_clustering-0.3.1/bk_clustering/utilities/postprocessing.py` & `bk_clustering-0.3.2/bk_clustering/utilities/postprocessing.py`

 * *Files identical despite different names*

### Comparing `bk_clustering-0.3.1/bk_clustering/utilities/preprocessing.py` & `bk_clustering-0.3.2/bk_clustering/utilities/preprocessing.py`

 * *Files identical despite different names*

### Comparing `bk_clustering-0.3.1/bk_clustering/utilities/tree_traversal.py` & `bk_clustering-0.3.2/bk_clustering/utilities/tree_traversal.py`

 * *Files identical despite different names*

### Comparing `bk_clustering-0.3.1/PKG-INFO` & `bk_clustering-0.3.2/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,24 +1,25 @@
 Metadata-Version: 2.1
 Name: bk-clustering
-Version: 0.3.1
+Version: 0.3.2
 Summary: The package is the implementation of the Burj Khalifa clustering algorithm
 Author: Ivan Reznikov
 Author-email: ivanreznikov@gmail.com
 Requires-Python: >=3.10,<3.12
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: anytree (>=2.8.0,<3.0.0)
 Requires-Dist: arff (>=0.9,<0.10)
 Requires-Dist: numpy (==1.23.5)
 Requires-Dist: scikit-learn (>=1.2.2,<2.0.0)
 Requires-Dist: scipy (>=1.10.1,<2.0.0)
 Description-Content-Type: text/markdown
 
-![Logo](https://github.com/IvanReznikov/bk_clustering/blob/main/docs/images/logo_white.png?raw=true)
+![Logo](https://github.com/IvanReznikov/bk_clustering/blob/main/docs/images/logo_black.png?raw=true)
 # Burj Khalifa Clustering
 The `bk_clustering` package is a Python realization of the Burj Khalifa clustering method.
 The Burj Khalifa method can be considered as Agglomerative clustering on steroids: great quality with no parameters required!
 
 The idea is to automatically detect solid clusters, based on the dendrogram. Read more in the publication section.
 
 ## Installation
```

