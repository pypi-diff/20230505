# Comparing `tmp/aimped-0.1.39.tar.gz` & `tmp/aimped-0.1.40.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/aimped-0.1.39.tar", last modified: Mon Apr  3 15:51:41 2023, max compression
+gzip compressed data, was "aimped-0.1.40.tar", last modified: Fri May  5 13:43:49 2023, max compression
```

## Comparing `aimped-0.1.39.tar` & `aimped-0.1.40.tar`

### file list

```diff
@@ -1,46 +1,46 @@
-drwxr-xr-x   0 DataScience   (501) staff       (20)        0 2023-04-03 15:51:41.000000 aimped-0.1.39/
--rw-r--r--   0 DataScience   (501) staff       (20)     2387 2023-04-03 15:51:41.000000 aimped-0.1.39/PKG-INFO
-drwxr-xr-x   0 DataScience   (501) staff       (20)        0 2023-04-03 15:51:41.000000 aimped-0.1.39/aimped/
--rw-r--r--   0 DataScience   (501) staff       (20)      139 2023-04-03 15:51:26.000000 aimped-0.1.39/aimped/version.py
--rw-r--r--   0 DataScience   (501) staff       (20)      502 2023-04-03 13:18:42.000000 aimped-0.1.39/aimped/models.py
-drwxr-xr-x   0 DataScience   (501) staff       (20)        0 2023-04-03 15:51:41.000000 aimped-0.1.39/aimped/test/
--rw-r--r--   0 DataScience   (501) staff       (20)     1313 2023-04-03 13:18:42.000000 aimped-0.1.39/aimped/test/test_chunk_merger.py
--rw-r--r--   0 DataScience   (501) staff       (20)     3320 2023-04-03 13:18:42.000000 aimped-0.1.39/aimped/test/test_relation_pipeline.py
--rw-r--r--   0 DataScience   (501) staff       (20)      610 2023-04-03 13:18:42.000000 aimped-0.1.39/aimped/test/test_tokenizer.py
--rw-r--r--   0 DataScience   (501) staff       (20)        0 2023-04-03 13:18:42.000000 aimped-0.1.39/aimped/test/__init__.py
--rw-r--r--   0 DataScience   (501) staff       (20)     1592 2023-04-03 13:18:42.000000 aimped-0.1.39/aimped/test/test_regex_parser.py
--rw-r--r--   0 DataScience   (501) staff       (20)     5585 2023-04-03 13:18:42.000000 aimped-0.1.39/aimped/test/test_translation_pipeline.py
--rw-r--r--   0 DataScience   (501) staff       (20)     1297 2023-04-03 13:18:42.000000 aimped-0.1.39/aimped/test/test_ner_results.py
--rw-r--r--   0 DataScience   (501) staff       (20)     2748 2023-04-03 13:18:42.000000 aimped-0.1.39/aimped/test/test_assertion.py
--rw-r--r--   0 DataScience   (501) staff       (20)     1866 2023-04-03 13:18:42.000000 aimped-0.1.39/aimped/test/test_deid_pipeline.py
--rw-r--r--   0 DataScience   (501) staff       (20)      165 2023-04-03 13:18:42.000000 aimped-0.1.39/aimped/__init__.py
--rw-r--r--   0 DataScience   (501) staff       (20)     2056 2023-04-03 13:18:42.000000 aimped-0.1.39/aimped/utils.py
-drwxr-xr-x   0 DataScience   (501) staff       (20)        0 2023-04-03 15:51:41.000000 aimped-0.1.39/aimped/model/
--rw-r--r--   0 DataScience   (501) staff       (20)        0 2023-04-03 13:18:42.000000 aimped-0.1.39/aimped/model/__init__.py
--rw-r--r--   0 DataScience   (501) staff       (20)     2338 2023-04-03 13:18:42.000000 aimped-0.1.39/aimped/model/load.py
-drwxr-xr-x   0 DataScience   (501) staff       (20)        0 2023-04-03 15:51:41.000000 aimped-0.1.39/aimped/nlp/
--rw-r--r--   0 DataScience   (501) staff       (20)    19853 2023-04-03 15:23:07.000000 aimped-0.1.39/aimped/nlp/relation_visualizer.py
--rw-r--r--   0 DataScience   (501) staff       (20)     4592 2023-04-03 15:48:56.000000 aimped-0.1.39/aimped/nlp/relation.py
--rw-r--r--   0 DataScience   (501) staff       (20)     3917 2023-04-03 13:18:42.000000 aimped-0.1.39/aimped/nlp/chunker.py
--rw-r--r--   0 DataScience   (501) staff       (20)     2251 2023-04-03 13:18:42.000000 aimped-0.1.39/aimped/nlp/tools.py
--rw-r--r--   0 DataScience   (501) staff       (20)      353 2023-04-03 13:18:42.000000 aimped-0.1.39/aimped/nlp/__init__.py
--rw-r--r--   0 DataScience   (501) staff       (20)     2228 2023-04-03 13:18:42.000000 aimped-0.1.39/aimped/nlp/assertion.py
--rw-r--r--   0 DataScience   (501) staff       (20)      803 2023-04-03 13:18:42.000000 aimped-0.1.39/aimped/nlp/tokenizer.py
--rw-r--r--   0 DataScience   (501) staff       (20)     2629 2023-04-03 13:18:42.000000 aimped-0.1.39/aimped/nlp/ner_cls_report.py
--rw-r--r--   0 DataScience   (501) staff       (20)     4521 2023-04-03 13:18:42.000000 aimped-0.1.39/aimped/nlp/ner.py
--rw-r--r--   0 DataScience   (501) staff       (20)     2825 2023-04-03 13:18:42.000000 aimped-0.1.39/aimped/nlp/deid.py
--rw-r--r--   0 DataScience   (501) staff       (20)     7231 2023-04-03 13:18:42.000000 aimped-0.1.39/aimped/nlp/pipeline.py
--rw-r--r--   0 DataScience   (501) staff       (20)     4007 2023-04-03 13:18:42.000000 aimped-0.1.39/aimped/nlp/translation.py
--rw-r--r--   0 DataScience   (501) staff       (20)     3899 2023-04-03 13:18:42.000000 aimped-0.1.39/aimped/nlp/regex_parser.py
-drwxr-xr-x   0 DataScience   (501) staff       (20)        0 2023-04-03 15:51:41.000000 aimped-0.1.39/aimped/nitro/
--rw-r--r--   0 DataScience   (501) staff       (20)        0 2023-04-03 13:18:42.000000 aimped-0.1.39/aimped/nitro/__init__.py
--rw-r--r--   0 DataScience   (501) staff       (20)     1063 2023-04-03 13:18:42.000000 aimped-0.1.39/LICENSE
--rw-r--r--   0 DataScience   (501) staff       (20)     1780 2023-04-03 13:18:42.000000 aimped-0.1.39/README.md
--rw-r--r--   0 DataScience   (501) staff       (20)     1139 2023-04-03 13:18:42.000000 aimped-0.1.39/setup.py
-drwxr-xr-x   0 DataScience   (501) staff       (20)        0 2023-04-03 15:51:41.000000 aimped-0.1.39/aimped.egg-info/
--rw-r--r--   0 DataScience   (501) staff       (20)     2387 2023-04-03 15:51:40.000000 aimped-0.1.39/aimped.egg-info/PKG-INFO
--rw-r--r--   0 DataScience   (501) staff       (20)      933 2023-04-03 15:51:41.000000 aimped-0.1.39/aimped.egg-info/SOURCES.txt
--rw-r--r--   0 DataScience   (501) staff       (20)       39 2023-04-03 15:51:40.000000 aimped-0.1.39/aimped.egg-info/requires.txt
--rw-r--r--   0 DataScience   (501) staff       (20)        7 2023-04-03 15:51:40.000000 aimped-0.1.39/aimped.egg-info/top_level.txt
--rw-r--r--   0 DataScience   (501) staff       (20)        1 2023-04-03 15:51:40.000000 aimped-0.1.39/aimped.egg-info/dependency_links.txt
--rw-r--r--   0 DataScience   (501) staff       (20)      103 2023-04-03 15:51:41.000000 aimped-0.1.39/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-05 13:43:49.730806 aimped-0.1.40/
+-rw-rw-rw-   0        0        0     1063 2023-04-03 13:18:42.000000 aimped-0.1.40/LICENSE
+-rw-rw-rw-   0        0        0     2426 2023-05-05 13:43:49.731797 aimped-0.1.40/PKG-INFO
+-rw-rw-rw-   0        0        0     1780 2023-04-03 13:18:42.000000 aimped-0.1.40/README.md
+drwxrwxrwx   0        0        0        0 2023-05-05 13:43:49.656926 aimped-0.1.40/aimped/
+-rw-rw-rw-   0        0        0      165 2023-04-03 13:18:42.000000 aimped-0.1.40/aimped/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-05 13:43:49.674677 aimped-0.1.40/aimped/model/
+-rw-rw-rw-   0        0        0        0 2023-04-03 13:18:42.000000 aimped-0.1.40/aimped/model/__init__.py
+-rw-rw-rw-   0        0        0     2338 2023-04-03 13:18:42.000000 aimped-0.1.40/aimped/model/load.py
+-rw-rw-rw-   0        0        0      502 2023-04-03 13:18:42.000000 aimped-0.1.40/aimped/models.py
+drwxrwxrwx   0        0        0        0 2023-05-05 13:43:49.676546 aimped-0.1.40/aimped/nitro/
+-rw-rw-rw-   0        0        0        0 2023-04-03 13:18:42.000000 aimped-0.1.40/aimped/nitro/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-05 13:43:49.706711 aimped-0.1.40/aimped/nlp/
+-rw-rw-rw-   0        0        0      353 2023-04-03 13:18:42.000000 aimped-0.1.40/aimped/nlp/__init__.py
+-rw-rw-rw-   0        0        0     2228 2023-04-03 13:18:42.000000 aimped-0.1.40/aimped/nlp/assertion.py
+-rw-rw-rw-   0        0        0     3917 2023-04-03 13:18:42.000000 aimped-0.1.40/aimped/nlp/chunker.py
+-rw-rw-rw-   0        0        0     2825 2023-04-03 13:18:42.000000 aimped-0.1.40/aimped/nlp/deid.py
+-rw-rw-rw-   0        0        0     4521 2023-04-03 13:18:42.000000 aimped-0.1.40/aimped/nlp/ner.py
+-rw-rw-rw-   0        0        0     2629 2023-04-03 13:18:42.000000 aimped-0.1.40/aimped/nlp/ner_cls_report.py
+-rw-rw-rw-   0        0        0     7231 2023-04-03 13:18:42.000000 aimped-0.1.40/aimped/nlp/pipeline.py
+-rw-rw-rw-   0        0        0     3899 2023-04-03 13:18:42.000000 aimped-0.1.40/aimped/nlp/regex_parser.py
+-rw-rw-rw-   0        0        0     4592 2023-04-03 15:48:56.000000 aimped-0.1.40/aimped/nlp/relation.py
+-rw-rw-rw-   0        0        0    19853 2023-04-03 15:23:07.000000 aimped-0.1.40/aimped/nlp/relation_visualizer.py
+-rw-rw-rw-   0        0        0      803 2023-04-03 13:18:42.000000 aimped-0.1.40/aimped/nlp/tokenizer.py
+-rw-rw-rw-   0        0        0     2251 2023-04-03 13:18:42.000000 aimped-0.1.40/aimped/nlp/tools.py
+-rw-rw-rw-   0        0        0     4007 2023-04-03 13:18:42.000000 aimped-0.1.40/aimped/nlp/translation.py
+drwxrwxrwx   0        0        0        0 2023-05-05 13:43:49.727830 aimped-0.1.40/aimped/test/
+-rw-rw-rw-   0        0        0        0 2023-04-03 13:18:42.000000 aimped-0.1.40/aimped/test/__init__.py
+-rw-rw-rw-   0        0        0     2748 2023-04-03 13:18:42.000000 aimped-0.1.40/aimped/test/test_assertion.py
+-rw-rw-rw-   0        0        0     1313 2023-04-03 13:18:42.000000 aimped-0.1.40/aimped/test/test_chunk_merger.py
+-rw-rw-rw-   0        0        0     1866 2023-04-03 13:18:42.000000 aimped-0.1.40/aimped/test/test_deid_pipeline.py
+-rw-rw-rw-   0        0        0     1297 2023-04-03 13:18:42.000000 aimped-0.1.40/aimped/test/test_ner_results.py
+-rw-rw-rw-   0        0        0     1592 2023-04-03 13:18:42.000000 aimped-0.1.40/aimped/test/test_regex_parser.py
+-rw-rw-rw-   0        0        0     3320 2023-04-03 13:18:42.000000 aimped-0.1.40/aimped/test/test_relation_pipeline.py
+-rw-rw-rw-   0        0        0      610 2023-04-03 13:18:42.000000 aimped-0.1.40/aimped/test/test_tokenizer.py
+-rw-rw-rw-   0        0        0     5585 2023-04-03 13:18:42.000000 aimped-0.1.40/aimped/test/test_translation_pipeline.py
+-rw-rw-rw-   0        0        0     2056 2023-04-03 13:18:42.000000 aimped-0.1.40/aimped/utils.py
+-rw-rw-rw-   0        0        0      123 2023-05-05 13:43:34.000000 aimped-0.1.40/aimped/version.py
+drwxrwxrwx   0        0        0        0 2023-05-05 13:43:49.671017 aimped-0.1.40/aimped.egg-info/
+-rw-rw-rw-   0        0        0     2426 2023-05-05 13:43:49.000000 aimped-0.1.40/aimped.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      933 2023-05-05 13:43:49.000000 aimped-0.1.40/aimped.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-05 13:43:49.000000 aimped-0.1.40/aimped.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       39 2023-05-05 13:43:49.000000 aimped-0.1.40/aimped.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-05-05 13:43:49.000000 aimped-0.1.40/aimped.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      111 2023-05-05 13:43:49.734796 aimped-0.1.40/setup.cfg
+-rw-rw-rw-   0        0        0     1139 2023-04-03 13:18:42.000000 aimped-0.1.40/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `aimped-0.1.39/PKG-INFO` & `aimped-0.1.40/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,80 +1,76 @@
-Metadata-Version: 2.1
-Name: aimped
-Version: 0.1.39
-Summary: Aimped is a unique library that provides classes and functions for only exclusively business-tailored AI-based NLP models.
-Home-page: https://dev.ml-hub.nioyatechai.com/
-Author: Russell C.
-Author-email: russell@aimped.com
-Maintainer: aimped
-Maintainer-email: contact@aimped.com
-License: UNKNOWN
-Platform: UNKNOWN
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-# **aimped**
-![aimped](https://dev.ml-hub.nioyatechai.com/static/media/AimpedBirdLogo.0b3c7cc26d31afe7bd73db496acb01d1.svg)
-
-**Aimped is a unique python library that provides classes and functions for only exclusively business-tailored AI-based NLP models.**  
-
-# Installation  
-```python
-pip install aimped
-```
-
-# Usage  
-```python  
-import aimped
-print(aimped.__version__)
-```
-## Examples  
-
-### Example 1
-
-```python  
-from aimped import nlp
-
-result = nlp.sentence_tokenizer("Hi, welcome to aimped. Explore ai models.",language="english")
-print(result)
-# ['Hi, welcome to aimped.', 'Explore ai models.']
-```
-
-### Example 2
-```python  
-from aimped.nlp.tokenizer import sentence_tokenizer
-
-result = sentence_tokenizer("Hi, welcome to aimped. Explore ai models.",language="english")
-print(result)
-# ['Hi, welcome to aimped.', 'Explore ai models.']
-```
-
-### Example 3
-```python  
-from aimped.nlp.pipeline import Pipeline
-
-pipe = Pipeline(model=model, tokenizer=tokenizer, device='cpu')
-result = pipe.ner_result(
-                        text=text,
-                        sents_tokens_list=sents_tokens_list,
-                        sentences=sentences)
-print(result)
-```
-### Example 4
-```python  
-from aimped.nlp.pipeline import Pipeline
-text = """Trotz aller medizinischen Interventionen konnte der bei dem Verkehrsunfall schwer verletzte Fahrer des Fahrzeugs nicht gerettet werden."""
-
-pipe = Pipeline(model=model, tokenizer=tokenizer, device='cpu')
-result = pipe.translation_result(
-                        text=[text],
-                        source_language = "german",
-                        output_language = "english")
-print(result)
-# ['Despite all medical interventions, the driver of the vehicle who was severely injured in the traffic accident could not be saved.']
-```
-
-
+Metadata-Version: 2.1
+Name: aimped
+Version: 0.1.40
+Summary: Aimped is a unique library that provides classes and functions for only exclusively business-tailored AI-based NLP models.
+Home-page: https://dev.ml-hub.nioyatechai.com/
+Author: Russell C.
+Author-email: russell@aimped.com
+Maintainer: aimped
+Maintainer-email: contact@aimped.com
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.6
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# **aimped**
+![aimped](https://dev.ml-hub.nioyatechai.com/static/media/AimpedBirdLogo.0b3c7cc26d31afe7bd73db496acb01d1.svg)
+
+**Aimped is a unique python library that provides classes and functions for only exclusively business-tailored AI-based NLP models.**  
+
+# Installation  
+```python
+pip install aimped
+```
+
+# Usage  
+```python  
+import aimped
+print(aimped.__version__)
+```
+## Examples  
+
+### Example 1
+
+```python  
+from aimped import nlp
+
+result = nlp.sentence_tokenizer("Hi, welcome to aimped. Explore ai models.",language="english")
+print(result)
+# ['Hi, welcome to aimped.', 'Explore ai models.']
+```
+
+### Example 2
+```python  
+from aimped.nlp.tokenizer import sentence_tokenizer
+
+result = sentence_tokenizer("Hi, welcome to aimped. Explore ai models.",language="english")
+print(result)
+# ['Hi, welcome to aimped.', 'Explore ai models.']
+```
+
+### Example 3
+```python  
+from aimped.nlp.pipeline import Pipeline
+
+pipe = Pipeline(model=model, tokenizer=tokenizer, device='cpu')
+result = pipe.ner_result(
+                        text=text,
+                        sents_tokens_list=sents_tokens_list,
+                        sentences=sentences)
+print(result)
+```
+### Example 4
+```python  
+from aimped.nlp.pipeline import Pipeline
+text = """Trotz aller medizinischen Interventionen konnte der bei dem Verkehrsunfall schwer verletzte Fahrer des Fahrzeugs nicht gerettet werden."""
+
+pipe = Pipeline(model=model, tokenizer=tokenizer, device='cpu')
+result = pipe.translation_result(
+                        text=[text],
+                        source_language = "german",
+                        output_language = "english")
+print(result)
+# ['Despite all medical interventions, the driver of the vehicle who was severely injured in the traffic accident could not be saved.']
+```
```

### Comparing `aimped-0.1.39/aimped/test/test_chunk_merger.py` & `aimped-0.1.40/aimped/test/test_chunk_merger.py`

 * *Files identical despite different names*

### Comparing `aimped-0.1.39/aimped/test/test_relation_pipeline.py` & `aimped-0.1.40/aimped/test/test_relation_pipeline.py`

 * *Files identical despite different names*

### Comparing `aimped-0.1.39/aimped/test/test_tokenizer.py` & `aimped-0.1.40/aimped/test/test_tokenizer.py`

 * *Files identical despite different names*

### Comparing `aimped-0.1.39/aimped/test/test_regex_parser.py` & `aimped-0.1.40/aimped/test/test_regex_parser.py`

 * *Files identical despite different names*

### Comparing `aimped-0.1.39/aimped/test/test_translation_pipeline.py` & `aimped-0.1.40/aimped/test/test_translation_pipeline.py`

 * *Files identical despite different names*

### Comparing `aimped-0.1.39/aimped/test/test_ner_results.py` & `aimped-0.1.40/aimped/test/test_ner_results.py`

 * *Files identical despite different names*

### Comparing `aimped-0.1.39/aimped/test/test_assertion.py` & `aimped-0.1.40/aimped/test/test_assertion.py`

 * *Files identical despite different names*

### Comparing `aimped-0.1.39/aimped/test/test_deid_pipeline.py` & `aimped-0.1.40/aimped/test/test_deid_pipeline.py`

 * *Files identical despite different names*

### Comparing `aimped-0.1.39/aimped/utils.py` & `aimped-0.1.40/aimped/utils.py`

 * *Files identical despite different names*

### Comparing `aimped-0.1.39/aimped/model/load.py` & `aimped-0.1.40/aimped/model/load.py`

 * *Files identical despite different names*

### Comparing `aimped-0.1.39/aimped/nlp/relation_visualizer.py` & `aimped-0.1.40/aimped/nlp/relation_visualizer.py`

 * *Files identical despite different names*

### Comparing `aimped-0.1.39/aimped/nlp/relation.py` & `aimped-0.1.40/aimped/nlp/relation.py`

 * *Files identical despite different names*

### Comparing `aimped-0.1.39/aimped/nlp/chunker.py` & `aimped-0.1.40/aimped/nlp/chunker.py`

 * *Files identical despite different names*

### Comparing `aimped-0.1.39/aimped/nlp/tools.py` & `aimped-0.1.40/aimped/nlp/tools.py`

 * *Files identical despite different names*

### Comparing `aimped-0.1.39/aimped/nlp/assertion.py` & `aimped-0.1.40/aimped/nlp/assertion.py`

 * *Files identical despite different names*

### Comparing `aimped-0.1.39/aimped/nlp/tokenizer.py` & `aimped-0.1.40/aimped/nlp/tokenizer.py`

 * *Files identical despite different names*

### Comparing `aimped-0.1.39/aimped/nlp/ner_cls_report.py` & `aimped-0.1.40/aimped/nlp/ner_cls_report.py`

 * *Files identical despite different names*

### Comparing `aimped-0.1.39/aimped/nlp/ner.py` & `aimped-0.1.40/aimped/nlp/ner.py`

 * *Files identical despite different names*

### Comparing `aimped-0.1.39/aimped/nlp/deid.py` & `aimped-0.1.40/aimped/nlp/deid.py`

 * *Files identical despite different names*

### Comparing `aimped-0.1.39/aimped/nlp/pipeline.py` & `aimped-0.1.40/aimped/nlp/pipeline.py`

 * *Files identical despite different names*

### Comparing `aimped-0.1.39/aimped/nlp/translation.py` & `aimped-0.1.40/aimped/nlp/translation.py`

 * *Files identical despite different names*

### Comparing `aimped-0.1.39/aimped/nlp/regex_parser.py` & `aimped-0.1.40/aimped/nlp/regex_parser.py`

 * *Files identical despite different names*

### Comparing `aimped-0.1.39/LICENSE` & `aimped-0.1.40/LICENSE`

 * *Files identical despite different names*

### Comparing `aimped-0.1.39/README.md` & `aimped-0.1.40/README.md`

 * *Files identical despite different names*

### Comparing `aimped-0.1.39/setup.py` & `aimped-0.1.40/setup.py`

 * *Files identical despite different names*

### Comparing `aimped-0.1.39/aimped.egg-info/PKG-INFO` & `aimped-0.1.40/aimped.egg-info/PKG-INFO`

 * *Files 17% similar despite different names*

```diff
@@ -1,80 +1,76 @@
-Metadata-Version: 2.1
-Name: aimped
-Version: 0.1.39
-Summary: Aimped is a unique library that provides classes and functions for only exclusively business-tailored AI-based NLP models.
-Home-page: https://dev.ml-hub.nioyatechai.com/
-Author: Russell C.
-Author-email: russell@aimped.com
-Maintainer: aimped
-Maintainer-email: contact@aimped.com
-License: UNKNOWN
-Platform: UNKNOWN
-Classifier: Programming Language :: Python :: 3
-Classifier: License :: OSI Approved :: MIT License
-Classifier: Operating System :: OS Independent
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
-# **aimped**
-![aimped](https://dev.ml-hub.nioyatechai.com/static/media/AimpedBirdLogo.0b3c7cc26d31afe7bd73db496acb01d1.svg)
-
-**Aimped is a unique python library that provides classes and functions for only exclusively business-tailored AI-based NLP models.**  
-
-# Installation  
-```python
-pip install aimped
-```
-
-# Usage  
-```python  
-import aimped
-print(aimped.__version__)
-```
-## Examples  
-
-### Example 1
-
-```python  
-from aimped import nlp
-
-result = nlp.sentence_tokenizer("Hi, welcome to aimped. Explore ai models.",language="english")
-print(result)
-# ['Hi, welcome to aimped.', 'Explore ai models.']
-```
-
-### Example 2
-```python  
-from aimped.nlp.tokenizer import sentence_tokenizer
-
-result = sentence_tokenizer("Hi, welcome to aimped. Explore ai models.",language="english")
-print(result)
-# ['Hi, welcome to aimped.', 'Explore ai models.']
-```
-
-### Example 3
-```python  
-from aimped.nlp.pipeline import Pipeline
-
-pipe = Pipeline(model=model, tokenizer=tokenizer, device='cpu')
-result = pipe.ner_result(
-                        text=text,
-                        sents_tokens_list=sents_tokens_list,
-                        sentences=sentences)
-print(result)
-```
-### Example 4
-```python  
-from aimped.nlp.pipeline import Pipeline
-text = """Trotz aller medizinischen Interventionen konnte der bei dem Verkehrsunfall schwer verletzte Fahrer des Fahrzeugs nicht gerettet werden."""
-
-pipe = Pipeline(model=model, tokenizer=tokenizer, device='cpu')
-result = pipe.translation_result(
-                        text=[text],
-                        source_language = "german",
-                        output_language = "english")
-print(result)
-# ['Despite all medical interventions, the driver of the vehicle who was severely injured in the traffic accident could not be saved.']
-```
-
-
+Metadata-Version: 2.1
+Name: aimped
+Version: 0.1.40
+Summary: Aimped is a unique library that provides classes and functions for only exclusively business-tailored AI-based NLP models.
+Home-page: https://dev.ml-hub.nioyatechai.com/
+Author: Russell C.
+Author-email: russell@aimped.com
+Maintainer: aimped
+Maintainer-email: contact@aimped.com
+Classifier: Programming Language :: Python :: 3
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Requires-Python: >=3.6
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# **aimped**
+![aimped](https://dev.ml-hub.nioyatechai.com/static/media/AimpedBirdLogo.0b3c7cc26d31afe7bd73db496acb01d1.svg)
+
+**Aimped is a unique python library that provides classes and functions for only exclusively business-tailored AI-based NLP models.**  
+
+# Installation  
+```python
+pip install aimped
+```
+
+# Usage  
+```python  
+import aimped
+print(aimped.__version__)
+```
+## Examples  
+
+### Example 1
+
+```python  
+from aimped import nlp
+
+result = nlp.sentence_tokenizer("Hi, welcome to aimped. Explore ai models.",language="english")
+print(result)
+# ['Hi, welcome to aimped.', 'Explore ai models.']
+```
+
+### Example 2
+```python  
+from aimped.nlp.tokenizer import sentence_tokenizer
+
+result = sentence_tokenizer("Hi, welcome to aimped. Explore ai models.",language="english")
+print(result)
+# ['Hi, welcome to aimped.', 'Explore ai models.']
+```
+
+### Example 3
+```python  
+from aimped.nlp.pipeline import Pipeline
+
+pipe = Pipeline(model=model, tokenizer=tokenizer, device='cpu')
+result = pipe.ner_result(
+                        text=text,
+                        sents_tokens_list=sents_tokens_list,
+                        sentences=sentences)
+print(result)
+```
+### Example 4
+```python  
+from aimped.nlp.pipeline import Pipeline
+text = """Trotz aller medizinischen Interventionen konnte der bei dem Verkehrsunfall schwer verletzte Fahrer des Fahrzeugs nicht gerettet werden."""
+
+pipe = Pipeline(model=model, tokenizer=tokenizer, device='cpu')
+result = pipe.translation_result(
+                        text=[text],
+                        source_language = "german",
+                        output_language = "english")
+print(result)
+# ['Despite all medical interventions, the driver of the vehicle who was severely injured in the traffic accident could not be saved.']
+```
```

### Comparing `aimped-0.1.39/aimped.egg-info/SOURCES.txt` & `aimped-0.1.40/aimped.egg-info/SOURCES.txt`

 * *Files identical despite different names*

