# Comparing `tmp/gpt4all-j-0.2.3.tar.gz` & `tmp/gpt4all-j-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "gpt4all-j-0.2.3.tar", last modified: Sun Apr 30 11:39:59 2023, max compression
+gzip compressed data, was "gpt4all-j-0.2.4.tar", last modified: Fri May  5 14:01:32 2023, max compression
```

## Comparing `gpt4all-j-0.2.3.tar` & `gpt4all-j-0.2.4.tar`

### file list

```diff
@@ -1,38 +1,39 @@
-drwxr-xr-x   0 ravindra  (1000) ravindra  (1000)        0 2023-04-30 11:39:59.904394 gpt4all-j-0.2.3/
--rw-r--r--   0 ravindra  (1000) ravindra  (1000)     3728 2023-04-30 11:39:59.904394 gpt4all-j-0.2.3/PKG-INFO
--rw-r--r--   0 ravindra  (1000) ravindra  (1000)     2114 2023-04-30 08:12:41.000000 gpt4all-j-0.2.3/README.md
-drwxr-xr-x   0 ravindra  (1000) ravindra  (1000)        0 2023-04-30 11:39:59.874394 gpt4all-j-0.2.3/gpt4all_j.egg-info/
--rw-r--r--   0 ravindra  (1000) ravindra  (1000)     3728 2023-04-30 11:39:59.000000 gpt4all-j-0.2.3/gpt4all_j.egg-info/PKG-INFO
--rw-r--r--   0 ravindra  (1000) ravindra  (1000)      797 2023-04-30 11:39:59.000000 gpt4all-j-0.2.3/gpt4all_j.egg-info/SOURCES.txt
--rw-r--r--   0 ravindra  (1000) ravindra  (1000)        1 2023-04-30 11:39:59.000000 gpt4all-j-0.2.3/gpt4all_j.egg-info/dependency_links.txt
--rw-r--r--   0 ravindra  (1000) ravindra  (1000)        1 2023-04-30 11:39:59.000000 gpt4all-j-0.2.3/gpt4all_j.egg-info/not-zip-safe
--rw-r--r--   0 ravindra  (1000) ravindra  (1000)       16 2023-04-30 11:39:59.000000 gpt4all-j-0.2.3/gpt4all_j.egg-info/requires.txt
--rw-r--r--   0 ravindra  (1000) ravindra  (1000)        9 2023-04-30 11:39:59.000000 gpt4all-j-0.2.3/gpt4all_j.egg-info/top_level.txt
-drwxr-xr-x   0 ravindra  (1000) ravindra  (1000)        0 2023-04-30 11:39:59.874394 gpt4all-j-0.2.3/gpt4allj/
--rw-r--r--   0 ravindra  (1000) ravindra  (1000)       55 2023-04-17 19:06:48.000000 gpt4all-j-0.2.3/gpt4allj/__init__.py
-drwxr-xr-x   0 ravindra  (1000) ravindra  (1000)        0 2023-04-30 11:39:59.874394 gpt4all-j-0.2.3/gpt4allj/lib/
-drwxr-xr-x   0 ravindra  (1000) ravindra  (1000)        0 2023-04-30 11:39:59.884394 gpt4all-j-0.2.3/gpt4allj/lib/avx/
--rw-r--r--   0 ravindra  (1000) ravindra  (1000)   179712 2023-04-30 11:13:00.000000 gpt4all-j-0.2.3/gpt4allj/lib/avx/ggml.dll
--rw-r--r--   0 ravindra  (1000) ravindra  (1000)   162816 2023-04-30 11:13:00.000000 gpt4all-j-0.2.3/gpt4allj/lib/avx/gptj.dll
--rw-r--r--   0 ravindra  (1000) ravindra  (1000)   469802 2023-04-30 11:13:00.000000 gpt4all-j-0.2.3/gpt4allj/lib/avx/libggml.dylib
--rw-r--r--   0 ravindra  (1000) ravindra  (1000)   196248 2023-04-30 11:13:00.000000 gpt4all-j-0.2.3/gpt4allj/lib/avx/libggml.so
--rw-r--r--   0 ravindra  (1000) ravindra  (1000)   381818 2023-04-30 11:13:00.000000 gpt4all-j-0.2.3/gpt4allj/lib/avx/libgptj.dylib
--rw-r--r--   0 ravindra  (1000) ravindra  (1000)   273760 2023-04-30 11:13:00.000000 gpt4all-j-0.2.3/gpt4allj/lib/avx/libgptj.so
-drwxr-xr-x   0 ravindra  (1000) ravindra  (1000)        0 2023-04-30 11:39:59.884394 gpt4all-j-0.2.3/gpt4allj/lib/avx2/
--rw-r--r--   0 ravindra  (1000) ravindra  (1000)   167424 2023-04-30 11:13:00.000000 gpt4all-j-0.2.3/gpt4allj/lib/avx2/ggml.dll
--rw-r--r--   0 ravindra  (1000) ravindra  (1000)   162816 2023-04-30 11:13:00.000000 gpt4all-j-0.2.3/gpt4allj/lib/avx2/gptj.dll
--rw-r--r--   0 ravindra  (1000) ravindra  (1000)   486186 2023-04-30 11:13:00.000000 gpt4all-j-0.2.3/gpt4allj/lib/avx2/libggml.dylib
--rw-r--r--   0 ravindra  (1000) ravindra  (1000)   192152 2023-04-30 11:13:00.000000 gpt4all-j-0.2.3/gpt4allj/lib/avx2/libggml.so
--rw-r--r--   0 ravindra  (1000) ravindra  (1000)   381818 2023-04-30 11:13:00.000000 gpt4all-j-0.2.3/gpt4allj/lib/avx2/libgptj.dylib
--rw-r--r--   0 ravindra  (1000) ravindra  (1000)   273760 2023-04-30 11:13:00.000000 gpt4all-j-0.2.3/gpt4allj/lib/avx2/libgptj.so
-drwxr-xr-x   0 ravindra  (1000) ravindra  (1000)        0 2023-04-30 11:39:59.894394 gpt4all-j-0.2.3/gpt4allj/lib/basic/
--rw-r--r--   0 ravindra  (1000) ravindra  (1000)   173568 2023-04-30 11:13:00.000000 gpt4all-j-0.2.3/gpt4allj/lib/basic/ggml.dll
--rw-r--r--   0 ravindra  (1000) ravindra  (1000)   162816 2023-04-30 11:13:00.000000 gpt4all-j-0.2.3/gpt4allj/lib/basic/gptj.dll
--rw-r--r--   0 ravindra  (1000) ravindra  (1000)   469802 2023-04-30 11:13:00.000000 gpt4all-j-0.2.3/gpt4allj/lib/basic/libggml.dylib
--rw-r--r--   0 ravindra  (1000) ravindra  (1000)   171672 2023-04-30 11:13:00.000000 gpt4all-j-0.2.3/gpt4allj/lib/basic/libggml.so
--rw-r--r--   0 ravindra  (1000) ravindra  (1000)   381818 2023-04-30 11:13:00.000000 gpt4all-j-0.2.3/gpt4allj/lib/basic/libgptj.dylib
--rw-r--r--   0 ravindra  (1000) ravindra  (1000)   273760 2023-04-30 11:13:00.000000 gpt4all-j-0.2.3/gpt4allj/lib/basic/libgptj.so
--rw-r--r--   0 ravindra  (1000) ravindra  (1000)     2071 2023-04-30 10:39:23.000000 gpt4all-j-0.2.3/gpt4allj/lib.py
--rw-r--r--   0 ravindra  (1000) ravindra  (1000)     2004 2023-04-30 10:40:17.000000 gpt4all-j-0.2.3/gpt4allj/model.py
--rw-r--r--   0 ravindra  (1000) ravindra  (1000)       38 2023-04-30 11:39:59.904394 gpt4all-j-0.2.3/setup.cfg
--rw-r--r--   0 ravindra  (1000) ravindra  (1000)     1396 2023-04-30 11:25:32.000000 gpt4all-j-0.2.3/setup.py
+drwxr-xr-x   0 ravindra  (1000) ravindra  (1000)        0 2023-05-05 14:01:32.046027 gpt4all-j-0.2.4/
+-rw-r--r--   0 ravindra  (1000) ravindra  (1000)     5273 2023-05-05 14:01:32.046027 gpt4all-j-0.2.4/PKG-INFO
+-rw-r--r--   0 ravindra  (1000) ravindra  (1000)     3267 2023-05-04 21:59:11.000000 gpt4all-j-0.2.4/README.md
+drwxr-xr-x   0 ravindra  (1000) ravindra  (1000)        0 2023-05-05 14:01:32.006027 gpt4all-j-0.2.4/gpt4all_j.egg-info/
+-rw-r--r--   0 ravindra  (1000) ravindra  (1000)     5273 2023-05-05 14:01:31.000000 gpt4all-j-0.2.4/gpt4all_j.egg-info/PKG-INFO
+-rw-r--r--   0 ravindra  (1000) ravindra  (1000)      819 2023-05-05 14:01:31.000000 gpt4all-j-0.2.4/gpt4all_j.egg-info/SOURCES.txt
+-rw-r--r--   0 ravindra  (1000) ravindra  (1000)        1 2023-05-05 14:01:31.000000 gpt4all-j-0.2.4/gpt4all_j.egg-info/dependency_links.txt
+-rw-r--r--   0 ravindra  (1000) ravindra  (1000)        1 2023-05-05 14:01:31.000000 gpt4all-j-0.2.4/gpt4all_j.egg-info/not-zip-safe
+-rw-r--r--   0 ravindra  (1000) ravindra  (1000)       16 2023-05-05 14:01:31.000000 gpt4all-j-0.2.4/gpt4all_j.egg-info/requires.txt
+-rw-r--r--   0 ravindra  (1000) ravindra  (1000)        9 2023-05-05 14:01:31.000000 gpt4all-j-0.2.4/gpt4all_j.egg-info/top_level.txt
+drwxr-xr-x   0 ravindra  (1000) ravindra  (1000)        0 2023-05-05 14:01:32.006027 gpt4all-j-0.2.4/gpt4allj/
+-rw-r--r--   0 ravindra  (1000) ravindra  (1000)       55 2023-04-17 19:06:48.000000 gpt4all-j-0.2.4/gpt4allj/__init__.py
+-rw-r--r--   0 ravindra  (1000) ravindra  (1000)     2529 2023-05-05 13:39:21.000000 gpt4all-j-0.2.4/gpt4allj/langchain.py
+drwxr-xr-x   0 ravindra  (1000) ravindra  (1000)        0 2023-05-05 14:01:32.006027 gpt4all-j-0.2.4/gpt4allj/lib/
+drwxr-xr-x   0 ravindra  (1000) ravindra  (1000)        0 2023-05-05 14:01:32.016027 gpt4all-j-0.2.4/gpt4allj/lib/avx/
+-rw-r--r--   0 ravindra  (1000) ravindra  (1000)   179712 2023-05-05 13:26:30.000000 gpt4all-j-0.2.4/gpt4allj/lib/avx/ggml.dll
+-rw-r--r--   0 ravindra  (1000) ravindra  (1000)   162816 2023-05-05 13:26:30.000000 gpt4all-j-0.2.4/gpt4allj/lib/avx/gptj.dll
+-rw-r--r--   0 ravindra  (1000) ravindra  (1000)   469802 2023-05-05 13:26:30.000000 gpt4all-j-0.2.4/gpt4allj/lib/avx/libggml.dylib
+-rw-r--r--   0 ravindra  (1000) ravindra  (1000)   196248 2023-05-05 13:26:30.000000 gpt4all-j-0.2.4/gpt4allj/lib/avx/libggml.so
+-rw-r--r--   0 ravindra  (1000) ravindra  (1000)   381818 2023-05-05 13:26:30.000000 gpt4all-j-0.2.4/gpt4allj/lib/avx/libgptj.dylib
+-rw-r--r--   0 ravindra  (1000) ravindra  (1000)   273760 2023-05-05 13:26:30.000000 gpt4all-j-0.2.4/gpt4allj/lib/avx/libgptj.so
+drwxr-xr-x   0 ravindra  (1000) ravindra  (1000)        0 2023-05-05 14:01:32.026027 gpt4all-j-0.2.4/gpt4allj/lib/avx2/
+-rw-r--r--   0 ravindra  (1000) ravindra  (1000)   167424 2023-05-05 13:26:30.000000 gpt4all-j-0.2.4/gpt4allj/lib/avx2/ggml.dll
+-rw-r--r--   0 ravindra  (1000) ravindra  (1000)   162816 2023-05-05 13:26:30.000000 gpt4all-j-0.2.4/gpt4allj/lib/avx2/gptj.dll
+-rw-r--r--   0 ravindra  (1000) ravindra  (1000)   486186 2023-05-05 13:26:30.000000 gpt4all-j-0.2.4/gpt4allj/lib/avx2/libggml.dylib
+-rw-r--r--   0 ravindra  (1000) ravindra  (1000)   192152 2023-05-05 13:26:30.000000 gpt4all-j-0.2.4/gpt4allj/lib/avx2/libggml.so
+-rw-r--r--   0 ravindra  (1000) ravindra  (1000)   381818 2023-05-05 13:26:30.000000 gpt4all-j-0.2.4/gpt4allj/lib/avx2/libgptj.dylib
+-rw-r--r--   0 ravindra  (1000) ravindra  (1000)   273760 2023-05-05 13:26:30.000000 gpt4all-j-0.2.4/gpt4allj/lib/avx2/libgptj.so
+drwxr-xr-x   0 ravindra  (1000) ravindra  (1000)        0 2023-05-05 14:01:32.046027 gpt4all-j-0.2.4/gpt4allj/lib/basic/
+-rw-r--r--   0 ravindra  (1000) ravindra  (1000)   173568 2023-05-05 13:26:30.000000 gpt4all-j-0.2.4/gpt4allj/lib/basic/ggml.dll
+-rw-r--r--   0 ravindra  (1000) ravindra  (1000)   162816 2023-05-05 13:26:30.000000 gpt4all-j-0.2.4/gpt4allj/lib/basic/gptj.dll
+-rw-r--r--   0 ravindra  (1000) ravindra  (1000)   469802 2023-05-05 13:26:30.000000 gpt4all-j-0.2.4/gpt4allj/lib/basic/libggml.dylib
+-rw-r--r--   0 ravindra  (1000) ravindra  (1000)   171672 2023-05-05 13:26:30.000000 gpt4all-j-0.2.4/gpt4allj/lib/basic/libggml.so
+-rw-r--r--   0 ravindra  (1000) ravindra  (1000)   381818 2023-05-05 13:26:30.000000 gpt4all-j-0.2.4/gpt4allj/lib/basic/libgptj.dylib
+-rw-r--r--   0 ravindra  (1000) ravindra  (1000)   273760 2023-05-05 13:26:30.000000 gpt4all-j-0.2.4/gpt4allj/lib/basic/libgptj.so
+-rw-r--r--   0 ravindra  (1000) ravindra  (1000)     2071 2023-04-30 10:39:23.000000 gpt4all-j-0.2.4/gpt4allj/lib.py
+-rw-r--r--   0 ravindra  (1000) ravindra  (1000)     1906 2023-05-04 19:31:59.000000 gpt4all-j-0.2.4/gpt4allj/model.py
+-rw-r--r--   0 ravindra  (1000) ravindra  (1000)       38 2023-05-05 14:01:32.046027 gpt4all-j-0.2.4/setup.cfg
+-rw-r--r--   0 ravindra  (1000) ravindra  (1000)     1396 2023-05-05 13:47:00.000000 gpt4all-j-0.2.4/setup.py
```

### Comparing `gpt4all-j-0.2.3/README.md` & `gpt4all-j-0.2.4/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 
 ## Installation
 
 ```sh
 pip install gpt4all-j
 ```
 
-Download the model from [here](https://gpt4all.io/models/ggml-gpt4all-j.bin).
+Download the model from [here](https://gpt4all.io/models/ggml-gpt4all-j-v1.3-groovy.bin).
 
 ## Usage
 
 ```py
 from gpt4allj import Model
 
 model = Model('/path/to/ggml-gpt4all-j.bin')
@@ -36,32 +36,81 @@
 model.generate(prompt,
                seed=-1,
                n_threads=-1,
                n_predict=200,
                top_k=40,
                top_p=0.9,
                temp=0.9,
-               n_batch=8,
                repeat_penalty=1.0,
                repeat_last_n=64,
+               n_batch=8,
                callback=None)
 ```
 
-### `callback`
+#### `callback`
 
-If a callback function is passed to `model.generate()`, it will be called once per each generated token. To stop generating more tokens, return `False` inside the callback function.
+If a callback function is passed, it will be called once per each generated token. To stop generating more tokens, return `False` inside the callback function.
 
 ```py
 def callback(token):
     print(token)
 
 model.generate('AI is going to', callback=callback)
 ```
 
-### C++ Library
+## LangChain
+
+[LangChain](https://python.langchain.com/) is a framework for developing applications powered by language models. A LangChain LLM object for the GPT4All-J model can be created using:
+
+```py
+from gpt4allj.langchain import GPT4AllJ
+
+llm = GPT4AllJ(model='/path/to/ggml-gpt4all-j.bin')
+
+print(llm('AI is going to'))
+```
+
+If you are getting `illegal instruction` error, try using `instructions='avx'` or `instructions='basic'`:
+
+```py
+llm = GPT4AllJ(model='/path/to/ggml-gpt4all-j.bin', instructions='avx')
+```
+
+It can be used with other LangChain modules:
+
+```py
+from langchain import PromptTemplate, LLMChain
+
+template = """Question: {question}
+
+Answer:"""
+
+prompt = PromptTemplate(template=template, input_variables=['question'])
+
+llm_chain = LLMChain(prompt=prompt, llm=llm)
+
+print(llm_chain.run('What is AI?'))
+```
+
+### Parameters
+
+```py
+llm = GPT4AllJ(model='/path/to/ggml-gpt4all-j.bin',
+               seed=-1,
+               n_threads=-1,
+               n_predict=200,
+               top_k=40,
+               top_p=0.9,
+               temp=0.9,
+               repeat_penalty=1.0,
+               repeat_last_n=64,
+               n_batch=8)
+```
+
+## C++ Library
 
 To build the C++ library from source, please see [gptj.cpp][gptj.cpp]. Once you have built the shared libraries, you can use them as:
 
 ```py
 from gpt4allj import Model, load_library
 
 lib = load_library('/path/to/libgptj.so', '/path/to/libggml.so')
```

### Comparing `gpt4all-j-0.2.3/gpt4all_j.egg-info/SOURCES.txt` & `gpt4all-j-0.2.4/gpt4all_j.egg-info/SOURCES.txt`

 * *Files 2% similar despite different names*

```diff
@@ -3,14 +3,15 @@
 gpt4all_j.egg-info/PKG-INFO
 gpt4all_j.egg-info/SOURCES.txt
 gpt4all_j.egg-info/dependency_links.txt
 gpt4all_j.egg-info/not-zip-safe
 gpt4all_j.egg-info/requires.txt
 gpt4all_j.egg-info/top_level.txt
 gpt4allj/__init__.py
+gpt4allj/langchain.py
 gpt4allj/lib.py
 gpt4allj/model.py
 gpt4allj/lib/avx/ggml.dll
 gpt4allj/lib/avx/gptj.dll
 gpt4allj/lib/avx/libggml.dylib
 gpt4allj/lib/avx/libggml.so
 gpt4allj/lib/avx/libgptj.dylib
```

### Comparing `gpt4all-j-0.2.3/gpt4allj/lib/avx/ggml.dll` & `gpt4all-j-0.2.4/gpt4allj/lib/avx/ggml.dll`

 * *Files identical despite different names*

### Comparing `gpt4all-j-0.2.3/gpt4allj/lib/avx/gptj.dll` & `gpt4all-j-0.2.4/gpt4allj/lib/avx/gptj.dll`

 * *Files identical despite different names*

### Comparing `gpt4all-j-0.2.3/gpt4allj/lib/avx/libggml.dylib` & `gpt4all-j-0.2.4/gpt4allj/lib/avx/libggml.dylib`

 * *Files identical despite different names*

### Comparing `gpt4all-j-0.2.3/gpt4allj/lib/avx/libggml.so` & `gpt4all-j-0.2.4/gpt4allj/lib/avx/libggml.so`

 * *Files identical despite different names*

### Comparing `gpt4all-j-0.2.3/gpt4allj/lib/avx/libgptj.dylib` & `gpt4all-j-0.2.4/gpt4allj/lib/avx/libgptj.dylib`

 * *Files identical despite different names*

### Comparing `gpt4all-j-0.2.3/gpt4allj/lib/avx/libgptj.so` & `gpt4all-j-0.2.4/gpt4allj/lib/avx/libgptj.so`

 * *Files identical despite different names*

### Comparing `gpt4all-j-0.2.3/gpt4allj/lib/avx2/ggml.dll` & `gpt4all-j-0.2.4/gpt4allj/lib/avx2/ggml.dll`

 * *Files identical despite different names*

### Comparing `gpt4all-j-0.2.3/gpt4allj/lib/avx2/gptj.dll` & `gpt4all-j-0.2.4/gpt4allj/lib/avx2/gptj.dll`

 * *Files identical despite different names*

### Comparing `gpt4all-j-0.2.3/gpt4allj/lib/avx2/libggml.dylib` & `gpt4all-j-0.2.4/gpt4allj/lib/avx2/libggml.dylib`

 * *Files identical despite different names*

### Comparing `gpt4all-j-0.2.3/gpt4allj/lib/avx2/libggml.so` & `gpt4all-j-0.2.4/gpt4allj/lib/avx2/libggml.so`

 * *Files identical despite different names*

### Comparing `gpt4all-j-0.2.3/gpt4allj/lib/avx2/libgptj.dylib` & `gpt4all-j-0.2.4/gpt4allj/lib/avx2/libgptj.dylib`

 * *Files identical despite different names*

### Comparing `gpt4all-j-0.2.3/gpt4allj/lib/avx2/libgptj.so` & `gpt4all-j-0.2.4/gpt4allj/lib/avx2/libgptj.so`

 * *Files identical despite different names*

### Comparing `gpt4all-j-0.2.3/gpt4allj/lib/basic/ggml.dll` & `gpt4all-j-0.2.4/gpt4allj/lib/basic/ggml.dll`

 * *Files identical despite different names*

### Comparing `gpt4all-j-0.2.3/gpt4allj/lib/basic/gptj.dll` & `gpt4all-j-0.2.4/gpt4allj/lib/basic/gptj.dll`

 * *Files identical despite different names*

### Comparing `gpt4all-j-0.2.3/gpt4allj/lib/basic/libggml.dylib` & `gpt4all-j-0.2.4/gpt4allj/lib/basic/libggml.dylib`

 * *Files identical despite different names*

### Comparing `gpt4all-j-0.2.3/gpt4allj/lib/basic/libggml.so` & `gpt4all-j-0.2.4/gpt4allj/lib/basic/libggml.so`

 * *Files identical despite different names*

### Comparing `gpt4all-j-0.2.3/gpt4allj/lib/basic/libgptj.dylib` & `gpt4all-j-0.2.4/gpt4allj/lib/basic/libgptj.dylib`

 * *Files identical despite different names*

### Comparing `gpt4all-j-0.2.3/gpt4allj/lib/basic/libgptj.so` & `gpt4all-j-0.2.4/gpt4allj/lib/basic/libgptj.so`

 * *Files identical despite different names*

### Comparing `gpt4all-j-0.2.3/gpt4allj/lib.py` & `gpt4all-j-0.2.4/gpt4allj/lib.py`

 * *Files identical despite different names*

### Comparing `gpt4all-j-0.2.3/gpt4allj/model.py` & `gpt4all-j-0.2.4/gpt4allj/model.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-from ctypes import create_string_buffer
-
 from .lib import load_library, gptj_params, gptj_generate_callback_t
 
 
 class Model:
 
     def __init__(self, model, lib=None, instructions=None):
         self._ctx = None
@@ -30,29 +28,27 @@
                              n_predict=n_predict,
                              top_k=top_k,
                              top_p=top_p,
                              temp=temp,
                              repeat_penalty=repeat_penalty,
                              repeat_last_n=repeat_last_n,
                              n_batch=n_batch)
+        callback = callback or (lambda token: True)
         response = []
 
         @gptj_generate_callback_t
         def cb(token):
             token = token.decode()
-            if callback:
-                return callback(token) is not False
-            else:
-                response.append(token)
-                return True
+            response.append(token)
+            return callback(token) is not False
 
         status = self._lib.gptj_generate(self._ctx, prompt, params, cb)
         if not status:
             raise RuntimeError(f'Failed to generate response for "{prompt}"')
-        return ''.join(response) if callback is None else None
+        return ''.join(response)
 
     def num_tokens(self, prompt):
         prompt = prompt.encode()
         return self._lib.gptj_num_tokens(self._ctx, prompt)
 
     def __del__(self):
         if self._ctx is not None:
```

### Comparing `gpt4all-j-0.2.3/setup.py` & `gpt4all-j-0.2.4/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 with open('README.md') as f:
     long_description = f.read()
 
 name = 'gpt4all-j'
 
 setup(
     name=name,
-    version='0.2.3',
+    version='0.2.4',
     description='Python bindings for the C++ port of GPT4All-J model.',
     long_description=long_description,
     long_description_content_type='text/markdown',
     author='Ravindra Marella',
     author_email='mv.ravindra007@gmail.com',
     url='https://github.com/marella/{}'.format(name),
     license='MIT',
```

