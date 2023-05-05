# Comparing `tmp/docs-ranking-metrics-0.0.2.dev0.tar.gz` & `tmp/docs-ranking-metrics-0.0.2.dev1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\docs-ranking-metrics-0.0.2.dev0.tar", last modified: Fri May  5 08:09:16 2023, max compression
+gzip compressed data, was "dist\docs-ranking-metrics-0.0.2.dev1.tar", last modified: Fri May  5 08:23:36 2023, max compression
```

## Comparing `docs-ranking-metrics-0.0.2.dev0.tar` & `docs-ranking-metrics-0.0.2.dev1.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-05-05 08:09:16.727558 docs-ranking-metrics-0.0.2.dev0/
--rw-rw-rw-   0        0        0     2373 2023-05-05 08:09:16.727558 docs-ranking-metrics-0.0.2.dev0/PKG-INFO
--rw-rw-rw-   0        0        0     2264 2023-05-05 08:08:34.000000 docs-ranking-metrics-0.0.2.dev0/README.md
--rw-rw-rw-   0        0        0       97 2023-05-03 09:34:56.000000 docs-ranking-metrics-0.0.2.dev0/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-05 08:09:16.728522 docs-ranking-metrics-0.0.2.dev0/setup.cfg
--rw-rw-rw-   0        0        0     8952 2023-05-05 08:04:22.000000 docs-ranking-metrics-0.0.2.dev0/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-05 08:09:16.617872 docs-ranking-metrics-0.0.2.dev0/src/
-drwxrwxrwx   0        0        0        0 2023-05-05 08:09:16.659038 docs-ranking-metrics-0.0.2.dev0/src/docs_ranking_metrics.egg-info/
--rw-rw-rw-   0        0        0     2373 2023-05-05 08:09:16.000000 docs-ranking-metrics-0.0.2.dev0/src/docs_ranking_metrics.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      385 2023-05-05 08:09:16.000000 docs-ranking-metrics-0.0.2.dev0/src/docs_ranking_metrics.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-05 08:09:16.000000 docs-ranking-metrics-0.0.2.dev0/src/docs_ranking_metrics.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       70 2023-05-05 08:09:16.000000 docs-ranking-metrics-0.0.2.dev0/src/docs_ranking_metrics.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2023-05-05 08:09:16.000000 docs-ranking-metrics-0.0.2.dev0/src/docs_ranking_metrics.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-05-05 08:09:16.725555 docs-ranking-metrics-0.0.2.dev0/src/ranking_metrics/
--rw-rw-rw-   0        0        0      135 2023-05-05 08:04:22.000000 docs-ranking-metrics-0.0.2.dev0/src/ranking_metrics/__init__.py
--rw-rw-rw-   0        0        0     9877 2023-05-05 06:32:01.000000 docs-ranking-metrics-0.0.2.dev0/src/ranking_metrics/evaluation_metrics.py
--rw-rw-rw-   0        0        0     7725 2023-05-05 06:37:34.000000 docs-ranking-metrics-0.0.2.dev0/src/ranking_metrics/ranking_metrics.py
+drwxrwxrwx   0        0        0        0 2023-05-05 08:23:36.012423 docs-ranking-metrics-0.0.2.dev1/
+-rw-rw-rw-   0        0        0     2373 2023-05-05 08:23:36.012423 docs-ranking-metrics-0.0.2.dev1/PKG-INFO
+-rw-rw-rw-   0        0        0     2359 2023-05-05 08:22:52.000000 docs-ranking-metrics-0.0.2.dev1/README.md
+-rw-rw-rw-   0        0        0       97 2023-05-03 09:34:56.000000 docs-ranking-metrics-0.0.2.dev1/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-05 08:23:36.013421 docs-ranking-metrics-0.0.2.dev1/setup.cfg
+-rw-rw-rw-   0        0        0     8957 2023-05-05 08:23:25.000000 docs-ranking-metrics-0.0.2.dev1/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-05 08:23:35.979222 docs-ranking-metrics-0.0.2.dev1/src/
+drwxrwxrwx   0        0        0        0 2023-05-05 08:23:35.988673 docs-ranking-metrics-0.0.2.dev1/src/docs_ranking_metrics/
+-rw-rw-rw-   0        0        0      135 2023-05-05 08:19:41.000000 docs-ranking-metrics-0.0.2.dev1/src/docs_ranking_metrics/__init__.py
+-rw-rw-rw-   0        0        0     9877 2023-05-05 06:32:01.000000 docs-ranking-metrics-0.0.2.dev1/src/docs_ranking_metrics/evaluation_metrics.py
+-rw-rw-rw-   0        0        0     7706 2023-05-05 08:19:41.000000 docs-ranking-metrics-0.0.2.dev1/src/docs_ranking_metrics/ranking_metrics.py
+drwxrwxrwx   0        0        0        0 2023-05-05 08:23:36.010784 docs-ranking-metrics-0.0.2.dev1/src/docs_ranking_metrics.egg-info/
+-rw-rw-rw-   0        0        0     2373 2023-05-05 08:23:35.000000 docs-ranking-metrics-0.0.2.dev1/src/docs_ranking_metrics.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      400 2023-05-05 08:23:35.000000 docs-ranking-metrics-0.0.2.dev1/src/docs_ranking_metrics.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-05 08:23:35.000000 docs-ranking-metrics-0.0.2.dev1/src/docs_ranking_metrics.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       70 2023-05-05 08:23:35.000000 docs-ranking-metrics-0.0.2.dev1/src/docs_ranking_metrics.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       21 2023-05-05 08:23:35.000000 docs-ranking-metrics-0.0.2.dev1/src/docs_ranking_metrics.egg-info/top_level.txt
```

### Comparing `docs-ranking-metrics-0.0.2.dev0/PKG-INFO` & `docs-ranking-metrics-0.0.2.dev1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: docs-ranking-metrics
-Version: 0.0.2.dev0
+Version: 0.0.2.dev1
 Summary: The package contains functions for calculating ranking metrics
 Home-page: https://github.com/betepok506/RankingMetrics
 Author: Andrey Rotanov
 Author-email: rotanov07@mail.ru
 License: UNKNOWN
 Keywords: test
 Platform: UNKNOWN
```

### Comparing `docs-ranking-metrics-0.0.2.dev0/README.md` & `docs-ranking-metrics-0.0.2.dev1/README.md`

 * *Files 3% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 
 Далее необходимо установить все зависимости:
 
 ```commandline
 pip install twine wheel
 ```
 
-Для создания пакета необходимо воспользоваться командой:
+Для создания пакета необходимо воспользоваться командой (**перед этим удалите все старые генерации пакетов**):
 ```commandline
 python3 setup.py sdist bdist_wheel
 ```
 
 ## Загрузка пакета в PyPI
 Для загрузки пакета необходимо воспользоваться командой:
```

### Comparing `docs-ranking-metrics-0.0.2.dev0/setup.py` & `docs-ranking-metrics-0.0.2.dev1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -57,15 +57,15 @@
     name="docs-ranking-metrics",  # Required
     # Versions should comply with PEP 440:
     # https://www.python.org/dev/peps/pep-0440/
     #
     # For a discussion on single-sourcing the version across setup.py and the
     # project code, see
     # https://packaging.python.org/guides/single-sourcing-package-version/
-    version=get_version("src/ranking_metrics/__init__.py"),  # Required
+    version=get_version("src/docs_ranking_metrics/__init__.py"),  # Required
     # This is a one-line description or tagline of what your project does. This
     # corresponds to the "Summary" metadata field:
     # https://packaging.python.org/specifications/core-metadata/#summary
     description="The package contains functions for calculating ranking metrics",  # Optional
     # This is an optional longer description of your project that represents
     # the body of text which users will see when they visit PyPI.
     #
```

### Comparing `docs-ranking-metrics-0.0.2.dev0/src/docs_ranking_metrics.egg-info/PKG-INFO` & `docs-ranking-metrics-0.0.2.dev1/src/docs_ranking_metrics.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: docs-ranking-metrics
-Version: 0.0.2.dev0
+Version: 0.0.2.dev1
 Summary: The package contains functions for calculating ranking metrics
 Home-page: https://github.com/betepok506/RankingMetrics
 Author: Andrey Rotanov
 Author-email: rotanov07@mail.ru
 License: UNKNOWN
 Keywords: test
 Platform: UNKNOWN
```

### Comparing `docs-ranking-metrics-0.0.2.dev0/src/ranking_metrics/evaluation_metrics.py` & `docs-ranking-metrics-0.0.2.dev1/src/docs_ranking_metrics/evaluation_metrics.py`

 * *Files identical despite different names*

### Comparing `docs-ranking-metrics-0.0.2.dev0/src/ranking_metrics/ranking_metrics.py` & `docs-ranking-metrics-0.0.2.dev1/src/docs_ranking_metrics/ranking_metrics.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from rank_bm25 import BM25Okapi
 from typing import List, Dict, Tuple, Union
 from sentence_transformers import SentenceTransformer, util
-from src.ranking_metrics.evaluation_metrics import (
+from .evaluation_metrics import (
     TopK, AverageLoc, FDARO
 )
 
 
 class Bm25:
     """Класс метрики ранжирования bm25"""
```

