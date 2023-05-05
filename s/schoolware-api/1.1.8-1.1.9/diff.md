# Comparing `tmp/schoolware_api-1.1.8.tar.gz` & `tmp/schoolware_api-1.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "schoolware_api-1.1.8.tar", last modified: Fri May  5 13:03:57 2023, max compression
+gzip compressed data, was "schoolware_api-1.1.9.tar", last modified: Fri May  5 13:08:24 2023, max compression
```

## Comparing `schoolware_api-1.1.8.tar` & `schoolware_api-1.1.9.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 13:03:57.605062 schoolware_api-1.1.8/
--rw-r--r--   0 runner    (1001) docker     (123)     1988 2023-05-05 13:03:57.605062 schoolware_api-1.1.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1484 2023-05-05 13:03:46.000000 schoolware_api-1.1.8/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      701 2023-05-05 13:03:46.000000 schoolware_api-1.1.8/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 13:03:57.605062 schoolware_api-1.1.8/schoolware_api/
--rw-r--r--   0 runner    (1001) docker     (123)       30 2023-05-05 13:03:46.000000 schoolware_api-1.1.8/schoolware_api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14303 2023-05-05 13:03:46.000000 schoolware_api-1.1.8/schoolware_api/schoolware_api.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 13:03:57.605062 schoolware_api-1.1.8/schoolware_api.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1988 2023-05-05 13:03:57.000000 schoolware_api-1.1.8/schoolware_api.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      282 2023-05-05 13:03:57.000000 schoolware_api-1.1.8/schoolware_api.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 13:03:57.000000 schoolware_api-1.1.8/schoolware_api.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       53 2023-05-05 13:03:57.000000 schoolware_api-1.1.8/schoolware_api.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-05-05 13:03:57.000000 schoolware_api-1.1.8/schoolware_api.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-05 13:03:57.605062 schoolware_api-1.1.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      392 2023-05-05 13:03:46.000000 schoolware_api-1.1.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 13:08:24.287369 schoolware_api-1.1.9/
+-rw-r--r--   0 runner    (1001) docker     (123)     1988 2023-05-05 13:08:24.287369 schoolware_api-1.1.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1484 2023-05-05 13:08:10.000000 schoolware_api-1.1.9/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      701 2023-05-05 13:08:10.000000 schoolware_api-1.1.9/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 13:08:24.287369 schoolware_api-1.1.9/schoolware_api/
+-rw-r--r--   0 runner    (1001) docker     (123)       30 2023-05-05 13:08:10.000000 schoolware_api-1.1.9/schoolware_api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14418 2023-05-05 13:08:10.000000 schoolware_api-1.1.9/schoolware_api/schoolware_api.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 13:08:24.287369 schoolware_api-1.1.9/schoolware_api.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1988 2023-05-05 13:08:24.000000 schoolware_api-1.1.9/schoolware_api.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      282 2023-05-05 13:08:24.000000 schoolware_api-1.1.9/schoolware_api.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 13:08:24.000000 schoolware_api-1.1.9/schoolware_api.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       53 2023-05-05 13:08:24.000000 schoolware_api-1.1.9/schoolware_api.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-05-05 13:08:24.000000 schoolware_api-1.1.9/schoolware_api.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-05 13:08:24.287369 schoolware_api-1.1.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      392 2023-05-05 13:08:10.000000 schoolware_api-1.1.9/setup.py
```

### Comparing `schoolware_api-1.1.8/PKG-INFO` & `schoolware_api-1.1.9/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: schoolware_api
-Version: 1.1.8
+Version: 1.1.9
 Summary: A api for schoolware written in python
 Author: Maarten Buelens
 Author-email: MB <schoolware_api@mb-server.com>
 License: MIT
 Project-URL: Homepage, https://github.com/Maarten-buelens/schoolware_api
 Project-URL: Bug Tracker, https://github.com/Maarten-buelens/schoolware_api/issues
 Classifier: Programming Language :: Python :: 3
```

### Comparing `schoolware_api-1.1.8/README.md` & `schoolware_api-1.1.9/README.md`

 * *Files identical despite different names*

### Comparing `schoolware_api-1.1.8/pyproject.toml` & `schoolware_api-1.1.9/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61.0"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "schoolware_api"
-version = "1.1.8"
+version = "1.1.9"
 authors = [
   { name="MB", email="schoolware_api@mb-server.com" },
 ]
 description = "A api for schoolware written in python"
 readme = "README.md"
 requires-python = ">=3.7"
 classifiers = [
```

### Comparing `schoolware_api-1.1.8/schoolware_api/schoolware_api.py` & `schoolware_api-1.1.9/schoolware_api/schoolware_api.py`

 * *Files 2% similar despite different names*

```diff
@@ -39,41 +39,41 @@
             logging.basicConfig(format='[%(levelname)s] %(asctime)s - %(message)s', level=logging.INFO)
         if("bg" in config):
             self.bg = config["bg"]
         else:
             self.bg = False
         
         if(self.bg):
-            self.bg_p = threading.Thread(target=bg, args=(self,))
+            self.bg_p = threading.Thread(target=self.bg, args=(self,))
             print("start bg")
             self.bg_p.start()
 
         if("bot_token" in config):
-            self.telegram_bg = threading.Thread(target=telegram_def, args=(self,))
+            self.telegram_bg = threading.Thread(target=self.telegram_def, args=(self,))
             self.telegram_bg.start()
             
         self.domain = self.config["domain"]
         self.user = self.config["user"]
         self.password = self.config["password"]
         self.token = ""
         self.cookie = ""
         self.rooster = []
         self.todo_list = []
         self.scores = []
-        verbose_print(self , message="starting schoolware_api",level=1)        
+        self.verbose_print(self , message="starting schoolware_api",level=1)        
         if(self.verbose):
             print("getting startup token")
         self.check_if_valid()
         self.num_points = len(self.punten())
         self.scores_prev = self.scores
         
 #Token&cookie stuff
     def get_new_token(self):
         ##########VERBOSE##########
-        verbose_print(self,"get_token")
+        self.verbose_print(self,"get_token")
         ##########VERBOSE##########
 
         with sync_playwright() as p:
             browser = p.chromium.launch()
             context = browser.new_context(user_agent="Mozilla/5.0 (Windows NT 10.0; Win64; x64; rv:108.0) Gecko/20100101 Firefox/108.0")
             page = context.new_page()
             page.goto(f"https://{self.domain}/webleerling/start.html#!fn=llagenda")
@@ -84,50 +84,50 @@
             page.get_by_text("Sign In").click()
             page.wait_for_load_state()
             if(context.cookies()[0]["name"] == "FPWebSession"):
                 self.token = context.cookies()[0]["value"]
                 self.cookie = dict(FPWebSession=self.token)
             browser.close()
             ##########VERBOSE##########
-            verbose_end(self,"get_token")
+            self.verbose_end(self,"get_token")
             ##########VERBOSE##########
             return self.token
     
     def check_if_valid(self):
         ##########VERBOSE##########
-        verbose_print(self,"check_token")
+        self.verbose_print(self,"check_token")
         ##########VERBOSE##########
 
         r = requests.get(f"https://{self.domain}/webleerling/bin/server.fcgi/REST/myschoolwareaccount", cookies=self.cookie)
 
 
         if (r.status_code != 200):
             if(r.status_code == 401):
                 ##########VERBOSE##########
-                verbose_end(self,"check_token invalid")
+                self.verbose_end(self,"check_token invalid")
                 ##########VERBOSE##########
                 self.get_new_token()
             else:
-                verbose_end(self,f"check_token error {r.status_code}")
+                self.verbose_end(self,f"check_token error {r.status_code}")
                 raise "error with token"
         else:
             ##########VERBOSE##########
-            verbose_end(self,"check_token")
+            self.verbose_end(self,"check_token")
             ##########VERBOSE##########
             return True
 
 #todo
     def todo(self):
         """gets all todo items from schoolware
 
         Returns:
             list: returns all todo items in a list ordered by descending date
         """
         ##########VERBOSE##########
-        verbose_print(self,"todo")
+        self.verbose_print(self,"todo")
         ##########VERBOSE##########
 
         self.check_if_valid()
         task_data = requests.get(f"https://{self.domain}/webleerling/bin/server.fcgi/REST/AgendaPunt/?_dc=1665240724814&MinVan={date.today()}T00:00:00&IsTaakOfToets=true", cookies=self.cookie).json()["data"]
         self.todo_list = []
 
         for taak in task_data:
@@ -150,27 +150,27 @@
                 "vak": vak,
                 "titel": titel,
                 "onderwerp": onderwerp,
                 "eind_time": eind_time,
                 "day": day
             })
         ##########VERBOSE##########
-        verbose_end(self,"todo")
+        self.verbose_end(self,"todo")
         ##########VERBOSE##########
         return self.todo_list
 
 #punten
     def punten(self):
         """Gets points from the whole year
 
         Returns:
             list: A list containing the points orderd by descending date
         """
         ##########VERBOSE##########
-        verbose_print(self,"punten")
+        self.verbose_print(self,"punten")
         ##########VERBOSE##########
         self.check_if_valid()
         punten_data = requests.get(f"https://{self.domain}/webleerling/bin/server.fcgi/REST/PuntenbladGridLeerling?&Leerling=15201&?BeoordelingMomentVan=1990-09-01+00:00:00", cookies=self.cookie).json()["data"]
         self.scores = []
         for vak in punten_data:
 
             for punt in vak["Beoordelingen"]:
@@ -206,30 +206,30 @@
                     "datum": datum,
                     "pub_datum": publicatie_datum,
                     "day": day,
                     "pub_day": pub_day,
                 })
         self.scores.sort(key=lambda x: datetime.strptime(x['datum'], '%Y-%m-%d %H:%M:%S'), reverse=True)
         ##########VERBOSE##########
-        verbose_end(self,"punten")
+        self.verbose_end(self,"punten")
         ##########VERBOSE##########
         return self.scores
 
 #agenda
     def agenda(self, datum=""):
         """Gets all agenda points of a given date from schoolware
 
         Args:
             datum (str, optional): Date to get agenda for. Defaults to "".
 
         Returns:
             list: returns output from filter_agenda
         """
         ##########VERBOSE##########
-        verbose_print(self,"agenda")
+        self.verbose_print(self,"agenda")
         ##########VERBOSE##########
         self.check_if_valid()
         #begin en einde week
         day = str(date.today())
         dt = datetime.strptime(day, '%Y-%m-%d')
         start = (dt - timedelta(days=dt.weekday())).strftime('%Y-%m-%d')
         if(self.verbose):
@@ -240,30 +240,30 @@
         ####
         agenda_data = requests.get(f"https://kov.schoolware.be/webleerling/bin/server.fcgi/REST/AgendaPunt/?_MaxVan={end}&MinTot={start}", cookies=self.cookie).json()["data"]
         self.rooster = []
         for agenda in agenda_data:
             if(agenda["TypePunt"]==1 or agenda["TypePunt"]==2):
                 self.rooster.append(agenda)
         ##########VERBOSE##########
-        verbose_end(self,"agenda")
+        self.verbose_end(self,"agenda")
         ##########VERBOSE##########
         return self.filter_rooster(self.rooster, datum)
 
     def filter_rooster(self, rooster, datum=""):
         """Internal function to filter a agenda rooster of a given date
 
         Args:
             rooster (list): The agenda points to filter
             datum (str, optional): The date to filter agenda points for. Defaults to "".
 
         Returns:
             list: Filters agenda points for a given date and points
         """
         ##########VERBOSE##########
-        verbose_print(self,"filter_agenda")
+        self.verbose_print(self,"filter_agenda")
         ##########VERBOSE##########
         today = []
         if(datum == ""):
             datum = datetime.today()
         datum = str(datum).split(' ')[0]
         for agenda in rooster:
             if(str(agenda['Van'].split(' ')[0]) == datum):
@@ -294,27 +294,27 @@
                         agenda["skip"] = True
                     elif(today[index+1]["vak"] == today[index+1]["titel"]):
                         today[index+1]["skip"] = True
                         today_filterd.append(agenda)
                 else:
                     today_filterd.append(agenda)
         ##########VERBOSE##########
-        verbose_end(self,"filter-agenda")
+        self.verbose_end(self,"filter-agenda")
         ##########VERBOSE##########
 
         return today_filterd
     
     def telegram_manual_send(self, msg):
         """Manualy send a telegram message
 
         Args:
             msg (String): Message to send
         """
         import asyncio
-        asyncio.run(telegram_send_msg(self, msg))
+        asyncio.run(self.telegram_send_msg(self, msg))
 
     ##########OTHER##########
 
     #bg procces
     def bg(self):
         """Function to keep token valid
         """
@@ -337,16 +337,16 @@
         self.bot = telegram.Bot(self.config["bot_token"])
         
         self.num_prev = len(self.scores)
         self.scores_prev = self.scores
         while True:
             sleep(5*60)
             if(self.verbose):
-                verbose_print(message=f"telegram checking")
-            telegram_point_diff(self)
+                self.verbose_print(message=f"telegram checking")
+            self.telegram_point_diff(self)
 
 
 
     def telegram_point_diff(self):
 
             import asyncio
             scores_now = self.punten()
@@ -356,16 +356,16 @@
                 diff = len(diff_list)
                 self.num_prev = num_now
                 self.scores_prev = scores_now
                 
                 msg = f"{diff} New points for:\n"
                 for item in diff_list:
                     msg = msg + f"{item['vak']}\n"
-                verbose_print(message=f"telegram send msg msg={msg}", level=1)
-                asyncio.run(telegram_send_msg(self, msg))
+                self.verbose_print(message=f"telegram send msg msg={msg}", level=1)
+                asyncio.run(self.telegram_send_msg(self, msg))
 
     async def telegram_send_msg(self, msg):
         """Function to send a telegram message to a set message-id
 
         Args:
             msg (string): the message to send in telegram msg
         """
@@ -382,15 +382,15 @@
         if(self.verbose):
             logging.debug(f"starting {message}")
 
         if(level == 1):
             logging.info(f"{message}")
 
     def verbose_end(self,message):
-        """Ends verbose_print with done and the time for the function
+        """Ends self.verbose_print with done and the time for the function
 
         Args:
             message (string): name of function to display
         """
         if(self.verbose):
             logging.debug(f"Done {message}")
```

### Comparing `schoolware_api-1.1.8/schoolware_api.egg-info/PKG-INFO` & `schoolware_api-1.1.9/schoolware_api.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: schoolware-api
-Version: 1.1.8
+Version: 1.1.9
 Summary: A api for schoolware written in python
 Author: Maarten Buelens
 Author-email: MB <schoolware_api@mb-server.com>
 License: MIT
 Project-URL: Homepage, https://github.com/Maarten-buelens/schoolware_api
 Project-URL: Bug Tracker, https://github.com/Maarten-buelens/schoolware_api/issues
 Classifier: Programming Language :: Python :: 3
```

