# Comparing `tmp/cogsgpt-1.0.1.tar.gz` & `tmp/cogsgpt-1.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cogsgpt-1.0.1.tar", last modified: Fri May  5 05:10:46 2023, max compression
+gzip compressed data, was "cogsgpt-1.0.2.tar", last modified: Fri May  5 05:55:00 2023, max compression
```

## Comparing `cogsgpt-1.0.1.tar` & `cogsgpt-1.0.2.tar`

### file list

```diff
@@ -1,54 +1,54 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 05:10:46.781779 cogsgpt-1.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-05-05 05:10:26.000000 cogsgpt-1.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-05 05:10:26.000000 cogsgpt-1.0.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     7519 2023-05-05 05:10:46.781779 cogsgpt-1.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5776 2023-05-05 05:10:26.000000 cogsgpt-1.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 05:10:46.773779 cogsgpt-1.0.1/cogsgpt/
--rw-r--r--   0 runner    (1001) docker     (123)      154 2023-05-05 05:10:26.000000 cogsgpt-1.0.1/cogsgpt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14467 2023-05-05 05:10:26.000000 cogsgpt-1.0.1/cogsgpt/awesome_chat.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 05:10:46.773779 cogsgpt-1.0.1/cogsgpt/cogsmodel/
--rw-r--r--   0 runner    (1001) docker     (123)       92 2023-05-05 05:10:26.000000 cogsgpt-1.0.1/cogsgpt/cogsmodel/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      202 2023-05-05 05:10:26.000000 cogsgpt-1.0.1/cogsgpt/cogsmodel/base_model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 05:10:46.777778 cogsgpt-1.0.1/cogsgpt/cogsmodel/cv/
--rw-r--r--   0 runner    (1001) docker     (123)     1058 2023-05-05 05:10:26.000000 cogsgpt-1.0.1/cogsgpt/cogsmodel/cv/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1869 2023-05-05 05:10:26.000000 cogsgpt-1.0.1/cogsgpt/cogsmodel/cv/background_remover.py
--rw-r--r--   0 runner    (1001) docker     (123)     5601 2023-05-05 05:10:26.000000 cogsgpt-1.0.1/cogsgpt/cogsmodel/cv/form_recognizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     7020 2023-05-05 05:10:26.000000 cogsgpt-1.0.1/cogsgpt/cogsmodel/cv/image_analysis_v3.py
--rw-r--r--   0 runner    (1001) docker     (123)     6544 2023-05-05 05:10:26.000000 cogsgpt-1.0.1/cogsgpt/cogsmodel/cv/image_analysis_v4.py
--rw-r--r--   0 runner    (1001) docker     (123)     2581 2023-05-05 05:10:26.000000 cogsgpt-1.0.1/cogsgpt/cogsmodel/cv/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 05:10:46.777778 cogsgpt-1.0.1/cogsgpt/cogsmodel/nlp/
--rw-r--r--   0 runner    (1001) docker     (123)      599 2023-05-05 05:10:26.000000 cogsgpt-1.0.1/cogsgpt/cogsmodel/nlp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3504 2023-05-05 05:10:26.000000 cogsgpt-1.0.1/cogsgpt/cogsmodel/nlp/text_analysis.py
--rw-r--r--   0 runner    (1001) docker     (123)     1823 2023-05-05 05:10:26.000000 cogsgpt-1.0.1/cogsgpt/cogsmodel/nlp/text_generation.py
--rw-r--r--   0 runner    (1001) docker     (123)     2219 2023-05-05 05:10:26.000000 cogsgpt-1.0.1/cogsgpt/cogsmodel/nlp/text_summarize.py
--rw-r--r--   0 runner    (1001) docker     (123)     1710 2023-05-05 05:10:26.000000 cogsgpt-1.0.1/cogsgpt/cogsmodel/nlp/text_translation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 05:10:46.777778 cogsgpt-1.0.1/cogsgpt/cogsmodel/speech/
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-05-05 05:10:26.000000 cogsgpt-1.0.1/cogsgpt/cogsmodel/speech/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3926 2023-05-05 05:10:26.000000 cogsgpt-1.0.1/cogsgpt/cogsmodel/speech/speech.py
--rw-r--r--   0 runner    (1001) docker     (123)     2835 2023-05-05 05:10:26.000000 cogsgpt-1.0.1/cogsgpt/llm.py
--rw-r--r--   0 runner    (1001) docker     (123)      460 2023-05-05 05:10:26.000000 cogsgpt-1.0.1/cogsgpt/logger.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 05:10:46.777778 cogsgpt-1.0.1/cogsgpt/metas/
--rw-r--r--   0 runner    (1001) docker     (123)      316 2023-05-05 05:10:26.000000 cogsgpt-1.0.1/cogsgpt/metas/generate_response_presteps.json
--rw-r--r--   0 runner    (1001) docker     (123)      955 2023-05-05 05:10:26.000000 cogsgpt-1.0.1/cogsgpt/metas/parse_task_presteps.json
--rw-r--r--   0 runner    (1001) docker     (123)     2183 2023-05-05 05:10:26.000000 cogsgpt-1.0.1/cogsgpt/metas/prompts.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     4718 2023-05-05 05:10:26.000000 cogsgpt-1.0.1/cogsgpt/metas/task_metas.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      369 2023-05-05 05:10:26.000000 cogsgpt-1.0.1/cogsgpt/schema.py
--rw-r--r--   0 runner    (1001) docker     (123)     1409 2023-05-05 05:10:26.000000 cogsgpt-1.0.1/cogsgpt/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 05:10:46.773779 cogsgpt-1.0.1/cogsgpt.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7519 2023-05-05 05:10:46.000000 cogsgpt-1.0.1/cogsgpt.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1261 2023-05-05 05:10:46.000000 cogsgpt-1.0.1/cogsgpt.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 05:10:46.000000 cogsgpt-1.0.1/cogsgpt.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      198 2023-05-05 05:10:46.000000 cogsgpt-1.0.1/cogsgpt.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-05 05:10:46.000000 cogsgpt-1.0.1/cogsgpt.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      948 2023-05-05 05:10:26.000000 cogsgpt-1.0.1/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-05 05:10:46.781779 cogsgpt-1.0.1/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 05:10:46.781779 cogsgpt-1.0.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1893 2023-05-05 05:10:26.000000 cogsgpt-1.0.1/tests/test_awesome_chat.py
--rw-r--r--   0 runner    (1001) docker     (123)      550 2023-05-05 05:10:26.000000 cogsgpt-1.0.1/tests/test_bg_remove.py
--rw-r--r--   0 runner    (1001) docker     (123)     2840 2023-05-05 05:10:26.000000 cogsgpt-1.0.1/tests/test_form_recognizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     4952 2023-05-05 05:10:26.000000 cogsgpt-1.0.1/tests/test_image_analisys.py
--rw-r--r--   0 runner    (1001) docker     (123)      602 2023-05-05 05:10:26.000000 cogsgpt-1.0.1/tests/test_speech.py
--rw-r--r--   0 runner    (1001) docker     (123)     1632 2023-05-05 05:10:26.000000 cogsgpt-1.0.1/tests/test_text_analysis.py
--rw-r--r--   0 runner    (1001) docker     (123)     1232 2023-05-05 05:10:26.000000 cogsgpt-1.0.1/tests/test_text_generation.py
--rw-r--r--   0 runner    (1001) docker     (123)     1971 2023-05-05 05:10:26.000000 cogsgpt-1.0.1/tests/test_text_summarize.py
--rw-r--r--   0 runner    (1001) docker     (123)     1195 2023-05-05 05:10:26.000000 cogsgpt-1.0.1/tests/test_text_translation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 05:55:00.068015 cogsgpt-1.0.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-05-05 05:54:48.000000 cogsgpt-1.0.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-05 05:54:48.000000 cogsgpt-1.0.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     7519 2023-05-05 05:55:00.068015 cogsgpt-1.0.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5776 2023-05-05 05:54:48.000000 cogsgpt-1.0.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 05:55:00.064015 cogsgpt-1.0.2/cogsgpt/
+-rw-r--r--   0 runner    (1001) docker     (123)      154 2023-05-05 05:54:48.000000 cogsgpt-1.0.2/cogsgpt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14467 2023-05-05 05:54:48.000000 cogsgpt-1.0.2/cogsgpt/awesome_chat.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 05:55:00.064015 cogsgpt-1.0.2/cogsgpt/cogsmodel/
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-05-05 05:54:48.000000 cogsgpt-1.0.2/cogsgpt/cogsmodel/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      202 2023-05-05 05:54:48.000000 cogsgpt-1.0.2/cogsgpt/cogsmodel/base_model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 05:55:00.064015 cogsgpt-1.0.2/cogsgpt/cogsmodel/cv/
+-rw-r--r--   0 runner    (1001) docker     (123)     1058 2023-05-05 05:54:48.000000 cogsgpt-1.0.2/cogsgpt/cogsmodel/cv/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1869 2023-05-05 05:54:48.000000 cogsgpt-1.0.2/cogsgpt/cogsmodel/cv/background_remover.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5601 2023-05-05 05:54:48.000000 cogsgpt-1.0.2/cogsgpt/cogsmodel/cv/form_recognizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7020 2023-05-05 05:54:48.000000 cogsgpt-1.0.2/cogsgpt/cogsmodel/cv/image_analysis_v3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6544 2023-05-05 05:54:48.000000 cogsgpt-1.0.2/cogsgpt/cogsmodel/cv/image_analysis_v4.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2581 2023-05-05 05:54:48.000000 cogsgpt-1.0.2/cogsgpt/cogsmodel/cv/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 05:55:00.068015 cogsgpt-1.0.2/cogsgpt/cogsmodel/nlp/
+-rw-r--r--   0 runner    (1001) docker     (123)      599 2023-05-05 05:54:48.000000 cogsgpt-1.0.2/cogsgpt/cogsmodel/nlp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3504 2023-05-05 05:54:48.000000 cogsgpt-1.0.2/cogsgpt/cogsmodel/nlp/text_analysis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1823 2023-05-05 05:54:48.000000 cogsgpt-1.0.2/cogsgpt/cogsmodel/nlp/text_generation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2219 2023-05-05 05:54:48.000000 cogsgpt-1.0.2/cogsgpt/cogsmodel/nlp/text_summarize.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1710 2023-05-05 05:54:48.000000 cogsgpt-1.0.2/cogsgpt/cogsmodel/nlp/text_translation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 05:55:00.068015 cogsgpt-1.0.2/cogsgpt/cogsmodel/speech/
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-05-05 05:54:48.000000 cogsgpt-1.0.2/cogsgpt/cogsmodel/speech/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3926 2023-05-05 05:54:48.000000 cogsgpt-1.0.2/cogsgpt/cogsmodel/speech/speech.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2835 2023-05-05 05:54:48.000000 cogsgpt-1.0.2/cogsgpt/llm.py
+-rw-r--r--   0 runner    (1001) docker     (123)      460 2023-05-05 05:54:48.000000 cogsgpt-1.0.2/cogsgpt/logger.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 05:55:00.068015 cogsgpt-1.0.2/cogsgpt/metas/
+-rw-r--r--   0 runner    (1001) docker     (123)      316 2023-05-05 05:54:48.000000 cogsgpt-1.0.2/cogsgpt/metas/generate_response_presteps.json
+-rw-r--r--   0 runner    (1001) docker     (123)      955 2023-05-05 05:54:48.000000 cogsgpt-1.0.2/cogsgpt/metas/parse_task_presteps.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2195 2023-05-05 05:54:48.000000 cogsgpt-1.0.2/cogsgpt/metas/prompts.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     4718 2023-05-05 05:54:48.000000 cogsgpt-1.0.2/cogsgpt/metas/task_metas.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      369 2023-05-05 05:54:48.000000 cogsgpt-1.0.2/cogsgpt/schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1409 2023-05-05 05:54:48.000000 cogsgpt-1.0.2/cogsgpt/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 05:55:00.064015 cogsgpt-1.0.2/cogsgpt.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7519 2023-05-05 05:55:00.000000 cogsgpt-1.0.2/cogsgpt.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1261 2023-05-05 05:55:00.000000 cogsgpt-1.0.2/cogsgpt.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 05:55:00.000000 cogsgpt-1.0.2/cogsgpt.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      198 2023-05-05 05:55:00.000000 cogsgpt-1.0.2/cogsgpt.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-05 05:55:00.000000 cogsgpt-1.0.2/cogsgpt.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      948 2023-05-05 05:54:48.000000 cogsgpt-1.0.2/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-05 05:55:00.068015 cogsgpt-1.0.2/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 05:55:00.068015 cogsgpt-1.0.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1893 2023-05-05 05:54:48.000000 cogsgpt-1.0.2/tests/test_awesome_chat.py
+-rw-r--r--   0 runner    (1001) docker     (123)      550 2023-05-05 05:54:48.000000 cogsgpt-1.0.2/tests/test_bg_remove.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2840 2023-05-05 05:54:48.000000 cogsgpt-1.0.2/tests/test_form_recognizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4952 2023-05-05 05:54:48.000000 cogsgpt-1.0.2/tests/test_image_analisys.py
+-rw-r--r--   0 runner    (1001) docker     (123)      602 2023-05-05 05:54:48.000000 cogsgpt-1.0.2/tests/test_speech.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1632 2023-05-05 05:54:48.000000 cogsgpt-1.0.2/tests/test_text_analysis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1232 2023-05-05 05:54:48.000000 cogsgpt-1.0.2/tests/test_text_generation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1971 2023-05-05 05:54:48.000000 cogsgpt-1.0.2/tests/test_text_summarize.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1195 2023-05-05 05:54:48.000000 cogsgpt-1.0.2/tests/test_text_translation.py
```

### Comparing `cogsgpt-1.0.1/LICENSE` & `cogsgpt-1.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `cogsgpt-1.0.1/PKG-INFO` & `cogsgpt-1.0.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cogsgpt
-Version: 1.0.1
+Version: 1.0.2
 Summary: A multi-modal LLM integrated ChatGPT with Azure Cognitive Service
 Author-email: weitian <weitian.bnu@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 Tian Wei
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `cogsgpt-1.0.1/README.md` & `cogsgpt-1.0.2/README.md`

 * *Files identical despite different names*

### Comparing `cogsgpt-1.0.1/cogsgpt/awesome_chat.py` & `cogsgpt-1.0.2/cogsgpt/awesome_chat.py`

 * *Files identical despite different names*

### Comparing `cogsgpt-1.0.1/cogsgpt/cogsmodel/cv/__init__.py` & `cogsgpt-1.0.2/cogsgpt/cogsmodel/cv/__init__.py`

 * *Files identical despite different names*

### Comparing `cogsgpt-1.0.1/cogsgpt/cogsmodel/cv/background_remover.py` & `cogsgpt-1.0.2/cogsgpt/cogsmodel/cv/background_remover.py`

 * *Files identical despite different names*

### Comparing `cogsgpt-1.0.1/cogsgpt/cogsmodel/cv/form_recognizer.py` & `cogsgpt-1.0.2/cogsgpt/cogsmodel/cv/form_recognizer.py`

 * *Files identical despite different names*

### Comparing `cogsgpt-1.0.1/cogsgpt/cogsmodel/cv/image_analysis_v3.py` & `cogsgpt-1.0.2/cogsgpt/cogsmodel/cv/image_analysis_v3.py`

 * *Files identical despite different names*

### Comparing `cogsgpt-1.0.1/cogsgpt/cogsmodel/cv/image_analysis_v4.py` & `cogsgpt-1.0.2/cogsgpt/cogsmodel/cv/image_analysis_v4.py`

 * *Files identical despite different names*

### Comparing `cogsgpt-1.0.1/cogsgpt/cogsmodel/cv/utils.py` & `cogsgpt-1.0.2/cogsgpt/cogsmodel/cv/utils.py`

 * *Files identical despite different names*

### Comparing `cogsgpt-1.0.1/cogsgpt/cogsmodel/nlp/__init__.py` & `cogsgpt-1.0.2/cogsgpt/cogsmodel/nlp/__init__.py`

 * *Files identical despite different names*

### Comparing `cogsgpt-1.0.1/cogsgpt/cogsmodel/nlp/text_analysis.py` & `cogsgpt-1.0.2/cogsgpt/cogsmodel/nlp/text_analysis.py`

 * *Files identical despite different names*

### Comparing `cogsgpt-1.0.1/cogsgpt/cogsmodel/nlp/text_generation.py` & `cogsgpt-1.0.2/cogsgpt/cogsmodel/nlp/text_generation.py`

 * *Files identical despite different names*

### Comparing `cogsgpt-1.0.1/cogsgpt/cogsmodel/nlp/text_summarize.py` & `cogsgpt-1.0.2/cogsgpt/cogsmodel/nlp/text_summarize.py`

 * *Files identical despite different names*

### Comparing `cogsgpt-1.0.1/cogsgpt/cogsmodel/nlp/text_translation.py` & `cogsgpt-1.0.2/cogsgpt/cogsmodel/nlp/text_translation.py`

 * *Files identical despite different names*

### Comparing `cogsgpt-1.0.1/cogsgpt/cogsmodel/speech/speech.py` & `cogsgpt-1.0.2/cogsgpt/cogsmodel/speech/speech.py`

 * *Files identical despite different names*

### Comparing `cogsgpt-1.0.1/cogsgpt/llm.py` & `cogsgpt-1.0.2/cogsgpt/llm.py`

 * *Files identical despite different names*

### Comparing `cogsgpt-1.0.1/cogsgpt/metas/parse_task_presteps.json` & `cogsgpt-1.0.2/cogsgpt/metas/parse_task_presteps.json`

 * *Files identical despite different names*

### Comparing `cogsgpt-1.0.1/cogsgpt/metas/prompts.yaml` & `cogsgpt-1.0.2/cogsgpt/metas/prompts.yaml`

 * *Files 6% similar despite different names*

```diff
@@ -23,9 +23,9 @@
   system: >-
     In this stage, you need to give a directly response to user's input with the task execution logs.
 
   user: >-
     Yes. Please follow the below rules to generate your response:
     1. First think carefully and filter out task results that are not relevant to my request.
     2. Then, based on the tasks results, directly answer my request in your friendly tone.
-    3. Your response MUST contain the paths to the generated ressources if they are relevant to my request.
+    3. Your response should contain the paths to the generated ressources if they exist and are relevant to my request.
     4. If there is nothing in the task results, you MUST tell me you can't solve my request.
```

### Comparing `cogsgpt-1.0.1/cogsgpt/metas/task_metas.yaml` & `cogsgpt-1.0.2/cogsgpt/metas/task_metas.yaml`

 * *Files identical despite different names*

### Comparing `cogsgpt-1.0.1/cogsgpt/utils.py` & `cogsgpt-1.0.2/cogsgpt/utils.py`

 * *Files identical despite different names*

### Comparing `cogsgpt-1.0.1/cogsgpt.egg-info/PKG-INFO` & `cogsgpt-1.0.2/cogsgpt.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cogsgpt
-Version: 1.0.1
+Version: 1.0.2
 Summary: A multi-modal LLM integrated ChatGPT with Azure Cognitive Service
 Author-email: weitian <weitian.bnu@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 Tian Wei
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
```

### Comparing `cogsgpt-1.0.1/cogsgpt.egg-info/SOURCES.txt` & `cogsgpt-1.0.2/cogsgpt.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cogsgpt-1.0.1/pyproject.toml` & `cogsgpt-1.0.2/pyproject.toml`

 * *Files 22% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 [build-system]
 requires      = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "cogsgpt"
-version = "1.0.1"
+version = "1.0.2"
 description = "A multi-modal LLM integrated ChatGPT with Azure Cognitive Service"
 readme = "README.md"
 authors = [{ name = "weitian", email = "weitian.bnu@gmail.com" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
```

### Comparing `cogsgpt-1.0.1/tests/test_awesome_chat.py` & `cogsgpt-1.0.2/tests/test_awesome_chat.py`

 * *Files identical despite different names*

### Comparing `cogsgpt-1.0.1/tests/test_bg_remove.py` & `cogsgpt-1.0.2/tests/test_bg_remove.py`

 * *Files identical despite different names*

### Comparing `cogsgpt-1.0.1/tests/test_form_recognizer.py` & `cogsgpt-1.0.2/tests/test_form_recognizer.py`

 * *Files identical despite different names*

### Comparing `cogsgpt-1.0.1/tests/test_image_analisys.py` & `cogsgpt-1.0.2/tests/test_image_analisys.py`

 * *Files identical despite different names*

### Comparing `cogsgpt-1.0.1/tests/test_speech.py` & `cogsgpt-1.0.2/tests/test_speech.py`

 * *Files identical despite different names*

### Comparing `cogsgpt-1.0.1/tests/test_text_analysis.py` & `cogsgpt-1.0.2/tests/test_text_analysis.py`

 * *Files identical despite different names*

### Comparing `cogsgpt-1.0.1/tests/test_text_generation.py` & `cogsgpt-1.0.2/tests/test_text_generation.py`

 * *Files identical despite different names*

### Comparing `cogsgpt-1.0.1/tests/test_text_summarize.py` & `cogsgpt-1.0.2/tests/test_text_summarize.py`

 * *Files identical despite different names*

### Comparing `cogsgpt-1.0.1/tests/test_text_translation.py` & `cogsgpt-1.0.2/tests/test_text_translation.py`

 * *Files identical despite different names*

