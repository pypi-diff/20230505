# Comparing `tmp/pybotx_fsm-0.4.7.tar.gz` & `tmp/pybotx_fsm-0.4.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pybotx_fsm-0.4.7.tar", max compression
+gzip compressed data, was "pybotx_fsm-0.4.8.tar", max compression
```

## Comparing `pybotx_fsm-0.4.7.tar` & `pybotx_fsm-0.4.8.tar`

### file list

```diff
@@ -1,12 +1,11 @@
--rw-r--r--   0        0        0     6078 2023-01-18 14:48:39.328220 pybotx_fsm-0.4.7/LICENSE.md
--rw-r--r--   0        0        0     5614 2023-01-18 14:48:39.328220 pybotx_fsm-0.4.7/README.md
--rw-r--r--   0        0        0      192 2023-01-18 14:48:39.328220 pybotx_fsm-0.4.7/pybotx_fsm/__init__.py
--rw-r--r--   0        0        0     1147 2023-01-18 14:48:39.328220 pybotx_fsm-0.4.7/pybotx_fsm/collector.py
--rw-r--r--   0        0        0     1711 2023-01-18 14:48:39.328220 pybotx_fsm-0.4.7/pybotx_fsm/fsm.py
--rw-r--r--   0        0        0     2211 2023-01-18 14:48:39.328220 pybotx_fsm-0.4.7/pybotx_fsm/middleware.py
--rw-r--r--   0        0        0        0 2023-01-18 14:48:39.332220 pybotx_fsm-0.4.7/pybotx_fsm/py.typed
--rw-r--r--   0        0        0      451 2023-01-18 14:48:39.332220 pybotx_fsm-0.4.7/pybotx_fsm/state_repo_proto.py
--rw-r--r--   0        0        0      122 2023-01-18 14:48:39.332220 pybotx_fsm-0.4.7/pybotx_fsm/templates.py
--rw-r--r--   0        0        0      549 2023-01-18 14:48:39.332220 pybotx_fsm-0.4.7/pyproject.toml
--rw-r--r--   0        0        0     6404 1970-01-01 00:00:00.000000 pybotx_fsm-0.4.7/setup.py
--rw-r--r--   0        0        0     6025 1970-01-01 00:00:00.000000 pybotx_fsm-0.4.7/PKG-INFO
+-rw-r--r--   0        0        0     6078 2023-05-05 08:17:15.901056 pybotx_fsm-0.4.8/LICENSE.md
+-rw-r--r--   0        0        0     5614 2023-05-05 08:17:15.901056 pybotx_fsm-0.4.8/README.md
+-rw-r--r--   0        0        0      192 2023-05-05 08:17:15.901056 pybotx_fsm-0.4.8/pybotx_fsm/__init__.py
+-rw-r--r--   0        0        0     1147 2023-05-05 08:17:15.901056 pybotx_fsm-0.4.8/pybotx_fsm/collector.py
+-rw-r--r--   0        0        0     1711 2023-05-05 08:17:15.901056 pybotx_fsm-0.4.8/pybotx_fsm/fsm.py
+-rw-r--r--   0        0        0     2211 2023-05-05 08:17:15.901056 pybotx_fsm-0.4.8/pybotx_fsm/middleware.py
+-rw-r--r--   0        0        0        0 2023-05-05 08:17:15.901056 pybotx_fsm-0.4.8/pybotx_fsm/py.typed
+-rw-r--r--   0        0        0      451 2023-05-05 08:17:15.901056 pybotx_fsm-0.4.8/pybotx_fsm/state_repo_proto.py
+-rw-r--r--   0        0        0      122 2023-05-05 08:17:15.901056 pybotx_fsm-0.4.8/pybotx_fsm/templates.py
+-rw-r--r--   0        0        0      549 2023-05-05 08:17:15.901056 pybotx_fsm-0.4.8/pyproject.toml
+-rw-r--r--   0        0        0     6025 1970-01-01 00:00:00.000000 pybotx_fsm-0.4.8/PKG-INFO
```

### Comparing `pybotx_fsm-0.4.7/LICENSE.md` & `pybotx_fsm-0.4.8/LICENSE.md`

 * *Files identical despite different names*

### Comparing `pybotx_fsm-0.4.7/README.md` & `pybotx_fsm-0.4.8/README.md`

 * *Files identical despite different names*

### Comparing `pybotx_fsm-0.4.7/pybotx_fsm/collector.py` & `pybotx_fsm-0.4.8/pybotx_fsm/collector.py`

 * *Files identical despite different names*

### Comparing `pybotx_fsm-0.4.7/pybotx_fsm/fsm.py` & `pybotx_fsm-0.4.8/pybotx_fsm/fsm.py`

 * *Files identical despite different names*

### Comparing `pybotx_fsm-0.4.7/pybotx_fsm/middleware.py` & `pybotx_fsm-0.4.8/pybotx_fsm/middleware.py`

 * *Files identical despite different names*

### Comparing `pybotx_fsm-0.4.7/pyproject.toml` & `pybotx_fsm-0.4.8/pyproject.toml`

 * *Files 19% similar despite different names*

```diff
@@ -1,20 +1,20 @@
 # https://python-poetry.org/docs/
 
 [tool.poetry]
 name = "pybotx-fsm"
-version = "0.4.7"
+version = "0.4.8"
 description = "FSM middleware for using with pybotx"
 readme = "README.md"
 authors = []
 
 [tool.poetry.dependencies]
 python = ">=3.8,<3.11"
 
-pybotx = ">=0.44.1,<0.54.0"
+pybotx = ">=0.44.1,<0.56.0"
 
 [tool.poetry.dev-dependencies]
 add-trailing-comma = "2.2.3"
 autoflake = "1.4.0"
 black = "22.3.0"
 isort = "5.10.1"
 mypy = "0.950.0"
```

### Comparing `pybotx_fsm-0.4.7/setup.py` & `pybotx_fsm-0.4.8/PKG-INFO`

 * *Files 16% similar despite different names*

```diff
@@ -1,30 +1,194 @@
-# -*- coding: utf-8 -*-
-from setuptools import setup
+Metadata-Version: 2.1
+Name: pybotx-fsm
+Version: 0.4.8
+Summary: FSM middleware for using with pybotx
+Requires-Python: >=3.8,<3.11
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Requires-Dist: pybotx (>=0.44.1,<0.56.0)
+Description-Content-Type: text/markdown
 
-packages = \
-['pybotx_fsm']
+# pybotx-fsm
 
-package_data = \
-{'': ['*']}
+[![codecov](https://codecov.io/gh/ExpressApp/pybotx-fsm/branch/master/graph/badge.svg?token=JWT9JWU2Z4)](https://codecov.io/gh/ExpressApp/pybotx-fsm)
 
-install_requires = \
-['pybotx>=0.44.1,<0.54.0']
-
-setup_kwargs = {
-    'name': 'pybotx-fsm',
-    'version': '0.4.7',
-    'description': 'FSM middleware for using with pybotx',
-    'long_description': '# pybotx-fsm\n\n[![codecov](https://codecov.io/gh/ExpressApp/pybotx-fsm/branch/master/graph/badge.svg?token=JWT9JWU2Z4)](https://codecov.io/gh/ExpressApp/pybotx-fsm)\n\nКонечный автомат (Finite state machine) для ботов на базе библиотеки\n[pybotx](https://github.com/ExpressApp/pybotx).\n\n\n## Возможности\n\n* Лёгкое создание графа состояний и их переключений.\n* Передача данных в следующее состояние при явном вызове перехода.\n\n\n## Подготовка к установке\n\nДля работы библиотеки необходим Redis, который уже встроен в последние версии\n[коробки](https://github.com/ExpressApp/async-box).\n\n\n## Установка\nИспользуя `poetry`:\n\n```bash\npoetry add pybotx-fsm\n```\n\n## Работа с графом состояний\n\n1. Создайте `enum` для возможных состояний автомата:\n\n```python #fsm_init\nfrom enum import Enum, auto\n\nfrom pybotx_fsm import FSMCollector\n\n\nclass LoginStates(Enum):\n    enter_email = auto()\n    enter_password = auto()\n\n\nfsm = FSMCollector(LoginStates)\n```\n\n\n2. Добавьте экземпляр автомата в мидлвари для того, чтобы бот мог использовать его:\n\n```python #fsm_usage\nBot(\n    collectors=[\n        myfile.collector,\n    ],\n    bot_accounts=[\n        BotAccountWithSecret(\n            # Не забудьте заменить эти учётные данные на настоящие,\n            # когда создадите бота в панели администратора.\n            id=UUID("123e4567-e89b-12d3-a456-426655440000"),\n            host="cts.example.com",\n            secret_key="e29b417773f2feab9dac143ee3da20c5",\n        ),\n    ],\n    middlewares=[\n        FSMMiddleware([myfile.fsm], state_repo_key="redis_repo"),\n    ],\n)\n```\n\n3. Добавьте в `bot.state.{state_repo_key}` совместимый redis репозиторий:\n\n```python #noqa\nbot.state.redis_repo = await RedisRepo.init(...)\n```\n\n\n4. Создайте обработчики конкретных состояний:\n\n```python #fsm_state_handlers\n@fsm.on(LoginStates.enter_email)\nasync def enter_email(message: IncomingMessage, bot: Bot) -> None:\n    email = message.body\n\n    if not check_user_exist(email):\n        await bot.answer_message("Wrong email, try again")\n        return\n\n    await message.state.fsm.change_state(LoginStates.enter_password, email=email)\n    await bot.answer_message("Enter your password")\n\n\n@fsm.on(LoginStates.enter_password)\nasync def enter_password(message: IncomingMessage, bot: Bot) -> None:\n    email = message.state.fsm_storage.email\n    password = message.body\n\n    try:\n        login(email, password)\n    except IncorrectPasswordError:\n        await bot.answer_message("Wrong password, try again")\n        return\n\n    await message.state.fsm.drop_state()\n    await bot.answer_message("Success!")\n```\n\n5. Передайте управление обработчику состояний из любого обработчика сообщений:\n\n```python #fsm_change_state\n@collector.command("/login")\nasync def start_login(message: IncomingMessage, bot: Bot) -> None:\n    await bot.answer_message("Enter your email")\n    await message.state.fsm.change_state(LoginStates.enter_email)\n```\n\n\n## Примеры\n\n### Минимальный пример бота с конечным автоматом\n\n```python #fsm_sample\n# Здесь и далее будут пропущены импорты и код, не затрагивающий\n# непосредственно pybotx_fsm\nclass FsmStates(Enum):\n    EXAMPLE_STATE = auto()\n\n\nfsm = FSMCollector(FsmStates)\n\n\n@collector.command("/echo", description="Echo command")\nasync def help_command(message: IncomingMessage, bot: Bot) -> None:\n    await message.state.fsm.change_state(FsmStates.EXAMPLE_STATE)\n    await bot.answer_message("Input your text:")\n\n\n@fsm.on(FsmStates.EXAMPLE_STATE)\nasync def example_state(message: IncomingMessage, bot: Bot) -> None:\n    user_text = message.body\n    await message.state.fsm.drop_state()\n    await bot.answer_message(f"Your text is {user_text}")\n\n\nbot = Bot(\n    collectors=[\n        collector,\n    ],\n    bot_accounts=[\n        BotAccountWithSecret(\n            # Не забудьте заменить эти учётные данные на настоящие,\n            # когда создадите бота в панели администратора.\n            id=UUID("123e4567-e89b-12d3-a456-426655440000"),\n            host="cts.example.com",\n            secret_key="e29b417773f2feab9dac143ee3da20c5",\n        ),\n    ],\n    middlewares=[\n        FSMMiddleware([fsm], state_repo_key="redis_repo"),\n    ],\n)\n```\n\n\n### Передача данных между состояниями\n```python #fsm_storage\n@fsm.on(FsmStates.INPUT_FIRST_NAME)\nasync def input_first_name(message: IncomingMessage, bot: Bot) -> None:\n    first_name = message.body\n    await message.state.fsm.change_state(\n        FsmStates.INPUT_LAST_NAME,\n        first_name=first_name,\n    )\n    await bot.answer_message("Input your last name:")\n\n\n@fsm.on(FsmStates.INPUT_LAST_NAME)\nasync def input_last_name(message: IncomingMessage, bot: Bot) -> None:\n    first_name = message.state.fsm_storage.first_name\n    last_name = message.body\n    await message.state.fsm.drop_state()\n    await bot.answer_message(f"Hello {first_name} {last_name}!")\n```\n',
-    'author': 'None',
-    'author_email': 'None',
-    'maintainer': 'None',
-    'maintainer_email': 'None',
-    'url': 'None',
-    'packages': packages,
-    'package_data': package_data,
-    'install_requires': install_requires,
-    'python_requires': '>=3.8,<3.11',
-}
+Конечный автомат (Finite state machine) для ботов на базе библиотеки
+[pybotx](https://github.com/ExpressApp/pybotx).
 
 
-setup(**setup_kwargs)
+## Возможности
+
+* Лёгкое создание графа состояний и их переключений.
+* Передача данных в следующее состояние при явном вызове перехода.
+
+
+## Подготовка к установке
+
+Для работы библиотеки необходим Redis, который уже встроен в последние версии
+[коробки](https://github.com/ExpressApp/async-box).
+
+
+## Установка
+Используя `poetry`:
+
+```bash
+poetry add pybotx-fsm
+```
+
+## Работа с графом состояний
+
+1. Создайте `enum` для возможных состояний автомата:
+
+```python #fsm_init
+from enum import Enum, auto
+
+from pybotx_fsm import FSMCollector
+
+
+class LoginStates(Enum):
+    enter_email = auto()
+    enter_password = auto()
+
+
+fsm = FSMCollector(LoginStates)
+```
+
+
+2. Добавьте экземпляр автомата в мидлвари для того, чтобы бот мог использовать его:
+
+```python #fsm_usage
+Bot(
+    collectors=[
+        myfile.collector,
+    ],
+    bot_accounts=[
+        BotAccountWithSecret(
+            # Не забудьте заменить эти учётные данные на настоящие,
+            # когда создадите бота в панели администратора.
+            id=UUID("123e4567-e89b-12d3-a456-426655440000"),
+            host="cts.example.com",
+            secret_key="e29b417773f2feab9dac143ee3da20c5",
+        ),
+    ],
+    middlewares=[
+        FSMMiddleware([myfile.fsm], state_repo_key="redis_repo"),
+    ],
+)
+```
+
+3. Добавьте в `bot.state.{state_repo_key}` совместимый redis репозиторий:
+
+```python #noqa
+bot.state.redis_repo = await RedisRepo.init(...)
+```
+
+
+4. Создайте обработчики конкретных состояний:
+
+```python #fsm_state_handlers
+@fsm.on(LoginStates.enter_email)
+async def enter_email(message: IncomingMessage, bot: Bot) -> None:
+    email = message.body
+
+    if not check_user_exist(email):
+        await bot.answer_message("Wrong email, try again")
+        return
+
+    await message.state.fsm.change_state(LoginStates.enter_password, email=email)
+    await bot.answer_message("Enter your password")
+
+
+@fsm.on(LoginStates.enter_password)
+async def enter_password(message: IncomingMessage, bot: Bot) -> None:
+    email = message.state.fsm_storage.email
+    password = message.body
+
+    try:
+        login(email, password)
+    except IncorrectPasswordError:
+        await bot.answer_message("Wrong password, try again")
+        return
+
+    await message.state.fsm.drop_state()
+    await bot.answer_message("Success!")
+```
+
+5. Передайте управление обработчику состояний из любого обработчика сообщений:
+
+```python #fsm_change_state
+@collector.command("/login")
+async def start_login(message: IncomingMessage, bot: Bot) -> None:
+    await bot.answer_message("Enter your email")
+    await message.state.fsm.change_state(LoginStates.enter_email)
+```
+
+
+## Примеры
+
+### Минимальный пример бота с конечным автоматом
+
+```python #fsm_sample
+# Здесь и далее будут пропущены импорты и код, не затрагивающий
+# непосредственно pybotx_fsm
+class FsmStates(Enum):
+    EXAMPLE_STATE = auto()
+
+
+fsm = FSMCollector(FsmStates)
+
+
+@collector.command("/echo", description="Echo command")
+async def help_command(message: IncomingMessage, bot: Bot) -> None:
+    await message.state.fsm.change_state(FsmStates.EXAMPLE_STATE)
+    await bot.answer_message("Input your text:")
+
+
+@fsm.on(FsmStates.EXAMPLE_STATE)
+async def example_state(message: IncomingMessage, bot: Bot) -> None:
+    user_text = message.body
+    await message.state.fsm.drop_state()
+    await bot.answer_message(f"Your text is {user_text}")
+
+
+bot = Bot(
+    collectors=[
+        collector,
+    ],
+    bot_accounts=[
+        BotAccountWithSecret(
+            # Не забудьте заменить эти учётные данные на настоящие,
+            # когда создадите бота в панели администратора.
+            id=UUID("123e4567-e89b-12d3-a456-426655440000"),
+            host="cts.example.com",
+            secret_key="e29b417773f2feab9dac143ee3da20c5",
+        ),
+    ],
+    middlewares=[
+        FSMMiddleware([fsm], state_repo_key="redis_repo"),
+    ],
+)
+```
+
+
+### Передача данных между состояниями
+```python #fsm_storage
+@fsm.on(FsmStates.INPUT_FIRST_NAME)
+async def input_first_name(message: IncomingMessage, bot: Bot) -> None:
+    first_name = message.body
+    await message.state.fsm.change_state(
+        FsmStates.INPUT_LAST_NAME,
+        first_name=first_name,
+    )
+    await bot.answer_message("Input your last name:")
+
+
+@fsm.on(FsmStates.INPUT_LAST_NAME)
+async def input_last_name(message: IncomingMessage, bot: Bot) -> None:
+    first_name = message.state.fsm_storage.first_name
+    last_name = message.body
+    await message.state.fsm.drop_state()
+    await bot.answer_message(f"Hello {first_name} {last_name}!")
+```
+
```

