# Comparing `tmp/discord-menu-0.8.1.tar.gz` & `tmp/discord-menu-0.9.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\discord-menu-0.8.1.tar", last modified: Tue Feb  2 07:57:48 2021, max compression
+gzip compressed data, was "dist\discord-menu-0.9.0.tar", last modified: Tue Feb  2 08:02:21 2021, max compression
```

## Comparing `discord-menu-0.8.1.tar` & `discord-menu-0.9.0.tar`

### file list

```diff
@@ -1,34 +1,34 @@
-drwxrwxrwx   0        0        0        0 2021-02-02 07:57:48.128005 discord-menu-0.8.1/
--rw-rw-rw-   0        0        0      568 2021-02-02 07:57:48.127004 discord-menu-0.8.1/PKG-INFO
--rw-rw-rw-   0        0        0       57 2021-01-12 01:46:25.000000 discord-menu-0.8.1/README.md
-drwxrwxrwx   0        0        0        0 2021-02-02 07:57:48.106986 discord-menu-0.8.1/discord_menu.egg-info/
--rw-rw-rw-   0        0        0      568 2021-02-02 07:57:47.000000 discord-menu-0.8.1/discord_menu.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      703 2021-02-02 07:57:48.000000 discord-menu-0.8.1/discord_menu.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2021-02-02 07:57:47.000000 discord-menu-0.8.1/discord_menu.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       17 2021-02-02 07:57:47.000000 discord-menu-0.8.1/discord_menu.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2021-02-02 07:57:48.110990 discord-menu-0.8.1/discordmenu/
--rw-rw-rw-   0        0        0        0 2021-01-12 02:09:53.000000 discord-menu-0.8.1/discordmenu/__init__.py
--rw-rw-rw-   0        0        0     2799 2021-02-02 07:25:42.000000 discord-menu-0.8.1/discordmenu/discord_client.py
-drwxrwxrwx   0        0        0        0 2021-02-02 07:57:48.118997 discord-menu-0.8.1/discordmenu/embed/
--rw-rw-rw-   0        0        0        0 2021-01-12 02:09:26.000000 discord-menu-0.8.1/discordmenu/embed/__init__.py
--rw-rw-rw-   0        0        0     1055 2021-01-16 23:27:49.000000 discord-menu-0.8.1/discordmenu/embed/base.py
--rw-rw-rw-   0        0        0     2396 2021-01-13 03:39:34.000000 discord-menu-0.8.1/discordmenu/embed/components.py
--rw-rw-rw-   0        0        0      595 2021-01-31 11:09:03.000000 discord-menu-0.8.1/discordmenu/embed/control.py
--rw-rw-rw-   0        0        0      248 2021-02-02 03:52:50.000000 discord-menu-0.8.1/discordmenu/embed/emoji.py
--rw-rw-rw-   0        0        0     3080 2021-02-02 07:56:12.000000 discord-menu-0.8.1/discordmenu/embed/menu.py
--rw-rw-rw-   0        0        0     3236 2021-01-17 22:28:36.000000 discord-menu-0.8.1/discordmenu/embed/text.py
--rw-rw-rw-   0        0        0     3331 2021-02-02 03:52:42.000000 discord-menu-0.8.1/discordmenu/embed/view.py
--rw-rw-rw-   0        0        0      533 2021-01-31 11:09:03.000000 discord-menu-0.8.1/discordmenu/embed/view_state.py
-drwxrwxrwx   0        0        0        0 2021-02-02 07:57:48.122000 discord-menu-0.8.1/discordmenu/emoji/
--rw-rw-rw-   0        0        0        0 2021-02-02 07:55:47.000000 discord-menu-0.8.1/discordmenu/emoji/__init__.py
--rw-rw-rw-   0        0        0      197 2021-02-02 07:53:49.000000 discord-menu-0.8.1/discordmenu/emoji/emoji.py
--rw-rw-rw-   0        0        0      945 2021-02-02 07:54:43.000000 discord-menu-0.8.1/discordmenu/emoji/emoji_cache.py
--rw-rw-rw-   0        0        0     2423 2021-01-11 00:36:31.000000 discord-menu-0.8.1/discordmenu/intra_message_state.py
--rw-rw-rw-   0        0        0     3433 2021-02-02 07:52:12.000000 discord-menu-0.8.1/discordmenu/reaction_filter.py
--rw-rw-rw-   0        0        0       42 2021-02-02 07:57:48.128005 discord-menu-0.8.1/setup.cfg
--rw-rw-rw-   0        0        0      745 2021-02-02 07:57:29.000000 discord-menu-0.8.1/setup.py
-drwxrwxrwx   0        0        0        0 2021-02-02 07:57:48.126004 discord-menu-0.8.1/test/
--rw-rw-rw-   0        0        0        0 2021-01-12 02:09:59.000000 discord-menu-0.8.1/test/__init__.py
--rw-rw-rw-   0        0        0     6445 2021-01-12 02:39:48.000000 discord-menu-0.8.1/test/test_embed.py
--rw-rw-rw-   0        0        0     1650 2021-01-12 02:39:48.000000 discord-menu-0.8.1/test/test_menu.py
--rw-rw-rw-   0        0        0     1935 2021-01-12 02:39:48.000000 discord-menu-0.8.1/test/test_reactions.py
+drwxrwxrwx   0        0        0        0 2021-02-02 08:02:21.634906 discord-menu-0.9.0/
+-rw-rw-rw-   0        0        0      568 2021-02-02 08:02:21.634906 discord-menu-0.9.0/PKG-INFO
+-rw-rw-rw-   0        0        0       57 2021-01-12 01:46:25.000000 discord-menu-0.9.0/README.md
+drwxrwxrwx   0        0        0        0 2021-02-02 08:02:21.615511 discord-menu-0.9.0/discord_menu.egg-info/
+-rw-rw-rw-   0        0        0      568 2021-02-02 08:02:21.000000 discord-menu-0.9.0/discord_menu.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      703 2021-02-02 08:02:21.000000 discord-menu-0.9.0/discord_menu.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2021-02-02 08:02:21.000000 discord-menu-0.9.0/discord_menu.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       17 2021-02-02 08:02:21.000000 discord-menu-0.9.0/discord_menu.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2021-02-02 08:02:21.618432 discord-menu-0.9.0/discordmenu/
+-rw-rw-rw-   0        0        0        0 2021-01-12 02:09:53.000000 discord-menu-0.9.0/discordmenu/__init__.py
+-rw-rw-rw-   0        0        0     2805 2021-02-02 07:59:26.000000 discord-menu-0.9.0/discordmenu/discord_client.py
+drwxrwxrwx   0        0        0        0 2021-02-02 08:02:21.627441 discord-menu-0.9.0/discordmenu/embed/
+-rw-rw-rw-   0        0        0        0 2021-01-12 02:09:26.000000 discord-menu-0.9.0/discordmenu/embed/__init__.py
+-rw-rw-rw-   0        0        0     1055 2021-01-16 23:27:49.000000 discord-menu-0.9.0/discordmenu/embed/base.py
+-rw-rw-rw-   0        0        0     2396 2021-01-13 03:39:34.000000 discord-menu-0.9.0/discordmenu/embed/components.py
+-rw-rw-rw-   0        0        0      595 2021-01-31 11:09:03.000000 discord-menu-0.9.0/discordmenu/embed/control.py
+-rw-rw-rw-   0        0        0      248 2021-02-02 03:52:50.000000 discord-menu-0.9.0/discordmenu/embed/emoji.py
+-rw-rw-rw-   0        0        0     3080 2021-02-02 07:56:12.000000 discord-menu-0.9.0/discordmenu/embed/menu.py
+-rw-rw-rw-   0        0        0     3236 2021-01-17 22:28:36.000000 discord-menu-0.9.0/discordmenu/embed/text.py
+-rw-rw-rw-   0        0        0     3331 2021-02-02 03:52:42.000000 discord-menu-0.9.0/discordmenu/embed/view.py
+-rw-rw-rw-   0        0        0      533 2021-01-31 11:09:03.000000 discord-menu-0.9.0/discordmenu/embed/view_state.py
+drwxrwxrwx   0        0        0        0 2021-02-02 08:02:21.630444 discord-menu-0.9.0/discordmenu/emoji/
+-rw-rw-rw-   0        0        0        0 2021-02-02 07:55:47.000000 discord-menu-0.9.0/discordmenu/emoji/__init__.py
+-rw-rw-rw-   0        0        0      197 2021-02-02 07:53:49.000000 discord-menu-0.9.0/discordmenu/emoji/emoji.py
+-rw-rw-rw-   0        0        0      945 2021-02-02 07:54:43.000000 discord-menu-0.9.0/discordmenu/emoji/emoji_cache.py
+-rw-rw-rw-   0        0        0     2423 2021-01-11 00:36:31.000000 discord-menu-0.9.0/discordmenu/intra_message_state.py
+-rw-rw-rw-   0        0        0     3383 2021-02-02 08:01:52.000000 discord-menu-0.9.0/discordmenu/reaction_filter.py
+-rw-rw-rw-   0        0        0       42 2021-02-02 08:02:21.634906 discord-menu-0.9.0/setup.cfg
+-rw-rw-rw-   0        0        0      745 2021-02-02 08:02:15.000000 discord-menu-0.9.0/setup.py
+drwxrwxrwx   0        0        0        0 2021-02-02 08:02:21.633904 discord-menu-0.9.0/test/
+-rw-rw-rw-   0        0        0        0 2021-01-12 02:09:59.000000 discord-menu-0.9.0/test/__init__.py
+-rw-rw-rw-   0        0        0     6445 2021-01-12 02:39:48.000000 discord-menu-0.9.0/test/test_embed.py
+-rw-rw-rw-   0        0        0     1656 2021-02-02 08:00:38.000000 discord-menu-0.9.0/test/test_menu.py
+-rw-rw-rw-   0        0        0     1935 2021-01-12 02:39:48.000000 discord-menu-0.9.0/test/test_reactions.py
```

### Comparing `discord-menu-0.8.1/PKG-INFO` & `discord-menu-0.9.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: discord-menu
-Version: 0.8.1
+Version: 0.9.0
 Summary: A library to create tabbed menus in Discord messages
 Home-page: https://github.com/TsubakiBotPad/discord-menu
 Author: The Tsubotki Team
 Author-email: 69992611+TsubakiBotPad@users.noreply.github.com
 License: Apache-2.0 License
 Description: # discord-menu
         Create tabbed menus in Discord messages
```

### Comparing `discord-menu-0.8.1/discord_menu.egg-info/PKG-INFO` & `discord-menu-0.9.0/discord_menu.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: discord-menu
-Version: 0.8.1
+Version: 0.9.0
 Summary: A library to create tabbed menus in Discord messages
 Home-page: https://github.com/TsubakiBotPad/discord-menu
 Author: The Tsubotki Team
 Author-email: 69992611+TsubakiBotPad@users.noreply.github.com
 License: Apache-2.0 License
 Description: # discord-menu
         Create tabbed menus in Discord messages
```

### Comparing `discord-menu-0.8.1/discord_menu.egg-info/SOURCES.txt` & `discord-menu-0.9.0/discord_menu.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `discord-menu-0.8.1/discordmenu/discord_client.py` & `discord-menu-0.9.0/discordmenu/discord_client.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 import asyncio
 from typing import Dict, List, Optional
 
 from discord import Embed, Emoji, Forbidden, Message, Reaction
 
 from discordmenu.embed.control import EmbedControl
-from discordmenu.emoji_cache import emoji_cache
+from discordmenu.emoji.emoji_cache import emoji_cache
 
 
 async def update_message(message: Message, updated_messaged_contents, guild_message: bool,
                          emoji_diff: Dict[str, List[Emoji]] = None):
     if isinstance(updated_messaged_contents, Embed):
         await message.edit(embed=updated_messaged_contents)
     else:
```

### Comparing `discord-menu-0.8.1/discordmenu/embed/base.py` & `discord-menu-0.9.0/discordmenu/embed/base.py`

 * *Files identical despite different names*

### Comparing `discord-menu-0.8.1/discordmenu/embed/components.py` & `discord-menu-0.9.0/discordmenu/embed/components.py`

 * *Files identical despite different names*

### Comparing `discord-menu-0.8.1/discordmenu/embed/control.py` & `discord-menu-0.9.0/discordmenu/embed/control.py`

 * *Files identical despite different names*

### Comparing `discord-menu-0.8.1/discordmenu/embed/menu.py` & `discord-menu-0.9.0/discordmenu/embed/menu.py`

 * *Files identical despite different names*

### Comparing `discord-menu-0.8.1/discordmenu/embed/text.py` & `discord-menu-0.9.0/discordmenu/embed/text.py`

 * *Files identical despite different names*

### Comparing `discord-menu-0.8.1/discordmenu/embed/view.py` & `discord-menu-0.9.0/discordmenu/embed/view.py`

 * *Files identical despite different names*

### Comparing `discord-menu-0.8.1/discordmenu/embed/view_state.py` & `discord-menu-0.9.0/discordmenu/embed/view_state.py`

 * *Files identical despite different names*

### Comparing `discord-menu-0.8.1/discordmenu/emoji/emoji_cache.py` & `discord-menu-0.9.0/discordmenu/emoji/emoji_cache.py`

 * *Files identical despite different names*

### Comparing `discord-menu-0.8.1/discordmenu/intra_message_state.py` & `discord-menu-0.9.0/discordmenu/intra_message_state.py`

 * *Files identical despite different names*

### Comparing `discord-menu-0.8.1/discordmenu/reaction_filter.py` & `discord-menu-0.9.0/discordmenu/reaction_filter.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 from collections.abc import Iterable
 from typing import Optional
 
 from discord import Reaction, Message, Member, RawReactionActionEvent
 
 from discordmenu.embed.emoji import DEFAULT_EMBED_MENU_EMOJI_CONFIG, EmbedMenuEmojiConfig
-from discordmenu.emoji_cache import discord_emoji_to_emoji_name
+from discordmenu.emoji.emoji import discord_emoji_to_emoji_name
 
 
 class ReactionFilter:
     def __init__(self, reaction_filter: Optional["ReactionFilter"] = None):
         self.inner_filter: ReactionFilter = reaction_filter
 
     async def allow_reaction(self, message: Message, reaction: Reaction, member: Member):
@@ -39,15 +39,14 @@
         default_emojis = default_emoji_override or DEFAULT_EMBED_MENU_EMOJI_CONFIG
         emoji_set = set(default_emojis.to_list())
         emoji_set.update(valid_emoji_names)
         self.valid_emoji_names = list(emoji_set)
 
     async def _allow_reaction(self, message: Message, reaction: Reaction, member: Member):
         valid_emoji_reaction = discord_emoji_to_emoji_name(reaction.emoji) in self.valid_emoji_names
-        print("valid emo", valid_emoji_reaction)
         return valid_emoji_reaction
 
     async def _allow_reaction_raw(self, message: Message, reaction: RawReactionActionEvent):
         valid_emoji_reaction = discord_emoji_to_emoji_name(reaction.emoji) in self.valid_emoji_names
         return valid_emoji_reaction
```

### Comparing `discord-menu-0.8.1/setup.py` & `discord-menu-0.9.0/setup.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="discord-menu",
-    version="0.8.1",
+    version="0.9.0",
     author="The Tsubotki Team",
     author_email="69992611+TsubakiBotPad@users.noreply.github.com",
     license="Apache-2.0 License",
     description="A library to create tabbed menus in Discord messages",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/TsubakiBotPad/discord-menu",
```

### Comparing `discord-menu-0.8.1/test/test_embed.py` & `discord-menu-0.9.0/test/test_embed.py`

 * *Files identical despite different names*

### Comparing `discord-menu-0.8.1/test/test_menu.py` & `discord-menu-0.9.0/test/test_menu.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from discordmenu.discord_client import send_embed_control
 from discordmenu.embed.menu import EmbedMenu, EmbedControl
-from discordmenu.emoji_cache import EmojiCache
+from discordmenu.emoji.emoji_cache import EmojiCache
 from discordmenu.reaction_filter import ValidEmojiReactionFilter, NotPosterEmojiReactionFilter, \
     MessageOwnerReactionFilter
 from discordmenu.test_embed import embed_view
 
 c = EmojiCache([713430119343063182])
```

### Comparing `discord-menu-0.8.1/test/test_reactions.py` & `discord-menu-0.9.0/test/test_reactions.py`

 * *Files identical despite different names*

