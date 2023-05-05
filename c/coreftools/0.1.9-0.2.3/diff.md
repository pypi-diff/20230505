# Comparing `tmp/coreftools-0.1.9-py3-none-any.whl.zip` & `tmp/coreftools-0.2.3-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,9 @@
-Zip file size: 5371 bytes, number of entries: 6
+Zip file size: 5623 bytes, number of entries: 7
 -rw-r--r--  2.0 unx        0 b- defN 23-May-04 12:56 coreftools/__init__.py
 -rw-r--r--  2.0 unx     6996 b- defN 23-May-05 19:20 coreftools/corefresolvers.py
--rw-r--r--  2.0 unx     3676 b- defN 23-May-05 19:57 coreftools-0.1.9.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-May-05 19:57 coreftools-0.1.9.dist-info/WHEEL
--rw-r--r--  2.0 unx       11 b- defN 23-May-05 19:57 coreftools-0.1.9.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      471 b- defN 23-May-05 19:57 coreftools-0.1.9.dist-info/RECORD
-6 files, 11246 bytes uncompressed, 4513 bytes compressed:  59.9%
+-rw-r--r--  2.0 unx     3593 b- defN 23-May-05 20:04 coreftools-0.2.3.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-May-05 20:04 coreftools-0.2.3.dist-info/WHEEL
+-rw-r--r--  2.0 unx      109 b- defN 23-May-05 20:04 coreftools-0.2.3.dist-info/dependency_links.txt
+-rw-r--r--  2.0 unx       11 b- defN 23-May-05 20:04 coreftools-0.2.3.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      574 b- defN 23-May-05 20:04 coreftools-0.2.3.dist-info/RECORD
+7 files, 11375 bytes uncompressed, 4595 bytes compressed:  59.6%
```

## zipnote {}

```diff
@@ -1,19 +1,22 @@
 Filename: coreftools/__init__.py
 Comment: 
 
 Filename: coreftools/corefresolvers.py
 Comment: 
 
-Filename: coreftools-0.1.9.dist-info/METADATA
+Filename: coreftools-0.2.3.dist-info/METADATA
 Comment: 
 
-Filename: coreftools-0.1.9.dist-info/WHEEL
+Filename: coreftools-0.2.3.dist-info/WHEEL
 Comment: 
 
-Filename: coreftools-0.1.9.dist-info/top_level.txt
+Filename: coreftools-0.2.3.dist-info/dependency_links.txt
 Comment: 
 
-Filename: coreftools-0.1.9.dist-info/RECORD
+Filename: coreftools-0.2.3.dist-info/top_level.txt
+Comment: 
+
+Filename: coreftools-0.2.3.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `coreftools-0.1.9.dist-info/METADATA` & `coreftools-0.2.3.dist-info/METADATA`

 * *Files 4% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 Metadata-Version: 2.1
 Name: coreftools
-Version: 0.1.9
+Version: 0.2.3
 Summary: Coreference-Resolution library
-Download-URL: https://github.com/explosion/spacy-models/releases/download/en_core_web_sm-2.1.0/en_core_web_sm-2.1.0.tar.gz
 Author: Soumya-Ranjan-Sahoo
 License: MIT
 Description-Content-Type: text/markdown
 Requires-Dist: neuralcoref
 Requires-Dist: spacy (==2.1.0)
 Requires-Dist: allennlp
 Requires-Dist: allennlp-models
 Requires-Dist: pandas
 Requires-Dist: openai
+Requires-Dist: en-core-web-sm (==2.1.0)
 
 
 This is a coreference resolution utility  package that supports multiple transformer-based coreference resolvers. The current version supports an improved version of the AllenNLP SPANBERT model and a GPT3 (text-davinci-003) based resolver that supports few-shot prompts. Coreference resolution is the task of identifying all expressions (e.g., pronouns, names, definite descriptions) in a text that refer to the same entity. This is a crucial task for many natural language processing applications such as question answering, summarization, and sentiment analysis.
 
 Our tool is designed to help researchers and developers experiment with different transformer-based coreference resolvers and compare their performance. The package is currently under experimentation and cannot be readily used. However, we aim to make it publicly available in the future.
 
 The AllenNLP SPAN-BERT model is a state-of-the-art coreference resolution model that is based on the popular BERT architecture. We have made improvements to the model by handling nested coreferent mentions and cataphoras. The GPT3-based resolver, on the other hand, is a cutting-edge model that is capable of few-shot learning, meaning that it can adapt to new variations with a few example prompts.
```

