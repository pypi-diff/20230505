# Comparing `tmp/polling-bot-0.1.0.tar.gz` & `tmp/polling-bot-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "polling-bot-0.1.0.tar", last modified: Sun Mar 26 19:57:06 2023, max compression
+gzip compressed data, was "polling-bot-0.2.0.tar", last modified: Thu May  4 07:09:27 2023, max compression
```

## Comparing `polling-bot-0.1.0.tar` & `polling-bot-0.2.0.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxrwxrwx   0 ganes     (1000) ganes     (1000)        0 2023-03-26 19:57:06.382154 polling-bot-0.1.0/
--rwxrwxrwx   0 ganes     (1000) ganes     (1000)      296 2023-03-26 19:18:01.000000 polling-bot-0.1.0/.bumpversion.cfg
--rwxrwxrwx   0 ganes     (1000) ganes     (1000)      817 2023-03-26 19:18:01.000000 polling-bot-0.1.0/CONTRIBUTING.md
--rwxrwxrwx   0 ganes     (1000) ganes     (1000)     1074 2023-03-26 19:18:01.000000 polling-bot-0.1.0/LICENSE
--rwxrwxrwx   0 ganes     (1000) ganes     (1000)      394 2023-03-26 19:18:01.000000 polling-bot-0.1.0/MANIFEST.in
--rwxrwxrwx   0 ganes     (1000) ganes     (1000)     2281 2023-03-26 19:18:01.000000 polling-bot-0.1.0/Makefile
--rwxrwxrwx   0 ganes     (1000) ganes     (1000)     6007 2023-03-26 19:57:06.382154 polling-bot-0.1.0/PKG-INFO
--rwxrwxrwx   0 ganes     (1000) ganes     (1000)     3875 2023-03-26 19:18:01.000000 polling-bot-0.1.0/README.md
-drwxrwxrwx   0 ganes     (1000) ganes     (1000)        0 2023-03-26 19:57:06.366537 polling-bot-0.1.0/polling-bot/
--rwxrwxrwx   0 ganes     (1000) ganes     (1000)       34 2023-03-26 19:18:01.000000 polling-bot-0.1.0/polling-bot/__init__.py
--rwxrwxrwx   0 ganes     (1000) ganes     (1000)      356 2023-03-26 19:18:01.000000 polling-bot-0.1.0/polling-bot/__main__.py
--rwxrwxrwx   0 ganes     (1000) ganes     (1000)       22 2023-03-26 19:18:01.000000 polling-bot-0.1.0/polling-bot/_version.py
--rwxrwxrwx   0 ganes     (1000) ganes     (1000)     7860 2023-03-26 19:18:01.000000 polling-bot-0.1.0/polling-bot/polling_bot.py
-drwxrwxrwx   0 ganes     (1000) ganes     (1000)        0 2023-03-26 19:57:06.366537 polling-bot-0.1.0/polling-bot/tests/
--rwxrwxrwx   0 ganes     (1000) ganes     (1000)     7002 2023-03-26 19:18:01.000000 polling-bot-0.1.0/polling-bot/tests/tests.py
-drwxrwxrwx   0 ganes     (1000) ganes     (1000)        0 2023-03-26 19:57:06.366537 polling-bot-0.1.0/polling_bot.egg-info/
--rwxrwxrwx   0 ganes     (1000) ganes     (1000)     6007 2023-03-26 19:57:06.000000 polling-bot-0.1.0/polling_bot.egg-info/PKG-INFO
--rwxrwxrwx   0 ganes     (1000) ganes     (1000)      395 2023-03-26 19:57:06.000000 polling-bot-0.1.0/polling_bot.egg-info/SOURCES.txt
--rwxrwxrwx   0 ganes     (1000) ganes     (1000)        1 2023-03-26 19:57:06.000000 polling-bot-0.1.0/polling_bot.egg-info/dependency_links.txt
--rwxrwxrwx   0 ganes     (1000) ganes     (1000)      187 2023-03-26 19:57:06.000000 polling-bot-0.1.0/polling_bot.egg-info/requires.txt
--rwxrwxrwx   0 ganes     (1000) ganes     (1000)        1 2023-03-26 19:57:06.000000 polling-bot-0.1.0/polling_bot.egg-info/top_level.txt
--rwxrwxrwx   0 ganes     (1000) ganes     (1000)     2298 2023-03-26 19:32:27.000000 polling-bot-0.1.0/pyproject.toml
--rwxrwxrwx   0 ganes     (1000) ganes     (1000)       38 2023-03-26 19:57:06.382154 polling-bot-0.1.0/setup.cfg
--rwxrwxrwx   0 ganes     (1000) ganes     (1000)       39 2023-03-26 19:18:01.000000 polling-bot-0.1.0/setup.py
+drwxrwxrwx   0 ganes     (1000) ganes     (1000)        0 2023-05-05 03:31:44.414222 polling-bot-0.2.0/
+-rwxrwxrwx   0 ganes     (1000) ganes     (1000)      296 2023-05-05 02:47:44.000000 polling-bot-0.2.0/.bumpversion.cfg
+-rwxrwxrwx   0 ganes     (1000) ganes     (1000)      817 2023-05-05 02:47:44.000000 polling-bot-0.2.0/CONTRIBUTING.md
+-rwxrwxrwx   0 ganes     (1000) ganes     (1000)     1074 2023-05-05 02:47:44.000000 polling-bot-0.2.0/LICENSE
+-rwxrwxrwx   0 ganes     (1000) ganes     (1000)      571 2023-05-05 03:24:28.000000 polling-bot-0.2.0/MANIFEST.in
+-rwxrwxrwx   0 ganes     (1000) ganes     (1000)     2645 2023-05-05 02:47:44.000000 polling-bot-0.2.0/Makefile
+-rwxrwxrwx   0 ganes     (1000) ganes     (1000)     6559 2023-05-05 03:31:44.398997 polling-bot-0.2.0/PKG-INFO
+-rwxrwxrwx   0 ganes     (1000) ganes     (1000)     4428 2023-05-05 02:47:44.000000 polling-bot-0.2.0/README.md
+drwxrwxrwx   0 ganes     (1000) ganes     (1000)        0 2023-05-05 03:31:43.659511 polling-bot-0.2.0/polling-bot/
+-rwxrwxrwx   0 ganes     (1000) ganes     (1000)       61 2023-05-05 02:47:45.000000 polling-bot-0.2.0/polling-bot/__init__.py
+-rwxrwxrwx   0 ganes     (1000) ganes     (1000)      398 2023-05-05 02:47:45.000000 polling-bot-0.2.0/polling-bot/__main__.py
+-rwxrwxrwx   0 ganes     (1000) ganes     (1000)       22 2023-05-05 02:47:45.000000 polling-bot-0.2.0/polling-bot/_version.py
+-rwxrwxrwx   0 ganes     (1000) ganes     (1000)    15188 2023-05-05 02:47:45.000000 polling-bot-0.2.0/polling-bot/polling_bot.py
+drwxrwxrwx   0 ganes     (1000) ganes     (1000)        0 2023-05-05 03:31:43.770155 polling-bot-0.2.0/polling-bot/tests/
+-rwxrwxrwx   0 ganes     (1000) ganes     (1000)    10157 2023-05-05 02:47:45.000000 polling-bot-0.2.0/polling-bot/tests/tests.py
+drwxrwxrwx   0 ganes     (1000) ganes     (1000)        0 2023-05-05 03:31:44.276539 polling-bot-0.2.0/polling_bot.egg-info/
+-rwxrwxrwx   0 ganes     (1000) ganes     (1000)     6559 2023-05-05 03:31:42.000000 polling-bot-0.2.0/polling_bot.egg-info/PKG-INFO
+-rwxrwxrwx   0 ganes     (1000) ganes     (1000)      395 2023-05-05 03:31:42.000000 polling-bot-0.2.0/polling_bot.egg-info/SOURCES.txt
+-rwxrwxrwx   0 ganes     (1000) ganes     (1000)        1 2023-05-05 03:31:42.000000 polling-bot-0.2.0/polling_bot.egg-info/dependency_links.txt
+-rwxrwxrwx   0 ganes     (1000) ganes     (1000)      187 2023-05-05 03:31:42.000000 polling-bot-0.2.0/polling_bot.egg-info/requires.txt
+-rwxrwxrwx   0 ganes     (1000) ganes     (1000)        1 2023-05-05 03:31:42.000000 polling-bot-0.2.0/polling_bot.egg-info/top_level.txt
+-rwxrwxrwx   0 ganes     (1000) ganes     (1000)     2298 2023-05-05 03:30:44.000000 polling-bot-0.2.0/pyproject.toml
+-rwxrwxrwx   0 ganes     (1000) ganes     (1000)       38 2023-05-05 03:31:44.418553 polling-bot-0.2.0/setup.cfg
+-rwxrwxrwx   0 ganes     (1000) ganes     (1000)       39 2023-05-05 02:47:45.000000 polling-bot-0.2.0/setup.py
```

### Comparing `polling-bot-0.1.0/CONTRIBUTING.md` & `polling-bot-0.2.0/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `polling-bot-0.1.0/LICENSE` & `polling-bot-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `polling-bot-0.1.0/Makefile` & `polling-bot-0.2.0/Makefile`

 * *Files 13% similar despite different names*

```diff
@@ -72,14 +72,34 @@
 	python3 -m twine check dist/*
 
 dist: clean build dist-build dist-check  ## Build dists
 
 publish:  # Upload python assets
 	echo "would usually run python3 -m twine upload dist/* --skip-existing"
 
+########
+# DOCS #
+########
+
+TMPREPO=/tmp/docs/polling-bot
+
+docs: 
+	$(MAKE) -C docs/ clean
+	$(MAKE) -C docs/ html
+
+pages: 
+	rm -rf $(TMPREPO)
+	git clone -b gh-pages https://github.com/grnarayanan/polling-bot.git $(TMPREPO)
+	rm -rf $(TMPREPO)/*
+	cp -r docs/build/html/* $(TMPREPO)
+	cd $(TMPREPO);\
+	git add -A ;\
+	git commit -a -m 'auto-updating docs' ;\
+	git push
+
 #########
 # CLEAN #
 #########
 deep-clean: ## clean everything from the repository
 	git clean -fdx
 
 clean: ## clean the repository
```

### Comparing `polling-bot-0.1.0/PKG-INFO` & `polling-bot-0.2.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: polling-bot
-Version: 0.1.0
+Version: 0.2.0
 Summary: polling-bot is a Discord bot to conduct basic polling functions in a Discord server
 Author-email: Ganesan Narayanan <ganesan.narayanan24@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 Ganesan Narayanan
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -43,23 +43,24 @@
 # polling-bot
 
 polling-bot is a Discord bot to conduct basic polling functions in a Discord server
 
 [![Build Status](https://github.com/grnarayanan/polling-bot/workflows/Build%20Status/badge.svg?branch=main)](https://github.com/grnarayanan/polling-bot/actions?query=workflow%3A%22Build+Status%22)
 [![codecov](https://codecov.io/gh/grnarayanan/polling-bot/branch/main/graph/badge.svg)](https://codecov.io/gh/grnarayanan/polling-bot)
 ![License](https://img.shields.io/github/license/grnarayanan/polling-bot.svg) ![GitHub issues](https://img.shields.io/github/issues/grnarayanan/polling-bot)
+[![PyPI](https://img.shields.io/pypi/v/polling-bot)](https://pypi.org/project/polling-bot/)
+[![Docs](https://img.shields.io/badge/docs-docs-green)](https://grnarayanan.github.io/polling-bot/)
 
 ## Overview
 
 Often times, reaching a consensus can be difficult without an organized method in place, and so this polling bot can be added to a Discord
 server to solve that need in a simple and efficient manner. Use cases could include deciding with friends on a place to eat, what video game 
 should be played, when to schedule a party, etc. 
 
-The bot supports starting a poll and adding options for choices by the users. It will then keep track of responses made to the poll,
-allow users to change their response, and surface the winner of the poll when called upon. 
+The bot supports starting a poll and adding options for choices by the users. It will then keep track of responses made to the poll, and surface the winner of the poll when called upon. 
 
 ## Details
 
 This project is a pure python project using modern tooling. It uses a `Makefile` as a command registry, with the following commands:
 - `make`: list available commands
 - `make develop`: install and build this library and its dependencies using `pip`
 - `make build`: build the library using `setuptools`
@@ -77,34 +78,45 @@
 2. Select "New Application" and give it a name ie. "polling-bot"
 3. Navigate to the Bot tab on the left side menu, and click "Add Bot" and confirm. 
 4. Under the TOKEN section, click "Copy" and copy the token.
 5. To add the bot to your Discord server, select the OAuth2 tab from the left side menu. From the SCOPES section, select bot option and from the BOT PERMISSIONS section, select Administrator. Copy and navigate to the generated URL and select the server you want to add the bot to from the dropdown, then click "Authorize."
 
 Next, install polling-bot with pip: `pip install polling-bot`.
 
-Navigate to the "polling-bot" directory and create a file called `.env` with the following content:
+Finally, to run the bot, import and run it as follows:
 
-`DISCORD_TOKEN={token}`, where token is the token copied from the Developer Portal above. 
+```python
 
-Finally, to run the bot, execute the command `python3 __main__.py`.
+import discord
+pollingbot = __import__("polling-bot")
+   
+bot = pollingbot.PollingBot(intents=discord.Intents.all(), command_prefix="/")
+bot.run('TOKEN')
+```
+
+Where token is the token copied from the Developer Portal above.
+
+The bot will now be responsive to commands in your Discord server. 
 
 ## Available Commands
 
 `/poll` - Starts a poll in the server
 
 `/add choice <content>` - Add choices to the poll
 
 `/edit <option> <content>` - Edit the content of the poll
 
-- Options are 'name', 'description', and 'choice'
+- Options are 'name', 'description', 'choice', and 'duration' (to alter how long the poll is open for [default is 5 mins])
 
 `/vote <choice #>` - Vote for a choice in the poll
 
 - Choice # is the # corresponding to the desired choice, viewable with `/view choices` or `/view poll`
 
 `/view <option>` - View the contents and results of the poll
 
 - Options are 'name', 'description', 'choices', 'poll', and 'results'
 
 ## Usage
 
 Start by executing `/poll` to create a poll. Edit the name and description of the poll using the `/edit` command. Next, add choices to the poll using the `/add` command. Have users then vote on the choices by running `/view poll` to see the current state of the poll, and then voting on their desired selection using the `/vote` command. Once all users have voted and the poll has concluded, run `/view results` to view the results and winner of the poll.
+
+<img src="https://github.com/grnarayanan/polling-bot/blob/main/docs/source/demos/short-version.gif" width="350" title="Quick demo using polling-bot in a Discord server" alt="Quick demo using polling-bot in a Discord server">
```

### Comparing `polling-bot-0.1.0/README.md` & `polling-bot-0.2.0/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 # polling-bot
 
 polling-bot is a Discord bot to conduct basic polling functions in a Discord server
 
 [![Build Status](https://github.com/grnarayanan/polling-bot/workflows/Build%20Status/badge.svg?branch=main)](https://github.com/grnarayanan/polling-bot/actions?query=workflow%3A%22Build+Status%22)
 [![codecov](https://codecov.io/gh/grnarayanan/polling-bot/branch/main/graph/badge.svg)](https://codecov.io/gh/grnarayanan/polling-bot)
 ![License](https://img.shields.io/github/license/grnarayanan/polling-bot.svg) ![GitHub issues](https://img.shields.io/github/issues/grnarayanan/polling-bot)
+[![PyPI](https://img.shields.io/pypi/v/polling-bot)](https://pypi.org/project/polling-bot/)
+[![Docs](https://img.shields.io/badge/docs-docs-green)](https://grnarayanan.github.io/polling-bot/)
 
 ## Overview
 
 Often times, reaching a consensus can be difficult without an organized method in place, and so this polling bot can be added to a Discord
 server to solve that need in a simple and efficient manner. Use cases could include deciding with friends on a place to eat, what video game 
 should be played, when to schedule a party, etc. 
 
-The bot supports starting a poll and adding options for choices by the users. It will then keep track of responses made to the poll,
-allow users to change their response, and surface the winner of the poll when called upon. 
+The bot supports starting a poll and adding options for choices by the users. It will then keep track of responses made to the poll, and surface the winner of the poll when called upon. 
 
 ## Details
 
 This project is a pure python project using modern tooling. It uses a `Makefile` as a command registry, with the following commands:
 - `make`: list available commands
 - `make develop`: install and build this library and its dependencies using `pip`
 - `make build`: build the library using `setuptools`
@@ -35,34 +36,45 @@
 2. Select "New Application" and give it a name ie. "polling-bot"
 3. Navigate to the Bot tab on the left side menu, and click "Add Bot" and confirm. 
 4. Under the TOKEN section, click "Copy" and copy the token.
 5. To add the bot to your Discord server, select the OAuth2 tab from the left side menu. From the SCOPES section, select bot option and from the BOT PERMISSIONS section, select Administrator. Copy and navigate to the generated URL and select the server you want to add the bot to from the dropdown, then click "Authorize."
 
 Next, install polling-bot with pip: `pip install polling-bot`.
 
-Navigate to the "polling-bot" directory and create a file called `.env` with the following content:
+Finally, to run the bot, import and run it as follows:
 
-`DISCORD_TOKEN={token}`, where token is the token copied from the Developer Portal above. 
+```python
 
-Finally, to run the bot, execute the command `python3 __main__.py`.
+import discord
+pollingbot = __import__("polling-bot")
+   
+bot = pollingbot.PollingBot(intents=discord.Intents.all(), command_prefix="/")
+bot.run('TOKEN')
+```
+
+Where token is the token copied from the Developer Portal above.
+
+The bot will now be responsive to commands in your Discord server. 
 
 ## Available Commands
 
 `/poll` - Starts a poll in the server
 
 `/add choice <content>` - Add choices to the poll
 
 `/edit <option> <content>` - Edit the content of the poll
 
-- Options are 'name', 'description', and 'choice'
+- Options are 'name', 'description', 'choice', and 'duration' (to alter how long the poll is open for [default is 5 mins])
 
 `/vote <choice #>` - Vote for a choice in the poll
 
 - Choice # is the # corresponding to the desired choice, viewable with `/view choices` or `/view poll`
 
 `/view <option>` - View the contents and results of the poll
 
 - Options are 'name', 'description', 'choices', 'poll', and 'results'
 
 ## Usage
 
-Start by executing `/poll` to create a poll. Edit the name and description of the poll using the `/edit` command. Next, add choices to the poll using the `/add` command. Have users then vote on the choices by running `/view poll` to see the current state of the poll, and then voting on their desired selection using the `/vote` command. Once all users have voted and the poll has concluded, run `/view results` to view the results and winner of the poll.
+Start by executing `/poll` to create a poll. Edit the name and description of the poll using the `/edit` command. Next, add choices to the poll using the `/add` command. Have users then vote on the choices by running `/view poll` to see the current state of the poll, and then voting on their desired selection using the `/vote` command. Once all users have voted and the poll has concluded, run `/view results` to view the results and winner of the poll.
+
+<img src="https://github.com/grnarayanan/polling-bot/blob/main/docs/source/demos/short-version.gif" width="350" title="Quick demo using polling-bot in a Discord server" alt="Quick demo using polling-bot in a Discord server">
```

### Comparing `polling-bot-0.1.0/polling_bot.egg-info/PKG-INFO` & `polling-bot-0.2.0/polling_bot.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: polling-bot
-Version: 0.1.0
+Version: 0.2.0
 Summary: polling-bot is a Discord bot to conduct basic polling functions in a Discord server
 Author-email: Ganesan Narayanan <ganesan.narayanan24@gmail.com>
 License: MIT License
         
         Copyright (c) 2023 Ganesan Narayanan
         
         Permission is hereby granted, free of charge, to any person obtaining a copy
@@ -43,23 +43,24 @@
 # polling-bot
 
 polling-bot is a Discord bot to conduct basic polling functions in a Discord server
 
 [![Build Status](https://github.com/grnarayanan/polling-bot/workflows/Build%20Status/badge.svg?branch=main)](https://github.com/grnarayanan/polling-bot/actions?query=workflow%3A%22Build+Status%22)
 [![codecov](https://codecov.io/gh/grnarayanan/polling-bot/branch/main/graph/badge.svg)](https://codecov.io/gh/grnarayanan/polling-bot)
 ![License](https://img.shields.io/github/license/grnarayanan/polling-bot.svg) ![GitHub issues](https://img.shields.io/github/issues/grnarayanan/polling-bot)
+[![PyPI](https://img.shields.io/pypi/v/polling-bot)](https://pypi.org/project/polling-bot/)
+[![Docs](https://img.shields.io/badge/docs-docs-green)](https://grnarayanan.github.io/polling-bot/)
 
 ## Overview
 
 Often times, reaching a consensus can be difficult without an organized method in place, and so this polling bot can be added to a Discord
 server to solve that need in a simple and efficient manner. Use cases could include deciding with friends on a place to eat, what video game 
 should be played, when to schedule a party, etc. 
 
-The bot supports starting a poll and adding options for choices by the users. It will then keep track of responses made to the poll,
-allow users to change their response, and surface the winner of the poll when called upon. 
+The bot supports starting a poll and adding options for choices by the users. It will then keep track of responses made to the poll, and surface the winner of the poll when called upon. 
 
 ## Details
 
 This project is a pure python project using modern tooling. It uses a `Makefile` as a command registry, with the following commands:
 - `make`: list available commands
 - `make develop`: install and build this library and its dependencies using `pip`
 - `make build`: build the library using `setuptools`
@@ -77,34 +78,45 @@
 2. Select "New Application" and give it a name ie. "polling-bot"
 3. Navigate to the Bot tab on the left side menu, and click "Add Bot" and confirm. 
 4. Under the TOKEN section, click "Copy" and copy the token.
 5. To add the bot to your Discord server, select the OAuth2 tab from the left side menu. From the SCOPES section, select bot option and from the BOT PERMISSIONS section, select Administrator. Copy and navigate to the generated URL and select the server you want to add the bot to from the dropdown, then click "Authorize."
 
 Next, install polling-bot with pip: `pip install polling-bot`.
 
-Navigate to the "polling-bot" directory and create a file called `.env` with the following content:
+Finally, to run the bot, import and run it as follows:
 
-`DISCORD_TOKEN={token}`, where token is the token copied from the Developer Portal above. 
+```python
 
-Finally, to run the bot, execute the command `python3 __main__.py`.
+import discord
+pollingbot = __import__("polling-bot")
+   
+bot = pollingbot.PollingBot(intents=discord.Intents.all(), command_prefix="/")
+bot.run('TOKEN')
+```
+
+Where token is the token copied from the Developer Portal above.
+
+The bot will now be responsive to commands in your Discord server. 
 
 ## Available Commands
 
 `/poll` - Starts a poll in the server
 
 `/add choice <content>` - Add choices to the poll
 
 `/edit <option> <content>` - Edit the content of the poll
 
-- Options are 'name', 'description', and 'choice'
+- Options are 'name', 'description', 'choice', and 'duration' (to alter how long the poll is open for [default is 5 mins])
 
 `/vote <choice #>` - Vote for a choice in the poll
 
 - Choice # is the # corresponding to the desired choice, viewable with `/view choices` or `/view poll`
 
 `/view <option>` - View the contents and results of the poll
 
 - Options are 'name', 'description', 'choices', 'poll', and 'results'
 
 ## Usage
 
 Start by executing `/poll` to create a poll. Edit the name and description of the poll using the `/edit` command. Next, add choices to the poll using the `/add` command. Have users then vote on the choices by running `/view poll` to see the current state of the poll, and then voting on their desired selection using the `/vote` command. Once all users have voted and the poll has concluded, run `/view results` to view the results and winner of the poll.
+
+<img src="https://github.com/grnarayanan/polling-bot/blob/main/docs/source/demos/short-version.gif" width="350" title="Quick demo using polling-bot in a Discord server" alt="Quick demo using polling-bot in a Discord server">
```

### Comparing `polling-bot-0.1.0/pyproject.toml` & `polling-bot-0.2.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -7,15 +7,15 @@
 build-backend="setuptools.build_meta"
 
 [project]
 name = "polling-bot"
 authors = [{name = "Ganesan Narayanan", email = "ganesan.narayanan24@gmail.com"}]
 description="polling-bot is a Discord bot to conduct basic polling functions in a Discord server"
 readme = "README.md"
-version="0.1.0"
+version="0.2.0"
 requires-python = ">=3.7"
 
 dependencies = [
         "discord.py",
         "python-dotenv",
 ]
```

