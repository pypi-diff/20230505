# Comparing `tmp/cogsgpt-1.0.0.tar.gz` & `tmp/cogsgpt-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cogsgpt-1.0.0.tar", last modified: Tue May  2 14:25:54 2023, max compression
+gzip compressed data, was "cogsgpt-1.0.1.tar", last modified: Fri May  5 05:10:46 2023, max compression
```

## Comparing `cogsgpt-1.0.0.tar` & `cogsgpt-1.0.1.tar`

### file list

```diff
@@ -1,54 +1,54 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 14:25:54.428562 cogsgpt-1.0.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-05-02 14:25:43.000000 cogsgpt-1.0.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-02 14:25:43.000000 cogsgpt-1.0.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     7412 2023-05-02 14:25:54.428562 cogsgpt-1.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     5669 2023-05-02 14:25:43.000000 cogsgpt-1.0.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 14:25:54.424562 cogsgpt-1.0.0/cogsgpt/
--rw-r--r--   0 runner    (1001) docker     (123)      154 2023-05-02 14:25:43.000000 cogsgpt-1.0.0/cogsgpt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13639 2023-05-02 14:25:43.000000 cogsgpt-1.0.0/cogsgpt/awesome_chat.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 14:25:54.428562 cogsgpt-1.0.0/cogsgpt/cogsmodel/
--rw-r--r--   0 runner    (1001) docker     (123)       92 2023-05-02 14:25:43.000000 cogsgpt-1.0.0/cogsgpt/cogsmodel/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      202 2023-05-02 14:25:43.000000 cogsgpt-1.0.0/cogsgpt/cogsmodel/base_model.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 14:25:54.428562 cogsgpt-1.0.0/cogsgpt/cogsmodel/cv/
--rw-r--r--   0 runner    (1001) docker     (123)     1058 2023-05-02 14:25:43.000000 cogsgpt-1.0.0/cogsgpt/cogsmodel/cv/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1869 2023-05-02 14:25:43.000000 cogsgpt-1.0.0/cogsgpt/cogsmodel/cv/background_remover.py
--rw-r--r--   0 runner    (1001) docker     (123)     5601 2023-05-02 14:25:43.000000 cogsgpt-1.0.0/cogsgpt/cogsmodel/cv/form_recognizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     7020 2023-05-02 14:25:43.000000 cogsgpt-1.0.0/cogsgpt/cogsmodel/cv/image_analysis_v3.py
--rw-r--r--   0 runner    (1001) docker     (123)     6544 2023-05-02 14:25:43.000000 cogsgpt-1.0.0/cogsgpt/cogsmodel/cv/image_analysis_v4.py
--rw-r--r--   0 runner    (1001) docker     (123)     2581 2023-05-02 14:25:43.000000 cogsgpt-1.0.0/cogsgpt/cogsmodel/cv/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 14:25:54.428562 cogsgpt-1.0.0/cogsgpt/cogsmodel/nlp/
--rw-r--r--   0 runner    (1001) docker     (123)      599 2023-05-02 14:25:43.000000 cogsgpt-1.0.0/cogsgpt/cogsmodel/nlp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3504 2023-05-02 14:25:43.000000 cogsgpt-1.0.0/cogsgpt/cogsmodel/nlp/text_analysis.py
--rw-r--r--   0 runner    (1001) docker     (123)     1823 2023-05-02 14:25:43.000000 cogsgpt-1.0.0/cogsgpt/cogsmodel/nlp/text_generation.py
--rw-r--r--   0 runner    (1001) docker     (123)     2219 2023-05-02 14:25:43.000000 cogsgpt-1.0.0/cogsgpt/cogsmodel/nlp/text_summarize.py
--rw-r--r--   0 runner    (1001) docker     (123)     1710 2023-05-02 14:25:43.000000 cogsgpt-1.0.0/cogsgpt/cogsmodel/nlp/text_translation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 14:25:54.428562 cogsgpt-1.0.0/cogsgpt/cogsmodel/speech/
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-05-02 14:25:43.000000 cogsgpt-1.0.0/cogsgpt/cogsmodel/speech/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3926 2023-05-02 14:25:43.000000 cogsgpt-1.0.0/cogsgpt/cogsmodel/speech/speech.py
--rw-r--r--   0 runner    (1001) docker     (123)     2835 2023-05-02 14:25:43.000000 cogsgpt-1.0.0/cogsgpt/llm.py
--rw-r--r--   0 runner    (1001) docker     (123)      460 2023-05-02 14:25:43.000000 cogsgpt-1.0.0/cogsgpt/logger.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 14:25:54.428562 cogsgpt-1.0.0/cogsgpt/metas/
--rw-r--r--   0 runner    (1001) docker     (123)      316 2023-05-02 14:25:43.000000 cogsgpt-1.0.0/cogsgpt/metas/generate_response_presteps.json
--rw-r--r--   0 runner    (1001) docker     (123)     2861 2023-05-02 14:25:43.000000 cogsgpt-1.0.0/cogsgpt/metas/parse_task_presteps.json
--rw-r--r--   0 runner    (1001) docker     (123)     2047 2023-05-02 14:25:43.000000 cogsgpt-1.0.0/cogsgpt/metas/prompts.yaml
--rw-r--r--   0 runner    (1001) docker     (123)     4718 2023-05-02 14:25:43.000000 cogsgpt-1.0.0/cogsgpt/metas/task_metas.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      369 2023-05-02 14:25:43.000000 cogsgpt-1.0.0/cogsgpt/schema.py
--rw-r--r--   0 runner    (1001) docker     (123)      892 2023-05-02 14:25:43.000000 cogsgpt-1.0.0/cogsgpt/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 14:25:54.428562 cogsgpt-1.0.0/cogsgpt.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7412 2023-05-02 14:25:54.000000 cogsgpt-1.0.0/cogsgpt.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1261 2023-05-02 14:25:54.000000 cogsgpt-1.0.0/cogsgpt.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-02 14:25:54.000000 cogsgpt-1.0.0/cogsgpt.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      189 2023-05-02 14:25:54.000000 cogsgpt-1.0.0/cogsgpt.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-02 14:25:54.000000 cogsgpt-1.0.0/cogsgpt.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      932 2023-05-02 14:25:43.000000 cogsgpt-1.0.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-02 14:25:54.428562 cogsgpt-1.0.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-02 14:25:54.428562 cogsgpt-1.0.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     1763 2023-05-02 14:25:43.000000 cogsgpt-1.0.0/tests/test_awesome_chat.py
--rw-r--r--   0 runner    (1001) docker     (123)      550 2023-05-02 14:25:43.000000 cogsgpt-1.0.0/tests/test_bg_remove.py
--rw-r--r--   0 runner    (1001) docker     (123)     2840 2023-05-02 14:25:43.000000 cogsgpt-1.0.0/tests/test_form_recognizer.py
--rw-r--r--   0 runner    (1001) docker     (123)     4952 2023-05-02 14:25:43.000000 cogsgpt-1.0.0/tests/test_image_analisys.py
--rw-r--r--   0 runner    (1001) docker     (123)      602 2023-05-02 14:25:43.000000 cogsgpt-1.0.0/tests/test_speech.py
--rw-r--r--   0 runner    (1001) docker     (123)     1632 2023-05-02 14:25:43.000000 cogsgpt-1.0.0/tests/test_text_analysis.py
--rw-r--r--   0 runner    (1001) docker     (123)     1232 2023-05-02 14:25:43.000000 cogsgpt-1.0.0/tests/test_text_generation.py
--rw-r--r--   0 runner    (1001) docker     (123)     1971 2023-05-02 14:25:43.000000 cogsgpt-1.0.0/tests/test_text_summarize.py
--rw-r--r--   0 runner    (1001) docker     (123)     1195 2023-05-02 14:25:43.000000 cogsgpt-1.0.0/tests/test_text_translation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 05:10:46.781779 cogsgpt-1.0.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-05-05 05:10:26.000000 cogsgpt-1.0.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-05 05:10:26.000000 cogsgpt-1.0.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     7519 2023-05-05 05:10:46.781779 cogsgpt-1.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     5776 2023-05-05 05:10:26.000000 cogsgpt-1.0.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 05:10:46.773779 cogsgpt-1.0.1/cogsgpt/
+-rw-r--r--   0 runner    (1001) docker     (123)      154 2023-05-05 05:10:26.000000 cogsgpt-1.0.1/cogsgpt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14467 2023-05-05 05:10:26.000000 cogsgpt-1.0.1/cogsgpt/awesome_chat.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 05:10:46.773779 cogsgpt-1.0.1/cogsgpt/cogsmodel/
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-05-05 05:10:26.000000 cogsgpt-1.0.1/cogsgpt/cogsmodel/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      202 2023-05-05 05:10:26.000000 cogsgpt-1.0.1/cogsgpt/cogsmodel/base_model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 05:10:46.777778 cogsgpt-1.0.1/cogsgpt/cogsmodel/cv/
+-rw-r--r--   0 runner    (1001) docker     (123)     1058 2023-05-05 05:10:26.000000 cogsgpt-1.0.1/cogsgpt/cogsmodel/cv/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1869 2023-05-05 05:10:26.000000 cogsgpt-1.0.1/cogsgpt/cogsmodel/cv/background_remover.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5601 2023-05-05 05:10:26.000000 cogsgpt-1.0.1/cogsgpt/cogsmodel/cv/form_recognizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7020 2023-05-05 05:10:26.000000 cogsgpt-1.0.1/cogsgpt/cogsmodel/cv/image_analysis_v3.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6544 2023-05-05 05:10:26.000000 cogsgpt-1.0.1/cogsgpt/cogsmodel/cv/image_analysis_v4.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2581 2023-05-05 05:10:26.000000 cogsgpt-1.0.1/cogsgpt/cogsmodel/cv/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 05:10:46.777778 cogsgpt-1.0.1/cogsgpt/cogsmodel/nlp/
+-rw-r--r--   0 runner    (1001) docker     (123)      599 2023-05-05 05:10:26.000000 cogsgpt-1.0.1/cogsgpt/cogsmodel/nlp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3504 2023-05-05 05:10:26.000000 cogsgpt-1.0.1/cogsgpt/cogsmodel/nlp/text_analysis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1823 2023-05-05 05:10:26.000000 cogsgpt-1.0.1/cogsgpt/cogsmodel/nlp/text_generation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2219 2023-05-05 05:10:26.000000 cogsgpt-1.0.1/cogsgpt/cogsmodel/nlp/text_summarize.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1710 2023-05-05 05:10:26.000000 cogsgpt-1.0.1/cogsgpt/cogsmodel/nlp/text_translation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 05:10:46.777778 cogsgpt-1.0.1/cogsgpt/cogsmodel/speech/
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-05-05 05:10:26.000000 cogsgpt-1.0.1/cogsgpt/cogsmodel/speech/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3926 2023-05-05 05:10:26.000000 cogsgpt-1.0.1/cogsgpt/cogsmodel/speech/speech.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2835 2023-05-05 05:10:26.000000 cogsgpt-1.0.1/cogsgpt/llm.py
+-rw-r--r--   0 runner    (1001) docker     (123)      460 2023-05-05 05:10:26.000000 cogsgpt-1.0.1/cogsgpt/logger.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 05:10:46.777778 cogsgpt-1.0.1/cogsgpt/metas/
+-rw-r--r--   0 runner    (1001) docker     (123)      316 2023-05-05 05:10:26.000000 cogsgpt-1.0.1/cogsgpt/metas/generate_response_presteps.json
+-rw-r--r--   0 runner    (1001) docker     (123)      955 2023-05-05 05:10:26.000000 cogsgpt-1.0.1/cogsgpt/metas/parse_task_presteps.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2183 2023-05-05 05:10:26.000000 cogsgpt-1.0.1/cogsgpt/metas/prompts.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     4718 2023-05-05 05:10:26.000000 cogsgpt-1.0.1/cogsgpt/metas/task_metas.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)      369 2023-05-05 05:10:26.000000 cogsgpt-1.0.1/cogsgpt/schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1409 2023-05-05 05:10:26.000000 cogsgpt-1.0.1/cogsgpt/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 05:10:46.773779 cogsgpt-1.0.1/cogsgpt.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7519 2023-05-05 05:10:46.000000 cogsgpt-1.0.1/cogsgpt.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1261 2023-05-05 05:10:46.000000 cogsgpt-1.0.1/cogsgpt.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 05:10:46.000000 cogsgpt-1.0.1/cogsgpt.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      198 2023-05-05 05:10:46.000000 cogsgpt-1.0.1/cogsgpt.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-05 05:10:46.000000 cogsgpt-1.0.1/cogsgpt.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      948 2023-05-05 05:10:26.000000 cogsgpt-1.0.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-05 05:10:46.781779 cogsgpt-1.0.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 05:10:46.781779 cogsgpt-1.0.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     1893 2023-05-05 05:10:26.000000 cogsgpt-1.0.1/tests/test_awesome_chat.py
+-rw-r--r--   0 runner    (1001) docker     (123)      550 2023-05-05 05:10:26.000000 cogsgpt-1.0.1/tests/test_bg_remove.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2840 2023-05-05 05:10:26.000000 cogsgpt-1.0.1/tests/test_form_recognizer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4952 2023-05-05 05:10:26.000000 cogsgpt-1.0.1/tests/test_image_analisys.py
+-rw-r--r--   0 runner    (1001) docker     (123)      602 2023-05-05 05:10:26.000000 cogsgpt-1.0.1/tests/test_speech.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1632 2023-05-05 05:10:26.000000 cogsgpt-1.0.1/tests/test_text_analysis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1232 2023-05-05 05:10:26.000000 cogsgpt-1.0.1/tests/test_text_generation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1971 2023-05-05 05:10:26.000000 cogsgpt-1.0.1/tests/test_text_summarize.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1195 2023-05-05 05:10:26.000000 cogsgpt-1.0.1/tests/test_text_translation.py
```

### Comparing `cogsgpt-1.0.0/LICENSE` & `cogsgpt-1.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `cogsgpt-1.0.0/PKG-INFO` & `cogsgpt-1.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cogsgpt
-Version: 1.0.0
+Version: 1.0.1
 Summary: A multi-modal LLM integrated ChatGPT with Azure Cognitive Service
 Author-email: weitian <weitian.bnu@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 Tian Wei
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -56,14 +56,16 @@
 *(Answered by ChatGPT)*
 
 > Azure Cognitive Services is a collection of pre-built machine learning models that developers can use to add intelligent features to their applications without requiring extensive knowledge of data science or machine learning. These services include vision, speech, language, and decision-making capabilities, such as text translation, speech recognition, image recognition, and sentiment analysis. Azure Cognitive Services allows developers to quickly and easily incorporate advanced AI features into their applications, reducing the time and cost of building such features from scratch. It also provides enterprise-level security, scalability, and availability for applications that require high levels of reliability and performance.
 
 ### What is CogsGPT
 CogsGPT is a conversational system which utilizes the ChatGPT model as the controller and integrates with Azure Cognitive Services as collaborative executors to achieve multimodal capabilities to some extent. Using CogsGPT, you can simply access Azure Cognitive Services via natural language to process image or audio inputs, without any knowledge of the underlying APIs. You can even ask CogsGPT to perform some complex tasks such as summarizing a long speech into a short audio clip while retaining the main information. CogsGPT will automatically decide which services to use and how to use them to achieve the goal.
 
+You can find the list of pre-built services supported by CogsGPT [here](./cogsgpt/metas/task_metas.yaml).
+
 ### How does CogsGPT work
 
 The workflow of CogsGPT consists of three stages:
 1. Task Planing Stage: In this stage, CogsGPT will leverage ChatGPT to parse user's input into a sequence of Azure Cognitive Service tasks which have the most potentials to solve user's request. Each task may depend on the execution result of previous tasks.
 2. Task Execution Stage: In this stage, CogsGPT will execute the tasks sequentially. The execution results will be stored for future reference.
 3. Response Generation Stage: In this stage, CogsGPT will leverage ChatGPT again to generate a final response to user's request based on the execution results of the second stage. The response may be a text, an image, an audio, or a combination of them.
```

### Comparing `cogsgpt-1.0.0/README.md` & `cogsgpt-1.0.1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -20,14 +20,16 @@
 *(Answered by ChatGPT)*
 
 > Azure Cognitive Services is a collection of pre-built machine learning models that developers can use to add intelligent features to their applications without requiring extensive knowledge of data science or machine learning. These services include vision, speech, language, and decision-making capabilities, such as text translation, speech recognition, image recognition, and sentiment analysis. Azure Cognitive Services allows developers to quickly and easily incorporate advanced AI features into their applications, reducing the time and cost of building such features from scratch. It also provides enterprise-level security, scalability, and availability for applications that require high levels of reliability and performance.
 
 ### What is CogsGPT
 CogsGPT is a conversational system which utilizes the ChatGPT model as the controller and integrates with Azure Cognitive Services as collaborative executors to achieve multimodal capabilities to some extent. Using CogsGPT, you can simply access Azure Cognitive Services via natural language to process image or audio inputs, without any knowledge of the underlying APIs. You can even ask CogsGPT to perform some complex tasks such as summarizing a long speech into a short audio clip while retaining the main information. CogsGPT will automatically decide which services to use and how to use them to achieve the goal.
 
+You can find the list of pre-built services supported by CogsGPT [here](./cogsgpt/metas/task_metas.yaml).
+
 ### How does CogsGPT work
 
 The workflow of CogsGPT consists of three stages:
 1. Task Planing Stage: In this stage, CogsGPT will leverage ChatGPT to parse user's input into a sequence of Azure Cognitive Service tasks which have the most potentials to solve user's request. Each task may depend on the execution result of previous tasks.
 2. Task Execution Stage: In this stage, CogsGPT will execute the tasks sequentially. The execution results will be stored for future reference.
 3. Response Generation Stage: In this stage, CogsGPT will leverage ChatGPT again to generate a final response to user's request based on the execution results of the second stage. The response may be a text, an image, an audio, or a combination of them.
```

### Comparing `cogsgpt-1.0.0/cogsgpt/awesome_chat.py` & `cogsgpt-1.0.1/cogsgpt/awesome_chat.py`

 * *Files 3% similar despite different names*

```diff
@@ -17,14 +17,15 @@
 from langchain.schema import PromptValue
 from langchain.memory import ConversationBufferMemory
 
 from cogsgpt.schema import ArgsType, LanguageType
 from cogsgpt.llm import LLMManager
 from cogsgpt.cogsmodel import *
 from cogsgpt.logger import logger
+from cogsgpt.utils import num_tokens_from_string
 
 
 TaskMap = {
     "form-recognizer": FormReadModel,
     "form-layout": FormLayoutModel,
     "form-key-value": FormKeyValueModel,
     "w2-tax-form": W2TaxFormModel,
@@ -67,27 +68,29 @@
                  model_name: str = "",
                  deployment_name: str = "",
                  deployment_version: str = "",
                  temperature: float = 0.7,
                  request_timeout: int = 60,
                  max_retries: int = 6,
                  max_tokens: int | None = None,
+                 save_history: bool = True,
                  verbose: bool = False,
                  ) -> None:
         """
         The CogsGPT class is the main class for the CogsGPT library. It provides a simple interface to chat with Azure Cognitive Services.
 
         Args:
             model_name (str, optional): The name of the OpenAI model. Defaults to "". If not specified, it will be read from the environment variable OPENAI_MODEL_NAME.
             deployment_name (str, optional): The name of the Azure deployment. Defaults to "". If not specified, it will be read from the environment variable OPENAI_DEPLOYMENT_NAME.
             deployment_version (str, optional): The version of the Azure deployment. Defaults to "". If not specified, it will be read from the environment variable OPENAI_DEPLOYMENT_VERSION.
             temperature (float, optional): The temperature of the OpenAI model. Defaults to 0.7.
             request_timeout (int, optional): The timeout of the OpenAI model. Defaults to 60.
             max_retries (int, optional): The maximum number of retries of the OpenAI model. Defaults to 6.
             max_tokens (int | None, optional): The maximum number of tokens of the OpenAI model. Defaults to None.
+            save_history (bool, optional): Whether to save the chat history. Defaults to True.
             verbose (bool, optional): Whether to print verbose logs. Defaults to False.
 
         Examples:
             >>> from cogsgpt import CogsGPT
             >>> chatbot = CogsGPT()
             >>> chatbot.chat("What's the content of this image?")
         """
@@ -143,14 +146,16 @@
             temperature=temperature,
             request_timeout=request_timeout,
             max_retries=max_retries,
             max_tokens=max_tokens,
             verbose=verbose,
         ).LLM
 
+        self._save_history = save_history
+
         if verbose:
             logger.setLevel("DEBUG")
 
     def _create_prompt(self, 
                        system_prompt: str = "", system_prompt_vars: List[str] = [],
                        user_prompt: str = "", user_prompt_vars: List[str] = [], 
                        presteps: List[Dict] = [], presteps_vars: List[str] = []) -> ChatPromptTemplate:
@@ -243,18 +248,22 @@
         Args:
             human_input (str): User input.
 
         Returns:
             List[Dict]: A list of Azure Cognitive Service tasks.
         """
         messages = self._format_parse_task_prompt(human_input)
+        messages_tokens = num_tokens_from_string(messages.to_string())
         logger.debug(f"[Parse Task] Prompt: {messages.to_string()}")
+        logger.debug(f"[Parse Task] Prompt Tokens: {messages_tokens}")
 
         response = self.chatbot(messages.to_messages()).content
+        response_tokens = num_tokens_from_string(response)
         logger.info(f"[Parse Task] Result: {response}")
+        logger.debug(f"[Parse Task] Result Tokens: {response_tokens}")
 
         return json.loads(response)
 
     def execute_tasks(self, task_list: List[Dict]) -> List[Dict]:
         """
         Execute a series of Azure Cognitive Service tasks.
 
@@ -288,18 +297,22 @@
             human_input (str): User input.
             task_result_list (List[Dict]): A list of Azure Cognitive Service tasks with results.
 
         Returns:
             str: Final response.
         """
         messages = self._format_generate_response_prompt(human_input, task_result_list)
+        messages_tokens = num_tokens_from_string(messages.to_string())
         logger.debug(f"[Generate Response] Prompt: {messages.to_string()}")
+        logger.debug(f"[Generate Response] Prompt Tokens: {messages_tokens}")
 
         response = self.chatbot(messages.to_messages()).content
+        response_tokens = num_tokens_from_string(response)
         logger.info(f"[Generate Response] Result: {response}")
+        logger.debug(f"[Generate Response] Result Tokens: {response_tokens}")
 
         return response
 
     def chat(self, human_input: str) -> str:
         """
         This is the main method of CogsGPT class. It calls the following methods in order to generate a final response:
         1. parse_tasks: parse user input into a series of Azure Cognitive Service tasks
@@ -322,11 +335,12 @@
         task_result_list = self.execute_tasks(task_list)
 
         # 3. generate response
         logger.info("[CogsGPT] Generating final response...")
         response = self.generate_response(human_input, task_result_list)
 
         # 4. save human_input/response into memory
-        logger.info("[CogsGPT] Saving context...")
-        self.save_context(human_input, response)
+        if self._save_history:
+            logger.info("[CogsGPT] Saving context...")
+            self.save_context(human_input, response)
 
         return response
```

### Comparing `cogsgpt-1.0.0/cogsgpt/cogsmodel/cv/__init__.py` & `cogsgpt-1.0.1/cogsgpt/cogsmodel/cv/__init__.py`

 * *Files identical despite different names*

### Comparing `cogsgpt-1.0.0/cogsgpt/cogsmodel/cv/background_remover.py` & `cogsgpt-1.0.1/cogsgpt/cogsmodel/cv/background_remover.py`

 * *Files identical despite different names*

### Comparing `cogsgpt-1.0.0/cogsgpt/cogsmodel/cv/form_recognizer.py` & `cogsgpt-1.0.1/cogsgpt/cogsmodel/cv/form_recognizer.py`

 * *Files identical despite different names*

### Comparing `cogsgpt-1.0.0/cogsgpt/cogsmodel/cv/image_analysis_v3.py` & `cogsgpt-1.0.1/cogsgpt/cogsmodel/cv/image_analysis_v3.py`

 * *Files identical despite different names*

### Comparing `cogsgpt-1.0.0/cogsgpt/cogsmodel/cv/image_analysis_v4.py` & `cogsgpt-1.0.1/cogsgpt/cogsmodel/cv/image_analysis_v4.py`

 * *Files identical despite different names*

### Comparing `cogsgpt-1.0.0/cogsgpt/cogsmodel/cv/utils.py` & `cogsgpt-1.0.1/cogsgpt/cogsmodel/cv/utils.py`

 * *Files identical despite different names*

### Comparing `cogsgpt-1.0.0/cogsgpt/cogsmodel/nlp/__init__.py` & `cogsgpt-1.0.1/cogsgpt/cogsmodel/nlp/__init__.py`

 * *Files identical despite different names*

### Comparing `cogsgpt-1.0.0/cogsgpt/cogsmodel/nlp/text_analysis.py` & `cogsgpt-1.0.1/cogsgpt/cogsmodel/nlp/text_analysis.py`

 * *Files identical despite different names*

### Comparing `cogsgpt-1.0.0/cogsgpt/cogsmodel/nlp/text_generation.py` & `cogsgpt-1.0.1/cogsgpt/cogsmodel/nlp/text_generation.py`

 * *Files identical despite different names*

### Comparing `cogsgpt-1.0.0/cogsgpt/cogsmodel/nlp/text_summarize.py` & `cogsgpt-1.0.1/cogsgpt/cogsmodel/nlp/text_summarize.py`

 * *Files identical despite different names*

### Comparing `cogsgpt-1.0.0/cogsgpt/cogsmodel/nlp/text_translation.py` & `cogsgpt-1.0.1/cogsgpt/cogsmodel/nlp/text_translation.py`

 * *Files identical despite different names*

### Comparing `cogsgpt-1.0.0/cogsgpt/cogsmodel/speech/speech.py` & `cogsgpt-1.0.1/cogsgpt/cogsmodel/speech/speech.py`

 * *Files identical despite different names*

### Comparing `cogsgpt-1.0.0/cogsgpt/llm.py` & `cogsgpt-1.0.1/cogsgpt/llm.py`

 * *Files identical despite different names*

### Comparing `cogsgpt-1.0.0/cogsgpt/metas/task_metas.yaml` & `cogsgpt-1.0.1/cogsgpt/metas/task_metas.yaml`

 * *Files identical despite different names*

### Comparing `cogsgpt-1.0.0/cogsgpt.egg-info/PKG-INFO` & `cogsgpt-1.0.1/cogsgpt.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cogsgpt
-Version: 1.0.0
+Version: 1.0.1
 Summary: A multi-modal LLM integrated ChatGPT with Azure Cognitive Service
 Author-email: weitian <weitian.bnu@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 Tian Wei
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -56,14 +56,16 @@
 *(Answered by ChatGPT)*
 
 > Azure Cognitive Services is a collection of pre-built machine learning models that developers can use to add intelligent features to their applications without requiring extensive knowledge of data science or machine learning. These services include vision, speech, language, and decision-making capabilities, such as text translation, speech recognition, image recognition, and sentiment analysis. Azure Cognitive Services allows developers to quickly and easily incorporate advanced AI features into their applications, reducing the time and cost of building such features from scratch. It also provides enterprise-level security, scalability, and availability for applications that require high levels of reliability and performance.
 
 ### What is CogsGPT
 CogsGPT is a conversational system which utilizes the ChatGPT model as the controller and integrates with Azure Cognitive Services as collaborative executors to achieve multimodal capabilities to some extent. Using CogsGPT, you can simply access Azure Cognitive Services via natural language to process image or audio inputs, without any knowledge of the underlying APIs. You can even ask CogsGPT to perform some complex tasks such as summarizing a long speech into a short audio clip while retaining the main information. CogsGPT will automatically decide which services to use and how to use them to achieve the goal.
 
+You can find the list of pre-built services supported by CogsGPT [here](./cogsgpt/metas/task_metas.yaml).
+
 ### How does CogsGPT work
 
 The workflow of CogsGPT consists of three stages:
 1. Task Planing Stage: In this stage, CogsGPT will leverage ChatGPT to parse user's input into a sequence of Azure Cognitive Service tasks which have the most potentials to solve user's request. Each task may depend on the execution result of previous tasks.
 2. Task Execution Stage: In this stage, CogsGPT will execute the tasks sequentially. The execution results will be stored for future reference.
 3. Response Generation Stage: In this stage, CogsGPT will leverage ChatGPT again to generate a final response to user's request based on the execution results of the second stage. The response may be a text, an image, an audio, or a combination of them.
```

### Comparing `cogsgpt-1.0.0/cogsgpt.egg-info/SOURCES.txt` & `cogsgpt-1.0.1/cogsgpt.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cogsgpt-1.0.0/pyproject.toml` & `cogsgpt-1.0.1/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 [build-system]
 requires      = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "cogsgpt"
-version = "1.0.0"
+version = "1.0.1"
 description = "A multi-modal LLM integrated ChatGPT with Azure Cognitive Service"
 readme = "README.md"
 authors = [{ name = "weitian", email = "weitian.bnu@gmail.com" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: MIT License",
     "Programming Language :: Python",
@@ -24,12 +24,13 @@
     "azure-ai-textanalytics==5.3.0b1",
     "azure-cognitiveservices-speech",
     "colorlog",
     "jinja2",
     "langchain",
     "openai",
     "pillow",
+    "tiktoken",
 ]
 requires-python = ">=3.8"
 
 [project.urls]
 Homepage = "https://github.com/whiskyboy/cogsgpt"
```

### Comparing `cogsgpt-1.0.0/tests/test_awesome_chat.py` & `cogsgpt-1.0.1/tests/test_awesome_chat.py`

 * *Files 13% similar despite different names*

```diff
@@ -4,30 +4,34 @@
 from cogsgpt.awesome_chat import CogsGPT
 
 
 if __name__ == "__main__":
     cogs_gpt = CogsGPT(temperature=0.2, verbose=True)
 
     test_cases = [
+        # ChitChat
+        "Hi, how are you?",
+        
         # CV
+        "What can I make with these ingredients? ./tests/examples/ingredients.png",
         "Describe the content of the image: ./tests/examples/presentation.png",
         "Extract the text from the image: ./tests/examples/handwritten-note.jpg",
         "How many people are there in the image: ./tests/examples/family.png?", 
         "Select images of dog from the list: [./tests/examples/animal-1.jpg, ./tests/examples/animal-2.jpg, ./tests/examples/animal-3.jpg]",
         "Remove the background of the image: ./tests/examples/wedding.png",
         "Crop a thumbnail for the image: ./tests/examples/wedding.png",
         
         # Speech
         "Convert the text 'CogsGPT is a multi-modal LLM integrated ChatGPT with Azure Cognitive Service' into speech.",
         "Extract the content of audio: ./tests/examples/cogsgpt.wav",
         
         # Form
         "List all the items and their prices from the receipt: ./tests/examples/receipt.png",
         "Extract the service address field from the invoice: ./tests/examples/sample-invoice.pdf",
-        "Extract the flight schedule table from the file: ./tests/examples/flight-schedule.png, and list all the flights with China Eastern airline.",
+        "List all the flights with China Eastern airline in the flight schedule table from the file: ./tests/examples/flight-schedule.png.",
         
         # Complex task
         "Summarize the content in the audio file: ./tests/examples/voa-1min-news.wav, and translate it into Chinese. Then read it out.",
     ]
 
     for test_case in test_cases:
         print('User: {}'.format(test_case))
```

### Comparing `cogsgpt-1.0.0/tests/test_bg_remove.py` & `cogsgpt-1.0.1/tests/test_bg_remove.py`

 * *Files identical despite different names*

### Comparing `cogsgpt-1.0.0/tests/test_form_recognizer.py` & `cogsgpt-1.0.1/tests/test_form_recognizer.py`

 * *Files identical despite different names*

### Comparing `cogsgpt-1.0.0/tests/test_image_analisys.py` & `cogsgpt-1.0.1/tests/test_image_analisys.py`

 * *Files identical despite different names*

### Comparing `cogsgpt-1.0.0/tests/test_speech.py` & `cogsgpt-1.0.1/tests/test_speech.py`

 * *Files identical despite different names*

### Comparing `cogsgpt-1.0.0/tests/test_text_analysis.py` & `cogsgpt-1.0.1/tests/test_text_analysis.py`

 * *Files identical despite different names*

### Comparing `cogsgpt-1.0.0/tests/test_text_generation.py` & `cogsgpt-1.0.1/tests/test_text_generation.py`

 * *Files identical despite different names*

### Comparing `cogsgpt-1.0.0/tests/test_text_summarize.py` & `cogsgpt-1.0.1/tests/test_text_summarize.py`

 * *Files identical despite different names*

### Comparing `cogsgpt-1.0.0/tests/test_text_translation.py` & `cogsgpt-1.0.1/tests/test_text_translation.py`

 * *Files identical despite different names*

