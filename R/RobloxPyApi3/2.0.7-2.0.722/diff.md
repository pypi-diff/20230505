# Comparing `tmp/RobloxPyApi3-2.0.7.tar.gz` & `tmp/RobloxPyApi3-2.0.722.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "RobloxPyApi3-2.0.7.tar", last modified: Fri May  5 19:41:03 2023, max compression
+gzip compressed data, was "RobloxPyApi3-2.0.722.tar", last modified: Fri May  5 19:55:00 2023, max compression
```

## Comparing `RobloxPyApi3-2.0.7.tar` & `RobloxPyApi3-2.0.722.tar`

### file list

```diff
@@ -1,40 +1,40 @@
-drwxrwxrwx   0        0        0        0 2023-05-05 19:41:02.000000 RobloxPyApi3-2.0.7/
--rw-rw-rw-   0        0        0       61 2023-04-27 12:20:20.000000 RobloxPyApi3-2.0.7/MANIFEST.in
--rw-rw-rw-   0        0        0     2225 2023-05-05 19:41:04.000000 RobloxPyApi3-2.0.7/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-05-05 19:41:02.000000 RobloxPyApi3-2.0.7/RobloxPyApi3/
--rw-rw-rw-   0        0        0    19220 2023-04-27 12:29:54.000000 RobloxPyApi3-2.0.7/RobloxPyApi3/AccountInformation.py
--rw-rw-rw-   0        0        0    15348 2023-05-05 19:16:44.000000 RobloxPyApi3-2.0.7/RobloxPyApi3/Auth.py
--rw-rw-rw-   0        0        0    21919 2023-04-27 12:29:56.000000 RobloxPyApi3-2.0.7/RobloxPyApi3/Avatar.py
--rw-rw-rw-   0        0        0    16287 2023-05-05 19:39:40.000000 RobloxPyApi3-2.0.7/RobloxPyApi3/Captcha.py
--rw-rw-rw-   0        0        0    36825 2023-04-27 12:29:56.000000 RobloxPyApi3-2.0.7/RobloxPyApi3/Catalog.py
--rw-rw-rw-   0        0        0     2739 2023-04-08 19:22:28.000000 RobloxPyApi3-2.0.7/RobloxPyApi3/Check.png
--rw-rw-rw-   0        0        0    18452 2023-04-27 12:29:56.000000 RobloxPyApi3-2.0.7/RobloxPyApi3/Client.py
--rw-rw-rw-   0        0        0     1557 2023-04-12 19:25:10.000000 RobloxPyApi3-2.0.7/RobloxPyApi3/Enums.py
--rw-rw-rw-   0        0        0     2213 2023-04-09 08:16:10.000000 RobloxPyApi3-2.0.7/RobloxPyApi3/Errors.py
--rw-rw-rw-   0        0        0    14748 2023-04-27 12:29:54.000000 RobloxPyApi3-2.0.7/RobloxPyApi3/FriendsAPI.py
--rw-rw-rw-   0        0        0     5938 2023-04-27 12:30:26.000000 RobloxPyApi3-2.0.7/RobloxPyApi3/JoinGame.py
--rw-rw-rw-   0        0        0      461 2023-04-27 12:29:54.000000 RobloxPyApi3-2.0.7/RobloxPyApi3/LeaveGame.py
--rw-rw-rw-   0        0        0     9570 2023-05-05 19:39:40.000000 RobloxPyApi3-2.0.7/RobloxPyApi3/MultiAccount.py
-drwxrwxrwx   0        0        0        0 2023-05-05 19:41:02.000000 RobloxPyApi3-2.0.7/RobloxPyApi3/Place/
--rw-rw-rw-   0        0        0     1977 2023-03-30 08:25:08.000000 RobloxPyApi3-2.0.7/RobloxPyApi3/Place/CallMethods.py
--rw-rw-rw-   0        0        0     3312 2023-04-27 12:29:54.000000 RobloxPyApi3-2.0.7/RobloxPyApi3/Place/Instructions.py
--rw-rw-rw-   0        0        0    26394 2023-04-27 12:29:56.000000 RobloxPyApi3-2.0.7/RobloxPyApi3/Place/Place.py
--rw-rw-rw-   0        0        0      122 2023-04-27 12:29:56.000000 RobloxPyApi3-2.0.7/RobloxPyApi3/Place/__init__.py
--rw-rw-rw-   0        0        0     9691 2023-04-27 12:29:54.000000 RobloxPyApi3-2.0.7/RobloxPyApi3/Place/rbxLua2py.py
--rw-rw-rw-   0        0        0     5550 2023-03-03 16:26:02.000000 RobloxPyApi3-2.0.7/RobloxPyApi3/Place.py
--rw-rw-rw-   0        0        0        0 2023-03-03 14:18:04.000000 RobloxPyApi3-2.0.7/RobloxPyApi3/PlacePropTypes.py
--rw-rw-rw-   0        0        0      505 2023-04-27 12:29:54.000000 RobloxPyApi3-2.0.7/RobloxPyApi3/SessionUtilities.py
--rw-rw-rw-   0        0        0       50 2023-04-15 15:18:22.000000 RobloxPyApi3-2.0.7/RobloxPyApi3/Test.py
--rw-rw-rw-   0        0        0     2762 2023-04-27 12:24:10.000000 RobloxPyApi3-2.0.7/RobloxPyApi3/Utilities.py
--rw-rw-rw-   0        0        0     1594 2023-04-27 13:26:04.000000 RobloxPyApi3-2.0.7/RobloxPyApi3/Version.py
--rw-rw-rw-   0        0        0     1049 2023-05-05 11:47:44.000000 RobloxPyApi3-2.0.7/RobloxPyApi3/__Changes__.py
--rw-rw-rw-   0        0        0    50881 2023-04-27 12:22:44.000000 RobloxPyApi3-2.0.7/RobloxPyApi3/__init__.py
--rw-rw-rw-   0        0        0     4637 2023-04-27 12:29:56.000000 RobloxPyApi3-2.0.7/RobloxPyApi3/friends.py
-drwxrwxrwx   0        0        0        0 2023-05-05 19:41:02.000000 RobloxPyApi3-2.0.7/RobloxPyApi3.egg-info/
--rw-rw-rw-   0        0        0     2225 2023-05-05 19:41:02.000000 RobloxPyApi3-2.0.7/RobloxPyApi3.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      918 2023-05-05 19:41:02.000000 RobloxPyApi3-2.0.7/RobloxPyApi3.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-05 19:41:02.000000 RobloxPyApi3-2.0.7/RobloxPyApi3.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       50 2023-05-05 19:41:02.000000 RobloxPyApi3-2.0.7/RobloxPyApi3.egg-info/requires.txt
--rw-rw-rw-   0        0        0       13 2023-05-05 19:41:02.000000 RobloxPyApi3-2.0.7/RobloxPyApi3.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-05 19:41:04.000000 RobloxPyApi3-2.0.7/setup.cfg
--rw-rw-rw-   0        0        0     2714 2023-05-05 19:40:52.000000 RobloxPyApi3-2.0.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-05 19:55:02.000000 RobloxPyApi3-2.0.722/
+-rw-rw-rw-   0        0        0       61 2023-04-27 12:20:20.000000 RobloxPyApi3-2.0.722/MANIFEST.in
+-rw-rw-rw-   0        0        0     2227 2023-05-05 19:55:02.000000 RobloxPyApi3-2.0.722/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-05-05 19:55:02.000000 RobloxPyApi3-2.0.722/RobloxPyApi3/
+-rw-rw-rw-   0        0        0    19220 2023-04-27 12:29:54.000000 RobloxPyApi3-2.0.722/RobloxPyApi3/AccountInformation.py
+-rw-rw-rw-   0        0        0    15348 2023-05-05 19:16:44.000000 RobloxPyApi3-2.0.722/RobloxPyApi3/Auth.py
+-rw-rw-rw-   0        0        0    21919 2023-04-27 12:29:56.000000 RobloxPyApi3-2.0.722/RobloxPyApi3/Avatar.py
+-rw-rw-rw-   0        0        0    16389 2023-05-05 19:54:48.000000 RobloxPyApi3-2.0.722/RobloxPyApi3/Captcha.py
+-rw-rw-rw-   0        0        0    36825 2023-04-27 12:29:56.000000 RobloxPyApi3-2.0.722/RobloxPyApi3/Catalog.py
+-rw-rw-rw-   0        0        0     2739 2023-04-08 19:22:28.000000 RobloxPyApi3-2.0.722/RobloxPyApi3/Check.png
+-rw-rw-rw-   0        0        0    18452 2023-04-27 12:29:56.000000 RobloxPyApi3-2.0.722/RobloxPyApi3/Client.py
+-rw-rw-rw-   0        0        0     1557 2023-04-12 19:25:10.000000 RobloxPyApi3-2.0.722/RobloxPyApi3/Enums.py
+-rw-rw-rw-   0        0        0     2213 2023-04-09 08:16:10.000000 RobloxPyApi3-2.0.722/RobloxPyApi3/Errors.py
+-rw-rw-rw-   0        0        0    14748 2023-04-27 12:29:54.000000 RobloxPyApi3-2.0.722/RobloxPyApi3/FriendsAPI.py
+-rw-rw-rw-   0        0        0     5938 2023-04-27 12:30:26.000000 RobloxPyApi3-2.0.722/RobloxPyApi3/JoinGame.py
+-rw-rw-rw-   0        0        0      461 2023-04-27 12:29:54.000000 RobloxPyApi3-2.0.722/RobloxPyApi3/LeaveGame.py
+-rw-rw-rw-   0        0        0     9570 2023-05-05 19:39:40.000000 RobloxPyApi3-2.0.722/RobloxPyApi3/MultiAccount.py
+drwxrwxrwx   0        0        0        0 2023-05-05 19:55:02.000000 RobloxPyApi3-2.0.722/RobloxPyApi3/Place/
+-rw-rw-rw-   0        0        0     1977 2023-03-30 08:25:08.000000 RobloxPyApi3-2.0.722/RobloxPyApi3/Place/CallMethods.py
+-rw-rw-rw-   0        0        0     3312 2023-04-27 12:29:54.000000 RobloxPyApi3-2.0.722/RobloxPyApi3/Place/Instructions.py
+-rw-rw-rw-   0        0        0    26394 2023-04-27 12:29:56.000000 RobloxPyApi3-2.0.722/RobloxPyApi3/Place/Place.py
+-rw-rw-rw-   0        0        0      122 2023-04-27 12:29:56.000000 RobloxPyApi3-2.0.722/RobloxPyApi3/Place/__init__.py
+-rw-rw-rw-   0        0        0     9691 2023-04-27 12:29:54.000000 RobloxPyApi3-2.0.722/RobloxPyApi3/Place/rbxLua2py.py
+-rw-rw-rw-   0        0        0     5550 2023-03-03 16:26:02.000000 RobloxPyApi3-2.0.722/RobloxPyApi3/Place.py
+-rw-rw-rw-   0        0        0        0 2023-03-03 14:18:04.000000 RobloxPyApi3-2.0.722/RobloxPyApi3/PlacePropTypes.py
+-rw-rw-rw-   0        0        0      505 2023-04-27 12:29:54.000000 RobloxPyApi3-2.0.722/RobloxPyApi3/SessionUtilities.py
+-rw-rw-rw-   0        0        0       50 2023-04-15 15:18:22.000000 RobloxPyApi3-2.0.722/RobloxPyApi3/Test.py
+-rw-rw-rw-   0        0        0     2762 2023-04-27 12:24:10.000000 RobloxPyApi3-2.0.722/RobloxPyApi3/Utilities.py
+-rw-rw-rw-   0        0        0     1594 2023-04-27 13:26:04.000000 RobloxPyApi3-2.0.722/RobloxPyApi3/Version.py
+-rw-rw-rw-   0        0        0     1049 2023-05-05 11:47:44.000000 RobloxPyApi3-2.0.722/RobloxPyApi3/__Changes__.py
+-rw-rw-rw-   0        0        0    50881 2023-04-27 12:22:44.000000 RobloxPyApi3-2.0.722/RobloxPyApi3/__init__.py
+-rw-rw-rw-   0        0        0     4637 2023-04-27 12:29:56.000000 RobloxPyApi3-2.0.722/RobloxPyApi3/friends.py
+drwxrwxrwx   0        0        0        0 2023-05-05 19:55:02.000000 RobloxPyApi3-2.0.722/RobloxPyApi3.egg-info/
+-rw-rw-rw-   0        0        0     2227 2023-05-05 19:55:00.000000 RobloxPyApi3-2.0.722/RobloxPyApi3.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      918 2023-05-05 19:55:02.000000 RobloxPyApi3-2.0.722/RobloxPyApi3.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-05 19:55:02.000000 RobloxPyApi3-2.0.722/RobloxPyApi3.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       60 2023-05-05 19:55:02.000000 RobloxPyApi3-2.0.722/RobloxPyApi3.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       13 2023-05-05 19:55:02.000000 RobloxPyApi3-2.0.722/RobloxPyApi3.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-05 19:55:02.000000 RobloxPyApi3-2.0.722/setup.cfg
+-rw-rw-rw-   0        0        0     2728 2023-05-05 19:54:46.000000 RobloxPyApi3-2.0.722/setup.py
```

### Comparing `RobloxPyApi3-2.0.7/PKG-INFO` & `RobloxPyApi3-2.0.722/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: RobloxPyApi3
-Version: 2.0.7
+Version: 2.0.722
 Summary: RobloxPyApi3 is a Python API controller for Roblox, offering API wrapping, multi-account management, and more. Create and manage Roblox accounts and Places with ease.
 Author: pyProjects3 (github.com/pyProjects3)
 License: MIT
 Keywords: Roblox,Api,wrapper,Bot,Client,Automated,Account Management,rbx,Python3,Place automation,post requests,get requests,JSON,Authorization,Roblox Development
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `RobloxPyApi3-2.0.7/RobloxPyApi3/AccountInformation.py` & `RobloxPyApi3-2.0.722/RobloxPyApi3/AccountInformation.py`

 * *Files identical despite different names*

### Comparing `RobloxPyApi3-2.0.7/RobloxPyApi3/Auth.py` & `RobloxPyApi3-2.0.722/RobloxPyApi3/Auth.py`

 * *Files identical despite different names*

### Comparing `RobloxPyApi3-2.0.7/RobloxPyApi3/Avatar.py` & `RobloxPyApi3-2.0.722/RobloxPyApi3/Avatar.py`

 * *Files identical despite different names*

### Comparing `RobloxPyApi3-2.0.7/RobloxPyApi3/Captcha.py` & `RobloxPyApi3-2.0.722/RobloxPyApi3/Captcha.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 import requests
 import random
 import time
 import webbrowser as WEB
 import pyautogui
 import base64
 import json
+import os
 class Captcha:
     def __init__(self,CaptchaRequiredRobloxAPI,data,Headers,WaitAfterComplete = 4.5,CaptchaType = "A2A14B1D-1AF3-C791-9BBC-EE33CC7A0A6F"):
         self.URL = CaptchaRequiredRobloxAPI
         self.Token = None
         self.ID = None
         self.blob = None
         self.TokenID = None
@@ -299,19 +300,20 @@
                 #f'- Received Captcha Details!\n\n\nCaptchaId : {self.ID}\nCaptchaBlob : {self.blob}\nLocation : {self.location}\ntoken : {self.TokenID}\n\n\n(Starting selenium browser to solve the captcha)..\n\n\n')
             print("[INFO] Starting Web browser to solve the captcha.")
             time.sleep(1)
             WEB.open(solver_url)
             time.sleep(1)
 
             image = 'Check.png'
-
+            d = os.path.dirname(os.path.realpath(__file__))
+            p = os.path.join(d,'Check.png')
             while True:
                 try:
                     # locate the image on the screen
-                    location = pyautogui.locateOnScreen(".//Check.png")
+                    location = pyautogui.locateOnScreen(p)
 
                     # if the image is found, break the loop and continue the script
                     if location is not None:
                         break
                 except Exception:
                     # if any exception occurs, continue the loop
                     pass
```

### Comparing `RobloxPyApi3-2.0.7/RobloxPyApi3/Catalog.py` & `RobloxPyApi3-2.0.722/RobloxPyApi3/Catalog.py`

 * *Files identical despite different names*

### Comparing `RobloxPyApi3-2.0.7/RobloxPyApi3/Check.png` & `RobloxPyApi3-2.0.722/RobloxPyApi3/Check.png`

 * *Files identical despite different names*

### Comparing `RobloxPyApi3-2.0.7/RobloxPyApi3/Client.py` & `RobloxPyApi3-2.0.722/RobloxPyApi3/Client.py`

 * *Files identical despite different names*

### Comparing `RobloxPyApi3-2.0.7/RobloxPyApi3/Enums.py` & `RobloxPyApi3-2.0.722/RobloxPyApi3/Enums.py`

 * *Files identical despite different names*

### Comparing `RobloxPyApi3-2.0.7/RobloxPyApi3/Errors.py` & `RobloxPyApi3-2.0.722/RobloxPyApi3/Errors.py`

 * *Files identical despite different names*

### Comparing `RobloxPyApi3-2.0.7/RobloxPyApi3/FriendsAPI.py` & `RobloxPyApi3-2.0.722/RobloxPyApi3/FriendsAPI.py`

 * *Files identical despite different names*

### Comparing `RobloxPyApi3-2.0.7/RobloxPyApi3/JoinGame.py` & `RobloxPyApi3-2.0.722/RobloxPyApi3/JoinGame.py`

 * *Files identical despite different names*

### Comparing `RobloxPyApi3-2.0.7/RobloxPyApi3/MultiAccount.py` & `RobloxPyApi3-2.0.722/RobloxPyApi3/MultiAccount.py`

 * *Files identical despite different names*

### Comparing `RobloxPyApi3-2.0.7/RobloxPyApi3/Place/CallMethods.py` & `RobloxPyApi3-2.0.722/RobloxPyApi3/Place/CallMethods.py`

 * *Files identical despite different names*

### Comparing `RobloxPyApi3-2.0.7/RobloxPyApi3/Place/Instructions.py` & `RobloxPyApi3-2.0.722/RobloxPyApi3/Place/Instructions.py`

 * *Files identical despite different names*

### Comparing `RobloxPyApi3-2.0.7/RobloxPyApi3/Place/Place.py` & `RobloxPyApi3-2.0.722/RobloxPyApi3/Place/Place.py`

 * *Files identical despite different names*

### Comparing `RobloxPyApi3-2.0.7/RobloxPyApi3/Place/rbxLua2py.py` & `RobloxPyApi3-2.0.722/RobloxPyApi3/Place/rbxLua2py.py`

 * *Files identical despite different names*

### Comparing `RobloxPyApi3-2.0.7/RobloxPyApi3/Place.py` & `RobloxPyApi3-2.0.722/RobloxPyApi3/Place.py`

 * *Files identical despite different names*

### Comparing `RobloxPyApi3-2.0.7/RobloxPyApi3/Utilities.py` & `RobloxPyApi3-2.0.722/RobloxPyApi3/Utilities.py`

 * *Files identical despite different names*

### Comparing `RobloxPyApi3-2.0.7/RobloxPyApi3/Version.py` & `RobloxPyApi3-2.0.722/RobloxPyApi3/Version.py`

 * *Files identical despite different names*

### Comparing `RobloxPyApi3-2.0.7/RobloxPyApi3/__Changes__.py` & `RobloxPyApi3-2.0.722/RobloxPyApi3/__Changes__.py`

 * *Files identical despite different names*

### Comparing `RobloxPyApi3-2.0.7/RobloxPyApi3/__init__.py` & `RobloxPyApi3-2.0.722/RobloxPyApi3/__init__.py`

 * *Files identical despite different names*

### Comparing `RobloxPyApi3-2.0.7/RobloxPyApi3/friends.py` & `RobloxPyApi3-2.0.722/RobloxPyApi3/friends.py`

 * *Files identical despite different names*

### Comparing `RobloxPyApi3-2.0.7/RobloxPyApi3.egg-info/PKG-INFO` & `RobloxPyApi3-2.0.722/RobloxPyApi3.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: RobloxPyApi3
-Version: 2.0.7
+Version: 2.0.722
 Summary: RobloxPyApi3 is a Python API controller for Roblox, offering API wrapping, multi-account management, and more. Create and manage Roblox accounts and Places with ease.
 Author: pyProjects3 (github.com/pyProjects3)
 License: MIT
 Keywords: Roblox,Api,wrapper,Bot,Client,Automated,Account Management,rbx,Python3,Place automation,post requests,get requests,JSON,Authorization,Roblox Development
 Classifier: Development Status :: 1 - Planning
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
```

### Comparing `RobloxPyApi3-2.0.7/RobloxPyApi3.egg-info/SOURCES.txt` & `RobloxPyApi3-2.0.722/RobloxPyApi3.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `RobloxPyApi3-2.0.7/setup.py` & `RobloxPyApi3-2.0.722/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 from setuptools import setup, find_packages
 from RobloxPyApi3.Version import __Copyright__
-Version = "2.0.7"
+Version = "2.0.722"
 
 Description = "RobloxPyApi3 is a Python API controller for Roblox, offering API wrapping, multi-account management, and more. Create and manage Roblox accounts and Places with ease."
 
 Long_Description = f"""
 Welcome to the RobloxPyAPI3 package, created by pyProjects3. This package is designed to make Roblox game development possible in python, API Wrapper (Access Roblox API), Multi Account management and being able to join games and leave games.
 
 One of the key features of this package is its support for Place creation. With our Place creation tools, you can now create your Roblox Places in python, whether you're working on a personal project or developing a game with a team. Our tools make it easy to upload new assets, manage permissions, and more.
@@ -25,15 +25,15 @@
     long_description_content_type="text/markdown",
     long_description=Long_Description,
     packages=find_packages(),
     license="MIT",
 
     package_data= {'Place':["*.py"]},
     include_package_data=True,
-    install_requires=['requests','colorama','psutil','RobloxPyApi3Update','enums'],
+    install_requires=['requests','colorama','psutil','RobloxPyApi3Update','enums',"pyautogui"],
     keywords=["Roblox","Api",'wrapper',"Bot",'Client','Automated',"Account Management","rbx","Python3","Place automation","post requests","get requests","JSON","Authorization","Roblox Development"],
     classifiers=[
         "Development Status :: 1 - Planning",
         "Intended Audience :: Developers",
         "Programming Language :: Python :: 3",
         "Operating System :: Microsoft :: Windows",
     ]
```

