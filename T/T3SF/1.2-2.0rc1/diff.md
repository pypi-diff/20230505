# Comparing `tmp/T3SF-1.2.tar.gz` & `tmp/T3SF-2.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "T3SF-1.2.tar", last modified: Wed Apr  5 21:33:24 2023, max compression
+gzip compressed data, was "T3SF-2.0rc1.tar", last modified: Fri May  5 16:03:16 2023, max compression
```

## Comparing `T3SF-1.2.tar` & `T3SF-2.0rc1.tar`

### file list

```diff
@@ -1,33 +1,36 @@
-drwxrwxr-x   0 lanfran   (1000) lanfran   (1000)        0 2023-04-05 21:33:24.679086 T3SF-1.2/
--rw-r--r--   0 lanfran   (1000) lanfran   (1000)    35149 2022-04-20 14:58:09.000000 T3SF-1.2/LICENSE
--rw-rw-r--   0 lanfran   (1000) lanfran   (1000)       42 2023-04-05 17:28:50.000000 T3SF-1.2/MANIFEST.in
--rw-rw-r--   0 lanfran   (1000) lanfran   (1000)     4744 2023-04-05 21:33:24.679086 T3SF-1.2/PKG-INFO
--rw-rw-r--   0 lanfran   (1000) lanfran   (1000)     4093 2023-04-05 21:17:53.000000 T3SF-1.2/README.md
--rw-rw-r--   0 lanfran   (1000) lanfran   (1000)      103 2023-04-05 21:33:24.679086 T3SF-1.2/setup.cfg
--rw-rw-r--   0 lanfran   (1000) lanfran   (1000)     1124 2023-04-05 20:00:46.000000 T3SF-1.2/setup.py
-drwxrwxr-x   0 lanfran   (1000) lanfran   (1000)        0 2023-04-05 21:33:24.675086 T3SF-1.2/src/
-drwxrwxr-x   0 lanfran   (1000) lanfran   (1000)        0 2023-04-05 21:33:24.675086 T3SF-1.2/src/T3SF/
--rw-rw-r--   0 lanfran   (1000) lanfran   (1000)    14853 2023-04-05 19:52:43.000000 T3SF-1.2/src/T3SF/T3SF.py
--rw-rw-r--   0 lanfran   (1000) lanfran   (1000)       19 2023-03-15 19:12:31.000000 T3SF-1.2/src/T3SF/__init__.py
-drwxrwxr-x   0 lanfran   (1000) lanfran   (1000)        0 2023-04-05 21:33:24.679086 T3SF-1.2/src/T3SF/discord/
--rw-rw-r--   0 lanfran   (1000) lanfran   (1000)       47 2023-04-05 21:17:53.000000 T3SF-1.2/src/T3SF/discord/__init__.py
--rw-rw-r--   0 lanfran   (1000) lanfran   (1000)     2670 2023-04-05 21:17:53.000000 T3SF-1.2/src/T3SF/discord/bot.py
--rw-rw-r--   0 lanfran   (1000) lanfran   (1000)    10581 2023-04-05 21:17:53.000000 T3SF-1.2/src/T3SF/discord/discord.py
-drwxrwxr-x   0 lanfran   (1000) lanfran   (1000)        0 2023-04-05 21:33:24.679086 T3SF-1.2/src/T3SF/gui/
--rw-rw-r--   0 lanfran   (1000) lanfran   (1000)       19 2023-04-05 21:17:53.000000 T3SF-1.2/src/T3SF/gui/__init__.py
--rw-rw-r--   0 lanfran   (1000) lanfran   (1000)     1883 2023-04-05 21:17:53.000000 T3SF-1.2/src/T3SF/gui/core.py
-drwxrwxr-x   0 lanfran   (1000) lanfran   (1000)        0 2023-04-05 21:33:24.679086 T3SF-1.2/src/T3SF/gui/templates/
--rw-rw-r--   0 lanfran   (1000) lanfran   (1000)     5844 2023-04-05 21:17:53.000000 T3SF-1.2/src/T3SF/gui/templates/index.html
-drwxrwxr-x   0 lanfran   (1000) lanfran   (1000)        0 2023-04-05 21:33:24.679086 T3SF-1.2/src/T3SF/logger/
--rw-rw-r--   0 lanfran   (1000) lanfran   (1000)       21 2023-04-05 21:17:53.000000 T3SF-1.2/src/T3SF/logger/__init__.py
--rw-rw-r--   0 lanfran   (1000) lanfran   (1000)     1319 2023-04-05 21:17:53.000000 T3SF-1.2/src/T3SF/logger/logger.py
-drwxrwxr-x   0 lanfran   (1000) lanfran   (1000)        0 2023-04-05 21:33:24.679086 T3SF-1.2/src/T3SF/slack/
--rw-rw-r--   0 lanfran   (1000) lanfran   (1000)       43 2023-04-05 21:17:53.000000 T3SF-1.2/src/T3SF/slack/__init__.py
--rw-rw-r--   0 lanfran   (1000) lanfran   (1000)     2848 2023-04-05 21:17:53.000000 T3SF-1.2/src/T3SF/slack/bot.py
--rw-rw-r--   0 lanfran   (1000) lanfran   (1000)    16784 2023-04-05 21:17:53.000000 T3SF-1.2/src/T3SF/slack/slack.py
-drwxrwxr-x   0 lanfran   (1000) lanfran   (1000)        0 2023-04-05 21:33:24.675086 T3SF-1.2/src/T3SF.egg-info/
--rw-rw-r--   0 lanfran   (1000) lanfran   (1000)     4744 2023-04-05 21:33:24.000000 T3SF-1.2/src/T3SF.egg-info/PKG-INFO
--rw-rw-r--   0 lanfran   (1000) lanfran   (1000)      533 2023-04-05 21:33:24.000000 T3SF-1.2/src/T3SF.egg-info/SOURCES.txt
--rw-rw-r--   0 lanfran   (1000) lanfran   (1000)        1 2023-04-05 21:33:24.000000 T3SF-1.2/src/T3SF.egg-info/dependency_links.txt
--rw-rw-r--   0 lanfran   (1000) lanfran   (1000)       77 2023-04-05 21:33:24.000000 T3SF-1.2/src/T3SF.egg-info/requires.txt
--rw-rw-r--   0 lanfran   (1000) lanfran   (1000)        5 2023-04-05 21:33:24.000000 T3SF-1.2/src/T3SF.egg-info/top_level.txt
+drwxrwxr-x   0 lanfran   (1000) lanfran   (1000)        0 2023-05-05 16:03:16.035343 T3SF-2.0rc1/
+-rw-r--r--   0 lanfran   (1000) lanfran   (1000)    35149 2022-04-20 14:58:09.000000 T3SF-2.0rc1/LICENSE
+-rw-rw-r--   0 lanfran   (1000) lanfran   (1000)       42 2023-04-05 17:28:50.000000 T3SF-2.0rc1/MANIFEST.in
+-rw-rw-r--   0 lanfran   (1000) lanfran   (1000)     4748 2023-05-05 16:03:16.035343 T3SF-2.0rc1/PKG-INFO
+-rw-rw-r--   0 lanfran   (1000) lanfran   (1000)     4094 2023-04-26 15:27:46.000000 T3SF-2.0rc1/README.md
+-rw-rw-r--   0 lanfran   (1000) lanfran   (1000)      103 2023-05-05 16:03:16.035343 T3SF-2.0rc1/setup.cfg
+-rw-rw-r--   0 lanfran   (1000) lanfran   (1000)     1128 2023-05-05 16:03:02.000000 T3SF-2.0rc1/setup.py
+drwxrwxr-x   0 lanfran   (1000) lanfran   (1000)        0 2023-05-05 16:03:16.035343 T3SF-2.0rc1/src/
+drwxrwxr-x   0 lanfran   (1000) lanfran   (1000)        0 2023-05-05 16:03:16.035343 T3SF-2.0rc1/src/T3SF/
+-rw-rw-r--   0 lanfran   (1000) lanfran   (1000)    14899 2023-05-05 03:47:07.000000 T3SF-2.0rc1/src/T3SF/T3SF.py
+-rw-rw-r--   0 lanfran   (1000) lanfran   (1000)       19 2023-04-10 17:12:06.000000 T3SF-2.0rc1/src/T3SF/__init__.py
+drwxrwxr-x   0 lanfran   (1000) lanfran   (1000)        0 2023-05-05 16:03:16.035343 T3SF-2.0rc1/src/T3SF/discord/
+-rw-rw-r--   0 lanfran   (1000) lanfran   (1000)       47 2023-04-10 17:12:06.000000 T3SF-2.0rc1/src/T3SF/discord/__init__.py
+-rw-rw-r--   0 lanfran   (1000) lanfran   (1000)     6754 2023-05-05 03:50:40.000000 T3SF-2.0rc1/src/T3SF/discord/bot.py
+-rw-rw-r--   0 lanfran   (1000) lanfran   (1000)    10672 2023-05-05 03:58:00.000000 T3SF-2.0rc1/src/T3SF/discord/discord.py
+drwxrwxr-x   0 lanfran   (1000) lanfran   (1000)        0 2023-05-05 16:03:16.035343 T3SF-2.0rc1/src/T3SF/gui/
+-rw-rw-r--   0 lanfran   (1000) lanfran   (1000)       19 2023-04-10 17:12:06.000000 T3SF-2.0rc1/src/T3SF/gui/__init__.py
+-rw-rw-r--   0 lanfran   (1000) lanfran   (1000)     4252 2023-05-05 15:15:11.000000 T3SF-2.0rc1/src/T3SF/gui/core.py
+drwxrwxr-x   0 lanfran   (1000) lanfran   (1000)        0 2023-05-05 16:03:16.035343 T3SF-2.0rc1/src/T3SF/gui/templates/
+-rw-rw-r--   0 lanfran   (1000) lanfran   (1000)     4458 2023-04-19 14:36:52.000000 T3SF-2.0rc1/src/T3SF/gui/templates/base.html
+-rw-rw-r--   0 lanfran   (1000) lanfran   (1000)     5575 2023-04-19 15:52:23.000000 T3SF-2.0rc1/src/T3SF/gui/templates/env_creation.html
+-rw-rw-r--   0 lanfran   (1000) lanfran   (1000)     7809 2023-05-05 03:49:36.000000 T3SF-2.0rc1/src/T3SF/gui/templates/index.html
+-rw-rw-r--   0 lanfran   (1000) lanfran   (1000)     3603 2023-05-05 15:17:00.000000 T3SF-2.0rc1/src/T3SF/gui/templates/msel_viewer.html
+drwxrwxr-x   0 lanfran   (1000) lanfran   (1000)        0 2023-05-05 16:03:16.035343 T3SF-2.0rc1/src/T3SF/logger/
+-rw-rw-r--   0 lanfran   (1000) lanfran   (1000)       21 2023-04-10 17:12:06.000000 T3SF-2.0rc1/src/T3SF/logger/__init__.py
+-rw-rw-r--   0 lanfran   (1000) lanfran   (1000)     1452 2023-04-28 16:51:21.000000 T3SF-2.0rc1/src/T3SF/logger/logger.py
+drwxrwxr-x   0 lanfran   (1000) lanfran   (1000)        0 2023-05-05 16:03:16.035343 T3SF-2.0rc1/src/T3SF/slack/
+-rw-rw-r--   0 lanfran   (1000) lanfran   (1000)       43 2023-04-10 17:12:06.000000 T3SF-2.0rc1/src/T3SF/slack/__init__.py
+-rw-rw-r--   0 lanfran   (1000) lanfran   (1000)     6520 2023-05-05 15:14:14.000000 T3SF-2.0rc1/src/T3SF/slack/bot.py
+-rw-rw-r--   0 lanfran   (1000) lanfran   (1000)    16784 2023-04-27 16:18:20.000000 T3SF-2.0rc1/src/T3SF/slack/slack.py
+drwxrwxr-x   0 lanfran   (1000) lanfran   (1000)        0 2023-05-05 16:03:16.035343 T3SF-2.0rc1/src/T3SF.egg-info/
+-rw-rw-r--   0 lanfran   (1000) lanfran   (1000)     4748 2023-05-05 16:03:15.000000 T3SF-2.0rc1/src/T3SF.egg-info/PKG-INFO
+-rw-rw-r--   0 lanfran   (1000) lanfran   (1000)      647 2023-05-05 16:03:16.000000 T3SF-2.0rc1/src/T3SF.egg-info/SOURCES.txt
+-rw-rw-r--   0 lanfran   (1000) lanfran   (1000)        1 2023-05-05 16:03:15.000000 T3SF-2.0rc1/src/T3SF.egg-info/dependency_links.txt
+-rw-rw-r--   0 lanfran   (1000) lanfran   (1000)       77 2023-05-05 16:03:15.000000 T3SF-2.0rc1/src/T3SF.egg-info/requires.txt
+-rw-rw-r--   0 lanfran   (1000) lanfran   (1000)        5 2023-05-05 16:03:15.000000 T3SF-2.0rc1/src/T3SF.egg-info/top_level.txt
```

### Comparing `T3SF-1.2/LICENSE` & `T3SF-2.0rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `T3SF-1.2/PKG-INFO` & `T3SF-2.0rc1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: T3SF
-Version: 1.2
+Version: 2.0rc1
 Summary: Technical Tabletop Exercises Simulation Framework
 Home-page: https://github.com/Base4Security/T3SF
 Author: BASE4 Security
 Author-email: jlanfranconi@base4sec.com
 Project-URL: Bug Tracker, https://github.com/Base4Security/T3SF/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
@@ -49,15 +49,15 @@
 ## Getting Things Ready <a name = "Starting"></a>
 To use the framework with your desired platform, whether it's Slack or Discord, you will need to install the required modules for that platform. But don't worry, installing these modules is easy and straightforward.
 
 To do this, you can follow this simple step-by-step guide, or if you're already comfortable installing packages with `pip`, you can skip to the last step!
 
 ```bash
 # Python 3.6+ required
-python -m venv .venv       # We will create a python virtual enviroment
+python -m venv .venv       # We will create a python virtual environment
 source .venv/bin/activate  # Let's get inside it
 
 pip install -U pip         # Upgrade pip
 ```
 
 Once you have created a Python virtual environment and activated it, you can install the T3SF framework for your desired platform by running the following command:
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: T3SF Version: 1.2 Summary: Technical Tabletop
+Metadata-Version: 2.1 Name: T3SF Version: 2.0rc1 Summary: Technical Tabletop
 Exercises Simulation Framework Home-page: https://github.com/Base4Security/T3SF
 Author: BASE4 Security Author-email: jlanfranconi@base4sec.com Project-URL: Bug
 Tracker, https://github.com/Base4Security/T3SF/issues Classifier: Programming
 Language :: Python :: 3 Classifier: License :: OSI Approved :: GNU General
 Public License v3 (GPLv3) Classifier: Topic :: Software Development ::
 Libraries :: Application Frameworks Classifier: Operating System :: OS
 Independent Description-Content-Type: text/markdown Provides-Extra: Slack
@@ -30,19 +30,19 @@
 organization, single area" and "multiple organization, multiple areas". ##
 Getting Things Ready  To use the framework with your desired platform, whether
 it's Slack or Discord, you will need to install the required modules for that
 platform. But don't worry, installing these modules is easy and
 straightforward. To do this, you can follow this simple step-by-step guide, or
 if you're already comfortable installing packages with `pip`, you can skip to
 the last step! ```bash # Python 3.6+ required python -m venv .venv # We will
-create a python virtual enviroment source .venv/bin/activate # Let's get inside
-it pip install -U pip # Upgrade pip ``` Once you have created a Python virtual
-environment and activated it, you can install the T3SF framework for your
-desired platform by running the following command: ```bash pip install "T3SF
-[Discord]" # Install the framework to work with Discord ``` or ```bash pip
+create a python virtual environment source .venv/bin/activate # Let's get
+inside it pip install -U pip # Upgrade pip ``` Once you have created a Python
+virtual environment and activated it, you can install the T3SF framework for
+your desired platform by running the following command: ```bash pip install
+"T3SF[Discord]" # Install the framework to work with Discord ``` or ```bash pip
 install "T3SF[Slack]" # Install the framework to work with Slack ``` This will
 install the T3SF framework along with the required dependencies for your chosen
 platform. Once the installation is complete, you can start using the framework
 with your platform of choice. We strongly recommend following the platform-
 specific guidance within our Read The Docs! Here are the links: - [Discord]
 (https://t3sf.readthedocs.io/en/latest/Discord.html#installation) - [Slack]
 (https://t3sf.readthedocs.io/en/latest/Slack.html#installation) - [Telegram]
```

### Comparing `T3SF-1.2/README.md` & `T3SF-2.0rc1/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -32,15 +32,15 @@
 ## Getting Things Ready <a name = "Starting"></a>
 To use the framework with your desired platform, whether it's Slack or Discord, you will need to install the required modules for that platform. But don't worry, installing these modules is easy and straightforward.
 
 To do this, you can follow this simple step-by-step guide, or if you're already comfortable installing packages with `pip`, you can skip to the last step!
 
 ```bash
 # Python 3.6+ required
-python -m venv .venv       # We will create a python virtual enviroment
+python -m venv .venv       # We will create a python virtual environment
 source .venv/bin/activate  # Let's get inside it
 
 pip install -U pip         # Upgrade pip
 ```
 
 Once you have created a Python virtual environment and activated it, you can install the T3SF framework for your desired platform by running the following command:
```

### Comparing `T3SF-1.2/setup.py` & `T3SF-2.0rc1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="T3SF",
-    version="1.2",
+    version="2.0-rc1",
     author="BASE4 Security",
     author_email="jlanfranconi@base4sec.com",
     description="Technical Tabletop Exercises Simulation Framework",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/Base4Security/T3SF",
     project_urls={
```

### Comparing `T3SF-1.2/src/T3SF/T3SF.py` & `T3SF-2.0rc1/src/T3SF/T3SF.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,14 +25,15 @@
 		self.process_quit = False
 		self.regex_ready = None
 		self.incidents_running = False
 		self.poll_answered = False
 		self.ch_names_list = []
 		self.players_list = []
 		self.platform = platform.lower()
+		self.guild_id = None
 
 		try:
 			if os.path.isfile(os.getcwd() + f"/inboxes_{self.platform}.json"):
 				self.inboxes_all = json.load(open(f"inboxes_{self.platform}.json", encoding='utf-8-sig'))
 				self.fetch_inboxes = False
 
 				T3SF_Logger.emit(message="Locally retrieved Inboxes", message_type="DEBUG")
@@ -99,25 +100,24 @@
 			self.data = json.load(open(MSEL, encoding='utf-8-sig'))
 
 			for inject in self.data:
 				player = inject['Player']
 				if player not in self.players_list:
 					self.players_list.append(player)
 			T3SF_Logger.emit(message="We have the inboxes right now", message_type="DEBUG")
-			return True
+			T3SF_Logger.emit(message="Incidents ready", message_type="DEBUG")
+			return self.players_list
 		else:
 			raise RuntimeError("Please set a method to retrieve the TTXs with the argument `MSEL` inside the `start` function.")
 
-		T3SF_Logger.emit(message="Incidents ready", message_type="DEBUG")
-
 	async def start(MSEL:str, platform, gui=False):
 		if gui == True:
 			T3SF_Logger.emit(message="Starting GUI", message_type="DEBUG")
 			gui_module = importlib.import_module("T3SF.gui.core")
-			gui_module.GUI(platform_run=platform)
+			gui_module.GUI(platform_run=platform, MSEL=MSEL)
 		
 		if platform.lower() == "slack":
 			bot_module = importlib.import_module("T3SF.slack.bot")
 
 		elif platform.lower() == "discord":
 			bot_module = importlib.import_module("T3SF.discord.bot")
 
@@ -368,15 +368,14 @@
 				self.response = await self.discord.SendMessage(T3SF_instance=self, color=color, title=title, description=description, view=view)
 				return self.response
 
 		elif self.platform == "slack":
 			self.response = await Slack.SendMessage(self=self.slack, channel = channel, title=title, description=description, color=color, image=image, author=author, buttons=buttons, text_input=text_input, checkboxes=checkboxes)
 			return self.response
 
-
 	async def EditMessage(self,
 		color=None, 
 		style:str="simple", 
 		title:str=None, 
 		description:str=None,
 		response=None, 
 		variable=None,
```

### Comparing `T3SF-1.2/src/T3SF/discord/discord.py` & `T3SF-2.0rc1/src/T3SF/discord/discord.py`

 * *Files 1% similar despite different names*

```diff
@@ -12,15 +12,17 @@
 
 		async def InboxesAuto(self, T3SF_instance):
 			mensaje_inboxes = ""
 			image_example = "https://i.ibb.co/NCrPD3Y/discord-exp.png"
 
 			if T3SF_instance.fetch_inboxes == True:
 				if T3SF_instance._ctx == None:
-					channels = self.bot.get_all_channels()
+					# Exercise started from the GUI
+					guild = self.bot.get_guild(int(T3SF_instance.guild_id))
+					channels = guild.text_channels
 
 					for channel in channels:
 						if "chat" in channel.name:
 							accuracy = similar(str(channel.name).lower(),"gm-chat")
 							if accuracy >= 0.8:
 								inbox = channel.id
 								T3SF_instance._ctx = self.bot.get_channel(channel.id)
@@ -31,14 +33,15 @@
 				player_itinerator = 0
 				regex = ""
 
 				try:
 					channels = T3SF_instance._ctx.message.guild.channels
 					categories = T3SF_instance._ctx.message.guild.categories
 					started_from_gui = False
+
 				except Exception:
 					channels = T3SF_instance._ctx.guild.channels
 					categories = T3SF_instance._ctx.guild.categories
 					started_from_gui = True
 
 				while regex == "" and len(T3SF_instance.players_list) > player_itinerator:
 					for category in categories:
```

### Comparing `T3SF-1.2/src/T3SF/gui/templates/index.html` & `T3SF-2.0rc1/src/T3SF/gui/templates/env_creation.html`

 * *Files 24% similar despite different names*

```diff
@@ -1,366 +1,349 @@
-00000000: 3c21 444f 4354 5950 4520 6874 6d6c 3e0a  <!DOCTYPE html>.
-00000010: 3c68 746d 6c3e 0a3c 6865 6164 3e0a 093c  <html>.<head>..<
-00000020: 7469 746c 653e 5433 5346 202d 2047 5549  title>T3SF - GUI
-00000030: 3c2f 7469 746c 653e 0a09 3c6c 696e 6b20  </title>..<link 
-00000040: 7265 6c3d 2269 636f 6e22 2074 7970 653d  rel="icon" type=
-00000050: 2269 6d61 6765 2f78 2d69 636f 6e22 2068  "image/x-icon" h
-00000060: 7265 663d 2268 7474 7073 3a2f 2f75 7365  ref="https://use
-00000070: 722d 696d 6167 6573 2e67 6974 6875 6275  r-images.githubu
-00000080: 7365 7263 6f6e 7465 6e74 2e63 6f6d 2f31  sercontent.com/1
-00000090: 3033 3132 3431 3537 2f31 3634 3235 3839  03124157/1642589
-000000a0: 3636 2d37 6130 3439 6436 632d 3430 3132  66-7a049d6c-4012
-000000b0: 2d34 3963 612d 3866 3764 2d32 6262 3831  -49ca-8f7d-2bb81
-000000c0: 3463 3234 3030 392e 706e 6722 3e0a 0a09  4c24009.png">...
-000000d0: 3c73 6372 6970 7420 7372 633d 222f 2f63  <script src="//c
-000000e0: 646e 6a73 2e63 6c6f 7564 666c 6172 652e  dnjs.cloudflare.
-000000f0: 636f 6d2f 616a 6178 2f6c 6962 732f 6a71  com/ajax/libs/jq
-00000100: 7565 7279 2f33 2e36 2e33 2f6a 7175 6572  uery/3.6.3/jquer
-00000110: 792e 6d69 6e2e 6a73 223e 3c2f 7363 7269  y.min.js"></scri
-00000120: 7074 3e0a 0a09 3c6c 696e 6b20 6872 6566  pt>...<link href
-00000130: 3d22 6874 7470 733a 2f2f 6364 6e2e 6a73  ="https://cdn.js
-00000140: 6465 6c69 7672 2e6e 6574 2f6e 706d 2f62  delivr.net/npm/b
-00000150: 6f6f 7473 7472 6170 4035 2e33 2e30 2d61  ootstrap@5.3.0-a
-00000160: 6c70 6861 312f 6469 7374 2f63 7373 2f62  lpha1/dist/css/b
-00000170: 6f6f 7473 7472 6170 2e6d 696e 2e63 7373  ootstrap.min.css
-00000180: 2220 7265 6c3d 2273 7479 6c65 7368 6565  " rel="styleshee
-00000190: 7422 2069 6e74 6567 7269 7479 3d22 7368  t" integrity="sh
-000001a0: 6133 3834 2d47 4c68 6c54 5138 6952 4142  a384-GLhlTQ8iRAB
-000001b0: 645a 4c6c 364f 336f 564d 5753 6b74 514f  dZLl6O3oVMWSktQO
-000001c0: 7036 6237 496e 315a 6c33 2f4a 7235 3962  p6b7In1Zl3/Jr59b
-000001d0: 3645 4747 6f49 3161 466b 7737 636d 4441  6EGGoI1aFkw7cmDA
-000001e0: 366a 3667 4422 2063 726f 7373 6f72 6967  6j6gD" crossorig
-000001f0: 696e 3d22 616e 6f6e 796d 6f75 7322 3e0a  in="anonymous">.
-00000200: 090a 093c 7363 7269 7074 2073 7263 3d22  ...<script src="
-00000210: 6874 7470 733a 2f2f 6364 6e2e 6a73 6465  https://cdn.jsde
-00000220: 6c69 7672 2e6e 6574 2f6e 706d 2f62 6f6f  livr.net/npm/boo
-00000230: 7473 7472 6170 4035 2e33 2e30 2d61 6c70  tstrap@5.3.0-alp
-00000240: 6861 312f 6469 7374 2f6a 732f 626f 6f74  ha1/dist/js/boot
-00000250: 7374 7261 702e 6275 6e64 6c65 2e6d 696e  strap.bundle.min
-00000260: 2e6a 7322 2069 6e74 6567 7269 7479 3d22  .js" integrity="
-00000270: 7368 6133 3834 2d77 3736 4171 5066 446b  sha384-w76AqPfDk
-00000280: 4d42 4458 6f33 306a 5331 5367 657a 3670  MBDXo30jS1Sgez6p
-00000290: 7233 7835 4d6c 5131 5a41 4743 2b6e 755a  r3x5MlQ1ZAGC+nuZ
-000002a0: 422b 4559 6467 525a 6769 7778 6854 4254  B+EYdgRZgiwxhTBT
-000002b0: 6b46 3743 5876 4e22 2063 726f 7373 6f72  kF7CXvN" crossor
-000002c0: 6967 696e 3d22 616e 6f6e 796d 6f75 7322  igin="anonymous"
-000002d0: 3e3c 2f73 6372 6970 743e 0a0a 0a09 3c73  ></script>....<s
-000002e0: 7479 6c65 2074 7970 653d 2274 6578 742f  tyle type="text/
-000002f0: 6373 7322 3e0a 0909 236c 6f67 732d 636f  css">...#logs-co
-00000300: 6e74 656e 7420 7b0a 0909 0968 6569 6768  ntent {....heigh
-00000310: 743a 2035 3030 7078 3b0a 0909 096f 7665  t: 500px;....ove
-00000320: 7266 6c6f 773a 2061 7574 6f3b 0a09 0909  rflow: auto;....
-00000330: 7768 6974 652d 7370 6163 653a 2070 7265  white-space: pre
-00000340: 2d77 7261 703b 0a09 0909 666c 6578 2d67  -wrap;....flex-g
-00000350: 726f 773a 2031 3b0a 0909 7d0a 0909 406d  row: 1;...}...@m
-00000360: 6564 6961 2028 6d61 782d 7769 6474 683a  edia (max-width:
-00000370: 2039 3931 7078 2920 7b0a 0909 0968 746d   991px) {....htm
-00000380: 6c2c 2062 6f64 792c 2023 6c6f 6773 2d63  l, body, #logs-c
-00000390: 6f6e 7465 6e74 207b 0a09 0909 0968 6569  ontent {.....hei
-000003a0: 6768 743a 2031 3030 253b 0a09 0909 0977  ght: 100%;.....w
-000003b0: 6964 7468 3a20 3130 3025 3b0a 0909 0909  idth: 100%;.....
-000003c0: 6d61 782d 7769 6474 683a 206e 6f6e 653b  max-width: none;
-000003d0: 0a09 0909 7d0a 0a09 0909 236c 6f67 732d  ....}.....#logs-
-000003e0: 636f 6e74 656e 7420 7b0a 0909 0909 6d61  content {.....ma
-000003f0: 7267 696e 2d74 6f70 3a20 303b 0a09 0909  rgin-top: 0;....
-00000400: 7d0a 0909 7d0a 0a09 092e 6c6f 672d 7479  }...}.....log-ty
-00000410: 7065 2d44 4542 5547 207b 0a09 0909 666c  pe-DEBUG {....fl
-00000420: 6f61 743a 206c 6566 743b 0a09 0909 636f  oat: left;....co
-00000430: 6c6f 723a 2062 6c75 653b 0a09 097d 0a09  lor: blue;...}..
-00000440: 092e 6c6f 672d 7479 7065 2d49 4e46 4f20  ..log-type-INFO 
-00000450: 7b0a 0909 0966 6c6f 6174 3a20 6c65 6674  {....float: left
-00000460: 3b0a 0909 0963 6f6c 6f72 3a20 6772 6565  ;....color: gree
-00000470: 6e3b 0a09 097d 0a09 092e 6c6f 672d 7479  n;...}....log-ty
-00000480: 7065 2d57 4152 4e20 7b0a 0909 0966 6c6f  pe-WARN {....flo
-00000490: 6174 3a20 6c65 6674 3b0a 0909 0963 6f6c  at: left;....col
-000004a0: 6f72 3a20 2346 4643 3130 373b 0a09 097d  or: #FFC107;...}
-000004b0: 0a09 092e 6c6f 672d 7479 7065 2d45 5252  ....log-type-ERR
-000004c0: 4f52 207b 0a09 0909 666c 6f61 743a 206c  OR {....float: l
-000004d0: 6566 743b 0a09 0909 636f 6c6f 723a 2072  eft;....color: r
-000004e0: 6564 3b0a 0909 7d0a 0a09 092e 6c6f 672d  ed;...}.....log-
-000004f0: 7469 6d65 7374 616d 7020 7b0a 0909 0966  timestamp {....f
-00000500: 6f6e 742d 7369 7a65 3a20 3132 7078 3b0a  ont-size: 12px;.
-00000510: 0909 0963 6f6c 6f72 3a20 6772 6179 3b0a  ...color: gray;.
-00000520: 0909 0966 6c6f 6174 3a20 7269 6768 743b  ...float: right;
-00000530: 0a09 097d 0a0a 0909 236c 6f67 732d 6c65  ...}....#logs-le
-00000540: 7665 6c2d 6472 6f70 646f 776e 207b 0a09  vel-dropdown {..
-00000550: 0909 626f 7264 6572 3a20 3170 7820 736f  ..border: 1px so
-00000560: 6c69 6420 2363 6363 3b0a 0909 0962 6f72  lid #ccc;....bor
-00000570: 6465 722d 7261 6469 7573 3a20 3470 783b  der-radius: 4px;
-00000580: 0a09 0909 7061 6464 696e 673a 2034 7078  ....padding: 4px
-00000590: 2038 7078 3b0a 0909 0966 6f6e 742d 7369   8px;....font-si
-000005a0: 7a65 3a20 3136 7078 3b0a 0909 0966 6f6e  ze: 16px;....fon
-000005b0: 742d 6661 6d69 6c79 3a20 4172 6961 6c2c  t-family: Arial,
-000005c0: 2073 616e 732d 7365 7269 663b 0a09 0909   sans-serif;....
-000005d0: 636f 6c6f 723a 2023 3333 333b 0a09 0909  color: #333;....
-000005e0: 6261 636b 6772 6f75 6e64 2d63 6f6c 6f72  background-color
-000005f0: 3a20 2366 6666 3b0a 0909 0962 6f78 2d73  : #fff;....box-s
-00000600: 6861 646f 773a 2069 6e73 6574 2030 2031  hadow: inset 0 1
-00000610: 7078 2033 7078 2072 6762 6128 302c 2030  px 3px rgba(0, 0
-00000620: 2c20 302c 2030 2e31 293b 0a09 0909 7472  , 0, 0.1);....tr
-00000630: 616e 7369 7469 6f6e 3a20 626f 7264 6572  ansition: border
-00000640: 2d63 6f6c 6f72 2030 2e32 7320 6561 7365  -color 0.2s ease
-00000650: 2d69 6e2d 6f75 742c 2062 6f78 2d73 6861  -in-out, box-sha
-00000660: 646f 7720 302e 3273 2065 6173 652d 696e  dow 0.2s ease-in
-00000670: 2d6f 7574 3b0a 0909 7d0a 0a09 0923 6c6f  -out;...}....#lo
-00000680: 6773 2d6c 6576 656c 2d64 726f 7064 6f77  gs-level-dropdow
-00000690: 6e3a 666f 6375 7320 7b0a 0909 096f 7574  n:focus {....out
-000006a0: 6c69 6e65 3a20 6e6f 6e65 3b0a 0909 0962  line: none;....b
-000006b0: 6f72 6465 722d 636f 6c6f 723a 2023 3030  order-color: #00
-000006c0: 3762 6666 3b0a 0909 0962 6f78 2d73 6861  7bff;....box-sha
-000006d0: 646f 773a 2069 6e73 6574 2030 2031 7078  dow: inset 0 1px
-000006e0: 2033 7078 2072 6762 6128 302c 2030 2c20   3px rgba(0, 0, 
-000006f0: 302c 2030 2e31 292c 2030 2030 2030 2032  0, 0.1), 0 0 0 2
-00000700: 7078 2072 6762 6128 302c 2031 3233 2c20  px rgba(0, 123, 
-00000710: 3235 352c 2030 2e35 293b 0a09 097d 0a0a  255, 0.5);...}..
-00000720: 0909 236c 6f67 732d 6c65 7665 6c2d 666f  ..#logs-level-fo
-00000730: 726d 206c 6162 656c 207b 0a09 0909 666f  rm label {....fo
-00000740: 6e74 2d73 697a 653a 2031 3670 783b 0a09  nt-size: 16px;..
-00000750: 0909 666f 6e74 2d66 616d 696c 793a 2041  ..font-family: A
-00000760: 7269 616c 2c20 7361 6e73 2d73 6572 6966  rial, sans-serif
-00000770: 3b0a 0909 0966 6f6e 742d 7765 6967 6874  ;....font-weight
-00000780: 3a20 626f 6c64 3b0a 0909 096d 6172 6769  : bold;....margi
-00000790: 6e2d 7269 6768 743a 2038 7078 3b0a 0909  n-right: 8px;...
-000007a0: 0963 6f6c 6f72 3a20 2333 3333 3b0a 0909  .color: #333;...
-000007b0: 7d0a 0a0a 0909 236c 6f67 732d 6c65 7665  }.....#logs-leve
-000007c0: 6c2d 666f 726d 2d63 6f6e 7461 696e 6572  l-form-container
-000007d0: 207b 0a09 0920 2064 6973 706c 6179 3a20   {...  display: 
-000007e0: 696e 6c69 6e65 2d62 6c6f 636b 3b0a 0909  inline-block;...
-000007f0: 7d0a 0a09 0923 6c6f 6773 2d6c 6576 656c  }....#logs-level
-00000800: 2d66 6f72 6d2c 0a09 0923 6c6f 6773 2d6c  -form,...#logs-l
-00000810: 6576 656c 2d64 726f 7064 6f77 6e20 7b0a  evel-dropdown {.
-00000820: 0909 2020 6469 7370 6c61 793a 2069 6e6c  ..  display: inl
-00000830: 696e 652d 626c 6f63 6b3b 0a09 097d 0a09  ine-block;...}..
-00000840: 3c2f 7374 796c 653e 0a3c 2f68 6561 643e  </style>.</head>
-00000850: 0a0a 3c62 6f64 793e 0a09 3c64 6976 2063  ..<body>..<div c
-00000860: 6c61 7373 3d22 636f 6e74 6169 6e65 7222  lass="container"
-00000870: 3e0a 0909 3c64 6976 2063 6c61 7373 3d22  >...<div class="
-00000880: 702d 3520 6d62 2d34 2062 672d 6c69 6768  p-5 mb-4 bg-ligh
-00000890: 7420 726f 756e 6465 642d 3322 3e0a 0909  t rounded-3">...
-000008a0: 093c 6831 2063 6c61 7373 3d22 6469 7370  .<h1 class="disp
-000008b0: 6c61 792d 3520 6677 2d62 6f6c 6422 3e54  lay-5 fw-bold">T
-000008c0: 3353 4620 2d20 4d61 6e61 6765 6d65 6e74  3SF - Management
-000008d0: 2047 5549 3c2f 6831 3e0a 0909 093c 7020   GUI</h1>....<p 
-000008e0: 636c 6173 733d 2263 6f6c 2d6d 642d 3820  class="col-md-8 
-000008f0: 6673 2d34 223e 5669 6577 2061 6e64 2063  fs-4">View and c
-00000900: 6f6e 7472 6f6c 2074 6865 2073 7461 7475  ontrol the statu
-00000910: 7320 6f66 2074 6865 2065 7865 7263 6973  s of the exercis
-00000920: 652e 3c2f 703e 0a09 093c 2f64 6976 3e0a  e.</p>...</div>.
-00000930: 093c 2f64 6976 3e0a 090a 3c2f 6469 763e  .</div>...</div>
-00000940: 0a3c 6469 7620 636c 6173 733d 2263 6f6e  .<div class="con
-00000950: 7461 696e 6572 2220 6964 3d22 636f 6e74  tainer" id="cont
-00000960: 656e 7422 3e0a 2020 3c64 6976 2063 6c61  ent">.  <div cla
-00000970: 7373 3d22 726f 7720 616c 6967 6e2d 6974  ss="row align-it
-00000980: 656d 732d 6365 6e74 6572 223e 0a20 2020  ems-center">.   
-00000990: 203c 6469 7620 636c 6173 733d 2263 6f6c   <div class="col
-000009a0: 223e 0a20 2020 2020 203c 6833 3e4c 6f67  ">.      <h3>Log
-000009b0: 733a 3c2f 6833 3e0a 2020 2020 3c2f 6469  s:</h3>.    </di
-000009c0: 763e 0a20 2020 203c 6469 7620 636c 6173  v>.    <div clas
-000009d0: 733d 2263 6f6c 2d61 7574 6f22 3e0a 2020  s="col-auto">.  
-000009e0: 2020 2020 3c66 6f72 6d20 6964 3d22 6c6f      <form id="lo
-000009f0: 6773 2d6c 6576 656c 2d66 6f72 6d22 3e0a  gs-level-form">.
-00000a00: 2020 2020 2020 2020 3c6c 6162 656c 2066          <label f
-00000a10: 6f72 3d22 6c6f 6773 2d6c 6576 656c 2d64  or="logs-level-d
-00000a20: 726f 7064 6f77 6e22 3e53 6574 204c 6f67  ropdown">Set Log
-00000a30: 203c 6162 6272 2074 6974 6c65 3d22 4561   <abbr title="Ea
-00000a40: 6368 206c 6f67 206c 6576 656c 2069 6e63  ch log level inc
-00000a50: 6c75 6465 7320 616c 6c20 6c65 7665 6c73  ludes all levels
-00000a60: 2061 626f 7665 2069 742e 223e 4c65 7665   above it.">Leve
-00000a70: 6c3c 2f61 6262 723e 3a3c 2f6c 6162 656c  l</abbr>:</label
-00000a80: 3e0a 2020 2020 2020 2020 3c73 656c 6563  >.        <selec
-00000a90: 7420 6964 3d22 6c6f 6773 2d6c 6576 656c  t id="logs-level
-00000aa0: 2d64 726f 7064 6f77 6e22 206e 616d 653d  -dropdown" name=
-00000ab0: 226c 6f67 732d 6c65 7665 6c2d 6472 6f70  "logs-level-drop
-00000ac0: 646f 776e 223e 0a20 2020 2020 2020 2020  down">.         
-00000ad0: 203c 6f70 7469 6f6e 2076 616c 7565 3d22   <option value="
-00000ae0: 4445 4255 4722 3e44 6562 7567 3c2f 6f70  DEBUG">Debug</op
-00000af0: 7469 6f6e 3e0a 2020 2020 2020 2020 2020  tion>.          
-00000b00: 3c6f 7074 696f 6e20 7661 6c75 653d 2249  <option value="I
-00000b10: 4e46 4f22 3e49 6e66 6f3c 2f6f 7074 696f  NFO">Info</optio
-00000b20: 6e3e 0a20 2020 2020 2020 2020 203c 6f70  n>.          <op
-00000b30: 7469 6f6e 2076 616c 7565 3d22 5741 524e  tion value="WARN
-00000b40: 223e 5761 726e 3c2f 6f70 7469 6f6e 3e0a  ">Warn</option>.
-00000b50: 2020 2020 2020 2020 2020 3c6f 7074 696f            <optio
-00000b60: 6e20 7661 6c75 653d 2245 5252 4f52 223e  n value="ERROR">
-00000b70: 4572 726f 723c 2f6f 7074 696f 6e3e 0a20  Error</option>. 
-00000b80: 2020 2020 2020 203c 2f73 656c 6563 743e         </select>
-00000b90: 0a20 2020 2020 203c 2f66 6f72 6d3e 0a20  .      </form>. 
-00000ba0: 2020 203c 2f64 6976 3e0a 2020 2020 3c64     </div>.    <d
-00000bb0: 6976 2063 6c61 7373 3d22 636f 6c2d 6175  iv class="col-au
-00000bc0: 746f 223e 0a20 2020 2020 203c 6275 7474  to">.      <butt
-00000bd0: 6f6e 2069 643d 2273 7461 7274 2d62 7574  on id="start-but
-00000be0: 746f 6e22 2063 6c61 7373 3d22 6274 6e20  ton" class="btn 
-00000bf0: 6274 6e2d 7375 6363 6573 7322 3e53 7461  btn-success">Sta
-00000c00: 7274 3c2f 6275 7474 6f6e 3e0a 2020 2020  rt</button>.    
-00000c10: 2020 3c62 7574 746f 6e20 6964 3d22 7374    <button id="st
-00000c20: 6f70 2d62 7574 746f 6e22 2063 6c61 7373  op-button" class
-00000c30: 3d22 6274 6e20 6274 6e2d 6461 6e67 6572  ="btn btn-danger
-00000c40: 223e 5374 6f70 3c2f 6275 7474 6f6e 3e0a  ">Stop</button>.
-00000c50: 2020 2020 2020 3c62 7574 746f 6e20 6964        <button id
-00000c60: 3d22 636c 6561 722d 6275 7474 6f6e 2220  ="clear-button" 
-00000c70: 636c 6173 733d 2262 746e 2062 746e 2d77  class="btn btn-w
-00000c80: 6172 6e69 6e67 223e 436c 6561 7220 4c6f  arning">Clear Lo
-00000c90: 6773 3c2f 6275 7474 6f6e 3e0a 2020 2020  gs</button>.    
-00000ca0: 3c2f 6469 763e 0a20 203c 2f64 6976 3e0a  </div>.  </div>.
-00000cb0: 2020 3c64 6976 2063 6c61 7373 3d22 726f    <div class="ro
-00000cc0: 7722 3e0a 2020 2020 3c64 6976 2063 6c61  w">.    <div cla
-00000cd0: 7373 3d22 636f 6c22 3e0a 2020 2020 2020  ss="col">.      
-00000ce0: 3c64 6976 2063 6c61 7373 3d22 6267 2d6c  <div class="bg-l
-00000cf0: 6967 6874 2072 6f75 6e64 6564 2070 2d33  ight rounded p-3
-00000d00: 2220 6964 3d22 6c6f 6773 2d63 6f6e 7465  " id="logs-conte
-00000d10: 6e74 223e 0a20 2020 2020 203c 2f64 6976  nt">.      </div
-00000d20: 3e0a 2020 2020 3c2f 6469 763e 0a20 203c  >.    </div>.  <
-00000d30: 2f64 6976 3e0a 3c2f 6469 763e 0a0a 3c73  /div>.</div>..<s
-00000d40: 6372 6970 743e 0a09 2f2f 2044 6566 696e  cript>..// Defin
-00000d50: 6520 7468 6520 6c6f 6720 6c65 7665 6c73  e the log levels
-00000d60: 2061 6e64 2074 6865 6972 2063 6f72 7265   and their corre
-00000d70: 7370 6f6e 6469 6e67 2066 696c 7465 7269  sponding filteri
-00000d80: 6e67 2063 6f6e 6469 7469 6f6e 730a 0963  ng conditions..c
-00000d90: 6f6e 7374 206c 6f67 4c65 7665 6c73 203d  onst logLevels =
-00000da0: 207b 0a09 0927 4445 4255 4727 3a20 095b   {...'DEBUG': .[
-00000db0: 2744 4542 5547 272c 2027 494e 464f 272c  'DEBUG', 'INFO',
-00000dc0: 2027 5741 524e 272c 2027 4552 524f 5227   'WARN', 'ERROR'
-00000dd0: 5d2c 0a09 0927 494e 464f 273a 2009 5b27  ],...'INFO': .['
-00000de0: 494e 464f 272c 2027 5741 524e 272c 2027  INFO', 'WARN', '
-00000df0: 4552 524f 5227 5d2c 0a09 0927 5741 524e  ERROR'],...'WARN
-00000e00: 273a 2009 5b27 5741 524e 272c 2027 4552  ': .['WARN', 'ER
-00000e10: 524f 5227 5d2c 0a09 0927 4552 524f 5227  ROR'],...'ERROR'
-00000e20: 3a20 095b 2745 5252 4f52 275d 0a09 7d3b  : .['ERROR']..};
-00000e30: 0a0a 0976 6172 2068 6973 746f 7269 635f  ...var historic_
-00000e40: 6c6f 6773 203d 205b 5d3b 0a09 7661 7220  logs = [];..var 
-00000e50: 6576 656e 7453 6f75 7263 6520 3d20 6e65  eventSource = ne
-00000e60: 7720 4576 656e 7453 6f75 7263 6528 272f  w EventSource('/
-00000e70: 7374 7265 616d 2729 3b0a 0a09 6576 656e  stream');...even
-00000e80: 7453 6f75 7263 652e 6f6e 6d65 7373 6167  tSource.onmessag
-00000e90: 6520 3d20 6675 6e63 7469 6f6e 2865 7665  e = function(eve
-00000ea0: 6e74 2920 7b0a 0909 7661 7220 6d65 7373  nt) {...var mess
-00000eb0: 6167 6520 3d20 4a53 4f4e 2e70 6172 7365  age = JSON.parse
-00000ec0: 2865 7665 6e74 2e64 6174 6129 3b0a 0909  (event.data);...
-00000ed0: 7661 7220 6d65 7373 6167 6549 6420 3d20  var messageId = 
-00000ee0: 6d65 7373 6167 652e 6964 3b0a 0a09 2020  message.id;...  
-00000ef0: 2f2f 2047 6574 2074 6865 2073 656c 6563  // Get the selec
-00000f00: 7465 6420 6c6f 6720 6c65 7665 6c0a 0909  ted log level...
-00000f10: 7661 7220 6c6f 674c 6576 656c 203d 2024  var logLevel = $
-00000f20: 2827 236c 6f67 732d 6c65 7665 6c2d 6472  ('#logs-level-dr
-00000f30: 6f70 646f 776e 2729 2e76 616c 2829 3b0a  opdown').val();.
-00000f40: 0909 7661 7220 6c6f 674c 6576 656c 5f73  ..var logLevel_s
-00000f50: 746f 7265 6420 3d20 6c6f 6361 6c53 746f  tored = localSto
-00000f60: 7261 6765 2e67 6574 4974 656d 2822 6c6f  rage.getItem("lo
-00000f70: 675f 6c65 7665 6c22 293b 0a0a 0909 6966  g_level");....if
-00000f80: 2028 6c6f 674c 6576 656c 2021 3d3d 206c   (logLevel !== l
-00000f90: 6f67 4c65 7665 6c5f 7374 6f72 6564 2920  ogLevel_stored) 
-00000fa0: 7b0a 0909 0924 2822 236c 6f67 732d 6c65  {....$("#logs-le
-00000fb0: 7665 6c2d 6472 6f70 646f 776e 2229 2e76  vel-dropdown").v
-00000fc0: 616c 286c 6f67 4c65 7665 6c5f 7374 6f72  al(logLevel_stor
-00000fd0: 6564 292e 6368 616e 6765 2829 3b0a 0909  ed).change();...
-00000fe0: 096c 6f67 4c65 7665 6c20 3d20 6c6f 674c  .logLevel = logL
-00000ff0: 6576 656c 5f73 746f 7265 643b 0a09 097d  evel_stored;...}
-00001000: 0a0a 0920 202f 2f20 4368 6563 6b20 6966  ...  // Check if
-00001010: 2074 6865 206d 6573 7361 6765 2074 7970   the message typ
-00001020: 6520 6d61 7463 6865 7320 7468 6520 6669  e matches the fi
-00001030: 6c74 6572 696e 6720 636f 6e64 6974 696f  ltering conditio
-00001040: 6e0a 0909 6966 2028 2168 6973 746f 7269  n...if (!histori
-00001050: 635f 6c6f 6773 2e69 6e63 6c75 6465 7328  c_logs.includes(
-00001060: 6d65 7373 6167 6549 6429 2026 2620 6c6f  messageId) && lo
-00001070: 674c 6576 656c 735b 6c6f 674c 6576 656c  gLevels[logLevel
-00001080: 5d2e 696e 636c 7564 6573 286d 6573 7361  ].includes(messa
-00001090: 6765 2e74 7970 6529 2920 7b0a 0920 2020  ge.type)) {..   
-000010a0: 202f 2f20 5374 6f72 6520 746f 2074 6865   // Store to the
-000010b0: 2068 6973 746f 7269 6373 0a09 0909 6869   historics....hi
-000010c0: 7374 6f72 6963 5f6c 6f67 732e 7075 7368  storic_logs.push
-000010d0: 286d 6573 7361 6765 4964 293b 0a0a 0920  (messageId);... 
-000010e0: 2020 202f 2f20 466f 726d 6174 2074 6865     // Format the
-000010f0: 206e 6577 206c 6f67 0a09 0909 7661 7220   new log....var 
-00001100: 6c6f 6753 7472 696e 6720 3d20 273c 6469  logString = '<di
-00001110: 763e 5c0a 0909 093c 7370 616e 2063 6c61  v>\....<span cla
-00001120: 7373 3d22 6c6f 672d 7479 7065 2d27 2b6d  ss="log-type-'+m
-00001130: 6573 7361 6765 2e74 7970 652b 2722 3e5b  essage.type+'">[
-00001140: 2720 2b20 6d65 7373 6167 652e 7479 7065  ' + message.type
-00001150: 202b 2027 5d20 3c2f 7370 616e 3e5c 0a09   + '] </span>\..
-00001160: 0909 3c73 7061 6e20 636c 6173 733d 2266  ..<span class="f
-00001170: 6c6f 6174 2d73 7461 7274 223e 2720 2b20  loat-start">' + 
-00001180: 6d65 7373 6167 652e 636f 6e74 656e 7420  message.content 
-00001190: 2b20 273c 2f73 7061 6e3e 5c0a 0909 093c  + '</span>\....<
-000011a0: 7370 616e 2063 6c61 7373 3d22 6c6f 672d  span class="log-
-000011b0: 7469 6d65 7374 616d 7022 3e27 202b 206d  timestamp">' + m
-000011c0: 6573 7361 6765 2e74 696d 6573 7461 6d70  essage.timestamp
-000011d0: 202b 2027 3c2f 7370 616e 3e5c 0a09 0909   + '</span>\....
-000011e0: 3c2f 6469 763e 273b 0a0a 0920 2020 202f  </div>';...    /
-000011f0: 2f20 4170 7065 6e64 2074 6865 206e 6577  / Append the new
-00001200: 206c 6f67 0a09 0909 2428 2723 6c6f 6773   log....$('#logs
-00001210: 2d63 6f6e 7465 6e74 2729 2e61 7070 656e  -content').appen
-00001220: 6428 6c6f 6753 7472 696e 6729 3b0a 0a09  d(logString);...
-00001230: 2020 2020 2f2f 2053 6372 6f6c 6c20 746f      // Scroll to
-00001240: 206c 6174 6573 7420 6d65 7373 6167 650a   latest message.
-00001250: 0909 0976 6172 206c 6f67 7343 6f6e 7465  ...var logsConte
-00001260: 6e74 203d 2064 6f63 756d 656e 742e 6765  nt = document.ge
-00001270: 7445 6c65 6d65 6e74 4279 4964 2822 6c6f  tElementById("lo
-00001280: 6773 2d63 6f6e 7465 6e74 2229 3b0a 0909  gs-content");...
-00001290: 096c 6f67 7343 6f6e 7465 6e74 2e73 6372  .logsContent.scr
-000012a0: 6f6c 6c54 6f70 203d 206c 6f67 7343 6f6e  ollTop = logsCon
-000012b0: 7465 6e74 2e73 6372 6f6c 6c48 6569 6768  tent.scrollHeigh
-000012c0: 743b 0a09 097d 0a09 7d3b 0a09 0a09 2f2f  t;...}..};....//
-000012d0: 2048 616e 646c 6520 6669 6c74 6572 2064   Handle filter d
-000012e0: 726f 7064 6f77 6e20 6368 616e 6765 2065  ropdown change e
-000012f0: 7665 6e74 090a 0924 2827 236c 6f67 732d  vent...$('#logs-
-00001300: 6c65 7665 6c2d 6472 6f70 646f 776e 2729  level-dropdown')
-00001310: 2e63 6861 6e67 6528 6675 6e63 7469 6f6e  .change(function
-00001320: 2829 207b 0a09 096c 6f67 5f6c 6576 656c  () {...log_level
-00001330: 203d 2024 2874 6869 7329 2e76 616c 2829   = $(this).val()
-00001340: 3b0a 0909 2428 2723 6c6f 6773 2d63 6f6e  ;...$('#logs-con
-00001350: 7465 6e74 2729 2e65 6d70 7479 2829 3b0a  tent').empty();.
-00001360: 0909 6c6f 6361 6c53 746f 7261 6765 2e73  ..localStorage.s
-00001370: 6574 4974 656d 2827 6c6f 675f 6c65 7665  etItem('log_leve
-00001380: 6c27 2c20 6c6f 675f 6c65 7665 6c29 3b0a  l', log_level);.
-00001390: 0909 6869 7374 6f72 6963 5f6c 6f67 7320  ..historic_logs 
-000013a0: 3d20 5b5d 3b0a 097d 293b 0a0a 092f 2f20  = [];..});...// 
-000013b0: 4861 6e64 6c65 2053 7461 7274 2062 7574  Handle Start but
-000013c0: 746f 6e20 636c 6963 6b20 6576 656e 740a  ton click event.
-000013d0: 0924 2827 2373 7461 7274 2d62 7574 746f  .$('#start-butto
-000013e0: 6e27 292e 636c 6963 6b28 6675 6e63 7469  n').click(functi
-000013f0: 6f6e 2829 207b 0a09 0924 2e61 6a61 7828  on() {...$.ajax(
-00001400: 7b20 0a09 0909 7479 7065 3a20 2247 4554  { ....type: "GET
-00001410: 222c 0a09 0909 7572 6c3a 2022 7374 6172  ",....url: "star
-00001420: 7422 2c0a 0909 0973 7563 6365 7373 3a20  t",....success: 
-00001430: 6675 6e63 7469 6f6e 2864 6174 6129 7b0a  function(data){.
-00001440: 0909 0909 2f2f 2061 6c65 7274 2827 7374  ....// alert('st
-00001450: 6172 7465 6427 293b 0a09 0909 7d2c 0a09  arted');....},..
-00001460: 0909 6572 726f 723a 2066 756e 6374 696f  ..error: functio
-00001470: 6e28 7868 7229 7b0a 0909 0909 2f2f 2061  n(xhr){.....// a
-00001480: 6c65 7274 2827 6e6f 7420 7374 6172 7465  lert('not starte
-00001490: 6427 293b 0a09 0909 7d0a 0909 7d29 3b0a  d');....}...});.
-000014a0: 097d 293b 0a0a 092f 2f20 4861 6e64 6c65  .});...// Handle
-000014b0: 2053 746f 7020 6275 7474 6f6e 2063 6c69   Stop button cli
-000014c0: 636b 2065 7665 6e74 0a09 2428 2723 7374  ck event..$('#st
-000014d0: 6f70 2d62 7574 746f 6e27 292e 636c 6963  op-button').clic
-000014e0: 6b28 6675 6e63 7469 6f6e 2829 207b 0a09  k(function() {..
-000014f0: 0924 2e61 6a61 7828 7b20 0a09 0909 7479  .$.ajax({ ....ty
-00001500: 7065 3a20 2247 4554 222c 0a09 0909 7572  pe: "GET",....ur
-00001510: 6c3a 2022 7374 6f70 222c 0a09 0909 7375  l: "stop",....su
-00001520: 6363 6573 733a 2066 756e 6374 696f 6e28  ccess: function(
-00001530: 6461 7461 297b 0a09 0909 0965 7665 6e74  data){.....event
-00001540: 536f 7572 6365 2e63 6c6f 7365 2829 3b0a  Source.close();.
-00001550: 0909 0909 2f2f 2061 6c65 7274 2827 7374  ....// alert('st
-00001560: 6f70 7065 6427 293b 0a09 0909 7d2c 0a09  opped');....},..
-00001570: 0909 6572 726f 723a 2066 756e 6374 696f  ..error: functio
-00001580: 6e28 7868 7229 7b0a 0909 0909 2f2f 2061  n(xhr){.....// a
-00001590: 6c65 7274 2827 6e6f 7420 7374 6f70 7065  lert('not stoppe
-000015a0: 6427 293b 0a09 0909 7d0a 0909 7d29 3b0a  d');....}...});.
-000015b0: 097d 293b 0a0a 092f 2f20 4861 6e64 6c65  .});...// Handle
-000015c0: 2063 6c65 6172 206c 6f67 7320 6275 7474   clear logs butt
-000015d0: 6f6e 2063 6c69 636b 2065 7665 6e74 0a09  on click event..
-000015e0: 2428 2723 636c 6561 722d 6275 7474 6f6e  $('#clear-button
-000015f0: 2729 2e63 6c69 636b 2866 756e 6374 696f  ').click(functio
-00001600: 6e28 2920 7b0a 0909 242e 616a 6178 287b  n() {...$.ajax({
-00001610: 200a 0909 0974 7970 653a 2022 4745 5422   ....type: "GET"
-00001620: 2c0a 0909 0975 726c 3a20 2263 6c65 6172  ,....url: "clear
-00001630: 222c 0a09 0909 7375 6363 6573 733a 2066  ",....success: f
-00001640: 756e 6374 696f 6e28 6461 7461 297b 0a09  unction(data){..
-00001650: 0909 0924 2827 236c 6f67 732d 636f 6e74  ...$('#logs-cont
-00001660: 656e 7427 292e 656d 7074 7928 293b 0a09  ent').empty();..
-00001670: 0909 7d2c 0a09 0909 6572 726f 723a 2066  ..},....error: f
-00001680: 756e 6374 696f 6e28 7868 7229 7b0a 0909  unction(xhr){...
-00001690: 0909 2f2f 2061 6c65 7274 2827 6e6f 7420  ..// alert('not 
-000016a0: 636c 6561 7227 293b 0a09 0909 7d0a 0909  clear');....}...
-000016b0: 7d29 3b0a 097d 293b 0a3c 2f73 6372 6970  });..});.</scrip
-000016c0: 743e 0a0a 3c2f 626f 6479 3e0a 3c2f 6874  t>..</body>.</ht
-000016d0: 6d6c 3e0a                                ml>.
+00000000: 7b25 2065 7874 656e 6473 2027 6261 7365  {% extends 'base
+00000010: 2e68 746d 6c27 2025 7d0a 0a0a 7b25 2062  .html' %}...{% b
+00000020: 6c6f 636b 2074 6974 6c65 2025 7d20 456e  lock title %} En
+00000030: 7669 726f 6e6d 656e 7420 6372 6561 7469  vironment creati
+00000040: 6f6e 207b 2520 656e 6462 6c6f 636b 2025  on {% endblock %
+00000050: 7d0a 0a7b 2520 626c 6f63 6b20 6578 7472  }..{% block extr
+00000060: 615f 6865 6164 2025 7d0a 3c73 7479 6c65  a_head %}.<style
+00000070: 2074 7970 653d 2274 6578 742f 6373 7322   type="text/css"
+00000080: 3e0a 0909 236c 6f67 732d 636f 6e74 656e  >...#logs-conten
+00000090: 7420 7b0a 0909 0968 6569 6768 743a 2035  t {....height: 5
+000000a0: 3030 7078 3b0a 0909 096f 7665 7266 6c6f  00px;....overflo
+000000b0: 773a 2061 7574 6f3b 0a09 0909 7768 6974  w: auto;....whit
+000000c0: 652d 7370 6163 653a 2070 7265 2d77 7261  e-space: pre-wra
+000000d0: 703b 0a09 0909 666c 6578 2d67 726f 773a  p;....flex-grow:
+000000e0: 2031 3b0a 0909 7d0a 0909 406d 6564 6961   1;...}...@media
+000000f0: 2028 6d61 782d 7769 6474 683a 2039 3931   (max-width: 991
+00000100: 7078 2920 7b0a 0909 0968 746d 6c2c 2062  px) {....html, b
+00000110: 6f64 792c 2023 6c6f 6773 2d63 6f6e 7465  ody, #logs-conte
+00000120: 6e74 207b 0a09 0909 0968 6569 6768 743a  nt {.....height:
+00000130: 2031 3030 253b 0a09 0909 0977 6964 7468   100%;.....width
+00000140: 3a20 3130 3025 3b0a 0909 0909 6d61 782d  : 100%;.....max-
+00000150: 7769 6474 683a 206e 6f6e 653b 0a09 0909  width: none;....
+00000160: 7d0a 0a09 0909 236c 6f67 732d 636f 6e74  }.....#logs-cont
+00000170: 656e 7420 7b0a 0909 0909 6d61 7267 696e  ent {.....margin
+00000180: 2d74 6f70 3a20 303b 0a09 0909 7d0a 0909  -top: 0;....}...
+00000190: 7d0a 0a09 092e 6c6f 672d 7479 7065 2d44  }.....log-type-D
+000001a0: 4542 5547 207b 0a09 0909 666c 6f61 743a  EBUG {....float:
+000001b0: 206c 6566 743b 0a09 0909 636f 6c6f 723a   left;....color:
+000001c0: 2062 6c75 653b 0a09 097d 0a09 092e 6c6f   blue;...}....lo
+000001d0: 672d 7479 7065 2d49 4e46 4f20 7b0a 0909  g-type-INFO {...
+000001e0: 0966 6c6f 6174 3a20 6c65 6674 3b0a 0909  .float: left;...
+000001f0: 0963 6f6c 6f72 3a20 6772 6565 6e3b 0a09  .color: green;..
+00000200: 097d 0a09 092e 6c6f 672d 7479 7065 2d57  .}....log-type-W
+00000210: 4152 4e20 7b0a 0909 0966 6c6f 6174 3a20  ARN {....float: 
+00000220: 6c65 6674 3b0a 0909 0963 6f6c 6f72 3a20  left;....color: 
+00000230: 2346 4643 3130 373b 0a09 097d 0a09 092e  #FFC107;...}....
+00000240: 6c6f 672d 7479 7065 2d45 5252 4f52 207b  log-type-ERROR {
+00000250: 0a09 0909 666c 6f61 743a 206c 6566 743b  ....float: left;
+00000260: 0a09 0909 636f 6c6f 723a 2072 6564 3b0a  ....color: red;.
+00000270: 0909 7d0a 0a09 092e 6c6f 672d 7469 6d65  ..}.....log-time
+00000280: 7374 616d 7020 7b0a 0909 0966 6f6e 742d  stamp {....font-
+00000290: 7369 7a65 3a20 3132 7078 3b0a 0909 0963  size: 12px;....c
+000002a0: 6f6c 6f72 3a20 6772 6179 3b0a 0909 0966  olor: gray;....f
+000002b0: 6c6f 6174 3a20 7269 6768 743b 0a09 097d  loat: right;...}
+000002c0: 0a0a 0909 236c 6f67 732d 6c65 7665 6c2d  ....#logs-level-
+000002d0: 6472 6f70 646f 776e 207b 0a09 0909 626f  dropdown {....bo
+000002e0: 7264 6572 3a20 3170 7820 736f 6c69 6420  rder: 1px solid 
+000002f0: 2363 6363 3b0a 0909 0962 6f72 6465 722d  #ccc;....border-
+00000300: 7261 6469 7573 3a20 3470 783b 0a09 0909  radius: 4px;....
+00000310: 7061 6464 696e 673a 2034 7078 2038 7078  padding: 4px 8px
+00000320: 3b0a 0909 0966 6f6e 742d 7369 7a65 3a20  ;....font-size: 
+00000330: 3136 7078 3b0a 0909 0966 6f6e 742d 6661  16px;....font-fa
+00000340: 6d69 6c79 3a20 4172 6961 6c2c 2073 616e  mily: Arial, san
+00000350: 732d 7365 7269 663b 0a09 0909 636f 6c6f  s-serif;....colo
+00000360: 723a 2023 3333 333b 0a09 0909 6261 636b  r: #333;....back
+00000370: 6772 6f75 6e64 2d63 6f6c 6f72 3a20 2366  ground-color: #f
+00000380: 6666 3b0a 0909 0962 6f78 2d73 6861 646f  ff;....box-shado
+00000390: 773a 2069 6e73 6574 2030 2031 7078 2033  w: inset 0 1px 3
+000003a0: 7078 2072 6762 6128 302c 2030 2c20 302c  px rgba(0, 0, 0,
+000003b0: 2030 2e31 293b 0a09 0909 7472 616e 7369   0.1);....transi
+000003c0: 7469 6f6e 3a20 626f 7264 6572 2d63 6f6c  tion: border-col
+000003d0: 6f72 2030 2e32 7320 6561 7365 2d69 6e2d  or 0.2s ease-in-
+000003e0: 6f75 742c 2062 6f78 2d73 6861 646f 7720  out, box-shadow 
+000003f0: 302e 3273 2065 6173 652d 696e 2d6f 7574  0.2s ease-in-out
+00000400: 3b0a 0909 7d0a 0a09 0923 6c6f 6773 2d6c  ;...}....#logs-l
+00000410: 6576 656c 2d64 726f 7064 6f77 6e3a 666f  evel-dropdown:fo
+00000420: 6375 7320 7b0a 0909 096f 7574 6c69 6e65  cus {....outline
+00000430: 3a20 6e6f 6e65 3b0a 0909 0962 6f72 6465  : none;....borde
+00000440: 722d 636f 6c6f 723a 2023 3030 3762 6666  r-color: #007bff
+00000450: 3b0a 0909 0962 6f78 2d73 6861 646f 773a  ;....box-shadow:
+00000460: 2069 6e73 6574 2030 2031 7078 2033 7078   inset 0 1px 3px
+00000470: 2072 6762 6128 302c 2030 2c20 302c 2030   rgba(0, 0, 0, 0
+00000480: 2e31 292c 2030 2030 2030 2032 7078 2072  .1), 0 0 0 2px r
+00000490: 6762 6128 302c 2031 3233 2c20 3235 352c  gba(0, 123, 255,
+000004a0: 2030 2e35 293b 0a09 097d 0a0a 0909 236c   0.5);...}....#l
+000004b0: 6f67 732d 6c65 7665 6c2d 666f 726d 206c  ogs-level-form l
+000004c0: 6162 656c 207b 0a09 0909 666f 6e74 2d73  abel {....font-s
+000004d0: 697a 653a 2031 3670 783b 0a09 0909 666f  ize: 16px;....fo
+000004e0: 6e74 2d66 616d 696c 793a 2041 7269 616c  nt-family: Arial
+000004f0: 2c20 7361 6e73 2d73 6572 6966 3b0a 0909  , sans-serif;...
+00000500: 0966 6f6e 742d 7765 6967 6874 3a20 626f  .font-weight: bo
+00000510: 6c64 3b0a 0909 096d 6172 6769 6e2d 7269  ld;....margin-ri
+00000520: 6768 743a 2038 7078 3b0a 0909 0963 6f6c  ght: 8px;....col
+00000530: 6f72 3a20 2333 3333 3b0a 0909 7d0a 0a09  or: #333;...}...
+00000540: 0923 6c6f 6773 2d6c 6576 656c 2d66 6f72  .#logs-level-for
+00000550: 6d2d 636f 6e74 6169 6e65 7220 7b0a 0909  m-container {...
+00000560: 0964 6973 706c 6179 3a20 696e 6c69 6e65  .display: inline
+00000570: 2d62 6c6f 636b 3b0a 0909 7d0a 0a09 0923  -block;...}....#
+00000580: 6c6f 6773 2d6c 6576 656c 2d66 6f72 6d2c  logs-level-form,
+00000590: 0a09 0923 6c6f 6773 2d6c 6576 656c 2d64  ...#logs-level-d
+000005a0: 726f 7064 6f77 6e20 7b0a 0909 0964 6973  ropdown {....dis
+000005b0: 706c 6179 3a20 696e 6c69 6e65 2d62 6c6f  play: inline-blo
+000005c0: 636b 3b0a 0909 7d0a 0a09 7d0a 093c 2f73  ck;...}...}..</s
+000005d0: 7479 6c65 3e0a 0a7b 2520 656e 6462 6c6f  tyle>..{% endblo
+000005e0: 636b 2025 7d0a 7b25 2062 6c6f 636b 2063  ck %}.{% block c
+000005f0: 6f6e 7465 6e74 2025 7d0a 3c64 6976 2063  ontent %}.<div c
+00000600: 6c61 7373 3d22 636f 6e74 6169 6e65 7222  lass="container"
+00000610: 2069 643d 2263 6f6e 7465 6e74 223e 0a09   id="content">..
+00000620: 3c64 6976 2063 6c61 7373 3d22 726f 7720  <div class="row 
+00000630: 616c 6967 6e2d 6974 656d 732d 6365 6e74  align-items-cent
+00000640: 6572 223e 0a09 093c 6469 7620 636c 6173  er">...<div clas
+00000650: 733d 2263 6f6c 223e 0a09 0909 3c68 333e  s="col">....<h3>
+00000660: 456e 7669 726f 6e6d 656e 7420 6372 6561  Environment crea
+00000670: 7469 6f6e 3c2f 6833 3e0a 0909 3c2f 6469  tion</h3>...</di
+00000680: 763e 0a09 093c 6469 7620 636c 6173 733d  v>...<div class=
+00000690: 2263 6f6c 2d61 7574 6f22 3e0a 0909 093c  "col-auto">....<
+000006a0: 6275 7474 6f6e 2069 643d 2263 7265 6174  button id="creat
+000006b0: 655f 656e 765f 6275 7474 6f6e 2220 636c  e_env_button" cl
+000006c0: 6173 733d 2262 746e 2062 746e 2d73 7563  ass="btn btn-suc
+000006d0: 6365 7373 223e 4372 6561 7465 3c2f 6275  cess">Create</bu
+000006e0: 7474 6f6e 3e0a 0909 3c2f 6469 763e 0a09  tton>...</div>..
+000006f0: 3c2f 6469 763e 0a09 3c68 723e 0a09 3c64  </div>..<hr>..<d
+00000700: 6976 2063 6c61 7373 3d22 726f 7722 3e0a  iv class="row">.
+00000710: 0909 3c64 6976 2063 6c61 7373 3d22 636f  ..<div class="co
+00000720: 6c22 3e0a 0909 093c 6469 7620 636c 6173  l">....<div clas
+00000730: 733d 2272 6f77 223e 0a09 0909 093c 6469  s="row">.....<di
+00000740: 7620 636c 6173 733d 2263 6f6c 223e 0a09  v class="col">..
+00000750: 0909 0909 3c68 343e 4172 6561 733a 207b  ....<h4>Areas: {
+00000760: 7b20 5433 5346 2e70 6c61 7965 7273 5f6c  { T3SF.players_l
+00000770: 6973 747c 636f 756e 7420 7d7d 203c 2f68  ist|count }} </h
+00000780: 343e 0a09 0909 093c 2f64 6976 3e0a 0909  4>.....</div>...
+00000790: 0909 3c64 6976 2063 6c61 7373 3d22 636f  ..<div class="co
+000007a0: 6c22 3e0a 0909 0909 093c 6834 3e43 6861  l">......<h4>Cha
+000007b0: 6e6e 656c 7320 746f 2063 7265 6174 6520  nnels to create 
+000007c0: 7065 7220 4172 6561 3a3c 2f68 343e 0a09  per Area:</h4>..
+000007d0: 0909 093c 2f64 6976 3e0a 0909 0909 3c64  ...</div>.....<d
+000007e0: 6976 2063 6c61 7373 3d22 636f 6c22 3e0a  iv class="col">.
+000007f0: 0909 0909 093c 6834 3e43 6861 6e6e 656c  .....<h4>Channel
+00000800: 7320 666f 7220 4761 6d65 204d 6173 7465  s for Game Maste
+00000810: 7273 3a3c 2f68 343e 0a09 0909 093c 2f64  rs:</h4>.....</d
+00000820: 6976 3e0a 0909 093c 2f64 6976 3e0a 0909  iv>....</div>...
+00000830: 093c 6469 7620 636c 6173 733d 2272 6f77  .<div class="row
+00000840: 223e 0a09 0909 093c 6469 7620 636c 6173  ">.....<div clas
+00000850: 733d 2263 6f6c 223e 0a09 0909 0909 7b25  s="col">......{%
+00000860: 2d20 666f 7220 706c 6179 6572 2069 6e20  - for player in 
+00000870: 5433 5346 2e70 6c61 7965 7273 5f6c 6973  T3SF.players_lis
+00000880: 7420 2d25 7d0a 0909 0909 0909 3c68 3520  t -%}.......<h5 
+00000890: 636c 6173 733d 2274 6578 742d 6d75 7465  class="text-mute
+000008a0: 6422 3e7b 7b70 6c61 7965 727d 7d3c 6835  d">{{player}}<h5
+000008b0: 3e0a 0909 0909 097b 252d 2065 6e64 666f  >......{%- endfo
+000008c0: 7220 2d25 7d0a 0909 0909 3c2f 6469 763e  r -%}.....</div>
+000008d0: 0a09 0909 093c 6469 7620 636c 6173 733d  .....<div class=
+000008e0: 2263 6f6c 223e 0a09 0909 0909 3c68 3520  "col">......<h5 
+000008f0: 636c 6173 733d 2274 6578 742d 6d75 7465  class="text-mute
+00000900: 6422 3e49 6e74 6572 6e61 6c20 6368 6174  d">Internal chat
+00000910: 3c68 353e 0a09 0909 0909 3c68 3520 636c  <h5>......<h5 cl
+00000920: 6173 733d 2274 6578 742d 6d75 7465 6422  ass="text-muted"
+00000930: 3e49 6e62 6f78 3c68 353e 0a09 0909 0909  >Inbox<h5>......
+00000940: 3c68 3520 636c 6173 733d 2274 6578 742d  <h5 class="text-
+00000950: 6d75 7465 6422 3e44 6563 6973 696f 6e20  muted">Decision 
+00000960: 6c6f 673c 6835 3e0a 0909 0909 097b 252d  log<h5>......{%-
+00000970: 2069 6620 5433 5346 2e70 6c61 7466 6f72   if T3SF.platfor
+00000980: 6d20 3d3d 2022 6469 7363 6f72 6422 202d  m == "discord" -
+00000990: 257d 0a09 0909 0909 093c 6835 2063 6c61  %}.......<h5 cla
+000009a0: 7373 3d22 7465 7874 2d6d 7574 6564 223e  ss="text-muted">
+000009b0: 566f 6963 6520 6368 616e 6e65 6c3c 6835  Voice channel<h5
+000009c0: 3e0a 0909 0909 097b 252d 2065 6e64 6966  >......{%- endif
+000009d0: 202d 257d 0a09 0909 093c 2f64 6976 3e0a   -%}.....</div>.
+000009e0: 0909 0909 3c64 6976 2063 6c61 7373 3d22  ....<div class="
+000009f0: 636f 6c22 3e0a 0909 0909 093c 6835 2063  col">......<h5 c
+00000a00: 6c61 7373 3d22 7465 7874 2d6d 7574 6564  lass="text-muted
+00000a10: 223e 496e 7465 726e 616c 2063 6861 743c  ">Internal chat<
+00000a20: 6835 3e0a 0909 0909 093c 6835 2063 6c61  h5>......<h5 cla
+00000a30: 7373 3d22 7465 7874 2d6d 7574 6564 223e  ss="text-muted">
+00000a40: 4c6f 6773 3c68 353e 0a09 0909 0909 7b25  Logs<h5>......{%
+00000a50: 2d20 6966 2054 3353 462e 706c 6174 666f  - if T3SF.platfo
+00000a60: 726d 203d 3d20 2264 6973 636f 7264 2220  rm == "discord" 
+00000a70: 2d25 7d0a 0909 0909 0909 3c68 3520 636c  -%}.......<h5 cl
+00000a80: 6173 733d 2274 6578 742d 6d75 7465 6422  ass="text-muted"
+00000a90: 3e56 6f69 6365 2063 6861 6e6e 656c 3c68  >Voice channel<h
+00000aa0: 353e 0a09 0909 0909 7b25 2d20 656e 6469  5>......{%- endi
+00000ab0: 6620 2d25 7d0a 0909 0909 3c2f 6469 763e  f -%}.....</div>
+00000ac0: 0a09 0909 3c2f 6469 763e 0a09 093c 2f64  ....</div>...</d
+00000ad0: 6976 3e0a 093c 2f64 6976 3e0a 093c 6469  iv>..</div>..<di
+00000ae0: 7620 636c 6173 733d 2272 6f77 2220 7374  v class="row" st
+00000af0: 796c 653d 2276 6973 6962 696c 6974 793a  yle="visibility:
+00000b00: 2068 6964 6465 6e3b 2220 6964 3d22 6c6f   hidden;" id="lo
+00000b10: 6773 2d63 6f6e 7461 696e 6572 223e 0a09  gs-container">..
+00000b20: 093c 6469 7620 636c 6173 733d 2263 6f6c  .<div class="col
+00000b30: 223e 0a09 0909 3c68 723e 0a09 0909 3c64  ">....<hr>....<d
+00000b40: 6976 2063 6c61 7373 3d22 6267 2d6c 6967  iv class="bg-lig
+00000b50: 6874 2072 6f75 6e64 6564 2070 2d33 2220  ht rounded p-3" 
+00000b60: 6964 3d22 6c6f 6773 2d63 6f6e 7465 6e74  id="logs-content
+00000b70: 223e 0a09 0909 3c2f 6469 763e 0a09 093c  ">....</div>...<
+00000b80: 2f64 6976 3e0a 093c 2f64 6976 3e0a 3c2f  /div>..</div>.</
+00000b90: 6469 763e 0a3c 7363 7269 7074 3e0a 0924  div>.<script>..$
+00000ba0: 2827 2363 7265 6174 655f 656e 765f 6275  ('#create_env_bu
+00000bb0: 7474 6f6e 2729 2e63 6c69 636b 2866 756e  tton').click(fun
+00000bc0: 6374 696f 6e28 2920 7b0a 0909 7b25 2d20  ction() {...{%- 
+00000bd0: 6966 2054 3353 462e 706c 6174 666f 726d  if T3SF.platform
+00000be0: 203d 3d20 2264 6973 636f 7264 2220 2d25   == "discord" -%
+00000bf0: 7d0a 0909 7661 7220 6e75 6d20 3d20 7072  }...var num = pr
+00000c00: 6f6d 7074 2822 5768 6174 2773 2079 6f75  ompt("What's you
+00000c10: 7220 4469 7363 6f72 6427 7320 7365 7276  r Discord's serv
+00000c20: 6572 2049 443f 2022 293b 0a09 0976 6172  er ID? ");...var
+00000c30: 2075 726c 203d 2022 6372 6561 7465 3f73   url = "create?s
+00000c40: 6572 7665 723d 2220 2b20 6e75 6d3b 0a09  erver=" + num;..
+00000c50: 097b 252d 2065 6c73 6520 2d25 7d0a 0909  .{%- else -%}...
+00000c60: 7661 7220 7572 6c20 3d20 2263 7265 6174  var url = "creat
+00000c70: 6522 3b0a 0909 7b25 2d20 656e 6469 6620  e";...{%- endif 
+00000c80: 2d25 7d0a 0909 242e 616a 6178 287b 200a  -%}...$.ajax({ .
+00000c90: 0909 0974 7970 653a 2022 4745 5422 2c0a  ...type: "GET",.
+00000ca0: 0909 0975 726c 3a20 7572 6c2c 0a09 0909  ...url: url,....
+00000cb0: 6265 666f 7265 5365 6e64 3a20 6675 6e63  beforeSend: func
+00000cc0: 7469 6f6e 2829 207b 0a09 0909 0964 6f63  tion() {.....doc
+00000cd0: 756d 656e 742e 6765 7445 6c65 6d65 6e74  ument.getElement
+00000ce0: 4279 4964 2827 6372 6561 7465 5f65 6e76  ById('create_env
+00000cf0: 5f62 7574 746f 6e27 292e 6469 7361 626c  _button').disabl
+00000d00: 6564 203d 2074 7275 653b 0a09 0909 0962  ed = true;.....b
+00000d10: 3574 6f61 7374 2e73 686f 7728 2277 6172  5toast.show("war
+00000d20: 6e69 6e67 222c 2022 4372 6561 7469 6e67  ning", "Creating
+00000d30: 2065 6e76 6972 6f6e 6d65 6e74 2120 222c   environment! ",
+00000d40: 2022 546f 2063 6865 636b 2074 6865 2073   "To check the s
+00000d50: 7461 7475 7320 6f66 2074 6865 2045 6e76  tatus of the Env
+00000d60: 6972 6f6e 6d65 6e74 2063 7265 6174 696f  ironment creatio
+00000d70: 6e20 6368 6563 6b20 7468 6520 6c6f 6773  n check the logs
+00000d80: 2062 656c 6f77 222c 2033 3030 3029 3b0a   below", 3000);.
+00000d90: 0909 0909 2428 2723 6c6f 6773 2d63 6f6e  ....$('#logs-con
+00000da0: 7465 6e74 2729 2e65 6d70 7479 2829 3b0a  tent').empty();.
+00000db0: 0909 0909 2428 2223 6c6f 6773 2d63 6f6e  ....$("#logs-con
+00000dc0: 7461 696e 6572 2229 2e63 7373 2822 7669  tainer").css("vi
+00000dd0: 7369 6269 6c69 7479 222c 2022 7669 7369  sibility", "visi
+00000de0: 626c 6522 293b 0a09 0909 090a 0909 0909  ble");..........
+00000df0: 6469 7363 6c61 696d 6572 203d 207b 2520  disclaimer = {% 
+00000e00: 6966 2054 3353 462e 706c 6174 666f 726d  if T3SF.platform
+00000e10: 203d 3d20 2264 6973 636f 7264 2220 257d   == "discord" %}
+00000e20: 2754 6865 2073 6572 7665 7220 6f77 6e65  'The server owne
+00000e30: 7220 7368 6f75 6c64 2073 6565 2065 6163  r should see eac
+00000e40: 6820 6372 6561 7465 6420 6368 616e 6e65  h created channe
+00000e50: 6c2e 277b 2520 656c 7365 2025 7d27 5765  l.'{% else %}'We
+00000e60: 2077 696c 6c20 696e 7669 7465 2074 6865   will invite the
+00000e70: 2057 6f72 6b73 7061 6365 206f 776e 6572   Workspace owner
+00000e80: 2074 6f20 6561 6368 2063 7265 6174 6564   to each created
+00000e90: 2063 6861 6e6e 656c 2e27 7b25 2065 6e64   channel.'{% end
+00000ea0: 6966 2025 7d0a 0a09 0909 0976 6172 206c  if %}......var l
+00000eb0: 6f67 5374 7269 6e67 203d 2027 3c62 3e5c  ogString = '<b>\
+00000ec0: 3c64 6976 3e5c 0a09 0909 093c 7370 616e  <div>\.....<span
+00000ed0: 2063 6c61 7373 3d22 6c6f 672d 7479 7065   class="log-type
+00000ee0: 2d49 4e46 4f22 3e5b 494e 464f 5d20 3c2f  -INFO">[INFO] </
+00000ef0: 7370 616e 3e5c 0a09 0909 093c 7370 616e  span>\.....<span
+00000f00: 2063 6c61 7373 3d22 666c 6f61 742d 7374   class="float-st
+00000f10: 6172 7422 3e3c 623e 2720 2b20 6469 7363  art"><b>' + disc
+00000f20: 6c61 696d 6572 202b 273c 2f62 3e3c 2f73  laimer +'</b></s
+00000f30: 7061 6e3e 5c0a 0909 0909 3c2f 6469 763e  pan>\.....</div>
+00000f40: 3c2f 623e 273b 0a09 0909 0924 2827 236c  </b>';.....$('#l
+00000f50: 6f67 732d 636f 6e74 656e 7427 292e 6170  ogs-content').ap
+00000f60: 7065 6e64 286c 6f67 5374 7269 6e67 293b  pend(logString);
+00000f70: 207d 2c0a 0909 0973 7563 6365 7373 3a20   },....success: 
+00000f80: 6675 6e63 7469 6f6e 2864 6174 6129 7b0a  function(data){.
+00000f90: 0909 0909 6235 746f 6173 742e 7368 6f77  ....b5toast.show
+00000fa0: 2822 7375 6363 6573 7322 2c20 2245 6e76  ("success", "Env
+00000fb0: 6972 6f6e 6d65 6e74 2063 7265 6174 6564  ironment created
+00000fc0: 2120 222c 2022 5669 6577 2074 6865 206c  ! ", "View the l
+00000fd0: 6f67 7320 666f 7220 6d6f 7265 2069 6e66  ogs for more inf
+00000fe0: 6f72 6d61 7469 6f6e 222c 2033 3030 3029  ormation", 3000)
+00000ff0: 3b0a 0909 097d 2c0a 0909 0965 7272 6f72  ;....},....error
+00001000: 3a20 6675 6e63 7469 6f6e 2878 6872 297b  : function(xhr){
+00001010: 0a09 0909 0964 6f63 756d 656e 742e 6765  .....document.ge
+00001020: 7445 6c65 6d65 6e74 4279 4964 2827 6372  tElementById('cr
+00001030: 6561 7465 5f65 6e76 5f62 7574 746f 6e27  eate_env_button'
+00001040: 292e 6469 7361 626c 6564 203d 2066 616c  ).disabled = fal
+00001050: 7365 3b0a 0909 0909 6235 746f 6173 742e  se;.....b5toast.
+00001060: 7368 6f77 2822 6461 6e67 6572 222c 2022  show("danger", "
+00001070: 4572 726f 7220 6372 6561 7469 6e67 2065  Error creating e
+00001080: 7665 7279 7468 696e 6721 2022 2c20 2256  verything! ", "V
+00001090: 6965 7720 7468 6520 6c6f 6773 2066 6f72  iew the logs for
+000010a0: 206d 6f72 6520 696e 666f 726d 6174 696f   more informatio
+000010b0: 6e22 2c20 3530 3030 293b 0a09 0909 7d0a  n", 5000);....}.
+000010c0: 0909 7d29 3b0a 097d 293b 0a3c 2f73 6372  ..});..});.</scr
+000010d0: 6970 743e 0a0a 3c73 6372 6970 743e 0a09  ipt>..<script>..
+000010e0: 6c65 7420 6576 656e 7453 6f75 7263 6520  let eventSource 
+000010f0: 3d20 6e65 7720 4576 656e 7453 6f75 7263  = new EventSourc
+00001100: 6528 272f 7374 7265 616d 5f6e 6577 7327  e('/stream_news'
+00001110: 293b 0a09 6c65 7420 6869 7374 6f72 6963  );..let historic
+00001120: 5f6c 6f67 7320 3d20 5b5d 3b0a 0a09 6576  _logs = [];...ev
+00001130: 656e 7453 6f75 7263 652e 6f6e 6f70 656e  entSource.onopen
+00001140: 203d 2066 756e 6374 696f 6e28 2920 7b0a   = function() {.
+00001150: 0909 6861 6e64 6c65 5f73 7365 5f73 7461  ..handle_sse_sta
+00001160: 7274 2865 7665 6e74 293b 0a09 7d3b 0a0a  rt(event);..};..
+00001170: 0965 7665 6e74 536f 7572 6365 2e6f 6e6d  .eventSource.onm
+00001180: 6573 7361 6765 203d 2066 756e 6374 696f  essage = functio
+00001190: 6e28 6576 656e 7429 207b 0a09 0968 616e  n(event) {...han
+000011a0: 646c 655f 7373 655f 6d65 7373 6167 6573  dle_sse_messages
+000011b0: 2865 7665 6e74 293b 0a09 7d3b 0a0a 0965  (event);..};...e
+000011c0: 7665 6e74 536f 7572 6365 2e6f 6e65 7272  ventSource.onerr
+000011d0: 6f72 203d 2066 756e 6374 696f 6e28 6576  or = function(ev
+000011e0: 656e 7429 207b 0a09 0968 616e 646c 655f  ent) {...handle_
+000011f0: 7373 655f 6572 726f 7273 2865 7665 6e74  sse_errors(event
+00001200: 293b 0a09 7d3b 0a0a 0966 756e 6374 696f  );..};...functio
+00001210: 6e20 6861 6e64 6c65 5f73 7365 5f6d 6573  n handle_sse_mes
+00001220: 7361 6765 7328 6576 656e 7429 7b0a 0909  sages(event){...
+00001230: 7661 7220 6d65 7373 6167 6520 3d20 4a53  var message = JS
+00001240: 4f4e 2e70 6172 7365 2865 7665 6e74 2e64  ON.parse(event.d
+00001250: 6174 6129 3b0a 0909 7661 7220 6d65 7373  ata);...var mess
+00001260: 6167 6549 6420 3d20 6d65 7373 6167 652e  ageId = message.
+00001270: 6964 3b0a 0a09 0969 6620 2821 6869 7374  id;....if (!hist
+00001280: 6f72 6963 5f6c 6f67 732e 696e 636c 7564  oric_logs.includ
+00001290: 6573 286d 6573 7361 6765 4964 2929 207b  es(messageId)) {
+000012a0: 0a09 0909 2f2f 2053 746f 7265 2074 6f20  ....// Store to 
+000012b0: 7468 6520 6869 7374 6f72 6963 730a 0909  the historics...
+000012c0: 0968 6973 746f 7269 635f 6c6f 6773 2e70  .historic_logs.p
+000012d0: 7573 6828 6d65 7373 6167 6549 6429 3b0a  ush(messageId);.
+000012e0: 0a09 0909 2f2f 2046 6f72 6d61 7420 7468  ....// Format th
+000012f0: 6520 6e65 7720 6c6f 670a 0909 0976 6172  e new log....var
+00001300: 206c 6f67 5374 7269 6e67 203d 2027 3c64   logString = '<d
+00001310: 6976 3e5c 0a09 0909 3c73 7061 6e20 636c  iv>\....<span cl
+00001320: 6173 733d 226c 6f67 2d74 7970 652d 272b  ass="log-type-'+
+00001330: 6d65 7373 6167 652e 7479 7065 2b27 223e  message.type+'">
+00001340: 5b27 202b 206d 6573 7361 6765 2e74 7970  [' + message.typ
+00001350: 6520 2b20 275d 203c 2f73 7061 6e3e 5c0a  e + '] </span>\.
+00001360: 0909 093c 7370 616e 2063 6c61 7373 3d22  ...<span class="
+00001370: 666c 6f61 742d 7374 6172 7422 3e27 202b  float-start">' +
+00001380: 206d 6573 7361 6765 2e63 6f6e 7465 6e74   message.content
+00001390: 202b 2027 3c2f 7370 616e 3e5c 0a09 0909   + '</span>\....
+000013a0: 3c73 7061 6e20 636c 6173 733d 226c 6f67  <span class="log
+000013b0: 2d74 696d 6573 7461 6d70 223e 2720 2b20  -timestamp">' + 
+000013c0: 6d65 7373 6167 652e 7469 6d65 7374 616d  message.timestam
+000013d0: 7020 2b20 273c 2f73 7061 6e3e 5c0a 0909  p + '</span>\...
+000013e0: 093c 2f64 6976 3e27 3b0a 0a09 0909 2f2f  .</div>';.....//
+000013f0: 2041 7070 656e 6420 7468 6520 6e65 7720   Append the new 
+00001400: 6c6f 670a 0909 0924 2827 236c 6f67 732d  log....$('#logs-
+00001410: 636f 6e74 656e 7427 292e 6170 7065 6e64  content').append
+00001420: 286c 6f67 5374 7269 6e67 293b 0a0a 0909  (logString);....
+00001430: 092f 2f20 5363 726f 6c6c 2074 6f20 6c61  .// Scroll to la
+00001440: 7465 7374 206d 6573 7361 6765 0a09 0909  test message....
+00001450: 7661 7220 6c6f 6773 436f 6e74 656e 7420  var logsContent 
+00001460: 3d20 646f 6375 6d65 6e74 2e67 6574 456c  = document.getEl
+00001470: 656d 656e 7442 7949 6428 226c 6f67 732d  ementById("logs-
+00001480: 636f 6e74 656e 7422 293b 0a09 0909 6c6f  content");....lo
+00001490: 6773 436f 6e74 656e 742e 7363 726f 6c6c  gsContent.scroll
+000014a0: 546f 7020 3d20 6c6f 6773 436f 6e74 656e  Top = logsConten
+000014b0: 742e 7363 726f 6c6c 4865 6967 6874 3b0a  t.scrollHeight;.
+000014c0: 0909 7d0a 097d 3b0a 0a09 6675 6e63 7469  ..}..};...functi
+000014d0: 6f6e 2068 616e 646c 655f 7373 655f 7374  on handle_sse_st
+000014e0: 6172 7428 6576 656e 7429 7b0a 0909 636f  art(event){...co
+000014f0: 6e73 6f6c 652e 6c6f 6728 2247 6574 7469  nsole.log("Getti
+00001500: 6e67 2073 6572 7665 7220 7570 6461 7465  ng server update
+00001510: 7322 293b 0a09 7d3b 0a0a 0966 756e 6374  s");..};...funct
+00001520: 696f 6e20 6861 6e64 6c65 5f73 7365 5f65  ion handle_sse_e
+00001530: 7272 6f72 7328 6576 656e 7429 7b0a 0909  rrors(event){...
+00001540: 636f 6e73 6f6c 652e 6c6f 6728 2745 7665  console.log('Eve
+00001550: 6e74 536f 7572 6365 2065 7272 6f72 3a27  ntSource error:'
+00001560: 2c20 6576 656e 7429 3b0a 0909 646f 6375  , event);...docu
+00001570: 6d65 6e74 2e67 6574 456c 656d 656e 7442  ment.getElementB
+00001580: 7949 6428 2763 7265 6174 655f 656e 765f  yId('create_env_
+00001590: 6275 7474 6f6e 2729 2e64 6973 6162 6c65  button').disable
+000015a0: 6420 3d20 7472 7565 3b0a 0a09 7d3b 0a3c  d = true;...};.<
+000015b0: 2f73 6372 6970 743e 0a7b 2520 656e 6462  /script>.{% endb
+000015c0: 6c6f 636b 2025 7d                        lock %}
```

### Comparing `T3SF-1.2/src/T3SF/logger/logger.py` & `T3SF-2.0rc1/src/T3SF/logger/logger.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,11 +1,13 @@
+from T3SF.gui.core import MessageAnnouncer
 from datetime import datetime
 import json
 import uuid
 
+
 class T3SF_Logger:
     @staticmethod
     def emit(message,message_type="DEBUG"):
         try:
             message = message.replace("\n"," ")
 
             # Create a dictionary with the message data
@@ -15,16 +17,19 @@
                 "content": message,
                 "timestamp": datetime.now().strftime("%H:%M:%S")
             }
 
             # Convert the dictionary to a JSON string
             sse_msg = f"data: {json.dumps(message_data)}\n\n"
 
+            announcer = MessageAnnouncer()
+            announcer.announce(msg=sse_msg)
+
             # Do something with the EventSource-formatted message, such as writing it to a file
-            with open('logs.txt', 'a') as f:
+            with open('logs.txt', 'a+') as f:
                 f.write(sse_msg)
 
             # Print some critical information to the terminal
             if message_type in ['WARN', 'ERROR']:
                 red = '\033[91m\033[5m'
                 yellow = '\033[93m\033[5m'
                 nc = '\033[0m'
```

### Comparing `T3SF-1.2/src/T3SF/slack/slack.py` & `T3SF-2.0rc1/src/T3SF/slack/slack.py`

 * *Files identical despite different names*

### Comparing `T3SF-1.2/src/T3SF.egg-info/PKG-INFO` & `T3SF-2.0rc1/src/T3SF.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: T3SF
-Version: 1.2
+Version: 2.0rc1
 Summary: Technical Tabletop Exercises Simulation Framework
 Home-page: https://github.com/Base4Security/T3SF
 Author: BASE4 Security
 Author-email: jlanfranconi@base4sec.com
 Project-URL: Bug Tracker, https://github.com/Base4Security/T3SF/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
@@ -49,15 +49,15 @@
 ## Getting Things Ready <a name = "Starting"></a>
 To use the framework with your desired platform, whether it's Slack or Discord, you will need to install the required modules for that platform. But don't worry, installing these modules is easy and straightforward.
 
 To do this, you can follow this simple step-by-step guide, or if you're already comfortable installing packages with `pip`, you can skip to the last step!
 
 ```bash
 # Python 3.6+ required
-python -m venv .venv       # We will create a python virtual enviroment
+python -m venv .venv       # We will create a python virtual environment
 source .venv/bin/activate  # Let's get inside it
 
 pip install -U pip         # Upgrade pip
 ```
 
 Once you have created a Python virtual environment and activated it, you can install the T3SF framework for your desired platform by running the following command:
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: T3SF Version: 1.2 Summary: Technical Tabletop
+Metadata-Version: 2.1 Name: T3SF Version: 2.0rc1 Summary: Technical Tabletop
 Exercises Simulation Framework Home-page: https://github.com/Base4Security/T3SF
 Author: BASE4 Security Author-email: jlanfranconi@base4sec.com Project-URL: Bug
 Tracker, https://github.com/Base4Security/T3SF/issues Classifier: Programming
 Language :: Python :: 3 Classifier: License :: OSI Approved :: GNU General
 Public License v3 (GPLv3) Classifier: Topic :: Software Development ::
 Libraries :: Application Frameworks Classifier: Operating System :: OS
 Independent Description-Content-Type: text/markdown Provides-Extra: Slack
@@ -30,19 +30,19 @@
 organization, single area" and "multiple organization, multiple areas". ##
 Getting Things Ready  To use the framework with your desired platform, whether
 it's Slack or Discord, you will need to install the required modules for that
 platform. But don't worry, installing these modules is easy and
 straightforward. To do this, you can follow this simple step-by-step guide, or
 if you're already comfortable installing packages with `pip`, you can skip to
 the last step! ```bash # Python 3.6+ required python -m venv .venv # We will
-create a python virtual enviroment source .venv/bin/activate # Let's get inside
-it pip install -U pip # Upgrade pip ``` Once you have created a Python virtual
-environment and activated it, you can install the T3SF framework for your
-desired platform by running the following command: ```bash pip install "T3SF
-[Discord]" # Install the framework to work with Discord ``` or ```bash pip
+create a python virtual environment source .venv/bin/activate # Let's get
+inside it pip install -U pip # Upgrade pip ``` Once you have created a Python
+virtual environment and activated it, you can install the T3SF framework for
+your desired platform by running the following command: ```bash pip install
+"T3SF[Discord]" # Install the framework to work with Discord ``` or ```bash pip
 install "T3SF[Slack]" # Install the framework to work with Slack ``` This will
 install the T3SF framework along with the required dependencies for your chosen
 platform. Once the installation is complete, you can start using the framework
 with your platform of choice. We strongly recommend following the platform-
 specific guidance within our Read The Docs! Here are the links: - [Discord]
 (https://t3sf.readthedocs.io/en/latest/Discord.html#installation) - [Slack]
 (https://t3sf.readthedocs.io/en/latest/Slack.html#installation) - [Telegram]
```

### Comparing `T3SF-1.2/src/T3SF.egg-info/SOURCES.txt` & `T3SF-2.0rc1/src/T3SF.egg-info/SOURCES.txt`

 * *Files 10% similar despite different names*

```diff
@@ -11,13 +11,16 @@
 src/T3SF.egg-info/requires.txt
 src/T3SF.egg-info/top_level.txt
 src/T3SF/discord/__init__.py
 src/T3SF/discord/bot.py
 src/T3SF/discord/discord.py
 src/T3SF/gui/__init__.py
 src/T3SF/gui/core.py
+src/T3SF/gui/templates/base.html
+src/T3SF/gui/templates/env_creation.html
 src/T3SF/gui/templates/index.html
+src/T3SF/gui/templates/msel_viewer.html
 src/T3SF/logger/__init__.py
 src/T3SF/logger/logger.py
 src/T3SF/slack/__init__.py
 src/T3SF/slack/bot.py
 src/T3SF/slack/slack.py
```

