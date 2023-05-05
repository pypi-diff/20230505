# Comparing `tmp/connpy-3.0.7.tar.gz` & `tmp/connpy-3.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "connpy-3.0.7.tar", last modified: Tue Apr 18 21:02:41 2023, max compression
+gzip compressed data, was "connpy-3.2.0.tar", last modified: Fri May  5 16:42:49 2023, max compression
```

## Comparing `connpy-3.0.7.tar` & `connpy-3.2.0.tar`

### file list

```diff
@@ -1,22 +1,23 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 21:02:41.223078 connpy-3.0.7/
--rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-04-18 21:02:30.000000 connpy-3.0.7/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     7851 2023-04-18 21:02:41.223078 connpy-3.0.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7020 2023-04-18 21:02:30.000000 connpy-3.0.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 21:02:41.223078 connpy-3.0.7/connpy/
--rw-r--r--   0 runner    (1001) docker     (123)     6911 2023-04-18 21:02:30.000000 connpy-3.0.7/connpy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      181 2023-04-18 21:02:30.000000 connpy-3.0.7/connpy/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-18 21:02:30.000000 connpy-3.0.7/connpy/_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     4441 2023-04-18 21:02:30.000000 connpy-3.0.7/connpy/api.py
--rw-r--r--   0 runner    (1001) docker     (123)     3566 2023-04-18 21:02:30.000000 connpy-3.0.7/connpy/completion.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    11869 2023-04-18 21:02:30.000000 connpy-3.0.7/connpy/configfile.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    47695 2023-04-18 21:02:30.000000 connpy-3.0.7/connpy/connapp.py
--rwxr-xr-x   0 runner    (1001) docker     (123)    27894 2023-04-18 21:02:30.000000 connpy-3.0.7/connpy/core.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 21:02:41.223078 connpy-3.0.7/connpy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     7851 2023-04-18 21:02:41.000000 connpy-3.0.7/connpy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      364 2023-04-18 21:02:41.000000 connpy-3.0.7/connpy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 21:02:41.000000 connpy-3.0.7/connpy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      126 2023-04-18 21:02:41.000000 connpy-3.0.7/connpy.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-04-18 21:02:41.000000 connpy-3.0.7/connpy.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-18 21:02:41.000000 connpy-3.0.7/connpy.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     1149 2023-04-18 21:02:41.227078 connpy-3.0.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-04-18 21:02:30.000000 connpy-3.0.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 16:42:49.592495 connpy-3.2.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1068 2023-05-05 16:42:37.000000 connpy-3.2.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     9276 2023-05-05 16:42:49.592495 connpy-3.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     8445 2023-05-05 16:42:37.000000 connpy-3.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 16:42:49.592495 connpy-3.2.0/connpy/
+-rw-r--r--   0 runner    (1001) docker     (123)     8379 2023-05-05 16:42:37.000000 connpy-3.2.0/connpy/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      181 2023-05-05 16:42:37.000000 connpy-3.2.0/connpy/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-05 16:42:37.000000 connpy-3.2.0/connpy/_version.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    14771 2023-05-05 16:42:37.000000 connpy-3.2.0/connpy/ai.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4713 2023-05-05 16:42:37.000000 connpy-3.2.0/connpy/api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3566 2023-05-05 16:42:37.000000 connpy-3.2.0/connpy/completion.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    15540 2023-05-05 16:42:37.000000 connpy-3.2.0/connpy/configfile.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    50300 2023-05-05 16:42:37.000000 connpy-3.2.0/connpy/connapp.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)    28719 2023-05-05 16:42:37.000000 connpy-3.2.0/connpy/core.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 16:42:49.592495 connpy-3.2.0/connpy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     9276 2023-05-05 16:42:49.000000 connpy-3.2.0/connpy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      377 2023-05-05 16:42:49.000000 connpy-3.2.0/connpy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 16:42:49.000000 connpy-3.2.0/connpy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-05-05 16:42:49.000000 connpy-3.2.0/connpy.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       89 2023-05-05 16:42:49.000000 connpy-3.2.0/connpy.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-05 16:42:49.000000 connpy-3.2.0/connpy.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     1167 2023-05-05 16:42:49.592495 connpy-3.2.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-05-05 16:42:37.000000 connpy-3.2.0/setup.py
```

### Comparing `connpy-3.0.7/LICENSE` & `connpy-3.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `connpy-3.0.7/PKG-INFO` & `connpy-3.2.0/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,29 +1,7 @@
-Metadata-Version: 2.1
-Name: connpy
-Version: 3.0.7
-Summary: Connpy is a SSH/Telnet connection manager and automation module
-Home-page: https://github.com/fluzzi/connpy
-Author: Federico Luzzi
-Author-email: fluzzi@gmail.com
-License: MIT License
-Project-URL: Bug Tracker, https://github.com/fluzzi/connpy/issues
-Project-URL: Documentation, https://fluzzi.github.io/connpy/
-Keywords: networking,automation,ssh,telnet,connection manager
-Classifier: Development Status :: 4 - Beta
-Classifier: Topic :: System :: Networking
-Classifier: Intended Audience :: Telecommunications Industry
-Classifier: Programming Language :: Python :: 3
-Classifier: Natural Language :: English
-Classifier: Operating System :: MacOS
-Classifier: Operating System :: Unix
-Description-Content-Type: text/markdown
-Provides-Extra: fuzzysearch
-License-File: LICENSE
-
 # Conn
 [![](https://img.shields.io/pypi/v/connpy.svg?style=flat-square)](https://pypi.org/pypi/connpy/)
 [![](https://img.shields.io/pypi/pyversions/connpy.svg?style=flat-square)](https://pypi.org/pypi/connpy/)
 [![](https://img.shields.io/pypi/l/connpy.svg?style=flat-square)](https://github.com/fluzzi/connpy/blob/main/LICENSE)
 [![](https://img.shields.io/pypi/dm/connpy.svg?style=flat-square)](https://pypi.org/pypi/connpy/)
 
 Connpy is a ssh and telnet connection manager and automation module
@@ -32,15 +10,15 @@
 
 pip install connpy
 
 ## Automation module usage
 ### Standalone module
 ```
 import connpy
-router = connpy.node("unique name","ip/hostname", user="username", password="password")
+router = connpy.node("uniqueName","ip/host", user="username", password="password")
 router.run(["term len 0","show run"])
 print(router.output)
 hasip = router.test("show ip int brief","1.1.1.1")
 if hasip:
     print("Router has ip 1.1.1.1")
 else:
     print("router does not have ip 1.1.1.1")
@@ -64,17 +42,17 @@
 #You can also get each node individually:
 nodes = {}
 nodes["router1"] = conf.getitem("router1@office")
 nodes["router2"] = conf.getitem("router2@office")
 nodes["router10"] = conf.getitem("router10@datacenter")
 #Also, you can create the nodes manually:
 nodes = {}
-nodes["router1"] = {"host": "1.1.1.1", "user": "username", "password": "password1"}
-nodes["router2"] = {"host": "1.1.1.2", "user": "username", "password": "password2"}
-nodes["router3"] = {"host": "1.1.1.2", "user": "username", "password": "password3"}
+nodes["router1"] = {"host": "1.1.1.1", "user": "user", "password": "password1"}
+nodes["router2"] = {"host": "1.1.1.2", "user": "user", "password": "password2"}
+nodes["router3"] = {"host": "1.1.1.2", "user": "user", "password": "password3"}
 #Finally you run some tasks on the nodes
 mynodes = connpy.nodes(nodes, config = conf)
 result = mynodes.test(["show ip int br"], "1.1.1.2")
 for i in result:
     print("---" + i + "---")
     print(result[i])
     print()
@@ -100,15 +78,25 @@
 expected = "!"
 routers = connpy.nodes(nodes, config = config)
 routers.run(commands, variables)
 routers.test("ping {ip}", expected, variables)
 for key in routers.result:
     print(key, ' ---> ', ("pass" if routers.result[key] else "fail"))
 ```
-
+### Using AI
+```
+import connpy
+conf = connpy.configfile()
+organization = 'openai-org'
+api_key = "openai-key"
+myia = ai(conf, organization, api_key)
+input = "go to router 1 and get me the full configuration"
+result = myia.ask(input, dryrun = False)
+print(result)
+```
 ## Connection manager 
 ### Features
     - You can generate profiles and reference them from nodes using @profilename so you dont
       need to edit multiple nodes when changing password or other information.
     - Nodes can be stored on @folder or @subfolder@folder to organize your devices. Then can 
       be referenced using node@subfolder@folder or node@folder
     - If you have too many nodes. Get completion script using: conn config --completion.
@@ -200,15 +188,39 @@
 
 #### Response:
 
 - A JSON array containing the filtered list of nodes.
 
 ---
 
-### 2. Run Commands
+### 2. Get Nodes
+
+**Endpoint**: `/get_nodes`
+
+**Method**: `POST`
+
+**Description**: This route returns a dictionary of nodes with all their attributes. It can also filter the nodes based on a given keyword.
+
+#### Request Body:
+
+```json
+{
+  "filter": "<keyword>"
+}
+```
+
+* `filter` (optional): A keyword to filter the nodes. It returns only the nodes that contain the keyword. If not provided, the route will return the entire list of nodes.
+
+#### Response:
+
+- A JSON array containing the filtered nodes.
+
+---
+
+### 3. Run Commands
 
 **Endpoint**: `/run_commands`
 
 **Method**: `POST`
 
 **Description**: This route runs commands on selected nodes based on the provided action, nodes, and commands. It also supports executing tests by providing expected results.
 
@@ -229,7 +241,33 @@
 * `commands` (required): A list of commands to be executed on the specified nodes.
 * `expected` (optional, only used when the action is `test`): A single expected result for the test.
 * `options` (optional): Array to pass options to the run command, options are: `prompt`, `parallel`, `timeout`  
 
 #### Response:
 
 - A JSON object with the results of the executed commands on the nodes.
+
+### 4. Ask AI
+
+**Endpoint**: `/ask_ai`
+
+**Method**: `POST`
+
+**Description**: This route sends to chatgpt IA a request that will parse it into an understandable output for the application and then run the request.
+
+#### Request Body:
+
+```json
+{
+  "input": "<user input request>",
+  "dryrun": true or false
+}
+```
+
+* `input` (required): The user input requesting the AI to perform an action on some devices or get the devices list.
+* `dryrun` (optional): If set to true, it will return the parameters to run the request but it won't run it. default is false.
+
+#### Response:
+
+- A JSON array containing the action to run and the parameters and the result of the action.
+
+
```

### Comparing `connpy-3.0.7/README.md` & `connpy-3.2.0/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,7 +1,29 @@
+Metadata-Version: 2.1
+Name: connpy
+Version: 3.2.0
+Summary: Connpy is a SSH/Telnet connection manager and automation module
+Home-page: https://github.com/fluzzi/connpy
+Author: Federico Luzzi
+Author-email: fluzzi@gmail.com
+License: MIT License
+Project-URL: Bug Tracker, https://github.com/fluzzi/connpy/issues
+Project-URL: Documentation, https://fluzzi.github.io/connpy/
+Keywords: networking,automation,ssh,telnet,connection manager
+Classifier: Development Status :: 4 - Beta
+Classifier: Topic :: System :: Networking
+Classifier: Intended Audience :: Telecommunications Industry
+Classifier: Programming Language :: Python :: 3
+Classifier: Natural Language :: English
+Classifier: Operating System :: MacOS
+Classifier: Operating System :: Unix
+Description-Content-Type: text/markdown
+Provides-Extra: fuzzysearch
+License-File: LICENSE
+
 # Conn
 [![](https://img.shields.io/pypi/v/connpy.svg?style=flat-square)](https://pypi.org/pypi/connpy/)
 [![](https://img.shields.io/pypi/pyversions/connpy.svg?style=flat-square)](https://pypi.org/pypi/connpy/)
 [![](https://img.shields.io/pypi/l/connpy.svg?style=flat-square)](https://github.com/fluzzi/connpy/blob/main/LICENSE)
 [![](https://img.shields.io/pypi/dm/connpy.svg?style=flat-square)](https://pypi.org/pypi/connpy/)
 
 Connpy is a ssh and telnet connection manager and automation module
@@ -10,15 +32,15 @@
 
 pip install connpy
 
 ## Automation module usage
 ### Standalone module
 ```
 import connpy
-router = connpy.node("unique name","ip/hostname", user="username", password="password")
+router = connpy.node("uniqueName","ip/host", user="username", password="password")
 router.run(["term len 0","show run"])
 print(router.output)
 hasip = router.test("show ip int brief","1.1.1.1")
 if hasip:
     print("Router has ip 1.1.1.1")
 else:
     print("router does not have ip 1.1.1.1")
@@ -42,17 +64,17 @@
 #You can also get each node individually:
 nodes = {}
 nodes["router1"] = conf.getitem("router1@office")
 nodes["router2"] = conf.getitem("router2@office")
 nodes["router10"] = conf.getitem("router10@datacenter")
 #Also, you can create the nodes manually:
 nodes = {}
-nodes["router1"] = {"host": "1.1.1.1", "user": "username", "password": "password1"}
-nodes["router2"] = {"host": "1.1.1.2", "user": "username", "password": "password2"}
-nodes["router3"] = {"host": "1.1.1.2", "user": "username", "password": "password3"}
+nodes["router1"] = {"host": "1.1.1.1", "user": "user", "password": "password1"}
+nodes["router2"] = {"host": "1.1.1.2", "user": "user", "password": "password2"}
+nodes["router3"] = {"host": "1.1.1.2", "user": "user", "password": "password3"}
 #Finally you run some tasks on the nodes
 mynodes = connpy.nodes(nodes, config = conf)
 result = mynodes.test(["show ip int br"], "1.1.1.2")
 for i in result:
     print("---" + i + "---")
     print(result[i])
     print()
@@ -78,15 +100,25 @@
 expected = "!"
 routers = connpy.nodes(nodes, config = config)
 routers.run(commands, variables)
 routers.test("ping {ip}", expected, variables)
 for key in routers.result:
     print(key, ' ---> ', ("pass" if routers.result[key] else "fail"))
 ```
-
+### Using AI
+```
+import connpy
+conf = connpy.configfile()
+organization = 'openai-org'
+api_key = "openai-key"
+myia = ai(conf, organization, api_key)
+input = "go to router 1 and get me the full configuration"
+result = myia.ask(input, dryrun = False)
+print(result)
+```
 ## Connection manager 
 ### Features
     - You can generate profiles and reference them from nodes using @profilename so you dont
       need to edit multiple nodes when changing password or other information.
     - Nodes can be stored on @folder or @subfolder@folder to organize your devices. Then can 
       be referenced using node@subfolder@folder or node@folder
     - If you have too many nodes. Get completion script using: conn config --completion.
@@ -178,15 +210,39 @@
 
 #### Response:
 
 - A JSON array containing the filtered list of nodes.
 
 ---
 
-### 2. Run Commands
+### 2. Get Nodes
+
+**Endpoint**: `/get_nodes`
+
+**Method**: `POST`
+
+**Description**: This route returns a dictionary of nodes with all their attributes. It can also filter the nodes based on a given keyword.
+
+#### Request Body:
+
+```json
+{
+  "filter": "<keyword>"
+}
+```
+
+* `filter` (optional): A keyword to filter the nodes. It returns only the nodes that contain the keyword. If not provided, the route will return the entire list of nodes.
+
+#### Response:
+
+- A JSON array containing the filtered nodes.
+
+---
+
+### 3. Run Commands
 
 **Endpoint**: `/run_commands`
 
 **Method**: `POST`
 
 **Description**: This route runs commands on selected nodes based on the provided action, nodes, and commands. It also supports executing tests by providing expected results.
 
@@ -207,7 +263,33 @@
 * `commands` (required): A list of commands to be executed on the specified nodes.
 * `expected` (optional, only used when the action is `test`): A single expected result for the test.
 * `options` (optional): Array to pass options to the run command, options are: `prompt`, `parallel`, `timeout`  
 
 #### Response:
 
 - A JSON object with the results of the executed commands on the nodes.
+
+### 4. Ask AI
+
+**Endpoint**: `/ask_ai`
+
+**Method**: `POST`
+
+**Description**: This route sends to chatgpt IA a request that will parse it into an understandable output for the application and then run the request.
+
+#### Request Body:
+
+```json
+{
+  "input": "<user input request>",
+  "dryrun": true or false
+}
+```
+
+* `input` (required): The user input requesting the AI to perform an action on some devices or get the devices list.
+* `dryrun` (optional): If set to true, it will return the parameters to run the request but it won't run it. default is false.
+
+#### Response:
+
+- A JSON array containing the action to run and the parameters and the result of the action.
+
+
```

### Comparing `connpy-3.0.7/connpy/__init__.py` & `connpy-3.2.0/connpy/__init__.py`

 * *Files 23% similar despite different names*

```diff
@@ -94,15 +94,39 @@
 
 #### Response:
 
 - A JSON array containing the filtered list of nodes.
 
 ---
 
-### 2. Run Commands
+### 2. Get Nodes
+
+**Endpoint**: `/get_nodes`
+
+**Method**: `POST`
+
+**Description**: This route returns a dictionary of nodes with all their attributes. It can also filter the nodes based on a given keyword.
+
+#### Request Body:
+
+```json
+{
+  "filter": "<keyword>"
+}
+```
+
+* `filter` (optional): A keyword to filter the nodes. It returns only the nodes that contain the keyword. If not provided, the route will return the entire list of nodes.
+
+#### Response:
+
+- A JSON array containing the filtered nodes.
+
+---
+
+### 3. Run Commands
 
 **Endpoint**: `/run_commands`
 
 **Method**: `POST`
 
 **Description**: This route runs commands on selected nodes based on the provided action, nodes, and commands. It also supports executing tests by providing expected results.
 
@@ -123,21 +147,45 @@
 * `commands` (required): A list of commands to be executed on the specified nodes.
 * `expected` (optional, only used when the action is `test`): A single expected result for the test.
 * `options` (optional): Array to pass options to the run command, options are: `prompt`, `parallel`, `timeout`  
 
 #### Response:
 
 - A JSON object with the results of the executed commands on the nodes.
-## Automation module
-the automation module
 
+### 4. Ask AI
+
+**Endpoint**: `/ask_ai`
+
+**Method**: `POST`
+
+**Description**: This route sends to chatgpt IA a request that will parse it into an understandable output for the application and then run the request.
+
+#### Request Body:
+
+```json
+{
+  "input": "<user input request>",
+  "dryrun": true or false
+}
+```
+
+* `input` (required): The user input requesting the AI to perform an action on some devices or get the devices list.
+* `dryrun` (optional): If set to true, it will return the parameters to run the request but it won't run it. default is false.
+
+#### Response:
+
+- A JSON array containing the action to run and the parameters and the result of the action.
+
+## Automation module
+The automation module
 ### Standalone module
 ```
 import connpy
-router = connpy.node("unique name","ip/hostname", user="user", password="pass")
+router = connpy.node("uniqueName","ip/host", user="user", password="pass")
 router.run(["term len 0","show run"])
 print(router.output)
 hasip = router.test("show ip int brief","1.1.1.1")
 if hasip:
     print("Router has ip 1.1.1.1")
 else:
     print("router does not have ip 1.1.1.1")
@@ -161,17 +209,17 @@
 #You can also get each node individually:
 nodes = {}
 nodes["router1"] = conf.getitem("router1@office")
 nodes["router2"] = conf.getitem("router2@office")
 nodes["router10"] = conf.getitem("router10@datacenter")
 #Also, you can create the nodes manually:
 nodes = {}
-nodes["router1"] = {"host": "1.1.1.1", "user": "username", "password": "pass1"}
-nodes["router2"] = {"host": "1.1.1.2", "user": "username", "password": "pass2"}
-nodes["router3"] = {"host": "1.1.1.2", "user": "username", "password": "pass3"}
+nodes["router1"] = {"host": "1.1.1.1", "user": "user", "password": "pass1"}
+nodes["router2"] = {"host": "1.1.1.2", "user": "user", "password": "pass2"}
+nodes["router3"] = {"host": "1.1.1.2", "user": "user", "password": "pass3"}
 #Finally you run some tasks on the nodes
 mynodes = connpy.nodes(nodes, config = conf)
 result = mynodes.test(["show ip int br"], "1.1.1.2")
 for i in result:
     print("---" + i + "---")
     print(result[i])
     print()
@@ -197,21 +245,34 @@
 expected = "!"
 routers = connpy.nodes(nodes, config = config)
 routers.run(commands, variables)
 routers.test("ping {ip}", expected, variables)
 for key in routers.result:
     print(key, ' ---> ', ("pass" if routers.result[key] else "fail"))
 ```
+### Using AI
+```
+import connpy
+conf = connpy.configfile()
+organization = 'openai-org'
+api_key = "openai-key"
+myia = ai(conf, organization, api_key)
+input = "go to router 1 and get me the full configuration"
+result = myia.ask(input, dryrun = False)
+print(result)
+```
 '''
 from .core import node,nodes
 from .configfile import configfile
 from .connapp import connapp
+from .api import *
+from .ai import ai
 from ._version import __version__
 from pkg_resources import get_distribution
 
-__all__ = ["node", "nodes", "configfile", "connapp"]
+__all__ = ["node", "nodes", "configfile", "connapp", "ai"]
 __author__ = "Federico Luzzi"
 __pdoc__ = {
     'core': False,
     'completion': False,
     'api': False
 }
```

### Comparing `connpy-3.0.7/connpy/api.py` & `connpy-3.2.0/connpy/api.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 from flask import Flask, request, jsonify
 from connpy import configfile, node, nodes
+from connpy.ai import ai as myai
 from waitress import serve
 import os
 import signal
 
 app = Flask(__name__)
 conf = configfile()
 
@@ -18,26 +19,58 @@
         'version': '1.0',
         'documentation': 'https://fluzzi.github.io/connpy/'
     })
 
 @app.route("/list_nodes", methods=["POST"])
 def list_nodes():
     conf = app.custom_config
-    output = conf._getallnodes()
     case = conf.config["case"]
     try:
         data = request.get_json()
         filter = data["filter"]
         if not case:
-            filter = filter.lower()
-        output = [item for item in output if filter in item]
+            if isinstance(filter, list):
+                filter = [item.lower() for item in filter]
+            else:
+                filter = filter.lower()
+        output = conf._getallnodes(filter)
     except:
-        pass
+        output = conf._getallnodes()
     return jsonify(output)
 
+@app.route("/get_nodes", methods=["POST"])
+def get_nodes():
+    conf = app.custom_config
+    case = conf.config["case"]
+    try:
+        data = request.get_json()
+        filter = data["filter"]
+        if not case:
+            if isinstance(filter, list):
+                filter = [item.lower() for item in filter]
+            else:
+                filter = filter.lower()
+        output = conf._getallnodesfull(filter)
+    except:
+        output = conf._getallnodesfull()
+    return jsonify(output)
+
+@app.route("/ask_ai", methods=["POST"])
+def ask_ai():
+    conf = app.custom_config
+    data = request.get_json()
+    input = data["input"]
+    if "dryrun" in data:
+        dryrun = data["dryrun"] 
+    else:
+        dryrun = False
+    ai = myai(conf)
+    return ai.ask(input, dryrun)
+
+
 @app.route("/run_commands", methods=["POST"])
 def run_commands():
     conf = app.custom_config
     data = request.get_json()
     case = conf.config["case"]
     mynodes = {}
     args = {}
@@ -47,33 +80,15 @@
         args["commands"] = data["commands"]
         if action == "test":
             args["expected"] = data["expected"]
     except KeyError as e:
         error = "'{}' is mandatory".format(e.args[0])
         return({"DataError": error})
     if isinstance(nodelist, list):
-        for i in nodelist:
-            if isinstance(i, dict):
-                name = list(i.keys())[0]
-                mylist = i[name]
-                if not case:
-                    name = name.lower()
-                    mylist = [item.lower() for item in mylist]
-                this = conf.getitem(name, mylist)
-                mynodes.update(this)
-            elif i.startswith("@"):
-                if not case:
-                    i = i.lower()
-                this = conf.getitem(i)
-                mynodes.update(this)
-            else:
-                if not case:
-                    i = i.lower()
-                this = conf.getitem(i)
-                mynodes[i] = this
+        mynodes = conf.getitems(nodelist)
     else:
         if not case:
             nodelist = nodelist.lower()
         if nodelist.startswith("@"):
             mynodes = conf.getitem(nodelist)
         else:
             mynodes[nodelist] = conf.getitem(nodelist)
```

### Comparing `connpy-3.0.7/connpy/completion.py` & `connpy-3.2.0/connpy/completion.py`

 * *Files identical despite different names*

### Comparing `connpy-3.0.7/connpy/configfile.py` & `connpy-3.2.0/connpy/configfile.py`

 * *Files 15% similar despite different names*

```diff
@@ -88,15 +88,15 @@
         jsonconf = open(conf)
         jsondata = json.load(jsonconf)
         jsonconf.close()
         return jsondata
 
     def _createconfig(self, conf):
         #Create config file
-        defaultconfig = {'config': {'case': False, 'idletime': 30, 'fzf': False}, 'connections': {}, 'profiles': { "default": { "host":"", "protocol":"ssh", "port":"", "user":"", "password":"", "options":"", "logs":"" }}}
+        defaultconfig = {'config': {'case': False, 'idletime': 30, 'fzf': False}, 'connections': {}, 'profiles': { "default": { "host":"", "protocol":"ssh", "port":"", "user":"", "password":"", "options":"", "logs":"", "tags": "" }}}
         if not os.path.exists(conf):
             with open(conf, "w") as f:
                 json.dump(defaultconfig, f, indent = 4)
                 f.close()
                 os.chmod(conf, 0o600)
         jsonconf = open(conf)
         jsondata = json.load(jsonconf)
@@ -155,16 +155,16 @@
         ### Optional Parameters:  
 
             - keys (list): In case you pass a folder as unique, you can filter
                            nodes inside the folder passing a list.
 
         ### Returns:  
 
-            dict: Dictionary containing information of node or multiple dictionaries
-                  of multiple nodes.
+            dict: Dictionary containing information of node or multiple 
+                  dictionaries of multiple nodes.
 
         '''
         uniques = self._explode_unique(unique)
         if unique.startswith("@"):
             if uniques.keys() >= {"folder", "subfolder"}:
                 folder = self.connections[uniques["folder"]][uniques["subfolder"]]
             else:
@@ -193,22 +193,61 @@
                 node = self.connections[uniques["folder"]][uniques["id"]]
             else:
                 node = self.connections[uniques["id"]]
             newnode = deepcopy(node)
             newnode.pop("type")
             return newnode
 
-    def _connections_add(self,*, id, host, folder='', subfolder='', options='', logs='', password='', port='', protocol='', user='', type = "connection" ):
+    def getitems(self, uniques):
+        '''
+        Get a group of nodes from configfile which can be passed to node/nodes class
+
+        ### Parameters:  
+
+            - uniques (str/list): Regex string name that will match hostnames 
+                                  from the connection manager. It can be a 
+                                  list of strings.
+
+        ### Returns:  
+
+            dict: Dictionary containing information of node or multiple 
+                  dictionaries of multiple nodes.
+
+        '''
+        nodes = {}
+        for i in uniques:
+            if isinstance(i, dict):
+                name = list(i.keys())[0]
+                mylist = i[name]
+                if not self.config["case"]:
+                    name = name.lower()
+                    mylist = [item.lower() for item in mylist]
+                this = self.getitem(name, mylist)
+                nodes.update(this)
+            elif i.startswith("@"):
+                if not self.config["case"]:
+                    i = i.lower()
+                this = self.getitem(i)
+                nodes.update(this)
+            else:
+                if not self.config["case"]:
+                    i = i.lower()
+                this = self.getitem(i)
+                nodes[i] = this
+        return nodes
+
+
+    def _connections_add(self,*, id, host, folder='', subfolder='', options='', logs='', password='', port='', protocol='', user='', tags='', type = "connection" ):
         #Add connection from config
         if folder == '':
-            self.connections[id] = {"host": host, "options": options, "logs": logs, "password": password, "port": port, "protocol": protocol, "user": user, "type": type}
+            self.connections[id] = {"host": host, "options": options, "logs": logs, "password": password, "port": port, "protocol": protocol, "user": user, "tags": tags,"type": type}
         elif folder != '' and subfolder == '':
-            self.connections[folder][id] = {"host": host, "options": options, "logs": logs, "password": password, "port": port, "protocol": protocol, "user": user, "type": type}
+            self.connections[folder][id] = {"host": host, "options": options, "logs": logs, "password": password, "port": port, "protocol": protocol, "user": user, "tags": tags, "type": type}
         elif folder != '' and subfolder != '':
-            self.connections[folder][subfolder][id] = {"host": host, "options": options, "logs": logs, "password": password, "port": port, "protocol": protocol, "user": user, "type": type}
+            self.connections[folder][subfolder][id] = {"host": host, "options": options, "logs": logs, "password": password, "port": port, "protocol": protocol, "user": user, "tags": tags, "type": type}
             
 
     def _connections_del(self,*, id, folder='', subfolder=''):
         #Delete connection from config
         if folder == '':
             del self.connections[id]
         elif folder != '' and subfolder == '':
@@ -229,38 +268,81 @@
         #Delete folder from config
         if subfolder == '':
             del self.connections[folder]
         else:
             del self.connections[folder][subfolder]
 
 
-    def _profiles_add(self,*, id, host = '', options='', logs='', password='', port='', protocol='', user='' ):
+    def _profiles_add(self,*, id, host = '', options='', logs='', password='', port='', protocol='', user='', tags='' ):
         #Add profile from config
-        self.profiles[id] = {"host": host, "options": options, "logs": logs, "password": password, "port": port, "protocol": protocol, "user": user}
+        self.profiles[id] = {"host": host, "options": options, "logs": logs, "password": password, "port": port, "protocol": protocol, "user": user, "tags": tags}
             
 
     def _profiles_del(self,*, id ):
         #Delete profile from config
         del self.profiles[id]
         
-    def _getallnodes(self):
+    def _getallnodes(self, filter = None):
         #get all nodes on configfile
         nodes = []
         layer1 = [k for k,v in self.connections.items() if isinstance(v, dict) and v["type"] == "connection"]
         folders = [k for k,v in self.connections.items() if isinstance(v, dict) and v["type"] == "folder"]
         nodes.extend(layer1)
         for f in folders:
             layer2 = [k + "@" + f for k,v in self.connections[f].items() if isinstance(v, dict) and v["type"] == "connection"]
             nodes.extend(layer2)
             subfolders = [k for k,v in self.connections[f].items() if isinstance(v, dict) and v["type"] == "subfolder"]
             for s in subfolders:
                 layer3 = [k + "@" + s + "@" + f for k,v in self.connections[f][s].items() if isinstance(v, dict) and v["type"] == "connection"]
                 nodes.extend(layer3)
+        if filter:
+            if isinstance(filter, str):
+                nodes = [item for item in nodes if re.search(filter, item)]
+            elif isinstance(filter, list):
+                nodes = [item for item in nodes if any(re.search(pattern, item) for pattern in filter)]
+            else:
+                raise ValueError("filter must be a string or a list of strings")
         return nodes
 
+    def _getallnodesfull(self, filter = None):
+        #get all nodes on configfile with all their attributes.
+        nodes = {}
+        layer1 = {k:v for k,v in self.connections.items() if isinstance(v, dict) and v["type"] == "connection"}
+        folders = [k for k,v in self.connections.items() if isinstance(v, dict) and v["type"] == "folder"]
+        nodes.update(layer1)
+        for f in folders:
+            layer2 = {k + "@" + f:v for k,v in self.connections[f].items() if isinstance(v, dict) and v["type"] == "connection"}
+            nodes.update(layer2)
+            subfolders = [k for k,v in self.connections[f].items() if isinstance(v, dict) and v["type"] == "subfolder"]
+            for s in subfolders:
+                layer3 = {k + "@" + s + "@" + f:v for k,v in self.connections[f][s].items() if isinstance(v, dict) and v["type"] == "connection"}
+                nodes.update(layer3)
+        if filter:
+            if isinstance(filter, str):
+                nodes = {k: v for k, v in nodes.items() if re.search(filter, k)}
+            elif isinstance(filter, list):
+                nodes = {k: v for k, v in nodes.items() if any(re.search(pattern, k) for pattern in filter)}
+            else:
+                raise ValueError("filter must be a string or a list of strings")
+        for node, keys in nodes.items():
+            for key, value in keys.items():
+                profile = re.search("^@(.*)", str(value))
+                if profile:
+                    try:
+                        nodes[node][key] = self.profiles[profile.group(1)][key]
+                    except:
+                        nodes[node][key] = ""
+                elif value == '' and key == "protocol":
+                    try:
+                        nodes[node][key] = config.profiles["default"][key]
+                    except:
+                        nodes[node][key] = "ssh"
+        return nodes
+
+
     def _getallfolders(self):
         #get all folders on configfile
         folders = ["@" + k for k,v in self.connections.items() if isinstance(v, dict) and v["type"] == "folder"]
         subfolders = []
         for f in folders:
             s = ["@" + k + f for k,v in self.connections[f[1:]].items() if isinstance(v, dict) and v["type"] == "subfolder"]
             subfolders.extend(s)
```

### Comparing `connpy-3.0.7/connpy/connapp.py` & `connpy-3.2.0/connpy/connapp.py`

 * *Files 2% similar despite different names*

```diff
@@ -6,16 +6,17 @@
 from Crypto.Cipher import PKCS1_OAEP
 import ast
 import argparse
 import sys
 import inquirer
 from .core import node,nodes
 from ._version import __version__
-from .api import *
+from .api import start_api,stop_api,debug_api
 import yaml
+import ast
 try:
     from pyfzf.pyfzf import FzfPrompt
 except:
     FzfPrompt = None
 home = os.path.expanduser("~")
 defaultdir = home + '/.config/conn'
 
@@ -115,14 +116,15 @@
         configparser = subparsers.add_parser("config", help="Manage app config") 
         configcrud = configparser.add_mutually_exclusive_group(required=True)
         configcrud.add_argument("--allow-uppercase", dest="case", nargs=1, action=self._store_type, help="Allow case sensitive names", choices=["true","false"])
         configcrud.add_argument("--fzf", dest="fzf", nargs=1, action=self._store_type, help="Use fzf for lists", choices=["true","false"])
         configcrud.add_argument("--keepalive", dest="idletime", nargs=1, action=self._store_type, help="Set keepalive time in seconds, 0 to disable", type=int, metavar="INT")
         configcrud.add_argument("--completion", dest="completion", nargs=1, choices=["bash","zsh"], action=self._store_type, help="Get terminal completion configuration for conn")
         configcrud.add_argument("--configfolder", dest="configfolder", nargs=1, action=self._store_type, help="Set the default location for config file", metavar="FOLDER")
+        configcrud.add_argument("--openai", dest="openai", nargs=2, action=self._store_type, help="Set openai organization and api_key", metavar=("ORGANIZATION", "API_KEY"))
         configparser.set_defaults(func=self._func_others)
         #Manage sys arguments
         commands = ["node", "profile", "mv", "move","copy", "cp", "bulk", "ls", "list", "run", "config", "api"]
         profilecmds = ["--add", "-a", "--del", "--rm",  "-r", "--mod", "--edit", "-e", "--show", "-s"]
         if len(argv) >= 2 and argv[1] == "profile" and argv[0] in profilecmds:
             argv[1] = argv[0]
             argv[0] = "profile"
@@ -240,14 +242,15 @@
                 if uniques == False:
                     print("Invalid node {}".format(args.data))
                     exit(5)
                 print("You can use the configured setting in a profile using @profilename.")
                 print("You can also leave empty any value except hostname/IP.")
                 print("You can pass 1 or more passwords using comma separated @profiles")
                 print("You can use this variables on logging file name: ${id} ${unique} ${host} ${port} ${user} ${protocol}")
+                print("Some useful tags to set for automation are 'os', 'screen_length_command', and 'prompt'.")
                 newnode = self._questions_nodes(args.data, uniques)
                 if newnode == False:
                     exit(7)
                 self.config._connections_add(**newnode)
                 self.config._saveconfig(self.config.file)
                 print("{} added succesfully".format(args.data))
 
@@ -368,15 +371,15 @@
         else:
             self.config._profiles_add(**updateprofile)
             self.config._saveconfig(self.config.file)
             print("{} edited succesfully".format(args.data[0]))
     
     def _func_others(self, args):
         #Function called when using other commands
-        actions = {"ls": self._ls, "move": self._mvcp, "cp": self._mvcp, "bulk": self._bulk, "completion": self._completion, "case": self._case, "fzf": self._fzf, "idletime": self._idletime, "configfolder": self._configfolder}
+        actions = {"ls": self._ls, "move": self._mvcp, "cp": self._mvcp, "bulk": self._bulk, "completion": self._completion, "case": self._case, "fzf": self._fzf, "idletime": self._idletime, "configfolder": self._configfolder, "openai": self._openai}
         return actions.get(args.command)(args)
 
     def _ls(self, args):
         print(*getattr(self, args.data), sep="\n")
 
     def _mvcp(self, args):
         if not self.case:
@@ -438,14 +441,15 @@
                 newnode["host"] = hosts[index]
             else:
                 newnode["host"] = hosts[0]
             newnode["protocol"] = newnodes["protocol"]
             newnode["port"] = newnodes["port"]
             newnode["options"] = newnodes["options"]
             newnode["logs"] = newnodes["logs"]
+            newnode["tags"] = newnodes["tags"]
             newnode["user"] = newnodes["user"]
             newnode["password"] = newnodes["password"]
             count +=1
             self.config._connections_add(**newnode)
             self.nodes = self.config._getallnodes()
         if count > 0:
             self.config._saveconfig(self.config.file)
@@ -483,14 +487,21 @@
             raise argparse.ArgumentTypeError(f"readable_dir:{args.data[0]} is not a valid path")
         else:
             pathfile = defaultdir + "/.folder"
             folder = os.path.abspath(args.data[0]).rstrip('/')
             with open(pathfile, "w") as f:
                 f.write(str(folder))
             print("Config saved")
+        
+    def _openai(self, args):
+        openaikeys = {}
+        openaikeys["organization"] = args.data[0]
+        openaikeys["api_key"] = args.data[1]
+        self._change_settings(args.command, openaikeys)
+
 
     def _change_settings(self, name, value):
         self.config.config[name] = value
         self.config._saveconfig(self.config.file)
         print("Config saved")
 
     def _func_run(self, args):
@@ -512,15 +523,14 @@
                 debug_api(args.data)
             else:
                 debug_api()
         return
 
     def _node_run(self, args):
         command = " ".join(args.data[1:])
-        command = command.split("-")
         matches = list(filter(lambda k: k == args.data[0], self.nodes))
         if len(matches) == 0:
             print("{} not found".format(args.data[0]))
             exit(2)
         node = self.config.getitem(matches[0])
         node = self.node(matches[0],**node, config = self.config)
         node.run(command)
@@ -541,38 +551,26 @@
         try:
             with open(args.data[0]) as file:
                 scripts = yaml.load(file, Loader=yaml.FullLoader)
         except:
             print("failed reading file {}".format(args.data[0]))
             exit(10)
         for script in scripts["tasks"]:
-            nodes = {}
             args = {}
             try:
                 action = script["action"]
                 nodelist = script["nodes"]
                 args["commands"] = script["commands"]
                 output = script["output"]
                 if action == "test":
                     args["expected"] = script["expected"]
             except KeyError as e:
                 print("'{}' is mandatory".format(e.args[0]))
                 exit(11)
-            for i in nodelist:
-                if isinstance(i, dict):
-                    name = list(i.keys())[0]
-                    this = self.config.getitem(name, i[name])
-                    nodes.update(this)
-                elif i.startswith("@"):
-                    this = self.config.getitem(i)
-                    nodes.update(this)
-                else:
-                    this = self.config.getitem(i)
-                    nodes[i] = this
-            nodes = self.connnodes(nodes, config = self.config)
+            nodes = self.connnodes(self.config.getitems(nodelist), config = self.config)
             stdout = False
             if output is None:
                 pass
             elif output == "stdout":
                 stdout = True
             elif isinstance(output, str) and action == "run":
                 args["folder"] = output
@@ -694,14 +692,41 @@
         #Validate password in inquirer
         profiles = current.split(",")
         for i in profiles:
             if not re.match(regex, i) or i[1:] not in self.profiles:
                 raise inquirer.errors.ValidationError("", reason="Profile {} don't exist".format(i))
         return True
 
+    def _tags_validation(self, answers, current):
+        #Validation for Tags in inquirer when managing nodes
+        if current.startswith("@"):
+            if current[1:] not in self.profiles:
+                raise inquirer.errors.ValidationError("", reason="Profile {} don't exist".format(current))
+        elif current != "":
+            isdict = False
+            try:
+                isdict = ast.literal_eval(current)
+            except:
+                pass
+            if not isinstance (isdict, dict):
+                raise inquirer.errors.ValidationError("", reason="Tags should be a python dictionary.".format(current))
+        return True
+
+    def _profile_tags_validation(self, answers, current):
+        #Validation for Tags in inquirer when managing profiles
+        if current != "":
+            isdict = False
+            try:
+                isdict = ast.literal_eval(current)
+            except:
+                pass
+            if not isinstance (isdict, dict):
+                raise inquirer.errors.ValidationError("", reason="Tags should be a python dictionary.".format(current))
+        return True
+
     def _default_validation(self, answers, current):
         #Default validation type used in multiples questions in inquirer
         if current.startswith("@"):
             if current[1:] not in self.profiles:
                 raise inquirer.errors.ValidationError("", reason="Profile {} don't exist".format(current))
         return True
 
@@ -740,29 +765,31 @@
         #Inquirer questions when editing nodes or profiles
         questions = []
         questions.append(inquirer.Confirm("host", message="Edit Hostname/IP?"))
         questions.append(inquirer.Confirm("protocol", message="Edit Protocol?"))
         questions.append(inquirer.Confirm("port", message="Edit Port?"))
         questions.append(inquirer.Confirm("options", message="Edit Options?"))
         questions.append(inquirer.Confirm("logs", message="Edit logging path/file?"))
+        questions.append(inquirer.Confirm("tags", message="Edit tags?"))
         questions.append(inquirer.Confirm("user", message="Edit User?"))
         questions.append(inquirer.Confirm("password", message="Edit password?"))
         answers = inquirer.prompt(questions)
         return answers
 
     def _questions_nodes(self, unique, uniques = None, edit = None):
         #Questions when adding or editing nodes
         try:
             defaults = self.config.getitem(unique)
+            if "tags" not in defaults:
+                defaults["tags"] = ""
         except:
-            defaults = { "host":"", "protocol":"", "port":"", "user":"", "options":"", "logs":"" }
+            defaults = { "host":"", "protocol":"", "port":"", "user":"", "options":"", "logs":"" , "tags":""}
         node = {}
-
         if edit == None:
-            edit = { "host":True, "protocol":True, "port":True, "user":True, "password": True,"options":True, "logs":True }
+            edit = { "host":True, "protocol":True, "port":True, "user":True, "password": True,"options":True, "logs":True, "tags":True }
         questions = []
         if edit["host"]:
             questions.append(inquirer.Text("host", message="Add Hostname or IP", validate=self._host_validation, default=defaults["host"]))
         else:
             node["host"] = defaults["host"]
         if edit["protocol"]:
             questions.append(inquirer.Text("protocol", message="Select Protocol", validate=self._protocol_validation, default=defaults["protocol"]))
@@ -776,14 +803,18 @@
             questions.append(inquirer.Text("options", message="Pass extra options to protocol", validate=self._default_validation, default=defaults["options"]))
         else:
             node["options"] = defaults["options"]
         if edit["logs"]:
             questions.append(inquirer.Text("logs", message="Pick logging path/file ",  validate=self._default_validation, default=defaults["logs"].replace("{","{{").replace("}","}}")))
         else:
             node["logs"] = defaults["logs"]
+        if edit["tags"]:
+            questions.append(inquirer.Text("tags", message="Add tags dictionary",  validate=self._tags_validation, default=str(defaults["tags"]).replace("{","{{").replace("}","}}")))
+        else:
+            node["tags"] = defaults["tags"]
         if edit["user"]:
             questions.append(inquirer.Text("user", message="Pick username", validate=self._default_validation, default=defaults["user"]))
         else:
             node["user"] = defaults["user"]
         if edit["password"]:
             questions.append(inquirer.List("password", message="Password: Use a local password, no password or a list of profiles to reference?", choices=["Local Password", "Profiles", "No Password"]))
         else:
@@ -802,27 +833,31 @@
                 passq = [(inquirer.Text("password", message="Set a @profile or a comma separated list of @profiles", validate=self._pass_validation))]
                 passa = inquirer.prompt(passq)
                 if passa == None:
                     return False
                 answer["password"] = passa["password"].split(",")
             elif answer["password"] == "No Password":
                 answer["password"] = ""
+        if "tags" in answer.keys() and not answer["tags"].startswith("@") and answer["tags"]:
+            answer["tags"] = ast.literal_eval(answer["tags"])
         result = {**uniques, **answer, **node}
         result["type"] = "connection"
         return result
 
     def _questions_profiles(self, unique, edit = None):
         #Questions when adding or editing profiles
         try:
             defaults = self.config.profiles[unique]
+            if "tags" not in defaults:
+                defaults["tags"] = ""
         except:
-            defaults = { "host":"", "protocol":"", "port":"", "user":"", "options":"", "logs":"" }
+            defaults = { "host":"", "protocol":"", "port":"", "user":"", "options":"", "logs":"", "tags": "" }
         profile = {}
         if edit == None:
-            edit = { "host":True, "protocol":True, "port":True, "user":True, "password": True,"options":True, "logs":True }
+            edit = { "host":True, "protocol":True, "port":True, "user":True, "password": True,"options":True, "logs":True, "tags":True }
         questions = []
         if edit["host"]:
             questions.append(inquirer.Text("host", message="Add Hostname or IP", default=defaults["host"]))
         else:
             profile["host"] = defaults["host"]
         if edit["protocol"]:
             questions.append(inquirer.Text("protocol", message="Select Protocol", validate=self._profile_protocol_validation, default=defaults["protocol"]))
@@ -836,42 +871,49 @@
             questions.append(inquirer.Text("options", message="Pass extra options to protocol", default=defaults["options"]))
         else:
             profile["options"] = defaults["options"]
         if edit["logs"]:
             questions.append(inquirer.Text("logs", message="Pick logging path/file ", default=defaults["logs"].replace("{","{{").replace("}","}}")))
         else:
             profile["logs"] = defaults["logs"]
+        if edit["tags"]:
+            questions.append(inquirer.Text("tags", message="Add tags dictionary",  validate=self._profile_tags_validation, default=str(defaults["tags"]).replace("{","{{").replace("}","}}")))
+        else:
+            profile["tags"] = defaults["tags"]
         if edit["user"]:
             questions.append(inquirer.Text("user", message="Pick username", default=defaults["user"]))
         else:
             profile["user"] = defaults["user"]
         if edit["password"]:
             questions.append(inquirer.Password("password", message="Set Password"))
         else:
             profile["password"] = defaults["password"]
         answer = inquirer.prompt(questions)
         if answer == None:
             return False
         if "password" in answer.keys():
             if answer["password"] != "":
                 answer["password"] = self.encrypt(answer["password"])
+        if "tags" in answer.keys() and answer["tags"]:
+            answer["tags"] = ast.literal_eval(answer["tags"])
         result = {**answer, **profile}
         result["id"] = unique
         return result
 
     def _questions_bulk(self):
         #Questions when using bulk command
         questions = []
         questions.append(inquirer.Text("ids", message="add a comma separated list of nodes to add", validate=self._bulk_node_validation))
         questions.append(inquirer.Text("location", message="Add a @folder, @subfolder@folder or leave empty", validate=self._bulk_folder_validation))
         questions.append(inquirer.Text("host", message="Add comma separated list of Hostnames or IPs", validate=self._bulk_host_validation))
         questions.append(inquirer.Text("protocol", message="Select Protocol", validate=self._protocol_validation))
         questions.append(inquirer.Text("port", message="Select Port Number", validate=self._port_validation))
         questions.append(inquirer.Text("options", message="Pass extra options to protocol", validate=self._default_validation))
         questions.append(inquirer.Text("logs", message="Pick logging path/file ", validate=self._default_validation))
+        questions.append(inquirer.Text("tags", message="Add tags dictionary",  validate=self._tags_validation))
         questions.append(inquirer.Text("user", message="Pick username", validate=self._default_validation))
         questions.append(inquirer.List("password", message="Password: Use a local password, no password or a list of profiles to reference?", choices=["Local Password", "Profiles", "No Password"]))
         answer = inquirer.prompt(questions)
         if answer == None:
             return False
         if "password" in answer.keys():
             if answer["password"] == "Local Password":
@@ -881,14 +923,16 @@
             elif answer["password"] == "Profiles":
                 passq = [(inquirer.Text("password", message="Set a @profile or a comma separated list of @profiles", validate=self._pass_validation))]
                 passa = inquirer.prompt(passq)
                 answer["password"] = passa["password"].split(",")
             elif answer["password"] == "No Password":
                 answer["password"] = ""
         answer["type"] = "connection"
+        if "tags" in answer.keys() and not answer["tags"].startswith("@") and answer["tags"]:
+            answer["tags"] = ast.literal_eval(answer["tags"])
         return answer
 
     def _type_node(self, arg_value, pat=re.compile(r"^[0-9a-zA-Z_.$@#-]+$")):
         if not pat.match(arg_value):
             raise argparse.ArgumentTypeError
         return arg_value
```

### Comparing `connpy-3.0.7/connpy/core.py` & `connpy-3.2.0/connpy/core.py`

 * *Files 3% similar despite different names*

```diff
@@ -29,15 +29,15 @@
 
         - status (int): 0 if the method run or test run succesfully.
                         1 if connection failed.
                         2 if expect timeouts without prompt or EOF.
 
         '''
     
-    def __init__(self, unique, host, options='', logs='', password='', port='', protocol='', user='', config=''):
+    def __init__(self, unique, host, options='', logs='', password='', port='', protocol='', user='', config='', tags=''):
         ''' 
             
         ### Parameters:  
 
             - unique (str): Unique name to assign to the node.
 
             - host   (str): IP address or hostname of the node.
@@ -59,27 +59,33 @@
             - protocol (str): Select ssh or telnet. Default is ssh.  
 
             - user     (str): Username to of the node.  
 
             - config   (obj): Pass the object created with class configfile with 
                               key for decryption and extra configuration if you 
                               are using connection manager.  
+
+            - tags   (dict) : Tags useful for automation and personal porpuse
+                              like "os", "prompt" and "screenleght_command"
         '''
         if config == '':
             self.idletime = 0
             self.key = None
         else:
             self.idletime = config.config["idletime"]
             self.key = config.key
         self.unique = unique
-        attr = {"host": host, "logs": logs, "options":options, "port": port, "protocol": protocol, "user": user}
+        attr = {"host": host, "logs": logs, "options":options, "port": port, "protocol": protocol, "user": user, "tags": tags}
         for key in attr:
-            profile = re.search("^@(.*)", attr[key])
+            profile = re.search("^@(.*)", str(attr[key]))
             if profile and config != '':
-                setattr(self,key,config.profiles[profile.group(1)][key])
+                try:
+                    setattr(self,key,config.profiles[profile.group(1)][key])
+                except:
+                    setattr(self,key,"")
             elif attr[key] == '' and key == "protocol":
                 try:
                     setattr(self,key,config.profiles["default"][key])
                 except:
                     setattr(self,key,"ssh")
             else: 
                 setattr(self,key,attr[key])
@@ -247,19 +253,23 @@
 
             str: Output of the commands you ran on the node.
 
         '''
         connect = self._connect(timeout = timeout)
         now = datetime.datetime.now().strftime('%Y-%m-%d_%H%M%S')
         if connect == True:
+            if "prompt" in self.tags:
+                prompt = self.tags["prompt"]
             expects = [prompt, pexpect.EOF, pexpect.TIMEOUT]
             output = ''
             status = ''
             if not isinstance(commands, list):
                 commands = [commands]
+            if "screen_length_command" in self.tags:
+                commands.insert(0, self.tags["screen_length_command"])
             self.mylog = io.BytesIO()
             self.child.logfile_read = self.mylog
             for c in commands:
                 if vars is not None:
                     c = c.format(**vars)
                 result = self.child.expect(expects, timeout = timeout)
                 self.child.sendline(c)
@@ -329,45 +339,50 @@
         ### Returns: 
             bool: true if expected value is found after running the commands 
                   false if prompt is found before.
 
         '''
         connect = self._connect(timeout = timeout)
         if connect == True:
+            if "prompt" in self.tags:
+                prompt = self.tags["prompt"]
             expects = [prompt, pexpect.EOF, pexpect.TIMEOUT]
             output = ''
             if not isinstance(commands, list):
                 commands = [commands]
+            if "screen_length_command" in self.tags:
+                commands.insert(0, self.tags["screen_length_command"])
             self.mylog = io.BytesIO()
             self.child.logfile_read = self.mylog
             for c in commands:
                 if vars is not None:
                     c = c.format(**vars)
                 result = self.child.expect(expects, timeout = timeout)
                 self.child.sendline(c)
                 if result == 2:
-                    result = 3
                     break
-            if not result == 3:
-                if vars is not None:
-                    expected = expected.format(**vars)
-                expects = [expected, prompt, pexpect.EOF, pexpect.TIMEOUT]
+            if not result == 2:
                 result = self.child.expect(expects, timeout = timeout)
             self.child.close()
             output = self._logclean(self.mylog.getvalue().decode(), True)
             self.output = output
-            if result == 0:
-                self.result = True
-                self.status = 0
-                return True
-            if result in [1, 2]:
-                self.result = False
+            if result in [0, 1]:
+                lastcommand = commands[-1]
+                if vars is not None:
+                    expected = expected.format(**vars)
+                    lastcommand = lastcommand.format(**vars)
+                last_command_index = output.rfind(lastcommand)
+                cleaned_output = output[last_command_index + len(lastcommand):].strip()
+                if expected in cleaned_output:
+                    self.result = True
+                else:
+                    self.result = False
                 self.status = 0
                 return False
-            if result == 3:
+            if result == 2:
                 self.result = None
                 self.status = 2
                 return output
         else:
             self.result = None
             self.output = connect
             self.status = 1
```

### Comparing `connpy-3.0.7/connpy.egg-info/PKG-INFO` & `connpy-3.2.0/connpy.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: connpy
-Version: 3.0.7
+Version: 3.2.0
 Summary: Connpy is a SSH/Telnet connection manager and automation module
 Home-page: https://github.com/fluzzi/connpy
 Author: Federico Luzzi
 Author-email: fluzzi@gmail.com
 License: MIT License
 Project-URL: Bug Tracker, https://github.com/fluzzi/connpy/issues
 Project-URL: Documentation, https://fluzzi.github.io/connpy/
@@ -32,15 +32,15 @@
 
 pip install connpy
 
 ## Automation module usage
 ### Standalone module
 ```
 import connpy
-router = connpy.node("unique name","ip/hostname", user="username", password="password")
+router = connpy.node("uniqueName","ip/host", user="username", password="password")
 router.run(["term len 0","show run"])
 print(router.output)
 hasip = router.test("show ip int brief","1.1.1.1")
 if hasip:
     print("Router has ip 1.1.1.1")
 else:
     print("router does not have ip 1.1.1.1")
@@ -64,17 +64,17 @@
 #You can also get each node individually:
 nodes = {}
 nodes["router1"] = conf.getitem("router1@office")
 nodes["router2"] = conf.getitem("router2@office")
 nodes["router10"] = conf.getitem("router10@datacenter")
 #Also, you can create the nodes manually:
 nodes = {}
-nodes["router1"] = {"host": "1.1.1.1", "user": "username", "password": "password1"}
-nodes["router2"] = {"host": "1.1.1.2", "user": "username", "password": "password2"}
-nodes["router3"] = {"host": "1.1.1.2", "user": "username", "password": "password3"}
+nodes["router1"] = {"host": "1.1.1.1", "user": "user", "password": "password1"}
+nodes["router2"] = {"host": "1.1.1.2", "user": "user", "password": "password2"}
+nodes["router3"] = {"host": "1.1.1.2", "user": "user", "password": "password3"}
 #Finally you run some tasks on the nodes
 mynodes = connpy.nodes(nodes, config = conf)
 result = mynodes.test(["show ip int br"], "1.1.1.2")
 for i in result:
     print("---" + i + "---")
     print(result[i])
     print()
@@ -100,15 +100,25 @@
 expected = "!"
 routers = connpy.nodes(nodes, config = config)
 routers.run(commands, variables)
 routers.test("ping {ip}", expected, variables)
 for key in routers.result:
     print(key, ' ---> ', ("pass" if routers.result[key] else "fail"))
 ```
-
+### Using AI
+```
+import connpy
+conf = connpy.configfile()
+organization = 'openai-org'
+api_key = "openai-key"
+myia = ai(conf, organization, api_key)
+input = "go to router 1 and get me the full configuration"
+result = myia.ask(input, dryrun = False)
+print(result)
+```
 ## Connection manager 
 ### Features
     - You can generate profiles and reference them from nodes using @profilename so you dont
       need to edit multiple nodes when changing password or other information.
     - Nodes can be stored on @folder or @subfolder@folder to organize your devices. Then can 
       be referenced using node@subfolder@folder or node@folder
     - If you have too many nodes. Get completion script using: conn config --completion.
@@ -200,15 +210,39 @@
 
 #### Response:
 
 - A JSON array containing the filtered list of nodes.
 
 ---
 
-### 2. Run Commands
+### 2. Get Nodes
+
+**Endpoint**: `/get_nodes`
+
+**Method**: `POST`
+
+**Description**: This route returns a dictionary of nodes with all their attributes. It can also filter the nodes based on a given keyword.
+
+#### Request Body:
+
+```json
+{
+  "filter": "<keyword>"
+}
+```
+
+* `filter` (optional): A keyword to filter the nodes. It returns only the nodes that contain the keyword. If not provided, the route will return the entire list of nodes.
+
+#### Response:
+
+- A JSON array containing the filtered nodes.
+
+---
+
+### 3. Run Commands
 
 **Endpoint**: `/run_commands`
 
 **Method**: `POST`
 
 **Description**: This route runs commands on selected nodes based on the provided action, nodes, and commands. It also supports executing tests by providing expected results.
 
@@ -229,7 +263,33 @@
 * `commands` (required): A list of commands to be executed on the specified nodes.
 * `expected` (optional, only used when the action is `test`): A single expected result for the test.
 * `options` (optional): Array to pass options to the run command, options are: `prompt`, `parallel`, `timeout`  
 
 #### Response:
 
 - A JSON object with the results of the executed commands on the nodes.
+
+### 4. Ask AI
+
+**Endpoint**: `/ask_ai`
+
+**Method**: `POST`
+
+**Description**: This route sends to chatgpt IA a request that will parse it into an understandable output for the application and then run the request.
+
+#### Request Body:
+
+```json
+{
+  "input": "<user input request>",
+  "dryrun": true or false
+}
+```
+
+* `input` (required): The user input requesting the AI to perform an action on some devices or get the devices list.
+* `dryrun` (optional): If set to true, it will return the parameters to run the request but it won't run it. default is false.
+
+#### Response:
+
+- A JSON array containing the action to run and the parameters and the result of the action.
+
+
```

### Comparing `connpy-3.0.7/setup.cfg` & `connpy-3.2.0/setup.cfg`

 * *Files 4% similar despite different names*

```diff
@@ -27,14 +27,16 @@
 install_requires = 
 	inquirer
 	pexpect
 	pycryptodome
 	Flask
 	waitress
 	PyYAML
+	openai
+	requests
 
 [options.extras_require]
 fuzzysearch = pyfzf
 
 [options.entry_points]
 console_scripts = 
 	conn = connpy.__main__:main
```

