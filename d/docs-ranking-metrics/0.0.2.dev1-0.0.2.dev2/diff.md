# Comparing `tmp/docs-ranking-metrics-0.0.2.dev1.tar.gz` & `tmp/docs-ranking-metrics-0.0.2.dev2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\docs-ranking-metrics-0.0.2.dev1.tar", last modified: Fri May  5 08:23:36 2023, max compression
+gzip compressed data, was "dist\docs-ranking-metrics-0.0.2.dev2.tar", last modified: Fri May  5 08:41:42 2023, max compression
```

## Comparing `docs-ranking-metrics-0.0.2.dev1.tar` & `docs-ranking-metrics-0.0.2.dev2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-05-05 08:23:36.012423 docs-ranking-metrics-0.0.2.dev1/
--rw-rw-rw-   0        0        0     2373 2023-05-05 08:23:36.012423 docs-ranking-metrics-0.0.2.dev1/PKG-INFO
--rw-rw-rw-   0        0        0     2359 2023-05-05 08:22:52.000000 docs-ranking-metrics-0.0.2.dev1/README.md
--rw-rw-rw-   0        0        0       97 2023-05-03 09:34:56.000000 docs-ranking-metrics-0.0.2.dev1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-05 08:23:36.013421 docs-ranking-metrics-0.0.2.dev1/setup.cfg
--rw-rw-rw-   0        0        0     8957 2023-05-05 08:23:25.000000 docs-ranking-metrics-0.0.2.dev1/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-05 08:23:35.979222 docs-ranking-metrics-0.0.2.dev1/src/
-drwxrwxrwx   0        0        0        0 2023-05-05 08:23:35.988673 docs-ranking-metrics-0.0.2.dev1/src/docs_ranking_metrics/
--rw-rw-rw-   0        0        0      135 2023-05-05 08:19:41.000000 docs-ranking-metrics-0.0.2.dev1/src/docs_ranking_metrics/__init__.py
--rw-rw-rw-   0        0        0     9877 2023-05-05 06:32:01.000000 docs-ranking-metrics-0.0.2.dev1/src/docs_ranking_metrics/evaluation_metrics.py
--rw-rw-rw-   0        0        0     7706 2023-05-05 08:19:41.000000 docs-ranking-metrics-0.0.2.dev1/src/docs_ranking_metrics/ranking_metrics.py
-drwxrwxrwx   0        0        0        0 2023-05-05 08:23:36.010784 docs-ranking-metrics-0.0.2.dev1/src/docs_ranking_metrics.egg-info/
--rw-rw-rw-   0        0        0     2373 2023-05-05 08:23:35.000000 docs-ranking-metrics-0.0.2.dev1/src/docs_ranking_metrics.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      400 2023-05-05 08:23:35.000000 docs-ranking-metrics-0.0.2.dev1/src/docs_ranking_metrics.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-05 08:23:35.000000 docs-ranking-metrics-0.0.2.dev1/src/docs_ranking_metrics.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       70 2023-05-05 08:23:35.000000 docs-ranking-metrics-0.0.2.dev1/src/docs_ranking_metrics.egg-info/requires.txt
--rw-rw-rw-   0        0        0       21 2023-05-05 08:23:35.000000 docs-ranking-metrics-0.0.2.dev1/src/docs_ranking_metrics.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-05 08:41:42.357390 docs-ranking-metrics-0.0.2.dev2/
+-rw-rw-rw-   0        0        0     2373 2023-05-05 08:41:42.356860 docs-ranking-metrics-0.0.2.dev2/PKG-INFO
+-rw-rw-rw-   0        0        0     2359 2023-05-05 08:22:52.000000 docs-ranking-metrics-0.0.2.dev2/README.md
+-rw-rw-rw-   0        0        0       97 2023-05-03 09:34:56.000000 docs-ranking-metrics-0.0.2.dev2/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-05 08:41:42.357390 docs-ranking-metrics-0.0.2.dev2/setup.cfg
+-rw-rw-rw-   0        0        0     8957 2023-05-05 08:23:25.000000 docs-ranking-metrics-0.0.2.dev2/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-05 08:41:42.327684 docs-ranking-metrics-0.0.2.dev2/src/
+drwxrwxrwx   0        0        0        0 2023-05-05 08:41:42.337018 docs-ranking-metrics-0.0.2.dev2/src/docs_ranking_metrics/
+-rw-rw-rw-   0        0        0      135 2023-05-05 08:41:36.000000 docs-ranking-metrics-0.0.2.dev2/src/docs_ranking_metrics/__init__.py
+-rw-rw-rw-   0        0        0     9860 2023-05-05 08:41:07.000000 docs-ranking-metrics-0.0.2.dev2/src/docs_ranking_metrics/evaluation_metrics.py
+-rw-rw-rw-   0        0        0     7706 2023-05-05 08:19:41.000000 docs-ranking-metrics-0.0.2.dev2/src/docs_ranking_metrics/ranking_metrics.py
+drwxrwxrwx   0        0        0        0 2023-05-05 08:41:42.355277 docs-ranking-metrics-0.0.2.dev2/src/docs_ranking_metrics.egg-info/
+-rw-rw-rw-   0        0        0     2373 2023-05-05 08:41:42.000000 docs-ranking-metrics-0.0.2.dev2/src/docs_ranking_metrics.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      400 2023-05-05 08:41:42.000000 docs-ranking-metrics-0.0.2.dev2/src/docs_ranking_metrics.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-05 08:41:42.000000 docs-ranking-metrics-0.0.2.dev2/src/docs_ranking_metrics.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       76 2023-05-05 08:41:42.000000 docs-ranking-metrics-0.0.2.dev2/src/docs_ranking_metrics.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       21 2023-05-05 08:41:42.000000 docs-ranking-metrics-0.0.2.dev2/src/docs_ranking_metrics.egg-info/top_level.txt
```

### Comparing `docs-ranking-metrics-0.0.2.dev1/PKG-INFO` & `docs-ranking-metrics-0.0.2.dev2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: docs-ranking-metrics
-Version: 0.0.2.dev1
+Version: 0.0.2.dev2
 Summary: The package contains functions for calculating ranking metrics
 Home-page: https://github.com/betepok506/RankingMetrics
 Author: Andrey Rotanov
 Author-email: rotanov07@mail.ru
 License: UNKNOWN
 Keywords: test
 Platform: UNKNOWN
```

### Comparing `docs-ranking-metrics-0.0.2.dev1/README.md` & `docs-ranking-metrics-0.0.2.dev2/README.md`

 * *Files identical despite different names*

### Comparing `docs-ranking-metrics-0.0.2.dev1/setup.py` & `docs-ranking-metrics-0.0.2.dev2/setup.py`

 * *Files identical despite different names*

### Comparing `docs-ranking-metrics-0.0.2.dev1/src/docs_ranking_metrics/evaluation_metrics.py` & `docs-ranking-metrics-0.0.2.dev2/src/docs_ranking_metrics/evaluation_metrics.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 from typing import List, Union, Tuple, Dict
-
+import numpy as np
 
 class TopK:
     TOP1 = 1
     TOP3 = 3
     TOP5 = 5
 
     def __init__(self, ranking_metrics: List) -> None:
@@ -234,11 +234,11 @@
             if not isinstance(label, int):
                 raise TypeError("The tags of fake documents must be 'int'!")
 
     if not isinstance(ranking_list, list):
         raise TypeError("The list of ranked elements should be of type 'list'!")
     else:
         for item in ranking_list:
-            if not (isinstance(item, tuple) or isinstance(item, list)) or \
-                    not (isinstance(item[0], float) or isinstance(item[0], int)) or not isinstance(item[1], int) or \
+            if not isinstance(item, (tuple, list)) or \
+                    not isinstance(item[0], (np.floating, float)) or not isinstance(item[1], int) or \
                     len(item) != 2:
                 raise TypeError("The list of ranked elements should contain pairs of elements: rating, label")
```

### Comparing `docs-ranking-metrics-0.0.2.dev1/src/docs_ranking_metrics/ranking_metrics.py` & `docs-ranking-metrics-0.0.2.dev2/src/docs_ranking_metrics/ranking_metrics.py`

 * *Files identical despite different names*

### Comparing `docs-ranking-metrics-0.0.2.dev1/src/docs_ranking_metrics.egg-info/PKG-INFO` & `docs-ranking-metrics-0.0.2.dev2/src/docs_ranking_metrics.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: docs-ranking-metrics
-Version: 0.0.2.dev1
+Version: 0.0.2.dev2
 Summary: The package contains functions for calculating ranking metrics
 Home-page: https://github.com/betepok506/RankingMetrics
 Author: Andrey Rotanov
 Author-email: rotanov07@mail.ru
 License: UNKNOWN
 Keywords: test
 Platform: UNKNOWN
```

