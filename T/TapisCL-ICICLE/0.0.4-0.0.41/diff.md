# Comparing `tmp/TapisCL-ICICLE-0.0.4.tar.gz` & `tmp/TapisCL-ICICLE-0.0.41.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "TapisCL-ICICLE-0.0.4.tar", last modified: Sat Apr 29 19:04:23 2023, max compression
+gzip compressed data, was "TapisCL-ICICLE-0.0.41.tar", last modified: Fri May  5 04:55:44 2023, max compression
```

## Comparing `TapisCL-ICICLE-0.0.4.tar` & `TapisCL-ICICLE-0.0.41.tar`

### file list

```diff
@@ -1,36 +1,37 @@
-drwxrwxrwx   0        0        0        0 2023-04-29 19:04:23.343618 TapisCL-ICICLE-0.0.4/
--rw-rw-rw-   0        0        0    35823 2023-04-12 23:35:22.000000 TapisCL-ICICLE-0.0.4/LICENSE
--rw-rw-rw-   0        0        0    45181 2023-04-29 19:04:23.343618 TapisCL-ICICLE-0.0.4/PKG-INFO
--rw-rw-rw-   0        0        0     3270 2023-04-29 18:49:44.000000 TapisCL-ICICLE-0.0.4/README.md
-drwxrwxrwx   0        0        0        0 2023-04-29 19:04:23.328060 TapisCL-ICICLE-0.0.4/TapisCLICICLE/
--rw-rw-rw-   0        0        0        0 2023-04-12 23:35:22.000000 TapisCL-ICICLE-0.0.4/TapisCLICICLE/__init__.py
--rw-rw-rw-   0        0        0      132 2023-04-12 23:35:22.000000 TapisCL-ICICLE-0.0.4/TapisCLICICLE/__main__.py
--rw-rw-rw-   0        0        0    11350 2023-04-29 18:56:06.000000 TapisCL-ICICLE-0.0.4/TapisCLICICLE/cli.py
-drwxrwxrwx   0        0        0        0 2023-04-29 19:04:23.334039 TapisCL-ICICLE-0.0.4/TapisCLICICLE/commands/
--rw-rw-rw-   0        0        0        0 2023-04-28 22:36:06.000000 TapisCL-ICICLE-0.0.4/TapisCLICICLE/commands/__init__.py
--rw-rw-rw-   0        0        0     3663 2023-04-28 22:36:06.000000 TapisCL-ICICLE-0.0.4/TapisCLICICLE/commands/apps.py
--rw-rw-rw-   0        0        0     2158 2023-04-29 18:35:45.000000 TapisCL-ICICLE-0.0.4/TapisCLICICLE/commands/baseWrappers.py
--rw-rw-rw-   0        0        0     2459 2023-04-28 22:36:06.000000 TapisCL-ICICLE-0.0.4/TapisCLICICLE/commands/files.py
--rw-rw-rw-   0        0        0     5416 2023-04-28 22:36:06.000000 TapisCL-ICICLE-0.0.4/TapisCLICICLE/commands/pods.py
--rw-rw-rw-   0        0        0     2024 2023-04-28 22:36:06.000000 TapisCL-ICICLE-0.0.4/TapisCLICICLE/commands/query.py
--rw-rw-rw-   0        0        0     5022 2023-04-29 18:25:51.000000 TapisCL-ICICLE-0.0.4/TapisCLICICLE/commands/serverCommands.py
--rw-rw-rw-   0        0        0     5353 2023-04-28 22:36:06.000000 TapisCL-ICICLE-0.0.4/TapisCLICICLE/commands/systems.py
--rw-rw-rw-   0        0        0     8464 2023-04-29 19:03:22.000000 TapisCL-ICICLE-0.0.4/TapisCLICICLE/server.py
-drwxrwxrwx   0        0        0        0 2023-04-29 19:04:23.338635 TapisCL-ICICLE-0.0.4/TapisCLICICLE/utilities/
--rw-rw-rw-   0        0        0        0 2023-04-28 22:36:06.000000 TapisCL-ICICLE-0.0.4/TapisCLICICLE/utilities/__init__.py
--rw-rw-rw-   0        0        0     1474 2023-04-28 22:36:06.000000 TapisCL-ICICLE-0.0.4/TapisCLICICLE/utilities/args.py
--rw-rw-rw-   0        0        0     9545 2023-04-29 18:02:05.000000 TapisCL-ICICLE-0.0.4/TapisCLICICLE/utilities/decorators.py
--rw-rw-rw-   0        0        0     2121 2023-04-29 18:26:16.000000 TapisCL-ICICLE-0.0.4/TapisCLICICLE/utilities/exceptions.py
--rw-rw-rw-   0        0        0     6069 2023-04-28 22:36:06.000000 TapisCL-ICICLE-0.0.4/TapisCLICICLE/utilities/helpers.py
--rw-rw-rw-   0        0        0      925 2023-04-29 17:45:39.000000 TapisCL-ICICLE-0.0.4/TapisCLICICLE/utilities/logger.py
--rw-rw-rw-   0        0        0     2127 2023-04-29 18:53:15.000000 TapisCL-ICICLE-0.0.4/TapisCLICICLE/utilities/schemas.py
--rw-rw-rw-   0        0        0     1844 2023-04-29 17:29:42.000000 TapisCL-ICICLE-0.0.4/TapisCLICICLE/utilities/socketOpts.py
-drwxrwxrwx   0        0        0        0 2023-04-29 19:04:23.342621 TapisCL-ICICLE-0.0.4/TapisCL_ICICLE.egg-info/
--rw-rw-rw-   0        0        0    45181 2023-04-29 19:04:23.000000 TapisCL-ICICLE-0.0.4/TapisCL_ICICLE.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      920 2023-04-29 19:04:23.000000 TapisCL-ICICLE-0.0.4/TapisCL_ICICLE.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-29 19:04:23.000000 TapisCL-ICICLE-0.0.4/TapisCL_ICICLE.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       59 2023-04-29 19:04:23.000000 TapisCL-ICICLE-0.0.4/TapisCL_ICICLE.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       57 2023-04-29 19:04:23.000000 TapisCL-ICICLE-0.0.4/TapisCL_ICICLE.egg-info/requires.txt
--rw-rw-rw-   0        0        0       14 2023-04-29 19:04:23.000000 TapisCL-ICICLE-0.0.4/TapisCL_ICICLE.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     1084 2023-04-29 18:41:37.000000 TapisCL-ICICLE-0.0.4/pyproject.toml
--rw-rw-rw-   0        0        0       42 2023-04-29 19:04:23.343618 TapisCL-ICICLE-0.0.4/setup.cfg
+drwxrwxrwx   0        0        0        0 2023-05-05 04:55:44.307656 TapisCL-ICICLE-0.0.41/
+-rw-rw-rw-   0        0        0    35823 2023-04-12 23:35:22.000000 TapisCL-ICICLE-0.0.41/LICENSE
+-rw-rw-rw-   0        0        0    45182 2023-05-05 04:55:44.307656 TapisCL-ICICLE-0.0.41/PKG-INFO
+-rw-rw-rw-   0        0        0     3270 2023-04-29 18:49:44.000000 TapisCL-ICICLE-0.0.41/README.md
+drwxrwxrwx   0        0        0        0 2023-05-05 04:55:44.292088 TapisCL-ICICLE-0.0.41/TapisCLICICLE/
+-rw-rw-rw-   0        0        0        0 2023-04-12 23:35:22.000000 TapisCL-ICICLE-0.0.41/TapisCLICICLE/__init__.py
+-rw-rw-rw-   0        0        0      132 2023-04-12 23:35:22.000000 TapisCL-ICICLE-0.0.41/TapisCLICICLE/__main__.py
+-rw-rw-rw-   0        0        0    11616 2023-05-05 01:58:15.000000 TapisCL-ICICLE-0.0.41/TapisCLICICLE/cli.py
+drwxrwxrwx   0        0        0        0 2023-05-05 04:55:44.296180 TapisCL-ICICLE-0.0.41/TapisCLICICLE/commands/
+-rw-rw-rw-   0        0        0        0 2023-04-28 22:36:06.000000 TapisCL-ICICLE-0.0.41/TapisCLICICLE/commands/__init__.py
+-rw-rw-rw-   0        0        0     3705 2023-05-04 21:09:52.000000 TapisCL-ICICLE-0.0.41/TapisCLICICLE/commands/apps.py
+-rw-rw-rw-   0        0        0     2164 2023-05-04 21:08:20.000000 TapisCL-ICICLE-0.0.41/TapisCLICICLE/commands/baseWrappers.py
+-rw-rw-rw-   0        0        0     2477 2023-05-04 21:08:10.000000 TapisCL-ICICLE-0.0.41/TapisCLICICLE/commands/files.py
+-rw-rw-rw-   0        0        0     5482 2023-05-04 21:07:53.000000 TapisCL-ICICLE-0.0.41/TapisCLICICLE/commands/pods.py
+-rw-rw-rw-   0        0        0     2036 2023-05-04 21:06:58.000000 TapisCL-ICICLE-0.0.41/TapisCLICICLE/commands/query.py
+-rw-rw-rw-   0        0        0     5089 2023-05-05 02:51:57.000000 TapisCL-ICICLE-0.0.41/TapisCLICICLE/commands/serverCommands.py
+-rw-rw-rw-   0        0        0     5389 2023-05-04 21:05:56.000000 TapisCL-ICICLE-0.0.41/TapisCLICICLE/commands/systems.py
+-rw-rw-rw-   0        0        0     8231 2023-05-05 04:54:37.000000 TapisCL-ICICLE-0.0.41/TapisCLICICLE/server.py
+drwxrwxrwx   0        0        0        0 2023-05-05 04:55:44.302159 TapisCL-ICICLE-0.0.41/TapisCLICICLE/utilities/
+-rw-rw-rw-   0        0        0        0 2023-04-28 22:36:06.000000 TapisCL-ICICLE-0.0.41/TapisCLICICLE/utilities/__init__.py
+-rw-rw-rw-   0        0        0     1474 2023-04-28 22:36:06.000000 TapisCL-ICICLE-0.0.41/TapisCLICICLE/utilities/args.py
+-rw-rw-rw-   0        0        0     9449 2023-05-05 02:42:29.000000 TapisCL-ICICLE-0.0.41/TapisCLICICLE/utilities/decorators.py
+-rw-rw-rw-   0        0        0     2121 2023-04-29 18:26:16.000000 TapisCL-ICICLE-0.0.41/TapisCLICICLE/utilities/exceptions.py
+-rw-rw-rw-   0        0        0     6098 2023-05-05 02:34:10.000000 TapisCL-ICICLE-0.0.41/TapisCLICICLE/utilities/helpers.py
+-rw-rw-rw-   0        0        0      925 2023-04-29 17:45:39.000000 TapisCL-ICICLE-0.0.41/TapisCLICICLE/utilities/logger.py
+-rw-rw-rw-   0        0        0     2127 2023-04-29 18:53:15.000000 TapisCL-ICICLE-0.0.41/TapisCLICICLE/utilities/schemas.py
+-rw-rw-rw-   0        0        0      493 2023-05-05 04:54:37.000000 TapisCL-ICICLE-0.0.41/TapisCLICICLE/utilities/serverConnection.py
+-rw-rw-rw-   0        0        0     2525 2023-05-05 02:37:18.000000 TapisCL-ICICLE-0.0.41/TapisCLICICLE/utilities/socketOpts.py
+drwxrwxrwx   0        0        0        0 2023-05-05 04:55:44.306659 TapisCL-ICICLE-0.0.41/TapisCL_ICICLE.egg-info/
+-rw-rw-rw-   0        0        0    45182 2023-05-05 04:55:44.000000 TapisCL-ICICLE-0.0.41/TapisCL_ICICLE.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      964 2023-05-05 04:55:44.000000 TapisCL-ICICLE-0.0.41/TapisCL_ICICLE.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-05 04:55:44.000000 TapisCL-ICICLE-0.0.41/TapisCL_ICICLE.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       59 2023-05-05 04:55:44.000000 TapisCL-ICICLE-0.0.41/TapisCL_ICICLE.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       57 2023-05-05 04:55:44.000000 TapisCL-ICICLE-0.0.41/TapisCL_ICICLE.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       14 2023-05-05 04:55:44.000000 TapisCL-ICICLE-0.0.41/TapisCL_ICICLE.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     1085 2023-05-05 04:54:14.000000 TapisCL-ICICLE-0.0.41/pyproject.toml
+-rw-rw-rw-   0        0        0       42 2023-05-05 04:55:44.308158 TapisCL-ICICLE-0.0.41/setup.cfg
```

### Comparing `TapisCL-ICICLE-0.0.4/LICENSE` & `TapisCL-ICICLE-0.0.41/LICENSE`

 * *Files identical despite different names*

### Comparing `TapisCL-ICICLE-0.0.4/PKG-INFO` & `TapisCL-ICICLE-0.0.41/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: TapisCL-ICICLE
-Version: 0.0.4
+Version: 0.0.41
 Summary: Provide good performance command line user interface for Tapis services hosted on HPC clusters
 Author-email: Michael Ray <ahumanbeing189@gmail.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `TapisCL-ICICLE-0.0.4/README.md` & `TapisCL-ICICLE-0.0.41/README.md`

 * *Files identical despite different names*

### Comparing `TapisCL-ICICLE-0.0.4/TapisCLICICLE/cli.py` & `TapisCL-ICICLE-0.0.41/TapisCLICICLE/cli.py`

 * *Files 5% similar despite different names*

```diff
@@ -22,15 +22,15 @@
 
 
 __location__ = os.path.realpath(
     os.path.join(os.getcwd(), os.path.dirname(__file__)))
 server_path = os.path.join(__location__, 'server.py')
 
 
-class CLI(SO.SocketOpts, helpers.OperationsHelper, decorators.DecoratorSetup, helpers.Formatters):
+class CLI(SO.ClientSocketOpts, helpers.OperationsHelper, decorators.DecoratorSetup, helpers.Formatters):
     """
     Receive user input, either direct from bash environment or from the custom interface, then parse these commands and send them to the server to be executed. 
     """
     def __init__(self, IP: str, PORT: int):
 
         self.ip, self.port = IP, PORT
         self.connection = socket.socket(socket.AF_INET, socket.SOCK_STREAM) 
@@ -87,35 +87,36 @@
 
     def connect(self):
         """
         connect to the local server
         """
         self.connection_initialization() 
         #self.connection.connect((self.ip, self.port)) # enable me for debugging. Requires manual server start
-        connection_info: schemas.StartupData = self.schema_unpack() # receive info from the server whether it is a first time connection
+        connection_info: schemas.StartupData = self.schema_unpack_explicit(self.connection) # receive info from the server whether it is a first time connection
         if connection_info.initial: # if the server is receiving its first connection for the session\
             while True:
                 try:
                     url = str(input("\nEnter the link for the tapis service you are connecting to: ")).strip()
                 except KeyboardInterrupt:
                     url = " "
                     pass
                 url_data = schemas.StartupData(url=url)
-                self.json_send(url_data.dict())
-                auth_request: schemas.AuthRequest = self.schema_unpack()
+                self.json_send_explicit(self.connection, url_data.dict())
+                print("URL send")
+                auth_request: schemas.AuthRequest = self.schema_unpack_explicit(self.connection)
                 try:
                     username = str(input("\nUsername: ")).strip()
                     password = getpass("Password: ").strip() 
                 except KeyboardInterrupt:
                     username, password = " ", " "
                     pass
                 auth_data = schemas.AuthData(username = username, password = password)
-                self.json_send(auth_data.dict())
+                self.json_send_explicit(self.connection, auth_data.dict())
 
-                verification: schemas.ResponseData | schemas.StartupData = self.schema_unpack() 
+                verification: schemas.ResponseData | schemas.StartupData = self.schema_unpack_explicit(self.connection)
                 if verification.schema_type == 'StartupData': # verification success, program moves forward
                     return verification.username, verification.url
                 else: # verification failed. User has 3 tries, afterwards the program will shut down
                     print(f"[-] verification failure, attempt # {verification.response_message[1]}")
                     if verification.response_message[1] == 3:
                         sys.exit(0)
                     continue
@@ -200,21 +201,21 @@
         return filled_form
     
     def special_forms_ops(self):
         """
         handle special form requests sent by the server
         """
         while True:
-            message = self.schema_unpack()
+            message = self.schema_unpack_explicit(self.connection)
             message_type = message.schema_type
             if message_type in self.message_handlers.keys():
                 filled_form = self.message_handlers[message_type](message)
             else:
                 return message
-            self.json_send(filled_form.dict())
+            self.json_send_explicit(self.connection, filled_form.dict())
 
     def environment_cli_response_stream_handler(self, response):
         if response.schema_type == 'ResponseData' and response.exit_status: # if the command was a shutdown or exit, close the program
             self.print_response(response.response_message)
             os._exit(0)
         elif response.schema_type == 'ResponseData':
             if response.active_username:
@@ -227,15 +228,15 @@
         try:
             kwargs = self.parser.parse_args()
         except:
             print("Invalid Arguments")
             os._exit(0)
         kwargs = vars(kwargs)
         command = self.command_input_parser(kwargs, exit_=1) # operate with args, send them over
-        self.json_send(command.dict())
+        self.json_send_explicit(self.connection, command.dict())
         response = self.special_forms_ops()
         if response.schema_type == 'ResponseData':
             self.print_response(response.response_message)
         os._exit(0)
 
     def environment_cli(self):
         title = pyfiglet.figlet_format("-----------\nTapisCLICICLE\n-----------", font="slant") # print the title when CLI is accessed
@@ -247,15 +248,15 @@
                 kwargs = self.process_command(str(input(f"[{self.username}@{self.url}] "))) # ask for and process user input
                 try:
                     command = self.command_input_parser(kwargs) # run operations
                 except:
                     continue
                 if not command:
                     continue
-                self.json_send(command.dict())
+                self.json_send_explicit(self.connection, command.dict())
                 response = self.special_forms_ops()
                 self.environment_cli_response_stream_handler(response)
             except KeyboardInterrupt:
                 pass # keyboard interrupts mess with the server, dont do it! it wont work anyway, hahahaha
             except WindowsError: # if connection error with the server (there wont be any connection errors)
                 print("[-] Connection was dropped. Exiting")
                 os._exit(0)
```

### Comparing `TapisCL-ICICLE-0.0.4/TapisCLICICLE/commands/apps.py` & `TapisCL-ICICLE-0.0.41/TapisCLICICLE/commands/apps.py`

 * *Files 6% similar despite different names*

```diff
@@ -20,66 +20,66 @@
             'run_app':self.run_job,
             'get_app_status':self.get_job_status,
             'download_app_results':self.download_job_output,
             'help':self.help,
         }
         super().__init__(tapis_instance, username, password, connection=connection, command_map=command_map)
 
-    def create_app(self, file: str, connection=None) -> str: # create a tapis app taking a json descriptor file path
+    async def create_app(self, file: str, connection=None) -> str: # create a tapis app taking a json descriptor file path
         """
         @help: create an app. You must have a properly configured app config file. 
         See a template at https://github.com/sdsc-hpc-training-org/hello_icicle_auth_clients/blob/main/icicle_rel_04_2023/CLI/TapisCL-ICICLE/tapis-config-files/app-config.json
         """
         with open(file, 'r') as f:
             app_def = json.loads(f.read())
         url = self.t.apps.createAppVersion(**app_def)
         return f"App created successfully\nID: {app_def['id']}\nVersion: {app_def['version']}\nURL: {url}\n"
 
-    def get_apps(self, connection=None) -> str:
+    async def get_apps(self, connection=None) -> str:
         """
         @help: get all the apps on a system
         """
         apps = self.t.apps.getApps()
         return str(apps)
 
     @decorators.NeedsConfirmation
-    def delete_app(self, id: str, version: str, connection=None) -> str:
+    async def delete_app(self, id: str, version: str, connection=None) -> str:
         """
         @help: delete the selected app
         """
         return_value = self.t.apps.deleteApp(appId=id, appVersion=version)
         return str(return_value)
 
-    def get_app(self, verbose: bool, id: str, version: str, connection=None)-> None | str: # returns app information with an id and version as arguments
+    async def get_app(self, verbose: bool, id: str, version: str, connection=None)-> None | str: # returns app information with an id and version as arguments
         """
         @help: return selected app information
         """
         app = self.t.apps.getApp(appId=id, appVersion=version)
         if verbose:
             return str(app)
         return None
 
-    def run_job(self, file: str, connection=None)->str: # run a job using an app. Takes a job descriptor json file path
+    async def run_job(self, file: str, connection=None)->str: # run a job using an app. Takes a job descriptor json file path
         """
         @help: run a job from an app on a system. You must have a properly configured job config file. 
         See a template at https://github.com/sdsc-hpc-training-org/hello_icicle_auth_clients/blob/main/icicle_rel_04_2023/CLI/TapisCL-ICICLE/tapis-config-files/job-config.json
         """
         with open(file, 'r') as f:
             app = json.loads(f.read())
         job = self.t.jobs.submitJob(**app)
         return str(job.uuid)
 
-    def get_job_status(self, uuid: str, connection=None)->str: # return a job status with its Uuid
+    async def get_job_status(self, uuid: str, connection=None)->str: # return a job status with its Uuid
         """
         @help: get the status of a job
         """
         job_status = self.t.jobs.getJobStatus(jobUuid=uuid)
         return str(job_status)
 
-    def download_job_output(self, uuid: str, file: str, connection=None)->str: # download the output of a job with its Uuid
+    async def download_job_output(self, uuid: str, file: str, connection=None)->str: # download the output of a job with its Uuid
         """
         @help: download a job output from the system 
         """
         jobs_output = self.t.jobs.getJobOutputDownload(jobUuid=uuid, outputPath='tapisjob.out')
         with open(file, 'w') as f:
             f.write(jobs_output)
         return f"Successfully downloaded job output to {file}"
```

### Comparing `TapisCL-ICICLE-0.0.4/TapisCLICICLE/commands/baseWrappers.py` & `TapisCL-ICICLE-0.0.41/TapisCLICICLE/commands/baseWrappers.py`

 * *Files 1% similar despite different names*

```diff
@@ -33,15 +33,15 @@
             result = command(**kwargs)
             if type(result) == TapisResult:
                 return str(result)
             return result
         except KeyError:
             raise KeyError(f"The command {kwargs['command']} does not exist. See help menu")
     
-    def help(self, name: typing.Optional[str]):
+    async def help(self, name: typing.Optional[str]):
         """
         @help: get help information for the command group
         """
         if name:
             return self.help[name]
         return self.help
```

### Comparing `TapisCL-ICICLE-0.0.4/TapisCLICICLE/commands/files.py` & `TapisCL-ICICLE-0.0.41/TapisCLICICLE/commands/files.py`

 * *Files 4% similar despite different names*

```diff
@@ -16,37 +16,37 @@
             'help':self.help
         }
         super().__init__(tapis_instance, username, password, connection=connection, command_map=command_map)
 
     def return_formatter(self, info):
         return f"name: {info.name}\ngroup: {info.group}\npath: {info.path}\n"
 
-    def list_files(self, verbose: bool, id: str, file: str, connection=None) -> str: # lists files available on a tapis account
+    async def list_files(self, verbose: bool, id: str, file: str, connection=None) -> str: # lists files available on a tapis account
         """
         @help: list the files on a system 
         """
         file_list = self.t.files.listFiles(systemId=id, path=file)
         if verbose:
             return str(file_list)
         file_list = [self.return_formatter(f) for f in file_list]
         return str(file_list)
 
-    def upload(self, file: str, id: str, connection=None) -> str: # upload a file from local to remote using tapis. Takes source and destination paths
+    async def upload(self, file: str, id: str, connection=None) -> str: # upload a file from local to remote using tapis. Takes source and destination paths
         """
         @help: upload a file to the system 
         the source and destination files must both be in the file argument, respectively, separated by a comma
         """
         source = file.split(",")[0]
         destination = file.split(",")[1]
         self.t.upload(system_id=id,
                 source_file_path=source,
                 dest_file_path=destination)
         return f'successfully uploaded {source} to {destination}'
             
-    def download(self, file: str, id: str, connection=None) -> str: # download a remote file using tapis, operates basically the same as upload
+    async def download(self, file: str, id: str, connection=None) -> str: # download a remote file using tapis, operates basically the same as upload
         """
         @help: download a file from the system
         the source and destination files must both be in the file argument, respectively, separated by a comma
         """
         source = file.split(",")[0]
         destination = file.split(",")[1]
         file_info = self.t.files.getContents(systemId=id,
```

### Comparing `TapisCL-ICICLE-0.0.4/TapisCLICICLE/commands/pods.py` & `TapisCL-ICICLE-0.0.41/TapisCLICICLE/commands/pods.py`

 * *Files 10% similar despite different names*

```diff
@@ -27,105 +27,105 @@
                 'help':self.help
             }
         super().__init__(tapis_instance, username, password, connection=connection, command_map=command_map)
 
     def return_formatter(self, info):
         return f"Pod ID: {info.pod_id}\nPod Template: {info.pod_template}\nStatus: {info.status_requested}\n\n"
 
-    def get_pods(self, verbose: bool, connection=None) -> str: 
+    async def get_pods(self, verbose: bool, connection=None) -> str: 
         """
         @help: return a list of pods the current tapis instance has access to
         """
         pods_list = self.t.pods.get_pods()
         if verbose:
             return str(pods_list)
         pods_list = [self.return_formatter(pod) for pod in pods_list]
         pods_string = ""
         for pod in pods_list:
             pods_string += str(pod)
         return pods_string
 
     @decorators.RequiresForm
-    def create_pod(self, id: str, template: str, verbose: bool, description: str | None = None, connection=None) -> str:
+    async def create_pod(self, id: str, template: str, verbose: bool, description: str | None = None, connection=None) -> str:
         """
         @help: create a new pod on the selected Tapis service
         """
         pod_information = self.t.pods.create_pod(pod_id=id, pod_template=template, description=description)
         if verbose:
             return str(pod_information)
         return pod_information
     
-    def start_pod(self, id: str, connection=None):
+    async def start_pod(self, id: str, connection=None):
         """
         @help: start the pod specified with ID
         """
         return_information = self.t.pods.start_pod(pod_id=id)
         return str(return_information)
 
     @decorators.NeedsConfirmation
-    def restart_pod(self, id: str, verbose: bool, connection=None) -> str:
+    async def restart_pod(self, id: str, verbose: bool, connection=None) -> str:
         """
         @help: initiate a pod restart
         """
         return_information = self.t.pods.restart_pod(pod_id=id)
         if verbose:
             return str(return_information)
         return return_information
     
     @decorators.NeedsConfirmation
-    def stop_pod(self, id: str, connection=None):
+    async def stop_pod(self, id: str, connection=None):
         """
         @help: stop a pod's operations
         """
         return_information = self.t.pods.stop_pod(pod_id=id)
         return return_information
         
     @decorators.NeedsConfirmation
-    def delete_pod(self, id: str, verbose: bool, connection=None) -> str: 
+    async def delete_pod(self, id: str, verbose: bool, connection=None) -> str: 
         """
         @help: delete select pod
         """
         return_information = self.t.pods.delete_pod(pod_id=id)
         if verbose:
             return str(return_information)
         return return_information
 
-    def set_pod_perms(self, id: str, username: str, level: str, connection=None) -> str: # set pod permissions, given a pod id, user, and permission level
+    async def set_pod_perms(self, id: str, username: str, level: str, connection=None) -> str: # set pod permissions, given a pod id, user, and permission level
         """
         @help: set the permissions for the pod selected
         """
         return_information = self.t.pods.set_pod_permission(pod_id=id, user=username, level=level)
         return str(return_information)
     
     @decorators.NeedsConfirmation
-    def delete_pod_perms(self, id: str, username: str, connection=None) -> str: # take away someones perms if they are being malicious, or something
+    async def delete_pod_perms(self, id: str, username: str, connection=None) -> str: # take away someones perms if they are being malicious, or something
         """
         @help: delete the selected pod from the pods service you are connected to
         """
         return_information = self.t.pods.delete_pod_perms(pod_id=id, user=username)
         return str(return_information)
 
-    def get_perms(self, id: str, connection=None) -> str: # return a list of permissions on a given pod
+    async def get_perms(self, id: str, connection=None) -> str: # return a list of permissions on a given pod
         """
         @help: get the permissions list for the selected pod
         """
         return_information = self.t.pods.get_pod_permissions(pod_id=id)
         return str(return_information)
 
     @decorators.Auth
-    def copy_pod_password(self, id: str, connection=None) -> str: # copies the pod password to clipboard so that the user can access the pod via the neo4j desktop app. Maybe a security risk? not as bad as printing passwords out!
+    async def copy_pod_password(self, id: str, connection=None) -> str: # copies the pod password to clipboard so that the user can access the pod via the neo4j desktop app. Maybe a security risk? not as bad as printing passwords out!
         """
         @help: copy the pod password to the clipboard
         """
         password = self.t.pods.get_pod_credentials(pod_id=id).user_password
         pyperclip.copy(password)
         password = None
         return 'copied to clipboard'
     
-    def get_pod_logs(self, id: str, file=None, connection=None):
+    async def get_pod_logs(self, id: str, file=None, connection=None):
         """
         @help: retrieve the logs of an active pod and either print them to the console, or write them to the specified file
         """
         logs = self.t.pods.get_pod_logs(pod_id=id)
         if file:
             with open(file, 'w') as f:
                 f.write(logs)
```

### Comparing `TapisCL-ICICLE-0.0.4/TapisCLICICLE/commands/query.py` & `TapisCL-ICICLE-0.0.41/TapisCLICICLE/commands/query.py`

 * *Files 9% similar despite different names*

```diff
@@ -9,30 +9,30 @@
 
 
 class PostgresCLI(baseWrappers.TapisQuery):
     """
     @help: integrated CLI to interface with Postgres pods
     """
     @decorators.RequiresExpression
-    def query(self, id: str, expression: str, connection=None) -> str:
+    async def query(self, id: str, expression: str, connection=None) -> str:
         uname, pword = self.get_credentials(id)
         with psycopg2.connect(f"postgresql://{uname}:{pword}@{id}.pods.{self.t.base_url.split('https://')[1]}:443") as conn:
             conn.autocommit = True
             with conn.cursor() as cur:
                 cur.execute(query=expression)
                 return_value = cur.fetchall()
         return str(f'[+][{id}] {return_value}')
 
 
 class Neo4jCLI(baseWrappers.TapisQuery):
     """
     @help: integrated CLI to interface with Neo4j pods
     """
     @decorators.RequiresExpression
-    def query(self, id: str, expression: str, connection=None) -> str: # function to submit queries to a Neo4j knowledge graph
+    async def query(self, id: str, expression: str, connection=None) -> str: # function to submit queries to a Neo4j knowledge graph
         uname, pword = self.get_credentials(id)
         graph = Graph(f"bolt+ssc://{id}.pods.{self.t.base_url.split('https://')[1]}:443", auth=(uname, pword), secure=True, verify=True)
 
         try:
             return_value = graph.run(expression)
             print(type(return_value))
             if str(return_value) == '(No data)' and 'create' in expression.lower(): # if no data is returned (mostly if something is created) then just say 'success'
```

### Comparing `TapisCL-ICICLE-0.0.4/TapisCLICICLE/commands/serverCommands.py` & `TapisCL-ICICLE-0.0.41/TapisCLICICLE/commands/serverCommands.py`

 * *Files 7% similar despite different names*

```diff
@@ -62,27 +62,28 @@
             'switch_service':self.tapis_init
         }
         help0, help1 = self.help_generation()
         self.help_menu = dict(help0, **help1)
         print(self.help_menu)
 
     @decorators.Auth
-    def tapis_init(self, username: str, password: str, link: str, connection=None) -> tuple[typing.Any, str, str] | None:  # link is the baseURL
+    async def tapis_init(self, username: str, password: str, link: str, connection=None) -> tuple[typing.Any, str, str] | None:  # link is the baseURL
         """
         @help: switch the connected tapis service
         """
         start = time.time()
         self.username = username
         self.password = password
         try:
             t = Tapis(base_url=link,
                     username=username,
                     password=password)
             t.get_tokens()
-        except:
+        except Exception as e:
+            print(e)
             raise exceptions.InvalidCredentialsReceived(function=self.tapis_init, cred_type="Tapis Auth")
 
         self.configure_decorators(self.username, self.password)
         # V3 Headers
         header_dat = {"X-Tapis-token": t.access_token.access_token,
                       "Content-Type": "application/json"}
 
@@ -111,38 +112,38 @@
         self.url = url
         self.access_token = access_token
 
         self.logger.info(f"initiated in {time.time()-start}")
 
         return f"Successfully initialized tapis service on {self.url}"
       
-    def exit(self, connection=None):
+    async def exit(self, connection=None):
         """
         @help: exit the CLI without shutting down the service
         """
         raise exceptions.Exit
     
-    def shutdown(self, connection=None):
+    async def shutdown(self, connection=None):
         """
         @help: exit the CLI and shutdown the service
         """
         self.logger.info("Shutdown initiated")
         raise exceptions.Shutdown
     
-    def help(self, command: str, connection=None):
+    async def help(self, command: str, connection=None):
         """
         @help: returns help information. To get specific help information for tapis services, you can run <service> -c help. enter -c args to see detailed command usage
         """
         if command == "args":
             return args.Args.argparser_args
         elif command in self.help_menu:
             return self.help_menu[command]
         return self.help_menu
     
-    def whoami(self, verbose: bool, connection=None) -> str:
+    async def whoami(self, verbose: bool, connection=None) -> str:
         """
         @help: returns the username of the current user
         """
         user_info = self.t.authenticator.get_userinfo()
         if verbose:
             return str(user_info)
         return user_info.username
```

### Comparing `TapisCL-ICICLE-0.0.4/TapisCLICICLE/commands/systems.py` & `TapisCL-ICICLE-0.0.41/TapisCLICICLE/commands/systems.py`

 * *Files 6% similar despite different names*

```diff
@@ -42,51 +42,51 @@
                 formatted_key = ""
                 for line in f.readlines()[1:-1]:
                     formatted_key += line.strip()
 
             with open(f"{__location__}\\id_rsa", 'w') as f:
                 f.write(formatted_key)
 
-    def get_systems(self, verbose: bool, connection=None):
+    async def get_systems(self, verbose: bool, connection=None):
         """
         @help: Gets and returns the list of systems the current Tapis service and account have access to
         @doc: this is an example of the doc segment of the docstring. not included in help message
         """
         systems = self.t.systems.getSystems()
         if systems and verbose:
             return str(systems)
         systems = [self.return_formatter(system) for system in systems]
         systems_string = ''
         for system in systems:
             systems_string += system
         return systems_string
 
-    def get_system_info(self, verbose: bool, id:str, connection=None): # get information about a system given its ID
+    async def get_system_info(self, verbose: bool, id:str, connection=None): # get information about a system given its ID
         """
         @help: get information on a selected system
         """
         system_info = self.t.systems.getSystem(systemId=id)
         if verbose:
             return str(system_info)
         return self.return_formatter(system_info)
     
-    def create_system(self, file: str, connection=None) -> str: # create a tapius system. Takes a path to a json file with all system information, as well as an ID
+    async def create_system(self, file: str, connection=None) -> str: # create a tapius system. Takes a path to a json file with all system information, as well as an ID
         """
         @help: create a system. Must have a properly configured system file.
         see the template at https://github.com/sdsc-hpc-training-org/hello_icicle_auth_clients/blob/main/icicle_rel_04_2023/CLI/TapisCL-ICICLE/tapis-config-files/system-config.json
         this command will automatically create and upload the ssh keys
         """
         self.__keygen()
         with open(file, 'r') as f:
             system = json.loads(f.read())
         return_value = self.t.systems.createSystem(**system)
         self.system_credential_upload(id=system['id'], file=f"{__location__}\\id_rsa,{__location__}\\id_rsa.pub")
         return str(return_value)
     
-    def system_credential_upload(self, id: str, file: str, connection=None) -> str: # upload key credentials for the system
+    async def system_credential_upload(self, id: str, file: str, connection=None) -> str: # upload key credentials for the system
         """
         @help: upload system credentials to a system. Must generate keys first using 'ssh-keygen -m PEM -f id_rsa', and format with, 'awk -v ORS='\\n' '1' <private_key_name>
         file argument must contain the path to the private and public keys respectively, separated by a ','
         """
         with open(file.split(",")[0], 'r') as f:
             private_key = f.read()
 
@@ -97,26 +97,26 @@
                             userName=self.username,
                             privateKey=private_key,
                             publicKey=public_key)
 
         return str(cred_return_value)
 
     @decorators.SecureInput
-    def system_password_set(self, id: str, password: str, connection=None) -> str: # set the password for a system
+    async def system_password_set(self, id: str, password: str, connection=None) -> str: # set the password for a system
         """
         @help: set a system password
         """
         try:
             password_return_value = self.t.systems.createUserCredential(systemId=id, # will put this in a getpass later
                                 userName=self.username,
                                 password=password)
             return str(password_return_value)
         except Exception as e:
             raise Exception(f"{e}\nTry running set_credentials if the problem persists")
 
     @decorators.NeedsConfirmation
-    def delete_system(self, id: str, connection=None) -> str:
+    async def delete_system(self, id: str, connection=None) -> str:
         """
         @help: delete the selected system
         """
         return_value = self.t.systems.deleteSystem(systemId=id)
         return return_value
```

### Comparing `TapisCL-ICICLE-0.0.4/TapisCLICICLE/utilities/args.py` & `TapisCL-ICICLE-0.0.41/TapisCLICICLE/utilities/args.py`

 * *Files identical despite different names*

### Comparing `TapisCL-ICICLE-0.0.4/TapisCLICICLE/utilities/decorators.py` & `TapisCL-ICICLE-0.0.41/TapisCLICICLE/utilities/decorators.py`

 * *Files 13% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 except:
     import utilities.helpers as helpers
     import utilities.schemas as schemas
     import utilities.socketOpts as socketOpts
     import utilities.exceptions as exceptions
 
 
-class BaseRequirementDecorator(socketOpts.SocketOpts, helpers.OperationsHelper):
+class BaseRequirementDecorator(helpers.OperationsHelper):
     username: typing.Optional[str] = None
     password: typing.Optional[str] = None
     def __init__(self, func: typing.Callable):
         update_wrapper(self, func)
         self.function = func
         self.__code__ = func.__code__
         self.__doc__ = func.__doc__
@@ -45,115 +45,118 @@
 
 class RequiresForm(BaseRequirementDecorator):
     """
     This is for when you want to request separate input for specific command parameters instead of taking directly from the original command input (kwargs)
     Takes the parameters list of the function in question, filters out the ones that were not received from the original request message, sends another message 
     to request the unreceived parameters, and receives a message in response from the client to execute the function
     """
-    def __call__(self, obj, *args, **kwargs):
+    async def __call__(self, obj, *args, **kwargs):
         if kwargs['connection']:
+            connection = kwargs['connection']
             fields = list(helpers.get_parameters(self.function))
             for key, value in kwargs.items():
                 if value or value == False:
                     fields.remove(key)
             if not fields:
                 raise AttributeError(f"The decorated function {self.function} has no parameters.")
             form_request = schemas.FormRequest(arguments_list=fields)
-            self.json_send_explicit(kwargs['connection'], form_request.dict())
-            filled_form: schemas.FormResponse = self.schema_unpack_explicit(kwargs['connection']).arguments_list
+            await connection.send(form_request)
+            filled_form: schemas.FormResponse = await connection.receive().arguments_list
             for key, value in filled_form.items():
                 kwargs[key] = value
 
-        return self.function(obj, **kwargs)
+        return await self.function(obj, **kwargs)
 
 
 class RequiresExpression(BaseRequirementDecorator):
     """
     This is for when you have something like a Neo4j or postgres interface to add to the tapisObjectWrappers file. Writing a Neo4j query directly in a command is cumbersome, its much
     easier to do if you have a blank, multiline environment to write. This will send a request for an expression, if an expression parameter exists in the decorated function.
     The client will open a new interface to type the expression. This is then sent back and fed to the function
     """
-    def __call__(self, obj, *args, **kwargs):
+    async def __call__(self, obj, *args, **kwargs):
         if kwargs['connection']:
+            connection = kwargs['connection']
             fields = list(helpers.get_parameters(self.function))
             if 'expression' not in fields:
                 raise AttributeError(f"The function {self.function} does not contain an 'expression' parameter")
             form_request = schemas.FormRequest(arguments_list=[])
-            self.json_send_explicit(kwargs['connection'], form_request.dict())
-            filled_form: schemas.FormResponse = self.schema_unpack_explicit(connection=kwargs['connection'])
+            await connection.send(form_request)
+            filled_form: schemas.FormResponse = await connection.receive()
             kwargs['expression'] = filled_form.arguments_list
 
-        return self.function(obj, **kwargs)
+        return await self.function(obj, **kwargs)
     
 
 class SecureInput(BaseRequirementDecorator):
     """
     Use this for functions where you need to hide input while typing into the cli. For instance, if you want to add a password to a service, as a user, but you dont actually
     want to authenticate. Checks if the decorated function has a password parameter, then requests secure input of a new password from the client
     """
-    def __call__(self, obj, *args, **kwargs):
+    async def __call__(self, obj, *args, **kwargs):
         if kwargs['connection']:
+            connection = kwargs['connection']
             fields = list(helpers.get_parameters(self.function))
             if 'password' in fields:
                 secure_input_request = schemas.AuthRequest(secure_input=True)
-                self.json_send_explicit(kwargs['connection'], secure_input_request.dict())
-                secure_input_data: schemas.AuthData = self.schema_unpack_explicit(kwargs['connection'])
+                await connection.send(secure_input_request)
+                secure_input_data: schemas.AuthData = await connection.receive()
                 kwargs['password'] = secure_input_data.password
-                return self.function(obj, **kwargs)
+                return await self.function(obj, **kwargs)
             raise AttributeError(f"The function {self.function} does not contain a 'password' parameter to securely input")
-        return self.function(obj, **kwargs)
+        return await self.function(obj, **kwargs)
 
 
 class Auth(BaseRequirementDecorator):
     """
     used for secure authentication from the client. Requires that the function has a username and password parameter for credentials. sends request for credentials from 
     the client, and checks those credentials against the stored credentials in the server.
     """
-    def __call__(self, obj, *args, **kwargs):
+    async def __call__(self, obj, *args, **kwargs):
         no_username = False
         if kwargs['connection']:
+            connection = kwargs['connection']
             if self.function.__name__ == 'tapis_init' and kwargs['username'] and kwargs['password']:
-                return self.function(obj, **kwargs)
+                return await self.function(obj, **kwargs)
             fields = list(helpers.get_parameters(self.function))
             if kwargs['username']:
                 no_username = True
                 auth_request = schemas.AuthRequest(requires_username=False)
             else:
                 auth_request = schemas.AuthRequest()
-            kwargs['connection'].setblocking(True)
-            self.json_send_explicit(kwargs['connection'], auth_request.dict())
-            auth_data: schemas.AuthData = self.schema_unpack_explicit(kwargs['connection'])
-            kwargs['connection'].setblocking(False)
+            await connection.send(auth_request)
+            auth_data: schemas.AuthData = await connection.receive()
             if 'username' in fields and 'password' in fields and not no_username:
                 kwargs['username'], kwargs['password'] = auth_data.username, auth_data.password
-                return self.function(obj, **kwargs)
+                return await self.function(obj, **kwargs)
             elif 'password' in fields and no_username:
                 kwargs['password'] = auth_data.password
             username, password = auth_data.username, auth_data.password
             if username != BaseRequirementDecorator.username:
                 raise exceptions.InvalidCredentialsReceived(self.function, 'username')
             elif password != BaseRequirementDecorator.password:    
                 raise exceptions.InvalidCredentialsReceived(self.function, 'password')
 
-        return self.function(obj, **kwargs)
+        return await self.function(obj, **kwargs)
 
 
 class NeedsConfirmation(BaseRequirementDecorator):
     """
     add to functions that you want user confirmation to exit. If you accidentally enter a command to delete a pod, this will not let you until you confirm
     """
-    def __call__(self, obj, *args, **kwargs):
+    async def __call__(self, obj, *args, **kwargs):
         if kwargs['connection']:
+            connection = kwargs['connection']
             confirmation_request = schemas.ConfirmationRequest(message=f"YOU REQUESTED TO {self.function.__name__}. THIS MIGHT CAUSE DATA LOSS! Please confirm (y/n)")
-            self.json_send_explicit(kwargs['connection'], confirmation_request.dict())
-            confirmation_reply: schemas.ResponseData = self.schema_unpack_explicit(kwargs['connection'])
+            await connection.send(confirmation_request)
+            confirmation_reply: schemas.ResponseData = await connection.receive()
             confirmed = confirmation_reply.response_message
             if not confirmed:
                 raise exceptions.NoConfirmationError(self.function)
-        return self.function(obj, **kwargs)
+        return await self.function(obj, **kwargs)
 
     
 class DecoratorSetup:
     """
     for instantiation of the tapis wrappers, and the server, to set up decorators with user credentials and the socket connection. If you want to use the decorators in your class
     YOU WILL NEED TO USE THIS!
     """
```

### Comparing `TapisCL-ICICLE-0.0.4/TapisCLICICLE/utilities/exceptions.py` & `TapisCL-ICICLE-0.0.41/TapisCLICICLE/utilities/exceptions.py`

 * *Files identical despite different names*

### Comparing `TapisCL-ICICLE-0.0.4/TapisCLICICLE/utilities/helpers.py` & `TapisCL-ICICLE-0.0.41/TapisCLICICLE/utilities/helpers.py`

 * *Files 1% similar despite different names*

```diff
@@ -42,14 +42,15 @@
     to generate helps for each command, iterate over the command map of the selected tapis wrapper object, and generate separate help menu for each
     """
     def __locate_docstring_help(self, func: typing.Callable | object, command_name: str) -> str:
         """
         extract @help from the docstring
         """
         docstring_components = func.__doc__
+        print(func.__doc__)
         if docstring_components:
             docstring_components = docstring_components.split("@")
         else:
             raise exceptions.HelpDoesNotExist(command_name)
         for docstring_component in docstring_components:
             if re.match(r'^[^:]+', docstring_component).group(0) == "help":
                 return docstring_component.split("help: ")[1]
```

### Comparing `TapisCL-ICICLE-0.0.4/TapisCLICICLE/utilities/logger.py` & `TapisCL-ICICLE-0.0.41/TapisCLICICLE/utilities/logger.py`

 * *Files identical despite different names*

### Comparing `TapisCL-ICICLE-0.0.4/TapisCLICICLE/utilities/schemas.py` & `TapisCL-ICICLE-0.0.41/TapisCLICICLE/utilities/schemas.py`

 * *Files identical despite different names*

### Comparing `TapisCL-ICICLE-0.0.4/TapisCL_ICICLE.egg-info/PKG-INFO` & `TapisCL-ICICLE-0.0.41/TapisCL_ICICLE.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: TapisCL-ICICLE
-Version: 0.0.4
+Version: 0.0.41
 Summary: Provide good performance command line user interface for Tapis services hosted on HPC clusters
 Author-email: Michael Ray <ahumanbeing189@gmail.com>
 License:                     GNU GENERAL PUBLIC LICENSE
                                Version 3, 29 June 2007
         
          Copyright (C) 2007 Free Software Foundation, Inc. <https://fsf.org/>
          Everyone is permitted to copy and distribute verbatim copies
```

### Comparing `TapisCL-ICICLE-0.0.4/TapisCL_ICICLE.egg-info/SOURCES.txt` & `TapisCL-ICICLE-0.0.41/TapisCL_ICICLE.egg-info/SOURCES.txt`

 * *Files 5% similar despite different names*

```diff
@@ -16,14 +16,15 @@
 TapisCLICICLE/utilities/__init__.py
 TapisCLICICLE/utilities/args.py
 TapisCLICICLE/utilities/decorators.py
 TapisCLICICLE/utilities/exceptions.py
 TapisCLICICLE/utilities/helpers.py
 TapisCLICICLE/utilities/logger.py
 TapisCLICICLE/utilities/schemas.py
+TapisCLICICLE/utilities/serverConnection.py
 TapisCLICICLE/utilities/socketOpts.py
 TapisCL_ICICLE.egg-info/PKG-INFO
 TapisCL_ICICLE.egg-info/SOURCES.txt
 TapisCL_ICICLE.egg-info/dependency_links.txt
 TapisCL_ICICLE.egg-info/entry_points.txt
 TapisCL_ICICLE.egg-info/requires.txt
 TapisCL_ICICLE.egg-info/top_level.txt
```

### Comparing `TapisCL-ICICLE-0.0.4/pyproject.toml` & `TapisCL-ICICLE-0.0.41/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 [build-system]
 requires      = ["setuptools>=61.0.0", "wheel"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "TapisCL-ICICLE"
-version = "0.0.4"
+version = "0.0.41"
 description = "Provide good performance command line user interface for Tapis services hosted on HPC clusters"
 readme = "README.md"
 authors = [{ name = "Michael Ray", email = "ahumanbeing189@gmail.com" }]
 license = { file = "LICENSE" }
 classifiers = [
     "License :: OSI Approved :: GNU General Public License (GPL)",
     "Programming Language :: Python",
```

