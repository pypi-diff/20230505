# Comparing `tmp/emailnator-0.1.0.tar.gz` & `tmp/emailnator-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "emailnator-0.1.0.tar", last modified: Fri May  5 15:28:56 2023, max compression
+gzip compressed data, was "emailnator-0.1.1.tar", last modified: Fri May  5 15:58:28 2023, max compression
```

## Comparing `emailnator-0.1.0.tar` & `emailnator-0.1.1.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 15:28:56.076625 emailnator-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)     3505 2023-05-05 15:28:56.076625 emailnator-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3189 2023-05-05 15:28:38.000000 emailnator-0.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 15:28:56.076625 emailnator-0.1.0/emailnator/
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-05-05 15:28:38.000000 emailnator-0.1.0/emailnator/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5396 2023-05-05 15:28:38.000000 emailnator-0.1.0/emailnator/emailnator.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 15:28:56.076625 emailnator-0.1.0/emailnator.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3505 2023-05-05 15:28:56.000000 emailnator-0.1.0/emailnator.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      235 2023-05-05 15:28:56.000000 emailnator-0.1.0/emailnator.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 15:28:56.000000 emailnator-0.1.0/emailnator.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-05 15:28:56.000000 emailnator-0.1.0/emailnator.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-05 15:28:56.000000 emailnator-0.1.0/emailnator.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-05 15:28:56.076625 emailnator-0.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      772 2023-05-05 15:28:38.000000 emailnator-0.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 15:58:28.008745 emailnator-0.1.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     3505 2023-05-05 15:58:28.008745 emailnator-0.1.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3189 2023-05-05 15:58:16.000000 emailnator-0.1.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 15:58:28.008745 emailnator-0.1.1/emailnator/
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-05-05 15:58:16.000000 emailnator-0.1.1/emailnator/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6109 2023-05-05 15:58:16.000000 emailnator-0.1.1/emailnator/emailnator.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-05 15:58:28.008745 emailnator-0.1.1/emailnator.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3505 2023-05-05 15:58:28.000000 emailnator-0.1.1/emailnator.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      235 2023-05-05 15:58:28.000000 emailnator-0.1.1/emailnator.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-05 15:58:28.000000 emailnator-0.1.1/emailnator.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-05-05 15:58:28.000000 emailnator-0.1.1/emailnator.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       11 2023-05-05 15:58:28.000000 emailnator-0.1.1/emailnator.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-05-05 15:58:28.008745 emailnator-0.1.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      772 2023-05-05 15:58:16.000000 emailnator-0.1.1/setup.py
```

### Comparing `emailnator-0.1.0/PKG-INFO` & `emailnator-0.1.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: emailnator
-Version: 0.1.0
+Version: 0.1.1
 Summary: A Python wrapper for the Emailnator temporary email service.
 Home-page: https://github.com/repollo/emailnator
 Author: repollo
 Author-email: repollo.marrero@gmail.com
 Keywords: emailnator wrapper temporary email
 Description-Content-Type: text/markdown
```

### Comparing `emailnator-0.1.0/README.md` & `emailnator-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `emailnator-0.1.0/emailnator/emailnator.py` & `emailnator-0.1.1/emailnator/emailnator.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 import os
+import random
 from dotenv import load_dotenv, set_key
 from urllib.parse import unquote
 import requests
 
 
 class EmailnatorError(Exception):
     pass
@@ -106,52 +107,72 @@
         Raises:
             EmailnatorError: If the response status code is not 200.
         """
         if response.status_code != 200:
             raise EmailnatorError(f"Error: {response.status_code}: {response.text}")
         return response.json()
 
-    def generate_email(self, options=["dotGmail"]):
+    def generate_email(self, options=None):
         """
         Generate Email
         
         options (Array): ["domain", "plusGmail", "dotGmail"]
         """
+        
+        valid_options = ["domain", "plusGmail", "dotGmail"]
+        
+        if options is None:
+            options = [random.choice(valid_options)]
+        else:
+            if not all(option in valid_options for option in options):
+                raise EmailnatorError("Invalid input: options should be a list containing valid option strings.")
+
+
         url = f"{self.base_url}/generate-email"
         payload = {"email": options}
         response = requests.post(url, json=payload, headers=self.headers)
         json_data = self._handle_response(response)
 
         self.email = json_data["email"][0]
         self.env_manager.set("EMAIL", self.email)
 
         return json_data
 
     def inbox(self, email):
         """
         Retrieve Inbox
-        
+
         email: Email address
         """
+        if not isinstance(email, str):
+            raise EmailnatorError("Invalid input: email should be a string.")
+
         url = f"{self.base_url}/message-list"
-        payload = { "email": email }
+        payload = {"email": email}
         response = requests.post(url, json=payload, headers=self.headers)
         return self._handle_response(response)
 
     def get_message(self, email, message_id):
         """
         Get Message
-        
+
         email: Email address
         message_id: Message ID
         """
+        if not isinstance(email, str):
+            raise EmailnatorError("Invalid input: email should be a string.")
+
+        if not isinstance(message_id, str):
+            raise EmailnatorError("Invalid input: message_id should be a string.")
+
         url = f"{self.base_url}/message-list"
         payload = {"email": email, "messageID": message_id}
         response = requests.post(url, json=payload, headers=self.headers)
         return response.text
+
     
     def get_existing_email(self):
         """
         Get the existing generated email from the .env file, if available.
 
         Returns:
             str: The existing email, or None if no email exists in the .env file.
```

### Comparing `emailnator-0.1.0/emailnator.egg-info/PKG-INFO` & `emailnator-0.1.1/emailnator.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: emailnator
-Version: 0.1.0
+Version: 0.1.1
 Summary: A Python wrapper for the Emailnator temporary email service.
 Home-page: https://github.com/repollo/emailnator
 Author: repollo
 Author-email: repollo.marrero@gmail.com
 Keywords: emailnator wrapper temporary email
 Description-Content-Type: text/markdown
```

### Comparing `emailnator-0.1.0/setup.py` & `emailnator-0.1.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 # Read the contents of README.md
 this_directory = path.abspath(path.dirname(__file__))
 with open(path.join(this_directory, "README.md"), encoding="utf-8") as f:
     long_description = f.read()
 
 setup(
     name="emailnator",
-    version="0.1.0",
+    version="0.1.1",
     packages=find_packages(),
     install_requires=[
         "requests",
         "python-dotenv",
     ],
     author="repollo",
     author_email="repollo.marrero@gmail.com",
```

