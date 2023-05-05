# Comparing `tmp/practice_turkish-1.4.0.tar.gz` & `tmp/practice_turkish-1.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "practice_turkish-1.4.0.tar", max compression
+gzip compressed data, was "practice_turkish-1.4.1.tar", max compression
```

## Comparing `practice_turkish-1.4.0.tar` & `practice_turkish-1.4.1.tar`

### file list

```diff
@@ -1,23 +1,24 @@
--rw-r--r--   0        0        0     1067 2023-04-08 13:06:59.919174 practice_turkish-1.4.0/LICENSE
--rw-r--r--   0        0        0     4471 2023-04-08 13:06:59.919174 practice_turkish-1.4.0/README.md
--rw-r--r--   0        0        0        0 2023-04-08 13:06:59.919174 practice_turkish-1.4.0/practice_turkish/__init__.py
--rw-r--r--   0        0        0      279 2023-04-08 13:06:59.919174 practice_turkish-1.4.0/practice_turkish/dictionaries/__init__.py
--rw-r--r--   0        0        0     4624 2023-04-08 13:06:59.919174 practice_turkish-1.4.0/practice_turkish/dictionaries/csvdictionary.py
--rw-r--r--   0        0        0     8154 2023-04-08 13:06:59.919174 practice_turkish-1.4.0/practice_turkish/dictionaries/dictionary.py
--rw-r--r--   0        0        0      536 2023-04-08 13:06:59.919174 practice_turkish-1.4.0/practice_turkish/dictionaries/parse.py
--rw-r--r--   0        0        0     3990 2023-04-08 13:06:59.923174 practice_turkish-1.4.0/practice_turkish/dictionaries/telegram.py
--rw-r--r--   0        0        0     3049 2023-04-08 13:06:59.923174 practice_turkish-1.4.0/practice_turkish/dictionaries/turkrutdictionary.py
--rw-r--r--   0        0        0     3191 2023-04-08 13:06:59.923174 practice_turkish-1.4.0/practice_turkish/filepath.py
--rw-r--r--   0        0        0      146 2023-04-08 13:06:59.923174 practice_turkish-1.4.0/practice_turkish/languages/__init__.py
--rw-r--r--   0        0        0     1649 2023-04-08 13:06:59.923174 practice_turkish-1.4.0/practice_turkish/languages/clipboard.py
--rw-r--r--   0        0        0     1066 2023-04-08 13:06:59.923174 practice_turkish-1.4.0/practice_turkish/languages/englishinput.py
--rw-r--r--   0        0        0     2975 2023-04-08 13:06:59.923174 practice_turkish-1.4.0/practice_turkish/languages/languages.py
--rw-r--r--   0        0        0     1200 2023-04-08 13:06:59.923174 practice_turkish-1.4.0/practice_turkish/languages/russianinput.py
--rw-r--r--   0        0        0     2922 2023-04-08 13:06:59.923174 practice_turkish-1.4.0/practice_turkish/languages/turkishinput.py
--rw-r--r--   0        0        0     1345 2023-04-08 13:06:59.923174 practice_turkish-1.4.0/practice_turkish/languages/validator.py
--rw-r--r--   0        0        0     8791 2023-04-08 13:06:59.923174 practice_turkish-1.4.0/practice_turkish/make_csv.py
--rw-r--r--   0        0        0     5281 2023-04-08 13:06:59.923174 practice_turkish-1.4.0/practice_turkish/number.py
--rw-r--r--   0        0        0      486 2023-04-08 13:06:59.923174 practice_turkish-1.4.0/practice_turkish/practice.py
--rw-r--r--   0        0        0     7494 2023-04-08 13:06:59.923174 practice_turkish-1.4.0/practice_turkish/translation.py
--rw-r--r--   0        0        0     1043 2023-04-08 13:06:59.923174 practice_turkish-1.4.0/pyproject.toml
--rw-r--r--   0        0        0     5258 1970-01-01 00:00:00.000000 practice_turkish-1.4.0/PKG-INFO
+-rw-r--r--   0        0        0     1067 2023-05-05 16:37:05.685858 practice_turkish-1.4.1/LICENSE
+-rw-r--r--   0        0        0     4471 2023-05-05 16:37:05.685858 practice_turkish-1.4.1/README.md
+-rw-r--r--   0        0        0        0 2023-05-05 16:37:05.685858 practice_turkish-1.4.1/practice_turkish/__init__.py
+-rw-r--r--   0        0        0      279 2023-05-05 16:37:05.685858 practice_turkish-1.4.1/practice_turkish/dictionaries/__init__.py
+-rw-r--r--   0        0        0     4624 2023-05-05 16:37:05.685858 practice_turkish-1.4.1/practice_turkish/dictionaries/csvdictionary.py
+-rw-r--r--   0        0        0     8154 2023-05-05 16:37:05.685858 practice_turkish-1.4.1/practice_turkish/dictionaries/dictionary.py
+-rw-r--r--   0        0        0      536 2023-05-05 16:37:05.689858 practice_turkish-1.4.1/practice_turkish/dictionaries/parse.py
+-rw-r--r--   0        0        0     3990 2023-05-05 16:37:05.689858 practice_turkish-1.4.1/practice_turkish/dictionaries/telegram.py
+-rw-r--r--   0        0        0     3049 2023-05-05 16:37:05.689858 practice_turkish-1.4.1/practice_turkish/dictionaries/turkrutdictionary.py
+-rw-r--r--   0        0        0     3934 2023-05-05 16:37:05.689858 practice_turkish-1.4.1/practice_turkish/filepath.py
+-rw-r--r--   0        0        0      146 2023-05-05 16:37:05.689858 practice_turkish-1.4.1/practice_turkish/languages/__init__.py
+-rw-r--r--   0        0        0     1649 2023-05-05 16:37:05.689858 practice_turkish-1.4.1/practice_turkish/languages/clipboard.py
+-rw-r--r--   0        0        0     1066 2023-05-05 16:37:05.689858 practice_turkish-1.4.1/practice_turkish/languages/englishinput.py
+-rw-r--r--   0        0        0     2975 2023-05-05 16:37:05.689858 practice_turkish-1.4.1/practice_turkish/languages/languages.py
+-rw-r--r--   0        0        0     1200 2023-05-05 16:37:05.689858 practice_turkish-1.4.1/practice_turkish/languages/russianinput.py
+-rw-r--r--   0        0        0     2922 2023-05-05 16:37:05.689858 practice_turkish-1.4.1/practice_turkish/languages/turkishinput.py
+-rw-r--r--   0        0        0     1345 2023-05-05 16:37:05.689858 practice_turkish-1.4.1/practice_turkish/languages/validator.py
+-rw-r--r--   0        0        0     8791 2023-05-05 16:37:05.689858 practice_turkish-1.4.1/practice_turkish/make_csv.py
+-rw-r--r--   0        0        0     5281 2023-05-05 16:37:05.689858 practice_turkish-1.4.1/practice_turkish/number.py
+-rw-r--r--   0        0        0      486 2023-05-05 16:37:05.689858 practice_turkish-1.4.1/practice_turkish/practice.py
+-rw-r--r--   0        0        0      871 2023-05-05 16:37:05.689858 practice_turkish-1.4.1/practice_turkish/to_telegram.py
+-rw-r--r--   0        0        0     6938 2023-05-05 16:37:05.689858 practice_turkish-1.4.1/practice_turkish/translation.py
+-rw-r--r--   0        0        0     1094 2023-05-05 16:37:05.689858 practice_turkish-1.4.1/pyproject.toml
+-rw-r--r--   0        0        0     5258 1970-01-01 00:00:00.000000 practice_turkish-1.4.1/PKG-INFO
```

### Comparing `practice_turkish-1.4.0/LICENSE` & `practice_turkish-1.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `practice_turkish-1.4.0/README.md` & `practice_turkish-1.4.1/README.md`

 * *Files identical despite different names*

### Comparing `practice_turkish-1.4.0/practice_turkish/dictionaries/csvdictionary.py` & `practice_turkish-1.4.1/practice_turkish/dictionaries/csvdictionary.py`

 * *Files identical despite different names*

### Comparing `practice_turkish-1.4.0/practice_turkish/dictionaries/dictionary.py` & `practice_turkish-1.4.1/practice_turkish/dictionaries/dictionary.py`

 * *Files identical despite different names*

### Comparing `practice_turkish-1.4.0/practice_turkish/dictionaries/parse.py` & `practice_turkish-1.4.1/practice_turkish/dictionaries/parse.py`

 * *Files identical despite different names*

### Comparing `practice_turkish-1.4.0/practice_turkish/dictionaries/telegram.py` & `practice_turkish-1.4.1/practice_turkish/dictionaries/telegram.py`

 * *Files 1% similar despite different names*

```diff
@@ -102,15 +102,15 @@
     ----------
     AuthenticationError
         If the pair (`user_id`, `token`) is rejected by the bot.
     """
     response = requests.post(
         url=url,
         data=json.dumps({"user id": user_id, "token": token, "text": text}),
-        timeout=10,
+        timeout=30,
     )
     if response.status_code == 403:
         raise AuthenticationError(
             """User token is rejected!
             Please, check 'USER ID' and 'TOKEN' fields in your configuration file."""
         )
     if response.status_code != 200:
```

### Comparing `practice_turkish-1.4.0/practice_turkish/dictionaries/turkrutdictionary.py` & `practice_turkish-1.4.1/practice_turkish/dictionaries/turkrutdictionary.py`

 * *Files identical despite different names*

### Comparing `practice_turkish-1.4.0/practice_turkish/filepath.py` & `practice_turkish-1.4.1/practice_turkish/filepath.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,16 +1,23 @@
 import os
 from pathlib import Path
-from typing import Generator, Optional
+from typing import Generator, Optional, Type
 
 from prompt_toolkit.document import Document
 from prompt_toolkit.completion import Completion, CompleteEvent
 from InquirerPy import inquirer
 from InquirerPy.prompts.filepath import FilePathCompleter
 from InquirerPy.validator import PathValidator
+from InquirerPy.base.control import Choice
+
+from practice_turkish.dictionaries import (
+    DictionaryEntry,
+    CSVDictionaryEntry,
+    TurkrutDictionaryEntry,
+)
 
 
 class ExtensionFilePathCompleter(FilePathCompleter):
     """A class used to generate completions for path of a file with an extension.
 
     Extends `FilePathCompleter` provided by `InquirerPy` library. Overloads the
     `get_completions` method to generate completions only for files with
@@ -86,9 +93,28 @@
         message=message,
         default=str(path.absolute()) + os.path.sep,
         completer=completer,
         validate=validator,
     ).execute()
 
 
+def prompt_dictionary_type() -> Type[DictionaryEntry]:
+    """Prompt a type of a dictionary from the user.
+
+    Request the user to pick a type of a supported dictionary.
+    This type later is used in order to parse the content of the file.
+
+    Returns
+    ----------
+    T : A subclass of DictionaryItem class
+    """
+    return inquirer.select(
+        message="What is the format of the file?",
+        choices=[
+            Choice(value=TurkrutDictionaryEntry, name="turkrut.ru"),
+            Choice(value=CSVDictionaryEntry, name="csv"),
+        ],
+    ).execute()
+
+
 if __name__ == "__main__":
     print(prompt_filepath("> ", extension=".txt", is_file=True))
```

### Comparing `practice_turkish-1.4.0/practice_turkish/languages/clipboard.py` & `practice_turkish-1.4.1/practice_turkish/languages/clipboard.py`

 * *Files identical despite different names*

### Comparing `practice_turkish-1.4.0/practice_turkish/languages/englishinput.py` & `practice_turkish-1.4.1/practice_turkish/languages/englishinput.py`

 * *Files identical despite different names*

### Comparing `practice_turkish-1.4.0/practice_turkish/languages/languages.py` & `practice_turkish-1.4.1/practice_turkish/languages/languages.py`

 * *Files identical despite different names*

### Comparing `practice_turkish-1.4.0/practice_turkish/languages/russianinput.py` & `practice_turkish-1.4.1/practice_turkish/languages/russianinput.py`

 * *Files identical despite different names*

### Comparing `practice_turkish-1.4.0/practice_turkish/languages/turkishinput.py` & `practice_turkish-1.4.1/practice_turkish/languages/turkishinput.py`

 * *Files identical despite different names*

### Comparing `practice_turkish-1.4.0/practice_turkish/languages/validator.py` & `practice_turkish-1.4.1/practice_turkish/languages/validator.py`

 * *Files identical despite different names*

### Comparing `practice_turkish-1.4.0/practice_turkish/make_csv.py` & `practice_turkish-1.4.1/practice_turkish/make_csv.py`

 * *Files identical despite different names*

### Comparing `practice_turkish-1.4.0/practice_turkish/number.py` & `practice_turkish-1.4.1/practice_turkish/number.py`

 * *Files identical despite different names*

### Comparing `practice_turkish-1.4.0/practice_turkish/translation.py` & `practice_turkish-1.4.1/practice_turkish/translation.py`

 * *Files 8% similar despite different names*

```diff
@@ -5,20 +5,18 @@
 
 from rich import print
 import typer
 from InquirerPy import inquirer
 from InquirerPy.base.control import Choice
 
 from practice_turkish.languages import prompt_way_of_translation
-from practice_turkish.filepath import prompt_filepath
+from practice_turkish.filepath import prompt_filepath, prompt_dictionary_type
 from practice_turkish.dictionaries import (
     Dictionary,
     DictionaryEntry,
-    CSVDictionaryEntry,
-    TurkrutDictionaryEntry,
 )
 
 
 class AnswerType(str, Enum):
     """An enum used to represent form of the answers by an user.
 
     Values
@@ -29,33 +27,14 @@
         User picks an answer from a list of options.
     """
 
     TYPING = "TYPING"
     CHOICE = "CHOICE"
 
 
-def prompt_dictionary_type() -> Type[DictionaryEntry]:
-    """Prompt a type of a dictionary from the user.
-
-    Request the user to pick a type of a supported dictionary.
-    This type later is used in order to parse the content of the file.
-
-    Returns
-    ----------
-    T : A subclass of DictionaryItem class
-    """
-    return inquirer.select(
-        message="What is the format of the file?",
-        choices=[
-            Choice(value=TurkrutDictionaryEntry, name="turkrut.ru"),
-            Choice(value=CSVDictionaryEntry, name="csv"),
-        ],
-    ).execute()
-
-
 def prompt_shuffle() -> bool:
     """Prompt the user whether to shuffle the dictionary or not.
 
     Returns
     ----------
     x : bool
         True if user chooses to shuffle, False otherwise.
@@ -71,15 +50,16 @@
 
 def prompt_answer_type() -> AnswerType:
     "Prompt the user to pick the form of their answers."
     return inquirer.select(
         message="How would you prefer to answer?",
         choices=[
             Choice(value=AnswerType.TYPING, name="Type it in"),
-            Choice(value=AnswerType.CHOICE, name="Choose from multiple options"),
+            Choice(value=AnswerType.CHOICE,
+                   name="Choose from multiple options"),
         ],
     ).execute()
 
 
 def answer_with_prompt(entry: DictionaryEntry, a2b: bool) -> bool:
     """Prompt an answer from the user by typing it in, and check its correctness.
 
@@ -136,30 +116,32 @@
     Returns
     ----------
     is_correct : bool
         True if translation is correct, False otherwise.
     """
     query = the_entry.query_a if a2b else the_entry.query_b
     incorrect_options = random.sample(dictionary.entries, k=n_choices)
-    incorrect_options = [entry for entry in incorrect_options if entry is not the_entry]
+    incorrect_options = [
+        entry for entry in incorrect_options if entry is not the_entry]
     options = [the_entry] + incorrect_options[: n_choices - 1]
     random.shuffle(options)
     choices = [
         Choice(value=i, name=o.query_b if a2b else o.query_a)
         for i, o in enumerate(options)
     ]
 
     i = inquirer.select(message=f"{query} ⇨ ", choices=choices).execute()
 
     choice = options[i]
     if choice is the_entry:
         print("[green]Correct![/green]")
         return True
     correct_answer = the_entry.query_b if a2b else the_entry.query_a
-    print(f"[red]Incorrect![/red] Correct option was '[green]{correct_answer}[/green]'")
+    print(
+        f"[red]Incorrect![/red] Correct option was '[green]{correct_answer}[/green]'")
     return False
 
 
 def prepare_session() -> (
     tuple[Dictionary[DictionaryEntry], Callable[[DictionaryEntry], bool]]
 ):
     """Prepare translation session.
@@ -183,15 +165,16 @@
         extension=dictionary_entry_type.extension(),
         directory=dictionary_entry_type.default_directory(),
     )
     dictionary = Dictionary.from_file(path, dictionary_entry_type)
     if prompt_shuffle():
         dictionary.shuffle()
 
-    a2b = prompt_way_of_translation(dictionary.language_a, dictionary.language_b)
+    a2b = prompt_way_of_translation(
+        dictionary.language_a, dictionary.language_b)
     match prompt_answer_type():
         case AnswerType.TYPING:
             answer_function = partial(answer_with_prompt, a2b=a2b)
         case AnswerType.CHOICE:
             answer_function = partial(
                 answer_with_choice, a2b=a2b, dictionary=dictionary
             )
```

### Comparing `practice_turkish-1.4.0/pyproject.toml` & `practice_turkish-1.4.1/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "practice_turkish"
-version = "1.4.0"
+version = "1.4.1"
 description = "A set of tools to practice your Turkish"
 authors = ["Egor Fadeev <fadeevegor@yandex.ru>"]
 readme = "README.md"
 packages = [{include = "practice_turkish"}]
 license = "MIT"
 repository = "https://github.com/FadeevEgor/PracticeTurkish"
 
@@ -17,14 +17,16 @@
 prompt-toolkit = "^3.0.38"
 
 [tool.poetry.scripts]
 practice_turkish = "practice_turkish.practice:main"
 translate = "practice_turkish.translation:main"
 numbers = "practice_turkish.number:main"
 new_dictionary = "practice_turkish.make_csv:main"
+to_telegram = "practice_turkish.to_telegram:main"
+
 
 [tool.pylint.message_control]
 disable = [
     "duplicate-code",
     "cyclic-import",
     "invalid-name",
     "missing-module-docstring",
```

### Comparing `practice_turkish-1.4.0/PKG-INFO` & `practice_turkish-1.4.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: practice-turkish
-Version: 1.4.0
+Version: 1.4.1
 Summary: A set of tools to practice your Turkish
 Home-page: https://github.com/FadeevEgor/PracticeTurkish
 License: MIT
 Author: Egor Fadeev
 Author-email: fadeevegor@yandex.ru
 Requires-Python: >=3.10,<4.0
 Classifier: License :: OSI Approved :: MIT License
```

