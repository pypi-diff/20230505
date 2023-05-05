# Comparing `tmp/vectorGPTBot-0.1.5.tar.gz` & `tmp/vectorGPTBot-0.1.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vectorGPTBot-0.1.5.tar", last modified: Thu May  4 17:29:55 2023, max compression
+gzip compressed data, was "vectorGPTBot-0.1.6.tar", last modified: Fri May  5 14:11:09 2023, max compression
```

## Comparing `vectorGPTBot-0.1.5.tar` & `vectorGPTBot-0.1.6.tar`

### file list

```diff
@@ -1,13 +1,13 @@
-drwxrwxrwx   0     1000     1000        0 2023-05-04 17:29:55.151923 vectorGPTBot-0.1.5/
--rwxrwxrwx   0     1000     1000      782 2023-05-04 17:29:55.148430 vectorGPTBot-0.1.5/PKG-INFO
--rwxrwxrwx   0     1000     1000       38 2023-05-04 17:29:55.153922 vectorGPTBot-0.1.5/setup.cfg
--rwxrwxrwx   0     1000     1000      989 2023-05-04 17:29:11.000000 vectorGPTBot-0.1.5/setup.py
-drwxrwxrwx   0     1000     1000        0 2023-05-04 17:29:54.968970 vectorGPTBot-0.1.5/vectorGPTBot/
--rwxrwxrwx   0     1000     1000        0 2023-05-04 15:22:50.000000 vectorGPTBot-0.1.5/vectorGPTBot/__init__.py
--rwxrwxrwx   0     1000     1000     3594 2023-05-04 17:22:43.000000 vectorGPTBot-0.1.5/vectorGPTBot/vectorGPTBot.py
-drwxrwxrwx   0     1000     1000        0 2023-05-04 17:29:55.106864 vectorGPTBot-0.1.5/vectorGPTBot.egg-info/
--rwxrwxrwx   0     1000     1000      782 2023-05-04 17:29:54.000000 vectorGPTBot-0.1.5/vectorGPTBot.egg-info/PKG-INFO
--rwxrwxrwx   0     1000     1000      241 2023-05-04 17:29:54.000000 vectorGPTBot-0.1.5/vectorGPTBot.egg-info/SOURCES.txt
--rwxrwxrwx   0     1000     1000        1 2023-05-04 17:29:54.000000 vectorGPTBot-0.1.5/vectorGPTBot.egg-info/dependency_links.txt
--rwxrwxrwx   0     1000     1000       33 2023-05-04 17:29:54.000000 vectorGPTBot-0.1.5/vectorGPTBot.egg-info/requires.txt
--rwxrwxrwx   0     1000     1000       13 2023-05-04 17:29:54.000000 vectorGPTBot-0.1.5/vectorGPTBot.egg-info/top_level.txt
+drwxrwxrwx   0     1000     1000        0 2023-05-05 14:11:09.254524 vectorGPTBot-0.1.6/
+-rwxrwxrwx   0     1000     1000      782 2023-05-05 14:11:09.254524 vectorGPTBot-0.1.6/PKG-INFO
+-rwxrwxrwx   0     1000     1000       38 2023-05-05 14:11:09.270163 vectorGPTBot-0.1.6/setup.cfg
+-rwxrwxrwx   0     1000     1000     1012 2023-05-05 14:10:24.000000 vectorGPTBot-0.1.6/setup.py
+drwxrwxrwx   0     1000     1000        0 2023-05-05 14:11:09.064929 vectorGPTBot-0.1.6/vectorGPTBot/
+-rwxrwxrwx   0     1000     1000        0 2023-05-04 15:22:50.000000 vectorGPTBot-0.1.6/vectorGPTBot/__init__.py
+-rwxrwxrwx   0     1000     1000     3783 2023-05-05 14:07:18.000000 vectorGPTBot-0.1.6/vectorGPTBot/vectorGPTBot.py
+drwxrwxrwx   0     1000     1000        0 2023-05-05 14:11:09.218792 vectorGPTBot-0.1.6/vectorGPTBot.egg-info/
+-rwxrwxrwx   0     1000     1000      782 2023-05-05 14:11:08.000000 vectorGPTBot-0.1.6/vectorGPTBot.egg-info/PKG-INFO
+-rwxrwxrwx   0     1000     1000      241 2023-05-05 14:11:08.000000 vectorGPTBot-0.1.6/vectorGPTBot.egg-info/SOURCES.txt
+-rwxrwxrwx   0     1000     1000        1 2023-05-05 14:11:08.000000 vectorGPTBot-0.1.6/vectorGPTBot.egg-info/dependency_links.txt
+-rwxrwxrwx   0     1000     1000       45 2023-05-05 14:11:08.000000 vectorGPTBot-0.1.6/vectorGPTBot.egg-info/requires.txt
+-rwxrwxrwx   0     1000     1000       13 2023-05-05 14:11:08.000000 vectorGPTBot-0.1.6/vectorGPTBot.egg-info/top_level.txt
```

### Comparing `vectorGPTBot-0.1.5/PKG-INFO` & `vectorGPTBot-0.1.6/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vectorGPTBot
-Version: 0.1.5
+Version: 0.1.6
 Summary: A sample vectorGPTBot
 Home-page: UNKNOWN
 Author: wstart
 License: Apache License 2.0
 Keywords: vectorGPTBot
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
```

### Comparing `vectorGPTBot-0.1.5/setup.py` & `vectorGPTBot-0.1.6/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 from setuptools import setup, find_packages
 
 setup(
     name='vectorGPTBot',
-    version='0.1.5',
+    version='0.1.6',
     author='wstart',
     description='A sample vectorGPTBot',
     long_description='A sample vectorGPTBot',
     long_description_content_type="text/markdown",
     packages=find_packages(),
     install_requires=[
         'chromadb',
         'modelscope',
-        'transformers'
+        'transformers',
+        'cpm_kernels'
     ],
     classifiers=[
         'Development Status :: 3 - Alpha',
         'Intended Audience :: Developers',
         'License :: OSI Approved :: MIT License',
         'Programming Language :: Python :: 3',
         'Programming Language :: Python :: 3.6',
```

### Comparing `vectorGPTBot-0.1.5/vectorGPTBot/vectorGPTBot.py` & `vectorGPTBot-0.1.6/vectorGPTBot/vectorGPTBot.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,46 +1,63 @@
 import chromadb
 from transformers import AutoTokenizer, AutoModel
 from modelscope.models import Model
 from modelscope.pipelines import pipeline
 from modelscope.utils.constant import Tasks
 from chromadb.config import Settings
 
+import chromadb
+from transformers import AutoTokenizer, AutoModel
+from modelscope.models import Model
+from modelscope.pipelines import pipeline
+from modelscope.utils.constant import Tasks
+from chromadb.config import Settings
+        
+ 
+        
 
 class mainClass():
-    def __init__(self,file_pah,model_path="THUDM/chatglm-6b"):
-        model_id = "damo/nlp_corom_sentence-embedding_chinese-base"
-        self.pipeline_se = pipeline(Tasks.sentence_embedding,
-                       model=model_id)
+    def __init__(self,file_pah,
+                 textvetor_model_id="damo/nlp_corom_sentence-embedding_chinese-base",
+                 llm_model_id='ZhipuAI/ChatGLM-6B',
+                ):
+        
+        self.pipeline_textvetor = pipeline(Tasks.sentence_embedding,
+                       model=textvetor_model_id)
+        
+        self.pipeline_llm = pipeline(task=Tasks.chat, 
+                                     model=llm_model_id,)
             
-        self.tokenizer = AutoTokenizer.from_pretrained(model_path, trust_remote_code=True)
-        self.model = AutoModel.from_pretrained(model_path, trust_remote_code=True).half().cuda()
+       
         self.client = chromadb.Client(Settings(
             chroma_db_impl="duckdb+parquet",
             anonymized_telemetry=False,
             persist_directory=file_pah # Optional, defaults to .chromadb/ in the current directory
         ))
         self.db = self.client.get_or_create_collection('miandb') 
         pass
 
+    
+    
     def chatsss(self,text):
-        response, history = self.model.chat(self.tokenizer,
-                                    text,
-                                    history=[],
-                                    max_length= 2048,
-                                    top_p= 0.999,
-                                    temperature= 0.001)
+        response = self.pipeline_llm({
+            'text':text, 
+            'history': [],   
+            'top_p':0.999,
+              'temperature':0.001
+        })
+        #print(response)
         return response
 
     def vetor_db(self,db,input_text,ids):
         inputs = {
                 "source_sentence": input_text
             }
 
-        result = self.pipeline_se(input=inputs)
+        result = self.pipeline_textvetor(input=inputs)
         self.db.add(
             embeddings=result['text_embedding'].tolist(),
             documents=input_text,
             ids=ids
         ) 
 
     def put_data(self,text_list):
@@ -78,23 +95,23 @@
 
     """
         #print(qa)
         result = self.chatsss(qa)
         #print('接入知识库后回答：',result)
         #print('==============')
         #print('接入知识库前回答：',chatsss(src_qa))
-        return result
+        return result['response']
 
     def __query_data(self,text):
         db= self.db
         input_text = [ text ]
         inputs = {
                 "source_sentence": input_text
             }
-        result = self.pipeline_se(input=inputs)
+        result = self.pipeline_textvetor(input=inputs)
         
         result = db.query(
             query_embeddings=result['text_embedding'].tolist()
             ,n_results=5
         )
         return result
```

### Comparing `vectorGPTBot-0.1.5/vectorGPTBot.egg-info/PKG-INFO` & `vectorGPTBot-0.1.6/vectorGPTBot.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vectorGPTBot
-Version: 0.1.5
+Version: 0.1.6
 Summary: A sample vectorGPTBot
 Home-page: UNKNOWN
 Author: wstart
 License: Apache License 2.0
 Keywords: vectorGPTBot
 Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
```

