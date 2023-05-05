# Comparing `tmp/convey-1.4.2.tar.gz` & `tmp/convey-1.4.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "convey-1.4.2.tar", last modified: Thu Jan 19 13:30:49 2023, max compression
+gzip compressed data, was "convey-1.4.3.tar", last modified: Fri May  5 08:50:53 2023, max compression
```

## Comparing `convey-1.4.2.tar` & `convey-1.4.3.tar`

### file list

```diff
@@ -1,52 +1,52 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-19 13:30:49.456660 convey-1.4.2/
--rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-01-19 13:30:38.000000 convey-1.4.2/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)       88 2023-01-19 13:30:38.000000 convey-1.4.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)    34551 2023-01-19 13:30:49.456660 convey-1.4.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    34240 2023-01-19 13:30:38.000000 convey-1.4.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-19 13:30:49.456660 convey-1.4.2/convey/
--rw-r--r--   0 runner    (1001) docker     (123)      108 2023-01-19 13:30:38.000000 convey-1.4.2/convey/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4571 2023-01-19 13:30:38.000000 convey-1.4.2/convey/__main__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3363 2023-01-19 13:30:38.000000 convey-1.4.2/convey/action.py
--rw-r--r--   0 runner    (1001) docker     (123)    18940 2023-01-19 13:30:38.000000 convey-1.4.2/convey/action_controller.py
--rw-r--r--   0 runner    (1001) docker     (123)    20014 2023-01-19 13:30:38.000000 convey-1.4.2/convey/args_controller.py
--rw-r--r--   0 runner    (1001) docker     (123)     4766 2023-01-19 13:30:38.000000 convey-1.4.2/convey/attachment.py
--rw-r--r--   0 runner    (1001) docker     (123)    17917 2023-01-19 13:30:38.000000 convey-1.4.2/convey/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     1822 2023-01-19 13:30:38.000000 convey-1.4.2/convey/contacts.py
--rw-r--r--   0 runner    (1001) docker     (123)    41253 2023-01-19 13:30:38.000000 convey-1.4.2/convey/controller.py
--rw-r--r--   0 runner    (1001) docker     (123)     3517 2023-01-19 13:30:38.000000 convey-1.4.2/convey/decorators.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-19 13:30:49.456660 convey-1.4.2/convey/defaults/
--rw-r--r--   0 runner    (1001) docker     (123)    10363 2023-01-19 13:30:38.000000 convey-1.4.2/convey/defaults/config.ini
--rw-r--r--   0 runner    (1001) docker     (123)       18 2023-01-19 13:30:38.000000 convey-1.4.2/convey/defaults/contacts_abroad.csv
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-01-19 13:30:38.000000 convey-1.4.2/convey/defaults/contacts_cc.csv
--rw-r--r--   0 runner    (1001) docker     (123)       62 2023-01-19 13:30:38.000000 convey-1.4.2/convey/defaults/template.eml
--rw-r--r--   0 runner    (1001) docker     (123)       66 2023-01-19 13:30:38.000000 convey-1.4.2/convey/defaults/template_abroad.eml
--rw-r--r--   0 runner    (1001) docker     (123)       70 2023-01-19 13:30:38.000000 convey-1.4.2/convey/defaults/uwsgi.ini
--rw-r--r--   0 runner    (1001) docker     (123)     1610 2023-01-19 13:30:38.000000 convey-1.4.2/convey/definition.py
--rw-r--r--   0 runner    (1001) docker     (123)     7594 2023-01-19 13:30:38.000000 convey-1.4.2/convey/dialogue.py
--rw-r--r--   0 runner    (1001) docker     (123)     8250 2023-01-19 13:30:38.000000 convey-1.4.2/convey/field.py
--rw-r--r--   0 runner    (1001) docker     (123)     1698 2023-01-19 13:30:38.000000 convey-1.4.2/convey/flag.py
--rw-r--r--   0 runner    (1001) docker     (123)     3015 2023-01-19 13:30:38.000000 convey-1.4.2/convey/graph.py
--rw-r--r--   0 runner    (1001) docker     (123)    23254 2023-01-19 13:30:38.000000 convey-1.4.2/convey/identifier.py
--rw-r--r--   0 runner    (1001) docker     (123)    30076 2023-01-19 13:30:38.000000 convey-1.4.2/convey/infodicts.py
--rw-r--r--   0 runner    (1001) docker     (123)    20918 2023-01-19 13:30:38.000000 convey-1.4.2/convey/informer.py
--rw-r--r--   0 runner    (1001) docker     (123)     1149 2023-01-19 13:30:38.000000 convey-1.4.2/convey/ipc.py
--rw-r--r--   0 runner    (1001) docker     (123)    11386 2023-01-19 13:30:38.000000 convey-1.4.2/convey/mail_draft.py
--rw-r--r--   0 runner    (1001) docker     (123)    12560 2023-01-19 13:30:38.000000 convey-1.4.2/convey/mail_sender.py
--rw-r--r--   0 runner    (1001) docker     (123)    40331 2023-01-19 13:30:38.000000 convey-1.4.2/convey/parser.py
--rw-r--r--   0 runner    (1001) docker     (123)    22655 2023-01-19 13:30:38.000000 convey-1.4.2/convey/processor.py
--rw-r--r--   0 runner    (1001) docker     (123)    47827 2023-01-19 13:30:38.000000 convey-1.4.2/convey/types.py
--rw-r--r--   0 runner    (1001) docker     (123)     2379 2023-01-19 13:30:38.000000 convey-1.4.2/convey/utils.py
--rw-r--r--   0 runner    (1001) docker     (123)    20835 2023-01-19 13:30:38.000000 convey-1.4.2/convey/whois.py
--rw-r--r--   0 runner    (1001) docker     (123)    15735 2023-01-19 13:30:38.000000 convey-1.4.2/convey/wizzard.py
--rw-r--r--   0 runner    (1001) docker     (123)    19096 2023-01-19 13:30:38.000000 convey-1.4.2/convey/wrapper.py
--rw-r--r--   0 runner    (1001) docker     (123)     2904 2023-01-19 13:30:38.000000 convey-1.4.2/convey/wsgi.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-01-19 13:30:49.456660 convey-1.4.2/convey.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)    34551 2023-01-19 13:30:49.000000 convey-1.4.2/convey.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      975 2023-01-19 13:30:49.000000 convey-1.4.2/convey.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-01-19 13:30:49.000000 convey-1.4.2/convey.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       48 2023-01-19 13:30:49.000000 convey-1.4.2/convey.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      233 2023-01-19 13:30:49.000000 convey-1.4.2/convey.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-01-19 13:30:49.000000 convey-1.4.2/convey.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      233 2023-01-19 13:30:38.000000 convey-1.4.2/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-01-19 13:30:49.456660 convey-1.4.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      990 2023-01-19 13:30:38.000000 convey-1.4.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 08:50:53.350381 convey-1.4.3/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-05-05 08:50:41.000000 convey-1.4.3/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       88 2023-05-05 08:50:41.000000 convey-1.4.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)    34551 2023-05-05 08:50:53.350381 convey-1.4.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    34240 2023-05-05 08:50:41.000000 convey-1.4.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 08:50:53.346381 convey-1.4.3/convey/
+-rw-r--r--   0 runner    (1001) docker     (123)      108 2023-05-05 08:50:41.000000 convey-1.4.3/convey/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4571 2023-05-05 08:50:41.000000 convey-1.4.3/convey/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3363 2023-05-05 08:50:41.000000 convey-1.4.3/convey/action.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18940 2023-05-05 08:50:41.000000 convey-1.4.3/convey/action_controller.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20014 2023-05-05 08:50:41.000000 convey-1.4.3/convey/args_controller.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4766 2023-05-05 08:50:41.000000 convey-1.4.3/convey/attachment.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17917 2023-05-05 08:50:41.000000 convey-1.4.3/convey/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1822 2023-05-05 08:50:41.000000 convey-1.4.3/convey/contacts.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41253 2023-05-05 08:50:41.000000 convey-1.4.3/convey/controller.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3517 2023-05-05 08:50:41.000000 convey-1.4.3/convey/decorators.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 08:50:53.350381 convey-1.4.3/convey/defaults/
+-rw-r--r--   0 runner    (1001) docker     (123)    10363 2023-05-05 08:50:41.000000 convey-1.4.3/convey/defaults/config.ini
+-rw-r--r--   0 runner    (1001) docker     (123)       18 2023-05-05 08:50:41.000000 convey-1.4.3/convey/defaults/contacts_abroad.csv
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-05-05 08:50:41.000000 convey-1.4.3/convey/defaults/contacts_cc.csv
+-rw-r--r--   0 runner    (1001) docker     (123)       62 2023-05-05 08:50:41.000000 convey-1.4.3/convey/defaults/template.eml
+-rw-r--r--   0 runner    (1001) docker     (123)       66 2023-05-05 08:50:41.000000 convey-1.4.3/convey/defaults/template_abroad.eml
+-rw-r--r--   0 runner    (1001) docker     (123)       70 2023-05-05 08:50:41.000000 convey-1.4.3/convey/defaults/uwsgi.ini
+-rw-r--r--   0 runner    (1001) docker     (123)     1610 2023-05-05 08:50:41.000000 convey-1.4.3/convey/definition.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7594 2023-05-05 08:50:41.000000 convey-1.4.3/convey/dialogue.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8250 2023-05-05 08:50:41.000000 convey-1.4.3/convey/field.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1698 2023-05-05 08:50:41.000000 convey-1.4.3/convey/flag.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3015 2023-05-05 08:50:41.000000 convey-1.4.3/convey/graph.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23254 2023-05-05 08:50:41.000000 convey-1.4.3/convey/identifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30076 2023-05-05 08:50:41.000000 convey-1.4.3/convey/infodicts.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20918 2023-05-05 08:50:41.000000 convey-1.4.3/convey/informer.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1149 2023-05-05 08:50:41.000000 convey-1.4.3/convey/ipc.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11386 2023-05-05 08:50:41.000000 convey-1.4.3/convey/mail_draft.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13819 2023-05-05 08:50:41.000000 convey-1.4.3/convey/mail_sender.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40331 2023-05-05 08:50:41.000000 convey-1.4.3/convey/parser.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22655 2023-05-05 08:50:41.000000 convey-1.4.3/convey/processor.py
+-rw-r--r--   0 runner    (1001) docker     (123)    47827 2023-05-05 08:50:41.000000 convey-1.4.3/convey/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2379 2023-05-05 08:50:41.000000 convey-1.4.3/convey/utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)    20835 2023-05-05 08:50:41.000000 convey-1.4.3/convey/whois.py
+-rw-r--r--   0 runner    (1001) docker     (123)    15735 2023-05-05 08:50:41.000000 convey-1.4.3/convey/wizzard.py
+-rw-r--r--   0 runner    (1001) docker     (123)    19096 2023-05-05 08:50:41.000000 convey-1.4.3/convey/wrapper.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2904 2023-05-05 08:50:41.000000 convey-1.4.3/convey/wsgi.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 08:50:53.346381 convey-1.4.3/convey.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)    34551 2023-05-05 08:50:53.000000 convey-1.4.3/convey.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      975 2023-05-05 08:50:53.000000 convey-1.4.3/convey.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 08:50:53.000000 convey-1.4.3/convey.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       48 2023-05-05 08:50:53.000000 convey-1.4.3/convey.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      233 2023-05-05 08:50:53.000000 convey-1.4.3/convey.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-05-05 08:50:53.000000 convey-1.4.3/convey.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      233 2023-05-05 08:50:41.000000 convey-1.4.3/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-05 08:50:53.350381 convey-1.4.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      990 2023-05-05 08:50:41.000000 convey-1.4.3/setup.py
```

### Comparing `convey-1.4.2/LICENSE.txt` & `convey-1.4.3/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `convey-1.4.2/PKG-INFO` & `convey-1.4.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: convey
-Version: 1.4.2
+Version: 1.4.3
 Summary: CSV processing and mutual conversion of web related data types
 Home-page: https://github.com/CZ-NIC/convey
 Author: Edvard Rejthar
 Author-email: edvard.rejthar@nic.cz
 License: GNU GPLv3
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
```

### Comparing `convey-1.4.2/README.md` & `convey-1.4.3/README.md`

 * *Files identical despite different names*

### Comparing `convey-1.4.2/convey/__main__.py` & `convey-1.4.3/convey/__main__.py`

 * *Files identical despite different names*

### Comparing `convey-1.4.2/convey/action.py` & `convey-1.4.3/convey/action.py`

 * *Files identical despite different names*

### Comparing `convey-1.4.2/convey/action_controller.py` & `convey-1.4.3/convey/action_controller.py`

 * *Files identical despite different names*

### Comparing `convey-1.4.2/convey/args_controller.py` & `convey-1.4.3/convey/args_controller.py`

 * *Files identical despite different names*

### Comparing `convey-1.4.2/convey/attachment.py` & `convey-1.4.3/convey/attachment.py`

 * *Files identical despite different names*

### Comparing `convey-1.4.2/convey/config.py` & `convey-1.4.3/convey/config.py`

 * *Files identical despite different names*

### Comparing `convey-1.4.2/convey/contacts.py` & `convey-1.4.3/convey/contacts.py`

 * *Files identical despite different names*

### Comparing `convey-1.4.2/convey/controller.py` & `convey-1.4.3/convey/controller.py`

 * *Files identical despite different names*

### Comparing `convey-1.4.2/convey/decorators.py` & `convey-1.4.3/convey/decorators.py`

 * *Files identical despite different names*

### Comparing `convey-1.4.2/convey/defaults/config.ini` & `convey-1.4.3/convey/defaults/config.ini`

 * *Files identical despite different names*

### Comparing `convey-1.4.2/convey/definition.py` & `convey-1.4.3/convey/definition.py`

 * *Files identical despite different names*

### Comparing `convey-1.4.2/convey/dialogue.py` & `convey-1.4.3/convey/dialogue.py`

 * *Files identical despite different names*

### Comparing `convey-1.4.2/convey/field.py` & `convey-1.4.3/convey/field.py`

 * *Files identical despite different names*

### Comparing `convey-1.4.2/convey/flag.py` & `convey-1.4.3/convey/flag.py`

 * *Files identical despite different names*

### Comparing `convey-1.4.2/convey/graph.py` & `convey-1.4.3/convey/graph.py`

 * *Files identical despite different names*

### Comparing `convey-1.4.2/convey/identifier.py` & `convey-1.4.3/convey/identifier.py`

 * *Files identical despite different names*

### Comparing `convey-1.4.2/convey/infodicts.py` & `convey-1.4.3/convey/infodicts.py`

 * *Files identical despite different names*

### Comparing `convey-1.4.2/convey/informer.py` & `convey-1.4.3/convey/informer.py`

 * *Files identical despite different names*

### Comparing `convey-1.4.2/convey/ipc.py` & `convey-1.4.3/convey/ipc.py`

 * *Files identical despite different names*

### Comparing `convey-1.4.2/convey/mail_draft.py` & `convey-1.4.3/convey/mail_draft.py`

 * *Files identical despite different names*

### Comparing `convey-1.4.2/convey/mail_sender.py` & `convey-1.4.3/convey/mail_sender.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,13 +1,14 @@
 import logging
 import re
 import smtplib
 import sys
 from abc import abstractmethod, ABC
 from socket import gaierror
+from bs4 import BeautifulSoup
 from requests import get, post
 
 from validate_email import validate_email
 
 from envelope import Envelope
 
 
@@ -32,15 +33,15 @@
         pass
 
     @abstractmethod
     def process(self):
         pass
 
     def send_list(self, mails):
-        """ Send a bunch of e-mail messages 
+        """ Send a bunch of e-mail messages
         :type mails: Union[list, generator]
         """
         sent_mails = 0
         total_count = 0
         status = None
 
         if self.start() is False:
@@ -131,24 +132,43 @@
         # requests_log.setLevel(logging.INFO)
         # requests_log.propagate = True
 
         # upload attachments before the main request
         if attachments:
             # get FormID to pair attachments
             logger.debug("Receiving FormID")
-            form_id_r = get(url,
+            upload_form = get(url,
                             params={"ChallengeToken": self.parser.otrs_token,
                                     "Action": "AgentTicketForward",
                                     "TicketID": str(self.parser.otrs_id)},
                             cookies=cookies
                             )
-
-            m = re.search(r'FormID" value="((\d|\.)*)"', form_id_r.text)
+            m = re.search(r'FormID" value="((\d|\.)*)"', upload_form.text)
             if m:
                 form_id = m[1]
+
+                # Remove the attachment we have been split from (avoid duplicity)
+                if self.parser.source_file:
+                    try:
+                        bs = BeautifulSoup(upload_form.text, features="html.parser")
+                        tr = bs.find('td', {'class': 'Filename'}, lambda tag: tag.string == self.parser.source_file.name).parent
+                        data_file_id = tr.find('a', {'class': 'AttachmentDelete'})['data-file-id']
+                        logger.debug(f"Removing FileID={data_file_id} ({self.parser.source_file.name}) from attachments")
+                        post(url,
+                                params={"Action": "AjaxAttachment",
+                                        "Subaction": "Delete",
+                                        "FormID": form_id,
+                                        "ChallengeToken": self.parser.otrs_token,
+                                        "FileID": data_file_id
+                                        },
+                                cookies=cookies
+                                )
+                    except TypeError:
+                        logger.info(f"Unable to remove ({self.parser.source_file.name}) from attachments")
+
                 for a in attachments:
                     logger.debug("Uploading %s", a.name)
                     post(url,
                          params={"Action": "AjaxAttachment",
                                  "Subaction": "Upload",
                                  "FormID": form_id,
                                  "ChallengeToken": self.parser.otrs_token
```

### Comparing `convey-1.4.2/convey/parser.py` & `convey-1.4.3/convey/parser.py`

 * *Files identical despite different names*

### Comparing `convey-1.4.2/convey/processor.py` & `convey-1.4.3/convey/processor.py`

 * *Files identical despite different names*

### Comparing `convey-1.4.2/convey/types.py` & `convey-1.4.3/convey/types.py`

 * *Files identical despite different names*

### Comparing `convey-1.4.2/convey/utils.py` & `convey-1.4.3/convey/utils.py`

 * *Files identical despite different names*

### Comparing `convey-1.4.2/convey/whois.py` & `convey-1.4.3/convey/whois.py`

 * *Files identical despite different names*

### Comparing `convey-1.4.2/convey/wizzard.py` & `convey-1.4.3/convey/wizzard.py`

 * *Files identical despite different names*

### Comparing `convey-1.4.2/convey/wrapper.py` & `convey-1.4.3/convey/wrapper.py`

 * *Files identical despite different names*

### Comparing `convey-1.4.2/convey/wsgi.py` & `convey-1.4.3/convey/wsgi.py`

 * *Files identical despite different names*

### Comparing `convey-1.4.2/convey.egg-info/PKG-INFO` & `convey-1.4.3/convey.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: convey
-Version: 1.4.2
+Version: 1.4.3
 Summary: CSV processing and mutual conversion of web related data types
 Home-page: https://github.com/CZ-NIC/convey
 Author: Edvard Rejthar
 Author-email: edvard.rejthar@nic.cz
 License: GNU GPLv3
 Description-Content-Type: text/markdown
 License-File: LICENSE.txt
```

### Comparing `convey-1.4.2/convey.egg-info/SOURCES.txt` & `convey-1.4.3/convey.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `convey-1.4.2/setup.py` & `convey-1.4.3/setup.py`

 * *Files identical despite different names*

