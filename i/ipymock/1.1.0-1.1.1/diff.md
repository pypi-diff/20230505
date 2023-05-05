# Comparing `tmp/ipymock-1.1.0.tar.gz` & `tmp/ipymock-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ipymock-1.1.0.tar", last modified: Wed May  3 19:15:30 2023, max compression
+gzip compressed data, was "ipymock-1.1.1.tar", last modified: Fri May  5 04:55:09 2023, max compression
```

## Comparing `ipymock-1.1.0.tar` & `ipymock-1.1.1.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 saintway   (501) staff       (20)        0 2023-05-03 19:15:30.325563 ipymock-1.1.0/
--rw-rw-r--   0 saintway   (501) staff       (20)    11357 2021-03-19 07:00:57.000000 ipymock-1.1.0/LICENSE
--rw-rw-r--   0 saintway   (501) staff       (20)       87 2021-03-19 09:00:48.000000 ipymock-1.1.0/MANIFEST.in
--rw-r--r--   0 saintway   (501) staff       (20)    10620 2023-05-03 19:15:30.325027 ipymock-1.1.0/PKG-INFO
--rw-r--r--   0 saintway   (501) staff       (20)     9877 2023-05-03 19:12:45.000000 ipymock-1.1.0/README.md
-drwxr-xr-x   0 saintway   (501) staff       (20)        0 2023-05-03 19:15:30.319378 ipymock-1.1.0/ipymock/
--rw-rw-r--   0 saintway   (501) staff       (20)     1605 2023-05-03 19:12:22.000000 ipymock-1.1.0/ipymock/__init__.py
--rw-rw-r--   0 saintway   (501) staff       (20)     3111 2023-05-03 19:12:22.000000 ipymock-1.1.0/ipymock/_nbdev.py
--rw-rw-r--   0 saintway   (501) staff       (20)    18079 2023-05-03 19:12:22.000000 ipymock-1.1.0/ipymock/agi.py
--rw-rw-r--   0 saintway   (501) staff       (20)    18424 2023-05-03 19:12:22.000000 ipymock-1.1.0/ipymock/browser.py
--rw-rw-r--   0 saintway   (501) staff       (20)      995 2023-05-03 19:12:22.000000 ipymock-1.1.0/ipymock/llm.py
--rw-rw-r--   0 saintway   (501) staff       (20)     2974 2023-05-03 19:12:22.000000 ipymock-1.1.0/ipymock/reader.py
-drwxr-xr-x   0 saintway   (501) staff       (20)        0 2023-05-03 19:15:30.323157 ipymock-1.1.0/ipymock.egg-info/
-drwxr-xr-x   0 saintway   (501) staff       (20)        0 2023-05-03 19:15:30.324226 ipymock-1.1.0/ipymock.egg-info/.ipynb_checkpoints/
--rw-rw-r--   0 saintway   (501) staff       (20)      289 2023-04-18 09:17:57.000000 ipymock-1.1.0/ipymock.egg-info/.ipynb_checkpoints/SOURCES-checkpoint.txt
--rw-rw-r--   0 saintway   (501) staff       (20)        8 2023-04-18 09:17:56.000000 ipymock-1.1.0/ipymock.egg-info/.ipynb_checkpoints/top_level-checkpoint.txt
--rw-rw-r--   0 saintway   (501) staff       (20)    10620 2023-05-03 19:15:30.000000 ipymock-1.1.0/ipymock.egg-info/PKG-INFO
--rw-rw-r--   0 saintway   (501) staff       (20)      460 2023-05-03 19:15:30.000000 ipymock-1.1.0/ipymock.egg-info/SOURCES.txt
--rw-rw-r--   0 saintway   (501) staff       (20)        1 2023-05-03 19:15:30.000000 ipymock-1.1.0/ipymock.egg-info/dependency_links.txt
--rw-rw-r--   0 saintway   (501) staff       (20)        1 2023-04-18 09:17:56.000000 ipymock-1.1.0/ipymock.egg-info/not-zip-safe
--rw-rw-r--   0 saintway   (501) staff       (20)      129 2023-05-03 19:15:30.000000 ipymock-1.1.0/ipymock.egg-info/requires.txt
--rw-rw-r--   0 saintway   (501) staff       (20)        8 2023-05-03 19:15:30.000000 ipymock-1.1.0/ipymock.egg-info/top_level.txt
--rw-rw-r--   0 saintway   (501) staff       (20)     2610 2023-05-03 19:06:22.000000 ipymock-1.1.0/settings.ini
--rw-r--r--   0 saintway   (501) staff       (20)       38 2023-05-03 19:15:30.325662 ipymock-1.1.0/setup.cfg
--rw-rw-r--   0 saintway   (501) staff       (20)     2302 2021-03-19 07:00:57.000000 ipymock-1.1.0/setup.py
+drwxr-xr-x   0 saintway   (501) staff       (20)        0 2023-05-05 04:55:09.896762 ipymock-1.1.1/
+-rw-rw-r--   0 saintway   (501) staff       (20)    11357 2021-03-19 07:00:57.000000 ipymock-1.1.1/LICENSE
+-rw-rw-r--   0 saintway   (501) staff       (20)       87 2021-03-19 09:00:48.000000 ipymock-1.1.1/MANIFEST.in
+-rw-r--r--   0 saintway   (501) staff       (20)    11160 2023-05-05 04:55:09.896135 ipymock-1.1.1/PKG-INFO
+-rw-r--r--   0 saintway   (501) staff       (20)    10417 2023-05-05 04:51:03.000000 ipymock-1.1.1/README.md
+drwxr-xr-x   0 saintway   (501) staff       (20)        0 2023-05-05 04:55:09.889799 ipymock-1.1.1/ipymock/
+-rw-rw-r--   0 saintway   (501) staff       (20)     1605 2023-05-05 04:52:19.000000 ipymock-1.1.1/ipymock/__init__.py
+-rw-rw-r--   0 saintway   (501) staff       (20)     3343 2023-05-05 04:52:19.000000 ipymock-1.1.1/ipymock/_nbdev.py
+-rw-rw-r--   0 saintway   (501) staff       (20)    18079 2023-05-05 04:52:19.000000 ipymock-1.1.1/ipymock/agi.py
+-rw-rw-r--   0 saintway   (501) staff       (20)    20838 2023-05-05 04:52:19.000000 ipymock-1.1.1/ipymock/browser.py
+-rw-rw-r--   0 saintway   (501) staff       (20)      995 2023-05-05 04:52:19.000000 ipymock-1.1.1/ipymock/llm.py
+-rw-rw-r--   0 saintway   (501) staff       (20)     2974 2023-05-05 04:52:19.000000 ipymock-1.1.1/ipymock/reader.py
+drwxr-xr-x   0 saintway   (501) staff       (20)        0 2023-05-05 04:55:09.893736 ipymock-1.1.1/ipymock.egg-info/
+drwxr-xr-x   0 saintway   (501) staff       (20)        0 2023-05-05 04:55:09.895132 ipymock-1.1.1/ipymock.egg-info/.ipynb_checkpoints/
+-rw-rw-r--   0 saintway   (501) staff       (20)      289 2023-04-18 09:17:57.000000 ipymock-1.1.1/ipymock.egg-info/.ipynb_checkpoints/SOURCES-checkpoint.txt
+-rw-rw-r--   0 saintway   (501) staff       (20)        8 2023-04-18 09:17:56.000000 ipymock-1.1.1/ipymock.egg-info/.ipynb_checkpoints/top_level-checkpoint.txt
+-rw-rw-r--   0 saintway   (501) staff       (20)    11160 2023-05-05 04:55:09.000000 ipymock-1.1.1/ipymock.egg-info/PKG-INFO
+-rw-rw-r--   0 saintway   (501) staff       (20)      460 2023-05-05 04:55:09.000000 ipymock-1.1.1/ipymock.egg-info/SOURCES.txt
+-rw-rw-r--   0 saintway   (501) staff       (20)        1 2023-05-05 04:55:09.000000 ipymock-1.1.1/ipymock.egg-info/dependency_links.txt
+-rw-rw-r--   0 saintway   (501) staff       (20)        1 2023-04-18 09:17:56.000000 ipymock-1.1.1/ipymock.egg-info/not-zip-safe
+-rw-rw-r--   0 saintway   (501) staff       (20)      181 2023-05-05 04:55:09.000000 ipymock-1.1.1/ipymock.egg-info/requires.txt
+-rw-rw-r--   0 saintway   (501) staff       (20)        8 2023-05-05 04:55:09.000000 ipymock-1.1.1/ipymock.egg-info/top_level.txt
+-rw-rw-r--   0 saintway   (501) staff       (20)     2662 2023-05-05 04:51:47.000000 ipymock-1.1.1/settings.ini
+-rw-r--r--   0 saintway   (501) staff       (20)       38 2023-05-05 04:55:09.896918 ipymock-1.1.1/setup.cfg
+-rw-rw-r--   0 saintway   (501) staff       (20)     2302 2021-03-19 07:00:57.000000 ipymock-1.1.1/setup.py
```

### Comparing `ipymock-1.1.0/LICENSE` & `ipymock-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `ipymock-1.1.0/PKG-INFO` & `ipymock-1.1.1/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -1,66 +1,67 @@
-Metadata-Version: 2.1
-Name: ipymock
-Version: 1.1.0
-Summary: A Tool that Allows You Run PyTest within Jupyter Notebook Cells
-Home-page: https://github.com/seii-saintway/ipymock/tree/main/
-Author: andrew
-Author-email: andrew.saintway@gmail.com
-License: Apache Software License 2.0
-Keywords: pytest interactive jupyter
-Classifier: Development Status :: 3 - Alpha
-Classifier: Intended Audience :: Developers
-Classifier: Natural Language :: English
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
-Classifier: License :: OSI Approved :: Apache Software License
-Requires-Python: >=3.6
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # Running PyTest in Jupyter Notebooks
-> iPyMock uses GPT 3.5 turbo by browser automation and <a href='https://huggingface.co/GanymedeNil/text2vec-large-chinese'>a CoSENT based model</a> to embed English and Chinese.
 
+> iPyMock uses GPT 3.5 turbo by browser automation and <a href='https://huggingface.co/GanymedeNil/text2vec-large-chinese'>a CoSENT based model</a> to embed English and Chinese.
 
 [![Discord Follow](https://dcbadge.vercel.app/api/server/ARTMvTQv?style=flat)](https://discord.gg/ARTMvTQv)
 [![Twitter Follow](https://img.shields.io/twitter/follow/seii_saintway?style=social)](https://twitter.com/seii_saintway)
 
 ## Setup iPyMock
 
-Get your access_token at [openai api session](https://chat.openai.com/api/auth/session) and the conversation_id in the url of chat.openai.com/c/\<conversation_id\>
+`gmail_address` and `gmail_password` are needed for utilizing chrome automation locally.
+
+`conversation_id` could be found in the url of `chat.openai.com/c/<conversation_id>`.
+
+```bash
+mkdir -p ~/.config/ipymock
+
+cat << EOF > ~/.config/ipymock/config.json
+{
+  "email": "<gmail_address>",
+  "password": "<gmail_password>",
+  "conversation_id": "<conversation_id>"
+}
+EOF
+
+pip install --upgrade ipymock
+```
+
+`access_token` at [openai api session](https://chat.openai.com/api/auth/session) are needed for utilizing a backend api proxy.
 
 ```bash
 mkdir -p ~/.config/ipymock
 
 cat << EOF > ~/.config/ipymock/config.json
 {
+  "chat_gpt_base_url": "<chat_gpt_base_url>",
   "access_token": "<access_token>",
   "conversation_id": "<conversation_id>"
 }
 EOF
 
 pip install --upgrade ipymock
 ```
 
-## Using the Browser Side API in Jupyter Notebooks
+## Using the OpenAI Backend API from Browser Side in Jupyter Notebooks
 
 ```python
 from ipymock.browser import start_conversation
 import IPython
 
 def ask(prompt):
     for response in start_conversation(prompt):
         IPython.display.display(IPython.core.display.Markdown(response))
         IPython.display.clear_output(wait=True)
 
 import ipymock.browser
-# if the proxy is deployed locally
+# 1. you could initialize chrome automation locally
+ipymock.browser.init(['--headless'])
+# 2. or if a proxy is deployed locally
 ipymock.browser.common.chat_gpt_base_url = 'http://127.0.0.1:8080'
-# otherwise using a third party proxy
+# 3. otherwise using a third party proxy
 ipymock.browser.common.chat_gpt_base_url = 'https://.../api'
 # the conversation_id which is set in config.json
 print(ipymock.browser.common.conversation_id)
 
 ask('''
 what is the meaning of getting patched?
 ''')
@@ -104,17 +105,17 @@
 
 ```python
 import ipymock
 import ipymock.browser
 import ipymock.llm
 import pytest
 
-ipymock.browser.common.chat_gpt_base_url = 'http://127.0.0.1:8080'
 # reset conversation_id to empty to start a new chat
 ipymock.browser.common.conversation_id = ''
+ipymock.browser.init()
 
 @pytest.fixture
 def reset_embed_dimension(monkeypatch):
     import autogpt.memory.local
     monkeypatch.setattr(autogpt.memory.local, 'EMBED_DIM', 1024)
 
 ipymock.do(
@@ -127,15 +128,15 @@
 
 This project is still under development and lack of documentation.
 
 This is [an article](https://seii-saintway.github.io/2023/04/06/Autonomous-Agents/) I wrote that mock openai to test autonomous robots.
 
 ## The Mechanism of PyTesting the Python Testfiles
 
-```
+```python
 import pluggy
 pm = pluggy.PluginManager('pytest')
 
 import _pytest.hookspec
 pm.add_hookspecs(_pytest.hookspec)
 
 import _pytest.main
@@ -143,24 +144,24 @@
 
 import _pytest.config
 cfg = _pytest.config.get_config()
 cfg.parse(args=[])
 pm.hook.pytest_cmdline_main(config=cfg)
 ```
 
-```
+```python
 import _pytest.config
 cfg = _pytest.config.get_config()
 cfg.parse(args=[])
 cfg.pluginmanager.hook.pytest_cmdline_main(config=cfg)
 ```
 
 ### PyTesting the Python Testcases within iPyNb Runtimes
 
-```
+```python
 # content of test_time.py
 
 import pytest
 
 from datetime import datetime, timedelta
 
 
@@ -206,15 +207,15 @@
     ],
 )
 def test_timedistance_v3(a, b, expected):
     diff = a - b
     assert diff != expected
 ```
 
-```
+```python
 import _pytest.config
 cfg = _pytest.config.get_config()
 cfg.parse(args=[])
 
 import _pytest.main
 ss = _pytest.main.Session.from_config(cfg)
 import _pytest.runner
@@ -223,22 +224,22 @@
 ss._fixturemanager = _pytest.fixtures.FixtureManager(ss)
 
 import _pytest.python
 import py
 m = _pytest.python.Module.from_parent(parent=ss, fspath=py.path.local())
 ```
 
-```
+```python
 class Object(object):
     def __init__(self, **entries):
         self.__dict__.update(entries)
 m.obj = Object(**globals())
 ```
 
-```
+```python
 import _pytest.runner
 c = dict(enumerate(m.collect()))
 for i in c:
     print(f'idx = {i}')
     print(_pytest.runner.call_and_report(c[i], 'setup'))
     print(_pytest.runner.call_and_report(c[i], 'call'))
     print(_pytest.runner.call_and_report(c[i], 'teardown', nextitem=c.get(i+1)))
@@ -283,34 +284,34 @@
     print(f'idx = {i}')
     f.setup()
     f.runtest()
 ```
 
 ### How to Use the Do-PyTest?
 
-```
+```python
 import pytest
 
 @pytest.fixture
 def my_fixture_1(tmpdir_factory):
     return tmpdir_factory
 
 @pytest.fixture
 def my_fixture_2(tmpdir_factory):
     return tmpdir_factory
 
 def test_fixture(my_fixture_1, my_fixture_2):
     assert my_fixture_1 == my_fixture_2
 ```
 
-```
+```python
 from ipymock import do
 ```
 
-```
+```python
 do(
     my_fixture_1=my_fixture_1,
     my_fixture_2=my_fixture_2,
     test_fixture=test_fixture
 )
 ```
```

### Comparing `ipymock-1.1.0/README.md` & `ipymock-1.1.1/PKG-INFO`

 * *Files 25% similar despite different names*

```diff
@@ -1,46 +1,87 @@
+Metadata-Version: 2.1
+Name: ipymock
+Version: 1.1.1
+Summary: A Tool that Allows You Run PyTest within Jupyter Notebook Cells
+Home-page: https://github.com/seii-saintway/ipymock/tree/main/
+Author: andrew
+Author-email: andrew.saintway@gmail.com
+License: Apache Software License 2.0
+Keywords: pytest interactive jupyter
+Classifier: Development Status :: 3 - Alpha
+Classifier: Intended Audience :: Developers
+Classifier: Natural Language :: English
+Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: License :: OSI Approved :: Apache Software License
+Requires-Python: >=3.6
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # Running PyTest in Jupyter Notebooks
-> iPyMock uses GPT 3.5 turbo by browser automation and <a href='https://huggingface.co/GanymedeNil/text2vec-large-chinese'>a CoSENT based model</a> to embed English and Chinese.
 
+> iPyMock uses GPT 3.5 turbo by browser automation and <a href='https://huggingface.co/GanymedeNil/text2vec-large-chinese'>a CoSENT based model</a> to embed English and Chinese.
 
 [![Discord Follow](https://dcbadge.vercel.app/api/server/ARTMvTQv?style=flat)](https://discord.gg/ARTMvTQv)
 [![Twitter Follow](https://img.shields.io/twitter/follow/seii_saintway?style=social)](https://twitter.com/seii_saintway)
 
 ## Setup iPyMock
 
-Get your access_token at [openai api session](https://chat.openai.com/api/auth/session) and the conversation_id in the url of chat.openai.com/c/\<conversation_id\>
+`gmail_address` and `gmail_password` are needed for utilizing chrome automation locally.
+
+`conversation_id` could be found in the url of `chat.openai.com/c/<conversation_id>`.
+
+```bash
+mkdir -p ~/.config/ipymock
+
+cat << EOF > ~/.config/ipymock/config.json
+{
+  "email": "<gmail_address>",
+  "password": "<gmail_password>",
+  "conversation_id": "<conversation_id>"
+}
+EOF
+
+pip install --upgrade ipymock
+```
+
+`access_token` at [openai api session](https://chat.openai.com/api/auth/session) are needed for utilizing a backend api proxy.
 
 ```bash
 mkdir -p ~/.config/ipymock
 
 cat << EOF > ~/.config/ipymock/config.json
 {
+  "chat_gpt_base_url": "<chat_gpt_base_url>",
   "access_token": "<access_token>",
   "conversation_id": "<conversation_id>"
 }
 EOF
 
 pip install --upgrade ipymock
 ```
 
-## Using the Browser Side API in Jupyter Notebooks
+## Using the OpenAI Backend API from Browser Side in Jupyter Notebooks
 
 ```python
 from ipymock.browser import start_conversation
 import IPython
 
 def ask(prompt):
     for response in start_conversation(prompt):
         IPython.display.display(IPython.core.display.Markdown(response))
         IPython.display.clear_output(wait=True)
 
 import ipymock.browser
-# if the proxy is deployed locally
+# 1. you could initialize chrome automation locally
+ipymock.browser.init(['--headless'])
+# 2. or if a proxy is deployed locally
 ipymock.browser.common.chat_gpt_base_url = 'http://127.0.0.1:8080'
-# otherwise using a third party proxy
+# 3. otherwise using a third party proxy
 ipymock.browser.common.chat_gpt_base_url = 'https://.../api'
 # the conversation_id which is set in config.json
 print(ipymock.browser.common.conversation_id)
 
 ask('''
 what is the meaning of getting patched?
 ''')
@@ -84,17 +125,17 @@
 
 ```python
 import ipymock
 import ipymock.browser
 import ipymock.llm
 import pytest
 
-ipymock.browser.common.chat_gpt_base_url = 'http://127.0.0.1:8080'
 # reset conversation_id to empty to start a new chat
 ipymock.browser.common.conversation_id = ''
+ipymock.browser.init()
 
 @pytest.fixture
 def reset_embed_dimension(monkeypatch):
     import autogpt.memory.local
     monkeypatch.setattr(autogpt.memory.local, 'EMBED_DIM', 1024)
 
 ipymock.do(
@@ -107,15 +148,15 @@
 
 This project is still under development and lack of documentation.
 
 This is [an article](https://seii-saintway.github.io/2023/04/06/Autonomous-Agents/) I wrote that mock openai to test autonomous robots.
 
 ## The Mechanism of PyTesting the Python Testfiles
 
-```
+```python
 import pluggy
 pm = pluggy.PluginManager('pytest')
 
 import _pytest.hookspec
 pm.add_hookspecs(_pytest.hookspec)
 
 import _pytest.main
@@ -123,24 +164,24 @@
 
 import _pytest.config
 cfg = _pytest.config.get_config()
 cfg.parse(args=[])
 pm.hook.pytest_cmdline_main(config=cfg)
 ```
 
-```
+```python
 import _pytest.config
 cfg = _pytest.config.get_config()
 cfg.parse(args=[])
 cfg.pluginmanager.hook.pytest_cmdline_main(config=cfg)
 ```
 
 ### PyTesting the Python Testcases within iPyNb Runtimes
 
-```
+```python
 # content of test_time.py
 
 import pytest
 
 from datetime import datetime, timedelta
 
 
@@ -186,15 +227,15 @@
     ],
 )
 def test_timedistance_v3(a, b, expected):
     diff = a - b
     assert diff != expected
 ```
 
-```
+```python
 import _pytest.config
 cfg = _pytest.config.get_config()
 cfg.parse(args=[])
 
 import _pytest.main
 ss = _pytest.main.Session.from_config(cfg)
 import _pytest.runner
@@ -203,22 +244,22 @@
 ss._fixturemanager = _pytest.fixtures.FixtureManager(ss)
 
 import _pytest.python
 import py
 m = _pytest.python.Module.from_parent(parent=ss, fspath=py.path.local())
 ```
 
-```
+```python
 class Object(object):
     def __init__(self, **entries):
         self.__dict__.update(entries)
 m.obj = Object(**globals())
 ```
 
-```
+```python
 import _pytest.runner
 c = dict(enumerate(m.collect()))
 for i in c:
     print(f'idx = {i}')
     print(_pytest.runner.call_and_report(c[i], 'setup'))
     print(_pytest.runner.call_and_report(c[i], 'call'))
     print(_pytest.runner.call_and_report(c[i], 'teardown', nextitem=c.get(i+1)))
@@ -263,34 +304,34 @@
     print(f'idx = {i}')
     f.setup()
     f.runtest()
 ```
 
 ### How to Use the Do-PyTest?
 
-```
+```python
 import pytest
 
 @pytest.fixture
 def my_fixture_1(tmpdir_factory):
     return tmpdir_factory
 
 @pytest.fixture
 def my_fixture_2(tmpdir_factory):
     return tmpdir_factory
 
 def test_fixture(my_fixture_1, my_fixture_2):
     assert my_fixture_1 == my_fixture_2
 ```
 
-```
+```python
 from ipymock import do
 ```
 
-```
+```python
 do(
     my_fixture_1=my_fixture_1,
     my_fixture_2=my_fixture_2,
     test_fixture=test_fixture
 )
 ```
```

### Comparing `ipymock-1.1.0/ipymock/__init__.py` & `ipymock-1.1.1/ipymock/__init__.py`

 * *Files identical despite different names*

### Comparing `ipymock-1.1.0/ipymock/_nbdev.py` & `ipymock-1.1.1/ipymock/_nbdev.py`

 * *Files 2% similar despite different names*

```diff
@@ -12,26 +12,31 @@
          "handle_conversation_detail": "2_browser.ipynb",
          "start_conversation": "2_browser.ipynb",
          "generate_title": "2_browser.ipynb",
          "rename_title": "2_browser.ipynb",
          "delete_conversation": "2_browser.ipynb",
          "recover_conversation": "2_browser.ipynb",
          "clear_conversations": "2_browser.ipynb",
+         "ChatGPTConverter": "2_browser.ipynb",
+         "markdownize": "2_browser.ipynb",
          "init": "2_browser.ipynb",
          "login": "2_browser.ipynb",
          "open_chat": "2_browser.ipynb",
          "remove_portal": "2_browser.ipynb",
          "chatgpt_textbox": "2_browser.ipynb",
          "chatgpt_streaming": "2_browser.ipynb",
+         "chatgpt_response": "2_browser.ipynb",
+         "chatgpt_red_500": "2_browser.ipynb",
          "chatgpt_big_response": "2_browser.ipynb",
          "chatgpt_small_response": "2_browser.ipynb",
          "request": "2_browser.ipynb",
          "get_last_response": "2_browser.ipynb",
          "get_response": "2_browser.ipynb",
          "ask": "2_browser.ipynb",
+         "get_screenshot": "2_browser.ipynb",
          "attrdict": "2_browser.ipynb",
          "attributize": "2_browser.ipynb",
          "retry_on_status_code": "2_browser.ipynb",
          "content": "2_browser.ipynb",
          "new_id": "2_browser.ipynb",
          "delta": "2_browser.ipynb",
          "chat_delta": "2_browser.ipynb",
```

### Comparing `ipymock-1.1.0/ipymock/agi.py` & `ipymock-1.1.1/ipymock/agi.py`

 * *Files identical despite different names*

### Comparing `ipymock-1.1.0/ipymock/browser.py` & `ipymock-1.1.1/ipymock/browser.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 # AUTOGENERATED! DO NOT EDIT! File to edit: nbs/2_browser.ipynb (unless otherwise specified).
 
 __all__ = ['common', 'get_conversations', 'get_conversation', 'handle_conversation_detail', 'start_conversation',
            'generate_title', 'rename_title', 'delete_conversation', 'recover_conversation', 'clear_conversations',
            'init', 'login', 'open_chat', 'remove_portal', 'request', 'get_last_response', 'get_response', 'ask',
-           'attrdict', 'attributize', 'retry_on_status_code', 'content', 'new_id', 'delta', 'chat_delta', 'mock_create',
-           'mock_chat_create', 'mock_openai']
+           'get_screenshot', 'attrdict', 'attributize', 'retry_on_status_code', 'content', 'new_id', 'delta',
+           'chat_delta', 'mock_create', 'mock_chat_create', 'mock_openai']
 
 # Internal Cell
 from queue import Queue
 
 class Common:
     chat_gpt_base_url = 'http://127.0.0.1:8080'
     access_token = None
@@ -233,30 +233,52 @@
     requests.patch(f'{common.chat_gpt_base_url}/conversations', headers = {'Authorization': f'Bearer {common.access_token}'}, data = {'is_visible': False})
 
     common.conversation_id = ''
     common.parent_message_id = ''
     common.reload_conversations_channel.put(True)
 
 # Internal Cell
+from selenium.common.exceptions import StaleElementReferenceException, TimeoutException
 from selenium.webdriver.common.action_chains import ActionChains
 from selenium.webdriver.common.by import By
 from selenium.webdriver.common.keys import Keys
 from selenium.webdriver.support import expected_conditions
 from selenium.webdriver.support.ui import WebDriverWait
 
 import undetected_chromedriver as uc
 
+# Internal Cell
+from markdownify import MarkdownConverter
+
+class ChatGPTConverter(MarkdownConverter):
+    def convert_a(self, node, text, convert_as_inline):
+        if node.get('href') == text:
+            return node.get('href')
+        return f"[{text}]({node.get('href')})"
+
+    def convert_pre(self, node, text, convert_as_inline):
+        node_code = node.find('code')
+        return (
+            f"```{' '.join([c[len('language-'):] for c in node_code.get('class') if c.startswith('language-')])}\n"
+            f'{node_code.text.strip()}\n'
+            '```\n'
+        )
+
+markdownize = ChatGPTConverter().convert
+
 # Cell
-def init():
+def init(chrome_args = None):
     options = uc.ChromeOptions()
-    options.add_argument('--headless')
+    if isinstance(chrome_args, list):
+        for arg in chrome_args:
+            options.add_argument(arg)
     common.driver = uc.Chrome(options = options)
 
     login()
-    open_chat()
+    open_chat(common.conversation_id)
 
     global start_conversation
     start_conversation = ask
 
 def login():
     common.driver.get('https://chat.openai.com/auth/login')
 
@@ -323,82 +345,117 @@
         view: window,
         bubbles: true,
         cancelable: true
       })
     );
     ''')
 
-    WebDriverWait(common.driver, 5).until(
+    WebDriverWait(common.driver, 10).until(
         expected_conditions.element_to_be_clickable((By.XPATH, '//input[@type="password"]'))
     ).click()
 
     ActionChains(common.driver).send_keys(common.config['password']).send_keys(Keys.ENTER).perform()
 
     remove_portal()
 
-def open_chat():
-    common.driver.get(f'https://chat.openai.com/c/{common.config["conversation_id"]}')
+def open_chat(conversation_id = ''):
+    if conversation_id == '':
+        common.driver.get('https://chat.openai.com')
+    else:
+        common.driver.get(f'https://chat.openai.com/c/{conversation_id}')
+        if common.conversation_id != conversation_id:
+            common.conversation_id = conversation_id
+            common.parent_message_id = ''
     remove_portal()
 
 def remove_portal():
     WebDriverWait(common.driver, 10).until(
         expected_conditions.presence_of_element_located((By.ID, 'headlessui-portal-root'))
     )
 
     common.driver.execute_script('''
     document.getElementById('headlessui-portal-root').remove();
     ''')
 
 # Internal Cell
 chatgpt_textbox = (By.TAG_NAME, 'textarea')
 chatgpt_streaming = (By.CLASS_NAME, 'result-streaming')
+chatgpt_response = (By.XPATH, '//div[starts-with(@class, "flex flex-grow flex-col gap-3")]')
+chatgpt_red_500 = (By.XPATH, '//div[contains(@class, "border-red-500 bg-red-500/10")]')
 chatgpt_big_response = (By.XPATH, '//div[@class="flex-1 overflow-hidden"]//div[p]')
 chatgpt_small_response = (By.XPATH, '//div[starts-with(@class, "markdown prose w-full break-words")]')
 
 # Cell
 def request(prompt: str) -> None:
-    textbox = WebDriverWait(common.driver, 5).until(
-        expected_conditions.element_to_be_clickable(chatgpt_textbox)
-    )
+    try:
+        textbox = WebDriverWait(common.driver, 5).until(
+            expected_conditions.element_to_be_clickable(chatgpt_textbox)
+        )
+    except TimeoutException:
+        open_chat(common.conversation_id)
+        textbox = WebDriverWait(common.driver, 5).until(
+            expected_conditions.element_to_be_clickable(chatgpt_textbox)
+        )
     textbox.click()
     common.driver.execute_script('''
-var element = arguments[0], txt = arguments[1];
-element.value += txt;
-element.dispatchEvent(new Event("change"));
-''',
+    var element = arguments[0], txt = arguments[1];
+    element.value += txt;
+    element.dispatchEvent(new Event("change"));
+    ''',
         textbox,
         prompt,
     )
     textbox.send_keys(Keys.ENTER)
 
 def get_last_response():
     responses = common.driver.find_elements(*chatgpt_big_response)
-    if responses:
-        response = responses[-1]
-        if 'text-red' in response.get_attribute('class'):
-            raise ValueError(response.text)
-        return response
-    return common.driver.find_elements(*chatgpt_small_response)[-1]
+    if responses != []:
+        return responses[-1]
+    responses = common.driver.find_elements(*chatgpt_small_response)
+    if responses != []:
+        return responses[-1]
 
 def get_response() -> str:
-    result_streaming = WebDriverWait(common.driver, 3).until(
-        expected_conditions.presence_of_element_located(chatgpt_streaming)
-    )
+    try:
+        result_streaming = WebDriverWait(common.driver, 30).until(
+            expected_conditions.presence_of_element_located(chatgpt_streaming)
+        )
+    except TimeoutException:
+        response = common.driver.find_elements(*chatgpt_response)[-1]
+        is_error = common.driver.find_elements(*chatgpt_red_500) != []
+        sys.stderr.write(
+            'TimeoutException: having waited 30 seconds for result-streaming\n'
+            f'response.text = {response.text}\n'
+            f'is_error = {is_error}\n'
+        )
+        if not is_error:
+            yield markdownize(response.get_attribute('innerHTML'))
+        return
     while result_streaming:
         response = get_last_response()
-        response = response.get_attribute('innerHTML')
-        yield response
+        try:
+            if 'text-red' in response.get_attribute('class'):
+                sys.stderr.write(f'Error Responding: response.text = {response.text}\n')
+            yield markdownize(response.get_attribute('innerHTML'))
+        except StaleElementReferenceException:
+            pass
         result_streaming = common.driver.find_elements(*chatgpt_streaming)
     response = get_last_response()
-    yield response.get_attribute('innerHTML')
+    yield markdownize(response.get_attribute('innerHTML'))
 
 def ask(prompt: str) -> str:
     request(prompt)
     return get_response()
 
+# Cell
+import io, PIL.Image
+
+def get_screenshot() -> 'PIL.PngImagePlugin.PngImageFile':
+    return PIL.Image.open(io.BytesIO(common.driver.get_screenshot_as_png()))
+
 # Internal Cell
 import random, string
 
 # Cell
 class attrdict(dict):
     def __getattr__(self, attr):
         return self.get(attr)
@@ -439,19 +496,19 @@
                 break
     return wrapper
 
 @retry_on_status_code
 def content(prompt):
     for response in start_conversation(prompt):
         pass
-    if response == '':
+    if locals().get('response') == '':
         sys.stderr.write(
             f'Error Responding: response = {repr(response)}\n'
         )
-    return response
+    return locals().get('response', '')
 
 def new_id():
     return ''.join(
         random.choices(string.ascii_letters + string.digits, k = 29)
     )
 
 def delta(prompt):
@@ -464,15 +521,15 @@
                     'logprobs': None,
                     'text': response[len(res):],
                 }
             ],
             'id': f'cmpl-{new_id()}',
         })
         res = response
-    if response == '':
+    if locals().get('response') == '':
         sys.stderr.write(
             f'Error Responding: response = {repr(response)}\n'
         )
 
 def chat_delta(prompt):
     res = ''
     for response in start_conversation(prompt):
@@ -484,15 +541,15 @@
                         'content': response[len(res):],
                     }
                 }
             ],
             'id': f'chatcmpl-{new_id()}',
         })
         res = response
-    if response == '':
+    if locals().get('response') == '':
         sys.stderr.write(
             f'Error Responding: response = {repr(response)}\n'
         )
 
 def mock_create(*args, **kwargs):
     prompts = []
     if isinstance(kwargs['prompt'], str):
```

### Comparing `ipymock-1.1.0/ipymock/llm.py` & `ipymock-1.1.1/ipymock/llm.py`

 * *Files identical despite different names*

### Comparing `ipymock-1.1.0/ipymock/reader.py` & `ipymock-1.1.1/ipymock/reader.py`

 * *Files identical despite different names*

### Comparing `ipymock-1.1.0/ipymock.egg-info/PKG-INFO` & `ipymock-1.1.1/ipymock.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ipymock
-Version: 1.1.0
+Version: 1.1.1
 Summary: A Tool that Allows You Run PyTest within Jupyter Notebook Cells
 Home-page: https://github.com/seii-saintway/ipymock/tree/main/
 Author: andrew
 Author-email: andrew.saintway@gmail.com
 License: Apache Software License 2.0
 Keywords: pytest interactive jupyter
 Classifier: Development Status :: 3 - Alpha
@@ -15,52 +15,73 @@
 Classifier: Programming Language :: Python :: 3.8
 Classifier: License :: OSI Approved :: Apache Software License
 Requires-Python: >=3.6
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Running PyTest in Jupyter Notebooks
-> iPyMock uses GPT 3.5 turbo by browser automation and <a href='https://huggingface.co/GanymedeNil/text2vec-large-chinese'>a CoSENT based model</a> to embed English and Chinese.
 
+> iPyMock uses GPT 3.5 turbo by browser automation and <a href='https://huggingface.co/GanymedeNil/text2vec-large-chinese'>a CoSENT based model</a> to embed English and Chinese.
 
 [![Discord Follow](https://dcbadge.vercel.app/api/server/ARTMvTQv?style=flat)](https://discord.gg/ARTMvTQv)
 [![Twitter Follow](https://img.shields.io/twitter/follow/seii_saintway?style=social)](https://twitter.com/seii_saintway)
 
 ## Setup iPyMock
 
-Get your access_token at [openai api session](https://chat.openai.com/api/auth/session) and the conversation_id in the url of chat.openai.com/c/\<conversation_id\>
+`gmail_address` and `gmail_password` are needed for utilizing chrome automation locally.
+
+`conversation_id` could be found in the url of `chat.openai.com/c/<conversation_id>`.
+
+```bash
+mkdir -p ~/.config/ipymock
+
+cat << EOF > ~/.config/ipymock/config.json
+{
+  "email": "<gmail_address>",
+  "password": "<gmail_password>",
+  "conversation_id": "<conversation_id>"
+}
+EOF
+
+pip install --upgrade ipymock
+```
+
+`access_token` at [openai api session](https://chat.openai.com/api/auth/session) are needed for utilizing a backend api proxy.
 
 ```bash
 mkdir -p ~/.config/ipymock
 
 cat << EOF > ~/.config/ipymock/config.json
 {
+  "chat_gpt_base_url": "<chat_gpt_base_url>",
   "access_token": "<access_token>",
   "conversation_id": "<conversation_id>"
 }
 EOF
 
 pip install --upgrade ipymock
 ```
 
-## Using the Browser Side API in Jupyter Notebooks
+## Using the OpenAI Backend API from Browser Side in Jupyter Notebooks
 
 ```python
 from ipymock.browser import start_conversation
 import IPython
 
 def ask(prompt):
     for response in start_conversation(prompt):
         IPython.display.display(IPython.core.display.Markdown(response))
         IPython.display.clear_output(wait=True)
 
 import ipymock.browser
-# if the proxy is deployed locally
+# 1. you could initialize chrome automation locally
+ipymock.browser.init(['--headless'])
+# 2. or if a proxy is deployed locally
 ipymock.browser.common.chat_gpt_base_url = 'http://127.0.0.1:8080'
-# otherwise using a third party proxy
+# 3. otherwise using a third party proxy
 ipymock.browser.common.chat_gpt_base_url = 'https://.../api'
 # the conversation_id which is set in config.json
 print(ipymock.browser.common.conversation_id)
 
 ask('''
 what is the meaning of getting patched?
 ''')
@@ -104,17 +125,17 @@
 
 ```python
 import ipymock
 import ipymock.browser
 import ipymock.llm
 import pytest
 
-ipymock.browser.common.chat_gpt_base_url = 'http://127.0.0.1:8080'
 # reset conversation_id to empty to start a new chat
 ipymock.browser.common.conversation_id = ''
+ipymock.browser.init()
 
 @pytest.fixture
 def reset_embed_dimension(monkeypatch):
     import autogpt.memory.local
     monkeypatch.setattr(autogpt.memory.local, 'EMBED_DIM', 1024)
 
 ipymock.do(
@@ -127,15 +148,15 @@
 
 This project is still under development and lack of documentation.
 
 This is [an article](https://seii-saintway.github.io/2023/04/06/Autonomous-Agents/) I wrote that mock openai to test autonomous robots.
 
 ## The Mechanism of PyTesting the Python Testfiles
 
-```
+```python
 import pluggy
 pm = pluggy.PluginManager('pytest')
 
 import _pytest.hookspec
 pm.add_hookspecs(_pytest.hookspec)
 
 import _pytest.main
@@ -143,24 +164,24 @@
 
 import _pytest.config
 cfg = _pytest.config.get_config()
 cfg.parse(args=[])
 pm.hook.pytest_cmdline_main(config=cfg)
 ```
 
-```
+```python
 import _pytest.config
 cfg = _pytest.config.get_config()
 cfg.parse(args=[])
 cfg.pluginmanager.hook.pytest_cmdline_main(config=cfg)
 ```
 
 ### PyTesting the Python Testcases within iPyNb Runtimes
 
-```
+```python
 # content of test_time.py
 
 import pytest
 
 from datetime import datetime, timedelta
 
 
@@ -206,15 +227,15 @@
     ],
 )
 def test_timedistance_v3(a, b, expected):
     diff = a - b
     assert diff != expected
 ```
 
-```
+```python
 import _pytest.config
 cfg = _pytest.config.get_config()
 cfg.parse(args=[])
 
 import _pytest.main
 ss = _pytest.main.Session.from_config(cfg)
 import _pytest.runner
@@ -223,22 +244,22 @@
 ss._fixturemanager = _pytest.fixtures.FixtureManager(ss)
 
 import _pytest.python
 import py
 m = _pytest.python.Module.from_parent(parent=ss, fspath=py.path.local())
 ```
 
-```
+```python
 class Object(object):
     def __init__(self, **entries):
         self.__dict__.update(entries)
 m.obj = Object(**globals())
 ```
 
-```
+```python
 import _pytest.runner
 c = dict(enumerate(m.collect()))
 for i in c:
     print(f'idx = {i}')
     print(_pytest.runner.call_and_report(c[i], 'setup'))
     print(_pytest.runner.call_and_report(c[i], 'call'))
     print(_pytest.runner.call_and_report(c[i], 'teardown', nextitem=c.get(i+1)))
@@ -283,34 +304,34 @@
     print(f'idx = {i}')
     f.setup()
     f.runtest()
 ```
 
 ### How to Use the Do-PyTest?
 
-```
+```python
 import pytest
 
 @pytest.fixture
 def my_fixture_1(tmpdir_factory):
     return tmpdir_factory
 
 @pytest.fixture
 def my_fixture_2(tmpdir_factory):
     return tmpdir_factory
 
 def test_fixture(my_fixture_1, my_fixture_2):
     assert my_fixture_1 == my_fixture_2
 ```
 
-```
+```python
 from ipymock import do
 ```
 
-```
+```python
 do(
     my_fixture_1=my_fixture_1,
     my_fixture_2=my_fixture_2,
     test_fixture=test_fixture
 )
 ```
```

### Comparing `ipymock-1.1.0/settings.ini` & `ipymock-1.1.1/settings.ini`

 * *Files 2% similar despite different names*

```diff
@@ -9,27 +9,27 @@
 user = seii-saintway
 description = A Tool that Allows You Run PyTest within Jupyter Notebook Cells
 keywords = pytest interactive jupyter
 author = andrew
 author_email = andrew.saintway@gmail.com
 copyright = 2023 onwards, Neuro Spirit, DAO.
 branch = main
-version = 1.1.0
+version = 1.1.1
 min_python = 3.6
 audience = Developers
 language = English
 # Set to True if you want to create a more fancy sidebar.json than the default
 custom_sidebar = False
 # Add licenses and see current list in `setup.py`
 license = apache2
 # From 1-7: Planning Pre-Alpha Alpha Beta Production Mature Inactive
 status = 2
 
 # Optional. Same format as setuptools requirements
-requirements = pytest==6.* nbdev==1.* openai==0.* sentence_transformers==2.* pydantic==1.* langchain==0.* faiss-cpu==1.* duckduckgo_search==2.*
+requirements = pytest==6.* nbdev==1.* openai==0.* sentence_transformers==2.* pydantic==1.* langchain==0.* faiss-cpu==1.* duckduckgo_search==2.* undetected_chromedriver==3.* selenium_profiles==2.*
 # Optional. Same format as setuptools console_scripts
 # console_scripts = 
 # Optional. Same format as setuptools dependency-links
 # dep_links = 
 
 ###
 # You probably won't need to change anything under here,
```

### Comparing `ipymock-1.1.0/setup.py` & `ipymock-1.1.1/setup.py`

 * *Files identical despite different names*

