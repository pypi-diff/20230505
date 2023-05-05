# Comparing `tmp/auto-eval-0.1.3.tar.gz` & `tmp/auto-eval-0.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "auto-eval-0.1.3.tar", last modified: Thu May  4 08:50:09 2023, max compression
+gzip compressed data, was "auto-eval-0.1.4.tar", last modified: Fri May  5 09:01:52 2023, max compression
```

## Comparing `auto-eval-0.1.3.tar` & `auto-eval-0.1.4.tar`

### file list

```diff
@@ -1,26 +1,26 @@
-drwxr-xr-x   0 zhangchong   (501) staff       (20)        0 2023-05-04 08:50:09.368690 auto-eval-0.1.3/
--rw-r--r--   0 zhangchong   (501) staff       (20)     1071 2023-04-28 07:53:45.000000 auto-eval-0.1.3/LICENSE
--rw-r--r--   0 zhangchong   (501) staff       (20)    11559 2023-05-04 08:50:09.368471 auto-eval-0.1.3/PKG-INFO
--rw-r--r--   0 zhangchong   (501) staff       (20)    11133 2023-05-04 08:48:55.000000 auto-eval-0.1.3/README.md
-drwxr-xr-x   0 zhangchong   (501) staff       (20)        0 2023-05-04 08:50:09.365954 auto-eval-0.1.3/auto_eval.egg-info/
--rw-r--r--   0 zhangchong   (501) staff       (20)    11559 2023-05-04 08:50:09.000000 auto-eval-0.1.3/auto_eval.egg-info/PKG-INFO
--rw-r--r--   0 zhangchong   (501) staff       (20)      445 2023-05-04 08:50:09.000000 auto-eval-0.1.3/auto_eval.egg-info/SOURCES.txt
--rw-r--r--   0 zhangchong   (501) staff       (20)        1 2023-05-04 08:50:09.000000 auto-eval-0.1.3/auto_eval.egg-info/dependency_links.txt
--rw-r--r--   0 zhangchong   (501) staff       (20)       54 2023-05-04 08:50:09.000000 auto-eval-0.1.3/auto_eval.egg-info/entry_points.txt
--rw-r--r--   0 zhangchong   (501) staff       (20)       49 2023-05-04 08:50:09.000000 auto-eval-0.1.3/auto_eval.egg-info/requires.txt
--rw-r--r--   0 zhangchong   (501) staff       (20)       36 2023-05-04 08:50:09.000000 auto-eval-0.1.3/auto_eval.egg-info/top_level.txt
-drwxr-xr-x   0 zhangchong   (501) staff       (20)        0 2023-05-04 08:50:09.366183 auto-eval-0.1.3/commands/
--rw-r--r--   0 zhangchong   (501) staff       (20)        0 2023-04-28 08:32:15.000000 auto-eval-0.1.3/commands/__init__.py
--rw-r--r--   0 zhangchong   (501) staff       (20)     3824 2023-05-04 05:20:21.000000 auto-eval-0.1.3/commands/auto_eval.py
-drwxr-xr-x   0 zhangchong   (501) staff       (20)        0 2023-05-04 08:50:09.366711 auto-eval-0.1.3/eval/
--rw-r--r--   0 zhangchong   (501) staff       (20)       79 2023-05-04 02:44:34.000000 auto-eval-0.1.3/eval/__init__.py
--rw-r--r--   0 zhangchong   (501) staff       (20)     6997 2023-05-04 07:58:43.000000 auto-eval-0.1.3/eval/auto_llms_eval.py
-drwxr-xr-x   0 zhangchong   (501) staff       (20)        0 2023-05-04 08:50:09.367521 auto-eval-0.1.3/prompt_template/
--rw-r--r--   0 zhangchong   (501) staff       (20)       42 2023-04-28 09:38:25.000000 auto-eval-0.1.3/prompt_template/__init__.py
--rw-r--r--   0 zhangchong   (501) staff       (20)      860 2023-04-28 08:33:34.000000 auto-eval-0.1.3/prompt_template/eval_prompt_template.json
--rw-r--r--   0 zhangchong   (501) staff       (20)     5527 2023-05-04 02:47:26.000000 auto-eval-0.1.3/prompt_template/prompter.py
--rw-r--r--   0 zhangchong   (501) staff       (20)       38 2023-05-04 08:50:09.368743 auto-eval-0.1.3/setup.cfg
--rw-r--r--   0 zhangchong   (501) staff       (20)      940 2023-05-04 08:44:58.000000 auto-eval-0.1.3/setup.py
-drwxr-xr-x   0 zhangchong   (501) staff       (20)        0 2023-05-04 08:50:09.368109 auto-eval-0.1.3/utils/
--rw-r--r--   0 zhangchong   (501) staff       (20)       26 2023-04-28 09:40:19.000000 auto-eval-0.1.3/utils/__init__.py
--rw-r--r--   0 zhangchong   (501) staff       (20)     2832 2023-05-04 04:56:04.000000 auto-eval-0.1.3/utils/data_utils.py
+drwxr-xr-x   0 zhangchong   (501) staff       (20)        0 2023-05-05 09:01:52.662127 auto-eval-0.1.4/
+-rw-r--r--   0 zhangchong   (501) staff       (20)     1071 2023-04-28 07:53:45.000000 auto-eval-0.1.4/LICENSE
+-rw-r--r--   0 zhangchong   (501) staff       (20)    11479 2023-05-05 09:01:52.661918 auto-eval-0.1.4/PKG-INFO
+-rw-r--r--   0 zhangchong   (501) staff       (20)    11053 2023-05-05 08:55:21.000000 auto-eval-0.1.4/README.md
+drwxr-xr-x   0 zhangchong   (501) staff       (20)        0 2023-05-05 09:01:52.659087 auto-eval-0.1.4/auto_eval.egg-info/
+-rw-r--r--   0 zhangchong   (501) staff       (20)    11479 2023-05-05 09:01:52.000000 auto-eval-0.1.4/auto_eval.egg-info/PKG-INFO
+-rw-r--r--   0 zhangchong   (501) staff       (20)      445 2023-05-05 09:01:52.000000 auto-eval-0.1.4/auto_eval.egg-info/SOURCES.txt
+-rw-r--r--   0 zhangchong   (501) staff       (20)        1 2023-05-05 09:01:52.000000 auto-eval-0.1.4/auto_eval.egg-info/dependency_links.txt
+-rw-r--r--   0 zhangchong   (501) staff       (20)       54 2023-05-05 09:01:52.000000 auto-eval-0.1.4/auto_eval.egg-info/entry_points.txt
+-rw-r--r--   0 zhangchong   (501) staff       (20)       49 2023-05-05 09:01:52.000000 auto-eval-0.1.4/auto_eval.egg-info/requires.txt
+-rw-r--r--   0 zhangchong   (501) staff       (20)       36 2023-05-05 09:01:52.000000 auto-eval-0.1.4/auto_eval.egg-info/top_level.txt
+drwxr-xr-x   0 zhangchong   (501) staff       (20)        0 2023-05-05 09:01:52.659489 auto-eval-0.1.4/commands/
+-rw-r--r--   0 zhangchong   (501) staff       (20)        0 2023-04-28 08:32:15.000000 auto-eval-0.1.4/commands/__init__.py
+-rw-r--r--   0 zhangchong   (501) staff       (20)     3909 2023-05-05 08:12:59.000000 auto-eval-0.1.4/commands/auto_eval.py
+drwxr-xr-x   0 zhangchong   (501) staff       (20)        0 2023-05-05 09:01:52.660141 auto-eval-0.1.4/eval/
+-rw-r--r--   0 zhangchong   (501) staff       (20)      131 2023-05-05 08:11:08.000000 auto-eval-0.1.4/eval/__init__.py
+-rw-r--r--   0 zhangchong   (501) staff       (20)     7071 2023-05-05 08:56:41.000000 auto-eval-0.1.4/eval/auto_llms_eval.py
+drwxr-xr-x   0 zhangchong   (501) staff       (20)        0 2023-05-05 09:01:52.660845 auto-eval-0.1.4/prompt_template/
+-rw-r--r--   0 zhangchong   (501) staff       (20)       44 2023-05-05 07:40:16.000000 auto-eval-0.1.4/prompt_template/__init__.py
+-rw-r--r--   0 zhangchong   (501) staff       (20)      773 2023-05-05 07:29:57.000000 auto-eval-0.1.4/prompt_template/eval_prompt_template.json
+-rw-r--r--   0 zhangchong   (501) staff       (20)     2948 2023-05-05 08:21:30.000000 auto-eval-0.1.4/prompt_template/prompter.py
+-rw-r--r--   0 zhangchong   (501) staff       (20)       38 2023-05-05 09:01:52.662178 auto-eval-0.1.4/setup.cfg
+-rw-r--r--   0 zhangchong   (501) staff       (20)      940 2023-05-05 08:58:28.000000 auto-eval-0.1.4/setup.py
+drwxr-xr-x   0 zhangchong   (501) staff       (20)        0 2023-05-05 09:01:52.661445 auto-eval-0.1.4/utils/
+-rw-r--r--   0 zhangchong   (501) staff       (20)       26 2023-04-28 09:40:19.000000 auto-eval-0.1.4/utils/__init__.py
+-rw-r--r--   0 zhangchong   (501) staff       (20)     2832 2023-05-04 04:56:04.000000 auto-eval-0.1.4/utils/data_utils.py
```

### Comparing `auto-eval-0.1.3/LICENSE` & `auto-eval-0.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `auto-eval-0.1.3/PKG-INFO` & `auto-eval-0.1.4/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,32 +1,27 @@
 Metadata-Version: 2.1
 Name: auto-eval
-Version: 0.1.3
+Version: 0.1.4
 Summary: Using only one line of commmands to evaluate multiple models
 Home-page: https://github.com/muximus3/Auto-Eval
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Auto-Eval
 
 **Auto-Eval** utilizes ChatGPT (GPT-3.5-turbo), GPT-4, and Claude's API to evaluate language models with a single command. 
 
-By default, it assesses the accuracy of language models in various areas such as mathematical calculations, question answering, translation, classification and more. 
-
 The evaluation prompt has been extensively tested to ensure maximum accuracy even when using GPT-3.5 while minimizing word usage to save token budget since GPT-4 can be quite expensive 💰.
 
 To further personalize the prompt, you can modify it using the default templates as a basis. For additional information, please refer to the documentation provided below ([click here](#jump)).
 
-Our unified interface integrates multiple GPT APIs using the [One-API-Tool](https://github.com/muximus3/OneAPI) library, allowing for maximum customization and future development.
-
-
 ## Installation
 ```sh
 pip install -U auto-eval
 ```
 
 ## Usage
 To utilize this repository, you must first obtain API keys from OpenAI, Microsoft Azure, or Anthropic. To acquire your OpenAI API key, visit their website at https://platform.openai.com/account/api-keys. For your Claude API key, go to the Anthropic website at https://console.anthropic.com/account/keys.
@@ -67,15 +62,15 @@
 ```sh
 auto-eval line --config_file CHANGE_TO_YOUR_CONFIG_PATH \
 --model gpt-3.5-turbo \
 --prompt "Janet’s ducks lay 16 eggs per day. She eats three for breakfast every morning and bakes muffins for her friends every day with four. She sells the remainder at the farmers' market daily for $2 per fresh duck egg. How much in dollars does she make every day at the farmers' market?" \
 --answers 20 100 21 18 \
 --target "Janet sells 16 - 3 - 4 = <<16-3-4=9>>9 duck eggs a day. She makes 9 * 2 = $<<9*2=18>>18 every day at the farmer’s market. #### 18"
 ```
-<details> <summary>Click to see log output example:</summary>
+<details> <summary>log output example:</summary>
 
 ```text
 
 Using prompt template:
  {
   "eval_with_target_instruction": "Please evaluate and comment each [Candidate answer] based on the [Correct answer]. Then output all [Candidate answer] scores (0-1) in a summary format of {\"number\": \"score\"}, e.g, {\"A\": \"0.2\", \"B\": \"0.8\"}",
   "eval_with_target_template": "[Question]: {q}\n\n[Correct answer]: {target}\n\n[Candidate answer]:\n{options}\n\n[System]:\n{instruction}",
@@ -127,68 +122,70 @@
 
 -------------------- response end --------------------
 
 
 SCORE:
 [0.0, 0.0, 0.2, 1.0]
 ```
+
 </details>
 
 
 #### Evaluate one file
 ```sh
-auto-eval-file --config_file CHANGE_TO_YOUR_CONFIG_PATH \
---eval_data_path   \
---output_path  \
---model gpt-3.5-turbo 
+auto-eval file --config_file CHANGE_TO_YOUR_CONFIG_PATH \
+--eval_data_path model_a_pred.json model_b_pred.json  \
+--output_path eval_result_path.xlsx \
+--model gpt-4 
 ```
-<details> <summary>Click to see log output example:</summary>
-
+<details open> <summary>log output example:</summary>
 
+<br>
 prompts and responses detail...
 
 -------------------- Scores by Model --------------------
 | model                      | score   |
 |:---------------------------|:--------|
-| model A       | 1.5/3   |
-| model B | 1.3/3   |
-| model C          | 0.0/3   |
+| model A       | 81.5/100   |
+| model B |91.3/100   |
+| model C          | 80.0/100   |
 
 -------------------- Scores by Model and Task Category --------------------
 | model                      | category   | score   |
 |:---------------------------|:-----------|:--------|
-| model A       | Common sense QA   | 1.5/2   |
-| model A       | Elementary arithmetic   | 0.0/1   |
-| model B | Common sense QA   | 1.3/2   |
-| model B | Elementary arithmetic   | 0.0/1   |
-| model C           | Common sense QA   | 0.0/2   |
-| model C           | Elementary arithmetic   | 0.0/1   |
+| model A       | Common sense QA   | 15.5/20   |
+| model A       | Elementary arithmetic   | 10.0/15   |
+| model B | Common sense QA   | 17.3/20   |
+| model B | Elementary arithmetic   | 11.0/15   |
+| model C           | Common sense QA   | 14.7/20   |
+| model C           | Elementary arithmetic   | 9.2/15   |
+
 
 </details>
 
 ## Arguments Definitions:
 
 ### Shared arguments
 `--config_file` string ${\color{orange}\text{Required}}$ <br>A local configuration file containing API key information.
 
- <span id="jump">`--template_path`${\color{grey}\text{Optional}}$ <br> A cuatom template json file path, Please refer to the default prompt template for modification. You can define the position of instruction at the beginning or end, define the content of instruction, arrange the output of the model to be evaluated, and specify output formats. Currently, only JSON format parsing or score mode separated by spaces are supported as output formats. For example: `{"A":0,"B": 0.1}` or 0 0.1.<br>
-Would use the template provided below if there is no specific one available.
+ <span id="jump">`--template_path`${\color{grey}\text{Optional}}$ <br>
+The template file path should be in JSON format and instructs the model to evaluate and comment on each answer, as well as output summary scores in JSON format, such as `{"A": 0, "B": 0.1}`.<br>
+If no specific template is available, the default one provided below will be used.<br>
+If you want to use a custom template, make sure it has slots for "question", "answers", and "target". The first two are required, while "target" is only necessary if your evaluation data has a column named "target".
 ```json
 {
-    "eval_without_target_instruction": "Please solve the [Question] independently to obtain the [Correct answer], and then evaluate and comment each [Candidate answer] based on the [Correct answer]. Finally, output all [Candidate answers] scores (0-1) in a summary format of {\"number\": \"score\"}, e.g, {\"A\": \"0.2\", \"B\": \"0.8\"}",
-    "eval_with_target_instruction": "Please evaluate and comment each [Candidate answer] based on the [Correct answer]. Then output all [Candidate answer] scores (0-1) in a summary format of {\"number\": \"score\"}, e.g, {\"A\": \"0.2\", \"B\": \"0.8\"}",
-    "eval_with_target_template": "[Question]: {q}\n\n[Correct answer]: {target}\n\n[Candidate answer]:\n{options}\n\n[System]:\n{instruction}",
-    "eval_without_target_template": "[Question]: {q}\n\n[Candidate answer]:\n{options}\n\n[System]:\n{instruction}" 
+    "eval_with_target_template": "[Question]: {question}\n\n[Correct answer]: {target}\n\n[Candidate answer]:\n{answers}\n\n[System]:\nPlease solve the [Question] independently to obtain the [Correct answer], and then evaluate and comment each [Candidate answer] based on the [Correct answer]. Finally, output all [Candidate answers] scores (0-1) in a summary format of {{\"number\": \"score\"}}, e.g, {{\"A\": \"0.2\", \"B\": \"0.8\"}}",
+    "eval_without_target_template": "[Question]: {question}\n\n[Candidate answer]:\n{answers}\n\n[System]:\nPlease evaluate and comment each [Candidate answer] based on the [Correct answer]. Then output all [Candidate answer] scores (0-1) in a summary format of {{\"number\": \"score\"}}, e.g, {{\"A\": \"0.2\", \"B\": \"0.8\"}}" 
 }
 ```
 
 
 `--verbose` bool ${\color{grey}\text{Optional}}$ Defaults to True <br> Whether to print every prompt and response evaluation detail.
 
-`--model` string ${\color{grey}\text{Optional}}$  Defaults to GPT-3.5-turbo or Claude-v1.3 depends on `api_type`<br> Which model to perform evaluation.
+`--model` string ${\color{grey}\text{Optional}}$  Defaults to gpt-3.5-turbo or claude-v1.3 depends on `api_type`<br> Which model to perform evaluation, The default model for evaluation is either gpt-3.5-turbo or claude-v1.3, depending on the API type. You can specify which model to use for evaluation by providing its name, such as "gpt-4", "claude-instant-v1", or "claude-v1.3".
 
 `--temperature` number ${\color{grey}\text{Optional}}$ Defaults to 1 <br>What sampling temperature to use.  Higher values like 1 will make the output more random, while lower values like 0.1 will make it more focused and deterministic.
 
 `--max_new_tokens` integer ${\color{grey}\text{Optional}}$ Defaults to 2048 <br>
 The maximum number of tokens to generate in the chat completion.
 The total length of input tokens and generated tokens is limited by the model's context length.
 
@@ -201,18 +198,18 @@
 `--answers` array ${\color{orange}\text{Required}}$ <br>
 LLMs outputs correspond to the question in the prompt, answers must be separated by space. e.g., A set of four answers would look like this: 1 0 -1 2
 
 `--target` ${\color{grey}\text{Optional}}$ Defaults to \'\'<br> The correct answer for the question. The prompt will be different depending on whether the target is provided, e.g., if no target is provided, the model is asked to solve the question first and then evaluate each candidate answer.
 
 ### Evaluate file arguments
 
-`--eval_data_path`: string ${\color{orange}\text{Required}}$ <br>The file path of the input data to be evaluated.<br>
+`--eval_data_path`: string ${\color{orange}\text{Required}}$ <br>This refers to the file paths of the input data that will be evaluated. If multiple paths are provided, please ensure that they have identical column names.
 
 **Input file format:**
-The input file currently supports files with .json, .jsonl, .csv, and .xlsx extensions. The header of the file can be one of the following types: `{'instruction', 'input', ‘output’}`, `{'prompt', 'output'}`, `{'prompt', 'target'}`, `{'question', 'answer'}`, or `{'question', 'output'}`.
+The input file currently supports files with .json, .jsonl, .csv, and .xlsx extensions. The header of the file can be one of the following types: `{'instruction', 'input', ‘output’}`, `{'prompt', 'output'}`, `{'question', 'answer'}`, or `{'question', 'output'}`.
 
 `--output_path`: string ${\color{orange}\text{Required}}$ <br>The output file path for evaluation results.
 
 **Output File format:**
 The output file can be specified as a .json, .jsonl, .csv or.xlsx extension. If it contains a field called "model", scores and statistics will be grouped based on this field. If it also contains fields called "model" and "category", scores and statistics will be grouped based on both fields. Any other fields will not be processed; the output will include all columns from the original input along with evaluation scores and explanations.
 
 `--eval_categories`: array ${\color{grey}\text{Optional}}$ Defaults to null <br> Choose specific types of question categories to evaluate. This only works when the input file contains a "category" column corresponding to each question.
```

### Comparing `auto-eval-0.1.3/README.md` & `auto-eval-0.1.4/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,20 +1,15 @@
 # Auto-Eval
 
 **Auto-Eval** utilizes ChatGPT (GPT-3.5-turbo), GPT-4, and Claude's API to evaluate language models with a single command. 
 
-By default, it assesses the accuracy of language models in various areas such as mathematical calculations, question answering, translation, classification and more. 
-
 The evaluation prompt has been extensively tested to ensure maximum accuracy even when using GPT-3.5 while minimizing word usage to save token budget since GPT-4 can be quite expensive 💰.
 
 To further personalize the prompt, you can modify it using the default templates as a basis. For additional information, please refer to the documentation provided below ([click here](#jump)).
 
-Our unified interface integrates multiple GPT APIs using the [One-API-Tool](https://github.com/muximus3/OneAPI) library, allowing for maximum customization and future development.
-
-
 ## Installation
 ```sh
 pip install -U auto-eval
 ```
 
 ## Usage
 To utilize this repository, you must first obtain API keys from OpenAI, Microsoft Azure, or Anthropic. To acquire your OpenAI API key, visit their website at https://platform.openai.com/account/api-keys. For your Claude API key, go to the Anthropic website at https://console.anthropic.com/account/keys.
@@ -55,15 +50,15 @@
 ```sh
 auto-eval line --config_file CHANGE_TO_YOUR_CONFIG_PATH \
 --model gpt-3.5-turbo \
 --prompt "Janet’s ducks lay 16 eggs per day. She eats three for breakfast every morning and bakes muffins for her friends every day with four. She sells the remainder at the farmers' market daily for $2 per fresh duck egg. How much in dollars does she make every day at the farmers' market?" \
 --answers 20 100 21 18 \
 --target "Janet sells 16 - 3 - 4 = <<16-3-4=9>>9 duck eggs a day. She makes 9 * 2 = $<<9*2=18>>18 every day at the farmer’s market. #### 18"
 ```
-<details> <summary>Click to see log output example:</summary>
+<details> <summary>log output example:</summary>
 
 ```text
 
 Using prompt template:
  {
   "eval_with_target_instruction": "Please evaluate and comment each [Candidate answer] based on the [Correct answer]. Then output all [Candidate answer] scores (0-1) in a summary format of {\"number\": \"score\"}, e.g, {\"A\": \"0.2\", \"B\": \"0.8\"}",
   "eval_with_target_template": "[Question]: {q}\n\n[Correct answer]: {target}\n\n[Candidate answer]:\n{options}\n\n[System]:\n{instruction}",
@@ -115,68 +110,70 @@
 
 -------------------- response end --------------------
 
 
 SCORE:
 [0.0, 0.0, 0.2, 1.0]
 ```
+
 </details>
 
 
 #### Evaluate one file
 ```sh
-auto-eval-file --config_file CHANGE_TO_YOUR_CONFIG_PATH \
---eval_data_path   \
---output_path  \
---model gpt-3.5-turbo 
+auto-eval file --config_file CHANGE_TO_YOUR_CONFIG_PATH \
+--eval_data_path model_a_pred.json model_b_pred.json  \
+--output_path eval_result_path.xlsx \
+--model gpt-4 
 ```
-<details> <summary>Click to see log output example:</summary>
-
+<details open> <summary>log output example:</summary>
 
+<br>
 prompts and responses detail...
 
 -------------------- Scores by Model --------------------
 | model                      | score   |
 |:---------------------------|:--------|
-| model A       | 1.5/3   |
-| model B | 1.3/3   |
-| model C          | 0.0/3   |
+| model A       | 81.5/100   |
+| model B |91.3/100   |
+| model C          | 80.0/100   |
 
 -------------------- Scores by Model and Task Category --------------------
 | model                      | category   | score   |
 |:---------------------------|:-----------|:--------|
-| model A       | Common sense QA   | 1.5/2   |
-| model A       | Elementary arithmetic   | 0.0/1   |
-| model B | Common sense QA   | 1.3/2   |
-| model B | Elementary arithmetic   | 0.0/1   |
-| model C           | Common sense QA   | 0.0/2   |
-| model C           | Elementary arithmetic   | 0.0/1   |
+| model A       | Common sense QA   | 15.5/20   |
+| model A       | Elementary arithmetic   | 10.0/15   |
+| model B | Common sense QA   | 17.3/20   |
+| model B | Elementary arithmetic   | 11.0/15   |
+| model C           | Common sense QA   | 14.7/20   |
+| model C           | Elementary arithmetic   | 9.2/15   |
+
 
 </details>
 
 ## Arguments Definitions:
 
 ### Shared arguments
 `--config_file` string ${\color{orange}\text{Required}}$ <br>A local configuration file containing API key information.
 
- <span id="jump">`--template_path`${\color{grey}\text{Optional}}$ <br> A cuatom template json file path, Please refer to the default prompt template for modification. You can define the position of instruction at the beginning or end, define the content of instruction, arrange the output of the model to be evaluated, and specify output formats. Currently, only JSON format parsing or score mode separated by spaces are supported as output formats. For example: `{"A":0,"B": 0.1}` or 0 0.1.<br>
-Would use the template provided below if there is no specific one available.
+ <span id="jump">`--template_path`${\color{grey}\text{Optional}}$ <br>
+The template file path should be in JSON format and instructs the model to evaluate and comment on each answer, as well as output summary scores in JSON format, such as `{"A": 0, "B": 0.1}`.<br>
+If no specific template is available, the default one provided below will be used.<br>
+If you want to use a custom template, make sure it has slots for "question", "answers", and "target". The first two are required, while "target" is only necessary if your evaluation data has a column named "target".
 ```json
 {
-    "eval_without_target_instruction": "Please solve the [Question] independently to obtain the [Correct answer], and then evaluate and comment each [Candidate answer] based on the [Correct answer]. Finally, output all [Candidate answers] scores (0-1) in a summary format of {\"number\": \"score\"}, e.g, {\"A\": \"0.2\", \"B\": \"0.8\"}",
-    "eval_with_target_instruction": "Please evaluate and comment each [Candidate answer] based on the [Correct answer]. Then output all [Candidate answer] scores (0-1) in a summary format of {\"number\": \"score\"}, e.g, {\"A\": \"0.2\", \"B\": \"0.8\"}",
-    "eval_with_target_template": "[Question]: {q}\n\n[Correct answer]: {target}\n\n[Candidate answer]:\n{options}\n\n[System]:\n{instruction}",
-    "eval_without_target_template": "[Question]: {q}\n\n[Candidate answer]:\n{options}\n\n[System]:\n{instruction}" 
+    "eval_with_target_template": "[Question]: {question}\n\n[Correct answer]: {target}\n\n[Candidate answer]:\n{answers}\n\n[System]:\nPlease solve the [Question] independently to obtain the [Correct answer], and then evaluate and comment each [Candidate answer] based on the [Correct answer]. Finally, output all [Candidate answers] scores (0-1) in a summary format of {{\"number\": \"score\"}}, e.g, {{\"A\": \"0.2\", \"B\": \"0.8\"}}",
+    "eval_without_target_template": "[Question]: {question}\n\n[Candidate answer]:\n{answers}\n\n[System]:\nPlease evaluate and comment each [Candidate answer] based on the [Correct answer]. Then output all [Candidate answer] scores (0-1) in a summary format of {{\"number\": \"score\"}}, e.g, {{\"A\": \"0.2\", \"B\": \"0.8\"}}" 
 }
 ```
 
 
 `--verbose` bool ${\color{grey}\text{Optional}}$ Defaults to True <br> Whether to print every prompt and response evaluation detail.
 
-`--model` string ${\color{grey}\text{Optional}}$  Defaults to GPT-3.5-turbo or Claude-v1.3 depends on `api_type`<br> Which model to perform evaluation.
+`--model` string ${\color{grey}\text{Optional}}$  Defaults to gpt-3.5-turbo or claude-v1.3 depends on `api_type`<br> Which model to perform evaluation, The default model for evaluation is either gpt-3.5-turbo or claude-v1.3, depending on the API type. You can specify which model to use for evaluation by providing its name, such as "gpt-4", "claude-instant-v1", or "claude-v1.3".
 
 `--temperature` number ${\color{grey}\text{Optional}}$ Defaults to 1 <br>What sampling temperature to use.  Higher values like 1 will make the output more random, while lower values like 0.1 will make it more focused and deterministic.
 
 `--max_new_tokens` integer ${\color{grey}\text{Optional}}$ Defaults to 2048 <br>
 The maximum number of tokens to generate in the chat completion.
 The total length of input tokens and generated tokens is limited by the model's context length.
 
@@ -189,18 +186,18 @@
 `--answers` array ${\color{orange}\text{Required}}$ <br>
 LLMs outputs correspond to the question in the prompt, answers must be separated by space. e.g., A set of four answers would look like this: 1 0 -1 2
 
 `--target` ${\color{grey}\text{Optional}}$ Defaults to \'\'<br> The correct answer for the question. The prompt will be different depending on whether the target is provided, e.g., if no target is provided, the model is asked to solve the question first and then evaluate each candidate answer.
 
 ### Evaluate file arguments
 
-`--eval_data_path`: string ${\color{orange}\text{Required}}$ <br>The file path of the input data to be evaluated.<br>
+`--eval_data_path`: string ${\color{orange}\text{Required}}$ <br>This refers to the file paths of the input data that will be evaluated. If multiple paths are provided, please ensure that they have identical column names.
 
 **Input file format:**
-The input file currently supports files with .json, .jsonl, .csv, and .xlsx extensions. The header of the file can be one of the following types: `{'instruction', 'input', ‘output’}`, `{'prompt', 'output'}`, `{'prompt', 'target'}`, `{'question', 'answer'}`, or `{'question', 'output'}`.
+The input file currently supports files with .json, .jsonl, .csv, and .xlsx extensions. The header of the file can be one of the following types: `{'instruction', 'input', ‘output’}`, `{'prompt', 'output'}`, `{'question', 'answer'}`, or `{'question', 'output'}`.
 
 `--output_path`: string ${\color{orange}\text{Required}}$ <br>The output file path for evaluation results.
 
 **Output File format:**
 The output file can be specified as a .json, .jsonl, .csv or.xlsx extension. If it contains a field called "model", scores and statistics will be grouped based on this field. If it also contains fields called "model" and "category", scores and statistics will be grouped based on both fields. Any other fields will not be processed; the output will include all columns from the original input along with evaluation scores and explanations.
 
 `--eval_categories`: array ${\color{grey}\text{Optional}}$ Defaults to null <br> Choose specific types of question categories to evaluate. This only works when the input file contains a "category" column corresponding to each question.
```

### Comparing `auto-eval-0.1.3/auto_eval.egg-info/PKG-INFO` & `auto-eval-0.1.4/auto_eval.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,32 +1,27 @@
 Metadata-Version: 2.1
 Name: auto-eval
-Version: 0.1.3
+Version: 0.1.4
 Summary: Using only one line of commmands to evaluate multiple models
 Home-page: https://github.com/muximus3/Auto-Eval
 Classifier: Development Status :: 3 - Alpha
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Auto-Eval
 
 **Auto-Eval** utilizes ChatGPT (GPT-3.5-turbo), GPT-4, and Claude's API to evaluate language models with a single command. 
 
-By default, it assesses the accuracy of language models in various areas such as mathematical calculations, question answering, translation, classification and more. 
-
 The evaluation prompt has been extensively tested to ensure maximum accuracy even when using GPT-3.5 while minimizing word usage to save token budget since GPT-4 can be quite expensive 💰.
 
 To further personalize the prompt, you can modify it using the default templates as a basis. For additional information, please refer to the documentation provided below ([click here](#jump)).
 
-Our unified interface integrates multiple GPT APIs using the [One-API-Tool](https://github.com/muximus3/OneAPI) library, allowing for maximum customization and future development.
-
-
 ## Installation
 ```sh
 pip install -U auto-eval
 ```
 
 ## Usage
 To utilize this repository, you must first obtain API keys from OpenAI, Microsoft Azure, or Anthropic. To acquire your OpenAI API key, visit their website at https://platform.openai.com/account/api-keys. For your Claude API key, go to the Anthropic website at https://console.anthropic.com/account/keys.
@@ -67,15 +62,15 @@
 ```sh
 auto-eval line --config_file CHANGE_TO_YOUR_CONFIG_PATH \
 --model gpt-3.5-turbo \
 --prompt "Janet’s ducks lay 16 eggs per day. She eats three for breakfast every morning and bakes muffins for her friends every day with four. She sells the remainder at the farmers' market daily for $2 per fresh duck egg. How much in dollars does she make every day at the farmers' market?" \
 --answers 20 100 21 18 \
 --target "Janet sells 16 - 3 - 4 = <<16-3-4=9>>9 duck eggs a day. She makes 9 * 2 = $<<9*2=18>>18 every day at the farmer’s market. #### 18"
 ```
-<details> <summary>Click to see log output example:</summary>
+<details> <summary>log output example:</summary>
 
 ```text
 
 Using prompt template:
  {
   "eval_with_target_instruction": "Please evaluate and comment each [Candidate answer] based on the [Correct answer]. Then output all [Candidate answer] scores (0-1) in a summary format of {\"number\": \"score\"}, e.g, {\"A\": \"0.2\", \"B\": \"0.8\"}",
   "eval_with_target_template": "[Question]: {q}\n\n[Correct answer]: {target}\n\n[Candidate answer]:\n{options}\n\n[System]:\n{instruction}",
@@ -127,68 +122,70 @@
 
 -------------------- response end --------------------
 
 
 SCORE:
 [0.0, 0.0, 0.2, 1.0]
 ```
+
 </details>
 
 
 #### Evaluate one file
 ```sh
-auto-eval-file --config_file CHANGE_TO_YOUR_CONFIG_PATH \
---eval_data_path   \
---output_path  \
---model gpt-3.5-turbo 
+auto-eval file --config_file CHANGE_TO_YOUR_CONFIG_PATH \
+--eval_data_path model_a_pred.json model_b_pred.json  \
+--output_path eval_result_path.xlsx \
+--model gpt-4 
 ```
-<details> <summary>Click to see log output example:</summary>
-
+<details open> <summary>log output example:</summary>
 
+<br>
 prompts and responses detail...
 
 -------------------- Scores by Model --------------------
 | model                      | score   |
 |:---------------------------|:--------|
-| model A       | 1.5/3   |
-| model B | 1.3/3   |
-| model C          | 0.0/3   |
+| model A       | 81.5/100   |
+| model B |91.3/100   |
+| model C          | 80.0/100   |
 
 -------------------- Scores by Model and Task Category --------------------
 | model                      | category   | score   |
 |:---------------------------|:-----------|:--------|
-| model A       | Common sense QA   | 1.5/2   |
-| model A       | Elementary arithmetic   | 0.0/1   |
-| model B | Common sense QA   | 1.3/2   |
-| model B | Elementary arithmetic   | 0.0/1   |
-| model C           | Common sense QA   | 0.0/2   |
-| model C           | Elementary arithmetic   | 0.0/1   |
+| model A       | Common sense QA   | 15.5/20   |
+| model A       | Elementary arithmetic   | 10.0/15   |
+| model B | Common sense QA   | 17.3/20   |
+| model B | Elementary arithmetic   | 11.0/15   |
+| model C           | Common sense QA   | 14.7/20   |
+| model C           | Elementary arithmetic   | 9.2/15   |
+
 
 </details>
 
 ## Arguments Definitions:
 
 ### Shared arguments
 `--config_file` string ${\color{orange}\text{Required}}$ <br>A local configuration file containing API key information.
 
- <span id="jump">`--template_path`${\color{grey}\text{Optional}}$ <br> A cuatom template json file path, Please refer to the default prompt template for modification. You can define the position of instruction at the beginning or end, define the content of instruction, arrange the output of the model to be evaluated, and specify output formats. Currently, only JSON format parsing or score mode separated by spaces are supported as output formats. For example: `{"A":0,"B": 0.1}` or 0 0.1.<br>
-Would use the template provided below if there is no specific one available.
+ <span id="jump">`--template_path`${\color{grey}\text{Optional}}$ <br>
+The template file path should be in JSON format and instructs the model to evaluate and comment on each answer, as well as output summary scores in JSON format, such as `{"A": 0, "B": 0.1}`.<br>
+If no specific template is available, the default one provided below will be used.<br>
+If you want to use a custom template, make sure it has slots for "question", "answers", and "target". The first two are required, while "target" is only necessary if your evaluation data has a column named "target".
 ```json
 {
-    "eval_without_target_instruction": "Please solve the [Question] independently to obtain the [Correct answer], and then evaluate and comment each [Candidate answer] based on the [Correct answer]. Finally, output all [Candidate answers] scores (0-1) in a summary format of {\"number\": \"score\"}, e.g, {\"A\": \"0.2\", \"B\": \"0.8\"}",
-    "eval_with_target_instruction": "Please evaluate and comment each [Candidate answer] based on the [Correct answer]. Then output all [Candidate answer] scores (0-1) in a summary format of {\"number\": \"score\"}, e.g, {\"A\": \"0.2\", \"B\": \"0.8\"}",
-    "eval_with_target_template": "[Question]: {q}\n\n[Correct answer]: {target}\n\n[Candidate answer]:\n{options}\n\n[System]:\n{instruction}",
-    "eval_without_target_template": "[Question]: {q}\n\n[Candidate answer]:\n{options}\n\n[System]:\n{instruction}" 
+    "eval_with_target_template": "[Question]: {question}\n\n[Correct answer]: {target}\n\n[Candidate answer]:\n{answers}\n\n[System]:\nPlease solve the [Question] independently to obtain the [Correct answer], and then evaluate and comment each [Candidate answer] based on the [Correct answer]. Finally, output all [Candidate answers] scores (0-1) in a summary format of {{\"number\": \"score\"}}, e.g, {{\"A\": \"0.2\", \"B\": \"0.8\"}}",
+    "eval_without_target_template": "[Question]: {question}\n\n[Candidate answer]:\n{answers}\n\n[System]:\nPlease evaluate and comment each [Candidate answer] based on the [Correct answer]. Then output all [Candidate answer] scores (0-1) in a summary format of {{\"number\": \"score\"}}, e.g, {{\"A\": \"0.2\", \"B\": \"0.8\"}}" 
 }
 ```
 
 
 `--verbose` bool ${\color{grey}\text{Optional}}$ Defaults to True <br> Whether to print every prompt and response evaluation detail.
 
-`--model` string ${\color{grey}\text{Optional}}$  Defaults to GPT-3.5-turbo or Claude-v1.3 depends on `api_type`<br> Which model to perform evaluation.
+`--model` string ${\color{grey}\text{Optional}}$  Defaults to gpt-3.5-turbo or claude-v1.3 depends on `api_type`<br> Which model to perform evaluation, The default model for evaluation is either gpt-3.5-turbo or claude-v1.3, depending on the API type. You can specify which model to use for evaluation by providing its name, such as "gpt-4", "claude-instant-v1", or "claude-v1.3".
 
 `--temperature` number ${\color{grey}\text{Optional}}$ Defaults to 1 <br>What sampling temperature to use.  Higher values like 1 will make the output more random, while lower values like 0.1 will make it more focused and deterministic.
 
 `--max_new_tokens` integer ${\color{grey}\text{Optional}}$ Defaults to 2048 <br>
 The maximum number of tokens to generate in the chat completion.
 The total length of input tokens and generated tokens is limited by the model's context length.
 
@@ -201,18 +198,18 @@
 `--answers` array ${\color{orange}\text{Required}}$ <br>
 LLMs outputs correspond to the question in the prompt, answers must be separated by space. e.g., A set of four answers would look like this: 1 0 -1 2
 
 `--target` ${\color{grey}\text{Optional}}$ Defaults to \'\'<br> The correct answer for the question. The prompt will be different depending on whether the target is provided, e.g., if no target is provided, the model is asked to solve the question first and then evaluate each candidate answer.
 
 ### Evaluate file arguments
 
-`--eval_data_path`: string ${\color{orange}\text{Required}}$ <br>The file path of the input data to be evaluated.<br>
+`--eval_data_path`: string ${\color{orange}\text{Required}}$ <br>This refers to the file paths of the input data that will be evaluated. If multiple paths are provided, please ensure that they have identical column names.
 
 **Input file format:**
-The input file currently supports files with .json, .jsonl, .csv, and .xlsx extensions. The header of the file can be one of the following types: `{'instruction', 'input', ‘output’}`, `{'prompt', 'output'}`, `{'prompt', 'target'}`, `{'question', 'answer'}`, or `{'question', 'output'}`.
+The input file currently supports files with .json, .jsonl, .csv, and .xlsx extensions. The header of the file can be one of the following types: `{'instruction', 'input', ‘output’}`, `{'prompt', 'output'}`, `{'question', 'answer'}`, or `{'question', 'output'}`.
 
 `--output_path`: string ${\color{orange}\text{Required}}$ <br>The output file path for evaluation results.
 
 **Output File format:**
 The output file can be specified as a .json, .jsonl, .csv or.xlsx extension. If it contains a field called "model", scores and statistics will be grouped based on this field. If it also contains fields called "model" and "category", scores and statistics will be grouped based on both fields. Any other fields will not be processed; the output will include all columns from the original input along with evaluation scores and explanations.
 
 `--eval_categories`: array ${\color{grey}\text{Optional}}$ Defaults to null <br> Choose specific types of question categories to evaluate. This only works when the input file contains a "category" column corresponding to each question.
```

### Comparing `auto-eval-0.1.3/commands/auto_eval.py` & `auto-eval-0.1.4/commands/auto_eval.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import os
 import sys
 import argparse
 from oneapi import OneAPITool
 sys.path.append(os.path.normpath(f"{os.path.dirname(os.path.abspath(__file__))}/.."))
-from eval import eval_one_file, eval_one, EvalConfig 
+from eval import eval_one_group, eval_one_qa, eval_groups, EvalConfig
+from utils.data_utils import df_reader
 import prompt_template
     
 def add_shared_arguments(parser):
     parser.add_argument("-c", "--config_file", type=str, help="config file path", required=True)
     parser.add_argument("-tp", "--template_path", type=str, default=None, help="eval prompt template path", required=False)
     parser.add_argument("-v", "--verbose", type=bool, default=True, help="print every prompt and response detail", required=False)
     parser.add_argument("-m", "--model", type=str, default="", help="evaluate model name, e.g., gpt-35-turbo, gpt-4", required=False)
@@ -25,44 +26,44 @@
     line_parser.add_argument("-p", "--prompt", type=str, help="question", required=True)
     line_parser.add_argument("-a", "--answers", nargs='+', help="candidate answers", required=True)
     line_parser.add_argument("-ta", "--target", type=str, default="", help="standard answer", required=False)
 
     # auto-eval file
     file_parser = subparsers.add_parser("file", help="auto-eval file [<args>]")
     add_shared_arguments(file_parser)
-    file_parser.add_argument("-edp", "--eval_data_path", type=str, help="", required=True)
+    file_parser.add_argument("-edp", "--eval_data_path", nargs="+", help="one or more eval data path", required=True)
     file_parser.add_argument("-op", "--output_path", type=str, default="", help="", required=False)
     file_parser.add_argument("-ec", "--eval_categories", default=None, nargs="+", help="only evaluate chosen categories", required=False)
     file_parser.add_argument("-sn", "--sample_num", type=int, default=0, help="", required=False)
     file_parser.add_argument("-i", "--interval", type=int, default=1, help="request interval, gpt-4 need longer interval, e.g.,10s", required=False)
     file_parser.add_argument("-r", "--retry", type=bool, default=True, help="", required=False)
 
     args = parser.parse_args()
     if not args.template_path:
         template_path =  os.path.join(os.path.dirname(prompt_template.__file__), 'eval_prompt_template.json')
     else:
         template_path = args.template_path
-    eval_prompter = prompt_template.EvalPrompt.from_config(template_path, verbose=args.verbose)
+    eval_prompter = prompt_template.EvalPrompter.from_config(template_path, verbose=args.verbose)
 
     if args.command == "line":
         tool = OneAPITool.from_config_file(args.config_file)
-        score, raw_response = eval_one(
+        score, raw_response = eval_one_qa(
             eval_prompter=eval_prompter,
             question=args.prompt, 
             candidate_answers=args.answers, 
             target=args.target,
             api_tool=tool,
             model=args.model,
             temperature=args.temperature,
             max_new_tokens=args.max_new_tokens,
             )
         print(f'\nSCORE:\n{score}')
 
     elif args.command == "file":
-        eval_one_file(
+        eval_groups(
             EvalConfig(
             eval_prompter=eval_prompter,
             api_config_file=args.config_file, 
             eval_data_path=args.eval_data_path, 
             output_path=args.output_path, 
             model=args.model,
             eval_categories=args.eval_categories,
```

### Comparing `auto-eval-0.1.3/eval/auto_llms_eval.py` & `auto-eval-0.1.4/eval/auto_llms_eval.py`

 * *Files 6% similar despite different names*

```diff
@@ -7,24 +7,25 @@
 from tqdm import tqdm
 from typing import Optional, Tuple
 import time
 import sys
 from dataclasses import dataclass
 from oneapi import OneAPITool
 sys.path.append(os.path.normpath(f'{os.path.dirname(os.path.abspath(__file__))}/..'))
-from utils import df_reader, df_saver
+from utils import df_saver, df_reader
 from prompt_template import Prompter
 
 
-def eval_one(eval_prompter: Prompter,
+def eval_one_qa(
+             api_tool: OneAPITool,
+             eval_prompter: Prompter,
              question: str,
              candidate_answers: List[str],
-             target: Union[str, None],
-             api_tool: OneAPITool,
-             model: str,
+             target: Union[str, None]=None,
+             model: str='',
              temperature=0.1,
              max_new_tokens=2048) -> Tuple[Union[List[float], None], str]:
     raw_response = ''
     eval_prompt = eval_prompter.generate_prompt(question, target,
                                                 candidate_answers)
     try:
         raw_response = api_tool.simple_chat(eval_prompt,
@@ -39,54 +40,53 @@
         return None, raw_response
 
 
 def eval_one_group(
     api_tool: OneAPITool,
     eval_prompter: Prompter,
     data_group: pd.DataFrame,
-    model: str,
+    model: str='',
     temperature=0.1,
     max_new_tokens=2048,
 ) -> Union[pd.DataFrame, None]:
     group = data_group.reset_index()
     question = group['question'].unique()[0]
     candidate_answers = group['output']
     if 'target' in data_group.keys():
         target = group['target'].unique()[0]
     else:
         target = ''
-    scores, raw_response = eval_one(eval_prompter=eval_prompter,
+    scores, raw_response = eval_one_qa(api_tool=api_tool,
+                      eval_prompter=eval_prompter,
                       question=question,
                       candidate_answers=candidate_answers,
                       target=target,
-                      api_tool=api_tool,
                       model=model,
                       temperature=temperature,
                       max_new_tokens=max_new_tokens)
     if scores is not None and len(scores) == len(candidate_answers):
         group.at[0, 'raw_response'] = raw_response
         for i in range(len(scores)):
             group.at[i, 'score'] = scores[i]
         return group
     else:
         return None
 
 
 
-def prepare_eval_data(eval_data: pd.DataFrame, eval_categories: Optional[List[str]] = None, sample_num: int=0) -> List[pd.DataFrame]:
+def prepare_eval_data(eval_data_path: List[str], eval_categories: Optional[List[str]] = None, sample_num: int=0) -> List[pd.DataFrame]:
+    eval_data = df_reader(eval_data_path[0]) if len(eval_data_path) == 1 else pd.concat([df_reader(file_path) for file_path in eval_data_path])
     if 'score' in eval_data.keys():
         eval_data['score'] = 0.
     eval_data = eval_data.fillna('')
     if len({'instruction', 'input', 'output'} - set(eval_data.keys())) == 0:
         eval_data['question'] = eval_data['instruction'].str.cat(
             eval_data['input'], sep=' ')
     elif len({'prompt', 'output'} - set(eval_data.keys())) == 0:
         eval_data['quesion'] = eval_data['prompt'].copy()
-    elif len({'prompt', 'target'} - set(eval_data.keys())) == 0:
-        eval_data['output'] = eval_data['target'].copy()
     elif len({'question', 'answer'} - set(eval_data.keys())) == 0:
         eval_data['output'] = eval_data['answer'].copy()
     elif len({'question', 'output'} - set(eval_data.keys())) == 0:
         pass
     else:
         raise KeyError(
             f'Eval data columns must be either: ["instruction", "input", "output"] or ["prompt", "output"] or ["question", "output"]'
@@ -106,15 +106,15 @@
     if 'model' in eval_results_df.keys():
         print( eval_results_df.groupby('model')['score'])
         score_models = eval_results_df.groupby('model')['score'].apply(lambda x: f'{x.sum():.1f}/{len(x)}')
         print(f'{"-"*20} Scores by Model {"-"*20}\n{score_models.to_markdown()}')
         if 'category' in eval_results_df.keys():
             score_category = eval_results_df.groupby([
                 'model', 'category'
-            ])['score'].apply(lambda x: f'{x.sum():.1f}/{len(x)}').reset_index().sort_values(by='model')
+            ])['score'].apply(lambda x: f'{x.sum():.1f}/{len(x)}').reset_index().sort_values(by='category')
             print(
                 f'\n{"-"*20} Scores by Model and Task Category {"-"*20}\n{score_category.to_markdown(index=False)}'
             )
 
 def save_results(eval_results_df: pd.DataFrame, output_path: str):
     print(f'Saving evaluation results: {output_path}')
     df_saver(eval_results_df, output_path)
@@ -131,20 +131,19 @@
     sample_num: int = 0
     request_interval: int = 1
     retry: bool = True
     verbose: bool = False
     temperature: float = 0.1
     max_new_tokens: int = 2048
 
-def eval_one_file(
+def eval_groups(
     eval_config: EvalConfig
 ):
     # Preparing data
-    eval_data = df_reader(eval_config.eval_data_path)
-    eval_groups = prepare_eval_data(eval_data, eval_config.eval_categories, eval_config.sample_num)
+    eval_groups = prepare_eval_data(eval_config.eval_data_path, eval_config.eval_categories, eval_config.sample_num)
 
     # Init api tool and prompter
     tool = OneAPITool.from_config_file(config_file=eval_config.api_config_file)
 
     eval_results = []
     failed_results = []
     for group in tqdm(eval_groups):
@@ -165,11 +164,12 @@
             time.sleep(eval_config.request_interval)
 
     eval_results.extend(failed_results)
     eval_results_df = pd.concat(eval_results)
     log_score_results(eval_results_df=eval_results_df)
     # Log score results
     print(f'Eval model: {eval_config.model}')
+    print(f'Eval files: {eval_config.eval_data_path}')
     print(f'Failed requests: {len(failed_results)}/{len(eval_groups)}')
     # Save results
     if eval_config.output_path:
         save_results(eval_results_df=eval_results_df, output_path=eval_config.output_path)
```

### Comparing `auto-eval-0.1.3/prompt_template/eval_prompt_template.json` & `auto-eval-0.1.4/prompt_template/eval_prompt_template.json`

 * *Files 26% similar despite different names*

#### Pretty-printed

 * *Similarity: 0.25%*

 * *Differences: {"'eval_with_target_template'": "'[Question]: {question}\\n\\n[Correct answer]: "*

 * *                                '{target}\\n\\n[Candidate '*

 * *                                'answer]:\\n{answers}\\n\\n[System]:\\nPlease solve the [Question] '*

 * *                                'independently to obtain the [Correct answer], and then evaluate '*

 * *                                'and comment each [Candidate answer] based on the [Correct '*

 * *                                'answer]. Finally, output all [Candidate answ […]*

```diff
@@ -1,6 +1,4 @@
 {
-    "eval_with_target_instruction": "Please evaluate and comment each [Candidate answer] based on the [Correct answer]. Then output all [Candidate answer] scores (0-1) in a summary format of {\"number\": \"score\"}, e.g, {\"A\": \"0.2\", \"B\": \"0.8\"}",
-    "eval_with_target_template": "[Question]: {q}\n\n[Correct answer]: {target}\n\n[Candidate answer]:\n{options}\n\n[System]:\n{instruction}",
-    "eval_without_target_instruction": "Please solve the [Question] independently to obtain the [Correct answer], and then evaluate and comment each [Candidate answer] based on the [Correct answer]. Finally, output all [Candidate answers] scores (0-1) in a summary format of {\"number\": \"score\"}, e.g, {\"A\": \"0.2\", \"B\": \"0.8\"}",
-    "eval_without_target_template": "[Question]: {q}\n\n[Candidate answer]:\n{options}\n\n[System]:\n{instruction}"
+    "eval_with_target_template": "[Question]: {question}\n\n[Correct answer]: {target}\n\n[Candidate answer]:\n{answers}\n\n[System]:\nPlease solve the [Question] independently to obtain the [Correct answer], and then evaluate and comment each [Candidate answer] based on the [Correct answer]. Finally, output all [Candidate answers] scores (0-1) in a summary format of {{\"number\": \"score\"}}, e.g, {{\"A\": \"0.2\", \"B\": \"0.8\"}}",
+    "eval_without_target_template": "[Question]: {question}\n\n[Candidate answer]:\n{answers}\n\n[System]:\nPlease evaluate and comment each [Candidate answer] based on the [Correct answer]. Then output all [Candidate answer] scores (0-1) in a summary format of {{\"number\": \"score\"}}, e.g, {{\"A\": \"0.2\", \"B\": \"0.8\"}}"
 }
```

### Comparing `auto-eval-0.1.3/setup.py` & `auto-eval-0.1.4/setup.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from setuptools import setup, find_packages
 
 setup(
     name="auto-eval",
-    version="0.1.3",
+    version="0.1.4",
     packages=find_packages(),
     package_data={
       "prompt_template":["eval_prompt_template.json"]  
     },
     install_requires=[
         # Add your library's dependencies here
         "one-api-tool",
```

### Comparing `auto-eval-0.1.3/utils/data_utils.py` & `auto-eval-0.1.4/utils/data_utils.py`

 * *Files identical despite different names*

