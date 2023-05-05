# Comparing `tmp/schoolware_api-1.1.7.tar.gz` & `tmp/schoolware_api-1.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "schoolware_api-1.1.7.tar", last modified: Fri May  5 11:44:39 2023, max compression
+gzip compressed data, was "schoolware_api-1.1.8.tar", last modified: Fri May  5 13:03:57 2023, max compression
```

## Comparing `schoolware_api-1.1.7.tar` & `schoolware_api-1.1.8.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 11:44:39.646146 schoolware_api-1.1.7/
--rw-r--r--   0 runner    (1001) docker     (123)     1988 2023-05-05 11:44:39.646146 schoolware_api-1.1.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1484 2023-05-05 11:44:27.000000 schoolware_api-1.1.7/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      701 2023-05-05 11:44:27.000000 schoolware_api-1.1.7/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 11:44:39.646146 schoolware_api-1.1.7/schoolware_api/
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-05-05 11:44:27.000000 schoolware_api-1.1.7/schoolware_api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    13976 2023-05-05 11:44:27.000000 schoolware_api-1.1.7/schoolware_api/schoolware_api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 11:44:39.646146 schoolware_api-1.1.7/schoolware_api.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1988 2023-05-05 11:44:39.000000 schoolware_api-1.1.7/schoolware_api.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      282 2023-05-05 11:44:39.000000 schoolware_api-1.1.7/schoolware_api.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 11:44:39.000000 schoolware_api-1.1.7/schoolware_api.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-05-05 11:44:39.000000 schoolware_api-1.1.7/schoolware_api.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-05-05 11:44:39.000000 schoolware_api-1.1.7/schoolware_api.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-05 11:44:39.646146 schoolware_api-1.1.7/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      392 2023-05-05 11:44:27.000000 schoolware_api-1.1.7/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 13:03:57.605062 schoolware_api-1.1.8/
+-rw-r--r--   0 runner    (1001) docker     (123)     1988 2023-05-05 13:03:57.605062 schoolware_api-1.1.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1484 2023-05-05 13:03:46.000000 schoolware_api-1.1.8/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      701 2023-05-05 13:03:46.000000 schoolware_api-1.1.8/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 13:03:57.605062 schoolware_api-1.1.8/schoolware_api/
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-05-05 13:03:46.000000 schoolware_api-1.1.8/schoolware_api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14303 2023-05-05 13:03:46.000000 schoolware_api-1.1.8/schoolware_api/schoolware_api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 13:03:57.605062 schoolware_api-1.1.8/schoolware_api.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1988 2023-05-05 13:03:57.000000 schoolware_api-1.1.8/schoolware_api.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      282 2023-05-05 13:03:57.000000 schoolware_api-1.1.8/schoolware_api.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 13:03:57.000000 schoolware_api-1.1.8/schoolware_api.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-05-05 13:03:57.000000 schoolware_api-1.1.8/schoolware_api.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-05-05 13:03:57.000000 schoolware_api-1.1.8/schoolware_api.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-05 13:03:57.605062 schoolware_api-1.1.8/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      392 2023-05-05 13:03:46.000000 schoolware_api-1.1.8/setup.py
```

### Comparing `schoolware_api-1.1.7/PKG-INFO` & `schoolware_api-1.1.8/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: schoolware_api
-Version: 1.1.7
+Version: 1.1.8
 Summary: A api for schoolware written in python
 Author: Maarten Buelens
 Author-email: MB <schoolware_api@mb-server.com>
 License: MIT
 Project-URL: Homepage, https://github.com/Maarten-buelens/schoolware_api
 Project-URL: Bug Tracker, https://github.com/Maarten-buelens/schoolware_api/issues
 Classifier: Programming Language :: Python :: 3
```

### Comparing `schoolware_api-1.1.7/README.md` & `schoolware_api-1.1.8/README.md`

 * *Files identical despite different names*

### Comparing `schoolware_api-1.1.7/pyproject.toml` & `schoolware_api-1.1.8/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "schoolware_api"
-version = "1.1.7"
+version = "1.1.8"
 authors = [
   { name="MB", email="schoolware_api@mb-server.com" },
 ]
 description = "A api for schoolware written in python"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `schoolware_api-1.1.7/schoolware_api/schoolware_api.py` & `schoolware_api-1.1.8/schoolware_api/schoolware_api.py`

 * *Files 5% similar despite different names*

```diff
@@ -308,83 +308,90 @@
 
         Args:
             msg (String): Message to send
         """
         import asyncio
         asyncio.run(telegram_send_msg(self, msg))
 
-##########OTHER##########
+    ##########OTHER##########
 
-#bg procces
-def bg(self):
-    """Function to keep token valid
-    """
-    from time import sleep
-    if(self.verbose):
-        print(colored("background procces started","blue"))
-    while True:
-        sleep(5*60)
+    #bg procces
+    def bg(self):
+        """Function to keep token valid
+        """
+        from time import sleep
         if(self.verbose):
-            print(colored("background task: checking token","blue"))
-        self.check_if_valid()
-#telegram bot
-def telegram_def(self):
-    """The setup function for Telegram
-    """
-    import telegram
-    from time import sleep
-    import asyncio
-    
-    self.bot = telegram.Bot(self.config["bot_token"])
-    print(colored("telegram started","blue"))
-    num_prev = len(self.scores)
-    scores_prev = self.scores
-    while True:
-        sleep(5*60)
+            print(colored("background procces started","blue"))
+        while True:
+            sleep(5*60)
+            if(self.verbose):
+                print(colored("background task: checking token","blue"))
+            self.check_if_valid()
+    #telegram bot
+    def telegram_def(self):
+        """The setup function for Telegram
+        """
+        import telegram
+        from time import sleep
+        
+        
+        self.bot = telegram.Bot(self.config["bot_token"])
+        
+        self.num_prev = len(self.scores)
+        self.scores_prev = self.scores
+        while True:
+            sleep(5*60)
+            if(self.verbose):
+                verbose_print(message=f"telegram checking")
+            telegram_point_diff(self)
+
+
+
+    def telegram_point_diff(self):
+
+            import asyncio
+            scores_now = self.punten()
+            num_now = len(scores_now)
+            if(self.num_prev < num_now):
+                diff_list = [i for i in scores_now if i not in self.scores_prev]
+                diff = len(diff_list)
+                self.num_prev = num_now
+                self.scores_prev = scores_now
+                
+                msg = f"{diff} New points for:\n"
+                for item in diff_list:
+                    msg = msg + f"{item['vak']}\n"
+                verbose_print(message=f"telegram send msg msg={msg}", level=1)
+                asyncio.run(telegram_send_msg(self, msg))
+
+    async def telegram_send_msg(self, msg):
+        """Function to send a telegram message to a set message-id
+
+        Args:
+            msg (string): the message to send in telegram msg
+        """
+        async with self.bot:
+            await self.bot.send_message(text=msg, chat_id=self.config["chat_id"])
+
+    ##########VERBOSE##########
+    def verbose_print(self,message, level=0):
+        """To print a message when verbose is set also times function
+
+        Args:
+            message (string): name of function to display
+        """
+        if(self.verbose):
+            logging.debug(f"starting {message}")
+
+        if(level == 1):
+            logging.info(f"{message}")
+
+    def verbose_end(self,message):
+        """Ends verbose_print with done and the time for the function
+
+        Args:
+            message (string): name of function to display
+        """
         if(self.verbose):
-            verbose_print(message=f"telegram checking", level="debug")
-        scores_now = self.punten()
-        num_now = len(scores_now)
-        if(num_prev < num_now):
-            diff_list = [i for i in scores_now if i not in scores_prev]
-            diff = len(diff_list)
-            num_prev = num_now
-            scores_prev = scores_now
-            
-            msg = f"{diff} New points for:\n"
-            for item in diff_list:
-                msg = msg + f"{item['vak']}\n"
-            verbose_print(message=f"telegram send msg msg={msg}", level="info")
-            asyncio.run(telegram_send_msg(self, msg))
-
-async def telegram_send_msg(self, msg):
-    """Function to send a telegram message to a set message-id
-
-    Args:
-        msg (string): the message to send in telegram msg
-    """
-    async with self.bot:
-        await self.bot.send_message(text=msg, chat_id=self.config["chat_id"])
-
-##########VERBOSE##########
-def verbose_print(self,message, level=0):
-    """To print a message when verbose is set also times function
-
-    Args:
-        message (string): name of function to display
-    """
-    if(self.verbose):
-        logging.debug(f"starting {message}")
-
-    if(level == 1):
-        logging.info(f"{message}")
-
-def verbose_end(self,message):
-    """Ends verbose_print with done and the time for the function
-
-    Args:
-        message (string): name of function to display
-    """
-    if(self.verbose):
-        logging.debug(f"Done {message}")
+            logging.debug(f"Done {message}")
 
-##########VERBOSE##########
+    ##########VERBOSE##########
```

### Comparing `schoolware_api-1.1.7/schoolware_api.egg-info/PKG-INFO` & `schoolware_api-1.1.8/schoolware_api.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: schoolware-api
-Version: 1.1.7
+Version: 1.1.8
 Summary: A api for schoolware written in python
 Author: Maarten Buelens
 Author-email: MB <schoolware_api@mb-server.com>
 License: MIT
 Project-URL: Homepage, https://github.com/Maarten-buelens/schoolware_api
 Project-URL: Bug Tracker, https://github.com/Maarten-buelens/schoolware_api/issues
 Classifier: Programming Language :: Python :: 3
```

