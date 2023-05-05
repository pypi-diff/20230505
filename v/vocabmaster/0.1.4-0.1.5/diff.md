# Comparing `tmp/vocabmaster-0.1.4.tar.gz` & `tmp/vocabmaster-0.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vocabmaster-0.1.4.tar", last modified: Sun Apr 23 23:23:47 2023, max compression
+gzip compressed data, was "vocabmaster-0.1.5.tar", last modified: Fri May  5 18:15:22 2023, max compression
```

## Comparing `vocabmaster-0.1.4.tar` & `vocabmaster-0.1.5.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 sebastien  (1000) sebastien  (1000)        0 2023-04-23 23:23:47.240119 vocabmaster-0.1.4/
--rw-r--r--   0 sebastien  (1000) sebastien  (1000)     1079 2023-04-08 02:37:38.000000 vocabmaster-0.1.4/LICENSE
--rw-r--r--   0 sebastien  (1000) sebastien  (1000)     2594 2023-04-23 23:23:47.240119 vocabmaster-0.1.4/PKG-INFO
--rw-r--r--   0 sebastien  (1000) sebastien  (1000)     2461 2023-04-23 22:56:29.000000 vocabmaster-0.1.4/README.md
--rw-r--r--   0 sebastien  (1000) sebastien  (1000)       38 2023-04-23 23:23:47.240119 vocabmaster-0.1.4/setup.cfg
--rw-r--r--   0 sebastien  (1000) sebastien  (1000)      578 2023-04-23 23:22:55.000000 vocabmaster-0.1.4/setup.py
-drwxr-xr-x   0 sebastien  (1000) sebastien  (1000)        0 2023-04-23 23:23:47.240119 vocabmaster-0.1.4/vocabmaster/
--rw-r--r--   0 sebastien  (1000) sebastien  (1000)        0 2023-04-09 03:24:19.000000 vocabmaster-0.1.4/vocabmaster/__init__.py
--rw-r--r--   0 sebastien  (1000) sebastien  (1000)    18244 2023-04-23 23:21:09.000000 vocabmaster-0.1.4/vocabmaster/cli.py
--rw-r--r--   0 sebastien  (1000) sebastien  (1000)     4200 2023-04-16 12:02:38.000000 vocabmaster-0.1.4/vocabmaster/config_handler.py
--rw-r--r--   0 sebastien  (1000) sebastien  (1000)    10681 2023-04-16 12:02:38.000000 vocabmaster-0.1.4/vocabmaster/csv_handler.py
--rw-r--r--   0 sebastien  (1000) sebastien  (1000)     5606 2023-04-23 14:36:17.000000 vocabmaster-0.1.4/vocabmaster/gpt_integration.py
--rw-r--r--   0 sebastien  (1000) sebastien  (1000)     7282 2023-04-20 14:45:02.000000 vocabmaster-0.1.4/vocabmaster/utils.py
-drwxr-xr-x   0 sebastien  (1000) sebastien  (1000)        0 2023-04-23 23:23:47.240119 vocabmaster-0.1.4/vocabmaster.egg-info/
--rw-r--r--   0 sebastien  (1000) sebastien  (1000)     2594 2023-04-23 23:23:47.000000 vocabmaster-0.1.4/vocabmaster.egg-info/PKG-INFO
--rw-r--r--   0 sebastien  (1000) sebastien  (1000)      390 2023-04-23 23:23:47.000000 vocabmaster-0.1.4/vocabmaster.egg-info/SOURCES.txt
--rw-r--r--   0 sebastien  (1000) sebastien  (1000)        1 2023-04-23 23:23:47.000000 vocabmaster-0.1.4/vocabmaster.egg-info/dependency_links.txt
--rw-r--r--   0 sebastien  (1000) sebastien  (1000)       60 2023-04-23 23:23:47.000000 vocabmaster-0.1.4/vocabmaster.egg-info/entry_points.txt
--rw-r--r--   0 sebastien  (1000) sebastien  (1000)      277 2023-04-23 23:23:47.000000 vocabmaster-0.1.4/vocabmaster.egg-info/requires.txt
--rw-r--r--   0 sebastien  (1000) sebastien  (1000)       12 2023-04-23 23:23:47.000000 vocabmaster-0.1.4/vocabmaster.egg-info/top_level.txt
+drwxr-xr-x   0 sebastien  (1000) sebastien  (1000)        0 2023-05-05 18:15:22.743051 vocabmaster-0.1.5/
+-rw-r--r--   0 sebastien  (1000) sebastien  (1000)     1079 2023-04-08 02:37:38.000000 vocabmaster-0.1.5/LICENSE
+-rw-r--r--   0 sebastien  (1000) sebastien  (1000)     2698 2023-05-05 18:15:22.743051 vocabmaster-0.1.5/PKG-INFO
+-rw-r--r--   0 sebastien  (1000) sebastien  (1000)     2565 2023-05-04 11:47:01.000000 vocabmaster-0.1.5/README.md
+-rw-r--r--   0 sebastien  (1000) sebastien  (1000)       38 2023-05-05 18:15:22.743051 vocabmaster-0.1.5/setup.cfg
+-rw-r--r--   0 sebastien  (1000) sebastien  (1000)      578 2023-05-05 18:14:40.000000 vocabmaster-0.1.5/setup.py
+drwxr-xr-x   0 sebastien  (1000) sebastien  (1000)        0 2023-05-05 18:15:22.743051 vocabmaster-0.1.5/vocabmaster/
+-rw-r--r--   0 sebastien  (1000) sebastien  (1000)        0 2023-04-09 03:24:19.000000 vocabmaster-0.1.5/vocabmaster/__init__.py
+-rw-r--r--   0 sebastien  (1000) sebastien  (1000)    18006 2023-05-04 13:07:42.000000 vocabmaster-0.1.5/vocabmaster/cli.py
+-rw-r--r--   0 sebastien  (1000) sebastien  (1000)     4200 2023-04-16 12:02:38.000000 vocabmaster-0.1.5/vocabmaster/config_handler.py
+-rw-r--r--   0 sebastien  (1000) sebastien  (1000)    10722 2023-05-05 18:12:19.000000 vocabmaster-0.1.5/vocabmaster/csv_handler.py
+-rw-r--r--   0 sebastien  (1000) sebastien  (1000)     5646 2023-05-04 16:22:59.000000 vocabmaster-0.1.5/vocabmaster/gpt_integration.py
+-rw-r--r--   0 sebastien  (1000) sebastien  (1000)     7264 2023-05-04 13:33:03.000000 vocabmaster-0.1.5/vocabmaster/utils.py
+drwxr-xr-x   0 sebastien  (1000) sebastien  (1000)        0 2023-05-05 18:15:22.743051 vocabmaster-0.1.5/vocabmaster.egg-info/
+-rw-r--r--   0 sebastien  (1000) sebastien  (1000)     2698 2023-05-05 18:15:22.000000 vocabmaster-0.1.5/vocabmaster.egg-info/PKG-INFO
+-rw-r--r--   0 sebastien  (1000) sebastien  (1000)      390 2023-05-05 18:15:22.000000 vocabmaster-0.1.5/vocabmaster.egg-info/SOURCES.txt
+-rw-r--r--   0 sebastien  (1000) sebastien  (1000)        1 2023-05-05 18:15:22.000000 vocabmaster-0.1.5/vocabmaster.egg-info/dependency_links.txt
+-rw-r--r--   0 sebastien  (1000) sebastien  (1000)       60 2023-05-05 18:15:22.000000 vocabmaster-0.1.5/vocabmaster.egg-info/entry_points.txt
+-rw-r--r--   0 sebastien  (1000) sebastien  (1000)      277 2023-05-05 18:15:22.000000 vocabmaster-0.1.5/vocabmaster.egg-info/requires.txt
+-rw-r--r--   0 sebastien  (1000) sebastien  (1000)       12 2023-05-05 18:15:22.000000 vocabmaster-0.1.5/vocabmaster.egg-info/top_level.txt
```

### Comparing `vocabmaster-0.1.4/LICENSE` & `vocabmaster-0.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `vocabmaster-0.1.4/PKG-INFO` & `vocabmaster-0.1.5/README.md`

 * *Files 5% similar despite different names*

```diff
@@ -1,14 +1,7 @@
-Metadata-Version: 2.1
-Name: vocabmaster
-Version: 0.1.4
-Author: sderev
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # VocabMaster
 
 Master new languages with this user-friendly CLI tool, designed to help you record vocabulary, access translations and examples, and seamlessly import them into Anki for an optimized language learning experience.
 
 ## Features
 
 * Record vocabulary words with ease
@@ -29,25 +22,27 @@
 
 ```
 pip install vocabmaster
 ```
 
 ### Install via `pipx` (recommended)
 
-`pipx` is an alternative package manager for Python applications. It allows you to install and run Python applications in isolated environments, preventing conflicts between dependencies and ensuring that each application uses its own set of packages. We recommend using `pipx` to install VocabMaster.
+`pipx` is an alternative package manager for Python applications. It allows you to install and run Python applications in isolated environments, preventing conflicts between dependencies and ensuring that each application uses its own set of packages. I recommend using `pipx` to install VocabMaster.
 
 **First, install `pipx` if you haven't already:**
 
 * On macOS and Linux:
 
   ```
   python3 -m pip install --user pipx
   python3 -m pipx ensurepath
   ```
 
+Alternatively, you can use your package manager (`brew`, `apt`, etc.).
+
 * On Windows:
 
   ```
   py -m pip install --user pipx
   py -m pipx ensurepath
   ```
 
@@ -73,15 +68,20 @@
 source /path/to/vocabmaster/completion/_complete_vocabmaster.zsh
 ```
 
 Remember to replace `/path/to/vocabmaster` with the actual path where VocabMaster is installed.
 
 ## Usage
 
-Before using VocabMaster, you need to set up the OpenAI API key, which is required for the translations and usage examples. Follow the instructions provided within the CLI tool to configure the API key.
+Before using VocabMaster, you need to set up the OpenAI API key, which is required for the translations and usage examples. 
+Follow the instructions provided within the CLI tool to configure the API key:
+
+```
+vocabmaster config key
+```
 
 Below is an example of common commands and their usage:
 
 ### Set up a new language pair:
 
 ```
 vocabmaster setup
```

### Comparing `vocabmaster-0.1.4/README.md` & `vocabmaster-0.1.5/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,7 +1,14 @@
+Metadata-Version: 2.1
+Name: vocabmaster
+Version: 0.1.5
+Author: sderev
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # VocabMaster
 
 Master new languages with this user-friendly CLI tool, designed to help you record vocabulary, access translations and examples, and seamlessly import them into Anki for an optimized language learning experience.
 
 ## Features
 
 * Record vocabulary words with ease
@@ -22,25 +29,27 @@
 
 ```
 pip install vocabmaster
 ```
 
 ### Install via `pipx` (recommended)
 
-`pipx` is an alternative package manager for Python applications. It allows you to install and run Python applications in isolated environments, preventing conflicts between dependencies and ensuring that each application uses its own set of packages. We recommend using `pipx` to install VocabMaster.
+`pipx` is an alternative package manager for Python applications. It allows you to install and run Python applications in isolated environments, preventing conflicts between dependencies and ensuring that each application uses its own set of packages. I recommend using `pipx` to install VocabMaster.
 
 **First, install `pipx` if you haven't already:**
 
 * On macOS and Linux:
 
   ```
   python3 -m pip install --user pipx
   python3 -m pipx ensurepath
   ```
 
+Alternatively, you can use your package manager (`brew`, `apt`, etc.).
+
 * On Windows:
 
   ```
   py -m pip install --user pipx
   py -m pipx ensurepath
   ```
 
@@ -66,15 +75,20 @@
 source /path/to/vocabmaster/completion/_complete_vocabmaster.zsh
 ```
 
 Remember to replace `/path/to/vocabmaster` with the actual path where VocabMaster is installed.
 
 ## Usage
 
-Before using VocabMaster, you need to set up the OpenAI API key, which is required for the translations and usage examples. Follow the instructions provided within the CLI tool to configure the API key.
+Before using VocabMaster, you need to set up the OpenAI API key, which is required for the translations and usage examples. 
+Follow the instructions provided within the CLI tool to configure the API key:
+
+```
+vocabmaster config key
+```
 
 Below is an example of common commands and their usage:
 
 ### Set up a new language pair:
 
 ```
 vocabmaster setup
```

### Comparing `vocabmaster-0.1.4/setup.py` & `vocabmaster-0.1.5/setup.py`

 * *Files 17% similar despite different names*

```diff
@@ -5,15 +5,15 @@
     readme = file.read()
 
 with open("requirements.txt", "r", encoding="utf-8") as file:
     requirements = [line.strip() for line in file]
 
 setup(
     name="vocabmaster",
-    version="0.1.4",
+    version="0.1.5",
     packages=find_packages(),
     install_requires=requirements,
     entry_points={
         "console_scripts": [
             "vocabmaster = vocabmaster.cli:vocabmaster",
         ]
     },
```

### Comparing `vocabmaster-0.1.4/vocabmaster/cli.py` & `vocabmaster-0.1.5/vocabmaster/cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -125,17 +125,18 @@
 
     # Show untranslated words count if `--count` is used, then exit.
     if count:
         try:
             number_words = len(
                 csv_handler.get_words_to_translate(translations_filepath)
             )
-            click.echo(f"Number of words to translate: {BLUE}{number_words}{RESET}")
         except Exception as error:
             click.echo(f"{GREEN}Status:{RESET} {error}")
+        else:
+            click.echo(f"Number of words to translate: {BLUE}{number_words}{RESET}")
         return
 
     # Check for OpenAI API key
     if not openai_api_key_exists():
         openai_api_key_explain()
         return
 
@@ -192,15 +193,14 @@
     csv_handler.generate_anki_output_file(translations_filepath, anki_filepath)
     click.echo("The Anki deck has been generated 🤓✅")
     click.echo()
     click.echo(f"{GREEN}You can now import the deck into Anki{RESET} 📚")
 
     click.echo(f"{BOLD}The deck is located at:{RESET}")
     click.echo(f"{anki_filepath}")
-    click.echo()
 
 
 @vocabmaster.command()
 def anki():
     """
     Generate an Anki deck from your vocabulary list.
 
@@ -518,14 +518,15 @@
     default_language_to_learn = config_handler.get_default_language_pair()[
         "language_to_learn"
     ]
     default_mother_tongue = config_handler.get_default_language_pair()["mother_tongue"]
     click.echo(
         f"{BOLD}{ORANGE}{default_language_to_learn}:{default_mother_tongue}{RESET}"
     )
+    click.echo()
 
 
 def print_all_language_pairs():
     """
     Print all the language pairs that have been set up.
     """
     click.echo(f"{BLUE}The following language pairs have been set up:{RESET}")
@@ -533,16 +534,7 @@
     for idx, language_pair in enumerate(language_pairs, start=1):
         click.echo(
             f"{idx}."
             f" {language_pair['language_to_learn']}:{language_pair['mother_tongue']}"
         )
     click.echo()
 
-
-vocabmaster.add_command(config)
-vocabmaster.add_command(anki)
-vocabmaster.add_command(translate)
-vocabmaster.add_command(add)
-vocabmaster.add_command(anki)
-vocabmaster.add_command(default)
-vocabmaster.add_command(show)
-vocabmaster.add_command(tokens)
```

### Comparing `vocabmaster-0.1.4/vocabmaster/config_handler.py` & `vocabmaster-0.1.5/vocabmaster/config_handler.py`

 * *Files identical despite different names*

### Comparing `vocabmaster-0.1.4/vocabmaster/csv_handler.py` & `vocabmaster-0.1.5/vocabmaster/csv_handler.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,9 @@
 import csv
 from csv import DictReader, DictWriter
-import platform
 from pathlib import Path
 from vocabmaster import gpt_integration
 from vocabmaster import utils
 
 
 def word_exists(word, translations_filepath):
     """
@@ -207,24 +206,24 @@
     ) as anki_file:
         translations_dict_reader = DictReader(
             translations_file, fieldnames=["word", "translation", "example"]
         )
         next(translations_dict_reader)
 
         anki_dict_writer = DictWriter(
-            anki_file, fieldnames=["front", "back"], quoting=csv.QUOTE_MINIMAL
+            anki_file, fieldnames=["front", "back"], quoting=csv.QUOTE_MINIMAL, delimiter=";"
         )
 
         for translations in translations_dict_reader:
             if not translations["translation"] or not translations["example"]:
                 continue
             else:
                 translations["translation"] = translations["translation"].strip('"')
 
-                # Create a card with the word on the front and the translation and example on the back
+                # Create a card with the word on the front, and the translations and example on the back
                 card = {
                     "front": translations["word"],
                     "back": f"{translations['translation']}<br><br><details><summary>example</summary><i>&quot;{translations['example']}&quot;</i></details>",
                 }
 
                 # Write the card to the Anki output file
                 anki_dict_writer.writerow(card)
@@ -239,14 +238,16 @@
         fieldnames (list): A list of strings containing the column names.
     """
     with open(translations_filepath, "r+", encoding="UTF-8") as file:
         # Check if the fieldnames is already present in the first row of the content
         for line in file:
             if line.startswith(",".join(fieldnames)):
                 return
+            else:
+                break
 
         file.seek(0, 0)  # Move the file pointer to the beginning of the file
         content = file.read()
         file.seek(0, 0)
 
         writer = csv.writer(file)
         writer.writerow(fieldnames)  # Write the fieldnames to the first row
```

### Comparing `vocabmaster-0.1.4/vocabmaster/gpt_integration.py` & `vocabmaster-0.1.5/vocabmaster/gpt_integration.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 import os
+import json
 import openai
 import tiktoken
-import json
 import time
 from vocabmaster import csv_handler
 
 
 def format_prompt(language_to_learn, mother_tongue, words_to_translate):
     words_to_translate = "\n".join(words_to_translate)
     prompt = [
@@ -43,15 +43,15 @@
     model="gpt-3.5-turbo-0301",
     max_tokens=3600,
     n=1,
     temperature=0.5,
     stop=None,
     stream=False,
 ):
-    start_time = time.time()
+    start_time = time.monotonic_ns()
     openai.api_key = os.getenv("OPENAI_API_KEY")
 
     # Make the API request
     response = openai.ChatCompletion.create(
         messages=prompt,
         model=model,
         max_tokens=max_tokens,
@@ -72,23 +72,23 @@
             chunk_message = chunk["choices"][0]["delta"]  # extract the message
             collected_messages.append(chunk_message)  # save the message
             print(chunk_message.get("content", ""), end="")  # stream the message
         print()
         response = collected_chunks
 
         # Save the time delay and text received
-        response_time = time.time() - start_time
+        response_time = (time.monotonic_ns() - start_time) / 1e9
         generated_text = "".join([m.get("content", "") for m in collected_messages])
 
     else:
         # Extract and save the generated response
         generated_text = response["choices"][0]["message"]["content"]
 
         # Save the time delay
-        response_time = time.time() - start_time
+        response_time = (time.monotonic_ns() - start_time) / 1e9
 
     return (
         generated_text,
         response_time,
         response,
     )
```

### Comparing `vocabmaster-0.1.4/vocabmaster/utils.py` & `vocabmaster-0.1.5/vocabmaster/utils.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 import os
-import subprocess
 import platform
 import shutil
 from datetime import datetime
 from pathlib import Path
 from vocabmaster import config_handler
```

### Comparing `vocabmaster-0.1.4/vocabmaster.egg-info/PKG-INFO` & `vocabmaster-0.1.5/vocabmaster.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vocabmaster
-Version: 0.1.4
+Version: 0.1.5
 Author: sderev
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # VocabMaster
 
 Master new languages with this user-friendly CLI tool, designed to help you record vocabulary, access translations and examples, and seamlessly import them into Anki for an optimized language learning experience.
@@ -29,25 +29,27 @@
 
 ```
 pip install vocabmaster
 ```
 
 ### Install via `pipx` (recommended)
 
-`pipx` is an alternative package manager for Python applications. It allows you to install and run Python applications in isolated environments, preventing conflicts between dependencies and ensuring that each application uses its own set of packages. We recommend using `pipx` to install VocabMaster.
+`pipx` is an alternative package manager for Python applications. It allows you to install and run Python applications in isolated environments, preventing conflicts between dependencies and ensuring that each application uses its own set of packages. I recommend using `pipx` to install VocabMaster.
 
 **First, install `pipx` if you haven't already:**
 
 * On macOS and Linux:
 
   ```
   python3 -m pip install --user pipx
   python3 -m pipx ensurepath
   ```
 
+Alternatively, you can use your package manager (`brew`, `apt`, etc.).
+
 * On Windows:
 
   ```
   py -m pip install --user pipx
   py -m pipx ensurepath
   ```
 
@@ -73,15 +75,20 @@
 source /path/to/vocabmaster/completion/_complete_vocabmaster.zsh
 ```
 
 Remember to replace `/path/to/vocabmaster` with the actual path where VocabMaster is installed.
 
 ## Usage
 
-Before using VocabMaster, you need to set up the OpenAI API key, which is required for the translations and usage examples. Follow the instructions provided within the CLI tool to configure the API key.
+Before using VocabMaster, you need to set up the OpenAI API key, which is required for the translations and usage examples. 
+Follow the instructions provided within the CLI tool to configure the API key:
+
+```
+vocabmaster config key
+```
 
 Below is an example of common commands and their usage:
 
 ### Set up a new language pair:
 
 ```
 vocabmaster setup
```

