# Comparing `tmp/commandsgpt-1.1.0.tar.gz` & `tmp/commandsgpt-1.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "commandsgpt-1.1.0.tar", last modified: Thu May  4 20:32:28 2023, max compression
+gzip compressed data, was "commandsgpt-1.1.1.tar", last modified: Fri May  5 16:28:45 2023, max compression
```

## Comparing `commandsgpt-1.1.0.tar` & `commandsgpt-1.1.1.tar`

### file list

```diff
@@ -1,24 +1,24 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 20:32:28.868513 commandsgpt-1.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1093 2023-05-04 20:32:11.000000 commandsgpt-1.1.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)    11387 2023-05-04 20:32:28.868513 commandsgpt-1.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     9457 2023-05-04 20:32:11.000000 commandsgpt-1.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 20:32:28.868513 commandsgpt-1.1.0/commands_gpt/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 20:32:28.868513 commandsgpt-1.1.0/commands_gpt/commands_gpt/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 20:32:11.000000 commandsgpt-1.1.0/commands_gpt/commands_gpt/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      393 2023-05-04 20:32:11.000000 commandsgpt-1.1.0/commands_gpt/commands_gpt/chat.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 20:32:28.868513 commandsgpt-1.1.0/commands_gpt/commands_gpt/commands/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-04 20:32:11.000000 commandsgpt-1.1.0/commands_gpt/commands_gpt/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3601 2023-05-04 20:32:11.000000 commandsgpt-1.1.0/commands_gpt/commands_gpt/commands/commands_funcs.py
--rw-r--r--   0 runner    (1001) docker     (123)     5332 2023-05-04 20:32:11.000000 commandsgpt-1.1.0/commands_gpt/commands_gpt/commands/graphs.py
--rw-r--r--   0 runner    (1001) docker     (123)      226 2023-05-04 20:32:11.000000 commandsgpt-1.1.0/commands_gpt/commands_gpt/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     4922 2023-05-04 20:32:11.000000 commandsgpt-1.1.0/commands_gpt/commands_gpt/instruction_recognition.py
--rw-r--r--   0 runner    (1001) docker     (123)      141 2023-05-04 20:32:11.000000 commandsgpt-1.1.0/commands_gpt/commands_gpt/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     3619 2023-05-04 20:32:11.000000 commandsgpt-1.1.0/commands_gpt/commands_gpt/regex.py
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-05-04 20:32:11.000000 commandsgpt-1.1.0/commands_gpt/commands_gpt/static.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-04 20:32:28.868513 commandsgpt-1.1.0/commands_gpt/commandsgpt.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    11387 2023-05-04 20:32:28.000000 commandsgpt-1.1.0/commands_gpt/commandsgpt.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      647 2023-05-04 20:32:28.000000 commandsgpt-1.1.0/commands_gpt/commandsgpt.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-04 20:32:28.000000 commandsgpt-1.1.0/commands_gpt/commandsgpt.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-04 20:32:28.000000 commandsgpt-1.1.0/commands_gpt/commandsgpt.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       84 2023-05-04 20:32:11.000000 commandsgpt-1.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      977 2023-05-04 20:32:28.868513 commandsgpt-1.1.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 16:28:45.797868 commandsgpt-1.1.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1093 2023-05-05 16:28:31.000000 commandsgpt-1.1.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)    11342 2023-05-05 16:28:45.797868 commandsgpt-1.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     9412 2023-05-05 16:28:31.000000 commandsgpt-1.1.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 16:28:45.793868 commandsgpt-1.1.1/commands_gpt/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 16:28:45.797868 commandsgpt-1.1.1/commands_gpt/commands_gpt/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 16:28:31.000000 commandsgpt-1.1.1/commands_gpt/commands_gpt/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      393 2023-05-05 16:28:31.000000 commandsgpt-1.1.1/commands_gpt/commands_gpt/chat.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 16:28:45.797868 commandsgpt-1.1.1/commands_gpt/commands_gpt/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-05 16:28:31.000000 commandsgpt-1.1.1/commands_gpt/commands_gpt/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3601 2023-05-05 16:28:31.000000 commandsgpt-1.1.1/commands_gpt/commands_gpt/commands/commands_funcs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5451 2023-05-05 16:28:31.000000 commandsgpt-1.1.1/commands_gpt/commands_gpt/commands/graphs.py
+-rw-r--r--   0 runner    (1001) docker     (123)      405 2023-05-05 16:28:31.000000 commandsgpt-1.1.1/commands_gpt/commands_gpt/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5030 2023-05-05 16:28:31.000000 commandsgpt-1.1.1/commands_gpt/commands_gpt/instruction_recognition.py
+-rw-r--r--   0 runner    (1001) docker     (123)      141 2023-05-05 16:28:31.000000 commandsgpt-1.1.1/commands_gpt/commands_gpt/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3619 2023-05-05 16:28:31.000000 commandsgpt-1.1.1/commands_gpt/commands_gpt/regex.py
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-05-05 16:28:31.000000 commandsgpt-1.1.1/commands_gpt/commands_gpt/static.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 16:28:45.797868 commandsgpt-1.1.1/commands_gpt/commandsgpt.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    11342 2023-05-05 16:28:45.000000 commandsgpt-1.1.1/commands_gpt/commandsgpt.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      647 2023-05-05 16:28:45.000000 commandsgpt-1.1.1/commands_gpt/commandsgpt.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 16:28:45.000000 commandsgpt-1.1.1/commands_gpt/commandsgpt.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-05-05 16:28:45.000000 commandsgpt-1.1.1/commands_gpt/commandsgpt.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       84 2023-05-05 16:28:31.000000 commandsgpt-1.1.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      977 2023-05-05 16:28:45.797868 commandsgpt-1.1.1/setup.cfg
```

### Comparing `commandsgpt-1.1.0/LICENSE` & `commandsgpt-1.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `commandsgpt-1.1.0/PKG-INFO` & `commandsgpt-1.1.1/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: commandsgpt
-Version: 1.1.0
+Version: 1.1.1
 Summary: An implementation of GPT-4 that recognizes which commands it must run to fulfill an instruction, using a graph. Create new commands easily by describing them using natural language and coding the functions corresponding to the commands.
 Home-page: https://github.com/AlexisAndradeDev/CommandsGPT
 Author: Martín Alexis Martínez Andrade
 Author-email: alexis.martinez.contacto@gmail.com
 Project-URL: Bug Tracker, https://github.com/AlexisAndradeDev/CommandsGPT/issues
 Project-URL: repository, https://github.com/AlexisAndradeDev/CommandsGPT
 Classifier: License :: OSI Approved :: MIT License
@@ -51,15 +51,15 @@
     },
     ...
 }
 ```
 
 *Example of a command function*
 ```
-def request_user_input_command(config: Config, message: str) -> dict[str, Any]:
+def request_user_input_command(config: Config, graph: Graph, message: str) -> dict[str, Any]:
     input_ = input(f"{message}\n*: ")
     results = {
         "input": input_,
     }
     return results
 ```
 
@@ -78,35 +78,35 @@
 ```
 from commands_gpt.commands.commands_funcs import add_essential_commands
 add_essential_commands(commands, command_name_to_func)
 ```
 
 Your `config` object: 
 ```
-config = Config("gpt-4-0314", commands, command_name_to_func)
+config = Config("gpt-4-0314", verbosity=1) # verbosity is optional
 ```
 
 Create an instruction:
 
 ```
 instruction = input("Enter your instruction: ")
 ```
 
 Pass your instruction to the recognizer model:
 
 ```
-graph, graph_data = recognize_instruction_and_create_graph(
-    instruction, config.chat_model, config.commands, config.command_name_to_func,
+graph = recognize_instruction_and_create_graph(
+    instruction, config.chat_model, commands, command_name_to_func,
 )
 ```
 
 Finally, execute the graph of commands:
 
 ```
-execute_commands(config, graph, graph_data, config.commands, config.command_name_to_func)
+graph.execute_commands(config)
 ```
 
 # Basic example
 
 ```
 from typing import Any
 from pathlib import Path
@@ -141,29 +141,29 @@
         },
         "generates_data": {},
     },
 }
 
 # Commands functions
 
-def write_to_user_command(config: Config, content: str) -> dict[str, Any]:
+def write_to_user_command(config: Config, graph: Graph, content: str) -> dict[str, Any]:
     # add newlines because regex data injection replaces newline characters
     # by \\n substrings.
     content_with_newlines = "\n".join(content.split("\\n"))
     print(f">>> {content_with_newlines}")
     return {}
 
-def request_user_input_command(config: Config, message: str) -> dict[str, Any]:
+def request_user_input_command(config: Config, graph: Graph, message: str) -> dict[str, Any]:
     input_ = input(f"{message}\n*: ")
     results = {
         "input": input_,
     }
     return results
 
-def write_file_command(config: Config, content: str, file_path: str) -> dict[str, Any]:
+def write_file_command(config: Config, graph: Graph, content: str, file_path: str) -> dict[str, Any]:
     file_dir = Path(file_path).parent
     assert file_dir.exists(), f"Container directory '{file_dir}' does not exist."
     with open(file_path, "w+", encoding="utf-8") as f:
         f.write(content)
         f.close()
     return {}
 
@@ -175,21 +175,21 @@
 }
 
 from commands_gpt.commands.commands_funcs import add_essential_commands
 add_essential_commands(commands, command_name_to_func)
 
 chat_model = "gpt-4-0314"
 
-config = Config(chat_model, commands, command_name_to_func)
+config = Config(chat_model, verbosity=1)
 
 instruction = input("Enter your prompt: ")
-graph, graph_data = recognize_instruction_and_create_graph(
-    instruction, config.chat_model, config.commands, config.command_name_to_func,
+graph = recognize_instruction_and_create_graph(
+    instruction, config.chat_model, commands, command_name_to_func,
 )
-execute_commands(config, graph, graph_data, config.commands, config.command_name_to_func)
+graph.execute_commands(config)
 ```
 
 # Adding custom commands
 
 You can add and modify your own custom commands by creating two dictionaries:
 
 * commands: The commands that the model can use, described in natural language. The keys are the name of the commands, and the values are dictionaries.
@@ -244,39 +244,39 @@
 }
 ```
 
 * command_name_to_func: The keys of this dictionary are the name of the commands, and the values are the function.
 
     * The name of the function is irrelevant.
 
-    * The first argument must be the Config object.
+    * The first argument must be the Config object. The second argument is the Graph object.
 
     * The arguments must match the arguments from the commands dictionary.
 
     * The return value must be a dictionary which keys must match the "generates_data" key.
 
     * The data types must match the ones declared in the commands dictionary.
 
 ***Example***
 ```
-def write_to_user_command(config: Config, content: str) -> dict[str, Any]:
+def write_to_user_command(config: Config, graph: Graph, content: str) -> dict[str, Any]:
     # add newlines because regex data injection replaces newline characters
     # by \\n substrings.
     content_with_newlines = "\n".join(content.split("\\n"))
     print(f">>> {content_with_newlines}")
     return {}
 
-def request_user_input_command(config: Config, message: str) -> dict[str, Any]:
+def request_user_input_command(config: Config, graph: Graph, message: str) -> dict[str, Any]:
     input_ = input(f"{message}\n*: ")
     results = {
         "input": input_,
     }
     return results
 
-def write_file_command(config: Config, content: str, file_path: str) -> dict[str, Any]:
+def write_file_command(config: Config, graph: Graph, content: str, file_path: str) -> dict[str, Any]:
     file_dir = Path(file_path).parent
     assert file_dir.exists(), f"Container directory '{file_dir}' does not exist."
     with open(file_path, "w+", encoding="utf-8") as f:
         f.write(content)
         f.close()
     return {}
```

### Comparing `commandsgpt-1.1.0/README.md` & `commandsgpt-1.1.1/README.md`

 * *Files 14% similar despite different names*

```diff
@@ -35,15 +35,15 @@
     },
     ...
 }
 ```
 
 *Example of a command function*
 ```
-def request_user_input_command(config: Config, message: str) -> dict[str, Any]:
+def request_user_input_command(config: Config, graph: Graph, message: str) -> dict[str, Any]:
     input_ = input(f"{message}\n*: ")
     results = {
         "input": input_,
     }
     return results
 ```
 
@@ -62,35 +62,35 @@
 ```
 from commands_gpt.commands.commands_funcs import add_essential_commands
 add_essential_commands(commands, command_name_to_func)
 ```
 
 Your `config` object: 
 ```
-config = Config("gpt-4-0314", commands, command_name_to_func)
+config = Config("gpt-4-0314", verbosity=1) # verbosity is optional
 ```
 
 Create an instruction:
 
 ```
 instruction = input("Enter your instruction: ")
 ```
 
 Pass your instruction to the recognizer model:
 
 ```
-graph, graph_data = recognize_instruction_and_create_graph(
-    instruction, config.chat_model, config.commands, config.command_name_to_func,
+graph = recognize_instruction_and_create_graph(
+    instruction, config.chat_model, commands, command_name_to_func,
 )
 ```
 
 Finally, execute the graph of commands:
 
 ```
-execute_commands(config, graph, graph_data, config.commands, config.command_name_to_func)
+graph.execute_commands(config)
 ```
 
 # Basic example
 
 ```
 from typing import Any
 from pathlib import Path
@@ -125,29 +125,29 @@
         },
         "generates_data": {},
     },
 }
 
 # Commands functions
 
-def write_to_user_command(config: Config, content: str) -> dict[str, Any]:
+def write_to_user_command(config: Config, graph: Graph, content: str) -> dict[str, Any]:
     # add newlines because regex data injection replaces newline characters
     # by \\n substrings.
     content_with_newlines = "\n".join(content.split("\\n"))
     print(f">>> {content_with_newlines}")
     return {}
 
-def request_user_input_command(config: Config, message: str) -> dict[str, Any]:
+def request_user_input_command(config: Config, graph: Graph, message: str) -> dict[str, Any]:
     input_ = input(f"{message}\n*: ")
     results = {
         "input": input_,
     }
     return results
 
-def write_file_command(config: Config, content: str, file_path: str) -> dict[str, Any]:
+def write_file_command(config: Config, graph: Graph, content: str, file_path: str) -> dict[str, Any]:
     file_dir = Path(file_path).parent
     assert file_dir.exists(), f"Container directory '{file_dir}' does not exist."
     with open(file_path, "w+", encoding="utf-8") as f:
         f.write(content)
         f.close()
     return {}
 
@@ -159,21 +159,21 @@
 }
 
 from commands_gpt.commands.commands_funcs import add_essential_commands
 add_essential_commands(commands, command_name_to_func)
 
 chat_model = "gpt-4-0314"
 
-config = Config(chat_model, commands, command_name_to_func)
+config = Config(chat_model, verbosity=1)
 
 instruction = input("Enter your prompt: ")
-graph, graph_data = recognize_instruction_and_create_graph(
-    instruction, config.chat_model, config.commands, config.command_name_to_func,
+graph = recognize_instruction_and_create_graph(
+    instruction, config.chat_model, commands, command_name_to_func,
 )
-execute_commands(config, graph, graph_data, config.commands, config.command_name_to_func)
+graph.execute_commands(config)
 ```
 
 # Adding custom commands
 
 You can add and modify your own custom commands by creating two dictionaries:
 
 * commands: The commands that the model can use, described in natural language. The keys are the name of the commands, and the values are dictionaries.
@@ -228,39 +228,39 @@
 }
 ```
 
 * command_name_to_func: The keys of this dictionary are the name of the commands, and the values are the function.
 
     * The name of the function is irrelevant.
 
-    * The first argument must be the Config object.
+    * The first argument must be the Config object. The second argument is the Graph object.
 
     * The arguments must match the arguments from the commands dictionary.
 
     * The return value must be a dictionary which keys must match the "generates_data" key.
 
     * The data types must match the ones declared in the commands dictionary.
 
 ***Example***
 ```
-def write_to_user_command(config: Config, content: str) -> dict[str, Any]:
+def write_to_user_command(config: Config, graph: Graph, content: str) -> dict[str, Any]:
     # add newlines because regex data injection replaces newline characters
     # by \\n substrings.
     content_with_newlines = "\n".join(content.split("\\n"))
     print(f">>> {content_with_newlines}")
     return {}
 
-def request_user_input_command(config: Config, message: str) -> dict[str, Any]:
+def request_user_input_command(config: Config, graph: Graph, message: str) -> dict[str, Any]:
     input_ = input(f"{message}\n*: ")
     results = {
         "input": input_,
     }
     return results
 
-def write_file_command(config: Config, content: str, file_path: str) -> dict[str, Any]:
+def write_file_command(config: Config, graph: Graph, content: str, file_path: str) -> dict[str, Any]:
     file_dir = Path(file_path).parent
     assert file_dir.exists(), f"Container directory '{file_dir}' does not exist."
     with open(file_path, "w+", encoding="utf-8") as f:
         f.write(content)
         f.close()
     return {}
```

### Comparing `commandsgpt-1.1.0/commands_gpt/commands_gpt/commands/commands_funcs.py` & `commandsgpt-1.1.1/commands_gpt/commands_gpt/commands/commands_funcs.py`

 * *Files identical despite different names*

### Comparing `commandsgpt-1.1.0/commands_gpt/commands_gpt/commands/graphs.py` & `commandsgpt-1.1.1/commands_gpt/commands_gpt/commands/graphs.py`

 * *Files 3% similar despite different names*

```diff
@@ -28,27 +28,29 @@
         return self.id < other.id
 
     def __str__(self):
         return f"CommandNode(id={self.id}, previous_command_id={self.previous_command_id}, dependent_on_data={self.dependent_on_data}, required_value={self.required_value}, command={self.command})"
 
     def execute_command(self, config: Config, graph, arguments: dict[str, Any]):
         print(f"\n\nRunning '{self.command_name}' command with id {self.id}...")
+        if config.verbosity >= 2:
+            print(f"Using arguments: {arguments}")
         self.data_generated = self.command(config, graph, **arguments)
 
 class Graph:
     def __init__(self, raw_commands_data: StaticVar, commands: dict[str, dict], 
             command_name_to_func: dict[str, Callable]):
         self.build_graph(raw_commands_data, commands, command_name_to_func)
 
     def build_graph(self, raw_commands_data: StaticVar, commands: dict[str, dict], 
             command_name_to_func: dict[str, Callable]):
         self.raw_commands_data = raw_commands_data
         self.commands = commands
         self.command_name_to_func = command_name_to_func
-        self.commands_data, self.data_references = generate_graph_data(raw_commands_data)
+        self.commands_data, self.data_references = generate_graph_data(raw_commands_data.val)
         self.build_nodes()
 
     def build_nodes(self):
         self.nodes: dict[str, CommandNode] = {}
         for command_data in self.commands_data:
             node = CommandNode(command_data, self.commands, self.command_name_to_func)
             self.nodes[node.id] = node
@@ -95,15 +97,16 @@
                 print(f"\n\tExecuted after node «{node.previous_command_id}».")
             if node.dependent_on_data:
                 print(f"\n\t\tResult field '{node.dependent_on_data}' of node «{node.previous_command_id}» must have value «{node.required_value}» in order to execute this node.")
         print("\n--- -------------- ---\n")
 
     def execute_commands(self, config: Config):
         self.initialize_graph()
-        self.print_graph()
+        if config.verbosity >= 1:
+            self.print_graph()
 
         for node_id in sorted(self.nodes.keys()):
             self.execute_node(node_id, config)
 
 def generate_graph_data(raw_commands_data):
     """
     Parses a commands data string to a JSON to create the graph data
@@ -114,16 +117,16 @@
     Returns:
         a tuple: Containing:
         
             commands_data: data of the commands (to create a graph).
 
             data_references: data references (data that will be injected).
     """
-    data_references = regex.find_data_references_indices(raw_commands_data.val)
-    commands_data = regex.nullify_all_data_references(raw_commands_data.val)
+    data_references = regex.find_data_references_indices(raw_commands_data)
+    commands_data = regex.nullify_all_data_references(raw_commands_data)
 
     # TODO: Fix JSON parsing error that is sometimes raised when newline characters are written.
     try:
         commands_data = json.loads(commands_data, strict=False)
     except Exception as e:
         print(f"!!! Raw commands data: {raw_commands_data}")
         raise e
```

### Comparing `commandsgpt-1.1.0/commands_gpt/commands_gpt/instruction_recognition.py` & `commandsgpt-1.1.1/commands_gpt/commands_gpt/instruction_recognition.py`

 * *Files 2% similar despite different names*

```diff
@@ -46,14 +46,17 @@
             """\n\nExample 2:"""
             """\nUser prompt: 'Read my clipboard, write a scientific article about the content in it, and save it as a file with a name related to the article.'"""
             """\nYour response might be: '[[1, [], "%s", {}], [2, [1, null, null], "%s", {"about": "Scientific article about __&1.content__"}], [3, [2, null, null], "%s", {"about": "Name including extension to save a file about this article: __&2.thought__"}], [4, [3, null, null], "%s", {"content": "__&2.thought__", "file_name": "__&3.thought__"}]]'""" % ("READ_CLIPBOARD", "THINK", "THINK", "WRITE_FILE")
             +
             """\n\nExample 3:"""
             """\nUser prompt: 'Look up the best courses on ASP.Net on Google and show me the first page that appears, if it is relevant.'"""
             """\nYour response might be: '[[1, [], "%s", {"query": "best courses on ASP.Net"}], [2, [1, null, null], "%s", {"url": "__&1.urls[0]__"}], [3, [2, null, null], "%s", {"condition": "Is this a relevant course on ASP.Net? __&2.text__"}], [4, [3, "result", 1], "%s", {"content": "Relevant course: __&1.urls[0]__"}], [5, [3, "result", 0], "%s", {"content": "It is not relevant."}]]'""" % ("SEARCH_GOOGLE", "READ_WEBPAGE", "IF", "WRITE_TO_USER", "WRITE_TO_USER")
+            +
+
+            """\n\nThe structure is JSON-like (so, use double quotes to create str, etc.)"""
         }
     ]
     messages.append({"role": "user", "content": instruction})
     print(f"Tokens used by messages: ~{len(str(messages)) / 4} tokens.")
 
     print("Recognizing...")
     response = openai.ChatCompletion.create(
```

### Comparing `commandsgpt-1.1.0/commands_gpt/commands_gpt/regex.py` & `commandsgpt-1.1.1/commands_gpt/commands_gpt/regex.py`

 * *Files identical despite different names*

### Comparing `commandsgpt-1.1.0/commands_gpt/commandsgpt.egg-info/PKG-INFO` & `commandsgpt-1.1.1/commands_gpt/commandsgpt.egg-info/PKG-INFO`

 * *Files 7% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: commandsgpt
-Version: 1.1.0
+Version: 1.1.1
 Summary: An implementation of GPT-4 that recognizes which commands it must run to fulfill an instruction, using a graph. Create new commands easily by describing them using natural language and coding the functions corresponding to the commands.
 Home-page: https://github.com/AlexisAndradeDev/CommandsGPT
 Author: Martín Alexis Martínez Andrade
 Author-email: alexis.martinez.contacto@gmail.com
 Project-URL: Bug Tracker, https://github.com/AlexisAndradeDev/CommandsGPT/issues
 Project-URL: repository, https://github.com/AlexisAndradeDev/CommandsGPT
 Classifier: License :: OSI Approved :: MIT License
@@ -51,15 +51,15 @@
     },
     ...
 }
 ```
 
 *Example of a command function*
 ```
-def request_user_input_command(config: Config, message: str) -> dict[str, Any]:
+def request_user_input_command(config: Config, graph: Graph, message: str) -> dict[str, Any]:
     input_ = input(f"{message}\n*: ")
     results = {
         "input": input_,
     }
     return results
 ```
 
@@ -78,35 +78,35 @@
 ```
 from commands_gpt.commands.commands_funcs import add_essential_commands
 add_essential_commands(commands, command_name_to_func)
 ```
 
 Your `config` object: 
 ```
-config = Config("gpt-4-0314", commands, command_name_to_func)
+config = Config("gpt-4-0314", verbosity=1) # verbosity is optional
 ```
 
 Create an instruction:
 
 ```
 instruction = input("Enter your instruction: ")
 ```
 
 Pass your instruction to the recognizer model:
 
 ```
-graph, graph_data = recognize_instruction_and_create_graph(
-    instruction, config.chat_model, config.commands, config.command_name_to_func,
+graph = recognize_instruction_and_create_graph(
+    instruction, config.chat_model, commands, command_name_to_func,
 )
 ```
 
 Finally, execute the graph of commands:
 
 ```
-execute_commands(config, graph, graph_data, config.commands, config.command_name_to_func)
+graph.execute_commands(config)
 ```
 
 # Basic example
 
 ```
 from typing import Any
 from pathlib import Path
@@ -141,29 +141,29 @@
         },
         "generates_data": {},
     },
 }
 
 # Commands functions
 
-def write_to_user_command(config: Config, content: str) -> dict[str, Any]:
+def write_to_user_command(config: Config, graph: Graph, content: str) -> dict[str, Any]:
     # add newlines because regex data injection replaces newline characters
     # by \\n substrings.
     content_with_newlines = "\n".join(content.split("\\n"))
     print(f">>> {content_with_newlines}")
     return {}
 
-def request_user_input_command(config: Config, message: str) -> dict[str, Any]:
+def request_user_input_command(config: Config, graph: Graph, message: str) -> dict[str, Any]:
     input_ = input(f"{message}\n*: ")
     results = {
         "input": input_,
     }
     return results
 
-def write_file_command(config: Config, content: str, file_path: str) -> dict[str, Any]:
+def write_file_command(config: Config, graph: Graph, content: str, file_path: str) -> dict[str, Any]:
     file_dir = Path(file_path).parent
     assert file_dir.exists(), f"Container directory '{file_dir}' does not exist."
     with open(file_path, "w+", encoding="utf-8") as f:
         f.write(content)
         f.close()
     return {}
 
@@ -175,21 +175,21 @@
 }
 
 from commands_gpt.commands.commands_funcs import add_essential_commands
 add_essential_commands(commands, command_name_to_func)
 
 chat_model = "gpt-4-0314"
 
-config = Config(chat_model, commands, command_name_to_func)
+config = Config(chat_model, verbosity=1)
 
 instruction = input("Enter your prompt: ")
-graph, graph_data = recognize_instruction_and_create_graph(
-    instruction, config.chat_model, config.commands, config.command_name_to_func,
+graph = recognize_instruction_and_create_graph(
+    instruction, config.chat_model, commands, command_name_to_func,
 )
-execute_commands(config, graph, graph_data, config.commands, config.command_name_to_func)
+graph.execute_commands(config)
 ```
 
 # Adding custom commands
 
 You can add and modify your own custom commands by creating two dictionaries:
 
 * commands: The commands that the model can use, described in natural language. The keys are the name of the commands, and the values are dictionaries.
@@ -244,39 +244,39 @@
 }
 ```
 
 * command_name_to_func: The keys of this dictionary are the name of the commands, and the values are the function.
 
     * The name of the function is irrelevant.
 
-    * The first argument must be the Config object.
+    * The first argument must be the Config object. The second argument is the Graph object.
 
     * The arguments must match the arguments from the commands dictionary.
 
     * The return value must be a dictionary which keys must match the "generates_data" key.
 
     * The data types must match the ones declared in the commands dictionary.
 
 ***Example***
 ```
-def write_to_user_command(config: Config, content: str) -> dict[str, Any]:
+def write_to_user_command(config: Config, graph: Graph, content: str) -> dict[str, Any]:
     # add newlines because regex data injection replaces newline characters
     # by \\n substrings.
     content_with_newlines = "\n".join(content.split("\\n"))
     print(f">>> {content_with_newlines}")
     return {}
 
-def request_user_input_command(config: Config, message: str) -> dict[str, Any]:
+def request_user_input_command(config: Config, graph: Graph, message: str) -> dict[str, Any]:
     input_ = input(f"{message}\n*: ")
     results = {
         "input": input_,
     }
     return results
 
-def write_file_command(config: Config, content: str, file_path: str) -> dict[str, Any]:
+def write_file_command(config: Config, graph: Graph, content: str, file_path: str) -> dict[str, Any]:
     file_dir = Path(file_path).parent
     assert file_dir.exists(), f"Container directory '{file_dir}' does not exist."
     with open(file_path, "w+", encoding="utf-8") as f:
         f.write(content)
         f.close()
     return {}
```

### Comparing `commandsgpt-1.1.0/commands_gpt/commandsgpt.egg-info/SOURCES.txt` & `commandsgpt-1.1.1/commands_gpt/commandsgpt.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `commandsgpt-1.1.0/setup.cfg` & `commandsgpt-1.1.1/setup.cfg`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = commandsgpt
-version = 1.1.0
+version = 1.1.1
 author = Martín Alexis Martínez Andrade
 author_email = alexis.martinez.contacto@gmail.com
 description = An implementation of GPT-4 that recognizes which commands it must run to fulfill an instruction, using a graph. Create new commands easily by describing them using natural language and coding the functions corresponding to the commands.
 long_description = file: README.md, LICENSE
 long_description_content_type = text/markdown
 url = https://github.com/AlexisAndradeDev/CommandsGPT
 project_urls =
```

