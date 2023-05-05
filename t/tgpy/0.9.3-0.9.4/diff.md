# Comparing `tmp/tgpy-0.9.3.tar.gz` & `tmp/tgpy-0.9.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tgpy-0.9.3.tar", max compression
+gzip compressed data, was "tgpy-0.9.4.tar", max compression
```

## Comparing `tgpy-0.9.3.tar` & `tgpy-0.9.4.tar`

### file list

```diff
@@ -1,35 +1,34 @@
--rw-r--r--   0        0        0     1070 2023-02-25 18:13:34.225041 tgpy-0.9.3/LICENSE
--rw-r--r--   0        0        0     3157 2023-02-25 18:13:34.225041 tgpy-0.9.3/README.md
--rw-r--r--   0        0        0     1282 2023-02-25 18:13:51.541069 tgpy-0.9.3/pyproject.toml
--rw-r--r--   0        0        0      478 2023-02-25 18:13:34.233041 tgpy-0.9.3/tgpy/__init__.py
--rw-r--r--   0        0        0       35 2023-02-25 18:13:34.233041 tgpy-0.9.3/tgpy/__main__.py
--rw-r--r--   0        0        0        0 2023-02-25 18:13:34.233041 tgpy-0.9.3/tgpy/_core/__init__.py
--rw-r--r--   0        0        0     1102 2023-02-25 18:13:34.233041 tgpy-0.9.3/tgpy/_core/eval_message.py
--rw-r--r--   0        0        0     2904 2023-02-25 18:13:34.233041 tgpy-0.9.3/tgpy/_core/message_design.py
--rw-r--r--   0        0        0     5442 2023-02-25 18:13:34.233041 tgpy-0.9.3/tgpy/_core/meval.py
--rw-r--r--   0        0        0      429 2023-02-25 18:13:34.233041 tgpy-0.9.3/tgpy/_core/utils.py
--rw-r--r--   0        0        0     3530 2023-02-25 18:13:34.233041 tgpy-0.9.3/tgpy/_handlers/__init__.py
--rw-r--r--   0        0        0     1192 2023-02-25 18:13:34.233041 tgpy-0.9.3/tgpy/api/__init__.py
--rw-r--r--   0        0        0     1525 2023-02-25 18:13:34.233041 tgpy-0.9.3/tgpy/api/config.py
--rw-r--r--   0        0        0      449 2023-02-25 18:13:34.233041 tgpy-0.9.3/tgpy/api/directories.py
--rw-r--r--   0        0        0     4135 2023-02-25 18:13:34.233041 tgpy-0.9.3/tgpy/api/parse_code.py
--rw-r--r--   0        0        0      686 2023-02-25 18:13:34.233041 tgpy-0.9.3/tgpy/api/parse_tgpy_message.py
--rw-r--r--   0        0        0     1829 2023-02-25 18:13:34.233041 tgpy-0.9.3/tgpy/api/tgpy_eval.py
--rw-r--r--   0        0        0     4516 2023-02-25 18:13:34.233041 tgpy-0.9.3/tgpy/api/transformers.py
--rw-r--r--   0        0        0     2556 2023-02-25 18:13:34.233041 tgpy-0.9.3/tgpy/api/utils.py
--rw-r--r--   0        0        0     1380 2023-02-25 18:13:34.233041 tgpy-0.9.3/tgpy/context.py
--rw-r--r--   0        0        0     4577 2023-02-25 18:13:34.233041 tgpy-0.9.3/tgpy/main.py
--rw-r--r--   0        0        0     5251 2023-02-25 18:13:34.233041 tgpy-0.9.3/tgpy/modules.py
--rw-r--r--   0        0        0     1776 2023-02-25 18:13:34.233041 tgpy-0.9.3/tgpy/reactions_fix.py
--rw-r--r--   0        0        0     1198 2023-02-25 18:13:34.233041 tgpy-0.9.3/tgpy/std/compat.py
--rw-r--r--   0        0        0      221 2023-02-25 18:13:34.233041 tgpy-0.9.3/tgpy/std/constants.py
--rw-r--r--   0        0        0     2618 2023-02-25 18:13:34.233041 tgpy-0.9.3/tgpy/std/module_manager.py
--rw-r--r--   0        0        0      364 2023-02-25 18:13:34.233041 tgpy-0.9.3/tgpy/std/ping.py
--rw-r--r--   0        0        0     1263 2023-02-25 18:13:34.233041 tgpy-0.9.3/tgpy/std/postfix_await.py
--rw-r--r--   0        0        0     2360 2023-02-25 18:13:34.233041 tgpy-0.9.3/tgpy/std/prevent_eval.py
--rw-r--r--   0        0        0      915 2023-02-25 18:13:34.233041 tgpy-0.9.3/tgpy/std/restart.py
--rw-r--r--   0        0        0     1273 2023-02-25 18:13:34.233041 tgpy-0.9.3/tgpy/std/update.py
--rw-r--r--   0        0        0     2509 2023-02-25 18:13:34.233041 tgpy-0.9.3/tgpy/utils.py
--rw-r--r--   0        0        0       62 2023-02-25 18:13:53.633065 tgpy-0.9.3/tgpy/version.py
--rw-r--r--   0        0        0     4177 1970-01-01 00:00:00.000000 tgpy-0.9.3/setup.py
--rw-r--r--   0        0        0     4082 1970-01-01 00:00:00.000000 tgpy-0.9.3/PKG-INFO
+-rw-r--r--   0        0        0     1070 2023-05-05 17:58:56.186671 tgpy-0.9.4/LICENSE
+-rw-r--r--   0        0        0     3157 2023-05-05 17:58:56.186671 tgpy-0.9.4/README.md
+-rw-r--r--   0        0        0     1282 2023-05-05 17:59:10.999044 tgpy-0.9.4/pyproject.toml
+-rw-r--r--   0        0        0      478 2023-05-05 17:58:56.190671 tgpy-0.9.4/tgpy/__init__.py
+-rw-r--r--   0        0        0       35 2023-05-05 17:58:56.190671 tgpy-0.9.4/tgpy/__main__.py
+-rw-r--r--   0        0        0        0 2023-05-05 17:58:56.190671 tgpy-0.9.4/tgpy/_core/__init__.py
+-rw-r--r--   0        0        0     1102 2023-05-05 17:58:56.190671 tgpy-0.9.4/tgpy/_core/eval_message.py
+-rw-r--r--   0        0        0     2904 2023-05-05 17:58:56.190671 tgpy-0.9.4/tgpy/_core/message_design.py
+-rw-r--r--   0        0        0     5442 2023-05-05 17:58:56.194671 tgpy-0.9.4/tgpy/_core/meval.py
+-rw-r--r--   0        0        0      429 2023-05-05 17:58:56.194671 tgpy-0.9.4/tgpy/_core/utils.py
+-rw-r--r--   0        0        0     3530 2023-05-05 17:58:56.194671 tgpy-0.9.4/tgpy/_handlers/__init__.py
+-rw-r--r--   0        0        0     1192 2023-05-05 17:58:56.194671 tgpy-0.9.4/tgpy/api/__init__.py
+-rw-r--r--   0        0        0     1525 2023-05-05 17:58:56.194671 tgpy-0.9.4/tgpy/api/config.py
+-rw-r--r--   0        0        0      449 2023-05-05 17:58:56.194671 tgpy-0.9.4/tgpy/api/directories.py
+-rw-r--r--   0        0        0     4135 2023-05-05 17:58:56.194671 tgpy-0.9.4/tgpy/api/parse_code.py
+-rw-r--r--   0        0        0      686 2023-05-05 17:58:56.194671 tgpy-0.9.4/tgpy/api/parse_tgpy_message.py
+-rw-r--r--   0        0        0     1829 2023-05-05 17:58:56.194671 tgpy-0.9.4/tgpy/api/tgpy_eval.py
+-rw-r--r--   0        0        0     4516 2023-05-05 17:58:56.194671 tgpy-0.9.4/tgpy/api/transformers.py
+-rw-r--r--   0        0        0     2556 2023-05-05 17:58:56.194671 tgpy-0.9.4/tgpy/api/utils.py
+-rw-r--r--   0        0        0     1542 2023-05-05 17:58:56.194671 tgpy-0.9.4/tgpy/context.py
+-rw-r--r--   0        0        0     4880 2023-05-05 17:58:56.194671 tgpy-0.9.4/tgpy/main.py
+-rw-r--r--   0        0        0     5251 2023-05-05 17:58:56.194671 tgpy-0.9.4/tgpy/modules.py
+-rw-r--r--   0        0        0     1776 2023-05-05 17:58:56.194671 tgpy-0.9.4/tgpy/reactions_fix.py
+-rw-r--r--   0        0        0     1198 2023-05-05 17:58:56.194671 tgpy-0.9.4/tgpy/std/compat.py
+-rw-r--r--   0        0        0      221 2023-05-05 17:58:56.194671 tgpy-0.9.4/tgpy/std/constants.py
+-rw-r--r--   0        0        0     2618 2023-05-05 17:58:56.194671 tgpy-0.9.4/tgpy/std/module_manager.py
+-rw-r--r--   0        0        0      364 2023-05-05 17:58:56.194671 tgpy-0.9.4/tgpy/std/ping.py
+-rw-r--r--   0        0        0     1263 2023-05-05 17:58:56.194671 tgpy-0.9.4/tgpy/std/postfix_await.py
+-rw-r--r--   0        0        0     2360 2023-05-05 17:58:56.194671 tgpy-0.9.4/tgpy/std/prevent_eval.py
+-rw-r--r--   0        0        0      915 2023-05-05 17:58:56.194671 tgpy-0.9.4/tgpy/std/restart.py
+-rw-r--r--   0        0        0     1273 2023-05-05 17:58:56.194671 tgpy-0.9.4/tgpy/std/update.py
+-rw-r--r--   0        0        0     2509 2023-05-05 17:58:56.194671 tgpy-0.9.4/tgpy/utils.py
+-rw-r--r--   0        0        0       62 2023-05-05 17:59:12.495084 tgpy-0.9.4/tgpy/version.py
+-rw-r--r--   0        0        0     4082 1970-01-01 00:00:00.000000 tgpy-0.9.4/PKG-INFO
```

### Comparing `tgpy-0.9.3/LICENSE` & `tgpy-0.9.4/LICENSE`

 * *Files identical despite different names*

### Comparing `tgpy-0.9.3/README.md` & `tgpy-0.9.4/README.md`

 * *Files identical despite different names*

### Comparing `tgpy-0.9.3/pyproject.toml` & `tgpy-0.9.4/pyproject.toml`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "tgpy"
-version = "0.9.3"
+version = "0.9.4"
 description = "Run Python code right in your Telegram messages"
 authors = ["tmat <a@tmat.me>", "vanutp <hello@vanutp.dev>", "ntonee <a12286@yandex.com>"]
 license = "MIT"
 documentation = "https://tgpy.tmat.me/"
 repository = "https://github.com/tm-a-t/TGPy/"
 readme = "README.md"
 classifiers = [
```

### Comparing `tgpy-0.9.3/tgpy/_core/eval_message.py` & `tgpy-0.9.4/tgpy/_core/eval_message.py`

 * *Files identical despite different names*

### Comparing `tgpy-0.9.3/tgpy/_core/message_design.py` & `tgpy-0.9.4/tgpy/_core/message_design.py`

 * *Files identical despite different names*

### Comparing `tgpy-0.9.3/tgpy/_core/meval.py` & `tgpy-0.9.4/tgpy/_core/meval.py`

 * *Files identical despite different names*

### Comparing `tgpy-0.9.3/tgpy/_handlers/__init__.py` & `tgpy-0.9.4/tgpy/_handlers/__init__.py`

 * *Files identical despite different names*

### Comparing `tgpy-0.9.3/tgpy/api/__init__.py` & `tgpy-0.9.4/tgpy/api/__init__.py`

 * *Files identical despite different names*

### Comparing `tgpy-0.9.3/tgpy/api/config.py` & `tgpy-0.9.4/tgpy/api/config.py`

 * *Files identical despite different names*

### Comparing `tgpy-0.9.3/tgpy/api/parse_code.py` & `tgpy-0.9.4/tgpy/api/parse_code.py`

 * *Files identical despite different names*

### Comparing `tgpy-0.9.3/tgpy/api/parse_tgpy_message.py` & `tgpy-0.9.4/tgpy/api/parse_tgpy_message.py`

 * *Files identical despite different names*

### Comparing `tgpy-0.9.3/tgpy/api/tgpy_eval.py` & `tgpy-0.9.4/tgpy/api/tgpy_eval.py`

 * *Files identical despite different names*

### Comparing `tgpy-0.9.3/tgpy/api/transformers.py` & `tgpy-0.9.4/tgpy/api/transformers.py`

 * *Files identical despite different names*

### Comparing `tgpy-0.9.3/tgpy/api/utils.py` & `tgpy-0.9.4/tgpy/api/utils.py`

 * *Files identical despite different names*

### Comparing `tgpy-0.9.3/tgpy/context.py` & `tgpy-0.9.4/tgpy/context.py`

 * *Files 11% similar despite different names*

```diff
@@ -13,14 +13,21 @@
 class _StdoutWrapper(TextIOBase):
     def __getobj(self):
         return _stdout.get(sys.__stdout__)
 
     def write(self, s: str) -> int:
         return self.__getobj().write(s)
 
+    def flush(self) -> None:
+        return self.__getobj().flush()
+
+    @property
+    def isatty(self):
+        return getattr(self.__getobj(), 'isatty', None)
+
 
 sys.stdout = _StdoutWrapper()
 
 
 class Context:
     @property
     def is_module(self) -> bool:
```

### Comparing `tgpy-0.9.3/tgpy/main.py` & `tgpy-0.9.4/tgpy/main.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import asyncio
+import functools
 import logging
 
 import aiorun
 import yaml
 from rich.console import Console, Theme
 from telethon import TelegramClient, errors
 from yaml import YAMLError
@@ -15,30 +16,41 @@
 
 logger = logging.getLogger(__name__)
 
 theme = Theme(inherit=False)
 console = Console(theme=theme)
 
 
+async def ainput(prompt: str, password: bool = False):
+    def wrapper(prompt, password):
+        return console.input(prompt, password=password)
+
+    return await asyncio.get_event_loop().run_in_executor(
+        None, wrapper, prompt, password
+    )
+
+
 def create_client():
     client = TelegramClient(
         str(SESSION_FILENAME),
         config.get('core.api_id'),
         config.get('core.api_hash'),
     )
     client.parse_mode = 'html'
     return client
 
 
 async def start_client():
     await app.client.start(
-        phone=lambda: console.input('| Please enter your phone number: '),
-        code_callback=lambda: console.input('| Please enter the code you received: '),
-        password=lambda: console.input(
-            '| Please enter your 2FA password: ', password=True
+        phone=functools.partial(ainput, '| Please enter your phone number: '),
+        code_callback=functools.partial(
+            ainput, '| Please enter the code you received: '
+        ),
+        password=functools.partial(
+            ainput, '| Please enter your 2FA password: ', password=True
         ),
     )
 
 
 async def initial_setup():
     console.print('[bold on bright_cyan] Welcome to TGPy ')
     console.print('Starting setup...')
@@ -50,16 +62,16 @@
         '│  [cyan]2.[/] Login with your Telegram account\n'
         '│  [cyan]3.[/] Go to "API development tools"\n'
         '│  [cyan]4.[/] Create your app. Choose any app title and short_title. You can leave other fields empty.\n'
         '│ You will get api_id and api_hash.'
     )
     success = False
     while not success:
-        config.set('core.api_id', int(console.input('│ Please enter api_id: ')))
-        config.set('core.api_hash', console.input('│ ...and api_hash: '))
+        config.set('core.api_id', int(await ainput('│ Please enter api_id: ')))
+        config.set('core.api_hash', await ainput('│ ...and api_hash: '))
         try:
             app.client = create_client()
             console.print()
             console.print('[bold black on white] Step 2 of 2 ')
             console.print('│ Now login to Telegram.')
             await app.client.connect()
             await start_client()
```

### Comparing `tgpy-0.9.3/tgpy/modules.py` & `tgpy-0.9.4/tgpy/modules.py`

 * *Files identical despite different names*

### Comparing `tgpy-0.9.3/tgpy/reactions_fix.py` & `tgpy-0.9.4/tgpy/reactions_fix.py`

 * *Files identical despite different names*

### Comparing `tgpy-0.9.3/tgpy/std/compat.py` & `tgpy-0.9.4/tgpy/std/compat.py`

 * *Files identical despite different names*

### Comparing `tgpy-0.9.3/tgpy/std/module_manager.py` & `tgpy-0.9.4/tgpy/std/module_manager.py`

 * *Files identical despite different names*

### Comparing `tgpy-0.9.3/tgpy/std/postfix_await.py` & `tgpy-0.9.4/tgpy/std/postfix_await.py`

 * *Files identical despite different names*

### Comparing `tgpy-0.9.3/tgpy/std/prevent_eval.py` & `tgpy-0.9.4/tgpy/std/prevent_eval.py`

 * *Files identical despite different names*

### Comparing `tgpy-0.9.3/tgpy/std/restart.py` & `tgpy-0.9.4/tgpy/std/restart.py`

 * *Files identical despite different names*

### Comparing `tgpy-0.9.3/tgpy/std/update.py` & `tgpy-0.9.4/tgpy/std/update.py`

 * *Files identical despite different names*

### Comparing `tgpy-0.9.3/tgpy/utils.py` & `tgpy-0.9.4/tgpy/utils.py`

 * *Files identical despite different names*

### Comparing `tgpy-0.9.3/setup.py` & `tgpy-0.9.4/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,39 +1,110 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: tgpy
+Version: 0.9.4
+Summary: Run Python code right in your Telegram messages
+Home-page: https://github.com/tm-a-t/TGPy/
+License: MIT
+Author: tmat
+Author-email: a@tmat.me
+Requires-Python: >=3.9,<4.0
+Classifier: License :: OSI Approved :: MIT License
+Classifier: Operating System :: OS Independent
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Requires-Dist: PyYAML (>=6.0,<7.0)
+Requires-Dist: aiorun (>=2022.4.1,<2023.0.0)
+Requires-Dist: appdirs (>=1.4.4,<2.0.0)
+Requires-Dist: cryptg-anyos (>=0.4.1,<0.5.0)
+Requires-Dist: rich (>=12.5.1,<13.0.0)
+Requires-Dist: telethon-v1-24 (>=1.24.8,<2.0.0)
+Project-URL: Documentation, https://tgpy.tmat.me/
+Project-URL: Repository, https://github.com/tm-a-t/TGPy/
+Description-Content-Type: text/markdown
 
-packages = \
-['tgpy', 'tgpy._core', 'tgpy._handlers', 'tgpy.api', 'tgpy.std']
+<div align="center" style="width: 50%">
 
-package_data = \
-{'': ['*']}
+<h3>
+<a href="https://tgpy.tmat.me">
+<img alt="TGPy Logo" src="guide/docs/assets/TGPy.png" width=280>
+</a>
+ 
+Runs Python code snippets<br>within your Telegram messages
+</h3>
 
-install_requires = \
-['PyYAML>=6.0,<7.0',
- 'aiorun>=2022.4.1,<2023.0.0',
- 'appdirs>=1.4.4,<2.0.0',
- 'cryptg-anyos>=0.4.1,<0.5.0',
- 'rich>=12.5.1,<13.0.0',
- 'telethon-v1-24>=1.24.8,<2.0.0']
-
-entry_points = \
-{'console_scripts': ['tgpy = tgpy.main:main']}
-
-setup_kwargs = {
-    'name': 'tgpy',
-    'version': '0.9.3',
-    'description': 'Run Python code right in your Telegram messages',
-    'long_description': '<div align="center" style="width: 50%">\n\n<h3>\n<a href="https://tgpy.tmat.me">\n<img alt="TGPy Logo" src="guide/docs/assets/TGPy.png" width=280>\n</a>\n \nRuns Python code snippets<br>within your Telegram messages\n</h3>\n\n<h6></h6>\n  \n[![PyPI - Downloads](https://img.shields.io/pypi/dm/tgpy?style=flat-square)](https://pypi.org/project/tgpy/)\n[![PyPI](https://img.shields.io/pypi/v/tgpy?style=flat-square&color=9B59B6)](https://pypi.org/project/tgpy/)\n[![Docker Image Version (latest semver)](https://img.shields.io/docker/v/tgpy/tgpy?style=flat-square&label=docker&sort=semver&color=9B59B6)](https://hub.docker.com/r/tgpy/tgpy)\n[![Open issues](https://img.shields.io/github/issues-raw/tm-a-t/TGPy?style=flat-square)](https://github.com/tm-a-t/TGPy/issues)\n[![Docs](https://img.shields.io/website?style=flat-square&label=docs&url=https%3A%2F%2Ftgpy.tmat.me)](https://tgpy.tmat.me/)\n\n</div>\n\n<br>\n\nHere are a few examples of how people use TGPy:\n\n🧮 Run Python as an in-chat calculator\n\n🔍 Search for song lyrics within a chat\n\n🧹 Delete multiple messages with a command\n\n📊 Find out the most active members in a chat\n\n✏️ Instantly convert TeX to Unicode in messages:<br>For example, `x = \\alpha^7` becomes `x = α⁷`\n\n## About\n\nTGPy allows you to easily write and execute code snippets directly within your Telegram messages. Combine Telegram features with the full power of Python: Integrate with libraries and APIs. Create functions and TGPy modules to reuse code in the future. Set up code transformers and hooks to create custom commands and tweak Python syntax.\n\nTGPy uses Telegram API through the [Telethon](https://github.com/LonamiWebs/Telethon) library.\n\n## Quick Start\n\nPython 3.10+ required. Install TGPy and connect it to your Telegram account:\n\n```shell\n> pip install tgpy\n> tgpy\n```\n\nYou’re ready now. Send Python code to any chat, and it will run. Change your message to change the result. [Read more on installation](http://tgpy.tmat.me/installation/)\n\n## Learn\n\n[🙂 Basics Guide](https://tgpy.tmat.me/basics/code/)\n\n[😎 Extensibility Guide](https://tgpy.tmat.me/extensibility/context/)\n\n[📗 Reference](https://tgpy.tmat.me/reference/builtins/)\n\n[💬 Russian-Speaking Chat](https://t.me/tgpy_flood)\n\n\n## Demo\n\nhttps://user-images.githubusercontent.com/38432588/181266550-c4640ff1-71f2-4868-ab83-6ea3690c01b6.mp4\n\n<br>\n\n![A message processed with TGPy](guide/docs/assets/example.png)\n_Finding out the number of premium users in a chat_\n\n## Inspiration\n\nTGPy is inspired by [FTG](https://gitlab.com/friendly-telegram/friendly-telegram) and similar userbots. However, the key concept is different: TGPy is totally based on usage of code in Telegram rather than plugging extra modules. It was designed for running single-use scripts and reusing code flexibly. You can think of TGPy as a userbot for programmers.\n\n## Credits\n\nTGPy is built on [Telethon](https://github.com/LonamiWebs/Telethon), a Python library to interact with Telegram API.\n\nBasic code transformation (such as auto-return of values) is based on [meval](https://github.com/penn5/meval).\n\n## License\n\nThis project is licensed under the terms of the MIT license.\n',
-    'author': 'tmat',
-    'author_email': 'a@tmat.me',
-    'maintainer': 'None',
-    'maintainer_email': 'None',
-    'url': 'https://github.com/tm-a-t/TGPy/',
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'entry_points': entry_points,
-    'python_requires': '>=3.9,<4.0',
-}
+<h6></h6>
+  
+[![PyPI - Downloads](https://img.shields.io/pypi/dm/tgpy?style=flat-square)](https://pypi.org/project/tgpy/)
+[![PyPI](https://img.shields.io/pypi/v/tgpy?style=flat-square&color=9B59B6)](https://pypi.org/project/tgpy/)
+[![Docker Image Version (latest semver)](https://img.shields.io/docker/v/tgpy/tgpy?style=flat-square&label=docker&sort=semver&color=9B59B6)](https://hub.docker.com/r/tgpy/tgpy)
+[![Open issues](https://img.shields.io/github/issues-raw/tm-a-t/TGPy?style=flat-square)](https://github.com/tm-a-t/TGPy/issues)
+[![Docs](https://img.shields.io/website?style=flat-square&label=docs&url=https%3A%2F%2Ftgpy.tmat.me)](https://tgpy.tmat.me/)
 
+</div>
+
+<br>
+
+Here are a few examples of how people use TGPy:
+
+🧮 Run Python as an in-chat calculator
+
+🔍 Search for song lyrics within a chat
+
+🧹 Delete multiple messages with a command
+
+📊 Find out the most active members in a chat
+
+✏️ Instantly convert TeX to Unicode in messages:<br>For example, `x = \alpha^7` becomes `x = α⁷`
+
+## About
+
+TGPy allows you to easily write and execute code snippets directly within your Telegram messages. Combine Telegram features with the full power of Python: Integrate with libraries and APIs. Create functions and TGPy modules to reuse code in the future. Set up code transformers and hooks to create custom commands and tweak Python syntax.
+
+TGPy uses Telegram API through the [Telethon](https://github.com/LonamiWebs/Telethon) library.
+
+## Quick Start
+
+Python 3.10+ required. Install TGPy and connect it to your Telegram account:
+
+```shell
+> pip install tgpy
+> tgpy
+```
+
+You’re ready now. Send Python code to any chat, and it will run. Change your message to change the result. [Read more on installation](http://tgpy.tmat.me/installation/)
+
+## Learn
+
+[🙂 Basics Guide](https://tgpy.tmat.me/basics/code/)
+
+[😎 Extensibility Guide](https://tgpy.tmat.me/extensibility/context/)
+
+[📗 Reference](https://tgpy.tmat.me/reference/builtins/)
+
+[💬 Russian-Speaking Chat](https://t.me/tgpy_flood)
+
+
+## Demo
+
+https://user-images.githubusercontent.com/38432588/181266550-c4640ff1-71f2-4868-ab83-6ea3690c01b6.mp4
+
+<br>
+
+![A message processed with TGPy](guide/docs/assets/example.png)
+_Finding out the number of premium users in a chat_
+
+## Inspiration
+
+TGPy is inspired by [FTG](https://gitlab.com/friendly-telegram/friendly-telegram) and similar userbots. However, the key concept is different: TGPy is totally based on usage of code in Telegram rather than plugging extra modules. It was designed for running single-use scripts and reusing code flexibly. You can think of TGPy as a userbot for programmers.
+
+## Credits
+
+TGPy is built on [Telethon](https://github.com/LonamiWebs/Telethon), a Python library to interact with Telegram API.
+
+Basic code transformation (such as auto-return of values) is based on [meval](https://github.com/penn5/meval).
+
+## License
+
+This project is licensed under the terms of the MIT license.
 
-setup(**setup_kwargs)
```

#### html2text {}

```diff
@@ -1,58 +1,56 @@
-# -*- coding: utf-8 -*- from setuptools import setup packages = \ ['tgpy',
-'tgpy._core', 'tgpy._handlers', 'tgpy.api', 'tgpy.std'] package_data = \ {'':
-['*']} install_requires = \ ['PyYAML>=6.0,<7.0', 'aiorun>=2022.4.1,<2023.0.0',
-'appdirs>=1.4.4,<2.0.0', 'cryptg-anyos>=0.4.1,<0.5.0', 'rich>=12.5.1,<13.0.0',
-'telethon-v1-24>=1.24.8,<2.0.0'] entry_points = \ {'console_scripts': ['tgpy =
-tgpy.main:main']} setup_kwargs = { 'name': 'tgpy', 'version': '0.9.3',
-'description': 'Run Python code right in your Telegram messages',
-'long_description': '
-                                     \n\n
-             **** \n\n[TGPy_Logo]\n\n \nRuns Python code snippets
-                     within your Telegram messages\n ****
-                                     \n\n
-   \n \n[![PyPI - Downloads](https://img.shields.io/pypi/dm/tgpy?style=flat-
-square)](https://pypi.org/project/tgpy/)\n[![PyPI](https://img.shields.io/pypi/
-  v/tgpy?style=flat-square&color=9B59B6)](https://pypi.org/project/tgpy/)\n[!
- [Docker Image Version (latest semver)](https://img.shields.io/docker/v/tgpy/
+Metadata-Version: 2.1 Name: tgpy Version: 0.9.4 Summary: Run Python code right
+in your Telegram messages Home-page: https://github.com/tm-a-t/TGPy/ License:
+MIT Author: tmat Author-email: a@tmat.me Requires-Python: >=3.9,<4.0
+Classifier: License :: OSI Approved :: MIT License Classifier: Operating System
+:: OS Independent Classifier: Programming Language :: Python :: 3 Classifier:
+Programming Language :: Python :: 3.9 Classifier: Programming Language ::
+Python :: 3.10 Classifier: Programming Language :: Python :: 3.11 Requires-
+Dist: PyYAML (>=6.0,<7.0) Requires-Dist: aiorun (>=2022.4.1,<2023.0.0)
+Requires-Dist: appdirs (>=1.4.4,<2.0.0) Requires-Dist: cryptg-anyos
+(>=0.4.1,<0.5.0) Requires-Dist: rich (>=12.5.1,<13.0.0) Requires-Dist:
+telethon-v1-24 (>=1.24.8,<2.0.0) Project-URL: Documentation, https://
+tgpy.tmat.me/ Project-URL: Repository, https://github.com/tm-a-t/TGPy/
+Description-Content-Type: text/markdown
+                  **** [TGPy_Logo] Runs Python code snippets
+                      within your Telegram messages ****
+ [![PyPI - Downloads](https://img.shields.io/pypi/dm/tgpy?style=flat-square)]
+   (https://pypi.org/project/tgpy/) [![PyPI](https://img.shields.io/pypi/v/
+tgpy?style=flat-square&color=9B59B6)](https://pypi.org/project/tgpy/) [![Docker
+     Image Version (latest semver)](https://img.shields.io/docker/v/tgpy/
     tgpy?style=flat-square&label=docker&sort=semver&color=9B59B6)](https://
-  hub.docker.com/r/tgpy/tgpy)\n[![Open issues](https://img.shields.io/github/
+  hub.docker.com/r/tgpy/tgpy) [![Open issues](https://img.shields.io/github/
   issues-raw/tm-a-t/TGPy?style=flat-square)](https://github.com/tm-a-t/TGPy/
-         issues)\n[![Docs](https://img.shields.io/website?style=flat-
- square&label=docs&url=https%3A%2F%2Ftgpy.tmat.me)](https://tgpy.tmat.me/)\n\n
-\n\n
-\n\nHere are a few examples of how people use TGPy:\n\nð§® Run Python as an
-in-chat calculator\n\nð Search for song lyrics within a chat\n\nð§¹ Delete
-multiple messages with a command\n\nð Find out the most active members in a
-chat\n\nâï¸ Instantly convert TeX to Unicode in messages:
-For example, `x = \\alpha^7` becomes `x = Î±â·`\n\n## About\n\nTGPy allows you
-to easily write and execute code snippets directly within your Telegram
-messages. Combine Telegram features with the full power of Python: Integrate
-with libraries and APIs. Create functions and TGPy modules to reuse code in the
+          issues) [![Docs](https://img.shields.io/website?style=flat-
+   square&label=docs&url=https%3A%2F%2Ftgpy.tmat.me)](https://tgpy.tmat.me/)
+
+Here are a few examples of how people use TGPy: ð§® Run Python as an in-chat
+calculator ð Search for song lyrics within a chat ð§¹ Delete multiple
+messages with a command ð Find out the most active members in a chat âï¸
+Instantly convert TeX to Unicode in messages:
+For example, `x = \alpha^7` becomes `x = Î±â·` ## About TGPy allows you to
+easily write and execute code snippets directly within your Telegram messages.
+Combine Telegram features with the full power of Python: Integrate with
+libraries and APIs. Create functions and TGPy modules to reuse code in the
 future. Set up code transformers and hooks to create custom commands and tweak
-Python syntax.\n\nTGPy uses Telegram API through the [Telethon](https://
-github.com/LonamiWebs/Telethon) library.\n\n## Quick Start\n\nPython 3.10+
-required. Install TGPy and connect it to your Telegram account:\n\n```shell\n>
-pip install tgpy\n> tgpy\n```\n\nYouâre ready now. Send Python code to any
-chat, and it will run. Change your message to change the result. [Read more on
-installation](http://tgpy.tmat.me/installation/)\n\n## Learn\n\n[ð Basics
-Guide](https://tgpy.tmat.me/basics/code/)\n\n[ð Extensibility Guide](https:/
-/tgpy.tmat.me/extensibility/context/)\n\n[ð Reference](https://tgpy.tmat.me/
-reference/builtins/)\n\n[ð¬ Russian-Speaking Chat](https://t.me/
-tgpy_flood)\n\n\n## Demo\n\nhttps://user-images.githubusercontent.com/38432588/
-181266550-c4640ff1-71f2-4868-ab83-6ea3690c01b6.mp4\n\n
-\n\n![A message processed with TGPy](guide/docs/assets/example.png)\n_Finding
-out the number of premium users in a chat_\n\n## Inspiration\n\nTGPy is
-inspired by [FTG](https://gitlab.com/friendly-telegram/friendly-telegram) and
-similar userbots. However, the key concept is different: TGPy is totally based
-on usage of code in Telegram rather than plugging extra modules. It was
-designed for running single-use scripts and reusing code flexibly. You can
-think of TGPy as a userbot for programmers.\n\n## Credits\n\nTGPy is built on
-[Telethon](https://github.com/LonamiWebs/Telethon), a Python library to
-interact with Telegram API.\n\nBasic code transformation (such as auto-return
-of values) is based on [meval](https://github.com/penn5/meval).\n\n##
-License\n\nThis project is licensed under the terms of the MIT license.\n',
-'author': 'tmat', 'author_email': 'a@tmat.me', 'maintainer': 'None',
-'maintainer_email': 'None', 'url': 'https://github.com/tm-a-t/TGPy/',
-'packages': packages, 'package_data': package_data, 'install_requires':
-install_requires, 'entry_points': entry_points, 'python_requires':
-'>=3.9,<4.0', } setup(**setup_kwargs)
+Python syntax. TGPy uses Telegram API through the [Telethon](https://
+github.com/LonamiWebs/Telethon) library. ## Quick Start Python 3.10+ required.
+Install TGPy and connect it to your Telegram account: ```shell > pip install
+tgpy > tgpy ``` Youâre ready now. Send Python code to any chat, and it will
+run. Change your message to change the result. [Read more on installation]
+(http://tgpy.tmat.me/installation/) ## Learn [ð Basics Guide](https://
+tgpy.tmat.me/basics/code/) [ð Extensibility Guide](https://tgpy.tmat.me/
+extensibility/context/) [ð Reference](https://tgpy.tmat.me/reference/
+builtins/) [ð¬ Russian-Speaking Chat](https://t.me/tgpy_flood) ## Demo https:
+//user-images.githubusercontent.com/38432588/181266550-c4640ff1-71f2-4868-ab83-
+6ea3690c01b6.mp4
+![A message processed with TGPy](guide/docs/assets/example.png) _Finding out
+the number of premium users in a chat_ ## Inspiration TGPy is inspired by [FTG]
+(https://gitlab.com/friendly-telegram/friendly-telegram) and similar userbots.
+However, the key concept is different: TGPy is totally based on usage of code
+in Telegram rather than plugging extra modules. It was designed for running
+single-use scripts and reusing code flexibly. You can think of TGPy as a
+userbot for programmers. ## Credits TGPy is built on [Telethon](https://
+github.com/LonamiWebs/Telethon), a Python library to interact with Telegram
+API. Basic code transformation (such as auto-return of values) is based on
+[meval](https://github.com/penn5/meval). ## License This project is licensed
+under the terms of the MIT license.
```

