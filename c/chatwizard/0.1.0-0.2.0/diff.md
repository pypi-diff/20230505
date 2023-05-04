# Comparing `tmp/chatwizard-0.1.0.tar.gz` & `tmp/chatwizard-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "chatwizard-0.1.0.tar", last modified: Mon Mar 27 00:33:49 2023, max compression
+gzip compressed data, was "chatwizard-0.2.0.tar", last modified: Thu May  4 22:57:44 2023, max compression
```

## Comparing `chatwizard-0.1.0.tar` & `chatwizard-0.2.0.tar`

### file list

```diff
@@ -1,39 +1,44 @@
-drwxr-xr-x   0 ulasonat   (501) staff       (20)        0 2023-03-27 00:33:49.379929 chatwizard-0.1.0/
--rw-r--r--   0 ulasonat   (501) staff       (20)      296 2023-03-26 21:33:01.000000 chatwizard-0.1.0/.bumpversion.cfg
--rw-r--r--   0 ulasonat   (501) staff       (20)     2193 2023-03-26 23:59:07.000000 chatwizard-0.1.0/CONTRIBUTING.md
--rw-r--r--   0 ulasonat   (501) staff       (20)     1074 2023-03-26 21:33:01.000000 chatwizard-0.1.0/LICENSE
--rw-r--r--   0 ulasonat   (501) staff       (20)      602 2023-03-26 23:59:07.000000 chatwizard-0.1.0/MANIFEST.in
--rw-r--r--   0 ulasonat   (501) staff       (20)     2287 2023-03-26 21:33:01.000000 chatwizard-0.1.0/Makefile
--rw-r--r--   0 ulasonat   (501) staff       (20)      423 2023-03-27 00:33:49.379819 chatwizard-0.1.0/PKG-INFO
--rw-r--r--   0 ulasonat   (501) staff       (20)     2919 2023-03-26 23:59:07.000000 chatwizard-0.1.0/README.md
-drwxr-xr-x   0 ulasonat   (501) staff       (20)        0 2023-03-27 00:33:49.377658 chatwizard-0.1.0/chatwizard.egg-info/
--rw-r--r--   0 ulasonat   (501) staff       (20)      423 2023-03-27 00:33:49.000000 chatwizard-0.1.0/chatwizard.egg-info/PKG-INFO
--rw-r--r--   0 ulasonat   (501) staff       (20)      686 2023-03-27 00:33:49.000000 chatwizard-0.1.0/chatwizard.egg-info/SOURCES.txt
--rw-r--r--   0 ulasonat   (501) staff       (20)        1 2023-03-27 00:33:49.000000 chatwizard-0.1.0/chatwizard.egg-info/dependency_links.txt
--rw-r--r--   0 ulasonat   (501) staff       (20)       15 2023-03-27 00:33:49.000000 chatwizard-0.1.0/chatwizard.egg-info/requires.txt
--rw-r--r--   0 ulasonat   (501) staff       (20)        1 2023-03-27 00:33:49.000000 chatwizard-0.1.0/chatwizard.egg-info/top_level.txt
--rw-r--r--   0 ulasonat   (501) staff       (20)     2262 2023-03-27 00:29:11.000000 chatwizard-0.1.0/pyproject.toml
-drwxr-xr-x   0 ulasonat   (501) staff       (20)        0 2023-03-27 00:33:49.378448 chatwizard-0.1.0/scripts/
-drwxr-xr-x   0 ulasonat   (501) staff       (20)        0 2023-03-27 00:33:49.378573 chatwizard-0.1.0/scripts/.idea/
--rw-r--r--   0 ulasonat   (501) staff       (20)     4297 2023-03-26 21:33:01.000000 chatwizard-0.1.0/scripts/.idea/workspace.xml
--rw-r--r--   0 ulasonat   (501) staff       (20)       22 2023-03-26 23:59:07.000000 chatwizard-0.1.0/scripts/_version.py
--rw-r--r--   0 ulasonat   (501) staff       (20)     6939 2023-03-26 23:59:07.000000 chatwizard-0.1.0/scripts/discord_bot.py
--rw-r--r--   0 ulasonat   (501) staff       (20)     2887 2023-03-26 23:59:07.000000 chatwizard-0.1.0/scripts/integration_tests.py
-drwxr-xr-x   0 ulasonat   (501) staff       (20)        0 2023-03-27 00:33:49.378713 chatwizard-0.1.0/scripts/json/
--rw-r--r--   0 ulasonat   (501) staff       (20)      142 2023-03-26 23:59:07.000000 chatwizard-0.1.0/scripts/json/user_scores.json
-drwxr-xr-x   0 ulasonat   (501) staff       (20)        0 2023-03-27 00:33:49.378848 chatwizard-0.1.0/scripts/log/
--rw-r--r--   0 ulasonat   (501) staff       (20)     2567 2023-03-26 23:59:07.000000 chatwizard-0.1.0/scripts/log/log.txt
--rw-r--r--   0 ulasonat   (501) staff       (20)     1343 2023-03-26 23:59:07.000000 chatwizard-0.1.0/scripts/main.py
--rw-r--r--   0 ulasonat   (501) staff       (20)     4598 2023-03-26 23:59:07.000000 chatwizard-0.1.0/scripts/openai_handler.py
-drwxr-xr-x   0 ulasonat   (501) staff       (20)        0 2023-03-27 00:33:49.379252 chatwizard-0.1.0/scripts/prompts/
--rw-r--r--   0 ulasonat   (501) staff       (20)      895 2023-03-26 23:59:07.000000 chatwizard-0.1.0/scripts/prompts/friendliness.txt
--rw-r--r--   0 ulasonat   (501) staff       (20)      803 2023-03-26 23:59:07.000000 chatwizard-0.1.0/scripts/prompts/grammar.txt
--rw-r--r--   0 ulasonat   (501) staff       (20)      947 2023-03-26 23:59:07.000000 chatwizard-0.1.0/scripts/prompts/humor.txt
-drwxr-xr-x   0 ulasonat   (501) staff       (20)        0 2023-03-27 00:33:49.379648 chatwizard-0.1.0/scripts/tests_tmp/
--rw-r--r--   0 ulasonat   (501) staff       (20)       49 2023-03-26 23:59:07.000000 chatwizard-0.1.0/scripts/tests_tmp/temp_user_scores.json
--rw-r--r--   0 ulasonat   (501) staff       (20)      235 2023-03-26 23:59:07.000000 chatwizard-0.1.0/scripts/tests_tmp/test_log.txt
--rw-r--r--   0 ulasonat   (501) staff       (20)       26 2023-03-26 23:59:07.000000 chatwizard-0.1.0/scripts/tests_tmp/test_user_scores.json
--rw-r--r--   0 ulasonat   (501) staff       (20)     6059 2023-03-26 23:59:07.000000 chatwizard-0.1.0/scripts/unit_tests.py
--rw-r--r--   0 ulasonat   (501) staff       (20)       38 2023-03-27 00:33:49.379967 chatwizard-0.1.0/setup.cfg
--rw-r--r--   0 ulasonat   (501) staff       (20)      483 2023-03-27 00:33:15.000000 chatwizard-0.1.0/setup.py
--rw-r--r--   0 ulasonat   (501) staff       (20)       50 2023-03-26 23:59:07.000000 chatwizard-0.1.0/test_path
+drwxr-xr-x   0 ulasonat   (501) staff       (20)        0 2023-05-04 22:57:44.978027 chatwizard-0.2.0/
+-rw-r--r--   0 ulasonat   (501) staff       (20)      296 2023-05-04 21:58:52.000000 chatwizard-0.2.0/.bumpversion.cfg
+-rw-r--r--   0 ulasonat   (501) staff       (20)     2193 2023-05-04 21:21:02.000000 chatwizard-0.2.0/CONTRIBUTING.md
+-rw-r--r--   0 ulasonat   (501) staff       (20)     1074 2023-05-04 21:21:02.000000 chatwizard-0.2.0/LICENSE
+-rw-r--r--   0 ulasonat   (501) staff       (20)      674 2023-05-04 21:21:02.000000 chatwizard-0.2.0/MANIFEST.in
+-rw-r--r--   0 ulasonat   (501) staff       (20)     2287 2023-05-04 21:21:02.000000 chatwizard-0.2.0/Makefile
+-rw-r--r--   0 ulasonat   (501) staff       (20)     6187 2023-05-04 22:57:44.977853 chatwizard-0.2.0/PKG-INFO
+-rw-r--r--   0 ulasonat   (501) staff       (20)     3959 2023-05-04 21:58:52.000000 chatwizard-0.2.0/README.md
+drwxr-xr-x   0 ulasonat   (501) staff       (20)        0 2023-05-04 22:57:44.972935 chatwizard-0.2.0/chatwizard.egg-info/
+-rw-r--r--   0 ulasonat   (501) staff       (20)     6187 2023-05-04 22:57:44.000000 chatwizard-0.2.0/chatwizard.egg-info/PKG-INFO
+-rw-r--r--   0 ulasonat   (501) staff       (20)      756 2023-05-04 22:57:44.000000 chatwizard-0.2.0/chatwizard.egg-info/SOURCES.txt
+-rw-r--r--   0 ulasonat   (501) staff       (20)        1 2023-05-04 22:57:44.000000 chatwizard-0.2.0/chatwizard.egg-info/dependency_links.txt
+-rw-r--r--   0 ulasonat   (501) staff       (20)      177 2023-05-04 22:57:44.000000 chatwizard-0.2.0/chatwizard.egg-info/requires.txt
+-rw-r--r--   0 ulasonat   (501) staff       (20)        1 2023-05-04 22:57:44.000000 chatwizard-0.2.0/chatwizard.egg-info/top_level.txt
+drwxr-xr-x   0 ulasonat   (501) staff       (20)        0 2023-05-04 22:57:44.973694 chatwizard-0.2.0/docs/
+-rw-r--r--   0 ulasonat   (501) staff       (20)    81091 2023-05-04 21:21:02.000000 chatwizard-0.2.0/docs/demo.png
+-rw-r--r--   0 ulasonat   (501) staff       (20)       80 2023-05-04 21:21:02.000000 chatwizard-0.2.0/docs/documentation.rst
+-rw-r--r--   0 ulasonat   (501) staff       (20)      228 2023-05-04 21:21:02.000000 chatwizard-0.2.0/docs/index.rst
+-rw-r--r--   0 ulasonat   (501) staff       (20)     4132 2023-05-04 21:21:02.000000 chatwizard-0.2.0/docs/overview.rst
+-rw-r--r--   0 ulasonat   (501) staff       (20)     2262 2023-05-04 21:58:52.000000 chatwizard-0.2.0/pyproject.toml
+drwxr-xr-x   0 ulasonat   (501) staff       (20)        0 2023-05-04 22:57:44.975460 chatwizard-0.2.0/scripts/
+drwxr-xr-x   0 ulasonat   (501) staff       (20)        0 2023-05-04 22:57:44.975726 chatwizard-0.2.0/scripts/.idea/
+-rw-r--r--   0 ulasonat   (501) staff       (20)     4297 2023-05-04 21:21:02.000000 chatwizard-0.2.0/scripts/.idea/workspace.xml
+-rw-r--r--   0 ulasonat   (501) staff       (20)       22 2023-05-04 21:58:52.000000 chatwizard-0.2.0/scripts/_version.py
+-rw-r--r--   0 ulasonat   (501) staff       (20)     9358 2023-05-04 21:21:02.000000 chatwizard-0.2.0/scripts/discord_bot.py
+-rw-r--r--   0 ulasonat   (501) staff       (20)     2887 2023-05-04 21:21:02.000000 chatwizard-0.2.0/scripts/integration_tests.py
+drwxr-xr-x   0 ulasonat   (501) staff       (20)        0 2023-05-04 22:57:44.975939 chatwizard-0.2.0/scripts/json/
+-rw-r--r--   0 ulasonat   (501) staff       (20)      142 2023-05-04 21:21:02.000000 chatwizard-0.2.0/scripts/json/user_scores.json
+drwxr-xr-x   0 ulasonat   (501) staff       (20)        0 2023-05-04 22:57:44.976125 chatwizard-0.2.0/scripts/log/
+-rw-r--r--   0 ulasonat   (501) staff       (20)     2567 2023-05-04 21:21:02.000000 chatwizard-0.2.0/scripts/log/log.txt
+-rw-r--r--   0 ulasonat   (501) staff       (20)     2397 2023-05-04 21:21:02.000000 chatwizard-0.2.0/scripts/main.py
+-rw-r--r--   0 ulasonat   (501) staff       (20)     6440 2023-05-04 21:21:02.000000 chatwizard-0.2.0/scripts/openai_handler.py
+drwxr-xr-x   0 ulasonat   (501) staff       (20)        0 2023-05-04 22:57:44.976696 chatwizard-0.2.0/scripts/prompts/
+-rw-r--r--   0 ulasonat   (501) staff       (20)      895 2023-05-04 21:21:02.000000 chatwizard-0.2.0/scripts/prompts/friendliness.txt
+-rw-r--r--   0 ulasonat   (501) staff       (20)      803 2023-05-04 21:21:02.000000 chatwizard-0.2.0/scripts/prompts/grammar.txt
+-rw-r--r--   0 ulasonat   (501) staff       (20)      947 2023-05-04 21:21:02.000000 chatwizard-0.2.0/scripts/prompts/humor.txt
+drwxr-xr-x   0 ulasonat   (501) staff       (20)        0 2023-05-04 22:57:44.977591 chatwizard-0.2.0/scripts/tests_tmp/
+-rw-r--r--   0 ulasonat   (501) staff       (20)       49 2023-05-04 21:21:02.000000 chatwizard-0.2.0/scripts/tests_tmp/temp_user_scores.json
+-rw-r--r--   0 ulasonat   (501) staff       (20)      235 2023-05-04 21:21:02.000000 chatwizard-0.2.0/scripts/tests_tmp/test_log.txt
+-rw-r--r--   0 ulasonat   (501) staff       (20)       26 2023-05-04 21:21:02.000000 chatwizard-0.2.0/scripts/tests_tmp/test_user_scores.json
+-rw-r--r--   0 ulasonat   (501) staff       (20)     6481 2023-05-04 21:56:38.000000 chatwizard-0.2.0/scripts/unit_tests.py
+-rw-r--r--   0 ulasonat   (501) staff       (20)       38 2023-05-04 22:57:44.978076 chatwizard-0.2.0/setup.cfg
+-rw-r--r--   0 ulasonat   (501) staff       (20)      411 2023-05-04 21:58:52.000000 chatwizard-0.2.0/setup.py
+-rw-r--r--   0 ulasonat   (501) staff       (20)       50 2023-05-04 21:21:02.000000 chatwizard-0.2.0/test_path
```

### Comparing `chatwizard-0.1.0/CONTRIBUTING.md` & `chatwizard-0.2.0/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `chatwizard-0.1.0/LICENSE` & `chatwizard-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `chatwizard-0.1.0/MANIFEST.in` & `chatwizard-0.2.0/MANIFEST.in`

 * *Files 8% similar despite different names*

```diff
@@ -6,21 +6,24 @@
 
 include .bumpversion.cfg
 include pyproject.toml
 include Makefile
 include .coveragerc
 include test_path
 
+include *.png
 include *.md
 include .bumpversion.cfg
 include Makefile
 recursive-include scripts *.json
 recursive-include scripts *.py
 recursive-include scripts *.txt
 recursive-include scripts *.xml
+recursive-include docs *.png
+recursive-include docs *.rst
 
 prune .github
 exclude .gitignore
 exclude .gitattributes
 
 # Patterns to exclude from any directory
 global-exclude *~
```

### Comparing `chatwizard-0.1.0/Makefile` & `chatwizard-0.2.0/Makefile`

 * *Files identical despite different names*

### Comparing `chatwizard-0.1.0/README.md` & `chatwizard-0.2.0/README.md`

 * *Files 19% similar despite different names*

```diff
@@ -2,27 +2,33 @@
 Discord bot to encourage positiveness within a server by analyzing and scoring each member's behavior.
 
 
 ![](https://img.shields.io/github/license/ulasonat/prime-video-plus?color=blue&label=License)
 ![](https://img.shields.io/github/issues/ulasonat/ChatWizard)
 [![Build Status](https://github.com/ulasonat/ChatWizard/actions/workflows/build.yml/badge.svg?branch=main)](https://github.com/ulasonat/ChatWizard/actions/workflows/build.yml)
 [![codecov](https://codecov.io/gh/ulasonat/ChatWizard/branch/main/graph/badge.svg?token=G2AE2OWNO3)](https://codecov.io/gh/ulasonat/ChatWizard)
+[![](https://img.shields.io/pypi/v/chatwizard?color=blue)](https://pypi.org/project/chatwizard/)
+[![Documentation Status](https://readthedocs.org/projects/chatwizard/badge/?version=doc_website)](https://chatwizard.readthedocs.io/en/doc_website/?badge=doc_website)
 
 
 ## Overview
 
 ChatWizard is a Discord bot that encourages positivity within a server by analyzing and scoring each member's behavior. It uses OpenAI's GPT-3.5-turbo to assess members based on factors such as helpfulness, language use, friendliness, and humor. With ChatWizard, you can create a more welcoming, engaging, and supportive environment for everyone in your server.
 
 ## Features
 
-- Analyzes and scores server members based on grammar, friendliness, and humor.
+- Analyzes and scores server members based on grammar, friendliness, and humor values of their messages.
 - Encourages and rewards positive contributions to the server.
 - Provides a score breakdown so members can see how they're performing in each category.
 - Logs all messages sent, making it easy to review member behavior.
 
+## Demo
+
+<img src="demo.png" alt="Demo Image" style="width:50%;height:50%;">
+
 ## Dependencies 
 1. Python 3.6 or higher
 2. `discord.py` module (v1.7.3 or higher)
 3. `openai` module (v0.11.1 or higher)
 4. OpenAI API key (v4)
 5. A Discord user account and server
 
@@ -63,14 +69,34 @@
 
 Alternatively, you can import the library and call the main.run function by passing the Discord API key, OpenAI API key as arguments. Then, run the bot using the `run` method.
 
 ```python
 run(discord_api_key, openai_api_key)
 ```
 
+Moreover, you can have instances of either OpenAIHandler or DiscordBot classes, and use the functions available.
+If you want to use our library to get a humor score for the sentence, you can do the following:
+
+```python
+from openai_handler import OpenAIHandler
+
+openai_handler = OpenAIHandler(
+    api_key=open_ai_api_key,
+    grammar_prompt_path=grammar_prompt_path,
+    friendliness_prompt_path=friendliness_prompt_path,
+    humor_prompt_path=humor_prompt_path,
+)
+
+worst_joke_ever = 'Why did the tomato turn red? Because it saw the salad dressing!'
+
+humor_score = openai_handler.get_humor_score(worst_joke_ever)
+```
+
+More examples are included in our project's website.
+
 ## Bot Commands
 
 - To get help: `!help`
 - To view your scores: `!me`
 - To reset your scores: `!reset`
 
 After sending a message, ChatWizard will reply with an embed showing the score breakdown for that message.
```

### Comparing `chatwizard-0.1.0/chatwizard.egg-info/SOURCES.txt` & `chatwizard-0.2.0/chatwizard.egg-info/SOURCES.txt`

 * *Files 21% similar despite different names*

```diff
@@ -8,14 +8,18 @@
 setup.py
 test_path
 chatwizard.egg-info/PKG-INFO
 chatwizard.egg-info/SOURCES.txt
 chatwizard.egg-info/dependency_links.txt
 chatwizard.egg-info/requires.txt
 chatwizard.egg-info/top_level.txt
+docs/demo.png
+docs/documentation.rst
+docs/index.rst
+docs/overview.rst
 scripts/_version.py
 scripts/discord_bot.py
 scripts/integration_tests.py
 scripts/main.py
 scripts/openai_handler.py
 scripts/unit_tests.py
 scripts/.idea/workspace.xml
```

### Comparing `chatwizard-0.1.0/pyproject.toml` & `chatwizard-0.2.0/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 build-backend="setuptools.build_meta"
 
 [project]
 name = "chatwizard"
 authors = [{name = "Ulas Onat Alakent", email = "ulas.alakent@columbia.edu"}]
 description="Your DiscordBot for a safer environment"
 readme = "README.md"
-version="0.1.0"
+version="0.2.0"
 requires-python = ">=3.7"
 
 dependencies = []
 
 classifiers = [
     "Development Status :: 2 - Pre-Alpha",
     "Programming Language :: Python :: Implementation :: CPython",
```

### Comparing `chatwizard-0.1.0/scripts/.idea/workspace.xml` & `chatwizard-0.2.0/scripts/.idea/workspace.xml`

 * *Files identical despite different names*

### Comparing `chatwizard-0.1.0/scripts/discord_bot.py` & `chatwizard-0.2.0/scripts/discord_bot.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,38 +1,57 @@
+"""
+This script contains the implementation of the DiscordBot class, which is responsible for interacting with the
+Discord API and OpenAI's GPT-3.5-turbo API to analyze and score members' behavior based on different categories.
+"""
+
 import discord
 import os
 import json
 
 
 class DiscordBot(discord.Client):
+    """
+    A class that represents a Discord bot that encourages positivity
+    within a server by analyzing and scoring each member's behavior.
+    """
+
     def __init__(self, intents, openai_handler, log_file_path, user_scores_path):
         """
         Initializes a new instance of the DiscordBot class.
+
+        Parameters:
+            intents (discord.Intents): The intents of the discord client.
+            openai_handler (OpenAIHandler): The OpenAI API handler for the bot.
+            log_file_path (str): The log file path to store logs.
+            user_scores_path (str): The user scores file path to store user scores.
         """
 
         super().__init__(intents=intents)
         self.openai_handler = openai_handler
         self.log_file_path = log_file_path
         self.user_scores_path = user_scores_path
         self.user_scores = self.load_user_scores()
         self.categories = ['grammar', 'friendliness', 'humor']
 
     async def on_ready(self):
         """
-        A callback method that is called when the bot connects
-         to the Discord API.
-        Prints a message to the console indicating that the
-        bot has connected to Discord.
+        A callback method that is called when bot connects to Discord.
+        It prints a message to the console indicating that the bot has connected to Discord.
         """
+
         print(f"{self.user} has connected to Discord!")
 
     async def on_message(self, message):
         """
-        A callback method that is called when the bot
-        receives a message from a user.
+        A callback method that is called when the bot receives a message from a user.
+        It processes the text and generates scores on categories such as grammar, friendliness, and humor, and
+        responds with the scores and the appropriate label.
+
+        Parameters:
+            message (discord.Message): The message recieved from the discord server.
         """
 
         if not self.scan_message(message):
             return
 
         self.update_log_file(message.author, message.content)
 
@@ -111,90 +130,125 @@
 
             await message.channel.send(embed=embed)
 
     def scan_message(self, message):
         """
         Returns `True` if the message was sent by a user,
         and `False` otherwise, and prints the message
+
+        Parameters:
+            message (discord.Message): The message recieved from the discord server.
+
+        Returns:
+            bool: Whether the message was sent by a user or not.
         """
         if message.author == self.user:
             return False
 
         return True
 
     def update_scores(self, user_id, scores):
         """
         Updates the scores of the given user ID with the
-        scores from the most recent message they sent
+        scores from the most recent message they sent.
+
+        Parameters:
+            user_id (str): The user id whose scores needs to be updated.
+            scores (dict): A dictionary containing scores on different categories.
         """
         if user_id not in self.user_scores:
             self.user_scores[user_id] = self.openai_handler.generate_default_scores()
 
         self.save_updated_scores(user_id, scores)
 
     def save_updated_scores(self, user_id, scores):
         """
-        Saves the updated scores
+        Updates the scores for the given user ID with the scores from the most recent message sent by the user.
+
+        Parameters:
+            user_id (str): Unique ID of the user whose scores are being updated.
+            scores (dict): A dictionary containing the updated scores for the user.
         """
         self.user_scores[user_id]["grammar"] += scores["grammar"]
         self.user_scores[user_id]["friendliness"] += scores["friendliness"]
         self.user_scores[user_id]["humor"] += scores["humor"]
         self.save_user_scores()
 
     def load_user_scores(self):
         """
         Loads the user scores from the JSON file.
-        Returns a dictionary that maps user IDs to their scores.
+
+        Returns:
+            dict: A dictionary that maps user IDs to their scores.
         """
         if not os.path.exists(self.user_scores_path):
             return {}
 
         with open(self.user_scores_path, "r") as file:
             return json.load(file)
 
     def save_user_scores(self):
         """
-        Saves the user scores to the JSON file.
+        Saves the user scores to the JSON file by writing the self.user_scores dictionary to the JSON file.
         """
+
         with open(self.user_scores_path, "w") as file:
             json.dump(self.user_scores, file)
 
     def update_log_file(self, nickname, content):
         """
         Appends the nickname and message content to the log file.
         If the log file does not exist, creates a new log file.
+
+        Parameters:
+            nickname (str): The nickname of the user who sent the message.
+            content (str): The content of the message.
         """
 
         if not os.path.exists(self.log_file_path):
             with open(self.log_file_path, "w") as log_file:
                 log_file.write("Log file created.\n")
 
         with open(self.log_file_path, "a") as log_file:
             log_file.write(f"{nickname}: {content}\n")
 
+    def score_to_word(self, score_map, score):
+        """
+        Returns the corresponding word for a given score from the provided score map.
+
+        Parameters:
+            score_map (dict): The dictionary containing the score-word mapping.
+            score (int): The score in the range [-1, 0, 1].
+
+        Returns:
+            str: The corresponding word for the score in the score map.
+        """
+        if score in score_map:
+            return score_map[score]
+        else:
+            raise ValueError("Invalid score.")
+
     def get_corresponding_word(self, label, score):
-        if label not in self.categories:
-            raise ValueError
-        if score not in [-1, 0, 1]:
-            raise ValueError
-
-        if label == 'grammar':
-            if score == 1:
-                return 'Appropriate'
-            if score == 0:
-                return 'Mediocre'
-            if score == -1:
-                return 'Bad'
-        elif label == 'friendliness':
-            if score == 1:
-                return 'Friendly'
-            if score == 0:
-                return 'Natural'
-            if score == -1:
-                return 'Not friendly'
-        elif label == 'humor':
-            if score == 1:
-                return 'Funny'
-            if score == 0:
-                return 'Mediocre'
-            if score == -1:
-                return 'Not funny'
+        """
+        Returns the corresponding word for a given score and label.
+
+        Parameters:
+            label (str): The label/category for the score.
+            score (int): The score in the range [-1,0,1].
+
+        Returns:
+            str: The corresponding word for the score and label.
+
+        Raises:
+            ValueError: If label or score are not recognized or invalid.
+        """
+        valid_labels = ['grammar', 'friendliness', 'humor']
+        words = {
+            'grammar': {1: 'Appropriate', 0: 'Mediocre', -1: 'Bad'},
+            'friendliness': {1: 'Friendly', 0: 'Natural', -1: 'Not friendly'},
+            'humor': {1: 'Funny', 0: 'Mediocre', -1: 'Not funny'},
+        }
+
+        if label not in valid_labels:
+            raise ValueError("Invalid label.")
+
+        return self.score_to_word(words[label], score)
```

### Comparing `chatwizard-0.1.0/scripts/integration_tests.py` & `chatwizard-0.2.0/scripts/integration_tests.py`

 * *Files identical despite different names*

### Comparing `chatwizard-0.1.0/scripts/log/log.txt` & `chatwizard-0.2.0/scripts/log/log.txt`

 * *Files identical despite different names*

### Comparing `chatwizard-0.1.0/scripts/openai_handler.py` & `chatwizard-0.2.0/scripts/openai_handler.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,55 +1,96 @@
+"""
+This script handles interactions with OpenAI's API and includes methods to calculate scores in three categories:
+grammar, friendliness, and humor.
+"""
+
 import openai
 
 
 class OpenAIHandler:
+    """
+    Initializes a new instance of the OpenAIHandler class.
+
+    Parameters:
+        api_key (str): API key for OpenAI API
+        grammar_prompt_path (str): Path to grammar prompt text file
+        friendliness_prompt_path (str): Path to friendliness prompt text file
+        humor_prompt_path (str): Path to humor prompt text file
+    """
+
     def __init__(self, api_key, grammar_prompt_path, friendliness_prompt_path, humor_prompt_path):
         """
         Initializes a new instance of the OpenAIHandler class.
+
+        Parameters:
+            api_key (str): API key for OpenAI API
+            grammar_prompt_path (str): path to grammar prompt text file
+            friendliness_prompt_path (str): path to friendliness prompt text file
+            humor_prompt_path (str): path to humor prompt text file
         """
         self.api_key = api_key
         self.grammar_prompt_path = grammar_prompt_path
         self.friendliness_prompt_path = friendliness_prompt_path
         self.humor_prompt_path = humor_prompt_path
 
         openai.api_key = api_key
 
     def get_response(self, content):
         """
         Sends a prompt to the OpenAI API and returns the generated response.
+
+        Parameters:
+            content (str): text input prompt for OpenAI API
+
+        Returns:
+            str: generated response from OpenAI API
         """
-        # The code below returns a response using
-        # OpenAI based on the message.content that will be passed
         response = openai.ChatCompletion.create(
             model="gpt-4",
             messages=[
                 {"role": "system", "content": content},
             ],
         )
         return response.choices[0]["message"]["content"]
 
     def generate_default_scores(self):
         """
         Generates default scores for each category.
+
+        Returns:
+            dict: default scores for each category
         """
         return {"grammar": 10, "friendliness": 10, "humor": 10}
 
     def get_message_score(self, content):
         """
-        Processes the text and generates various
-         scores on different categories.
-        """
+        Processes the text and generates various scores on different categories.
+
+        Parameters:
+            content (str): text to generate score for
 
+        Returns:
+            dict: scores for each category
+        """
         return {
             "grammar": self.get_grammar_score(content),
             "friendliness": self.get_friendliness_score(content),
             "humor": self.get_humor_score(content),
         }
 
     def get_grammar_score(self, content):
+        """
+        Calculates the grammar score for a given message.
+
+        Parameters:
+            content (str): text to generate score for
+
+        Returns:
+            int: grammar score [-1, 0, 1]
+        """
         with open(self.grammar_prompt_path, "r") as file:
             prompt = file.read()
 
         prompt += content
 
         try:
             response = openai.ChatCompletion.create(
@@ -78,14 +119,23 @@
             return -1
         if grammar_score == 0:
             return 0
         if grammar_score >= 0:
             return 1
 
     def get_friendliness_score(self, content):
+        """
+        Calculates the friendliness score for a given message.
+
+        Parameters:
+            content (str): text to generate score for
+
+        Returns:
+            int: friendliness score [-1, 0, 1]
+        """
         with open(self.friendliness_prompt_path, "r") as file:
             prompt = file.read()
 
         prompt += content
 
         try:
             response = openai.ChatCompletion.create(
@@ -114,14 +164,27 @@
             return -1
         if friendliness_score == 0:
             return 0
         if friendliness_score >= 0:
             return 1
 
     def get_humor_score(self, content):
+        """
+        Calculates the humor score for a given message.
+
+        Parameters:
+            content (str): text to generate score for
+
+        Returns:
+            int: humor score [-1, 0, 1]
+
+        Raises:
+            AuthenticationError: raised if no API key provided
+            ValueError: raised if API does not produce pure numerical output
+        """
         with open(self.humor_prompt_path, "r") as file:
             prompt = file.read()
 
         prompt += content
 
         try:
             response = openai.ChatCompletion.create(
```

### Comparing `chatwizard-0.1.0/scripts/prompts/friendliness.txt` & `chatwizard-0.2.0/scripts/prompts/friendliness.txt`

 * *Files identical despite different names*

### Comparing `chatwizard-0.1.0/scripts/prompts/grammar.txt` & `chatwizard-0.2.0/scripts/prompts/grammar.txt`

 * *Files identical despite different names*

### Comparing `chatwizard-0.1.0/scripts/prompts/humor.txt` & `chatwizard-0.2.0/scripts/prompts/humor.txt`

 * *Files identical despite different names*

### Comparing `chatwizard-0.1.0/scripts/unit_tests.py` & `chatwizard-0.2.0/scripts/unit_tests.py`

 * *Files 4% similar despite different names*

```diff
@@ -58,15 +58,14 @@
 def test_scan_message(bot):
     message_from_bot = Mock(author=bot.user, content=Faker().text())
     message_from_user = Mock(author="user", content=Faker().text())
 
     assert not bot.scan_message(message_from_bot)
     assert bot.scan_message(message_from_user)
 
-
 def test_save_updated_scores(bot):
     test_user_id = Faker().pyint()
     test_scores = {"grammar": 10, "friendliness": 10, "humor": 10}
 
     assert test_user_id not in bot.user_scores
     bot.user_scores[test_user_id] = test_scores
     bot.save_updated_scores(test_user_id, test_scores)
@@ -188,13 +187,28 @@
     assert bot.get_corresponding_word('humor', -1) == 'Not funny'
 
     with pytest.raises(ValueError):
         bot.get_corresponding_word('invalid_label', 1)
         bot.get_corresponding_word('grammar', 2)
 
 
+def test_score_to_word(bot):
+    score_map = {1: "Appropriate", 0: "Mediocre", -1: "Bad"}
+
+    result_1 = bot.score_to_word(score_map, 1)
+    result_0 = bot.score_to_word(score_map, 0)
+    result_minus1 = bot.score_to_word(score_map, -1)
+
+    assert result_1 == "Appropriate"
+    assert result_0 == "Mediocre"
+    assert result_minus1 == "Bad"
+
+    with pytest.raises(ValueError):
+        bot.score_to_word(score_map, 3)
+
+
 def test_run_invalid():
     open_ai_api_key = '12345'
     discord_api_key = '67890'
 
     with pytest.raises(discord.errors.DiscordException):
         run(open_ai_api_key, discord_api_key)
```

