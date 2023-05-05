# Comparing `tmp/rellm-0.0.2.tar.gz` & `tmp/rellm-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "rellm-0.0.2.tar", max compression
+gzip compressed data, was "rellm-0.0.3.tar", max compression
```

## Comparing `rellm-0.0.2.tar` & `rellm-0.0.3.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0     1069 2023-05-05 02:22:49.141576 rellm-0.0.2/LICENSE
--rw-r--r--   0        0        0     2875 2023-05-05 02:53:28.095668 rellm-0.0.2/README.md
--rw-r--r--   0        0        0     1248 2023-05-05 03:43:53.699219 rellm-0.0.2/pyproject.toml
--rw-r--r--   0        0        0       35 2023-05-05 03:43:20.860386 rellm-0.0.2/rellm/__init__.py
--rw-r--r--   0        0        0     2698 2023-05-05 03:43:16.227349 rellm-0.0.2/rellm/rellm.py
--rw-r--r--   0        0        0     3723 1970-01-01 00:00:00.000000 rellm-0.0.2/setup.py
--rw-r--r--   0        0        0     4343 1970-01-01 00:00:00.000000 rellm-0.0.2/PKG-INFO
+-rw-r--r--   0        0        0     1069 2023-05-05 02:22:49.141576 rellm-0.0.3/LICENSE
+-rw-r--r--   0        0        0     3536 2023-05-05 03:49:02.216077 rellm-0.0.3/README.md
+-rw-r--r--   0        0        0     1265 2023-05-05 03:49:14.257547 rellm-0.0.3/pyproject.toml
+-rw-r--r--   0        0        0       35 2023-05-05 03:43:20.860386 rellm-0.0.3/rellm/__init__.py
+-rw-r--r--   0        0        0     2698 2023-05-05 03:43:16.227349 rellm-0.0.3/rellm/rellm.py
+-rw-r--r--   0        0        0     4435 1970-01-01 00:00:00.000000 rellm-0.0.3/setup.py
+-rw-r--r--   0        0        0     5042 1970-01-01 00:00:00.000000 rellm-0.0.3/PKG-INFO
```

### Comparing `rellm-0.0.2/LICENSE` & `rellm-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `rellm-0.0.2/README.md` & `rellm-0.0.3/README.md`

 * *Files 15% similar despite different names*

```diff
@@ -10,14 +10,39 @@
 ### Installation
 ```
 pip install rellm
 ```
 
 The preliminary results are interesting -- even for small models, constraining the token space with ReLLM can improve the quality of the completions. Not to mention the ability to more easily parse the output programmatically. Take a look at some of the examples below (you can run them with [example.py](example.py))
 
+```python
+import regex
+from transformers import AutoModelForCausalLM, AutoTokenizer
+
+from rellm import complete_re
+
+model = AutoModelForCausalLM.from_pretrained("gpt2")
+tokenizer = AutoTokenizer.from_pretrained("gpt2")
+
+prompt = "ReLLM, the best way to get structured data out of LLMs, is an acronym for "
+pattern = regex.compile(r'Re[a-z]+ L[a-z]+ L[a-z]+ M[a-z]+')
+output = complete_re(tokenizer=tokenizer, 
+                     model=model, 
+                     prompt=prompt,
+                     pattern=pattern,
+                     do_sample=True,
+                     max_new_tokens=80)
+print(output)
+```
+
+```
+> Realized Logistic Logistics Model
+```
+
+
 ## Examples using GPT2 (124 million parameters)
 
 **Prompt**: Return the first three letters of the alphabet in a json array:
 
 **Pattern** \[\"[a-z]\", \"[a-z]\", \"[a-z]\"\]
 
 **ReLLM**: ["a", "b", "c"]
@@ -78,12 +103,12 @@
 
 "Why, I don't understand. What did you mean by
 
 #
 
 **Prompt**: ReLLM, the best way to get structured data out of LLMs, is an acronym for
 
-**Patern**: Re[a-z]* L[a-z]* L[a-z]* M[a-z]*
+**Patern**: Re[a-z]+ L[a-z]+ L[a-z]+ M[a-z]+
 
 **ReLLM**: Realized Logistic Logistics Model
 
 **Without ReLLM**: Largest Largest Address Space (MELSP), which has its roots in the  Internet network, at least when compared
```

### Comparing `rellm-0.0.2/pyproject.toml` & `rellm-0.0.3/pyproject.toml`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "rellm"
-version = "0.0.2"
+version = "0.0.3"
 description = "Get exact structure out of any language models with regular expressions."
 authors = ["Matt Rickard <pypi@matt-rickard.com>"]
 maintainers = ["Matt Rickard <pypi@matt-rickard.com>"]
 readme = "README.md"
 license = "MIT"
 keywords = [
   "llm",
@@ -31,14 +31,15 @@
 urls = { repository = "https://github.com/r2d4/rellm" }
 
 [tool.poetry.dependencies]
 python = "^3.8"
 regex = "^2023.5.5"
 transformers = "^4.28.1"
 numpy = "^1.24.3"
+torch = "^2.0.0"
 
 [build-system]
 requires = ["poetry-core"]
 build-backend = "poetry.core.masonry.api"
 
 [tool.ruff]
 line-length = 119
```

### Comparing `rellm-0.0.2/rellm/rellm.py` & `rellm-0.0.3/rellm/rellm.py`

 * *Files identical despite different names*

### Comparing `rellm-0.0.2/setup.py` & `rellm-0.0.3/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -6,21 +6,22 @@
 
 package_data = \
 {'': ['*']}
 
 install_requires = \
 ['numpy>=1.24.3,<2.0.0',
  'regex>=2023.5.5,<2024.0.0',
+ 'torch>=2.0.0,<3.0.0',
  'transformers>=4.28.1,<5.0.0']
 
 setup_kwargs = {
     'name': 'rellm',
-    'version': '0.0.2',
+    'version': '0.0.3',
     'description': 'Get exact structure out of any language models with regular expressions.',
-    'long_description': '# ReLLM\nRegular Expressions for Language Model Completions.\n\nGet exact structure out of any language model completion with regular expressions.\n\nReturn specific syntactic structure (e.g. JSON or XML), or specific semantic structure (e.g. a date or a number), or even complete templates (e.g. a sentence with a blank to fill in).\n\nHow does it work? For each token, ReLLM tests every possible completion against a partial regex. For the potential completions that do not match the pattern, ReLLM masks the logits so that the language model does not generate them.\n\n### Installation\n```\npip install rellm\n```\n\nThe preliminary results are interesting -- even for small models, constraining the token space with ReLLM can improve the quality of the completions. Not to mention the ability to more easily parse the output programmatically. Take a look at some of the examples below (you can run them with [example.py](example.py))\n\n## Examples using GPT2 (124 million parameters)\n\n**Prompt**: Return the first three letters of the alphabet in a json array:\n\n**Pattern** \\[\\"[a-z]\\", \\"[a-z]\\", \\"[a-z]\\"\\]\n\n**ReLLM**: ["a", "b", "c"]\n\n**Without ReLLM**: { "index": 0, "id":"1", "description":"", "text": "[{ "id": 0, "name":\n#\n**Prompt**: Fill in the sentence with an interesting story about the dentist:\n\n**Pattern**: Today I\\\'m going to the [a-z]+ to [a-z]+ because ([a-z]+ )*\\.\n\n**ReLLM**: Today I\'m going to the dentist to see because it is a very important day for me\n\n**Without ReLLM**: \'My family bought me an appointment with a dentist when I was 15. The dentist gave me one a year and then I was told on\n#\n\n**Prompt**: Is this a good demo?\n\n**Pattern**: (Yes|No)\n\n**ReLLM**: No.\n\n**Without ReLLM**: I don\'t know, but this is amazing! Even more amazing is how the design can take place on a small stage that uses LEDs.\nAs\n\n#\n\n**Prompt**: Convert the date May 4, 2023 to the format mm/dd/yyyy:\n\n**Pattern**: [0-9]{2}/[0-9]{2}/[0-9]{4}\n\n**ReLLM**: 00/00/0045\n\n**Without ReLLM**:  mm:ss\n\nA-Z, Z-A, W-H (0-9:9:19)\n\nZ-R\n\n#\n\n**Prompt**: Jeff Dean is a\n\n**Pattern** (Programmer|Computer Scientist|AGI)\n\n**ReLLM**: Computer Scientist\n\n**Without ReLLM**: former national basketball champion and a former professional basketball player. He currently serves as general counsel for the NCAA Office of the Vice President for Academic Affairs.\n\n#\n\n**Prompt**: I can eat \n\n**Pattern**: [0-9]{1,10} [a-z]* of [a-z]*\n\n**ReLLM**: 800 calories of coffee\n\n**Without ReLLM**: iced coffee here on the west side and do this, so can you?"\n\n"Why, I don\'t understand. What did you mean by\n\n#\n\n**Prompt**: ReLLM, the best way to get structured data out of LLMs, is an acronym for\n\n**Patern**: Re[a-z]* L[a-z]* L[a-z]* M[a-z]*\n\n**ReLLM**: Realized Logistic Logistics Model\n\n**Without ReLLM**: Largest Largest Address Space (MELSP), which has its roots in the  Internet network, at least when compared\n',
+    'long_description': '# ReLLM\nRegular Expressions for Language Model Completions.\n\nGet exact structure out of any language model completion with regular expressions.\n\nReturn specific syntactic structure (e.g. JSON or XML), or specific semantic structure (e.g. a date or a number), or even complete templates (e.g. a sentence with a blank to fill in).\n\nHow does it work? For each token, ReLLM tests every possible completion against a partial regex. For the potential completions that do not match the pattern, ReLLM masks the logits so that the language model does not generate them.\n\n### Installation\n```\npip install rellm\n```\n\nThe preliminary results are interesting -- even for small models, constraining the token space with ReLLM can improve the quality of the completions. Not to mention the ability to more easily parse the output programmatically. Take a look at some of the examples below (you can run them with [example.py](example.py))\n\n```python\nimport regex\nfrom transformers import AutoModelForCausalLM, AutoTokenizer\n\nfrom rellm import complete_re\n\nmodel = AutoModelForCausalLM.from_pretrained("gpt2")\ntokenizer = AutoTokenizer.from_pretrained("gpt2")\n\nprompt = "ReLLM, the best way to get structured data out of LLMs, is an acronym for "\npattern = regex.compile(r\'Re[a-z]+ L[a-z]+ L[a-z]+ M[a-z]+\')\noutput = complete_re(tokenizer=tokenizer, \n                     model=model, \n                     prompt=prompt,\n                     pattern=pattern,\n                     do_sample=True,\n                     max_new_tokens=80)\nprint(output)\n```\n\n```\n> Realized Logistic Logistics Model\n```\n\n\n## Examples using GPT2 (124 million parameters)\n\n**Prompt**: Return the first three letters of the alphabet in a json array:\n\n**Pattern** \\[\\"[a-z]\\", \\"[a-z]\\", \\"[a-z]\\"\\]\n\n**ReLLM**: ["a", "b", "c"]\n\n**Without ReLLM**: { "index": 0, "id":"1", "description":"", "text": "[{ "id": 0, "name":\n#\n**Prompt**: Fill in the sentence with an interesting story about the dentist:\n\n**Pattern**: Today I\\\'m going to the [a-z]+ to [a-z]+ because ([a-z]+ )*\\.\n\n**ReLLM**: Today I\'m going to the dentist to see because it is a very important day for me\n\n**Without ReLLM**: \'My family bought me an appointment with a dentist when I was 15. The dentist gave me one a year and then I was told on\n#\n\n**Prompt**: Is this a good demo?\n\n**Pattern**: (Yes|No)\n\n**ReLLM**: No.\n\n**Without ReLLM**: I don\'t know, but this is amazing! Even more amazing is how the design can take place on a small stage that uses LEDs.\nAs\n\n#\n\n**Prompt**: Convert the date May 4, 2023 to the format mm/dd/yyyy:\n\n**Pattern**: [0-9]{2}/[0-9]{2}/[0-9]{4}\n\n**ReLLM**: 00/00/0045\n\n**Without ReLLM**:  mm:ss\n\nA-Z, Z-A, W-H (0-9:9:19)\n\nZ-R\n\n#\n\n**Prompt**: Jeff Dean is a\n\n**Pattern** (Programmer|Computer Scientist|AGI)\n\n**ReLLM**: Computer Scientist\n\n**Without ReLLM**: former national basketball champion and a former professional basketball player. He currently serves as general counsel for the NCAA Office of the Vice President for Academic Affairs.\n\n#\n\n**Prompt**: I can eat \n\n**Pattern**: [0-9]{1,10} [a-z]* of [a-z]*\n\n**ReLLM**: 800 calories of coffee\n\n**Without ReLLM**: iced coffee here on the west side and do this, so can you?"\n\n"Why, I don\'t understand. What did you mean by\n\n#\n\n**Prompt**: ReLLM, the best way to get structured data out of LLMs, is an acronym for\n\n**Patern**: Re[a-z]+ L[a-z]+ L[a-z]+ M[a-z]+\n\n**ReLLM**: Realized Logistic Logistics Model\n\n**Without ReLLM**: Largest Largest Address Space (MELSP), which has its roots in the  Internet network, at least when compared\n',
     'author': 'Matt Rickard',
     'author_email': 'pypi@matt-rickard.com',
     'maintainer': 'Matt Rickard',
     'maintainer_email': 'pypi@matt-rickard.com',
     'url': 'None',
     'packages': packages,
     'package_data': package_data,
```

### Comparing `rellm-0.0.2/PKG-INFO` & `rellm-0.0.3/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: rellm
-Version: 0.0.2
+Version: 0.0.3
 Summary: Get exact structure out of any language models with regular expressions.
 License: MIT
 Keywords: llm,ai,prompt,large language models,gpt-3,chatgpt
 Author: Matt Rickard
 Author-email: pypi@matt-rickard.com
 Maintainer: Matt Rickard
 Maintainer-email: pypi@matt-rickard.com
@@ -24,14 +24,15 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Scientific/Engineering :: Artificial Intelligence
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Topic :: Text Processing :: Linguistic
 Requires-Dist: numpy (>=1.24.3,<2.0.0)
 Requires-Dist: regex (>=2023.5.5,<2024.0.0)
+Requires-Dist: torch (>=2.0.0,<3.0.0)
 Requires-Dist: transformers (>=4.28.1,<5.0.0)
 Project-URL: repository, https://github.com/r2d4/rellm
 Description-Content-Type: text/markdown
 
 # ReLLM
 Regular Expressions for Language Model Completions.
 
@@ -44,14 +45,39 @@
 ### Installation
 ```
 pip install rellm
 ```
 
 The preliminary results are interesting -- even for small models, constraining the token space with ReLLM can improve the quality of the completions. Not to mention the ability to more easily parse the output programmatically. Take a look at some of the examples below (you can run them with [example.py](example.py))
 
+```python
+import regex
+from transformers import AutoModelForCausalLM, AutoTokenizer
+
+from rellm import complete_re
+
+model = AutoModelForCausalLM.from_pretrained("gpt2")
+tokenizer = AutoTokenizer.from_pretrained("gpt2")
+
+prompt = "ReLLM, the best way to get structured data out of LLMs, is an acronym for "
+pattern = regex.compile(r'Re[a-z]+ L[a-z]+ L[a-z]+ M[a-z]+')
+output = complete_re(tokenizer=tokenizer, 
+                     model=model, 
+                     prompt=prompt,
+                     pattern=pattern,
+                     do_sample=True,
+                     max_new_tokens=80)
+print(output)
+```
+
+```
+> Realized Logistic Logistics Model
+```
+
+
 ## Examples using GPT2 (124 million parameters)
 
 **Prompt**: Return the first three letters of the alphabet in a json array:
 
 **Pattern** \[\"[a-z]\", \"[a-z]\", \"[a-z]\"\]
 
 **ReLLM**: ["a", "b", "c"]
@@ -112,13 +138,13 @@
 
 "Why, I don't understand. What did you mean by
 
 #
 
 **Prompt**: ReLLM, the best way to get structured data out of LLMs, is an acronym for
 
-**Patern**: Re[a-z]* L[a-z]* L[a-z]* M[a-z]*
+**Patern**: Re[a-z]+ L[a-z]+ L[a-z]+ M[a-z]+
 
 **ReLLM**: Realized Logistic Logistics Model
 
 **Without ReLLM**: Largest Largest Address Space (MELSP), which has its roots in the  Internet network, at least when compared
```

