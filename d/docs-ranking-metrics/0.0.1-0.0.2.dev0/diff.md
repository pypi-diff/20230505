# Comparing `tmp/docs-ranking-metrics-0.0.1.tar.gz` & `tmp/docs-ranking-metrics-0.0.2.dev0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\docs-ranking-metrics-0.0.1.tar", last modified: Wed May  3 17:56:08 2023, max compression
+gzip compressed data, was "dist\docs-ranking-metrics-0.0.2.dev0.tar", last modified: Fri May  5 08:09:16 2023, max compression
```

## Comparing `docs-ranking-metrics-0.0.1.tar` & `docs-ranking-metrics-0.0.2.dev0.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0        0        0        0 2023-05-03 17:56:08.773610 docs-ranking-metrics-0.0.1/
--rw-rw-rw-   0        0        0     3015 2023-05-03 17:56:08.773610 docs-ranking-metrics-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0     2352 2023-05-03 17:11:25.000000 docs-ranking-metrics-0.0.1/README.md
--rw-rw-rw-   0        0        0       97 2023-05-03 09:34:56.000000 docs-ranking-metrics-0.0.1/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-05-03 17:56:08.773610 docs-ranking-metrics-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0     8944 2023-05-03 17:56:03.000000 docs-ranking-metrics-0.0.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-03 17:56:08.746607 docs-ranking-metrics-0.0.1/src/
-drwxrwxrwx   0        0        0        0 2023-05-03 17:56:08.767607 docs-ranking-metrics-0.0.1/src/docs_ranking_metrics.egg-info/
--rw-rw-rw-   0        0        0     3015 2023-05-03 17:56:08.000000 docs-ranking-metrics-0.0.1/src/docs_ranking_metrics.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      385 2023-05-03 17:56:08.000000 docs-ranking-metrics-0.0.1/src/docs_ranking_metrics.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-03 17:56:08.000000 docs-ranking-metrics-0.0.1/src/docs_ranking_metrics.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       70 2023-05-03 17:56:08.000000 docs-ranking-metrics-0.0.1/src/docs_ranking_metrics.egg-info/requires.txt
--rw-rw-rw-   0        0        0       16 2023-05-03 17:56:08.000000 docs-ranking-metrics-0.0.1/src/docs_ranking_metrics.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-05-03 17:56:08.771614 docs-ranking-metrics-0.0.1/src/ranking_metrics/
--rw-rw-rw-   0        0        0       83 2023-05-03 17:41:17.000000 docs-ranking-metrics-0.0.1/src/ranking_metrics/__init__.py
--rw-rw-rw-   0        0        0     6103 2023-05-03 09:25:56.000000 docs-ranking-metrics-0.0.1/src/ranking_metrics/evaluation_metrics.py
--rw-rw-rw-   0        0        0     7234 2023-05-03 10:49:55.000000 docs-ranking-metrics-0.0.1/src/ranking_metrics/ranking_metrics.py
+drwxrwxrwx   0        0        0        0 2023-05-05 08:09:16.727558 docs-ranking-metrics-0.0.2.dev0/
+-rw-rw-rw-   0        0        0     2373 2023-05-05 08:09:16.727558 docs-ranking-metrics-0.0.2.dev0/PKG-INFO
+-rw-rw-rw-   0        0        0     2264 2023-05-05 08:08:34.000000 docs-ranking-metrics-0.0.2.dev0/README.md
+-rw-rw-rw-   0        0        0       97 2023-05-03 09:34:56.000000 docs-ranking-metrics-0.0.2.dev0/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-05 08:09:16.728522 docs-ranking-metrics-0.0.2.dev0/setup.cfg
+-rw-rw-rw-   0        0        0     8952 2023-05-05 08:04:22.000000 docs-ranking-metrics-0.0.2.dev0/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-05 08:09:16.617872 docs-ranking-metrics-0.0.2.dev0/src/
+drwxrwxrwx   0        0        0        0 2023-05-05 08:09:16.659038 docs-ranking-metrics-0.0.2.dev0/src/docs_ranking_metrics.egg-info/
+-rw-rw-rw-   0        0        0     2373 2023-05-05 08:09:16.000000 docs-ranking-metrics-0.0.2.dev0/src/docs_ranking_metrics.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      385 2023-05-05 08:09:16.000000 docs-ranking-metrics-0.0.2.dev0/src/docs_ranking_metrics.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-05 08:09:16.000000 docs-ranking-metrics-0.0.2.dev0/src/docs_ranking_metrics.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       70 2023-05-05 08:09:16.000000 docs-ranking-metrics-0.0.2.dev0/src/docs_ranking_metrics.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       16 2023-05-05 08:09:16.000000 docs-ranking-metrics-0.0.2.dev0/src/docs_ranking_metrics.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-05 08:09:16.725555 docs-ranking-metrics-0.0.2.dev0/src/ranking_metrics/
+-rw-rw-rw-   0        0        0      135 2023-05-05 08:04:22.000000 docs-ranking-metrics-0.0.2.dev0/src/ranking_metrics/__init__.py
+-rw-rw-rw-   0        0        0     9877 2023-05-05 06:32:01.000000 docs-ranking-metrics-0.0.2.dev0/src/ranking_metrics/evaluation_metrics.py
+-rw-rw-rw-   0        0        0     7725 2023-05-05 06:37:34.000000 docs-ranking-metrics-0.0.2.dev0/src/ranking_metrics/ranking_metrics.py
```

### Comparing `docs-ranking-metrics-0.0.1/PKG-INFO` & `docs-ranking-metrics-0.0.2.dev0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: docs-ranking-metrics
-Version: 0.0.1
+Version: 0.0.2.dev0
 Summary: The package contains functions for calculating ranking metrics
 Home-page: https://github.com/betepok506/RankingMetrics
 Author: Andrey Rotanov
 Author-email: rotanov07@mail.ru
 License: UNKNOWN
 Keywords: test
 Platform: UNKNOWN
@@ -23,14 +23,21 @@
 с подсчетом метрик: 
 * Top@1;
 * Top@3;
 * Top@5;
 * Средняя позиция в выдачах (AverageLoc);
 * Оценка как часто фейковый документ выше релевантных (FDARO)
 
+
+# Установка
+Для установки пакета воспользуйтесь командой
+```
+pip install docs-ranking-metrics
+```
+
 # Пример использования
 Пример использования представлен в `examples/using_metrics.py`
 
 ```commandline
 # Объявление метрик
 metrics = [LaBSE(), Bm25()]
 # Объявление класса агрегирующего обновление метрик
@@ -63,32 +70,8 @@
     'Bm25_Top@3': 1.0, 
     'Bm25_Top@5': 1.0, 
     'LaBSE_FDARO': 0.6216, 
     'Bm25_FDARO': 1.0
 }
 ```
 
-# Загрузка пакета
-Необходимо установить все зависимости 
-
-```commandline
-pip install twine wheel
-```
-
-Для создания пакета необходимо воспользоваться командой:
-```commandline
-python3 setup.py sdist bdist_wheel
-```
-
-Загружаем пакет в PyPI
-```commandline
-python3 -m twine upload dist/*
-```
-
-# Улучшения:
-
-* Исправить подсчет метрик под документы разной релевантности
-* Внедрить модель https://huggingface.co/cross-encoder/ms-marco-MiniLM-L-6-v2
-* Придумать дополнительные метрики
-* Завернуть все в пакет
-* Написать тесты, workflows
```

### Comparing `docs-ranking-metrics-0.0.1/setup.py` & `docs-ranking-metrics-0.0.2.dev0/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -9,15 +9,15 @@
 from setuptools import setup, find_packages
 import pathlib
 import codecs
 import os.path
 
 here = pathlib.Path(__file__).parent.resolve()
 # Get the long description from the README file
-long_description = (here / "README.md").read_text(encoding="utf-8")
+long_description = (here / "README_PACKAGE.md").read_text(encoding="utf-8")
 
 
 # Arguments marked as "Required" below must be included for upload to PyPI.
 # Fields marked as "Optional" may be commented out.
 
 
 def read(rel_path):
```

### Comparing `docs-ranking-metrics-0.0.1/src/docs_ranking_metrics.egg-info/PKG-INFO` & `docs-ranking-metrics-0.0.2.dev0/src/docs_ranking_metrics.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: docs-ranking-metrics
-Version: 0.0.1
+Version: 0.0.2.dev0
 Summary: The package contains functions for calculating ranking metrics
 Home-page: https://github.com/betepok506/RankingMetrics
 Author: Andrey Rotanov
 Author-email: rotanov07@mail.ru
 License: UNKNOWN
 Keywords: test
 Platform: UNKNOWN
@@ -23,14 +23,21 @@
 с подсчетом метрик: 
 * Top@1;
 * Top@3;
 * Top@5;
 * Средняя позиция в выдачах (AverageLoc);
 * Оценка как часто фейковый документ выше релевантных (FDARO)
 
+
+# Установка
+Для установки пакета воспользуйтесь командой
+```
+pip install docs-ranking-metrics
+```
+
 # Пример использования
 Пример использования представлен в `examples/using_metrics.py`
 
 ```commandline
 # Объявление метрик
 metrics = [LaBSE(), Bm25()]
 # Объявление класса агрегирующего обновление метрик
@@ -63,32 +70,8 @@
     'Bm25_Top@3': 1.0, 
     'Bm25_Top@5': 1.0, 
     'LaBSE_FDARO': 0.6216, 
     'Bm25_FDARO': 1.0
 }
 ```
 
-# Загрузка пакета
-Необходимо установить все зависимости 
-
-```commandline
-pip install twine wheel
-```
-
-Для создания пакета необходимо воспользоваться командой:
-```commandline
-python3 setup.py sdist bdist_wheel
-```
-
-Загружаем пакет в PyPI
-```commandline
-python3 -m twine upload dist/*
-```
-
-# Улучшения:
-
-* Исправить подсчет метрик под документы разной релевантности
-* Внедрить модель https://huggingface.co/cross-encoder/ms-marco-MiniLM-L-6-v2
-* Придумать дополнительные метрики
-* Завернуть все в пакет
-* Написать тесты, workflows
```

### Comparing `docs-ranking-metrics-0.0.1/src/ranking_metrics/ranking_metrics.py` & `docs-ranking-metrics-0.0.2.dev0/src/ranking_metrics/ranking_metrics.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,203 +1,205 @@
 from rank_bm25 import BM25Okapi
+from typing import List, Dict, Tuple, Union
 from sentence_transformers import SentenceTransformer, util
-from src.metrics.evaluation_metrics import (
+from src.ranking_metrics.evaluation_metrics import (
     TopK, AverageLoc, FDARO
 )
 
+
 class Bm25:
     """Класс метрики ранжирования bm25"""
 
     def __init__(self):
         pass
 
-    def __name__(self):
+    def name(self):
         return "Bm25"
 
-    def ranking(self, query: str, sentences: list[str], labels: list[int]) -> list:
+    def ranking(self, query: str, sentences: List[str], labels: List[int]) -> List[Tuple[float, int]]:
         """
-        Функция ранжирования bm25
+        Функция ранжирования bm25. https://ru.wikipedia.org/wiki/Okapi_BM25
 
         Parameters
         ------------
         query: `str`
             Список токенов запроса
-        sentences: `list[str]`
+        sentences: `List[str]`
             Список списков токенов текстов
-        labels: `list[int]`
+        labels: `List[int]`
             Список меток текстов
 
         Returns
         ------------
-        `list`
+        `List[Tuple[float, int]]`
             Список оценок релевантности текстов
         """
         tokenized_query = self._encode(query)[0]
         tokenized_sentences = self._encode(sentences)
         bm25 = BM25Okapi(tokenized_sentences)
         scores = bm25.get_scores(tokenized_query)
 
         scores = self._sorted(scores, labels)
         return scores
 
-    def _sorted(self, scores: list[float], labels: list[int]):
+    def _sorted(self, scores: List[float], labels: List[int]) -> List[Tuple[float, int]]:
         """
         Функция сортировки оценки и лейблов
 
         Parameters
         ------------
-        scores: `list[float]`
-            Массив оценок ранка присвоенных ранкером
-        labels: `list[int]`
+        scores: `List[float]`
+            Массив оценок ранга присвоенных ранкером
+        labels: `List[int]`
             Массив меток
 
         Returns
         ------------
-        `list[list]`
+        `List[List]`
             Отсортированный список ранжируемых элементов по релевантности
         """
         return sorted([item for item in zip(scores, labels)], key=lambda x: x[0], reverse=True)
 
-    def _encode(self, sentences: str or list[str]):
+    def _encode(self, sentences: Union[str, List[str]]) -> List[List[str]]:
         """
         Функция для декодирования предложений в последовательность токенов
 
         Parameters
         ------------
-        sentences: `str, list[str]`
+        sentences: `str, List[str]`
+            Строка или массив строк для разбиения на токены
 
         Returns
         ------------
-        `list[str]` or `list[list[str]]`
+        `List[List[str]]`
             Последовательность токенов
         """
         # tokenized_sentences = self.tokenizer.encode(sentences, return_tensors="pt")
+        # TODO: Сделать более умную токенизацию
         if isinstance(sentences, str):
             sentences = [sentences]
 
         tokenized_sentences = []
         for cur_sent in sentences:
             tokenized_sentences.append(cur_sent.split(" "))
         return tokenized_sentences
 
 
 class LaBSE:
     """Класс метрики ранжирования LaBSE"""
 
-    def __init__(self):
+    def __init__(self) -> None:
         self.model = SentenceTransformer('sentence-transformers/LaBSE')
 
-    def __name__(self):
+    def name(self) -> str:
         return "LaBSE"
 
-    def ranking(self, query: str, sentences: list[str], labels: list[int]) -> list:
+    def ranking(self, query: str, sentences: List[str], labels: List[int]) -> List[Tuple[float, int]]:
         """
         Функция ранжирования LaBSE
 
         Parameters
         ------------
         query: `str`
             Строка запроса
-        sentences: `list[str]`
+        sentences: `List[str]`
             Список строк текстов
-        labels: `list[int]`
+        labels: `List[int]`
             Список меток текстов
 
         Returns
         ------------
-        `list`
+        `List[Tuple[float, int]]`
             Список оценок релевантности текстов
         """
         query = self.model.encode(query)
         embeddings = self.model.encode(sentences)
         scores = util.pytorch_cos_sim(query, embeddings).numpy()[0]
         scores = self._sorted(scores, labels)
         return scores
 
-    def _sorted(self, scores: list[str], labels: list[str]):
+    def _sorted(self, scores: List[float], labels: List[int]) -> List[Tuple[float, int]]:
         """
         Функция сортировки оценки и лейблов
 
         Parameters
         ------------
-        scores: `list[float]`
+        scores: `List[float]`
             Массив оценок ранка присвоенных ранкером
-        labels: `list[int]`
+        labels: `List[int]`
             Массив меток
 
         Returns
         ------------
-        `list[list]`
+        `List[Tuple[float, int]]`
             Отсортированный список ранжируемых элементов по релевантности
         """
         return sorted([item for item in zip(scores, labels)], key=lambda x: x[0])
 
 
 class RankingMetrics:
     """Класс аккумулирующий все метрики"""
-    FAKE_DOC_LABEL: int = 2
+    FAKE_DOC_LABEL: int = -1
 
-    def __init__(self, metrics):
+    def __init__(self, metrics) -> None:
         # Среднее место фейковых документов в финальной выдаче
         self.average_place_fake_doc = AverageLoc(metrics)
         # Количество случаев когда фейковый документ выше релевантного
         self.fake_doc_above_relevant_one = FDARO(metrics)
         # Количество случаев когда фейковый документ вошел в топ 1
         self.fake_top_k = TopK(metrics)
-        # Классы метрик для подсчета
+        # Массив метрик для подсчета
         self.metrics = metrics
 
-    def update(self, query: str, sentences: list[str], labels: list[int]):
+    def update(self, query: str, sentences: List[str], labels: List[int]) -> None:
         """
        Функция обновления всех метрик по переданным данным
 
        Parameters
        ------------
        query: `str`
            Строка запроса
-       sentences: `list[str]`
+       sentences: `List[str]`
            Список строк текстов
-       labels: `list[int]`
+       labels: `List[int]`
            Список меток текстов
-
        """
         if not isinstance(query, str):
             raise TypeError("The request must be a string!")
 
         if len(sentences) != len(labels):
-            raise "len(labels) must be equal to len(sentences)"
+            raise ValueError("len(labels) must be equal to len(sentences)")
 
         for item in sentences:
             if not isinstance(item, str):
-                raise "The sentences must be of the `list[str]` type!"
+                raise TypeError("The sentences must be of the `List[str]` type!")
 
-        for item in labels:
-            if not isinstance(item, int):
-                raise "The labels must be of the `list[int]` type!"
+        for item_label in labels:
+            if not isinstance(item_label, int):
+                raise TypeError("The labels must be of the `List[int]` type!")
 
         for cur_metric in self.metrics:
             ranking_list = cur_metric.ranking(query, sentences, labels)
-            self.fake_top_k.update(cur_metric.__name__(), ranking_list, RankingMetrics.FAKE_DOC_LABEL)
-            self.fake_doc_above_relevant_one.update(cur_metric.__name__(), ranking_list, RankingMetrics.FAKE_DOC_LABEL)
-            self.average_place_fake_doc.update(cur_metric.__name__(), ranking_list, RankingMetrics.FAKE_DOC_LABEL)
+            self.fake_top_k.update(cur_metric.name(), ranking_list, RankingMetrics.FAKE_DOC_LABEL)
+            self.fake_doc_above_relevant_one.update(cur_metric.name(), ranking_list, RankingMetrics.FAKE_DOC_LABEL)
+            self.average_place_fake_doc.update(cur_metric.name(), ranking_list, RankingMetrics.FAKE_DOC_LABEL)
 
-    def get(self):
+    def get(self) -> Dict:
         """
         Функция для получения значения всех метрик
 
         Returns
         ----------
-        `dict`
+        `Dict`
             Словарь значений метрик
         """
         result = {}
         for key_, value in self.average_place_fake_doc.get().items():
             result[key_] = value
 
         for key_, value in self.fake_top_k.get().items():
             result[key_] = value
 
         for key_, value in self.fake_doc_above_relevant_one.get().items():
             result[key_] = value
 
         return result
-
```

