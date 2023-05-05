# Comparing `tmp/schoolware_api-1.0.8.tar.gz` & `tmp/schoolware_api-1.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "schoolware_api-1.0.8.tar", last modified: Fri Apr 28 11:10:22 2023, max compression
+gzip compressed data, was "schoolware_api-1.1.0.tar", last modified: Fri May  5 08:11:56 2023, max compression
```

## Comparing `schoolware_api-1.0.8.tar` & `schoolware_api-1.1.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 11:10:22.009314 schoolware_api-1.0.8/
--rw-r--r--   0 runner    (1001) docker     (123)     1988 2023-04-28 11:10:22.009314 schoolware_api-1.0.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1484 2023-04-28 11:10:06.000000 schoolware_api-1.0.8/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      700 2023-04-28 11:10:06.000000 schoolware_api-1.0.8/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 11:10:22.005313 schoolware_api-1.0.8/schoolware_api/
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-04-28 11:10:06.000000 schoolware_api-1.0.8/schoolware_api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    12852 2023-04-28 11:10:06.000000 schoolware_api-1.0.8/schoolware_api/schoolware_api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-28 11:10:22.009314 schoolware_api-1.0.8/schoolware_api.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1988 2023-04-28 11:10:22.000000 schoolware_api-1.0.8/schoolware_api.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      282 2023-04-28 11:10:22.000000 schoolware_api-1.0.8/schoolware_api.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-28 11:10:22.000000 schoolware_api-1.0.8/schoolware_api.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-04-28 11:10:22.000000 schoolware_api-1.0.8/schoolware_api.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-04-28 11:10:22.000000 schoolware_api-1.0.8/schoolware_api.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-28 11:10:22.009314 schoolware_api-1.0.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      391 2023-04-28 11:10:06.000000 schoolware_api-1.0.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 08:11:56.608121 schoolware_api-1.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1988 2023-05-05 08:11:56.608121 schoolware_api-1.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1484 2023-05-05 08:11:42.000000 schoolware_api-1.1.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      701 2023-05-05 08:11:42.000000 schoolware_api-1.1.0/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 08:11:56.608121 schoolware_api-1.1.0/schoolware_api/
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-05-05 08:11:42.000000 schoolware_api-1.1.0/schoolware_api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13606 2023-05-05 08:11:42.000000 schoolware_api-1.1.0/schoolware_api/schoolware_api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 08:11:56.608121 schoolware_api-1.1.0/schoolware_api.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1988 2023-05-05 08:11:56.000000 schoolware_api-1.1.0/schoolware_api.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      282 2023-05-05 08:11:56.000000 schoolware_api-1.1.0/schoolware_api.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 08:11:56.000000 schoolware_api-1.1.0/schoolware_api.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-05-05 08:11:56.000000 schoolware_api-1.1.0/schoolware_api.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-05-05 08:11:56.000000 schoolware_api-1.1.0/schoolware_api.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-05 08:11:56.608121 schoolware_api-1.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      392 2023-05-05 08:11:42.000000 schoolware_api-1.1.0/setup.py
```

### Comparing `schoolware_api-1.0.8/PKG-INFO` & `schoolware_api-1.1.0/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: schoolware_api
-Version: 1.0.8
+Version: 1.1.0
 Summary: A api for schoolware written in python
 Author: Maarten Buelens
 Author-email: MB <schoolware_api@mb-server.com>
 License: MIT
 Project-URL: Homepage, https://github.com/Maarten-buelens/schoolware_api
 Project-URL: Bug Tracker, https://github.com/Maarten-buelens/schoolware_api/issues
 Classifier: Programming Language :: Python :: 3
```

### Comparing `schoolware_api-1.0.8/README.md` & `schoolware_api-1.1.0/README.md`

 * *Files identical despite different names*

### Comparing `schoolware_api-1.0.8/pyproject.toml` & `schoolware_api-1.1.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "schoolware_api"
-version = "1.0.8"
+version = "1.1.0"
 authors = [
   { name="MB", email="schoolware_api@mb-server.com" },
 ]
 description = "A api for schoolware written in python"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
@@ -19,8 +19,8 @@
 dependencies = [
   'requests>=2.25.1',
   'playwright>=1.31.1',
   'termcolor>=2.2.0'
 ]
 [project.urls]
 "Homepage" = "https://github.com/Maarten-buelens/schoolware_api"
-"Bug Tracker" = "https://github.com/Maarten-buelens/schoolware_api/issues"
+"Bug Tracker" = "https://github.com/Maarten-buelens/schoolware_api/issues"
```

### Comparing `schoolware_api-1.0.8/schoolware_api/schoolware_api.py` & `schoolware_api-1.1.0/schoolware_api/schoolware_api.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,15 @@
 import requests
 from datetime import date, datetime, timedelta
 from playwright.sync_api import sync_playwright
 import time
 from termcolor import colored
 import threading
+import logging
+
 class schoolware:
 
     def __init__(self, config) -> None:
         """Pass config dict to init class
         Args:
         | Key | Description |
         | --- | --- |
@@ -15,14 +17,15 @@
         | user | school microsoft email
         | password | school microsoft password
         | bg | background procces to keep token valid
         | bot_token | telegram bot token to enable telegram bot
         | chat_id | id to send messages to
         | verbose | show a lot more info
         """
+#        verbose_print(self , message="starting schoolware_api",level="info")
         self.config = config
         if("debug" in config):
             self.verbose = config["debug"]
         else:
             self.verbose = False
         if("verbose" in config):
             self.verbose = config["verbose"]
@@ -46,18 +49,20 @@
         self.user = self.config["user"]
         self.password = self.config["password"]
         self.token = ""
         self.cookie = ""
         self.rooster = []
         self.todo_list = []
         self.scores = []
+	verbose_print(self , message="starting schoolware_api",level="info")        
         if(self.verbose):
             print("getting startup token")
         self.check_if_valid()
         self.num_points = len(self.punten())
+        self.scores_prev = self.scores
         
 #Token&cookie stuff
     def get_new_token(self):
         ##########VERBOSE##########
         verbose_print(self,"get_token")
         ##########VERBOSE##########
 
@@ -105,15 +110,15 @@
             return True
 
 #todo
     def todo(self):
         """gets all todo items from schoolware
 
         Returns:
-            list: returns all todo items in a list
+            list: returns all todo items in a list ordered by descending date
         """
         ##########VERBOSE##########
         verbose_print(self,"todo")
         ##########VERBOSE##########
 
         self.check_if_valid()
         task_data = requests.get(f"https://{self.domain}/webleerling/bin/server.fcgi/REST/AgendaPunt/?_dc=1665240724814&MinVan={date.today()}T00:00:00&IsTaakOfToets=true", cookies=self.cookie).json()["data"]
@@ -148,15 +153,15 @@
         return self.todo_list
 
 #punten
     def punten(self):
         """Gets points from the whole year
 
         Returns:
-            list: A list containing the points orderd by date
+            list: A list containing the points orderd by descending date
         """
         ##########VERBOSE##########
         verbose_print(self,"punten")
         ##########VERBOSE##########
         self.check_if_valid()
         punten_data = requests.get(f"https://{self.domain}/webleerling/bin/server.fcgi/REST/PuntenbladGridLeerling?&Leerling=15201&?BeoordelingMomentVan=1990-09-01+00:00:00", cookies=self.cookie).json()["data"]
         self.scores = []
@@ -172,14 +177,17 @@
                 except:
                     behaalde_score = "n/a"
                 publicatie_datum = punt["BeoordelingMomentPublicatieDatum"]
                 datum = punt["BeoordelingMomentDatum"]
                 titel = punt["BeoordelingMomentOmschrijving"]
                 dt = datetime.strptime(punt["BeoordelingMomentDatum"].split(' ')[0], '%Y-%m-%d')
                 day = dt.strftime('%A')
+
+                pub_dt = datetime.strptime(punt["BeoordelingMomentPublicatieDatum"].split(' ')[0], '%Y-%m-%d')
+                pub_day = pub_dt.strftime('%A')
                 if(punt["BeoordelingMomentType_"] == "bmtToets"):
                     soort = "toets"
                 else:
                     soort = "taak"
 
                 self.scores.append({
                     "soort": soort,
@@ -187,15 +195,16 @@
                     "titel": titel,
                     "DW": DW,
                     "tot_sc": totale_score,
                     "gew_sc": gewenste_score,
                     "score": behaalde_score,
                     "datum": datum,
                     "pub_datum": publicatie_datum,
-                    "day": day
+                    "day": day,
+                    "pub_day": pub_day,
                 })
         self.scores.sort(key=lambda x: datetime.strptime(x['datum'], '%Y-%m-%d %H:%M:%S'), reverse=True)
         ##########VERBOSE##########
         verbose_end(self,"punten")
         ##########VERBOSE##########
         return self.scores
 
@@ -206,15 +215,15 @@
         Args:
             datum (str, optional): Date to get agenda for. Defaults to "".
 
         Returns:
             list: returns output from filter_agenda
         """
         ##########VERBOSE##########
-        verbose_print(self,"_agenda")
+        verbose_print(self,"agenda")
         ##########VERBOSE##########
         self.check_if_valid()
         #begin en einde week
         day = str(date.today())
         dt = datetime.strptime(day, '%Y-%m-%d')
         start = (dt - timedelta(days=dt.weekday())).strftime('%Y-%m-%d')
         if(self.verbose):
@@ -283,14 +292,23 @@
                 else:
                     today_filterd.append(agenda)
         ##########VERBOSE##########
         verbose_end(self,"filter-agenda")
         ##########VERBOSE##########
 
         return today_filterd
+    
+    def telegram_manual_send(self, msg):
+        """Manualy send a telegram message
+
+        Args:
+            msg (String): Message to send
+        """
+        import asyncio
+        asyncio.run(telegram_send_msg(self, msg))
 
 ##########OTHER##########
 
 #bg procces
 def bg(self):
     """Function to keep token valid
     """
@@ -305,54 +323,60 @@
 #telegram bot
 def telegram_def(self):
     """The setup function for Telegram
     """
     import telegram
     from time import sleep
     import asyncio
-    if(self.verbose):
-        self.bot = telegram.Bot(self.config["bot_token"])
+    
+    self.bot = telegram.Bot(self.config["bot_token"])
     print(colored("telegram started","blue"))
     while True:
         sleep(5*60)
         if(self.verbose):
             print(colored("telegram checking","blue"))
-        num_now = len(self.punten())
-        if(self.num_points < num_now):
-            diff = num_now - self.num_points
-            self.num_points = num_now
+        scores_now = self.punten()
+        num_now = len(scores_now)
+        if(num_prev < num_now):
+            diff_list = [i for i in scores_now if i not in scores_prev]
+            diff = len(diff_list)
+            num_prev = num_now
+            scores_prev = scores_now
             
-            asyncio.run(telegram_send_msg(self, diff))
+            msg = f"{diff} New points for:\n"
+            for item in diff_list:
+                msg = msg + f"{item['vak']}\n"
+            verbose_print(message=f"telegram send msg msg={msg}", level="info")
+            asyncio.run(telegram_send_msg(self, msg))
 
-async def telegram_send_msg(self, diff):
+async def telegram_send_msg(self, msg):
     """Function to send a telegram message to a set message-id
 
     Args:
-        diff (int): the number to display in the message
+        msg (string): the message to send in telegram msg
     """
     async with self.bot:
-        await self.bot.send_message(text=f'{diff} New point(s)', chat_id=self.config["chat_id"])
+        await self.bot.send_message(text=msg, chat_id=self.config["chat_id"])
 
 ##########VERBOSE##########
-def verbose_print(self,message):
+def verbose_print(self,message, level="debug"):
     """To print a message when verbose is set also times function
 
     Args:
         message (string): name of function to display
     """
     if(self.verbose):
-        print(colored("#"*50, "grey"))
-        self.start_time = time.time()
-        print(colored(f"• starting {message}", "green"))
-        print(colored("#"*50, "grey"))
+        logging.debug(f"starting {message}")
+
+    if(level == "info"):
+        logging.info(f"{message}")
+
 def verbose_end(self,message):
     """Ends verbose_print with done and the time for the function
 
     Args:
         message (string): name of function to display
     """
     if(self.verbose):
-        print(colored("#"*50, "grey"))
-        end_time = time.time()
-        print(colored(f"• Done {message} time:{end_time - self.start_time}", "green"))
-        print(colored("#"*50, "grey"))
+        logging.debug(f"Done {message}")
+
 ##########VERBOSE##########
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `schoolware_api-1.0.8/schoolware_api.egg-info/PKG-INFO` & `schoolware_api-1.1.0/schoolware_api.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: schoolware-api
-Version: 1.0.8
+Version: 1.1.0
 Summary: A api for schoolware written in python
 Author: Maarten Buelens
 Author-email: MB <schoolware_api@mb-server.com>
 License: MIT
 Project-URL: Homepage, https://github.com/Maarten-buelens/schoolware_api
 Project-URL: Bug Tracker, https://github.com/Maarten-buelens/schoolware_api/issues
 Classifier: Programming Language :: Python :: 3
```

