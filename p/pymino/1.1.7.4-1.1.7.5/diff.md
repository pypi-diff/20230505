# Comparing `tmp/pymino-1.1.7.4.tar.gz` & `tmp/pymino-1.1.7.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "C:\Users\12095\Desktop\pymino-1.1.7.4\dist\.tmp-bygfcxlr\pymino-1.1.7.4.tar", last modified: Thu Apr 13 01:05:09 2023, max compression
+gzip compressed data, was "C:\Users\12095\Desktop\submit v2\pymino-1.1.7.4\dist\.tmp-w_q_2xun\pymino-1.1.7.5.tar", last modified: Fri May  5 19:28:17 2023, max compression
```

## Comparing `pymino-1.1.7.4.tar` & `pymino-1.1.7.5.tar`

### file list

```diff
@@ -1,38 +1,38 @@
-drwxrwxrwx   0        0        0        0 2023-04-13 01:05:09.349109 pymino-1.1.7.4/
--rw-rw-rw-   0        0        0     1085 2023-02-11 18:40:37.000000 pymino-1.1.7.4/LICENSE
--rw-rw-rw-   0        0        0     6082 2023-04-13 01:05:09.349109 pymino-1.1.7.4/PKG-INFO
--rw-rw-rw-   0        0        0     5364 2023-03-09 02:27:22.000000 pymino-1.1.7.4/README.md
-drwxrwxrwx   0        0        0        0 2023-04-13 01:05:09.289068 pymino-1.1.7.4/pymino/
--rw-rw-rw-   0        0        0      676 2023-04-13 01:04:24.000000 pymino-1.1.7.4/pymino/__init__.py
--rw-rw-rw-   0        0        0    26133 2023-04-03 18:49:59.000000 pymino-1.1.7.4/pymino/bot.py
--rw-rw-rw-   0        0        0    48170 2023-04-13 01:03:38.000000 pymino-1.1.7.4/pymino/client.py
-drwxrwxrwx   0        0        0        0 2023-04-13 01:05:09.331723 pymino-1.1.7.4/pymino/ext/
--rw-rw-rw-   0        0        0      372 2023-02-10 13:25:37.000000 pymino-1.1.7.4/pymino/ext/__init__.py
--rw-rw-rw-   0        0        0    11206 2023-04-13 00:39:17.000000 pymino-1.1.7.4/pymino/ext/account.py
--rw-rw-rw-   0        0        0   271440 2023-04-13 01:04:28.000000 pymino-1.1.7.4/pymino/ext/community.py
--rw-rw-rw-   0        0        0    39378 2023-03-05 23:08:15.000000 pymino-1.1.7.4/pymino/ext/context.py
--rw-rw-rw-   0        0        0      871 2023-03-04 01:25:46.000000 pymino-1.1.7.4/pymino/ext/dispatcher.py
-drwxrwxrwx   0        0        0        0 2023-04-13 01:05:09.342139 pymino-1.1.7.4/pymino/ext/entities/
--rw-rw-rw-   0        0        0      198 2023-03-05 23:07:04.000000 pymino-1.1.7.4/pymino/ext/entities/__init__.py
--rw-rw-rw-   0        0        0      765 2023-03-05 16:56:17.000000 pymino-1.1.7.4/pymino/ext/entities/enums.py
--rw-rw-rw-   0        0        0    14506 2023-03-10 06:04:42.000000 pymino-1.1.7.4/pymino/ext/entities/exceptions.py
--rw-rw-rw-   0        0        0    48713 2023-02-25 04:12:35.000000 pymino-1.1.7.4/pymino/ext/entities/general.py
--rw-rw-rw-   0        0        0     2536 2023-03-03 22:30:34.000000 pymino-1.1.7.4/pymino/ext/entities/handlers.py
--rw-rw-rw-   0        0        0    42816 2023-02-06 10:45:41.000000 pymino-1.1.7.4/pymino/ext/entities/messages.py
--rw-rw-rw-   0        0        0     6109 2023-02-10 17:39:14.000000 pymino-1.1.7.4/pymino/ext/entities/threads.py
--rw-rw-rw-   0        0        0    31609 2023-02-13 01:22:30.000000 pymino-1.1.7.4/pymino/ext/entities/userprofile.py
--rw-rw-rw-   0        0        0     2230 2023-03-05 23:07:39.000000 pymino-1.1.7.4/pymino/ext/entities/wsevents.py
--rw-rw-rw-   0        0        0     7414 2023-03-03 22:30:22.000000 pymino-1.1.7.4/pymino/ext/socket.py
-drwxrwxrwx   0        0        0        0 2023-04-13 01:05:09.348091 pymino-1.1.7.4/pymino/ext/utilities/
--rw-rw-rw-   0        0        0       80 2023-03-04 01:08:01.000000 pymino-1.1.7.4/pymino/ext/utilities/__init__.py
--rw-rw-rw-   0        0        0     6396 2023-03-02 00:41:30.000000 pymino-1.1.7.4/pymino/ext/utilities/commands.py
--rw-rw-rw-   0        0        0     1110 2023-02-28 16:10:43.000000 pymino-1.1.7.4/pymino/ext/utilities/generate.py
--rw-rw-rw-   0        0        0    10274 2023-04-02 23:47:45.000000 pymino-1.1.7.4/pymino/ext/utilities/request_handler.py
-drwxrwxrwx   0        0        0        0 2023-04-13 01:05:09.304442 pymino-1.1.7.4/pymino.egg-info/
--rw-rw-rw-   0        0        0     6082 2023-04-13 01:05:09.000000 pymino-1.1.7.4/pymino.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      799 2023-04-13 01:05:09.000000 pymino-1.1.7.4/pymino.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-13 01:05:09.000000 pymino-1.1.7.4/pymino.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       87 2023-04-13 01:05:09.000000 pymino-1.1.7.4/pymino.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-04-13 01:05:09.000000 pymino-1.1.7.4/pymino.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      873 2023-04-13 01:05:09.354539 pymino-1.1.7.4/setup.cfg
--rw-rw-rw-   0        0        0     1340 2023-03-04 01:31:03.000000 pymino-1.1.7.4/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-05 19:28:17.030415 pymino-1.1.7.5/
+-rw-rw-rw-   0        0        0     1085 2023-02-11 18:40:37.000000 pymino-1.1.7.5/LICENSE
+-rw-rw-rw-   0        0        0     6082 2023-05-05 19:28:17.030415 pymino-1.1.7.5/PKG-INFO
+-rw-rw-rw-   0        0        0     5364 2023-03-09 02:27:22.000000 pymino-1.1.7.5/README.md
+drwxrwxrwx   0        0        0        0 2023-05-05 19:28:16.985278 pymino-1.1.7.5/pymino/
+-rw-rw-rw-   0        0        0      676 2023-05-05 19:27:51.000000 pymino-1.1.7.5/pymino/__init__.py
+-rw-rw-rw-   0        0        0    26133 2023-04-03 18:49:59.000000 pymino-1.1.7.5/pymino/bot.py
+-rw-rw-rw-   0        0        0    48170 2023-04-13 01:03:38.000000 pymino-1.1.7.5/pymino/client.py
+drwxrwxrwx   0        0        0        0 2023-05-05 19:28:17.011566 pymino-1.1.7.5/pymino/ext/
+-rw-rw-rw-   0        0        0      372 2023-02-10 13:25:37.000000 pymino-1.1.7.5/pymino/ext/__init__.py
+-rw-rw-rw-   0        0        0    11206 2023-04-13 00:39:17.000000 pymino-1.1.7.5/pymino/ext/account.py
+-rw-rw-rw-   0        0        0   271440 2023-04-13 01:04:28.000000 pymino-1.1.7.5/pymino/ext/community.py
+-rw-rw-rw-   0        0        0    39581 2023-05-05 19:27:29.000000 pymino-1.1.7.5/pymino/ext/context.py
+-rw-rw-rw-   0        0        0      871 2023-03-04 01:25:46.000000 pymino-1.1.7.5/pymino/ext/dispatcher.py
+drwxrwxrwx   0        0        0        0 2023-05-05 19:28:17.024462 pymino-1.1.7.5/pymino/ext/entities/
+-rw-rw-rw-   0        0        0      198 2023-03-05 23:07:04.000000 pymino-1.1.7.5/pymino/ext/entities/__init__.py
+-rw-rw-rw-   0        0        0      765 2023-03-05 16:56:17.000000 pymino-1.1.7.5/pymino/ext/entities/enums.py
+-rw-rw-rw-   0        0        0    14506 2023-03-10 06:04:42.000000 pymino-1.1.7.5/pymino/ext/entities/exceptions.py
+-rw-rw-rw-   0        0        0    48713 2023-02-25 04:12:35.000000 pymino-1.1.7.5/pymino/ext/entities/general.py
+-rw-rw-rw-   0        0        0     2536 2023-03-03 22:30:34.000000 pymino-1.1.7.5/pymino/ext/entities/handlers.py
+-rw-rw-rw-   0        0        0    42816 2023-02-06 10:45:41.000000 pymino-1.1.7.5/pymino/ext/entities/messages.py
+-rw-rw-rw-   0        0        0     6109 2023-02-10 17:39:14.000000 pymino-1.1.7.5/pymino/ext/entities/threads.py
+-rw-rw-rw-   0        0        0    31609 2023-02-13 01:22:30.000000 pymino-1.1.7.5/pymino/ext/entities/userprofile.py
+-rw-rw-rw-   0        0        0     2230 2023-03-05 23:07:39.000000 pymino-1.1.7.5/pymino/ext/entities/wsevents.py
+-rw-rw-rw-   0        0        0     7414 2023-03-03 22:30:22.000000 pymino-1.1.7.5/pymino/ext/socket.py
+drwxrwxrwx   0        0        0        0 2023-05-05 19:28:17.029422 pymino-1.1.7.5/pymino/ext/utilities/
+-rw-rw-rw-   0        0        0       80 2023-03-04 01:08:01.000000 pymino-1.1.7.5/pymino/ext/utilities/__init__.py
+-rw-rw-rw-   0        0        0     6396 2023-03-02 00:41:30.000000 pymino-1.1.7.5/pymino/ext/utilities/commands.py
+-rw-rw-rw-   0        0        0     1110 2023-02-28 16:10:43.000000 pymino-1.1.7.5/pymino/ext/utilities/generate.py
+-rw-rw-rw-   0        0        0    10274 2023-04-02 23:47:45.000000 pymino-1.1.7.5/pymino/ext/utilities/request_handler.py
+drwxrwxrwx   0        0        0        0 2023-05-05 19:28:17.003630 pymino-1.1.7.5/pymino.egg-info/
+-rw-rw-rw-   0        0        0     6082 2023-05-05 19:28:16.000000 pymino-1.1.7.5/pymino.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      799 2023-05-05 19:28:16.000000 pymino-1.1.7.5/pymino.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-05 19:28:16.000000 pymino-1.1.7.5/pymino.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       87 2023-05-05 19:28:16.000000 pymino-1.1.7.5/pymino.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-05-05 19:28:16.000000 pymino-1.1.7.5/pymino.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      873 2023-05-05 19:28:17.033886 pymino-1.1.7.5/setup.cfg
+-rw-rw-rw-   0        0        0     1340 2023-03-04 01:31:03.000000 pymino-1.1.7.5/setup.py
```

### Comparing `pymino-1.1.7.4/LICENSE` & `pymino-1.1.7.5/LICENSE`

 * *Files identical despite different names*

### Comparing `pymino-1.1.7.4/PKG-INFO` & `pymino-1.1.7.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pymino
-Version: 1.1.7.4
+Version: 1.1.7.5
 Summary: Easily create a bot for Amino Apps using a modern easy to use synchronous library.
 Home-page: https://github.com/forevercynical/pymino
 Author: forevercynical
 Author-email: me@cynical.gg
 License: MIT
 Keywords: amino,pymino,narvii,amino-api,narvii-bots,aminoapps,amino-bot,amino-bots
 Classifier: Programming Language :: Python :: 3
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pymino Version: 1.1.7.4 Summary: Easily create a
+Metadata-Version: 2.1 Name: pymino Version: 1.1.7.5 Summary: Easily create a
 bot for Amino Apps using a modern easy to use synchronous library. Home-page:
 https://github.com/forevercynical/pymino Author: forevercynical Author-email:
 me@cynical.gg License: MIT Keywords: amino,pymino,narvii,amino-api,narvii-
 bots,aminoapps,amino-bot,amino-bots Classifier: Programming Language :: Python
 :: 3 Classifier: Programming Language :: Python :: 3.7 Classifier: Programming
 Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
```

### Comparing `pymino-1.1.7.4/README.md` & `pymino-1.1.7.5/README.md`

 * *Files identical despite different names*

### Comparing `pymino-1.1.7.4/pymino/__init__.py` & `pymino-1.1.7.5/pymino/__init__.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 __title__ = 'pymino'
 __author__ = 'cynical'
 __license__ = 'MIT'
 __copyright__ = 'Copyright 2023 Cynical'
-__version__ = '1.1.7.4'
+__version__ = '1.1.7.5'
 __description__ = 'A Python wrapper for the aminoapps.com API'
 
 from .bot import Bot as Bot
 from .client import Client as Client
 
 from requests import get
 from colorama import Fore, Style
```

### Comparing `pymino-1.1.7.4/pymino/bot.py` & `pymino-1.1.7.5/pymino/bot.py`

 * *Files identical despite different names*

### Comparing `pymino-1.1.7.4/pymino/client.py` & `pymino-1.1.7.5/pymino/client.py`

 * *Files identical despite different names*

### Comparing `pymino-1.1.7.4/pymino/ext/account.py` & `pymino-1.1.7.5/pymino/ext/account.py`

 * *Files identical despite different names*

### Comparing `pymino-1.1.7.4/pymino/ext/community.py` & `pymino-1.1.7.5/pymino/ext/community.py`

 * *Files identical despite different names*

### Comparing `pymino-1.1.7.4/pymino/ext/context.py` & `pymino-1.1.7.5/pymino/ext/context.py`

 * *Files 1% similar despite different names*

```diff
@@ -665,21 +665,27 @@
         return self._commands.fetch_command(command_name)
 
     def _handle_command(self, data: Message):
         """`_handle_command` is a function that handles commands."""
         command_name = data.content[len(self.command_prefix):].split(" ")[0]
 
         if any([self.command_exists(command_name) != True, self.command_prefix != data.content[:len(self.command_prefix)]]):
-            if command_name == "help":
+            if (
+                command_name == "help"
+                and data.content == f"{self.command_prefix}help"
+            ):
                 return Context(data, self.request).reply(self._commands.__help__())
             elif "text_message" in self._events:
                 return self._handle_text_message(data)
             else:
                 return None
 
+        if data.content[:len(self.command_prefix)] != self.command_prefix:
+            return None
+
         message = data.content[len(self.command_prefix) + len(command_name) + 1:]
         parameters = [{
             "ctx": Context(data, self.request),
             "message": None if len(message) == 0 else message,
             "username": data.author.username,
             "userId": data.author.userId
         }.get(i) for i in inspect_signature(self.fetch_command(command_name).func).parameters]
```

### Comparing `pymino-1.1.7.4/pymino/ext/dispatcher.py` & `pymino-1.1.7.5/pymino/ext/dispatcher.py`

 * *Files identical despite different names*

### Comparing `pymino-1.1.7.4/pymino/ext/entities/enums.py` & `pymino-1.1.7.5/pymino/ext/entities/enums.py`

 * *Files identical despite different names*

### Comparing `pymino-1.1.7.4/pymino/ext/entities/exceptions.py` & `pymino-1.1.7.5/pymino/ext/entities/exceptions.py`

 * *Files identical despite different names*

### Comparing `pymino-1.1.7.4/pymino/ext/entities/general.py` & `pymino-1.1.7.5/pymino/ext/entities/general.py`

 * *Files identical despite different names*

### Comparing `pymino-1.1.7.4/pymino/ext/entities/handlers.py` & `pymino-1.1.7.5/pymino/ext/entities/handlers.py`

 * *Files identical despite different names*

### Comparing `pymino-1.1.7.4/pymino/ext/entities/messages.py` & `pymino-1.1.7.5/pymino/ext/entities/messages.py`

 * *Files identical despite different names*

### Comparing `pymino-1.1.7.4/pymino/ext/entities/threads.py` & `pymino-1.1.7.5/pymino/ext/entities/threads.py`

 * *Files identical despite different names*

### Comparing `pymino-1.1.7.4/pymino/ext/entities/userprofile.py` & `pymino-1.1.7.5/pymino/ext/entities/userprofile.py`

 * *Files identical despite different names*

### Comparing `pymino-1.1.7.4/pymino/ext/entities/wsevents.py` & `pymino-1.1.7.5/pymino/ext/entities/wsevents.py`

 * *Files identical despite different names*

### Comparing `pymino-1.1.7.4/pymino/ext/socket.py` & `pymino-1.1.7.5/pymino/ext/socket.py`

 * *Files identical despite different names*

### Comparing `pymino-1.1.7.4/pymino/ext/utilities/commands.py` & `pymino-1.1.7.5/pymino/ext/utilities/commands.py`

 * *Files identical despite different names*

### Comparing `pymino-1.1.7.4/pymino/ext/utilities/generate.py` & `pymino-1.1.7.5/pymino/ext/utilities/generate.py`

 * *Files identical despite different names*

### Comparing `pymino-1.1.7.4/pymino/ext/utilities/request_handler.py` & `pymino-1.1.7.5/pymino/ext/utilities/request_handler.py`

 * *Files identical despite different names*

### Comparing `pymino-1.1.7.4/pymino.egg-info/PKG-INFO` & `pymino-1.1.7.5/pymino.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pymino
-Version: 1.1.7.4
+Version: 1.1.7.5
 Summary: Easily create a bot for Amino Apps using a modern easy to use synchronous library.
 Home-page: https://github.com/forevercynical/pymino
 Author: forevercynical
 Author-email: me@cynical.gg
 License: MIT
 Keywords: amino,pymino,narvii,amino-api,narvii-bots,aminoapps,amino-bot,amino-bots
 Classifier: Programming Language :: Python :: 3
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: pymino Version: 1.1.7.4 Summary: Easily create a
+Metadata-Version: 2.1 Name: pymino Version: 1.1.7.5 Summary: Easily create a
 bot for Amino Apps using a modern easy to use synchronous library. Home-page:
 https://github.com/forevercynical/pymino Author: forevercynical Author-email:
 me@cynical.gg License: MIT Keywords: amino,pymino,narvii,amino-api,narvii-
 bots,aminoapps,amino-bot,amino-bots Classifier: Programming Language :: Python
 :: 3 Classifier: Programming Language :: Python :: 3.7 Classifier: Programming
 Language :: Python :: 3.8 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
```

### Comparing `pymino-1.1.7.4/pymino.egg-info/SOURCES.txt` & `pymino-1.1.7.5/pymino.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pymino-1.1.7.4/setup.cfg` & `pymino-1.1.7.5/setup.cfg`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2070 796d 696e 6f0d 0a76 6572 7369   = pymino..versi
-00000020: 6f6e 203d 2031 2e31 2e37 2e34 0d0a 6175  on = 1.1.7.4..au
+00000020: 6f6e 203d 2031 2e31 2e37 2e35 0d0a 6175  on = 1.1.7.5..au
 00000030: 7468 6f72 203d 2066 6f72 6576 6572 6379  thor = forevercy
 00000040: 6e69 6361 6c0d 0a61 7574 686f 725f 656d  nical..author_em
 00000050: 6169 6c20 3d20 6d65 4063 796e 6963 616c  ail = me@cynical
 00000060: 2e67 670d 0a64 6573 6372 6970 7469 6f6e  .gg..description
 00000070: 203d 2045 6173 696c 7920 6372 6561 7465   = Easily create
 00000080: 2061 2062 6f74 2066 6f72 2041 6d69 6e6f   a bot for Amino
 00000090: 2041 7070 7320 7573 696e 6720 6120 6d6f   Apps using a mo
```

### Comparing `pymino-1.1.7.4/setup.py` & `pymino-1.1.7.5/setup.py`

 * *Files identical despite different names*

