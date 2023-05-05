# Comparing `tmp/discord-qalib-2.2.1.tar.gz` & `tmp/discord-qalib-2.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "discord-qalib-2.2.1.tar", last modified: Sat Apr 29 18:21:38 2023, max compression
+gzip compressed data, was "discord-qalib-2.2.2.tar", last modified: Fri May  5 16:45:39 2023, max compression
```

## Comparing `discord-qalib-2.2.1.tar` & `discord-qalib-2.2.2.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 18:21:38.020867 discord-qalib-2.2.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-04-29 18:21:11.000000 discord-qalib-2.2.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     4766 2023-04-29 18:21:38.020867 discord-qalib-2.2.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     4087 2023-04-29 18:21:11.000000 discord-qalib-2.2.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 18:21:38.016867 discord-qalib-2.2.1/discord_qalib.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4766 2023-04-29 18:21:38.000000 discord-qalib-2.2.1/discord_qalib.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      689 2023-04-29 18:21:38.000000 discord-qalib-2.2.1/discord_qalib.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-29 18:21:38.000000 discord-qalib-2.2.1/discord_qalib.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      150 2023-04-29 18:21:38.000000 discord-qalib-2.2.1/discord_qalib.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        6 2023-04-29 18:21:38.000000 discord-qalib-2.2.1/discord_qalib.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1459 2023-04-29 18:21:27.000000 discord-qalib-2.2.1/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 18:21:38.020867 discord-qalib-2.2.1/qalib/
--rw-r--r--   0 runner    (1001) docker     (123)     3736 2023-04-29 18:21:27.000000 discord-qalib-2.2.1/qalib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6030 2023-04-29 18:21:11.000000 discord-qalib-2.2.1/qalib/context.py
--rw-r--r--   0 runner    (1001) docker     (123)     7380 2023-04-29 18:21:11.000000 discord-qalib-2.2.1/qalib/interaction.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-29 18:21:11.000000 discord-qalib-2.2.1/qalib/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)     3091 2023-04-29 18:21:11.000000 discord-qalib-2.2.1/qalib/renderer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 18:21:38.020867 discord-qalib-2.2.1/qalib/template_engines/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-29 18:21:11.000000 discord-qalib-2.2.1/qalib/template_engines/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1290 2023-04-29 18:21:11.000000 discord-qalib-2.2.1/qalib/template_engines/formatter.py
--rw-r--r--   0 runner    (1001) docker     (123)      618 2023-04-29 18:21:11.000000 discord-qalib-2.2.1/qalib/template_engines/jinja2.py
--rw-r--r--   0 runner    (1001) docker     (123)      481 2023-04-29 18:21:11.000000 discord-qalib-2.2.1/qalib/template_engines/template_engine.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-29 18:21:38.020867 discord-qalib-2.2.1/qalib/translators/
--rw-r--r--   0 runner    (1001) docker     (123)     5373 2023-04-29 18:21:11.000000 discord-qalib-2.2.1/qalib/translators/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1474 2023-04-29 18:21:11.000000 discord-qalib-2.2.1/qalib/translators/deserializer.py
--rw-r--r--   0 runner    (1001) docker     (123)     2776 2023-04-29 18:21:11.000000 discord-qalib-2.2.1/qalib/translators/factory.py
--rw-r--r--   0 runner    (1001) docker     (123)    26234 2023-04-29 18:21:11.000000 discord-qalib-2.2.1/qalib/translators/json.py
--rw-r--r--   0 runner    (1001) docker     (123)    14333 2023-04-29 18:21:11.000000 discord-qalib-2.2.1/qalib/translators/message_parsing.py
--rw-r--r--   0 runner    (1001) docker     (123)     1125 2023-04-29 18:21:11.000000 discord-qalib-2.2.1/qalib/translators/templater.py
--rw-r--r--   0 runner    (1001) docker     (123)    30812 2023-04-29 18:21:11.000000 discord-qalib-2.2.1/qalib/translators/xml.py
--rw-r--r--   0 runner    (1001) docker     (123)      149 2023-04-29 18:21:11.000000 discord-qalib-2.2.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-29 18:21:38.020867 discord-qalib-2.2.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      572 2023-04-29 18:21:27.000000 discord-qalib-2.2.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 16:45:39.025977 discord-qalib-2.2.2/
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-05-05 16:45:04.000000 discord-qalib-2.2.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4841 2023-05-05 16:45:39.025977 discord-qalib-2.2.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4162 2023-05-05 16:45:04.000000 discord-qalib-2.2.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 16:45:39.021977 discord-qalib-2.2.2/discord_qalib.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4841 2023-05-05 16:45:39.000000 discord-qalib-2.2.2/discord_qalib.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      689 2023-05-05 16:45:39.000000 discord-qalib-2.2.2/discord_qalib.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 16:45:39.000000 discord-qalib-2.2.2/discord_qalib.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      150 2023-05-05 16:45:39.000000 discord-qalib-2.2.2/discord_qalib.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-05 16:45:39.000000 discord-qalib-2.2.2/discord_qalib.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1459 2023-05-05 16:45:25.000000 discord-qalib-2.2.2/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 16:45:39.021977 discord-qalib-2.2.2/qalib/
+-rw-r--r--   0 runner    (1001) docker     (123)     3736 2023-05-05 16:45:25.000000 discord-qalib-2.2.2/qalib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6030 2023-05-05 16:45:04.000000 discord-qalib-2.2.2/qalib/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7380 2023-05-05 16:45:04.000000 discord-qalib-2.2.2/qalib/interaction.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 16:45:04.000000 discord-qalib-2.2.2/qalib/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)     3091 2023-05-05 16:45:04.000000 discord-qalib-2.2.2/qalib/renderer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 16:45:39.021977 discord-qalib-2.2.2/qalib/template_engines/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 16:45:04.000000 discord-qalib-2.2.2/qalib/template_engines/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1290 2023-05-05 16:45:04.000000 discord-qalib-2.2.2/qalib/template_engines/formatter.py
+-rw-r--r--   0 runner    (1001) docker     (123)      618 2023-05-05 16:45:04.000000 discord-qalib-2.2.2/qalib/template_engines/jinja2.py
+-rw-r--r--   0 runner    (1001) docker     (123)      481 2023-05-05 16:45:04.000000 discord-qalib-2.2.2/qalib/template_engines/template_engine.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 16:45:39.025977 discord-qalib-2.2.2/qalib/translators/
+-rw-r--r--   0 runner    (1001) docker     (123)     5569 2023-05-05 16:45:04.000000 discord-qalib-2.2.2/qalib/translators/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1474 2023-05-05 16:45:04.000000 discord-qalib-2.2.2/qalib/translators/deserializer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2776 2023-05-05 16:45:04.000000 discord-qalib-2.2.2/qalib/translators/factory.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26234 2023-05-05 16:45:04.000000 discord-qalib-2.2.2/qalib/translators/json.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14333 2023-05-05 16:45:04.000000 discord-qalib-2.2.2/qalib/translators/message_parsing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1125 2023-05-05 16:45:04.000000 discord-qalib-2.2.2/qalib/translators/templater.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30812 2023-05-05 16:45:04.000000 discord-qalib-2.2.2/qalib/translators/xml.py
+-rw-r--r--   0 runner    (1001) docker     (123)      149 2023-05-05 16:45:04.000000 discord-qalib-2.2.2/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-05 16:45:39.025977 discord-qalib-2.2.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      572 2023-05-05 16:45:25.000000 discord-qalib-2.2.2/setup.py
```

### Comparing `discord-qalib-2.2.1/LICENSE` & `discord-qalib-2.2.2/LICENSE`

 * *Files identical despite different names*

### Comparing `discord-qalib-2.2.1/PKG-INFO` & `discord-qalib-2.2.2/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: discord-qalib
-Version: 2.2.1
+Version: 2.2.2
 Summary: Discord library built on discord.py to simplify source code by rendering templates of embeds and menus
 Home-page: https://github.com/YousefEZ/discord-qalib
 Author: Yousef Zaher
 Author-email: YousefEZ <syberprojects@gmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/YousefEZ/discord-qalib
 Project-URL: Bug Tracker, https://github.com/YousefEZ/discord-qalib/issues
@@ -94,18 +94,20 @@
             <author>
                 <name>Test Author</name>
                 <icon>https://cdn.discordapp.com/embed/avatars/0.png</icon>
                 <url>https://discordapp.com</url>
             </author>
         </embed>
         <view>
-            <button key="understood_button">
-                <label>Understood</label>
-                <style>success</style>
-            </button>
+            <components>        
+                <button key="understood_button">
+                    <label>Understood</label>
+                    <style>success</style>
+                </button>
+            </components>
         </view>
     </message>
 </discord>
 ```
 
 using the above xml file, for example, you can create an embed with the following code:
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: discord-qalib Version: 2.2.1 Summary: Discord
+Metadata-Version: 2.1 Name: discord-qalib Version: 2.2.2 Summary: Discord
 library built on discord.py to simplify source code by rendering templates of
 embeds and menus Home-page: https://github.com/YousefEZ/discord-qalib Author:
 Yousef Zaher Author-email: YousefEZ
 gmail.com> License: MIT Project-URL: Homepage, https://github.com/YousefEZ/
 discord-qalib Project-URL: Bug Tracker, https://github.com/YousefEZ/discord-
 qalib/issues Classifier: Programming Language :: Python :: 3 Classifier:
 License :: OSI Approved :: MIT License Classifier: Operating System :: OS
@@ -31,16 +31,16 @@
 more detail in the [wiki](https://github.com/YousefEZ/discord-qalib/wiki)_ Wrap
 expressions that need to evaluated with ``{}``, such as ``{player.name}`` or ``
 {todays_date}`` Sample XML file: ```xml
 Test Description magenta {todays_date} https://www.discord.com   Test Field
 Test Text    Test Footer https://cdn.discordapp.com/embed/avatars/0.png  https:
 //cdn.discordapp.com/embed/avatars/0.png https://cdn.discordapp.com/embed/
 avatars/0.png  Test Author https://cdn.discordapp.com/embed/avatars/0.png
-https://discordapp.com     Understood
-     ``` using the above xml file, for example, you can create an embed with
+https://discordapp.com      Understood
+      ``` using the above xml file, for example, you can create an embed with
 the following code: ```python import datetime from typing import Literal import
 discord from discord.ext import commands import qalib from
 qalib.template_engines import formatter bot = commands.AutoShardedBot
 (command_prefix="!", intents=discord.Intents.all()) Messages = Literal
 ["test_key"] async def acknowledged(interaction: discord.Interaction): await
 interaction.response.send_message("Acknowledged", ephemeral=True) @bot.command
 () @qalib.qalib_context(formatter.Formatter(), "templates/test.xml") async def
```

### Comparing `discord-qalib-2.2.1/README.md` & `discord-qalib-2.2.2/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -77,18 +77,20 @@
             <author>
                 <name>Test Author</name>
                 <icon>https://cdn.discordapp.com/embed/avatars/0.png</icon>
                 <url>https://discordapp.com</url>
             </author>
         </embed>
         <view>
-            <button key="understood_button">
-                <label>Understood</label>
-                <style>success</style>
-            </button>
+            <components>        
+                <button key="understood_button">
+                    <label>Understood</label>
+                    <style>success</style>
+                </button>
+            </components>
         </view>
     </message>
 </discord>
 ```
 
 using the above xml file, for example, you can create an embed with the following code:
```

#### html2text {}

```diff
@@ -21,16 +21,16 @@
 more detail in the [wiki](https://github.com/YousefEZ/discord-qalib/wiki)_ Wrap
 expressions that need to evaluated with ``{}``, such as ``{player.name}`` or ``
 {todays_date}`` Sample XML file: ```xml
 Test Description magenta {todays_date} https://www.discord.com   Test Field
 Test Text    Test Footer https://cdn.discordapp.com/embed/avatars/0.png  https:
 //cdn.discordapp.com/embed/avatars/0.png https://cdn.discordapp.com/embed/
 avatars/0.png  Test Author https://cdn.discordapp.com/embed/avatars/0.png
-https://discordapp.com     Understood
-     ``` using the above xml file, for example, you can create an embed with
+https://discordapp.com      Understood
+      ``` using the above xml file, for example, you can create an embed with
 the following code: ```python import datetime from typing import Literal import
 discord from discord.ext import commands import qalib from
 qalib.template_engines import formatter bot = commands.AutoShardedBot
 (command_prefix="!", intents=discord.Intents.all()) Messages = Literal
 ["test_key"] async def acknowledged(interaction: discord.Interaction): await
 interaction.response.send_message("Acknowledged", ephemeral=True) @bot.command
 () @qalib.qalib_context(formatter.Formatter(), "templates/test.xml") async def
```

### Comparing `discord-qalib-2.2.1/discord_qalib.egg-info/PKG-INFO` & `discord-qalib-2.2.2/discord_qalib.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: discord-qalib
-Version: 2.2.1
+Version: 2.2.2
 Summary: Discord library built on discord.py to simplify source code by rendering templates of embeds and menus
 Home-page: https://github.com/YousefEZ/discord-qalib
 Author: Yousef Zaher
 Author-email: YousefEZ <syberprojects@gmail.com>
 License: MIT
 Project-URL: Homepage, https://github.com/YousefEZ/discord-qalib
 Project-URL: Bug Tracker, https://github.com/YousefEZ/discord-qalib/issues
@@ -94,18 +94,20 @@
             <author>
                 <name>Test Author</name>
                 <icon>https://cdn.discordapp.com/embed/avatars/0.png</icon>
                 <url>https://discordapp.com</url>
             </author>
         </embed>
         <view>
-            <button key="understood_button">
-                <label>Understood</label>
-                <style>success</style>
-            </button>
+            <components>        
+                <button key="understood_button">
+                    <label>Understood</label>
+                    <style>success</style>
+                </button>
+            </components>
         </view>
     </message>
 </discord>
 ```
 
 using the above xml file, for example, you can create an embed with the following code:
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: discord-qalib Version: 2.2.1 Summary: Discord
+Metadata-Version: 2.1 Name: discord-qalib Version: 2.2.2 Summary: Discord
 library built on discord.py to simplify source code by rendering templates of
 embeds and menus Home-page: https://github.com/YousefEZ/discord-qalib Author:
 Yousef Zaher Author-email: YousefEZ
 gmail.com> License: MIT Project-URL: Homepage, https://github.com/YousefEZ/
 discord-qalib Project-URL: Bug Tracker, https://github.com/YousefEZ/discord-
 qalib/issues Classifier: Programming Language :: Python :: 3 Classifier:
 License :: OSI Approved :: MIT License Classifier: Operating System :: OS
@@ -31,16 +31,16 @@
 more detail in the [wiki](https://github.com/YousefEZ/discord-qalib/wiki)_ Wrap
 expressions that need to evaluated with ``{}``, such as ``{player.name}`` or ``
 {todays_date}`` Sample XML file: ```xml
 Test Description magenta {todays_date} https://www.discord.com   Test Field
 Test Text    Test Footer https://cdn.discordapp.com/embed/avatars/0.png  https:
 //cdn.discordapp.com/embed/avatars/0.png https://cdn.discordapp.com/embed/
 avatars/0.png  Test Author https://cdn.discordapp.com/embed/avatars/0.png
-https://discordapp.com     Understood
-     ``` using the above xml file, for example, you can create an embed with
+https://discordapp.com      Understood
+      ``` using the above xml file, for example, you can create an embed with
 the following code: ```python import datetime from typing import Literal import
 discord from discord.ext import commands import qalib from
 qalib.template_engines import formatter bot = commands.AutoShardedBot
 (command_prefix="!", intents=discord.Intents.all()) Messages = Literal
 ["test_key"] async def acknowledged(interaction: discord.Interaction): await
 interaction.response.send_message("Acknowledged", ephemeral=True) @bot.command
 () @qalib.qalib_context(formatter.Formatter(), "templates/test.xml") async def
```

### Comparing `discord-qalib-2.2.1/discord_qalib.egg-info/SOURCES.txt` & `discord-qalib-2.2.2/discord_qalib.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `discord-qalib-2.2.1/pyproject.toml` & `discord-qalib-2.2.2/pyproject.toml`

 * *Files 6% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "discord-qalib"
-version = "2.2.1"
+version = "2.2.2"
 authors = [
     { name = "YousefEZ", email = "syberprojects@gmail.com" },
 ]
 description = "Discord library built on discord.py to simplify source code by rendering templates of embeds and menus"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
@@ -16,15 +16,15 @@
     "License :: OSI Approved :: MIT License",
     "Operating System :: OS Independent",
 ]
 dynamic = ["dependencies"]
 
 [tool.poetry]
 name = "discord-qalib"
-version = "2.2.1"
+version = "2.2.2"
 authors = ["YousefEZ syberprojects@gmail.com", ]
 description = "Discord library built on discord.py to simplify source code by rendering templates of embeds and menus"
 packages = [{ include = "qalib" }]
 
 [tool.pylint.messages_control]
 max-line-length = 120
 disable = [
```

### Comparing `discord-qalib-2.2.1/qalib/__init__.py` & `discord-qalib-2.2.2/qalib/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 from .template_engines.jinja2 import Jinja2
 from .template_engines.template_engine import TemplateEngine
 
 __title__ = "qalib"
 __author__ = "YousefEZ"
 __license__ = "MIT"
 __copyright__ = "Copyright 2022-present YousefEZ"
-__version__ = "2.2.1"
+__version__ = "2.2.2"
 
 T = TypeVar("T")
 Coro = Coroutine[Any, Any, T]
 
 
 def qalib_context(
         template_engine: TemplateEngine, filename: str, *renderer_options: RenderingOptions
```

### Comparing `discord-qalib-2.2.1/qalib/context.py` & `discord-qalib-2.2.2/qalib/context.py`

 * *Files identical despite different names*

### Comparing `discord-qalib-2.2.1/qalib/interaction.py` & `discord-qalib-2.2.2/qalib/interaction.py`

 * *Files identical despite different names*

### Comparing `discord-qalib-2.2.1/qalib/renderer.py` & `discord-qalib-2.2.2/qalib/renderer.py`

 * *Files identical despite different names*

### Comparing `discord-qalib-2.2.1/qalib/template_engines/formatter.py` & `discord-qalib-2.2.2/qalib/template_engines/formatter.py`

 * *Files identical despite different names*

### Comparing `discord-qalib-2.2.1/qalib/template_engines/jinja2.py` & `discord-qalib-2.2.2/qalib/template_engines/jinja2.py`

 * *Files identical despite different names*

### Comparing `discord-qalib-2.2.1/qalib/translators/__init__.py` & `discord-qalib-2.2.2/qalib/translators/__init__.py`

 * *Files 18% similar despite different names*

```diff
@@ -25,52 +25,52 @@
 class Base:
     def dict(self) -> Dict[str, Any]:
         return {key.name: attr for key in fields(self) if (attr := getattr(self, key.name)) is not None}
 
 
 @dataclass
 class BaseEditMessage(Base):
-    content: Optional[str]
-    embed: Optional[discord.Embed]
-    attachments: Optional[Sequence[Union[discord.Attachment, discord.File]]]
-    delete_after: Optional[float]
-    allowed_mentions: Optional[discord.AllowedMentions]
-    view: Optional[discord.ui.View]
+    content: Optional[str] = None
+    embed: Optional[discord.Embed] = None
+    attachments: Optional[Sequence[Union[discord.Attachment, discord.File]]] = None
+    delete_after: Optional[float] = None
+    allowed_mentions: Optional[discord.AllowedMentions] = None
+    view: Optional[discord.ui.View] = None
 
 
 # pylint: disable= too-many-instance-attributes
 @dataclass
 class BaseMessage(Base):
-    content: Optional[str]
-    embed: Optional[discord.Embed]
-    embeds: Optional[Sequence[discord.Embed]]
-    file: Optional[discord.File]
-    files: Optional[Sequence[discord.File]]
-    view: Optional[discord.ui.View]
-    tts: Optional[bool]
-    ephemeral: Optional[bool]
-    allowed_mentions: Optional[discord.AllowedMentions]
-    suppress_embeds: Optional[bool]
-    delete_after: Optional[float]
+    content: Optional[str] = None
+    embed: Optional[discord.Embed] = None
+    embeds: Optional[Sequence[discord.Embed]] = None
+    file: Optional[discord.File] = None
+    files: Optional[Sequence[discord.File]] = None
+    view: Optional[discord.ui.View] = None
+    tts: Optional[bool] = None
+    ephemeral: Optional[bool] = None
+    allowed_mentions: Optional[discord.AllowedMentions] = None
+    suppress_embeds: Optional[bool] = None
+    delete_after: Optional[float] = None
 
     def as_edit(self) -> BaseEditMessage:
         raise NotImplementedError
 
 
 @dataclass
 class EditContextMessage(BaseEditMessage):
-    suppress: Optional[bool]
+    suppress: Optional[bool] = None
 
 
 @dataclass
 class ContextMessage(BaseMessage):
-    stickers: Optional[Sequence[Union[discord.GuildSticker, discord.StickerItem]]]
-    nonce: Optional[Union[str, int]]
-    reference: Optional[Union[discord.Message, discord.MessageReference, discord.PartialMessage]]
-    mention_author: Optional[bool]
+    stickers: Optional[Sequence[Union[discord.GuildSticker, discord.StickerItem]]] = None
+    nonce: Optional[Union[str, int]] = None
+    reference: Optional[Union[discord.Message, discord.MessageReference, discord.PartialMessage]] = None
+    mention_author: Optional[bool] = None
 
     def as_edit(self) -> EditContextMessage:
         return EditContextMessage(
             content=self.content,
             embed=self.embed,
             attachments=self.files,
             suppress=self.suppress_embeds,
@@ -83,15 +83,15 @@
 @dataclass
 class InteractionEditMessage(BaseEditMessage):
     pass
 
 
 @dataclass
 class InteractionMessage(BaseMessage):
-    silent: Optional[bool]
+    silent: Optional[bool] = None
 
     def as_edit(self) -> InteractionEditMessage:
         return InteractionEditMessage(
             content=self.content,
             embed=self.embed,
             attachments=self.files,
             delete_after=self.delete_after,
@@ -123,19 +123,19 @@
 @dataclass
 class Message(BaseMessage):
     """Dataclass that represents the display of the message.
 
     Look at https://discordpy.readthedocs.io/en/latest/api.html?highlight=send#discord.abc.Messageable.send
     """
 
-    stickers: Optional[Sequence[Union[discord.GuildSticker, discord.StickerItem]]]
-    nonce: Optional[Union[str, int]]
-    reference: Optional[Union[discord.Message, discord.MessageReference, discord.PartialMessage]]
-    mention_author: Optional[bool]
-    silent: Optional[bool]
+    stickers: Optional[Sequence[Union[discord.GuildSticker, discord.StickerItem]]] = None
+    nonce: Optional[Union[str, int]] = None
+    reference: Optional[Union[discord.Message, discord.MessageReference, discord.PartialMessage]] = None
+    mention_author: Optional[bool] = None
+    silent: Optional[bool] = None
 
     def convert_to_context_message(self) -> ContextMessage:
         return ContextMessage(
             content=self.content,
             embed=self.embed,
             embeds=self.embeds,
             file=self.file,
```

### Comparing `discord-qalib-2.2.1/qalib/translators/deserializer.py` & `discord-qalib-2.2.2/qalib/translators/deserializer.py`

 * *Files identical despite different names*

### Comparing `discord-qalib-2.2.1/qalib/translators/factory.py` & `discord-qalib-2.2.2/qalib/translators/factory.py`

 * *Files identical despite different names*

### Comparing `discord-qalib-2.2.1/qalib/translators/json.py` & `discord-qalib-2.2.2/qalib/translators/json.py`

 * *Files identical despite different names*

### Comparing `discord-qalib-2.2.1/qalib/translators/message_parsing.py` & `discord-qalib-2.2.2/qalib/translators/message_parsing.py`

 * *Files identical despite different names*

### Comparing `discord-qalib-2.2.1/qalib/translators/templater.py` & `discord-qalib-2.2.2/qalib/translators/templater.py`

 * *Files identical despite different names*

### Comparing `discord-qalib-2.2.1/qalib/translators/xml.py` & `discord-qalib-2.2.2/qalib/translators/xml.py`

 * *Files identical despite different names*

### Comparing `discord-qalib-2.2.1/setup.py` & `discord-qalib-2.2.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -4,15 +4,15 @@
     requirements = f.read().splitlines()
 
 setup(
     name="Discord-Qalib",
     author="Yousef Zaher",
     author_email="syberprojects@gmail.com",
     url="https://github.com/YousefEZ/discord-qalib",
-    version="2.2.1",
+    version="2.2.2",
     description="A library for templating responses on .xml, and .json files for discord.py",
     packages=find_packages(exclude=("test*",)),
     license="MIT",
     python_requires=">=3.8.0",
     install_requires=requirements,
     package_data={"qalib": ["py.typed"]},
 )
```

