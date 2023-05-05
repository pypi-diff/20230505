# Comparing `tmp/AIPrompts-0.3.0.tar.gz` & `tmp/AIPrompts-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "AIPrompts-0.3.0.tar", last modified: Fri Mar 17 13:47:55 2023, max compression
+gzip compressed data, was "AIPrompts-0.4.0.tar", last modified: Fri May  5 01:56:56 2023, max compression
```

## Comparing `AIPrompts-0.3.0.tar` & `AIPrompts-0.4.0.tar`

### file list

```diff
@@ -1,26 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-17 13:47:55.510622 AIPrompts-0.3.0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-17 13:47:55.510622 AIPrompts-0.3.0/AIPrompts.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2579 2023-03-17 13:47:55.000000 AIPrompts-0.3.0/AIPrompts.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      434 2023-03-17 13:47:55.000000 AIPrompts-0.3.0/AIPrompts.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-17 13:47:55.000000 AIPrompts-0.3.0/AIPrompts.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-03-17 13:47:55.000000 AIPrompts-0.3.0/AIPrompts.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-03-17 13:47:55.000000 AIPrompts-0.3.0/AIPrompts.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-03-17 13:47:37.000000 AIPrompts-0.3.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2579 2023-03-17 13:47:55.510622 AIPrompts-0.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2263 2023-03-17 13:47:37.000000 AIPrompts-0.3.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-17 13:47:55.510622 AIPrompts-0.3.0/prompts/
--rw-r--r--   0 runner    (1001) docker     (123)       85 2023-03-17 13:47:37.000000 AIPrompts-0.3.0/prompts/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2911 2023-03-17 13:47:37.000000 AIPrompts-0.3.0/prompts/ensemble.py
--rw-r--r--   0 runner    (1001) docker     (123)      637 2023-03-17 13:47:37.000000 AIPrompts-0.3.0/prompts/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)     3819 2023-03-17 13:47:37.000000 AIPrompts-0.3.0/prompts/prompt_builder.py
--rw-r--r--   0 runner    (1001) docker     (123)     5988 2023-03-17 13:47:37.000000 AIPrompts-0.3.0/prompts/turbo.py
--rw-r--r--   0 runner    (1001) docker     (123)      150 2023-03-17 13:47:37.000000 AIPrompts-0.3.0/prompts/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)      140 2023-03-17 13:47:37.000000 AIPrompts-0.3.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-03-17 13:47:37.000000 AIPrompts-0.3.0/requirements-test.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-03-17 13:47:37.000000 AIPrompts-0.3.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-17 13:47:55.510622 AIPrompts-0.3.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1395 2023-03-17 13:47:37.000000 AIPrompts-0.3.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-17 13:47:55.510622 AIPrompts-0.3.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)     4563 2023-03-17 13:47:37.000000 AIPrompts-0.3.0/tests/test_ensemble.py
--rw-r--r--   0 runner    (1001) docker     (123)     2017 2023-03-17 13:47:37.000000 AIPrompts-0.3.0/tests/test_prompt.py
--rw-r--r--   0 runner    (1001) docker     (123)     3679 2023-03-17 13:47:37.000000 AIPrompts-0.3.0/tests/test_turbo.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 01:56:56.391970 AIPrompts-0.4.0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 01:56:56.387970 AIPrompts-0.4.0/AIPrompts.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2579 2023-05-05 01:56:56.000000 AIPrompts-0.4.0/AIPrompts.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      446 2023-05-05 01:56:56.000000 AIPrompts-0.4.0/AIPrompts.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 01:56:56.000000 AIPrompts-0.4.0/AIPrompts.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-05-05 01:56:56.000000 AIPrompts-0.4.0/AIPrompts.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-05 01:56:56.000000 AIPrompts-0.4.0/AIPrompts.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-05 01:56:41.000000 AIPrompts-0.4.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2579 2023-05-05 01:56:56.391970 AIPrompts-0.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2263 2023-05-05 01:56:41.000000 AIPrompts-0.4.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 01:56:56.391970 AIPrompts-0.4.0/prompts/
+-rw-r--r--   0 runner    (1001) docker     (123)      221 2023-05-05 01:56:41.000000 AIPrompts-0.4.0/prompts/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2080 2023-05-05 01:56:41.000000 AIPrompts-0.4.0/prompts/dynamic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3076 2023-05-05 01:56:41.000000 AIPrompts-0.4.0/prompts/ensemble.py
+-rw-r--r--   0 runner    (1001) docker     (123)      637 2023-05-05 01:56:41.000000 AIPrompts-0.4.0/prompts/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1516 2023-05-05 01:56:41.000000 AIPrompts-0.4.0/prompts/schemas.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8714 2023-05-05 01:56:41.000000 AIPrompts-0.4.0/prompts/turbo.py
+-rw-r--r--   0 runner    (1001) docker     (123)      169 2023-05-05 01:56:41.000000 AIPrompts-0.4.0/prompts/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)      140 2023-05-05 01:56:41.000000 AIPrompts-0.4.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-05 01:56:41.000000 AIPrompts-0.4.0/requirements-test.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-05-05 01:56:41.000000 AIPrompts-0.4.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-05 01:56:56.391970 AIPrompts-0.4.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1395 2023-05-05 01:56:41.000000 AIPrompts-0.4.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 01:56:56.391970 AIPrompts-0.4.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)     3973 2023-05-05 01:56:41.000000 AIPrompts-0.4.0/tests/test_ensemble.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1734 2023-05-05 01:56:41.000000 AIPrompts-0.4.0/tests/test_prompt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5107 2023-05-05 01:56:41.000000 AIPrompts-0.4.0/tests/test_turbo.py
```

### Comparing `AIPrompts-0.3.0/AIPrompts.egg-info/PKG-INFO` & `AIPrompts-0.4.0/AIPrompts.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: AIPrompts
-Version: 0.3.0
+Version: 0.4.0
 Summary: Create and parse prompts for large language models.
 Home-page: https://github.com/TeiaLabs/prompts
 Author: Teialabs
 Author-email: jonatas@teialabs.com
 Keywords: prompt openai teialabs gpt3
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
@@ -57,15 +57,15 @@
         return self.set_prompt_values(
             input_sentence=input_sentence,
         )
 ```
 
 ## Ensembling prompts
 
-To ensemble multiple prompts, you can use the `EnsemblePrompt` class:
+To ensemble multiple prompts, you can use the `PromptEnsemble` class:
 
 ```python
 templates = [
     '<label>', 
     'a photo of <label>', 
     'picture of <label>',
 ]
```

### Comparing `AIPrompts-0.3.0/PKG-INFO` & `AIPrompts-0.4.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: AIPrompts
-Version: 0.3.0
+Version: 0.4.0
 Summary: Create and parse prompts for large language models.
 Home-page: https://github.com/TeiaLabs/prompts
 Author: Teialabs
 Author-email: jonatas@teialabs.com
 Keywords: prompt openai teialabs gpt3
 Requires-Python: >=3.10
 Description-Content-Type: text/markdown
@@ -57,15 +57,15 @@
         return self.set_prompt_values(
             input_sentence=input_sentence,
         )
 ```
 
 ## Ensembling prompts
 
-To ensemble multiple prompts, you can use the `EnsemblePrompt` class:
+To ensemble multiple prompts, you can use the `PromptEnsemble` class:
 
 ```python
 templates = [
     '<label>', 
     'a photo of <label>', 
     'picture of <label>',
 ]
```

### Comparing `AIPrompts-0.3.0/README.md` & `AIPrompts-0.4.0/README.md`

 * *Files 4% similar despite different names*

```diff
@@ -46,15 +46,15 @@
         return self.set_prompt_values(
             input_sentence=input_sentence,
         )
 ```
 
 ## Ensembling prompts
 
-To ensemble multiple prompts, you can use the `EnsemblePrompt` class:
+To ensemble multiple prompts, you can use the `PromptEnsemble` class:
 
 ```python
 templates = [
     '<label>', 
     'a photo of <label>', 
     'picture of <label>',
 ]
```

### Comparing `AIPrompts-0.3.0/prompts/ensemble.py` & `AIPrompts-0.4.0/prompts/ensemble.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,21 +1,21 @@
 from __future__ import annotations
 
 from typing import Optional, Type
 
+from .dynamic import DynamicPrompt
 from .exceptions import ArgumentNumberOfElementsError, ExpectedVarsArgumentError
-from .prompt_builder import BasePrompt, DynamicPrompt
 
 
 class PromptEnsemble:
     def __init__(
         self,
-        templates: list[str] | Type[BasePrompt],
+        templates: list[str],
         expected_vars: Optional[list[str]] = None,
-        prompt_class=DynamicPrompt,
+        prompt_class: Type[DynamicPrompt] = DynamicPrompt,
     ):
         """
         Args:
             templates: templates with placeholder variable names
             expected_vars: variables expected in all templates
             prompt_class: allows custom prompt classes
 
@@ -29,15 +29,22 @@
         self.prompts = []
         for template in templates:
             if isinstance(template, str):
                 if expected_vars is None:
                     raise ExpectedVarsArgumentError(
                         "expected_vars argument is mandatory when using string templates"
                     )
-                self.prompts.append(prompt_class(template, expected_vars))
+
+                prompt = prompt_class(
+                    name="",
+                    description="",
+                    template=template,
+                    template_vars=expected_vars,
+                )
+                self.prompts.append(prompt)
             else:
                 self.prompts.append(template)
 
     def build(self, **kwargs) -> list:
         """
         Example:
         ```
```

### Comparing `AIPrompts-0.3.0/prompts/exceptions.py` & `AIPrompts-0.4.0/prompts/exceptions.py`

 * *Files identical despite different names*

### Comparing `AIPrompts-0.3.0/setup.py` & `AIPrompts-0.4.0/setup.py`

 * *Files identical despite different names*

### Comparing `AIPrompts-0.3.0/tests/test_ensemble.py` & `AIPrompts-0.4.0/tests/test_ensemble.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,166 +1,141 @@
 import pytest
 
 from prompts import DynamicPrompt, exceptions
 from prompts.ensemble import PromptEnsemble
 
 
 def test_ensemble():
-    templates = ['<label>', 'a photo of <label>', 'picture of <label>']
-    template_vars = ['label']
-    
+    templates = ["<label>", "a photo of <label>", "picture of <label>"]
+    template_vars = ["label"]
+
     prompt = PromptEnsemble(templates, template_vars)
 
-    prompted_list = prompt.build(label='dog')    
+    prompted_list = prompt.build(label="dog")
 
     assert len(prompted_list) == 3
-    assert prompted_list[0] == 'dog'
-    assert prompted_list[1] == 'a photo of dog'
-    assert prompted_list[2] == 'picture of dog'
+    assert prompted_list[0] == "dog"
+    assert prompted_list[1] == "a photo of dog"
+    assert prompted_list[2] == "picture of dog"
 
     with pytest.raises(exceptions.UndefinedVariableError):
-        _ = prompt.build(img_class='cat')
+        _ = prompt.build(img_class="cat")
 
     assert len(prompt) == 3
 
 
 def test_build_missing_args_valid():
-    templates = ['<label>/<superclass>', 'a photo of <label>']
-    template_vars = ['label', 'superclass']
+    templates = ["<label>/<superclass>", "a photo of <label>"]
+    template_vars = ["label", "superclass"]
 
     prompt = PromptEnsemble(templates, template_vars)
 
     prompted_list = prompt.build(
-        label='dog',
-        superclass='animal',
+        label="dog",
+        superclass="animal",
         strict=False,
     )
-    expected = ['dog/animal', 'a photo of dog']
+    expected = ["dog/animal", "a photo of dog"]
 
     assert len(prompted_list) == 2
     assert prompted_list == expected
 
 
 def test_build_missing_args():
-    templates = ['<label>/<superclass>', 'a photo of <label>']    
+    templates = ["<label>/<superclass>", "a photo of <label>"]
 
     with pytest.raises(exceptions.ExpectedVarsArgumentError):
         PromptEnsemble(templates, expected_vars=None)
 
 
-def test_build_missing_args_invalid():
-    templates = ['<label>', 'test']
-    template_vars = ['label']
-
-    with pytest.raises(exceptions.VariableNotInPromptError):
-        _ = PromptEnsemble(templates, template_vars)
-
-
 def test_build_many():
-    templates = ['<label>', 'a photo of <label>']
-    template_vars = ['label']
-    classes = ['dog', 'cat', 'horse']
-    
+    templates = ["<label>", "a photo of <label>"]
+    template_vars = ["label"]
+    classes = ["dog", "cat", "horse"]
+
     prompt = PromptEnsemble(templates, template_vars)
 
-    prompted_list = prompt.build_many(label=classes)    
+    prompted_list = prompt.build_many(label=classes)
 
     assert len(prompted_list) == 6
-    assert prompted_list[0] == 'dog'
-    assert prompted_list[1] == 'a photo of dog'
-    assert prompted_list[2] == 'cat'
-    assert prompted_list[3] == 'a photo of cat'
-    assert prompted_list[4] == 'horse'
-    assert prompted_list[5] == 'a photo of horse'
+    assert prompted_list[0] == "dog"
+    assert prompted_list[1] == "a photo of dog"
+    assert prompted_list[2] == "cat"
+    assert prompted_list[3] == "a photo of cat"
+    assert prompted_list[4] == "horse"
+    assert prompted_list[5] == "a photo of horse"
 
     with pytest.raises(exceptions.UndefinedVariableError):
-        _ = prompt.build(labels=['cat'])
+        _ = prompt.build(random=["cat"])
 
 
 def test_build_many_multiple_args():
-    templates = ['<label>/<superclass>', 'a photo of <label>/<superclass>']
-    template_vars = ['label', 'superclass']
-    labels = ['dog', 'cat', 't-shirt']
-    superclasses = ['animal', 'animal', 'clothes']
-    
+    templates = ["<label>/<superclass>", "a photo of <label>/<superclass>"]
+    template_vars = ["label", "superclass"]
+    labels = ["dog", "cat", "t-shirt"]
+    superclasses = ["animal", "animal", "clothes"]
+
     prompt = PromptEnsemble(templates, template_vars)
 
     prompted_list = prompt.build_many(
         label=labels,
         superclass=superclasses,
     )
     expected = [
-        'dog/animal', 
-        'a photo of dog/animal', 
-        'cat/animal', 
-        'a photo of cat/animal', 
-        't-shirt/clothes', 
-        'a photo of t-shirt/clothes',
+        "dog/animal",
+        "a photo of dog/animal",
+        "cat/animal",
+        "a photo of cat/animal",
+        "t-shirt/clothes",
+        "a photo of t-shirt/clothes",
     ]
 
     assert prompted_list == expected
 
-    # Test error 
+    # Test error
     with pytest.raises(exceptions.ArgumentNumberOfElementsError):
         prompted_list = prompt.build_many(
             label=labels,
             superclass=superclasses[:-1],
         )
 
 
 def test_build_many_missing_args_valid():
-    templates = ['<label>/<superclass>', 'a photo of <label>']
-    template_vars = ['label', 'superclass']
-    labels = ['dog', 'cat', 't-shirt']
-    superclasses = ['animal', 'animal', 'clothes']
+    templates = ["<label>/<superclass>", "a photo of <label>"]
+    template_vars = ["label", "superclass"]
+    labels = ["dog", "cat", "t-shirt"]
+    superclasses = ["animal", "animal", "clothes"]
 
     prompt = PromptEnsemble(templates, template_vars)
 
     prompted_list = prompt.build_many(
         label=labels,
         superclass=superclasses,
         strict=False,
     )
     expected = [
-        'dog/animal',
-        'a photo of dog',
-        'cat/animal',
-        'a photo of cat',
-        't-shirt/clothes',
-        'a photo of t-shirt',
+        "dog/animal",
+        "a photo of dog",
+        "cat/animal",
+        "a photo of cat",
+        "t-shirt/clothes",
+        "a photo of t-shirt",
     ]
 
     assert len(prompted_list) == 6
     assert prompted_list == expected
 
 
-def test_invalid_ensemble_template():
-    templates = ['<label>', 'a photo of <img_class>', 'picture of <label>']
-    template_vars = ['label']
-
-   # expect exception
-    with pytest.raises(exceptions.VariableNotInPromptError):
-        _ = PromptEnsemble(templates, template_vars)
-
-
 def test_prompt_ensemble_from_file():
     prompts = []
-    for i in range(3):
-        prompt_file = 'samples/sample.prompt.yaml'
+    prompt_file = "samples/sample.prompt.yaml"
+    for _ in range(3):
         prompt = DynamicPrompt.from_file(prompt_file)
         prompts.append(prompt)
-    
+
     prompt_ens = PromptEnsemble(prompts)
-    prompt_str = prompt_ens.build(
-        input_sentence='lets go'
-    )
+    prompt_str = prompt_ens.build(input_sentence="lets go")
     assert len(prompt_str) == 3
 
-    prompt_ens_ff = PromptEnsemble.from_paths(
-        [prompt_file, prompt_file, prompt_file]
-    )
-
-    prompt_ff = prompt_ens_ff.build(
-        input_sentence='lets go'
-    )
-
-    assert prompt_ff == prompt_str    
+    prompt_ens_ff = PromptEnsemble.from_paths([prompt_file, prompt_file, prompt_file])
+    prompt_ff = prompt_ens_ff.build(input_sentence="lets go")
+    assert prompt_ff == prompt_str
```

### Comparing `AIPrompts-0.3.0/tests/test_prompt.py` & `AIPrompts-0.4.0/tests/test_prompt.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 import pytest
 
-from prompts import BasePrompt, DynamicPrompt, exceptions
+from prompts import DynamicPrompt, exceptions
 
 
 class TestPrompt:
     
     template = 'a photo of a <img_label>'
-    template_vars = 'img_label'
+    template_vars = ['img_label']
 
     @staticmethod
     def test_prompt_from_file():
         prompt_file = 'samples/sample.prompt.yaml'
         prompt = DynamicPrompt.from_file(prompt_file)
         prompt_str = prompt.build(input_sentence='lets go')
         assert 'lets go' in prompt_str
@@ -18,42 +18,35 @@
             'Fix and improve writing of the sentence below:\n'
             'lets go\n'
             '\n'
             'Fixed sentence:\n'
         ))
         assert expected_prompt == prompt_str
 
-        settings = prompt.get_model_settings()
+        settings = prompt.settings
         assert isinstance(settings, dict)
         assert isinstance(settings['temperature'], float)
         assert settings['temperature'] == 0.15
         assert settings['engine'] == 'text-davinci-003'
 
     @staticmethod
     def test_str_prompt():
 
         prompt = DynamicPrompt(TestPrompt.template, TestPrompt.template_vars)
         filled_prompt = prompt.build(img_label='dog')
-        assert filled_prompt == 'a photo of a dog'
-
-    @staticmethod
-    def test_base_prompt():
-        # it has to throw exception because the build method is not implemented
-        with pytest.raises(exceptions.MissingArgumentError):
-            BasePrompt(TestPrompt.template, TestPrompt.template_vars)        
+        assert filled_prompt == 'a photo of a dog'      
 
     @staticmethod
     def test_str_prompt_without_vars():
         prompt = DynamicPrompt(TestPrompt.template)
         filled_prompt = prompt.build(img_label='dog')
         assert filled_prompt == 'a photo of a dog'
         
         with pytest.raises(exceptions.UndefinedVariableError):
             filled_prompt = prompt.build(img_labels='dog')
 
     @staticmethod
     def test_strict_mode():
-
         prompt = DynamicPrompt(TestPrompt.template, TestPrompt.template_vars)
         filled_prompt = prompt.build(
             strict=False, img_label='dog', animal='mamal')
         assert filled_prompt == 'a photo of a dog'
```

### Comparing `AIPrompts-0.3.0/tests/test_turbo.py` & `AIPrompts-0.4.0/tests/test_turbo.py`

 * *Files 25% similar despite different names*

```diff
@@ -1,45 +1,59 @@
-from prompts import DynamicPrompt
-from prompts.turbo import TurboPrompt
+from prompts import (
+    DynamicPrompt,
+    OpenAIModelSettings,
+    PromptRole,
+    TemplateContent,
+    TurboPrompt,
+)
 
 
 def test_turbo_all_none():
     tp = TurboPrompt()
     assert len(tp.prompts) == 0
     tp.add_system_message(message="You are an AI system that fixes text")
     tp.add_user_message(message="fix this text: she no went to the store")
     tp.add_assistant_message(message="fixed text: she did not go to the store")
     tp.add_user_message(message="fix this text: he is no smart")
-    
+
     assert len(tp.prompts) == 4
-    
+
     text = tp.build()
     expected = [
-        {"role": "system", "content": "You are an AI system that fixes text"},
-        {"role": "user", "content": "fix this text: she no went to the store"},
-        {"role": "assistant", "content": "fixed text: she did not go to the store"},
+        {
+            "role": "system",
+            "content": "You are an AI system that fixes text",
+        },
+        {
+            "role": "user",
+            "content": "fix this text: she no went to the store",
+        },
+        {
+            "role": "assistant",
+            "content": "fixed text: she did not go to the store",
+        },
         {"role": "user", "content": "fix this text: he is no smart"},
     ]
 
     assert text == expected
-    
+
 
 def test_turbo():
     system = DynamicPrompt("<message>")
-    user = DynamicPrompt("<name>: <message>")
+    user = DynamicPrompt("<user_name>: <message>")
     assistant = DynamicPrompt("answer: <message>")
 
     tp = TurboPrompt(
-        system_prompt=system,
-        user_prompt=user,
-        assistant_prompt=assistant,
+        system_templates=system,
+        user_templates=user,
+        assistant_templates=assistant,
     )
     assert len(tp.prompts) == 0
     tp.add_system_message(message="You are a chatbot")
-    tp.add_user_message(name="Qui-gon", message="may the force")
+    tp.add_user_message(user_name="Qui-gon", message="may the force")
     tp.add_assistant_message(message="be with you")
     assert len(tp.prompts) == 3
     text = tp.build()
     expected = [
         {"role": "system", "content": "You are a chatbot"},
         {"role": "user", "content": "Qui-gon: may the force"},
         {"role": "assistant", "content": "answer: be with you"},
@@ -47,41 +61,57 @@
     assert text == expected
 
 
 def test_from_file():
     tp = TurboPrompt.from_file("samples/turbo.prompt.yaml")
 
     tp.add_system_message()
-    tp.add_user_message(name="Qui-gon", message="Hey!")
+    tp.add_user_message(user_name="Qui-gon", message="Hey!")
     tp.add_assistant_message(message="Hello Jonatas! How can I help you today?")
 
     text = tp.build()
     expected = [
         {"role": "system", "content": "You are a chatbot\n"},
         {"role": "user", "content": "Qui-gon: Hey!\n"},
-        {"role": "assistant", "content": "answer: Hello Jonatas! How can I help you today?\n"},
+        {
+            "role": "assistant",
+            "content": "answer: Hello Jonatas! How can I help you today?\n",
+        },
     ]
     assert text == expected
 
-    assert tp.title == "Turbo prompt"
-    assert tp.settings == {
-        "top-k": 1,
-        "temperature": 0.15,
-        "engine": "gpt-3.5-turbo",
-        "max_tokens": 32,
-    }
+    assert tp.name == "basic_turbo_prompt"
+    assert tp.description == "Basic turbo prompt example"
+    from prompts.schemas import OpenAIModelSettings
+
+    assert tp.settings == OpenAIModelSettings(
+        **{
+            "temperature": 0.15,
+            "engine": "gpt-3.5-turbo",
+            "max_tokens": 32,
+        }
+    )
 
 
-def test_from_file_with_past_messages():
+def test_from_file_with_initial_template_data():
     tp = TurboPrompt.from_file("samples/sample.past.yaml")
 
     # Check the content of the past messages
-    assert tp.prompts[0]["prompt"] == "You are an AI that fixes code issues:\nLanguage: python\n"
-    assert tp.prompts[1]["prompt"] == "Code to check:\n```\ndef sum_numbers(a, b):\n    return a * b\n\n```\n"
-    assert tp.prompts[2]["prompt"] == "Bug Description:\nThe function should return the sum of a and b, not their product.\n\n"
+    assert (
+        tp.prompts[0]["content"]
+        == "You are an AI that fixes code issues:\nLanguage: python\n"
+    )
+    assert (
+        tp.prompts[1]["content"]
+        == "Code to check:\n```\ndef sum_numbers(a, b):\n    return a * b\n\n```\n"
+    )
+    assert (
+        tp.prompts[2]["content"]
+        == "Bug Description:\nThe function should return the sum of a and b, not their product.\n\n"
+    )
 
     # Add a new user message with a different code
     source_code = "def multiply_numbers(a, b):\n    return a - b\n"
     tp.add_user_message(source_code=source_code)
 
     # Check the built prompts
     expected_messages = [
@@ -90,9 +120,46 @@
         "Bug Description:\nThe function should return the sum of a and b, not their product.\n\n",
         "Code to check:\n```\ndef multiply_numbers(a, b):\n    return a - b\n\n```\n",
     ]
     text = tp.build()
     assert [msg["content"] for msg in text] == expected_messages
 
     # Check the title and settings attributes
-    assert tp.title == "Turbo prompt with past messages"
-    assert tp.settings == {"engine": "gpt-3.5-turbo"}
+    assert tp.name == "turbo_prompt_with_examples"
+    assert (
+        tp.description
+        == "Example of turbo prompt with initial_template_data (few-shot)"
+    )
+    sets = tp.settings
+    assert sets is not None
+    assert sets.engine == "gpt-3.5-turbo"
+
+
+def test_a_from_settings():
+    tp = TurboPrompt.from_file("samples/complex.yaml")
+    built = tp.build()
+    assert isinstance(built, list)
+    assert isinstance(built[0], dict)
+    assert len(built) == 3
+    assert built[-1]["role"] == "assistant"
+
+    tp = TurboPrompt.from_settings(
+        name="turbo_prompt_inline",
+        description="",
+        system_template="You are an AI",
+        user_template="Q:<message>",
+        assistant_template="A:",
+        settings=OpenAIModelSettings(engine="gpt-4"),
+        initial_template_data=[
+            TemplateContent(
+                content="hey", template_name="default", role=PromptRole.SYSTEM
+            )
+        ],
+    )
+
+    content = tp.build()
+    assert len(content) == 1
+    print(content)
+    assert content[0] == {
+        "role": "system",
+        "content": "hey",
+    }
```

