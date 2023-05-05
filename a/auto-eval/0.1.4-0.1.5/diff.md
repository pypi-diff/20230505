# Comparing `tmp/auto-eval-0.1.4.tar.gz` & `tmp/auto-eval-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "auto-eval-0.1.4.tar", last modified: Fri May  5 09:01:52 2023, max compression
+gzip compressed data, was "auto-eval-0.1.5.tar", last modified: Fri May  5 09:52:56 2023, max compression
```

## Comparing `auto-eval-0.1.4.tar` & `auto-eval-0.1.5.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 zhangchong   (501) staff       (20)        0 2023-05-05 09:01:52.662127 auto-eval-0.1.4/
--rw-r--r--   0 zhangchong   (501) staff       (20)     1071 2023-04-28 07:53:45.000000 auto-eval-0.1.4/LICENSE
--rw-r--r--   0 zhangchong   (501) staff       (20)    11479 2023-05-05 09:01:52.661918 auto-eval-0.1.4/PKG-INFO
--rw-r--r--   0 zhangchong   (501) staff       (20)    11053 2023-05-05 08:55:21.000000 auto-eval-0.1.4/README.md
-drwxr-xr-x   0 zhangchong   (501) staff       (20)        0 2023-05-05 09:01:52.659087 auto-eval-0.1.4/auto_eval.egg-info/
--rw-r--r--   0 zhangchong   (501) staff       (20)    11479 2023-05-05 09:01:52.000000 auto-eval-0.1.4/auto_eval.egg-info/PKG-INFO
--rw-r--r--   0 zhangchong   (501) staff       (20)      445 2023-05-05 09:01:52.000000 auto-eval-0.1.4/auto_eval.egg-info/SOURCES.txt
--rw-r--r--   0 zhangchong   (501) staff       (20)        1 2023-05-05 09:01:52.000000 auto-eval-0.1.4/auto_eval.egg-info/dependency_links.txt
--rw-r--r--   0 zhangchong   (501) staff       (20)       54 2023-05-05 09:01:52.000000 auto-eval-0.1.4/auto_eval.egg-info/entry_points.txt
--rw-r--r--   0 zhangchong   (501) staff       (20)       49 2023-05-05 09:01:52.000000 auto-eval-0.1.4/auto_eval.egg-info/requires.txt
--rw-r--r--   0 zhangchong   (501) staff       (20)       36 2023-05-05 09:01:52.000000 auto-eval-0.1.4/auto_eval.egg-info/top_level.txt
-drwxr-xr-x   0 zhangchong   (501) staff       (20)        0 2023-05-05 09:01:52.659489 auto-eval-0.1.4/commands/
--rw-r--r--   0 zhangchong   (501) staff       (20)        0 2023-04-28 08:32:15.000000 auto-eval-0.1.4/commands/__init__.py
--rw-r--r--   0 zhangchong   (501) staff       (20)     3909 2023-05-05 08:12:59.000000 auto-eval-0.1.4/commands/auto_eval.py
-drwxr-xr-x   0 zhangchong   (501) staff       (20)        0 2023-05-05 09:01:52.660141 auto-eval-0.1.4/eval/
--rw-r--r--   0 zhangchong   (501) staff       (20)      131 2023-05-05 08:11:08.000000 auto-eval-0.1.4/eval/__init__.py
--rw-r--r--   0 zhangchong   (501) staff       (20)     7071 2023-05-05 08:56:41.000000 auto-eval-0.1.4/eval/auto_llms_eval.py
-drwxr-xr-x   0 zhangchong   (501) staff       (20)        0 2023-05-05 09:01:52.660845 auto-eval-0.1.4/prompt_template/
--rw-r--r--   0 zhangchong   (501) staff       (20)       44 2023-05-05 07:40:16.000000 auto-eval-0.1.4/prompt_template/__init__.py
--rw-r--r--   0 zhangchong   (501) staff       (20)      773 2023-05-05 07:29:57.000000 auto-eval-0.1.4/prompt_template/eval_prompt_template.json
--rw-r--r--   0 zhangchong   (501) staff       (20)     2948 2023-05-05 08:21:30.000000 auto-eval-0.1.4/prompt_template/prompter.py
--rw-r--r--   0 zhangchong   (501) staff       (20)       38 2023-05-05 09:01:52.662178 auto-eval-0.1.4/setup.cfg
--rw-r--r--   0 zhangchong   (501) staff       (20)      940 2023-05-05 08:58:28.000000 auto-eval-0.1.4/setup.py
-drwxr-xr-x   0 zhangchong   (501) staff       (20)        0 2023-05-05 09:01:52.661445 auto-eval-0.1.4/utils/
--rw-r--r--   0 zhangchong   (501) staff       (20)       26 2023-04-28 09:40:19.000000 auto-eval-0.1.4/utils/__init__.py
--rw-r--r--   0 zhangchong   (501) staff       (20)     2832 2023-05-04 04:56:04.000000 auto-eval-0.1.4/utils/data_utils.py
+drwxr-xr-x   0 zhangchong   (501) staff       (20)        0 2023-05-05 09:52:56.353049 auto-eval-0.1.5/
+-rw-r--r--   0 zhangchong   (501) staff       (20)     1071 2023-04-28 07:53:45.000000 auto-eval-0.1.5/LICENSE
+-rw-r--r--   0 zhangchong   (501) staff       (20)    11478 2023-05-05 09:52:56.352689 auto-eval-0.1.5/PKG-INFO
+-rw-r--r--   0 zhangchong   (501) staff       (20)    11052 2023-05-05 09:05:05.000000 auto-eval-0.1.5/README.md
+drwxr-xr-x   0 zhangchong   (501) staff       (20)        0 2023-05-05 09:52:56.347443 auto-eval-0.1.5/auto_eval.egg-info/
+-rw-r--r--   0 zhangchong   (501) staff       (20)    11478 2023-05-05 09:52:56.000000 auto-eval-0.1.5/auto_eval.egg-info/PKG-INFO
+-rw-r--r--   0 zhangchong   (501) staff       (20)      445 2023-05-05 09:52:56.000000 auto-eval-0.1.5/auto_eval.egg-info/SOURCES.txt
+-rw-r--r--   0 zhangchong   (501) staff       (20)        1 2023-05-05 09:52:56.000000 auto-eval-0.1.5/auto_eval.egg-info/dependency_links.txt
+-rw-r--r--   0 zhangchong   (501) staff       (20)       54 2023-05-05 09:52:56.000000 auto-eval-0.1.5/auto_eval.egg-info/entry_points.txt
+-rw-r--r--   0 zhangchong   (501) staff       (20)       49 2023-05-05 09:52:56.000000 auto-eval-0.1.5/auto_eval.egg-info/requires.txt
+-rw-r--r--   0 zhangchong   (501) staff       (20)       36 2023-05-05 09:52:56.000000 auto-eval-0.1.5/auto_eval.egg-info/top_level.txt
+drwxr-xr-x   0 zhangchong   (501) staff       (20)        0 2023-05-05 09:52:56.347947 auto-eval-0.1.5/commands/
+-rw-r--r--   0 zhangchong   (501) staff       (20)        0 2023-04-28 08:32:15.000000 auto-eval-0.1.5/commands/__init__.py
+-rw-r--r--   0 zhangchong   (501) staff       (20)     3909 2023-05-05 08:12:59.000000 auto-eval-0.1.5/commands/auto_eval.py
+drwxr-xr-x   0 zhangchong   (501) staff       (20)        0 2023-05-05 09:52:56.349718 auto-eval-0.1.5/eval/
+-rw-r--r--   0 zhangchong   (501) staff       (20)      131 2023-05-05 08:11:08.000000 auto-eval-0.1.5/eval/__init__.py
+-rw-r--r--   0 zhangchong   (501) staff       (20)     7003 2023-05-05 09:26:08.000000 auto-eval-0.1.5/eval/auto_llms_eval.py
+drwxr-xr-x   0 zhangchong   (501) staff       (20)        0 2023-05-05 09:52:56.351443 auto-eval-0.1.5/prompt_template/
+-rw-r--r--   0 zhangchong   (501) staff       (20)       44 2023-05-05 07:40:16.000000 auto-eval-0.1.5/prompt_template/__init__.py
+-rw-r--r--   0 zhangchong   (501) staff       (20)      773 2023-05-05 07:29:57.000000 auto-eval-0.1.5/prompt_template/eval_prompt_template.json
+-rw-r--r--   0 zhangchong   (501) staff       (20)     2948 2023-05-05 08:21:30.000000 auto-eval-0.1.5/prompt_template/prompter.py
+-rw-r--r--   0 zhangchong   (501) staff       (20)       38 2023-05-05 09:52:56.353126 auto-eval-0.1.5/setup.cfg
+-rw-r--r--   0 zhangchong   (501) staff       (20)      940 2023-05-05 09:52:44.000000 auto-eval-0.1.5/setup.py
+drwxr-xr-x   0 zhangchong   (501) staff       (20)        0 2023-05-05 09:52:56.352121 auto-eval-0.1.5/utils/
+-rw-r--r--   0 zhangchong   (501) staff       (20)       26 2023-04-28 09:40:19.000000 auto-eval-0.1.5/utils/__init__.py
+-rw-r--r--   0 zhangchong   (501) staff       (20)     2911 2023-05-05 09:52:25.000000 auto-eval-0.1.5/utils/data_utils.py
```

### Comparing `auto-eval-0.1.4/LICENSE` & `auto-eval-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `auto-eval-0.1.4/PKG-INFO` & `auto-eval-0.1.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: auto-eval
-Version: 0.1.4
+Version: 0.1.5
 Summary: Using only one line of commmands to evaluate multiple models
 Home-page: https://github.com/muximus3/Auto-Eval
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
@@ -53,15 +53,15 @@
 {
     "api_key": "YOUR_API_KEY",
     "api": "https://api.anthropic.com",
     "api_type": "claude"
 }
 ```
 
-### 2. Use with command lines
+### 2. Usage with command lines
 #### Evaluate one sample
 ```sh
 auto-eval line --config_file CHANGE_TO_YOUR_CONFIG_PATH \
 --model gpt-3.5-turbo \
 --prompt "Janet’s ducks lay 16 eggs per day. She eats three for breakfast every morning and bakes muffins for her friends every day with four. She sells the remainder at the farmers' market daily for $2 per fresh duck egg. How much in dollars does she make every day at the farmers' market?" \
 --answers 20 100 21 18 \
 --target "Janet sells 16 - 3 - 4 = <<16-3-4=9>>9 duck eggs a day. She makes 9 * 2 = $<<9*2=18>>18 every day at the farmer’s market. #### 18"
@@ -126,15 +126,15 @@
 SCORE:
 [0.0, 0.0, 0.2, 1.0]
 ```
 
 </details>
 
 
-#### Evaluate one file
+#### Evaluate files
 ```sh
 auto-eval file --config_file CHANGE_TO_YOUR_CONFIG_PATH \
 --eval_data_path model_a_pred.json model_b_pred.json  \
 --output_path eval_result_path.xlsx \
 --model gpt-4 
 ```
 <details open> <summary>log output example:</summary>
```

### Comparing `auto-eval-0.1.4/README.md` & `auto-eval-0.1.5/README.md`

 * *Files 0% similar despite different names*

```diff
@@ -41,15 +41,15 @@
 {
     "api_key": "YOUR_API_KEY",
     "api": "https://api.anthropic.com",
     "api_type": "claude"
 }
 ```
 
-### 2. Use with command lines
+### 2. Usage with command lines
 #### Evaluate one sample
 ```sh
 auto-eval line --config_file CHANGE_TO_YOUR_CONFIG_PATH \
 --model gpt-3.5-turbo \
 --prompt "Janet’s ducks lay 16 eggs per day. She eats three for breakfast every morning and bakes muffins for her friends every day with four. She sells the remainder at the farmers' market daily for $2 per fresh duck egg. How much in dollars does she make every day at the farmers' market?" \
 --answers 20 100 21 18 \
 --target "Janet sells 16 - 3 - 4 = <<16-3-4=9>>9 duck eggs a day. She makes 9 * 2 = $<<9*2=18>>18 every day at the farmer’s market. #### 18"
@@ -114,15 +114,15 @@
 SCORE:
 [0.0, 0.0, 0.2, 1.0]
 ```
 
 </details>
 
 
-#### Evaluate one file
+#### Evaluate files
 ```sh
 auto-eval file --config_file CHANGE_TO_YOUR_CONFIG_PATH \
 --eval_data_path model_a_pred.json model_b_pred.json  \
 --output_path eval_result_path.xlsx \
 --model gpt-4 
 ```
 <details open> <summary>log output example:</summary>
```

### Comparing `auto-eval-0.1.4/auto_eval.egg-info/PKG-INFO` & `auto-eval-0.1.5/auto_eval.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: auto-eval
-Version: 0.1.4
+Version: 0.1.5
 Summary: Using only one line of commmands to evaluate multiple models
 Home-page: https://github.com/muximus3/Auto-Eval
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
@@ -53,15 +53,15 @@
 {
     "api_key": "YOUR_API_KEY",
     "api": "https://api.anthropic.com",
     "api_type": "claude"
 }
 ```
 
-### 2. Use with command lines
+### 2. Usage with command lines
 #### Evaluate one sample
 ```sh
 auto-eval line --config_file CHANGE_TO_YOUR_CONFIG_PATH \
 --model gpt-3.5-turbo \
 --prompt "Janet’s ducks lay 16 eggs per day. She eats three for breakfast every morning and bakes muffins for her friends every day with four. She sells the remainder at the farmers' market daily for $2 per fresh duck egg. How much in dollars does she make every day at the farmers' market?" \
 --answers 20 100 21 18 \
 --target "Janet sells 16 - 3 - 4 = <<16-3-4=9>>9 duck eggs a day. She makes 9 * 2 = $<<9*2=18>>18 every day at the farmer’s market. #### 18"
@@ -126,15 +126,15 @@
 SCORE:
 [0.0, 0.0, 0.2, 1.0]
 ```
 
 </details>
 
 
-#### Evaluate one file
+#### Evaluate files
 ```sh
 auto-eval file --config_file CHANGE_TO_YOUR_CONFIG_PATH \
 --eval_data_path model_a_pred.json model_b_pred.json  \
 --output_path eval_result_path.xlsx \
 --model gpt-4 
 ```
 <details open> <summary>log output example:</summary>
```

### Comparing `auto-eval-0.1.4/commands/auto_eval.py` & `auto-eval-0.1.5/commands/auto_eval.py`

 * *Files identical despite different names*

### Comparing `auto-eval-0.1.4/eval/auto_llms_eval.py` & `auto-eval-0.1.5/eval/auto_llms_eval.py`

 * *Files 4% similar despite different names*

```diff
@@ -71,16 +71,14 @@
     else:
         return None
 
 
 
 def prepare_eval_data(eval_data_path: List[str], eval_categories: Optional[List[str]] = None, sample_num: int=0) -> List[pd.DataFrame]:
     eval_data = df_reader(eval_data_path[0]) if len(eval_data_path) == 1 else pd.concat([df_reader(file_path) for file_path in eval_data_path])
-    if 'score' in eval_data.keys():
-        eval_data['score'] = 0.
     eval_data = eval_data.fillna('')
     if len({'instruction', 'input', 'output'} - set(eval_data.keys())) == 0:
         eval_data['question'] = eval_data['instruction'].str.cat(
             eval_data['input'], sep=' ')
     elif len({'prompt', 'output'} - set(eval_data.keys())) == 0:
         eval_data['quesion'] = eval_data['prompt'].copy()
     elif len({'question', 'answer'} - set(eval_data.keys())) == 0:
```

### Comparing `auto-eval-0.1.4/prompt_template/eval_prompt_template.json` & `auto-eval-0.1.5/prompt_template/eval_prompt_template.json`

 * *Files identical despite different names*

### Comparing `auto-eval-0.1.4/prompt_template/prompter.py` & `auto-eval-0.1.5/prompt_template/prompter.py`

 * *Files identical despite different names*

### Comparing `auto-eval-0.1.4/setup.py` & `auto-eval-0.1.5/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="auto-eval",
-    version="0.1.4",
+    version="0.1.5",
     packages=find_packages(),
     package_data={
       "prompt_template":["eval_prompt_template.json"]  
     },
     install_requires=[
         # Add your library's dependencies here
         "one-api-tool",
```

### Comparing `auto-eval-0.1.4/utils/data_utils.py` & `auto-eval-0.1.5/utils/data_utils.py`

 * *Files 4% similar despite different names*

```diff
@@ -2,16 +2,18 @@
 import re
 import os
 import json
 import pandas as pd
 
 
 def df_reader(data_path) -> pd.DataFrame:
-    if data_path.endswith(('json', 'jsonl')):
+    if data_path.endswith('json'):
         df_data = pd.read_json(data_path)
+    if data_path.endswith('jsonl'):
+        df_data = pd.read_json(data_path, lines=True)
     elif data_path.endswith('xlsx'):
         df_data = pd.read_excel(data_path)
     elif data_path.endswith('csv'):
         df_data = pd.read_csv(data_path)
     else:
         raise AssertionError(f'not supported file type:{data_path}, suport types: json, jsonl, xlsx, csv')
     return df_data
```

