# Comparing `tmp/ai_ghostfunctions-0.3.1.tar.gz` & `tmp/ai_ghostfunctions-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ai_ghostfunctions-0.3.1.tar", max compression
+gzip compressed data, was "ai_ghostfunctions-0.4.0.tar", max compression
```

## Comparing `ai_ghostfunctions-0.3.1.tar` & `ai_ghostfunctions-0.4.0.tar`

### file list

```diff
@@ -1,9 +1,9 @@
--rw-r--r--   0        0        0     1069 2023-04-19 20:58:17.657236 ai_ghostfunctions-0.3.1/LICENSE
--rw-r--r--   0        0        0     4451 2023-04-19 20:58:17.657236 ai_ghostfunctions-0.3.1/README.md
--rw-r--r--   0        0        0     1828 2023-04-19 20:58:31.241477 ai_ghostfunctions-0.3.1/pyproject.toml
--rw-r--r--   0        0        0      162 2023-04-19 20:58:17.661236 ai_ghostfunctions-0.3.1/src/ai_ghostfunctions/__init__.py
--rw-r--r--   0        0        0     6266 2023-04-19 20:58:17.661236 ai_ghostfunctions-0.3.1/src/ai_ghostfunctions/ghostfunctions.py
--rw-r--r--   0        0        0      231 2023-04-19 20:58:17.661236 ai_ghostfunctions-0.3.1/src/ai_ghostfunctions/keywords.py
--rw-r--r--   0        0        0        0 2023-04-19 20:58:17.661236 ai_ghostfunctions-0.3.1/src/ai_ghostfunctions/py.typed
--rw-r--r--   0        0        0      343 2023-04-19 20:58:17.661236 ai_ghostfunctions-0.3.1/src/ai_ghostfunctions/types.py
--rw-r--r--   0        0        0     5377 1970-01-01 00:00:00.000000 ai_ghostfunctions-0.3.1/PKG-INFO
+-rw-r--r--   0        0        0     1069 2023-05-04 22:43:14.564348 ai_ghostfunctions-0.4.0/LICENSE
+-rw-r--r--   0        0        0     4451 2023-05-04 22:43:14.568348 ai_ghostfunctions-0.4.0/README.md
+-rw-r--r--   0        0        0     1828 2023-05-04 22:43:30.620375 ai_ghostfunctions-0.4.0/pyproject.toml
+-rw-r--r--   0        0        0      162 2023-05-04 22:43:14.568348 ai_ghostfunctions-0.4.0/src/ai_ghostfunctions/__init__.py
+-rw-r--r--   0        0        0     6689 2023-05-04 22:43:14.568348 ai_ghostfunctions-0.4.0/src/ai_ghostfunctions/ghostfunctions.py
+-rw-r--r--   0        0        0      231 2023-05-04 22:43:14.568348 ai_ghostfunctions-0.4.0/src/ai_ghostfunctions/keywords.py
+-rw-r--r--   0        0        0        0 2023-05-04 22:43:14.568348 ai_ghostfunctions-0.4.0/src/ai_ghostfunctions/py.typed
+-rw-r--r--   0        0        0      343 2023-05-04 22:43:14.568348 ai_ghostfunctions-0.4.0/src/ai_ghostfunctions/types.py
+-rw-r--r--   0        0        0     5377 1970-01-01 00:00:00.000000 ai_ghostfunctions-0.4.0/PKG-INFO
```

### Comparing `ai_ghostfunctions-0.3.1/LICENSE` & `ai_ghostfunctions-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `ai_ghostfunctions-0.3.1/README.md` & `ai_ghostfunctions-0.4.0/README.md`

 * *Files identical despite different names*

### Comparing `ai_ghostfunctions-0.3.1/pyproject.toml` & `ai_ghostfunctions-0.4.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "ai-ghostfunctions"
-version = "0.3.1"
+version = "0.4.0"
 description = "AI Ghostfunctions"
 authors = ["Brian M. Ritz <brianmritz@gmail.com>"]
 license = "MIT"
 readme = "README.md"
 homepage = "https://github.com/bmritz/ai-ghostfunctions"
 repository = "https://github.com/bmritz/ai-ghostfunctions"
 documentation = "https://ai-ghostfunctions.readthedocs.io"
```

### Comparing `ai_ghostfunctions-0.3.1/src/ai_ghostfunctions/ghostfunctions.py` & `ai_ghostfunctions-0.4.0/src/ai_ghostfunctions/ghostfunctions.py`

 * *Files 3% similar despite different names*

```diff
@@ -15,17 +15,21 @@
 from .keywords import ASSISTANT
 from .keywords import SYSTEM
 from .keywords import USER
 from .types import Message
 
 
 def _make_chatgpt_message_from_function(
-    f: Callable[..., Any], **kwargs: Any
+    f: Callable[..., Any], *args: Any, **kwargs: Any
 ) -> Message:
     sig = inspect.signature(f)
+    if args:
+        params = list(sig.parameters)
+        for i, arg in enumerate(args):
+            kwargs[params[i]] = arg
     if not f.__doc__:
         raise ValueError("The function must have a docstring.")
     prompt = (
         (
             f"from mymodule import {f.__name__}\n"
             f"""
 # The return type annotation for the function {f.__name__} is {get_type_hints(f)['return']}
@@ -37,15 +41,17 @@
 result = {f.__name__}({",".join(f"{k}={kwargs[k].__repr__()}" for k in sig.parameters)})
 print(result)
 """
     )
     return Message(role=USER, content=prompt)
 
 
-def _default_prompt_creation(f: Callable[..., Any], **kwargs: Any) -> List[Message]:
+def _default_prompt_creation(
+    f: Callable[..., Any], *args: Any, **kwargs: Any
+) -> List[Message]:
     return [
         Message(
             role=SYSTEM,
             content=(
                 "You are role playing as an advanced python interpreter that never errors,"
                 " and always returns the intent of the programmer. Every user message is"
                 " valid python, and your job is to return only what python would return in"
@@ -60,15 +66,15 @@
         Message(
             role=ASSISTANT,
             content=(
                 "Hello! I am a Python interpreter. Please enter your Python code below and"
                 " I will return the output, and nothing else."
             ),
         ),
-        _make_chatgpt_message_from_function(f, **kwargs),
+        _make_chatgpt_message_from_function(f, *args, **kwargs),
     ]
 
 
 def _default_ai_callable() -> Callable[..., openai.openai_object.OpenAIObject]:
     import openai
 
     openai.api_key = os.environ["OPENAI_API_KEY"]
@@ -105,15 +111,20 @@
 
     Returns:
         The data from the ai result (data is of type `expected_return_type`)
 
     """
     to_return: str = ai_result["choices"][0]["message"]["content"]
     if expected_return_type is str:
+        if to_return.startswith("'") and to_return.endswith("'"):
+            return ast.literal_eval(to_return)
+        elif to_return.startswith('"') and to_return.endswith('"'):
+            return ast.literal_eval(to_return)
         return to_return
+
     data = ast.literal_eval(to_return)
     return typeguard.check_type(data, expected_return_type)
 
 
 def ghostfunction(
     function: Optional[Callable[..., Any]] = None,
     /,
@@ -139,16 +150,16 @@
         ai_callable = _default_ai_callable()
 
     if function is not None:
         _assert_function_has_return_type_annotation(function)
         return_type_annotation = get_type_hints(function)["return"]
 
         @wraps(function)
-        def wrapper(**kwargs_inner: Any) -> Any:
-            prompt = prompt_function(function, **kwargs_inner)  # type: ignore[arg-type]
+        def wrapper(*args_inner: Any, **kwargs_inner: Any) -> Any:
+            prompt = prompt_function(function, *args_inner, **kwargs_inner)  # type: ignore[arg-type]
             ai_result = ai_callable(messages=prompt, **kwargs)  # type: ignore[misc]
             return _parse_ai_result(
                 ai_result=ai_result, expected_return_type=return_type_annotation
             )
 
         return wrapper
```

### Comparing `ai_ghostfunctions-0.3.1/PKG-INFO` & `ai_ghostfunctions-0.4.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ai-ghostfunctions
-Version: 0.3.1
+Version: 0.4.0
 Summary: AI Ghostfunctions
 Home-page: https://github.com/bmritz/ai-ghostfunctions
 License: MIT
 Author: Brian M. Ritz
 Author-email: brianmritz@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: Development Status :: 3 - Alpha
```

