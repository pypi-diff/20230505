# Comparing `tmp/coreftools-0.1.3-py3-none-any.whl.zip` & `tmp/coreftools-0.1.5-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,8 +1,8 @@
-Zip file size: 4879 bytes, number of entries: 6
+Zip file size: 5295 bytes, number of entries: 6
 -rw-r--r--  2.0 unx        0 b- defN 23-May-04 12:56 coreftools/__init__.py
--rw-r--r--  2.0 unx     5994 b- defN 23-May-05 15:16 coreftools/corefresolvers.py
--rw-r--r--  2.0 unx     3229 b- defN 23-May-05 15:59 coreftools-0.1.3.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-May-05 15:59 coreftools-0.1.3.dist-info/WHEEL
--rw-r--r--  2.0 unx       11 b- defN 23-May-05 15:59 coreftools-0.1.3.dist-info/top_level.txt
-?rw-rw-r--  2.0 unx      471 b- defN 23-May-05 15:59 coreftools-0.1.3.dist-info/RECORD
-6 files, 9797 bytes uncompressed, 4021 bytes compressed:  59.0%
+-rw-r--r--  2.0 unx     6984 b- defN 23-May-05 18:16 coreftools/corefresolvers.py
+-rw-r--r--  2.0 unx     3530 b- defN 23-May-05 19:09 coreftools-0.1.5.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-May-05 19:09 coreftools-0.1.5.dist-info/WHEEL
+-rw-r--r--  2.0 unx       11 b- defN 23-May-05 19:09 coreftools-0.1.5.dist-info/top_level.txt
+?rw-rw-r--  2.0 unx      471 b- defN 23-May-05 19:09 coreftools-0.1.5.dist-info/RECORD
+6 files, 11088 bytes uncompressed, 4437 bytes compressed:  60.0%
```

## zipnote {}

```diff
@@ -1,19 +1,19 @@
 Filename: coreftools/__init__.py
 Comment: 
 
 Filename: coreftools/corefresolvers.py
 Comment: 
 
-Filename: coreftools-0.1.3.dist-info/METADATA
+Filename: coreftools-0.1.5.dist-info/METADATA
 Comment: 
 
-Filename: coreftools-0.1.3.dist-info/WHEEL
+Filename: coreftools-0.1.5.dist-info/WHEEL
 Comment: 
 
-Filename: coreftools-0.1.3.dist-info/top_level.txt
+Filename: coreftools-0.1.5.dist-info/top_level.txt
 Comment: 
 
-Filename: coreftools-0.1.3.dist-info/RECORD
+Filename: coreftools-0.1.5.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## coreftools/corefresolvers.py

```diff
@@ -2,15 +2,15 @@
 from allennlp.predictors.predictor import Predictor
 import neuralcoref
 from typing import List
 from spacy.tokens import Doc, Span
 import pandas as pd
 import os
 import openai
-#openai.api_key = os.getenv("OPENAI_API_KEY")
+import re
 #print(openai.api_key )
 
 class SpanBERTResolver:
     def __init__(self, model_url: str = 'default_model_url'):
         self.nlp = spacy.load('en_core_web_sm')
         neuralcoref.add_to_pipe(self.nlp)
         if model_url == 'default_model_url':
@@ -78,15 +78,15 @@
             return ""
         doc = self.nlp(query)
         return self.improved_replace_corefs(doc,clusters)
     
 
 query_to_resolve = "When is the next service appointment, vehicle check or oil change? With Teleservices, your BMW knows exactly when the next inspection is due. When maintenance work is required or if there is a malfunction, it sends all relevant data to you and your preferred service partner. Even before your BMW Service Partner calls you to make an appointment, he or she already knows the condition of your vehicle, can order spare parts and is perfectly prepared to meet the individual requirements of your vehicle. This also shortens the wait time during the appointment."
 allennlp =  SpanBERTResolver()
-print(allennlp.resolve_coref(query_to_resolve))
+print("SPANBERT:",allennlp.resolve_coref(query_to_resolve))
 
 
 
 
 
 ### Check how they pass on the prompts in BMW repo ###
 
@@ -105,28 +105,37 @@
     """
 
 
 class GPTResolver:
     """
     Currently raises: openai.error.AuthenticationError: Incorrect API key provided: <module
     """
-    def __init__(self, openai_key):
-        openai.api_key = openai_key
+    def __init__(self):
+        openai.api_key = os.getenv("OPENAI_API_KEY")
 
-    def resolve_coref(self, few_shot_prompt:str,query_to_resolve:str):
-        gpt_prompt = few_shot_prompt + query_to_resolve
+    def resolve_coref(self, query_to_resolve:str, few_shot_prompt:str = None, engine:str="text-davinci-003") -> str :
+        if not few_shot_prompt:
+            few_shot_prompt = """
+            
+{ "input": "Resolve the coreferences in the following sentence and do not paraphrase: {John and Jane went to the park. They had a picnic and played frisbee. When they were done, they walked home together.}", "output": "Resolved query: {John and Jane went to the park. John and Jane had a picnic and played frisbee. When John and Jane were done, John and Jane walked home together.}" }
+{ "input": "Resolve the coreferences in the following sentence and do not paraphrase: {My car needs an oil change. When can I have the next appointment for it? }", "output": "Resolved query: {My car needs an oil change. When can I have the next appointment for an oil change?}" }
+
+"""
+        formatted_input_query = f'{{"input": "Resolve the coreferences in the following sentence and do not paraphrase: {query_to_resolve}"}}'
+        gpt_prompt = few_shot_prompt + formatted_input_query
         response = openai.Completion.create(
-            engine="text-davinci-003",
+            engine=engine,
             prompt=gpt_prompt,
             temperature=0.5,
             max_tokens=256,
             top_p=1.0,
             frequency_penalty=0.0,
             presence_penalty=0.0
         )
         response = response['choices'][0]['text']
-        return response
+        clean_response = re.sub(r'[^a-zA-Z0-9\s]', '', response.split(": ")[2])
+        return clean_response
     
 
-# query_to_resolve = "Harish is Shyam's brother. They grew up in Mumbai. His mother name is Shanta"
-# GPT = GPTResolver(openai)
-# print(GPT.resolve_coref(few_shot_prompt, query_to_resolve))
+query_to_resolve = "The chef prepared a delicious meal. It included steak, mashed potatoes, and green beans."
+GPT = GPTResolver()
+print("GPT3:",GPT.resolve_coref(query_to_resolve))
```

## Comparing `coreftools-0.1.3.dist-info/METADATA` & `coreftools-0.1.5.dist-info/METADATA`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: coreftools
-Version: 0.1.3
+Version: 0.1.5
 Summary: Coreference-Resolution library
 Author: Soumya-Ranjan-Sahoo
 License: MIT
 Description-Content-Type: text/markdown
 Requires-Dist: neuralcoref
 Requires-Dist: spacy (==2.1.0)
 Requires-Dist: allennlp
@@ -15,15 +15,15 @@
 
 This is a coreference resolution utility  package that supports multiple transformer-based coreference resolvers. The current version supports an improved version of the AllenNLP SPANBERT model and a GPT3 (text-davinci-003) based resolver that supports few-shot prompts. Coreference resolution is the task of identifying all expressions (e.g., pronouns, names, definite descriptions) in a text that refer to the same entity. This is a crucial task for many natural language processing applications such as question answering, summarization, and sentiment analysis.
 
 Our tool is designed to help researchers and developers experiment with different transformer-based coreference resolvers and compare their performance. The package is currently under experimentation and cannot be readily used. However, we aim to make it publicly available in the future.
 
 The AllenNLP SPAN-BERT model is a state-of-the-art coreference resolution model that is based on the popular BERT architecture. We have made improvements to the model by handling nested coreferent mentions and cataphoras. The GPT3-based resolver, on the other hand, is a cutting-edge model that is capable of few-shot learning, meaning that it can adapt to new variations with a few example prompts.
 
-Our tool is implemented in Python and is designed to be easy to use and integrate with existing NLP pipelines. It provides a simple interface for loading and using different coreference resolvers, and supports various input formats such as raw text and pre-processed text. We believe that our tool will be a valuable resource for researchers and developers working on coreference resolution and related NLP tasks. 
+Our Python package is designed to be easy to use and integrate with existing NLP pipelines. It provides a simple interface for loading and using different coreference resolvers, and supports various input formats such as raw text and pre-processed text. We believe that our tool will be a valuable resource for researchers and developers working on coreference resolution and related NLP tasks. 
 
 
 # Examples of using CorefTools
 
 Here are a few examples of how to use CorefTools, a Python package for coreference resolution.
 
 ## Example 1: Using the SpanBERTResolver
@@ -40,15 +40,15 @@
 
 # Output
 # John and Jane went to the park. John and Jane had a picnic and played frisbee. When John and Jane were done, John and Jane walked home together.
 ```
 
 ## Example 2
 
-The following example demonstrates how to use the `GPTResolver` class to resolve coreferences using the GPT-3 model.
+The following example demonstrates how to use the `GPTResolver` class to resolve coreferences using the GPT-3 model. Note that we use "text-davinci-003" as our default model due to performance reasons. You can also pass other models, such as "text-davinci-002" or "GPT3.5" with engine parameter to `resolve_coref` method of the `GPTResolver` class. This would resemble `gpt.resolve_coref(query_to_resolve, engine=your_choice_of_engine)`
 
 ```ruby
 from coreftools.corefresolvers import GPTResolver
 
 resolver = GPTResolver()
 example_query = "My dog is very cute. She loves to play fetch."
 resolved_query = resolver.resolve_coref(example_query)
```

